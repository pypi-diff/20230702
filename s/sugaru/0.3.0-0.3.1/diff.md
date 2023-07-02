# Comparing `tmp/sugaru-0.3.0.tar.gz` & `tmp/sugaru-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sugaru-0.3.0.tar", max compression
+gzip compressed data, was "sugaru-0.3.1.tar", max compression
```

## Comparing `sugaru-0.3.0.tar` & `sugaru-0.3.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     1063 2023-07-02 20:21:14.838062 sugaru-0.3.0/LICENSE
--rw-r--r--   0        0        0     7045 2023-07-02 20:21:14.838062 sugaru-0.3.0/README.md
--rw-r--r--   0        0        0     2948 2023-07-02 20:21:14.838062 sugaru-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      207 2023-07-02 20:21:14.838062 sugaru-0.3.0/sugaru/__init__.py
--rw-r--r--   0        0        0     4112 2023-07-02 20:21:14.838062 sugaru-0.3.0/sugaru/__main__.py
--rw-r--r--   0        0        0      361 2023-07-02 20:21:14.838062 sugaru-0.3.0/sugaru/file_loader/__init__.py
--rw-r--r--   0        0        0       43 2023-07-02 20:21:14.838062 sugaru-0.3.0/sugaru/file_loader/logging.py
--rw-r--r--   0        0        0      213 2023-07-02 20:21:14.838062 sugaru-0.3.0/sugaru/file_loader/simple_json/__init__.py
--rw-r--r--   0        0        0       27 2023-07-02 20:21:14.838062 sugaru-0.3.0/sugaru/file_loader/simple_yaml/__init__.py
--rw-r--r--   0        0        0      900 2023-07-02 20:21:14.838062 sugaru-0.3.0/sugaru/file_loader/simple_yaml/loader.py
--rw-r--r--   0        0        0       57 2023-07-02 20:21:14.838062 sugaru-0.3.0/sugaru/file_loader/types.py
--rw-r--r--   0        0        0      715 2023-07-02 20:21:14.838062 sugaru-0.3.0/sugaru/file_writer/__init__.py
--rw-r--r--   0        0        0       43 2023-07-02 20:21:14.838062 sugaru-0.3.0/sugaru/file_writer/logging.py
--rw-r--r--   0        0        0      305 2023-07-02 20:21:14.838062 sugaru-0.3.0/sugaru/file_writer/simple_json/__init__.py
--rw-r--r--   0        0        0      558 2023-07-02 20:21:14.838062 sugaru-0.3.0/sugaru/file_writer/simple_yaml/__init__.py
--rw-r--r--   0        0        0       57 2023-07-02 20:21:14.838062 sugaru-0.3.0/sugaru/file_writer/types.py
--rw-r--r--   0        0        0     1450 2023-07-02 20:21:14.838062 sugaru-0.3.0/sugaru/interfaces.py
--rw-r--r--   0        0        0      762 2023-07-02 20:21:14.838062 sugaru-0.3.0/sugaru/logging.py
--rw-r--r--   0        0        0      168 2023-07-02 20:21:14.838062 sugaru-0.3.0/sugaru/object_loader/__init__.py
--rw-r--r--   0        0        0      760 2023-07-02 20:21:14.838062 sugaru-0.3.0/sugaru/object_loader/module_loader.py
--rw-r--r--   0        0        0      386 2023-07-02 20:21:14.838062 sugaru-0.3.0/sugaru/object_loader/object_creator.py
--rw-r--r--   0        0        0      972 2023-07-02 20:21:14.838062 sugaru-0.3.0/sugaru/object_loader/objects_loader.py
--rw-r--r--   0        0        0     1921 2023-07-02 20:21:14.838062 sugaru-0.3.0/sugaru/object_loader/simple_loader.py
--rw-r--r--   0        0        0       45 2023-07-02 20:21:14.838062 sugaru-0.3.0/sugaru/plugin_executor/__init__.py
--rw-r--r--   0        0        0     1729 2023-07-02 20:21:14.838062 sugaru-0.3.0/sugaru/plugin_executor/executor.py
--rw-r--r--   0        0        0        0 2023-07-02 20:21:14.838062 sugaru-0.3.0/sugaru/py.typed
--rw-r--r--   0        0        0     2088 2023-07-02 20:21:14.842062 sugaru-0.3.0/sugaru/sugarator.py
--rw-r--r--   0        0        0      335 2023-07-02 20:21:14.842062 sugaru-0.3.0/sugaru/types.py
--rw-r--r--   0        0        0      242 2023-07-02 20:21:14.842062 sugaru-0.3.0/sugaru/utils/__init__.py
--rw-r--r--   0        0        0      746 2023-07-02 20:21:14.842062 sugaru-0.3.0/sugaru/utils/encode_decode.py
--rw-r--r--   0        0        0      507 2023-07-02 20:21:14.842062 sugaru-0.3.0/sugaru/utils/names_and_types.py
--rw-r--r--   0        0        0      551 2023-07-02 20:21:14.842062 sugaru-0.3.0/sugaru/utils/object_loading.py
--rw-r--r--   0        0        0     2695 2023-07-02 20:21:14.842062 sugaru-0.3.0/sugaru/utils/signature.py
--rw-r--r--   0        0        0     8012 1970-01-01 00:00:00.000000 sugaru-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-07-02 20:33:31.443252 sugaru-0.3.1/LICENSE
+-rw-r--r--   0        0        0     7045 2023-07-02 20:33:31.443252 sugaru-0.3.1/README.md
+-rw-r--r--   0        0        0     2910 2023-07-02 20:33:31.447252 sugaru-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0      207 2023-07-02 20:33:31.447252 sugaru-0.3.1/sugaru/__init__.py
+-rw-r--r--   0        0        0     4112 2023-07-02 20:33:31.447252 sugaru-0.3.1/sugaru/__main__.py
+-rw-r--r--   0        0        0      361 2023-07-02 20:33:31.447252 sugaru-0.3.1/sugaru/file_loader/__init__.py
+-rw-r--r--   0        0        0       43 2023-07-02 20:33:31.447252 sugaru-0.3.1/sugaru/file_loader/logging.py
+-rw-r--r--   0        0        0      213 2023-07-02 20:33:31.447252 sugaru-0.3.1/sugaru/file_loader/simple_json/__init__.py
+-rw-r--r--   0        0        0       27 2023-07-02 20:33:31.447252 sugaru-0.3.1/sugaru/file_loader/simple_yaml/__init__.py
+-rw-r--r--   0        0        0      900 2023-07-02 20:33:31.447252 sugaru-0.3.1/sugaru/file_loader/simple_yaml/loader.py
+-rw-r--r--   0        0        0       57 2023-07-02 20:33:31.447252 sugaru-0.3.1/sugaru/file_loader/types.py
+-rw-r--r--   0        0        0      715 2023-07-02 20:33:31.447252 sugaru-0.3.1/sugaru/file_writer/__init__.py
+-rw-r--r--   0        0        0       43 2023-07-02 20:33:31.447252 sugaru-0.3.1/sugaru/file_writer/logging.py
+-rw-r--r--   0        0        0      305 2023-07-02 20:33:31.447252 sugaru-0.3.1/sugaru/file_writer/simple_json/__init__.py
+-rw-r--r--   0        0        0      558 2023-07-02 20:33:31.447252 sugaru-0.3.1/sugaru/file_writer/simple_yaml/__init__.py
+-rw-r--r--   0        0        0       57 2023-07-02 20:33:31.447252 sugaru-0.3.1/sugaru/file_writer/types.py
+-rw-r--r--   0        0        0     1450 2023-07-02 20:33:31.447252 sugaru-0.3.1/sugaru/interfaces.py
+-rw-r--r--   0        0        0      762 2023-07-02 20:33:31.447252 sugaru-0.3.1/sugaru/logging.py
+-rw-r--r--   0        0        0      168 2023-07-02 20:33:31.447252 sugaru-0.3.1/sugaru/object_loader/__init__.py
+-rw-r--r--   0        0        0      760 2023-07-02 20:33:31.447252 sugaru-0.3.1/sugaru/object_loader/module_loader.py
+-rw-r--r--   0        0        0      386 2023-07-02 20:33:31.447252 sugaru-0.3.1/sugaru/object_loader/object_creator.py
+-rw-r--r--   0        0        0      972 2023-07-02 20:33:31.447252 sugaru-0.3.1/sugaru/object_loader/objects_loader.py
+-rw-r--r--   0        0        0     1921 2023-07-02 20:33:31.447252 sugaru-0.3.1/sugaru/object_loader/simple_loader.py
+-rw-r--r--   0        0        0       45 2023-07-02 20:33:31.447252 sugaru-0.3.1/sugaru/plugin_executor/__init__.py
+-rw-r--r--   0        0        0     1729 2023-07-02 20:33:31.447252 sugaru-0.3.1/sugaru/plugin_executor/executor.py
+-rw-r--r--   0        0        0        0 2023-07-02 20:33:31.447252 sugaru-0.3.1/sugaru/py.typed
+-rw-r--r--   0        0        0     2088 2023-07-02 20:33:31.447252 sugaru-0.3.1/sugaru/sugarator.py
+-rw-r--r--   0        0        0      335 2023-07-02 20:33:31.447252 sugaru-0.3.1/sugaru/types.py
+-rw-r--r--   0        0        0      242 2023-07-02 20:33:31.447252 sugaru-0.3.1/sugaru/utils/__init__.py
+-rw-r--r--   0        0        0      746 2023-07-02 20:33:31.447252 sugaru-0.3.1/sugaru/utils/encode_decode.py
+-rw-r--r--   0        0        0      507 2023-07-02 20:33:31.447252 sugaru-0.3.1/sugaru/utils/names_and_types.py
+-rw-r--r--   0        0        0      551 2023-07-02 20:33:31.447252 sugaru-0.3.1/sugaru/utils/object_loading.py
+-rw-r--r--   0        0        0     2695 2023-07-02 20:33:31.451252 sugaru-0.3.1/sugaru/utils/signature.py
+-rw-r--r--   0        0        0     7973 1970-01-01 00:00:00.000000 sugaru-0.3.1/PKG-INFO
```

### Comparing `sugaru-0.3.0/LICENSE` & `sugaru-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sugaru-0.3.0/README.md` & `sugaru-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `sugaru-0.3.0/pyproject.toml` & `sugaru-0.3.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 lines_after_imports = 2
 include_trailing_comma = true
 use_parentheses= true
 
 
 [tool.poetry]
 name = "sugaru"
-version = "0.3.0"
+version = "0.3.1"
 description = "Create your own syntax stupidly simple!"
 readme = "README.md"
 license = "MIT"
 authors = ["Dmitry Makarov <mit.makaroff@gmail.com>"]
 classifiers = [
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
@@ -58,14 +58,15 @@
 
 
 [tool.poetry.dependencies]
 python = ">=3.7"
 typer = {extras = ["all"], version = "^0.9.0"}
 PyYAML = "^6.0"
 
+
 [tool.poetry.dev-dependencies]
 black = "*"
 mypy = ">1.0.0"
 isort = "*"
 pre-commit = "*"
 ruff = "*"
 pytest = "*"
@@ -77,16 +78,14 @@
 docformatter = "*"
 PyYAML = "*"
 loguru = "*"
 tox = "^4.5.2"
 typing-extensions = "^4.6.2"
 importlib-metadata = "^6.6.0"
 
-[tool.poetry.extras]
-yaml = ["pyyaml"]
 
 [tool.mypy]
 # https://mypy.readthedocs.io/en/stable/config_file.html
 python_version = "3.10"
 exclude = ["examples", "sugaru/__init__.py", "sugaru/mypy.py"]
 warn_unused_configs = true
 ignore_missing_imports = true
```

### Comparing `sugaru-0.3.0/sugaru/__main__.py` & `sugaru-0.3.1/sugaru/__main__.py`

 * *Files identical despite different names*

### Comparing `sugaru-0.3.0/sugaru/file_loader/simple_yaml/loader.py` & `sugaru-0.3.1/sugaru/file_loader/simple_yaml/loader.py`

 * *Files identical despite different names*

### Comparing `sugaru-0.3.0/sugaru/file_writer/__init__.py` & `sugaru-0.3.1/sugaru/file_writer/__init__.py`

 * *Files identical despite different names*

### Comparing `sugaru-0.3.0/sugaru/file_writer/simple_yaml/__init__.py` & `sugaru-0.3.1/sugaru/file_writer/simple_yaml/__init__.py`

 * *Files identical despite different names*

### Comparing `sugaru-0.3.0/sugaru/interfaces.py` & `sugaru-0.3.1/sugaru/interfaces.py`

 * *Files identical despite different names*

### Comparing `sugaru-0.3.0/sugaru/logging.py` & `sugaru-0.3.1/sugaru/logging.py`

 * *Files identical despite different names*

### Comparing `sugaru-0.3.0/sugaru/object_loader/module_loader.py` & `sugaru-0.3.1/sugaru/object_loader/module_loader.py`

 * *Files identical despite different names*

### Comparing `sugaru-0.3.0/sugaru/object_loader/objects_loader.py` & `sugaru-0.3.1/sugaru/object_loader/objects_loader.py`

 * *Files identical despite different names*

### Comparing `sugaru-0.3.0/sugaru/object_loader/simple_loader.py` & `sugaru-0.3.1/sugaru/object_loader/simple_loader.py`

 * *Files identical despite different names*

### Comparing `sugaru-0.3.0/sugaru/plugin_executor/executor.py` & `sugaru-0.3.1/sugaru/plugin_executor/executor.py`

 * *Files identical despite different names*

### Comparing `sugaru-0.3.0/sugaru/sugarator.py` & `sugaru-0.3.1/sugaru/sugarator.py`

 * *Files identical despite different names*

### Comparing `sugaru-0.3.0/sugaru/utils/encode_decode.py` & `sugaru-0.3.1/sugaru/utils/encode_decode.py`

 * *Files identical despite different names*

### Comparing `sugaru-0.3.0/sugaru/utils/object_loading.py` & `sugaru-0.3.1/sugaru/utils/object_loading.py`

 * *Files identical despite different names*

### Comparing `sugaru-0.3.0/sugaru/utils/signature.py` & `sugaru-0.3.1/sugaru/utils/signature.py`

 * *Files identical despite different names*

### Comparing `sugaru-0.3.0/PKG-INFO` & `sugaru-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sugaru
-Version: 0.3.0
+Version: 0.3.1
 Summary: Create your own syntax stupidly simple!
 License: MIT
 Author: Dmitry Makarov
 Author-email: mit.makaroff@gmail.com
 Requires-Python: >=3.7
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -14,16 +14,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Provides-Extra: yaml
-Requires-Dist: PyYAML (>=6.0,<7.0) ; extra == "yaml"
+Requires-Dist: PyYAML (>=6.0,<7.0)
 Requires-Dist: typer[all] (>=0.9.0,<0.10.0)
 Description-Content-Type: text/markdown
 
 
 <p align="center">
   <a href="https://pypi.org/project/sugaru/"><img width="300px" src="https://github.com/Mityuha/sugaru/assets/17745407/4b25b429-620e-4718-8643-70b11cde0065" alt='sugaru'></a>
 </p>
```

