# Comparing `tmp/unbelievaboat-1.1.0.tar.gz` & `tmp/unbelievaboat-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unbelievaboat-1.1.0.tar", last modified: Sat Jul  1 23:58:16 2023, max compression
+gzip compressed data, was "unbelievaboat-1.1.1.tar", last modified: Sun Jul  2 15:11:38 2023, max compression
```

## Comparing `unbelievaboat-1.1.0.tar` & `unbelievaboat-1.1.1.tar`

### file list

```diff
@@ -1,40 +1,39 @@
-drwxrwxrwx   0        0        0        0 2023-07-01 23:58:16.937073 unbelievaboat-1.1.0/
--rw-rw-rw-   0        0        0     1084 2023-07-01 15:11:46.000000 unbelievaboat-1.1.0/LICENSE
--rw-rw-rw-   0        0        0     3749 2023-07-01 23:58:16.933768 unbelievaboat-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     3008 2023-07-01 20:13:23.000000 unbelievaboat-1.1.0/README.md
--rw-rw-rw-   0        0        0       42 2023-07-01 23:58:16.938079 unbelievaboat-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1084 2023-07-01 23:57:38.000000 unbelievaboat-1.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-01 23:58:16.796860 unbelievaboat-1.1.0/unbelievaboat/
--rw-rw-rw-   0        0        0     7927 2023-07-01 23:56:31.000000 unbelievaboat-1.1.0/unbelievaboat/Client.py
--rw-rw-rw-   0        0        0     3736 2023-07-01 23:56:35.000000 unbelievaboat-1.1.0/unbelievaboat/RequestHandler.py
--rw-rw-rw-   0        0        0      365 2023-07-01 20:39:17.000000 unbelievaboat-1.1.0/unbelievaboat/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-01 23:58:16.856942 unbelievaboat-1.1.0/unbelievaboat/errors/
--rw-rw-rw-   0        0        0      497 2023-07-01 23:17:00.000000 unbelievaboat-1.1.0/unbelievaboat/errors/APIError.py
--rw-rw-rw-   0        0        0      514 2023-07-01 23:17:00.000000 unbelievaboat-1.1.0/unbelievaboat/errors/HTTPError.py
--rw-rw-rw-   0        0        0      105 2023-07-01 13:39:53.000000 unbelievaboat-1.1.0/unbelievaboat/errors/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-01 23:58:16.880113 unbelievaboat-1.1.0/unbelievaboat/structures/
--rw-rw-rw-   0        0        0      925 2023-07-01 16:58:46.000000 unbelievaboat-1.1.0/unbelievaboat/structures/Guild.py
--rw-rw-rw-   0        0        0      750 2023-07-01 20:59:31.000000 unbelievaboat-1.1.0/unbelievaboat/structures/Leaderboard.py
--rw-rw-rw-   0        0        0      929 2023-07-01 16:45:44.000000 unbelievaboat-1.1.0/unbelievaboat/structures/Permission.py
--rw-rw-rw-   0        0        0      711 2023-07-01 20:20:29.000000 unbelievaboat-1.1.0/unbelievaboat/structures/Store.py
--rw-rw-rw-   0        0        0     1306 2023-07-01 20:56:24.000000 unbelievaboat-1.1.0/unbelievaboat/structures/UserBalance.py
--rw-rw-rw-   0        0        0     2103 2023-07-01 23:12:16.000000 unbelievaboat-1.1.0/unbelievaboat/structures/UserInventory.py
--rw-rw-rw-   0        0        0      445 2023-07-01 20:39:39.000000 unbelievaboat-1.1.0/unbelievaboat/structures/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-01 23:58:16.898215 unbelievaboat-1.1.0/unbelievaboat/structures/items/
--rw-rw-rw-   0        0        0     1293 2023-07-01 16:54:27.000000 unbelievaboat-1.1.0/unbelievaboat/structures/items/BaseItem.py
--rw-rw-rw-   0        0        0      955 2023-07-01 22:06:03.000000 unbelievaboat-1.1.0/unbelievaboat/structures/items/InventoryItem.py
--rw-rw-rw-   0        0        0     1501 2023-07-01 20:53:07.000000 unbelievaboat-1.1.0/unbelievaboat/structures/items/StoreItem.py
--rw-rw-rw-   0        0        0     1030 2023-07-01 16:54:52.000000 unbelievaboat-1.1.0/unbelievaboat/structures/items/StoreItemAction.py
--rw-rw-rw-   0        0        0     1296 2023-07-01 16:55:37.000000 unbelievaboat-1.1.0/unbelievaboat/structures/items/StoreItemRequirement.py
--rw-rw-rw-   0        0        0      338 2023-07-01 13:39:53.000000 unbelievaboat-1.1.0/unbelievaboat/structures/items/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-01 23:58:16.929089 unbelievaboat-1.1.0/unbelievaboat/util/
--rw-rw-rw-   0        0        0     1422 2023-07-01 23:56:41.000000 unbelievaboat-1.1.0/unbelievaboat/util/Bucket.py
--rw-rw-rw-   0        0        0      383 2023-07-01 12:00:58.000000 unbelievaboat-1.1.0/unbelievaboat/util/Constants.py
--rw-rw-rw-   0        0        0      551 2023-07-01 13:15:13.000000 unbelievaboat-1.1.0/unbelievaboat/util/SnakeCaseConventer.py
--rw-rw-rw-   0        0        0      250 2023-07-01 13:41:07.000000 unbelievaboat-1.1.0/unbelievaboat/util/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-01 23:58:16.847076 unbelievaboat-1.1.0/unbelievaboat.egg-info/
--rw-rw-rw-   0        0        0     3749 2023-07-01 23:58:16.000000 unbelievaboat-1.1.0/unbelievaboat.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1074 2023-07-01 23:58:16.000000 unbelievaboat-1.1.0/unbelievaboat.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-01 23:58:16.000000 unbelievaboat-1.1.0/unbelievaboat.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-07-01 23:58:16.000000 unbelievaboat-1.1.0/unbelievaboat.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-07-01 23:58:16.000000 unbelievaboat-1.1.0/unbelievaboat.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-02 15:11:38.547157 unbelievaboat-1.1.1/
+-rw-rw-rw-   0        0        0     1084 2023-07-01 15:11:46.000000 unbelievaboat-1.1.1/LICENSE
+-rw-rw-rw-   0        0        0     3749 2023-07-02 15:11:38.546074 unbelievaboat-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3008 2023-07-01 20:13:23.000000 unbelievaboat-1.1.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-02 15:11:38.547157 unbelievaboat-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1084 2023-07-02 15:11:02.000000 unbelievaboat-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-02 15:11:38.478247 unbelievaboat-1.1.1/unbelievaboat/
+-rw-rw-rw-   0        0        0     7927 2023-07-01 23:56:31.000000 unbelievaboat-1.1.1/unbelievaboat/Client.py
+-rw-rw-rw-   0        0        0     3390 2023-07-02 15:10:49.000000 unbelievaboat-1.1.1/unbelievaboat/RequestHandler.py
+-rw-rw-rw-   0        0        0      365 2023-07-01 20:39:17.000000 unbelievaboat-1.1.1/unbelievaboat/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-02 15:11:38.522336 unbelievaboat-1.1.1/unbelievaboat/errors/
+-rw-rw-rw-   0        0        0      497 2023-07-01 23:17:00.000000 unbelievaboat-1.1.1/unbelievaboat/errors/APIError.py
+-rw-rw-rw-   0        0        0      514 2023-07-01 23:17:00.000000 unbelievaboat-1.1.1/unbelievaboat/errors/HTTPError.py
+-rw-rw-rw-   0        0        0      105 2023-07-01 13:39:53.000000 unbelievaboat-1.1.1/unbelievaboat/errors/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-02 15:11:38.532858 unbelievaboat-1.1.1/unbelievaboat/structures/
+-rw-rw-rw-   0        0        0      925 2023-07-01 16:58:46.000000 unbelievaboat-1.1.1/unbelievaboat/structures/Guild.py
+-rw-rw-rw-   0        0        0      750 2023-07-01 20:59:31.000000 unbelievaboat-1.1.1/unbelievaboat/structures/Leaderboard.py
+-rw-rw-rw-   0        0        0      929 2023-07-01 16:45:44.000000 unbelievaboat-1.1.1/unbelievaboat/structures/Permission.py
+-rw-rw-rw-   0        0        0      711 2023-07-01 20:20:29.000000 unbelievaboat-1.1.1/unbelievaboat/structures/Store.py
+-rw-rw-rw-   0        0        0     1306 2023-07-01 20:56:24.000000 unbelievaboat-1.1.1/unbelievaboat/structures/UserBalance.py
+-rw-rw-rw-   0        0        0     2103 2023-07-01 23:12:16.000000 unbelievaboat-1.1.1/unbelievaboat/structures/UserInventory.py
+-rw-rw-rw-   0        0        0      445 2023-07-01 20:39:39.000000 unbelievaboat-1.1.1/unbelievaboat/structures/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-02 15:11:38.540854 unbelievaboat-1.1.1/unbelievaboat/structures/items/
+-rw-rw-rw-   0        0        0     1293 2023-07-01 16:54:27.000000 unbelievaboat-1.1.1/unbelievaboat/structures/items/BaseItem.py
+-rw-rw-rw-   0        0        0      955 2023-07-01 22:06:03.000000 unbelievaboat-1.1.1/unbelievaboat/structures/items/InventoryItem.py
+-rw-rw-rw-   0        0        0     1501 2023-07-01 20:53:07.000000 unbelievaboat-1.1.1/unbelievaboat/structures/items/StoreItem.py
+-rw-rw-rw-   0        0        0     1030 2023-07-01 16:54:52.000000 unbelievaboat-1.1.1/unbelievaboat/structures/items/StoreItemAction.py
+-rw-rw-rw-   0        0        0     1296 2023-07-01 16:55:37.000000 unbelievaboat-1.1.1/unbelievaboat/structures/items/StoreItemRequirement.py
+-rw-rw-rw-   0        0        0      338 2023-07-01 13:39:53.000000 unbelievaboat-1.1.1/unbelievaboat/structures/items/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-02 15:11:38.544563 unbelievaboat-1.1.1/unbelievaboat/util/
+-rw-rw-rw-   0        0        0      383 2023-07-01 12:00:58.000000 unbelievaboat-1.1.1/unbelievaboat/util/Constants.py
+-rw-rw-rw-   0        0        0      551 2023-07-01 13:15:13.000000 unbelievaboat-1.1.1/unbelievaboat/util/SnakeCaseConventer.py
+-rw-rw-rw-   0        0        0      207 2023-07-02 15:05:17.000000 unbelievaboat-1.1.1/unbelievaboat/util/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-02 15:11:38.518303 unbelievaboat-1.1.1/unbelievaboat.egg-info/
+-rw-rw-rw-   0        0        0     3749 2023-07-02 15:11:38.000000 unbelievaboat-1.1.1/unbelievaboat.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1045 2023-07-02 15:11:38.000000 unbelievaboat-1.1.1/unbelievaboat.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-02 15:11:38.000000 unbelievaboat-1.1.1/unbelievaboat.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-07-02 15:11:38.000000 unbelievaboat-1.1.1/unbelievaboat.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-07-02 15:11:38.000000 unbelievaboat-1.1.1/unbelievaboat.egg-info/top_level.txt
```

### Comparing `unbelievaboat-1.1.0/LICENSE` & `unbelievaboat-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `unbelievaboat-1.1.0/PKG-INFO` & `unbelievaboat-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unbelievaboat
-Version: 1.1.0
+Version: 1.1.1
 Summary: Wrapper for UnbelievaBoat API.
 Home-page: https://github.com/yoggys/unbelievaboat
 Author: yoggys
 Author-email: yoggies@yoggies.ovh
 Keywords: python,unb,unbelievaboat,api,wrapper,async,asyncio
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `unbelievaboat-1.1.0/README.md` & `unbelievaboat-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `unbelievaboat-1.1.0/setup.py` & `unbelievaboat-1.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 
 cwd = Path(__file__).parent
 long_description = (cwd / "README.md").read_text()
 
 setup(
     name="unbelievaboat",
-    version="1.1.0",
+    version="1.1.1",
     author="yoggys",
     author_email="yoggies@yoggies.ovh",
     description="Wrapper for UnbelievaBoat API.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/yoggys/unbelievaboat",
     packages=find_packages(),
```

### Comparing `unbelievaboat-1.1.0/unbelievaboat/Client.py` & `unbelievaboat-1.1.1/unbelievaboat/Client.py`

 * *Files identical despite different names*

### Comparing `unbelievaboat-1.1.0/unbelievaboat/RequestHandler.py` & `unbelievaboat-1.1.1/unbelievaboat/RequestHandler.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,48 +1,48 @@
-import json
+import asyncio
 import time
 from typing import Any, Dict, Optional
 
 from .errors import APIError, HTTPError
-from .util import Bucket
 
 
 class RequestHandler:
     def __init__(self, client) -> None:
         self._client = client
-        self.ratelimits: Dict[str, Bucket] = {}
+        self.locks: Dict[str, asyncio.Lock] = {}
 
     def __str__(self) -> str:
         return "<RequestHandler>"
 
     async def request(
         self,
         method: str,
         endpoint: str,
         data: Optional[Dict[str, Any]] = None,
         params: Optional[Dict[str, Any]] = None,
         _attempts: int = 0,
     ) -> Any:
         route = self.get_route(method, endpoint)
-        if route not in self.ratelimits:
-            self.ratelimits[route] = Bucket()
+        if route not in self.locks:
+            self.locks[route] = asyncio.Lock()
 
-        return await self.ratelimits[route].queue(self.execute_request, route, method, endpoint, data, params, _attempts)
-        # await self.ratelimits[route].execute()
+        return await self.execute_request(
+            route, method, endpoint, data, params, _attempts
+        )
 
     async def execute_request(
         self,
         route: str,
         method: str,
         endpoint: str,
         data: Optional[Dict[str, Any]] = None,
         params: Optional[Dict[str, Any]] = None,
         _attempts: int = 0,
     ):
-        async with self.ratelimits[route].semaphore:
+        async with self.locks[route]:
             url = "{}/{}/{}".format(
                 self._client.base_url, self._client.version, endpoint
             )
             options = {
                 "headers": {
                     "Authorization": self._client.token,
                     "Content-Type": "application/json",
@@ -52,25 +52,24 @@
                 "json": data,
                 "params": params,
             }
 
             async with self._client._session.request(
                 **options
             ) as response:  # type: ClientResponse
-                # Increase the number of attempts
                 _attempts += 1
 
-                # Add the rate limit header data to the bucket
-                self.parse_rate_limit_headers(route, response.headers)
+                # Handle rate limits
+                await self.parse_rate_limit_headers(response.headers)
 
                 if response.status >= 200 and response.status < 300:
                     try:
                         return await response.json()
-                    except:
-                        return json.dumps(await response.text())
+                    except Exception as e:
+                        return await response.text()
 
                 if response.status == 429:
                     if _attempts >= self._client._max_retries:
                         raise APIError(await response.json(), response)
                     else:
                         await self.request(method, endpoint, data, params, _attempts)
 
@@ -85,24 +84,18 @@
             lambda match: match.group()
             if match.group(1) in major_params
             else f"/{match.group(1)}/:id",
             endpoint,
         )
         return f"{method}/{route}"
 
-    def parse_rate_limit_headers(self, route: str, headers: Dict[str, str]) -> None:
-        self.ratelimits[route].limit = int(headers.get("x-ratelimit-limit", 0))
-
-        remaining = headers.get("x-ratelimit-remaining")
-        self.ratelimits[route].remaining = (
-            int(remaining) if remaining is not None else 1
-        )
-
-        now = time.time()
-        retry_after = headers.get("retry-after")
-        if retry_after:
-            self.ratelimits[route].reset = float(retry_after) + now
-        else:
-            reset_time = headers.get("x-ratelimit-reset")
-            self.ratelimits[route].reset = (
-                max(int(reset_time)/1000, now) if reset_time else now
-            )
+    async def parse_rate_limit_headers(self, headers: Dict[str, str]) -> None:
+        remaining = int(headers.get("x-ratelimit-remaining", 0))
+        if remaining <= 0:
+            if headers.get("retry-after"):
+                retry_after = float(headers.get("retry-after", 0)) / 1000
+                await asyncio.sleep(retry_after)
+            else:
+                reset_after = (
+                    float(headers.get("x-ratelimit-reset", 0)) / 1000 - time.time()
+                )
+                await asyncio.sleep(reset_after)
```

### Comparing `unbelievaboat-1.1.0/unbelievaboat/errors/HTTPError.py` & `unbelievaboat-1.1.1/unbelievaboat/errors/HTTPError.py`

 * *Files identical despite different names*

### Comparing `unbelievaboat-1.1.0/unbelievaboat/structures/Guild.py` & `unbelievaboat-1.1.1/unbelievaboat/structures/Guild.py`

 * *Files identical despite different names*

### Comparing `unbelievaboat-1.1.0/unbelievaboat/structures/Leaderboard.py` & `unbelievaboat-1.1.1/unbelievaboat/structures/Leaderboard.py`

 * *Files identical despite different names*

### Comparing `unbelievaboat-1.1.0/unbelievaboat/structures/Permission.py` & `unbelievaboat-1.1.1/unbelievaboat/structures/Permission.py`

 * *Files identical despite different names*

### Comparing `unbelievaboat-1.1.0/unbelievaboat/structures/Store.py` & `unbelievaboat-1.1.1/unbelievaboat/structures/Store.py`

 * *Files identical despite different names*

### Comparing `unbelievaboat-1.1.0/unbelievaboat/structures/UserBalance.py` & `unbelievaboat-1.1.1/unbelievaboat/structures/UserBalance.py`

 * *Files identical despite different names*

### Comparing `unbelievaboat-1.1.0/unbelievaboat/structures/UserInventory.py` & `unbelievaboat-1.1.1/unbelievaboat/structures/UserInventory.py`

 * *Files identical despite different names*

### Comparing `unbelievaboat-1.1.0/unbelievaboat/structures/items/BaseItem.py` & `unbelievaboat-1.1.1/unbelievaboat/structures/items/BaseItem.py`

 * *Files identical despite different names*

### Comparing `unbelievaboat-1.1.0/unbelievaboat/structures/items/InventoryItem.py` & `unbelievaboat-1.1.1/unbelievaboat/structures/items/InventoryItem.py`

 * *Files identical despite different names*

### Comparing `unbelievaboat-1.1.0/unbelievaboat/structures/items/StoreItem.py` & `unbelievaboat-1.1.1/unbelievaboat/structures/items/StoreItem.py`

 * *Files identical despite different names*

### Comparing `unbelievaboat-1.1.0/unbelievaboat/structures/items/StoreItemAction.py` & `unbelievaboat-1.1.1/unbelievaboat/structures/items/StoreItemAction.py`

 * *Files identical despite different names*

### Comparing `unbelievaboat-1.1.0/unbelievaboat/structures/items/StoreItemRequirement.py` & `unbelievaboat-1.1.1/unbelievaboat/structures/items/StoreItemRequirement.py`

 * *Files identical despite different names*

### Comparing `unbelievaboat-1.1.0/unbelievaboat/util/SnakeCaseConventer.py` & `unbelievaboat-1.1.1/unbelievaboat/util/SnakeCaseConventer.py`

 * *Files identical despite different names*

### Comparing `unbelievaboat-1.1.0/unbelievaboat.egg-info/PKG-INFO` & `unbelievaboat-1.1.1/unbelievaboat.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unbelievaboat
-Version: 1.1.0
+Version: 1.1.1
 Summary: Wrapper for UnbelievaBoat API.
 Home-page: https://github.com/yoggys/unbelievaboat
 Author: yoggys
 Author-email: yoggies@yoggies.ovh
 Keywords: python,unb,unbelievaboat,api,wrapper,async,asyncio
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `unbelievaboat-1.1.0/unbelievaboat.egg-info/SOURCES.txt` & `unbelievaboat-1.1.1/unbelievaboat.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -21,11 +21,10 @@
 unbelievaboat/structures/__init__.py
 unbelievaboat/structures/items/BaseItem.py
 unbelievaboat/structures/items/InventoryItem.py
 unbelievaboat/structures/items/StoreItem.py
 unbelievaboat/structures/items/StoreItemAction.py
 unbelievaboat/structures/items/StoreItemRequirement.py
 unbelievaboat/structures/items/__init__.py
-unbelievaboat/util/Bucket.py
 unbelievaboat/util/Constants.py
 unbelievaboat/util/SnakeCaseConventer.py
 unbelievaboat/util/__init__.py
```

