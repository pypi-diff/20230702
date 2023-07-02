# Comparing `tmp/depthai-sdk-1.9.4.1.tar.gz` & `tmp/depthai-sdk-1.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "depthai-sdk-1.9.4.1.tar", last modified: Fri Feb 10 11:54:17 2023, max compression
+gzip compressed data, was "depthai-sdk-1.9.5.tar", last modified: Fri Apr 21 15:19:21 2023, max compression
```

## Comparing `depthai-sdk-1.9.4.1.tar` & `depthai-sdk-1.9.5.tar`

### file list

```diff
@@ -1,160 +1,184 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 11:54:17.301599 depthai-sdk-1.9.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-02-10 11:54:06.000000 depthai-sdk-1.9.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-02-10 11:54:17.301599 depthai-sdk-1.9.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-02-10 11:54:06.000000 depthai-sdk-1.9.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-02-10 11:54:06.000000 depthai-sdk-1.9.4.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-10 11:54:17.301599 depthai-sdk-1.9.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-02-10 11:54:06.000000 depthai-sdk-1.9.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 11:54:17.285598 depthai-sdk-1.9.4.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 11:54:17.289598 depthai-sdk-1.9.4.1/src/depthai_sdk/
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-02-10 11:54:06.000000 depthai-sdk-1.9.4.1/src/depthai_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10937 2023-02-10 11:54:06.000000 depthai-sdk-1.9.4.1/src/depthai_sdk/args_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 11:54:17.293598 depthai-sdk-1.9.4.1/src/depthai_sdk/classes/
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-02-10 11:54:06.000000 depthai-sdk-1.9.4.1/src/depthai_sdk/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-02-10 11:54:06.000000 depthai-sdk-1.9.4.1/src/depthai_sdk/classes/nn_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-02-10 11:54:06.000000 depthai-sdk-1.9.4.1/src/depthai_sdk/classes/nn_results.py
--rw-r--r--   0 runner    (1001) docker     (123)     4416 2023-02-10 11:54:06.000000 depthai-sdk-1.9.4.1/src/depthai_sdk/classes/output_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7208 2023-02-10 11:54:06.000000 depthai-sdk-1.9.4.1/src/depthai_sdk/classes/packets.py
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-02-10 11:54:06.000000 depthai-sdk-1.9.4.1/src/depthai_sdk/classes/yolo_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 11:54:17.293598 depthai-sdk-1.9.4.1/src/depthai_sdk/components/
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-02-10 11:54:06.000000 depthai-sdk-1.9.4.1/src/depthai_sdk/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19566 2023-02-10 11:54:06.000000 depthai-sdk-1.9.4.1/src/depthai_sdk/components/camera_component.py
--rw-r--r--   0 runner    (1001) docker     (123)    10578 2023-02-10 11:54:06.000000 depthai-sdk-1.9.4.1/src/depthai_sdk/components/camera_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-02-10 11:54:06.000000 depthai-sdk-1.9.4.1/src/depthai_sdk/components/component.py
--rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-02-10 11:54:06.000000 depthai-sdk-1.9.4.1/src/depthai_sdk/components/imu_component.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 11:54:17.293598 depthai-sdk-1.9.4.1/src/depthai_sdk/components/integrations/
--rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-02-10 11:54:06.000000 depthai-sdk-1.9.4.1/src/depthai_sdk/components/integrations/roboflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-02-10 11:54:06.000000 depthai-sdk-1.9.4.1/src/depthai_sdk/components/multi_stage_nn.py
--rw-r--r--   0 runner    (1001) docker     (123)    35688 2023-02-10 11:54:06.000000 depthai-sdk-1.9.4.1/src/depthai_sdk/components/nn_component.py
--rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-02-10 11:54:06.000000 depthai-sdk-1.9.4.1/src/depthai_sdk/components/nn_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     7877 2023-02-10 11:54:06.000000 depthai-sdk-1.9.4.1/src/depthai_sdk/components/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    15501 2023-02-10 11:54:06.000000 depthai-sdk-1.9.4.1/src/depthai_sdk/components/stereo_component.py
--rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-02-10 11:54:06.000000 depthai-sdk-1.9.4.1/src/depthai_sdk/components/template_multi_stage_script.py
--rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-02-10 11:54:06.000000 depthai-sdk-1.9.4.1/src/depthai_sdk/fps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 11:54:17.293598 depthai-sdk-1.9.4.1/src/depthai_sdk/managers/
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-02-10 11:54:06.000000 depthai-sdk-1.9.4.1/src/depthai_sdk/managers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18003 2023-02-10 11:54:06.000000 depthai-sdk-1.9.4.1/src/depthai_sdk/managers/arg_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     5406 2023-02-10 11:54:06.000000 depthai-sdk-1.9.4.1/src/depthai_sdk/managers/blob_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     4871 2023-02-10 11:54:06.000000 depthai-sdk-1.9.4.1/src/depthai_sdk/managers/encoding_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    21217 2023-02-10 11:54:06.000000 depthai-sdk-1.9.4.1/src/depthai_sdk/managers/nnet_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    35810 2023-02-10 11:54:06.000000 depthai-sdk-1.9.4.1/src/depthai_sdk/managers/pipeline_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    13226 2023-02-10 11:54:06.000000 depthai-sdk-1.9.4.1/src/depthai_sdk/managers/preview_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 11:54:17.289598 depthai-sdk-1.9.4.1/src/depthai_sdk/nn_models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 11:54:17.293598 depthai-sdk-1.9.4.1/src/depthai_sdk/nn_models/age-gender-recognition-retail-0013/
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-02-10 11:54:06.000000 depthai-sdk-1.9.4.1/src/depthai_sdk/nn_models/age-gender-recognition-retail-0013/config.json
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-02-10 11:54:06.000000 depthai-sdk-1.9.4.1/src/depthai_sdk/nn_models/age-gender-recognition-retail-0013/handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 11:54:17.293598 depthai-sdk-1.9.4.1/src/depthai_sdk/nn_models/deeplabv3_person/
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-02-10 11:54:06.000000 depthai-sdk-1.9.4.1/src/depthai_sdk/nn_models/deeplabv3_person/config.json
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-02-10 11:54:06.000000 depthai-sdk-1.9.4.1/src/depthai_sdk/nn_models/deeplabv3_person/handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 11:54:17.293598 depthai-sdk-1.9.4.1/src/depthai_sdk/nn_models/emotions-recognition-retail-0003/
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-02-10 11:54:06.000000 depthai-sdk-1.9.4.1/src/depthai_sdk/nn_models/emotions-recognition-retail-0003/config.json
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-02-10 11:54:06.000000 depthai-sdk-1.9.4.1/src/depthai_sdk/nn_models/emotions-recognition-retail-0003/handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 11:54:17.293598 depthai-sdk-1.9.4.1/src/depthai_sdk/nn_models/face-detection-adas-0001/
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-02-10 11:54:06.000000 depthai-sdk-1.9.4.1/src/depthai_sdk/nn_models/face-detection-adas-0001/config.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 11:54:17.293598 depthai-sdk-1.9.4.1/src/depthai_sdk/nn_models/face-detection-retail-0004/
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-02-10 11:54:06.000000 depthai-sdk-1.9.4.1/src/depthai_sdk/nn_models/face-detection-retail-0004/config.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 11:54:17.293598 depthai-sdk-1.9.4.1/src/depthai_sdk/nn_models/human-pose-estimation-0001/
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-02-10 11:54:06.000000 depthai-sdk-1.9.4.1/src/depthai_sdk/nn_models/human-pose-estimation-0001/config.json
--rw-r--r--   0 runner    (1001) docker     (123)     7551 2023-02-10 11:54:06.000000 depthai-sdk-1.9.4.1/src/depthai_sdk/nn_models/human-pose-estimation-0001/handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 11:54:17.293598 depthai-sdk-1.9.4.1/src/depthai_sdk/nn_models/mobilenet-ssd/
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-02-10 11:54:06.000000 depthai-sdk-1.9.4.1/src/depthai_sdk/nn_models/mobilenet-ssd/config.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 11:54:17.297598 depthai-sdk-1.9.4.1/src/depthai_sdk/nn_models/openpose2/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-02-10 11:54:06.000000 depthai-sdk-1.9.4.1/src/depthai_sdk/nn_models/openpose2/config.json
--rw-r--r--   0 runner    (1001) docker     (123)     7879 2023-02-10 11:54:06.000000 depthai-sdk-1.9.4.1/src/depthai_sdk/nn_models/openpose2/handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-02-10 11:54:06.000000 depthai-sdk-1.9.4.1/src/depthai_sdk/nn_models/openpose2/model.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 11:54:17.297598 depthai-sdk-1.9.4.1/src/depthai_sdk/nn_models/pedestrian-detection-adas-0002/
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-02-10 11:54:06.000000 depthai-sdk-1.9.4.1/src/depthai_sdk/nn_models/pedestrian-detection-adas-0002/config.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 11:54:17.297598 depthai-sdk-1.9.4.1/src/depthai_sdk/nn_models/person-detection-0200/
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-02-10 11:54:06.000000 depthai-sdk-1.9.4.1/src/depthai_sdk/nn_models/person-detection-0200/config.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 11:54:17.297598 depthai-sdk-1.9.4.1/src/depthai_sdk/nn_models/person-detection-retail-0013/
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-02-10 11:54:06.000000 depthai-sdk-1.9.4.1/src/depthai_sdk/nn_models/person-detection-retail-0013/config.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 11:54:17.297598 depthai-sdk-1.9.4.1/src/depthai_sdk/nn_models/person-reidentification-retail-0288/
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-02-10 11:54:06.000000 depthai-sdk-1.9.4.1/src/depthai_sdk/nn_models/person-reidentification-retail-0288/config.json
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-02-10 11:54:06.000000 depthai-sdk-1.9.4.1/src/depthai_sdk/nn_models/person-reidentification-retail-0288/handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 11:54:17.297598 depthai-sdk-1.9.4.1/src/depthai_sdk/nn_models/person-vehicle-bike-detection-crossroad-1016/
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-02-10 11:54:06.000000 depthai-sdk-1.9.4.1/src/depthai_sdk/nn_models/person-vehicle-bike-detection-crossroad-1016/config.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 11:54:17.297598 depthai-sdk-1.9.4.1/src/depthai_sdk/nn_models/road-segmentation-adas-0001/
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-02-10 11:54:06.000000 depthai-sdk-1.9.4.1/src/depthai_sdk/nn_models/road-segmentation-adas-0001/config.json
--rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-02-10 11:54:06.000000 depthai-sdk-1.9.4.1/src/depthai_sdk/nn_models/road-segmentation-adas-0001/handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 11:54:17.297598 depthai-sdk-1.9.4.1/src/depthai_sdk/nn_models/sbd_mask_classification_224x224/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-02-10 11:54:06.000000 depthai-sdk-1.9.4.1/src/depthai_sdk/nn_models/sbd_mask_classification_224x224/config.json
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-02-10 11:54:06.000000 depthai-sdk-1.9.4.1/src/depthai_sdk/nn_models/sbd_mask_classification_224x224/handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 11:54:17.297598 depthai-sdk-1.9.4.1/src/depthai_sdk/nn_models/vehicle-detection-0202/
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-02-10 11:54:06.000000 depthai-sdk-1.9.4.1/src/depthai_sdk/nn_models/vehicle-detection-0202/config.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 11:54:17.297598 depthai-sdk-1.9.4.1/src/depthai_sdk/nn_models/vehicle-detection-adas-0002/
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-02-10 11:54:06.000000 depthai-sdk-1.9.4.1/src/depthai_sdk/nn_models/vehicle-detection-adas-0002/config.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 11:54:17.297598 depthai-sdk-1.9.4.1/src/depthai_sdk/nn_models/vehicle-license-plate-detection-barrier-0106/
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-02-10 11:54:06.000000 depthai-sdk-1.9.4.1/src/depthai_sdk/nn_models/vehicle-license-plate-detection-barrier-0106/config.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 11:54:17.297598 depthai-sdk-1.9.4.1/src/depthai_sdk/nn_models/yolo-v3-tf/
--rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-02-10 11:54:06.000000 depthai-sdk-1.9.4.1/src/depthai_sdk/nn_models/yolo-v3-tf/config.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 11:54:17.297598 depthai-sdk-1.9.4.1/src/depthai_sdk/nn_models/yolo-v3-tiny-tf/
--rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-02-10 11:54:06.000000 depthai-sdk-1.9.4.1/src/depthai_sdk/nn_models/yolo-v3-tiny-tf/config.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 11:54:17.297598 depthai-sdk-1.9.4.1/src/depthai_sdk/nn_models/yolov4_coco_608x608/
--rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-02-10 11:54:06.000000 depthai-sdk-1.9.4.1/src/depthai_sdk/nn_models/yolov4_coco_608x608/config.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 11:54:17.297598 depthai-sdk-1.9.4.1/src/depthai_sdk/nn_models/yolov4_tiny_coco_416x416/
--rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-02-10 11:54:06.000000 depthai-sdk-1.9.4.1/src/depthai_sdk/nn_models/yolov4_tiny_coco_416x416/config.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 11:54:17.297598 depthai-sdk-1.9.4.1/src/depthai_sdk/nn_models/yolov5n_coco_416x416/
--rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-02-10 11:54:06.000000 depthai-sdk-1.9.4.1/src/depthai_sdk/nn_models/yolov5n_coco_416x416/config.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 11:54:17.297598 depthai-sdk-1.9.4.1/src/depthai_sdk/nn_models/yolov6n_coco_640x640/
--rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-02-10 11:54:06.000000 depthai-sdk-1.9.4.1/src/depthai_sdk/nn_models/yolov6n_coco_640x640/config.json
--rw-r--r--   0 runner    (1001) docker     (123)    22192 2023-02-10 11:54:06.000000 depthai-sdk-1.9.4.1/src/depthai_sdk/oak_camera.py
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-02-10 11:54:06.000000 depthai-sdk-1.9.4.1/src/depthai_sdk/oak_device.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 11:54:17.297598 depthai-sdk-1.9.4.1/src/depthai_sdk/oak_outputs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-10 11:54:06.000000 depthai-sdk-1.9.4.1/src/depthai_sdk/oak_outputs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-02-10 11:54:06.000000 depthai-sdk-1.9.4.1/src/depthai_sdk/oak_outputs/fps.py
--rw-r--r--   0 runner    (1001) docker     (123)     4419 2023-02-10 11:54:06.000000 depthai-sdk-1.9.4.1/src/depthai_sdk/oak_outputs/normalize_bb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-02-10 11:54:06.000000 depthai-sdk-1.9.4.1/src/depthai_sdk/oak_outputs/syncing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 11:54:17.301599 depthai-sdk-1.9.4.1/src/depthai_sdk/oak_outputs/xout/
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-02-10 11:54:06.000000 depthai-sdk-1.9.4.1/src/depthai_sdk/oak_outputs/xout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-02-10 11:54:06.000000 depthai-sdk-1.9.4.1/src/depthai_sdk/oak_outputs/xout/xout_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5215 2023-02-10 11:54:06.000000 depthai-sdk-1.9.4.1/src/depthai_sdk/oak_outputs/xout/xout_depth.py
--rw-r--r--   0 runner    (1001) docker     (123)     4768 2023-02-10 11:54:06.000000 depthai-sdk-1.9.4.1/src/depthai_sdk/oak_outputs/xout/xout_disparity.py
--rw-r--r--   0 runner    (1001) docker     (123)     3568 2023-02-10 11:54:06.000000 depthai-sdk-1.9.4.1/src/depthai_sdk/oak_outputs/xout/xout_frames.py
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-02-10 11:54:06.000000 depthai-sdk-1.9.4.1/src/depthai_sdk/oak_outputs/xout/xout_h26x.py
--rw-r--r--   0 runner    (1001) docker     (123)     4590 2023-02-10 11:54:06.000000 depthai-sdk-1.9.4.1/src/depthai_sdk/oak_outputs/xout/xout_imu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-02-10 11:54:06.000000 depthai-sdk-1.9.4.1/src/depthai_sdk/oak_outputs/xout/xout_mjpeg.py
--rw-r--r--   0 runner    (1001) docker     (123)    18032 2023-02-10 11:54:06.000000 depthai-sdk-1.9.4.1/src/depthai_sdk/oak_outputs/xout/xout_nn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-02-10 11:54:06.000000 depthai-sdk-1.9.4.1/src/depthai_sdk/oak_outputs/xout/xout_nn_encoded.py
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-02-10 11:54:06.000000 depthai-sdk-1.9.4.1/src/depthai_sdk/oak_outputs/xout/xout_seq_sync.py
--rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-02-10 11:54:06.000000 depthai-sdk-1.9.4.1/src/depthai_sdk/oak_outputs/xout/xout_tracker.py
--rw-r--r--   0 runner    (1001) docker     (123)    11394 2023-02-10 11:54:06.000000 depthai-sdk-1.9.4.1/src/depthai_sdk/previews.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 11:54:17.301599 depthai-sdk-1.9.4.1/src/depthai_sdk/readers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-10 11:54:06.000000 depthai-sdk-1.9.4.1/src/depthai_sdk/readers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-02-10 11:54:06.000000 depthai-sdk-1.9.4.1/src/depthai_sdk/readers/abstract_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-02-10 11:54:06.000000 depthai-sdk-1.9.4.1/src/depthai_sdk/readers/db3_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-02-10 11:54:06.000000 depthai-sdk-1.9.4.1/src/depthai_sdk/readers/image_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-02-10 11:54:06.000000 depthai-sdk-1.9.4.1/src/depthai_sdk/readers/mcap_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-02-10 11:54:06.000000 depthai-sdk-1.9.4.1/src/depthai_sdk/readers/rosbag_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-02-10 11:54:06.000000 depthai-sdk-1.9.4.1/src/depthai_sdk/readers/videocap_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     5354 2023-02-10 11:54:06.000000 depthai-sdk-1.9.4.1/src/depthai_sdk/record.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 11:54:17.301599 depthai-sdk-1.9.4.1/src/depthai_sdk/recorders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-10 11:54:06.000000 depthai-sdk-1.9.4.1/src/depthai_sdk/recorders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-02-10 11:54:06.000000 depthai-sdk-1.9.4.1/src/depthai_sdk/recorders/abstract_recorder.py
--rw-r--r--   0 runner    (1001) docker     (123)    12360 2023-02-10 11:54:06.000000 depthai-sdk-1.9.4.1/src/depthai_sdk/recorders/depthai2ros.py
--rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-02-10 11:54:06.000000 depthai-sdk-1.9.4.1/src/depthai_sdk/recorders/mcap_recorder.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    20528 2023-02-10 11:54:06.000000 depthai-sdk-1.9.4.1/src/depthai_sdk/recorders/rosbag_recorder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-02-10 11:54:06.000000 depthai-sdk-1.9.4.1/src/depthai_sdk/recorders/video_recorder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 11:54:17.301599 depthai-sdk-1.9.4.1/src/depthai_sdk/recorders/video_writers/
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-02-10 11:54:06.000000 depthai-sdk-1.9.4.1/src/depthai_sdk/recorders/video_writers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-02-10 11:54:06.000000 depthai-sdk-1.9.4.1/src/depthai_sdk/recorders/video_writers/abstract_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-02-10 11:54:06.000000 depthai-sdk-1.9.4.1/src/depthai_sdk/recorders/video_writers/av_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-02-10 11:54:06.000000 depthai-sdk-1.9.4.1/src/depthai_sdk/recorders/video_writers/file_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-02-10 11:54:06.000000 depthai-sdk-1.9.4.1/src/depthai_sdk/recorders/video_writers/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3918 2023-02-10 11:54:06.000000 depthai-sdk-1.9.4.1/src/depthai_sdk/recorders/video_writers/video_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)    13936 2023-02-10 11:54:06.000000 depthai-sdk-1.9.4.1/src/depthai_sdk/replay.py
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-02-10 11:54:06.000000 depthai-sdk-1.9.4.1/src/depthai_sdk/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    13233 2023-02-10 11:54:06.000000 depthai-sdk-1.9.4.1/src/depthai_sdk/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 11:54:17.301599 depthai-sdk-1.9.4.1/src/depthai_sdk/visualize/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-10 11:54:06.000000 depthai-sdk-1.9.4.1/src/depthai_sdk/visualize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-02-10 11:54:06.000000 depthai-sdk-1.9.4.1/src/depthai_sdk/visualize/configs.py
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-02-10 11:54:06.000000 depthai-sdk-1.9.4.1/src/depthai_sdk/visualize/encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)    26532 2023-02-10 11:54:06.000000 depthai-sdk-1.9.4.1/src/depthai_sdk/visualize/objects.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-02-10 11:54:06.000000 depthai-sdk-1.9.4.1/src/depthai_sdk/visualize/polygon.py
--rw-r--r--   0 runner    (1001) docker     (123)    13727 2023-02-10 11:54:06.000000 depthai-sdk-1.9.4.1/src/depthai_sdk/visualize/visualizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    15375 2023-02-10 11:54:06.000000 depthai-sdk-1.9.4.1/src/depthai_sdk/visualize/visualizer_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 11:54:17.289598 depthai-sdk-1.9.4.1/src/depthai_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-02-10 11:54:17.000000 depthai-sdk-1.9.4.1/src/depthai_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5524 2023-02-10 11:54:17.000000 depthai-sdk-1.9.4.1/src/depthai_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-10 11:54:17.000000 depthai-sdk-1.9.4.1/src/depthai_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-02-10 11:54:17.000000 depthai-sdk-1.9.4.1/src/depthai_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-02-10 11:54:17.000000 depthai-sdk-1.9.4.1/src/depthai_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:19:21.238091 depthai-sdk-1.9.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-04-21 15:19:08.000000 depthai-sdk-1.9.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-04-21 15:19:21.238091 depthai-sdk-1.9.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-04-21 15:19:08.000000 depthai-sdk-1.9.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-04-21 15:19:08.000000 depthai-sdk-1.9.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 15:19:21.238091 depthai-sdk-1.9.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-04-21 15:19:08.000000 depthai-sdk-1.9.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:19:21.218091 depthai-sdk-1.9.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:19:21.222091 depthai-sdk-1.9.5/src/depthai_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-04-21 15:19:08.000000 depthai-sdk-1.9.5/src/depthai_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10952 2023-04-21 15:19:08.000000 depthai-sdk-1.9.5/src/depthai_sdk/args_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:19:21.222091 depthai-sdk-1.9.5/src/depthai_sdk/classes/
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-21 15:19:08.000000 depthai-sdk-1.9.5/src/depthai_sdk/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-04-21 15:19:08.000000 depthai-sdk-1.9.5/src/depthai_sdk/classes/enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-04-21 15:19:08.000000 depthai-sdk-1.9.5/src/depthai_sdk/classes/nn_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-04-21 15:19:08.000000 depthai-sdk-1.9.5/src/depthai_sdk/classes/nn_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6012 2023-04-21 15:19:08.000000 depthai-sdk-1.9.5/src/depthai_sdk/classes/output_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7451 2023-04-21 15:19:08.000000 depthai-sdk-1.9.5/src/depthai_sdk/classes/packets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-04-21 15:19:08.000000 depthai-sdk-1.9.5/src/depthai_sdk/classes/yolo_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:19:21.226091 depthai-sdk-1.9.5/src/depthai_sdk/components/
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-04-21 15:19:08.000000 depthai-sdk-1.9.5/src/depthai_sdk/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21926 2023-04-21 15:19:08.000000 depthai-sdk-1.9.5/src/depthai_sdk/components/camera_component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9747 2023-04-21 15:19:08.000000 depthai-sdk-1.9.5/src/depthai_sdk/components/camera_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-04-21 15:19:08.000000 depthai-sdk-1.9.5/src/depthai_sdk/components/component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-04-21 15:19:08.000000 depthai-sdk-1.9.5/src/depthai_sdk/components/imu_component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-04-21 15:19:08.000000 depthai-sdk-1.9.5/src/depthai_sdk/components/multi_stage_nn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38641 2023-04-21 15:19:08.000000 depthai-sdk-1.9.5/src/depthai_sdk/components/nn_component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-04-21 15:19:08.000000 depthai-sdk-1.9.5/src/depthai_sdk/components/nn_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7921 2023-04-21 15:19:08.000000 depthai-sdk-1.9.5/src/depthai_sdk/components/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19255 2023-04-21 15:19:08.000000 depthai-sdk-1.9.5/src/depthai_sdk/components/stereo_component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-04-21 15:19:08.000000 depthai-sdk-1.9.5/src/depthai_sdk/components/template_multi_stage_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-04-21 15:19:08.000000 depthai-sdk-1.9.5/src/depthai_sdk/components/undistort.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-04-21 15:19:08.000000 depthai-sdk-1.9.5/src/depthai_sdk/fps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:19:21.226091 depthai-sdk-1.9.5/src/depthai_sdk/integrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 15:19:08.000000 depthai-sdk-1.9.5/src/depthai_sdk/integrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-04-21 15:19:08.000000 depthai-sdk-1.9.5/src/depthai_sdk/integrations/roboflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:19:21.226091 depthai-sdk-1.9.5/src/depthai_sdk/integrations/ros/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 15:19:08.000000 depthai-sdk-1.9.5/src/depthai_sdk/integrations/ros/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7304 2023-04-21 15:19:08.000000 depthai-sdk-1.9.5/src/depthai_sdk/integrations/ros/depthai2ros.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6303 2023-04-21 15:19:08.000000 depthai-sdk-1.9.5/src/depthai_sdk/integrations/ros/depthai2ros2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7395 2023-04-21 15:19:08.000000 depthai-sdk-1.9.5/src/depthai_sdk/integrations/ros/imu_interpolation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-04-21 15:19:08.000000 depthai-sdk-1.9.5/src/depthai_sdk/integrations/ros/ros2_streaming.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-04-21 15:19:08.000000 depthai-sdk-1.9.5/src/depthai_sdk/integrations/ros/ros_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-04-21 15:19:08.000000 depthai-sdk-1.9.5/src/depthai_sdk/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:19:21.226091 depthai-sdk-1.9.5/src/depthai_sdk/managers/
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-21 15:19:08.000000 depthai-sdk-1.9.5/src/depthai_sdk/managers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18003 2023-04-21 15:19:08.000000 depthai-sdk-1.9.5/src/depthai_sdk/managers/arg_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5406 2023-04-21 15:19:08.000000 depthai-sdk-1.9.5/src/depthai_sdk/managers/blob_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4871 2023-04-21 15:19:08.000000 depthai-sdk-1.9.5/src/depthai_sdk/managers/encoding_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21217 2023-04-21 15:19:08.000000 depthai-sdk-1.9.5/src/depthai_sdk/managers/nnet_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35810 2023-04-21 15:19:08.000000 depthai-sdk-1.9.5/src/depthai_sdk/managers/pipeline_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13226 2023-04-21 15:19:08.000000 depthai-sdk-1.9.5/src/depthai_sdk/managers/preview_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:19:21.218091 depthai-sdk-1.9.5/src/depthai_sdk/nn_models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:19:21.226091 depthai-sdk-1.9.5/src/depthai_sdk/nn_models/age-gender-recognition-retail-0013/
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-21 15:19:08.000000 depthai-sdk-1.9.5/src/depthai_sdk/nn_models/age-gender-recognition-retail-0013/config.json
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-21 15:19:08.000000 depthai-sdk-1.9.5/src/depthai_sdk/nn_models/age-gender-recognition-retail-0013/handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:19:21.226091 depthai-sdk-1.9.5/src/depthai_sdk/nn_models/deeplabv3_person/
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-21 15:19:08.000000 depthai-sdk-1.9.5/src/depthai_sdk/nn_models/deeplabv3_person/config.json
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-21 15:19:08.000000 depthai-sdk-1.9.5/src/depthai_sdk/nn_models/deeplabv3_person/handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:19:21.226091 depthai-sdk-1.9.5/src/depthai_sdk/nn_models/emotions-recognition-retail-0003/
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-21 15:19:08.000000 depthai-sdk-1.9.5/src/depthai_sdk/nn_models/emotions-recognition-retail-0003/config.json
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-21 15:19:08.000000 depthai-sdk-1.9.5/src/depthai_sdk/nn_models/emotions-recognition-retail-0003/handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:19:21.230091 depthai-sdk-1.9.5/src/depthai_sdk/nn_models/face-detection-adas-0001/
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-04-21 15:19:08.000000 depthai-sdk-1.9.5/src/depthai_sdk/nn_models/face-detection-adas-0001/config.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:19:21.230091 depthai-sdk-1.9.5/src/depthai_sdk/nn_models/face-detection-retail-0004/
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-04-21 15:19:08.000000 depthai-sdk-1.9.5/src/depthai_sdk/nn_models/face-detection-retail-0004/config.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:19:21.230091 depthai-sdk-1.9.5/src/depthai_sdk/nn_models/human-pose-estimation-0001/
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-21 15:19:08.000000 depthai-sdk-1.9.5/src/depthai_sdk/nn_models/human-pose-estimation-0001/config.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7551 2023-04-21 15:19:08.000000 depthai-sdk-1.9.5/src/depthai_sdk/nn_models/human-pose-estimation-0001/handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:19:21.230091 depthai-sdk-1.9.5/src/depthai_sdk/nn_models/mobilenet-ssd/
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-04-21 15:19:08.000000 depthai-sdk-1.9.5/src/depthai_sdk/nn_models/mobilenet-ssd/config.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:19:21.230091 depthai-sdk-1.9.5/src/depthai_sdk/nn_models/openpose2/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-21 15:19:08.000000 depthai-sdk-1.9.5/src/depthai_sdk/nn_models/openpose2/config.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7879 2023-04-21 15:19:08.000000 depthai-sdk-1.9.5/src/depthai_sdk/nn_models/openpose2/handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-04-21 15:19:08.000000 depthai-sdk-1.9.5/src/depthai_sdk/nn_models/openpose2/model.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:19:21.230091 depthai-sdk-1.9.5/src/depthai_sdk/nn_models/palm_detection_128x128/
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-04-21 15:19:08.000000 depthai-sdk-1.9.5/src/depthai_sdk/nn_models/palm_detection_128x128/config.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4653 2023-04-21 15:19:08.000000 depthai-sdk-1.9.5/src/depthai_sdk/nn_models/palm_detection_128x128/handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:19:21.230091 depthai-sdk-1.9.5/src/depthai_sdk/nn_models/pedestrian-detection-adas-0002/
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-04-21 15:19:08.000000 depthai-sdk-1.9.5/src/depthai_sdk/nn_models/pedestrian-detection-adas-0002/config.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:19:21.230091 depthai-sdk-1.9.5/src/depthai_sdk/nn_models/person-detection-0200/
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-04-21 15:19:08.000000 depthai-sdk-1.9.5/src/depthai_sdk/nn_models/person-detection-0200/config.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:19:21.230091 depthai-sdk-1.9.5/src/depthai_sdk/nn_models/person-detection-retail-0013/
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-21 15:19:08.000000 depthai-sdk-1.9.5/src/depthai_sdk/nn_models/person-detection-retail-0013/config.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:19:21.230091 depthai-sdk-1.9.5/src/depthai_sdk/nn_models/person-reidentification-retail-0288/
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-21 15:19:08.000000 depthai-sdk-1.9.5/src/depthai_sdk/nn_models/person-reidentification-retail-0288/config.json
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-21 15:19:08.000000 depthai-sdk-1.9.5/src/depthai_sdk/nn_models/person-reidentification-retail-0288/handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:19:21.230091 depthai-sdk-1.9.5/src/depthai_sdk/nn_models/person-vehicle-bike-detection-crossroad-1016/
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-04-21 15:19:08.000000 depthai-sdk-1.9.5/src/depthai_sdk/nn_models/person-vehicle-bike-detection-crossroad-1016/config.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:19:21.230091 depthai-sdk-1.9.5/src/depthai_sdk/nn_models/road-segmentation-adas-0001/
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-21 15:19:08.000000 depthai-sdk-1.9.5/src/depthai_sdk/nn_models/road-segmentation-adas-0001/config.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-04-21 15:19:08.000000 depthai-sdk-1.9.5/src/depthai_sdk/nn_models/road-segmentation-adas-0001/handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:19:21.230091 depthai-sdk-1.9.5/src/depthai_sdk/nn_models/sbd_mask_classification_224x224/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-21 15:19:08.000000 depthai-sdk-1.9.5/src/depthai_sdk/nn_models/sbd_mask_classification_224x224/config.json
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-21 15:19:08.000000 depthai-sdk-1.9.5/src/depthai_sdk/nn_models/sbd_mask_classification_224x224/handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:19:21.230091 depthai-sdk-1.9.5/src/depthai_sdk/nn_models/vehicle-detection-0202/
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-04-21 15:19:08.000000 depthai-sdk-1.9.5/src/depthai_sdk/nn_models/vehicle-detection-0202/config.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:19:21.230091 depthai-sdk-1.9.5/src/depthai_sdk/nn_models/vehicle-detection-adas-0002/
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-21 15:19:08.000000 depthai-sdk-1.9.5/src/depthai_sdk/nn_models/vehicle-detection-adas-0002/config.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:19:21.230091 depthai-sdk-1.9.5/src/depthai_sdk/nn_models/vehicle-license-plate-detection-barrier-0106/
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-04-21 15:19:08.000000 depthai-sdk-1.9.5/src/depthai_sdk/nn_models/vehicle-license-plate-detection-barrier-0106/config.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:19:21.230091 depthai-sdk-1.9.5/src/depthai_sdk/nn_models/yolo-v3-tf/
+-rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-04-21 15:19:08.000000 depthai-sdk-1.9.5/src/depthai_sdk/nn_models/yolo-v3-tf/config.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:19:21.230091 depthai-sdk-1.9.5/src/depthai_sdk/nn_models/yolo-v3-tiny-tf/
+-rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-04-21 15:19:08.000000 depthai-sdk-1.9.5/src/depthai_sdk/nn_models/yolo-v3-tiny-tf/config.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:19:21.230091 depthai-sdk-1.9.5/src/depthai_sdk/nn_models/yolov4_coco_608x608/
+-rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-04-21 15:19:08.000000 depthai-sdk-1.9.5/src/depthai_sdk/nn_models/yolov4_coco_608x608/config.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:19:21.230091 depthai-sdk-1.9.5/src/depthai_sdk/nn_models/yolov4_tiny_coco_416x416/
+-rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-04-21 15:19:08.000000 depthai-sdk-1.9.5/src/depthai_sdk/nn_models/yolov4_tiny_coco_416x416/config.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:19:21.230091 depthai-sdk-1.9.5/src/depthai_sdk/nn_models/yolov5n_coco_416x416/
+-rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-04-21 15:19:08.000000 depthai-sdk-1.9.5/src/depthai_sdk/nn_models/yolov5n_coco_416x416/config.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:19:21.230091 depthai-sdk-1.9.5/src/depthai_sdk/nn_models/yolov6n_coco_640x640/
+-rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-04-21 15:19:08.000000 depthai-sdk-1.9.5/src/depthai_sdk/nn_models/yolov6n_coco_640x640/config.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:19:21.230091 depthai-sdk-1.9.5/src/depthai_sdk/nn_models/yolov6nr3_coco_640x352/
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-04-21 15:19:08.000000 depthai-sdk-1.9.5/src/depthai_sdk/nn_models/yolov6nr3_coco_640x352/config.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:19:21.234091 depthai-sdk-1.9.5/src/depthai_sdk/nn_models/yolov7tiny_coco_416x416/
+-rw-r--r--   0 runner    (1001) docker     (123)     2605 2023-04-21 15:19:08.000000 depthai-sdk-1.9.5/src/depthai_sdk/nn_models/yolov7tiny_coco_416x416/config.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:19:21.234091 depthai-sdk-1.9.5/src/depthai_sdk/nn_models/yolov7tiny_coco_640x352/
+-rw-r--r--   0 runner    (1001) docker     (123)     2605 2023-04-21 15:19:08.000000 depthai-sdk-1.9.5/src/depthai_sdk/nn_models/yolov7tiny_coco_640x352/config.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:19:21.234091 depthai-sdk-1.9.5/src/depthai_sdk/nn_models/yolov8n_coco_640x352/
+-rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-04-21 15:19:08.000000 depthai-sdk-1.9.5/src/depthai_sdk/nn_models/yolov8n_coco_640x352/config.json
+-rw-r--r--   0 runner    (1001) docker     (123)    24260 2023-04-21 15:19:08.000000 depthai-sdk-1.9.5/src/depthai_sdk/oak_camera.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-04-21 15:19:08.000000 depthai-sdk-1.9.5/src/depthai_sdk/oak_device.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:19:21.234091 depthai-sdk-1.9.5/src/depthai_sdk/oak_outputs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 15:19:08.000000 depthai-sdk-1.9.5/src/depthai_sdk/oak_outputs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-21 15:19:08.000000 depthai-sdk-1.9.5/src/depthai_sdk/oak_outputs/fps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4410 2023-04-21 15:19:08.000000 depthai-sdk-1.9.5/src/depthai_sdk/oak_outputs/normalize_bb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-04-21 15:19:08.000000 depthai-sdk-1.9.5/src/depthai_sdk/oak_outputs/syncing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:19:21.234091 depthai-sdk-1.9.5/src/depthai_sdk/oak_outputs/xout/
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-21 15:19:08.000000 depthai-sdk-1.9.5/src/depthai_sdk/oak_outputs/xout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-04-21 15:19:08.000000 depthai-sdk-1.9.5/src/depthai_sdk/oak_outputs/xout/xout_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5696 2023-04-21 15:19:08.000000 depthai-sdk-1.9.5/src/depthai_sdk/oak_outputs/xout/xout_depth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5254 2023-04-21 15:19:08.000000 depthai-sdk-1.9.5/src/depthai_sdk/oak_outputs/xout/xout_disparity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3563 2023-04-21 15:19:08.000000 depthai-sdk-1.9.5/src/depthai_sdk/oak_outputs/xout/xout_frames.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-04-21 15:19:08.000000 depthai-sdk-1.9.5/src/depthai_sdk/oak_outputs/xout/xout_h26x.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4594 2023-04-21 15:19:08.000000 depthai-sdk-1.9.5/src/depthai_sdk/oak_outputs/xout/xout_imu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-04-21 15:19:08.000000 depthai-sdk-1.9.5/src/depthai_sdk/oak_outputs/xout/xout_mjpeg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19868 2023-04-21 15:19:08.000000 depthai-sdk-1.9.5/src/depthai_sdk/oak_outputs/xout/xout_nn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-04-21 15:19:08.000000 depthai-sdk-1.9.5/src/depthai_sdk/oak_outputs/xout/xout_nn_encoded.py
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-04-21 15:19:08.000000 depthai-sdk-1.9.5/src/depthai_sdk/oak_outputs/xout/xout_seq_sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14229 2023-04-21 15:19:08.000000 depthai-sdk-1.9.5/src/depthai_sdk/oak_outputs/xout/xout_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11394 2023-04-21 15:19:08.000000 depthai-sdk-1.9.5/src/depthai_sdk/previews.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:19:21.234091 depthai-sdk-1.9.5/src/depthai_sdk/readers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 15:19:08.000000 depthai-sdk-1.9.5/src/depthai_sdk/readers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-04-21 15:19:08.000000 depthai-sdk-1.9.5/src/depthai_sdk/readers/abstract_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-04-21 15:19:08.000000 depthai-sdk-1.9.5/src/depthai_sdk/readers/db3_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3347 2023-04-21 15:19:08.000000 depthai-sdk-1.9.5/src/depthai_sdk/readers/image_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-04-21 15:19:08.000000 depthai-sdk-1.9.5/src/depthai_sdk/readers/mcap_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-04-21 15:19:08.000000 depthai-sdk-1.9.5/src/depthai_sdk/readers/rosbag_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-04-21 15:19:08.000000 depthai-sdk-1.9.5/src/depthai_sdk/readers/videocap_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-04-21 15:19:08.000000 depthai-sdk-1.9.5/src/depthai_sdk/record.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:19:21.234091 depthai-sdk-1.9.5/src/depthai_sdk/recorders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 15:19:08.000000 depthai-sdk-1.9.5/src/depthai_sdk/recorders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-04-21 15:19:08.000000 depthai-sdk-1.9.5/src/depthai_sdk/recorders/abstract_recorder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-04-21 15:19:08.000000 depthai-sdk-1.9.5/src/depthai_sdk/recorders/mcap_recorder.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    24547 2023-04-21 15:19:08.000000 depthai-sdk-1.9.5/src/depthai_sdk/recorders/rosbag_recorder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-04-21 15:19:08.000000 depthai-sdk-1.9.5/src/depthai_sdk/recorders/video_recorder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:19:21.238091 depthai-sdk-1.9.5/src/depthai_sdk/recorders/video_writers/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-21 15:19:08.000000 depthai-sdk-1.9.5/src/depthai_sdk/recorders/video_writers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-21 15:19:08.000000 depthai-sdk-1.9.5/src/depthai_sdk/recorders/video_writers/abstract_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-04-21 15:19:08.000000 depthai-sdk-1.9.5/src/depthai_sdk/recorders/video_writers/av_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-04-21 15:19:08.000000 depthai-sdk-1.9.5/src/depthai_sdk/recorders/video_writers/file_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-04-21 15:19:08.000000 depthai-sdk-1.9.5/src/depthai_sdk/recorders/video_writers/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-04-21 15:19:08.000000 depthai-sdk-1.9.5/src/depthai_sdk/recorders/video_writers/video_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15741 2023-04-21 15:19:08.000000 depthai-sdk-1.9.5/src/depthai_sdk/replay.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:19:21.238091 depthai-sdk-1.9.5/src/depthai_sdk/tracking/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-21 15:19:08.000000 depthai-sdk-1.9.5/src/depthai_sdk/tracking/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-04-21 15:19:08.000000 depthai-sdk-1.9.5/src/depthai_sdk/tracking/kalman.py
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-21 15:19:08.000000 depthai-sdk-1.9.5/src/depthai_sdk/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13233 2023-04-21 15:19:08.000000 depthai-sdk-1.9.5/src/depthai_sdk/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:19:21.238091 depthai-sdk-1.9.5/src/depthai_sdk/visualize/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-21 15:19:08.000000 depthai-sdk-1.9.5/src/depthai_sdk/visualize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3067 2023-04-21 15:19:08.000000 depthai-sdk-1.9.5/src/depthai_sdk/visualize/configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-04-21 15:19:08.000000 depthai-sdk-1.9.5/src/depthai_sdk/visualize/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26519 2023-04-21 15:19:08.000000 depthai-sdk-1.9.5/src/depthai_sdk/visualize/objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-21 15:19:08.000000 depthai-sdk-1.9.5/src/depthai_sdk/visualize/polygon.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13832 2023-04-21 15:19:08.000000 depthai-sdk-1.9.5/src/depthai_sdk/visualize/visualizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15375 2023-04-21 15:19:08.000000 depthai-sdk-1.9.5/src/depthai_sdk/visualize/visualizer_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:19:21.222091 depthai-sdk-1.9.5/src/depthai_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-04-21 15:19:21.000000 depthai-sdk-1.9.5/src/depthai_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6340 2023-04-21 15:19:21.000000 depthai-sdk-1.9.5/src/depthai_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 15:19:21.000000 depthai-sdk-1.9.5/src/depthai_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-21 15:19:21.000000 depthai-sdk-1.9.5/src/depthai_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-21 15:19:21.000000 depthai-sdk-1.9.5/src/depthai_sdk.egg-info/top_level.txt
```

### Comparing `depthai-sdk-1.9.4.1/MANIFEST.in` & `depthai-sdk-1.9.5/MANIFEST.in`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 include src/depthai_sdk/classes/*.py
 recursive-include src/depthai_sdk/components *.py
+recursive-include src/depthai_sdk/integrations *.py
 include src/depthai_sdk/managers/*.py
 
 recursive-include src/depthai_sdk/nn_models handler.py
 recursive-include src/depthai_sdk/nn_models *.yml
 recursive-include src/depthai_sdk/nn_models config.json
 
 include src/depthai_sdk/oak_outputs/*.py
 include src/depthai_sdk/oak_outputs/xout/*.py
 include src/depthai_sdk/readers/*.py
 recursive-include src/depthai_sdk/recorders *.py
+include src/depthai_sdk/tracking/*.py
 include src/depthai_sdk/visualize/*.py
-include requirements.txt
+include requirements.txt
+include src/depthai_sdk/logger.py
```

### Comparing `depthai-sdk-1.9.4.1/PKG-INFO` & `depthai-sdk-1.9.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: depthai-sdk
-Version: 1.9.4.1
+Version: 1.9.5
 Summary: This package provides an abstraction of the DepthAI API library.
 Home-page: https://github.com/luxonis/depthai/tree/main/depthai_sdk
 Author: Luxonis
 Author-email: support@luxonis.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/luxonis/depthai/issues
 Project-URL: Source Code, https://github.com/luxonis/depthai/tree/main/depthai_sdk
```

### Comparing `depthai-sdk-1.9.4.1/README.md` & `depthai-sdk-1.9.5/README.md`

 * *Files identical despite different names*

### Comparing `depthai-sdk-1.9.4.1/setup.py` & `depthai-sdk-1.9.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 with open('requirements.txt') as f:
     requirements = f.readlines()
 
 install_requires = [requirement for requirement in requirements if '--' not in requirement]
 
 setup(
     name='depthai-sdk',
-    version='1.9.4.1',
+    version='1.9.5',
     description='This package provides an abstraction of the DepthAI API library.',
     long_description=io.open("README.md", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     url='https://github.com/luxonis/depthai/tree/main/depthai_sdk',
     keywords="depthai sdk oak camera",
     author='Luxonis',
     author_email='support@luxonis.com',
```

### Comparing `depthai-sdk-1.9.4.1/src/depthai_sdk/args_parser.py` & `depthai-sdk-1.9.5/src/depthai_sdk/args_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -129,15 +129,15 @@
         # parser.add_argument("--cameraContrast", type=_commaSeparated("all", int), nargs="+",
         #                     help="Specify image contrast")
         # parser.add_argument("--cameraBrightness", type=_commaSeparated("all", int), nargs="+",
         #                     help="Specify image brightness")
         # parser.add_argument("--cameraSharpness", type=_commaSeparated("all", int), nargs="+",
         #                     help="Specify image sharpness")
 
-        # Depth related arguments
+        # StereoDepth related arguments
         parser.add_argument("-dct", "--disparityConfidenceThreshold", type=_checkRange(0, 255),
                             help="Disparity confidence threshold, used for depth measurement.")
         parser.add_argument("-lrct", "--lrcThreshold", type=_checkRange(0, 10),
                             help="Left right check threshold, used for depth measurement. Default: %(default)s")
         parser.add_argument("-sig", "--sigma", type=_checkRange(0, 250),
                             help="Sigma value for Bilateral Filter applied on depth. Default: %(default)s")
         parser.add_argument("-med", "--stereoMedianSize", type=int, choices=[0, 3, 5, 7],
@@ -176,15 +176,15 @@
                             help="Force USB communication speed. Default: %(default)s")
         # Device after booting
         parser.add_argument("--irDotBrightness", "-laser", "--laser", type=_checkRange(0, 1200),
                             help="For OAK-D Pro: specify IR dot projector brightness, range: 0..1200 [mA], default 0 (turned off)")
         parser.add_argument("--irFloodBrightness", "-led", "--led", type=_checkRange(0, 1500),
                             help="For OAK-D Pro: specify IR flood illumination brightness, range: 0..1500 [mA], default 0 (turned off)")
 
-        args = parser.parse_args()
+        args = parser.parse_known_args()[0]
         # Parse arguments
         args.rgbResolution = rgb_resolution(args.rgbResolution)
         args.monoResolution = mono_resolution(args.monoResolution)
         # Global FPS setting, applied to all cameras
         if args.fps is not None:
             args.rgbFps = args.fps
             args.monoFps = args.fps
```

### Comparing `depthai-sdk-1.9.4.1/src/depthai_sdk/classes/nn_config.py` & `depthai-sdk-1.9.5/src/depthai_sdk/classes/nn_config.py`

 * *Files identical despite different names*

### Comparing `depthai-sdk-1.9.4.1/src/depthai_sdk/classes/nn_results.py` & `depthai-sdk-1.9.5/src/depthai_sdk/classes/nn_results.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 
 
 @dataclass
 class SemanticSegmentation(GenericNNOutput):  # In core, extend from NNData
     """
     Semantic segmentation results, with a mask for each class.
 
-    Examples: `DeeplabV3`, `Lanenet`, `road-semgentation-adas-0001`.
+    Examples: `DeeplabV3`, `Lanenet`, `road-segmentation-adas-0001`.
     """
     mask: List[np.ndarray]  # 2D np.array for each class
 
     def __init__(self, nn_data: NNData, mask: List[np.ndarray]):
         super().__init__(nn_data)
         self.mask = mask
```

### Comparing `depthai-sdk-1.9.4.1/src/depthai_sdk/classes/output_config.py` & `depthai-sdk-1.9.5/src/depthai_sdk/classes/output_config.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,36 +1,36 @@
+import subprocess
 from abc import abstractmethod
 from pathlib import Path
 from typing import Optional, Callable, List
-
 import depthai as dai
 
 from depthai_sdk.classes import FramePacket
 from depthai_sdk.oak_outputs.syncing import SequenceNumSync
 from depthai_sdk.oak_outputs.xout.xout_depth import XoutDepth
 from depthai_sdk.oak_outputs.xout.xout_frames import XoutFrames
 from depthai_sdk.oak_outputs.xout.xout_base import XoutBase
 from depthai_sdk.record import Record
 from depthai_sdk.recorders.video_recorder import VideoRecorder
 from depthai_sdk.visualize.visualizer import Visualizer
+import os
 
 
 class BaseConfig:
     @abstractmethod
     def setup(self, pipeline: dai.Pipeline, device, names: List[str]) -> List[XoutBase]:
         raise NotImplementedError()
 
 
 class OutputConfig(BaseConfig):
     """
     Saves callbacks/visualizers until the device is fully initialized. I'll admit it's not the cleanest solution.
     """
 
-    def __init__(self,
-                 output: Callable,
+    def __init__(self, output: Callable,
                  callback: Callable,
                  visualizer: Visualizer = None,
                  visualizer_enabled: bool = False,
                  record_path: Optional[str] = None):
         self.output = output  # Output of the component (a callback)
         self.callback = callback  # Callback that gets called after syncing
         self.visualizer = visualizer
@@ -92,36 +92,88 @@
 
         self.rec.setup_base(None)
         self.rec.start(device, xouts)
 
         return [self.rec]
 
 
+class RosStreamConfig(BaseConfig):
+    outputs: List[Callable]
+    ros = None
+
+    def __init__(self, outputs: List[Callable]):
+        self.outputs = outputs
+
+    def setup(self, pipeline: dai.Pipeline, device, names: List[str]) -> List[XoutBase]:
+        xouts: List[XoutFrames] = []
+        for output in self.outputs:
+            xoutbase: XoutFrames = output(pipeline, device)
+            xoutbase.setup_base(None)
+            xouts.append(xoutbase)
+
+        envs = os.environ
+        if 'ROS_VERSION' not in envs:
+            raise Exception('ROS installation not found! Please install or source the ROS you would like to use.')
+
+        version = envs['ROS_VERSION']
+        if version == '1':
+            raise Exception('ROS1 publsihing is not yet supported!')
+            from depthai_sdk.integrations.ros.ros1_streaming import Ros1Streaming
+            self.ros = Ros1Streaming()
+        elif version == '2':
+            from depthai_sdk.integrations.ros.ros2_streaming import Ros2Streaming
+            self.ros = Ros2Streaming()
+        else:
+            raise Exception(f"ROS version '{version}' not recognized! Should be either '1' or '2'")
+
+        self.ros.update(device, xouts)
+        return [self]
+
+    def new_msg(self, name, msg):
+        self.ros.new_msg(name, msg)
+    def check_queue(self, block):
+        pass  # No queues
+    def start_fps(self):
+        pass
+
+    # def is_ros1(self) -> bool:
+    #     try:
+    #         import rospy
+    #         return True
+    #     except:
+    #         return False
+    #
+    # def is_ros2(self):
+    #     try:
+    #         import rclpy
+    #         return True
+    #     except:
+    #         return False
+
+
 class SyncConfig(BaseConfig, SequenceNumSync):
     def __init__(self, outputs: List[Callable], callback: Callable):
         self.outputs = outputs
         self.callback = callback
 
         SequenceNumSync.__init__(self, len(outputs))
 
         self.packets = dict()
 
-    def new_packet(self, packet: FramePacket, _=None):
+    def new_packet(self, packet):
         # print('new packet', packet, packet.name, 'seq num',packet.imgFrame.getSequenceNum())
         synced = self.sync(
-            packet.imgFrame.getSequenceNum(),
+            packet.msg.getSequenceNum(),
             packet.name,
             packet
         )
         if synced:
             self.callback(synced)
 
     def setup(self, pipeline: dai.Pipeline, device: dai.Device, _) -> List[XoutBase]:
         xouts = []
         for output in self.outputs:
             xoutbase: XoutBase = output(pipeline, device)
             xoutbase.setup_base(self.new_packet)
             xouts.append(xoutbase)
 
-            xoutbase.setup_visualize(Visualizer(), xoutbase.name)
-
         return xouts
```

### Comparing `depthai-sdk-1.9.4.1/src/depthai_sdk/classes/packets.py` & `depthai-sdk-1.9.5/src/depthai_sdk/classes/packets.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,86 +27,99 @@
 
     def get_bbox(self) -> Tuple[float, float, float, float]:
         return self.img_detection.xmin, self.img_detection.ymin, self.img_detection.xmax, self.img_detection.ymax
 
 
 class _TrackingDetection(_Detection):
     tracklet: dai.Tracklet
+    speed: float = 0.0  # m/s
+    speed_kmph: float = 0.0  # km/h
+    speed_mph: float = 0.0  # mph
 
 
 class _TwoStageDetection(_Detection):
     nn_data: dai.NNData
 
+class NNDataPacket:
+    """
+    Contains only dai.NNData message
+    """
+    name: str  # NNData stream name
+    msg: dai.NNData  # Original depthai message
+
+    def __init__(self, name: str, nn_data: dai.NNData):
+        self.name = name
+        self.msg = nn_data
 
 class FramePacket:
     """
     Contains only dai.ImgFrame message and cv2 frame, which is used by visualization logic.
     """
 
     name: str  # ImgFrame stream name
-    imgFrame: dai.ImgFrame  # Original depthai message
+    msg: dai.ImgFrame  # Original depthai message
     frame: Optional[np.ndarray]  # cv2 frame for visualization
 
     def __init__(self,
                  name: str,
-                 img_frame: dai.ImgFrame,
+                 msg: dai.ImgFrame,
                  frame: Optional[np.ndarray],
                  visualizer: 'Visualizer' = None):
         self.name = name
-        self.imgFrame = img_frame
+        self.msg = msg
         self.frame = frame
         self.visualizer = visualizer
 
 
 class DepthPacket(FramePacket):
     mono_frame: dai.ImgFrame
 
     def __init__(self,
                  name: str,
                  disparity_frame: dai.ImgFrame,
                  mono_frame: dai.ImgFrame,
                  visualizer: 'Visualizer' = None):
         super().__init__(name=name,
-                         img_frame=disparity_frame,
+                         msg=disparity_frame,
                          frame=disparity_frame.getCvFrame() if cv2 else None,
                          visualizer=visualizer)
         self.mono_frame = mono_frame
 
 
 class SpatialBbMappingPacket(FramePacket):
     """
     Output from Spatial Detection nodes - depth frame + bounding box mappings. Inherits FramePacket.
     """
     spatials: dai.SpatialImgDetections
 
     def __init__(self,
                  name: str,
-                 img_frame: dai.ImgFrame,
+                 msg: dai.ImgFrame,
                  spatials: dai.SpatialImgDetections,
                  visualizer: 'Visualizer' = None):
         super().__init__(name=name,
-                         img_frame=img_frame,
-                         frame=img_frame.getFrame() if cv2 else None,
+                         msg=msg,
+                         frame=msg.getFrame() if cv2 else None,
                          visualizer=visualizer)
         self.spatials = spatials
 
 
 class DetectionPacket(FramePacket):
     """
     Output from Detection Network nodes - image frame + image detections. Inherits FramePacket.
     """
 
     def __init__(self,
                  name: str,
-                 img_frame: dai.ImgFrame,
+                 msg: dai.ImgFrame,
                  img_detections: Union[dai.ImgDetections, dai.SpatialImgDetections],
                  visualizer: 'Visualizer' = None):
         super().__init__(name=name,
-                         img_frame=img_frame,
-                         frame=img_frame.getCvFrame() if cv2 else None,
+                         msg=msg,
+                         frame=msg.getCvFrame() if cv2 else None,
                          visualizer=visualizer)
         self.img_detections = img_detections
         self.detections = []
 
     def _is_spatial_detection(self) -> bool:
         return isinstance(self.img_detections, dai.SpatialImgDetections)
 
@@ -123,20 +136,20 @@
 class TrackerPacket(FramePacket):
     """
     Output of Object Tracker node. Tracklets + Image frame. Inherits FramePacket.
     """
 
     def __init__(self,
                  name: str,
-                 img_frame: dai.ImgFrame,
+                 msg: dai.ImgFrame,
                  tracklets: dai.Tracklets,
                  visualizer: 'Visualizer' = None):
         super().__init__(name=name,
-                         img_frame=img_frame,
-                         frame=img_frame.getCvFrame() if cv2 else None,
+                         msg=msg,
+                         frame=msg.getCvFrame() if cv2 else None,
                          visualizer=visualizer)
         self.detections: List[_TrackingDetection] = []
         self.daiTracklets = tracklets
 
     def _add_detection(self, img_det: dai.ImgDetection, bbox: np.ndarray, txt: str, color):
         det = _TrackingDetection()
         det.img_detection = img_det
@@ -159,24 +172,24 @@
 
 class TwoStagePacket(DetectionPacket):
     """
     Output of 2-stage NN pipeline; Image frame, Image detections and multiple NNData results. Inherits DetectionPacket.
     """
 
     def __init__(self, name: str,
-                 img_frame: dai.ImgFrame,
+                 msg: dai.ImgFrame,
                  img_detections: dai.ImgDetections,
                  nn_data: List[dai.NNData],
                  labels: List[int],
                  visualizer: 'Visualizer' = None):
         super().__init__(name=name,
-                         img_frame=img_frame,
+                         msg=msg,
                          img_detections=img_detections,
                          visualizer=visualizer)
-        self.frame = self.imgFrame.getCvFrame() if cv2 else None
+        self.frame = self.msg.getCvFrame() if cv2 else None
         self.nnData = nn_data
         self.labels = labels
         self._cntr = 0
 
     def _add_detection(self, img_det: dai.ImgDetection, bbox: np.ndarray, txt: str, color):
         det = _TwoStageDetection()
         det.img_detection = img_det
```

### Comparing `depthai-sdk-1.9.4.1/src/depthai_sdk/components/camera_component.py` & `depthai-sdk-1.9.5/src/depthai_sdk/components/camera_component.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,26 @@
+import logging
 from typing import Dict
 
+from depthai_sdk.classes.enum import ResizeMode
 from depthai_sdk.components.camera_helper import *
 from depthai_sdk.components.component import Component
 from depthai_sdk.components.parser import parse_resolution, parse_encode, parse_camera_socket
+from depthai_sdk.oak_outputs.xout.xout_base import XoutBase, StreamXout, ReplayStream
+from depthai_sdk.oak_outputs.xout.xout_frames import XoutFrames
 from depthai_sdk.oak_outputs.xout.xout_h26x import XoutH26x
 from depthai_sdk.oak_outputs.xout.xout_mjpeg import XoutMjpeg
-from depthai_sdk.oak_outputs.xout.xout_frames import XoutFrames
-from depthai_sdk.oak_outputs.xout.xout_base import XoutBase, StreamXout, ReplayStream
 from depthai_sdk.replay import Replay
 
 
 class CameraComponent(Component):
     def __init__(self,
+                 device: dai.Device,
                  pipeline: dai.Pipeline,
-                 source: str,
+                 source: Union[str, dai.CameraBoardSocket],
                  resolution: Optional[Union[
                      str, dai.ColorCameraProperties.SensorResolution, dai.MonoCameraProperties.SensorResolution
                  ]] = None,
                  fps: Optional[float] = None,
                  encode: Union[None, str, bool, dai.VideoEncoderProperties.Profile] = None,
                  rotation: Optional[int] = None,
                  replay: Optional[Replay] = None,
@@ -25,207 +28,224 @@
                  args: Dict = None):
         """
         Creates Camera component. This abstracts ColorCamera/MonoCamera nodes and supports mocking the camera when
         recording is passed during OakCamera initialization. Mocking the camera will send frames from the host to the
         OAK device (via XLinkIn node).
 
         Args:
-            source (str): Source of the camera. Either color/rgb/right/left
+            device (dai.Device): OAK device
+            pipeline (dai.Pipeline): OAK pipeline
+            source (str or dai.CameraBoardSocket): Source of the camera. Either color/rgb/right/left
             resolution (optional): Camera resolution, eg. '800p' or '4k'
             fps (float, optional): Camera FPS
             encode: Encode streams before sending them to the host. Either True (use default), or mjpeg/h264/h265
             rotation (int, optional): Rotate the camera by 90, 180, 270 degrees
             replay (Replay object): Replay object to use for mocking the camera
             name (str, optional): Name of the output stream
             args (Dict): Use user defined arguments when constructing the pipeline
         """
         super().__init__()
         self.out = self.Out(self)
 
-        self.node: Optional[Union[dai.node.MonoCamera, dai.node.XLinkIn, dai.node.ColorCamera]] = None
+        self.node: Optional[Union[dai.node.ColorCamera, dai.node.MonoCamera, dai.node.XLinkIn]] = None
         self.encoder: Optional[dai.node.VideoEncoder] = None
+
         self.stream: Optional[dai.Node.Output] = None  # Node output to be used as eg. an input into NN
         self.stream_size: Optional[Tuple[int, int]] = None  # Output size
 
-        # Save passed settings
-        self._pipeline = pipeline
-        self._source = source
-        self._replay: Replay = replay
+        self._source = str(source)
+        self._replay: Optional[Replay] = replay
         self._args: Dict = args
         self.name = name
 
         if rotation not in [None, 0, 90, 180, 270]:
             raise ValueError(f'Angle {rotation} not supported! Use 0, 90, 180, 270.')
 
-        self._rotation = rotation
-
-        self._create_node(self._pipeline, source.upper())
-
-        self.encoder = None
-        if encode:
-            self.encoder = self._pipeline.createVideoEncoder()
-            # MJPEG by default
-            self._encoder_profile = parse_encode(encode)
-
-        self._resolution_forced: bool = resolution is not None
-        if resolution:
-            self._set_resolution(resolution)
-        if fps:
-            self.set_fps(fps)
+        self._num_frames_pool = 10
+        self._preview_num_frames_pool = 4
 
-    def on_init(self, pipeline: dai.Pipeline, device: dai.Device, version: dai.OpenVINO.Version):
-        if self.is_replay():  # If replay, don't create camera node
+        if self.is_replay():
+            if source.casefold() not in list(map(lambda x: x.casefold(), self._replay.getStreams())):
+                raise Exception(f"{source} stream was not found in specified depthai-recording!")
             res = self._replay.getShape(self._source)
             # print('resolution', res)
             # resize = getResize(res, width=1200)
             # self._replay.setResizeColor(resize)
-            self.node: dai.node.XLinkIn = getattr(self._replay, self._source)
+            stream = self._replay.streams[self._source]
+            if stream.node is None:
+                return  # Stream disabled
+
+            self.node = stream.node
             # print('resize', resize)
             self.node.setMaxDataSize(res[0] * res[1] * 3)
             self.stream_size = res
             self.stream = self.node.out
-            if self._rotation:
-                rot_manip = self._create_rotation_manip(pipeline) if self._rotation else None
+
+            if rotation in [90, 180, 270]:
+                rot_manip = self._create_rotation_manip(pipeline, rotation)
                 self.node.out.link(rot_manip.inputImage)
                 self.stream = rot_manip.out
+                if rotation in [90, 270]:
+                    self.stream_size = self.stream_size[::-1]
+        # Livestreaming, not replay
+        else:
+            node_type: dai.node = None
+            if isinstance(source, str):
+                source = source.upper()
+                # When sensors can be either color or mono (eg. AR0234), we allow specifying it
+                if "," in source:  # For sensors that support multiple
+                    parts = source.split(',')
+                    source = parts[0]
+                    if parts[1] in ["C", "COLOR"]:
+                        node_type = dai.node.ColorCamera
+                    elif parts[1] in ["M", "MONO"]:
+                        node_type = dai.node.MonoCamera
+                    else:
+                        raise Exception(
+                            "Please specify sensor type with c/color or m/mono after the ','"
+                            " - eg. `cam = oak.create_camera('cama,c')`"
+                        )
+
+            socket = parse_camera_socket(source)
+            sensor = [f for f in device.getConnectedCameraFeatures() if f.socket == socket][0]
+
+            if node_type is not None:  # User specified camera type
+                if node_type == dai.node.ColorCamera and dai.CameraSensorType.COLOR not in sensor.supportedTypes:
+                    raise Exception(
+                        f"User specified {node_type} node, but {sensor.sensorName} sensor doesn't support COLOR mode!"
+                    )
+                if node_type == dai.node.MonoCamera and dai.CameraSensorType.MONO not in sensor.supportedTypes:
+                    raise Exception(
+                        f"User specified {node_type} node, but {sensor.sensorName} sensor doesn't support MONO mode!"
+                    )
             else:
-                self.stream = self.node.out
+                type = sensor.supportedTypes[0]
+                if type == dai.CameraSensorType.COLOR:
+                    node_type = dai.node.ColorCamera
+                elif type == dai.CameraSensorType.MONO:
+                    node_type = dai.node.MonoCamera
+                else:
+                    raise Exception(f"{sensor} doesn't support either COLOR or MONO ")
+
+            # Create the node, and set the socket
+            self.node = pipeline.create(node_type)
+            self.node.setBoardSocket(socket)
 
+        self._resolution_forced: bool = resolution is not None
+        if resolution:
+            self._set_resolution(resolution)
+        if fps:
+            self.set_fps(fps)
+
+        # Default configuration for the nodes
         if isinstance(self.node, dai.node.ColorCamera):
             # DepthAI uses CHW (Planar) channel layout convention for NN inferencing
             self.node.setInterleaved(False)
             # DepthAI uses BGR color order convention for NN inferencing
             self.node.setColorOrder(dai.ColorCameraProperties.ColorOrder.BGR)
-            self.node.setPreviewNumFramesPool(4)
-
-            cams = device.getCameraSensorNames()
-            # print('Available sensors on OAK:', cams)
-            sensor_name = cams[dai.CameraBoardSocket.RGB]
+            self.node.setPreviewNumFramesPool(self._preview_num_frames_pool)
 
             if not self._resolution_forced:  # Find the closest resolution
-                self.node.setResolution(getClosesResolution(sensor_name, width=1300))
+                sensor = [f for f in device.getConnectedCameraFeatures() if f.socket == self.node.getBoardSocket()][0]
+                sensor_type = dai.CameraSensorType.COLOR if dai.node.ColorCamera else dai.CameraSensorType.MONO
+                res = getClosesResolution(sensor, sensor_type, width=1300)
+                self.node.setResolution(res)
                 scale = getClosestIspScale(self.node.getIspSize(), width=1300, videoEncoder=(self.encoder is not None))
                 self.node.setIspScale(*scale)
 
             curr_size = self.node.getVideoSize()
             closest = getClosestVideoSize(*curr_size)
             self.node.setVideoSize(*closest)
             self.node.setVideoNumFramesPool(2)  # We will increase it later if we are streaming to host
 
             self.node.setPreviewSize(*self.node.getVideoSize())
             self.stream_size = self.node.getPreviewSize()
-            self.stream = self.node.preview if self.encoder is None else self.node.video
+            self.stream = self.node.preview
 
         elif isinstance(self.node, dai.node.MonoCamera):
             self.stream_size = self.node.getResolutionSize()
             self.stream = self.node.out
 
-        if self._args:
-            self._config_camera_args(self._args)
-
-        if self._rotation:
-            rot_manip = self._create_rotation_manip(pipeline) if self._rotation else None
-            self.stream.link(rot_manip.inputImage)
-            self.stream = rot_manip.out
+        if rotation and not self.is_replay():
+            if rotation == 180:
+                self.node.setImageOrientation(dai.CameraImageOrientation.ROTATE_180_DEG)
+            else:
+                rot_manip = self._create_rotation_manip(pipeline, rotation)
+                self.stream.link(rot_manip.inputImage)
+                self.stream = rot_manip.out
+                self.stream_size = self.stream_size[::-1]
 
-        if self.encoder:
+        if encode:
+            self.encoder = pipeline.createVideoEncoder()
+            self._encoder_profile = parse_encode(encode)  # MJPEG by default
             self.encoder.setDefaultProfilePreset(self.get_fps(), self._encoder_profile)
+
             if self.is_replay():  # TODO - this might be not needed, we check for replay above and return
                 # Create ImageManip to convert to NV12
                 type_manip = pipeline.createImageManip()
                 type_manip.setFrameType(dai.ImgFrame.Type.NV12)
                 type_manip.setMaxOutputFrameSize(self.stream_size[0] * self.stream_size[1] * 3)
 
                 self.stream.link(type_manip.inputImage)
                 type_manip.out.link(self.encoder.input)
             elif self.is_mono():
                 self.stream.link(self.encoder.input)
             elif self.is_color():
-                self.stream.link(self.encoder.input)
+                self.node.video.link(self.encoder.input)
             else:
                 raise ValueError('CameraComponent is neither Color, Mono, nor Replay!')
 
-    def _create_rotation_manip(self, pipeline: dai.Pipeline):
+        if self._args:
+            self._config_camera_args(self._args)
+
+    def _create_rotation_manip(self, pipeline: dai.Pipeline, rotation: int):
         rot_manip = pipeline.createImageManip()
         rgb_rr = dai.RotatedRect()
         w, h = self.stream_size
         rgb_rr.center.x, rgb_rr.center.y = w // 2, h // 2
-        rgb_rr.size.width, rgb_rr.size.height = (w, h) if self._rotation % 180 == 0 else (h, w)
-        rgb_rr.angle = self._rotation
+        rgb_rr.size.width, rgb_rr.size.height = (w, h) if rotation % 180 == 0 else (h, w)
+        rgb_rr.angle = rotation
         rot_manip.initialConfig.setCropRotatedRect(rgb_rr, False)
         rot_manip.setMaxOutputFrameSize(w * h * 3)
         return rot_manip
 
-    def _create_node(self, pipeline: dai.Pipeline, source: str) -> None:
-        """
-        Called from __init__ to parse passed `source` argument.
-        @param source: User-input source
-        """
-        if "," in source:  # For OAK FFC cameras, so you can eg. specify "rgb,c" as source
-            parts = source.split(',')
-            source = parts[0]
-
-            if parts[1] in ["C", "COLOR"]:
-                self.node = pipeline.createColorCamera()
-            elif parts[1] in ["M", "MONO"]:
-                self.node = pipeline.createMonoCamera()
-
-            self.node.setBoardSocket(parse_camera_socket(source))
-            return
-
-        if self.is_replay():
-            if source.casefold() not in list(map(lambda x: x.casefold(), self._replay.getStreams())):
-                raise Exception(f"{source} stream was not found in specified depthai-recording!")
-            return
-
-        socket = parse_camera_socket(source)
-        # By default, we will assume color camera is connected to CAM_A,
-        # while 2x stereo cameras are connected to CAM_B and CAM_C
-        if socket == dai.CameraBoardSocket.CAM_A:
-            self.node = pipeline.createColorCamera()
-        elif socket in [dai.CameraBoardSocket.CAM_B, dai.CameraBoardSocket.CAM_C]:
-            self.node = pipeline.createMonoCamera()
-        else:
-            raise Exception(
-                "When specifying other camera sockets, you need to specify whether it's color or mono camera!"
-                "You can do this with eg. `cam_d,c` for color camera, or `cam_d,m` for mono camera."
-            )
-
-        self.node.setBoardSocket(socket)
-
     # Should be mono/color camera agnostic. Also call this from __init__ if args is enabled
     def config_camera(self,
                       # preview: Union[None, str, Tuple[int, int]] = None,
+                      size: Union[None, Tuple[int, int], str] = None,
+                      resize_mode: ResizeMode = ResizeMode.CROP,
                       fps: Optional[float] = None,
                       resolution: Optional[Union[
                           str, dai.ColorCameraProperties.SensorResolution, dai.MonoCameraProperties.SensorResolution
                       ]] = None
                       ) -> None:
         """
         Configure resolution, scale, FPS, etc.
         """
 
         # TODO
         if fps: self.set_fps(fps)
         if resolution: self._set_resolution(resolution)
 
-        # if preview:
-        #     from .parser import parse_size
-        #     preview = parse_size(preview)
-        #
-        #     self.stream_size = preview
-        #
-        #     if self._replay:
-        #         self._replay.setResizeColor(preview)
-        #     elif self.is_color():
-        #         self.node.setPreviewSize(preview)
-        #     else:
-        #         # TODO: Use ImageManip to set mono frame size
-        #
-        #         raise NotImplementedError("Not yet implemented")
+        if size:
+            from .parser import parse_size
+            size_tuple = parse_size(size)
+
+            if self._replay:
+                self._replay.resize(self._source, size_tuple, resize_mode)
+            elif self.is_color():
+                self.node.setStillSize(*size_tuple)
+                self.node.setVideoSize(*size_tuple)
+                self.node.setPreviewSize(*size_tuple)
+                if resize_mode != ResizeMode.CROP:
+                    raise ValueError("Currently only ResizeMode.CROP is supported mode for specifying size!")
+            else:
+                # TODO: Use ImageManip to set mono frame size
+
+                raise NotImplementedError("Not yet implemented")
 
     def _config_camera_args(self, args: Dict):
         if not isinstance(args, Dict):
             args = vars(args)  # Namespace -> Dict
 
         if self.is_color():
             self.config_camera(
@@ -249,15 +269,14 @@
                 fps=args.get('monoFps', None),
                 resolution=args.get('monoResolution', None),
             )
         else:  # Replay
             self.config_camera(fps=args.get('fps', None))
 
     def config_color_camera(self,
-                            size: Optional[Tuple[int, int]] = None,
                             interleaved: Optional[bool] = None,
                             color_order: Union[None, dai.ColorCameraProperties.ColorOrder, str] = None,
                             # Cam control
                             manual_focus: Optional[int] = None,
                             af_mode: Optional[dai.CameraControl.AutoFocusMode] = None,
                             awb_mode: Optional[dai.CameraControl.AutoWhiteBalanceMode] = None,
                             scene_mode: Optional[dai.CameraControl.SceneMode] = None,
@@ -266,47 +285,44 @@
                             # IQ settings
                             isp_scale: Optional[Tuple[int, int]] = None,
                             sharpness: Optional[int] = None,
                             luma_denoise: Optional[int] = None,
                             chroma_denoise: Optional[int] = None,
                             ) -> None:
         if not self.is_color():
-            print("Attempted to configure ColorCamera, but this component doesn't have it. Config attempt ignored.")
+            logging.info(
+                'Attempted to configure ColorCamera, but this component doesn\'t have it. Config attempt ignored.'
+            )
             return
 
-        if self._replay is not None:
-            print('Tried configuring ColorCamera, but replaying is enabled. Config attempt ignored.')
+        if self.is_replay():
+            logging.info('Tried configuring ColorCamera, but replaying is enabled. Config attempt ignored.')
             return
 
         self.node: dai.node.ColorCamera
 
-        if size:
-            self.node.setStillSize(*size)
-            self.node.setVideoSize(*size)
-            self.node.setPreviewSize(*size)
-
-        if interleaved: self.node.setInterleaved(interleaved)
+        if interleaved is not None: self.node.setInterleaved(interleaved)
         if color_order:
             if isinstance(color_order, str):
                 color_order = getattr(dai.ColorCameraProperties.ColorOrder, color_order.upper())
             self.node.setColorOrder(color_order)
 
-        if manual_focus: self.node.initialControl.setManualFocus(manual_focus)
+        if manual_focus is not None: self.node.initialControl.setManualFocus(manual_focus)
         if af_mode: self.node.initialControl.setAutoFocusMode(af_mode)
         if awb_mode: self.node.initialControl.setAutoWhiteBalanceMode(awb_mode)
         if scene_mode: self.node.initialControl.setSceneMode(scene_mode)
         if anti_banding_mode: self.node.initialControl.setAntiBandingMode(anti_banding_mode)
         if effect_mode: self.node.initialControl.setEffectMode(effect_mode)
         # EQ settings
         if isp_scale:
             self._resolution_forced = True
             self.node.setIspScale(*isp_scale)
-        if sharpness: self.node.initialControl.setSharpness(sharpness)
-        if luma_denoise: self.node.initialControl.setLumaDenoise(luma_denoise)
-        if chroma_denoise: self.node.initialControl.setChromaDenoise(chroma_denoise)
+        if sharpness is not None: self.node.initialControl.setSharpness(sharpness)
+        if luma_denoise is not None: self.node.initialControl.setLumaDenoise(luma_denoise)
+        if chroma_denoise is not None: self.node.initialControl.setChromaDenoise(chroma_denoise)
 
     def _set_resolution(self, resolution):
         if not self.is_replay():
             self.node.setResolution(parse_resolution(type(self.node), resolution))
         # TODO: support potentially downscaling depthai-recording
 
     def is_replay(self) -> bool:
@@ -314,64 +330,84 @@
 
     def is_color(self) -> bool:
         return isinstance(self.node, dai.node.ColorCamera)
 
     def is_mono(self) -> bool:
         return isinstance(self.node, dai.node.MonoCamera)
 
-    def get_fps(self):
-        return (self._replay if self.is_replay() else self.node).getFps()
+    def get_fps(self) -> float:
+        if self.is_replay():
+            return self._replay.get_fps()
+        else:
+            return self.node.getFps()
 
     def set_fps(self, fps: float):
-        (self._replay if self._replay else self.node).setFps(fps)
+        if self.is_replay():
+            self._replay.set_fps(fps)
+        else:
+            self.node.setFps(fps)
 
     def config_encoder_h26x(self,
                             rate_control_mode: Optional[dai.VideoEncoderProperties.RateControlMode] = None,
                             keyframe_freq: Optional[int] = None,
                             bitrate_kbps: Optional[int] = None,
                             num_b_frames: Optional[int] = None,
                             ):
         if self.encoder is None:
             raise Exception('Video encoder was not enabled!')
         if self._encoder_profile == dai.VideoEncoderProperties.Profile.MJPEG:
             raise Exception('Video encoder was set to MJPEG while trying to configure H26X attributes!')
 
-        if rate_control_mode:
+        if rate_control_mode is not None:
             self.encoder.setRateControlMode(rate_control_mode)
-        if keyframe_freq:
+        if keyframe_freq is not None:
             self.encoder.setKeyframeFrequency(keyframe_freq)
-        if bitrate_kbps:
+        if bitrate_kbps is not None:
             self.encoder.setBitrateKbps(bitrate_kbps)
-        if num_b_frames:
+        if num_b_frames is not None:
             self.encoder.setNumBFrames(num_b_frames)
 
     def config_encoder_mjpeg(self,
                              quality: Optional[int] = None,
                              lossless: bool = False
                              ):
         if self.encoder is None:
             raise Exception('Video encoder was not enabled!')
         if self._encoder_profile != dai.VideoEncoderProperties.Profile.MJPEG:
             raise Exception(
                 f'Video encoder was set to {self._encoder_profile} while trying to configure MJPEG attributes!'
             )
 
-        if quality:
+        if quality is not None:
             self.encoder.setQuality(quality)
-        if lossless:
+        if lossless is not None:
             self.encoder.setLossless(lossless)
 
     def get_stream_xout(self) -> StreamXout:
         if self.is_replay():
             return ReplayStream(self._source)
         elif self.is_mono():
             return StreamXout(self.node.id, self.stream, name=self.name)
         else:  # ColorCamera
-            self.node.setVideoNumFramesPool(10)
-            return StreamXout(self.node.id, self.stream, name=self.name)
+            self.node.setVideoNumFramesPool(self._num_frames_pool)
+            # node.video instead of preview (self.stream) was used to reduce bandwidth
+            # consumption by 2 (3bytes/pixel vs 1.5bytes/pixel)
+            return StreamXout(self.node.id, self.node.video, name=self.name)
+
+    def set_num_frames_pool(self, num_frames: int, preview_num_frames: Optional[int] = None):
+        """
+        Set the number of frames to be stored in the pool.
+
+        :param num_frames: Number of frames to be stored in the pool.
+        :param preview_num_frames: Number of frames to be stored in the pool for the preview stream.
+        """
+        if self.is_color():
+            self._num_frames_pool = num_frames
+            if preview_num_frames is not None:
+                self._preview_num_frames_pool = preview_num_frames
 
     """
     Available outputs (to the host) of this component
     """
 
     class Out:
         def __init__(self, camera_component: 'CameraComponent'):
```

### Comparing `depthai-sdk-1.9.4.1/src/depthai_sdk/components/camera_helper.py` & `depthai-sdk-1.9.5/src/depthai_sdk/components/camera_helper.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,65 +1,39 @@
 import math
 import depthai as dai
 from typing import *
+import numpy as np
+import cv2
 
 
-class ImageSensor:
-    name: str
-    resolutions: List[Union[
-        dai.ColorCameraProperties.SensorResolution,
-        dai.MonoCameraProperties.SensorResolution
-    ]]
-    type: dai.node
-
-    def __eq__(self, other):
-        return self.name == other
-
-    def __init__(self,
-                 name: str,
-                 resolutions: List[str],
-                 type: str):
-        from .parser import parse_resolution
-        self.name = name
-        self.type = dai.node.ColorCamera if type == 'color' else dai.node.MonoCamera
-        self.resolutions = [parse_resolution(self.type, resolution) for resolution in resolutions]
-
-    @property
-    def maxRes(self) -> Union[dai.ColorCameraProperties.SensorResolution, dai.MonoCameraProperties.SensorResolution]:
-        return self.resolutions[0]
-
-
-cameraSensors: List[ImageSensor] = [
-    ImageSensor('IMX378', ['12mp', '4k', '1080p'], 'color'),
-    ImageSensor('OV9282', ['800P', '720p', '400p'], 'mono'),
-    ImageSensor('OV9782', ['800P', '720p', '400p'], 'color'),
-    ImageSensor('OV9281', ['800P', '720p', '400p'], 'color'),
-    ImageSensor('IMX214', ['13mp', '12mp', '4k', '1080p'], 'color'),
-    ImageSensor('OV7750', ['480P', '400p'], 'mono'),
-    ImageSensor('OV7251', ['480P', '400p'], 'mono'),
-    ImageSensor('IMX477', ['12mp', '4k', '1080p'], 'color'),
-    ImageSensor('IMX577', ['12mp', '4k', '1080p'], 'color'),
-    ImageSensor('AR0234', ['1200P'], 'color'),
-    ImageSensor('IMX582', ['48mp', '12mp', '4k'], 'color'),
-]
-
-cameraResolutions: Dict[Any, Tuple[int, int]] = {
-    dai.ColorCameraProperties.SensorResolution.THE_13_MP: (4208, 3120),
-    dai.ColorCameraProperties.SensorResolution.THE_12_MP: (4056, 3040),
+monoResolutions: Dict[dai.MonoCameraProperties.SensorResolution, Tuple[int,int]] = {
+    dai.MonoCameraProperties.SensorResolution.THE_1200_P: (1920, 1200), # Monochrome AR0234
+    dai.MonoCameraProperties.SensorResolution.THE_800_P: (1280, 800), # OV9282
+    dai.MonoCameraProperties.SensorResolution.THE_720_P: (1280, 720),
+    dai.MonoCameraProperties.SensorResolution.THE_480_P: (640, 480), # OV7251
+    dai.MonoCameraProperties.SensorResolution.THE_400_P: (640, 400),
+}
+
+colorResolutions: Dict[dai.ColorCameraProperties.SensorResolution, Tuple[int,int]] = {
+    dai.ColorCameraProperties.SensorResolution.THE_5312X6000: (5312, 6000),  # IMX582 cropped
+    dai.ColorCameraProperties.SensorResolution.THE_13_MP: (4208, 3120),  # AR214
+    dai.ColorCameraProperties.SensorResolution.THE_12_MP: (4056, 3040),  # IMX378, IMX477, IMX577
+    dai.ColorCameraProperties.SensorResolution.THE_4000X3000: (4000, 3000),  # IMX582 with binning enabled
     dai.ColorCameraProperties.SensorResolution.THE_4_K: (3840, 2160),
+    dai.ColorCameraProperties.SensorResolution.THE_1200_P: (1920, 1200),  # AR0234
     dai.ColorCameraProperties.SensorResolution.THE_1080_P: (1920, 1080),
-    dai.ColorCameraProperties.SensorResolution.THE_800_P: (1280, 800),
+    dai.ColorCameraProperties.SensorResolution.THE_1440X1080: (1440, 1080),
+    dai.ColorCameraProperties.SensorResolution.THE_5_MP: (2592, 1944),  # OV5645
+    dai.ColorCameraProperties.SensorResolution.THE_800_P: (1280, 800),  # OV9782
     dai.ColorCameraProperties.SensorResolution.THE_720_P: (1280, 720),
-
-    dai.MonoCameraProperties.SensorResolution.THE_800_P: (1280, 800),
-    dai.MonoCameraProperties.SensorResolution.THE_720_P: (1280, 720),
-    dai.MonoCameraProperties.SensorResolution.THE_480_P: (640, 480),
-    dai.MonoCameraProperties.SensorResolution.THE_400_P: (640, 400),
 }
 
+sensorResolutions: Dict[Any, Tuple[int,int]] = []
+sensorResolutions.extend(monoResolutions)
+sensorResolutions.extend(colorResolutions)
 
 def availableIspScales() -> List[Tuple[int, Tuple[int, int]]]:
     """
     Calculates all supported
     @rtype: List[ratio, [Numerator, Denominator]]
     """
     lst = []
@@ -69,15 +43,14 @@
             if d < 32 or n % 2 == 0:
                 # Only if irreducible
                 if math.gcd(n, d) == 1:
                     lst.append((n / d, (n, d)))
     lst.sort(reverse=True)
     return lst
 
-
 def getClosestVideoSize(width: int, height: int, videoEncoder: bool=False) -> Tuple[int, int]:
     """
     For colorCamera.video output
     """
     while True:
         if width % 2 == 0: # YUV420/NV12 width needs to be an even number to be convertible to BGR on host using cv2
             if not videoEncoder or width % 32 == 0: # VideoEncoder HW limitation - width must be divisible by 32
@@ -189,56 +162,43 @@
         control.setLumaDenoise(lumaDenoise)
     if chromaDenoise is not None:
         control.setChromaDenoise(chromaDenoise)
 
     # TODO: Add contrast, exposure compensation, brightness, manual exposure, and saturation
 
 
-def cameraSensor(sensorName: str) -> ImageSensor:
-    return cameraSensors[cameraSensors.index(sensorName.upper())]
-
+def get_sensor_resolution(type: dai.CameraSensorType, width: int, height: int) -> Tuple[Union[dai.ColorCameraProperties.SensorResolution, dai.MonoCameraProperties.SensorResolution], Tuple[int,int]]:
+    def get_res(resolutions: Dict[Any, Tuple[int,int]]):
+        for res, (w, h) in resolutions.items():
+            if width == w and height == h:
+                return (res, (w,h))
+
+    if type == dai.CameraSensorType.COLOR:
+        return get_res(colorResolutions)
+    elif type == dai.CameraSensorType.MONO:
+        return get_res(monoResolutions)
+    else:
+        raise Exception('Camera sensor type unknown!', type)
 
-def cameraSensorType(sensorName: str) -> dai.node:
-    """
-    Gets camera sensor type from it's name, either MonoCamera or ColorCamera.
-    @param sensorName: Name of the camera sensor
-    @return: dai.node.MonoCamera or dai.node.ColorCamera
-    """
-    return cameraSensor(sensorName).type
-
-
-def cameraSensorResolution(sensorName: str
-                           ) -> Union[
-    dai.ColorCameraProperties.SensorResolution, dai.MonoCameraProperties.SensorResolution]:
-    """
-    Gets camera sensor type from it's name, either MonoCamera or ColorCamera.
-    @param sensorName: Name of the camera sensor
-    @return: dai.node.MonoCamera or dai.node.ColorCamera
-    """
-    return cameraSensor(sensorName).maxRes
-
-
-def cameraSensorResolutionSize(sensorName: str) -> Tuple[int, int]:
-    res = cameraSensorResolution(sensorName)
-    return cameraResolutions[res]
-
-
-def getClosesResolution(sensorName: str,
+def getClosesResolution(sensor: dai.CameraFeatures,
+                        type: dai.CameraSensorType,
                         width: Optional[int] = None,
                         height: Optional[int] = None, ):
     if width and height:
         raise ValueError("You have to specify EITHER width OR height to calculate desired ISP scaling options!")
     if not width and not height:
         raise ValueError("You have to provide width or height calculate desired ISP scaling options!")
 
     minError = 99999
     closestRes = None
     desired, i = (width, 0) if width else (height, 1)
-    for res in cameraSensor(sensorName).resolutions:
-        size = cameraResolutions[res]
+
+    resolutions = [get_sensor_resolution(type, conf.width, conf.height) for conf in sensor.configs if conf.type == type]
+
+    for (res, size) in resolutions:
         err = abs(size[i] - desired)
         if err < minError:
             minError = err
             closestRes = res
     return closestRes
```

### Comparing `depthai-sdk-1.9.4.1/src/depthai_sdk/components/component.py` & `depthai-sdk-1.9.5/src/depthai_sdk/components/component.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,21 +15,14 @@
         """
         Checks whether the component forces a specific OpenVINO version. Only used by NNComponent (which overrides this
         method). This function is called after Camera has been configured and right before we connect to the OAK camera.
         @return: Forced OpenVINO version (optional).
         """
         return None
 
-    @abstractmethod
-    def on_init(self, pipeline: dai.Pipeline, device: dai.Device, version: dai.OpenVINO.Version):
-        """
-        This function will be called after the app connects to the Device
-        """
-        raise NotImplementedError("Every component needs to include 'updateDeviceInfo()' method!")
-
     def _stream_name_ok(self, pipeline: dai.Pipeline, name: str) -> bool:
         # Check if there's already an XLinkOut stream with this name
         for node in pipeline.getAllNodes():
             if isinstance(node, dai.node.XLinkOut) and node.getStreamName() == name:
                 return False
         return True
```

### Comparing `depthai-sdk-1.9.4.1/src/depthai_sdk/components/imu_component.py` & `depthai-sdk-1.9.5/src/depthai_sdk/components/imu_component.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,17 @@
 
 from depthai_sdk.components.component import Component, XoutBase
 from depthai_sdk.oak_outputs.xout.xout_base import StreamXout
 from depthai_sdk.oak_outputs.xout.xout_imu import XoutIMU
 
 
 class IMUComponent(Component):
-    def __init__(self, pipeline: dai.Pipeline):
+    def __init__(self,
+                 device: dai.Device,
+                 pipeline: dai.Pipeline):
         self.out = self.Out(self)
 
         super().__init__()
         self.node = pipeline.createIMU()
         self.config_imu()  # Default settings, component won't work without them
 
     def config_imu(self,
@@ -39,17 +41,14 @@
         # TODO: check whether we have IMU (and which sensors are supported) once API supports it
 
         self.node.enableIMUSensor(sensors=sensors, reportRate=report_rate)
         self.node.setBatchReportThreshold(batchReportThreshold=batch_report_threshold)
         self.node.setMaxBatchReports(maxBatchReports=max_batch_reports)
         self.node.enableFirmwareUpdate(enable_firmware_update)
 
-    def on_init(self, pipeline: dai.Pipeline, device: dai.Device, version: dai.OpenVINO.Version):
-        pass
-
     class Out:
         def __init__(self, imu_component: 'IMUComponent'):
             self._comp = imu_component
 
         def main(self, pipeline: dai.Pipeline, device: dai.Device) -> XoutBase:
             """
             Default output. Uses either camera(), replay(), or encoded() depending on the component settings.
```

### Comparing `depthai-sdk-1.9.4.1/src/depthai_sdk/components/integrations/roboflow.py` & `depthai-sdk-1.9.5/src/depthai_sdk/integrations/roboflow.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,19 @@
-from typing import Dict, List
-import requests
-import depthai as dai
-from pathlib import Path
 import json
+import logging
+from pathlib import Path
+from typing import Dict
 from zipfile import ZipFile
 
+import depthai as dai
+import requests
+
 ROBOFLOW_MODELS = Path.home() / Path('.cache/roboflow-models')
 
+
 class RoboflowIntegration:
     def __init__(self, config: Dict):
         if 'key' not in config:
             raise ValueError("To download a model from Roboflow, you need to pass API key ('key')!")
         if 'model' not in config:
             raise ValueError("To download a model from Roboflow, you need to pass model path ('model')!")
 
@@ -23,15 +26,15 @@
         return files[0]
 
     def device_update(self, device: dai.Device) -> Path:
         mxid = device.getMxId()
         url = f"https://api.roboflow.com/depthai/{self.config['model']}/?api_key={self.config['key']}&device={mxid}"
         response = requests.get(url)
 
-        name = self.config['model'].replace('/', '_') # '/' isn't valid folder name
+        name = self.config['model'].replace('/', '_')  # '/' isn't valid folder name
 
         model_folder = ROBOFLOW_MODELS / name
         jsonFile = self._file_with_ext(model_folder, '.json')
         if jsonFile:
             return jsonFile
 
         json_res = response.json()
@@ -41,30 +44,30 @@
         response.raise_for_status()
         ret = json_res['depthai']
 
         if not str(ret['modelType']).startswith('yolov'):
             raise ValueError("This Roboflow's model is not from YOLO family!")
 
         if not str(ret['modelType']).endswith('n'):
-            print('We recommend using a lighter version of the model to get a better performance!')
+            logging.info('We recommend using a lighter version of the model to get a better performance!')
 
-        print(f"Downloading '{ret['name']}' model from Roboflow server")
+        logging.info(f"Downloading '{ret['name']}' model from Roboflow server")
 
         zipFileReq = requests.get(ret['model'])
         zipFileReq.raise_for_status()
 
         (ROBOFLOW_MODELS / name).mkdir(parents=True, exist_ok=True)
         zipFilePath = str(ROBOFLOW_MODELS / 'roboflow.zip')
         # Download the .zip where our model is
         with open(zipFilePath, 'wb') as f:
             f.write(zipFileReq.content)
 
-        print(f"Downloaded the model to {zipFilePath}")
+        logging.info(f"Downloaded the model to {zipFilePath}")
 
-        with ZipFile(zipFilePath, 'r') as zObject: # Extract the zip
+        with ZipFile(zipFilePath, 'r') as zObject:  # Extract the zip
             zObject.extractall(str(ROBOFLOW_MODELS / name))
 
         # Rename bin/xml files
         self._file_with_ext(model_folder, ".xml").rename(str(model_folder / (name + ".xml")))
         self._file_with_ext(model_folder, ".bin").rename(str(model_folder / (name + ".bin")))
 
         # Rename bin/xml paths inside the json
```

### Comparing `depthai-sdk-1.9.4.1/src/depthai_sdk/components/multi_stage_nn.py` & `depthai-sdk-1.9.5/src/depthai_sdk/components/multi_stage_nn.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,38 +20,40 @@
 
 class MultiStageNN:
     def __init__(self,
                  pipeline: dai.Pipeline,
                  detection_node: GenericNeuralNetwork,  # Object detection node
                  high_res_frames: dai.Node.Output,
                  size: Tuple[int, int],
-                 debug=False
+                 debug=False,
+                 num_frames_pool: int = 20
                  ) -> None:
         """
         Args:
             pipeline (dai.Pipeline): Pipeline object
             detection_node (GenericNeuralNetwork): Object detection NN
             high_res_frames (dai.Node.Output): Frames corresponding to the detection NN
             size (Tuple[int, int]): Size of the frames.
             debug (bool, optional): Enable debug mode. Defaults to False.
+            num_frames_pool (int, optional): Number of frames to keep in the pool. Defaults to 20.
         """
         self.script: dai.node.Script = pipeline.create(dai.node.Script)
         self.script.setProcessor(dai.ProcessorType.LEON_CSS)  # More stable
         self._size: Tuple[int, int] = size
 
         detection_node.out.link(self.script.inputs['detections'])
         high_res_frames.link(self.script.inputs['frames'])
 
         self.configure(MultiStageConfig(debug))
 
         self.manip: dai.node.ImageManip = pipeline.create(dai.node.ImageManip)
         self.manip.initialConfig.setResize(size)
         self.manip.setWaitForConfigInput(True)
         self.manip.setMaxOutputFrameSize(size[0] * size[1] * 3)
-        self.manip.setNumFramesPool(20)
+        self.manip.setNumFramesPool(num_frames_pool)
         self.script.outputs['manip_cfg'].link(self.manip.inputConfig)
         self.script.outputs['manip_img'].link(self.manip.inputImage)
         self.out: dai.Node.Output = self.manip.out
 
     def configure(self, config: MultiStageConfig = None) -> None:
         """
         Args:
```

### Comparing `depthai-sdk-1.9.4.1/src/depthai_sdk/components/nn_component.py` & `depthai-sdk-1.9.5/src/depthai_sdk/components/nn_component.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,38 +1,41 @@
 import json
+import logging
 import warnings
 from pathlib import Path
 from typing import Callable, Union, List, Dict
 
 try:
     import blobconverter
 except ImportError:
     blobconverter = None
 
 from depthai_sdk.classes.nn_config import Config
 from depthai_sdk.components.camera_component import CameraComponent
 from depthai_sdk.components.component import Component
-from depthai_sdk.components.integrations.roboflow import RoboflowIntegration
+from depthai_sdk.integrations.roboflow import RoboflowIntegration
 from depthai_sdk.components.multi_stage_nn import MultiStageNN, MultiStageConfig
 from depthai_sdk.components.nn_helper import *
+from depthai_sdk.classes.enum import ResizeMode
 from depthai_sdk.components.parser import *
 from depthai_sdk.components.stereo_component import StereoComponent
 from depthai_sdk.oak_outputs.xout.xout_base import StreamXout, XoutBase
 from depthai_sdk.oak_outputs.xout.xout_frames import XoutFrames
-from depthai_sdk.oak_outputs.xout.xout_nn import XoutTwoStage, XoutNnResults, XoutSpatialBbMappings
+from depthai_sdk.oak_outputs.xout.xout_nn import XoutTwoStage, XoutNnResults, XoutSpatialBbMappings, XoutNnData
 from depthai_sdk.oak_outputs.xout.xout_nn_encoded import XoutNnMjpeg, XoutNnH26x
 from depthai_sdk.oak_outputs.xout.xout_tracker import XoutTracker
 from depthai_sdk.replay import Replay
 
 
 class NNComponent(Component):
     def __init__(self,
+                 device: dai.Device,
                  pipeline: dai.Pipeline,
                  model: Union[str, Path, Dict],  # str for SDK supported model or Path to custom model's json
-                 input: Union[CameraComponent, 'NNComponent'],
+                 input: Union[CameraComponent, 'NNComponent', dai.Node.Output],
                  nn_type: Optional[str] = None,  # Either 'yolo' or 'mobilenet'
                  decode_fn: Optional[Callable] = None,
                  tracker: bool = False,  # Enable object tracker - only for Object detection models
                  spatial: Union[None, bool, StereoComponent] = None,
                  replay: Optional[Replay] = None,
                  args: Dict = None,  # User defined args
                  name: Optional[str] = None
@@ -42,95 +45,84 @@
          - DepthAI API nodes: NeuralNetwork, *DetectionNetwork, *SpatialDetectionNetwork, ObjectTracker
          - Downloading NN models (supported SDK NNs), parsing NN json configs and setting up the pipeline based on it
          - Decoding NN results
          - MultiStage pipelines - cropping high-res frames based on detections and use them for second NN inferencing
 
         Args:
             model (Union[str, Path, Dict]): str for SDK supported model / Path to blob or custom model's json
-            input: (Union[Component, dai.Node.Output]): Input to the NN. If nn_component that is object detector, crop HQ frame at detections (Script node + ImageManip node)
+            input: (Union[Component, dai.Node.Output, dai.Node.Output]): Input to the NN. If nn_component that is object detector, crop HQ frame at detections (Script node + ImageManip node)
             nn_type (str, optional): Type of the NN - Either 'Yolo' or 'MobileNet'
             tracker (bool, default False): Enable object tracker - only for Object detection models
             spatial (bool, default False): Enable getting Spatial coordinates (XYZ), only for Obj detectors. Yolo/SSD use on-device spatial calc, others on-host (gen2-calc-spatials-on-host)
             replay (Replay object): Replay
             args (Any, optional): Use user defined arguments when constructing the pipeline
             name (str, optional): Name of the output stream
         """
         super().__init__()
 
         self.name = name
         self.out = self.Out(self)
-        self.node: Optional[
-            dai.node.NeuralNetwork,
-            dai.node.MobileNetDetectionNetwork,
-            dai.node.MobileNetSpatialDetectionNetwork,
-            dai.node.YoloDetectionNetwork,
-            dai.node.YoloSpatialDetectionNetwork] = None
+        self.node: Union[None,
+                         dai.node.NeuralNetwork,
+                         dai.node.MobileNetDetectionNetwork, dai.node.MobileNetSpatialDetectionNetwork,
+                         dai.node.YoloDetectionNetwork, dai.node.YoloSpatialDetectionNetwork] = None
 
         # ImageManip used to resize the input to match the expected NN input size
         self.image_manip: Optional[dai.node.ImageManip] = None
         self.x_in: Optional[dai.node.XLinkIn] = None  # Used for multi-stage pipeline
         self.tracker = pipeline.createObjectTracker() if tracker else None
+        self.apply_tracking_filter = False
+        self.forget_after_n_frames = None
 
         # Private properties
         self._ar_resize_mode: ResizeMode = ResizeMode.LETTERBOX  # Default
-        self._input: Union[CameraComponent, 'NNComponent']  # Input to the NNComponent node passed on initialization
+        self._input: Union[CameraComponent, 'NNComponent', dai.Node.Output] = input  # Input to the NNComponent node passed on initialization
         self._stream_input: dai.Node.Output  # Node Output that will be used as the input for this NNComponent
 
         self._blob: Optional[dai.OpenVINO.Blob] = None
         self._forced_version: Optional[dai.OpenVINO.Version] = None  # Forced OpenVINO version
         self._size: Optional[Tuple[int, int]] = None  # Input size to the NN
-        self._args: Optional[Dict] = None
+        self._args: Optional[Dict] = args
         self._config: Optional[Dict] = None
         self._node_type: dai.node = dai.node.NeuralNetwork  # Type of the node for `node`
         self._roboflow: Optional[RoboflowIntegration] = None
 
+        # Multi-stage pipeline
         self._multi_stage_nn: Optional[MultiStageNN] = None
         self._multi_stage_config: Optional[MultiStageConfig] = None
+        self._multi_stage_num_frame_pool = 20
 
         self._input_queue = Optional[None]  # Input queue for multi-stage pipeline
 
-        self._spatial: Optional[Union[bool, StereoComponent]] = None
-        self._replay: Optional[Replay]  # Replay module
+        self._spatial: Optional[Union[bool, StereoComponent]] = spatial
+        self._replay: Optional[Replay] = replay  # Replay module
 
         # For visualizer
         self._labels: Optional[List] = None  # Obj detector labels
         self._handler: Optional[Callable] = None  # Custom model handler for decoding
 
         # Save passed settings
-        self._input = input
-        self._spatial = spatial
-        self._args = args
-        self._replay = replay
         self._decode_fn = decode_fn or None  # Decode function that will be used to decode NN results
 
         # Parse passed settings
         self._parse_model(model)
         if nn_type:
             self._parse_node_type(nn_type)
 
         # Create NN node
         self.node = pipeline.create(self._node_type)
         self._update_config()
 
-    def forced_openvino_version(self) -> dai.OpenVINO.Version:
-        """
-        Checks whether the component forces a specific OpenVINO version. This function is called after
-        Camera has been configured and right before we connect to the OAK camera.
-        @return: Forced OpenVINO version (optional).
-        """
-        return self._forced_version
-
-    def on_init(self, pipeline: dai.Pipeline, device: dai.Device, version: dai.OpenVINO.Version):
         if self._roboflow:
             path = self._roboflow.device_update(device)
             self._parse_config(path)
             self._update_config()
 
         if self._blob is None:
-            self._blob = dai.OpenVINO.Blob(self._blob_from_config(self._config['model'], version))
+            self._blob = dai.OpenVINO.Blob(self._blob_from_config(self._config['model']))
 
         # TODO: update NN input based on camera resolution
         self.node.setBlob(self._blob)
         self._out = self.node.out
 
         if 1 < len(self._blob.networkInputs):
             raise NotImplementedError()
@@ -149,34 +141,38 @@
             nn_size = self._input._size
             scale = frame_size[0] / nn_size[0], frame_size[1] / nn_size[1]
             i = 0 if scale[0] < scale[1] else 1
             crop = int(scale[i] * nn_size[0]), int(scale[i] * nn_size[1])
             # Crop the high-resolution frames, so it matches object detection frame aspect ratio
 
             self.image_manip = pipeline.createImageManip()
-            self.image_manip.setNumFramesPool(10)
+            self.image_manip.setNumFramesPool(self._multi_stage_num_frame_pool)
             self.image_manip_config = dai.ImageManipConfig()
             self.image_manip.initialConfig.setFrameType(dai.RawImgFrame.Type.BGR888p)
 
             self._input._stream_input.link(self.image_manip.inputImage)
             if self._input._is_detector() and self._decode_fn is None:
                 self.image_manip.setResize(*crop)
                 self.image_manip.setMaxOutputFrameSize(crop[0] * crop[1] * 3)
 
                 # Create script node, get HQ frames from input.
-                self._multi_stage_nn = MultiStageNN(pipeline, self._input.node, self.image_manip.out, self._size)
+                self._multi_stage_nn = MultiStageNN(pipeline=pipeline,
+                                                    detection_node=self._input.node,
+                                                    high_res_frames=self.image_manip.out,
+                                                    size=self._size,
+                                                    num_frames_pool=self._multi_stage_num_frame_pool)
                 self._multi_stage_nn.configure(self._multi_stage_config)
                 self._multi_stage_nn.out.link(self.node.input)  # Cropped frames
 
                 # For debugging, for integral counter
                 self.node.out.link(self._multi_stage_nn.script.inputs['recognition'])
                 self.node.input.setBlocking(True)
                 self.node.input.setQueueSize(20)
             else:
-                print('Using on-host decoding for multi-stage NN')
+                logging.debug('Using on-host decoding for multi-stage NN')
                 # Custom NN
                 self.image_manip.setResize(*self._size)
                 self.image_manip.setMaxOutputFrameSize(self._size[0] * self._size[1] * 3)
 
                 # TODO pass frame on device, and just send config from host
                 self.x_in = pipeline.createXLinkIn()
                 self.x_in.setStreamName("input_queue")
@@ -185,33 +181,43 @@
 
                 self.x_in_cfg = pipeline.createXLinkIn()
                 self.x_in_cfg.setStreamName("input_queue_cfg")
                 self.x_in_cfg.out.link(self.image_manip.inputConfig)
 
                 self.image_manip.out.link(self.node.input)
                 self.node.input.setQueueSize(20)
+        elif isinstance(self._input, dai.Node.Output):
+            self._stream_input = self._input
+            self._setup_resize_manip(pipeline).link(self.node.input)
         else:
             raise ValueError(
                 "'input' argument passed on init isn't supported!"
                 "You can only use NnComponent or CameraComponent as the input."
             )
 
         if self._spatial:
             if isinstance(self._spatial, bool):  # Create new StereoComponent
-                self._spatial = StereoComponent(pipeline, args=self._args, replay=self._replay)
-                self._spatial.on_init(pipeline, device, version)
+                self._spatial = StereoComponent(device, pipeline, args=self._args, replay=self._replay)
             if isinstance(self._spatial, StereoComponent):
                 self._spatial.depth.link(self.node.inputDepth)
                 self._spatial.config_stereo(align=self._input._source)
             # Configure Spatial Detection Network
 
         if self._args:
             if self._is_spatial():
                 self._config_spatials_args(self._args)
 
+    def forced_openvino_version(self) -> dai.OpenVINO.Version:
+        """
+        Checks whether the component forces a specific OpenVINO version. This function is called after
+        Camera has been configured and right before we connect to the OAK camera.
+        @return: Forced OpenVINO version (optional).
+        """
+        return self._forced_version
+
     def _parse_model(self, model):
         """
         Called when NNComponent is initialized. Parses "model" argument passed by user.
         """
         if isinstance(model, Dict):
             self._parse_config(model)
             return
@@ -230,15 +236,15 @@
             models = getSupportedModels(printModels=False)
             zoo_models = blobconverter.zoo_list()
 
             if str(model) in models:
                 model = models[str(model)] / 'config.json'
                 self._parse_config(model)
             elif str(model) in zoo_models:
-                print(
+                logging.warning(
                     'Models from the OpenVINO Model Zoo do not carry any metadata'
                     ' (e.g., label map, decoding logic). Please keep this in mind when using models from Zoo.'
                 )
                 self._blob = dai.OpenVINO.Blob(blobconverter.from_zoo(str(model), shaves=6))
                 self._forced_version = self._blob.version
             else:
                 raise ValueError(f"Specified model '{str(model)}' is not supported by DepthAI SDK.\n"
@@ -274,15 +280,15 @@
             with model_config.open() as f:
                 self._config = Config().load(json.loads(f.read()))
         else:  # Dict
             self._config = model_config
 
         if 'source' in self._config:
             if self._config['source'] == 'roboflow':
-                from depthai_sdk.components.integrations.roboflow import RoboflowIntegration
+                from depthai_sdk.integrations.roboflow import RoboflowIntegration
                 self._roboflow = RoboflowIntegration(self._config)
                 self._parse_node_type('YOLO')  # Roboflow only supports YOLO models
                 return
             else:
                 raise ValueError(f"[NN Dict configuration] Source '{self._config['source']}' not supported")
 
         # Get blob from the config file
@@ -306,30 +312,34 @@
         self._labels = self._config.get("mappings", {}).get("labels", None)
 
         # Handler.py logic to decode raw NN results into standardized AI results
         if 'handler' in self._config:
             self._handler = loadModule(model_config.parent / self._config["handler"])
 
             if not callable(getattr(self._handler, "decode", None)):
-                raise RuntimeError("Custom model handler does not contain 'decode' method!")
+                logging.debug("Custom model handler does not contain 'decode' method!")
+            else:
+                self._decode_fn = self._handler.decode if self._decode_fn is None else self._decode_fn
 
         if 'nn_config' in self._config:
             nn_config = self._config.get("nn_config", {})
 
             # Parse node type
             nn_family = nn_config.get("NN_family", None)
             if nn_family:
                 self._parse_node_type(nn_family)
 
-    def _blob_from_config(self, model: Dict, version: dai.OpenVINO.Version) -> str:
+    def _blob_from_config(self, model: Dict, version: Optional[dai.OpenVINO.Version] = None) -> str:
         """
         Gets the blob from the config file.
         """
-        vals = str(version).split('_')
-        version_str = f"{vals[1]}.{vals[2]}"
+        version_str = None
+        if version is not None:
+            vals = str(version).split('_')
+            version_str = f"{vals[1]}.{vals[2]}"
 
         if 'model_name' in model:  # Use blobconverter to download the model
             zoo_type = model.get("zoo", 'intel')
             return blobconverter.from_zoo(model['model_name'],
                                           zoo_type=zoo_type,
                                           shaves=6,  # TODO: Calculate ideal shave amount
                                           version=version_str
@@ -355,44 +365,57 @@
             self._stream_input.link(self.image_manip.inputImage)
             self.image_manip.setMaxOutputFrameSize(self._size[0] * self._size[1] * 3)
             self.image_manip.initialConfig.setFrameType(dai.RawImgFrame.Type.BGR888p)
             # Set to non-blocking
             self.image_manip.inputImage.setBlocking(False)
             self.image_manip.inputImage.setQueueSize(2)
 
-        # Set Aspect Ratio resizing mode
-        if self._ar_resize_mode == ResizeMode.CROP:
-            # Cropping is already the default mode of the ImageManip node
-            self.image_manip.initialConfig.setResize(self._size)
-        elif self._ar_resize_mode == ResizeMode.LETTERBOX:
-            self.image_manip.initialConfig.setResizeThumbnail(*self._size)
-        elif self._ar_resize_mode == ResizeMode.STRETCH:
-            self.image_manip.initialConfig.setResize(self._size)
-            self.image_manip.setKeepAspectRatio(False)  # Not keeping aspect ratio -> stretching the image
-
+        self.image_manip.initialConfig.setResizeThumbnail(*self._size)
         return self.image_manip.out
 
+    def _change_resize_mode(self, mode: ResizeMode) -> None:
+        """
+        Changes the resize mode of the ImageManip node.
+
+        Args:
+            mode (ResizeMode): Resize mode to use
+        """
+        self._ar_resize_mode = mode
+
+        if self.image_manip:
+            if self._ar_resize_mode == ResizeMode.CROP:
+                # Cropping is already the default mode of the ImageManip node
+                self.image_manip.initialConfig.setResize(self._size)
+            elif self._ar_resize_mode == ResizeMode.LETTERBOX:
+                self.image_manip.initialConfig.setResizeThumbnail(*self._size)
+            elif self._ar_resize_mode == ResizeMode.STRETCH:
+                self.image_manip.initialConfig.setResize(self._size)
+                self.image_manip.setKeepAspectRatio(False)  # Not keeping aspect ratio -> stretching the image
+
     def config_multistage_nn(self,
                              debug=False,
                              labels: Optional[List[int]] = None,
                              scale_bb: Optional[Tuple[int, int]] = None,
+                             num_frame_pool: int = None
                              ) -> None:
         """
         Configures the MultiStage NN pipeline. Available if the input to this NNComponent is Detection NNComponent.
 
         Args:
             debug (bool, default False): Debug script node
             labels (List[int], optional): Crop & run inference only on objects with these labels
             scale_bb (Tuple[int, int], optional): Scale detection bounding boxes (x, y) before cropping the frame. In %.
+            num_frame_pool (int, optional): Number of frames to pool for inference. If None, will use the default value.
         """
         if not self._is_multi_stage():
-            print("Input to this model was not a NNComponent, so 2-stage NN inferencing isn't possible!"
-                  "This configuration attempt will be ignored.")
+            logging.warning("Input to this model was not a NNComponent, so 2-stage NN inferencing isn't possible!"
+                            "This configuration attempt will be ignored.")
             return
 
+        self._multi_stage_num_frame_pool = num_frame_pool
         self._multi_stage_config = MultiStageConfig(debug, labels, scale_bb)
 
     def _parse_label(self, label: Union[str, int]) -> int:
         if isinstance(label, int):
             return label
         elif isinstance(label, str):
             if not self._labels:
@@ -407,50 +430,60 @@
             raise Exception('_parse_label only accepts int or str')
 
     def config_tracker(self,
                        tracker_type: Optional[dai.TrackerType] = None,
                        track_labels: Optional[List[int]] = None,
                        assignment_policy: Optional[dai.TrackerIdAssignmentPolicy] = None,
                        max_obj: Optional[int] = None,
-                       threshold: Optional[float] = None
+                       threshold: Optional[float] = None,
+                       apply_tracking_filter: Optional[bool] = None,
+                       forget_after_n_frames: Optional[int] = None,
                        ):
         """
         Configure Object Tracker node (if it's enabled).
 
         Args:
             tracker_type (dai.TrackerType, optional): Set object tracker type
             track_labels (List[int], optional): Set detection labels to track
             assignment_policy (dai.TrackerType, optional): Set object tracker ID assignment policy
             max_obj (int, optional): Set max objects to track. Max 60.
-            threshold (float, optional): Set threshold for object detection confidence. Default: 0.0
+            threshold (float, optional): Specify tracker threshold. Default: 0.0
+            apply_tracking_filter (bool, optional): Set whether to apply Kalman filter to the tracked objects. Done on the host.
+            forget_after_n_frames (int, optional): Set how many frames to track an object before forgetting it.
         """
 
         if self.tracker is None:
             warnings.warn("Tracker was not enabled! Enable with cam.create_nn('[model]', tracker=True)."
                           "This configuration attempt will be ignored.")
             return
 
-        if tracker_type:
+        if tracker_type is not None:
             self.tracker.setTrackerType(type=tracker_type)
 
-        if track_labels and 0 < len(track_labels):
+        if track_labels is not None and 0 < len(track_labels):
             labels = [self._parse_label(l) for l in track_labels]
             self.tracker.setDetectionLabelsToTrack(labels)
 
-        if assignment_policy:
+        if assignment_policy is not None:
             self.tracker.setTrackerIdAssignmentPolicy(assignment_policy)
 
-        if max_obj:
+        if max_obj is not None:
             if 60 < max_obj:
                 raise ValueError("Maximum objects to track is 60!")
             self.tracker.setMaxObjectsToTrack(max_obj)
 
-        if threshold:
+        if threshold is not None:
             self.tracker.setTrackerThreshold(threshold)
 
+        if apply_tracking_filter is not None:
+            self.apply_tracking_filter = apply_tracking_filter
+
+        if forget_after_n_frames is not None:
+            self.forget_after_n_frames = forget_after_n_frames
+
     def config_yolo_from_metadata(self, metadata: Dict):
         """
         Configures (Spatial) Yolo Detection Network node with a dictionary. Calls config_yolo().
         """
         return self.config_yolo(
             num_classes=metadata['classes'],
             coordinate_size=metadata['coordinates'],
@@ -466,30 +499,29 @@
                     anchors: List[float],
                     masks: Dict[str, List[int]],
                     iou_threshold: float,
                     conf_threshold: Optional[float] = None,
                     ) -> None:
         """
         Configures (Spatial) Yolo Detection Network node.
-
         """
         if not self._is_yolo():
-            print('This is not a YOLO detection network! This configuration attempt will be ignored.')
+            logging.warning('This is not a YOLO detection network! This configuration attempt will be ignored.')
             return
 
         if not self.node:
             raise Exception('YOLO node not initialized!')
 
         self.node.setNumClasses(num_classes)
         self.node.setCoordinateSize(coordinate_size)
         self.node.setAnchors(anchors)
         self.node.setAnchorMasks(masks)
         self.node.setIouThreshold(iou_threshold)
 
-        if conf_threshold:
+        if conf_threshold is not None:
             self.node.setConfidenceThreshold(conf_threshold)
 
     def config_nn(self,
                   conf_threshold: Optional[float] = None,
                   resize_mode: Union[ResizeMode, str] = None):
         """
         Configures the Detection Network node.
@@ -499,20 +531,20 @@
             resize_mode: (ResizeMode, optional): Change aspect ratio resizing mode - to either STRETCH, CROP, or LETTERBOX.
         """
         if resize_mode:
             if isinstance(resize_mode, str):
                 try:
                     resize_mode = ResizeMode[resize_mode.upper()]
                 except (AttributeError, KeyError):
-                    print('AR resize mode was not recognizied.'
-                          'Options (case insensitive): STRETCH, CROP, LETTERBOX.'
-                          'Using default LETTERBOX mode.')
+                    logging.warning('AR resize mode was not recognizied.'
+                                    'Options (case insensitive): STRETCH, CROP, LETTERBOX.'
+                                    'Using default LETTERBOX mode.')
 
-            self._ar_resize_mode = resize_mode
-        if conf_threshold and self._is_detector():
+            self._change_resize_mode(resize_mode)
+        if conf_threshold is not None and self._is_detector():
             self.node.setConfidenceThreshold(conf_threshold)
 
     def config_spatial(self,
                        bb_scale_factor: Optional[float] = None,
                        lower_threshold: Optional[int] = None,
                        upper_threshold: Optional[int] = None,
                        calc_algo: Optional[dai.SpatialLocationCalculatorAlgorithm] = None):
@@ -522,22 +554,22 @@
         Args:
             bb_scale_factor (float, optional): Specifies scale factor for detected bounding boxes (0..1]
             lower_threshold (int, optional): Specifies lower threshold in depth units (millimeter by default) for depth values which will used to calculate spatial data
             upper_threshold (int, optional): Specifies upper threshold in depth units (millimeter by default) for depth values which will used to calculate spatial data
             calc_algo (dai.SpatialLocationCalculatorAlgorithm, optional): Specifies spatial location calculator algorithm: Average/Min/Max
         """
         if not self._is_spatial():
-            print('This is not a Spatial Detection network! This configuration attempt will be ignored.')
+            logging.warning('This is not a Spatial Detection network! This configuration attempt will be ignored.')
             return
 
-        if bb_scale_factor:
+        if bb_scale_factor is not None:
             self.node.setBoundingBoxScaleFactor(bb_scale_factor)
-        if lower_threshold:
+        if lower_threshold is not None:
             self.node.setDepthLowerThreshold(lower_threshold)
-        if upper_threshold:
+        if upper_threshold is not None:
             self.node.setDepthUpperThreshold(upper_threshold)
         if calc_algo:
             self.node.setSpatialCalculationAlgorithm(calc_algo)
 
     def _update_config(self):
         if self.node is None or self._config is None:
             return
@@ -575,17 +607,19 @@
                                    frames=self._comp._input._input.get_stream_xout(),
                                    det_out=det_nn_out,
                                    second_nn_out=second_nn_out,
                                    device=device,
                                    input_queue_name="input_queue" if self._comp.x_in else None)
             else:
                 det_nn_out = StreamXout(id=self._comp.node.id, out=self._comp.node.out, name=self._comp.name)
-
+                input_stream = self._comp._stream_input
                 out = XoutNnResults(det_nn=self._comp,
-                                    frames=self._comp._input.get_stream_xout(),
+                                    frames=StreamXout(id=input_stream.getParent().id,
+                                                      out=input_stream,
+                                                      name=self._comp.name),
                                     nn_results=det_nn_out)
 
             return self._comp._create_xout(pipeline, out)
 
         def passthrough(self, pipeline: dai.Pipeline, device: dai.Device) -> XoutBase:
             """
             Default output. Streams NN results and passthrough frames (frames used for inferencing)
@@ -669,15 +703,18 @@
             self._comp.node.out.link(self._comp.tracker.inputDetections)
 
             # TODO: add support for full frame tracking
             self._comp.node.passthrough.link(self._comp.tracker.inputTrackerFrame)
 
             out = XoutTracker(det_nn=self._comp,
                               frames=self._comp._input.get_stream_xout(),  # CameraComponent
-                              tracklets=StreamXout(self._comp.tracker.id, self._comp.tracker.out))
+                              device=device,
+                              tracklets=StreamXout(self._comp.tracker.id, self._comp.tracker.out),
+                              apply_kalman=self._comp.apply_tracking_filter,
+                              forget_after_n_frames=self._comp.forget_after_n_frames)
 
             return self._comp._create_xout(pipeline, out)
 
         def encoded(self, pipeline: dai.Pipeline, device: dai.Device) -> XoutNnResults:
             """
             Streams NN results and encoded frames (frames used for inferencing)
             Produces DetectionPacket or TwoStagePacket (if it's 2. stage NNComponent).
@@ -707,14 +744,21 @@
                     profile=self._comp._input._encoder_profile,
                     fps=self._comp._input.encoder.getFrameRate(),
                     frame_shape=self._comp._input.stream_size
                 )
 
             return self._comp._create_xout(pipeline, out)
 
+        def nn_data(self, pipeline: dai.Pipeline, device: dai.Device) -> XoutNnData:
+            if type(self._comp.node) == dai.node.NeuralNetwork:
+                out = XoutNnData(xout=StreamXout(self._comp.node.id, self._comp.node.out))
+            else:
+                out = XoutNnData(xout=StreamXout(self._comp.node.id, self._comp.node.outNetwork))
+            return self._comp._create_xout(pipeline, out)
+
     # Checks
     def _is_spatial(self) -> bool:
         return self._spatial is not None  # todo fix if spatial is bool and equals to False
 
     def _is_tracker(self) -> bool:
         # Currently, only object detectors are supported
         return self._is_detector() and self.tracker is not None
```

### Comparing `depthai-sdk-1.9.4.1/src/depthai_sdk/components/nn_helper.py` & `depthai-sdk-1.9.5/src/depthai_sdk/components/nn_helper.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,17 @@
 import importlib
-from enum import IntEnum
 from pathlib import Path
 import os
 from typing import Dict, Union, Optional, Tuple
 import requests
 import depthai as dai
 
 BLOBS_PATH = Path.home() / Path('.cache/blobs')
 
 
-class ResizeMode(IntEnum):
-    """
-    If NN input frame is in different aspect ratio than what the model expect, we have 3 different
-    modes of operation. Full documentation:
-    https://docs.luxonis.com/projects/api/en/latest/tutorials/maximize_fov/
-    """
-    LETTERBOX = 0  # Preserves full FOV, but smaller frame means less features which might decrease NN accuracy
-    STRETCH = 1  # Preserves full FOV, but frames are stretched which might decrease NN accuracy
-    CROP = 2  # Crops some FOV to match the required FOV. No potential NN accuracy decrease.
-
-
 def getBlob(url: str) -> Path:
     """
     Download the blob path from the url. If blob is cached, serve that. TODO: compute hash, check server hash,
     as there will likely be many `model.blob`s.
 
     @param url: Url to the blob
     @return: Local path to the blob
```

### Comparing `depthai-sdk-1.9.4.1/src/depthai_sdk/components/parser.py` & `depthai-sdk-1.9.5/src/depthai_sdk/components/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,25 +8,27 @@
     """
     Parses Color camera resolution based on the string
     """
     if isinstance(resolution, dai.ColorCameraProperties.SensorResolution) or resolution is None:
         return resolution
 
     resolution = str(resolution).upper()
-    if resolution == '3120' or resolution == '13MP':
+    if resolution in ['3120', '13MP']:
         return dai.ColorCameraProperties.SensorResolution.THE_13_MP
-    elif resolution == '3040' or resolution == '12MP':
+    elif resolution in ['3040', '12MP']:
         return dai.ColorCameraProperties.SensorResolution.THE_12_MP
-    elif resolution == '2160' or resolution == '4K':
+    elif resolution in ['2160', '4K']:
         return dai.ColorCameraProperties.SensorResolution.THE_4_K
     # elif resolution == '1920' or resolution == '5MP':
     #     return dai.ColorCameraProperties.SensorResolution.THE_5_MP
-    elif resolution == '800' or resolution == '800P':
+    elif resolution in ['1200', '1200P']:
+        return dai.ColorCameraProperties.SensorResolution.THE_1200_P
+    elif resolution in ['800', '800P']:
         return dai.ColorCameraProperties.SensorResolution.THE_800_P
-    elif resolution == '720' or resolution == '720P':
+    elif resolution in ['720', '720P']:
         return dai.ColorCameraProperties.SensorResolution.THE_720_P
     else:  # Default
         return dai.ColorCameraProperties.SensorResolution.THE_1080_P
 
 
 def mono_resolution(resolution: Union[
     None, str, dai.MonoCameraProperties.SensorResolution]) -> dai.MonoCameraProperties.SensorResolution:
@@ -64,24 +66,25 @@
         return True
     elif value.upper() in ['0', 'FALSE', 'OFF', 'NO']:
         return False
     else:
         raise ValueError(f"Couldn't parse '{value}' to bool!")
 
 
-def parse_camera_socket(value: str) -> dai.CameraBoardSocket:
+def parse_camera_socket(value: Union[str, dai.CameraBoardSocket]) -> dai.CameraBoardSocket:
+    if isinstance(value, dai.CameraBoardSocket):
+        return value
+
     value = value.upper()
     if value in ["COLOR", "RGB", "CENTER", "CAMA", "CAM_A", "CAM-A"]:
         return dai.CameraBoardSocket.CAM_A
     elif value in ["LEFT", "CAMB", "CAM_B", "CAM-B"]:
         return dai.CameraBoardSocket.CAM_B
     elif value in ["RIGHT", "CAMC", "CAM_C", "CAM-C"]:
         return dai.CameraBoardSocket.CAM_C
-    elif value in ["RIGHT", "CAMC", "CAM_C", "CAM-C"]:
-        return dai.CameraBoardSocket.CAM_C
     elif value in ["CAMD", "CAM_D", "CAM-D"]:
         return dai.CameraBoardSocket.CAM_D
     elif value in ["CAME", "CAM_E", "CAM-E"]:
         return dai.CameraBoardSocket.CAM_E
     elif value in ["CAMF", "CAM_F", "CAM-F"]:
         return dai.CameraBoardSocket.CAM_F
     elif value in ["CAMG", "CAM_G", "CAM-G"]:
```

### Comparing `depthai-sdk-1.9.4.1/src/depthai_sdk/components/stereo_component.py` & `depthai-sdk-1.9.5/src/depthai_sdk/components/stereo_component.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,50 @@
+import logging
 import warnings
 from enum import Enum
-from typing import Optional, Union, Any, Dict
+from typing import Optional, Union, Any, Dict, Tuple
 
+import cv2
 import depthai as dai
-
+import numpy as np
 from depthai_sdk.components.camera_component import CameraComponent
 from depthai_sdk.components.component import Component
 from depthai_sdk.components.parser import parse_cam_socket, parse_median_filter, parse_encode
+from depthai_sdk.components.undistort import _get_mesh
 from depthai_sdk.oak_outputs.xout.xout_base import XoutBase, StreamXout
 from depthai_sdk.oak_outputs.xout.xout_depth import XoutDepth
 from depthai_sdk.oak_outputs.xout.xout_disparity import XoutDisparity
+from depthai_sdk.oak_outputs.xout.xout_frames import XoutFrames
 from depthai_sdk.oak_outputs.xout.xout_h26x import XoutH26x
 from depthai_sdk.oak_outputs.xout.xout_mjpeg import XoutMjpeg
 from depthai_sdk.replay import Replay
 from depthai_sdk.visualize.configs import StereoColor
 
 
 class WLSLevel(Enum):
     """WLS filter level"""
     LOW = (1000, 0.8)
     MEDIUM = (6000, 1.5)
     HIGH = (12000, 2.0)
 
 
 class StereoComponent(Component):
+
+    @property
+    def depth(self) -> dai.Node.Output:
+        # Depth output from the StereoDepth node.
+        return self.node.depth
+
+    @property
+    def disparity(self) -> dai.Node.Output:
+        # Disparity output from the StereoDepth node.
+        return self.node.disparity
+
     def __init__(self,
+                 device: dai.Device,
                  pipeline: dai.Pipeline,
                  resolution: Union[None, str, dai.MonoCameraProperties.SensorResolution] = None,
                  fps: Optional[float] = None,
                  left: Union[None, CameraComponent, dai.node.MonoCamera] = None,  # Left mono camera
                  right: Union[None, CameraComponent, dai.node.MonoCamera] = None,  # Right mono camera
                  replay: Optional[Replay] = None,
                  args: Any = None,
@@ -51,116 +67,137 @@
 
         self.left: Union[None, CameraComponent, dai.node.MonoCamera, dai.node.ColorCamera, dai.Node.Output]
         self.right: Union[None, CameraComponent, dai.node.MonoCamera, dai.node.ColorCamera, dai.Node.Output]
 
         self._left_stream: dai.Node.Output
         self._right_stream: dai.Node.Output
 
-        self.colormap = None
+        self.colormap = None  # for on-device colorization
 
         self._replay: Optional[Replay] = replay
         self._resolution: Optional[Union[str, dai.MonoCameraProperties.SensorResolution]] = resolution
         self._fps: Optional[float] = fps
         self._args: Dict = args
         self.name = name
 
         self.left = left
         self.right = right
 
         self.node: dai.node.StereoDepth = pipeline.createStereoDepth()
         self.node.setDefaultProfilePreset(dai.node.StereoDepth.PresetMode.HIGH_DENSITY)
 
+        # Encoder
         self.encoder = None
         if encode:
             self.encoder = pipeline.createVideoEncoder()
             # MJPEG by default
             self._encoderProfile = parse_encode(encode)
 
-        # Configuration variables
+        # Postprocessing options
         self._colorize = None
         self._postprocess_colormap = None
         self.wls_enabled = None
         self._wls_level = None
         self._wls_lambda = None
         self._wls_sigma = None
 
-    def get_output_stream(self, input: Union[
-        CameraComponent, dai.node.MonoCamera, dai.node.ColorCamera, dai.Node.Output
-    ]) -> dai.Node.Output:
-        if isinstance(input, CameraComponent):
-            return input.stream
-        elif isinstance(input, dai.node.MonoCamera):
-            return input.out
-        elif isinstance(input, dai.node.ColorCamera):
-            return input.video
-        elif isinstance(input, dai.Node.Output):
-            return input
-        else:
-            raise ValueError('get_output_stream() accepts either CameraComponent,'
-                             'dai.node.MonoCamera, dai.node.ColorCamera, dai.Node.Output!')
+        self._undistortion_offset: Optional[int] = None
 
-    def on_init(self, pipeline: dai.Pipeline, device: dai.Device, version: dai.OpenVINO.Version):
         if not self._replay:
             # Live stream, check whether we have correct cameras
             if len(device.getCameraSensorNames()) == 1:
                 raise Exception('OAK-1 camera does not have Stereo camera pair!')
 
+            # If not specified, default to 400P resolution for faster processing
+            self._resolution = self._resolution or dai.MonoCameraProperties.SensorResolution.THE_400_P
+
             if not self.left:
-                self.left = CameraComponent(pipeline, 'left', self._resolution, self._fps, replay=self._replay)
-                self.left.on_init(pipeline, device, version)
+                self.left = CameraComponent(device, pipeline, 'left', self._resolution, self._fps, replay=self._replay)
             if not self.right:
-                self.right = CameraComponent(pipeline, 'right', self._resolution, self._fps, replay=self._replay)
-                self.right.on_init(pipeline, device, version)
+                self.right = CameraComponent(device, pipeline, 'right', self._resolution, self._fps, replay=self._replay)
 
             if 0 < len(device.getIrDrivers()):
                 laser = self._args.get('irDotBrightness', None)
-                laser = int(laser) if laser else 800
+                laser = laser if laser is not None else 800
                 if 0 < laser:
                     device.setIrLaserDotProjectorBrightness(laser)
-                    print(f'Setting IR laser dot projector brightness to {laser}mA')
+                    logging.info(f'Setting IR laser dot projector brightness to {laser}mA')
 
                 led = self._args.get('irFloodBrightness', None)
                 if led is not None:
                     device.setIrFloodLightBrightness(int(led))
-                    print(f'Setting IR flood LED brightness to {int(led)}mA')
+                    logging.info(f'Setting IR flood LED brightness to {int(led)}mA')
+
+            input_size = self._get_stream_size(self.left)
+            if input_size:
+                self.node.setInputResolution(*input_size)
 
-        self._left_stream = self.get_output_stream(self.left)
-        self._right_stream = self.get_output_stream(self.right)
+        self._left_stream = self._get_output_stream(self.left)
+        self._right_stream = self._get_output_stream(self.right)
 
         if self._replay:  # Replay
-            self._replay.initStereoDepth(self.node)
+            self._replay.initStereoDepth(self.node, left_name=self.left._source, right_name=self.right._source)
         else:
             self._left_stream.link(self.node.left)
             self._right_stream.link(self.node.right)
 
-        colormap_manip = None
-        if self.colormap:
-            colormap_manip = pipeline.create(dai.node.ImageManip)
-            colormap_manip.initialConfig.setColormap(self.colormap, self.node.initialConfig.getMaxDisparity())
-            colormap_manip.initialConfig.setFrameType(dai.ImgFrame.Type.NV12)
-            colormap_manip.setMaxOutputFrameSize(1200 * 800 * 3)
-            self.node.disparity.link(colormap_manip.inputImage)
-
         if self.encoder:
             try:
                 fps = self.left.get_fps()  # CameraComponent
             except AttributeError:
                 fps = self.left.getFps()  # MonoCamera
 
             self.encoder.setDefaultProfilePreset(fps, self._encoderProfile)
-            if colormap_manip:
-                colormap_manip.out.link(self.encoder.input)
-            else:
-                self.node.disparity.link(self.encoder.input)
+            self.node.disparity.link(self.encoder.input)
+
+        self.node.setRectifyEdgeFillColor(0)
 
-        self.node.setOutputSize(1200, 800)
+        if self._undistortion_offset is not None:
+            calibData = self._replay._calibData if self._replay else device.readCalibration()
+            w_frame, h_frame = self._get_stream_size(self.left)
+            mapX_left, mapY_left, mapX_right, mapY_right = self._get_maps(w_frame, h_frame, calibData)
+            mesh_l = _get_mesh(mapX_left, mapY_left)
+            mesh_r = _get_mesh(mapX_right, mapY_right)
+            meshLeft = list(mesh_l.tobytes())
+            meshRight = list(mesh_r.tobytes())
+            self.node.loadMeshData(meshLeft, meshRight)
 
         if self._args:
             self._config_stereo_args(self._args)
 
+    def _get_output_stream(self, input: Union[
+        CameraComponent, dai.node.MonoCamera, dai.node.ColorCamera, dai.Node.Output
+    ]) -> dai.Node.Output:
+        if isinstance(input, CameraComponent):
+            return input.stream
+        elif isinstance(input, dai.node.MonoCamera):
+            return input.out
+        elif isinstance(input, dai.node.ColorCamera):
+            return input.video
+        elif isinstance(input, dai.Node.Output):
+            return input
+        else:
+            raise ValueError('get_output_stream() accepts either CameraComponent,'
+                             'dai.node.MonoCamera, dai.node.ColorCamera, dai.Node.Output!')
+
+    def _get_stream_size(self,
+                         input: Union[CameraComponent, dai.node.MonoCamera, dai.node.ColorCamera, dai.Node.Output]) -> \
+            Optional[Tuple[int, int]]:
+        if isinstance(input, CameraComponent):
+            return input.stream_size
+        elif isinstance(input, dai.node.MonoCamera):
+            return input.getResolutionSize()
+        elif isinstance(input, dai.node.ColorCamera):
+            return input.getVideoSize()
+        else:
+            return None
+
+    def config_undistortion(self, M2_offset: int = 0):
+        self._undistortion_offset = M2_offset
+
     def _config_stereo_args(self, args: Dict):
         if not isinstance(args, Dict):
             args = vars(args)  # Namespace -> Dict
 
         self.config_stereo(
             confidence=args.get('disparityConfidenceThreshold', None),
             median=args.get('stereoMedianSize', None),
@@ -180,22 +217,22 @@
                       lr_check: Optional[bool] = None,
                       sigma: Optional[int] = None,
                       lr_check_threshold: Optional[int] = None,
                       ) -> None:
         """
         Configures StereoDepth modes and options.
         """
-        if confidence: self.node.initialConfig.setConfidenceThreshold(confidence)
-        if align: self.node.setDepthAlign(parse_cam_socket(align))
-        if median: self.node.setMedianFilter(parse_median_filter(median))
-        if extended: self.node.initialConfig.setExtendedDisparity(extended)
-        if subpixel: self.node.initialConfig.setSubpixel(subpixel)
-        if lr_check: self.node.initialConfig.setLeftRightCheck(lr_check)
-        if sigma: self.node.initialConfig.setBilateralFilterSigma(sigma)
-        if lr_check_threshold: self.node.initialConfig.setLeftRightCheckThreshold(lr_check_threshold)
+        if confidence is not None: self.node.initialConfig.setConfidenceThreshold(confidence)
+        if align is not None: self.node.setDepthAlign(parse_cam_socket(align))
+        if median is not None: self.node.setMedianFilter(parse_median_filter(median))
+        if extended is not None: self.node.initialConfig.setExtendedDisparity(extended)
+        if subpixel is not None: self.node.initialConfig.setSubpixel(subpixel)
+        if lr_check is not None: self.node.initialConfig.setLeftRightCheck(lr_check)
+        if sigma is not None: self.node.initialConfig.setBilateralFilterSigma(sigma)
+        if lr_check_threshold is not None: self.node.initialConfig.setLeftRightCheckThreshold(lr_check_threshold)
 
     def config_postprocessing(self,
                               colorize: Union[StereoColor, bool] = None,
                               colormap: int = None
                               ) -> None:
         """
         Configures postprocessing options.
@@ -229,26 +266,42 @@
             wls_sigma: WLS filter sigma.
         """
         self.wls_enabled = True if wls_level else False
 
         if isinstance(wls_level, WLSLevel):
             self._wls_level = wls_level
         elif isinstance(wls_level, str):
-            self._wls_level = WLSLevel(wls_level.upper())
+            self._wls_level = WLSLevel[wls_level.upper()]
 
         self._wls_lambda = wls_lambda
         self._wls_sigma = wls_sigma
 
     def set_colormap(self, colormap: dai.Colormap):
         """
         Sets the colormap to use for colorizing the disparity map. Used for on-device postprocessing.
+        Works only with `encoded` output.
+        Note: This setting can affect the performance.
 
         Args:
             colormap: Colormap to use for colorizing the disparity map.
         """
+        if self.colormap != colormap and self.encoder:
+            colormap_manip = self.node.getParentPipeline().create(dai.node.ImageManip)
+            colormap_manip.initialConfig.setColormap(colormap, self.node.initialConfig.getMaxDisparity())
+            colormap_manip.initialConfig.setFrameType(dai.ImgFrame.Type.NV12)
+            h, w = self.left.stream_size
+            colormap_manip.setMaxOutputFrameSize(h * w * 3)
+            self.node.disparity.link(colormap_manip.inputImage)
+
+            if self.encoder:
+                self.node.disparity.unlink(self.encoder.input)
+                colormap_manip.out.link(self.encoder.input)
+        elif not self.encoder:
+            warnings.warn('At the moment, colormap can be used only if encoder is enabled.')
+
         self.colormap = colormap
 
     def _get_disparity_factor(self, device: dai.Device) -> float:
         """
         Calculates the disparity factor used to calculate depth from disparity.
         `depth = disparity_factor / disparity`
         @param device: OAK device
@@ -256,42 +309,52 @@
         calib = device.readCalibration()
         baseline = calib.getBaselineDistance(useSpecTranslation=True) * 10  # mm
         intrinsics = calib.getCameraIntrinsics(dai.CameraBoardSocket.RIGHT, self.right.getResolutionSize())
         focalLength = intrinsics[0][0]
         disp_levels = self.node.getMaxDisparity() / 95
         return baseline * focalLength * disp_levels
 
-    @property
-    def depth(self) -> dai.Node.Output:
-        # Depth output from the StereoDepth node.
-        return self.node.depth
-
-    @property
-    def disparity(self) -> dai.Node.Output:
-        # Disparity output from the StereoDepth node.
-        return self.node.disparity
+    def _get_maps(self, width: int, height: int, calib: dai.CalibrationHandler):
+        imageSize = (width, height)
+        M1 = np.array(calib.getCameraIntrinsics(calib.getStereoLeftCameraId(), width, height))
+        M2 = np.array(calib.getCameraIntrinsics(calib.getStereoRightCameraId(), width, height))
+        d1 = np.array(calib.getDistortionCoefficients(calib.getStereoLeftCameraId()))
+        d2 = np.array(calib.getDistortionCoefficients(calib.getStereoRightCameraId()))
+        R1 = np.array(calib.getStereoLeftRectificationRotation())
+        R2 = np.array(calib.getStereoRightRectificationRotation())
+
+        # increaseOffset = -100 if width == 1152 else -166.67
+        """ increaseOffset = 0
+        M2_focal = M2.copy()
+        M2_focal[0][0] += increaseOffset
+        M2_focal[1][1] += increaseOffset
+        kScaledL = M2_focal
+        kScaledR = kScaledL """
+
+        M2[0][0] += self._undistortion_offset
+        M2[1][1] += self._undistortion_offset
+
+        mapX_l, mapY_l = cv2.initUndistortRectifyMap(M1, d1, R1, M2, imageSize, cv2.CV_32FC1)
+        mapX_r, mapY_r = cv2.initUndistortRectifyMap(M2, d2, R2, M2, imageSize, cv2.CV_32FC1)
+        return mapX_l, mapY_l, mapX_r, mapY_r
 
     """
     Available outputs (to the host) of this component
     """
 
     class Out:
         def __init__(self, stereo_component: 'StereoComponent'):
             self._comp = stereo_component
 
         def main(self, pipeline: dai.Pipeline, device: dai.Device) -> XoutBase:
             # By default, we want to show disparity
             return self.depth(pipeline, device)
 
         def disparity(self, pipeline: dai.Pipeline, device: dai.Device) -> XoutBase:
-            if self._comp.colormap:
-                warnings.warn('Colormap set with `set_colormap` is ignored when using disparity output. '
-                              'Please use `configure_postprocessing` instead.')
-
-            fps = self._comp.left.get_fps() if self._comp._replay is None else self._comp._replay.getFps()
+            fps = self._comp.left.get_fps() if self._comp._replay is None else self._comp._replay.get_fps()
 
             out = XoutDisparity(
                 disparity_frames=StreamXout(self._comp.node.id, self._comp.disparity, name=self._comp.name),
                 mono_frames=StreamXout(self._comp.node.id, self._comp._right_stream, name=self._comp.name),
                 max_disp=self._comp.node.getMaxDisparity(),
                 fps=fps,
                 colorize=self._comp._colorize,
@@ -300,20 +363,32 @@
                 wls_level=self._comp._wls_level,
                 wls_lambda=self._comp._wls_lambda,
                 wls_sigma=self._comp._wls_sigma
             )
 
             return self._comp._create_xout(pipeline, out)
 
-        def depth(self, pipeline: dai.Pipeline, device: dai.Device) -> XoutBase:
-            if self._comp.colormap:
-                warnings.warn('Colormap set with `set_colormap` is ignored when using depth output. '
-                              'Please use `configure_postprocessing` instead.')
+        def rectified_left(self, pipeline: dai.Pipeline, device: dai.Device) -> XoutBase:
+            fps = self._comp.left.get_fps() if self._comp._replay is None else self._comp._replay.get_fps()
+            out = XoutFrames(
+                frames=StreamXout(self._comp.node.id, self._comp.node.rectifiedLeft),
+                fps=fps)
+            out.name = 'Rectified left'
+            return self._comp._create_xout(pipeline, out)
+
+        def rectified_right(self, pipeline: dai.Pipeline, device: dai.Device) -> XoutBase:
+            fps = self._comp.left.get_fps() if self._comp._replay is None else self._comp._replay.get_fps()
+            out = XoutFrames(
+                frames=StreamXout(self._comp.node.id, self._comp.node.rectifiedRight),
+                fps=fps)
+            out.name = 'Rectified right'
+            return self._comp._create_xout(pipeline, out)
 
-            fps = self._comp.left.get_fps() if self._comp._replay is None else self._comp._replay.getFps()
+        def depth(self, pipeline: dai.Pipeline, device: dai.Device) -> XoutBase:
+            fps = self._comp.left.get_fps() if self._comp._replay is None else self._comp._replay.get_fps()
             out = XoutDepth(
                 device=device,
                 frames=StreamXout(self._comp.node.id, self._comp.depth, name=self._comp.name),
                 mono_frames=StreamXout(self._comp.node.id, self._comp._right_stream, name=self._comp.name),
                 fps=fps,
                 colorize=self._comp._colorize,
                 colormap=self._comp._postprocess_colormap,
```

### Comparing `depthai-sdk-1.9.4.1/src/depthai_sdk/components/template_multi_stage_script.py` & `depthai-sdk-1.9.5/src/depthai_sdk/components/template_multi_stage_script.py`

 * *Files identical despite different names*

### Comparing `depthai-sdk-1.9.4.1/src/depthai_sdk/fps.py` & `depthai-sdk-1.9.5/src/depthai_sdk/fps.py`

 * *Files identical despite different names*

### Comparing `depthai-sdk-1.9.4.1/src/depthai_sdk/managers/arg_manager.py` & `depthai-sdk-1.9.5/src/depthai_sdk/managers/arg_manager.py`

 * *Files identical despite different names*

### Comparing `depthai-sdk-1.9.4.1/src/depthai_sdk/managers/blob_manager.py` & `depthai-sdk-1.9.5/src/depthai_sdk/managers/blob_manager.py`

 * *Files identical despite different names*

### Comparing `depthai-sdk-1.9.4.1/src/depthai_sdk/managers/encoding_manager.py` & `depthai-sdk-1.9.5/src/depthai_sdk/managers/encoding_manager.py`

 * *Files identical despite different names*

### Comparing `depthai-sdk-1.9.4.1/src/depthai_sdk/managers/nnet_manager.py` & `depthai-sdk-1.9.5/src/depthai_sdk/managers/nnet_manager.py`

 * *Files identical despite different names*

### Comparing `depthai-sdk-1.9.4.1/src/depthai_sdk/managers/pipeline_manager.py` & `depthai-sdk-1.9.5/src/depthai_sdk/managers/pipeline_manager.py`

 * *Files identical despite different names*

### Comparing `depthai-sdk-1.9.4.1/src/depthai_sdk/managers/preview_manager.py` & `depthai-sdk-1.9.5/src/depthai_sdk/managers/preview_manager.py`

 * *Files identical despite different names*

### Comparing `depthai-sdk-1.9.4.1/src/depthai_sdk/nn_models/human-pose-estimation-0001/handler.py` & `depthai-sdk-1.9.5/src/depthai_sdk/nn_models/human-pose-estimation-0001/handler.py`

 * *Files identical despite different names*

### Comparing `depthai-sdk-1.9.4.1/src/depthai_sdk/nn_models/mobilenet-ssd/config.json` & `depthai-sdk-1.9.5/src/depthai_sdk/nn_models/mobilenet-ssd/config.json`

 * *Files identical despite different names*

### Comparing `depthai-sdk-1.9.4.1/src/depthai_sdk/nn_models/openpose2/handler.py` & `depthai-sdk-1.9.5/src/depthai_sdk/nn_models/openpose2/handler.py`

 * *Files identical despite different names*

### Comparing `depthai-sdk-1.9.4.1/src/depthai_sdk/nn_models/openpose2/model.yml` & `depthai-sdk-1.9.5/src/depthai_sdk/nn_models/openpose2/model.yml`

 * *Files identical despite different names*

### Comparing `depthai-sdk-1.9.4.1/src/depthai_sdk/nn_models/road-segmentation-adas-0001/handler.py` & `depthai-sdk-1.9.5/src/depthai_sdk/nn_models/road-segmentation-adas-0001/handler.py`

 * *Files identical despite different names*

### Comparing `depthai-sdk-1.9.4.1/src/depthai_sdk/nn_models/yolo-v3-tf/config.json` & `depthai-sdk-1.9.5/src/depthai_sdk/nn_models/yolo-v3-tf/config.json`

 * *Files identical despite different names*

### Comparing `depthai-sdk-1.9.4.1/src/depthai_sdk/nn_models/yolo-v3-tiny-tf/config.json` & `depthai-sdk-1.9.5/src/depthai_sdk/nn_models/yolo-v3-tiny-tf/config.json`

 * *Files identical despite different names*

### Comparing `depthai-sdk-1.9.4.1/src/depthai_sdk/nn_models/yolov4_coco_608x608/config.json` & `depthai-sdk-1.9.5/src/depthai_sdk/nn_models/yolov4_coco_608x608/config.json`

 * *Files identical despite different names*

### Comparing `depthai-sdk-1.9.4.1/src/depthai_sdk/nn_models/yolov4_tiny_coco_416x416/config.json` & `depthai-sdk-1.9.5/src/depthai_sdk/nn_models/yolov4_tiny_coco_416x416/config.json`

 * *Files identical despite different names*

### Comparing `depthai-sdk-1.9.4.1/src/depthai_sdk/nn_models/yolov5n_coco_416x416/config.json` & `depthai-sdk-1.9.5/src/depthai_sdk/nn_models/yolov5n_coco_416x416/config.json`

 * *Files identical despite different names*

### Comparing `depthai-sdk-1.9.4.1/src/depthai_sdk/nn_models/yolov6n_coco_640x640/config.json` & `depthai-sdk-1.9.5/src/depthai_sdk/nn_models/yolov6n_coco_640x640/config.json`

 * *Files identical despite different names*

### Comparing `depthai-sdk-1.9.4.1/src/depthai_sdk/oak_camera.py` & `depthai-sdk-1.9.5/src/depthai_sdk/oak_camera.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import copy
+import logging
 import time
 import warnings
 from pathlib import Path
 from typing import Dict, Any, Optional, List, Union, Callable
 
 from depthai_sdk.visualize.visualizer import Visualizer
 
@@ -10,15 +11,15 @@
     import cv2
 except ImportError:
     cv2 = None
 
 import depthai as dai
 
 from depthai_sdk.args_parser import ArgsParser
-from depthai_sdk.classes.output_config import BaseConfig, RecordConfig, OutputConfig, SyncConfig
+from depthai_sdk.classes.output_config import BaseConfig, RecordConfig, OutputConfig, SyncConfig, RosStreamConfig
 from depthai_sdk.components.camera_component import CameraComponent
 from depthai_sdk.components.component import Component
 from depthai_sdk.components.imu_component import IMUComponent
 from depthai_sdk.components.nn_component import NNComponent
 from depthai_sdk.components.parser import parse_usb_speed
 from depthai_sdk.components.stereo_component import StereoComponent
 from depthai_sdk.oak_device import OakDevice
@@ -38,107 +39,136 @@
     It abstracts DepthAI API pipeline building, different camera permutations, stream recording/replaying, it adds
     debugging features, does AI model handling, message syncing & visualization, and much more.
 
     It was designed with interoperability with depthai API in mind.
     """
 
     def __init__(self,
-                 device: Optional[str] = None,  # MxId / IP / USB port
+                 device: Optional[str] = None,
                  usb_speed: Union[None, str, dai.UsbSpeed] = None,  # Auto by default
                  replay: Optional[str] = None,
                  rotation: int = 0,
                  args: Union[bool, Dict] = True
                  ):
         """
         Initializes OakCamera
 
         Args:
-            device (str, optional): OAK device we want to connect to
+            device (str, optional): OAK device we want to connect to, either MxId, IP, or USB port
             usb_speed (str, optional): USB speed we want to use. Defaults to 'auto'.
             replay (str, optional): Replay a depthai-recording - either local path, or from depthai-recordings repo
             rotation (int, optional): Rotate the camera output by this amount of degrees, 0 by default, 90, 180, 270 are supported.
             args (None, bool, Dict): Use user defined arguments when constructing the pipeline
         """
+
         # User should be able to access these:
         self.replay: Optional[Replay] = None
 
-        self._pipeline: Optional[dai.Pipeline] = None
+        self.pipeline = dai.Pipeline()
         self._args: Optional[Dict[str, Any]] = None  # User defined arguments
-        self._usb_speed: Optional[dai.UsbSpeed] = None
-        self._device_name: Optional[str] = None  # MxId / IP / USB port
-
-        self._device_name = device
         self._oak = OakDevice()
-        self._init_device()
+
+        if args:
+            if isinstance(args, bool):
+                self._args = ArgsParser.parseArgs()
+                # Set up the OakCamera
+                if self._args.get('recording', None):
+                    replay = self._args.get('recording', None)
+                if self._args.get('deviceId', None):
+                    device = self._args.get('deviceId', None)
+                if self._args.get('usbSpeed', None):
+                    usb_speed = parse_usb_speed(self._args.get('usbSpeed', None))
+            else:  # Already parsed
+                self._args = args
+
+        self._init_device(device, parse_usb_speed(usb_speed))
 
         # Whether to stop running the OAK camera. Used by oak.running()
         self._stop = False
-        self._usb_speed = parse_usb_speed(usb_speed)
-        self._pipeline = dai.Pipeline()
-        self._pipeline_built = False
+        self._built = False
         self._polling = []
 
         self._components: List[Component] = []  # List of components
         self._out_templates: List[BaseConfig] = []
 
         self._rotation = rotation
 
-        if args:
-            if isinstance(args, bool):
-                if args:
-                    self._args = ArgsParser.parseArgs()
-                    # Set up the OakCamera
-                    if self._args.get('recording', None):
-                        replay = self._args.get('recording', None)
-                    if self._args.get('deviceId', None):
-                        self._device_name = self._args.get('deviceId', None)
-                    if self._args.get('usbSpeed', None):
-                        self._usb_speed = parse_usb_speed(self._args.get('usbSpeed', None))
-
-                # else False - we don't want to parse user arguments
-            else:  # Already parsed
-                self._args = args
-
-        if replay:
+        if replay is not None:
             self.replay = Replay(replay)
-            print('Available streams from recording:', self.replay.getStreams())
+            self.replay.initPipeline(self.pipeline)
+            logging.info('Available streams from recording:', self.replay.getStreams())
 
     def create_camera(self,
-                      source: str,
+                      source: Union[str, dai.CameraBoardSocket],
                       resolution: Optional[Union[
                           str, dai.ColorCameraProperties.SensorResolution, dai.MonoCameraProperties.SensorResolution
                       ]] = None,
                       fps: Optional[float] = None,
                       encode: Union[None, str, bool, dai.VideoEncoderProperties.Profile] = None,
                       name: Optional[str] = None,
                       ) -> CameraComponent:
         """
         Creates Camera component. This abstracts ColorCamera/MonoCamera nodes and supports mocking the camera when
         recording is passed during OakCamera initialization. Mocking the camera will send frames from the host to the
         OAK device (via XLinkIn node).
 
         Args:
-            source (str): Either 'color', 'left' or 'right' (these 2 will create MonoCamera nodes)
+            source (str / dai.CameraBoardSocket): Camera source
             resolution (str/SensorResolution): Sensor resolution of the camera.
             fps (float): Sensor FPS
             encode (bool/str/Profile): Whether we want to enable video encoding (accessible via cameraComponent.out_encoded). If True, it will use MJPEG
             name (str): Name used to identify the X-out stream. This name will also be associated with the frame in the callback function.
         """
-        comp = CameraComponent(self._pipeline,
+        comp = CameraComponent(self._oak.device,
+                               self.pipeline,
                                source=source,
                                resolution=resolution,
                                fps=fps,
                                encode=encode,
                                rotation=self._rotation,
                                replay=self.replay,
                                name=name,
                                args=self._args)
         self._components.append(comp)
         return comp
 
+    def create_all_cameras(self,
+                           resolution: Optional[Union[
+                          str, dai.ColorCameraProperties.SensorResolution, dai.MonoCameraProperties.SensorResolution
+                      ]] = None,
+                           fps: Optional[float] = None,
+                           encode: Union[None, str, bool, dai.VideoEncoderProperties.Profile] = None,
+                           ) -> List[CameraComponent]:
+        """
+        Creates Camera component for each camera sensors on the OAK camera.
+
+        Args:
+            resolution (str/SensorResolution): Sensor resolution of the camera.
+            fps (float): Sensor FPS
+            encode (bool/str/Profile): Whether we want to enable video encoding (accessible via cameraComponent.out_encoded). If True, it will use MJPEG
+        """
+        components: List[CameraComponent] = []
+        # Loop over all available camera sensors
+        for cam_sensor in self._oak.device.getConnectedCameraFeatures():
+            comp = CameraComponent(self._oak.device,
+                                   self.pipeline,
+                                   source=cam_sensor.socket,
+                                   resolution=resolution,
+                                   fps=fps,
+                                   encode=encode,
+                                   rotation=self._rotation,
+                                   replay=self.replay,
+                                   name=None,
+                                   args=self._args)
+            components.append(comp)
+
+        self._components.extend(components)
+        return components
+
+
     def create_nn(self,
                   model: Union[str, Dict, Path],
                   input: Union[CameraComponent, NNComponent],
                   nn_type: Optional[str] = None,
                   tracker: bool = False,  # Enable object tracker - only for Object detection models
                   spatial: Union[None, bool, StereoComponent] = None,
                   decode_fn: Optional[Callable] = None,
@@ -152,15 +182,16 @@
             input (CameraComponent/NNComponent): Input to the model. If NNComponent (detector), it creates 2-stage NN
             nn_type (str): Type of the network (yolo/mobilenet) for on-device NN result decoding (only needed if blob path was specified)
             tracker: Enable object tracker, if model is object detector (yolo/mobilenet)
             spatial: Calculate 3D spatial coordinates, if model is object detector (yolo/mobilenet) and depth stream is available
             decode_fn: Custom decoding function for the model's output
             name (str): Name used to identify the X-out stream. This name will also be associated with the frame in the callback function.
         """
-        comp = NNComponent(self._pipeline,
+        comp = NNComponent(self._oak.device,
+                           self.pipeline,
                            model=model,
                            input=input,
                            nn_type=nn_type,
                            tracker=tracker,
                            spatial=spatial,
                            decode_fn=decode_fn,
                            replay=self.replay,
@@ -184,15 +215,16 @@
             resolution (str/SensorResolution): If monochrome cameras aren't already passed, create them and set specified resolution
             fps (float): If monochrome cameras aren't already passed, create them and set specified FPS
             left (CameraComponent/dai.node.MonoCamera): Pass the camera object (component/node) that will be used for stereo camera.
             right (CameraComponent/dai.node.MonoCamera): Pass the camera object (component/node) that will be used for stereo camera.
             name (str): Name used to identify the X-out stream. This name will also be associated with the frame in the callback function.
             encode (bool/str/Profile): Whether we want to enable video encoding (accessible via StereoComponent.out.encoded). If True, it will use h264 codec.
         """
-        comp = StereoComponent(self._pipeline,
+        comp = StereoComponent(self._oak.device,
+                               self.pipeline,
                                resolution=resolution,
                                fps=fps,
                                left=left,
                                right=right,
                                replay=self.replay,
                                args=self._args,
                                name=name,
@@ -200,98 +232,103 @@
         self._components.append(comp)
         return comp
 
     def create_imu(self) -> IMUComponent:
         """
         Create IMU component
         """
-        comp = IMUComponent(self._pipeline)
+        comp = IMUComponent(self._oak.device, self.pipeline)
         self._components.append(comp)
         return comp
 
-    def _init_device(self) -> None:
+    def _init_device(self, device_str: Optional[str] = None, usb_speed: Optional[dai.UsbSpeed] = None) -> None:
         """
         Connect to the OAK camera
         """
-        if self._device_name:
-            device_info = dai.DeviceInfo(self._device_name)
+        if device_str is not None:
+            device_info = dai.DeviceInfo(device_str)
         else:
             (found, device_info) = dai.Device.getFirstAvailableDevice()
             if not found:
                 raise Exception("No OAK device found to connect to!")
 
-        if self._usb_speed == dai.UsbSpeed.SUPER:
+        if usb_speed == dai.UsbSpeed.SUPER:
             self._oak.device = dai.Device(
                 version=dai.OpenVINO.VERSION_UNIVERSAL,
                 deviceInfo=device_info,
                 usb2Mode=True
             )
         else:
             self._oak.device = dai.Device(
                 version=dai.OpenVINO.VERSION_UNIVERSAL,
                 deviceInfo=device_info,
-                maxUsbSpeed=dai.UsbSpeed.SUPER if self._usb_speed is None else self._usb_speed
+                maxUsbSpeed=usb_speed or dai.UsbSpeed.SUPER
             )
 
         # TODO test with usb3 (SUPER speed)
-        if self._usb_speed != dai.UsbSpeed.HIGH and self._oak.device.getUsbSpeed() == dai.UsbSpeed.HIGH:
+        if usb_speed != dai.UsbSpeed.HIGH and self._oak.device.getUsbSpeed() == dai.UsbSpeed.HIGH:
             warnings.warn("Device connected in USB2 mode! This might cause some issues. "
                           "In such case, please try using a (different) USB3 cable, "
                           "or force USB2 mode 'with OakCamera(usbSpeed=depthai.UsbSpeed.HIGH)'", UsbWarning)
 
-    def config_camera(self, rotation: Optional[int] = None) -> None:
-        """
-        Configures general camera settings.
-        Args:
-            rotation: Rotate the camera output by this amount of degrees, 0 by default, 90, 180, 270 are supported.
-        """
-        self._rotation = rotation or self._rotation
-
     def config_pipeline(self,
                         xlink_chunk: Optional[int] = None,
                         calib: Optional[dai.CalibrationHandler] = None,
                         tuning_blob: Optional[str] = None,
                         openvino_version: Union[None, str, dai.OpenVINO.Version] = None
                         ):
         """
         Configures DepthAI pipeline.
         @param xlink_chunk: Chunk size of XLink messages. 0 can result in lower latency
         @param calib: Calibration data to be uploaded to OAK
         @param tuning_blob: Camera tuning blob
         @param openvino_version: Force specific OpenVINO version
         """
-        configPipeline(self._pipeline, xlink_chunk, calib, tuning_blob, openvino_version)
+        configPipeline(self.pipeline, xlink_chunk, calib, tuning_blob, openvino_version)
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, tb):
-        print("Closing OAK camera")
+        logging.info("Closing OAK camera")
         if self.replay:
-            print("Closing replay")
+            logging.info("Closing replay")
             self.replay.close()
         if self._oak.device is not None:
             self._oak.device.close()
 
         for out in self._out_templates:
             if isinstance(out, RecordConfig):
                 out.rec.close()
 
     def start(self, blocking=False):
         """
         Start the application - upload the pipeline to the OAK device.
         Args:
             blocking (bool):  Continuously loop and call oak.poll() until program exits
         """
-        if not self._pipeline_built:
-            self.build()  # Build the pipeline
+        self.build()
 
-        self._oak.device.startPipeline(self._pipeline)
+        # Remove unused nodes. There's a better way though.
+        # self._pipeline.
+        # schema = self._pipeline.serializeToJson()['pipeline']
+        # used_nodes = []
+        # for conn in schema['connections']:
+        #     print()
+        #     used_nodes.append(conn["node1Id"])
+        #     used_nodes.append(conn["node2Id"])
+        #
+        # for node in self._pipeline.getAllNodes():
+        #     if node.id not in used_nodes:
+        #         print(f"Removed node {node} (id: {node.id}) from the pipeline as it hasn't been used!")
+        #         self._pipeline.remove(node)
 
-        self._oak.init_callbacks(self._pipeline)
+        self._oak.device.startPipeline(self.pipeline)
+
+        self._oak.init_callbacks(self.pipeline)
 
         for xout in self._oak.oak_out_streams:  # Start FPS counters
             xout.start_fps()
 
         if self.replay:
             self.replay.createQueues(self._oak.device)
             # Called from Replay module on each new frame sent to the device.
@@ -300,14 +337,16 @@
         # Check if callbacks (sync/non-sync are set)
         if blocking:
             # Constant loop: get messages, call callbacks
             while self.running():
                 time.sleep(0.001)
                 self.poll()
 
+            cv2.destroyAllWindows()
+
     def running(self) -> bool:
         """
         Check if camera is running.
         Returns:
             True if camera is running, False otherwise.
         """
         return not self._stop
@@ -327,14 +366,17 @@
             key = -1
 
         # TODO: check if components have controls enabled and check whether key == `control`
 
         self._oak.check_sync()
 
         if self.replay:
+            if key == ord(' '):
+                self.replay.toggle_pause()
+
             if self.replay._stop:
                 self._stop = True
                 return key
 
         for poll in self._polling:
             poll()  # Poll all callbacks
 
@@ -347,60 +389,62 @@
     def build(self) -> dai.Pipeline:
         """
         Connect to the device and build the pipeline based on previously provided configuration. Configure XLink queues,
         upload the pipeline to the device. This function must only be called once!  build() is also called by start().
         Return:
             Built dai.Pipeline
         """
-        if self._pipeline_built:
-            raise Exception('Pipeline can be built only once!')
-
-        self._pipeline_built = True
-        if self.replay:
-            self.replay.initPipeline(self._pipeline)
+        if self._built:
+            return
+        self._built = True
 
         # First go through each component to check whether any is forcing an OpenVINO version
         # TODO: check each component's SHAVE usage
         for c in self._components:
             ov = c.forced_openvino_version()
             if ov:
-                if self._pipeline.getRequiredOpenVINOVersion() and self._pipeline.getRequiredOpenVINOVersion() != ov:
+                if self.pipeline.getRequiredOpenVINOVersion() and self.pipeline.getRequiredOpenVINOVersion() != ov:
                     raise Exception(
                         'Two components forced two different OpenVINO version!'
                         'Please make sure that all your models are compiled using the same OpenVINO version.'
                     )
-                self._pipeline.setOpenVINOVersion(ov)
+                self.pipeline.setOpenVINOVersion(ov)
 
-        if self._pipeline.getRequiredOpenVINOVersion() is None:
+        if self.pipeline.getRequiredOpenVINOVersion() is None:
             # Force 2021.4 as it's better supported (blobconverter, compile tool) for now.
-            self._pipeline.setOpenVINOVersion(dai.OpenVINO.VERSION_2021_4)
+            self.pipeline.setOpenVINOVersion(dai.OpenVINO.VERSION_2021_4)
 
-        # Go through each component
-        for component in self._components:
-            # Update the component now that we can query device info
-            component.on_init(self._pipeline, self._oak.device, self._pipeline.getOpenVINOVersion())
 
         # Create XLinkOuts based on visualizers/callbacks enabled
 
         # TODO: clean this up and potentially move elsewhere
-
         names = []
         for out in self._out_templates:
-            xouts = out.setup(self._pipeline, self._oak.device, names)
+            xouts = out.setup(self.pipeline, self._oak.device, names)
             self._oak.oak_out_streams.extend(xouts)
 
         # User-defined arguments
         if self._args:
             self.config_pipeline(
                 xlink_chunk=self._args.get('xlinkChunkSize', None),
                 tuning_blob=self._args.get('cameraTuning', None),
                 openvino_version=self._args.get('openvinoVersion', None),
             )
 
-        return self._pipeline
+        return self.pipeline
+
+    def _get_component_outputs(self, output: Union[List, Callable, Component]) -> List[Callable]:
+        if not isinstance(output, List):
+            output = [output]
+
+        for i in range(len(output)):
+            if isinstance(output[i], Component):
+                # Select default (main) output of the component
+                output[i] = output[i].out.main
+        return output
 
     def sync(self, outputs: Union[Callable, List[Callable]], callback: Callable, visualize=False):
         """
         Synchronize multiple components outputs forward them to the callback.
         Args:
             outputs: Component output(s)
             callback: Where to send synced streams
@@ -419,39 +463,30 @@
         Record component outputs. This handles syncing multiple streams (eg. left, right, color, depth) and saving
         them to the computer in desired format (raw, mp4, mcap, bag..).
         Args:
             outputs (Component/Component output): Component output(s) to be recorded
             path: Folder path where to save these streams
             record_type: Record type
         """
-        if isinstance(outputs, Callable):
-            outputs = [outputs]  # to list
-
-        for i in range(len(outputs)):
-            if isinstance(outputs[i], Component):
-                outputs[i] = outputs[i].out.main
-
         record = Record(Path(path).resolve(), record_type)
-        self._out_templates.append(RecordConfig(outputs, record))
+        self._out_templates.append(RecordConfig(self._get_component_outputs(outputs), record))
         return record
 
     def show_graph(self):
         """
         Shows DepthAI Pipeline graph, which can be useful when debugging. Builds the pipeline (oak.build()).
         """
-        from depthai_sdk.components.integrations.depthai_pipeline_graph.depthai_pipeline_graph.pipeline_graph import \
+        self.build()
+        from depthai_sdk.integrations.depthai_pipeline_graph.depthai_pipeline_graph.pipeline_graph import \
             PipelineGraph
 
-        if not self._pipeline_built:
-            self.build()  # Build the pipeline
-
         p = PipelineGraph()
-        p.create_graph(self._pipeline.serializeToJson()['pipeline'], self.device)
+        p.create_graph(self.pipeline.serializeToJson()['pipeline'], self.device)
         self._polling.append(p.update)
-        print('process started')
+        logging.info('Process started')
 
     def visualize(self,
                   output: Union[List, Callable, Component],
                   record_path: Optional[str] = None,
                   scale: float = None,
                   fps=False,
                   callback: Callable = None):
@@ -498,14 +533,25 @@
         Args:
             output: Component output(s) to be visualized. If component is passed, SDK will visualize its default output.
             callback: Handler function to which the Packet will be sent.
             enable_visualizer: Whether to enable visualizer for this output.
         """
         self._callback(output, callback, Visualizer() if enable_visualizer else None)
 
+    def ros_stream(self, output: Union[List, Callable, Component]):
+        self._out_templates.append(RosStreamConfig(self._get_component_outputs(output)))
+
+    def set_max_queue_size(self, size: int):
+        """
+        Set maximum queue size for all outputs. This is the maximum number of frames that can be stored in the queue.
+        Args:
+            size: Maximum queue size for all outputs.
+        """
+        self._oak.set_max_queue_size(size)
+
     @property
     def device(self) -> dai.Device:
         """
         Returns dai.Device object. oak.built() has to be called before querying this property!
         """
         return self._oak.device
```

### Comparing `depthai-sdk-1.9.4.1/src/depthai_sdk/oak_device.py` & `depthai-sdk-1.9.5/src/depthai_sdk/oak_device.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 
 class OakDevice:
     def __init__(self):
         self.device: Optional[dai.Device] = None
         # fpsHandlers: Dict[str, FPS] = dict()
         self.oak_out_streams: List[XoutBase] = []
+        self.max_queue_size = 4
 
     @property
     def image_sensors(self) -> List[dai.CameraBoardSocket]:
         """
         Available imageSensors available on the camera
         """
         return self.device.getConnectedCameras()
@@ -23,21 +24,24 @@
         return self.device.getDeviceInfo()
 
     def init_callbacks(self, pipeline: dai.Pipeline):
         for node in pipeline.getAllNodes():
             if isinstance(node, dai.node.XLinkOut):
                 stream_name = node.getStreamName()
                 # self.fpsHandlers[name] = FPS()
-                self.device.getOutputQueue(stream_name, maxSize=4, blocking=False).addCallback(
+                self.device.getOutputQueue(stream_name, maxSize=self.max_queue_size, blocking=False).addCallback(
                     lambda name, msg: self.new_msg(name, msg)
                 )
 
     def new_msg(self, name, msg):
         for sync in self.oak_out_streams:
             sync.new_msg(name, msg)
 
     def check_sync(self):
         """
         Checks whether there are new synced messages, non-blocking.
         """
         for sync in self.oak_out_streams:
             sync.check_queue(block=False)  # Don't block!
+
+    def set_max_queue_size(self, size: int):
+        self.max_queue_size = size
```

### Comparing `depthai-sdk-1.9.4.1/src/depthai_sdk/oak_outputs/normalize_bb.py` & `depthai-sdk-1.9.5/src/depthai_sdk/oak_outputs/normalize_bb.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 from typing import Tuple, Any
-
 import numpy as np
+from depthai_sdk.classes.enum import ResizeMode
 
-from depthai_sdk.components.nn_helper import ResizeMode
 
 
 class NormalizeBoundingBox:
     """
     Normalized bounding box (BB) received from the device. It will also take into account type of aspect ratio
     resize mode and map coordinates to correct location.
     """
-
     def __init__(self, aspect_ratio: Tuple[float, float], resize_mode: ResizeMode):
         """
         :param aspect_ratio: NN input size
         :param resize_mode: Aspect ratio resize mode
         """
         self.aspect_ratio = aspect_ratio
         self.resize_mode = resize_mode
@@ -29,14 +27,15 @@
 
         Returns:
             list: Bounding box points mapped to pixel values on frame
         """
         bbox = np.array(bbox)
 
         # Edit the bounding boxes before normalizing them
+
         if self.resize_mode == ResizeMode.CROP:
             ar_diff = (self.aspect_ratio[0] / self.aspect_ratio[1]) / (frame.shape[1] / frame.shape[0])
             if ar_diff < 1:
                 new_w = frame.shape[1] * ar_diff
                 new_h = frame.shape[0]
                 bbox[0] = bbox[0] * new_w + (frame.shape[1] - new_w) / 2
                 bbox[1] = bbox[1] * new_h
```

### Comparing `depthai-sdk-1.9.4.1/src/depthai_sdk/oak_outputs/syncing.py` & `depthai-sdk-1.9.5/src/depthai_sdk/oak_outputs/syncing.py`

 * *Files identical despite different names*

### Comparing `depthai-sdk-1.9.4.1/src/depthai_sdk/oak_outputs/xout/xout_depth.py` & `depthai-sdk-1.9.5/src/depthai_sdk/oak_outputs/xout/xout_depth.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import logging
+import warnings
 from typing import List
 
 import depthai as dai
 import numpy as np
 
 from depthai_sdk.classes.packets import DepthPacket
 from depthai_sdk.oak_outputs.xout import Clickable
@@ -39,15 +41,17 @@
         self.colorize = colorize
         self.colormap = colormap
 
         self.use_wls_filter = use_wls_filter
 
         # Prefer to use WLS level if set, otherwise use lambda and sigma
         if wls_level and use_wls_filter:
-            print(f'Using WLS level: {wls_level.name} (lambda: {wls_level.value[0]}, sigma: {wls_level.value[1]})')
+            logging.debug(
+                f'Using WLS level: {wls_level.name} (lambda: {wls_level.value[0]}, sigma: {wls_level.value[1]})'
+            )
             self.wls_lambda = wls_level.value[0]
             self.wls_sigma = wls_level.value[1]
         else:
             self.wls_lambda = wls_lambda
             self.wls_sigma = wls_sigma
 
         self.wls_filter = None
@@ -56,18 +60,26 @@
     def setup_visualize(self,
                         visualizer: Visualizer,
                         visualizer_enabled: bool,
                         name: str = None):
         super().setup_visualize(visualizer, visualizer_enabled, name)
 
         if self._visualizer.config.stereo.wls_filter or self.use_wls_filter:
-            self.wls_filter = cv2.ximgproc.createDisparityWLSFilterGeneric(False)
+            try:
+                self.wls_filter = cv2.ximgproc.createDisparityWLSFilterGeneric(False)
+            except AttributeError:
+                warnings.warn(
+                    'OpenCV version does not support WLS filter. Disabling WLS filter. '
+                    'Make sure you have opencv-contrib-python installed. '
+                    'If not, run "pip uninstall opencv-python && pip install opencv-contrib-python -U"'
+                )
+                self.use_wls_filter = False
 
     def visualize(self, packet: DepthPacket):
-        depth_frame = packet.imgFrame.getFrame()
+        depth_frame = packet.msg.getFrame()
 
         stereo_config = self._visualizer.config.stereo
 
         if self.use_wls_filter or stereo_config.wls_filter:
             self.wls_filter.setLambda(stereo_config.wls_lambda)
             self.wls_filter.setSigmaColor(stereo_config.wls_sigma)
             depth_frame = self.wls_filter.filter(depth_frame, packet.mono_frame.getCvFrame())
```

### Comparing `depthai-sdk-1.9.4.1/src/depthai_sdk/oak_outputs/xout/xout_disparity.py` & `depthai-sdk-1.9.5/src/depthai_sdk/oak_outputs/xout/xout_disparity.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import logging
+import warnings
 from typing import List
 
 import depthai as dai
 import numpy as np
 
 from depthai_sdk.classes.packets import DepthPacket
 from depthai_sdk.oak_outputs.xout import Clickable
@@ -37,23 +39,33 @@
         self.colorize = colorize
         self.colormap = colormap
 
         self.use_wls_filter = use_wls_filter
 
         # Prefer to use WLS level if set, otherwise use lambda and sigma
         if wls_level and use_wls_filter:
-            print(f'Using WLS level: {wls_level.name} (lambda: {wls_level.value[0]}, sigma: {wls_level.value[1]})')
+            logging.debug(
+                f'Using WLS level: {wls_level.name} (lambda: {wls_level.value[0]}, sigma: {wls_level.value[1]})'
+            )
             self.wls_lambda = wls_level.value[0]
             self.wls_sigma = wls_level.value[1]
         else:
             self.wls_lambda = wls_lambda
             self.wls_sigma = wls_sigma
 
         if self.use_wls_filter:
-            self.wls_filter = cv2.ximgproc.createDisparityWLSFilterGeneric(False)
+            try:
+                self.wls_filter = cv2.ximgproc.createDisparityWLSFilterGeneric(False)
+            except AttributeError:
+                warnings.warn(
+                    'OpenCV version does not support WLS filter. Disabling WLS filter. '
+                    'Make sure you have opencv-contrib-python installed. '
+                    'If not, run "pip uninstall opencv-python && pip install opencv-contrib-python -U"'
+                )
+                self.use_wls_filter = False
 
         self.msgs = dict()
 
         XoutFrames.__init__(self, frames=disparity_frames, fps=fps)
         Clickable.__init__(self, decay_step=int(self.fps))
 
     def visualize(self, packet: DepthPacket):
```

### Comparing `depthai-sdk-1.9.4.1/src/depthai_sdk/oak_outputs/xout/xout_frames.py` & `depthai-sdk-1.9.5/src/depthai_sdk/oak_outputs/xout/xout_frames.py`

 * *Files 4% similar despite different names*

```diff
@@ -73,15 +73,15 @@
             else:
                 pass
 
     def on_record(self, packet) -> None:
         if self._video_recorder:
             # TODO not ideal to check it this way
             if isinstance(self._video_recorder[self.name], AvWriter):
-                self._video_recorder.write(self.name, packet.imgFrame)
+                self._video_recorder.write(self.name, packet.msg)
             else:
                 self._video_recorder.write(self.name, packet.frame)
         # else:
         #     self._video_recorder.add_to_buffer(self.name, packet.frame)
 
     def xstreams(self) -> List[StreamXout]:
         return [self.frames]
```

### Comparing `depthai-sdk-1.9.4.1/src/depthai_sdk/oak_outputs/xout/xout_h26x.py` & `depthai-sdk-1.9.5/src/depthai_sdk/oak_outputs/xout/xout_h26x.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         fourcc = 'hevc' if profile == dai.VideoEncoderProperties.Profile.H265_MAIN else 'h264'
         self.codec = av.CodecContext.create(fourcc, "r") if av else None
 
     def decode_frame(self, packet: FramePacket):
         if not self.codec:
             raise ImportError('av is not installed. Please install it with `pip install av`')
 
-        enc_packets = self.codec.parse(packet.imgFrame.getData())
+        enc_packets = self.codec.parse(packet.msg.getData())
         if len(enc_packets) == 0:
             return None
 
         frames = self.codec.decode(enc_packets[-1])
         if not frames:
             return None
```

### Comparing `depthai-sdk-1.9.4.1/src/depthai_sdk/oak_outputs/xout/xout_imu.py` & `depthai-sdk-1.9.5/src/depthai_sdk/oak_outputs/xout/xout_imu.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,34 +38,35 @@
 
         self._visualizer = visualizer
         self._visualizer_enabled = visualizer_enabled
         self.name = name or self.name
 
         self.fig, self.axes = plt.subplots(2, 1, figsize=(10, 10), constrained_layout=True)
         labels = ['x', 'y', 'z']
+        colors = ['r', 'g', 'b']
 
         for i in range(3):
-            self.acceleration_lines.append(self.axes[0].plot([], [], label=f'Acceleration {labels[i]}')[0])
+            self.acceleration_lines.append(self.axes[0].plot([], [], label=f'Acceleration {labels[i]}', color=colors[i])[0])
             self.axes[0].set_ylabel('Acceleration (m/s^2)')
             self.axes[0].set_xlabel('Time (s)')
             self.axes[0].legend()
 
         for i in range(3):
-            self.gyroscope_lines.append(self.axes[1].plot([], [], label=f'Gyroscope {labels[i]}')[0])
+            self.gyroscope_lines.append(self.axes[1].plot([], [], label=f'Gyroscope {labels[i]}', color=colors[i])[0])
             self.axes[1].set_ylabel('Gyroscope (rad/s)')
             self.axes[1].set_xlabel('Time (s)')
             self.axes[1].legend()
 
     def visualize(self, packet: IMUPacket):
         if self.start_time == 0.0:
             self.start_time = packet.data[0].acceleroMeter.timestamp.get()
 
         acceleration_x = [el.acceleroMeter.x for el in packet.data]
-        acceleration_z = [el.acceleroMeter.y for el in packet.data]
-        acceleration_y = [el.acceleroMeter.z for el in packet.data]
+        acceleration_y = [el.acceleroMeter.y for el in packet.data]
+        acceleration_z = [el.acceleroMeter.z for el in packet.data]
 
         t_acceleration = [(el.acceleroMeter.timestamp.get() - self.start_time).total_seconds() for el in packet.data]
 
         # Keep only last 100 values
         if len(self.acceleration_buffer) > 100:
             self.acceleration_buffer.pop(0)
 
@@ -107,15 +108,14 @@
         img = cv2.cvtColor(img, cv2.COLOR_RGB2BGR)
 
         packet.frame = img
 
         if self.callback:  # Don't display frame, call the callback
             self.callback(packet)
         else:
-            packet.frame = self._visualizer.draw(packet.frame)
             cv2.imshow(self.name, packet.frame)
 
     def xstreams(self) -> List[StreamXout]:
         return [self.imu_out]
 
     def new_msg(self, name: str, msg: dai.IMUData) -> None:
         if name not in self._streams:
```

### Comparing `depthai-sdk-1.9.4.1/src/depthai_sdk/oak_outputs/xout/xout_mjpeg.py` & `depthai-sdk-1.9.5/src/depthai_sdk/oak_outputs/xout/xout_mjpeg.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,12 +23,12 @@
         self.fps = fps
         self._frame_shape = frame_shape
 
         if lossless and self._visualizer:
             raise ValueError('Visualizing Lossless MJPEG stream is not supported!')
 
     def decode_frame(self, packet: FramePacket) -> np.ndarray:
-        return cv2.imdecode(packet.imgFrame.getData(), self.flag)
+        return cv2.imdecode(packet.msg.getData(), self.flag)
 
     def visualize(self, packet: FramePacket):
         packet.frame = self.decode_frame(packet)
         super().visualize(packet)
```

### Comparing `depthai-sdk-1.9.4.1/src/depthai_sdk/oak_outputs/xout/xout_nn.py` & `depthai-sdk-1.9.5/src/depthai_sdk/oak_outputs/xout/xout_nn.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,53 @@
 from typing import List, Union, Dict, Any, Optional, Tuple
 
 import depthai as dai
 import numpy as np
 from distinctipy import distinctipy
 
 from depthai_sdk.classes import Detections, ImgLandmarks, SemanticSegmentation
+from depthai_sdk.classes.enum import ResizeMode
 from depthai_sdk.classes.packets import (
-    _Detection, DetectionPacket, TrackerPacket, SpatialBbMappingPacket, TwoStagePacket
+    _Detection, DetectionPacket, TrackerPacket, SpatialBbMappingPacket, TwoStagePacket, NNDataPacket
 )
-from depthai_sdk.components.nn_helper import ResizeMode
+from depthai_sdk.classes.enum import ResizeMode
 from depthai_sdk.oak_outputs.normalize_bb import NormalizeBoundingBox
-from depthai_sdk.oak_outputs.xout.xout_base import StreamXout
+from depthai_sdk.oak_outputs.xout.xout_base import XoutBase, StreamXout
 from depthai_sdk.oak_outputs.xout.xout_frames import XoutFrames
 from depthai_sdk.oak_outputs.xout.xout_seq_sync import XoutSeqSync
 from depthai_sdk.visualize.visualizer import Visualizer
 from depthai_sdk.visualize.visualizer_helper import hex_to_bgr, calc_disp_multiplier, colorize_disparity, draw_mappings
 
 try:
     import cv2
 except ImportError:
     cv2 = None
 
+class XoutNnData(XoutBase):
+    def __init__(self, xout: StreamXout):
+        self.nndata_out = xout
+        super().__init__()
+        self.name = 'NNData'
+
+    def visualize(self, packet: NNDataPacket):
+        print('Visualization of NNData is not supported')
+
+    def xstreams(self) -> List[StreamXout]:
+        return [self.nndata_out]
+
+    def new_msg(self, name: str, msg: dai.NNData) -> None:
+        if name not in self._streams:
+            return
+
+        if self.queue.full():
+            self.queue.get()  # Get one, so queue isn't full
+
+        packet = NNDataPacket(name=self.name, nn_data=msg)
+        self.queue.put(packet, block=False)
+
 
 class XoutNnResults(XoutSeqSync, XoutFrames):
     def xstreams(self) -> List[StreamXout]:
         return [self.nn_results, self.frames]
 
     def __init__(self,
                  det_nn: 'NNComponent',
@@ -55,40 +78,47 @@
                     color = hex_to_bgr(label[1])
                 else:
                     raise ValueError('Model JSON config error. Label map list can have either str or list!')
 
                 self.labels.append((text, color))
 
         self.normalizer = NormalizeBoundingBox(det_nn._size, det_nn._ar_resize_mode)
-        try:
-            self._frame_shape = self.det_nn._input.node.getPreviewSize()
-        except AttributeError:
-            self._frame_shape = self.det_nn._input.stream_size  # Replay
 
-        self._frame_shape = np.array(self._frame_shape)[::-1]
+        self._frame_shape = None
+        if isinstance(self.det_nn._input, dai.Node.Output):
+            pass # No good way to get size of dai.Node.Output. We will set it on first received frame
+        else: # CameeraComponent / NNComponent
+            if isinstance(self.det_nn._input.node, dai.node.ColorCamera):
+                self._frame_shape = self.det_nn._input.node.getPreviewSize()
+            elif isinstance(self.det_nn._input.node, dai.node.MonoCamera):
+                self._frame_shape = self.det_nn._input.node.getResolutionSize()
+            elif isinstance(self.det_nn._input.node, dai.node.XLinkIn): # Replay
+                self._frame_shape = self.det_nn._input.stream_size
+            # [width, height] to [height, width]
+            self._frame_shape = np.array(self._frame_shape)[::-1]
 
         self.segmentation_colormap = None
 
     def setup_visualize(self,
                         visualizer: Visualizer,
                         visualizer_enabled: bool,
                         name: str = None):
         super().setup_visualize(visualizer, visualizer_enabled, name)
 
     def on_callback(self, packet: Union[DetectionPacket, TrackerPacket]):
-        if self._visualizer and self._visualizer.frame_shape is None:
-            try:
-                shape = packet.imgFrame.getCvFrame().shape[:2]
-            except RuntimeError as e:
-                raise RuntimeError(f'Error getting frame shape - {e}')
-            if len(shape) == 1:
-                self._visualizer.frame_shape = self._frame_shape
-            else:
-                self._visualizer.frame_shape = shape
-                self._frame_shape = shape
+        # Convert Grayscale to BGR
+        if len(packet.frame.shape) == 2:
+            packet.frame = np.dstack((packet.frame, packet.frame, packet.frame))
+
+        if self._frame_shape is None:
+            # Lazy-load the frame shape
+            self._frame_shape = np.array([packet.frame.shape[0], packet.frame.shape[1]])
+
+        if self._visualizer:
+            self._visualizer.frame_shape = self._frame_shape
 
         # Add detections to packet
         if isinstance(packet.img_detections, dai.ImgDetections) \
                 or isinstance(packet.img_detections, dai.SpatialImgDetections) \
                 or isinstance(packet.img_detections, Detections):
             for detection in packet.img_detections.detections:
                 d = _Detection()
@@ -133,21 +163,26 @@
 
             # Generate colormap if not already generated
             if self.segmentation_colormap is None:
                 n_classes = len(self.labels) if self.labels else 8
                 self.segmentation_colormap = self._generate_colors(n_classes)
 
             mask = np.array(packet.img_detections.mask).astype(np.uint8)
+
+            if mask.ndim == 3:
+                mask = np.argmax(mask, axis=0)
+
             try:
                 colorized_mask = np.array(self.segmentation_colormap)[mask]
             except IndexError:
                 unique_classes = np.unique(mask)
                 max_class = np.max(unique_classes)
                 new_colors = self._generate_colors(max_class - len(self.segmentation_colormap) + 1)
                 self.segmentation_colormap.extend(new_colors)
+                colorized_mask = np.array(self.segmentation_colormap)[mask]
 
             bbox = None
             if self.normalizer.resize_mode == ResizeMode.LETTERBOX:
                 bbox = self.normalizer.get_letterbox_bbox(packet.frame, normalize=True)
                 input_h, input_w = self.normalizer.aspect_ratio
                 resize_bbox = bbox[0] * input_w, bbox[1] * input_h, bbox[2] * input_w, bbox[3] * input_h
                 resize_bbox = np.int0(resize_bbox)
@@ -180,15 +215,27 @@
             msgs[self.frames.name],
             msgs[self.nn_results.name] if decode_fn is None else decode_fn(msgs[self.nn_results.name]),
             self._visualizer
         )
 
         self.queue.put(packet, block=False)
 
-    def _generate_colors(self, n_colors, exclude=None):
+    def _set_frame_shape(self, packet):
+        try:
+            shape = packet.msg.getCvFrame().shape[:2]
+        except RuntimeError as e:
+            raise RuntimeError(f'Error getting frame shape - {e}')
+        if self._visualizer and self._visualizer.frame_shape is None and len(shape) == 1:
+            self._visualizer.frame_shape = self._frame_shape
+        else:
+            self._visualizer.frame_shape = shape
+            self._frame_shape = shape
+
+    @staticmethod
+    def _generate_colors(n_colors, exclude=None):
         colors = distinctipy.get_colors(n_colors, exclude / 255 if exclude else None,
                                         rng=11, pastel_factor=0.3, n_attempts=100)
         rgb_colors = np.array(colors) * 255
         return rgb_colors.astype(np.uint8)
 
 
 class XoutSpatialBbMappings(XoutSeqSync, XoutFrames):
@@ -205,19 +252,19 @@
         self.name = 'Depth & Bounding Boxes'
 
     def xstreams(self) -> List[StreamXout]:
         return [self.frames, self.configs]
 
     def visualize(self, packet: SpatialBbMappingPacket):
         if not self.factor:
-            size = (packet.imgFrame.getWidth(), packet.imgFrame.getHeight())
+            size = (packet.msg.getWidth(), packet.msg.getHeight())
             self.factor = calc_disp_multiplier(self.device, size)
 
-        depth = np.array(packet.imgFrame.getFrame())
-        with np.errstate(divide='ignore'):
+        depth = np.array(packet.msg.getFrame())
+        with np.errstate(all='ignore'):
             disp = (self.factor / depth).astype(np.uint8)
 
         packet.frame = colorize_disparity(disp, multiplier=self.multiplier)
         draw_mappings(packet)
 
         super().visualize(packet)
```

### Comparing `depthai-sdk-1.9.4.1/src/depthai_sdk/oak_outputs/xout/xout_nn_encoded.py` & `depthai-sdk-1.9.5/src/depthai_sdk/oak_outputs/xout/xout_nn_encoded.py`

 * *Files identical despite different names*

### Comparing `depthai-sdk-1.9.4.1/src/depthai_sdk/oak_outputs/xout/xout_seq_sync.py` & `depthai-sdk-1.9.5/src/depthai_sdk/oak_outputs/xout/xout_seq_sync.py`

 * *Files identical despite different names*

### Comparing `depthai-sdk-1.9.4.1/src/depthai_sdk/previews.py` & `depthai-sdk-1.9.5/src/depthai_sdk/previews.py`

 * *Files identical despite different names*

### Comparing `depthai-sdk-1.9.4.1/src/depthai_sdk/readers/abstract_reader.py` & `depthai-sdk-1.9.5/src/depthai_sdk/readers/abstract_reader.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import os
 from abc import ABC, abstractmethod
 from pathlib import Path
-from typing import List, Tuple
-
+from typing import List, Tuple, Dict
+import numpy as np
 
 class AbstractReader(ABC):
     @abstractmethod
-    def read(self):
+    def read(self) -> Dict[str, np.ndarray]:
         """
         Read a frame (or multiple frames) from the reader.
         @return: Single np.ndarray, or dict of frames and their names. None if frames weren't read or there was an error.
         """
         pass
 
     @abstractmethod
@@ -21,14 +21,22 @@
     def getShape(self, name: str) -> Tuple[int, int]:
         """
         Returns (width, height)
         """
         pass
 
     @abstractmethod
+    def get_message_size(self, name: str) -> int:
+        """
+        @param name: Stream name
+        @return: Number of bytes for that this message contains
+        """
+        pass
+
+    @abstractmethod
     def close(self):
         pass
 
     @abstractmethod
     def disableStream(self, name: str):
         """
         @param name: Name of the stream to be disabled
```

### Comparing `depthai-sdk-1.9.4.1/src/depthai_sdk/readers/db3_reader.py` & `depthai-sdk-1.9.5/src/depthai_sdk/readers/db3_reader.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,15 +7,17 @@
 from rosbags.serde import deserialize_cdr
 
 from depthai_sdk.previews import PreviewDecoder
 from depthai_sdk.readers.abstract_reader import AbstractReader
 
 
 class Db3Reader(AbstractReader):
-    STREAMS = ['left', 'right', 'depth']
+    STREAMS = ['left', 'right', 'rgb', 'depth']
+    generators: Dict[str, Generator] = {}
+    frames = None  # For shapes
 
     def __init__(self, folder: Path) -> None:
         self.reader = Reader(str(folder))
         self.reader.open()
         self.generators: Dict[str, Generator] = {}
         self.frames = None  # For shapes
 
@@ -28,16 +30,18 @@
         self.frames = self.read()
 
         for con in self.reader.connections:
             for stream in self.STREAMS:
                 if stream.lower() in con.topic.lower():
                     self.generators[stream.lower()] = self.reader.messages([con])
 
-    def read(self):
-        ros_msgs: Dict[str, Any] = dict()
+
+    def read(self) -> Dict[str, np.ndarray]:
+        ros_msgs: Dict[str, np.ndarray] = dict()
+
         try:
             for name, gen in self.generators.items():
                 con, ts, raw = next(gen)
                 ros_msgs[name] = self._getCvFrame(deserialize_cdr(raw, con.msgtype), name)
             return ros_msgs
         except:
             return None
@@ -48,14 +52,15 @@
 
     def _getCvFrame(self, msg, name: str):
         """
         Convert ROS message to cv2 frame (numpy array)
         """
         msg_type = str(type(msg))
         data = np.frombuffer(msg.data, dtype=np.int8)
+
         if 'CompressedImage' in msg_type:
             if name == 'color':
                 return PreviewDecoder.jpegDecode(data, cv2.IMREAD_COLOR)
             else:  # left, right, disparity
                 return PreviewDecoder.jpegDecode(data, cv2.IMREAD_GRAYSCALE)
         elif 'Image' in msg_type:
             if msg.encoding == 'mono16':
@@ -69,9 +74,15 @@
         streams = [name for name in self.frames]
         return streams
 
     def getShape(self, name: str) -> Tuple[int, int]:
         frame = self.frames[name]
         return (frame.shape[1], frame.shape[0])
 
+    def get_message_size(self, name: str) -> int:
+        size = 1
+        for shape in self.frames[name].shape:
+            size *= shape
+        return size
+
     def close(self):
         self.reader.close()
```

### Comparing `depthai-sdk-1.9.4.1/src/depthai_sdk/readers/image_reader.py` & `depthai-sdk-1.9.5/src/depthai_sdk/readers/image_reader.py`

 * *Files 8% similar despite different names*

```diff
@@ -38,15 +38,15 @@
         self.cntr: Dict[str, int] = dict()
 
         if path.is_file():
             stream, flag = get_name_flag(path.stem)
             self.frames[stream].append(cv2.imread(str(path), flag))
         else:
             shape = None
-            for fileName in os.listdir(str(path)):
+            for fileName in sorted(os.listdir(str(path))):
                 f_name, ext = os.path.splitext(fileName)
                 if ext not in _imageExt: continue
                 stream, flag = get_name_flag(f_name)
 
                 frame = cv2.imread(str(path / fileName), flag)
                 if shape is None:
                     shape = (frame.shape[1], frame.shape[0])
@@ -54,20 +54,24 @@
                 frame = cv2.resize(frame, shape)
 
                 self.frames[stream].append(frame)
 
         for name, arr in self.frames.items():
             self.cntr[name] = 0
 
-        self.cycle = time.time()
+        self.last_cycle_time = time.time()
+        self.cycle_sec = 3.0 # Images get cycled every 3 seconds by default
 
-    def read(self):
+    def set_cycle_fps(self, fps): # Called from replay.py on set_fps()
+        self.cycle_sec = 1.0 / fps
+
+    def read(self) -> Dict[str, np.ndarray]:
         # Increase counters
-        if 3 < time.time() - self.cycle:
-            self.cycle = time.time()
+        if self.cycle_sec < time.time() - self.last_cycle_time:
+            self.last_cycle_time = time.time()
             for name in self.cntr:
                 self.cntr[name] += 1
                 if len(self.frames[name]) <= self.cntr[name]:
                     self.cntr[name] = 0
 
         msgs: Dict[str, np.ndarray] = dict()
         for name, arr in self.frames.items():
@@ -82,13 +86,19 @@
                 streams.append(name)
         return streams
 
     def getShape(self, name: str) -> Tuple[int, int]:
         shape = self.frames[name][0].shape
         return (shape[1], shape[0])
 
+    def get_message_size(self, name: str) -> int:
+        size = 1
+        for shape in self.frames[name][0].shape:
+            size *= shape
+        return size
+
     def close(self):
         pass
 
     def disableStream(self, name: str):
         if name in self.frames:
             self.frames[name] = []
```

### Comparing `depthai-sdk-1.9.4.1/src/depthai_sdk/readers/mcap_reader.py` & `depthai-sdk-1.9.5/src/depthai_sdk/readers/mcap_reader.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from pathlib import Path
-from typing import List, Tuple
+from typing import List, Tuple, Dict
 
 import cv2
 import numpy as np
 from mcap.mcap0.reader import make_reader
 from mcap.mcap0.stream_reader import StreamReader
 from mcap_ros1.decoder import Decoder
 
@@ -15,33 +15,33 @@
     """
     Reads all saved streams from .mcap recording.
     Supported ROS messages: Image (depth), CompressedImage (left, right, color, disparity)
     """
 
     def __init__(self, folder: Path) -> None:
         # Get available topics
-        with open(source, "rb") as file:
+        with open(folder, "rb") as file:
             reader = make_reader(file)
             channels = reader.get_summary().channels
             self._topics = [c.topic.split('/')[0] for _, c in channels.items()]
 
         self._readFrames = dict()
 
         # Init msg array
         for topic in self._topics:
             self._readFrames[topic] = []
 
         # Create MCAP decoder
-        decoder = Decoder(StreamReader(str(source)))
+        decoder = Decoder(StreamReader(str(folder)))
         self.msgs = decoder.messages
         # Prepare initial frames so we can get frame size
 
         self._prepareFrames()
 
-    def read(self):
+    def read(self) -> Dict[str, np.ndarray]:
         """
         Read and return one frame from each available stream.
         """
         self._prepareFrames()
         return self._returnFrames()
 
     def _prepareFrames(self):
@@ -77,15 +77,15 @@
         """
         Check if there is at least one frame from each available stream.
         """
         for _, arr in self._readFrames.items():
             if len(arr) < 1: return False
         return True
 
-    def _returnFrames(self):
+    def _returnFrames(self) -> Dict[str, np.ndarray]:
         """
         Return synced frames (one of each available).
         """
         ret = dict()
         for name, arr in self._readFrames.items():
             ret[name] = arr.pop(0)
         return ret
@@ -96,9 +96,15 @@
         """
         return [name for name in self._topics]
 
     def getShape(self, name: str) -> Tuple[int, int]:
         frame = self._readFrames[name][0]
         return (frame.shape[1], frame.shape[0])
 
+    def get_message_size(self, name: str) -> int:
+        size = 1
+        for shape in self._readFrames[name][0].shape:
+            size *= shape
+        return size
+
     def close(self):
         pass
```

### Comparing `depthai-sdk-1.9.4.1/src/depthai_sdk/readers/rosbag_reader.py` & `depthai-sdk-1.9.5/src/depthai_sdk/readers/rosbag_reader.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,28 +10,35 @@
 
 class RosbagReader(AbstractReader):
     """
     TODO: make the stream selectable, add function that returns all available streams
     """
 
     def __init__(self, folder: Path) -> None:
-        self.reader = Reader(source)
+        self.reader = Reader(folder)
         self.reader.open()
         if '/device_0/sensor_0/Depth_0/image/data' not in self.reader.topics:
             raise Exception("Provided rosbag can't find required topic (`/device_0/sensor_0/Depth_0/image/data`)")
         self.generator = self.reader.messages('/device_0/sensor_0/Depth_0/image/data')
 
     def read(self):
         connection, _, rawdata = next(self.generator)
         msg = deserialize_cdr(ros1_to_cdr(rawdata, connection.msgtype), connection.msgtype)
-        return msg.data.view(np.int16).reshape((msg.height, msg.width))
+        return {
+            'depth': msg.data.view(np.int16).reshape((msg.height, msg.width))
+        }
 
     def getStreams(self) -> List[str]:
         return ["depth"]  # Only depth recording is supported
 
     def getShape(self, name: str) -> Tuple[int, int]:
         connection, _, rawdata = next(self.reader.messages('/device_0/sensor_0/Depth_0/image/data'))
         msg = deserialize_cdr(ros1_to_cdr(rawdata, connection.msgtype), connection.msgtype)
         return (msg.width, msg.height)
 
+    def get_message_size(self, name: str) -> int:
+        connection, _, rawdata = next(self.reader.messages('/device_0/sensor_0/Depth_0/image/data'))
+        msg = deserialize_cdr(ros1_to_cdr(rawdata, connection.msgtype), connection.msgtype)
+        return len(msg.data) # TODO: test
+
     def close(self):
         self.reader.close()
```

### Comparing `depthai-sdk-1.9.4.1/src/depthai_sdk/record.py` & `depthai-sdk-1.9.5/src/depthai_sdk/record.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 #!/usr/bin/env python3
+import logging
 from enum import IntEnum
 from pathlib import Path
 from queue import Queue
 from threading import Thread
 from typing import Dict, List
 
 import depthai as dai
@@ -26,28 +27,28 @@
             for name in frames:
                 # Save all synced frames into files
                 recorder.write(name, frames[name])
         except KeyboardInterrupt:
             break
     # Close all recorders - Can't use ExitStack with VideoWriter
     recorder.close()
-    print('Exiting store frame thread')
+    logging.info('Exiting store frame thread')
 
 
 class RecordType(IntEnum):
     VIDEO = 1  # Save to video file
-    BAG = 2  # To ROS .bag
+    ROSBAG = 2  # To ROS .bag
     MCAP = 3  # To .mcap
+    DB3 = 4 # To .db3 (ros2)
 
 
 class Record(XoutSeqSync):
     """
     This class records depthai streams from OAK cameras into different formats.
-    Available formats: .h265, .mjpeg, .mp4, .mcap, .bag
-    It will also save calibration .json, so depth reconstruction will
+    It will also save calibration .json, so depth reconstruction will be possible.
     """
 
     def __init__(self, path: Path, record_type: RecordType):
         """
         Args:
             path (Path): Path to the recording folder
             record_type (RecordType): Recording type
@@ -65,17 +66,20 @@
 
         if self.record_type == RecordType.MCAP:
             from .recorders.mcap_recorder import McapRecorder
             self.recorder = McapRecorder()
         elif self.record_type == RecordType.VIDEO:
             from .recorders.video_recorder import VideoRecorder
             self.recorder = VideoRecorder()
-        elif self.record_type == RecordType.BAG:
-            from .recorders.rosbag_recorder import RosbagRecorder
-            self.recorder = RosbagRecorder()
+        elif self.record_type == RecordType.ROSBAG:
+            from .recorders.rosbag_recorder import Rosbag1Recorder
+            self.recorder = Rosbag1Recorder()
+        elif self.record_type == RecordType.DB3:
+            from .recorders.rosbag_recorder import Rosbag2Recorder
+            self.recorder = Rosbag2Recorder()
         else:
             raise ValueError(f"Recording type '{self.record_type}' isn't supported!")
 
     def package(self, msgs: Dict):
         # Here we get sequence-num synced messages:)
         mapped = dict()
         for name, msg in msgs.items():
@@ -101,15 +105,15 @@
         """
         if self.record_type == RecordType.VIDEO:
             self._streams = [out.frames.name for out in xouts]  # required by XoutSeqSync
             self.stream_num = len(xouts)
             self.name_mapping = dict()
             for xout in xouts:
                 self.name_mapping[xout.frames.name] = xout.name
-        else:  # For MCAP/Ros bags we don't need msg syncing
+        else:  # For MCAP/Rosbags we don't need msg syncing
             self.new_msg = self.no_sync
 
         self.mxid = device.getMxId()
         self.path = self._create_folder(self.folder, self.mxid)
         calib_data = device.readCalibration()
         calib_data.eepromToJsonFile(str(self.path / "calib.json"))
 
@@ -118,15 +122,15 @@
         self.frame_q = Queue(maxsize=20)
         self.process = Thread(target=_run, args=(self.recorder, self.frame_q))
         self.process.start()
 
     # TODO: support pointclouds in MCAP
     def config_mcap(self, pointcloud: bool):
         if self.record_type != RecordType.MCAP:
-            print(f"Recorder type is {self.record_type}, not MCAP! Config attempt ignored.")
+            logging.info(f"Recorder type is {self.record_type}, not MCAP! Config attempt ignored.")
             return
         self.recorder.set_pointcloud(pointcloud)
 
     # def config_video(self, ):
     # Nothing to configure for video recorder
 
     # TODO: implement config of BAG to either record depth as frame or pointcloud
```

### Comparing `depthai-sdk-1.9.4.1/src/depthai_sdk/recorders/abstract_recorder.py` & `depthai-sdk-1.9.5/src/depthai_sdk/recorders/abstract_recorder.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 from abc import ABC, abstractmethod
-from enum import IntEnum
 from pathlib import Path
 from typing import List
-
 import depthai as dai
-
-import depthai_sdk
 import depthai_sdk.oak_outputs.xout as outputs
+from enum import IntEnum
 
 
 class Recorder(ABC):
     @abstractmethod
     def write(self, name: str, frame: dai.ImgFrame):
         raise NotImplementedError()
 
@@ -29,30 +26,30 @@
         MJPEG = 1
         H264 = 2
         H265 = 3
         DEPTH = 4  # 16 bit
         IMU = 5
 
     def __init__(self, xout: outputs.xout_base.XoutBase):
-        if isinstance(xout, depthai_sdk.oak_outputs.xout.xout_mjpeg.XoutMjpeg):
+        if isinstance(xout, outputs.xout_mjpeg.XoutMjpeg):
             self.type = self.StreamType.MJPEG
             self.xlink_name = xout.frames.name
         elif isinstance(xout, outputs.xout_h26x.XoutH26x):
             self.xlink_name = xout.frames.name
             if xout.profile == dai.VideoEncoderProperties.Profile.H265_MAIN:
                 self.type = self.StreamType.H265
             else:
                 self.type = self.StreamType.H264
         elif isinstance(xout, outputs.xout_depth.XoutDepth):
             self.xlink_name = xout.frames.name
             self.type = self.StreamType.DEPTH  # TODO is depth raw or should it be DEPTH?
         elif isinstance(xout, outputs.xout_disparity.XoutDisparity):
             self.xlink_name = xout.frames.name
             self.type = self.StreamType.RAW
-        elif isinstance(xout, depthai_sdk.oak_outputs.xout.xout_frames.XoutFrames):
+        elif isinstance(xout, outputs.xout_frames.XoutFrames):
             self.xlink_name = xout.frames.name
             self.type = self.StreamType.RAW
         elif isinstance(xout, outputs.XoutIMU):
             self.xlink_name = xout.imu_out.name
             self.type = self.StreamType.IMU
         else:
             raise ValueError("You have passed invalid Component Output to the Recorder!")
```

### Comparing `depthai-sdk-1.9.4.1/src/depthai_sdk/recorders/rosbag_recorder.py` & `depthai-sdk-1.9.5/src/depthai_sdk/recorders/rosbag_recorder.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,44 @@
 '''
 This is a helper class that let's you save depth frames into rosbag (.bag), which can be replayed using RealSense Viewer app.
 '''
+import datetime
+import logging
 import os
 import time
 from pathlib import Path
-from typing import List
+from typing import List, Any, Dict, Union
 
 import depthai as dai
 import numpy as np
-from rosbags.rosbag1 import Writer
+from rosbags.rosbag1 import Writer as WriterRos1
+from rosbags.rosbag2 import Writer as WriterRos2
 from rosbags.serde import cdr_to_ros1, serialize_cdr
+
 from rosbags.typesys import get_types_from_msg, register_types
 from rosbags.typesys.types import builtin_interfaces__msg__Time as Time
-from rosbags.typesys.types import diagnostic_msgs__msg__KeyValue as KeyValue
 from rosbags.typesys.types import geometry_msgs__msg__Quaternion as Quaternion
 from rosbags.typesys.types import geometry_msgs__msg__Transform as Transform
 from rosbags.typesys.types import geometry_msgs__msg__Vector3 as Vector3
-from rosbags.typesys.types import sensor_msgs__msg__Image as Image
 from rosbags.typesys.types import sensor_msgs__msg__RegionOfInterest as Roi
 from rosbags.typesys.types import std_msgs__msg__Header as Header
 from rosbags.typesys.types import std_msgs__msg__UInt32 as UInt32
 
+# Message types
+from rosbags.typesys.types import sensor_msgs__msg__Image as Image
+from rosbags.typesys.types import sensor_msgs__msg__CompressedImage as CompressedImage
+from rosbags.typesys.types import sensor_msgs__msg__PointCloud2 as PointCloud2
+from rosbags.typesys.types import sensor_msgs__msg__Imu as Imu
+
+from rosbags.typesys.types import diagnostic_msgs__msg__KeyValue as KeyValue
+
 from depthai_sdk.recorders.abstract_recorder import Recorder
 
+from depthai_sdk.integrations.ros.imu_interpolation import ImuInterpolation, ImuSyncMethod
+
 CAMERA_INFO = """
 # This message defines meta information for a camera. It should be in a
 # camera namespace on topic "camera_info" and accompanied by up to five
 # image topics named:
 #
 #   image_raw - raw data from the camera driver, possibly Bayer encoded
 #   image            - monochrome, distorted
@@ -198,256 +210,347 @@
 
 uint32 fps        # The nominal streaming rate, defined in Hz
 string encoding   # Stream's data format
 bool is_recommended # Is this stream recommended by RealSense SDK
 """
 
 
-class RosbagRecorder(Recorder):
+class RosStream:
+    datatype: dai.DatatypeEnum  # dai datatype of the stream
+    xout: 'XoutBase'  # From which Xout is the stream
+    topic: str  # Topic name, eg. color/compressed
+    ros_type: Any  # CompressedImage, Image, IMU, PointCloud2...
+    connection: Any # Writer connection
+
+class _RosbagBaseRecorder(Recorder):
     def __init__(self):
         super().__init__()
-        self.rgb_meta_conn = None
-        self.calib = None
-        self.rgb_conn = None
-        self.path = None
+
+        self.streams: Dict[str, RosStream] = {}  # key = xlink stream name
+
+        self.path: str = None
         self.start_nanos = None
-        self.writer = None
-        self.dir = None
-        self.CamInfo = None
-        self.depth_conn = None
-        self.depth_meta_conn = None
+
+        self.pointcloud = False
+
         self._frame_init: List[str] = []
         self._closed = False
 
-    def update(self, path: Path, device: dai.Device, _):
+        self.imu_interpolation = ImuInterpolation()
+    def _update(self, device: dai.Device, xouts: List['XoutFrames']):
         """
         Args:
             path: Path to the folder where rosbag will be saved
             device: depthai.Device object
+            xouts: XoutFrames
         """
-        if path.suffix != '.bag':
-            path = path / 'recording.bag'
-        if path.exists():
-            path.unlink()
-        self.path = path
 
-        rgb = False  # TODO: support rgb/mono recording as well
         self._frame_init = []
         self.start_nanos = 0
-        self.writer = Writer(self.path)
-        # Compression will cause error in RealSense
-        # self.writer.set_compression(Writer.CompressionFormat.LZ4)
-        self.writer.open()
+
+        for xout in xouts:
+            for stream in xout.xstreams():
+                rs = RosStream()
+                rs.datatype = stream.stream.possibleDatatypes[0].datatype
+                name = xout.name.lower()
+
+                if xout.is_depth() and not stream.name.endswith('depth'):
+                    # Mono right frame for WLS, skip
+                    continue
+
+                if xout.is_mjpeg():
+                    rs.topic = f'/{name}/compressed'
+                    rs.ros_type = CompressedImage
+                elif xout.is_depth() and self.pointcloud:
+                    rs.topic = '/pointcloud/raw'
+                    rs.ros_type = PointCloud2
+                elif xout.is_imu():
+                    rs.topic = '/imu'
+                    rs.ros_type = Imu
+                else: # Non-encoded frames; rgb, mono, depth
+                    rs.topic = f'/{name}/raw'
+                    rs.ros_type = Image
+
+                self.streams[stream.name] = rs
+
+
+        # self.depth_meta_conn = self.add_connection('/device_0/sensor_0/Depth_0/image/metadata', KeyValue.__msgtype__)
+
+        # self.write_uint32('/file_version', 2)
+        # self.write_keyvalues('/device_0/info', {
+        #     'Name': 'OAK camera',
+        #     'Location': '',
+        #     'Debug Op Code': 0,
+        #     'Advanced Mode': 'YES',
+        #     'Product Id': '0000',
+        # })
+
+        # self.write_keyvalues('/device_0/sensor_0/info', {'Name': 'Stereo'})
+        # self.write_keyvalues('/device_0/sensor_0/property', {
+        #     'Depth Units': '0.001000',
+        #     # 'Serial Number': device.getMxId(),
+        #     # 'Library Version': dai.__version__,
+        #     # 'Exposure': '8000.000000',
+        #     # 'Gain': '16.0',
+        #     # 'Enable Auto Exposure': '0.000000',
+        #     # 'Visual Preset': '2.000000',
+        #     # 'Laser Power': '240.000000',
+        #     # 'Emitter Enabled':'1.000000',
+        #     # 'Frames Queue Size': '16.000000',
+        #     # 'Asic Temperature': '35.000000',
+        #     # 'Error Polling Enabled': '1.000000',
+        #     # 'Projector Temperature': '31.000000',
+        # })
+        # self.write_transform('/device_0/sensor_0/Depth_0/tf/0')
 
         # sensor_msgs__msg__CameraInfo won't work, as parameters (eg. D, K, R) are in lowercase (d, k, r), so
         # RealSense Viewer doesn't recognize the msg
-        self.dir = os.path.dirname(os.path.realpath(__file__))
-        register_types(get_types_from_msg(CAMERA_INFO, 'sensor_msgs/msg/CamInfo'))
-        from rosbags.typesys.types import sensor_msgs__msg__CamInfo as CamInfo
-        self.CamInfo = CamInfo
-
-        self.depth_conn = self.writer.add_connection('/device_0/sensor_0/Depth_0/image/data', Image.__msgtype__,
-                                                     latching=1)
-        self.depth_meta_conn = self.writer.add_connection('/device_0/sensor_0/Depth_0/image/metadata',
-                                                          KeyValue.__msgtype__, latching=1)
-
-        self.write_uint32('/file_version', 2)
-        self.write_keyvalues('/device_0/info', {
-            'Name': 'OAK camera',
-            'Location': '',
-            'Debug Op Code': 0,
-            'Advanced Mode': 'YES',
-            'Product Id': '0000',
-        })
-        self.write_streamInfo(depth=True)
-
-        self.write_keyvalues('/device_0/sensor_0/info', {'Name': 'Stereo'})
-        self.write_keyvalues('/device_0/sensor_0/property', {
-            'Depth Units': '0.001000',
-            # 'Serial Number': device.getMxId(),
-            # 'Library Version': dai.__version__,
-            # 'Exposure': '8000.000000',
-            # 'Gain': '16.0',
-            # 'Enable Auto Exposure': '0.000000',
-            # 'Visual Preset': '2.000000',
-            # 'Laser Power': '240.000000',
-            # 'Emitter Enabled':'1.000000',
-            # 'Frames Queue Size': '16.000000',
-            # 'Asic Temperature': '35.000000',
-            # 'Error Polling Enabled': '1.000000',
-            # 'Projector Temperature': '31.000000',
-        })
-        self.write_transform('/device_0/sensor_0/Depth_0/tf/0')
-
-        self.calib = device.readCalibration()
-
-        if rgb:
-            # Color recording isn't yet possible.
-            self.write_keyvalues('/device_0/sensor_1/info', {'Name': 'RGB Camera'})
-            self.write_keyvalues('/device_0/sensor_1/property', {
-                'Backlight Compensation': '0.000000',
-                # 'Brightness': '0.000000',
-                # 'Contrast': '50.000000',
-                # 'Exposure': '6.000000',
-                # 'Gain': '64.000000',
-                # 'Gamma': '300.000000',
-                # 'Hue': '0.000000',
-                # 'Saturation': '64.000000',
-                # 'Sharpness': '50.000000',
-                # 'White Balance': '4600.000000',
-                # 'Enable Auto Exposure': '1.000000',
-                # 'Enable Auto White Balance': '1.000000',
-                # 'Frames Queue Size': '16.000000',
-                # 'Power Line Frequency': '3.000000',
-            })
-            self.write_transform('/device_0/sensor_1/Color_0/tf/0')
-
-            self.rgb_conn = self.writer.add_connection('/device_0/sensor_1/Color_0/image/data', Image.__msgtype__,
-                                                       latching=1)
-            self.rgb_meta_conn = self.writer.add_connection('/device_0/sensor_1/Color_0/image/metadata',
-                                                            KeyValue.__msgtype__, latching=1)
-
-    def _init_stream(self, frame: dai.ImgFrame):
-        resolution = (frame.getWidth(), frame.getHeight())
-
-        if frame.getType() == dai.ImgFrame.Type.RAW16:  # Depth
-            self.write_depthInfo('/device_0/sensor_0/Depth_0/info/camera_info', resolution, self.calib)
-        else:
-            raise NotImplementedError('RosBags currently only support recording of depth!')
+        # register_types(get_types_from_msg(CAMERA_INFO, 'sensor_msgs/msg/CamInfo'))
+        # from rosbags.typesys.types import sensor_msgs__msg__CamInfo as CamInfo
+
+        # self.write_streamInfo(depth=True)
+        # if rgb:
+        #     # Color recording isn't yet possible.
+        #     self.write_keyvalues('/device_0/sensor_1/info', {'Name': 'RGB Camera'})
+        #     self.write_keyvalues('/device_0/sensor_1/property', {
+        #         'Backlight Compensation': '0.000000',
+        #     })
+        #     self.write_transform('/device_0/sensor_1/Color_0/tf/0')
+        #
+        #     self.rgb_meta_conn = self.add_connection('/device_0/sensor_1/Color_0/image/metadata', KeyValue.__msgtype__)
+
+    # def _init_stream(self, frame: dai.ImgFrame):
+    #     resolution = (frame.getWidth(), frame.getHeight())
+    #
+    #     if frame.getType() == dai.ImgFrame.Type.RAW16:  # Depth
+    #         self.write_depthInfo('/device_0/sensor_0/Depth_0/info/camera_info', resolution, self.calib)
+    #     else:
+    #         raise NotImplementedError('RosBags currently only support recording of depth!')
         #
         # elif frame.getType() == dai.ImgFrame.Type.RAW8: # Mono Cams
         #     pass
         # else: # Color
         #     fourcc = "I420"
         #     self.write_colorInfo('/device_0/sensor_1/Color_0/info/camera_info', resolution, self.calib)
 
-    def write(self, name: str, img_frame: dai.ImgFrame):
-        if name not in self._frame_init:
-            self._init_stream(img_frame)
-            self._frame_init.append(name)
+    def write(self, name: str, dai_msg: dai.Buffer):
+        # if name not in self._frame_init:
+        #     self._init_stream(img_frame)
+        #     self._frame_init.append(name)
+        #
+        # frame: np.ndarray = img_frame.getCvFrame()
+
+        if name not in self.streams:  # Not relevant
+            return
 
-        frame = img_frame.getCvFrame()
-        # First frames
+        # depthai msgs, name = xlink name
+        stream = self.streams[name]
         if self.start_nanos == 0: self.start_nanos = time.time_ns()
 
-        rgb = len(frame.shape) == 3
-        if rgb:
-            frame = frame[:, :, [2, 1, 0]]
-        img = Image(header=self.get_current_header(),
-                    height=frame.shape[0],
-                    width=frame.shape[1],
-                    encoding='rgb8' if rgb else 'mono16',
-                    is_bigendian=0,
-                    step=frame.shape[1] * 2,
-                    data=frame.flatten().view(dtype=np.int8))
-        msg_type = Image.__msgtype__
-
-        self._write(self.rgb_conn if rgb else self.depth_conn, msg_type, img)
-
-        self.write_keyvalues(self.rgb_meta_conn if rgb else self.depth_meta_conn, {
-            'system_time': "%.6f" % time.time(),
-            'timestamp_domain': 'System Time',
-            'Time Of Arrival': int(time.time())
-        }, connection=True)
+        msg = None
+        if stream.ros_type == CompressedImage:
+            # msg = self.bridge.CompressedImage(dai_msg)
+            msg = CompressedImage(header=self.get_header(dai_msg.getTimestampDevice(), dai_msg.getSequenceNum()),
+                        format = "jpeg",
+                        data=np.array(dai_msg.getData())
+                                  )
+            self.write_to_rosbag(name, stream.ros_type.__msgtype__, msg)
+        elif stream.ros_type == PointCloud2:
+            raise Exception('PointCloud2 not yet implemented')
+        elif stream.ros_type == Imu:
+            dai_msg: dai.IMUData
+            for packet in dai_msg.packets:
+                report = packet.acceleroMeter or packet.gyroscope or packet.magneticField or packet.rotationVector
+                msg = Imu(
+                    header=self.get_header(report.getTimestampDevice(), report.sequence),
+                    orientation=Quaternion(x=0.0, y=0.0, z=0.0, w=1.0),
+                    orientation_covariance=np.array([-1.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0]),
+                    angular_velocity=Vector3(0.0, 0.0, 0.0),
+                    angular_velocity_covariance=np.array([]),
+                    linear_acceleration=Vector3(0.0, 0.0, 0.0),
+                    linear_acceleration_covariance=np.array([])
+                )
+                self.imu_interpolation.Imu(msg, packet)
+                self.write_to_rosbag(name, stream.ros_type.__msgtype__, msg)
+        elif stream.ros_type == Image:
+            # msg = self.bridge.Image(dai_msg)
+            dai_msg: dai.ImgFrame
+            step = dai_msg.getWidth()
+
+            type = dai_msg.getType()
+            TYPE = dai.ImgFrame.Type
+            if type == TYPE.RAW16:  # Depth
+                encoding = 'mono16'
+                step *= 2  # 2 bytes per pixelE
+            elif type in [TYPE.GRAY8, TYPE.RAW8]:  # Mono frame
+                encoding = 'mono8'
+            else:
+                encoding = 'bgr8'
+
+            msg = Image(header=self.get_header(dai_msg.getTimestampDevice(), dai_msg.getSequenceNum()),
+                        height=dai_msg.getHeight(),
+                        width=dai_msg.getWidth(),
+                        encoding=encoding,
+                        is_bigendian=0,
+                        step=step,
+                        data=np.array(dai_msg.getCvFrame()).flatten().view(dtype=np.int8)
+                        )
+            self.write_to_rosbag(name, stream.ros_type.__msgtype__, msg)
+
+        # First frames
+
+
+
+        # rgb = len(frame.shape) == 3
+        # if rgb:
+        #     frame = frame[:, :, [2, 1, 0]]
+
+
+
+        # self.write_keyvalues(self.rgb_meta_conn if rgb else self.depth_meta_conn, {
+        #     'system_time': "%.6f" % time.time(),
+        #     'timestamp_domain': 'System Time',
+        #     'Time Of Arrival': int(time.time())
+        # }, connection=True)
 
     def close(self):
         if self._closed: return
         self._closed = True
-        print("ROS .bag saved at: ", str(self.path))
+        logging.info("ROS .bag saved at: ", str(self.path))
         self.writer.close()
 
-    def _write(self, connection, type, data):
-        self.writer.write(connection, time.time_ns() - self.start_nanos, cdr_to_ros1(serialize_cdr(data, type), type))
-
-    def write_streamInfo(self, depth=False, rgb=False):
-        # Inspired by https://github.com/IntelRealSense/librealsense/blob/master/third-party/realsense-file/rosbag/msgs/realsense_msgs/StreamInfo.h
-        register_types(get_types_from_msg(STREAM_INFO, 'realsense_msgs/msg/StreamInfo'))
-        from rosbags.typesys.types import realsense_msgs__msg__StreamInfo as StreamInfo
-
-        if depth:
-            streamInfo = StreamInfo(fps=30, encoding="mono16", is_recommended=False)
-            c = self.writer.add_connection('/device_0/sensor_0/Depth_0/info', streamInfo.__msgtype__)
-            self._write(c, streamInfo.__msgtype__, streamInfo)
-        if rgb:
-            streamInfo = StreamInfo(fps=30, encoding="rgb8", is_recommended=False)
-            c = self.writer.add_connection('/device_0/sensor_1/Color_0/info', streamInfo.__msgtype__)
-            self._write(c, streamInfo.__msgtype__, streamInfo)
-
-    def write_keyvalues(self, topic_or_connection, array, connection=False):
-        type = KeyValue.__msgtype__
-        if not connection:
-            c = self.writer.add_connection(topic_or_connection, type, latching=1)
-        for name in array:
-            self._write(topic_or_connection if connection else c, type, KeyValue(key=name, value=str(array[name])))
-
-    def write_uint32(self, topic, uint32):
-        msg_type = UInt32.__msgtype__
-        c = self.writer.add_connection(topic, msg_type, latching=1)
-        self._write(c, msg_type, UInt32(data=uint32))
+    # def write_streamInfo(self, depth=False, rgb=False):
+    #     # Inspired by https://github.com/IntelRealSense/librealsense/blob/master/third-party/realsense-file/rosbag/msgs/realsense_msgs/StreamInfo.h
+    #     register_types(get_types_from_msg(STREAM_INFO, 'realsense_msgs/msg/StreamInfo'))
+    #     from rosbags.typesys.types import realsense_msgs__msg__StreamInfo as StreamInfo
+    #
+    #     if depth:
+    #         streamInfo = StreamInfo(fps=30, encoding="mono16", is_recommended=False)
+    #         c = self.add_connection('/device_0/sensor_0/Depth_0/info', streamInfo.__msgtype__)
+    #         self._write(c, streamInfo.__msgtype__, streamInfo)
+    #     if rgb:
+    #         streamInfo = StreamInfo(fps=30, encoding="rgb8", is_recommended=False)
+    #         c = self.add_connection('/device_0/sensor_1/Color_0/info', streamInfo.__msgtype__)
+    #         self._write(c, streamInfo.__msgtype__, streamInfo)
+
+    # def write_keyvalues(self, topic_or_connection, array, connection=False):
+    #     type = KeyValue.__msgtype__
+    #     if not connection:
+    #         c = self.add_connection(topic_or_connection, type)
+    #     for name in array:
+    #         self.write_to_rosbag(topic_or_connection if connection else c, type, KeyValue(key=name, value=str(array[name])))
+    #
+    # def write_uint32(self, topic, uint32):
+    #     msg_type = UInt32.__msgtype__
+    #     c = self.add_connection(topic, msg_type)
+    #     self.write_to_rosbag(c, msg_type, UInt32(data=uint32))
 
     # translation: [x,y,z]
     # rotation: [x,y,z,w]
     # We will use depth alignment to color camera in case we record depth
-    def write_transform(self, topic, translation=None, rotation=None):
-        translation = translation or [0, 0, 0]
-        rotation = rotation or [0, 0, 0, 0]
-
-        msg_type = Transform.__msgtype__
-        translation = Vector3(x=translation[0], y=translation[1], z=translation[2])
-        rotation = Quaternion(x=rotation[0], y=rotation[1], z=rotation[2], w=rotation[3])
-        c = self.writer.add_connection(topic, msg_type, latching=1)
-        self._write(c, msg_type, Transform(translation=translation, rotation=rotation))
-
-    def write_depthInfo(self, topic, resolution, calib_data):
-        # Distortion parameters (k1,k2,t1,t2,k3)
-        dist = np.array(calib_data.getDistortionCoefficients(dai.CameraBoardSocket.RIGHT))
-
-        # Intrinsic camera matrix
-        M_right = np.array(calib_data.getCameraIntrinsics(dai.CameraBoardSocket.RIGHT, resolution[0], resolution[1]))
-
-        R1 = np.array(calib_data.getStereoLeftRectificationRotation())
-
-        # Rectification matrix (stereo cameras only)
-        H_right = np.matmul(np.matmul(M_right, R1), np.linalg.inv(M_right))
-
-        # Projection/camera matrix
-        lr_extrinsics = np.array(calib_data.getCameraExtrinsics(dai.CameraBoardSocket.LEFT, dai.CameraBoardSocket.RIGHT))
-
-        self.write_cameraInfo(topic, resolution, M_right, H_right, lr_extrinsics)
-
-    def write_colorInfo(self, topic, resolution, calib_data):
-        # Distortion parameters (k1,k2,t1,t2,k3)
-        dist = np.array(calib_data.getDistortionCoefficients(dai.CameraBoardSocket.RGB))
-
-        # Intrinsic camera matrix
-        M_color = np.array(calib_data.getCameraIntrinsics(dai.CameraBoardSocket.RGB, resolution[0], resolution[1]))
-        self.write_cameraInfo(topic, resolution, M_color, np.zeros((3, 3)), np.zeros((4, 4)))
-
-    def write_cameraInfo(self, topic, resolution, intrinsics, rect, project):
-        # print(topic, resolution)
-        msg_type = self.CamInfo.__msgtype__
-        c = self.writer.add_connection(topic, msg_type, latching=1)
-        info = self.CamInfo(header=self.get__default_header(),
-                            height=resolution[1],
-                            width=resolution[0],
-                            distortion_model='Brown Conrady',
-                            # D=dist[:5], # Doesn't work
-                            D=np.zeros(5),  # Distortion parameters (k1,k2,t1,t2,k3)
-                            K=intrinsics.flatten(),  # Intrinsic camera matrix
-                            R=rect.flatten(),  # Rectification matrix (stereo cameras only)
-                            P=project[:3, :].flatten(),  # Projection/camera matrix
-                            binning_x=0,
-                            binning_y=0,
-                            roi=self.get_default_roi())
-        self._write(c, msg_type, info)
+    # def write_transform(self, topic, translation=None, rotation=None):
+    #     translation = translation or [0, 0, 0]
+    #     rotation = rotation or [0, 0, 0, 0]
+    # 
+    #     msg_type = Transform.__msgtype__
+    #     translation = Vector3(x=translation[0], y=translation[1], z=translation[2])
+    #     rotation = Quaternion(x=rotation[0], y=rotation[1], z=rotation[2], w=rotation[3])
+    #     c = self.add_connection(topic, msg_type)
+    #     self.write_to_rosbag(c, msg_type, Transform(translation=translation, rotation=rotation))
+    # 
+    # def write_depthInfo(self, topic, resolution, calib_data):
+    #     # Distortion parameters (k1,k2,t1,t2,k3)
+    #     dist = np.array(calib_data.getDistortionCoefficients(dai.CameraBoardSocket.RIGHT))
+    # 
+    #     # Intrinsic camera matrix
+    #     M_right = np.array(calib_data.getCameraIntrinsics(dai.CameraBoardSocket.RIGHT, resolution[0], resolution[1]))
+    # 
+    #     R1 = np.array(calib_data.getStereoLeftRectificationRotation())
+    # 
+    #     # Rectification matrix (stereo cameras only)
+    #     H_right = np.matmul(np.matmul(M_right, R1), np.linalg.inv(M_right))
+    # 
+    #     # Projection/camera matrix
+    #     lr_extrinsics = np.array(calib_data.getCameraExtrinsics(dai.CameraBoardSocket.LEFT, dai.CameraBoardSocket.RIGHT))
+    # 
+    #     self.write_cameraInfo(topic, resolution, M_right, H_right, lr_extrinsics)
+    # 
+    # def write_colorInfo(self, topic, resolution, calib_data):
+    #     # Distortion parameters (k1,k2,t1,t2,k3)
+    #     dist = np.array(calib_data.getDistortionCoefficients(dai.CameraBoardSocket.RGB))
+    # 
+    #     # Intrinsic camera matrix
+    #     M_color = np.array(calib_data.getCameraIntrinsics(dai.CameraBoardSocket.RGB, resolution[0], resolution[1]))
+    #     self.write_cameraInfo(topic, resolution, M_color, np.zeros((3, 3)), np.zeros((4, 4)))
+    # 
+    # def write_cameraInfo(self, topic, resolution, intrinsics, rect, project):
+    #     # print(topic, resolution)
+    #     msg_type = self.CamInfo.__msgtype__
+    #     c = self.add_connection(topic, msg_type)
+    #     info = self.CamInfo(header=self.get__default_header(),
+    #                         height=resolution[1],
+    #                         width=resolution[0],
+    #                         distortion_model='Brown Conrady',
+    #                         # D=dist[:5], # Doesn't work
+    #                         D=np.zeros(5),  # Distortion parameters (k1,k2,t1,t2,k3)
+    #                         K=intrinsics.flatten(),  # Intrinsic camera matrix
+    #                         R=rect.flatten(),  # Rectification matrix (stereo cameras only)
+    #                         P=project[:3, :].flatten(),  # Projection/camera matrix
+    #                         binning_x=0,
+    #                         binning_y=0,
+    #                         roi=self.get_default_roi())
+    #     self.write_to_rosbag(c, msg_type, info)
 
     def get__default_header(self):
         t = Time(sec=0, nanosec=0)
         return Header(stamp=t, frame_id='0')
 
-    def get_current_header(self):
-        t_str_arr = ("%.9f" % time.time()).split('.')
-        t = Time(sec=int(t_str_arr[0]), nanosec=int(t_str_arr[1]))
-        return Header(stamp=t, frame_id='0')
+    def get_header(self, td: datetime.timedelta, sequence: int):
+        time = Time(sec=td.seconds, nanosec=td.microseconds * 1000)
+        return Header(stamp=time, frame_id=str(sequence))
 
     def get_default_roi(self):
         return Roi(x_offset=0, y_offset=0, height=0, width=0, do_rectify=False)
+
+
+class Rosbag1Recorder(_RosbagBaseRecorder):
+    writer: WriterRos1
+
+    def update(self, path: Path, device: dai.Device, xouts: List['XoutFrames']):
+        if path.suffix != '.bag':
+            path = path / 'recording.bag'
+        if path.exists():
+            path.unlink()
+        self.path = path
+        self.writer = None
+
+        _RosbagBaseRecorder._update(self, device, xouts)
+    def write_to_rosbag(self, name: str, type, data):
+        if self.writer is None:
+            self.writer = WriterRos1(self.path)
+            # self.writer.set_compression(Writer.CompressionFormat.LZ4)
+            self.writer.open()
+            for _, stream in self.streams.items():
+                stream.connection = self.writer.add_connection(stream.topic, stream.ros_type.__msgtype__, latching=True)
+
+        self.writer.write(self.streams[name].connection, time.time_ns() - self.start_nanos, cdr_to_ros1(serialize_cdr(data, type), type))
+
+
+class Rosbag2Recorder(_RosbagBaseRecorder):
+    writer: WriterRos2
+    def update(self, path: Path, device: dai.Device, xouts: List['XoutFrames']):
+        self.path = path / 'recording'
+        self.writer = None
+        _RosbagBaseRecorder._update(self, device, xouts)
+
+
+    def write_to_rosbag(self, name: str, type, data):
+        if self.writer is None:
+            self.writer = WriterRos2(self.path)
+            self.writer.open()
+            for _, stream in self.streams.items():
+                stream.connection = self.writer.add_connection(stream.topic, stream.ros_type.__msgtype__, 'cdr', '')
+
+        self.writer.write(self.streams[name].connection, time.time_ns() - self.start_nanos, serialize_cdr(data, type))
+
+
+
```

### Comparing `depthai-sdk-1.9.4.1/src/depthai_sdk/recorders/video_recorder.py` & `depthai-sdk-1.9.5/src/depthai_sdk/recorders/video_recorder.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import logging
 from typing import Union
 
 import numpy as np
 
 from .abstract_recorder import *
 
 
@@ -45,25 +46,25 @@
                 self._writers[name] = VideoWriter(self.path, name, fourcc, xout.fps)
             else:
                 try:
                     from .video_writers.av_writer import AvWriter
                     self._writers[name] = AvWriter(self.path, name, fourcc, xout.fps)
                 except Exception as e:
                     # TODO here can be other errors, not only import error
-                    print('Exception while creating AvWriter: ', e)
-                    print('Falling back to FileWriter, saving uncontainerized encoded streams.')
+                    logging.warning(f'Exception while creating AvWriter: {e}.'
+                                    '\nFalling back to FileWriter, saving uncontainerized encoded streams.')
                     from .video_writers.file_writer import FileWriter
                     self._writers[name] = FileWriter(self.path, name, fourcc)
 
     def write(self, name: str, frame: Union[np.ndarray, dai.ImgFrame]):
         self._writers[name].write(frame)
 
     def add_to_buffer(self, name: str, frame: Union[np.ndarray, dai.ImgFrame]):
         self._writers[name].add_to_buffer(frame)
 
     def close(self):
         if self._closed: return
         self._closed = True
-        print("Video Recorder saved stream(s) to folder:", str(self.path))
+        logging.info("Video Recorder saved stream(s) to folder:", str(self.path))
         # Close opened files
         for name, writer in self._writers.items():
             writer.close()
```

### Comparing `depthai-sdk-1.9.4.1/src/depthai_sdk/recorders/video_writers/av_writer.py` & `depthai-sdk-1.9.5/src/depthai_sdk/recorders/video_writers/av_writer.py`

 * *Files identical despite different names*

### Comparing `depthai-sdk-1.9.4.1/src/depthai_sdk/recorders/video_writers/file_writer.py` & `depthai-sdk-1.9.5/src/depthai_sdk/recorders/video_writers/file_writer.py`

 * *Files identical despite different names*

### Comparing `depthai-sdk-1.9.4.1/src/depthai_sdk/recorders/video_writers/video_writer.py` & `depthai-sdk-1.9.5/src/depthai_sdk/recorders/video_writers/video_writer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import logging
 from collections import deque
 from datetime import datetime
 from pathlib import Path
 from typing import Union
 
 try:
     import cv2
@@ -97,15 +98,15 @@
                 buffer_copy.popleft()
                 continue
 
             el = buffer_copy.popleft()
             snapshot_file.write(el if isinstance(el, np.ndarray) else el.getCvFrame())
 
         snapshot_file.release()
-        print('Snapshot saved to', save_path)
+        logging.info('Snapshot saved to', save_path)
 
     def set_fourcc(self, fourcc: str):
         self._fourcc = fourcc
 
     def add_to_buffer(self, frame: Union[dai.ImgFrame, np.ndarray]):
         if not self._is_buffer_enabled:
             return
```

### Comparing `depthai-sdk-1.9.4.1/src/depthai_sdk/replay.py` & `depthai-sdk-1.9.5/src/depthai_sdk/replay.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,40 +1,73 @@
+import logging
 import os
 import time
 from threading import Thread
 from time import monotonic
 
 import depthai as dai
 
+from depthai_sdk.classes.enum import ResizeMode
 from depthai_sdk.readers.abstract_reader import AbstractReader
 from depthai_sdk.utils import *
 
 _fileTypes = ['color', 'left', 'right', 'disparity', 'depth']
 _videoExt = ['.mjpeg', '.avi', '.mp4', '.h265', '.h264', '.webm']
 _imageExt = ['.bmp', '.dib', '.jpeg', '.jpg', '.jpe', '.jp2', '.png', '.webp', '.pbm', '.pgm', '.ppm', '.pxm',
              '.pnm', '.pfm', '.sr', '.ras', '.tiff', '.tif', '.exr', '.hdr', '.pic']
 
 
+class ReplayStream:
+    stream_name: str  # XLink stream name
+    queue: dai.DataInputQueue  # Input queue
+    frame: np.ndarray  # Last read frame from Reader (ndarray)
+    imgFrame: dai.ImgFrame  # Last read ImgFrame from Reader (dai.ImgFrame)
+    _shape: Tuple[int, int]  # width, height
+    disabled: bool
+    size_bytes: int  # bytes
+
+    @property
+    def shape(self) -> Tuple[int, int]:
+        return self.resize if self.resize else self._shape
+
+    def __init__(self):
+        self.node: dai.node.XLinkIn = None
+        self.disabled = False
+        self.stream_name = ''
+        self.camera_socket: dai.CameraBoardSocket = None
+
+        self.resize: Tuple[int, int] = None
+        self.resize_mode: ResizeMode = None
+
+    def get_socket(self) -> dai.CameraBoardSocket:
+        if self.camera_socket:
+            return self.camera_socket
+        if 'left' in self.stream_name:
+            return dai.CameraBoardSocket.LEFT
+        elif 'right' in self.stream_name:
+            return dai.CameraBoardSocket.RIGHT
+        else:
+            return dai.CameraBoardSocket.RGB
+        # raise Exception("Please specify replay stream CameraBoardSocket via replay.specify_socket()")
+
+
 class Replay:
     def __init__(self, path: str):
         """
         Helper file to replay recorded depthai stream. It reads from recorded files (mjpeg/avi/mp4/h265/h264/bag)
         and sends frames back to OAK camera to replay the scene, including depth reconstruction from 2 synced mono
         streams.
     
         Args:
             path (str): Path to the recording folder
         """
         self.path = self._get_path(path)
 
         self.disabledStreams: List[str] = []
-        # Nodes
-        self.left: Optional[dai.node.XLinkIn] = None
-        self.right: Optional[dai.node.XLinkIn] = None
-        self.color: Optional[dai.node.XLinkIn] = None
+        self.streams: Dict[str, ReplayStream] = {}
 
         self._inputQueues = dict()  # dai.InputQueue dictionary for each stream
         self._seqNum = 0  # Frame sequence number, added to each imgFrame
         self._now: monotonic = None
         self._colorSize = None
         self._keepAR = True  # By default, crop image as needed to keep the aspect ratio
         self._pause = False
@@ -91,14 +124,21 @@
                 self.reader = VideoCapReader(self.path)
             elif self.path.suffix in _imageExt:
                 from .readers.image_reader import ImageReader
                 self.reader = ImageReader(self.path)
             else:
                 raise NotImplementedError('Please select folder')
 
+        # Read all available streams
+        for stream_name in self.reader.getStreams():
+            stream = ReplayStream()
+            stream._shape = self.reader.getShape(stream_name)
+            stream.size_bytes = self.reader.get_message_size(stream_name)
+            self.streams[stream_name] = stream
+
     def _get_path(self, path: str) -> Path:
         """
         Either use local depthai-recording, YT link, mp4 url
         @param path: depthai-recording path.
         @return: Replay module
         """
         if isUrl(path):
@@ -117,257 +157,258 @@
         if path is not None:
             return path
 
         # Try to download from the server
         dic = getAvailableRecordings()
         if recording_name in dic:
             arr = dic[recording_name]
-            print("Downloading depthai recording '{}' from Luxonis' servers, in total {:.2f} MB".format(recording_name,
-                                                                                                        arr[1] / 1e6))
+            logging.info("Downloading depthai recording '{}' from Luxonis' servers, in total {:.2f} MB"
+                         .format(recording_name, arr[1] / 1e6))
             path = downloadRecording(recording_name, arr[0])
             return path
         else:
             raise ValueError(f"DepthAI recording '{recording_name}' was not found on the server!")
 
-    def togglePause(self):
+    def toggle_pause(self):
         """
         Toggle pausing of sending frames to the OAK camera.
         """
         self._pause = not self._pause
-        print("PAUSE", self._pause)
 
-    def setFps(self, fps: float):
+    def set_fps(self, fps: float):
         """
         Sets frequency at which Replay module will send frames to the camera. Default 30FPS.
         """
-        self.fps = fps
+        if type(self.reader).__name__ == 'ImageReader':
+            self.reader.set_cycle_fps(fps)
+        else:
+            self.fps = fps
 
-    def getFps(self) -> float:
+    def get_fps(self) -> float:
         return self.fps
 
-    def setResizeColor(self, size: tuple):
+    def resize(self, stream_name: str, size: Tuple[int, int], mode: ResizeMode = ResizeMode.STRETCH):
         """
         Resize color frames prior to sending them to the device.
 
         Args:
-            size (tuple(width, heigth)): Size of color frames that are sent to the camera
+            stream_name (str): Name of the stream we want to resize
+            size (Tuple(width, heigth)): Size of color frames that are sent to the camera
+            mode (ResizeMode): How to actually resize the stream
         """
-        self._colorSize = size
+        self.streams[stream_name].resize = size
+        self.streams[stream_name].resize_mode = mode
 
     def keepAspectRatio(self, keepAspectRatio: bool):
-        """
-        Used when we want to resize color frames before sending them to the host. By default,
-        this is set to True, so frames are cropped to keep the original aspect ratio.
-        """
-        self._keepAR = keepAspectRatio
+        raise Exception('keepAspectRatio() has been deprecated, use resize(mode=ResizeMode) to set whether to keep AR!')
 
-    def disableStream(self, streamName: str, disableReading: bool = False):
+    def disableStream(self, stream_name: str, disableReading: bool = False):
         """
         Disable sending a recorded stream to the device.
 
         Args:
             streamName(str): Name of the stream to disable (eg. 'left', 'color', 'depth', etc.)
             disableReading (bool, Optional): Also disable reading frames from the file
         """
-        # if streamName not in self.readers:
-        #     print(f"There's no stream '{streamName}' available!")
-        #     return
         if disableReading:
-            self.reader.disableStream(streamName)
-
-        self.disabledStreams.append(streamName)
-
-    def sendFrames(self, cb=None) -> bool:
-        """
-        Reads and sends recorded frames from all enabled streams to the OAK camera.
-
-        Returns:
-            bool: True if successful, otherwise False.
-        """
-        if not self._pause:  # If replaying is paused, don't read new frames
-            if not self._readFrames():
-                return False  # End of the recording
-
-        self._now = monotonic()
-        for name in self.frames:
-            imgFrame = self._createImgFrame(name, self.frames[name])
-            # Save the imgFrame
-            self.imgFrames[name] = imgFrame
-            if cb:  # callback
-                cb(name, imgFrame)
-
-            # Don't send these frames to the OAK camera
-            if name in self.disabledStreams: continue
-
-            # Send an imgFrame to the OAK camera
-            self._inputQueues[name].send(imgFrame)
+            self.reader.disableStream(stream_name)
 
-        self._seqNum += 1
-        return True
+        if stream_name not in self.streams:
+            logging.info(f"There's no stream '{stream_name}' available!")
+            return
+
+        self.streams[stream_name].disabled = True
+
+    def specify_socket(self, stream_name: str, socket: dai.CameraBoardSocket):
+        if stream_name not in self.streams:
+            logging.info(f"There's no stream '{stream_name}' available!")
+            return
+        self.streams[stream_name].camera_socket = socket
 
     def initPipeline(self, pipeline: dai.Pipeline = None):
         """
         Prepares the pipeline for replaying. It creates XLinkIn nodes and sets up StereoDepth node.
         Returns: dai.Pipeline
         """
         if pipeline is None:  # Create pipeline if not passed
             pipeline = dai.Pipeline()
 
         if self._calibData is not None:
             pipeline.setCalibrationData(self._calibData)
 
-        def createXIn(p: dai.Pipeline, name: str):
+        def createXIn(p: dai.Pipeline, xlink_stream_name: str, size: int):
             xin = p.create(dai.node.XLinkIn)
-            xin.setMaxDataSize(self._getMaxSize(name))
-            xin.setStreamName(name + '_in')
-            self.xins.append(name)
+            xin.setMaxDataSize(size)
+            xin.setStreamName(xlink_stream_name)
             return xin
 
-        for name in self.reader.getStreams():
-            if name not in self.disabledStreams:
-                xin = createXIn(pipeline, name)
-                if name.upper() == 'LEFT':
-                    self.left = xin
-                elif name.upper() == 'RIGHT':
-                    self.right = xin
-                elif name.upper() == 'COLOR':
-                    self.color = xin
-                else:
-                    pass  # Not implemented
+        for name, stream in self.streams.items():
+            if stream.disabled: continue
+
+            stream.stream_name = name + '_in'
+            stream.node = createXIn(pipeline, stream.stream_name, stream.size_bytes)
 
         return pipeline
 
-    def initStereoDepth(self, stereo: dai.node.StereoDepth):
-        streams = self.reader.getStreams()
-        if 'left' not in streams or 'right' not in streams:
+    def initStereoDepth(self,
+                        stereo: dai.node.StereoDepth,
+                        left_name: str = 'left',
+                        right_name: str = 'right',
+                        align_to: str = ''):
+        if left_name not in self.streams or right_name not in self.streams:
             raise Exception("Tried to init StereoDepth, but left/right streams aren't available!")
-        stereo.setInputResolution(self.getShape('left'))
 
-        if self.color:  # Enable RGB-depth alignment
+        left = self.streams[left_name]
+        right = self.streams[right_name]
+
+        stereo.setInputResolution(left.shape)
+
+        if not left.camera_socket:
+            left.camera_socket = dai.CameraBoardSocket.LEFT
+        if not right.camera_socket:
+            right.camera_socket = dai.CameraBoardSocket.RIGHT
+
+        if align_to:  # Enable RGB-depth alignment
             stereo.setDepthAlign(dai.CameraBoardSocket.RGB)
-            if self._colorSize is not None:
-                stereo.setOutputSize(*self._colorSize)
-            else:
-                stereo.setOutputSize(*self.getShape('color'))
+            stereo.setOutputSize(*self.streams[align_to].shape)
 
-        self.left.out.link(stereo.left)
-        self.right.out.link(stereo.right)
+        left.node.out.link(stereo.left)
+        right.node.out.link(stereo.right)
 
     def start(self, cb):
         """
         Start sending frames to the OAK device on a new thread
         """
         self.thread = Thread(target=self.run, args=(cb,))
         self.thread.start()
 
     def run(self, cb):
         delay = 1.0 / self.fps
         while True:
             if not self.sendFrames(cb): break
             time.sleep(delay)
             if self._stop: break
-        print('Replay `run` thread stopped')
+        logging.info('Replay `run` thread stopped')
         self._stop = True
 
+    def sendFrames(self, cb=None) -> bool:
+        """
+        Reads and sends recorded frames from all enabled streams to the OAK camera.
+
+        Returns:
+            bool: True if successful, otherwise False.
+        """
+        if not self._pause:  # If replaying is paused, don't read new frames
+            if not self._readFrames():
+                return False  # End of the recording
+
+        self._now = monotonic()
+        for stream_name, stream in self.streams.items():
+            stream.imgFrame = self._createImgFrame(stream)
+            # Save the imgFrame
+            if cb:  # callback
+                cb(stream_name, stream.imgFrame)
+
+            # Don't send these frames to the OAK camera
+            if stream.disabled: continue
+
+            # Send an imgFrame to the OAK camera
+            stream.queue.send(stream.imgFrame)
+
+        self._seqNum += 1
+        return True
+
     def createQueues(self, device: dai.Device):
         """
         Creates input queue for each enabled stream
         
         Args:
             device (dai.Device): Device to which we will stream frames
         """
-        for name in self.xins:
-            self._inputQueues[name] = device.getInputQueue(name + '_in')
+
+        for name, stream in self.streams.items():
+            if stream.stream_name:
+                stream.queue = device.getInputQueue(stream.stream_name)
 
     def getStreams(self) -> List[str]:
-        streams: List[str] = []
-        [streams.append(name) for name in self.reader.getStreams()]
-        return streams
-
-    def _resizeColor(self, frame):
-        if self._colorSize is None:
-            # No resizing needed
-            return frame
+        return [name for name, stream in self.streams.items()]
 
-        if not self._keepAR:
+    def _resize_frame(self, frame: np.ndarray, size: Tuple[int, int], mode: ResizeMode) -> np.ndarray:
+        if mode == ResizeMode.STRETCH:
             # No need to keep aspect ratio, image will be squished
-            return cv2.resize(frame, self._colorSize)
-
-        cropped = cropToAspectRatio(frame, self._colorSize)
-        return cv2.resize(cropped, self._colorSize)
+            return cv2.resize(frame, size)
+        elif mode == ResizeMode.CROP:
+            cropped = cropToAspectRatio(frame, size)
+            return cv2.resize(cropped, size)
+        elif mode == ResizeMode.FULL_CROP:
+            w = frame.shape[1]
+            start_w = int((w - size[0]) / 2)
+            h = frame.shape[0]
+            start_h = int((h - size[1]) / 2)
+            return frame[start_h:h - start_h, start_w:w - start_w]
 
     def _createNewFrame(self, cvFrame) -> dai.ImgFrame:
         imgFrame = dai.ImgFrame()
         imgFrame.setData(cvFrame)
         imgFrame.setTimestamp(self._now)
         imgFrame.setSequenceNum(self._seqNum)
         shape = cvFrame.shape[::-1]
         imgFrame.setWidth(shape[0])
         imgFrame.setHeight(shape[1])
         return imgFrame
 
-    def _createImgFrame(self, name: str, cvFrame) -> dai.ImgFrame:
-        imgFrame: dai.ImgFrame
-        if name == 'color':
+    def _createImgFrame(self, stream: ReplayStream) -> dai.ImgFrame:
+        cvFrame: np.ndarray = stream.frame
+        if stream.resize:
+            cvFrame = self._resize_frame(cvFrame, stream.resize, stream.resize_mode)
+
+        if cvFrame.shape[-1] == 3:  # 3 channels = RGB
             # Resize/crop color frame as specified by the user
-            cvFrame = self._resizeColor(cvFrame)
             # cv2 reads frames in interleaved format, and most networks expect planar by default
             cvFrame = toPlanar(cvFrame)
             imgFrame = self._createNewFrame(cvFrame)
             imgFrame.setType(dai.RawImgFrame.Type.BGR888p)
-            imgFrame.setInstanceNum(dai.CameraBoardSocket.RGB)
-        elif name == 'left' or name == 'right':
+            imgFrame.setInstanceNum(int(stream.get_socket()))
+        elif cvFrame.dtype == np.uint8:
             imgFrame = self._createNewFrame(cvFrame)
             imgFrame.setType(dai.RawImgFrame.Type.RAW8)
-            imgFrame.setInstanceNum(getattr(dai.CameraBoardSocket, name.upper()))
-        elif name == 'depth':
+            imgFrame.setInstanceNum(int(stream.get_socket()))
+        elif cvFrame.dtype == np.uint16:
             imgFrame = self._createNewFrame(cvFrame)
             imgFrame.setType(dai.RawImgFrame.Type.RAW16)
+        else:
+            raise Exception('Unknown frame types')
 
         return imgFrame
 
     def _readFrames(self) -> bool:
         """
         Reads frames from all Readers.
         
         Returns:
             bool: True if successful, otherwise False.
         """
-        self.frames = dict()
         frames = self.reader.read()
         if not frames:
             return False  # No more frames!
 
         for name, frame in frames.items():
-            self.frames[name] = frame
+            self.streams[name].frame = frame
 
         # Compress 3-plane frame to a single plane
-        for name, frame in self.frames.items():
-            if name in ["left", "right", "disparity"] and len(frame.shape) == 3:
-                self.frames[name] = frame[:, :, 0]  # All 3 planes are the same
+        # for name, frame in self.frames.items():
+        #     if name in ["left", "right", "disparity"] and len(frame.shape) == 3:
+        #         self.frames[name] = frame[:, :, 0]  # All 3 planes are the same
         return True
 
-    def _getMaxSize(self, name: str) -> int:
-        """
-        Used when setting XLinkIn nodes, so they consume the least amount of memory needed.
-        """
-        size = self.getShape(name)
-        bytes_per_pixel = 1
-        if name == 'color':
-            bytes_per_pixel = 3
-        elif name == 'depth':
-            bytes_per_pixel = 2  # 16bit
-        return size[0] * size[1] * bytes_per_pixel
-
     def getShape(self, name: str) -> Tuple[int, int]:
         """
         Get shape of a stream
         """
-        if name in self.reader.getStreams():
-            return self.reader.getShape(name)
+        return self.streams[name].shape
 
     def close(self):
         """
         Closes all video readers.
         """
         self._stop = True
         if self.thread:
```

### Comparing `depthai-sdk-1.9.4.1/src/depthai_sdk/utils.py` & `depthai-sdk-1.9.5/src/depthai_sdk/utils.py`

 * *Files identical despite different names*

### Comparing `depthai-sdk-1.9.4.1/src/depthai_sdk/visualize/configs.py` & `depthai-sdk-1.9.5/src/depthai_sdk/visualize/configs.py`

 * *Files 6% similar despite different names*

```diff
@@ -91,14 +91,15 @@
 @dataclass
 class TrackingConfig:
     """Configuration for drawing tracking bounding boxes."""
     max_length: int = -1
     deletion_lost_threshold: int = 5
     line_thickness: int = 1
     fading_tails: bool = False
+    speed: bool = False
     line_color: Tuple[int, int, int] = (255, 255, 255)
     line_type: int = 16  # cv2.LINE_AA
     bg_color: Tuple[int, int, int] = (0, 0, 0)
 
 
 @dataclass
 class SegmentationConfig:
```

### Comparing `depthai-sdk-1.9.4.1/src/depthai_sdk/visualize/encoder.py` & `depthai-sdk-1.9.5/src/depthai_sdk/visualize/encoder.py`

 * *Files identical despite different names*

### Comparing `depthai-sdk-1.9.4.1/src/depthai_sdk/visualize/objects.py` & `depthai-sdk-1.9.5/src/depthai_sdk/visualize/objects.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import logging
 from abc import ABC, abstractmethod
 from collections import defaultdict
 from typing import Tuple, List, Union
 
 try:
     import cv2
 except ImportError:
@@ -294,16 +295,16 @@
 
         for i, detection in enumerate(self.detections):
             # Get normalized bounding box
             bbox = detection.xmin, detection.ymin, detection.xmax, detection.ymax
             mock_frame = np.zeros(self.frame_shape, dtype=np.uint8)
 
             if mock_frame.ndim < 2:
-                print('Frame shape is 1D, please make sure that you are not using encoded frames.'
-                      'If you are using encoded frames, please decode them first.')
+                logging.debug('Visualizer: skipping detection because frame shape is invalid: {}'
+                              .format(mock_frame.shape))
                 return self
             # TODO can normalize accept frame shape?
             normalized_bbox = self.normalizer.normalize(mock_frame, bbox) if self.normalizer else bbox
 
             if self.label_map:
                 label, color = self.label_map[detection.label]
             else:
```

### Comparing `depthai-sdk-1.9.4.1/src/depthai_sdk/visualize/visualizer.py` & `depthai-sdk-1.9.5/src/depthai_sdk/visualize/visualizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,15 +86,15 @@
 
     def add_text(self,
                  text: str,
                  coords: Tuple[int, int] = None,
                  size: int = None,
                  color: Tuple[int, int, int] = None,
                  thickness: int = None,
-                 outline: bool = False,
+                 outline: bool = True,
                  bbox: Union[np.ndarray, Tuple[int, int, int, int]] = None,
                  position: TextPosition = TextPosition.TOP_LEFT,
                  padding: int = 10) -> 'Visualizer':
         """
         Add text to the visualizer.
 
         Args:
@@ -355,25 +355,27 @@
         return self
 
     def tracking(self,
                  max_length: int = None,
                  deletion_lost_threshold: int = None,
                  line_thickness: int = None,
                  fading_tails: bool = None,
+                 speed: bool = None,
                  line_color: Tuple[int, int, int] = None,
                  line_type: int = None,
                  bg_color: Tuple[int, int, int] = None) -> 'Visualizer':
         """
         Configure how tracking trails will look like.
 
         Args:
             max_length: Maximum length of the trail (in pixels).
             deletion_lost_threshold: Number of consequent LOST statuses after which the trail is deleted.
             line_thickness: Thickness of the line.
             fading_tails: Flag that indicates if the tails should fade.
+            speed: Flag that indicates if the speed should be shown.
             line_color: Color of the line.
             line_type: Type of the line (from cv2).
             bg_color: Text background color.
 
         Returns:
             self
         """
```

### Comparing `depthai-sdk-1.9.4.1/src/depthai_sdk/visualize/visualizer_helper.py` & `depthai-sdk-1.9.5/src/depthai_sdk/visualize/visualizer_helper.py`

 * *Files identical despite different names*

### Comparing `depthai-sdk-1.9.4.1/src/depthai_sdk.egg-info/PKG-INFO` & `depthai-sdk-1.9.5/src/depthai_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: depthai-sdk
-Version: 1.9.4.1
+Version: 1.9.5
 Summary: This package provides an abstraction of the DepthAI API library.
 Home-page: https://github.com/luxonis/depthai/tree/main/depthai_sdk
 Author: Luxonis
 Author-email: support@luxonis.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/luxonis/depthai/issues
 Project-URL: Source Code, https://github.com/luxonis/depthai/tree/main/depthai_sdk
```

### Comparing `depthai-sdk-1.9.4.1/src/depthai_sdk.egg-info/SOURCES.txt` & `depthai-sdk-1.9.5/src/depthai_sdk.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 MANIFEST.in
 README.md
 requirements.txt
 setup.py
 src/depthai_sdk/__init__.py
 src/depthai_sdk/args_parser.py
 src/depthai_sdk/fps.py
+src/depthai_sdk/logger.py
 src/depthai_sdk/oak_camera.py
 src/depthai_sdk/oak_device.py
 src/depthai_sdk/previews.py
 src/depthai_sdk/record.py
 src/depthai_sdk/replay.py
 src/depthai_sdk/types.py
 src/depthai_sdk/utils.py
 src/depthai_sdk.egg-info/PKG-INFO
 src/depthai_sdk.egg-info/SOURCES.txt
 src/depthai_sdk.egg-info/dependency_links.txt
 src/depthai_sdk.egg-info/requires.txt
 src/depthai_sdk.egg-info/top_level.txt
 src/depthai_sdk/classes/__init__.py
+src/depthai_sdk/classes/enum.py
 src/depthai_sdk/classes/nn_config.py
 src/depthai_sdk/classes/nn_results.py
 src/depthai_sdk/classes/output_config.py
 src/depthai_sdk/classes/packets.py
 src/depthai_sdk/classes/yolo_config.py
 src/depthai_sdk/components/__init__.py
 src/depthai_sdk/components/camera_component.py
@@ -30,15 +32,23 @@
 src/depthai_sdk/components/imu_component.py
 src/depthai_sdk/components/multi_stage_nn.py
 src/depthai_sdk/components/nn_component.py
 src/depthai_sdk/components/nn_helper.py
 src/depthai_sdk/components/parser.py
 src/depthai_sdk/components/stereo_component.py
 src/depthai_sdk/components/template_multi_stage_script.py
-src/depthai_sdk/components/integrations/roboflow.py
+src/depthai_sdk/components/undistort.py
+src/depthai_sdk/integrations/__init__.py
+src/depthai_sdk/integrations/roboflow.py
+src/depthai_sdk/integrations/ros/__init__.py
+src/depthai_sdk/integrations/ros/depthai2ros.py
+src/depthai_sdk/integrations/ros/depthai2ros2.py
+src/depthai_sdk/integrations/ros/imu_interpolation.py
+src/depthai_sdk/integrations/ros/ros2_streaming.py
+src/depthai_sdk/integrations/ros/ros_base.py
 src/depthai_sdk/managers/__init__.py
 src/depthai_sdk/managers/arg_manager.py
 src/depthai_sdk/managers/blob_manager.py
 src/depthai_sdk/managers/encoding_manager.py
 src/depthai_sdk/managers/nnet_manager.py
 src/depthai_sdk/managers/pipeline_manager.py
 src/depthai_sdk/managers/preview_manager.py
@@ -52,14 +62,16 @@
 src/depthai_sdk/nn_models/face-detection-retail-0004/config.json
 src/depthai_sdk/nn_models/human-pose-estimation-0001/config.json
 src/depthai_sdk/nn_models/human-pose-estimation-0001/handler.py
 src/depthai_sdk/nn_models/mobilenet-ssd/config.json
 src/depthai_sdk/nn_models/openpose2/config.json
 src/depthai_sdk/nn_models/openpose2/handler.py
 src/depthai_sdk/nn_models/openpose2/model.yml
+src/depthai_sdk/nn_models/palm_detection_128x128/config.json
+src/depthai_sdk/nn_models/palm_detection_128x128/handler.py
 src/depthai_sdk/nn_models/pedestrian-detection-adas-0002/config.json
 src/depthai_sdk/nn_models/person-detection-0200/config.json
 src/depthai_sdk/nn_models/person-detection-retail-0013/config.json
 src/depthai_sdk/nn_models/person-reidentification-retail-0288/config.json
 src/depthai_sdk/nn_models/person-reidentification-retail-0288/handler.py
 src/depthai_sdk/nn_models/person-vehicle-bike-detection-crossroad-1016/config.json
 src/depthai_sdk/nn_models/road-segmentation-adas-0001/config.json
@@ -71,14 +83,18 @@
 src/depthai_sdk/nn_models/vehicle-license-plate-detection-barrier-0106/config.json
 src/depthai_sdk/nn_models/yolo-v3-tf/config.json
 src/depthai_sdk/nn_models/yolo-v3-tiny-tf/config.json
 src/depthai_sdk/nn_models/yolov4_coco_608x608/config.json
 src/depthai_sdk/nn_models/yolov4_tiny_coco_416x416/config.json
 src/depthai_sdk/nn_models/yolov5n_coco_416x416/config.json
 src/depthai_sdk/nn_models/yolov6n_coco_640x640/config.json
+src/depthai_sdk/nn_models/yolov6nr3_coco_640x352/config.json
+src/depthai_sdk/nn_models/yolov7tiny_coco_416x416/config.json
+src/depthai_sdk/nn_models/yolov7tiny_coco_640x352/config.json
+src/depthai_sdk/nn_models/yolov8n_coco_640x352/config.json
 src/depthai_sdk/oak_outputs/__init__.py
 src/depthai_sdk/oak_outputs/fps.py
 src/depthai_sdk/oak_outputs/normalize_bb.py
 src/depthai_sdk/oak_outputs/syncing.py
 src/depthai_sdk/oak_outputs/xout/__init__.py
 src/depthai_sdk/oak_outputs/xout/xout_base.py
 src/depthai_sdk/oak_outputs/xout/xout_depth.py
@@ -96,24 +112,25 @@
 src/depthai_sdk/readers/db3_reader.py
 src/depthai_sdk/readers/image_reader.py
 src/depthai_sdk/readers/mcap_reader.py
 src/depthai_sdk/readers/rosbag_reader.py
 src/depthai_sdk/readers/videocap_reader.py
 src/depthai_sdk/recorders/__init__.py
 src/depthai_sdk/recorders/abstract_recorder.py
-src/depthai_sdk/recorders/depthai2ros.py
 src/depthai_sdk/recorders/mcap_recorder.py
 src/depthai_sdk/recorders/rosbag_recorder.py
 src/depthai_sdk/recorders/video_recorder.py
 src/depthai_sdk/recorders/video_writers/__init__.py
 src/depthai_sdk/recorders/video_writers/abstract_writer.py
 src/depthai_sdk/recorders/video_writers/av_writer.py
 src/depthai_sdk/recorders/video_writers/file_writer.py
 src/depthai_sdk/recorders/video_writers/utils.py
 src/depthai_sdk/recorders/video_writers/video_writer.py
+src/depthai_sdk/tracking/__init__.py
+src/depthai_sdk/tracking/kalman.py
 src/depthai_sdk/visualize/__init__.py
 src/depthai_sdk/visualize/configs.py
 src/depthai_sdk/visualize/encoder.py
 src/depthai_sdk/visualize/objects.py
 src/depthai_sdk/visualize/polygon.py
 src/depthai_sdk/visualize/visualizer.py
 src/depthai_sdk/visualize/visualizer_helper.py
```

### Comparing `depthai-sdk-1.9.4.1/src/depthai_sdk.egg-info/requires.txt` & `depthai-sdk-1.9.5/src/depthai_sdk.egg-info/requires.txt`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 opencv-contrib-python>4
 blobconverter>=1.2.8
 pytube>=12.1.0
-depthai>=2.20.1.0
+depthai==2.21.2
 PyTurboJPEG==1.6.4
 marshmallow==3.17.0
 distinctipy
 xmltodict
 
 [:python_version < "3.7"]
 numpy>=1.19
```

