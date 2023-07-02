# Comparing `tmp/HFODetector-0.0.8.tar.gz` & `tmp/HFODetector-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HFODetector-0.0.8.tar", last modified: Sat Mar  5 04:09:28 2022, max compression
+gzip compressed data, was "HFODetector-0.0.9.tar", last modified: Sat Mar  5 04:35:19 2022, max compression
```

## Comparing `HFODetector-0.0.8.tar` & `HFODetector-0.0.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 taylorchung  (1017) taylorchung  (1017)        0 2022-03-05 04:09:27.993045 HFODetector-0.0.8/
--rw-rw-r--   0 taylorchung  (1017) taylorchung  (1017)        0 2022-03-04 08:00:39.000000 HFODetector-0.0.8/LICENSE
--rw-rw-r--   0 taylorchung  (1017) taylorchung  (1017)       49 2022-03-04 08:24:40.000000 HFODetector-0.0.8/MANIFEST.in
--rw-rw-r--   0 taylorchung  (1017) taylorchung  (1017)      456 2022-03-05 04:09:27.993045 HFODetector-0.0.8/PKG-INFO
--rw-rw-r--   0 taylorchung  (1017) taylorchung  (1017)       29 2022-03-04 08:03:55.000000 HFODetector-0.0.8/README.md
--rw-rw-r--   0 taylorchung  (1017) taylorchung  (1017)      105 2022-03-04 08:03:44.000000 HFODetector-0.0.8/pyproject.toml
--rw-rw-r--   0 taylorchung  (1017) taylorchung  (1017)       38 2022-03-05 04:09:27.993045 HFODetector-0.0.8/setup.cfg
--rw-rw-r--   0 taylorchung  (1017) taylorchung  (1017)      834 2022-03-05 04:09:11.000000 HFODetector-0.0.8/setup.py
-drwxrwxr-x   0 taylorchung  (1017) taylorchung  (1017)        0 2022-03-05 04:09:27.993045 HFODetector-0.0.8/src/
-drwxrwxr-x   0 taylorchung  (1017) taylorchung  (1017)        0 2022-03-05 04:09:27.993045 HFODetector-0.0.8/src/HFODetector/
--rw-rw-r--   0 taylorchung  (1017) taylorchung  (1017)     7638 2022-03-05 03:57:20.000000 HFODetector-0.0.8/src/HFODetector/RMSDetector.py
--rwxrwxr-x   0 taylorchung  (1017) taylorchung  (1017)     5622 2022-03-04 07:59:56.000000 HFODetector-0.0.8/src/HFODetector/SOS.mat
--rw-rw-r--   0 taylorchung  (1017) taylorchung  (1017)        0 2022-03-04 08:09:04.000000 HFODetector-0.0.8/src/HFODetector/__init__.py
--rw-rw-r--   0 taylorchung  (1017) taylorchung  (1017)     7140 2022-03-04 08:18:30.000000 HFODetector-0.0.8/src/HFODetector/utils.py
-drwxrwxr-x   0 taylorchung  (1017) taylorchung  (1017)        0 2022-03-05 04:09:27.993045 HFODetector-0.0.8/src/HFODetector.egg-info/
--rw-rw-r--   0 taylorchung  (1017) taylorchung  (1017)      456 2022-03-05 04:09:27.000000 HFODetector-0.0.8/src/HFODetector.egg-info/PKG-INFO
--rw-rw-r--   0 taylorchung  (1017) taylorchung  (1017)      355 2022-03-05 04:09:27.000000 HFODetector-0.0.8/src/HFODetector.egg-info/SOURCES.txt
--rw-rw-r--   0 taylorchung  (1017) taylorchung  (1017)        1 2022-03-05 04:09:27.000000 HFODetector-0.0.8/src/HFODetector.egg-info/dependency_links.txt
--rw-rw-r--   0 taylorchung  (1017) taylorchung  (1017)       34 2022-03-05 04:09:27.000000 HFODetector-0.0.8/src/HFODetector.egg-info/requires.txt
--rw-rw-r--   0 taylorchung  (1017) taylorchung  (1017)       12 2022-03-05 04:09:27.000000 HFODetector-0.0.8/src/HFODetector.egg-info/top_level.txt
+drwxrwxr-x   0 taylorchung  (1017) taylorchung  (1017)        0 2022-03-05 04:35:19.416707 HFODetector-0.0.9/
+-rw-rw-r--   0 taylorchung  (1017) taylorchung  (1017)        0 2022-03-04 08:00:39.000000 HFODetector-0.0.9/LICENSE
+-rw-rw-r--   0 taylorchung  (1017) taylorchung  (1017)       49 2022-03-04 08:24:40.000000 HFODetector-0.0.9/MANIFEST.in
+-rw-rw-r--   0 taylorchung  (1017) taylorchung  (1017)     1106 2022-03-05 04:35:19.416707 HFODetector-0.0.9/PKG-INFO
+-rw-rw-r--   0 taylorchung  (1017) taylorchung  (1017)      679 2022-03-05 04:34:55.000000 HFODetector-0.0.9/README.md
+-rw-rw-r--   0 taylorchung  (1017) taylorchung  (1017)      105 2022-03-04 08:03:44.000000 HFODetector-0.0.9/pyproject.toml
+-rw-rw-r--   0 taylorchung  (1017) taylorchung  (1017)       38 2022-03-05 04:35:19.416707 HFODetector-0.0.9/setup.cfg
+-rw-rw-r--   0 taylorchung  (1017) taylorchung  (1017)      834 2022-03-05 04:35:02.000000 HFODetector-0.0.9/setup.py
+drwxrwxr-x   0 taylorchung  (1017) taylorchung  (1017)        0 2022-03-05 04:35:19.416707 HFODetector-0.0.9/src/
+drwxrwxr-x   0 taylorchung  (1017) taylorchung  (1017)        0 2022-03-05 04:35:19.416707 HFODetector-0.0.9/src/HFODetector/
+-rw-rw-r--   0 taylorchung  (1017) taylorchung  (1017)     7638 2022-03-05 03:57:20.000000 HFODetector-0.0.9/src/HFODetector/RMSDetector.py
+-rwxrwxr-x   0 taylorchung  (1017) taylorchung  (1017)     5622 2022-03-04 07:59:56.000000 HFODetector-0.0.9/src/HFODetector/SOS.mat
+-rw-rw-r--   0 taylorchung  (1017) taylorchung  (1017)        0 2022-03-04 08:09:04.000000 HFODetector-0.0.9/src/HFODetector/__init__.py
+-rw-rw-r--   0 taylorchung  (1017) taylorchung  (1017)     7140 2022-03-04 08:18:30.000000 HFODetector-0.0.9/src/HFODetector/utils.py
+drwxrwxr-x   0 taylorchung  (1017) taylorchung  (1017)        0 2022-03-05 04:35:19.416707 HFODetector-0.0.9/src/HFODetector.egg-info/
+-rw-rw-r--   0 taylorchung  (1017) taylorchung  (1017)     1106 2022-03-05 04:35:19.000000 HFODetector-0.0.9/src/HFODetector.egg-info/PKG-INFO
+-rw-rw-r--   0 taylorchung  (1017) taylorchung  (1017)      355 2022-03-05 04:35:19.000000 HFODetector-0.0.9/src/HFODetector.egg-info/SOURCES.txt
+-rw-rw-r--   0 taylorchung  (1017) taylorchung  (1017)        1 2022-03-05 04:35:19.000000 HFODetector-0.0.9/src/HFODetector.egg-info/dependency_links.txt
+-rw-rw-r--   0 taylorchung  (1017) taylorchung  (1017)       34 2022-03-05 04:35:19.000000 HFODetector-0.0.9/src/HFODetector.egg-info/requires.txt
+-rw-rw-r--   0 taylorchung  (1017) taylorchung  (1017)       12 2022-03-05 04:35:19.000000 HFODetector-0.0.9/src/HFODetector.egg-info/top_level.txt
```

### Comparing `HFODetector-0.0.8/setup.py` & `HFODetector-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="HFODetector",
-    version="0.0.8",
+    version="0.0.9",
     author="Taylor Chung",
     author_email="taylorchung@ucla.edu",
     description="Package for detecing HFOs",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     project_urls={ },
```

### Comparing `HFODetector-0.0.8/src/HFODetector/RMSDetector.py` & `HFODetector-0.0.9/src/HFODetector/RMSDetector.py`

 * *Files identical despite different names*

### Comparing `HFODetector-0.0.8/src/HFODetector/SOS.mat` & `HFODetector-0.0.9/src/HFODetector/SOS.mat`

 * *Files identical despite different names*

### Comparing `HFODetector-0.0.8/src/HFODetector/utils.py` & `HFODetector-0.0.9/src/HFODetector/utils.py`

 * *Files identical despite different names*

