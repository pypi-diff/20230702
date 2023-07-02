# Comparing `tmp/kaiju_redis-2.1.3-py3-none-any.whl.zip` & `tmp/kaiju_redis-2.1.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 8984 bytes, number of entries: 10
--rw-r--r--  2.0 unx      110 b- defN 23-Jun-30 16:33 kaiju_redis/__init__.py
--rw-r--r--  2.0 unx    14924 b- defN 23-Jun-30 16:33 kaiju_redis/services.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-30 16:33 kaiju_redis/tests/__init__.py
--rw-r--r--  2.0 unx     2956 b- defN 23-Jun-30 16:33 kaiju_redis/tests/fixtures.py
--rw-r--r--  2.0 unx     4086 b- defN 23-Jun-30 16:33 kaiju_redis/tests/test_redis.py
--rw-rw-rw-  2.0 unx      610 b- defN 23-Jun-30 16:33 kaiju_redis-2.1.3.dist-info/LICENSE
--rw-r--r--  2.0 unx     3002 b- defN 23-Jun-30 16:33 kaiju_redis-2.1.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-30 16:33 kaiju_redis-2.1.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 23-Jun-30 16:33 kaiju_redis-2.1.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      822 b- defN 23-Jun-30 16:33 kaiju_redis-2.1.3.dist-info/RECORD
-10 files, 26614 bytes uncompressed, 7574 bytes compressed:  71.5%
+Zip file size: 8999 bytes, number of entries: 10
+-rw-r--r--  2.0 unx      110 b- defN 23-Jul-02 12:45 kaiju_redis/__init__.py
+-rw-r--r--  2.0 unx    14894 b- defN 23-Jul-02 12:45 kaiju_redis/services.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-02 12:45 kaiju_redis/tests/__init__.py
+-rw-r--r--  2.0 unx     2956 b- defN 23-Jul-02 12:45 kaiju_redis/tests/fixtures.py
+-rw-r--r--  2.0 unx     4086 b- defN 23-Jul-02 12:45 kaiju_redis/tests/test_redis.py
+-rw-rw-rw-  2.0 unx      610 b- defN 23-Jul-02 12:45 kaiju_redis-2.1.4.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3002 b- defN 23-Jul-02 12:45 kaiju_redis-2.1.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-02 12:45 kaiju_redis-2.1.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 23-Jul-02 12:45 kaiju_redis-2.1.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      822 b- defN 23-Jul-02 12:45 kaiju_redis-2.1.4.dist-info/RECORD
+10 files, 26584 bytes uncompressed, 7589 bytes compressed:  71.5%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: kaiju_redis/tests/fixtures.py
 Comment: 
 
 Filename: kaiju_redis/tests/test_redis.py
 Comment: 
 
-Filename: kaiju_redis-2.1.3.dist-info/LICENSE
+Filename: kaiju_redis-2.1.4.dist-info/LICENSE
 Comment: 
 
-Filename: kaiju_redis-2.1.3.dist-info/METADATA
+Filename: kaiju_redis-2.1.4.dist-info/METADATA
 Comment: 
 
-Filename: kaiju_redis-2.1.3.dist-info/WHEEL
+Filename: kaiju_redis-2.1.4.dist-info/WHEEL
 Comment: 
 
-Filename: kaiju_redis-2.1.3.dist-info/top_level.txt
+Filename: kaiju_redis-2.1.4.dist-info/top_level.txt
 Comment: 
 
-Filename: kaiju_redis-2.1.3.dist-info/RECORD
+Filename: kaiju_redis-2.1.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## kaiju_redis/__init__.py

```diff
@@ -1,5 +1,5 @@
 from .services import *
 
-__version__ = '2.1.3'
+__version__ = '2.1.4'
 __python_version__ = '3.8'
 __author__ = 'antonnidhoggr@me.com'
```

## kaiju_redis/services.py

```diff
@@ -2,15 +2,15 @@
 
 import textwrap
 from typing import Collection, FrozenSet, Type, List
 
 from coredis import Redis, RedisCluster  # noqa: pycharm
 from coredis.exceptions import ResponseError, StreamConsumerGroupError  # noqa: pycharm
 
-from kaiju_tools.app import ContextableService, service_class_registry
+from kaiju_tools.app import ContextableService, SERVICE_CLASS_REGISTRY
 from kaiju_tools.cache import BaseCacheService
 from kaiju_tools.encoding import msgpack_dumps, msgpack_loads
 from kaiju_tools.functions import retry
 from kaiju_tools.locks import BaseLocksService, NotLockOwnerError, LockExistsError
 from kaiju_tools.streams import StreamRPCClient, Listener
 from kaiju_tools.types import NSKey
 
@@ -426,12 +426,12 @@
         :param body: rpc request body
         :param headers: request headers
         :param key: (optional) message id
         """
         await self._transport.xadd(topic, {b'_': self._dumps((body, headers))}, identifier=key if key else '*')
 
 
-service_class_registry.register_class(RedisTransportService)
-service_class_registry.register_class(RedisCacheService)
-service_class_registry.register_class(RedisLocksService)
-service_class_registry.register_class(RedisListener)
-service_class_registry.register_class(RedisStreamRPCClient)
+SERVICE_CLASS_REGISTRY.register(RedisTransportService)
+SERVICE_CLASS_REGISTRY.register(RedisCacheService)
+SERVICE_CLASS_REGISTRY.register(RedisLocksService)
+SERVICE_CLASS_REGISTRY.register(RedisListener)
+SERVICE_CLASS_REGISTRY.register(RedisStreamRPCClient)
```

## Comparing `kaiju_redis-2.1.3.dist-info/LICENSE` & `kaiju_redis-2.1.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `kaiju_redis-2.1.3.dist-info/METADATA` & `kaiju_redis-2.1.4.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kaiju-redis
-Version: 2.1.3
+Version: 2.1.4
 Summary: Redis and keydb services
 Home-page: https://gitlab.com/kaiju-python/kaiju-redis
 Author: antonnidhoggr@me.com
 Author-email: antonnidhoggr@me.com
 License: Apache Software License 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
```

## Comparing `kaiju_redis-2.1.3.dist-info/RECORD` & `kaiju_redis-2.1.4.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-kaiju_redis/__init__.py,sha256=JmtJgmAL4CtiRhvOhSOMEnjSvETVkulGQZ6jdJbffbM,110
-kaiju_redis/services.py,sha256=dMWkjranM-GPLkOR68THufqPyz7P3p1-F6MKVfwvA04,14924
+kaiju_redis/__init__.py,sha256=GbveAxfFie7WR4l0-ZEZQX5pX1f98fV-MIQ_VL_1304,110
+kaiju_redis/services.py,sha256=Xu-sQXiilGnHTUqnfPF2pnn6VG5fRuTFrMrqqXcJePg,14894
 kaiju_redis/tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 kaiju_redis/tests/fixtures.py,sha256=YDaJxKaEmbPQyi64x0o-dxDwK9JE90hdzUxbEc6QkEk,2956
 kaiju_redis/tests/test_redis.py,sha256=Mu5hl5EYY5mEkXxU7TeXVYBsxh6ZiV59X1ovYqP68BE,4086
-kaiju_redis-2.1.3.dist-info/LICENSE,sha256=XIlN2qA8UqpBDA-PteoYP4hTU0qBW0G9PRB__khO2zc,610
-kaiju_redis-2.1.3.dist-info/METADATA,sha256=q3v5tNQH3ZDW-tKrQ8hIaGW7CuQ7Eh_6ZNJqShSVMu4,3002
-kaiju_redis-2.1.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-kaiju_redis-2.1.3.dist-info/top_level.txt,sha256=-4Sc1VXkNcLW_b2uQWx-BICdwMu_NTUwDmt_q_SxB1Q,12
-kaiju_redis-2.1.3.dist-info/RECORD,,
+kaiju_redis-2.1.4.dist-info/LICENSE,sha256=XIlN2qA8UqpBDA-PteoYP4hTU0qBW0G9PRB__khO2zc,610
+kaiju_redis-2.1.4.dist-info/METADATA,sha256=Lrakp3Z-xqAQ7si4mV6y-X_5OaEV4hwiu4NM1vYNq5U,3002
+kaiju_redis-2.1.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+kaiju_redis-2.1.4.dist-info/top_level.txt,sha256=-4Sc1VXkNcLW_b2uQWx-BICdwMu_NTUwDmt_q_SxB1Q,12
+kaiju_redis-2.1.4.dist-info/RECORD,,
```

