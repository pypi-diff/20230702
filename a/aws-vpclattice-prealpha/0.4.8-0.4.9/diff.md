# Comparing `tmp/aws-vpclattice-prealpha-0.4.8.tar.gz` & `tmp/aws-vpclattice-prealpha-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws-vpclattice-prealpha-0.4.8.tar", last modified: Sun Jul  2 09:48:08 2023, max compression
+gzip compressed data, was "aws-vpclattice-prealpha-0.4.9.tar", last modified: Sun Jul  2 10:45:47 2023, max compression
```

## Comparing `aws-vpclattice-prealpha-0.4.8.tar` & `aws-vpclattice-prealpha-0.4.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:48:08.288814 aws-vpclattice-prealpha-0.4.8/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-02 09:47:55.000000 aws-vpclattice-prealpha-0.4.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-02 09:47:55.000000 aws-vpclattice-prealpha-0.4.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-07-02 09:48:08.288814 aws-vpclattice-prealpha-0.4.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-02 09:47:55.000000 aws-vpclattice-prealpha-0.4.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-02 09:47:55.000000 aws-vpclattice-prealpha-0.4.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 09:48:08.288814 aws-vpclattice-prealpha-0.4.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-07-02 09:47:55.000000 aws-vpclattice-prealpha-0.4.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:48:08.288814 aws-vpclattice-prealpha-0.4.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:48:08.288814 aws-vpclattice-prealpha-0.4.8/src/aws_vpclattice_prealpha.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-07-02 09:48:08.000000 aws-vpclattice-prealpha-0.4.8/src/aws_vpclattice_prealpha.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-07-02 09:48:08.000000 aws-vpclattice-prealpha-0.4.8/src/aws_vpclattice_prealpha.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 09:48:08.000000 aws-vpclattice-prealpha-0.4.8/src/aws_vpclattice_prealpha.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-02 09:48:08.000000 aws-vpclattice-prealpha-0.4.8/src/aws_vpclattice_prealpha.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-02 09:48:08.000000 aws-vpclattice-prealpha-0.4.8/src/aws_vpclattice_prealpha.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:48:08.288814 aws-vpclattice-prealpha-0.4.8/src/vpc_lattice/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:48:08.288814 aws-vpclattice-prealpha-0.4.8/src/vpc_lattice/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-07-02 09:47:55.000000 aws-vpclattice-prealpha-0.4.8/src/vpc_lattice/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12804 2023-07-02 09:47:55.000000 aws-vpclattice-prealpha-0.4.8/src/vpc_lattice/_jsii/aws-vpclattice-prealpha@0.4.8.jsii.tgz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:45:47.923478 aws-vpclattice-prealpha-0.4.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-02 10:45:35.000000 aws-vpclattice-prealpha-0.4.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-02 10:45:35.000000 aws-vpclattice-prealpha-0.4.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-07-02 10:45:47.923478 aws-vpclattice-prealpha-0.4.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-02 10:45:35.000000 aws-vpclattice-prealpha-0.4.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-02 10:45:35.000000 aws-vpclattice-prealpha-0.4.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 10:45:47.923478 aws-vpclattice-prealpha-0.4.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-07-02 10:45:35.000000 aws-vpclattice-prealpha-0.4.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:45:47.919478 aws-vpclattice-prealpha-0.4.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:45:47.923478 aws-vpclattice-prealpha-0.4.9/src/aws_vpclattice_prealpha.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-07-02 10:45:47.000000 aws-vpclattice-prealpha-0.4.9/src/aws_vpclattice_prealpha.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-07-02 10:45:47.000000 aws-vpclattice-prealpha-0.4.9/src/aws_vpclattice_prealpha.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 10:45:47.000000 aws-vpclattice-prealpha-0.4.9/src/aws_vpclattice_prealpha.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-02 10:45:47.000000 aws-vpclattice-prealpha-0.4.9/src/aws_vpclattice_prealpha.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-02 10:45:47.000000 aws-vpclattice-prealpha-0.4.9/src/aws_vpclattice_prealpha.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:45:47.919478 aws-vpclattice-prealpha-0.4.9/src/vpc_lattice/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:45:47.923478 aws-vpclattice-prealpha-0.4.9/src/vpc_lattice/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-07-02 10:45:35.000000 aws-vpclattice-prealpha-0.4.9/src/vpc_lattice/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12838 2023-07-02 10:45:35.000000 aws-vpclattice-prealpha-0.4.9/src/vpc_lattice/_jsii/aws-vpclattice-prealpha@0.4.9.jsii.tgz
```

### Comparing `aws-vpclattice-prealpha-0.4.8/LICENSE` & `aws-vpclattice-prealpha-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `aws-vpclattice-prealpha-0.4.8/PKG-INFO` & `aws-vpclattice-prealpha-0.4.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-vpclattice-prealpha
-Version: 0.4.8
+Version: 0.4.9
 Summary: aws-vpclattice-prealpha
 Home-page: https://github.com/raindancers/aws-vpclattice-prealpha.git
 Author: Andrew Frazer<andrew.frazer@raindancers.cloud>
 License: Apache-2.0
 Project-URL: Source, https://github.com/raindancers/aws-vpclattice-prealpha.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `aws-vpclattice-prealpha-0.4.8/setup.py` & `aws-vpclattice-prealpha-0.4.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "aws-vpclattice-prealpha",
-    "version": "0.4.8",
+    "version": "0.4.9",
     "description": "aws-vpclattice-prealpha",
     "license": "Apache-2.0",
     "url": "https://github.com/raindancers/aws-vpclattice-prealpha.git",
     "long_description_content_type": "text/markdown",
     "author": "Andrew Frazer<andrew.frazer@raindancers.cloud>",
     "bdist_wheel": {
         "universal": true
@@ -21,15 +21,15 @@
         "": "src"
     },
     "packages": [
         "vpc_lattice._jsii"
     ],
     "package_data": {
         "vpc_lattice._jsii": [
-            "aws-vpclattice-prealpha@0.4.8.jsii.tgz"
+            "aws-vpclattice-prealpha@0.4.9.jsii.tgz"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
         "aws-cdk-lib>=2.80.0, <3.0.0",
         "constructs>=10.0.5, <11.0.0",
         "jsii>=1.84.0, <2.0.0",
```

### Comparing `aws-vpclattice-prealpha-0.4.8/src/aws_vpclattice_prealpha.egg-info/PKG-INFO` & `aws-vpclattice-prealpha-0.4.9/src/aws_vpclattice_prealpha.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-vpclattice-prealpha
-Version: 0.4.8
+Version: 0.4.9
 Summary: aws-vpclattice-prealpha
 Home-page: https://github.com/raindancers/aws-vpclattice-prealpha.git
 Author: Andrew Frazer<andrew.frazer@raindancers.cloud>
 License: Apache-2.0
 Project-URL: Source, https://github.com/raindancers/aws-vpclattice-prealpha.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

