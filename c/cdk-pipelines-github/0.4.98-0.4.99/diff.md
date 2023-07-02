# Comparing `tmp/cdk-pipelines-github-0.4.98.tar.gz` & `tmp/cdk-pipelines-github-0.4.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk-pipelines-github-0.4.98.tar", last modified: Sat Jul  1 00:20:16 2023, max compression
+gzip compressed data, was "cdk-pipelines-github-0.4.99.tar", last modified: Sun Jul  2 00:20:01 2023, max compression
```

## Comparing `cdk-pipelines-github-0.4.98.tar` & `cdk-pipelines-github-0.4.99.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:20:16.862165 cdk-pipelines-github-0.4.98/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-01 00:20:00.000000 cdk-pipelines-github-0.4.98/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-01 00:20:00.000000 cdk-pipelines-github-0.4.98/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-01 00:20:00.000000 cdk-pipelines-github-0.4.98/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)    24130 2023-07-01 00:20:16.862165 cdk-pipelines-github-0.4.98/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    23145 2023-07-01 00:20:00.000000 cdk-pipelines-github-0.4.98/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-01 00:20:00.000000 cdk-pipelines-github-0.4.98/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 00:20:16.862165 cdk-pipelines-github-0.4.98/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-07-01 00:20:00.000000 cdk-pipelines-github-0.4.98/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:20:16.858165 cdk-pipelines-github-0.4.98/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:20:16.858165 cdk-pipelines-github-0.4.98/src/cdk_pipelines_github/
--rw-r--r--   0 runner    (1001) docker     (123)   312642 2023-07-01 00:20:00.000000 cdk-pipelines-github-0.4.98/src/cdk_pipelines_github/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:20:16.862165 cdk-pipelines-github-0.4.98/src/cdk_pipelines_github/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-07-01 00:20:00.000000 cdk-pipelines-github-0.4.98/src/cdk_pipelines_github/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   322706 2023-07-01 00:20:00.000000 cdk-pipelines-github-0.4.98/src/cdk_pipelines_github/_jsii/cdk-pipelines-github@0.4.98.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 00:20:00.000000 cdk-pipelines-github-0.4.98/src/cdk_pipelines_github/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 00:20:16.858165 cdk-pipelines-github-0.4.98/src/cdk_pipelines_github.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    24130 2023-07-01 00:20:16.000000 cdk-pipelines-github-0.4.98/src/cdk_pipelines_github.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-07-01 00:20:16.000000 cdk-pipelines-github-0.4.98/src/cdk_pipelines_github.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 00:20:16.000000 cdk-pipelines-github-0.4.98/src/cdk_pipelines_github.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-01 00:20:16.000000 cdk-pipelines-github-0.4.98/src/cdk_pipelines_github.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-01 00:20:16.000000 cdk-pipelines-github-0.4.98/src/cdk_pipelines_github.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 00:20:01.406036 cdk-pipelines-github-0.4.99/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-02 00:19:45.000000 cdk-pipelines-github-0.4.99/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-02 00:19:45.000000 cdk-pipelines-github-0.4.99/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-02 00:19:45.000000 cdk-pipelines-github-0.4.99/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)    24130 2023-07-02 00:20:01.406036 cdk-pipelines-github-0.4.99/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    23145 2023-07-02 00:19:45.000000 cdk-pipelines-github-0.4.99/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-02 00:19:45.000000 cdk-pipelines-github-0.4.99/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 00:20:01.406036 cdk-pipelines-github-0.4.99/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-07-02 00:19:45.000000 cdk-pipelines-github-0.4.99/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 00:20:01.402036 cdk-pipelines-github-0.4.99/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 00:20:01.406036 cdk-pipelines-github-0.4.99/src/cdk_pipelines_github/
+-rw-r--r--   0 runner    (1001) docker     (123)   312642 2023-07-02 00:19:45.000000 cdk-pipelines-github-0.4.99/src/cdk_pipelines_github/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 00:20:01.406036 cdk-pipelines-github-0.4.99/src/cdk_pipelines_github/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-07-02 00:19:45.000000 cdk-pipelines-github-0.4.99/src/cdk_pipelines_github/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   322704 2023-07-02 00:19:45.000000 cdk-pipelines-github-0.4.99/src/cdk_pipelines_github/_jsii/cdk-pipelines-github@0.4.99.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 00:19:45.000000 cdk-pipelines-github-0.4.99/src/cdk_pipelines_github/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 00:20:01.406036 cdk-pipelines-github-0.4.99/src/cdk_pipelines_github.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    24130 2023-07-02 00:20:01.000000 cdk-pipelines-github-0.4.99/src/cdk_pipelines_github.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-07-02 00:20:01.000000 cdk-pipelines-github-0.4.99/src/cdk_pipelines_github.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 00:20:01.000000 cdk-pipelines-github-0.4.99/src/cdk_pipelines_github.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-02 00:20:01.000000 cdk-pipelines-github-0.4.99/src/cdk_pipelines_github.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-02 00:20:01.000000 cdk-pipelines-github-0.4.99/src/cdk_pipelines_github.egg-info/top_level.txt
```

### Comparing `cdk-pipelines-github-0.4.98/LICENSE` & `cdk-pipelines-github-0.4.99/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-pipelines-github-0.4.98/PKG-INFO` & `cdk-pipelines-github-0.4.99/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-pipelines-github
-Version: 0.4.98
+Version: 0.4.99
 Summary: GitHub Workflows support for CDK Pipelines
 Home-page: https://github.com/cdklabs/cdk-pipelines-github.git
 Author: Amazon Web Services<aws-cdk-dev@amazon.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdklabs/cdk-pipelines-github.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdk-pipelines-github-0.4.98/README.md` & `cdk-pipelines-github-0.4.99/README.md`

 * *Files identical despite different names*

### Comparing `cdk-pipelines-github-0.4.98/setup.py` & `cdk-pipelines-github-0.4.99/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-pipelines-github",
-    "version": "0.4.98",
+    "version": "0.4.99",
     "description": "GitHub Workflows support for CDK Pipelines",
     "license": "Apache-2.0",
     "url": "https://github.com/cdklabs/cdk-pipelines-github.git",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services<aws-cdk-dev@amazon.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "cdk_pipelines_github",
         "cdk_pipelines_github._jsii"
     ],
     "package_data": {
         "cdk_pipelines_github._jsii": [
-            "cdk-pipelines-github@0.4.98.jsii.tgz"
+            "cdk-pipelines-github@0.4.99.jsii.tgz"
         ],
         "cdk_pipelines_github": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `cdk-pipelines-github-0.4.98/src/cdk_pipelines_github/__init__.py` & `cdk-pipelines-github-0.4.99/src/cdk_pipelines_github/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-pipelines-github-0.4.98/src/cdk_pipelines_github.egg-info/PKG-INFO` & `cdk-pipelines-github-0.4.99/src/cdk_pipelines_github.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-pipelines-github
-Version: 0.4.98
+Version: 0.4.99
 Summary: GitHub Workflows support for CDK Pipelines
 Home-page: https://github.com/cdklabs/cdk-pipelines-github.git
 Author: Amazon Web Services<aws-cdk-dev@amazon.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdklabs/cdk-pipelines-github.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

