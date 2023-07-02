# Comparing `tmp/target_permutation_importances-1.0.2.tar.gz` & `tmp/target_permutation_importances-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "target_permutation_importances-1.0.2.tar", max compression
+gzip compressed data, was "target_permutation_importances-1.0.3.tar", max compression
```

## Comparing `target_permutation_importances-1.0.2.tar` & `target_permutation_importances-1.0.3.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     6169 2023-07-02 14:55:08.507731 target_permutation_importances-1.0.2/README.md
--rw-r--r--   0        0        0      792 2023-07-02 14:55:08.507731 target_permutation_importances-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     7363 2023-07-02 14:55:08.507731 target_permutation_importances-1.0.2/target_permutation_importances/__init__.py
--rw-r--r--   0        0        0     6762 1970-01-01 00:00:00.000000 target_permutation_importances-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     6835 2023-07-02 16:13:49.892000 target_permutation_importances-1.0.3/README.md
+-rw-r--r--   0        0        0      818 2023-07-02 16:13:49.892000 target_permutation_importances-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     7363 2023-07-02 16:13:49.892000 target_permutation_importances-1.0.3/target_permutation_importances/__init__.py
+-rw-r--r--   0        0        0     7428 1970-01-01 00:00:00.000000 target_permutation_importances-1.0.3/PKG-INFO
```

### Comparing `target_permutation_importances-1.0.2/README.md` & `target_permutation_importances-1.0.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,16 @@
 # Target Permutation Importances
 
+[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json)](https://github.com/kingychiu/target-permutation-importances)
+[![image](https://img.shields.io/pypi/v/target-permutation-importances.svg)](https://pypi.python.org/pypi/target-permutation-importances)
+[![image](https://img.shields.io/pypi/pyversions/target-permutation-importances.svg)](https://pypi.python.org/pypi/target-permutation-importances)
+[![Actions status](https://github.com/kingychiu/target-permutation-importances/workflows/CI/badge.svg)](https://github.com/kingychiu/target-permutation-importances/actions/workflows/main.yaml)
+
+
+
 ## Overview
 This method aims to lower the feature attribution due to a feature's variance.
 If a feature shows high importance to a model after the target vector is shuffled, it fits the noise.
 
 Overall, this package 
 
 1. Fit the given model class $M$ times to get $M$ actual feature importances of feature f: $A_f = [a_{f_1},a_{f_2}...a_{f_M}]$.
@@ -66,15 +73,15 @@
 )
 ```
 
 You can find more detailed examples in the "Feature Selection Examples" section.
 
 ## Advance Usage / Customization
 This package exposes `generic_compute` to allow customization.
-Read [`target_permutation_importances.__init__.py`](./target_permutation_importances/__init__.py) for details.
+Read [`target_permutation_importances.__init__.py`](target_permutation_importances/__init__.py) for details.
 
 
 ## Feature Selection Examples
 TODO
 
 ## Benchmarks
```

### Comparing `target_permutation_importances-1.0.2/pyproject.toml` & `target_permutation_importances-1.0.3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "target-permutation-importances"
-version = "1.0.2"
+version = "1.0.3"
 description = "Compute (Target) Permutation Importances of a machine learning model"
 authors = ["Anthony Chiu <kingychiu@gmail.com>"]
 readme = "README.md"
 packages = [{include = "target_permutation_importances"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
@@ -24,11 +24,12 @@
 scikit-learn = "^1.3.0"
 pandas-stubs = "^2.0.2.230605"
 types-tqdm = "^4.65.0.1"
 xgboost = "^1.7.6"
 catboost = "^1.2"
 cmake = "^3.26.4"
 lightgbm = "^3.3.5"
+coverage-badge = "^1.1.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `target_permutation_importances-1.0.2/target_permutation_importances/__init__.py` & `target_permutation_importances-1.0.3/target_permutation_importances/__init__.py`

 * *Files identical despite different names*

### Comparing `target_permutation_importances-1.0.2/PKG-INFO` & `target_permutation_importances-1.0.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: target-permutation-importances
-Version: 1.0.2
+Version: 1.0.3
 Summary: Compute (Target) Permutation Importances of a machine learning model
 Author: Anthony Chiu
 Author-email: kingychiu@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -12,14 +12,21 @@
 Requires-Dist: numpy (>=1.25.0,<2.0.0)
 Requires-Dist: pandas (>=2.0.3,<3.0.0)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Description-Content-Type: text/markdown
 
 # Target Permutation Importances
 
+[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json)](https://github.com/kingychiu/target-permutation-importances)
+[![image](https://img.shields.io/pypi/v/target-permutation-importances.svg)](https://pypi.python.org/pypi/target-permutation-importances)
+[![image](https://img.shields.io/pypi/pyversions/target-permutation-importances.svg)](https://pypi.python.org/pypi/target-permutation-importances)
+[![Actions status](https://github.com/kingychiu/target-permutation-importances/workflows/CI/badge.svg)](https://github.com/kingychiu/target-permutation-importances/actions/workflows/main.yaml)
+
+
+
 ## Overview
 This method aims to lower the feature attribution due to a feature's variance.
 If a feature shows high importance to a model after the target vector is shuffled, it fits the noise.
 
 Overall, this package 
 
 1. Fit the given model class $M$ times to get $M$ actual feature importances of feature f: $A_f = [a_{f_1},a_{f_2}...a_{f_M}]$.
@@ -82,15 +89,15 @@
 )
 ```
 
 You can find more detailed examples in the "Feature Selection Examples" section.
 
 ## Advance Usage / Customization
 This package exposes `generic_compute` to allow customization.
-Read [`target_permutation_importances.__init__.py`](./target_permutation_importances/__init__.py) for details.
+Read [`target_permutation_importances.__init__.py`](target_permutation_importances/__init__.py) for details.
 
 
 ## Feature Selection Examples
 TODO
 
 ## Benchmarks
```

