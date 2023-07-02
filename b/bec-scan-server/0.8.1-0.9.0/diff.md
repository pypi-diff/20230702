# Comparing `tmp/bec_scan_server-0.8.1.tar.gz` & `tmp/bec_scan_server-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bec_scan_server-0.8.1.tar", last modified: Sun Jul  2 18:15:20 2023, max compression
+gzip compressed data, was "bec_scan_server-0.9.0.tar", last modified: Sun Jul  2 18:58:55 2023, max compression
```

## Comparing `bec_scan_server-0.8.1.tar` & `bec_scan_server-0.9.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 18:15:20.707840 bec_scan_server-0.8.1/
--rw-r--r--   0 root         (0) root         (0)     2560 2023-07-02 18:15:20.707840 bec_scan_server-0.8.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2115 2023-06-27 20:50:04.000000 bec_scan_server-0.8.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 18:15:20.706840 bec_scan_server-0.8.1/bec_scan_server.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2560 2023-07-02 18:15:20.000000 bec_scan_server-0.8.1/bec_scan_server.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      534 2023-07-02 18:15:20.000000 bec_scan_server-0.8.1/bec_scan_server.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-02 18:15:20.000000 bec_scan_server-0.8.1/bec_scan_server.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       77 2023-07-02 18:15:20.000000 bec_scan_server-0.8.1/bec_scan_server.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-07-02 18:15:20.000000 bec_scan_server-0.8.1/bec_scan_server.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 18:15:20.706840 bec_scan_server-0.8.1/scan_server/
--rw-rw-rw-   0 root         (0) root         (0)       26 2023-04-24 15:23:42.000000 bec_scan_server-0.8.1/scan_server/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      128 2023-04-24 15:23:42.000000 bec_scan_server-0.8.1/scan_server/errors.py
--rw-rw-rw-   0 root         (0) root         (0)     3489 2023-06-19 08:14:59.000000 bec_scan_server-0.8.1/scan_server/path_optimization.py
--rw-r--r--   0 root         (0) root         (0)     1861 2023-06-28 10:41:58.000000 bec_scan_server-0.8.1/scan_server/scan_assembler.py
--rw-r--r--   0 root         (0) root         (0)     6937 2023-06-28 10:41:58.000000 bec_scan_server-0.8.1/scan_server/scan_guard.py
--rw-r--r--   0 root         (0) root         (0)     3175 2023-06-28 10:41:58.000000 bec_scan_server-0.8.1/scan_server/scan_manager.py
--rw-r--r--   0 root         (0) root         (0)    30785 2023-06-28 10:41:58.000000 bec_scan_server-0.8.1/scan_server/scan_queue.py
--rw-r--r--   0 root         (0) root         (0)     3549 2023-06-28 10:41:58.000000 bec_scan_server-0.8.1/scan_server/scan_server.py
--rw-r--r--   0 root         (0) root         (0)    13324 2023-06-28 10:41:58.000000 bec_scan_server-0.8.1/scan_server/scan_stubs.py
--rw-r--r--   0 root         (0) root         (0)    26660 2023-06-28 15:23:35.000000 bec_scan_server-0.8.1/scan_server/scan_worker.py
--rw-r--r--   0 root         (0) root         (0)    42711 2023-06-28 10:41:58.000000 bec_scan_server-0.8.1/scan_server/scans.py
--rw-r--r--   0 root         (0) root         (0)      513 2023-07-02 18:15:20.707840 bec_scan_server-0.8.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      842 2023-06-28 14:27:03.000000 bec_scan_server-0.8.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 18:58:55.346857 bec_scan_server-0.9.0/
+-rw-r--r--   0 root         (0) root         (0)     2560 2023-07-02 18:58:55.346857 bec_scan_server-0.9.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2115 2023-06-27 20:50:04.000000 bec_scan_server-0.9.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 18:58:55.346857 bec_scan_server-0.9.0/bec_scan_server.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2560 2023-07-02 18:58:55.000000 bec_scan_server-0.9.0/bec_scan_server.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      534 2023-07-02 18:58:55.000000 bec_scan_server-0.9.0/bec_scan_server.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-02 18:58:55.000000 bec_scan_server-0.9.0/bec_scan_server.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       77 2023-07-02 18:58:55.000000 bec_scan_server-0.9.0/bec_scan_server.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-07-02 18:58:55.000000 bec_scan_server-0.9.0/bec_scan_server.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 18:58:55.345857 bec_scan_server-0.9.0/scan_server/
+-rw-rw-rw-   0 root         (0) root         (0)       26 2023-04-24 15:23:42.000000 bec_scan_server-0.9.0/scan_server/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      128 2023-04-24 15:23:42.000000 bec_scan_server-0.9.0/scan_server/errors.py
+-rw-rw-rw-   0 root         (0) root         (0)     3489 2023-06-19 08:14:59.000000 bec_scan_server-0.9.0/scan_server/path_optimization.py
+-rw-r--r--   0 root         (0) root         (0)     1861 2023-06-28 10:41:58.000000 bec_scan_server-0.9.0/scan_server/scan_assembler.py
+-rw-r--r--   0 root         (0) root         (0)     6937 2023-06-28 10:41:58.000000 bec_scan_server-0.9.0/scan_server/scan_guard.py
+-rw-r--r--   0 root         (0) root         (0)     3407 2023-07-02 18:58:28.000000 bec_scan_server-0.9.0/scan_server/scan_manager.py
+-rw-r--r--   0 root         (0) root         (0)    30785 2023-06-28 10:41:58.000000 bec_scan_server-0.9.0/scan_server/scan_queue.py
+-rw-r--r--   0 root         (0) root         (0)     3549 2023-06-28 10:41:58.000000 bec_scan_server-0.9.0/scan_server/scan_server.py
+-rw-r--r--   0 root         (0) root         (0)    13324 2023-06-28 10:41:58.000000 bec_scan_server-0.9.0/scan_server/scan_stubs.py
+-rw-r--r--   0 root         (0) root         (0)    26660 2023-06-28 15:23:35.000000 bec_scan_server-0.9.0/scan_server/scan_worker.py
+-rw-r--r--   0 root         (0) root         (0)    42711 2023-06-28 10:41:58.000000 bec_scan_server-0.9.0/scan_server/scans.py
+-rw-r--r--   0 root         (0) root         (0)      513 2023-07-02 18:58:55.347857 bec_scan_server-0.9.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      842 2023-06-28 14:27:03.000000 bec_scan_server-0.9.0/setup.py
```

### Comparing `bec_scan_server-0.8.1/PKG-INFO` & `bec_scan_server-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bec_scan_server
-Version: 0.8.1
+Version: 0.9.0
 Summary: BEC scan server
 Home-page: https://gitlab.psi.ch/bec/bec
 License: UNKNOWN
 Project-URL: Bug Tracker, https://gitlab.psi.ch/bec/bec/issues
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `bec_scan_server-0.8.1/README.md` & `bec_scan_server-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `bec_scan_server-0.8.1/bec_scan_server.egg-info/PKG-INFO` & `bec_scan_server-0.9.0/bec_scan_server.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bec-scan-server
-Version: 0.8.1
+Version: 0.9.0
 Summary: BEC scan server
 Home-page: https://gitlab.psi.ch/bec/bec
 License: UNKNOWN
 Project-URL: Bug Tracker, https://gitlab.psi.ch/bec/bec/issues
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `bec_scan_server-0.8.1/bec_scan_server.egg-info/SOURCES.txt` & `bec_scan_server-0.9.0/bec_scan_server.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bec_scan_server-0.8.1/scan_server/path_optimization.py` & `bec_scan_server-0.9.0/scan_server/path_optimization.py`

 * *Files identical despite different names*

### Comparing `bec_scan_server-0.8.1/scan_server/scan_assembler.py` & `bec_scan_server-0.9.0/scan_server/scan_assembler.py`

 * *Files identical despite different names*

### Comparing `bec_scan_server-0.8.1/scan_server/scan_guard.py` & `bec_scan_server-0.9.0/scan_server/scan_guard.py`

 * *Files identical despite different names*

### Comparing `bec_scan_server-0.8.1/scan_server/scan_manager.py` & `bec_scan_server-0.9.0/scan_server/scan_manager.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,17 +10,15 @@
 
 from . import scans as ScanServerScans
 
 logger = bec_logger.logger
 
 
 class ScanManager:
-    DEFAULT_PLUGIN_PATH = Path(
-        os.path.dirname(os.path.abspath(__file__)) + "/../scan_plugins"
-    ).resolve()
+    DEFAULT_PLUGIN_PATH = Path(os.path.dirname(os.path.abspath(__file__)) + "/../../").resolve()
 
     def __init__(self, *, parent):
         """
         Scan Manager loads and manages the available scans.
         """
         self.parent = parent
         self.available_scans = {}
@@ -28,20 +26,25 @@
         self._plugins = {}
         self.load_plugins()
         self.update_available_scans()
         self.publish_available_scans()
 
     def load_plugins(self):
         """load scan plugins"""
-        plugin_path = self.DEFAULT_PLUGIN_PATH
+        plugin_path = os.environ.get("BEC_PLUGIN_PATH")
+        if not plugin_path:
+            logger.info("BEC_PLUGIN_PATH not set. Using default plugin path.")
+            plugin_path = self.DEFAULT_PLUGIN_PATH
+        else:
+            logger.info(f"Using plugin path {plugin_path}")
+        plugin_path = os.path.join(plugin_path, "scan_server/scan_plugins")
         files = glob.glob(os.path.join(plugin_path, "*.py"))
         for file in files:
             if file.endswith("__init__.py"):
                 continue
-            filename = os.path.basename(file).split(".py")[0]
             module_spec = importlib.util.spec_from_file_location("scan_plugins", file)
             plugin_module = importlib.util.module_from_spec(module_spec)
             module_spec.loader.exec_module(plugin_module)
             module_members = inspect.getmembers(plugin_module)
             for name, cls in module_members:
                 if not inspect.isclass(cls):
                     continue
```

### Comparing `bec_scan_server-0.8.1/scan_server/scan_queue.py` & `bec_scan_server-0.9.0/scan_server/scan_queue.py`

 * *Files identical despite different names*

### Comparing `bec_scan_server-0.8.1/scan_server/scan_server.py` & `bec_scan_server-0.9.0/scan_server/scan_server.py`

 * *Files identical despite different names*

### Comparing `bec_scan_server-0.8.1/scan_server/scan_stubs.py` & `bec_scan_server-0.9.0/scan_server/scan_stubs.py`

 * *Files identical despite different names*

### Comparing `bec_scan_server-0.8.1/scan_server/scan_worker.py` & `bec_scan_server-0.9.0/scan_server/scan_worker.py`

 * *Files identical despite different names*

### Comparing `bec_scan_server-0.8.1/scan_server/scans.py` & `bec_scan_server-0.9.0/scan_server/scans.py`

 * *Files identical despite different names*

### Comparing `bec_scan_server-0.8.1/setup.cfg` & `bec_scan_server-0.9.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `bec_scan_server-0.8.1/setup.py` & `bec_scan_server-0.9.0/setup.py`

 * *Files identical despite different names*

