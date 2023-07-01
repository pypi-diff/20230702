# Comparing `tmp/cjm-yolox-pytorch-0.0.4.tar.gz` & `tmp/cjm-yolox-pytorch-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cjm-yolox-pytorch-0.0.4.tar", last modified: Sat Jul  1 23:39:59 2023, max compression
+gzip compressed data, was "cjm-yolox-pytorch-0.0.5.tar", last modified: Sat Jul  1 23:42:52 2023, max compression
```

## Comparing `cjm-yolox-pytorch-0.0.4.tar` & `cjm-yolox-pytorch-0.0.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        0 2023-07-01 23:39:59.547224 cjm-yolox-pytorch-0.0.4/
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     1075 2023-06-22 23:01:16.000000 cjm-yolox-pytorch-0.0.4/LICENSE
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)      111 2023-04-27 10:12:58.000000 cjm-yolox-pytorch-0.0.4/MANIFEST.in
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     1815 2023-07-01 23:39:59.547054 cjm-yolox-pytorch-0.0.4/PKG-INFO
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     1050 2023-07-01 23:25:02.000000 cjm-yolox-pytorch-0.0.4/README.md
-drwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        0 2023-07-01 23:39:59.544317 cjm-yolox-pytorch-0.0.4/cjm_yolox_pytorch/
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       22 2023-07-01 23:39:41.000000 cjm-yolox-pytorch-0.0.4/cjm_yolox_pytorch/__init__.py
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)    13616 2023-07-01 23:39:41.000000 cjm-yolox-pytorch-0.0.4/cjm_yolox_pytorch/_modidx.py
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)    20864 2023-07-01 23:39:41.000000 cjm-yolox-pytorch-0.0.4/cjm_yolox_pytorch/loss.py
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)    44295 2023-07-01 23:39:41.000000 cjm-yolox-pytorch-0.0.4/cjm_yolox_pytorch/model.py
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)    15374 2023-07-01 23:39:41.000000 cjm-yolox-pytorch-0.0.4/cjm_yolox_pytorch/simota.py
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     2419 2023-07-01 23:39:41.000000 cjm-yolox-pytorch-0.0.4/cjm_yolox_pytorch/utils.py
-drwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        0 2023-07-01 23:39:59.546712 cjm-yolox-pytorch-0.0.4/cjm_yolox_pytorch.egg-info/
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     1815 2023-07-01 23:39:59.000000 cjm-yolox-pytorch-0.0.4/cjm_yolox_pytorch.egg-info/PKG-INFO
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)      506 2023-07-01 23:39:59.000000 cjm-yolox-pytorch-0.0.4/cjm_yolox_pytorch.egg-info/SOURCES.txt
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        1 2023-07-01 23:39:59.000000 cjm-yolox-pytorch-0.0.4/cjm_yolox_pytorch.egg-info/dependency_links.txt
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       56 2023-07-01 23:39:59.000000 cjm-yolox-pytorch-0.0.4/cjm_yolox_pytorch.egg-info/entry_points.txt
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        1 2023-06-23 01:14:13.000000 cjm-yolox-pytorch-0.0.4/cjm_yolox_pytorch.egg-info/not-zip-safe
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       31 2023-07-01 23:39:59.000000 cjm-yolox-pytorch-0.0.4/cjm_yolox_pytorch.egg-info/requires.txt
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       18 2023-07-01 23:39:59.000000 cjm-yolox-pytorch-0.0.4/cjm_yolox_pytorch.egg-info/top_level.txt
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     1052 2023-07-01 23:38:51.000000 cjm-yolox-pytorch-0.0.4/settings.ini
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       38 2023-07-01 23:39:59.547276 cjm-yolox-pytorch-0.0.4/setup.cfg
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     2596 2023-04-27 10:12:58.000000 cjm-yolox-pytorch-0.0.4/setup.py
+drwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        0 2023-07-01 23:42:52.412919 cjm-yolox-pytorch-0.0.5/
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     1075 2023-06-22 23:01:16.000000 cjm-yolox-pytorch-0.0.5/LICENSE
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)      111 2023-04-27 10:12:58.000000 cjm-yolox-pytorch-0.0.5/MANIFEST.in
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     1815 2023-07-01 23:42:52.412749 cjm-yolox-pytorch-0.0.5/PKG-INFO
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     1050 2023-07-01 23:25:02.000000 cjm-yolox-pytorch-0.0.5/README.md
+drwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        0 2023-07-01 23:42:52.409917 cjm-yolox-pytorch-0.0.5/cjm_yolox_pytorch/
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       22 2023-07-01 23:42:17.000000 cjm-yolox-pytorch-0.0.5/cjm_yolox_pytorch/__init__.py
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)    13616 2023-07-01 23:42:17.000000 cjm-yolox-pytorch-0.0.5/cjm_yolox_pytorch/_modidx.py
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)    20895 2023-07-01 23:42:17.000000 cjm-yolox-pytorch-0.0.5/cjm_yolox_pytorch/loss.py
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)    44295 2023-07-01 23:42:17.000000 cjm-yolox-pytorch-0.0.5/cjm_yolox_pytorch/model.py
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)    15405 2023-07-01 23:42:17.000000 cjm-yolox-pytorch-0.0.5/cjm_yolox_pytorch/simota.py
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     2419 2023-07-01 23:42:17.000000 cjm-yolox-pytorch-0.0.5/cjm_yolox_pytorch/utils.py
+drwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        0 2023-07-01 23:42:52.412250 cjm-yolox-pytorch-0.0.5/cjm_yolox_pytorch.egg-info/
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     1815 2023-07-01 23:42:52.000000 cjm-yolox-pytorch-0.0.5/cjm_yolox_pytorch.egg-info/PKG-INFO
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)      506 2023-07-01 23:42:52.000000 cjm-yolox-pytorch-0.0.5/cjm_yolox_pytorch.egg-info/SOURCES.txt
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        1 2023-07-01 23:42:52.000000 cjm-yolox-pytorch-0.0.5/cjm_yolox_pytorch.egg-info/dependency_links.txt
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       56 2023-07-01 23:42:52.000000 cjm-yolox-pytorch-0.0.5/cjm_yolox_pytorch.egg-info/entry_points.txt
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        1 2023-06-23 01:14:13.000000 cjm-yolox-pytorch-0.0.5/cjm_yolox_pytorch.egg-info/not-zip-safe
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       31 2023-07-01 23:42:52.000000 cjm-yolox-pytorch-0.0.5/cjm_yolox_pytorch.egg-info/requires.txt
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       18 2023-07-01 23:42:52.000000 cjm-yolox-pytorch-0.0.5/cjm_yolox_pytorch.egg-info/top_level.txt
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     1052 2023-07-01 23:42:12.000000 cjm-yolox-pytorch-0.0.5/settings.ini
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       38 2023-07-01 23:42:52.412970 cjm-yolox-pytorch-0.0.5/setup.cfg
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     2596 2023-04-27 10:12:58.000000 cjm-yolox-pytorch-0.0.5/setup.py
```

### Comparing `cjm-yolox-pytorch-0.0.4/LICENSE` & `cjm-yolox-pytorch-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cjm-yolox-pytorch-0.0.4/PKG-INFO` & `cjm-yolox-pytorch-0.0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cjm-yolox-pytorch
-Version: 0.0.4
+Version: 0.0.5
 Summary: A PyTorch implementation of the YOLOX object detection model based on the mmdetection implementation.
 Home-page: https://github.com/cj-mills/cjm-yolox-pytorch
 Author: cj-mills
 Author-email: millscj.mills2@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python torch
 Classifier: Development Status :: 4 - Beta
```

### Comparing `cjm-yolox-pytorch-0.0.4/README.md` & `cjm-yolox-pytorch-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `cjm-yolox-pytorch-0.0.4/cjm_yolox_pytorch/_modidx.py` & `cjm-yolox-pytorch-0.0.5/cjm_yolox_pytorch/_modidx.py`

 * *Files identical despite different names*

### Comparing `cjm-yolox-pytorch-0.0.4/cjm_yolox_pytorch/loss.py` & `cjm-yolox-pytorch-0.0.5/cjm_yolox_pytorch/loss.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from functools import partial
 
 # %% ../nbs/02_loss.ipynb 5
 import numpy as np
 
 import torch
 from torch.nn.modules.utils import _pair
-
+import torch.nn.functional as F
 import torchvision
 
 # %% ../nbs/02_loss.ipynb 6
 from .utils import multi_apply
 from .simota import SimOTAAssigner
 
 # %% ../nbs/02_loss.ipynb 8
```

### Comparing `cjm-yolox-pytorch-0.0.4/cjm_yolox_pytorch/model.py` & `cjm-yolox-pytorch-0.0.5/cjm_yolox_pytorch/model.py`

 * *Files identical despite different names*

### Comparing `cjm-yolox-pytorch-0.0.4/cjm_yolox_pytorch/simota.py` & `cjm-yolox-pytorch-0.0.5/cjm_yolox_pytorch/simota.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 # %% ../nbs/03_simota.ipynb 4
 from typing import Any, Type, List, Optional, Callable, Tuple, Union
 from functools import partial
 
 # %% ../nbs/03_simota.ipynb 5
 import torch
-
+import torch.nn.functional as F
 import torchvision
 
 # %% ../nbs/03_simota.ipynb 7
 class AssignResult():
     """
     Stores assignments between predicted bounding boxes and actual truth bounding boxes.
```

### Comparing `cjm-yolox-pytorch-0.0.4/cjm_yolox_pytorch/utils.py` & `cjm-yolox-pytorch-0.0.5/cjm_yolox_pytorch/utils.py`

 * *Files identical despite different names*

### Comparing `cjm-yolox-pytorch-0.0.4/cjm_yolox_pytorch.egg-info/PKG-INFO` & `cjm-yolox-pytorch-0.0.5/cjm_yolox_pytorch.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cjm-yolox-pytorch
-Version: 0.0.4
+Version: 0.0.5
 Summary: A PyTorch implementation of the YOLOX object detection model based on the mmdetection implementation.
 Home-page: https://github.com/cj-mills/cjm-yolox-pytorch
 Author: cj-mills
 Author-email: millscj.mills2@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python torch
 Classifier: Development Status :: 4 - Beta
```

### Comparing `cjm-yolox-pytorch-0.0.4/settings.ini` & `cjm-yolox-pytorch-0.0.5/settings.ini`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = cjm-yolox-pytorch
 lib_name = %(repo)s
-version = 0.0.4
+version = 0.0.5
 min_python = 3.9
 license = apache2
 black_formatting = False
 
 ### nbdev ###
 doc_path = _docs
 lib_path = cjm_yolox_pytorch
```

### Comparing `cjm-yolox-pytorch-0.0.4/setup.py` & `cjm-yolox-pytorch-0.0.5/setup.py`

 * *Files identical despite different names*

