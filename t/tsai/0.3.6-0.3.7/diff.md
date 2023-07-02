# Comparing `tmp/tsai-0.3.6.tar.gz` & `tmp/tsai-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tsai-0.3.6.tar", last modified: Sun Apr  2 19:39:01 2023, max compression
+gzip compressed data, was "tsai-0.3.7.tar", last modified: Sun Jul  2 20:47:40 2023, max compression
```

## Comparing `tsai-0.3.6.tar` & `tsai-0.3.7.tar`

### file list

```diff
@@ -1,111 +1,114 @@
-drwxr-xr-x   0 nacho      (501) staff       (20)        0 2023-04-02 19:39:01.407058 tsai-0.3.6/
--rw-r--r--   0 nacho      (501) staff       (20)     5400 2023-03-31 19:52:01.000000 tsai-0.3.6/CONTRIBUTING.md
--rw-r--r--   0 nacho      (501) staff       (20)    11357 2021-04-15 15:58:44.000000 tsai-0.3.6/LICENSE
--rw-r--r--   0 nacho      (501) staff       (20)      111 2021-04-15 15:58:44.000000 tsai-0.3.6/MANIFEST.in
--rw-r--r--   0 nacho      (501) staff       (20)    15975 2023-04-02 19:39:01.403714 tsai-0.3.6/PKG-INFO
--rw-r--r--   0 nacho      (501) staff       (20)    14964 2023-04-01 19:34:41.000000 tsai-0.3.6/README.md
--rw-r--r--   0 nacho      (501) staff       (20)     1277 2023-04-01 20:50:04.000000 tsai-0.3.6/settings.ini
--rw-r--r--   0 nacho      (501) staff       (20)       38 2023-04-02 19:39:01.415020 tsai-0.3.6/setup.cfg
--rw-r--r--   0 nacho      (501) staff       (20)     2864 2022-10-08 18:52:14.000000 tsai-0.3.6/setup.py
-drwxr-xr-x   0 nacho      (501) staff       (20)        0 2023-04-02 19:39:01.161369 tsai-0.3.6/tsai/
--rw-r--r--   0 nacho      (501) staff       (20)       21 2023-04-02 18:55:34.000000 tsai-0.3.6/tsai/__init__.py
--rw-r--r--   0 nacho      (501) staff       (20)   344061 2023-04-02 18:55:36.000000 tsai-0.3.6/tsai/_modidx.py
--rw-r--r--   0 nacho      (501) staff       (20)    42866 2022-10-08 12:17:23.000000 tsai-0.3.6/tsai/_nbdev.py
--rw-r--r--   0 nacho      (501) staff       (20)      392 2022-03-01 14:30:56.000000 tsai-0.3.6/tsai/all.py
--rw-r--r--   0 nacho      (501) staff       (20)    21956 2023-04-02 18:55:32.000000 tsai-0.3.6/tsai/analysis.py
--rw-r--r--   0 nacho      (501) staff       (20)      335 2022-03-01 14:31:40.000000 tsai-0.3.6/tsai/basics.py
--rw-r--r--   0 nacho      (501) staff       (20)     6755 2023-04-02 18:55:32.000000 tsai-0.3.6/tsai/calibration.py
-drwxr-xr-x   0 nacho      (501) staff       (20)        0 2023-04-02 19:39:01.197976 tsai-0.3.6/tsai/callback/
--rw-r--r--   0 nacho      (501) staff       (20)    13868 2023-04-02 18:55:32.000000 tsai-0.3.6/tsai/callback/MVP.py
--rw-r--r--   0 nacho      (501) staff       (20)     8602 2023-04-02 18:55:33.000000 tsai-0.3.6/tsai/callback/PredictionDynamics.py
--rw-r--r--   0 nacho      (501) staff       (20)        0 2023-04-02 18:55:34.000000 tsai-0.3.6/tsai/callback/__init__.py
--rw-r--r--   0 nacho      (501) staff       (20)      129 2022-03-01 14:34:50.000000 tsai-0.3.6/tsai/callback/all.py
--rw-r--r--   0 nacho      (501) staff       (20)    14220 2023-04-02 18:55:32.000000 tsai-0.3.6/tsai/callback/core.py
--rw-r--r--   0 nacho      (501) staff       (20)     8961 2023-04-02 18:55:32.000000 tsai-0.3.6/tsai/callback/experimental.py
--rw-r--r--   0 nacho      (501) staff       (20)     5199 2023-04-02 18:55:32.000000 tsai-0.3.6/tsai/callback/noisy_student.py
-drwxr-xr-x   0 nacho      (501) staff       (20)        0 2023-04-02 19:39:01.254519 tsai-0.3.6/tsai/data/
--rw-r--r--   0 nacho      (501) staff       (20)        0 2023-04-02 18:55:34.000000 tsai-0.3.6/tsai/data/__init__.py
--rw-r--r--   0 nacho      (501) staff       (20)      328 2022-03-03 08:27:56.000000 tsai-0.3.6/tsai/data/all.py
--rw-r--r--   0 nacho      (501) staff       (20)      185 2022-03-01 14:32:50.000000 tsai-0.3.6/tsai/data/basics.py
--rw-r--r--   0 nacho      (501) staff       (20)    50414 2023-04-02 18:55:31.000000 tsai-0.3.6/tsai/data/core.py
--rw-r--r--   0 nacho      (501) staff       (20)   149556 2023-04-02 18:55:31.000000 tsai-0.3.6/tsai/data/external.py
--rw-r--r--   0 nacho      (501) staff       (20)     1896 2023-04-02 18:55:32.000000 tsai-0.3.6/tsai/data/features.py
--rw-r--r--   0 nacho      (501) staff       (20)     9503 2023-04-02 18:55:32.000000 tsai-0.3.6/tsai/data/image.py
--rw-r--r--   0 nacho      (501) staff       (20)     3069 2023-04-02 18:55:31.000000 tsai-0.3.6/tsai/data/metadatasets.py
--rw-r--r--   0 nacho      (501) staff       (20)     6906 2023-04-02 18:55:32.000000 tsai-0.3.6/tsai/data/mixed.py
--rw-r--r--   0 nacho      (501) staff       (20)     4807 2023-04-02 18:55:32.000000 tsai-0.3.6/tsai/data/mixed_augmentation.py
--rw-r--r--   0 nacho      (501) staff       (20)    47523 2023-04-02 18:55:30.000000 tsai-0.3.6/tsai/data/preparation.py
--rw-r--r--   0 nacho      (501) staff       (20)    67803 2023-04-02 18:55:31.000000 tsai-0.3.6/tsai/data/preprocessing.py
--rw-r--r--   0 nacho      (501) staff       (20)     3112 2023-04-02 18:55:32.000000 tsai-0.3.6/tsai/data/tabular.py
--rw-r--r--   0 nacho      (501) staff       (20)    44670 2023-04-02 18:55:32.000000 tsai-0.3.6/tsai/data/transforms.py
--rw-r--r--   0 nacho      (501) staff       (20)     3470 2023-04-02 18:55:31.000000 tsai-0.3.6/tsai/data/unwindowed.py
--rw-r--r--   0 nacho      (501) staff       (20)    33777 2023-04-02 18:55:30.000000 tsai-0.3.6/tsai/data/validation.py
--rw-r--r--   0 nacho      (501) staff       (20)    10833 2023-04-02 18:55:29.000000 tsai-0.3.6/tsai/export.py
--rw-r--r--   0 nacho      (501) staff       (20)    12876 2023-03-16 10:57:48.000000 tsai-0.3.6/tsai/imports.py
--rw-r--r--   0 nacho      (501) staff       (20)      103 2022-04-30 11:41:05.000000 tsai-0.3.6/tsai/index.py
--rw-r--r--   0 nacho      (501) staff       (20)     1125 2023-04-02 18:55:32.000000 tsai-0.3.6/tsai/inference.py
--rw-r--r--   0 nacho      (501) staff       (20)    26139 2023-04-02 18:55:32.000000 tsai-0.3.6/tsai/learner.py
--rw-r--r--   0 nacho      (501) staff       (20)     6287 2023-04-02 18:55:32.000000 tsai-0.3.6/tsai/losses.py
--rw-r--r--   0 nacho      (501) staff       (20)     8344 2023-04-02 18:55:32.000000 tsai-0.3.6/tsai/metrics.py
-drwxr-xr-x   0 nacho      (501) staff       (20)        0 2023-04-02 19:39:01.400899 tsai-0.3.6/tsai/models/
--rw-r--r--   0 nacho      (501) staff       (20)      803 2023-04-02 18:55:33.000000 tsai-0.3.6/tsai/models/FCN.py
--rw-r--r--   0 nacho      (501) staff       (20)     2533 2023-04-02 18:55:33.000000 tsai-0.3.6/tsai/models/FCNPlus.py
--rw-r--r--   0 nacho      (501) staff       (20)     1719 2023-04-02 18:55:34.000000 tsai-0.3.6/tsai/models/GatedTabTransformer.py
--rw-r--r--   0 nacho      (501) staff       (20)     2961 2023-04-02 18:55:33.000000 tsai-0.3.6/tsai/models/InceptionTime.py
--rw-r--r--   0 nacho      (501) staff       (20)     9867 2023-04-02 18:55:33.000000 tsai-0.3.6/tsai/models/InceptionTimePlus.py
--rw-r--r--   0 nacho      (501) staff       (20)     8927 2023-04-02 18:55:34.000000 tsai-0.3.6/tsai/models/MINIROCKET.py
--rw-r--r--   0 nacho      (501) staff       (20)    15510 2023-04-02 18:55:34.000000 tsai-0.3.6/tsai/models/MINIROCKETPlus_Pytorch.py
--rw-r--r--   0 nacho      (501) staff       (20)     9541 2023-04-02 18:55:34.000000 tsai-0.3.6/tsai/models/MINIROCKET_Pytorch.py
--rw-r--r--   0 nacho      (501) staff       (20)     1192 2023-04-02 18:55:33.000000 tsai-0.3.6/tsai/models/MLP.py
--rw-r--r--   0 nacho      (501) staff       (20)     3130 2023-04-02 18:55:34.000000 tsai-0.3.6/tsai/models/MultiInputNet.py
--rw-r--r--   0 nacho      (501) staff       (20)     4601 2023-04-02 18:55:34.000000 tsai-0.3.6/tsai/models/OmniScaleCNN.py
--rw-r--r--   0 nacho      (501) staff       (20)    19902 2023-04-02 18:55:34.000000 tsai-0.3.6/tsai/models/PatchTST.py
--rw-r--r--   0 nacho      (501) staff       (20)     2189 2023-04-02 18:55:33.000000 tsai-0.3.6/tsai/models/RNN.py
--rw-r--r--   0 nacho      (501) staff       (20)    10187 2023-04-02 18:55:34.000000 tsai-0.3.6/tsai/models/RNNAttention.py
--rw-r--r--   0 nacho      (501) staff       (20)     6231 2023-04-02 18:55:33.000000 tsai-0.3.6/tsai/models/RNNPlus.py
--rw-r--r--   0 nacho      (501) staff       (20)     3053 2023-04-02 18:55:33.000000 tsai-0.3.6/tsai/models/RNN_FCN.py
--rw-r--r--   0 nacho      (501) staff       (20)     4315 2023-04-02 18:55:33.000000 tsai-0.3.6/tsai/models/RNN_FCNPlus.py
--rw-r--r--   0 nacho      (501) staff       (20)     4356 2023-04-02 18:55:34.000000 tsai-0.3.6/tsai/models/ROCKET.py
--rw-r--r--   0 nacho      (501) staff       (20)     3049 2023-04-02 18:55:34.000000 tsai-0.3.6/tsai/models/ROCKET_Pytorch.py
--rw-r--r--   0 nacho      (501) staff       (20)     1973 2023-04-02 18:55:33.000000 tsai-0.3.6/tsai/models/ResCNN.py
--rw-r--r--   0 nacho      (501) staff       (20)     1492 2023-04-02 18:55:33.000000 tsai-0.3.6/tsai/models/ResNet.py
--rw-r--r--   0 nacho      (501) staff       (20)     3508 2023-04-02 18:55:33.000000 tsai-0.3.6/tsai/models/ResNetPlus.py
--rw-r--r--   0 nacho      (501) staff       (20)     2879 2023-04-02 18:55:34.000000 tsai-0.3.6/tsai/models/TCN.py
--rw-r--r--   0 nacho      (501) staff       (20)     9879 2023-04-02 18:55:34.000000 tsai-0.3.6/tsai/models/TSPerceiver.py
--rw-r--r--   0 nacho      (501) staff       (20)    13176 2023-04-02 18:55:34.000000 tsai-0.3.6/tsai/models/TSSequencerPlus.py
--rw-r--r--   0 nacho      (501) staff       (20)    10674 2023-04-02 18:55:33.000000 tsai-0.3.6/tsai/models/TST.py
--rw-r--r--   0 nacho      (501) staff       (20)    19652 2023-04-02 18:55:33.000000 tsai-0.3.6/tsai/models/TSTPlus.py
--rw-r--r--   0 nacho      (501) staff       (20)    14086 2023-04-02 18:55:34.000000 tsai-0.3.6/tsai/models/TSiTPlus.py
--rw-r--r--   0 nacho      (501) staff       (20)    14453 2023-04-02 18:55:34.000000 tsai-0.3.6/tsai/models/TabFusionTransformer.py
--rw-r--r--   0 nacho      (501) staff       (20)     3004 2023-04-02 18:55:34.000000 tsai-0.3.6/tsai/models/TabModel.py
--rw-r--r--   0 nacho      (501) staff       (20)    12863 2023-04-02 18:55:34.000000 tsai-0.3.6/tsai/models/TabTransformer.py
--rw-r--r--   0 nacho      (501) staff       (20)     2194 2023-04-02 18:55:33.000000 tsai-0.3.6/tsai/models/TransformerModel.py
--rw-r--r--   0 nacho      (501) staff       (20)     4200 2023-04-02 18:55:34.000000 tsai-0.3.6/tsai/models/XCM.py
--rw-r--r--   0 nacho      (501) staff       (20)     4712 2023-04-02 18:55:34.000000 tsai-0.3.6/tsai/models/XCMPlus.py
--rw-r--r--   0 nacho      (501) staff       (20)     2213 2023-04-02 18:55:34.000000 tsai-0.3.6/tsai/models/XResNet1d.py
--rw-r--r--   0 nacho      (501) staff       (20)     5507 2023-04-02 18:55:34.000000 tsai-0.3.6/tsai/models/XResNet1dPlus.py
--rw-r--r--   0 nacho      (501) staff       (20)     3298 2023-04-02 18:55:33.000000 tsai-0.3.6/tsai/models/XceptionTime.py
--rw-r--r--   0 nacho      (501) staff       (20)     5063 2023-04-02 18:55:33.000000 tsai-0.3.6/tsai/models/XceptionTimePlus.py
--rw-r--r--   0 nacho      (501) staff       (20)        0 2023-04-02 18:55:34.000000 tsai-0.3.6/tsai/models/__init__.py
--rw-r--r--   0 nacho      (501) staff       (20)     1210 2023-03-16 17:21:46.000000 tsai-0.3.6/tsai/models/all.py
--rw-r--r--   0 nacho      (501) staff       (20)     2401 2023-04-02 18:55:33.000000 tsai-0.3.6/tsai/models/explainability.py
--rw-r--r--   0 nacho      (501) staff       (20)     2428 2023-04-02 18:55:33.000000 tsai-0.3.6/tsai/models/gMLP.py
--rw-r--r--   0 nacho      (501) staff       (20)    62784 2023-04-02 18:55:33.000000 tsai-0.3.6/tsai/models/layers.py
--rw-r--r--   0 nacho      (501) staff       (20)     4232 2023-04-02 18:55:34.000000 tsai-0.3.6/tsai/models/mWDN.py
--rw-r--r--   0 nacho      (501) staff       (20)     1958 2023-04-02 18:55:34.000000 tsai-0.3.6/tsai/models/misc.py
--rw-r--r--   0 nacho      (501) staff       (20)     1775 2023-04-02 18:55:33.000000 tsai-0.3.6/tsai/models/positional_encoders.py
--rw-r--r--   0 nacho      (501) staff       (20)    13400 2023-04-02 18:55:33.000000 tsai-0.3.6/tsai/models/utils.py
--rw-r--r--   0 nacho      (501) staff       (20)      328 2023-04-02 18:55:32.000000 tsai-0.3.6/tsai/optimizer.py
--rw-r--r--   0 nacho      (501) staff       (20)     6592 2023-04-02 18:55:34.000000 tsai-0.3.6/tsai/optuna.py
--rw-r--r--   0 nacho      (501) staff       (20)    13468 2023-04-02 18:55:32.000000 tsai-0.3.6/tsai/tslearner.py
--rw-r--r--   0 nacho      (501) staff       (20)      111 2022-10-08 12:17:15.000000 tsai-0.3.6/tsai/tutorials.py
--rw-r--r--   0 nacho      (501) staff       (20)    64888 2023-04-02 18:55:30.000000 tsai-0.3.6/tsai/utils.py
--rw-r--r--   0 nacho      (501) staff       (20)     2543 2023-04-02 18:55:34.000000 tsai-0.3.6/tsai/wandb.py
-drwxr-xr-x   0 nacho      (501) staff       (20)        0 2023-04-02 19:39:01.177558 tsai-0.3.6/tsai.egg-info/
--rw-r--r--   0 nacho      (501) staff       (20)    15975 2023-04-02 19:39:00.000000 tsai-0.3.6/tsai.egg-info/PKG-INFO
--rw-r--r--   0 nacho      (501) staff       (20)     2343 2023-04-02 19:39:00.000000 tsai-0.3.6/tsai.egg-info/SOURCES.txt
--rw-r--r--   0 nacho      (501) staff       (20)        1 2023-04-02 19:39:00.000000 tsai-0.3.6/tsai.egg-info/dependency_links.txt
--rw-r--r--   0 nacho      (501) staff       (20)       75 2023-04-02 19:39:00.000000 tsai-0.3.6/tsai.egg-info/entry_points.txt
--rw-r--r--   0 nacho      (501) staff       (20)        1 2021-07-01 11:48:36.000000 tsai-0.3.6/tsai.egg-info/not-zip-safe
--rw-r--r--   0 nacho      (501) staff       (20)      184 2023-04-02 19:39:00.000000 tsai-0.3.6/tsai.egg-info/requires.txt
--rw-r--r--   0 nacho      (501) staff       (20)        5 2023-04-02 19:39:00.000000 tsai-0.3.6/tsai.egg-info/top_level.txt
+drwxr-xr-x   0 nacho      (501) staff       (20)        0 2023-07-02 20:47:40.147092 tsai-0.3.7/
+-rw-r--r--   0 nacho      (501) staff       (20)     5400 2023-03-31 19:52:01.000000 tsai-0.3.7/CONTRIBUTING.md
+-rw-r--r--   0 nacho      (501) staff       (20)    11357 2021-04-15 15:58:44.000000 tsai-0.3.7/LICENSE
+-rw-r--r--   0 nacho      (501) staff       (20)      111 2021-04-15 15:58:44.000000 tsai-0.3.7/MANIFEST.in
+-rw-r--r--   0 nacho      (501) staff       (20)    15975 2023-07-02 20:47:40.144676 tsai-0.3.7/PKG-INFO
+-rw-r--r--   0 nacho      (501) staff       (20)    14964 2023-04-01 19:34:41.000000 tsai-0.3.7/README.md
+-rw-r--r--   0 nacho      (501) staff       (20)     1306 2023-07-01 16:57:14.000000 tsai-0.3.7/settings.ini
+-rw-r--r--   0 nacho      (501) staff       (20)       38 2023-07-02 20:47:40.147636 tsai-0.3.7/setup.cfg
+-rw-r--r--   0 nacho      (501) staff       (20)     2864 2022-10-08 18:52:14.000000 tsai-0.3.7/setup.py
+drwxr-xr-x   0 nacho      (501) staff       (20)        0 2023-07-02 20:47:39.924392 tsai-0.3.7/tsai/
+-rw-r--r--   0 nacho      (501) staff       (20)       21 2023-07-02 16:51:28.000000 tsai-0.3.7/tsai/__init__.py
+-rw-r--r--   0 nacho      (501) staff       (20)   368063 2023-07-02 16:51:30.000000 tsai-0.3.7/tsai/_modidx.py
+-rw-r--r--   0 nacho      (501) staff       (20)    42866 2022-10-08 12:17:23.000000 tsai-0.3.7/tsai/_nbdev.py
+-rw-r--r--   0 nacho      (501) staff       (20)      392 2022-03-01 14:30:56.000000 tsai-0.3.7/tsai/all.py
+-rw-r--r--   0 nacho      (501) staff       (20)    22352 2023-07-02 16:51:26.000000 tsai-0.3.7/tsai/analysis.py
+-rw-r--r--   0 nacho      (501) staff       (20)      335 2022-03-01 14:31:40.000000 tsai-0.3.7/tsai/basics.py
+-rw-r--r--   0 nacho      (501) staff       (20)     6755 2023-07-02 16:51:26.000000 tsai-0.3.7/tsai/calibration.py
+drwxr-xr-x   0 nacho      (501) staff       (20)        0 2023-07-02 20:47:39.952360 tsai-0.3.7/tsai/callback/
+-rw-r--r--   0 nacho      (501) staff       (20)    13868 2023-07-02 16:51:26.000000 tsai-0.3.7/tsai/callback/MVP.py
+-rw-r--r--   0 nacho      (501) staff       (20)     8602 2023-07-02 16:51:26.000000 tsai-0.3.7/tsai/callback/PredictionDynamics.py
+-rw-r--r--   0 nacho      (501) staff       (20)        0 2023-07-02 16:51:28.000000 tsai-0.3.7/tsai/callback/__init__.py
+-rw-r--r--   0 nacho      (501) staff       (20)      129 2022-03-01 14:34:50.000000 tsai-0.3.7/tsai/callback/all.py
+-rw-r--r--   0 nacho      (501) staff       (20)    14220 2023-07-02 16:51:26.000000 tsai-0.3.7/tsai/callback/core.py
+-rw-r--r--   0 nacho      (501) staff       (20)     8961 2023-07-02 16:51:26.000000 tsai-0.3.7/tsai/callback/experimental.py
+-rw-r--r--   0 nacho      (501) staff       (20)     5199 2023-07-02 16:51:26.000000 tsai-0.3.7/tsai/callback/noisy_student.py
+drwxr-xr-x   0 nacho      (501) staff       (20)        0 2023-07-02 20:47:39.995927 tsai-0.3.7/tsai/data/
+-rw-r--r--   0 nacho      (501) staff       (20)        0 2023-07-02 16:51:28.000000 tsai-0.3.7/tsai/data/__init__.py
+-rw-r--r--   0 nacho      (501) staff       (20)      328 2022-03-03 08:27:56.000000 tsai-0.3.7/tsai/data/all.py
+-rw-r--r--   0 nacho      (501) staff       (20)      185 2022-03-01 14:32:50.000000 tsai-0.3.7/tsai/data/basics.py
+-rw-r--r--   0 nacho      (501) staff       (20)    51475 2023-07-02 16:51:25.000000 tsai-0.3.7/tsai/data/core.py
+-rw-r--r--   0 nacho      (501) staff       (20)   149570 2023-07-02 16:51:25.000000 tsai-0.3.7/tsai/data/external.py
+-rw-r--r--   0 nacho      (501) staff       (20)     1896 2023-07-02 16:51:26.000000 tsai-0.3.7/tsai/data/features.py
+-rw-r--r--   0 nacho      (501) staff       (20)     9503 2023-07-02 16:51:25.000000 tsai-0.3.7/tsai/data/image.py
+-rw-r--r--   0 nacho      (501) staff       (20)     3069 2023-07-02 16:51:25.000000 tsai-0.3.7/tsai/data/metadatasets.py
+-rw-r--r--   0 nacho      (501) staff       (20)     6906 2023-07-02 16:51:26.000000 tsai-0.3.7/tsai/data/mixed.py
+-rw-r--r--   0 nacho      (501) staff       (20)     5119 2023-07-02 16:51:25.000000 tsai-0.3.7/tsai/data/mixed_augmentation.py
+-rw-r--r--   0 nacho      (501) staff       (20)    47787 2023-07-02 16:51:24.000000 tsai-0.3.7/tsai/data/preparation.py
+-rw-r--r--   0 nacho      (501) staff       (20)    81947 2023-07-02 16:51:25.000000 tsai-0.3.7/tsai/data/preprocessing.py
+-rw-r--r--   0 nacho      (501) staff       (20)     3112 2023-07-02 16:51:26.000000 tsai-0.3.7/tsai/data/tabular.py
+-rw-r--r--   0 nacho      (501) staff       (20)    45120 2023-07-02 16:51:25.000000 tsai-0.3.7/tsai/data/transforms.py
+-rw-r--r--   0 nacho      (501) staff       (20)     3470 2023-07-02 16:51:25.000000 tsai-0.3.7/tsai/data/unwindowed.py
+-rw-r--r--   0 nacho      (501) staff       (20)    34525 2023-07-02 16:51:24.000000 tsai-0.3.7/tsai/data/validation.py
+-rw-r--r--   0 nacho      (501) staff       (20)    10877 2023-07-02 16:51:23.000000 tsai-0.3.7/tsai/export.py
+-rw-r--r--   0 nacho      (501) staff       (20)    12995 2023-06-27 07:20:40.000000 tsai-0.3.7/tsai/imports.py
+-rw-r--r--   0 nacho      (501) staff       (20)      103 2022-04-30 11:41:05.000000 tsai-0.3.7/tsai/index.py
+-rw-r--r--   0 nacho      (501) staff       (20)     1125 2023-07-02 16:51:26.000000 tsai-0.3.7/tsai/inference.py
+-rw-r--r--   0 nacho      (501) staff       (20)    27545 2023-07-02 16:51:26.000000 tsai-0.3.7/tsai/learner.py
+-rw-r--r--   0 nacho      (501) staff       (20)     6287 2023-07-02 16:51:26.000000 tsai-0.3.7/tsai/losses.py
+-rw-r--r--   0 nacho      (501) staff       (20)     8344 2023-07-02 16:51:26.000000 tsai-0.3.7/tsai/metrics.py
+drwxr-xr-x   0 nacho      (501) staff       (20)        0 2023-07-02 20:47:40.140592 tsai-0.3.7/tsai/models/
+-rw-r--r--   0 nacho      (501) staff       (20)      803 2023-07-02 16:51:27.000000 tsai-0.3.7/tsai/models/FCN.py
+-rw-r--r--   0 nacho      (501) staff       (20)     2533 2023-07-02 16:51:27.000000 tsai-0.3.7/tsai/models/FCNPlus.py
+-rw-r--r--   0 nacho      (501) staff       (20)     1719 2023-07-02 16:51:28.000000 tsai-0.3.7/tsai/models/GatedTabTransformer.py
+-rw-r--r--   0 nacho      (501) staff       (20)     2961 2023-07-02 16:51:27.000000 tsai-0.3.7/tsai/models/InceptionTime.py
+-rw-r--r--   0 nacho      (501) staff       (20)     9867 2023-07-02 16:51:27.000000 tsai-0.3.7/tsai/models/InceptionTimePlus.py
+-rw-r--r--   0 nacho      (501) staff       (20)     8927 2023-07-02 16:51:27.000000 tsai-0.3.7/tsai/models/MINIROCKET.py
+-rw-r--r--   0 nacho      (501) staff       (20)    15510 2023-07-02 16:51:27.000000 tsai-0.3.7/tsai/models/MINIROCKETPlus_Pytorch.py
+-rw-r--r--   0 nacho      (501) staff       (20)     9541 2023-07-02 16:51:27.000000 tsai-0.3.7/tsai/models/MINIROCKET_Pytorch.py
+-rw-r--r--   0 nacho      (501) staff       (20)     1192 2023-07-02 16:51:27.000000 tsai-0.3.7/tsai/models/MLP.py
+-rw-r--r--   0 nacho      (501) staff       (20)     3130 2023-07-02 16:51:28.000000 tsai-0.3.7/tsai/models/MultiInputNet.py
+-rw-r--r--   0 nacho      (501) staff       (20)    13189 2023-07-02 16:51:28.000000 tsai-0.3.7/tsai/models/MultiRocketPlus.py
+-rw-r--r--   0 nacho      (501) staff       (20)     4601 2023-07-02 16:51:27.000000 tsai-0.3.7/tsai/models/OmniScaleCNN.py
+-rw-r--r--   0 nacho      (501) staff       (20)    19902 2023-07-02 16:51:27.000000 tsai-0.3.7/tsai/models/PatchTST.py
+-rw-r--r--   0 nacho      (501) staff       (20)     2189 2023-07-02 16:51:27.000000 tsai-0.3.7/tsai/models/RNN.py
+-rw-r--r--   0 nacho      (501) staff       (20)    10187 2023-07-02 16:51:28.000000 tsai-0.3.7/tsai/models/RNNAttention.py
+-rw-r--r--   0 nacho      (501) staff       (20)     6231 2023-07-02 16:51:27.000000 tsai-0.3.7/tsai/models/RNNPlus.py
+-rw-r--r--   0 nacho      (501) staff       (20)     3053 2023-07-02 16:51:27.000000 tsai-0.3.7/tsai/models/RNN_FCN.py
+-rw-r--r--   0 nacho      (501) staff       (20)     4315 2023-07-02 16:51:27.000000 tsai-0.3.7/tsai/models/RNN_FCNPlus.py
+-rw-r--r--   0 nacho      (501) staff       (20)     4356 2023-07-02 16:51:27.000000 tsai-0.3.7/tsai/models/ROCKET.py
+-rw-r--r--   0 nacho      (501) staff       (20)     3049 2023-07-02 16:51:27.000000 tsai-0.3.7/tsai/models/ROCKET_Pytorch.py
+-rw-r--r--   0 nacho      (501) staff       (20)     1973 2023-07-02 16:51:27.000000 tsai-0.3.7/tsai/models/ResCNN.py
+-rw-r--r--   0 nacho      (501) staff       (20)     1492 2023-07-02 16:51:27.000000 tsai-0.3.7/tsai/models/ResNet.py
+-rw-r--r--   0 nacho      (501) staff       (20)     3508 2023-07-02 16:51:27.000000 tsai-0.3.7/tsai/models/ResNetPlus.py
+-rw-r--r--   0 nacho      (501) staff       (20)     2879 2023-07-02 16:51:27.000000 tsai-0.3.7/tsai/models/TCN.py
+-rw-r--r--   0 nacho      (501) staff       (20)     9879 2023-07-02 16:51:28.000000 tsai-0.3.7/tsai/models/TSPerceiver.py
+-rw-r--r--   0 nacho      (501) staff       (20)    13176 2023-07-02 16:51:28.000000 tsai-0.3.7/tsai/models/TSSequencerPlus.py
+-rw-r--r--   0 nacho      (501) staff       (20)    10674 2023-07-02 16:51:27.000000 tsai-0.3.7/tsai/models/TST.py
+-rw-r--r--   0 nacho      (501) staff       (20)    19652 2023-07-02 16:51:27.000000 tsai-0.3.7/tsai/models/TSTPlus.py
+-rw-r--r--   0 nacho      (501) staff       (20)    14086 2023-07-02 16:51:28.000000 tsai-0.3.7/tsai/models/TSiTPlus.py
+-rw-r--r--   0 nacho      (501) staff       (20)    14453 2023-07-02 16:51:28.000000 tsai-0.3.7/tsai/models/TabFusionTransformer.py
+-rw-r--r--   0 nacho      (501) staff       (20)     3004 2023-07-02 16:51:27.000000 tsai-0.3.7/tsai/models/TabModel.py
+-rw-r--r--   0 nacho      (501) staff       (20)    12863 2023-07-02 16:51:27.000000 tsai-0.3.7/tsai/models/TabTransformer.py
+-rw-r--r--   0 nacho      (501) staff       (20)     2194 2023-07-02 16:51:27.000000 tsai-0.3.7/tsai/models/TransformerModel.py
+-rw-r--r--   0 nacho      (501) staff       (20)     5495 2023-07-02 16:51:28.000000 tsai-0.3.7/tsai/models/TransformerRNNPlus.py
+-rw-r--r--   0 nacho      (501) staff       (20)     4200 2023-07-02 16:51:27.000000 tsai-0.3.7/tsai/models/XCM.py
+-rw-r--r--   0 nacho      (501) staff       (20)     4712 2023-07-02 16:51:27.000000 tsai-0.3.7/tsai/models/XCMPlus.py
+-rw-r--r--   0 nacho      (501) staff       (20)     2213 2023-07-02 16:51:27.000000 tsai-0.3.7/tsai/models/XResNet1d.py
+-rw-r--r--   0 nacho      (501) staff       (20)     5507 2023-07-02 16:51:27.000000 tsai-0.3.7/tsai/models/XResNet1dPlus.py
+-rw-r--r--   0 nacho      (501) staff       (20)     3298 2023-07-02 16:51:27.000000 tsai-0.3.7/tsai/models/XceptionTime.py
+-rw-r--r--   0 nacho      (501) staff       (20)     5063 2023-07-02 16:51:27.000000 tsai-0.3.7/tsai/models/XceptionTimePlus.py
+-rw-r--r--   0 nacho      (501) staff       (20)        0 2023-07-02 16:51:28.000000 tsai-0.3.7/tsai/models/__init__.py
+-rw-r--r--   0 nacho      (501) staff       (20)     1275 2023-06-17 09:15:44.000000 tsai-0.3.7/tsai/models/all.py
+-rw-r--r--   0 nacho      (501) staff       (20)     2401 2023-07-02 16:51:27.000000 tsai-0.3.7/tsai/models/explainability.py
+-rw-r--r--   0 nacho      (501) staff       (20)     2428 2023-07-02 16:51:27.000000 tsai-0.3.7/tsai/models/gMLP.py
+-rw-r--r--   0 nacho      (501) staff       (20)    62786 2023-07-02 16:51:26.000000 tsai-0.3.7/tsai/models/layers.py
+-rw-r--r--   0 nacho      (501) staff       (20)     4232 2023-07-02 16:51:27.000000 tsai-0.3.7/tsai/models/mWDN.py
+-rw-r--r--   0 nacho      (501) staff       (20)     1958 2023-07-02 16:51:28.000000 tsai-0.3.7/tsai/models/misc.py
+-rw-r--r--   0 nacho      (501) staff       (20)    16841 2023-07-02 16:51:28.000000 tsai-0.3.7/tsai/models/multimodal.py
+-rw-r--r--   0 nacho      (501) staff       (20)     1775 2023-07-02 16:51:27.000000 tsai-0.3.7/tsai/models/positional_encoders.py
+-rw-r--r--   0 nacho      (501) staff       (20)    15376 2023-07-02 16:51:27.000000 tsai-0.3.7/tsai/models/utils.py
+-rw-r--r--   0 nacho      (501) staff       (20)      328 2023-07-02 16:51:26.000000 tsai-0.3.7/tsai/optimizer.py
+-rw-r--r--   0 nacho      (501) staff       (20)     6592 2023-07-02 16:51:28.000000 tsai-0.3.7/tsai/optuna.py
+-rw-r--r--   0 nacho      (501) staff       (20)    16303 2023-07-02 16:51:26.000000 tsai-0.3.7/tsai/tslearner.py
+-rw-r--r--   0 nacho      (501) staff       (20)      111 2022-10-08 12:17:15.000000 tsai-0.3.7/tsai/tutorials.py
+-rw-r--r--   0 nacho      (501) staff       (20)    66311 2023-07-02 16:51:24.000000 tsai-0.3.7/tsai/utils.py
+-rw-r--r--   0 nacho      (501) staff       (20)     2543 2023-07-02 16:51:28.000000 tsai-0.3.7/tsai/wandb.py
+drwxr-xr-x   0 nacho      (501) staff       (20)        0 2023-07-02 20:47:39.937560 tsai-0.3.7/tsai.egg-info/
+-rw-r--r--   0 nacho      (501) staff       (20)    15975 2023-07-02 20:47:39.000000 tsai-0.3.7/tsai.egg-info/PKG-INFO
+-rw-r--r--   0 nacho      (501) staff       (20)     2434 2023-07-02 20:47:39.000000 tsai-0.3.7/tsai.egg-info/SOURCES.txt
+-rw-r--r--   0 nacho      (501) staff       (20)        1 2023-07-02 20:47:39.000000 tsai-0.3.7/tsai.egg-info/dependency_links.txt
+-rw-r--r--   0 nacho      (501) staff       (20)       75 2023-07-02 20:47:39.000000 tsai-0.3.7/tsai.egg-info/entry_points.txt
+-rw-r--r--   0 nacho      (501) staff       (20)        1 2021-07-01 11:48:36.000000 tsai-0.3.7/tsai.egg-info/not-zip-safe
+-rw-r--r--   0 nacho      (501) staff       (20)      207 2023-07-02 20:47:39.000000 tsai-0.3.7/tsai.egg-info/requires.txt
+-rw-r--r--   0 nacho      (501) staff       (20)        5 2023-07-02 20:47:39.000000 tsai-0.3.7/tsai.egg-info/top_level.txt
```

### Comparing `tsai-0.3.6/CONTRIBUTING.md` & `tsai-0.3.7/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `tsai-0.3.6/LICENSE` & `tsai-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `tsai-0.3.6/PKG-INFO` & `tsai-0.3.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsai
-Version: 0.3.6
+Version: 0.3.7
 Summary: Practical Deep Learning for Time Series / Sequential Data library based on fastai & Pytorch
 Home-page: https://github.com/timeseriesAI/tsai/
 Author: Ignacio Oguiza and contributors
 Author-email: oguiza@timeseriesAI.co
 License: Apache Software License 2.0
 Project-URL: Documentation, https://timeseriesAI.github.io/tsai/
 Keywords: fastai time-series time-series-classification time-series-regression deep-learning Pytorch
```

### Comparing `tsai-0.3.6/README.md` & `tsai-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `tsai-0.3.6/settings.ini` & `tsai-0.3.7/settings.ini`

 * *Files 5% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 [DEFAULT]
 host = github
 lib_name = tsai
 repo = tsai
 user = timeseriesAI
 branch = main
-version = 0.3.6
+version = 0.3.7
 description = Practical Deep Learning for Time Series / Sequential Data library based on fastai & Pytorch
 keywords = fastai time-series time-series-classification time-series-regression deep-learning Pytorch
 author = Ignacio Oguiza and contributors
 author_email = oguiza@timeseriesAI.co
 copyright = Ignacio Oguiza
 license = apache2
 status = 4
 min_python = 3.7
 audience = Developers
 language = English
-requirements = fastai>=2.7.12 pyts>=0.12.0 imbalanced-learn>=0.8.0 psutil>=5.4.8
+requirements = fastai>=2.7.12 pyts>=0.12.0 imbalanced-learn>=0.8.0 psutil>=5.4.8 scikit-learn>=1.2,<1.3
 pip_requirements = torch>=1.7,<2.1
 conda_user = timeseriesAI
 conda_requirements = pytorch>=1.7,<2.1
 extra_requirements = sktime>=0.10.1 tsfresh>=0.18.0 PyWavelets>=1.1.1 nbformat>=5.1.3
 dev_requirements = nbdev>2 ipykernel>6
 console_scripts = nb2py=tsai.export:nb2py
 nbs_path = nbs
 doc_path = _docs
 doc_host = https://timeseriesAI.github.io/tsai
 doc_baseurl = /
 git_url = https://github.com/timeseriesAI/tsai/
 lib_path = tsai
 title = tsai
-tst_flags = slow extras onnx
+tst_flags = local slow extras onnx
 custom_sidebar = True
 recursive = True
 clean_ids = True
 black_formatting = False
 readme_nb = index.ipynb
 allowed_metadata_keys =
 allowed_cell_metadata_keys =
```

### Comparing `tsai-0.3.6/setup.py` & `tsai-0.3.7/setup.py`

 * *Files identical despite different names*

### Comparing `tsai-0.3.6/tsai/_modidx.py` & `tsai-0.3.7/tsai/_modidx.py`

 * *Files 3% similar despite different names*

```diff
@@ -279,16 +279,22 @@
                                 'tsai.data.core.TSDataset': ('data.core.html#tsdataset', 'tsai/data/core.py'),
                                 'tsai.data.core.TSDataset.__getitem__': ('data.core.html#tsdataset.__getitem__', 'tsai/data/core.py'),
                                 'tsai.data.core.TSDataset.__init__': ('data.core.html#tsdataset.__init__', 'tsai/data/core.py'),
                                 'tsai.data.core.TSDataset.__len__': ('data.core.html#tsdataset.__len__', 'tsai/data/core.py'),
                                 'tsai.data.core.TSDatasets': ('data.core.html#tsdatasets', 'tsai/data/core.py'),
                                 'tsai.data.core.TSDatasets.__getitem__': ('data.core.html#tsdatasets.__getitem__', 'tsai/data/core.py'),
                                 'tsai.data.core.TSDatasets.__init__': ('data.core.html#tsdatasets.__init__', 'tsai/data/core.py'),
+                                'tsai.data.core.TSDatasets.__len__': ('data.core.html#tsdatasets.__len__', 'tsai/data/core.py'),
+                                'tsai.data.core.TSDatasets.__repr__': ('data.core.html#tsdatasets.__repr__', 'tsai/data/core.py'),
                                 'tsai.data.core.TSDatasets._new': ('data.core.html#tsdatasets._new', 'tsai/data/core.py'),
+                                'tsai.data.core.TSDatasets.add_dataset': ('data.core.html#tsdatasets.add_dataset', 'tsai/data/core.py'),
+                                'tsai.data.core.TSDatasets.add_test': ('data.core.html#tsdatasets.add_test', 'tsai/data/core.py'),
+                                'tsai.data.core.TSDatasets.add_unlabeled': ('data.core.html#tsdatasets.add_unlabeled', 'tsai/data/core.py'),
                                 'tsai.data.core.TSDatasets.new_empty': ('data.core.html#tsdatasets.new_empty', 'tsai/data/core.py'),
+                                'tsai.data.core.TSDatasets.show_at': ('data.core.html#tsdatasets.show_at', 'tsai/data/core.py'),
                                 'tsai.data.core.TSDatasets.subset': ('data.core.html#tsdatasets.subset', 'tsai/data/core.py'),
                                 'tsai.data.core.TSLabelTensor': ('data.core.html#tslabeltensor', 'tsai/data/core.py'),
                                 'tsai.data.core.TSLabelTensor.__repr__': ('data.core.html#tslabeltensor.__repr__', 'tsai/data/core.py'),
                                 'tsai.data.core.TSMaskTensor': ('data.core.html#tsmasktensor', 'tsai/data/core.py'),
                                 'tsai.data.core.TSMaskTensor.__repr__': ('data.core.html#tsmasktensor.__repr__', 'tsai/data/core.py'),
                                 'tsai.data.core.TSMultiLabelClassification': ( 'data.core.html#tsmultilabelclassification',
                                                                                'tsai/data/core.py'),
@@ -564,14 +570,20 @@
                                          'tsai.data.preprocessing.OneHot': ('data.preprocessing.html#onehot', 'tsai/data/preprocessing.py'),
                                          'tsai.data.preprocessing.OneHot.__init__': ( 'data.preprocessing.html#onehot.__init__',
                                                                                       'tsai/data/preprocessing.py'),
                                          'tsai.data.preprocessing.OneHot.decodes': ( 'data.preprocessing.html#onehot.decodes',
                                                                                      'tsai/data/preprocessing.py'),
                                          'tsai.data.preprocessing.OneHot.encodes': ( 'data.preprocessing.html#onehot.encodes',
                                                                                      'tsai/data/preprocessing.py'),
+                                         'tsai.data.preprocessing.PatchEncoder': ( 'data.preprocessing.html#patchencoder',
+                                                                                   'tsai/data/preprocessing.py'),
+                                         'tsai.data.preprocessing.PatchEncoder.__call__': ( 'data.preprocessing.html#patchencoder.__call__',
+                                                                                            'tsai/data/preprocessing.py'),
+                                         'tsai.data.preprocessing.PatchEncoder.__init__': ( 'data.preprocessing.html#patchencoder.__init__',
+                                                                                            'tsai/data/preprocessing.py'),
                                          'tsai.data.preprocessing.Preprocessor': ( 'data.preprocessing.html#preprocessor',
                                                                                    'tsai/data/preprocessing.py'),
                                          'tsai.data.preprocessing.Preprocessor.__init__': ( 'data.preprocessing.html#preprocessor.__init__',
                                                                                             'tsai/data/preprocessing.py'),
                                          'tsai.data.preprocessing.Preprocessor.fit': ( 'data.preprocessing.html#preprocessor.fit',
                                                                                        'tsai/data/preprocessing.py'),
                                          'tsai.data.preprocessing.Preprocessor.inverse_transform': ( 'data.preprocessing.html#preprocessor.inverse_transform',
@@ -593,14 +605,24 @@
                                                                                                       'tsai/data/preprocessing.py'),
                                          'tsai.data.preprocessing.TSAddMissingTimestamps.fit': ( 'data.preprocessing.html#tsaddmissingtimestamps.fit',
                                                                                                  'tsai/data/preprocessing.py'),
                                          'tsai.data.preprocessing.TSAddMissingTimestamps.inverse_transform': ( 'data.preprocessing.html#tsaddmissingtimestamps.inverse_transform',
                                                                                                                'tsai/data/preprocessing.py'),
                                          'tsai.data.preprocessing.TSAddMissingTimestamps.transform': ( 'data.preprocessing.html#tsaddmissingtimestamps.transform',
                                                                                                        'tsai/data/preprocessing.py'),
+                                         'tsai.data.preprocessing.TSApplyFunction': ( 'data.preprocessing.html#tsapplyfunction',
+                                                                                      'tsai/data/preprocessing.py'),
+                                         'tsai.data.preprocessing.TSApplyFunction.__init__': ( 'data.preprocessing.html#tsapplyfunction.__init__',
+                                                                                               'tsai/data/preprocessing.py'),
+                                         'tsai.data.preprocessing.TSApplyFunction.fit': ( 'data.preprocessing.html#tsapplyfunction.fit',
+                                                                                          'tsai/data/preprocessing.py'),
+                                         'tsai.data.preprocessing.TSApplyFunction.inverse_transform': ( 'data.preprocessing.html#tsapplyfunction.inverse_transform',
+                                                                                                        'tsai/data/preprocessing.py'),
+                                         'tsai.data.preprocessing.TSApplyFunction.transform': ( 'data.preprocessing.html#tsapplyfunction.transform',
+                                                                                                'tsai/data/preprocessing.py'),
                                          'tsai.data.preprocessing.TSCatEncode': ( 'data.preprocessing.html#tscatencode',
                                                                                   'tsai/data/preprocessing.py'),
                                          'tsai.data.preprocessing.TSCatEncode.__init__': ( 'data.preprocessing.html#tscatencode.__init__',
                                                                                            'tsai/data/preprocessing.py'),
                                          'tsai.data.preprocessing.TSCatEncode.encodes': ( 'data.preprocessing.html#tscatencode.encodes',
                                                                                           'tsai/data/preprocessing.py'),
                                          'tsai.data.preprocessing.TSCategoricalEncoder': ( 'data.preprocessing.html#tscategoricalencoder',
@@ -671,14 +693,24 @@
                                                                                                  'tsai/data/preprocessing.py'),
                                          'tsai.data.preprocessing.TSDropFeatByKey': ( 'data.preprocessing.html#tsdropfeatbykey',
                                                                                       'tsai/data/preprocessing.py'),
                                          'tsai.data.preprocessing.TSDropFeatByKey.__init__': ( 'data.preprocessing.html#tsdropfeatbykey.__init__',
                                                                                                'tsai/data/preprocessing.py'),
                                          'tsai.data.preprocessing.TSDropFeatByKey.encodes': ( 'data.preprocessing.html#tsdropfeatbykey.encodes',
                                                                                               'tsai/data/preprocessing.py'),
+                                         'tsai.data.preprocessing.TSDropIfTrueCols': ( 'data.preprocessing.html#tsdropiftruecols',
+                                                                                       'tsai/data/preprocessing.py'),
+                                         'tsai.data.preprocessing.TSDropIfTrueCols.__init__': ( 'data.preprocessing.html#tsdropiftruecols.__init__',
+                                                                                                'tsai/data/preprocessing.py'),
+                                         'tsai.data.preprocessing.TSDropIfTrueCols.fit': ( 'data.preprocessing.html#tsdropiftruecols.fit',
+                                                                                           'tsai/data/preprocessing.py'),
+                                         'tsai.data.preprocessing.TSDropIfTrueCols.inverse_transform': ( 'data.preprocessing.html#tsdropiftruecols.inverse_transform',
+                                                                                                         'tsai/data/preprocessing.py'),
+                                         'tsai.data.preprocessing.TSDropIfTrueCols.transform': ( 'data.preprocessing.html#tsdropiftruecols.transform',
+                                                                                                 'tsai/data/preprocessing.py'),
                                          'tsai.data.preprocessing.TSDropVars': ( 'data.preprocessing.html#tsdropvars',
                                                                                  'tsai/data/preprocessing.py'),
                                          'tsai.data.preprocessing.TSDropVars.__init__': ( 'data.preprocessing.html#tsdropvars.__init__',
                                                                                           'tsai/data/preprocessing.py'),
                                          'tsai.data.preprocessing.TSDropVars.encodes': ( 'data.preprocessing.html#tsdropvars.encodes',
                                                                                          'tsai/data/preprocessing.py'),
                                          'tsai.data.preprocessing.TSFillMissing': ( 'data.preprocessing.html#tsfillmissing',
@@ -766,14 +798,20 @@
                                                                                                'tsai/data/preprocessing.py'),
                                          'tsai.data.preprocessing.TSOneHotEncoder.fit': ( 'data.preprocessing.html#tsonehotencoder.fit',
                                                                                           'tsai/data/preprocessing.py'),
                                          'tsai.data.preprocessing.TSOneHotEncoder.inverse_transform': ( 'data.preprocessing.html#tsonehotencoder.inverse_transform',
                                                                                                         'tsai/data/preprocessing.py'),
                                          'tsai.data.preprocessing.TSOneHotEncoder.transform': ( 'data.preprocessing.html#tsonehotencoder.transform',
                                                                                                 'tsai/data/preprocessing.py'),
+                                         'tsai.data.preprocessing.TSPatchEncoder': ( 'data.preprocessing.html#tspatchencoder',
+                                                                                     'tsai/data/preprocessing.py'),
+                                         'tsai.data.preprocessing.TSPatchEncoder.__init__': ( 'data.preprocessing.html#tspatchencoder.__init__',
+                                                                                              'tsai/data/preprocessing.py'),
+                                         'tsai.data.preprocessing.TSPatchEncoder.encodes': ( 'data.preprocessing.html#tspatchencoder.encodes',
+                                                                                             'tsai/data/preprocessing.py'),
                                          'tsai.data.preprocessing.TSPosition': ( 'data.preprocessing.html#tsposition',
                                                                                  'tsai/data/preprocessing.py'),
                                          'tsai.data.preprocessing.TSPosition.__init__': ( 'data.preprocessing.html#tsposition.__init__',
                                                                                           'tsai/data/preprocessing.py'),
                                          'tsai.data.preprocessing.TSPosition.encodes': ( 'data.preprocessing.html#tsposition.encodes',
                                                                                          'tsai/data/preprocessing.py'),
                                          'tsai.data.preprocessing.TSPositionGaps': ( 'data.preprocessing.html#tspositiongaps',
@@ -788,14 +826,24 @@
                                                                                              'tsai/data/preprocessing.py'),
                                          'tsai.data.preprocessing.TSRobustScale.__repr__': ( 'data.preprocessing.html#tsrobustscale.__repr__',
                                                                                              'tsai/data/preprocessing.py'),
                                          'tsai.data.preprocessing.TSRobustScale.encodes': ( 'data.preprocessing.html#tsrobustscale.encodes',
                                                                                             'tsai/data/preprocessing.py'),
                                          'tsai.data.preprocessing.TSRobustScale.setups': ( 'data.preprocessing.html#tsrobustscale.setups',
                                                                                            'tsai/data/preprocessing.py'),
+                                         'tsai.data.preprocessing.TSRobustScaler': ( 'data.preprocessing.html#tsrobustscaler',
+                                                                                     'tsai/data/preprocessing.py'),
+                                         'tsai.data.preprocessing.TSRobustScaler.__init__': ( 'data.preprocessing.html#tsrobustscaler.__init__',
+                                                                                              'tsai/data/preprocessing.py'),
+                                         'tsai.data.preprocessing.TSRobustScaler.fit': ( 'data.preprocessing.html#tsrobustscaler.fit',
+                                                                                         'tsai/data/preprocessing.py'),
+                                         'tsai.data.preprocessing.TSRobustScaler.inverse_transform': ( 'data.preprocessing.html#tsrobustscaler.inverse_transform',
+                                                                                                       'tsai/data/preprocessing.py'),
+                                         'tsai.data.preprocessing.TSRobustScaler.transform': ( 'data.preprocessing.html#tsrobustscaler.transform',
+                                                                                               'tsai/data/preprocessing.py'),
                                          'tsai.data.preprocessing.TSRollingMean': ( 'data.preprocessing.html#tsrollingmean',
                                                                                     'tsai/data/preprocessing.py'),
                                          'tsai.data.preprocessing.TSRollingMean.__init__': ( 'data.preprocessing.html#tsrollingmean.__init__',
                                                                                              'tsai/data/preprocessing.py'),
                                          'tsai.data.preprocessing.TSRollingMean.encodes': ( 'data.preprocessing.html#tsrollingmean.encodes',
                                                                                             'tsai/data/preprocessing.py'),
                                          'tsai.data.preprocessing.TSSelectColumns': ( 'data.preprocessing.html#tsselectcolumns',
@@ -872,30 +920,48 @@
                                                                                                  'tsai/data/preprocessing.py'),
                                          'tsai.data.preprocessing.TSStepsSinceStart.fit': ( 'data.preprocessing.html#tsstepssincestart.fit',
                                                                                             'tsai/data/preprocessing.py'),
                                          'tsai.data.preprocessing.TSStepsSinceStart.inverse_transform': ( 'data.preprocessing.html#tsstepssincestart.inverse_transform',
                                                                                                           'tsai/data/preprocessing.py'),
                                          'tsai.data.preprocessing.TSStepsSinceStart.transform': ( 'data.preprocessing.html#tsstepssincestart.transform',
                                                                                                   'tsai/data/preprocessing.py'),
+                                         'tsai.data.preprocessing.TSTargetEncoder': ( 'data.preprocessing.html#tstargetencoder',
+                                                                                      'tsai/data/preprocessing.py'),
+                                         'tsai.data.preprocessing.TSTargetEncoder.__init__': ( 'data.preprocessing.html#tstargetencoder.__init__',
+                                                                                               'tsai/data/preprocessing.py'),
+                                         'tsai.data.preprocessing.TSTargetEncoder.fit': ( 'data.preprocessing.html#tstargetencoder.fit',
+                                                                                          'tsai/data/preprocessing.py'),
+                                         'tsai.data.preprocessing.TSTargetEncoder.inverse_transform': ( 'data.preprocessing.html#tstargetencoder.inverse_transform',
+                                                                                                        'tsai/data/preprocessing.py'),
+                                         'tsai.data.preprocessing.TSTargetEncoder.transform': ( 'data.preprocessing.html#tstargetencoder.transform',
+                                                                                                'tsai/data/preprocessing.py'),
                                          'tsai.data.preprocessing.TSTensor.mul_max': ( 'data.preprocessing.html#tstensor.mul_max',
                                                                                        'tsai/data/preprocessing.py'),
                                          'tsai.data.preprocessing.TSTensor.mul_min': ( 'data.preprocessing.html#tstensor.mul_min',
                                                                                        'tsai/data/preprocessing.py'),
+                                         'tsai.data.preprocessing.TSTuplePatchEncoder': ( 'data.preprocessing.html#tstuplepatchencoder',
+                                                                                          'tsai/data/preprocessing.py'),
+                                         'tsai.data.preprocessing.TSTuplePatchEncoder.__init__': ( 'data.preprocessing.html#tstuplepatchencoder.__init__',
+                                                                                                   'tsai/data/preprocessing.py'),
+                                         'tsai.data.preprocessing.TSTuplePatchEncoder.encodes': ( 'data.preprocessing.html#tstuplepatchencoder.encodes',
+                                                                                                  'tsai/data/preprocessing.py'),
                                          'tsai.data.preprocessing.ToNumpyCategory': ( 'data.preprocessing.html#tonumpycategory',
                                                                                       'tsai/data/preprocessing.py'),
                                          'tsai.data.preprocessing.ToNumpyCategory.__init__': ( 'data.preprocessing.html#tonumpycategory.__init__',
                                                                                                'tsai/data/preprocessing.py'),
                                          'tsai.data.preprocessing.ToNumpyCategory.decodes': ( 'data.preprocessing.html#tonumpycategory.decodes',
                                                                                               'tsai/data/preprocessing.py'),
                                          'tsai.data.preprocessing.ToNumpyCategory.encodes': ( 'data.preprocessing.html#tonumpycategory.encodes',
                                                                                               'tsai/data/preprocessing.py'),
                                          'tsai.data.preprocessing.get_random_stats': ( 'data.preprocessing.html#get_random_stats',
                                                                                        'tsai/data/preprocessing.py'),
                                          'tsai.data.preprocessing.get_stats_with_uncertainty': ( 'data.preprocessing.html#get_stats_with_uncertainty',
                                                                                                  'tsai/data/preprocessing.py'),
+                                         'tsai.data.preprocessing.object2date': ( 'data.preprocessing.html#object2date',
+                                                                                  'tsai/data/preprocessing.py'),
                                          'tsai.data.preprocessing.torch.Tensor.mul_max': ( 'data.preprocessing.html#torch.tensor.mul_max',
                                                                                            'tsai/data/preprocessing.py'),
                                          'tsai.data.preprocessing.torch.Tensor.mul_min': ( 'data.preprocessing.html#torch.tensor.mul_min',
                                                                                            'tsai/data/preprocessing.py')},
             'tsai.data.tabular': { 'tsai.data.tabular.get_tabular_dls': ('data.tabular.html#get_tabular_dls', 'tsai/data/tabular.py'),
                                    'tsai.data.tabular.get_tabular_ds': ('data.tabular.html#get_tabular_ds', 'tsai/data/tabular.py'),
                                    'tsai.data.tabular.preprocess_df': ('data.tabular.html#preprocess_df', 'tsai/data/tabular.py')},
@@ -1082,14 +1148,18 @@
                                       'tsai.data.transforms.TSResampleSteps.encodes': ( 'data.transforms.html#tsresamplesteps.encodes',
                                                                                         'tsai/data/transforms.py'),
                                       'tsai.data.transforms.TSResize': ('data.transforms.html#tsresize', 'tsai/data/transforms.py'),
                                       'tsai.data.transforms.TSResize.__init__': ( 'data.transforms.html#tsresize.__init__',
                                                                                   'tsai/data/transforms.py'),
                                       'tsai.data.transforms.TSResize.encodes': ( 'data.transforms.html#tsresize.encodes',
                                                                                  'tsai/data/transforms.py'),
+                                      'tsai.data.transforms.TSSelfDropout': ( 'data.transforms.html#tsselfdropout',
+                                                                              'tsai/data/transforms.py'),
+                                      'tsai.data.transforms.TSSelfDropout.encodes': ( 'data.transforms.html#tsselfdropout.encodes',
+                                                                                      'tsai/data/transforms.py'),
                                       'tsai.data.transforms.TSShuffleSteps': ( 'data.transforms.html#tsshufflesteps',
                                                                                'tsai/data/transforms.py'),
                                       'tsai.data.transforms.TSShuffleSteps.__init__': ( 'data.transforms.html#tsshufflesteps.__init__',
                                                                                         'tsai/data/transforms.py'),
                                       'tsai.data.transforms.TSShuffleSteps.encodes': ( 'data.transforms.html#tsshufflesteps.encodes',
                                                                                        'tsai/data/transforms.py'),
                                       'tsai.data.transforms.TSShuffle_HLs': ( 'data.transforms.html#tsshuffle_hls',
@@ -1156,15 +1226,16 @@
                                       'tsai.data.transforms.random_cum_curve_generator': ( 'data.transforms.html#random_cum_curve_generator',
                                                                                            'tsai/data/transforms.py'),
                                       'tsai.data.transforms.random_cum_linear_generator': ( 'data.transforms.html#random_cum_linear_generator',
                                                                                             'tsai/data/transforms.py'),
                                       'tsai.data.transforms.random_cum_noise_generator': ( 'data.transforms.html#random_cum_noise_generator',
                                                                                            'tsai/data/transforms.py'),
                                       'tsai.data.transforms.random_curve_generator': ( 'data.transforms.html#random_curve_generator',
-                                                                                       'tsai/data/transforms.py')},
+                                                                                       'tsai/data/transforms.py'),
+                                      'tsai.data.transforms.self_mask': ('data.transforms.html#self_mask', 'tsai/data/transforms.py')},
             'tsai.data.unwindowed': { 'tsai.data.unwindowed.TSUnwindowedDataset': ( 'data.unwindowed.html#tsunwindoweddataset',
                                                                                     'tsai/data/unwindowed.py'),
                                       'tsai.data.unwindowed.TSUnwindowedDataset.__getitem__': ( 'data.unwindowed.html#tsunwindoweddataset.__getitem__',
                                                                                                 'tsai/data/unwindowed.py'),
                                       'tsai.data.unwindowed.TSUnwindowedDataset.__init__': ( 'data.unwindowed.html#tsunwindoweddataset.__init__',
                                                                                              'tsai/data/unwindowed.py'),
                                       'tsai.data.unwindowed.TSUnwindowedDataset.__len__': ( 'data.unwindowed.html#tsunwindoweddataset.__len__',
@@ -1485,14 +1556,58 @@
                                  'tsai.models.MLP.MLP.forward': ('models.mlp.html#mlp.forward', 'tsai/models/MLP.py')},
             'tsai.models.MultiInputNet': { 'tsai.models.MultiInputNet.MultiInputNet': ( 'models.multiinputnet.html#multiinputnet',
                                                                                         'tsai/models/MultiInputNet.py'),
                                            'tsai.models.MultiInputNet.MultiInputNet.__init__': ( 'models.multiinputnet.html#multiinputnet.__init__',
                                                                                                  'tsai/models/MultiInputNet.py'),
                                            'tsai.models.MultiInputNet.MultiInputNet.forward': ( 'models.multiinputnet.html#multiinputnet.forward',
                                                                                                 'tsai/models/MultiInputNet.py')},
+            'tsai.models.MultiRocketPlus': { 'tsai.models.MultiRocketPlus.Flatten': ( 'models.multirocketplus.html#flatten',
+                                                                                      'tsai/models/MultiRocketPlus.py'),
+                                             'tsai.models.MultiRocketPlus.Flatten.forward': ( 'models.multirocketplus.html#flatten.forward',
+                                                                                              'tsai/models/MultiRocketPlus.py'),
+                                             'tsai.models.MultiRocketPlus.MultiRocketBackbonePlus': ( 'models.multirocketplus.html#multirocketbackboneplus',
+                                                                                                      'tsai/models/MultiRocketPlus.py'),
+                                             'tsai.models.MultiRocketPlus.MultiRocketBackbonePlus.__init__': ( 'models.multirocketplus.html#multirocketbackboneplus.__init__',
+                                                                                                               'tsai/models/MultiRocketPlus.py'),
+                                             'tsai.models.MultiRocketPlus.MultiRocketBackbonePlus.forward': ( 'models.multirocketplus.html#multirocketbackboneplus.forward',
+                                                                                                              'tsai/models/MultiRocketPlus.py'),
+                                             'tsai.models.MultiRocketPlus.MultiRocketFeaturesPlus': ( 'models.multirocketplus.html#multirocketfeaturesplus',
+                                                                                                      'tsai/models/MultiRocketPlus.py'),
+                                             'tsai.models.MultiRocketPlus.MultiRocketFeaturesPlus.__init__': ( 'models.multirocketplus.html#multirocketfeaturesplus.__init__',
+                                                                                                               'tsai/models/MultiRocketPlus.py'),
+                                             'tsai.models.MultiRocketPlus.MultiRocketFeaturesPlus.apply_pooling_ops': ( 'models.multirocketplus.html#multirocketfeaturesplus.apply_pooling_ops',
+                                                                                                                        'tsai/models/MultiRocketPlus.py'),
+                                             'tsai.models.MultiRocketPlus.MultiRocketFeaturesPlus.fit': ( 'models.multirocketplus.html#multirocketfeaturesplus.fit',
+                                                                                                          'tsai/models/MultiRocketPlus.py'),
+                                             'tsai.models.MultiRocketPlus.MultiRocketFeaturesPlus.forward': ( 'models.multirocketplus.html#multirocketfeaturesplus.forward',
+                                                                                                              'tsai/models/MultiRocketPlus.py'),
+                                             'tsai.models.MultiRocketPlus.MultiRocketFeaturesPlus.get_bias': ( 'models.multirocketplus.html#multirocketfeaturesplus.get_bias',
+                                                                                                               'tsai/models/MultiRocketPlus.py'),
+                                             'tsai.models.MultiRocketPlus.MultiRocketFeaturesPlus.get_indices': ( 'models.multirocketplus.html#multirocketfeaturesplus.get_indices',
+                                                                                                                  'tsai/models/MultiRocketPlus.py'),
+                                             'tsai.models.MultiRocketPlus.MultiRocketFeaturesPlus.get_quantiles': ( 'models.multirocketplus.html#multirocketfeaturesplus.get_quantiles',
+                                                                                                                    'tsai/models/MultiRocketPlus.py'),
+                                             'tsai.models.MultiRocketPlus.MultiRocketFeaturesPlus.set_channel_combinations': ( 'models.multirocketplus.html#multirocketfeaturesplus.set_channel_combinations',
+                                                                                                                               'tsai/models/MultiRocketPlus.py'),
+                                             'tsai.models.MultiRocketPlus.MultiRocketFeaturesPlus.set_dilations': ( 'models.multirocketplus.html#multirocketfeaturesplus.set_dilations',
+                                                                                                                    'tsai/models/MultiRocketPlus.py'),
+                                             'tsai.models.MultiRocketPlus.MultiRocketPlus': ( 'models.multirocketplus.html#multirocketplus',
+                                                                                              'tsai/models/MultiRocketPlus.py'),
+                                             'tsai.models.MultiRocketPlus.MultiRocketPlus.__init__': ( 'models.multirocketplus.html#multirocketplus.__init__',
+                                                                                                       'tsai/models/MultiRocketPlus.py'),
+                                             'tsai.models.MultiRocketPlus._LPVV': ( 'models.multirocketplus.html#_lpvv',
+                                                                                    'tsai/models/MultiRocketPlus.py'),
+                                             'tsai.models.MultiRocketPlus._MIPV': ( 'models.multirocketplus.html#_mipv',
+                                                                                    'tsai/models/MultiRocketPlus.py'),
+                                             'tsai.models.MultiRocketPlus._MPV': ( 'models.multirocketplus.html#_mpv',
+                                                                                   'tsai/models/MultiRocketPlus.py'),
+                                             'tsai.models.MultiRocketPlus._PPV': ( 'models.multirocketplus.html#_ppv',
+                                                                                   'tsai/models/MultiRocketPlus.py'),
+                                             'tsai.models.MultiRocketPlus._RSPV': ( 'models.multirocketplus.html#_rspv',
+                                                                                    'tsai/models/MultiRocketPlus.py')},
             'tsai.models.OmniScaleCNN': { 'tsai.models.OmniScaleCNN.OmniScaleCNN': ( 'models.omniscalecnn.html#omniscalecnn',
                                                                                      'tsai/models/OmniScaleCNN.py'),
                                           'tsai.models.OmniScaleCNN.OmniScaleCNN.__init__': ( 'models.omniscalecnn.html#omniscalecnn.__init__',
                                                                                               'tsai/models/OmniScaleCNN.py'),
                                           'tsai.models.OmniScaleCNN.OmniScaleCNN.forward': ( 'models.omniscalecnn.html#omniscalecnn.forward',
                                                                                              'tsai/models/OmniScaleCNN.py'),
                                           'tsai.models.OmniScaleCNN.SampaddingConv1D_BN': ( 'models.omniscalecnn.html#sampaddingconv1d_bn',
@@ -2005,14 +2120,30 @@
                                                                                    'tsai/models/TabTransformer.py')},
             'tsai.models.TransformerModel': { 'tsai.models.TransformerModel.TransformerModel': ( 'models.transformermodel.html#transformermodel',
                                                                                                  'tsai/models/TransformerModel.py'),
                                               'tsai.models.TransformerModel.TransformerModel.__init__': ( 'models.transformermodel.html#transformermodel.__init__',
                                                                                                           'tsai/models/TransformerModel.py'),
                                               'tsai.models.TransformerModel.TransformerModel.forward': ( 'models.transformermodel.html#transformermodel.forward',
                                                                                                          'tsai/models/TransformerModel.py')},
+            'tsai.models.TransformerRNNPlus': { 'tsai.models.TransformerRNNPlus.TransformerGRUPlus': ( 'models.transformerrnnplus.html#transformergruplus',
+                                                                                                       'tsai/models/TransformerRNNPlus.py'),
+                                                'tsai.models.TransformerRNNPlus.TransformerLSTMPlus': ( 'models.transformerrnnplus.html#transformerlstmplus',
+                                                                                                        'tsai/models/TransformerRNNPlus.py'),
+                                                'tsai.models.TransformerRNNPlus.TransformerRNNPlus': ( 'models.transformerrnnplus.html#transformerrnnplus',
+                                                                                                       'tsai/models/TransformerRNNPlus.py'),
+                                                'tsai.models.TransformerRNNPlus._TransformerRNNEncoder': ( 'models.transformerrnnplus.html#_transformerrnnencoder',
+                                                                                                           'tsai/models/TransformerRNNPlus.py'),
+                                                'tsai.models.TransformerRNNPlus._TransformerRNNEncoder.__init__': ( 'models.transformerrnnplus.html#_transformerrnnencoder.__init__',
+                                                                                                                    'tsai/models/TransformerRNNPlus.py'),
+                                                'tsai.models.TransformerRNNPlus._TransformerRNNEncoder.forward': ( 'models.transformerrnnplus.html#_transformerrnnencoder.forward',
+                                                                                                                   'tsai/models/TransformerRNNPlus.py'),
+                                                'tsai.models.TransformerRNNPlus._TransformerRNNPlus': ( 'models.transformerrnnplus.html#_transformerrnnplus',
+                                                                                                        'tsai/models/TransformerRNNPlus.py'),
+                                                'tsai.models.TransformerRNNPlus._TransformerRNNPlus.__init__': ( 'models.transformerrnnplus.html#_transformerrnnplus.__init__',
+                                                                                                                 'tsai/models/TransformerRNNPlus.py')},
             'tsai.models.XCM': { 'tsai.models.XCM.XCM': ('models.xcm.html#xcm', 'tsai/models/XCM.py'),
                                  'tsai.models.XCM.XCM.__init__': ('models.xcm.html#xcm.__init__', 'tsai/models/XCM.py'),
                                  'tsai.models.XCM.XCM.create_head': ('models.xcm.html#xcm.create_head', 'tsai/models/XCM.py'),
                                  'tsai.models.XCM.XCM.forward': ('models.xcm.html#xcm.forward', 'tsai/models/XCM.py'),
                                  'tsai.models.XCM.XCM.show_gradcam': ('models.xcm.html#xcm.show_gradcam', 'tsai/models/XCM.py')},
             'tsai.models.XCMPlus': { 'tsai.models.XCMPlus.XCMPlus': ('models.xcmplus.html#xcmplus', 'tsai/models/XCMPlus.py'),
                                      'tsai.models.XCMPlus.XCMPlus.__init__': ( 'models.xcmplus.html#xcmplus.__init__',
@@ -2467,14 +2598,57 @@
                                   'tsai.models.misc.RecursiveWrapper.forward': ( 'models.misc.html#recursivewrapper.forward',
                                                                                  'tsai/models/misc.py'),
                                   'tsai.models.misc.ResidualWrapper': ('models.misc.html#residualwrapper', 'tsai/models/misc.py'),
                                   'tsai.models.misc.ResidualWrapper.__init__': ( 'models.misc.html#residualwrapper.__init__',
                                                                                  'tsai/models/misc.py'),
                                   'tsai.models.misc.ResidualWrapper.forward': ( 'models.misc.html#residualwrapper.forward',
                                                                                 'tsai/models/misc.py')},
+            'tsai.models.multimodal': { 'tsai.models.multimodal.Embeddings': ( 'models.multimodal.html#embeddings',
+                                                                               'tsai/models/multimodal.py'),
+                                        'tsai.models.multimodal.Embeddings.__init__': ( 'models.multimodal.html#embeddings.__init__',
+                                                                                        'tsai/models/multimodal.py'),
+                                        'tsai.models.multimodal.Embeddings.forward': ( 'models.multimodal.html#embeddings.forward',
+                                                                                       'tsai/models/multimodal.py'),
+                                        'tsai.models.multimodal.FusionMLP': ( 'models.multimodal.html#fusionmlp',
+                                                                              'tsai/models/multimodal.py'),
+                                        'tsai.models.multimodal.FusionMLP.__init__': ( 'models.multimodal.html#fusionmlp.__init__',
+                                                                                       'tsai/models/multimodal.py'),
+                                        'tsai.models.multimodal.FusionMLP.forward': ( 'models.multimodal.html#fusionmlp.forward',
+                                                                                      'tsai/models/multimodal.py'),
+                                        'tsai.models.multimodal.MultInputBackboneWrapper': ( 'models.multimodal.html#multinputbackbonewrapper',
+                                                                                             'tsai/models/multimodal.py'),
+                                        'tsai.models.multimodal.MultInputBackboneWrapper.__init__': ( 'models.multimodal.html#multinputbackbonewrapper.__init__',
+                                                                                                      'tsai/models/multimodal.py'),
+                                        'tsai.models.multimodal.MultInputBackboneWrapper.forward': ( 'models.multimodal.html#multinputbackbonewrapper.forward',
+                                                                                                     'tsai/models/multimodal.py'),
+                                        'tsai.models.multimodal.MultInputWrapper': ( 'models.multimodal.html#multinputwrapper',
+                                                                                     'tsai/models/multimodal.py'),
+                                        'tsai.models.multimodal.MultInputWrapper.__init__': ( 'models.multimodal.html#multinputwrapper.__init__',
+                                                                                              'tsai/models/multimodal.py'),
+                                        'tsai.models.multimodal.StaticBackbone': ( 'models.multimodal.html#staticbackbone',
+                                                                                   'tsai/models/multimodal.py'),
+                                        'tsai.models.multimodal.StaticBackbone.__init__': ( 'models.multimodal.html#staticbackbone.__init__',
+                                                                                            'tsai/models/multimodal.py'),
+                                        'tsai.models.multimodal.StaticBackbone.forward': ( 'models.multimodal.html#staticbackbone.forward',
+                                                                                           'tsai/models/multimodal.py'),
+                                        'tsai.models.multimodal.TensorSplitter': ( 'models.multimodal.html#tensorsplitter',
+                                                                                   'tsai/models/multimodal.py'),
+                                        'tsai.models.multimodal.TensorSplitter.__init__': ( 'models.multimodal.html#tensorsplitter.__init__',
+                                                                                            'tsai/models/multimodal.py'),
+                                        'tsai.models.multimodal.TensorSplitter._check_overlap': ( 'models.multimodal.html#tensorsplitter._check_overlap',
+                                                                                                  'tsai/models/multimodal.py'),
+                                        'tsai.models.multimodal.TensorSplitter._to_list': ( 'models.multimodal.html#tensorsplitter._to_list',
+                                                                                            'tsai/models/multimodal.py'),
+                                        'tsai.models.multimodal.TensorSplitter.forward': ( 'models.multimodal.html#tensorsplitter.forward',
+                                                                                           'tsai/models/multimodal.py'),
+                                        'tsai.models.multimodal._to_list': ('models.multimodal.html#_to_list', 'tsai/models/multimodal.py'),
+                                        'tsai.models.multimodal.get_feat_idxs': ( 'models.multimodal.html#get_feat_idxs',
+                                                                                  'tsai/models/multimodal.py'),
+                                        'tsai.models.multimodal.get_o_cont_idxs': ( 'models.multimodal.html#get_o_cont_idxs',
+                                                                                    'tsai/models/multimodal.py')},
             'tsai.models.positional_encoders': { 'tsai.models.positional_encoders.Coord1dPosEncoding': ( 'models.positional_encoders.html#coord1dposencoding',
                                                                                                          'tsai/models/positional_encoders.py'),
                                                  'tsai.models.positional_encoders.Coord2dPosEncoding': ( 'models.positional_encoders.html#coord2dposencoding',
                                                                                                          'tsai/models/positional_encoders.py'),
                                                  'tsai.models.positional_encoders.PositionalEncoding': ( 'models.positional_encoders.html#positionalencoding',
                                                                                                          'tsai/models/positional_encoders.py')},
             'tsai.models.utils': { 'tsai.models.utils.SeqTokenizer': ('models.utils.html#seqtokenizer', 'tsai/models/utils.py'),
@@ -2633,14 +2807,15 @@
                             'tsai.utils.shuffle_along_axis': ('utils.html#shuffle_along_axis', 'tsai/utils.py'),
                             'tsai.utils.sincos_encoding': ('utils.html#sincos_encoding', 'tsai/utils.py'),
                             'tsai.utils.smallest_dtype': ('utils.html#smallest_dtype', 'tsai/utils.py'),
                             'tsai.utils.sort_generator': ('utils.html#sort_generator', 'tsai/utils.py'),
                             'tsai.utils.split_in_chunks': ('utils.html#split_in_chunks', 'tsai/utils.py'),
                             'tsai.utils.stack': ('utils.html#stack', 'tsai/utils.py'),
                             'tsai.utils.stack_pad': ('utils.html#stack_pad', 'tsai/utils.py'),
+                            'tsai.utils.str2callable': ('utils.html#str2callable', 'tsai/utils.py'),
                             'tsai.utils.str2index': ('utils.html#str2index', 'tsai/utils.py'),
                             'tsai.utils.str2list': ('utils.html#str2list', 'tsai/utils.py'),
                             'tsai.utils.test_eq_nan': ('utils.html#test_eq_nan', 'tsai/utils.py'),
                             'tsai.utils.test_error': ('utils.html#test_error', 'tsai/utils.py'),
                             'tsai.utils.test_ge': ('utils.html#test_ge', 'tsai/utils.py'),
                             'tsai.utils.test_gt': ('utils.html#test_gt', 'tsai/utils.py'),
                             'tsai.utils.test_le': ('utils.html#test_le', 'tsai/utils.py'),
```

### Comparing `tsai-0.3.6/tsai/_nbdev.py` & `tsai-0.3.7/tsai/_nbdev.py`

 * *Files identical despite different names*

### Comparing `tsai-0.3.6/tsai/analysis.py` & `tsai-0.3.7/tsai/analysis.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,14 +131,15 @@
     dl.show_batch(b, max_n=k, **kwargs)
 
 # %% ../nbs/020_analysis.ipynb 9
 @patch
 def feature_importance(self:Learner, 
     X=None, # array-like object containing the time series. If None, all data in the validation set will be used.
     y=None, # array-like object containing the targets. If None, all targets in the validation set will be used.
+    bs:int=None, # batch size. If None, the default batch size of the dataloader will be used.
     partial_n:(int, float)=None, # # (int) or % (float) of used to measure feature importance. If None, all data will be used.
     method:str='permutation', # Method used to invalidate feature. Use 'permutation' for shuffling or 'ablation' for setting values to np.nan.
     feature_names:list=None, # Optional list of feature names that will be displayed if available. Otherwise var_0, var_1, etc.
     sel_classes:(str, list)=None, # classes for which the analysis will be made
     key_metric_idx:int=0, # Optional position of the metric used. If None or no metric is available, the loss will be used.
     show_chart:bool=True, # Flag to indicate if a chart showing permutation feature importance will be plotted.
     figsize:tuple=None, # Size of the chart.
@@ -146,16 +147,14 @@
     return_df:bool=True, # Flag to indicate if the dataframe with feature importance will be returned.
     save_df_path:Path=None, # Path where dataframe containing the permutation feature importance results will be saved.
     random_state:int=23, # Optional int that controls the shuffling applied to the data.
     verbose:bool=True, # Flag that controls verbosity.
     ):
     r"""Calculates feature importance as the drop in the model's validation loss or metric when a feature value is randomly shuffled"""
     
-    global output, metric
-    
     assert method in ['permutation', 'ablation']
 
     # X, y
     if X is None:
         X = self.dls.train.dataset.tls[0].items
         if hasattr(self.dls.train.dataset.tls[0], '_splits'): X = X[self.dls.train.dataset.tls[0]._splits]
     if y is None:
@@ -167,14 +166,16 @@
     else: 
         X, y = X[:], y[:]
     if sel_classes is not None:
         filt = np.isin(y, listify(sel_classes))
         X, y = X[filt], y[filt]
     pv(f'X.shape: {X.shape}', verbose)
     pv(f'y.shape: {y.shape}', verbose)
+    if bs is None:
+        bs = self.dls.valid.bs
 
     # Metrics
     metrics = [mn for mn in self.recorder.metric_names if mn not in ['epoch', 'train_loss', 'valid_loss', 'time']]
     if len(metrics) == 0 or key_metric_idx is None:
         metric_name = self.loss_func.__class__.__name__
         key_metric_idx = None
     else:
@@ -220,17 +221,17 @@
                 save_feat = X[:, k].copy()
                 if method == 'permutation':
                     # shuffle along samples & steps
                     X[:, k] = random_shuffle(X[:, k].flatten(), random_state=random_state).reshape(X[:, k].shape)
                 elif method == 'ablation':
                     X[:, k] = np.nan
             if key_metric_idx is None:
-                value = self.get_X_preds(X, y, with_loss=True)[-1].mean().item()
+                value = self.get_X_preds(X, y, with_loss=True, with_decoded=False, bs=bs)[-1].mean().item()
             else:
-                output = self.get_X_preds(X, y)
+                output = self.get_X_preds(X, y, with_decoded=False, bs=bs)
                 if self.dls.c == 2:
                     try: 
                         if sklearn_metric:
                             value = metric(output[1], output[0][:, 1]).item()
                         else:
                             value = metric(output[0][:, 1], output[1]).item()
                     except: 
@@ -301,14 +302,15 @@
 
 # %% ../nbs/020_analysis.ipynb 10
 @patch
 def step_importance(
     self:Learner, 
     X=None, # array-like object containing the time series. If None, all data in the validation set will be used.
     y=None, # array-like object containing the targets. If None, all targets in the validation set will be used.
+    bs:int=None, # batch size used to compute predictions. If None, the batch size used in the validation set will be used.
     partial_n:(int, float)=None, # # (int) or % (float) of used to measure feature importance. If None, all data will be used.
     method:str='permutation', # Method used to invalidate feature. Use 'permutation' for shuffling or 'ablation' for setting values to np.nan.
     step_names:list=None, # Optional list of step names that will be displayed if available. Otherwise 0, 1, 2, etc.
     sel_classes:(str, list)=None, # classes for which the analysis will be made
     n_steps:int=1, # # of steps that will be analyzed at a time. Default is 1.
     key_metric_idx:int=0, # Optional position of the metric used. If None or no metric is available, the loss will be used.
     show_chart:bool=True, # Flag to indicate if a chart showing permutation feature importance will be plotted.
@@ -337,14 +339,16 @@
     else: 
         X, y = X[:], y[:]
     if sel_classes is not None:
         filt = np.isin(y, listify(sel_classes))
         X, y = X[filt], y[filt]
     pv(f'X.shape: {X.shape}', verbose)
     pv(f'y.shape: {y.shape}', verbose)
+    if bs is None:
+        bs = self.dls.valid.bs
 
     # Metrics
     metrics = [mn for mn in self.recorder.metric_names if mn not in ['epoch', 'train_loss', 'valid_loss', 'time']]
     if len(metrics) == 0 or key_metric_idx is None:
         metric_name = self.loss_func.__class__.__name__
         key_metric_idx = None
     else:
@@ -378,17 +382,17 @@
                 save_feat = X[..., k].copy()
                 if method == 'permutation':
                     # shuffle along samples
                     X[..., k] = shuffle_along_axis(X[..., k], axis=0, random_state=random_state)
                 elif method == 'ablation':
                     X[..., k] = np.nan
             if key_metric_idx is None:
-                value = self.get_X_preds(X, y, with_loss=True)[-1].mean().item()
+                value = self.get_X_preds(X, y, bs=bs, with_loss=True, with_decoded=False)[-1].mean().item()
             else:
-                output = self.get_X_preds(X, y)
+                output = self.get_X_preds(X, y, bs=bs, with_decoded=False)
                 if self.dls.c == 2:
                     try: 
                         if sklearn_metric:
                             value = metric(output[1], output[0][:, 1]).item()
                         else:
                             value = metric(output[0][:, 1], output[1]).item()
                     except:
```

### Comparing `tsai-0.3.6/tsai/calibration.py` & `tsai-0.3.7/tsai/calibration.py`

 * *Files identical despite different names*

### Comparing `tsai-0.3.6/tsai/callback/MVP.py` & `tsai-0.3.7/tsai/callback/MVP.py`

 * *Files identical despite different names*

### Comparing `tsai-0.3.6/tsai/callback/PredictionDynamics.py` & `tsai-0.3.7/tsai/callback/PredictionDynamics.py`

 * *Files identical despite different names*

### Comparing `tsai-0.3.6/tsai/callback/core.py` & `tsai-0.3.7/tsai/callback/core.py`

 * *Files identical despite different names*

### Comparing `tsai-0.3.6/tsai/callback/experimental.py` & `tsai-0.3.7/tsai/callback/experimental.py`

 * *Files identical despite different names*

### Comparing `tsai-0.3.6/tsai/callback/noisy_student.py` & `tsai-0.3.7/tsai/callback/noisy_student.py`

 * *Files identical despite different names*

### Comparing `tsai-0.3.6/tsai/data/core.py` & `tsai-0.3.7/tsai/data/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -172,14 +172,15 @@
     def setups(self, dset):
         if self.vocab is None and dset is not None:
             dset = np.asarray(dset).flatten()
             self.vocab = CategoryMap(dset, sort=self.sort, add_na=False)
         self.c = len(self.vocab)
         self.vocab_keys = np.array(list(self.vocab.o2i.keys()))[:, None]
 
+    def encodes(self, o:torch.Tensor): return o
     def encodes(self, o):
         try:
             if not hasattr(o, "ndim") or o.ndim <= 1:
                 return TensorCategory((self.vocab_keys == o).argmax(axis=0))
             else:
                 return TensorCategory((self.vocab_keys == o.flatten()).argmax(axis=0).reshape(*o.shape))
         except KeyError as e:
@@ -210,14 +211,15 @@
         if self.vocab is None:
             vals = set()
             for b in dsets: vals = vals.union(set(b))
             self.vocab = CategoryMap(list(vals), add_na=self.add_na)
             if self.c is None: self.c = len(self.vocab)
             if not self.c: warn("Couldn't infer the number of classes, please pass a value for `c` at init")
 
+    def encodes(self, o:torch.Tensor): return o
     def encodes(self, o):
         if not all(elem in self.vocab.o2i.keys() for elem in o):
             diff = [elem for elem in o if elem not in self.vocab.o2i.keys()]
             diff_str = "', '".join(diff)
             raise KeyError(f"Labels '{diff_str}' were not included in the training dataset")
         return TensorMultiCategory(one_hot([self.vocab.o2i[o_] for o_ in o], self.c).float())
     def decodes(self, o): 
@@ -286,31 +288,44 @@
         else:
             y = self._types[1](self.y[idx], device=self.device, dtype=self.dtype)
         return (X, y)
     def __len__(self): return len(self.X) if self.split is None else len(self.split)
 
 # %% ../../nbs/006_data.core.ipynb 40
 def _flatten_list(lst):
+    "Flattens a list of lists with splits"
+
     def __flatten_list(lst):
-        if lst is None: return L([])
-        if not hasattr(lst, "__iter__"): lst = [lst]
-        flattened = []
-        for item in lst:
-            if isinstance(item, (list, tuple, L)):
-                flattened += __flatten_list(item)
-            elif isinstance(item, np.ndarray):
-                flattened += __flatten_list(item.ravel())
-            else:
-                flattened.append(item)
-        output = L(flattened)
-        return output
+        if lst is None: 
+            return L([])
+        if not hasattr(lst, "__iter__"): 
+            lst = [lst]
+
+        # clean_up_list
+        if len(lst) > 10:
+            return lst 
+        else:
+            lst = [l for l in lst if l is not None or (hasattr(l, "__len__") and len(l) == 0)]
+
+        # count lists
+        n_lists = sum([hasattr(l, "__iter__") for l in lst])
+        if n_lists == 0:
+            return lst
+        elif len(lst) == n_lists == 1:
+            return lst[0]
+        else:
+            output = np.concatenate([l if hasattr(l, "__iter__") else [l] for l in lst])
+            if len(output) == 0:
+                return L([])
+            return output.astype(smallest_dtype(int(max(output))))
+
     output = __flatten_list(lst)
     if len(output) == 0: return output
     dtype = smallest_dtype(np.max(output))
-    return np.asarray(output).astype(dtype)
+    return np.asarray(output, dtype=dtype)
 
 def _remove_brackets(l):
     return [li if (not li or not is_listy(li) or len(li) > 1) else li[0] for li in l]
     
 class NoTfmLists(TfmdLists):
     def __init__(self, items, tfms=None, splits=None, split_idx=None, types=None, do_setup=False, **kwargs):
         self.splits = ifnone(splits, L(np.arange(len(items)).tolist(),[]))
@@ -366,21 +381,21 @@
             if tfms is None:
                 self.tfms, lts = [None] * len(items), [NoTfmLists] * len(items)
             else:
                 self.tfms = _remove_brackets(tfms)
                 lts = [NoTfmLists if t is None else TSTfmdLists if getattr(t, 'vectorized', None) else TfmdLists for t in self.tfms]
 
             self.tls = L(lt(item, t, **kwargs) for lt,item,t in zip(lts, items, self.tfms))
-            if len(self.tls) > 0 and len(self.tls[0]) > 0:
-                self.typs = [type(tl[0]) if isinstance(tl[0], torch.Tensor) else self.typs[i] for i,tl in enumerate(self.tls)]
+            # if len(self.tls) > 0 and len(self.tls[0]) > 0:
+            #     self.typs = [type(tl[0]) if isinstance(tl[0], torch.Tensor) else self.typs[i] for i,tl in enumerate(self.tls)]
             self.ptls = L([typ(stack(tl[:])) for i,(tl,typ) in enumerate(zip(self.tls,self.typs))]) if inplace else self.tls
         else:
             self.tls = tls
-            if len(self.tls) > 0 and len(self.tls[0]) > 0:
-                self.typs = [type(tl[0]) if isinstance(tl[0], torch.Tensor) else self.typs[i] for i,tl in enumerate(self.tls)]
+            # if len(self.tls) > 0 and len(self.tls[0]) > 0:
+            #     self.typs = [type(tl[0]) if isinstance(tl[0], torch.Tensor) else self.typs[i] for i,tl in enumerate(self.tls)]
             self.ptls = L([typ(stack(tl[:])) for i,(tl,typ) in enumerate(zip(self.tls,self.typs))]) if inplace and len(tls[0]) != 0 else tls
 
         self.n_inp = 1
         if kwargs.get('splits', None) is not None:
             split_idxs = _flatten_list(kwargs['splits'])
         else: 
             split_idxs = _flatten_list(np.arange(len(self)))
@@ -417,16 +432,16 @@
 def tscoll_repr(c, max_n=10):
     "String repr of up to `max_n` items of (possibly lazy) collection `c`"
     _len = len(c)
     if _len == 0: return coll_repr(c)
     return f'(#{_len}) {L(c[i] for i in range(min(len(c), max_n)))} ...]'
 
 # %% ../../nbs/006_data.core.ipynb 48
-@delegates(NumpyDatasets.__init__)
-class TSDatasets(NumpyDatasets):
+@delegates(Datasets.__init__)
+class TSDatasets(Datasets):
     """A dataset that creates tuples from X (and optionally y) and applies `item_tfms`"""
     typs = TSTensor, torch.as_tensor
     def __init__(self, X=None, y=None, items=None, sel_vars=None, sel_steps=None, tfms=None, tls=None, n_inp=None, dl_type=None, 
                  inplace=True, **kwargs):
 
         # Prepare X (and y)
         if X is not None:
@@ -465,39 +480,38 @@
             items = tuple((X,)) if y is None else tuple((X, y))
             if tfms is None:
                 self.tfms, lts = [None] * len(items), [NoTfmLists] * len(items)
             else:
                 self.tfms = _remove_brackets(tfms)
                 lts = [NoTfmLists if t is None else TSTfmdLists if getattr(t, 'vectorized', None) else TfmdLists for t in self.tfms]
             self.tls = L(lt(item, t, **kwargs) for lt,item,t in zip(lts, items, self.tfms))
-            if len(self.tls) > 0 and len(self.tls[0]) > 0:
-                self.typs = [type(tl.items[0]) if isinstance(tl.items[0], torch.Tensor) else self.typs[i] for i,tl in enumerate(self.tls)]
+            # if len(self.tls) > 0 and len(self.tls[0]) > 0:
+            #     self.typs = [type(tl.items[0]) if isinstance(tl.items[0], torch.Tensor) else self.typs[i] for i,tl in enumerate(self.tls)]
             if self.inplace and (tfms is None or tfms == [None] * len(self.tls)):
                 for tl,typ in zip(self.tls, self.typs):
                     tl.items = typ(tl.items)
                 self.ptls = self.tls
                 self.no_tfm = True
             else:
                 self.ptls = L([typ(stack(tl[:]))[...,self.sel_vars, self.sel_steps] if (i==0 and self.multi_index) else typ(stack(tl[:])) \
                     for i,(tl,typ) in enumerate(zip(self.tls,self.typs))]) if inplace else self.tls
                 self.no_tfm = False
         else:
             self.tls = tls
-            if len(self.tls) > 0 and len(self.tls[0]) > 0:
-                self.typs = [type(tl[0]) if isinstance(tl[0], torch.Tensor) else self.typs[i] for i,tl in enumerate(self.tls)]
+            # if len(self.tls) > 0 and len(self.tls[0]) > 0:
+            #     self.typs = [type(tl[0]) if isinstance(tl[0], torch.Tensor) else self.typs[i] for i,tl in enumerate(self.tls)]
             self.ptls = L([typ(stack(tl[:]))[...,self.sel_vars, self.sel_steps] if (i==0 and self.multi_index) else typ(stack(tl[:])) \
                 for i,(tl,typ) in enumerate(zip(self.tls,self.typs))]) if inplace and len(tls[0]) != 0 else tls
             self.no_tfm = False
             
         self.n_inp = 1
         if kwargs.get('splits', None) is not None:
-            split_idxs = _flatten_list(kwargs['splits'])
+            split_idxs = _flatten_list(kwargs.get('splits'))
         else: 
-            dtype = np.int16 if np.can_cast(len(self.tls[0].items), np.int16) else np.int32 if np.can_cast(len(self.tls[0].items), np.int32) else np.int64
-            split_idxs = _flatten_list(np.arange(len(self), dtype=dtype))
+            split_idxs = np.arange(len(self), dtype=smallest_dtype(len(self)))
         self.split_idxs = split_idxs
 
     def __getitem__(self, it):
         if self.inplace or self.no_tfm:
             return tuple([ptl[it] for ptl in self.ptls])
         else:
             return tuple([typ(stack(ptl[it]))[...,self.sel_vars, self.sel_steps] if (i==0 and self.multi_index) else typ(stack(ptl[it])) \
@@ -520,14 +534,22 @@
     def _new(self, X, y=None, **kwargs):
         return type(self)(X, y=y, sel_vars=self.sel_vars, sel_steps=self.sel_steps, tfms=self.tfms, inplace=self.inplace, 
                           do_setup=False, **kwargs)
     
     def new_empty(self): return type(self)(tls=[tl.new_empty() for tl in self.tls], sel_vars=self.sel_vars, sel_steps=self.sel_steps, 
                                            n_inp=self.n_inp, inplace=self.inplace)
 
+    def __len__(self): return len(self.tls[0])
+    
+    def show_at(self, idx, **kwargs):
+        self.show(self[idx], **kwargs)
+        plt.show()
+        
+    def __repr__(self): return tscoll_repr(self)
+
 # %% ../../nbs/006_data.core.ipynb 51
 def add_ds(dsets, X, y=None, inplace=True):
     "Create test datasets from X (and y) using validation transforms of `dsets`"
     items = tuple((X,)) if y is None else tuple((X, y))
     with_labels = False if y is None else True 
     if isinstance(dsets, TSDatasets):
         tls = dsets.tls if with_labels else dsets.tls[:dsets.n_inp]
@@ -555,24 +577,36 @@
 def add_test(self:NumpyDatasets, X, y=None, inplace=True):
     return add_ds(self, X, y=y, inplace=inplace)
 
 @patch
 def add_unlabeled(self:NumpyDatasets, X, inplace=True):
     return add_ds(self, X, y=None, inplace=inplace)
 
-# %% ../../nbs/006_data.core.ipynb 67
+@patch
+def add_dataset(self:TSDatasets, X, y=None, inplace=True):
+    return add_ds(self, X, y=y, inplace=inplace)
+
+@patch
+def add_test(self:TSDatasets, X, y=None, inplace=True):
+    return add_ds(self, X, y=y, inplace=inplace)
+
+@patch
+def add_unlabeled(self:TSDatasets, X, inplace=True):
+    return add_ds(self, X, y=None, inplace=inplace)
+
+# %% ../../nbs/006_data.core.ipynb 68
 @patch
 def _one_pass(self:TfmdDL):
     b = self.do_batch([self.do_item(0)])
     if self.device is not None: b = to_device(b, self.device)
     its = self.after_batch(b)
     self._n_inp = 1 if not isinstance(its, (list,tuple)) or len(its)==1 else len(its)-1
     self._types = explode_types(its)
 
-# %% ../../nbs/006_data.core.ipynb 68
+# %% ../../nbs/006_data.core.ipynb 69
 _batch_tfms = ('after_item','before_batch','after_batch')
 
 @delegates(TfmdDL.__init__)
 class NumpyDataLoader(TfmdDL):
     idxs = None
     do_item = noops # create batch returns indices
     def __init__(self, dataset, bs=64, shuffle=False, drop_last=False, num_workers=0, verbose=False, do_setup=True, vocab=None,
@@ -584,15 +618,17 @@
         
         for nm in _batch_tfms:
             if nm == 'after_batch' and kwargs.get('batch_tfms',None) is not None: kwargs[nm] = Pipeline(listify(kwargs.get('batch_tfms')))
             else: kwargs[nm] = Pipeline(kwargs.get(nm,None))
         bs = max(1, min(bs, len(dataset))) # bs cannot be 1
         if is_listy(partial_n): partial_n = partial_n[0]
         if isinstance(partial_n, float): partial_n = int(round(partial_n * len(dataset)))
-        if partial_n is not None: bs = min(bs, partial_n)
+        if partial_n is not None: 
+            partial_n = min(partial_n, len(dataset))
+            bs = min(bs, partial_n)
         if weights is not None: weights = weights / weights.sum()
         self.weights, self.partial_n, self.sampler, self.sort, self.do_setup = weights, partial_n, sampler, sort, do_setup
         super().__init__(dataset, bs=bs, shuffle=shuffle, drop_last=drop_last, num_workers=num_workers, verbose=verbose, do_setup=do_setup, **kwargs)
         if vocab is not None:
             self.vocab = vocab
     
     def new_dl(self, X, y=None, bs=64):
@@ -630,23 +666,24 @@
         else: n = self.n
         if self.sampler is not None:
             idxs = np.array(list(iter(self.sampler)))
             if self.partial_n is not None: idxs = idxs[:n]
             return idxs
         if self.weights is not None:
             return random_choice(self.n, n, p=self.weights)
-        idxs = Inf.count if self.indexed else Inf.nones
         if self.n is not None:
-            idxs = np.arange(self.n)
             if self.partial_n is not None:
-                idxs = random_choice(idxs, n, False)
+                return random_choice(self.n, n, False, dtype=smallest_dtype(self.n)) # already shuffled
+            else:
+                idxs = np.arange(self.n, dtype=smallest_dtype(self.n))
+        else:
+            idxs = Inf.count if self.indexed else Inf.nones
         if self.shuffle: idxs = self.shuffle_fn(idxs)
         return idxs
 
-
     def shuffle_fn(self, idxs):
         return np.random.permutation(idxs)
 
     def unique_batch(self, max_n=9):
         old_bs = self.bs
         self.bs = 1
         old_get_idxs = self.get_idxs
@@ -811,15 +848,15 @@
         b = self.one_batch()
         i = getattr(self, 'n_inp', 1 if len(b)==1 else len(b)-1)
         xb = b[:i]
         if hasattr(xb[0], 'len'): return xb[0].len
         if xb[0].ndim >= 4: return xb[0].shape[-2:]
         else: return xb[0].shape[-1]
 
-# %% ../../nbs/006_data.core.ipynb 69
+# %% ../../nbs/006_data.core.ipynb 70
 _batch_tfms = ('after_item','before_batch','after_batch')
 
 class NumpyDataLoaders(DataLoaders):
     _xblock = NumpyTensorBlock
     _dl_type = NumpyDataLoader
     def __init__(self, *loaders, path='.', device=None):
         create_dir(path, verbose=False)
@@ -869,27 +906,27 @@
         defaults = {'shuffle': shuffle_default, 'drop_last': drop_last_default}
         kwargs = merge(defaults, {k: tuplify(v, match=ds) for k,v in kwargs.items()})
         kwargs = [{k: v[i] for k,v in kwargs.items()} for i in range_of(ds)]
         if not is_listy(bs): bs = [bs]
         if len(bs) != len(ds): bs = bs * len(ds)
         if weights is None: weights = [None] * len(ds)
         if not is_listy(partial_n): partial_n = [partial_n]
-        if len(partial_n) != len(ds): partial_n = partial_n * len(ds)
+        if len(partial_n) != len(ds) and len(ds) > 1: partial_n = partial_n + [None] * (len(ds) - len(partial_n))
         if not is_listy(sampler): sampler = [sampler]
         if len(sampler) != len(ds): sampler = sampler * len(ds)
         loaders = [cls._dl_type(d, bs=b, num_workers=num_workers, batch_tfms=batch_tfms, weights=w, partial_n=n, sampler=s, sort=sort, vocab=vocab, **k)\
                    for d,k,b,w,n,s in zip(ds, kwargs, bs, weights, partial_n, sampler)]
         return cls(*loaders, path=path, device=device)
 
 
 class TSDataLoaders(NumpyDataLoaders):
     _xblock = TSTensorBlock
     _dl_type = TSDataLoader
 
-# %% ../../nbs/006_data.core.ipynb 70
+# %% ../../nbs/006_data.core.ipynb 71
 class StratifiedSampler:
     "Sampler where batches preserve the percentage of samples for each class"
     
     def __init__(self, 
         y, # The target variable for supervised learning problems. Stratification is done based on the y labels.
         bs : int = 64, # Batch size
         shuffle : bool = False, # Flag to shuffle each class’s samples before splitting into batches.
@@ -908,24 +945,24 @@
         for _,idx in self.skf.split(self.y, self.y):
             chunklist.extend(idx)
         yield chunklist
 
     def __len__(self):
         return self.n
 
-# %% ../../nbs/006_data.core.ipynb 72
+# %% ../../nbs/006_data.core.ipynb 73
 def get_c(dls):
     if getattr(dls, 'c', False): return dls.c
     if getattr(getattr(dls.train, 'after_item', None), 'c', False): return dls.train.after_item.c
     if getattr(getattr(dls.train, 'after_batch', None), 'c', False): return dls.train.after_batch.c
     vocab = getattr(dls, 'vocab', [])
     if len(vocab) > 0 and is_listy(vocab[-1]): vocab = vocab[-1]
     return len(vocab)
 
-# %% ../../nbs/006_data.core.ipynb 73
+# %% ../../nbs/006_data.core.ipynb 74
 def get_best_dl_params(dl, n_iters=10, num_workers=[0, 1, 2, 4, 8], pin_memory=[True, False], prefetch_factor=[2, 4, 8], return_best=True, 
                        verbose=True): 
 
     if not torch.cuda.is_available(): 
         num_workers = 0
     n_iters = min(n_iters, len(dl))
     if not return_best: verbose = True
@@ -1020,21 +1057,21 @@
     return dl
 
 def get_best_dls_params(dls, n_iters=10, num_workers=[0, 1, 2, 4, 8], pin_memory=[True, False], prefetch_factor=[2, 4, 8], 
                         return_best=True, verbose=True): 
     
     for i in range(len(dls.loaders)):
         try:
-            print(f'\nDataloader {i}\n')
+            pv(f'\nDataloader {i}\n', verbose)
             dls.loaders[i] = get_best_dl_params(dls.loaders[i], n_iters=n_iters, num_workers=num_workers, pin_memory=pin_memory, 
                                             prefetch_factor=prefetch_factor, return_best=return_best, verbose=verbose)
         except KeyboardInterrupt: pass
     return dls
 
-# %% ../../nbs/006_data.core.ipynb 74
+# %% ../../nbs/006_data.core.ipynb 75
 def _check_splits(X, splits):
     if splits is None:
         _dtype = smallest_dtype(len(X))
         if len(X) < 1e6: 
             splits = (L(np.arange(len(X), dtype=_dtype).tolist()), L())
         else: 
             _dtype = smallest_dtype(len(X))
@@ -1063,15 +1100,15 @@
     dls   = TSDataLoaders.from_dsets(*dsets, path=path, bs=bs, batch_tfms=batch_tfms, num_workers=num_workers,
                                      device=device, shuffle_train=shuffle_train, drop_last=drop_last, weights=weights, 
                                      partial_n=partial_n, sampler=sampler, sort=sort, **kwargs)
     return dls
 
 get_tsimage_dls = get_ts_dls
 
-# %% ../../nbs/006_data.core.ipynb 76
+# %% ../../nbs/006_data.core.ipynb 77
 def _check_split(X, split):
     if split is None:
         _dtype = smallest_dtype(len(X))
         if len(X) < 1e6: 
             split = L(np.arange(len(X), dtype=_dtype).tolist())
         else: 
             _dtype = smallest_dtype(len(X))
@@ -1090,15 +1127,15 @@
                                      partial_n=partial_n, sampler=sampler, sort=sort, **kwargs)
     return dls.train
 
 
 
 def get_subset_dl(dl, idxs): return dl.new(dl.dataset.subset(idxs))
 
-# %% ../../nbs/006_data.core.ipynb 115
+# %% ../../nbs/006_data.core.ipynb 116
 def get_time_per_batch(dl, model=None, n_batches=None):
     try:
         timer.start(False)
         pbar = progress_bar(dl, leave=False)
         for i, (xb, _) in enumerate(pbar): 
             if model is not None: 
                 _ = model(xb)
```

### Comparing `tsai-0.3.6/tsai/data/external.py` & `tsai-0.3.7/tsai/data/external.py`

 * *Files 0% similar despite different names*

```diff
@@ -2191,15 +2191,15 @@
     pv(f'Dataset: {dsid}', verbose)
     full_parent_dir = Path(path)/parent_dir
     full_tgt_dir = full_parent_dir/dsid
 #     if not os.path.exists(full_tgt_dir): os.makedirs(full_tgt_dir)
     full_tgt_dir.parent.mkdir(parents=True, exist_ok=True)
     if force_download or not all([os.path.isfile(f'{full_tgt_dir}/{fn}.npy') for fn in ['X_train', 'X_valid', 'y_train', 'y_valid', 'X', 'y']]):
         # Option A
-        src_website = 'http://www.timeseriesclassification.com/Downloads'
+        src_website = 'http://www.timeseriesclassification.com/ClassificationDownloads'
         decompress_from_url(f'{src_website}/{dsid}.zip', target_dir=full_tgt_dir, verbose=verbose)
         if dsid == 'DuckDuckGeese':
             with zipfile.ZipFile(Path(f'{full_parent_dir}/DuckDuckGeese/DuckDuckGeese_ts.zip'), 'r') as zip_ref:
                 zip_ref.extractall(Path(parent_dir))
         if not os.path.exists(full_tgt_dir/f'{dsid}_TRAIN.ts') or not os.path.exists(full_tgt_dir/f'{dsid}_TRAIN.ts') or \
         Path(full_tgt_dir/f'{dsid}_TRAIN.ts').stat().st_size == 0 or Path(full_tgt_dir/f'{dsid}_TEST.ts').stat().st_size == 0: 
             print('It has not been possible to download the required files')
```

### Comparing `tsai-0.3.6/tsai/data/features.py` & `tsai-0.3.7/tsai/data/features.py`

 * *Files identical despite different names*

### Comparing `tsai-0.3.6/tsai/data/image.py` & `tsai-0.3.7/tsai/data/image.py`

 * *Files identical despite different names*

### Comparing `tsai-0.3.6/tsai/data/metadatasets.py` & `tsai-0.3.7/tsai/data/metadatasets.py`

 * *Files identical despite different names*

### Comparing `tsai-0.3.6/tsai/data/mixed.py` & `tsai-0.3.7/tsai/data/mixed.py`

 * *Files identical despite different names*

### Comparing `tsai-0.3.6/tsai/data/mixed_augmentation.py` & `tsai-0.3.7/tsai/data/mixed_augmentation.py`

 * *Files 15% similar despite different names*

```diff
@@ -21,15 +21,17 @@
     "A handler class for implementing mixed sample data augmentation"
     run_valid = False
 
     def __init__(self, alpha=0.5):
         self.distrib = Beta(alpha, alpha)
 
     def before_train(self):
-        self.labeled = self.dls.d
+        if not self.training: return
+        b = self.learn.dls.one_batch()
+        self.labeled = len(b) > 1
         if self.labeled:
             self.stack_y = getattr(self.learn.loss_func, 'y_int', False)
             if self.stack_y: self.old_lf, self.learn.loss_func = self.learn.loss_func, self.lf
 
     def after_train(self):
         if self.labeled and self.stack_y: self.learn.loss_func = self.old_lf
 
@@ -42,14 +44,15 @@
 class MixUp1d(MixHandler1d):
     "Implementation of https://arxiv.org/abs/1710.09412"
 
     def __init__(self, alpha=.4):
         super().__init__(alpha)
 
     def before_batch(self):
+        if not self.training: return
         lam = self.distrib.sample((self.x.size(0), ))
         self.lam = torch.max(lam, 1 - lam).to(self.x.device)
         shuffle = torch.randperm(self.x.size(0))
         xb1 = self.x[shuffle]
         self.learn.xb = L(xb1, self.xb).map_zip(torch.lerp, weight=unsqueeze(self.lam, n=self.x.ndim - 1))
         if self.labeled:
             self.yb1 = tuple((self.y[shuffle], ))
@@ -59,18 +62,20 @@
 
 # %% ../../nbs/011_data.mixed_augmentation.ipynb 9
 class CutMix1d(MixHandler1d):
     "Implementation of `https://arxiv.org/abs/1905.04899`"
 
     def __init__(self, alpha=1.):
         super().__init__(alpha)
-
+            
     def before_batch(self):
+        if not self.training: return
         bs, *_, seq_len = self.x.size()
-        self.lam = self.distrib.sample((1, ))
+        lam = self.distrib.sample((1, ))
+        self.lam = torch.max(lam, 1 - lam).to(self.x.device)
         shuffle = torch.randperm(bs)
         xb1 = self.x[shuffle]
         x1, x2 = self.rand_bbox(seq_len, self.lam)
         self.learn.xb[0][..., x1:x2] = xb1[..., x1:x2]
         self.lam = (1 - (x2 - x1) / float(seq_len)).item()
         if self.labeled:
             self.yb1 = tuple((self.y[shuffle], ))
@@ -78,41 +83,43 @@
                 self.learn.yb = tuple(L(self.yb1, self.yb).map_zip(torch.lerp, weight=unsqueeze(self.lam, n=self.y.ndim - 1)))
 
     def rand_bbox(self, seq_len, lam):
         cut_seq_len = torch.round(seq_len * (1. - lam)).type(torch.long)
         half_cut_seq_len = torch.div(cut_seq_len, 2, rounding_mode='floor')
 
         # uniform
-        cx = torch.randint(0, seq_len, (1, ))
+        cx = torch.randint(0, seq_len, (1, ), device=lam.device)
         x1 = torch.clamp(cx - half_cut_seq_len, 0, seq_len)
         x2 = torch.clamp(cx + half_cut_seq_len, 0, seq_len)
         return x1, x2
 
+
 # %% ../../nbs/011_data.mixed_augmentation.ipynb 10
 class IntraClassCutMix1d(Callback):
     "Implementation of CutMix applied to examples of the same class"
     run_valid = False
 
     def __init__(self, alpha=1.):
         self.distrib = Beta(tensor(alpha), tensor(alpha))
 
     def before_batch(self):
+        if not self.training: return
         bs, *_, seq_len = self.x.size()
         idxs = torch.arange(bs, device=self.x.device)
         y = torch.tensor(self.y)
         unique_c = torch.unique(y).tolist()
         idxs_by_class = torch.cat([idxs[torch.eq(y, c)] for c in unique_c])
         idxs_shuffled_by_class = torch.cat([random_shuffle(idxs[torch.eq(y, c)]) for c in unique_c])
-        self.lam = self.distrib.sample((1, ))
+        self.lam = self.distrib.sample((1, )).to(self.x.device)
         x1, x2 = self.rand_bbox(seq_len, self.lam)
         xb1 = self.x[idxs_shuffled_by_class]
         self.learn.xb[0][idxs_by_class, :, x1:x2] = xb1[..., x1:x2]
 
     def rand_bbox(self, seq_len, lam):
         cut_seq_len = torch.round(seq_len * (1. - lam)).type(torch.long)
         half_cut_seq_len = torch.div(cut_seq_len, 2, rounding_mode='floor')
 
         # uniform
-        cx = torch.randint(0, seq_len, (1, ))
+        cx = torch.randint(0, seq_len, (1, ), device=lam.device)
         x1 = torch.clamp(cx - half_cut_seq_len, 0, seq_len)
         x2 = torch.clamp(cx + half_cut_seq_len, 0, seq_len)
         return x1, x2
```

### Comparing `tsai-0.3.6/tsai/data/preparation.py` & `tsai-0.3.7/tsai/data/preparation.py`

 * *Files 2% similar despite different names*

```diff
@@ -867,49 +867,50 @@
     freq="D",  # datetime units. May contain a letters only or a combination of ints + letters: eg. "7D"
     datetime_format="%Y-%m-%d",  # format used to convert "today"
     datetime_col=None,  # str data column containing the datetime
     use_index=False,  # bool flag to indicate if index should be used to get column
 ):
     "Returns the start and end datetimes used by the forecast"
     min_datetime, max_datetime = get_df_datetime_bounds(df, datetime_col=datetime_col, use_index=use_index)
-    min_datetime, max_datetime = pd.Timestamp(min_datetime, freq=freq), pd.Timestamp(max_datetime, freq=freq)
+    min_datetime, max_datetime = pd.Timestamp(min_datetime).floor(freq), pd.Timestamp(max_datetime).floor(freq)
     fcst_datetime_min, fcst_datetime_max = split_fcst_datetime(fcst_datetime)
     if fcst_datetime_min is None and fcst_datetime_max is None:
         start_datetime, end_datetime = min_datetime, max_datetime
     else:
-        
         if fcst_datetime_min == "today":
             fcst_datetime_min = get_today(fcst_datetime_min, datetime_format=datetime_format)
         if fcst_datetime_max == "today":
             fcst_datetime_max = get_today(fcst_datetime_max, datetime_format=datetime_format)
         
         # end_datetime
         if fcst_datetime_max is None:
             fcst_dt = end_datetime = max_datetime
         else:
-            fcst_dt = end_datetime = pd.Timestamp(fcst_datetime_max, freq=freq)
+            fcst_dt = end_datetime = pd.Timestamp(fcst_datetime_max).floor(freq)
             if fcst_horizon:
-                end_datetime = end_datetime + end_datetime.freq * fcst_horizon
+                end_datetime = pd.date_range(end_datetime, periods=fcst_horizon + 1, freq=freq).floor(freq)[-1]
 
         # start_datetime
         if fcst_datetime_min is None:
             start_datetime = min_datetime
         elif fcst_datetime_min == fcst_datetime_max:
             start_datetime = fcst_dt
             if fcst_history:
-                start_datetime -= start_datetime.freq * (fcst_history - 1)
+                start_datetime = pd.date_range(end=start_datetime, periods=fcst_history, freq=freq).floor(freq)[0]
         else:
-            n_periods = int((fcst_dt - pd.Timestamp(fcst_datetime_min)) / fcst_dt.freq)
+            # n_periods = int((fcst_dt - pd.Timestamp(fcst_datetime_min)) / fcst_dt.freq)
+            n_periods = len(pd.date_range(start=fcst_datetime_min, end=fcst_dt, freq=freq))
             if fcst_history:
                 n_periods += fcst_history - 1
-            start_datetime = fcst_dt - n_periods * fcst_dt.freq
+            # start_datetime = fcst_dt - n_periods * fcst_dt.freq
+            start_datetime = pd.date_range(end=fcst_dt, periods=n_periods, freq=freq).floor(freq)[0]
     
     return start_datetime, end_datetime
 
-# %% ../../nbs/004_data.preparation.ipynb 120
+# %% ../../nbs/004_data.preparation.ipynb 121
 def filter_df_by_datetime(
     df,  # dataframe containing forecasting data
     start_datetime=None, # lower datetime bound
     end_datetime=None, # upper datetime bound
     datetime_col=None,  # str data column containing the datetime
     use_index=False,  # bool flag to indicate if index should be used to get column
 ):
@@ -934,15 +935,15 @@
             mask = df[datetime_col] <= end_datetime
     if (start_datetime is not None or end_datetime is not None) and mask.mean() != 1:
         df = df.loc[mask]
         if not use_index:
             df.reset_index(drop=True, inplace=True)
     return df
 
-# %% ../../nbs/004_data.preparation.ipynb 122
+# %% ../../nbs/004_data.preparation.ipynb 123
 def get_fcst_data_from_df(
     df,  # dataframe containing forecasting data
     fcst_datetime,  # datetime for which a fcst is created. Optionally tuple of datatimes if the fcst is created for a range of dates.
     fcst_history=None,  # # steps used as input
     fcst_horizon=None,  # # predicted steps
     freq="D",  # datetime units. May contain a letters only or a combination of ints + letters: eg. "7D"
     datetime_format="%Y-%m-%d",  # format used to convert "today"
```

### Comparing `tsai-0.3.6/tsai/data/preprocessing.py` & `tsai-0.3.7/tsai/data/preprocessing.py`

 * *Files 18% similar despite different names*

```diff
@@ -19,17 +19,19 @@
 # %% auto 0
 __all__ = ['Nan2Value', 'TSRandomStandardize', 'default_date_attr', 'PD_TIME_UNITS', 'StandardScaler', 'RobustScaler',
            'Normalizer', 'BoxCox', 'YeoJohnshon', 'Quantile', 'ToNumpyCategory', 'OneHot', 'TSNan2Value',
            'TSStandardize', 'TSNormalize', 'TSStandardizeTuple', 'TSCatEncode', 'TSDropFeatByKey', 'TSClipOutliers',
            'TSClip', 'TSSelfMissingness', 'TSRobustScale', 'get_stats_with_uncertainty', 'get_random_stats',
            'TSGaussianStandardize', 'TSDiff', 'TSLog', 'TSCyclicalPosition', 'TSLinearPosition', 'TSMissingness',
            'TSPositionGaps', 'TSRollingMean', 'TSLogReturn', 'TSAdd', 'TSClipByVar', 'TSDropVars', 'TSOneHotEncode',
-           'TSPosition', 'TSShrinkDataFrame', 'TSOneHotEncoder', 'TSCategoricalEncoder', 'TSDateTimeEncoder',
-           'TSMissingnessEncoder', 'TSSortByColumns', 'TSSelectColumns', 'TSStepsSinceStart', 'TSStandardScaler',
-           'TSAddMissingTimestamps', 'TSDropDuplicates', 'TSFillMissing', 'Preprocessor', 'ReLabeler']
+           'TSPosition', 'PatchEncoder', 'TSPatchEncoder', 'TSTuplePatchEncoder', 'TSShrinkDataFrame', 'object2date',
+           'TSOneHotEncoder', 'TSCategoricalEncoder', 'TSTargetEncoder', 'TSDateTimeEncoder', 'TSDropIfTrueCols',
+           'TSApplyFunction', 'TSMissingnessEncoder', 'TSSortByColumns', 'TSSelectColumns', 'TSStepsSinceStart',
+           'TSStandardScaler', 'TSRobustScaler', 'TSAddMissingTimestamps', 'TSDropDuplicates', 'TSFillMissing',
+           'Preprocessor', 'ReLabeler']
 
 # %% ../../nbs/009_data.preprocessing.ipynb 6
 class ToNumpyCategory(Transform):
     "Categorize a numpy batch"
     order = 90
 
     def __init__(self, **kwargs):
@@ -856,15 +858,167 @@
         super().__init__(**kwargs)
 
     def encodes(self, o: TSTensor):
         bs = o.shape[0]
         steps = self.steps.expand(bs, -1, -1).to(device=o.device, dtype=o.dtype)
         return torch.cat([o, steps], 1)
 
-# %% ../../nbs/009_data.preprocessing.ipynb 80
+# %% ../../nbs/009_data.preprocessing.ipynb 79
+import torch
+import torch.nn.functional as F
+
+class PatchEncoder():
+    "Creates a sequence of patches from a 3d input tensor."
+
+    def __init__(self, 
+        patch_len:int, # Number of time steps in each patch.
+        patch_stride:int=None, # Stride of the patch.
+        pad_at_start:bool=True, # If True, pad the input tensor at the start to ensure that the input tensor is evenly divisible by the patch length.
+        value:float=0.0, # Value to pad the input tensor with.
+        seq_len:int=None, # Number of time steps in the input tensor. If None, make sure seq_len >= patch_len and a multiple of stride
+        merge_dims:bool=True, # If True, merge channels within the same patch.
+        reduction:str='none', # type of reduction applied. Available: "none", "mean", "min", "max", "mode"
+        reduction_dim:int=-1, # dimension where the reduction is applied
+        swap_dims:tuple=None, # If True, swap the time and channel dimensions.
+        ):
+        super().__init__()
+
+        self.seq_len = seq_len
+        self.patch_len = patch_len
+        self.patch_stride = patch_stride or patch_len
+        self.pad_at_start = pad_at_start
+        self.value = value
+        self.merge_dims = merge_dims
+
+        assert reduction in ["none", "mean", "min", "max", "mode"]
+        self.reduction = reduction
+        self.reduction_dim = reduction_dim
+        self.swap_dims = swap_dims
+        
+        if seq_len is None:
+            self.pad_size = 0
+        elif self.seq_len < self.patch_len:
+            self.pad_size = self.patch_len - self.seq_len
+        else:
+            if (self.seq_len % self.patch_len) % self.patch_stride == 0:
+                self.pad_size = 0
+            else:
+                self.pad_size = self.patch_stride - (self.seq_len % self.patch_len) % self.patch_stride
+
+    def __call__(self, 
+        x: torch.Tensor # 3d input tensor with shape [batch size, sequence length, channels]
+        ) -> torch.Tensor: #  Transformed tensor of patches with shape [batch size, channels*patch length, number of patches]
+
+        if x.ndim == 2:
+            x = x[:, None]
+            
+        bs, c_in, *_ = x.size()
+        if not bs: 
+            return x
+        
+        if self.pad_size:
+            x = F.pad(x, (self.pad_size, 0), value=self.value) if self.pad_at_start else F.pad(x, (0, self.pad_size), value=self.value)
+        
+        x = x.unfold(2, self.patch_len, self.patch_stride)
+        x = x.permute(0, 1, 3, 2)
+        if self.merge_dims:
+            x = x.reshape(bs, c_in * self.patch_len, -1)
+
+        if self.reduction == "mean":
+            x = x.mean(self.reduction_dim)
+        elif self.reduction == "min":
+            x = x.min(self.reduction_dim).values
+        elif self.reduction == "max":
+            x = x.max(self.reduction_dim).values
+        elif self.reduction == "mode":
+            x = x.mode(self.reduction_dim).values
+
+        if self.swap_dims:
+            x = x.swapaxes(*self.swap_dims)
+
+        return x
+
+# %% ../../nbs/009_data.preprocessing.ipynb 81
+class TSPatchEncoder(Transform):
+    "Tansforms a time series into a sequence of patches along the last dimension"
+    order = 90
+    
+    def __init__(self, 
+        patch_len:int, # Number of time steps in each patch.
+        patch_stride:int=None, # Stride of the patch.
+        pad_at_start:bool=True, # If True, pad the input tensor at the start to ensure that the input tensor is evenly divisible by the patch length.
+        value:float=0.0, # Value to pad the input tensor with.
+        seq_len:int=None, # Number of time steps in the input tensor. If None, make sure seq_len >= patch_len and a multiple of stride
+        merge_dims:bool=True, # If True, merge channels within the same patch.
+        reduction:str='none', # type of reduction applied. Available: "none", "mean", "min", "max", "mode"
+        reduction_dim:int=-2, # dimension where the y reduction is applied.
+        swap_dims:tuple=None, # If True, swap the time and channel dimensions.
+        ):
+        super().__init__()
+
+        self.patch_encoder = PatchEncoder(patch_len=patch_len, 
+                                          patch_stride=patch_stride, 
+                                          pad_at_start=pad_at_start, 
+                                          value=value,
+                                          seq_len=seq_len, 
+                                          merge_dims=merge_dims,
+                                          reduction=reduction,
+                                          reduction_dim=reduction_dim,
+                                          swap_dims=swap_dims)
+
+    def encodes(self, o:TSTensor):
+        return self.patch_encoder(o)
+
+# %% ../../nbs/009_data.preprocessing.ipynb 83
+from fastcore.transform import ItemTransform
+
+class TSTuplePatchEncoder(ItemTransform):
+    "Tansforms a time series with x and y into sequences of patches along the last dimension"
+    order = 90
+    
+    def __init__(self, 
+        patch_len:int, # Number of time steps in each patch.
+        patch_stride:int=None, # Stride of the patch.
+        pad_at_start:bool=True, # If True, pad the input tensor at the start to ensure that the input tensor is evenly divisible by the patch length.
+        value:float=0.0, # Value to pad the input tensor with.
+        seq_len:int=None, # Number of time steps in the input tensor. If None, make sure seq_len >= patch_len and a multiple of stride
+        merge_dims:bool=True, # If True, merge y channels within the same patch.
+        reduction:str='none', # type of reduction applied to y. Available: "none", "mean", "min", "max", "mode"
+        reduction_dim:int=-2, # dimension where the y reduction is applied.
+        swap_dims:tuple=None, # If True, swap the time and channel dimensions in y.
+        ):
+        super().__init__()
+
+        self.x_patch_encoder = PatchEncoder(patch_len=patch_len, 
+                                            patch_stride=patch_stride, 
+                                            pad_at_start=pad_at_start, 
+                                            value=value,
+                                            seq_len=seq_len)
+
+        self.y_patch_encoder = PatchEncoder(patch_len=patch_len, 
+                                            patch_stride=patch_stride, 
+                                            pad_at_start=pad_at_start, 
+                                            value=value,
+                                            seq_len=seq_len, 
+                                            merge_dims=merge_dims,
+                                            reduction=reduction,
+                                            reduction_dim=reduction_dim,
+                                            swap_dims=swap_dims)
+
+    def encodes(self, xy):
+        if len(xy) == 2:
+            x, y = xy
+            x, y = self.x_patch_encoder(x), self.y_patch_encoder(y)
+            return (x, y)
+        elif len(xy) == 1:
+            x = xy[0]
+            x = self.x_patch_encoder(x)
+            return (x, )
+
+# %% ../../nbs/009_data.preprocessing.ipynb 86
 class TSShrinkDataFrame(BaseEstimator, TransformerMixin):
     """A transformer to shrink dataframe or series memory usage"""
 
     def __init__(self, 
         columns=None, # List[str], optional. Columns to shrink, all columns by default.
         skip=None, # List[str], optional. Columns to skip, None by default.
         obj2cat=True, # bool, optional. Convert object columns to category, True by default.
@@ -873,14 +1027,18 @@
         ):
         self.columns, self.skip, self.obj2cat, self.int2uint, self.verbose = listify(columns), listify(skip), obj2cat, int2uint, verbose
         
     def fit(self, X, y=None, **fit_params):
         if isinstance(X, pd.Series): 
             X = X.to_frame()
         assert isinstance(X, pd.DataFrame), "X must be a pd.DataFrame or pd.Series" 
+        if isinstance(X, pd.Series):
+            X = X.to_frame().apply(object2date)
+        else:
+            X = X.apply(object2date)
         if self.columns:
             self.dt = df_shrink_dtypes(X[self.columns], self.skip, obj2cat=self.obj2cat, int2uint=self.int2uint)
         else:
             self.dt = df_shrink_dtypes(X, self.skip, obj2cat=self.obj2cat, int2uint=self.int2uint)
         return self
         
     def transform(self, X, **kwargs):
@@ -889,29 +1047,41 @@
             X = X.to_frame()
         else:
             col_name = None
         assert isinstance(X, pd.DataFrame), "X must be a pd.DataFrame or pd.Series"
         if self.verbose:
             start_memory = X.memory_usage().sum()
             print(f"Initial memory usage: {bytes2str(start_memory):10}")
+        if isinstance(X, pd.Series):
+            X = X.to_frame().apply(object2date)
+        else:
+            X = X.apply(object2date)
         if self.columns:
             X.loc[:, self.columns] = X[self.columns].astype(self.dt)
         else:
             X = X.astype(self.dt)
         if self.verbose:
             end_memory = X.memory_usage().sum()
             print(f"Final memory usage  : {bytes2str(end_memory):10} ({(end_memory - start_memory) / start_memory:.1%})")
         if col_name is not None:
             X = X[col_name]
         return X
          
     def inverse_transform(self, X, **kwargs):
         return X
 
-# %% ../../nbs/009_data.preprocessing.ipynb 82
+
+def object2date(x, format=None):
+    if not x.dtype == np.dtype('object'): return x
+    try:
+        return pd.to_datetime(x, format=format)
+    except:
+        return x
+
+# %% ../../nbs/009_data.preprocessing.ipynb 90
 class TSOneHotEncoder(BaseEstimator, TransformerMixin):
     "Encode categorical variables using one-hot encoding"
 
     def __init__(
         self,
         columns=None,  # (str or List[str], optional): Column name(s) to encode. If None, all columns will be encoded. Defaults to None.
         drop=True,  # (bool, optional): Whether to drop the original columns after encoding. Defaults to True.
@@ -957,15 +1127,15 @@
             X[col] = output[:, i]
             if hasattr(d, "categories"):
                 X[col] = X[col].astype('category')
         if self.drop:
             X = X.drop(self.new_cols, axis=1)
         return X
 
-# %% ../../nbs/009_data.preprocessing.ipynb 84
+# %% ../../nbs/009_data.preprocessing.ipynb 92
 class TSCategoricalEncoder(BaseEstimator, TransformerMixin):
     """A transformer to encode categorical columns"""
 
     def __init__(self,
         columns=None, # List[str], optional. Columns to encode, all columns by default.
         add_na=True, # bool, optional. Add a NaN category, True by default.
         sort=True, # bool, optional. Sort categories by frequency, True by default.
@@ -1048,39 +1218,98 @@
                     continue
                 name = []
                 if self.prefix: name += [self.prefix]
                 name += [column]
                 if self.suffix: name += [self.suffix]
                 new_col = '_'.join(name)
                 if self.add_na:
-                    X.loc[:, new_col] = np.array(['#na#'] + list(categories.categories))[X.loc[:, new_col]]
+                    X.loc[:, new_col] = np.array(['#na#'] + list(categories.categories))[X.loc[:, new_col].astype(int)]
                 else:
-                    X.loc[:, new_col] = categories.categories[X.loc[:, new_col]]
+                    X.loc[:, new_col] = categories.categories[X.loc[:, new_col].astype(int)]
         else:
             if self.add_na:
                 X = pd.Series(np.array(['#na#'] + list(self.categories[0].categories))[X], name=X.name, index=X.index)
             else:
                 X = pd.Series(self.categories[0].categories[X], name=X.name, index=X.index)
         return X
 
     def to_categorical(self, categories):
         if is_listy(categories[0]):
             return [pd.CategoricalDtype(categories=np.sort(c) if self.sort else c, ordered=True) for c in categories]
         else:
             return pd.CategoricalDtype(categories=np.sort(categories) if self.sort else categories, ordered=True)
 
-# %% ../../nbs/009_data.preprocessing.ipynb 90
+# %% ../../nbs/009_data.preprocessing.ipynb 98
+class TSTargetEncoder(TransformerMixin, BaseEstimator):
+    def __init__(self, 
+        target_column, # column containing the target 
+        columns=None, # List[str], optional. Columns to encode, all non-numerical columns by default.
+        inplace=True, # bool, optional. Modify input DataFrame, True by default.
+        prefix=None, # str, optional. Prefix for created column names. None by default.
+        suffix=None, # str, optional. Suffix for created column names. None by default.
+        drop=True, # bool, optional. Drop original columns, False by default.
+        dtypes=["object", "category"], # List[str]. List with dtypes that will be used to identify columns to encode if not explicitly passed.
+        ):
+        "Transforms categorical columns into numerical by replacing categories with target means."
+        
+        self.columns = listify(columns)
+        self.target_column = target_column
+        self.target_means = {}
+        self.inplace = inplace
+        self.prefix = prefix
+        self.suffix = suffix
+        self.drop = drop
+        self.dtypes = listify(dtypes)
+
+    def fit(self, X, y=None, **fit_params):
+        assert isinstance(X, pd.DataFrame)
+        if not self.columns:
+            self.columns = X.select_dtypes(include=self.dtypes).columns
+                
+        assert self.target_column in X.columns
+        idxs = fit_params.get("idxs", slice(None))
+        X_fit = X.loc[idxs]
+
+        for column in self.columns:
+            assert column in X.columns
+            self.target_means[column] = X_fit.groupby(column)[self.target_column].mean()
+
+        return self
+
+    def transform(self, X, **kwargs):
+        assert isinstance(X, pd.DataFrame)
+        if not self.inplace:
+            X = X.copy()
+        for column in self.columns:
+            if column not in X.columns:
+                continue
+            name = []
+            if self.prefix: name += [self.prefix]
+            name += [column]
+            if self.suffix: name += [self.suffix]
+            new_col = '_'.join(name)
+            if self.drop:
+                X.loc[:, column] = X.loc[:, column].map(self.target_means[column])
+                X.rename(columns={column: new_col}, inplace=True)
+            else:
+                X.loc[:, new_col] = X.loc[:, column].map(self.target_means[column])
+        return X
+
+    def inverse_transform(self, X, **kwargs):
+        raise NotImplementedError("This method cannot be implemented because the original data cannot be reconstructed exactly.")
+
+# %% ../../nbs/009_data.preprocessing.ipynb 100
 default_date_attr = ['Year', 'Month', 'Week', 'Day', 'Dayofweek', 'Dayofyear', 'Is_month_end', 'Is_month_start', 
                      'Is_quarter_end', 'Is_quarter_start', 'Is_year_end', 'Is_year_start']
 
 class TSDateTimeEncoder(BaseEstimator, TransformerMixin):
 
     def __init__(self, datetime_columns=None, prefix=None, drop=True, time=False, attr=default_date_attr):
         self.datetime_columns = listify(datetime_columns)
-        self.prefix, self.drop, self.time, self.attr = prefix, drop, time ,attr
+        self.prefix, self.drop, self.time, self.attr = prefix, drop, time, listify(attr)
         
     def fit(self, X, y=None, **fit_params):
         assert isinstance(X, pd.DataFrame)
         if self.time: self.attr = self.attr + ['Hour', 'Minute', 'Second']
         if not self.datetime_columns:
             self.datetime_columns = X.columns
         self.prefixes = []
@@ -1097,15 +1326,73 @@
 
             # Pandas removed `dt.week` in v1.1.10
             week = field.dt.isocalendar().week.astype(field.dt.day.dtype) if hasattr(field.dt, 'isocalendar') else field.dt.week
             for n in self.attr: X[prefix + "_" + n] = getattr(field.dt, n.lower()) if n != 'Week' else week
             if self.drop: X = X.drop(self.datetime_columns, axis=1)
         return X
 
-# %% ../../nbs/009_data.preprocessing.ipynb 93
+# %% ../../nbs/009_data.preprocessing.ipynb 103
+class TSDropIfTrueCols(BaseEstimator, TransformerMixin):
+
+    def __init__(self, columns=None):
+        self.columns = listify(columns)
+
+    def fit(self, X, y=None, **fit_params):
+        assert isinstance(X, pd.DataFrame)
+        if not self.columns: self.columns = X.columns
+        return self
+
+    def transform(self, X, **kwargs):
+        assert isinstance(X, pd.DataFrame)
+        mask = X[self.columns].sum(axis=1) == 0
+        X = X[mask].reset_index(drop=True)
+        X.drop(columns=self.columns, inplace=True)
+        return X
+
+    def inverse_transform(self, X, **kwargs):
+        raise NotImplementedError("Inverse transform is not implemented for TSDropIfTrueCols")
+
+# %% ../../nbs/009_data.preprocessing.ipynb 105
+class TSApplyFunction(BaseEstimator, TransformerMixin):
+
+    def __init__(self, function, groups=None, group_keys=False, axis=1, columns=None, reset_index=False, drop=True):
+        self.function = function
+        self.groups = listify(groups)
+        self.group_keys = group_keys
+        self.columns = listify(columns)
+        self.reset_index = reset_index
+        self.drop = drop
+        self.axis = axis
+
+    def fit(self, X, y=None, **fit_params):
+        assert isinstance(X, pd.DataFrame)
+        if self.columns is None:
+            self.columns = X.columns
+        return self
+
+    def transform(self, X, **kwargs):
+        assert isinstance(X, pd.DataFrame)
+        if self.groups:
+            if self.columns:
+                X = X.groupby(self.groups, group_keys=self.group_keys)[self.columns].apply(lambda x: self.function(x))
+            else:
+                X = X.groupby(self.groups, group_keys=self.group_keys).apply(lambda x: self.function(x))
+        else:
+            if self.columns:
+                X[self.columns] = X[self.columns].apply(lambda x: self.function(x), axis=self.axis)
+            else:
+                X = X.apply(lambda x: self.function(x), axis=self.axis)
+        if self.reset_index: 
+            X = X.reset_index(drop=self.drop)
+        return X
+
+    def inverse_transform(self, X, **kwargs):
+        raise NotImplementedError("Inverse transform is not implemented for ApplyFunction")
+
+# %% ../../nbs/009_data.preprocessing.ipynb 109
 class TSMissingnessEncoder(BaseEstimator, TransformerMixin):
 
     def __init__(self, columns=None):
         self.columns = listify(columns)
         
     def fit(self, X, y=None, **fit_params):
         assert isinstance(X, pd.DataFrame)
@@ -1119,15 +1406,15 @@
         return X
          
     def inverse_transform(self, X, **kwargs):
         assert isinstance(X, pd.DataFrame)
         X.drop(self.missing_columns, axis=1, inplace=True)
         return X
 
-# %% ../../nbs/009_data.preprocessing.ipynb 95
+# %% ../../nbs/009_data.preprocessing.ipynb 111
 class TSSortByColumns(TransformerMixin, BaseEstimator):
     "Transforms a dataframe by sorting by columns."
 
     def __init__(self, 
         columns, # Columns to sort by
         ascending=True, # Ascending or descending
         inplace=True, # Perform operation in place
@@ -1152,37 +1439,37 @@
             X = X.sort_values(self.columns, axis=0, ascending=self.ascending, inplace=False, kind=self.kind, 
                               na_position=self.na_position, ignore_index=self.ignore_index, key=self.key)
         return X
 
     def inverse_transform(self, X, **kwargs):
         return X
 
-# %% ../../nbs/009_data.preprocessing.ipynb 97
+# %% ../../nbs/009_data.preprocessing.ipynb 113
 class TSSelectColumns(TransformerMixin, BaseEstimator):
-    "Transform used to selec columns"
+    "Transform used to select columns"
 
     def __init__(self, 
         columns # str or List[str]. Selected columns.
         ):
         self.columns = listify(columns)
     
     def fit(self, X, y=None, **fit_params):
         assert isinstance(X, (pd.DataFrame, pd.Series))
         return self
         
     def transform(self, X, idxs=None, **kwargs):
         assert isinstance(X, (pd.DataFrame, pd.Series))
         if idxs is not None:
             return X.loc[idxs, self.columns]
-        return X[self.columns]
+        return X[self.columns].copy()
 
     def inverse_transform(self, X, **kwargs):
         return X
 
-# %% ../../nbs/009_data.preprocessing.ipynb 99
+# %% ../../nbs/009_data.preprocessing.ipynb 115
 PD_TIME_UNITS = dict([
     ("Y", "year"), 
     ("M", "month"), 
     ("W", "week"), 
     ("D", "day"), 
     ("h", "hour"), 
     ("m", "minute"), 
@@ -1243,15 +1530,15 @@
         if self.drop: 
             X[self.new_col] = datetimes
             X.rename(columns={self.new_col:self.datetime_col}, inplace=True)
         else:
             X[self.datetime_col] = datetimes
         return X
 
-# %% ../../nbs/009_data.preprocessing.ipynb 101
+# %% ../../nbs/009_data.preprocessing.ipynb 117
 class TSStandardScaler(TransformerMixin, BaseEstimator):
     "Scale the values of specified columns in the input DataFrame to have a mean of 0 and standard deviation of 1."
 
     def __init__(self,
         columns=None, # Column name(s) to be transformed. If None, all columns are transformed. Defaults to None.
         mean=None, # Mean value for each column. If None, the mean value of each column is calculated during the fit method. Defaults to None.
         std=None, # Stdev value for each column. If None, the standard deviation value of each column is calculated during the fit method. Defaults to None.
@@ -1292,15 +1579,57 @@
 
     def inverse_transform(self, X, **kwargs):
         assert isinstance(X, (pd.DataFrame, pd.Series))
         for c, m, s in zip(self.columns, self.mean, self.std):
             X[c] = X[c] * (s + self.eps)  + m
         return X
 
-# %% ../../nbs/009_data.preprocessing.ipynb 104
+# %% ../../nbs/009_data.preprocessing.ipynb 120
+class TSRobustScaler(TransformerMixin, BaseEstimator):
+    """This Scaler removes the median and scales the data according to the quantile range (defaults to IQR: Interquartile Range)"""
+
+    def __init__(self, columns=None, quantile_range=(25.0, 75.0), eps=1e-6):
+        self.columns = listify(columns)
+        self.quantile_range = quantile_range
+        self.eps = np.array(eps, dtype='float32')
+
+    def fit(self, X, y=None, **fit_params):
+        assert isinstance(X, (pd.DataFrame, pd.Series))
+        if not self.columns:
+            if isinstance(X, pd.DataFrame):
+                self.columns = X.columns
+            else:
+                self.columns = X.name
+        idxs = fit_params.get("idxs", slice(None))
+        
+        self.median = []
+        for c in self.columns:
+            self.median.append(np.nanpercentile(X.loc[idxs, c], 50))
+
+        self.iqr = []
+        for c in self.columns:
+            q1 = np.nanpercentile(X.loc[idxs, c], self.quantile_range[0])
+            q3 = np.nanpercentile(X.loc[idxs, c], self.quantile_range[1])
+            self.iqr.append(q3 - q1)
+                
+        return self
+
+    def transform(self, X, **kwargs):
+        assert isinstance(X, (pd.DataFrame, pd.Series))
+        for c, m, q in zip(self.columns, self.median, self.iqr):
+            X[c] = (X[c] - m) / (q + self.eps)
+        return X
+
+    def inverse_transform(self, X, **kwargs):
+        assert isinstance(X, (pd.DataFrame, pd.Series))
+        for c, m, q in zip(self.columns, self.median, self.iqr):
+            X[c] = X[c] * (q + self.eps) + m
+        return X
+
+# %% ../../nbs/009_data.preprocessing.ipynb 122
 class TSAddMissingTimestamps(TransformerMixin, BaseEstimator):
     def __init__(self, datetime_col=None, use_index=False, unique_id_cols=None, fill_value=np.nan, range_by_group=True, 
                  start_date=None, end_date=None, freq=None):
         assert datetime_col is not None or use_index
         store_attr()
         self.func = partial(add_missing_timestamps, datetime_col=datetime_col, use_index=use_index, unique_id_cols=unique_id_cols, 
                             fill_value=fill_value, range_by_group=range_by_group, start_date=start_date, end_date=end_date, 
@@ -1314,15 +1643,15 @@
         assert isinstance(X, (pd.DataFrame, pd.Series))
         X = self.func(X)
         return X
 
     def inverse_transform(self, X, **kwargs):
         return X
 
-# %% ../../nbs/009_data.preprocessing.ipynb 108
+# %% ../../nbs/009_data.preprocessing.ipynb 126
 class TSDropDuplicates(TransformerMixin, BaseEstimator):
     "Drop rows with duplicated values in a set of columns, optionally including a datetime column or index"
 
     def __init__(self,
         datetime_col=None, #(str or List[str], optional): Name(s) of column(s) containing datetime values. If None, the index is used if use_index=True.
         use_index=False, #(bool, optional): Whether to include the index in the set of columns for checking duplicates. Defaults to False.
         unique_id_cols=None, #(str or List[str], optional): Name(s) of column(s) to be included in the set of columns for checking duplicates. Defaults to None.
@@ -1351,15 +1680,15 @@
             if not self.use_index and self.reset_index:
                 X.reset_index(drop=True, inplace=True)
         return X
 
     def inverse_transform(self, X, **kwargs):
         return X
 
-# %% ../../nbs/009_data.preprocessing.ipynb 110
+# %% ../../nbs/009_data.preprocessing.ipynb 128
 class TSFillMissing(TransformerMixin, BaseEstimator):
     "Fill missing values in specified columns using the specified method and/ or value."
 
     def __init__(self,
         columns=None, #(str or List[str], optional): Column name(s) to be transformed. If None, all columns are transformed. Defaults to None.
         unique_id_cols=None, #(str or List[str], optional): Col name(s) with unique ids for each row. If None, uses all rows at once. Defaults to None .
         method='ffill', #(str, optional): The method to use for filling missing values, e.g. 'ffill', 'bfill'. If None, `value` is used. Defaults to None.
@@ -1392,15 +1721,15 @@
             for c in self.columns:
                 X[c] = X[c].fillna(value=self.value)
         return X
 
     def inverse_transform(self, X, **kwargs):
         return X
 
-# %% ../../nbs/009_data.preprocessing.ipynb 112
+# %% ../../nbs/009_data.preprocessing.ipynb 130
 class TSMissingnessEncoder(BaseEstimator, TransformerMixin):
 
     def __init__(self, columns=None):
         self.columns = listify(columns)
 
     def fit(self, X, y=None, **fit_params):
         assert isinstance(X, pd.DataFrame)
@@ -1412,15 +1741,15 @@
         assert isinstance(X, pd.DataFrame)
         X[self.missing_columns] = X[self.columns].isnull().astype(np.int16)
         return X
 
     def inverse_transform(self, X):
         return X
 
-# %% ../../nbs/009_data.preprocessing.ipynb 116
+# %% ../../nbs/009_data.preprocessing.ipynb 134
 class Preprocessor():
     def __init__(self, preprocessor, **kwargs): 
         self.preprocessor = preprocessor(**kwargs)
         
     def fit(self, o): 
         if isinstance(o, pd.Series): o = o.values.reshape(-1,1)
         else: o = o.reshape(-1,1)
@@ -1454,15 +1783,15 @@
 BoxCox = partial(sklearn.preprocessing.PowerTransformer, method='box-cox')
 setattr(BoxCox, '__name__', 'BoxCox')
 YeoJohnshon = partial(sklearn.preprocessing.PowerTransformer, method='yeo-johnson')
 setattr(YeoJohnshon, '__name__', 'YeoJohnshon')
 Quantile = partial(sklearn.preprocessing.QuantileTransformer, n_quantiles=1_000, output_distribution='normal', random_state=0)
 setattr(Quantile, '__name__', 'Quantile')
 
-# %% ../../nbs/009_data.preprocessing.ipynb 124
+# %% ../../nbs/009_data.preprocessing.ipynb 142
 def ReLabeler(cm):
     r"""Changes the labels in a dataset based on a dictionary (class mapping) 
         Args:
             cm = class mapping dictionary
     """
     def _relabel(y):
         obj = len(set([len(listify(v)) for v in cm.values()])) > 1
```

### Comparing `tsai-0.3.6/tsai/data/tabular.py` & `tsai-0.3.7/tsai/data/tabular.py`

 * *Files identical despite different names*

### Comparing `tsai-0.3.6/tsai/data/transforms.py` & `tsai-0.3.7/tsai/data/transforms.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,16 @@
            'random_curve_generator', 'random_cum_curve_generator', 'random_cum_noise_generator',
            'random_cum_linear_generator', 'TSTimeNoise', 'TSMagWarp', 'TSTimeWarp', 'TSWindowWarp', 'TSMagScale',
            'TSMagScalePerVar', 'TSRandomResizedCrop', 'TSWindowSlicing', 'TSRandomZoomOut', 'TSRandomTimeScale',
            'TSRandomTimeStep', 'TSResampleSteps', 'TSBlur', 'TSSmooth', 'maddest', 'TSFreqDenoise', 'TSRandomFreqNoise',
            'TSRandomResizedLookBack', 'TSRandomLookBackOut', 'TSVarOut', 'TSCutOut', 'TSTimeStepOut', 'TSRandomCropPad',
            'TSMaskOut', 'TSInputDropout', 'TSTranslateX', 'TSRandomShift', 'TSHorizontalFlip', 'TSRandomTrend',
            'TSVerticalFlip', 'TSResize', 'TSRandomSize', 'TSRandomLowRes', 'TSDownUpScale', 'TSRandomDownUpScale',
-           'TSRandomConv', 'TSRandom2Value', 'TSMask2Value', 'RandAugment', 'TestTfm', 'get_tfm_name']
+           'TSRandomConv', 'TSRandom2Value', 'TSMask2Value', 'self_mask', 'TSSelfDropout', 'RandAugment', 'TestTfm',
+           'get_tfm_name']
 
 # %% ../../nbs/010_data.transforms.ipynb 3
 from ..imports import *
 from scipy.interpolate import CubicSpline
 from scipy.ndimage import convolve1d
 from fastcore.transform import compose_tfms
 from fastai.vision.augment import RandTransform
@@ -863,14 +864,29 @@
     def encodes(self, o:TSTensor):
         mask = self.mask_fn(o)
         if self.sel_vars is not None:
             mask[:, self.sel_vars] = False
         return o.masked_fill(mask, self.value)
 
 # %% ../../nbs/010_data.transforms.ipynb 98
+def self_mask(o): 
+    mask1 = torch.isnan(o)
+    mask2 = rotate_axis0(mask1)
+    return torch.logical_and(mask2, ~mask1)
+
+
+class TSSelfDropout(RandTransform):
+    """Applies dropout to a tensor with nan values by rotating axis=0 inplace"""
+    order = 90
+    def encodes(self, o: TSTensor):
+        mask = self_mask(o)
+        o[mask] = np.nan
+        return o
+
+# %% ../../nbs/010_data.transforms.ipynb 100
 all_TS_randaugs = [
     
     TSIdentity, 
     
     # Noise
     (TSMagAddNoise, 0.1, 1.),
     (TSGaussianNoise, .01, 1.),
@@ -912,15 +928,15 @@
     (TSRandomResizedLookBack, 0.1, 1.),
     (TSTimeStepOut, 0.01, 0.2),
     (TSRandomCropPad, 0.05, 0.5), 
     (TSRandomResizedCrop, 0.05, 0.5),
     (TSMaskOut, 0.01, 0.2),
 ]
 
-# %% ../../nbs/010_data.transforms.ipynb 99
+# %% ../../nbs/010_data.transforms.ipynb 101
 class RandAugment(RandTransform):
     order = 90
     def __init__(self, tfms:list, N:int=1, M:int=3, **kwargs):
         '''
         tfms   : list of tfm functions (not called)
         N      : number of tfms applied to each batch (usual values 1-3)
         M      : tfm magnitude multiplier (1-10, usually 3-5). Only works if tfms are tuples (tfm, min, max)
@@ -939,28 +955,28 @@
             if isinstance(tfm, tuple):
                 t, min_val, max_val = tfm
                 tfms_ += [t(magnitude=self.magnitude * float(max_val - min_val) + min_val)]
             else:  tfms_ += [tfm()]
         output = compose_tfms(o, tfms_, split_idx=self.split_idx)
         return output
 
-# %% ../../nbs/010_data.transforms.ipynb 101
+# %% ../../nbs/010_data.transforms.ipynb 103
 class TestTfm(RandTransform):
     "Utility class to test the output of selected tfms during training"
     def __init__(self, tfm, magnitude=1., ex=None, **kwargs): 
         self.tfm, self.magnitude, self.ex = tfm, magnitude, ex
         self.tfmd, self.shape = [], []
         super().__init__(**kwargs)
     def encodes(self, o: TSTensor): 
         if not self.magnitude or self.magnitude <= 0: return o
         output = self.tfm(o, split_idx=self.split_idx)
         self.tfmd.append(torch.equal(o, output))
         self.shape.append(o.shape)
         return output
 
-# %% ../../nbs/010_data.transforms.ipynb 102
+# %% ../../nbs/010_data.transforms.ipynb 104
 def get_tfm_name(tfm):
     if isinstance(tfm, tuple): tfm = tfm[0]
     if hasattr(tfm, "func"): tfm = tfm.func
     if hasattr(tfm, "__name__"): return tfm.__name__
     elif hasattr(tfm, "__class__") and hasattr(tfm.__class__, "__name__"): return tfm.__class__.__name__
     else: return tfm
```

### Comparing `tsai-0.3.6/tsai/data/unwindowed.py` & `tsai-0.3.7/tsai/data/unwindowed.py`

 * *Files identical despite different names*

### Comparing `tsai-0.3.6/tsai/data/validation.py` & `tsai-0.3.7/tsai/data/validation.py`

 * *Files 2% similar despite different names*

```diff
@@ -382,21 +382,29 @@
         
     def _inner(o):
         valid_cut = valid_size if isinstance(valid_size, Integral) else round(valid_size * len(o))
         if test_size: 
             test_cut = test_size if isinstance(test_size, Integral) else round(test_size * len(o))
         else:
             test_cut = 0
-        idx = np.arange(len(o))
+        idx = np.arange(len(o), dtype=smallest_dtype(len(o)))
         if test_size: 
-            splits = (L(idx[:-valid_cut - test_cut - fcst_horizon].tolist()), 
-                      L(idx[-valid_cut - test_cut: - test_cut - fcst_horizon].tolist()),
-                      L(idx[-test_cut:].tolist()))
+            if len(idx) < 1_000_000:
+                splits = (L(idx[:-valid_cut - test_cut - fcst_horizon].tolist()), 
+                          L(idx[-valid_cut - test_cut: - test_cut - fcst_horizon].tolist()),
+                          L(idx[-test_cut:].tolist()))
+            else:
+                splits = (idx[:-valid_cut - test_cut - fcst_horizon], 
+                          idx[-valid_cut - test_cut: - test_cut - fcst_horizon],
+                          idx[-test_cut:])
         else: 
-            splits = (L(idx[:-valid_cut - fcst_horizon].tolist()), L(idx[-valid_cut:].tolist()))
+            if len(idx) < 1_000_000:
+                splits = (L(idx[:-valid_cut - fcst_horizon].tolist()), L(idx[-valid_cut:].tolist()))
+            else:
+                splits = (idx[:-valid_cut - fcst_horizon], idx[-valid_cut:])
         if show_plot: 
             if len(o) > 1_000_000:
                 warnings.warn('the splits are too large to be plotted')
             else: 
                 plot_splits(splits) if test_size else plot_splits(splits[:2])
         return splits
     return _inner
@@ -427,42 +435,48 @@
         if isinstance(split[0], (list, L, tuple)):  _len.append([len(s) for s in split])
         else: _len.append(len(split))
     return _len
 
 # %% ../../nbs/003_data.validation.ipynb 41
 def get_usable_idxs(df, fcst_history, fcst_horizon, stride=1):
     if len(df) < fcst_history + fcst_horizon:
-        return []
+        return np.array([], dtype=int)
     usable_idxs = df[fcst_history - 1:len(df) - fcst_horizon].index.values
     if stride != 1:
         usable_idxs = usable_idxs[::-stride][::-1]
     return usable_idxs
 
 
 def get_df_usable_idxs(
     df,                         # dataframe containing a sorted time series
     fcst_history,               # # historical steps used as input (size of the sliding window for the input)
     fcst_horizon,               # # steps forecasted into the future (size of the sliding window for the target)
     stride=1,                   # int or tuple of 2 int containing the strides of the sliding windows (input and target)
     unique_id_cols=None,        # str indicating the column/s with the unique identifier/s for each entity
+    return_np_indices=False,    # bool indicating what type of indices are returned. Default to False (dataframe indices)
 ):
+    "Calculates the indices that can be used from a df when using a sliding window"
+    
     dtype = smallest_dtype(len(df))
     if unique_id_cols is not None:
         usable_df_idxs = np.sort(np.concatenate(df
                                                 .reset_index(drop=True)
                                                 .groupby(unique_id_cols)
                                                 .apply(lambda x: get_usable_idxs(x, 
                                                                                  fcst_history=fcst_history, 
                                                                                  fcst_horizon=fcst_horizon, 
                                                                                  stride=stride
                                                                                 )).values, dtype=dtype))
     else:
         usable_df_idxs = np.sort(get_usable_idxs(df, fcst_history, fcst_horizon, stride).astype(dtype=dtype))
+    if return_np_indices:
+        usable_df_idxs = usable_df_idxs - (fcst_history - 1)
     return usable_df_idxs
 
+
 # %% ../../nbs/003_data.validation.ipynb 42
 def calculate_fcst_stats(
     df, # dataframe containing a sorted time series for a single entity or subject
     fcst_history, # # historical steps used as input.
     fcst_horizon, # # steps forecasted into the future. 
     splits, # splits that will be used to train the model. splits[0] is the train split:
     x_vars=None, # features used as input
```

### Comparing `tsai-0.3.6/tsai/export.py` & `tsai-0.3.7/tsai/export.py`

 * *Files 1% similar despite different names*

```diff
@@ -216,15 +216,17 @@
             nb_path = get_nb_path()
         except: 
             print("nb2py couldn't get the nb name. Pass it as an nb argument and rerun nb2py.")
             return
     if nb_path is None: 
         print("nb2py couldn't get the nb name. Pass it as an nb argument and rerun nb2py.")
         return
+    
     nb_name = nb_path.name
+    nb_path = Path(nb_path).absolute()
     assert os.path.isfile(nb_path), f"nb2py couldn't find {nb_path}. Please, confirm the path is correct."
     
     # save nb: only those that are run from the notebook itself
     if save and not is_colab() and nb is None: 
         try: save_nb(nb_name)
         except: print(f"nb2py couldn't save the nb automatically. It will used last saved at {to_local_time(os.path.getmtime(nb_name))}")
```

### Comparing `tsai-0.3.6/tsai/imports.py` & `tsai-0.3.7/tsai/imports.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 import time
 import warnings
 from configparser import ConfigParser
 from functools import partial
 from numbers import Integral
 from pathlib import Path
 from time import strftime
+from tqdm import tqdm
 from typing import (
     Dict,
     Generator,
     Iterable,
     Iterator,
     List,
     Optional,
@@ -56,14 +57,15 @@
 from fastcore.dispatch import *
 from fastcore.foundation import *
 from fastcore.imports import *
 from fastcore.meta import *
 from fastcore.test import *
 from fastcore.xtras import *
 from numpy import array
+from numpy.lib.stride_tricks import sliding_window_view
 from torch import Tensor
 
 config = ConfigParser(delimiters=["="])
 config.read("../settings.ini")
 cfg = config["DEFAULT"]
 lib_name = cfg.get("lib_name")
 
@@ -147,16 +149,16 @@
         _save_nb()
     else:
         saved = False
         current_time = time.time()
         for i in range(attempts):
             _save_nb()
             # confirm it's saved. This takes come variable time.
-            for j in range(20):
-                time.sleep(0.5)
+            for j in range(10):
+                time.sleep(1)
                 saved_time = os.path.getmtime(nb_name)
                 if saved_time >= current_time:
                     break
             if saved_time >= current_time:
                 saved = True
                 break
         if verbose:
@@ -225,15 +227,15 @@
         path = Path.cwd()
         nb_name = Path(nb_name).name
         full_nb_name = str(path / nb_name)
         nb_export(full_nb_name)
         output = py_last_saved(nb_name, max_elapsed)
         beep(output)
     else:
-        nb_export()
+        print("Couldn't get nb_name. Script not created 😔")
 
 
 class Timer:
     def __init__(self, verbose=True, return_seconds=True, instance=None):
         self.verbose, self.return_seconds, self.instance = verbose, return_seconds, instance
 
     def start(self, verbose=None, return_seconds=None, instance=None):
```

### Comparing `tsai-0.3.6/tsai/inference.py` & `tsai-0.3.7/tsai/inference.py`

 * *Files identical despite different names*

### Comparing `tsai-0.3.6/tsai/learner.py` & `tsai-0.3.7/tsai/learner.py`

 * *Files 3% similar despite different names*

```diff
@@ -95,19 +95,21 @@
     pv(f"learner_fname = '{learner_fname}.pkl'", verbose)
     
     
 def load_all(path='export', dls_fname='dls', model_fname='model', learner_fname='learner', device=None, pickle_module=pickle, verbose=False):
 
     if isinstance(device, int): device = torch.device('cuda', device)
     elif device is None: device = default_device()
-    if device == 'cpu': cpu = True
+    if device.type == 'cpu': cpu = True
     else: cpu = None
 
     path = Path(path)
     learn = load_learner(path/f'{learner_fname}.pkl', cpu=cpu, pickle_module=pickle_module)
+    learn.path = path
+    learn.model_dir = Path() # '.'
     learn.load(f'{model_fname}', with_opt=True, device=device)
 
     
     if learn.dls_type == "MixedDataLoaders":
         from tsai.data.mixed import MixedDataLoader, MixedDataLoaders
         dls_fnames = []
         _dls = []
@@ -140,15 +142,15 @@
     pv(f"dls_fname     = '{dls_fnames}'", verbose)
     pv(f"model_fname   = '{model_fname}.pth'", verbose)
     pv(f"learner_fname = '{learner_fname}.pkl'", verbose)
     return learn
 
 load_learner_all = load_all
 
-# %% ../nbs/018_learner.ipynb 10
+# %% ../nbs/018_learner.ipynb 11
 @patch
 @delegates(subplots)
 def plot_metrics(self: Recorder, nrows=None, ncols=None, figsize=None, final_losses=True, perc=.5, **kwargs):
     
     n_values = len(self.recorder.values)
     if n_values < 2:
         print('not enough values to plot a chart')
@@ -226,30 +228,33 @@
     
     
 @patch
 @delegates(subplots)
 def plot_metrics(self: Learner, **kwargs):
     self.recorder.plot_metrics(**kwargs)
 
-# %% ../nbs/018_learner.ipynb 11
+# %% ../nbs/018_learner.ipynb 12
 all_arch_names =  ['FCN', 'FCNPlus', 'InceptionTime', 'InceptionTimePlus', 'InCoordTime', 'XCoordTime', 'InceptionTimePlus17x17', 'InceptionTimePlus32x32', 
                    'InceptionTimePlus47x47', 'InceptionTimePlus62x62', 'InceptionTimeXLPlus', 'MultiInceptionTimePlus', 'MiniRocketClassifier', "MiniRocket",
-                   'MiniRocketRegressor', 'MiniRocketVotingClassifier', 'MiniRocketVotingRegressor', 'MiniRocketPlus', 
+                   'MiniRocketRegressor', 'MiniRocketVotingClassifier', 'MiniRocketVotingRegressor', 'MiniRocketPlus', 'MultiRocket', 'MultiRocketPlus',
                    'MiniRocketHead', 'InceptionRocketPlus', 'MLP', 'gMLP', 'MultiInputNet', 'OmniScaleCNN', 'RNN', 'LSTM', 'GRU', 
                    'RNNPlus', 'LSTMPlus', 'GRUPlus', 'RNN_FCN', 'LSTM_FCN', 'GRU_FCN', 'MRNN_FCN', 'MLSTM_FCN', 'MGRU_FCN', 'ROCKET', 'RocketClassifier', 
                    'RocketRegressor', 'ResCNN', 'ResNet', 'ResNetPlus', 'TCN', 'TSPerceiver', 'TST', 'TSTPlus', 'MultiTSTPlus', 'TSiTPlus', 
                    'TabFusionTransformer', 'TSTabFusionTransformer', 'TabModel', 'TabTransformer', 'GatedTabTransformer', 'TransformerModel', 'XCM', 'XCMPlus', 
                    'xresnet1d18', 'xresnet1d34', 'xresnet1d50', 'xresnet1d101', 'xresnet1d152', 'xresnet1d18_deep', 'xresnet1d34_deep', 'xresnet1d50_deep', 
                    'xresnet1d18_deeper', 'xresnet1d34_deeper', 'xresnet1d50_deeper', 'XResNet1dPlus', 'xresnet1d18plus', 'xresnet1d34plus', 
                    'xresnet1d50plus', 'xresnet1d101plus', 'xresnet1d152plus', 'xresnet1d18_deepplus', 'xresnet1d34_deepplus', 'xresnet1d50_deepplus', 
                    'xresnet1d18_deeperplus', 'xresnet1d34_deeperplus', 'xresnet1d50_deeperplus', 'XceptionTime', 'XceptionTimePlus', 'mWDN',
-                   'TSSequencer', 'TSSequencerPlus', "PatchTST", "RNNAttention", "LSTMAttention", "GRUAttention"]
+                   'TSSequencer', 'TSSequencerPlus', "PatchTST", "RNNAttention", "LSTMAttention", "GRUAttention", 
+                   "TransformerRNNPlus", "TransformerLSTMPlus", "TransformerGRUPlus"]
 
 
 def get_arch(arch_name):
+    if not isinstance(arch_name, str): return arch_name
+    arch = None
     if arch_name == "FCN":  
         from tsai.models.FCN import FCN
         arch = FCN
     elif arch_name == "FCNPlus":  
         from tsai.models.FCNPlus import FCNPlus
         arch = FCNPlus
     elif arch_name == "InceptionTime":  
@@ -296,14 +301,20 @@
         arch = MiniRocketVotingRegressor
     elif arch_name == "MiniRocketFeaturesPlus":  
         from tsai.models.MINIROCKETPlus_Pytorch import MiniRocketFeaturesPlus
         arch = MiniRocketFeaturesPlus
     elif arch_name == "MiniRocket":  
         from tsai.models.MINIROCKET_Pytorch import MiniRocket
         arch = MiniRocket
+    elif arch_name == "MultiRocket":  
+        from tsai.models.MultiRocketPlus import MultiRocket
+        arch = MultiRocket
+    elif arch_name == "MultiRocketPlus":  
+        from tsai.models.MultiRocketPlus import MultiRocketPlus
+        arch = MultiRocketPlus
     elif arch_name == "MiniRocketPlus":  
         from tsai.models.MINIROCKETPlus_Pytorch import MiniRocketPlus
         arch = MiniRocketPlus
     elif arch_name == "MiniRocketHead":  
         from tsai.models.MINIROCKETPlus_Pytorch import MiniRocketHead
         arch = MiniRocketHead
     elif arch_name == "InceptionRocketFeaturesPlus":  
@@ -446,17 +457,14 @@
         arch = TransformerModel
     elif arch_name == "XCM":  
         from tsai.models.XCM import XCM
         arch = XCM
     elif arch_name == "XCMPlus":  
         from tsai.models.XCMPlus import XCMPlus
         arch = XCMPlus
-    elif arch_name == "XResNet1d":  
-        from tsai.models.XResNet1d import XResNet1d
-        arch = XResNet1d
     elif arch_name == "xresnet1d18":  
         from tsai.models.XResNet1d import xresnet1d18
         arch = xresnet1d18
     elif arch_name == "xresnet1d34":  
         from tsai.models.XResNet1d import xresnet1d34
         arch = xresnet1d34
     elif arch_name == "xresnet1d50":  
@@ -539,36 +547,51 @@
         arch = RNNAttention
     elif arch_name == "LSTMAttention":  
         from tsai.models.RNNAttention import LSTMAttention
         arch = LSTMAttention
     elif arch_name == "GRUAttention":  
         from tsai.models.RNNAttention import GRUAttention
         arch = GRUAttention
-    else: print(f"please, confirm the name of the architecture ({arch_name})")
+    elif arch_name == "TransformerRNNPlus":
+        from tsai.models.TransformerRNNPlus import TransformerRNNPlus
+        arch = TransformerRNNPlus
+    elif arch_name == "TransformerLSTMPlus":
+        from tsai.models.TransformerRNNPlus import TransformerLSTMPlus
+        arch = TransformerLSTMPlus
+    elif arch_name == "TransformerGRUPlus":
+        from tsai.models.TransformerRNNPlus import TransformerGRUPlus
+        arch = TransformerGRUPlus
+    else: 
+        raise ValueError(f"Architecture {arch_name} not found. Please, check the name is correct.")
+    
     assert arch.__name__.replace("Plus", "") == arch_name.replace("Plus", ""), f"{arch.__name__} - {arch_name}"
     return arch
 
-# %% ../nbs/018_learner.ipynb 13
+# %% ../nbs/018_learner.ipynb 14
 @delegates(build_ts_model)
-def ts_learner(dls, arch=None, c_in=None, c_out=None, seq_len=None, d=None, splitter=trainable_params,
-               loss_func=None, opt_func=Adam, lr=defaults.lr, cbs=None, metrics=None, path=None,
+def ts_learner(dls, arch=None, c_in=None, c_out=None, seq_len=None, d=None, 
+               s_cat_idxs=None, s_cat_embeddings=None, s_cat_embedding_dims=None, s_cont_idxs=None, 
+               o_cat_idxs=None, o_cat_embeddings=None, o_cat_embedding_dims=None, o_cont_idxs=None,
+               splitter=trainable_params, loss_func=None, opt_func=Adam, lr=defaults.lr, cbs=None, metrics=None, path=None,
                model_dir='models', wd=None, wd_bn_bias=False, train_bn=True, moms=(0.95,0.85,0.95), 
                train_metrics=False, valid_metrics=True, seed=None, **kwargs)->Learner:
 
     if seed is not None:
         set_seed(seed, reproducible=True)
     
     if isinstance(arch, nn.Module): 
         model = arch
         if kwargs: 
             warnings.warn("You have passed kwargs to a model that is already intantiated. They will not have any effect.", UserWarning)
     else:
         if arch is None: arch = InceptionTimePlus
         elif isinstance(arch, str): arch = get_arch(arch)
-        model = build_ts_model(arch, dls=dls, c_in=c_in, c_out=c_out, seq_len=seq_len, d=d, **kwargs)
+        model = build_ts_model(arch, dls=dls, c_in=c_in, c_out=c_out, seq_len=seq_len, d=d, 
+                               s_cat_idxs=s_cat_idxs, s_cat_embeddings=s_cat_embeddings, s_cat_embedding_dims=s_cat_embedding_dims, s_cont_idxs=s_cont_idxs, 
+                               o_cat_idxs=o_cat_idxs, o_cat_embeddings=o_cat_embeddings, o_cat_embedding_dims=o_cat_embedding_dims, o_cont_idxs=o_cont_idxs, **kwargs)
     if hasattr(model, "backbone") and hasattr(model, "head"):
         splitter = ts_splitter
     if loss_func is None:
         if hasattr(dls, 'loss_func'): loss_func = dls.loss_func
         elif hasattr(dls, 'train_ds') and hasattr(dls.train_ds, 'loss_func'): loss_func = dls.train_ds.loss_func
         elif hasattr(dls, 'cat') and not dls.cat: loss_func = MSELossFlat()
         
@@ -581,15 +604,15 @@
             learn.recorder.valid_metrics = valid_metrics if len(dls.valid) > 0 else False
     
     # keep track of args for loggers
     store_attr('arch', self=learn)
 
     return learn
 
-# %% ../nbs/018_learner.ipynb 14
+# %% ../nbs/018_learner.ipynb 15
 @delegates(build_tsimage_model)
 def tsimage_learner(dls, arch=None, pretrained=False,
                loss_func=None, opt_func=Adam, lr=defaults.lr, cbs=None, metrics=None, path=None,
                model_dir='models', wd=None, wd_bn_bias=False, train_bn=True, moms=(0.95,0.85,0.95),
                **kwargs):
 
     if arch is None: 
@@ -602,10 +625,10 @@
                     model_dir=model_dir, wd=wd, wd_bn_bias=wd_bn_bias, train_bn=train_bn, moms=moms)
 
     # keep track of args for loggers
     store_attr('arch', self=learn)
 
     return learn
 
-# %% ../nbs/018_learner.ipynb 15
+# %% ../nbs/018_learner.ipynb 16
 @patch
 def decoder(self:Learner, o): return L([self.dls.decodes(oi) for oi in o])
```

### Comparing `tsai-0.3.6/tsai/losses.py` & `tsai-0.3.7/tsai/losses.py`

 * *Files identical despite different names*

### Comparing `tsai-0.3.6/tsai/metrics.py` & `tsai-0.3.7/tsai/metrics.py`

 * *Files identical despite different names*

### Comparing `tsai-0.3.6/tsai/models/FCN.py` & `tsai-0.3.7/tsai/models/FCN.py`

 * *Files identical despite different names*

### Comparing `tsai-0.3.6/tsai/models/FCNPlus.py` & `tsai-0.3.7/tsai/models/FCNPlus.py`

 * *Files identical despite different names*

### Comparing `tsai-0.3.6/tsai/models/GatedTabTransformer.py` & `tsai-0.3.7/tsai/models/GatedTabTransformer.py`

 * *Files identical despite different names*

### Comparing `tsai-0.3.6/tsai/models/InceptionTime.py` & `tsai-0.3.7/tsai/models/InceptionTime.py`

 * *Files identical despite different names*

### Comparing `tsai-0.3.6/tsai/models/InceptionTimePlus.py` & `tsai-0.3.7/tsai/models/InceptionTimePlus.py`

 * *Files identical despite different names*

### Comparing `tsai-0.3.6/tsai/models/MINIROCKET.py` & `tsai-0.3.7/tsai/models/MINIROCKET.py`

 * *Files identical despite different names*

### Comparing `tsai-0.3.6/tsai/models/MINIROCKETPlus_Pytorch.py` & `tsai-0.3.7/tsai/models/MINIROCKETPlus_Pytorch.py`

 * *Files identical despite different names*

### Comparing `tsai-0.3.6/tsai/models/MINIROCKET_Pytorch.py` & `tsai-0.3.7/tsai/models/MINIROCKET_Pytorch.py`

 * *Files identical despite different names*

### Comparing `tsai-0.3.6/tsai/models/MLP.py` & `tsai-0.3.7/tsai/models/MLP.py`

 * *Files identical despite different names*

### Comparing `tsai-0.3.6/tsai/models/MultiInputNet.py` & `tsai-0.3.7/tsai/models/MultiInputNet.py`

 * *Files identical despite different names*

### Comparing `tsai-0.3.6/tsai/models/OmniScaleCNN.py` & `tsai-0.3.7/tsai/models/OmniScaleCNN.py`

 * *Files identical despite different names*

### Comparing `tsai-0.3.6/tsai/models/PatchTST.py` & `tsai-0.3.7/tsai/models/PatchTST.py`

 * *Files identical despite different names*

### Comparing `tsai-0.3.6/tsai/models/RNN.py` & `tsai-0.3.7/tsai/models/RNN.py`

 * *Files identical despite different names*

### Comparing `tsai-0.3.6/tsai/models/RNNAttention.py` & `tsai-0.3.7/tsai/models/RNNAttention.py`

 * *Files identical despite different names*

### Comparing `tsai-0.3.6/tsai/models/RNNPlus.py` & `tsai-0.3.7/tsai/models/RNNPlus.py`

 * *Files identical despite different names*

### Comparing `tsai-0.3.6/tsai/models/RNN_FCN.py` & `tsai-0.3.7/tsai/models/RNN_FCN.py`

 * *Files identical despite different names*

### Comparing `tsai-0.3.6/tsai/models/RNN_FCNPlus.py` & `tsai-0.3.7/tsai/models/RNN_FCNPlus.py`

 * *Files identical despite different names*

### Comparing `tsai-0.3.6/tsai/models/ROCKET.py` & `tsai-0.3.7/tsai/models/ROCKET.py`

 * *Files identical despite different names*

### Comparing `tsai-0.3.6/tsai/models/ROCKET_Pytorch.py` & `tsai-0.3.7/tsai/models/ROCKET_Pytorch.py`

 * *Files identical despite different names*

### Comparing `tsai-0.3.6/tsai/models/ResCNN.py` & `tsai-0.3.7/tsai/models/ResCNN.py`

 * *Files identical despite different names*

### Comparing `tsai-0.3.6/tsai/models/ResNet.py` & `tsai-0.3.7/tsai/models/ResNet.py`

 * *Files identical despite different names*

### Comparing `tsai-0.3.6/tsai/models/ResNetPlus.py` & `tsai-0.3.7/tsai/models/ResNetPlus.py`

 * *Files identical despite different names*

### Comparing `tsai-0.3.6/tsai/models/TCN.py` & `tsai-0.3.7/tsai/models/TCN.py`

 * *Files identical despite different names*

### Comparing `tsai-0.3.6/tsai/models/TSPerceiver.py` & `tsai-0.3.7/tsai/models/TSPerceiver.py`

 * *Files identical despite different names*

### Comparing `tsai-0.3.6/tsai/models/TSSequencerPlus.py` & `tsai-0.3.7/tsai/models/TSSequencerPlus.py`

 * *Files identical despite different names*

### Comparing `tsai-0.3.6/tsai/models/TST.py` & `tsai-0.3.7/tsai/models/TST.py`

 * *Files identical despite different names*

### Comparing `tsai-0.3.6/tsai/models/TSTPlus.py` & `tsai-0.3.7/tsai/models/TSTPlus.py`

 * *Files identical despite different names*

### Comparing `tsai-0.3.6/tsai/models/TSiTPlus.py` & `tsai-0.3.7/tsai/models/TSiTPlus.py`

 * *Files identical despite different names*

### Comparing `tsai-0.3.6/tsai/models/TabFusionTransformer.py` & `tsai-0.3.7/tsai/models/TabFusionTransformer.py`

 * *Files identical despite different names*

### Comparing `tsai-0.3.6/tsai/models/TabModel.py` & `tsai-0.3.7/tsai/models/TabModel.py`

 * *Files identical despite different names*

### Comparing `tsai-0.3.6/tsai/models/TabTransformer.py` & `tsai-0.3.7/tsai/models/TabTransformer.py`

 * *Files identical despite different names*

### Comparing `tsai-0.3.6/tsai/models/TransformerModel.py` & `tsai-0.3.7/tsai/models/TransformerModel.py`

 * *Files identical despite different names*

### Comparing `tsai-0.3.6/tsai/models/XCM.py` & `tsai-0.3.7/tsai/models/XCM.py`

 * *Files identical despite different names*

### Comparing `tsai-0.3.6/tsai/models/XCMPlus.py` & `tsai-0.3.7/tsai/models/XCMPlus.py`

 * *Files identical despite different names*

### Comparing `tsai-0.3.6/tsai/models/XResNet1d.py` & `tsai-0.3.7/tsai/models/XResNet1d.py`

 * *Files identical despite different names*

### Comparing `tsai-0.3.6/tsai/models/XResNet1dPlus.py` & `tsai-0.3.7/tsai/models/XResNet1dPlus.py`

 * *Files identical despite different names*

### Comparing `tsai-0.3.6/tsai/models/XceptionTime.py` & `tsai-0.3.7/tsai/models/XceptionTime.py`

 * *Files identical despite different names*

### Comparing `tsai-0.3.6/tsai/models/XceptionTimePlus.py` & `tsai-0.3.7/tsai/models/XceptionTimePlus.py`

 * *Files identical despite different names*

### Comparing `tsai-0.3.6/tsai/models/all.py` & `tsai-0.3.7/tsai/models/all.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,15 +21,17 @@
 from .RNN_FCN import *
 from .RNN_FCNPlus import *
 from .ROCKET import *
 from .MINIROCKET import *
 from .ROCKET_Pytorch import *
 from .MINIROCKET_Pytorch import *
 from .MINIROCKETPlus_Pytorch import *
+from .MultiRocketPlus import *
 from .TransformerModel import *
+from .TransformerRNNPlus import *
 from .TST import *
 from .TSTPlus import *
 from .XceptionTime import *
 from .XceptionTimePlus import *
 from .XCM import *
 from .XCMPlus import *
 from .XResNet1d import *
```

### Comparing `tsai-0.3.6/tsai/models/explainability.py` & `tsai-0.3.7/tsai/models/explainability.py`

 * *Files identical despite different names*

### Comparing `tsai-0.3.6/tsai/models/gMLP.py` & `tsai-0.3.7/tsai/models/gMLP.py`

 * *Files identical despite different names*

### Comparing `tsai-0.3.6/tsai/models/layers.py` & `tsai-0.3.7/tsai/models/layers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1062,15 +1062,15 @@
         layers = []
         if use_bn:
             layers += [nn.BatchNorm1d(n_in)]
         if fc_dropout:
             layers += [nn.Dropout(fc_dropout)]
         if d is None:
             if not flatten or seq_len == 1:
-                layers += [nn.AdaptiveAvgPool1d(1), Squeeze(-1), nn.Linear(nf, n_out)]
+                layers += [nn.AdaptiveAvgPool1d(1), Squeeze(-1), nn.Linear(n_in, n_out)]
                 if n_out == 1:
                     layers += [Squeeze(-1)]
             else:
                 layers += [Reshape(), nn.Linear(n_in * seq_len, n_out * fd)]
                 if n_out * fd== 1:
                     layers += [Squeeze(-1)]
         else:
```

### Comparing `tsai-0.3.6/tsai/models/mWDN.py` & `tsai-0.3.7/tsai/models/mWDN.py`

 * *Files identical despite different names*

### Comparing `tsai-0.3.6/tsai/models/misc.py` & `tsai-0.3.7/tsai/models/misc.py`

 * *Files identical despite different names*

### Comparing `tsai-0.3.6/tsai/models/positional_encoders.py` & `tsai-0.3.7/tsai/models/positional_encoders.py`

 * *Files identical despite different names*

### Comparing `tsai-0.3.6/tsai/models/utils.py` & `tsai-0.3.7/tsai/models/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -136,56 +136,72 @@
         if len(unmatched_layers) > 0:
             print(f'check unmatched_layers: {unmatched_layers}')
         else:
             print(f"weights from {weights_path} successfully transferred!\n")
 
 # %% ../../nbs/030_models.utils.ipynb 13
 def build_ts_model(arch, c_in=None, c_out=None, seq_len=None, d=None, dls=None, device=None, verbose=False, 
+                   s_cat_idxs=None, s_cat_embeddings=None, s_cat_embedding_dims=None, s_cont_idxs=None, 
+                   o_cat_idxs=None, o_cat_embeddings=None, o_cat_embedding_dims=None, o_cont_idxs=None,
+                   patch_len=None, patch_stride=None, fusion_layers=128, fusion_act='relu', fusion_dropout=0., fusion_use_bn=True, 
                    pretrained=False, weights_path=None, exclude_head=True, cut=-1, init=None, arch_config={}, **kwargs):
 
     device = ifnone(device, default_device())
     if dls is not None:
         c_in = ifnone(c_in, dls.vars)
         c_out = ifnone(c_out, dls.c)
         seq_len = ifnone(seq_len, dls.len)
         d = ifnone(d, dls.d)
-    if d and not 'patchtst' in arch.__name__.lower(): 
-        if 'custom_head' not in kwargs.keys(): 
-            if "rocket" in arch.__name__.lower():
-                kwargs['custom_head'] = partial(rocket_nd_head, d=d)
-            elif "xresnet1d" in arch.__name__.lower():
-                kwargs["custom_head"] = partial(xresnet1d_nd_head, d=d)
-            else:
-                kwargs['custom_head'] = partial(lin_nd_head, d=d)
-        elif not isinstance(kwargs['custom_head'], nn.Module):
-            kwargs['custom_head'] = partial(kwargs['custom_head'], d=d)
-    if 'ltsf_' in arch.__name__.lower() or 'patchtst' in arch.__name__.lower():
-        pv(f'arch: {arch.__name__}(c_in={c_in} c_out={c_out} seq_len={seq_len} pred_dim={d} arch_config={arch_config}, kwargs={kwargs})', verbose)
-        model = (arch(c_in=c_in, c_out=c_out, seq_len=seq_len, pred_dim=d, **arch_config, **kwargs)).to(device=device)
-    elif sum([1 for v in ['RNN_FCN', 'LSTM_FCN', 'RNNPlus', 'LSTMPlus', 'GRUPlus', 'InceptionTime', 'TSiT', 'Sequencer', 'XceptionTimePlus',
-                        'GRU_FCN', 'OmniScaleCNN', 'mWDN', 'TST', 'XCM', 'MLP', 'MiniRocket', 'InceptionRocket', 'ResNetPlus', 
-                        'RNNAttention', 'LSTMAttention', 'GRUAttention']
-            if v in arch.__name__]):
-        pv(f'arch: {arch.__name__}(c_in={c_in} c_out={c_out} seq_len={seq_len} arch_config={arch_config} kwargs={kwargs})', verbose)
-        model = arch(c_in, c_out, seq_len=seq_len, **arch_config, **kwargs).to(device=device)
-    elif 'xresnet' in arch.__name__ and not '1d' in arch.__name__:
-        pv(f'arch: {arch.__name__}(c_in={c_in} n_out={c_out} arch_config={arch_config} kwargs={kwargs})', verbose)
-        model = (arch(c_in=c_in, n_out=c_out, **arch_config, **kwargs)).to(device=device)
-    elif 'xresnet1d' in arch.__name__.lower():
-        pv(f'arch: {arch.__name__}(c_in={c_in} c_out={c_out} seq_len={seq_len} arch_config={arch_config} kwargs={kwargs})', verbose)
-        model = (arch(c_in=c_in, c_out=c_out, seq_len=seq_len, **arch_config, **kwargs)).to(device=device)
-    elif 'minirockethead' in arch.__name__.lower():
-        pv(f'arch: {arch.__name__}(c_in={c_in} seq_len={seq_len} arch_config={arch_config} kwargs={kwargs})', verbose)
-        model = (arch(c_in, c_out, seq_len=1, **arch_config, **kwargs)).to(device=device)
-    elif 'rocket' in arch.__name__.lower():
-        pv(f'arch: {arch.__name__}(c_in={c_in} seq_len={seq_len} arch_config={arch_config} kwargs={kwargs})', verbose)
-        model = (arch(c_in=c_in, seq_len=seq_len, **arch_config, **kwargs)).to(device=device)
+    
+    if s_cat_idxs or s_cat_embeddings or s_cat_embedding_dims or s_cont_idxs or o_cat_idxs or o_cat_embeddings or o_cat_embedding_dims or o_cont_idxs:
+        from tsai.models.multimodal import MultInputWrapper
+        model = MultInputWrapper(arch, c_in=c_in, c_out=c_out, seq_len=seq_len, d=d,
+                                 s_cat_idxs=s_cat_idxs, s_cat_embeddings=s_cat_embeddings, s_cat_embedding_dims=s_cat_embedding_dims, s_cont_idxs=s_cont_idxs, 
+                                 o_cat_idxs=o_cat_idxs, o_cat_embeddings=o_cat_embeddings, o_cat_embedding_dims=o_cat_embedding_dims, o_cont_idxs=o_cont_idxs, 
+                                 patch_len=patch_len, patch_stride=patch_stride, 
+                                 fusion_layers=fusion_layers, fusion_act=fusion_act, fusion_dropout=fusion_dropout, fusion_use_bn=fusion_use_bn,
+                                 **kwargs)
     else:
-        pv(f'arch: {arch.__name__}(c_in={c_in} c_out={c_out} arch_config={arch_config} kwargs={kwargs})', verbose)
-        model = arch(c_in, c_out, **arch_config, **kwargs).to(device=device)
+        if d and arch.__name__ not in ["PatchTST", "PatchTSTPlus", 'TransformerRNNPlus', 'TransformerLSTMPlus', 'TransformerGRUPlus']:
+            if 'custom_head' not in kwargs.keys(): 
+                if "rocket" in arch.__name__.lower():
+                    kwargs['custom_head'] = partial(rocket_nd_head, d=d)
+                elif "xresnet1d" in arch.__name__.lower():
+                    kwargs["custom_head"] = partial(xresnet1d_nd_head, d=d)
+                else:
+                    kwargs['custom_head'] = partial(lin_nd_head, d=d)
+            elif not isinstance(kwargs['custom_head'], nn.Module):
+                kwargs['custom_head'] = partial(kwargs['custom_head'], d=d)
+        if 'ltsf_' in arch.__name__.lower() or 'patchtst' in arch.__name__.lower():
+            pv(f'arch: {arch.__name__}(c_in={c_in} c_out={c_out} seq_len={seq_len} pred_dim={d} arch_config={arch_config}, kwargs={kwargs})', verbose)
+            model = (arch(c_in=c_in, c_out=c_out, seq_len=seq_len, pred_dim=d, **arch_config, **kwargs)).to(device=device)
+        elif arch.__name__ in ['TransformerRNNPlus', 'TransformerLSTMPlus', 'TransformerGRUPlus']:
+            pv(f'arch: {arch.__name__}(c_in={c_in} c_out={c_out} seq_len={seq_len} d={d} arch_config={arch_config}, kwargs={kwargs})', verbose)
+            model = (arch(c_in=c_in, c_out=c_out, seq_len=seq_len, d=d, **arch_config, **kwargs)).to(device=device)
+        elif sum([1 for v in ['RNN_FCN', 'LSTM_FCN', 'RNNPlus', 'LSTMPlus', 'GRUPlus', 'InceptionTime', 'TSiT', 'Sequencer', 'XceptionTimePlus',
+                            'GRU_FCN', 'OmniScaleCNN', 'mWDN', 'TST', 'XCM', 'MLP', 'MiniRocket', 'InceptionRocket', 'ResNetPlus', 
+                            'RNNAttention', 'LSTMAttention', 'GRUAttention', 'MultiRocket', 'MultiRocketPlus']
+                if v in arch.__name__]):
+            pv(f'arch: {arch.__name__}(c_in={c_in} c_out={c_out} seq_len={seq_len} arch_config={arch_config} kwargs={kwargs})', verbose)
+            model = arch(c_in, c_out, seq_len=seq_len, **arch_config, **kwargs).to(device=device)
+        elif 'xresnet' in arch.__name__ and not '1d' in arch.__name__:
+            pv(f'arch: {arch.__name__}(c_in={c_in} n_out={c_out} arch_config={arch_config} kwargs={kwargs})', verbose)
+            model = (arch(c_in=c_in, n_out=c_out, **arch_config, **kwargs)).to(device=device)
+        elif 'xresnet1d' in arch.__name__.lower():
+            pv(f'arch: {arch.__name__}(c_in={c_in} c_out={c_out} seq_len={seq_len} arch_config={arch_config} kwargs={kwargs})', verbose)
+            model = (arch(c_in=c_in, c_out=c_out, seq_len=seq_len, **arch_config, **kwargs)).to(device=device)
+        elif 'minirockethead' in arch.__name__.lower():
+            pv(f'arch: {arch.__name__}(c_in={c_in} seq_len={seq_len} arch_config={arch_config} kwargs={kwargs})', verbose)
+            model = (arch(c_in, c_out, seq_len=1, **arch_config, **kwargs)).to(device=device)
+        elif 'rocket' in arch.__name__.lower():
+            pv(f'arch: {arch.__name__}(c_in={c_in} seq_len={seq_len} arch_config={arch_config} kwargs={kwargs})', verbose)
+            model = (arch(c_in=c_in, seq_len=seq_len, **arch_config, **kwargs)).to(device=device)
+        else:
+            pv(f'arch: {arch.__name__}(c_in={c_in} c_out={c_out} arch_config={arch_config} kwargs={kwargs})', verbose)
+            model = arch(c_in, c_out, **arch_config, **kwargs).to(device=device)
 
     try:
         model[0], model[1]
         subscriptable = True
     except:
         subscriptable = False
     if hasattr(model, "head_nf"):  head_nf = model.head_nf
@@ -269,15 +285,19 @@
     try: 
         params_0 = list(mod.parameters())[0]
         xb = torch.rand(1, c_in, seq_len, device=params_0.device, dtype=params_0.dtype)
     except: 
         xb = torch.rand(1, c_in, seq_len)
     training = mod.training
     mod.eval()
-    c_out, q_len = mod.to(xb.device)(xb).shape[1:]
+    output_shape = tuple(mod.to(xb.device)(xb).shape)
+    if len(output_shape) == 2:
+        c_out, q_len = output_shape[1], None
+    else:
+        c_out, q_len = output_shape[1:]
     mod.training = training
     if return_q_len:
         return c_out, q_len
     else: 
         return c_out, None
 
 # %% ../../nbs/030_models.utils.ipynb 24
```

### Comparing `tsai-0.3.6/tsai/optuna.py` & `tsai-0.3.7/tsai/optuna.py`

 * *Files identical despite different names*

### Comparing `tsai-0.3.6/tsai/tslearner.py` & `tsai-0.3.7/tsai/tslearner.py`

 * *Files 24% similar despite different names*

```diff
@@ -14,15 +14,19 @@
 from .data.core import *
 from .models.InceptionTimePlus import *
 from .models.utils import *
 from .metrics import *
 
 # %% ../nbs/022_tslearner.ipynb 5
 class TSClassifier(Learner):
-    def __init__(self, X, y=None, splits=None, tfms=None, inplace=True, sel_vars=None, sel_steps=None, weights=None, partial_n=None, vocab=None,
+    def __init__(self, X, y=None, splits=None, tfms=None, inplace=True, sel_vars=None, sel_steps=None, 
+                 s_cat_idxs=None, s_cat_embeddings=None, s_cat_embedding_dims=None, s_cont_idxs=None, 
+                 o_cat_idxs=None, o_cat_embeddings=None, o_cat_embedding_dims=None, o_cont_idxs=None,
+                 patch_len=None, patch_stride=None, fusion_layers=128, fusion_act='relu', fusion_dropout=0., fusion_use_bn=True, 
+                 weights=None, partial_n=None, vocab=None,
                  train_metrics=False, valid_metrics=True, bs=[64, 128], batch_size=None, batch_tfms=None, pipelines=None,
                  shuffle_train=True, drop_last=True, num_workers=0, do_setup=True, device=None, seed=None,
                  arch=None, arch_config={}, pretrained=False, weights_path=None, exclude_head=True, cut=-1, init=None,
                  loss_func=None, opt_func=Adam, lr=0.001, metrics=accuracy, cbs=None, wd=None, wd_bn_bias=False,
                  train_bn=True, moms=(0.95, 0.85, 0.95),  path='.', model_dir='models', splitter=trainable_params, verbose=False):
 
         # Seed
@@ -60,16 +64,21 @@
             # if 'xresnet' in arch.__name__.lower() and not '1d' in arch.__name__.lower():
             #     model = build_tsimage_model(arch, dls=dls, pretrained=pretrained, init=init, device=device, verbose=verbose, arch_config=arch_config)
             # elif 'tabularmodel' in arch.__name__.lower():
             #     model = build_tabular_model(arch, dls=dls, device=device, arch_config=arch_config)
             # else:
             #     model = build_ts_model(arch, dls=dls, device=device, verbose=verbose, pretrained=pretrained, weights_path=weights_path,
             #                            exclude_head=exclude_head, cut=cut, init=init, arch_config=arch_config)
-            model = build_ts_model(arch, dls=dls, device=device, verbose=verbose, pretrained=pretrained, weights_path=weights_path,
-                                    exclude_head=exclude_head, cut=cut, init=init, arch_config=arch_config)
+            model = build_ts_model(arch, dls=dls, 
+                                   s_cat_idxs=s_cat_idxs, s_cat_embeddings=s_cat_embeddings, s_cat_embedding_dims=s_cat_embedding_dims, s_cont_idxs=s_cont_idxs, 
+                                   o_cat_idxs=o_cat_idxs, o_cat_embeddings=o_cat_embeddings, o_cat_embedding_dims=o_cat_embedding_dims, o_cont_idxs=o_cont_idxs,
+                                   patch_len=patch_len, patch_stride=patch_stride, 
+                                   fusion_layers=fusion_layers, fusion_act=fusion_act, fusion_dropout=fusion_dropout, fusion_use_bn=fusion_use_bn, 
+                                   device=device, verbose=verbose, pretrained=pretrained, weights_path=weights_path,
+                                   exclude_head=exclude_head, cut=cut, init=init, arch_config=arch_config)
         try:
             setattr(model, "__name__", arch.__name__)
         except:
             setattr(model, "__name__", arch.__class__.__name__)
         
         if hasattr(model, "backbone") and hasattr(model, "head"):
             splitter = ts_splitter
@@ -87,15 +96,19 @@
                 (len(splits) >= 2 and (splits[1] is None or not hasattr(splits[1], "__len__"))): 
                 self.recorder.valid_metrics = False
             else:
                 self.recorder.valid_metrics = valid_metrics
 
 # %% ../nbs/022_tslearner.ipynb 11
 class TSRegressor(Learner):
-    def __init__(self, X, y=None, splits=None, tfms=None, inplace=True, sel_vars=None, sel_steps=None, weights=None, partial_n=None, 
+    def __init__(self, X, y=None, splits=None, tfms=None, inplace=True, sel_vars=None, sel_steps=None, 
+                 s_cat_idxs=None, s_cat_embeddings=None, s_cat_embedding_dims=None, s_cont_idxs=None, 
+                 o_cat_idxs=None, o_cat_embeddings=None, o_cat_embedding_dims=None, o_cont_idxs=None,
+                 patch_len=None, patch_stride=None, fusion_layers=128, fusion_act='relu', fusion_dropout=0., fusion_use_bn=True, 
+                 weights=None, partial_n=None, 
                  train_metrics=False, valid_metrics=True, bs=[64, 128], batch_size=None, batch_tfms=None, pipelines=None,
                  shuffle_train=True, drop_last=True, num_workers=0, do_setup=True, device=None, seed=None,
                  arch=None, arch_config={}, pretrained=False, weights_path=None, exclude_head=True, cut=-1, init=None,
                  loss_func=None, opt_func=Adam, lr=0.001, metrics=None, cbs=None, wd=None, wd_bn_bias=False,
                  train_bn=True, moms=(0.95, 0.85, 0.95),  path='.', model_dir='models', splitter=trainable_params, verbose=False):
 
         # Seed
@@ -134,16 +147,21 @@
             # if 'xresnet' in arch.__name__.lower() and not '1d' in arch.__name__.lower():
             #     model = build_tsimage_model(arch, dls=dls, pretrained=pretrained, init=init, device=device, verbose=verbose, arch_config=arch_config)
             # elif 'tabularmodel' in arch.__name__.lower():
             #     model = build_tabular_model(arch, dls=dls, device=device, arch_config=arch_config)
             # else:
             #     model = build_ts_model(arch, dls=dls, device=device, verbose=verbose, pretrained=pretrained, weights_path=weights_path,
             #                        exclude_head=exclude_head, cut=cut, init=init, arch_config=arch_config)
-            model = build_ts_model(arch, dls=dls, device=device, verbose=verbose, pretrained=pretrained, weights_path=weights_path,
-                                exclude_head=exclude_head, cut=cut, init=init, arch_config=arch_config)
+            model = build_ts_model(arch, dls=dls, 
+                                   s_cat_idxs=s_cat_idxs, s_cat_embeddings=s_cat_embeddings, s_cat_embedding_dims=s_cat_embedding_dims, s_cont_idxs=s_cont_idxs, 
+                                   o_cat_idxs=o_cat_idxs, o_cat_embeddings=o_cat_embeddings, o_cat_embedding_dims=o_cat_embedding_dims, o_cont_idxs=o_cont_idxs,
+                                   patch_len=patch_len, patch_stride=patch_stride, 
+                                   fusion_layers=fusion_layers, fusion_act=fusion_act, fusion_dropout=fusion_dropout, fusion_use_bn=fusion_use_bn,
+                                   device=device, verbose=verbose, pretrained=pretrained, weights_path=weights_path,
+                                   exclude_head=exclude_head, cut=cut, init=init, arch_config=arch_config)
         try:
             setattr(model, "__name__", arch.__name__)
         except:
             setattr(model, "__name__", arch.__class__.__name__)
         
         if hasattr(model, "backbone") and hasattr(model, "head"):
             splitter = ts_splitter
@@ -161,15 +179,19 @@
                 (len(splits) >= 2 and (splits[1] is None or not hasattr(splits[1], "__len__"))): 
                 self.recorder.valid_metrics = False
             else:
                 self.recorder.valid_metrics = valid_metrics
 
 # %% ../nbs/022_tslearner.ipynb 14
 class TSForecaster(Learner):
-    def __init__(self, X, y=None, splits=None, tfms=None, inplace=True, sel_vars=None, sel_steps=None, weights=None, partial_n=None, 
+    def __init__(self, X, y=None, splits=None, tfms=None, inplace=True, sel_vars=None, sel_steps=None, 
+                 s_cat_idxs=None, s_cat_embeddings=None, s_cat_embedding_dims=None, s_cont_idxs=None, 
+                 o_cat_idxs=None, o_cat_embeddings=None, o_cat_embedding_dims=None, o_cont_idxs=None,
+                 patch_len=None, patch_stride=None, fusion_layers=128, fusion_act='relu', fusion_dropout=0., fusion_use_bn=True, 
+                 weights=None, partial_n=None, 
                  train_metrics=False, valid_metrics=True, bs=[64, 128], batch_size=None, batch_tfms=None, pipelines=None,
                  shuffle_train=True, drop_last=True, num_workers=0, do_setup=True, device=None, seed=None,
                  arch=None, arch_config={}, pretrained=False, weights_path=None, exclude_head=True, cut=-1, init=None,
                  loss_func=None, opt_func=Adam, lr=0.001, metrics=None, cbs=None, wd=None, wd_bn_bias=False,
                  train_bn=True, moms=(0.95, 0.85, 0.95),  path='.', model_dir='models', splitter=trainable_params, verbose=False):
 
         # Seed
@@ -207,16 +229,21 @@
             # if 'xresnet' in arch.__name__.lower() and not '1d' in arch.__name__.lower():
             #     model = build_tsimage_model(arch, dls=dls, pretrained=pretrained, init=init, device=device, verbose=verbose, arch_config=arch_config)
             # elif 'tabularmodel' in arch.__name__.lower():
             #     model = build_tabular_model(arch, dls=dls, device=device, arch_config=arch_config)
             # else:
             #     model = build_ts_model(arch, dls=dls, device=device, verbose=verbose, pretrained=pretrained, weights_path=weights_path,
             #                        exclude_head=exclude_head, cut=cut, init=init, arch_config=arch_config)
-            model = build_ts_model(arch, dls=dls, device=device, verbose=verbose, pretrained=pretrained, weights_path=weights_path,
-                                exclude_head=exclude_head, cut=cut, init=init, arch_config=arch_config)
+            model = build_ts_model(arch, dls=dls, 
+                                   s_cat_idxs=s_cat_idxs, s_cat_embeddings=s_cat_embeddings, s_cat_embedding_dims=s_cat_embedding_dims, s_cont_idxs=s_cont_idxs, 
+                                   o_cat_idxs=o_cat_idxs, o_cat_embeddings=o_cat_embeddings, o_cat_embedding_dims=o_cat_embedding_dims, o_cont_idxs=o_cont_idxs,
+                                   patch_len=patch_len, patch_stride=patch_stride, 
+                                   fusion_layers=fusion_layers, fusion_act=fusion_act, fusion_dropout=fusion_dropout, fusion_use_bn=fusion_use_bn,
+                                   device=device, verbose=verbose, pretrained=pretrained, weights_path=weights_path,
+                                   exclude_head=exclude_head, cut=cut, init=init, arch_config=arch_config)
         try:
             setattr(model, "__name__", arch.__name__)
         except:
             setattr(model, "__name__", arch.__class__.__name__)
         
         if hasattr(model, "backbone") and hasattr(model, "head"):
             splitter = ts_splitter
```

### Comparing `tsai-0.3.6/tsai/utils.py` & `tsai-0.3.7/tsai/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
            'torch_nan_to_num', 'torch_masked_to_num', 'mpl_trend', 'int2digits', 'array2digits', 'sincos_encoding',
            'linear_encoding', 'encode_positions', 'sort_generator', 'get_subset_dict', 'create_dir', 'remove_dir',
            'named_partial', 'attrdict2dict', 'dict2attrdict', 'dict2yaml', 'yaml2dict', 'get_config', 'str2list',
            'str2index', 'get_cont_cols', 'get_cat_cols', 'get_mapping', 'map_array', 'log_tfm', 'to_sincos_time',
            'plot_feature_dist', 'rolling_moving_average', 'ffill_sequence', 'bfill_sequence', 'fbfill_sequence',
            'dummify', 'shuffle_along_axis', 'analyze_feature', 'analyze_array', 'get_relpath', 'get_root',
            'to_root_path', 'split_in_chunks', 'save_object', 'load_object', 'get_idxs_to_keep', 'zerofy', 'feat2list',
-           'smallest_dtype', 'plot_forecast']
+           'smallest_dtype', 'plot_forecast', 'str2callable']
 
 # %% ../nbs/002_utils.ipynb 3
 from .imports import *
 import joblib
 import string
 import yaml
 from numbers import Integral
@@ -416,16 +416,16 @@
     else:
         return retain_type(np.stack(o, axis), o[0]) if retain else np.stack(o, axis)
     
     
 def stack_pad(o, padding_value=np.nan):
     'Converts a an iterable into a numpy array using padding if necessary'
     if not is_listy(o) or not is_array(o):
-        if not hasattr(o, "ndim"): o = np.asarray([o])
-        else: o = np.asarray(o)
+        if not hasattr(o, "ndim"): o = np.asarray([o], dtype=object)
+        else: o = np.asarray(o, dtype=object)
     o_ndim = 1
     if o.ndim > 1:
         o_ndim = o.ndim
         o_shape = o.shape
         o = o.flatten()
     o = [oi if (is_array(oi) and oi.ndim > 0) or is_listy(oi) else [oi] for oi in o]
     row_length = len(max(o, key=len))
@@ -1671,7 +1671,57 @@
         for idx in iterator:
             if sel_vars is True:
                 sel_vars = np.arange(y_true.shape[1])
             else:
                 sel_vars = listify(sel_vars)
             for sel_var in sel_vars:
                 _plot_forecast(X_true, y_true, y_pred, sel_var=sel_var, idx=idx, figsize=figsize)
+
+# %% ../nbs/002_utils.ipynb 197
+def str2callable(
+    object_path: str = None # The string representing the object path.
+):
+    "Transform a string into a callable object without importing it in the script."
+
+
+    if object_path in [None, "null", "None", "none"]:
+        return None
+
+
+    pattern = r'([\w\.]+)\((.*)\)'
+    match = re.match(pattern, object_path)
+
+
+    if match:
+        path, args_str = match.groups()
+
+
+        # Parse the arguments string into a dictionary
+        kwargs = {}
+        if args_str:
+            for arg_str in args_str.split(','):
+                key, value = arg_str.split('=')
+                kwargs[key.strip()] = eval(value.strip())
+
+
+        mod_name, object_name = path.rsplit(".", 1)
+    else:
+        mod_name, object_name = object_path.rsplit(".", 1)
+        kwargs = {}
+
+
+    try:
+        mod = importlib.import_module(mod_name)
+        obj = getattr(mod, object_name)
+
+
+        if inspect.isclass(obj):
+            return obj(**kwargs)
+        elif inspect.isfunction(obj):
+            return functools.partial(obj, **kwargs)
+        else:
+            raise TypeError(f"{object_path} is not a class or a function")
+    except (ImportError, AttributeError) as e:
+        raise ImportError(f"Failed to import {object_path}: {e}")
+    except Exception as e:
+        raise TypeError(f"{object_path} is not a class or a function: {e}")
+
```

### Comparing `tsai-0.3.6/tsai/wandb.py` & `tsai-0.3.7/tsai/wandb.py`

 * *Files identical despite different names*

### Comparing `tsai-0.3.6/tsai.egg-info/PKG-INFO` & `tsai-0.3.7/tsai.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsai
-Version: 0.3.6
+Version: 0.3.7
 Summary: Practical Deep Learning for Time Series / Sequential Data library based on fastai & Pytorch
 Home-page: https://github.com/timeseriesAI/tsai/
 Author: Ignacio Oguiza and contributors
 Author-email: oguiza@timeseriesAI.co
 License: Apache Software License 2.0
 Project-URL: Documentation, https://timeseriesAI.github.io/tsai/
 Keywords: fastai time-series time-series-classification time-series-regression deep-learning Pytorch
```

### Comparing `tsai-0.3.6/tsai.egg-info/SOURCES.txt` & `tsai-0.3.7/tsai.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -60,14 +60,15 @@
 tsai/models/InceptionTime.py
 tsai/models/InceptionTimePlus.py
 tsai/models/MINIROCKET.py
 tsai/models/MINIROCKETPlus_Pytorch.py
 tsai/models/MINIROCKET_Pytorch.py
 tsai/models/MLP.py
 tsai/models/MultiInputNet.py
+tsai/models/MultiRocketPlus.py
 tsai/models/OmniScaleCNN.py
 tsai/models/PatchTST.py
 tsai/models/RNN.py
 tsai/models/RNNAttention.py
 tsai/models/RNNPlus.py
 tsai/models/RNN_FCN.py
 tsai/models/RNN_FCNPlus.py
@@ -82,22 +83,24 @@
 tsai/models/TST.py
 tsai/models/TSTPlus.py
 tsai/models/TSiTPlus.py
 tsai/models/TabFusionTransformer.py
 tsai/models/TabModel.py
 tsai/models/TabTransformer.py
 tsai/models/TransformerModel.py
+tsai/models/TransformerRNNPlus.py
 tsai/models/XCM.py
 tsai/models/XCMPlus.py
 tsai/models/XResNet1d.py
 tsai/models/XResNet1dPlus.py
 tsai/models/XceptionTime.py
 tsai/models/XceptionTimePlus.py
 tsai/models/__init__.py
 tsai/models/all.py
 tsai/models/explainability.py
 tsai/models/gMLP.py
 tsai/models/layers.py
 tsai/models/mWDN.py
 tsai/models/misc.py
+tsai/models/multimodal.py
 tsai/models/positional_encoders.py
 tsai/models/utils.py
```

