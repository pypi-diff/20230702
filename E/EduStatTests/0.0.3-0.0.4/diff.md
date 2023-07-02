# Comparing `tmp/EduStatTests-0.0.3.tar.gz` & `tmp/EduStatTests-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EduStatTests-0.0.3.tar", last modified: Sun Jul  2 12:43:23 2023, max compression
+gzip compressed data, was "EduStatTests-0.0.4.tar", last modified: Sun Jul  2 13:21:22 2023, max compression
```

## Comparing `EduStatTests-0.0.3.tar` & `EduStatTests-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 hakan     (1000) hakan     (1000)        0 2023-07-02 12:43:23.991051 EduStatTests-0.0.3/
--rw-rw-r--   0 hakan     (1000) hakan     (1000)     1070 2023-07-02 11:36:16.000000 EduStatTests-0.0.3/LICENSE
--rw-rw-r--   0 hakan     (1000) hakan     (1000)      551 2023-07-02 12:43:23.991051 EduStatTests-0.0.3/PKG-INFO
--rw-rw-r--   0 hakan     (1000) hakan     (1000)       79 2023-07-02 11:36:16.000000 EduStatTests-0.0.3/README.md
--rw-rw-r--   0 hakan     (1000) hakan     (1000)      587 2023-07-02 12:42:15.000000 EduStatTests-0.0.3/pyproject.toml
--rw-rw-r--   0 hakan     (1000) hakan     (1000)       38 2023-07-02 12:43:23.991051 EduStatTests-0.0.3/setup.cfg
-drwxrwxr-x   0 hakan     (1000) hakan     (1000)        0 2023-07-02 12:43:23.987051 EduStatTests-0.0.3/src/
-drwxrwxr-x   0 hakan     (1000) hakan     (1000)        0 2023-07-02 12:43:23.991051 EduStatTests-0.0.3/src/EduStatTests.egg-info/
--rw-rw-r--   0 hakan     (1000) hakan     (1000)      551 2023-07-02 12:43:23.000000 EduStatTests-0.0.3/src/EduStatTests.egg-info/PKG-INFO
--rw-rw-r--   0 hakan     (1000) hakan     (1000)      225 2023-07-02 12:43:23.000000 EduStatTests-0.0.3/src/EduStatTests.egg-info/SOURCES.txt
--rw-rw-r--   0 hakan     (1000) hakan     (1000)        1 2023-07-02 12:43:23.000000 EduStatTests-0.0.3/src/EduStatTests.egg-info/dependency_links.txt
--rw-rw-r--   0 hakan     (1000) hakan     (1000)       19 2023-07-02 12:43:23.000000 EduStatTests-0.0.3/src/EduStatTests.egg-info/top_level.txt
--rw-rw-r--   0 hakan     (1000) hakan     (1000)     1227 2023-07-02 11:52:58.000000 EduStatTests-0.0.3/src/StatTests.py
--rw-rw-r--   0 hakan     (1000) hakan     (1000)        0 2023-07-02 11:47:24.000000 EduStatTests-0.0.3/src/__init__.py
+drwxrwxr-x   0 hakan     (1000) hakan     (1000)        0 2023-07-02 13:21:22.591949 EduStatTests-0.0.4/
+-rw-rw-r--   0 hakan     (1000) hakan     (1000)     1070 2023-07-02 11:36:16.000000 EduStatTests-0.0.4/LICENSE
+-rw-rw-r--   0 hakan     (1000) hakan     (1000)      551 2023-07-02 13:21:22.587949 EduStatTests-0.0.4/PKG-INFO
+-rw-rw-r--   0 hakan     (1000) hakan     (1000)       79 2023-07-02 11:36:16.000000 EduStatTests-0.0.4/README.md
+-rw-rw-r--   0 hakan     (1000) hakan     (1000)      587 2023-07-02 13:21:09.000000 EduStatTests-0.0.4/pyproject.toml
+-rw-rw-r--   0 hakan     (1000) hakan     (1000)       38 2023-07-02 13:21:22.591949 EduStatTests-0.0.4/setup.cfg
+drwxrwxr-x   0 hakan     (1000) hakan     (1000)        0 2023-07-02 13:21:22.587949 EduStatTests-0.0.4/src/
+drwxrwxr-x   0 hakan     (1000) hakan     (1000)        0 2023-07-02 13:21:22.587949 EduStatTests-0.0.4/src/EduStatTests.egg-info/
+-rw-rw-r--   0 hakan     (1000) hakan     (1000)      551 2023-07-02 13:21:22.000000 EduStatTests-0.0.4/src/EduStatTests.egg-info/PKG-INFO
+-rw-rw-r--   0 hakan     (1000) hakan     (1000)      228 2023-07-02 13:21:22.000000 EduStatTests-0.0.4/src/EduStatTests.egg-info/SOURCES.txt
+-rw-rw-r--   0 hakan     (1000) hakan     (1000)        1 2023-07-02 13:21:22.000000 EduStatTests-0.0.4/src/EduStatTests.egg-info/dependency_links.txt
+-rw-rw-r--   0 hakan     (1000) hakan     (1000)       22 2023-07-02 13:21:22.000000 EduStatTests-0.0.4/src/EduStatTests.egg-info/top_level.txt
+-rw-rw-r--   0 hakan     (1000) hakan     (1000)     1227 2023-07-02 13:19:19.000000 EduStatTests-0.0.4/src/EduStatTests.py
+-rw-rw-r--   0 hakan     (1000) hakan     (1000)        0 2023-07-02 11:47:24.000000 EduStatTests-0.0.4/src/__init__.py
```

### Comparing `EduStatTests-0.0.3/LICENSE` & `EduStatTests-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `EduStatTests-0.0.3/PKG-INFO` & `EduStatTests-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EduStatTests
-Version: 0.0.3
+Version: 0.0.4
 Author-email: Hakan Güldal <hguldal@gmail.com>
 Project-URL: Homepage, https://github.com/hguldal/EduStatTests
 Project-URL: Bug Tracker, https://github.com/hguldal/EduStatTests/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `EduStatTests-0.0.3/pyproject.toml` & `EduStatTests-0.0.4/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0","numpy; python_version>='3.12'"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "EduStatTests"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Hakan Güldal", email="hguldal@gmail.com" },
 ]
 description = ""
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `EduStatTests-0.0.3/src/EduStatTests.egg-info/PKG-INFO` & `EduStatTests-0.0.4/src/EduStatTests.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EduStatTests
-Version: 0.0.3
+Version: 0.0.4
 Author-email: Hakan Güldal <hguldal@gmail.com>
 Project-URL: Homepage, https://github.com/hguldal/EduStatTests
 Project-URL: Bug Tracker, https://github.com/hguldal/EduStatTests/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `EduStatTests-0.0.3/src/StatTests.py` & `EduStatTests-0.0.4/src/EduStatTests.py`

 * *Files identical despite different names*

