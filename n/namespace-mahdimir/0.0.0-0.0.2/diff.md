# Comparing `tmp/namespace_mahdimir-0.0.0.tar.gz` & `tmp/namespace_mahdimir-0.0.2.tar.gz`

## Comparing `namespace_mahdimir-0.0.0.tar` & `namespace_mahdimir-0.0.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 namespace_mahdimir-0.0.0/.gitattributes
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 namespace_mahdimir-0.0.0/src/namespace_mahdimir/__init__.py
--rw-r--r--   0        0        0     2416 2020-02-02 00:00:00.000000 namespace_mahdimir-0.0.0/src/namespace_mahdimir/tse.py
--rw-r--r--   0        0        0     3526 2020-02-02 00:00:00.000000 namespace_mahdimir-0.0.0/.gitignore
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 namespace_mahdimir-0.0.0/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 namespace_mahdimir-0.0.0/README.md
--rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 namespace_mahdimir-0.0.0/pyproject.toml
--rw-r--r--   0        0        0     2153 2020-02-02 00:00:00.000000 namespace_mahdimir-0.0.0/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 namespace_mahdimir-0.0.2/.gitattributes
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 namespace_mahdimir-0.0.2/src/namespace_mahdimir/__init__.py
+-rw-r--r--   0        0        0     2416 2020-02-02 00:00:00.000000 namespace_mahdimir-0.0.2/src/namespace_mahdimir/tse.py
+-rw-r--r--   0        0        0     3526 2020-02-02 00:00:00.000000 namespace_mahdimir-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 namespace_mahdimir-0.0.2/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 namespace_mahdimir-0.0.2/README.md
+-rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 namespace_mahdimir-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 namespace_mahdimir-0.0.2/PKG-INFO
```

### Comparing `namespace_mahdimir-0.0.0/src/namespace_mahdimir/tse.py` & `namespace_mahdimir-0.0.2/src/namespace_mahdimir/tse.py`

 * *Files identical despite different names*

### Comparing `namespace_mahdimir-0.0.0/.gitignore` & `namespace_mahdimir-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `namespace_mahdimir-0.0.0/LICENSE` & `namespace_mahdimir-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `namespace_mahdimir-0.0.0/pyproject.toml` & `namespace_mahdimir-0.0.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "namespace_mahdimir"
-version = "0.0.0"
+version = "0.0.2"
 authors = [{ name = "Mahdi Mir", email = "imahdimir@gmail.com" }]
 description = "Some Namespaces for Python"
 readme = "README.md"
 license = { file = "LICENSE" }
 dependencies = [
 
 ]
@@ -18,14 +18,15 @@
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3.6",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: Implementation :: PyPy",
     "Topic :: Utilities"]
 keywords = [
     "TSE",
     "Finance",
     "data",
     "cleaning",
```

### Comparing `namespace_mahdimir-0.0.0/PKG-INFO` & `namespace_mahdimir-0.0.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: namespace_mahdimir
-Version: 0.0.0
+Version: 0.0.2
 Summary: Some Namespaces for Python
 Project-URL: Homepage, https://github.com/imahdimir/namespace_mahdimir
 Project-URL: Bug Tracker, https://github.com/imahdimir/namespace_mahdimir/issues
 Author-email: Mahdi Mir <imahdimir@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Mahdi
@@ -33,9 +33,10 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Utilities
```

