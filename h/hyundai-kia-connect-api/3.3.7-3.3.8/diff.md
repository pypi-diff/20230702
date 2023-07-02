# Comparing `tmp/hyundai_kia_connect_api-3.3.7.tar.gz` & `tmp/hyundai_kia_connect_api-3.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyundai_kia_connect_api-3.3.7.tar", last modified: Thu May 25 02:04:03 2023, max compression
+gzip compressed data, was "hyundai_kia_connect_api-3.3.8.tar", last modified: Sun Jul  2 20:07:01 2023, max compression
```

## Comparing `hyundai_kia_connect_api-3.3.7.tar` & `hyundai_kia_connect_api-3.3.8.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:04:03.517141 hyundai_kia_connect_api-3.3.7/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-25 02:03:24.000000 hyundai_kia_connect_api-3.3.7/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3699 2023-05-25 02:03:24.000000 hyundai_kia_connect_api-3.3.7/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-25 02:03:24.000000 hyundai_kia_connect_api-3.3.7/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-25 02:03:24.000000 hyundai_kia_connect_api-3.3.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-25 02:03:24.000000 hyundai_kia_connect_api-3.3.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5578 2023-05-25 02:04:03.517141 hyundai_kia_connect_api-3.3.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4940 2023-05-25 02:03:24.000000 hyundai_kia_connect_api-3.3.7/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:04:03.513141 hyundai_kia_connect_api-3.3.7/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-05-25 02:03:24.000000 hyundai_kia_connect_api-3.3.7/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-25 02:03:24.000000 hyundai_kia_connect_api-3.3.7/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5079 2023-05-25 02:03:24.000000 hyundai_kia_connect_api-3.3.7/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-25 02:03:24.000000 hyundai_kia_connect_api-3.3.7/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-25 02:03:24.000000 hyundai_kia_connect_api-3.3.7/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-25 02:03:24.000000 hyundai_kia_connect_api-3.3.7/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-05-25 02:03:24.000000 hyundai_kia_connect_api-3.3.7/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-25 02:03:24.000000 hyundai_kia_connect_api-3.3.7/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-25 02:03:24.000000 hyundai_kia_connect_api-3.3.7/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-25 02:03:24.000000 hyundai_kia_connect_api-3.3.7/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:04:03.517141 hyundai_kia_connect_api-3.3.7/hyundai_kia_connect_api/
--rw-r--r--   0 runner    (1001) docker     (123)     4626 2023-05-25 02:03:24.000000 hyundai_kia_connect_api-3.3.7/hyundai_kia_connect_api/ApiImpl.py
--rw-r--r--   0 runner    (1001) docker     (123)    23880 2023-05-25 02:03:24.000000 hyundai_kia_connect_api-3.3.7/hyundai_kia_connect_api/HyundaiBlueLinkAPIUSA.py
--rw-r--r--   0 runner    (1001) docker     (123)    27449 2023-05-25 02:03:24.000000 hyundai_kia_connect_api-3.3.7/hyundai_kia_connect_api/KiaUvoAPIUSA.py
--rw-r--r--   0 runner    (1001) docker     (123)    29985 2023-05-25 02:03:24.000000 hyundai_kia_connect_api-3.3.7/hyundai_kia_connect_api/KiaUvoApiCA.py
--rw-r--r--   0 runner    (1001) docker     (123)    51311 2023-05-25 02:03:24.000000 hyundai_kia_connect_api-3.3.7/hyundai_kia_connect_api/KiaUvoApiCN.py
--rw-r--r--   0 runner    (1001) docker     (123)    53887 2023-05-25 02:03:24.000000 hyundai_kia_connect_api-3.3.7/hyundai_kia_connect_api/KiaUvoApiEU.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-25 02:03:24.000000 hyundai_kia_connect_api-3.3.7/hyundai_kia_connect_api/Token.py
--rw-r--r--   0 runner    (1001) docker     (123)    12772 2023-05-25 02:03:24.000000 hyundai_kia_connect_api-3.3.7/hyundai_kia_connect_api/Vehicle.py
--rw-r--r--   0 runner    (1001) docker     (123)     9083 2023-05-25 02:03:24.000000 hyundai_kia_connect_api-3.3.7/hyundai_kia_connect_api/VehicleManager.py
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-25 02:03:24.000000 hyundai_kia_connect_api-3.3.7/hyundai_kia_connect_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-05-25 02:03:24.000000 hyundai_kia_connect_api-3.3.7/hyundai_kia_connect_api/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-05-25 02:03:24.000000 hyundai_kia_connect_api-3.3.7/hyundai_kia_connect_api/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-05-25 02:03:24.000000 hyundai_kia_connect_api-3.3.7/hyundai_kia_connect_api/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:04:03.517141 hyundai_kia_connect_api-3.3.7/hyundai_kia_connect_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5578 2023-05-25 02:04:03.000000 hyundai_kia_connect_api-3.3.7/hyundai_kia_connect_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-05-25 02:04:03.000000 hyundai_kia_connect_api-3.3.7/hyundai_kia_connect_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 02:04:03.000000 hyundai_kia_connect_api-3.3.7/hyundai_kia_connect_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 02:04:03.000000 hyundai_kia_connect_api-3.3.7/hyundai_kia_connect_api.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-25 02:04:03.000000 hyundai_kia_connect_api-3.3.7/hyundai_kia_connect_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-25 02:04:03.000000 hyundai_kia_connect_api-3.3.7/hyundai_kia_connect_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-25 02:03:24.000000 hyundai_kia_connect_api-3.3.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-25 02:04:03.517141 hyundai_kia_connect_api-3.3.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-25 02:03:51.000000 hyundai_kia_connect_api-3.3.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:04:03.517141 hyundai_kia_connect_api-3.3.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 02:03:24.000000 hyundai_kia_connect_api-3.3.7/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-05-25 02:03:24.000000 hyundai_kia_connect_api-3.3.7/tests/ca_login_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-05-25 02:03:24.000000 hyundai_kia_connect_api-3.3.7/tests/eu_check_response_for_errors_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-25 02:03:24.000000 hyundai_kia_connect_api-3.3.7/tests/eu_login_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 20:07:01.405008 hyundai_kia_connect_api-3.3.8/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-02 20:06:17.000000 hyundai_kia_connect_api-3.3.8/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3699 2023-07-02 20:06:17.000000 hyundai_kia_connect_api-3.3.8/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-02 20:06:17.000000 hyundai_kia_connect_api-3.3.8/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-02 20:06:17.000000 hyundai_kia_connect_api-3.3.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-02 20:06:17.000000 hyundai_kia_connect_api-3.3.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5578 2023-07-02 20:07:01.405008 hyundai_kia_connect_api-3.3.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4940 2023-07-02 20:06:17.000000 hyundai_kia_connect_api-3.3.8/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 20:07:01.401008 hyundai_kia_connect_api-3.3.8/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-07-02 20:06:17.000000 hyundai_kia_connect_api-3.3.8/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-02 20:06:17.000000 hyundai_kia_connect_api-3.3.8/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5079 2023-07-02 20:06:17.000000 hyundai_kia_connect_api-3.3.8/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-02 20:06:17.000000 hyundai_kia_connect_api-3.3.8/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-02 20:06:17.000000 hyundai_kia_connect_api-3.3.8/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-02 20:06:17.000000 hyundai_kia_connect_api-3.3.8/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-07-02 20:06:17.000000 hyundai_kia_connect_api-3.3.8/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-02 20:06:17.000000 hyundai_kia_connect_api-3.3.8/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-02 20:06:17.000000 hyundai_kia_connect_api-3.3.8/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-02 20:06:17.000000 hyundai_kia_connect_api-3.3.8/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 20:07:01.405008 hyundai_kia_connect_api-3.3.8/hyundai_kia_connect_api/
+-rw-r--r--   0 runner    (1001) docker     (123)     4626 2023-07-02 20:06:17.000000 hyundai_kia_connect_api-3.3.8/hyundai_kia_connect_api/ApiImpl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23880 2023-07-02 20:06:17.000000 hyundai_kia_connect_api-3.3.8/hyundai_kia_connect_api/HyundaiBlueLinkAPIUSA.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27449 2023-07-02 20:06:17.000000 hyundai_kia_connect_api-3.3.8/hyundai_kia_connect_api/KiaUvoAPIUSA.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29985 2023-07-02 20:06:17.000000 hyundai_kia_connect_api-3.3.8/hyundai_kia_connect_api/KiaUvoApiCA.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51311 2023-07-02 20:06:17.000000 hyundai_kia_connect_api-3.3.8/hyundai_kia_connect_api/KiaUvoApiCN.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53979 2023-07-02 20:06:17.000000 hyundai_kia_connect_api-3.3.8/hyundai_kia_connect_api/KiaUvoApiEU.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-02 20:06:17.000000 hyundai_kia_connect_api-3.3.8/hyundai_kia_connect_api/Token.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12772 2023-07-02 20:06:17.000000 hyundai_kia_connect_api-3.3.8/hyundai_kia_connect_api/Vehicle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9083 2023-07-02 20:06:17.000000 hyundai_kia_connect_api-3.3.8/hyundai_kia_connect_api/VehicleManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-07-02 20:06:17.000000 hyundai_kia_connect_api-3.3.8/hyundai_kia_connect_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-07-02 20:06:17.000000 hyundai_kia_connect_api-3.3.8/hyundai_kia_connect_api/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-07-02 20:06:17.000000 hyundai_kia_connect_api-3.3.8/hyundai_kia_connect_api/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-02 20:06:17.000000 hyundai_kia_connect_api-3.3.8/hyundai_kia_connect_api/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 20:07:01.405008 hyundai_kia_connect_api-3.3.8/hyundai_kia_connect_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5578 2023-07-02 20:07:01.000000 hyundai_kia_connect_api-3.3.8/hyundai_kia_connect_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-07-02 20:07:01.000000 hyundai_kia_connect_api-3.3.8/hyundai_kia_connect_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 20:07:01.000000 hyundai_kia_connect_api-3.3.8/hyundai_kia_connect_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 20:07:01.000000 hyundai_kia_connect_api-3.3.8/hyundai_kia_connect_api.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-02 20:07:01.000000 hyundai_kia_connect_api-3.3.8/hyundai_kia_connect_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-02 20:07:01.000000 hyundai_kia_connect_api-3.3.8/hyundai_kia_connect_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-02 20:06:17.000000 hyundai_kia_connect_api-3.3.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-02 20:07:01.405008 hyundai_kia_connect_api-3.3.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-07-02 20:06:47.000000 hyundai_kia_connect_api-3.3.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 20:07:01.405008 hyundai_kia_connect_api-3.3.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 20:06:17.000000 hyundai_kia_connect_api-3.3.8/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-02 20:06:17.000000 hyundai_kia_connect_api-3.3.8/tests/ca_login_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-07-02 20:06:17.000000 hyundai_kia_connect_api-3.3.8/tests/eu_check_response_for_errors_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-07-02 20:06:17.000000 hyundai_kia_connect_api-3.3.8/tests/eu_login_test.py
```

### Comparing `hyundai_kia_connect_api-3.3.7/CONTRIBUTING.rst` & `hyundai_kia_connect_api-3.3.8/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.3.7/LICENSE` & `hyundai_kia_connect_api-3.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.3.7/PKG-INFO` & `hyundai_kia_connect_api-3.3.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyundai_kia_connect_api
-Version: 3.3.7
+Version: 3.3.8
 Summary: Python Boilerplate contains all the boilerplate you need to create a Python package.
 Home-page: https://github.com/fuatakgun/hyundai_kia_connect_api
 Author: Fuat Akgun
 Author-email: fuatakgun@gmail.com
 License: MIT license
 Keywords: hyundai_kia_connect_api
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `hyundai_kia_connect_api-3.3.7/README.rst` & `hyundai_kia_connect_api-3.3.8/README.rst`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.3.7/docs/Makefile` & `hyundai_kia_connect_api-3.3.8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.3.7/docs/conf.py` & `hyundai_kia_connect_api-3.3.8/docs/conf.py`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.3.7/docs/installation.rst` & `hyundai_kia_connect_api-3.3.8/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.3.7/docs/make.bat` & `hyundai_kia_connect_api-3.3.8/docs/make.bat`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.3.7/hyundai_kia_connect_api/ApiImpl.py` & `hyundai_kia_connect_api-3.3.8/hyundai_kia_connect_api/ApiImpl.py`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.3.7/hyundai_kia_connect_api/HyundaiBlueLinkAPIUSA.py` & `hyundai_kia_connect_api-3.3.8/hyundai_kia_connect_api/HyundaiBlueLinkAPIUSA.py`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.3.7/hyundai_kia_connect_api/KiaUvoAPIUSA.py` & `hyundai_kia_connect_api-3.3.8/hyundai_kia_connect_api/KiaUvoAPIUSA.py`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.3.7/hyundai_kia_connect_api/KiaUvoApiCA.py` & `hyundai_kia_connect_api-3.3.8/hyundai_kia_connect_api/KiaUvoApiCA.py`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.3.7/hyundai_kia_connect_api/KiaUvoApiCN.py` & `hyundai_kia_connect_api-3.3.8/hyundai_kia_connect_api/KiaUvoApiCN.py`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.3.7/hyundai_kia_connect_api/KiaUvoApiEU.py` & `hyundai_kia_connect_api-3.3.8/hyundai_kia_connect_api/KiaUvoApiEU.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """KiaUvoApiEU.py"""
 # pylint:disable=missing-timeout,missing-class-docstring,missing-function-docstring,wildcard-import,unused-wildcard-import,invalid-name,logging-fstring-interpolation,broad-except,bare-except,super-init-not-called,unused-argument,line-too-long,too-many-lines
 
+import random
 import datetime as dt
 import logging
 import re
 import uuid
 from time import sleep
 from urllib.parse import parse_qs, urlparse
 
@@ -1076,15 +1077,17 @@
         if (position * 100.0) / stamp_count > 90:
             self.stamps = None
             return self._get_stamp()
         else:
             return self.stamps["stamps"][position]
 
     def _get_device_id(self, stamp: str):
-        registration_id = 1
+        ran = random.randrange(10**80)
+        myhex = "%064x" % ran
+        registration_id = myhex[:64]
         url = self.SPA_API_URL + "notifications/register"
         payload = {
             "pushRegId": registration_id,
             "pushType": "GCM",
             "uuid": str(uuid.uuid4()),
         }
```

### Comparing `hyundai_kia_connect_api-3.3.7/hyundai_kia_connect_api/Vehicle.py` & `hyundai_kia_connect_api-3.3.8/hyundai_kia_connect_api/Vehicle.py`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.3.7/hyundai_kia_connect_api/VehicleManager.py` & `hyundai_kia_connect_api-3.3.8/hyundai_kia_connect_api/VehicleManager.py`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.3.7/hyundai_kia_connect_api/const.py` & `hyundai_kia_connect_api-3.3.8/hyundai_kia_connect_api/const.py`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.3.7/hyundai_kia_connect_api/exceptions.py` & `hyundai_kia_connect_api-3.3.8/hyundai_kia_connect_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.3.7/hyundai_kia_connect_api/utils.py` & `hyundai_kia_connect_api-3.3.8/hyundai_kia_connect_api/utils.py`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.3.7/hyundai_kia_connect_api.egg-info/PKG-INFO` & `hyundai_kia_connect_api-3.3.8/hyundai_kia_connect_api.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyundai-kia-connect-api
-Version: 3.3.7
+Version: 3.3.8
 Summary: Python Boilerplate contains all the boilerplate you need to create a Python package.
 Home-page: https://github.com/fuatakgun/hyundai_kia_connect_api
 Author: Fuat Akgun
 Author-email: fuatakgun@gmail.com
 License: MIT license
 Keywords: hyundai_kia_connect_api
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `hyundai_kia_connect_api-3.3.7/hyundai_kia_connect_api.egg-info/SOURCES.txt` & `hyundai_kia_connect_api-3.3.8/hyundai_kia_connect_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.3.7/setup.py` & `hyundai_kia_connect_api-3.3.8/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -40,10 +40,10 @@
     name="hyundai_kia_connect_api",
     packages=find_packages(
         include=["hyundai_kia_connect_api", "hyundai_kia_connect_api.*"]
     ),
     test_suite="tests",
     tests_require=test_requirements,
     url="https://github.com/fuatakgun/hyundai_kia_connect_api",
-    version="3.3.7",
+    version="3.3.8",
     zip_safe=False,
 )
```

### Comparing `hyundai_kia_connect_api-3.3.7/tests/ca_login_test.py` & `hyundai_kia_connect_api-3.3.8/tests/ca_login_test.py`

 * *Files identical despite different names*

### Comparing `hyundai_kia_connect_api-3.3.7/tests/eu_check_response_for_errors_test.py` & `hyundai_kia_connect_api-3.3.8/tests/eu_check_response_for_errors_test.py`

 * *Files identical despite different names*

