# Comparing `tmp/target_permutation_importances-1.0.4.tar.gz` & `tmp/target_permutation_importances-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "target_permutation_importances-1.0.4.tar", max compression
+gzip compressed data, was "target_permutation_importances-1.0.5.tar", max compression
```

## Comparing `target_permutation_importances-1.0.4.tar` & `target_permutation_importances-1.0.5.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     6835 2023-07-02 17:11:25.753122 target_permutation_importances-1.0.4/README.md
--rw-r--r--   0        0        0      818 2023-07-02 17:11:25.753122 target_permutation_importances-1.0.4/pyproject.toml
--rw-r--r--   0        0        0     7363 2023-07-02 17:11:25.753122 target_permutation_importances-1.0.4/target_permutation_importances/__init__.py
--rw-r--r--   0        0        0     7428 1970-01-01 00:00:00.000000 target_permutation_importances-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0     6835 2023-07-02 17:14:24.911185 target_permutation_importances-1.0.5/README.md
+-rw-r--r--   0        0        0      818 2023-07-02 17:14:24.911185 target_permutation_importances-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0     7363 2023-07-02 17:14:24.911185 target_permutation_importances-1.0.5/target_permutation_importances/__init__.py
+-rw-r--r--   0        0        0     7428 1970-01-01 00:00:00.000000 target_permutation_importances-1.0.5/PKG-INFO
```

### Comparing `target_permutation_importances-1.0.4/README.md` & `target_permutation_importances-1.0.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 Overall, this package 
 
 1. Fit the given model class $M$ times to get $M$ actual feature importances of feature f: $A_f = [a_{f_1},a_{f_2}...a_{f_M}]$.
 2. Fit the given model class with shuffled targets for $N$ times to get $N$ feature random importances: $R_f = [r_{f_1},r_{f_2}...r_{f_N}]$.
 3. Compute the final importances of a feature $f$ by various methods, such as:
     - $A_f$ - $R_f$
-    - $A_f$ - ($R_f + 1)$
+    - $A_f$ / ($R_f + 1)$
 
 Not to be confused with [sklearn.inspection.permutation_importance](https://scikit-learn.org/stable/modules/generated/sklearn.inspection.permutation_importance.html#sklearn.inspection.permutation_importance),
 this sklearn method is about feature permutation instead of target permutation.
 
 This method were originally proposed/implemented by:
 - [Permutation importance: a corrected feature importance measure](https://academic.oup.com/bioinformatics/article/26/10/1340/193348)
 - [Feature Selection with Null Importances
```

### Comparing `target_permutation_importances-1.0.4/pyproject.toml` & `target_permutation_importances-1.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "target-permutation-importances"
-version = "1.0.4"
+version = "1.0.5"
 description = "Compute (Target) Permutation Importances of a machine learning model"
 authors = ["Anthony Chiu <kingychiu@gmail.com>"]
 readme = "README.md"
 packages = [{include = "target_permutation_importances"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `target_permutation_importances-1.0.4/target_permutation_importances/__init__.py` & `target_permutation_importances-1.0.5/target_permutation_importances/__init__.py`

 * *Files identical despite different names*

### Comparing `target_permutation_importances-1.0.4/PKG-INFO` & `target_permutation_importances-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: target-permutation-importances
-Version: 1.0.4
+Version: 1.0.5
 Summary: Compute (Target) Permutation Importances of a machine learning model
 Author: Anthony Chiu
 Author-email: kingychiu@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -29,15 +29,15 @@
 
 Overall, this package 
 
 1. Fit the given model class $M$ times to get $M$ actual feature importances of feature f: $A_f = [a_{f_1},a_{f_2}...a_{f_M}]$.
 2. Fit the given model class with shuffled targets for $N$ times to get $N$ feature random importances: $R_f = [r_{f_1},r_{f_2}...r_{f_N}]$.
 3. Compute the final importances of a feature $f$ by various methods, such as:
     - $A_f$ - $R_f$
-    - $A_f$ - ($R_f + 1)$
+    - $A_f$ / ($R_f + 1)$
 
 Not to be confused with [sklearn.inspection.permutation_importance](https://scikit-learn.org/stable/modules/generated/sklearn.inspection.permutation_importance.html#sklearn.inspection.permutation_importance),
 this sklearn method is about feature permutation instead of target permutation.
 
 This method were originally proposed/implemented by:
 - [Permutation importance: a corrected feature importance measure](https://academic.oup.com/bioinformatics/article/26/10/1340/193348)
 - [Feature Selection with Null Importances
```

