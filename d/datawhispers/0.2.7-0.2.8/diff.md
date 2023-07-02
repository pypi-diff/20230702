# Comparing `tmp/datawhispers-0.2.7.tar.gz` & `tmp/datawhispers-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datawhispers-0.2.7.tar", last modified: Sat Jul  1 16:58:48 2023, max compression
+gzip compressed data, was "datawhispers-0.2.8.tar", last modified: Sun Jul  2 18:44:53 2023, max compression
```

## Comparing `datawhispers-0.2.7.tar` & `datawhispers-0.2.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 german     (501) staff       (20)        0 2023-07-01 16:58:48.038656 datawhispers-0.2.7/
--rw-r--r--   0 german     (501) staff       (20)     1061 2023-07-01 09:46:39.000000 datawhispers-0.2.7/LICENSE
--rw-r--r--   0 german     (501) staff       (20)     1556 2023-07-01 16:58:48.038536 datawhispers-0.2.7/PKG-INFO
--rw-r--r--   0 german     (501) staff       (20)      436 2023-07-01 11:20:15.000000 datawhispers-0.2.7/README.md
-drwxr-xr-x   0 german     (501) staff       (20)        0 2023-07-01 16:58:48.037542 datawhispers-0.2.7/datawhispers/
--rw-r--r--   0 german     (501) staff       (20)       75 2023-07-01 10:41:44.000000 datawhispers-0.2.7/datawhispers/__init__.py
--rw-r--r--   0 german     (501) staff       (20)     8342 2023-07-01 13:49:41.000000 datawhispers-0.2.7/datawhispers/advanced_prog.py
--rw-r--r--   0 german     (501) staff       (20)     7569 2023-07-01 09:48:05.000000 datawhispers-0.2.7/datawhispers/datavis.py
-drwxr-xr-x   0 german     (501) staff       (20)        0 2023-07-01 16:58:48.038323 datawhispers-0.2.7/datawhispers.egg-info/
--rw-r--r--   0 german     (501) staff       (20)     1556 2023-07-01 16:58:48.000000 datawhispers-0.2.7/datawhispers.egg-info/PKG-INFO
--rw-r--r--   0 german     (501) staff       (20)      284 2023-07-01 16:58:48.000000 datawhispers-0.2.7/datawhispers.egg-info/SOURCES.txt
--rw-r--r--   0 german     (501) staff       (20)        1 2023-07-01 16:58:48.000000 datawhispers-0.2.7/datawhispers.egg-info/dependency_links.txt
--rw-r--r--   0 german     (501) staff       (20)       38 2023-07-01 16:58:48.000000 datawhispers-0.2.7/datawhispers.egg-info/requires.txt
--rw-r--r--   0 german     (501) staff       (20)       13 2023-07-01 16:58:48.000000 datawhispers-0.2.7/datawhispers.egg-info/top_level.txt
--rw-r--r--   0 german     (501) staff       (20)       38 2023-07-01 16:58:48.038703 datawhispers-0.2.7/setup.cfg
--rw-r--r--   0 german     (501) staff       (20)     2271 2023-07-01 16:58:42.000000 datawhispers-0.2.7/setup.py
+drwxr-xr-x   0 german     (501) staff       (20)        0 2023-07-02 18:44:53.517411 datawhispers-0.2.8/
+-rw-r--r--   0 german     (501) staff       (20)     1061 2023-07-01 09:46:39.000000 datawhispers-0.2.8/LICENSE
+-rw-r--r--   0 german     (501) staff       (20)     1750 2023-07-02 18:44:53.517283 datawhispers-0.2.8/PKG-INFO
+-rw-r--r--   0 german     (501) staff       (20)      629 2023-07-02 13:40:10.000000 datawhispers-0.2.8/README.md
+drwxr-xr-x   0 german     (501) staff       (20)        0 2023-07-02 18:44:53.516044 datawhispers-0.2.8/datawhispers/
+-rw-r--r--   0 german     (501) staff       (20)       74 2023-07-02 18:37:43.000000 datawhispers-0.2.8/datawhispers/__init__.py
+-rw-r--r--   0 german     (501) staff       (20)     8342 2023-07-02 11:15:25.000000 datawhispers-0.2.8/datawhispers/advancedProg.py
+-rw-r--r--   0 german     (501) staff       (20)     7569 2023-07-01 09:48:05.000000 datawhispers-0.2.8/datawhispers/datavis.py
+drwxr-xr-x   0 german     (501) staff       (20)        0 2023-07-02 18:44:53.517066 datawhispers-0.2.8/datawhispers.egg-info/
+-rw-r--r--   0 german     (501) staff       (20)     1750 2023-07-02 18:44:53.000000 datawhispers-0.2.8/datawhispers.egg-info/PKG-INFO
+-rw-r--r--   0 german     (501) staff       (20)      283 2023-07-02 18:44:53.000000 datawhispers-0.2.8/datawhispers.egg-info/SOURCES.txt
+-rw-r--r--   0 german     (501) staff       (20)        1 2023-07-02 18:44:53.000000 datawhispers-0.2.8/datawhispers.egg-info/dependency_links.txt
+-rw-r--r--   0 german     (501) staff       (20)       38 2023-07-02 18:44:53.000000 datawhispers-0.2.8/datawhispers.egg-info/requires.txt
+-rw-r--r--   0 german     (501) staff       (20)       13 2023-07-02 18:44:53.000000 datawhispers-0.2.8/datawhispers.egg-info/top_level.txt
+-rw-r--r--   0 german     (501) staff       (20)       38 2023-07-02 18:44:53.517458 datawhispers-0.2.8/setup.cfg
+-rw-r--r--   0 german     (501) staff       (20)     2271 2023-07-02 18:43:18.000000 datawhispers-0.2.8/setup.py
```

### Comparing `datawhispers-0.2.7/LICENSE` & `datawhispers-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `datawhispers-0.2.7/PKG-INFO` & `datawhispers-0.2.8/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datawhispers
-Version: 0.2.7
+Version: 0.2.8
 Summary: This is a library to solve regression problems or statistical analysis for the DHBW Mannheim courses Advanced Programming and Data Visualisation
 Home-page: https://github.com/GermanPaul12/datawhispers
 Download-URL: https://github.com/GermanPaul12/datawhispers/archive/v_01.tar.gz
 Author: German Paul
 Author-email: motets-rosiest-0r@icloud.com
 License: MIT
 Keywords: Python3,Data Visualisation,Statistical Analysis,Regression,Advanced Programming
@@ -18,14 +18,20 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# The DataWhispers module is used for solving regression and statistical problems
+# DataWhispers Module
 
-## It was programmed for exams in advanced programming and data visualisation at DHBW Mannheim
+![DataWhispers Logo](assets/logo.png)
 
-### Solve regression problems (lin, poly, trig, free, least_squares), plot the results and mnist numbers or do some statistical analysis with chi2, pearson or student-t
+## Documentation: [![doc](https://img.shields.io/badge/Made%20with-Sphinx-1f425f.svg)](https://germanpaul12.github.io/datawhispers/)
 
-#### To install just write "pip install datawhispers" in your command prompt of choice
+### The **DataWhispers** module is used for solving regression and statistical problems
+
+It was programmed for exams in advanced programming and data visualisation at DHBW Mannheim
+
+Solve regression problems (lin, poly, trig, free, least_squares), plot the results and mnist numbers or do some statistical analysis with chi2, pearson or student-t
+
+To install just write ```pip install datawhispers``` in your command prompt of choice
```

### Comparing `datawhispers-0.2.7/datawhispers/advanced_prog.py` & `datawhispers-0.2.8/datawhispers/advancedProg.py`

 * *Files identical despite different names*

### Comparing `datawhispers-0.2.7/datawhispers/datavis.py` & `datawhispers-0.2.8/datawhispers/datavis.py`

 * *Files identical despite different names*

### Comparing `datawhispers-0.2.7/datawhispers.egg-info/PKG-INFO` & `datawhispers-0.2.8/datawhispers.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datawhispers
-Version: 0.2.7
+Version: 0.2.8
 Summary: This is a library to solve regression problems or statistical analysis for the DHBW Mannheim courses Advanced Programming and Data Visualisation
 Home-page: https://github.com/GermanPaul12/datawhispers
 Download-URL: https://github.com/GermanPaul12/datawhispers/archive/v_01.tar.gz
 Author: German Paul
 Author-email: motets-rosiest-0r@icloud.com
 License: MIT
 Keywords: Python3,Data Visualisation,Statistical Analysis,Regression,Advanced Programming
@@ -18,14 +18,20 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# The DataWhispers module is used for solving regression and statistical problems
+# DataWhispers Module
 
-## It was programmed for exams in advanced programming and data visualisation at DHBW Mannheim
+![DataWhispers Logo](assets/logo.png)
 
-### Solve regression problems (lin, poly, trig, free, least_squares), plot the results and mnist numbers or do some statistical analysis with chi2, pearson or student-t
+## Documentation: [![doc](https://img.shields.io/badge/Made%20with-Sphinx-1f425f.svg)](https://germanpaul12.github.io/datawhispers/)
 
-#### To install just write "pip install datawhispers" in your command prompt of choice
+### The **DataWhispers** module is used for solving regression and statistical problems
+
+It was programmed for exams in advanced programming and data visualisation at DHBW Mannheim
+
+Solve regression problems (lin, poly, trig, free, least_squares), plot the results and mnist numbers or do some statistical analysis with chi2, pearson or student-t
+
+To install just write ```pip install datawhispers``` in your command prompt of choice
```

### Comparing `datawhispers-0.2.7/setup.py` & `datawhispers-0.2.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from distutils.core import setup
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 setup(
   name = 'datawhispers',         # How you named your package folder (MyLib)
   packages = ["datawhispers"],   # Chose the same as "name"
-  version = '0.2.7',      # Start with a small number and increase it with every change you make
+  version = '0.2.8',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'This is a library to solve regression problems or statistical analysis for the DHBW Mannheim courses Advanced Programming and Data Visualisation',   # Give a short description about your library
   author = 'German Paul',                   # Type in your name
   author_email = 'motets-rosiest-0r@icloud.com',      # Type in your E-Mail
   url = 'https://github.com/GermanPaul12/datawhispers',   # Provide either the link to your github or to your website
   download_url = 'https://github.com/GermanPaul12/datawhispers/archive/v_01.tar.gz',    # I explain this later on
   keywords = ['Python3', 'Data Visualisation', 'Statistical Analysis', "Regression", "Advanced Programming"],   # Keywords that define your package best
```

