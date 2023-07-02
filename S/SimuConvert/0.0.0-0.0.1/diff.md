# Comparing `tmp/SimuConvert-0.0.0.tar.gz` & `tmp/SimuConvert-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SimuConvert-0.0.0.tar", last modified: Sat Jul  1 11:23:42 2023, max compression
+gzip compressed data, was "SimuConvert-0.0.1.tar", last modified: Sun Jul  2 12:26:17 2023, max compression
```

## Comparing `SimuConvert-0.0.0.tar` & `SimuConvert-0.0.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 yanzhonghuang   (501) staff       (20)        0 2023-07-01 11:23:42.107677 SimuConvert-0.0.0/
--rw-r--r--   0 yanzhonghuang   (501) staff       (20)     1071 2023-07-01 08:02:44.000000 SimuConvert-0.0.0/LICENSE
--rw-r--r--   0 yanzhonghuang   (501) staff       (20)      932 2023-07-01 11:23:42.107548 SimuConvert-0.0.0/PKG-INFO
--rw-r--r--   0 yanzhonghuang   (501) staff       (20)      480 2023-07-01 08:55:36.000000 SimuConvert-0.0.0/README.md
-drwxr-xr-x   0 yanzhonghuang   (501) staff       (20)        0 2023-07-01 11:23:42.106214 SimuConvert-0.0.0/SimuConvert/
-drwxr-xr-x   0 yanzhonghuang   (501) staff       (20)        0 2023-07-01 11:23:42.107347 SimuConvert-0.0.0/SimuConvert/SimuConvert.egg-info/
--rw-r--r--   0 yanzhonghuang   (501) staff       (20)      932 2023-07-01 11:23:42.000000 SimuConvert-0.0.0/SimuConvert/SimuConvert.egg-info/PKG-INFO
--rw-r--r--   0 yanzhonghuang   (501) staff       (20)      260 2023-07-01 11:23:42.000000 SimuConvert-0.0.0/SimuConvert/SimuConvert.egg-info/SOURCES.txt
--rw-r--r--   0 yanzhonghuang   (501) staff       (20)        1 2023-07-01 11:23:42.000000 SimuConvert-0.0.0/SimuConvert/SimuConvert.egg-info/dependency_links.txt
--rw-r--r--   0 yanzhonghuang   (501) staff       (20)       62 2023-07-01 11:23:42.000000 SimuConvert-0.0.0/SimuConvert/SimuConvert.egg-info/requires.txt
--rw-r--r--   0 yanzhonghuang   (501) staff       (20)        1 2023-07-01 11:23:42.000000 SimuConvert-0.0.0/SimuConvert/SimuConvert.egg-info/top_level.txt
--rw-r--r--   0 yanzhonghuang   (501) staff       (20)       38 2023-07-01 11:23:42.107717 SimuConvert-0.0.0/setup.cfg
--rw-r--r--   0 yanzhonghuang   (501) staff       (20)      907 2023-07-01 11:20:00.000000 SimuConvert-0.0.0/setup.py
+drwxr-xr-x   0 yanzhonghuang   (501) staff       (20)        0 2023-07-02 12:26:17.142136 SimuConvert-0.0.1/
+-rw-r--r--   0 yanzhonghuang   (501) staff       (20)     1071 2023-07-01 08:02:44.000000 SimuConvert-0.0.1/LICENSE
+-rw-r--r--   0 yanzhonghuang   (501) staff       (20)      932 2023-07-02 12:26:17.142003 SimuConvert-0.0.1/PKG-INFO
+-rw-r--r--   0 yanzhonghuang   (501) staff       (20)      480 2023-07-01 08:55:36.000000 SimuConvert-0.0.1/README.md
+drwxr-xr-x   0 yanzhonghuang   (501) staff       (20)        0 2023-07-02 12:26:17.140650 SimuConvert-0.0.1/SimuConvert/
+drwxr-xr-x   0 yanzhonghuang   (501) staff       (20)        0 2023-07-02 12:26:17.141822 SimuConvert-0.0.1/SimuConvert/SimuConvert.egg-info/
+-rw-r--r--   0 yanzhonghuang   (501) staff       (20)      932 2023-07-02 12:26:17.000000 SimuConvert-0.0.1/SimuConvert/SimuConvert.egg-info/PKG-INFO
+-rw-r--r--   0 yanzhonghuang   (501) staff       (20)      260 2023-07-02 12:26:17.000000 SimuConvert-0.0.1/SimuConvert/SimuConvert.egg-info/SOURCES.txt
+-rw-r--r--   0 yanzhonghuang   (501) staff       (20)        1 2023-07-02 12:26:17.000000 SimuConvert-0.0.1/SimuConvert/SimuConvert.egg-info/dependency_links.txt
+-rw-r--r--   0 yanzhonghuang   (501) staff       (20)       62 2023-07-02 12:26:17.000000 SimuConvert-0.0.1/SimuConvert/SimuConvert.egg-info/requires.txt
+-rw-r--r--   0 yanzhonghuang   (501) staff       (20)        1 2023-07-02 12:26:17.000000 SimuConvert-0.0.1/SimuConvert/SimuConvert.egg-info/top_level.txt
+-rw-r--r--   0 yanzhonghuang   (501) staff       (20)       38 2023-07-02 12:26:17.142177 SimuConvert-0.0.1/setup.cfg
+-rw-r--r--   0 yanzhonghuang   (501) staff       (20)      907 2023-07-02 12:26:04.000000 SimuConvert-0.0.1/setup.py
```

### Comparing `SimuConvert-0.0.0/LICENSE` & `SimuConvert-0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `SimuConvert-0.0.0/PKG-INFO` & `SimuConvert-0.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SimuConvert
-Version: 0.0.0
+Version: 0.0.1
 Summary: A package for converting private fund equity data 
 Home-page: https://github.com/Yanzhong-Hub/SimuConvert
 Author: Yanzhong Huang
 Author-email: yanzhong.huang@outlook.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `SimuConvert-0.0.0/SimuConvert/SimuConvert.egg-info/PKG-INFO` & `SimuConvert-0.0.1/SimuConvert/SimuConvert.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SimuConvert
-Version: 0.0.0
+Version: 0.0.1
 Summary: A package for converting private fund equity data 
 Home-page: https://github.com/Yanzhong-Hub/SimuConvert
 Author: Yanzhong Huang
 Author-email: yanzhong.huang@outlook.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `SimuConvert-0.0.0/setup.py` & `SimuConvert-0.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="SimuConvert",
-    version="0.0.0",
+    version="0.0.1",
     author="Yanzhong Huang",
     author_email="yanzhong.huang@outlook.com",
     description="A package for converting private fund equity data ",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Yanzhong-Hub/SimuConvert",
     package_dir={"": "SimuConvert"},
```

