# Comparing `tmp/target_permutation_importances-1.0.0.tar.gz` & `tmp/target_permutation_importances-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "target_permutation_importances-1.0.0.tar", max compression
+gzip compressed data, was "target_permutation_importances-1.0.1.tar", max compression
```

## Comparing `target_permutation_importances-1.0.0.tar` & `target_permutation_importances-1.0.1.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     5850 2023-07-02 09:08:35.742949 target_permutation_importances-1.0.0/README.md
--rw-r--r--   0        0        0      717 2023-07-02 09:08:35.742949 target_permutation_importances-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     7535 2023-07-02 09:08:35.742949 target_permutation_importances-1.0.0/target_permutation_importances/__init__.py
--rw-r--r--   0        0        0     6443 1970-01-01 00:00:00.000000 target_permutation_importances-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     6079 2023-07-02 10:12:25.830020 target_permutation_importances-1.0.1/README.md
+-rw-r--r--   0        0        0      792 2023-07-02 10:12:25.834020 target_permutation_importances-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     7742 2023-07-02 10:12:25.834020 target_permutation_importances-1.0.1/target_permutation_importances/__init__.py
+-rw-r--r--   0        0        0     6672 1970-01-01 00:00:00.000000 target_permutation_importances-1.0.1/PKG-INFO
```

### Comparing `target_permutation_importances-1.0.0/README.md` & `target_permutation_importances-1.0.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Target Permutation Importances
 
 ## Overview
-This method aims at lower the feature attribution due to the variance of a feature.
-If a feature is important after the target vector is shuffled, it is fitting to noise.
+This method aims to lower the feature attribution due to a feature's variance.
+If a feature shows high importance to a model after the target vector is shuffled, it fits the noise.
 
 Overall, this package 
 
 1. Fit the given model class $M$ times to get $M$ actual feature importances ($A$).
 2. Fit the given model class with shuffled targets for $N$ times to get $N$ feature random importances ($R$).
 3. Compute the final importances by various methods, such as:
     - $A - R$ 
@@ -17,48 +17,64 @@
 
 This method were originally proposed/implemented by:
 - [Permutation importance: a corrected feature importance measure](https://academic.oup.com/bioinformatics/article/26/10/1340/193348)
 - [Feature Selection with Null Importances
 ](https://www.kaggle.com/code/ogrellier/feature-selection-with-null-importances/notebook)
 
 
+## Install
+
+```
+pip install target-permutation-importances
+```
+or
+```
+poetry add target-permutation-importances
+```
+
 ## Basic Usage
 
 ```python
 # Import the function
 from target_permutation_importances import compute
 
 # Prepare a dataset
+import pandas as pd
 from sklearn.datasets import load_breast_cancer
+
+# Models
+from catboost import CatBoostClassifier
+from lightgbm import LGBMClassifier
 from sklearn.ensemble import RandomForestClassifier
-import pandas as pd
+from xgboost import XGBClassifier
 
 data = load_breast_cancer()
 
+# Convert to a pandas dataframe
+Xpd = pd.DataFrame(data.data, columns=data.feature_names)
+
 # Compute permutation importances with default settings
 result_df = compute(
-    # RandomForestClassifier, XGBClassifier, CatBoostClassifier, LGBMClassifier...
-    model_cls=RandomForestClassifier,
+    model_cls=RandomForestClassifier, # Or other models
     model_cls_params={ # The params for the model class construction
         "n_estimators": 1,
     },
     model_fit_params={}, # The params for model.fit
     X=Xpd,
     y=data.target,
     num_actual_runs=2,
     num_random_runs=10,
-    permutation_importance_calculator=compute_permutation_importance_by_subtraction,
 )
 ```
 
 You can find more detailed examples in the "Feature Selection Examples" section.
 
 ## Advance Usage / Customization
-Instead of calling `compute` this package also expose `generic_compute` to allow customization.
-Read `target_permutation_importances.__init__` for details.
+This package exposes `generic_compute` to allow customization.
+Read [`target_permutation_importances.__init__.py`](./target_permutation_importances/__init__.py) for details.
 
 
 ## Feature Selection Examples
 TODO
 
 ## Benchmarks
 
@@ -71,22 +87,22 @@
 - `xgboost.XGBClassifier`
 - `xgboost.XGBRegressor`
 - `catboost.CatBoostClassifier`
 - `catboost.CatBoostRegressor`
 - `lightgbm.LGBMClassifier`
 - `lightgbm.LGBMRegressor`
 
-For binary classification task, `sklearn.metrics.f1_score` is used for evaluation. For regression task, `sklearn.metrics.mean_squared_error` is used for evaluation.
+For the binary classification task, `sklearn.metrics.f1_score` is used for evaluation. For the regression task, `sklearn.metrics.mean_squared_error` is used for evaluation.
 
 The downloaded datasets are divided into 3 sections: `train`: 50%, `val`: 10%, `test`: 40%.
 Feature importance is calculated from the `train` set. Feature selection is done on the `val` set. 
 The final benchmark is evaluated on the `test` set. Therefore the `test` set is unseen to both the feature importance and selection process.
 
 
-Raw result data are in `target-permutation-importances/benchmarks/results/tabular_benchmark.csv`.
+Raw result data are in [`benchmarks/results/tabular_benchmark.csv`](benchmarks/results/tabular_benchmark.csv).
 
 ## Kaggle Competitions
 Many Kaggle Competition top solutions involve this method, here are some examples
 
 | Year | Competition                                                                                                                  | Medal | Link                                                                                                                                        |
 | ---- | ---------------------------------------------------------------------------------------------------------------------------- | ----- | ------------------------------------------------------------------------------------------------------------------------------------------- |
 | 2023 | [Predict Student Performance from Game Play](https://www.kaggle.com/competitions/predict-student-performance-from-game-play) | Gold  | [3rd place solution](https://www.kaggle.com/competitions/predict-student-performance-from-game-play/discussion/420235)                      |
@@ -94,23 +110,23 @@
 | 2018 | [Home Credit Default Risk](https://www.kaggle.com/competitions/home-credit-default-risk/overview)                            | Gold  | [10th place solution](https://www.kaggle.com/competitions/home-credit-default-risk/discussion/64598)                                        |
 
 
 ## Development Setup and Contribution Guide
 **Python Version**
 
 You can find the suggested development Python version in `.python-version`.
-You might consider setting up `Pyenv` if you want to have multiple Python versions in your machine.
+You might consider setting up `Pyenv` if you want to have multiple Python versions on your machine.
 
 **Python packages**
 
-This repository is setup with `Poetry`. If you are not familiar with Poetry, you can find packages requirements are listed in `pyproject.toml`. 
-Otherwise, you can just set up with `poetry install`
+This repository is setup with `Poetry`. If you are not familiar with Poetry, you can find package requirements listed in `pyproject.toml`. 
+Otherwise, you can just set it up with `poetry install`
 
 **Run Benchmarks**
 
-To run benchmark locally on your machine, run `make run_tabular_benchmark` or `python -m benchmarks.run_tabular_benchmark`
+To run the benchmark locally on your machine, run `make run_tabular_benchmark` or `python -m benchmarks.run_tabular_benchmark`
 
 **Make Changes**
 
 Following the [Make Changes Guide from Github](https://github.com/github/docs/blob/main/CONTRIBUTING.md#make-changes)
 Before committing or merging, please run the linters defined in `make lint` and the tests defined in `make test`
```

### Comparing `target_permutation_importances-1.0.0/pyproject.toml` & `target_permutation_importances-1.0.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "target-permutation-importances"
-version = "1.0.0"
+version = "1.0.1"
 description = "Compute (Target) Permutation Importances of a machine learning model"
 authors = ["Anthony Chiu <kingychiu@gmail.com>"]
 readme = "README.md"
 packages = [{include = "target_permutation_importances"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
@@ -20,11 +20,15 @@
 mypy = "^1.4.1"
 pytest = "^7.4.0"
 pytest-cov = "^4.1.0"
 datasets = "^2.13.1"
 scikit-learn = "^1.3.0"
 pandas-stubs = "^2.0.2.230605"
 types-tqdm = "^4.65.0.1"
+xgboost = "^1.7.6"
+catboost = "^1.2"
+cmake = "^3.26.4"
+lightgbm = "^3.3.5"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `target_permutation_importances-1.0.0/target_permutation_importances/__init__.py` & `target_permutation_importances-1.0.1/target_permutation_importances/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -198,17 +198,23 @@
     def _model_builder() -> Any:
         return model_cls(**model_cls_params)
 
     def _model_fitter(model: Any, X: XType, y: YType) -> Any:
         return model.fit(X, y, **model_fit_params)
 
     def _model_importance_calculator(model: Any, X: XType, y: YType) -> pd.DataFrame:
+        feature_attr = "feature_names_in_"
+        if "LGBM" in str(model.__class__):
+            feature_attr = "feature_name_"
+        elif "Cat" in str(model.__class__):
+            feature_attr = "feature_names_"
+
         return pd.DataFrame(
             {
-                "feature": model.feature_names_in_,
+                "feature": feature_attr,
                 "importance": model.feature_importances_,
             }
         )
 
     return generic_compute(
         model_builder=_model_builder,
         model_fitter=_model_fitter,
```

### Comparing `target_permutation_importances-1.0.0/PKG-INFO` & `target_permutation_importances-1.0.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: target-permutation-importances
-Version: 1.0.0
+Version: 1.0.1
 Summary: Compute (Target) Permutation Importances of a machine learning model
 Author: Anthony Chiu
 Author-email: kingychiu@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -13,16 +13,16 @@
 Requires-Dist: pandas (>=2.0.3,<3.0.0)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Description-Content-Type: text/markdown
 
 # Target Permutation Importances
 
 ## Overview
-This method aims at lower the feature attribution due to the variance of a feature.
-If a feature is important after the target vector is shuffled, it is fitting to noise.
+This method aims to lower the feature attribution due to a feature's variance.
+If a feature shows high importance to a model after the target vector is shuffled, it fits the noise.
 
 Overall, this package 
 
 1. Fit the given model class $M$ times to get $M$ actual feature importances ($A$).
 2. Fit the given model class with shuffled targets for $N$ times to get $N$ feature random importances ($R$).
 3. Compute the final importances by various methods, such as:
     - $A - R$ 
@@ -33,48 +33,64 @@
 
 This method were originally proposed/implemented by:
 - [Permutation importance: a corrected feature importance measure](https://academic.oup.com/bioinformatics/article/26/10/1340/193348)
 - [Feature Selection with Null Importances
 ](https://www.kaggle.com/code/ogrellier/feature-selection-with-null-importances/notebook)
 
 
+## Install
+
+```
+pip install target-permutation-importances
+```
+or
+```
+poetry add target-permutation-importances
+```
+
 ## Basic Usage
 
 ```python
 # Import the function
 from target_permutation_importances import compute
 
 # Prepare a dataset
+import pandas as pd
 from sklearn.datasets import load_breast_cancer
+
+# Models
+from catboost import CatBoostClassifier
+from lightgbm import LGBMClassifier
 from sklearn.ensemble import RandomForestClassifier
-import pandas as pd
+from xgboost import XGBClassifier
 
 data = load_breast_cancer()
 
+# Convert to a pandas dataframe
+Xpd = pd.DataFrame(data.data, columns=data.feature_names)
+
 # Compute permutation importances with default settings
 result_df = compute(
-    # RandomForestClassifier, XGBClassifier, CatBoostClassifier, LGBMClassifier...
-    model_cls=RandomForestClassifier,
+    model_cls=RandomForestClassifier, # Or other models
     model_cls_params={ # The params for the model class construction
         "n_estimators": 1,
     },
     model_fit_params={}, # The params for model.fit
     X=Xpd,
     y=data.target,
     num_actual_runs=2,
     num_random_runs=10,
-    permutation_importance_calculator=compute_permutation_importance_by_subtraction,
 )
 ```
 
 You can find more detailed examples in the "Feature Selection Examples" section.
 
 ## Advance Usage / Customization
-Instead of calling `compute` this package also expose `generic_compute` to allow customization.
-Read `target_permutation_importances.__init__` for details.
+This package exposes `generic_compute` to allow customization.
+Read [`target_permutation_importances.__init__.py`](./target_permutation_importances/__init__.py) for details.
 
 
 ## Feature Selection Examples
 TODO
 
 ## Benchmarks
 
@@ -87,22 +103,22 @@
 - `xgboost.XGBClassifier`
 - `xgboost.XGBRegressor`
 - `catboost.CatBoostClassifier`
 - `catboost.CatBoostRegressor`
 - `lightgbm.LGBMClassifier`
 - `lightgbm.LGBMRegressor`
 
-For binary classification task, `sklearn.metrics.f1_score` is used for evaluation. For regression task, `sklearn.metrics.mean_squared_error` is used for evaluation.
+For the binary classification task, `sklearn.metrics.f1_score` is used for evaluation. For the regression task, `sklearn.metrics.mean_squared_error` is used for evaluation.
 
 The downloaded datasets are divided into 3 sections: `train`: 50%, `val`: 10%, `test`: 40%.
 Feature importance is calculated from the `train` set. Feature selection is done on the `val` set. 
 The final benchmark is evaluated on the `test` set. Therefore the `test` set is unseen to both the feature importance and selection process.
 
 
-Raw result data are in `target-permutation-importances/benchmarks/results/tabular_benchmark.csv`.
+Raw result data are in [`benchmarks/results/tabular_benchmark.csv`](benchmarks/results/tabular_benchmark.csv).
 
 ## Kaggle Competitions
 Many Kaggle Competition top solutions involve this method, here are some examples
 
 | Year | Competition                                                                                                                  | Medal | Link                                                                                                                                        |
 | ---- | ---------------------------------------------------------------------------------------------------------------------------- | ----- | ------------------------------------------------------------------------------------------------------------------------------------------- |
 | 2023 | [Predict Student Performance from Game Play](https://www.kaggle.com/competitions/predict-student-performance-from-game-play) | Gold  | [3rd place solution](https://www.kaggle.com/competitions/predict-student-performance-from-game-play/discussion/420235)                      |
@@ -110,24 +126,24 @@
 | 2018 | [Home Credit Default Risk](https://www.kaggle.com/competitions/home-credit-default-risk/overview)                            | Gold  | [10th place solution](https://www.kaggle.com/competitions/home-credit-default-risk/discussion/64598)                                        |
 
 
 ## Development Setup and Contribution Guide
 **Python Version**
 
 You can find the suggested development Python version in `.python-version`.
-You might consider setting up `Pyenv` if you want to have multiple Python versions in your machine.
+You might consider setting up `Pyenv` if you want to have multiple Python versions on your machine.
 
 **Python packages**
 
-This repository is setup with `Poetry`. If you are not familiar with Poetry, you can find packages requirements are listed in `pyproject.toml`. 
-Otherwise, you can just set up with `poetry install`
+This repository is setup with `Poetry`. If you are not familiar with Poetry, you can find package requirements listed in `pyproject.toml`. 
+Otherwise, you can just set it up with `poetry install`
 
 **Run Benchmarks**
 
-To run benchmark locally on your machine, run `make run_tabular_benchmark` or `python -m benchmarks.run_tabular_benchmark`
+To run the benchmark locally on your machine, run `make run_tabular_benchmark` or `python -m benchmarks.run_tabular_benchmark`
 
 **Make Changes**
 
 Following the [Make Changes Guide from Github](https://github.com/github/docs/blob/main/CONTRIBUTING.md#make-changes)
 Before committing or merging, please run the linters defined in `make lint` and the tests defined in `make test`
```

