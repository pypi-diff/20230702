# Comparing `tmp/PJYoloVision-0.0.0.tar.gz` & `tmp/PJYoloVision-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PJYoloVision-0.0.0.tar", last modified: Sun Jul  2 16:30:31 2023, max compression
+gzip compressed data, was "PJYoloVision-0.0.1.tar", last modified: Sun Jul  2 17:45:33 2023, max compression
```

## Comparing `PJYoloVision-0.0.0.tar` & `PJYoloVision-0.0.1.tar`

### file list

```diff
@@ -1,100 +1,100 @@
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-02 16:30:31.384323 PJYoloVision-0.0.0/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)    35149 2023-07-02 16:13:08.000000 PJYoloVision-0.0.0/LICENCE.md
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-02 16:30:31.376323 PJYoloVision-0.0.0/PJYoloVision/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     4906 2023-07-02 16:29:21.000000 PJYoloVision-0.0.0/PJYoloVision/__init__.py
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-02 16:30:31.376323 PJYoloVision-0.0.0/PJYoloVision/nn/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)        0 2023-07-02 16:13:08.000000 PJYoloVision-0.0.0/PJYoloVision/nn/__init__.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     5599 2023-07-02 16:29:22.000000 PJYoloVision-0.0.0/PJYoloVision/nn/autobackend.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)    10975 2023-07-02 16:29:22.000000 PJYoloVision-0.0.0/PJYoloVision/nn/autoshape.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)      867 2023-07-02 16:13:08.000000 PJYoloVision-0.0.0/PJYoloVision/nn/modules.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)    17463 2023-07-02 16:29:21.000000 PJYoloVision-0.0.0/PJYoloVision/nn/tasks.py
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-02 16:30:31.376323 PJYoloVision-0.0.0/PJYoloVision/tracker/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)      162 2023-07-02 16:13:08.000000 PJYoloVision-0.0.0/PJYoloVision/tracker/__init__.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     1594 2023-07-02 16:29:21.000000 PJYoloVision-0.0.0/PJYoloVision/tracker/track.py
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-02 16:30:31.376323 PJYoloVision-0.0.0/PJYoloVision/tracker/trackers/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)      131 2023-07-02 16:13:08.000000 PJYoloVision-0.0.0/PJYoloVision/tracker/trackers/__init__.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     1085 2023-07-02 16:13:08.000000 PJYoloVision-0.0.0/PJYoloVision/tracker/trackers/basetrack.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     4858 2023-07-02 16:13:08.000000 PJYoloVision-0.0.0/PJYoloVision/tracker/trackers/bot_sort.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)    13185 2023-07-02 16:13:08.000000 PJYoloVision-0.0.0/PJYoloVision/tracker/trackers/byte_tracker.py
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-02 16:30:31.376323 PJYoloVision-0.0.0/PJYoloVision/tracker/utils/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)        0 2023-07-02 16:13:08.000000 PJYoloVision-0.0.0/PJYoloVision/tracker/utils/__init__.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)    11965 2023-07-02 16:29:21.000000 PJYoloVision-0.0.0/PJYoloVision/tracker/utils/gmc.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)    18422 2023-07-02 16:13:08.000000 PJYoloVision-0.0.0/PJYoloVision/tracker/utils/kalman_filter.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     7634 2023-07-02 16:13:08.000000 PJYoloVision-0.0.0/PJYoloVision/tracker/utils/matching.py
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-02 16:30:31.376323 PJYoloVision-0.0.0/PJYoloVision/yolo/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)       45 2023-07-02 16:13:08.000000 PJYoloVision-0.0.0/PJYoloVision/yolo/__init__.py
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-02 16:30:31.376323 PJYoloVision-0.0.0/PJYoloVision/yolo/cfg/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)    11774 2023-07-02 16:29:21.000000 PJYoloVision-0.0.0/PJYoloVision/yolo/cfg/__init__.py
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-02 16:30:31.376323 PJYoloVision-0.0.0/PJYoloVision/yolo/core/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)        0 2023-07-02 16:13:08.000000 PJYoloVision-0.0.0/PJYoloVision/yolo/core/__init__.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)    35343 2023-07-02 16:29:21.000000 PJYoloVision-0.0.0/PJYoloVision/yolo/core/exporter.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     9762 2023-07-02 16:29:21.000000 PJYoloVision-0.0.0/PJYoloVision/yolo/core/model.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)    13012 2023-07-02 16:29:22.000000 PJYoloVision-0.0.0/PJYoloVision/yolo/core/predictor.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)    12519 2023-07-02 16:29:21.000000 PJYoloVision-0.0.0/PJYoloVision/yolo/core/results.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)    29828 2023-07-02 16:29:22.000000 PJYoloVision-0.0.0/PJYoloVision/yolo/core/trainer.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     9205 2023-07-02 16:29:22.000000 PJYoloVision-0.0.0/PJYoloVision/yolo/core/validator.py
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-02 16:30:31.380324 PJYoloVision-0.0.0/PJYoloVision/yolo/data/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)      444 2023-07-02 16:13:08.000000 PJYoloVision-0.0.0/PJYoloVision/yolo/data/__init__.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)    31854 2023-07-02 16:29:22.000000 PJYoloVision-0.0.0/PJYoloVision/yolo/data/augment.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     8963 2023-07-02 16:13:08.000000 PJYoloVision-0.0.0/PJYoloVision/yolo/data/base.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     7658 2023-07-02 16:29:21.000000 PJYoloVision-0.0.0/PJYoloVision/yolo/data/build.py
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-02 16:30:31.380324 PJYoloVision-0.0.0/PJYoloVision/yolo/data/dataloaders/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)        0 2023-07-02 16:13:08.000000 PJYoloVision-0.0.0/PJYoloVision/yolo/data/dataloaders/__init__.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)    12613 2023-07-02 16:29:22.000000 PJYoloVision-0.0.0/PJYoloVision/yolo/data/dataloaders/stream_loaders.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)    17533 2023-07-02 16:29:21.000000 PJYoloVision-0.0.0/PJYoloVision/yolo/data/dataloaders/v5augmentations.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)    46519 2023-07-02 16:29:21.000000 PJYoloVision-0.0.0/PJYoloVision/yolo/data/dataloaders/v5loader.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)    11030 2023-07-02 16:29:22.000000 PJYoloVision-0.0.0/PJYoloVision/yolo/data/dataset.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     1359 2023-07-02 16:13:08.000000 PJYoloVision-0.0.0/PJYoloVision/yolo/data/dataset_wrappers.py
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-02 16:30:31.380324 PJYoloVision-0.0.0/PJYoloVision/yolo/data/scripts/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)        0 2023-07-02 16:13:08.000000 PJYoloVision-0.0.0/PJYoloVision/yolo/data/scripts/__init__.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)    18817 2023-07-02 16:29:22.000000 PJYoloVision-0.0.0/PJYoloVision/yolo/data/utils.py
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-02 16:30:31.380324 PJYoloVision-0.0.0/PJYoloVision/yolo/utils/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)    17619 2023-07-02 16:29:22.000000 PJYoloVision-0.0.0/PJYoloVision/yolo/utils/__init__.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     3175 2023-07-02 16:29:22.000000 PJYoloVision-0.0.0/PJYoloVision/yolo/utils/autobatch.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     4043 2023-07-02 16:29:22.000000 PJYoloVision-0.0.0/PJYoloVision/yolo/utils/benchmarks.py
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-02 16:30:31.380324 PJYoloVision-0.0.0/PJYoloVision/yolo/utils/callbacks/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)      123 2023-07-02 16:13:08.000000 PJYoloVision-0.0.0/PJYoloVision/yolo/utils/callbacks/__init__.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     3842 2023-07-02 16:13:08.000000 PJYoloVision-0.0.0/PJYoloVision/yolo/utils/callbacks/base.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     2205 2023-07-02 16:29:22.000000 PJYoloVision-0.0.0/PJYoloVision/yolo/utils/callbacks/clearml.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     2162 2023-07-02 16:29:21.000000 PJYoloVision-0.0.0/PJYoloVision/yolo/utils/callbacks/comet.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     3040 2023-07-02 16:29:21.000000 PJYoloVision-0.0.0/PJYoloVision/yolo/utils/callbacks/hub.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     1323 2023-07-02 16:29:21.000000 PJYoloVision-0.0.0/PJYoloVision/yolo/utils/callbacks/tensorboard.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     9837 2023-07-02 16:29:21.000000 PJYoloVision-0.0.0/PJYoloVision/yolo/utils/checks.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     2424 2023-07-02 16:13:08.000000 PJYoloVision-0.0.0/PJYoloVision/yolo/utils/dist.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     6474 2023-07-02 16:29:21.000000 PJYoloVision-0.0.0/PJYoloVision/yolo/utils/downloads.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     2556 2023-07-02 16:13:08.000000 PJYoloVision-0.0.0/PJYoloVision/yolo/utils/files.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)    11762 2023-07-02 16:13:08.000000 PJYoloVision-0.0.0/PJYoloVision/yolo/utils/instance.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     2326 2023-07-02 16:13:08.000000 PJYoloVision-0.0.0/PJYoloVision/yolo/utils/loss.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)    28016 2023-07-02 16:29:21.000000 PJYoloVision-0.0.0/PJYoloVision/yolo/utils/metrics.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)    19809 2023-07-02 16:29:22.000000 PJYoloVision-0.0.0/PJYoloVision/yolo/utils/ops.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)    15709 2023-07-02 16:29:22.000000 PJYoloVision-0.0.0/PJYoloVision/yolo/utils/plotting.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)    10646 2023-07-02 16:13:08.000000 PJYoloVision-0.0.0/PJYoloVision/yolo/utils/tal.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)    18671 2023-07-02 16:29:21.000000 PJYoloVision-0.0.0/PJYoloVision/yolo/utils/torch_utils.py
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-02 16:30:31.384323 PJYoloVision-0.0.0/PJYoloVision/yolo/vision/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)      122 2023-07-02 16:29:21.000000 PJYoloVision-0.0.0/PJYoloVision/yolo/vision/__init__.py
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-02 16:30:31.384323 PJYoloVision-0.0.0/PJYoloVision/yolo/vision/classify/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)      318 2023-07-02 16:29:22.000000 PJYoloVision-0.0.0/PJYoloVision/yolo/vision/classify/__init__.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     2649 2023-07-02 16:29:21.000000 PJYoloVision-0.0.0/PJYoloVision/yolo/vision/classify/predict.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     5479 2023-07-02 16:29:21.000000 PJYoloVision-0.0.0/PJYoloVision/yolo/vision/classify/train.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     2237 2023-07-02 16:29:21.000000 PJYoloVision-0.0.0/PJYoloVision/yolo/vision/classify/val.py
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-02 16:30:31.384323 PJYoloVision-0.0.0/PJYoloVision/yolo/vision/detection/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)      190 2023-07-02 16:13:08.000000 PJYoloVision-0.0.0/PJYoloVision/yolo/vision/detection/__init__.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     4193 2023-07-02 16:29:22.000000 PJYoloVision-0.0.0/PJYoloVision/yolo/vision/detection/predict.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     8474 2023-07-02 16:29:22.000000 PJYoloVision-0.0.0/PJYoloVision/yolo/vision/detection/train.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)    11661 2023-07-02 16:29:21.000000 PJYoloVision-0.0.0/PJYoloVision/yolo/vision/detection/val.py
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-02 16:30:31.384323 PJYoloVision-0.0.0/PJYoloVision/yolo/vision/segmentation/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)      208 2023-07-02 16:13:08.000000 PJYoloVision-0.0.0/PJYoloVision/yolo/vision/segmentation/__init__.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     4940 2023-07-02 16:29:21.000000 PJYoloVision-0.0.0/PJYoloVision/yolo/vision/segmentation/predict.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     7299 2023-07-02 16:29:22.000000 PJYoloVision-0.0.0/PJYoloVision/yolo/vision/segmentation/train.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)    12004 2023-07-02 16:29:21.000000 PJYoloVision-0.0.0/PJYoloVision/yolo/vision/segmentation/val.py
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-02 16:30:31.376323 PJYoloVision-0.0.0/PJYoloVision.egg-info/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     5384 2023-07-02 16:30:31.000000 PJYoloVision-0.0.0/PJYoloVision.egg-info/PKG-INFO
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     2906 2023-07-02 16:30:31.000000 PJYoloVision-0.0.0/PJYoloVision.egg-info/SOURCES.txt
--rw-rw-r--   0 erfan     (1000) erfan     (1000)        1 2023-07-02 16:30:31.000000 PJYoloVision-0.0.0/PJYoloVision.egg-info/dependency_links.txt
--rw-rw-r--   0 erfan     (1000) erfan     (1000)       14 2023-07-02 16:30:31.000000 PJYoloVision-0.0.0/PJYoloVision.egg-info/requires.txt
--rw-rw-r--   0 erfan     (1000) erfan     (1000)       13 2023-07-02 16:30:31.000000 PJYoloVision-0.0.0/PJYoloVision.egg-info/top_level.txt
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     5384 2023-07-02 16:30:31.384323 PJYoloVision-0.0.0/PKG-INFO
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     4441 2023-07-02 16:30:14.000000 PJYoloVision-0.0.0/README.md
--rw-rw-r--   0 erfan     (1000) erfan     (1000)      607 2023-07-02 16:19:19.000000 PJYoloVision-0.0.0/pyproject.toml
--rw-rw-r--   0 erfan     (1000) erfan     (1000)       38 2023-07-02 16:30:31.384323 PJYoloVision-0.0.0/setup.cfg
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     1495 2023-07-02 16:30:25.000000 PJYoloVision-0.0.0/setup.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-02 17:45:33.533211 PJYoloVision-0.0.1/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    35149 2023-07-02 16:13:08.000000 PJYoloVision-0.0.1/LICENCE.md
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-02 17:45:33.521211 PJYoloVision-0.0.1/PJYoloVision/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     4906 2023-07-02 16:29:21.000000 PJYoloVision-0.0.1/PJYoloVision/__init__.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-02 17:45:33.525211 PJYoloVision-0.0.1/PJYoloVision/nn/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)        0 2023-07-02 16:13:08.000000 PJYoloVision-0.0.1/PJYoloVision/nn/__init__.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     5599 2023-07-02 16:29:22.000000 PJYoloVision-0.0.1/PJYoloVision/nn/autobackend.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    10975 2023-07-02 16:29:22.000000 PJYoloVision-0.0.1/PJYoloVision/nn/autoshape.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)      867 2023-07-02 16:13:08.000000 PJYoloVision-0.0.1/PJYoloVision/nn/modules.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    17463 2023-07-02 16:29:21.000000 PJYoloVision-0.0.1/PJYoloVision/nn/tasks.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-02 17:45:33.525211 PJYoloVision-0.0.1/PJYoloVision/tracker/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)      162 2023-07-02 16:13:08.000000 PJYoloVision-0.0.1/PJYoloVision/tracker/__init__.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     1594 2023-07-02 16:29:21.000000 PJYoloVision-0.0.1/PJYoloVision/tracker/track.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-02 17:45:33.525211 PJYoloVision-0.0.1/PJYoloVision/tracker/trackers/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)      131 2023-07-02 16:13:08.000000 PJYoloVision-0.0.1/PJYoloVision/tracker/trackers/__init__.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     1085 2023-07-02 16:13:08.000000 PJYoloVision-0.0.1/PJYoloVision/tracker/trackers/basetrack.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     4858 2023-07-02 16:13:08.000000 PJYoloVision-0.0.1/PJYoloVision/tracker/trackers/bot_sort.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    13185 2023-07-02 16:13:08.000000 PJYoloVision-0.0.1/PJYoloVision/tracker/trackers/byte_tracker.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-02 17:45:33.525211 PJYoloVision-0.0.1/PJYoloVision/tracker/utils/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)        0 2023-07-02 16:13:08.000000 PJYoloVision-0.0.1/PJYoloVision/tracker/utils/__init__.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    11965 2023-07-02 16:29:21.000000 PJYoloVision-0.0.1/PJYoloVision/tracker/utils/gmc.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    18422 2023-07-02 16:13:08.000000 PJYoloVision-0.0.1/PJYoloVision/tracker/utils/kalman_filter.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     7634 2023-07-02 16:13:08.000000 PJYoloVision-0.0.1/PJYoloVision/tracker/utils/matching.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-02 17:45:33.525211 PJYoloVision-0.0.1/PJYoloVision/yolo/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)       45 2023-07-02 16:13:08.000000 PJYoloVision-0.0.1/PJYoloVision/yolo/__init__.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-02 17:45:33.525211 PJYoloVision-0.0.1/PJYoloVision/yolo/cfg/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    11774 2023-07-02 16:29:21.000000 PJYoloVision-0.0.1/PJYoloVision/yolo/cfg/__init__.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-02 17:45:33.525211 PJYoloVision-0.0.1/PJYoloVision/yolo/core/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)        0 2023-07-02 16:13:08.000000 PJYoloVision-0.0.1/PJYoloVision/yolo/core/__init__.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    35343 2023-07-02 16:29:21.000000 PJYoloVision-0.0.1/PJYoloVision/yolo/core/exporter.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     9784 2023-07-02 17:45:18.000000 PJYoloVision-0.0.1/PJYoloVision/yolo/core/model.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    13012 2023-07-02 16:29:22.000000 PJYoloVision-0.0.1/PJYoloVision/yolo/core/predictor.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    12519 2023-07-02 16:29:21.000000 PJYoloVision-0.0.1/PJYoloVision/yolo/core/results.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    29828 2023-07-02 16:29:22.000000 PJYoloVision-0.0.1/PJYoloVision/yolo/core/trainer.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     9205 2023-07-02 16:29:22.000000 PJYoloVision-0.0.1/PJYoloVision/yolo/core/validator.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-02 17:45:33.525211 PJYoloVision-0.0.1/PJYoloVision/yolo/data/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)      444 2023-07-02 16:13:08.000000 PJYoloVision-0.0.1/PJYoloVision/yolo/data/__init__.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    31854 2023-07-02 16:29:22.000000 PJYoloVision-0.0.1/PJYoloVision/yolo/data/augment.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     8963 2023-07-02 16:13:08.000000 PJYoloVision-0.0.1/PJYoloVision/yolo/data/base.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     7658 2023-07-02 16:29:21.000000 PJYoloVision-0.0.1/PJYoloVision/yolo/data/build.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-02 17:45:33.529211 PJYoloVision-0.0.1/PJYoloVision/yolo/data/dataloaders/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)        0 2023-07-02 16:13:08.000000 PJYoloVision-0.0.1/PJYoloVision/yolo/data/dataloaders/__init__.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    12613 2023-07-02 16:29:22.000000 PJYoloVision-0.0.1/PJYoloVision/yolo/data/dataloaders/stream_loaders.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    17533 2023-07-02 16:29:21.000000 PJYoloVision-0.0.1/PJYoloVision/yolo/data/dataloaders/v5augmentations.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    46519 2023-07-02 16:29:21.000000 PJYoloVision-0.0.1/PJYoloVision/yolo/data/dataloaders/v5loader.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    11030 2023-07-02 16:29:22.000000 PJYoloVision-0.0.1/PJYoloVision/yolo/data/dataset.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     1359 2023-07-02 16:13:08.000000 PJYoloVision-0.0.1/PJYoloVision/yolo/data/dataset_wrappers.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-02 17:45:33.529211 PJYoloVision-0.0.1/PJYoloVision/yolo/data/scripts/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)        0 2023-07-02 16:13:08.000000 PJYoloVision-0.0.1/PJYoloVision/yolo/data/scripts/__init__.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    18817 2023-07-02 16:29:22.000000 PJYoloVision-0.0.1/PJYoloVision/yolo/data/utils.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-02 17:45:33.529211 PJYoloVision-0.0.1/PJYoloVision/yolo/utils/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    17619 2023-07-02 16:29:22.000000 PJYoloVision-0.0.1/PJYoloVision/yolo/utils/__init__.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     3175 2023-07-02 16:29:22.000000 PJYoloVision-0.0.1/PJYoloVision/yolo/utils/autobatch.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     4043 2023-07-02 16:29:22.000000 PJYoloVision-0.0.1/PJYoloVision/yolo/utils/benchmarks.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-02 17:45:33.529211 PJYoloVision-0.0.1/PJYoloVision/yolo/utils/callbacks/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)      123 2023-07-02 16:13:08.000000 PJYoloVision-0.0.1/PJYoloVision/yolo/utils/callbacks/__init__.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     3842 2023-07-02 16:13:08.000000 PJYoloVision-0.0.1/PJYoloVision/yolo/utils/callbacks/base.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     2205 2023-07-02 16:29:22.000000 PJYoloVision-0.0.1/PJYoloVision/yolo/utils/callbacks/clearml.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     2162 2023-07-02 16:29:21.000000 PJYoloVision-0.0.1/PJYoloVision/yolo/utils/callbacks/comet.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     3040 2023-07-02 16:29:21.000000 PJYoloVision-0.0.1/PJYoloVision/yolo/utils/callbacks/hub.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     1323 2023-07-02 16:29:21.000000 PJYoloVision-0.0.1/PJYoloVision/yolo/utils/callbacks/tensorboard.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     9837 2023-07-02 16:29:21.000000 PJYoloVision-0.0.1/PJYoloVision/yolo/utils/checks.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     2424 2023-07-02 16:13:08.000000 PJYoloVision-0.0.1/PJYoloVision/yolo/utils/dist.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     6474 2023-07-02 16:29:21.000000 PJYoloVision-0.0.1/PJYoloVision/yolo/utils/downloads.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     2556 2023-07-02 16:13:08.000000 PJYoloVision-0.0.1/PJYoloVision/yolo/utils/files.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    11762 2023-07-02 16:13:08.000000 PJYoloVision-0.0.1/PJYoloVision/yolo/utils/instance.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     2326 2023-07-02 16:13:08.000000 PJYoloVision-0.0.1/PJYoloVision/yolo/utils/loss.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    28016 2023-07-02 16:29:21.000000 PJYoloVision-0.0.1/PJYoloVision/yolo/utils/metrics.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    19809 2023-07-02 16:29:22.000000 PJYoloVision-0.0.1/PJYoloVision/yolo/utils/ops.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    15709 2023-07-02 16:29:22.000000 PJYoloVision-0.0.1/PJYoloVision/yolo/utils/plotting.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    10646 2023-07-02 16:13:08.000000 PJYoloVision-0.0.1/PJYoloVision/yolo/utils/tal.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    18671 2023-07-02 16:29:21.000000 PJYoloVision-0.0.1/PJYoloVision/yolo/utils/torch_utils.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-02 17:45:33.529211 PJYoloVision-0.0.1/PJYoloVision/yolo/vision/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)      122 2023-07-02 16:29:21.000000 PJYoloVision-0.0.1/PJYoloVision/yolo/vision/__init__.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-02 17:45:33.529211 PJYoloVision-0.0.1/PJYoloVision/yolo/vision/classify/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)      318 2023-07-02 16:29:22.000000 PJYoloVision-0.0.1/PJYoloVision/yolo/vision/classify/__init__.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     2649 2023-07-02 16:29:21.000000 PJYoloVision-0.0.1/PJYoloVision/yolo/vision/classify/predict.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     5479 2023-07-02 16:29:21.000000 PJYoloVision-0.0.1/PJYoloVision/yolo/vision/classify/train.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     2237 2023-07-02 16:29:21.000000 PJYoloVision-0.0.1/PJYoloVision/yolo/vision/classify/val.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-02 17:45:33.533211 PJYoloVision-0.0.1/PJYoloVision/yolo/vision/detection/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)      190 2023-07-02 16:13:08.000000 PJYoloVision-0.0.1/PJYoloVision/yolo/vision/detection/__init__.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     4193 2023-07-02 16:29:22.000000 PJYoloVision-0.0.1/PJYoloVision/yolo/vision/detection/predict.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     8474 2023-07-02 16:29:22.000000 PJYoloVision-0.0.1/PJYoloVision/yolo/vision/detection/train.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    11661 2023-07-02 16:29:21.000000 PJYoloVision-0.0.1/PJYoloVision/yolo/vision/detection/val.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-02 17:45:33.533211 PJYoloVision-0.0.1/PJYoloVision/yolo/vision/segmentation/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)      208 2023-07-02 16:13:08.000000 PJYoloVision-0.0.1/PJYoloVision/yolo/vision/segmentation/__init__.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     4940 2023-07-02 16:29:21.000000 PJYoloVision-0.0.1/PJYoloVision/yolo/vision/segmentation/predict.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     7299 2023-07-02 16:29:22.000000 PJYoloVision-0.0.1/PJYoloVision/yolo/vision/segmentation/train.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    12004 2023-07-02 16:29:21.000000 PJYoloVision-0.0.1/PJYoloVision/yolo/vision/segmentation/val.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-07-02 17:45:33.525211 PJYoloVision-0.0.1/PJYoloVision.egg-info/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     5384 2023-07-02 17:45:33.000000 PJYoloVision-0.0.1/PJYoloVision.egg-info/PKG-INFO
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     2906 2023-07-02 17:45:33.000000 PJYoloVision-0.0.1/PJYoloVision.egg-info/SOURCES.txt
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)        1 2023-07-02 17:45:33.000000 PJYoloVision-0.0.1/PJYoloVision.egg-info/dependency_links.txt
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)       14 2023-07-02 17:45:33.000000 PJYoloVision-0.0.1/PJYoloVision.egg-info/requires.txt
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)       13 2023-07-02 17:45:33.000000 PJYoloVision-0.0.1/PJYoloVision.egg-info/top_level.txt
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     5384 2023-07-02 17:45:33.533211 PJYoloVision-0.0.1/PKG-INFO
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     4441 2023-07-02 16:30:14.000000 PJYoloVision-0.0.1/README.md
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)      607 2023-07-02 16:19:19.000000 PJYoloVision-0.0.1/pyproject.toml
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)       38 2023-07-02 17:45:33.533211 PJYoloVision-0.0.1/setup.cfg
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     1495 2023-07-02 17:45:29.000000 PJYoloVision-0.0.1/setup.py
```

### Comparing `PJYoloVision-0.0.0/LICENCE.md` & `PJYoloVision-0.0.1/LICENCE.md`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.0/PJYoloVision/__init__.py` & `PJYoloVision-0.0.1/PJYoloVision/__init__.py`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.0/PJYoloVision/nn/autobackend.py` & `PJYoloVision-0.0.1/PJYoloVision/nn/autobackend.py`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.0/PJYoloVision/nn/autoshape.py` & `PJYoloVision-0.0.1/PJYoloVision/nn/autoshape.py`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.0/PJYoloVision/nn/modules.py` & `PJYoloVision-0.0.1/PJYoloVision/nn/modules.py`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.0/PJYoloVision/nn/tasks.py` & `PJYoloVision-0.0.1/PJYoloVision/nn/tasks.py`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.0/PJYoloVision/tracker/track.py` & `PJYoloVision-0.0.1/PJYoloVision/tracker/track.py`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.0/PJYoloVision/tracker/trackers/basetrack.py` & `PJYoloVision-0.0.1/PJYoloVision/tracker/trackers/basetrack.py`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.0/PJYoloVision/tracker/trackers/bot_sort.py` & `PJYoloVision-0.0.1/PJYoloVision/tracker/trackers/bot_sort.py`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.0/PJYoloVision/tracker/trackers/byte_tracker.py` & `PJYoloVision-0.0.1/PJYoloVision/tracker/trackers/byte_tracker.py`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.0/PJYoloVision/tracker/utils/gmc.py` & `PJYoloVision-0.0.1/PJYoloVision/tracker/utils/gmc.py`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.0/PJYoloVision/tracker/utils/kalman_filter.py` & `PJYoloVision-0.0.1/PJYoloVision/tracker/utils/kalman_filter.py`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.0/PJYoloVision/tracker/utils/matching.py` & `PJYoloVision-0.0.1/PJYoloVision/tracker/utils/matching.py`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.0/PJYoloVision/yolo/cfg/__init__.py` & `PJYoloVision-0.0.1/PJYoloVision/yolo/cfg/__init__.py`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.0/PJYoloVision/yolo/core/exporter.py` & `PJYoloVision-0.0.1/PJYoloVision/yolo/core/exporter.py`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.0/PJYoloVision/yolo/core/model.py` & `PJYoloVision-0.0.1/PJYoloVision/yolo/core/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,15 +74,15 @@
         self.model.args = {k: v for k, v in args.items() if k in DEFAULT_CFG_KEYS}
         self.model.task = self.task
 
     def _load_model(self, weights: str, task=None, *args, **kwargs):
         suffix = Path(weights).suffix
         if suffix == '.pt':
             self.model, self.ckpt = attempt_load_one_weight(weights)
-            self.task = self.model.args['task']
+            self.task = task or self.model.args['train_args']['task']
             self.overrides = self.model.args = self._reset_ckpt_args(self.model.args)
             self.ckpt_path = self.model.pt_path
         else:
             weights = check_file(weights)
             self.model, self.ckpt = weights, None
             self.task = task or get_model_task_from_cfg(weights)
             self.ckpt_path = weights
```

### Comparing `PJYoloVision-0.0.0/PJYoloVision/yolo/core/predictor.py` & `PJYoloVision-0.0.1/PJYoloVision/yolo/core/predictor.py`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.0/PJYoloVision/yolo/core/results.py` & `PJYoloVision-0.0.1/PJYoloVision/yolo/core/results.py`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.0/PJYoloVision/yolo/core/trainer.py` & `PJYoloVision-0.0.1/PJYoloVision/yolo/core/trainer.py`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.0/PJYoloVision/yolo/core/validator.py` & `PJYoloVision-0.0.1/PJYoloVision/yolo/core/validator.py`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.0/PJYoloVision/yolo/data/augment.py` & `PJYoloVision-0.0.1/PJYoloVision/yolo/data/augment.py`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.0/PJYoloVision/yolo/data/base.py` & `PJYoloVision-0.0.1/PJYoloVision/yolo/data/base.py`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.0/PJYoloVision/yolo/data/build.py` & `PJYoloVision-0.0.1/PJYoloVision/yolo/data/build.py`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.0/PJYoloVision/yolo/data/dataloaders/stream_loaders.py` & `PJYoloVision-0.0.1/PJYoloVision/yolo/data/dataloaders/stream_loaders.py`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.0/PJYoloVision/yolo/data/dataloaders/v5augmentations.py` & `PJYoloVision-0.0.1/PJYoloVision/yolo/data/dataloaders/v5augmentations.py`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.0/PJYoloVision/yolo/data/dataloaders/v5loader.py` & `PJYoloVision-0.0.1/PJYoloVision/yolo/data/dataloaders/v5loader.py`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.0/PJYoloVision/yolo/data/dataset.py` & `PJYoloVision-0.0.1/PJYoloVision/yolo/data/dataset.py`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.0/PJYoloVision/yolo/data/dataset_wrappers.py` & `PJYoloVision-0.0.1/PJYoloVision/yolo/data/dataset_wrappers.py`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.0/PJYoloVision/yolo/data/utils.py` & `PJYoloVision-0.0.1/PJYoloVision/yolo/data/utils.py`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.0/PJYoloVision/yolo/utils/__init__.py` & `PJYoloVision-0.0.1/PJYoloVision/yolo/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.0/PJYoloVision/yolo/utils/autobatch.py` & `PJYoloVision-0.0.1/PJYoloVision/yolo/utils/autobatch.py`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.0/PJYoloVision/yolo/utils/benchmarks.py` & `PJYoloVision-0.0.1/PJYoloVision/yolo/utils/benchmarks.py`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.0/PJYoloVision/yolo/utils/callbacks/base.py` & `PJYoloVision-0.0.1/PJYoloVision/yolo/utils/callbacks/base.py`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.0/PJYoloVision/yolo/utils/callbacks/clearml.py` & `PJYoloVision-0.0.1/PJYoloVision/yolo/utils/callbacks/clearml.py`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.0/PJYoloVision/yolo/utils/callbacks/comet.py` & `PJYoloVision-0.0.1/PJYoloVision/yolo/utils/callbacks/comet.py`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.0/PJYoloVision/yolo/utils/callbacks/hub.py` & `PJYoloVision-0.0.1/PJYoloVision/yolo/utils/callbacks/hub.py`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.0/PJYoloVision/yolo/utils/callbacks/tensorboard.py` & `PJYoloVision-0.0.1/PJYoloVision/yolo/utils/callbacks/tensorboard.py`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.0/PJYoloVision/yolo/utils/checks.py` & `PJYoloVision-0.0.1/PJYoloVision/yolo/utils/checks.py`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.0/PJYoloVision/yolo/utils/dist.py` & `PJYoloVision-0.0.1/PJYoloVision/yolo/utils/dist.py`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.0/PJYoloVision/yolo/utils/downloads.py` & `PJYoloVision-0.0.1/PJYoloVision/yolo/utils/downloads.py`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.0/PJYoloVision/yolo/utils/files.py` & `PJYoloVision-0.0.1/PJYoloVision/yolo/utils/files.py`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.0/PJYoloVision/yolo/utils/instance.py` & `PJYoloVision-0.0.1/PJYoloVision/yolo/utils/instance.py`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.0/PJYoloVision/yolo/utils/loss.py` & `PJYoloVision-0.0.1/PJYoloVision/yolo/utils/loss.py`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.0/PJYoloVision/yolo/utils/metrics.py` & `PJYoloVision-0.0.1/PJYoloVision/yolo/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.0/PJYoloVision/yolo/utils/ops.py` & `PJYoloVision-0.0.1/PJYoloVision/yolo/utils/ops.py`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.0/PJYoloVision/yolo/utils/plotting.py` & `PJYoloVision-0.0.1/PJYoloVision/yolo/utils/plotting.py`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.0/PJYoloVision/yolo/utils/tal.py` & `PJYoloVision-0.0.1/PJYoloVision/yolo/utils/tal.py`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.0/PJYoloVision/yolo/utils/torch_utils.py` & `PJYoloVision-0.0.1/PJYoloVision/yolo/utils/torch_utils.py`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.0/PJYoloVision/yolo/vision/classify/predict.py` & `PJYoloVision-0.0.1/PJYoloVision/yolo/vision/classify/predict.py`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.0/PJYoloVision/yolo/vision/classify/train.py` & `PJYoloVision-0.0.1/PJYoloVision/yolo/vision/classify/train.py`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.0/PJYoloVision/yolo/vision/classify/val.py` & `PJYoloVision-0.0.1/PJYoloVision/yolo/vision/classify/val.py`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.0/PJYoloVision/yolo/vision/detection/predict.py` & `PJYoloVision-0.0.1/PJYoloVision/yolo/vision/detection/predict.py`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.0/PJYoloVision/yolo/vision/detection/train.py` & `PJYoloVision-0.0.1/PJYoloVision/yolo/vision/detection/train.py`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.0/PJYoloVision/yolo/vision/detection/val.py` & `PJYoloVision-0.0.1/PJYoloVision/yolo/vision/detection/val.py`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.0/PJYoloVision/yolo/vision/segmentation/predict.py` & `PJYoloVision-0.0.1/PJYoloVision/yolo/vision/segmentation/predict.py`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.0/PJYoloVision/yolo/vision/segmentation/train.py` & `PJYoloVision-0.0.1/PJYoloVision/yolo/vision/segmentation/train.py`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.0/PJYoloVision/yolo/vision/segmentation/val.py` & `PJYoloVision-0.0.1/PJYoloVision/yolo/vision/segmentation/val.py`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.0/PJYoloVision.egg-info/PKG-INFO` & `PJYoloVision-0.0.1/PJYoloVision.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PJYoloVision
-Version: 0.0.0
+Version: 0.0.1
 Summary: The object detection models in PJYoloVision can detect and locate objects in real-time images and video streams. 
 Home-page: https://github.com/erfanzar/PJYoloVision
 Author: Erfan Zare Chavoshi
 Author-email: erfanzare82@eyahoo.com
 License: UNKNOWN
 Keywords: machine learning,deep learning,pytorch
 Platform: UNKNOWN
```

### Comparing `PJYoloVision-0.0.0/PJYoloVision.egg-info/SOURCES.txt` & `PJYoloVision-0.0.1/PJYoloVision.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.0/PKG-INFO` & `PJYoloVision-0.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PJYoloVision
-Version: 0.0.0
+Version: 0.0.1
 Summary: The object detection models in PJYoloVision can detect and locate objects in real-time images and video streams. 
 Home-page: https://github.com/erfanzar/PJYoloVision
 Author: Erfan Zare Chavoshi
 Author-email: erfanzare82@eyahoo.com
 License: UNKNOWN
 Keywords: machine learning,deep learning,pytorch
 Platform: UNKNOWN
```

### Comparing `PJYoloVision-0.0.0/README.md` & `PJYoloVision-0.0.1/README.md`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.0/pyproject.toml` & `PJYoloVision-0.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `PJYoloVision-0.0.0/setup.py` & `PJYoloVision-0.0.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='PJYoloVision',
-    version='0.0.0',
+    version='0.0.1',
     author='Erfan Zare Chavoshi',
     author_email='erfanzare82@eyahoo.com',
     description="""
     The object detection models in PJYoloVision can detect and locate objects in real-time images and video streams. 
     These models can be trained to detect specific types of objects, such as cars, people, animals,
      or any other object of interest. The YOLO models are known for being fast and accurate, 
      making them a good choice for real-time applications.
```

