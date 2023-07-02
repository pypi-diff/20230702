# Comparing `tmp/mbnk-0.0.7.tar.gz` & `tmp/mbnk-0.1.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mbnk-0.0.7.tar", max compression
+gzip compressed data, was "mbnk-0.1.0a0.tar", max compression
```

## Comparing `mbnk-0.0.7.tar` & `mbnk-0.1.0a0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      692 2023-05-05 16:01:16.349631 mbnk-0.0.7/README.md
--rw-r--r--   0        0        0      290 2023-06-29 11:51:13.889758 mbnk-0.0.7/mbnk/__init__.py
--rw-r--r--   0        0        0      108 2023-06-26 17:49:44.968379 mbnk-0.0.7/mbnk/asyncio/__init__.py
--rw-r--r--   0        0        0     5341 2023-06-29 22:12:37.821115 mbnk-0.0.7/mbnk/asyncio/mbnk.py
--rw-r--r--   0        0        0     2014 2023-06-26 20:24:53.337731 mbnk-0.0.7/mbnk/decorators.py
--rw-r--r--   0        0        0     1031 2023-06-26 19:21:25.551426 mbnk-0.0.7/mbnk/enums.py
--rw-r--r--   0        0        0        0 2023-06-26 17:26:19.588213 mbnk-0.0.7/mbnk/exceptions.py
--rw-r--r--   0        0        0       24 2023-05-05 14:27:50.660629 mbnk-0.0.7/mbnk/instances/__init__.py
--rw-r--r--   0        0        0     1027 2023-05-05 15:24:33.653100 mbnk-0.0.7/mbnk/instances/instances.py
--rw-r--r--   0        0        0     6498 2023-06-26 17:52:49.728848 mbnk-0.0.7/mbnk/monobank.py
--rw-r--r--   0        0        0      554 2023-05-05 15:32:04.350739 mbnk-0.0.7/mbnk/responses.py
--rw-r--r--   0        0        0      104 2023-05-05 14:19:51.878618 mbnk-0.0.7/mbnk/utils/__init__.py
--rw-r--r--   0        0        0      276 2023-06-26 19:48:53.018019 mbnk-0.0.7/mbnk/utils/builders.py
--rw-r--r--   0        0        0      152 2023-06-26 16:15:25.376467 mbnk-0.0.7/mbnk/utils/is_exception.py
--rw-r--r--   0        0        0      141 2023-06-26 16:51:30.107547 mbnk-0.0.7/mbnk/utils/to_camel_case.py
--rw-r--r--   0        0        0      505 2023-05-01 23:52:09.567523 mbnk-0.0.7/mbnk/utils/webhook_authentication.py
--rw-r--r--   0        0        0      313 2023-06-29 22:12:43.317089 mbnk-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     1223 1970-01-01 00:00:00.000000 mbnk-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1420 2023-07-02 05:05:53.695059 mbnk-0.1.0a0/README.md
+-rw-r--r--   0        0        0      359 2023-07-02 05:26:34.519609 mbnk-0.1.0a0/mbnk/__init__.py
+-rw-r--r--   0        0        0    14803 2023-07-02 18:44:15.060560 mbnk-0.1.0a0/mbnk/api.py
+-rw-r--r--   0        0        0      101 2023-07-02 05:26:15.783700 mbnk-0.1.0a0/mbnk/asyncio/__init__.py
+-rw-r--r--   0        0        0      323 2023-07-02 17:30:10.132706 mbnk-0.1.0a0/mbnk/asyncio/mbnk.py
+-rw-r--r--   0        0        0     2710 2023-07-02 17:32:57.818194 mbnk-0.1.0a0/mbnk/decorators.py
+-rw-r--r--   0        0        0     1697 2023-07-02 05:20:44.513374 mbnk-0.1.0a0/mbnk/enums.py
+-rw-r--r--   0        0        0      300 2023-07-02 01:07:19.623331 mbnk-0.1.0a0/mbnk/exceptions.py
+-rw-r--r--   0        0        0     2164 2023-07-02 18:13:15.452507 mbnk-0.1.0a0/mbnk/instances.py
+-rw-r--r--   0        0        0      315 2023-07-02 18:14:01.695715 mbnk-0.1.0a0/mbnk/mbnk.py
+-rw-r--r--   0        0        0     2217 2023-07-01 23:15:46.030057 mbnk-0.1.0a0/mbnk/responses.py
+-rw-r--r--   0        0        0       97 2023-07-01 23:23:24.859301 mbnk-0.1.0a0/mbnk/utils/__init__.py
+-rw-r--r--   0        0        0      269 2023-07-01 23:23:25.011300 mbnk-0.1.0a0/mbnk/utils/builders.py
+-rw-r--r--   0        0        0      839 2023-07-02 18:14:30.643213 mbnk-0.1.0a0/mbnk/utils/format.py
+-rw-r--r--   0        0        0      389 2023-07-02 01:04:35.544706 mbnk-0.1.0a0/mbnk/utils/is_exception.py
+-rw-r--r--   0        0        0      466 2023-07-01 22:05:58.624489 mbnk-0.1.0a0/mbnk/utils/webhook.py
+-rw-r--r--   0        0        0      315 2023-07-02 18:55:37.617760 mbnk-0.1.0a0/pyproject.toml
+-rw-r--r--   0        0        0     1953 1970-01-01 00:00:00.000000 mbnk-0.1.0a0/PKG-INFO
```

### Comparing `mbnk-0.0.7/mbnk/decorators.py` & `mbnk-0.1.0a0/mbnk/decorators.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,69 +1,97 @@
-import aiohttp
 import json
-from mbnk.utils import data_builder
+import requests
 
+from aiohttp import ClientSession
 
-def async_get_request(url):
-    def outer(func):
-        async def inner(self, *args, **kwargs):
-            params = data_builder(**kwargs)
-
-            async with aiohttp.ClientSession() as session:
-                async with session.get(
-                    url=url.format(
-                        base_url=self.__base_url__
-                    ),
-                    headers=self.__headers__,
-                    params=params
-                ) as response:
-                    response_data = await response.json()
+from mbnk.utils import data_builder, is_exception
+from mbnk.utils.format import convert_json, camel_to_underscore
+from mbnk.exceptions import MonoPayAPIException, MonobankAPIException
+
+
+def api_request(
+        method: str,
+        url: str,
+        headers: dict,
+        data: str = None,
+        params: str = None
+):
+    request = getattr(requests, method)
+    response = request(
+        url=url,
+        headers=headers,
+        data=json.dumps(data) if data is not None else None,
+        params=params
+    )
+
+    response_data = response.json()
+    response_data = convert_json(response_data, camel_to_underscore)
+
+    if is_exception(response):
+        return MonoPayAPIException(**response_data)
+
+    return response_data
+
+
+async def async_api_request(
+        method: str,
+        url: str,
+        headers: dict,
+        data: str = None,
+        params: str = None
+):
+    async with ClientSession() as session:
+        request = getattr(session, method)
+        async with request(
+                url=url,
+                headers=headers,
+                data=json.dumps(data) if data is not None else None,
+                params=params
+        ) as response:
+
+            response_data = await response.json()
+            response_data = convert_json(response_data, camel_to_underscore)
 
-                    return func(self, *args, **kwargs, response_data=response_data)
+            if is_exception(response):
+                return MonoPayAPIException(**response_data)
 
-        return inner
-
-    return outer
+            return response_data
 
 
-def async_post_request(url):
+def api_method(method: str, url: str):
     def outer(func):
-        async def inner(self, *args, **kwargs):
-            data = data_builder(**kwargs)
+        def inner(self, *args, **kwargs):
 
-            async with aiohttp.ClientSession() as session:
-                async with session.post(
-                    url=url.format(
-                        base_url=self.__base_url__
-                    ),
-                    headers=self.__headers__,
-                    data=json.dumps(data)
-                ) as response:
-                    response_data = await response.json()
+            func_args = {
+                "method": method,
+                "url": url.format(
+                    base_url=self.__base_url__
+                ),
+                "headers": self.__headers__,
+                ("params" if method == "get" else "data"): data_builder(**kwargs)
+            }
 
-                    return func(self, *args, **kwargs, response_data=response_data)
+            async def async_wrapper():
+                response = await async_api_request(**func_args)
 
-        return inner
+                if isinstance(response, MonoPayAPIException) or isinstance(response, MonobankAPIException):
+                    return response
 
-    return outer
+                return func(self, *args, **kwargs, response_data=response)
 
+            def sync_wrapper():
+                response = api_request(**func_args)
 
-def async_delete_request(url):
-    def outer(func):
-        async def inner(self, *args, **kwargs):
-            data = data_builder(**kwargs)
+                if isinstance(response, MonoPayAPIException) or isinstance(response, MonobankAPIException):
+                    return response
 
-            async with aiohttp.ClientSession() as session:
-                async with session.delete(
-                    url=url.format(
-                        base_url=self.__base_url__
-                    ),
-                    headers=self.__headers__,
-                    params=data
-                ) as response:
-                    response_data = await response.json()
+                return func(self, *args, **kwargs, response_data=response)
 
-                    return func(self, *args, **kwargs, response_data=response_data)
+            if self.__is_async__:
+                return async_wrapper()
+            else:
+                return sync_wrapper()
 
         return inner
 
     return outer
+
```

