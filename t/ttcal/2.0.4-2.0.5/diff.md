# Comparing `tmp/ttcal-2.0.4.tar.gz` & `tmp/ttcal-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ttcal-2.0.4.tar", last modified: Sun Jul  2 19:53:12 2023, max compression
+gzip compressed data, was "ttcal-2.0.5.tar", last modified: Sun Jul  2 19:59:31 2023, max compression
```

## Comparing `ttcal-2.0.4.tar` & `ttcal-2.0.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 19:53:12.643231 ttcal-2.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-07-02 19:53:00.000000 ttcal-2.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-07-02 19:53:12.643231 ttcal-2.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-07-02 19:53:00.000000 ttcal-2.0.4/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-02 19:53:12.643231 ttcal-2.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-02 19:53:00.000000 ttcal-2.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 19:53:12.643231 ttcal-2.0.4/ttcal/
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-07-02 19:53:00.000000 ttcal-2.0.4/ttcal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-07-02 19:53:00.000000 ttcal-2.0.4/ttcal/calfns.py
--rw-r--r--   0 runner    (1001) docker     (123)    15869 2023-07-02 19:53:00.000000 ttcal-2.0.4/ttcal/day.py
--rw-r--r--   0 runner    (1001) docker     (123)     9262 2023-07-02 19:53:00.000000 ttcal-2.0.4/ttcal/duration.py
--rw-r--r--   0 runner    (1001) docker     (123)    10783 2023-07-02 19:53:00.000000 ttcal-2.0.4/ttcal/month.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 19:53:12.643231 ttcal-2.0.4/ttcal/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 19:53:00.000000 ttcal-2.0.4/ttcal/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-02 19:53:00.000000 ttcal-2.0.4/ttcal/templatetags/ttcal_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     6399 2023-07-02 19:53:00.000000 ttcal-2.0.4/ttcal/week.py
--rw-r--r--   0 runner    (1001) docker     (123)     8524 2023-07-02 19:53:00.000000 ttcal-2.0.4/ttcal/year.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 19:53:12.643231 ttcal-2.0.4/ttcal.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-07-02 19:53:12.000000 ttcal-2.0.4/ttcal.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-02 19:53:12.000000 ttcal-2.0.4/ttcal.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 19:53:12.000000 ttcal-2.0.4/ttcal.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 19:53:12.000000 ttcal-2.0.4/ttcal.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-02 19:53:12.000000 ttcal-2.0.4/ttcal.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 19:59:31.648700 ttcal-2.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-07-02 19:59:19.000000 ttcal-2.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-07-02 19:59:31.648700 ttcal-2.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-07-02 19:59:19.000000 ttcal-2.0.5/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-02 19:59:31.648700 ttcal-2.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-07-02 19:59:19.000000 ttcal-2.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 19:59:31.648700 ttcal-2.0.5/ttcal/
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-07-02 19:59:19.000000 ttcal-2.0.5/ttcal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-07-02 19:59:19.000000 ttcal-2.0.5/ttcal/calfns.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15869 2023-07-02 19:59:19.000000 ttcal-2.0.5/ttcal/day.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9262 2023-07-02 19:59:19.000000 ttcal-2.0.5/ttcal/duration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10783 2023-07-02 19:59:19.000000 ttcal-2.0.5/ttcal/month.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 19:59:31.648700 ttcal-2.0.5/ttcal/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 19:59:19.000000 ttcal-2.0.5/ttcal/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-02 19:59:19.000000 ttcal-2.0.5/ttcal/templatetags/ttcal_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6399 2023-07-02 19:59:19.000000 ttcal-2.0.5/ttcal/week.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8524 2023-07-02 19:59:19.000000 ttcal-2.0.5/ttcal/year.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 19:59:31.648700 ttcal-2.0.5/ttcal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-07-02 19:59:31.000000 ttcal-2.0.5/ttcal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-02 19:59:31.000000 ttcal-2.0.5/ttcal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 19:59:31.000000 ttcal-2.0.5/ttcal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 19:59:31.000000 ttcal-2.0.5/ttcal.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-02 19:59:31.000000 ttcal-2.0.5/ttcal.egg-info/top_level.txt
```

### Comparing `ttcal-2.0.4/LICENSE` & `ttcal-2.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ttcal-2.0.4/PKG-INFO` & `ttcal-2.0.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: ttcal
-Version: 2.0.4
-Summary: UNKNOWN
+Version: 2.0.5
+Summary: ttcal - calendar operations
 Home-page: https://github.com/datakortet/ttcal
 Author: Bjorn Pettersen
 Author-email: bp@datakortet.no
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `ttcal-2.0.4/README.rst` & `ttcal-2.0.5/README.rst`

 * *Files identical despite different names*

### Comparing `ttcal-2.0.4/setup.py` & `ttcal-2.0.5/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,39 +1,38 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 """
 ttcal - calendar operations
-===========================
 """
 
 classifiers = """\
 Development Status :: 5 - Production/Stable
 Intended Audience :: Developers
 Programming Language :: Python
 Programming Language :: Python :: 3
 Topic :: Software Development :: Libraries
 """
 
-import sys, os
+import os
 import setuptools
 
-version = '2.0.4'
+version = '2.0.5'
 
 DIRNAME = os.path.dirname(__file__)
 description = open(os.path.join(DIRNAME, 'README.rst'), 'r').read()
 
 
 setuptools.setup(
     name='ttcal',
     version=version,
     url='https://github.com/datakortet/ttcal',
     author='Bjorn Pettersen',
     author_email='bp@datakortet.no',
     requires=[],
     install_requires=[],
-    # description=__doc__.strip(),
+    description=__doc__.strip(),
     long_description=description,
     classifiers=[line for line in classifiers.split('\n') if line],
     packages=setuptools.find_packages(exclude=['tests']),
     zip_safe=False,
 )
```

### Comparing `ttcal-2.0.4/ttcal/__init__.py` & `ttcal-2.0.5/ttcal/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 Date classes (originally from TikTok).
 """
-__version__ = '2.0.4'
+__version__ = '2.0.5'
 from .day import Day, Days, Today   # noqa  
 from .duration import Duration, Period  # noqa
 from .calfns import chop, isoweek   # noqa
 from .month import Month
 from .week import Week
 from .year import Year
```

### Comparing `ttcal-2.0.4/ttcal/calfns.py` & `ttcal-2.0.5/ttcal/calfns.py`

 * *Files identical despite different names*

### Comparing `ttcal-2.0.4/ttcal/day.py` & `ttcal-2.0.5/ttcal/day.py`

 * *Files identical despite different names*

### Comparing `ttcal-2.0.4/ttcal/duration.py` & `ttcal-2.0.5/ttcal/duration.py`

 * *Files identical despite different names*

### Comparing `ttcal-2.0.4/ttcal/month.py` & `ttcal-2.0.5/ttcal/month.py`

 * *Files identical despite different names*

### Comparing `ttcal-2.0.4/ttcal/templatetags/ttcal_tags.py` & `ttcal-2.0.5/ttcal/templatetags/ttcal_tags.py`

 * *Files identical despite different names*

### Comparing `ttcal-2.0.4/ttcal/week.py` & `ttcal-2.0.5/ttcal/week.py`

 * *Files identical despite different names*

### Comparing `ttcal-2.0.4/ttcal/year.py` & `ttcal-2.0.5/ttcal/year.py`

 * *Files identical despite different names*

### Comparing `ttcal-2.0.4/ttcal.egg-info/PKG-INFO` & `ttcal-2.0.5/ttcal.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: ttcal
-Version: 2.0.4
-Summary: UNKNOWN
+Version: 2.0.5
+Summary: ttcal - calendar operations
 Home-page: https://github.com/datakortet/ttcal
 Author: Bjorn Pettersen
 Author-email: bp@datakortet.no
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

