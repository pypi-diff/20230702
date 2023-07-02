# Comparing `tmp/climalysis-0.2.0.tar.gz` & `tmp/climalysis-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "climalysis-0.2.0.tar", last modified: Fri Jun 16 17:38:58 2023, max compression
+gzip compressed data, was "climalysis-0.2.1.tar", last modified: Sun Jul  2 11:20:11 2023, max compression
```

## Comparing `climalysis-0.2.0.tar` & `climalysis-0.2.1.tar`

### file list

```diff
@@ -1,16 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:38:58.604428 climalysis-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-16 17:38:44.000000 climalysis-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3384 2023-06-16 17:38:58.604428 climalysis-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-06-16 17:38:44.000000 climalysis-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:38:58.604428 climalysis-0.2.0/climalysis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3384 2023-06-16 17:38:58.000000 climalysis-0.2.0/climalysis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-16 17:38:58.000000 climalysis-0.2.0/climalysis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 17:38:58.000000 climalysis-0.2.0/climalysis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-16 17:38:58.000000 climalysis-0.2.0/climalysis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-16 17:38:58.000000 climalysis-0.2.0/climalysis.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 17:38:58.604428 climalysis-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-06-16 17:38:44.000000 climalysis-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:38:58.604428 climalysis-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 17:38:44.000000 climalysis-0.2.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 17:38:44.000000 climalysis-0.2.0/tests/test_module1.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 17:38:44.000000 climalysis-0.2.0/tests/test_module2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 11:20:11.087338 climalysis-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-02 11:19:54.000000 climalysis-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3384 2023-07-02 11:20:11.087338 climalysis-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-07-02 11:19:54.000000 climalysis-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 11:20:11.083338 climalysis-0.2.1/climalysis/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-02 11:19:54.000000 climalysis-0.2.1/climalysis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 11:20:11.087338 climalysis-0.2.1/climalysis/indices/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 11:19:54.000000 climalysis-0.2.1/climalysis/indices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 11:19:54.000000 climalysis-0.2.1/climalysis/indices/module1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 11:20:11.087338 climalysis-0.2.1/climalysis/mapping/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 11:19:54.000000 climalysis-0.2.1/climalysis/mapping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 11:19:54.000000 climalysis-0.2.1/climalysis/mapping/module1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 11:20:11.087338 climalysis-0.2.1/climalysis/series/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 11:19:54.000000 climalysis-0.2.1/climalysis/series/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 11:19:54.000000 climalysis-0.2.1/climalysis/series/module1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 11:20:11.087338 climalysis-0.2.1/climalysis/statistics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 11:19:54.000000 climalysis-0.2.1/climalysis/statistics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-07-02 11:19:54.000000 climalysis-0.2.1/climalysis/statistics/moving_average.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 11:20:11.083338 climalysis-0.2.1/climalysis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3384 2023-07-02 11:20:11.000000 climalysis-0.2.1/climalysis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-07-02 11:20:11.000000 climalysis-0.2.1/climalysis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 11:20:11.000000 climalysis-0.2.1/climalysis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-02 11:20:11.000000 climalysis-0.2.1/climalysis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-02 11:20:11.000000 climalysis-0.2.1/climalysis.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 11:20:11.087338 climalysis-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-07-02 11:19:54.000000 climalysis-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 11:20:11.087338 climalysis-0.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 11:19:54.000000 climalysis-0.2.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 11:19:54.000000 climalysis-0.2.1/tests/test_module1.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 11:19:54.000000 climalysis-0.2.1/tests/test_module2.py
```

### Comparing `climalysis-0.2.0/LICENSE` & `climalysis-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `climalysis-0.2.0/PKG-INFO` & `climalysis-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: climalysis
-Version: 0.2.0
+Version: 0.2.1
 Summary: A comprehensive toolkit for climate impact analysis.
 Author: Jake Casselman
 Author-email: <jake.casselman@climalinks.com
 Keywords: python,climate,analysis,climate analysis,climate data,impact analysis
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
```

### Comparing `climalysis-0.2.0/README.md` & `climalysis-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `climalysis-0.2.0/climalysis.egg-info/PKG-INFO` & `climalysis-0.2.1/climalysis.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: climalysis
-Version: 0.2.0
+Version: 0.2.1
 Summary: A comprehensive toolkit for climate impact analysis.
 Author: Jake Casselman
 Author-email: <jake.casselman@climalinks.com
 Keywords: python,climate,analysis,climate analysis,climate data,impact analysis
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
```

### Comparing `climalysis-0.2.0/setup.py` & `climalysis-0.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.2.0'
+VERSION = '0.2.1'
 DESCRIPTION = 'A comprehensive toolkit for climate impact analysis.'
 LONG_DESCRIPTION = 'A package that allows researchers, analysts, and climate enthusiasts to dissect complex climate data.'
 
 # Setting up
 setup(
     name="climalysis",
     version=VERSION,
```

