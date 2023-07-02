# Comparing `tmp/climalysis-0.0.3.tar.gz` & `tmp/climalysis-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "climalysis-0.0.3.tar", last modified: Sun Jul  2 12:58:03 2023, max compression
+gzip compressed data, was "climalysis-0.0.4.tar", last modified: Sun Jul  2 13:00:33 2023, max compression
```

## Comparing `climalysis-0.0.3.tar` & `climalysis-0.0.4.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 12:58:03.270338 climalysis-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-02 12:57:21.000000 climalysis-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3647 2023-07-02 12:58:03.270338 climalysis-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-07-02 12:57:21.000000 climalysis-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 12:58:03.266338 climalysis-0.0.3/climalysis/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-02 12:57:21.000000 climalysis-0.0.3/climalysis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 12:58:03.266338 climalysis-0.0.3/climalysis/indices/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 12:57:21.000000 climalysis-0.0.3/climalysis/indices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-07-02 12:57:21.000000 climalysis-0.0.3/climalysis/indices/ninoSST.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 12:58:03.266338 climalysis-0.0.3/climalysis/mapping/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 12:57:21.000000 climalysis-0.0.3/climalysis/mapping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 12:57:21.000000 climalysis-0.0.3/climalysis/mapping/module1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 12:58:03.266338 climalysis-0.0.3/climalysis/series/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 12:57:21.000000 climalysis-0.0.3/climalysis/series/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 12:57:21.000000 climalysis-0.0.3/climalysis/series/module1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 12:58:03.270338 climalysis-0.0.3/climalysis/statistics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 12:57:21.000000 climalysis-0.0.3/climalysis/statistics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-07-02 12:57:21.000000 climalysis-0.0.3/climalysis/statistics/fisherTransform.py
--rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-07-02 12:57:21.000000 climalysis-0.0.3/climalysis/statistics/linearDetrend.py
--rw-r--r--   0 runner    (1001) docker     (123)     4787 2023-07-02 12:57:21.000000 climalysis-0.0.3/climalysis/statistics/lowessAnalysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-07-02 12:57:21.000000 climalysis-0.0.3/climalysis/statistics/movingAverage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 12:58:03.266338 climalysis-0.0.3/climalysis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3647 2023-07-02 12:58:03.000000 climalysis-0.0.3/climalysis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-07-02 12:58:03.000000 climalysis-0.0.3/climalysis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 12:58:03.000000 climalysis-0.0.3/climalysis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-02 12:58:03.000000 climalysis-0.0.3/climalysis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-02 12:58:03.000000 climalysis-0.0.3/climalysis.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 12:58:03.270338 climalysis-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-07-02 12:57:21.000000 climalysis-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 12:58:03.270338 climalysis-0.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 12:57:21.000000 climalysis-0.0.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 12:57:21.000000 climalysis-0.0.3/tests/test_module1.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 12:57:21.000000 climalysis-0.0.3/tests/test_module2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:00:33.628692 climalysis-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-02 12:59:54.000000 climalysis-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-07-02 13:00:33.624692 climalysis-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-07-02 12:59:54.000000 climalysis-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:00:33.620692 climalysis-0.0.4/climalysis/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-02 12:59:54.000000 climalysis-0.0.4/climalysis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:00:33.624692 climalysis-0.0.4/climalysis/indices/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 12:59:54.000000 climalysis-0.0.4/climalysis/indices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-07-02 12:59:54.000000 climalysis-0.0.4/climalysis/indices/ninoSST.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:00:33.624692 climalysis-0.0.4/climalysis/mapping/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 12:59:54.000000 climalysis-0.0.4/climalysis/mapping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 12:59:54.000000 climalysis-0.0.4/climalysis/mapping/module1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:00:33.624692 climalysis-0.0.4/climalysis/series/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 12:59:54.000000 climalysis-0.0.4/climalysis/series/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 12:59:54.000000 climalysis-0.0.4/climalysis/series/module1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:00:33.624692 climalysis-0.0.4/climalysis/statistics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 12:59:54.000000 climalysis-0.0.4/climalysis/statistics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-07-02 12:59:54.000000 climalysis-0.0.4/climalysis/statistics/fisherTransform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-07-02 12:59:54.000000 climalysis-0.0.4/climalysis/statistics/linearDetrend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4787 2023-07-02 12:59:54.000000 climalysis-0.0.4/climalysis/statistics/lowessAnalysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-07-02 12:59:54.000000 climalysis-0.0.4/climalysis/statistics/movingAverage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:00:33.624692 climalysis-0.0.4/climalysis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-07-02 13:00:33.000000 climalysis-0.0.4/climalysis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-07-02 13:00:33.000000 climalysis-0.0.4/climalysis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 13:00:33.000000 climalysis-0.0.4/climalysis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-02 13:00:33.000000 climalysis-0.0.4/climalysis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-02 13:00:33.000000 climalysis-0.0.4/climalysis.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 13:00:33.628692 climalysis-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-07-02 12:59:54.000000 climalysis-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:00:33.624692 climalysis-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 12:59:54.000000 climalysis-0.0.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 12:59:54.000000 climalysis-0.0.4/tests/test_module1.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 12:59:54.000000 climalysis-0.0.4/tests/test_module2.py
```

### Comparing `climalysis-0.0.3/LICENSE` & `climalysis-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `climalysis-0.0.3/PKG-INFO` & `climalysis-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: climalysis
-Version: 0.0.3
+Version: 0.0.4
 Summary: A comprehensive toolkit for climate impact analysis.
 Author: Jake Casselman
 Author-email: <jake.casselman@climalinks.com
 Keywords: python,climate,analysis,climate analysis,climate data,impact analysis
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
@@ -75,15 +75,15 @@
 - statsmodels==0.13.5
 - xarray==2023.3.0
 
 These packages can be installed using pip by running the following command in your terminal:
 
 ```bash
 pip install -r requirements.txt
-
+```
 
 ## Usage
 
 After installation, you can import and use our package in your Python scripts:
 
 ```python
 from climalysis import module1, module2
```

### Comparing `climalysis-0.0.3/README.md` & `climalysis-0.0.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 - statsmodels==0.13.5
 - xarray==2023.3.0
 
 These packages can be installed using pip by running the following command in your terminal:
 
 ```bash
 pip install -r requirements.txt
-
+```
 
 ## Usage
 
 After installation, you can import and use our package in your Python scripts:
 
 ```python
 from climalysis import module1, module2
```

### Comparing `climalysis-0.0.3/climalysis/indices/ninoSST.py` & `climalysis-0.0.4/climalysis/indices/ninoSST.py`

 * *Files identical despite different names*

### Comparing `climalysis-0.0.3/climalysis/statistics/fisherTransform.py` & `climalysis-0.0.4/climalysis/statistics/fisherTransform.py`

 * *Files identical despite different names*

### Comparing `climalysis-0.0.3/climalysis/statistics/linearDetrend.py` & `climalysis-0.0.4/climalysis/statistics/linearDetrend.py`

 * *Files identical despite different names*

### Comparing `climalysis-0.0.3/climalysis/statistics/lowessAnalysis.py` & `climalysis-0.0.4/climalysis/statistics/lowessAnalysis.py`

 * *Files identical despite different names*

### Comparing `climalysis-0.0.3/climalysis/statistics/movingAverage.py` & `climalysis-0.0.4/climalysis/statistics/movingAverage.py`

 * *Files identical despite different names*

### Comparing `climalysis-0.0.3/climalysis.egg-info/PKG-INFO` & `climalysis-0.0.4/climalysis.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: climalysis
-Version: 0.0.3
+Version: 0.0.4
 Summary: A comprehensive toolkit for climate impact analysis.
 Author: Jake Casselman
 Author-email: <jake.casselman@climalinks.com
 Keywords: python,climate,analysis,climate analysis,climate data,impact analysis
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
@@ -75,15 +75,15 @@
 - statsmodels==0.13.5
 - xarray==2023.3.0
 
 These packages can be installed using pip by running the following command in your terminal:
 
 ```bash
 pip install -r requirements.txt
-
+```
 
 ## Usage
 
 After installation, you can import and use our package in your Python scripts:
 
 ```python
 from climalysis import module1, module2
```

### Comparing `climalysis-0.0.3/climalysis.egg-info/SOURCES.txt` & `climalysis-0.0.4/climalysis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `climalysis-0.0.3/setup.py` & `climalysis-0.0.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.3'
+VERSION = '0.0.4'
 DESCRIPTION = 'A comprehensive toolkit for climate impact analysis.'
 LONG_DESCRIPTION = 'A package that allows researchers, analysts, and climate enthusiasts to dissect complex climate data.'
 
 # Setting up
 setup(
     name="climalysis",
     version=VERSION,
```

