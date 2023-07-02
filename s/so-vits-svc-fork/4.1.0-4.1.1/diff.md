# Comparing `tmp/so_vits_svc_fork-4.1.0.tar.gz` & `tmp/so_vits_svc_fork-4.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "so_vits_svc_fork-4.1.0.tar", max compression
+gzip compressed data, was "so_vits_svc_fork-4.1.1.tar", max compression
```

## Comparing `so_vits_svc_fork-4.1.0.tar` & `so_vits_svc_fork-4.1.1.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0    12463 2023-06-25 14:18:35.879591 so_vits_svc_fork-4.1.0/LICENSE
--rw-r--r--   0        0        0    28911 2023-06-25 14:18:35.879591 so_vits_svc_fork-4.1.0/README.md
--rw-r--r--   0        0        0     3093 2023-06-25 14:18:36.895603 so_vits_svc_fork-4.1.0/pyproject.toml
--rw-r--r--   0        0        0       70 2023-06-25 14:18:36.843603 so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/__init__.py
--rw-r--r--   0        0        0    24947 2023-06-25 14:18:35.883592 so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/__main__.py
--rw-r--r--   0        0        0     1393 2023-06-25 14:18:35.883592 so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/cluster/__init__.py
--rw-r--r--   0        0        0     4914 2023-06-25 14:18:35.883592 so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/cluster/train_cluster.py
--rw-r--r--   0        0        0     2875 2023-06-25 14:18:35.883592 so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/dataset.py
--rw-r--r--   0        0        0     2599 2023-06-25 14:18:35.883592 so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/default_gui_presets.json
--rw-r--r--   0        0        0     7267 2023-06-25 14:18:35.883592 so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/f0.py
--rw-r--r--   0        0        0    30617 2023-06-25 14:18:35.883592 so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/gui.py
--rw-r--r--   0        0        0      864 2023-06-25 14:18:35.883592 so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/hparams.py
--rw-r--r--   0        0        0        0 2023-06-25 14:18:35.883592 so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/inference/__init__.py
--rw-r--r--   0        0        0    24605 2023-06-25 14:18:35.883592 so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/inference/core.py
--rw-r--r--   0        0        0     9418 2023-06-25 14:18:35.883592 so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/inference/main.py
--rw-r--r--   0        0        0     1169 2023-06-25 14:18:35.883592 so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/logger.py
--rw-r--r--   0        0        0        0 2023-06-25 14:18:35.883592 so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/modules/__init__.py
--rw-r--r--   0        0        0    16683 2023-06-25 14:18:35.883592 so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/modules/attentions.py
--rw-r--r--   0        0        0     4620 2023-06-25 14:18:35.883592 so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/modules/commons.py
--rw-r--r--   0        0        0        0 2023-06-25 14:18:35.883592 so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/modules/decoders/__init__.py
--rw-r--r--   0        0        0     1463 2023-06-25 14:18:35.883592 so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/modules/decoders/f0.py
--rw-r--r--   0        0        0       76 2023-06-25 14:18:35.883592 so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/modules/decoders/hifigan/__init__.py
--rw-r--r--   0        0        0    11618 2023-06-25 14:18:35.883592 so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/modules/decoders/hifigan/_models.py
--rw-r--r--   0        0        0      340 2023-06-25 14:18:35.883592 so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/modules/decoders/hifigan/_utils.py
--rw-r--r--   0        0        0      318 2023-06-25 14:18:35.883592 so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/modules/decoders/mb_istft/__init__.py
--rw-r--r--   0        0        0    12477 2023-06-25 14:18:35.883592 so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/modules/decoders/mb_istft/_generators.py
--rw-r--r--   0        0        0      419 2023-06-25 14:18:35.883592 so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/modules/decoders/mb_istft/_loss.py
--rw-r--r--   0        0        0     4725 2023-06-25 14:18:35.883592 so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/modules/decoders/mb_istft/_pqmf.py
--rw-r--r--   0        0        0     8954 2023-06-25 14:18:35.883592 so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft.py
--rw-r--r--   0        0        0     4879 2023-06-25 14:18:35.883592 so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft_loss.py
--rw-r--r--   0        0        0     5604 2023-06-25 14:18:35.883592 so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/modules/descriminators.py
--rw-r--r--   0        0        0     4400 2023-06-25 14:18:35.883592 so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/modules/encoders.py
--rw-r--r--   0        0        0     1390 2023-06-25 14:18:35.883592 so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/modules/flows.py
--rw-r--r--   0        0        0     1405 2023-06-25 14:18:35.883592 so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/modules/losses.py
--rw-r--r--   0        0        0     5753 2023-06-25 14:18:35.883592 so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/modules/mel_processing.py
--rw-r--r--   0        0        0    14435 2023-06-25 14:18:35.883592 so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/modules/modules.py
--rw-r--r--   0        0        0     8178 2023-06-25 14:18:35.887591 so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/modules/synthesizers.py
--rw-r--r--   0        0        0        0 2023-06-25 14:18:35.887591 so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/preprocessing/__init__.py
--rw-r--r--   0        0        0     2051 2023-06-25 14:18:35.887591 so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/preprocessing/config_templates/quickvc.json
--rw-r--r--   0        0        0     1705 2023-06-25 14:18:35.887591 so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1-legacy.json
--rw-r--r--   0        0        0     1862 2023-06-25 14:18:35.887591 so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1.json
--rw-r--r--   0        0        0     2975 2023-06-25 14:18:35.887591 so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/preprocessing/preprocess_classify.py
--rw-r--r--   0        0        0     2710 2023-06-25 14:18:35.887591 so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/preprocessing/preprocess_flist_config.py
--rw-r--r--   0        0        0     4667 2023-06-25 14:18:35.887591 so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/preprocessing/preprocess_hubert_f0.py
--rw-r--r--   0        0        0     4447 2023-06-25 14:18:35.887591 so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/preprocessing/preprocess_resample.py
--rw-r--r--   0        0        0     2948 2023-06-25 14:18:35.887591 so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/preprocessing/preprocess_speaker_diarization.py
--rw-r--r--   0        0        0     2206 2023-06-25 14:18:35.887591 so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/preprocessing/preprocess_split.py
--rw-r--r--   0        0        0      126 2023-06-25 14:18:35.887591 so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/preprocessing/preprocess_utils.py
--rw-r--r--   0        0        0        0 2023-06-25 14:18:35.887591 so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/py.typed
--rw-r--r--   0        0        0    21359 2023-06-25 14:18:35.887591 so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/train.py
--rw-r--r--   0        0        0    14797 2023-06-25 14:18:35.887591 so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/utils.py
--rw-r--r--   0        0        0    30719 1970-01-01 00:00:00.000000 so_vits_svc_fork-4.1.0/PKG-INFO
+-rw-r--r--   0        0        0    12463 2023-07-02 04:00:33.319877 so_vits_svc_fork-4.1.1/LICENSE
+-rw-r--r--   0        0        0    28911 2023-07-02 04:00:33.319877 so_vits_svc_fork-4.1.1/README.md
+-rw-r--r--   0        0        0     3093 2023-07-02 04:00:34.195884 so_vits_svc_fork-4.1.1/pyproject.toml
+-rw-r--r--   0        0        0       70 2023-07-02 04:00:34.151884 so_vits_svc_fork-4.1.1/src/so_vits_svc_fork/__init__.py
+-rw-r--r--   0        0        0    24947 2023-07-02 04:00:33.323877 so_vits_svc_fork-4.1.1/src/so_vits_svc_fork/__main__.py
+-rw-r--r--   0        0        0     1393 2023-07-02 04:00:33.323877 so_vits_svc_fork-4.1.1/src/so_vits_svc_fork/cluster/__init__.py
+-rw-r--r--   0        0        0     4914 2023-07-02 04:00:33.323877 so_vits_svc_fork-4.1.1/src/so_vits_svc_fork/cluster/train_cluster.py
+-rw-r--r--   0        0        0     2875 2023-07-02 04:00:33.323877 so_vits_svc_fork-4.1.1/src/so_vits_svc_fork/dataset.py
+-rw-r--r--   0        0        0     2599 2023-07-02 04:00:33.323877 so_vits_svc_fork-4.1.1/src/so_vits_svc_fork/default_gui_presets.json
+-rw-r--r--   0        0        0     7267 2023-07-02 04:00:33.323877 so_vits_svc_fork-4.1.1/src/so_vits_svc_fork/f0.py
+-rw-r--r--   0        0        0    30617 2023-07-02 04:00:33.323877 so_vits_svc_fork-4.1.1/src/so_vits_svc_fork/gui.py
+-rw-r--r--   0        0        0      864 2023-07-02 04:00:33.323877 so_vits_svc_fork-4.1.1/src/so_vits_svc_fork/hparams.py
+-rw-r--r--   0        0        0        0 2023-07-02 04:00:33.323877 so_vits_svc_fork-4.1.1/src/so_vits_svc_fork/inference/__init__.py
+-rw-r--r--   0        0        0    24749 2023-07-02 04:00:33.323877 so_vits_svc_fork-4.1.1/src/so_vits_svc_fork/inference/core.py
+-rw-r--r--   0        0        0     9418 2023-07-02 04:00:33.323877 so_vits_svc_fork-4.1.1/src/so_vits_svc_fork/inference/main.py
+-rw-r--r--   0        0        0     1169 2023-07-02 04:00:33.323877 so_vits_svc_fork-4.1.1/src/so_vits_svc_fork/logger.py
+-rw-r--r--   0        0        0        0 2023-07-02 04:00:33.323877 so_vits_svc_fork-4.1.1/src/so_vits_svc_fork/modules/__init__.py
+-rw-r--r--   0        0        0    16683 2023-07-02 04:00:33.323877 so_vits_svc_fork-4.1.1/src/so_vits_svc_fork/modules/attentions.py
+-rw-r--r--   0        0        0     4620 2023-07-02 04:00:33.323877 so_vits_svc_fork-4.1.1/src/so_vits_svc_fork/modules/commons.py
+-rw-r--r--   0        0        0        0 2023-07-02 04:00:33.323877 so_vits_svc_fork-4.1.1/src/so_vits_svc_fork/modules/decoders/__init__.py
+-rw-r--r--   0        0        0     1463 2023-07-02 04:00:33.323877 so_vits_svc_fork-4.1.1/src/so_vits_svc_fork/modules/decoders/f0.py
+-rw-r--r--   0        0        0       76 2023-07-02 04:00:33.323877 so_vits_svc_fork-4.1.1/src/so_vits_svc_fork/modules/decoders/hifigan/__init__.py
+-rw-r--r--   0        0        0    11618 2023-07-02 04:00:33.323877 so_vits_svc_fork-4.1.1/src/so_vits_svc_fork/modules/decoders/hifigan/_models.py
+-rw-r--r--   0        0        0      340 2023-07-02 04:00:33.323877 so_vits_svc_fork-4.1.1/src/so_vits_svc_fork/modules/decoders/hifigan/_utils.py
+-rw-r--r--   0        0        0      318 2023-07-02 04:00:33.323877 so_vits_svc_fork-4.1.1/src/so_vits_svc_fork/modules/decoders/mb_istft/__init__.py
+-rw-r--r--   0        0        0    12477 2023-07-02 04:00:33.323877 so_vits_svc_fork-4.1.1/src/so_vits_svc_fork/modules/decoders/mb_istft/_generators.py
+-rw-r--r--   0        0        0      419 2023-07-02 04:00:33.323877 so_vits_svc_fork-4.1.1/src/so_vits_svc_fork/modules/decoders/mb_istft/_loss.py
+-rw-r--r--   0        0        0     4725 2023-07-02 04:00:33.323877 so_vits_svc_fork-4.1.1/src/so_vits_svc_fork/modules/decoders/mb_istft/_pqmf.py
+-rw-r--r--   0        0        0     8954 2023-07-02 04:00:33.323877 so_vits_svc_fork-4.1.1/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft.py
+-rw-r--r--   0        0        0     4879 2023-07-02 04:00:33.323877 so_vits_svc_fork-4.1.1/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft_loss.py
+-rw-r--r--   0        0        0     5604 2023-07-02 04:00:33.323877 so_vits_svc_fork-4.1.1/src/so_vits_svc_fork/modules/descriminators.py
+-rw-r--r--   0        0        0     4400 2023-07-02 04:00:33.323877 so_vits_svc_fork-4.1.1/src/so_vits_svc_fork/modules/encoders.py
+-rw-r--r--   0        0        0     1390 2023-07-02 04:00:33.323877 so_vits_svc_fork-4.1.1/src/so_vits_svc_fork/modules/flows.py
+-rw-r--r--   0        0        0     1405 2023-07-02 04:00:33.323877 so_vits_svc_fork-4.1.1/src/so_vits_svc_fork/modules/losses.py
+-rw-r--r--   0        0        0     5753 2023-07-02 04:00:33.323877 so_vits_svc_fork-4.1.1/src/so_vits_svc_fork/modules/mel_processing.py
+-rw-r--r--   0        0        0    14435 2023-07-02 04:00:33.327878 so_vits_svc_fork-4.1.1/src/so_vits_svc_fork/modules/modules.py
+-rw-r--r--   0        0        0     8178 2023-07-02 04:00:33.327878 so_vits_svc_fork-4.1.1/src/so_vits_svc_fork/modules/synthesizers.py
+-rw-r--r--   0        0        0        0 2023-07-02 04:00:33.327878 so_vits_svc_fork-4.1.1/src/so_vits_svc_fork/preprocessing/__init__.py
+-rw-r--r--   0        0        0     2051 2023-07-02 04:00:33.327878 so_vits_svc_fork-4.1.1/src/so_vits_svc_fork/preprocessing/config_templates/quickvc.json
+-rw-r--r--   0        0        0     1705 2023-07-02 04:00:33.327878 so_vits_svc_fork-4.1.1/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1-legacy.json
+-rw-r--r--   0        0        0     1862 2023-07-02 04:00:33.327878 so_vits_svc_fork-4.1.1/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1.json
+-rw-r--r--   0        0        0     2975 2023-07-02 04:00:33.327878 so_vits_svc_fork-4.1.1/src/so_vits_svc_fork/preprocessing/preprocess_classify.py
+-rw-r--r--   0        0        0     2710 2023-07-02 04:00:33.327878 so_vits_svc_fork-4.1.1/src/so_vits_svc_fork/preprocessing/preprocess_flist_config.py
+-rw-r--r--   0        0        0     4667 2023-07-02 04:00:33.327878 so_vits_svc_fork-4.1.1/src/so_vits_svc_fork/preprocessing/preprocess_hubert_f0.py
+-rw-r--r--   0        0        0     4447 2023-07-02 04:00:33.327878 so_vits_svc_fork-4.1.1/src/so_vits_svc_fork/preprocessing/preprocess_resample.py
+-rw-r--r--   0        0        0     2948 2023-07-02 04:00:33.327878 so_vits_svc_fork-4.1.1/src/so_vits_svc_fork/preprocessing/preprocess_speaker_diarization.py
+-rw-r--r--   0        0        0     2206 2023-07-02 04:00:33.327878 so_vits_svc_fork-4.1.1/src/so_vits_svc_fork/preprocessing/preprocess_split.py
+-rw-r--r--   0        0        0      126 2023-07-02 04:00:33.327878 so_vits_svc_fork-4.1.1/src/so_vits_svc_fork/preprocessing/preprocess_utils.py
+-rw-r--r--   0        0        0        0 2023-07-02 04:00:33.327878 so_vits_svc_fork-4.1.1/src/so_vits_svc_fork/py.typed
+-rw-r--r--   0        0        0    21359 2023-07-02 04:00:33.327878 so_vits_svc_fork-4.1.1/src/so_vits_svc_fork/train.py
+-rw-r--r--   0        0        0    15617 2023-07-02 04:00:33.327878 so_vits_svc_fork-4.1.1/src/so_vits_svc_fork/utils.py
+-rw-r--r--   0        0        0    30719 1970-01-01 00:00:00.000000 so_vits_svc_fork-4.1.1/PKG-INFO
```

### Comparing `so_vits_svc_fork-4.1.0/LICENSE` & `so_vits_svc_fork-4.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.1.0/README.md` & `so_vits_svc_fork-4.1.1/README.md`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.1.0/pyproject.toml` & `so_vits_svc_fork-4.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "so-vits-svc-fork"
-version = "4.1.0"
+version = "4.1.1"
 description = "A fork of so-vits-svc."
 authors = ["34j <34j.95a2p@simplelogin.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/34j/so-vits-svc-fork"
 documentation = "https://so-vits-svc-fork.readthedocs.io"
 classifiers = [
@@ -51,15 +51,15 @@
 tqdm-joblib = "*"
 tensorboardx = "*"
 cm-time = ">=0.1.2"
 pysimplegui = ">=4.6"
 pebble = ">=5.0"
 torchcrepe = ">=0.0.17"
 lightning = "^2.0.1"
-fastapi = "==0.98.0"
+fastapi = "==0.99.0"
 transformers = "^4.28.1"
 matplotlib = "^3.7.1"
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = ">=3"
 pytest = "^7.0"
 pytest-cov = "^4.0.0"
```

### Comparing `so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/__main__.py` & `so_vits_svc_fork-4.1.1/src/so_vits_svc_fork/__main__.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/cluster/__init__.py` & `so_vits_svc_fork-4.1.1/src/so_vits_svc_fork/cluster/__init__.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/cluster/train_cluster.py` & `so_vits_svc_fork-4.1.1/src/so_vits_svc_fork/cluster/train_cluster.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/dataset.py` & `so_vits_svc_fork-4.1.1/src/so_vits_svc_fork/dataset.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/default_gui_presets.json` & `so_vits_svc_fork-4.1.1/src/so_vits_svc_fork/default_gui_presets.json`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/f0.py` & `so_vits_svc_fork-4.1.1/src/so_vits_svc_fork/f0.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/gui.py` & `so_vits_svc_fork-4.1.1/src/so_vits_svc_fork/gui.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/hparams.py` & `so_vits_svc_fork-4.1.1/src/so_vits_svc_fork/hparams.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/inference/core.py` & `so_vits_svc_fork-4.1.1/src/so_vits_svc_fork/inference/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -130,15 +130,19 @@
     def load_model(self):
         self.net_g = SynthesizerTrn(
             self.hps.data.filter_length // 2 + 1,
             self.hps.train.segment_size // self.hps.data.hop_length,
             **self.hps.model,
         )
         _ = utils.load_checkpoint(self.net_g_path, self.net_g, None)
-        _ = self.net_g.eval().to(self.device, dtype=self.dtype)
+        _ = self.net_g.eval()
+        for m in self.net_g.modules():
+            utils.remove_weight_norm_if_exists(m)
+        _ = self.net_g.to(self.device, dtype=self.dtype)
+        self.net_g = self.net_g
 
     def get_unit_f0(
         self,
         audio: ndarray[Any, dtype[float32]],
         tran: int,
         cluster_infer_ratio: float,
         speaker: int | str,
```

### Comparing `so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/inference/main.py` & `so_vits_svc_fork-4.1.1/src/so_vits_svc_fork/inference/main.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/logger.py` & `so_vits_svc_fork-4.1.1/src/so_vits_svc_fork/logger.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/modules/attentions.py` & `so_vits_svc_fork-4.1.1/src/so_vits_svc_fork/modules/attentions.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/modules/commons.py` & `so_vits_svc_fork-4.1.1/src/so_vits_svc_fork/modules/commons.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/modules/decoders/f0.py` & `so_vits_svc_fork-4.1.1/src/so_vits_svc_fork/modules/decoders/f0.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/modules/decoders/hifigan/_models.py` & `so_vits_svc_fork-4.1.1/src/so_vits_svc_fork/modules/decoders/hifigan/_models.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/modules/decoders/mb_istft/_generators.py` & `so_vits_svc_fork-4.1.1/src/so_vits_svc_fork/modules/decoders/mb_istft/_generators.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/modules/decoders/mb_istft/_pqmf.py` & `so_vits_svc_fork-4.1.1/src/so_vits_svc_fork/modules/decoders/mb_istft/_pqmf.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft.py` & `so_vits_svc_fork-4.1.1/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft_loss.py` & `so_vits_svc_fork-4.1.1/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft_loss.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/modules/descriminators.py` & `so_vits_svc_fork-4.1.1/src/so_vits_svc_fork/modules/descriminators.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/modules/encoders.py` & `so_vits_svc_fork-4.1.1/src/so_vits_svc_fork/modules/encoders.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/modules/flows.py` & `so_vits_svc_fork-4.1.1/src/so_vits_svc_fork/modules/flows.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/modules/losses.py` & `so_vits_svc_fork-4.1.1/src/so_vits_svc_fork/modules/losses.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/modules/mel_processing.py` & `so_vits_svc_fork-4.1.1/src/so_vits_svc_fork/modules/mel_processing.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/modules/modules.py` & `so_vits_svc_fork-4.1.1/src/so_vits_svc_fork/modules/modules.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/modules/synthesizers.py` & `so_vits_svc_fork-4.1.1/src/so_vits_svc_fork/modules/synthesizers.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/preprocessing/config_templates/quickvc.json` & `so_vits_svc_fork-4.1.1/src/so_vits_svc_fork/preprocessing/config_templates/quickvc.json`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1-legacy.json` & `so_vits_svc_fork-4.1.1/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1-legacy.json`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1.json` & `so_vits_svc_fork-4.1.1/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1.json`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/preprocessing/preprocess_classify.py` & `so_vits_svc_fork-4.1.1/src/so_vits_svc_fork/preprocessing/preprocess_classify.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/preprocessing/preprocess_flist_config.py` & `so_vits_svc_fork-4.1.1/src/so_vits_svc_fork/preprocessing/preprocess_flist_config.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/preprocessing/preprocess_hubert_f0.py` & `so_vits_svc_fork-4.1.1/src/so_vits_svc_fork/preprocessing/preprocess_hubert_f0.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/preprocessing/preprocess_resample.py` & `so_vits_svc_fork-4.1.1/src/so_vits_svc_fork/preprocessing/preprocess_resample.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/preprocessing/preprocess_speaker_diarization.py` & `so_vits_svc_fork-4.1.1/src/so_vits_svc_fork/preprocessing/preprocess_speaker_diarization.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/preprocessing/preprocess_split.py` & `so_vits_svc_fork-4.1.1/src/so_vits_svc_fork/preprocessing/preprocess_split.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/train.py` & `so_vits_svc_fork-4.1.1/src/so_vits_svc_fork/train.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/utils.py` & `so_vits_svc_fork-4.1.1/src/so_vits_svc_fork/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -165,23 +165,47 @@
 
         # The final projection layer is only used for backward compatibility.
         # Following https://github.com/auspicious3000/contentvec/issues/6
         # Remove this layer is necessary to achieve the desired outcome.
         self.final_proj = nn.Linear(config.hidden_size, config.classifier_proj_size)
 
 
+def remove_weight_norm_if_exists(module, name: str = "weight"):
+    r"""Removes the weight normalization reparameterization from a module.
+
+    Args:
+        module (Module): containing module
+        name (str, optional): name of weight parameter
+
+    Example:
+        >>> m = weight_norm(nn.Linear(20, 40))
+        >>> remove_weight_norm(m)
+    """
+    from torch.nn.utils.weight_norm import WeightNorm
+
+    for k, hook in module._forward_pre_hooks.items():
+        if isinstance(hook, WeightNorm) and hook.name == name:
+            hook.remove(module)
+            del module._forward_pre_hooks[k]
+            return module
+
+
 def get_hubert_model(
     device: str | torch.device, final_proj: bool = True
 ) -> HubertModel:
     if final_proj:
-        return HubertModelWithFinalProj.from_pretrained(
-            "lengyue233/content-vec-best"
-        ).to(device)
+        model = HubertModelWithFinalProj.from_pretrained("lengyue233/content-vec-best")
     else:
-        return HubertModel.from_pretrained("lengyue233/content-vec-best").to(device)
+        model = HubertModel.from_pretrained("lengyue233/content-vec-best")
+    # Hubert is always used in inference mode, we can safely remove weight-norms
+    for m in model.modules():
+        if isinstance(m, (nn.Conv2d, nn.Conv1d)):
+            remove_weight_norm_if_exists(m)
+
+    return model.to(device)
 
 
 def get_content(
     cmodel: HubertModel,
     audio: torch.Tensor | ndarray[Any, Any],
     device: torch.device | str,
     sr: int,
```

### Comparing `so_vits_svc_fork-4.1.0/PKG-INFO` & `so_vits_svc_fork-4.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: so-vits-svc-fork
-Version: 4.1.0
+Version: 4.1.1
 Summary: A fork of so-vits-svc.
 Home-page: https://github.com/34j/so-vits-svc-fork
 License: MIT
 Author: 34j
 Author-email: 34j.95a2p@simplelogin.com
 Requires-Python: >=3.8,<3.11
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -15,15 +15,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries
 Requires-Dist: SoundFile
 Requires-Dist: cm-time (>=0.1.2)
-Requires-Dist: fastapi (==0.98.0)
+Requires-Dist: fastapi (==0.99.0)
 Requires-Dist: librosa
 Requires-Dist: lightning (>=2.0.1,<3.0.0)
 Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
 Requires-Dist: numpy (>=1.23,<2.0)
 Requires-Dist: onnx
 Requires-Dist: onnxoptimizer
 Requires-Dist: onnxsim
```

#### html2text {}

```diff
@@ -1,18 +1,18 @@
-Metadata-Version: 2.1 Name: so-vits-svc-fork Version: 4.1.0 Summary: A fork of
+Metadata-Version: 2.1 Name: so-vits-svc-fork Version: 4.1.1 Summary: A fork of
 so-vits-svc. Home-page: https://github.com/34j/so-vits-svc-fork License: MIT
 Author: 34j Author-email: 34j.95a2p@simplelogin.com Requires-Python:
 >=3.8,<3.11 Classifier: Development Status :: 2 - Pre-Alpha Classifier:
 Intended Audience :: Developers Classifier: License :: OSI Approved :: MIT
 License Classifier: Natural Language :: English Classifier: Operating System ::
 OS Independent Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Topic :: Software Development :: Libraries Requires-Dist: SoundFile Requires-
-Dist: cm-time (>=0.1.2) Requires-Dist: fastapi (==0.98.0) Requires-Dist:
+Dist: cm-time (>=0.1.2) Requires-Dist: fastapi (==0.99.0) Requires-Dist:
 librosa Requires-Dist: lightning (>=2.0.1,<3.0.0) Requires-Dist: matplotlib
 (>=3.7.1,<4.0.0) Requires-Dist: numpy (>=1.23,<2.0) Requires-Dist: onnx
 Requires-Dist: onnxoptimizer Requires-Dist: onnxsim Requires-Dist: pebble
 (>=5.0) Requires-Dist: praat-parselmouth Requires-Dist: pysimplegui (>=4.6)
 Requires-Dist: pyworld Requires-Dist: requests Requires-Dist: rich Requires-
 Dist: scipy Requires-Dist: sounddevice Requires-Dist: tensorboard Requires-
 Dist: tensorboardx Requires-Dist: torch Requires-Dist: torchaudio Requires-
```

