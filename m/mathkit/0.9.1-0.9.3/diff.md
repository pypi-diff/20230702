# Comparing `tmp/mathkit-0.9.1.tar.gz` & `tmp/mathkit-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mathkit-0.9.1.tar", last modified: Sun Jul  2 02:48:56 2023, max compression
+gzip compressed data, was "mathkit-0.9.3.tar", last modified: Sun Jul  2 03:39:18 2023, max compression
```

## Comparing `mathkit-0.9.1.tar` & `mathkit-0.9.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-07-02 02:48:56.377047 mathkit-0.9.1/
--rw-rw-rw-   0        0        0     3460 2023-07-02 02:48:56.377047 mathkit-0.9.1/PKG-INFO
--rw-rw-rw-   0        0        0     3021 2023-07-02 02:47:56.000000 mathkit-0.9.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-02 02:48:56.318289 mathkit-0.9.1/mathkit/
--rw-rw-rw-   0        0        0      467 2023-07-02 02:00:13.000000 mathkit-0.9.1/mathkit/__init__.py
--rw-rw-rw-   0        0        0     5057 2023-07-02 01:46:47.000000 mathkit-0.9.1/mathkit/main.py
-drwxrwxrwx   0        0        0        0 2023-07-02 02:48:56.377047 mathkit-0.9.1/mathkit.egg-info/
--rw-rw-rw-   0        0        0     3460 2023-07-02 02:48:56.000000 mathkit-0.9.1/mathkit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      178 2023-07-02 02:48:56.000000 mathkit-0.9.1/mathkit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-02 02:48:56.000000 mathkit-0.9.1/mathkit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-07-02 02:48:56.000000 mathkit-0.9.1/mathkit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-02 02:48:56.377047 mathkit-0.9.1/setup.cfg
--rw-rw-rw-   0        0        0      706 2023-07-02 02:48:50.000000 mathkit-0.9.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-02 03:39:18.306041 mathkit-0.9.3/
+-rw-rw-rw-   0        0        0     3466 2023-07-02 03:39:18.306041 mathkit-0.9.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3021 2023-07-02 02:47:56.000000 mathkit-0.9.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-02 03:39:18.273522 mathkit-0.9.3/mathkit/
+-rw-rw-rw-   0        0        0      482 2023-07-02 03:38:48.000000 mathkit-0.9.3/mathkit/__init__.py
+-rw-rw-rw-   0        0        0     5057 2023-07-02 01:46:47.000000 mathkit-0.9.3/mathkit/main.py
+drwxrwxrwx   0        0        0        0 2023-07-02 03:39:18.297891 mathkit-0.9.3/mathkit.egg-info/
+-rw-rw-rw-   0        0        0     3466 2023-07-02 03:39:18.000000 mathkit-0.9.3/mathkit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      178 2023-07-02 03:39:18.000000 mathkit-0.9.3/mathkit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-02 03:39:18.000000 mathkit-0.9.3/mathkit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-07-02 03:39:18.000000 mathkit-0.9.3/mathkit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-02 03:39:18.306041 mathkit-0.9.3/setup.cfg
+-rw-rw-rw-   0        0        0      712 2023-07-02 03:39:14.000000 mathkit-0.9.3/setup.py
```

### Comparing `mathkit-0.9.1/PKG-INFO` & `mathkit-0.9.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: mathkit
-Version: 0.9.1
+Version: 0.9.3
 Summary: Python library for mathematical functions
 Home-page: https://github.com/theunkownhacker/mathkit
-Author: Your Name
+Author: TheUnkownHacker
 Author-email: theunkownhacker@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `mathkit-0.9.1/README.md` & `mathkit-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `mathkit-0.9.1/mathkit/main.py` & `mathkit-0.9.3/mathkit/main.py`

 * *Files identical despite different names*

### Comparing `mathkit-0.9.1/mathkit.egg-info/PKG-INFO` & `mathkit-0.9.3/mathkit.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: mathkit
-Version: 0.9.1
+Version: 0.9.3
 Summary: Python library for mathematical functions
 Home-page: https://github.com/theunkownhacker/mathkit
-Author: Your Name
+Author: TheUnkownHacker
 Author-email: theunkownhacker@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `mathkit-0.9.1/setup.py` & `mathkit-0.9.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="mathkit",
-    version="0.9.1",
-    author="Your Name",
+    version="0.9.3",
+    author="TheUnkownHacker",
     author_email="theunkownhacker@gmail.com",
     description="Python library for mathematical functions",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/theunkownhacker/mathkit",
     packages=find_packages(),
     classifiers=[
```

