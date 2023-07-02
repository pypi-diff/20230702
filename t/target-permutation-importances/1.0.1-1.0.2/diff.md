# Comparing `tmp/target_permutation_importances-1.0.1.tar.gz` & `tmp/target_permutation_importances-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "target_permutation_importances-1.0.1.tar", max compression
+gzip compressed data, was "target_permutation_importances-1.0.2.tar", max compression
```

## Comparing `target_permutation_importances-1.0.1.tar` & `target_permutation_importances-1.0.2.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     6079 2023-07-02 10:12:25.830020 target_permutation_importances-1.0.1/README.md
--rw-r--r--   0        0        0      792 2023-07-02 10:12:25.834020 target_permutation_importances-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     7742 2023-07-02 10:12:25.834020 target_permutation_importances-1.0.1/target_permutation_importances/__init__.py
--rw-r--r--   0        0        0     6672 1970-01-01 00:00:00.000000 target_permutation_importances-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     6169 2023-07-02 14:55:08.507731 target_permutation_importances-1.0.2/README.md
+-rw-r--r--   0        0        0      792 2023-07-02 14:55:08.507731 target_permutation_importances-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     7363 2023-07-02 14:55:08.507731 target_permutation_importances-1.0.2/target_permutation_importances/__init__.py
+-rw-r--r--   0        0        0     6762 1970-01-01 00:00:00.000000 target_permutation_importances-1.0.2/PKG-INFO
```

### Comparing `target_permutation_importances-1.0.1/README.md` & `target_permutation_importances-1.0.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 
 ## Overview
 This method aims to lower the feature attribution due to a feature's variance.
 If a feature shows high importance to a model after the target vector is shuffled, it fits the noise.
 
 Overall, this package 
 
-1. Fit the given model class $M$ times to get $M$ actual feature importances ($A$).
-2. Fit the given model class with shuffled targets for $N$ times to get $N$ feature random importances ($R$).
-3. Compute the final importances by various methods, such as:
-    - $A - R$ 
-    - $A / (MinMaxScale(R) + 1)$
+1. Fit the given model class $M$ times to get $M$ actual feature importances of feature f: $A_f = [a_{f_1},a_{f_2}...a_{f_M}]$.
+2. Fit the given model class with shuffled targets for $N$ times to get $N$ feature random importances: $R_f = [r_{f_1},r_{f_2}...r_{f_N}]$.
+3. Compute the final importances of a feature $f$ by various methods, such as:
+    - $A_f$ - $R_f$
+    - $A_f$ - ($R_f + 1)$
 
 Not to be confused with [sklearn.inspection.permutation_importance](https://scikit-learn.org/stable/modules/generated/sklearn.inspection.permutation_importance.html#sklearn.inspection.permutation_importance),
 this sklearn method is about feature permutation instead of target permutation.
 
 This method were originally proposed/implemented by:
 - [Permutation importance: a corrected feature importance measure](https://academic.oup.com/bioinformatics/article/26/10/1340/193348)
 - [Feature Selection with Null Importances
```

### Comparing `target_permutation_importances-1.0.1/pyproject.toml` & `target_permutation_importances-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "target-permutation-importances"
-version = "1.0.1"
+version = "1.0.2"
 description = "Compute (Target) Permutation Importances of a machine learning model"
 authors = ["Anthony Chiu <kingychiu@gmail.com>"]
 readme = "README.md"
 packages = [{include = "target_permutation_importances"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `target_permutation_importances-1.0.1/target_permutation_importances/__init__.py` & `target_permutation_importances-1.0.2/target_permutation_importances/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -56,25 +56,25 @@
     )
     # Sort by feature name to make sure the order is the same
     mean_actual_importance_df = mean_actual_importance_df.sort_index()
     mean_random_importance_df = mean_random_importance_df.sort_index()
     assert (mean_random_importance_df.index == mean_actual_importance_df.index).all()
 
     # Calculate the signal to noise ratio
-    mean_actual_importance_df["permutation_importance"] = mean_actual_importance_df[
+    mean_actual_importance_df["importance"] = mean_actual_importance_df[
         "importance"
     ] - (mean_random_importance_df["importance"])
     mean_actual_importance_df["mean_actual_importance"] = mean_actual_importance_df[
         "importance"
     ]
     mean_actual_importance_df["mean_random_importance"] = mean_random_importance_df[
         "importance"
     ]
     return mean_actual_importance_df[
-        ["permutation_importance", "mean_actual_importance", "mean_random_importance"]
+        ["importance", "mean_actual_importance", "mean_random_importance"]
     ].reset_index()
 
 
 def compute_permutation_importance_by_division(
     actual_importance_dfs: List[pd.DataFrame], random_importance_dfs: List[pd.DataFrame]
 ) -> pd.DataFrame:
     # Calculate the mean importance
@@ -86,34 +86,26 @@
         pd.concat(random_importance_dfs).groupby("feature").mean()
     )
     # Sort by feature name to make sure the order is the same
     mean_actual_importance_df = mean_actual_importance_df.sort_index()
     mean_random_importance_df = mean_random_importance_df.sort_index()
     assert (mean_random_importance_df.index == mean_actual_importance_df.index).all()
 
-    # MinMax scale the random importance + 1
-    random_min = mean_random_importance_df["importance"].min()
-    random_max = mean_random_importance_df["importance"].max()
-    mean_random_importance_df["importance"] -= random_min
-    mean_random_importance_df["importance"] /= random_max - random_min
-    mean_random_importance_df["importance"] += 1
-
     # Calculate the signal to noise ratio
-    mean_actual_importance_df["permutation_importance"] = mean_actual_importance_df[
+    mean_actual_importance_df["importance"] = mean_actual_importance_df[
         "importance"
-    ] / (mean_random_importance_df["importance"])
+    ] / (mean_random_importance_df["importance"] + 1)
     mean_actual_importance_df["mean_actual_importance"] = mean_actual_importance_df[
         "importance"
     ]
     mean_actual_importance_df["mean_random_importance"] = mean_random_importance_df[
         "importance"
     ]
-
     return mean_actual_importance_df[
-        ["permutation_importance", "mean_actual_importance", "mean_random_importance"]
+        ["importance", "mean_actual_importance", "mean_random_importance"]
     ].reset_index()
 
 
 def _compute_one_run(
     model_builder: ModelBuilderType,
     model_fitter: ModelFitterType,
     model_importance_calculator: ModelImportanceCalculatorType,
@@ -206,15 +198,15 @@
         if "LGBM" in str(model.__class__):
             feature_attr = "feature_name_"
         elif "Cat" in str(model.__class__):
             feature_attr = "feature_names_"
 
         return pd.DataFrame(
             {
-                "feature": feature_attr,
+                "feature": getattr(model, feature_attr),
                 "importance": model.feature_importances_,
             }
         )
 
     return generic_compute(
         model_builder=_model_builder,
         model_fitter=_model_fitter,
```

### Comparing `target_permutation_importances-1.0.1/PKG-INFO` & `target_permutation_importances-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: target-permutation-importances
-Version: 1.0.1
+Version: 1.0.2
 Summary: Compute (Target) Permutation Importances of a machine learning model
 Author: Anthony Chiu
 Author-email: kingychiu@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -18,19 +18,19 @@
 
 ## Overview
 This method aims to lower the feature attribution due to a feature's variance.
 If a feature shows high importance to a model after the target vector is shuffled, it fits the noise.
 
 Overall, this package 
 
-1. Fit the given model class $M$ times to get $M$ actual feature importances ($A$).
-2. Fit the given model class with shuffled targets for $N$ times to get $N$ feature random importances ($R$).
-3. Compute the final importances by various methods, such as:
-    - $A - R$ 
-    - $A / (MinMaxScale(R) + 1)$
+1. Fit the given model class $M$ times to get $M$ actual feature importances of feature f: $A_f = [a_{f_1},a_{f_2}...a_{f_M}]$.
+2. Fit the given model class with shuffled targets for $N$ times to get $N$ feature random importances: $R_f = [r_{f_1},r_{f_2}...r_{f_N}]$.
+3. Compute the final importances of a feature $f$ by various methods, such as:
+    - $A_f$ - $R_f$
+    - $A_f$ - ($R_f + 1)$
 
 Not to be confused with [sklearn.inspection.permutation_importance](https://scikit-learn.org/stable/modules/generated/sklearn.inspection.permutation_importance.html#sklearn.inspection.permutation_importance),
 this sklearn method is about feature permutation instead of target permutation.
 
 This method were originally proposed/implemented by:
 - [Permutation importance: a corrected feature importance measure](https://academic.oup.com/bioinformatics/article/26/10/1340/193348)
 - [Feature Selection with Null Importances
```

