# Comparing `tmp/simpm-2.0.1.tar.gz` & `tmp/simpm-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simpm-2.0.1.tar", last modified: Sun May 28 16:59:13 2023, max compression
+gzip compressed data, was "simpm-2.0.2.tar", last modified: Sun Jul  2 15:59:53 2023, max compression
```

## Comparing `simpm-2.0.1.tar` & `simpm-2.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 16:59:13.138248 simpm-2.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-28 16:59:02.000000 simpm-2.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-05-28 16:59:13.138248 simpm-2.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-05-28 16:59:02.000000 simpm-2.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-05-28 16:59:13.138248 simpm-2.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-28 16:59:02.000000 simpm-2.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 16:59:13.134248 simpm-2.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 16:59:13.138248 simpm-2.0.1/src/simpm/
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-28 16:59:02.000000 simpm-2.0.1/src/simpm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-05-28 16:59:02.000000 simpm-2.0.1/src/simpm/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    40268 2023-05-28 16:59:02.000000 simpm-2.0.1/src/simpm/des.py
--rw-r--r--   0 runner    (1001) docker     (123)     7049 2023-05-28 16:59:02.000000 simpm-2.0.1/src/simpm/dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     8724 2023-05-28 16:59:02.000000 simpm-2.0.1/src/simpm/log_cfg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 16:59:13.138248 simpm-2.0.1/src/simpm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-05-28 16:59:13.000000 simpm-2.0.1/src/simpm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-28 16:59:13.000000 simpm-2.0.1/src/simpm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 16:59:13.000000 simpm-2.0.1/src/simpm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 16:59:13.000000 simpm-2.0.1/src/simpm.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-28 16:59:13.000000 simpm-2.0.1/src/simpm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-28 16:59:13.000000 simpm-2.0.1/src/simpm.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 15:59:53.144596 simpm-2.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-02 15:59:43.000000 simpm-2.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-07-02 15:59:53.144596 simpm-2.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-07-02 15:59:43.000000 simpm-2.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-07-02 15:59:53.144596 simpm-2.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-07-02 15:59:43.000000 simpm-2.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 15:59:53.140596 simpm-2.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 15:59:53.144596 simpm-2.0.2/src/simpm/
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-02 15:59:43.000000 simpm-2.0.2/src/simpm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-02 15:59:43.000000 simpm-2.0.2/src/simpm/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40268 2023-07-02 15:59:43.000000 simpm-2.0.2/src/simpm/des.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7049 2023-07-02 15:59:43.000000 simpm-2.0.2/src/simpm/dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8724 2023-07-02 15:59:43.000000 simpm-2.0.2/src/simpm/log_cfg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 15:59:53.144596 simpm-2.0.2/src/simpm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-07-02 15:59:53.000000 simpm-2.0.2/src/simpm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-07-02 15:59:53.000000 simpm-2.0.2/src/simpm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 15:59:53.000000 simpm-2.0.2/src/simpm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 15:59:53.000000 simpm-2.0.2/src/simpm.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-02 15:59:53.000000 simpm-2.0.2/src/simpm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-02 15:59:53.000000 simpm-2.0.2/src/simpm.egg-info/top_level.txt
```

### Comparing `simpm-2.0.1/LICENSE` & `simpm-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `simpm-2.0.1/PKG-INFO` & `simpm-2.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simpm
-Version: 2.0.1
+Version: 2.0.2
 Summary: Simulation Tool in Project Management.
 Home-page: https://github.com/Project-SimPM
 Author: Naimeh Sadeghi, Pedram Elmi
 Author-email: "naima.sadeghi@gmail.com", "pedram.elmi@gmail.com"
 License: MIT License
 Keywords: python,project management,construction,simulation
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `simpm-2.0.1/README.md` & `simpm-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `simpm-2.0.1/setup.cfg` & `simpm-2.0.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `simpm-2.0.1/setup.py` & `simpm-2.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `simpm-2.0.1/src/simpm/_utils.py` & `simpm-2.0.2/src/simpm/_utils.py`

 * *Files identical despite different names*

### Comparing `simpm-2.0.1/src/simpm/des.py` & `simpm-2.0.2/src/simpm/des.py`

 * *Files identical despite different names*

### Comparing `simpm-2.0.1/src/simpm/dist.py` & `simpm-2.0.2/src/simpm/dist.py`

 * *Files identical despite different names*

### Comparing `simpm-2.0.1/src/simpm/log_cfg.py` & `simpm-2.0.2/src/simpm/log_cfg.py`

 * *Files identical despite different names*

### Comparing `simpm-2.0.1/src/simpm.egg-info/PKG-INFO` & `simpm-2.0.2/src/simpm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simpm
-Version: 2.0.1
+Version: 2.0.2
 Summary: Simulation Tool in Project Management.
 Home-page: https://github.com/Project-SimPM
 Author: Naimeh Sadeghi, Pedram Elmi
 Author-email: "naima.sadeghi@gmail.com", "pedram.elmi@gmail.com"
 License: MIT License
 Keywords: python,project management,construction,simulation
 Classifier: Development Status :: 5 - Production/Stable
```

