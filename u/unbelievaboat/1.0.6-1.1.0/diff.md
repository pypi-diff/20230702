# Comparing `tmp/unbelievaboat-1.0.6.tar.gz` & `tmp/unbelievaboat-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unbelievaboat-1.0.6.tar", last modified: Sat Jul  1 22:48:57 2023, max compression
+gzip compressed data, was "unbelievaboat-1.1.0.tar", last modified: Sat Jul  1 23:58:16 2023, max compression
```

## Comparing `unbelievaboat-1.0.6.tar` & `unbelievaboat-1.1.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxrwx   0        0        0        0 2023-07-01 22:48:57.963254 unbelievaboat-1.0.6/
--rw-rw-rw-   0        0        0     1084 2023-07-01 15:11:46.000000 unbelievaboat-1.0.6/LICENSE
--rw-rw-rw-   0        0        0     3749 2023-07-01 22:48:57.962238 unbelievaboat-1.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     3008 2023-07-01 20:13:23.000000 unbelievaboat-1.0.6/README.md
--rw-rw-rw-   0        0        0       42 2023-07-01 22:48:57.963254 unbelievaboat-1.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1084 2023-07-01 22:48:32.000000 unbelievaboat-1.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-01 22:48:57.890012 unbelievaboat-1.0.6/unbelievaboat/
--rw-rw-rw-   0        0        0     7927 2023-07-01 22:45:49.000000 unbelievaboat-1.0.6/unbelievaboat/Client.py
--rw-rw-rw-   0        0        0     3301 2023-07-01 22:39:10.000000 unbelievaboat-1.0.6/unbelievaboat/RequestHandler.py
--rw-rw-rw-   0        0        0      365 2023-07-01 20:39:17.000000 unbelievaboat-1.0.6/unbelievaboat/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-01 22:48:57.934340 unbelievaboat-1.0.6/unbelievaboat/errors/
--rw-rw-rw-   0        0        0      509 2023-07-01 22:42:38.000000 unbelievaboat-1.0.6/unbelievaboat/errors/APIError.py
--rw-rw-rw-   0        0        0      518 2023-07-01 22:42:02.000000 unbelievaboat-1.0.6/unbelievaboat/errors/HTTPError.py
--rw-rw-rw-   0        0        0      105 2023-07-01 13:39:53.000000 unbelievaboat-1.0.6/unbelievaboat/errors/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-01 22:48:57.944557 unbelievaboat-1.0.6/unbelievaboat/structures/
--rw-rw-rw-   0        0        0      925 2023-07-01 16:58:46.000000 unbelievaboat-1.0.6/unbelievaboat/structures/Guild.py
--rw-rw-rw-   0        0        0      750 2023-07-01 20:59:31.000000 unbelievaboat-1.0.6/unbelievaboat/structures/Leaderboard.py
--rw-rw-rw-   0        0        0      929 2023-07-01 16:45:44.000000 unbelievaboat-1.0.6/unbelievaboat/structures/Permission.py
--rw-rw-rw-   0        0        0      711 2023-07-01 20:20:29.000000 unbelievaboat-1.0.6/unbelievaboat/structures/Store.py
--rw-rw-rw-   0        0        0     1306 2023-07-01 20:56:24.000000 unbelievaboat-1.0.6/unbelievaboat/structures/UserBalance.py
--rw-rw-rw-   0        0        0     2079 2023-07-01 22:32:11.000000 unbelievaboat-1.0.6/unbelievaboat/structures/UserInventory.py
--rw-rw-rw-   0        0        0      445 2023-07-01 20:39:39.000000 unbelievaboat-1.0.6/unbelievaboat/structures/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-01 22:48:57.955263 unbelievaboat-1.0.6/unbelievaboat/structures/items/
--rw-rw-rw-   0        0        0     1293 2023-07-01 16:54:27.000000 unbelievaboat-1.0.6/unbelievaboat/structures/items/BaseItem.py
--rw-rw-rw-   0        0        0      955 2023-07-01 22:06:03.000000 unbelievaboat-1.0.6/unbelievaboat/structures/items/InventoryItem.py
--rw-rw-rw-   0        0        0     1501 2023-07-01 20:53:07.000000 unbelievaboat-1.0.6/unbelievaboat/structures/items/StoreItem.py
--rw-rw-rw-   0        0        0     1030 2023-07-01 16:54:52.000000 unbelievaboat-1.0.6/unbelievaboat/structures/items/StoreItemAction.py
--rw-rw-rw-   0        0        0     1296 2023-07-01 16:55:37.000000 unbelievaboat-1.0.6/unbelievaboat/structures/items/StoreItemRequirement.py
--rw-rw-rw-   0        0        0      338 2023-07-01 13:39:53.000000 unbelievaboat-1.0.6/unbelievaboat/structures/items/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-01 22:48:57.961182 unbelievaboat-1.0.6/unbelievaboat/util/
--rw-rw-rw-   0        0        0     1143 2023-07-01 11:45:16.000000 unbelievaboat-1.0.6/unbelievaboat/util/Bucket.py
--rw-rw-rw-   0        0        0      383 2023-07-01 12:00:58.000000 unbelievaboat-1.0.6/unbelievaboat/util/Constants.py
--rw-rw-rw-   0        0        0      551 2023-07-01 13:15:13.000000 unbelievaboat-1.0.6/unbelievaboat/util/SnakeCaseConventer.py
--rw-rw-rw-   0        0        0      250 2023-07-01 13:41:07.000000 unbelievaboat-1.0.6/unbelievaboat/util/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-01 22:48:57.929573 unbelievaboat-1.0.6/unbelievaboat.egg-info/
--rw-rw-rw-   0        0        0     3749 2023-07-01 22:48:57.000000 unbelievaboat-1.0.6/unbelievaboat.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1074 2023-07-01 22:48:57.000000 unbelievaboat-1.0.6/unbelievaboat.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-01 22:48:57.000000 unbelievaboat-1.0.6/unbelievaboat.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-07-01 22:48:57.000000 unbelievaboat-1.0.6/unbelievaboat.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-07-01 22:48:57.000000 unbelievaboat-1.0.6/unbelievaboat.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-01 23:58:16.937073 unbelievaboat-1.1.0/
+-rw-rw-rw-   0        0        0     1084 2023-07-01 15:11:46.000000 unbelievaboat-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0     3749 2023-07-01 23:58:16.933768 unbelievaboat-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3008 2023-07-01 20:13:23.000000 unbelievaboat-1.1.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-01 23:58:16.938079 unbelievaboat-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1084 2023-07-01 23:57:38.000000 unbelievaboat-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-01 23:58:16.796860 unbelievaboat-1.1.0/unbelievaboat/
+-rw-rw-rw-   0        0        0     7927 2023-07-01 23:56:31.000000 unbelievaboat-1.1.0/unbelievaboat/Client.py
+-rw-rw-rw-   0        0        0     3736 2023-07-01 23:56:35.000000 unbelievaboat-1.1.0/unbelievaboat/RequestHandler.py
+-rw-rw-rw-   0        0        0      365 2023-07-01 20:39:17.000000 unbelievaboat-1.1.0/unbelievaboat/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-01 23:58:16.856942 unbelievaboat-1.1.0/unbelievaboat/errors/
+-rw-rw-rw-   0        0        0      497 2023-07-01 23:17:00.000000 unbelievaboat-1.1.0/unbelievaboat/errors/APIError.py
+-rw-rw-rw-   0        0        0      514 2023-07-01 23:17:00.000000 unbelievaboat-1.1.0/unbelievaboat/errors/HTTPError.py
+-rw-rw-rw-   0        0        0      105 2023-07-01 13:39:53.000000 unbelievaboat-1.1.0/unbelievaboat/errors/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-01 23:58:16.880113 unbelievaboat-1.1.0/unbelievaboat/structures/
+-rw-rw-rw-   0        0        0      925 2023-07-01 16:58:46.000000 unbelievaboat-1.1.0/unbelievaboat/structures/Guild.py
+-rw-rw-rw-   0        0        0      750 2023-07-01 20:59:31.000000 unbelievaboat-1.1.0/unbelievaboat/structures/Leaderboard.py
+-rw-rw-rw-   0        0        0      929 2023-07-01 16:45:44.000000 unbelievaboat-1.1.0/unbelievaboat/structures/Permission.py
+-rw-rw-rw-   0        0        0      711 2023-07-01 20:20:29.000000 unbelievaboat-1.1.0/unbelievaboat/structures/Store.py
+-rw-rw-rw-   0        0        0     1306 2023-07-01 20:56:24.000000 unbelievaboat-1.1.0/unbelievaboat/structures/UserBalance.py
+-rw-rw-rw-   0        0        0     2103 2023-07-01 23:12:16.000000 unbelievaboat-1.1.0/unbelievaboat/structures/UserInventory.py
+-rw-rw-rw-   0        0        0      445 2023-07-01 20:39:39.000000 unbelievaboat-1.1.0/unbelievaboat/structures/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-01 23:58:16.898215 unbelievaboat-1.1.0/unbelievaboat/structures/items/
+-rw-rw-rw-   0        0        0     1293 2023-07-01 16:54:27.000000 unbelievaboat-1.1.0/unbelievaboat/structures/items/BaseItem.py
+-rw-rw-rw-   0        0        0      955 2023-07-01 22:06:03.000000 unbelievaboat-1.1.0/unbelievaboat/structures/items/InventoryItem.py
+-rw-rw-rw-   0        0        0     1501 2023-07-01 20:53:07.000000 unbelievaboat-1.1.0/unbelievaboat/structures/items/StoreItem.py
+-rw-rw-rw-   0        0        0     1030 2023-07-01 16:54:52.000000 unbelievaboat-1.1.0/unbelievaboat/structures/items/StoreItemAction.py
+-rw-rw-rw-   0        0        0     1296 2023-07-01 16:55:37.000000 unbelievaboat-1.1.0/unbelievaboat/structures/items/StoreItemRequirement.py
+-rw-rw-rw-   0        0        0      338 2023-07-01 13:39:53.000000 unbelievaboat-1.1.0/unbelievaboat/structures/items/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-01 23:58:16.929089 unbelievaboat-1.1.0/unbelievaboat/util/
+-rw-rw-rw-   0        0        0     1422 2023-07-01 23:56:41.000000 unbelievaboat-1.1.0/unbelievaboat/util/Bucket.py
+-rw-rw-rw-   0        0        0      383 2023-07-01 12:00:58.000000 unbelievaboat-1.1.0/unbelievaboat/util/Constants.py
+-rw-rw-rw-   0        0        0      551 2023-07-01 13:15:13.000000 unbelievaboat-1.1.0/unbelievaboat/util/SnakeCaseConventer.py
+-rw-rw-rw-   0        0        0      250 2023-07-01 13:41:07.000000 unbelievaboat-1.1.0/unbelievaboat/util/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-01 23:58:16.847076 unbelievaboat-1.1.0/unbelievaboat.egg-info/
+-rw-rw-rw-   0        0        0     3749 2023-07-01 23:58:16.000000 unbelievaboat-1.1.0/unbelievaboat.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1074 2023-07-01 23:58:16.000000 unbelievaboat-1.1.0/unbelievaboat.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-01 23:58:16.000000 unbelievaboat-1.1.0/unbelievaboat.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-07-01 23:58:16.000000 unbelievaboat-1.1.0/unbelievaboat.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-07-01 23:58:16.000000 unbelievaboat-1.1.0/unbelievaboat.egg-info/top_level.txt
```

### Comparing `unbelievaboat-1.0.6/LICENSE` & `unbelievaboat-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `unbelievaboat-1.0.6/PKG-INFO` & `unbelievaboat-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unbelievaboat
-Version: 1.0.6
+Version: 1.1.0
 Summary: Wrapper for UnbelievaBoat API.
 Home-page: https://github.com/yoggys/unbelievaboat
 Author: yoggys
 Author-email: yoggies@yoggies.ovh
 Keywords: python,unb,unbelievaboat,api,wrapper,async,asyncio
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `unbelievaboat-1.0.6/README.md` & `unbelievaboat-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `unbelievaboat-1.0.6/setup.py` & `unbelievaboat-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 
 cwd = Path(__file__).parent
 long_description = (cwd / "README.md").read_text()
 
 setup(
     name="unbelievaboat",
-    version="1.0.6",
+    version="1.1.0",
     author="yoggys",
     author_email="yoggies@yoggies.ovh",
     description="Wrapper for UnbelievaBoat API.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/yoggys/unbelievaboat",
     packages=find_packages(),
```

### Comparing `unbelievaboat-1.0.6/unbelievaboat/Client.py` & `unbelievaboat-1.1.0/unbelievaboat/Client.py`

 * *Files identical despite different names*

### Comparing `unbelievaboat-1.0.6/unbelievaboat/RequestHandler.py` & `unbelievaboat-1.1.0/unbelievaboat/RequestHandler.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import json
+import time
 from typing import Any, Dict, Optional
 
 from .errors import APIError, HTTPError
 from .util import Bucket
 
 
 class RequestHandler:
@@ -21,14 +22,26 @@
         params: Optional[Dict[str, Any]] = None,
         _attempts: int = 0,
     ) -> Any:
         route = self.get_route(method, endpoint)
         if route not in self.ratelimits:
             self.ratelimits[route] = Bucket()
 
+        return await self.ratelimits[route].queue(self.execute_request, route, method, endpoint, data, params, _attempts)
+        # await self.ratelimits[route].execute()
+
+    async def execute_request(
+        self,
+        route: str,
+        method: str,
+        endpoint: str,
+        data: Optional[Dict[str, Any]] = None,
+        params: Optional[Dict[str, Any]] = None,
+        _attempts: int = 0,
+    ):
         async with self.ratelimits[route].semaphore:
             url = "{}/{}/{}".format(
                 self._client.base_url, self._client.version, endpoint
             )
             options = {
                 "headers": {
                     "Authorization": self._client.token,
@@ -53,19 +66,19 @@
                     try:
                         return await response.json()
                     except:
                         return json.dumps(await response.text())
 
                 if response.status == 429:
                     if _attempts >= self._client._max_retries:
-                        raise APIError(response)
+                        raise APIError(await response.json(), response)
                     else:
                         await self.request(method, endpoint, data, params, _attempts)
 
-                raise HTTPError(response.status, await response.json())
+                raise HTTPError(await response.json(), response)
 
     def get_route(self, method: str, endpoint: str) -> str:
         import re
 
         major_params = ["guilds"]
         route = re.sub(
             r"/([a-z-]+)/(?:(\d+))",
@@ -73,26 +86,23 @@
             if match.group(1) in major_params
             else f"/{match.group(1)}/:id",
             endpoint,
         )
         return f"{method}/{route}"
 
     def parse_rate_limit_headers(self, route: str, headers: Dict[str, str]) -> None:
-        import time
-
-        now = time.time()
-
         self.ratelimits[route].limit = int(headers.get("x-ratelimit-limit", 0))
 
         remaining = headers.get("x-ratelimit-remaining")
         self.ratelimits[route].remaining = (
             int(remaining) if remaining is not None else 1
         )
 
+        now = time.time()
         retry_after = headers.get("retry-after")
         if retry_after:
-            self.ratelimits[route].reset = int(retry_after) + now
+            self.ratelimits[route].reset = float(retry_after) + now
         else:
             reset_time = headers.get("x-ratelimit-reset")
             self.ratelimits[route].reset = (
-                max(int(reset_time), now) if reset_time else now
+                max(int(reset_time)/1000, now) if reset_time else now
             )
```

### Comparing `unbelievaboat-1.0.6/unbelievaboat/errors/HTTPError.py` & `unbelievaboat-1.1.0/unbelievaboat/errors/HTTPError.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from typing import Any, Dict
 
 import aiohttp
 
 
 class HTTPError(Exception):
-    def __init__(self, status: int, data: Dict[str, Any], response: aiohttp.ClientResponse) -> None:
+    def __init__(self, data: Dict[str, Any], response: aiohttp.ClientResponse) -> None:
         super().__init__(response)
         self.name: str = self.__class__.__name__
-        self.status: int = status
+        self.status: int = response.status
         self.message: str = data.get("message") or "Unknown error"
 
         self.response: aiohttp.ClientResponse = response
 
     def __str__(self):
         return f"HTTP Error {self.status}: {self.message}"
```

### Comparing `unbelievaboat-1.0.6/unbelievaboat/structures/Guild.py` & `unbelievaboat-1.1.0/unbelievaboat/structures/Guild.py`

 * *Files identical despite different names*

### Comparing `unbelievaboat-1.0.6/unbelievaboat/structures/Leaderboard.py` & `unbelievaboat-1.1.0/unbelievaboat/structures/Leaderboard.py`

 * *Files identical despite different names*

### Comparing `unbelievaboat-1.0.6/unbelievaboat/structures/Permission.py` & `unbelievaboat-1.1.0/unbelievaboat/structures/Permission.py`

 * *Files identical despite different names*

### Comparing `unbelievaboat-1.0.6/unbelievaboat/structures/Store.py` & `unbelievaboat-1.1.0/unbelievaboat/structures/Store.py`

 * *Files identical despite different names*

### Comparing `unbelievaboat-1.0.6/unbelievaboat/structures/UserBalance.py` & `unbelievaboat-1.1.0/unbelievaboat/structures/UserBalance.py`

 * *Files identical despite different names*

### Comparing `unbelievaboat-1.0.6/unbelievaboat/structures/UserInventory.py` & `unbelievaboat-1.1.0/unbelievaboat/structures/UserInventory.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,17 @@
         )
 
     async def add_item(
         self, item: Union[str, Union[InventoryItem, StoreItem]], quantity: int = 1
     ) -> Self:
         item_id = item if isinstance(item, str) else item.id
         data: Dict[str, any] = {"item_id": item_id, "quantity": quantity}
-        added_item = await self._client.add_inventory_item(self.guild_id, self.user_id, data)
+        added_item = await self._client.add_inventory_item(
+            self.guild_id, self.user_id, data
+        )
         for item in self.items:
             if item.id == added_item.id:
                 item = added_item
                 return self
         self.items.append(added_item)
         return self
```

### Comparing `unbelievaboat-1.0.6/unbelievaboat/structures/items/BaseItem.py` & `unbelievaboat-1.1.0/unbelievaboat/structures/items/BaseItem.py`

 * *Files identical despite different names*

### Comparing `unbelievaboat-1.0.6/unbelievaboat/structures/items/InventoryItem.py` & `unbelievaboat-1.1.0/unbelievaboat/structures/items/InventoryItem.py`

 * *Files identical despite different names*

### Comparing `unbelievaboat-1.0.6/unbelievaboat/structures/items/StoreItem.py` & `unbelievaboat-1.1.0/unbelievaboat/structures/items/StoreItem.py`

 * *Files identical despite different names*

### Comparing `unbelievaboat-1.0.6/unbelievaboat/structures/items/StoreItemAction.py` & `unbelievaboat-1.1.0/unbelievaboat/structures/items/StoreItemAction.py`

 * *Files identical despite different names*

### Comparing `unbelievaboat-1.0.6/unbelievaboat/structures/items/StoreItemRequirement.py` & `unbelievaboat-1.1.0/unbelievaboat/structures/items/StoreItemRequirement.py`

 * *Files identical despite different names*

### Comparing `unbelievaboat-1.0.6/unbelievaboat/util/SnakeCaseConventer.py` & `unbelievaboat-1.1.0/unbelievaboat/util/SnakeCaseConventer.py`

 * *Files identical despite different names*

### Comparing `unbelievaboat-1.0.6/unbelievaboat.egg-info/PKG-INFO` & `unbelievaboat-1.1.0/unbelievaboat.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unbelievaboat
-Version: 1.0.6
+Version: 1.1.0
 Summary: Wrapper for UnbelievaBoat API.
 Home-page: https://github.com/yoggys/unbelievaboat
 Author: yoggys
 Author-email: yoggies@yoggies.ovh
 Keywords: python,unb,unbelievaboat,api,wrapper,async,asyncio
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `unbelievaboat-1.0.6/unbelievaboat.egg-info/SOURCES.txt` & `unbelievaboat-1.1.0/unbelievaboat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

