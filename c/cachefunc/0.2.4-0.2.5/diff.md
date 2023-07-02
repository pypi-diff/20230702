# Comparing `tmp/cachefunc-0.2.4.tar.gz` & `tmp/cachefunc-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cachefunc-0.2.4.tar", max compression
+gzip compressed data, was "cachefunc-0.2.5.tar", max compression
```

## Comparing `cachefunc-0.2.4.tar` & `cachefunc-0.2.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      182 2023-07-01 20:38:06.456807 cachefunc-0.2.4/README.md
--rw-r--r--   0        0        0      222 2023-07-01 20:11:47.197988 cachefunc-0.2.4/cachefunc/__init__.py
--rw-r--r--   0        0        0     2181 2023-07-01 20:11:47.198253 cachefunc-0.2.4/cachefunc/cache/base.py
--rw-r--r--   0        0        0      919 2023-07-01 20:11:47.198477 cachefunc-0.2.4/cachefunc/cache/dict_cache.py
--rw-r--r--   0        0        0      592 2023-07-01 20:36:16.521857 cachefunc-0.2.4/cachefunc/cache/redis_cache.py
--rw-r--r--   0        0        0      680 2023-07-01 20:19:20.506787 cachefunc-0.2.4/cachefunc/log.py
--rw-r--r--   0        0        0     1190 2023-07-01 20:25:52.221635 cachefunc-0.2.4/cachefunc/main.py
--rw-r--r--   0        0        0      394 2023-07-01 20:39:18.909786 cachefunc-0.2.4/pyproject.toml
--rw-r--r--   0        0        0      742 1970-01-01 00:00:00.000000 cachefunc-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0     1734 2023-07-02 14:10:32.741223 cachefunc-0.2.5/README.md
+-rw-r--r--   0        0        0      222 2023-07-01 20:11:47.197988 cachefunc-0.2.5/cachefunc/__init__.py
+-rw-r--r--   0        0        0     1680 2023-07-02 13:49:54.101540 cachefunc-0.2.5/cachefunc/cache/base.py
+-rw-r--r--   0        0        0      865 2023-07-02 13:50:55.496357 cachefunc-0.2.5/cachefunc/cache/dict_cache.py
+-rw-r--r--   0        0        0      545 2023-07-02 13:50:48.773435 cachefunc-0.2.5/cachefunc/cache/redis_cache.py
+-rw-r--r--   0        0        0      680 2023-07-01 20:19:20.506787 cachefunc-0.2.5/cachefunc/log.py
+-rw-r--r--   0        0        0     1190 2023-07-01 20:25:52.221635 cachefunc-0.2.5/cachefunc/main.py
+-rw-r--r--   0        0        0      394 2023-07-02 14:08:34.340523 cachefunc-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0     2294 1970-01-01 00:00:00.000000 cachefunc-0.2.5/PKG-INFO
```

### Comparing `cachefunc-0.2.4/cachefunc/cache/base.py` & `cachefunc-0.2.5/cachefunc/cache/base.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from __future__ import annotations
 
 
 from dataclasses import dataclass
-from datetime import timedelta
-from typing import Any, Callable, Coroutine, Dict, Hashable, Tuple, Union
+from typing import Any, Callable, Coroutine, Dict, Tuple, Union
 from uuid import uuid4
 
 from cachefunc.log import get_logger
 
 
 logger = get_logger(__name__)
 
@@ -23,58 +22,45 @@
 
     def __str__(self) -> str:
         return (
             f'{self.func.__qualname__}; '
             f'args: {self.func_args}; '
             f'kwargs {self.func_kwargs}'
         )
-
-    def __eq__(self, other: FuncCall) -> bool:
-        return (
-            self.func == other.func and
-            self.func_args == other.func_args and
-            self.func_kwargs == other.func_kwargs
+    
+    def to_key(self) -> int:
+        return hash(
+            self.func.__qualname__ +
+            ''.join(str(id(v)) for v in self.func_args) +
+            ''.join(str(id(v)) for v in self.func_kwargs.values())
         )
 
 
 class BaseCache:
-    def __init__(self):
-        self.__func_call_registry = dict()
-
     def get(
         self,
         func: Union[Callable, Coroutine],
         func_args: Tuple[Any],
         func_kwargs: Dict[str, Any],
     ) -> None:
         func_call = FuncCall(func, func_args, func_kwargs)
-        if key := self._get_key(func_call):
-            logger.info(f'Found data in cache for function call: {func_call}')
-            return self._get(key)
-        raise NotCached
+        key = func_call.to_key()
+        result = self._get(key)
+        logger.info(f'Found data in cache for function call: {func_call}')
+        return result
 
     def set(
         self,
         func: Union[Callable, Coroutine],
         func_args: Tuple[Any],
         func_kwargs: Dict[str, Any],
         result: Any,
         **kwargs,
     ) -> None:
         func_call = FuncCall(func, func_args, func_kwargs)
         logger.info(f'No data was found in cache, call function: {func_call}')
-        key = self._set_key(func_call)
+        key = func_call.to_key()
         self._set(key, result, **kwargs)
 
-    def _get_key(self, func_call: FuncCall) -> Hashable:
-        for key, registered_func_call in self.__func_call_registry.items():
-            if func_call == registered_func_call:
-                return key
-        
-    def _set_key(self, func_call: FuncCall) -> Hashable:
-        key = uuid4()
-        self.__func_call_registry[key] = func_call
-        return key
-
-    def _get(self, key: Hashable) -> Any: ...
+    def _get(self, key: int) -> Any: ...
 
-    def _set(self, key: Hashable, result: Any, **kwargs) -> None: ...
+    def _set(self, key: int, result: Any, **kwargs) -> None: ...
```

### Comparing `cachefunc-0.2.4/cachefunc/cache/dict_cache.py` & `cachefunc-0.2.5/cachefunc/cache/dict_cache.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 from contextlib import suppress
 from datetime import datetime, timedelta
-from typing import Any, Hashable, Union
+from typing import Any
 
 from cachefunc.cache.base import BaseCache, NotCached
 
 
 class DictCache(BaseCache):
     DEFAULT_TIMEOUT = timedelta(hours=1)
 
     def __init__(self):
-        super().__init__()
         self.cache = dict()
 
     def clear(self) -> None:
         self.cache.clear()
 
-    def _get(self, key: Hashable) -> Any:
+    def _get(self, key: int) -> Any:
         with suppress(KeyError):
             return self.cache[key][0]
         raise NotCached()
     
-    def _set(self, key: Hashable, result: Any, **kwargs) -> None:
+    def _set(self, key: int, result: Any, **kwargs) -> None:
         timeout = kwargs.get('timeout', self.DEFAULT_TIMEOUT)
         self._clear_expired()
         self.cache[key] = (result, datetime.now() + timeout)
 
     def _clear_expired(self) -> None:
         now = datetime.now()
         for key, data in self.cache.items():
```

### Comparing `cachefunc-0.2.4/cachefunc/cache/redis_cache.py` & `cachefunc-0.2.5/cachefunc/cache/redis_cache.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 from pickle import loads, dumps
 from redis import Redis
-from typing import Any, Hashable
+from typing import Any
 
 from cachefunc.cache.base import BaseCache, NotCached
 
 
 class RedisCache(BaseCache):
     def __init__(self, host: str = 'localhost', port: int = 6379, db: int = 0):
-        super().__init__()
         self.redis = Redis(host, port, db)
 
-    def _get(self, key: Hashable) -> Any:
+    def _get(self, key: int) -> Any:
         if (result := self.redis.get(key)) is not None:
             return loads(result)
         raise NotCached()
 
-    def _set(self, key: Hashable, result: Any, **kwargs) -> None:
+    def _set(self, key: int, result: Any, **kwargs) -> None:
         self.redis.set(key, dumps(result))
```

### Comparing `cachefunc-0.2.4/cachefunc/log.py` & `cachefunc-0.2.5/cachefunc/log.py`

 * *Files identical despite different names*

### Comparing `cachefunc-0.2.4/cachefunc/main.py` & `cachefunc-0.2.5/cachefunc/main.py`

 * *Files identical despite different names*

