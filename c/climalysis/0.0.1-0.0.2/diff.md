# Comparing `tmp/climalysis-0.0.1.tar.gz` & `tmp/climalysis-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "climalysis-0.0.1.tar", last modified: Sun Jul  2 12:25:35 2023, max compression
+gzip compressed data, was "climalysis-0.0.2.tar", last modified: Sun Jul  2 12:45:05 2023, max compression
```

## Comparing `climalysis-0.0.1.tar` & `climalysis-0.0.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 12:25:35.210150 climalysis-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-02 12:25:17.000000 climalysis-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3384 2023-07-02 12:25:35.210150 climalysis-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-07-02 12:25:17.000000 climalysis-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 12:25:35.206150 climalysis-0.0.1/climalysis/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-02 12:25:17.000000 climalysis-0.0.1/climalysis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 12:25:35.206150 climalysis-0.0.1/climalysis/indices/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 12:25:17.000000 climalysis-0.0.1/climalysis/indices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-07-02 12:25:17.000000 climalysis-0.0.1/climalysis/indices/ninoSST.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 12:25:35.206150 climalysis-0.0.1/climalysis/mapping/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 12:25:17.000000 climalysis-0.0.1/climalysis/mapping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 12:25:17.000000 climalysis-0.0.1/climalysis/mapping/module1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 12:25:35.210150 climalysis-0.0.1/climalysis/series/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 12:25:17.000000 climalysis-0.0.1/climalysis/series/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 12:25:17.000000 climalysis-0.0.1/climalysis/series/module1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 12:25:35.210150 climalysis-0.0.1/climalysis/statistics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 12:25:17.000000 climalysis-0.0.1/climalysis/statistics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-07-02 12:25:17.000000 climalysis-0.0.1/climalysis/statistics/fisherTransform.py
--rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-07-02 12:25:17.000000 climalysis-0.0.1/climalysis/statistics/linearDetrend.py
--rw-r--r--   0 runner    (1001) docker     (123)     4787 2023-07-02 12:25:17.000000 climalysis-0.0.1/climalysis/statistics/lowessAnalysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-07-02 12:25:17.000000 climalysis-0.0.1/climalysis/statistics/movingAverage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 12:25:35.206150 climalysis-0.0.1/climalysis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3384 2023-07-02 12:25:35.000000 climalysis-0.0.1/climalysis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-07-02 12:25:35.000000 climalysis-0.0.1/climalysis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 12:25:35.000000 climalysis-0.0.1/climalysis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-02 12:25:35.000000 climalysis-0.0.1/climalysis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-02 12:25:35.000000 climalysis-0.0.1/climalysis.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 12:25:35.210150 climalysis-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-07-02 12:25:17.000000 climalysis-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 12:25:35.210150 climalysis-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 12:25:17.000000 climalysis-0.0.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 12:25:17.000000 climalysis-0.0.1/tests/test_module1.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 12:25:17.000000 climalysis-0.0.1/tests/test_module2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 12:45:05.475837 climalysis-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-02 12:44:52.000000 climalysis-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-07-02 12:45:05.475837 climalysis-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-07-02 12:44:52.000000 climalysis-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 12:45:05.471837 climalysis-0.0.2/climalysis/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-02 12:44:52.000000 climalysis-0.0.2/climalysis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 12:45:05.471837 climalysis-0.0.2/climalysis/indices/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 12:44:52.000000 climalysis-0.0.2/climalysis/indices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-07-02 12:44:52.000000 climalysis-0.0.2/climalysis/indices/ninoSST.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 12:45:05.475837 climalysis-0.0.2/climalysis/mapping/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 12:44:52.000000 climalysis-0.0.2/climalysis/mapping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 12:44:52.000000 climalysis-0.0.2/climalysis/mapping/module1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 12:45:05.475837 climalysis-0.0.2/climalysis/series/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 12:44:52.000000 climalysis-0.0.2/climalysis/series/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 12:44:52.000000 climalysis-0.0.2/climalysis/series/module1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 12:45:05.475837 climalysis-0.0.2/climalysis/statistics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 12:44:52.000000 climalysis-0.0.2/climalysis/statistics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-07-02 12:44:52.000000 climalysis-0.0.2/climalysis/statistics/fisherTransform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-07-02 12:44:52.000000 climalysis-0.0.2/climalysis/statistics/linearDetrend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4787 2023-07-02 12:44:52.000000 climalysis-0.0.2/climalysis/statistics/lowessAnalysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-07-02 12:44:52.000000 climalysis-0.0.2/climalysis/statistics/movingAverage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 12:45:05.471837 climalysis-0.0.2/climalysis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-07-02 12:45:05.000000 climalysis-0.0.2/climalysis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-07-02 12:45:05.000000 climalysis-0.0.2/climalysis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 12:45:05.000000 climalysis-0.0.2/climalysis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-02 12:45:05.000000 climalysis-0.0.2/climalysis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-02 12:45:05.000000 climalysis-0.0.2/climalysis.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 12:45:05.475837 climalysis-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-07-02 12:44:52.000000 climalysis-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 12:45:05.475837 climalysis-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 12:44:52.000000 climalysis-0.0.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 12:44:52.000000 climalysis-0.0.2/tests/test_module1.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 12:44:52.000000 climalysis-0.0.2/tests/test_module2.py
```

### Comparing `climalysis-0.0.1/LICENSE` & `climalysis-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `climalysis-0.0.1/PKG-INFO` & `climalysis-0.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: climalysis
-Version: 0.0.1
+Version: 0.0.2
 Summary: A comprehensive toolkit for climate impact analysis.
 Author: Jake Casselman
 Author-email: <jake.casselman@climalinks.com
 Keywords: python,climate,analysis,climate analysis,climate data,impact analysis
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Atmospheric Science
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # Climalysis: Your Toolkit for Climate Impact Analysis ☁️🌞
-[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://github.com/jake-casselman/climalysis/blob/main/LICENSE) [![codebeat badge](https://codebeat.co/badges/d65911fc-a11d-4ca2-a914-792df78cb420)](https://codebeat.co/projects/github-com-jake-casselman-climalysis-main) ![PyPI](https://img.shields.io/pypi/v/climalysis.svg) [![DOI](https://zenodo.org/badge/652251221.svg)](https://zenodo.org/badge/latestdoi/652251221)
+[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://github.com/jake-casselman/climalysis/blob/main/LICENSE) [![codebeat badge](https://codebeat.co/badges/d65911fc-a11d-4ca2-a914-792df78cb420)](https://codebeat.co/projects/github-com-jake-casselman-climalysis-main) ![PyPI](https://img.shields.io/pypi/v/climalysis.svg) [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.8105734.svg)](https://doi.org/10.5281/zenodo.8105734)
+
 
 
 
 Developed by an assortment of active and past climate researchers, Climalysis is more than just a project – it's your one-stop platform for comprehensive climate impact studies. 
 
 **Our Mission:**
```

### Comparing `climalysis-0.0.1/README.md` & `climalysis-0.0.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # Climalysis: Your Toolkit for Climate Impact Analysis ☁️🌞
-[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://github.com/jake-casselman/climalysis/blob/main/LICENSE) [![codebeat badge](https://codebeat.co/badges/d65911fc-a11d-4ca2-a914-792df78cb420)](https://codebeat.co/projects/github-com-jake-casselman-climalysis-main) ![PyPI](https://img.shields.io/pypi/v/climalysis.svg) [![DOI](https://zenodo.org/badge/652251221.svg)](https://zenodo.org/badge/latestdoi/652251221)
+[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://github.com/jake-casselman/climalysis/blob/main/LICENSE) [![codebeat badge](https://codebeat.co/badges/d65911fc-a11d-4ca2-a914-792df78cb420)](https://codebeat.co/projects/github-com-jake-casselman-climalysis-main) ![PyPI](https://img.shields.io/pypi/v/climalysis.svg) [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.8105734.svg)](https://doi.org/10.5281/zenodo.8105734)
+
 
 
 
 Developed by an assortment of active and past climate researchers, Climalysis is more than just a project – it's your one-stop platform for comprehensive climate impact studies. 
 
 **Our Mission:**
```

### Comparing `climalysis-0.0.1/climalysis/indices/ninoSST.py` & `climalysis-0.0.2/climalysis/indices/ninoSST.py`

 * *Files identical despite different names*

### Comparing `climalysis-0.0.1/climalysis/statistics/fisherTransform.py` & `climalysis-0.0.2/climalysis/statistics/fisherTransform.py`

 * *Files identical despite different names*

### Comparing `climalysis-0.0.1/climalysis/statistics/linearDetrend.py` & `climalysis-0.0.2/climalysis/statistics/linearDetrend.py`

 * *Files identical despite different names*

### Comparing `climalysis-0.0.1/climalysis/statistics/lowessAnalysis.py` & `climalysis-0.0.2/climalysis/statistics/lowessAnalysis.py`

 * *Files identical despite different names*

### Comparing `climalysis-0.0.1/climalysis/statistics/movingAverage.py` & `climalysis-0.0.2/climalysis/statistics/movingAverage.py`

 * *Files identical despite different names*

### Comparing `climalysis-0.0.1/climalysis.egg-info/PKG-INFO` & `climalysis-0.0.2/climalysis.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: climalysis
-Version: 0.0.1
+Version: 0.0.2
 Summary: A comprehensive toolkit for climate impact analysis.
 Author: Jake Casselman
 Author-email: <jake.casselman@climalinks.com
 Keywords: python,climate,analysis,climate analysis,climate data,impact analysis
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Atmospheric Science
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # Climalysis: Your Toolkit for Climate Impact Analysis ☁️🌞
-[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://github.com/jake-casselman/climalysis/blob/main/LICENSE) [![codebeat badge](https://codebeat.co/badges/d65911fc-a11d-4ca2-a914-792df78cb420)](https://codebeat.co/projects/github-com-jake-casselman-climalysis-main) ![PyPI](https://img.shields.io/pypi/v/climalysis.svg) [![DOI](https://zenodo.org/badge/652251221.svg)](https://zenodo.org/badge/latestdoi/652251221)
+[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://github.com/jake-casselman/climalysis/blob/main/LICENSE) [![codebeat badge](https://codebeat.co/badges/d65911fc-a11d-4ca2-a914-792df78cb420)](https://codebeat.co/projects/github-com-jake-casselman-climalysis-main) ![PyPI](https://img.shields.io/pypi/v/climalysis.svg) [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.8105734.svg)](https://doi.org/10.5281/zenodo.8105734)
+
 
 
 
 Developed by an assortment of active and past climate researchers, Climalysis is more than just a project – it's your one-stop platform for comprehensive climate impact studies. 
 
 **Our Mission:**
```

### Comparing `climalysis-0.0.1/climalysis.egg-info/SOURCES.txt` & `climalysis-0.0.2/climalysis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `climalysis-0.0.1/setup.py` & `climalysis-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = 'A comprehensive toolkit for climate impact analysis.'
 LONG_DESCRIPTION = 'A package that allows researchers, analysts, and climate enthusiasts to dissect complex climate data.'
 
 # Setting up
 setup(
     name="climalysis",
     version=VERSION,
```

