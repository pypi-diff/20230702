# Comparing `tmp/wqw_example_pkg-3.0.1.tar.gz` & `tmp/wqw_example_pkg-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wqw_example_pkg-3.0.1.tar", last modified: Sun Jul  2 10:39:10 2023, max compression
+gzip compressed data, was "wqw_example_pkg-4.0.1.tar", last modified: Sun Jul  2 10:53:18 2023, max compression
```

## Comparing `wqw_example_pkg-3.0.1.tar` & `wqw_example_pkg-4.0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-02 10:39:10.210440 wqw_example_pkg-3.0.1/
--rw-rw-rw-   0        0        0     1088 2023-07-02 08:32:59.000000 wqw_example_pkg-3.0.1/LICENSE
--rw-rw-rw-   0        0        0      587 2023-07-02 10:39:10.210440 wqw_example_pkg-3.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      174 2023-07-02 08:32:17.000000 wqw_example_pkg-3.0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-07-02 10:39:10.211438 wqw_example_pkg-3.0.1/setup.cfg
--rw-rw-rw-   0        0        0      629 2023-07-02 10:39:07.000000 wqw_example_pkg-3.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-02 10:39:10.204457 wqw_example_pkg-3.0.1/wqw_example_pkg/
--rw-rw-rw-   0        0        0       20 2023-07-02 01:21:42.000000 wqw_example_pkg-3.0.1/wqw_example_pkg/__init__.py
--rw-rw-rw-   0        0        0       38 2023-07-02 08:36:00.000000 wqw_example_pkg-3.0.1/wqw_example_pkg/addSome.py
-drwxrwxrwx   0        0        0        0 2023-07-02 10:39:10.208447 wqw_example_pkg-3.0.1/wqw_example_pkg.egg-info/
--rw-rw-rw-   0        0        0      587 2023-07-02 10:39:10.000000 wqw_example_pkg-3.0.1/wqw_example_pkg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      237 2023-07-02 10:39:10.000000 wqw_example_pkg-3.0.1/wqw_example_pkg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-02 10:39:10.000000 wqw_example_pkg-3.0.1/wqw_example_pkg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-07-02 10:39:10.000000 wqw_example_pkg-3.0.1/wqw_example_pkg.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-02 10:53:18.487289 wqw_example_pkg-4.0.1/
+-rw-rw-rw-   0        0        0     1088 2023-07-02 08:32:59.000000 wqw_example_pkg-4.0.1/LICENSE
+-rw-rw-rw-   0        0        0      587 2023-07-02 10:53:18.486319 wqw_example_pkg-4.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      174 2023-07-02 08:32:17.000000 wqw_example_pkg-4.0.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-02 10:53:18.488289 wqw_example_pkg-4.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      629 2023-07-02 10:51:38.000000 wqw_example_pkg-4.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-02 10:53:18.476324 wqw_example_pkg-4.0.1/wqw_example_pkg/
+-rw-rw-rw-   0        0        0       20 2023-07-02 01:21:42.000000 wqw_example_pkg-4.0.1/wqw_example_pkg/__init__.py
+-rw-rw-rw-   0        0        0       38 2023-07-02 08:36:00.000000 wqw_example_pkg-4.0.1/wqw_example_pkg/test.py
+drwxrwxrwx   0        0        0        0 2023-07-02 10:53:18.484298 wqw_example_pkg-4.0.1/wqw_example_pkg.egg-info/
+-rw-rw-rw-   0        0        0      587 2023-07-02 10:53:18.000000 wqw_example_pkg-4.0.1/wqw_example_pkg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      234 2023-07-02 10:53:18.000000 wqw_example_pkg-4.0.1/wqw_example_pkg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-02 10:53:18.000000 wqw_example_pkg-4.0.1/wqw_example_pkg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-07-02 10:53:18.000000 wqw_example_pkg-4.0.1/wqw_example_pkg.egg-info/top_level.txt
```

### Comparing `wqw_example_pkg-3.0.1/LICENSE` & `wqw_example_pkg-4.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `wqw_example_pkg-3.0.1/PKG-INFO` & `wqw_example_pkg-4.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wqw_example_pkg
-Version: 3.0.1
+Version: 4.0.1
 Summary: A test example package
 Home-page: https://github.com/pypa/sampleproject
 Author: MoBot Wang
 Author-email: wangqw1@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `wqw_example_pkg-3.0.1/setup.py` & `wqw_example_pkg-4.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="wqw_example_pkg",
-    version="3.0.1",
+    version="4.0.1",
     author="MoBot Wang",
     author_email="wangqw1@163.com",
     description="A test example package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/pypa/sampleproject",
     packages=setuptools.find_packages(),
```

### Comparing `wqw_example_pkg-3.0.1/wqw_example_pkg.egg-info/PKG-INFO` & `wqw_example_pkg-4.0.1/wqw_example_pkg.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wqw-example-pkg
-Version: 3.0.1
+Version: 4.0.1
 Summary: A test example package
 Home-page: https://github.com/pypa/sampleproject
 Author: MoBot Wang
 Author-email: wangqw1@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

