# Comparing `tmp/AileenTestFirstAttempt-0.0.1.tar.gz` & `tmp/AileenTestFirstAttempt-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AileenTestFirstAttempt-0.0.1.tar", last modified: Sun Jul  2 06:15:12 2023, max compression
+gzip compressed data, was "AileenTestFirstAttempt-0.0.2.tar", last modified: Sun Jul  2 06:42:31 2023, max compression
```

## Comparing `AileenTestFirstAttempt-0.0.1.tar` & `AileenTestFirstAttempt-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-02 06:15:12.963282 AileenTestFirstAttempt-0.0.1/
-drwxrwxrwx   0        0        0        0 2023-07-02 06:15:12.946879 AileenTestFirstAttempt-0.0.1/AileenTestFirstAttempt.egg-info/
--rw-rw-rw-   0        0        0      528 2023-07-02 06:15:12.000000 AileenTestFirstAttempt-0.0.1/AileenTestFirstAttempt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      277 2023-07-02 06:15:12.000000 AileenTestFirstAttempt-0.0.1/AileenTestFirstAttempt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-02 06:15:12.000000 AileenTestFirstAttempt-0.0.1/AileenTestFirstAttempt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-07-02 06:15:12.000000 AileenTestFirstAttempt-0.0.1/AileenTestFirstAttempt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-07-02 06:15:12.000000 AileenTestFirstAttempt-0.0.1/AileenTestFirstAttempt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      528 2023-07-02 06:15:12.960281 AileenTestFirstAttempt-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-06-30 23:10:16.000000 AileenTestFirstAttempt-0.0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-07-02 06:15:12.963282 AileenTestFirstAttempt-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      907 2023-07-02 06:14:42.000000 AileenTestFirstAttempt-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-02 06:15:12.955284 AileenTestFirstAttempt-0.0.1/test/
--rw-rw-rw-   0        0        0       20 2023-06-30 23:20:00.000000 AileenTestFirstAttempt-0.0.1/test/__init__.py
--rw-rw-rw-   0        0        0      105 2023-06-30 23:19:24.000000 AileenTestFirstAttempt-0.0.1/test/test.py
+drwxrwxrwx   0        0        0        0 2023-07-02 06:42:31.703312 AileenTestFirstAttempt-0.0.2/
+drwxrwxrwx   0        0        0        0 2023-07-02 06:42:31.688302 AileenTestFirstAttempt-0.0.2/AileenTestFirstAttempt.egg-info/
+-rw-rw-rw-   0        0        0      528 2023-07-02 06:42:31.000000 AileenTestFirstAttempt-0.0.2/AileenTestFirstAttempt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      277 2023-07-02 06:42:31.000000 AileenTestFirstAttempt-0.0.2/AileenTestFirstAttempt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-02 06:42:31.000000 AileenTestFirstAttempt-0.0.2/AileenTestFirstAttempt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-07-02 06:42:31.000000 AileenTestFirstAttempt-0.0.2/AileenTestFirstAttempt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-07-02 06:42:31.000000 AileenTestFirstAttempt-0.0.2/AileenTestFirstAttempt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      528 2023-07-02 06:42:31.702306 AileenTestFirstAttempt-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-06-30 23:10:16.000000 AileenTestFirstAttempt-0.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-02 06:42:31.704306 AileenTestFirstAttempt-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      907 2023-07-02 06:42:24.000000 AileenTestFirstAttempt-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-02 06:42:31.696303 AileenTestFirstAttempt-0.0.2/test/
+-rw-rw-rw-   0        0        0       20 2023-06-30 23:20:00.000000 AileenTestFirstAttempt-0.0.2/test/__init__.py
+-rw-rw-rw-   0        0        0      105 2023-06-30 23:19:24.000000 AileenTestFirstAttempt-0.0.2/test/test.py
```

### Comparing `AileenTestFirstAttempt-0.0.1/AileenTestFirstAttempt.egg-info/PKG-INFO` & `AileenTestFirstAttempt-0.0.2/AileenTestFirstAttempt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AileenTestFirstAttempt
-Version: 0.0.1
+Version: 0.0.2
 Summary: Streaming video data via networks
 Author: Aileen Ouyang
 Author-email: <aileenzouyang@gmail.com >
 Keywords: python,video,stream,video stream,camera stream,sockets
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `AileenTestFirstAttempt-0.0.1/PKG-INFO` & `AileenTestFirstAttempt-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AileenTestFirstAttempt
-Version: 0.0.1
+Version: 0.0.2
 Summary: Streaming video data via networks
 Author: Aileen Ouyang
 Author-email: <aileenzouyang@gmail.com >
 Keywords: python,video,stream,video stream,camera stream,sockets
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `AileenTestFirstAttempt-0.0.1/setup.py` & `AileenTestFirstAttempt-0.0.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = 'Streaming video data via networks'
 LONG_DESCRIPTION = 'A package that allows to build simple streams of video, audio and camera data.'
 
 # Setting up
 setup(
     name="AileenTestFirstAttempt",
     version=VERSION,
```

