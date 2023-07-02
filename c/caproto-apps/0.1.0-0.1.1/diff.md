# Comparing `tmp/caproto-apps-0.1.0.tar.gz` & `tmp/caproto-apps-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caproto-apps-0.1.0.tar", last modified: Sun Jul  2 02:20:47 2023, max compression
+gzip compressed data, was "caproto-apps-0.1.1.tar", last modified: Sun Jul  2 02:25:51 2023, max compression
```

## Comparing `caproto-apps-0.1.0.tar` & `caproto-apps-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwx------   0 b268176   (2319) xsdspc    (1117)        0 2023-07-02 02:20:47.653473 caproto-apps-0.1.0/
--rw-------   0 b268176   (2319) xsdspc    (1117)     3736 2023-07-02 02:20:47.652473 caproto-apps-0.1.0/PKG-INFO
--rw-r--r--   0 b268176   (2319) xsdspc    (1117)     3177 2023-07-02 02:19:09.000000 caproto-apps-0.1.0/README.md
--rw-------   0 b268176   (2319) xsdspc    (1117)     1043 2023-07-02 02:10:14.000000 caproto-apps-0.1.0/pyproject.toml
--rw-------   0 b268176   (2319) xsdspc    (1117)       38 2023-07-02 02:20:47.653473 caproto-apps-0.1.0/setup.cfg
-drwx------   0 b268176   (2319) xsdspc    (1117)        0 2023-07-02 02:20:47.647473 caproto-apps-0.1.0/src/
-drwx------   0 b268176   (2319) xsdspc    (1117)        0 2023-07-02 02:20:47.650473 caproto-apps-0.1.0/src/caproto_apps.egg-info/
--rw-r--r--   0 b268176   (2319) xsdspc    (1117)     3736 2023-07-02 02:20:47.000000 caproto-apps-0.1.0/src/caproto_apps.egg-info/PKG-INFO
--rw-r--r--   0 b268176   (2319) xsdspc    (1117)      345 2023-07-02 02:20:47.000000 caproto-apps-0.1.0/src/caproto_apps.egg-info/SOURCES.txt
--rw-r--r--   0 b268176   (2319) xsdspc    (1117)        1 2023-07-02 02:20:47.000000 caproto-apps-0.1.0/src/caproto_apps.egg-info/dependency_links.txt
--rw-r--r--   0 b268176   (2319) xsdspc    (1117)       62 2023-07-02 02:20:47.000000 caproto-apps-0.1.0/src/caproto_apps.egg-info/requires.txt
--rw-r--r--   0 b268176   (2319) xsdspc    (1117)       12 2023-07-02 02:20:47.000000 caproto-apps-0.1.0/src/caproto_apps.egg-info/top_level.txt
-drwx------   0 b268176   (2319) xsdspc    (1117)        0 2023-07-02 02:20:47.650473 caproto-apps-0.1.0/src/caprotoapps/
--rw-------   0 b268176   (2319) xsdspc    (1117)       64 2023-07-02 02:10:14.000000 caproto-apps-0.1.0/src/caprotoapps/__init__.py
--rw-r--r--   0 b268176   (2319) xsdspc    (1117)    20766 2023-06-28 04:14:07.000000 caproto-apps-0.1.0/src/caprotoapps/alive.py
--rw-------   0 b268176   (2319) xsdspc    (1117)     8190 2023-07-02 02:10:14.000000 caproto-apps-0.1.0/src/caprotoapps/manager.py
-drwx------   0 b268176   (2319) xsdspc    (1117)        0 2023-07-02 02:20:47.651473 caproto-apps-0.1.0/tests/
--rw-r--r--   0 b268176   (2319) xsdspc    (1117)    10768 2023-07-01 02:49:25.000000 caproto-apps-0.1.0/tests/test_alive.py
--rw-------   0 b268176   (2319) xsdspc    (1117)     4002 2023-07-01 23:53:32.000000 caproto-apps-0.1.0/tests/test_manager.py
+drwx------   0 b268176   (2319) xsdspc    (1117)        0 2023-07-02 02:25:51.215747 caproto-apps-0.1.1/
+-rw-------   0 b268176   (2319) xsdspc    (1117)     3736 2023-07-02 02:25:51.215747 caproto-apps-0.1.1/PKG-INFO
+-rw-r--r--   0 b268176   (2319) xsdspc    (1117)     3177 2023-07-02 02:19:09.000000 caproto-apps-0.1.1/README.md
+-rw-------   0 b268176   (2319) xsdspc    (1117)     1043 2023-07-02 02:25:13.000000 caproto-apps-0.1.1/pyproject.toml
+-rw-------   0 b268176   (2319) xsdspc    (1117)       38 2023-07-02 02:25:51.215747 caproto-apps-0.1.1/setup.cfg
+drwx------   0 b268176   (2319) xsdspc    (1117)        0 2023-07-02 02:25:51.212747 caproto-apps-0.1.1/src/
+drwx------   0 b268176   (2319) xsdspc    (1117)        0 2023-07-02 02:25:51.213747 caproto-apps-0.1.1/src/caproto_apps.egg-info/
+-rw-r--r--   0 b268176   (2319) xsdspc    (1117)     3736 2023-07-02 02:25:51.000000 caproto-apps-0.1.1/src/caproto_apps.egg-info/PKG-INFO
+-rw-r--r--   0 b268176   (2319) xsdspc    (1117)      345 2023-07-02 02:25:51.000000 caproto-apps-0.1.1/src/caproto_apps.egg-info/SOURCES.txt
+-rw-r--r--   0 b268176   (2319) xsdspc    (1117)        1 2023-07-02 02:25:51.000000 caproto-apps-0.1.1/src/caproto_apps.egg-info/dependency_links.txt
+-rw-r--r--   0 b268176   (2319) xsdspc    (1117)       62 2023-07-02 02:25:51.000000 caproto-apps-0.1.1/src/caproto_apps.egg-info/requires.txt
+-rw-r--r--   0 b268176   (2319) xsdspc    (1117)       12 2023-07-02 02:25:51.000000 caproto-apps-0.1.1/src/caproto_apps.egg-info/top_level.txt
+drwx------   0 b268176   (2319) xsdspc    (1117)        0 2023-07-02 02:25:51.214747 caproto-apps-0.1.1/src/caprotoapps/
+-rw-------   0 b268176   (2319) xsdspc    (1117)       64 2023-07-02 02:10:14.000000 caproto-apps-0.1.1/src/caprotoapps/__init__.py
+-rw-r--r--   0 b268176   (2319) xsdspc    (1117)    20766 2023-06-28 04:14:07.000000 caproto-apps-0.1.1/src/caprotoapps/alive.py
+-rw-------   0 b268176   (2319) xsdspc    (1117)     8403 2023-07-02 02:24:39.000000 caproto-apps-0.1.1/src/caprotoapps/manager.py
+drwx------   0 b268176   (2319) xsdspc    (1117)        0 2023-07-02 02:25:51.214747 caproto-apps-0.1.1/tests/
+-rw-r--r--   0 b268176   (2319) xsdspc    (1117)    10768 2023-07-01 02:49:25.000000 caproto-apps-0.1.1/tests/test_alive.py
+-rw-------   0 b268176   (2319) xsdspc    (1117)     4002 2023-07-01 23:53:32.000000 caproto-apps-0.1.1/tests/test_manager.py
```

### Comparing `caproto-apps-0.1.0/PKG-INFO` & `caproto-apps-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caproto-apps
-Version: 0.1.0
+Version: 0.1.1
 Summary: Variety of useful extensions for caproto IOCs.
 Author-email: Mark Wolfman <wolfman@anl.gov>
 Project-URL: Homepage, https://github.com/canismarko/caproto-apps
 Keywords: caproto,controls
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `caproto-apps-0.1.0/README.md` & `caproto-apps-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `caproto-apps-0.1.0/pyproject.toml` & `caproto-apps-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 # [build-system]
 # requires = ["hatchling"]
 # build-backend = "hatchling.build"
 
 [project]
 name = "caproto-apps"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="Mark Wolfman", email="wolfman@anl.gov" },
 ]
 description = "Variety of useful extensions for caproto IOCs."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `caproto-apps-0.1.0/src/caproto_apps.egg-info/PKG-INFO` & `caproto-apps-0.1.1/src/caproto_apps.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caproto-apps
-Version: 0.1.0
+Version: 0.1.1
 Summary: Variety of useful extensions for caproto IOCs.
 Author-email: Mark Wolfman <wolfman@anl.gov>
 Project-URL: Homepage, https://github.com/canismarko/caproto-apps
 Keywords: caproto,controls
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `caproto-apps-0.1.0/src/caprotoapps/alive.py` & `caproto-apps-0.1.1/src/caprotoapps/alive.py`

 * *Files identical despite different names*

### Comparing `caproto-apps-0.1.0/src/caprotoapps/manager.py` & `caproto-apps-0.1.1/src/caprotoapps/manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -168,24 +168,30 @@
             return IOCStatus.Stopped
         else:
             return IOCStatus.Running
                 
 
 
 class BCDASSHRunner(BCDARunner):
-    ssh_connection: Connection
+    ssh_connection: Connection = None
     
     def __init__(self, user: str, host: str, script_path: Path):
-        self.ssh_connection = Connection(host=host, user=user)
+        self.user = user
+        self.host = host
         super().__init__(script_path=script_path)
 
     def execute_script(self, args):
         """Execute *args* on local machine."""
+        # Establish connection
+        if self.ssh_connection is None:
+            self.ssh_connection = Connection(host=self.host, user=self.user)
+        # Send command to the remote host
         cmd = " ".join(args)
         result = self.ssh_connection.run(cmd, hide="out")
+        # Parse the response
         response = result.stdout.strip()
         return response
 
 
 def guess_runner(script: str):
     """Determine which IOC runner to use based on the script type."""
     user, host, path = parse_script_location(script)
```

### Comparing `caproto-apps-0.1.0/tests/test_alive.py` & `caproto-apps-0.1.1/tests/test_alive.py`

 * *Files identical despite different names*

### Comparing `caproto-apps-0.1.0/tests/test_manager.py` & `caproto-apps-0.1.1/tests/test_manager.py`

 * *Files identical despite different names*

