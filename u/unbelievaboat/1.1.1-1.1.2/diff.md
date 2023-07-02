# Comparing `tmp/unbelievaboat-1.1.1.tar.gz` & `tmp/unbelievaboat-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unbelievaboat-1.1.1.tar", last modified: Sun Jul  2 15:11:38 2023, max compression
+gzip compressed data, was "unbelievaboat-1.1.2.tar", last modified: Sun Jul  2 15:29:17 2023, max compression
```

## Comparing `unbelievaboat-1.1.1.tar` & `unbelievaboat-1.1.2.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0        0        0        0 2023-07-02 15:11:38.547157 unbelievaboat-1.1.1/
--rw-rw-rw-   0        0        0     1084 2023-07-01 15:11:46.000000 unbelievaboat-1.1.1/LICENSE
--rw-rw-rw-   0        0        0     3749 2023-07-02 15:11:38.546074 unbelievaboat-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     3008 2023-07-01 20:13:23.000000 unbelievaboat-1.1.1/README.md
--rw-rw-rw-   0        0        0       42 2023-07-02 15:11:38.547157 unbelievaboat-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1084 2023-07-02 15:11:02.000000 unbelievaboat-1.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-02 15:11:38.478247 unbelievaboat-1.1.1/unbelievaboat/
--rw-rw-rw-   0        0        0     7927 2023-07-01 23:56:31.000000 unbelievaboat-1.1.1/unbelievaboat/Client.py
--rw-rw-rw-   0        0        0     3390 2023-07-02 15:10:49.000000 unbelievaboat-1.1.1/unbelievaboat/RequestHandler.py
--rw-rw-rw-   0        0        0      365 2023-07-01 20:39:17.000000 unbelievaboat-1.1.1/unbelievaboat/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-02 15:11:38.522336 unbelievaboat-1.1.1/unbelievaboat/errors/
--rw-rw-rw-   0        0        0      497 2023-07-01 23:17:00.000000 unbelievaboat-1.1.1/unbelievaboat/errors/APIError.py
--rw-rw-rw-   0        0        0      514 2023-07-01 23:17:00.000000 unbelievaboat-1.1.1/unbelievaboat/errors/HTTPError.py
--rw-rw-rw-   0        0        0      105 2023-07-01 13:39:53.000000 unbelievaboat-1.1.1/unbelievaboat/errors/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-02 15:11:38.532858 unbelievaboat-1.1.1/unbelievaboat/structures/
--rw-rw-rw-   0        0        0      925 2023-07-01 16:58:46.000000 unbelievaboat-1.1.1/unbelievaboat/structures/Guild.py
--rw-rw-rw-   0        0        0      750 2023-07-01 20:59:31.000000 unbelievaboat-1.1.1/unbelievaboat/structures/Leaderboard.py
--rw-rw-rw-   0        0        0      929 2023-07-01 16:45:44.000000 unbelievaboat-1.1.1/unbelievaboat/structures/Permission.py
--rw-rw-rw-   0        0        0      711 2023-07-01 20:20:29.000000 unbelievaboat-1.1.1/unbelievaboat/structures/Store.py
--rw-rw-rw-   0        0        0     1306 2023-07-01 20:56:24.000000 unbelievaboat-1.1.1/unbelievaboat/structures/UserBalance.py
--rw-rw-rw-   0        0        0     2103 2023-07-01 23:12:16.000000 unbelievaboat-1.1.1/unbelievaboat/structures/UserInventory.py
--rw-rw-rw-   0        0        0      445 2023-07-01 20:39:39.000000 unbelievaboat-1.1.1/unbelievaboat/structures/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-02 15:11:38.540854 unbelievaboat-1.1.1/unbelievaboat/structures/items/
--rw-rw-rw-   0        0        0     1293 2023-07-01 16:54:27.000000 unbelievaboat-1.1.1/unbelievaboat/structures/items/BaseItem.py
--rw-rw-rw-   0        0        0      955 2023-07-01 22:06:03.000000 unbelievaboat-1.1.1/unbelievaboat/structures/items/InventoryItem.py
--rw-rw-rw-   0        0        0     1501 2023-07-01 20:53:07.000000 unbelievaboat-1.1.1/unbelievaboat/structures/items/StoreItem.py
--rw-rw-rw-   0        0        0     1030 2023-07-01 16:54:52.000000 unbelievaboat-1.1.1/unbelievaboat/structures/items/StoreItemAction.py
--rw-rw-rw-   0        0        0     1296 2023-07-01 16:55:37.000000 unbelievaboat-1.1.1/unbelievaboat/structures/items/StoreItemRequirement.py
--rw-rw-rw-   0        0        0      338 2023-07-01 13:39:53.000000 unbelievaboat-1.1.1/unbelievaboat/structures/items/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-02 15:11:38.544563 unbelievaboat-1.1.1/unbelievaboat/util/
--rw-rw-rw-   0        0        0      383 2023-07-01 12:00:58.000000 unbelievaboat-1.1.1/unbelievaboat/util/Constants.py
--rw-rw-rw-   0        0        0      551 2023-07-01 13:15:13.000000 unbelievaboat-1.1.1/unbelievaboat/util/SnakeCaseConventer.py
--rw-rw-rw-   0        0        0      207 2023-07-02 15:05:17.000000 unbelievaboat-1.1.1/unbelievaboat/util/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-02 15:11:38.518303 unbelievaboat-1.1.1/unbelievaboat.egg-info/
--rw-rw-rw-   0        0        0     3749 2023-07-02 15:11:38.000000 unbelievaboat-1.1.1/unbelievaboat.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1045 2023-07-02 15:11:38.000000 unbelievaboat-1.1.1/unbelievaboat.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-02 15:11:38.000000 unbelievaboat-1.1.1/unbelievaboat.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-07-02 15:11:38.000000 unbelievaboat-1.1.1/unbelievaboat.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-07-02 15:11:38.000000 unbelievaboat-1.1.1/unbelievaboat.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-02 15:29:17.367874 unbelievaboat-1.1.2/
+-rw-rw-rw-   0        0        0     1084 2023-07-01 15:11:46.000000 unbelievaboat-1.1.2/LICENSE
+-rw-rw-rw-   0        0        0     3749 2023-07-02 15:29:17.366873 unbelievaboat-1.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3008 2023-07-01 20:13:23.000000 unbelievaboat-1.1.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-02 15:29:17.367874 unbelievaboat-1.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1084 2023-07-02 15:29:02.000000 unbelievaboat-1.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-02 15:29:17.302178 unbelievaboat-1.1.2/unbelievaboat/
+-rw-rw-rw-   0        0        0     7927 2023-07-01 23:56:31.000000 unbelievaboat-1.1.2/unbelievaboat/Client.py
+-rw-rw-rw-   0        0        0     3390 2023-07-02 15:10:49.000000 unbelievaboat-1.1.2/unbelievaboat/RequestHandler.py
+-rw-rw-rw-   0        0        0      365 2023-07-01 20:39:17.000000 unbelievaboat-1.1.2/unbelievaboat/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-02 15:29:17.337385 unbelievaboat-1.1.2/unbelievaboat/errors/
+-rw-rw-rw-   0        0        0      497 2023-07-01 23:17:00.000000 unbelievaboat-1.1.2/unbelievaboat/errors/APIError.py
+-rw-rw-rw-   0        0        0      514 2023-07-01 23:17:00.000000 unbelievaboat-1.1.2/unbelievaboat/errors/HTTPError.py
+-rw-rw-rw-   0        0        0      105 2023-07-01 13:39:53.000000 unbelievaboat-1.1.2/unbelievaboat/errors/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-02 15:29:17.351556 unbelievaboat-1.1.2/unbelievaboat/structures/
+-rw-rw-rw-   0        0        0      925 2023-07-01 16:58:46.000000 unbelievaboat-1.1.2/unbelievaboat/structures/Guild.py
+-rw-rw-rw-   0        0        0      750 2023-07-01 20:59:31.000000 unbelievaboat-1.1.2/unbelievaboat/structures/Leaderboard.py
+-rw-rw-rw-   0        0        0      929 2023-07-01 16:45:44.000000 unbelievaboat-1.1.2/unbelievaboat/structures/Permission.py
+-rw-rw-rw-   0        0        0      711 2023-07-01 20:20:29.000000 unbelievaboat-1.1.2/unbelievaboat/structures/Store.py
+-rw-rw-rw-   0        0        0     1306 2023-07-01 20:56:24.000000 unbelievaboat-1.1.2/unbelievaboat/structures/UserBalance.py
+-rw-rw-rw-   0        0        0     2103 2023-07-01 23:12:16.000000 unbelievaboat-1.1.2/unbelievaboat/structures/UserInventory.py
+-rw-rw-rw-   0        0        0      445 2023-07-01 20:39:39.000000 unbelievaboat-1.1.2/unbelievaboat/structures/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-02 15:29:17.360815 unbelievaboat-1.1.2/unbelievaboat/structures/items/
+-rw-rw-rw-   0        0        0     1322 2023-07-02 15:20:48.000000 unbelievaboat-1.1.2/unbelievaboat/structures/items/BaseItem.py
+-rw-rw-rw-   0        0        0     1169 2023-07-02 15:20:05.000000 unbelievaboat-1.1.2/unbelievaboat/structures/items/InventoryItem.py
+-rw-rw-rw-   0        0        0     1623 2023-07-02 15:21:56.000000 unbelievaboat-1.1.2/unbelievaboat/structures/items/StoreItem.py
+-rw-rw-rw-   0        0        0     1320 2023-07-02 15:27:56.000000 unbelievaboat-1.1.2/unbelievaboat/structures/items/StoreItemAction.py
+-rw-rw-rw-   0        0        0     1487 2023-07-02 15:27:17.000000 unbelievaboat-1.1.2/unbelievaboat/structures/items/StoreItemRequirement.py
+-rw-rw-rw-   0        0        0      338 2023-07-01 13:39:53.000000 unbelievaboat-1.1.2/unbelievaboat/structures/items/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-02 15:29:17.365866 unbelievaboat-1.1.2/unbelievaboat/util/
+-rw-rw-rw-   0        0        0      383 2023-07-01 12:00:58.000000 unbelievaboat-1.1.2/unbelievaboat/util/Constants.py
+-rw-rw-rw-   0        0        0      551 2023-07-01 13:15:13.000000 unbelievaboat-1.1.2/unbelievaboat/util/SnakeCaseConventer.py
+-rw-rw-rw-   0        0        0      207 2023-07-02 15:05:17.000000 unbelievaboat-1.1.2/unbelievaboat/util/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-02 15:29:17.332422 unbelievaboat-1.1.2/unbelievaboat.egg-info/
+-rw-rw-rw-   0        0        0     3749 2023-07-02 15:29:17.000000 unbelievaboat-1.1.2/unbelievaboat.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1045 2023-07-02 15:29:17.000000 unbelievaboat-1.1.2/unbelievaboat.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-02 15:29:17.000000 unbelievaboat-1.1.2/unbelievaboat.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-07-02 15:29:17.000000 unbelievaboat-1.1.2/unbelievaboat.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-07-02 15:29:17.000000 unbelievaboat-1.1.2/unbelievaboat.egg-info/top_level.txt
```

### Comparing `unbelievaboat-1.1.1/LICENSE` & `unbelievaboat-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `unbelievaboat-1.1.1/PKG-INFO` & `unbelievaboat-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unbelievaboat
-Version: 1.1.1
+Version: 1.1.2
 Summary: Wrapper for UnbelievaBoat API.
 Home-page: https://github.com/yoggys/unbelievaboat
 Author: yoggys
 Author-email: yoggies@yoggies.ovh
 Keywords: python,unb,unbelievaboat,api,wrapper,async,asyncio
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `unbelievaboat-1.1.1/README.md` & `unbelievaboat-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `unbelievaboat-1.1.1/setup.py` & `unbelievaboat-1.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 
 cwd = Path(__file__).parent
 long_description = (cwd / "README.md").read_text()
 
 setup(
     name="unbelievaboat",
-    version="1.1.1",
+    version="1.1.2",
     author="yoggys",
     author_email="yoggies@yoggies.ovh",
     description="Wrapper for UnbelievaBoat API.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/yoggys/unbelievaboat",
     packages=find_packages(),
```

### Comparing `unbelievaboat-1.1.1/unbelievaboat/Client.py` & `unbelievaboat-1.1.2/unbelievaboat/Client.py`

 * *Files identical despite different names*

### Comparing `unbelievaboat-1.1.1/unbelievaboat/RequestHandler.py` & `unbelievaboat-1.1.2/unbelievaboat/RequestHandler.py`

 * *Files identical despite different names*

### Comparing `unbelievaboat-1.1.1/unbelievaboat/errors/HTTPError.py` & `unbelievaboat-1.1.2/unbelievaboat/errors/HTTPError.py`

 * *Files identical despite different names*

### Comparing `unbelievaboat-1.1.1/unbelievaboat/structures/Guild.py` & `unbelievaboat-1.1.2/unbelievaboat/structures/Guild.py`

 * *Files identical despite different names*

### Comparing `unbelievaboat-1.1.1/unbelievaboat/structures/Leaderboard.py` & `unbelievaboat-1.1.2/unbelievaboat/structures/Leaderboard.py`

 * *Files identical despite different names*

### Comparing `unbelievaboat-1.1.1/unbelievaboat/structures/Permission.py` & `unbelievaboat-1.1.2/unbelievaboat/structures/Permission.py`

 * *Files identical despite different names*

### Comparing `unbelievaboat-1.1.1/unbelievaboat/structures/Store.py` & `unbelievaboat-1.1.2/unbelievaboat/structures/Store.py`

 * *Files identical despite different names*

### Comparing `unbelievaboat-1.1.1/unbelievaboat/structures/UserBalance.py` & `unbelievaboat-1.1.2/unbelievaboat/structures/UserBalance.py`

 * *Files identical despite different names*

### Comparing `unbelievaboat-1.1.1/unbelievaboat/structures/UserInventory.py` & `unbelievaboat-1.1.2/unbelievaboat/structures/UserInventory.py`

 * *Files identical despite different names*

### Comparing `unbelievaboat-1.1.1/unbelievaboat/structures/items/BaseItem.py` & `unbelievaboat-1.1.2/unbelievaboat/structures/items/BaseItem.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,18 +7,19 @@
 class BaseItem:
     def __init__(self, data: Dict[str, Any]) -> None:
         self.name: str = data["name"]
         self.description: Optional[str] = data.get("description", None)
         self.is_usable: bool = data["is_usable"]
         self.is_sellable: bool = data["is_sellable"]
         self.requirements: List[StoreItemRequirement] = [
-            StoreItemRequirement(requirement) for requirement in data["requirements"]
+            StoreItemRequirement(requirement)
+            for requirement in data.get("requirements", [])
         ]
         self.actions: List[StoreItemAction] = [
-            StoreItemAction(action) for action in data["actions"]
+            StoreItemAction(action) for action in data.get("actions", [])
         ]
         self.emoji_unicode: Optional[str] = data.get("emoji_unicode", None)
         self.emoji_id: Optional[str] = data.get("emoji_id", None)
 
     def __str__(self) -> str:
         return "<BaseItem name={} description={} is_usable={} is_sellable={} requirements={} actions={} emoji_unicode={} emoji_id={}>".format(
             self.name,
```

### Comparing `unbelievaboat-1.1.1/unbelievaboat/structures/items/StoreItem.py` & `unbelievaboat-1.1.2/unbelievaboat/structures/items/StoreItem.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,22 +18,24 @@
             if data.get("expires_at")
             else None
         )
 
         self._client = client
 
     def __str__(self) -> str:
-        return "<StoreItem id={} guild_id={} price={} is_inventory={} stock_remaining={} unlimited_stock={} expires_at={}>".format(
+        return "<StoreItem id={} guild_id={} price={} is_inventory={} stock_remaining={} unlimited_stock={} expires_at={} actions={} requirements={}>".format(
             self.id,
             self.guild_id,
             self.price,
             self.is_inventory,
             self.stock_remaining,
             self.unlimited_stock,
             self.expires_at,
+            [str(a) for a in self.actions],
+            [str(r) for r in self.requirements],
         )
 
     async def edit(
         self, data: Dict[str, Any] = {}, params: Dict[str, Any] = {}
     ) -> Self:
         self = await self._client.edit_store_item(self.guild_id, self.id, data, params)
         return self
```

### Comparing `unbelievaboat-1.1.1/unbelievaboat/structures/items/StoreItemAction.py` & `unbelievaboat-1.1.2/unbelievaboat/structures/items/StoreItemAction.py`

 * *Files 24% similar despite different names*

```diff
@@ -19,10 +19,19 @@
         elif self.type in [ItemActionType.ADD_BALANCE, ItemActionType.REMOVE_BALANCE]:
             self.balance: Optional[int] = data.get("balance")
 
     def toJSON(self) -> dict:
         return {"type": self.type.value, **self.__dict__}
 
     def __str__(self) -> str:
-        return "<StoreItemAction type={} message={} ids={} balance={}>".format(
-            self.type, self.message, self.ids, self.balance
-        )
+        if hasattr(self, "message"):
+            return "<StoreItemAction type={} message={}>".format(
+                self.type, self.message
+            )
+
+        if hasattr(self, "ids"):
+            return "<StoreItemAction type={} ids={}>".format(self.type, self.ids)
+
+        if hasattr(self, "balance"):
+            return "<StoreItemAction type={} balance={}>".format(
+                self.type, self.balance
+            )
```

### Comparing `unbelievaboat-1.1.1/unbelievaboat/structures/items/StoreItemRequirement.py` & `unbelievaboat-1.1.2/unbelievaboat/structures/items/StoreItemRequirement.py`

 * *Files 14% similar despite different names*

```diff
@@ -23,10 +23,16 @@
         if self.type in [ItemRequirementType.ROLE, ItemRequirementType.ITEM]:
             json["ids"] = self.ids
         elif self.type == ItemRequirementType.TOTAL_BALANCE:
             json["balance"] = self.balance
         return json
 
     def __str__(self) -> str:
-        return "<StoreItemRequirement type={} matchType={} ids={} balance={}>".format(
-            self.type, self.matchType, self.ids, self.balance
-        )
+        if hasattr(self, "matchType"):
+            return "<StoreItemRequirement type={} matchType={} ids={}>".format(
+                self.type, self.matchType, self.ids
+            )
+
+        if hasattr(self, "ids"):
+            return "<StoreItemRequirement type={} balance={}>".format(
+                self.type, self.balance
+            )
```

### Comparing `unbelievaboat-1.1.1/unbelievaboat/util/SnakeCaseConventer.py` & `unbelievaboat-1.1.2/unbelievaboat/util/SnakeCaseConventer.py`

 * *Files identical despite different names*

### Comparing `unbelievaboat-1.1.1/unbelievaboat.egg-info/PKG-INFO` & `unbelievaboat-1.1.2/unbelievaboat.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unbelievaboat
-Version: 1.1.1
+Version: 1.1.2
 Summary: Wrapper for UnbelievaBoat API.
 Home-page: https://github.com/yoggys/unbelievaboat
 Author: yoggys
 Author-email: yoggies@yoggies.ovh
 Keywords: python,unb,unbelievaboat,api,wrapper,async,asyncio
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `unbelievaboat-1.1.1/unbelievaboat.egg-info/SOURCES.txt` & `unbelievaboat-1.1.2/unbelievaboat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

