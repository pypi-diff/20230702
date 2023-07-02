# Comparing `tmp/fast-webflow-0.2.1.tar.gz` & `tmp/fast-webflow-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fast-webflow-0.2.1.tar", last modified: Sat Jul  1 17:20:38 2023, max compression
+gzip compressed data, was "fast-webflow-0.2.2.tar", last modified: Sun Jul  2 08:38:28 2023, max compression
```

## Comparing `fast-webflow-0.2.1.tar` & `fast-webflow-0.2.2.tar`

### file list

```diff
@@ -1,19 +1,12 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 17:20:38.891965 fast-webflow-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-01 17:20:24.000000 fast-webflow-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5217 2023-07-01 17:20:38.891965 fast-webflow-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4683 2023-07-01 17:20:24.000000 fast-webflow-0.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-01 17:20:24.000000 fast-webflow-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-07-01 17:20:38.891965 fast-webflow-0.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 17:20:38.887965 fast-webflow-0.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 17:20:38.891965 fast-webflow-0.2.1/src/cms/
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-01 17:20:24.000000 fast-webflow-0.2.1/src/cms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3843 2023-07-01 17:20:24.000000 fast-webflow-0.2.1/src/cms/collection.py
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-07-01 17:20:24.000000 fast-webflow-0.2.1/src/cms/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-07-01 17:20:24.000000 fast-webflow-0.2.1/src/cms/item.py
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-07-01 17:20:24.000000 fast-webflow-0.2.1/src/cms/site.py
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-07-01 17:20:24.000000 fast-webflow-0.2.1/src/cms/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 17:20:38.891965 fast-webflow-0.2.1/src/fast_webflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5217 2023-07-01 17:20:38.000000 fast-webflow-0.2.1/src/fast_webflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-01 17:20:38.000000 fast-webflow-0.2.1/src/fast_webflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 17:20:38.000000 fast-webflow-0.2.1/src/fast_webflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-01 17:20:38.000000 fast-webflow-0.2.1/src/fast_webflow.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 08:38:28.331219 fast-webflow-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-02 08:38:19.000000 fast-webflow-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5217 2023-07-02 08:38:28.331219 fast-webflow-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4683 2023-07-02 08:38:19.000000 fast-webflow-0.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-02 08:38:19.000000 fast-webflow-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-07-02 08:38:28.335219 fast-webflow-0.2.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 08:38:28.331219 fast-webflow-0.2.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 08:38:28.331219 fast-webflow-0.2.2/src/fast_webflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5217 2023-07-02 08:38:28.000000 fast-webflow-0.2.2/src/fast_webflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-02 08:38:28.000000 fast-webflow-0.2.2/src/fast_webflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 08:38:28.000000 fast-webflow-0.2.2/src/fast_webflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 08:38:28.000000 fast-webflow-0.2.2/src/fast_webflow.egg-info/top_level.txt
```

### Comparing `fast-webflow-0.2.1/LICENSE` & `fast-webflow-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fast-webflow-0.2.1/PKG-INFO` & `fast-webflow-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast-webflow
-Version: 0.2.1
+Version: 0.2.2
 Summary: A client library to communicate with the WebFlow API
 Home-page: https://github.com/tcilloni/fast-webflow
 Author: Thomas Cilloni
 Author-email: tcilloni@outlook.com
 Project-URL: Bug Tracker, https://github.com/tcilloni/fast-webflow/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fast-webflow-0.2.1/README.md` & `fast-webflow-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `fast-webflow-0.2.1/setup.cfg` & `fast-webflow-0.2.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = fast-webflow
-version = 0.2.1
+version = 0.2.2
 author = Thomas Cilloni
 author_email = tcilloni@outlook.com
 description = A client library to communicate with the WebFlow API
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/tcilloni/fast-webflow
 project_urls =
```

### Comparing `fast-webflow-0.2.1/src/fast_webflow.egg-info/PKG-INFO` & `fast-webflow-0.2.2/src/fast_webflow.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast-webflow
-Version: 0.2.1
+Version: 0.2.2
 Summary: A client library to communicate with the WebFlow API
 Home-page: https://github.com/tcilloni/fast-webflow
 Author: Thomas Cilloni
 Author-email: tcilloni@outlook.com
 Project-URL: Bug Tracker, https://github.com/tcilloni/fast-webflow/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

