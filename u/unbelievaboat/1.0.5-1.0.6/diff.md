# Comparing `tmp/unbelievaboat-1.0.5.tar.gz` & `tmp/unbelievaboat-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unbelievaboat-1.0.5.tar", last modified: Sat Jul  1 18:54:31 2023, max compression
+gzip compressed data, was "unbelievaboat-1.0.6.tar", last modified: Sat Jul  1 22:48:57 2023, max compression
```

## Comparing `unbelievaboat-1.0.5.tar` & `unbelievaboat-1.0.6.tar`

### file list

```diff
@@ -1,39 +1,40 @@
-drwxrwxrwx   0        0        0        0 2023-07-01 18:54:31.540339 unbelievaboat-1.0.5/
--rw-rw-rw-   0        0        0     1084 2023-07-01 15:11:46.000000 unbelievaboat-1.0.5/LICENSE
--rw-rw-rw-   0        0        0     3749 2023-07-01 18:54:31.538342 unbelievaboat-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     3008 2023-07-01 18:53:47.000000 unbelievaboat-1.0.5/README.md
--rw-rw-rw-   0        0        0       42 2023-07-01 18:54:31.541690 unbelievaboat-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1084 2023-07-01 18:54:13.000000 unbelievaboat-1.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-01 18:54:31.331824 unbelievaboat-1.0.5/unbelievaboat/
--rw-rw-rw-   0        0        0     5584 2023-07-01 16:55:18.000000 unbelievaboat-1.0.5/unbelievaboat/Client.py
--rw-rw-rw-   0        0        0     3133 2023-07-01 14:59:51.000000 unbelievaboat-1.0.5/unbelievaboat/RequestHandler.py
--rw-rw-rw-   0        0        0      336 2023-07-01 14:55:29.000000 unbelievaboat-1.0.5/unbelievaboat/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-01 18:54:31.433503 unbelievaboat-1.0.5/unbelievaboat/errors/
--rw-rw-rw-   0        0        0      572 2023-07-01 11:55:22.000000 unbelievaboat-1.0.5/unbelievaboat/errors/APIError.py
--rw-rw-rw-   0        0        0      551 2023-07-01 13:35:00.000000 unbelievaboat-1.0.5/unbelievaboat/errors/HTTPError.py
--rw-rw-rw-   0        0        0      105 2023-07-01 13:39:53.000000 unbelievaboat-1.0.5/unbelievaboat/errors/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-01 18:54:31.490214 unbelievaboat-1.0.5/unbelievaboat/structures/
--rw-rw-rw-   0        0        0      925 2023-07-01 16:58:46.000000 unbelievaboat-1.0.5/unbelievaboat/structures/Guild.py
--rw-rw-rw-   0        0        0      728 2023-07-01 16:59:19.000000 unbelievaboat-1.0.5/unbelievaboat/structures/Leaderboard.py
--rw-rw-rw-   0        0        0      929 2023-07-01 16:45:44.000000 unbelievaboat-1.0.5/unbelievaboat/structures/Permission.py
--rw-rw-rw-   0        0        0      704 2023-07-01 16:45:44.000000 unbelievaboat-1.0.5/unbelievaboat/structures/Store.py
--rw-rw-rw-   0        0        0     1258 2023-07-01 18:53:50.000000 unbelievaboat-1.0.5/unbelievaboat/structures/User.py
--rw-rw-rw-   0        0        0      362 2023-07-01 14:56:55.000000 unbelievaboat-1.0.5/unbelievaboat/structures/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-01 18:54:31.519812 unbelievaboat-1.0.5/unbelievaboat/structures/items/
--rw-rw-rw-   0        0        0     1293 2023-07-01 16:54:27.000000 unbelievaboat-1.0.5/unbelievaboat/structures/items/BaseItem.py
--rw-rw-rw-   0        0        0      429 2023-07-01 16:54:36.000000 unbelievaboat-1.0.5/unbelievaboat/structures/items/InventoryItem.py
--rw-rw-rw-   0        0        0     1353 2023-07-01 16:57:10.000000 unbelievaboat-1.0.5/unbelievaboat/structures/items/StoreItem.py
--rw-rw-rw-   0        0        0     1030 2023-07-01 16:54:52.000000 unbelievaboat-1.0.5/unbelievaboat/structures/items/StoreItemAction.py
--rw-rw-rw-   0        0        0     1296 2023-07-01 16:55:37.000000 unbelievaboat-1.0.5/unbelievaboat/structures/items/StoreItemRequirement.py
--rw-rw-rw-   0        0        0      338 2023-07-01 13:39:53.000000 unbelievaboat-1.0.5/unbelievaboat/structures/items/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-01 18:54:31.534342 unbelievaboat-1.0.5/unbelievaboat/util/
--rw-rw-rw-   0        0        0     1143 2023-07-01 11:45:16.000000 unbelievaboat-1.0.5/unbelievaboat/util/Bucket.py
--rw-rw-rw-   0        0        0      383 2023-07-01 12:00:58.000000 unbelievaboat-1.0.5/unbelievaboat/util/Constants.py
--rw-rw-rw-   0        0        0      551 2023-07-01 13:15:13.000000 unbelievaboat-1.0.5/unbelievaboat/util/SnakeCaseConventer.py
--rw-rw-rw-   0        0        0      250 2023-07-01 13:41:07.000000 unbelievaboat-1.0.5/unbelievaboat/util/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-01 18:54:31.417418 unbelievaboat-1.0.5/unbelievaboat.egg-info/
--rw-rw-rw-   0        0        0     3749 2023-07-01 18:54:31.000000 unbelievaboat-1.0.5/unbelievaboat.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1025 2023-07-01 18:54:31.000000 unbelievaboat-1.0.5/unbelievaboat.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-01 18:54:31.000000 unbelievaboat-1.0.5/unbelievaboat.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-07-01 18:54:31.000000 unbelievaboat-1.0.5/unbelievaboat.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-07-01 18:54:31.000000 unbelievaboat-1.0.5/unbelievaboat.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-01 22:48:57.963254 unbelievaboat-1.0.6/
+-rw-rw-rw-   0        0        0     1084 2023-07-01 15:11:46.000000 unbelievaboat-1.0.6/LICENSE
+-rw-rw-rw-   0        0        0     3749 2023-07-01 22:48:57.962238 unbelievaboat-1.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     3008 2023-07-01 20:13:23.000000 unbelievaboat-1.0.6/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-01 22:48:57.963254 unbelievaboat-1.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1084 2023-07-01 22:48:32.000000 unbelievaboat-1.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-01 22:48:57.890012 unbelievaboat-1.0.6/unbelievaboat/
+-rw-rw-rw-   0        0        0     7927 2023-07-01 22:45:49.000000 unbelievaboat-1.0.6/unbelievaboat/Client.py
+-rw-rw-rw-   0        0        0     3301 2023-07-01 22:39:10.000000 unbelievaboat-1.0.6/unbelievaboat/RequestHandler.py
+-rw-rw-rw-   0        0        0      365 2023-07-01 20:39:17.000000 unbelievaboat-1.0.6/unbelievaboat/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-01 22:48:57.934340 unbelievaboat-1.0.6/unbelievaboat/errors/
+-rw-rw-rw-   0        0        0      509 2023-07-01 22:42:38.000000 unbelievaboat-1.0.6/unbelievaboat/errors/APIError.py
+-rw-rw-rw-   0        0        0      518 2023-07-01 22:42:02.000000 unbelievaboat-1.0.6/unbelievaboat/errors/HTTPError.py
+-rw-rw-rw-   0        0        0      105 2023-07-01 13:39:53.000000 unbelievaboat-1.0.6/unbelievaboat/errors/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-01 22:48:57.944557 unbelievaboat-1.0.6/unbelievaboat/structures/
+-rw-rw-rw-   0        0        0      925 2023-07-01 16:58:46.000000 unbelievaboat-1.0.6/unbelievaboat/structures/Guild.py
+-rw-rw-rw-   0        0        0      750 2023-07-01 20:59:31.000000 unbelievaboat-1.0.6/unbelievaboat/structures/Leaderboard.py
+-rw-rw-rw-   0        0        0      929 2023-07-01 16:45:44.000000 unbelievaboat-1.0.6/unbelievaboat/structures/Permission.py
+-rw-rw-rw-   0        0        0      711 2023-07-01 20:20:29.000000 unbelievaboat-1.0.6/unbelievaboat/structures/Store.py
+-rw-rw-rw-   0        0        0     1306 2023-07-01 20:56:24.000000 unbelievaboat-1.0.6/unbelievaboat/structures/UserBalance.py
+-rw-rw-rw-   0        0        0     2079 2023-07-01 22:32:11.000000 unbelievaboat-1.0.6/unbelievaboat/structures/UserInventory.py
+-rw-rw-rw-   0        0        0      445 2023-07-01 20:39:39.000000 unbelievaboat-1.0.6/unbelievaboat/structures/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-01 22:48:57.955263 unbelievaboat-1.0.6/unbelievaboat/structures/items/
+-rw-rw-rw-   0        0        0     1293 2023-07-01 16:54:27.000000 unbelievaboat-1.0.6/unbelievaboat/structures/items/BaseItem.py
+-rw-rw-rw-   0        0        0      955 2023-07-01 22:06:03.000000 unbelievaboat-1.0.6/unbelievaboat/structures/items/InventoryItem.py
+-rw-rw-rw-   0        0        0     1501 2023-07-01 20:53:07.000000 unbelievaboat-1.0.6/unbelievaboat/structures/items/StoreItem.py
+-rw-rw-rw-   0        0        0     1030 2023-07-01 16:54:52.000000 unbelievaboat-1.0.6/unbelievaboat/structures/items/StoreItemAction.py
+-rw-rw-rw-   0        0        0     1296 2023-07-01 16:55:37.000000 unbelievaboat-1.0.6/unbelievaboat/structures/items/StoreItemRequirement.py
+-rw-rw-rw-   0        0        0      338 2023-07-01 13:39:53.000000 unbelievaboat-1.0.6/unbelievaboat/structures/items/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-01 22:48:57.961182 unbelievaboat-1.0.6/unbelievaboat/util/
+-rw-rw-rw-   0        0        0     1143 2023-07-01 11:45:16.000000 unbelievaboat-1.0.6/unbelievaboat/util/Bucket.py
+-rw-rw-rw-   0        0        0      383 2023-07-01 12:00:58.000000 unbelievaboat-1.0.6/unbelievaboat/util/Constants.py
+-rw-rw-rw-   0        0        0      551 2023-07-01 13:15:13.000000 unbelievaboat-1.0.6/unbelievaboat/util/SnakeCaseConventer.py
+-rw-rw-rw-   0        0        0      250 2023-07-01 13:41:07.000000 unbelievaboat-1.0.6/unbelievaboat/util/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-01 22:48:57.929573 unbelievaboat-1.0.6/unbelievaboat.egg-info/
+-rw-rw-rw-   0        0        0     3749 2023-07-01 22:48:57.000000 unbelievaboat-1.0.6/unbelievaboat.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1074 2023-07-01 22:48:57.000000 unbelievaboat-1.0.6/unbelievaboat.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-01 22:48:57.000000 unbelievaboat-1.0.6/unbelievaboat.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-07-01 22:48:57.000000 unbelievaboat-1.0.6/unbelievaboat.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-07-01 22:48:57.000000 unbelievaboat-1.0.6/unbelievaboat.egg-info/top_level.txt
```

### Comparing `unbelievaboat-1.0.5/LICENSE` & `unbelievaboat-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `unbelievaboat-1.0.5/PKG-INFO` & `unbelievaboat-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unbelievaboat
-Version: 1.0.5
+Version: 1.0.6
 Summary: Wrapper for UnbelievaBoat API.
 Home-page: https://github.com/yoggys/unbelievaboat
 Author: yoggys
 Author-email: yoggies@yoggies.ovh
 Keywords: python,unb,unbelievaboat,api,wrapper,async,asyncio
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `unbelievaboat-1.0.5/README.md` & `unbelievaboat-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `unbelievaboat-1.0.5/setup.py` & `unbelievaboat-1.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 
 cwd = Path(__file__).parent
 long_description = (cwd / "README.md").read_text()
 
 setup(
     name="unbelievaboat",
-    version="1.0.5",
+    version="1.0.6",
     author="yoggys",
     author_email="yoggies@yoggies.ovh",
     description="Wrapper for UnbelievaBoat API.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/yoggys/unbelievaboat",
     packages=find_packages(),
```

### Comparing `unbelievaboat-1.0.5/unbelievaboat/RequestHandler.py` & `unbelievaboat-1.0.6/unbelievaboat/RequestHandler.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import json
 from typing import Any, Dict, Optional
 
 from .errors import APIError, HTTPError
 from .util import Bucket
 
 
 class RequestHandler:
@@ -45,23 +46,26 @@
                 # Increase the number of attempts
                 _attempts += 1
 
                 # Add the rate limit header data to the bucket
                 self.parse_rate_limit_headers(route, response.headers)
 
                 if response.status >= 200 and response.status < 300:
-                    return await response.json()
+                    try:
+                        return await response.json()
+                    except:
+                        return json.dumps(await response.text())
 
                 if response.status == 429:
                     if _attempts >= self._client._max_retries:
                         raise APIError(response)
                     else:
                         await self.request(method, endpoint, data, params, _attempts)
 
-                raise HTTPError(response)
+                raise HTTPError(response.status, await response.json())
 
     def get_route(self, method: str, endpoint: str) -> str:
         import re
 
         major_params = ["guilds"]
         route = re.sub(
             r"/([a-z-]+)/(?:(\d+))",
```

### Comparing `unbelievaboat-1.0.5/unbelievaboat/errors/HTTPError.py` & `unbelievaboat-1.0.6/unbelievaboat/errors/HTTPError.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,16 @@
+from typing import Any, Dict
+
 import aiohttp
 
 
 class HTTPError(Exception):
-    def __init__(self, response: aiohttp.ClientResponse) -> None:
+    def __init__(self, status: int, data: Dict[str, Any], response: aiohttp.ClientResponse) -> None:
         super().__init__(response)
         self.name: str = self.__class__.__name__
-        self.status: int = response.status
-        self.message: str = (
-            response.status_text
-            if hasattr(response, "status_text")
-            else "Unknown error"
-        )
+        self.status: int = status
+        self.message: str = data.get("message") or "Unknown error"
 
         self.response: aiohttp.ClientResponse = response
 
     def __str__(self):
         return f"HTTP Error {self.status}: {self.message}"
```

### Comparing `unbelievaboat-1.0.5/unbelievaboat/structures/Guild.py` & `unbelievaboat-1.0.6/unbelievaboat/structures/Guild.py`

 * *Files identical despite different names*

### Comparing `unbelievaboat-1.0.5/unbelievaboat/structures/Leaderboard.py` & `unbelievaboat-1.0.6/unbelievaboat/structures/Leaderboard.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from typing import Any, Dict, List
 
-from .User import User
+from .UserBalance import UserBalance
 
 
 class Leaderboard:
     def __init__(self, client, data: Dict[str, Any] = {}) -> None:
         self.guild_id: str = data.get("guild_id")
-        self.users: List[User] = [
-            User(client, {**user, "guild_id": self.guild_id})
+        self.users: List[UserBalance] = [
+            UserBalance(client, {**user, "guild_id": self.guild_id})
             for user in data.get("users", [])
         ]
-        self.total_pages: int = data.get("total_pages", 1)
-        self.page: int = data.get("page", 1)
+        self.total_pages: int = data.get("total_pages")
+        self.page: int = data.get("page")
 
     def __str__(self) -> str:
         return "<Leaderboard guild_id={} users={} total_pages={} page={}>".format(
             self.guild_id,
             [str(user) for user in self.users],
             self.total_pages,
             self.page,
```

### Comparing `unbelievaboat-1.0.5/unbelievaboat/structures/Permission.py` & `unbelievaboat-1.0.6/unbelievaboat/structures/Permission.py`

 * *Files identical despite different names*

### Comparing `unbelievaboat-1.0.5/unbelievaboat/structures/Store.py` & `unbelievaboat-1.0.6/unbelievaboat/structures/Store.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-from typing import List, Optional
+from typing import List
 
 from .items import StoreItem
 
 
 class Store:
     def __init__(self, client, data: dict = {}) -> None:
         self.guild_id: str = data.get("guild_id")
-        self.items = [
+        self.items: List[StoreItem] = [
             StoreItem(client, {**item, "guild_id": self.guild_id})
             for item in data.get("items", [])
         ]
         self.total_pages: int = data.get("total_pages", 1)
         self.page: int = data.get("page", 1)
 
     def __str__(self) -> str:
```

### Comparing `unbelievaboat-1.0.5/unbelievaboat/structures/User.py` & `unbelievaboat-1.0.6/unbelievaboat/structures/UserBalance.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 from typing import Any, Dict, Optional, Self
 
 
-class User:
+class UserBalance:
     def __init__(self, client, data: Dict[str, Any] = {}) -> None:
         self.guild_id: str = data.get("guild_id")
         self.user_id: str = data.get("user_id")
         self.rank: Optional[int] = data.get("rank")
         self.cash: int = data.get("cash")
         self.bank: int = data.get("bank")
         self.total: int = data.get("total")
 
         self._client = client
         self._raw_data: Dict[str, Any] = data
 
     def __str__(self) -> str:
-        return "<User id={} guild_id={} rank={} cash={} bank={} total={}>".format(
-            self.id, self.guild_id, self.rank, self.cash, self.bank, self.total
+        return (
+            "<UserBalance id={} guild_id={} rank={} cash={} bank={} total={}>".format(
+                self.id, self.guild_id, self.rank, self.cash, self.bank, self.total
+            )
         )
 
     @property
     def id(self) -> str:
         return self.user_id
 
     async def set_balance(self, data: Dict[str, Any] = {}, reason: str = None) -> Self:
```

### Comparing `unbelievaboat-1.0.5/unbelievaboat/structures/items/BaseItem.py` & `unbelievaboat-1.0.6/unbelievaboat/structures/items/BaseItem.py`

 * *Files identical despite different names*

### Comparing `unbelievaboat-1.0.5/unbelievaboat/structures/items/StoreItem.py` & `unbelievaboat-1.0.6/unbelievaboat/structures/items/StoreItem.py`

 * *Files 16% similar despite different names*

```diff
@@ -31,9 +31,12 @@
             self.unlimited_stock,
             self.expires_at,
         )
 
     async def edit(
         self, data: Dict[str, Any] = {}, params: Dict[str, Any] = {}
     ) -> Self:
-        self = await self._client.edit_item(self.guild_id, self.id, data, params)
+        self = await self._client.edit_store_item(self.guild_id, self.id, data, params)
         return self
+
+    async def delete(self, cascade: bool = False) -> None:
+        self = await self._client.delete_item(self.guild_id, self.id, cascade)
```

### Comparing `unbelievaboat-1.0.5/unbelievaboat/structures/items/StoreItemAction.py` & `unbelievaboat-1.0.6/unbelievaboat/structures/items/StoreItemAction.py`

 * *Files identical despite different names*

### Comparing `unbelievaboat-1.0.5/unbelievaboat/structures/items/StoreItemRequirement.py` & `unbelievaboat-1.0.6/unbelievaboat/structures/items/StoreItemRequirement.py`

 * *Files identical despite different names*

### Comparing `unbelievaboat-1.0.5/unbelievaboat/util/Bucket.py` & `unbelievaboat-1.0.6/unbelievaboat/util/Bucket.py`

 * *Files identical despite different names*

### Comparing `unbelievaboat-1.0.5/unbelievaboat/util/SnakeCaseConventer.py` & `unbelievaboat-1.0.6/unbelievaboat/util/SnakeCaseConventer.py`

 * *Files identical despite different names*

### Comparing `unbelievaboat-1.0.5/unbelievaboat.egg-info/PKG-INFO` & `unbelievaboat-1.0.6/unbelievaboat.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unbelievaboat
-Version: 1.0.5
+Version: 1.0.6
 Summary: Wrapper for UnbelievaBoat API.
 Home-page: https://github.com/yoggys/unbelievaboat
 Author: yoggys
 Author-email: yoggies@yoggies.ovh
 Keywords: python,unb,unbelievaboat,api,wrapper,async,asyncio
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `unbelievaboat-1.0.5/unbelievaboat.egg-info/SOURCES.txt` & `unbelievaboat-1.0.6/unbelievaboat.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -12,15 +12,16 @@
 unbelievaboat/errors/APIError.py
 unbelievaboat/errors/HTTPError.py
 unbelievaboat/errors/__init__.py
 unbelievaboat/structures/Guild.py
 unbelievaboat/structures/Leaderboard.py
 unbelievaboat/structures/Permission.py
 unbelievaboat/structures/Store.py
-unbelievaboat/structures/User.py
+unbelievaboat/structures/UserBalance.py
+unbelievaboat/structures/UserInventory.py
 unbelievaboat/structures/__init__.py
 unbelievaboat/structures/items/BaseItem.py
 unbelievaboat/structures/items/InventoryItem.py
 unbelievaboat/structures/items/StoreItem.py
 unbelievaboat/structures/items/StoreItemAction.py
 unbelievaboat/structures/items/StoreItemRequirement.py
 unbelievaboat/structures/items/__init__.py
```

