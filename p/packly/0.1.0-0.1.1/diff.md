# Comparing `tmp/packly-0.1.0.tar.gz` & `tmp/packly-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "packly-0.1.0.tar", max compression
+gzip compressed data, was "packly-0.1.1.tar", max compression
```

## Comparing `packly-0.1.0.tar` & `packly-0.1.1.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0      257 2023-07-02 10:51:05.473626 packly-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-07-02 10:42:32.485175 packly-0.1.0/packly/__init__.py
--rw-r--r--   0        0        0      297 2023-07-02 10:48:45.532823 packly-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      573 1970-01-01 00:00:00.000000 packly-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      524 2023-07-02 11:05:49.863925 packly-0.1.1/README.md
+-rw-r--r--   0        0        0      175 2023-07-02 11:12:21.899661 packly-0.1.1/packly/pk.py
+-rw-r--r--   0        0        0      369 2023-07-02 11:12:36.413029 packly-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      840 1970-01-01 00:00:00.000000 packly-0.1.1/PKG-INFO
```

### Comparing `packly-0.1.0/PKG-INFO` & `packly-0.1.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: packly
-Version: 0.1.0
+Version: 0.1.1
 Summary: Packly makes Python packaging easy
 Author: dylanopen
 Author-email: opendylan@proton.me
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
@@ -13,7 +13,29 @@
 
 Packly is a project designed to help make creating Python packages as easy as possible.
 
 You can add a function at the press of a button, and instantly be coding.
 
 Check out Packly - you'll never want to turn back!
 
+## Installation
+
+You can install Packly using PyPI:
+
+``` sh
+python3 -m pip install packly
+```
+
+Then simply run the `packly` command from your terminal:
+
+``` sh
+packly
+```
+
+You may need to use the `python3 -m` command:
+
+``` sh
+python3 -m packly
+```
+
+Happy packaging!
+
```

