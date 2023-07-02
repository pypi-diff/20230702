# Comparing `tmp/powerdns-secondary-cleaner-1.0.tar.gz` & `tmp/powerdns-secondary-cleaner-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "powerdns-secondary-cleaner-1.0.tar", last modified: Sun Jul  2 14:20:39 2023, max compression
+gzip compressed data, was "powerdns-secondary-cleaner-1.0.1.tar", last modified: Sun Jul  2 15:51:37 2023, max compression
```

## Comparing `powerdns-secondary-cleaner-1.0.tar` & `powerdns-secondary-cleaner-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 14:20:39.915873 powerdns-secondary-cleaner-1.0/
--rw-rw-rw-   0 root         (0) root         (0)     1068 2023-07-02 14:10:40.000000 powerdns-secondary-cleaner-1.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1970 2023-07-02 14:20:39.915873 powerdns-secondary-cleaner-1.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1345 2023-07-02 14:10:40.000000 powerdns-secondary-cleaner-1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 14:20:39.915873 powerdns-secondary-cleaner-1.0/powerdns_secondary_cleaner/
--rw-rw-rw-   0 root         (0) root         (0)     1947 2023-07-02 14:10:40.000000 powerdns-secondary-cleaner-1.0/powerdns_secondary_cleaner/CLI.py
--rw-rw-rw-   0 root         (0) root         (0)       46 2023-07-02 14:10:40.000000 powerdns-secondary-cleaner-1.0/powerdns_secondary_cleaner/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1532 2023-07-02 14:10:40.000000 powerdns-secondary-cleaner-1.0/powerdns_secondary_cleaner/powerdns_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 14:20:39.915873 powerdns-secondary-cleaner-1.0/powerdns_secondary_cleaner.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1970 2023-07-02 14:20:39.000000 powerdns-secondary-cleaner-1.0/powerdns_secondary_cleaner.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      469 2023-07-02 14:20:39.000000 powerdns-secondary-cleaner-1.0/powerdns_secondary_cleaner.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-02 14:20:39.000000 powerdns-secondary-cleaner-1.0/powerdns_secondary_cleaner.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       84 2023-07-02 14:20:39.000000 powerdns-secondary-cleaner-1.0/powerdns_secondary_cleaner.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       45 2023-07-02 14:20:39.000000 powerdns-secondary-cleaner-1.0/powerdns_secondary_cleaner.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       27 2023-07-02 14:20:39.000000 powerdns-secondary-cleaner-1.0/powerdns_secondary_cleaner.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      340 2023-07-02 14:10:40.000000 powerdns-secondary-cleaner-1.0/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      199 2023-07-02 14:20:39.919873 powerdns-secondary-cleaner-1.0/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1284 2023-07-02 14:10:40.000000 powerdns-secondary-cleaner-1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 15:51:37.170128 powerdns-secondary-cleaner-1.0.1/
+-rw-rw-rw-   0 root         (0) root         (0)     1068 2023-07-02 14:10:40.000000 powerdns-secondary-cleaner-1.0.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1972 2023-07-02 15:51:37.170128 powerdns-secondary-cleaner-1.0.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1345 2023-07-02 14:10:40.000000 powerdns-secondary-cleaner-1.0.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 15:51:37.170128 powerdns-secondary-cleaner-1.0.1/powerdns_secondary_cleaner/
+-rw-rw-rw-   0 root         (0) root         (0)     1947 2023-07-02 14:10:40.000000 powerdns-secondary-cleaner-1.0.1/powerdns_secondary_cleaner/CLI.py
+-rw-rw-rw-   0 root         (0) root         (0)       46 2023-07-02 14:10:40.000000 powerdns-secondary-cleaner-1.0.1/powerdns_secondary_cleaner/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1532 2023-07-02 14:10:40.000000 powerdns-secondary-cleaner-1.0.1/powerdns_secondary_cleaner/powerdns_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 15:51:37.170128 powerdns-secondary-cleaner-1.0.1/powerdns_secondary_cleaner.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1972 2023-07-02 15:51:37.000000 powerdns-secondary-cleaner-1.0.1/powerdns_secondary_cleaner.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      469 2023-07-02 15:51:37.000000 powerdns-secondary-cleaner-1.0.1/powerdns_secondary_cleaner.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-02 15:51:37.000000 powerdns-secondary-cleaner-1.0.1/powerdns_secondary_cleaner.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       84 2023-07-02 15:51:37.000000 powerdns-secondary-cleaner-1.0.1/powerdns_secondary_cleaner.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       45 2023-07-02 15:51:37.000000 powerdns-secondary-cleaner-1.0.1/powerdns_secondary_cleaner.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       27 2023-07-02 15:51:37.000000 powerdns-secondary-cleaner-1.0.1/powerdns_secondary_cleaner.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      340 2023-07-02 14:10:40.000000 powerdns-secondary-cleaner-1.0.1/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      199 2023-07-02 15:51:37.170128 powerdns-secondary-cleaner-1.0.1/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1286 2023-07-02 15:50:24.000000 powerdns-secondary-cleaner-1.0.1/setup.py
```

### Comparing `powerdns-secondary-cleaner-1.0/LICENSE` & `powerdns-secondary-cleaner-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `powerdns-secondary-cleaner-1.0/PKG-INFO` & `powerdns-secondary-cleaner-1.0.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: powerdns-secondary-cleaner
-Version: 1.0
+Version: 1.0.1
 Summary: Use powerdns-secondary-cleaner to delete zones on secondary PowerDNS server that were deleted on primary PowerDNS server.
 Home-page: https://github.com/CyberfusionIO/powerdns-secondary-cleaner
 Author: William Edwards
 Author-email: support@cyberfusion.nl
 License: MIT
 Keywords: cyberfusion,powerdns
 Platform: linux
```

### Comparing `powerdns-secondary-cleaner-1.0/README.md` & `powerdns-secondary-cleaner-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `powerdns-secondary-cleaner-1.0/powerdns_secondary_cleaner/CLI.py` & `powerdns-secondary-cleaner-1.0.1/powerdns_secondary_cleaner/CLI.py`

 * *Files identical despite different names*

### Comparing `powerdns-secondary-cleaner-1.0/powerdns_secondary_cleaner/powerdns_api.py` & `powerdns-secondary-cleaner-1.0.1/powerdns_secondary_cleaner/powerdns_api.py`

 * *Files identical despite different names*

### Comparing `powerdns-secondary-cleaner-1.0/powerdns_secondary_cleaner.egg-info/PKG-INFO` & `powerdns-secondary-cleaner-1.0.1/powerdns_secondary_cleaner.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: powerdns-secondary-cleaner
-Version: 1.0
+Version: 1.0.1
 Summary: Use powerdns-secondary-cleaner to delete zones on secondary PowerDNS server that were deleted on primary PowerDNS server.
 Home-page: https://github.com/CyberfusionIO/powerdns-secondary-cleaner
 Author: William Edwards
 Author-email: support@cyberfusion.nl
 License: MIT
 Keywords: cyberfusion,powerdns
 Platform: linux
```

### Comparing `powerdns-secondary-cleaner-1.0/setup.py` & `powerdns-secondary-cleaner-1.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="powerdns-secondary-cleaner",
-    version="1.0",
+    version="1.0.1",
     description="Use powerdns-secondary-cleaner to delete zones on secondary PowerDNS server that were deleted on primary PowerDNS server.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     python_requires=">=3.6",
     author="William Edwards",
     author_email="support@cyberfusion.nl",
     url="https://github.com/CyberfusionIO/powerdns-secondary-cleaner",
@@ -21,15 +21,15 @@
             "powerdns_secondary_cleaner",
             "powerdns_secondary_cleaner.*",
         ]
     ),
     data_files=[],
     entry_points={
         "console_scripts": [
-            "powerdns_secondary_cleaner=powerdns_secondary_cleaner.CLI:main"
+            "powerdns-secondary-cleaner=powerdns_secondary_cleaner.CLI:main"
         ]
     },
     install_requires=["docopt==0.6.2", "schema==0.7.2", "requests==2.27.1"],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
```

