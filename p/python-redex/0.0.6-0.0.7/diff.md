# Comparing `tmp/python_redex-0.0.6.tar.gz` & `tmp/python_redex-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_redex-0.0.6.tar", last modified: Sun Jul  2 16:47:20 2023, max compression
+gzip compressed data, was "python_redex-0.0.7.tar", last modified: Sun Jul  2 17:33:23 2023, max compression
```

## Comparing `python_redex-0.0.6.tar` & `python_redex-0.0.7.tar`

### file list

```diff
@@ -1,24 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-02 16:47:20.987508 python_redex-0.0.6/
--rw-rw-rw-   0        0        0      461 2023-07-02 16:46:04.000000 python_redex-0.0.6/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1064 2023-07-02 15:30:02.000000 python_redex-0.0.6/LICENCE.txt
--rw-rw-rw-   0        0        0       27 2023-07-02 16:36:53.000000 python_redex-0.0.6/MANIFEST.in
--rw-rw-rw-   0        0        0      635 2023-07-02 16:47:20.986401 python_redex-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0      116 2023-07-02 15:27:01.000000 python_redex-0.0.6/README.txt
-drwxrwxrwx   0        0        0        0 2023-07-02 16:47:20.954658 python_redex-0.0.6/python_redex.egg-info/
--rw-rw-rw-   0        0        0      635 2023-07-02 16:47:20.000000 python_redex-0.0.6/python_redex.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      403 2023-07-02 16:47:20.000000 python_redex-0.0.6/python_redex.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-02 16:47:20.000000 python_redex-0.0.6/python_redex.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-07-02 16:47:20.000000 python_redex-0.0.6/python_redex.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-02 16:47:20.968860 python_redex-0.0.6/redex/
--rw-rw-rw-   0        0        0     1428 2023-07-02 16:45:41.000000 python_redex-0.0.6/redex/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-02 16:47:20.983930 python_redex-0.0.6/redex/lib/
--rw-rw-rw-   0        0        0     2445 2023-07-02 16:43:01.000000 python_redex-0.0.6/redex/lib/action.py
--rw-rw-rw-   0        0        0     2203 2023-07-02 16:43:10.000000 python_redex-0.0.6/redex/lib/lexical_analysis.py
--rw-rw-rw-   0        0        0      581 2023-07-02 15:01:38.000000 python_redex-0.0.6/redex/lib/split.py
--rw-rw-rw-   0        0        0      559 2023-07-02 15:02:16.000000 python_redex-0.0.6/redex/lib/wildcards.py
-drwxrwxrwx   0        0        0        0 2023-07-02 16:47:20.975082 python_redex-0.0.6/redex.egg-info/
--rw-rw-rw-   0        0        0      177 2023-07-02 15:53:02.000000 python_redex-0.0.6/redex.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-02 15:53:02.000000 python_redex-0.0.6/redex.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-07-02 15:53:02.000000 python_redex-0.0.6/redex.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-02 16:47:20.987508 python_redex-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      793 2023-07-02 16:45:34.000000 python_redex-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-02 17:33:23.056410 python_redex-0.0.7/
+-rw-rw-rw-   0        0        0      536 2023-07-02 17:33:13.000000 python_redex-0.0.7/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1064 2023-07-02 15:30:02.000000 python_redex-0.0.7/LICENCE.txt
+-rw-rw-rw-   0        0        0       27 2023-07-02 16:36:53.000000 python_redex-0.0.7/MANIFEST.in
+-rw-rw-rw-   0        0        0      635 2023-07-02 17:33:23.055407 python_redex-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0      116 2023-07-02 15:27:01.000000 python_redex-0.0.7/README.txt
+drwxrwxrwx   0        0        0        0 2023-07-02 17:33:23.010259 python_redex-0.0.7/python_redex.egg-info/
+-rw-rw-rw-   0        0        0      635 2023-07-02 17:33:22.000000 python_redex-0.0.7/python_redex.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      387 2023-07-02 17:33:22.000000 python_redex-0.0.7/python_redex.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-02 17:33:22.000000 python_redex-0.0.7/python_redex.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-07-02 17:33:22.000000 python_redex-0.0.7/python_redex.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-02 17:33:23.045252 python_redex-0.0.7/redex/
+-rw-rw-rw-   0        0        0     1432 2023-07-02 17:32:49.000000 python_redex-0.0.7/redex/__init__.py
+-rw-rw-rw-   0        0        0     2447 2023-07-02 17:32:27.000000 python_redex-0.0.7/redex/action.py
+-rw-rw-rw-   0        0        0     2207 2023-07-02 17:32:37.000000 python_redex-0.0.7/redex/lexical_analysis.py
+-rw-rw-rw-   0        0        0      581 2023-07-02 15:01:38.000000 python_redex-0.0.7/redex/split.py
+-rw-rw-rw-   0        0        0      559 2023-07-02 15:02:16.000000 python_redex-0.0.7/redex/wildcards.py
+drwxrwxrwx   0        0        0        0 2023-07-02 17:33:23.053408 python_redex-0.0.7/redex.egg-info/
+-rw-rw-rw-   0        0        0      177 2023-07-02 15:53:02.000000 python_redex-0.0.7/redex.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-02 15:53:02.000000 python_redex-0.0.7/redex.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-07-02 15:53:02.000000 python_redex-0.0.7/redex.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-02 17:33:23.056410 python_redex-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      787 2023-07-02 17:32:57.000000 python_redex-0.0.7/setup.py
```

### Comparing `python_redex-0.0.6/LICENCE.txt` & `python_redex-0.0.7/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `python_redex-0.0.6/PKG-INFO` & `python_redex-0.0.7/python_redex.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: python_redex
-Version: 0.0.6
+Name: python-redex
+Version: 0.0.7
 Summary: User friendly version of regex. More information available at https://github.com/TimoKats/redex
 Home-page: 
 Author: Timo Kats
 Author-email: tpakats@gmail.com
 License: MIT
 Keywords: regex
 Classifier: Development Status :: 4 - Beta
```

### Comparing `python_redex-0.0.6/python_redex.egg-info/PKG-INFO` & `python_redex-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: python-redex
-Version: 0.0.6
+Name: python_redex
+Version: 0.0.7
 Summary: User friendly version of regex. More information available at https://github.com/TimoKats/redex
 Home-page: 
 Author: Timo Kats
 Author-email: tpakats@gmail.com
 License: MIT
 Keywords: regex
 Classifier: Development Status :: 4 - Beta
```

### Comparing `python_redex-0.0.6/redex/__init__.py` & `python_redex-0.0.7/redex/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 __description__ = 'contains the basic functionalities of redex'
 __filename__ = '__init__.py'
 __author__ = 'Timo Kats'
 
 # local imports
 
-from lib.lexical_analysis import *
-from lib.split import *
+from redex.lexical_analysis import *
+from redex.split import *
 
 # main functionalities
 
 def has(query, string, split=' ', granularity=1, threads=2):
     search = RedexSearch(query, string, split=split, granularity=granularity, threads=threads)
     search.parse_query()
     if True in search.get_result():
```

### Comparing `python_redex-0.0.6/redex/lib/action.py` & `python_redex-0.0.7/redex/action.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 __description__ = 'contains the actions that user can call in redex'
 __filename__ = 'action.py'
 __author__ = 'Timo Kats'
 
 # local imports
 
-from lib.wildcards import *
+from redex.wildcards import *
 
 # helper functions
 
 def is_in(char, string):
     if char in wildcard.keys():
         for wchar in wildcard[char]:
             if wchar in string:
```

### Comparing `python_redex-0.0.6/redex/lib/lexical_analysis.py` & `python_redex-0.0.7/redex/lexical_analysis.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 # libraries
 
 from multiprocessing import Pool
 from itertools import repeat
 
 # local imports
 
-from lib.action import *
-from lib.split import *
+from redex.action import *
+from redex.split import *
 
 class RedexSearch:
     def __init__(self, query, string, split, granularity, threads=2):
         self.subqueries = self.extract_subqueries(query)
         self.query = query
         self.string = string
         self.split = split
```

### Comparing `python_redex-0.0.6/redex/lib/split.py` & `python_redex-0.0.7/redex/split.py`

 * *Files identical despite different names*

### Comparing `python_redex-0.0.6/redex/lib/wildcards.py` & `python_redex-0.0.7/redex/wildcards.py`

 * *Files identical despite different names*

### Comparing `python_redex-0.0.6/setup.py` & `python_redex-0.0.7/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,19 +7,19 @@
     'License :: OSI Approved :: MIT License',
     'Operating System :: Microsoft :: Windows',
     'Programming Language :: Python :: 3'
 ]
 
 setup(
     name='python_redex',
-    version='0.0.6',
+    version='0.0.7',
     description='User friendly version of regex. More information available at https://github.com/TimoKats/redex',
     long_description='More information available at https://github.com/TimoKats/redex',
     url='',  
     author='Timo Kats',
     author_email='tpakats@gmail.com',
     license='MIT', 
     classifiers=classifiers,
     keywords='regex', 
-    packages=find_packages(),
+    packages=['redex'],
     install_requires=[''] 
 )
```

