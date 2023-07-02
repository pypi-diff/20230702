# Comparing `tmp/sherpa-onnx-1.4.6.tar.gz` & `tmp/sherpa-onnx-1.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sherpa-onnx-1.4.6.tar", last modified: Tue Jun 27 10:32:03 2023, max compression
+gzip compressed data, was "sherpa-onnx-1.4.8.tar", last modified: Sun Jul  2 16:08:34 2023, max compression
```

## Comparing `sherpa-onnx-1.4.6.tar` & `sherpa-onnx-1.4.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:32:03.244605 sherpa-onnx-1.4.6/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-27 10:19:08.000000 sherpa-onnx-1.4.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-06-27 10:32:03.244605 sherpa-onnx-1.4.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-27 10:19:08.000000 sherpa-onnx-1.4.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 10:32:03.244605 sherpa-onnx-1.4.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-06-27 10:19:08.000000 sherpa-onnx-1.4.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:32:03.240605 sherpa-onnx-1.4.6/sherpa-onnx/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:32:03.240605 sherpa-onnx-1.4.6/sherpa-onnx/python/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:32:03.240605 sherpa-onnx-1.4.6/sherpa-onnx/python/sherpa_onnx/
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-06-27 10:32:03.000000 sherpa-onnx-1.4.6/sherpa-onnx/python/sherpa_onnx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7146 2023-06-27 10:19:08.000000 sherpa-onnx-1.4.6/sherpa-onnx/python/sherpa_onnx/offline_recognizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5267 2023-06-27 10:19:08.000000 sherpa-onnx-1.4.6/sherpa-onnx/python/sherpa_onnx/online_recognizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-06-27 10:19:08.000000 sherpa-onnx-1.4.6/sherpa-onnx/python/sherpa_onnx/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 10:32:03.244605 sherpa-onnx-1.4.6/sherpa_onnx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-06-27 10:32:03.000000 sherpa-onnx-1.4.6/sherpa_onnx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-06-27 10:32:03.000000 sherpa-onnx-1.4.6/sherpa_onnx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 10:32:03.000000 sherpa-onnx-1.4.6/sherpa_onnx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 10:32:03.000000 sherpa-onnx-1.4.6/sherpa_onnx.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-27 10:32:03.000000 sherpa-onnx-1.4.6/sherpa_onnx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-27 10:32:03.000000 sherpa-onnx-1.4.6/sherpa_onnx.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 16:08:34.421527 sherpa-onnx-1.4.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-02 15:57:43.000000 sherpa-onnx-1.4.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-02 16:08:34.421527 sherpa-onnx-1.4.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-02 15:57:43.000000 sherpa-onnx-1.4.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 16:08:34.421527 sherpa-onnx-1.4.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-07-02 15:57:43.000000 sherpa-onnx-1.4.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 16:08:34.421527 sherpa-onnx-1.4.8/sherpa-onnx/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 16:08:34.421527 sherpa-onnx-1.4.8/sherpa-onnx/python/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 16:08:34.421527 sherpa-onnx-1.4.8/sherpa-onnx/python/sherpa_onnx/
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-02 16:08:34.000000 sherpa-onnx-1.4.8/sherpa-onnx/python/sherpa_onnx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7146 2023-07-02 15:57:43.000000 sherpa-onnx-1.4.8/sherpa-onnx/python/sherpa_onnx/offline_recognizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5520 2023-07-02 15:57:43.000000 sherpa-onnx-1.4.8/sherpa-onnx/python/sherpa_onnx/online_recognizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-07-02 15:57:43.000000 sherpa-onnx-1.4.8/sherpa-onnx/python/sherpa_onnx/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 16:08:34.421527 sherpa-onnx-1.4.8/sherpa_onnx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-02 16:08:34.000000 sherpa-onnx-1.4.8/sherpa_onnx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-07-02 16:08:34.000000 sherpa-onnx-1.4.8/sherpa_onnx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 16:08:34.000000 sherpa-onnx-1.4.8/sherpa_onnx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 16:08:34.000000 sherpa-onnx-1.4.8/sherpa_onnx.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-02 16:08:34.000000 sherpa-onnx-1.4.8/sherpa_onnx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-02 16:08:34.000000 sherpa-onnx-1.4.8/sherpa_onnx.egg-info/top_level.txt
```

### Comparing `sherpa-onnx-1.4.6/LICENSE` & `sherpa-onnx-1.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.4.6/PKG-INFO` & `sherpa-onnx-1.4.8/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sherpa-onnx
-Version: 1.4.6
+Version: 1.4.8
 Summary: UNKNOWN
 Home-page: https://github.com/k2-fsa/sherpa-onnx
 Author: The sherpa-onnx development team
 Author-email: dpovey@gmail.com
 License: Apache licensed, as found in the LICENSE file
 Platform: UNKNOWN
 Classifier: Programming Language :: C++
```

### Comparing `sherpa-onnx-1.4.6/setup.py` & `sherpa-onnx-1.4.8/setup.py`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.4.6/sherpa-onnx/python/sherpa_onnx/offline_recognizer.py` & `sherpa-onnx-1.4.8/sherpa-onnx/python/sherpa_onnx/offline_recognizer.py`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.4.6/sherpa-onnx/python/sherpa_onnx/online_recognizer.py` & `sherpa-onnx-1.4.8/sherpa-onnx/python/sherpa_onnx/online_recognizer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Copyright (c)  2023  Xiaomi Corporation
 from pathlib import Path
-from typing import List
+from typing import List, Optional
 
 from _sherpa_onnx import (
     EndpointConfig,
     FeatureExtractorConfig,
     OnlineRecognizer as _Recognizer,
     OnlineRecognizerConfig,
     OnlineStream,
@@ -35,14 +35,15 @@
         feature_dim: int = 80,
         enable_endpoint_detection: bool = False,
         rule1_min_trailing_silence: float = 2.4,
         rule2_min_trailing_silence: float = 1.2,
         rule3_min_utterance_length: float = 20.0,
         decoding_method: str = "greedy_search",
         max_active_paths: int = 4,
+        context_score: float = 1.5,
         provider: str = "cpu",
     ):
         """
         Please refer to
         `<https://k2-fsa.github.io/sherpa/onnx/pretrained_models/index.html>`_
         to download pre-trained models for different languages, e.g., Chinese,
         English, etc.
@@ -120,21 +121,25 @@
         recognizer_config = OnlineRecognizerConfig(
             feat_config=feat_config,
             model_config=model_config,
             endpoint_config=endpoint_config,
             enable_endpoint=enable_endpoint_detection,
             decoding_method=decoding_method,
             max_active_paths=max_active_paths,
+            context_score=context_score,
         )
 
         self.recognizer = _Recognizer(recognizer_config)
         self.config = recognizer_config
 
-    def create_stream(self):
-        return self.recognizer.create_stream()
+    def create_stream(self, contexts_list : Optional[List[List[int]]] = None):
+        if contexts_list is None:
+            return self.recognizer.create_stream()
+        else:
+            return self.recognizer.create_stream(contexts_list)
 
     def decode_stream(self, s: OnlineStream):
         self.recognizer.decode_stream(s)
 
     def decode_streams(self, ss: List[OnlineStream]):
         self.recognizer.decode_streams(ss)
```

### Comparing `sherpa-onnx-1.4.6/sherpa-onnx/python/sherpa_onnx/utils.py` & `sherpa-onnx-1.4.8/sherpa-onnx/python/sherpa_onnx/utils.py`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.4.6/sherpa_onnx.egg-info/PKG-INFO` & `sherpa-onnx-1.4.8/sherpa_onnx.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sherpa-onnx
-Version: 1.4.6
+Version: 1.4.8
 Summary: UNKNOWN
 Home-page: https://github.com/k2-fsa/sherpa-onnx
 Author: The sherpa-onnx development team
 Author-email: dpovey@gmail.com
 License: Apache licensed, as found in the LICENSE file
 Platform: UNKNOWN
 Classifier: Programming Language :: C++
```

