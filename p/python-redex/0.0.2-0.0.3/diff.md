# Comparing `tmp/python_redex-0.0.2.tar.gz` & `tmp/python_redex-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_redex-0.0.2.tar", last modified: Sun Jul  2 15:58:59 2023, max compression
+gzip compressed data, was "python_redex-0.0.3.tar", last modified: Sun Jul  2 16:31:56 2023, max compression
```

## Comparing `python_redex-0.0.2.tar` & `python_redex-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-02 15:58:59.230078 python_redex-0.0.2/
--rw-rw-rw-   0        0        0     1064 2023-07-02 15:30:02.000000 python_redex-0.0.2/LICENCE.txt
--rw-rw-rw-   0        0        0       11 2023-07-02 15:28:52.000000 python_redex-0.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0      635 2023-07-02 15:58:59.229060 python_redex-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      116 2023-07-02 15:27:01.000000 python_redex-0.0.2/README.txt
-drwxrwxrwx   0        0        0        0 2023-07-02 15:58:59.226179 python_redex-0.0.2/python_redex.egg-info/
--rw-rw-rw-   0        0        0      635 2023-07-02 15:58:59.000000 python_redex-0.0.2/python_redex.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      205 2023-07-02 15:58:59.000000 python_redex-0.0.2/python_redex.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-02 15:58:59.000000 python_redex-0.0.2/python_redex.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-07-02 15:58:59.000000 python_redex-0.0.2/python_redex.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-02 15:58:59.227144 python_redex-0.0.2/redex/
--rw-rw-rw-   0        0        0     1440 2023-07-02 15:58:19.000000 python_redex-0.0.2/redex/__init__.py
--rw-rw-rw-   0        0        0       42 2023-07-02 15:58:59.230078 python_redex-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      793 2023-07-02 15:58:53.000000 python_redex-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-02 16:31:56.721902 python_redex-0.0.3/
+-rw-rw-rw-   0        0        0     1064 2023-07-02 15:30:02.000000 python_redex-0.0.3/LICENCE.txt
+-rw-rw-rw-   0        0        0       11 2023-07-02 15:28:52.000000 python_redex-0.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0      635 2023-07-02 16:31:56.719845 python_redex-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      116 2023-07-02 15:27:01.000000 python_redex-0.0.3/README.txt
+drwxrwxrwx   0        0        0        0 2023-07-02 16:31:56.714764 python_redex-0.0.3/python_redex.egg-info/
+-rw-rw-rw-   0        0        0      635 2023-07-02 16:31:56.000000 python_redex-0.0.3/python_redex.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      205 2023-07-02 16:31:56.000000 python_redex-0.0.3/python_redex.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-02 16:31:56.000000 python_redex-0.0.3/python_redex.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-07-02 16:31:56.000000 python_redex-0.0.3/python_redex.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-02 16:31:56.716862 python_redex-0.0.3/redex/
+-rw-rw-rw-   0        0        0     1428 2023-07-02 16:31:39.000000 python_redex-0.0.3/redex/__init__.py
+-rw-rw-rw-   0        0        0       42 2023-07-02 16:31:56.722860 python_redex-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      793 2023-07-02 16:31:04.000000 python_redex-0.0.3/setup.py
```

### Comparing `python_redex-0.0.2/LICENCE.txt` & `python_redex-0.0.3/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `python_redex-0.0.2/PKG-INFO` & `python_redex-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python_redex
-Version: 0.0.2
+Version: 0.0.3
 Summary: User friendly version of regex. More information available at https://github.com/TimoKats/redex
 Home-page: 
 Author: Timo Kats
 Author-email: tpakats@gmail.com
 License: MIT
 Keywords: regex
 Classifier: Development Status :: 4 - Beta
```

### Comparing `python_redex-0.0.2/python_redex.egg-info/PKG-INFO` & `python_redex-0.0.3/python_redex.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-redex
-Version: 0.0.2
+Version: 0.0.3
 Summary: User friendly version of regex. More information available at https://github.com/TimoKats/redex
 Home-page: 
 Author: Timo Kats
 Author-email: tpakats@gmail.com
 License: MIT
 Keywords: regex
 Classifier: Development Status :: 4 - Beta
```

### Comparing `python_redex-0.0.2/redex/__init__.py` & `python_redex-0.0.3/redex/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 __description__ = 'contains the basic functionalities of redex'
 __filename__ = '__init__.py'
 __author__ = 'Timo Kats'
 
 # local imports
 
-from redex.lib.lexical_analysis import *
-from redex.lib.split import *
+from lib.lexical_analysis import *
+from lib.split import *
 
 # main functionalities
 
 def has(query, string, split=' ', granularity=1, threads=2):
     search = RedexSearch(query, string, split=split, granularity=granularity, threads=threads)
     search.parse_query()
     if True in search.get_result():
@@ -29,10 +29,10 @@
         elif search.get_result()[index] and format == 'tuple':
             locations.append((index, location))
     return locations
 
 def info():
     print('\n---')
     print('    ^ ^          Description:        Python library for readable regex.')
-    print('("\(-_-)/")      Version:            0.0.2') 
+    print('("\(-_-)/")      Version:            0.0.3') 
     print(' )(  O  )(       Author:             Timo Kats')
     print('((...)(...))     Last updated:       02/07/2023', end='\n---\n\n')
```

### Comparing `python_redex-0.0.2/setup.py` & `python_redex-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     'License :: OSI Approved :: MIT License',
     'Operating System :: Microsoft :: Windows',
     'Programming Language :: Python :: 3'
 ]
 
 setup(
     name='python_redex',
-    version='0.0.2',
+    version='0.0.3',
     description='User friendly version of regex. More information available at https://github.com/TimoKats/redex',
     long_description='More information available at https://github.com/TimoKats/redex',
     url='',  
     author='Timo Kats',
     author_email='tpakats@gmail.com',
     license='MIT', 
     classifiers=classifiers,
```

