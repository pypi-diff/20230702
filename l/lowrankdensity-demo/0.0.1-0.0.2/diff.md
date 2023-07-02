# Comparing `tmp/lowrankdensity_demo-0.0.1.tar.gz` & `tmp/lowrankdensity_demo-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\Laur\350neDAVID\Documents\ss_demo\Summer_School_Package\dist\.tmp-q2wiymy1\lowrankdensity_demo-0.0.1.tar", last modified: Sat Jul  1 22:36:27 2023, max compression
+gzip compressed data, was "C:\Users\Laur\350neDAVID\Documents\ss_demo\Summer_School_Package\dist\.tmp-e238z788\lowrankdensity_demo-0.0.2.tar", last modified: Sun Jul  2 19:27:54 2023, max compression
```

## Comparing `lowrankdensity_demo-0.0.1.tar` & `lowrankdensity_demo-0.0.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-07-01 22:36:27.401270 lowrankdensity_demo-0.0.1/
--rw-rw-rw-   0        0        0     1070 2023-06-27 16:20:17.000000 lowrankdensity_demo-0.0.1/LICENSE
--rw-rw-rw-   0        0        0       52 2023-06-27 16:20:17.000000 lowrankdensity_demo-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0      367 2023-07-01 22:36:27.401270 lowrankdensity_demo-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      105 2023-06-30 13:43:33.000000 lowrankdensity_demo-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0      817 2023-07-01 22:36:27.403423 lowrankdensity_demo-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-01 22:36:27.332750 lowrankdensity_demo-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-07-01 22:36:27.341911 lowrankdensity_demo-0.0.1/src/lowrankdensity/
--rw-rw-rw-   0        0        0       60 2023-06-27 16:22:05.000000 lowrankdensity_demo-0.0.1/src/lowrankdensity/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-01 22:36:27.345816 lowrankdensity_demo-0.0.1/src/lowrankdensity/datasets/
--rw-rw-rw-   0        0        0       54 2023-06-27 16:21:18.000000 lowrankdensity_demo-0.0.1/src/lowrankdensity/datasets/__init__.py
--rw-rw-rw-   0        0        0     3858 2023-06-27 16:20:17.000000 lowrankdensity_demo-0.0.1/src/lowrankdensity/datasets/generate_samples.py
-drwxrwxrwx   0        0        0        0 2023-07-01 22:36:27.380335 lowrankdensity_demo-0.0.1/src/lowrankdensity/models/
--rw-rw-rw-   0        0        0       35 2023-06-27 16:20:17.000000 lowrankdensity_demo-0.0.1/src/lowrankdensity/models/__init__.py
--rw-rw-rw-   0        0        0     7691 2023-06-27 16:20:17.000000 lowrankdensity_demo-0.0.1/src/lowrankdensity/models/continuous.py
--rw-rw-rw-   0        0        0     7185 2023-06-27 16:20:17.000000 lowrankdensity_demo-0.0.1/src/lowrankdensity/models/discrete.py
-drwxrwxrwx   0        0        0        0 2023-07-01 22:36:27.393694 lowrankdensity_demo-0.0.1/src/lowrankdensity_demo.egg-info/
--rw-rw-rw-   0        0        0      367 2023-07-01 22:36:27.000000 lowrankdensity_demo-0.0.1/src/lowrankdensity_demo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      589 2023-07-01 22:36:27.000000 lowrankdensity_demo-0.0.1/src/lowrankdensity_demo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-01 22:36:27.000000 lowrankdensity_demo-0.0.1/src/lowrankdensity_demo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-07-01 22:36:27.000000 lowrankdensity_demo-0.0.1/src/lowrankdensity_demo.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-07-01 22:36:27.000000 lowrankdensity_demo-0.0.1/src/lowrankdensity_demo.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-01 22:36:27.398708 lowrankdensity_demo-0.0.1/test/
--rw-rw-rw-   0        0        0     3555 2023-06-27 16:20:37.000000 lowrankdensity_demo-0.0.1/test/test_continuous.py
--rw-rw-rw-   0        0        0     7079 2023-06-27 16:20:46.000000 lowrankdensity_demo-0.0.1/test/test_discrete.py
--rw-rw-rw-   0        0        0     4133 2023-06-30 13:29:20.000000 lowrankdensity_demo-0.0.1/test/test_generate_samples.py
+drwxrwxrwx   0        0        0        0 2023-07-02 19:27:54.379652 lowrankdensity_demo-0.0.2/
+-rw-rw-rw-   0        0        0     1070 2023-06-27 16:20:17.000000 lowrankdensity_demo-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0       52 2023-06-27 16:20:17.000000 lowrankdensity_demo-0.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      367 2023-07-02 19:27:54.379652 lowrankdensity_demo-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      105 2023-06-30 13:43:33.000000 lowrankdensity_demo-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0      817 2023-07-02 19:27:54.393845 lowrankdensity_demo-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-02 19:27:54.296974 lowrankdensity_demo-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-07-02 19:27:54.335160 lowrankdensity_demo-0.0.2/src/lowrankdensity/
+-rw-rw-rw-   0        0        0       60 2023-06-27 16:22:05.000000 lowrankdensity_demo-0.0.2/src/lowrankdensity/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-02 19:27:54.338958 lowrankdensity_demo-0.0.2/src/lowrankdensity/datasets/
+-rw-rw-rw-   0        0        0       54 2023-06-27 16:21:18.000000 lowrankdensity_demo-0.0.2/src/lowrankdensity/datasets/__init__.py
+-rw-rw-rw-   0        0        0     3858 2023-06-27 16:20:17.000000 lowrankdensity_demo-0.0.2/src/lowrankdensity/datasets/generate_samples.py
+drwxrwxrwx   0        0        0        0 2023-07-02 19:27:54.345591 lowrankdensity_demo-0.0.2/src/lowrankdensity/models/
+-rw-rw-rw-   0        0        0       35 2023-06-27 16:20:17.000000 lowrankdensity_demo-0.0.2/src/lowrankdensity/models/__init__.py
+-rw-rw-rw-   0        0        0     7691 2023-06-27 16:20:17.000000 lowrankdensity_demo-0.0.2/src/lowrankdensity/models/continuous.py
+-rw-rw-rw-   0        0        0     7185 2023-06-27 16:20:17.000000 lowrankdensity_demo-0.0.2/src/lowrankdensity/models/discrete.py
+drwxrwxrwx   0        0        0        0 2023-07-02 19:27:54.370672 lowrankdensity_demo-0.0.2/src/lowrankdensity_demo.egg-info/
+-rw-rw-rw-   0        0        0      367 2023-07-02 19:27:54.000000 lowrankdensity_demo-0.0.2/src/lowrankdensity_demo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      589 2023-07-02 19:27:54.000000 lowrankdensity_demo-0.0.2/src/lowrankdensity_demo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-02 19:27:54.000000 lowrankdensity_demo-0.0.2/src/lowrankdensity_demo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-07-02 19:27:54.000000 lowrankdensity_demo-0.0.2/src/lowrankdensity_demo.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-07-02 19:27:54.000000 lowrankdensity_demo-0.0.2/src/lowrankdensity_demo.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-02 19:27:54.379652 lowrankdensity_demo-0.0.2/test/
+-rw-rw-rw-   0        0        0     3555 2023-06-27 16:20:37.000000 lowrankdensity_demo-0.0.2/test/test_continuous.py
+-rw-rw-rw-   0        0        0     7079 2023-06-27 16:20:46.000000 lowrankdensity_demo-0.0.2/test/test_discrete.py
+-rw-rw-rw-   0        0        0     4133 2023-06-30 13:29:20.000000 lowrankdensity_demo-0.0.2/test/test_generate_samples.py
```

### Comparing `lowrankdensity_demo-0.0.1/LICENSE` & `lowrankdensity_demo-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lowrankdensity_demo-0.0.1/setup.cfg` & `lowrankdensity_demo-0.0.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206c 6f77 7261 6e6b 6465 6e73 6974   = lowrankdensit
 00000020: 795f 6465 6d6f 0d0a 7665 7273 696f 6e20  y_demo..version 
-00000030: 3d20 302e 302e 310d 0a64 6573 6372 6970  = 0.0.1..descrip
+00000030: 3d20 302e 302e 320d 0a64 6573 6372 6970  = 0.0.2..descrip
 00000040: 7469 6f6e 203d 2054 6869 7320 7061 636b  tion = This pack
 00000050: 6167 6520 646f 6573 2061 6d61 7a69 6e67  age does amazing
 00000060: 2074 6869 6e67 732e 0d0a 6c6f 6e67 5f64   things...long_d
 00000070: 6573 6372 6970 7469 6f6e 203d 2066 696c  escription = fil
 00000080: 653a 2052 4541 444d 452e 6d64 0d0a 6c6f  e: README.md..lo
 00000090: 6e67 5f64 6573 6372 6970 7469 6f6e 5f63  ng_description_c
 000000a0: 6f6e 7465 6e74 5f74 7970 6520 3d20 7465  ontent_type = te
```

### Comparing `lowrankdensity_demo-0.0.1/src/lowrankdensity/datasets/generate_samples.py` & `lowrankdensity_demo-0.0.2/src/lowrankdensity/datasets/generate_samples.py`

 * *Files identical despite different names*

### Comparing `lowrankdensity_demo-0.0.1/src/lowrankdensity/models/continuous.py` & `lowrankdensity_demo-0.0.2/src/lowrankdensity/models/continuous.py`

 * *Files identical despite different names*

### Comparing `lowrankdensity_demo-0.0.1/src/lowrankdensity/models/discrete.py` & `lowrankdensity_demo-0.0.2/src/lowrankdensity/models/discrete.py`

 * *Files identical despite different names*

### Comparing `lowrankdensity_demo-0.0.1/src/lowrankdensity_demo.egg-info/SOURCES.txt` & `lowrankdensity_demo-0.0.2/src/lowrankdensity_demo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lowrankdensity_demo-0.0.1/test/test_continuous.py` & `lowrankdensity_demo-0.0.2/test/test_continuous.py`

 * *Files identical despite different names*

### Comparing `lowrankdensity_demo-0.0.1/test/test_discrete.py` & `lowrankdensity_demo-0.0.2/test/test_discrete.py`

 * *Files identical despite different names*

### Comparing `lowrankdensity_demo-0.0.1/test/test_generate_samples.py` & `lowrankdensity_demo-0.0.2/test/test_generate_samples.py`

 * *Files identical despite different names*

