# Comparing `tmp/sugaru-0.1.0.tar.gz` & `tmp/sugaru-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sugaru-0.1.0.tar", max compression
+gzip compressed data, was "sugaru-0.2.0.tar", max compression
```

## Comparing `sugaru-0.1.0.tar` & `sugaru-0.2.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     1063 2023-07-02 18:21:56.816316 sugaru-0.1.0/LICENSE
--rw-r--r--   0        0        0     6690 2023-07-02 18:21:56.816316 sugaru-0.1.0/README.md
--rw-r--r--   0        0        0     2932 2023-07-02 18:21:56.820316 sugaru-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      207 2023-07-02 18:21:56.820316 sugaru-0.1.0/sugaru/__init__.py
--rw-r--r--   0        0        0     4112 2023-07-02 18:21:56.820316 sugaru-0.1.0/sugaru/__main__.py
--rw-r--r--   0        0        0      361 2023-07-02 18:21:56.820316 sugaru-0.1.0/sugaru/file_loader/__init__.py
--rw-r--r--   0        0        0       43 2023-07-02 18:21:56.820316 sugaru-0.1.0/sugaru/file_loader/logging.py
--rw-r--r--   0        0        0      213 2023-07-02 18:21:56.820316 sugaru-0.1.0/sugaru/file_loader/simple_json/__init__.py
--rw-r--r--   0        0        0       27 2023-07-02 18:21:56.820316 sugaru-0.1.0/sugaru/file_loader/simple_yaml/__init__.py
--rw-r--r--   0        0        0      900 2023-07-02 18:21:56.820316 sugaru-0.1.0/sugaru/file_loader/simple_yaml/loader.py
--rw-r--r--   0        0        0       57 2023-07-02 18:21:56.820316 sugaru-0.1.0/sugaru/file_loader/types.py
--rw-r--r--   0        0        0      715 2023-07-02 18:21:56.820316 sugaru-0.1.0/sugaru/file_writer/__init__.py
--rw-r--r--   0        0        0       43 2023-07-02 18:21:56.820316 sugaru-0.1.0/sugaru/file_writer/logging.py
--rw-r--r--   0        0        0      305 2023-07-02 18:21:56.820316 sugaru-0.1.0/sugaru/file_writer/simple_json/__init__.py
--rw-r--r--   0        0        0      558 2023-07-02 18:21:56.820316 sugaru-0.1.0/sugaru/file_writer/simple_yaml/__init__.py
--rw-r--r--   0        0        0       57 2023-07-02 18:21:56.820316 sugaru-0.1.0/sugaru/file_writer/types.py
--rw-r--r--   0        0        0     1450 2023-07-02 18:21:56.820316 sugaru-0.1.0/sugaru/interfaces.py
--rw-r--r--   0        0        0      762 2023-07-02 18:21:56.820316 sugaru-0.1.0/sugaru/logging.py
--rw-r--r--   0        0        0      168 2023-07-02 18:21:56.820316 sugaru-0.1.0/sugaru/object_loader/__init__.py
--rw-r--r--   0        0        0      760 2023-07-02 18:21:56.820316 sugaru-0.1.0/sugaru/object_loader/module_loader.py
--rw-r--r--   0        0        0      386 2023-07-02 18:21:56.820316 sugaru-0.1.0/sugaru/object_loader/object_creator.py
--rw-r--r--   0        0        0      972 2023-07-02 18:21:56.820316 sugaru-0.1.0/sugaru/object_loader/objects_loader.py
--rw-r--r--   0        0        0     1921 2023-07-02 18:21:56.820316 sugaru-0.1.0/sugaru/object_loader/simple_loader.py
--rw-r--r--   0        0        0       45 2023-07-02 18:21:56.820316 sugaru-0.1.0/sugaru/plugin_executor/__init__.py
--rw-r--r--   0        0        0     1729 2023-07-02 18:21:56.820316 sugaru-0.1.0/sugaru/plugin_executor/executor.py
--rw-r--r--   0        0        0        0 2023-07-02 18:21:56.820316 sugaru-0.1.0/sugaru/py.typed
--rw-r--r--   0        0        0     2088 2023-07-02 18:21:56.820316 sugaru-0.1.0/sugaru/sugarator.py
--rw-r--r--   0        0        0      335 2023-07-02 18:21:56.824316 sugaru-0.1.0/sugaru/types.py
--rw-r--r--   0        0        0      242 2023-07-02 18:21:56.824316 sugaru-0.1.0/sugaru/utils/__init__.py
--rw-r--r--   0        0        0      746 2023-07-02 18:21:56.824316 sugaru-0.1.0/sugaru/utils/encode_decode.py
--rw-r--r--   0        0        0      507 2023-07-02 18:21:56.824316 sugaru-0.1.0/sugaru/utils/names_and_types.py
--rw-r--r--   0        0        0      551 2023-07-02 18:21:56.824316 sugaru-0.1.0/sugaru/utils/object_loading.py
--rw-r--r--   0        0        0     2695 2023-07-02 18:21:56.824316 sugaru-0.1.0/sugaru/utils/signature.py
--rw-r--r--   0        0        0     7604 1970-01-01 00:00:00.000000 sugaru-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-07-02 18:40:43.000350 sugaru-0.2.0/LICENSE
+-rw-r--r--   0        0        0     6942 2023-07-02 18:40:43.000350 sugaru-0.2.0/README.md
+-rw-r--r--   0        0        0     2932 2023-07-02 18:40:43.000350 sugaru-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      207 2023-07-02 18:40:43.000350 sugaru-0.2.0/sugaru/__init__.py
+-rw-r--r--   0        0        0     4112 2023-07-02 18:40:43.000350 sugaru-0.2.0/sugaru/__main__.py
+-rw-r--r--   0        0        0      361 2023-07-02 18:40:43.000350 sugaru-0.2.0/sugaru/file_loader/__init__.py
+-rw-r--r--   0        0        0       43 2023-07-02 18:40:43.000350 sugaru-0.2.0/sugaru/file_loader/logging.py
+-rw-r--r--   0        0        0      213 2023-07-02 18:40:43.000350 sugaru-0.2.0/sugaru/file_loader/simple_json/__init__.py
+-rw-r--r--   0        0        0       27 2023-07-02 18:40:43.000350 sugaru-0.2.0/sugaru/file_loader/simple_yaml/__init__.py
+-rw-r--r--   0        0        0      900 2023-07-02 18:40:43.000350 sugaru-0.2.0/sugaru/file_loader/simple_yaml/loader.py
+-rw-r--r--   0        0        0       57 2023-07-02 18:40:43.000350 sugaru-0.2.0/sugaru/file_loader/types.py
+-rw-r--r--   0        0        0      715 2023-07-02 18:40:43.000350 sugaru-0.2.0/sugaru/file_writer/__init__.py
+-rw-r--r--   0        0        0       43 2023-07-02 18:40:43.000350 sugaru-0.2.0/sugaru/file_writer/logging.py
+-rw-r--r--   0        0        0      305 2023-07-02 18:40:43.000350 sugaru-0.2.0/sugaru/file_writer/simple_json/__init__.py
+-rw-r--r--   0        0        0      558 2023-07-02 18:40:43.000350 sugaru-0.2.0/sugaru/file_writer/simple_yaml/__init__.py
+-rw-r--r--   0        0        0       57 2023-07-02 18:40:43.000350 sugaru-0.2.0/sugaru/file_writer/types.py
+-rw-r--r--   0        0        0     1450 2023-07-02 18:40:43.000350 sugaru-0.2.0/sugaru/interfaces.py
+-rw-r--r--   0        0        0      762 2023-07-02 18:40:43.000350 sugaru-0.2.0/sugaru/logging.py
+-rw-r--r--   0        0        0      168 2023-07-02 18:40:43.000350 sugaru-0.2.0/sugaru/object_loader/__init__.py
+-rw-r--r--   0        0        0      760 2023-07-02 18:40:43.000350 sugaru-0.2.0/sugaru/object_loader/module_loader.py
+-rw-r--r--   0        0        0      386 2023-07-02 18:40:43.000350 sugaru-0.2.0/sugaru/object_loader/object_creator.py
+-rw-r--r--   0        0        0      972 2023-07-02 18:40:43.000350 sugaru-0.2.0/sugaru/object_loader/objects_loader.py
+-rw-r--r--   0        0        0     1921 2023-07-02 18:40:43.000350 sugaru-0.2.0/sugaru/object_loader/simple_loader.py
+-rw-r--r--   0        0        0       45 2023-07-02 18:40:43.000350 sugaru-0.2.0/sugaru/plugin_executor/__init__.py
+-rw-r--r--   0        0        0     1729 2023-07-02 18:40:43.000350 sugaru-0.2.0/sugaru/plugin_executor/executor.py
+-rw-r--r--   0        0        0        0 2023-07-02 18:40:43.000350 sugaru-0.2.0/sugaru/py.typed
+-rw-r--r--   0        0        0     2088 2023-07-02 18:40:43.000350 sugaru-0.2.0/sugaru/sugarator.py
+-rw-r--r--   0        0        0      335 2023-07-02 18:40:43.004350 sugaru-0.2.0/sugaru/types.py
+-rw-r--r--   0        0        0      242 2023-07-02 18:40:43.004350 sugaru-0.2.0/sugaru/utils/__init__.py
+-rw-r--r--   0        0        0      746 2023-07-02 18:40:43.004350 sugaru-0.2.0/sugaru/utils/encode_decode.py
+-rw-r--r--   0        0        0      507 2023-07-02 18:40:43.004350 sugaru-0.2.0/sugaru/utils/names_and_types.py
+-rw-r--r--   0        0        0      551 2023-07-02 18:40:43.004350 sugaru-0.2.0/sugaru/utils/object_loading.py
+-rw-r--r--   0        0        0     2695 2023-07-02 18:40:43.004350 sugaru-0.2.0/sugaru/utils/signature.py
+-rw-r--r--   0        0        0     7856 1970-01-01 00:00:00.000000 sugaru-0.2.0/PKG-INFO
```

### Comparing `sugaru-0.1.0/LICENSE` & `sugaru-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sugaru-0.1.0/README.md` & `sugaru-0.2.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
 <p align="center">
-  <a href="https://pypi.org/project/sugaru/"><img width="300px" src="https://github.com/Mityuha/sugaru/assets/17745407/c4429d72-8e53-49d5-97c2-f6421c6a320c" alt='sugaru'></a>
+  <a href="https://pypi.org/project/sugaru/"><img width="300px" src="https://github.com/Mityuha/sugaru/assets/17745407/4b25b429-620e-4718-8643-70b11cde0065" alt='sugaru'></a>
 </p>
 <p align="center">
     <em>🍭 Your own syntax you've always been dreaming of. 🍭</em>
 </p>
 
 ---
 
@@ -27,15 +27,15 @@
 
 ```shell
 $ pip3 install sugaru
 ```
 
 ## Table of contents
    * [Quickstart](#quickstart)
-   * [How it works](#how-it-works)
+   * [How it actually works](#how-it-actually-works)
    * [Preparations under the hood](#preparations-under-the-hood)
    * [How objects are loaded](#how-objects-are-loaded)
    * [Examples](#examples)
    * [Dependencies](#dependencies)
    * [Changelog](#changelog)
 
 ## Quickstart
@@ -92,20 +92,24 @@
     }
 ```
 Let's put our plugins into the file called `python_tests.py`. And put our awesome yml syntax into the file called `.my-gitlab-ci.yml`.   
 To make it work simply type:
 ```bash
 $ python3 -m sugaru .my-gitlab-ci.yml --plugin python_tests
 ```
-That's it. You will see the correct `.gitlab-ci.yml` syntax output on your screen.
+That's it. You will see the correct `.gitlab-ci.yml` syntax output on your screen.  
+<p align="left">
+  <img width="400px" src="https://github.com/Mityuha/sugaru/assets/17745407/b47f9353-1f95-4407-83fb-13fb18abfa91" alt='how-it-works-no-detail'>
+</p>
+This picture illustrates how sugaru works in a nutshell.
 
-## How it works
+## How it actually works
 There are some classes under the hood that work as a pipeline:    
 <p align="left">
-  <img width="400px" src="https://github.com/Mityuha/sugaru/assets/17745407/2b101211-bf91-46d3-9717-2f121987e713" alt='how-it-works'>
+  <img width="400px" src="https://github.com/Mityuha/sugaru/assets/17745407/c94cda75-b50c-48d8-827b-62d50e9d94f3" alt='how-it-works'>
 </p>
 There is a file path as an entry point parameter (e.g. path to `.my-gitlab-ci.yml`). Then the output of every component is the input of the next component.
 
 * File Loader  
   * Output: file content as any JSON type
 * Section Encoder
   * Output: sections, i.e. mapping section-name: section-content.
@@ -120,15 +124,15 @@
 
 ## Preparations under the hood
 There is the default implementation for every component listed above.    
 Instead of using default components, you can define your own ones.    
 If you do so, such components are loaded by Object Loader component.    
 
 <p align="left">
-  <img width="600px" src="https://github.com/Mityuha/sugaru/assets/17745407/82c4f32c-b3d0-498c-a3fb-68580cf836b3" alt='components-loading'>
+  <img width="600px" src="https://github.com/Mityuha/sugaru/assets/17745407/f1c97b38-a469-4d72-900a-c02eff81f956" alt='components-loading'>
 </p>
 
 And what about the Object Loader component itself?    
 Actually, you can even implement a custom Object Loader component. Such the custom Object Loader will be loaded by default Object Loader first and then will *replace* the default one.
 
 ## How objects are loaded
 All custom defined objects -- including user plugins -- are loaded by interfaces.
```

### Comparing `sugaru-0.1.0/pyproject.toml` & `sugaru-0.2.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 lines_after_imports = 2
 include_trailing_comma = true
 use_parentheses= true
 
 
 [tool.poetry]
 name = "sugaru"
-version = "0.1.0"
+version = "0.2.0"
 description = "Create your own syntax stupidly simple!"
 readme = "README.md"
 license = "MIT"
 authors = ["Dmitry Makarov <mit.makaroff@gmail.com>"]
 classifiers = [
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
```

### Comparing `sugaru-0.1.0/sugaru/__main__.py` & `sugaru-0.2.0/sugaru/__main__.py`

 * *Files identical despite different names*

### Comparing `sugaru-0.1.0/sugaru/file_loader/simple_yaml/loader.py` & `sugaru-0.2.0/sugaru/file_loader/simple_yaml/loader.py`

 * *Files identical despite different names*

### Comparing `sugaru-0.1.0/sugaru/file_writer/__init__.py` & `sugaru-0.2.0/sugaru/file_writer/__init__.py`

 * *Files identical despite different names*

### Comparing `sugaru-0.1.0/sugaru/file_writer/simple_yaml/__init__.py` & `sugaru-0.2.0/sugaru/file_writer/simple_yaml/__init__.py`

 * *Files identical despite different names*

### Comparing `sugaru-0.1.0/sugaru/interfaces.py` & `sugaru-0.2.0/sugaru/interfaces.py`

 * *Files identical despite different names*

### Comparing `sugaru-0.1.0/sugaru/logging.py` & `sugaru-0.2.0/sugaru/logging.py`

 * *Files identical despite different names*

### Comparing `sugaru-0.1.0/sugaru/object_loader/module_loader.py` & `sugaru-0.2.0/sugaru/object_loader/module_loader.py`

 * *Files identical despite different names*

### Comparing `sugaru-0.1.0/sugaru/object_loader/objects_loader.py` & `sugaru-0.2.0/sugaru/object_loader/objects_loader.py`

 * *Files identical despite different names*

### Comparing `sugaru-0.1.0/sugaru/object_loader/simple_loader.py` & `sugaru-0.2.0/sugaru/object_loader/simple_loader.py`

 * *Files identical despite different names*

### Comparing `sugaru-0.1.0/sugaru/plugin_executor/executor.py` & `sugaru-0.2.0/sugaru/plugin_executor/executor.py`

 * *Files identical despite different names*

### Comparing `sugaru-0.1.0/sugaru/sugarator.py` & `sugaru-0.2.0/sugaru/sugarator.py`

 * *Files identical despite different names*

### Comparing `sugaru-0.1.0/sugaru/utils/encode_decode.py` & `sugaru-0.2.0/sugaru/utils/encode_decode.py`

 * *Files identical despite different names*

### Comparing `sugaru-0.1.0/sugaru/utils/object_loading.py` & `sugaru-0.2.0/sugaru/utils/object_loading.py`

 * *Files identical despite different names*

### Comparing `sugaru-0.1.0/sugaru/utils/signature.py` & `sugaru-0.2.0/sugaru/utils/signature.py`

 * *Files identical despite different names*

### Comparing `sugaru-0.1.0/PKG-INFO` & `sugaru-0.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sugaru
-Version: 0.1.0
+Version: 0.2.0
 Summary: Create your own syntax stupidly simple!
 License: MIT
 Author: Dmitry Makarov
 Author-email: mit.makaroff@gmail.com
 Requires-Python: >=3.7
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -20,15 +20,15 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: yaml
 Requires-Dist: typer[all] (>=0.9.0,<0.10.0)
 Description-Content-Type: text/markdown
 
 
 <p align="center">
-  <a href="https://pypi.org/project/sugaru/"><img width="300px" src="https://github.com/Mityuha/sugaru/assets/17745407/c4429d72-8e53-49d5-97c2-f6421c6a320c" alt='sugaru'></a>
+  <a href="https://pypi.org/project/sugaru/"><img width="300px" src="https://github.com/Mityuha/sugaru/assets/17745407/4b25b429-620e-4718-8643-70b11cde0065" alt='sugaru'></a>
 </p>
 <p align="center">
     <em>🍭 Your own syntax you've always been dreaming of. 🍭</em>
 </p>
 
 ---
 
@@ -51,15 +51,15 @@
 
 ```shell
 $ pip3 install sugaru
 ```
 
 ## Table of contents
    * [Quickstart](#quickstart)
-   * [How it works](#how-it-works)
+   * [How it actually works](#how-it-actually-works)
    * [Preparations under the hood](#preparations-under-the-hood)
    * [How objects are loaded](#how-objects-are-loaded)
    * [Examples](#examples)
    * [Dependencies](#dependencies)
    * [Changelog](#changelog)
 
 ## Quickstart
@@ -116,20 +116,24 @@
     }
 ```
 Let's put our plugins into the file called `python_tests.py`. And put our awesome yml syntax into the file called `.my-gitlab-ci.yml`.   
 To make it work simply type:
 ```bash
 $ python3 -m sugaru .my-gitlab-ci.yml --plugin python_tests
 ```
-That's it. You will see the correct `.gitlab-ci.yml` syntax output on your screen.
+That's it. You will see the correct `.gitlab-ci.yml` syntax output on your screen.  
+<p align="left">
+  <img width="400px" src="https://github.com/Mityuha/sugaru/assets/17745407/b47f9353-1f95-4407-83fb-13fb18abfa91" alt='how-it-works-no-detail'>
+</p>
+This picture illustrates how sugaru works in a nutshell.
 
-## How it works
+## How it actually works
 There are some classes under the hood that work as a pipeline:    
 <p align="left">
-  <img width="400px" src="https://github.com/Mityuha/sugaru/assets/17745407/2b101211-bf91-46d3-9717-2f121987e713" alt='how-it-works'>
+  <img width="400px" src="https://github.com/Mityuha/sugaru/assets/17745407/c94cda75-b50c-48d8-827b-62d50e9d94f3" alt='how-it-works'>
 </p>
 There is a file path as an entry point parameter (e.g. path to `.my-gitlab-ci.yml`). Then the output of every component is the input of the next component.
 
 * File Loader  
   * Output: file content as any JSON type
 * Section Encoder
   * Output: sections, i.e. mapping section-name: section-content.
@@ -144,15 +148,15 @@
 
 ## Preparations under the hood
 There is the default implementation for every component listed above.    
 Instead of using default components, you can define your own ones.    
 If you do so, such components are loaded by Object Loader component.    
 
 <p align="left">
-  <img width="600px" src="https://github.com/Mityuha/sugaru/assets/17745407/82c4f32c-b3d0-498c-a3fb-68580cf836b3" alt='components-loading'>
+  <img width="600px" src="https://github.com/Mityuha/sugaru/assets/17745407/f1c97b38-a469-4d72-900a-c02eff81f956" alt='components-loading'>
 </p>
 
 And what about the Object Loader component itself?    
 Actually, you can even implement a custom Object Loader component. Such the custom Object Loader will be loaded by default Object Loader first and then will *replace* the default one.
 
 ## How objects are loaded
 All custom defined objects -- including user plugins -- are loaded by interfaces.
```

