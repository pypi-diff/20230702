# Comparing `tmp/cjm-yolox-pytorch-0.0.2.tar.gz` & `tmp/cjm-yolox-pytorch-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cjm-yolox-pytorch-0.0.2.tar", last modified: Sat Jul  1 23:33:36 2023, max compression
+gzip compressed data, was "cjm-yolox-pytorch-0.0.3.tar", last modified: Sat Jul  1 23:37:09 2023, max compression
```

## Comparing `cjm-yolox-pytorch-0.0.2.tar` & `cjm-yolox-pytorch-0.0.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        0 2023-07-01 23:33:36.577867 cjm-yolox-pytorch-0.0.2/
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     1075 2023-06-22 23:01:16.000000 cjm-yolox-pytorch-0.0.2/LICENSE
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)      111 2023-04-27 10:12:58.000000 cjm-yolox-pytorch-0.0.2/MANIFEST.in
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     1815 2023-07-01 23:33:36.577704 cjm-yolox-pytorch-0.0.2/PKG-INFO
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     1050 2023-07-01 23:25:02.000000 cjm-yolox-pytorch-0.0.2/README.md
-drwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        0 2023-07-01 23:33:36.575177 cjm-yolox-pytorch-0.0.2/cjm_yolox_pytorch/
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       22 2023-07-01 23:33:00.000000 cjm-yolox-pytorch-0.0.2/cjm_yolox_pytorch/__init__.py
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)    13616 2023-07-01 23:33:00.000000 cjm-yolox-pytorch-0.0.2/cjm_yolox_pytorch/_modidx.py
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)    20844 2023-07-01 23:33:00.000000 cjm-yolox-pytorch-0.0.2/cjm_yolox_pytorch/loss.py
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)    44295 2023-07-01 23:33:00.000000 cjm-yolox-pytorch-0.0.2/cjm_yolox_pytorch/model.py
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)    15354 2023-07-01 23:33:00.000000 cjm-yolox-pytorch-0.0.2/cjm_yolox_pytorch/simota.py
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     2419 2023-07-01 23:33:00.000000 cjm-yolox-pytorch-0.0.2/cjm_yolox_pytorch/utils.py
-drwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        0 2023-07-01 23:33:36.577298 cjm-yolox-pytorch-0.0.2/cjm_yolox_pytorch.egg-info/
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     1815 2023-07-01 23:33:36.000000 cjm-yolox-pytorch-0.0.2/cjm_yolox_pytorch.egg-info/PKG-INFO
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)      506 2023-07-01 23:33:36.000000 cjm-yolox-pytorch-0.0.2/cjm_yolox_pytorch.egg-info/SOURCES.txt
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        1 2023-07-01 23:33:36.000000 cjm-yolox-pytorch-0.0.2/cjm_yolox_pytorch.egg-info/dependency_links.txt
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       56 2023-07-01 23:33:36.000000 cjm-yolox-pytorch-0.0.2/cjm_yolox_pytorch.egg-info/entry_points.txt
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        1 2023-06-23 01:14:13.000000 cjm-yolox-pytorch-0.0.2/cjm_yolox_pytorch.egg-info/not-zip-safe
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       19 2023-07-01 23:33:36.000000 cjm-yolox-pytorch-0.0.2/cjm_yolox_pytorch.egg-info/requires.txt
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       18 2023-07-01 23:33:36.000000 cjm-yolox-pytorch-0.0.2/cjm_yolox_pytorch.egg-info/top_level.txt
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     1040 2023-07-01 23:32:51.000000 cjm-yolox-pytorch-0.0.2/settings.ini
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       38 2023-07-01 23:33:36.577916 cjm-yolox-pytorch-0.0.2/setup.cfg
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     2596 2023-04-27 10:12:58.000000 cjm-yolox-pytorch-0.0.2/setup.py
+drwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        0 2023-07-01 23:37:09.318257 cjm-yolox-pytorch-0.0.3/
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     1075 2023-06-22 23:01:16.000000 cjm-yolox-pytorch-0.0.3/LICENSE
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)      111 2023-04-27 10:12:58.000000 cjm-yolox-pytorch-0.0.3/MANIFEST.in
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     1815 2023-07-01 23:37:09.318083 cjm-yolox-pytorch-0.0.3/PKG-INFO
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     1050 2023-07-01 23:25:02.000000 cjm-yolox-pytorch-0.0.3/README.md
+drwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        0 2023-07-01 23:37:09.315261 cjm-yolox-pytorch-0.0.3/cjm_yolox_pytorch/
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       22 2023-07-01 23:36:38.000000 cjm-yolox-pytorch-0.0.3/cjm_yolox_pytorch/__init__.py
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)    13616 2023-07-01 23:36:38.000000 cjm-yolox-pytorch-0.0.3/cjm_yolox_pytorch/_modidx.py
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)    20864 2023-07-01 23:36:38.000000 cjm-yolox-pytorch-0.0.3/cjm_yolox_pytorch/loss.py
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)    44295 2023-07-01 23:36:38.000000 cjm-yolox-pytorch-0.0.3/cjm_yolox_pytorch/model.py
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)    15354 2023-07-01 23:36:38.000000 cjm-yolox-pytorch-0.0.3/cjm_yolox_pytorch/simota.py
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     2419 2023-07-01 23:36:38.000000 cjm-yolox-pytorch-0.0.3/cjm_yolox_pytorch/utils.py
+drwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        0 2023-07-01 23:37:09.317752 cjm-yolox-pytorch-0.0.3/cjm_yolox_pytorch.egg-info/
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     1815 2023-07-01 23:37:09.000000 cjm-yolox-pytorch-0.0.3/cjm_yolox_pytorch.egg-info/PKG-INFO
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)      506 2023-07-01 23:37:09.000000 cjm-yolox-pytorch-0.0.3/cjm_yolox_pytorch.egg-info/SOURCES.txt
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        1 2023-07-01 23:37:09.000000 cjm-yolox-pytorch-0.0.3/cjm_yolox_pytorch.egg-info/dependency_links.txt
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       56 2023-07-01 23:37:09.000000 cjm-yolox-pytorch-0.0.3/cjm_yolox_pytorch.egg-info/entry_points.txt
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        1 2023-06-23 01:14:13.000000 cjm-yolox-pytorch-0.0.3/cjm_yolox_pytorch.egg-info/not-zip-safe
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       31 2023-07-01 23:37:09.000000 cjm-yolox-pytorch-0.0.3/cjm_yolox_pytorch.egg-info/requires.txt
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       18 2023-07-01 23:37:09.000000 cjm-yolox-pytorch-0.0.3/cjm_yolox_pytorch.egg-info/top_level.txt
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     1052 2023-07-01 23:36:06.000000 cjm-yolox-pytorch-0.0.3/settings.ini
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       38 2023-07-01 23:37:09.318307 cjm-yolox-pytorch-0.0.3/setup.cfg
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     2596 2023-04-27 10:12:58.000000 cjm-yolox-pytorch-0.0.3/setup.py
```

### Comparing `cjm-yolox-pytorch-0.0.2/LICENSE` & `cjm-yolox-pytorch-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cjm-yolox-pytorch-0.0.2/PKG-INFO` & `cjm-yolox-pytorch-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cjm-yolox-pytorch
-Version: 0.0.2
+Version: 0.0.3
 Summary: A PyTorch implementation of the YOLOX object detection model based on the mmdetection implementation.
 Home-page: https://github.com/cj-mills/cjm-yolox-pytorch
 Author: cj-mills
 Author-email: millscj.mills2@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python torch
 Classifier: Development Status :: 4 - Beta
```

### Comparing `cjm-yolox-pytorch-0.0.2/README.md` & `cjm-yolox-pytorch-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `cjm-yolox-pytorch-0.0.2/cjm_yolox_pytorch/_modidx.py` & `cjm-yolox-pytorch-0.0.3/cjm_yolox_pytorch/_modidx.py`

 * *Files identical despite different names*

### Comparing `cjm-yolox-pytorch-0.0.2/cjm_yolox_pytorch/loss.py` & `cjm-yolox-pytorch-0.0.3/cjm_yolox_pytorch/loss.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 
 # %% ../nbs/02_loss.ipynb 5
 import numpy as np
 
 import torch
 from torch.nn.modules.utils import _pair
 
+import torchvision
+
 # %% ../nbs/02_loss.ipynb 6
 from .utils import multi_apply
 from .simota import SimOTAAssigner
 
 # %% ../nbs/02_loss.ipynb 8
 class MlvlPointGenerator:
     """Standard points generator for multi-level (Mlvl) feature maps in 2D points-based detectors.
```

### Comparing `cjm-yolox-pytorch-0.0.2/cjm_yolox_pytorch/model.py` & `cjm-yolox-pytorch-0.0.3/cjm_yolox_pytorch/model.py`

 * *Files identical despite different names*

### Comparing `cjm-yolox-pytorch-0.0.2/cjm_yolox_pytorch/simota.py` & `cjm-yolox-pytorch-0.0.3/cjm_yolox_pytorch/simota.py`

 * *Files identical despite different names*

### Comparing `cjm-yolox-pytorch-0.0.2/cjm_yolox_pytorch/utils.py` & `cjm-yolox-pytorch-0.0.3/cjm_yolox_pytorch/utils.py`

 * *Files identical despite different names*

### Comparing `cjm-yolox-pytorch-0.0.2/cjm_yolox_pytorch.egg-info/PKG-INFO` & `cjm-yolox-pytorch-0.0.3/cjm_yolox_pytorch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cjm-yolox-pytorch
-Version: 0.0.2
+Version: 0.0.3
 Summary: A PyTorch implementation of the YOLOX object detection model based on the mmdetection implementation.
 Home-page: https://github.com/cj-mills/cjm-yolox-pytorch
 Author: cj-mills
 Author-email: millscj.mills2@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python torch
 Classifier: Development Status :: 4 - Beta
```

### Comparing `cjm-yolox-pytorch-0.0.2/settings.ini` & `cjm-yolox-pytorch-0.0.3/settings.ini`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = cjm-yolox-pytorch
 lib_name = %(repo)s
-version = 0.0.2
+version = 0.0.3
 min_python = 3.9
 license = apache2
 black_formatting = False
 
 ### nbdev ###
 doc_path = _docs
 lib_path = cjm_yolox_pytorch
@@ -34,10 +34,10 @@
 description = A PyTorch implementation of the YOLOX object detection model based on the mmdetection implementation.
 keywords = nbdev jupyter notebook python torch
 language = English
 status = 3
 user = cj-mills
 
 ### Optional ###
-requirements = torch numpy
+requirements = torch numpy torchvision
 # dev_requirements = 
 # console_scripts =
```

### Comparing `cjm-yolox-pytorch-0.0.2/setup.py` & `cjm-yolox-pytorch-0.0.3/setup.py`

 * *Files identical despite different names*

