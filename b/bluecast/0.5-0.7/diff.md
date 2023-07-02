# Comparing `tmp/bluecast-0.5.tar.gz` & `tmp/bluecast-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bluecast-0.5.tar", max compression
+gzip compressed data, was "bluecast-0.7.tar", max compression
```

## Comparing `bluecast-0.5.tar` & `bluecast-0.7.tar`

### file list

```diff
@@ -1,103 +1,111 @@
--rw-r--r--   0        0        0     1076 2023-06-09 06:31:48.848397 bluecast-0.5/LICENSE
--rw-r--r--   0        0        0    18025 2023-06-25 05:34:18.251804 bluecast-0.5/README.md
--rw-r--r--   0        0        0        0 2023-06-07 04:37:38.208179 bluecast-0.5/bluecast/__init__.py
--rw-r--r--   0        0        0        0 2023-06-05 07:59:16.422757 bluecast-0.5/bluecast/blueprints/__init__.py
--rw-r--r--   0        0        0      159 2023-06-07 04:38:14.752744 bluecast-0.5/bluecast/blueprints/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      157 2023-06-07 04:41:13.295925 bluecast-0.5/bluecast/blueprints/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0    11452 2023-06-25 05:34:24.396073 bluecast-0.5/bluecast/blueprints/__pycache__/cast.cpython-310.pyc
--rw-r--r--   0        0        0     7485 2023-06-08 04:50:54.090183 bluecast-0.5/bluecast/blueprints/__pycache__/cast.cpython-38.pyc
--rw-r--r--   0        0        0    16373 2023-06-25 05:34:02.506980 bluecast-0.5/bluecast/blueprints/cast.py
--rw-r--r--   0        0        0        0 2023-06-05 07:59:16.422757 bluecast-0.5/bluecast/config/__init__.py
--rw-r--r--   0        0        0      155 2023-06-07 04:38:14.752744 bluecast-0.5/bluecast/config/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      153 2023-06-07 04:41:13.443928 bluecast-0.5/bluecast/config/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     3843 2023-06-25 05:34:24.400073 bluecast-0.5/bluecast/config/__pycache__/training_config.cpython-310.pyc
--rw-r--r--   0        0        0     3347 2023-06-08 04:35:46.974972 bluecast-0.5/bluecast/config/__pycache__/training_config.cpython-38.pyc
--rw-r--r--   0        0        0     2969 2023-06-25 05:34:02.506980 bluecast-0.5/bluecast/config/training_config.py
--rw-r--r--   0        0        0        0 2023-06-07 04:18:43.414068 bluecast-0.5/bluecast/evaluation/__init__.py
--rw-r--r--   0        0        0      159 2023-06-07 04:38:14.768744 bluecast-0.5/bluecast/evaluation/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      157 2023-06-07 04:41:13.459928 bluecast-0.5/bluecast/evaluation/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     1955 2023-06-25 05:34:24.432074 bluecast-0.5/bluecast/evaluation/__pycache__/eval_metrics.cpython-310.pyc
--rw-r--r--   0        0        0     1585 2023-06-08 04:35:46.978972 bluecast-0.5/bluecast/evaluation/__pycache__/eval_metrics.cpython-38.pyc
--rw-r--r--   0        0        0     1323 2023-06-09 12:39:11.740235 bluecast-0.5/bluecast/evaluation/__pycache__/shap_values.cpython-310.pyc
--rw-r--r--   0        0        0     1407 2023-06-08 04:35:46.978972 bluecast-0.5/bluecast/evaluation/__pycache__/shap_values.cpython-38.pyc
--rw-r--r--   0        0        0     2212 2023-06-25 05:34:02.506980 bluecast-0.5/bluecast/evaluation/eval_metrics.py
--rw-r--r--   0        0        0     1389 2023-06-09 12:39:09.708202 bluecast-0.5/bluecast/evaluation/shap_values.py
--rw-r--r--   0        0        0        0 2023-06-07 13:39:05.783478 bluecast-0.5/bluecast/general_utils/__init__.py
--rw-r--r--   0        0        0      162 2023-06-07 13:42:50.413219 bluecast-0.5/bluecast/general_utils/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      160 2023-06-07 14:07:29.547668 bluecast-0.5/bluecast/general_utils/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     2431 2023-06-08 04:36:45.751908 bluecast-0.5/bluecast/general_utils/__pycache__/general_utils.cpython-310.pyc
--rw-r--r--   0        0        0     2442 2023-06-08 04:35:46.978972 bluecast-0.5/bluecast/general_utils/__pycache__/general_utils.cpython-38.pyc
--rw-r--r--   0        0        0     2248 2023-06-08 04:28:32.967204 bluecast-0.5/bluecast/general_utils/general_utils.py
--rw-r--r--   0        0        0        0 2023-06-05 07:59:16.422757 bluecast-0.5/bluecast/ml_modelling/__init__.py
--rw-r--r--   0        0        0      161 2023-06-07 04:38:15.136750 bluecast-0.5/bluecast/ml_modelling/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      159 2023-06-07 04:41:14.219941 bluecast-0.5/bluecast/ml_modelling/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     1431 2023-06-08 04:36:46.587922 bluecast-0.5/bluecast/ml_modelling/__pycache__/base_classes.cpython-310.pyc
--rw-r--r--   0        0        0     1416 2023-06-08 04:35:46.978972 bluecast-0.5/bluecast/ml_modelling/__pycache__/base_classes.cpython-38.pyc
--rw-r--r--   0        0        0     8999 2023-06-25 05:34:25.660126 bluecast-0.5/bluecast/ml_modelling/__pycache__/xgboost.cpython-310.pyc
--rw-r--r--   0        0        0     8279 2023-06-08 04:35:46.978972 bluecast-0.5/bluecast/ml_modelling/__pycache__/xgboost.cpython-38.pyc
--rw-r--r--   0        0        0      982 2023-06-08 04:28:32.971163 bluecast-0.5/bluecast/ml_modelling/base_classes.py
--rw-r--r--   0        0        0    13523 2023-06-25 05:33:45.141515 bluecast-0.5/bluecast/ml_modelling/xgboost.py
--rw-r--r--   0        0        0        0 2023-06-05 07:59:16.422757 bluecast-0.5/bluecast/preprocessing/__init__.py
--rw-r--r--   0        0        0      162 2023-06-07 04:38:14.968747 bluecast-0.5/bluecast/preprocessing/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      160 2023-06-07 04:41:13.631931 bluecast-0.5/bluecast/preprocessing/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     1924 2023-06-23 04:26:17.139640 bluecast-0.5/bluecast/preprocessing/__pycache__/custom.cpython-310.pyc
--rw-r--r--   0        0        0     1534 2023-06-08 04:36:46.587922 bluecast-0.5/bluecast/preprocessing/__pycache__/datetime_features.cpython-310.pyc
--rw-r--r--   0        0        0     1502 2023-06-08 04:35:46.982972 bluecast-0.5/bluecast/preprocessing/__pycache__/datetime_features.cpython-38.pyc
--rw-r--r--   0        0        0     3666 2023-06-08 04:36:46.587922 bluecast-0.5/bluecast/preprocessing/__pycache__/encode_target_labels.cpython-310.pyc
--rw-r--r--   0        0        0     3656 2023-06-08 04:35:46.982972 bluecast-0.5/bluecast/preprocessing/__pycache__/encode_target_labels.cpython-38.pyc
--rw-r--r--   0        0        0     2239 2023-06-25 05:34:26.012141 bluecast-0.5/bluecast/preprocessing/__pycache__/feature_selection.cpython-310.pyc
--rw-r--r--   0        0        0     4575 2023-06-23 04:26:17.143641 bluecast-0.5/bluecast/preprocessing/__pycache__/feature_types.cpython-310.pyc
--rw-r--r--   0        0        0     4561 2023-06-08 04:35:46.982972 bluecast-0.5/bluecast/preprocessing/__pycache__/feature_types.cpython-38.pyc
--rw-r--r--   0        0        0     1167 2023-06-08 04:36:46.587922 bluecast-0.5/bluecast/preprocessing/__pycache__/nulls_and_infs.cpython-310.pyc
--rw-r--r--   0        0        0     1163 2023-06-08 04:35:46.982972 bluecast-0.5/bluecast/preprocessing/__pycache__/nulls_and_infs.cpython-38.pyc
--rw-r--r--   0        0        0     1948 2023-06-08 06:48:48.640550 bluecast-0.5/bluecast/preprocessing/__pycache__/schema_checks.cpython-310.pyc
--rw-r--r--   0        0        0     1929 2023-06-08 04:53:15.604550 bluecast-0.5/bluecast/preprocessing/__pycache__/schema_checks.cpython-38.pyc
--rw-r--r--   0        0        0     4931 2023-06-08 04:36:46.591922 bluecast-0.5/bluecast/preprocessing/__pycache__/target_encoding.cpython-310.pyc
--rw-r--r--   0        0        0     5044 2023-06-08 04:35:46.982972 bluecast-0.5/bluecast/preprocessing/__pycache__/target_encoding.cpython-38.pyc
--rw-r--r--   0        0        0     2352 2023-06-23 04:26:17.187641 bluecast-0.5/bluecast/preprocessing/__pycache__/train_test_split.cpython-310.pyc
--rw-r--r--   0        0        0     1790 2023-06-08 04:35:46.982972 bluecast-0.5/bluecast/preprocessing/__pycache__/train_test_split.cpython-38.pyc
--rw-r--r--   0        0        0     1402 2023-06-21 05:07:47.892424 bluecast-0.5/bluecast/preprocessing/custom.py
--rw-r--r--   0        0        0     1424 2023-06-08 04:28:32.971163 bluecast-0.5/bluecast/preprocessing/datetime_features.py
--rw-r--r--   0        0        0     3122 2023-06-08 04:28:32.971163 bluecast-0.5/bluecast/preprocessing/encode_target_labels.py
--rw-r--r--   0        0        0     1890 2023-06-25 05:34:02.506980 bluecast-0.5/bluecast/preprocessing/feature_selection.py
--rw-r--r--   0        0        0     6190 2023-06-21 05:07:47.896425 bluecast-0.5/bluecast/preprocessing/feature_types.py
--rw-r--r--   0        0        0      862 2023-06-08 04:28:32.971163 bluecast-0.5/bluecast/preprocessing/nulls_and_infs.py
--rw-r--r--   0        0        0     1452 2023-06-08 06:48:42.348436 bluecast-0.5/bluecast/preprocessing/schema_checks.py
--rw-r--r--   0        0        0     4561 2023-06-08 04:28:32.971163 bluecast-0.5/bluecast/preprocessing/target_encoding.py
--rw-r--r--   0        0        0     2871 2023-06-21 05:07:47.896425 bluecast-0.5/bluecast/preprocessing/train_test_split.py
--rw-r--r--   0        0        0        0 2023-06-07 04:18:43.418068 bluecast-0.5/bluecast/tests/__init__.py
--rw-r--r--   0        0        0      154 2023-06-07 04:38:14.600741 bluecast-0.5/bluecast/tests/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     8731 2023-06-25 05:34:23.192022 bluecast-0.5/bluecast/tests/__pycache__/test_cast.cpython-310-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     3156 2023-06-07 13:42:51.261239 bluecast-0.5/bluecast/tests/__pycache__/test_check_gpu_support.cpython-310-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     4342 2023-06-09 12:37:48.734873 bluecast-0.5/bluecast/tests/__pycache__/test_custom_processing_base_class.cpython-310-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     1137 2023-06-07 04:38:15.364753 bluecast-0.5/bluecast/tests/__pycache__/test_datetime_features.cpython-310-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     2392 2023-06-07 04:38:15.364753 bluecast-0.5/bluecast/tests/__pycache__/test_encode_target_labels.cpython-310-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     4803 2023-06-07 13:42:51.269239 bluecast-0.5/bluecast/tests/__pycache__/test_feature_type_detector.cpython-310-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     1597 2023-06-09 12:06:35.203065 bluecast-0.5/bluecast/tests/__pycache__/test_load_for_production.cpython-310-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     4589 2023-06-07 04:38:15.372753 bluecast-0.5/bluecast/tests/__pycache__/test_nulls_and_infs.cpython-310-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     1902 2023-06-09 12:06:35.207064 bluecast-0.5/bluecast/tests/__pycache__/test_save_to_production.cpython-310-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     2099 2023-06-08 06:48:48.672551 bluecast-0.5/bluecast/tests/__pycache__/test_schema_checks.cpython-310-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     4064 2023-06-25 05:34:26.144146 bluecast-0.5/bluecast/tests/__pycache__/test_shap_explanations.cpython-310-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     1877 2023-06-07 04:38:15.372753 bluecast-0.5/bluecast/tests/__pycache__/test_target_encoding_binary.cpython-310-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     1449 2023-06-07 04:38:15.376753 bluecast-0.5/bluecast/tests/__pycache__/test_target_encoding_multiclass.cpython-310-pytest-6.2.5.pyc
--rw-r--r--   0        0        0     2148 2023-06-07 04:54:58.773706 bluecast-0.5/bluecast/tests/__pycache__/test_train_test_split.cpython-310-pytest-6.2.5.pyc
--rw-r--r--   0        0        0        0 2023-06-07 04:18:43.418068 bluecast-0.5/bluecast/tests/make_data/__init__.py
--rw-r--r--   0        0        0      164 2023-06-07 04:38:15.360753 bluecast-0.5/bluecast/tests/make_data/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1123 2023-06-07 04:38:15.360753 bluecast-0.5/bluecast/tests/make_data/__pycache__/create_data.cpython-310.pyc
--rw-r--r--   0        0        0     1289 2023-06-07 04:18:43.418068 bluecast-0.5/bluecast/tests/make_data/create_data.py
--rw-r--r--   0        0        0     6604 2023-06-25 05:34:02.506980 bluecast-0.5/bluecast/tests/test_cast.py
--rw-r--r--   0        0        0     1328 2023-06-07 13:40:33.489843 bluecast-0.5/bluecast/tests/test_check_gpu_support.py
--rw-r--r--   0        0        0     1789 2023-06-09 12:35:55.653016 bluecast-0.5/bluecast/tests/test_custom_processing_base_class.py
--rw-r--r--   0        0        0     1097 2023-06-07 04:38:03.828575 bluecast-0.5/bluecast/tests/test_datetime_features.py
--rw-r--r--   0        0        0     1996 2023-06-07 04:38:03.792574 bluecast-0.5/bluecast/tests/test_encode_target_labels.py
--rw-r--r--   0        0        0     2608 2023-06-07 13:42:39.380960 bluecast-0.5/bluecast/tests/test_feature_type_detector.py
--rw-r--r--   0        0        0     1482 2023-06-09 05:52:17.052295 bluecast-0.5/bluecast/tests/test_load_for_production.py
--rw-r--r--   0        0        0     1575 2023-06-07 04:38:03.788574 bluecast-0.5/bluecast/tests/test_nulls_and_infs.py
--rw-r--r--   0        0        0     1020 2023-06-09 05:52:17.052295 bluecast-0.5/bluecast/tests/test_save_to_production.py
--rw-r--r--   0        0        0     2080 2023-06-08 06:48:42.364437 bluecast-0.5/bluecast/tests/test_schema_checks.py
--rw-r--r--   0        0        0     2296 2023-06-25 05:34:02.506980 bluecast-0.5/bluecast/tests/test_shap_explanations.py
--rw-r--r--   0        0        0     1337 2023-06-07 04:38:03.800574 bluecast-0.5/bluecast/tests/test_target_encoding_binary.py
--rw-r--r--   0        0        0      735 2023-06-07 04:38:03.832575 bluecast-0.5/bluecast/tests/test_target_encoding_multiclass.py
--rw-r--r--   0        0        0     1051 2023-06-07 04:53:26.008207 bluecast-0.5/bluecast/tests/test_train_test_split.py
--rw-r--r--   0        0        0     1457 2023-06-25 05:34:02.506980 bluecast-0.5/pyproject.toml
--rw-r--r--   0        0        0    19141 1970-01-01 00:00:00.000000 bluecast-0.5/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-06-09 06:31:48.848397 bluecast-0.7/LICENSE
+-rw-r--r--   0        0        0    20021 2023-06-30 06:13:52.474377 bluecast-0.7/README.md
+-rw-r--r--   0        0        0        0 2023-06-07 04:37:38.208179 bluecast-0.7/bluecast/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-05 07:59:16.422757 bluecast-0.7/bluecast/blueprints/__init__.py
+-rw-r--r--   0        0        0      159 2023-06-07 04:38:14.752744 bluecast-0.7/bluecast/blueprints/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      157 2023-06-07 04:41:13.295925 bluecast-0.7/bluecast/blueprints/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0    12782 2023-06-27 06:12:53.582996 bluecast-0.7/bluecast/blueprints/__pycache__/cast.cpython-310.pyc
+-rw-r--r--   0        0        0    12769 2023-06-27 07:43:47.489769 bluecast-0.7/bluecast/blueprints/__pycache__/cast.cpython-38.pyc
+-rw-r--r--   0        0        0    18653 2023-06-27 06:12:51.958971 bluecast-0.7/bluecast/blueprints/cast.py
+-rw-r--r--   0        0        0        0 2023-06-05 07:59:16.422757 bluecast-0.7/bluecast/config/__init__.py
+-rw-r--r--   0        0        0      155 2023-06-07 04:38:14.752744 bluecast-0.7/bluecast/config/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      153 2023-06-07 04:41:13.443928 bluecast-0.7/bluecast/config/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     3962 2023-06-29 10:56:40.664250 bluecast-0.7/bluecast/config/__pycache__/training_config.cpython-310.pyc
+-rw-r--r--   0        0        0     3612 2023-06-29 17:56:28.976335 bluecast-0.7/bluecast/config/__pycache__/training_config.cpython-38.pyc
+-rw-r--r--   0        0        0     2873 2023-06-29 15:32:18.638107 bluecast-0.7/bluecast/config/training_config.py
+-rw-r--r--   0        0        0        0 2023-06-29 09:57:47.802211 bluecast-0.7/bluecast/eda/__init__.py
+-rw-r--r--   0        0        0      152 2023-06-29 10:24:21.113333 bluecast-0.7/bluecast/eda/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     3051 2023-06-29 10:56:40.208243 bluecast-0.7/bluecast/eda/__pycache__/analyse.cpython-310.pyc
+-rw-r--r--   0        0        0     3708 2023-06-29 10:32:55.497841 bluecast-0.7/bluecast/eda/analyse.py
+-rw-r--r--   0        0        0        0 2023-06-07 04:18:43.414068 bluecast-0.7/bluecast/evaluation/__init__.py
+-rw-r--r--   0        0        0      159 2023-06-07 04:38:14.768744 bluecast-0.7/bluecast/evaluation/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      157 2023-06-07 04:41:13.459928 bluecast-0.7/bluecast/evaluation/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     1955 2023-06-29 10:24:22.109350 bluecast-0.7/bluecast/evaluation/__pycache__/eval_metrics.cpython-310.pyc
+-rw-r--r--   0        0        0     1957 2023-06-29 13:35:03.129236 bluecast-0.7/bluecast/evaluation/__pycache__/eval_metrics.cpython-38.pyc
+-rw-r--r--   0        0        0     1323 2023-06-09 12:39:11.740235 bluecast-0.7/bluecast/evaluation/__pycache__/shap_values.cpython-310.pyc
+-rw-r--r--   0        0        0     1321 2023-06-27 07:43:47.497769 bluecast-0.7/bluecast/evaluation/__pycache__/shap_values.cpython-38.pyc
+-rw-r--r--   0        0        0     2212 2023-06-28 11:13:13.084298 bluecast-0.7/bluecast/evaluation/eval_metrics.py
+-rw-r--r--   0        0        0     1389 2023-06-09 12:39:09.708202 bluecast-0.7/bluecast/evaluation/shap_values.py
+-rw-r--r--   0        0        0        0 2023-06-07 13:39:05.783478 bluecast-0.7/bluecast/general_utils/__init__.py
+-rw-r--r--   0        0        0      162 2023-06-07 13:42:50.413219 bluecast-0.7/bluecast/general_utils/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      160 2023-06-07 14:07:29.547668 bluecast-0.7/bluecast/general_utils/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     2431 2023-06-08 04:36:45.751908 bluecast-0.7/bluecast/general_utils/__pycache__/general_utils.cpython-310.pyc
+-rw-r--r--   0        0        0     2442 2023-06-08 04:35:46.978972 bluecast-0.7/bluecast/general_utils/__pycache__/general_utils.cpython-38.pyc
+-rw-r--r--   0        0        0     2248 2023-06-08 04:28:32.967204 bluecast-0.7/bluecast/general_utils/general_utils.py
+-rw-r--r--   0        0        0        0 2023-06-05 07:59:16.422757 bluecast-0.7/bluecast/ml_modelling/__init__.py
+-rw-r--r--   0        0        0      161 2023-06-07 04:38:15.136750 bluecast-0.7/bluecast/ml_modelling/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      159 2023-06-07 04:41:14.219941 bluecast-0.7/bluecast/ml_modelling/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     1431 2023-06-08 04:36:46.587922 bluecast-0.7/bluecast/ml_modelling/__pycache__/base_classes.cpython-310.pyc
+-rw-r--r--   0        0        0     1416 2023-06-08 04:35:46.978972 bluecast-0.7/bluecast/ml_modelling/__pycache__/base_classes.cpython-38.pyc
+-rw-r--r--   0        0        0     9292 2023-06-29 10:56:40.924254 bluecast-0.7/bluecast/ml_modelling/__pycache__/xgboost.cpython-310.pyc
+-rw-r--r--   0        0        0     8899 2023-06-29 15:25:20.467211 bluecast-0.7/bluecast/ml_modelling/__pycache__/xgboost.cpython-38.pyc
+-rw-r--r--   0        0        0      982 2023-06-08 04:28:32.971163 bluecast-0.7/bluecast/ml_modelling/base_classes.py
+-rw-r--r--   0        0        0    14148 2023-06-30 05:58:04.387112 bluecast-0.7/bluecast/ml_modelling/xgboost.py
+-rw-r--r--   0        0        0        0 2023-06-05 07:59:16.422757 bluecast-0.7/bluecast/preprocessing/__init__.py
+-rw-r--r--   0        0        0      162 2023-06-07 04:38:14.968747 bluecast-0.7/bluecast/preprocessing/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      160 2023-06-07 04:41:13.631931 bluecast-0.7/bluecast/preprocessing/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     1924 2023-06-23 04:26:17.139640 bluecast-0.7/bluecast/preprocessing/__pycache__/custom.cpython-310.pyc
+-rw-r--r--   0        0        0     1919 2023-06-27 07:43:47.497769 bluecast-0.7/bluecast/preprocessing/__pycache__/custom.cpython-38.pyc
+-rw-r--r--   0        0        0     1534 2023-06-08 04:36:46.587922 bluecast-0.7/bluecast/preprocessing/__pycache__/datetime_features.cpython-310.pyc
+-rw-r--r--   0        0        0     1502 2023-06-08 04:35:46.982972 bluecast-0.7/bluecast/preprocessing/__pycache__/datetime_features.cpython-38.pyc
+-rw-r--r--   0        0        0     3666 2023-06-08 04:36:46.587922 bluecast-0.7/bluecast/preprocessing/__pycache__/encode_target_labels.cpython-310.pyc
+-rw-r--r--   0        0        0     3656 2023-06-08 04:35:46.982972 bluecast-0.7/bluecast/preprocessing/__pycache__/encode_target_labels.cpython-38.pyc
+-rw-r--r--   0        0        0     2239 2023-06-27 04:06:05.910063 bluecast-0.7/bluecast/preprocessing/__pycache__/feature_selection.cpython-310.pyc
+-rw-r--r--   0        0        0     2228 2023-06-27 07:43:47.497769 bluecast-0.7/bluecast/preprocessing/__pycache__/feature_selection.cpython-38.pyc
+-rw-r--r--   0        0        0     4575 2023-06-23 04:26:17.143641 bluecast-0.7/bluecast/preprocessing/__pycache__/feature_types.cpython-310.pyc
+-rw-r--r--   0        0        0     4561 2023-06-27 07:43:47.501769 bluecast-0.7/bluecast/preprocessing/__pycache__/feature_types.cpython-38.pyc
+-rw-r--r--   0        0        0     1167 2023-06-08 04:36:46.587922 bluecast-0.7/bluecast/preprocessing/__pycache__/nulls_and_infs.cpython-310.pyc
+-rw-r--r--   0        0        0     1163 2023-06-08 04:35:46.982972 bluecast-0.7/bluecast/preprocessing/__pycache__/nulls_and_infs.cpython-38.pyc
+-rw-r--r--   0        0        0     1948 2023-06-08 06:48:48.640550 bluecast-0.7/bluecast/preprocessing/__pycache__/schema_checks.cpython-310.pyc
+-rw-r--r--   0        0        0     1982 2023-06-27 07:43:47.505769 bluecast-0.7/bluecast/preprocessing/__pycache__/schema_checks.cpython-38.pyc
+-rw-r--r--   0        0        0     4931 2023-06-08 04:36:46.591922 bluecast-0.7/bluecast/preprocessing/__pycache__/target_encoding.cpython-310.pyc
+-rw-r--r--   0        0        0     5044 2023-06-08 04:35:46.982972 bluecast-0.7/bluecast/preprocessing/__pycache__/target_encoding.cpython-38.pyc
+-rw-r--r--   0        0        0     2352 2023-06-23 04:26:17.187641 bluecast-0.7/bluecast/preprocessing/__pycache__/train_test_split.cpython-310.pyc
+-rw-r--r--   0        0        0     2332 2023-06-27 07:43:47.505769 bluecast-0.7/bluecast/preprocessing/__pycache__/train_test_split.cpython-38.pyc
+-rw-r--r--   0        0        0     1402 2023-06-21 05:07:47.892424 bluecast-0.7/bluecast/preprocessing/custom.py
+-rw-r--r--   0        0        0     1424 2023-06-08 04:28:32.971163 bluecast-0.7/bluecast/preprocessing/datetime_features.py
+-rw-r--r--   0        0        0     3122 2023-06-08 04:28:32.971163 bluecast-0.7/bluecast/preprocessing/encode_target_labels.py
+-rw-r--r--   0        0        0     1890 2023-06-27 03:46:28.907353 bluecast-0.7/bluecast/preprocessing/feature_selection.py
+-rw-r--r--   0        0        0     6190 2023-06-21 05:07:47.896425 bluecast-0.7/bluecast/preprocessing/feature_types.py
+-rw-r--r--   0        0        0      862 2023-06-08 04:28:32.971163 bluecast-0.7/bluecast/preprocessing/nulls_and_infs.py
+-rw-r--r--   0        0        0     1452 2023-06-08 06:48:42.348436 bluecast-0.7/bluecast/preprocessing/schema_checks.py
+-rw-r--r--   0        0        0     4561 2023-06-08 04:28:32.971163 bluecast-0.7/bluecast/preprocessing/target_encoding.py
+-rw-r--r--   0        0        0     2871 2023-06-21 05:07:47.896425 bluecast-0.7/bluecast/preprocessing/train_test_split.py
+-rw-r--r--   0        0        0        0 2023-06-07 04:18:43.418068 bluecast-0.7/bluecast/tests/__init__.py
+-rw-r--r--   0        0        0      154 2023-06-07 04:38:14.600741 bluecast-0.7/bluecast/tests/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1797 2023-06-29 10:57:31.301060 bluecast-0.7/bluecast/tests/__pycache__/test_analyse.cpython-310-pytest-6.2.5.pyc
+-rw-r--r--   0        0        0     8753 2023-06-29 10:24:22.017348 bluecast-0.7/bluecast/tests/__pycache__/test_cast.cpython-310-pytest-6.2.5.pyc
+-rw-r--r--   0        0        0     3156 2023-06-07 13:42:51.261239 bluecast-0.7/bluecast/tests/__pycache__/test_check_gpu_support.cpython-310-pytest-6.2.5.pyc
+-rw-r--r--   0        0        0     4342 2023-06-09 12:37:48.734873 bluecast-0.7/bluecast/tests/__pycache__/test_custom_processing_base_class.cpython-310-pytest-6.2.5.pyc
+-rw-r--r--   0        0        0     1137 2023-06-07 04:38:15.364753 bluecast-0.7/bluecast/tests/__pycache__/test_datetime_features.cpython-310-pytest-6.2.5.pyc
+-rw-r--r--   0        0        0     2392 2023-06-07 04:38:15.364753 bluecast-0.7/bluecast/tests/__pycache__/test_encode_target_labels.cpython-310-pytest-6.2.5.pyc
+-rw-r--r--   0        0        0     4803 2023-06-07 13:42:51.269239 bluecast-0.7/bluecast/tests/__pycache__/test_feature_type_detector.cpython-310-pytest-6.2.5.pyc
+-rw-r--r--   0        0        0     1597 2023-06-09 12:06:35.203065 bluecast-0.7/bluecast/tests/__pycache__/test_load_for_production.cpython-310-pytest-6.2.5.pyc
+-rw-r--r--   0        0        0     4589 2023-06-07 04:38:15.372753 bluecast-0.7/bluecast/tests/__pycache__/test_nulls_and_infs.cpython-310-pytest-6.2.5.pyc
+-rw-r--r--   0        0        0     1902 2023-06-09 12:06:35.207064 bluecast-0.7/bluecast/tests/__pycache__/test_save_to_production.cpython-310-pytest-6.2.5.pyc
+-rw-r--r--   0        0        0     2099 2023-06-08 06:48:48.672551 bluecast-0.7/bluecast/tests/__pycache__/test_schema_checks.cpython-310-pytest-6.2.5.pyc
+-rw-r--r--   0        0        0     4064 2023-06-27 04:06:05.962063 bluecast-0.7/bluecast/tests/__pycache__/test_shap_explanations.cpython-310-pytest-6.2.5.pyc
+-rw-r--r--   0        0        0     1877 2023-06-07 04:38:15.372753 bluecast-0.7/bluecast/tests/__pycache__/test_target_encoding_binary.cpython-310-pytest-6.2.5.pyc
+-rw-r--r--   0        0        0     1449 2023-06-07 04:38:15.376753 bluecast-0.7/bluecast/tests/__pycache__/test_target_encoding_multiclass.cpython-310-pytest-6.2.5.pyc
+-rw-r--r--   0        0        0     2148 2023-06-07 04:54:58.773706 bluecast-0.7/bluecast/tests/__pycache__/test_train_test_split.cpython-310-pytest-6.2.5.pyc
+-rw-r--r--   0        0        0        0 2023-06-07 04:18:43.418068 bluecast-0.7/bluecast/tests/make_data/__init__.py
+-rw-r--r--   0        0        0      164 2023-06-07 04:38:15.360753 bluecast-0.7/bluecast/tests/make_data/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1123 2023-06-07 04:38:15.360753 bluecast-0.7/bluecast/tests/make_data/__pycache__/create_data.cpython-310.pyc
+-rw-r--r--   0        0        0     1289 2023-06-07 04:18:43.418068 bluecast-0.7/bluecast/tests/make_data/create_data.py
+-rw-r--r--   0        0        0     1176 2023-06-29 10:57:29.465031 bluecast-0.7/bluecast/tests/test_analyse.py
+-rw-r--r--   0        0        0     6677 2023-06-28 11:19:35.634947 bluecast-0.7/bluecast/tests/test_cast.py
+-rw-r--r--   0        0        0     1328 2023-06-07 13:40:33.489843 bluecast-0.7/bluecast/tests/test_check_gpu_support.py
+-rw-r--r--   0        0        0     1789 2023-06-09 12:35:55.653016 bluecast-0.7/bluecast/tests/test_custom_processing_base_class.py
+-rw-r--r--   0        0        0     1097 2023-06-07 04:38:03.828575 bluecast-0.7/bluecast/tests/test_datetime_features.py
+-rw-r--r--   0        0        0     1996 2023-06-07 04:38:03.792574 bluecast-0.7/bluecast/tests/test_encode_target_labels.py
+-rw-r--r--   0        0        0     2608 2023-06-07 13:42:39.380960 bluecast-0.7/bluecast/tests/test_feature_type_detector.py
+-rw-r--r--   0        0        0     1482 2023-06-09 05:52:17.052295 bluecast-0.7/bluecast/tests/test_load_for_production.py
+-rw-r--r--   0        0        0     1575 2023-06-07 04:38:03.788574 bluecast-0.7/bluecast/tests/test_nulls_and_infs.py
+-rw-r--r--   0        0        0     1020 2023-06-09 05:52:17.052295 bluecast-0.7/bluecast/tests/test_save_to_production.py
+-rw-r--r--   0        0        0     2080 2023-06-08 06:48:42.364437 bluecast-0.7/bluecast/tests/test_schema_checks.py
+-rw-r--r--   0        0        0     2296 2023-06-27 03:46:28.907353 bluecast-0.7/bluecast/tests/test_shap_explanations.py
+-rw-r--r--   0        0        0     1337 2023-06-07 04:38:03.800574 bluecast-0.7/bluecast/tests/test_target_encoding_binary.py
+-rw-r--r--   0        0        0      735 2023-06-07 04:38:03.832575 bluecast-0.7/bluecast/tests/test_target_encoding_multiclass.py
+-rw-r--r--   0        0        0     1051 2023-06-07 04:53:26.008207 bluecast-0.7/bluecast/tests/test_train_test_split.py
+-rw-r--r--   0        0        0     1478 2023-06-30 06:15:04.035657 bluecast-0.7/pyproject.toml
+-rw-r--r--   0        0        0    21171 1970-01-01 00:00:00.000000 bluecast-0.7/PKG-INFO
```

### Comparing `bluecast-0.5/LICENSE` & `bluecast-0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `bluecast-0.5/README.md` & `bluecast-0.7/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -28,15 +28,17 @@
 
 * [Installation](#installation)
   * [Installation for end users](#installation-for-end-users)
   * [Installation for developers](#installation-for-developers)
 * [General usage](#general-usage)
   * [Basic usage](#basic-usage)
   * [Advanced usage](#advanced-usage)
-    * [Custom training configuration](#custom--training-configuration)
+    * [Explanatory analysis](#explanatory-analysis)
+    * [Enable cross-validation](#enable-cross-validation)
+    * [Categorical encoding](#categorical-encoding)
     * [Custom preprocessing](#custom-preprocessing)
     * [Custom feature selection](#custom-feature-selection)
     * [Custom ML model](#custom-ml-model)
 * [Convenience features](#convenience-features)
 * [Code quality](#code-quality)
 * [Documentation](#documentation)
 * [How to contribute](#how-to-contribute)
@@ -84,14 +86,74 @@
 
 automl.fit(df_train, target_col="target")
 y_probs, y_classes = automl.predict(df_val)
 ```
 
 ### Advanced usage
 
+#### Explanatory analysis
+
+BlueCast offers a simple way to get a first overview of the data. This is
+
+#### Enable cross-validation
+
+While the default behaviour of BlueCast is to use a simple
+train-test-split, cross-validation can be enabled easily:
+
+```sh
+from bluecast.eda.analyse import (
+    bi_variate_plots,
+    correlation_heatmap,
+    correlation_to_target,
+    univariate_plots,
+)
+
+from bluecast.preprocessing.feature_types import FeatureTypeDetector
+
+# Here we automatically detect the numeric columns
+feat_type_detector = FeatureTypeDetector()
+train_data = feat_type_detector.fit_transform_feature_types(train_data)
+
+# show univariate plots
+univariate_plots(
+        train_data.loc[
+            :, feat_type_detector.num_columns  # here the target column EC1 is already included
+        ],
+        "EC1",
+    )
+
+# show bi-variate plots
+bi_variate_plots(train_data.loc[
+            :, feat_type_detector.num_columns
+        ],
+        "EC1")
+
+# show correlation heatmap
+correlation_heatmap(train_data.loc[
+            :, feat_type_detector.num_columns])
+
+# show correlation to target
+correlation_to_target(train_data.loc[
+            :, feat_type_detector.num_columns
+        ],
+        "EC1",)
+```
+
+#### Categorical encoding
+
+By default, BlueCast uses target encoding.
+This behaviour can be changed in the TrainingConfig by setting `cat_encoding_via_ml_algorithm`
+to True. This will change the expectations of `custom_last_mile_computation` though.
+If `cat_encoding_via_ml_algorithm` is set to False, `custom_last_mile_computation`
+will receive numerical features only as target encoding will apply before. If `cat_encoding_via_ml_algorithm`
+is True (default setting) `custom_last_mile_computation` will receive categorical
+features as well, because Xgboost#s inbuilt categorical encoding will be used.
+
+```sh
+
 #### Custom  training configuration
 
 Despite e2eml, BlueCast allows easy customization. Users can adjust the
 configuration and just pass it to the `BlueCast` class. Here is an example:
 
 ```sh
 from bluecast.blueprints.cast import BlueCast
@@ -401,21 +463,22 @@
 
 Despite being a lightweight library, BlueCast also includes some convenience
 with the following features:
 
 * automatic feature type detection and casting
 * automatic DataFrame schema detection: checks if unseen data has new or
   missing columns
-* categorical feature encoding
+* categorical feature encoding (target encoding or directly in Xgboost)
 * datetime feature encoding
 * automated GPU availability check and usage for Xgboost
   a fit_eval method to fit a model and evaluate it on a validation set
   to mimic production environment reality
 * functions to save and load a trained pipeline
 * shapley values
+* warnings for potential misconfigurations
 
 The fit_eval method can be used like this:
 
 ```sh
 from bluecast.blueprints.cast import BlueCast
 
 automl = BlueCast(
```

### Comparing `bluecast-0.5/bluecast/blueprints/__pycache__/cast.cpython-310.pyc` & `bluecast-0.7/bluecast/blueprints/__pycache__/cast.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun Jun 25 05:34:02 2023 UTC, .py size: 16373 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 cad1 9764 f53f 0000  o..........d.?..
+00000000: 6f0d 0d0a 0000 0000 e37d 9a64 dd48 0000  o........}.d.H..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 1601 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d02 5a02 0100 6401 6404 6c03 6d04 5a04  m.Z...d.d.l.m.Z.
 00000050: 6d05 5a05 6d06 5a06 6d07 5a07 6d08 5a08  m.Z.m.Z.m.Z.m.Z.
 00000060: 6d09 5a09 6d0a 5a0a 0100 6401 6402 6c0b  m.Z.m.Z...d.d.l.
 00000070: 5a0c 6401 6402 6c0d 5a0e 6401 6405 6c0f  Z.d.d.l.Z.d.d.l.
@@ -245,472 +245,555 @@
 00000f40: 7473 2f63 6173 742e 7079 da08 5f5f 696e  ts/cast.py..__in
 00000f50: 6974 5f5f 3c00 0000 7326 0000 0006 1106  it__<...s&......
 00000f60: 0106 0106 0106 0106 0106 0106 0106 0106  ................
 00000f70: 0102 0304 fe06 0306 0106 0106 0106 0106  ................
 00000f80: 010a 017a 1142 6c75 6543 6173 742e 5f5f  ...z.BlueCast.__
 00000f90: 696e 6974 5f5f da02 6466 da06 7265 7475  init__..df..retu
 00000fa0: 726e 6302 0000 0000 0000 0000 0000 0003  rnc.............
-00000fb0: 0000 0005 0000 0043 0000 0073 dc00 0000  .......C...s....
+00000fb0: 0000 0005 0000 0043 0000 0073 3001 0000  .......C...s0...
 00000fc0: 7c00 6a00 7307 7401 8300 7c00 5f00 7c00  |.j.s.t...|._.|.
 00000fd0: 6a00 6a02 7315 6401 7d02 7403 6a04 7c02  j.j.s.d.}.t.j.|.
 00000fe0: 7405 6402 6403 8d03 0100 7c00 6a00 6a06  t.d.d.....|.j.j.
 00000ff0: 6404 6b02 7225 6405 7d02 7403 6a04 7c02  d.k.r%d.}.t.j.|.
 00001000: 7405 6402 6403 8d03 0100 7c00 6a00 6a02  t.d.d.....|.j.j.
 00001010: 7236 7c00 6a07 7336 6406 7d02 7403 6a04  r6|.j.s6d.}.t.j.
 00001020: 7c02 7405 6402 6403 8d03 0100 7c00 6a08  |.t.d.d.....|.j.
 00001030: 7343 6407 7d02 7403 6a04 7c02 7405 6402  sCd.}.t.j.|.t.d.
 00001040: 6403 8d03 0100 7c00 6a00 6a09 740a 7c01  d.....|.j.j.t.|.
 00001050: 6a0b 8301 6b05 725a 7c00 6a00 6a02 725a  j...k.rZ|.j.j.rZ
 00001060: 6408 7d02 7403 6a04 7c02 7405 6402 6403  d.}.t.j.|.t.d.d.
-00001070: 8d03 0100 7c00 6a0c 7c01 6a0b 7600 726c  ....|.j.|.j.v.rl
-00001080: 6409 7d02 7403 6a04 7c02 7405 6402 6403  d.}.t.j.|.t.d.d.
-00001090: 8d03 0100 6400 5300 6400 5300 290a 4e61  ....d.S.d.S.).Na
-000010a0: 9301 0000 4665 6174 7572 6520 7365 6c65  ....Feature sele
-000010b0: 6374 696f 6e20 6973 2064 6973 6162 6c65  ction is disable
-000010c0: 642e 2055 7064 6174 6520 7468 6520 5472  d. Update the Tr
-000010d0: 6169 6e69 6e67 436f 6e66 6967 2070 6172  ainingConfig par
-000010e0: 616d 2027 656e 6162 6c65 5f66 6561 7475  am 'enable_featu
-000010f0: 7265 5f73 656c 6563 7469 6f6e 270a 2020  re_selection'.  
-00001100: 2020 2020 2020 2020 2020 746f 2065 6e61            to ena
-00001110: 626c 6520 6974 206f 7220 6d61 6b65 2075  ble it or make u
-00001120: 7365 206f 6620 6120 6375 7374 6f6d 2070  se of a custom p
-00001130: 7265 7072 6f63 6573 736f 7220 746f 2064  reprocessor to d
-00001140: 6f20 6974 206d 616e 7561 6c6c 7920 6475  o it manually du
-00001150: 7269 6e67 2074 6865 206c 6173 7420 6d69  ring the last mi
-00001160: 6c65 2063 6f6d 7075 7461 7469 6f6e 7320  le computations 
-00001170: 7374 6570 2e0a 2020 2020 2020 2020 2020  step..          
-00001180: 2020 4665 6174 7572 6520 7365 6c65 6374    Feature select
-00001190: 696f 6e20 6973 2072 6563 6f6d 6d65 6e64  ion is recommend
-000011a0: 6564 2066 6f72 2064 6174 6173 6574 7320  ed for datasets 
-000011b0: 7769 7468 206d 616e 7920 6665 6174 7572  with many featur
-000011c0: 6573 2028 3e31 3030 3029 2e20 466f 7220  es (>1000). For 
-000011d0: 6461 7461 7365 7473 2077 6974 6820 6120  datasets with a 
-000011e0: 736d 616c 6c20 616d 6f75 6e74 0a20 2020  small amount.   
-000011f0: 2020 2020 2020 2020 206f 6620 6665 6174           of feat
-00001200: 7572 6573 2066 6561 7475 7265 2073 656c  ures feature sel
-00001210: 6563 7469 6f6e 2069 7320 6e6f 7420 7265  ection is not re
-00001220: 636f 6d6d 656e 6465 642e 0a20 2020 2020  commended..     
-00001230: 2020 2020 2020 20e9 0200 0000 2901 da0a         .....)...
-00001240: 7374 6163 6b6c 6576 656c e901 0000 0061  stacklevel.....a
-00001250: 0501 0000 4372 6f73 7320 7661 6c69 6461  ....Cross valida
-00001260: 7469 6f6e 2069 7320 6469 7361 626c 6564  tion is disabled
-00001270: 2e20 5570 6461 7465 2074 6865 2054 7261  . Update the Tra
-00001280: 696e 696e 6743 6f6e 6669 6720 7061 7261  iningConfig para
-00001290: 6d20 2768 7970 6572 7475 6e69 6e67 5f63  m 'hypertuning_c
-000012a0: 765f 666f 6c64 7327 0a20 2020 2020 2020  v_folds'.       
-000012b0: 2020 2020 2074 6f20 656e 6162 6c65 2069       to enable i
-000012c0: 742e 2043 726f 7373 2076 616c 6964 6174  t. Cross validat
-000012d0: 696f 6e20 6973 2064 6973 6162 6c65 6420  ion is disabled 
-000012e0: 6f6e 2064 6566 6175 6c74 2074 6f20 616c  on default to al
-000012f0: 6c6f 7720 6661 7374 2070 726f 746f 7479  low fast prototy
-00001300: 7069 6e67 2e20 466f 7220 726f 6275 7374  ping. For robust
-00001310: 2068 7970 6572 7061 7261 6d65 7465 720a   hyperparameter.
-00001320: 2020 2020 2020 2020 2020 2020 7475 6e69              tuni
-00001330: 6e67 2075 7369 6e67 2061 7420 6c65 6173  ng using at leas
-00001340: 7420 3520 666f 6c64 7320 6973 2072 6563  t 5 folds is rec
-00001350: 6f6d 6d65 6e64 6564 2e61 5f01 0000 4665  ommended.a_...Fe
-00001360: 6174 7572 6520 7365 6c65 6374 696f 6e20  ature selection 
-00001370: 6973 2065 6e61 626c 6564 2062 7574 206e  is enabled but n
-00001380: 6f20 6665 6174 7572 6520 7365 6c65 6374  o feature select
-00001390: 6f72 2068 6173 2062 6565 6e20 7072 6f76  or has been prov
-000013a0: 6964 6564 2e20 4661 6c6c 696e 6720 6261  ided. Falling ba
-000013b0: 636b 2074 6f0a 2020 2020 2020 2020 2020  ck to.          
-000013c0: 2020 6372 6f73 732d 7661 6c69 6461 7465    cross-validate
-000013d0: 6420 6665 6174 7572 6520 656c 696d 696e  d feature elimin
-000013e0: 6174 696f 6e2e 2053 7065 6369 6669 6361  ation. Specifica
-000013f0: 6c6c 7920 666f 7220 736d 616c 6c20 6461  lly for small da
-00001400: 7461 7365 7473 2063 6865 636b 2074 6865  tasets check the
-00001410: 206c 6f67 7320 746f 2076 6572 6966 7920   logs to verify 
-00001420: 7468 6174 206e 6f74 2074 6f6f 0a20 2020  that not too.   
-00001430: 2020 2020 2020 2020 206d 616e 7920 6665           many fe
-00001440: 6174 7572 6573 2068 6176 6520 6265 656e  atures have been
-00001450: 2072 656d 6f76 6564 2e20 4f74 6865 7277   removed. Otherw
-00001460: 6973 652c 2063 6f6e 7369 6465 7220 6469  ise, consider di
-00001470: 7361 626c 696e 6720 6665 6174 7572 6520  sabling feature 
-00001480: 7365 6c65 6374 696f 6e20 6f72 2070 726f  selection or pro
-00001490: 7669 6469 6e67 2061 2063 7573 746f 6d0a  viding a custom.
-000014a0: 2020 2020 2020 2020 2020 2020 6665 6174              feat
-000014b0: 7572 6520 7365 6c65 6374 6f72 2e61 6501  ure selector.ae.
-000014c0: 0000 4e6f 2058 6762 6f6f 7374 5475 6e65  ..No XgboostTune
-000014d0: 5061 7261 6d73 436f 6e66 6967 2068 6173  ParamsConfig has
-000014e0: 2062 6565 6e20 7072 6f76 6964 6564 2e20   been provided. 
-000014f0: 4661 6c6c 696e 6720 6261 636b 2074 6f20  Falling back to 
-00001500: 6465 6661 756c 7420 7661 6c75 6573 2e20  default values. 
-00001510: 4465 6661 756c 7420 7661 6c75 6573 0a20  Default values. 
-00001520: 2020 2020 2020 2020 2020 2068 6176 6520             have 
-00001530: 6265 656e 2063 686f 7365 6e20 746f 2073  been chosen to s
-00001540: 7065 6564 2075 7020 7468 6520 7072 6f74  peed up the prot
-00001550: 6f74 7970 696e 672e 2046 6f72 2072 6f62  otyping. For rob
-00001560: 7573 7420 6879 7065 7270 6172 616d 6574  ust hyperparamet
-00001570: 6572 2074 756e 696e 6720 636f 6e73 6964  er tuning consid
-00001580: 6572 2070 726f 7669 6469 6e67 2061 2063  er providing a c
-00001590: 7573 746f 6d0a 2020 2020 2020 2020 2020  ustom.          
-000015a0: 2020 5867 626f 6f73 7454 756e 6550 6172    XgboostTunePar
-000015b0: 616d 7343 6f6e 6669 6720 7769 7468 2061  amsConfig with a
-000015c0: 2064 6565 7065 7220 6879 7065 7270 6172   deeper hyperpar
-000015d0: 616d 6574 6572 2073 6561 7263 6820 7370  ameter search sp
-000015e0: 6163 6520 616e 6420 6120 6375 7374 6f6d  ace and a custom
-000015f0: 2054 7261 696e 696e 6743 6f6e 6669 6720   TrainingConfig 
-00001600: 746f 2065 6e61 626c 650a 2020 2020 2020  to enable.      
-00001610: 2020 2020 2020 6372 6f73 732d 7661 6c69        cross-vali
-00001620: 6461 7469 6f6e 2e61 0f01 0000 5468 6520  dation.a....The 
-00001630: 6d69 6e69 6d75 6d20 6e75 6d62 6572 206f  minimum number o
-00001640: 6620 6665 6174 7572 6573 2074 6f20 7365  f features to se
-00001650: 6c65 6374 2069 7320 6772 6561 7465 7220  lect is greater 
-00001660: 6f72 2065 7175 616c 2074 6f20 7468 6520  or equal to the 
-00001670: 6e75 6d62 6572 206f 6620 6665 6174 7572  number of featur
-00001680: 6573 2069 6e0a 2020 2020 2020 2020 2020  es in.          
-00001690: 2020 7468 6520 6461 7461 7365 7420 7768    the dataset wh
-000016a0: 696c 6520 6665 6174 7572 6520 7365 6c65  ile feature sele
-000016b0: 6374 696f 6e20 6973 2065 6e61 626c 6564  ction is enabled
-000016c0: 2e20 436f 6e73 6964 6572 2072 6564 7563  . Consider reduc
-000016d0: 696e 6720 7468 6520 6d69 6e69 6d75 6d20  ing the minimum 
-000016e0: 6e75 6d62 6572 206f 6620 6665 6174 7572  number of featur
-000016f0: 6573 2074 6f0a 2020 2020 2020 2020 2020  es to.          
-00001700: 2020 7365 6c65 6374 206f 7220 6469 7361    select or disa
-00001710: 626c 696e 6720 6665 6174 7572 6520 7365  bling feature se
-00001720: 6c65 6374 696f 6e20 7669 6120 5472 6169  lection via Trai
-00001730: 6e69 6e67 436f 6e66 6967 2e7a 8154 6865  ningConfig.z.The
-00001740: 2074 6172 6765 7420 636f 6c75 6d6e 2069   target column i
-00001750: 7320 7072 6573 656e 7420 696e 2074 6865  s present in the
-00001760: 2064 6174 6173 6574 2e20 436f 6e73 6964   dataset. Consid
-00001770: 6572 2072 656d 6f76 696e 6720 7468 6520  er removing the 
-00001780: 7461 7267 6574 2063 6f6c 756d 6e20 6672  target column fr
-00001790: 6f6d 2074 6865 0a20 2020 2020 2020 2020  om the.         
-000017a0: 2020 2064 6174 6173 6574 2074 6f20 7072     dataset to pr
-000017b0: 6576 656e 7420 6c65 616b 6167 652e 290d  event leakage.).
-000017c0: 7228 0000 0072 0a00 0000 da18 656e 6162  r(...r......enab
-000017d0: 6c65 5f66 6561 7475 7265 5f73 656c 6563  le_feature_selec
-000017e0: 7469 6f6e da08 7761 726e 696e 6773 da04  tion..warnings..
-000017f0: 7761 726e da0b 5573 6572 5761 726e 696e  warn..UserWarnin
-00001800: 67da 1468 7970 6572 7475 6e69 6e67 5f63  g..hypertuning_c
-00001810: 765f 666f 6c64 7372 2700 0000 7229 0000  v_foldsr'...r)..
-00001820: 00da 166d 696e 5f66 6561 7475 7265 735f  ...min_features_
-00001830: 746f 5f73 656c 6563 74da 036c 656e da07  to_select..len..
-00001840: 636f 6c75 6d6e 7372 2000 0000 2903 7231  columnsr ...).r1
-00001850: 0000 0072 3500 0000 da07 6d65 7373 6167  ...r5.....messag
-00001860: 6572 3200 0000 7232 0000 0072 3300 0000  er2...r2...r3...
-00001870: da0e 696e 6974 6961 6c5f 6368 6563 6b73  ..initial_checks
-00001880: 6200 0000 7334 0000 0006 0108 0108 0104  b...s4..........
-00001890: 0110 050c 0204 0110 0306 0302 ff04 0202  ................
-000018a0: fe04 0410 0406 0104 0110 0412 0206 0102  ................
-000018b0: ff04 0310 030c 0104 0114 0204 fd7a 1742  .............z.B
-000018c0: 6c75 6543 6173 742e 696e 6974 6961 6c5f  lueCast.initial_
-000018d0: 6368 6563 6b73 da0a 7461 7267 6574 5f63  checks..target_c
-000018e0: 6f6c 6303 0000 0000 0000 0000 0000 0009  olc.............
-000018f0: 0000 0007 0000 0043 0000 0073 d002 0000  .......C...s....
-00001900: 7400 8300 0100 7401 8300 7d03 7c03 a002  t.....t...}.|...
-00001910: 7c01 a101 7d01 7c03 7c00 5f03 7c00 6a03  |...}.|.|._.|.j.
-00001920: 6a04 7229 7c00 6a05 7c00 6a03 6a04 7600  j.r)|.j.|.j.j.v.
-00001930: 7229 7406 8300 7c00 5f07 7c00 6a07 a008  r)t...|._.|.j...
-00001940: 7c01 7c00 6a05 1900 a101 7c01 7c00 6a05  |.|.j.....|.|.j.
-00001950: 3c00 7c00 6a03 6a04 7c00 5f04 7c00 6a03  <.|.j.j.|._.|.j.
-00001960: 6a09 7c00 5f09 7c00 6a0a 733a 740b 8300  j.|._.|.j.s:t...
-00001970: 7c00 5f0a 7c00 a00c 7c01 a101 0100 740d  |._.|...|.....t.
-00001980: 7c01 7c02 7c00 6a0e 7c00 6a0a 6a0f 7c00  |.|.|.j.|.j.j.|.
-00001990: 6a0a 6a10 7c00 6a0a 6a11 8306 5c04 7d04  j.j.|.j.j...\.}.
-000019a0: 7d05 7d06 7d07 7c00 6a12 7297 7c00 6a12  }.}.}.|.j.r.|.j.
-000019b0: a013 7c04 7c06 a102 5c02 7d04 7d06 7c00  ..|.|...\.}.}.|.
-000019c0: 6a12 6a14 7c05 7c07 6401 6402 8d03 5c02  j.j.|.|.d.d...\.
-000019d0: 7d05 7d07 7401 8300 7d03 7c03 a002 7c04  }.}.t...}.|...|.
-000019e0: a101 7d08 7c04 6a15 6403 6404 8d01 7c06  ..}.|.j.d.d...|.
-000019f0: 6a15 6403 6404 8d01 0202 7d04 7d06 7c05  j.d.d.....}.}.|.
-00001a00: 6a15 6403 6404 8d01 7c07 6a15 6403 6404  j.d.d...|.j.d.d.
-00001a10: 8d01 0202 7d05 7d07 7c02 7c03 6a04 7600  ....}.}.|.|.j.v.
-00001a20: 7297 7c03 6a04 a016 7c02 a101 0100 7417  r.|.j...|.....t.
-00001a30: 7c04 8301 7417 7c05 8301 0202 7d04 7d05  |...t.|.....}.}.
-00001a40: 7418 7c04 7c00 6a09 8302 7418 7c05 7c00  t.|.|.j...t.|.|.
-00001a50: 6a09 8302 0202 7d04 7d05 7419 8300 7c00  j.....}.}.t...|.
-00001a60: 5f1a 7c00 6a1a a01b 7c04 a101 0100 7c00  _.|.j...|.....|.
-00001a70: 6a1a a014 7c05 a101 7d05 7c00 6a04 6405  j...|...}.|.j.d.
-00001a80: 7501 72db 7c00 6a1c 6406 6b02 72db 741d  u.r.|.j.d.k.r.t.
-00001a90: 7c03 6a04 8301 7c00 5f1e 7c00 6a1e a01f  |.j...|._.|.j...
-00001aa0: 7c04 7c06 a102 7d04 7c00 6a1e a020 7c05  |.|...}.|.j.. |.
-00001ab0: a101 7d05 6e1d 7c00 6a04 6405 7501 72f8  ..}.n.|.j.d.u.r.
-00001ac0: 7c00 6a1c 6407 6b02 72f8 7421 7c03 6a04  |.j.d.k.r.t!|.j.
-00001ad0: 8301 7c00 5f1e 7c00 6a1e a022 7c04 7c06  ..|._.|.j.."|.|.
-00001ae0: a102 7d04 7c00 6a1e a023 7c05 a101 7d05  ..}.|.j..#|...}.
-00001af0: 7c00 6a24 9001 7210 7c00 6a24 a013 7c04  |.j$..r.|.j$..|.
-00001b00: 7c06 a102 5c02 7d04 7d06 7c00 6a24 6a14  |...\.}.}.|.j$j.
-00001b10: 7c05 7c07 6401 6402 8d03 5c02 7d05 7d07  |.|.d.d...\.}.}.
-00001b20: 7c00 6a25 9001 731f 7426 7c00 6a0a 6a10  |.j%..s.t&|.j.j.
-00001b30: 7c00 6a0a 6a27 6408 8d02 7c00 5f25 7c00  |.j.j'd...|._%|.
-00001b40: 6a0a 6a28 9001 7237 7c00 6a25 a013 7c04  j.j(..r7|.j%..|.
-00001b50: 7c06 a102 5c02 7d04 7d06 7c00 6a25 6a14  |...\.}.}.|.j%j.
-00001b60: 7c05 6401 6402 8d02 5c02 7d05 7d08 7c00  |.d.d...\.}.}.|.
-00001b70: 6a29 9001 7348 742a 7c00 6a1c 7c00 6a0a  j)..sHt*|.j.|.j.
-00001b80: 7c00 6a2b 7c00 6a2c 6409 8d04 7c00 5f29  |.j+|.j,d...|._)
-00001b90: 7c00 6a29 a01b 7c04 7c05 7c06 7c07 a104  |.j)..|.|.|.|...
-00001ba0: 0100 7c00 6a0a 9001 7263 7c00 6a0a 6a2d  ..|.j...rc|.j.j-
-00001bb0: 9001 7263 742e 7c00 6a29 6a2f 7c05 640a  ..rct.|.j)j/|.d.
-00001bc0: 8303 7c00 5f30 6403 7c00 5f31 6405 5300  ..|._0d.|._1d.S.
-00001bd0: 290b 7a19 5472 6169 6e20 6120 6675 6c6c  ).z.Train a full
-00001be0: 204d 4c20 7069 7065 6c69 6e65 2e46 a901   ML pipeline.F..
-00001bf0: da0e 7072 6564 6963 746f 6e5f 6d6f 6465  ..predicton_mode
-00001c00: 54a9 01da 0464 726f 704e 721e 0000 0072  T....dropNr....r
-00001c10: 1f00 0000 2902 da0c 7261 6e64 6f6d 5f73  ....)...random_s
-00001c20: 7461 7465 723f 0000 0029 0372 2800 0000  tater?...).r(...
-00001c30: 7229 0000 0072 2a00 0000 da04 7472 6565  r)...r*.....tree
-00001c40: 2932 720f 0000 0072 1600 0000 5a1b 6669  )2r....r....Z.fi
-00001c50: 745f 7472 616e 7366 6f72 6d5f 6665 6174  t_transform_feat
-00001c60: 7572 655f 7479 7065 7372 2c00 0000 7221  ure_typesr,...r!
-00001c70: 0000 0072 2000 0000 7214 0000 0072 2e00  ...r ...r....r..
-00001c80: 0000 5a1b 6669 745f 7472 616e 7366 6f72  ..Z.fit_transfor
-00001c90: 6d5f 7461 7267 6574 5f6c 6162 656c 7372  m_target_labelsr
-00001ca0: 2200 0000 7228 0000 0072 0a00 0000 7243  "...r(...r....rC
-00001cb0: 0000 0072 1b00 0000 7223 0000 00da 0a74  ...r....r#.....t
-00001cc0: 7261 696e 5f73 697a 655a 1367 6c6f 6261  rain_sizeZ.globa
-00001cd0: 6c5f 7261 6e64 6f6d 5f73 7461 7465 5a14  l_random_stateZ.
-00001ce0: 7472 6169 6e5f 7370 6c69 745f 7374 7261  train_split_stra
-00001cf0: 7469 6679 7226 0000 00da 0d66 6974 5f74  tifyr&.....fit_t
-00001d00: 7261 6e73 666f 726d da09 7472 616e 7366  ransform..transf
-00001d10: 6f72 6dda 0b72 6573 6574 5f69 6e64 6578  orm..reset_index
-00001d20: da06 7265 6d6f 7665 7217 0000 0072 1300  ..remover....r..
-00001d30: 0000 7218 0000 0072 2f00 0000 da03 6669  ..r....r/.....fi
-00001d40: 7472 1d00 0000 7219 0000 0072 2d00 0000  tr....r....r-...
-00001d50: 5a1e 6669 745f 7461 7267 6574 5f65 6e63  Z.fit_target_enc
-00001d60: 6f64 655f 6269 6e61 7279 5f63 6c61 7373  ode_binary_class
-00001d70: da24 7472 616e 7366 6f72 6d5f 7461 7267  .$transform_targ
-00001d80: 6574 5f65 6e63 6f64 655f 6269 6e61 7279  et_encode_binary
-00001d90: 5f63 6c61 7373 721a 0000 005a 1c66 6974  _classr....Z.fit
-00001da0: 5f74 6172 6765 745f 656e 636f 6465 5f6d  _target_encode_m
-00001db0: 756c 7469 636c 6173 73da 2274 7261 6e73  ulticlass."trans
-00001dc0: 666f 726d 5f74 6172 6765 745f 656e 636f  form_target_enco
-00001dd0: 6465 5f6d 756c 7469 636c 6173 7372 2500  de_multiclassr%.
-00001de0: 0000 7227 0000 0072 1500 0000 723f 0000  ..r'...r....r?..
-00001df0: 0072 3a00 0000 7224 0000 0072 1100 0000  .r:...r$...r....
-00001e00: 7229 0000 0072 2a00 0000 5a15 6361 6c63  r)...r*...Z.calc
-00001e10: 756c 6174 655f 7368 6170 5f76 616c 7565  ulate_shap_value
-00001e20: 7372 0e00 0000 da05 6d6f 6465 6c72 3000  sr......modelr0.
-00001e30: 0000 722b 0000 0029 0972 3100 0000 7235  ..r+...).r1...r5
-00001e40: 0000 0072 4400 0000 722c 0000 00da 0778  ...rD...r,.....x
-00001e50: 5f74 7261 696e da06 785f 7465 7374 da07  _train..x_test..
-00001e60: 795f 7472 6169 6eda 0679 5f74 6573 74da  y_train..y_test.
-00001e70: 015f 7232 0000 0072 3200 0000 7233 0000  ._r2...r2...r3..
-00001e80: 0072 5000 0000 8f00 0000 73ac 0000 0006  .rP.......s.....
-00001e90: 0206 010a 0106 0108 020e 0108 0106 0308  ................
-00001ea0: 0102 ff02 fe04 0102 ff0a 060a 0106 0208  ................
-00001eb0: 010a 0202 0202 0102 0104 0106 0106 0106  ................
-00001ec0: 010c fa06 0912 0106 0106 010a ff06 030a  ................
-00001ed0: 010e 0102 010a ff0e 0302 010a ff0a 030c  ................
-00001ee0: 0112 020c 0106 0108 ff08 040c 010c 0114  ................
-00001ef0: 020c 010e 010e 0114 010c 010e 010c 0108  ................
-00001f00: 0206 0104 0108 ff06 0306 010a ff08 0402  ................
-00001f10: 0106 0106 0108 fe0a 0506 0104 0108 ff06  ................
-00001f20: 0304 010a ff08 0402 0104 0104 0104 0104  ................
-00001f30: 0108 fc12 0612 0112 010a 017a 0c42 6c75  ...........z.Blu
-00001f40: 6543 6173 742e 6669 74da 0764 665f 6576  eCast.fit..df_ev
-00001f50: 616c da0b 7461 7267 6574 5f65 7661 6c63  al..target_evalc
-00001f60: 0500 0000 0000 0000 0000 0000 0800 0000  ................
-00001f70: 0400 0000 4300 0000 732c 0000 007c 00a0  ....C...s,...|..
-00001f80: 007c 017c 04a1 0201 007c 00a0 017c 02a1  .|.|.....|...|..
-00001f90: 015c 027d 057d 0674 027c 036a 037c 057c  .\.}.}.t.|.j.|.|
-00001fa0: 0683 037d 077c 0753 0029 0161 8e02 0000  ...}.|.S.).a....
-00001fb0: 5472 6169 6e20 6120 6675 6c6c 204d 4c20  Train a full ML 
-00001fc0: 7069 7065 6c69 6e65 2061 6e64 2065 7661  pipeline and eva
-00001fd0: 6c75 6174 6520 6f6e 2061 2068 6f6c 646f  luate on a holdo
-00001fe0: 7574 2073 6574 2e0a 0a20 2020 2020 2020  ut set...       
-00001ff0: 2054 6869 7320 6973 2061 2063 6f6e 7665   This is a conve
-00002000: 6e69 656e 6365 2066 756e 6374 696f 6e20  nience function 
-00002010: 746f 2074 7261 696e 2061 6e64 2065 7661  to train and eva
-00002020: 6c75 6174 6520 6f6e 2061 2068 6f6c 646f  luate on a holdo
-00002030: 7574 2073 6574 2e20 4974 2069 7320 7265  ut set. It is re
-00002040: 636f 6d6d 656e 6465 6420 746f 2075 7365  commended to use
-00002050: 2074 6869 7320 666f 7220 6d6f 6465 6c0a   this for model.
-00002060: 2020 2020 2020 2020 6578 706c 6f72 6174          explorat
-00002070: 696f 6e2e 204f 6e20 7072 6f64 7563 7469  ion. On producti
-00002080: 6f6e 2074 6865 2073 696d 706c 6520 6669  on the simple fi
-00002090: 7428 2920 6675 6e63 7469 6f6e 2073 686f  t() function sho
-000020a0: 756c 6420 6265 2075 7365 642e 0a20 2020  uld be used..   
-000020b0: 2020 2020 203a 7061 7261 6d20 3a64 663a       :param :df:
-000020c0: 2054 616b 6573 2061 2070 616e 6461 7320   Takes a pandas 
-000020d0: 4461 7461 4672 616d 6520 636f 6e74 6169  DataFrame contai
-000020e0: 6e69 6e67 2074 6865 2074 7261 696e 696e  ning the trainin
-000020f0: 6720 6461 7461 2061 6e64 2074 6865 2074  g data and the t
-00002100: 6172 6765 7473 2e0a 2020 2020 2020 2020  argets..        
-00002110: 3a70 6172 616d 203a 6466 5f65 7661 6c3a  :param :df_eval:
-00002120: 2054 616b 6573 2061 2070 616e 6461 7320   Takes a pandas 
-00002130: 4461 7461 4672 616d 6520 636f 6e74 6169  DataFrame contai
-00002140: 6e69 6e67 2074 6865 2065 7661 6c75 6174  ning the evaluat
-00002150: 696f 6e20 6461 7461 2c20 6275 7420 6e6f  ion data, but no
-00002160: 7420 7468 6520 7461 7267 6574 732e 0a20  t the targets.. 
-00002170: 2020 2020 2020 203a 7061 7261 6d20 3a74         :param :t
-00002180: 6172 6765 745f 6576 616c 3a20 5461 6b65  arget_eval: Take
-00002190: 7320 6120 7061 6e64 6173 2053 6572 6965  s a pandas Serie
-000021a0: 7320 636f 6e74 6169 6e69 6e67 2074 6865  s containing the
-000021b0: 2065 7661 6c75 6174 696f 6e20 7461 7267   evaluation targ
-000021c0: 6574 732e 0a20 2020 2020 2020 203a 7061  ets..        :pa
-000021d0: 7261 6d20 3a74 6172 6765 745f 636f 6c3a  ram :target_col:
-000021e0: 2054 616b 6573 2061 2073 7472 696e 6720   Takes a string 
-000021f0: 636f 6e74 6169 6e69 6e67 2074 6865 206e  containing the n
-00002200: 616d 6520 6f66 2074 6865 2074 6172 6765  ame of the targe
-00002210: 7420 636f 6c75 6d6e 2069 6e73 6964 6520  t column inside 
-00002220: 7468 6520 7472 6169 6e69 6e67 2064 6174  the training dat
-00002230: 6120 6466 2e0a 2020 2020 2020 2020 2904  a df..        ).
-00002240: 7250 0000 00da 0770 7265 6469 6374 720d  rP.....predictr.
-00002250: 0000 00da 0676 616c 7565 7329 0872 3100  .....values).r1.
-00002260: 0000 7235 0000 0072 5900 0000 725a 0000  ..r5...rY...rZ..
-00002270: 0072 4400 0000 da07 795f 7072 6f62 73da  .rD.....y_probs.
-00002280: 0979 5f63 6c61 7373 6573 5a09 6576 616c  .y_classesZ.eval
-00002290: 5f64 6963 7472 3200 0000 7232 0000 0072  _dictr2...r2...r
-000022a0: 3300 0000 da08 6669 745f 6576 616c f400  3.....fit_eval..
-000022b0: 0000 7308 0000 000c 100e 010e 0104 017a  ..s............z
-000022c0: 1142 6c75 6543 6173 742e 6669 745f 6576  .BlueCast.fit_ev
-000022d0: 616c 6302 0000 0000 0000 0000 0000 0003  alc.............
-000022e0: 0000 0004 0000 0043 0000 0073 2001 0000  .......C...s ...
-000022f0: 7400 8300 0100 7c00 6a01 730a 7402 6401  t.....|.j.s.t.d.
-00002300: 8301 8201 7c00 6a03 7311 7402 6402 8301  ....|.j.s.t.d...
-00002310: 8201 7c00 6a01 6a04 7c01 7c00 6a05 6701  ..|.j.j.|.|.j.g.
-00002320: 6403 8d02 7d01 7c00 6a06 722e 7c00 6a06  d...}.|.j.r.|.j.
-00002330: 6a07 7c01 6404 6405 8d02 5c02 7d01 7d02  j.|.d.d...\.}.}.
-00002340: 7c01 6a08 6404 6406 8d01 7d01 7409 7c01  |.j.d.d...}.t.|.
-00002350: 8301 7d01 740a 7c01 7c00 6a0b 8302 7d01  ..}.t.|.|.j...}.
-00002360: 7c00 6a0c 7241 7c00 6a0c a007 7c01 a101  |.j.rA|.j...|...
-00002370: 7d01 7c00 6a0d 7259 7c00 6a0e 7259 7c00  }.|.j.rY|.j.rY|.
-00002380: 6a0f 6407 6b02 7259 7410 7c00 6a0e 7411  j.d.k.rYt.|.j.t.
-00002390: 8302 7259 7c00 6a0e a012 7c01 a101 7d01  ..rY|.j...|...}.
-000023a0: 6e17 7c00 6a0d 7270 7c00 6a0e 7270 7c00  n.|.j.rp|.j.rp|.
-000023b0: 6a0f 6408 6b02 7270 7410 7c00 6a0e 7413  j.d.k.rpt.|.j.t.
-000023c0: 8302 7270 7c00 6a0e a014 7c01 a101 7d01  ..rp|.j...|...}.
-000023d0: 7c00 6a15 727d 7c00 6a15 6a07 7c01 6404  |.j.r}|.j.j.|.d.
-000023e0: 6405 8d02 5c02 7d01 7d02 7c00 6a16 728e  d...\.}.}.|.j.r.
-000023f0: 7c00 6a03 6a17 728e 7c00 6a16 6a07 7c01  |.j.j.r.|.j.j.|.
-00002400: 6404 6405 8d02 5c02 7d01 7d02 7c01 5300  d.d...\.}.}.|.S.
-00002410: 2909 7a37 5472 616e 7366 6f72 6d20 6e65  ).z7Transform ne
-00002420: 7720 6461 7461 2061 6363 6f72 6469 6e67  w data according
-00002430: 2074 6f20 7072 6570 726f 6365 7373 696e   to preprocessin
-00002440: 6720 7069 7065 6c69 6e65 2efa 2a46 6561  g pipeline..*Fea
-00002450: 7475 7265 2074 7970 6520 636f 6e76 6572  ture type conver
-00002460: 7465 7220 636f 756c 6420 6e6f 7420 6265  ter could not be
-00002470: 2066 6f75 6e64 2e7a 2a54 7261 696e 696e   found.z*Trainin
-00002480: 6720 636f 6e66 6967 7572 6174 696f 6e20  g configuration 
-00002490: 636f 756c 6420 6e6f 7420 6265 2066 6f75  could not be fou
-000024a0: 6e64 2e29 015a 0b69 676e 6f72 655f 636f  nd.).Z.ignore_co
-000024b0: 6c73 5472 4500 0000 7247 0000 0072 1e00  lsTrE...rG...r..
-000024c0: 0000 721f 0000 0029 1872 0f00 0000 722c  ..r....).r....r,
-000024d0: 0000 00da 0945 7863 6570 7469 6f6e 7228  .....Exceptionr(
-000024e0: 0000 005a 1774 7261 6e73 666f 726d 5f66  ...Z.transform_f
-000024f0: 6561 7475 7265 5f74 7970 6573 7220 0000  eature_typesr ..
-00002500: 0072 2600 0000 724d 0000 0072 4e00 0000  .r&...rM...rN...
-00002510: 7217 0000 0072 1300 0000 7222 0000 0072  r....r....r"...r
-00002520: 2f00 0000 7221 0000 0072 2d00 0000 721d  /...r!...r-...r.
-00002530: 0000 00da 0a69 7369 6e73 7461 6e63 6572  .....isinstancer
-00002540: 1900 0000 7251 0000 0072 1a00 0000 7252  ....rQ...r....rR
-00002550: 0000 0072 2500 0000 7227 0000 0072 3a00  ...r%...r'...r:.
-00002560: 0000 2903 7231 0000 0072 3500 0000 7258  ..).r1...r5...rX
-00002570: 0000 0072 3200 0000 7232 0000 0072 3300  ...r2...r2...r3.
-00002580: 0000 da12 7472 616e 7366 6f72 6d5f 6e65  ....transform_ne
-00002590: 775f 6461 7461 0901 0000 7348 0000 0006  w_data....sH....
-000025a0: 0206 0108 0106 0208 0106 0208 0106 ff06  ................
-000025b0: 0414 010c 0108 020c 0106 020c 0104 0302  ................
-000025c0: ff04 0202 fe0a 030a 0102 ff0e 0304 0202  ................
-000025d0: ff04 0202 fe0a 030a 0102 ff0c 0306 0214  ................
-000025e0: 010e 0214 0104 027a 1b42 6c75 6543 6173  .......z.BlueCas
-000025f0: 742e 7472 616e 7366 6f72 6d5f 6e65 775f  t.transform_new_
-00002600: 6461 7461 6302 0000 0000 0000 0000 0000  datac...........
-00002610: 0004 0000 0005 0000 0043 0000 0073 8a00  .........C...s..
-00002620: 0000 7c00 6a00 7307 7401 6401 8301 8201  ..|.j.s.t.d.....
-00002630: 7c00 6a02 730e 7401 6402 8301 8201 7403  |.j.s.t.d.....t.
-00002640: 8300 0100 7c00 a004 7c01 a101 7d01 7405  ....|...|...}.t.
-00002650: 7406 a007 a100 9b00 6403 9d02 8301 0100  t.......d.......
-00002660: 7c00 6a00 a008 7c01 a101 5c02 7d02 7d03  |.j...|...\.}.}.
-00002670: 7c00 6a02 6a09 7241 7c00 6a0a 7c00 6a02  |.j.j.rA|.j.|.j.
-00002680: 6a09 7600 7241 7c00 6a0b 7241 7c00 6a02  j.v.rA|.j.rA|.j.
-00002690: 7241 7c00 6a0b a00c 740d a00e 7c03 a101  rA|.j...t...|...
-000026a0: a101 7d03 7c02 7c03 6602 5300 2904 7a90  ..}.|.|.f.S.).z.
-000026b0: 5072 6564 6963 7420 6f6e 2075 6e73 6565  Predict on unsee
-000026c0: 6e20 6461 7461 2e0a 0a20 2020 2020 2020  n data...       
-000026d0: 2052 6574 7572 6e20 7468 6520 7072 6564   Return the pred
-000026e0: 6963 7465 6420 7072 6f62 6162 696c 6974  icted probabilit
-000026f0: 6965 7320 616e 6420 7468 6520 7072 6564  ies and the pred
-00002700: 6963 7465 6420 636c 6173 7365 733a 0a20  icted classes:. 
-00002710: 2020 2020 2020 2079 5f70 726f 6273 2c20         y_probs, 
-00002720: 795f 636c 6173 7365 7320 3d20 7072 6564  y_classes = pred
-00002730: 6963 7428 6466 290a 2020 2020 2020 2020  ict(df).        
-00002740: 7a1b 4d6c 206d 6f64 656c 2063 6f75 6c64  z.Ml model could
-00002750: 206e 6f74 2062 6520 666f 756e 6472 6000   not be foundr`.
-00002760: 0000 7a0f 3a20 5072 6564 6963 7469 6e67  ..z.: Predicting
-00002770: 2e2e 2e29 0f72 2400 0000 7261 0000 0072  ...).r$...ra...r
-00002780: 2c00 0000 720f 0000 0072 6300 0000 7210  ,...r....rc...r.
-00002790: 0000 0072 0200 0000 da06 7574 636e 6f77  ...r......utcnow
-000027a0: 725b 0000 0072 2100 0000 7220 0000 0072  r[...r!...r ...r
-000027b0: 2e00 0000 5a1f 6c61 6265 6c5f 656e 636f  ....Z.label_enco
-000027c0: 6465 725f 7265 7665 7273 655f 7472 616e  der_reverse_tran
-000027d0: 7366 6f72 6dda 0270 64da 0653 6572 6965  sform..pd..Serie
-000027e0: 7329 0472 3100 0000 7235 0000 0072 5d00  s).r1...r5...r].
-000027f0: 0000 725e 0000 0072 3200 0000 7232 0000  ..r^...r2...r2..
-00002800: 0072 3300 0000 725b 0000 0037 0100 0073  .r3...r[...7...s
-00002810: 2400 0000 0606 0801 0602 0801 0602 0a01  $...............
-00002820: 1202 1001 0802 0e02 0401 02ff 0402 02fe  ................
-00002830: 0604 0801 04ff 0804 7a10 426c 7565 4361  ........z.BlueCa
-00002840: 7374 2e70 7265 6469 6374 290a 4e4e 4e4e  st.predict).NNNN
-00002850: 4e4e 4e4e 4e4e 291f da08 5f5f 6e61 6d65  NNNNNN)...__name
-00002860: 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f da0c  __..__module__..
-00002870: 5f5f 7175 616c 6e61 6d65 5f5f da07 5f5f  __qualname__..__
-00002880: 646f 635f 5f72 0600 0000 7209 0000 00da  doc__r....r.....
-00002890: 0373 7472 da05 666c 6f61 74da 0369 6e74  .str..float..int
-000028a0: 7207 0000 0072 0500 0000 7211 0000 0072  r....r....r....r
-000028b0: 0300 0000 7212 0000 0072 1500 0000 720a  ....r....r....r.
-000028c0: 0000 0072 0c00 0000 720b 0000 0072 3400  ...r....r....r4.
-000028d0: 0000 7265 0000 00da 0944 6174 6146 7261  ..re.....DataFra
-000028e0: 6d65 7243 0000 0072 5000 0000 7266 0000  merC...rP...rf..
-000028f0: 0072 0400 0000 725f 0000 0072 6300 0000  .r....r_...rc...
-00002900: 7208 0000 00da 026e 70da 076e 6461 7272  r......np..ndarr
-00002910: 6179 725b 0000 0072 3200 0000 7232 0000  ayr[...r2...r2..
-00002920: 0072 3200 0000 7233 0000 0072 1c00 0000  .r2...r3...r....
-00002930: 2700 0000 736c 0000 0008 0004 0102 1802  '...sl..........
-00002940: 0102 0102 0102 0102 0102 0302 0102 0102  ................
-00002950: 0104 f106 0202 fe0c 0302 fd14 0402 fc14  ................
-00002960: 0502 fb06 0602 fa0e 0702 f906 0802 f806  ................
-00002970: 0902 f702 0a0a 0102 ff02 f606 0d02 f306  ................
-00002980: 0e02 f206 0f0a f114 2618 2d02 6504 0202  ........&.-.e...
-00002990: fe04 0302 fd04 0402 fc02 0502 fb0a 060a  ................
-000029a0: fa16 1524 2e72 1c00 0000 2930 726a 0000  ...$.r....)0rj..
-000029b0: 0072 3b00 0000 7202 0000 00da 0674 7970  .r;...r......typ
-000029c0: 696e 6772 0300 0000 7204 0000 0072 0500  ingr....r....r..
-000029d0: 0000 7206 0000 0072 0700 0000 7208 0000  ..r....r....r...
-000029e0: 0072 0900 0000 da05 6e75 6d70 7972 6f00  .r......numpyro.
-000029f0: 0000 da06 7061 6e64 6173 7265 0000 00da  ....pandasre....
-00002a00: 1f62 6c75 6563 6173 742e 636f 6e66 6967  .bluecast.config
-00002a10: 2e74 7261 696e 696e 675f 636f 6e66 6967  .training_config
-00002a20: 720a 0000 0072 0b00 0000 720c 0000 005a  r....r....r....Z
-00002a30: 2062 6c75 6563 6173 742e 6576 616c 7561   bluecast.evalua
-00002a40: 7469 6f6e 2e65 7661 6c5f 6d65 7472 6963  tion.eval_metric
-00002a50: 7372 0d00 0000 5a1f 626c 7565 6361 7374  sr....Z.bluecast
-00002a60: 2e65 7661 6c75 6174 696f 6e2e 7368 6170  .evaluation.shap
-00002a70: 5f76 616c 7565 7372 0e00 0000 5a24 626c  _valuesr....Z$bl
-00002a80: 7565 6361 7374 2e67 656e 6572 616c 5f75  uecast.general_u
-00002a90: 7469 6c73 2e67 656e 6572 616c 5f75 7469  tils.general_uti
-00002aa0: 6c73 720f 0000 0072 1000 0000 5a1d 626c  lsr....r....Z.bl
-00002ab0: 7565 6361 7374 2e6d 6c5f 6d6f 6465 6c6c  uecast.ml_modell
-00002ac0: 696e 672e 7867 626f 6f73 7472 1100 0000  ing.xgboostr....
-00002ad0: da1d 626c 7565 6361 7374 2e70 7265 7072  ..bluecast.prepr
-00002ae0: 6f63 6573 7369 6e67 2e63 7573 746f 6d72  ocessing.customr
-00002af0: 1200 0000 5a28 626c 7565 6361 7374 2e70  ....Z(bluecast.p
-00002b00: 7265 7072 6f63 6573 7369 6e67 2e64 6174  reprocessing.dat
-00002b10: 6574 696d 655f 6665 6174 7572 6573 7213  etime_featuresr.
-00002b20: 0000 005a 2b62 6c75 6563 6173 742e 7072  ...Z+bluecast.pr
-00002b30: 6570 726f 6365 7373 696e 672e 656e 636f  eprocessing.enco
-00002b40: 6465 5f74 6172 6765 745f 6c61 6265 6c73  de_target_labels
-00002b50: 7214 0000 005a 2862 6c75 6563 6173 742e  r....Z(bluecast.
-00002b60: 7072 6570 726f 6365 7373 696e 672e 6665  preprocessing.fe
-00002b70: 6174 7572 655f 7365 6c65 6374 696f 6e72  ature_selectionr
-00002b80: 1500 0000 5a24 626c 7565 6361 7374 2e70  ....Z$bluecast.p
-00002b90: 7265 7072 6f63 6573 7369 6e67 2e66 6561  reprocessing.fea
-00002ba0: 7475 7265 5f74 7970 6573 7216 0000 005a  ture_typesr....Z
-00002bb0: 2562 6c75 6563 6173 742e 7072 6570 726f  %bluecast.prepro
-00002bc0: 6365 7373 696e 672e 6e75 6c6c 735f 616e  cessing.nulls_an
-00002bd0: 645f 696e 6673 7217 0000 005a 2462 6c75  d_infsr....Z$blu
-00002be0: 6563 6173 742e 7072 6570 726f 6365 7373  ecast.preprocess
-00002bf0: 696e 672e 7363 6865 6d61 5f63 6865 636b  ing.schema_check
-00002c00: 7372 1800 0000 5a26 626c 7565 6361 7374  sr....Z&bluecast
-00002c10: 2e70 7265 7072 6f63 6573 7369 6e67 2e74  .preprocessing.t
-00002c20: 6172 6765 745f 656e 636f 6469 6e67 7219  arget_encodingr.
-00002c30: 0000 0072 1a00 0000 5a27 626c 7565 6361  ...r....Z'blueca
-00002c40: 7374 2e70 7265 7072 6f63 6573 7369 6e67  st.preprocessing
-00002c50: 2e74 7261 696e 5f74 6573 745f 7370 6c69  .train_test_spli
-00002c60: 7472 1b00 0000 721c 0000 0072 3200 0000  tr....r....r2...
-00002c70: 7232 0000 0072 3200 0000 7233 0000 00da  r2...r2...r3....
-00002c80: 083c 6d6f 6475 6c65 3e01 0000 0073 2a00  .<module>....s*.
-00002c90: 0000 0400 0808 0c01 2401 0802 0801 1402  ........$.......
-00002ca0: 0c05 0c01 1001 0c01 0c01 0c01 0c01 0c01  ................
-00002cb0: 0c01 0c01 0c01 1001 0c04 1203            ............
+00001070: 8d03 0100 7c00 6a00 6a0c 7270 7c00 6a00  ....|.j.j.rp|.j.
+00001080: 6a0d 7270 6409 7c00 6a00 5f0d 640a 7d02  j.rpd.|.j._.d.}.
+00001090: 7403 6a04 7c02 7405 6402 6403 8d03 0100  t.j.|.t.d.d.....
+000010a0: 7c00 6a00 6a0c 7281 7c00 6a0e 7281 640b  |.j.j.r.|.j.r.d.
+000010b0: 7d02 7403 6a04 7c02 7405 6402 6403 8d03  }.t.j.|.t.d.d...
+000010c0: 0100 7c00 6a00 6a0c 7294 7c00 6a0f 7296  ..|.j.j.r.|.j.r.
+000010d0: 640c 7d02 7403 6a04 7c02 7405 6402 6403  d.}.t.j.|.t.d.d.
+000010e0: 8d03 0100 6400 5300 6400 5300 6400 5300  ....d.S.d.S.d.S.
+000010f0: 290d 4e61 9301 0000 4665 6174 7572 6520  ).Na....Feature 
+00001100: 7365 6c65 6374 696f 6e20 6973 2064 6973  selection is dis
+00001110: 6162 6c65 642e 2055 7064 6174 6520 7468  abled. Update th
+00001120: 6520 5472 6169 6e69 6e67 436f 6e66 6967  e TrainingConfig
+00001130: 2070 6172 616d 2027 656e 6162 6c65 5f66   param 'enable_f
+00001140: 6561 7475 7265 5f73 656c 6563 7469 6f6e  eature_selection
+00001150: 270a 2020 2020 2020 2020 2020 2020 746f  '.            to
+00001160: 2065 6e61 626c 6520 6974 206f 7220 6d61   enable it or ma
+00001170: 6b65 2075 7365 206f 6620 6120 6375 7374  ke use of a cust
+00001180: 6f6d 2070 7265 7072 6f63 6573 736f 7220  om preprocessor 
+00001190: 746f 2064 6f20 6974 206d 616e 7561 6c6c  to do it manuall
+000011a0: 7920 6475 7269 6e67 2074 6865 206c 6173  y during the las
+000011b0: 7420 6d69 6c65 2063 6f6d 7075 7461 7469  t mile computati
+000011c0: 6f6e 7320 7374 6570 2e0a 2020 2020 2020  ons step..      
+000011d0: 2020 2020 2020 4665 6174 7572 6520 7365        Feature se
+000011e0: 6c65 6374 696f 6e20 6973 2072 6563 6f6d  lection is recom
+000011f0: 6d65 6e64 6564 2066 6f72 2064 6174 6173  mended for datas
+00001200: 6574 7320 7769 7468 206d 616e 7920 6665  ets with many fe
+00001210: 6174 7572 6573 2028 3e31 3030 3029 2e20  atures (>1000). 
+00001220: 466f 7220 6461 7461 7365 7473 2077 6974  For datasets wit
+00001230: 6820 6120 736d 616c 6c20 616d 6f75 6e74  h a small amount
+00001240: 0a20 2020 2020 2020 2020 2020 206f 6620  .            of 
+00001250: 6665 6174 7572 6573 2066 6561 7475 7265  features feature
+00001260: 2073 656c 6563 7469 6f6e 2069 7320 6e6f   selection is no
+00001270: 7420 7265 636f 6d6d 656e 6465 642e 0a20  t recommended.. 
+00001280: 2020 2020 2020 2020 2020 20e9 0200 0000             .....
+00001290: 2901 da0a 7374 6163 6b6c 6576 656c e901  )...stacklevel..
+000012a0: 0000 0061 0501 0000 4372 6f73 7320 7661  ...a....Cross va
+000012b0: 6c69 6461 7469 6f6e 2069 7320 6469 7361  lidation is disa
+000012c0: 626c 6564 2e20 5570 6461 7465 2074 6865  bled. Update the
+000012d0: 2054 7261 696e 696e 6743 6f6e 6669 6720   TrainingConfig 
+000012e0: 7061 7261 6d20 2768 7970 6572 7475 6e69  param 'hypertuni
+000012f0: 6e67 5f63 765f 666f 6c64 7327 0a20 2020  ng_cv_folds'.   
+00001300: 2020 2020 2020 2020 2074 6f20 656e 6162           to enab
+00001310: 6c65 2069 742e 2043 726f 7373 2076 616c  le it. Cross val
+00001320: 6964 6174 696f 6e20 6973 2064 6973 6162  idation is disab
+00001330: 6c65 6420 6f6e 2064 6566 6175 6c74 2074  led on default t
+00001340: 6f20 616c 6c6f 7720 6661 7374 2070 726f  o allow fast pro
+00001350: 746f 7479 7069 6e67 2e20 466f 7220 726f  totyping. For ro
+00001360: 6275 7374 2068 7970 6572 7061 7261 6d65  bust hyperparame
+00001370: 7465 720a 2020 2020 2020 2020 2020 2020  ter.            
+00001380: 7475 6e69 6e67 2075 7369 6e67 2061 7420  tuning using at 
+00001390: 6c65 6173 7420 3520 666f 6c64 7320 6973  least 5 folds is
+000013a0: 2072 6563 6f6d 6d65 6e64 6564 2e61 5f01   recommended.a_.
+000013b0: 0000 4665 6174 7572 6520 7365 6c65 6374  ..Feature select
+000013c0: 696f 6e20 6973 2065 6e61 626c 6564 2062  ion is enabled b
+000013d0: 7574 206e 6f20 6665 6174 7572 6520 7365  ut no feature se
+000013e0: 6c65 6374 6f72 2068 6173 2062 6565 6e20  lector has been 
+000013f0: 7072 6f76 6964 6564 2e20 4661 6c6c 696e  provided. Fallin
+00001400: 6720 6261 636b 2074 6f0a 2020 2020 2020  g back to.      
+00001410: 2020 2020 2020 6372 6f73 732d 7661 6c69        cross-vali
+00001420: 6461 7465 6420 6665 6174 7572 6520 656c  dated feature el
+00001430: 696d 696e 6174 696f 6e2e 2053 7065 6369  imination. Speci
+00001440: 6669 6361 6c6c 7920 666f 7220 736d 616c  fically for smal
+00001450: 6c20 6461 7461 7365 7473 2063 6865 636b  l datasets check
+00001460: 2074 6865 206c 6f67 7320 746f 2076 6572   the logs to ver
+00001470: 6966 7920 7468 6174 206e 6f74 2074 6f6f  ify that not too
+00001480: 0a20 2020 2020 2020 2020 2020 206d 616e  .            man
+00001490: 7920 6665 6174 7572 6573 2068 6176 6520  y features have 
+000014a0: 6265 656e 2072 656d 6f76 6564 2e20 4f74  been removed. Ot
+000014b0: 6865 7277 6973 652c 2063 6f6e 7369 6465  herwise, conside
+000014c0: 7220 6469 7361 626c 696e 6720 6665 6174  r disabling feat
+000014d0: 7572 6520 7365 6c65 6374 696f 6e20 6f72  ure selection or
+000014e0: 2070 726f 7669 6469 6e67 2061 2063 7573   providing a cus
+000014f0: 746f 6d0a 2020 2020 2020 2020 2020 2020  tom.            
+00001500: 6665 6174 7572 6520 7365 6c65 6374 6f72  feature selector
+00001510: 2e61 6501 0000 4e6f 2058 6762 6f6f 7374  .ae...No Xgboost
+00001520: 5475 6e65 5061 7261 6d73 436f 6e66 6967  TuneParamsConfig
+00001530: 2068 6173 2062 6565 6e20 7072 6f76 6964   has been provid
+00001540: 6564 2e20 4661 6c6c 696e 6720 6261 636b  ed. Falling back
+00001550: 2074 6f20 6465 6661 756c 7420 7661 6c75   to default valu
+00001560: 6573 2e20 4465 6661 756c 7420 7661 6c75  es. Default valu
+00001570: 6573 0a20 2020 2020 2020 2020 2020 2068  es.            h
+00001580: 6176 6520 6265 656e 2063 686f 7365 6e20  ave been chosen 
+00001590: 746f 2073 7065 6564 2075 7020 7468 6520  to speed up the 
+000015a0: 7072 6f74 6f74 7970 696e 672e 2046 6f72  prototyping. For
+000015b0: 2072 6f62 7573 7420 6879 7065 7270 6172   robust hyperpar
+000015c0: 616d 6574 6572 2074 756e 696e 6720 636f  ameter tuning co
+000015d0: 6e73 6964 6572 2070 726f 7669 6469 6e67  nsider providing
+000015e0: 2061 2063 7573 746f 6d0a 2020 2020 2020   a custom.      
+000015f0: 2020 2020 2020 5867 626f 6f73 7454 756e        XgboostTun
+00001600: 6550 6172 616d 7343 6f6e 6669 6720 7769  eParamsConfig wi
+00001610: 7468 2061 2064 6565 7065 7220 6879 7065  th a deeper hype
+00001620: 7270 6172 616d 6574 6572 2073 6561 7263  rparameter searc
+00001630: 6820 7370 6163 6520 616e 6420 6120 6375  h space and a cu
+00001640: 7374 6f6d 2054 7261 696e 696e 6743 6f6e  stom TrainingCon
+00001650: 6669 6720 746f 2065 6e61 626c 650a 2020  fig to enable.  
+00001660: 2020 2020 2020 2020 2020 6372 6f73 732d            cross-
+00001670: 7661 6c69 6461 7469 6f6e 2e61 0f01 0000  validation.a....
+00001680: 5468 6520 6d69 6e69 6d75 6d20 6e75 6d62  The minimum numb
+00001690: 6572 206f 6620 6665 6174 7572 6573 2074  er of features t
+000016a0: 6f20 7365 6c65 6374 2069 7320 6772 6561  o select is grea
+000016b0: 7465 7220 6f72 2065 7175 616c 2074 6f20  ter or equal to 
+000016c0: 7468 6520 6e75 6d62 6572 206f 6620 6665  the number of fe
+000016d0: 6174 7572 6573 2069 6e0a 2020 2020 2020  atures in.      
+000016e0: 2020 2020 2020 7468 6520 6461 7461 7365        the datase
+000016f0: 7420 7768 696c 6520 6665 6174 7572 6520  t while feature 
+00001700: 7365 6c65 6374 696f 6e20 6973 2065 6e61  selection is ena
+00001710: 626c 6564 2e20 436f 6e73 6964 6572 2072  bled. Consider r
+00001720: 6564 7563 696e 6720 7468 6520 6d69 6e69  educing the mini
+00001730: 6d75 6d20 6e75 6d62 6572 206f 6620 6665  mum number of fe
+00001740: 6174 7572 6573 2074 6f0a 2020 2020 2020  atures to.      
+00001750: 2020 2020 2020 7365 6c65 6374 206f 7220        select or 
+00001760: 6469 7361 626c 696e 6720 6665 6174 7572  disabling featur
+00001770: 6520 7365 6c65 6374 696f 6e20 7669 6120  e selection via 
+00001780: 5472 6169 6e69 6e67 436f 6e66 6967 2e46  TrainingConfig.F
+00001790: 612b 0200 0053 4841 5020 7661 6c75 6573  a+...SHAP values
+000017a0: 2063 616e 6e6f 7420 6265 2063 616c 6375   cannot be calcu
+000017b0: 6c61 7465 6420 7768 656e 2063 6174 6567  lated when categ
+000017c0: 6f72 6963 616c 2065 6e63 6f64 696e 6720  orical encoding 
+000017d0: 7669 6120 4d4c 2061 6c67 6f72 6974 686d  via ML algorithm
+000017e0: 2069 7320 656e 6162 6c65 6420 6475 6520   is enabled due 
+000017f0: 746f 0a20 2020 2020 2020 2020 2020 2069  to.            i
+00001800: 6e63 6f6d 7061 7469 6269 6c69 7479 2077  ncompatibility w
+00001810: 6974 6820 7468 6520 7368 6170 206c 6962  ith the shap lib
+00001820: 7261 7279 2e20 5365 6520 7468 6973 2047  rary. See this G
+00001830: 6974 4875 6220 6973 7375 6520 666f 7220  itHub issue for 
+00001840: 6d6f 7265 2063 6f6e 7465 7874 3a0a 2020  more context:.  
+00001850: 2020 2020 2020 2020 2020 6874 7470 733a            https:
+00001860: 2f2f 6769 7468 7562 2e63 6f6d 2f73 6c75  //github.com/slu
+00001870: 6e64 6265 7267 2f73 6861 702f 6973 7375  ndberg/shap/issu
+00001880: 6573 2f32 3636 0a0a 2020 2020 2020 2020  es/266..        
+00001890: 2020 2020 4361 6c63 756c 6174 696f 6e20      Calculation 
+000018a0: 6f66 2053 6861 7020 7661 6c75 6573 2068  of Shap values h
+000018b0: 6173 2062 6565 6e20 6368 616e 6765 6420  as been changed 
+000018c0: 746f 2066 616c 7365 2e0a 2020 2020 2020  to false..      
+000018d0: 2020 2020 2020 436f 6e73 6964 6572 2064        Consider d
+000018e0: 6973 6162 6c69 6e67 2063 6174 6567 6f72  isabling categor
+000018f0: 6963 616c 2065 6e63 6f64 696e 6720 7669  ical encoding vi
+00001900: 6120 4d4c 2061 6c67 6f72 6974 686d 2069  a ML algorithm i
+00001910: 6e20 7468 6520 5472 6169 6e69 6e67 436f  n the TrainingCo
+00001920: 6e66 6967 2069 6620 7368 6170 2076 616c  nfig if shap val
+00001930: 7565 7320 6172 650a 2020 2020 2020 2020  ues are.        
+00001940: 2020 2020 7265 7175 6972 6564 2e20 416c      required. Al
+00001950: 7465 726e 6174 6976 656c 7920 7573 6520  ternatively use 
+00001960: 5867 626f 6f73 7420 6173 2061 2063 7573  Xgboost as a cus
+00001970: 746f 6d20 6d6f 6465 6c20 616e 6420 6361  tom model and ca
+00001980: 6c63 756c 6174 6520 7368 6170 2076 616c  lculate shap val
+00001990: 7565 7320 6d61 6e75 616c 6c79 2076 6961  ues manually via
+000019a0: 0a20 2020 2020 2020 2020 2020 2070 7265  .            pre
+000019b0: 645f 636f 6e74 7269 6273 3d54 7275 652e  d_contribs=True.
+000019c0: 7af0 4361 7465 676f 7269 6361 6c20 656e  z.Categorical en
+000019d0: 636f 6469 6e67 2076 6961 204d 4c20 616c  coding via ML al
+000019e0: 676f 7269 7468 6d20 6973 2065 6e61 626c  gorithm is enabl
+000019f0: 6564 2e20 4d61 6b65 2073 7572 6520 746f  ed. Make sure to
+00001a00: 2068 616e 646c 6520 6361 7465 676f 7269   handle categori
+00001a10: 6361 6c20 6665 6174 7572 6573 0a20 2020  cal features.   
+00001a20: 2020 2020 2020 2020 2077 6974 6869 6e20           within 
+00001a30: 7468 6520 7072 6f76 6964 6564 206d 6c20  the provided ml 
+00001a40: 6d6f 6465 6c20 6f72 2063 6f6e 7369 6465  model or conside
+00001a50: 7220 6469 7361 626c 696e 6720 6361 7465  r disabling cate
+00001a60: 676f 7269 6361 6c20 656e 636f 6469 6e67  gorical encoding
+00001a70: 2076 6961 204d 4c20 616c 676f 7269 7468   via ML algorith
+00001a80: 6d20 696e 2074 6865 0a20 2020 2020 2020  m in the.       
+00001a90: 2020 2020 2054 7261 696e 696e 6743 6f6e       TrainingCon
+00001aa0: 6669 6720 616c 7465 726e 6174 6976 656c  fig alternativel
+00001ab0: 792e 7afd 4361 7465 676f 7269 6361 6c20  y.z.Categorical 
+00001ac0: 656e 636f 6469 6e67 2076 6961 204d 4c20  encoding via ML 
+00001ad0: 616c 676f 7269 7468 6d20 6973 2065 6e61  algorithm is ena
+00001ae0: 626c 6564 2e20 4d61 6b65 2073 7572 6520  bled. Make sure 
+00001af0: 746f 2068 616e 646c 6520 6361 7465 676f  to handle catego
+00001b00: 7269 6361 6c20 6665 6174 7572 6573 0a20  rical features. 
+00001b10: 2020 2020 2020 2020 2020 2077 6974 6869             withi
+00001b20: 6e20 7468 6520 7072 6f76 6964 6564 206c  n the provided l
+00001b30: 6173 7420 6d69 6c65 2063 6f6d 7075 7461  ast mile computa
+00001b40: 7469 6f6e 206f 7220 636f 6e73 6964 6572  tion or consider
+00001b50: 2064 6973 6162 6c69 6e67 2063 6174 6567   disabling categ
+00001b60: 6f72 6963 616c 2065 6e63 6f64 696e 6720  orical encoding 
+00001b70: 7669 6120 4d4c 2061 6c67 6f72 6974 686d  via ML algorithm
+00001b80: 2069 6e20 7468 650a 2020 2020 2020 2020   in the.        
+00001b90: 2020 2020 5472 6169 6e69 6e67 436f 6e66      TrainingConf
+00001ba0: 6967 2061 6c74 6572 6e61 7469 7665 6c79  ig alternatively
+00001bb0: 2e29 1072 2800 0000 720a 0000 00da 1865  .).r(...r......e
+00001bc0: 6e61 626c 655f 6665 6174 7572 655f 7365  nable_feature_se
+00001bd0: 6c65 6374 696f 6eda 0877 6172 6e69 6e67  lection..warning
+00001be0: 73da 0477 6172 6eda 0b55 7365 7257 6172  s..warn..UserWar
+00001bf0: 6e69 6e67 da14 6879 7065 7274 756e 696e  ning..hypertunin
+00001c00: 675f 6376 5f66 6f6c 6473 7227 0000 0072  g_cv_foldsr'...r
+00001c10: 2900 0000 da16 6d69 6e5f 6665 6174 7572  ).....min_featur
+00001c20: 6573 5f74 6f5f 7365 6c65 6374 da03 6c65  es_to_select..le
+00001c30: 6eda 0763 6f6c 756d 6e73 da1d 6361 745f  n..columns..cat_
+00001c40: 656e 636f 6469 6e67 5f76 6961 5f6d 6c5f  encoding_via_ml_
+00001c50: 616c 676f 7269 7468 6dda 1563 616c 6375  algorithm..calcu
+00001c60: 6c61 7465 5f73 6861 705f 7661 6c75 6573  late_shap_values
+00001c70: 7224 0000 0072 2500 0000 2903 7231 0000  r$...r%...).r1..
+00001c80: 0072 3500 0000 da07 6d65 7373 6167 6572  .r5.....messager
+00001c90: 3200 0000 7232 0000 0072 3300 0000 da0e  2...r2...r3.....
+00001ca0: 696e 6974 6961 6c5f 6368 6563 6b73 6200  initial_checksb.
+00001cb0: 0000 734e 0000 0006 0108 0108 0104 0110  ..sN............
+00001cc0: 050c 0204 0110 0306 0302 ff04 0202 fe04  ................
+00001cd0: 0410 0406 0104 0110 0412 0206 0102 ff04  ................
+00001ce0: 0310 0306 0202 ff06 0202 fe08 0404 0110  ................
+00001cf0: 080e 0104 0110 0306 0202 ff04 0202 fe04  ................
+00001d00: 0414 0308 f97a 1742 6c75 6543 6173 742e  .....z.BlueCast.
+00001d10: 696e 6974 6961 6c5f 6368 6563 6b73 da0a  initial_checks..
+00001d20: 7461 7267 6574 5f63 6f6c 6303 0000 0000  target_colc.....
+00001d30: 0000 0000 0000 0009 0000 0007 0000 0043  ...............C
+00001d40: 0000 0073 1e03 0000 7400 8300 0100 7401  ...s....t.....t.
+00001d50: 8300 7d03 7c03 a002 7c01 a101 7d01 7c03  ..}.|...|...}.|.
+00001d60: 7c00 5f03 7c00 6a03 6a04 7229 7c00 6a05  |._.|.j.j.r)|.j.
+00001d70: 7c00 6a03 6a04 7600 7229 7406 8300 7c00  |.j.j.v.r)t...|.
+00001d80: 5f07 7c00 6a07 a008 7c01 7c00 6a05 1900  _.|.j...|.|.j...
+00001d90: a101 7c01 7c00 6a05 3c00 7c00 6a03 6a04  ..|.|.j.<.|.j.j.
+00001da0: 7c00 5f04 7c00 6a03 6a09 7c00 5f09 7c00  |._.|.j.j.|._.|.
+00001db0: 6a0a 733a 740b 8300 7c00 5f0a 7c00 a00c  j.s:t...|._.|...
+00001dc0: 7c01 a101 0100 740d 7c01 7c02 7c00 6a0e  |.....t.|.|.|.j.
+00001dd0: 7c00 6a0a 6a0f 7c00 6a0a 6a10 7c00 6a0a  |.j.j.|.j.j.|.j.
+00001de0: 6a11 8306 5c04 7d04 7d05 7d06 7d07 7c00  j...\.}.}.}.}.|.
+00001df0: 6a12 7297 7c00 6a12 a013 7c04 7c06 a102  j.r.|.j...|.|...
+00001e00: 5c02 7d04 7d06 7c00 6a12 6a14 7c05 7c07  \.}.}.|.j.j.|.|.
+00001e10: 6401 6402 8d03 5c02 7d05 7d07 7401 8300  d.d...\.}.}.t...
+00001e20: 7d03 7c03 a002 7c04 a101 7d08 7c04 6a15  }.|...|...}.|.j.
+00001e30: 6403 6404 8d01 7c06 6a15 6403 6404 8d01  d.d...|.j.d.d...
+00001e40: 0202 7d04 7d06 7c05 6a15 6403 6404 8d01  ..}.}.|.j.d.d...
+00001e50: 7c07 6a15 6403 6404 8d01 0202 7d05 7d07  |.j.d.d.....}.}.
+00001e60: 7c02 7c03 6a04 7600 7297 7c03 6a04 a016  |.|.j.v.r.|.j...
+00001e70: 7c02 a101 0100 7417 7c04 8301 7417 7c05  |.....t.|...t.|.
+00001e80: 8301 0202 7d04 7d05 7418 7c04 7c00 6a09  ....}.}.t.|.|.j.
+00001e90: 8302 7418 7c05 7c00 6a09 8302 0202 7d04  ..t.|.|.j.....}.
+00001ea0: 7d05 7419 8300 7c00 5f1a 7c00 6a1a a01b  }.t...|._.|.j...
+00001eb0: 7c04 a101 0100 7c00 6a1a a014 7c05 a101  |.....|.j...|...
+00001ec0: 7d05 7c00 6a04 6405 7501 72df 7c00 6a1c  }.|.j.d.u.r.|.j.
+00001ed0: 6406 6b02 72df 7c00 6a0a 6a1d 73df 741e  d.k.r.|.j.j.s.t.
+00001ee0: 7c03 6a04 8301 7c00 5f1f 7c00 6a1f a020  |.j...|._.|.j.. 
+00001ef0: 7c04 7c06 a102 7d04 7c00 6a1f a021 7c05  |.|...}.|.j..!|.
+00001f00: a101 7d05 6e40 7c00 6a04 6405 7501 9001  ..}.n@|.j.d.u...
+00001f10: 7204 7c00 6a1c 6407 6b02 9001 7204 7c00  r.|.j.d.k...r.|.
+00001f20: 6a0a 6a1d 9001 7304 7422 7c03 6a04 8301  j.j...s.t"|.j...
+00001f30: 7c00 5f1f 7c00 6a1f a023 7c04 7c06 a102  |._.|.j..#|.|...
+00001f40: 7d04 7c00 6a1f a024 7c05 a101 7d05 6e1b  }.|.j..$|...}.n.
+00001f50: 7c00 6a0a 6a1d 9001 721f 7c04 7c00 6a04  |.j.j...r.|.|.j.
+00001f60: 1900 a025 6408 a101 7c04 7c00 6a04 3c00  ...%d...|.|.j.<.
+00001f70: 7c05 7c00 6a04 1900 a025 6408 a101 7c05  |.|.j....%d...|.
+00001f80: 7c00 6a04 3c00 7c00 6a26 9001 7237 7c00  |.j.<.|.j&..r7|.
+00001f90: 6a26 a013 7c04 7c06 a102 5c02 7d04 7d06  j&..|.|...\.}.}.
+00001fa0: 7c00 6a26 6a14 7c05 7c07 6401 6402 8d03  |.j&j.|.|.d.d...
+00001fb0: 5c02 7d05 7d07 7c00 6a27 9001 7346 7428  \.}.}.|.j'..sFt(
+00001fc0: 7c00 6a0a 6a10 7c00 6a0a 6a29 6409 8d02  |.j.j.|.j.j)d...
+00001fd0: 7c00 5f27 7c00 6a0a 6a2a 9001 725e 7c00  |._'|.j.j*..r^|.
+00001fe0: 6a27 a013 7c04 7c06 a102 5c02 7d04 7d06  j'..|.|...\.}.}.
+00001ff0: 7c00 6a27 6a14 7c05 6401 6402 8d02 5c02  |.j'j.|.d.d...\.
+00002000: 7d05 7d08 7c00 6a2b 9001 736f 742c 7c00  }.}.|.j+..sot,|.
+00002010: 6a1c 7c00 6a0a 7c00 6a2d 7c00 6a2e 640a  j.|.j.|.j-|.j.d.
+00002020: 8d04 7c00 5f2b 7c00 6a2b a01b 7c04 7c05  ..|._+|.j+..|.|.
+00002030: 7c06 7c07 a104 0100 7c00 6a0a 9001 728a  |.|.....|.j...r.
+00002040: 7c00 6a0a 6a2f 9001 728a 7430 7c00 6a2b  |.j.j/..r.t0|.j+
+00002050: 6a31 7c05 640b 8303 7c00 5f32 6403 7c00  j1|.d...|._2d.|.
+00002060: 5f33 6405 5300 290c 7a19 5472 6169 6e20  _3d.S.).z.Train 
+00002070: 6120 6675 6c6c 204d 4c20 7069 7065 6c69  a full ML pipeli
+00002080: 6e65 2e46 a901 da0e 7072 6564 6963 746f  ne.F....predicto
+00002090: 6e5f 6d6f 6465 54a9 01da 0464 726f 704e  n_modeT....dropN
+000020a0: 721e 0000 0072 1f00 0000 da08 6361 7465  r....r......cate
+000020b0: 676f 7279 2902 da0c 7261 6e64 6f6d 5f73  gory)...random_s
+000020c0: 7461 7465 723f 0000 0029 0372 2800 0000  tater?...).r(...
+000020d0: 7229 0000 0072 2a00 0000 da04 7472 6565  r)...r*.....tree
+000020e0: 2934 720f 0000 0072 1600 0000 5a1b 6669  )4r....r....Z.fi
+000020f0: 745f 7472 616e 7366 6f72 6d5f 6665 6174  t_transform_feat
+00002100: 7572 655f 7479 7065 7372 2c00 0000 7221  ure_typesr,...r!
+00002110: 0000 0072 2000 0000 7214 0000 0072 2e00  ...r ...r....r..
+00002120: 0000 5a1b 6669 745f 7472 616e 7366 6f72  ..Z.fit_transfor
+00002130: 6d5f 7461 7267 6574 5f6c 6162 656c 7372  m_target_labelsr
+00002140: 2200 0000 7228 0000 0072 0a00 0000 7245  "...r(...r....rE
+00002150: 0000 0072 1b00 0000 7223 0000 00da 0a74  ...r....r#.....t
+00002160: 7261 696e 5f73 697a 655a 1367 6c6f 6261  rain_sizeZ.globa
+00002170: 6c5f 7261 6e64 6f6d 5f73 7461 7465 5a14  l_random_stateZ.
+00002180: 7472 6169 6e5f 7370 6c69 745f 7374 7261  train_split_stra
+00002190: 7469 6679 7226 0000 00da 0d66 6974 5f74  tifyr&.....fit_t
+000021a0: 7261 6e73 666f 726d da09 7472 616e 7366  ransform..transf
+000021b0: 6f72 6dda 0b72 6573 6574 5f69 6e64 6578  orm..reset_index
+000021c0: da06 7265 6d6f 7665 7217 0000 0072 1300  ..remover....r..
+000021d0: 0000 7218 0000 0072 2f00 0000 da03 6669  ..r....r/.....fi
+000021e0: 7472 1d00 0000 7242 0000 0072 1900 0000  tr....rB...r....
+000021f0: 722d 0000 005a 1e66 6974 5f74 6172 6765  r-...Z.fit_targe
+00002200: 745f 656e 636f 6465 5f62 696e 6172 795f  t_encode_binary_
+00002210: 636c 6173 73da 2474 7261 6e73 666f 726d  class.$transform
+00002220: 5f74 6172 6765 745f 656e 636f 6465 5f62  _target_encode_b
+00002230: 696e 6172 795f 636c 6173 7372 1a00 0000  inary_classr....
+00002240: 5a1c 6669 745f 7461 7267 6574 5f65 6e63  Z.fit_target_enc
+00002250: 6f64 655f 6d75 6c74 6963 6c61 7373 da22  ode_multiclass."
+00002260: 7472 616e 7366 6f72 6d5f 7461 7267 6574  transform_target
+00002270: 5f65 6e63 6f64 655f 6d75 6c74 6963 6c61  _encode_multicla
+00002280: 7373 da06 6173 7479 7065 7225 0000 0072  ss..astyper%...r
+00002290: 2700 0000 7215 0000 0072 3f00 0000 723a  '...r....r?...r:
+000022a0: 0000 0072 2400 0000 7211 0000 0072 2900  ...r$...r....r).
+000022b0: 0000 722a 0000 0072 4300 0000 720e 0000  ..r*...rC...r...
+000022c0: 00da 056d 6f64 656c 7230 0000 0072 2b00  ...modelr0...r+.
+000022d0: 0000 2909 7231 0000 0072 3500 0000 7246  ..).r1...r5...rF
+000022e0: 0000 0072 2c00 0000 da07 785f 7472 6169  ...r,.....x_trai
+000022f0: 6eda 0678 5f74 6573 74da 0779 5f74 7261  n..x_test..y_tra
+00002300: 696e da06 795f 7465 7374 da01 5f72 3200  in..y_test.._r2.
+00002310: 0000 7232 0000 0072 3300 0000 7253 0000  ..r2...r3...rS..
+00002320: 00a6 0000 0073 be00 0000 0602 0601 0a01  .....s..........
+00002330: 0601 0802 0e01 0801 0603 0801 02ff 02fe  ................
+00002340: 0401 02ff 0a06 0a01 0602 0801 0a02 0202  ................
+00002350: 0201 0201 0401 0601 0601 0601 0cfa 0609  ................
+00002360: 1201 0601 0601 0aff 0603 0a01 0e01 0201  ................
+00002370: 0aff 0e03 0201 0aff 0a03 0c01 1202 0c01  ................
+00002380: 0601 08ff 0804 0c01 0c01 0a03 0a01 0601  ................
+00002390: 02ff 0c03 0e01 0e01 0c02 0c01 0601 04ff  ................
+000023a0: 0c03 0e01 0e01 0a01 1601 1601 0802 0601  ................
+000023b0: 0401 08ff 0603 0601 0aff 0804 0201 0601  ................
+000023c0: 0601 08fe 0a05 0601 0401 08ff 0603 0401  ................
+000023d0: 0aff 0804 0201 0401 0401 0401 0401 08fc  ................
+000023e0: 1206 1201 1201 0a01 7a0c 426c 7565 4361  ........z.BlueCa
+000023f0: 7374 2e66 6974 da07 6466 5f65 7661 6cda  st.fit..df_eval.
+00002400: 0b74 6172 6765 745f 6576 616c 6305 0000  .target_evalc...
+00002410: 0000 0000 0000 0000 0008 0000 0004 0000  ................
+00002420: 0043 0000 0073 2c00 0000 7c00 a000 7c01  .C...s,...|...|.
+00002430: 7c04 a102 0100 7c00 a001 7c02 a101 5c02  |.....|...|...\.
+00002440: 7d05 7d06 7402 7c03 6a03 7c05 7c06 8303  }.}.t.|.j.|.|...
+00002450: 7d07 7c07 5300 2901 618e 0200 0054 7261  }.|.S.).a....Tra
+00002460: 696e 2061 2066 756c 6c20 4d4c 2070 6970  in a full ML pip
+00002470: 656c 696e 6520 616e 6420 6576 616c 7561  eline and evalua
+00002480: 7465 206f 6e20 6120 686f 6c64 6f75 7420  te on a holdout 
+00002490: 7365 742e 0a0a 2020 2020 2020 2020 5468  set...        Th
+000024a0: 6973 2069 7320 6120 636f 6e76 656e 6965  is is a convenie
+000024b0: 6e63 6520 6675 6e63 7469 6f6e 2074 6f20  nce function to 
+000024c0: 7472 6169 6e20 616e 6420 6576 616c 7561  train and evalua
+000024d0: 7465 206f 6e20 6120 686f 6c64 6f75 7420  te on a holdout 
+000024e0: 7365 742e 2049 7420 6973 2072 6563 6f6d  set. It is recom
+000024f0: 6d65 6e64 6564 2074 6f20 7573 6520 7468  mended to use th
+00002500: 6973 2066 6f72 206d 6f64 656c 0a20 2020  is for model.   
+00002510: 2020 2020 2065 7870 6c6f 7261 7469 6f6e       exploration
+00002520: 2e20 4f6e 2070 726f 6475 6374 696f 6e20  . On production 
+00002530: 7468 6520 7369 6d70 6c65 2066 6974 2829  the simple fit()
+00002540: 2066 756e 6374 696f 6e20 7368 6f75 6c64   function should
+00002550: 2062 6520 7573 6564 2e0a 2020 2020 2020   be used..      
+00002560: 2020 3a70 6172 616d 203a 6466 3a20 5461    :param :df: Ta
+00002570: 6b65 7320 6120 7061 6e64 6173 2044 6174  kes a pandas Dat
+00002580: 6146 7261 6d65 2063 6f6e 7461 696e 696e  aFrame containin
+00002590: 6720 7468 6520 7472 6169 6e69 6e67 2064  g the training d
+000025a0: 6174 6120 616e 6420 7468 6520 7461 7267  ata and the targ
+000025b0: 6574 732e 0a20 2020 2020 2020 203a 7061  ets..        :pa
+000025c0: 7261 6d20 3a64 665f 6576 616c 3a20 5461  ram :df_eval: Ta
+000025d0: 6b65 7320 6120 7061 6e64 6173 2044 6174  kes a pandas Dat
+000025e0: 6146 7261 6d65 2063 6f6e 7461 696e 696e  aFrame containin
+000025f0: 6720 7468 6520 6576 616c 7561 7469 6f6e  g the evaluation
+00002600: 2064 6174 612c 2062 7574 206e 6f74 2074   data, but not t
+00002610: 6865 2074 6172 6765 7473 2e0a 2020 2020  he targets..    
+00002620: 2020 2020 3a70 6172 616d 203a 7461 7267      :param :targ
+00002630: 6574 5f65 7661 6c3a 2054 616b 6573 2061  et_eval: Takes a
+00002640: 2070 616e 6461 7320 5365 7269 6573 2063   pandas Series c
+00002650: 6f6e 7461 696e 696e 6720 7468 6520 6576  ontaining the ev
+00002660: 616c 7561 7469 6f6e 2074 6172 6765 7473  aluation targets
+00002670: 2e0a 2020 2020 2020 2020 3a70 6172 616d  ..        :param
+00002680: 203a 7461 7267 6574 5f63 6f6c 3a20 5461   :target_col: Ta
+00002690: 6b65 7320 6120 7374 7269 6e67 2063 6f6e  kes a string con
+000026a0: 7461 696e 696e 6720 7468 6520 6e61 6d65  taining the name
+000026b0: 206f 6620 7468 6520 7461 7267 6574 2063   of the target c
+000026c0: 6f6c 756d 6e20 696e 7369 6465 2074 6865  olumn inside the
+000026d0: 2074 7261 696e 696e 6720 6461 7461 2064   training data d
+000026e0: 662e 0a20 2020 2020 2020 2029 0472 5300  f..        ).rS.
+000026f0: 0000 da07 7072 6564 6963 7472 0d00 0000  ....predictr....
+00002700: da06 7661 6c75 6573 2908 7231 0000 0072  ..values).r1...r
+00002710: 3500 0000 725d 0000 0072 5e00 0000 7246  5...r]...r^...rF
+00002720: 0000 00da 0779 5f70 726f 6273 da09 795f  .....y_probs..y_
+00002730: 636c 6173 7365 735a 0965 7661 6c5f 6469  classesZ.eval_di
+00002740: 6374 7232 0000 0072 3200 0000 7233 0000  ctr2...r2...r3..
+00002750: 00da 0866 6974 5f65 7661 6c16 0100 0073  ...fit_eval....s
+00002760: 0800 0000 0c10 0e01 0e01 0401 7a11 426c  ............z.Bl
+00002770: 7565 4361 7374 2e66 6974 5f65 7661 6c63  ueCast.fit_evalc
+00002780: 0200 0000 0000 0000 0000 0000 0300 0000  ................
+00002790: 0400 0000 4300 0000 7350 0100 0074 0083  ....C...sP...t..
+000027a0: 0001 007c 006a 0173 0a74 0264 0183 0182  ...|.j.s.t.d....
+000027b0: 017c 006a 0373 1174 0264 0283 0182 017c  .|.j.s.t.d.....|
+000027c0: 006a 016a 047c 017c 006a 0567 0164 038d  .j.j.|.|.j.g.d..
+000027d0: 027d 017c 006a 0672 2e7c 006a 066a 077c  .}.|.j.r.|.j.j.|
+000027e0: 0164 0464 058d 025c 027d 017d 027c 016a  .d.d...\.}.}.|.j
+000027f0: 0864 0464 068d 017d 0174 097c 0183 017d  .d.d...}.t.|...}
+00002800: 0174 0a7c 017c 006a 0b83 027d 017c 006a  .t.|.|.j...}.|.j
+00002810: 0c72 417c 006a 0ca0 077c 01a1 017d 017c  .rA|.j...|...}.|
+00002820: 006a 0d72 5d7c 006a 0e72 5d7c 006a 0f64  .j.r]|.j.r]|.j.d
+00002830: 076b 0272 5d74 107c 006a 0e74 1183 0272  .k.r]t.|.j.t...r
+00002840: 5d7c 006a 036a 1273 5d7c 006a 0ea0 137c  ]|.j.j.s]|.j...|
+00002850: 01a1 017d 016e 2b7c 006a 0d72 797c 006a  ...}.n+|.j.ry|.j
+00002860: 0e72 797c 006a 0f64 086b 0272 7974 107c  .ry|.j.d.k.ryt.|
+00002870: 006a 0e74 1483 0272 797c 006a 036a 1273  .j.t...ry|.j.j.s
+00002880: 797c 006a 0ea0 157c 01a1 017d 016e 0f7c  y|.j...|...}.n.|
+00002890: 006a 036a 1272 887c 017c 006a 0d19 00a0  .j.j.r.|.|.j....
+000028a0: 1664 09a1 017c 017c 006a 0d3c 007c 006a  .d...|.|.j.<.|.j
+000028b0: 1772 957c 006a 176a 077c 0164 0464 058d  .r.|.j.j.|.d.d..
+000028c0: 025c 027d 017d 027c 006a 1872 a67c 006a  .\.}.}.|.j.r.|.j
+000028d0: 036a 1972 a67c 006a 186a 077c 0164 0464  .j.r.|.j.j.|.d.d
+000028e0: 058d 025c 027d 017d 027c 0153 0029 0a7a  ...\.}.}.|.S.).z
+000028f0: 3754 7261 6e73 666f 726d 206e 6577 2064  7Transform new d
+00002900: 6174 6120 6163 636f 7264 696e 6720 746f  ata according to
+00002910: 2070 7265 7072 6f63 6573 7369 6e67 2070   preprocessing p
+00002920: 6970 656c 696e 652e fa2a 4665 6174 7572  ipeline..*Featur
+00002930: 6520 7479 7065 2063 6f6e 7665 7274 6572  e type converter
+00002940: 2063 6f75 6c64 206e 6f74 2062 6520 666f   could not be fo
+00002950: 756e 642e 7a2a 5472 6169 6e69 6e67 2063  und.z*Training c
+00002960: 6f6e 6669 6775 7261 7469 6f6e 2063 6f75  onfiguration cou
+00002970: 6c64 206e 6f74 2062 6520 666f 756e 642e  ld not be found.
+00002980: 2901 5a0b 6967 6e6f 7265 5f63 6f6c 7354  ).Z.ignore_colsT
+00002990: 7247 0000 0072 4900 0000 721e 0000 0072  rG...rI...r....r
+000029a0: 1f00 0000 724b 0000 0029 1a72 0f00 0000  ....rK...).r....
+000029b0: 722c 0000 00da 0945 7863 6570 7469 6f6e  r,.....Exception
+000029c0: 7228 0000 005a 1774 7261 6e73 666f 726d  r(...Z.transform
+000029d0: 5f66 6561 7475 7265 5f74 7970 6573 7220  _feature_typesr 
+000029e0: 0000 0072 2600 0000 7250 0000 0072 5100  ...r&...rP...rQ.
+000029f0: 0000 7217 0000 0072 1300 0000 7222 0000  ..r....r....r"..
+00002a00: 0072 2f00 0000 7221 0000 0072 2d00 0000  .r/...r!...r-...
+00002a10: 721d 0000 00da 0a69 7369 6e73 7461 6e63  r......isinstanc
+00002a20: 6572 1900 0000 7242 0000 0072 5400 0000  er....rB...rT...
+00002a30: 721a 0000 0072 5500 0000 7256 0000 0072  r....rU...rV...r
+00002a40: 2500 0000 7227 0000 0072 3a00 0000 2903  %...r'...r:...).
+00002a50: 7231 0000 0072 3500 0000 725c 0000 0072  r1...r5...r\...r
+00002a60: 3200 0000 7232 0000 0072 3300 0000 da12  2...r2...r3.....
+00002a70: 7472 616e 7366 6f72 6d5f 6e65 775f 6461  transform_new_da
+00002a80: 7461 2b01 0000 7354 0000 0006 0206 0108  ta+...sT........
+00002a90: 0106 0208 0106 0208 0106 ff06 0414 010c  ................
+00002aa0: 0108 020c 0106 020c 0104 0302 ff04 0202  ................
+00002ab0: fe0a 030a 0102 ff06 0202 fe0e 0404 0202  ................
+00002ac0: ff04 0202 fe0a 030a 0102 ff06 0202 fe0e  ................
+00002ad0: 0408 0116 0106 0214 010e 0214 0104 027a  ...............z
+00002ae0: 1b42 6c75 6543 6173 742e 7472 616e 7366  .BlueCast.transf
+00002af0: 6f72 6d5f 6e65 775f 6461 7461 6302 0000  orm_new_datac...
+00002b00: 0000 0000 0000 0000 0004 0000 0005 0000  ................
+00002b10: 0043 0000 0073 9800 0000 7c00 6a00 7307  .C...s....|.j.s.
+00002b20: 7401 6401 8301 8201 7c00 6a02 730e 7401  t.d.....|.j.s.t.
+00002b30: 6402 8301 8201 7c00 6a03 7315 7404 6403  d.....|.j.s.t.d.
+00002b40: 8301 8201 7405 8300 0100 7c00 a006 7c01  ....t.....|...|.
+00002b50: a101 7d01 7407 7408 a009 a100 9b00 6404  ..}.t.t.......d.
+00002b60: 9d02 8301 0100 7c00 6a00 a00a 7c01 a101  ......|.j...|...
+00002b70: 5c02 7d02 7d03 7c00 6a02 6a0b 7248 7c00  \.}.}.|.j.j.rH|.
+00002b80: 6a0c 7c00 6a02 6a0b 7600 7248 7c00 6a0d  j.|.j.j.v.rH|.j.
+00002b90: 7248 7c00 6a02 7248 7c00 6a0d a00e 740f  rH|.j.rH|.j...t.
+00002ba0: a010 7c03 a101 a101 7d03 7c02 7c03 6602  ..|.....}.|.|.f.
+00002bb0: 5300 2905 7a90 5072 6564 6963 7420 6f6e  S.).z.Predict on
+00002bc0: 2075 6e73 6565 6e20 6461 7461 2e0a 0a20   unseen data... 
+00002bd0: 2020 2020 2020 2052 6574 7572 6e20 7468         Return th
+00002be0: 6520 7072 6564 6963 7465 6420 7072 6f62  e predicted prob
+00002bf0: 6162 696c 6974 6965 7320 616e 6420 7468  abilities and th
+00002c00: 6520 7072 6564 6963 7465 6420 636c 6173  e predicted clas
+00002c10: 7365 733a 0a20 2020 2020 2020 2079 5f70  ses:.        y_p
+00002c20: 726f 6273 2c20 795f 636c 6173 7365 7320  robs, y_classes 
+00002c30: 3d20 7072 6564 6963 7428 6466 290a 2020  = predict(df).  
+00002c40: 2020 2020 2020 7a1b 4d6c 206d 6f64 656c        z.Ml model
+00002c50: 2063 6f75 6c64 206e 6f74 2062 6520 666f   could not be fo
+00002c60: 756e 6472 6400 0000 7a15 636f 6e66 5f74  undrd...z.conf_t
+00002c70: 7261 696e 696e 6720 6973 204e 6f6e 657a  raining is Nonez
+00002c80: 0f3a 2050 7265 6469 6374 696e 672e 2e2e  .: Predicting...
+00002c90: 2911 7224 0000 0072 6500 0000 722c 0000  ).r$...re...r,..
+00002ca0: 0072 2800 0000 da0a 5661 6c75 6545 7272  .r(.....ValueErr
+00002cb0: 6f72 720f 0000 0072 6700 0000 7210 0000  orr....rg...r...
+00002cc0: 0072 0200 0000 da06 7574 636e 6f77 725f  .r......utcnowr_
+00002cd0: 0000 0072 2100 0000 7220 0000 0072 2e00  ...r!...r ...r..
+00002ce0: 0000 5a1f 6c61 6265 6c5f 656e 636f 6465  ..Z.label_encode
+00002cf0: 725f 7265 7665 7273 655f 7472 616e 7366  r_reverse_transf
+00002d00: 6f72 6dda 0270 64da 0653 6572 6965 7329  orm..pd..Series)
+00002d10: 0472 3100 0000 7235 0000 0072 6100 0000  .r1...r5...ra...
+00002d20: 7262 0000 0072 3200 0000 7232 0000 0072  rb...r2...r2...r
+00002d30: 3300 0000 725f 0000 005d 0100 0073 2800  3...r_...]...s(.
+00002d40: 0000 0606 0801 0602 0801 0602 0801 0602  ................
+00002d50: 0a01 1202 1001 0802 0e02 0401 02ff 0402  ................
+00002d60: 02fe 0604 0801 04ff 0804 7a10 426c 7565  ..........z.Blue
+00002d70: 4361 7374 2e70 7265 6469 6374 290a 4e4e  Cast.predict).NN
+00002d80: 4e4e 4e4e 4e4e 4e4e 291f da08 5f5f 6e61  NNNNNNNN)...__na
+00002d90: 6d65 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f  me__..__module__
+00002da0: da0c 5f5f 7175 616c 6e61 6d65 5f5f da07  ..__qualname__..
+00002db0: 5f5f 646f 635f 5f72 0600 0000 7209 0000  __doc__r....r...
+00002dc0: 00da 0373 7472 da05 666c 6f61 74da 0369  ...str..float..i
+00002dd0: 6e74 7207 0000 0072 0500 0000 7211 0000  ntr....r....r...
+00002de0: 0072 0300 0000 7212 0000 0072 1500 0000  .r....r....r....
+00002df0: 720a 0000 0072 0c00 0000 720b 0000 0072  r....r....r....r
+00002e00: 3400 0000 726a 0000 00da 0944 6174 6146  4...rj.....DataF
+00002e10: 7261 6d65 7245 0000 0072 5300 0000 726b  ramerE...rS...rk
+00002e20: 0000 0072 0400 0000 7263 0000 0072 6700  ...r....rc...rg.
+00002e30: 0000 7208 0000 00da 026e 70da 076e 6461  ..r......np..nda
+00002e40: 7272 6179 725f 0000 0072 3200 0000 7232  rrayr_...r2...r2
+00002e50: 0000 0072 3200 0000 7233 0000 0072 1c00  ...r2...r3...r..
+00002e60: 0000 2700 0000 736c 0000 0008 0004 0102  ..'...sl........
+00002e70: 1802 0102 0102 0102 0102 0102 0302 0102  ................
+00002e80: 0102 0104 f106 0202 fe0c 0302 fd14 0402  ................
+00002e90: fc14 0502 fb06 0602 fa0e 0702 f906 0802  ................
+00002ea0: f806 0902 f702 0a0a 0102 ff02 f606 0d02  ................
+00002eb0: f306 0e02 f206 0f0a f114 2618 4402 7004  ..........&.D.p.
+00002ec0: 0202 fe04 0302 fd04 0402 fc02 0502 fb0a  ................
+00002ed0: 060a fa16 1524 3272 1c00 0000 2930 726f  .....$2r....)0ro
+00002ee0: 0000 0072 3b00 0000 7202 0000 00da 0674  ...r;...r......t
+00002ef0: 7970 696e 6772 0300 0000 7204 0000 0072  ypingr....r....r
+00002f00: 0500 0000 7206 0000 0072 0700 0000 7208  ....r....r....r.
+00002f10: 0000 0072 0900 0000 da05 6e75 6d70 7972  ...r......numpyr
+00002f20: 7400 0000 da06 7061 6e64 6173 726a 0000  t.....pandasrj..
+00002f30: 00da 1f62 6c75 6563 6173 742e 636f 6e66  ...bluecast.conf
+00002f40: 6967 2e74 7261 696e 696e 675f 636f 6e66  ig.training_conf
+00002f50: 6967 720a 0000 0072 0b00 0000 720c 0000  igr....r....r...
+00002f60: 005a 2062 6c75 6563 6173 742e 6576 616c  .Z bluecast.eval
+00002f70: 7561 7469 6f6e 2e65 7661 6c5f 6d65 7472  uation.eval_metr
+00002f80: 6963 7372 0d00 0000 5a1f 626c 7565 6361  icsr....Z.blueca
+00002f90: 7374 2e65 7661 6c75 6174 696f 6e2e 7368  st.evaluation.sh
+00002fa0: 6170 5f76 616c 7565 7372 0e00 0000 5a24  ap_valuesr....Z$
+00002fb0: 626c 7565 6361 7374 2e67 656e 6572 616c  bluecast.general
+00002fc0: 5f75 7469 6c73 2e67 656e 6572 616c 5f75  _utils.general_u
+00002fd0: 7469 6c73 720f 0000 0072 1000 0000 5a1d  tilsr....r....Z.
+00002fe0: 626c 7565 6361 7374 2e6d 6c5f 6d6f 6465  bluecast.ml_mode
+00002ff0: 6c6c 696e 672e 7867 626f 6f73 7472 1100  lling.xgboostr..
+00003000: 0000 da1d 626c 7565 6361 7374 2e70 7265  ....bluecast.pre
+00003010: 7072 6f63 6573 7369 6e67 2e63 7573 746f  processing.custo
+00003020: 6d72 1200 0000 5a28 626c 7565 6361 7374  mr....Z(bluecast
+00003030: 2e70 7265 7072 6f63 6573 7369 6e67 2e64  .preprocessing.d
+00003040: 6174 6574 696d 655f 6665 6174 7572 6573  atetime_features
+00003050: 7213 0000 005a 2b62 6c75 6563 6173 742e  r....Z+bluecast.
+00003060: 7072 6570 726f 6365 7373 696e 672e 656e  preprocessing.en
+00003070: 636f 6465 5f74 6172 6765 745f 6c61 6265  code_target_labe
+00003080: 6c73 7214 0000 005a 2862 6c75 6563 6173  lsr....Z(bluecas
+00003090: 742e 7072 6570 726f 6365 7373 696e 672e  t.preprocessing.
+000030a0: 6665 6174 7572 655f 7365 6c65 6374 696f  feature_selectio
+000030b0: 6e72 1500 0000 5a24 626c 7565 6361 7374  nr....Z$bluecast
+000030c0: 2e70 7265 7072 6f63 6573 7369 6e67 2e66  .preprocessing.f
+000030d0: 6561 7475 7265 5f74 7970 6573 7216 0000  eature_typesr...
+000030e0: 005a 2562 6c75 6563 6173 742e 7072 6570  .Z%bluecast.prep
+000030f0: 726f 6365 7373 696e 672e 6e75 6c6c 735f  rocessing.nulls_
+00003100: 616e 645f 696e 6673 7217 0000 005a 2462  and_infsr....Z$b
+00003110: 6c75 6563 6173 742e 7072 6570 726f 6365  luecast.preproce
+00003120: 7373 696e 672e 7363 6865 6d61 5f63 6865  ssing.schema_che
+00003130: 636b 7372 1800 0000 5a26 626c 7565 6361  cksr....Z&blueca
+00003140: 7374 2e70 7265 7072 6f63 6573 7369 6e67  st.preprocessing
+00003150: 2e74 6172 6765 745f 656e 636f 6469 6e67  .target_encoding
+00003160: 7219 0000 0072 1a00 0000 5a27 626c 7565  r....r....Z'blue
+00003170: 6361 7374 2e70 7265 7072 6f63 6573 7369  cast.preprocessi
+00003180: 6e67 2e74 7261 696e 5f74 6573 745f 7370  ng.train_test_sp
+00003190: 6c69 7472 1b00 0000 721c 0000 0072 3200  litr....r....r2.
+000031a0: 0000 7232 0000 0072 3200 0000 7233 0000  ..r2...r2...r3..
+000031b0: 00da 083c 6d6f 6475 6c65 3e01 0000 0073  ...<module>....s
+000031c0: 2a00 0000 0400 0808 0c01 2401 0802 0801  *.........$.....
+000031d0: 1402 0c05 0c01 1001 0c01 0c01 0c01 0c01  ................
+000031e0: 0c01 0c01 0c01 0c01 1001 0c04 1203       ..............
```

### Comparing `bluecast-0.5/bluecast/blueprints/cast.py` & `bluecast-0.7/bluecast/blueprints/cast.py`

 * *Files 10% similar despite different names*

```diff
@@ -131,17 +131,40 @@
             self.conf_training.min_features_to_select >= len(df.columns)
             and self.conf_training.enable_feature_selection
         ):
             message = """The minimum number of features to select is greater or equal to the number of features in
             the dataset while feature selection is enabled. Consider reducing the minimum number of features to
             select or disabling feature selection via TrainingConfig."""
             warnings.warn(message, UserWarning, stacklevel=2)
-        if self.target_column in df.columns:
-            message = """The target column is present in the dataset. Consider removing the target column from the
-            dataset to prevent leakage."""
+        if (
+            self.conf_training.cat_encoding_via_ml_algorithm
+            and self.conf_training.calculate_shap_values
+        ):
+            self.conf_training.calculate_shap_values = False
+            message = """SHAP values cannot be calculated when categorical encoding via ML algorithm is enabled due to
+            incompatibility with the shap library. See this GitHub issue for more context:
+            https://github.com/slundberg/shap/issues/266
+
+            Calculation of Shap values has been changed to false.
+            Consider disabling categorical encoding via ML algorithm in the TrainingConfig if shap values are
+            required. Alternatively use Xgboost as a custom model and calculate shap values manually via
+            pred_contribs=True."""
+            warnings.warn(message, UserWarning, stacklevel=2)
+        if self.conf_training.cat_encoding_via_ml_algorithm and self.ml_model:
+            message = """Categorical encoding via ML algorithm is enabled. Make sure to handle categorical features
+            within the provided ml model or consider disabling categorical encoding via ML algorithm in the
+            TrainingConfig alternatively."""
+            warnings.warn(message, UserWarning, stacklevel=2)
+        if (
+            self.conf_training.cat_encoding_via_ml_algorithm
+            and self.custom_last_mile_computation
+        ):
+            message = """Categorical encoding via ML algorithm is enabled. Make sure to handle categorical features
+            within the provided last mile computation or consider disabling categorical encoding via ML algorithm in the
+            TrainingConfig alternatively."""
             warnings.warn(message, UserWarning, stacklevel=2)
 
     def fit(self, df: pd.DataFrame, target_col: str) -> None:
         """Train a full ML pipeline."""
         check_gpu_support()
         feat_type_detector = FeatureTypeDetector()
         df = feat_type_detector.fit_transform_feature_types(df)
@@ -194,22 +217,33 @@
             x_test, self.date_columns
         )
 
         self.schema_detector = SchemaDetector()
         self.schema_detector.fit(x_train)
         x_test = self.schema_detector.transform(x_test)
 
-        if self.cat_columns is not None and self.class_problem == "binary":
+        if (
+            self.cat_columns is not None
+            and self.class_problem == "binary"
+            and not self.conf_training.cat_encoding_via_ml_algorithm
+        ):
             self.cat_encoder = BinaryClassTargetEncoder(feat_type_detector.cat_columns)
             x_train = self.cat_encoder.fit_target_encode_binary_class(x_train, y_train)
             x_test = self.cat_encoder.transform_target_encode_binary_class(x_test)
-        elif self.cat_columns is not None and self.class_problem == "multiclass":
+        elif (
+            self.cat_columns is not None
+            and self.class_problem == "multiclass"
+            and not self.conf_training.cat_encoding_via_ml_algorithm
+        ):
             self.cat_encoder = MultiClassTargetEncoder(feat_type_detector.cat_columns)
             x_train = self.cat_encoder.fit_target_encode_multiclass(x_train, y_train)
             x_test = self.cat_encoder.transform_target_encode_multiclass(x_test)
+        elif self.conf_training.cat_encoding_via_ml_algorithm:
+            x_train[self.cat_columns] = x_train[self.cat_columns].astype("category")
+            x_test[self.cat_columns] = x_test[self.cat_columns].astype("category")
 
         if self.custom_last_mile_computation:
             x_train, y_train = self.custom_last_mile_computation.fit_transform(
                 x_train, y_train
             )
             x_test, y_test = self.custom_last_mile_computation.transform(
                 x_test, y_test, predicton_mode=False
@@ -286,23 +320,27 @@
             df = self.schema_detector.transform(df)
 
         if (
             self.cat_columns
             and self.cat_encoder
             and self.class_problem == "binary"
             and isinstance(self.cat_encoder, BinaryClassTargetEncoder)
+            and not self.conf_training.cat_encoding_via_ml_algorithm
         ):
             df = self.cat_encoder.transform_target_encode_binary_class(df)
         elif (
             self.cat_columns
             and self.cat_encoder
             and self.class_problem == "multiclass"
             and isinstance(self.cat_encoder, MultiClassTargetEncoder)
+            and not self.conf_training.cat_encoding_via_ml_algorithm
         ):
             df = self.cat_encoder.transform_target_encode_multiclass(df)
+        elif self.conf_training.cat_encoding_via_ml_algorithm:
+            df[self.cat_columns] = df[self.cat_columns].astype("category")
 
         if self.custom_last_mile_computation:
             df, _ = self.custom_last_mile_computation.transform(df, predicton_mode=True)
 
         if self.custom_feature_selector and self.conf_training.enable_feature_selection:
             df, _ = self.custom_feature_selector.transform(df, predicton_mode=True)
 
@@ -316,14 +354,17 @@
         """
         if not self.ml_model:
             raise Exception("Ml model could not be found")
 
         if not self.feat_type_detector:
             raise Exception("Feature type converter could not be found.")
 
+        if not self.conf_training:
+            raise ValueError("conf_training is None")
+
         check_gpu_support()
         df = self.transform_new_data(df)
 
         logger(f"{datetime.utcnow()}: Predicting...")
         y_probs, y_classes = self.ml_model.predict(df)
 
         if self.feat_type_detector.cat_columns:
```

### Comparing `bluecast-0.5/bluecast/config/__pycache__/training_config.cpython-310.pyc` & `bluecast-0.7/bluecast/config/__pycache__/training_config.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun Jun 25 05:34:02 2023 UTC, .py size: 2969 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 cad1 9764 990b 0000  o..........d....
+00000000: 6f0d 0d0a 0000 0000 6063 9d64 ff0b 0000  o.......`c.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 6800 0000 6400  .....@...sh...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 6d03 5a03  Z.d.d.l.m.Z.m.Z.
 00000040: 0100 6401 6403 6c04 6d05 5a05 0100 4700  ..d.d.l.m.Z...G.
 00000050: 6404 6405 8400 6405 8302 5a06 6505 4700  d.d...d...Z.e.G.
 00000060: 6406 6407 8400 6407 8302 8301 5a07 6505  d.d...d.....Z.e.
 00000070: 4700 6408 6409 8400 6409 8302 8301 5a08  G.d.d...d.....Z.
@@ -51,191 +51,198 @@
 00000320: 0000 fa45 2f68 6f6d 652f 7468 6f6d 6173  ...E/home/thomas
 00000330: 2f49 6465 6150 726f 6a65 6374 732f 426c  /IdeaProjects/Bl
 00000340: 7565 4361 7374 2f62 6c75 6563 6173 742f  ueCast/bluecast/
 00000350: 636f 6e66 6967 2f74 7261 696e 696e 675f  config/training_
 00000360: 636f 6e66 6967 2e70 7972 0500 0000 0d00  config.pyr......
 00000370: 0000 7304 0000 0008 0008 0172 0500 0000  ..s........r....
 00000380: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
-00000390: 0003 0000 0040 0000 0073 ae00 0000 6500  .....@...s....e.
+00000390: 0003 0000 0040 0000 0073 ba00 0000 6500  .....@...s....e.
 000003a0: 5a01 6400 5a02 5500 6401 5a03 6402 5a04  Z.d.Z.U.d.Z.d.Z.
 000003b0: 6505 6506 6403 3c00 6404 5a07 6508 6506  e.e.d.<.d.Z.e.e.
 000003c0: 6405 3c00 6406 5a09 6505 6506 6407 3c00  d.<.d.Z.e.e.d.<.
 000003d0: 6408 5a0a 6505 6506 6409 3c00 640a 5a0b  d.Z.e.e.d.<.d.Z.
 000003e0: 6505 6506 640b 3c00 6402 5a0c 6505 6506  e.e.d.<.d.Z.e.e.
 000003f0: 640c 3c00 6404 5a0d 6508 6506 640d 3c00  d.<.d.Z.e.e.d.<.
 00000400: 640e 5a0e 6508 6506 640f 3c00 6404 5a0f  d.Z.e.e.d.<.d.Z.
 00000410: 6508 6506 6410 3c00 6411 5a10 6511 6506  e.e.d.<.d.Z.e.e.
 00000420: 6412 3c00 6404 5a12 6508 6506 6413 3c00  d.<.d.Z.e.e.d.<.
 00000430: 6404 5a13 6508 6506 6414 3c00 6415 5a14  d.Z.e.e.d.<.d.Z.
-00000440: 6505 6506 6416 3c00 6417 5300 2918 da0e  e.e.d.<.d.S.)...
-00000450: 5472 6169 6e69 6e67 436f 6e66 6967 7a23  TrainingConfigz#
-00000460: 4465 6669 6e65 2067 656e 6572 616c 2074  Define general t
-00000470: 7261 696e 696e 6720 7061 7261 6d65 7465  raining paramete
-00000480: 7273 2ee9 0a00 0000 da13 676c 6f62 616c  rs........global
-00000490: 5f72 616e 646f 6d5f 7374 6174 6554 da17  _random_stateT..
-000004a0: 7368 7566 666c 655f 6475 7269 6e67 5f74  shuffle_during_t
-000004b0: 7261 696e 696e 67e9 6400 0000 da1c 6879  raining.d.....hy
-000004c0: 7065 7270 6172 616d 6574 6572 5f74 756e  perparameter_tun
-000004d0: 696e 675f 726f 756e 6473 6910 0e00 00da  ing_roundsi.....
-000004e0: 2668 7970 6572 7061 7261 6d65 7465 725f  &hyperparameter_
-000004f0: 7475 6e69 6e67 5f6d 6178 5f72 756e 7469  tuning_max_runti
-00000500: 6d65 5f73 6563 73e9 0100 0000 da14 6879  me_secs.......hy
-00000510: 7065 7274 756e 696e 675f 6376 5f66 6f6c  pertuning_cv_fol
-00000520: 6473 da15 6561 726c 795f 7374 6f70 7069  ds..early_stoppi
-00000530: 6e67 5f72 6f75 6e64 73da 0e61 7574 6f74  ng_rounds..autot
-00000540: 756e 655f 6d6f 6465 6c46 da18 656e 6162  une_modelF..enab
-00000550: 6c65 5f66 6561 7475 7265 5f73 656c 6563  le_feature_selec
-00000560: 7469 6f6e da15 6361 6c63 756c 6174 655f  tion..calculate_
-00000570: 7368 6170 5f76 616c 7565 73e7 9a99 9999  shap_values.....
-00000580: 9999 e93f da0a 7472 6169 6e5f 7369 7a65  ...?..train_size
-00000590: da14 7472 6169 6e5f 7370 6c69 745f 7374  ..train_split_st
-000005a0: 7261 7469 6679 da1d 7573 655f 6675 6c6c  ratify..use_full
-000005b0: 5f64 6174 615f 666f 725f 6669 6e61 6c5f  _data_for_final_
-000005c0: 6d6f 6465 6ce9 0500 0000 da16 6d69 6e5f  model.......min_
-000005d0: 6665 6174 7572 6573 5f74 6f5f 7365 6c65  features_to_sele
-000005e0: 6374 4e29 1572 0600 0000 7207 0000 0072  ctN).r....r....r
-000005f0: 0800 0000 da07 5f5f 646f 635f 5f72 0d00  ......__doc__r..
-00000600: 0000 da03 696e 74da 0f5f 5f61 6e6e 6f74  ....int..__annot
-00000610: 6174 696f 6e73 5f5f 720e 0000 00da 0462  ations__r......b
-00000620: 6f6f 6c72 1000 0000 7211 0000 0072 1300  oolr....r....r..
-00000630: 0000 7214 0000 0072 1500 0000 7216 0000  ..r....r....r...
-00000640: 0072 1700 0000 7219 0000 00da 0566 6c6f  .r....r......flo
-00000650: 6174 721a 0000 0072 1b00 0000 721d 0000  atr....r....r...
-00000660: 0072 0900 0000 7209 0000 0072 0900 0000  .r....r....r....
-00000670: 720a 0000 0072 0b00 0000 1100 0000 731e  r....r........s.
-00000680: 0000 000a 0004 020c 020c 010c 010c 010c  ................
-00000690: 010c 010c 010c 010c 010c 010c 010c 0110  ................
-000006a0: 0172 0b00 0000 6300 0000 0000 0000 0000  .r....c.........
-000006b0: 0000 0000 0000 0003 0000 0040 0000 0073  ...........@...s
-000006c0: 4a01 0000 6500 5a01 6400 5a02 5500 6401  J...e.Z.d.Z.U.d.
-000006d0: 5a03 6402 5a04 6505 6506 6403 3c00 6404  Z.d.Z.e.e.d.<.d.
-000006e0: 5a07 6505 6506 6405 3c00 6406 5a08 6509  Z.e.e.d.<.d.Z.e.
-000006f0: 6506 6407 3c00 6408 5a0a 6509 6506 6409  e.d.<.d.Z.e.e.d.
-00000700: 3c00 6406 5a0b 6509 6506 640a 3c00 6408  <.d.Z.e.e.d.<.d.
-00000710: 5a0c 6509 6506 640b 3c00 6402 5a0d 6505  Z.e.e.d.<.d.Z.e.
-00000720: 6506 640c 3c00 640d 5a0e 6505 6506 640e  e.d.<.d.Z.e.e.d.
-00000730: 3c00 640f 5a0f 6509 6506 6410 3c00 6406  <.d.Z.e.e.d.<.d.
-00000740: 5a10 6509 6506 6411 3c00 640f 5a11 6509  Z.e.e.d.<.d.Z.e.
-00000750: 6506 6412 3c00 6406 5a12 6509 6506 6413  e.d.<.d.Z.e.e.d.
-00000760: 3c00 640f 5a13 6509 6506 6414 3c00 6406  <.d.Z.e.e.d.<.d.
-00000770: 5a14 6509 6506 6415 3c00 640f 5a15 6509  Z.e.e.d.<.d.Z.e.
-00000780: 6506 6416 3c00 6406 5a16 6509 6506 6417  e.d.<.d.Z.e.e.d.
-00000790: 3c00 6402 5a17 6505 6506 6418 3c00 6419  <.d.Z.e.e.d.<.d.
-000007a0: 5a18 6505 6506 641a 3c00 641b 5a19 6509  Z.e.e.d.<.d.Z.e.
-000007b0: 6506 641c 3c00 6402 5a1a 6505 6506 641d  e.d.<.d.Z.e.e.d.
-000007c0: 3c00 641e 5a1b 6505 6506 641f 3c00 6420  <.d.Z.e.e.d.<.d 
-000007d0: 5a1c 6505 6506 6421 3c00 6404 5a1d 6505  Z.e.e.d!<.d.Z.e.
-000007e0: 6506 6422 3c00 6423 5a1e 6505 6506 6424  e.d"<.d#Z.e.e.d$
-000007f0: 3c00 6425 5a1f 6520 6506 6426 3c00 6427  <.d%Z.e e.d&<.d'
-00000800: 5a21 6520 6506 6428 3c00 6429 5300 292a  Z!e e.d(<.d)S.)*
-00000810: da17 5867 626f 6f73 7454 756e 6550 6172  ..XgboostTunePar
-00000820: 616d 7343 6f6e 6669 677a 2a44 6566 696e  amsConfigz*Defin
-00000830: 6520 6879 7065 7270 6172 616d 6574 6572  e hyperparameter
-00000840: 2074 756e 696e 6720 7365 6172 6368 2073   tuning search s
-00000850: 7061 6365 2ee9 0200 0000 da0d 6d61 785f  pace........max_
-00000860: 6465 7074 685f 6d69 6ee9 0300 0000 da0d  depth_min.......
-00000870: 6d61 785f 6465 7074 685f 6d61 7867 0000  max_depth_maxg..
-00000880: 0000 0000 f03f da09 616c 7068 615f 6d69  .....?..alpha_mi
-00000890: 6e67 0000 0000 0040 8f40 da09 616c 7068  ng.....@.@..alph
-000008a0: 615f 6d61 78da 0a6c 616d 6264 615f 6d69  a_max..lambda_mi
-000008b0: 6eda 0a6c 616d 6264 615f 6d61 78da 0e6e  n..lambda_max..n
-000008c0: 756d 5f6c 6561 7665 735f 6d69 6ee9 4000  um_leaves_min.@.
-000008d0: 0000 da0e 6e75 6d5f 6c65 6176 6573 5f6d  ....num_leaves_m
-000008e0: 6178 6733 3333 3333 33d3 3fda 0e73 7562  axg333333.?..sub
-000008f0: 5f73 616d 706c 655f 6d69 6eda 0e73 7562  _sample_min..sub
-00000900: 5f73 616d 706c 655f 6d61 78da 1663 6f6c  _sample_max..col
-00000910: 5f73 616d 706c 655f 6279 5f74 7265 655f  _sample_by_tree_
-00000920: 6d69 6eda 1663 6f6c 5f73 616d 706c 655f  min..col_sample_
-00000930: 6279 5f74 7265 655f 6d61 78da 1763 6f6c  by_tree_max..col
-00000940: 5f73 616d 706c 655f 6279 5f6c 6576 656c  _sample_by_level
-00000950: 5f6d 696e da17 636f 6c5f 7361 6d70 6c65  _min..col_sample
-00000960: 5f62 795f 6c65 7665 6c5f 6d61 78da 1663  _by_level_max..c
-00000970: 6f6c 5f73 616d 706c 655f 6279 5f6e 6f64  ol_sample_by_nod
-00000980: 655f 6d69 6eda 1663 6f6c 5f73 616d 706c  e_min..col_sampl
-00000990: 655f 6279 5f6e 6f64 655f 6d61 78da 156d  e_by_node_max..m
-000009a0: 696e 5f63 6869 6c64 5f73 616d 706c 6573  in_child_samples
-000009b0: 5f6d 696e e9e8 0300 00da 156d 696e 5f63  _min.......min_c
-000009c0: 6869 6c64 5f73 616d 706c 6573 5f6d 6178  hild_samples_max
-000009d0: e79a 9999 9999 99b9 3fda 0365 7461 da09  ........?..eta..
-000009e0: 7374 6570 735f 6d69 6e69 50c3 0000 da09  steps_miniP.....
-000009f0: 7374 6570 735f 6d61 7872 1200 0000 da15  steps_maxr......
-00000a00: 6e75 6d5f 7061 7261 6c6c 656c 5f74 7265  num_parallel_tre
-00000a10: 655f 6d69 6eda 156e 756d 5f70 6172 616c  e_min..num_paral
-00000a20: 6c65 6c5f 7472 6565 5f6d 6178 7201 0000  lel_tree_maxr...
-00000a30: 00da 0f6d 6f64 656c 5f76 6572 626f 7369  ...model_verbosi
-00000a40: 7479 fa0e 6d75 6c74 693a 736f 6674 7072  ty..multi:softpr
-00000a50: 6f62 da0f 6d6f 6465 6c5f 6f62 6a65 6374  ob..model_object
-00000a60: 6976 65da 086d 6c6f 676c 6f73 73da 116d  ive..mlogloss..m
-00000a70: 6f64 656c 5f65 7661 6c5f 6d65 7472 6963  odel_eval_metric
-00000a80: 4e29 2272 0600 0000 7207 0000 0072 0800  N)"r....r....r..
-00000a90: 0000 721e 0000 0072 2500 0000 721f 0000  ..r....r%...r...
-00000aa0: 0072 2000 0000 7227 0000 0072 2800 0000  .r ...r'...r(...
-00000ab0: 7222 0000 0072 2900 0000 722a 0000 0072  r"...r)...r*...r
-00000ac0: 2b00 0000 722c 0000 0072 2e00 0000 722f  +...r,...r....r/
-00000ad0: 0000 0072 3000 0000 7231 0000 0072 3200  ...r0...r1...r2.
-00000ae0: 0000 7233 0000 0072 3400 0000 7235 0000  ..r3...r4...r5..
-00000af0: 0072 3600 0000 7237 0000 0072 3900 0000  .r6...r7...r9...
-00000b00: 723b 0000 0072 3c00 0000 723d 0000 0072  r;...r<...r=...r
-00000b10: 3e00 0000 723f 0000 0072 4000 0000 7242  >...r?...r@...rB
-00000b20: 0000 00da 0373 7472 7244 0000 0072 0900  .....strrD...r..
-00000b30: 0000 7209 0000 0072 0900 0000 720a 0000  ..r....r....r...
-00000b40: 0072 2300 0000 2400 0000 7338 0000 000a  .r#...$...s8....
-00000b50: 0004 020c 020c 010c 010c 010c 010c 010c  ................
-00000b60: 010c 010c 010c 010c 010c 010c 010c 010c  ................
-00000b70: 010c 010c 010c 010c 010c 010c 010c 010c  ................
-00000b80: 010c 010c 0110 0172 2300 0000 6300 0000  .......r#...c...
-00000b90: 0000 0000 0000 0000 0000 0000 0004 0000  ................
-00000ba0: 0040 0000 0073 a000 0000 6500 5a01 6400  .@...s....e.Z.d.
-00000bb0: 5a02 5500 6401 5a03 6900 6402 6403 9301  Z.U.d.Z.i.d.d...
-00000bc0: 6404 6405 9301 6406 6407 9301 6408 6409  d.d...d.d...d.d.
-00000bd0: 9301 640a 640b 9301 640c 640d 9301 640e  ..d.d...d.d...d.
-00000be0: 640f 9301 6410 640f 9301 6411 6412 9301  d...d.d...d.d...
-00000bf0: 6413 6414 9301 6415 6414 9301 6416 6414  d.d...d.d...d.d.
-00000c00: 9301 6417 6414 9301 6418 6419 9301 641a  ..d.d...d.d...d.
-00000c10: 640f 9301 641b 641c 9301 641d 641e 9301  d...d.d...d.d...
-00000c20: 5a04 641f 5a05 6506 6507 6508 6509 6602  Z.d.Z.e.e.e.e.f.
-00000c30: 1900 1900 650a 6420 3c00 6421 5a0b 6509  ....e.d <.d!Z.e.
-00000c40: 650a 6422 3c00 641f 5300 2923 da17 5867  e.d"<.d.S.)#..Xg
-00000c50: 626f 6f73 7446 696e 616c 5061 7261 6d43  boostFinalParamC
-00000c60: 6f6e 6669 677a 1e44 6566 696e 6520 6669  onfigz.Define fi
-00000c70: 6e61 6c20 6879 7065 7220 7061 7261 6d65  nal hyper parame
-00000c80: 7465 7273 2eda 096f 626a 6563 7469 7665  ters...objective
-00000c90: 7241 0000 00da 0b65 7661 6c5f 6d65 7472  rA.....eval_metr
-00000ca0: 6963 7243 0000 00da 0776 6572 626f 7365  icrC.....verbose
-00000cb0: 7201 0000 00da 0b74 7265 655f 6d65 7468  r......tree_meth
-00000cc0: 6f64 da05 6578 6163 74da 096e 756d 5f63  od..exact..num_c
-00000cd0: 6c61 7373 7224 0000 00da 096d 6178 5f64  lassr$.....max_d
-00000ce0: 6570 7468 7226 0000 00da 0561 6c70 6861  epthr&.....alpha
-00000cf0: 723a 0000 00da 066c 616d 6264 61da 0a6e  r:.....lambda..n
-00000d00: 756d 5f6c 6561 7665 73e9 1000 0000 da09  um_leaves.......
-00000d10: 7375 6273 616d 706c 6572 1800 0000 da10  subsampler......
-00000d20: 636f 6c73 616d 706c 655f 6279 7472 6565  colsample_bytree
-00000d30: da11 636f 6c73 616d 706c 655f 6279 6c65  ..colsample_byle
-00000d40: 7665 6cda 1063 6f6c 7361 6d70 6c65 5f62  vel..colsample_b
-00000d50: 796e 6f64 65da 116d 696e 5f63 6869 6c64  ynode..min_child
-00000d60: 5f73 616d 706c 6573 720f 0000 0072 3b00  _samplesr....r;.
-00000d70: 0000 da05 7374 6570 7372 3800 0000 da11  ....stepsr8.....
-00000d80: 6e75 6d5f 7061 7261 6c6c 656c 5f74 7265  num_parallel_tre
-00000d90: 6572 1200 0000 4eda 0d73 616d 706c 655f  er....N..sample_
-00000da0: 7765 6967 6874 6700 0000 0000 00e0 3fda  weightg.......?.
-00000db0: 1863 6c61 7373 6966 6963 6174 696f 6e5f  .classification_
-00000dc0: 7468 7265 7368 6f6c 6429 0c72 0600 0000  threshold).r....
-00000dd0: 7207 0000 0072 0800 0000 721e 0000 00da  r....r....r.....
-00000de0: 0670 6172 616d 7372 5900 0000 7203 0000  .paramsrY...r...
-00000df0: 0072 0200 0000 7245 0000 0072 2200 0000  .r....rE...r"...
-00000e00: 7220 0000 0072 5a00 0000 7209 0000 0072  r ...rZ...r....r
-00000e10: 0900 0000 7209 0000 0072 0a00 0000 7246  ....r....r....rF
-00000e20: 0000 0044 0000 0073 4e00 0000 0a00 0402  ...D...sN.......
-00000e30: 0202 0401 02ff 0402 02fe 0403 02fd 0404  ................
-00000e40: 02fc 0405 02fb 0406 02fa 0407 02f9 0408  ................
-00000e50: 02f8 0409 02f7 040a 02f6 040b 02f5 040c  ................
-00000e60: 02f4 040d 02f3 040e 02f2 040f 02f1 0410  ................
-00000e70: 02f0 0411 04ef 1813 1001 7246 0000 004e  ..........rF...N
-00000e80: 290a 721e 0000 00da 0674 7970 696e 6772  ).r......typingr
-00000e90: 0200 0000 7203 0000 005a 1470 7964 616e  ....r....Z.pydan
-00000ea0: 7469 632e 6461 7461 636c 6173 7365 7372  tic.dataclassesr
-00000eb0: 0400 0000 7205 0000 0072 0b00 0000 7223  ....r....r....r#
-00000ec0: 0000 0072 4600 0000 7209 0000 0072 0900  ...rF...r....r..
-00000ed0: 0000 7209 0000 0072 0a00 0000 da08 3c6d  ..r....r......<m
-00000ee0: 6f64 756c 653e 0100 0000 7314 0000 0004  odule>....s.....
-00000ef0: 0010 070c 020e 0302 0410 0102 1210 0102  ................
-00000f00: 1f14 01                                  ...
+00000440: 6505 6506 6416 3c00 640e 5a15 6508 6506  e.e.d.<.d.Z.e.e.
+00000450: 6417 3c00 6418 5300 2919 da0e 5472 6169  d.<.d.S.)...Trai
+00000460: 6e69 6e67 436f 6e66 6967 7a23 4465 6669  ningConfigz#Defi
+00000470: 6e65 2067 656e 6572 616c 2074 7261 696e  ne general train
+00000480: 696e 6720 7061 7261 6d65 7465 7273 2ee9  ing parameters..
+00000490: 0a00 0000 da13 676c 6f62 616c 5f72 616e  ......global_ran
+000004a0: 646f 6d5f 7374 6174 6554 da17 7368 7566  dom_stateT..shuf
+000004b0: 666c 655f 6475 7269 6e67 5f74 7261 696e  fle_during_train
+000004c0: 696e 67e9 6400 0000 da1c 6879 7065 7270  ing.d.....hyperp
+000004d0: 6172 616d 6574 6572 5f74 756e 696e 675f  arameter_tuning_
+000004e0: 726f 756e 6473 6910 0e00 00da 2668 7970  roundsi.....&hyp
+000004f0: 6572 7061 7261 6d65 7465 725f 7475 6e69  erparameter_tuni
+00000500: 6e67 5f6d 6178 5f72 756e 7469 6d65 5f73  ng_max_runtime_s
+00000510: 6563 73e9 0100 0000 da14 6879 7065 7274  ecs.......hypert
+00000520: 756e 696e 675f 6376 5f66 6f6c 6473 da15  uning_cv_folds..
+00000530: 6561 726c 795f 7374 6f70 7069 6e67 5f72  early_stopping_r
+00000540: 6f75 6e64 73da 0e61 7574 6f74 756e 655f  ounds..autotune_
+00000550: 6d6f 6465 6c46 da18 656e 6162 6c65 5f66  modelF..enable_f
+00000560: 6561 7475 7265 5f73 656c 6563 7469 6f6e  eature_selection
+00000570: da15 6361 6c63 756c 6174 655f 7368 6170  ..calculate_shap
+00000580: 5f76 616c 7565 73e7 9a99 9999 9999 e93f  _values........?
+00000590: da0a 7472 6169 6e5f 7369 7a65 da14 7472  ..train_size..tr
+000005a0: 6169 6e5f 7370 6c69 745f 7374 7261 7469  ain_split_strati
+000005b0: 6679 da1d 7573 655f 6675 6c6c 5f64 6174  fy..use_full_dat
+000005c0: 615f 666f 725f 6669 6e61 6c5f 6d6f 6465  a_for_final_mode
+000005d0: 6ce9 0500 0000 da16 6d69 6e5f 6665 6174  l.......min_feat
+000005e0: 7572 6573 5f74 6f5f 7365 6c65 6374 da1d  ures_to_select..
+000005f0: 6361 745f 656e 636f 6469 6e67 5f76 6961  cat_encoding_via
+00000600: 5f6d 6c5f 616c 676f 7269 7468 6d4e 2916  _ml_algorithmN).
+00000610: 7206 0000 0072 0700 0000 7208 0000 00da  r....r....r.....
+00000620: 075f 5f64 6f63 5f5f 720d 0000 00da 0369  .__doc__r......i
+00000630: 6e74 da0f 5f5f 616e 6e6f 7461 7469 6f6e  nt..__annotation
+00000640: 735f 5f72 0e00 0000 da04 626f 6f6c 7210  s__r......boolr.
+00000650: 0000 0072 1100 0000 7213 0000 0072 1400  ...r....r....r..
+00000660: 0000 7215 0000 0072 1600 0000 7217 0000  ..r....r....r...
+00000670: 0072 1900 0000 da05 666c 6f61 7472 1a00  .r......floatr..
+00000680: 0000 721b 0000 0072 1d00 0000 721e 0000  ..r....r....r...
+00000690: 0072 0900 0000 7209 0000 0072 0900 0000  .r....r....r....
+000006a0: 720a 0000 0072 0b00 0000 1100 0000 7320  r....r........s 
+000006b0: 0000 000a 0004 020c 020c 010c 010c 010c  ................
+000006c0: 010c 010c 010c 010c 010c 010c 010c 010c  ................
+000006d0: 0110 0172 0b00 0000 6300 0000 0000 0000  ...r....c.......
+000006e0: 0000 0000 0000 0000 0003 0000 0040 0000  .............@..
+000006f0: 0073 6201 0000 6500 5a01 6400 5a02 5500  .sb...e.Z.d.Z.U.
+00000700: 6401 5a03 6402 5a04 6505 6506 6403 3c00  d.Z.d.Z.e.e.d.<.
+00000710: 6404 5a07 6505 6506 6405 3c00 6406 5a08  d.Z.e.e.d.<.d.Z.
+00000720: 6509 6506 6407 3c00 6408 5a0a 6509 6506  e.e.d.<.d.Z.e.e.
+00000730: 6409 3c00 640a 5a0b 6509 6506 640b 3c00  d.<.d.Z.e.e.d.<.
+00000740: 6408 5a0c 6509 6506 640c 3c00 6406 5a0d  d.Z.e.e.d.<.d.Z.
+00000750: 6509 6506 640d 3c00 6408 5a0e 6509 6506  e.e.d.<.d.Z.e.e.
+00000760: 640e 3c00 6402 5a0f 6505 6506 640f 3c00  d.<.d.Z.e.e.d.<.
+00000770: 6410 5a10 6505 6506 6411 3c00 6412 5a11  d.Z.e.e.d.<.d.Z.
+00000780: 6509 6506 6413 3c00 640a 5a12 6509 6506  e.e.d.<.d.Z.e.e.
+00000790: 6414 3c00 6412 5a13 6509 6506 6415 3c00  d.<.d.Z.e.e.d.<.
+000007a0: 640a 5a14 6509 6506 6416 3c00 6412 5a15  d.Z.e.e.d.<.d.Z.
+000007b0: 6509 6506 6417 3c00 640a 5a16 6509 6506  e.e.d.<.d.Z.e.e.
+000007c0: 6418 3c00 6412 5a17 6509 6506 6419 3c00  d.<.d.Z.e.e.d.<.
+000007d0: 640a 5a18 6509 6506 641a 3c00 6402 5a19  d.Z.e.e.d.<.d.Z.
+000007e0: 6505 6506 641b 3c00 641c 5a1a 6505 6506  e.e.d.<.d.Z.e.e.
+000007f0: 641d 3c00 641e 5a1b 6509 6506 641f 3c00  d.<.d.Z.e.e.d.<.
+00000800: 6402 5a1c 6505 6506 6420 3c00 6421 5a1d  d.Z.e.e.d <.d!Z.
+00000810: 6505 6506 6422 3c00 6423 5a1e 6505 6506  e.e.d"<.d#Z.e.e.
+00000820: 6424 3c00 6404 5a1f 6505 6506 6425 3c00  d$<.d.Z.e.e.d%<.
+00000830: 6426 5a20 6505 6506 6427 3c00 6428 5a21  d&Z e.e.d'<.d(Z!
+00000840: 6522 6506 6429 3c00 642a 5a23 6522 6506  e"e.d)<.d*Z#e"e.
+00000850: 642b 3c00 642c 5300 292d da17 5867 626f  d+<.d,S.)-..Xgbo
+00000860: 6f73 7454 756e 6550 6172 616d 7343 6f6e  ostTuneParamsCon
+00000870: 6669 677a 2a44 6566 696e 6520 6879 7065  figz*Define hype
+00000880: 7270 6172 616d 6574 6572 2074 756e 696e  rparameter tunin
+00000890: 6720 7365 6172 6368 2073 7061 6365 2ee9  g search space..
+000008a0: 0200 0000 da0d 6d61 785f 6465 7074 685f  ......max_depth_
+000008b0: 6d69 6ee9 0300 0000 da0d 6d61 785f 6465  min.......max_de
+000008c0: 7074 685f 6d61 7867 0000 0000 0000 0000  pth_maxg........
+000008d0: da09 616c 7068 615f 6d69 6e67 0000 0000  ..alpha_ming....
+000008e0: 0040 8f40 da09 616c 7068 615f 6d61 7867  .@.@..alpha_maxg
+000008f0: 0000 0000 0000 f03f da0a 6c61 6d62 6461  .......?..lambda
+00000900: 5f6d 696e da0a 6c61 6d62 6461 5f6d 6178  _min..lambda_max
+00000910: da09 6761 6d6d 615f 6d69 6eda 0967 616d  ..gamma_min..gam
+00000920: 6d61 5f6d 6178 da0e 6e75 6d5f 6c65 6176  ma_max..num_leav
+00000930: 6573 5f6d 696e e940 0000 00da 0e6e 756d  es_min.@.....num
+00000940: 5f6c 6561 7665 735f 6d61 7867 3333 3333  _leaves_maxg3333
+00000950: 3333 d33f da0e 7375 625f 7361 6d70 6c65  33.?..sub_sample
+00000960: 5f6d 696e da0e 7375 625f 7361 6d70 6c65  _min..sub_sample
+00000970: 5f6d 6178 da16 636f 6c5f 7361 6d70 6c65  _max..col_sample
+00000980: 5f62 795f 7472 6565 5f6d 696e da16 636f  _by_tree_min..co
+00000990: 6c5f 7361 6d70 6c65 5f62 795f 7472 6565  l_sample_by_tree
+000009a0: 5f6d 6178 da17 636f 6c5f 7361 6d70 6c65  _max..col_sample
+000009b0: 5f62 795f 6c65 7665 6c5f 6d69 6eda 1763  _by_level_min..c
+000009c0: 6f6c 5f73 616d 706c 655f 6279 5f6c 6576  ol_sample_by_lev
+000009d0: 656c 5f6d 6178 da16 636f 6c5f 7361 6d70  el_max..col_samp
+000009e0: 6c65 5f62 795f 6e6f 6465 5f6d 696e da16  le_by_node_min..
+000009f0: 636f 6c5f 7361 6d70 6c65 5f62 795f 6e6f  col_sample_by_no
+00000a00: 6465 5f6d 6178 da15 6d69 6e5f 6368 696c  de_max..min_chil
+00000a10: 645f 7361 6d70 6c65 735f 6d69 6ee9 e803  d_samples_min...
+00000a20: 0000 da15 6d69 6e5f 6368 696c 645f 7361  ....min_child_sa
+00000a30: 6d70 6c65 735f 6d61 78e7 9a99 9999 9999  mples_max.......
+00000a40: b93f da03 6574 61da 0973 7465 7073 5f6d  .?..eta..steps_m
+00000a50: 696e 6950 c300 00da 0973 7465 7073 5f6d  iniP.....steps_m
+00000a60: 6178 7212 0000 00da 156e 756d 5f70 6172  axr......num_par
+00000a70: 616c 6c65 6c5f 7472 6565 5f6d 696e da15  allel_tree_min..
+00000a80: 6e75 6d5f 7061 7261 6c6c 656c 5f74 7265  num_parallel_tre
+00000a90: 655f 6d61 7872 0100 0000 da0f 6d6f 6465  e_maxr......mode
+00000aa0: 6c5f 7665 7262 6f73 6974 79fa 0e6d 756c  l_verbosity..mul
+00000ab0: 7469 3a73 6f66 7470 726f 62da 0f6d 6f64  ti:softprob..mod
+00000ac0: 656c 5f6f 626a 6563 7469 7665 da08 6d6c  el_objective..ml
+00000ad0: 6f67 6c6f 7373 da11 6d6f 6465 6c5f 6576  ogloss..model_ev
+00000ae0: 616c 5f6d 6574 7269 634e 2924 7206 0000  al_metricN)$r...
+00000af0: 0072 0700 0000 7208 0000 0072 1f00 0000  .r....r....r....
+00000b00: 7226 0000 0072 2000 0000 7221 0000 0072  r&...r ...r!...r
+00000b10: 2800 0000 7229 0000 0072 2300 0000 722a  (...r)...r#...r*
+00000b20: 0000 0072 2b00 0000 722c 0000 0072 2d00  ...r+...r,...r-.
+00000b30: 0000 722e 0000 0072 2f00 0000 7231 0000  ..r....r/...r1..
+00000b40: 0072 3200 0000 7233 0000 0072 3400 0000  .r2...r3...r4...
+00000b50: 7235 0000 0072 3600 0000 7237 0000 0072  r5...r6...r7...r
+00000b60: 3800 0000 7239 0000 0072 3a00 0000 723c  8...r9...r:...r<
+00000b70: 0000 0072 3e00 0000 723f 0000 0072 4000  ...r>...r?...r@.
+00000b80: 0000 7241 0000 0072 4200 0000 7243 0000  ..rA...rB...rC..
+00000b90: 0072 4500 0000 da03 7374 7272 4700 0000  .rE.....strrG...
+00000ba0: 7209 0000 0072 0900 0000 7209 0000 0072  r....r....r....r
+00000bb0: 0a00 0000 7224 0000 0025 0000 0073 3c00  ....r$...%...s<.
+00000bc0: 0000 0a00 0402 0c02 0c01 0c01 0c01 0c01  ................
+00000bd0: 0c01 0c01 0c01 0c01 0c01 0c01 0c01 0c01  ................
+00000be0: 0c01 0c01 0c01 0c01 0c01 0c01 0c01 0c01  ................
+00000bf0: 0c01 0c01 0c01 0c01 0c01 0c01 1001 7224  ..............r$
+00000c00: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
+00000c10: 0000 0000 0400 0000 4000 0000 73a0 0000  ........@...s...
+00000c20: 0065 005a 0164 005a 0255 0064 015a 0369  .e.Z.d.Z.U.d.Z.i
+00000c30: 0064 0264 0393 0164 0464 0593 0164 0664  .d.d...d.d...d.d
+00000c40: 0793 0164 0864 0993 0164 0a64 0b93 0164  ...d.d...d.d...d
+00000c50: 0c64 0d93 0164 0e64 0f93 0164 1064 0f93  .d...d.d...d.d..
+00000c60: 0164 1164 1293 0164 1364 1493 0164 1564  .d.d...d.d...d.d
+00000c70: 1493 0164 1664 1493 0164 1764 1493 0164  ...d.d...d.d...d
+00000c80: 1864 1993 0164 1a64 0f93 0164 1b64 1c93  .d...d.d...d.d..
+00000c90: 0164 1d64 1e93 015a 0464 1f5a 0565 0665  .d.d...Z.d.Z.e.e
+00000ca0: 0765 0865 0966 0219 0019 0065 0a64 203c  .e.e.f.....e.d <
+00000cb0: 0064 215a 0b65 0965 0a64 223c 0064 1f53  .d!Z.e.e.d"<.d.S
+00000cc0: 0029 23da 1758 6762 6f6f 7374 4669 6e61  .)#..XgboostFina
+00000cd0: 6c50 6172 616d 436f 6e66 6967 7a1e 4465  lParamConfigz.De
+00000ce0: 6669 6e65 2066 696e 616c 2068 7970 6572  fine final hyper
+00000cf0: 2070 6172 616d 6574 6572 732e da09 6f62   parameters...ob
+00000d00: 6a65 6374 6976 6572 4400 0000 da0b 6576  jectiverD.....ev
+00000d10: 616c 5f6d 6574 7269 6372 4600 0000 da07  al_metricrF.....
+00000d20: 7665 7262 6f73 6572 0100 0000 da0b 7472  verboser......tr
+00000d30: 6565 5f6d 6574 686f 64da 0565 7861 6374  ee_method..exact
+00000d40: da09 6e75 6d5f 636c 6173 7372 2500 0000  ..num_classr%...
+00000d50: da09 6d61 785f 6465 7074 6872 2700 0000  ..max_depthr'...
+00000d60: da05 616c 7068 6172 3d00 0000 da06 6c61  ..alphar=.....la
+00000d70: 6d62 6461 da0a 6e75 6d5f 6c65 6176 6573  mbda..num_leaves
+00000d80: e910 0000 00da 0973 7562 7361 6d70 6c65  .......subsample
+00000d90: 7218 0000 00da 1063 6f6c 7361 6d70 6c65  r......colsample
+00000da0: 5f62 7974 7265 65da 1163 6f6c 7361 6d70  _bytree..colsamp
+00000db0: 6c65 5f62 796c 6576 656c da10 636f 6c73  le_bylevel..cols
+00000dc0: 616d 706c 655f 6279 6e6f 6465 da11 6d69  ample_bynode..mi
+00000dd0: 6e5f 6368 696c 645f 7361 6d70 6c65 7372  n_child_samplesr
+00000de0: 0f00 0000 723e 0000 00da 0573 7465 7073  ....r>.....steps
+00000df0: 723b 0000 00da 116e 756d 5f70 6172 616c  r;.....num_paral
+00000e00: 6c65 6c5f 7472 6565 7212 0000 004e da0d  lel_treer....N..
+00000e10: 7361 6d70 6c65 5f77 6569 6768 7467 0000  sample_weightg..
+00000e20: 0000 0000 e03f da18 636c 6173 7369 6669  .....?..classifi
+00000e30: 6361 7469 6f6e 5f74 6872 6573 686f 6c64  cation_threshold
+00000e40: 290c 7206 0000 0072 0700 0000 7208 0000  ).r....r....r...
+00000e50: 0072 1f00 0000 da06 7061 7261 6d73 725c  .r......paramsr\
+00000e60: 0000 0072 0300 0000 7202 0000 0072 4800  ...r....r....rH.
+00000e70: 0000 7223 0000 0072 2100 0000 725d 0000  ..r#...r!...r]..
+00000e80: 0072 0900 0000 7209 0000 0072 0900 0000  .r....r....r....
+00000e90: 720a 0000 0072 4900 0000 4700 0000 734e  r....rI...G...sN
+00000ea0: 0000 000a 0004 0202 0204 0102 ff04 0202  ................
+00000eb0: fe04 0302 fd04 0402 fc04 0502 fb04 0602  ................
+00000ec0: fa04 0702 f904 0802 f804 0902 f704 0a02  ................
+00000ed0: f604 0b02 f504 0c02 f404 0d02 f304 0e02  ................
+00000ee0: f204 0f02 f104 1002 f004 1104 ef18 1310  ................
+00000ef0: 0172 4900 0000 4e29 0a72 1f00 0000 da06  .rI...N).r......
+00000f00: 7479 7069 6e67 7202 0000 0072 0300 0000  typingr....r....
+00000f10: 5a14 7079 6461 6e74 6963 2e64 6174 6163  Z.pydantic.datac
+00000f20: 6c61 7373 6573 7204 0000 0072 0500 0000  lassesr....r....
+00000f30: 720b 0000 0072 2400 0000 7249 0000 0072  r....r$...rI...r
+00000f40: 0900 0000 7209 0000 0072 0900 0000 720a  ....r....r....r.
+00000f50: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
+00000f60: 0073 1400 0000 0400 1007 0c02 0e03 0204  .s..............
+00000f70: 1001 0213 1001 0221 1401                 .......!..
```

### Comparing `bluecast-0.5/bluecast/config/__pycache__/training_config.cpython-38.pyc` & `bluecast-0.7/bluecast/config/__pycache__/training_config.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Thu Jun  8 04:28:32 2023 UTC, .py size: 2726 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 16% similar despite different names*

```diff
@@ -1,210 +1,226 @@
-00000000: 550d 0d0a 0000 0000 f058 8164 a60a 0000  U........X.d....
+00000000: 550d 0d0a 0000 0000 02a4 9d64 390b 0000  U..........d9...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 5a00 0000 6400  .....@...sZ...d.
+00000020: 0004 0000 0040 0000 0073 6800 0000 6400  .....@...sh...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 6d03 5a03  Z.d.d.l.m.Z.m.Z.
-00000040: 0100 6401 6403 6c04 6d05 5a05 0100 6505  ..d.d.l.m.Z...e.
-00000050: 4700 6404 6405 8400 6405 8302 8301 5a06  G.d.d...d.....Z.
-00000060: 6505 4700 6406 6407 8400 6407 8302 8301  e.G.d.d...d.....
-00000070: 5a07 6505 4700 6408 6409 8400 6409 8302  Z.e.G.d.d...d...
-00000080: 8301 5a08 640a 5300 290b 61dc 0100 0044  ..Z.d.S.).a....D
-00000090: 6566 696e 6520 7472 6169 6e69 6e67 2061  efine training a
-000000a0: 6e64 2063 6f6d 6d6f 6e20 636f 6e66 6967  nd common config
-000000b0: 7572 6174 696f 6e20 7061 7261 6d65 7465  uration paramete
-000000c0: 7273 2e0a 0a50 7964 616e 7469 6320 6461  rs...Pydantic da
-000000d0: 7461 636c 6173 7365 7320 6172 6520 7573  taclasses are us
-000000e0: 6564 2074 6f20 6465 6669 6e65 2074 6865  ed to define the
-000000f0: 2063 6f6e 6669 6775 7261 7469 6f6e 2070   configuration p
-00000100: 6172 616d 6574 6572 732e 2054 6869 7320  arameters. This 
-00000110: 616c 6c6f 7773 2066 6f72 2074 7970 6520  allows for type 
-00000120: 6368 6563 6b69 6e67 2061 6e64 2076 616c  checking and val
-00000130: 6964 6174 696f 6e20 6f66 0a74 6865 2063  idation of.the c
-00000140: 6f6e 6669 6775 7261 7469 6f6e 2070 6172  onfiguration par
-00000150: 616d 6574 6572 732e 2054 6865 2063 6f6e  ameters. The con
-00000160: 6669 6775 7261 7469 6f6e 2070 6172 616d  figuration param
-00000170: 6574 6572 7320 6172 6520 7573 6564 2069  eters are used i
-00000180: 6e20 7468 6520 7472 6169 6e69 6e67 2070  n the training p
-00000190: 6970 656c 696e 6520 616e 6420 696e 2074  ipeline and in t
-000001a0: 6865 2065 7661 6c75 6174 696f 6e0a 7069  he evaluation.pi
-000001b0: 7065 6c69 6e65 2e20 5079 6461 6e74 6963  peline. Pydantic
-000001c0: 2064 6174 6163 6c61 7373 6573 2061 7265   dataclasses are
-000001d0: 2075 7365 6420 746f 2061 6c6c 6f77 2075   used to allow u
-000001e0: 7365 7273 2061 2070 7974 686f 6e69 6320  sers a pythonic 
-000001f0: 7761 7920 746f 2064 6566 696e 6520 7468  way to define th
-00000200: 6520 636f 6e66 6967 7572 6174 696f 6e20  e configuration 
-00000210: 7061 7261 6d65 7465 7273 2e0a 4465 6661  parameters..Defa
-00000220: 756c 7420 636f 6e66 6967 7572 6174 696f  ult configuratio
-00000230: 6e73 2063 616e 2062 6520 6c6f 6164 6564  ns can be loaded
-00000240: 2c20 6164 6a75 7374 6564 2061 6e64 2070  , adjusted and p
-00000250: 6173 7365 6420 696e 746f 2074 6865 2062  assed into the b
-00000260: 6c75 6570 7269 6e74 732e 0ae9 0000 0000  lueprints.......
-00000270: 2902 da04 4469 6374 da08 4f70 7469 6f6e  )...Dict..Option
-00000280: 616c 2901 da09 6461 7461 636c 6173 7363  al)...dataclassc
-00000290: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000002a0: 0300 0000 4000 0000 7372 0000 0065 005a  ....@...sr...e.Z
-000002b0: 0164 005a 0255 0064 015a 0364 025a 0465  .d.Z.U.d.Z.d.Z.e
-000002c0: 0565 0664 033c 0064 045a 0765 0865 0664  .e.d.<.d.Z.e.e.d
-000002d0: 053c 0064 065a 0965 0565 0664 073c 0064  .<.d.Z.e.e.d.<.d
-000002e0: 085a 0a65 0565 0664 093c 0064 0a5a 0b65  .Z.e.e.d.<.d.Z.e
-000002f0: 0565 0664 0b3c 0064 025a 0c65 0565 0664  .e.d.<.d.Z.e.e.d
-00000300: 0c3c 0064 045a 0d65 0865 0664 0d3c 0064  .<.d.Z.e.e.d.<.d
-00000310: 045a 0e65 0865 0664 0e3c 0064 0f53 0029  .Z.e.e.d.<.d.S.)
-00000320: 10da 0e54 7261 696e 696e 6743 6f6e 6669  ...TrainingConfi
-00000330: 677a 2344 6566 696e 6520 6765 6e65 7261  gz#Define genera
-00000340: 6c20 7472 6169 6e69 6e67 2070 6172 616d  l training param
-00000350: 6574 6572 732e e90a 0000 00da 1367 6c6f  eters........glo
-00000360: 6261 6c5f 7261 6e64 6f6d 5f73 7461 7465  bal_random_state
-00000370: 54da 1773 6875 6666 6c65 5f64 7572 696e  T..shuffle_durin
-00000380: 675f 7472 6169 6e69 6e67 e964 0000 00da  g_training.d....
-00000390: 1c68 7970 6572 7061 7261 6d65 7465 725f  .hyperparameter_
-000003a0: 7475 6e69 6e67 5f72 6f75 6e64 7369 100e  tuning_roundsi..
-000003b0: 0000 da26 6879 7065 7270 6172 616d 6574  ...&hyperparamet
-000003c0: 6572 5f74 756e 696e 675f 6d61 785f 7275  er_tuning_max_ru
-000003d0: 6e74 696d 655f 7365 6373 e901 0000 00da  ntime_secs......
-000003e0: 1468 7970 6572 7475 6e69 6e67 5f63 765f  .hypertuning_cv_
-000003f0: 666f 6c64 73da 1565 6172 6c79 5f73 746f  folds..early_sto
-00000400: 7070 696e 675f 726f 756e 6473 da0e 6175  pping_rounds..au
-00000410: 746f 7475 6e65 5f6d 6f64 656c da15 6361  totune_model..ca
-00000420: 6c63 756c 6174 655f 7368 6170 5f76 616c  lculate_shap_val
-00000430: 7565 734e 290f da08 5f5f 6e61 6d65 5f5f  uesN)...__name__
-00000440: da0a 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f  ..__module__..__
-00000450: 7175 616c 6e61 6d65 5f5f da07 5f5f 646f  qualname__..__do
-00000460: 635f 5f72 0700 0000 da03 696e 74da 0f5f  c__r......int.._
-00000470: 5f61 6e6e 6f74 6174 696f 6e73 5f5f 7208  _annotations__r.
-00000480: 0000 00da 0462 6f6f 6c72 0a00 0000 720b  .....boolr....r.
-00000490: 0000 0072 0d00 0000 720e 0000 0072 0f00  ...r....r....r..
-000004a0: 0000 7210 0000 00a9 0072 1800 0000 7218  ..r......r....r.
-000004b0: 0000 00fa 452f 686f 6d65 2f74 686f 6d61  ....E/home/thoma
-000004c0: 732f 4964 6561 5072 6f6a 6563 7473 2f42  s/IdeaProjects/B
-000004d0: 6c75 6543 6173 742f 626c 7565 6361 7374  lueCast/bluecast
-000004e0: 2f63 6f6e 6669 672f 7472 6169 6e69 6e67  /config/training
-000004f0: 5f63 6f6e 6669 672e 7079 7205 0000 000d  _config.pyr.....
-00000500: 0000 0073 1200 0000 0a02 0402 0c01 0c01  ...s............
-00000510: 0c01 0c01 0c01 0c01 0c01 7205 0000 0063  ..........r....c
-00000520: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000530: 0300 0000 4000 0000 734a 0100 0065 005a  ....@...sJ...e.Z
-00000540: 0164 005a 0255 0064 015a 0364 025a 0465  .d.Z.U.d.Z.d.Z.e
-00000550: 0565 0664 033c 0064 045a 0765 0565 0664  .e.d.<.d.Z.e.e.d
-00000560: 053c 0064 065a 0865 0965 0664 073c 0064  .<.d.Z.e.e.d.<.d
-00000570: 085a 0a65 0965 0664 093c 0064 065a 0b65  .Z.e.e.d.<.d.Z.e
-00000580: 0965 0664 0a3c 0064 085a 0c65 0965 0664  .e.d.<.d.Z.e.e.d
-00000590: 0b3c 0064 025a 0d65 0565 0664 0c3c 0064  .<.d.Z.e.e.d.<.d
-000005a0: 0d5a 0e65 0565 0664 0e3c 0064 0f5a 0f65  .Z.e.e.d.<.d.Z.e
-000005b0: 0965 0664 103c 0064 065a 1065 0965 0664  .e.d.<.d.Z.e.e.d
-000005c0: 113c 0064 0f5a 1165 0965 0664 123c 0064  .<.d.Z.e.e.d.<.d
-000005d0: 065a 1265 0965 0664 133c 0064 0f5a 1365  .Z.e.e.d.<.d.Z.e
-000005e0: 0965 0664 143c 0064 065a 1465 0965 0664  .e.d.<.d.Z.e.e.d
-000005f0: 153c 0064 0f5a 1565 0965 0664 163c 0064  .<.d.Z.e.e.d.<.d
-00000600: 065a 1665 0965 0664 173c 0064 025a 1765  .Z.e.e.d.<.d.Z.e
-00000610: 0565 0664 183c 0064 195a 1865 0565 0664  .e.d.<.d.Z.e.e.d
-00000620: 1a3c 0064 1b5a 1965 0965 0664 1c3c 0064  .<.d.Z.e.e.d.<.d
-00000630: 025a 1a65 0565 0664 1d3c 0064 1e5a 1b65  .Z.e.e.d.<.d.Z.e
-00000640: 0565 0664 1f3c 0064 205a 1c65 0565 0664  .e.d.<.d Z.e.e.d
-00000650: 213c 0064 045a 1d65 0565 0664 223c 0064  !<.d.Z.e.e.d"<.d
-00000660: 235a 1e65 0565 0664 243c 0064 255a 1f65  #Z.e.e.d$<.d%Z.e
-00000670: 2065 0664 263c 0064 275a 2165 2065 0664   e.d&<.d'Z!e e.d
-00000680: 283c 0064 2953 0029 2ada 1758 6762 6f6f  (<.d)S.)*..Xgboo
-00000690: 7374 5475 6e65 5061 7261 6d73 436f 6e66  stTuneParamsConf
-000006a0: 6967 7a2a 4465 6669 6e65 2068 7970 6572  igz*Define hyper
-000006b0: 7061 7261 6d65 7465 7220 7475 6e69 6e67  parameter tuning
-000006c0: 2073 6561 7263 6820 7370 6163 652e e902   search space...
-000006d0: 0000 00da 0d6d 6178 5f64 6570 7468 5f6d  .....max_depth_m
-000006e0: 696e e903 0000 00da 0d6d 6178 5f64 6570  in.......max_dep
-000006f0: 7468 5f6d 6178 6700 0000 0000 00f0 3fda  th_maxg.......?.
-00000700: 0961 6c70 6861 5f6d 696e 6700 0000 0000  .alpha_ming.....
-00000710: 408f 40da 0961 6c70 6861 5f6d 6178 da0a  @.@..alpha_max..
-00000720: 6c61 6d62 6461 5f6d 696e da0a 6c61 6d62  lambda_min..lamb
-00000730: 6461 5f6d 6178 da0e 6e75 6d5f 6c65 6176  da_max..num_leav
-00000740: 6573 5f6d 696e e940 0000 00da 0e6e 756d  es_min.@.....num
-00000750: 5f6c 6561 7665 735f 6d61 7867 3333 3333  _leaves_maxg3333
-00000760: 3333 d33f da0e 7375 625f 7361 6d70 6c65  33.?..sub_sample
-00000770: 5f6d 696e da0e 7375 625f 7361 6d70 6c65  _min..sub_sample
-00000780: 5f6d 6178 da16 636f 6c5f 7361 6d70 6c65  _max..col_sample
-00000790: 5f62 795f 7472 6565 5f6d 696e da16 636f  _by_tree_min..co
-000007a0: 6c5f 7361 6d70 6c65 5f62 795f 7472 6565  l_sample_by_tree
-000007b0: 5f6d 6178 da17 636f 6c5f 7361 6d70 6c65  _max..col_sample
-000007c0: 5f62 795f 6c65 7665 6c5f 6d69 6eda 1763  _by_level_min..c
-000007d0: 6f6c 5f73 616d 706c 655f 6279 5f6c 6576  ol_sample_by_lev
-000007e0: 656c 5f6d 6178 da16 636f 6c5f 7361 6d70  el_max..col_samp
-000007f0: 6c65 5f62 795f 6e6f 6465 5f6d 696e da16  le_by_node_min..
-00000800: 636f 6c5f 7361 6d70 6c65 5f62 795f 6e6f  col_sample_by_no
-00000810: 6465 5f6d 6178 da15 6d69 6e5f 6368 696c  de_max..min_chil
-00000820: 645f 7361 6d70 6c65 735f 6d69 6ee9 e803  d_samples_min...
-00000830: 0000 da15 6d69 6e5f 6368 696c 645f 7361  ....min_child_sa
-00000840: 6d70 6c65 735f 6d61 78e7 9a99 9999 9999  mples_max.......
-00000850: b93f da03 6574 61da 0973 7465 7073 5f6d  .?..eta..steps_m
-00000860: 696e 6950 c300 00da 0973 7465 7073 5f6d  iniP.....steps_m
-00000870: 6178 720c 0000 00da 156e 756d 5f70 6172  axr......num_par
-00000880: 616c 6c65 6c5f 7472 6565 5f6d 696e da15  allel_tree_min..
-00000890: 6e75 6d5f 7061 7261 6c6c 656c 5f74 7265  num_parallel_tre
-000008a0: 655f 6d61 7872 0100 0000 da0f 6d6f 6465  e_maxr......mode
-000008b0: 6c5f 7665 7262 6f73 6974 79fa 0e6d 756c  l_verbosity..mul
-000008c0: 7469 3a73 6f66 7470 726f 62da 0f6d 6f64  ti:softprob..mod
-000008d0: 656c 5f6f 626a 6563 7469 7665 da08 6d6c  el_objective..ml
-000008e0: 6f67 6c6f 7373 da11 6d6f 6465 6c5f 6576  ogloss..model_ev
-000008f0: 616c 5f6d 6574 7269 634e 2922 7211 0000  al_metricN)"r...
-00000900: 0072 1200 0000 7213 0000 0072 1400 0000  .r....r....r....
-00000910: 721c 0000 0072 1500 0000 7216 0000 0072  r....r....r....r
-00000920: 1e00 0000 721f 0000 00da 0566 6c6f 6174  ....r......float
-00000930: 7220 0000 0072 2100 0000 7222 0000 0072  r ...r!...r"...r
-00000940: 2300 0000 7225 0000 0072 2600 0000 7227  #...r%...r&...r'
-00000950: 0000 0072 2800 0000 7229 0000 0072 2a00  ...r(...r)...r*.
-00000960: 0000 722b 0000 0072 2c00 0000 722d 0000  ..r+...r,...r-..
-00000970: 0072 2e00 0000 7230 0000 0072 3200 0000  .r....r0...r2...
-00000980: 7233 0000 0072 3400 0000 7235 0000 0072  r3...r4...r5...r
-00000990: 3600 0000 7237 0000 0072 3900 0000 da03  6...r7...r9.....
-000009a0: 7374 7272 3b00 0000 7218 0000 0072 1800  strr;...r....r..
-000009b0: 0000 7218 0000 0072 1900 0000 721a 0000  ..r....r....r...
-000009c0: 001b 0000 0073 3600 0000 0a02 0402 0c01  .....s6.........
-000009d0: 0c01 0c01 0c01 0c01 0c01 0c01 0c01 0c01  ................
-000009e0: 0c01 0c01 0c01 0c01 0c01 0c01 0c01 0c01  ................
-000009f0: 0c01 0c01 0c01 0c01 0c01 0c01 0c01 0c01  ................
-00000a00: 721a 0000 0063 0000 0000 0000 0000 0000  r....c..........
-00000a10: 0000 0000 0000 1200 0000 4000 0000 735e  ..........@...s^
-00000a20: 0000 0065 005a 0164 005a 0255 0064 015a  ...e.Z.d.Z.U.d.Z
-00000a30: 0364 0264 0364 0464 0564 0664 0764 0864  .d.d.d.d.d.d.d.d
-00000a40: 0864 0964 0a64 0a64 0a64 0a64 0b64 0864  .d.d.d.d.d.d.d.d
-00000a50: 0c64 0d64 0e9c 115a 0464 0f5a 0565 0665  .d.d...Z.d.Z.e.e
-00000a60: 0765 0865 0966 0219 0019 0065 0a64 103c  .e.e.f.....e.d.<
-00000a70: 0064 115a 0b65 0965 0a64 123c 0064 0f53  .d.Z.e.e.d.<.d.S
-00000a80: 0029 13da 1758 6762 6f6f 7374 4669 6e61  .)...XgboostFina
-00000a90: 6c50 6172 616d 436f 6e66 6967 7a1e 4465  lParamConfigz.De
-00000aa0: 6669 6e65 2066 696e 616c 2068 7970 6572  fine final hyper
-00000ab0: 2070 6172 616d 6574 6572 732e 7238 0000   parameters.r8..
-00000ac0: 0072 3a00 0000 7201 0000 00da 0565 7861  .r:...r......exa
-00000ad0: 6374 721b 0000 0072 1d00 0000 7231 0000  ctr....r....r1..
-00000ae0: 00e9 1000 0000 679a 9999 9999 99e9 3f72  ......g.......?r
-00000af0: 0900 0000 722f 0000 0072 0c00 0000 2911  ....r/...r....).
-00000b00: da09 6f62 6a65 6374 6976 65da 0b65 7661  ..objective..eva
-00000b10: 6c5f 6d65 7472 6963 da07 7665 7262 6f73  l_metric..verbos
-00000b20: 65da 0b74 7265 655f 6d65 7468 6f64 da09  e..tree_method..
-00000b30: 6e75 6d5f 636c 6173 73da 096d 6178 5f64  num_class..max_d
-00000b40: 6570 7468 da05 616c 7068 61da 066c 616d  epth..alpha..lam
-00000b50: 6264 61da 0a6e 756d 5f6c 6561 7665 73da  bda..num_leaves.
-00000b60: 0973 7562 7361 6d70 6c65 da10 636f 6c73  .subsample..cols
-00000b70: 616d 706c 655f 6279 7472 6565 da11 636f  ample_bytree..co
-00000b80: 6c73 616d 706c 655f 6279 6c65 7665 6cda  lsample_bylevel.
-00000b90: 1063 6f6c 7361 6d70 6c65 5f62 796e 6f64  .colsample_bynod
-00000ba0: 65da 116d 696e 5f63 6869 6c64 5f73 616d  e..min_child_sam
-00000bb0: 706c 6573 7232 0000 00da 0573 7465 7073  plesr2.....steps
-00000bc0: da11 6e75 6d5f 7061 7261 6c6c 656c 5f74  ..num_parallel_t
-00000bd0: 7265 654e da0d 7361 6d70 6c65 5f77 6569  reeN..sample_wei
-00000be0: 6768 7467 0000 0000 0000 e03f da18 636c  ghtg.......?..cl
-00000bf0: 6173 7369 6669 6361 7469 6f6e 5f74 6872  assification_thr
-00000c00: 6573 686f 6c64 290c 7211 0000 0072 1200  eshold).r....r..
-00000c10: 0000 7213 0000 0072 1400 0000 da06 7061  ..r....r......pa
-00000c20: 7261 6d73 7251 0000 0072 0300 0000 7202  ramsrQ...r....r.
-00000c30: 0000 0072 3d00 0000 723c 0000 0072 1600  ...r=...r<...r..
-00000c40: 0000 7252 0000 0072 1800 0000 7218 0000  ..rR...r....r...
-00000c50: 0072 1800 0000 7219 0000 0072 3e00 0000  .r....r....r>...
-00000c60: 3b00 0000 732a 0000 000a 0204 0302 0102  ;...s*..........
-00000c70: 0102 0102 0102 0102 0102 0102 0102 0102  ................
-00000c80: 0102 0102 0102 0102 0102 0102 0102 ef06  ................
-00000c90: 1318 0172 3e00 0000 4e29 0972 1400 0000  ...r>...N).r....
-00000ca0: da06 7479 7069 6e67 7202 0000 0072 0300  ..typingr....r..
-00000cb0: 0000 da14 7079 6461 6e74 6963 2e64 6174  ....pydantic.dat
-00000cc0: 6163 6c61 7373 6573 7204 0000 0072 0500  aclassesr....r..
-00000cd0: 0000 721a 0000 0072 3e00 0000 7218 0000  ..r....r>...r...
-00000ce0: 0072 1800 0000 7218 0000 0072 1900 0000  .r....r....r....
-00000cf0: da08 3c6d 6f64 756c 653e 0100 0000 7310  ..<module>....s.
-00000d00: 0000 0004 0710 020c 0302 0110 0d02 0110  ................
-00000d10: 1f02 01                                  ...
+00000040: 0100 6401 6403 6c04 6d05 5a05 0100 4700  ..d.d.l.m.Z...G.
+00000050: 6404 6405 8400 6405 8302 5a06 6505 4700  d.d...d...Z.e.G.
+00000060: 6406 6407 8400 6407 8302 8301 5a07 6505  d.d...d.....Z.e.
+00000070: 4700 6408 6409 8400 6409 8302 8301 5a08  G.d.d...d.....Z.
+00000080: 6505 4700 640a 640b 8400 640b 8302 8301  e.G.d.d...d.....
+00000090: 5a09 640c 5300 290d 61dc 0100 0044 6566  Z.d.S.).a....Def
+000000a0: 696e 6520 7472 6169 6e69 6e67 2061 6e64  ine training and
+000000b0: 2063 6f6d 6d6f 6e20 636f 6e66 6967 7572   common configur
+000000c0: 6174 696f 6e20 7061 7261 6d65 7465 7273  ation parameters
+000000d0: 2e0a 0a50 7964 616e 7469 6320 6461 7461  ...Pydantic data
+000000e0: 636c 6173 7365 7320 6172 6520 7573 6564  classes are used
+000000f0: 2074 6f20 6465 6669 6e65 2074 6865 2063   to define the c
+00000100: 6f6e 6669 6775 7261 7469 6f6e 2070 6172  onfiguration par
+00000110: 616d 6574 6572 732e 2054 6869 7320 616c  ameters. This al
+00000120: 6c6f 7773 2066 6f72 2074 7970 6520 6368  lows for type ch
+00000130: 6563 6b69 6e67 2061 6e64 2076 616c 6964  ecking and valid
+00000140: 6174 696f 6e20 6f66 0a74 6865 2063 6f6e  ation of.the con
+00000150: 6669 6775 7261 7469 6f6e 2070 6172 616d  figuration param
+00000160: 6574 6572 732e 2054 6865 2063 6f6e 6669  eters. The confi
+00000170: 6775 7261 7469 6f6e 2070 6172 616d 6574  guration paramet
+00000180: 6572 7320 6172 6520 7573 6564 2069 6e20  ers are used in 
+00000190: 7468 6520 7472 6169 6e69 6e67 2070 6970  the training pip
+000001a0: 656c 696e 6520 616e 6420 696e 2074 6865  eline and in the
+000001b0: 2065 7661 6c75 6174 696f 6e0a 7069 7065   evaluation.pipe
+000001c0: 6c69 6e65 2e20 5079 6461 6e74 6963 2064  line. Pydantic d
+000001d0: 6174 6163 6c61 7373 6573 2061 7265 2075  ataclasses are u
+000001e0: 7365 6420 746f 2061 6c6c 6f77 2075 7365  sed to allow use
+000001f0: 7273 2061 2070 7974 686f 6e69 6320 7761  rs a pythonic wa
+00000200: 7920 746f 2064 6566 696e 6520 7468 6520  y to define the 
+00000210: 636f 6e66 6967 7572 6174 696f 6e20 7061  configuration pa
+00000220: 7261 6d65 7465 7273 2e0a 4465 6661 756c  rameters..Defaul
+00000230: 7420 636f 6e66 6967 7572 6174 696f 6e73  t configurations
+00000240: 2063 616e 2062 6520 6c6f 6164 6564 2c20   can be loaded, 
+00000250: 6164 6a75 7374 6564 2061 6e64 2070 6173  adjusted and pas
+00000260: 7365 6420 696e 746f 2074 6865 2062 6c75  sed into the blu
+00000270: 6570 7269 6e74 732e 0ae9 0000 0000 2902  eprints.......).
+00000280: da04 4469 6374 da08 4f70 7469 6f6e 616c  ..Dict..Optional
+00000290: 2901 da09 6461 7461 636c 6173 7363 0000  )...dataclassc..
+000002a0: 0000 0000 0000 0000 0000 0000 0000 0100  ................
+000002b0: 0000 4000 0000 7310 0000 0065 005a 0164  ..@...s....e.Z.d
+000002c0: 005a 0264 015a 0364 0253 0029 03da 0643  .Z.d.Z.d.S.)...C
+000002d0: 6f6e 6669 6754 4e29 04da 085f 5f6e 616d  onfigTN)...__nam
+000002e0: 655f 5fda 0a5f 5f6d 6f64 756c 655f 5fda  e__..__module__.
+000002f0: 0c5f 5f71 7561 6c6e 616d 655f 5fda 1761  .__qualname__..a
+00000300: 7262 6974 7261 7279 5f74 7970 6573 5f61  rbitrary_types_a
+00000310: 6c6c 6f77 6564 a900 720a 0000 0072 0a00  llowed..r....r..
+00000320: 0000 fa45 2f68 6f6d 652f 7468 6f6d 6173  ...E/home/thomas
+00000330: 2f49 6465 6150 726f 6a65 6374 732f 426c  /IdeaProjects/Bl
+00000340: 7565 4361 7374 2f62 6c75 6563 6173 742f  ueCast/bluecast/
+00000350: 636f 6e66 6967 2f74 7261 696e 696e 675f  config/training_
+00000360: 636f 6e66 6967 2e70 7972 0500 0000 0d00  config.pyr......
+00000370: 0000 7302 0000 0008 0172 0500 0000 6300  ..s......r....c.
+00000380: 0000 0000 0000 0000 0000 0000 0000 0003  ................
+00000390: 0000 0040 0000 0073 ba00 0000 6500 5a01  ...@...s....e.Z.
+000003a0: 6400 5a02 5500 6401 5a03 6402 5a04 6505  d.Z.U.d.Z.d.Z.e.
+000003b0: 6506 6403 3c00 6404 5a07 6508 6506 6405  e.d.<.d.Z.e.e.d.
+000003c0: 3c00 6406 5a09 6505 6506 6407 3c00 6408  <.d.Z.e.e.d.<.d.
+000003d0: 5a0a 6505 6506 6409 3c00 640a 5a0b 6505  Z.e.e.d.<.d.Z.e.
+000003e0: 6506 640b 3c00 6402 5a0c 6505 6506 640c  e.d.<.d.Z.e.e.d.
+000003f0: 3c00 6404 5a0d 6508 6506 640d 3c00 640e  <.d.Z.e.e.d.<.d.
+00000400: 5a0e 6508 6506 640f 3c00 6404 5a0f 6508  Z.e.e.d.<.d.Z.e.
+00000410: 6506 6410 3c00 6411 5a10 6511 6506 6412  e.d.<.d.Z.e.e.d.
+00000420: 3c00 6404 5a12 6508 6506 6413 3c00 6404  <.d.Z.e.e.d.<.d.
+00000430: 5a13 6508 6506 6414 3c00 6415 5a14 6505  Z.e.e.d.<.d.Z.e.
+00000440: 6506 6416 3c00 640e 5a15 6508 6506 6417  e.d.<.d.Z.e.e.d.
+00000450: 3c00 6418 5300 2919 da0e 5472 6169 6e69  <.d.S.)...Traini
+00000460: 6e67 436f 6e66 6967 7a23 4465 6669 6e65  ngConfigz#Define
+00000470: 2067 656e 6572 616c 2074 7261 696e 696e   general trainin
+00000480: 6720 7061 7261 6d65 7465 7273 2ee9 0a00  g parameters....
+00000490: 0000 da13 676c 6f62 616c 5f72 616e 646f  ....global_rando
+000004a0: 6d5f 7374 6174 6554 da17 7368 7566 666c  m_stateT..shuffl
+000004b0: 655f 6475 7269 6e67 5f74 7261 696e 696e  e_during_trainin
+000004c0: 67e9 6400 0000 da1c 6879 7065 7270 6172  g.d.....hyperpar
+000004d0: 616d 6574 6572 5f74 756e 696e 675f 726f  ameter_tuning_ro
+000004e0: 756e 6473 6910 0e00 00da 2668 7970 6572  undsi.....&hyper
+000004f0: 7061 7261 6d65 7465 725f 7475 6e69 6e67  parameter_tuning
+00000500: 5f6d 6178 5f72 756e 7469 6d65 5f73 6563  _max_runtime_sec
+00000510: 73e9 0100 0000 da14 6879 7065 7274 756e  s.......hypertun
+00000520: 696e 675f 6376 5f66 6f6c 6473 da15 6561  ing_cv_folds..ea
+00000530: 726c 795f 7374 6f70 7069 6e67 5f72 6f75  rly_stopping_rou
+00000540: 6e64 73da 0e61 7574 6f74 756e 655f 6d6f  nds..autotune_mo
+00000550: 6465 6c46 da18 656e 6162 6c65 5f66 6561  delF..enable_fea
+00000560: 7475 7265 5f73 656c 6563 7469 6f6e da15  ture_selection..
+00000570: 6361 6c63 756c 6174 655f 7368 6170 5f76  calculate_shap_v
+00000580: 616c 7565 73e7 9a99 9999 9999 e93f da0a  alues........?..
+00000590: 7472 6169 6e5f 7369 7a65 da14 7472 6169  train_size..trai
+000005a0: 6e5f 7370 6c69 745f 7374 7261 7469 6679  n_split_stratify
+000005b0: da1d 7573 655f 6675 6c6c 5f64 6174 615f  ..use_full_data_
+000005c0: 666f 725f 6669 6e61 6c5f 6d6f 6465 6ce9  for_final_model.
+000005d0: 0500 0000 da16 6d69 6e5f 6665 6174 7572  ......min_featur
+000005e0: 6573 5f74 6f5f 7365 6c65 6374 da1d 6361  es_to_select..ca
+000005f0: 745f 656e 636f 6469 6e67 5f76 6961 5f6d  t_encoding_via_m
+00000600: 6c5f 616c 676f 7269 7468 6d4e 2916 7206  l_algorithmN).r.
+00000610: 0000 0072 0700 0000 7208 0000 00da 075f  ...r....r......_
+00000620: 5f64 6f63 5f5f 720e 0000 00da 0369 6e74  _doc__r......int
+00000630: da0f 5f5f 616e 6e6f 7461 7469 6f6e 735f  ..__annotations_
+00000640: 5f72 0f00 0000 da04 626f 6f6c 7211 0000  _r......boolr...
+00000650: 0072 1200 0000 7214 0000 0072 1500 0000  .r....r....r....
+00000660: 7216 0000 0072 1700 0000 7218 0000 0072  r....r....r....r
+00000670: 1a00 0000 da05 666c 6f61 7472 1b00 0000  ......floatr....
+00000680: 721c 0000 0072 1e00 0000 721f 0000 0072  r....r....r....r
+00000690: 0a00 0000 720a 0000 0072 0a00 0000 720b  ....r....r....r.
+000006a0: 0000 0072 0c00 0000 1100 0000 731e 0000  ...r........s...
+000006b0: 000a 0204 020c 010c 010c 010c 010c 010c  ................
+000006c0: 010c 010c 010c 010c 010c 010c 010c 0172  ...............r
+000006d0: 0c00 0000 6300 0000 0000 0000 0000 0000  ....c...........
+000006e0: 0000 0000 0003 0000 0040 0000 0073 1a01  .........@...s..
+000006f0: 0000 6500 5a01 6400 5a02 5500 6401 5a03  ..e.Z.d.Z.U.d.Z.
+00000700: 6402 5a04 6505 6506 6403 3c00 6404 5a07  d.Z.e.e.d.<.d.Z.
+00000710: 6505 6506 6405 3c00 6406 5a08 6509 6506  e.e.d.<.d.Z.e.e.
+00000720: 6407 3c00 6408 5a0a 6509 6506 6409 3c00  d.<.d.Z.e.e.d.<.
+00000730: 6406 5a0b 6509 6506 640a 3c00 6408 5a0c  d.Z.e.e.d.<.d.Z.
+00000740: 6509 6506 640b 3c00 6402 5a0d 6505 6506  e.e.d.<.d.Z.e.e.
+00000750: 640c 3c00 640d 5a0e 6505 6506 640e 3c00  d.<.d.Z.e.e.d.<.
+00000760: 640f 5a0f 6509 6506 6410 3c00 6411 5a10  d.Z.e.e.d.<.d.Z.
+00000770: 6509 6506 6412 3c00 640f 5a11 6509 6506  e.e.d.<.d.Z.e.e.
+00000780: 6413 3c00 6411 5a12 6509 6506 6414 3c00  d.<.d.Z.e.e.d.<.
+00000790: 640f 5a13 6509 6506 6415 3c00 6411 5a14  d.Z.e.e.d.<.d.Z.
+000007a0: 6509 6506 6416 3c00 6406 5a15 6509 6506  e.e.d.<.d.Z.e.e.
+000007b0: 6417 3c00 6408 5a16 6509 6506 6418 3c00  d.<.d.Z.e.e.d.<.
+000007c0: 6419 5a17 6509 6506 641a 3c00 6402 5a18  d.Z.e.e.d.<.d.Z.
+000007d0: 6505 6506 641b 3c00 641c 5a19 6505 6506  e.e.d.<.d.Z.e.e.
+000007e0: 641d 3c00 641e 5a1a 6505 6506 641f 3c00  d.<.d.Z.e.e.d.<.
+000007f0: 6420 5a1b 651c 6506 6421 3c00 6422 5a1d  d Z.e.e.d!<.d"Z.
+00000800: 651c 6506 6423 3c00 6424 5300 2925 da17  e.e.d#<.d$S.)%..
+00000810: 5867 626f 6f73 7454 756e 6550 6172 616d  XgboostTuneParam
+00000820: 7343 6f6e 6669 677a 2a44 6566 696e 6520  sConfigz*Define 
+00000830: 6879 7065 7270 6172 616d 6574 6572 2074  hyperparameter t
+00000840: 756e 696e 6720 7365 6172 6368 2073 7061  uning search spa
+00000850: 6365 2ee9 0200 0000 da0d 6d61 785f 6465  ce........max_de
+00000860: 7074 685f 6d69 6ee9 0600 0000 da0d 6d61  pth_min.......ma
+00000870: 785f 6465 7074 685f 6d61 7867 0000 0000  x_depth_maxg....
+00000880: 0000 0000 da09 616c 7068 615f 6d69 6e67  ......alpha_ming
+00000890: 0000 0000 0000 2440 da09 616c 7068 615f  ......$@..alpha_
+000008a0: 6d61 78da 0a6c 616d 6264 615f 6d69 6eda  max..lambda_min.
+000008b0: 0a6c 616d 6264 615f 6d61 78da 0e6e 756d  .lambda_max..num
+000008c0: 5f6c 6561 7665 735f 6d69 6ee9 4000 0000  _leaves_min.@...
+000008d0: da0e 6e75 6d5f 6c65 6176 6573 5f6d 6178  ..num_leaves_max
+000008e0: 6733 3333 3333 33d3 3fda 0e73 7562 5f73  g333333.?..sub_s
+000008f0: 616d 706c 655f 6d69 6e67 0000 0000 0000  ample_ming......
+00000900: f03f da0e 7375 625f 7361 6d70 6c65 5f6d  .?..sub_sample_m
+00000910: 6178 da16 636f 6c5f 7361 6d70 6c65 5f62  ax..col_sample_b
+00000920: 795f 7472 6565 5f6d 696e da16 636f 6c5f  y_tree_min..col_
+00000930: 7361 6d70 6c65 5f62 795f 7472 6565 5f6d  sample_by_tree_m
+00000940: 6178 da17 636f 6c5f 7361 6d70 6c65 5f62  ax..col_sample_b
+00000950: 795f 6c65 7665 6c5f 6d69 6eda 1763 6f6c  y_level_min..col
+00000960: 5f73 616d 706c 655f 6279 5f6c 6576 656c  _sample_by_level
+00000970: 5f6d 6178 da14 6d69 6e5f 6368 696c 645f  _max..min_child_
+00000980: 7765 6967 6874 5f6d 696e da14 6d69 6e5f  weight_min..min_
+00000990: 6368 696c 645f 7765 6967 6874 5f6d 6178  child_weight_max
+000009a0: e79a 9999 9999 99b9 3fda 0365 7461 da09  ........?..eta..
+000009b0: 7374 6570 735f 6d69 6e69 50c3 0000 da09  steps_miniP.....
+000009c0: 7374 6570 735f 6d61 7872 0100 0000 da0f  steps_maxr......
+000009d0: 6d6f 6465 6c5f 7665 7262 6f73 6974 79fa  model_verbosity.
+000009e0: 0e6d 756c 7469 3a73 6f66 7470 726f 62da  .multi:softprob.
+000009f0: 0f6d 6f64 656c 5f6f 626a 6563 7469 7665  .model_objective
+00000a00: da08 6d6c 6f67 6c6f 7373 da11 6d6f 6465  ..mlogloss..mode
+00000a10: 6c5f 6576 616c 5f6d 6574 7269 634e 291e  l_eval_metricN).
+00000a20: 7206 0000 0072 0700 0000 7208 0000 0072  r....r....r....r
+00000a30: 2000 0000 7227 0000 0072 2100 0000 7222   ...r'...r!...r"
+00000a40: 0000 0072 2900 0000 722a 0000 0072 2400  ...r)...r*...r$.
+00000a50: 0000 722b 0000 0072 2c00 0000 722d 0000  ..r+...r,...r-..
+00000a60: 0072 2e00 0000 7230 0000 0072 3100 0000  .r....r0...r1...
+00000a70: 7232 0000 0072 3300 0000 7234 0000 0072  r2...r3...r4...r
+00000a80: 3500 0000 7236 0000 0072 3700 0000 7238  5...r6...r7...r8
+00000a90: 0000 0072 3a00 0000 723b 0000 0072 3c00  ...r:...r;...r<.
+00000aa0: 0000 723d 0000 0072 3f00 0000 da03 7374  ..r=...r?.....st
+00000ab0: 7272 4100 0000 720a 0000 0072 0a00 0000  rrA...r....r....
+00000ac0: 720a 0000 0072 0b00 0000 7225 0000 0025  r....r....r%...%
+00000ad0: 0000 0073 2e00 0000 0a02 0402 0c01 0c01  ...s............
+00000ae0: 0c01 0c01 0c01 0c01 0c01 0c01 0c01 0c01  ................
+00000af0: 0c01 0c01 0c01 0c01 0c01 0c01 0c01 0c01  ................
+00000b00: 0c01 0c01 0c01 7225 0000 0063 0000 0000  ......r%...c....
+00000b10: 0000 0000 0000 0000 0000 0000 1200 0000  ................
+00000b20: 4000 0000 735e 0000 0065 005a 0164 005a  @...s^...e.Z.d.Z
+00000b30: 0255 0064 015a 0364 0264 0364 0464 0564  .U.d.Z.d.d.d.d.d
+00000b40: 0664 0764 0864 0864 0964 0a64 0a64 0a64  .d.d.d.d.d.d.d.d
+00000b50: 0a64 0b64 0864 0c64 0d64 0e9c 115a 0464  .d.d.d.d.d...Z.d
+00000b60: 0f5a 0565 0665 0765 0865 0966 0219 0019  .Z.e.e.e.e.f....
+00000b70: 0065 0a64 103c 0064 115a 0b65 0965 0a64  .e.d.<.d.Z.e.e.d
+00000b80: 123c 0064 0f53 0029 13da 1758 6762 6f6f  .<.d.S.)...Xgboo
+00000b90: 7374 4669 6e61 6c50 6172 616d 436f 6e66  stFinalParamConf
+00000ba0: 6967 7a1e 4465 6669 6e65 2066 696e 616c  igz.Define final
+00000bb0: 2068 7970 6572 2070 6172 616d 6574 6572   hyper parameter
+00000bc0: 732e 723e 0000 0072 4000 0000 7201 0000  s.r>...r@...r...
+00000bd0: 00da 0565 7861 6374 7226 0000 00e9 0300  ...exactr&......
+00000be0: 0000 7239 0000 00e9 1000 0000 7219 0000  ..r9........r...
+00000bf0: 0072 1000 0000 69e8 0300 0072 1300 0000  .r....i....r....
+00000c00: 2911 da09 6f62 6a65 6374 6976 65da 0b65  )...objective..e
+00000c10: 7661 6c5f 6d65 7472 6963 da07 7665 7262  val_metric..verb
+00000c20: 6f73 65da 0b74 7265 655f 6d65 7468 6f64  ose..tree_method
+00000c30: da09 6e75 6d5f 636c 6173 73da 096d 6178  ..num_class..max
+00000c40: 5f64 6570 7468 da05 616c 7068 61da 066c  _depth..alpha..l
+00000c50: 616d 6264 61da 0a6e 756d 5f6c 6561 7665  ambda..num_leave
+00000c60: 73da 0973 7562 7361 6d70 6c65 da10 636f  s..subsample..co
+00000c70: 6c73 616d 706c 655f 6279 7472 6565 da11  lsample_bytree..
+00000c80: 636f 6c73 616d 706c 655f 6279 6c65 7665  colsample_byleve
+00000c90: 6cda 1063 6f6c 7361 6d70 6c65 5f62 796e  l..colsample_byn
+00000ca0: 6f64 65da 116d 696e 5f63 6869 6c64 5f73  ode..min_child_s
+00000cb0: 616d 706c 6573 723a 0000 00da 0573 7465  amplesr:.....ste
+00000cc0: 7073 da11 6e75 6d5f 7061 7261 6c6c 656c  ps..num_parallel
+00000cd0: 5f74 7265 654e da0d 7361 6d70 6c65 5f77  _treeN..sample_w
+00000ce0: 6569 6768 7467 0000 0000 0000 e03f da18  eightg.......?..
+00000cf0: 636c 6173 7369 6669 6361 7469 6f6e 5f74  classification_t
+00000d00: 6872 6573 686f 6c64 290c 7206 0000 0072  hreshold).r....r
+00000d10: 0700 0000 7208 0000 0072 2000 0000 da06  ....r....r .....
+00000d20: 7061 7261 6d73 7257 0000 0072 0300 0000  paramsrW...r....
+00000d30: 7202 0000 0072 4200 0000 7224 0000 0072  r....rB...r$...r
+00000d40: 2200 0000 7258 0000 0072 0a00 0000 720a  "...rX...r....r.
+00000d50: 0000 0072 0a00 0000 720b 0000 0072 4300  ...r....r....rC.
+00000d60: 0000 4100 0000 732a 0000 000a 0204 0302  ..A...s*........
+00000d70: 0102 0102 0102 0102 0102 0102 0102 0102  ................
+00000d80: 0102 0102 0102 0102 0102 0102 0102 0102  ................
+00000d90: ef06 1318 0172 4300 0000 4e29 0a72 2000  .....rC...N).r .
+00000da0: 0000 da06 7479 7069 6e67 7202 0000 0072  ....typingr....r
+00000db0: 0300 0000 da14 7079 6461 6e74 6963 2e64  ......pydantic.d
+00000dc0: 6174 6163 6c61 7373 6573 7204 0000 0072  ataclassesr....r
+00000dd0: 0500 0000 720c 0000 0072 2500 0000 7243  ....r....r%...rC
+00000de0: 0000 0072 0a00 0000 720a 0000 0072 0a00  ...r....r....r..
+00000df0: 0000 720b 0000 00da 083c 6d6f 6475 6c65  ..r......<module
+00000e00: 3e01 0000 0073 1200 0000 0407 1002 0c03  >....s..........
+00000e10: 0e04 0201 1013 0201 101b 0201            ............
```

### Comparing `bluecast-0.5/bluecast/config/training_config.py` & `bluecast-0.7/bluecast/config/training_config.py`

 * *Files 12% similar despite different names*

```diff
@@ -27,43 +27,40 @@
     autotune_model: bool = True
     enable_feature_selection: bool = False
     calculate_shap_values: bool = True
     train_size: float = 0.8
     train_split_stratify: bool = True
     use_full_data_for_final_model: bool = True
     min_features_to_select: int = 5
+    cat_encoding_via_ml_algorithm: bool = False
 
 
 @dataclass
 class XgboostTuneParamsConfig:
     """Define hyperparameter tuning search space."""
 
     max_depth_min: int = 2
-    max_depth_max: int = 3
-    alpha_min: float = 1.0
-    alpha_max: float = 1e3
-    lambda_min: float = 1.0
-    lambda_max: float = 1e3
+    max_depth_max: int = 6
+    alpha_min: float = 0.0
+    alpha_max: float = 10.0
+    lambda_min: float = 0.0
+    lambda_max: float = 10.0
     num_leaves_min: int = 2
     num_leaves_max: int = 64
     sub_sample_min: float = 0.3
     sub_sample_max: float = 1.0
     col_sample_by_tree_min: float = 0.3
     col_sample_by_tree_max: float = 1.0
     col_sample_by_level_min: float = 0.3
     col_sample_by_level_max: float = 1.0
-    col_sample_by_node_min: float = 0.3
-    col_sample_by_node_max: float = 1.0
-    min_child_samples_min: int = 2
-    min_child_samples_max: int = 1000
+    min_child_weight_min: float = 0.0
+    min_child_weight_max: float = 10.0
     eta: float = 0.1
     steps_min: int = 2
     steps_max: int = 50000
-    num_parallel_tree_min: int = 1
-    num_parallel_tree_max: int = 3
     model_verbosity: int = 0
     model_objective: str = "multi:softprob"
     model_eval_metric: str = "mlogloss"
 
 
 @dataclass
 class XgboostFinalParamConfig:
```

### Comparing `bluecast-0.5/bluecast/evaluation/__pycache__/eval_metrics.cpython-310.pyc` & `bluecast-0.7/bluecast/evaluation/__pycache__/eval_metrics.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun Jun 25 05:34:02 2023 UTC, .py size: 2212 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 cad1 9764 a408 0000  o..........d....
+00000000: 6f0d 0d0a 0000 0000 c915 9c64 a408 0000  o..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 000a 0000 0040 0000 0073 7c00 0000 6400  .....@...s|...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 6d03 5a03  Z.d.d.l.m.Z.m.Z.
 00000040: 0100 6401 6403 6c04 5a05 6401 6404 6c06  ..d.d.l.Z.d.d.l.
 00000050: 6d07 5a07 6d08 5a08 6d09 5a09 6d0a 5a0a  m.Z.m.Z.m.Z.m.Z.
 00000060: 6d0b 5a0b 6d0c 5a0c 0100 6401 6405 6c0d  m.Z.m.Z...d.d.l.
 00000070: 6d0e 5a0e 0100 6406 6407 8400 5a0f 6408  m.Z...d.d...Z.d.
```

### Comparing `bluecast-0.5/bluecast/evaluation/__pycache__/shap_values.cpython-310.pyc` & `bluecast-0.7/bluecast/evaluation/__pycache__/shap_values.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.5/bluecast/evaluation/__pycache__/shap_values.cpython-38.pyc` & `bluecast-0.7/bluecast/evaluation/__pycache__/shap_values.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Thu Jun  8 04:28:32 2023 UTC, .py size: 1486 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 13% similar despite different names*

```diff
@@ -1,88 +1,83 @@
-00000000: 550d 0d0a 0000 0000 f058 8164 ce05 0000  U........X.d....
+00000000: 550d 0d0a 0000 0000 6d1d 8364 6d05 0000  U.......m..dm...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0005 0000 0040 0000 0073 4400 0000 6400  .....@...sD...d.
-00000030: 5a00 6401 6402 6c01 6d02 5a03 0100 6401  Z.d.d.l.m.Z...d.
-00000040: 6402 6c04 5a05 6401 6402 6c06 5a07 6401  d.l.Z.d.d.l.Z.d.
-00000050: 6402 6c08 5a08 6407 6507 6a09 650a 6505  d.l.Z.d.e.j.e.e.
-00000060: 6a0b 6404 9c03 6405 6406 8405 5a0c 6402  j.d...d.d...Z.d.
-00000070: 5300 2908 7ab2 4d6f 6475 6c65 2074 6f20  S.).z.Module to 
-00000080: 6361 6c63 756c 6174 6520 5348 4150 2076  calculate SHAP v
-00000090: 616c 7565 7320 666f 7220 6120 7472 6169  alues for a trai
-000000a0: 6e65 6420 4d4c 206d 6f64 656c 2e0a 0a54  ned ML model...T
-000000b0: 6865 2069 6d70 6c65 6d65 6e74 6174 696f  he implementatio
-000000c0: 6e20 6973 2066 6c65 7869 626c 6520 616e  n is flexible an
-000000d0: 6420 6361 6e20 6265 2075 7365 6420 666f  d can be used fo
-000000e0: 7220 616c 6d6f 7374 2061 6e79 204d 4c20  r almost any ML 
-000000f0: 6d6f 6465 6c2e 2054 6865 2069 6d70 6c65  model. The imple
-00000100: 6d65 6e74 6174 696f 6e20 6973 2062 6173  mentation is bas
-00000110: 6564 206f 6e20 7468 6520 5348 4150 206c  ed on the SHAP l
-00000120: 6962 7261 7279 2e0a e900 0000 004e da04  ibrary.......N..
-00000130: 7472 6565 2903 da02 6466 da09 6578 706c  tree)...df..expl
-00000140: 6169 6e65 72da 0672 6574 7572 6e63 0300  ainer..returnc..
-00000150: 0000 0000 0000 0000 0000 0600 0000 0800  ................
-00000160: 0000 4300 0000 73c2 0000 0074 00a0 01a1  ..C...s....t....
-00000170: 0001 007c 0264 016b 0272 8a7a 3274 00a0  ...|.d.k.r.z2t..
-00000180: 027c 00a1 017d 037c 03a0 037c 01a1 017d  .|...}.|...|...}
-00000190: 0474 006a 047c 047c 0164 0264 0364 048d  .t.j.|.|.d.d.d..
-000001a0: 0401 0074 05a0 06a1 0001 0057 0071 be04  ...t.......W.q..
-000001b0: 0074 076b 0a72 8601 0001 0001 0074 00a0  .t.k.r.......t..
-000001c0: 087c 006a 097c 01a1 027d 057c 05a0 037c  .|.j.|...}.|...|
-000001d0: 01a1 017d 0474 006a 047c 047c 0164 0364  ...}.t.j.|.|.d.d
-000001e0: 058d 0301 0074 05a0 06a1 0001 0059 0071  .....t.......Y.q
-000001f0: be58 006e 3474 00a0 087c 006a 097c 01a1  .X.n4t...|.j.|..
-00000200: 027d 057c 05a0 037c 01a1 017d 0474 006a  .}.|...|...}.t.j
-00000210: 047c 047c 0164 0364 058d 0301 0074 05a0  .|.|.d.d.....t..
-00000220: 06a1 0001 007c 0453 0064 0653 0029 0761  .....|.S.d.S.).a
-00000230: 3d01 0000 0a20 2020 2053 6565 2065 7870  =....    See exp
-00000240: 6c61 6e61 7469 6f6e 7320 756e 6465 723a  lanations under:
-00000250: 0a20 2020 2068 7474 7073 3a2f 2f6d 6564  .    https://med
-00000260: 6975 6d2e 636f 6d2f 7261 7069 6473 2d61  ium.com/rapids-a
-00000270: 692f 6770 752d 6163 6365 6c65 7261 7465  i/gpu-accelerate
-00000280: 642d 7368 6170 2d76 616c 7565 732d 7769  d-shap-values-wi
-00000290: 7468 2d78 6762 6f6f 7374 2d31 2d33 2d61  th-xgboost-1-3-a
-000002a0: 6e64 2d72 6170 6964 732d 3538 3766 6164  nd-rapids-587fad
-000002b0: 3638 3232 0a20 2020 203a 7061 7261 6d20  6822.    :param 
-000002c0: 6d6f 6465 6c3a 2054 7261 696e 6564 204d  model: Trained M
-000002d0: 4c20 6d6f 6465 6c0a 2020 2020 3a70 6172  L model.    :par
-000002e0: 616d 2064 663a 2054 6573 7420 6461 7461  am df: Test data
-000002f0: 2074 6f20 7072 6564 6963 7420 6f6e 2e0a   to predict on..
-00000300: 2020 2020 3a70 6172 616d 2065 7870 6c61      :param expla
-00000310: 696e 6572 3a20 5365 7420 2274 7265 6522  iner: Set "tree"
-00000320: 2066 6f72 2054 7265 6545 7870 6c61 696e   for TreeExplain
-00000330: 6572 2e20 4f74 6865 7277 6973 6520 7573  er. Otherwise us
-00000340: 6573 204b 6572 6e65 6c45 7870 6c61 696e  es KernelExplain
-00000350: 6572 2e0a 2020 2020 3a72 6574 7572 6e3a  er..    :return:
-00000360: 2053 6861 7020 7661 6c75 6573 0a20 2020   Shap values.   
-00000370: 2072 0200 0000 da03 6261 7254 2902 da09   r......barT)...
-00000380: 706c 6f74 5f74 7970 65da 0473 686f 7729  plot_type..show)
-00000390: 0172 0800 0000 4e29 0ada 0473 6861 70da  .r....N)...shap.
-000003a0: 0669 6e69 746a 73da 0d54 7265 6545 7870  .initjs..TreeExp
-000003b0: 6c61 696e 6572 da0b 7368 6170 5f76 616c  lainer..shap_val
-000003c0: 7565 73da 0c73 756d 6d61 7279 5f70 6c6f  ues..summary_plo
-000003d0: 74da 0370 6c74 7208 0000 00da 0e41 7373  t..pltr......Ass
-000003e0: 6572 7469 6f6e 4572 726f 72da 0f4b 6572  ertionError..Ker
-000003f0: 6e65 6c45 7870 6c61 696e 6572 da07 7072  nelExplainer..pr
-00000400: 6564 6963 7429 06da 056d 6f64 656c 7203  edict)...modelr.
-00000410: 0000 0072 0400 0000 5a0e 7472 6565 5f65  ...r....Z.tree_e
-00000420: 7870 6c61 696e 6572 da11 6d6f 6465 6c5f  xplainer..model_
-00000430: 7368 6170 5f76 616c 7565 73da 146d 6f64  shap_values..mod
-00000440: 656c 5f73 6861 705f 6578 706c 6169 6e65  el_shap_explaine
-00000450: 72a9 0072 1500 0000 fa45 2f68 6f6d 652f  r..r.....E/home/
-00000460: 7468 6f6d 6173 2f49 6465 6150 726f 6a65  thomas/IdeaProje
-00000470: 6374 732f 426c 7565 4361 7374 2f62 6c75  cts/BlueCast/blu
-00000480: 6563 6173 742f 6576 616c 7561 7469 6f6e  ecast/evaluation
-00000490: 2f73 6861 705f 7661 6c75 6573 2e70 79da  /shap_values.py.
-000004a0: 1173 6861 705f 6578 706c 616e 6174 696f  .shap_explanatio
-000004b0: 6e73 0b00 0000 7322 0000 0000 0908 0108  ns....s"........
-000004c0: 0102 010a 010a 0112 010c 010e 010e 010a  ................
-000004d0: 0110 0110 020e 010a 0110 0108 0172 1700  .............r..
-000004e0: 0000 2901 7202 0000 0029 0dda 075f 5f64  ..).r....)...__d
-000004f0: 6f63 5f5f da11 6d61 7470 6c6f 746c 6962  oc__..matplotlib
-00000500: 2e70 7970 6c6f 74da 0670 7970 6c6f 7472  .pyplot..pyplotr
-00000510: 0e00 0000 da05 6e75 6d70 79da 026e 70da  ......numpy..np.
-00000520: 0670 616e 6461 73da 0270 6472 0900 0000  .pandas..pdr....
-00000530: da09 4461 7461 4672 616d 65da 0373 7472  ..DataFrame..str
-00000540: da07 6e64 6172 7261 7972 1700 0000 7215  ..ndarrayr....r.
-00000550: 0000 0072 1500 0000 7215 0000 0072 1600  ...r....r....r..
-00000560: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
-00000570: 730a 0000 0004 040c 0108 0108 0108 03    s..............
+00000020: 0005 0000 0040 0000 0073 3800 0000 6400  .....@...s8...d.
+00000030: 5a00 6401 6402 6c01 5a02 6401 6402 6c03  Z.d.d.l.Z.d.d.l.
+00000040: 5a04 6401 6402 6c05 5a05 6407 6504 6a06  Z.d.d.l.Z.d.e.j.
+00000050: 6507 6502 6a08 6404 9c03 6405 6406 8405  e.e.j.d...d.d...
+00000060: 5a09 6402 5300 2908 7ab2 4d6f 6475 6c65  Z.d.S.).z.Module
+00000070: 2074 6f20 6361 6c63 756c 6174 6520 5348   to calculate SH
+00000080: 4150 2076 616c 7565 7320 666f 7220 6120  AP values for a 
+00000090: 7472 6169 6e65 6420 4d4c 206d 6f64 656c  trained ML model
+000000a0: 2e0a 0a54 6865 2069 6d70 6c65 6d65 6e74  ...The implement
+000000b0: 6174 696f 6e20 6973 2066 6c65 7869 626c  ation is flexibl
+000000c0: 6520 616e 6420 6361 6e20 6265 2075 7365  e and can be use
+000000d0: 6420 666f 7220 616c 6d6f 7374 2061 6e79  d for almost any
+000000e0: 204d 4c20 6d6f 6465 6c2e 2054 6865 2069   ML model. The i
+000000f0: 6d70 6c65 6d65 6e74 6174 696f 6e20 6973  mplementation is
+00000100: 2062 6173 6564 206f 6e20 7468 6520 5348   based on the SH
+00000110: 4150 206c 6962 7261 7279 2e0a e900 0000  AP library......
+00000120: 004e da04 7472 6565 2903 da02 6466 da09  .N..tree)...df..
+00000130: 6578 706c 6169 6e65 72da 0672 6574 7572  explainer..retur
+00000140: 6e63 0300 0000 0000 0000 0000 0000 0600  nc..............
+00000150: 0000 0800 0000 4300 0000 73aa 0000 0074  ......C...s....t
+00000160: 00a0 01a1 0001 007c 0264 016b 0272 7a7a  .......|.d.k.rzz
+00000170: 2a74 00a0 027c 00a1 017d 037c 03a0 037c  *t...|...}.|...|
+00000180: 01a1 017d 0474 006a 047c 047c 0164 0264  ...}.t.j.|.|.d.d
+00000190: 0364 048d 0401 0057 0071 a604 0074 056b  .d.....W.q...t.k
+000001a0: 0a72 7601 0001 0001 0074 00a0 067c 006a  .rv......t...|.j
+000001b0: 077c 01a1 027d 057c 05a0 037c 01a1 017d  .|...}.|...|...}
+000001c0: 0474 006a 047c 047c 0164 0364 058d 0301  .t.j.|.|.d.d....
+000001d0: 0059 0071 a658 006e 2c74 00a0 067c 006a  .Y.q.X.n,t...|.j
+000001e0: 077c 01a1 027d 057c 05a0 037c 01a1 017d  .|...}.|...|...}
+000001f0: 0474 006a 047c 047c 0164 0364 058d 0301  .t.j.|.|.d.d....
+00000200: 007c 0453 0064 0653 0029 0761 3d01 0000  .|.S.d.S.).a=...
+00000210: 0a20 2020 2053 6565 2065 7870 6c61 6e61  .    See explana
+00000220: 7469 6f6e 7320 756e 6465 723a 0a20 2020  tions under:.   
+00000230: 2068 7474 7073 3a2f 2f6d 6564 6975 6d2e   https://medium.
+00000240: 636f 6d2f 7261 7069 6473 2d61 692f 6770  com/rapids-ai/gp
+00000250: 752d 6163 6365 6c65 7261 7465 642d 7368  u-accelerated-sh
+00000260: 6170 2d76 616c 7565 732d 7769 7468 2d78  ap-values-with-x
+00000270: 6762 6f6f 7374 2d31 2d33 2d61 6e64 2d72  gboost-1-3-and-r
+00000280: 6170 6964 732d 3538 3766 6164 3638 3232  apids-587fad6822
+00000290: 0a20 2020 203a 7061 7261 6d20 6d6f 6465  .    :param mode
+000002a0: 6c3a 2054 7261 696e 6564 204d 4c20 6d6f  l: Trained ML mo
+000002b0: 6465 6c0a 2020 2020 3a70 6172 616d 2064  del.    :param d
+000002c0: 663a 2054 6573 7420 6461 7461 2074 6f20  f: Test data to 
+000002d0: 7072 6564 6963 7420 6f6e 2e0a 2020 2020  predict on..    
+000002e0: 3a70 6172 616d 2065 7870 6c61 696e 6572  :param explainer
+000002f0: 3a20 5365 7420 2274 7265 6522 2066 6f72  : Set "tree" for
+00000300: 2054 7265 6545 7870 6c61 696e 6572 2e20   TreeExplainer. 
+00000310: 4f74 6865 7277 6973 6520 7573 6573 204b  Otherwise uses K
+00000320: 6572 6e65 6c45 7870 6c61 696e 6572 2e0a  ernelExplainer..
+00000330: 2020 2020 3a72 6574 7572 6e3a 2053 6861      :return: Sha
+00000340: 7020 7661 6c75 6573 0a20 2020 2072 0200  p values.    r..
+00000350: 0000 da03 6261 7254 2902 da09 706c 6f74  ....barT)...plot
+00000360: 5f74 7970 65da 0473 686f 7729 0172 0800  _type..show).r..
+00000370: 0000 4e29 08da 0473 6861 70da 0669 6e69  ..N)...shap..ini
+00000380: 746a 73da 0d54 7265 6545 7870 6c61 696e  tjs..TreeExplain
+00000390: 6572 da0b 7368 6170 5f76 616c 7565 73da  er..shap_values.
+000003a0: 0c73 756d 6d61 7279 5f70 6c6f 74da 0e41  .summary_plot..A
+000003b0: 7373 6572 7469 6f6e 4572 726f 72da 0f4b  ssertionError..K
+000003c0: 6572 6e65 6c45 7870 6c61 696e 6572 da07  ernelExplainer..
+000003d0: 7072 6564 6963 7429 06da 056d 6f64 656c  predict)...model
+000003e0: 7203 0000 0072 0400 0000 5a0e 7472 6565  r....r....Z.tree
+000003f0: 5f65 7870 6c61 696e 6572 da11 6d6f 6465  _explainer..mode
+00000400: 6c5f 7368 6170 5f76 616c 7565 73da 146d  l_shap_values..m
+00000410: 6f64 656c 5f73 6861 705f 6578 706c 6169  odel_shap_explai
+00000420: 6e65 72a9 0072 1400 0000 fa45 2f68 6f6d  ner..r.....E/hom
+00000430: 652f 7468 6f6d 6173 2f49 6465 6150 726f  e/thomas/IdeaPro
+00000440: 6a65 6374 732f 426c 7565 4361 7374 2f62  jects/BlueCast/b
+00000450: 6c75 6563 6173 742f 6576 616c 7561 7469  luecast/evaluati
+00000460: 6f6e 2f73 6861 705f 7661 6c75 6573 2e70  on/shap_values.p
+00000470: 79da 1173 6861 705f 6578 706c 616e 6174  y..shap_explanat
+00000480: 696f 6e73 0a00 0000 731c 0000 0000 0908  ions....s.......
+00000490: 0108 0102 010a 010a 0116 010e 010e 010a  ................
+000004a0: 0118 020e 010a 0110 0172 1600 0000 2901  .........r....).
+000004b0: 7202 0000 0029 0ada 075f 5f64 6f63 5f5f  r....)...__doc__
+000004c0: da05 6e75 6d70 79da 026e 70da 0670 616e  ..numpy..np..pan
+000004d0: 6461 73da 0270 6472 0900 0000 da09 4461  das..pdr......Da
+000004e0: 7461 4672 616d 65da 0373 7472 da07 6e64  taFrame..str..nd
+000004f0: 6172 7261 7972 1600 0000 7214 0000 0072  arrayr....r....r
+00000500: 1400 0000 7214 0000 0072 1500 0000 da08  ....r....r......
+00000510: 3c6d 6f64 756c 653e 0100 0000 7308 0000  <module>....s...
+00000520: 0004 0408 0108 0108 03                   .........
```

### Comparing `bluecast-0.5/bluecast/evaluation/eval_metrics.py` & `bluecast-0.7/bluecast/evaluation/eval_metrics.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.5/bluecast/evaluation/shap_values.py` & `bluecast-0.7/bluecast/evaluation/shap_values.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.5/bluecast/general_utils/__pycache__/general_utils.cpython-310.pyc` & `bluecast-0.7/bluecast/general_utils/__pycache__/general_utils.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.5/bluecast/general_utils/__pycache__/general_utils.cpython-38.pyc` & `bluecast-0.7/bluecast/general_utils/__pycache__/general_utils.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.5/bluecast/general_utils/general_utils.py` & `bluecast-0.7/bluecast/general_utils/general_utils.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.5/bluecast/ml_modelling/__pycache__/base_classes.cpython-310.pyc` & `bluecast-0.7/bluecast/ml_modelling/__pycache__/base_classes.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.5/bluecast/ml_modelling/__pycache__/base_classes.cpython-38.pyc` & `bluecast-0.7/bluecast/ml_modelling/__pycache__/base_classes.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.5/bluecast/ml_modelling/__pycache__/xgboost.cpython-310.pyc` & `bluecast-0.7/bluecast/ml_modelling/__pycache__/xgboost.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun Jun 25 05:33:45 2023 UTC, .py size: 13523 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 b9d1 9764 d334 0000  o..........d.4..
+00000000: 6f0d 0d0a 0000 0000 6063 9d64 7e3a 0000  o.......`c.d~:..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 a400 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d01 5a01 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c02 6d03 5a03 6d04 5a04 6d05 5a05  d.l.m.Z.m.Z.m.Z.
 00000050: 6d06 5a06 0100 6401 6404 6c07 5a08 6401  m.Z...d.d.l.Z.d.
 00000060: 6404 6c09 5a09 6401 6404 6c0a 5a0b 6401  d.l.Z.d.d.l.Z.d.
 00000070: 6404 6c0c 5a0d 6401 6405 6c0e 6d0f 5a0f  d.l.Z.d.d.l.m.Z.
@@ -149,415 +149,433 @@
 00000940: 0114 0112 0206 0208 0114 0112 0206 0208  ................
 00000950: 0116 0116 027a 1d58 6762 6f6f 7374 4d6f  .....z.XgboostMo
 00000960: 6465 6c2e 6368 6563 6b5f 6c6f 6164 5f63  del.check_load_c
 00000970: 6f6e 6673 da07 785f 7472 6169 6eda 0678  onfs..x_train..x
 00000980: 5f74 6573 74da 0779 5f74 7261 696e da06  _test..y_train..
 00000990: 795f 7465 7374 6305 0000 0000 0000 0000  y_testc.........
 000009a0: 0000 0009 0000 0007 0000 0043 0000 0073  ...........C...s
-000009b0: 3e01 0000 7400 7401 a002 a100 9b00 6401  >...t.t.......d.
+000009b0: 5601 0000 7400 7401 a002 a100 9b00 6401  V...t.t.......d.
 000009c0: 9d02 8301 0100 7c00 a003 a100 0100 7c00  ......|.......|.
 000009d0: 6a04 7213 7c00 6a05 7317 7406 6402 8301  j.r.|.j.s.t.d...
 000009e0: 8201 7c00 6a05 6a07 7223 7c00 a008 7c01  ..|.j.j.r#|...|.
 000009f0: 7c02 7c03 7c04 a104 0100 7409 6403 8301  |.|.|.....t.d...
 00000a00: 0100 7409 6404 8301 0100 7c00 6a05 6a0a  ..t.d.....|.j.j.
 00000a10: 7246 7400 7401 a002 a100 9b00 6405 9d02  rFt.t.......d...
 00000a20: 8301 0100 740b a00c 7c01 7c02 6702 a101  ....t...|.|.g...
 00000a30: 7d01 740b a00c 7c03 7c04 6702 a101 7d03  }.t...|.|.g...}.
-00000a40: 7c00 6a04 6a0d 7258 7c00 a00e 7c03 a101  |.j.j.rX|...|...
-00000a50: 7d05 740f 6a10 7c01 7c03 7c05 6406 8d03  }.t.j.|.|.|.d...
-00000a60: 7d06 6e07 740f 6a10 7c01 7c03 6407 8d02  }.n.t.j.|.|.d...
-00000a70: 7d06 740f 6a10 7c02 7c04 6407 8d02 7d07  }.t.j.|.|.d...}.
-00000a80: 7c06 6408 6602 7c07 6409 6602 6702 7d08  |.d.f.|.d.f.g.}.
-00000a90: 7c00 6a05 6a11 640a 6b02 7288 740f 6a12  |.j.j.d.k.r.t.j.
-00000aa0: 7c00 6a04 6a13 7c06 7c00 6a04 6a13 640b  |.j.j.|.|.j.j.d.
-00000ab0: 1900 7c00 6a05 6a14 7c08 640c 8d05 7c00  ..|.j.j.|.d...|.
-00000ac0: 5f15 6e10 740f 6a12 7c00 6a04 6a13 7c06  _.n.t.j.|.j.j.|.
-00000ad0: 7c00 6a04 6a13 640b 1900 7c08 640d 8d04  |.j.j.d...|.d...
-00000ae0: 7c00 5f15 7409 640e 8301 0100 7c00 6a15  |._.t.d.....|.j.
-00000af0: 5300 290f 7a3f 5472 6169 6e20 5867 626f  S.).z?Train Xgbo
-00000b00: 6f73 7420 6d6f 6465 6c2e 2049 6e63 6c75  ost model. Inclu
-00000b10: 6465 7320 6879 7065 7270 6172 616d 6574  des hyperparamet
-00000b20: 6572 2074 756e 696e 6720 6f6e 2064 6566  er tuning on def
-00000b30: 6175 6c74 2e7a 1e3a 2053 7461 7274 2066  ault.z.: Start f
-00000b40: 6974 7469 6e67 2058 6762 6f6f 7374 206d  itting Xgboost m
-00000b50: 6f64 656c 2e7a 2c63 6f6e 665f 7061 7261  odel.z,conf_para
-00000b60: 6d73 5f78 6762 6f6f 7374 206f 7220 636f  ms_xgboost or co
-00000b70: 6e66 5f74 7261 696e 696e 6720 6973 204e  nf_training is N
-00000b80: 6f6e 657a 1e46 696e 6973 6865 6420 6879  onez.Finished hy
-00000b90: 7065 7270 6172 616d 6574 6572 2074 756e  perparameter tun
-00000ba0: 696e 677a 0e53 7461 7274 2074 7261 696e  ingz.Start train
-00000bb0: 696e 677a 7f3a 2055 6e69 6f6e 2074 7261  ingz.: Union tra
-00000bc0: 696e 2061 6e64 2074 6573 7420 6461 7461  in and test data
-00000bd0: 2066 6f72 2066 696e 616c 206d 6f64 656c   for final model
-00000be0: 2074 7261 696e 696e 6720 6261 7365 6420   training based 
-00000bf0: 6f6e 2054 7261 696e 696e 6743 6f6e 6669  on TrainingConfi
-00000c00: 670a 2020 2020 2020 2020 2020 2020 2070  g.             p
-00000c10: 6172 616d 2027 7573 655f 6675 6c6c 5f64  aram 'use_full_d
-00000c20: 6174 615f 666f 725f 6669 6e61 6c5f 6d6f  ata_for_final_mo
-00000c30: 6465 6c27 a902 da05 6c61 6265 6cda 0677  del'....label..w
-00000c40: 6569 6768 74a9 0172 2800 0000 da05 7472  eight..r(.....tr
-00000c50: 6169 6eda 0474 6573 74e9 0100 0000 da05  ain..test.......
-00000c60: 7374 6570 7329 03da 0f6e 756d 5f62 6f6f  steps)...num_boo
-00000c70: 7374 5f72 6f75 6e64 da15 6561 726c 795f  st_round..early_
-00000c80: 7374 6f70 7069 6e67 5f72 6f75 6e64 73da  stopping_rounds.
-00000c90: 0565 7661 6c73 2902 722f 0000 0072 3100  .evals).r/...r1.
-00000ca0: 0000 7a11 4669 6e69 7368 6564 2074 7261  ..z.Finished tra
-00000cb0: 696e 696e 6729 1672 0d00 0000 7202 0000  ining).r....r...
-00000cc0: 0072 1e00 0000 7222 0000 0072 1500 0000  .r....r"...r....
-00000cd0: 7213 0000 00da 0a56 616c 7565 4572 726f  r......ValueErro
-00000ce0: 72da 0e61 7574 6f74 756e 655f 6d6f 6465  r..autotune_mode
-00000cf0: 6cda 0861 7574 6f74 756e 65da 0570 7269  l..autotune..pri
-00000d00: 6e74 da1d 7573 655f 6675 6c6c 5f64 6174  nt..use_full_dat
-00000d10: 615f 666f 725f 6669 6e61 6c5f 6d6f 6465  a_for_final_mode
-00000d20: 6cda 0270 64da 0663 6f6e 6361 74da 0d73  l..pd..concat..s
-00000d30: 616d 706c 655f 7765 6967 6874 7221 0000  ample_weightr!..
-00000d40: 00da 0378 6762 da07 444d 6174 7269 78da  ...xgb..DMatrix.
-00000d50: 1468 7970 6572 7475 6e69 6e67 5f63 765f  .hypertuning_cv_
-00000d60: 666f 6c64 7372 2b00 0000 da06 7061 7261  foldsr+.....para
-00000d70: 6d73 7230 0000 0072 1600 0000 2909 7217  msr0...r....).r.
-00000d80: 0000 0072 2300 0000 7224 0000 0072 2500  ...r#...r$...r%.
-00000d90: 0000 7226 0000 0072 2000 0000 da07 645f  ..r&...r .....d_
-00000da0: 7472 6169 6eda 0664 5f74 6573 74da 0865  train..d_test..e
-00000db0: 7661 6c5f 7365 7472 1800 0000 7218 0000  val_setr....r...
-00000dc0: 0072 1900 0000 da03 6669 7447 0000 0073  .r......fitG...s
-00000dd0: 4800 0000 1208 0801 0c02 0801 0802 1001  H...............
-00000de0: 0802 0802 0801 0201 0c01 04ff 0e04 0e01  ................
-00000df0: 0802 0a01 1201 0e02 0e02 1001 0c02 0401  ................
-00000e00: 0601 0201 0a01 0601 0201 0afb 0408 0601  ................
-00000e10: 0201 0a01 0201 08fc 0806 0601 7a10 5867  ............z.Xg
-00000e20: 626f 6f73 744d 6f64 656c 2e66 6974 6305  boostModel.fitc.
-00000e30: 0000 0000 0000 0000 0000 000b 0000 000a  ................
-00000e40: 0000 0003 0000 0073 c201 0000 7400 7401  .......s....t.t.
-00000e50: a002 a100 9b00 6401 9d02 8301 0100 7403  ......d.......t.
-00000e60: 6a04 7c02 8804 6402 8d02 8900 7405 8300  j.|...d.....t...
-00000e70: 8902 8801 a006 a100 0100 8801 6a07 7220  ............j.r 
-00000e80: 8801 6a08 7220 8801 6a09 7324 740a 6403  ..j.r ..j.s$t.d.
-00000e90: 8301 8201 8700 8701 8702 8703 8704 8705  ................
-00000ea0: 6606 6404 6405 8408 7d05 6406 7d06 740b  f.d.d...}.d.}.t.
-00000eb0: 6a0c 6a0d 6407 8801 6a08 6a0e 6408 8d02  j.j.d...j.j.d...
-00000ec0: 7d07 740b 6a0f 6409 7c07 7c06 9b00 640a  }.t.j.d.|.|...d.
-00000ed0: 9d02 640b 8d03 7d08 7c08 6a10 7c05 8801  ..d...}.|.j.|...
-00000ee0: 6a08 6a11 8801 6a08 6a12 6407 6407 640c  j.j...j.j.d.d.d.
-00000ef0: 8d05 0100 7a16 740b 6a13 a014 7c08 a101  ....z.t.j...|...
-00000f00: 7d09 7c09 a015 a100 0100 740b 6a13 a016  }.|.......t.j...
-00000f10: 7c08 a101 7d09 7c09 a015 a100 0100 5700  |...}.|.......W.
-00000f20: 6e0c 0400 7417 7418 740a 6603 7976 0100  n...t.t.t.f.yv..
-00000f30: 0100 0100 5900 6e01 7700 7c08 6a19 6a1a  ....Y.n.w.|.j.j.
-00000f40: 7d0a 6900 640d 8801 6a09 6a1b 9301 640e  }.i.d...j.j...d.
-00000f50: 8801 6a09 6a1c 9301 640f 8801 6a09 6a1d  ..j.j...d...j.j.
-00000f60: 9301 6410 8802 9301 6411 8805 a01e a100  ..d.....d.......
-00000f70: 9301 6412 7c0a 6412 1900 9301 6413 7c0a  ..d.|.d.....d.|.
-00000f80: 6413 1900 9301 6414 7c0a 6414 1900 9301  d.....d.|.d.....
-00000f90: 6415 7c0a 6415 1900 9301 6416 7c0a 6416  d.|.d.....d.|.d.
-00000fa0: 1900 9301 6417 7c0a 6417 1900 9301 6418  ....d.|.d.....d.
-00000fb0: 7c0a 6418 1900 9301 6419 7c0a 6419 1900  |.d.....d.|.d...
-00000fc0: 9301 641a 7c0a 641a 1900 9301 641b 8801  ..d.|.d.....d...
-00000fd0: 6a09 6a1f 9301 641c 7c0a 641c 1900 9301  j.j...d.|.d.....
-00000fe0: 641d 7c0a 641d 1900 9301 8801 6a07 5f1a  d.|.d.......j._.
-00000ff0: 7420 641e 8801 6a07 6a1a 8302 0100 7c0a  t d...j.j.....|.
-00001000: 641f 1900 8801 6a07 5f21 6420 5300 2921  d.....j._!d S.)!
-00001010: 7a7b 5475 6e65 2068 7970 6572 7061 7261  z{Tune hyperpara
-00001020: 6d65 7465 7273 2e0a 0a20 2020 2020 2020  meters...       
-00001030: 2041 6e20 616c 7465 726e 6174 6976 6520   An alternative 
-00001040: 636f 6e66 6967 2063 616e 2062 6520 7072  config can be pr
-00001050: 6f76 6964 6564 2074 6f20 6f76 6572 7772  ovided to overwr
-00001060: 6974 6520 7468 6520 6879 7065 7270 6172  ite the hyperpar
-00001070: 616d 6574 6572 2073 6561 7263 6820 7370  ameter search sp
-00001080: 6163 652e 0a20 2020 2020 2020 207a 2f3a  ace..        z/:
-00001090: 2053 7461 7274 2068 7970 6572 7061 7261   Start hyperpara
-000010a0: 6d65 7465 7220 7475 6e69 6e67 206f 6620  meter tuning of 
-000010b0: 5867 626f 6f73 7420 6d6f 6465 6c2e 722a  Xgboost model.r*
-000010c0: 0000 007a 3941 7420 6c65 6173 7420 6f6e  ...z9At least on
-000010d0: 6520 6f66 2074 6865 2063 6f6e 6669 6773  e of the configs
-000010e0: 2069 7320 4e6f 6e65 2c20 7768 6963 6820   is None, which 
-000010f0: 6973 206e 6f74 2061 6c6c 6f77 6564 6301  is not allowedc.
-00001100: 0000 0000 0000 0000 0000 000c 0000 000a  ................
-00001110: 0000 0013 0000 0073 3c02 0000 6900 6401  .......s<...i.d.
-00001120: 8801 6a00 6a01 9301 6402 8801 6a00 6a02  ..j.j...d...j.j.
-00001130: 9301 6403 8801 6a00 6a03 9301 6404 8802  ..d...j.j...d...
-00001140: 9301 6405 8805 a004 a100 9301 6406 7c00  ..d.........d.|.
-00001150: a005 6406 8801 6a00 6a06 8801 6a00 6a07  ..d...j.j...j.j.
-00001160: a103 9301 6407 7c00 a008 6407 8801 6a00  ....d.|...d...j.
-00001170: 6a09 8801 6a00 6a0a a103 9301 6408 7c00  j...j.j.....d.|.
-00001180: a008 6408 8801 6a00 6a0b 8801 6a00 6a0c  ..d...j.j...j.j.
-00001190: a103 9301 6409 7c00 a005 6409 8801 6a00  ....d.|...d...j.
-000011a0: 6a0d 8801 6a00 6a0e a103 9301 640a 7c00  j...j.j.....d.|.
-000011b0: a008 640a 8801 6a00 6a0f 8801 6a00 6a10  ..d...j.j...j.j.
-000011c0: a103 9301 640b 7c00 a008 640b 8801 6a00  ....d.|...d...j.
-000011d0: 6a11 8801 6a00 6a12 a103 9301 640c 7c00  j...j.j.....d.|.
-000011e0: a008 640c 8801 6a00 6a13 8801 6a00 6a14  ..d...j.j...j.j.
-000011f0: a103 9301 640d 7c00 a008 640d 8801 6a00  ....d.|...d...j.
-00001200: 6a15 8801 6a00 6a16 a103 9301 640e 7c00  j...j.j.....d.|.
-00001210: a005 640e 8801 6a00 6a17 8801 6a00 6a18  ..d...j.j...j.j.
-00001220: a103 9301 640f 8801 6a00 6a19 9301 6410  ....d...j.j...d.
-00001230: 7c00 a005 6410 8801 6a00 6a1a 8801 6a00  |...d...j.j...j.
-00001240: 6a1b a103 9301 6411 7c00 a005 6411 8801  j.....d.|...d...
-00001250: 6a00 6a1c 8801 6a00 6a1d a103 9301 7d01  j.j...j.j.....}.
-00001260: 7c00 a01e 6412 6413 6414 6702 a102 7d02  |...d.d.d.g...}.
-00001270: 7c02 72ba 8801 a01f 8805 a101 7d03 7420  |.r.........}.t 
-00001280: 6a21 8803 8805 7c03 6415 8d03 7d04 6e07  j!....|.d...}.n.
-00001290: 7420 6a21 8803 8805 6416 8d02 7d04 7422  t j!....d...}.t"
-000012a0: 6a23 a024 7c00 6417 a102 7d05 8801 6a25  j#.$|.d...}...j%
-000012b0: 6a26 6418 6b02 9001 7202 7c04 6419 6602  j&d.k...r.|.d.f.
-000012c0: 8800 641a 6602 6702 7d06 7420 6a27 7c01  ..d.f.g.}.t j'|.
-000012d0: 7c04 7c01 6410 1900 8801 6a25 6a28 7c06  |.|.d.....j%j(|.
-000012e0: 7c05 6701 8801 6a00 6a03 641b 8d07 7d07  |.g...j.j.d...}.
-000012f0: 7c07 a029 8800 a101 7d08 742a a02b 641c  |..)....}.t*.+d.
-00001300: 641d 8400 7c08 4400 8301 a101 7d09 742c  d...|.D.....}.t,
-00001310: 8804 7c09 8302 641e 1400 7d0a 7c0a 5300  ..|...d...}.|.S.
-00001320: 7420 6a2d 7c01 7c04 7c01 6410 1900 8801  t j-|.|.|.d.....
-00001330: 6a25 6a26 6413 8801 6a25 6a2e 7c05 6701  j%j&d...j%j.|.g.
-00001340: 8801 6a25 6a2f 641f 8d08 7d0b 7c0b 6420  ..j%j/d...}.|.d 
-00001350: 1900 a030 a100 5300 2921 4eda 096f 626a  ...0..S.)!N..obj
-00001360: 6563 7469 7665 da0b 6576 616c 5f6d 6574  ective..eval_met
-00001370: 7269 63da 0776 6572 626f 7365 da0b 7472  ric..verbose..tr
-00001380: 6565 5f6d 6574 686f 64da 096e 756d 5f63  ee_method..num_c
-00001390: 6c61 7373 da09 6d61 785f 6465 7074 68da  lass..max_depth.
-000013a0: 0561 6c70 6861 da06 6c61 6d62 6461 da0a  .alpha..lambda..
-000013b0: 6e75 6d5f 6c65 6176 6573 da09 7375 6273  num_leaves..subs
-000013c0: 616d 706c 65da 1063 6f6c 7361 6d70 6c65  ample..colsample
-000013d0: 5f62 7974 7265 65da 1163 6f6c 7361 6d70  _bytree..colsamp
-000013e0: 6c65 5f62 796c 6576 656c da10 636f 6c73  le_bylevel..cols
-000013f0: 616d 706c 655f 6279 6e6f 6465 da11 6d69  ample_bynode..mi
-00001400: 6e5f 6368 696c 645f 7361 6d70 6c65 73da  n_child_samples.
-00001410: 0365 7461 722e 0000 00da 116e 756d 5f70  .etar......num_p
-00001420: 6172 616c 6c65 6c5f 7472 6565 7239 0000  arallel_treer9..
-00001430: 0054 4672 2700 0000 722a 0000 007a 0d74  .TFr'...r*...z.t
-00001440: 6573 742d 6d6c 6f67 6c6f 7373 722d 0000  est-mloglossr-..
-00001450: 0072 2b00 0000 722c 0000 0029 0572 2f00  .r+...r,...).r/.
-00001460: 0000 7230 0000 0072 3100 0000 da09 6361  ..r0...r1.....ca
-00001470: 6c6c 6261 636b 73da 0c76 6572 626f 7365  llbacks..verbose
-00001480: 5f65 7661 6c63 0100 0000 0000 0000 0000  _evalc..........
-00001490: 0000 0200 0000 0500 0000 5300 0000 f316  ..........S.....
-000014a0: 0000 0067 007c 005d 077d 0174 00a0 017c  ...g.|.].}.t...|
-000014b0: 01a1 0191 0271 0253 0072 1800 0000 a902  .....q.S.r......
-000014c0: da02 6e70 da06 6172 676d 6178 a902 da02  ..np..argmax....
-000014d0: 2e30 da04 6c69 6e65 7218 0000 0072 1800  .0..liner....r..
-000014e0: 0000 7219 0000 00da 0a3c 6c69 7374 636f  ..r......<listco
-000014f0: 6d70 3ee9 0000 00f3 0200 0000 1600 7a3c  mp>...........z<
-00001500: 5867 626f 6f73 744d 6f64 656c 2e61 7574  XgboostModel.aut
-00001510: 6f74 756e 652e 3c6c 6f63 616c 733e 2e6f  otune.<locals>.o
-00001520: 626a 6563 7469 7665 2e3c 6c6f 6361 6c73  bjective.<locals
-00001530: 3e2e 3c6c 6973 7463 6f6d 703e e9ff ffff  >.<listcomp>....
-00001540: ff29 0872 3d00 0000 da06 6474 7261 696e  .).r=.....dtrain
-00001550: 722f 0000 00da 056e 666f 6c64 da09 6173  r/.....nfold..as
-00001560: 5f70 616e 6461 73da 0473 6565 6472 5200  _pandas..seedrR.
-00001570: 0000 da07 7368 7566 666c 657a 1274 6573  ....shufflez.tes
-00001580: 742d 6d6c 6f67 6c6f 7373 2d6d 6561 6e29  t-mlogloss-mean)
-00001590: 3172 1400 0000 da0f 6d6f 6465 6c5f 6f62  1r......model_ob
-000015a0: 6a65 6374 6976 65da 116d 6f64 656c 5f65  jective..model_e
-000015b0: 7661 6c5f 6d65 7472 6963 da0f 6d6f 6465  val_metric..mode
-000015c0: 6c5f 7665 7262 6f73 6974 79da 076e 756e  l_verbosity..nun
-000015d0: 6971 7565 5a0b 7375 6767 6573 745f 696e  iqueZ.suggest_in
-000015e0: 74da 0d6d 6178 5f64 6570 7468 5f6d 696e  t..max_depth_min
-000015f0: da0d 6d61 785f 6465 7074 685f 6d61 785a  ..max_depth_maxZ
-00001600: 0d73 7567 6765 7374 5f66 6c6f 6174 da09  .suggest_float..
-00001610: 616c 7068 615f 6d69 6eda 0961 6c70 6861  alpha_min..alpha
-00001620: 5f6d 6178 da0a 6c61 6d62 6461 5f6d 696e  _max..lambda_min
-00001630: da0a 6c61 6d62 6461 5f6d 6178 da0e 6e75  ..lambda_max..nu
-00001640: 6d5f 6c65 6176 6573 5f6d 696e da0e 6e75  m_leaves_min..nu
-00001650: 6d5f 6c65 6176 6573 5f6d 6178 da0e 7375  m_leaves_max..su
-00001660: 625f 7361 6d70 6c65 5f6d 696e da0e 7375  b_sample_min..su
-00001670: 625f 7361 6d70 6c65 5f6d 6178 da16 636f  b_sample_max..co
-00001680: 6c5f 7361 6d70 6c65 5f62 795f 7472 6565  l_sample_by_tree
-00001690: 5f6d 696e da16 636f 6c5f 7361 6d70 6c65  _min..col_sample
-000016a0: 5f62 795f 7472 6565 5f6d 6178 da17 636f  _by_tree_max..co
-000016b0: 6c5f 7361 6d70 6c65 5f62 795f 6c65 7665  l_sample_by_leve
-000016c0: 6c5f 6d69 6eda 1763 6f6c 5f73 616d 706c  l_min..col_sampl
-000016d0: 655f 6279 5f6c 6576 656c 5f6d 6178 da16  e_by_level_max..
-000016e0: 636f 6c5f 7361 6d70 6c65 5f62 795f 6e6f  col_sample_by_no
-000016f0: 6465 5f6d 696e da16 636f 6c5f 7361 6d70  de_min..col_samp
-00001700: 6c65 5f62 795f 6e6f 6465 5f6d 6178 da15  le_by_node_max..
-00001710: 6d69 6e5f 6368 696c 645f 7361 6d70 6c65  min_child_sample
-00001720: 735f 6d69 6eda 156d 696e 5f63 6869 6c64  s_min..min_child
-00001730: 5f73 616d 706c 6573 5f6d 6178 7250 0000  _samples_maxrP..
-00001740: 00da 0973 7465 7073 5f6d 696e da09 7374  ...steps_min..st
-00001750: 6570 735f 6d61 78da 156e 756d 5f70 6172  eps_max..num_par
-00001760: 616c 6c65 6c5f 7472 6565 5f6d 696e da15  allel_tree_min..
-00001770: 6e75 6d5f 7061 7261 6c6c 656c 5f74 7265  num_parallel_tre
-00001780: 655f 6d61 785a 1373 7567 6765 7374 5f63  e_maxZ.suggest_c
-00001790: 6174 6567 6f72 6963 616c 7221 0000 0072  ategoricalr!...r
-000017a0: 3a00 0000 723b 0000 00da 066f 7074 756e  :...r;.....optun
-000017b0: 615a 0b69 6e74 6567 7261 7469 6f6e 5a16  aZ.integrationZ.
-000017c0: 5847 426f 6f73 7450 7275 6e69 6e67 4361  XGBoostPruningCa
-000017d0: 6c6c 6261 636b 7213 0000 0072 3c00 0000  llbackr....r<...
-000017e0: 722b 0000 0072 3000 0000 da07 7072 6564  r+...r0.....pred
-000017f0: 6963 7472 5600 0000 da07 6173 6172 7261  ictrV.....asarra
-00001800: 7972 0700 0000 da02 6376 da13 676c 6f62  yr......cv..glob
-00001810: 616c 5f72 616e 646f 6d5f 7374 6174 65da  al_random_state.
-00001820: 1773 6875 6666 6c65 5f64 7572 696e 675f  .shuffle_during_
-00001830: 7472 6169 6e69 6e67 da04 6d65 616e 290c  training..mean).
-00001840: da05 7472 6961 6cda 0570 6172 616d 7239  ..trial..paramr9
-00001850: 0000 0072 2000 0000 723e 0000 005a 1070  ...r ...r>...Z.p
-00001860: 7275 6e69 6e67 5f63 616c 6c62 6163 6b72  runing_callbackr
-00001870: 4000 0000 7216 0000 00da 0570 7265 6473  @...r......preds
-00001880: da0b 7072 6564 5f6c 6162 656c 735a 076d  ..pred_labelsZ.m
-00001890: 6174 7468 6577 da06 7265 7375 6c74 a906  atthew..result..
-000018a0: 723f 0000 0072 1700 0000 5a08 7472 6169  r?...r....Z.trai
-000018b0: 6e5f 6f6e 7223 0000 0072 2600 0000 7225  n_onr#...r&...r%
-000018c0: 0000 0072 1800 0000 7219 0000 0072 4200  ...r....r....rB.
-000018d0: 0000 9800 0000 73d6 0000 0002 0108 0102  ......s.........
-000018e0: ff08 0202 fe08 0302 fd04 0402 fc08 0502  ................
-000018f0: fb06 0602 0106 0106 0102 fd02 fa06 0b0e  ................
-00001900: 0102 ff02 f506 0e0e 0102 ff02 f206 1102  ................
-00001910: 0106 0106 0102 fd02 ef06 1602 0106 0106  ................
-00001920: 0102 fd02 ea06 1b02 0106 0106 0102 fd02  ................
-00001930: e506 2002 0106 0106 0102 fd02 e006 2502  .. ...........%.
-00001940: 0106 0106 0102 fd02 db06 2a02 0106 0106  ..........*.....
-00001950: 0102 fd02 d608 2f02 d106 300e 0102 ff02  ....../...0.....
-00001960: d006 3302 0106 0106 0102 fd04 cd10 3904  ..3...........9.
-00001970: 010a 0112 010e 0206 0204 0104 ff0e 0410  ................
-00001980: 0104 0102 0102 0106 0106 0102 0104 0106  ................
-00001990: 0106 f90a 0914 010e 0104 0104 0202 0102  ................
-000019a0: 0106 0106 0202 0106 0104 0106 0106 f70c  ................
-000019b0: 0c7a 2858 6762 6f6f 7374 4d6f 6465 6c2e  .z(XgboostModel.
-000019c0: 6175 746f 7475 6e65 2e3c 6c6f 6361 6c73  autotune.<locals
-000019d0: 3e2e 6f62 6a65 6374 6976 65da 0778 6762  >.objective..xgb
-000019e0: 6f6f 7374 5429 025a 0c6d 756c 7469 7661  oostT).Z.multiva
-000019f0: 7269 6174 6572 6100 0000 da08 6d69 6e69  riatera.....mini
-00001a00: 6d69 7a65 7a07 2074 756e 696e 6729 03da  mizez. tuning)..
-00001a10: 0964 6972 6563 7469 6f6e da07 7361 6d70  .direction..samp
-00001a20: 6c65 725a 0a73 7475 6479 5f6e 616d 6529  lerZ.study_name)
-00001a30: 04da 086e 5f74 7269 616c 73da 0774 696d  ...n_trials..tim
-00001a40: 656f 7574 5a0e 6763 5f61 6674 6572 5f74  eoutZ.gc_after_t
-00001a50: 7269 616c 5a11 7368 6f77 5f70 726f 6772  rialZ.show_progr
-00001a60: 6573 735f 6261 7272 4200 0000 7243 0000  ess_barrB...rC..
-00001a70: 0072 4400 0000 7245 0000 0072 4600 0000  .rD...rE...rF...
-00001a80: 7247 0000 0072 4800 0000 7249 0000 0072  rG...rH...rI...r
-00001a90: 4a00 0000 724b 0000 0072 4c00 0000 724d  J...rK...rL...rM
-00001aa0: 0000 0072 4e00 0000 724f 0000 0072 5000  ...rN...rO...rP.
-00001ab0: 0000 722e 0000 0072 5100 0000 7a0d 4265  ..r....rQ...z.Be
-00001ac0: 7374 2070 6172 616d 733a 2072 3900 0000  st params: r9...
-00001ad0: 4e29 2272 0d00 0000 7202 0000 0072 1e00  N)"r....r....r..
-00001ae0: 0000 723a 0000 0072 3b00 0000 720c 0000  ..r:...r;...r...
-00001af0: 0072 2200 0000 7215 0000 0072 1300 0000  .r"...r....r....
-00001b00: 7214 0000 0072 3200 0000 727d 0000 005a  r....r2...r}...Z
-00001b10: 0873 616d 706c 6572 735a 0a54 5045 5361  .samplersZ.TPESa
-00001b20: 6d70 6c65 7272 8100 0000 5a0c 6372 6561  mplerr....Z.crea
-00001b30: 7465 5f73 7475 6479 da08 6f70 7469 6d69  te_study..optimi
-00001b40: 7a65 da1c 6879 7065 7270 6172 616d 6574  ze..hyperparamet
-00001b50: 6572 5f74 756e 696e 675f 726f 756e 6473  er_tuning_rounds
-00001b60: da26 6879 7065 7270 6172 616d 6574 6572  .&hyperparameter
-00001b70: 5f74 756e 696e 675f 6d61 785f 7275 6e74  _tuning_max_runt
-00001b80: 696d 655f 7365 6373 5a0d 7669 7375 616c  ime_secsZ.visual
-00001b90: 697a 6174 696f 6e5a 1970 6c6f 745f 6f70  izationZ.plot_op
-00001ba0: 7469 6d69 7a61 7469 6f6e 5f68 6973 746f  timization_histo
-00001bb0: 7279 da04 7368 6f77 5a16 706c 6f74 5f70  ry..showZ.plot_p
-00001bc0: 6172 616d 5f69 6d70 6f72 7461 6e63 6573  aram_importances
-00001bd0: da11 5a65 726f 4469 7669 7369 6f6e 4572  ..ZeroDivisionEr
-00001be0: 726f 72da 0c52 756e 7469 6d65 4572 726f  ror..RuntimeErro
-00001bf0: 725a 0a62 6573 745f 7472 6961 6c72 3d00  rZ.best_trialr=.
-00001c00: 0000 7263 0000 0072 6400 0000 7265 0000  ..rc...rd...re..
-00001c10: 0072 6600 0000 7250 0000 0072 3500 0000  .rf...rP...r5...
-00001c20: 7239 0000 0029 0b72 1700 0000 7223 0000  r9...).r....r#..
-00001c30: 0072 2400 0000 7225 0000 0072 2600 0000  .r$...r%...r&...
-00001c40: 7242 0000 00da 0961 6c67 6f72 6974 686d  rB.....algorithm
-00001c50: 728d 0000 005a 0573 7475 6479 da03 6669  r....Z.study..fi
-00001c60: 675a 1278 6762 6f6f 7374 5f62 6573 745f  gZ.xgboost_best_
-00001c70: 7061 7261 6d72 1800 0000 7289 0000 0072  paramr....r....r
-00001c80: 1900 0000 7234 0000 007e 0000 0073 9c00  ....r4...~...s..
-00001c90: 0000 120b 0e01 0601 0802 0403 02ff 0402  ................
-00001ca0: 02fe 0403 02fd 0205 0201 04ff 1604 0463  ...............c
-00001cb0: 0601 0801 06ff 0403 0201 0201 0801 06fd  ................
-00001cc0: 0406 0201 0601 0601 0201 0201 06fb 0207  ................
-00001cd0: 0c01 0801 0c01 0c01 1201 0401 02ff 0803  ................
-00001ce0: 0201 0801 02ff 0802 02fe 0803 02fd 0404  ................
-00001cf0: 02fc 0805 02fb 0406 0201 02ff 02fa 0809  ................
-00001d00: 02f7 080a 02f6 080b 02f5 080c 02f4 080d  ................
-00001d10: 02f3 080e 02f2 080f 02f1 0810 02f0 0811  ................
-00001d20: 02ef 0812 02ee 0813 08ed 0e15 1001 7a15  ..............z.
-00001d30: 5867 626f 6f73 744d 6f64 656c 2e61 7574  XgboostModel.aut
-00001d40: 6f74 756e 65da 0264 6663 0200 0000 0000  otune..dfc......
-00001d50: 0000 0000 0000 0600 0000 0400 0000 4300  ..............C.
-00001d60: 0000 73a0 0000 0074 0074 01a0 02a1 009b  ..s....t.t......
-00001d70: 0064 019d 0283 0101 0074 0364 0283 0101  .d.......t.d....
-00001d80: 0074 04a0 057c 01a1 017d 027c 006a 0673  .t...|...}.|.j.s
-00001d90: 1974 0764 0383 0182 017c 006a 0873 2074  .t.d.....|.j.s t
-00001da0: 0764 0483 0182 017c 006a 06a0 097c 02a1  .d.....|.j...|..
-00001db0: 017d 037c 006a 0a64 056b 0272 3c74 0ba0  .}.|.j.d.k.r<t..
-00001dc0: 0c64 0664 0784 007c 0344 0083 01a1 017d  .d.d...|.D.....}
-00001dd0: 047c 047c 006a 086a 0d6b 047d 056e 0c7c  .|.|.j.j.k.}.n.|
-00001de0: 037d 0474 0ba0 0c64 0864 0784 007c 0344  .}.t...d.d...|.D
-00001df0: 0083 01a1 017d 0574 0364 0983 0101 007c  .....}.t.d.....|
-00001e00: 047c 0566 0253 0029 0a7a 1750 7265 6469  .|.f.S.).z.Predi
-00001e10: 6374 206f 6e20 756e 7365 656e 2064 6174  ct on unseen dat
-00001e20: 612e 7a33 3a20 5374 6172 7420 7072 6564  a.z3: Start pred
-00001e30: 6963 7469 6e67 206f 6e20 6e65 7720 6461  icting on new da
-00001e40: 7461 2075 7369 6e67 2058 6762 6f6f 7374  ta using Xgboost
-00001e50: 206d 6f64 656c 2e7a 1c2b 2b2b 2b2b 2b2b   model.z.+++++++
-00001e60: 2b2b 2b2b 2b2b 2b2b 2b2b 2b2b 2b2b 2b2b  ++++++++++++++++
-00001e70: 2b2b 2b2b 2b7a 204e 6f20 7472 6169 6e65  +++++z No traine
-00001e80: 6420 6d6f 6465 6c20 6861 7320 6265 656e  d model has been
-00001e90: 2066 6f75 6e64 2e7a 2b4e 6f20 6d6f 6465   found.z+No mode
-00001ea0: 6c20 636f 6e66 6967 7572 6174 696f 6e20  l configuration 
-00001eb0: 6669 6c65 2068 6173 2062 6565 6e20 666f  file has been fo
-00001ec0: 756e 642e 7211 0000 0063 0100 0000 0000  und.r....c......
-00001ed0: 0000 0000 0000 0200 0000 0400 0000 5300  ..............S.
-00001ee0: 0000 7314 0000 0067 007c 005d 067d 017c  ..s....g.|.].}.|
-00001ef0: 0164 0019 0091 0271 0253 0029 0172 2d00  .d.....q.S.).r-.
-00001f00: 0000 7218 0000 0072 5800 0000 7218 0000  ..r....rX...r...
-00001f10: 0072 1800 0000 7219 0000 0072 5b00 0000  .r....r....r[...
-00001f20: 3c01 0000 7302 0000 0014 007a 2858 6762  <...s......z(Xgb
-00001f30: 6f6f 7374 4d6f 6465 6c2e 7072 6564 6963  oostModel.predic
-00001f40: 742e 3c6c 6f63 616c 733e 2e3c 6c69 7374  t.<locals>.<list
-00001f50: 636f 6d70 3e63 0100 0000 0000 0000 0000  comp>c..........
-00001f60: 0000 0200 0000 0500 0000 5300 0000 7254  ..........S...rT
-00001f70: 0000 0072 1800 0000 7255 0000 0072 5800  ...r....rU...rX.
-00001f80: 0000 7218 0000 0072 1800 0000 7219 0000  ..r....r....r...
-00001f90: 0072 5b00 0000 4201 0000 725c 0000 007a  .r[...B...r\...z
-00001fa0: 1346 696e 6973 6865 6420 7072 6564 6963  .Finished predic
-00001fb0: 7469 6e67 290e 720d 0000 0072 0200 0000  ting).r....r....
-00001fc0: 721e 0000 0072 3500 0000 723a 0000 0072  r....r5...r:...r
-00001fd0: 3b00 0000 7216 0000 00da 0945 7863 6570  ;...r......Excep
-00001fe0: 7469 6f6e 7215 0000 0072 7e00 0000 7210  tionr....r~...r.
-00001ff0: 0000 0072 5600 0000 727f 0000 00da 1863  ...rV...r......c
-00002000: 6c61 7373 6966 6963 6174 696f 6e5f 7468  lassification_th
-00002010: 7265 7368 6f6c 6429 0672 1700 0000 7298  reshold).r....r.
-00002020: 0000 0072 3f00 0000 5a0d 7061 7274 6961  ...r?...Z.partia
-00002030: 6c5f 7072 6f62 735a 0f70 7265 6469 6374  l_probsZ.predict
-00002040: 6564 5f70 726f 6273 da11 7072 6564 6963  ed_probs..predic
-00002050: 7465 645f 636c 6173 7365 7372 1800 0000  ted_classesr....
-00002060: 7218 0000 0072 1900 0000 727e 0000 002d  r....r....r~...-
-00002070: 0100 0073 2400 0000 0202 0c01 04ff 0803  ...s$...........
-00002080: 0a01 0601 0801 0602 0801 0c02 0a01 1401  ................
-00002090: 0a02 04ff 0404 1401 0801 0801 7a14 5867  ............z.Xg
-000020a0: 626f 6f73 744d 6f64 656c 2e70 7265 6469  boostModel.predi
-000020b0: 6374 2903 4e4e 4e29 1ada 085f 5f6e 616d  ct).NNN)...__nam
-000020c0: 655f 5fda 0a5f 5f6d 6f64 756c 655f 5fda  e__..__module__.
-000020d0: 0c5f 5f71 7561 6c6e 616d 655f 5fda 075f  .__qualname__.._
-000020e0: 5f64 6f63 5f5f 7204 0000 0072 0500 0000  _doc__r....r....
-000020f0: 7209 0000 0072 0b00 0000 720a 0000 0072  r....r....r....r
-00002100: 1a00 0000 7237 0000 00da 0653 6572 6965  ....r7.....Serie
-00002110: 7372 0300 0000 da03 7374 72da 0566 6c6f  sr......str..flo
-00002120: 6174 7221 0000 0072 2200 0000 da09 4461  atr!...r".....Da
-00002130: 7461 4672 616d 6572 3a00 0000 da07 426f  taFramer:.....Bo
-00002140: 6f73 7465 7272 4100 0000 7234 0000 0072  osterrA...r4...r
-00002150: 0600 0000 7256 0000 00da 076e 6461 7272  ....rV.....ndarr
-00002160: 6179 727e 0000 0072 1800 0000 7218 0000  ayr~...r....r...
-00002170: 0072 1800 0000 7219 0000 0072 0f00 0000  .r....r....r....
-00002180: 1a00 0000 7350 0000 0008 0004 0102 0502  ....sP..........
-00002190: 0102 0104 fb06 0202 fe06 0302 fd06 0402  ................
-000021a0: fc06 050a fb1c 0d08 0802 1504 0202 fe04  ................
-000021b0: 0302 fd04 0402 fc04 0502 fb04 060a fa02  ................
-000021c0: 3704 0202 fe04 0302 fd04 0402 fc04 0502  7...............
-000021d0: fb02 060a fa00 7f24 3072 0f00 0000 291c  .......$0r....).
-000021e0: 729f 0000 0072 0200 0000 da06 7479 7069  r....r......typi
-000021f0: 6e67 7203 0000 0072 0400 0000 7205 0000  ngr....r....r...
-00002200: 0072 0600 0000 da05 6e75 6d70 7972 5600  .r......numpyrV.
-00002210: 0000 727d 0000 00da 0670 616e 6461 7372  ..r}.....pandasr
-00002220: 3700 0000 728a 0000 0072 3a00 0000 da0f  7...r....r:.....
-00002230: 736b 6c65 6172 6e2e 6d65 7472 6963 7372  sklearn.metricsr
-00002240: 0700 0000 da0d 736b 6c65 6172 6e2e 7574  ......sklearn.ut
-00002250: 696c 7372 0800 0000 da1f 626c 7565 6361  ilsr......blueca
-00002260: 7374 2e63 6f6e 6669 672e 7472 6169 6e69  st.config.traini
-00002270: 6e67 5f63 6f6e 6669 6772 0900 0000 720a  ng_configr....r.
-00002280: 0000 0072 0b00 0000 da24 626c 7565 6361  ...r.....$blueca
-00002290: 7374 2e67 656e 6572 616c 5f75 7469 6c73  st.general_utils
-000022a0: 2e67 656e 6572 616c 5f75 7469 6c73 720c  .general_utilsr.
-000022b0: 0000 0072 0d00 0000 da22 626c 7565 6361  ...r....."blueca
-000022c0: 7374 2e6d 6c5f 6d6f 6465 6c6c 696e 672e  st.ml_modelling.
-000022d0: 6261 7365 5f63 6c61 7373 6573 720e 0000  base_classesr...
-000022e0: 0072 0f00 0000 7218 0000 0072 1800 0000  .r....r....r....
-000022f0: 7218 0000 0072 1900 0000 da08 3c6d 6f64  r....r......<mod
-00002300: 756c 653e 0100 0000 731a 0000 0004 000c  ule>....s.......
-00002310: 0618 0108 0208 0108 0108 010c 010c 0114  ................
-00002320: 0210 050c 0114 03                        .......
+00000a40: 7c00 6a04 6a0d 725b 7c00 a00e 7c03 a101  |.j.j.r[|...|...
+00000a50: 7d05 740f 6a10 7c01 7c03 7c05 7c00 6a05  }.t.j.|.|.|.|.j.
+00000a60: 6a11 6406 8d04 7d06 6e0a 740f 6a10 7c01  j.d...}.n.t.j.|.
+00000a70: 7c03 7c00 6a05 6a11 6407 8d03 7d06 740f  |.|.j.j.d...}.t.
+00000a80: 6a10 7c02 7c04 7c00 6a05 6a11 6407 8d03  j.|.|.|.j.j.d...
+00000a90: 7d07 7c06 6408 6602 7c07 6409 6602 6702  }.|.d.f.|.d.f.g.
+00000aa0: 7d08 7c00 6a05 6a12 640a 6b02 7291 740f  }.|.j.j.d.k.r.t.
+00000ab0: 6a13 7c00 6a04 6a14 7c06 7c00 6a04 6a14  j.|.j.j.|.|.j.j.
+00000ac0: 640b 1900 7c00 6a05 6a15 7c08 640c 8d05  d...|.j.j.|.d...
+00000ad0: 7c00 5f16 6e13 740f 6a13 7c00 6a04 6a14  |._.n.t.j.|.j.j.
+00000ae0: 7c06 7c00 6a04 6a14 640b 1900 7c00 6a05  |.|.j.j.d...|.j.
+00000af0: 6a15 7c08 640c 8d05 7c00 5f16 7409 640d  j.|.d...|._.t.d.
+00000b00: 8301 0100 7c00 6a16 5300 290e 7a3f 5472  ....|.j.S.).z?Tr
+00000b10: 6169 6e20 5867 626f 6f73 7420 6d6f 6465  ain Xgboost mode
+00000b20: 6c2e 2049 6e63 6c75 6465 7320 6879 7065  l. Includes hype
+00000b30: 7270 6172 616d 6574 6572 2074 756e 696e  rparameter tunin
+00000b40: 6720 6f6e 2064 6566 6175 6c74 2e7a 1e3a  g on default.z.:
+00000b50: 2053 7461 7274 2066 6974 7469 6e67 2058   Start fitting X
+00000b60: 6762 6f6f 7374 206d 6f64 656c 2efa 2c63  gboost model..,c
+00000b70: 6f6e 665f 7061 7261 6d73 5f78 6762 6f6f  onf_params_xgboo
+00000b80: 7374 206f 7220 636f 6e66 5f74 7261 696e  st or conf_train
+00000b90: 696e 6720 6973 204e 6f6e 657a 1e46 696e  ing is Nonez.Fin
+00000ba0: 6973 6865 6420 6879 7065 7270 6172 616d  ished hyperparam
+00000bb0: 6574 6572 2074 756e 696e 677a 0e53 7461  eter tuningz.Sta
+00000bc0: 7274 2074 7261 696e 696e 677a 7f3a 2055  rt trainingz.: U
+00000bd0: 6e69 6f6e 2074 7261 696e 2061 6e64 2074  nion train and t
+00000be0: 6573 7420 6461 7461 2066 6f72 2066 696e  est data for fin
+00000bf0: 616c 206d 6f64 656c 2074 7261 696e 696e  al model trainin
+00000c00: 6720 6261 7365 6420 6f6e 2054 7261 696e  g based on Train
+00000c10: 696e 6743 6f6e 6669 670a 2020 2020 2020  ingConfig.      
+00000c20: 2020 2020 2020 2070 6172 616d 2027 7573         param 'us
+00000c30: 655f 6675 6c6c 5f64 6174 615f 666f 725f  e_full_data_for_
+00000c40: 6669 6e61 6c5f 6d6f 6465 6c27 a903 da05  final_model'....
+00000c50: 6c61 6265 6cda 0677 6569 6768 74da 1265  label..weight..e
+00000c60: 6e61 626c 655f 6361 7465 676f 7269 6361  nable_categorica
+00000c70: 6ca9 0272 2900 0000 722b 0000 00da 0574  l..r)...r+.....t
+00000c80: 7261 696e da04 7465 7374 e901 0000 00da  rain..test......
+00000c90: 0573 7465 7073 2903 da0f 6e75 6d5f 626f  .steps)...num_bo
+00000ca0: 6f73 745f 726f 756e 64da 1565 6172 6c79  ost_round..early
+00000cb0: 5f73 746f 7070 696e 675f 726f 756e 6473  _stopping_rounds
+00000cc0: da05 6576 616c 737a 1146 696e 6973 6865  ..evalsz.Finishe
+00000cd0: 6420 7472 6169 6e69 6e67 2917 720d 0000  d training).r...
+00000ce0: 0072 0200 0000 721e 0000 0072 2200 0000  .r....r....r"...
+00000cf0: 7215 0000 0072 1300 0000 da0a 5661 6c75  r....r......Valu
+00000d00: 6545 7272 6f72 da0e 6175 746f 7475 6e65  eError..autotune
+00000d10: 5f6d 6f64 656c da08 6175 746f 7475 6e65  _model..autotune
+00000d20: da05 7072 696e 74da 1d75 7365 5f66 756c  ..print..use_ful
+00000d30: 6c5f 6461 7461 5f66 6f72 5f66 696e 616c  l_data_for_final
+00000d40: 5f6d 6f64 656c da02 7064 da06 636f 6e63  _model..pd..conc
+00000d50: 6174 da0d 7361 6d70 6c65 5f77 6569 6768  at..sample_weigh
+00000d60: 7472 2100 0000 da03 7867 62da 0744 4d61  tr!.....xgb..DMa
+00000d70: 7472 6978 da1d 6361 745f 656e 636f 6469  trix..cat_encodi
+00000d80: 6e67 5f76 6961 5f6d 6c5f 616c 676f 7269  ng_via_ml_algori
+00000d90: 7468 6dda 1468 7970 6572 7475 6e69 6e67  thm..hypertuning
+00000da0: 5f63 765f 666f 6c64 7372 2d00 0000 da06  _cv_foldsr-.....
+00000db0: 7061 7261 6d73 7232 0000 0072 1600 0000  paramsr2...r....
+00000dc0: 2909 7217 0000 0072 2300 0000 7224 0000  ).r....r#...r$..
+00000dd0: 0072 2500 0000 7226 0000 0072 2000 0000  .r%...r&...r ...
+00000de0: da07 645f 7472 6169 6eda 0664 5f74 6573  ..d_train..d_tes
+00000df0: 74da 0865 7661 6c5f 7365 7472 1800 0000  t..eval_setr....
+00000e00: 7218 0000 0072 1900 0000 da03 6669 7447  r....r......fitG
+00000e10: 0000 0073 6400 0000 1208 0801 0c02 0801  ...sd...........
+00000e20: 0802 1001 0802 0802 0801 0201 0c01 04ff  ................
+00000e30: 0e04 0e01 0802 0a01 0401 0201 0201 0201  ................
+00000e40: 0601 08fc 0407 0201 0201 0601 06fd 0406  ................
+00000e50: 0201 0201 0601 06fd 1005 0c02 0401 0601  ................
+00000e60: 0201 0a01 0601 0201 0afb 0408 0601 0201  ................
+00000e70: 0a01 0601 0201 08fb 0807 0601 7a10 5867  ............z.Xg
+00000e80: 626f 6f73 744d 6f64 656c 2e66 6974 6305  boostModel.fitc.
+00000e90: 0000 0000 0000 0000 0000 000b 0000 000a  ................
+00000ea0: 0000 0003 0000 0073 e801 0000 7400 7401  .......s....t.t.
+00000eb0: a002 a100 9b00 6401 9d02 8301 0100 8801  ......d.........
+00000ec0: 6a03 720f 8801 6a04 7313 7405 6402 8301  j.r...j.s.t.d...
+00000ed0: 8201 7406 6a07 7c02 8804 8801 6a04 6a08  ..t.j.|.....j.j.
+00000ee0: 6403 8d03 8900 7409 8300 8902 8801 a00a  d.....t.........
+00000ef0: a100 0100 8801 6a03 722d 8801 6a04 722d  ......j.r-..j.r-
+00000f00: 8801 6a0b 7331 7405 6404 8301 8201 8700  ..j.s1t.d.......
+00000f10: 8701 8702 8703 8704 8705 6606 6405 6406  ..........f.d.d.
+00000f20: 8408 7d05 6407 7d06 740c 6a0d 6a0e 6408  ..}.d.}.t.j.j.d.
+00000f30: 8801 6a04 6a0f 6409 8d02 7d07 740c 6a10  ..j.j.d...}.t.j.
+00000f40: 640a 7c07 7c06 9b00 640b 9d02 640c 8d03  d.|.|...d...d...
+00000f50: 7d08 7c08 6a11 7c05 8801 6a04 6a12 8801  }.|.j.|...j.j...
+00000f60: 6a04 6a13 6408 6408 640d 8d05 0100 7a16  j.j.d.d.d.....z.
+00000f70: 740c 6a14 a015 7c08 a101 7d09 7c09 a016  t.j...|...}.|...
+00000f80: a100 0100 740c 6a14 a017 7c08 a101 7d09  ....t.j...|...}.
+00000f90: 7c09 a016 a100 0100 5700 6e0c 0400 7418  |.......W.n...t.
+00000fa0: 7419 7405 6603 7983 0100 0100 0100 5900  t.t.f.y.......Y.
+00000fb0: 6e01 7700 7c08 6a1a 6a1b 7d0a 6900 640e  n.w.|.j.j.}.i.d.
+00000fc0: 8801 6a0b 6a1c 9301 640f 8801 6a0b 6a1d  ..j.j...d...j.j.
+00000fd0: 9301 6410 8801 6a0b 6a1e 9301 6411 8802  ..d...j.j...d...
+00000fe0: 9301 6412 8805 a01f a100 9301 6413 7c0a  ..d.........d.|.
+00000ff0: 6413 1900 9301 6414 7c0a 6414 1900 9301  d.....d.|.d.....
+00001000: 6415 7c0a 6415 1900 9301 6416 7c0a 6416  d.|.d.....d.|.d.
+00001010: 1900 9301 6417 7c0a 6417 1900 9301 6418  ....d.|.d.....d.
+00001020: 7c0a 6418 1900 9301 6419 7c0a 6419 1900  |.d.....d.|.d...
+00001030: 9301 641a 7c0a 641a 1900 9301 641b 7c0a  ..d.|.d.....d.|.
+00001040: 641b 1900 9301 641c 7c0a 641c 1900 9301  d.....d.|.d.....
+00001050: 641d 8801 6a0b 6a20 9301 641e 7c0a 641e  d...j.j ..d.|.d.
+00001060: 1900 9301 641f 7c0a 641f 1900 6901 a501  ....d.|.d...i...
+00001070: 8801 6a03 5f1b 7421 6420 8801 6a03 6a1b  ..j._.t!d ..j.j.
+00001080: 8302 0100 7c0a 6421 1900 8801 6a03 5f22  ....|.d!....j._"
+00001090: 6422 5300 2923 7a7b 5475 6e65 2068 7970  d"S.)#z{Tune hyp
+000010a0: 6572 7061 7261 6d65 7465 7273 2e0a 0a20  erparameters... 
+000010b0: 2020 2020 2020 2041 6e20 616c 7465 726e         An altern
+000010c0: 6174 6976 6520 636f 6e66 6967 2063 616e  ative config can
+000010d0: 2062 6520 7072 6f76 6964 6564 2074 6f20   be provided to 
+000010e0: 6f76 6572 7772 6974 6520 7468 6520 6879  overwrite the hy
+000010f0: 7065 7270 6172 616d 6574 6572 2073 6561  perparameter sea
+00001100: 7263 6820 7370 6163 652e 0a20 2020 2020  rch space..     
+00001110: 2020 207a 2f3a 2053 7461 7274 2068 7970     z/: Start hyp
+00001120: 6572 7061 7261 6d65 7465 7220 7475 6e69  erparameter tuni
+00001130: 6e67 206f 6620 5867 626f 6f73 7420 6d6f  ng of Xgboost mo
+00001140: 6465 6c2e 7227 0000 0072 2c00 0000 7a39  del.r'...r,...z9
+00001150: 4174 206c 6561 7374 206f 6e65 206f 6620  At least one of 
+00001160: 7468 6520 636f 6e66 6967 7320 6973 204e  the configs is N
+00001170: 6f6e 652c 2077 6869 6368 2069 7320 6e6f  one, which is no
+00001180: 7420 616c 6c6f 7765 6463 0100 0000 0000  t allowedc......
+00001190: 0000 0000 0000 0c00 0000 0a00 0000 1300  ................
+000011a0: 0000 7362 0200 0069 0064 0188 016a 006a  ..sb...i.d...j.j
+000011b0: 0193 0164 0288 016a 006a 0293 0164 0388  ...d...j.j...d..
+000011c0: 016a 006a 0393 0164 0488 0293 0164 0588  .j.j...d.....d..
+000011d0: 05a0 04a1 0093 0164 067c 00a0 0564 0688  .......d.|...d..
+000011e0: 016a 006a 0688 016a 006a 07a1 0393 0164  .j.j...j.j.....d
+000011f0: 077c 00a0 0864 0788 016a 006a 0988 016a  .|...d...j.j...j
+00001200: 006a 0aa1 0393 0164 087c 00a0 0864 0888  .j.....d.|...d..
+00001210: 016a 006a 0b88 016a 006a 0ca1 0393 0164  .j.j...j.j.....d
+00001220: 097c 00a0 0864 0988 016a 006a 0d88 016a  .|...d...j.j...j
+00001230: 006a 0ea1 0393 0164 0a7c 00a0 0564 0a88  .j.....d.|...d..
+00001240: 016a 006a 0f88 016a 006a 10a1 0393 0164  .j.j...j.j.....d
+00001250: 0b7c 00a0 0864 0b88 016a 006a 1188 016a  .|...d...j.j...j
+00001260: 006a 12a1 0393 0164 0c7c 00a0 0864 0c88  .j.....d.|...d..
+00001270: 016a 006a 1388 016a 006a 14a1 0393 0164  .j.j...j.j.....d
+00001280: 0d7c 00a0 0864 0d88 016a 006a 1588 016a  .|...d...j.j...j
+00001290: 006a 16a1 0393 0164 0e7c 00a0 0864 0e88  .j.....d.|...d..
+000012a0: 016a 006a 1788 016a 006a 18a1 0393 0164  .j.j...j.j.....d
+000012b0: 0f7c 00a0 0564 0f88 016a 006a 1988 016a  .|...d...j.j...j
+000012c0: 006a 1aa1 0393 0164 1088 016a 006a 1b93  .j.....d...j.j..
+000012d0: 0164 117c 00a0 0564 1188 016a 006a 1c88  .d.|...d...j.j..
+000012e0: 016a 006a 1da1 0393 0164 127c 00a0 0564  .j.j.....d.|...d
+000012f0: 1288 016a 006a 1e88 016a 006a 1fa1 0369  ...j.j...j.j...i
+00001300: 01a5 017d 017c 00a0 2064 1364 1464 1567  ...}.|.. d.d.d.g
+00001310: 02a1 027d 027c 0272 ca88 01a0 2188 05a1  ...}.|.r....!...
+00001320: 017d 0374 226a 2388 0388 057c 0388 016a  .}.t"j#....|...j
+00001330: 246a 2564 168d 047d 046e 0a74 226a 2388  $j%d...}.n.t"j#.
+00001340: 0388 0588 016a 246a 2564 178d 037d 0474  .....j$j%d...}.t
+00001350: 266a 27a0 287c 0064 18a1 027d 0588 016a  &j'.(|.d...}...j
+00001360: 246a 2964 196b 0290 0172 157c 0464 1a66  $j)d.k...r.|.d.f
+00001370: 0288 0064 1b66 0267 027d 0674 226a 2a7c  ...d.f.g.}.t"j*|
+00001380: 017c 047c 0164 1119 0088 016a 246a 2b7c  .|.|.d.....j$j+|
+00001390: 067c 0567 0188 016a 006a 0364 1c8d 077d  .|.g...j.j.d...}
+000013a0: 077c 07a0 2c88 00a1 017d 0874 2da0 2e64  .|..,....}.t-..d
+000013b0: 1d64 1e84 007c 0844 0083 01a1 017d 0974  .d...|.D.....}.t
+000013c0: 2f88 047c 0983 0264 1f14 007d 0a7c 0a53  /..|...d...}.|.S
+000013d0: 0074 226a 307c 017c 047c 0164 1119 0088  .t"j0|.|.|.d....
+000013e0: 016a 246a 2964 1488 016a 246a 317c 0567  .j$j)d...j$j1|.g
+000013f0: 0188 016a 246a 3264 208d 087d 0b7c 0b64  ...j$j2d ..}.|.d
+00001400: 2119 00a0 33a1 0053 0029 224e da09 6f62  !...3..S.)"N..ob
+00001410: 6a65 6374 6976 65da 0b65 7661 6c5f 6d65  jective..eval_me
+00001420: 7472 6963 da07 7665 7262 6f73 65da 0b74  tric..verbose..t
+00001430: 7265 655f 6d65 7468 6f64 da09 6e75 6d5f  ree_method..num_
+00001440: 636c 6173 73da 096d 6178 5f64 6570 7468  class..max_depth
+00001450: da05 616c 7068 61da 066c 616d 6264 61da  ..alpha..lambda.
+00001460: 0567 616d 6d61 da0a 6e75 6d5f 6c65 6176  .gamma..num_leav
+00001470: 6573 da09 7375 6273 616d 706c 65da 1063  es..subsample..c
+00001480: 6f6c 7361 6d70 6c65 5f62 7974 7265 65da  olsample_bytree.
+00001490: 1163 6f6c 7361 6d70 6c65 5f62 796c 6576  .colsample_bylev
+000014a0: 656c da10 636f 6c73 616d 706c 655f 6279  el..colsample_by
+000014b0: 6e6f 6465 da11 6d69 6e5f 6368 696c 645f  node..min_child_
+000014c0: 7361 6d70 6c65 73da 0365 7461 7230 0000  samples..etar0..
+000014d0: 00da 116e 756d 5f70 6172 616c 6c65 6c5f  ...num_parallel_
+000014e0: 7472 6565 723b 0000 0054 4672 2800 0000  treer;...TFr(...
+000014f0: 722c 0000 007a 0d74 6573 742d 6d6c 6f67  r,...z.test-mlog
+00001500: 6c6f 7373 722f 0000 0072 2d00 0000 722e  lossr/...r-...r.
+00001510: 0000 0029 0572 3100 0000 7232 0000 0072  ...).r1...r2...r
+00001520: 3300 0000 da09 6361 6c6c 6261 636b 73da  3.....callbacks.
+00001530: 0c76 6572 626f 7365 5f65 7661 6c63 0100  .verbose_evalc..
+00001540: 0000 0000 0000 0000 0000 0200 0000 0500  ................
+00001550: 0000 5300 0000 f316 0000 0067 007c 005d  ..S........g.|.]
+00001560: 077d 0174 00a0 017c 01a1 0191 0271 0253  .}.t...|.....q.S
+00001570: 0072 1800 0000 a902 da02 6e70 da06 6172  .r........np..ar
+00001580: 676d 6178 a902 da02 2e30 da04 6c69 6e65  gmax.....0..line
+00001590: 7218 0000 0072 1800 0000 7219 0000 00da  r....r....r.....
+000015a0: 0a3c 6c69 7374 636f 6d70 3e0a 0100 00f3  .<listcomp>.....
+000015b0: 0200 0000 1600 7a3c 5867 626f 6f73 744d  ......z<XgboostM
+000015c0: 6f64 656c 2e61 7574 6f74 756e 652e 3c6c  odel.autotune.<l
+000015d0: 6f63 616c 733e 2e6f 626a 6563 7469 7665  ocals>.objective
+000015e0: 2e3c 6c6f 6361 6c73 3e2e 3c6c 6973 7463  .<locals>.<listc
+000015f0: 6f6d 703e e9ff ffff ff29 0872 4000 0000  omp>.....).r@...
+00001600: da06 6474 7261 696e 7231 0000 00da 056e  ..dtrainr1.....n
+00001610: 666f 6c64 da09 6173 5f70 616e 6461 73da  fold..as_pandas.
+00001620: 0473 6565 6472 5600 0000 da07 7368 7566  .seedrV.....shuf
+00001630: 666c 657a 1274 6573 742d 6d6c 6f67 6c6f  flez.test-mloglo
+00001640: 7373 2d6d 6561 6e29 3472 1400 0000 da0f  ss-mean)4r......
+00001650: 6d6f 6465 6c5f 6f62 6a65 6374 6976 65da  model_objective.
+00001660: 116d 6f64 656c 5f65 7661 6c5f 6d65 7472  .model_eval_metr
+00001670: 6963 da0f 6d6f 6465 6c5f 7665 7262 6f73  ic..model_verbos
+00001680: 6974 79da 076e 756e 6971 7565 5a0b 7375  ity..nuniqueZ.su
+00001690: 6767 6573 745f 696e 74da 0d6d 6178 5f64  ggest_int..max_d
+000016a0: 6570 7468 5f6d 696e da0d 6d61 785f 6465  epth_min..max_de
+000016b0: 7074 685f 6d61 785a 0d73 7567 6765 7374  pth_maxZ.suggest
+000016c0: 5f66 6c6f 6174 da09 616c 7068 615f 6d69  _float..alpha_mi
+000016d0: 6eda 0961 6c70 6861 5f6d 6178 da0a 6c61  n..alpha_max..la
+000016e0: 6d62 6461 5f6d 696e da0a 6c61 6d62 6461  mbda_min..lambda
+000016f0: 5f6d 6178 da09 6761 6d6d 615f 6d69 6eda  _max..gamma_min.
+00001700: 0967 616d 6d61 5f6d 6178 da0e 6e75 6d5f  .gamma_max..num_
+00001710: 6c65 6176 6573 5f6d 696e da0e 6e75 6d5f  leaves_min..num_
+00001720: 6c65 6176 6573 5f6d 6178 da0e 7375 625f  leaves_max..sub_
+00001730: 7361 6d70 6c65 5f6d 696e da0e 7375 625f  sample_min..sub_
+00001740: 7361 6d70 6c65 5f6d 6178 da16 636f 6c5f  sample_max..col_
+00001750: 7361 6d70 6c65 5f62 795f 7472 6565 5f6d  sample_by_tree_m
+00001760: 696e da16 636f 6c5f 7361 6d70 6c65 5f62  in..col_sample_b
+00001770: 795f 7472 6565 5f6d 6178 da17 636f 6c5f  y_tree_max..col_
+00001780: 7361 6d70 6c65 5f62 795f 6c65 7665 6c5f  sample_by_level_
+00001790: 6d69 6eda 1763 6f6c 5f73 616d 706c 655f  min..col_sample_
+000017a0: 6279 5f6c 6576 656c 5f6d 6178 da16 636f  by_level_max..co
+000017b0: 6c5f 7361 6d70 6c65 5f62 795f 6e6f 6465  l_sample_by_node
+000017c0: 5f6d 696e da16 636f 6c5f 7361 6d70 6c65  _min..col_sample
+000017d0: 5f62 795f 6e6f 6465 5f6d 6178 da15 6d69  _by_node_max..mi
+000017e0: 6e5f 6368 696c 645f 7361 6d70 6c65 735f  n_child_samples_
+000017f0: 6d69 6eda 156d 696e 5f63 6869 6c64 5f73  min..min_child_s
+00001800: 616d 706c 6573 5f6d 6178 7254 0000 00da  amples_maxrT....
+00001810: 0973 7465 7073 5f6d 696e da09 7374 6570  .steps_min..step
+00001820: 735f 6d61 78da 156e 756d 5f70 6172 616c  s_max..num_paral
+00001830: 6c65 6c5f 7472 6565 5f6d 696e da15 6e75  lel_tree_min..nu
+00001840: 6d5f 7061 7261 6c6c 656c 5f74 7265 655f  m_parallel_tree_
+00001850: 6d61 785a 1373 7567 6765 7374 5f63 6174  maxZ.suggest_cat
+00001860: 6567 6f72 6963 616c 7221 0000 0072 3c00  egoricalr!...r<.
+00001870: 0000 723d 0000 0072 1300 0000 723e 0000  ..r=...r....r>..
+00001880: 00da 066f 7074 756e 615a 0b69 6e74 6567  ...optunaZ.integ
+00001890: 7261 7469 6f6e 5a16 5847 426f 6f73 7450  rationZ.XGBoostP
+000018a0: 7275 6e69 6e67 4361 6c6c 6261 636b 723f  runingCallbackr?
+000018b0: 0000 0072 2d00 0000 7232 0000 00da 0770  ...r-...r2.....p
+000018c0: 7265 6469 6374 725a 0000 00da 0761 7361  redictrZ.....asa
+000018d0: 7272 6179 7207 0000 00da 0263 76da 1367  rrayr......cv..g
+000018e0: 6c6f 6261 6c5f 7261 6e64 6f6d 5f73 7461  lobal_random_sta
+000018f0: 7465 da17 7368 7566 666c 655f 6475 7269  te..shuffle_duri
+00001900: 6e67 5f74 7261 696e 696e 67da 046d 6561  ng_training..mea
+00001910: 6e29 0cda 0574 7269 616c da05 7061 7261  n)...trial..para
+00001920: 6d72 3b00 0000 7220 0000 0072 4100 0000  mr;...r ...rA...
+00001930: 5a10 7072 756e 696e 675f 6361 6c6c 6261  Z.pruning_callba
+00001940: 636b 7243 0000 0072 1600 0000 da05 7072  ckrC...r......pr
+00001950: 6564 73da 0b70 7265 645f 6c61 6265 6c73  eds..pred_labels
+00001960: 5a07 6d61 7474 6865 77da 0672 6573 756c  Z.matthew..resul
+00001970: 74a9 0672 4200 0000 7217 0000 005a 0874  t..rB...r....Z.t
+00001980: 7261 696e 5f6f 6e72 2300 0000 7226 0000  rain_onr#...r&..
+00001990: 0072 2500 0000 7218 0000 0072 1900 0000  .r%...r....r....
+000019a0: 7245 0000 00ad 0000 0073 f000 0000 0201  rE.......s......
+000019b0: 0801 02ff 0802 02fe 0803 02fd 0404 02fc  ................
+000019c0: 0805 02fb 0606 0201 0601 0601 02fd 02fa  ................
+000019d0: 060b 0e01 02ff 02f5 060e 0e01 02ff 02f2  ................
+000019e0: 0611 0e01 02ff 02ef 0614 0201 0601 0601  ................
+000019f0: 02fd 02ec 0619 0201 0601 0601 02fd 02e7  ................
+00001a00: 061e 0201 0601 0601 02fd 02e2 0623 0201  .............#..
+00001a10: 0601 0601 02fd 02dd 0628 0201 0601 0601  .........(......
+00001a20: 02fd 02d8 062d 0201 0601 0601 02fd 02d3  .....-..........
+00001a30: 0832 02ce 0633 0e01 02ff 02cd 0636 0201  .2...3.......6..
+00001a40: 0601 0601 02fd 06ca 103c 0401 0a01 0401  .........<......
+00001a50: 0201 0201 0201 0601 08fc 0407 0201 0201  ................
+00001a60: 0601 06fd 0606 0401 04ff 0e04 1001 0401  ................
+00001a70: 0201 0201 0601 0601 0201 0401 0601 06f9  ................
+00001a80: 0a09 1401 0e01 0401 0402 0201 0201 0601  ................
+00001a90: 0602 0201 0601 0401 0601 06f7 0c0c 7a28  ..............z(
+00001aa0: 5867 626f 6f73 744d 6f64 656c 2e61 7574  XgboostModel.aut
+00001ab0: 6f74 756e 652e 3c6c 6f63 616c 733e 2e6f  otune.<locals>.o
+00001ac0: 626a 6563 7469 7665 da07 7867 626f 6f73  bjective..xgboos
+00001ad0: 7454 2902 5a0c 6d75 6c74 6976 6172 6961  tT).Z.multivaria
+00001ae0: 7465 7265 0000 00da 086d 696e 696d 697a  tere.....minimiz
+00001af0: 657a 0720 7475 6e69 6e67 2903 da09 6469  ez. tuning)...di
+00001b00: 7265 6374 696f 6eda 0773 616d 706c 6572  rection..sampler
+00001b10: 5a0a 7374 7564 795f 6e61 6d65 2904 da08  Z.study_name)...
+00001b20: 6e5f 7472 6961 6c73 da07 7469 6d65 6f75  n_trials..timeou
+00001b30: 745a 0e67 635f 6166 7465 725f 7472 6961  tZ.gc_after_tria
+00001b40: 6c5a 1173 686f 775f 7072 6f67 7265 7373  lZ.show_progress
+00001b50: 5f62 6172 7245 0000 0072 4600 0000 7247  _barrE...rF...rG
+00001b60: 0000 0072 4800 0000 7249 0000 0072 4a00  ...rH...rI...rJ.
+00001b70: 0000 724b 0000 0072 4c00 0000 724d 0000  ..rK...rL...rM..
+00001b80: 0072 4e00 0000 724f 0000 0072 5000 0000  .rN...rO...rP...
+00001b90: 7251 0000 0072 5200 0000 7253 0000 0072  rQ...rR...rS...r
+00001ba0: 5400 0000 7230 0000 0072 5500 0000 7a0d  T...r0...rU...z.
+00001bb0: 4265 7374 2070 6172 616d 733a 2072 3b00  Best params: r;.
+00001bc0: 0000 4e29 2372 0d00 0000 7202 0000 0072  ..N)#r....r....r
+00001bd0: 1e00 0000 7215 0000 0072 1300 0000 7234  ....r....r....r4
+00001be0: 0000 0072 3c00 0000 723d 0000 0072 3e00  ...r<...r=...r>.
+00001bf0: 0000 720c 0000 0072 2200 0000 7214 0000  ..r....r"...r...
+00001c00: 0072 8300 0000 5a08 7361 6d70 6c65 7273  .r....Z.samplers
+00001c10: 5a0a 5450 4553 616d 706c 6572 7287 0000  Z.TPESamplerr...
+00001c20: 005a 0c63 7265 6174 655f 7374 7564 79da  .Z.create_study.
+00001c30: 086f 7074 696d 697a 65da 1c68 7970 6572  .optimize..hyper
+00001c40: 7061 7261 6d65 7465 725f 7475 6e69 6e67  parameter_tuning
+00001c50: 5f72 6f75 6e64 73da 2668 7970 6572 7061  _rounds.&hyperpa
+00001c60: 7261 6d65 7465 725f 7475 6e69 6e67 5f6d  rameter_tuning_m
+00001c70: 6178 5f72 756e 7469 6d65 5f73 6563 735a  ax_runtime_secsZ
+00001c80: 0d76 6973 7561 6c69 7a61 7469 6f6e 5a19  .visualizationZ.
+00001c90: 706c 6f74 5f6f 7074 696d 697a 6174 696f  plot_optimizatio
+00001ca0: 6e5f 6869 7374 6f72 79da 0473 686f 775a  n_history..showZ
+00001cb0: 1670 6c6f 745f 7061 7261 6d5f 696d 706f  .plot_param_impo
+00001cc0: 7274 616e 6365 73da 115a 6572 6f44 6976  rtances..ZeroDiv
+00001cd0: 6973 696f 6e45 7272 6f72 da0c 5275 6e74  isionError..Runt
+00001ce0: 696d 6545 7272 6f72 5a0a 6265 7374 5f74  imeErrorZ.best_t
+00001cf0: 7269 616c 7240 0000 0072 6700 0000 7268  rialr@...rg...rh
+00001d00: 0000 0072 6900 0000 726a 0000 0072 5400  ...ri...rj...rT.
+00001d10: 0000 7237 0000 0072 3b00 0000 290b 7217  ..r7...r;...).r.
+00001d20: 0000 0072 2300 0000 7224 0000 0072 2500  ...r#...r$...r%.
+00001d30: 0000 7226 0000 0072 4500 0000 da09 616c  ..r&...rE.....al
+00001d40: 676f 7269 7468 6d72 9300 0000 5a05 7374  gorithmr....Z.st
+00001d50: 7564 79da 0366 6967 5a12 7867 626f 6f73  udy..figZ.xgboos
+00001d60: 745f 6265 7374 5f70 6172 616d 7218 0000  t_best_paramr...
+00001d70: 0072 8f00 0000 7219 0000 0072 3600 0000  .r....r....r6...
+00001d80: 8c00 0000 73ac 0000 0012 0b0c 0108 0104  ....s...........
+00001d90: 0202 0102 0106 0106 fd06 0508 0204 0302  ................
+00001da0: ff04 0202 fe04 0302 fd02 0502 0104 ff16  ................
+00001db0: 0404 6f06 0108 0106 ff04 0302 0102 0108  ..o.............
+00001dc0: 0106 fd04 0602 0106 0106 0102 0102 0106  ................
+00001dd0: fb02 070c 0108 010c 010c 0112 0104 0102  ................
+00001de0: ff08 0302 0108 0102 ff08 0202 fe08 0302  ................
+00001df0: fd04 0402 fc08 0502 fb04 0602 0102 ff02  ................
+00001e00: fa08 0902 f708 0a02 f608 0b02 f508 0c02  ................
+00001e10: f408 0d02 f308 0e02 f208 0f02 f108 1002  ................
+00001e20: f008 1102 ef08 1202 ee08 1302 ed08 140a  ................
+00001e30: ec0e 1610 017a 1558 6762 6f6f 7374 4d6f  .....z.XgboostMo
+00001e40: 6465 6c2e 6175 746f 7475 6e65 da02 6466  del.autotune..df
+00001e50: 6302 0000 0000 0000 0000 0000 0006 0000  c...............
+00001e60: 0004 0000 0043 0000 0073 b400 0000 7400  .....C...s....t.
+00001e70: 7401 a002 a100 9b00 6401 9d02 8301 0100  t.......d.......
+00001e80: 7c00 6a03 720f 7c00 6a04 7313 7405 6402  |.j.r.|.j.s.t.d.
+00001e90: 8301 8201 7406 6a07 7c01 7c00 6a04 6a08  ....t.j.|.|.j.j.
+00001ea0: 6403 8d02 7d02 7c00 6a09 7323 740a 6404  d...}.|.j.s#t.d.
+00001eb0: 8301 8201 7c00 6a0b 732a 740a 6405 8301  ....|.j.s*t.d...
+00001ec0: 8201 7c00 6a09 a00c 7c02 a101 7d03 7c00  ..|.j...|...}.|.
+00001ed0: 6a0d 6406 6b02 7246 740e a00f 6407 6408  j.d.k.rFt...d.d.
+00001ee0: 8400 7c03 4400 8301 a101 7d04 7c04 7c00  ..|.D.....}.|.|.
+00001ef0: 6a0b 6a10 6b04 7d05 6e0c 7c03 7d04 740e  j.j.k.}.n.|.}.t.
+00001f00: a00f 6409 6408 8400 7c03 4400 8301 a101  ..d.d...|.D.....
+00001f10: 7d05 7411 640a 8301 0100 7c04 7c05 6602  }.t.d.....|.|.f.
+00001f20: 5300 290b 7a17 5072 6564 6963 7420 6f6e  S.).z.Predict on
+00001f30: 2075 6e73 6565 6e20 6461 7461 2e7a 333a   unseen data.z3:
+00001f40: 2053 7461 7274 2070 7265 6469 6374 696e   Start predictin
+00001f50: 6720 6f6e 206e 6577 2064 6174 6120 7573  g on new data us
+00001f60: 696e 6720 5867 626f 6f73 7420 6d6f 6465  ing Xgboost mode
+00001f70: 6c2e 7227 0000 0029 0172 2b00 0000 7a20  l.r'...).r+...z 
+00001f80: 4e6f 2074 7261 696e 6564 206d 6f64 656c  No trained model
+00001f90: 2068 6173 2062 6565 6e20 666f 756e 642e   has been found.
+00001fa0: 7a2b 4e6f 206d 6f64 656c 2063 6f6e 6669  z+No model confi
+00001fb0: 6775 7261 7469 6f6e 2066 696c 6520 6861  guration file ha
+00001fc0: 7320 6265 656e 2066 6f75 6e64 2e72 1100  s been found.r..
+00001fd0: 0000 6301 0000 0000 0000 0000 0000 0002  ..c.............
+00001fe0: 0000 0004 0000 0053 0000 0073 1400 0000  .......S...s....
+00001ff0: 6700 7c00 5d06 7d01 7c01 6400 1900 9102  g.|.].}.|.d.....
+00002000: 7102 5300 2901 722f 0000 0072 1800 0000  q.S.).r/...r....
+00002010: 725c 0000 0072 1800 0000 7218 0000 0072  r\...r....r....r
+00002020: 1900 0000 725f 0000 0064 0100 0073 0200  ....r_...d...s..
+00002030: 0000 1400 7a28 5867 626f 6f73 744d 6f64  ....z(XgboostMod
+00002040: 656c 2e70 7265 6469 6374 2e3c 6c6f 6361  el.predict.<loca
+00002050: 6c73 3e2e 3c6c 6973 7463 6f6d 703e 6301  ls>.<listcomp>c.
+00002060: 0000 0000 0000 0000 0000 0002 0000 0005  ................
+00002070: 0000 0053 0000 0072 5800 0000 7218 0000  ...S...rX...r...
+00002080: 0072 5900 0000 725c 0000 0072 1800 0000  .rY...r\...r....
+00002090: 7218 0000 0072 1900 0000 725f 0000 006a  r....r....r_...j
+000020a0: 0100 0072 6000 0000 7a13 4669 6e69 7368  ...r`...z.Finish
+000020b0: 6564 2070 7265 6469 6374 696e 6729 1272  ed predicting).r
+000020c0: 0d00 0000 7202 0000 0072 1e00 0000 7214  ....r....r....r.
+000020d0: 0000 0072 1300 0000 7234 0000 0072 3c00  ...r....r4...r<.
+000020e0: 0000 723d 0000 0072 3e00 0000 7216 0000  ..r=...r>...r...
+000020f0: 00da 0945 7863 6570 7469 6f6e 7215 0000  ...Exceptionr...
+00002100: 0072 8400 0000 7210 0000 0072 5a00 0000  .r....r....rZ...
+00002110: 7285 0000 00da 1863 6c61 7373 6966 6963  r......classific
+00002120: 6174 696f 6e5f 7468 7265 7368 6f6c 6472  ation_thresholdr
+00002130: 3700 0000 2906 7217 0000 0072 9e00 0000  7...).r....r....
+00002140: 7242 0000 005a 0d70 6172 7469 616c 5f70  rB...Z.partial_p
+00002150: 726f 6273 5a0f 7072 6564 6963 7465 645f  robsZ.predicted_
+00002160: 7072 6f62 73da 1170 7265 6469 6374 6564  probs..predicted
+00002170: 5f63 6c61 7373 6573 7218 0000 0072 1800  _classesr....r..
+00002180: 0000 7219 0000 0072 8400 0000 4f01 0000  ..r....r....O...
+00002190: 732c 0000 0002 020c 0104 ff0c 0308 0104  s,..............
+000021a0: 0202 0106 0106 fe06 0508 0106 0208 010c  ................
+000021b0: 020a 0114 010a 0204 ff04 0414 0108 0108  ................
+000021c0: 017a 1458 6762 6f6f 7374 4d6f 6465 6c2e  .z.XgboostModel.
+000021d0: 7072 6564 6963 7429 034e 4e4e 291a da08  predict).NNN)...
+000021e0: 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f 6475  __name__..__modu
+000021f0: 6c65 5f5f da0c 5f5f 7175 616c 6e61 6d65  le__..__qualname
+00002200: 5f5f da07 5f5f 646f 635f 5f72 0400 0000  __..__doc__r....
+00002210: 7205 0000 0072 0900 0000 720b 0000 0072  r....r....r....r
+00002220: 0a00 0000 721a 0000 0072 3900 0000 da06  ....r....r9.....
+00002230: 5365 7269 6573 7203 0000 00da 0373 7472  Seriesr......str
+00002240: da05 666c 6f61 7472 2100 0000 7222 0000  ..floatr!...r"..
+00002250: 00da 0944 6174 6146 7261 6d65 723c 0000  ...DataFramer<..
+00002260: 00da 0742 6f6f 7374 6572 7244 0000 0072  ...BoosterrD...r
+00002270: 3600 0000 7206 0000 0072 5a00 0000 da07  6...r....rZ.....
+00002280: 6e64 6172 7261 7972 8400 0000 7218 0000  ndarrayr....r...
+00002290: 0072 1800 0000 7218 0000 0072 1900 0000  .r....r....r....
+000022a0: 720f 0000 001a 0000 0073 5000 0000 0800  r........sP.....
+000022b0: 0401 0205 0201 0201 04fb 0602 02fe 0603  ................
+000022c0: 02fd 0604 02fc 0605 0afb 1c0d 0808 0215  ................
+000022d0: 0402 02fe 0403 02fd 0404 02fc 0405 02fb  ................
+000022e0: 0406 0afa 0245 0402 02fe 0403 02fd 0404  .....E..........
+000022f0: 02fc 0405 02fb 0206 0afa 007f 2444 720f  ............$Dr.
+00002300: 0000 0029 1c72 a500 0000 7202 0000 00da  ...).r....r.....
+00002310: 0674 7970 696e 6772 0300 0000 7204 0000  .typingr....r...
+00002320: 0072 0500 0000 7206 0000 00da 056e 756d  .r....r......num
+00002330: 7079 725a 0000 0072 8300 0000 da06 7061  pyrZ...r......pa
+00002340: 6e64 6173 7239 0000 0072 9000 0000 723c  ndasr9...r....r<
+00002350: 0000 00da 0f73 6b6c 6561 726e 2e6d 6574  .....sklearn.met
+00002360: 7269 6373 7207 0000 00da 0d73 6b6c 6561  ricsr......sklea
+00002370: 726e 2e75 7469 6c73 7208 0000 00da 1f62  rn.utilsr......b
+00002380: 6c75 6563 6173 742e 636f 6e66 6967 2e74  luecast.config.t
+00002390: 7261 696e 696e 675f 636f 6e66 6967 7209  raining_configr.
+000023a0: 0000 0072 0a00 0000 720b 0000 00da 2462  ...r....r.....$b
+000023b0: 6c75 6563 6173 742e 6765 6e65 7261 6c5f  luecast.general_
+000023c0: 7574 696c 732e 6765 6e65 7261 6c5f 7574  utils.general_ut
+000023d0: 696c 7372 0c00 0000 720d 0000 00da 2262  ilsr....r....."b
+000023e0: 6c75 6563 6173 742e 6d6c 5f6d 6f64 656c  luecast.ml_model
+000023f0: 6c69 6e67 2e62 6173 655f 636c 6173 7365  ling.base_classe
+00002400: 7372 0e00 0000 720f 0000 0072 1800 0000  sr....r....r....
+00002410: 7218 0000 0072 1800 0000 7219 0000 00da  r....r....r.....
+00002420: 083c 6d6f 6475 6c65 3e01 0000 0073 1a00  .<module>....s..
+00002430: 0000 0400 0c06 1801 0802 0801 0801 0801  ................
+00002440: 0c01 0c01 1402 1005 0c01 1403            ............
```

### Comparing `bluecast-0.5/bluecast/ml_modelling/__pycache__/xgboost.cpython-38.pyc` & `bluecast-0.7/bluecast/ml_modelling/__pycache__/xgboost.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Thu Jun  8 04:28:32 2023 UTC, .py size: 12460 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 f058 8164 ac30 0000  U........X.d.0..
+00000000: 550d 0d0a 0000 0000 b69d 9d64 1b37 0000  U..........d.7..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 a400 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d01 5a01 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c02 6d03 5a03 6d04 5a04 6d05 5a05  d.l.m.Z.m.Z.m.Z.
 00000050: 6d06 5a06 0100 6401 6404 6c07 5a08 6401  m.Z...d.d.l.Z.d.
 00000060: 6404 6c09 5a09 6401 6404 6c0a 5a0b 6401  d.l.Z.d.d.l.Z.d.
 00000070: 6404 6c0c 5a0d 6401 6405 6c0e 6d0f 5a0f  d.l.Z.d.d.l.m.Z.
@@ -101,418 +101,457 @@
 00000640: 0000 da17 6361 6c63 756c 6174 655f 636c  ....calculate_cl
 00000650: 6173 735f 7765 6967 6874 732a 0000 0073  ass_weights*...s
 00000660: 0c00 0000 0002 1201 0401 0200 02ff 0603  ................
 00000670: 7a24 5867 626f 6f73 744d 6f64 656c 2e63  z$XgboostModel.c
 00000680: 616c 6375 6c61 7465 5f63 6c61 7373 5f77  alculate_class_w
 00000690: 6569 6768 7473 6301 0000 0000 0000 0000  eightsc.........
 000006a0: 0000 0001 0000 0003 0000 0043 0000 0073  ...........C...s
-000006b0: 7600 0000 7400 7401 a002 a100 9b00 6401  v...t.t.......d.
-000006c0: 9d02 8301 0100 7c00 6a03 7332 7404 8300  ......|.j.s2t...
+000006b0: b200 0000 7400 7401 a002 a100 9b00 6401  ....t.t.......d.
+000006c0: 9d02 8301 0100 7c00 6a03 7334 7404 8300  ......|.j.s4t...
 000006d0: 7c00 5f03 7400 7401 a002 a100 9b00 6402  |._.t.t.......d.
-000006e0: 9d02 8301 0100 7c00 6a05 7352 7406 8300  ......|.j.sRt...
-000006f0: 7c00 5f05 7400 7401 a002 a100 9b00 6403  |._.t.t.......d.
-00000700: 9d02 8301 0100 7c00 6a07 7372 7408 8300  ......|.j.srt...
-00000710: 7c00 5f07 7400 7401 a002 a100 9b00 6404  |._.t.t.......d.
-00000720: 9d02 8301 0100 6405 5300 2906 7a36 4c6f  ......d.S.).z6Lo
-00000730: 6164 206d 756c 7469 706c 6520 636f 6e66  ad multiple conf
-00000740: 6967 7320 6f72 206c 6f61 6420 6465 6661  igs or load defa
-00000750: 756c 7420 636f 6e66 6967 7320 696e 7374  ult configs inst
-00000760: 6561 642e 7a32 3a20 5374 6172 7420 6c6f  ead.z2: Start lo
-00000770: 6164 696e 6720 6578 6973 7469 6e67 206f  ading existing o
-00000780: 7220 6465 6661 756c 7420 636f 6e66 6967  r default config
-00000790: 2066 696c 6573 2e2e 7a1e 3a20 4c6f 6164   files..z.: Load
-000007a0: 2064 6566 6175 6c74 2054 7261 696e 696e   default Trainin
-000007b0: 6743 6f6e 6669 672e 7a27 3a20 4c6f 6164  gConfig.z': Load
-000007c0: 2064 6566 6175 6c74 2058 6762 6f6f 7374   default Xgboost
-000007d0: 5475 6e65 5061 7261 6d73 436f 6e66 6967  TuneParamsConfig
-000007e0: 2e7a 273a 204c 6f61 6420 6465 6661 756c  .z': Load defaul
-000007f0: 7420 5867 626f 6f73 7446 696e 616c 5061  t XgboostFinalPa
-00000800: 7261 6d43 6f6e 6669 672e 4e29 0972 0d00  ramConfig.N).r..
-00000810: 0000 7202 0000 0072 1e00 0000 7213 0000  ..r....r....r...
-00000820: 0072 0900 0000 7214 0000 0072 0b00 0000  .r....r....r....
-00000830: 7215 0000 0072 0a00 0000 2901 7217 0000  r....r....).r...
-00000840: 0072 1800 0000 7218 0000 0072 1900 0000  .r....r....r....
-00000850: da10 6368 6563 6b5f 6c6f 6164 5f63 6f6e  ..check_load_con
-00000860: 6673 3200 0000 7314 0000 0000 0212 0106  fs2...s.........
-00000870: 0108 0112 0206 0108 0112 0206 0108 017a  ...............z
-00000880: 1d58 6762 6f6f 7374 4d6f 6465 6c2e 6368  .XgboostModel.ch
-00000890: 6563 6b5f 6c6f 6164 5f63 6f6e 6673 2905  eck_load_confs).
-000008a0: da07 785f 7472 6169 6eda 0678 5f74 6573  ..x_train..x_tes
-000008b0: 74da 0779 5f74 7261 696e da06 795f 7465  t..y_train..y_te
-000008c0: 7374 721c 0000 0063 0500 0000 0000 0000  str....c........
-000008d0: 0000 0000 0900 0000 0700 0000 4300 0000  ............C...
-000008e0: 73d2 0000 0074 0074 01a0 02a1 009b 0064  s....t.t.......d
-000008f0: 019d 0283 0101 007c 00a0 03a1 0001 007c  .......|.......|
-00000900: 006a 0472 267c 006a 0573 2e74 0664 0283  .j.r&|.j.s.t.d..
-00000910: 0182 017c 006a 056a 0772 467c 00a0 087c  ...|.j.j.rF|...|
-00000920: 017c 027c 037c 04a1 0401 0074 0964 0383  .|.|.|.....t.d..
-00000930: 0101 007c 006a 046a 0a72 727c 00a0 0b7c  ...|.j.j.rr|...|
-00000940: 03a1 017d 0574 0c6a 0d7c 017c 037c 0564  ...}.t.j.|.|.|.d
-00000950: 048d 037d 066e 0e74 0c6a 0d7c 017c 0364  ...}.n.t.j.|.|.d
-00000960: 058d 027d 0674 0c6a 0d7c 027c 0464 058d  ...}.t.j.|.|.d..
-00000970: 027d 077c 0664 0666 027c 0764 0766 0267  .}.|.d.f.|.d.f.g
-00000980: 027d 0874 0c6a 0e7c 006a 046a 0f7c 067c  .}.t.j.|.j.j.|.|
-00000990: 006a 046a 0f64 0819 007c 006a 056a 107c  .j.j.d...|.j.j.|
-000009a0: 0864 098d 057c 005f 1174 0964 0a83 0101  .d...|._.t.d....
-000009b0: 007c 006a 1153 0029 0b7a 3f54 7261 696e  .|.j.S.).z?Train
-000009c0: 2058 6762 6f6f 7374 206d 6f64 656c 2e20   Xgboost model. 
-000009d0: 496e 636c 7564 6573 2068 7970 6572 7061  Includes hyperpa
-000009e0: 7261 6d65 7465 7220 7475 6e69 6e67 206f  rameter tuning o
-000009f0: 6e20 6465 6661 756c 742e 7a1e 3a20 5374  n default.z.: St
-00000a00: 6172 7420 6669 7474 696e 6720 5867 626f  art fitting Xgbo
-00000a10: 6f73 7420 6d6f 6465 6c2e 7a2c 636f 6e66  ost model.z,conf
-00000a20: 5f70 6172 616d 735f 7867 626f 6f73 7420  _params_xgboost 
-00000a30: 6f72 2063 6f6e 665f 7472 6169 6e69 6e67  or conf_training
-00000a40: 2069 7320 4e6f 6e65 7a1e 4669 6e69 7368   is Nonez.Finish
-00000a50: 6564 2068 7970 6572 7061 7261 6d65 7465  ed hyperparamete
-00000a60: 7220 7475 6e69 6e67 a902 da05 6c61 6265  r tuning....labe
-00000a70: 6cda 0677 6569 6768 74a9 0172 2800 0000  l..weight..r(...
-00000a80: da05 7472 6169 6eda 0474 6573 74da 0573  ..train..test..s
-00000a90: 7465 7073 2903 da0f 6e75 6d5f 626f 6f73  teps)...num_boos
-00000aa0: 745f 726f 756e 64da 1565 6172 6c79 5f73  t_round..early_s
-00000ab0: 746f 7070 696e 675f 726f 756e 6473 da05  topping_rounds..
-00000ac0: 6576 616c 737a 1146 696e 6973 6865 6420  evalsz.Finished 
-00000ad0: 7472 6169 6e69 6e67 2912 720d 0000 0072  training).r....r
-00000ae0: 0200 0000 721e 0000 0072 2200 0000 7215  ....r....r"...r.
-00000af0: 0000 0072 1300 0000 da0a 5661 6c75 6545  ...r......ValueE
-00000b00: 7272 6f72 da0e 6175 746f 7475 6e65 5f6d  rror..autotune_m
-00000b10: 6f64 656c da08 6175 746f 7475 6e65 da05  odel..autotune..
-00000b20: 7072 696e 74da 0d73 616d 706c 655f 7765  print..sample_we
-00000b30: 6967 6874 7221 0000 00da 0378 6762 da07  ightr!.....xgb..
-00000b40: 444d 6174 7269 7872 2b00 0000 da06 7061  DMatrixr+.....pa
-00000b50: 7261 6d73 722f 0000 0072 1600 0000 2909  ramsr/...r....).
-00000b60: 7217 0000 0072 2300 0000 7224 0000 0072  r....r#...r$...r
-00000b70: 2500 0000 7226 0000 0072 2000 0000 da07  %...r&...r .....
-00000b80: 645f 7472 6169 6eda 0664 5f74 6573 74da  d_train..d_test.
-00000b90: 0865 7661 6c5f 7365 7472 1800 0000 7218  .eval_setr....r.
-00000ba0: 0000 0072 1900 0000 da03 6669 7441 0000  ...r......fitA..
-00000bb0: 0073 2c00 0000 0008 1201 0802 0c01 0802  .s,.............
-00000bc0: 0801 1002 0802 0801 0a01 1202 0e01 0e01  ................
-00000bd0: 1002 0401 0601 0201 0a01 0601 02fb 0807  ................
-00000be0: 0801 7a10 5867 626f 6f73 744d 6f64 656c  ..z.XgboostModel
-00000bf0: 2e66 6974 6305 0000 0000 0000 0000 0000  .fitc...........
-00000c00: 000b 0000 0012 0000 0003 0000 0073 8201  .............s..
-00000c10: 0000 7400 7401 a002 a100 9b00 6401 9d02  ..t.t.......d...
-00000c20: 8301 0100 7403 6a04 7c02 8804 6402 8d02  ....t.j.|...d...
-00000c30: 8900 7405 8300 8902 8801 a006 a100 0100  ..t.............
-00000c40: 8801 6a07 7240 8801 6a08 7240 8801 6a09  ..j.r@..j.r@..j.
-00000c50: 7348 740a 6403 8301 8201 8700 8701 8702  sHt.d...........
-00000c60: 8703 8704 8705 6606 6404 6405 8408 7d05  ......f.d.d...}.
-00000c70: 6406 7d06 740b 6a0c 6a0d 6407 8801 6a08  d.}.t.j.j.d...j.
-00000c80: 6a0e 6408 8d02 7d07 740b 6a0f 6409 7c07  j.d...}.t.j.d.|.
-00000c90: 7c06 9b00 640a 9d02 640b 8d03 7d08 7c08  |...d...d...}.|.
-00000ca0: 6a10 7c05 8801 6a08 6a11 8801 6a08 6a12  j.|...j.j...j.j.
-00000cb0: 6407 6407 640c 8d05 0100 7a2c 740b 6a13  d.d.d.....z,t.j.
-00000cc0: a014 7c08 a101 7d09 7c09 a015 a100 0100  ..|...}.|.......
-00000cd0: 740b 6a13 a016 7c08 a101 7d09 7c09 a015  t.j...|...}.|...
-00000ce0: a100 0100 5700 6e1a 0400 7417 7418 740a  ....W.n...t.t.t.
-00000cf0: 6603 6b0a 72ee 0100 0100 0100 5900 6e02  f.k.r.......Y.n.
-00000d00: 5800 7c08 6a19 6a1a 7d0a 8801 6a09 6a1b  X.|.j.j.}...j.j.
-00000d10: 8801 6a09 6a1c 8801 6a09 6a1d 8802 8805  ..j.j...j.j.....
-00000d20: a01e a100 7c0a 640d 1900 7c0a 640e 1900  ....|.d...|.d...
-00000d30: 7c0a 640f 1900 7c0a 6410 1900 7c0a 6411  |.d...|.d...|.d.
-00000d40: 1900 7c0a 6412 1900 7c0a 6413 1900 7c0a  ..|.d...|.d...|.
-00000d50: 6414 1900 7c0a 6415 1900 8801 6a09 6a1f  d...|.d.....j.j.
-00000d60: 7c0a 6416 1900 7c0a 6417 1900 6418 9c11  |.d...|.d...d...
-00000d70: 8801 6a07 5f1a 7420 6419 8801 6a07 6a1a  ..j._.t d...j.j.
-00000d80: 8302 0100 7c0a 641a 1900 8801 6a07 5f21  ....|.d.....j._!
-00000d90: 641b 5300 291c 7a7b 5475 6e65 2068 7970  d.S.).z{Tune hyp
-00000da0: 6572 7061 7261 6d65 7465 7273 2e0a 0a20  erparameters... 
-00000db0: 2020 2020 2020 2041 6e20 616c 7465 726e         An altern
-00000dc0: 6174 6976 6520 636f 6e66 6967 2063 616e  ative config can
-00000dd0: 2062 6520 7072 6f76 6964 6564 2074 6f20   be provided to 
-00000de0: 6f76 6572 7772 6974 6520 7468 6520 6879  overwrite the hy
-00000df0: 7065 7270 6172 616d 6574 6572 2073 6561  perparameter sea
-00000e00: 7263 6820 7370 6163 652e 0a20 2020 2020  rch space..     
-00000e10: 2020 207a 2f3a 2053 7461 7274 2068 7970     z/: Start hyp
-00000e20: 6572 7061 7261 6d65 7465 7220 7475 6e69  erparameter tuni
-00000e30: 6e67 206f 6620 5867 626f 6f73 7420 6d6f  ng of Xgboost mo
-00000e40: 6465 6c2e 722a 0000 007a 3941 7420 6c65  del.r*...z9At le
-00000e50: 6173 7420 6f6e 6520 6f66 2074 6865 2063  ast one of the c
-00000e60: 6f6e 6669 6773 2069 7320 4e6f 6e65 2c20  onfigs is None, 
-00000e70: 7768 6963 6820 6973 206e 6f74 2061 6c6c  which is not all
-00000e80: 6f77 6564 6301 0000 0000 0000 0000 0000  owedc...........
-00000e90: 000c 0000 0015 0000 0013 0000 0073 0602  .............s..
-00000ea0: 0000 8801 6a00 6a01 8801 6a00 6a02 8801  ....j.j...j.j...
-00000eb0: 6a00 6a03 8802 8805 a004 a100 7c00 a005  j.j.........|...
-00000ec0: 6401 8801 6a00 6a06 8801 6a00 6a07 a103  d...j.j...j.j...
-00000ed0: 7c00 a008 6402 8801 6a00 6a09 8801 6a00  |...d...j.j...j.
-00000ee0: 6a0a a103 7c00 a008 6403 8801 6a00 6a0b  j...|...d...j.j.
-00000ef0: 8801 6a00 6a0c a103 7c00 a005 6404 8801  ..j.j...|...d...
-00000f00: 6a00 6a0d 8801 6a00 6a0e a103 7c00 a008  j.j...j.j...|...
-00000f10: 6405 8801 6a00 6a0f 8801 6a00 6a10 a103  d...j.j...j.j...
-00000f20: 7c00 a008 6406 8801 6a00 6a11 8801 6a00  |...d...j.j...j.
-00000f30: 6a12 a103 7c00 a008 6407 8801 6a00 6a13  j...|...d...j.j.
-00000f40: 8801 6a00 6a14 a103 7c00 a008 6408 8801  ..j.j...|...d...
-00000f50: 6a00 6a15 8801 6a00 6a16 a103 7c00 a005  j.j...j.j...|...
-00000f60: 6409 8801 6a00 6a17 8801 6a00 6a18 a103  d...j.j...j.j...
-00000f70: 8801 6a00 6a19 7c00 a005 640a 8801 6a00  ..j.j.|...d...j.
-00000f80: 6a1a 8801 6a00 6a1b a103 7c00 a005 640b  j...j.j...|...d.
-00000f90: 8801 6a00 6a1c 8801 6a00 6a1d a103 640c  ..j.j...j.j...d.
-00000fa0: 9c11 7d01 7c00 a01e 640d 640e 640f 6702  ..}.|...d.d.d.g.
-00000fb0: a102 7d02 7c02 9001 7234 8801 a01f 8805  ..}.|...r4......
-00000fc0: a101 7d03 7420 6a21 8803 8805 7c03 6410  ..}.t j!....|.d.
-00000fd0: 8d03 7d04 6e0e 7420 6a21 8803 8805 6411  ..}.n.t j!....d.
-00000fe0: 8d02 7d04 7422 6a23 a024 7c00 6412 a102  ..}.t"j#.$|.d...
-00000ff0: 7d05 8801 6a25 6a26 6413 6b02 9001 72c4  }...j%j&d.k...r.
-00001000: 7c04 6414 6602 8800 6415 6602 6702 7d06  |.d.f...d.f.g.}.
-00001010: 7420 6a27 7c01 7c04 7c01 640a 1900 8801  t j'|.|.|.d.....
-00001020: 6a25 6a28 7c06 7c05 6701 8801 6a00 6a03  j%j(|.|.g...j.j.
-00001030: 6416 8d07 7d07 7c07 a029 8800 a101 7d08  d...}.|..)....}.
-00001040: 742a a02b 6417 6418 8400 7c08 4400 8301  t*.+d.d...|.D...
-00001050: a101 7d09 742c 8804 7c09 8302 6419 1400  ..}.t,..|...d...
-00001060: 7d0a 7c0a 5300 7420 6a2d 7c01 7c04 7c01  }.|.S.t j-|.|.|.
-00001070: 640a 1900 8801 6a25 6a28 8801 6a25 6a26  d.....j%j(..j%j&
-00001080: 640e 8801 6a25 6a2e 7c05 6701 8801 6a25  d...j%j.|.g...j%
-00001090: 6a2f 641a 8d09 7d0b 7c0b 641b 1900 a030  j/d...}.|.d....0
-000010a0: a100 5300 6400 5300 291c 4eda 096d 6178  ..S.d.S.).N..max
-000010b0: 5f64 6570 7468 da05 616c 7068 61da 066c  _depth..alpha..l
-000010c0: 616d 6264 61da 0a6e 756d 5f6c 6561 7665  ambda..num_leave
-000010d0: 73da 0973 7562 7361 6d70 6c65 da10 636f  s..subsample..co
-000010e0: 6c73 616d 706c 655f 6279 7472 6565 da11  lsample_bytree..
-000010f0: 636f 6c73 616d 706c 655f 6279 6c65 7665  colsample_byleve
-00001100: 6cda 1063 6f6c 7361 6d70 6c65 5f62 796e  l..colsample_byn
-00001110: 6f64 65da 116d 696e 5f63 6869 6c64 5f73  ode..min_child_s
-00001120: 616d 706c 6573 722d 0000 00da 116e 756d  amplesr-.....num
-00001130: 5f70 6172 616c 6c65 6c5f 7472 6565 a911  _parallel_tree..
-00001140: da09 6f62 6a65 6374 6976 65da 0b65 7661  ..objective..eva
-00001150: 6c5f 6d65 7472 6963 da07 7665 7262 6f73  l_metric..verbos
-00001160: 65da 0b74 7265 655f 6d65 7468 6f64 da09  e..tree_method..
-00001170: 6e75 6d5f 636c 6173 7372 3d00 0000 723e  num_classr=...r>
-00001180: 0000 0072 3f00 0000 7240 0000 0072 4100  ...r?...r@...rA.
-00001190: 0000 7242 0000 0072 4300 0000 7244 0000  ..rB...rC...rD..
-000011a0: 0072 4500 0000 da03 6574 6172 2d00 0000  .rE.....etar-...
-000011b0: 7246 0000 0072 3500 0000 5446 7227 0000  rF...r5...TFr'..
-000011c0: 0072 2a00 0000 7a0d 7465 7374 2d6d 6c6f  .r*...z.test-mlo
-000011d0: 676c 6f73 73e9 0100 0000 722b 0000 0072  gloss.....r+...r
-000011e0: 2c00 0000 2905 722e 0000 0072 2f00 0000  ,...).r....r/...
-000011f0: 7230 0000 00da 0963 616c 6c62 6163 6b73  r0.....callbacks
-00001200: da0c 7665 7262 6f73 655f 6576 616c 6301  ..verbose_evalc.
-00001210: 0000 0000 0000 0000 0000 0002 0000 0005  ................
-00001220: 0000 0053 0000 0073 1600 0000 6700 7c00  ...S...s....g.|.
-00001230: 5d0e 7d01 7400 a001 7c01 a101 9102 7104  ].}.t...|.....q.
-00001240: 5300 7218 0000 00a9 02da 026e 70da 0661  S.r........np..a
-00001250: 7267 6d61 78a9 02da 022e 30da 046c 696e  rgmax.....0..lin
-00001260: 6572 1800 0000 7218 0000 0072 1900 0000  er....r....r....
-00001270: da0a 3c6c 6973 7463 6f6d 703e d100 0000  ..<listcomp>....
-00001280: 7304 0000 0006 0002 007a 3c58 6762 6f6f  s........z<Xgboo
-00001290: 7374 4d6f 6465 6c2e 6175 746f 7475 6e65  stModel.autotune
-000012a0: 2e3c 6c6f 6361 6c73 3e2e 6f62 6a65 6374  .<locals>.object
-000012b0: 6976 652e 3c6c 6f63 616c 733e 2e3c 6c69  ive.<locals>.<li
-000012c0: 7374 636f 6d70 3ee9 ffff ffff 2909 7238  stcomp>.....).r8
-000012d0: 0000 00da 0664 7472 6169 6e72 2e00 0000  .....dtrainr....
-000012e0: 722f 0000 00da 056e 666f 6c64 da09 6173  r/.....nfold..as
-000012f0: 5f70 616e 6461 73da 0473 6565 6472 4f00  _pandas..seedrO.
-00001300: 0000 da07 7368 7566 666c 657a 1274 6573  ....shufflez.tes
-00001310: 742d 6d6c 6f67 6c6f 7373 2d6d 6561 6e29  t-mlogloss-mean)
-00001320: 3172 1400 0000 da0f 6d6f 6465 6c5f 6f62  1r......model_ob
-00001330: 6a65 6374 6976 65da 116d 6f64 656c 5f65  jective..model_e
-00001340: 7661 6c5f 6d65 7472 6963 da0f 6d6f 6465  val_metric..mode
-00001350: 6c5f 7665 7262 6f73 6974 79da 076e 756e  l_verbosity..nun
-00001360: 6971 7565 da0b 7375 6767 6573 745f 696e  ique..suggest_in
-00001370: 74da 0d6d 6178 5f64 6570 7468 5f6d 696e  t..max_depth_min
-00001380: da0d 6d61 785f 6465 7074 685f 6d61 78da  ..max_depth_max.
-00001390: 0d73 7567 6765 7374 5f66 6c6f 6174 da09  .suggest_float..
-000013a0: 616c 7068 615f 6d69 6eda 0961 6c70 6861  alpha_min..alpha
-000013b0: 5f6d 6178 da0a 6c61 6d62 6461 5f6d 696e  _max..lambda_min
-000013c0: da0a 6c61 6d62 6461 5f6d 6178 da0e 6e75  ..lambda_max..nu
-000013d0: 6d5f 6c65 6176 6573 5f6d 696e da0e 6e75  m_leaves_min..nu
-000013e0: 6d5f 6c65 6176 6573 5f6d 6178 da0e 7375  m_leaves_max..su
-000013f0: 625f 7361 6d70 6c65 5f6d 696e da0e 7375  b_sample_min..su
-00001400: 625f 7361 6d70 6c65 5f6d 6178 da16 636f  b_sample_max..co
-00001410: 6c5f 7361 6d70 6c65 5f62 795f 7472 6565  l_sample_by_tree
-00001420: 5f6d 696e da16 636f 6c5f 7361 6d70 6c65  _min..col_sample
-00001430: 5f62 795f 7472 6565 5f6d 6178 da17 636f  _by_tree_max..co
-00001440: 6c5f 7361 6d70 6c65 5f62 795f 6c65 7665  l_sample_by_leve
-00001450: 6c5f 6d69 6eda 1763 6f6c 5f73 616d 706c  l_min..col_sampl
-00001460: 655f 6279 5f6c 6576 656c 5f6d 6178 da16  e_by_level_max..
-00001470: 636f 6c5f 7361 6d70 6c65 5f62 795f 6e6f  col_sample_by_no
-00001480: 6465 5f6d 696e da16 636f 6c5f 7361 6d70  de_min..col_samp
-00001490: 6c65 5f62 795f 6e6f 6465 5f6d 6178 da15  le_by_node_max..
-000014a0: 6d69 6e5f 6368 696c 645f 7361 6d70 6c65  min_child_sample
-000014b0: 735f 6d69 6eda 156d 696e 5f63 6869 6c64  s_min..min_child
-000014c0: 5f73 616d 706c 6573 5f6d 6178 724d 0000  _samples_maxrM..
-000014d0: 00da 0973 7465 7073 5f6d 696e da09 7374  ...steps_min..st
-000014e0: 6570 735f 6d61 78da 156e 756d 5f70 6172  eps_max..num_par
-000014f0: 616c 6c65 6c5f 7472 6565 5f6d 696e da15  allel_tree_min..
-00001500: 6e75 6d5f 7061 7261 6c6c 656c 5f74 7265  num_parallel_tre
-00001510: 655f 6d61 78da 1373 7567 6765 7374 5f63  e_max..suggest_c
-00001520: 6174 6567 6f72 6963 616c 7221 0000 0072  ategoricalr!...r
-00001530: 3600 0000 7237 0000 00da 066f 7074 756e  6...r7.....optun
-00001540: 61da 0b69 6e74 6567 7261 7469 6f6e da16  a..integration..
-00001550: 5847 426f 6f73 7450 7275 6e69 6e67 4361  XGBoostPruningCa
-00001560: 6c6c 6261 636b 7213 0000 00da 1468 7970  llbackr......hyp
-00001570: 6572 7475 6e69 6e67 5f63 765f 666f 6c64  ertuning_cv_fold
-00001580: 7372 2b00 0000 722f 0000 00da 0770 7265  sr+...r/.....pre
-00001590: 6469 6374 7252 0000 00da 0761 7361 7272  dictrR.....asarr
-000015a0: 6179 7207 0000 00da 0263 76da 1367 6c6f  ayr......cv..glo
-000015b0: 6261 6c5f 7261 6e64 6f6d 5f73 7461 7465  bal_random_state
-000015c0: da17 7368 7566 666c 655f 6475 7269 6e67  ..shuffle_during
-000015d0: 5f74 7261 696e 696e 67da 046d 6561 6e29  _training..mean)
-000015e0: 0cda 0574 7269 616c da05 7061 7261 6d72  ...trial..paramr
-000015f0: 3500 0000 7220 0000 0072 3900 0000 da10  5...r ...r9.....
-00001600: 7072 756e 696e 675f 6361 6c6c 6261 636b  pruning_callback
-00001610: 723b 0000 0072 1600 0000 da05 7072 6564  r;...r......pred
-00001620: 73da 0b70 7265 645f 6c61 6265 6c73 da07  s..pred_labels..
-00001630: 6d61 7474 6865 77da 0672 6573 756c 74a9  matthew..result.
-00001640: 0672 3a00 0000 7217 0000 00da 0874 7261  .r:...r......tra
-00001650: 696e 5f6f 6e72 2300 0000 7226 0000 0072  in_onr#...r&...r
-00001660: 2500 0000 7218 0000 0072 1900 0000 7248  %...r....r....rH
-00001670: 0000 0080 0000 0073 c400 0000 0002 0601  .......s........
-00001680: 0601 0601 0201 0601 0401 0201 0601 06fd  ................
-00001690: 0205 0401 0200 0600 06ff 0203 0401 0200  ................
-000016a0: 0600 06ff 0203 0401 0201 0601 06fd 0205  ................
-000016b0: 0401 0201 0601 06fd 0205 0401 0201 0601  ................
-000016c0: 06fd 0205 0401 0201 0601 06fd 0205 0401  ................
-000016d0: 0201 0601 06fd 0205 0401 0201 0601 06fd  ................
-000016e0: 0205 0601 0401 0200 0600 06ff 0203 0401  ................
-000016f0: 0201 0601 06fd 02cd 0639 1001 0601 0a01  .........9......
-00001700: 1202 0e02 0601 0200 02ff 0404 0e01 1001  ................
-00001710: 0401 0201 0201 0601 0601 0201 0401 06f9  ................
-00001720: 0609 0a01 1401 0e01 0402 0401 0201 0201  ................
-00001730: 0601 0601 0601 0201 0601 0401 06f7 060c  ................
-00001740: 7a28 5867 626f 6f73 744d 6f64 656c 2e61  z(XgboostModel.a
-00001750: 7574 6f74 756e 652e 3c6c 6f63 616c 733e  utotune.<locals>
-00001760: 2e6f 626a 6563 7469 7665 da07 7867 626f  .objective..xgbo
-00001770: 6f73 7454 2902 da0c 6d75 6c74 6976 6172  ostT)...multivar
-00001780: 6961 7465 725c 0000 00da 086d 696e 696d  iater\.....minim
-00001790: 697a 657a 0720 7475 6e69 6e67 2903 da09  izez. tuning)...
-000017a0: 6469 7265 6374 696f 6eda 0773 616d 706c  direction..sampl
-000017b0: 6572 da0a 7374 7564 795f 6e61 6d65 2904  er..study_name).
-000017c0: da08 6e5f 7472 6961 6c73 da07 7469 6d65  ..n_trials..time
-000017d0: 6f75 74da 0e67 635f 6166 7465 725f 7472  out..gc_after_tr
-000017e0: 6961 6cda 1173 686f 775f 7072 6f67 7265  ial..show_progre
-000017f0: 7373 5f62 6172 723d 0000 0072 3e00 0000  ss_barr=...r>...
-00001800: 723f 0000 0072 4000 0000 7241 0000 0072  r?...r@...rA...r
-00001810: 4200 0000 7243 0000 0072 4400 0000 7245  B...rC...rD...rE
-00001820: 0000 0072 2d00 0000 7246 0000 0072 4700  ...r-...rF...rG.
-00001830: 0000 7a0d 4265 7374 2070 6172 616d 733a  ..z.Best params:
-00001840: 2072 3500 0000 4e29 2272 0d00 0000 7202   r5...N)"r....r.
-00001850: 0000 0072 1e00 0000 7236 0000 0072 3700  ...r....r6...r7.
-00001860: 0000 720c 0000 0072 2200 0000 7215 0000  ..r....r"...r...
-00001870: 0072 1300 0000 7214 0000 0072 3100 0000  .r....r....r1...
-00001880: 727b 0000 00da 0873 616d 706c 6572 73da  r{.....samplers.
-00001890: 0a54 5045 5361 6d70 6c65 7272 8200 0000  .TPESamplerr....
-000018a0: da0c 6372 6561 7465 5f73 7475 6479 da08  ..create_study..
-000018b0: 6f70 7469 6d69 7a65 da1c 6879 7065 7270  optimize..hyperp
-000018c0: 6172 616d 6574 6572 5f74 756e 696e 675f  arameter_tuning_
-000018d0: 726f 756e 6473 da26 6879 7065 7270 6172  rounds.&hyperpar
-000018e0: 616d 6574 6572 5f74 756e 696e 675f 6d61  ameter_tuning_ma
-000018f0: 785f 7275 6e74 696d 655f 7365 6373 da0d  x_runtime_secs..
-00001900: 7669 7375 616c 697a 6174 696f 6eda 1970  visualization..p
-00001910: 6c6f 745f 6f70 7469 6d69 7a61 7469 6f6e  lot_optimization
-00001920: 5f68 6973 746f 7279 da04 7368 6f77 da16  _history..show..
-00001930: 706c 6f74 5f70 6172 616d 5f69 6d70 6f72  plot_param_impor
-00001940: 7461 6e63 6573 da11 5a65 726f 4469 7669  tances..ZeroDivi
-00001950: 7369 6f6e 4572 726f 72da 0c52 756e 7469  sionError..Runti
-00001960: 6d65 4572 726f 72da 0a62 6573 745f 7472  meError..best_tr
-00001970: 6961 6c72 3800 0000 725e 0000 0072 5f00  ialr8...r^...r_.
-00001980: 0000 7260 0000 0072 6100 0000 724d 0000  ..r`...ra...rM..
-00001990: 0072 3400 0000 7235 0000 0029 0b72 1700  .r4...r5...).r..
-000019a0: 0000 7223 0000 0072 2400 0000 7225 0000  ..r#...r$...r%..
-000019b0: 0072 2600 0000 7248 0000 00da 0961 6c67  .r&...rH.....alg
-000019c0: 6f72 6974 686d 7292 0000 00da 0573 7475  orithmr......stu
-000019d0: 6479 da03 6669 675a 1278 6762 6f6f 7374  dy..figZ.xgboost
-000019e0: 5f62 6573 745f 7061 7261 6d72 1800 0000  _best_paramr....
-000019f0: 728c 0000 0072 1900 0000 7233 0000 0066  r....r....r3...f
-00001a00: 0000 0073 7a00 0000 000b 1201 0e01 0602  ...sz...........
-00001a10: 0803 04ff 0202 04fe 0203 04fd 0205 0201  ................
-00001a20: 02ff 0404 1663 0401 0601 0200 06ff 0603  .....c..........
-00001a30: 0401 0201 0201 08fd 0606 0401 0201 0601  ................
-00001a40: 0601 0201 02fb 0607 0201 0c01 0801 0c01  ................
-00001a50: 0c01 1401 0602 0802 0601 0601 0601 0201  ................
-00001a60: 0601 0201 02ff 0203 0601 0601 0601 0601  ................
-00001a70: 0601 0601 0601 0601 0601 0601 06ed 0a15  ................
-00001a80: 0e01 7a15 5867 626f 6f73 744d 6f64 656c  ..z.XgboostModel
-00001a90: 2e61 7574 6f74 756e 6529 02da 0264 6672  .autotune)...dfr
-00001aa0: 1c00 0000 6302 0000 0000 0000 0000 0000  ....c...........
-00001ab0: 0006 0000 0004 0000 0043 0000 0073 9800  .........C...s..
-00001ac0: 0000 7400 7401 a002 a100 9b00 6401 9d02  ..t.t.......d...
-00001ad0: 8301 0100 7403 a004 7c01 a101 7d02 7c00  ....t...|...}.|.
-00001ae0: 6a05 732a 7406 6402 8301 8201 7c00 6a07  j.s*t.d.....|.j.
-00001af0: 7338 7406 6403 8301 8201 7c00 6a05 a008  s8t.d.....|.j...
-00001b00: 7c02 a101 7d03 7c00 6a09 6404 6b02 7270  |...}.|.j.d.k.rp
-00001b10: 740a a00b 6405 6406 8400 7c03 4400 8301  t...d.d...|.D...
-00001b20: a101 7d04 7c04 7c00 6a07 6a0c 6b04 7d05  ..}.|.|.j.j.k.}.
-00001b30: 6e18 7c03 7d04 740a a00b 6407 6406 8400  n.|.}.t...d.d...
-00001b40: 7c03 4400 8301 a101 7d05 740d 6408 8301  |.D.....}.t.d...
-00001b50: 0100 7c04 7c05 6602 5300 2909 7a17 5072  ..|.|.f.S.).z.Pr
-00001b60: 6564 6963 7420 6f6e 2075 6e73 6565 6e20  edict on unseen 
-00001b70: 6461 7461 2e7a 333a 2053 7461 7274 2070  data.z3: Start p
-00001b80: 7265 6469 6374 696e 6720 6f6e 206e 6577  redicting on new
-00001b90: 2064 6174 6120 7573 696e 6720 5867 626f   data using Xgbo
-00001ba0: 6f73 7420 6d6f 6465 6c2e 7a20 4e6f 2074  ost model.z No t
-00001bb0: 7261 696e 6564 206d 6f64 656c 2068 6173  rained model has
-00001bc0: 2062 6565 6e20 666f 756e 642e 7a2b 4e6f   been found.z+No
-00001bd0: 206d 6f64 656c 2063 6f6e 6669 6775 7261   model configura
-00001be0: 7469 6f6e 2066 696c 6520 6861 7320 6265  tion file has be
-00001bf0: 656e 2066 6f75 6e64 2e72 1000 0000 6301  en found.r....c.
-00001c00: 0000 0000 0000 0000 0000 0002 0000 0004  ................
-00001c10: 0000 0053 0000 0073 1400 0000 6700 7c00  ...S...s....g.|.
-00001c20: 5d0c 7d01 7c01 6400 1900 9102 7104 5300  ].}.|.d.....q.S.
-00001c30: 2901 724e 0000 0072 1800 0000 7254 0000  ).rN...r....rT..
-00001c40: 0072 1800 0000 7218 0000 0072 1900 0000  .r....r....r....
-00001c50: 7257 0000 0023 0100 0073 0400 0000 0600  rW...#...s......
-00001c60: 0200 7a28 5867 626f 6f73 744d 6f64 656c  ..z(XgboostModel
-00001c70: 2e70 7265 6469 6374 2e3c 6c6f 6361 6c73  .predict.<locals
-00001c80: 3e2e 3c6c 6973 7463 6f6d 703e 6301 0000  >.<listcomp>c...
-00001c90: 0000 0000 0000 0000 0002 0000 0005 0000  ................
-00001ca0: 0053 0000 0073 1600 0000 6700 7c00 5d0e  .S...s....g.|.].
-00001cb0: 7d01 7400 a001 7c01 a101 9102 7104 5300  }.t...|.....q.S.
-00001cc0: 7218 0000 0072 5100 0000 7254 0000 0072  r....rQ...rT...r
-00001cd0: 1800 0000 7218 0000 0072 1900 0000 7257  ....r....r....rW
-00001ce0: 0000 0029 0100 0073 0400 0000 0600 0200  ...)...s........
-00001cf0: 7a13 4669 6e69 7368 6564 2070 7265 6469  z.Finished predi
-00001d00: 6374 696e 6729 0e72 0d00 0000 7202 0000  cting).r....r...
-00001d10: 0072 1e00 0000 7236 0000 0072 3700 0000  .r....r6...r7...
-00001d20: 7216 0000 00da 0945 7863 6570 7469 6f6e  r......Exception
-00001d30: 7215 0000 0072 7f00 0000 7212 0000 0072  r....r....r....r
-00001d40: 5200 0000 7280 0000 00da 1863 6c61 7373  R...r......class
-00001d50: 6966 6963 6174 696f 6e5f 7468 7265 7368  ification_thresh
-00001d60: 6f6c 6472 3400 0000 2906 7217 0000 0072  oldr4...).r....r
-00001d70: a800 0000 723a 0000 00da 0d70 6172 7469  ....r:.....parti
-00001d80: 616c 5f70 726f 6273 da0f 7072 6564 6963  al_probs..predic
-00001d90: 7465 645f 7072 6f62 73da 1170 7265 6469  ted_probs..predi
-00001da0: 6374 6564 5f63 6c61 7373 6573 7218 0000  cted_classesr...
-00001db0: 0072 1800 0000 7219 0000 0072 7f00 0000  .r....r....r....
-00001dc0: 1501 0000 7322 0000 0000 0202 010c ff04  ....s"..........
-00001dd0: 030a 0106 0108 0206 0108 020c 010a 0114  ................
-00001de0: 020a ff04 0404 0114 0108 017a 1458 6762  ...........z.Xgb
-00001df0: 6f6f 7374 4d6f 6465 6c2e 7072 6564 6963  oostModel.predic
-00001e00: 7429 034e 4e4e 291a da08 5f5f 6e61 6d65  t).NNN)...__name
-00001e10: 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f da0c  __..__module__..
-00001e20: 5f5f 7175 616c 6e61 6d65 5f5f da07 5f5f  __qualname__..__
-00001e30: 646f 635f 5f72 0400 0000 7205 0000 0072  doc__r....r....r
-00001e40: 0900 0000 720b 0000 0072 0a00 0000 721a  ....r....r....r.
-00001e50: 0000 00da 0270 64da 0653 6572 6965 7372  .....pd..Seriesr
-00001e60: 0300 0000 da03 7374 72da 0566 6c6f 6174  ......str..float
-00001e70: 7221 0000 0072 2200 0000 da09 4461 7461  r!...r".....Data
-00001e80: 4672 616d 6572 3600 0000 da07 426f 6f73  Framer6.....Boos
-00001e90: 7465 7272 3c00 0000 7233 0000 0072 0600  terr<...r3...r..
-00001ea0: 0000 7252 0000 00da 076e 6461 7272 6179  ..rR.....ndarray
-00001eb0: 727f 0000 0072 1800 0000 7218 0000 0072  r....r....r....r
-00001ec0: 1800 0000 7219 0000 0072 0f00 0000 1a00  ....r....r......
-00001ed0: 0000 7334 0000 0008 0104 0500 0100 0100  ..s4............
-00001ee0: fb02 0206 0106 0106 0106 fb0c 0d1a 0808  ................
-00001ef0: 1104 0104 0104 0104 0104 fa0c 2704 0104  ............'...
-00001f00: 0104 0104 0102 fa0c 7f00 3072 0f00 0000  ..........0r....
-00001f10: 291c 72b1 0000 0072 0200 0000 da06 7479  ).r....r......ty
-00001f20: 7069 6e67 7203 0000 0072 0400 0000 7205  pingr....r....r.
-00001f30: 0000 0072 0600 0000 da05 6e75 6d70 7972  ...r......numpyr
-00001f40: 5200 0000 727b 0000 00da 0670 616e 6461  R...r{.....panda
-00001f50: 7372 b200 0000 728e 0000 0072 3600 0000  sr....r....r6...
-00001f60: da0f 736b 6c65 6172 6e2e 6d65 7472 6963  ..sklearn.metric
-00001f70: 7372 0700 0000 5a0d 736b 6c65 6172 6e2e  sr....Z.sklearn.
-00001f80: 7574 696c 7372 0800 0000 da1f 626c 7565  utilsr......blue
-00001f90: 6361 7374 2e63 6f6e 6669 672e 7472 6169  cast.config.trai
-00001fa0: 6e69 6e67 5f63 6f6e 6669 6772 0900 0000  ning_configr....
-00001fb0: 720a 0000 0072 0b00 0000 da24 626c 7565  r....r.....$blue
-00001fc0: 6361 7374 2e67 656e 6572 616c 5f75 7469  cast.general_uti
-00001fd0: 6c73 2e67 656e 6572 616c 5f75 7469 6c73  ls.general_utils
-00001fe0: 720c 0000 0072 0d00 0000 5a22 626c 7565  r....r....Z"blue
-00001ff0: 6361 7374 2e6d 6c5f 6d6f 6465 6c6c 696e  cast.ml_modellin
-00002000: 672e 6261 7365 5f63 6c61 7373 6573 720e  g.base_classesr.
-00002010: 0000 0072 0f00 0000 7218 0000 0072 1800  ...r....r....r..
-00002020: 0000 7218 0000 0072 1900 0000 da08 3c6d  ..r....r......<m
-00002030: 6f64 756c 653e 0100 0000 7318 0000 0004  odule>....s.....
-00002040: 060c 0118 0208 0108 0108 0108 010c 010c  ................
-00002050: 0214 0510 010c 03                        .......
+000006e0: 9d02 8301 0100 6e12 7400 7401 a002 a100  ......n.t.t.....
+000006f0: 9b00 6403 9d02 8301 0100 7c00 6a05 7368  ..d.......|.j.sh
+00000700: 7406 8300 7c00 5f05 7400 7401 a002 a100  t...|._.t.t.....
+00000710: 9b00 6404 9d02 8301 0100 6e12 7400 7401  ..d.......n.t.t.
+00000720: a002 a100 9b00 6405 9d02 8301 0100 7c00  ......d.......|.
+00000730: 6a07 739c 7408 8300 7c00 5f07 7400 7401  j.s.t...|._.t.t.
+00000740: a002 a100 9b00 6406 9d02 8301 0100 6e12  ......d.......n.
+00000750: 7400 7401 a002 a100 9b00 6407 9d02 8301  t.t.......d.....
+00000760: 0100 6408 5300 2909 7a36 4c6f 6164 206d  ..d.S.).z6Load m
+00000770: 756c 7469 706c 6520 636f 6e66 6967 7320  ultiple configs 
+00000780: 6f72 206c 6f61 6420 6465 6661 756c 7420  or load default 
+00000790: 636f 6e66 6967 7320 696e 7374 6561 642e  configs instead.
+000007a0: 7a32 3a20 5374 6172 7420 6c6f 6164 696e  z2: Start loadin
+000007b0: 6720 6578 6973 7469 6e67 206f 7220 6465  g existing or de
+000007c0: 6661 756c 7420 636f 6e66 6967 2066 696c  fault config fil
+000007d0: 6573 2e2e 7a1e 3a20 4c6f 6164 2064 6566  es..z.: Load def
+000007e0: 6175 6c74 2054 7261 696e 696e 6743 6f6e  ault TrainingCon
+000007f0: 6669 672e 7a20 3a20 466f 756e 6420 7072  fig.z : Found pr
+00000800: 6f76 6964 6564 2054 7261 696e 696e 6743  ovided TrainingC
+00000810: 6f6e 6669 672e 7a27 3a20 4c6f 6164 2064  onfig.z': Load d
+00000820: 6566 6175 6c74 2058 6762 6f6f 7374 5475  efault XgboostTu
+00000830: 6e65 5061 7261 6d73 436f 6e66 6967 2e7a  neParamsConfig.z
+00000840: 293a 2046 6f75 6e64 2070 726f 7669 6465  ): Found provide
+00000850: 6420 5867 626f 6f73 7454 756e 6550 6172  d XgboostTunePar
+00000860: 616d 7343 6f6e 6669 672e 7a27 3a20 4c6f  amsConfig.z': Lo
+00000870: 6164 2064 6566 6175 6c74 2058 6762 6f6f  ad default Xgboo
+00000880: 7374 4669 6e61 6c50 6172 616d 436f 6e66  stFinalParamConf
+00000890: 6967 2e7a 293a 2046 6f75 6e64 2070 726f  ig.z): Found pro
+000008a0: 7669 6465 6420 5867 626f 6f73 7446 696e  vided XgboostFin
+000008b0: 616c 5061 7261 6d43 6f6e 6669 672e 4e29  alParamConfig.N)
+000008c0: 0972 0d00 0000 7202 0000 0072 1e00 0000  .r....r....r....
+000008d0: 7213 0000 0072 0900 0000 7214 0000 0072  r....r....r....r
+000008e0: 0b00 0000 7215 0000 0072 0a00 0000 2901  ....r....r....).
+000008f0: 7217 0000 0072 1800 0000 7218 0000 0072  r....r....r....r
+00000900: 1900 0000 da10 6368 6563 6b5f 6c6f 6164  ......check_load
+00000910: 5f63 6f6e 6673 3200 0000 731a 0000 0000  _confs2...s.....
+00000920: 0212 0106 0108 0114 0212 0206 0108 0114  ................
+00000930: 0212 0206 0108 0114 027a 1d58 6762 6f6f  .........z.Xgboo
+00000940: 7374 4d6f 6465 6c2e 6368 6563 6b5f 6c6f  stModel.check_lo
+00000950: 6164 5f63 6f6e 6673 2905 da07 785f 7472  ad_confs)...x_tr
+00000960: 6169 6eda 0678 5f74 6573 74da 0779 5f74  ain..x_test..y_t
+00000970: 7261 696e da06 795f 7465 7374 721c 0000  rain..y_testr...
+00000980: 0063 0500 0000 0000 0000 0000 0000 0900  .c..............
+00000990: 0000 0700 0000 4300 0000 7352 0100 0074  ......C...sR...t
+000009a0: 0074 01a0 02a1 009b 0064 019d 0283 0101  .t.......d......
+000009b0: 007c 00a0 03a1 0001 007c 006a 0472 267c  .|.......|.j.r&|
+000009c0: 006a 0573 2e74 0664 0283 0182 017c 006a  .j.s.t.d.....|.j
+000009d0: 056a 0772 467c 00a0 087c 017c 027c 037c  .j.rF|...|.|.|.|
+000009e0: 04a1 0401 0074 0964 0383 0101 0074 0964  .....t.d.....t.d
+000009f0: 0483 0101 007c 006a 056a 0a72 8c74 0074  .....|.j.j.r.t.t
+00000a00: 01a0 02a1 009b 0064 059d 0283 0101 0074  .......d.......t
+00000a10: 0ba0 0c7c 017c 0267 02a1 017d 0174 0ba0  ...|.|.g...}.t..
+00000a20: 0c7c 037c 0467 02a1 017d 037c 006a 046a  .|.|.g...}.|.j.j
+00000a30: 0d72 b67c 00a0 0e7c 03a1 017d 0574 0f6a  .r.|...|...}.t.j
+00000a40: 107c 017c 037c 057c 006a 056a 1164 068d  .|.|.|.|.j.j.d..
+00000a50: 047d 066e 1474 0f6a 107c 017c 037c 006a  .}.n.t.j.|.|.|.j
+00000a60: 056a 1164 078d 037d 0674 0f6a 107c 027c  .j.d...}.t.j.|.|
+00000a70: 047c 006a 056a 1164 078d 037d 077c 0664  .|.j.j.d...}.|.d
+00000a80: 0866 027c 0764 0966 0267 027d 087c 006a  .f.|.d.f.g.}.|.j
+00000a90: 056a 1264 0a6b 0290 0172 2474 0f6a 137c  .j.d.k...r$t.j.|
+00000aa0: 006a 046a 147c 067c 006a 046a 1464 0b19  .j.j.|.|.j.j.d..
+00000ab0: 007c 006a 056a 157c 0864 0c8d 057c 005f  .|.j.j.|.d...|._
+00000ac0: 166e 2074 0f6a 137c 006a 046a 147c 067c  .n t.j.|.j.j.|.|
+00000ad0: 006a 046a 1464 0b19 007c 0864 0d8d 047c  .j.j.d...|.d...|
+00000ae0: 005f 1674 0964 0e83 0101 007c 006a 1653  ._.t.d.....|.j.S
+00000af0: 0029 0f7a 3f54 7261 696e 2058 6762 6f6f  .).z?Train Xgboo
+00000b00: 7374 206d 6f64 656c 2e20 496e 636c 7564  st model. Includ
+00000b10: 6573 2068 7970 6572 7061 7261 6d65 7465  es hyperparamete
+00000b20: 7220 7475 6e69 6e67 206f 6e20 6465 6661  r tuning on defa
+00000b30: 756c 742e 7a1e 3a20 5374 6172 7420 6669  ult.z.: Start fi
+00000b40: 7474 696e 6720 5867 626f 6f73 7420 6d6f  tting Xgboost mo
+00000b50: 6465 6c2e fa2c 636f 6e66 5f70 6172 616d  del..,conf_param
+00000b60: 735f 7867 626f 6f73 7420 6f72 2063 6f6e  s_xgboost or con
+00000b70: 665f 7472 6169 6e69 6e67 2069 7320 4e6f  f_training is No
+00000b80: 6e65 7a1e 4669 6e69 7368 6564 2068 7970  nez.Finished hyp
+00000b90: 6572 7061 7261 6d65 7465 7220 7475 6e69  erparameter tuni
+00000ba0: 6e67 7a0e 5374 6172 7420 7472 6169 6e69  ngz.Start traini
+00000bb0: 6e67 7a7f 3a20 556e 696f 6e20 7472 6169  ngz.: Union trai
+00000bc0: 6e20 616e 6420 7465 7374 2064 6174 6120  n and test data 
+00000bd0: 666f 7220 6669 6e61 6c20 6d6f 6465 6c20  for final model 
+00000be0: 7472 6169 6e69 6e67 2062 6173 6564 206f  training based o
+00000bf0: 6e20 5472 6169 6e69 6e67 436f 6e66 6967  n TrainingConfig
+00000c00: 0a20 2020 2020 2020 2020 2020 2020 7061  .             pa
+00000c10: 7261 6d20 2775 7365 5f66 756c 6c5f 6461  ram 'use_full_da
+00000c20: 7461 5f66 6f72 5f66 696e 616c 5f6d 6f64  ta_for_final_mod
+00000c30: 656c 27a9 03da 056c 6162 656c da06 7765  el'....label..we
+00000c40: 6967 6874 da12 656e 6162 6c65 5f63 6174  ight..enable_cat
+00000c50: 6567 6f72 6963 616c a902 7229 0000 0072  egorical..r)...r
+00000c60: 2b00 0000 da05 7472 6169 6eda 0474 6573  +.....train..tes
+00000c70: 74e9 0100 0000 da05 7374 6570 7329 03da  t.......steps)..
+00000c80: 0f6e 756d 5f62 6f6f 7374 5f72 6f75 6e64  .num_boost_round
+00000c90: da15 6561 726c 795f 7374 6f70 7069 6e67  ..early_stopping
+00000ca0: 5f72 6f75 6e64 73da 0565 7661 6c73 2902  _rounds..evals).
+00000cb0: 7231 0000 0072 3300 0000 7a11 4669 6e69  r1...r3...z.Fini
+00000cc0: 7368 6564 2074 7261 696e 696e 6729 1772  shed training).r
+00000cd0: 0d00 0000 7202 0000 0072 1e00 0000 7222  ....r....r....r"
+00000ce0: 0000 0072 1500 0000 7213 0000 00da 0a56  ...r....r......V
+00000cf0: 616c 7565 4572 726f 72da 0e61 7574 6f74  alueError..autot
+00000d00: 756e 655f 6d6f 6465 6cda 0861 7574 6f74  une_model..autot
+00000d10: 756e 65da 0570 7269 6e74 da1d 7573 655f  une..print..use_
+00000d20: 6675 6c6c 5f64 6174 615f 666f 725f 6669  full_data_for_fi
+00000d30: 6e61 6c5f 6d6f 6465 6cda 0270 64da 0663  nal_model..pd..c
+00000d40: 6f6e 6361 74da 0d73 616d 706c 655f 7765  oncat..sample_we
+00000d50: 6967 6874 7221 0000 00da 0378 6762 da07  ightr!.....xgb..
+00000d60: 444d 6174 7269 78da 1d63 6174 5f65 6e63  DMatrix..cat_enc
+00000d70: 6f64 696e 675f 7669 615f 6d6c 5f61 6c67  oding_via_ml_alg
+00000d80: 6f72 6974 686d da14 6879 7065 7274 756e  orithm..hypertun
+00000d90: 696e 675f 6376 5f66 6f6c 6473 722d 0000  ing_cv_foldsr-..
+00000da0: 00da 0670 6172 616d 7372 3200 0000 7216  ...paramsr2...r.
+00000db0: 0000 0029 0972 1700 0000 7223 0000 0072  ...).r....r#...r
+00000dc0: 2400 0000 7225 0000 0072 2600 0000 7220  $...r%...r&...r 
+00000dd0: 0000 00da 0764 5f74 7261 696e da06 645f  .....d_train..d_
+00000de0: 7465 7374 da08 6576 616c 5f73 6574 7218  test..eval_setr.
+00000df0: 0000 0072 1800 0000 7219 0000 00da 0366  ...r....r......f
+00000e00: 6974 4700 0000 7362 0000 0000 0812 0108  itG...sb........
+00000e10: 020c 0108 0208 0110 0208 0208 0108 0102  ................
+00000e20: 010c ff04 040e 010e 0208 010a 0104 0102  ................
+00000e30: 0102 0102 0106 fc08 0704 0102 0102 0106  ................
+00000e40: fd06 0604 0102 0102 0106 fd06 0510 020e  ................
+00000e50: 0104 0106 0102 010a 0106 0102 fb0a 0804  ................
+00000e60: 0106 0102 010a 0202 fb08 0708 017a 1058  .............z.X
+00000e70: 6762 6f6f 7374 4d6f 6465 6c2e 6669 7463  gboostModel.fitc
+00000e80: 0500 0000 0000 0000 0000 0000 0b00 0000  ................
+00000e90: 1000 0000 0300 0000 7392 0100 0074 0074  ........s....t.t
+00000ea0: 01a0 02a1 009b 0064 019d 0283 0101 0088  .......d........
+00000eb0: 016a 0372 1e88 016a 0473 2674 0564 0283  .j.r...j.s&t.d..
+00000ec0: 0182 0174 066a 077c 0288 0488 016a 046a  ...t.j.|.....j.j
+00000ed0: 0864 038d 0389 0074 0983 0089 0288 01a0  .d.....t........
+00000ee0: 0aa1 0001 0088 016a 0372 5a88 016a 0472  .......j.rZ..j.r
+00000ef0: 5a88 016a 0b73 6274 0564 0483 0182 0187  Z..j.sbt.d......
+00000f00: 0087 0187 0287 0387 0487 0566 0664 0564  ...........f.d.d
+00000f10: 0684 087d 0564 077d 0674 0c6a 0d6a 0e64  ...}.d.}.t.j.j.d
+00000f20: 0888 016a 046a 0f64 098d 027d 0774 0c6a  ...j.j.d...}.t.j
+00000f30: 1064 0a7c 077c 069b 0064 0b9d 0264 0c8d  .d.|.|...d...d..
+00000f40: 037d 087c 086a 117c 0588 016a 046a 1288  .}.|.j.|...j.j..
+00000f50: 016a 046a 1364 0d64 0d64 0e8d 0501 007a  .j.j.d.d.d.....z
+00000f60: 2c74 0c6a 14a0 157c 08a1 017d 097c 09a0  ,t.j...|...}.|..
+00000f70: 16a1 0001 0074 0c6a 14a0 177c 08a1 017d  .....t.j...|...}
+00000f80: 097c 09a0 16a1 0001 0057 006e 1c04 0074  .|.......W.n...t
+00000f90: 1874 1974 0566 036b 0a90 0172 0a01 0001  .t.t.f.k...r....
+00000fa0: 0001 0059 006e 0258 007c 086a 1a6a 1b7d  ...Y.n.X.|.j.j.}
+00000fb0: 0a88 016a 0b6a 1c88 016a 0b6a 1d88 016a  ...j.j...j.j...j
+00000fc0: 0b6a 1e88 0288 05a0 1fa1 007c 0a64 0f19  .j.........|.d..
+00000fd0: 007c 0a64 1019 007c 0a64 1119 007c 0a64  .|.d...|.d...|.d
+00000fe0: 1219 007c 0a64 1319 007c 0a64 1419 007c  ...|.d...|.d...|
+00000ff0: 0a64 1519 007c 0a64 1619 0088 016a 0b6a  .d...|.d.....j.j
+00001000: 207c 0a64 1719 0064 189c 0f88 016a 035f   |.d...d.....j._
+00001010: 1b74 2164 1988 016a 036a 1b83 0201 007c  .t!d...j.j.....|
+00001020: 0a64 1a19 0088 016a 035f 2264 1b53 0029  .d.....j._"d.S.)
+00001030: 1c7a 7b54 756e 6520 6879 7065 7270 6172  .z{Tune hyperpar
+00001040: 616d 6574 6572 732e 0a0a 2020 2020 2020  ameters...      
+00001050: 2020 416e 2061 6c74 6572 6e61 7469 7665    An alternative
+00001060: 2063 6f6e 6669 6720 6361 6e20 6265 2070   config can be p
+00001070: 726f 7669 6465 6420 746f 206f 7665 7277  rovided to overw
+00001080: 7269 7465 2074 6865 2068 7970 6572 7061  rite the hyperpa
+00001090: 7261 6d65 7465 7220 7365 6172 6368 2073  rameter search s
+000010a0: 7061 6365 2e0a 2020 2020 2020 2020 7a2f  pace..        z/
+000010b0: 3a20 5374 6172 7420 6879 7065 7270 6172  : Start hyperpar
+000010c0: 616d 6574 6572 2074 756e 696e 6720 6f66  ameter tuning of
+000010d0: 2058 6762 6f6f 7374 206d 6f64 656c 2e72   Xgboost model.r
+000010e0: 2700 0000 722c 0000 007a 3941 7420 6c65  '...r,...z9At le
+000010f0: 6173 7420 6f6e 6520 6f66 2074 6865 2063  ast one of the c
+00001100: 6f6e 6669 6773 2069 7320 4e6f 6e65 2c20  onfigs is None, 
+00001110: 7768 6963 6820 6973 206e 6f74 2061 6c6c  which is not all
+00001120: 6f77 6564 6301 0000 0000 0000 0000 0000  owedc...........
+00001130: 000c 0000 0013 0000 0013 0000 0073 e401  .............s..
+00001140: 0000 8801 6a00 6a01 8801 6a00 6a02 8801  ....j.j...j.j...
+00001150: 6a00 6a03 8802 8805 a004 a100 7c00 a005  j.j.........|...
+00001160: 6401 8801 6a00 6a06 8801 6a00 6a07 a103  d...j.j...j.j...
+00001170: 7c00 a008 6402 8801 6a00 6a09 8801 6a00  |...d...j.j...j.
+00001180: 6a0a a103 7c00 a008 6403 8801 6a00 6a0b  j...|...d...j.j.
+00001190: 8801 6a00 6a0c a103 7c00 a008 6404 8801  ..j.j...|...d...
+000011a0: 6a00 6a0d 8801 6a00 6a0e a103 7c00 a005  j.j...j.j...|...
+000011b0: 6405 8801 6a00 6a0f 8801 6a00 6a10 a103  d...j.j...j.j...
+000011c0: 7c00 a008 6406 8801 6a00 6a11 8801 6a00  |...d...j.j...j.
+000011d0: 6a12 a103 7c00 a008 6407 8801 6a00 6a13  j...|...d...j.j.
+000011e0: 8801 6a00 6a14 a103 7c00 a008 6408 8801  ..j.j...|...d...
+000011f0: 6a00 6a15 8801 6a00 6a16 a103 8801 6a00  j.j...j.j.....j.
+00001200: 6a17 7c00 a005 6409 8801 6a00 6a18 8801  j.|...d...j.j...
+00001210: 6a00 6a19 a103 640a 9c0f 7d01 7c00 a01a  j.j...d...}.|...
+00001220: 640b 640c 640d 6702 a102 7d02 7c02 9001  d.d.d.g...}.|...
+00001230: 7212 8801 a01b 8805 a101 7d03 741c 6a1d  r.........}.t.j.
+00001240: 8803 8805 7c03 8801 6a1e 6a1f 640e 8d04  ....|...j.j.d...
+00001250: 7d04 6e14 741c 6a1d 8803 8805 8801 6a1e  }.n.t.j.......j.
+00001260: 6a1f 640f 8d03 7d04 7420 6a21 a022 7c00  j.d...}.t j!."|.
+00001270: 6410 a102 7d05 8801 6a1e 6a23 6411 6b02  d...}...j.j#d.k.
+00001280: 9001 72a8 7c04 6412 6602 8800 6413 6602  ..r.|.d.f...d.f.
+00001290: 6702 7d06 741c 6a24 7c01 7c04 7c01 6409  g.}.t.j$|.|.|.d.
+000012a0: 1900 8801 6a1e 6a25 7c06 7c05 6701 8801  ....j.j%|.|.g...
+000012b0: 6a00 6a03 6414 8d07 7d07 7c07 a026 8800  j.j.d...}.|..&..
+000012c0: a101 7d08 7427 a028 6415 6416 8400 7c08  ..}.t'.(d.d...|.
+000012d0: 4400 8301 a101 7d09 7429 8804 7c09 8302  D.....}.t)..|...
+000012e0: 6417 1400 7d0a 7c0a 5300 741c 6a2a 7c01  d...}.|.S.t.j*|.
+000012f0: 7c04 7c01 6409 1900 8801 6a1e 6a23 640c  |.|.d.....j.j#d.
+00001300: 8801 6a1e 6a2b 7c05 6701 8801 6a1e 6a2c  ..j.j+|.g...j.j,
+00001310: 6418 8d08 7d0b 7c0b 6419 1900 a02d a100  d...}.|.d....-..
+00001320: 5300 6400 5300 291a 4eda 096d 6178 5f64  S.d.S.).N..max_d
+00001330: 6570 7468 da05 616c 7068 61da 066c 616d  epth..alpha..lam
+00001340: 6264 61da 106d 696e 5f63 6869 6c64 5f77  bda..min_child_w
+00001350: 6569 6768 74da 0a6e 756d 5f6c 6561 7665  eight..num_leave
+00001360: 73da 0973 7562 7361 6d70 6c65 da10 636f  s..subsample..co
+00001370: 6c73 616d 706c 655f 6279 7472 6565 da11  lsample_bytree..
+00001380: 636f 6c73 616d 706c 655f 6279 6c65 7665  colsample_byleve
+00001390: 6c72 3000 0000 290f da09 6f62 6a65 6374  lr0...)...object
+000013a0: 6976 65da 0b65 7661 6c5f 6d65 7472 6963  ive..eval_metric
+000013b0: da07 7665 7262 6f73 65da 0b74 7265 655f  ..verbose..tree_
+000013c0: 6d65 7468 6f64 da09 6e75 6d5f 636c 6173  method..num_clas
+000013d0: 7372 4500 0000 7246 0000 0072 4700 0000  srE...rF...rG...
+000013e0: 7248 0000 0072 4900 0000 724a 0000 0072  rH...rI...rJ...r
+000013f0: 4b00 0000 724c 0000 00da 0365 7461 7230  K...rL.....etar0
+00001400: 0000 0072 3b00 0000 5446 7228 0000 0072  ...r;...TFr(...r
+00001410: 2c00 0000 7a0d 7465 7374 2d6d 6c6f 676c  ,...z.test-mlogl
+00001420: 6f73 7372 2f00 0000 722d 0000 0072 2e00  ossr/...r-...r..
+00001430: 0000 2905 7231 0000 0072 3200 0000 7233  ..).r1...r2...r3
+00001440: 0000 00da 0963 616c 6c62 6163 6b73 da0c  .....callbacks..
+00001450: 7665 7262 6f73 655f 6576 616c 6301 0000  verbose_evalc...
+00001460: 0000 0000 0000 0000 0002 0000 0005 0000  ................
+00001470: 0053 0000 0073 1600 0000 6700 7c00 5d0e  .S...s....g.|.].
+00001480: 7d01 7400 a001 7c01 a101 9102 7104 5300  }.t...|.....q.S.
+00001490: 7218 0000 00a9 02da 026e 70da 0661 7267  r........np..arg
+000014a0: 6d61 78a9 02da 022e 30da 046c 696e 6572  max.....0..liner
+000014b0: 1800 0000 7218 0000 0072 1900 0000 da0a  ....r....r......
+000014c0: 3c6c 6973 7463 6f6d 703e fb00 0000 7304  <listcomp>....s.
+000014d0: 0000 0006 0002 007a 3c58 6762 6f6f 7374  .......z<Xgboost
+000014e0: 4d6f 6465 6c2e 6175 746f 7475 6e65 2e3c  Model.autotune.<
+000014f0: 6c6f 6361 6c73 3e2e 6f62 6a65 6374 6976  locals>.objectiv
+00001500: 652e 3c6c 6f63 616c 733e 2e3c 6c69 7374  e.<locals>.<list
+00001510: 636f 6d70 3ee9 ffff ffff 2908 7240 0000  comp>.....).r@..
+00001520: 00da 0664 7472 6169 6e72 3100 0000 da05  ...dtrainr1.....
+00001530: 6e66 6f6c 64da 0961 735f 7061 6e64 6173  nfold..as_pandas
+00001540: da04 7365 6564 7253 0000 00da 0773 6875  ..seedrS.....shu
+00001550: 6666 6c65 7a12 7465 7374 2d6d 6c6f 676c  fflez.test-mlogl
+00001560: 6f73 732d 6d65 616e 292e 7214 0000 00da  oss-mean).r.....
+00001570: 0f6d 6f64 656c 5f6f 626a 6563 7469 7665  .model_objective
+00001580: da11 6d6f 6465 6c5f 6576 616c 5f6d 6574  ..model_eval_met
+00001590: 7269 63da 0f6d 6f64 656c 5f76 6572 626f  ric..model_verbo
+000015a0: 7369 7479 da07 6e75 6e69 7175 65da 0b73  sity..nunique..s
+000015b0: 7567 6765 7374 5f69 6e74 da0d 6d61 785f  uggest_int..max_
+000015c0: 6465 7074 685f 6d69 6eda 0d6d 6178 5f64  depth_min..max_d
+000015d0: 6570 7468 5f6d 6178 da0d 7375 6767 6573  epth_max..sugges
+000015e0: 745f 666c 6f61 74da 0961 6c70 6861 5f6d  t_float..alpha_m
+000015f0: 696e da09 616c 7068 615f 6d61 78da 0a6c  in..alpha_max..l
+00001600: 616d 6264 615f 6d69 6eda 0a6c 616d 6264  ambda_min..lambd
+00001610: 615f 6d61 78da 146d 696e 5f63 6869 6c64  a_max..min_child
+00001620: 5f77 6569 6768 745f 6d69 6eda 146d 696e  _weight_min..min
+00001630: 5f63 6869 6c64 5f77 6569 6768 745f 6d61  _child_weight_ma
+00001640: 78da 0e6e 756d 5f6c 6561 7665 735f 6d69  x..num_leaves_mi
+00001650: 6eda 0e6e 756d 5f6c 6561 7665 735f 6d61  n..num_leaves_ma
+00001660: 78da 0e73 7562 5f73 616d 706c 655f 6d69  x..sub_sample_mi
+00001670: 6eda 0e73 7562 5f73 616d 706c 655f 6d61  n..sub_sample_ma
+00001680: 78da 1663 6f6c 5f73 616d 706c 655f 6279  x..col_sample_by
+00001690: 5f74 7265 655f 6d69 6eda 1663 6f6c 5f73  _tree_min..col_s
+000016a0: 616d 706c 655f 6279 5f74 7265 655f 6d61  ample_by_tree_ma
+000016b0: 78da 1763 6f6c 5f73 616d 706c 655f 6279  x..col_sample_by
+000016c0: 5f6c 6576 656c 5f6d 696e da17 636f 6c5f  _level_min..col_
+000016d0: 7361 6d70 6c65 5f62 795f 6c65 7665 6c5f  sample_by_level_
+000016e0: 6d61 7872 5200 0000 da09 7374 6570 735f  maxrR.....steps_
+000016f0: 6d69 6eda 0973 7465 7073 5f6d 6178 da13  min..steps_max..
+00001700: 7375 6767 6573 745f 6361 7465 676f 7269  suggest_categori
+00001710: 6361 6c72 2100 0000 723c 0000 0072 3d00  calr!...r<...r=.
+00001720: 0000 7213 0000 0072 3e00 0000 da06 6f70  ..r....r>.....op
+00001730: 7475 6e61 da0b 696e 7465 6772 6174 696f  tuna..integratio
+00001740: 6eda 1658 4742 6f6f 7374 5072 756e 696e  n..XGBoostPrunin
+00001750: 6743 616c 6c62 6163 6b72 3f00 0000 722d  gCallbackr?...r-
+00001760: 0000 0072 3200 0000 da07 7072 6564 6963  ...r2.....predic
+00001770: 7472 5600 0000 da07 6173 6172 7261 7972  trV.....asarrayr
+00001780: 0700 0000 da02 6376 da13 676c 6f62 616c  ......cv..global
+00001790: 5f72 616e 646f 6d5f 7374 6174 65da 1773  _random_state..s
+000017a0: 6875 6666 6c65 5f64 7572 696e 675f 7472  huffle_during_tr
+000017b0: 6169 6e69 6e67 da04 6d65 616e 290c da05  aining..mean)...
+000017c0: 7472 6961 6cda 0570 6172 616d 723b 0000  trial..paramr;..
+000017d0: 0072 2000 0000 7241 0000 00da 1070 7275  .r ...rA.....pru
+000017e0: 6e69 6e67 5f63 616c 6c62 6163 6b72 4300  ning_callbackrC.
+000017f0: 0000 7216 0000 00da 0570 7265 6473 da0b  ..r......preds..
+00001800: 7072 6564 5f6c 6162 656c 73da 076d 6174  pred_labels..mat
+00001810: 7468 6577 da06 7265 7375 6c74 a906 7242  thew..result..rB
+00001820: 0000 0072 1700 0000 da08 7472 6169 6e5f  ...r......train_
+00001830: 6f6e 7223 0000 0072 2600 0000 7225 0000  onr#...r&...r%..
+00001840: 0072 1800 0000 7219 0000 0072 4d00 0000  .r....r....rM...
+00001850: ad00 0000 73c0 0000 0000 0206 0106 0106  ....s...........
+00001860: 0102 0106 0104 0102 0106 0106 fd02 0504  ................
+00001870: 0102 0006 0006 ff02 0304 0102 0006 0006  ................
+00001880: ff02 0304 0102 0006 0006 ff02 0304 0102  ................
+00001890: 0106 0106 fd02 0504 0102 0106 0106 fd02  ................
+000018a0: 0504 0102 0106 0106 fd02 0504 0102 0106  ................
+000018b0: 0106 fd02 0506 0104 0102 0006 0006 ff02  ................
+000018c0: d706 2d10 0106 010a 0104 0102 0102 0102  ..-.............
+000018d0: 0106 fc08 0704 0102 0102 0106 fd06 0606  ................
+000018e0: 0102 0002 ff04 040e 0110 0104 0102 0102  ................
+000018f0: 0106 0106 0102 0104 0106 f906 090a 0114  ................
+00001900: 010e 0104 0204 0102 0102 0106 0206 0102  ................
+00001910: 0106 0104 0106 f706 0c7a 2858 6762 6f6f  .........z(Xgboo
+00001920: 7374 4d6f 6465 6c2e 6175 746f 7475 6e65  stModel.autotune
+00001930: 2e3c 6c6f 6361 6c73 3e2e 6f62 6a65 6374  .<locals>.object
+00001940: 6976 65da 0778 6762 6f6f 7374 4629 02da  ive..xgboostF)..
+00001950: 0c6d 756c 7469 7661 7269 6174 6572 6000  .multivariater`.
+00001960: 0000 da08 6d69 6e69 6d69 7a65 7a07 2074  ....minimizez. t
+00001970: 756e 696e 6729 03da 0964 6972 6563 7469  uning)...directi
+00001980: 6f6e da07 7361 6d70 6c65 72da 0a73 7475  on..sampler..stu
+00001990: 6479 5f6e 616d 6554 2904 da08 6e5f 7472  dy_nameT)...n_tr
+000019a0: 6961 6c73 da07 7469 6d65 6f75 74da 0e67  ials..timeout..g
+000019b0: 635f 6166 7465 725f 7472 6961 6cda 1173  c_after_trial..s
+000019c0: 686f 775f 7072 6f67 7265 7373 5f62 6172  how_progress_bar
+000019d0: 7245 0000 0072 4600 0000 7247 0000 0072  rE...rF...rG...r
+000019e0: 4900 0000 724a 0000 0072 4b00 0000 724c  I...rJ...rK...rL
+000019f0: 0000 0072 4800 0000 7230 0000 0029 0f72  ...rH...r0...).r
+00001a00: 4d00 0000 724e 0000 0072 4f00 0000 7250  M...rN...rO...rP
+00001a10: 0000 0072 5100 0000 7245 0000 0072 4600  ...rQ...rE...rF.
+00001a20: 0000 7247 0000 0072 4900 0000 724a 0000  ..rG...rI...rJ..
+00001a30: 0072 4b00 0000 724c 0000 0072 4800 0000  .rK...rL...rH...
+00001a40: 7252 0000 0072 3000 0000 7a0d 4265 7374  rR...r0...z.Best
+00001a50: 2070 6172 616d 733a 2072 3b00 0000 4e29   params: r;...N)
+00001a60: 2372 0d00 0000 7202 0000 0072 1e00 0000  #r....r....r....
+00001a70: 7215 0000 0072 1300 0000 7234 0000 0072  r....r....r4...r
+00001a80: 3c00 0000 723d 0000 0072 3e00 0000 720c  <...r=...r>...r.
+00001a90: 0000 0072 2200 0000 7214 0000 0072 7b00  ...r"...r....r{.
+00001aa0: 0000 da08 7361 6d70 6c65 7273 da0a 5450  ....samplers..TP
+00001ab0: 4553 616d 706c 6572 7281 0000 00da 0c63  ESamplerr......c
+00001ac0: 7265 6174 655f 7374 7564 79da 086f 7074  reate_study..opt
+00001ad0: 696d 697a 65da 1c68 7970 6572 7061 7261  imize..hyperpara
+00001ae0: 6d65 7465 725f 7475 6e69 6e67 5f72 6f75  meter_tuning_rou
+00001af0: 6e64 73da 2668 7970 6572 7061 7261 6d65  nds.&hyperparame
+00001b00: 7465 725f 7475 6e69 6e67 5f6d 6178 5f72  ter_tuning_max_r
+00001b10: 756e 7469 6d65 5f73 6563 73da 0d76 6973  untime_secs..vis
+00001b20: 7561 6c69 7a61 7469 6f6e da19 706c 6f74  ualization..plot
+00001b30: 5f6f 7074 696d 697a 6174 696f 6e5f 6869  _optimization_hi
+00001b40: 7374 6f72 79da 0473 686f 77da 1670 6c6f  story..show..plo
+00001b50: 745f 7061 7261 6d5f 696d 706f 7274 616e  t_param_importan
+00001b60: 6365 73da 115a 6572 6f44 6976 6973 696f  ces..ZeroDivisio
+00001b70: 6e45 7272 6f72 da0c 5275 6e74 696d 6545  nError..RuntimeE
+00001b80: 7272 6f72 da0a 6265 7374 5f74 7269 616c  rror..best_trial
+00001b90: 7240 0000 0072 6200 0000 7263 0000 0072  r@...rb...rc...r
+00001ba0: 6400 0000 7265 0000 0072 5200 0000 7237  d...re...rR...r7
+00001bb0: 0000 0072 3b00 0000 290b 7217 0000 0072  ...r;...).r....r
+00001bc0: 2300 0000 7224 0000 0072 2500 0000 7226  #...r$...r%...r&
+00001bd0: 0000 0072 4d00 0000 da09 616c 676f 7269  ...rM.....algori
+00001be0: 7468 6d72 9100 0000 da05 7374 7564 79da  thmr......study.
+00001bf0: 0366 6967 5a12 7867 626f 6f73 745f 6265  .figZ.xgboost_be
+00001c00: 7374 5f70 6172 616d 7218 0000 0072 8b00  st_paramr....r..
+00001c10: 0000 7219 0000 0072 3600 0000 8c00 0000  ..r....r6.......
+00001c20: 7382 0000 0000 0b12 010c 0108 0204 0102  s...............
+00001c30: 0102 0106 fd06 0506 0208 0304 ff02 0204  ................
+00001c40: fe02 0304 fd02 0502 0102 ff04 0416 6004  ..............`.
+00001c50: 0106 0102 0006 ff06 0304 0102 0102 0108  ................
+00001c60: fd06 0604 0102 0106 0106 0102 0102 fb06  ................
+00001c70: 0702 010c 0108 010c 010c 0116 0106 0208  ................
+00001c80: 0206 0106 0106 0102 0106 0102 0102 ff02  ................
+00001c90: 0306 0106 0106 0106 0106 0106 0106 0106  ................
+00001ca0: 0106 ef0a 130e 017a 1558 6762 6f6f 7374  .......z.Xgboost
+00001cb0: 4d6f 6465 6c2e 6175 746f 7475 6e65 2902  Model.autotune).
+00001cc0: da02 6466 721c 0000 0063 0200 0000 0000  ..dfr....c......
+00001cd0: 0000 0000 0000 0600 0000 0400 0000 4300  ..............C.
+00001ce0: 0000 73b4 0000 0074 0074 01a0 02a1 009b  ..s....t.t......
+00001cf0: 0064 019d 0283 0101 007c 006a 0372 1e7c  .d.......|.j.r.|
+00001d00: 006a 0473 2674 0564 0283 0182 0174 066a  .j.s&t.d.....t.j
+00001d10: 077c 017c 006a 046a 0864 038d 027d 027c  .|.|.j.j.d...}.|
+00001d20: 006a 0973 4674 0a64 0483 0182 017c 006a  .j.sFt.d.....|.j
+00001d30: 0b73 5474 0a64 0583 0182 017c 006a 09a0  .sTt.d.....|.j..
+00001d40: 0c7c 02a1 017d 037c 006a 0d64 066b 0272  .|...}.|.j.d.k.r
+00001d50: 8c74 0ea0 0f64 0764 0884 007c 0344 0083  .t...d.d...|.D..
+00001d60: 01a1 017d 047c 047c 006a 0b6a 106b 047d  ...}.|.|.j.j.k.}
+00001d70: 056e 187c 037d 0474 0ea0 0f64 0964 0884  .n.|.}.t...d.d..
+00001d80: 007c 0344 0083 01a1 017d 0574 1164 0a83  .|.D.....}.t.d..
+00001d90: 0101 007c 047c 0566 0253 0029 0b7a 1750  ...|.|.f.S.).z.P
+00001da0: 7265 6469 6374 206f 6e20 756e 7365 656e  redict on unseen
+00001db0: 2064 6174 612e 7a33 3a20 5374 6172 7420   data.z3: Start 
+00001dc0: 7072 6564 6963 7469 6e67 206f 6e20 6e65  predicting on ne
+00001dd0: 7720 6461 7461 2075 7369 6e67 2058 6762  w data using Xgb
+00001de0: 6f6f 7374 206d 6f64 656c 2e72 2700 0000  oost model.r'...
+00001df0: 2901 722b 0000 007a 204e 6f20 7472 6169  ).r+...z No trai
+00001e00: 6e65 6420 6d6f 6465 6c20 6861 7320 6265  ned model has be
+00001e10: 656e 2066 6f75 6e64 2e7a 2b4e 6f20 6d6f  en found.z+No mo
+00001e20: 6465 6c20 636f 6e66 6967 7572 6174 696f  del configuratio
+00001e30: 6e20 6669 6c65 2068 6173 2062 6565 6e20  n file has been 
+00001e40: 666f 756e 642e 7210 0000 0063 0100 0000  found.r....c....
+00001e50: 0000 0000 0000 0000 0200 0000 0400 0000  ................
+00001e60: 5300 0000 7314 0000 0067 007c 005d 0c7d  S...s....g.|.].}
+00001e70: 017c 0164 0019 0091 0271 0453 0029 0172  .|.d.....q.S.).r
+00001e80: 2f00 0000 7218 0000 0072 5800 0000 7218  /...r....rX...r.
+00001e90: 0000 0072 1800 0000 7219 0000 0072 5b00  ...r....r....r[.
+00001ea0: 0000 5201 0000 7304 0000 0006 0002 007a  ..R...s........z
+00001eb0: 2858 6762 6f6f 7374 4d6f 6465 6c2e 7072  (XgboostModel.pr
+00001ec0: 6564 6963 742e 3c6c 6f63 616c 733e 2e3c  edict.<locals>.<
+00001ed0: 6c69 7374 636f 6d70 3e63 0100 0000 0000  listcomp>c......
+00001ee0: 0000 0000 0000 0200 0000 0500 0000 5300  ..............S.
+00001ef0: 0000 7316 0000 0067 007c 005d 0e7d 0174  ..s....g.|.].}.t
+00001f00: 00a0 017c 01a1 0191 0271 0453 0072 1800  ...|.....q.S.r..
+00001f10: 0000 7255 0000 0072 5800 0000 7218 0000  ..rU...rX...r...
+00001f20: 0072 1800 0000 7219 0000 0072 5b00 0000  .r....r....r[...
+00001f30: 5801 0000 7304 0000 0006 0002 007a 1346  X...s........z.F
+00001f40: 696e 6973 6865 6420 7072 6564 6963 7469  inished predicti
+00001f50: 6e67 2912 720d 0000 0072 0200 0000 721e  ng).r....r....r.
+00001f60: 0000 0072 1400 0000 7213 0000 0072 3400  ...r....r....r4.
+00001f70: 0000 723c 0000 0072 3d00 0000 723e 0000  ..r<...r=...r>..
+00001f80: 0072 1600 0000 da09 4578 6365 7074 696f  .r......Exceptio
+00001f90: 6e72 1500 0000 727e 0000 0072 1200 0000  nr....r~...r....
+00001fa0: 7256 0000 0072 7f00 0000 da18 636c 6173  rV...r......clas
+00001fb0: 7369 6669 6361 7469 6f6e 5f74 6872 6573  sification_thres
+00001fc0: 686f 6c64 7237 0000 0029 0672 1700 0000  holdr7...).r....
+00001fd0: 72a7 0000 0072 4200 0000 da0d 7061 7274  r....rB.....part
+00001fe0: 6961 6c5f 7072 6f62 73da 0f70 7265 6469  ial_probs..predi
+00001ff0: 6374 6564 5f70 726f 6273 da11 7072 6564  cted_probs..pred
+00002000: 6963 7465 645f 636c 6173 7365 7372 1800  icted_classesr..
+00002010: 0000 7218 0000 0072 1900 0000 727e 0000  ..r....r....r~..
+00002020: 003d 0100 0073 2c00 0000 0002 0201 0cff  .=...s,.........
+00002030: 0403 0c01 0802 0401 0201 06fe 0605 0601  ................
+00002040: 0802 0601 0802 0c01 0a01 1402 0aff 0404  ................
+00002050: 0401 1401 0801 7a14 5867 626f 6f73 744d  ......z.XgboostM
+00002060: 6f64 656c 2e70 7265 6469 6374 2903 4e4e  odel.predict).NN
+00002070: 4e29 1ada 085f 5f6e 616d 655f 5fda 0a5f  N)...__name__.._
+00002080: 5f6d 6f64 756c 655f 5fda 0c5f 5f71 7561  _module__..__qua
+00002090: 6c6e 616d 655f 5fda 075f 5f64 6f63 5f5f  lname__..__doc__
+000020a0: 7204 0000 0072 0500 0000 7209 0000 0072  r....r....r....r
+000020b0: 0b00 0000 720a 0000 0072 1a00 0000 7239  ....r....r....r9
+000020c0: 0000 00da 0653 6572 6965 7372 0300 0000  .....Seriesr....
+000020d0: da03 7374 72da 0566 6c6f 6174 7221 0000  ..str..floatr!..
+000020e0: 0072 2200 0000 da09 4461 7461 4672 616d  .r".....DataFram
+000020f0: 6572 3c00 0000 da07 426f 6f73 7465 7272  er<.....Boosterr
+00002100: 4400 0000 7236 0000 0072 0600 0000 7256  D...r6...r....rV
+00002110: 0000 00da 076e 6461 7272 6179 727e 0000  .....ndarrayr~..
+00002120: 0072 1800 0000 7218 0000 0072 1800 0000  .r....r....r....
+00002130: 7219 0000 0072 0f00 0000 1a00 0000 7334  r....r........s4
+00002140: 0000 0008 0104 0500 0100 0100 fb02 0206  ................
+00002150: 0106 0106 0106 fb0c 0d1a 0808 1704 0104  ................
+00002160: 0104 0104 0104 fa0c 4704 0104 0104 0104  ........G.......
+00002170: 0102 fa0c 7f00 3272 0f00 0000 291c 72b0  ......2r....).r.
+00002180: 0000 0072 0200 0000 da06 7479 7069 6e67  ...r......typing
+00002190: 7203 0000 0072 0400 0000 7205 0000 0072  r....r....r....r
+000021a0: 0600 0000 da05 6e75 6d70 7972 5600 0000  ......numpyrV...
+000021b0: 727b 0000 00da 0670 616e 6461 7372 3900  r{.....pandasr9.
+000021c0: 0000 728d 0000 0072 3c00 0000 da0f 736b  ..r....r<.....sk
+000021d0: 6c65 6172 6e2e 6d65 7472 6963 7372 0700  learn.metricsr..
+000021e0: 0000 5a0d 736b 6c65 6172 6e2e 7574 696c  ..Z.sklearn.util
+000021f0: 7372 0800 0000 da1f 626c 7565 6361 7374  sr......bluecast
+00002200: 2e63 6f6e 6669 672e 7472 6169 6e69 6e67  .config.training
+00002210: 5f63 6f6e 6669 6772 0900 0000 720a 0000  _configr....r...
+00002220: 0072 0b00 0000 da24 626c 7565 6361 7374  .r.....$bluecast
+00002230: 2e67 656e 6572 616c 5f75 7469 6c73 2e67  .general_utils.g
+00002240: 656e 6572 616c 5f75 7469 6c73 720c 0000  eneral_utilsr...
+00002250: 0072 0d00 0000 5a22 626c 7565 6361 7374  .r....Z"bluecast
+00002260: 2e6d 6c5f 6d6f 6465 6c6c 696e 672e 6261  .ml_modelling.ba
+00002270: 7365 5f63 6c61 7373 6573 720e 0000 0072  se_classesr....r
+00002280: 0f00 0000 7218 0000 0072 1800 0000 7218  ....r....r....r.
+00002290: 0000 0072 1900 0000 da08 3c6d 6f64 756c  ...r......<modul
+000022a0: 653e 0100 0000 7318 0000 0004 060c 0118  e>....s.........
+000022b0: 0208 0108 0108 0108 010c 010c 0214 0510  ................
+000022c0: 010c 03                                  ...
```

### Comparing `bluecast-0.5/bluecast/ml_modelling/base_classes.py` & `bluecast-0.7/bluecast/ml_modelling/base_classes.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.5/bluecast/ml_modelling/xgboost.py` & `bluecast-0.7/bluecast/ml_modelling/xgboost.py`

 * *Files 6% similar despite different names*

```diff
@@ -94,19 +94,32 @@
              param 'use_full_data_for_final_model'"""
             )
             x_train = pd.concat([x_train, x_test])
             y_train = pd.concat([y_train, y_test])
 
         if self.conf_params_xgboost.sample_weight:
             classes_weights = self.calculate_class_weights(y_train)
-            d_train = xgb.DMatrix(x_train, label=y_train, weight=classes_weights)
+            d_train = xgb.DMatrix(
+                x_train,
+                label=y_train,
+                weight=classes_weights,
+                enable_categorical=self.conf_training.cat_encoding_via_ml_algorithm,
+            )
         else:
-            d_train = xgb.DMatrix(x_train, label=y_train)
+            d_train = xgb.DMatrix(
+                x_train,
+                label=y_train,
+                enable_categorical=self.conf_training.cat_encoding_via_ml_algorithm,
+            )
 
-        d_test = xgb.DMatrix(x_test, label=y_test)
+        d_test = xgb.DMatrix(
+            x_test,
+            label=y_test,
+            enable_categorical=self.conf_training.cat_encoding_via_ml_algorithm,
+        )
         eval_set = [(d_train, "train"), (d_test, "test")]
 
         if self.conf_training.hypertuning_cv_folds == 1:
             self.model = xgb.train(
                 self.conf_params_xgboost.params,
                 d_train,
                 num_boost_round=self.conf_params_xgboost.params["steps"],
@@ -114,14 +127,15 @@
                 evals=eval_set,
             )
         else:
             self.model = xgb.train(
                 self.conf_params_xgboost.params,
                 d_train,
                 num_boost_round=self.conf_params_xgboost.params["steps"],
+                # early_stopping_rounds=self.conf_training.early_stopping_rounds,
                 evals=eval_set,
             )
         print("Finished training")
         return self.model
 
     def autotune(
         self,
@@ -131,15 +145,22 @@
         y_test: pd.Series,
     ) -> None:
         """Tune hyperparameters.
 
         An alternative config can be provided to overwrite the hyperparameter search space.
         """
         logger(f"{datetime.utcnow()}: Start hyperparameter tuning of Xgboost model.")
-        d_test = xgb.DMatrix(x_test, label=y_test)
+        if not self.conf_params_xgboost or not self.conf_training:
+            raise ValueError("conf_params_xgboost or conf_training is None")
+
+        d_test = xgb.DMatrix(
+            x_test,
+            label=y_test,
+            enable_categorical=self.conf_training.cat_encoding_via_ml_algorithm,
+        )
         train_on = check_gpu_support()
 
         self.check_load_confs()
 
         if (
             not self.conf_params_xgboost
             or not self.conf_training
@@ -163,14 +184,19 @@
                 ),
                 "alpha": trial.suggest_float(
                     "alpha", self.conf_xgboost.alpha_min, self.conf_xgboost.alpha_max
                 ),
                 "lambda": trial.suggest_float(
                     "lambda", self.conf_xgboost.lambda_min, self.conf_xgboost.lambda_max
                 ),
+                "min_child_weight": trial.suggest_float(
+                    "min_child_weight",
+                    self.conf_xgboost.min_child_weight_min,
+                    self.conf_xgboost.min_child_weight_max,
+                ),
                 "num_leaves": trial.suggest_int(
                     "num_leaves",
                     self.conf_xgboost.num_leaves_min,
                     self.conf_xgboost.num_leaves_max,
                 ),
                 "subsample": trial.suggest_float(
                     "subsample",
@@ -183,40 +209,34 @@
                     self.conf_xgboost.col_sample_by_tree_max,
                 ),
                 "colsample_bylevel": trial.suggest_float(
                     "colsample_bylevel",
                     self.conf_xgboost.col_sample_by_level_min,
                     self.conf_xgboost.col_sample_by_level_max,
                 ),
-                "colsample_bynode": trial.suggest_float(
-                    "colsample_bynode",
-                    self.conf_xgboost.col_sample_by_node_min,
-                    self.conf_xgboost.col_sample_by_node_max,
-                ),
-                "min_child_samples": trial.suggest_int(
-                    "min_child_samples",
-                    self.conf_xgboost.min_child_samples_min,
-                    self.conf_xgboost.min_child_samples_max,
-                ),
                 "eta": self.conf_xgboost.eta,
                 "steps": trial.suggest_int(
                     "steps", self.conf_xgboost.steps_min, self.conf_xgboost.steps_max
                 ),
-                "num_parallel_tree": trial.suggest_int(
-                    "num_parallel_tree",
-                    self.conf_xgboost.num_parallel_tree_min,
-                    self.conf_xgboost.num_parallel_tree_max,
-                ),
             }
             sample_weight = trial.suggest_categorical("sample_weight", [True, False])
             if sample_weight:
                 classes_weights = self.calculate_class_weights(y_train)
-                d_train = xgb.DMatrix(x_train, label=y_train, weight=classes_weights)
+                d_train = xgb.DMatrix(
+                    x_train,
+                    label=y_train,
+                    weight=classes_weights,
+                    enable_categorical=self.conf_training.cat_encoding_via_ml_algorithm,
+                )
             else:
-                d_train = xgb.DMatrix(x_train, label=y_train)
+                d_train = xgb.DMatrix(
+                    x_train,
+                    label=y_train,
+                    enable_categorical=self.conf_training.cat_encoding_via_ml_algorithm,
+                )
 
             pruning_callback = optuna.integration.XGBoostPruningCallback(
                 trial, "test-mlogloss"
             )
 
             if self.conf_training.hypertuning_cv_folds == 1:
                 eval_set = [(d_train, "train"), (d_test, "test")]
@@ -246,15 +266,15 @@
                     shuffle=self.conf_training.shuffle_during_training,
                 )
 
                 return result["test-mlogloss-mean"].mean()
 
         algorithm = "xgboost"
         sampler = optuna.samplers.TPESampler(
-            multivariate=True, seed=self.conf_training.global_random_state
+            multivariate=False, seed=self.conf_training.global_random_state
         )
         study = optuna.create_study(
             direction="minimize",
             sampler=sampler,
             study_name=f"{algorithm} tuning",
         )
 
@@ -285,30 +305,34 @@
             ],  # maximum depth of the decision trees being trained
             "alpha": xgboost_best_param["alpha"],
             "lambda": xgboost_best_param["lambda"],
             "num_leaves": xgboost_best_param["num_leaves"],
             "subsample": xgboost_best_param["subsample"],
             "colsample_bytree": xgboost_best_param["colsample_bytree"],
             "colsample_bylevel": xgboost_best_param["colsample_bylevel"],
-            "colsample_bynode": xgboost_best_param["colsample_bynode"],
-            "min_child_samples": xgboost_best_param["min_child_samples"],
+            "min_child_weight": xgboost_best_param["min_child_weight"],
             "eta": self.conf_xgboost.eta,
             "steps": xgboost_best_param["steps"],
-            "num_parallel_tree": xgboost_best_param["num_parallel_tree"],
         }
         print("Best params: ", self.conf_params_xgboost.params)
         self.conf_params_xgboost.sample_weight = xgboost_best_param["sample_weight"]
 
     def predict(self, df: pd.DataFrame) -> Tuple[np.ndarray, np.ndarray]:
         """Predict on unseen data."""
         logger(
             f"{datetime.utcnow()}: Start predicting on new data using Xgboost model."
         )
-        print("++++++++++++++++++++++++++++")
-        d_test = xgb.DMatrix(df)
+        if not self.conf_xgboost or not self.conf_training:
+            raise ValueError("conf_params_xgboost or conf_training is None")
+
+        d_test = xgb.DMatrix(
+            df,
+            enable_categorical=self.conf_training.cat_encoding_via_ml_algorithm,
+        )
+
         if not self.model:
             raise Exception("No trained model has been found.")
 
         if not self.conf_params_xgboost:
             raise Exception("No model configuration file has been found.")
 
         partial_probs = self.model.predict(d_test)
```

### Comparing `bluecast-0.5/bluecast/preprocessing/__pycache__/custom.cpython-310.pyc` & `bluecast-0.7/bluecast/preprocessing/__pycache__/custom.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.5/bluecast/preprocessing/__pycache__/datetime_features.cpython-310.pyc` & `bluecast-0.7/bluecast/preprocessing/__pycache__/datetime_features.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.5/bluecast/preprocessing/__pycache__/datetime_features.cpython-38.pyc` & `bluecast-0.7/bluecast/preprocessing/__pycache__/datetime_features.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.5/bluecast/preprocessing/__pycache__/encode_target_labels.cpython-310.pyc` & `bluecast-0.7/bluecast/preprocessing/__pycache__/encode_target_labels.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.5/bluecast/preprocessing/__pycache__/encode_target_labels.cpython-38.pyc` & `bluecast-0.7/bluecast/preprocessing/__pycache__/encode_target_labels.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.5/bluecast/preprocessing/__pycache__/feature_selection.cpython-310.pyc` & `bluecast-0.7/bluecast/preprocessing/__pycache__/feature_selection.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun Jun 25 05:34:02 2023 UTC, .py size: 1890 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 cad1 9764 6207 0000  o..........db...
+00000000: 6f0d 0d0a 0000 0000 945b 9a64 6207 0000  o........[.db...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 8000 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d00 5a00 0100 6400 6402 6c01  d.l.m.Z...d.d.l.
 00000040: 6d02 5a02 6d03 5a03 0100 6400 6403 6c04  m.Z.m.Z...d.d.l.
 00000050: 5a05 6400 6403 6c06 5a07 6400 6404 6c08  Z.d.d.l.Z.d.d.l.
 00000060: 6d09 5a09 0100 6400 6405 6c0a 6d0b 5a0b  m.Z...d.d.l.m.Z.
 00000070: 6d0c 5a0c 0100 6400 6406 6c0d 6d0e 5a0e  m.Z...d.d.l.m.Z.
```

### Comparing `bluecast-0.5/bluecast/preprocessing/__pycache__/feature_types.cpython-310.pyc` & `bluecast-0.7/bluecast/preprocessing/__pycache__/feature_types.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.5/bluecast/preprocessing/__pycache__/feature_types.cpython-38.pyc` & `bluecast-0.7/bluecast/preprocessing/__pycache__/feature_types.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Thu Jun  8 04:28:32 2023 UTC, .py size: 6054 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 10% similar despite different names*

```diff
@@ -1,286 +1,286 @@
-00000000: 550d 0d0a 0000 0000 f058 8164 a617 0000  U........X.d....
+00000000: 550d 0d0a 0000 0000 a385 9264 2e18 0000  U..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0003 0000 0040 0000 0073 3a00 0000 6400  .....@...s:...d.
+00000020: 0003 0000 0040 0000 0073 3600 0000 6400  .....@...s6...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 6d03 5a03  Z.d.d.l.m.Z.m.Z.
-00000040: 6d04 5a04 6d05 5a05 6d06 5a06 0100 6401  m.Z.m.Z.m.Z...d.
-00000050: 6403 6c07 5a08 4700 6404 6405 8400 6405  d.l.Z.G.d.d...d.
-00000060: 8302 5a09 6403 5300 2906 7ae3 0a46 6561  ..Z.d.S.).z..Fea
-00000070: 7475 7265 2074 7970 6520 6465 7465 6374  ture type detect
-00000080: 696f 6e20 616e 6420 6361 7374 696e 672e  ion and casting.
-00000090: 0a0a 5468 6973 2069 7320 6120 636f 6e76  ..This is a conv
-000000a0: 656e 6965 6e63 6520 636c 6173 7320 746f  enience class to
-000000b0: 2064 6574 6563 7420 616e 6420 6361 7374   detect and cast
-000000c0: 2066 6561 7475 7265 2074 7970 6573 2069   feature types i
-000000d0: 6e20 6120 4461 7461 4672 616d 652e 2049  n a DataFrame. I
-000000e0: 7420 6361 6e20 6265 2075 7365 6420 746f  t can be used to
-000000f0: 2064 6574 6563 7420 6e75 6d65 7269 6361   detect numerica
-00000100: 6c2c 0a63 6174 6567 6f72 6963 616c 2061  l,.categorical a
-00000110: 6e64 2064 6174 6574 696d 6520 636f 6c75  nd datetime colu
-00000120: 6d6e 732e 2049 7420 616c 736f 2063 6173  mns. It also cas
-00000130: 7473 2063 6f6c 756d 6e73 2074 6f20 6120  ts columns to a 
-00000140: 7370 6563 6966 6963 2074 7970 652e 0ae9  specific type...
-00000150: 0000 0000 2905 da04 4469 6374 da04 4c69  ....)...Dict..Li
-00000160: 7374 da08 4f70 7469 6f6e 616c da05 5475  st..Optional..Tu
-00000170: 706c 65da 0555 6e69 6f6e 4e63 0000 0000  ple..UnionNc....
-00000180: 0000 0000 0000 0000 0000 0000 0900 0000  ................
-00000190: 4000 0000 7320 0100 0065 005a 0164 005a  @...s ...e.Z.d.Z
-000001a0: 0264 015a 0364 1765 0465 0565 0665 0765  .d.Z.d.e.e.e.e.e
-000001b0: 0865 0966 0319 0019 0019 0065 0465 0565  .e.f.......e.e.e
-000001c0: 0665 0765 0865 0966 0319 0019 0019 0065  .e.e.e.f.......e
-000001d0: 0465 0565 0665 0765 0865 0966 0319 0019  .e.e.e.e.e.f....
-000001e0: 0019 0064 039c 0364 0464 0584 055a 0a65  ...d...d.d...Z.e
-000001f0: 0b6a 0c64 069c 0164 0764 0884 045a 0d65  .j.d...d.d...Z.e
-00000200: 0b6a 0c65 0e65 0565 0665 0765 0965 0866  .j.e.e.e.e.e.e.f
-00000210: 0319 0019 0065 0565 0665 0765 0965 0866  .....e.e.e.e.e.f
-00000220: 0319 0019 0066 0219 0064 099c 0264 0a64  .....f...d...d.d
-00000230: 0b84 045a 0f65 0b6a 0c65 0565 0665 0765  ...Z.e.j.e.e.e.e
-00000240: 0965 0866 0319 0019 0064 0c9c 0264 0d64  .e.f.....d...d.d
-00000250: 0e84 045a 1065 0b6a 0c65 0565 0665 0765  ...Z.e.j.e.e.e.e
-00000260: 0965 0866 0319 0019 0065 0b6a 0c64 0f9c  .e.f.....e.j.d..
-00000270: 0364 1064 1184 045a 1165 0b6a 0c65 0b6a  .d.d...Z.e.j.e.j
-00000280: 0c64 099c 0264 1264 1384 045a 1264 1865  .d...d.d...Z.d.e
-00000290: 0b6a 0c65 0565 0665 0765 0965 0864 0266  .j.e.e.e.e.e.d.f
-000002a0: 0419 0019 0065 0b6a 0c64 149c 0364 1564  .....e.j.d...d.d
-000002b0: 1684 055a 1364 0253 0029 19da 1346 6561  ...Z.d.S.)...Fea
-000002c0: 7475 7265 5479 7065 4465 7465 6374 6f72  tureTypeDetector
-000002d0: 7aa9 4465 7465 6374 2061 6e64 2063 6173  z.Detect and cas
-000002e0: 7420 6665 6174 7572 6520 7479 7065 7320  t feature types 
-000002f0: 696e 2044 6174 6146 7261 6d65 2e0a 0a20  in DataFrame... 
-00000300: 2020 2043 6f6c 756d 6e20 6e61 6d65 7320     Column names 
-00000310: 666f 7220 696e 6469 7669 6475 616c 2066  for individual f
-00000320: 6561 7475 7265 2074 7970 6573 2063 616e  eature types can
-00000330: 2062 6520 7072 6f76 6964 6564 2e20 4f74   be provided. Ot
-00000340: 6865 7277 6973 6520 7479 7065 7320 7769  herwise types wi
-00000350: 6c6c 2062 6520 696e 6665 7272 6564 2061  ll be inferred a
-00000360: 6e64 2063 6173 7465 6420 6163 636f 7264  nd casted accord
-00000370: 696e 676c 792e 0a20 2020 204e 2903 da0b  ingly..    N)...
-00000380: 6e75 6d5f 636f 6c75 6d6e 73da 0b63 6174  num_columns..cat
-00000390: 5f63 6f6c 756d 6e73 da0c 6461 7465 5f63  _columns..date_c
-000003a0: 6f6c 756d 6e73 6304 0000 0000 0000 0000  olumnsc.........
-000003b0: 0000 0004 0000 0007 0000 0043 0000 0073  ...........C...s
-000003c0: 3000 0000 7c01 7c00 5f00 7c02 7c00 5f01  0...|.|._.|.|._.
-000003d0: 7c03 7c00 5f02 6900 7c00 5f03 6401 6402  |.|._.i.|._.d.d.
-000003e0: 6403 6404 6405 6406 6407 6707 7c00 5f04  d.d.d.d.d.g.|._.
-000003f0: 6400 5300 2908 4eda 0469 6e74 38da 0569  d.S.).N..int8..i
-00000400: 6e74 3136 da05 696e 7433 32da 0569 6e74  nt16..int32..int
-00000410: 3634 da07 666c 6f61 7431 36da 0766 6c6f  64..float16..flo
-00000420: 6174 3332 da07 666c 6f61 7436 3429 0572  at32..float64).r
-00000430: 0800 0000 7209 0000 0072 0a00 0000 da12  ....r....r......
-00000440: 6465 7465 6374 6564 5f63 6f6c 5f74 7970  detected_col_typ
-00000450: 6573 da0a 6e75 6d5f 6474 7970 6573 2904  es..num_dtypes).
-00000460: da04 7365 6c66 7208 0000 0072 0900 0000  ..selfr....r....
-00000470: 720a 0000 00a9 0072 1500 0000 fa4a 2f68  r......r.....J/h
-00000480: 6f6d 652f 7468 6f6d 6173 2f49 6465 6150  ome/thomas/IdeaP
-00000490: 726f 6a65 6374 732f 426c 7565 4361 7374  rojects/BlueCast
-000004a0: 2f62 6c75 6563 6173 742f 7072 6570 726f  /bluecast/prepro
-000004b0: 6365 7373 696e 672f 6665 6174 7572 655f  cessing/feature_
-000004c0: 7479 7065 732e 7079 da08 5f5f 696e 6974  types.py..__init
-000004d0: 5f5f 1200 0000 7318 0000 0000 0606 0106  __....s.........
-000004e0: 0106 0106 0202 0102 0102 0102 0102 0102  ................
-000004f0: 0102 f97a 1c46 6561 7475 7265 5479 7065  ...z.FeatureType
-00000500: 4465 7465 6374 6f72 2e5f 5f69 6e69 745f  Detector.__init_
-00000510: 5f29 01da 0264 6663 0200 0000 0000 0000  _)...dfc........
-00000520: 0000 0000 0600 0000 0500 0000 4300 0000  ............C...
-00000530: 7346 0000 007c 006a 0073 4067 007d 027c  sF...|.j.s@g.}.|
-00000540: 006a 0144 005d 287d 037c 016a 027c 0367  .j.D.](}.|.j.|.g
-00000550: 0164 018d 016a 037d 047c 0444 005d 0e7d  .d...j.}.|.D.].}
-00000560: 057c 02a0 047c 05a1 0101 0071 2871 107c  .|...|.....q(q.|
-00000570: 027c 005f 007c 006a 0053 0029 027a 3f49  .|._.|.j.S.).z?I
-00000580: 6465 6e74 6966 7920 6e75 6d65 7269 6361  dentify numerica
-00000590: 6c20 636f 6c75 6d6e 7320 6261 7365 6420  l columns based 
-000005a0: 6f6e 2061 6c72 6561 6479 2065 7869 7374  on already exist
-000005b0: 696e 6720 6461 7461 2074 7970 652e 2901  ing data type.).
-000005c0: da07 696e 636c 7564 6529 0572 0800 0000  ..include).r....
-000005d0: 7213 0000 00da 0d73 656c 6563 745f 6474  r......select_dt
-000005e0: 7970 6573 da07 636f 6c75 6d6e 73da 0661  ypes..columns..a
-000005f0: 7070 656e 6429 0672 1400 0000 7218 0000  ppend).r....r...
-00000600: 00da 0c6e 756d 5f63 6f6c 5f6c 6973 74da  ...num_col_list.
-00000610: 0776 6172 7479 7065 da08 6e75 6d5f 636f  .vartype..num_co
-00000620: 6c73 da03 636f 6c72 1500 0000 7215 0000  ls..colr....r...
-00000630: 0072 1600 0000 da14 6964 656e 7469 6679  .r......identify
-00000640: 5f6e 756d 5f63 6f6c 756d 6e73 2600 0000  _num_columns&...
-00000650: 7310 0000 0000 0306 0104 010a 0110 0108  s...............
-00000660: 010e 0106 017a 2846 6561 7475 7265 5479  .....z(FeatureTy
-00000670: 7065 4465 7465 6374 6f72 2e69 6465 6e74  peDetector.ident
-00000680: 6966 795f 6e75 6d5f 636f 6c75 6d6e 7329  ify_num_columns)
-00000690: 0272 1800 0000 da06 7265 7475 726e 6302  .r......returnc.
-000006a0: 0000 0000 0000 0000 0000 0006 0000 0008  ................
-000006b0: 0000 0043 0000 0073 8800 0000 7400 7c01  ...C...s....t.|.
-000006c0: a001 6401 6701 a101 8301 7d02 7c02 4400  ..d.g.....}.|.D.
-000006d0: 5d20 7d03 7c01 7c03 1900 a002 7403 a101  ] }.|.|.....t...
-000006e0: 7c01 7c03 3c00 6401 7c00 6a04 7c03 3c00  |.|.<.d.|.j.|.<.
-000006f0: 7114 7a2a 7c01 6a05 6402 6402 8502 7c01  q.z*|.j.d.d...|.
-00000700: 6a06 a007 7c02 a101 0f00 6602 1900 7d04  j...|.....f...}.
-00000710: 7c04 6a06 a008 a100 7d05 5700 6e1e 0400  |.j.....}.W.n...
-00000720: 7409 6b0a 727e 0100 0100 0100 7c01 6a06  t.k.r~......|.j.
-00000730: a008 a100 7d05 5900 6e02 5800 7c02 7c05  ....}.Y.n.X.|.|.
-00000740: 6602 5300 2903 7a2b 4964 656e 7469 6679  f.S.).z+Identify
-00000750: 2062 6f6f 6c65 616e 2063 6f6c 756d 6e73   boolean columns
-00000760: 2062 6173 6564 206f 6e20 6461 7461 2074   based on data t
-00000770: 7970 65da 0462 6f6f 6c4e 290a da04 6c69  ype..boolN)...li
-00000780: 7374 721a 0000 00da 0661 7374 7970 6572  str......astyper
-00000790: 2300 0000 7212 0000 00da 036c 6f63 721b  #...r......locr.
-000007a0: 0000 00da 0469 7369 6eda 0774 6f5f 6c69  .....isin..to_li
-000007b0: 7374 da09 4578 6365 7074 696f 6e29 0672  st..Exception).r
-000007c0: 1400 0000 7218 0000 00da 0962 6f6f 6c5f  ....r......bool_
-000007d0: 636f 6c73 7220 0000 00da 0a6e 6f5f 626f  colsr .....no_bo
-000007e0: 6f6c 5f64 66da 0c6e 6f5f 626f 6f6c 5f63  ol_df..no_bool_c
-000007f0: 6f6c 7372 1500 0000 7215 0000 0072 1600  olsr....r....r..
-00000800: 0000 da15 6964 656e 7469 6679 5f62 6f6f  ....identify_boo
-00000810: 6c5f 636f 6c75 6d6e 7332 0000 0073 1400  l_columns2...s..
-00000820: 0000 0004 1001 0801 1201 0c03 0201 1c01  ................
-00000830: 0e01 0e01 1001 7a29 4665 6174 7572 6554  ......z)FeatureT
-00000840: 7970 6544 6574 6563 746f 722e 6964 656e  ypeDetector.iden
-00000850: 7469 6679 5f62 6f6f 6c5f 636f 6c75 6d6e  tify_bool_column
-00000860: 7329 0272 1800 0000 722c 0000 0063 0300  s).r....r,...c..
-00000870: 0000 0000 0000 0000 0000 0500 0000 0900  ................
-00000880: 0000 4300 0000 73ea 0000 007c 006a 0072  ..C...s....|.j.r
-00000890: 747c 006a 0172 7467 007d 037c 006a 0044  t|.j.rtg.}.|.j.D
-000008a0: 005d 567d 047c 047c 006a 016b 0772 167a  .]V}.|.|.j.k.r.z
-000008b0: 3274 026a 037c 017c 0419 0064 0164 028d  2t.j.|.|...d.d..
-000008c0: 027c 017c 043c 007c 03a0 047c 04a1 0101  .|.|.<.|...|....
-000008d0: 0064 037c 006a 0574 067c 0483 013c 0057  .d.|.j.t.|...<.W
-000008e0: 0071 1604 0074 076b 0a72 6a01 0001 0001  .q...t.k.rj.....
-000008f0: 0059 0071 1658 0071 167c 037c 005f 007c  .Y.q.X.q.|.|._.|
-00000900: 006a 0073 e67c 006a 0172 e667 007d 037c  .j.s.|.j.r.g.}.|
-00000910: 0244 005d 567d 047c 047c 006a 016b 0772  .D.]V}.|.|.j.k.r
-00000920: 887a 3274 026a 037c 017c 0419 0064 0164  .z2t.j.|.|...d.d
-00000930: 028d 027c 017c 043c 007c 03a0 047c 04a1  ...|.|.<.|...|..
-00000940: 0101 0064 037c 006a 0574 067c 0483 013c  ...d.|.j.t.|...<
-00000950: 0057 0071 8804 0074 076b 0a72 dc01 0001  .W.q...t.k.r....
-00000960: 0001 0059 0071 8858 0071 887c 037c 005f  ...Y.q.X.q.|.|._
-00000970: 0064 0453 0029 057a 4454 7279 2063 6173  .d.S.).zDTry cas
-00000980: 7469 6e67 2074 6f20 6461 7465 7469 6d65  ting to datetime
-00000990: 2e20 4578 7065 6374 6564 2069 7320 6120  . Expected is a 
-000009a0: 6461 7465 7469 6d65 2066 6f72 6d61 7420  datetime format 
-000009b0: 6f66 2059 5959 592d 4d4d 2d44 4454 a901  of YYYY-MM-DDT..
-000009c0: da09 7965 6172 6669 7273 74fa 0c64 6174  ..yearfirst..dat
-000009d0: 6574 696d 655b 6e73 5d4e 2908 720a 0000  etime[ns]N).r...
-000009e0: 0072 0800 0000 da02 7064 da0b 746f 5f64  .r......pd..to_d
-000009f0: 6174 6574 696d 6572 1c00 0000 7212 0000  atetimer....r...
-00000a00: 00da 0373 7472 7229 0000 0029 0572 1400  ...strr)...).r..
-00000a10: 0000 7218 0000 0072 2c00 0000 720a 0000  ..r....r,...r...
-00000a20: 0072 2000 0000 7215 0000 0072 1500 0000  .r ...r....r....
-00000a30: 7216 0000 00da 1a69 6465 6e74 6966 795f  r......identify_
-00000a40: 6461 7465 5f74 696d 655f 636f 6c75 6d6e  date_time_column
-00000a50: 7343 0000 0073 2c00 0000 0004 0c01 0402  sC...s,.........
-00000a60: 0a01 0a01 0201 1601 0a01 1201 0e01 0801  ................
-00000a70: 0601 0c01 0402 0801 0a01 0201 1601 0a01  ................
-00000a80: 1201 0e01 0801 7a2e 4665 6174 7572 6554  ......z.FeatureT
-00000a90: 7970 6544 6574 6563 746f 722e 6964 656e  ypeDetector.iden
-00000aa0: 7469 6679 5f64 6174 655f 7469 6d65 5f63  tify_date_time_c
-00000ab0: 6f6c 756d 6e73 2903 7218 0000 0072 2a00  olumns).r....r*.
-00000ac0: 0000 7222 0000 0063 0300 0000 0000 0000  ..r"...c........
-00000ad0: 0000 0000 0800 0000 0900 0000 4300 0000  ............C...
-00000ae0: 73d6 0000 007c 0272 167c 006a 0072 167c  s....|.r.|.j.r.|
-00000af0: 027c 006a 0017 007d 036e 267c 0272 267c  .|.j...}.n&|.r&|
-00000b00: 006a 0073 267c 027d 036e 167c 0273 387c  .j.s&|.}.n.|.s8|
-00000b10: 006a 0072 387c 006a 007d 036e 0467 007d  .j.r8|.j.}.n.g.}
-00000b20: 037c 016a 0164 0164 0185 027c 016a 02a0  .|.j.d.d...|.j..
-00000b30: 037c 03a1 010f 0066 0219 007d 047c 046a  .|.....f...}.|.j
-00000b40: 02a0 04a1 007d 0567 007d 067c 0544 005d  .....}.g.}.|.D.]
-00000b50: 607d 077a 207c 017c 0719 00a0 0574 06a1  `}.z |.|.....t..
-00000b60: 017c 017c 073c 0064 027c 006a 077c 073c  .|.|.<.d.|.j.|.<
-00000b70: 0057 0071 6a04 0074 086b 0a72 c801 0001  .W.qj..t.k.r....
-00000b80: 0001 007c 017c 0719 00a0 0574 09a1 017c  ...|.|.....t...|
-00000b90: 017c 073c 0064 037c 006a 077c 073c 007c  .|.<.d.|.j.|.<.|
-00000ba0: 06a0 0a7c 07a1 0101 0059 0071 6a58 0071  ...|.....Y.qjX.q
-00000bb0: 6a7c 067c 005f 0b7c 0153 0029 047a ae54  j|.|._.|.S.).z.T
-00000bc0: 7265 6174 2072 656d 6169 6e69 6e67 2063  reat remaining c
-00000bd0: 6f6c 756d 6e73 2e0a 0a20 2020 2020 2020  olumns...       
-00000be0: 2054 616b 6573 2072 656d 6169 6e69 6e67   Takes remaining
-00000bf0: 2063 6f6c 756d 6e73 2061 6e64 2074 7269   columns and tri
-00000c00: 6573 2074 6f20 6361 7374 2074 6865 6d20  es to cast them 
-00000c10: 6173 206e 756d 6572 6963 616c 2e20 4966  as numerical. If
-00000c20: 206e 6f74 2073 7563 6365 7373 6675 6c2c   not successful,
-00000c30: 2074 6865 6e20 636f 6c75 6d6e 7320 6172   then columns ar
-00000c40: 6520 6173 7375 6d65 6420 746f 2062 650a  e assumed to be.
-00000c50: 2020 2020 2020 2020 6361 7465 676f 7269          categori
-00000c60: 6361 6c2e 0a20 2020 2020 2020 204e da05  cal..        N..
-00000c70: 666c 6f61 74da 066f 626a 6563 7429 0c72  float..object).r
-00000c80: 0a00 0000 7226 0000 0072 1b00 0000 7227  ....r&...r....r'
-00000c90: 0000 0072 2800 0000 7225 0000 0072 3500  ...r(...r%...r5.
-00000ca0: 0000 7212 0000 0072 2900 0000 7233 0000  ..r....r)...r3..
-00000cb0: 0072 1c00 0000 7209 0000 0029 0872 1400  .r....r....).r..
-00000cc0: 0000 7218 0000 0072 2a00 0000 da0f 6e6f  ..r....r*.....no
-00000cd0: 5f62 6f6f 6c5f 6474 5f63 6f6c 73da 136e  _bool_dt_cols..n
-00000ce0: 6f5f 626f 6f6c 5f64 6174 6574 696d 655f  o_bool_datetime_
-00000cf0: 6466 da15 6e6f 5f62 6f6f 6c5f 6461 7465  df..no_bool_date
-00000d00: 7469 6d65 5f63 6f6c 7372 0900 0000 7220  time_colsr....r 
-00000d10: 0000 0072 1500 0000 7215 0000 0072 1600  ...r....r....r..
-00000d20: 0000 da1b 6361 7374 5f72 6573 745f 636f  ....cast_rest_co
-00000d30: 6c75 6d6e 735f 746f 5f6f 626a 6563 7460  lumns_to_object`
-00000d40: 0000 0073 2800 0000 0008 0a01 0c01 0a01  ...s(...........
-00000d50: 0601 0a01 0802 0401 1c01 0a01 0401 0801  ................
-00000d60: 0201 1201 0e01 0e01 1201 0a01 1201 0601  ................
-00000d70: 7a2f 4665 6174 7572 6554 7970 6544 6574  z/FeatureTypeDet
-00000d80: 6563 746f 722e 6361 7374 5f72 6573 745f  ector.cast_rest_
-00000d90: 636f 6c75 6d6e 735f 746f 5f6f 626a 6563  columns_to_objec
-00000da0: 7463 0200 0000 0000 0000 0000 0000 0400  tc..............
-00000db0: 0000 0400 0000 4300 0000 7334 0000 007c  ......C...s4...|
-00000dc0: 00a0 007c 01a1 0101 007c 00a0 017c 01a1  ...|.....|...|..
-00000dd0: 015c 027d 027d 037c 00a0 027c 017c 03a1  .\.}.}.|...|.|..
-00000de0: 0201 007c 00a0 037c 017c 02a1 027d 017c  ...|...|.|...}.|
-00000df0: 0153 0029 017a 7249 6465 6e74 6966 7920  .S.).zrIdentify 
-00000e00: 616e 6420 7472 616e 7366 6f72 6d20 6665  and transform fe
-00000e10: 6174 7572 6520 7479 7065 732e 0a0a 2020  ature types...  
-00000e20: 2020 2020 2020 5772 6170 7065 7220 6675        Wrapper fu
-00000e30: 6e63 7469 6f6e 2074 6f20 6f72 6368 6573  nction to orches
-00000e40: 7465 7220 6469 6666 6572 656e 7420 6465  ter different de
-00000e50: 7465 6374 696f 6e20 6d65 7468 6f64 732e  tection methods.
-00000e60: 0a20 2020 2020 2020 2029 0472 2100 0000  .        ).r!...
-00000e70: 722d 0000 0072 3400 0000 723a 0000 0029  r-...r4...r:...)
-00000e80: 0472 1400 0000 7218 0000 0072 2a00 0000  .r....r....r*...
-00000e90: 722c 0000 0072 1500 0000 7215 0000 0072  r,...r....r....r
-00000ea0: 1600 0000 da1b 6669 745f 7472 616e 7366  ......fit_transf
-00000eb0: 6f72 6d5f 6665 6174 7572 655f 7479 7065  orm_feature_type
-00000ec0: 737e 0000 0073 0a00 0000 0005 0a01 0e01  s~...s..........
-00000ed0: 0c01 0c01 7a2f 4665 6174 7572 6554 7970  ....z/FeatureTyp
-00000ee0: 6544 6574 6563 746f 722e 6669 745f 7472  eDetector.fit_tr
-00000ef0: 616e 7366 6f72 6d5f 6665 6174 7572 655f  ansform_feature_
-00000f00: 7479 7065 7329 0372 1800 0000 da0b 6967  types).r......ig
-00000f10: 6e6f 7265 5f63 6f6c 7372 2200 0000 6303  nore_colsr"...c.
-00000f20: 0000 0000 0000 0000 0000 0004 0000 0005  ................
-00000f30: 0000 0043 0000 0073 6400 0000 7c00 6a00  ...C...sd...|.j.
-00000f40: 4400 5d58 7d03 7c02 7206 7c03 7c02 6b07  D.]X}.|.r.|.|.k.
-00000f50: 7206 7c03 7c01 6a01 6b06 7206 7c00 6a00  r.|.|.j.k.r.|.j.
-00000f60: 7c03 1900 6401 6b02 7246 7402 6a03 7c01  |...d.k.rFt.j.|.
-00000f70: 7c03 1900 6402 6403 8d02 7c01 7c03 3c00  |...d.d...|.|.<.
-00000f80: 7106 7c01 7c03 1900 a004 7c00 6a00 7c03  q.|.|.....|.j.|.
-00000f90: 1900 a101 7c01 7c03 3c00 7106 7c01 5300  ....|.|.<.q.|.S.
-00000fa0: 2904 7a36 5472 616e 7366 6f72 6d20 6665  ).z6Transform fe
-00000fb0: 6174 7572 6520 7479 7065 7320 6261 7365  ature types base
-00000fc0: 6420 6f6e 2061 6c72 6561 6479 206d 6170  d on already map
-00000fd0: 7065 6420 7479 7065 732e 7230 0000 0054  ped types.r0...T
-00000fe0: 722e 0000 0029 0572 1200 0000 721b 0000  r....).r....r...
-00000ff0: 0072 3100 0000 7232 0000 0072 2500 0000  .r1...r2...r%...
-00001000: 2904 7214 0000 0072 1800 0000 723c 0000  ).r....r....r<..
-00001010: 00da 036b 6579 7215 0000 0072 1500 0000  ...keyr....r....
-00001020: 7216 0000 00da 1774 7261 6e73 666f 726d  r......transform
-00001030: 5f66 6561 7475 7265 5f74 7970 6573 8900  _feature_types..
-00001040: 0000 730c 0000 0000 080a 0116 010e 0118  ..s.............
-00001050: 021a 017a 2b46 6561 7475 7265 5479 7065  ...z+FeatureType
-00001060: 4465 7465 6374 6f72 2e74 7261 6e73 666f  Detector.transfo
-00001070: 726d 5f66 6561 7475 7265 5f74 7970 6573  rm_feature_types
-00001080: 2903 4e4e 4e29 014e 2914 da08 5f5f 6e61  ).NNN).N)...__na
-00001090: 6d65 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f  me__..__module__
-000010a0: da0c 5f5f 7175 616c 6e61 6d65 5f5f da07  ..__qualname__..
-000010b0: 5f5f 646f 635f 5f72 0400 0000 7203 0000  __doc__r....r...
-000010c0: 0072 0600 0000 7233 0000 00da 0369 6e74  .r....r3.....int
-000010d0: 7235 0000 0072 1700 0000 7231 0000 00da  r5...r....r1....
-000010e0: 0944 6174 6146 7261 6d65 7221 0000 0072  .DataFramer!...r
-000010f0: 0500 0000 722d 0000 0072 3400 0000 723a  ....r-...r4...r:
-00001100: 0000 0072 3b00 0000 723e 0000 0072 1500  ...r;...r>...r..
-00001110: 0000 7215 0000 0072 1500 0000 7216 0000  ..r....r....r...
-00001120: 0072 0700 0000 0c00 0000 7336 0000 0008  .r........s6....
-00001130: 0104 0700 0100 0100 fc02 0214 0114 0114  ................
-00001140: fc0c 1410 0d04 0126 fe0c 1204 0010 ff0c  .......&........
-00001150: 1e04 0010 0104 fe0c 1e14 0c00 ff02 0104  ................
-00001160: 0012 0104 fe72 0700 0000 290a 7242 0000  .....r....).rB..
-00001170: 00da 0674 7970 696e 6772 0200 0000 7203  ...typingr....r.
-00001180: 0000 0072 0400 0000 7205 0000 0072 0600  ...r....r....r..
-00001190: 0000 da06 7061 6e64 6173 7231 0000 0072  ....pandasr1...r
-000011a0: 0700 0000 7215 0000 0072 1500 0000 7215  ....r....r....r.
-000011b0: 0000 0072 1600 0000 da08 3c6d 6f64 756c  ...r......<modul
-000011c0: 653e 0100 0000 7306 0000 0004 061c 0208  e>....s.........
+00000040: 6d04 5a04 6d05 5a05 0100 6401 6403 6c06  m.Z.m.Z...d.d.l.
+00000050: 5a07 4700 6404 6405 8400 6405 8302 5a08  Z.G.d.d...d...Z.
+00000060: 6403 5300 2906 7ae3 0a46 6561 7475 7265  d.S.).z..Feature
+00000070: 2074 7970 6520 6465 7465 6374 696f 6e20   type detection 
+00000080: 616e 6420 6361 7374 696e 672e 0a0a 5468  and casting...Th
+00000090: 6973 2069 7320 6120 636f 6e76 656e 6965  is is a convenie
+000000a0: 6e63 6520 636c 6173 7320 746f 2064 6574  nce class to det
+000000b0: 6563 7420 616e 6420 6361 7374 2066 6561  ect and cast fea
+000000c0: 7475 7265 2074 7970 6573 2069 6e20 6120  ture types in a 
+000000d0: 4461 7461 4672 616d 652e 2049 7420 6361  DataFrame. It ca
+000000e0: 6e20 6265 2075 7365 6420 746f 2064 6574  n be used to det
+000000f0: 6563 7420 6e75 6d65 7269 6361 6c2c 0a63  ect numerical,.c
+00000100: 6174 6567 6f72 6963 616c 2061 6e64 2064  ategorical and d
+00000110: 6174 6574 696d 6520 636f 6c75 6d6e 732e  atetime columns.
+00000120: 2049 7420 616c 736f 2063 6173 7473 2063   It also casts c
+00000130: 6f6c 756d 6e73 2074 6f20 6120 7370 6563  olumns to a spec
+00000140: 6966 6963 2074 7970 652e 0ae9 0000 0000  ific type.......
+00000150: 2904 da04 4469 6374 da04 4c69 7374 da05  )...Dict..List..
+00000160: 5475 706c 65da 0555 6e69 6f6e 4e63 0000  Tuple..UnionNc..
+00000170: 0000 0000 0000 0000 0000 0000 0000 0800  ................
+00000180: 0000 4000 0000 7314 0100 0065 005a 0164  ..@...s....e.Z.d
+00000190: 005a 0264 015a 0364 1765 0465 0565 0665  .Z.d.Z.d.e.e.e.e
+000001a0: 0765 0866 0319 0019 0065 0465 0565 0665  .e.f.....e.e.e.e
+000001b0: 0765 0866 0319 0019 0065 0465 0565 0665  .e.f.....e.e.e.e
+000001c0: 0765 0866 0319 0019 0064 039c 0364 0464  .e.f.....d...d.d
+000001d0: 0584 055a 0965 0a6a 0b64 069c 0164 0764  ...Z.e.j.d...d.d
+000001e0: 0884 045a 0c65 0a6a 0b65 0d65 0465 0565  ...Z.e.j.e.e.e.e
+000001f0: 0665 0865 0766 0319 0019 0065 0465 0565  .e.e.f.....e.e.e
+00000200: 0665 0865 0766 0319 0019 0066 0219 0064  .e.e.f.....f...d
+00000210: 099c 0264 0a64 0b84 045a 0e65 0a6a 0b65  ...d.d...Z.e.j.e
+00000220: 0465 0565 0665 0865 0766 0319 0019 0064  .e.e.e.e.f.....d
+00000230: 0c9c 0264 0d64 0e84 045a 0f65 0a6a 0b65  ...d.d...Z.e.j.e
+00000240: 0465 0565 0665 0865 0766 0319 0019 0065  .e.e.e.e.f.....e
+00000250: 0a6a 0b64 0f9c 0364 1064 1184 045a 1065  .j.d...d.d...Z.e
+00000260: 0a6a 0b65 0a6a 0b64 099c 0264 1264 1384  .j.e.j.d...d.d..
+00000270: 045a 1164 1865 0a6a 0b65 0465 0565 0665  .Z.d.e.j.e.e.e.e
+00000280: 0865 0764 0266 0419 0019 0065 0a6a 0b64  .e.d.f.....e.j.d
+00000290: 149c 0364 1564 1684 055a 1264 0253 0029  ...d.d...Z.d.S.)
+000002a0: 19da 1346 6561 7475 7265 5479 7065 4465  ...FeatureTypeDe
+000002b0: 7465 6374 6f72 7aa9 4465 7465 6374 2061  tectorz.Detect a
+000002c0: 6e64 2063 6173 7420 6665 6174 7572 6520  nd cast feature 
+000002d0: 7479 7065 7320 696e 2044 6174 6146 7261  types in DataFra
+000002e0: 6d65 2e0a 0a20 2020 2043 6f6c 756d 6e20  me...    Column 
+000002f0: 6e61 6d65 7320 666f 7220 696e 6469 7669  names for indivi
+00000300: 6475 616c 2066 6561 7475 7265 2074 7970  dual feature typ
+00000310: 6573 2063 616e 2062 6520 7072 6f76 6964  es can be provid
+00000320: 6564 2e20 4f74 6865 7277 6973 6520 7479  ed. Otherwise ty
+00000330: 7065 7320 7769 6c6c 2062 6520 696e 6665  pes will be infe
+00000340: 7272 6564 2061 6e64 2063 6173 7465 6420  rred and casted 
+00000350: 6163 636f 7264 696e 676c 792e 0a20 2020  accordingly..   
+00000360: 204e 2903 da0b 6e75 6d5f 636f 6c75 6d6e   N)...num_column
+00000370: 73da 0b63 6174 5f63 6f6c 756d 6e73 da0c  s..cat_columns..
+00000380: 6461 7465 5f63 6f6c 756d 6e73 6304 0000  date_columnsc...
+00000390: 0000 0000 0000 0000 0004 0000 0007 0000  ................
+000003a0: 0043 0000 0073 4800 0000 7c01 7308 6700  .C...sH...|.s.g.
+000003b0: 7d01 7c01 7c00 5f00 7c02 7316 6700 7d02  }.|.|._.|.s.g.}.
+000003c0: 7c02 7c00 5f01 7c03 7324 6700 7d03 7c03  |.|._.|.s$g.}.|.
+000003d0: 7c00 5f02 6900 7c00 5f03 6401 6402 6403  |._.i.|._.d.d.d.
+000003e0: 6404 6405 6406 6407 6707 7c00 5f04 6400  d.d.d.d.g.|._.d.
+000003f0: 5300 2908 4eda 0469 6e74 38da 0569 6e74  S.).N..int8..int
+00000400: 3136 da05 696e 7433 32da 0569 6e74 3634  16..int32..int64
+00000410: da07 666c 6f61 7431 36da 0766 6c6f 6174  ..float16..float
+00000420: 3332 da07 666c 6f61 7436 3429 0572 0700  32..float64).r..
+00000430: 0000 7208 0000 0072 0900 0000 da12 6465  ..r....r......de
+00000440: 7465 6374 6564 5f63 6f6c 5f74 7970 6573  tected_col_types
+00000450: da0a 6e75 6d5f 6474 7970 6573 2904 da04  ..num_dtypes)...
+00000460: 7365 6c66 7207 0000 0072 0800 0000 7209  selfr....r....r.
+00000470: 0000 00a9 0072 1400 0000 fa4a 2f68 6f6d  .....r.....J/hom
+00000480: 652f 7468 6f6d 6173 2f49 6465 6150 726f  e/thomas/IdeaPro
+00000490: 6a65 6374 732f 426c 7565 4361 7374 2f62  jects/BlueCast/b
+000004a0: 6c75 6563 6173 742f 7072 6570 726f 6365  luecast/preproce
+000004b0: 7373 696e 672f 6665 6174 7572 655f 7479  ssing/feature_ty
+000004c0: 7065 732e 7079 da08 5f5f 696e 6974 5f5f  pes.py..__init__
+000004d0: 1200 0000 7324 0000 0000 0604 0104 0106  ....s$..........
+000004e0: 0204 0104 0106 0204 0104 0106 0206 0202  ................
+000004f0: 0102 0102 0102 0102 0102 0102 f97a 1c46  .............z.F
+00000500: 6561 7475 7265 5479 7065 4465 7465 6374  eatureTypeDetect
+00000510: 6f72 2e5f 5f69 6e69 745f 5f29 01da 0264  or.__init__)...d
+00000520: 6663 0200 0000 0000 0000 0000 0000 0600  fc..............
+00000530: 0000 0500 0000 4300 0000 7346 0000 007c  ......C...sF...|
+00000540: 006a 0073 4067 007d 027c 006a 0144 005d  .j.s@g.}.|.j.D.]
+00000550: 287d 037c 016a 027c 0367 0164 018d 016a  (}.|.j.|.g.d...j
+00000560: 037d 047c 0444 005d 0e7d 057c 02a0 047c  .}.|.D.].}.|...|
+00000570: 05a1 0101 0071 2871 107c 027c 005f 007c  .....q(q.|.|._.|
+00000580: 006a 0053 0029 027a 3f49 6465 6e74 6966  .j.S.).z?Identif
+00000590: 7920 6e75 6d65 7269 6361 6c20 636f 6c75  y numerical colu
+000005a0: 6d6e 7320 6261 7365 6420 6f6e 2061 6c72  mns based on alr
+000005b0: 6561 6479 2065 7869 7374 696e 6720 6461  eady existing da
+000005c0: 7461 2074 7970 652e 2901 da07 696e 636c  ta type.)...incl
+000005d0: 7564 6529 0572 0700 0000 7212 0000 00da  ude).r....r.....
+000005e0: 0d73 656c 6563 745f 6474 7970 6573 da07  .select_dtypes..
+000005f0: 636f 6c75 6d6e 73da 0661 7070 656e 6429  columns..append)
+00000600: 0672 1300 0000 7217 0000 00da 0c6e 756d  .r....r......num
+00000610: 5f63 6f6c 5f6c 6973 74da 0776 6172 7479  _col_list..varty
+00000620: 7065 da08 6e75 6d5f 636f 6c73 da03 636f  pe..num_cols..co
+00000630: 6c72 1400 0000 7214 0000 0072 1500 0000  lr....r....r....
+00000640: da14 6964 656e 7469 6679 5f6e 756d 5f63  ..identify_num_c
+00000650: 6f6c 756d 6e73 2f00 0000 7310 0000 0000  olumns/...s.....
+00000660: 0306 0104 010a 0110 0108 010e 0106 017a  ...............z
+00000670: 2846 6561 7475 7265 5479 7065 4465 7465  (FeatureTypeDete
+00000680: 6374 6f72 2e69 6465 6e74 6966 795f 6e75  ctor.identify_nu
+00000690: 6d5f 636f 6c75 6d6e 7329 0272 1700 0000  m_columns).r....
+000006a0: da06 7265 7475 726e 6302 0000 0000 0000  ..returnc.......
+000006b0: 0000 0000 0006 0000 0008 0000 0043 0000  .............C..
+000006c0: 0073 8800 0000 7400 7c01 a001 6401 6701  .s....t.|...d.g.
+000006d0: a101 8301 7d02 7c02 4400 5d20 7d03 7c01  ....}.|.D.] }.|.
+000006e0: 7c03 1900 a002 7403 a101 7c01 7c03 3c00  |.....t...|.|.<.
+000006f0: 6401 7c00 6a04 7c03 3c00 7114 7a2a 7c01  d.|.j.|.<.q.z*|.
+00000700: 6a05 6402 6402 8502 7c01 6a06 a007 7c02  j.d.d...|.j...|.
+00000710: a101 0f00 6602 1900 7d04 7c04 6a06 a008  ....f...}.|.j...
+00000720: a100 7d05 5700 6e1e 0400 7409 6b0a 727e  ..}.W.n...t.k.r~
+00000730: 0100 0100 0100 7c01 6a06 a008 a100 7d05  ......|.j.....}.
+00000740: 5900 6e02 5800 7c02 7c05 6602 5300 2903  Y.n.X.|.|.f.S.).
+00000750: 7a2b 4964 656e 7469 6679 2062 6f6f 6c65  z+Identify boole
+00000760: 616e 2063 6f6c 756d 6e73 2062 6173 6564  an columns based
+00000770: 206f 6e20 6461 7461 2074 7970 65da 0462   on data type..b
+00000780: 6f6f 6c4e 290a da04 6c69 7374 7219 0000  oolN)...listr...
+00000790: 00da 0661 7374 7970 6572 2200 0000 7211  ...astyper"...r.
+000007a0: 0000 00da 036c 6f63 721a 0000 00da 0469  .....locr......i
+000007b0: 7369 6eda 0774 6f5f 6c69 7374 da09 4578  sin..to_list..Ex
+000007c0: 6365 7074 696f 6e29 0672 1300 0000 7217  ception).r....r.
+000007d0: 0000 00da 0962 6f6f 6c5f 636f 6c73 721f  .....bool_colsr.
+000007e0: 0000 00da 0a6e 6f5f 626f 6f6c 5f64 66da  .....no_bool_df.
+000007f0: 0c6e 6f5f 626f 6f6c 5f63 6f6c 7372 1400  .no_bool_colsr..
+00000800: 0000 7214 0000 0072 1500 0000 da15 6964  ..r....r......id
+00000810: 656e 7469 6679 5f62 6f6f 6c5f 636f 6c75  entify_bool_colu
+00000820: 6d6e 733b 0000 0073 1400 0000 0004 1001  mns;...s........
+00000830: 0801 1201 0c03 0201 1c01 0e01 0e01 1001  ................
+00000840: 7a29 4665 6174 7572 6554 7970 6544 6574  z)FeatureTypeDet
+00000850: 6563 746f 722e 6964 656e 7469 6679 5f62  ector.identify_b
+00000860: 6f6f 6c5f 636f 6c75 6d6e 7329 0272 1700  ool_columns).r..
+00000870: 0000 722b 0000 0063 0300 0000 0000 0000  ..r+...c........
+00000880: 0000 0000 0500 0000 0900 0000 4300 0000  ............C...
+00000890: 73ea 0000 007c 006a 0072 747c 006a 0172  s....|.j.rt|.j.r
+000008a0: 7467 007d 037c 006a 0044 005d 567d 047c  tg.}.|.j.D.]V}.|
+000008b0: 047c 006a 016b 0772 167a 3274 026a 037c  .|.j.k.r.z2t.j.|
+000008c0: 017c 0419 0064 0164 028d 027c 017c 043c  .|...d.d...|.|.<
+000008d0: 007c 03a0 047c 04a1 0101 0064 037c 006a  .|...|.....d.|.j
+000008e0: 0574 067c 0483 013c 0057 0071 1604 0074  .t.|...<.W.q...t
+000008f0: 076b 0a72 6a01 0001 0001 0059 0071 1658  .k.rj......Y.q.X
+00000900: 0071 167c 037c 005f 007c 006a 0073 e67c  .q.|.|._.|.j.s.|
+00000910: 006a 0172 e667 007d 037c 0244 005d 567d  .j.r.g.}.|.D.]V}
+00000920: 047c 047c 006a 016b 0772 887a 3274 026a  .|.|.j.k.r.z2t.j
+00000930: 037c 017c 0419 0064 0164 028d 027c 017c  .|.|...d.d...|.|
+00000940: 043c 007c 03a0 047c 04a1 0101 0064 037c  .<.|...|.....d.|
+00000950: 006a 0574 067c 0483 013c 0057 0071 8804  .j.t.|...<.W.q..
+00000960: 0074 076b 0a72 dc01 0001 0001 0059 0071  .t.k.r.......Y.q
+00000970: 8858 0071 887c 037c 005f 0064 0453 0029  .X.q.|.|._.d.S.)
+00000980: 057a 4454 7279 2063 6173 7469 6e67 2074  .zDTry casting t
+00000990: 6f20 6461 7465 7469 6d65 2e20 4578 7065  o datetime. Expe
+000009a0: 6374 6564 2069 7320 6120 6461 7465 7469  cted is a dateti
+000009b0: 6d65 2066 6f72 6d61 7420 6f66 2059 5959  me format of YYY
+000009c0: 592d 4d4d 2d44 4454 a901 da09 7965 6172  Y-MM-DDT....year
+000009d0: 6669 7273 74fa 0c64 6174 6574 696d 655b  first..datetime[
+000009e0: 6e73 5d4e 2908 7209 0000 0072 0700 0000  ns]N).r....r....
+000009f0: da02 7064 da0b 746f 5f64 6174 6574 696d  ..pd..to_datetim
+00000a00: 6572 1b00 0000 7211 0000 00da 0373 7472  er....r......str
+00000a10: 7228 0000 0029 0572 1300 0000 7217 0000  r(...).r....r...
+00000a20: 0072 2b00 0000 7209 0000 0072 1f00 0000  .r+...r....r....
+00000a30: 7214 0000 0072 1400 0000 7215 0000 00da  r....r....r.....
+00000a40: 1a69 6465 6e74 6966 795f 6461 7465 5f74  .identify_date_t
+00000a50: 696d 655f 636f 6c75 6d6e 734c 0000 0073  ime_columnsL...s
+00000a60: 2c00 0000 0004 0c01 0402 0a01 0a01 0201  ,...............
+00000a70: 1601 0a01 1201 0e01 0801 0601 0c01 0402  ................
+00000a80: 0801 0a01 0201 1601 0a01 1201 0e01 0801  ................
+00000a90: 7a2e 4665 6174 7572 6554 7970 6544 6574  z.FeatureTypeDet
+00000aa0: 6563 746f 722e 6964 656e 7469 6679 5f64  ector.identify_d
+00000ab0: 6174 655f 7469 6d65 5f63 6f6c 756d 6e73  ate_time_columns
+00000ac0: 2903 7217 0000 0072 2900 0000 7221 0000  ).r....r)...r!..
+00000ad0: 0063 0300 0000 0000 0000 0000 0000 0800  .c..............
+00000ae0: 0000 0900 0000 4300 0000 73d6 0000 007c  ......C...s....|
+00000af0: 0272 167c 006a 0072 167c 027c 006a 0017  .r.|.j.r.|.|.j..
+00000b00: 007d 036e 267c 0272 267c 006a 0073 267c  .}.n&|.r&|.j.s&|
+00000b10: 027d 036e 167c 0273 387c 006a 0072 387c  .}.n.|.s8|.j.r8|
+00000b20: 006a 007d 036e 0467 007d 037c 016a 0164  .j.}.n.g.}.|.j.d
+00000b30: 0164 0185 027c 016a 02a0 037c 03a1 010f  .d...|.j...|....
+00000b40: 0066 0219 007d 047c 046a 02a0 04a1 007d  .f...}.|.j.....}
+00000b50: 0567 007d 067c 0544 005d 607d 077a 207c  .g.}.|.D.]`}.z |
+00000b60: 017c 0719 00a0 0574 06a1 017c 017c 073c  .|.....t...|.|.<
+00000b70: 0064 027c 006a 077c 073c 0057 0071 6a04  .d.|.j.|.<.W.qj.
+00000b80: 0074 086b 0a72 c801 0001 0001 007c 017c  .t.k.r.......|.|
+00000b90: 0719 00a0 0574 09a1 017c 017c 073c 0064  .....t...|.|.<.d
+00000ba0: 037c 006a 077c 073c 007c 06a0 0a7c 07a1  .|.j.|.<.|...|..
+00000bb0: 0101 0059 0071 6a58 0071 6a7c 067c 005f  ...Y.qjX.qj|.|._
+00000bc0: 0b7c 0153 0029 047a ae54 7265 6174 2072  .|.S.).z.Treat r
+00000bd0: 656d 6169 6e69 6e67 2063 6f6c 756d 6e73  emaining columns
+00000be0: 2e0a 0a20 2020 2020 2020 2054 616b 6573  ...        Takes
+00000bf0: 2072 656d 6169 6e69 6e67 2063 6f6c 756d   remaining colum
+00000c00: 6e73 2061 6e64 2074 7269 6573 2074 6f20  ns and tries to 
+00000c10: 6361 7374 2074 6865 6d20 6173 206e 756d  cast them as num
+00000c20: 6572 6963 616c 2e20 4966 206e 6f74 2073  erical. If not s
+00000c30: 7563 6365 7373 6675 6c2c 2074 6865 6e20  uccessful, then 
+00000c40: 636f 6c75 6d6e 7320 6172 6520 6173 7375  columns are assu
+00000c50: 6d65 6420 746f 2062 650a 2020 2020 2020  med to be.      
+00000c60: 2020 6361 7465 676f 7269 6361 6c2e 0a20    categorical.. 
+00000c70: 2020 2020 2020 204e da05 666c 6f61 74da         N..float.
+00000c80: 066f 626a 6563 7429 0c72 0900 0000 7225  .object).r....r%
+00000c90: 0000 0072 1a00 0000 7226 0000 0072 2700  ...r....r&...r'.
+00000ca0: 0000 7224 0000 0072 3400 0000 7211 0000  ..r$...r4...r...
+00000cb0: 0072 2800 0000 7232 0000 0072 1b00 0000  .r(...r2...r....
+00000cc0: 7208 0000 0029 0872 1300 0000 7217 0000  r....).r....r...
+00000cd0: 0072 2900 0000 da0f 6e6f 5f62 6f6f 6c5f  .r).....no_bool_
+00000ce0: 6474 5f63 6f6c 73da 136e 6f5f 626f 6f6c  dt_cols..no_bool
+00000cf0: 5f64 6174 6574 696d 655f 6466 da15 6e6f  _datetime_df..no
+00000d00: 5f62 6f6f 6c5f 6461 7465 7469 6d65 5f63  _bool_datetime_c
+00000d10: 6f6c 7372 0800 0000 721f 0000 0072 1400  olsr....r....r..
+00000d20: 0000 7214 0000 0072 1500 0000 da1b 6361  ..r....r......ca
+00000d30: 7374 5f72 6573 745f 636f 6c75 6d6e 735f  st_rest_columns_
+00000d40: 746f 5f6f 626a 6563 7469 0000 0073 2800  to_objecti...s(.
+00000d50: 0000 0008 0a01 0c01 0a01 0601 0a01 0802  ................
+00000d60: 0401 1c01 0a01 0401 0801 0201 1201 0e01  ................
+00000d70: 0e01 1201 0a01 1201 0601 7a2f 4665 6174  ..........z/Feat
+00000d80: 7572 6554 7970 6544 6574 6563 746f 722e  ureTypeDetector.
+00000d90: 6361 7374 5f72 6573 745f 636f 6c75 6d6e  cast_rest_column
+00000da0: 735f 746f 5f6f 626a 6563 7463 0200 0000  s_to_objectc....
+00000db0: 0000 0000 0000 0000 0400 0000 0400 0000  ................
+00000dc0: 4300 0000 7334 0000 007c 00a0 007c 01a1  C...s4...|...|..
+00000dd0: 0101 007c 00a0 017c 01a1 015c 027d 027d  ...|...|...\.}.}
+00000de0: 037c 00a0 027c 017c 03a1 0201 007c 00a0  .|...|.|.....|..
+00000df0: 037c 017c 02a1 027d 017c 0153 0029 017a  .|.|...}.|.S.).z
+00000e00: 7249 6465 6e74 6966 7920 616e 6420 7472  rIdentify and tr
+00000e10: 616e 7366 6f72 6d20 6665 6174 7572 6520  ansform feature 
+00000e20: 7479 7065 732e 0a0a 2020 2020 2020 2020  types...        
+00000e30: 5772 6170 7065 7220 6675 6e63 7469 6f6e  Wrapper function
+00000e40: 2074 6f20 6f72 6368 6573 7465 7220 6469   to orchester di
+00000e50: 6666 6572 656e 7420 6465 7465 6374 696f  fferent detectio
+00000e60: 6e20 6d65 7468 6f64 732e 0a20 2020 2020  n methods..     
+00000e70: 2020 2029 0472 2000 0000 722c 0000 0072     ).r ...r,...r
+00000e80: 3300 0000 7239 0000 0029 0472 1300 0000  3...r9...).r....
+00000e90: 7217 0000 0072 2900 0000 722b 0000 0072  r....r)...r+...r
+00000ea0: 1400 0000 7214 0000 0072 1500 0000 da1b  ....r....r......
+00000eb0: 6669 745f 7472 616e 7366 6f72 6d5f 6665  fit_transform_fe
+00000ec0: 6174 7572 655f 7479 7065 7387 0000 0073  ature_types....s
+00000ed0: 0a00 0000 0005 0a01 0e01 0c01 0c01 7a2f  ..............z/
+00000ee0: 4665 6174 7572 6554 7970 6544 6574 6563  FeatureTypeDetec
+00000ef0: 746f 722e 6669 745f 7472 616e 7366 6f72  tor.fit_transfor
+00000f00: 6d5f 6665 6174 7572 655f 7479 7065 7329  m_feature_types)
+00000f10: 0372 1700 0000 da0b 6967 6e6f 7265 5f63  .r......ignore_c
+00000f20: 6f6c 7372 2100 0000 6303 0000 0000 0000  olsr!...c.......
+00000f30: 0000 0000 0004 0000 0005 0000 0043 0000  .............C..
+00000f40: 0073 6400 0000 7c00 6a00 4400 5d58 7d03  .sd...|.j.D.]X}.
+00000f50: 7c02 7206 7c03 7c02 6b07 7206 7c03 7c01  |.r.|.|.k.r.|.|.
+00000f60: 6a01 6b06 7206 7c00 6a00 7c03 1900 6401  j.k.r.|.j.|...d.
+00000f70: 6b02 7246 7402 6a03 7c01 7c03 1900 6402  k.rFt.j.|.|...d.
+00000f80: 6403 8d02 7c01 7c03 3c00 7106 7c01 7c03  d...|.|.<.q.|.|.
+00000f90: 1900 a004 7c00 6a00 7c03 1900 a101 7c01  ....|.j.|.....|.
+00000fa0: 7c03 3c00 7106 7c01 5300 2904 7a36 5472  |.<.q.|.S.).z6Tr
+00000fb0: 616e 7366 6f72 6d20 6665 6174 7572 6520  ansform feature 
+00000fc0: 7479 7065 7320 6261 7365 6420 6f6e 2061  types based on a
+00000fd0: 6c72 6561 6479 206d 6170 7065 6420 7479  lready mapped ty
+00000fe0: 7065 732e 722f 0000 0054 722d 0000 0029  pes.r/...Tr-...)
+00000ff0: 0572 1100 0000 721a 0000 0072 3000 0000  .r....r....r0...
+00001000: 7231 0000 0072 2400 0000 2904 7213 0000  r1...r$...).r...
+00001010: 0072 1700 0000 723b 0000 00da 036b 6579  .r....r;.....key
+00001020: 7214 0000 0072 1400 0000 7215 0000 00da  r....r....r.....
+00001030: 1774 7261 6e73 666f 726d 5f66 6561 7475  .transform_featu
+00001040: 7265 5f74 7970 6573 9200 0000 730c 0000  re_types....s...
+00001050: 0000 080a 0116 010e 0118 021a 017a 2b46  .............z+F
+00001060: 6561 7475 7265 5479 7065 4465 7465 6374  eatureTypeDetect
+00001070: 6f72 2e74 7261 6e73 666f 726d 5f66 6561  or.transform_fea
+00001080: 7475 7265 5f74 7970 6573 2903 4e4e 4e29  ture_types).NNN)
+00001090: 014e 2913 da08 5f5f 6e61 6d65 5f5f da0a  .N)...__name__..
+000010a0: 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f 7175  __module__..__qu
+000010b0: 616c 6e61 6d65 5f5f da07 5f5f 646f 635f  alname__..__doc_
+000010c0: 5f72 0300 0000 7205 0000 0072 3200 0000  _r....r....r2...
+000010d0: da03 696e 7472 3400 0000 7216 0000 0072  ..intr4...r....r
+000010e0: 3000 0000 da09 4461 7461 4672 616d 6572  0.....DataFramer
+000010f0: 2000 0000 7204 0000 0072 2c00 0000 7233   ...r....r,...r3
+00001100: 0000 0072 3900 0000 723a 0000 0072 3d00  ...r9...r:...r=.
+00001110: 0000 7214 0000 0072 1400 0000 7214 0000  ..r....r....r...
+00001120: 0072 1500 0000 7206 0000 000c 0000 0073  .r....r........s
+00001130: 3600 0000 0801 0407 0001 0001 00fc 0202  6...............
+00001140: 1001 1001 10fc 0c1d 100d 0401 26fe 0c12  ............&...
+00001150: 0400 10ff 0c1e 0400 1001 04fe 0c1e 140c  ................
+00001160: 00ff 0201 0400 1201 04fe 7206 0000 0029  ..........r....)
+00001170: 0972 4100 0000 da06 7479 7069 6e67 7202  .rA.....typingr.
+00001180: 0000 0072 0300 0000 7204 0000 0072 0500  ...r....r....r..
+00001190: 0000 da06 7061 6e64 6173 7230 0000 0072  ....pandasr0...r
+000011a0: 0600 0000 7214 0000 0072 1400 0000 7214  ....r....r....r.
+000011b0: 0000 0072 1500 0000 da08 3c6d 6f64 756c  ...r......<modul
+000011c0: 653e 0100 0000 7306 0000 0004 0618 0208  e>....s.........
 000011d0: 03                                       .
```

### Comparing `bluecast-0.5/bluecast/preprocessing/__pycache__/nulls_and_infs.cpython-310.pyc` & `bluecast-0.7/bluecast/preprocessing/__pycache__/nulls_and_infs.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.5/bluecast/preprocessing/__pycache__/nulls_and_infs.cpython-38.pyc` & `bluecast-0.7/bluecast/preprocessing/__pycache__/nulls_and_infs.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.5/bluecast/preprocessing/__pycache__/schema_checks.cpython-310.pyc` & `bluecast-0.7/bluecast/preprocessing/__pycache__/schema_checks.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.5/bluecast/preprocessing/__pycache__/schema_checks.cpython-38.pyc` & `bluecast-0.7/bluecast/preprocessing/__pycache__/schema_checks.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Thu Jun  8 04:52:47 2023 UTC, .py size: 1351 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 8% similar despite different names*

```diff
@@ -1,121 +1,124 @@
-00000000: 550d 0d0a 0000 0000 9f5e 8164 4705 0000  U........^.dG...
+00000000: 550d 0d0a 0000 0000 ca79 8164 ac05 0000  U........y.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0003 0000 0040 0000 0073 2a00 0000 6400  .....@...s*...d.
-00000030: 6401 6c00 5a01 6400 6402 6c02 6d03 5a03  d.l.Z.d.d.l.m.Z.
-00000040: 6d04 5a04 0100 4700 6403 6404 8400 6404  m.Z...G.d.d...d.
-00000050: 8302 5a05 6401 5300 2905 e900 0000 004e  ..Z.d.S.)......N
-00000060: 2902 da04 4c69 7374 da05 556e 696f 6e63  )...List..Unionc
-00000070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000080: 0300 0000 4000 0000 7338 0000 0065 005a  ....@...s8...e.Z
-00000090: 0164 005a 0264 015a 0364 0264 0384 005a  .d.Z.d.Z.d.d...Z
-000000a0: 0465 056a 0664 049c 0164 0564 0684 045a  .e.j.d...d.d...Z
-000000b0: 0765 056a 0664 049c 0164 0764 0884 045a  .e.j.d...d.d...Z
-000000c0: 0864 0953 0029 0ada 0e53 6368 656d 6144  .d.S.)...SchemaD
-000000d0: 6574 6563 746f 727a 2244 6574 6563 7420  etectorz"Detect 
-000000e0: 616e 6420 6368 6563 6b20 4461 7461 4672  and check DataFr
-000000f0: 616d 6520 7363 6865 6d61 2e63 0100 0000  ame schema.c....
-00000100: 0000 0000 0000 0000 0100 0000 0200 0000  ................
-00000110: 4300 0000 730a 0000 0067 007c 005f 0064  C...s....g.|._.d
-00000120: 0053 0029 014e a901 da0c 7472 6169 6e5f  .S.).N....train_
-00000130: 7363 6865 6d61 a901 da04 7365 6c66 a900  schema....self..
-00000140: 7209 0000 00fa 4a2f 686f 6d65 2f74 686f  r.....J/home/tho
-00000150: 6d61 732f 4964 6561 5072 6f6a 6563 7473  mas/IdeaProjects
-00000160: 2f42 6c75 6543 6173 742f 626c 7565 6361  /BlueCast/blueca
-00000170: 7374 2f70 7265 7072 6f63 6573 7369 6e67  st/preprocessing
-00000180: 2f73 6368 656d 615f 6368 6563 6b73 2e70  /schema_checks.p
-00000190: 79da 085f 5f69 6e69 745f 5f07 0000 0073  y..__init__....s
-000001a0: 0200 0000 0001 7a17 5363 6865 6d61 4465  ......z.SchemaDe
-000001b0: 7465 6374 6f72 2e5f 5f69 6e69 745f 5fa9  tector.__init__.
-000001c0: 01da 0264 6663 0200 0000 0000 0000 0000  ...dfc..........
-000001d0: 0000 0200 0000 0200 0000 4300 0000 7312  ..........C...s.
-000001e0: 0000 007c 016a 00a0 01a1 007c 005f 027c  ...|.j.....|._.|
-000001f0: 006a 0253 0029 017a 2653 746f 7265 2074  .j.S.).z&Store t
-00000200: 6865 2073 6368 656d 6120 6f66 2074 6865  he schema of the
-00000210: 2074 7261 696e 2064 6174 6173 6574 2e29   train dataset.)
-00000220: 03da 0763 6f6c 756d 6e73 da07 746f 5f6c  ...columns..to_l
-00000230: 6973 7472 0600 0000 2902 7208 0000 0072  istr....).r....r
-00000240: 0d00 0000 7209 0000 0072 0900 0000 720a  ....r....r....r.
-00000250: 0000 00da 0366 6974 0a00 0000 7304 0000  .....fit....s...
-00000260: 0000 020c 017a 1253 6368 656d 6144 6574  .....z.SchemaDet
-00000270: 6563 746f 722e 6669 7463 0200 0000 0000  ector.fitc......
-00000280: 0000 0000 0000 0400 0000 0400 0000 0300  ................
-00000290: 0000 737c 0000 0074 0088 006a 0183 0174  ..s|...t...j...t
-000002a0: 0088 016a 0283 016b 0472 3a87 0166 0164  ...j...k.r:..f.d
-000002b0: 0164 0284 0888 006a 0144 0083 017d 0274  .d.....j.D...}.t
-000002c0: 0364 037c 029b 0064 049d 0383 0182 016e  .d.|...d.......n
-000002d0: 3874 0088 006a 0183 0174 0088 016a 0283  8t...j...t...j..
-000002e0: 016b 0072 7287 0066 0164 0564 0284 0888  .k.rr..f.d.d....
-000002f0: 016a 0244 0083 017d 0374 0364 067c 039b  .j.D...}.t.d.|..
-00000300: 0064 049d 0383 0182 0188 0088 016a 0219  .d...........j..
-00000310: 0053 0029 077a cb43 6865 636b 2069 6620  .S.).z.Check if 
-00000320: 7468 6520 7465 7374 2064 6174 6173 6574  the test dataset
-00000330: 2068 6173 2074 6865 2073 616d 6520 7363   has the same sc
-00000340: 6865 6d61 2061 7320 7468 6520 7472 6169  hema as the trai
-00000350: 6e20 6461 7461 7365 742e 200a 0a20 2020  n dataset. ..   
-00000360: 2020 2020 2057 696c 6c20 7261 6973 6520       Will raise 
-00000370: 616e 2065 7272 6f72 2069 6620 7363 6865  an error if sche
-00000380: 6d61 206c 656e 6774 6820 646f 6573 206e  ma length does n
-00000390: 6f74 206d 6174 6368 2061 6e64 2077 696c  ot match and wil
-000003a0: 6c20 7261 6973 6520 6120 7761 726e 696e  l raise a warnin
-000003b0: 6720 696e 6469 6361 7469 6e67 2074 6865  g indicating the
-000003c0: 206d 6973 7369 6e67 206f 7220 6578 7472   missing or extr
-000003d0: 610a 2020 2020 2020 2020 636f 6c75 6d6e  a.        column
-000003e0: 732e 6301 0000 0000 0000 0000 0000 0002  s.c.............
-000003f0: 0000 0004 0000 0013 0000 0073 1a00 0000  ...........s....
-00000400: 6700 7c00 5d12 7d01 7c01 8800 6a00 6b07  g.|.].}.|...j.k.
-00000410: 7204 7c01 9102 7104 5300 7209 0000 0072  r.|...q.S.r....r
-00000420: 0500 0000 a902 da02 2e30 da03 636f 6c72  .........0..colr
-00000430: 0700 0000 7209 0000 0072 0a00 0000 da0a  ....r....r......
-00000440: 3c6c 6973 7463 6f6d 703e 1500 0000 7306  <listcomp>....s.
-00000450: 0000 0006 0002 000a 007a 2c53 6368 656d  .........z,Schem
-00000460: 6144 6574 6563 746f 722e 7472 616e 7366  aDetector.transf
-00000470: 6f72 6d2e 3c6c 6f63 616c 733e 2e3c 6c69  orm.<locals>.<li
-00000480: 7374 636f 6d70 3e7a 9454 6865 206e 756d  stcomp>z.The num
-00000490: 6265 7220 6f66 2063 6f6c 756d 6e73 2069  ber of columns i
-000004a0: 6e20 7468 6520 7465 7374 2064 6174 6173  n the test datas
-000004b0: 6574 2069 7320 6772 6561 7465 7220 7468  et is greater th
-000004c0: 616e 2074 6865 206e 756d 6265 7220 6f66  an the number of
-000004d0: 2063 6f6c 756d 6e73 200a 2020 2020 2020   columns .      
-000004e0: 2020 2020 2020 696e 2074 6865 2074 7261        in the tra
-000004f0: 696e 2064 6174 6173 6574 2e20 466f 756e  in dataset. Foun
-00000500: 6420 7468 6520 666f 6c6c 6f77 696e 6720  d the following 
-00000510: 6e65 7720 636f 6c75 6d6e 733a 20da 012e  new columns: ...
-00000520: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
-00000530: 0004 0000 0013 0000 0073 1a00 0000 6700  .........s....g.
-00000540: 7c00 5d12 7d01 7c01 8800 6a00 6b07 7204  |.].}.|...j.k.r.
-00000550: 7c01 9102 7104 5300 7209 0000 0029 0172  |...q.S.r....).r
-00000560: 0e00 0000 7211 0000 0072 0c00 0000 7209  ....r....r....r.
-00000570: 0000 0072 0a00 0000 7214 0000 0019 0000  ...r....r.......
-00000580: 0073 0600 0000 0600 0200 0a00 7a92 5468  .s..........z.Th
-00000590: 6520 6e75 6d62 6572 206f 6620 636f 6c75  e number of colu
-000005a0: 6d6e 7320 696e 2074 6865 2074 6573 7420  mns in the test 
-000005b0: 6461 7461 7365 7420 6973 2073 6d61 6c6c  dataset is small
-000005c0: 6572 2074 6861 6e20 7468 6520 6e75 6d62  er than the numb
-000005d0: 6572 206f 6620 636f 6c75 6d6e 7320 0a20  er of columns . 
-000005e0: 2020 2020 2020 2020 2020 2069 6e20 7468             in th
-000005f0: 6520 7472 6169 6e20 6461 7461 7365 742e  e train dataset.
-00000600: 204d 6973 7369 6e67 2074 6865 2066 6f6c   Missing the fol
-00000610: 6c6f 7769 6e67 2063 6f6c 756d 6e73 3a20  lowing columns: 
-00000620: 2904 da03 6c65 6e72 0e00 0000 7206 0000  )...lenr....r...
-00000630: 00da 0a56 616c 7565 4572 726f 7229 0472  ...ValueError).r
-00000640: 0800 0000 720d 0000 00da 086e 6577 5f63  ....r......new_c
-00000650: 6f6c 73da 0c6d 6973 7369 6e67 5f63 6f6c  ols..missing_col
-00000660: 7372 0900 0000 2902 720d 0000 0072 0800  sr....).r....r..
-00000670: 0000 720a 0000 00da 0974 7261 6e73 666f  ..r......transfo
-00000680: 726d 0f00 0000 7316 0000 0000 0514 0114  rm....s.........
-00000690: 0104 0102 ff0c 0214 0114 0104 0102 ff0a  ................
-000006a0: 027a 1853 6368 656d 6144 6574 6563 746f  .z.SchemaDetecto
-000006b0: 722e 7472 616e 7366 6f72 6d4e 2909 da08  r.transformN)...
-000006c0: 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f 6475  __name__..__modu
-000006d0: 6c65 5f5f da0c 5f5f 7175 616c 6e61 6d65  le__..__qualname
-000006e0: 5f5f da07 5f5f 646f 635f 5f72 0b00 0000  __..__doc__r....
-000006f0: da02 7064 da09 4461 7461 4672 616d 6572  ..pd..DataFramer
-00000700: 1000 0000 721a 0000 0072 0900 0000 7209  ....r....r....r.
-00000710: 0000 0072 0900 0000 720a 0000 0072 0400  ...r....r....r..
-00000720: 0000 0500 0000 7308 0000 0008 0104 0108  ......s.........
-00000730: 0310 0572 0400 0000 2906 da06 7061 6e64  ...r....)...pand
-00000740: 6173 721f 0000 00da 0674 7970 696e 6772  asr......typingr
-00000750: 0200 0000 7203 0000 0072 0400 0000 7209  ....r....r....r.
-00000760: 0000 0072 0900 0000 7209 0000 0072 0a00  ...r....r....r..
-00000770: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
-00000780: 7304 0000 0008 0110 03                   s........
+00000020: 0003 0000 0040 0000 0073 2e00 0000 6400  .....@...s....d.
+00000030: 5a00 6401 6402 6c01 6d02 5a02 6d03 5a03  Z.d.d.l.m.Z.m.Z.
+00000040: 0100 6401 6403 6c04 5a05 4700 6404 6405  ..d.d.l.Z.G.d.d.
+00000050: 8400 6405 8302 5a06 6403 5300 2906 7a23  ..d...Z.d.S.).z#
+00000060: 4d6f 6475 6c65 2066 6f72 2044 6174 6146  Module for DataF
+00000070: 7261 6d65 2073 6368 656d 6120 6368 6563  rame schema chec
+00000080: 6b73 2ee9 0000 0000 2902 da04 4c69 7374  ks......)...List
+00000090: da05 556e 696f 6e4e 6300 0000 0000 0000  ..UnionNc.......
+000000a0: 0000 0000 0000 0000 0003 0000 0040 0000  .............@..
+000000b0: 0073 3800 0000 6500 5a01 6400 5a02 6401  .s8...e.Z.d.Z.d.
+000000c0: 5a03 6402 6403 8400 5a04 6505 6a06 6404  Z.d.d...Z.e.j.d.
+000000d0: 9c01 6405 6406 8404 5a07 6505 6a06 6404  ..d.d...Z.e.j.d.
+000000e0: 9c01 6407 6408 8404 5a08 6409 5300 290a  ..d.d...Z.d.S.).
+000000f0: da0e 5363 6865 6d61 4465 7465 6374 6f72  ..SchemaDetector
+00000100: 7a22 4465 7465 6374 2061 6e64 2063 6865  z"Detect and che
+00000110: 636b 2044 6174 6146 7261 6d65 2073 6368  ck DataFrame sch
+00000120: 656d 612e 6301 0000 0000 0000 0000 0000  ema.c...........
+00000130: 0001 0000 0002 0000 0043 0000 0073 0a00  .........C...s..
+00000140: 0000 6700 7c00 5f00 6400 5300 2901 4ea9  ..g.|._.d.S.).N.
+00000150: 01da 0c74 7261 696e 5f73 6368 656d 61a9  ...train_schema.
+00000160: 01da 0473 656c 66a9 0072 0900 0000 fa4a  ...self..r.....J
+00000170: 2f68 6f6d 652f 7468 6f6d 6173 2f49 6465  /home/thomas/Ide
+00000180: 6150 726f 6a65 6374 732f 426c 7565 4361  aProjects/BlueCa
+00000190: 7374 2f62 6c75 6563 6173 742f 7072 6570  st/bluecast/prep
+000001a0: 726f 6365 7373 696e 672f 7363 6865 6d61  rocessing/schema
+000001b0: 5f63 6865 636b 732e 7079 da08 5f5f 696e  _checks.py..__in
+000001c0: 6974 5f5f 0a00 0000 7302 0000 0000 017a  it__....s......z
+000001d0: 1753 6368 656d 6144 6574 6563 746f 722e  .SchemaDetector.
+000001e0: 5f5f 696e 6974 5f5f a901 da02 6466 6302  __init__....dfc.
+000001f0: 0000 0000 0000 0000 0000 0002 0000 0002  ................
+00000200: 0000 0043 0000 0073 1200 0000 7c01 6a00  ...C...s....|.j.
+00000210: a001 a100 7c00 5f02 7c00 6a02 5300 2901  ....|._.|.j.S.).
+00000220: 7a26 5374 6f72 6520 7468 6520 7363 6865  z&Store the sche
+00000230: 6d61 206f 6620 7468 6520 7472 6169 6e20  ma of the train 
+00000240: 6461 7461 7365 742e 2903 da07 636f 6c75  dataset.)...colu
+00000250: 6d6e 73da 0774 6f5f 6c69 7374 7206 0000  mns..to_listr...
+00000260: 0029 0272 0800 0000 720d 0000 0072 0900  .).r....r....r..
+00000270: 0000 7209 0000 0072 0a00 0000 da03 6669  ..r....r......fi
+00000280: 740d 0000 0073 0400 0000 0002 0c01 7a12  t....s........z.
+00000290: 5363 6865 6d61 4465 7465 6374 6f72 2e66  SchemaDetector.f
+000002a0: 6974 6302 0000 0000 0000 0000 0000 0004  itc.............
+000002b0: 0000 0004 0000 0003 0000 0073 7c00 0000  ...........s|...
+000002c0: 7400 8800 6a01 8301 7400 8801 6a02 8301  t...j...t...j...
+000002d0: 6b04 723a 8701 6601 6401 6402 8408 8800  k.r:..f.d.d.....
+000002e0: 6a01 4400 8301 7d02 7403 6403 7c02 9b00  j.D...}.t.d.|...
+000002f0: 6404 9d03 8301 8201 6e38 7400 8800 6a01  d.......n8t...j.
+00000300: 8301 7400 8801 6a02 8301 6b00 7272 8700  ..t...j...k.rr..
+00000310: 6601 6405 6402 8408 8801 6a02 4400 8301  f.d.d.....j.D...
+00000320: 7d03 7403 6406 7c03 9b00 6404 9d03 8301  }.t.d.|...d.....
+00000330: 8201 8800 8801 6a02 1900 5300 2907 7aca  ......j...S.).z.
+00000340: 4368 6563 6b20 6966 2074 6865 2074 6573  Check if the tes
+00000350: 7420 6461 7461 7365 7420 6861 7320 7468  t dataset has th
+00000360: 6520 7361 6d65 2073 6368 656d 6120 6173  e same schema as
+00000370: 2074 6865 2074 7261 696e 2064 6174 6173   the train datas
+00000380: 6574 2e0a 0a20 2020 2020 2020 2057 696c  et...        Wil
+00000390: 6c20 7261 6973 6520 616e 2065 7272 6f72  l raise an error
+000003a0: 2069 6620 7363 6865 6d61 206c 656e 6774   if schema lengt
+000003b0: 6820 646f 6573 206e 6f74 206d 6174 6368  h does not match
+000003c0: 2061 6e64 2077 696c 6c20 7261 6973 6520   and will raise 
+000003d0: 6120 7761 726e 696e 6720 696e 6469 6361  a warning indica
+000003e0: 7469 6e67 2074 6865 206d 6973 7369 6e67  ting the missing
+000003f0: 206f 7220 6578 7472 610a 2020 2020 2020   or extra.      
+00000400: 2020 636f 6c75 6d6e 732e 6301 0000 0000    columns.c.....
+00000410: 0000 0000 0000 0002 0000 0004 0000 0013  ................
+00000420: 0000 0073 1a00 0000 6700 7c00 5d12 7d01  ...s....g.|.].}.
+00000430: 7c01 8800 6a00 6b07 7204 7c01 9102 7104  |...j.k.r.|...q.
+00000440: 5300 7209 0000 0072 0500 0000 a902 da02  S.r....r........
+00000450: 2e30 da03 636f 6c72 0700 0000 7209 0000  .0..colr....r...
+00000460: 0072 0a00 0000 da0a 3c6c 6973 7463 6f6d  .r......<listcom
+00000470: 703e 1800 0000 7306 0000 0006 0002 000a  p>....s.........
+00000480: 007a 2c53 6368 656d 6144 6574 6563 746f  .z,SchemaDetecto
+00000490: 722e 7472 616e 7366 6f72 6d2e 3c6c 6f63  r.transform.<loc
+000004a0: 616c 733e 2e3c 6c69 7374 636f 6d70 3e7a  als>.<listcomp>z
+000004b0: 9354 6865 206e 756d 6265 7220 6f66 2063  .The number of c
+000004c0: 6f6c 756d 6e73 2069 6e20 7468 6520 7465  olumns in the te
+000004d0: 7374 2064 6174 6173 6574 2069 7320 6772  st dataset is gr
+000004e0: 6561 7465 7220 7468 616e 2074 6865 206e  eater than the n
+000004f0: 756d 6265 7220 6f66 2063 6f6c 756d 6e73  umber of columns
+00000500: 0a20 2020 2020 2020 2020 2020 2069 6e20  .            in 
+00000510: 7468 6520 7472 6169 6e20 6461 7461 7365  the train datase
+00000520: 742e 2046 6f75 6e64 2074 6865 2066 6f6c  t. Found the fol
+00000530: 6c6f 7769 6e67 206e 6577 2063 6f6c 756d  lowing new colum
+00000540: 6e73 3a20 da01 2e63 0100 0000 0000 0000  ns: ...c........
+00000550: 0000 0000 0200 0000 0400 0000 1300 0000  ................
+00000560: 731a 0000 0067 007c 005d 127d 017c 0188  s....g.|.].}.|..
+00000570: 006a 006b 0772 047c 0191 0271 0453 0072  .j.k.r.|...q.S.r
+00000580: 0900 0000 2901 720e 0000 0072 1100 0000  ....).r....r....
+00000590: 720c 0000 0072 0900 0000 720a 0000 0072  r....r....r....r
+000005a0: 1400 0000 1e00 0000 7306 0000 0006 0002  ........s.......
+000005b0: 000a 007a 9154 6865 206e 756d 6265 7220  ...z.The number 
+000005c0: 6f66 2063 6f6c 756d 6e73 2069 6e20 7468  of columns in th
+000005d0: 6520 7465 7374 2064 6174 6173 6574 2069  e test dataset i
+000005e0: 7320 736d 616c 6c65 7220 7468 616e 2074  s smaller than t
+000005f0: 6865 206e 756d 6265 7220 6f66 2063 6f6c  he number of col
+00000600: 756d 6e73 0a20 2020 2020 2020 2020 2020  umns.           
+00000610: 2069 6e20 7468 6520 7472 6169 6e20 6461   in the train da
+00000620: 7461 7365 742e 204d 6973 7369 6e67 2074  taset. Missing t
+00000630: 6865 2066 6f6c 6c6f 7769 6e67 2063 6f6c  he following col
+00000640: 756d 6e73 3a20 2904 da03 6c65 6e72 0e00  umns: )...lenr..
+00000650: 0000 7206 0000 00da 0a56 616c 7565 4572  ..r......ValueEr
+00000660: 726f 7229 0472 0800 0000 720d 0000 00da  ror).r....r.....
+00000670: 086e 6577 5f63 6f6c 73da 0c6d 6973 7369  .new_cols..missi
+00000680: 6e67 5f63 6f6c 7372 0900 0000 2902 720d  ng_colsr....).r.
+00000690: 0000 0072 0800 0000 720a 0000 00da 0974  ...r....r......t
+000006a0: 7261 6e73 666f 726d 1200 0000 731e 0000  ransform....s...
+000006b0: 0000 0514 0114 0102 0102 0102 ff06 ff06  ................
+000006c0: 0414 0114 0102 0102 0102 ff06 ff04 047a  ...............z
+000006d0: 1853 6368 656d 6144 6574 6563 746f 722e  .SchemaDetector.
+000006e0: 7472 616e 7366 6f72 6d4e 2909 da08 5f5f  transformN)...__
+000006f0: 6e61 6d65 5f5f da0a 5f5f 6d6f 6475 6c65  name__..__module
+00000700: 5f5f da0c 5f5f 7175 616c 6e61 6d65 5f5f  __..__qualname__
+00000710: da07 5f5f 646f 635f 5f72 0b00 0000 da02  ..__doc__r......
+00000720: 7064 da09 4461 7461 4672 616d 6572 1000  pd..DataFramer..
+00000730: 0000 721a 0000 0072 0900 0000 7209 0000  ..r....r....r...
+00000740: 0072 0900 0000 720a 0000 0072 0400 0000  .r....r....r....
+00000750: 0700 0000 7308 0000 0008 0104 0208 0310  ....s...........
+00000760: 0572 0400 0000 2907 721e 0000 00da 0674  .r....).r......t
+00000770: 7970 696e 6772 0200 0000 7203 0000 00da  ypingr....r.....
+00000780: 0670 616e 6461 7372 1f00 0000 7204 0000  .pandasr....r...
+00000790: 0072 0900 0000 7209 0000 0072 0900 0000  .r....r....r....
+000007a0: 720a 0000 00da 083c 6d6f 6475 6c65 3e01  r......<module>.
+000007b0: 0000 0073 0600 0000 0401 1002 0803       ...s..........
```

### Comparing `bluecast-0.5/bluecast/preprocessing/__pycache__/target_encoding.cpython-310.pyc` & `bluecast-0.7/bluecast/preprocessing/__pycache__/target_encoding.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.5/bluecast/preprocessing/__pycache__/target_encoding.cpython-38.pyc` & `bluecast-0.7/bluecast/preprocessing/__pycache__/target_encoding.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.5/bluecast/preprocessing/__pycache__/train_test_split.cpython-310.pyc` & `bluecast-0.7/bluecast/preprocessing/__pycache__/train_test_split.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.5/bluecast/preprocessing/__pycache__/train_test_split.cpython-38.pyc` & `bluecast-0.7/bluecast/preprocessing/__pycache__/train_test_split.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Thu Jun  8 04:28:32 2023 UTC, .py size: 1748 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 23% similar despite different names*

```diff
@@ -1,112 +1,146 @@
-00000000: 550d 0d0a 0000 0000 f058 8164 d406 0000  U........X.d....
+00000000: 550d 0d0a 0000 0000 a385 9264 370b 0000  U..........d7...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0006 0000 0040 0000 0073 6400 0000 6400  .....@...sd...d.
+00000020: 0008 0000 0040 0000 0073 9000 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d01 5a01 0100 6401  Z.d.d.l.m.Z...d.
-00000040: 6403 6c02 5a03 6401 6404 6c04 6d05 5a05  d.l.Z.d.d.l.m.Z.
-00000050: 0100 6401 6405 6c06 6d07 5a07 0100 640e  ..d.d.l.m.Z...d.
-00000060: 6503 6a08 6509 650a 6509 6408 9c04 6409  e.j.e.e.e.d...d.
-00000070: 640a 8405 5a0b 640f 6503 6a08 6509 6509  d...Z.d.e.j.e.e.
-00000080: 650c 640b 9c04 640c 640d 8405 5a0d 6403  e.d...d.d...Z.d.
-00000090: 5300 2910 7ab2 0a54 6869 7320 6d6f 6475  S.).z..This modu
-000000a0: 6c65 2063 6f6e 7461 696e 7320 6675 6e63  le contains func
-000000b0: 7469 6f6e 7320 746f 2073 706c 6974 2064  tions to split d
-000000c0: 6174 6120 696e 746f 2074 7261 696e 2061  ata into train a
-000000d0: 6e64 2074 6573 7420 7365 7473 2e0a 0a54  nd test sets...T
-000000e0: 6865 2074 7261 696e 2d74 6573 7420 7370  he train-test sp
-000000f0: 6c69 7420 6361 6e20 6265 2064 6f6e 6520  lit can be done 
-00000100: 696e 2074 776f 2077 6179 733a 0a20 2020  in two ways:.   
-00000110: 202d 2052 616e 646f 6d6c 790a 2020 2020   - Randomly.    
-00000120: 2d20 4261 7365 6420 6f6e 2061 2070 726f  - Based on a pro
-00000130: 7669 6465 6420 6f72 6465 7220 2869 2e65  vided order (i.e
-00000140: 2e20 7469 6d65 290a e900 0000 0029 01da  . time)......)..
-00000150: 0864 6174 6574 696d 654e 2901 da0f 6d6f  .datetimeN)...mo
-00000160: 6465 6c5f 7365 6c65 6374 696f 6e29 01da  del_selection)..
-00000170: 066c 6f67 6765 72e7 9a99 9999 9999 e93f  .logger........?
-00000180: e964 0000 0029 04da 0264 66da 0a74 6172  .d...)...df..tar
-00000190: 6765 745f 636f 6cda 0c72 616e 646f 6d5f  get_col..random_
-000001a0: 7374 6174 65da 0c73 7472 6174 6966 795f  state..stratify_
-000001b0: 636f 6c63 0500 0000 0000 0000 0000 0000  colc............
-000001c0: 0a00 0000 0700 0000 4300 0000 735a 0000  ........C...sZ..
-000001d0: 0074 0074 01a0 02a1 009b 0064 017c 029b  .t.t.......d.|..
-000001e0: 0064 029d 0483 0101 007c 007c 0119 00a0  .d.......|.|....
-000001f0: 03a1 007d 057c 006a 047c 0164 0364 048d  ...}.|.j.|.d.d..
-00000200: 027d 0074 056a 067c 007c 057c 027c 037c  .}.t.j.|.|.|.|.|
-00000210: 0464 058d 055c 047d 067d 077d 087d 097c  .d...\.}.}.}.}.|
-00000220: 067c 077c 087c 0966 0453 0029 067a 3b53  .|.|.|.f.S.).z;S
-00000230: 706c 6974 2064 6174 6120 696e 746f 2074  plit data into t
-00000240: 7261 696e 2061 6e64 2074 6573 742e 2053  rain and test. S
-00000250: 7472 6174 6966 6963 6174 696f 6e20 6973  tratification is
-00000260: 2070 6f73 7369 626c 652e 7a36 3a20 5374   possible.z6: St
-00000270: 6172 7420 6578 6563 7574 696e 6720 7472  art executing tr
-00000280: 6169 6e2d 7465 7374 2073 706c 6974 2077  ain-test split w
-00000290: 6974 6820 7472 6169 6e20 7369 7a65 206f  ith train size o
-000002a0: 6620 da01 2ee9 0100 0000 2901 da04 6178  f ........)...ax
-000002b0: 6973 2903 da0a 7472 6169 6e5f 7369 7a65  is)...train_size
-000002c0: 7209 0000 00da 0873 7472 6174 6966 7929  r......stratify)
-000002d0: 0772 0400 0000 7202 0000 00da 0675 7463  .r....r......utc
-000002e0: 6e6f 77da 0463 6f70 79da 0464 726f 7072  now..copy..dropr
-000002f0: 0300 0000 da10 7472 6169 6e5f 7465 7374  ......train_test
-00000300: 5f73 706c 6974 290a 7207 0000 0072 0800  _split).r....r..
-00000310: 0000 720e 0000 0072 0900 0000 720a 0000  ..r....r....r...
-00000320: 00da 0674 6172 6765 74da 0778 5f74 7261  ...target..x_tra
-00000330: 696e da06 785f 7465 7374 da07 795f 7472  in..x_test..y_tr
-00000340: 6169 6eda 0679 5f74 6573 74a9 0072 1900  ain..y_test..r..
-00000350: 0000 fa4d 2f68 6f6d 652f 7468 6f6d 6173  ...M/home/thomas
-00000360: 2f49 6465 6150 726f 6a65 6374 732f 426c  /IdeaProjects/Bl
-00000370: 7565 4361 7374 2f62 6c75 6563 6173 742f  ueCast/bluecast/
-00000380: 7072 6570 726f 6365 7373 696e 672f 7472  preprocessing/tr
-00000390: 6169 6e5f 7465 7374 5f73 706c 6974 2e70  ain_test_split.p
-000003a0: 79da 1674 7261 696e 5f74 6573 745f 7370  y..train_test_sp
-000003b0: 6c69 745f 6372 6f73 7310 0000 0073 1a00  lit_cross....s..
-000003c0: 0000 0008 0201 12ff 0403 0c01 0e01 0401  ................
-000003d0: 0201 0201 0201 0201 02fb 0e07 721b 0000  ............r...
-000003e0: 0029 0472 0700 0000 7208 0000 00da 0c73  .).r....r......s
-000003f0: 706c 6974 5f62 795f 636f 6c72 0e00 0000  plit_by_colr....
-00000400: 6304 0000 0000 0000 0000 0000 000b 0000  c...............
-00000410: 0005 0000 0043 0000 0073 8800 0000 7400  .....C...s....t.
-00000420: 7401 a002 a100 9b00 6401 7c03 9b00 6402  t.......d.|...d.
-00000430: 9d04 8301 0100 7403 7c00 6a04 8301 7d04  ......t.|.j...}.
-00000440: 7405 7c04 7c03 1400 8301 7d05 7c04 7c05  t.|.|.....}.|.|.
-00000450: 1800 7d06 7c02 7344 7c00 a006 a100 7d00  ..}.|.sD|.....}.
-00000460: 6e14 7c02 7258 7c00 6a07 7c02 6701 6403  n.|.rX|.j.|.g.d.
-00000470: 8d01 7d00 6e00 7c00 a008 7c05 a101 7d07  ..}.n.|...|...}.
-00000480: 7c00 a009 7c06 a101 7d08 7c07 7c01 1900  |...|...}.|.|...
-00000490: 7d09 7c08 7c01 1900 7d0a 7c07 7c08 7c09  }.|.|...}.|.|.|.
-000004a0: 7c0a 6604 5300 2904 7a45 5370 6c69 7420  |.f.S.).zESplit 
-000004b0: 6461 7461 2069 6e74 6f20 7472 6169 6e20  data into train 
-000004c0: 616e 6420 7465 7374 2062 6173 6564 206f  and test based o
-000004d0: 6e20 6120 7072 6f76 6964 6564 206f 7264  n a provided ord
-000004e0: 6572 2028 692e 652e 2074 696d 6529 2e7a  er (i.e. time).z
-000004f0: 3e3a 2053 7461 7274 2065 7865 6375 7469  >: Start executi
-00000500: 6e67 206f 7264 6572 6564 2074 7261 696e  ng ordered train
-00000510: 2d74 6573 7420 7370 6c69 7420 7769 7468  -test split with
-00000520: 2074 7261 696e 2073 697a 6520 6f66 2072   train size of r
-00000530: 0b00 0000 2901 da02 6279 290a 7204 0000  ....)...by).r...
-00000540: 0072 0200 0000 7210 0000 00da 036c 656e  .r....r......len
-00000550: da05 696e 6465 78da 0369 6e74 da0a 736f  ..index..int..so
-00000560: 7274 5f69 6e64 6578 da0b 736f 7274 5f76  rt_index..sort_v
-00000570: 616c 7565 73da 0468 6561 64da 0474 6169  alues..head..tai
-00000580: 6c29 0b72 0700 0000 7208 0000 0072 1c00  l).r....r....r..
-00000590: 0000 720e 0000 00da 066c 656e 6774 68da  ..r......length.
-000005a0: 0c74 7261 696e 5f6c 656e 6774 68da 0b74  .train_length..t
-000005b0: 6573 745f 6c65 6e67 7468 7215 0000 0072  est_lengthr....r
-000005c0: 1600 0000 7217 0000 0072 1800 0000 7219  ....r....r....r.
-000005d0: 0000 0072 1900 0000 721a 0000 00da 1574  ...r....r......t
-000005e0: 7261 696e 5f74 6573 745f 7370 6c69 745f  rain_test_split_
-000005f0: 7469 6d65 2700 0000 731e 0000 0000 0402  time'...s.......
-00000600: 0112 ff04 030a 010c 0108 0104 010a 0104  ................
-00000610: 0110 030a 010a 0108 0108 0172 2800 0000  ...........r(...
-00000620: 2903 7205 0000 0072 0600 0000 4e29 0172  ).r....r....N).r
-00000630: 0500 0000 290e da07 5f5f 646f 635f 5f72  ....)...__doc__r
-00000640: 0200 0000 da06 7061 6e64 6173 da02 7064  ......pandas..pd
-00000650: da07 736b 6c65 6172 6e72 0300 0000 da24  ..sklearnr.....$
-00000660: 626c 7565 6361 7374 2e67 656e 6572 616c  bluecast.general
-00000670: 5f75 7469 6c73 2e67 656e 6572 616c 5f75  _utils.general_u
-00000680: 7469 6c73 7204 0000 00da 0944 6174 6146  tilsr......DataF
-00000690: 7261 6d65 da03 7374 7272 2000 0000 721b  rame..strr ...r.
-000006a0: 0000 00da 0566 6c6f 6174 7228 0000 0072  .....floatr(...r
-000006b0: 1900 0000 7219 0000 0072 1900 0000 721a  ....r....r....r.
-000006c0: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
-000006d0: 0073 2800 0000 0407 0c02 0801 0c02 0c06  .s(.............
-000006e0: 0001 0001 00fb 0201 0401 0202 0201 02fb  ................
-000006f0: 0c18 00ff 0201 0400 0200 0200 02ff       ..............
+00000040: 6403 6c02 6d03 5a03 0100 6401 6404 6c04  d.l.m.Z...d.d.l.
+00000050: 5a05 6401 6405 6c06 6d07 5a07 0100 6401  Z.d.d.l.m.Z...d.
+00000060: 6406 6c08 6d09 5a09 0100 6413 6505 6a0a  d.l.m.Z...d.e.j.
+00000070: 650b 650c 650d 640a 9c04 640b 640c 8405  e.e.e.d...d.d...
+00000080: 5a0e 6414 6505 6a0a 650b 650b 650f 640d  Z.d.e.j.e.e.e.d.
+00000090: 9c04 640e 640f 8405 5a10 6415 6505 6a0a  ..d.d...Z.d.e.j.
+000000a0: 650b 6503 650b 1900 650f 650c 650d 6410  e.e.e...e.e.e.d.
+000000b0: 9c06 6411 6412 8405 5a11 6404 5300 2916  ..d.d...Z.d.S.).
+000000c0: 7ab2 0a54 6869 7320 6d6f 6475 6c65 2063  z..This module c
+000000d0: 6f6e 7461 696e 7320 6675 6e63 7469 6f6e  ontains function
+000000e0: 7320 746f 2073 706c 6974 2064 6174 6120  s to split data 
+000000f0: 696e 746f 2074 7261 696e 2061 6e64 2074  into train and t
+00000100: 6573 7420 7365 7473 2e0a 0a54 6865 2074  est sets...The t
+00000110: 7261 696e 2d74 6573 7420 7370 6c69 7420  rain-test split 
+00000120: 6361 6e20 6265 2064 6f6e 6520 696e 2074  can be done in t
+00000130: 776f 2077 6179 733a 0a20 2020 202d 2052  wo ways:.    - R
+00000140: 616e 646f 6d6c 790a 2020 2020 2d20 4261  andomly.    - Ba
+00000150: 7365 6420 6f6e 2061 2070 726f 7669 6465  sed on a provide
+00000160: 6420 6f72 6465 7220 2869 2e65 2e20 7469  d order (i.e. ti
+00000170: 6d65 290a e900 0000 0029 01da 0864 6174  me)......)...dat
+00000180: 6574 696d 6529 01da 084f 7074 696f 6e61  etime)...Optiona
+00000190: 6c4e 2901 da0f 6d6f 6465 6c5f 7365 6c65  lN)...model_sele
+000001a0: 6374 696f 6e29 01da 066c 6f67 6765 72e7  ction)...logger.
+000001b0: 9a99 9999 9999 e93f e964 0000 0046 2904  .......?.d...F).
+000001c0: da02 6466 da0a 7461 7267 6574 5f63 6f6c  ..df..target_col
+000001d0: da0c 7261 6e64 6f6d 5f73 7461 7465 da08  ..random_state..
+000001e0: 7374 7261 7469 6679 6305 0000 0000 0000  stratifyc.......
+000001f0: 0000 0000 000b 0000 0007 0000 0043 0000  .............C..
+00000200: 0073 8e00 0000 7400 7401 a002 a100 9b00  .s....t.t.......
+00000210: 6401 7c02 9b00 6402 9d04 8301 0100 7c00  d.|...d.......|.
+00000220: 7c01 1900 a003 a100 7d05 7c00 6a04 7c01  |.......}.|.j.|.
+00000230: 6403 6404 8d02 7d00 7c04 723c 7c05 7d06  d.d...}.|.r<|.}.
+00000240: 6e04 6405 7d06 7405 6a06 7c00 7c05 7c02  n.d.}.t.j.|.|.|.
+00000250: 7c03 7c06 6406 8d05 5c04 7d07 7d08 7d09  |.|.d...\.}.}.}.
+00000260: 7d0a 7c01 7c07 6a07 6b06 7282 7c07 6a04  }.|.|.j.k.r.|.j.
+00000270: 7c01 6403 6404 8d02 7d07 7c08 6a04 7c01  |.d.d...}.|.j.|.
+00000280: 6403 6404 8d02 7d08 7c07 7c08 7c09 7c0a  d.d...}.|.|.|.|.
+00000290: 6604 5300 2907 7a3b 5370 6c69 7420 6461  f.S.).z;Split da
+000002a0: 7461 2069 6e74 6f20 7472 6169 6e20 616e  ta into train an
+000002b0: 6420 7465 7374 2e20 5374 7261 7469 6669  d test. Stratifi
+000002c0: 6361 7469 6f6e 2069 7320 706f 7373 6962  cation is possib
+000002d0: 6c65 2e7a 363a 2053 7461 7274 2065 7865  le.z6: Start exe
+000002e0: 6375 7469 6e67 2074 7261 696e 2d74 6573  cuting train-tes
+000002f0: 7420 7370 6c69 7420 7769 7468 2074 7261  t split with tra
+00000300: 696e 2073 697a 6520 6f66 20da 012e e901  in size of .....
+00000310: 0000 00a9 01da 0461 7869 734e a903 da0a  .......axisN....
+00000320: 7472 6169 6e5f 7369 7a65 720a 0000 0072  train_sizer....r
+00000330: 0b00 0000 2908 7205 0000 0072 0200 0000  ....).r....r....
+00000340: da06 7574 636e 6f77 da04 636f 7079 da04  ..utcnow..copy..
+00000350: 6472 6f70 7204 0000 00da 1074 7261 696e  dropr......train
+00000360: 5f74 6573 745f 7370 6c69 74da 0763 6f6c  _test_split..col
+00000370: 756d 6e73 290b 7208 0000 0072 0900 0000  umns).r....r....
+00000380: 7211 0000 0072 0a00 0000 720b 0000 00da  r....r....r.....
+00000390: 0674 6172 6765 745a 0d73 7472 6174 6966  .targetZ.stratif
+000003a0: 795f 6461 7461 da07 785f 7472 6169 6eda  y_data..x_train.
+000003b0: 0678 5f74 6573 74da 0779 5f74 7261 696e  .x_test..y_train
+000003c0: da06 795f 7465 7374 a900 721c 0000 00fa  ..y_test..r.....
+000003d0: 4d2f 686f 6d65 2f74 686f 6d61 732f 4964  M/home/thomas/Id
+000003e0: 6561 5072 6f6a 6563 7473 2f42 6c75 6543  eaProjects/BlueC
+000003f0: 6173 742f 626c 7565 6361 7374 2f70 7265  ast/bluecast/pre
+00000400: 7072 6f63 6573 7369 6e67 2f74 7261 696e  processing/train
+00000410: 5f74 6573 745f 7370 6c69 742e 7079 da16  _test_split.py..
+00000420: 7472 6169 6e5f 7465 7374 5f73 706c 6974  train_test_split
+00000430: 5f63 726f 7373 1100 0000 7326 0000 0000  _cross....s&....
+00000440: 0802 0112 ff04 030c 010e 0104 0106 0204  ................
+00000450: 0204 0102 0102 0102 0102 0102 fb0e 070a  ................
+00000460: 010e 010e 0172 1e00 0000 2904 7208 0000  .....r....).r...
+00000470: 0072 0900 0000 da0c 7370 6c69 745f 6279  .r......split_by
+00000480: 5f63 6f6c 7211 0000 0063 0400 0000 0000  _colr....c......
+00000490: 0000 0000 0000 0b00 0000 0500 0000 4300  ..............C.
+000004a0: 0000 73ae 0000 0074 0074 01a0 02a1 009b  ..s....t.t......
+000004b0: 0064 017c 039b 0064 029d 0483 0101 0074  .d.|...d.......t
+000004c0: 037c 006a 0483 017d 0474 057c 047c 0314  .|.j...}.t.|.|..
+000004d0: 0083 017d 057c 047c 0518 007d 067c 0273  ...}.|.|...}.|.s
+000004e0: 447c 00a0 06a1 007d 006e 147c 0272 587c  D|.....}.n.|.rX|
+000004f0: 006a 077c 0267 0164 038d 017d 006e 007c  .j.|.g.d...}.n.|
+00000500: 00a0 087c 05a1 017d 077c 00a0 097c 06a1  ...|...}.|...|..
+00000510: 017d 087c 077c 0119 007d 097c 087c 0119  .}.|.|...}.|.|..
+00000520: 007d 0a7c 017c 076a 0a6b 0672 a27c 076a  .}.|.|.j.k.r.|.j
+00000530: 0b7c 0164 0464 058d 027d 077c 086a 0b7c  .|.d.d...}.|.j.|
+00000540: 0164 0464 058d 027d 087c 077c 087c 097c  .d.d...}.|.|.|.|
+00000550: 0a66 0453 0029 067a 4553 706c 6974 2064  .f.S.).zESplit d
+00000560: 6174 6120 696e 746f 2074 7261 696e 2061  ata into train a
+00000570: 6e64 2074 6573 7420 6261 7365 6420 6f6e  nd test based on
+00000580: 2061 2070 726f 7669 6465 6420 6f72 6465   a provided orde
+00000590: 7220 2869 2e65 2e20 7469 6d65 292e 7a3e  r (i.e. time).z>
+000005a0: 3a20 5374 6172 7420 6578 6563 7574 696e  : Start executin
+000005b0: 6720 6f72 6465 7265 6420 7472 6169 6e2d  g ordered train-
+000005c0: 7465 7374 2073 706c 6974 2077 6974 6820  test split with 
+000005d0: 7472 6169 6e20 7369 7a65 206f 6620 720c  train size of r.
+000005e0: 0000 0029 01da 0262 7972 0d00 0000 720e  ...)...byr....r.
+000005f0: 0000 0029 0c72 0500 0000 7202 0000 0072  ...).r....r....r
+00000600: 1200 0000 da03 6c65 6eda 0569 6e64 6578  ......len..index
+00000610: da03 696e 74da 0a73 6f72 745f 696e 6465  ..int..sort_inde
+00000620: 78da 0b73 6f72 745f 7661 6c75 6573 da04  x..sort_values..
+00000630: 6865 6164 da04 7461 696c 7216 0000 0072  head..tailr....r
+00000640: 1400 0000 290b 7208 0000 0072 0900 0000  ....).r....r....
+00000650: 721f 0000 0072 1100 0000 da06 6c65 6e67  r....r......leng
+00000660: 7468 da0c 7472 6169 6e5f 6c65 6e67 7468  th..train_length
+00000670: da0b 7465 7374 5f6c 656e 6774 6872 1800  ..test_lengthr..
+00000680: 0000 7219 0000 0072 1a00 0000 721b 0000  ..r....r....r...
+00000690: 0072 1c00 0000 721c 0000 0072 1d00 0000  .r....r....r....
+000006a0: da15 7472 6169 6e5f 7465 7374 5f73 706c  ..train_test_spl
+000006b0: 6974 5f74 696d 6530 0000 0073 2400 0000  it_time0...s$...
+000006c0: 0004 0201 12ff 0403 0a01 0c01 0801 0401  ................
+000006d0: 0a01 0401 1003 0a01 0a01 0801 0802 0a01  ................
+000006e0: 0e01 0e01 722b 0000 0029 0672 0800 0000  ....r+...).r....
+000006f0: 7209 0000 0072 1f00 0000 7211 0000 0072  r....r....r....r
+00000700: 0a00 0000 720b 0000 0063 0600 0000 0000  ....r....c......
+00000710: 0000 0000 0000 0a00 0000 0700 0000 4300  ..............C.
+00000720: 0000 7348 0000 007c 0264 006b 0972 2274  ..sH...|.d.k.r"t
+00000730: 007c 007c 017c 027c 0364 018d 045c 047d  .|.|.|.|.d...\.}
+00000740: 067d 077d 087d 096e 1a74 017c 007c 017c  .}.}.}.n.t.|.|.|
+00000750: 037c 047c 0564 028d 055c 047d 067d 077d  .|.|.d...\.}.}.}
+00000760: 087d 097c 067c 077c 087c 0966 0453 0029  .}.|.|.|.|.f.S.)
+00000770: 034e 2901 7211 0000 0072 1000 0000 2902  .N).r....r....).
+00000780: 722b 0000 0072 1e00 0000 290a 7208 0000  r+...r....).r...
+00000790: 0072 0900 0000 721f 0000 0072 1100 0000  .r....r....r....
+000007a0: 720a 0000 0072 0b00 0000 7218 0000 0072  r....r....r....r
+000007b0: 1900 0000 721a 0000 0072 1b00 0000 721c  ....r....r....r.
+000007c0: 0000 0072 1c00 0000 721d 0000 0072 1500  ...r....r....r..
+000007d0: 0000 4b00 0000 731e 0000 0000 0808 0102  ..K...s.........
+000007e0: 0102 0102 0102 0102 fc10 0702 0102 0102  ................
+000007f0: 0102 0102 0102 fb0e 0772 1500 0000 2903  .........r....).
+00000800: 7206 0000 0072 0700 0000 4629 0172 0600  r....r....F).r..
+00000810: 0000 2904 4e72 0600 0000 7201 0000 0046  ..).Nr....r....F
+00000820: 2912 da07 5f5f 646f 635f 5f72 0200 0000  )...__doc__r....
+00000830: da06 7479 7069 6e67 7203 0000 00da 0670  ..typingr......p
+00000840: 616e 6461 73da 0270 64da 0773 6b6c 6561  andas..pd..sklea
+00000850: 726e 7204 0000 00da 2462 6c75 6563 6173  rnr.....$bluecas
+00000860: 742e 6765 6e65 7261 6c5f 7574 696c 732e  t.general_utils.
+00000870: 6765 6e65 7261 6c5f 7574 696c 7372 0500  general_utilsr..
+00000880: 0000 da09 4461 7461 4672 616d 65da 0373  ....DataFrame..s
+00000890: 7472 7223 0000 00da 0462 6f6f 6c72 1e00  trr#.....boolr..
+000008a0: 0000 da05 666c 6f61 7472 2b00 0000 7215  ....floatr+...r.
+000008b0: 0000 0072 1c00 0000 721c 0000 0072 1c00  ...r....r....r..
+000008c0: 0000 721d 0000 00da 083c 6d6f 6475 6c65  ..r......<module
+000008d0: 3e01 0000 0073 4200 0000 0407 0c01 0c02  >....sB.........
+000008e0: 0801 0c02 0c06 0001 0001 00fb 0201 0401  ................
+000008f0: 0202 0201 02fb 0c20 00ff 0201 0400 0200  ....... ........
+00000900: 0200 02ff 0c1e 0001 0001 0001 00fa 0201  ................
+00000910: 0401 0201 0601 0201 0201 02fa            ............
```

### Comparing `bluecast-0.5/bluecast/preprocessing/custom.py` & `bluecast-0.7/bluecast/preprocessing/custom.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.5/bluecast/preprocessing/datetime_features.py` & `bluecast-0.7/bluecast/preprocessing/datetime_features.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.5/bluecast/preprocessing/encode_target_labels.py` & `bluecast-0.7/bluecast/preprocessing/encode_target_labels.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.5/bluecast/preprocessing/feature_selection.py` & `bluecast-0.7/bluecast/preprocessing/feature_selection.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.5/bluecast/preprocessing/feature_types.py` & `bluecast-0.7/bluecast/preprocessing/feature_types.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.5/bluecast/preprocessing/nulls_and_infs.py` & `bluecast-0.7/bluecast/preprocessing/nulls_and_infs.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.5/bluecast/preprocessing/schema_checks.py` & `bluecast-0.7/bluecast/preprocessing/schema_checks.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.5/bluecast/preprocessing/target_encoding.py` & `bluecast-0.7/bluecast/preprocessing/target_encoding.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.5/bluecast/preprocessing/train_test_split.py` & `bluecast-0.7/bluecast/preprocessing/train_test_split.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.5/bluecast/tests/__pycache__/test_cast.cpython-310-pytest-6.2.5.pyc` & `bluecast-0.7/bluecast/tests/__pycache__/test_cast.cpython-310-pytest-6.2.5.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun Jun 25 05:34:02 2023 UTC, .py size: 6604 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 cad1 9764 cc19 0000  o..........d....
+00000000: 6f0d 0d0a 0000 0000 4717 9c64 151a 0000  o.......G..d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 0a01 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6400 6402 6c06 6d07  ..m.Z...d.d.l.m.
 00000050: 5a07 6d08 5a08 0100 6400 6401 6c09 5a0a  Z.m.Z...d.d.l.Z.
 00000060: 6400 6401 6c0b 5a0c 6400 6401 6c0d 5a0d  d.d.l.Z.d.d.l.Z.
 00000070: 6400 6401 6c0e 5a0f 6400 6403 6c10 6d11  d.d.l.Z.d.d.l.m.
@@ -47,500 +47,502 @@
 000002e0: 6f6d 6173 2f49 6465 6150 726f 6a65 6374  omas/IdeaProject
 000002f0: 732f 426c 7565 4361 7374 2f62 6c75 6563  s/BlueCast/bluec
 00000300: 6173 742f 7465 7374 732f 7465 7374 5f63  ast/tests/test_c
 00000310: 6173 742e 7079 da19 7379 6e74 6865 7469  ast.py..syntheti
 00000320: 635f 7472 6169 6e5f 7465 7374 5f64 6174  c_train_test_dat
 00000330: 6117 0000 0073 0600 0000 0c02 0c01 0801  a....s..........
 00000340: 721a 0000 0063 0100 0000 0000 0000 0000  r....c..........
-00000350: 0000 1000 0000 0a00 0000 4300 0000 73ba  ..........C...s.
+00000350: 0000 1000 0000 0a00 0000 4300 0000 73d0  ..........C...s.
 00000360: 0200 007c 0064 0119 007d 017c 0064 0219  ...|.d...}.|.d..
 00000370: 007d 0274 0083 007d 0364 037c 035f 0164  .}.t...}.d.|._.d
 00000380: 047c 035f 0274 0383 007d 0464 057c 045f  .|._.t...}.d.|._
 00000390: 0464 067c 045f 0564 027c 045f 0647 0064  .d.|._.d.|._.G.d
 000003a0: 0764 0884 0064 0874 0783 037d 057c 0583  .d...d.t...}.|..
 000003b0: 007d 0674 0864 0964 0a7c 047c 037c 0664  .}.t.d.d.|.|.|.d
-000003c0: 0b8d 057d 077c 076a 097c 0164 0a64 0c8d  ...}.|.j.|.d.d..
-000003d0: 0201 0074 0a64 0d83 0101 007c 07a0 0b7c  ...t.d.....|...|
-000003e0: 026a 0c64 0a64 0264 0e8d 02a1 015c 027d  .j.d.d.d.....\.}
-000003f0: 087d 0974 0a64 0f83 0101 0074 0d7c 0883  .}.t.d.....t.|..
-00000400: 017d 0a7c 026a 0e7d 0b74 0d7c 0b83 017d  .}.|.j.}.t.|...}
-00000410: 0c7c 0a7c 0c6b 027d 0d7c 0d73 c874 0fa0  .|.|.k.}.|.s.t..
-00000420: 1064 107c 0d66 0164 117c 0a7c 0c66 02a1  .d.|.f.d.|.|.f..
-00000430: 0464 1274 11a0 12a1 0076 0073 7274 0fa0  .d.t.....v.srt..
-00000440: 1374 0da1 0172 7774 0fa0 1474 0da1 016e  .t...rwt...t...n
-00000450: 0164 1264 1374 11a0 12a1 0076 0073 8374  .d.d.t.....v.s.t
-00000460: 0fa0 137c 08a1 0172 8874 0fa0 147c 08a1  ...|...r.t...|..
-00000470: 016e 0164 1374 0fa0 147c 0aa1 0164 1274  .n.d.t...|...d.t
-00000480: 11a0 12a1 0076 0073 9874 0fa0 1374 0da1  .....v.s.t...t..
-00000490: 0172 9d74 0fa0 1474 0da1 016e 0164 1264  .r.t...t...n.d.d
-000004a0: 1474 11a0 12a1 0076 0073 a974 0fa0 137c  .t.....v.s.t...|
-000004b0: 02a1 0172 ae74 0fa0 147c 02a1 016e 0164  ...r.t...|...n.d
-000004c0: 1474 0fa0 147c 0ba1 0174 0fa0 147c 0ca1  .t...|...t...|..
-000004d0: 0164 159c 0716 007d 0e64 1664 177c 0e69  .d.....}.d.d.|.i
-000004e0: 0116 007d 0f74 1574 0fa0 167c 0fa1 0183  ...}.t.t...|....
-000004f0: 0182 0164 1804 007d 0a04 007d 0d04 007d  ...d...}...}...}
-00000500: 0b7d 0c74 0d7c 0983 017d 0a7c 026a 0e7d  .}.t.|...}.|.j.}
-00000510: 0b74 0d7c 0b83 017d 0c7c 0a7c 0c6b 027d  .t.|...}.|.|.k.}
-00000520: 0d7c 0d90 0173 5374 0fa0 1064 107c 0d66  .|...sSt...d.|.f
-00000530: 0164 117c 0a7c 0c66 02a1 0464 1274 11a0  .d.|.|.f...d.t..
-00000540: 12a1 0076 0073 f774 0fa0 1374 0da1 0172  ...v.s.t...t...r
-00000550: fc74 0fa0 1474 0da1 016e 0164 1264 1974  .t...t...n.d.d.t
-00000560: 11a0 12a1 0076 0090 0173 0a74 0fa0 137c  .....v...s.t...|
-00000570: 09a1 0190 0172 0f74 0fa0 147c 09a1 016e  .....r.t...|...n
-00000580: 0164 1974 0fa0 147c 0aa1 0164 1274 11a0  .d.t...|...d.t..
-00000590: 12a1 0076 0090 0173 2174 0fa0 1374 0da1  ...v...s!t...t..
-000005a0: 0190 0172 2674 0fa0 1474 0da1 016e 0164  ...r&t...t...n.d
-000005b0: 1264 1474 11a0 12a1 0076 0090 0173 3474  .d.t.....v...s4t
-000005c0: 0fa0 137c 02a1 0190 0172 3974 0fa0 147c  ...|.....r9t...|
-000005d0: 02a1 016e 0164 1474 0fa0 147c 0ba1 0174  ...n.d.t...|...t
-000005e0: 0fa0 147c 0ca1 0164 159c 0716 007d 0e64  ...|...d.....}.d
-000005f0: 1664 177c 0e69 0116 007d 0f74 1574 0fa0  .d.|.i...}.t.t..
-00000600: 167c 0fa1 0183 0182 0164 1804 007d 0a04  .|.......d...}..
-00000610: 007d 0d04 007d 0b7d 0c64 1853 0029 1a7a  .}...}.}.d.S.).z
-00000620: 2254 6573 7420 7468 6174 2074 6573 7473  "Test that tests
-00000630: 2074 6865 2042 6c75 6543 6173 7420 636c   the BlueCast cl
-00000640: 6173 7372 0100 0000 e901 0000 00e9 6400  assr..........d.
-00000650: 0000 e910 0000 00e9 0a00 0000 4663 0000  ............Fc..
-00000660: 0000 0000 0000 0000 0000 0000 0000 0c00  ................
-00000670: 0000 4000 0000 7380 0000 0065 005a 0164  ..@...s....e.Z.d
-00000680: 005a 0264 0165 036a 0464 0265 036a 0466  .Z.d.e.j.d.e.j.f
-00000690: 0464 0364 0484 045a 0564 0165 036a 0464  .d.d...Z.d.e.j.d
-000006a0: 0565 036a 0664 0265 0765 036a 0465 036a  .e.j.d.e.e.j.e.j
-000006b0: 0666 0219 0066 0664 0664 0784 045a 0809  .f...f.d.d...Z..
-000006c0: 0809 0964 0d64 0165 036a 0464 0565 0965  ...d.d.e.j.d.e.e
-000006d0: 036a 0619 0064 0a65 0a64 0265 0765 036a  .j...d.e.d.e.e.j
-000006e0: 0465 0965 036a 0619 0066 0219 0066 0864  .e.e.j...f...f.d
-000006f0: 0b64 0c84 055a 0b64 0853 0029 0e7a 3d74  .d...Z.d.S.).z=t
-00000700: 6573 745f 626c 7565 7072 696e 745f 7867  est_blueprint_xg
-00000710: 626f 6f73 742e 3c6c 6f63 616c 733e 2e4d  boost.<locals>.M
-00000720: 7943 7573 746f 6d4c 6173 744d 696c 6550  yCustomLastMileP
-00000730: 7265 7072 6f63 6573 7369 6e67 da02 6466  reprocessing..df
-00000740: 7212 0000 0063 0200 0000 0000 0000 0000  r....c..........
-00000750: 0000 0200 0000 0300 0000 5300 0000 7314  ..........S...s.
-00000760: 0000 007c 0164 011b 007d 0164 027c 0164  ...|.d...}.d.|.d
-00000770: 033c 007c 0153 0029 044e e902 0000 00e9  .<.|.S.).N......
-00000780: 0500 0000 5a0a 6375 7374 6f6d 5f63 6f6c  ....Z.custom_col
-00000790: 7218 0000 0029 02da 0473 656c 6672 1f00  r....)...selfr..
-000007a0: 0000 7218 0000 0072 1800 0000 7219 0000  ..r....r....r...
-000007b0: 00da 0f63 7573 746f 6d5f 6675 6e63 7469  ...custom_functi
-000007c0: 6f6e 2c00 0000 7306 0000 0008 0108 0104  on,...s.........
-000007d0: 017a 4d74 6573 745f 626c 7565 7072 696e  .zMtest_blueprin
-000007e0: 745f 7867 626f 6f73 742e 3c6c 6f63 616c  t_xgboost.<local
-000007f0: 733e 2e4d 7943 7573 746f 6d4c 6173 744d  s>.MyCustomLastM
-00000800: 696c 6550 7265 7072 6f63 6573 7369 6e67  ilePreprocessing
-00000810: 2e63 7573 746f 6d5f 6675 6e63 7469 6f6e  .custom_function
-00000820: da06 7461 7267 6574 6303 0000 0000 0000  ..targetc.......
-00000830: 0000 0000 0003 0000 0003 0000 0053 0000  .............S..
-00000840: 0073 2600 0000 7c00 a000 7c01 a101 7d01  .s&...|...|...}.
-00000850: 7c01 a001 6401 a101 7d01 7c02 a001 6401  |...d...}.|...d.
-00000860: a101 7d02 7c01 7c02 6602 5300 2902 4e69  ..}.|.|.f.S.).Ni
-00000870: e803 0000 2902 7223 0000 00da 0468 6561  ....).r#.....hea
-00000880: 64a9 0372 2200 0000 721f 0000 0072 2400  d..r"...r....r$.
-00000890: 0000 7218 0000 0072 1800 0000 7219 0000  ..r....r....r...
-000008a0: 00da 0d66 6974 5f74 7261 6e73 666f 726d  ...fit_transform
-000008b0: 3100 0000 7308 0000 000a 030a 010a 0108  1...s...........
-000008c0: 017a 4b74 6573 745f 626c 7565 7072 696e  .zKtest_blueprin
-000008d0: 745f 7867 626f 6f73 742e 3c6c 6f63 616c  t_xgboost.<local
-000008e0: 733e 2e4d 7943 7573 746f 6d4c 6173 744d  s>.MyCustomLastM
-000008f0: 696c 6550 7265 7072 6f63 6573 7369 6e67  ilePreprocessing
-00000900: 2e66 6974 5f74 7261 6e73 666f 726d 4e46  .fit_transformNF
-00000910: da0e 7072 6564 6963 746f 6e5f 6d6f 6465  ..predicton_mode
-00000920: 6304 0000 0000 0000 0000 0000 0004 0000  c...............
-00000930: 0003 0000 0053 0000 0073 3600 0000 7c00  .....S...s6...|.
-00000940: a000 7c01 a101 7d01 7c03 7317 7401 7c02  ..|...}.|.s.t.|.
-00000950: 7402 6a03 8302 7217 7c01 a004 6401 a101  t.j...r.|...d...
-00000960: 7d01 7c02 a004 6401 a101 7d02 7c01 7c02  }.|...d...}.|.|.
-00000970: 6602 5300 2902 4e72 1c00 0000 2905 7223  f.S.).Nr....).r#
-00000980: 0000 00da 0a69 7369 6e73 7461 6e63 65da  .....isinstance.
-00000990: 0270 64da 0653 6572 6965 7372 2500 0000  .pd..Seriesr%...
-000009a0: a904 7222 0000 0072 1f00 0000 7224 0000  ..r"...r....r$..
-000009b0: 0072 2800 0000 7218 0000 0072 1800 0000  .r(...r....r....
-000009c0: 7219 0000 00da 0974 7261 6e73 666f 726d  r......transform
-000009d0: 3900 0000 730a 0000 000a 0610 010a 010a  9...s...........
-000009e0: 0108 017a 4774 6573 745f 626c 7565 7072  ...zGtest_bluepr
-000009f0: 696e 745f 7867 626f 6f73 742e 3c6c 6f63  int_xgboost.<loc
-00000a00: 616c 733e 2e4d 7943 7573 746f 6d4c 6173  als>.MyCustomLas
-00000a10: 744d 696c 6550 7265 7072 6f63 6573 7369  tMilePreprocessi
-00000a20: 6e67 2e74 7261 6e73 666f 726d a902 4e46  ng.transform..NF
-00000a30: 290c da08 5f5f 6e61 6d65 5f5f da0a 5f5f  )...__name__..__
-00000a40: 6d6f 6475 6c65 5f5f da0c 5f5f 7175 616c  module__..__qual
-00000a50: 6e61 6d65 5f5f 722a 0000 00da 0944 6174  name__r*.....Dat
-00000a60: 6146 7261 6d65 7223 0000 0072 2b00 0000  aFramer#...r+...
-00000a70: 7203 0000 0072 2700 0000 7202 0000 00da  r....r'...r.....
-00000a80: 0462 6f6f 6c72 2d00 0000 7218 0000 0072  .boolr-...r....r
-00000a90: 1800 0000 7218 0000 0072 1900 0000 da1d  ....r....r......
-00000aa0: 4d79 4375 7374 6f6d 4c61 7374 4d69 6c65  MyCustomLastMile
-00000ab0: 5072 6570 726f 6365 7373 696e 672b 0000  Preprocessing+..
-00000ac0: 0073 2800 0000 0800 1601 0205 0401 02ff  .s(.............
-00000ad0: 0401 02ff 0e02 0afe 020b 0201 04fc 0402  ................
-00000ae0: 02fe 0803 02fd 0204 02fc 1205 0efb 7234  ..............r4
-00000af0: 0000 00da 0662 696e 6172 7972 2400 0000  .....binaryr$...
-00000b00: 2905 da0d 636c 6173 735f 7072 6f62 6c65  )...class_proble
-00000b10: 6dda 0d74 6172 6765 745f 636f 6c75 6d6e  m..target_column
-00000b20: da0d 636f 6e66 5f74 7261 696e 696e 675a  ..conf_trainingZ
-00000b30: 0c63 6f6e 665f 7867 626f 6f73 74da 1c63  .conf_xgboost..c
-00000b40: 7573 746f 6d5f 6c61 7374 5f6d 696c 655f  ustom_last_mile_
-00000b50: 636f 6d70 7574 6174 696f 6e29 015a 0a74  computation).Z.t
-00000b60: 6172 6765 745f 636f 6c7a 1641 7574 6f74  arget_colz.Autot
-00000b70: 756e 696e 6720 7375 6363 6573 7366 756c  uning successful
-00000b80: 2e29 015a 0461 7869 737a 1650 7265 6469  .).Z.axisz.Predi
-00000b90: 6374 696e 6720 7375 6363 6573 7366 756c  cting successful
-00000ba0: 2e29 01fa 023d 3d29 017a 6b25 2870 7933  .)...==).zk%(py3
-00000bb0: 2973 0a7b 2528 7079 3329 7320 3d20 2528  )s.{%(py3)s = %(
-00000bc0: 7079 3029 7328 2528 7079 3129 7329 0a7d  py0)s(%(py1)s).}
-00000bd0: 203d 3d20 2528 7079 3130 2973 0a7b 2528   == %(py10)s.{%(
-00000be0: 7079 3130 2973 203d 2025 2870 7935 2973  py10)s = %(py5)s
-00000bf0: 2825 2870 7938 2973 0a7b 2528 7079 3829  (%(py8)s.{%(py8)
-00000c00: 7320 3d20 2528 7079 3629 732e 696e 6465  s = %(py6)s.inde
-00000c10: 780a 7d29 0a7d da03 6c65 6eda 0779 5f70  x.}).}..len..y_p
-00000c20: 726f 6273 7217 0000 0029 07da 0370 7930  robsr....)...py0
-00000c30: da03 7079 315a 0370 7933 5a03 7079 35da  ..py1Z.py3Z.py5.
-00000c40: 0370 7936 5a03 7079 385a 0470 7931 307a  .py6Z.py8Z.py10z
-00000c50: 0f61 7373 6572 7420 2528 7079 3132 2973  .assert %(py12)s
-00000c60: 5a04 7079 3132 4eda 0979 5f63 6c61 7373  Z.py12N..y_class
-00000c70: 6573 2917 720b 0000 005a 0973 7465 7073  es).r....Z.steps
-00000c80: 5f6d 6178 5a0e 6e75 6d5f 6c65 6176 6573  _maxZ.num_leaves
-00000c90: 5f6d 6178 720a 0000 00da 1c68 7970 6572  _maxr......hyper
-00000ca0: 7061 7261 6d65 7465 725f 7475 6e69 6e67  parameter_tuning
-00000cb0: 5f72 6f75 6e64 73da 1865 6e61 626c 655f  _rounds..enable_
-00000cc0: 6665 6174 7572 655f 7365 6c65 6374 696f  feature_selectio
-00000cd0: 6eda 1468 7970 6572 7475 6e69 6e67 5f63  n..hypertuning_c
-00000ce0: 765f 666f 6c64 7372 0f00 0000 7209 0000  v_foldsr....r...
-00000cf0: 00da 0366 6974 da05 7072 696e 74da 0770  ...fit..print..p
-00000d00: 7265 6469 6374 5a04 6472 6f70 723b 0000  redictZ.dropr;..
-00000d10: 00da 0569 6e64 6578 da0a 4070 7974 6573  ...index..@pytes
-00000d20: 745f 6172 da11 5f63 616c 6c5f 7265 7072  t_ar.._call_repr
-00000d30: 636f 6d70 6172 65da 0c40 7079 5f62 7569  compare..@py_bui
-00000d40: 6c74 696e 73da 066c 6f63 616c 73da 185f  ltins..locals.._
-00000d50: 7368 6f75 6c64 5f72 6570 725f 676c 6f62  should_repr_glob
-00000d60: 616c 5f6e 616d 65da 095f 7361 6665 7265  al_name.._safere
-00000d70: 7072 da0e 4173 7365 7274 696f 6e45 7272  pr..AssertionErr
-00000d80: 6f72 da13 5f66 6f72 6d61 745f 6578 706c  or.._format_expl
-00000d90: 616e 6174 696f 6e29 1072 1a00 0000 7216  anation).r....r.
-00000da0: 0000 0072 1700 0000 5a14 7867 626f 6f73  ...r....Z.xgboos
-00000db0: 745f 7061 7261 6d5f 636f 6e66 6967 da0c  t_param_config..
-00000dc0: 7472 6169 6e5f 636f 6e66 6967 7234 0000  train_configr4..
-00000dd0: 0072 3900 0000 5a06 6175 746f 6d6c 723c  .r9...Z.automlr<
-00000de0: 0000 0072 4000 0000 5a0b 4070 795f 6173  ...r@...Z.@py_as
-00000df0: 7365 7274 325a 0b40 7079 5f61 7373 6572  sert2Z.@py_asser
-00000e00: 7437 5a0b 4070 795f 6173 7365 7274 395a  t7Z.@py_assert9Z
-00000e10: 0b40 7079 5f61 7373 6572 7434 5a0c 4070  .@py_assert4Z.@p
-00000e20: 795f 666f 726d 6174 3131 5a0c 4070 795f  y_format11Z.@py_
-00000e30: 666f 726d 6174 3133 7218 0000 0072 1800  format13r....r..
-00000e40: 0000 7219 0000 00da 1674 6573 745f 626c  ..r......test_bl
-00000e50: 7565 7072 696e 745f 7867 626f 6f73 741e  ueprint_xgboost.
-00000e60: 0000 0073 3400 0000 0802 0801 0601 0601  ...s4...........
-00000e70: 0601 0601 0601 0601 0601 1003 061a 0202  ................
-00000e80: 0201 0201 0201 0201 0201 06fb 0e07 0801  ................
-00000e90: 1801 0801 fe01 0a00 fe01 1c00 7251 0000  ............rQ..
-00000ea0: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
-00000eb0: 0000 0a00 0000 4000 0000 7356 0000 0065  ......@...sV...e
-00000ec0: 005a 0164 005a 0264 0164 0284 005a 0364  .Z.d.Z.d.d...Z.d
-00000ed0: 0365 046a 0564 0465 046a 0564 0565 046a  .e.j.d.e.j.d.e.j
-00000ee0: 0664 0665 046a 0664 0764 0866 0a64 0964  .d.e.j.d.d.f.d.d
-00000ef0: 0a84 045a 0764 0b65 046a 0564 0765 0865  ...Z.d.e.j.d.e.e
-00000f00: 0965 0a66 0219 0066 0464 0c64 0d84 045a  .e.f...f.d.d...Z
-00000f10: 0b64 0853 0029 0eda 0b43 7573 746f 6d4d  .d.S.)...CustomM
-00000f20: 6f64 656c 6301 0000 0000 0000 0000 0000  odelc...........
-00000f30: 0001 0000 0002 0000 0043 0000 0073 0a00  .........C...s..
-00000f40: 0000 6400 7c00 5f00 6400 5300 a901 4e29  ..d.|._.d.S...N)
-00000f50: 01da 056d 6f64 656c 2901 7222 0000 0072  ...model).r"...r
-00000f60: 1800 0000 7218 0000 0072 1900 0000 da08  ....r....r......
-00000f70: 5f5f 696e 6974 5f5f 5700 0000 7302 0000  __init__W...s...
-00000f80: 000a 017a 1443 7573 746f 6d4d 6f64 656c  ...z.CustomModel
-00000f90: 2e5f 5f69 6e69 745f 5fda 0778 5f74 7261  .__init__..x_tra
-00000fa0: 696e da06 785f 7465 7374 da07 795f 7472  in..x_test..y_tr
-00000fb0: 6169 6eda 0679 5f74 6573 7472 1200 0000  ain..y_testr....
-00000fc0: 4e63 0500 0000 0000 0000 0000 0000 0500  Nc..............
-00000fd0: 0000 0400 0000 4300 0000 731a 0000 0074  ......C...s....t
-00000fe0: 0083 007c 005f 017c 006a 01a0 027c 017c  ...|._.|.j...|.|
-00000ff0: 03a1 0201 0064 0053 0072 5300 0000 2903  .....d.S.rS...).
-00001000: 7204 0000 0072 5400 0000 7244 0000 0029  r....rT...rD...)
-00001010: 0572 2200 0000 7256 0000 0072 5700 0000  .r"...rV...rW...
-00001020: 7258 0000 0072 5900 0000 7218 0000 0072  rX...rY...r....r
-00001030: 1800 0000 7219 0000 0072 4400 0000 5a00  ....r....rD...Z.
-00001040: 0000 7304 0000 0008 0712 017a 0f43 7573  ..s........z.Cus
-00001050: 746f 6d4d 6f64 656c 2e66 6974 721f 0000  tomModel.fitr...
-00001060: 0063 0200 0000 0000 0000 0000 0000 0400  .c..............
-00001070: 0000 0300 0000 4300 0000 7320 0000 007c  ......C...s ...|
-00001080: 006a 00a0 017c 01a1 017d 027c 006a 00a0  .j...|...}.|.j..
-00001090: 027c 01a1 017d 037c 027c 0366 0253 0072  .|...}.|.|.f.S.r
-000010a0: 5300 0000 2903 7254 0000 005a 0d70 7265  S...).rT...Z.pre
-000010b0: 6469 6374 5f70 726f 6261 7246 0000 0029  dict_probarF...)
-000010c0: 0472 2200 0000 721f 0000 00da 1070 7265  .r"...r......pre
-000010d0: 6469 6374 6564 5f70 726f 6261 73da 1170  dicted_probas..p
-000010e0: 7265 6469 6374 6564 5f63 6c61 7373 6573  redicted_classes
-000010f0: 7218 0000 0072 1800 0000 7219 0000 0072  r....r....r....r
-00001100: 4600 0000 6400 0000 7306 0000 000c 010c  F...d...s.......
-00001110: 0108 017a 1343 7573 746f 6d4d 6f64 656c  ...z.CustomModel
-00001120: 2e70 7265 6469 6374 290c 722f 0000 0072  .predict).r/...r
-00001130: 3000 0000 7231 0000 0072 5500 0000 722a  0...r1...rU...r*
-00001140: 0000 0072 3200 0000 722b 0000 0072 4400  ...r2...r+...rD.
-00001150: 0000 7203 0000 0072 0e00 0000 720d 0000  ..r....r....r...
-00001160: 0072 4600 0000 7218 0000 0072 1800 0000  .rF...r....r....
-00001170: 7218 0000 0072 1900 0000 7252 0000 0056  r....r....rR...V
-00001180: 0000 0073 1c00 0000 0800 0801 0203 0402  ...s............
-00001190: 02fe 0403 02fd 0404 02fc 0405 02fb 0206  ................
-000011a0: 0afa 200a 7252 0000 0063 0000 0000 0000  .. .rR...c......
-000011b0: 0000 0000 0000 0d00 0000 0a00 0000 4300  ..............C.
-000011c0: 0000 73b4 0200 0074 0083 007d 0074 0183  ..s....t...}.t..
-000011d0: 007d 0164 017c 015f 0264 027c 015f 0364  .}.d.|._.d.|._.d
-000011e0: 037c 015f 0447 0064 0464 0584 0064 0574  .|._.G.d.d...d.t
-000011f0: 0583 037d 027c 0283 007d 0374 0664 0664  ...}.|...}.t.d.d
-00001200: 077c 007c 017c 0364 088d 057d 0474 07a0  .|.|.|.d...}.t..
-00001210: 0864 0964 0a84 0074 0964 0183 0144 0083  .d.d...t.d...D..
-00001220: 0164 0b64 0a84 0074 0964 0183 0144 0083  .d.d...t.d...D..
-00001230: 0164 0c64 0a84 0074 0964 0183 0144 0083  .d.d...t.d...D..
-00001240: 0164 0d64 0a84 0074 0964 0183 0144 0083  .d.d...t.d...D..
-00001250: 0164 0e64 0a84 0074 0964 0183 0144 0083  .d.d...t.d...D..
-00001260: 0164 0f64 0a84 0074 0964 0183 0144 0083  .d.d...t.d...D..
-00001270: 0164 109c 06a1 017d 0574 07a0 0a67 0064  .d.....}.t...g.d
-00001280: 11a2 01a1 017d 0674 07a0 0864 1264 0a84  .....}.t...d.d..
-00001290: 0074 0964 0183 0144 0083 0164 1364 0a84  .t.d...D...d.d..
-000012a0: 0074 0964 0183 0144 0083 0164 1464 0a84  .t.d...D...d.d..
-000012b0: 0074 0964 0183 0144 0083 0164 1564 0a84  .t.d...D...d.d..
-000012c0: 0074 0964 0183 0144 0083 0164 1664 0a84  .t.d...D...d.d..
-000012d0: 0074 0964 0183 0144 0083 0164 1764 0a84  .t.d...D...d.d..
-000012e0: 0074 0964 0183 0144 0083 0164 109c 06a1  .t.d...D...d....
-000012f0: 017d 077c 067c 0564 073c 007c 04a0 0b7c  .}.|.|.d.<.|...|
-00001300: 0564 07a1 0201 007c 04a0 0c7c 07a1 015c  .d.....|...|...\
-00001310: 027d 087d 0974 0d6a 0e7d 0a74 0f7c 087c  .}.}.t.j.}.t.|.|
-00001320: 0a83 027d 0b7c 0b73 f864 1864 1974 10a0  ...}.|.s.d.d.t..
-00001330: 11a1 0076 0073 bd74 12a0 1374 0fa1 0172  ...v.s.t...t...r
-00001340: c274 12a0 1474 0fa1 016e 0164 1964 1a74  .t...t...n.d.d.t
-00001350: 10a0 11a1 0076 0073 ce74 12a0 137c 08a1  .....v.s.t...|..
-00001360: 0172 d374 12a0 147c 08a1 016e 0164 1a64  .r.t...|...n.d.d
-00001370: 1b74 10a0 11a1 0076 0073 df74 12a0 1374  .t.....v.s.t...t
-00001380: 0da1 0172 e474 12a0 1474 0da1 016e 0164  ...r.t...t...n.d
-00001390: 1b74 12a0 147c 0aa1 0174 12a0 147c 0ba1  .t...|...t...|..
-000013a0: 0164 1c9c 0516 007d 0c74 1574 12a0 167c  .d.....}.t.t...|
-000013b0: 0ca1 0183 0182 0164 0004 007d 0a7d 0b74  .......d...}.}.t
-000013c0: 0d6a 0e7d 0a74 0f7c 097c 0a83 027d 0b7c  .j.}.t.|.|...}.|
-000013d0: 0b90 0173 5464 1864 1974 10a0 11a1 0076  ...sTd.d.t.....v
-000013e0: 0090 0173 1574 12a0 1374 0fa1 0190 0172  ...s.t...t.....r
-000013f0: 1a74 12a0 1474 0fa1 016e 0164 1964 1d74  .t...t...n.d.d.t
-00001400: 10a0 11a1 0076 0090 0173 2874 12a0 137c  .....v...s(t...|
-00001410: 09a1 0190 0172 2d74 12a0 147c 09a1 016e  .....r-t...|...n
-00001420: 0164 1d64 1b74 10a0 11a1 0076 0090 0173  .d.d.t.....v...s
-00001430: 3b74 12a0 1374 0da1 0190 0172 4074 12a0  ;t...t.....r@t..
-00001440: 1474 0da1 016e 0164 1b74 12a0 147c 0aa1  .t...n.d.t...|..
-00001450: 0174 12a0 147c 0ba1 0164 1c9c 0516 007d  .t...|...d.....}
-00001460: 0c74 1574 12a0 167c 0ca1 0183 0182 0164  .t.t...|.......d
-00001470: 0004 007d 0a7d 0b64 0053 0029 1e4e 721e  ...}.}.d.S.).Nr.
-00001480: 0000 0054 7220 0000 0063 0000 0000 0000  ...Tr ...c......
-00001490: 0000 0000 0000 0000 0000 0c00 0000 0000  ................
-000014a0: 0000 7386 0000 0065 005a 0164 005a 0264  ..s....e.Z.d.Z.d
-000014b0: 0f64 0265 0366 0287 0066 0164 0364 0484  .d.e.f...f.d.d..
-000014c0: 0d5a 0464 0565 056a 0664 0665 056a 0764  .Z.d.e.j.d.e.j.d
-000014d0: 0765 0865 056a 0665 0965 056a 0719 0066  .e.e.j.e.e.j...f
-000014e0: 0219 0066 0664 0864 0984 045a 0a09 0a09  ...f.d.d...Z....
-000014f0: 0b64 1064 0565 056a 0664 0665 0965 056a  .d.d.e.j.d.e.e.j
-00001500: 0719 0064 0c65 0b64 0765 0865 056a 0665  ...d.e.d.e.e.j.e
-00001510: 0965 056a 0719 0066 0219 0066 0864 0d64  .e.j...f...f.d.d
-00001520: 0e84 055a 0c87 0004 005a 0d53 0029 117a  ...Z.....Z.S.).z
-00001530: 3674 6573 745f 626c 7565 6361 7374 5f77  6test_bluecast_w
-00001540: 6974 685f 6375 7374 6f6d 5f6d 6f64 656c  ith_custom_model
-00001550: 2e3c 6c6f 6361 6c73 3e2e 5246 4543 5653  .<locals>.RFECVS
-00001560: 656c 6563 746f 7272 0100 0000 7214 0000  electorr....r...
-00001570: 0063 0200 0000 0000 0000 0000 0000 0200  .c..............
-00001580: 0000 0800 0000 1300 0000 7342 0000 0074  ..........sB...t
-00001590: 0083 00a0 01a1 0001 0064 007c 005f 027c  .........d.|._.|
-000015a0: 017c 005f 0374 0474 05a0 06a1 0064 0174  .|._.t.t.....d.t
-000015b0: 0764 027c 0164 0364 048d 0364 0174 0874  .d.|.d.d...d.t.t
-000015c0: 0983 0164 0264 058d 067c 005f 0a64 0053  ...d.d...|._.d.S
-000015d0: 0029 064e 721b 0000 0072 2000 0000 5429  .).Nr....r ...T)
-000015e0: 0272 1400 0000 da07 7368 7566 666c 6529  .r......shuffle)
-000015f0: 065a 0965 7374 696d 6174 6f72 da04 7374  .Z.estimator..st
-00001600: 6570 5a02 6376 5a16 6d69 6e5f 6665 6174  epZ.cvZ.min_feat
-00001610: 7572 6573 5f74 6f5f 7365 6c65 6374 5a07  ures_to_selectZ.
-00001620: 7363 6f72 696e 675a 066e 5f6a 6f62 7329  scoringZ.n_jobs)
-00001630: 0bda 0573 7570 6572 7255 0000 00da 1173  ...superrU.....s
-00001640: 656c 6563 7465 645f 6665 6174 7572 6573  elected_features
-00001650: 7214 0000 0072 0500 0000 da03 7867 625a  r....r......xgbZ
-00001660: 0d58 4742 436c 6173 7369 6669 6572 7208  .XGBClassifierr.
-00001670: 0000 0072 0600 0000 7207 0000 00da 1273  ...r....r......s
-00001680: 656c 6563 7469 6f6e 5f73 7472 6174 6567  election_strateg
-00001690: 7929 0272 2200 0000 7214 0000 00a9 01da  y).r"...r.......
-000016a0: 095f 5f63 6c61 7373 5f5f 7218 0000 0072  .__class__r....r
-000016b0: 1900 0000 7255 0000 0074 0000 0073 1600  ....rU...t...s..
-000016c0: 0000 0a01 0601 0601 0201 0601 0201 0c01  ................
-000016d0: 0201 0601 0201 0cfa 7a3f 7465 7374 5f62  ........z?test_b
-000016e0: 6c75 6563 6173 745f 7769 7468 5f63 7573  luecast_with_cus
-000016f0: 746f 6d5f 6d6f 6465 6c2e 3c6c 6f63 616c  tom_model.<local
-00001700: 733e 2e52 4645 4356 5365 6c65 6374 6f72  s>.RFECVSelector
-00001710: 2e5f 5f69 6e69 745f 5f72 1f00 0000 7224  .__init__r....r$
-00001720: 0000 0072 1200 0000 6303 0000 0000 0000  ...r....c.......
-00001730: 0000 0000 0003 0000 0004 0000 0053 0000  .............S..
-00001740: 0073 3400 0000 7c00 6a00 a001 7c01 7c02  .s4...|.j...|.|.
-00001750: a102 0100 7c00 6a00 6a02 7c00 5f03 7c01  ....|.j.j.|._.|.
-00001760: 6a04 6400 6400 8502 7c00 6a03 6602 1900  j.d.d...|.j.f...
-00001770: 7d01 7c01 7c02 6602 5300 7253 0000 0029  }.|.|.f.S.rS...)
-00001780: 0572 6100 0000 7244 0000 005a 0873 7570  .ra...rD...Z.sup
-00001790: 706f 7274 5f72 5f00 0000 da03 6c6f 6372  port_r_.....locr
-000017a0: 2600 0000 7218 0000 0072 1800 0000 7219  &...r....r....r.
-000017b0: 0000 0072 2700 0000 8100 0000 7308 0000  ...r'.......s...
-000017c0: 000e 030a 0114 0108 017a 4474 6573 745f  .........zDtest_
-000017d0: 626c 7565 6361 7374 5f77 6974 685f 6375  bluecast_with_cu
-000017e0: 7374 6f6d 5f6d 6f64 656c 2e3c 6c6f 6361  stom_model.<loca
-000017f0: 6c73 3e2e 5246 4543 5653 656c 6563 746f  ls>.RFECVSelecto
-00001800: 722e 6669 745f 7472 616e 7366 6f72 6d4e  r.fit_transformN
-00001810: 4672 2800 0000 6304 0000 0000 0000 0000  Fr(...c.........
-00001820: 0000 0004 0000 0003 0000 0053 0000 0073  ...........S...s
-00001830: 1c00 0000 7c01 6a00 6400 6400 8502 7c00  ....|.j.d.d...|.
-00001840: 6a01 6602 1900 7d01 7c01 7c02 6602 5300  j.f...}.|.|.f.S.
-00001850: 7253 0000 0029 0272 6400 0000 725f 0000  rS...).rd...r_..
-00001860: 0072 2c00 0000 7218 0000 0072 1800 0000  .r,...r....r....
-00001870: 7219 0000 0072 2d00 0000 8900 0000 7304  r....r-.......s.
-00001880: 0000 0014 0608 017a 4074 6573 745f 626c  .......z@test_bl
-00001890: 7565 6361 7374 5f77 6974 685f 6375 7374  uecast_with_cust
-000018a0: 6f6d 5f6d 6f64 656c 2e3c 6c6f 6361 6c73  om_model.<locals
-000018b0: 3e2e 5246 4543 5653 656c 6563 746f 722e  >.RFECVSelector.
-000018c0: 7472 616e 7366 6f72 6d29 0172 0100 0000  transform).r....
-000018d0: 722e 0000 0029 0e72 2f00 0000 7230 0000  r....).r/...r0..
-000018e0: 0072 3100 0000 da03 696e 7472 5500 0000  .r1.....intrU...
-000018f0: 722a 0000 0072 3200 0000 722b 0000 0072  r*...r2...r+...r
-00001900: 0300 0000 7202 0000 0072 2700 0000 7233  ....r....r'...r3
-00001910: 0000 0072 2d00 0000 da0d 5f5f 636c 6173  ...r-.....__clas
-00001920: 7363 656c 6c5f 5f72 1800 0000 7218 0000  scell__r....r...
-00001930: 0072 6200 0000 7219 0000 00da 0d52 4645  .rb...r......RFE
-00001940: 4356 5365 6c65 6374 6f72 7300 0000 7328  CVSelectors...s(
-00001950: 0000 0008 0014 0102 0d04 0102 ff04 0102  ................
-00001960: ff12 020a fe02 0b02 0104 fc04 0202 fe08  ................
-00001970: 0302 fd02 0402 fc12 0512 fb72 6700 0000  ...........rg...
-00001980: 7235 0000 0072 2400 0000 2905 7236 0000  r5...r$...).r6..
-00001990: 0072 3700 0000 5a08 6d6c 5f6d 6f64 656c  .r7...Z.ml_model
-000019a0: 7238 0000 00da 1763 7573 746f 6d5f 6665  r8.....custom_fe
-000019b0: 6174 7572 655f 7365 6c65 6374 6f72 6301  ature_selectorc.
-000019c0: 0000 0000 0000 0000 0000 0002 0000 0003  ................
-000019d0: 0000 0053 0000 00f3 1000 0000 6700 7c00  ...S........g.|.
-000019e0: 5d04 7d01 7c01 9102 7102 5300 7218 0000  ].}.|...q.S.r...
-000019f0: 0072 1800 0000 a902 da02 2e30 da01 6972  .r.........0..ir
-00001a00: 1800 0000 7218 0000 0072 1900 0000 da0a  ....r....r......
-00001a10: 3c6c 6973 7463 6f6d 703e a000 0000 f302  <listcomp>......
-00001a20: 0000 0010 007a 3374 6573 745f 626c 7565  .....z3test_blue
-00001a30: 6361 7374 5f77 6974 685f 6375 7374 6f6d  cast_with_custom
-00001a40: 5f6d 6f64 656c 2e3c 6c6f 6361 6c73 3e2e  _model.<locals>.
-00001a50: 3c6c 6973 7463 6f6d 703e 6301 0000 0000  <listcomp>c.....
-00001a60: 0000 0000 0000 0002 0000 0003 0000 0053  ...............S
-00001a70: 0000 0072 6900 0000 7218 0000 0072 1800  ...ri...r....r..
-00001a80: 0000 726a 0000 0072 1800 0000 7218 0000  ..rj...r....r...
-00001a90: 0072 1900 0000 726d 0000 00a1 0000 0072  .r....rm.......r
-00001aa0: 6e00 0000 6301 0000 0000 0000 0000 0000  n...c...........
-00001ab0: 0002 0000 0003 0000 0053 0000 0072 6900  .........S...ri.
-00001ac0: 0000 7218 0000 0072 1800 0000 726a 0000  ..r....r....rj..
-00001ad0: 0072 1800 0000 7218 0000 0072 1900 0000  .r....r....r....
-00001ae0: 726d 0000 00a2 0000 0072 6e00 0000 6301  rm.......rn...c.
-00001af0: 0000 0000 0000 0000 0000 0002 0000 0003  ................
-00001b00: 0000 0053 0000 0072 6900 0000 7218 0000  ...S...ri...r...
-00001b10: 0072 1800 0000 726a 0000 0072 1800 0000  .r....rj...r....
-00001b20: 7218 0000 0072 1900 0000 726d 0000 00a3  r....r....rm....
-00001b30: 0000 0072 6e00 0000 6301 0000 0000 0000  ...rn...c.......
-00001b40: 0000 0000 0002 0000 0003 0000 0053 0000  .............S..
-00001b50: 0072 6900 0000 7218 0000 0072 1800 0000  .ri...r....r....
-00001b60: 726a 0000 0072 1800 0000 7218 0000 0072  rj...r....r....r
-00001b70: 1900 0000 726d 0000 00a4 0000 0072 6e00  ....rm.......rn.
-00001b80: 0000 6301 0000 0000 0000 0000 0000 0002  ..c.............
-00001b90: 0000 0003 0000 0053 0000 0072 6900 0000  .......S...ri...
-00001ba0: 7218 0000 0072 1800 0000 726a 0000 0072  r....r....rj...r
-00001bb0: 1800 0000 7218 0000 0072 1900 0000 726d  ....r....r....rm
-00001bc0: 0000 00a5 0000 0072 6e00 0000 2906 5a08  .......rn...).Z.
-00001bd0: 6665 6174 7572 6531 5a08 6665 6174 7572  feature1Z.featur
-00001be0: 6532 5a08 6665 6174 7572 6533 5a08 6665  e2Z.feature3Z.fe
-00001bf0: 6174 7572 6534 5a08 6665 6174 7572 6535  ature4Z.feature5
-00001c00: 5a08 6665 6174 7572 6536 290a 7201 0000  Z.feature6).r...
-00001c10: 0072 1b00 0000 7201 0000 0072 1b00 0000  .r....r....r....
-00001c20: 7201 0000 0072 1b00 0000 7201 0000 0072  r....r....r....r
-00001c30: 1b00 0000 7201 0000 0072 1b00 0000 6301  ....r....r....c.
-00001c40: 0000 0000 0000 0000 0000 0002 0000 0003  ................
-00001c50: 0000 0053 0000 0072 6900 0000 7218 0000  ...S...ri...r...
-00001c60: 0072 1800 0000 726a 0000 0072 1800 0000  .r....rj...r....
-00001c70: 7218 0000 0072 1900 0000 726d 0000 00ab  r....r....rm....
-00001c80: 0000 0072 6e00 0000 6301 0000 0000 0000  ...rn...c.......
-00001c90: 0000 0000 0002 0000 0003 0000 0053 0000  .............S..
-00001ca0: 0072 6900 0000 7218 0000 0072 1800 0000  .ri...r....r....
-00001cb0: 726a 0000 0072 1800 0000 7218 0000 0072  rj...r....r....r
-00001cc0: 1900 0000 726d 0000 00ac 0000 0072 6e00  ....rm.......rn.
-00001cd0: 0000 6301 0000 0000 0000 0000 0000 0002  ..c.............
-00001ce0: 0000 0003 0000 0053 0000 0072 6900 0000  .......S...ri...
-00001cf0: 7218 0000 0072 1800 0000 726a 0000 0072  r....r....rj...r
-00001d00: 1800 0000 7218 0000 0072 1900 0000 726d  ....r....r....rm
-00001d10: 0000 00ad 0000 0072 6e00 0000 6301 0000  .......rn...c...
-00001d20: 0000 0000 0000 0000 0002 0000 0003 0000  ................
-00001d30: 0053 0000 0072 6900 0000 7218 0000 0072  .S...ri...r....r
-00001d40: 1800 0000 726a 0000 0072 1800 0000 7218  ....rj...r....r.
-00001d50: 0000 0072 1900 0000 726d 0000 00ae 0000  ...r....rm......
-00001d60: 0072 6e00 0000 6301 0000 0000 0000 0000  .rn...c.........
-00001d70: 0000 0002 0000 0003 0000 0053 0000 0072  ...........S...r
-00001d80: 6900 0000 7218 0000 0072 1800 0000 726a  i...r....r....rj
-00001d90: 0000 0072 1800 0000 7218 0000 0072 1900  ...r....r....r..
-00001da0: 0000 726d 0000 00af 0000 0072 6e00 0000  ..rm.......rn...
-00001db0: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
-00001dc0: 0003 0000 0053 0000 0072 6900 0000 7218  .....S...ri...r.
-00001dd0: 0000 0072 1800 0000 726a 0000 0072 1800  ...r....rj...r..
-00001de0: 0000 7218 0000 0072 1900 0000 726d 0000  ..r....r....rm..
-00001df0: 00b0 0000 0072 6e00 0000 7a52 6173 7365  .....rn...zRasse
-00001e00: 7274 2025 2870 7936 2973 0a7b 2528 7079  rt %(py6)s.{%(py
-00001e10: 3629 7320 3d20 2528 7079 3029 7328 2528  6)s = %(py0)s(%(
-00001e20: 7079 3129 732c 2025 2870 7934 2973 0a7b  py1)s, %(py4)s.{
-00001e30: 2528 7079 3429 7320 3d20 2528 7079 3229  %(py4)s = %(py2)
-00001e40: 732e 6e64 6172 7261 790a 7d29 0a7d 7229  s.ndarray.}).}r)
-00001e50: 0000 0072 5a00 0000 da02 6e70 2905 723d  ...rZ.....np).r=
-00001e60: 0000 0072 3e00 0000 5a03 7079 325a 0370  ...r>...Z.py2Z.p
-00001e70: 7934 723f 0000 0072 5b00 0000 2917 7252  y4r?...r[...).rR
-00001e80: 0000 0072 0a00 0000 7241 0000 0072 4200  ...r....rA...rB.
-00001e90: 0000 7243 0000 0072 0f00 0000 7209 0000  ..rC...r....r...
-00001ea0: 0072 2a00 0000 7232 0000 00da 0572 616e  .r*...r2.....ran
-00001eb0: 6765 722b 0000 0072 4400 0000 7246 0000  ger+...rD...rF..
-00001ec0: 0072 6f00 0000 da07 6e64 6172 7261 7972  .ro.....ndarrayr
-00001ed0: 2900 0000 724a 0000 0072 4b00 0000 7248  )...rJ...rK...rH
-00001ee0: 0000 0072 4c00 0000 724d 0000 0072 4e00  ...rL...rM...rN.
-00001ef0: 0000 724f 0000 0029 0d5a 0c63 7573 746f  ..rO...).Z.custo
-00001f00: 6d5f 6d6f 6465 6c72 5000 0000 7267 0000  m_modelrP...rg..
-00001f10: 0072 6800 0000 da08 626c 7565 6361 7374  .rh.....bluecast
-00001f20: 7256 0000 0072 5800 0000 7257 0000 0072  rV...rX...rW...r
-00001f30: 5a00 0000 725b 0000 005a 0b40 7079 5f61  Z...r[...Z.@py_a
-00001f40: 7373 6572 7433 5a0b 4070 795f 6173 7365  ssert3Z.@py_asse
-00001f50: 7274 355a 0b40 7079 5f66 6f72 6d61 7437  rt5Z.@py_format7
-00001f60: 7218 0000 0072 1800 0000 7219 0000 00da  r....r....r.....
-00001f70: 1f74 6573 745f 626c 7565 6361 7374 5f77  .test_bluecast_w
-00001f80: 6974 685f 6375 7374 6f6d 5f6d 6f64 656c  ith_custom_model
-00001f90: 6a00 0000 734c 0000 0006 0206 0106 0106  j...sL..........
-00001fa0: 0106 0110 0306 1f02 0302 0102 0102 0102  ................
-00001fb0: 0102 0106 fb04 0910 0210 0110 0110 0110  ................
-00001fc0: 0110 0104 fa04 ff0e 0a04 0110 0210 0110  ................
-00001fd0: 0110 0110 0110 0104 fa04 ff08 0b0c 030e  ................
-00001fe0: 03aa 03bc 0172 7300 0000 292c da08 6275  .....rs...),..bu
-00001ff0: 696c 7469 6e73 724a 0000 00da 195f 7079  iltinsrJ....._py
-00002000: 7465 7374 2e61 7373 6572 7469 6f6e 2e72  test.assertion.r
-00002010: 6577 7269 7465 da09 6173 7365 7274 696f  ewrite..assertio
-00002020: 6eda 0772 6577 7269 7465 7248 0000 00da  n..rewriterH....
-00002030: 0674 7970 696e 6772 0200 0000 7203 0000  .typingr....r...
-00002040: 00da 056e 756d 7079 726f 0000 005a 0670  ...numpyro...Z.p
-00002050: 616e 6461 7372 2a00 0000 da06 7079 7465  andasr*.....pyte
-00002060: 7374 5a07 7867 626f 6f73 7472 6000 0000  stZ.xgboostr`...
-00002070: 5a10 736b 6c65 6172 6e2e 656e 7365 6d62  Z.sklearn.ensemb
-00002080: 6c65 7204 0000 005a 1973 6b6c 6561 726e  ler....Z.sklearn
-00002090: 2e66 6561 7475 7265 5f73 656c 6563 7469  .feature_selecti
-000020a0: 6f6e 7205 0000 005a 0f73 6b6c 6561 726e  onr....Z.sklearn
-000020b0: 2e6d 6574 7269 6373 7206 0000 0072 0700  .metricsr....r..
-000020c0: 0000 5a17 736b 6c65 6172 6e2e 6d6f 6465  ..Z.sklearn.mode
-000020d0: 6c5f 7365 6c65 6374 696f 6e72 0800 0000  l_selectionr....
-000020e0: 5a18 626c 7565 6361 7374 2e62 6c75 6570  Z.bluecast.bluep
-000020f0: 7269 6e74 732e 6361 7374 7209 0000 005a  rints.castr....Z
-00002100: 1f62 6c75 6563 6173 742e 636f 6e66 6967  .bluecast.config
-00002110: 2e74 7261 696e 696e 675f 636f 6e66 6967  .training_config
-00002120: 720a 0000 0072 0b00 0000 5a22 626c 7565  r....r....Z"blue
-00002130: 6361 7374 2e6d 6c5f 6d6f 6465 6c6c 696e  cast.ml_modellin
-00002140: 672e 6261 7365 5f63 6c61 7373 6573 720c  g.base_classesr.
-00002150: 0000 0072 0d00 0000 720e 0000 005a 1d62  ...r....r....Z.b
-00002160: 6c75 6563 6173 742e 7072 6570 726f 6365  luecast.preproce
-00002170: 7373 696e 672e 6375 7374 6f6d 720f 0000  ssing.customr...
-00002180: 005a 2462 6c75 6563 6173 742e 7465 7374  .Z$bluecast.test
-00002190: 732e 6d61 6b65 5f64 6174 612e 6372 6561  s.make_data.crea
-000021a0: 7465 5f64 6174 6172 1100 0000 da07 6669  te_datar......fi
-000021b0: 7874 7572 6572 3200 0000 721a 0000 0072  xturer2...r....r
-000021c0: 5100 0000 7252 0000 0072 7300 0000 7218  Q...rR...rs...r.
-000021d0: 0000 0072 1800 0000 7218 0000 0072 1900  ...r....r....r..
-000021e0: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
-000021f0: 7326 0000 002a 0008 0208 0108 0108 010c  s&...*..........
-00002200: 010c 0110 010c 010c 0210 0114 010c 050c  ................
-00002210: 0104 031c 0108 0610 380c 14              ........8..
+000003c0: 0b8d 057d 077c 076a 097c 017c 016a 0a64  ...}.|.j.|.|.j.d
+000003d0: 0a64 0264 0c8d 027c 0164 0a19 0064 0a64  .d.d...|.d...d.d
+000003e0: 0d8d 0401 0074 0b64 0e83 0101 007c 07a0  .....t.d.....|..
+000003f0: 0c7c 026a 0a64 0a64 0264 0c8d 02a1 015c  .|.j.d.d.d.....\
+00000400: 027d 087d 0974 0b64 0f83 0101 0074 0d7c  .}.}.t.d.....t.|
+00000410: 0883 017d 0a7c 026a 0e7d 0b74 0d7c 0b83  ...}.|.j.}.t.|..
+00000420: 017d 0c7c 0a7c 0c6b 027d 0d7c 0d73 d174  .}.|.|.k.}.|.s.t
+00000430: 0fa0 1064 107c 0d66 0164 117c 0a7c 0c66  ...d.|.f.d.|.|.f
+00000440: 02a1 0464 1274 11a0 12a1 0076 0073 7b74  ...d.t.....v.s{t
+00000450: 0fa0 1374 0da1 0172 8074 0fa0 1474 0da1  ...t...r.t...t..
+00000460: 016e 0164 1264 1374 11a0 12a1 0076 0073  .n.d.d.t.....v.s
+00000470: 8c74 0fa0 137c 08a1 0172 9174 0fa0 147c  .t...|...r.t...|
+00000480: 08a1 016e 0164 1374 0fa0 147c 0aa1 0164  ...n.d.t...|...d
+00000490: 1274 11a0 12a1 0076 0073 a174 0fa0 1374  .t.....v.s.t...t
+000004a0: 0da1 0172 a674 0fa0 1474 0da1 016e 0164  ...r.t...t...n.d
+000004b0: 1264 1474 11a0 12a1 0076 0073 b274 0fa0  .d.t.....v.s.t..
+000004c0: 137c 02a1 0172 b774 0fa0 147c 02a1 016e  .|...r.t...|...n
+000004d0: 0164 1474 0fa0 147c 0ba1 0174 0fa0 147c  .d.t...|...t...|
+000004e0: 0ca1 0164 159c 0716 007d 0e64 1664 177c  ...d.....}.d.d.|
+000004f0: 0e69 0116 007d 0f74 1574 0fa0 167c 0fa1  .i...}.t.t...|..
+00000500: 0183 0182 0164 1804 007d 0a04 007d 0d04  .....d...}...}..
+00000510: 007d 0b7d 0c74 0d7c 0983 017d 0a7c 026a  .}.}.t.|...}.|.j
+00000520: 0e7d 0b74 0d7c 0b83 017d 0c7c 0a7c 0c6b  .}.t.|...}.|.|.k
+00000530: 027d 0d7c 0d90 0173 5e74 0fa0 1064 107c  .}.|...s^t...d.|
+00000540: 0d66 0164 117c 0a7c 0c66 02a1 0464 1274  .f.d.|.|.f...d.t
+00000550: 11a0 12a1 0076 0090 0173 0274 0fa0 1374  .....v...s.t...t
+00000560: 0da1 0190 0172 0774 0fa0 1474 0da1 016e  .....r.t...t...n
+00000570: 0164 1264 1974 11a0 12a1 0076 0090 0173  .d.d.t.....v...s
+00000580: 1574 0fa0 137c 09a1 0190 0172 1a74 0fa0  .t...|.....r.t..
+00000590: 147c 09a1 016e 0164 1974 0fa0 147c 0aa1  .|...n.d.t...|..
+000005a0: 0164 1274 11a0 12a1 0076 0090 0173 2c74  .d.t.....v...s,t
+000005b0: 0fa0 1374 0da1 0190 0172 3174 0fa0 1474  ...t.....r1t...t
+000005c0: 0da1 016e 0164 1264 1474 11a0 12a1 0076  ...n.d.d.t.....v
+000005d0: 0090 0173 3f74 0fa0 137c 02a1 0190 0172  ...s?t...|.....r
+000005e0: 4474 0fa0 147c 02a1 016e 0164 1474 0fa0  Dt...|...n.d.t..
+000005f0: 147c 0ba1 0174 0fa0 147c 0ca1 0164 159c  .|...t...|...d..
+00000600: 0716 007d 0e64 1664 177c 0e69 0116 007d  ...}.d.d.|.i...}
+00000610: 0f74 1574 0fa0 167c 0fa1 0183 0182 0164  .t.t...|.......d
+00000620: 1804 007d 0a04 007d 0d04 007d 0b7d 0c64  ...}...}...}.}.d
+00000630: 1853 0029 1a7a 2254 6573 7420 7468 6174  .S.).z"Test that
+00000640: 2074 6573 7473 2074 6865 2042 6c75 6543   tests the BlueC
+00000650: 6173 7420 636c 6173 7372 0100 0000 e901  ast classr......
+00000660: 0000 00e9 6400 0000 e910 0000 00e9 0a00  ....d...........
+00000670: 0000 4663 0000 0000 0000 0000 0000 0000  ..Fc............
+00000680: 0000 0000 0c00 0000 4000 0000 7380 0000  ........@...s...
+00000690: 0065 005a 0164 005a 0264 0165 036a 0464  .e.Z.d.Z.d.e.j.d
+000006a0: 0265 036a 0466 0464 0364 0484 045a 0564  .e.j.f.d.d...Z.d
+000006b0: 0165 036a 0464 0565 036a 0664 0265 0765  .e.j.d.e.j.d.e.e
+000006c0: 036a 0465 036a 0666 0219 0066 0664 0664  .j.e.j.f...f.d.d
+000006d0: 0784 045a 0809 0809 0964 0d64 0165 036a  ...Z.....d.d.e.j
+000006e0: 0464 0565 0965 036a 0619 0064 0a65 0a64  .d.e.e.j...d.e.d
+000006f0: 0265 0765 036a 0465 0965 036a 0619 0066  .e.e.j.e.e.j...f
+00000700: 0219 0066 0864 0b64 0c84 055a 0b64 0853  ...f.d.d...Z.d.S
+00000710: 0029 0e7a 3d74 6573 745f 626c 7565 7072  .).z=test_bluepr
+00000720: 696e 745f 7867 626f 6f73 742e 3c6c 6f63  int_xgboost.<loc
+00000730: 616c 733e 2e4d 7943 7573 746f 6d4c 6173  als>.MyCustomLas
+00000740: 744d 696c 6550 7265 7072 6f63 6573 7369  tMilePreprocessi
+00000750: 6e67 da02 6466 7212 0000 0063 0200 0000  ng..dfr....c....
+00000760: 0000 0000 0000 0000 0200 0000 0300 0000  ................
+00000770: 5300 0000 730c 0000 0064 017c 0164 023c  S...s....d.|.d.<
+00000780: 007c 0153 0029 034e e905 0000 005a 0a63  .|.S.).N.....Z.c
+00000790: 7573 746f 6d5f 636f 6c72 1800 0000 2902  ustom_colr....).
+000007a0: da04 7365 6c66 721f 0000 0072 1800 0000  ..selfr....r....
+000007b0: 7218 0000 0072 1900 0000 da0f 6375 7374  r....r......cust
+000007c0: 6f6d 5f66 756e 6374 696f 6e2c 0000 0073  om_function,...s
+000007d0: 0400 0000 0801 0401 7a4d 7465 7374 5f62  ........zMtest_b
+000007e0: 6c75 6570 7269 6e74 5f78 6762 6f6f 7374  lueprint_xgboost
+000007f0: 2e3c 6c6f 6361 6c73 3e2e 4d79 4375 7374  .<locals>.MyCust
+00000800: 6f6d 4c61 7374 4d69 6c65 5072 6570 726f  omLastMilePrepro
+00000810: 6365 7373 696e 672e 6375 7374 6f6d 5f66  cessing.custom_f
+00000820: 756e 6374 696f 6eda 0674 6172 6765 7463  unction..targetc
+00000830: 0300 0000 0000 0000 0000 0000 0300 0000  ................
+00000840: 0300 0000 5300 0000 7326 0000 007c 00a0  ....S...s&...|..
+00000850: 007c 01a1 017d 017c 01a0 0164 01a1 017d  .|...}.|...d...}
+00000860: 017c 02a0 0164 01a1 017d 027c 017c 0266  .|...d...}.|.|.f
+00000870: 0253 0029 024e 69e8 0300 0029 0272 2200  .S.).Ni....).r".
+00000880: 0000 da04 6865 6164 a903 7221 0000 0072  ....head..r!...r
+00000890: 1f00 0000 7223 0000 0072 1800 0000 7218  ....r#...r....r.
+000008a0: 0000 0072 1900 0000 da0d 6669 745f 7472  ...r......fit_tr
+000008b0: 616e 7366 6f72 6d30 0000 0073 0800 0000  ansform0...s....
+000008c0: 0a03 0a01 0a01 0801 7a4b 7465 7374 5f62  ........zKtest_b
+000008d0: 6c75 6570 7269 6e74 5f78 6762 6f6f 7374  lueprint_xgboost
+000008e0: 2e3c 6c6f 6361 6c73 3e2e 4d79 4375 7374  .<locals>.MyCust
+000008f0: 6f6d 4c61 7374 4d69 6c65 5072 6570 726f  omLastMilePrepro
+00000900: 6365 7373 696e 672e 6669 745f 7472 616e  cessing.fit_tran
+00000910: 7366 6f72 6d4e 46da 0e70 7265 6469 6374  sformNF..predict
+00000920: 6f6e 5f6d 6f64 6563 0400 0000 0000 0000  on_modec........
+00000930: 0000 0000 0400 0000 0300 0000 5300 0000  ............S...
+00000940: 7336 0000 007c 00a0 007c 01a1 017d 017c  s6...|...|...}.|
+00000950: 0373 1774 017c 0274 026a 0383 0272 177c  .s.t.|.t.j...r.|
+00000960: 01a0 0464 01a1 017d 017c 02a0 0464 01a1  ...d...}.|...d..
+00000970: 017d 027c 017c 0266 0253 0029 024e 721c  .}.|.|.f.S.).Nr.
+00000980: 0000 0029 0572 2200 0000 da0a 6973 696e  ...).r".....isin
+00000990: 7374 616e 6365 da02 7064 da06 5365 7269  stance..pd..Seri
+000009a0: 6573 7224 0000 00a9 0472 2100 0000 721f  esr$.....r!...r.
+000009b0: 0000 0072 2300 0000 7227 0000 0072 1800  ...r#...r'...r..
+000009c0: 0000 7218 0000 0072 1900 0000 da09 7472  ..r....r......tr
+000009d0: 616e 7366 6f72 6d38 0000 0073 0a00 0000  ansform8...s....
+000009e0: 0a06 1001 0a01 0a01 0801 7a47 7465 7374  ..........zGtest
+000009f0: 5f62 6c75 6570 7269 6e74 5f78 6762 6f6f  _blueprint_xgboo
+00000a00: 7374 2e3c 6c6f 6361 6c73 3e2e 4d79 4375  st.<locals>.MyCu
+00000a10: 7374 6f6d 4c61 7374 4d69 6c65 5072 6570  stomLastMilePrep
+00000a20: 726f 6365 7373 696e 672e 7472 616e 7366  rocessing.transf
+00000a30: 6f72 6da9 024e 4629 0cda 085f 5f6e 616d  orm..NF)...__nam
+00000a40: 655f 5fda 0a5f 5f6d 6f64 756c 655f 5fda  e__..__module__.
+00000a50: 0c5f 5f71 7561 6c6e 616d 655f 5f72 2900  .__qualname__r).
+00000a60: 0000 da09 4461 7461 4672 616d 6572 2200  ....DataFramer".
+00000a70: 0000 722a 0000 0072 0300 0000 7226 0000  ..r*...r....r&..
+00000a80: 0072 0200 0000 da04 626f 6f6c 722c 0000  .r......boolr,..
+00000a90: 0072 1800 0000 7218 0000 0072 1800 0000  .r....r....r....
+00000aa0: 7219 0000 00da 1d4d 7943 7573 746f 6d4c  r......MyCustomL
+00000ab0: 6173 744d 696c 6550 7265 7072 6f63 6573  astMilePreproces
+00000ac0: 7369 6e67 2b00 0000 7328 0000 0008 0016  sing+...s(......
+00000ad0: 0102 0404 0102 ff04 0102 ff0e 020a fe02  ................
+00000ae0: 0b02 0104 fc04 0202 fe08 0302 fd02 0402  ................
+00000af0: fc12 050e fb72 3300 0000 da06 6269 6e61  .....r3.....bina
+00000b00: 7279 7223 0000 0029 05da 0d63 6c61 7373  ryr#...)...class
+00000b10: 5f70 726f 626c 656d da0d 7461 7267 6574  _problem..target
+00000b20: 5f63 6f6c 756d 6eda 0d63 6f6e 665f 7472  _column..conf_tr
+00000b30: 6169 6e69 6e67 5a0c 636f 6e66 5f78 6762  ainingZ.conf_xgb
+00000b40: 6f6f 7374 da1c 6375 7374 6f6d 5f6c 6173  oost..custom_las
+00000b50: 745f 6d69 6c65 5f63 6f6d 7075 7461 7469  t_mile_computati
+00000b60: 6f6e 2901 da04 6178 6973 2901 5a0a 7461  on)...axis).Z.ta
+00000b70: 7267 6574 5f63 6f6c 7a16 4175 746f 7475  rget_colz.Autotu
+00000b80: 6e69 6e67 2073 7563 6365 7373 6675 6c2e  ning successful.
+00000b90: 7a16 5072 6564 6963 7469 6e67 2073 7563  z.Predicting suc
+00000ba0: 6365 7373 6675 6c2e 2901 fa02 3d3d 2901  cessful.)...==).
+00000bb0: 7a6b 2528 7079 3329 730a 7b25 2870 7933  zk%(py3)s.{%(py3
+00000bc0: 2973 203d 2025 2870 7930 2973 2825 2870  )s = %(py0)s(%(p
+00000bd0: 7931 2973 290a 7d20 3d3d 2025 2870 7931  y1)s).} == %(py1
+00000be0: 3029 730a 7b25 2870 7931 3029 7320 3d20  0)s.{%(py10)s = 
+00000bf0: 2528 7079 3529 7328 2528 7079 3829 730a  %(py5)s(%(py8)s.
+00000c00: 7b25 2870 7938 2973 203d 2025 2870 7936  {%(py8)s = %(py6
+00000c10: 2973 2e69 6e64 6578 0a7d 290a 7dda 036c  )s.index.}).}..l
+00000c20: 656e da07 795f 7072 6f62 7372 1700 0000  en..y_probsr....
+00000c30: 2907 da03 7079 30da 0370 7931 5a03 7079  )...py0..py1Z.py
+00000c40: 335a 0370 7935 da03 7079 365a 0370 7938  3Z.py5..py6Z.py8
+00000c50: 5a04 7079 3130 7a0f 6173 7365 7274 2025  Z.py10z.assert %
+00000c60: 2870 7931 3229 735a 0470 7931 324e da09  (py12)sZ.py12N..
+00000c70: 795f 636c 6173 7365 7329 1772 0b00 0000  y_classes).r....
+00000c80: 5a09 7374 6570 735f 6d61 785a 0e6e 756d  Z.steps_maxZ.num
+00000c90: 5f6c 6561 7665 735f 6d61 7872 0a00 0000  _leaves_maxr....
+00000ca0: da1c 6879 7065 7270 6172 616d 6574 6572  ..hyperparameter
+00000cb0: 5f74 756e 696e 675f 726f 756e 6473 da18  _tuning_rounds..
+00000cc0: 656e 6162 6c65 5f66 6561 7475 7265 5f73  enable_feature_s
+00000cd0: 656c 6563 7469 6f6e da14 6879 7065 7274  election..hypert
+00000ce0: 756e 696e 675f 6376 5f66 6f6c 6473 720f  uning_cv_foldsr.
+00000cf0: 0000 0072 0900 0000 5a08 6669 745f 6576  ...r....Z.fit_ev
+00000d00: 616c da04 6472 6f70 da05 7072 696e 74da  al..drop..print.
+00000d10: 0770 7265 6469 6374 723b 0000 00da 0569  .predictr;.....i
+00000d20: 6e64 6578 da0a 4070 7974 6573 745f 6172  ndex..@pytest_ar
+00000d30: da11 5f63 616c 6c5f 7265 7072 636f 6d70  .._call_reprcomp
+00000d40: 6172 65da 0c40 7079 5f62 7569 6c74 696e  are..@py_builtin
+00000d50: 73da 066c 6f63 616c 73da 185f 7368 6f75  s..locals.._shou
+00000d60: 6c64 5f72 6570 725f 676c 6f62 616c 5f6e  ld_repr_global_n
+00000d70: 616d 65da 095f 7361 6665 7265 7072 da0e  ame.._saferepr..
+00000d80: 4173 7365 7274 696f 6e45 7272 6f72 da13  AssertionError..
+00000d90: 5f66 6f72 6d61 745f 6578 706c 616e 6174  _format_explanat
+00000da0: 696f 6e29 1072 1a00 0000 7216 0000 0072  ion).r....r....r
+00000db0: 1700 0000 5a14 7867 626f 6f73 745f 7061  ....Z.xgboost_pa
+00000dc0: 7261 6d5f 636f 6e66 6967 da0c 7472 6169  ram_config..trai
+00000dd0: 6e5f 636f 6e66 6967 7233 0000 0072 3800  n_configr3...r8.
+00000de0: 0000 5a06 6175 746f 6d6c 723c 0000 0072  ..Z.automlr<...r
+00000df0: 4000 0000 5a0b 4070 795f 6173 7365 7274  @...Z.@py_assert
+00000e00: 325a 0b40 7079 5f61 7373 6572 7437 5a0b  2Z.@py_assert7Z.
+00000e10: 4070 795f 6173 7365 7274 395a 0b40 7079  @py_assert9Z.@py
+00000e20: 5f61 7373 6572 7434 5a0c 4070 795f 666f  _assert4Z.@py_fo
+00000e30: 726d 6174 3131 5a0c 4070 795f 666f 726d  rmat11Z.@py_form
+00000e40: 6174 3133 7218 0000 0072 1800 0000 7219  at13r....r....r.
+00000e50: 0000 00da 1674 6573 745f 626c 7565 7072  .....test_bluepr
+00000e60: 696e 745f 7867 626f 6f73 741e 0000 0073  int_xgboost....s
+00000e70: 3e00 0000 0802 0801 0601 0601 0601 0601  >...............
+00000e80: 0601 0601 0601 1003 0619 0202 0201 0201  ................
+00000e90: 0201 0201 0201 06fb 0407 0201 0c01 0601  ................
+00000ea0: 0201 06fc 0806 1801 0801 fe01 0a00 fe01  ................
+00000eb0: 2000 7251 0000 0063 0000 0000 0000 0000   .rQ...c........
+00000ec0: 0000 0000 0000 0000 0a00 0000 4000 0000  ............@...
+00000ed0: 7356 0000 0065 005a 0164 005a 0264 0164  sV...e.Z.d.Z.d.d
+00000ee0: 0284 005a 0364 0365 046a 0564 0465 046a  ...Z.d.e.j.d.e.j
+00000ef0: 0564 0565 046a 0664 0665 046a 0664 0764  .d.e.j.d.e.j.d.d
+00000f00: 0866 0a64 0964 0a84 045a 0764 0b65 046a  .f.d.d...Z.d.e.j
+00000f10: 0564 0765 0865 0965 0a66 0219 0066 0464  .d.e.e.e.f...f.d
+00000f20: 0c64 0d84 045a 0b64 0853 0029 0eda 0b43  .d...Z.d.S.)...C
+00000f30: 7573 746f 6d4d 6f64 656c 6301 0000 0000  ustomModelc.....
+00000f40: 0000 0000 0000 0001 0000 0002 0000 0043  ...............C
+00000f50: 0000 0073 0a00 0000 6400 7c00 5f00 6400  ...s....d.|._.d.
+00000f60: 5300 a901 4e29 01da 056d 6f64 656c 2901  S...N)...model).
+00000f70: 7221 0000 0072 1800 0000 7218 0000 0072  r!...r....r....r
+00000f80: 1900 0000 da08 5f5f 696e 6974 5f5f 5b00  ......__init__[.
+00000f90: 0000 7302 0000 000a 017a 1443 7573 746f  ..s......z.Custo
+00000fa0: 6d4d 6f64 656c 2e5f 5f69 6e69 745f 5fda  mModel.__init__.
+00000fb0: 0778 5f74 7261 696e da06 785f 7465 7374  .x_train..x_test
+00000fc0: da07 795f 7472 6169 6eda 0679 5f74 6573  ..y_train..y_tes
+00000fd0: 7472 1200 0000 4e63 0500 0000 0000 0000  tr....Nc........
+00000fe0: 0000 0000 0500 0000 0400 0000 4300 0000  ............C...
+00000ff0: 731a 0000 0074 0083 007c 005f 017c 006a  s....t...|._.|.j
+00001000: 01a0 027c 017c 03a1 0201 0064 0053 0072  ...|.|.....d.S.r
+00001010: 5300 0000 2903 7204 0000 0072 5400 0000  S...).r....rT...
+00001020: da03 6669 7429 0572 2100 0000 7256 0000  ..fit).r!...rV..
+00001030: 0072 5700 0000 7258 0000 0072 5900 0000  .rW...rX...rY...
+00001040: 7218 0000 0072 1800 0000 7219 0000 0072  r....r....r....r
+00001050: 5a00 0000 5e00 0000 7304 0000 0008 0712  Z...^...s.......
+00001060: 017a 0f43 7573 746f 6d4d 6f64 656c 2e66  .z.CustomModel.f
+00001070: 6974 721f 0000 0063 0200 0000 0000 0000  itr....c........
+00001080: 0000 0000 0400 0000 0300 0000 4300 0000  ............C...
+00001090: 7320 0000 007c 006a 00a0 017c 01a1 017d  s ...|.j...|...}
+000010a0: 027c 006a 00a0 027c 01a1 017d 037c 027c  .|.j...|...}.|.|
+000010b0: 0366 0253 0072 5300 0000 2903 7254 0000  .f.S.rS...).rT..
+000010c0: 005a 0d70 7265 6469 6374 5f70 726f 6261  .Z.predict_proba
+000010d0: 7246 0000 0029 0472 2100 0000 721f 0000  rF...).r!...r...
+000010e0: 00da 1070 7265 6469 6374 6564 5f70 726f  ...predicted_pro
+000010f0: 6261 73da 1170 7265 6469 6374 6564 5f63  bas..predicted_c
+00001100: 6c61 7373 6573 7218 0000 0072 1800 0000  lassesr....r....
+00001110: 7219 0000 0072 4600 0000 6800 0000 7306  r....rF...h...s.
+00001120: 0000 000c 010c 0108 017a 1343 7573 746f  .........z.Custo
+00001130: 6d4d 6f64 656c 2e70 7265 6469 6374 290c  mModel.predict).
+00001140: 722e 0000 0072 2f00 0000 7230 0000 0072  r....r/...r0...r
+00001150: 5500 0000 7229 0000 0072 3100 0000 722a  U...r)...r1...r*
+00001160: 0000 0072 5a00 0000 7203 0000 0072 0e00  ...rZ...r....r..
+00001170: 0000 720d 0000 0072 4600 0000 7218 0000  ..r....rF...r...
+00001180: 0072 1800 0000 7218 0000 0072 1900 0000  .r....r....r....
+00001190: 7252 0000 005a 0000 0073 1c00 0000 0800  rR...Z...s......
+000011a0: 0801 0203 0402 02fe 0403 02fd 0404 02fc  ................
+000011b0: 0405 02fb 0206 0afa 200a 7252 0000 0063  ........ .rR...c
+000011c0: 0000 0000 0000 0000 0000 0000 0d00 0000  ................
+000011d0: 0a00 0000 4300 0000 73b4 0200 0074 0083  ....C...s....t..
+000011e0: 007d 0074 0183 007d 0164 017c 015f 0264  .}.t...}.d.|._.d
+000011f0: 027c 015f 0364 037c 015f 0447 0064 0464  .|._.d.|._.G.d.d
+00001200: 0584 0064 0574 0583 037d 027c 0283 007d  ...d.t...}.|...}
+00001210: 0374 0664 0664 077c 007c 017c 0364 088d  .t.d.d.|.|.|.d..
+00001220: 057d 0474 07a0 0864 0964 0a84 0074 0964  .}.t...d.d...t.d
+00001230: 0183 0144 0083 0164 0b64 0a84 0074 0964  ...D...d.d...t.d
+00001240: 0183 0144 0083 0164 0c64 0a84 0074 0964  ...D...d.d...t.d
+00001250: 0183 0144 0083 0164 0d64 0a84 0074 0964  ...D...d.d...t.d
+00001260: 0183 0144 0083 0164 0e64 0a84 0074 0964  ...D...d.d...t.d
+00001270: 0183 0144 0083 0164 0f64 0a84 0074 0964  ...D...d.d...t.d
+00001280: 0183 0144 0083 0164 109c 06a1 017d 0574  ...D...d.....}.t
+00001290: 07a0 0a67 0064 11a2 01a1 017d 0674 07a0  ...g.d.....}.t..
+000012a0: 0864 1264 0a84 0074 0964 0183 0144 0083  .d.d...t.d...D..
+000012b0: 0164 1364 0a84 0074 0964 0183 0144 0083  .d.d...t.d...D..
+000012c0: 0164 1464 0a84 0074 0964 0183 0144 0083  .d.d...t.d...D..
+000012d0: 0164 1564 0a84 0074 0964 0183 0144 0083  .d.d...t.d...D..
+000012e0: 0164 1664 0a84 0074 0964 0183 0144 0083  .d.d...t.d...D..
+000012f0: 0164 1764 0a84 0074 0964 0183 0144 0083  .d.d...t.d...D..
+00001300: 0164 109c 06a1 017d 077c 067c 0564 073c  .d.....}.|.|.d.<
+00001310: 007c 04a0 0b7c 0564 07a1 0201 007c 04a0  .|...|.d.....|..
+00001320: 0c7c 07a1 015c 027d 087d 0974 0d6a 0e7d  .|...\.}.}.t.j.}
+00001330: 0a74 0f7c 087c 0a83 027d 0b7c 0b73 f864  .t.|.|...}.|.s.d
+00001340: 1864 1974 10a0 11a1 0076 0073 bd74 12a0  .d.t.....v.s.t..
+00001350: 1374 0fa1 0172 c274 12a0 1474 0fa1 016e  .t...r.t...t...n
+00001360: 0164 1964 1a74 10a0 11a1 0076 0073 ce74  .d.d.t.....v.s.t
+00001370: 12a0 137c 08a1 0172 d374 12a0 147c 08a1  ...|...r.t...|..
+00001380: 016e 0164 1a64 1b74 10a0 11a1 0076 0073  .n.d.d.t.....v.s
+00001390: df74 12a0 1374 0da1 0172 e474 12a0 1474  .t...t...r.t...t
+000013a0: 0da1 016e 0164 1b74 12a0 147c 0aa1 0174  ...n.d.t...|...t
+000013b0: 12a0 147c 0ba1 0164 1c9c 0516 007d 0c74  ...|...d.....}.t
+000013c0: 1574 12a0 167c 0ca1 0183 0182 0164 0004  .t...|.......d..
+000013d0: 007d 0a7d 0b74 0d6a 0e7d 0a74 0f7c 097c  .}.}.t.j.}.t.|.|
+000013e0: 0a83 027d 0b7c 0b90 0173 5464 1864 1974  ...}.|...sTd.d.t
+000013f0: 10a0 11a1 0076 0090 0173 1574 12a0 1374  .....v...s.t...t
+00001400: 0fa1 0190 0172 1a74 12a0 1474 0fa1 016e  .....r.t...t...n
+00001410: 0164 1964 1d74 10a0 11a1 0076 0090 0173  .d.d.t.....v...s
+00001420: 2874 12a0 137c 09a1 0190 0172 2d74 12a0  (t...|.....r-t..
+00001430: 147c 09a1 016e 0164 1d64 1b74 10a0 11a1  .|...n.d.d.t....
+00001440: 0076 0090 0173 3b74 12a0 1374 0da1 0190  .v...s;t...t....
+00001450: 0172 4074 12a0 1474 0da1 016e 0164 1b74  .r@t...t...n.d.t
+00001460: 12a0 147c 0aa1 0174 12a0 147c 0ba1 0164  ...|...t...|...d
+00001470: 1c9c 0516 007d 0c74 1574 12a0 167c 0ca1  .....}.t.t...|..
+00001480: 0183 0182 0164 0004 007d 0a7d 0b64 0053  .....d...}.}.d.S
+00001490: 0029 1e4e 721e 0000 0054 e902 0000 0063  .).Nr....T.....c
+000014a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000014b0: 0c00 0000 0000 0000 7386 0000 0065 005a  ........s....e.Z
+000014c0: 0164 005a 0264 0f64 0265 0366 0287 0066  .d.Z.d.d.e.f...f
+000014d0: 0164 0364 0484 0d5a 0464 0565 056a 0664  .d.d...Z.d.e.j.d
+000014e0: 0665 056a 0764 0765 0865 056a 0665 0965  .e.j.d.e.e.j.e.e
+000014f0: 056a 0719 0066 0219 0066 0664 0864 0984  .j...f...f.d.d..
+00001500: 045a 0a09 0a09 0b64 1064 0565 056a 0664  .Z.....d.d.e.j.d
+00001510: 0665 0965 056a 0719 0064 0c65 0b64 0765  .e.e.j...d.e.d.e
+00001520: 0865 056a 0665 0965 056a 0719 0066 0219  .e.j.e.e.j...f..
+00001530: 0066 0864 0d64 0e84 055a 0c87 0004 005a  .f.d.d...Z.....Z
+00001540: 0d53 0029 117a 3674 6573 745f 626c 7565  .S.).z6test_blue
+00001550: 6361 7374 5f77 6974 685f 6375 7374 6f6d  cast_with_custom
+00001560: 5f6d 6f64 656c 2e3c 6c6f 6361 6c73 3e2e  _model.<locals>.
+00001570: 5246 4543 5653 656c 6563 746f 7272 0100  RFECVSelectorr..
+00001580: 0000 7214 0000 0063 0200 0000 0000 0000  ..r....c........
+00001590: 0000 0000 0200 0000 0800 0000 1300 0000  ................
+000015a0: 7342 0000 0074 0083 00a0 01a1 0001 0064  sB...t.........d
+000015b0: 007c 005f 027c 017c 005f 0374 0474 05a0  .|._.|.|._.t.t..
+000015c0: 06a1 0064 0174 0764 027c 0164 0364 048d  ...d.t.d.|.d.d..
+000015d0: 0364 0174 0874 0983 0164 0264 058d 067c  .d.t.t...d.d...|
+000015e0: 005f 0a64 0053 0029 064e 721b 0000 0072  ._.d.S.).Nr....r
+000015f0: 5d00 0000 5429 0272 1400 0000 da07 7368  ]...T).r......sh
+00001600: 7566 666c 6529 06da 0965 7374 696d 6174  uffle)...estimat
+00001610: 6f72 da04 7374 6570 da02 6376 5a16 6d69  or..step..cvZ.mi
+00001620: 6e5f 6665 6174 7572 6573 5f74 6f5f 7365  n_features_to_se
+00001630: 6c65 6374 5a07 7363 6f72 696e 67da 066e  lectZ.scoring..n
+00001640: 5f6a 6f62 7329 0bda 0573 7570 6572 7255  _jobs)...superrU
+00001650: 0000 00da 1173 656c 6563 7465 645f 6665  .....selected_fe
+00001660: 6174 7572 6573 7214 0000 0072 0500 0000  aturesr....r....
+00001670: da03 7867 625a 0d58 4742 436c 6173 7369  ..xgbZ.XGBClassi
+00001680: 6669 6572 7208 0000 0072 0600 0000 7207  fierr....r....r.
+00001690: 0000 00da 1273 656c 6563 7469 6f6e 5f73  .....selection_s
+000016a0: 7472 6174 6567 7929 0272 2100 0000 7214  trategy).r!...r.
+000016b0: 0000 00a9 01da 095f 5f63 6c61 7373 5f5f  .......__class__
+000016c0: 7218 0000 0072 1900 0000 7255 0000 0078  r....r....rU...x
+000016d0: 0000 0073 1600 0000 0a01 0601 0601 0201  ...s............
+000016e0: 0601 0201 0c01 0201 0601 0201 0cfa 7a3f  ..............z?
+000016f0: 7465 7374 5f62 6c75 6563 6173 745f 7769  test_bluecast_wi
+00001700: 7468 5f63 7573 746f 6d5f 6d6f 6465 6c2e  th_custom_model.
+00001710: 3c6c 6f63 616c 733e 2e52 4645 4356 5365  <locals>.RFECVSe
+00001720: 6c65 6374 6f72 2e5f 5f69 6e69 745f 5f72  lector.__init__r
+00001730: 1f00 0000 7223 0000 0072 1200 0000 6303  ....r#...r....c.
+00001740: 0000 0000 0000 0000 0000 0003 0000 0004  ................
+00001750: 0000 0053 0000 0073 3400 0000 7c00 6a00  ...S...s4...|.j.
+00001760: a001 7c01 7c02 a102 0100 7c00 6a00 6a02  ..|.|.....|.j.j.
+00001770: 7c00 5f03 7c01 6a04 6400 6400 8502 7c00  |._.|.j.d.d...|.
+00001780: 6a03 6602 1900 7d01 7c01 7c02 6602 5300  j.f...}.|.|.f.S.
+00001790: 7253 0000 0029 0572 6600 0000 725a 0000  rS...).rf...rZ..
+000017a0: 005a 0873 7570 706f 7274 5f72 6400 0000  .Z.support_rd...
+000017b0: da03 6c6f 6372 2500 0000 7218 0000 0072  ..locr%...r....r
+000017c0: 1800 0000 7219 0000 0072 2600 0000 8500  ....r....r&.....
+000017d0: 0000 7308 0000 000e 030a 0114 0108 017a  ..s............z
+000017e0: 4474 6573 745f 626c 7565 6361 7374 5f77  Dtest_bluecast_w
+000017f0: 6974 685f 6375 7374 6f6d 5f6d 6f64 656c  ith_custom_model
+00001800: 2e3c 6c6f 6361 6c73 3e2e 5246 4543 5653  .<locals>.RFECVS
+00001810: 656c 6563 746f 722e 6669 745f 7472 616e  elector.fit_tran
+00001820: 7366 6f72 6d4e 4672 2700 0000 6304 0000  sformNFr'...c...
+00001830: 0000 0000 0000 0000 0004 0000 0003 0000  ................
+00001840: 0053 0000 0073 1c00 0000 7c01 6a00 6400  .S...s....|.j.d.
+00001850: 6400 8502 7c00 6a01 6602 1900 7d01 7c01  d...|.j.f...}.|.
+00001860: 7c02 6602 5300 7253 0000 0029 0272 6900  |.f.S.rS...).ri.
+00001870: 0000 7264 0000 0072 2b00 0000 7218 0000  ..rd...r+...r...
+00001880: 0072 1800 0000 7219 0000 0072 2c00 0000  .r....r....r,...
+00001890: 8d00 0000 7304 0000 0014 0608 017a 4074  ....s........z@t
+000018a0: 6573 745f 626c 7565 6361 7374 5f77 6974  est_bluecast_wit
+000018b0: 685f 6375 7374 6f6d 5f6d 6f64 656c 2e3c  h_custom_model.<
+000018c0: 6c6f 6361 6c73 3e2e 5246 4543 5653 656c  locals>.RFECVSel
+000018d0: 6563 746f 722e 7472 616e 7366 6f72 6d29  ector.transform)
+000018e0: 0172 0100 0000 722d 0000 0029 0e72 2e00  .r....r-...).r..
+000018f0: 0000 722f 0000 0072 3000 0000 da03 696e  ..r/...r0.....in
+00001900: 7472 5500 0000 7229 0000 0072 3100 0000  trU...r)...r1...
+00001910: 722a 0000 0072 0300 0000 7202 0000 0072  r*...r....r....r
+00001920: 2600 0000 7232 0000 0072 2c00 0000 da0d  &...r2...r,.....
+00001930: 5f5f 636c 6173 7363 656c 6c5f 5f72 1800  __classcell__r..
+00001940: 0000 7218 0000 0072 6700 0000 7219 0000  ..r....rg...r...
+00001950: 00da 0d52 4645 4356 5365 6c65 6374 6f72  ...RFECVSelector
+00001960: 7700 0000 7328 0000 0008 0014 0102 0d04  w...s(..........
+00001970: 0102 ff04 0102 ff12 020a fe02 0b02 0104  ................
+00001980: fc04 0202 fe08 0302 fd02 0402 fc12 0512  ................
+00001990: fb72 6c00 0000 7234 0000 0072 2300 0000  .rl...r4...r#...
+000019a0: 2905 7235 0000 0072 3600 0000 5a08 6d6c  ).r5...r6...Z.ml
+000019b0: 5f6d 6f64 656c 7237 0000 00da 1763 7573  _modelr7.....cus
+000019c0: 746f 6d5f 6665 6174 7572 655f 7365 6c65  tom_feature_sele
+000019d0: 6374 6f72 6301 0000 0000 0000 0000 0000  ctorc...........
+000019e0: 0002 0000 0003 0000 0053 0000 00f3 1000  .........S......
+000019f0: 0000 6700 7c00 5d04 7d01 7c01 9102 7102  ..g.|.].}.|...q.
+00001a00: 5300 7218 0000 0072 1800 0000 a902 da02  S.r....r........
+00001a10: 2e30 da01 6972 1800 0000 7218 0000 0072  .0..ir....r....r
+00001a20: 1900 0000 da0a 3c6c 6973 7463 6f6d 703e  ......<listcomp>
+00001a30: a400 0000 f302 0000 0010 007a 3374 6573  ...........z3tes
+00001a40: 745f 626c 7565 6361 7374 5f77 6974 685f  t_bluecast_with_
+00001a50: 6375 7374 6f6d 5f6d 6f64 656c 2e3c 6c6f  custom_model.<lo
+00001a60: 6361 6c73 3e2e 3c6c 6973 7463 6f6d 703e  cals>.<listcomp>
+00001a70: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
+00001a80: 0003 0000 0053 0000 0072 6e00 0000 7218  .....S...rn...r.
+00001a90: 0000 0072 1800 0000 726f 0000 0072 1800  ...r....ro...r..
+00001aa0: 0000 7218 0000 0072 1900 0000 7272 0000  ..r....r....rr..
+00001ab0: 00a5 0000 0072 7300 0000 6301 0000 0000  .....rs...c.....
+00001ac0: 0000 0000 0000 0002 0000 0003 0000 0053  ...............S
+00001ad0: 0000 0072 6e00 0000 7218 0000 0072 1800  ...rn...r....r..
+00001ae0: 0000 726f 0000 0072 1800 0000 7218 0000  ..ro...r....r...
+00001af0: 0072 1900 0000 7272 0000 00a6 0000 0072  .r....rr.......r
+00001b00: 7300 0000 6301 0000 0000 0000 0000 0000  s...c...........
+00001b10: 0002 0000 0003 0000 0053 0000 0072 6e00  .........S...rn.
+00001b20: 0000 7218 0000 0072 1800 0000 726f 0000  ..r....r....ro..
+00001b30: 0072 1800 0000 7218 0000 0072 1900 0000  .r....r....r....
+00001b40: 7272 0000 00a7 0000 0072 7300 0000 6301  rr.......rs...c.
+00001b50: 0000 0000 0000 0000 0000 0002 0000 0003  ................
+00001b60: 0000 0053 0000 0072 6e00 0000 7218 0000  ...S...rn...r...
+00001b70: 0072 1800 0000 726f 0000 0072 1800 0000  .r....ro...r....
+00001b80: 7218 0000 0072 1900 0000 7272 0000 00a8  r....r....rr....
+00001b90: 0000 0072 7300 0000 6301 0000 0000 0000  ...rs...c.......
+00001ba0: 0000 0000 0002 0000 0003 0000 0053 0000  .............S..
+00001bb0: 0072 6e00 0000 7218 0000 0072 1800 0000  .rn...r....r....
+00001bc0: 726f 0000 0072 1800 0000 7218 0000 0072  ro...r....r....r
+00001bd0: 1900 0000 7272 0000 00a9 0000 0072 7300  ....rr.......rs.
+00001be0: 0000 2906 5a08 6665 6174 7572 6531 5a08  ..).Z.feature1Z.
+00001bf0: 6665 6174 7572 6532 5a08 6665 6174 7572  feature2Z.featur
+00001c00: 6533 5a08 6665 6174 7572 6534 5a08 6665  e3Z.feature4Z.fe
+00001c10: 6174 7572 6535 5a08 6665 6174 7572 6536  ature5Z.feature6
+00001c20: 290a 7201 0000 0072 1b00 0000 7201 0000  ).r....r....r...
+00001c30: 0072 1b00 0000 7201 0000 0072 1b00 0000  .r....r....r....
+00001c40: 7201 0000 0072 1b00 0000 7201 0000 0072  r....r....r....r
+00001c50: 1b00 0000 6301 0000 0000 0000 0000 0000  ....c...........
+00001c60: 0002 0000 0003 0000 0053 0000 0072 6e00  .........S...rn.
+00001c70: 0000 7218 0000 0072 1800 0000 726f 0000  ..r....r....ro..
+00001c80: 0072 1800 0000 7218 0000 0072 1900 0000  .r....r....r....
+00001c90: 7272 0000 00af 0000 0072 7300 0000 6301  rr.......rs...c.
+00001ca0: 0000 0000 0000 0000 0000 0002 0000 0003  ................
+00001cb0: 0000 0053 0000 0072 6e00 0000 7218 0000  ...S...rn...r...
+00001cc0: 0072 1800 0000 726f 0000 0072 1800 0000  .r....ro...r....
+00001cd0: 7218 0000 0072 1900 0000 7272 0000 00b0  r....r....rr....
+00001ce0: 0000 0072 7300 0000 6301 0000 0000 0000  ...rs...c.......
+00001cf0: 0000 0000 0002 0000 0003 0000 0053 0000  .............S..
+00001d00: 0072 6e00 0000 7218 0000 0072 1800 0000  .rn...r....r....
+00001d10: 726f 0000 0072 1800 0000 7218 0000 0072  ro...r....r....r
+00001d20: 1900 0000 7272 0000 00b1 0000 0072 7300  ....rr.......rs.
+00001d30: 0000 6301 0000 0000 0000 0000 0000 0002  ..c.............
+00001d40: 0000 0003 0000 0053 0000 0072 6e00 0000  .......S...rn...
+00001d50: 7218 0000 0072 1800 0000 726f 0000 0072  r....r....ro...r
+00001d60: 1800 0000 7218 0000 0072 1900 0000 7272  ....r....r....rr
+00001d70: 0000 00b2 0000 0072 7300 0000 6301 0000  .......rs...c...
+00001d80: 0000 0000 0000 0000 0002 0000 0003 0000  ................
+00001d90: 0053 0000 0072 6e00 0000 7218 0000 0072  .S...rn...r....r
+00001da0: 1800 0000 726f 0000 0072 1800 0000 7218  ....ro...r....r.
+00001db0: 0000 0072 1900 0000 7272 0000 00b3 0000  ...r....rr......
+00001dc0: 0072 7300 0000 6301 0000 0000 0000 0000  .rs...c.........
+00001dd0: 0000 0002 0000 0003 0000 0053 0000 0072  ...........S...r
+00001de0: 6e00 0000 7218 0000 0072 1800 0000 726f  n...r....r....ro
+00001df0: 0000 0072 1800 0000 7218 0000 0072 1900  ...r....r....r..
+00001e00: 0000 7272 0000 00b4 0000 0072 7300 0000  ..rr.......rs...
+00001e10: 7a52 6173 7365 7274 2025 2870 7936 2973  zRassert %(py6)s
+00001e20: 0a7b 2528 7079 3629 7320 3d20 2528 7079  .{%(py6)s = %(py
+00001e30: 3029 7328 2528 7079 3129 732c 2025 2870  0)s(%(py1)s, %(p
+00001e40: 7934 2973 0a7b 2528 7079 3429 7320 3d20  y4)s.{%(py4)s = 
+00001e50: 2528 7079 3229 732e 6e64 6172 7261 790a  %(py2)s.ndarray.
+00001e60: 7d29 0a7d 7228 0000 0072 5b00 0000 da02  }).}r(...r[.....
+00001e70: 6e70 2905 723d 0000 0072 3e00 0000 5a03  np).r=...r>...Z.
+00001e80: 7079 325a 0370 7934 723f 0000 0072 5c00  py2Z.py4r?...r\.
+00001e90: 0000 2917 7252 0000 0072 0a00 0000 7241  ..).rR...r....rA
+00001ea0: 0000 0072 4200 0000 7243 0000 0072 0f00  ...rB...rC...r..
+00001eb0: 0000 7209 0000 0072 2900 0000 7231 0000  ..r....r)...r1..
+00001ec0: 00da 0572 616e 6765 722a 0000 0072 5a00  ...ranger*...rZ.
+00001ed0: 0000 7246 0000 0072 7400 0000 da07 6e64  ..rF...rt.....nd
+00001ee0: 6172 7261 7972 2800 0000 724a 0000 0072  arrayr(...rJ...r
+00001ef0: 4b00 0000 7248 0000 0072 4c00 0000 724d  K...rH...rL...rM
+00001f00: 0000 0072 4e00 0000 724f 0000 0029 0d5a  ...rN...rO...).Z
+00001f10: 0c63 7573 746f 6d5f 6d6f 6465 6c72 5000  .custom_modelrP.
+00001f20: 0000 726c 0000 0072 6d00 0000 da08 626c  ..rl...rm.....bl
+00001f30: 7565 6361 7374 7256 0000 0072 5800 0000  uecastrV...rX...
+00001f40: 7257 0000 0072 5b00 0000 725c 0000 005a  rW...r[...r\...Z
+00001f50: 0b40 7079 5f61 7373 6572 7433 5a0b 4070  .@py_assert3Z.@p
+00001f60: 795f 6173 7365 7274 355a 0b40 7079 5f66  y_assert5Z.@py_f
+00001f70: 6f72 6d61 7437 7218 0000 0072 1800 0000  ormat7r....r....
+00001f80: 7219 0000 00da 1f74 6573 745f 626c 7565  r......test_blue
+00001f90: 6361 7374 5f77 6974 685f 6375 7374 6f6d  cast_with_custom
+00001fa0: 5f6d 6f64 656c 6e00 0000 734c 0000 0006  _modeln...sL....
+00001fb0: 0206 0106 0106 0106 0110 0306 1f02 0302  ................
+00001fc0: 0102 0102 0102 0102 0106 fb04 0910 0210  ................
+00001fd0: 0110 0110 0110 0110 0104 fa04 ff0e 0a04  ................
+00001fe0: 0110 0210 0110 0110 0110 0110 0104 fa04  ................
+00001ff0: ff08 0b0c 030e 03aa 03bc 0172 7800 0000  ...........rx...
+00002000: 292c da08 6275 696c 7469 6e73 724a 0000  ),..builtinsrJ..
+00002010: 00da 195f 7079 7465 7374 2e61 7373 6572  ..._pytest.asser
+00002020: 7469 6f6e 2e72 6577 7269 7465 da09 6173  tion.rewrite..as
+00002030: 7365 7274 696f 6eda 0772 6577 7269 7465  sertion..rewrite
+00002040: 7248 0000 00da 0674 7970 696e 6772 0200  rH.....typingr..
+00002050: 0000 7203 0000 00da 056e 756d 7079 7274  ..r......numpyrt
+00002060: 0000 00da 0670 616e 6461 7372 2900 0000  .....pandasr)...
+00002070: da06 7079 7465 7374 5a07 7867 626f 6f73  ..pytestZ.xgboos
+00002080: 7472 6500 0000 5a10 736b 6c65 6172 6e2e  tre...Z.sklearn.
+00002090: 656e 7365 6d62 6c65 7204 0000 005a 1973  ensembler....Z.s
+000020a0: 6b6c 6561 726e 2e66 6561 7475 7265 5f73  klearn.feature_s
+000020b0: 656c 6563 7469 6f6e 7205 0000 005a 0f73  electionr....Z.s
+000020c0: 6b6c 6561 726e 2e6d 6574 7269 6373 7206  klearn.metricsr.
+000020d0: 0000 0072 0700 0000 5a17 736b 6c65 6172  ...r....Z.sklear
+000020e0: 6e2e 6d6f 6465 6c5f 7365 6c65 6374 696f  n.model_selectio
+000020f0: 6e72 0800 0000 5a18 626c 7565 6361 7374  nr....Z.bluecast
+00002100: 2e62 6c75 6570 7269 6e74 732e 6361 7374  .blueprints.cast
+00002110: 7209 0000 005a 1f62 6c75 6563 6173 742e  r....Z.bluecast.
+00002120: 636f 6e66 6967 2e74 7261 696e 696e 675f  config.training_
+00002130: 636f 6e66 6967 720a 0000 0072 0b00 0000  configr....r....
+00002140: 5a22 626c 7565 6361 7374 2e6d 6c5f 6d6f  Z"bluecast.ml_mo
+00002150: 6465 6c6c 696e 672e 6261 7365 5f63 6c61  delling.base_cla
+00002160: 7373 6573 720c 0000 0072 0d00 0000 720e  ssesr....r....r.
+00002170: 0000 005a 1d62 6c75 6563 6173 742e 7072  ...Z.bluecast.pr
+00002180: 6570 726f 6365 7373 696e 672e 6375 7374  eprocessing.cust
+00002190: 6f6d 720f 0000 00da 2462 6c75 6563 6173  omr.....$bluecas
+000021a0: 742e 7465 7374 732e 6d61 6b65 5f64 6174  t.tests.make_dat
+000021b0: 612e 6372 6561 7465 5f64 6174 6172 1100  a.create_datar..
+000021c0: 0000 da07 6669 7874 7572 6572 3100 0000  ....fixturer1...
+000021d0: 721a 0000 0072 5100 0000 7252 0000 0072  r....rQ...rR...r
+000021e0: 7800 0000 7218 0000 0072 1800 0000 7218  x...r....r....r.
+000021f0: 0000 0072 1900 0000 da08 3c6d 6f64 756c  ...r......<modul
+00002200: 653e 0100 0000 7326 0000 002a 0008 0208  e>....s&...*....
+00002210: 0108 0108 010c 010c 0110 010c 010c 0210  ................
+00002220: 0114 010c 050c 0104 031c 0108 0610 3c0c  ..............<.
+00002230: 14                                       .
```

### Comparing `bluecast-0.5/bluecast/tests/__pycache__/test_check_gpu_support.cpython-310-pytest-6.2.5.pyc` & `bluecast-0.7/bluecast/tests/__pycache__/test_check_gpu_support.cpython-310-pytest-6.2.5.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.5/bluecast/tests/__pycache__/test_custom_processing_base_class.cpython-310-pytest-6.2.5.pyc` & `bluecast-0.7/bluecast/tests/__pycache__/test_custom_processing_base_class.cpython-310-pytest-6.2.5.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.5/bluecast/tests/__pycache__/test_datetime_features.cpython-310-pytest-6.2.5.pyc` & `bluecast-0.7/bluecast/tests/__pycache__/test_datetime_features.cpython-310-pytest-6.2.5.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.5/bluecast/tests/__pycache__/test_encode_target_labels.cpython-310-pytest-6.2.5.pyc` & `bluecast-0.7/bluecast/tests/__pycache__/test_encode_target_labels.cpython-310-pytest-6.2.5.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.5/bluecast/tests/__pycache__/test_feature_type_detector.cpython-310-pytest-6.2.5.pyc` & `bluecast-0.7/bluecast/tests/__pycache__/test_feature_type_detector.cpython-310-pytest-6.2.5.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.5/bluecast/tests/__pycache__/test_load_for_production.cpython-310-pytest-6.2.5.pyc` & `bluecast-0.7/bluecast/tests/__pycache__/test_load_for_production.cpython-310-pytest-6.2.5.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.5/bluecast/tests/__pycache__/test_nulls_and_infs.cpython-310-pytest-6.2.5.pyc` & `bluecast-0.7/bluecast/tests/__pycache__/test_nulls_and_infs.cpython-310-pytest-6.2.5.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.5/bluecast/tests/__pycache__/test_save_to_production.cpython-310-pytest-6.2.5.pyc` & `bluecast-0.7/bluecast/tests/__pycache__/test_save_to_production.cpython-310-pytest-6.2.5.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.5/bluecast/tests/__pycache__/test_schema_checks.cpython-310-pytest-6.2.5.pyc` & `bluecast-0.7/bluecast/tests/__pycache__/test_schema_checks.cpython-310-pytest-6.2.5.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.5/bluecast/tests/__pycache__/test_shap_explanations.cpython-310-pytest-6.2.5.pyc` & `bluecast-0.7/bluecast/tests/__pycache__/test_shap_explanations.cpython-310-pytest-6.2.5.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun Jun 25 05:34:02 2023 UTC, .py size: 2296 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 cad1 9764 f808 0000  o..........d....
+00000000: 6f0d 0d0a 0000 0000 945b 9a64 f808 0000  o........[.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 b600 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6400 6402 6c06 6d07  ..m.Z...d.d.l.m.
 00000050: 5a07 0100 6400 6401 6c08 5a09 6400 6401  Z...d.d.l.Z.d.d.
 00000060: 6c0a 5a0b 6400 6401 6c0c 5a0c 6400 6403  l.Z.d.d.l.Z.d.d.
 00000070: 6c0d 6d0e 5a0e 0100 6400 6404 6c0f 6d10  l.m.Z...d.d.l.m.
```

### Comparing `bluecast-0.5/bluecast/tests/__pycache__/test_target_encoding_binary.cpython-310-pytest-6.2.5.pyc` & `bluecast-0.7/bluecast/tests/__pycache__/test_target_encoding_binary.cpython-310-pytest-6.2.5.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.5/bluecast/tests/__pycache__/test_target_encoding_multiclass.cpython-310-pytest-6.2.5.pyc` & `bluecast-0.7/bluecast/tests/__pycache__/test_target_encoding_multiclass.cpython-310-pytest-6.2.5.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.5/bluecast/tests/__pycache__/test_train_test_split.cpython-310-pytest-6.2.5.pyc` & `bluecast-0.7/bluecast/tests/__pycache__/test_train_test_split.cpython-310-pytest-6.2.5.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.5/bluecast/tests/make_data/__pycache__/create_data.cpython-310.pyc` & `bluecast-0.7/bluecast/tests/make_data/__pycache__/create_data.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bluecast-0.5/bluecast/tests/make_data/create_data.py` & `bluecast-0.7/bluecast/tests/make_data/create_data.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.5/bluecast/tests/test_cast.py` & `bluecast-0.7/bluecast/tests/test_cast.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,14 @@
     train_config.hyperparameter_tuning_rounds = 10
     train_config.enable_feature_selection = False
     train_config.hypertuning_cv_folds = 1
 
     # add custom last mile computation
     class MyCustomLastMilePreprocessing(CustomPreprocessing):
         def custom_function(self, df: pd.DataFrame) -> pd.DataFrame:
-            df = df / 2
             df["custom_col"] = 5
             return df
 
         def fit_transform(
             self, df: pd.DataFrame, target: pd.Series
         ) -> Tuple[pd.DataFrame, pd.Series]:
             df = self.custom_function(df)
@@ -71,15 +70,20 @@
     automl = BlueCast(
         class_problem="binary",
         target_column="target",
         conf_training=train_config,
         conf_xgboost=xgboost_param_config,
         custom_last_mile_computation=custom_last_mile_computation,
     )
-    automl.fit(df_train, target_col="target")
+    automl.fit_eval(
+        df_train,
+        df_train.drop("target", axis=1),
+        df_train["target"],
+        target_col="target",
+    )
     print("Autotuning successful.")
     y_probs, y_classes = automl.predict(df_val.drop("target", axis=1))
     print("Predicting successful.")
     assert len(y_probs) == len(df_val.index)
     assert len(y_classes) == len(df_val.index)
```

### Comparing `bluecast-0.5/bluecast/tests/test_check_gpu_support.py` & `bluecast-0.7/bluecast/tests/test_check_gpu_support.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.5/bluecast/tests/test_custom_processing_base_class.py` & `bluecast-0.7/bluecast/tests/test_custom_processing_base_class.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.5/bluecast/tests/test_datetime_features.py` & `bluecast-0.7/bluecast/tests/test_datetime_features.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.5/bluecast/tests/test_encode_target_labels.py` & `bluecast-0.7/bluecast/tests/test_encode_target_labels.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.5/bluecast/tests/test_feature_type_detector.py` & `bluecast-0.7/bluecast/tests/test_feature_type_detector.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.5/bluecast/tests/test_load_for_production.py` & `bluecast-0.7/bluecast/tests/test_load_for_production.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.5/bluecast/tests/test_nulls_and_infs.py` & `bluecast-0.7/bluecast/tests/test_nulls_and_infs.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.5/bluecast/tests/test_save_to_production.py` & `bluecast-0.7/bluecast/tests/test_save_to_production.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.5/bluecast/tests/test_schema_checks.py` & `bluecast-0.7/bluecast/tests/test_schema_checks.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.5/bluecast/tests/test_shap_explanations.py` & `bluecast-0.7/bluecast/tests/test_shap_explanations.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.5/bluecast/tests/test_target_encoding_binary.py` & `bluecast-0.7/bluecast/tests/test_target_encoding_binary.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.5/bluecast/tests/test_target_encoding_multiclass.py` & `bluecast-0.7/bluecast/tests/test_target_encoding_multiclass.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.5/bluecast/tests/test_train_test_split.py` & `bluecast-0.7/bluecast/tests/test_train_test_split.py`

 * *Files identical despite different names*

### Comparing `bluecast-0.5/pyproject.toml` & `bluecast-0.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bluecast"
-version = "0.5"
+version = "0.7"
 description = "A lightweight and fast automl framework"
 authors = ["Thomas Meißner <meissnercorporation@gmx.de>"]
 license = "GPL-3.0-only"
 classifiers = [
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
 ]
@@ -21,14 +21,15 @@
 dill = "^0.3.3"
 matplotlib = ">=3.1.3" # pinned due to cannot import _png error
 numpy = "<1.24.0" # otherwise: AttributeError: module 'numpy' has no attribute 'int'
 optuna = ">=2.8.0"
 pandas = "^1.1.5"
 plotly = "^5"
 pydantic = "^1.8.2"
+seaborn = ">=0.10.0"
 scikit-learn = "^1.0.1"
 shap = "^0"
 xgboost = "^1.5.3"
 
 [tool.poetry.group.dev.dependencies]
 ipython = "^7.10.0"
 jupyter_core = "^4.7.0"
```

### Comparing `bluecast-0.5/PKG-INFO` & `bluecast-0.7/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bluecast
-Version: 0.5
+Version: 0.7
 Summary: A lightweight and fast automl framework
 Home-page: https://github.com/ThomasMeissnerDS/BlueCast
 License: GPL-3.0-only
 Author: Thomas Meißner
 Author-email: meissnercorporation@gmx.de
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -19,14 +19,15 @@
 Requires-Dist: matplotlib (>=3.1.3)
 Requires-Dist: numpy (<1.24.0)
 Requires-Dist: optuna (>=2.8.0)
 Requires-Dist: pandas (>=1.1.5,<2.0.0)
 Requires-Dist: plotly (>=5,<6)
 Requires-Dist: pydantic (>=1.8.2,<2.0.0)
 Requires-Dist: scikit-learn (>=1.0.1,<2.0.0)
+Requires-Dist: seaborn (>=0.10.0)
 Requires-Dist: shap (>=0,<1)
 Requires-Dist: xgboost (>=1.5.3,<2.0.0)
 Project-URL: Repository, https://github.com/ThomasMeissnerDS/BlueCast
 Description-Content-Type: text/markdown
 
 # BlueCast
 
@@ -58,15 +59,17 @@
 
 * [Installation](#installation)
   * [Installation for end users](#installation-for-end-users)
   * [Installation for developers](#installation-for-developers)
 * [General usage](#general-usage)
   * [Basic usage](#basic-usage)
   * [Advanced usage](#advanced-usage)
-    * [Custom training configuration](#custom--training-configuration)
+    * [Explanatory analysis](#explanatory-analysis)
+    * [Enable cross-validation](#enable-cross-validation)
+    * [Categorical encoding](#categorical-encoding)
     * [Custom preprocessing](#custom-preprocessing)
     * [Custom feature selection](#custom-feature-selection)
     * [Custom ML model](#custom-ml-model)
 * [Convenience features](#convenience-features)
 * [Code quality](#code-quality)
 * [Documentation](#documentation)
 * [How to contribute](#how-to-contribute)
@@ -114,14 +117,74 @@
 
 automl.fit(df_train, target_col="target")
 y_probs, y_classes = automl.predict(df_val)
 ```
 
 ### Advanced usage
 
+#### Explanatory analysis
+
+BlueCast offers a simple way to get a first overview of the data. This is
+
+#### Enable cross-validation
+
+While the default behaviour of BlueCast is to use a simple
+train-test-split, cross-validation can be enabled easily:
+
+```sh
+from bluecast.eda.analyse import (
+    bi_variate_plots,
+    correlation_heatmap,
+    correlation_to_target,
+    univariate_plots,
+)
+
+from bluecast.preprocessing.feature_types import FeatureTypeDetector
+
+# Here we automatically detect the numeric columns
+feat_type_detector = FeatureTypeDetector()
+train_data = feat_type_detector.fit_transform_feature_types(train_data)
+
+# show univariate plots
+univariate_plots(
+        train_data.loc[
+            :, feat_type_detector.num_columns  # here the target column EC1 is already included
+        ],
+        "EC1",
+    )
+
+# show bi-variate plots
+bi_variate_plots(train_data.loc[
+            :, feat_type_detector.num_columns
+        ],
+        "EC1")
+
+# show correlation heatmap
+correlation_heatmap(train_data.loc[
+            :, feat_type_detector.num_columns])
+
+# show correlation to target
+correlation_to_target(train_data.loc[
+            :, feat_type_detector.num_columns
+        ],
+        "EC1",)
+```
+
+#### Categorical encoding
+
+By default, BlueCast uses target encoding.
+This behaviour can be changed in the TrainingConfig by setting `cat_encoding_via_ml_algorithm`
+to True. This will change the expectations of `custom_last_mile_computation` though.
+If `cat_encoding_via_ml_algorithm` is set to False, `custom_last_mile_computation`
+will receive numerical features only as target encoding will apply before. If `cat_encoding_via_ml_algorithm`
+is True (default setting) `custom_last_mile_computation` will receive categorical
+features as well, because Xgboost#s inbuilt categorical encoding will be used.
+
+```sh
+
 #### Custom  training configuration
 
 Despite e2eml, BlueCast allows easy customization. Users can adjust the
 configuration and just pass it to the `BlueCast` class. Here is an example:
 
 ```sh
 from bluecast.blueprints.cast import BlueCast
@@ -431,21 +494,22 @@
 
 Despite being a lightweight library, BlueCast also includes some convenience
 with the following features:
 
 * automatic feature type detection and casting
 * automatic DataFrame schema detection: checks if unseen data has new or
   missing columns
-* categorical feature encoding
+* categorical feature encoding (target encoding or directly in Xgboost)
 * datetime feature encoding
 * automated GPU availability check and usage for Xgboost
   a fit_eval method to fit a model and evaluate it on a validation set
   to mimic production environment reality
 * functions to save and load a trained pipeline
 * shapley values
+* warnings for potential misconfigurations
 
 The fit_eval method can be used like this:
 
 ```sh
 from bluecast.blueprints.cast import BlueCast
 
 automl = BlueCast(
```

