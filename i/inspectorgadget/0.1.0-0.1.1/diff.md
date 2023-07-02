# Comparing `tmp/inspectorgadget-0.1.0.tar.gz` & `tmp/inspectorgadget-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inspectorgadget-0.1.0.tar", max compression
+gzip compressed data, was "inspectorgadget-0.1.1.tar", max compression
```

## Comparing `inspectorgadget-0.1.0.tar` & `inspectorgadget-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1067 2023-06-28 20:36:56.302986 inspectorgadget-0.1.0/LICENSE
--rw-r--r--   0        0        0     1324 2023-06-28 20:36:56.302986 inspectorgadget-0.1.0/README.md
--rw-r--r--   0        0        0     4848 2023-06-28 20:36:56.302986 inspectorgadget-0.1.0/inspectorgadget/__init__.py
--rw-r--r--   0        0        0     2170 2023-06-28 20:36:56.302986 inspectorgadget-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1873 1970-01-01 00:00:00.000000 inspectorgadget-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-07-02 20:19:58.453060 inspectorgadget-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1324 2023-07-02 20:19:58.453060 inspectorgadget-0.1.1/README.md
+-rw-r--r--   0        0        0     4843 2023-07-02 20:19:58.453060 inspectorgadget-0.1.1/inspectorgadget/__init__.py
+-rw-r--r--   0        0        0     2170 2023-07-02 20:19:58.453060 inspectorgadget-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1873 1970-01-01 00:00:00.000000 inspectorgadget-0.1.1/PKG-INFO
```

### Comparing `inspectorgadget-0.1.0/LICENSE` & `inspectorgadget-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `inspectorgadget-0.1.0/README.md` & `inspectorgadget-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `inspectorgadget-0.1.0/inspectorgadget/__init__.py` & `inspectorgadget-0.1.1/inspectorgadget/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,15 @@
     In case of given variables `vars_` the caller equivalent is returned.
 
     >>> get_signature(func, {'a': 4, 'b': 2})
     'func(4)'
     >>> get_signature(func, {'a': 4, 'b': 9})
     'func(4, b=9)'
 
-    This is useful in combination with :any:`vars()`.
+    This is useful in combination with `vars()`.
 
     >>> def func(a, b=2):
     ...     print(get_signature(func, vars()))
     >>> func(10, b=8)
     func(10, b=8)
 
     Positional arguments:
```

### Comparing `inspectorgadget-0.1.0/pyproject.toml` & `inspectorgadget-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "inspectorgadget"
-version = "0.1.0"
+version = "0.1.1"
 description = "Inspector Gadget - Extended Python Inspection"
 readme = "README.md"
 license = "MIT"
 authors = [
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `inspectorgadget-0.1.0/PKG-INFO` & `inspectorgadget-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inspectorgadget
-Version: 0.1.0
+Version: 0.1.1
 Summary: Inspector Gadget - Extended Python Inspection
 License: MIT
 Requires-Python: >=3.7.2,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

