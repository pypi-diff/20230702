# Comparing `tmp/pygittesting-0.1.tar.gz` & `tmp/pygittesting-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygittesting-0.1.tar", last modified: Sun Jul  2 06:32:33 2023, max compression
+gzip compressed data, was "pygittesting-0.2.2.tar", last modified: Sun Jul  2 06:42:25 2023, max compression
```

## Comparing `pygittesting-0.1.tar` & `pygittesting-0.2.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 06:32:33.488838 pygittesting-0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-02 06:32:23.000000 pygittesting-0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-07-02 06:32:33.488838 pygittesting-0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-02 06:32:23.000000 pygittesting-0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 06:32:33.488838 pygittesting-0.1/TEST/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-02 06:32:23.000000 pygittesting-0.1/TEST/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-02 06:32:23.000000 pygittesting-0.1/TEST/data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 06:32:33.488838 pygittesting-0.1/pygittesting.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-07-02 06:32:33.000000 pygittesting-0.1/pygittesting.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-02 06:32:33.000000 pygittesting-0.1/pygittesting.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 06:32:33.000000 pygittesting-0.1/pygittesting.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-02 06:32:33.000000 pygittesting-0.1/pygittesting.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-02 06:32:33.000000 pygittesting-0.1/pygittesting.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 06:32:33.488838 pygittesting-0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-07-02 06:32:23.000000 pygittesting-0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 06:42:25.074151 pygittesting-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-02 06:42:13.000000 pygittesting-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-02 06:42:25.074151 pygittesting-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-02 06:42:13.000000 pygittesting-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 06:42:25.074151 pygittesting-0.2.2/TEST/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-02 06:42:13.000000 pygittesting-0.2.2/TEST/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-02 06:42:13.000000 pygittesting-0.2.2/TEST/data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 06:42:25.074151 pygittesting-0.2.2/pygittesting.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-02 06:42:25.000000 pygittesting-0.2.2/pygittesting.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-02 06:42:25.000000 pygittesting-0.2.2/pygittesting.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 06:42:25.000000 pygittesting-0.2.2/pygittesting.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-02 06:42:25.000000 pygittesting-0.2.2/pygittesting.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-02 06:42:25.000000 pygittesting-0.2.2/pygittesting.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 06:42:25.074151 pygittesting-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-07-02 06:42:13.000000 pygittesting-0.2.2/setup.py
```

### Comparing `pygittesting-0.1/LICENSE` & `pygittesting-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pygittesting-0.1/PKG-INFO` & `pygittesting-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygittesting
-Version: 0.1
+Version: 0.2.2
 Summary: This is a simple package which is used in HackBot Support Pyrogram + Telethon
 Home-page: https://github.com/LEGEND-AI/exampl_test
 Author: LegendBoy
 Author-email: krishna045jaiswal@gmail.com
 License: GNU General Public License v3.0
 Keywords: test
 Classifier: Framework :: AsyncIO
```

### Comparing `pygittesting-0.1/pygittesting.egg-info/PKG-INFO` & `pygittesting-0.2.2/pygittesting.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygittesting
-Version: 0.1
+Version: 0.2.2
 Summary: This is a simple package which is used in HackBot Support Pyrogram + Telethon
 Home-page: https://github.com/LEGEND-AI/exampl_test
 Author: LegendBoy
 Author-email: krishna045jaiswal@gmail.com
 License: GNU General Public License v3.0
 Keywords: test
 Classifier: Framework :: AsyncIO
```

### Comparing `pygittesting-0.1/setup.py` & `pygittesting-0.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     sys.stderr.write( "Warning: Could not open README.md due %s\n" % error )
     
 
 setup(
     name="pygittesting",
     author="LegendBoy",
     author_email="krishna045jaiswal@gmail.com",
-    version="0.1",
+    version="0.2.2",
     description="This is a simple package which is used in HackBot Support Pyrogram + Telethon",
     long_description = readme_contents,
     long_description_content_type="text/markdown",
     url="https://github.com/LEGEND-AI/exampl_test",
     packages=find_packages(),
     license="GNU General Public License v3.0",
     include_package_data=True,
```

