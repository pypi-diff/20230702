# Comparing `tmp/cjm-yolox-pytorch-0.0.1.tar.gz` & `tmp/cjm-yolox-pytorch-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cjm-yolox-pytorch-0.0.1.tar", last modified: Fri Jun 30 22:10:39 2023, max compression
+gzip compressed data, was "cjm-yolox-pytorch-0.0.2.tar", last modified: Sat Jul  1 23:33:36 2023, max compression
```

## Comparing `cjm-yolox-pytorch-0.0.1.tar` & `cjm-yolox-pytorch-0.0.2.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        0 2023-06-30 22:10:39.544851 cjm-yolox-pytorch-0.0.1/
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     1075 2023-06-22 23:01:16.000000 cjm-yolox-pytorch-0.0.1/LICENSE
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)      111 2023-04-27 10:12:58.000000 cjm-yolox-pytorch-0.0.1/MANIFEST.in
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     1815 2023-06-30 22:10:39.544675 cjm-yolox-pytorch-0.0.1/PKG-INFO
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     1050 2023-06-30 22:02:24.000000 cjm-yolox-pytorch-0.0.1/README.md
-drwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        0 2023-06-30 22:10:39.542099 cjm-yolox-pytorch-0.0.1/cjm_yolox_pytorch/
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       22 2023-06-30 22:04:55.000000 cjm-yolox-pytorch-0.0.1/cjm_yolox_pytorch/__init__.py
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     8156 2023-06-30 22:04:55.000000 cjm-yolox-pytorch-0.0.1/cjm_yolox_pytorch/_modidx.py
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)    44295 2023-06-30 22:04:55.000000 cjm-yolox-pytorch-0.0.1/cjm_yolox_pytorch/model.py
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     2397 2023-06-30 22:04:55.000000 cjm-yolox-pytorch-0.0.1/cjm_yolox_pytorch/utils.py
-drwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        0 2023-06-30 22:10:39.544315 cjm-yolox-pytorch-0.0.1/cjm_yolox_pytorch.egg-info/
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     1815 2023-06-30 22:10:39.000000 cjm-yolox-pytorch-0.0.1/cjm_yolox_pytorch.egg-info/PKG-INFO
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)      452 2023-06-30 22:10:39.000000 cjm-yolox-pytorch-0.0.1/cjm_yolox_pytorch.egg-info/SOURCES.txt
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        1 2023-06-30 22:10:39.000000 cjm-yolox-pytorch-0.0.1/cjm_yolox_pytorch.egg-info/dependency_links.txt
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       56 2023-06-30 22:10:39.000000 cjm-yolox-pytorch-0.0.1/cjm_yolox_pytorch.egg-info/entry_points.txt
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        1 2023-06-23 01:14:13.000000 cjm-yolox-pytorch-0.0.1/cjm_yolox_pytorch.egg-info/not-zip-safe
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       13 2023-06-30 22:10:39.000000 cjm-yolox-pytorch-0.0.1/cjm_yolox_pytorch.egg-info/requires.txt
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       18 2023-06-30 22:10:39.000000 cjm-yolox-pytorch-0.0.1/cjm_yolox_pytorch.egg-info/top_level.txt
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     1034 2023-06-30 22:04:51.000000 cjm-yolox-pytorch-0.0.1/settings.ini
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       38 2023-06-30 22:10:39.544904 cjm-yolox-pytorch-0.0.1/setup.cfg
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     2596 2023-04-27 10:12:58.000000 cjm-yolox-pytorch-0.0.1/setup.py
+drwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        0 2023-07-01 23:33:36.577867 cjm-yolox-pytorch-0.0.2/
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     1075 2023-06-22 23:01:16.000000 cjm-yolox-pytorch-0.0.2/LICENSE
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)      111 2023-04-27 10:12:58.000000 cjm-yolox-pytorch-0.0.2/MANIFEST.in
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     1815 2023-07-01 23:33:36.577704 cjm-yolox-pytorch-0.0.2/PKG-INFO
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     1050 2023-07-01 23:25:02.000000 cjm-yolox-pytorch-0.0.2/README.md
+drwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        0 2023-07-01 23:33:36.575177 cjm-yolox-pytorch-0.0.2/cjm_yolox_pytorch/
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       22 2023-07-01 23:33:00.000000 cjm-yolox-pytorch-0.0.2/cjm_yolox_pytorch/__init__.py
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)    13616 2023-07-01 23:33:00.000000 cjm-yolox-pytorch-0.0.2/cjm_yolox_pytorch/_modidx.py
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)    20844 2023-07-01 23:33:00.000000 cjm-yolox-pytorch-0.0.2/cjm_yolox_pytorch/loss.py
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)    44295 2023-07-01 23:33:00.000000 cjm-yolox-pytorch-0.0.2/cjm_yolox_pytorch/model.py
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)    15354 2023-07-01 23:33:00.000000 cjm-yolox-pytorch-0.0.2/cjm_yolox_pytorch/simota.py
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     2419 2023-07-01 23:33:00.000000 cjm-yolox-pytorch-0.0.2/cjm_yolox_pytorch/utils.py
+drwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        0 2023-07-01 23:33:36.577298 cjm-yolox-pytorch-0.0.2/cjm_yolox_pytorch.egg-info/
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     1815 2023-07-01 23:33:36.000000 cjm-yolox-pytorch-0.0.2/cjm_yolox_pytorch.egg-info/PKG-INFO
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)      506 2023-07-01 23:33:36.000000 cjm-yolox-pytorch-0.0.2/cjm_yolox_pytorch.egg-info/SOURCES.txt
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        1 2023-07-01 23:33:36.000000 cjm-yolox-pytorch-0.0.2/cjm_yolox_pytorch.egg-info/dependency_links.txt
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       56 2023-07-01 23:33:36.000000 cjm-yolox-pytorch-0.0.2/cjm_yolox_pytorch.egg-info/entry_points.txt
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        1 2023-06-23 01:14:13.000000 cjm-yolox-pytorch-0.0.2/cjm_yolox_pytorch.egg-info/not-zip-safe
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       19 2023-07-01 23:33:36.000000 cjm-yolox-pytorch-0.0.2/cjm_yolox_pytorch.egg-info/requires.txt
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       18 2023-07-01 23:33:36.000000 cjm-yolox-pytorch-0.0.2/cjm_yolox_pytorch.egg-info/top_level.txt
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     1040 2023-07-01 23:32:51.000000 cjm-yolox-pytorch-0.0.2/settings.ini
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       38 2023-07-01 23:33:36.577916 cjm-yolox-pytorch-0.0.2/setup.cfg
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     2596 2023-04-27 10:12:58.000000 cjm-yolox-pytorch-0.0.2/setup.py
```

### Comparing `cjm-yolox-pytorch-0.0.1/LICENSE` & `cjm-yolox-pytorch-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cjm-yolox-pytorch-0.0.1/PKG-INFO` & `cjm-yolox-pytorch-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cjm-yolox-pytorch
-Version: 0.0.1
+Version: 0.0.2
 Summary: A PyTorch implementation of the YOLOX object detection model based on the mmdetection implementation.
 Home-page: https://github.com/cj-mills/cjm-yolox-pytorch
 Author: cj-mills
 Author-email: millscj.mills2@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python torch
 Classifier: Development Status :: 4 - Beta
```

### Comparing `cjm-yolox-pytorch-0.0.1/README.md` & `cjm-yolox-pytorch-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `cjm-yolox-pytorch-0.0.1/cjm_yolox_pytorch/model.py` & `cjm-yolox-pytorch-0.0.2/cjm_yolox_pytorch/model.py`

 * *Files identical despite different names*

### Comparing `cjm-yolox-pytorch-0.0.1/cjm_yolox_pytorch/utils.py` & `cjm-yolox-pytorch-0.0.2/cjm_yolox_pytorch/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,26 +8,25 @@
 
 from typing import Any, Type, List, Optional, Callable, Tuple
 from functools import partial
 
 import urllib.request
 
 # %% ../nbs/01_utils.ipynb 6
-# Based on:
-# https://github.com/open-mmlab/mmdetection/blob/d64e719172335fa3d7a757a2a3636bd19e9efb62/mmdet/core/utils/misc.py#L11
-
-def multi_apply(func: Callable[..., Any], # Function to apply.
-                *args: Any, # Variable length argument list.
-                **kwargs: Any # Arbitrary keyword arguments.
+def multi_apply(func:Callable[..., Any], # Function to apply.
+                *args:Any,
+                **kwargs:Any
                ) -> Tuple[List[Any], ...]:
     """
     Applies the function `func` to each set of arguments in `*args`, 
     possibly using keyword arguments `**kwargs`.
     
+    Based on OpenMMLab's implementation in the mmdetection library:
     
+    - [OpenMMLab's Implementation](https://github.com/open-mmlab/mmdetection/blob/d64e719172335fa3d7a757a2a3636bd19e9efb62/mmdet/core/utils/misc.py#L11)
 
     """
     try:
         pfunc = partial(func, **kwargs) if kwargs else func
         map_results = map(pfunc, *args)
         return tuple(map(list, zip(*map_results)))
     except Exception as e:
```

### Comparing `cjm-yolox-pytorch-0.0.1/cjm_yolox_pytorch.egg-info/PKG-INFO` & `cjm-yolox-pytorch-0.0.2/cjm_yolox_pytorch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cjm-yolox-pytorch
-Version: 0.0.1
+Version: 0.0.2
 Summary: A PyTorch implementation of the YOLOX object detection model based on the mmdetection implementation.
 Home-page: https://github.com/cj-mills/cjm-yolox-pytorch
 Author: cj-mills
 Author-email: millscj.mills2@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python torch
 Classifier: Development Status :: 4 - Beta
```

### Comparing `cjm-yolox-pytorch-0.0.1/settings.ini` & `cjm-yolox-pytorch-0.0.2/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = cjm-yolox-pytorch
 lib_name = %(repo)s
-version = 0.0.1
+version = 0.0.2
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
-requirements = torch
+requirements = torch numpy
 # dev_requirements = 
 # console_scripts =
```

### Comparing `cjm-yolox-pytorch-0.0.1/setup.py` & `cjm-yolox-pytorch-0.0.2/setup.py`

 * *Files identical despite different names*

