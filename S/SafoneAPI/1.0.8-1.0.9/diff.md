# Comparing `tmp/SafoneAPI-1.0.8.tar.gz` & `tmp/SafoneAPI-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SafoneAPI-1.0.8.tar", last modified: Thu Jul 21 17:06:46 2022, max compression
+gzip compressed data, was "SafoneAPI-1.0.9.tar", last modified: Thu Jul 21 17:43:12 2022, max compression
```

## Comparing `SafoneAPI-1.0.8.tar` & `SafoneAPI-1.0.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 17:06:46.207067 SafoneAPI-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1066 2022-07-21 17:06:29.000000 SafoneAPI-1.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     3088 2022-07-21 17:06:46.207067 SafoneAPI-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2334 2022-07-21 17:06:29.000000 SafoneAPI-1.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 17:06:46.203066 SafoneAPI-1.0.8/SafoneAPI/
--rw-r--r--   0 runner    (1001) docker     (121)    31157 2022-07-21 17:06:29.000000 SafoneAPI-1.0.8/SafoneAPI/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 17:06:46.203066 SafoneAPI-1.0.8/SafoneAPI.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3088 2022-07-21 17:06:46.000000 SafoneAPI-1.0.8/SafoneAPI.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      212 2022-07-21 17:06:46.000000 SafoneAPI-1.0.8/SafoneAPI.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-21 17:06:46.000000 SafoneAPI-1.0.8/SafoneAPI.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       33 2022-07-21 17:06:46.000000 SafoneAPI-1.0.8/SafoneAPI.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-07-21 17:06:46.000000 SafoneAPI-1.0.8/SafoneAPI.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-07-21 17:06:46.207067 SafoneAPI-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1265 2022-07-21 17:06:29.000000 SafoneAPI-1.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 17:43:12.792690 SafoneAPI-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     1066 2022-07-21 17:42:59.000000 SafoneAPI-1.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     3088 2022-07-21 17:43:12.788690 SafoneAPI-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2334 2022-07-21 17:42:59.000000 SafoneAPI-1.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 17:43:12.788690 SafoneAPI-1.0.9/SafoneAPI/
+-rw-r--r--   0 runner    (1001) docker     (121)    31308 2022-07-21 17:42:59.000000 SafoneAPI-1.0.9/SafoneAPI/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 17:43:12.788690 SafoneAPI-1.0.9/SafoneAPI.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3088 2022-07-21 17:43:12.000000 SafoneAPI-1.0.9/SafoneAPI.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      212 2022-07-21 17:43:12.000000 SafoneAPI-1.0.9/SafoneAPI.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-21 17:43:12.000000 SafoneAPI-1.0.9/SafoneAPI.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       33 2022-07-21 17:43:12.000000 SafoneAPI-1.0.9/SafoneAPI.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       10 2022-07-21 17:43:12.000000 SafoneAPI-1.0.9/SafoneAPI.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-07-21 17:43:12.792690 SafoneAPI-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1265 2022-07-21 17:42:59.000000 SafoneAPI-1.0.9/setup.py
```

### Comparing `SafoneAPI-1.0.8/LICENSE` & `SafoneAPI-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `SafoneAPI-1.0.8/PKG-INFO` & `SafoneAPI-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SafoneAPI
-Version: 1.0.8
+Version: 1.0.9
 Summary: Asynchronous Python Wrapper For SafoneAPI
 Home-page: https://github.com/AsmSafone/SafoneAPI
 Author: AsmSafone
 Author-email: asmsafone@gmail.com
 License: MIT
 Keywords: API,SafoneAPI,Safone_API,Safone-API
 Classifier: Programming Language :: Python :: 3
```

### Comparing `SafoneAPI-1.0.8/README.md` & `SafoneAPI-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `SafoneAPI-1.0.8/SafoneAPI/__init__.py` & `SafoneAPI-1.0.9/SafoneAPI/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from typing import List
 from dotmap import DotMap
 from base64 import b64decode
 from pyrogram.types import Message, User
 from asyncio.exceptions import TimeoutError
 
 
-__version__ = "1.0.8"
+__version__ = "1.0.9"
 __author__ = "AsmSafone"
 
 
 class SafoneAPI:
     """
     SafoneAPI class to access all the endpoints of api
 
@@ -22,82 +22,85 @@
     def __init__(self) -> None:
         self.api = "https://api.safone.tech/"
         self.session = aiohttp.ClientSession
 
     def _get_name(self, user: User) -> str:
         return f"{user.first_name} {user.last_name or ''}".rstrip()
 
-    def _get_fname(self, format: str) -> str:
-        return f"{str(round(time.time()))}.{format}".rstrip()
+    def _get_fname(self, type: str) -> str:
+        return f"{str(round(time.time()))}.{type.split('/')[1]}".rstrip()
 
     async def _parse(self, response):
         try:
-            response = DotMap(await response.json())
+            response = DotMap(response)
         except Exception:
             raise InvalidContent(
                 "Invalid Content-Type, Please report this: https://api.safone.tech/report"
             )
         if response.type:
+            types = ["jpg", "jpeg", "png", "gif", "webp"]
             try:
-                type = response.type.split('/')[1]
+                if response.type.split('/')[1] in types:
+                    img_ = response.image.encode("utf-8")
+                    response = BytesIO(b64decode(img_))
+                    response.name = self._get_fname(response.type)
             except IndexError:
-                type = None
-            if type and type in ["jpg", "jpeg", "png", "gif", "webp"]:
-                img_ = response.image.encode("utf-8")
-                response = BytesIO(b64decode(img_))
-                response.name = self._get_fname(type)
+                pass
         return response
 
     async def _fetch(self, route, timeout=30, **params):
         try:
             async with self.session() as client:
                 resp = await client.get(self.api + route, params=params, timeout=timeout)
                 if resp.status == 400:
                     raise InvalidRequest(
                         "Invalid Request, Please read docs: https://api.safone.tech/redoc"
                     )
                 if resp.status == 422:
                     raise GenericApiError(
                         "Api Call Failed, Please report this: https://api.safone.tech/report"
                     )
+                response = await resp.json()
         except TimeoutError:
             raise TimeoutError("Failed to communicate with api server.")
-        return await self._parse(resp)
+        return await self._parse(response)
 
     async def _post_data(self, route, data, timeout=30):
         try:
             async with self.session() as client:
                 resp = await client.post(self.api + route, data=data, timeout=timeout)
                 if resp.status == 400:
                     raise InvalidRequest(
                         "Invalid Request, Please read docs: https://api.safone.tech/redoc"
                     )
                 if resp.status == 422:
                     raise GenericApiError(
                         "Api Call Failed, Please report this: https://api.safone.tech/report"
                     )
+                response = await resp.json()
         except TimeoutError:
             raise TimeoutError("Failed to communicate with api server.")
-        return await self._parse(resp)
+        return await self._parse(response)
 
     async def _post_json(self, route, json, timeout=30):
         try:
             async with self.session() as client:
                 resp = await client.post(self.api + route, json=json, timeout=timeout)
                 if resp.status == 400:
                     raise InvalidRequest(
                         "Invalid Request, Please read docs: https://api.safone.tech/redoc"
                     )
                 if resp.status == 422:
                     raise GenericApiError(
                         "Api Call Failed, Please report this: https://api.safone.tech/report"
                     )
+                response = await resp.json()
         except TimeoutError:
             raise TimeoutError("Failed to communicate with api server.")
-        return await self._parse(resp)
+        return await self._parse(response)
 
     async def advice(self):
         """
         Returns An Object.
 
                 Returns:
                         Result object (str): Results which you can access with dot notation
```

### Comparing `SafoneAPI-1.0.8/SafoneAPI.egg-info/PKG-INFO` & `SafoneAPI-1.0.9/SafoneAPI.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SafoneAPI
-Version: 1.0.8
+Version: 1.0.9
 Summary: Asynchronous Python Wrapper For SafoneAPI
 Home-page: https://github.com/AsmSafone/SafoneAPI
 Author: AsmSafone
 Author-email: asmsafone@gmail.com
 License: MIT
 Keywords: API,SafoneAPI,Safone_API,Safone-API
 Classifier: Programming Language :: Python :: 3
```

### Comparing `SafoneAPI-1.0.8/setup.py` & `SafoneAPI-1.0.9/setup.py`

 * *Files identical despite different names*

