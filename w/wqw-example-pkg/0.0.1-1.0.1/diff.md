# Comparing `tmp/wqw_example_pkg-0.0.1.tar.gz` & `tmp/wqw_example_pkg-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wqw_example_pkg-0.0.1.tar", last modified: Sun Jul  2 09:33:34 2023, max compression
+gzip compressed data, was "wqw_example_pkg-1.0.1.tar", last modified: Sun Jul  2 10:13:42 2023, max compression
```

## Comparing `wqw_example_pkg-0.0.1.tar` & `wqw_example_pkg-1.0.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-07-02 09:33:34.592772 wqw_example_pkg-0.0.1/
--rw-rw-rw-   0        0        0     1088 2023-07-02 08:32:59.000000 wqw_example_pkg-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      587 2023-07-02 09:33:34.592772 wqw_example_pkg-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      174 2023-07-02 08:32:17.000000 wqw_example_pkg-0.0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-07-02 09:33:34.593733 wqw_example_pkg-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      629 2023-07-02 09:27:46.000000 wqw_example_pkg-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-02 09:33:34.591738 wqw_example_pkg-0.0.1/wqw_example_pkg.egg-info/
--rw-rw-rw-   0        0        0      587 2023-07-02 09:33:34.000000 wqw_example_pkg-0.0.1/wqw_example_pkg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      182 2023-07-02 09:33:34.000000 wqw_example_pkg-0.0.1/wqw_example_pkg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-02 09:33:34.000000 wqw_example_pkg-0.0.1/wqw_example_pkg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-07-02 09:33:34.000000 wqw_example_pkg-0.0.1/wqw_example_pkg.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-02 10:13:42.581916 wqw_example_pkg-1.0.1/
+-rw-rw-rw-   0        0        0     1088 2023-07-02 08:32:59.000000 wqw_example_pkg-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0      587 2023-07-02 10:13:42.580946 wqw_example_pkg-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      174 2023-07-02 08:32:17.000000 wqw_example_pkg-1.0.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-02 10:13:42.581916 wqw_example_pkg-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      629 2023-07-02 10:13:30.000000 wqw_example_pkg-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-02 10:13:42.579920 wqw_example_pkg-1.0.1/wqw_example_pkg.egg-info/
+-rw-rw-rw-   0        0        0      587 2023-07-02 10:13:42.000000 wqw_example_pkg-1.0.1/wqw_example_pkg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      182 2023-07-02 10:13:42.000000 wqw_example_pkg-1.0.1/wqw_example_pkg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-02 10:13:42.000000 wqw_example_pkg-1.0.1/wqw_example_pkg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-07-02 10:13:42.000000 wqw_example_pkg-1.0.1/wqw_example_pkg.egg-info/top_level.txt
```

### Comparing `wqw_example_pkg-0.0.1/LICENSE` & `wqw_example_pkg-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `wqw_example_pkg-0.0.1/PKG-INFO` & `wqw_example_pkg-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wqw_example_pkg
-Version: 0.0.1
+Version: 1.0.1
 Summary: A test example package
 Home-page: https://github.com/pypa/sampleproject
 Author: MoBot Wang
 Author-email: wangqw1@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `wqw_example_pkg-0.0.1/setup.py` & `wqw_example_pkg-1.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="wqw_example_pkg",
-    version="0.0.1",
+    version="1.0.1",
     author="MoBot Wang",
     author_email="wangqw1@163.com",
     description="A test example package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/pypa/sampleproject",
     packages=setuptools.find_packages(),
```

### Comparing `wqw_example_pkg-0.0.1/wqw_example_pkg.egg-info/PKG-INFO` & `wqw_example_pkg-1.0.1/wqw_example_pkg.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wqw-example-pkg
-Version: 0.0.1
+Version: 1.0.1
 Summary: A test example package
 Home-page: https://github.com/pypa/sampleproject
 Author: MoBot Wang
 Author-email: wangqw1@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

