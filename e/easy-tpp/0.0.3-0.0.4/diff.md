# Comparing `tmp/easy_tpp-0.0.3.tar.gz` & `tmp/easy_tpp-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/easy_tpp-0.0.3.tar", last modified: Sun Jul  2 03:19:21 2023, max compression
+gzip compressed data, was "dist/easy_tpp-0.0.4.tar", last modified: Sun Jul  2 03:53:02 2023, max compression
```

## Comparing `easy_tpp-0.0.3.tar` & `easy_tpp-0.0.4.tar`

### file list

```diff
@@ -1,86 +1,89 @@
-drwxr-xr-x   0 sissif     (501) staff       (20)        0 2023-07-02 03:19:21.000000 easy_tpp-0.0.3/
--rw-rw-r--   0 sissif     (501) staff       (20)    11415 2023-06-30 14:39:45.000000 easy_tpp-0.0.3/LICENCE
--rw-rw-r--   0 sissif     (501) staff       (20)      704 2023-06-30 14:39:45.000000 easy_tpp-0.0.3/NOTICE
--rw-r--r--   0 sissif     (501) staff       (20)      227 2023-07-02 03:19:21.000000 easy_tpp-0.0.3/PKG-INFO
--rw-rw-r--   0 sissif     (501) staff       (20)     9479 2023-06-30 14:39:45.000000 easy_tpp-0.0.3/README.md
-drwxr-xr-x   0 sissif     (501) staff       (20)        0 2023-07-02 03:19:21.000000 easy_tpp-0.0.3/easy_tpp/
--rw-rw-r--   0 sissif     (501) staff       (20)       21 2023-06-30 14:39:45.000000 easy_tpp-0.0.3/easy_tpp/__init__.py
-drwxr-xr-x   0 sissif     (501) staff       (20)        0 2023-07-02 03:19:21.000000 easy_tpp-0.0.3/easy_tpp/config_factory/
--rw-rw-r--   0 sissif     (501) staff       (20)      495 2023-06-30 14:39:45.000000 easy_tpp-0.0.3/easy_tpp/config_factory/__init__.py
--rw-rw-r--   0 sissif     (501) staff       (20)     2801 2023-06-30 14:39:45.000000 easy_tpp-0.0.3/easy_tpp/config_factory/base_config.py
--rw-rw-r--   0 sissif     (501) staff       (20)     3067 2023-06-30 14:39:45.000000 easy_tpp-0.0.3/easy_tpp/config_factory/config.py
--rw-rw-r--   0 sissif     (501) staff       (20)     5165 2023-06-30 14:39:45.000000 easy_tpp-0.0.3/easy_tpp/config_factory/data_config.py
--rw-rw-r--   0 sissif     (501) staff       (20)     4347 2023-06-30 14:39:45.000000 easy_tpp-0.0.3/easy_tpp/config_factory/hpo_config.py
--rw-rw-r--   0 sissif     (501) staff       (20)    10944 2023-06-30 14:39:45.000000 easy_tpp-0.0.3/easy_tpp/config_factory/model_config.py
--rw-rw-r--   0 sissif     (501) staff       (20)     7723 2023-06-30 14:39:45.000000 easy_tpp-0.0.3/easy_tpp/config_factory/runner_config.py
-drwxr-xr-x   0 sissif     (501) staff       (20)        0 2023-07-02 03:19:21.000000 easy_tpp-0.0.3/easy_tpp/default_registers/
--rw-rw-r--   0 sissif     (501) staff       (20)        0 2023-06-30 14:39:45.000000 easy_tpp-0.0.3/easy_tpp/default_registers/__init__.py
--rw-rw-r--   0 sissif     (501) staff       (20)     1432 2023-06-30 14:39:45.000000 easy_tpp-0.0.3/easy_tpp/default_registers/register_metrics.py
--rw-rw-r--   0 sissif     (501) staff       (20)      512 2023-06-30 14:39:45.000000 easy_tpp-0.0.3/easy_tpp/default_registers/register_optuna_trials.py
-drwxr-xr-x   0 sissif     (501) staff       (20)        0 2023-07-02 03:19:21.000000 easy_tpp-0.0.3/easy_tpp/hpo/
--rw-rw-r--   0 sissif     (501) staff       (20)      208 2023-06-30 14:39:45.000000 easy_tpp-0.0.3/easy_tpp/hpo/__init__.py
--rw-rw-r--   0 sissif     (501) staff       (20)     4143 2023-06-30 14:39:45.000000 easy_tpp-0.0.3/easy_tpp/hpo/base_hpo.py
--rw-rw-r--   0 sissif     (501) staff       (20)    13912 2023-06-30 14:39:45.000000 easy_tpp-0.0.3/easy_tpp/hpo/optuna_hpo.py
-drwxr-xr-x   0 sissif     (501) staff       (20)        0 2023-07-02 03:19:21.000000 easy_tpp-0.0.3/easy_tpp/model/
--rw-rw-r--   0 sissif     (501) staff       (20)     1950 2023-06-30 14:39:45.000000 easy_tpp-0.0.3/easy_tpp/model/__init__.py
-drwxr-xr-x   0 sissif     (501) staff       (20)        0 2023-07-02 03:19:21.000000 easy_tpp-0.0.3/easy_tpp/model/tf_model/
--rw-rw-r--   0 sissif     (501) staff       (20)        0 2023-06-30 14:39:45.000000 easy_tpp-0.0.3/easy_tpp/model/tf_model/__init__.py
--rw-rw-r--   0 sissif     (501) staff       (20)    15311 2023-06-30 14:39:45.000000 easy_tpp-0.0.3/easy_tpp/model/tf_model/tf_anhn.py
--rw-rw-r--   0 sissif     (501) staff       (20)    14714 2023-06-30 14:39:45.000000 easy_tpp-0.0.3/easy_tpp/model/tf_model/tf_attnhp.py
--rw-rw-r--   0 sissif     (501) staff       (20)    14993 2023-06-30 14:39:45.000000 easy_tpp-0.0.3/easy_tpp/model/tf_model/tf_baselayer.py
--rw-rw-r--   0 sissif     (501) staff       (20)    11994 2023-06-30 14:39:45.000000 easy_tpp-0.0.3/easy_tpp/model/tf_model/tf_basemodel.py
--rw-rw-r--   0 sissif     (501) staff       (20)     9485 2023-06-30 14:39:45.000000 easy_tpp-0.0.3/easy_tpp/model/tf_model/tf_fullynn.py
--rw-rw-r--   0 sissif     (501) staff       (20)     7868 2023-06-30 14:39:45.000000 easy_tpp-0.0.3/easy_tpp/model/tf_model/tf_intensity_free.py
--rw-rw-r--   0 sissif     (501) staff       (20)    13935 2023-06-30 14:39:45.000000 easy_tpp-0.0.3/easy_tpp/model/tf_model/tf_nhp.py
--rw-rw-r--   0 sissif     (501) staff       (20)    14001 2023-06-30 14:39:45.000000 easy_tpp-0.0.3/easy_tpp/model/tf_model/tf_ode_tpp.py
--rw-rw-r--   0 sissif     (501) staff       (20)     8575 2023-06-30 14:39:45.000000 easy_tpp-0.0.3/easy_tpp/model/tf_model/tf_rmtpp.py
--rw-rw-r--   0 sissif     (501) staff       (20)    10020 2023-06-30 14:39:45.000000 easy_tpp-0.0.3/easy_tpp/model/tf_model/tf_sahp.py
--rw-rw-r--   0 sissif     (501) staff       (20)     9178 2023-06-30 14:39:45.000000 easy_tpp-0.0.3/easy_tpp/model/tf_model/tf_thinning.py
--rw-rw-r--   0 sissif     (501) staff       (20)     9361 2023-06-30 14:39:45.000000 easy_tpp-0.0.3/easy_tpp/model/tf_model/tf_thp.py
-drwxr-xr-x   0 sissif     (501) staff       (20)        0 2023-07-02 03:19:21.000000 easy_tpp-0.0.3/easy_tpp/model/torch_model/
--rw-rw-r--   0 sissif     (501) staff       (20)        0 2023-06-30 14:39:45.000000 easy_tpp-0.0.3/easy_tpp/model/torch_model/__init__.py
--rw-rw-r--   0 sissif     (501) staff       (20)    12246 2023-06-30 14:39:45.000000 easy_tpp-0.0.3/easy_tpp/model/torch_model/torch_anhn.py
--rw-rw-r--   0 sissif     (501) staff       (20)    14471 2023-06-30 14:39:45.000000 easy_tpp-0.0.3/easy_tpp/model/torch_model/torch_attnhp.py
--rw-rw-r--   0 sissif     (501) staff       (20)     8860 2023-06-30 14:39:45.000000 easy_tpp-0.0.3/easy_tpp/model/torch_model/torch_baselayer.py
--rw-rw-r--   0 sissif     (501) staff       (20)    11617 2023-06-30 14:39:45.000000 easy_tpp-0.0.3/easy_tpp/model/torch_model/torch_basemodel.py
--rw-rw-r--   0 sissif     (501) staff       (20)     8562 2023-06-30 14:39:45.000000 easy_tpp-0.0.3/easy_tpp/model/torch_model/torch_fullynn.py
--rw-rw-r--   0 sissif     (501) staff       (20)     8085 2023-06-30 14:39:45.000000 easy_tpp-0.0.3/easy_tpp/model/torch_model/torch_intensity_free.py
--rw-rw-r--   0 sissif     (501) staff       (20)    14572 2023-06-30 14:39:45.000000 easy_tpp-0.0.3/easy_tpp/model/torch_model/torch_nhp.py
--rw-rw-r--   0 sissif     (501) staff       (20)    11244 2023-06-30 14:39:45.000000 easy_tpp-0.0.3/easy_tpp/model/torch_model/torch_ode_tpp.py
--rw-rw-r--   0 sissif     (501) staff       (20)     7765 2023-06-30 14:39:45.000000 easy_tpp-0.0.3/easy_tpp/model/torch_model/torch_rmtpp.py
--rw-rw-r--   0 sissif     (501) staff       (20)     8815 2023-06-30 14:39:45.000000 easy_tpp-0.0.3/easy_tpp/model/torch_model/torch_sahp.py
--rw-rw-r--   0 sissif     (501) staff       (20)    10684 2023-06-30 14:39:45.000000 easy_tpp-0.0.3/easy_tpp/model/torch_model/torch_thinning.py
--rw-rw-r--   0 sissif     (501) staff       (20)     7873 2023-06-30 14:39:45.000000 easy_tpp-0.0.3/easy_tpp/model/torch_model/torch_thp.py
-drwxr-xr-x   0 sissif     (501) staff       (20)        0 2023-07-02 03:19:21.000000 easy_tpp-0.0.3/easy_tpp/preprocess/
--rw-rw-r--   0 sissif     (501) staff       (20)      216 2023-06-30 14:39:45.000000 easy_tpp-0.0.3/easy_tpp/preprocess/__init__.py
--rw-rw-r--   0 sissif     (501) staff       (20)     1982 2023-06-30 14:39:45.000000 easy_tpp-0.0.3/easy_tpp/preprocess/data_collator.py
--rw-rw-r--   0 sissif     (501) staff       (20)     3217 2023-06-30 14:39:45.000000 easy_tpp-0.0.3/easy_tpp/preprocess/data_loader.py
--rw-rw-r--   0 sissif     (501) staff       (20)     5048 2023-06-30 14:39:45.000000 easy_tpp-0.0.3/easy_tpp/preprocess/dataset.py
--rw-rw-r--   0 sissif     (501) staff       (20)    25680 2023-06-30 14:39:45.000000 easy_tpp-0.0.3/easy_tpp/preprocess/event_tokenizer.py
-drwxr-xr-x   0 sissif     (501) staff       (20)        0 2023-07-02 03:19:21.000000 easy_tpp-0.0.3/easy_tpp/runner/
--rw-rw-r--   0 sissif     (501) staff       (20)      237 2023-06-30 14:39:45.000000 easy_tpp-0.0.3/easy_tpp/runner/__init__.py
--rw-rw-r--   0 sissif     (501) staff       (20)     6416 2023-06-30 14:39:45.000000 easy_tpp-0.0.3/easy_tpp/runner/base_runner.py
--rw-rw-r--   0 sissif     (501) staff       (20)     8761 2023-06-30 14:39:45.000000 easy_tpp-0.0.3/easy_tpp/runner/tpp_runner.py
--rw-rw-r--   0 sissif     (501) staff       (20)     6201 2023-06-30 14:39:45.000000 easy_tpp-0.0.3/easy_tpp/tf_wrapper.py
--rw-rw-r--   0 sissif     (501) staff       (20)     5704 2023-06-30 14:39:45.000000 easy_tpp-0.0.3/easy_tpp/torch_wrapper.py
-drwxr-xr-x   0 sissif     (501) staff       (20)        0 2023-07-02 03:19:21.000000 easy_tpp-0.0.3/easy_tpp/utils/
--rw-rw-r--   0 sissif     (501) staff       (20)     2462 2023-06-30 14:39:45.000000 easy_tpp-0.0.3/easy_tpp/utils/__init__.py
--rw-rw-r--   0 sissif     (501) staff       (20)     2166 2023-06-30 14:39:45.000000 easy_tpp-0.0.3/easy_tpp/utils/const.py
--rw-rw-r--   0 sissif     (501) staff       (20)     2419 2023-06-30 14:39:45.000000 easy_tpp-0.0.3/easy_tpp/utils/generic.py
--rw-rw-r--   0 sissif     (501) staff       (20)     7459 2023-06-30 14:39:45.000000 easy_tpp-0.0.3/easy_tpp/utils/import_utils.py
--rw-rw-r--   0 sissif     (501) staff       (20)     1435 2023-06-30 14:39:45.000000 easy_tpp-0.0.3/easy_tpp/utils/log_utils.py
--rw-rw-r--   0 sissif     (501) staff       (20)     3333 2023-06-30 14:39:45.000000 easy_tpp-0.0.3/easy_tpp/utils/metrics.py
--rw-rw-r--   0 sissif     (501) staff       (20)     6890 2023-06-30 14:39:45.000000 easy_tpp-0.0.3/easy_tpp/utils/misc.py
--rw-rw-r--   0 sissif     (501) staff       (20)     2887 2023-06-30 14:39:45.000000 easy_tpp-0.0.3/easy_tpp/utils/multiprocess_utils.py
--rw-rw-r--   0 sissif     (501) staff       (20)     2700 2023-06-30 14:39:45.000000 easy_tpp-0.0.3/easy_tpp/utils/ode_utils.py
--rw-rw-r--   0 sissif     (501) staff       (20)     7118 2023-06-30 14:39:45.000000 easy_tpp-0.0.3/easy_tpp/utils/registrable.py
--rw-rw-r--   0 sissif     (501) staff       (20)     3150 2023-06-30 14:39:45.000000 easy_tpp-0.0.3/easy_tpp/utils/tf_utils.py
--rw-rw-r--   0 sissif     (501) staff       (20)     1856 2023-06-30 14:39:45.000000 easy_tpp-0.0.3/easy_tpp/utils/torch_utils.py
-drwxr-xr-x   0 sissif     (501) staff       (20)        0 2023-07-02 03:19:21.000000 easy_tpp-0.0.3/easy_tpp.egg-info/
--rw-r--r--   0 sissif     (501) staff       (20)      227 2023-07-02 03:19:21.000000 easy_tpp-0.0.3/easy_tpp.egg-info/PKG-INFO
--rw-r--r--   0 sissif     (501) staff       (20)     2431 2023-07-02 03:19:21.000000 easy_tpp-0.0.3/easy_tpp.egg-info/SOURCES.txt
--rw-r--r--   0 sissif     (501) staff       (20)        1 2023-07-02 03:19:21.000000 easy_tpp-0.0.3/easy_tpp.egg-info/dependency_links.txt
--rw-r--r--   0 sissif     (501) staff       (20)       31 2023-07-02 03:19:21.000000 easy_tpp-0.0.3/easy_tpp.egg-info/requires.txt
--rw-r--r--   0 sissif     (501) staff       (20)        9 2023-07-02 03:19:21.000000 easy_tpp-0.0.3/easy_tpp.egg-info/top_level.txt
--rw-r--r--   0 sissif     (501) staff       (20)       79 2023-07-02 03:19:21.000000 easy_tpp-0.0.3/setup.cfg
--rw-rw-r--   0 sissif     (501) staff       (20)     1728 2023-07-02 03:19:08.000000 easy_tpp-0.0.3/setup.py
+drwxr-xr-x   0 sissif     (501) staff       (20)        0 2023-07-02 03:53:02.000000 easy_tpp-0.0.4/
+-rw-rw-r--   0 sissif     (501) staff       (20)    11415 2023-07-02 03:47:06.000000 easy_tpp-0.0.4/LICENCE
+-rw-rw-r--   0 sissif     (501) staff       (20)       43 2023-07-02 03:47:06.000000 easy_tpp-0.0.4/MANIFEST.in
+-rw-rw-r--   0 sissif     (501) staff       (20)      704 2023-07-02 03:47:06.000000 easy_tpp-0.0.4/NOTICE
+-rw-r--r--   0 sissif     (501) staff       (20)      296 2023-07-02 03:53:02.000000 easy_tpp-0.0.4/PKG-INFO
+-rw-rw-r--   0 sissif     (501) staff       (20)    12168 2023-07-02 03:47:06.000000 easy_tpp-0.0.4/README.md
+drwxr-xr-x   0 sissif     (501) staff       (20)        0 2023-07-02 03:53:02.000000 easy_tpp-0.0.4/easy_tpp/
+-rw-rw-r--   0 sissif     (501) staff       (20)       21 2023-07-02 03:47:06.000000 easy_tpp-0.0.4/easy_tpp/__init__.py
+drwxr-xr-x   0 sissif     (501) staff       (20)        0 2023-07-02 03:53:02.000000 easy_tpp-0.0.4/easy_tpp/config_factory/
+-rw-rw-r--   0 sissif     (501) staff       (20)      495 2023-07-02 03:47:06.000000 easy_tpp-0.0.4/easy_tpp/config_factory/__init__.py
+-rw-rw-r--   0 sissif     (501) staff       (20)     2801 2023-07-02 03:47:06.000000 easy_tpp-0.0.4/easy_tpp/config_factory/base_config.py
+-rw-rw-r--   0 sissif     (501) staff       (20)     3067 2023-07-02 03:47:06.000000 easy_tpp-0.0.4/easy_tpp/config_factory/config.py
+-rw-rw-r--   0 sissif     (501) staff       (20)     5165 2023-07-02 03:47:06.000000 easy_tpp-0.0.4/easy_tpp/config_factory/data_config.py
+-rw-rw-r--   0 sissif     (501) staff       (20)     4347 2023-07-02 03:47:06.000000 easy_tpp-0.0.4/easy_tpp/config_factory/hpo_config.py
+-rw-rw-r--   0 sissif     (501) staff       (20)    10944 2023-07-02 03:47:06.000000 easy_tpp-0.0.4/easy_tpp/config_factory/model_config.py
+-rw-rw-r--   0 sissif     (501) staff       (20)     7723 2023-07-02 03:47:06.000000 easy_tpp-0.0.4/easy_tpp/config_factory/runner_config.py
+drwxr-xr-x   0 sissif     (501) staff       (20)        0 2023-07-02 03:53:02.000000 easy_tpp-0.0.4/easy_tpp/default_registers/
+-rw-rw-r--   0 sissif     (501) staff       (20)        0 2023-07-02 03:47:06.000000 easy_tpp-0.0.4/easy_tpp/default_registers/__init__.py
+-rw-rw-r--   0 sissif     (501) staff       (20)     1432 2023-07-02 03:47:06.000000 easy_tpp-0.0.4/easy_tpp/default_registers/register_metrics.py
+-rw-rw-r--   0 sissif     (501) staff       (20)      512 2023-07-02 03:47:06.000000 easy_tpp-0.0.4/easy_tpp/default_registers/register_optuna_trials.py
+drwxr-xr-x   0 sissif     (501) staff       (20)        0 2023-07-02 03:53:02.000000 easy_tpp-0.0.4/easy_tpp/hpo/
+-rw-rw-r--   0 sissif     (501) staff       (20)      208 2023-07-02 03:47:06.000000 easy_tpp-0.0.4/easy_tpp/hpo/__init__.py
+-rw-rw-r--   0 sissif     (501) staff       (20)     4143 2023-07-02 03:47:06.000000 easy_tpp-0.0.4/easy_tpp/hpo/base_hpo.py
+-rw-rw-r--   0 sissif     (501) staff       (20)    13912 2023-07-02 03:47:06.000000 easy_tpp-0.0.4/easy_tpp/hpo/optuna_hpo.py
+drwxr-xr-x   0 sissif     (501) staff       (20)        0 2023-07-02 03:53:02.000000 easy_tpp-0.0.4/easy_tpp/model/
+-rw-rw-r--   0 sissif     (501) staff       (20)     1950 2023-07-02 03:47:06.000000 easy_tpp-0.0.4/easy_tpp/model/__init__.py
+drwxr-xr-x   0 sissif     (501) staff       (20)        0 2023-07-02 03:53:02.000000 easy_tpp-0.0.4/easy_tpp/model/tf_model/
+-rw-rw-r--   0 sissif     (501) staff       (20)        0 2023-07-02 03:47:06.000000 easy_tpp-0.0.4/easy_tpp/model/tf_model/__init__.py
+-rw-rw-r--   0 sissif     (501) staff       (20)    15311 2023-07-02 03:47:06.000000 easy_tpp-0.0.4/easy_tpp/model/tf_model/tf_anhn.py
+-rw-rw-r--   0 sissif     (501) staff       (20)    14714 2023-07-02 03:47:06.000000 easy_tpp-0.0.4/easy_tpp/model/tf_model/tf_attnhp.py
+-rw-rw-r--   0 sissif     (501) staff       (20)    14993 2023-07-02 03:47:06.000000 easy_tpp-0.0.4/easy_tpp/model/tf_model/tf_baselayer.py
+-rw-rw-r--   0 sissif     (501) staff       (20)    11994 2023-07-02 03:47:06.000000 easy_tpp-0.0.4/easy_tpp/model/tf_model/tf_basemodel.py
+-rw-rw-r--   0 sissif     (501) staff       (20)     9485 2023-07-02 03:47:06.000000 easy_tpp-0.0.4/easy_tpp/model/tf_model/tf_fullynn.py
+-rw-rw-r--   0 sissif     (501) staff       (20)     7868 2023-07-02 03:47:06.000000 easy_tpp-0.0.4/easy_tpp/model/tf_model/tf_intensity_free.py
+-rw-rw-r--   0 sissif     (501) staff       (20)    13935 2023-07-02 03:47:06.000000 easy_tpp-0.0.4/easy_tpp/model/tf_model/tf_nhp.py
+-rw-rw-r--   0 sissif     (501) staff       (20)    14001 2023-07-02 03:47:06.000000 easy_tpp-0.0.4/easy_tpp/model/tf_model/tf_ode_tpp.py
+-rw-rw-r--   0 sissif     (501) staff       (20)     8575 2023-07-02 03:47:06.000000 easy_tpp-0.0.4/easy_tpp/model/tf_model/tf_rmtpp.py
+-rw-rw-r--   0 sissif     (501) staff       (20)    10020 2023-07-02 03:47:06.000000 easy_tpp-0.0.4/easy_tpp/model/tf_model/tf_sahp.py
+-rw-rw-r--   0 sissif     (501) staff       (20)     9178 2023-07-02 03:47:06.000000 easy_tpp-0.0.4/easy_tpp/model/tf_model/tf_thinning.py
+-rw-rw-r--   0 sissif     (501) staff       (20)     9361 2023-07-02 03:47:06.000000 easy_tpp-0.0.4/easy_tpp/model/tf_model/tf_thp.py
+drwxr-xr-x   0 sissif     (501) staff       (20)        0 2023-07-02 03:53:02.000000 easy_tpp-0.0.4/easy_tpp/model/torch_model/
+-rw-rw-r--   0 sissif     (501) staff       (20)        0 2023-07-02 03:47:06.000000 easy_tpp-0.0.4/easy_tpp/model/torch_model/__init__.py
+-rw-rw-r--   0 sissif     (501) staff       (20)    12246 2023-07-02 03:47:06.000000 easy_tpp-0.0.4/easy_tpp/model/torch_model/torch_anhn.py
+-rw-rw-r--   0 sissif     (501) staff       (20)    14471 2023-07-02 03:47:06.000000 easy_tpp-0.0.4/easy_tpp/model/torch_model/torch_attnhp.py
+-rw-rw-r--   0 sissif     (501) staff       (20)     8860 2023-07-02 03:47:06.000000 easy_tpp-0.0.4/easy_tpp/model/torch_model/torch_baselayer.py
+-rw-rw-r--   0 sissif     (501) staff       (20)    11617 2023-07-02 03:47:06.000000 easy_tpp-0.0.4/easy_tpp/model/torch_model/torch_basemodel.py
+-rw-rw-r--   0 sissif     (501) staff       (20)     8562 2023-07-02 03:47:06.000000 easy_tpp-0.0.4/easy_tpp/model/torch_model/torch_fullynn.py
+-rw-rw-r--   0 sissif     (501) staff       (20)     8085 2023-07-02 03:47:06.000000 easy_tpp-0.0.4/easy_tpp/model/torch_model/torch_intensity_free.py
+-rw-rw-r--   0 sissif     (501) staff       (20)    14572 2023-07-02 03:47:06.000000 easy_tpp-0.0.4/easy_tpp/model/torch_model/torch_nhp.py
+-rw-rw-r--   0 sissif     (501) staff       (20)    11244 2023-07-02 03:47:06.000000 easy_tpp-0.0.4/easy_tpp/model/torch_model/torch_ode_tpp.py
+-rw-rw-r--   0 sissif     (501) staff       (20)     7765 2023-07-02 03:47:06.000000 easy_tpp-0.0.4/easy_tpp/model/torch_model/torch_rmtpp.py
+-rw-rw-r--   0 sissif     (501) staff       (20)     8815 2023-07-02 03:47:06.000000 easy_tpp-0.0.4/easy_tpp/model/torch_model/torch_sahp.py
+-rw-rw-r--   0 sissif     (501) staff       (20)    10684 2023-07-02 03:47:06.000000 easy_tpp-0.0.4/easy_tpp/model/torch_model/torch_thinning.py
+-rw-rw-r--   0 sissif     (501) staff       (20)     7873 2023-07-02 03:47:06.000000 easy_tpp-0.0.4/easy_tpp/model/torch_model/torch_thp.py
+drwxr-xr-x   0 sissif     (501) staff       (20)        0 2023-07-02 03:53:02.000000 easy_tpp-0.0.4/easy_tpp/preprocess/
+-rw-rw-r--   0 sissif     (501) staff       (20)      216 2023-07-02 03:47:06.000000 easy_tpp-0.0.4/easy_tpp/preprocess/__init__.py
+-rw-rw-r--   0 sissif     (501) staff       (20)     1982 2023-07-02 03:47:06.000000 easy_tpp-0.0.4/easy_tpp/preprocess/data_collator.py
+-rw-rw-r--   0 sissif     (501) staff       (20)     3217 2023-07-02 03:47:06.000000 easy_tpp-0.0.4/easy_tpp/preprocess/data_loader.py
+-rw-rw-r--   0 sissif     (501) staff       (20)     5048 2023-07-02 03:47:06.000000 easy_tpp-0.0.4/easy_tpp/preprocess/dataset.py
+-rw-rw-r--   0 sissif     (501) staff       (20)    25680 2023-07-02 03:47:06.000000 easy_tpp-0.0.4/easy_tpp/preprocess/event_tokenizer.py
+drwxr-xr-x   0 sissif     (501) staff       (20)        0 2023-07-02 03:53:02.000000 easy_tpp-0.0.4/easy_tpp/runner/
+-rw-rw-r--   0 sissif     (501) staff       (20)      237 2023-07-02 03:47:06.000000 easy_tpp-0.0.4/easy_tpp/runner/__init__.py
+-rw-rw-r--   0 sissif     (501) staff       (20)     6416 2023-07-02 03:47:06.000000 easy_tpp-0.0.4/easy_tpp/runner/base_runner.py
+-rw-rw-r--   0 sissif     (501) staff       (20)     8761 2023-07-02 03:47:06.000000 easy_tpp-0.0.4/easy_tpp/runner/tpp_runner.py
+-rw-rw-r--   0 sissif     (501) staff       (20)     6201 2023-07-02 03:47:06.000000 easy_tpp-0.0.4/easy_tpp/tf_wrapper.py
+-rw-rw-r--   0 sissif     (501) staff       (20)     5704 2023-07-02 03:47:06.000000 easy_tpp-0.0.4/easy_tpp/torch_wrapper.py
+drwxr-xr-x   0 sissif     (501) staff       (20)        0 2023-07-02 03:53:02.000000 easy_tpp-0.0.4/easy_tpp/utils/
+-rw-rw-r--   0 sissif     (501) staff       (20)     2462 2023-07-02 03:47:06.000000 easy_tpp-0.0.4/easy_tpp/utils/__init__.py
+-rw-rw-r--   0 sissif     (501) staff       (20)     2166 2023-07-02 03:47:06.000000 easy_tpp-0.0.4/easy_tpp/utils/const.py
+-rw-rw-r--   0 sissif     (501) staff       (20)     2419 2023-07-02 03:47:06.000000 easy_tpp-0.0.4/easy_tpp/utils/generic.py
+-rw-rw-r--   0 sissif     (501) staff       (20)     7459 2023-07-02 03:47:06.000000 easy_tpp-0.0.4/easy_tpp/utils/import_utils.py
+-rw-rw-r--   0 sissif     (501) staff       (20)     1435 2023-07-02 03:47:06.000000 easy_tpp-0.0.4/easy_tpp/utils/log_utils.py
+-rw-rw-r--   0 sissif     (501) staff       (20)     3333 2023-07-02 03:47:06.000000 easy_tpp-0.0.4/easy_tpp/utils/metrics.py
+-rw-rw-r--   0 sissif     (501) staff       (20)     6890 2023-07-02 03:47:06.000000 easy_tpp-0.0.4/easy_tpp/utils/misc.py
+-rw-rw-r--   0 sissif     (501) staff       (20)     2887 2023-07-02 03:47:06.000000 easy_tpp-0.0.4/easy_tpp/utils/multiprocess_utils.py
+-rw-rw-r--   0 sissif     (501) staff       (20)     2700 2023-07-02 03:47:06.000000 easy_tpp-0.0.4/easy_tpp/utils/ode_utils.py
+-rw-rw-r--   0 sissif     (501) staff       (20)     7118 2023-07-02 03:47:06.000000 easy_tpp-0.0.4/easy_tpp/utils/registrable.py
+-rw-rw-r--   0 sissif     (501) staff       (20)     3150 2023-07-02 03:47:06.000000 easy_tpp-0.0.4/easy_tpp/utils/tf_utils.py
+-rw-rw-r--   0 sissif     (501) staff       (20)     1856 2023-07-02 03:47:06.000000 easy_tpp-0.0.4/easy_tpp/utils/torch_utils.py
+drwxr-xr-x   0 sissif     (501) staff       (20)        0 2023-07-02 03:53:02.000000 easy_tpp-0.0.4/easy_tpp.egg-info/
+-rw-r--r--   0 sissif     (501) staff       (20)      296 2023-07-02 03:53:02.000000 easy_tpp-0.0.4/easy_tpp.egg-info/PKG-INFO
+-rw-r--r--   0 sissif     (501) staff       (20)     2471 2023-07-02 03:53:02.000000 easy_tpp-0.0.4/easy_tpp.egg-info/SOURCES.txt
+-rw-r--r--   0 sissif     (501) staff       (20)        1 2023-07-02 03:53:02.000000 easy_tpp-0.0.4/easy_tpp.egg-info/dependency_links.txt
+-rw-r--r--   0 sissif     (501) staff       (20)       31 2023-07-02 03:53:02.000000 easy_tpp-0.0.4/easy_tpp.egg-info/requires.txt
+-rw-r--r--   0 sissif     (501) staff       (20)        9 2023-07-02 03:53:02.000000 easy_tpp-0.0.4/easy_tpp.egg-info/top_level.txt
+-rw-rw-r--   0 sissif     (501) staff       (20)       30 2023-07-02 03:47:06.000000 easy_tpp-0.0.4/requirements.txt
+-rw-rw-r--   0 sissif     (501) staff       (20)       79 2023-07-02 03:53:02.000000 easy_tpp-0.0.4/setup.cfg
+-rw-rw-r--   0 sissif     (501) staff       (20)     1838 2023-07-02 03:47:06.000000 easy_tpp-0.0.4/setup.py
+-rw-rw-r--   0 sissif     (501) staff       (20)       22 2023-07-02 03:47:06.000000 easy_tpp-0.0.4/version.py
```

### Comparing `easy_tpp-0.0.3/LICENCE` & `easy_tpp-0.0.4/LICENCE`

 * *Files identical despite different names*

### Comparing `easy_tpp-0.0.3/NOTICE` & `easy_tpp-0.0.4/NOTICE`

 * *Files identical despite different names*

### Comparing `easy_tpp-0.0.3/README.md` & `easy_tpp-0.0.4/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # EasyTPP
 
 ![Python 3.9+](https://img.shields.io/badge/python-3.9+-blue.svg)
 ![](https://img.shields.io/badge/license-Apache-000000.svg)
 ![PRs Welcome](https://img.shields.io/badge/PRs-Welcome-green) 
 ![GitHub last commit](https://img.shields.io/github/last-commit/ant-research/EasyTemporalPointProcess)
 ![Stars](https://img.shields.io/github/stars/ant-research/EasyTemporalPointProcess)
+[![PyPI version fury.io](https://badge.fury.io/py/easy-tpp.svg)](https://pypi.python.org/pypi/easy-tpp/)
+[![Downloads](https://pepy.tech/badge/easy-tpp)](https://pepy.tech/project/easy-tpp)
 
 ** We are actively updating the repo now. We will try to finish the first version in a few days. **
 
 `EasyTPP` is an easy-to-use development and application toolkit for [Temporal Point Process](https://mathworld.wolfram.com/TemporalPointProcess.html) (TPP), with key features in configurability, compatibility and reproducibility. We hope this project could benefit both researchers and practitioners with the goal of easily customized development and open benchmarking in TPP.
 <span id='top'/>
 
 
@@ -66,14 +68,96 @@
 - Amazon ([Amazon Review, 2018](https://nijianmo.github.io/amazon/)): timestamped user online shopping behavior events in Amazon platform.
 
   All datasets are preprocess to the `Gatech` format dataset widely used for TPP researchers, and saved at [Google Drive](https://drive.google.com/drive/u/0/folders/1f8k82-NL6KFKuNMsUwozmbzDSFycYvz7) with a public access.
 
 ## Quick Start <a href='#top'>[Back to Top]</a>
 <span id='quick-start'/>
 
+We provide an end-to-end example for users to run a standard TPP model with `EasyTPP`.
+
+
+### Step 1. Installation
+
+First of all, we can install the package either by using pip or from the source code on Github.
+
+To install the latest stable version:
+```bash
+pip install easy-tpp
+```
+
+To install the latest on GitHub:
+```bash
+git clone https://github.com/ant-research/EasyTemporalPointProcess.git
+cd EasyTemporalPointProcess
+python setup.py install
+```
+
+
+### Step 2. Prepare datasets 
+
+We need to put the datasets in a local directory before running a model and the datasets should follow a certain format. See [OnlineDoc - Datasets](https://ant-research.github.io/EasyTemporalPointProcess/user_guide/dataset.html) for more details.
+
+Suppose we use the [taxi dataset](https://chriswhong.com/open-data/foil_nyc_taxi/) in the example.
+
+### Step 3. Train the model
+
+
+Before start training, we need to set up the config file for the pipeline. We provide a preset config file in [Example Config](https://github.com/ant-research/EasyTemporalPointProcess/blob/main/examples/configs/experiment_config.yaml). The details of the configuration can be found in [OnlineDoc - Training Pipeline](https://ant-research.github.io/EasyTemporalPointProcess/user_guide/run_train_pipeline.html).
+
+After the setup of data and config, the directory structure is as follows:
+
+```bash
+
+    data
+     |______taxi
+             |____ train.pkl
+             |____ dev.pkl
+             |____ test.pkl
+
+    configs
+     |______experiment_config.yaml
+
+```
+
+
+Then we start the training by simply running the script 
+
+```python
+
+import argparse
+from easy_tpp.config_factory import Config
+from easy_tpp.runner import Runner
+
+
+def main():
+    parser = argparse.ArgumentParser()
+
+    parser.add_argument('--config_dir', type=str, required=False, default='configs/experiment_config.yaml',
+                        help='Dir of configuration yaml to train and evaluate the model.')
+
+    parser.add_argument('--experiment_id', type=str, required=False, default='NHP_train',
+                        help='Experiment id in the config file.')
+
+    args = parser.parse_args()
+
+    config = Config.build_from_yaml_file(args.config_dir, experiment_id=args.experiment_id)
+
+    model_runner = Runner.build_from_config(config)
+
+    model_runner.run()
+
+
+if __name__ == '__main__':
+    main()
+
+```
+
+A more detailed example can be found at [OnlineDoc - QuickStart](https://ant-research.github.io/EasyTemporalPointProcess/get_started/quick_start.html).
+
+
 ## Documentation <a href='#top'>[Back to Top]</a>
 <span id='doc'/>
 
 The classes and methods of `EasyTPP` have been well documented so that users can generate the documentation by:
 
 ```shell
 cd doc
```

#### html2text {}

```diff
@@ -1,21 +1,24 @@
 # EasyTPP ![Python 3.9+](https://img.shields.io/badge/python-3.9+-blue.svg) ![]
 (https://img.shields.io/badge/license-Apache-000000.svg) ![PRs Welcome](https:/
 /img.shields.io/badge/PRs-Welcome-green) ![GitHub last commit](https://
 img.shields.io/github/last-commit/ant-research/EasyTemporalPointProcess) !
 [Stars](https://img.shields.io/github/stars/ant-research/
-EasyTemporalPointProcess) ** We are actively updating the repo now. We will try
-to finish the first version in a few days. ** `EasyTPP` is an easy-to-use
-development and application toolkit for [Temporal Point Process](https://
-mathworld.wolfram.com/TemporalPointProcess.html) (TPP), with key features in
-configurability, compatibility and reproducibility. We hope this project could
-benefit both researchers and practitioners with the goal of easily customized
-development and open benchmarking in TPP.  | Features|Install | Model_List |
-Dataset | Quick_Start | Documentation | Citation |Acknowledgement | Star
-History | ## News  - ![new](https://img.alicdn.com/imgextra/i4/
+EasyTemporalPointProcess) [![PyPI version fury.io](https://badge.fury.io/py/
+easy-tpp.svg)](https://pypi.python.org/pypi/easy-tpp/) [![Downloads](https://
+pepy.tech/badge/easy-tpp)](https://pepy.tech/project/easy-tpp) ** We are
+actively updating the repo now. We will try to finish the first version in a
+few days. ** `EasyTPP` is an easy-to-use development and application toolkit
+for [Temporal Point Process](https://mathworld.wolfram.com/
+TemporalPointProcess.html) (TPP), with key features in configurability,
+compatibility and reproducibility. We hope this project could benefit both
+researchers and practitioners with the goal of easily customized development
+and open benchmarking in TPP.  | Features|Install | Model_List | Dataset |
+Quick_Start | Documentation | Citation |Acknowledgement | Star_History | ##
+News  - ![new](https://img.alicdn.com/imgextra/i4/
 O1CN01kUiDtl1HVxN6G56vN_!!6000000000764-2-tps-43-19.png) [06-22-2023] Our paper
 [Language Model Can Improve Event Prediction by Few-Shot Abductive Reasoning]
 (https://arxiv.org/abs/2305.16646) is accepted by the [Knowledge and Logical
 Reasoning Workshop, ICML'2023](https://klr-icml2023.github.io/cfp.html)! - !
 [new](https://img.alicdn.com/imgextra/i4/
 O1CN01kUiDtl1HVxN6G56vN_!!6000000000764-2-tps-43-19.png) [05-29-2023] We
 release ``EasyTPP`` v0.0.1! - [12-27-2022] Our paper [Bellman Meets Hawkes:
@@ -79,15 +82,46 @@
 reward events in StackOverflow. - Taobao ([Xue et al, 2022](https://arxiv.org/
 abs/2210.01753)): timestamped user online shopping behavior events in Taobao
 platform. - Amazon ([Amazon Review, 2018](https://nijianmo.github.io/amazon/)):
 timestamped user online shopping behavior events in Amazon platform. All
 datasets are preprocess to the `Gatech` format dataset widely used for TPP
 researchers, and saved at [Google Drive](https://drive.google.com/drive/u/0/
 folders/1f8k82-NL6KFKuNMsUwozmbzDSFycYvz7) with a public access. ## Quick Start
-[Back_to_Top]  ## Documentation [Back_to_Top]  The classes and methods of
+[Back_to_Top]  We provide an end-to-end example for users to run a standard TPP
+model with `EasyTPP`. ### Step 1. Installation First of all, we can install the
+package either by using pip or from the source code on Github. To install the
+latest stable version: ```bash pip install easy-tpp ``` To install the latest
+on GitHub: ```bash git clone https://github.com/ant-research/
+EasyTemporalPointProcess.git cd EasyTemporalPointProcess python setup.py
+install ``` ### Step 2. Prepare datasets We need to put the datasets in a local
+directory before running a model and the datasets should follow a certain
+format. See [OnlineDoc - Datasets](https://ant-research.github.io/
+EasyTemporalPointProcess/user_guide/dataset.html) for more details. Suppose we
+use the [taxi dataset](https://chriswhong.com/open-data/foil_nyc_taxi/) in the
+example. ### Step 3. Train the model Before start training, we need to set up
+the config file for the pipeline. We provide a preset config file in [Example
+Config](https://github.com/ant-research/EasyTemporalPointProcess/blob/main/
+examples/configs/experiment_config.yaml). The details of the configuration can
+be found in [OnlineDoc - Training Pipeline](https://ant-research.github.io/
+EasyTemporalPointProcess/user_guide/run_train_pipeline.html). After the setup
+of data and config, the directory structure is as follows: ```bash data
+|______taxi |____ train.pkl |____ dev.pkl |____ test.pkl configs
+|______experiment_config.yaml ``` Then we start the training by simply running
+the script ```python import argparse from easy_tpp.config_factory import Config
+from easy_tpp.runner import Runner def main(): parser = argparse.ArgumentParser
+() parser.add_argument('--config_dir', type=str, required=False,
+default='configs/experiment_config.yaml', help='Dir of configuration yaml to
+train and evaluate the model.') parser.add_argument('--experiment_id',
+type=str, required=False, default='NHP_train', help='Experiment id in the
+config file.') args = parser.parse_args() config = Config.build_from_yaml_file
+(args.config_dir, experiment_id=args.experiment_id) model_runner =
+Runner.build_from_config(config) model_runner.run() if __name__ == '__main__':
+main() ``` A more detailed example can be found at [OnlineDoc - QuickStart]
+(https://ant-research.github.io/EasyTemporalPointProcess/get_started/
+quick_start.html). ## Documentation [Back_to_Top]  The classes and methods of
 `EasyTPP` have been well documented so that users can generate the
 documentation by: ```shell cd doc pip install -r requirements.txt make html ```
 NOTE: * The `doc/requirements.txt` is only for documentation by Sphinx, which
 can be automatically generated by Github actions `.github/workflows/docs.yml`.
 (Trigger by pull request.) The full documentation is available on the [website]
 (https://ant-research.github.io/EasyTemporalPointProcess/). ## License [Back_to
 Top] This project is licensed under the [Apache License (Version 2.0)](https://
```

### Comparing `easy_tpp-0.0.3/easy_tpp/config_factory/base_config.py` & `easy_tpp-0.0.4/easy_tpp/config_factory/base_config.py`

 * *Files identical despite different names*

### Comparing `easy_tpp-0.0.3/easy_tpp/config_factory/config.py` & `easy_tpp-0.0.4/easy_tpp/config_factory/config.py`

 * *Files identical despite different names*

### Comparing `easy_tpp-0.0.3/easy_tpp/config_factory/data_config.py` & `easy_tpp-0.0.4/easy_tpp/config_factory/data_config.py`

 * *Files identical despite different names*

### Comparing `easy_tpp-0.0.3/easy_tpp/config_factory/hpo_config.py` & `easy_tpp-0.0.4/easy_tpp/config_factory/hpo_config.py`

 * *Files identical despite different names*

### Comparing `easy_tpp-0.0.3/easy_tpp/config_factory/model_config.py` & `easy_tpp-0.0.4/easy_tpp/config_factory/model_config.py`

 * *Files identical despite different names*

### Comparing `easy_tpp-0.0.3/easy_tpp/config_factory/runner_config.py` & `easy_tpp-0.0.4/easy_tpp/config_factory/runner_config.py`

 * *Files identical despite different names*

### Comparing `easy_tpp-0.0.3/easy_tpp/default_registers/register_metrics.py` & `easy_tpp-0.0.4/easy_tpp/default_registers/register_metrics.py`

 * *Files identical despite different names*

### Comparing `easy_tpp-0.0.3/easy_tpp/default_registers/register_optuna_trials.py` & `easy_tpp-0.0.4/easy_tpp/default_registers/register_optuna_trials.py`

 * *Files identical despite different names*

### Comparing `easy_tpp-0.0.3/easy_tpp/hpo/base_hpo.py` & `easy_tpp-0.0.4/easy_tpp/hpo/base_hpo.py`

 * *Files identical despite different names*

### Comparing `easy_tpp-0.0.3/easy_tpp/hpo/optuna_hpo.py` & `easy_tpp-0.0.4/easy_tpp/hpo/optuna_hpo.py`

 * *Files identical despite different names*

### Comparing `easy_tpp-0.0.3/easy_tpp/model/__init__.py` & `easy_tpp-0.0.4/easy_tpp/model/__init__.py`

 * *Files identical despite different names*

### Comparing `easy_tpp-0.0.3/easy_tpp/model/tf_model/tf_anhn.py` & `easy_tpp-0.0.4/easy_tpp/model/tf_model/tf_anhn.py`

 * *Files identical despite different names*

### Comparing `easy_tpp-0.0.3/easy_tpp/model/tf_model/tf_attnhp.py` & `easy_tpp-0.0.4/easy_tpp/model/tf_model/tf_attnhp.py`

 * *Files identical despite different names*

### Comparing `easy_tpp-0.0.3/easy_tpp/model/tf_model/tf_baselayer.py` & `easy_tpp-0.0.4/easy_tpp/model/tf_model/tf_baselayer.py`

 * *Files identical despite different names*

### Comparing `easy_tpp-0.0.3/easy_tpp/model/tf_model/tf_basemodel.py` & `easy_tpp-0.0.4/easy_tpp/model/tf_model/tf_basemodel.py`

 * *Files identical despite different names*

### Comparing `easy_tpp-0.0.3/easy_tpp/model/tf_model/tf_fullynn.py` & `easy_tpp-0.0.4/easy_tpp/model/tf_model/tf_fullynn.py`

 * *Files identical despite different names*

### Comparing `easy_tpp-0.0.3/easy_tpp/model/tf_model/tf_intensity_free.py` & `easy_tpp-0.0.4/easy_tpp/model/tf_model/tf_intensity_free.py`

 * *Files identical despite different names*

### Comparing `easy_tpp-0.0.3/easy_tpp/model/tf_model/tf_nhp.py` & `easy_tpp-0.0.4/easy_tpp/model/tf_model/tf_nhp.py`

 * *Files identical despite different names*

### Comparing `easy_tpp-0.0.3/easy_tpp/model/tf_model/tf_ode_tpp.py` & `easy_tpp-0.0.4/easy_tpp/model/tf_model/tf_ode_tpp.py`

 * *Files identical despite different names*

### Comparing `easy_tpp-0.0.3/easy_tpp/model/tf_model/tf_rmtpp.py` & `easy_tpp-0.0.4/easy_tpp/model/tf_model/tf_rmtpp.py`

 * *Files identical despite different names*

### Comparing `easy_tpp-0.0.3/easy_tpp/model/tf_model/tf_sahp.py` & `easy_tpp-0.0.4/easy_tpp/model/tf_model/tf_sahp.py`

 * *Files identical despite different names*

### Comparing `easy_tpp-0.0.3/easy_tpp/model/tf_model/tf_thinning.py` & `easy_tpp-0.0.4/easy_tpp/model/tf_model/tf_thinning.py`

 * *Files identical despite different names*

### Comparing `easy_tpp-0.0.3/easy_tpp/model/tf_model/tf_thp.py` & `easy_tpp-0.0.4/easy_tpp/model/tf_model/tf_thp.py`

 * *Files identical despite different names*

### Comparing `easy_tpp-0.0.3/easy_tpp/model/torch_model/torch_anhn.py` & `easy_tpp-0.0.4/easy_tpp/model/torch_model/torch_anhn.py`

 * *Files identical despite different names*

### Comparing `easy_tpp-0.0.3/easy_tpp/model/torch_model/torch_attnhp.py` & `easy_tpp-0.0.4/easy_tpp/model/torch_model/torch_attnhp.py`

 * *Files identical despite different names*

### Comparing `easy_tpp-0.0.3/easy_tpp/model/torch_model/torch_baselayer.py` & `easy_tpp-0.0.4/easy_tpp/model/torch_model/torch_baselayer.py`

 * *Files identical despite different names*

### Comparing `easy_tpp-0.0.3/easy_tpp/model/torch_model/torch_basemodel.py` & `easy_tpp-0.0.4/easy_tpp/model/torch_model/torch_basemodel.py`

 * *Files identical despite different names*

### Comparing `easy_tpp-0.0.3/easy_tpp/model/torch_model/torch_fullynn.py` & `easy_tpp-0.0.4/easy_tpp/model/torch_model/torch_fullynn.py`

 * *Files identical despite different names*

### Comparing `easy_tpp-0.0.3/easy_tpp/model/torch_model/torch_intensity_free.py` & `easy_tpp-0.0.4/easy_tpp/model/torch_model/torch_intensity_free.py`

 * *Files identical despite different names*

### Comparing `easy_tpp-0.0.3/easy_tpp/model/torch_model/torch_nhp.py` & `easy_tpp-0.0.4/easy_tpp/model/torch_model/torch_nhp.py`

 * *Files identical despite different names*

### Comparing `easy_tpp-0.0.3/easy_tpp/model/torch_model/torch_ode_tpp.py` & `easy_tpp-0.0.4/easy_tpp/model/torch_model/torch_ode_tpp.py`

 * *Files identical despite different names*

### Comparing `easy_tpp-0.0.3/easy_tpp/model/torch_model/torch_rmtpp.py` & `easy_tpp-0.0.4/easy_tpp/model/torch_model/torch_rmtpp.py`

 * *Files identical despite different names*

### Comparing `easy_tpp-0.0.3/easy_tpp/model/torch_model/torch_sahp.py` & `easy_tpp-0.0.4/easy_tpp/model/torch_model/torch_sahp.py`

 * *Files identical despite different names*

### Comparing `easy_tpp-0.0.3/easy_tpp/model/torch_model/torch_thinning.py` & `easy_tpp-0.0.4/easy_tpp/model/torch_model/torch_thinning.py`

 * *Files identical despite different names*

### Comparing `easy_tpp-0.0.3/easy_tpp/model/torch_model/torch_thp.py` & `easy_tpp-0.0.4/easy_tpp/model/torch_model/torch_thp.py`

 * *Files identical despite different names*

### Comparing `easy_tpp-0.0.3/easy_tpp/preprocess/data_collator.py` & `easy_tpp-0.0.4/easy_tpp/preprocess/data_collator.py`

 * *Files identical despite different names*

### Comparing `easy_tpp-0.0.3/easy_tpp/preprocess/data_loader.py` & `easy_tpp-0.0.4/easy_tpp/preprocess/data_loader.py`

 * *Files identical despite different names*

### Comparing `easy_tpp-0.0.3/easy_tpp/preprocess/dataset.py` & `easy_tpp-0.0.4/easy_tpp/preprocess/dataset.py`

 * *Files identical despite different names*

### Comparing `easy_tpp-0.0.3/easy_tpp/preprocess/event_tokenizer.py` & `easy_tpp-0.0.4/easy_tpp/preprocess/event_tokenizer.py`

 * *Files identical despite different names*

### Comparing `easy_tpp-0.0.3/easy_tpp/runner/base_runner.py` & `easy_tpp-0.0.4/easy_tpp/runner/base_runner.py`

 * *Files identical despite different names*

### Comparing `easy_tpp-0.0.3/easy_tpp/runner/tpp_runner.py` & `easy_tpp-0.0.4/easy_tpp/runner/tpp_runner.py`

 * *Files identical despite different names*

### Comparing `easy_tpp-0.0.3/easy_tpp/tf_wrapper.py` & `easy_tpp-0.0.4/easy_tpp/tf_wrapper.py`

 * *Files identical despite different names*

### Comparing `easy_tpp-0.0.3/easy_tpp/torch_wrapper.py` & `easy_tpp-0.0.4/easy_tpp/torch_wrapper.py`

 * *Files identical despite different names*

### Comparing `easy_tpp-0.0.3/easy_tpp/utils/__init__.py` & `easy_tpp-0.0.4/easy_tpp/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `easy_tpp-0.0.3/easy_tpp/utils/const.py` & `easy_tpp-0.0.4/easy_tpp/utils/const.py`

 * *Files identical despite different names*

### Comparing `easy_tpp-0.0.3/easy_tpp/utils/generic.py` & `easy_tpp-0.0.4/easy_tpp/utils/generic.py`

 * *Files identical despite different names*

### Comparing `easy_tpp-0.0.3/easy_tpp/utils/import_utils.py` & `easy_tpp-0.0.4/easy_tpp/utils/import_utils.py`

 * *Files identical despite different names*

### Comparing `easy_tpp-0.0.3/easy_tpp/utils/log_utils.py` & `easy_tpp-0.0.4/easy_tpp/utils/log_utils.py`

 * *Files identical despite different names*

### Comparing `easy_tpp-0.0.3/easy_tpp/utils/metrics.py` & `easy_tpp-0.0.4/easy_tpp/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `easy_tpp-0.0.3/easy_tpp/utils/misc.py` & `easy_tpp-0.0.4/easy_tpp/utils/misc.py`

 * *Files identical despite different names*

### Comparing `easy_tpp-0.0.3/easy_tpp/utils/multiprocess_utils.py` & `easy_tpp-0.0.4/easy_tpp/utils/multiprocess_utils.py`

 * *Files identical despite different names*

### Comparing `easy_tpp-0.0.3/easy_tpp/utils/ode_utils.py` & `easy_tpp-0.0.4/easy_tpp/utils/ode_utils.py`

 * *Files identical despite different names*

### Comparing `easy_tpp-0.0.3/easy_tpp/utils/registrable.py` & `easy_tpp-0.0.4/easy_tpp/utils/registrable.py`

 * *Files identical despite different names*

### Comparing `easy_tpp-0.0.3/easy_tpp/utils/tf_utils.py` & `easy_tpp-0.0.4/easy_tpp/utils/tf_utils.py`

 * *Files identical despite different names*

### Comparing `easy_tpp-0.0.3/easy_tpp/utils/torch_utils.py` & `easy_tpp-0.0.4/easy_tpp/utils/torch_utils.py`

 * *Files identical despite different names*

### Comparing `easy_tpp-0.0.3/easy_tpp.egg-info/SOURCES.txt` & `easy_tpp-0.0.4/easy_tpp.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 LICENCE
+MANIFEST.in
 NOTICE
 README.md
+requirements.txt
 setup.cfg
 setup.py
+version.py
 easy_tpp/__init__.py
 easy_tpp/tf_wrapper.py
 easy_tpp/torch_wrapper.py
 easy_tpp.egg-info/PKG-INFO
 easy_tpp.egg-info/SOURCES.txt
 easy_tpp.egg-info/dependency_links.txt
 easy_tpp.egg-info/requires.txt
```

### Comparing `easy_tpp-0.0.3/setup.py` & `easy_tpp-0.0.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,16 +42,18 @@
 
     packages = list(parse_require_file(fname))
     return packages
 
 
 setup(
     name='easy_tpp',
-    version='0.0.3',
+    version=get_version(),
     description='An easy and flexible tool for neural temporal point process',
+    url = 'https://github.com/ant-research/EasyTemporalPointProcess/',
+    # long_description=readme(),
     author='Alipay',
     packages=find_packages(exclude=["*.tests", "*.tests.*", "tests.*", "tests"]),
     include_package_data=True,
     classifiers=[
         'Programming Language :: Python :: 3'
     ],
     install_requires=parse_requirements('requirements.txt'))
```

