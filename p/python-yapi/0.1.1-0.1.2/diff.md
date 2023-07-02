# Comparing `tmp/python-yapi-0.1.1.tar.gz` & `tmp/python_yapi-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-yapi-0.1.1.tar", last modified: Sun Jul  2 08:54:50 2023, max compression
+gzip compressed data, was "python_yapi-0.1.2.tar", last modified: Sun Jul  2 09:17:45 2023, max compression
```

## Comparing `python-yapi-0.1.1.tar` & `python_yapi-0.1.2.tar`

### file list

```diff
@@ -1,25 +1,41 @@
-drwxr-xr-x   0 superhin   (502) staff       (20)        0 2023-07-02 08:54:50.402688 python-yapi-0.1.1/
--rw-r--r--   0 superhin   (502) staff       (20)      153 2023-06-28 07:02:56.000000 python-yapi-0.1.1/AUTHORS.rst
--rw-r--r--   0 superhin   (502) staff       (20)     3562 2023-06-28 08:12:06.000000 python-yapi-0.1.1/CONTRIBUTING.rst
--rw-r--r--   0 superhin   (502) staff       (20)       89 2023-06-28 07:02:56.000000 python-yapi-0.1.1/HISTORY.rst
--rw-r--r--   0 superhin   (502) staff       (20)     1068 2023-06-10 12:41:28.000000 python-yapi-0.1.1/LICENSE
--rw-r--r--   0 superhin   (502) staff       (20)      137 2023-06-10 12:41:28.000000 python-yapi-0.1.1/MANIFEST.in
--rw-r--r--   0 superhin   (502) staff       (20)     1476 2023-07-02 08:54:50.402862 python-yapi-0.1.1/PKG-INFO
--rw-r--r--   0 superhin   (502) staff       (20)     1005 2023-07-02 08:53:16.000000 python-yapi-0.1.1/README.md
--rw-r--r--   0 superhin   (502) staff       (20)     2761 2023-06-28 06:53:34.000000 python-yapi-0.1.1/README.rst
-drwxr-xr-x   0 superhin   (502) staff       (20)        0 2023-07-02 08:54:50.398560 python-yapi-0.1.1/python_yapi.egg-info/
--rw-r--r--   0 superhin   (502) staff       (20)     1476 2023-07-02 08:54:50.000000 python-yapi-0.1.1/python_yapi.egg-info/PKG-INFO
--rw-r--r--   0 superhin   (502) staff       (20)      399 2023-07-02 08:54:50.000000 python-yapi-0.1.1/python_yapi.egg-info/SOURCES.txt
--rw-r--r--   0 superhin   (502) staff       (20)        1 2023-07-02 08:54:50.000000 python-yapi-0.1.1/python_yapi.egg-info/dependency_links.txt
--rw-r--r--   0 superhin   (502) staff       (20)        1 2023-07-02 08:54:50.000000 python-yapi-0.1.1/python_yapi.egg-info/top_level.txt
--rw-r--r--   0 superhin   (502) staff       (20)        1 2023-06-10 12:41:40.000000 python-yapi-0.1.1/python_yapi.egg-info/zip-safe
--rw-r--r--   0 superhin   (502) staff       (20)      216 2023-06-30 11:38:00.000000 python-yapi-0.1.1/requirements_dev.txt
--rw-r--r--   0 superhin   (502) staff       (20)       24 2023-06-30 10:48:01.000000 python-yapi-0.1.1/requirments.txt
--rw-r--r--   0 superhin   (502) staff       (20)      428 2023-07-02 08:54:50.403497 python-yapi-0.1.1/setup.cfg
--rw-r--r--   0 superhin   (502) staff       (20)     1183 2023-07-02 08:54:37.000000 python-yapi-0.1.1/setup.py
-drwxr-xr-x   0 superhin   (502) staff       (20)        0 2023-07-02 08:54:50.401959 python-yapi-0.1.1/tests/
--rw-r--r--   0 superhin   (502) staff       (20)        0 2023-06-10 13:10:56.000000 python-yapi-0.1.1/tests/test_base_api.py
--rw-r--r--   0 superhin   (502) staff       (20)      491 2023-06-30 11:59:56.000000 python-yapi-0.1.1/tests/test_group.py
--rw-r--r--   0 superhin   (502) staff       (20)     2650 2023-06-30 12:49:41.000000 python-yapi-0.1.1/tests/test_project.py
--rw-r--r--   0 superhin   (502) staff       (20)      275 2023-06-30 09:09:18.000000 python-yapi-0.1.1/tests/test_user.py
--rw-r--r--   0 superhin   (502) staff       (20)      542 2023-06-28 07:02:56.000000 python-yapi-0.1.1/tox.ini
+drwxr-xr-x   0 superhin   (502) staff       (20)        0 2023-07-02 09:17:45.784664 python_yapi-0.1.2/
+-rw-r--r--   0 superhin   (502) staff       (20)      153 2023-06-28 07:02:56.000000 python_yapi-0.1.2/AUTHORS.rst
+-rw-r--r--   0 superhin   (502) staff       (20)     3562 2023-06-28 08:12:06.000000 python_yapi-0.1.2/CONTRIBUTING.rst
+-rw-r--r--   0 superhin   (502) staff       (20)       89 2023-06-28 07:02:56.000000 python_yapi-0.1.2/HISTORY.rst
+-rw-r--r--   0 superhin   (502) staff       (20)     1068 2023-06-10 12:41:28.000000 python_yapi-0.1.2/LICENSE
+-rw-r--r--   0 superhin   (502) staff       (20)      137 2023-06-10 12:41:28.000000 python_yapi-0.1.2/MANIFEST.in
+-rw-r--r--   0 superhin   (502) staff       (20)     1476 2023-07-02 09:17:45.784906 python_yapi-0.1.2/PKG-INFO
+-rw-r--r--   0 superhin   (502) staff       (20)     1005 2023-07-02 08:53:16.000000 python_yapi-0.1.2/README.md
+-rw-r--r--   0 superhin   (502) staff       (20)     2761 2023-06-28 06:53:34.000000 python_yapi-0.1.2/README.rst
+drwxr-xr-x   0 superhin   (502) staff       (20)        0 2023-07-02 09:17:45.773514 python_yapi-0.1.2/python_yapi/
+-rw-r--r--   0 superhin   (502) staff       (20)       42 2023-06-28 03:57:06.000000 python_yapi-0.1.2/python_yapi/__init__.py
+-rw-r--r--   0 superhin   (502) staff       (20)     3546 2023-06-30 12:47:33.000000 python_yapi-0.1.2/python_yapi/base.py
+-rw-r--r--   0 superhin   (502) staff       (20)      448 2023-06-28 07:02:56.000000 python_yapi-0.1.2/python_yapi/cli.py
+-rw-r--r--   0 superhin   (502) staff       (20)      295 2023-06-28 03:56:07.000000 python_yapi-0.1.2/python_yapi/collection.py
+-rw-r--r--   0 superhin   (502) staff       (20)      202 2023-06-30 11:36:46.000000 python_yapi-0.1.2/python_yapi/constants.py
+-rw-r--r--   0 superhin   (502) staff       (20)      347 2023-06-30 12:24:32.000000 python_yapi-0.1.2/python_yapi/exceptions.py
+-rw-r--r--   0 superhin   (502) staff       (20)      336 2023-06-28 09:01:36.000000 python_yapi-0.1.2/python_yapi/follow.py
+-rw-r--r--   0 superhin   (502) staff       (20)     1361 2023-06-30 11:59:22.000000 python_yapi-0.1.2/python_yapi/group.py
+-rw-r--r--   0 superhin   (502) staff       (20)     2224 2023-07-02 08:54:14.000000 python_yapi-0.1.2/python_yapi/interface.py
+-rw-r--r--   0 superhin   (502) staff       (20)      307 2023-06-28 08:57:31.000000 python_yapi-0.1.2/python_yapi/log.py
+-rw-r--r--   0 superhin   (502) staff       (20)     1286 2023-06-28 09:45:42.000000 python_yapi-0.1.2/python_yapi/models.py
+-rw-r--r--   0 superhin   (502) staff       (20)    14308 2023-06-30 13:00:29.000000 python_yapi-0.1.2/python_yapi/project.py
+-rw-r--r--   0 superhin   (502) staff       (20)     3409 2023-06-30 12:51:34.000000 python_yapi-0.1.2/python_yapi/user.py
+-rw-r--r--   0 superhin   (502) staff       (20)      993 2023-06-28 04:36:56.000000 python_yapi-0.1.2/python_yapi/utils.py
+-rw-r--r--   0 superhin   (502) staff       (20)      260 2023-06-30 09:01:05.000000 python_yapi-0.1.2/python_yapi/yapi.py
+drwxr-xr-x   0 superhin   (502) staff       (20)        0 2023-07-02 09:17:45.778959 python_yapi-0.1.2/python_yapi.egg-info/
+-rw-r--r--   0 superhin   (502) staff       (20)     1476 2023-07-02 09:17:45.000000 python_yapi-0.1.2/python_yapi.egg-info/PKG-INFO
+-rw-r--r--   0 superhin   (502) staff       (20)      732 2023-07-02 09:17:45.000000 python_yapi-0.1.2/python_yapi.egg-info/SOURCES.txt
+-rw-r--r--   0 superhin   (502) staff       (20)        1 2023-07-02 09:17:45.000000 python_yapi-0.1.2/python_yapi.egg-info/dependency_links.txt
+-rw-r--r--   0 superhin   (502) staff       (20)       12 2023-07-02 09:17:45.000000 python_yapi-0.1.2/python_yapi.egg-info/top_level.txt
+-rw-r--r--   0 superhin   (502) staff       (20)        1 2023-06-10 12:41:40.000000 python_yapi-0.1.2/python_yapi.egg-info/zip-safe
+-rw-r--r--   0 superhin   (502) staff       (20)      216 2023-06-30 11:38:00.000000 python_yapi-0.1.2/requirements_dev.txt
+-rw-r--r--   0 superhin   (502) staff       (20)       24 2023-06-30 10:48:01.000000 python_yapi-0.1.2/requirments.txt
+-rw-r--r--   0 superhin   (502) staff       (20)      428 2023-07-02 09:17:45.785935 python_yapi-0.1.2/setup.cfg
+-rw-r--r--   0 superhin   (502) staff       (20)     1183 2023-07-02 09:17:36.000000 python_yapi-0.1.2/setup.py
+drwxr-xr-x   0 superhin   (502) staff       (20)        0 2023-07-02 09:17:45.783845 python_yapi-0.1.2/tests/
+-rw-r--r--   0 superhin   (502) staff       (20)        0 2023-06-10 13:10:56.000000 python_yapi-0.1.2/tests/test_base_api.py
+-rw-r--r--   0 superhin   (502) staff       (20)      491 2023-06-30 11:59:56.000000 python_yapi-0.1.2/tests/test_group.py
+-rw-r--r--   0 superhin   (502) staff       (20)     2650 2023-06-30 12:49:41.000000 python_yapi-0.1.2/tests/test_project.py
+-rw-r--r--   0 superhin   (502) staff       (20)      275 2023-06-30 09:09:18.000000 python_yapi-0.1.2/tests/test_user.py
+-rw-r--r--   0 superhin   (502) staff       (20)      542 2023-06-28 07:02:56.000000 python_yapi-0.1.2/tox.ini
```

### Comparing `python-yapi-0.1.1/CONTRIBUTING.rst` & `python_yapi-0.1.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `python-yapi-0.1.1/LICENSE` & `python_yapi-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `python-yapi-0.1.1/PKG-INFO` & `python_yapi-0.1.2/python_yapi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-yapi
-Version: 0.1.1
+Version: 0.1.2
 Summary: python yapi sdk
 Home-page: https://github.com/hanzhichao/python-yapi
 Author: Han Zhichao
 Author-email: superhin@126.com
 License: MIT license
 Keywords: yapi,python-yapi,pyyapi
 Classifier: Programming Language :: Python
```

### Comparing `python-yapi-0.1.1/README.md` & `python_yapi-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `python-yapi-0.1.1/README.rst` & `python_yapi-0.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `python-yapi-0.1.1/python_yapi.egg-info/PKG-INFO` & `python_yapi-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: python-yapi
-Version: 0.1.1
+Name: python_yapi
+Version: 0.1.2
 Summary: python yapi sdk
 Home-page: https://github.com/hanzhichao/python-yapi
 Author: Han Zhichao
 Author-email: superhin@126.com
 License: MIT license
 Keywords: yapi,python-yapi,pyyapi
 Classifier: Programming Language :: Python
```

### Comparing `python-yapi-0.1.1/setup.py` & `python_yapi-0.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 """The setup script."""
 import os
 from setuptools import setup, find_packages
 
-version = '0.1.1'
+version = '0.1.2'
 
 this_directory = os.path.abspath(os.path.dirname(__file__))
 setup_requirements = ['requests',
                       'python-slugify']
 
 def read_file(filename):
     with open(os.path.join(this_directory, filename), encoding='utf-8') as f:
@@ -28,15 +28,15 @@
         'Programming Language :: Python :: 3.7',
     ],
     license="MIT license",
     include_package_data=True,
     keywords=[
         'yapi', 'python-yapi', 'pyyapi',
     ],
-    name='python-yapi',
-    packages=find_packages(include=['python-yapi']),
+    name='python_yapi',
+    packages=find_packages(include=['python_yapi']),
     setup_requires=setup_requirements,
     url='https://github.com/hanzhichao/python-yapi',
     version=version,
     zip_safe=True,
     install_requires=[]
 )
```

### Comparing `python-yapi-0.1.1/tests/test_project.py` & `python_yapi-0.1.2/tests/test_project.py`

 * *Files identical despite different names*

### Comparing `python-yapi-0.1.1/tox.ini` & `python_yapi-0.1.2/tox.ini`

 * *Files identical despite different names*

