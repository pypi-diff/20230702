# Comparing `tmp/omnivoreql-0.2.3.tar.gz` & `tmp/omnivoreql-0.2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omnivoreql-0.2.3.tar", last modified: Sun Jul  2 15:29:55 2023, max compression
+gzip compressed data, was "omnivoreql-0.2.3.1.tar", last modified: Sun Jul  2 17:27:44 2023, max compression
```

## Comparing `omnivoreql-0.2.3.tar` & `omnivoreql-0.2.3.1.tar`

### file list

```diff
@@ -1,20 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 15:29:55.848713 omnivoreql-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-02 15:29:51.000000 omnivoreql-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-02 15:29:51.000000 omnivoreql-0.2.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-07-02 15:29:55.848713 omnivoreql-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-07-02 15:29:51.000000 omnivoreql-0.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 15:29:55.844714 omnivoreql-0.2.3/omnivoreql/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-02 15:29:51.000000 omnivoreql-0.2.3/omnivoreql/__init__,py
--rw-r--r--   0 runner    (1001) docker     (123)    10216 2023-07-02 15:29:51.000000 omnivoreql-0.2.3/omnivoreql/omnivoreql.py
--rw-r--r--   0 runner    (1001) docker     (123)    53876 2023-07-02 15:29:51.000000 omnivoreql-0.2.3/omnivoreql/schema.gql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 15:29:55.848713 omnivoreql-0.2.3/omnivoreql.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-07-02 15:29:55.000000 omnivoreql-0.2.3/omnivoreql.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-02 15:29:55.000000 omnivoreql-0.2.3/omnivoreql.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 15:29:55.000000 omnivoreql-0.2.3/omnivoreql.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-02 15:29:55.000000 omnivoreql-0.2.3/omnivoreql.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 15:29:55.000000 omnivoreql-0.2.3/omnivoreql.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-02 15:29:51.000000 omnivoreql-0.2.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 15:29:55.848713 omnivoreql-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-07-02 15:29:51.000000 omnivoreql-0.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 15:29:55.848713 omnivoreql-0.2.3/test/
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-07-02 15:29:51.000000 omnivoreql-0.2.3/test/test_omnivoreql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 17:27:44.913563 omnivoreql-0.2.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-02 17:27:40.000000 omnivoreql-0.2.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-02 17:27:40.000000 omnivoreql-0.2.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-07-02 17:27:44.913563 omnivoreql-0.2.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-07-02 17:27:40.000000 omnivoreql-0.2.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 17:27:44.913563 omnivoreql-0.2.3.1/omnivoreql/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-02 17:27:40.000000 omnivoreql-0.2.3.1/omnivoreql/__init__,py
+-rw-r--r--   0 runner    (1001) docker     (123)    10216 2023-07-02 17:27:40.000000 omnivoreql-0.2.3.1/omnivoreql/omnivoreql.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53876 2023-07-02 17:27:40.000000 omnivoreql-0.2.3.1/omnivoreql/schema.gql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 17:27:44.913563 omnivoreql-0.2.3.1/omnivoreql.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-07-02 17:27:44.000000 omnivoreql-0.2.3.1/omnivoreql.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-02 17:27:44.000000 omnivoreql-0.2.3.1/omnivoreql.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 17:27:44.000000 omnivoreql-0.2.3.1/omnivoreql.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-02 17:27:44.000000 omnivoreql-0.2.3.1/omnivoreql.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 17:27:44.000000 omnivoreql-0.2.3.1/omnivoreql.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-02 17:27:40.000000 omnivoreql-0.2.3.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 17:27:44.913563 omnivoreql-0.2.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-07-02 17:27:40.000000 omnivoreql-0.2.3.1/setup.py
```

### Comparing `omnivoreql-0.2.3/LICENSE` & `omnivoreql-0.2.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `omnivoreql-0.2.3/PKG-INFO` & `omnivoreql-0.2.3.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omnivoreql
-Version: 0.2.3
+Version: 0.2.3.1
 Summary: Omnivore API Client for Python
 Home-page: https://github.com/yazdipour/OmnivoreQL
 Author: Shahriar Yazdipour
 Author-email: git@yazdipour.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/yazdipour/OmnivoreQL/issues
 Project-URL: Source Code, https://github.com/yazdipour/OmnivoreQL
```

### Comparing `omnivoreql-0.2.3/README.md` & `omnivoreql-0.2.3.1/README.md`

 * *Files identical despite different names*

### Comparing `omnivoreql-0.2.3/omnivoreql/omnivoreql.py` & `omnivoreql-0.2.3.1/omnivoreql/omnivoreql.py`

 * *Files identical despite different names*

### Comparing `omnivoreql-0.2.3/omnivoreql/schema.gql` & `omnivoreql-0.2.3.1/omnivoreql/schema.gql`

 * *Files identical despite different names*

### Comparing `omnivoreql-0.2.3/omnivoreql.egg-info/PKG-INFO` & `omnivoreql-0.2.3.1/omnivoreql.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omnivoreql
-Version: 0.2.3
+Version: 0.2.3.1
 Summary: Omnivore API Client for Python
 Home-page: https://github.com/yazdipour/OmnivoreQL
 Author: Shahriar Yazdipour
 Author-email: git@yazdipour.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/yazdipour/OmnivoreQL/issues
 Project-URL: Source Code, https://github.com/yazdipour/OmnivoreQL
```

### Comparing `omnivoreql-0.2.3/setup.py` & `omnivoreql-0.2.3.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = "0.2.3"
+VERSION = "0.2.3.1"
 PROJECT_URLS = {
     "Bug Tracker": "https://github.com/yazdipour/OmnivoreQL/issues",
     "Source Code": "https://github.com/yazdipour/OmnivoreQL",
 }
 
 setup(
     name='omnivoreql',
```

