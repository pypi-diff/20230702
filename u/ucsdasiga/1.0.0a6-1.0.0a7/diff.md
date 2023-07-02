# Comparing `tmp/ucsdasiga-1.0.0a6.tar.gz` & `tmp/ucsdasiga-1.0.0a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ucsdasiga-1.0.0a6.tar", last modified: Thu Apr 27 22:42:37 2023, max compression
+gzip compressed data, was "ucsdasiga-1.0.0a7.tar", last modified: Sun Jul  2 16:55:19 2023, max compression
```

## Comparing `ucsdasiga-1.0.0a6.tar` & `ucsdasiga-1.0.0a7.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-27 22:42:37.881288 ucsdasiga-1.0.0a6/
--rw-rw-rw-   0        0        0     1087 2023-04-26 02:03:10.000000 ucsdasiga-1.0.0a6/LICENSE
--rw-rw-rw-   0        0        0     8465 2023-04-27 22:42:37.880273 ucsdasiga-1.0.0a6/PKG-INFO
--rw-rw-rw-   0        0        0     6235 2023-04-27 20:14:28.000000 ucsdasiga-1.0.0a6/README.md
-drwxrwxrwx   0        0        0        0 2023-04-27 22:42:37.826640 ucsdasiga-1.0.0a6/asiga/
--rw-rw-rw-   0        0        0     1692 2023-04-27 20:14:28.000000 ucsdasiga-1.0.0a6/asiga/__init__.py
--rw-rw-rw-   0        0        0       64 2023-04-26 03:35:05.000000 ucsdasiga-1.0.0a6/asiga/__main__.py
--rw-rw-rw-   0        0        0     2413 2023-04-27 20:14:28.000000 ucsdasiga-1.0.0a6/asiga/scraper.py
--rw-rw-rw-   0        0        0     1117 2023-04-27 22:40:53.000000 ucsdasiga-1.0.0a6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-27 22:42:37.881288 ucsdasiga-1.0.0a6/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-27 22:42:37.878567 ucsdasiga-1.0.0a6/ucsdasiga.egg-info/
--rw-rw-rw-   0        0        0     8465 2023-04-27 22:42:37.000000 ucsdasiga-1.0.0a6/ucsdasiga.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      217 2023-04-27 22:42:37.000000 ucsdasiga-1.0.0a6/ucsdasiga.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-27 22:42:37.000000 ucsdasiga-1.0.0a6/ucsdasiga.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-04-27 22:42:37.000000 ucsdasiga-1.0.0a6/ucsdasiga.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-02 16:55:19.591250 ucsdasiga-1.0.0a7/
+-rw-rw-rw-   0        0        0     1087 2023-04-26 02:03:10.000000 ucsdasiga-1.0.0a7/LICENSE
+-rw-rw-rw-   0        0        0     8364 2023-07-02 16:55:19.575641 ucsdasiga-1.0.0a7/PKG-INFO
+-rw-rw-rw-   0        0        0     6235 2023-04-27 22:45:21.000000 ucsdasiga-1.0.0a7/README.md
+drwxrwxrwx   0        0        0        0 2023-07-02 16:55:19.519145 ucsdasiga-1.0.0a7/asiga/
+-rw-rw-rw-   0        0        0      361 2023-07-02 16:53:39.000000 ucsdasiga-1.0.0a7/asiga/__init__.py
+-rw-rw-rw-   0        0        0       64 2023-04-27 22:45:21.000000 ucsdasiga-1.0.0a7/asiga/__main__.py
+-rw-rw-rw-   0        0        0     6294 2023-07-02 16:53:39.000000 ucsdasiga-1.0.0a7/asiga/scraper.py
+-rw-rw-rw-   0        0        0     1628 2023-07-02 16:53:43.000000 ucsdasiga-1.0.0a7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-02 16:55:19.591250 ucsdasiga-1.0.0a7/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-02 16:55:19.575641 ucsdasiga-1.0.0a7/ucsdasiga.egg-info/
+-rw-rw-rw-   0        0        0     8364 2023-07-02 16:55:19.000000 ucsdasiga-1.0.0a7/ucsdasiga.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      249 2023-07-02 16:55:19.000000 ucsdasiga-1.0.0a7/ucsdasiga.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-02 16:55:19.000000 ucsdasiga-1.0.0a7/ucsdasiga.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      433 2023-07-02 16:55:19.000000 ucsdasiga-1.0.0a7/ucsdasiga.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-02 16:55:19.000000 ucsdasiga-1.0.0a7/ucsdasiga.egg-info/top_level.txt
```

### Comparing `ucsdasiga-1.0.0a6/LICENSE` & `ucsdasiga-1.0.0a7/LICENSE`

 * *Files identical despite different names*

### Comparing `ucsdasiga-1.0.0a6/PKG-INFO` & `ucsdasiga-1.0.0a7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ucsdasiga
-Version: 1.0.0a6
+Version: 1.0.0a7
 Summary: A simple API wrapper and web scraper for the UCSD Associated Students (AS) instructor grade archive.
 Author-email: Jacob Lee <Jacob.J.Lee@outlook.com>
 License: MIT License
         
         Copyright (c) 2023 Jacob Lee
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -28,21 +28,19 @@
 Project-URL: homepage, https://github.com/JacobLee23/UCSD-AS-One
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.5
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # UCSD Associated Students (AS) Instructor Grade Archive (IGA)
 
 ![GitHub Pipenv locked Python version](https://img.shields.io/github/pipenv/locked/python-version/JacobLee23/UCSD-AS-IGA)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/ucsdasiga)](https://pypi.org/project/ucsdasiga)
```

### Comparing `ucsdasiga-1.0.0a6/README.md` & `ucsdasiga-1.0.0a7/README.md`

 * *Files identical despite different names*

### Comparing `ucsdasiga-1.0.0a6/ucsdasiga.egg-info/PKG-INFO` & `ucsdasiga-1.0.0a7/ucsdasiga.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ucsdasiga
-Version: 1.0.0a6
+Version: 1.0.0a7
 Summary: A simple API wrapper and web scraper for the UCSD Associated Students (AS) instructor grade archive.
 Author-email: Jacob Lee <Jacob.J.Lee@outlook.com>
 License: MIT License
         
         Copyright (c) 2023 Jacob Lee
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -28,21 +28,19 @@
 Project-URL: homepage, https://github.com/JacobLee23/UCSD-AS-One
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.5
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # UCSD Associated Students (AS) Instructor Grade Archive (IGA)
 
 ![GitHub Pipenv locked Python version](https://img.shields.io/github/pipenv/locked/python-version/JacobLee23/UCSD-AS-IGA)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/ucsdasiga)](https://pypi.org/project/ucsdasiga)
```

