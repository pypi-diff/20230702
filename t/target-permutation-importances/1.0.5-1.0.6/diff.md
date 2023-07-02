# Comparing `tmp/target_permutation_importances-1.0.5.tar.gz` & `tmp/target_permutation_importances-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "target_permutation_importances-1.0.5.tar", max compression
+gzip compressed data, was "target_permutation_importances-1.0.6.tar", max compression
```

## Comparing `target_permutation_importances-1.0.5.tar` & `target_permutation_importances-1.0.6.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     6835 2023-07-02 17:14:24.911185 target_permutation_importances-1.0.5/README.md
--rw-r--r--   0        0        0      818 2023-07-02 17:14:24.911185 target_permutation_importances-1.0.5/pyproject.toml
--rw-r--r--   0        0        0     7363 2023-07-02 17:14:24.911185 target_permutation_importances-1.0.5/target_permutation_importances/__init__.py
--rw-r--r--   0        0        0     7428 1970-01-01 00:00:00.000000 target_permutation_importances-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0     6835 2023-07-02 17:24:42.192437 target_permutation_importances-1.0.6/README.md
+-rw-r--r--   0        0        0      818 2023-07-02 17:24:42.196437 target_permutation_importances-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0     7363 2023-07-02 17:24:42.196437 target_permutation_importances-1.0.6/target_permutation_importances/__init__.py
+-rw-r--r--   0        0        0     7428 1970-01-01 00:00:00.000000 target_permutation_importances-1.0.6/PKG-INFO
```

### Comparing `target_permutation_importances-1.0.5/README.md` & `target_permutation_importances-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `target_permutation_importances-1.0.5/pyproject.toml` & `target_permutation_importances-1.0.6/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "target-permutation-importances"
-version = "1.0.5"
+version = "1.0.6"
 description = "Compute (Target) Permutation Importances of a machine learning model"
 authors = ["Anthony Chiu <kingychiu@gmail.com>"]
 readme = "README.md"
 packages = [{include = "target_permutation_importances"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
-numpy = "^1.25.0"
+numpy = "^1.21.0"
 pandas = "^1.5.3"
-tqdm = "^4.65.0"
+tqdm = "^4.48.2"
 
 
 [tool.poetry.group.dev.dependencies]
 ruff = "^0.0.275"
 black = "^23.3.0"
 isort = "^5.12.0"
 mypy = "^1.4.1"
```

### Comparing `target_permutation_importances-1.0.5/target_permutation_importances/__init__.py` & `target_permutation_importances-1.0.6/target_permutation_importances/__init__.py`

 * *Files identical despite different names*

### Comparing `target_permutation_importances-1.0.5/PKG-INFO` & `target_permutation_importances-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: target-permutation-importances
-Version: 1.0.5
+Version: 1.0.6
 Summary: Compute (Target) Permutation Importances of a machine learning model
 Author: Anthony Chiu
 Author-email: kingychiu@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: numpy (>=1.25.0,<2.0.0)
+Requires-Dist: numpy (>=1.21.0,<2.0.0)
 Requires-Dist: pandas (>=1.5.3,<2.0.0)
-Requires-Dist: tqdm (>=4.65.0,<5.0.0)
+Requires-Dist: tqdm (>=4.48.2,<5.0.0)
 Description-Content-Type: text/markdown
 
 # Target Permutation Importances
 
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json)](https://github.com/kingychiu/target-permutation-importances)
 [![image](https://img.shields.io/pypi/v/target-permutation-importances.svg)](https://pypi.python.org/pypi/target-permutation-importances)
 [![image](https://img.shields.io/pypi/pyversions/target-permutation-importances.svg)](https://pypi.python.org/pypi/target-permutation-importances)
```

