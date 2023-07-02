# Comparing `tmp/scReGAT-0.0.3.tar.gz` & `tmp/scReGAT-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/scReGAT-0.0.3.tar", last modified: Thu Jun 29 14:08:15 2023, max compression
+gzip compressed data, was "dist/scReGAT-0.0.4.tar", last modified: Sun Jul  2 08:33:41 2023, max compression
```

## Comparing `scReGAT-0.0.3.tar` & `scReGAT-0.0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 14:08:15.088652 scReGAT-0.0.3/
--rw-r--r--   0 root         (0) root         (0)      336 2023-06-29 14:08:15.088652 scReGAT-0.0.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      101 2023-06-05 08:08:33.000000 scReGAT-0.0.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 14:08:15.088652 scReGAT-0.0.3/example/
--rw-r--r--   0 root         (0) root         (0)      246 2023-06-04 09:41:22.000000 scReGAT-0.0.3/example/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 14:08:15.088652 scReGAT-0.0.3/scReGAT.egg-info/
--rw-r--r--   0 root         (0) root         (0)      336 2023-06-29 14:08:15.000000 scReGAT-0.0.3/scReGAT.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      305 2023-06-29 14:08:15.000000 scReGAT-0.0.3/scReGAT.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-29 14:08:15.000000 scReGAT-0.0.3/scReGAT.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      120 2023-06-29 14:08:15.000000 scReGAT-0.0.3/scReGAT.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-06-29 14:08:15.000000 scReGAT-0.0.3/scReGAT.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 14:08:15.088652 scReGAT-0.0.3/scregat/
--rw-r--r--   0 root         (0) root         (0)       18 2023-06-29 13:17:07.000000 scReGAT-0.0.3/scregat/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)    25982 2023-06-29 11:45:18.000000 scReGAT-0.0.3/scregat/data_process.py
--rwxr-xr-x   0 root         (0) root         (0)    23602 2023-04-03 07:03:21.000000 scReGAT-0.0.3/scregat/data_process_1.py
--rwxr-xr-x   0 root         (0) root         (0)    27891 2023-04-03 11:48:59.000000 scReGAT-0.0.3/scregat/data_process_2.py
--rwxr-xr-x   0 root         (0) root         (0)    22374 2023-06-08 06:29:07.000000 scReGAT-0.0.3/scregat/model.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-29 14:08:15.088652 scReGAT-0.0.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1054 2023-06-29 14:08:04.000000 scReGAT-0.0.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 08:33:41.750866 scReGAT-0.0.4/
+-rw-r--r--   0 root         (0) root         (0)      336 2023-07-02 08:33:41.750866 scReGAT-0.0.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      101 2023-06-05 08:08:33.000000 scReGAT-0.0.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 08:33:41.690866 scReGAT-0.0.4/example/
+-rw-r--r--   0 root         (0) root         (0)      246 2023-06-04 09:41:22.000000 scReGAT-0.0.4/example/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 08:33:41.706866 scReGAT-0.0.4/scReGAT.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      336 2023-07-02 08:33:41.000000 scReGAT-0.0.4/scReGAT.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      305 2023-07-02 08:33:41.000000 scReGAT-0.0.4/scReGAT.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-02 08:33:41.000000 scReGAT-0.0.4/scReGAT.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      125 2023-07-02 08:33:41.000000 scReGAT-0.0.4/scReGAT.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-07-02 08:33:41.000000 scReGAT-0.0.4/scReGAT.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 08:33:41.750866 scReGAT-0.0.4/scregat/
+-rw-r--r--   0 root         (0) root         (0)       18 2023-06-29 13:17:07.000000 scReGAT-0.0.4/scregat/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)    25982 2023-06-29 11:45:18.000000 scReGAT-0.0.4/scregat/data_process.py
+-rwxr-xr-x   0 root         (0) root         (0)    23602 2023-04-03 07:03:21.000000 scReGAT-0.0.4/scregat/data_process_1.py
+-rwxr-xr-x   0 root         (0) root         (0)    27891 2023-04-03 11:48:59.000000 scReGAT-0.0.4/scregat/data_process_2.py
+-rwxr-xr-x   0 root         (0) root         (0)    22374 2023-06-08 06:29:07.000000 scReGAT-0.0.4/scregat/model.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-02 08:33:41.750866 scReGAT-0.0.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1059 2023-07-02 08:32:46.000000 scReGAT-0.0.4/setup.py
```

### Comparing `scReGAT-0.0.3/scregat/data_process.py` & `scReGAT-0.0.4/scregat/data_process.py`

 * *Files identical despite different names*

### Comparing `scReGAT-0.0.3/scregat/data_process_1.py` & `scReGAT-0.0.4/scregat/data_process_1.py`

 * *Files identical despite different names*

### Comparing `scReGAT-0.0.3/scregat/data_process_2.py` & `scReGAT-0.0.4/scregat/data_process_2.py`

 * *Files identical despite different names*

### Comparing `scReGAT-0.0.3/scregat/model.py` & `scReGAT-0.0.4/scregat/model.py`

 * *Files identical despite different names*

### Comparing `scReGAT-0.0.3/setup.py` & `scReGAT-0.0.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,20 +9,20 @@
 NAME = 'scReGAT'
 DESCRIPTION = \
     'A GAT-based computational framework to predict long-range gene regulatory relationships'
 URL = 'https://github.com/Drizzle-Zhang/scReGAT'
 EMAIL = 'zhang_yu18@fudan.edu.cn'
 AUTHOR = 'Yu Zhang'
 REQUIRES_PYTHON = '>=3.8.3'
-VERSION = '0.0.3'
+VERSION = '0.0.4'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
-    "numpy", "pandas", "sklearn", "scipy", "statsmodels", "anndata", "scanpy", "episcanpy", "cosg",
-    "torch", "torch_geometric", "captum", "audtorch", "torch_sparse",
+    "numpy", "pandas", "scikit-learn", "scipy", "statsmodels", "anndata", "scanpy", "episcanpy",
+    "cosg", "torch", "torch_geometric", "captum", "audtorch", "torch_sparse",
 ]
 
 # Setting.
 setup(
     name=NAME,
     version=VERSION,
     description=DESCRIPTION,
```

