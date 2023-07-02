# Comparing `tmp/fablab-0.0.0.tar.gz` & `tmp/fablab-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/thomassatterly/Developer/python/fablab/dist/.tmp-owyi_5ef/fablab-0.0.0.tar", last modified: Thu Jan 26 00:35:27 2023, max compression
+gzip compressed data, was "fablab-0.0.2.tar", last modified: Sun Jul  2 19:49:50 2023, max compression
```

## Comparing `fablab-0.0.0.tar` & `fablab-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,19 @@
-drwxr-xr-x   0 thomassatterly   (501) staff       (20)        0 2023-01-26 00:35:27.166367 fablab-0.0.0/
--rw-r--r--   0 thomassatterly   (501) staff       (20)     1030 2023-01-20 02:06:57.000000 fablab-0.0.0/LICENSE
--rw-r--r--   0 thomassatterly   (501) staff       (20)       40 2023-01-26 00:26:50.000000 fablab-0.0.0/MANIFEST.in
--rw-r--r--   0 thomassatterly   (501) staff       (20)     1527 2023-01-26 00:35:27.166059 fablab-0.0.0/PKG-INFO
--rw-r--r--   0 thomassatterly   (501) staff       (20)        0 2023-01-20 01:59:48.000000 fablab-0.0.0/README.md
--rw-r--r--   0 thomassatterly   (501) staff       (20)      592 2023-01-26 00:26:34.000000 fablab-0.0.0/pyproject.toml
--rw-r--r--   0 thomassatterly   (501) staff       (20)       38 2023-01-26 00:35:27.166450 fablab-0.0.0/setup.cfg
--rw-r--r--   0 thomassatterly   (501) staff       (20)       37 2023-01-26 00:33:20.000000 fablab-0.0.0/setup.py
-drwxr-xr-x   0 thomassatterly   (501) staff       (20)        0 2023-01-26 00:35:27.162346 fablab-0.0.0/src/
-drwxr-xr-x   0 thomassatterly   (501) staff       (20)        0 2023-01-26 00:35:27.164292 fablab-0.0.0/src/fablab/
--rw-r--r--   0 thomassatterly   (501) staff       (20)       22 2023-01-20 02:02:56.000000 fablab-0.0.0/src/fablab/__init__.py
-drwxr-xr-x   0 thomassatterly   (501) staff       (20)        0 2023-01-26 00:35:27.165652 fablab-0.0.0/src/fablab.egg-info/
--rw-r--r--   0 thomassatterly   (501) staff       (20)     1527 2023-01-26 00:35:27.000000 fablab-0.0.0/src/fablab.egg-info/PKG-INFO
--rw-r--r--   0 thomassatterly   (501) staff       (20)      212 2023-01-26 00:35:27.000000 fablab-0.0.0/src/fablab.egg-info/SOURCES.txt
--rw-r--r--   0 thomassatterly   (501) staff       (20)        1 2023-01-26 00:35:27.000000 fablab-0.0.0/src/fablab.egg-info/dependency_links.txt
--rw-r--r--   0 thomassatterly   (501) staff       (20)        7 2023-01-26 00:35:27.000000 fablab-0.0.0/src/fablab.egg-info/top_level.txt
+drwxr-xr-x   0 thomassatterly   (501) staff       (20)        0 2023-07-02 19:49:50.214548 fablab-0.0.2/
+-rw-r--r--   0 thomassatterly   (501) staff       (20)     1030 2023-01-20 02:06:57.000000 fablab-0.0.2/LICENSE
+-rw-r--r--   0 thomassatterly   (501) staff       (20)       40 2023-01-26 00:26:50.000000 fablab-0.0.2/MANIFEST.in
+-rw-r--r--   0 thomassatterly   (501) staff       (20)     1494 2023-07-02 19:49:50.214145 fablab-0.0.2/PKG-INFO
+-rw-r--r--   0 thomassatterly   (501) staff       (20)        0 2023-01-20 01:59:48.000000 fablab-0.0.2/README.md
+-rw-r--r--   0 thomassatterly   (501) staff       (20)      559 2023-07-02 19:48:13.000000 fablab-0.0.2/pyproject.toml
+-rw-r--r--   0 thomassatterly   (501) staff       (20)       38 2023-07-02 19:49:50.214730 fablab-0.0.2/setup.cfg
+drwxr-xr-x   0 thomassatterly   (501) staff       (20)        0 2023-07-02 19:49:50.206367 fablab-0.0.2/src/
+drwxr-xr-x   0 thomassatterly   (501) staff       (20)        0 2023-07-02 19:49:50.211055 fablab-0.0.2/src/fablab/
+-rw-r--r--   0 thomassatterly   (501) staff       (20)      194 2023-07-02 19:41:22.000000 fablab-0.0.2/src/fablab/__init__.py
+-rw-r--r--   0 thomassatterly   (501) staff       (20)      405 2023-06-27 01:35:31.000000 fablab-0.0.2/src/fablab/common.py
+-rw-r--r--   0 thomassatterly   (501) staff       (20)     6441 2023-06-27 02:24:45.000000 fablab-0.0.2/src/fablab/loaders.py
+-rw-r--r--   0 thomassatterly   (501) staff       (20)     6700 2023-06-27 02:23:14.000000 fablab-0.0.2/src/fablab/savers.py
+-rw-r--r--   0 thomassatterly   (501) staff       (20)      204 2023-06-27 01:10:14.000000 fablab-0.0.2/src/fablab/utils.py
+drwxr-xr-x   0 thomassatterly   (501) staff       (20)        0 2023-07-02 19:49:50.213551 fablab-0.0.2/src/fablab.egg-info/
+-rw-r--r--   0 thomassatterly   (501) staff       (20)     1494 2023-07-02 19:49:50.000000 fablab-0.0.2/src/fablab.egg-info/PKG-INFO
+-rw-r--r--   0 thomassatterly   (501) staff       (20)      287 2023-07-02 19:49:50.000000 fablab-0.0.2/src/fablab.egg-info/SOURCES.txt
+-rw-r--r--   0 thomassatterly   (501) staff       (20)        1 2023-07-02 19:49:50.000000 fablab-0.0.2/src/fablab.egg-info/dependency_links.txt
+-rw-r--r--   0 thomassatterly   (501) staff       (20)        7 2023-07-02 19:49:50.000000 fablab-0.0.2/src/fablab.egg-info/top_level.txt
```

### Comparing `fablab-0.0.0/LICENSE` & `fablab-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fablab-0.0.0/PKG-INFO` & `fablab-0.0.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: fablab
-Version: 0.0.0
-Summary: Fabrication Labratory -- Configuration utility for building Python objects from human-readable JSON
+Version: 0.0.2
+Summary: Fabrication Labratory -- Like pickle, but uses human-readable JSON
 Author-email: Thomas Satterly <tasat@me.com>
 License: Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
         
         THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 Keywords: configuration
```

### Comparing `fablab-0.0.0/pyproject.toml` & `fablab-0.0.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fablab"
-version = "0.0.0"
-description = "Fabrication Labratory -- Configuration utility for building Python objects from human-readable JSON"
+version = "0.0.2"
+description = "Fabrication Labratory -- Like pickle, but uses human-readable JSON"
 readme = "README.md"
 authors = [{ name = "Thomas Satterly", email = "tasat@me.com"}]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
```

### Comparing `fablab-0.0.0/src/fablab.egg-info/PKG-INFO` & `fablab-0.0.2/src/fablab.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: fablab
-Version: 0.0.0
-Summary: Fabrication Labratory -- Configuration utility for building Python objects from human-readable JSON
+Version: 0.0.2
+Summary: Fabrication Labratory -- Like pickle, but uses human-readable JSON
 Author-email: Thomas Satterly <tasat@me.com>
 License: Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
         
         THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 Keywords: configuration
```

