# Comparing `tmp/prolog_primitives-0.4.1.tar.gz` & `tmp/prolog_primitives-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prolog_primitives-0.4.1.tar", last modified: Sat Jul  1 10:35:10 2023, max compression
+gzip compressed data, was "prolog_primitives-0.4.2.tar", last modified: Sun Jul  2 16:00:33 2023, max compression
```

## Comparing `prolog_primitives-0.4.1.tar` & `prolog_primitives-0.4.2.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 10:35:10.107066 prolog_primitives-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11353 2023-07-01 10:33:51.000000 prolog_primitives-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-01 10:33:51.000000 prolog_primitives-0.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-01 10:35:10.107066 prolog_primitives-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-01 10:33:51.000000 prolog_primitives-0.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 10:35:10.099066 prolog_primitives-0.4.1/prolog_primitives/
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-01 10:35:03.000000 prolog_primitives-0.4.1/prolog_primitives/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 10:35:10.099066 prolog_primitives-0.4.1/prolog_primitives/basic/
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-07-01 10:33:51.000000 prolog_primitives-0.4.1/prolog_primitives/basic/DBManager.py
--rw-r--r--   0 runner    (1001) docker     (123)     4249 2023-07-01 10:33:51.000000 prolog_primitives-0.4.1/prolog_primitives/basic/DistributedElements.py
--rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-07-01 10:33:51.000000 prolog_primitives-0.4.1/prolog_primitives/basic/PrimitiveWrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4938 2023-07-01 10:33:51.000000 prolog_primitives-0.4.1/prolog_primitives/basic/Session.py
--rw-r--r--   0 runner    (1001) docker     (123)     3858 2023-07-01 10:33:51.000000 prolog_primitives-0.4.1/prolog_primitives/basic/SubRequestEvent.py
--rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-07-01 10:33:51.000000 prolog_primitives-0.4.1/prolog_primitives/basic/Utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-01 10:33:51.000000 prolog_primitives-0.4.1/prolog_primitives/basic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-07-01 10:33:51.000000 prolog_primitives-0.4.1/prolog_primitives/basic/filterKbPrimitive.py
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-01 10:33:51.000000 prolog_primitives-0.4.1/prolog_primitives/basic/ntPrimitive.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 10:35:10.103066 prolog_primitives-0.4.1/prolog_primitives/generatedProto/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 10:35:03.000000 prolog_primitives-0.4.1/prolog_primitives/generatedProto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7130 2023-07-01 10:35:03.000000 prolog_primitives-0.4.1/prolog_primitives/generatedProto/basicMessages_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-01 10:35:03.000000 prolog_primitives-0.4.1/prolog_primitives/generatedProto/basicMessages_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5228 2023-07-01 10:35:03.000000 prolog_primitives-0.4.1/prolog_primitives/generatedProto/errorsMessages_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-01 10:35:03.000000 prolog_primitives-0.4.1/prolog_primitives/generatedProto/errorsMessages_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     9189 2023-07-01 10:35:03.000000 prolog_primitives-0.4.1/prolog_primitives/generatedProto/primitiveService_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-07-01 10:35:03.000000 prolog_primitives-0.4.1/prolog_primitives/generatedProto/primitiveService_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     9838 2023-07-01 10:35:03.000000 prolog_primitives-0.4.1/prolog_primitives/generatedProto/sideEffectsMessages_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-01 10:35:03.000000 prolog_primitives-0.4.1/prolog_primitives/generatedProto/sideEffectsMessages_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 10:35:10.103066 prolog_primitives-0.4.1/prolog_primitives/ml_lib/
--rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-07-01 10:33:51.000000 prolog_primitives-0.4.1/prolog_primitives/ml_lib/Collections.py
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-01 10:33:51.000000 prolog_primitives-0.4.1/prolog_primitives/ml_lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-01 10:33:51.000000 prolog_primitives-0.4.1/prolog_primitives/ml_lib/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 10:35:10.103066 prolog_primitives-0.4.1/prolog_primitives/ml_lib/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-07-01 10:33:51.000000 prolog_primitives-0.4.1/prolog_primitives/ml_lib/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-07-01 10:33:51.000000 prolog_primitives-0.4.1/prolog_primitives/ml_lib/dataset/cell.py
--rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-07-01 10:33:51.000000 prolog_primitives-0.4.1/prolog_primitives/ml_lib/dataset/column.py
--rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-07-01 10:33:51.000000 prolog_primitives-0.4.1/prolog_primitives/ml_lib/dataset/fold.py
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-07-01 10:33:51.000000 prolog_primitives-0.4.1/prolog_primitives/ml_lib/dataset/randomSplit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-07-01 10:33:51.000000 prolog_primitives-0.4.1/prolog_primitives/ml_lib/dataset/row.py
--rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-07-01 10:33:51.000000 prolog_primitives-0.4.1/prolog_primitives/ml_lib/dataset/theoryToDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-07-01 10:33:51.000000 prolog_primitives-0.4.1/prolog_primitives/ml_lib/dataset/theory_from_Dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-07-01 10:33:51.000000 prolog_primitives-0.4.1/prolog_primitives/ml_lib/launcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 10:35:10.103066 prolog_primitives-0.4.1/prolog_primitives/ml_lib/neuralNetwork/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-01 10:33:51.000000 prolog_primitives-0.4.1/prolog_primitives/ml_lib/neuralNetwork/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-07-01 10:33:51.000000 prolog_primitives-0.4.1/prolog_primitives/ml_lib/neuralNetwork/denseLayer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-07-01 10:33:51.000000 prolog_primitives-0.4.1/prolog_primitives/ml_lib/neuralNetwork/inputLayer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-07-01 10:33:51.000000 prolog_primitives-0.4.1/prolog_primitives/ml_lib/neuralNetwork/neuralNetwork.py
--rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-07-01 10:33:51.000000 prolog_primitives-0.4.1/prolog_primitives/ml_lib/neuralNetwork/outputLayer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 10:35:10.103066 prolog_primitives-0.4.1/prolog_primitives/ml_lib/predictors/
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-01 10:33:51.000000 prolog_primitives-0.4.1/prolog_primitives/ml_lib/predictors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-07-01 10:33:51.000000 prolog_primitives-0.4.1/prolog_primitives/ml_lib/predictors/classify.py
--rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-07-01 10:33:51.000000 prolog_primitives-0.4.1/prolog_primitives/ml_lib/predictors/predict.py
--rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-07-01 10:33:51.000000 prolog_primitives-0.4.1/prolog_primitives/ml_lib/predictors/score.py
--rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-07-01 10:33:51.000000 prolog_primitives-0.4.1/prolog_primitives/ml_lib/predictors/train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 10:35:10.103066 prolog_primitives-0.4.1/prolog_primitives/ml_lib/schema/
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-01 10:33:51.000000 prolog_primitives-0.4.1/prolog_primitives/ml_lib/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-07-01 10:33:51.000000 prolog_primitives-0.4.1/prolog_primitives/ml_lib/schema/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-07-01 10:33:51.000000 prolog_primitives-0.4.1/prolog_primitives/ml_lib/schema/schemaClass.py
--rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-07-01 10:33:51.000000 prolog_primitives-0.4.1/prolog_primitives/ml_lib/schema/theoryToSchema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 10:35:10.107066 prolog_primitives-0.4.1/prolog_primitives/ml_lib/transformations/
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-01 10:33:51.000000 prolog_primitives-0.4.1/prolog_primitives/ml_lib/transformations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-07-01 10:33:51.000000 prolog_primitives-0.4.1/prolog_primitives/ml_lib/transformations/drop.py
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-07-01 10:33:51.000000 prolog_primitives-0.4.1/prolog_primitives/ml_lib/transformations/fit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-07-01 10:33:51.000000 prolog_primitives-0.4.1/prolog_primitives/ml_lib/transformations/normalization.py
--rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-07-01 10:33:51.000000 prolog_primitives-0.4.1/prolog_primitives/ml_lib/transformations/one_hot_encode.py
--rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-07-01 10:33:51.000000 prolog_primitives-0.4.1/prolog_primitives/ml_lib/transformations/schema_trasformation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-07-01 10:33:51.000000 prolog_primitives-0.4.1/prolog_primitives/ml_lib/transformations/transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     4539 2023-07-01 10:33:51.000000 prolog_primitives-0.4.1/prolog_primitives/ml_lib/transformations/transformationClass.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 10:35:10.099066 prolog_primitives-0.4.1/prolog_primitives.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-01 10:35:10.000000 prolog_primitives-0.4.1/prolog_primitives.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-07-01 10:35:10.000000 prolog_primitives-0.4.1/prolog_primitives.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 10:35:10.000000 prolog_primitives-0.4.1/prolog_primitives.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 10:35:09.000000 prolog_primitives-0.4.1/prolog_primitives.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-01 10:35:10.000000 prolog_primitives-0.4.1/prolog_primitives.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-01 10:35:10.000000 prolog_primitives-0.4.1/prolog_primitives.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-01 10:33:51.000000 prolog_primitives-0.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-01 10:33:51.000000 prolog_primitives-0.4.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 10:35:10.107066 prolog_primitives-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-07-01 10:33:51.000000 prolog_primitives-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 16:00:33.364863 prolog_primitives-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11353 2023-07-02 15:59:11.000000 prolog_primitives-0.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-02 15:59:11.000000 prolog_primitives-0.4.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-02 16:00:33.364863 prolog_primitives-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-02 15:59:11.000000 prolog_primitives-0.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 16:00:33.356862 prolog_primitives-0.4.2/prolog_primitives/
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-02 16:00:25.000000 prolog_primitives-0.4.2/prolog_primitives/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 16:00:33.360862 prolog_primitives-0.4.2/prolog_primitives/basic/
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-07-02 15:59:11.000000 prolog_primitives-0.4.2/prolog_primitives/basic/DBManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4249 2023-07-02 15:59:11.000000 prolog_primitives-0.4.2/prolog_primitives/basic/DistributedElements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-07-02 15:59:11.000000 prolog_primitives-0.4.2/prolog_primitives/basic/PrimitiveWrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4938 2023-07-02 15:59:11.000000 prolog_primitives-0.4.2/prolog_primitives/basic/Session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3858 2023-07-02 15:59:11.000000 prolog_primitives-0.4.2/prolog_primitives/basic/SubRequestEvent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-07-02 15:59:11.000000 prolog_primitives-0.4.2/prolog_primitives/basic/Utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-02 15:59:11.000000 prolog_primitives-0.4.2/prolog_primitives/basic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-07-02 15:59:11.000000 prolog_primitives-0.4.2/prolog_primitives/basic/filterKbPrimitive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-02 15:59:11.000000 prolog_primitives-0.4.2/prolog_primitives/basic/ntPrimitive.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 16:00:33.360862 prolog_primitives-0.4.2/prolog_primitives/generatedProto/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 16:00:25.000000 prolog_primitives-0.4.2/prolog_primitives/generatedProto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7130 2023-07-02 16:00:25.000000 prolog_primitives-0.4.2/prolog_primitives/generatedProto/basicMessages_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-02 16:00:25.000000 prolog_primitives-0.4.2/prolog_primitives/generatedProto/basicMessages_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5228 2023-07-02 16:00:25.000000 prolog_primitives-0.4.2/prolog_primitives/generatedProto/errorsMessages_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-02 16:00:25.000000 prolog_primitives-0.4.2/prolog_primitives/generatedProto/errorsMessages_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9189 2023-07-02 16:00:25.000000 prolog_primitives-0.4.2/prolog_primitives/generatedProto/primitiveService_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-07-02 16:00:25.000000 prolog_primitives-0.4.2/prolog_primitives/generatedProto/primitiveService_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9838 2023-07-02 16:00:25.000000 prolog_primitives-0.4.2/prolog_primitives/generatedProto/sideEffectsMessages_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-02 16:00:25.000000 prolog_primitives-0.4.2/prolog_primitives/generatedProto/sideEffectsMessages_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 16:00:33.360862 prolog_primitives-0.4.2/prolog_primitives/ml_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-02 15:59:11.000000 prolog_primitives-0.4.2/prolog_primitives/ml_lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-02 15:59:11.000000 prolog_primitives-0.4.2/prolog_primitives/ml_lib/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-07-02 15:59:11.000000 prolog_primitives-0.4.2/prolog_primitives/ml_lib/collections.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 16:00:33.364863 prolog_primitives-0.4.2/prolog_primitives/ml_lib/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-07-02 15:59:11.000000 prolog_primitives-0.4.2/prolog_primitives/ml_lib/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-07-02 15:59:11.000000 prolog_primitives-0.4.2/prolog_primitives/ml_lib/dataset/cell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-07-02 15:59:11.000000 prolog_primitives-0.4.2/prolog_primitives/ml_lib/dataset/column.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-07-02 15:59:11.000000 prolog_primitives-0.4.2/prolog_primitives/ml_lib/dataset/fold.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-07-02 15:59:11.000000 prolog_primitives-0.4.2/prolog_primitives/ml_lib/dataset/randomSplit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-07-02 15:59:11.000000 prolog_primitives-0.4.2/prolog_primitives/ml_lib/dataset/row.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-07-02 15:59:11.000000 prolog_primitives-0.4.2/prolog_primitives/ml_lib/dataset/theoryToDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-07-02 15:59:11.000000 prolog_primitives-0.4.2/prolog_primitives/ml_lib/dataset/theory_from_Dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-07-02 15:59:11.000000 prolog_primitives-0.4.2/prolog_primitives/ml_lib/launcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 16:00:33.364863 prolog_primitives-0.4.2/prolog_primitives/ml_lib/neuralNetwork/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-02 15:59:11.000000 prolog_primitives-0.4.2/prolog_primitives/ml_lib/neuralNetwork/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-07-02 15:59:11.000000 prolog_primitives-0.4.2/prolog_primitives/ml_lib/neuralNetwork/denseLayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-07-02 15:59:11.000000 prolog_primitives-0.4.2/prolog_primitives/ml_lib/neuralNetwork/inputLayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-07-02 15:59:11.000000 prolog_primitives-0.4.2/prolog_primitives/ml_lib/neuralNetwork/neuralNetwork.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-07-02 15:59:11.000000 prolog_primitives-0.4.2/prolog_primitives/ml_lib/neuralNetwork/outputLayer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 16:00:33.364863 prolog_primitives-0.4.2/prolog_primitives/ml_lib/predictors/
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-02 15:59:11.000000 prolog_primitives-0.4.2/prolog_primitives/ml_lib/predictors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-07-02 15:59:11.000000 prolog_primitives-0.4.2/prolog_primitives/ml_lib/predictors/classify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-07-02 15:59:11.000000 prolog_primitives-0.4.2/prolog_primitives/ml_lib/predictors/predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-07-02 15:59:11.000000 prolog_primitives-0.4.2/prolog_primitives/ml_lib/predictors/score.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-07-02 15:59:11.000000 prolog_primitives-0.4.2/prolog_primitives/ml_lib/predictors/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 16:00:33.364863 prolog_primitives-0.4.2/prolog_primitives/ml_lib/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-02 15:59:11.000000 prolog_primitives-0.4.2/prolog_primitives/ml_lib/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-07-02 15:59:11.000000 prolog_primitives-0.4.2/prolog_primitives/ml_lib/schema/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-07-02 15:59:11.000000 prolog_primitives-0.4.2/prolog_primitives/ml_lib/schema/schemaClass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-07-02 15:59:11.000000 prolog_primitives-0.4.2/prolog_primitives/ml_lib/schema/theoryToSchema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 16:00:33.364863 prolog_primitives-0.4.2/prolog_primitives/ml_lib/transformations/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-02 15:59:11.000000 prolog_primitives-0.4.2/prolog_primitives/ml_lib/transformations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-07-02 15:59:11.000000 prolog_primitives-0.4.2/prolog_primitives/ml_lib/transformations/drop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-07-02 15:59:11.000000 prolog_primitives-0.4.2/prolog_primitives/ml_lib/transformations/fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-07-02 15:59:11.000000 prolog_primitives-0.4.2/prolog_primitives/ml_lib/transformations/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-07-02 15:59:11.000000 prolog_primitives-0.4.2/prolog_primitives/ml_lib/transformations/one_hot_encode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-07-02 15:59:11.000000 prolog_primitives-0.4.2/prolog_primitives/ml_lib/transformations/schema_trasformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-07-02 15:59:11.000000 prolog_primitives-0.4.2/prolog_primitives/ml_lib/transformations/transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4539 2023-07-02 15:59:11.000000 prolog_primitives-0.4.2/prolog_primitives/ml_lib/transformations/transformationClass.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 16:00:33.360862 prolog_primitives-0.4.2/prolog_primitives.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-02 16:00:33.000000 prolog_primitives-0.4.2/prolog_primitives.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-07-02 16:00:33.000000 prolog_primitives-0.4.2/prolog_primitives.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 16:00:33.000000 prolog_primitives-0.4.2/prolog_primitives.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 16:00:33.000000 prolog_primitives-0.4.2/prolog_primitives.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-02 16:00:33.000000 prolog_primitives-0.4.2/prolog_primitives.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-02 16:00:33.000000 prolog_primitives-0.4.2/prolog_primitives.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-02 15:59:11.000000 prolog_primitives-0.4.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-02 15:59:11.000000 prolog_primitives-0.4.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 16:00:33.364863 prolog_primitives-0.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-07-02 15:59:11.000000 prolog_primitives-0.4.2/setup.py
```

### Comparing `prolog_primitives-0.4.1/LICENSE` & `prolog_primitives-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `prolog_primitives-0.4.1/PKG-INFO` & `prolog_primitives-0.4.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prolog_primitives
-Version: 0.4.1
+Version: 0.4.2
 Summary: description here
 Home-page: https://github.com/lorenzo-osimani/prolog_primitives/
 Author: Lorenzo Osimani
 Author-email: lorenzo.osimani@studio.unibo.it
 License: Apache 2.0 License
 Project-URL: Bug Reports, https://github.com/lorenzo-osimani/prolog_primitives/issues
 Project-URL: Source, https://github.com/lorenzo-osimani/prolog_primitives/
```

### Comparing `prolog_primitives-0.4.1/prolog_primitives/basic/DBManager.py` & `prolog_primitives-0.4.2/prolog_primitives/basic/DBManager.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-0.4.1/prolog_primitives/basic/DistributedElements.py` & `prolog_primitives-0.4.2/prolog_primitives/basic/DistributedElements.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-0.4.1/prolog_primitives/basic/PrimitiveWrapper.py` & `prolog_primitives-0.4.2/prolog_primitives/basic/PrimitiveWrapper.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-0.4.1/prolog_primitives/basic/Session.py` & `prolog_primitives-0.4.2/prolog_primitives/basic/Session.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-0.4.1/prolog_primitives/basic/SubRequestEvent.py` & `prolog_primitives-0.4.2/prolog_primitives/basic/SubRequestEvent.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-0.4.1/prolog_primitives/basic/Utils.py` & `prolog_primitives-0.4.2/prolog_primitives/basic/Utils.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-0.4.1/prolog_primitives/basic/filterKbPrimitive.py` & `prolog_primitives-0.4.2/prolog_primitives/basic/filterKbPrimitive.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-0.4.1/prolog_primitives/basic/ntPrimitive.py` & `prolog_primitives-0.4.2/prolog_primitives/basic/ntPrimitive.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-0.4.1/prolog_primitives/generatedProto/basicMessages_pb2.py` & `prolog_primitives-0.4.2/prolog_primitives/generatedProto/basicMessages_pb2.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-0.4.1/prolog_primitives/generatedProto/errorsMessages_pb2.py` & `prolog_primitives-0.4.2/prolog_primitives/generatedProto/errorsMessages_pb2.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-0.4.1/prolog_primitives/generatedProto/primitiveService_pb2.py` & `prolog_primitives-0.4.2/prolog_primitives/generatedProto/primitiveService_pb2.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-0.4.1/prolog_primitives/generatedProto/primitiveService_pb2_grpc.py` & `prolog_primitives-0.4.2/prolog_primitives/generatedProto/primitiveService_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-0.4.1/prolog_primitives/generatedProto/sideEffectsMessages_pb2.py` & `prolog_primitives-0.4.2/prolog_primitives/generatedProto/sideEffectsMessages_pb2.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-0.4.1/prolog_primitives/ml_lib/Collections.py` & `prolog_primitives-0.4.2/prolog_primitives/ml_lib/collections.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-0.4.1/prolog_primitives/ml_lib/dataset/cell.py` & `prolog_primitives-0.4.2/prolog_primitives/ml_lib/dataset/cell.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-0.4.1/prolog_primitives/ml_lib/dataset/column.py` & `prolog_primitives-0.4.2/prolog_primitives/ml_lib/dataset/column.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-0.4.1/prolog_primitives/ml_lib/dataset/fold.py` & `prolog_primitives-0.4.2/prolog_primitives/ml_lib/dataset/fold.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-0.4.1/prolog_primitives/ml_lib/dataset/randomSplit.py` & `prolog_primitives-0.4.2/prolog_primitives/ml_lib/dataset/randomSplit.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-0.4.1/prolog_primitives/ml_lib/dataset/row.py` & `prolog_primitives-0.4.2/prolog_primitives/ml_lib/dataset/row.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-0.4.1/prolog_primitives/ml_lib/dataset/theoryToDataset.py` & `prolog_primitives-0.4.2/prolog_primitives/ml_lib/dataset/theoryToDataset.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-0.4.1/prolog_primitives/ml_lib/dataset/theory_from_Dataset.py` & `prolog_primitives-0.4.2/prolog_primitives/ml_lib/dataset/theory_from_Dataset.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-0.4.1/prolog_primitives/ml_lib/launcher.py` & `prolog_primitives-0.4.2/prolog_primitives/ml_lib/launcher.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-0.4.1/prolog_primitives/ml_lib/neuralNetwork/denseLayer.py` & `prolog_primitives-0.4.2/prolog_primitives/ml_lib/neuralNetwork/denseLayer.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-0.4.1/prolog_primitives/ml_lib/neuralNetwork/inputLayer.py` & `prolog_primitives-0.4.2/prolog_primitives/ml_lib/neuralNetwork/inputLayer.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-0.4.1/prolog_primitives/ml_lib/neuralNetwork/neuralNetwork.py` & `prolog_primitives-0.4.2/prolog_primitives/ml_lib/neuralNetwork/neuralNetwork.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-0.4.1/prolog_primitives/ml_lib/neuralNetwork/outputLayer.py` & `prolog_primitives-0.4.2/prolog_primitives/ml_lib/neuralNetwork/outputLayer.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-0.4.1/prolog_primitives/ml_lib/predictors/classify.py` & `prolog_primitives-0.4.2/prolog_primitives/ml_lib/predictors/classify.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-0.4.1/prolog_primitives/ml_lib/predictors/predict.py` & `prolog_primitives-0.4.2/prolog_primitives/ml_lib/predictors/predict.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-0.4.1/prolog_primitives/ml_lib/predictors/score.py` & `prolog_primitives-0.4.2/prolog_primitives/ml_lib/predictors/score.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-0.4.1/prolog_primitives/ml_lib/predictors/train.py` & `prolog_primitives-0.4.2/prolog_primitives/ml_lib/predictors/train.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-0.4.1/prolog_primitives/ml_lib/schema/schema.py` & `prolog_primitives-0.4.2/prolog_primitives/ml_lib/schema/schema.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-0.4.1/prolog_primitives/ml_lib/schema/schemaClass.py` & `prolog_primitives-0.4.2/prolog_primitives/ml_lib/schema/schemaClass.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-0.4.1/prolog_primitives/ml_lib/schema/theoryToSchema.py` & `prolog_primitives-0.4.2/prolog_primitives/ml_lib/schema/theoryToSchema.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-0.4.1/prolog_primitives/ml_lib/transformations/drop.py` & `prolog_primitives-0.4.2/prolog_primitives/ml_lib/transformations/drop.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-0.4.1/prolog_primitives/ml_lib/transformations/fit.py` & `prolog_primitives-0.4.2/prolog_primitives/ml_lib/transformations/fit.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-0.4.1/prolog_primitives/ml_lib/transformations/normalization.py` & `prolog_primitives-0.4.2/prolog_primitives/ml_lib/transformations/normalization.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-0.4.1/prolog_primitives/ml_lib/transformations/one_hot_encode.py` & `prolog_primitives-0.4.2/prolog_primitives/ml_lib/transformations/one_hot_encode.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-0.4.1/prolog_primitives/ml_lib/transformations/schema_trasformation.py` & `prolog_primitives-0.4.2/prolog_primitives/ml_lib/transformations/schema_trasformation.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-0.4.1/prolog_primitives/ml_lib/transformations/transform.py` & `prolog_primitives-0.4.2/prolog_primitives/ml_lib/transformations/transform.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-0.4.1/prolog_primitives/ml_lib/transformations/transformationClass.py` & `prolog_primitives-0.4.2/prolog_primitives/ml_lib/transformations/transformationClass.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-0.4.1/prolog_primitives.egg-info/PKG-INFO` & `prolog_primitives-0.4.2/prolog_primitives.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prolog-primitives
-Version: 0.4.1
+Version: 0.4.2
 Summary: description here
 Home-page: https://github.com/lorenzo-osimani/prolog_primitives/
 Author: Lorenzo Osimani
 Author-email: lorenzo.osimani@studio.unibo.it
 License: Apache 2.0 License
 Project-URL: Bug Reports, https://github.com/lorenzo-osimani/prolog_primitives/issues
 Project-URL: Source, https://github.com/lorenzo-osimani/prolog_primitives/
```

### Comparing `prolog_primitives-0.4.1/prolog_primitives.egg-info/SOURCES.txt` & `prolog_primitives-0.4.2/prolog_primitives.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -25,17 +25,17 @@
 prolog_primitives/generatedProto/basicMessages_pb2_grpc.py
 prolog_primitives/generatedProto/errorsMessages_pb2.py
 prolog_primitives/generatedProto/errorsMessages_pb2_grpc.py
 prolog_primitives/generatedProto/primitiveService_pb2.py
 prolog_primitives/generatedProto/primitiveService_pb2_grpc.py
 prolog_primitives/generatedProto/sideEffectsMessages_pb2.py
 prolog_primitives/generatedProto/sideEffectsMessages_pb2_grpc.py
-prolog_primitives/ml_lib/Collections.py
 prolog_primitives/ml_lib/__init__.py
 prolog_primitives/ml_lib/__main__.py
+prolog_primitives/ml_lib/collections.py
 prolog_primitives/ml_lib/launcher.py
 prolog_primitives/ml_lib/dataset/__init__.py
 prolog_primitives/ml_lib/dataset/cell.py
 prolog_primitives/ml_lib/dataset/column.py
 prolog_primitives/ml_lib/dataset/fold.py
 prolog_primitives/ml_lib/dataset/randomSplit.py
 prolog_primitives/ml_lib/dataset/row.py
```

### Comparing `prolog_primitives-0.4.1/setup.py` & `prolog_primitives-0.4.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         with version_file.open('w') as f:
             f.write(version)
         return version
     except subprocess.CalledProcessError:
         if version_file.exists():
             return version_file.read_text().strip()
         else:
-            return '0.4.1'
+            return '0.4.2'
 
 
 version = get_version_from_git()
 
 
 print(f"Detected version {version} from git describe")
```

