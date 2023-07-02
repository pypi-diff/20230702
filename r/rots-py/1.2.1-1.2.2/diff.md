# Comparing `tmp/rots-py-1.2.1.tar.gz` & `tmp/rots-py-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rots-py-1.2.1.tar", last modified: Fri Jun 30 13:10:06 2023, max compression
+gzip compressed data, was "rots-py-1.2.2.tar", last modified: Sun Jul  2 11:58:55 2023, max compression
```

## Comparing `rots-py-1.2.1.tar` & `rots-py-1.2.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-06-30 13:10:06.800663 rots-py-1.2.1/
--rw-rw-rw-   0        0        0     1097 2023-04-18 12:29:22.000000 rots-py-1.2.1/LICENSE
--rw-rw-rw-   0        0        0       91 2023-06-30 13:08:44.000000 rots-py-1.2.1/MANIFEST.in
--rw-rw-rw-   0        0        0     6380 2023-06-30 13:10:06.798663 rots-py-1.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     4583 2023-06-30 10:40:04.000000 rots-py-1.2.1/README.md
--rw-rw-rw-   0        0        0      858 2023-06-30 13:09:16.000000 rots-py-1.2.1/pyproject.toml
--rw-rw-rw-   0        0        0     2390 2023-06-29 12:09:31.000000 rots-py-1.2.1/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-06-30 13:10:06.800663 rots-py-1.2.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-30 13:10:06.579664 rots-py-1.2.1/src/
-drwxrwxrwx   0        0        0        0 2023-06-30 13:10:06.664664 rots-py-1.2.1/src/optim_cy/
--rw-rw-rw-   0        0        0   184832 2023-06-18 22:44:29.000000 rots-py-1.2.1/src/optim_cy/optim.cp39-win_amd64.pyd
--rw-rw-rw-   0        0        0      542 2023-06-29 12:09:31.000000 rots-py-1.2.1/src/optim_cy/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-30 13:10:06.756666 rots-py-1.2.1/src/rots_py.egg-info/
--rw-rw-rw-   0        0        0     6380 2023-06-30 13:10:06.000000 rots-py-1.2.1/src/rots_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      510 2023-06-30 13:10:06.000000 rots-py-1.2.1/src/rots_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-30 13:10:06.000000 rots-py-1.2.1/src/rots_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-06-30 13:10:06.000000 rots-py-1.2.1/src/rots_py.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       56 2023-06-30 13:10:06.000000 rots-py-1.2.1/src/rots_py.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-06-30 13:10:06.000000 rots-py-1.2.1/src/rots_py.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-30 13:10:06.795666 rots-py-1.2.1/src/rotspy/
--rw-rw-rw-   0        0        0      108 2023-06-29 12:09:31.000000 rots-py-1.2.1/src/rotspy/__init__.py
--rw-rw-rw-   0        0        0      139 2023-06-29 12:09:31.000000 rots-py-1.2.1/src/rotspy/__main__.py
--rw-rw-rw-   0        0        0     3101 2023-06-29 12:09:31.000000 rots-py-1.2.1/src/rotspy/calculateOverlaps1.py
--rw-rw-rw-   0        0        0     2816 2023-06-29 12:09:31.000000 rots-py-1.2.1/src/rotspy/calculateOverlaps2.py
--rw-rw-rw-   0        0        0    10374 2023-06-29 12:09:31.000000 rots-py-1.2.1/src/rotspy/helpers.py
--rw-rw-rw-   0        0        0     2382 2023-06-29 12:09:31.000000 rots-py-1.2.1/src/rotspy/plot_rots.py
--rw-rw-rw-   0        0        0    11320 2023-06-29 12:09:31.000000 rots-py-1.2.1/src/rotspy/rots.py
+drwxrwxrwx   0        0        0        0 2023-07-02 11:58:55.583193 rots-py-1.2.2/
+-rw-rw-rw-   0        0        0     1097 2023-04-18 12:29:22.000000 rots-py-1.2.2/LICENSE
+-rw-rw-rw-   0        0        0      150 2023-07-02 11:04:31.000000 rots-py-1.2.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     6380 2023-07-02 11:58:55.579192 rots-py-1.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4583 2023-06-30 10:40:04.000000 rots-py-1.2.2/README.md
+-rw-rw-rw-   0        0        0     1006 2023-07-02 11:58:21.000000 rots-py-1.2.2/pyproject.toml
+-rw-rw-rw-   0        0        0     4700 2023-07-02 11:14:20.000000 rots-py-1.2.2/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-02 11:58:55.584189 rots-py-1.2.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-02 11:58:55.482201 rots-py-1.2.2/src/
+drwxrwxrwx   0        0        0        0 2023-07-02 11:58:55.506195 rots-py-1.2.2/src/optim_cy/
+-rw-rw-rw-   0        0        0   184832 2023-06-18 22:44:29.000000 rots-py-1.2.2/src/optim_cy/optim.cp39-win_amd64.pyd
+-rw-rw-rw-   0        0        0  1009818 2023-06-29 12:09:31.000000 rots-py-1.2.2/src/optim_cy/optim.cpp
+drwxrwxrwx   0        0        0        0 2023-07-02 11:58:55.554190 rots-py-1.2.2/src/rots_py.egg-info/
+-rw-rw-rw-   0        0        0     6380 2023-07-02 11:58:55.000000 rots-py-1.2.2/src/rots_py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      511 2023-07-02 11:58:55.000000 rots-py-1.2.2/src/rots_py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-02 11:58:55.000000 rots-py-1.2.2/src/rots_py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-07-02 11:58:55.000000 rots-py-1.2.2/src/rots_py.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       79 2023-07-02 11:58:55.000000 rots-py-1.2.2/src/rots_py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-07-02 11:58:55.000000 rots-py-1.2.2/src/rots_py.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-02 11:58:55.577188 rots-py-1.2.2/src/rotspy/
+-rw-rw-rw-   0        0        0      108 2023-06-29 12:09:31.000000 rots-py-1.2.2/src/rotspy/__init__.py
+-rw-rw-rw-   0        0        0      288 2023-07-02 11:49:52.000000 rots-py-1.2.2/src/rotspy/__main__.py
+-rw-rw-rw-   0        0        0     3101 2023-06-29 12:09:31.000000 rots-py-1.2.2/src/rotspy/calculateOverlaps1.py
+-rw-rw-rw-   0        0        0     2816 2023-06-29 12:09:31.000000 rots-py-1.2.2/src/rotspy/calculateOverlaps2.py
+-rw-rw-rw-   0        0        0    10374 2023-06-29 12:09:31.000000 rots-py-1.2.2/src/rotspy/helpers.py
+-rw-rw-rw-   0        0        0     2382 2023-06-29 12:09:31.000000 rots-py-1.2.2/src/rotspy/plot_rots.py
+-rw-rw-rw-   0        0        0    11320 2023-06-29 12:09:31.000000 rots-py-1.2.2/src/rotspy/rots.py
```

### Comparing `rots-py-1.2.1/LICENSE` & `rots-py-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rots-py-1.2.1/PKG-INFO` & `rots-py-1.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rots-py
-Version: 1.2.1
+Version: 1.2.2
 Summary: ROTS gene ranking implementation in Python
 Author-email: "F.Mamadbekov, M.Shakya, A.Montoya, I.Ul-Haq" <fmamadbe@abo.fi>
 License: MIT License
         
         Copyright (c) 2023 EDISS-intake2-team4
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `rots-py-1.2.1/README.md` & `rots-py-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `rots-py-1.2.1/pyproject.toml` & `rots-py-1.2.2/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 # pyproject.toml
 
 [build-system]
-requires      = ["setuptools>=58.1.0", "wheel"]
+requires      = ['setuptools>=58.1.0', 'wheel', 'importlib-metadata >= 1.0 ; python_version < "3.8"']
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "rots-py"
-version = "1.2.1"
+version = "1.2.2"
 description = "ROTS gene ranking implementation in Python"
 readme = "README.md"
 authors = [{ name = "F.Mamadbekov, M.Shakya, A.Montoya, I.Ul-Haq", email = "fmamadbe@abo.fi" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
 keywords = ["rots", "gene", "ranking"]
 dependencies = [
+    "scikit-learn>=1.2.0",
+    "seaborn>=0.12.2",
+    "openpyxl>=3.1.2",
     "numba >= 0.56.4",
-    "numpy",
-    "pandas",
     "tqdm>=4.64.1",
-    "Cython>=0.29.35",
 ]
 requires-python = ">=3.6"
 
+[tool.setuptools.dynamic]
+version = {attr = "package.__version__"}
+
 [project.urls]
 Homepage = "https://github.com/EDISS-intake2-team4/rots-py"
 
 [project.scripts]
 realpython = "rotspy.__main__:main"
```

### Comparing `rots-py-1.2.1/src/rots_py.egg-info/PKG-INFO` & `rots-py-1.2.2/src/rots_py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rots-py
-Version: 1.2.1
+Version: 1.2.2
 Summary: ROTS gene ranking implementation in Python
 Author-email: "F.Mamadbekov, M.Shakya, A.Montoya, I.Ul-Haq" <fmamadbe@abo.fi>
 License: MIT License
         
         Copyright (c) 2023 EDISS-intake2-team4
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `rots-py-1.2.1/src/rotspy/calculateOverlaps1.py` & `rots-py-1.2.2/src/rotspy/calculateOverlaps1.py`

 * *Files identical despite different names*

### Comparing `rots-py-1.2.1/src/rotspy/calculateOverlaps2.py` & `rots-py-1.2.2/src/rotspy/calculateOverlaps2.py`

 * *Files identical despite different names*

### Comparing `rots-py-1.2.1/src/rotspy/helpers.py` & `rots-py-1.2.2/src/rotspy/helpers.py`

 * *Files identical despite different names*

### Comparing `rots-py-1.2.1/src/rotspy/plot_rots.py` & `rots-py-1.2.2/src/rotspy/plot_rots.py`

 * *Files identical despite different names*

### Comparing `rots-py-1.2.1/src/rotspy/rots.py` & `rots-py-1.2.2/src/rotspy/rots.py`

 * *Files identical despite different names*

