# Comparing `tmp/pyrosimple-2.8.0.tar.gz` & `tmp/pyrosimple-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrosimple-2.8.0.tar", max compression
+gzip compressed data, was "pyrosimple-2.9.0.tar", max compression
```

## Comparing `pyrosimple-2.8.0.tar` & `pyrosimple-2.9.0.tar`

### file list

```diff
@@ -1,43 +1,44 @@
--rw-r--r--   0        0        0     2131 2023-04-13 23:28:24.964236 pyrosimple-2.8.0/README.md
--rw-r--r--   0        0        0     3349 2023-04-29 17:00:31.095411 pyrosimple-2.8.0/pyproject.toml
--rw-r--r--   0        0        0      538 2023-04-13 23:28:24.974236 pyrosimple-2.8.0/src/pyrosimple/__init__.py
--rw-r--r--   0        0        0     8723 2023-04-29 15:30:45.920385 pyrosimple-2.8.0/src/pyrosimple/config.py
--rw-r--r--   0        0        0       67 2023-04-13 23:29:22.257480 pyrosimple-2.8.0/src/pyrosimple/data/__init__.py
--rw-r--r--   0        0        0    10194 2023-04-13 23:28:24.977569 pyrosimple-2.8.0/src/pyrosimple/data/full-example.rc
--rw-r--r--   0        0        0     1273 2023-04-13 23:28:24.977569 pyrosimple-2.8.0/src/pyrosimple/error.py
--rw-r--r--   0        0        0        0 2023-04-13 23:28:24.977569 pyrosimple-2.8.0/src/pyrosimple/io/__init__.py
--rw-r--r--   0        0        0     8616 2023-04-20 06:43:18.099234 pyrosimple-2.8.0/src/pyrosimple/io/scgi.py
--rw-r--r--   0        0        0        0 2023-04-13 23:28:24.977569 pyrosimple-2.8.0/src/pyrosimple/job/__init__.py
--rw-r--r--   0        0        0     2963 2023-04-13 23:28:24.977569 pyrosimple-2.8.0/src/pyrosimple/job/action.py
--rw-r--r--   0        0        0     2977 2023-04-13 23:28:24.977569 pyrosimple-2.8.0/src/pyrosimple/job/base.py
--rw-r--r--   0        0        0     9444 2023-04-13 23:29:22.257480 pyrosimple-2.8.0/src/pyrosimple/job/metrics.py
--rw-r--r--   0        0        0     1691 2023-04-13 23:28:24.977569 pyrosimple-2.8.0/src/pyrosimple/job/move_path.py
--rw-r--r--   0        0        0     1743 2023-04-13 23:28:24.977569 pyrosimple-2.8.0/src/pyrosimple/job/move_torrent.py
--rw-r--r--   0        0        0     4197 2023-04-13 23:28:24.977569 pyrosimple-2.8.0/src/pyrosimple/job/queue.py
--rw-r--r--   0        0        0     9954 2023-04-13 23:29:54.100762 pyrosimple-2.8.0/src/pyrosimple/job/watch.py
--rw-r--r--   0        0        0        0 2023-04-13 23:28:24.977569 pyrosimple-2.8.0/src/pyrosimple/py.typed
--rw-r--r--   0        0        0      112 2023-04-13 23:28:24.977569 pyrosimple-2.8.0/src/pyrosimple/scripts/__init__.py
--rw-r--r--   0        0        0     8094 2023-04-14 00:40:44.581127 pyrosimple-2.8.0/src/pyrosimple/scripts/base.py
--rw-r--r--   0        0        0    17593 2023-04-13 23:38:22.673176 pyrosimple-2.8.0/src/pyrosimple/scripts/chtor.py
--rw-r--r--   0        0        0     6590 2023-04-13 23:29:22.260813 pyrosimple-2.8.0/src/pyrosimple/scripts/lstor.py
--rw-r--r--   0        0        0     9723 2023-04-13 23:29:22.260813 pyrosimple-2.8.0/src/pyrosimple/scripts/mktor.py
--rw-r--r--   0        0        0    13632 2023-04-29 15:30:45.910385 pyrosimple-2.8.0/src/pyrosimple/scripts/pyroadmin.py
--rw-r--r--   0        0        0     9555 2023-04-13 23:29:22.260813 pyrosimple-2.8.0/src/pyrosimple/scripts/pyrotorque.py
--rw-r--r--   0        0        0    35338 2023-04-13 23:29:22.260813 pyrosimple-2.8.0/src/pyrosimple/scripts/rtcontrol.py
--rw-r--r--   0        0        0    10294 2023-04-13 23:28:24.980902 pyrosimple-2.8.0/src/pyrosimple/scripts/rtxmlrpc.py
--rw-r--r--   0        0        0      117 2023-04-13 23:28:24.980902 pyrosimple-2.8.0/src/pyrosimple/torrent/__init__.py
--rw-r--r--   0        0        0    30437 2023-04-29 17:00:31.095411 pyrosimple-2.8.0/src/pyrosimple/torrent/engine.py
--rw-r--r--   0        0        0    37020 2023-04-19 03:02:54.236669 pyrosimple-2.8.0/src/pyrosimple/torrent/rtorrent.py
--rw-r--r--   0        0        0      118 2023-04-13 23:28:24.984236 pyrosimple-2.8.0/src/pyrosimple/ui/__init__.py
--rw-r--r--   0        0        0     2903 2023-04-13 23:28:24.984236 pyrosimple-2.8.0/src/pyrosimple/ui/categories.py
--rw-r--r--   0        0        0      122 2023-04-13 23:28:24.984236 pyrosimple-2.8.0/src/pyrosimple/util/__init__.py
--rw-r--r--   0        0        0     2164 2023-04-19 02:04:04.304690 pyrosimple-2.8.0/src/pyrosimple/util/cache.py
--rw-r--r--   0        0        0     7891 2023-04-13 23:28:24.984236 pyrosimple-2.8.0/src/pyrosimple/util/fmt.py
--rw-r--r--   0        0        0      459 2023-04-13 23:28:24.984236 pyrosimple-2.8.0/src/pyrosimple/util/logutil.py
--rw-r--r--   0        0        0    31824 2023-04-13 23:38:22.676510 pyrosimple-2.8.0/src/pyrosimple/util/matching.py
--rw-r--r--   0        0        0    26411 2023-04-13 23:29:22.267480 pyrosimple-2.8.0/src/pyrosimple/util/metafile.py
--rw-r--r--   0        0        0     1999 2023-04-13 23:28:24.984236 pyrosimple-2.8.0/src/pyrosimple/util/pymagic.py
--rwxr-xr-x   0        0        0     9554 2023-04-13 23:29:22.267480 pyrosimple-2.8.0/src/pyrosimple/util/rpc.py
--rw-r--r--   0        0        0     8584 2023-04-19 02:15:38.352321 pyrosimple-2.8.0/src/pyrosimple/util/traits.py
--rw-r--r--   0        0        0     2187 2023-04-13 23:28:24.984236 pyrosimple-2.8.0/src/pyrosimple/util/ui.py
--rw-r--r--   0        0        0     4287 1970-01-01 00:00:00.000000 pyrosimple-2.8.0/PKG-INFO
+-rw-r--r--   0        0        0     2131 2023-04-13 23:28:24.964236 pyrosimple-2.9.0/README.md
+-rw-r--r--   0        0        0     3349 2023-07-02 14:02:08.845891 pyrosimple-2.9.0/pyproject.toml
+-rw-r--r--   0        0        0      538 2023-04-13 23:28:24.974236 pyrosimple-2.9.0/src/pyrosimple/__init__.py
+-rw-r--r--   0        0        0     8778 2023-05-20 14:13:17.963479 pyrosimple-2.9.0/src/pyrosimple/config.py
+-rw-r--r--   0        0        0       67 2023-04-13 23:29:22.257480 pyrosimple-2.9.0/src/pyrosimple/data/__init__.py
+-rw-r--r--   0        0        0    10194 2023-04-13 23:28:24.977569 pyrosimple-2.9.0/src/pyrosimple/data/full-example.rc
+-rw-r--r--   0        0        0     1273 2023-04-13 23:28:24.977569 pyrosimple-2.9.0/src/pyrosimple/error.py
+-rw-r--r--   0        0        0        0 2023-04-13 23:28:24.977569 pyrosimple-2.9.0/src/pyrosimple/io/__init__.py
+-rw-r--r--   0        0        0     8666 2023-06-13 22:46:07.960229 pyrosimple-2.9.0/src/pyrosimple/io/scgi.py
+-rw-r--r--   0        0        0        0 2023-04-13 23:28:24.977569 pyrosimple-2.9.0/src/pyrosimple/job/__init__.py
+-rw-r--r--   0        0        0     2963 2023-04-13 23:28:24.977569 pyrosimple-2.9.0/src/pyrosimple/job/action.py
+-rw-r--r--   0        0        0     2977 2023-04-13 23:28:24.977569 pyrosimple-2.9.0/src/pyrosimple/job/base.py
+-rw-r--r--   0        0        0     9444 2023-04-13 23:29:22.257480 pyrosimple-2.9.0/src/pyrosimple/job/metrics.py
+-rw-r--r--   0        0        0     1691 2023-04-13 23:28:24.977569 pyrosimple-2.9.0/src/pyrosimple/job/move_path.py
+-rw-r--r--   0        0        0     1743 2023-04-13 23:28:24.977569 pyrosimple-2.9.0/src/pyrosimple/job/move_torrent.py
+-rw-r--r--   0        0        0     4192 2023-04-29 17:58:28.391573 pyrosimple-2.9.0/src/pyrosimple/job/queue.py
+-rw-r--r--   0        0        0     9954 2023-04-13 23:29:54.100762 pyrosimple-2.9.0/src/pyrosimple/job/watch.py
+-rw-r--r--   0        0        0        0 2023-04-13 23:28:24.977569 pyrosimple-2.9.0/src/pyrosimple/py.typed
+-rw-r--r--   0        0        0      112 2023-04-13 23:28:24.977569 pyrosimple-2.9.0/src/pyrosimple/scripts/__init__.py
+-rw-r--r--   0        0        0     8094 2023-04-29 17:15:41.825951 pyrosimple-2.9.0/src/pyrosimple/scripts/base.py
+-rw-r--r--   0        0        0    17593 2023-04-13 23:38:22.673176 pyrosimple-2.9.0/src/pyrosimple/scripts/chtor.py
+-rw-r--r--   0        0        0     6590 2023-04-13 23:29:22.260813 pyrosimple-2.9.0/src/pyrosimple/scripts/lstor.py
+-rw-r--r--   0        0        0     9779 2023-06-11 16:08:49.615631 pyrosimple-2.9.0/src/pyrosimple/scripts/mktor.py
+-rw-r--r--   0        0        0    13632 2023-04-29 15:30:45.910385 pyrosimple-2.9.0/src/pyrosimple/scripts/pyroadmin.py
+-rw-r--r--   0        0        0     9555 2023-04-13 23:29:22.260813 pyrosimple-2.9.0/src/pyrosimple/scripts/pyrotorque.py
+-rw-r--r--   0        0        0    36574 2023-05-31 14:56:02.708905 pyrosimple-2.9.0/src/pyrosimple/scripts/rtcontrol.py
+-rw-r--r--   0        0        0     8199 2023-05-30 20:05:50.210723 pyrosimple-2.9.0/src/pyrosimple/scripts/rtmv_legacy.py
+-rw-r--r--   0        0        0    10373 2023-05-20 14:17:01.248156 pyrosimple-2.9.0/src/pyrosimple/scripts/rtxmlrpc.py
+-rw-r--r--   0        0        0      117 2023-04-13 23:28:24.980902 pyrosimple-2.9.0/src/pyrosimple/torrent/__init__.py
+-rw-r--r--   0        0        0    30483 2023-06-08 19:31:12.538264 pyrosimple-2.9.0/src/pyrosimple/torrent/engine.py
+-rw-r--r--   0        0        0    37020 2023-05-20 14:01:14.338449 pyrosimple-2.9.0/src/pyrosimple/torrent/rtorrent.py
+-rw-r--r--   0        0        0      118 2023-04-13 23:28:24.984236 pyrosimple-2.9.0/src/pyrosimple/ui/__init__.py
+-rw-r--r--   0        0        0     2903 2023-04-13 23:28:24.984236 pyrosimple-2.9.0/src/pyrosimple/ui/categories.py
+-rw-r--r--   0        0        0      122 2023-04-13 23:28:24.984236 pyrosimple-2.9.0/src/pyrosimple/util/__init__.py
+-rw-r--r--   0        0        0     2164 2023-04-19 02:04:04.304690 pyrosimple-2.9.0/src/pyrosimple/util/cache.py
+-rw-r--r--   0        0        0     7891 2023-04-13 23:28:24.984236 pyrosimple-2.9.0/src/pyrosimple/util/fmt.py
+-rw-r--r--   0        0        0      459 2023-04-13 23:28:24.984236 pyrosimple-2.9.0/src/pyrosimple/util/logutil.py
+-rw-r--r--   0        0        0    32171 2023-06-24 12:58:29.919468 pyrosimple-2.9.0/src/pyrosimple/util/matching.py
+-rw-r--r--   0        0        0    26411 2023-04-13 23:29:22.267480 pyrosimple-2.9.0/src/pyrosimple/util/metafile.py
+-rw-r--r--   0        0        0     2124 2023-05-30 20:07:35.753819 pyrosimple-2.9.0/src/pyrosimple/util/pymagic.py
+-rwxr-xr-x   0        0        0     9602 2023-05-20 14:22:27.819352 pyrosimple-2.9.0/src/pyrosimple/util/rpc.py
+-rw-r--r--   0        0        0     8584 2023-04-19 02:15:38.352321 pyrosimple-2.9.0/src/pyrosimple/util/traits.py
+-rw-r--r--   0        0        0     2187 2023-04-13 23:28:24.984236 pyrosimple-2.9.0/src/pyrosimple/util/ui.py
+-rw-r--r--   0        0        0     4287 1970-01-01 00:00:00.000000 pyrosimple-2.9.0/PKG-INFO
```

### Comparing `pyrosimple-2.8.0/README.md` & `pyrosimple-2.9.0/README.md`

 * *Files identical despite different names*

### Comparing `pyrosimple-2.8.0/pyproject.toml` & `pyrosimple-2.9.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyrosimple"
-version = "2.8.0"
+version = "2.9.0"
 description = "A stripped-down version of the pyrocore tools for working with rTorrent"
 authors = ["kannibalox <kannibalox@gmail.com>"]
 repository = "https://github.com/kannibalox/pyrosimple"
 documentation = "https://kannibalox.github.io/pyrosimple/"
 readme = "README.md"
 license = "GPL-3.0-or-later"
 classifiers = [
```

### Comparing `pyrosimple-2.8.0/src/pyrosimple/__init__.py` & `pyrosimple-2.9.0/src/pyrosimple/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrosimple-2.8.0/src/pyrosimple/config.py` & `pyrosimple-2.9.0/src/pyrosimple/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -145,40 +145,44 @@
 
     settings["SCGI_URL"] = scgi_url
 
     return str(settings.SCGI_URL)
 
 
 def lookup_announce_alias(name: str):
-    """Get canonical alias name and announce URL list for the given alias."""
+    """Get canonical alias name and announce URL list for the given
+    alias."""
     for alias, urls in settings["ALIASES"].items():
         if alias.lower() == name.lower():
             return alias, urls
 
     raise KeyError(f"Unknown alias {name}")
 
 
 def lookup_announce_url(name: str):
-    """Get canonical alias name and announce URL list for the given alias.
+    """Get canonical alias name and announce URL list for the given
+    alias.
 
-    Unlike lookup_announce_alias, only valid URLs are returned"""
+    Unlike lookup_announce_alias, only valid URLs are returned
+    """
     for alias, urls in settings["ALIASES"].items():
         if alias.lower() == name.lower():
             result = []
             for url in urls:
                 if urllib.parse.urlparse(url).scheme:
                     result.append(url)
             return alias, result
 
     raise KeyError(f"Unknown alias {name}")
 
 
 @functools.lru_cache(maxsize=None)
 def map_announce2alias(url: str) -> str:
-    """Get tracker alias for announce URL, and if none is defined, the 2nd level domain."""
+    """Get tracker alias for announce URL, and if none is defined, the
+    2nd level domain."""
     if url in settings["ALIASES"].items():
         return url
     # Try to find an exact alias URL match and return its label
     for alias, urls in settings["ALIASES"].items():
         if any(i == url for i in urls):
             return str(alias)
 
@@ -203,15 +207,16 @@
     except IndexError:
         return parts.netloc
 
 
 def load_custom_py():
     """Load custom python configuration.
 
-    This only gets called when CLI tools are called to prevent some weird code injection
+    This only gets called manually to prevent some weird code
+    injection if pyrosimple is ever used in a library.
     """
     log = logging.getLogger(__name__)
     if not settings.CONFIG_PY:
         log.debug("Custom code loading is disabled")
     if settings.CONFIG_PY_LOADED:
         log.debug("Custom code has already been loaded")
     config_file = Path(settings.CONFIG_PY).expanduser()
@@ -222,24 +227,26 @@
             exec(handle.read())
         settings.CONFIG_PY_LOADED = True
     else:
         log.debug("Configuration file '%s' not found.", config_file)
 
 
 def lookup_connection_alias(url: str) -> str:
-    """Convert a connection alias to the actual URL (if set in the config"""
+    """Convert a connection alias to the actual URL (if set in the
+    config"""
     if url in settings["CONNECTIONS"]:
         return str(settings["CONNECTIONS"][url])
     return url
 
 
 def multi_connection_lookup(url: str) -> Iterator[str]:
     """Return a list of urls.
 
-    This is separate from lookup_connection_alias due to scripts needing to be written specifically
-    to handle this"""
+    This is separate from lookup_connection_alias due to scripts
+    needing to be written specifically to handle this.
+    """
     val = settings["CONNECTIONS"].get(url, [url])
     if isinstance(val, list):
         for v in val:
             yield lookup_connection_alias(v)
     else:
         yield lookup_connection_alias(val)
```

### Comparing `pyrosimple-2.8.0/src/pyrosimple/data/full-example.rc` & `pyrosimple-2.9.0/src/pyrosimple/data/full-example.rc`

 * *Files identical despite different names*

### Comparing `pyrosimple-2.8.0/src/pyrosimple/error.py` & `pyrosimple-2.9.0/src/pyrosimple/error.py`

 * *Files identical despite different names*

### Comparing `pyrosimple-2.8.0/src/pyrosimple/io/scgi.py` & `pyrosimple-2.9.0/src/pyrosimple/io/scgi.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Handles RPC methods over various transports"""
 import io
 import logging
+import os
 import socket
 import subprocess
 import sys
 
 from typing import Dict, List, Optional, Tuple, Type
 from urllib import parse as urlparse
 from urllib.error import URLError
@@ -37,15 +38,15 @@
     """Base class for handling transports. Primarily exists to allow
     using the different transports with different underlying RPC mechanisms"""
 
     def __init__(self, *args, url, codec=xmlrpclib, headers=(), **kwargs):
         if "/" not in url and ":" in url and url.rsplit(":")[-1].isdigit():
             url = "scgi://" + url
         if url.startswith("/") or url.startswith("~"):
-            url = "scgi+unix://" + url
+            url = "scgi+unix://" + os.path.expanduser(url)
         self.url = url
         self.codec = codec
         self.verbose = False
         # We need to handle the headers differently based on the RPC protocols
         self._headers = list(headers)
         # Pass them to the transport in py 3.8+ only
         if sys.version_info.minor >= 8:
@@ -160,15 +161,15 @@
 
 
 def transport_from_url(url: str) -> Type[xmlrpclib.Transport]:
     """Create a transport for the given URL."""
     if "/" not in url and ":" in url and url.rsplit(":")[-1].isdigit():
         url = "scgi://" + url
     if url.startswith("/") or url.startswith("~"):
-        url = "scgi+unix://" + url
+        url = "scgi+unix://" + os.path.expanduser(url)
     parsed_url = urlparse.urlsplit(url, allow_fragments=False)
     try:
         transport = TRANSPORTS[parsed_url.scheme.lower()]
         return transport
     except KeyError:
         # Support simplified "domain:port" URLs
         if not any((parsed_url.netloc, parsed_url.query)) and parsed_url.path.isdigit():
```

### Comparing `pyrosimple-2.8.0/src/pyrosimple/job/action.py` & `pyrosimple-2.9.0/src/pyrosimple/job/action.py`

 * *Files identical despite different names*

### Comparing `pyrosimple-2.8.0/src/pyrosimple/job/base.py` & `pyrosimple-2.9.0/src/pyrosimple/job/base.py`

 * *Files identical despite different names*

### Comparing `pyrosimple-2.8.0/src/pyrosimple/job/metrics.py` & `pyrosimple-2.9.0/src/pyrosimple/job/metrics.py`

 * *Files identical despite different names*

### Comparing `pyrosimple-2.8.0/src/pyrosimple/job/move_path.py` & `pyrosimple-2.9.0/src/pyrosimple/job/move_path.py`

 * *Files identical despite different names*

### Comparing `pyrosimple-2.8.0/src/pyrosimple/job/move_torrent.py` & `pyrosimple-2.9.0/src/pyrosimple/job/move_torrent.py`

 * *Files identical despite different names*

### Comparing `pyrosimple-2.8.0/src/pyrosimple/job/queue.py` & `pyrosimple-2.9.0/src/pyrosimple/job/queue.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,15 +66,15 @@
             )
             if down_traffic > int(self.config["downloading_traffic_max"]):
                 self.log.debug(
                     "Skipping start due to max download traffic '%s' reached",
                     self.config["downloading_traffic_max"],
                 )
                 return
-        self.allowed_start_count: int = max(
+        self.allowed_start_count = max(
             self.config["start_at_once"],
             self.config["downloading_min"] - len(downloading),
         )
         if self.allowed_start_count <= 0:
             self.log.debug("Skipping start due to allowed start count reached")
         if self.downloading_count >= self.config["downloading_max"]:
             self.log.debug(
```

### Comparing `pyrosimple-2.8.0/src/pyrosimple/job/watch.py` & `pyrosimple-2.9.0/src/pyrosimple/job/watch.py`

 * *Files identical despite different names*

### Comparing `pyrosimple-2.8.0/src/pyrosimple/scripts/base.py` & `pyrosimple-2.9.0/src/pyrosimple/scripts/base.py`

 * *Files identical despite different names*

### Comparing `pyrosimple-2.8.0/src/pyrosimple/scripts/chtor.py` & `pyrosimple-2.9.0/src/pyrosimple/scripts/chtor.py`

 * *Files identical despite different names*

### Comparing `pyrosimple-2.8.0/src/pyrosimple/scripts/lstor.py` & `pyrosimple-2.9.0/src/pyrosimple/scripts/lstor.py`

 * *Files identical despite different names*

### Comparing `pyrosimple-2.8.0/src/pyrosimple/scripts/mktor.py` & `pyrosimple-2.9.0/src/pyrosimple/scripts/mktor.py`

 * *Files 2% similar despite different names*

```diff
@@ -132,15 +132,15 @@
         )
 
         if not self.options.magnet_watch:
             self.fatal("You MUST set the '--magnet-watch' config option!")
         meta_path = os.path.join(
             self.options.magnet_watch, f"magnet-{meta_name}.torrent"
         )
-        self.log.debug("Writing magnet-url metafile %r...", meta_path)
+        self.log.debug("Writing magnet-url metafile %r", meta_path)
 
         try:
             bencode.bwrite(meta_path, meta)
         except OSError as exc:
             self.fatal("Error writing magnet-url metafile %r (%s)", (meta_path, exc))
             raise
 
@@ -186,19 +186,20 @@
 
         # Create and configure metafile factory
         datapath = Path(self.args[0])
         metapath = Path(datapath)
         if self.options.output_filename:
             metapath = Path(self.options.output_filename)
             if metapath.is_dir():
-                metapath = metapath.joinpath(os.path.basename(datapath)).with_suffix(
-                    ".torrent"
-                )
+                metapath = metapath.joinpath(datapath.name).with_suffix(".torrent")
         else:
-            metapath = datapath.with_suffix(".torrent")
+            if metapath.is_dir():
+                metapath = Path(str(datapath) + ".torrent")
+            else:
+                metapath = datapath.with_suffix(".torrent")
 
         # Build progress bar
         # pylint: disable=import-outside-toplevel
         from pyrosimple.util.ui import HashProgressBar
 
         with HashProgressBar() as pb:
             if (
@@ -243,29 +244,29 @@
             torrent["info"]["x_cross_seed"] = hashlib.md5(announce.encode()).hexdigest()
             torrent.assign_fields(self.options.set)
             if len(self.args) == 2:
                 # If only one announce, just save to file
                 save_metapath = metapath
             else:
                 save_metapath = Path(f"{alias}_{metapath}")
-            self.log.info("Writing metafile %s...", save_metapath)
+            self.log.info("Writing metafile %s", save_metapath)
             torrent.save(save_metapath)
 
             # Create second metafile with fast-resume?
             if self.options.hashed:
                 try:
                     torrent.add_fast_resume(datapath)
                 except OSError as exc:
                     self.fatal(f"Error making fast-resume data ({exc})")
                     raise
 
                 hashed_path = Path(
                     re.sub(r"\.torrent$", "", str(save_metapath)) + "-resume.torrent"
                 )
-                self.log.info("Writing fast-resume metafile %s...", hashed_path)
+                self.log.info("Writing fast-resume metafile %s", hashed_path)
                 try:
                     torrent.save(hashed_path)
                 except OSError as exc:
                     self.fatal(
                         f"Error writing fast-resume metafile {hashed_path!r} ({exc})"
                     )
                     raise
```

### Comparing `pyrosimple-2.8.0/src/pyrosimple/scripts/pyroadmin.py` & `pyrosimple-2.9.0/src/pyrosimple/scripts/pyroadmin.py`

 * *Files identical despite different names*

### Comparing `pyrosimple-2.8.0/src/pyrosimple/scripts/pyrotorque.py` & `pyrosimple-2.9.0/src/pyrosimple/scripts/pyrotorque.py`

 * *Files identical despite different names*

### Comparing `pyrosimple-2.8.0/src/pyrosimple/scripts/rtcontrol.py` & `pyrosimple-2.9.0/src/pyrosimple/scripts/rtcontrol.py`

 * *Files 3% similar despite different names*

```diff
@@ -250,14 +250,18 @@
         #           like "tracker_dated = ~/done//$(alias)s/$(completed).7s",
         #           will move to ~/done/OBT/2010-08 for example
         #        self.add_value_option("--move", "TARGET",
         #            help="move data to given target directory (implies -i, can be combined with --delete)")
         # TODO: --copy, and --move/--link across devices
     )
 
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.engines = {}
+
     def add_options(self):
         """Add program options."""
         super().add_options()
 
         # basic options
         self.parser.add_argument(
             "filter",
@@ -630,14 +634,46 @@
         if self.options.sort_fields is None:
             self.options.sort_fields = config.settings.SORT_FIELDS
         if self.options.sort_fields == "*":
             self.options.sort_fields = ",".join(self.get_output_fields())
 
         return rtorrent.validate_sort_fields(self.options.sort_fields)
 
+    def open(self):
+        """Open connections and return engines."""
+        # pylint: disable=import-outside-toplevel
+        from pyrosimple import config
+        from pyrosimple.torrent import rtorrent
+
+        # pylint: enable=import-outside-toplevel
+
+        if not self.engines:
+            if not config.settings["SCGI_URL"]:
+                config.autoload_scgi_url()
+            if not config.settings["SCGI_URL"]:
+                self.log.error(
+                    "Unable to automatically detect a RPC connection, see"
+                    " https://kannibalox.github.io/pyrosimple/configuration/#reference"
+                )
+            for url in config.multi_connection_lookup(
+                self.options.url or config.settings["SCGI_URL"]
+            ):
+                try:
+                    self.engines[url] = rtorrent.RtorrentEngine(url, auto_open=True)
+                except rpc.ERRORS as e:
+                    raise error.EngineError(
+                        f"Could not load engine from url {url!r}: {e}"
+                    ) from e
+            if not self.engines:
+                raise error.ConfigurationError(
+                    "Received an empty engine list, check the settings in config.toml"
+                )
+
+        return self.engines
+
     def show_in_view(self, sourceview, matches, targetname=None):
         """Show search result in ncurses view."""
         append = self.options.alter_view == "append"
         remove = self.options.alter_view == "remove"
         action_name = (
             ", appending to" if append else ", removing from" if remove else " into"
         )
@@ -732,24 +768,21 @@
                 stdin=sys.stdin,
                 stdout=sys.stdout,
                 stderr=sys.stderr,
             )
             dcontext.open()
 
         # Find matching torrents
-        engines = {}
-        for url in config.multi_connection_lookup(
-            self.options.url or config.settings["SCGI_URL"]
-        ):
-            engines[url] = rtorrent.RtorrentEngine(url, auto_open=True)
+        self.engines = {}
+        self.open()
 
         # Kick off the result fetcher in a thread pool
-        pool = ThreadPool(processes=len(engines))
+        pool = ThreadPool(processes=len(self.engines))
         futures = {}
-        for url, r_engine in engines.items():
+        for url, r_engine in self.engines.items():
 
             def fetch(e):
                 # pylint: disable=import-outside-toplevel
                 from pyrosimple.torrent import engine
 
                 view = e.view(self.options.from_view, matcher)
                 prefetch = [
@@ -765,15 +798,15 @@
                 matches = list(e.items(view=view, prefetch=prefetch))
                 matches.sort(key=sort_key, reverse=self.options.reverse_sort)
                 return matches
 
             futures[url] = pool.apply_async(fetch, (r_engine,))
 
         # The rest of the pipeline should still be done in sequence
-        for url, r_engine in engines.items():
+        for url, r_engine in self.engines.items():
             view = r_engine.view(self.options.from_view, matcher)
             matches = futures[url].get()
 
             if selection:
                 matches = matches[selection[0] - 1 : selection[1]]
 
             if not matches:
```

### Comparing `pyrosimple-2.8.0/src/pyrosimple/scripts/rtxmlrpc.py` & `pyrosimple-2.9.0/src/pyrosimple/scripts/rtxmlrpc.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,27 +81,28 @@
         )
         self.add_bool_option(
             "--repl",
             help="Open an interactive prompt to run commands",
         )
 
     def open(self):
-        """Open connection and return proxy."""
+        """Open connections and return proxies."""
         if not self.proxies:
             if not config.settings["SCGI_URL"]:
                 config.autoload_scgi_url()
             if not config.settings["SCGI_URL"]:
                 self.log.error(
-                    "You need to configure a RPC connection, read"
-                    " https://pyrosimple.readthedocs.io/en/latest/setup.html"
+                    "Unable to automatically detect a RPC connection, see"
+                    " https://kannibalox.github.io/pyrosimple/configuration/#reference"
                 )
             for url in config.multi_connection_lookup(
                 self.options.url or config.settings["SCGI_URL"]
             ):
-                self.proxies.append(rpc.RTorrentProxy(url))
+                if url:
+                    self.proxies.append(rpc.RTorrentProxy(url))
         return self.proxies
 
     def cooked(self, raw_args):
         """Return interpreted / typed list of args."""
         args = []
         for arg in raw_args:
             if arg and arg[0] in "+-":
@@ -125,17 +126,18 @@
 
     def execute(self, proxy, method, args):
         """Execute given RPC call."""
         try:
             result = getattr(proxy, method)(*tuple(args))
         except rpc.ERRORS as exc:
             self.log.error(
-                "While calling %s(%s): %s",
+                "While calling %s(%s) via %s: %s",
                 method,
                 ", ".join(repr(i) for i in args),
+                proxy,
                 exc,
             )
             if f"Method '{method}' not defined" in str(
                 exc
             ) or f"method not found: {method}" in str(exc):
                 cmds = difflib.get_close_matches(
                     method, proxy.system.listMethods() + ["system.listMethods"]
```

### Comparing `pyrosimple-2.8.0/src/pyrosimple/torrent/engine.py` & `pyrosimple-2.9.0/src/pyrosimple/torrent/engine.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """ Torrent Engine Interface.
 
     Copyright (c) 2009, 2010, 2011 The PyroScope Project <pyroscope.project@gmail.com>
 """
 
+import json
 import logging
 import os
 import re
 import time
 import warnings
 
 from typing import Callable, Dict, Optional, Set, cast
@@ -863,14 +864,15 @@
         return DynamicField(
             list,
             name,
             f"Dynamic rpc call for {prefix}.multicall={call_name}",
             accessor=lambda o: [
                 i[0] for i in o.rpc_call(f"{prefix}.multicall", ["", call_name])
             ],
+            formatter=json.dumps,
             matcher=matching.PatternFilter,
             requires=[f"{prefix}.multicall=,{call_name}"],
         )
 
     return generate_call
```

### Comparing `pyrosimple-2.8.0/src/pyrosimple/torrent/rtorrent.py` & `pyrosimple-2.9.0/src/pyrosimple/torrent/rtorrent.py`

 * *Files 1% similar despite different names*

```diff
@@ -492,15 +492,15 @@
         remote_proxy.d.hash(self.hash)
 
         # Keep custom values. Trying to load these in during the
         # load.raw tends to cause either the load to fail or the
         # values to get corrupted, even for simple values.
         for k, v in self.custom_items().items():
             remote_proxy.d.custom.set(self.hash, k, v)
-        for key in range(1, 5):
+        for key in range(1, 6):
             value = getattr(proxy.d, f"custom{key}")(self.hash)
             if value:
                 getattr(remote_proxy.d, f"custom{key}.set")(self.hash, value)
 
         remote_proxy.d.start(self.hash)
         if not copy:
             proxy.d.erase(self.hash)
@@ -629,16 +629,16 @@
         if url is None:
             config.autoload_scgi_url()
             self.url = config.settings.SCGI_URL
         else:
             self.url = url
         if not self.url:
             raise error.UserError(
-                "You need to configure a RPC connection, read"
-                " https://kannibalox.github.io/pyrosimple/configuration/#top-level-section"
+                "Unable to automatically detect a RPC connection, see"
+                " https://kannibalox.github.io/pyrosimple/configuration/#reference"
             )
         self.rpc = rpc.RTorrentProxy(self.url)
         if auto_open:
             self.open()
 
     def view(self, viewname="default", matcher=None):
         """Get list of download items."""
```

### Comparing `pyrosimple-2.8.0/src/pyrosimple/ui/categories.py` & `pyrosimple-2.9.0/src/pyrosimple/ui/categories.py`

 * *Files identical despite different names*

### Comparing `pyrosimple-2.8.0/src/pyrosimple/util/cache.py` & `pyrosimple-2.9.0/src/pyrosimple/util/cache.py`

 * *Files identical despite different names*

### Comparing `pyrosimple-2.8.0/src/pyrosimple/util/fmt.py` & `pyrosimple-2.9.0/src/pyrosimple/util/fmt.py`

 * *Files identical despite different names*

### Comparing `pyrosimple-2.8.0/src/pyrosimple/util/matching.py` & `pyrosimple-2.9.0/src/pyrosimple/util/matching.py`

 * *Files 2% similar despite different names*

```diff
@@ -187,18 +187,18 @@
     """This node performs a logical OR for all of it's children."""
 
     def match(self, item) -> bool:
         return any(c.match(item) for c in self.children)
 
     def pre_filter(self) -> str:
         """Return rTorrent condition to speed up data transfer."""
-        if int(config.settings.get("FAST_QUERY")) == 1:
-            return ""
         if len(self.children) == 1:
             return str(self.children[0].pre_filter())
+        if int(config.settings.get("FAST_QUERY")) == 1:
+            return ""
         result = [x.pre_filter() for x in self.children]
         result = [x for x in result if x]
         if result:
             return f'or={",".join(result)}'
         return ""
 
     def __repr__(self):
@@ -293,15 +293,15 @@
 
 
 class PatternFilter(FieldFilter):
     """Pattern filter, either a glob or a /regex/ pattern."""
 
     CLEAN_PRE_VAL_RE = re.compile(r"(?:\[.*?\])|(?:\(.*?\))|(?:{.*?})|(?:\\)")
     SPLIT_PRE_VAL_RE = re.compile(r"[^a-zA-Z0-9/_]+")
-    SPLIT_PRE_GLOB_RE = re.compile(r"[?*]+")
+    SPLIT_PRE_GLOB_RE = re.compile(r"[?*[\]]+")
 
     def validate(self) -> None:
         """Validate filter condition (template method)."""
 
         super().validate()
         self._value: str = self._value
         self._template = None
@@ -315,14 +315,15 @@
             self._value.endswith("/") or self._value.endswith("/i")
         ):
             # Pick out a couple regexes that can be simplified
             if self._value in ["//", "/.*/", "//i", "/.*/i"]:
                 self._matcher = lambda _, __: True
             elif self._value in ["/.+/", "/.+/i"]:
                 self._matcher = lambda val, __: bool(val)
+            # Otherwise handle it generically
             else:
                 value = self._value
                 if self._value.endswith("/i"):
                     self._flags = re.IGNORECASE
                     value = self._value.rstrip("i")
                 regex = re.compile(value[1:-1], self._flags)
                 self._matcher = lambda val, _: bool(regex.search(val))
@@ -340,15 +341,18 @@
 
             self._matcher = _template_globber
         else:
             # Pick out a glob that can be simplified
             if self._value == "*":
                 self._matcher = lambda _, __: True
             else:
-                self._matcher = lambda val, _: fnmatch.fnmatchcase(val, self._value)
+                self._matcher = (
+                    lambda val, _: fnmatch.fnmatchcase(val, self._value)
+                    or val == self._value
+                )
 
     def pre_filter_eq(self) -> str:
         """Return rTorrent condition to speed up data transfer."""
         pf = prefilter_field_lookup(self._name)
         if pf is None or self._template:
             return ""
         if not self._value or self._value == '""':
@@ -547,15 +551,14 @@
         "m": lambda d: d * 60,
         "s": lambda d: d,
     }
     TIMEDELTA_RE = re.compile(
         "^" + "".join(r"(?:(?P<{0}>\d+)[{0}{0}])?".format(i) for i in "yMwdhms") + "$"
     )
 
-    # pylint: disable=super-init-not-called
     def __init__(self, name: str, op: FilterOperator, value: str):
         # During validate(), one of these two must be set to something
         # non-None
         self._timestamp_offset = None
         self._timestamp = None
         super().__init__(name, op, value)
 
@@ -785,15 +788,15 @@
         self._value = self._value * scale
 
 
 QueryGrammar = Grammar(
     r"""
     query = (group / stmt) (ws (group / stmt))*
     stmt = (or_stmt / conds)
-    or_stmt = (group / conds) ws or ws (group / conds)
+    or_stmt = (group / conds) (ws or ws (group / conds))*
     group = (not ws)? lpar ws stmt ws rpar
     conds = cond (ws cond)*
     cond = (&or / &lpar / &rpar / &not / named_cond / unnamed_cond)
     named_cond = word conditional filter
     unnamed_cond = filter
     filter      = (quoted_regex / quoted / glob / regex / word)
     glob = ~r"[\S]+"
@@ -879,15 +882,22 @@
         if len(real_children) == 0:
             return None
         if len(real_children) == 1:
             return real_children[0]
         return class_(real_children)
 
     def visit_or_stmt(self, node, visited_children):
-        return OrNode([c for c in visited_children if c is not None])
+        children = [visited_children[0]]
+        if visited_children[1] is not None:
+            if isinstance(visited_children[1], list):
+                for c in visited_children[1]:
+                    children.append(c)
+            else:
+                children.append(visited_children[1])
+        return OrNode(children)
 
     def visit_conds(self, node, visited_children):
         if len(visited_children) == 2 and isinstance(visited_children[1], list):
             children = [visited_children[0]] + visited_children[1]
         else:
             children = visited_children
         pared = self.__pare_children(children, AndNode)
```

### Comparing `pyrosimple-2.8.0/src/pyrosimple/util/metafile.py` & `pyrosimple-2.9.0/src/pyrosimple/util/metafile.py`

 * *Files identical despite different names*

### Comparing `pyrosimple-2.8.0/src/pyrosimple/util/pymagic.py` & `pyrosimple-2.9.0/src/pyrosimple/util/pymagic.py`

 * *Files 7% similar despite different names*

```diff
@@ -46,14 +46,16 @@
         result = getattr(result, attr)
 
     return result
 
 
 def get_class_logger(obj):
     """Get a logger specific for the given object's class."""
+    if obj.__class__.__module__ == "__main__":
+        return logging.getLogger("pyrosimple.main." + obj.__class__.__name__)
     return logging.getLogger(obj.__class__.__module__ + "." + obj.__class__.__name__)
 
 
 class JSONEncoder(json.JSONEncoder):
     """Custom JSON encoder."""
 
     def default(self, o):
```

### Comparing `pyrosimple-2.8.0/src/pyrosimple/util/rpc.py` & `pyrosimple-2.9.0/src/pyrosimple/util/rpc.py`

 * *Files 1% similar despite different names*

```diff
@@ -203,19 +203,21 @@
                 }
             )
             .encode(self.__encoding, "xmlcharrefreplace")
         )
         if self.__verbose:
             logger.info("req: %s", request)
 
-        response: Dict = self.__transport.request(
-            self.__host,
-            self.__handler,
-            request,
-            verbose=self.__verbose,
+        response: Dict = dict(
+            self.__transport.request(
+                self.__host,
+                self.__handler,
+                request,
+                verbose=self.__verbose,
+            )
         )
 
         if response["id"] != rpc_id:
             raise ValueError(
                 f"RPC IDs do not match: sent={rpc_id} received={response['id']}"
             )
         if "error" in response:
```

### Comparing `pyrosimple-2.8.0/src/pyrosimple/util/traits.py` & `pyrosimple-2.9.0/src/pyrosimple/util/traits.py`

 * *Files identical despite different names*

### Comparing `pyrosimple-2.8.0/src/pyrosimple/util/ui.py` & `pyrosimple-2.9.0/src/pyrosimple/util/ui.py`

 * *Files identical despite different names*

### Comparing `pyrosimple-2.8.0/PKG-INFO` & `pyrosimple-2.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrosimple
-Version: 2.8.0
+Version: 2.9.0
 Summary: A stripped-down version of the pyrocore tools for working with rTorrent
 Home-page: https://github.com/kannibalox/pyrosimple
 License: GPL-3.0-or-later
 Author: kannibalox
 Author-email: kannibalox@gmail.com
 Requires-Python: >=3.7.2,<4
 Classifier: Development Status :: 4 - Beta
```

