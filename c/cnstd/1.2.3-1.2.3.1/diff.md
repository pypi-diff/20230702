# Comparing `tmp/cnstd-1.2.3.tar.gz` & `tmp/cnstd-1.2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cnstd-1.2.3.tar", last modified: Fri Jun 30 04:27:44 2023, max compression
+gzip compressed data, was "cnstd-1.2.3.1.tar", last modified: Sat Jul  1 15:16:55 2023, max compression
```

## Comparing `cnstd-1.2.3.tar` & `cnstd-1.2.3.1.tar`

### file list

```diff
@@ -1,98 +1,98 @@
-drwxr-xr-x   0 king       (501) staff       (20)        0 2023-06-30 04:27:44.426244 cnstd-1.2.3/
--rw-r--r--   0 king       (501) staff       (20)    41980 2019-03-26 07:39:48.000000 cnstd-1.2.3/LICENSE
--rw-r--r--   0 king       (501) staff       (20)    28335 2023-06-30 04:27:44.423622 cnstd-1.2.3/PKG-INFO
--rw-r--r--   0 king       (501) staff       (20)    27254 2023-06-30 04:25:33.000000 cnstd-1.2.3/README.md
-drwxr-xr-x   0 king       (501) staff       (20)        0 2023-06-30 04:27:44.321058 cnstd-1.2.3/cnstd/
--rw-r--r--   0 king       (501) staff       (20)     1025 2022-10-07 15:02:09.000000 cnstd-1.2.3/cnstd/__init__.py
--rw-r--r--   0 king       (501) staff       (20)      896 2023-06-30 04:08:02.000000 cnstd-1.2.3/cnstd/__version__.py
--rw-r--r--   0 king       (501) staff       (20)     4891 2022-07-06 05:54:12.000000 cnstd-1.2.3/cnstd/app.py
--rw-r--r--   0 king       (501) staff       (20)    13890 2023-02-19 02:44:43.000000 cnstd-1.2.3/cnstd/cli.py
--rw-r--r--   0 king       (501) staff       (20)    10018 2023-02-11 16:08:09.000000 cnstd-1.2.3/cnstd/cn_std.py
--rw-r--r--   0 king       (501) staff       (20)     8753 2023-06-30 04:07:55.000000 cnstd-1.2.3/cnstd/consts.py
-drwxr-xr-x   0 king       (501) staff       (20)        0 2023-06-30 04:27:44.331887 cnstd-1.2.3/cnstd/datasets/
--rw-r--r--   0 king       (501) staff       (20)      916 2021-08-26 09:54:14.000000 cnstd-1.2.3/cnstd/datasets/__init__.py
--rw-r--r--   0 king       (501) staff       (20)    10658 2022-06-30 13:44:51.000000 cnstd-1.2.3/cnstd/datasets/dataset.py
--rw-r--r--   0 king       (501) staff       (20)     8936 2021-08-26 09:54:14.000000 cnstd-1.2.3/cnstd/datasets/util.py
--rw-r--r--   0 king       (501) staff       (20)    12240 2022-07-31 07:00:29.000000 cnstd-1.2.3/cnstd/detector.py
--rw-r--r--   0 king       (501) staff       (20)     7573 2021-12-05 08:15:10.000000 cnstd-1.2.3/cnstd/lr_scheduler.py
-drwxr-xr-x   0 king       (501) staff       (20)        0 2023-06-30 04:27:44.336797 cnstd-1.2.3/cnstd/model/
--rw-r--r--   0 king       (501) staff       (20)     1733 2021-08-26 09:54:14.000000 cnstd-1.2.3/cnstd/model/__init__.py
--rw-r--r--   0 king       (501) staff       (20)    15884 2021-08-26 09:54:14.000000 cnstd-1.2.3/cnstd/model/base.py
--rw-r--r--   0 king       (501) staff       (20)    10382 2022-07-05 04:55:42.000000 cnstd-1.2.3/cnstd/model/core.py
--rw-r--r--   0 king       (501) staff       (20)    10061 2021-12-05 08:14:50.000000 cnstd-1.2.3/cnstd/model/dbnet.py
--rw-r--r--   0 king       (501) staff       (20)     4061 2021-12-05 08:14:50.000000 cnstd-1.2.3/cnstd/model/fpn.py
-drwxr-xr-x   0 king       (501) staff       (20)        0 2023-06-30 04:27:44.350460 cnstd-1.2.3/cnstd/ppocr/
--rw-r--r--   0 king       (501) staff       (20)     1070 2022-07-02 11:56:46.000000 cnstd-1.2.3/cnstd/ppocr/__init__.py
--rwxr-xr-x   0 king       (501) staff       (20)     7586 2023-02-11 13:26:35.000000 cnstd-1.2.3/cnstd/ppocr/angle_classifier.py
--rw-r--r--   0 king       (501) staff       (20)     1192 2022-07-01 02:57:56.000000 cnstd-1.2.3/cnstd/ppocr/consts.py
--rw-r--r--   0 king       (501) staff       (20)    14517 2022-07-06 02:43:04.000000 cnstd-1.2.3/cnstd/ppocr/img_operators.py
--rw-r--r--   0 king       (501) staff       (20)     1856 2022-07-02 11:57:35.000000 cnstd-1.2.3/cnstd/ppocr/opt_utils.py
-drwxr-xr-x   0 king       (501) staff       (20)        0 2023-06-30 04:27:44.360363 cnstd-1.2.3/cnstd/ppocr/postprocess/
--rw-r--r--   0 king       (501) staff       (20)     1636 2022-07-02 11:55:21.000000 cnstd-1.2.3/cnstd/ppocr/postprocess/__init__.py
--rw-r--r--   0 king       (501) staff       (20)     1522 2022-07-02 11:55:40.000000 cnstd-1.2.3/cnstd/ppocr/postprocess/cls_postprocess.py
--rwxr-xr-x   0 king       (501) staff       (20)     8091 2022-07-05 02:34:41.000000 cnstd-1.2.3/cnstd/ppocr/postprocess/db_postprocess.py
--rwxr-xr-x   0 king       (501) staff       (20)     5103 2022-05-27 13:20:26.000000 cnstd-1.2.3/cnstd/ppocr/postprocess/east_postprocess.py
--rw-r--r--   0 king       (501) staff       (20)     5034 2022-05-02 05:59:45.000000 cnstd-1.2.3/cnstd/ppocr/postprocess/locality_aware_nms.py
--rw-r--r--   0 king       (501) staff       (20)     1813 2022-05-02 05:59:45.000000 cnstd-1.2.3/cnstd/ppocr/postprocess/pg_postprocess.py
-drwxr-xr-x   0 king       (501) staff       (20)        0 2023-06-30 04:27:44.364259 cnstd-1.2.3/cnstd/ppocr/postprocess/pse_postprocess/
--rw-r--r--   0 king       (501) staff       (20)      654 2022-05-02 05:59:45.000000 cnstd-1.2.3/cnstd/ppocr/postprocess/pse_postprocess/__init__.py
-drwxr-xr-x   0 king       (501) staff       (20)        0 2023-06-30 04:27:44.366442 cnstd-1.2.3/cnstd/ppocr/postprocess/pse_postprocess/pse/
--rw-r--r--   0 king       (501) staff       (20)     1145 2022-05-02 05:59:45.000000 cnstd-1.2.3/cnstd/ppocr/postprocess/pse_postprocess/pse/__init__.py
--rw-r--r--   0 king       (501) staff       (20)      326 2022-05-02 05:59:45.000000 cnstd-1.2.3/cnstd/ppocr/postprocess/pse_postprocess/pse/setup.py
--rwxr-xr-x   0 king       (501) staff       (20)     4047 2022-05-02 05:59:45.000000 cnstd-1.2.3/cnstd/ppocr/postprocess/pse_postprocess/pse_postprocess.py
--rw-r--r--   0 king       (501) staff       (20)    25211 2022-05-15 09:38:05.000000 cnstd-1.2.3/cnstd/ppocr/postprocess/rec_postprocess.py
--rwxr-xr-x   0 king       (501) staff       (20)    13673 2022-05-15 09:49:29.000000 cnstd-1.2.3/cnstd/ppocr/postprocess/sast_postprocess.py
--rwxr-xr-x   0 king       (501) staff       (20)    11632 2023-02-18 14:58:36.000000 cnstd-1.2.3/cnstd/ppocr/pp_detector.py
--rwxr-xr-x   0 king       (501) staff       (20)    17083 2022-05-15 10:20:14.000000 cnstd-1.2.3/cnstd/ppocr/predict_rec.py
--rwxr-xr-x   0 king       (501) staff       (20)     8506 2022-07-02 10:58:02.000000 cnstd-1.2.3/cnstd/ppocr/predict_system.py
--rw-r--r--   0 king       (501) staff       (20)    18824 2022-07-06 03:52:50.000000 cnstd-1.2.3/cnstd/ppocr/utility.py
--rw-r--r--   0 king       (501) staff       (20)     8872 2021-12-05 08:14:50.000000 cnstd-1.2.3/cnstd/trainer.py
-drwxr-xr-x   0 king       (501) staff       (20)        0 2023-06-30 04:27:44.372243 cnstd-1.2.3/cnstd/transforms/
--rw-r--r--   0 king       (501) staff       (20)     1009 2021-12-05 08:14:50.000000 cnstd-1.2.3/cnstd/transforms/__init__.py
--rw-r--r--   0 king       (501) staff       (20)     4029 2021-08-26 09:54:14.000000 cnstd-1.2.3/cnstd/transforms/base.py
--rw-r--r--   0 king       (501) staff       (20)    11529 2021-12-05 08:14:50.000000 cnstd-1.2.3/cnstd/transforms/process_data.py
--rw-r--r--   0 king       (501) staff       (20)     2836 2021-12-05 08:14:50.000000 cnstd-1.2.3/cnstd/transforms/random_crop.py
--rw-r--r--   0 king       (501) staff       (20)     3018 2022-06-30 13:47:18.000000 cnstd-1.2.3/cnstd/transforms/resize.py
--rw-r--r--   0 king       (501) staff       (20)     4109 2021-08-26 09:54:14.000000 cnstd-1.2.3/cnstd/transforms/utils.py
-drwxr-xr-x   0 king       (501) staff       (20)        0 2023-06-30 04:27:44.383505 cnstd-1.2.3/cnstd/utils/
--rw-r--r--   0 king       (501) staff       (20)     1043 2021-08-26 09:54:14.000000 cnstd-1.2.3/cnstd/utils/__init__.py
--rw-r--r--   0 king       (501) staff       (20)     9475 2023-02-01 06:21:40.000000 cnstd-1.2.3/cnstd/utils/_utils.py
--rw-r--r--   0 king       (501) staff       (20)     1236 2021-08-26 09:54:14.000000 cnstd-1.2.3/cnstd/utils/common_types.py
--rw-r--r--   0 king       (501) staff       (20)     4329 2021-08-26 09:54:14.000000 cnstd-1.2.3/cnstd/utils/geometry.py
--rw-r--r--   0 king       (501) staff       (20)    15158 2021-08-26 09:54:14.000000 cnstd-1.2.3/cnstd/utils/metrics.py
--rw-r--r--   0 king       (501) staff       (20)     2649 2021-08-26 09:54:14.000000 cnstd-1.2.3/cnstd/utils/repr.py
--rw-r--r--   0 king       (501) staff       (20)    15834 2023-06-30 02:47:39.000000 cnstd-1.2.3/cnstd/utils/utils.py
-drwxr-xr-x   0 king       (501) staff       (20)        0 2023-06-30 04:27:44.406919 cnstd-1.2.3/cnstd/yolov7/
--rw-r--r--   0 king       (501) staff       (20)      869 2022-10-06 08:11:18.000000 cnstd-1.2.3/cnstd/yolov7/__init__.py
--rw-r--r--   0 king       (501) staff       (20)     8109 2022-10-06 08:12:51.000000 cnstd-1.2.3/cnstd/yolov7/autoanchor.py
--rw-r--r--   0 king       (501) staff       (20)    85336 2022-10-06 08:12:58.000000 cnstd-1.2.3/cnstd/yolov7/common.py
--rw-r--r--   0 king       (501) staff       (20)     1300 2022-12-18 14:43:12.000000 cnstd-1.2.3/cnstd/yolov7/consts.py
--rw-r--r--   0 king       (501) staff       (20)    57174 2023-02-01 06:27:41.000000 cnstd-1.2.3/cnstd/yolov7/datasets.py
--rw-r--r--   0 king       (501) staff       (20)    11822 2022-10-06 08:14:21.000000 cnstd-1.2.3/cnstd/yolov7/experimental.py
--rw-r--r--   0 king       (501) staff       (20)    38670 2022-12-18 15:04:18.000000 cnstd-1.2.3/cnstd/yolov7/general.py
--rw-r--r--   0 king       (501) staff       (20)    13911 2023-02-19 02:09:32.000000 cnstd-1.2.3/cnstd/yolov7/layout_analyzer.py
--rw-r--r--   0 king       (501) staff       (20)    75901 2022-10-06 08:14:45.000000 cnstd-1.2.3/cnstd/yolov7/loss.py
--rw-r--r--   0 king       (501) staff       (20)    10277 2022-10-06 08:14:45.000000 cnstd-1.2.3/cnstd/yolov7/metrics.py
--rw-r--r--   0 king       (501) staff       (20)    22030 2022-10-13 04:28:33.000000 cnstd-1.2.3/cnstd/yolov7/plots.py
--rw-r--r--   0 king       (501) staff       (20)    16420 2022-12-18 14:21:22.000000 cnstd-1.2.3/cnstd/yolov7/torch_utils.py
--rw-r--r--   0 king       (501) staff       (20)    40992 2022-10-06 08:15:08.000000 cnstd-1.2.3/cnstd/yolov7/yolo.py
--rw-r--r--   0 king       (501) staff       (20)     5010 2023-02-08 07:45:10.000000 cnstd-1.2.3/cnstd/yolov7/yolov7-mfd.yaml
--rw-r--r--   0 king       (501) staff       (20)     5586 2022-10-06 08:15:22.000000 cnstd-1.2.3/cnstd/yolov7/yolov7-tiny-layout.yaml
--rw-r--r--   0 king       (501) staff       (20)     5630 2022-12-18 13:53:41.000000 cnstd-1.2.3/cnstd/yolov7/yolov7-tiny-mfd.yaml
-drwxr-xr-x   0 king       (501) staff       (20)        0 2023-06-30 04:27:44.326361 cnstd-1.2.3/cnstd.egg-info/
--rw-r--r--   0 king       (501) staff       (20)    28335 2023-06-30 04:27:44.000000 cnstd-1.2.3/cnstd.egg-info/PKG-INFO
--rw-r--r--   0 king       (501) staff       (20)     2256 2023-06-30 04:27:44.000000 cnstd-1.2.3/cnstd.egg-info/SOURCES.txt
--rw-r--r--   0 king       (501) staff       (20)        1 2023-06-30 04:27:44.000000 cnstd-1.2.3/cnstd.egg-info/dependency_links.txt
--rw-r--r--   0 king       (501) staff       (20)       40 2023-06-30 04:27:44.000000 cnstd-1.2.3/cnstd.egg-info/entry_points.txt
--rw-r--r--   0 king       (501) staff       (20)        1 2020-05-31 06:07:08.000000 cnstd-1.2.3/cnstd.egg-info/not-zip-safe
--rw-r--r--   0 king       (501) staff       (20)      235 2023-06-30 04:27:44.000000 cnstd-1.2.3/cnstd.egg-info/requires.txt
--rw-r--r--   0 king       (501) staff       (20)        6 2023-06-30 04:27:44.000000 cnstd-1.2.3/cnstd.egg-info/top_level.txt
--rw-r--r--   0 king       (501) staff       (20)       38 2023-06-30 04:27:44.426751 cnstd-1.2.3/setup.cfg
--rw-r--r--   0 king       (501) staff       (20)     3317 2023-06-30 04:04:58.000000 cnstd-1.2.3/setup.py
-drwxr-xr-x   0 king       (501) staff       (20)        0 2023-06-30 04:27:44.418166 cnstd-1.2.3/tests/
--rw-r--r--   0 king       (501) staff       (20)     1046 2022-07-06 06:05:27.000000 cnstd-1.2.3/tests/test_cnstd.py
--rw-r--r--   0 king       (501) staff       (20)     1411 2021-12-05 08:14:50.000000 cnstd-1.2.3/tests/test_lr_schedulers.py
--rw-r--r--   0 king       (501) staff       (20)      986 2021-12-05 08:14:50.000000 cnstd-1.2.3/tests/test_models.py
--rw-r--r--   0 king       (501) staff       (20)      910 2021-08-26 09:54:14.000000 cnstd-1.2.3/tests/test_transforms.py
--rw-r--r--   0 king       (501) staff       (20)      456 2023-02-18 14:57:29.000000 cnstd-1.2.3/tests/test_utils.py
--rw-r--r--   0 king       (501) staff       (20)      281 2022-10-07 14:46:08.000000 cnstd-1.2.3/tests/test_yolov7.py
+drwxr-xr-x   0 king       (501) staff       (20)        0 2023-07-01 15:16:55.539939 cnstd-1.2.3.1/
+-rw-r--r--   0 king       (501) staff       (20)    41980 2019-03-26 07:39:48.000000 cnstd-1.2.3.1/LICENSE
+-rw-r--r--   0 king       (501) staff       (20)    28337 2023-07-01 15:16:55.539492 cnstd-1.2.3.1/PKG-INFO
+-rw-r--r--   0 king       (501) staff       (20)    27254 2023-06-30 06:57:54.000000 cnstd-1.2.3.1/README.md
+drwxr-xr-x   0 king       (501) staff       (20)        0 2023-07-01 15:16:55.451956 cnstd-1.2.3.1/cnstd/
+-rw-r--r--   0 king       (501) staff       (20)     1025 2022-10-07 15:02:09.000000 cnstd-1.2.3.1/cnstd/__init__.py
+-rw-r--r--   0 king       (501) staff       (20)      898 2023-07-01 15:12:35.000000 cnstd-1.2.3.1/cnstd/__version__.py
+-rw-r--r--   0 king       (501) staff       (20)     4891 2022-07-06 05:54:12.000000 cnstd-1.2.3.1/cnstd/app.py
+-rw-r--r--   0 king       (501) staff       (20)    13871 2023-06-30 09:57:38.000000 cnstd-1.2.3.1/cnstd/cli.py
+-rw-r--r--   0 king       (501) staff       (20)    10018 2023-02-11 16:08:09.000000 cnstd-1.2.3.1/cnstd/cn_std.py
+-rw-r--r--   0 king       (501) staff       (20)     8753 2023-06-30 04:07:55.000000 cnstd-1.2.3.1/cnstd/consts.py
+drwxr-xr-x   0 king       (501) staff       (20)        0 2023-07-01 15:16:55.465232 cnstd-1.2.3.1/cnstd/datasets/
+-rw-r--r--   0 king       (501) staff       (20)      916 2021-08-26 09:54:14.000000 cnstd-1.2.3.1/cnstd/datasets/__init__.py
+-rw-r--r--   0 king       (501) staff       (20)    10658 2022-06-30 13:44:51.000000 cnstd-1.2.3.1/cnstd/datasets/dataset.py
+-rw-r--r--   0 king       (501) staff       (20)     8936 2021-08-26 09:54:14.000000 cnstd-1.2.3.1/cnstd/datasets/util.py
+-rw-r--r--   0 king       (501) staff       (20)    12240 2022-07-31 07:00:29.000000 cnstd-1.2.3.1/cnstd/detector.py
+-rw-r--r--   0 king       (501) staff       (20)     7573 2021-12-05 08:15:10.000000 cnstd-1.2.3.1/cnstd/lr_scheduler.py
+drwxr-xr-x   0 king       (501) staff       (20)        0 2023-07-01 15:16:55.470325 cnstd-1.2.3.1/cnstd/model/
+-rw-r--r--   0 king       (501) staff       (20)     1733 2021-08-26 09:54:14.000000 cnstd-1.2.3.1/cnstd/model/__init__.py
+-rw-r--r--   0 king       (501) staff       (20)    15884 2023-06-30 10:13:21.000000 cnstd-1.2.3.1/cnstd/model/base.py
+-rw-r--r--   0 king       (501) staff       (20)    10519 2023-06-30 10:27:24.000000 cnstd-1.2.3.1/cnstd/model/core.py
+-rw-r--r--   0 king       (501) staff       (20)    10061 2021-12-05 08:14:50.000000 cnstd-1.2.3.1/cnstd/model/dbnet.py
+-rw-r--r--   0 king       (501) staff       (20)     4061 2021-12-05 08:14:50.000000 cnstd-1.2.3.1/cnstd/model/fpn.py
+drwxr-xr-x   0 king       (501) staff       (20)        0 2023-07-01 15:16:55.478216 cnstd-1.2.3.1/cnstd/ppocr/
+-rw-r--r--   0 king       (501) staff       (20)     1070 2022-07-02 11:56:46.000000 cnstd-1.2.3.1/cnstd/ppocr/__init__.py
+-rwxr-xr-x   0 king       (501) staff       (20)     7586 2023-02-11 13:26:35.000000 cnstd-1.2.3.1/cnstd/ppocr/angle_classifier.py
+-rw-r--r--   0 king       (501) staff       (20)     1192 2022-07-01 02:57:56.000000 cnstd-1.2.3.1/cnstd/ppocr/consts.py
+-rw-r--r--   0 king       (501) staff       (20)    14517 2022-07-06 02:43:04.000000 cnstd-1.2.3.1/cnstd/ppocr/img_operators.py
+-rw-r--r--   0 king       (501) staff       (20)     1856 2022-07-02 11:57:35.000000 cnstd-1.2.3.1/cnstd/ppocr/opt_utils.py
+drwxr-xr-x   0 king       (501) staff       (20)        0 2023-07-01 15:16:55.491681 cnstd-1.2.3.1/cnstd/ppocr/postprocess/
+-rw-r--r--   0 king       (501) staff       (20)     1636 2022-07-02 11:55:21.000000 cnstd-1.2.3.1/cnstd/ppocr/postprocess/__init__.py
+-rw-r--r--   0 king       (501) staff       (20)     1522 2022-07-02 11:55:40.000000 cnstd-1.2.3.1/cnstd/ppocr/postprocess/cls_postprocess.py
+-rwxr-xr-x   0 king       (501) staff       (20)     8091 2022-07-05 02:34:41.000000 cnstd-1.2.3.1/cnstd/ppocr/postprocess/db_postprocess.py
+-rwxr-xr-x   0 king       (501) staff       (20)     5103 2022-05-27 13:20:26.000000 cnstd-1.2.3.1/cnstd/ppocr/postprocess/east_postprocess.py
+-rw-r--r--   0 king       (501) staff       (20)     5034 2022-05-02 05:59:45.000000 cnstd-1.2.3.1/cnstd/ppocr/postprocess/locality_aware_nms.py
+-rw-r--r--   0 king       (501) staff       (20)     1813 2022-05-02 05:59:45.000000 cnstd-1.2.3.1/cnstd/ppocr/postprocess/pg_postprocess.py
+drwxr-xr-x   0 king       (501) staff       (20)        0 2023-07-01 15:16:55.494065 cnstd-1.2.3.1/cnstd/ppocr/postprocess/pse_postprocess/
+-rw-r--r--   0 king       (501) staff       (20)      654 2022-05-02 05:59:45.000000 cnstd-1.2.3.1/cnstd/ppocr/postprocess/pse_postprocess/__init__.py
+drwxr-xr-x   0 king       (501) staff       (20)        0 2023-07-01 15:16:55.496077 cnstd-1.2.3.1/cnstd/ppocr/postprocess/pse_postprocess/pse/
+-rw-r--r--   0 king       (501) staff       (20)     1145 2022-05-02 05:59:45.000000 cnstd-1.2.3.1/cnstd/ppocr/postprocess/pse_postprocess/pse/__init__.py
+-rw-r--r--   0 king       (501) staff       (20)      326 2022-05-02 05:59:45.000000 cnstd-1.2.3.1/cnstd/ppocr/postprocess/pse_postprocess/pse/setup.py
+-rwxr-xr-x   0 king       (501) staff       (20)     4047 2022-05-02 05:59:45.000000 cnstd-1.2.3.1/cnstd/ppocr/postprocess/pse_postprocess/pse_postprocess.py
+-rw-r--r--   0 king       (501) staff       (20)    25211 2022-05-15 09:38:05.000000 cnstd-1.2.3.1/cnstd/ppocr/postprocess/rec_postprocess.py
+-rwxr-xr-x   0 king       (501) staff       (20)    13673 2022-05-15 09:49:29.000000 cnstd-1.2.3.1/cnstd/ppocr/postprocess/sast_postprocess.py
+-rwxr-xr-x   0 king       (501) staff       (20)    11632 2023-02-18 14:58:36.000000 cnstd-1.2.3.1/cnstd/ppocr/pp_detector.py
+-rwxr-xr-x   0 king       (501) staff       (20)    17083 2022-05-15 10:20:14.000000 cnstd-1.2.3.1/cnstd/ppocr/predict_rec.py
+-rwxr-xr-x   0 king       (501) staff       (20)     8506 2022-07-02 10:58:02.000000 cnstd-1.2.3.1/cnstd/ppocr/predict_system.py
+-rw-r--r--   0 king       (501) staff       (20)    18824 2022-07-06 03:52:50.000000 cnstd-1.2.3.1/cnstd/ppocr/utility.py
+-rw-r--r--   0 king       (501) staff       (20)     8872 2021-12-05 08:14:50.000000 cnstd-1.2.3.1/cnstd/trainer.py
+drwxr-xr-x   0 king       (501) staff       (20)        0 2023-07-01 15:16:55.502529 cnstd-1.2.3.1/cnstd/transforms/
+-rw-r--r--   0 king       (501) staff       (20)     1009 2021-12-05 08:14:50.000000 cnstd-1.2.3.1/cnstd/transforms/__init__.py
+-rw-r--r--   0 king       (501) staff       (20)     4029 2021-08-26 09:54:14.000000 cnstd-1.2.3.1/cnstd/transforms/base.py
+-rw-r--r--   0 king       (501) staff       (20)    11529 2021-12-05 08:14:50.000000 cnstd-1.2.3.1/cnstd/transforms/process_data.py
+-rw-r--r--   0 king       (501) staff       (20)     2836 2021-12-05 08:14:50.000000 cnstd-1.2.3.1/cnstd/transforms/random_crop.py
+-rw-r--r--   0 king       (501) staff       (20)     3018 2022-06-30 13:47:18.000000 cnstd-1.2.3.1/cnstd/transforms/resize.py
+-rw-r--r--   0 king       (501) staff       (20)     4109 2021-08-26 09:54:14.000000 cnstd-1.2.3.1/cnstd/transforms/utils.py
+drwxr-xr-x   0 king       (501) staff       (20)        0 2023-07-01 15:16:55.508393 cnstd-1.2.3.1/cnstd/utils/
+-rw-r--r--   0 king       (501) staff       (20)     1043 2021-08-26 09:54:14.000000 cnstd-1.2.3.1/cnstd/utils/__init__.py
+-rw-r--r--   0 king       (501) staff       (20)     9475 2023-06-30 10:13:05.000000 cnstd-1.2.3.1/cnstd/utils/_utils.py
+-rw-r--r--   0 king       (501) staff       (20)     1236 2021-08-26 09:54:14.000000 cnstd-1.2.3.1/cnstd/utils/common_types.py
+-rw-r--r--   0 king       (501) staff       (20)     4329 2021-08-26 09:54:14.000000 cnstd-1.2.3.1/cnstd/utils/geometry.py
+-rw-r--r--   0 king       (501) staff       (20)    15158 2021-08-26 09:54:14.000000 cnstd-1.2.3.1/cnstd/utils/metrics.py
+-rw-r--r--   0 king       (501) staff       (20)     2649 2021-08-26 09:54:14.000000 cnstd-1.2.3.1/cnstd/utils/repr.py
+-rw-r--r--   0 king       (501) staff       (20)    15834 2023-06-30 02:47:39.000000 cnstd-1.2.3.1/cnstd/utils/utils.py
+drwxr-xr-x   0 king       (501) staff       (20)        0 2023-07-01 15:16:55.533582 cnstd-1.2.3.1/cnstd/yolov7/
+-rw-r--r--   0 king       (501) staff       (20)      869 2022-10-06 08:11:18.000000 cnstd-1.2.3.1/cnstd/yolov7/__init__.py
+-rw-r--r--   0 king       (501) staff       (20)     8109 2022-10-06 08:12:51.000000 cnstd-1.2.3.1/cnstd/yolov7/autoanchor.py
+-rw-r--r--   0 king       (501) staff       (20)    85336 2022-10-06 08:12:58.000000 cnstd-1.2.3.1/cnstd/yolov7/common.py
+-rw-r--r--   0 king       (501) staff       (20)     1300 2022-12-18 14:43:12.000000 cnstd-1.2.3.1/cnstd/yolov7/consts.py
+-rw-r--r--   0 king       (501) staff       (20)    57174 2023-02-01 06:27:41.000000 cnstd-1.2.3.1/cnstd/yolov7/datasets.py
+-rw-r--r--   0 king       (501) staff       (20)    11822 2022-10-06 08:14:21.000000 cnstd-1.2.3.1/cnstd/yolov7/experimental.py
+-rw-r--r--   0 king       (501) staff       (20)    38670 2022-12-18 15:04:18.000000 cnstd-1.2.3.1/cnstd/yolov7/general.py
+-rw-r--r--   0 king       (501) staff       (20)    13911 2023-02-19 02:09:32.000000 cnstd-1.2.3.1/cnstd/yolov7/layout_analyzer.py
+-rw-r--r--   0 king       (501) staff       (20)    75901 2022-10-06 08:14:45.000000 cnstd-1.2.3.1/cnstd/yolov7/loss.py
+-rw-r--r--   0 king       (501) staff       (20)    10277 2022-10-06 08:14:45.000000 cnstd-1.2.3.1/cnstd/yolov7/metrics.py
+-rw-r--r--   0 king       (501) staff       (20)    22030 2022-10-13 04:28:33.000000 cnstd-1.2.3.1/cnstd/yolov7/plots.py
+-rw-r--r--   0 king       (501) staff       (20)    16420 2022-12-18 14:21:22.000000 cnstd-1.2.3.1/cnstd/yolov7/torch_utils.py
+-rw-r--r--   0 king       (501) staff       (20)    40992 2022-10-06 08:15:08.000000 cnstd-1.2.3.1/cnstd/yolov7/yolo.py
+-rw-r--r--   0 king       (501) staff       (20)     5010 2023-02-08 07:45:10.000000 cnstd-1.2.3.1/cnstd/yolov7/yolov7-mfd.yaml
+-rw-r--r--   0 king       (501) staff       (20)     5586 2022-10-06 08:15:22.000000 cnstd-1.2.3.1/cnstd/yolov7/yolov7-tiny-layout.yaml
+-rw-r--r--   0 king       (501) staff       (20)     5630 2022-12-18 13:53:41.000000 cnstd-1.2.3.1/cnstd/yolov7/yolov7-tiny-mfd.yaml
+drwxr-xr-x   0 king       (501) staff       (20)        0 2023-07-01 15:16:55.462370 cnstd-1.2.3.1/cnstd.egg-info/
+-rw-r--r--   0 king       (501) staff       (20)    28337 2023-07-01 15:16:55.000000 cnstd-1.2.3.1/cnstd.egg-info/PKG-INFO
+-rw-r--r--   0 king       (501) staff       (20)     2256 2023-07-01 15:16:55.000000 cnstd-1.2.3.1/cnstd.egg-info/SOURCES.txt
+-rw-r--r--   0 king       (501) staff       (20)        1 2023-07-01 15:16:55.000000 cnstd-1.2.3.1/cnstd.egg-info/dependency_links.txt
+-rw-r--r--   0 king       (501) staff       (20)       40 2023-07-01 15:16:55.000000 cnstd-1.2.3.1/cnstd.egg-info/entry_points.txt
+-rw-r--r--   0 king       (501) staff       (20)        1 2020-05-31 06:07:08.000000 cnstd-1.2.3.1/cnstd.egg-info/not-zip-safe
+-rw-r--r--   0 king       (501) staff       (20)      235 2023-07-01 15:16:55.000000 cnstd-1.2.3.1/cnstd.egg-info/requires.txt
+-rw-r--r--   0 king       (501) staff       (20)        6 2023-07-01 15:16:55.000000 cnstd-1.2.3.1/cnstd.egg-info/top_level.txt
+-rw-r--r--   0 king       (501) staff       (20)       38 2023-07-01 15:16:55.540143 cnstd-1.2.3.1/setup.cfg
+-rw-r--r--   0 king       (501) staff       (20)     3317 2023-06-30 04:04:58.000000 cnstd-1.2.3.1/setup.py
+drwxr-xr-x   0 king       (501) staff       (20)        0 2023-07-01 15:16:55.538064 cnstd-1.2.3.1/tests/
+-rw-r--r--   0 king       (501) staff       (20)     1046 2022-07-06 06:05:27.000000 cnstd-1.2.3.1/tests/test_cnstd.py
+-rw-r--r--   0 king       (501) staff       (20)     1411 2021-12-05 08:14:50.000000 cnstd-1.2.3.1/tests/test_lr_schedulers.py
+-rw-r--r--   0 king       (501) staff       (20)      986 2021-12-05 08:14:50.000000 cnstd-1.2.3.1/tests/test_models.py
+-rw-r--r--   0 king       (501) staff       (20)      910 2021-08-26 09:54:14.000000 cnstd-1.2.3.1/tests/test_transforms.py
+-rw-r--r--   0 king       (501) staff       (20)      456 2023-02-18 14:57:29.000000 cnstd-1.2.3.1/tests/test_utils.py
+-rw-r--r--   0 king       (501) staff       (20)      281 2022-10-07 14:46:08.000000 cnstd-1.2.3.1/tests/test_yolov7.py
```

### Comparing `cnstd-1.2.3/LICENSE` & `cnstd-1.2.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.3/PKG-INFO` & `cnstd-1.2.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cnstd
-Version: 1.2.3
+Version: 1.2.3.1
 Summary: Python3 package for Chinese/English Scene Text Detection (STD), Mathematical Formula Detection (MFD), and Layout Analysis, with free pretrained models
 Home-page: https://github.com/breezedeus/cnstd
 Author: breezedeus
 Author-email: breezedeus@163.com
 License: Apache 2.0
 Platform: Mac
 Platform: Linux
```

### Comparing `cnstd-1.2.3/README.md` & `cnstd-1.2.3.1/README.md`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.3/cnstd/__init__.py` & `cnstd-1.2.3.1/cnstd/__init__.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.3/cnstd/__version__.py` & `cnstd-1.2.3.1/cnstd/__version__.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
-__version__ = '1.2.3'
+__version__ = '1.2.3.1'
```

### Comparing `cnstd-1.2.3/cnstd/app.py` & `cnstd-1.2.3.1/cnstd/app.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.3/cnstd/cli.py` & `cnstd-1.2.3.1/cnstd/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -194,15 +194,15 @@
     '-p',
     '--pretrained-model-fp',
     type=str,
     default=None,
     help='使用训练好的模型。默认为 `None`，表示使用系统自带的预训练模型',
 )
 @click.option(
-    "-r", "--rotated-bbox", is_flag=True, help="是否检测带角度（非水平和垂直）的文本框。默认为 `True`"
+    "-r", "--rotated-bbox", is_flag=True, help="是否检测带角度（非水平和垂直）的文本框"
 )
 @click.option(
     "--resized-shape",
     type=str,
     default='768,768',
     help='格式："height,width"; 预测时把图片resize到此大小再进行预测。两个值都需要是32的倍数。默认为 `768,768`',
 )
```

### Comparing `cnstd-1.2.3/cnstd/cn_std.py` & `cnstd-1.2.3.1/cnstd/cn_std.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.3/cnstd/consts.py` & `cnstd-1.2.3.1/cnstd/consts.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.3/cnstd/datasets/__init__.py` & `cnstd-1.2.3.1/cnstd/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.3/cnstd/datasets/dataset.py` & `cnstd-1.2.3.1/cnstd/datasets/dataset.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.3/cnstd/datasets/util.py` & `cnstd-1.2.3.1/cnstd/datasets/util.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.3/cnstd/detector.py` & `cnstd-1.2.3.1/cnstd/detector.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.3/cnstd/lr_scheduler.py` & `cnstd-1.2.3.1/cnstd/lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.3/cnstd/model/__init__.py` & `cnstd-1.2.3.1/cnstd/model/__init__.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.3/cnstd/model/base.py` & `cnstd-1.2.3.1/cnstd/model/base.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.3/cnstd/model/core.py` & `cnstd-1.2.3.1/cnstd/model/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -172,15 +172,15 @@
         """
 
         Args:
             img_list: list, which element's should be one type of Image.Image and np.ndarray.
                 For Image.Image, it should be generated from read_img;
                 For np.ndarray, it should be RGB-style, with shape [H, W, 3], scale [0, 255]
             resized_shape: tuple, [height, width], height and width after resizing original images
-            preserve_aspect_ratio: whether or not presserve aspect ratio of original images when resizing them
+            preserve_aspect_ratio: whether or not preserve aspect ratio of original images when resizing them
             min_box_size: minimal size of detected boxes; boxes with smaller height or width will be ignored
             box_score_thresh: score threshold for boxes, boxes with scores lower than this value will be ignored
             **kwargs:
 
         Returns:
 
         """
@@ -203,15 +203,17 @@
             image = image.transpose((1, 2, 0)).astype(np.uint8)  # res: [H, W, 3]
             rotated_img = np.ascontiguousarray(rotate_page(image, -angle))
 
             _scores = _boxes[:, -1].tolist()
             _boxes = _boxes[:, :-1]
             # resize back
             _boxes[:, [0, 2]] /= compress_ratio[1]
+            _boxes[:, [0, 2]] = np.clip(_boxes[:, [0, 2]], 0.0, 1.0)
             _boxes[:, [1, 3]] /= compress_ratio[0]
+            _boxes[:, [1, 3]] = np.clip(_boxes[:, [1, 3]], 0.0, 1.0)
 
             out_boxes = _boxes.copy()
             out_boxes[:, [0, 2]] *= rotated_img.shape[1]
             out_boxes[:, [1, 3]] *= rotated_img.shape[0]
 
             one_out = []
             for crop, score, box in zip(
```

### Comparing `cnstd-1.2.3/cnstd/model/dbnet.py` & `cnstd-1.2.3.1/cnstd/model/dbnet.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.3/cnstd/model/fpn.py` & `cnstd-1.2.3.1/cnstd/model/fpn.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.3/cnstd/ppocr/__init__.py` & `cnstd-1.2.3.1/cnstd/ppocr/__init__.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.3/cnstd/ppocr/angle_classifier.py` & `cnstd-1.2.3.1/cnstd/ppocr/angle_classifier.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.3/cnstd/ppocr/consts.py` & `cnstd-1.2.3.1/cnstd/ppocr/consts.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.3/cnstd/ppocr/img_operators.py` & `cnstd-1.2.3.1/cnstd/ppocr/img_operators.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.3/cnstd/ppocr/opt_utils.py` & `cnstd-1.2.3.1/cnstd/ppocr/opt_utils.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.3/cnstd/ppocr/postprocess/__init__.py` & `cnstd-1.2.3.1/cnstd/ppocr/postprocess/__init__.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.3/cnstd/ppocr/postprocess/cls_postprocess.py` & `cnstd-1.2.3.1/cnstd/ppocr/postprocess/cls_postprocess.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.3/cnstd/ppocr/postprocess/db_postprocess.py` & `cnstd-1.2.3.1/cnstd/ppocr/postprocess/db_postprocess.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.3/cnstd/ppocr/postprocess/east_postprocess.py` & `cnstd-1.2.3.1/cnstd/ppocr/postprocess/east_postprocess.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.3/cnstd/ppocr/postprocess/locality_aware_nms.py` & `cnstd-1.2.3.1/cnstd/ppocr/postprocess/locality_aware_nms.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.3/cnstd/ppocr/postprocess/pg_postprocess.py` & `cnstd-1.2.3.1/cnstd/ppocr/postprocess/pg_postprocess.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.3/cnstd/ppocr/postprocess/pse_postprocess/__init__.py` & `cnstd-1.2.3.1/cnstd/ppocr/postprocess/pse_postprocess/__init__.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.3/cnstd/ppocr/postprocess/pse_postprocess/pse/__init__.py` & `cnstd-1.2.3.1/cnstd/ppocr/postprocess/pse_postprocess/pse/__init__.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.3/cnstd/ppocr/postprocess/pse_postprocess/pse_postprocess.py` & `cnstd-1.2.3.1/cnstd/ppocr/postprocess/pse_postprocess/pse_postprocess.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.3/cnstd/ppocr/postprocess/rec_postprocess.py` & `cnstd-1.2.3.1/cnstd/ppocr/postprocess/rec_postprocess.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.3/cnstd/ppocr/postprocess/sast_postprocess.py` & `cnstd-1.2.3.1/cnstd/ppocr/postprocess/sast_postprocess.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.3/cnstd/ppocr/pp_detector.py` & `cnstd-1.2.3.1/cnstd/ppocr/pp_detector.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.3/cnstd/ppocr/predict_rec.py` & `cnstd-1.2.3.1/cnstd/ppocr/predict_rec.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.3/cnstd/ppocr/predict_system.py` & `cnstd-1.2.3.1/cnstd/ppocr/predict_system.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.3/cnstd/ppocr/utility.py` & `cnstd-1.2.3.1/cnstd/ppocr/utility.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.3/cnstd/trainer.py` & `cnstd-1.2.3.1/cnstd/trainer.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.3/cnstd/transforms/__init__.py` & `cnstd-1.2.3.1/cnstd/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.3/cnstd/transforms/base.py` & `cnstd-1.2.3.1/cnstd/transforms/base.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.3/cnstd/transforms/process_data.py` & `cnstd-1.2.3.1/cnstd/transforms/process_data.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.3/cnstd/transforms/random_crop.py` & `cnstd-1.2.3.1/cnstd/transforms/random_crop.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.3/cnstd/transforms/resize.py` & `cnstd-1.2.3.1/cnstd/transforms/resize.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.3/cnstd/transforms/utils.py` & `cnstd-1.2.3.1/cnstd/transforms/utils.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.3/cnstd/utils/__init__.py` & `cnstd-1.2.3.1/cnstd/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.3/cnstd/utils/_utils.py` & `cnstd-1.2.3.1/cnstd/utils/_utils.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.3/cnstd/utils/common_types.py` & `cnstd-1.2.3.1/cnstd/utils/common_types.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.3/cnstd/utils/geometry.py` & `cnstd-1.2.3.1/cnstd/utils/geometry.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.3/cnstd/utils/metrics.py` & `cnstd-1.2.3.1/cnstd/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.3/cnstd/utils/repr.py` & `cnstd-1.2.3.1/cnstd/utils/repr.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.3/cnstd/utils/utils.py` & `cnstd-1.2.3.1/cnstd/utils/utils.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.3/cnstd/yolov7/__init__.py` & `cnstd-1.2.3.1/cnstd/yolov7/__init__.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.3/cnstd/yolov7/autoanchor.py` & `cnstd-1.2.3.1/cnstd/yolov7/autoanchor.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.3/cnstd/yolov7/common.py` & `cnstd-1.2.3.1/cnstd/yolov7/common.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.3/cnstd/yolov7/consts.py` & `cnstd-1.2.3.1/cnstd/yolov7/consts.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.3/cnstd/yolov7/datasets.py` & `cnstd-1.2.3.1/cnstd/yolov7/datasets.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.3/cnstd/yolov7/experimental.py` & `cnstd-1.2.3.1/cnstd/yolov7/experimental.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.3/cnstd/yolov7/general.py` & `cnstd-1.2.3.1/cnstd/yolov7/general.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.3/cnstd/yolov7/layout_analyzer.py` & `cnstd-1.2.3.1/cnstd/yolov7/layout_analyzer.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.3/cnstd/yolov7/loss.py` & `cnstd-1.2.3.1/cnstd/yolov7/loss.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.3/cnstd/yolov7/metrics.py` & `cnstd-1.2.3.1/cnstd/yolov7/metrics.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.3/cnstd/yolov7/plots.py` & `cnstd-1.2.3.1/cnstd/yolov7/plots.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.3/cnstd/yolov7/torch_utils.py` & `cnstd-1.2.3.1/cnstd/yolov7/torch_utils.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.3/cnstd/yolov7/yolo.py` & `cnstd-1.2.3.1/cnstd/yolov7/yolo.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.3/cnstd/yolov7/yolov7-mfd.yaml` & `cnstd-1.2.3.1/cnstd/yolov7/yolov7-mfd.yaml`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.3/cnstd/yolov7/yolov7-tiny-layout.yaml` & `cnstd-1.2.3.1/cnstd/yolov7/yolov7-tiny-layout.yaml`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.3/cnstd/yolov7/yolov7-tiny-mfd.yaml` & `cnstd-1.2.3.1/cnstd/yolov7/yolov7-tiny-mfd.yaml`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.3/cnstd.egg-info/PKG-INFO` & `cnstd-1.2.3.1/cnstd.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cnstd
-Version: 1.2.3
+Version: 1.2.3.1
 Summary: Python3 package for Chinese/English Scene Text Detection (STD), Mathematical Formula Detection (MFD), and Layout Analysis, with free pretrained models
 Home-page: https://github.com/breezedeus/cnstd
 Author: breezedeus
 Author-email: breezedeus@163.com
 License: Apache 2.0
 Platform: Mac
 Platform: Linux
```

### Comparing `cnstd-1.2.3/cnstd.egg-info/SOURCES.txt` & `cnstd-1.2.3.1/cnstd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.3/setup.py` & `cnstd-1.2.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.3/tests/test_cnstd.py` & `cnstd-1.2.3.1/tests/test_cnstd.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.3/tests/test_lr_schedulers.py` & `cnstd-1.2.3.1/tests/test_lr_schedulers.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.3/tests/test_models.py` & `cnstd-1.2.3.1/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `cnstd-1.2.3/tests/test_transforms.py` & `cnstd-1.2.3.1/tests/test_transforms.py`

 * *Files identical despite different names*

