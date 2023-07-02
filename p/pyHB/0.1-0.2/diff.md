# Comparing `tmp/pyHB-0.1.tar.gz` & `tmp/pyHB-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyHB-0.1.tar", last modified: Sun Jul  2 04:00:02 2023, max compression
+gzip compressed data, was "pyHB-0.2.tar", last modified: Sun Jul  2 04:46:04 2023, max compression
```

## Comparing `pyHB-0.1.tar` & `pyHB-0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 04:00:02.753198 pyHB-0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-02 03:59:50.000000 pyHB-0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-07-02 04:00:02.753198 pyHB-0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-02 03:59:50.000000 pyHB-0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 04:00:02.753198 pyHB-0.1/pyHB.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-07-02 04:00:02.000000 pyHB-0.1/pyHB.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-02 04:00:02.000000 pyHB-0.1/pyHB.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 04:00:02.000000 pyHB-0.1/pyHB.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-02 04:00:02.000000 pyHB-0.1/pyHB.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 04:00:02.000000 pyHB-0.1/pyHB.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 04:00:02.753198 pyHB-0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-07-02 03:59:50.000000 pyHB-0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 04:46:04.898384 pyHB-0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-02 04:45:53.000000 pyHB-0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-07-02 04:46:04.898384 pyHB-0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-02 04:45:53.000000 pyHB-0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 04:46:04.898384 pyHB-0.2/pyHB.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-07-02 04:46:04.000000 pyHB-0.2/pyHB.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-02 04:46:04.000000 pyHB-0.2/pyHB.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 04:46:04.000000 pyHB-0.2/pyHB.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-02 04:46:04.000000 pyHB-0.2/pyHB.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 04:46:04.000000 pyHB-0.2/pyHB.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 04:46:04.898384 pyHB-0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-07-02 04:45:53.000000 pyHB-0.2/setup.py
```

### Comparing `pyHB-0.1/LICENSE` & `pyHB-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyHB-0.1/PKG-INFO` & `pyHB-0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyHB
-Version: 0.1
+Version: 0.2
 Summary: This is a simple package which is used in HackBot Support Pyrogram + Telethon
 Home-page: https://github.com/LEGEND-AI/pyHB
 Author: LegendBoy
 Author-email: krishna045jaiswal@gmail.com
 License: GNU General Public License v3.0
 Keywords: pyHB,HB
 Classifier: Framework :: AsyncIO
```

### Comparing `pyHB-0.1/pyHB.egg-info/PKG-INFO` & `pyHB-0.2/pyHB.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyHB
-Version: 0.1
+Version: 0.2
 Summary: This is a simple package which is used in HackBot Support Pyrogram + Telethon
 Home-page: https://github.com/LEGEND-AI/pyHB
 Author: LegendBoy
 Author-email: krishna045jaiswal@gmail.com
 License: GNU General Public License v3.0
 Keywords: pyHB,HB
 Classifier: Framework :: AsyncIO
```

### Comparing `pyHB-0.1/setup.py` & `pyHB-0.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     sys.stderr.write( "Warning: Could not open README.md due %s\n" % error )
     
 
 setup(
     name="pyHB",
     author="LegendBoy",
     author_email="krishna045jaiswal@gmail.com",
-    version="0.1",
+    version="0.2",
     description="This is a simple package which is used in HackBot Support Pyrogram + Telethon",
     long_description = readme_contents,
     long_description_content_type="text/markdown",
     url="https://github.com/LEGEND-AI/pyHB",
     packages=find_packages(),
     license="GNU General Public License v3.0",
     include_package_data=True,
```

