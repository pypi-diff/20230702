# Comparing `tmp/aws-vpclattice-prealpha-0.0.3.tar.gz` & `tmp/aws-vpclattice-prealpha-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws-vpclattice-prealpha-0.0.3.tar", last modified: Sun Jul  2 09:29:58 2023, max compression
+gzip compressed data, was "aws-vpclattice-prealpha-0.0.4.tar", last modified: Sun Jul  2 09:36:52 2023, max compression
```

## Comparing `aws-vpclattice-prealpha-0.0.3.tar` & `aws-vpclattice-prealpha-0.0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:29:58.383065 aws-vpclattice-prealpha-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-02 09:29:46.000000 aws-vpclattice-prealpha-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-02 09:29:46.000000 aws-vpclattice-prealpha-0.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-07-02 09:29:58.383065 aws-vpclattice-prealpha-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-02 09:29:46.000000 aws-vpclattice-prealpha-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-02 09:29:46.000000 aws-vpclattice-prealpha-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 09:29:58.383065 aws-vpclattice-prealpha-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-07-02 09:29:46.000000 aws-vpclattice-prealpha-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:29:58.383065 aws-vpclattice-prealpha-0.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:29:58.383065 aws-vpclattice-prealpha-0.0.3/src/aws_vpclattice_prealpha.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-07-02 09:29:58.000000 aws-vpclattice-prealpha-0.0.3/src/aws_vpclattice_prealpha.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-07-02 09:29:58.000000 aws-vpclattice-prealpha-0.0.3/src/aws_vpclattice_prealpha.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 09:29:58.000000 aws-vpclattice-prealpha-0.0.3/src/aws_vpclattice_prealpha.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-02 09:29:58.000000 aws-vpclattice-prealpha-0.0.3/src/aws_vpclattice_prealpha.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-02 09:29:58.000000 aws-vpclattice-prealpha-0.0.3/src/aws_vpclattice_prealpha.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:29:58.383065 aws-vpclattice-prealpha-0.0.3/src/vpc_lattice/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:29:58.383065 aws-vpclattice-prealpha-0.0.3/src/vpc_lattice/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-07-02 09:29:46.000000 aws-vpclattice-prealpha-0.0.3/src/vpc_lattice/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12804 2023-07-02 09:29:46.000000 aws-vpclattice-prealpha-0.0.3/src/vpc_lattice/_jsii/aws-vpclattice-prealpha@0.0.3.jsii.tgz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:36:52.455073 aws-vpclattice-prealpha-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-02 09:36:37.000000 aws-vpclattice-prealpha-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-02 09:36:37.000000 aws-vpclattice-prealpha-0.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-07-02 09:36:52.455073 aws-vpclattice-prealpha-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-02 09:36:37.000000 aws-vpclattice-prealpha-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-02 09:36:37.000000 aws-vpclattice-prealpha-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 09:36:52.455073 aws-vpclattice-prealpha-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-07-02 09:36:37.000000 aws-vpclattice-prealpha-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:36:52.451074 aws-vpclattice-prealpha-0.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:36:52.451074 aws-vpclattice-prealpha-0.0.4/src/aws_vpclattice_prealpha.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-07-02 09:36:52.000000 aws-vpclattice-prealpha-0.0.4/src/aws_vpclattice_prealpha.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-07-02 09:36:52.000000 aws-vpclattice-prealpha-0.0.4/src/aws_vpclattice_prealpha.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 09:36:52.000000 aws-vpclattice-prealpha-0.0.4/src/aws_vpclattice_prealpha.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-02 09:36:52.000000 aws-vpclattice-prealpha-0.0.4/src/aws_vpclattice_prealpha.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-02 09:36:52.000000 aws-vpclattice-prealpha-0.0.4/src/aws_vpclattice_prealpha.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:36:52.451074 aws-vpclattice-prealpha-0.0.4/src/vpc_lattice/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:36:52.451074 aws-vpclattice-prealpha-0.0.4/src/vpc_lattice/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-07-02 09:36:37.000000 aws-vpclattice-prealpha-0.0.4/src/vpc_lattice/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12802 2023-07-02 09:36:37.000000 aws-vpclattice-prealpha-0.0.4/src/vpc_lattice/_jsii/aws-vpclattice-prealpha@0.0.4.jsii.tgz
```

### Comparing `aws-vpclattice-prealpha-0.0.3/LICENSE` & `aws-vpclattice-prealpha-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `aws-vpclattice-prealpha-0.0.3/PKG-INFO` & `aws-vpclattice-prealpha-0.0.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-vpclattice-prealpha
-Version: 0.0.3
+Version: 0.0.4
 Summary: aws-vpclattice-prealpha
 Home-page: https://github.com/raindancers/aws-vpclattice-prealpha.git
 Author: Andrew Frazer<andrew.frazer@raindancers.cloud>
 License: Apache-2.0
 Project-URL: Source, https://github.com/raindancers/aws-vpclattice-prealpha.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `aws-vpclattice-prealpha-0.0.3/setup.py` & `aws-vpclattice-prealpha-0.0.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "aws-vpclattice-prealpha",
-    "version": "0.0.3",
+    "version": "0.0.4",
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
-            "aws-vpclattice-prealpha@0.0.3.jsii.tgz"
+            "aws-vpclattice-prealpha@0.0.4.jsii.tgz"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
         "aws-cdk-lib>=2.80.0, <3.0.0",
         "constructs>=10.0.5, <11.0.0",
         "jsii>=1.84.0, <2.0.0",
```

### Comparing `aws-vpclattice-prealpha-0.0.3/src/aws_vpclattice_prealpha.egg-info/PKG-INFO` & `aws-vpclattice-prealpha-0.0.4/src/aws_vpclattice_prealpha.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-vpclattice-prealpha
-Version: 0.0.3
+Version: 0.0.4
 Summary: aws-vpclattice-prealpha
 Home-page: https://github.com/raindancers/aws-vpclattice-prealpha.git
 Author: Andrew Frazer<andrew.frazer@raindancers.cloud>
 License: Apache-2.0
 Project-URL: Source, https://github.com/raindancers/aws-vpclattice-prealpha.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

