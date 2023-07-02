# Comparing `tmp/rtorrent_rpc-0.0.7.tar.gz` & `tmp/rtorrent_rpc-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rtorrent_rpc-0.0.7.tar", max compression
+gzip compressed data, was "rtorrent_rpc-0.0.8.tar", max compression
```

## Comparing `rtorrent_rpc-0.0.7.tar` & `rtorrent_rpc-0.0.8.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1084 2023-07-01 17:53:48.588005 rtorrent_rpc-0.0.7/LICENSE
--rw-r--r--   0        0        0     2523 2023-07-01 17:53:48.588005 rtorrent_rpc-0.0.7/pyproject.toml
--rw-r--r--   0        0        0      741 2023-07-01 17:53:48.588005 rtorrent_rpc-0.0.7/readme.md
--rw-r--r--   0        0        0    22583 2023-07-01 17:53:48.592005 rtorrent_rpc-0.0.7/rtorrent_rpc/__init__.py
--rw-r--r--   0        0        0     2098 2023-07-01 17:53:48.592005 rtorrent_rpc-0.0.7/rtorrent_rpc/helper.py
--rw-r--r--   0        0        0        0 2023-07-01 17:53:48.592005 rtorrent_rpc-0.0.7/rtorrent_rpc/py.typed
--rw-r--r--   0        0        0     1644 1970-01-01 00:00:00.000000 rtorrent_rpc-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1084 2023-07-02 01:56:37.638747 rtorrent_rpc-0.0.8/LICENSE
+-rw-r--r--   0        0        0     2523 2023-07-02 01:56:37.638747 rtorrent_rpc-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0      741 2023-07-02 01:56:37.638747 rtorrent_rpc-0.0.8/readme.md
+-rw-r--r--   0        0        0    22594 2023-07-02 01:56:37.638747 rtorrent_rpc-0.0.8/rtorrent_rpc/__init__.py
+-rw-r--r--   0        0        0     2098 2023-07-02 01:56:37.638747 rtorrent_rpc-0.0.8/rtorrent_rpc/helper.py
+-rw-r--r--   0        0        0        0 2023-07-02 01:56:37.638747 rtorrent_rpc-0.0.8/rtorrent_rpc/py.typed
+-rw-r--r--   0        0        0     1644 1970-01-01 00:00:00.000000 rtorrent_rpc-0.0.8/PKG-INFO
```

### Comparing `rtorrent_rpc-0.0.7/LICENSE` & `rtorrent_rpc-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `rtorrent_rpc-0.0.7/pyproject.toml` & `rtorrent_rpc-0.0.8/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "rtorrent-rpc"
-version = "0.0.7"
+version = "0.0.8"
 description = "Typed rtorrent rpc client"
 authors = ["Trim21 <i@trim21.me>"]
 readme = 'readme.md'
 repository = 'https://github.com/trim21/rtorrent-rpc'
 license = 'MIT'
 packages = [{ include = 'rtorrent_rpc' }]
 keywords = ['rtorrent', 'rpc']
```

### Comparing `rtorrent_rpc-0.0.7/readme.md` & `rtorrent_rpc-0.0.8/readme.md`

 * *Files identical despite different names*

### Comparing `rtorrent_rpc-0.0.7/rtorrent_rpc/__init__.py` & `rtorrent_rpc-0.0.8/rtorrent_rpc/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import time
 import urllib.parse
 import xmlrpc.client
-from collections.abc import Iterator
+from collections.abc import Iterable
 from typing import Any, Literal, Protocol, TypeAlias, TypedDict
 
 from rtorrent_xmlrpc import SCGIServerProxy
 from typing_extensions import NotRequired
 
 __all__ = ["RTorrent", "MultiCall"]
 
@@ -60,15 +60,16 @@
         :param directory: download base directory
         :param tags: optional tags for download
         """
         params = [
             "",
             content,
             'd.tied_to_file.set=""',
-            f"d.custom.set=addtime,{int(time.time())}",  # this custom is commonly used by ruTorrent and flood.
+            f"d.custom.set=addtime,{int(time.time())}",
+            # this custom is commonly used by ruTorrent and flood.
             f'd.directory_base.set="{directory}"',
         ]
 
         if tags:
             params.append(f'd.custom1.set="{_encode_tags(tags)}"')
 
         self.rpc.load.raw_start_verbose(*params)
@@ -108,15 +109,15 @@
     @property
     def d(self) -> _DownloadRpc:
         return self.rpc.d
 
     def d_save_resume(self, info_hash: str) -> None:
         return self.rpc.d.save_resume(info_hash)
 
-    def d_set_tags(self, info_hash: str, tags: Iterator[str]) -> None:
+    def d_set_tags(self, info_hash: str, tags: Iterable[str]) -> None:
         """set download tags"""
         self.rpc.d.custom1.set(info_hash, ",".join(tags))
 
 
 _methods = [
     "system.methodExist",
     "system.methodHelp",
```

### Comparing `rtorrent_rpc-0.0.7/rtorrent_rpc/helper.py` & `rtorrent_rpc-0.0.8/rtorrent_rpc/helper.py`

 * *Files identical despite different names*

### Comparing `rtorrent_rpc-0.0.7/PKG-INFO` & `rtorrent_rpc-0.0.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rtorrent-rpc
-Version: 0.0.7
+Version: 0.0.8
 Summary: Typed rtorrent rpc client
 Home-page: https://github.com/trim21/rtorrent-rpc
 License: MIT
 Keywords: rtorrent,rpc
 Author: Trim21
 Author-email: i@trim21.me
 Requires-Python: >=3.10,<4.0
```

