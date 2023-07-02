# Comparing `tmp/reliableGPT-0.2.956.tar.gz` & `tmp/reliableGPT-0.2.957.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reliableGPT-0.2.956.tar", last modified: Sun Jul  2 04:04:17 2023, max compression
+gzip compressed data, was "reliableGPT-0.2.957.tar", last modified: Sun Jul  2 04:14:13 2023, max compression
```

## Comparing `reliableGPT-0.2.956.tar` & `reliableGPT-0.2.957.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-07-02 04:04:17.375158 reliableGPT-0.2.956/
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     1065 2023-06-23 13:49:22.000000 reliableGPT-0.2.956/LICENSE
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      156 2023-07-02 04:04:17.375044 reliableGPT-0.2.956/PKG-INFO
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     6254 2023-07-01 20:41:40.000000 reliableGPT-0.2.956/README.md
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      497 2023-06-29 02:51:34.000000 reliableGPT-0.2.956/pyproject.toml
-drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-07-02 04:04:17.372668 reliableGPT-0.2.956/reliableGPT.egg-info/
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      156 2023-07-02 04:04:17.000000 reliableGPT-0.2.956/reliableGPT.egg-info/PKG-INFO
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      485 2023-07-02 04:04:17.000000 reliableGPT-0.2.956/reliableGPT.egg-info/SOURCES.txt
--rw-r--r--   0 krrishdholakia   (501) staff       (20)        1 2023-07-02 04:04:17.000000 reliableGPT-0.2.956/reliableGPT.egg-info/dependency_links.txt
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      113 2023-07-02 04:04:17.000000 reliableGPT-0.2.956/reliableGPT.egg-info/requires.txt
--rw-r--r--   0 krrishdholakia   (501) staff       (20)       12 2023-07-02 04:04:17.000000 reliableGPT-0.2.956/reliableGPT.egg-info/top_level.txt
-drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-07-02 04:04:17.374829 reliableGPT-0.2.956/reliablegpt/
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     4210 2023-06-29 02:51:34.000000 reliableGPT-0.2.956/reliablegpt/APICallHandler.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     3120 2023-07-01 20:41:27.000000 reliableGPT-0.2.956/reliablegpt/Alerting.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     4407 2023-06-29 02:51:34.000000 reliableGPT-0.2.956/reliablegpt/CustomQueue.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)    11224 2023-07-01 20:41:40.000000 reliableGPT-0.2.956/reliablegpt/IndividualRequest.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     1286 2023-07-01 20:41:40.000000 reliableGPT-0.2.956/reliablegpt/Model.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     5195 2023-07-01 20:41:27.000000 reliableGPT-0.2.956/reliablegpt/RateLimitHandler.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     6398 2023-07-02 03:58:41.000000 reliableGPT-0.2.956/reliablegpt/ReliableDataLoaders.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      374 2023-07-01 20:43:51.000000 reliableGPT-0.2.956/reliablegpt/__init__.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     3921 2023-07-01 20:41:40.000000 reliableGPT-0.2.956/reliablegpt/main.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)       38 2023-07-02 04:04:17.375198 reliableGPT-0.2.956/setup.cfg
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      524 2023-07-02 04:04:14.000000 reliableGPT-0.2.956/setup.py
+drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-07-02 04:14:13.458633 reliableGPT-0.2.957/
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)     1065 2023-06-23 13:49:22.000000 reliableGPT-0.2.957/LICENSE
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)      156 2023-07-02 04:14:13.458511 reliableGPT-0.2.957/PKG-INFO
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)     6254 2023-07-01 20:41:40.000000 reliableGPT-0.2.957/README.md
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)      497 2023-06-29 02:51:34.000000 reliableGPT-0.2.957/pyproject.toml
+drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-07-02 04:14:13.457103 reliableGPT-0.2.957/reliableGPT.egg-info/
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)      156 2023-07-02 04:14:13.000000 reliableGPT-0.2.957/reliableGPT.egg-info/PKG-INFO
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)      485 2023-07-02 04:14:13.000000 reliableGPT-0.2.957/reliableGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)        1 2023-07-02 04:14:13.000000 reliableGPT-0.2.957/reliableGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)       54 2023-07-02 04:14:13.000000 reliableGPT-0.2.957/reliableGPT.egg-info/requires.txt
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)       12 2023-07-02 04:14:13.000000 reliableGPT-0.2.957/reliableGPT.egg-info/top_level.txt
+drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-07-02 04:14:13.458323 reliableGPT-0.2.957/reliablegpt/
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)     4210 2023-06-29 02:51:34.000000 reliableGPT-0.2.957/reliablegpt/APICallHandler.py
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)     3120 2023-07-02 04:13:32.000000 reliableGPT-0.2.957/reliablegpt/Alerting.py
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)     4407 2023-06-29 02:51:34.000000 reliableGPT-0.2.957/reliablegpt/CustomQueue.py
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)    11224 2023-07-01 20:41:40.000000 reliableGPT-0.2.957/reliablegpt/IndividualRequest.py
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)     1286 2023-07-01 20:41:40.000000 reliableGPT-0.2.957/reliablegpt/Model.py
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)     5195 2023-07-01 20:41:27.000000 reliableGPT-0.2.957/reliablegpt/RateLimitHandler.py
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)     7119 2023-07-02 04:12:52.000000 reliableGPT-0.2.957/reliablegpt/ReliableDataLoaders.py
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)      374 2023-07-01 20:43:51.000000 reliableGPT-0.2.957/reliablegpt/__init__.py
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)     3921 2023-07-01 20:41:40.000000 reliableGPT-0.2.957/reliablegpt/main.py
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)       38 2023-07-02 04:14:13.458673 reliableGPT-0.2.957/setup.cfg
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)      398 2023-07-02 04:14:03.000000 reliableGPT-0.2.957/setup.py
```

### Comparing `reliableGPT-0.2.956/LICENSE` & `reliableGPT-0.2.957/LICENSE`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.956/README.md` & `reliableGPT-0.2.957/README.md`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.956/reliablegpt/APICallHandler.py` & `reliableGPT-0.2.957/reliablegpt/APICallHandler.py`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.956/reliablegpt/Alerting.py` & `reliableGPT-0.2.957/reliablegpt/Alerting.py`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.956/reliablegpt/CustomQueue.py` & `reliableGPT-0.2.957/reliablegpt/CustomQueue.py`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.956/reliablegpt/IndividualRequest.py` & `reliableGPT-0.2.957/reliablegpt/IndividualRequest.py`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.956/reliablegpt/Model.py` & `reliableGPT-0.2.957/reliablegpt/Model.py`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.956/reliablegpt/RateLimitHandler.py` & `reliableGPT-0.2.957/reliablegpt/RateLimitHandler.py`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.956/reliablegpt/ReliableDataLoaders.py` & `reliableGPT-0.2.957/reliablegpt/ReliableDataLoaders.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,33 @@
+import subprocess
+
+# Libraries to install
+packages = ['langchain', 'resend', 'pypdf', 'pymupdf', 'pdfminer', 'pdfminer.six', 'unstructured']
+
+# Try importing the libraries
+try:
+    import langchain
+    import resend
+    import pypdf
+    import pymupdf
+    import pdfminer
+    import pdfminer.six
+    import unstructured
+except ImportError as e:
+    print(f"Import error: {e}")
+    print("Installing required packages...")
+
+    # Install missing packages using pip
+    for package in packages:
+        try:
+            subprocess.check_call(['pip', 'install', package])
+            print(f"Successfully installed {package}")
+        except subprocess.CalledProcessError:
+            print(f"Failed to install {package}")
+
 from typing import Any
 from functools import wraps
 from langchain.document_loaders.pdf import (PyMuPDFLoader, PDFMinerLoader, PyPDFLoader, OnlinePDFLoader)
 from langchain.document_loaders.csv_loader import CSVLoader
 from langchain.document_loaders import UnstructuredURLLoader
 import resend
 from termcolor import colored
```

### Comparing `reliableGPT-0.2.956/reliablegpt/main.py` & `reliableGPT-0.2.957/reliablegpt/main.py`

 * *Files identical despite different names*

