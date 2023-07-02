# Comparing `tmp/python-yapi-0.1.tar.gz` & `tmp/python-yapi-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/python-yapi-0.1.tar", last modified: Fri Oct 15 04:59:12 2021, max compression
+gzip compressed data, was "python-yapi-0.1.1.tar", last modified: Sun Jul  2 08:54:50 2023, max compression
```

## Comparing `python-yapi-0.1.tar` & `python-yapi-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,25 @@
-drwxr-xr-x   0 superhin   (501) staff       (20)        0 2021-10-15 04:59:12.004524 python-yapi-0.1/
--rw-r--r--   0 superhin   (501) staff       (20)     1068 2021-10-15 03:48:34.000000 python-yapi-0.1/LICENSE
--rw-r--r--   0 superhin   (501) staff       (20)      137 2021-10-15 03:48:34.000000 python-yapi-0.1/MANIFEST.in
--rw-r--r--   0 superhin   (501) staff       (20)      497 2021-10-15 04:59:12.004238 python-yapi-0.1/PKG-INFO
--rw-r--r--   0 superhin   (501) staff       (20)       34 2021-10-15 04:57:17.000000 python-yapi-0.1/README.md
-drwxr-xr-x   0 superhin   (501) staff       (20)        0 2021-10-15 04:59:12.003889 python-yapi-0.1/python_yapi.egg-info/
--rw-r--r--   0 superhin   (501) staff       (20)      497 2021-10-15 04:59:11.000000 python-yapi-0.1/python_yapi.egg-info/PKG-INFO
--rw-r--r--   0 superhin   (501) staff       (20)      208 2021-10-15 04:59:11.000000 python-yapi-0.1/python_yapi.egg-info/SOURCES.txt
--rw-r--r--   0 superhin   (501) staff       (20)        1 2021-10-15 04:59:11.000000 python-yapi-0.1/python_yapi.egg-info/dependency_links.txt
--rw-r--r--   0 superhin   (501) staff       (20)        1 2021-10-15 04:59:11.000000 python-yapi-0.1/python_yapi.egg-info/top_level.txt
--rw-r--r--   0 superhin   (501) staff       (20)        1 2021-10-15 04:59:11.000000 python-yapi-0.1/python_yapi.egg-info/zip-safe
--rw-r--r--   0 superhin   (501) staff       (20)       38 2021-10-15 04:59:12.004622 python-yapi-0.1/setup.cfg
--rw-r--r--   0 superhin   (501) staff       (20)     1113 2021-10-15 04:58:03.000000 python-yapi-0.1/setup.py
+drwxr-xr-x   0 superhin   (502) staff       (20)        0 2023-07-02 08:54:50.402688 python-yapi-0.1.1/
+-rw-r--r--   0 superhin   (502) staff       (20)      153 2023-06-28 07:02:56.000000 python-yapi-0.1.1/AUTHORS.rst
+-rw-r--r--   0 superhin   (502) staff       (20)     3562 2023-06-28 08:12:06.000000 python-yapi-0.1.1/CONTRIBUTING.rst
+-rw-r--r--   0 superhin   (502) staff       (20)       89 2023-06-28 07:02:56.000000 python-yapi-0.1.1/HISTORY.rst
+-rw-r--r--   0 superhin   (502) staff       (20)     1068 2023-06-10 12:41:28.000000 python-yapi-0.1.1/LICENSE
+-rw-r--r--   0 superhin   (502) staff       (20)      137 2023-06-10 12:41:28.000000 python-yapi-0.1.1/MANIFEST.in
+-rw-r--r--   0 superhin   (502) staff       (20)     1476 2023-07-02 08:54:50.402862 python-yapi-0.1.1/PKG-INFO
+-rw-r--r--   0 superhin   (502) staff       (20)     1005 2023-07-02 08:53:16.000000 python-yapi-0.1.1/README.md
+-rw-r--r--   0 superhin   (502) staff       (20)     2761 2023-06-28 06:53:34.000000 python-yapi-0.1.1/README.rst
+drwxr-xr-x   0 superhin   (502) staff       (20)        0 2023-07-02 08:54:50.398560 python-yapi-0.1.1/python_yapi.egg-info/
+-rw-r--r--   0 superhin   (502) staff       (20)     1476 2023-07-02 08:54:50.000000 python-yapi-0.1.1/python_yapi.egg-info/PKG-INFO
+-rw-r--r--   0 superhin   (502) staff       (20)      399 2023-07-02 08:54:50.000000 python-yapi-0.1.1/python_yapi.egg-info/SOURCES.txt
+-rw-r--r--   0 superhin   (502) staff       (20)        1 2023-07-02 08:54:50.000000 python-yapi-0.1.1/python_yapi.egg-info/dependency_links.txt
+-rw-r--r--   0 superhin   (502) staff       (20)        1 2023-07-02 08:54:50.000000 python-yapi-0.1.1/python_yapi.egg-info/top_level.txt
+-rw-r--r--   0 superhin   (502) staff       (20)        1 2023-06-10 12:41:40.000000 python-yapi-0.1.1/python_yapi.egg-info/zip-safe
+-rw-r--r--   0 superhin   (502) staff       (20)      216 2023-06-30 11:38:00.000000 python-yapi-0.1.1/requirements_dev.txt
+-rw-r--r--   0 superhin   (502) staff       (20)       24 2023-06-30 10:48:01.000000 python-yapi-0.1.1/requirments.txt
+-rw-r--r--   0 superhin   (502) staff       (20)      428 2023-07-02 08:54:50.403497 python-yapi-0.1.1/setup.cfg
+-rw-r--r--   0 superhin   (502) staff       (20)     1183 2023-07-02 08:54:37.000000 python-yapi-0.1.1/setup.py
+drwxr-xr-x   0 superhin   (502) staff       (20)        0 2023-07-02 08:54:50.401959 python-yapi-0.1.1/tests/
+-rw-r--r--   0 superhin   (502) staff       (20)        0 2023-06-10 13:10:56.000000 python-yapi-0.1.1/tests/test_base_api.py
+-rw-r--r--   0 superhin   (502) staff       (20)      491 2023-06-30 11:59:56.000000 python-yapi-0.1.1/tests/test_group.py
+-rw-r--r--   0 superhin   (502) staff       (20)     2650 2023-06-30 12:49:41.000000 python-yapi-0.1.1/tests/test_project.py
+-rw-r--r--   0 superhin   (502) staff       (20)      275 2023-06-30 09:09:18.000000 python-yapi-0.1.1/tests/test_user.py
+-rw-r--r--   0 superhin   (502) staff       (20)      542 2023-06-28 07:02:56.000000 python-yapi-0.1.1/tox.ini
```

### Comparing `python-yapi-0.1/LICENSE` & `python-yapi-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `python-yapi-0.1/setup.py` & `python-yapi-0.1.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 """The setup script."""
 import os
 from setuptools import setup, find_packages
 
-this_directory = os.path.abspath(os.path.dirname(__file__))
-setup_requirements = []
+version = '0.1.1'
 
+this_directory = os.path.abspath(os.path.dirname(__file__))
+setup_requirements = ['requests',
+                      'python-slugify']
 
 def read_file(filename):
     with open(os.path.join(this_directory, filename), encoding='utf-8') as f:
         long_description = f.read()
     return long_description
 
 
@@ -30,11 +32,11 @@
     keywords=[
         'yapi', 'python-yapi', 'pyyapi',
     ],
     name='python-yapi',
     packages=find_packages(include=['python-yapi']),
     setup_requires=setup_requirements,
     url='https://github.com/hanzhichao/python-yapi',
-    version='0.1',
+    version=version,
     zip_safe=True,
     install_requires=[]
 )
```

