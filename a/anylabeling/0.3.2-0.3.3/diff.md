# Comparing `tmp/anylabeling-0.3.2.tar.gz` & `tmp/anylabeling-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anylabeling-0.3.2.tar", last modified: Thu Jun 29 01:14:47 2023, max compression
+gzip compressed data, was "anylabeling-0.3.3.tar", last modified: Sun Jul  2 04:00:12 2023, max compression
```

## Comparing `anylabeling-0.3.2.tar` & `anylabeling-0.3.3.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 01:14:47.077762 anylabeling-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-29 01:14:36.000000 anylabeling-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-29 01:14:36.000000 anylabeling-0.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4864 2023-06-29 01:14:47.077762 anylabeling-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4079 2023-06-29 01:14:36.000000 anylabeling-0.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 01:14:47.049762 anylabeling-0.3.2/anylabeling/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-29 01:14:36.000000 anylabeling-0.3.2/anylabeling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6675 2023-06-29 01:14:36.000000 anylabeling-0.3.2/anylabeling/app.py
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-29 01:14:38.000000 anylabeling-0.3.2/anylabeling/app_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-06-29 01:14:36.000000 anylabeling-0.3.2/anylabeling/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 01:14:47.053762 anylabeling-0.3.2/anylabeling/configs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 01:14:36.000000 anylabeling-0.3.2/anylabeling/configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-06-29 01:14:36.000000 anylabeling-0.3.2/anylabeling/configs/anylabeling_config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 01:14:47.053762 anylabeling-0.3.2/anylabeling/configs/auto_labeling/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 01:14:36.000000 anylabeling-0.3.2/anylabeling/configs/auto_labeling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-06-29 01:14:36.000000 anylabeling-0.3.2/anylabeling/configs/auto_labeling/models.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 01:14:47.053762 anylabeling-0.3.2/anylabeling/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 01:14:36.000000 anylabeling-0.3.2/anylabeling/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  9961730 2023-06-29 01:14:36.000000 anylabeling-0.3.2/anylabeling/resources/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 01:14:47.065762 anylabeling-0.3.2/anylabeling/services/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 01:14:36.000000 anylabeling-0.3.2/anylabeling/services/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 01:14:47.069762 anylabeling-0.3.2/anylabeling/services/auto_labeling/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 01:14:36.000000 anylabeling-0.3.2/anylabeling/services/auto_labeling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-06-29 01:14:36.000000 anylabeling-0.3.2/anylabeling/services/auto_labeling/lru_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-06-29 01:14:36.000000 anylabeling-0.3.2/anylabeling/services/auto_labeling/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    20431 2023-06-29 01:14:36.000000 anylabeling-0.3.2/anylabeling/services/auto_labeling/model_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-06-29 01:14:36.000000 anylabeling-0.3.2/anylabeling/services/auto_labeling/sam_onnx.py
--rw-r--r--   0 runner    (1001) docker     (123)     9630 2023-06-29 01:14:36.000000 anylabeling-0.3.2/anylabeling/services/auto_labeling/segment_anything.py
--rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-06-29 01:14:36.000000 anylabeling-0.3.2/anylabeling/services/auto_labeling/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     5767 2023-06-29 01:14:36.000000 anylabeling-0.3.2/anylabeling/services/auto_labeling/yolov5.py
--rw-r--r--   0 runner    (1001) docker     (123)     5527 2023-06-29 01:14:36.000000 anylabeling-0.3.2/anylabeling/services/auto_labeling/yolov8.py
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-06-29 01:14:36.000000 anylabeling-0.3.2/anylabeling/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 01:14:47.069762 anylabeling-0.3.2/anylabeling/views/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 01:14:36.000000 anylabeling-0.3.2/anylabeling/views/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 01:14:47.069762 anylabeling-0.3.2/anylabeling/views/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 01:14:36.000000 anylabeling-0.3.2/anylabeling/views/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9530 2023-06-29 01:14:36.000000 anylabeling-0.3.2/anylabeling/views/common/toaster.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 01:14:47.073762 anylabeling-0.3.2/anylabeling/views/labeling/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 01:14:36.000000 anylabeling-0.3.2/anylabeling/views/labeling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5995 2023-06-29 01:14:36.000000 anylabeling-0.3.2/anylabeling/views/labeling/label_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    97932 2023-06-29 01:14:36.000000 anylabeling-0.3.2/anylabeling/views/labeling/label_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-06-29 01:14:36.000000 anylabeling-0.3.2/anylabeling/views/labeling/label_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-06-29 01:14:36.000000 anylabeling-0.3.2/anylabeling/views/labeling/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    10828 2023-06-29 01:14:36.000000 anylabeling-0.3.2/anylabeling/views/labeling/shape.py
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-06-29 01:14:36.000000 anylabeling-0.3.2/anylabeling/views/labeling/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 01:14:47.073762 anylabeling-0.3.2/anylabeling/views/labeling/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-29 01:14:36.000000 anylabeling-0.3.2/anylabeling/views/labeling/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-29 01:14:36.000000 anylabeling-0.3.2/anylabeling/views/labeling/utils/_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-06-29 01:14:36.000000 anylabeling-0.3.2/anylabeling/views/labeling/utils/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-06-29 01:14:36.000000 anylabeling-0.3.2/anylabeling/views/labeling/utils/opencv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-06-29 01:14:36.000000 anylabeling-0.3.2/anylabeling/views/labeling/utils/qt.py
--rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-06-29 01:14:36.000000 anylabeling-0.3.2/anylabeling/views/labeling/utils/shape.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 01:14:47.077762 anylabeling-0.3.2/anylabeling/views/labeling/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-06-29 01:14:36.000000 anylabeling-0.3.2/anylabeling/views/labeling/widgets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 01:14:47.077762 anylabeling-0.3.2/anylabeling/views/labeling/widgets/auto_labeling/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-29 01:14:36.000000 anylabeling-0.3.2/anylabeling/views/labeling/widgets/auto_labeling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10796 2023-06-29 01:14:36.000000 anylabeling-0.3.2/anylabeling/views/labeling/widgets/auto_labeling/auto_labeling.py
--rw-r--r--   0 runner    (1001) docker     (123)     5302 2023-06-29 01:14:36.000000 anylabeling-0.3.2/anylabeling/views/labeling/widgets/auto_labeling/auto_labeling.ui
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-06-29 01:14:36.000000 anylabeling-0.3.2/anylabeling/views/labeling/widgets/brightness_contrast_dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)    48911 2023-06-29 01:14:36.000000 anylabeling-0.3.2/anylabeling/views/labeling/widgets/canvas.py
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-06-29 01:14:36.000000 anylabeling-0.3.2/anylabeling/views/labeling/widgets/color_dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-29 01:14:36.000000 anylabeling-0.3.2/anylabeling/views/labeling/widgets/escapable_qlist_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-06-29 01:14:36.000000 anylabeling-0.3.2/anylabeling/views/labeling/widgets/file_dialog_preview.py
--rw-r--r--   0 runner    (1001) docker     (123)     8353 2023-06-29 01:14:36.000000 anylabeling-0.3.2/anylabeling/views/labeling/widgets/label_dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)     5790 2023-06-29 01:14:36.000000 anylabeling-0.3.2/anylabeling/views/labeling/widgets/label_list_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-06-29 01:14:36.000000 anylabeling-0.3.2/anylabeling/views/labeling/widgets/toolbar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-06-29 01:14:36.000000 anylabeling-0.3.2/anylabeling/views/labeling/widgets/unique_label_qlist_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-06-29 01:14:36.000000 anylabeling-0.3.2/anylabeling/views/labeling/widgets/zoom_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-06-29 01:14:36.000000 anylabeling-0.3.2/anylabeling/views/mainwindow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 01:14:47.053762 anylabeling-0.3.2/anylabeling.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4864 2023-06-29 01:14:47.000000 anylabeling-0.3.2/anylabeling.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-06-29 01:14:47.000000 anylabeling-0.3.2/anylabeling.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 01:14:47.000000 anylabeling-0.3.2/anylabeling.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-29 01:14:47.000000 anylabeling-0.3.2/anylabeling.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-29 01:14:47.000000 anylabeling-0.3.2/anylabeling.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-29 01:14:47.000000 anylabeling-0.3.2/anylabeling.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-29 01:14:36.000000 anylabeling-0.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 01:14:47.077762 anylabeling-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-06-29 01:14:36.000000 anylabeling-0.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 04:00:12.576238 anylabeling-0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-02 04:00:01.000000 anylabeling-0.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-02 04:00:01.000000 anylabeling-0.3.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4864 2023-07-02 04:00:12.576238 anylabeling-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4079 2023-07-02 04:00:01.000000 anylabeling-0.3.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 04:00:12.560238 anylabeling-0.3.3/anylabeling/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-02 04:00:01.000000 anylabeling-0.3.3/anylabeling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6675 2023-07-02 04:00:01.000000 anylabeling-0.3.3/anylabeling/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-02 04:00:05.000000 anylabeling-0.3.3/anylabeling/app_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-07-02 04:00:01.000000 anylabeling-0.3.3/anylabeling/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 04:00:12.560238 anylabeling-0.3.3/anylabeling/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 04:00:01.000000 anylabeling-0.3.3/anylabeling/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-07-02 04:00:01.000000 anylabeling-0.3.3/anylabeling/configs/anylabeling_config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 04:00:12.560238 anylabeling-0.3.3/anylabeling/configs/auto_labeling/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 04:00:01.000000 anylabeling-0.3.3/anylabeling/configs/auto_labeling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-07-02 04:00:01.000000 anylabeling-0.3.3/anylabeling/configs/auto_labeling/models.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 04:00:12.560238 anylabeling-0.3.3/anylabeling/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 04:00:01.000000 anylabeling-0.3.3/anylabeling/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  9961730 2023-07-02 04:00:02.000000 anylabeling-0.3.3/anylabeling/resources/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 04:00:12.568238 anylabeling-0.3.3/anylabeling/services/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 04:00:02.000000 anylabeling-0.3.3/anylabeling/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 04:00:12.572239 anylabeling-0.3.3/anylabeling/services/auto_labeling/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 04:00:02.000000 anylabeling-0.3.3/anylabeling/services/auto_labeling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-07-02 04:00:02.000000 anylabeling-0.3.3/anylabeling/services/auto_labeling/lru_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-07-02 04:00:02.000000 anylabeling-0.3.3/anylabeling/services/auto_labeling/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20431 2023-07-02 04:00:02.000000 anylabeling-0.3.3/anylabeling/services/auto_labeling/model_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-07-02 04:00:02.000000 anylabeling-0.3.3/anylabeling/services/auto_labeling/sam_onnx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10088 2023-07-02 04:00:02.000000 anylabeling-0.3.3/anylabeling/services/auto_labeling/segment_anything.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-07-02 04:00:02.000000 anylabeling-0.3.3/anylabeling/services/auto_labeling/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5767 2023-07-02 04:00:02.000000 anylabeling-0.3.3/anylabeling/services/auto_labeling/yolov5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5527 2023-07-02 04:00:02.000000 anylabeling-0.3.3/anylabeling/services/auto_labeling/yolov8.py
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-07-02 04:00:02.000000 anylabeling-0.3.3/anylabeling/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 04:00:12.572239 anylabeling-0.3.3/anylabeling/views/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 04:00:02.000000 anylabeling-0.3.3/anylabeling/views/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 04:00:12.572239 anylabeling-0.3.3/anylabeling/views/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 04:00:02.000000 anylabeling-0.3.3/anylabeling/views/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9530 2023-07-02 04:00:02.000000 anylabeling-0.3.3/anylabeling/views/common/toaster.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 04:00:12.572239 anylabeling-0.3.3/anylabeling/views/labeling/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 04:00:02.000000 anylabeling-0.3.3/anylabeling/views/labeling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5995 2023-07-02 04:00:02.000000 anylabeling-0.3.3/anylabeling/views/labeling/label_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    98002 2023-07-02 04:00:02.000000 anylabeling-0.3.3/anylabeling/views/labeling/label_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-07-02 04:00:02.000000 anylabeling-0.3.3/anylabeling/views/labeling/label_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-07-02 04:00:02.000000 anylabeling-0.3.3/anylabeling/views/labeling/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10828 2023-07-02 04:00:02.000000 anylabeling-0.3.3/anylabeling/views/labeling/shape.py
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-02 04:00:02.000000 anylabeling-0.3.3/anylabeling/views/labeling/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 04:00:12.572239 anylabeling-0.3.3/anylabeling/views/labeling/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-02 04:00:02.000000 anylabeling-0.3.3/anylabeling/views/labeling/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-07-02 04:00:02.000000 anylabeling-0.3.3/anylabeling/views/labeling/utils/_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-07-02 04:00:02.000000 anylabeling-0.3.3/anylabeling/views/labeling/utils/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-07-02 04:00:02.000000 anylabeling-0.3.3/anylabeling/views/labeling/utils/opencv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-07-02 04:00:02.000000 anylabeling-0.3.3/anylabeling/views/labeling/utils/qt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-07-02 04:00:02.000000 anylabeling-0.3.3/anylabeling/views/labeling/utils/shape.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 04:00:12.576238 anylabeling-0.3.3/anylabeling/views/labeling/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-07-02 04:00:02.000000 anylabeling-0.3.3/anylabeling/views/labeling/widgets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 04:00:12.576238 anylabeling-0.3.3/anylabeling/views/labeling/widgets/auto_labeling/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-02 04:00:02.000000 anylabeling-0.3.3/anylabeling/views/labeling/widgets/auto_labeling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11660 2023-07-02 04:00:02.000000 anylabeling-0.3.3/anylabeling/views/labeling/widgets/auto_labeling/auto_labeling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5289 2023-07-02 04:00:02.000000 anylabeling-0.3.3/anylabeling/views/labeling/widgets/auto_labeling/auto_labeling.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-07-02 04:00:02.000000 anylabeling-0.3.3/anylabeling/views/labeling/widgets/brightness_contrast_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48911 2023-07-02 04:00:02.000000 anylabeling-0.3.3/anylabeling/views/labeling/widgets/canvas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-07-02 04:00:02.000000 anylabeling-0.3.3/anylabeling/views/labeling/widgets/color_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-02 04:00:02.000000 anylabeling-0.3.3/anylabeling/views/labeling/widgets/escapable_qlist_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-07-02 04:00:02.000000 anylabeling-0.3.3/anylabeling/views/labeling/widgets/file_dialog_preview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8353 2023-07-02 04:00:02.000000 anylabeling-0.3.3/anylabeling/views/labeling/widgets/label_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5790 2023-07-02 04:00:02.000000 anylabeling-0.3.3/anylabeling/views/labeling/widgets/label_list_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-07-02 04:00:02.000000 anylabeling-0.3.3/anylabeling/views/labeling/widgets/toolbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-07-02 04:00:02.000000 anylabeling-0.3.3/anylabeling/views/labeling/widgets/unique_label_qlist_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-02 04:00:02.000000 anylabeling-0.3.3/anylabeling/views/labeling/widgets/zoom_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-07-02 04:00:02.000000 anylabeling-0.3.3/anylabeling/views/mainwindow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 04:00:12.560238 anylabeling-0.3.3/anylabeling.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4864 2023-07-02 04:00:12.000000 anylabeling-0.3.3/anylabeling.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-07-02 04:00:12.000000 anylabeling-0.3.3/anylabeling.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 04:00:12.000000 anylabeling-0.3.3/anylabeling.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-02 04:00:12.000000 anylabeling-0.3.3/anylabeling.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-02 04:00:12.000000 anylabeling-0.3.3/anylabeling.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-02 04:00:12.000000 anylabeling-0.3.3/anylabeling.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-02 04:00:02.000000 anylabeling-0.3.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 04:00:12.576238 anylabeling-0.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3433 2023-07-02 04:00:02.000000 anylabeling-0.3.3/setup.py
```

### Comparing `anylabeling-0.3.2/LICENSE` & `anylabeling-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `anylabeling-0.3.2/PKG-INFO` & `anylabeling-0.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anylabeling
-Version: 0.3.2
+Version: 0.3.3
 Summary: Effortless data labeling with AI support
 Home-page: https://github.com/vietanhdev/anylabeling
 Author: Viet-Anh Nguyen
 Author-email: vietanh.dev@gmail.com
 License: GPLv3
 Keywords: Image Annotation,Machine Learning,Deep Learning
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: anylabeling Version: 0.3.2 Summary: Effortless data
+Metadata-Version: 2.1 Name: anylabeling Version: 0.3.3 Summary: Effortless data
 labeling with AI support Home-page: https://github.com/vietanhdev/anylabeling
 Author: Viet-Anh Nguyen Author-email: vietanh.dev@gmail.com License: GPLv3
 Keywords: Image Annotation,Machine Learning,Deep Learning Classifier: Intended
 Audience :: Developers Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `anylabeling-0.3.2/README.md` & `anylabeling-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `anylabeling-0.3.2/anylabeling/app.py` & `anylabeling-0.3.3/anylabeling/app.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.3.2/anylabeling/config.py` & `anylabeling-0.3.3/anylabeling/config.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.3.2/anylabeling/configs/anylabeling_config.yaml` & `anylabeling-0.3.3/anylabeling/configs/anylabeling_config.yaml`

 * *Files identical despite different names*

### Comparing `anylabeling-0.3.2/anylabeling/configs/auto_labeling/models.yaml` & `anylabeling-0.3.3/anylabeling/configs/auto_labeling/models.yaml`

 * *Files identical despite different names*

### Comparing `anylabeling-0.3.2/anylabeling/resources/resources.py` & `anylabeling-0.3.3/anylabeling/resources/resources.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.3.2/anylabeling/services/auto_labeling/lru_cache.py` & `anylabeling-0.3.3/anylabeling/services/auto_labeling/lru_cache.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.3.2/anylabeling/services/auto_labeling/model.py` & `anylabeling-0.3.3/anylabeling/services/auto_labeling/model.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.3.2/anylabeling/services/auto_labeling/model_manager.py` & `anylabeling-0.3.3/anylabeling/services/auto_labeling/model_manager.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.3.2/anylabeling/services/auto_labeling/sam_onnx.py` & `anylabeling-0.3.3/anylabeling/services/auto_labeling/sam_onnx.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.3.2/anylabeling/services/auto_labeling/segment_anything.py` & `anylabeling-0.3.3/anylabeling/services/auto_labeling/segment_anything.py`

 * *Files 3% similar despite different names*

```diff
@@ -101,26 +101,39 @@
         self.marks = marks
 
     def post_process(self, masks):
         """
         Post process masks
         """
         # Find contours
+        masks[masks > 0.0] = 255
+        masks[masks <= 0.0] = 0
+        masks = masks.astype(np.uint8)
         contours, _ = cv2.findContours(
-            masks.astype(np.uint8), cv2.RETR_EXTERNAL, cv2.CHAIN_APPROX_NONE
+            masks, cv2.RETR_EXTERNAL, cv2.CHAIN_APPROX_NONE
         )
 
         # Refine contours
         approx_contours = []
         for contour in contours:
             # Approximate contour
             epsilon = 0.001 * cv2.arcLength(contour, True)
             approx = cv2.approxPolyDP(contour, epsilon, True)
             approx_contours.append(approx)
 
+        # Remove too big contours ( >90% of image size)
+        if len(approx_contours) > 1:
+            image_size = masks.shape[0] * masks.shape[1]
+            areas = [cv2.contourArea(contour) for contour in approx_contours]
+            filtered_approx_contours = [
+                contour
+                for contour, area in zip(approx_contours, areas)
+                if area < image_size * 0.9
+            ]
+
         # Remove small contours (area < 20% of average area)
         if len(approx_contours) > 1:
             areas = [cv2.contourArea(contour) for contour in approx_contours]
             avg_area = np.mean(areas)
 
             filtered_approx_contours = [
                 contour
@@ -231,15 +244,14 @@
         result = AutoLabelingResult(shapes, replace=False)
         return result
 
     def unload(self):
         self.stop_inference = True
         if self.pre_inference_thread:
             self.pre_inference_thread.quit()
-            self.pre_inference_thread.wait()
 
     def preload_worker(self, files):
         """
         Preload next files, run inference and cache results
         """
         files = files[: self.preloaded_size]
         for filename in files:
```

### Comparing `anylabeling-0.3.2/anylabeling/services/auto_labeling/types.py` & `anylabeling-0.3.3/anylabeling/services/auto_labeling/types.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.3.2/anylabeling/services/auto_labeling/yolov5.py` & `anylabeling-0.3.3/anylabeling/services/auto_labeling/yolov5.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.3.2/anylabeling/services/auto_labeling/yolov8.py` & `anylabeling-0.3.3/anylabeling/services/auto_labeling/yolov8.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.3.2/anylabeling/views/common/toaster.py` & `anylabeling-0.3.3/anylabeling/views/common/toaster.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.3.2/anylabeling/views/labeling/label_file.py` & `anylabeling-0.3.3/anylabeling/views/labeling/label_file.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.3.2/anylabeling/views/labeling/label_widget.py` & `anylabeling-0.3.3/anylabeling/views/labeling/label_widget.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import html
 import math
 import os
 import os.path as osp
 import re
 import webbrowser
 
+import darkdetect
 import imgviz
 import natsort
 from PyQt5 import QtCore, QtGui, QtWidgets
 from PyQt5.QtCore import Qt, pyqtSlot
 from PyQt5.QtWidgets import (
     QDockWidget,
     QHBoxLayout,
@@ -120,14 +121,31 @@
             fit_to_content=self._config["fit_to_content"],
             flags=self._config["label_flags"],
         )
 
         self.label_list = LabelListWidget()
         self.last_open_dir = None
 
+        if not darkdetect.isDark():
+            dock_title_style = (
+                "QDockWidget::title {"
+                "text-align: center;"
+                "padding: 0px;"
+                "background-color: #f0f0f0;"
+                "}"
+            )
+        else:
+            dock_title_style = (
+                "QDockWidget::title {"
+                "text-align: center;"
+                "padding: 0px;"
+                "background-color: #333333;"
+                "}"
+            )
+
         self.flag_dock = self.flag_widget = None
         self.flag_dock = QtWidgets.QDockWidget(self.tr("Flags"), self)
         self.flag_dock.setObjectName("Flags")
         self.flag_widget = QtWidgets.QListWidget()
         if config["flags"]:
             self.load_flags({k: False for k in config["flags"]})
         else:
@@ -147,21 +165,15 @@
         )
         self.label_list.item_double_clicked.connect(self.edit_label)
         self.label_list.item_changed.connect(self.label_item_changed)
         self.label_list.item_dropped.connect(self.label_order_changed)
         self.shape_dock = QtWidgets.QDockWidget(self.tr("Objects"), self)
         self.shape_dock.setObjectName("Objects")
         self.shape_dock.setWidget(self.label_list)
-        self.shape_dock.setStyleSheet(
-            "QDockWidget::title {"
-            "text-align: center;"
-            "padding: 0px;"
-            "background-color: #f0f0f0;"
-            "}"
-        )
+        self.shape_dock.setStyleSheet(dock_title_style)
 
         self.unique_label_list = UniqueLabelQListWidget()
         self.unique_label_list.setToolTip(
             self.tr(
                 "Select label to start annotating for it. "
                 "Press 'Esc' to deselect."
             )
@@ -171,21 +183,15 @@
                 item = self.unique_label_list.create_item_from_label(label)
                 self.unique_label_list.addItem(item)
                 rgb = self._get_rgb_by_label(label)
                 self.unique_label_list.set_item_label(item, label, rgb)
         self.label_dock = QtWidgets.QDockWidget(self.tr("Labels"), self)
         self.label_dock.setObjectName("Labels")
         self.label_dock.setWidget(self.unique_label_list)
-        self.label_dock.setStyleSheet(
-            "QDockWidget::title {"
-            "text-align: center;"
-            "padding: 0px;"
-            "background-color: #f0f0f0;"
-            "}"
-        )
+        self.label_dock.setStyleSheet(dock_title_style)
 
         self.file_search = QtWidgets.QLineEdit()
         self.file_search.setPlaceholderText(self.tr("Search Filename"))
         self.file_search.textChanged.connect(self.file_search_changed)
         self.file_list_widget = QtWidgets.QListWidget()
         self.file_list_widget.itemSelectionChanged.connect(
             self.file_selection_changed
@@ -196,21 +202,15 @@
         file_list_layout.addWidget(self.file_search)
         file_list_layout.addWidget(self.file_list_widget)
         self.file_dock = QtWidgets.QDockWidget(self.tr("Files"), self)
         self.file_dock.setObjectName("Files")
         file_list_widget = QtWidgets.QWidget()
         file_list_widget.setLayout(file_list_layout)
         self.file_dock.setWidget(file_list_widget)
-        self.file_dock.setStyleSheet(
-            "QDockWidget::title {"
-            "text-align: center;"
-            "padding: 0px;"
-            "background-color: #f0f0f0;"
-            "}"
-        )
+        self.file_dock.setStyleSheet(dock_title_style)
 
         self.zoom_widget = ZoomWidget()
         self.setAcceptDrops(True)
 
         self.canvas = self.label_list.canvas = Canvas(
             parent=self,
             epsilon=self._config["epsilon"],
```

### Comparing `anylabeling-0.3.2/anylabeling/views/labeling/label_wrapper.py` & `anylabeling-0.3.3/anylabeling/views/labeling/label_wrapper.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.3.2/anylabeling/views/labeling/logger.py` & `anylabeling-0.3.3/anylabeling/views/labeling/logger.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.3.2/anylabeling/views/labeling/shape.py` & `anylabeling-0.3.3/anylabeling/views/labeling/shape.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.3.2/anylabeling/views/labeling/testing.py` & `anylabeling-0.3.3/anylabeling/views/labeling/testing.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.3.2/anylabeling/views/labeling/utils/_io.py` & `anylabeling-0.3.3/anylabeling/views/labeling/utils/_io.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.3.2/anylabeling/views/labeling/utils/image.py` & `anylabeling-0.3.3/anylabeling/views/labeling/utils/image.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.3.2/anylabeling/views/labeling/utils/opencv.py` & `anylabeling-0.3.3/anylabeling/views/labeling/utils/opencv.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.3.2/anylabeling/views/labeling/utils/qt.py` & `anylabeling-0.3.3/anylabeling/views/labeling/utils/qt.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.3.2/anylabeling/views/labeling/utils/shape.py` & `anylabeling-0.3.3/anylabeling/views/labeling/utils/shape.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.3.2/anylabeling/views/labeling/widgets/auto_labeling/auto_labeling.py` & `anylabeling-0.3.3/anylabeling/views/labeling/widgets/auto_labeling/auto_labeling.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import os
 
+import darkdetect
 from PyQt5 import uic
 from PyQt5.QtCore import pyqtSignal, pyqtSlot
 from PyQt5.QtWidgets import QWidget, QFileDialog
 
 from anylabeling.services.auto_labeling.model_manager import ModelManager
 from anylabeling.services.auto_labeling.types import AutoLabelingMode
 
@@ -52,14 +53,31 @@
             lambda: self.model_manager.set_output_mode(
                 self.output_select_combobox.currentData()
             )
         )
 
         self.update_model_configs(self.model_manager.get_model_configs())
 
+        # Disable tools when inference is running
+        def set_enable_tools(enable):
+            self.model_select_combobox.setEnabled(enable)
+            self.output_select_combobox.setEnabled(enable)
+            self.button_add_point.setEnabled(enable)
+            self.button_remove_point.setEnabled(enable)
+            self.button_add_rect.setEnabled(enable)
+            self.button_clear.setEnabled(enable)
+            self.button_finish_object.setEnabled(enable)
+
+        self.model_manager.prediction_started.connect(
+            lambda: set_enable_tools(False)
+        )
+        self.model_manager.prediction_finished.connect(
+            lambda: set_enable_tools(True)
+        )
+
         # Auto labeling buttons
         self.button_run.setShortcut("I")
         self.button_run.clicked.connect(self.run_prediction)
         self.button_add_point.clicked.connect(
             lambda: self.set_auto_labeling_mode(
                 AutoLabelingMode.ADD, AutoLabelingMode.POINT
             )
@@ -124,40 +142,43 @@
         style_sheet = """
             text-align: center;
             margin-right: 3px;
             border-radius: 5px;
             padding: 4px 8px;
             border: 1px solid #999999;
         """
+        normal_color = "#333333" if darkdetect.isDark() else "#ffffff"
         for button in [
             self.button_add_point,
             self.button_remove_point,
             self.button_add_rect,
             self.button_clear,
             self.button_finish_object,
         ]:
-            button.setStyleSheet(style_sheet + "background-color: #ffffff;")
+            button.setStyleSheet(
+                style_sheet + f"background-color: {normal_color};"
+            )
         if self.auto_labeling_mode == AutoLabelingMode.NONE:
             return
         if self.auto_labeling_mode.edit_mode == AutoLabelingMode.ADD:
             if self.auto_labeling_mode.shape_type == AutoLabelingMode.POINT:
                 self.button_add_point.setStyleSheet(
-                    style_sheet + "background-color: #00ff00;"
+                    style_sheet + "background-color: #00c100; color: #555555;"
                 )
             elif (
                 self.auto_labeling_mode.shape_type
                 == AutoLabelingMode.RECTANGLE
             ):
                 self.button_add_rect.setStyleSheet(
-                    style_sheet + "background-color: #00ff00;"
+                    style_sheet + "background-color: #00c100; color: #555555;"
                 )
         elif self.auto_labeling_mode.edit_mode == AutoLabelingMode.REMOVE:
             if self.auto_labeling_mode.shape_type == AutoLabelingMode.POINT:
                 self.button_remove_point.setStyleSheet(
-                    style_sheet + "background-color: #ff0000;"
+                    style_sheet + "background-color: #d30000; color: #fff;"
                 )
 
     def set_auto_labeling_mode(self, edit_mode, shape_type=None):
         """Set auto labeling mode"""
         if edit_mode is None:
             self.auto_labeling_mode = AutoLabelingMode.NONE
         else:
```

### Comparing `anylabeling-0.3.2/anylabeling/views/labeling/widgets/auto_labeling/auto_labeling.ui` & `anylabeling-0.3.3/anylabeling/views/labeling/widgets/auto_labeling/auto_labeling.ui`

 * *Files 1% similar despite different names*

#### Comparing `anylabeling-0.3.2/anylabeling/views/labeling/widgets/auto_labeling/auto_labeling.ui` & `anylabeling-0.3.3/anylabeling/views/labeling/widgets/auto_labeling/auto_labeling.ui`

```diff
@@ -187,16 +187,15 @@
             <sizepolicy hsizetype="Expanding" vsizetype="Minimum">
               <horstretch>0</horstretch>
               <verstretch>0</verstretch>
             </sizepolicy>
           </property>
           <property name="styleSheet">
             <string notr="true">margin-top: 0;
-margin-bottom: 10px;
-color: #456;</string>
+margin-bottom: 10px;</string>
           </property>
           <property name="text">
             <string>Ready!</string>
           </property>
         </widget>
       </item>
     </layout>
```

### Comparing `anylabeling-0.3.2/anylabeling/views/labeling/widgets/brightness_contrast_dialog.py` & `anylabeling-0.3.3/anylabeling/views/labeling/widgets/brightness_contrast_dialog.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.3.2/anylabeling/views/labeling/widgets/canvas.py` & `anylabeling-0.3.3/anylabeling/views/labeling/widgets/canvas.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.3.2/anylabeling/views/labeling/widgets/color_dialog.py` & `anylabeling-0.3.3/anylabeling/views/labeling/widgets/color_dialog.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.3.2/anylabeling/views/labeling/widgets/file_dialog_preview.py` & `anylabeling-0.3.3/anylabeling/views/labeling/widgets/file_dialog_preview.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.3.2/anylabeling/views/labeling/widgets/label_dialog.py` & `anylabeling-0.3.3/anylabeling/views/labeling/widgets/label_dialog.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.3.2/anylabeling/views/labeling/widgets/label_list_widget.py` & `anylabeling-0.3.3/anylabeling/views/labeling/widgets/label_list_widget.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.3.2/anylabeling/views/labeling/widgets/toolbar.py` & `anylabeling-0.3.3/anylabeling/views/labeling/widgets/toolbar.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Defines toolbar for anylabeling, including """
 
+import darkdetect
 from PyQt5 import QtCore, QtWidgets
 
 
 class ToolBar(QtWidgets.QToolBar):
     """Toolbar widget for labeling tool"""
 
     def __init__(self, title):
@@ -11,25 +12,38 @@
         layout = self.layout()
         margin = (0, 0, 0, 0)
         layout.setSpacing(0)
         layout.setContentsMargins(*margin)
         self.setContentsMargins(*margin)
         self.setWindowFlags(self.windowFlags() | QtCore.Qt.FramelessWindowHint)
 
-        self.setStyleSheet(
-            """
-            QToolBar {
-                background: #fff;
-                padding: 0px;
-                border: 0px;
-                border-radius: 5px;
-                border: 2px solid #aaa;
-            }
-            """
-        )
+        if darkdetect.isDark():
+            self.setStyleSheet(
+                """
+                QToolBar {
+                    background: #555;
+                    padding: 0px;
+                    border: 0px;
+                    border-radius: 5px;
+                    border: 2px solid #222;
+                }
+                """
+            )
+        else:
+            self.setStyleSheet(
+                """
+                QToolBar {
+                    background: #fff;
+                    padding: 0px;
+                    border: 0px;
+                    border-radius: 5px;
+                    border: 2px solid #aaa;
+                }
+                """
+            )
 
     def add_action(self, action):
         """Add an action (button) to the toolbar"""
         if isinstance(action, QtWidgets.QWidgetAction):
             return super().addAction(action)
         btn = QtWidgets.QToolButton()
         btn.setDefaultAction(action)
```

### Comparing `anylabeling-0.3.2/anylabeling/views/labeling/widgets/unique_label_qlist_widget.py` & `anylabeling-0.3.3/anylabeling/views/labeling/widgets/unique_label_qlist_widget.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.3.2/anylabeling/views/labeling/widgets/zoom_widget.py` & `anylabeling-0.3.3/anylabeling/views/labeling/widgets/zoom_widget.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.3.2/anylabeling/views/mainwindow.py` & `anylabeling-0.3.3/anylabeling/views/mainwindow.py`

 * *Files identical despite different names*

### Comparing `anylabeling-0.3.2/anylabeling.egg-info/PKG-INFO` & `anylabeling-0.3.3/anylabeling.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anylabeling
-Version: 0.3.2
+Version: 0.3.3
 Summary: Effortless data labeling with AI support
 Home-page: https://github.com/vietanhdev/anylabeling
 Author: Viet-Anh Nguyen
 Author-email: vietanh.dev@gmail.com
 License: GPLv3
 Keywords: Image Annotation,Machine Learning,Deep Learning
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: anylabeling Version: 0.3.2 Summary: Effortless data
+Metadata-Version: 2.1 Name: anylabeling Version: 0.3.3 Summary: Effortless data
 labeling with AI support Home-page: https://github.com/vietanhdev/anylabeling
 Author: Viet-Anh Nguyen Author-email: vietanh.dev@gmail.com License: GPLv3
 Keywords: Image Annotation,Machine Learning,Deep Learning Classifier: Intended
 Audience :: Developers Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `anylabeling-0.3.2/anylabeling.egg-info/SOURCES.txt` & `anylabeling-0.3.3/anylabeling.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `anylabeling-0.3.2/setup.py` & `anylabeling-0.3.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,14 +49,15 @@
         "Pillow>=2.8",
         "PyYAML",
         "termcolor",
         "opencv-python-headless",
         'PyQt5>=5.15.7; platform_system != "Darwin"',
         "onnx==1.13.1",
         "qimage2ndarray==1.10.0",
+        "darkdetect==0.8.0",
     ]
 
     # Add onnxruntime-gpu if GPU is preferred
     # otherwise, add onnxruntime.
     # Note: onnxruntime-gpu is not available on macOS
     preferred_device = get_preferred_device()
     if preferred_device == "GPU" and platform.system() != "Darwin":
```

