# Comparing `tmp/omnivoreql-0.2.2.tar.gz` & `tmp/omnivoreql-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omnivoreql-0.2.2.tar", last modified: Sun Jul  2 11:46:03 2023, max compression
+gzip compressed data, was "omnivoreql-0.2.3.tar", last modified: Sun Jul  2 15:29:55 2023, max compression
```

## Comparing `omnivoreql-0.2.2.tar` & `omnivoreql-0.2.3.tar`

### file list

```diff
@@ -1,22 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 11:46:03.451197 omnivoreql-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-07-02 11:45:59.000000 omnivoreql-0.2.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-02 11:45:59.000000 omnivoreql-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-02 11:45:59.000000 omnivoreql-0.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-07-02 11:46:03.451197 omnivoreql-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-07-02 11:45:59.000000 omnivoreql-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 11:46:03.451197 omnivoreql-0.2.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-07-02 11:45:59.000000 omnivoreql-0.2.2/docs/PYPI.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 11:45:59.000000 omnivoreql-0.2.2/docs/__init__,py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 11:46:03.451197 omnivoreql-0.2.2/omnivoreql/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-02 11:45:59.000000 omnivoreql-0.2.2/omnivoreql/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 11:46:03.451197 omnivoreql-0.2.2/omnivoreql.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-07-02 11:46:03.000000 omnivoreql-0.2.2/omnivoreql.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-07-02 11:46:03.000000 omnivoreql-0.2.2/omnivoreql.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 11:46:03.000000 omnivoreql-0.2.2/omnivoreql.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-02 11:46:03.000000 omnivoreql-0.2.2/omnivoreql.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 11:46:03.000000 omnivoreql-0.2.2/omnivoreql.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-02 11:45:59.000000 omnivoreql-0.2.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 11:46:03.451197 omnivoreql-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-07-02 11:45:59.000000 omnivoreql-0.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 11:46:03.451197 omnivoreql-0.2.2/test/
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-07-02 11:45:59.000000 omnivoreql-0.2.2/test/test_omnivoreql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 15:29:55.848713 omnivoreql-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-02 15:29:51.000000 omnivoreql-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-02 15:29:51.000000 omnivoreql-0.2.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-07-02 15:29:55.848713 omnivoreql-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-07-02 15:29:51.000000 omnivoreql-0.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 15:29:55.844714 omnivoreql-0.2.3/omnivoreql/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-02 15:29:51.000000 omnivoreql-0.2.3/omnivoreql/__init__,py
+-rw-r--r--   0 runner    (1001) docker     (123)    10216 2023-07-02 15:29:51.000000 omnivoreql-0.2.3/omnivoreql/omnivoreql.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53876 2023-07-02 15:29:51.000000 omnivoreql-0.2.3/omnivoreql/schema.gql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 15:29:55.848713 omnivoreql-0.2.3/omnivoreql.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-07-02 15:29:55.000000 omnivoreql-0.2.3/omnivoreql.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-02 15:29:55.000000 omnivoreql-0.2.3/omnivoreql.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 15:29:55.000000 omnivoreql-0.2.3/omnivoreql.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-02 15:29:55.000000 omnivoreql-0.2.3/omnivoreql.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 15:29:55.000000 omnivoreql-0.2.3/omnivoreql.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-02 15:29:51.000000 omnivoreql-0.2.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 15:29:55.848713 omnivoreql-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-07-02 15:29:51.000000 omnivoreql-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 15:29:55.848713 omnivoreql-0.2.3/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-07-02 15:29:51.000000 omnivoreql-0.2.3/test/test_omnivoreql.py
```

### Comparing `omnivoreql-0.2.2/LICENSE` & `omnivoreql-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `omnivoreql-0.2.2/PKG-INFO` & `omnivoreql-0.2.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: omnivoreql
-Version: 0.2.2
+Version: 0.2.3
 Summary: Omnivore API Client for Python
 Home-page: https://github.com/yazdipour/OmnivoreQL
 Author: Shahriar Yazdipour
 Author-email: git@yazdipour.com
 License: MIT
+Project-URL: Bug Tracker, https://github.com/yazdipour/OmnivoreQL/issues
+Project-URL: Source Code, https://github.com/yazdipour/OmnivoreQL
 Keywords: omnivore api readlater graphql gql client
 Platform: any
-Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `omnivoreql-0.2.2/README.md` & `omnivoreql-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `omnivoreql-0.2.2/omnivoreql.egg-info/PKG-INFO` & `omnivoreql-0.2.3/omnivoreql.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: omnivoreql
-Version: 0.2.2
+Version: 0.2.3
 Summary: Omnivore API Client for Python
 Home-page: https://github.com/yazdipour/OmnivoreQL
 Author: Shahriar Yazdipour
 Author-email: git@yazdipour.com
 License: MIT
+Project-URL: Bug Tracker, https://github.com/yazdipour/OmnivoreQL/issues
+Project-URL: Source Code, https://github.com/yazdipour/OmnivoreQL
 Keywords: omnivore api readlater graphql gql client
 Platform: any
-Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `omnivoreql-0.2.2/test/test_omnivoreql.py` & `omnivoreql-0.2.3/test/test_omnivoreql.py`

 * *Files identical despite different names*

