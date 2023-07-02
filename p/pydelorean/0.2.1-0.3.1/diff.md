# Comparing `tmp/pydelorean-0.2.1.tar.gz` & `tmp/pydelorean-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydelorean-0.2.1.tar", last modified: Tue Jun 20 23:53:29 2023, max compression
+gzip compressed data, was "pydelorean-0.3.1.tar", last modified: Sun Jul  2 15:28:56 2023, max compression
```

## Comparing `pydelorean-0.2.1.tar` & `pydelorean-0.3.1.tar`

### file list

```diff
@@ -1,23 +1,25 @@
-drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-06-20 23:53:29.511133 pydelorean-0.2.1/
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)    11358 2023-05-11 12:19:37.000000 pydelorean-0.2.1/LICENSE
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     2551 2023-06-20 23:53:29.511133 pydelorean-0.2.1/PKG-INFO
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     2108 2023-06-12 11:33:27.000000 pydelorean-0.2.1/README.rst
-drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-06-20 23:53:29.511133 pydelorean-0.2.1/pydelorean/
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     1974 2023-06-20 23:44:32.000000 pydelorean-0.2.1/pydelorean/__init__.py
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     3903 2023-06-20 23:53:14.000000 pydelorean-0.2.1/pydelorean/delorean.py
-drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-06-20 23:53:29.511133 pydelorean-0.2.1/pydelorean/parser/
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)       22 2023-06-12 11:33:27.000000 pydelorean-0.2.1/pydelorean/parser/__init__.py
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     1311 2023-06-12 11:33:27.000000 pydelorean-0.2.1/pydelorean/parser/parser.py
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     4865 2023-06-12 11:40:12.000000 pydelorean-0.2.1/pydelorean/parser/utils.py
-drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-06-20 23:53:29.511133 pydelorean-0.2.1/pydelorean/tree/
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)       21 2023-06-12 11:33:27.000000 pydelorean-0.2.1/pydelorean/tree/__init__.py
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     2789 2023-06-12 11:33:27.000000 pydelorean-0.2.1/pydelorean/tree/types.py
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)      245 2023-06-12 11:33:27.000000 pydelorean-0.2.1/pydelorean/utils.py
-drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-06-20 23:53:29.511133 pydelorean-0.2.1/pydelorean.egg-info/
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     2551 2023-06-20 23:53:29.000000 pydelorean-0.2.1/pydelorean.egg-info/PKG-INFO
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)      400 2023-06-20 23:53:29.000000 pydelorean-0.2.1/pydelorean.egg-info/SOURCES.txt
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)        1 2023-06-20 23:53:29.000000 pydelorean-0.2.1/pydelorean.egg-info/dependency_links.txt
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)       43 2023-06-20 23:53:29.000000 pydelorean-0.2.1/pydelorean.egg-info/requires.txt
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)       11 2023-06-20 23:53:29.000000 pydelorean-0.2.1/pydelorean.egg-info/top_level.txt
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)       38 2023-06-20 23:53:29.511133 pydelorean-0.2.1/setup.cfg
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)      962 2023-06-20 23:46:05.000000 pydelorean-0.2.1/setup.py
+drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-07-02 15:28:56.380357 pydelorean-0.3.1/
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)    11358 2023-06-10 12:13:51.000000 pydelorean-0.3.1/LICENSE
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     2532 2023-07-02 15:28:56.380357 pydelorean-0.3.1/PKG-INFO
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     2108 2023-06-11 13:16:27.000000 pydelorean-0.3.1/README.rst
+drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-07-02 15:28:56.378357 pydelorean-0.3.1/pydelorean/
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     1974 2023-06-14 12:58:48.000000 pydelorean-0.3.1/pydelorean/__init__.py
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     3903 2023-07-02 13:53:53.000000 pydelorean-0.3.1/pydelorean/delorean.py
+drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-07-02 15:28:56.379357 pydelorean-0.3.1/pydelorean/parser/
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)       22 2023-06-10 12:14:10.000000 pydelorean-0.3.1/pydelorean/parser/__init__.py
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     1311 2023-06-14 12:58:48.000000 pydelorean-0.3.1/pydelorean/parser/parser.py
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     4865 2023-07-02 13:55:11.000000 pydelorean-0.3.1/pydelorean/parser/utils.py
+drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-07-02 15:28:56.380357 pydelorean-0.3.1/pydelorean/tree/
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)       21 2023-06-10 12:13:51.000000 pydelorean-0.3.1/pydelorean/tree/__init__.py
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     2789 2023-06-10 16:47:52.000000 pydelorean-0.3.1/pydelorean/tree/types.py
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)      245 2023-06-14 12:58:48.000000 pydelorean-0.3.1/pydelorean/utils.py
+drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-07-02 15:28:56.379357 pydelorean-0.3.1/pydelorean.egg-info/
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     2532 2023-07-02 15:28:56.000000 pydelorean-0.3.1/pydelorean.egg-info/PKG-INFO
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)      421 2023-07-02 15:28:56.000000 pydelorean-0.3.1/pydelorean.egg-info/SOURCES.txt
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)        1 2023-07-02 15:28:56.000000 pydelorean-0.3.1/pydelorean.egg-info/dependency_links.txt
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)       32 2023-07-02 15:28:56.000000 pydelorean-0.3.1/pydelorean.egg-info/requires.txt
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)       11 2023-07-02 15:28:56.000000 pydelorean-0.3.1/pydelorean.egg-info/top_level.txt
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)       38 2023-07-02 15:28:56.380357 pydelorean-0.3.1/setup.cfg
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)      951 2023-07-02 15:28:29.000000 pydelorean-0.3.1/setup.py
+drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-07-02 15:28:56.380357 pydelorean-0.3.1/tests/
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     1198 2023-06-11 13:13:52.000000 pydelorean-0.3.1/tests/test_mdtree.py
```

### Comparing `pydelorean-0.2.1/LICENSE` & `pydelorean-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pydelorean-0.2.1/PKG-INFO` & `pydelorean-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: pydelorean
-Version: 0.2.1
+Version: 0.3.1
 Summary: A package to convert between markup language documents and a forest data structure for efficient processing.
 Home-page: http://github.com/kj3moraes/delorean
+Download-URL: https://github.com/kj3moraes/delorean/archive/0.3.1.zip
 Author: Keane Moraes
 Author-email: lordvader3002@gmail.com
 License: Apache 2.0
-Download-URL: https://github.com/kj3moraes/delorean/archive/0.2.1.zip
-Platform: UNKNOWN
 Classifier: Topic :: Utilities
 License-File: LICENSE
 
 .. image:: media/image.png
    :width: 200
 
 delorean
@@ -102,8 +101,7 @@
 3. Traverse and edit the Python data structure.
 
 License
 -------
 
 This project is licensed under the Apache 2.0 License. A copy of the license 
 can be found in the LICENSE file.
-
```

### Comparing `pydelorean-0.2.1/README.rst` & `pydelorean-0.3.1/README.rst`

 * *Files identical despite different names*

### Comparing `pydelorean-0.2.1/pydelorean/__init__.py` & `pydelorean-0.3.1/pydelorean/__init__.py`

 * *Files identical despite different names*

### Comparing `pydelorean-0.2.1/pydelorean/delorean.py` & `pydelorean-0.3.1/pydelorean/delorean.py`

 * *Files identical despite different names*

### Comparing `pydelorean-0.2.1/pydelorean/parser/parser.py` & `pydelorean-0.3.1/pydelorean/parser/parser.py`

 * *Files identical despite different names*

### Comparing `pydelorean-0.2.1/pydelorean/parser/utils.py` & `pydelorean-0.3.1/pydelorean/parser/utils.py`

 * *Files identical despite different names*

### Comparing `pydelorean-0.2.1/pydelorean/tree/types.py` & `pydelorean-0.3.1/pydelorean/tree/types.py`

 * *Files identical despite different names*

### Comparing `pydelorean-0.2.1/pydelorean.egg-info/PKG-INFO` & `pydelorean-0.3.1/pydelorean.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: pydelorean
-Version: 0.2.1
+Version: 0.3.1
 Summary: A package to convert between markup language documents and a forest data structure for efficient processing.
 Home-page: http://github.com/kj3moraes/delorean
+Download-URL: https://github.com/kj3moraes/delorean/archive/0.3.1.zip
 Author: Keane Moraes
 Author-email: lordvader3002@gmail.com
 License: Apache 2.0
-Download-URL: https://github.com/kj3moraes/delorean/archive/0.2.1.zip
-Platform: UNKNOWN
 Classifier: Topic :: Utilities
 License-File: LICENSE
 
 .. image:: media/image.png
    :width: 200
 
 delorean
@@ -102,8 +101,7 @@
 3. Traverse and edit the Python data structure.
 
 License
 -------
 
 This project is licensed under the Apache 2.0 License. A copy of the license 
 can be found in the LICENSE file.
-
```

### Comparing `pydelorean-0.2.1/setup.py` & `pydelorean-0.3.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from setuptools import setup
 from setuptools.command.test import test as TestCommand
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 LONG_DESCRIPTION = (this_directory / "README.rst").read_text()
 
-VERSION = '0.2.1'
+VERSION = '0.3.1'
 DESCRIPTION = 'A package to convert between markup language documents and a forest data structure for efficient processing.'
 
 setup(
     name = "pydelorean",
     version = VERSION,
     author = "Keane Moraes",
     author_email = 'lordvader3002@gmail.com',
     description = DESCRIPTION,
     long_description=LONG_DESCRIPTION,
     license = "Apache 2.0",
     url = "http://github.com/kj3moraes/delorean",
     packages = ['pydelorean', 'pydelorean.tree', 'pydelorean.parser'],
     tests_require = ['unittest'],
-    install_requires = ['markdown', 'beautifulsoup4', 'python-frontmatter'],
+    install_requires = ['markdown', 'treelib', 'beautifulsoup4'],
     download_url = 'https://github.com/kj3moraes/delorean/archive/%s.zip' % VERSION,
     classifiers = [
         "Topic :: Utilities",
     ],
 )
```

