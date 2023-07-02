# Comparing `tmp/tvdcn-0.3.0.tar.gz` & `tmp/tvdcn-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tvdcn-0.3.0.tar", last modified: Fri Jun 30 15:54:22 2023, max compression
+gzip compressed data, was "tvdcn-0.3.1.tar", last modified: Sun Jul  2 06:53:12 2023, max compression
```

## Comparing `tvdcn-0.3.0.tar` & `tvdcn-0.3.1.tar`

### file list

```diff
@@ -1,54 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:54:22.044675 tvdcn-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-30 15:52:27.000000 tvdcn-0.3.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-30 15:52:27.000000 tvdcn-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8967 2023-06-30 15:54:22.044675 tvdcn-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7686 2023-06-30 15:52:27.000000 tvdcn-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-06-30 15:52:27.000000 tvdcn-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-30 15:52:27.000000 tvdcn-0.3.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-06-30 15:54:22.048675 tvdcn-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-06-30 15:52:27.000000 tvdcn-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:54:22.032675 tvdcn-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-06-30 15:52:27.000000 tvdcn-0.3.0/tests/test_compatibility_with_torchvision.py
--rw-r--r--   0 runner    (1001) docker     (123)     3199 2023-06-30 15:52:27.000000 tvdcn-0.3.0/tests/test_grad.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:54:22.032675 tvdcn-0.3.0/tvdcn/
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-30 15:52:27.000000 tvdcn-0.3.0/tvdcn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-30 15:52:27.000000 tvdcn-0.3.0/tvdcn/_types.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-30 15:52:27.000000 tvdcn-0.3.0/tvdcn/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:54:22.036675 tvdcn-0.3.0/tvdcn/csrc/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:54:22.036675 tvdcn-0.3.0/tvdcn/csrc/ops/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:54:22.040675 tvdcn-0.3.0/tvdcn/csrc/ops/cpu/
--rw-r--r--   0 runner    (1001) docker     (123)    20248 2023-06-30 15:52:27.000000 tvdcn-0.3.0/tvdcn/csrc/ops/cpu/deform_conv1d_kernels_cpu.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    27047 2023-06-30 15:52:27.000000 tvdcn-0.3.0/tvdcn/csrc/ops/cpu/deform_conv2d_kernels_cpu.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    35454 2023-06-30 15:52:27.000000 tvdcn-0.3.0/tvdcn/csrc/ops/cpu/deform_conv3d_kernels_cpu.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:54:22.040675 tvdcn-0.3.0/tvdcn/csrc/ops/cuda/
--rw-r--r--   0 runner    (1001) docker     (123)    23346 2023-06-30 15:52:27.000000 tvdcn-0.3.0/tvdcn/csrc/ops/cuda/deform_conv1d_kernels_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (123)    30172 2023-06-30 15:52:27.000000 tvdcn-0.3.0/tvdcn/csrc/ops/cuda/deform_conv2d_kernels_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (123)    38630 2023-06-30 15:52:27.000000 tvdcn-0.3.0/tvdcn/csrc/ops/cuda/deform_conv3d_kernels_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (123)    26844 2023-06-30 15:52:27.000000 tvdcn-0.3.0/tvdcn/csrc/ops/deform_conv1d.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    30614 2023-06-30 15:52:27.000000 tvdcn-0.3.0/tvdcn/csrc/ops/deform_conv2d.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    34378 2023-06-30 15:52:27.000000 tvdcn-0.3.0/tvdcn/csrc/ops/deform_conv3d.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    27619 2023-06-30 15:52:27.000000 tvdcn-0.3.0/tvdcn/csrc/ops/deform_conv_transpose1d.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    31385 2023-06-30 15:52:27.000000 tvdcn-0.3.0/tvdcn/csrc/ops/deform_conv_transpose2d.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    35145 2023-06-30 15:52:27.000000 tvdcn-0.3.0/tvdcn/csrc/ops/deform_conv_transpose3d.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:54:22.044675 tvdcn-0.3.0/tvdcn/csrc/ops/dispatch/
--rw-r--r--   0 runner    (1001) docker     (123)    10352 2023-06-30 15:52:27.000000 tvdcn-0.3.0/tvdcn/csrc/ops/dispatch/deform_conv1d_kernels.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    13592 2023-06-30 15:52:27.000000 tvdcn-0.3.0/tvdcn/csrc/ops/dispatch/deform_conv2d_kernels.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    17006 2023-06-30 15:52:27.000000 tvdcn-0.3.0/tvdcn/csrc/ops/dispatch/deform_conv3d_kernels.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-06-30 15:52:27.000000 tvdcn-0.3.0/tvdcn/csrc/tvdcn.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5237 2023-06-30 15:52:27.000000 tvdcn-0.3.0/tvdcn/extension.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:54:22.044675 tvdcn-0.3.0/tvdcn/ops/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-30 15:52:27.000000 tvdcn-0.3.0/tvdcn/ops/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:54:22.044675 tvdcn-0.3.0/tvdcn/ops/activations/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-30 15:52:27.000000 tvdcn-0.3.0/tvdcn/ops/activations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-06-30 15:52:27.000000 tvdcn-0.3.0/tvdcn/ops/activations/mask_sigmoid.py
--rw-r--r--   0 runner    (1001) docker     (123)     6324 2023-06-30 15:52:27.000000 tvdcn-0.3.0/tvdcn/ops/activations/mask_softmax.py
--rw-r--r--   0 runner    (1001) docker     (123)    31021 2023-06-30 15:52:27.000000 tvdcn-0.3.0/tvdcn/ops/deform_conv.py
--rw-r--r--   0 runner    (1001) docker     (123)    34045 2023-06-30 15:52:27.000000 tvdcn-0.3.0/tvdcn/ops/deform_conv_transpose.py
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-06-30 15:52:27.000000 tvdcn-0.3.0/tvdcn/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:54:22.036675 tvdcn-0.3.0/tvdcn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8967 2023-06-30 15:54:22.000000 tvdcn-0.3.0/tvdcn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-06-30 15:54:22.000000 tvdcn-0.3.0/tvdcn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 15:54:22.000000 tvdcn-0.3.0/tvdcn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 15:54:22.000000 tvdcn-0.3.0/tvdcn.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-30 15:54:22.000000 tvdcn-0.3.0/tvdcn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-30 15:54:22.000000 tvdcn-0.3.0/tvdcn.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 06:53:12.559211 tvdcn-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-02 06:51:20.000000 tvdcn-0.3.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-02 06:51:20.000000 tvdcn-0.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8967 2023-07-02 06:53:12.559211 tvdcn-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7686 2023-07-02 06:51:20.000000 tvdcn-0.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-07-02 06:51:20.000000 tvdcn-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-02 06:51:20.000000 tvdcn-0.3.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-07-02 06:53:12.559211 tvdcn-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3673 2023-07-02 06:51:20.000000 tvdcn-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 06:53:12.547211 tvdcn-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-07-02 06:51:20.000000 tvdcn-0.3.1/tests/test_compatibility_with_torchvision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3199 2023-07-02 06:51:20.000000 tvdcn-0.3.1/tests/test_grad.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 06:53:12.547211 tvdcn-0.3.1/tvdcn/
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-02 06:51:20.000000 tvdcn-0.3.1/tvdcn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-02 06:51:20.000000 tvdcn-0.3.1/tvdcn/_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-02 06:51:20.000000 tvdcn-0.3.1/tvdcn/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 06:53:12.551211 tvdcn-0.3.1/tvdcn/csrc/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 06:53:12.551211 tvdcn-0.3.1/tvdcn/csrc/ops/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 06:53:12.555211 tvdcn-0.3.1/tvdcn/csrc/ops/cpu/
+-rw-r--r--   0 runner    (1001) docker     (123)    20248 2023-07-02 06:51:20.000000 tvdcn-0.3.1/tvdcn/csrc/ops/cpu/deform_conv1d_kernels_cpu.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    27047 2023-07-02 06:51:20.000000 tvdcn-0.3.1/tvdcn/csrc/ops/cpu/deform_conv2d_kernels_cpu.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    35454 2023-07-02 06:51:20.000000 tvdcn-0.3.1/tvdcn/csrc/ops/cpu/deform_conv3d_kernels_cpu.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 06:53:12.555211 tvdcn-0.3.1/tvdcn/csrc/ops/cuda/
+-rw-r--r--   0 runner    (1001) docker     (123)    23346 2023-07-02 06:51:20.000000 tvdcn-0.3.1/tvdcn/csrc/ops/cuda/deform_conv1d_kernels_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (123)    30172 2023-07-02 06:51:20.000000 tvdcn-0.3.1/tvdcn/csrc/ops/cuda/deform_conv2d_kernels_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (123)    38630 2023-07-02 06:51:20.000000 tvdcn-0.3.1/tvdcn/csrc/ops/cuda/deform_conv3d_kernels_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (123)    26564 2023-07-02 06:51:20.000000 tvdcn-0.3.1/tvdcn/csrc/ops/deform_conv1d.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    30412 2023-07-02 06:51:20.000000 tvdcn-0.3.1/tvdcn/csrc/ops/deform_conv2d.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    34230 2023-07-02 06:51:20.000000 tvdcn-0.3.1/tvdcn/csrc/ops/deform_conv3d.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    27339 2023-07-02 06:51:20.000000 tvdcn-0.3.1/tvdcn/csrc/ops/deform_conv_transpose1d.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    31183 2023-07-02 06:51:20.000000 tvdcn-0.3.1/tvdcn/csrc/ops/deform_conv_transpose2d.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    34997 2023-07-02 06:51:20.000000 tvdcn-0.3.1/tvdcn/csrc/ops/deform_conv_transpose3d.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 06:53:12.555211 tvdcn-0.3.1/tvdcn/csrc/ops/dispatch/
+-rw-r--r--   0 runner    (1001) docker     (123)    10352 2023-07-02 06:51:20.000000 tvdcn-0.3.1/tvdcn/csrc/ops/dispatch/deform_conv1d_kernels.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    13592 2023-07-02 06:51:20.000000 tvdcn-0.3.1/tvdcn/csrc/ops/dispatch/deform_conv2d_kernels.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    17006 2023-07-02 06:51:20.000000 tvdcn-0.3.1/tvdcn/csrc/ops/dispatch/deform_conv3d_kernels.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 06:53:12.555211 tvdcn-0.3.1/tvdcn/csrc/ops/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-07-02 06:51:20.000000 tvdcn-0.3.1/tvdcn/csrc/ops/utils/tensor_utils.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-07-02 06:51:20.000000 tvdcn-0.3.1/tvdcn/csrc/tvdcn.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5237 2023-07-02 06:51:20.000000 tvdcn-0.3.1/tvdcn/extension.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 06:53:12.559211 tvdcn-0.3.1/tvdcn/ops/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-02 06:51:20.000000 tvdcn-0.3.1/tvdcn/ops/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 06:53:12.559211 tvdcn-0.3.1/tvdcn/ops/activations/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-02 06:51:20.000000 tvdcn-0.3.1/tvdcn/ops/activations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-02 06:51:20.000000 tvdcn-0.3.1/tvdcn/ops/activations/mask_sigmoid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6324 2023-07-02 06:51:20.000000 tvdcn-0.3.1/tvdcn/ops/activations/mask_softmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30949 2023-07-02 06:51:20.000000 tvdcn-0.3.1/tvdcn/ops/deform_conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33943 2023-07-02 06:51:20.000000 tvdcn-0.3.1/tvdcn/ops/deform_conv_transpose.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-07-02 06:51:20.000000 tvdcn-0.3.1/tvdcn/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 06:53:12.551211 tvdcn-0.3.1/tvdcn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8967 2023-07-02 06:53:12.000000 tvdcn-0.3.1/tvdcn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-07-02 06:53:12.000000 tvdcn-0.3.1/tvdcn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 06:53:12.000000 tvdcn-0.3.1/tvdcn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 06:53:12.000000 tvdcn-0.3.1/tvdcn.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-02 06:53:12.000000 tvdcn-0.3.1/tvdcn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-02 06:53:12.000000 tvdcn-0.3.1/tvdcn.egg-info/top_level.txt
```

### Comparing `tvdcn-0.3.0/LICENSE.txt` & `tvdcn-0.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tvdcn-0.3.0/PKG-INFO` & `tvdcn-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tvdcn
-Version: 0.3.0
+Version: 0.3.1
 Summary: Torchvision+ Deformable Convolutional Networks
 Home-page: https://github.com/inspiros/tvdcn
 Author: Hoang-Nhat Tran (inspiros)
 Author-email: hnhat.tran@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/inspiros/tvdcn
 Keywords: deform_conv; deformable convolution
```

### Comparing `tvdcn-0.3.0/README.md` & `tvdcn-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `tvdcn-0.3.0/pyproject.toml` & `tvdcn-0.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tvdcn-0.3.0/setup.cfg` & `tvdcn-0.3.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `tvdcn-0.3.0/setup.py` & `tvdcn-0.3.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,15 +29,16 @@
     main_file = (glob.glob(os.path.join(extensions_dir, '*.cpp')) +
                  glob.glob(os.path.join(extensions_dir, 'ops', '*.cpp'))
                  )
 
     source_cpu = (glob.glob(os.path.join(extensions_dir, 'ops', 'cpu', '*.cpp')) +
                   glob.glob(os.path.join(extensions_dir, 'ops', 'dispatch', '*.cpp')) +
                   glob.glob(os.path.join(extensions_dir, 'ops', 'autograd', '*.cpp')) +
-                  glob.glob(os.path.join(extensions_dir, 'ops', 'quantized', 'cpu', '*.cpp'))
+                  glob.glob(os.path.join(extensions_dir, 'ops', 'quantized', 'cpu', '*.cpp')) +
+                  glob.glob(os.path.join(extensions_dir, 'ops', 'utils', '*.cpp'))
                   )
 
     source_cuda = glob.glob(os.path.join(extensions_dir, 'ops', 'cuda', '*.cu'))
     source_cuda += glob.glob(os.path.join(extensions_dir, 'ops', 'autocast', '*.cpp'))
 
     sources = main_file + source_cpu
     extension = CppExtension
```

### Comparing `tvdcn-0.3.0/tests/test_compatibility_with_torchvision.py` & `tvdcn-0.3.1/tests/test_compatibility_with_torchvision.py`

 * *Files identical despite different names*

### Comparing `tvdcn-0.3.0/tests/test_grad.py` & `tvdcn-0.3.1/tests/test_grad.py`

 * *Files identical despite different names*

### Comparing `tvdcn-0.3.0/tvdcn/csrc/ops/cpu/deform_conv1d_kernels_cpu.cpp` & `tvdcn-0.3.1/tvdcn/csrc/ops/cpu/deform_conv1d_kernels_cpu.cpp`

 * *Files identical despite different names*

### Comparing `tvdcn-0.3.0/tvdcn/csrc/ops/cpu/deform_conv2d_kernels_cpu.cpp` & `tvdcn-0.3.1/tvdcn/csrc/ops/cpu/deform_conv2d_kernels_cpu.cpp`

 * *Files identical despite different names*

### Comparing `tvdcn-0.3.0/tvdcn/csrc/ops/cpu/deform_conv3d_kernels_cpu.cpp` & `tvdcn-0.3.1/tvdcn/csrc/ops/cpu/deform_conv3d_kernels_cpu.cpp`

 * *Files identical despite different names*

### Comparing `tvdcn-0.3.0/tvdcn/csrc/ops/cuda/deform_conv1d_kernels_cuda.cu` & `tvdcn-0.3.1/tvdcn/csrc/ops/cuda/deform_conv1d_kernels_cuda.cu`

 * *Files identical despite different names*

### Comparing `tvdcn-0.3.0/tvdcn/csrc/ops/cuda/deform_conv2d_kernels_cuda.cu` & `tvdcn-0.3.1/tvdcn/csrc/ops/cuda/deform_conv2d_kernels_cuda.cu`

 * *Files identical despite different names*

### Comparing `tvdcn-0.3.0/tvdcn/csrc/ops/cuda/deform_conv3d_kernels_cuda.cu` & `tvdcn-0.3.1/tvdcn/csrc/ops/cuda/deform_conv3d_kernels_cuda.cu`

 * *Files identical despite different names*

### Comparing `tvdcn-0.3.0/tvdcn/csrc/ops/deform_conv1d.cpp` & `tvdcn-0.3.1/tvdcn/csrc/ops/deform_conv1d.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -66,41 +66,44 @@
 // modified from
 // https://github.com/open-mmlab/mmdetection/blob/master/mmdet/ops/dcn/src/deform_conv_cuda.cpp
 
 // modified from
 // https://github.com/pytorch/vision/blob/master/torchvision/csrc/cpu/deform_conv2d_kernel.cpp
 
 #include <torch/autograd.h>
-#include "utils/parallel_helpers.h"
+
 #include "dispatch/deform_conv1d_kernels.h"
+#include "utils/parallel_helpers.h"
+#include "utils/tensor_utils.h"
 
 namespace tvdcn {
     namespace ops {
         at::Tensor deform_conv1d_forward(
                 const at::Tensor &input,
                 const at::Tensor &weight,
                 const at::Tensor &offset,
                 const at::Tensor &mask,
                 const at::Tensor &bias,
                 at::IntArrayRef stride,
                 at::IntArrayRef padding,
                 at::IntArrayRef dilation,
-                int64_t groups,
-                bool deformable,
-                bool modulated) {
+                int64_t groups) {
             at::CheckedFrom c = "deform_conv1d_forward";
             auto args = {
                     at::TensorArg(input, "input", 1),
                     at::TensorArg(weight, "weight", 2),
                     at::TensorArg(offset, "offset", 3),
                     at::TensorArg(mask, "mask", 4),
                     at::TensorArg(bias, "bias", 5)};
             at::checkAllSameType(c, args);
-            if (input.device().is_cuda())
-                at::checkAllSameGPU(c, args);
+            at::checkAllSameDevice(c, args);
+
+            bool deformable = offset.defined() && offset.numel();
+            bool modulated = mask.defined() && mask.numel();
+            bool with_bias = bias.defined() && bias.numel();
 
             at::Tensor input_c = input.contiguous();
             at::Tensor weight_c = weight.contiguous();
             at::Tensor offset_c = offset.contiguous();
             at::Tensor mask_c = mask.contiguous();
             at::Tensor bias_c = bias.contiguous();
 
@@ -130,66 +133,74 @@
                     weight_w > 0,
                     " weight_w: ",
                     weight_w)
             TORCH_CHECK(
                     stride_w > 0,
                     " stride_w: ",
                     stride_w)
-            TORCH_CHECK(pad_w >= 0, " pad_w: ", pad_w)
-            TORCH_CHECK(dilation_w > 0, " dilation_w: ", dilation_w)
+            TORCH_CHECK(
+                    pad_w >= 0,
+                    " pad_w: ",
+                    pad_w)
+            TORCH_CHECK(
+                    dilation_w > 0,
+                    " dilation_w: ",
+                    dilation_w)
 
             TORCH_CHECK(weight_c.size(1) * groups == in_channels)
             TORCH_CHECK(weight_c.size(0) % groups == 0)
 
-            int64_t offset_groups = offset.size(1) / weight_w;
-            int64_t mask_groups = mask.size(1) / weight_w;
+            int64_t offset_groups = deformable ? offset.size(1) / weight_w : 0;
+            int64_t mask_groups = modulated ? mask.size(1) / weight_w : 0;
 
-            TORCH_CHECK(!deformable || offset_groups > 0,
-                        "The shape of the offset tensor at dimension 1 is not valid. It should "
-                        "be a multiple of weight.size(2).\nGot offset.size(1)=",
-                        offset.size(1),
-                        ", while weight.size(2)=",
-                        weight_w)
+            TORCH_CHECK(
+                    !deformable || offset_c.size(0) == input_c.size(0),
+                    "invalid batch size of offset")
+            TORCH_CHECK(
+                    !deformable || offset_groups > 0,
+                    "The shape of the offset tensor at dimension 1 is not valid. It should "
+                    "be a multiple of weight.size(2).\nGot offset.size(1)=",
+                    offset.size(1),
+                    ", while weight.size(2)=",
+                    weight_w)
             TORCH_CHECK(!deformable || input_c.size(1) % offset_groups == 0)
-
-            TORCH_CHECK(!modulated || mask_groups > 0,
-                        "The shape of the mask tensor at dimension 1 is not valid. It should "
-                        "be a multiple of weight.size(2).\nGot mask.size(1)=",
-                        mask.size(1),
-                        ", while weight.size(2)=",
-                        weight_w)
-            TORCH_CHECK(!modulated || input_c.size(1) % mask_groups == 0)
-
             TORCH_CHECK(
-                    (!deformable || offset_c.size(1) == offset_groups * weight_w),
+                    !deformable || offset_c.size(1) == offset_groups * weight_w,
                     "offset.shape[1] is not valid. got: ",
                     offset_c.size(1),
                     " expected: ",
                     offset_groups * weight_w)
             TORCH_CHECK(
-                    (offset_c.size(0) == input_c.size(0)), "invalid batch size of offset")
-            TORCH_CHECK(
-                    (!deformable || offset_c.size(2) == out_w),
+                    !deformable || offset_c.size(2) == out_w,
                     "offset output dims: (",
                     offset_c.size(2),
                     ") - ",
                     "computed output dims: (",
                     out_w,
                     ")")
 
             TORCH_CHECK(
-                    (!modulated || mask_c.size(1) == mask_groups * weight_w),
+                    !modulated || mask_c.size(0) == input_c.size(0),
+                    "invalid batch size of mask")
+            TORCH_CHECK(
+                    !modulated || mask_groups > 0,
+                    "The shape of the mask tensor at dimension 1 is not valid. It should "
+                    "be a multiple of weight.size(2).\nGot mask.size(1)=",
+                    mask.size(1),
+                    ", while weight.size(2)=",
+                    weight_w)
+            TORCH_CHECK(!modulated || input_c.size(1) % mask_groups == 0)
+            TORCH_CHECK(
+                    !modulated || mask_c.size(1) == mask_groups * weight_w,
                     "mask.shape[1] is not valid. got: ",
                     mask_c.size(1),
                     " expected: ",
                     mask_groups * weight_w)
             TORCH_CHECK(
-                    (mask_c.size(0) == input_c.size(0)), "invalid batch size of mask")
-            TORCH_CHECK(
-                    (!modulated || mask_c.size(2) == out_w),
+                    !modulated || mask_c.size(2) == out_w,
                     "mask output dims: (",
                     mask_c.size(2),
                     ") - ",
                     "computed output dims: (",
                     out_w,
                     ")")
 
@@ -285,33 +296,37 @@
             output_buf = output_buf.view({batch_sz / n_parallel_imgs,
                                           out_channels,
                                           n_parallel_imgs,
                                           out_w});
             output_buf.transpose_(1, 2);
             output.copy_(output_buf);
             output = output.view({batch_sz, out_channels, out_w});
+            if (with_bias)
+                output.add_(bias_c.view({1, out_channels, 1}));
 
-            return output + bias_c.view({1, out_channels, 1});
+            return output;
         }
 
         namespace detail {
             std::tuple<at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor>
             _deform_conv1d_backward(
                     const at::Tensor &grad_out,
                     const at::Tensor &input,
                     const at::Tensor &weight,
                     const at::Tensor &offset,
                     const at::Tensor &mask,
                     const at::Tensor &bias,
                     at::IntArrayRef stride,
                     at::IntArrayRef padding,
                     at::IntArrayRef dilation,
-                    int64_t groups,
-                    bool deformable,
-                    bool modulated) {
+                    int64_t groups) {
+                bool deformable = offset.defined() && offset.numel();
+                bool modulated = mask.defined() && mask.numel();
+                bool with_bias = bias.defined() && bias.numel();
+
                 at::Tensor grad_out_c = grad_out.contiguous();
                 at::Tensor input_c = input.contiguous();
                 at::Tensor weight_c = weight.contiguous();
                 at::Tensor offset_c = offset.contiguous();
                 at::Tensor mask_c = mask.contiguous();
                 at::Tensor bias_c = bias.contiguous();
 
@@ -328,22 +343,22 @@
 
                 int64_t pad_w = padding[0];
 
                 int64_t dilation_w = dilation[0];
 
                 int64_t out_w = (in_w + 2 * pad_w - (dilation_w * (weight_w - 1) + 1)) / stride_w + 1;
 
-                int64_t offset_groups = offset.size(1) / weight_w;
-                int64_t mask_groups = mask.size(1) / weight_w;
+                int64_t offset_groups = deformable ? offset.size(1) / weight_w : 0;
+                int64_t mask_groups = modulated ? mask.size(1) / weight_w : 0;
 
                 auto grad_input = at::zeros_like(input_c);
                 auto grad_weight = at::zeros_like(weight_c);
                 auto grad_offset = at::zeros_like(offset_c);
                 auto grad_mask = at::zeros_like(mask_c);
-                auto grad_bias = at::ones_like(bias_c);
+                auto grad_bias = with_bias ? grad_out_c.sum(at::IntArrayRef({0, 2})) : at::zeros_like(bias_c);
 
                 // Separate into blocks
                 input_c = input_c.view({batch_sz / n_parallel_imgs,
                                         n_parallel_imgs,
                                         in_channels,
                                         in_w});
                 grad_input = grad_input.view_as(input_c);
@@ -479,15 +494,14 @@
                     }
                 }
 
                 grad_input = grad_input.view_as(input);
                 grad_weight = grad_weight.view_as(weight);
                 grad_offset = grad_offset.view_as(offset);
                 grad_mask = grad_mask.view_as(mask);
-                grad_bias *= grad_out.sum(at::IntArrayRef({0, 2}));
 
                 return std::make_tuple(grad_input, grad_weight, grad_offset, grad_mask, grad_bias);
             }
         }
 
         class DeformConv1dFunction
                 : public torch::autograd::Function<DeformConv1dFunction> {
@@ -498,38 +512,32 @@
                     const torch::autograd::Variable &weight,
                     const torch::autograd::Variable &offset,
                     const torch::autograd::Variable &mask,
                     const torch::autograd::Variable &bias,
                     at::IntArrayRef stride,
                     at::IntArrayRef padding,
                     at::IntArrayRef dilation,
-                    int64_t groups,
-                    bool deformable,
-                    bool modulated) {
+                    int64_t groups) {
                 at::AutoDispatchBelowADInplaceOrView g;
                 auto output = deform_conv1d_forward(
                         input,
                         weight,
                         offset,
                         mask,
                         bias,
                         stride,
                         padding,
                         dilation,
-                        groups,
-                        deformable,
-                        modulated);
+                        groups);
 
                 ctx->save_for_backward({input, weight, offset, mask, bias});
                 ctx->saved_data["stride"] = stride.vec();
                 ctx->saved_data["padding"] = padding.vec();
                 ctx->saved_data["dilation"] = dilation.vec();
                 ctx->saved_data["groups"] = groups;
-                ctx->saved_data["deformable"] = deformable;
-                ctx->saved_data["modulated"] = modulated;
 
                 return {
                         output,
                 };
             }
 
             static torch::autograd::variable_list backward(
@@ -542,30 +550,26 @@
                 auto mask = saved[3];
                 auto bias = saved[4];
 
                 auto stride = ctx->saved_data["stride"].toIntVector();
                 auto padding = ctx->saved_data["padding"].toIntVector();
                 auto dilation = ctx->saved_data["dilation"].toIntVector();
                 auto groups = ctx->saved_data["groups"].toInt();
-                auto deformable = ctx->saved_data["deformable"].toBool();
-                auto modulated = ctx->saved_data["modulated"].toBool();
 
                 auto grads = detail::_deform_conv1d_backward(
                         grad_output[0],
                         input,
                         weight,
                         offset,
                         mask,
                         bias,
                         stride,
                         padding,
                         dilation,
-                        groups,
-                        deformable,
-                        modulated);
+                        groups);
                 auto grad_input = std::get<0>(grads);
                 auto grad_weight = std::get<1>(grads);
                 auto grad_offset = std::get<2>(grads);
                 auto grad_mask = std::get<3>(grads);
                 auto grad_bias = std::get<4>(grads);
 
                 return {
@@ -574,43 +578,39 @@
                         grad_offset,
                         grad_mask,
                         grad_bias,
                         torch::autograd::Variable(),
                         torch::autograd::Variable(),
                         torch::autograd::Variable(),
                         torch::autograd::Variable(),
-                        torch::autograd::Variable(),
-                        torch::autograd::Variable(),
                 };
             }
         };
 
         at::Tensor deform_conv1d(
                 const at::Tensor &input,
                 const at::Tensor &weight,
                 const at::optional<at::Tensor> &offset = {},
                 const at::optional<at::Tensor> &mask = {},
                 const at::optional<at::Tensor> &bias = {},
                 at::IntArrayRef stride = 1,
                 at::IntArrayRef padding = 0,
                 at::IntArrayRef dilation = 1,
                 int64_t groups = 1) {
-            C10_LOG_API_USAGE_ONCE("tvdcn.csrc.ops.deform_conv.deform_conv1d");
+            C10_LOG_API_USAGE_ONCE("tvdcn.csrc.ops.deform_conv.deform_conv1d")
             auto result = DeformConv1dFunction::apply(
                     input,
                     weight,
-                    offset.value_or(at::zeros({input.size(0), 0}, input.options().requires_grad(false))),
-                    mask.value_or(at::zeros({input.size(0), 0}, input.options().requires_grad(false))),
-                    bias.value_or(at::zeros({weight.size(0)}, input.options().requires_grad(false))),
+                    offset.value_or(input.new_zeros(0)),
+                    mask.value_or(input.new_zeros(0)),
+                    bias.value_or(input.new_zeros(0)),
                     stride,
                     padding,
                     dilation,
-                    groups,
-                    offset.has_value(),
-                    mask.has_value());
+                    groups);
             return result[0];
         }
 
         TORCH_LIBRARY_FRAGMENT(tvdcn, m) {
             m.def("tvdcn::deform_conv1d(Tensor input, Tensor weight, "
                   "Tensor? offset=None, Tensor? mask=None, Tensor? bias=None, "
                   "int[1] stride=1, int[1] padding=0, int[1] dilation=1, int groups=1) -> Tensor",
```

### Comparing `tvdcn-0.3.0/tvdcn/csrc/ops/deform_conv2d.cpp` & `tvdcn-0.3.1/tvdcn/csrc/ops/deform_conv2d.cpp`

 * *Files 5% similar despite different names*

```diff
@@ -66,41 +66,44 @@
 // modified from
 // https://github.com/open-mmlab/mmdetection/blob/master/mmdet/ops/dcn/src/deform_conv_cuda.cpp
 
 // modified from
 // https://github.com/pytorch/vision/blob/master/torchvision/csrc/cpu/deform_conv2d_kernel.cpp
 
 #include <torch/autograd.h>
-#include "utils/parallel_helpers.h"
+
 #include "dispatch/deform_conv2d_kernels.h"
+#include "utils/parallel_helpers.h"
+#include "utils/tensor_utils.h"
 
 namespace tvdcn {
     namespace ops {
         at::Tensor deform_conv2d_forward(
                 const at::Tensor &input,
                 const at::Tensor &weight,
                 const at::Tensor &offset,
                 const at::Tensor &mask,
                 const at::Tensor &bias,
                 at::IntArrayRef stride,
                 at::IntArrayRef padding,
                 at::IntArrayRef dilation,
-                int64_t groups,
-                bool deformable,
-                bool modulated) {
+                int64_t groups) {
             at::CheckedFrom c = "deform_conv2d_forward";
             auto args = {
                     at::TensorArg(input, "input", 1),
                     at::TensorArg(weight, "weight", 2),
                     at::TensorArg(offset, "offset", 3),
                     at::TensorArg(mask, "mask", 4),
                     at::TensorArg(bias, "bias", 5)};
             at::checkAllSameType(c, args);
-            if (input.device().is_cuda())
-                at::checkAllSameGPU(c, args);
+            at::checkAllSameDevice(c, args);
+
+            bool deformable = offset.defined() && offset.numel();
+            bool modulated = mask.defined() && mask.numel();
+            bool with_bias = bias.defined() && bias.numel();
 
             at::Tensor input_c = input.contiguous();
             at::Tensor weight_c = weight.contiguous();
             at::Tensor offset_c = offset.contiguous();
             at::Tensor mask_c = mask.contiguous();
             at::Tensor bias_c = bias.contiguous();
 
@@ -140,72 +143,84 @@
                     weight_w)
             TORCH_CHECK(
                     stride_h > 0 && stride_w > 0,
                     "stride_h: ",
                     stride_h,
                     " stride_w: ",
                     stride_w)
-            TORCH_CHECK(pad_h >= 0 && pad_w >= 0, "pad_h: ", pad_h, " pad_w: ", pad_w)
-            TORCH_CHECK(dilation_h > 0 && dilation_w > 0, "dilation_h: ", dilation_h, " dilation_w: ", dilation_w)
+            TORCH_CHECK(
+                    pad_h >= 0 && pad_w >= 0,
+                    "pad_h: ",
+                    pad_h,
+                    " pad_w: ",
+                    pad_w)
+            TORCH_CHECK(
+                    dilation_h > 0 && dilation_w > 0,
+                    "dilation_h: ",
+                    dilation_h,
+                    " dilation_w: ",
+                    dilation_w)
 
             TORCH_CHECK(weight_c.size(1) * groups == in_channels)
             TORCH_CHECK(weight_c.size(0) % groups == 0)
 
-            int64_t offset_groups = offset.size(1) / (2 * weight_h * weight_w);
-            int64_t mask_groups = mask.size(1) / (weight_h * weight_w);
+            int64_t offset_groups = deformable ? offset.size(1) / (2 * weight_h * weight_w) : 0;
+            int64_t mask_groups = modulated ? mask.size(1) / (weight_h * weight_w) : 0;
 
-            TORCH_CHECK(!deformable || offset_groups > 0,
-                        "The shape of the offset tensor at dimension 1 is not valid. It should "
-                        "be a multiple of 2 * weight.size(2) * weight.size(3).\nGot offset.size(1)=",
-                        offset.size(1),
-                        ", while 2 * weight.size(2) * weight.size(3)=",
-                        2 * weight_h * weight_w)
+            TORCH_CHECK(
+                    !deformable || offset_c.size(0) == input_c.size(0),
+                    "invalid batch size of offset")
+            TORCH_CHECK(
+                    !deformable || offset_groups > 0,
+                    "The shape of the offset tensor at dimension 1 is not valid. It should "
+                    "be a multiple of 2 * weight.size(2) * weight.size(3).\nGot offset.size(1)=",
+                    offset.size(1),
+                    ", while 2 * weight.size(2) * weight.size(3)=",
+                    2 * weight_h * weight_w)
             TORCH_CHECK(!deformable || input_c.size(1) % offset_groups == 0)
-
-            TORCH_CHECK(!modulated || mask_groups > 0,
-                        "The shape of the mask tensor at dimension 1 is not valid. It should "
-                        "be a multiple of weight.size(2) * weight.size(3).\nGot mask.size(1)=",
-                        mask.size(1),
-                        ", while weight.size(2) * weight.size(3)=",
-                        weight_h * weight_w)
-            TORCH_CHECK(!modulated || input_c.size(1) % mask_groups == 0)
-
             TORCH_CHECK(
-                    (!deformable || offset_c.size(1) == offset_groups * 2 * weight_h * weight_w),
+                    !deformable || offset_c.size(1) == offset_groups * 2 * weight_h * weight_w,
                     "offset.shape[1] is not valid. got: ",
                     offset_c.size(1),
                     " expected: ",
                     offset_groups * 2 * weight_h * weight_w)
             TORCH_CHECK(
-                    (offset_c.size(0) == input_c.size(0)), "invalid batch size of offset")
-            TORCH_CHECK(
-                    (!deformable || (offset_c.size(2) == out_h &&
-                                     offset_c.size(3) == out_w)),
+                    !deformable || (offset_c.size(2) == out_h &&
+                                    offset_c.size(3) == out_w),
                     "offset output dims: (",
                     offset_c.size(2),
                     ", ",
                     offset_c.size(3),
                     ") - ",
                     "computed output dims: (",
                     out_h,
                     ", ",
                     out_w,
                     ")")
 
             TORCH_CHECK(
-                    (!modulated || mask_c.size(1) == mask_groups * weight_h * weight_w),
+                    !modulated || mask_c.size(0) == input_c.size(0),
+                    "invalid batch size of mask")
+            TORCH_CHECK(
+                    !modulated || mask_groups > 0,
+                    "The shape of the mask tensor at dimension 1 is not valid. It should "
+                    "be a multiple of weight.size(2) * weight.size(3).\nGot mask.size(1)=",
+                    mask.size(1),
+                    ", while weight.size(2) * weight.size(3)=",
+                    weight_h * weight_w)
+            TORCH_CHECK(!modulated || input_c.size(1) % mask_groups == 0)
+            TORCH_CHECK(
+                    !modulated || mask_c.size(1) == mask_groups * weight_h * weight_w,
                     "mask.shape[1] is not valid. got: ",
                     mask_c.size(1),
                     " expected: ",
                     mask_groups * weight_h * weight_w)
             TORCH_CHECK(
-                    (mask_c.size(0) == input_c.size(0)), "invalid batch size of mask")
-            TORCH_CHECK(
-                    (!modulated || (mask_c.size(2) == out_h &&
-                                    mask_c.size(3) == out_w)),
+                    !modulated || (mask_c.size(2) == out_h &&
+                                   mask_c.size(3) == out_w),
                     "mask output dims: (",
                     mask_c.size(2),
                     ", ",
                     mask_c.size(3),
                     ") - ",
                     "computed output dims: (",
                     out_h,
@@ -325,33 +340,37 @@
                                           out_channels,
                                           n_parallel_imgs,
                                           out_h,
                                           out_w});
             output_buf.transpose_(1, 2);
             output.copy_(output_buf);
             output = output.view({batch_sz, out_channels, out_h, out_w});
+            if (with_bias)
+                output.add_(bias_c.view({1, out_channels, 1, 1}));
 
-            return output + bias_c.view({1, out_channels, 1, 1});
+            return output;
         }
 
         namespace detail {
             std::tuple<at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor>
             _deform_conv2d_backward(
                     const at::Tensor &grad_out,
                     const at::Tensor &input,
                     const at::Tensor &weight,
                     const at::Tensor &offset,
                     const at::Tensor &mask,
                     const at::Tensor &bias,
                     at::IntArrayRef stride,
                     at::IntArrayRef padding,
                     at::IntArrayRef dilation,
-                    int64_t groups,
-                    bool deformable,
-                    bool modulated) {
+                    int64_t groups) {
+                bool deformable = offset.defined() && offset.numel();
+                bool modulated = mask.defined() && mask.numel();
+                bool with_bias = bias.defined() && bias.numel();
+
                 at::Tensor grad_out_c = grad_out.contiguous();
                 at::Tensor input_c = input.contiguous();
                 at::Tensor weight_c = weight.contiguous();
                 at::Tensor offset_c = offset.contiguous();
                 at::Tensor mask_c = mask.contiguous();
                 at::Tensor bias_c = bias.contiguous();
 
@@ -374,22 +393,22 @@
 
                 int64_t dilation_h = dilation[0];
                 int64_t dilation_w = dilation[1];
 
                 int64_t out_h = (in_h + 2 * pad_h - (dilation_h * (weight_h - 1) + 1)) / stride_h + 1;
                 int64_t out_w = (in_w + 2 * pad_w - (dilation_w * (weight_w - 1) + 1)) / stride_w + 1;
 
-                int64_t offset_groups = offset.size(1) / (2 * weight_h * weight_w);
-                int64_t mask_groups = mask.size(1) / (weight_h * weight_w);
+                int64_t offset_groups = deformable ? offset.size(1) / (2 * weight_h * weight_w) : 0;
+                int64_t mask_groups = modulated ? mask.size(1) / (weight_h * weight_w) : 0;
 
                 auto grad_input = at::zeros_like(input_c);
                 auto grad_weight = at::zeros_like(weight_c);
                 auto grad_offset = at::zeros_like(offset_c);
                 auto grad_mask = at::zeros_like(mask_c);
-                auto grad_bias = at::ones_like(bias_c);
+                auto grad_bias = with_bias ? grad_out_c.sum(at::IntArrayRef({0, 2, 3})) : at::zeros_like(bias_c);
 
                 // Separate into blocks
                 input_c = input_c.view({batch_sz / n_parallel_imgs,
                                         n_parallel_imgs,
                                         in_channels,
                                         in_h,
                                         in_w});
@@ -558,15 +577,14 @@
                     }
                 }
 
                 grad_input = grad_input.view_as(input);
                 grad_weight = grad_weight.view_as(weight);
                 grad_offset = grad_offset.view_as(offset);
                 grad_mask = grad_mask.view_as(mask);
-                grad_bias *= grad_out.sum(at::IntArrayRef({0, 2, 3}));
 
                 return std::make_tuple(grad_input, grad_weight, grad_offset, grad_mask, grad_bias);
             }
         }
 
         class DeformConv2dFunction
                 : public torch::autograd::Function<DeformConv2dFunction> {
@@ -577,38 +595,32 @@
                     const torch::autograd::Variable &weight,
                     const torch::autograd::Variable &offset,
                     const torch::autograd::Variable &mask,
                     const torch::autograd::Variable &bias,
                     at::IntArrayRef stride,
                     at::IntArrayRef padding,
                     at::IntArrayRef dilation,
-                    int64_t groups,
-                    bool deformable,
-                    bool modulated) {
+                    int64_t groups) {
                 at::AutoDispatchBelowADInplaceOrView g;
                 auto output = deform_conv2d_forward(
                         input,
                         weight,
                         offset,
                         mask,
                         bias,
                         stride,
                         padding,
                         dilation,
-                        groups,
-                        deformable,
-                        modulated);
+                        groups);
 
                 ctx->save_for_backward({input, weight, offset, mask, bias});
                 ctx->saved_data["stride"] = stride.vec();
                 ctx->saved_data["padding"] = padding.vec();
                 ctx->saved_data["dilation"] = dilation.vec();
                 ctx->saved_data["groups"] = groups;
-                ctx->saved_data["deformable"] = deformable;
-                ctx->saved_data["modulated"] = modulated;
 
                 return {
                         output,
                 };
             }
 
             static torch::autograd::variable_list backward(
@@ -621,30 +633,26 @@
                 auto mask = saved[3];
                 auto bias = saved[4];
 
                 auto stride = ctx->saved_data["stride"].toIntVector();
                 auto padding = ctx->saved_data["padding"].toIntVector();
                 auto dilation = ctx->saved_data["dilation"].toIntVector();
                 auto groups = ctx->saved_data["groups"].toInt();
-                auto deformable = ctx->saved_data["deformable"].toBool();
-                auto modulated = ctx->saved_data["modulated"].toBool();
 
                 auto grads = detail::_deform_conv2d_backward(
                         grad_output[0],
                         input,
                         weight,
                         offset,
                         mask,
                         bias,
                         stride,
                         padding,
                         dilation,
-                        groups,
-                        deformable,
-                        modulated);
+                        groups);
                 auto grad_input = std::get<0>(grads);
                 auto grad_weight = std::get<1>(grads);
                 auto grad_offset = std::get<2>(grads);
                 auto grad_mask = std::get<3>(grads);
                 auto grad_bias = std::get<4>(grads);
 
                 return {
@@ -653,43 +661,39 @@
                         grad_offset,
                         grad_mask,
                         grad_bias,
                         torch::autograd::Variable(),
                         torch::autograd::Variable(),
                         torch::autograd::Variable(),
                         torch::autograd::Variable(),
-                        torch::autograd::Variable(),
-                        torch::autograd::Variable(),
                 };
             }
         };
 
         at::Tensor deform_conv2d(
                 const at::Tensor &input,
                 const at::Tensor &weight,
                 const at::optional<at::Tensor> &offset = {},
                 const at::optional<at::Tensor> &mask = {},
                 const at::optional<at::Tensor> &bias = {},
                 at::IntArrayRef stride = 1,
                 at::IntArrayRef padding = 0,
                 at::IntArrayRef dilation = 1,
                 int64_t groups = 1) {
-            C10_LOG_API_USAGE_ONCE("tvdcn.csrc.ops.deform_conv.deform_conv2d");
+            C10_LOG_API_USAGE_ONCE("tvdcn.csrc.ops.deform_conv.deform_conv2d")
             auto result = DeformConv2dFunction::apply(
                     input,
                     weight,
-                    offset.value_or(at::zeros({input.size(0), 0}, input.options().requires_grad(false))),
-                    mask.value_or(at::zeros({input.size(0), 0}, input.options().requires_grad(false))),
-                    bias.value_or(at::zeros({weight.size(0)}, input.options().requires_grad(false))),
+                    offset.value_or(input.new_zeros(0)),
+                    mask.value_or(input.new_zeros(0)),
+                    bias.value_or(input.new_zeros(0)),
                     stride,
                     padding,
                     dilation,
-                    groups,
-                    offset.has_value(),
-                    mask.has_value());
+                    groups);
             return result[0];
         }
 
         TORCH_LIBRARY_FRAGMENT(tvdcn, m) {
             m.def("tvdcn::deform_conv2d(Tensor input, Tensor weight, "
                   "Tensor? offset=None, Tensor? mask=None, Tensor? bias=None, "
                   "int[2] stride=1, int[2] padding=0, int[2] dilation=1, int groups=1) -> Tensor",
```

### Comparing `tvdcn-0.3.0/tvdcn/csrc/ops/deform_conv3d.cpp` & `tvdcn-0.3.1/tvdcn/csrc/ops/deform_conv3d.cpp`

 * *Files 3% similar despite different names*

```diff
@@ -66,41 +66,44 @@
 // modified from
 // https://github.com/open-mmlab/mmdetection/blob/master/mmdet/ops/dcn/src/deform_conv_cuda.cpp
 
 // modified from
 // https://github.com/pytorch/vision/blob/master/torchvision/csrc/cpu/deform_conv2d_kernel.cpp
 
 #include <torch/autograd.h>
-#include "utils/parallel_helpers.h"
+
 #include "dispatch/deform_conv3d_kernels.h"
+#include "utils/parallel_helpers.h"
+#include "utils/tensor_utils.h"
 
 namespace tvdcn {
     namespace ops {
         at::Tensor deform_conv3d_forward(
                 const at::Tensor &input,
                 const at::Tensor &weight,
                 const at::Tensor &offset,
                 const at::Tensor &mask,
                 const at::Tensor &bias,
                 at::IntArrayRef stride,
                 at::IntArrayRef padding,
                 at::IntArrayRef dilation,
-                int64_t groups,
-                bool deformable,
-                bool modulated) {
+                int64_t groups) {
             at::CheckedFrom c = "deform_conv3d_forward";
             auto args = {
                     at::TensorArg(input, "input", 1),
                     at::TensorArg(weight, "weight", 2),
                     at::TensorArg(offset, "offset", 3),
                     at::TensorArg(mask, "mask", 4),
                     at::TensorArg(bias, "bias", 5)};
             at::checkAllSameType(c, args);
-            if (input.device().is_cuda())
-                at::checkAllSameGPU(c, args);
+            at::checkAllSameDevice(c, args);
+
+            bool deformable = offset.defined() && offset.numel();
+            bool modulated = mask.defined() && mask.numel();
+            bool with_bias = bias.defined() && bias.numel();
 
             at::Tensor input_c = input.contiguous();
             at::Tensor weight_c = weight.contiguous();
             at::Tensor offset_c = offset.contiguous();
             at::Tensor mask_c = mask.contiguous();
             at::Tensor bias_c = bias.contiguous();
 
@@ -150,52 +153,58 @@
                     stride_d > 0 && stride_h > 0 && stride_w > 0,
                     " stride_d: ",
                     stride_d,
                     "stride_h: ",
                     stride_h,
                     " stride_w: ",
                     stride_w)
-            TORCH_CHECK(pad_d >= 0 && pad_h >= 0 && pad_w >= 0, "pad_d: ", pad_d, " pad_h: ", pad_h, " pad_w: ", pad_w)
-            TORCH_CHECK(dilation_d > 0 && dilation_h > 0 && dilation_w > 0, "dilation_d: ", dilation_d, " dilation_h: ",
-                        dilation_h, " dilation_w: ", dilation_w)
+            TORCH_CHECK(
+                    pad_d >= 0 && pad_h >= 0 && pad_w >= 0,
+                    "pad_d: ",
+                    pad_d,
+                    " pad_h: ",
+                    pad_h,
+                    " pad_w: ",
+                    pad_w)
+            TORCH_CHECK(
+                    dilation_d > 0 && dilation_h > 0 && dilation_w > 0,
+                    "dilation_d: ",
+                    dilation_d,
+                    " dilation_h: ",
+                    dilation_h,
+                    " dilation_w: ",
+                    dilation_w)
 
             TORCH_CHECK(weight_c.size(1) * groups == in_channels)
             TORCH_CHECK(weight_c.size(0) % groups == 0)
 
-            int64_t offset_groups = offset.size(1) / (3 * weight_d * weight_h * weight_w);
-            int64_t mask_groups = mask.size(1) / (weight_d * weight_h * weight_w);
+            int64_t offset_groups = deformable ? offset.size(1) / (3 * weight_d * weight_h * weight_w) : 0;
+            int64_t mask_groups = modulated ? mask.size(1) / (weight_d * weight_h * weight_w) : 0;
 
-            TORCH_CHECK(!deformable || offset_groups > 0,
-                        "The shape of the offset tensor at dimension 1 is not valid. It should "
-                        "be a multiple of 3 * weight.size(2) * weight.size(3) * weight.size(4).\nGot offset.size(1)=",
-                        offset.size(1),
-                        ", while 3 * weight.size(2) * weight.size(3) * weight.size(3)=",
-                        3 * weight_d * weight_h * weight_w)
+            TORCH_CHECK(
+                    !deformable || offset_c.size(0) == input_c.size(0),
+                    "invalid batch size of offset")
+            TORCH_CHECK(
+                    !deformable || offset_groups > 0,
+                    "The shape of the offset tensor at dimension 1 is not valid. It should "
+                    "be a multiple of 3 * weight.size(2) * weight.size(3) * weight.size(4).\nGot offset.size(1)=",
+                    offset.size(1),
+                    ", while 3 * weight.size(2) * weight.size(3) * weight.size(3)=",
+                    3 * weight_d * weight_h * weight_w)
             TORCH_CHECK(!deformable || input_c.size(1) % offset_groups == 0)
-
-            TORCH_CHECK(!modulated || mask_groups > 0,
-                        "The shape of the mask tensor at dimension 1 is not valid. It should "
-                        "be a multiple of weight.size(2) * weight.size(3) * weight.size(4).\nGot mask.size(1)=",
-                        mask.size(1),
-                        ", while weight.size(2) * weight.size(3) * weight.size(4)=",
-                        weight_d * weight_h * weight_w)
-            TORCH_CHECK(!modulated || input_c.size(1) % mask_groups == 0)
-
             TORCH_CHECK(
-                    (!deformable || offset_c.size(1) == offset_groups * 3 * weight_d * weight_h * weight_w),
+                    !deformable || offset_c.size(1) == offset_groups * 3 * weight_d * weight_h * weight_w,
                     "offset.shape[1] is not valid. got: ",
                     offset_c.size(1),
                     " expected: ",
                     offset_groups * 3 * weight_d * weight_h * weight_w)
             TORCH_CHECK(
-                    (offset_c.size(0) == input_c.size(0)), "invalid batch size of offset")
-            TORCH_CHECK(
-                    (!deformable || (offset_c.size(2) == out_d &&
-                                     offset_c.size(3) == out_h &&
-                                     offset_c.size(4) == out_w)),
+                    !deformable || (offset_c.size(2) == out_d &&
+                                    offset_c.size(3) == out_h &&
+                                    offset_c.size(4) == out_w),
                     "offset output dims: (",
                     offset_c.size(2),
                     ", ",
                     offset_c.size(3),
                     ", ",
                     offset_c.size(4),
                     ") - ",
@@ -204,25 +213,34 @@
                     ", ",
                     out_h,
                     ", ",
                     out_w,
                     ")")
 
             TORCH_CHECK(
-                    (!modulated || mask_c.size(1) == mask_groups * weight_d * weight_h * weight_w),
+                    !modulated || mask_c.size(0) == input_c.size(0),
+                    "invalid batch size of mask")
+            TORCH_CHECK(
+                    !modulated || mask_groups > 0,
+                    "The shape of the mask tensor at dimension 1 is not valid. It should "
+                    "be a multiple of weight.size(2) * weight.size(3) * weight.size(4).\nGot mask.size(1)=",
+                    mask.size(1),
+                    ", while weight.size(2) * weight.size(3) * weight.size(4)=",
+                    weight_d * weight_h * weight_w)
+            TORCH_CHECK(!modulated || input_c.size(1) % mask_groups == 0)
+            TORCH_CHECK(
+                    !modulated || mask_c.size(1) == mask_groups * weight_d * weight_h * weight_w,
                     "mask.shape[1] is not valid. got: ",
                     mask_c.size(1),
                     " expected: ",
                     mask_groups * weight_d * weight_h * weight_w)
             TORCH_CHECK(
-                    (mask_c.size(0) == input_c.size(0)), "invalid batch size of mask")
-            TORCH_CHECK(
-                    (!modulated || (mask_c.size(2) == out_d &&
-                                    mask_c.size(3) == out_h &&
-                                    mask_c.size(4) == out_w)),
+                    !modulated || (mask_c.size(2) == out_d &&
+                                   mask_c.size(3) == out_h &&
+                                   mask_c.size(4) == out_w),
                     "mask output dims: (",
                     mask_c.size(2),
                     ", ",
                     mask_c.size(3),
                     ", ",
                     mask_c.size(4),
                     ") - ",
@@ -366,33 +384,37 @@
                                           n_parallel_imgs,
                                           out_d,
                                           out_h,
                                           out_w});
             output_buf.transpose_(1, 2);
             output.copy_(output_buf);
             output = output.view({batch_sz, out_channels, out_d, out_h, out_w});
+            if (with_bias)
+                output.add_(bias_c.view({1, out_channels, 1, 1, 1}));
 
-            return output + bias_c.view({1, out_channels, 1, 1, 1});
+            return output;
         }
 
         namespace detail {
             std::tuple<at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor>
             _deform_conv3d_backward(
                     const at::Tensor &grad_out,
                     const at::Tensor &input,
                     const at::Tensor &weight,
                     const at::Tensor &offset,
                     const at::Tensor &mask,
                     const at::Tensor &bias,
                     at::IntArrayRef stride,
                     at::IntArrayRef padding,
                     at::IntArrayRef dilation,
-                    int64_t groups,
-                    bool deformable,
-                    bool modulated) {
+                    int64_t groups) {
+                bool deformable = offset.defined() && offset.numel();
+                bool modulated = mask.defined() && mask.numel();
+                bool with_bias = bias.defined() && bias.numel();
+
                 at::Tensor grad_out_c = grad_out.contiguous();
                 at::Tensor input_c = input.contiguous();
                 at::Tensor weight_c = weight.contiguous();
                 at::Tensor offset_c = offset.contiguous();
                 at::Tensor mask_c = mask.contiguous();
                 at::Tensor bias_c = bias.contiguous();
 
@@ -421,22 +443,22 @@
                 int64_t dilation_h = dilation[1];
                 int64_t dilation_w = dilation[2];
 
                 int64_t out_d = (in_d + 2 * pad_d - (dilation_d * (weight_d - 1) + 1)) / stride_d + 1;
                 int64_t out_h = (in_h + 2 * pad_h - (dilation_h * (weight_h - 1) + 1)) / stride_h + 1;
                 int64_t out_w = (in_w + 2 * pad_w - (dilation_w * (weight_w - 1) + 1)) / stride_w + 1;
 
-                int64_t offset_groups = offset.size(1) / (3 * weight_d * weight_h * weight_w);
-                int64_t mask_groups = mask.size(1) / (weight_d * weight_h * weight_w);
+                int64_t offset_groups = deformable ? offset.size(1) / (3 * weight_d * weight_h * weight_w) : 0;
+                int64_t mask_groups = modulated ? mask.size(1) / (weight_d * weight_h * weight_w) : 0;
 
                 auto grad_input = at::zeros_like(input_c);
                 auto grad_weight = at::zeros_like(weight_c);
                 auto grad_offset = at::zeros_like(offset_c);
                 auto grad_mask = at::zeros_like(mask_c);
-                auto grad_bias = at::ones_like(bias_c);
+                auto grad_bias = with_bias ? grad_out_c.sum(at::IntArrayRef({0, 2, 3, 4})) : at::zeros_like(bias_c);
 
                 // Separate into blocks
                 input_c = input_c.view({batch_sz / n_parallel_imgs,
                                         n_parallel_imgs,
                                         in_channels,
                                         in_d,
                                         in_h,
@@ -638,15 +660,14 @@
                     }
                 }
 
                 grad_input = grad_input.view_as(input);
                 grad_weight = grad_weight.view_as(weight);
                 grad_offset = grad_offset.view_as(offset);
                 grad_mask = grad_mask.view_as(mask);
-                grad_bias *= grad_out.sum(at::IntArrayRef({0, 2, 3, 4}));
 
                 return std::make_tuple(grad_input, grad_weight, grad_offset, grad_mask, grad_bias);
             }
         }
 
         class DeformConv3dFunction
                 : public torch::autograd::Function<DeformConv3dFunction> {
@@ -657,38 +678,32 @@
                     const torch::autograd::Variable &weight,
                     const torch::autograd::Variable &offset,
                     const torch::autograd::Variable &mask,
                     const torch::autograd::Variable &bias,
                     at::IntArrayRef stride,
                     at::IntArrayRef padding,
                     at::IntArrayRef dilation,
-                    int64_t groups,
-                    bool deformable,
-                    bool modulated) {
+                    int64_t groups) {
                 at::AutoDispatchBelowADInplaceOrView g;
                 auto output = deform_conv3d_forward(
                         input,
                         weight,
                         offset,
                         mask,
                         bias,
                         stride,
                         padding,
                         dilation,
-                        groups,
-                        deformable,
-                        modulated);
+                        groups);
 
                 ctx->save_for_backward({input, weight, offset, mask, bias});
                 ctx->saved_data["stride"] = stride.vec();
                 ctx->saved_data["padding"] = padding.vec();
                 ctx->saved_data["dilation"] = dilation.vec();
                 ctx->saved_data["groups"] = groups;
-                ctx->saved_data["deformable"] = deformable;
-                ctx->saved_data["modulated"] = modulated;
 
                 return {
                         output,
                 };
             }
 
             static torch::autograd::variable_list backward(
@@ -701,30 +716,26 @@
                 auto mask = saved[3];
                 auto bias = saved[4];
 
                 auto stride = ctx->saved_data["stride"].toIntVector();
                 auto padding = ctx->saved_data["padding"].toIntVector();
                 auto dilation = ctx->saved_data["dilation"].toIntVector();
                 auto groups = ctx->saved_data["groups"].toInt();
-                auto deformable = ctx->saved_data["deformable"].toBool();
-                auto modulated = ctx->saved_data["modulated"].toBool();
 
                 auto grads = detail::_deform_conv3d_backward(
                         grad_output[0],
                         input,
                         weight,
                         offset,
                         mask,
                         bias,
                         stride,
                         padding,
                         dilation,
-                        groups,
-                        deformable,
-                        modulated);
+                        groups);
                 auto grad_input = std::get<0>(grads);
                 auto grad_weight = std::get<1>(grads);
                 auto grad_offset = std::get<2>(grads);
                 auto grad_mask = std::get<3>(grads);
                 auto grad_bias = std::get<4>(grads);
 
                 return {
@@ -733,43 +744,39 @@
                         grad_offset,
                         grad_mask,
                         grad_bias,
                         torch::autograd::Variable(),
                         torch::autograd::Variable(),
                         torch::autograd::Variable(),
                         torch::autograd::Variable(),
-                        torch::autograd::Variable(),
-                        torch::autograd::Variable(),
                 };
             }
         };
 
         at::Tensor deform_conv3d(
                 const at::Tensor &input,
                 const at::Tensor &weight,
                 const at::optional<at::Tensor> &offset = {},
                 const at::optional<at::Tensor> &mask = {},
                 const at::optional<at::Tensor> &bias = {},
                 at::IntArrayRef stride = 1,
                 at::IntArrayRef padding = 0,
                 at::IntArrayRef dilation = 1,
                 int64_t groups = 1) {
-            C10_LOG_API_USAGE_ONCE("tvdcn.csrc.ops.deform_conv.deform_conv3d");
+            C10_LOG_API_USAGE_ONCE("tvdcn.csrc.ops.deform_conv.deform_conv3d")
             auto result = DeformConv3dFunction::apply(
                     input,
                     weight,
-                    offset.value_or(at::zeros({input.size(0), 0}, input.options().requires_grad(false))),
-                    mask.value_or(at::zeros({input.size(0), 0}, input.options().requires_grad(false))),
-                    bias.value_or(at::zeros({weight.size(0)}, input.options().requires_grad(false))),
+                    offset.value_or(input.new_zeros(0)),
+                    mask.value_or(input.new_zeros(0)),
+                    bias.value_or(input.new_zeros(0)),
                     stride,
                     padding,
                     dilation,
-                    groups,
-                    offset.has_value(),
-                    mask.has_value());
+                    groups);
             return result[0];
         }
 
         TORCH_LIBRARY_FRAGMENT(tvdcn, m) {
             m.def("tvdcn::deform_conv3d(Tensor input, Tensor weight, "
                   "Tensor? offset=None, Tensor? mask=None, Tensor? bias=None, "
                   "int[3] stride=1, int[3] padding=0, int[3] dilation=1, int groups=1) -> Tensor",
```

### Comparing `tvdcn-0.3.0/tvdcn/csrc/ops/deform_conv_transpose1d.cpp` & `tvdcn-0.3.1/tvdcn/csrc/ops/deform_conv_transpose1d.cpp`

 * *Files 5% similar despite different names*

```diff
@@ -66,42 +66,45 @@
 // modified from
 // https://github.com/open-mmlab/mmdetection/blob/master/mmdet/ops/dcn/src/deform_conv_cuda.cpp
 
 // modified from
 // https://github.com/pytorch/vision/blob/master/torchvision/csrc/cpu/deform_conv2d_kernel.cpp
 
 #include <torch/autograd.h>
-#include "utils/parallel_helpers.h"
+
 #include "dispatch/deform_conv1d_kernels.h"
+#include "utils/parallel_helpers.h"
+#include "utils/tensor_utils.h"
 
 namespace tvdcn {
     namespace ops {
         at::Tensor deform_conv_transpose1d_forward(
                 const at::Tensor &input,
                 const at::Tensor &weight,
                 const at::Tensor &offset,
                 const at::Tensor &mask,
                 const at::Tensor &bias,
                 at::IntArrayRef stride,
                 at::IntArrayRef padding,
                 at::IntArrayRef output_padding,
                 at::IntArrayRef dilation,
-                int64_t groups,
-                bool deformable,
-                bool modulated) {
+                int64_t groups) {
             at::CheckedFrom c = "deform_conv_transpose2d_forward";
             auto args = {
                     at::TensorArg(input, "input", 1),
                     at::TensorArg(weight, "weight", 2),
                     at::TensorArg(offset, "offset", 3),
                     at::TensorArg(mask, "mask", 4),
                     at::TensorArg(bias, "bias", 5)};
             at::checkAllSameType(c, args);
-            if (input.device().is_cuda())
-                at::checkAllSameGPU(c, args);
+            at::checkAllSameDevice(c, args);
+
+            bool deformable = offset.defined() && offset.numel();
+            bool modulated = mask.defined() && mask.numel();
+            bool with_bias = bias.defined() && bias.numel();
 
             at::Tensor input_c = input.contiguous();
             at::Tensor weight_c = weight.contiguous();
             at::Tensor offset_c = offset.contiguous();
             at::Tensor mask_c = mask.contiguous();
             at::Tensor bias_c = bias.contiguous();
 
@@ -133,66 +136,74 @@
                     weight_w > 0,
                     " weight_w: ",
                     weight_w)
             TORCH_CHECK(
                     stride_w > 0,
                     " stride_w: ",
                     stride_w)
-            TORCH_CHECK(pad_w >= 0, " pad_w: ", pad_w)
-            TORCH_CHECK(dilation_w > 0, " dilation_w: ", dilation_w)
+            TORCH_CHECK(
+                    pad_w >= 0,
+                    " pad_w: ",
+                    pad_w)
+            TORCH_CHECK(
+                    dilation_w > 0,
+                    " dilation_w: ",
+                    dilation_w)
 
             TORCH_CHECK(weight_c.size(1) * groups == out_channels)
             TORCH_CHECK(weight_c.size(0) % groups == 0)
 
-            int64_t offset_groups = offset.size(1) / weight_w;
-            int64_t mask_groups = mask.size(1) / weight_w;
+            int64_t offset_groups = deformable ? offset.size(1) / weight_w : 0;
+            int64_t mask_groups = modulated ? mask.size(1) / weight_w : 0;
 
-            TORCH_CHECK(!deformable || offset_groups > 0,
-                        "The shape of the offset tensor at dimension 1 is not valid. It should "
-                        "be a multiple of weight.size(2).\nGot offset.size(1)=",
-                        offset.size(1),
-                        ", while weight.size(2)=",
-                        weight_w)
+            TORCH_CHECK(
+                    !deformable || offset_c.size(0) == input_c.size(0),
+                    "invalid batch size of offset")
+            TORCH_CHECK(
+                    !deformable || offset_groups > 0,
+                    "The shape of the offset tensor at dimension 1 is not valid. It should "
+                    "be a multiple of weight.size(2).\nGot offset.size(1)=",
+                    offset.size(1),
+                    ", while weight.size(2)=",
+                    weight_w)
             TORCH_CHECK(!deformable || input_c.size(1) % offset_groups == 0)
-
-            TORCH_CHECK(!modulated || mask_groups > 0,
-                        "The shape of the mask tensor at dimension 1 is not valid. It should "
-                        "be a multiple of weight.size(2).\nGot mask.size(1)=",
-                        mask.size(1),
-                        ", while weight.size(2)=",
-                        weight_w)
-            TORCH_CHECK(!modulated || input_c.size(1) % mask_groups == 0)
-
             TORCH_CHECK(
-                    (!deformable || offset_c.size(1) == offset_groups * weight_w),
+                    !deformable || offset_c.size(1) == offset_groups * weight_w,
                     "offset.shape[1] is not valid. got: ",
                     offset_c.size(1),
                     " expected: ",
                     offset_groups * weight_w)
             TORCH_CHECK(
-                    (offset_c.size(0) == input_c.size(0)), "invalid batch size of offset")
-            TORCH_CHECK(
-                    (!deformable || offset_c.size(2) == in_w),
+                    !deformable || offset_c.size(2) == in_w,
                     "offset output dims: (",
                     offset_c.size(2),
                     ") - ",
                     "input dims: (",
                     in_w,
                     ")")
 
             TORCH_CHECK(
-                    (!modulated || mask_c.size(1) == mask_groups * weight_w),
+                    !modulated || mask_c.size(0) == input_c.size(0),
+                    "invalid batch size of mask")
+            TORCH_CHECK(
+                    !modulated || mask_groups > 0,
+                    "The shape of the mask tensor at dimension 1 is not valid. It should "
+                    "be a multiple of weight.size(2).\nGot mask.size(1)=",
+                    mask.size(1),
+                    ", while weight.size(2)=",
+                    weight_w)
+            TORCH_CHECK(!modulated || input_c.size(1) % mask_groups == 0)
+            TORCH_CHECK(
+                    !modulated || mask_c.size(1) == mask_groups * weight_w,
                     "mask.shape[1] is not valid. got: ",
                     mask_c.size(1),
                     " expected: ",
                     mask_groups * weight_w)
             TORCH_CHECK(
-                    (mask_c.size(0) == input_c.size(0)), "invalid batch size of mask")
-            TORCH_CHECK(
-                    (!modulated || mask_c.size(2) == in_w),
+                    !modulated || mask_c.size(2) == in_w,
                     "mask output dims: (",
                     mask_c.size(2),
                     ") - ",
                     "input dims: (",
                     in_w,
                     ")")
 
@@ -273,16 +284,18 @@
                         mask_groups,
                         deformable,
                         modulated,
                         output_b);
             }
 
             output = output.view({batch_sz, out_channels, out_w});
+            if (with_bias)
+                output.add_(bias_c.view({1, out_channels, 1}));
 
-            return output + bias_c.view({1, out_channels, 1});
+            return output;
         }
 
         namespace detail {
             std::tuple<at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor>
             _deform_conv_transpose1d_backward(
                     const at::Tensor &grad_out,
                     const at::Tensor &input,
@@ -290,17 +303,19 @@
                     const at::Tensor &offset,
                     const at::Tensor &mask,
                     const at::Tensor &bias,
                     at::IntArrayRef stride,
                     at::IntArrayRef padding,
                     at::IntArrayRef output_padding,
                     at::IntArrayRef dilation,
-                    int64_t groups,
-                    bool deformable,
-                    bool modulated) {
+                    int64_t groups) {
+                bool deformable = offset.defined() && offset.numel();
+                bool modulated = mask.defined() && mask.numel();
+                bool with_bias = bias.defined() && bias.numel();
+
                 at::Tensor grad_out_c = grad_out.contiguous();
                 at::Tensor input_c = input.contiguous();
                 at::Tensor weight_c = weight.contiguous();
                 at::Tensor offset_c = offset.contiguous();
                 at::Tensor mask_c = mask.contiguous();
                 at::Tensor bias_c = bias.contiguous();
 
@@ -319,22 +334,22 @@
 
                 int64_t out_pad_w = output_padding[0];
 
                 int64_t dilation_w = dilation[0];
 
                 int64_t out_w = (in_w - 1) * stride_w - 2 * pad_w + dilation_w * (weight_w - 1) + 1 + out_pad_w;
 
-                int64_t offset_groups = offset.size(1) / weight_w;
-                int64_t mask_groups = mask.size(1) / weight_w;
+                int64_t offset_groups = deformable ? offset.size(1) / weight_w : 0;
+                int64_t mask_groups = modulated ? mask.size(1) / weight_w : 0;
 
                 auto grad_input = at::zeros_like(input_c);
                 auto grad_weight = at::zeros_like(weight_c);
                 auto grad_offset = at::zeros_like(offset_c);
                 auto grad_mask = at::zeros_like(mask_c);
-                auto grad_bias = at::ones_like(bias_c);
+                auto grad_bias = with_bias ? grad_out_c.sum(at::IntArrayRef({0, 2})) : at::zeros_like(bias_c);
 
                 // Separate into blocks
                 grad_out_c = grad_out_c.view({batch_sz / n_parallel_imgs,
                                               n_parallel_imgs,
                                               out_channels,
                                               out_w});
 
@@ -474,15 +489,14 @@
                                                       in_w}).transpose_(1, 2);
                 grad_input.copy_(grad_input_buf);
 
                 grad_input = grad_input.view_as(input);
                 grad_weight = grad_weight.view_as(weight);
                 grad_offset = grad_offset.view_as(offset);
                 grad_mask = grad_mask.view_as(mask);
-                grad_bias *= grad_out.sum(at::IntArrayRef({0, 2}));
 
                 return std::make_tuple(grad_input, grad_weight, grad_offset, grad_mask, grad_bias);
             }
         }
 
         class DeformConvTranspose1dFunction
                 : public torch::autograd::Function<DeformConvTranspose1dFunction> {
@@ -494,40 +508,34 @@
                     const torch::autograd::Variable &offset,
                     const torch::autograd::Variable &mask,
                     const torch::autograd::Variable &bias,
                     at::IntArrayRef stride,
                     at::IntArrayRef padding,
                     at::IntArrayRef output_padding,
                     at::IntArrayRef dilation,
-                    int64_t groups,
-                    bool deformable,
-                    bool modulated) {
+                    int64_t groups) {
                 at::AutoDispatchBelowADInplaceOrView g;
                 auto output = deform_conv_transpose1d_forward(
                         input,
                         weight,
                         offset,
                         mask,
                         bias,
                         stride,
                         padding,
                         output_padding,
                         dilation,
-                        groups,
-                        deformable,
-                        modulated);
+                        groups);
 
                 ctx->save_for_backward({input, weight, offset, mask, bias});
                 ctx->saved_data["stride"] = stride.vec();
                 ctx->saved_data["padding"] = padding.vec();
                 ctx->saved_data["output_padding"] = output_padding.vec();
                 ctx->saved_data["dilation"] = dilation.vec();
                 ctx->saved_data["groups"] = groups;
-                ctx->saved_data["deformable"] = deformable;
-                ctx->saved_data["modulated"] = modulated;
 
                 return {
                         output,
                 };
             }
 
             static torch::autograd::variable_list backward(
@@ -541,31 +549,27 @@
                 auto bias = saved[4];
 
                 auto stride = ctx->saved_data["stride"].toIntVector();
                 auto padding = ctx->saved_data["padding"].toIntVector();
                 auto output_padding = ctx->saved_data["output_padding"].toIntVector();
                 auto dilation = ctx->saved_data["dilation"].toIntVector();
                 auto groups = ctx->saved_data["groups"].toInt();
-                auto deformable = ctx->saved_data["deformable"].toBool();
-                auto modulated = ctx->saved_data["modulated"].toBool();
 
                 auto grads = detail::_deform_conv_transpose1d_backward(
                         grad_output[0],
                         input,
                         weight,
                         offset,
                         mask,
                         bias,
                         stride,
                         padding,
                         output_padding,
                         dilation,
-                        groups,
-                        deformable,
-                        modulated);
+                        groups);
                 auto grad_input = std::get<0>(grads);
                 auto grad_weight = std::get<1>(grads);
                 auto grad_offset = std::get<2>(grads);
                 auto grad_mask = std::get<3>(grads);
                 auto grad_bias = std::get<4>(grads);
 
                 return {
@@ -575,16 +579,14 @@
                         grad_mask,
                         grad_bias,
                         torch::autograd::Variable(),
                         torch::autograd::Variable(),
                         torch::autograd::Variable(),
                         torch::autograd::Variable(),
                         torch::autograd::Variable(),
-                        torch::autograd::Variable(),
-                        torch::autograd::Variable(),
                 };
             }
         };
 
         at::Tensor deform_conv_transpose1d(
                 const at::Tensor &input,
                 const at::Tensor &weight,
@@ -592,28 +594,26 @@
                 const at::optional<at::Tensor> &mask = {},
                 const at::optional<at::Tensor> &bias = {},
                 at::IntArrayRef stride = 1,
                 at::IntArrayRef padding = 0,
                 at::IntArrayRef output_padding = 0,
                 at::IntArrayRef dilation = 1,
                 int64_t groups = 1) {
-            C10_LOG_API_USAGE_ONCE("tvdcn.csrc.ops.deform_conv_transpose.deform_conv_transpose1d");
+            C10_LOG_API_USAGE_ONCE("tvdcn.csrc.ops.deform_conv_transpose.deform_conv_transpose1d")
             auto result = DeformConvTranspose1dFunction::apply(
                     input,
                     weight,
-                    offset.value_or(at::zeros({input.size(0), 0}, input.options().requires_grad(false))),
-                    mask.value_or(at::zeros({input.size(0), 0}, input.options().requires_grad(false))),
-                    bias.value_or(at::zeros({weight.size(0)}, input.options().requires_grad(false))),
+                    offset.value_or(input.new_zeros(0)),
+                    mask.value_or(input.new_zeros(0)),
+                    bias.value_or(input.new_zeros(0)),
                     stride,
                     padding,
                     output_padding,
                     dilation,
-                    groups,
-                    offset.has_value(),
-                    mask.has_value());
+                    groups);
             return result[0];
         }
 
         TORCH_LIBRARY_FRAGMENT(tvdcn, m) {
             m.def("tvdcn::deform_conv_transpose1d(Tensor input, Tensor weight, "
                   "Tensor? offset=None, Tensor? mask=None, Tensor? bias=None, "
                   "int[1] stride=1, int[1] padding=0, int[1] output_padding=0, "
```

### Comparing `tvdcn-0.3.0/tvdcn/csrc/ops/deform_conv_transpose2d.cpp` & `tvdcn-0.3.1/tvdcn/csrc/ops/deform_conv_transpose2d.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -66,42 +66,45 @@
 // modified from
 // https://github.com/open-mmlab/mmdetection/blob/master/mmdet/ops/dcn/src/deform_conv_cuda.cpp
 
 // modified from
 // https://github.com/pytorch/vision/blob/master/torchvision/csrc/cpu/deform_conv2d_kernel.cpp
 
 #include <torch/autograd.h>
-#include "utils/parallel_helpers.h"
+
 #include "dispatch/deform_conv2d_kernels.h"
+#include "utils/parallel_helpers.h"
+#include "utils/tensor_utils.h"
 
 namespace tvdcn {
     namespace ops {
         at::Tensor deform_conv_transpose2d_forward(
                 const at::Tensor &input,
                 const at::Tensor &weight,
                 const at::Tensor &offset,
                 const at::Tensor &mask,
                 const at::Tensor &bias,
                 at::IntArrayRef stride,
                 at::IntArrayRef padding,
                 at::IntArrayRef output_padding,
                 at::IntArrayRef dilation,
-                int64_t groups,
-                bool deformable,
-                bool modulated) {
+                int64_t groups) {
             at::CheckedFrom c = "deform_conv_transpose2d_forward";
             auto args = {
                     at::TensorArg(input, "input", 1),
                     at::TensorArg(weight, "weight", 2),
                     at::TensorArg(offset, "offset", 3),
                     at::TensorArg(mask, "mask", 4),
                     at::TensorArg(bias, "bias", 5)};
             at::checkAllSameType(c, args);
-            if (input.device().is_cuda())
-                at::checkAllSameGPU(c, args);
+            at::checkAllSameDevice(c, args);
+
+            bool deformable = offset.defined() && offset.numel();
+            bool modulated = mask.defined() && mask.numel();
+            bool with_bias = bias.defined() && bias.numel();
 
             at::Tensor input_c = input.contiguous();
             at::Tensor weight_c = weight.contiguous();
             at::Tensor offset_c = offset.contiguous();
             at::Tensor mask_c = mask.contiguous();
             at::Tensor bias_c = bias.contiguous();
 
@@ -144,72 +147,84 @@
                     weight_w)
             TORCH_CHECK(
                     stride_h > 0 && stride_w > 0,
                     "stride_h: ",
                     stride_h,
                     " stride_w: ",
                     stride_w)
-            TORCH_CHECK(pad_h >= 0 && pad_w >= 0, "pad_h: ", pad_h, " pad_w: ", pad_w)
-            TORCH_CHECK(dilation_h > 0 && dilation_w > 0, "dilation_h: ", dilation_h, " dilation_w: ", dilation_w)
+            TORCH_CHECK(
+                    pad_h >= 0 && pad_w >= 0,
+                    "pad_h: ",
+                    pad_h,
+                    " pad_w: ",
+                    pad_w)
+            TORCH_CHECK(
+                    dilation_h > 0 && dilation_w > 0,
+                    "dilation_h: ",
+                    dilation_h,
+                    " dilation_w: ",
+                    dilation_w)
 
             TORCH_CHECK(weight_c.size(1) * groups == out_channels)
             TORCH_CHECK(weight_c.size(0) % groups == 0)
 
-            int64_t offset_groups = offset.size(1) / (2 * weight_h * weight_w);
-            int64_t mask_groups = mask.size(1) / (weight_h * weight_w);
+            int64_t offset_groups = deformable ? offset.size(1) / (2 * weight_h * weight_w) : 0;
+            int64_t mask_groups = modulated ? mask.size(1) / (weight_h * weight_w) : 0;
 
-            TORCH_CHECK(!deformable || offset_groups > 0,
-                        "The shape of the offset tensor at dimension 1 is not valid. It should "
-                        "be a multiple of 2 * weight.size(2) * weight.size(3).\nGot offset.size(1)=",
-                        offset.size(1),
-                        ", while 2 * weight.size(2) * weight.size(3)=",
-                        2 * weight_h * weight_w)
+            TORCH_CHECK(
+                    !deformable || offset_c.size(0) == input_c.size(0),
+                    "invalid batch size of offset")
+            TORCH_CHECK(
+                    !deformable || offset_groups > 0,
+                    "The shape of the offset tensor at dimension 1 is not valid. It should "
+                    "be a multiple of 2 * weight.size(2) * weight.size(3).\nGot offset.size(1)=",
+                    offset.size(1),
+                    ", while 2 * weight.size(2) * weight.size(3)=",
+                    2 * weight_h * weight_w)
             TORCH_CHECK(!deformable || input_c.size(1) % offset_groups == 0)
-
-            TORCH_CHECK(!modulated || mask_groups > 0,
-                        "The shape of the mask tensor at dimension 1 is not valid. It should "
-                        "be a multiple of weight.size(2) * weight.size(3).\nGot mask.size(1)=",
-                        mask.size(1),
-                        ", while weight.size(2) * weight.size(3)=",
-                        weight_h * weight_w)
-            TORCH_CHECK(!modulated || input_c.size(1) % mask_groups == 0)
-
             TORCH_CHECK(
-                    (!deformable || offset_c.size(1) == offset_groups * 2 * weight_h * weight_w),
+                    !deformable || offset_c.size(1) == offset_groups * 2 * weight_h * weight_w,
                     "offset.shape[1] is not valid. got: ",
                     offset_c.size(1),
                     " expected: ",
                     offset_groups * 2 * weight_h * weight_w)
             TORCH_CHECK(
-                    (offset_c.size(0) == input_c.size(0)), "invalid batch size of offset")
-            TORCH_CHECK(
-                    (!deformable || (offset_c.size(2) == in_h &&
-                                     offset_c.size(3) == in_w)),
+                    !deformable || (offset_c.size(2) == in_h &&
+                                    offset_c.size(3) == in_w),
                     "offset input dims: (",
                     offset_c.size(2),
                     ", ",
                     offset_c.size(3),
                     ") - ",
                     "input dims: (",
                     in_h,
                     ", ",
                     in_w,
                     ")")
 
             TORCH_CHECK(
-                    (!modulated || mask_c.size(1) == mask_groups * weight_h * weight_w),
+                    !modulated || mask_c.size(0) == input_c.size(0),
+                    "invalid batch size of mask")
+            TORCH_CHECK(
+                    !modulated || mask_groups > 0,
+                    "The shape of the mask tensor at dimension 1 is not valid. It should "
+                    "be a multiple of weight.size(2) * weight.size(3).\nGot mask.size(1)=",
+                    mask.size(1),
+                    ", while weight.size(2) * weight.size(3)=",
+                    weight_h * weight_w)
+            TORCH_CHECK(!modulated || input_c.size(1) % mask_groups == 0)
+            TORCH_CHECK(
+                    !modulated || mask_c.size(1) == mask_groups * weight_h * weight_w,
                     "mask.shape[1] is not valid. got: ",
                     mask_c.size(1),
                     " expected: ",
                     mask_groups * weight_h * weight_w)
             TORCH_CHECK(
-                    (mask_c.size(0) == input_c.size(0)), "invalid batch size of mask")
-            TORCH_CHECK(
-                    (!modulated || (mask_c.size(2) == in_h &&
-                                    mask_c.size(3) == in_w)),
+                    !modulated || (mask_c.size(2) == in_h &&
+                                   mask_c.size(3) == in_w),
                     "mask input dims: (",
                     mask_c.size(2),
                     ", ",
                     mask_c.size(3),
                     ") - ",
                     "input dims: (",
                     in_h,
@@ -311,16 +326,18 @@
                         mask_groups,
                         deformable,
                         modulated,
                         output_b);
             }
 
             output = output.view({batch_sz, out_channels, out_h, out_w});
+            if (with_bias)
+                output.add_(bias_c.view({1, out_channels, 1, 1}));
 
-            return output + bias_c.view({1, out_channels, 1, 1});
+            return output;
         }
 
         namespace detail {
             std::tuple<at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor>
             _deform_conv_transpose2d_backward(
                     const at::Tensor &grad_out,
                     const at::Tensor &input,
@@ -328,17 +345,19 @@
                     const at::Tensor &offset,
                     const at::Tensor &mask,
                     const at::Tensor &bias,
                     at::IntArrayRef stride,
                     at::IntArrayRef padding,
                     at::IntArrayRef output_padding,
                     at::IntArrayRef dilation,
-                    int64_t groups,
-                    bool deformable,
-                    bool modulated) {
+                    int64_t groups) {
+                bool deformable = offset.defined() && offset.numel();
+                bool modulated = mask.defined() && mask.numel();
+                bool with_bias = bias.defined() && bias.numel();
+
                 at::Tensor grad_out_c = grad_out.contiguous();
                 at::Tensor input_c = input.contiguous();
                 at::Tensor weight_c = weight.contiguous();
                 at::Tensor offset_c = offset.contiguous();
                 at::Tensor mask_c = mask.contiguous();
                 at::Tensor bias_c = bias.contiguous();
 
@@ -364,22 +383,22 @@
 
                 int64_t dilation_h = dilation[0];
                 int64_t dilation_w = dilation[1];
 
                 int64_t out_h = (in_h - 1) * stride_h - 2 * pad_h + dilation_h * (weight_h - 1) + 1 + out_pad_h;
                 int64_t out_w = (in_w - 1) * stride_w - 2 * pad_w + dilation_w * (weight_w - 1) + 1 + out_pad_w;
 
-                int64_t offset_groups = offset.size(1) / (2 * weight_h * weight_w);
-                int64_t mask_groups = mask.size(1) / (weight_h * weight_w);
+                int64_t offset_groups = deformable ? offset.size(1) / (2 * weight_h * weight_w) : 0;
+                int64_t mask_groups = modulated ? mask.size(1) / (weight_h * weight_w) : 0;
 
                 auto grad_input = at::zeros_like(input_c);
                 auto grad_weight = at::zeros_like(weight_c);
                 auto grad_offset = at::zeros_like(offset_c);
                 auto grad_mask = at::zeros_like(mask_c);
-                auto grad_bias = at::ones_like(bias_c);
+                auto grad_bias = with_bias ? grad_out_c.sum(at::IntArrayRef({0, 2, 3})) : at::zeros_like(bias_c);
 
                 // Separate into blocks
                 grad_out_c = grad_out_c.view({batch_sz / n_parallel_imgs,
                                               n_parallel_imgs,
                                               out_channels,
                                               out_h,
                                               out_w});
@@ -550,15 +569,14 @@
                                                       in_w}).transpose_(1, 2);
                 grad_input.copy_(grad_input_buf);
 
                 grad_input = grad_input.view_as(input);
                 grad_weight = grad_weight.view_as(weight);
                 grad_offset = grad_offset.view_as(offset);
                 grad_mask = grad_mask.view_as(mask);
-                grad_bias *= grad_out.sum(at::IntArrayRef({0, 2, 3}));
 
                 return std::make_tuple(grad_input, grad_weight, grad_offset, grad_mask, grad_bias);
             }
         }
 
         class DeformConvTranspose2dFunction
                 : public torch::autograd::Function<DeformConvTranspose2dFunction> {
@@ -570,40 +588,34 @@
                     const torch::autograd::Variable &offset,
                     const torch::autograd::Variable &mask,
                     const torch::autograd::Variable &bias,
                     at::IntArrayRef stride,
                     at::IntArrayRef padding,
                     at::IntArrayRef output_padding,
                     at::IntArrayRef dilation,
-                    int64_t groups,
-                    bool deformable,
-                    bool modulated) {
+                    int64_t groups) {
                 at::AutoDispatchBelowADInplaceOrView g;
                 auto output = deform_conv_transpose2d_forward(
                         input,
                         weight,
                         offset,
                         mask,
                         bias,
                         stride,
                         padding,
                         output_padding,
                         dilation,
-                        groups,
-                        deformable,
-                        modulated);
+                        groups);
 
                 ctx->save_for_backward({input, weight, offset, mask, bias});
                 ctx->saved_data["stride"] = stride.vec();
                 ctx->saved_data["padding"] = padding.vec();
                 ctx->saved_data["output_padding"] = output_padding.vec();
                 ctx->saved_data["dilation"] = dilation.vec();
                 ctx->saved_data["groups"] = groups;
-                ctx->saved_data["deformable"] = deformable;
-                ctx->saved_data["modulated"] = modulated;
 
                 return {
                         output,
                 };
             }
 
             static torch::autograd::variable_list backward(
@@ -617,31 +629,27 @@
                 auto bias = saved[4];
 
                 auto stride = ctx->saved_data["stride"].toIntVector();
                 auto padding = ctx->saved_data["padding"].toIntVector();
                 auto output_padding = ctx->saved_data["output_padding"].toIntVector();
                 auto dilation = ctx->saved_data["dilation"].toIntVector();
                 auto groups = ctx->saved_data["groups"].toInt();
-                auto deformable = ctx->saved_data["deformable"].toBool();
-                auto modulated = ctx->saved_data["modulated"].toBool();
 
                 auto grads = detail::_deform_conv_transpose2d_backward(
                         grad_output[0],
                         input,
                         weight,
                         offset,
                         mask,
                         bias,
                         stride,
                         padding,
                         output_padding,
                         dilation,
-                        groups,
-                        deformable,
-                        modulated);
+                        groups);
                 auto grad_input = std::get<0>(grads);
                 auto grad_weight = std::get<1>(grads);
                 auto grad_offset = std::get<2>(grads);
                 auto grad_mask = std::get<3>(grads);
                 auto grad_bias = std::get<4>(grads);
 
                 return {
@@ -651,16 +659,14 @@
                         grad_mask,
                         grad_bias,
                         torch::autograd::Variable(),
                         torch::autograd::Variable(),
                         torch::autograd::Variable(),
                         torch::autograd::Variable(),
                         torch::autograd::Variable(),
-                        torch::autograd::Variable(),
-                        torch::autograd::Variable(),
                 };
             }
         };
 
         at::Tensor deform_conv_transpose2d(
                 const at::Tensor &input,
                 const at::Tensor &weight,
@@ -668,28 +674,26 @@
                 const at::optional<at::Tensor> &mask = {},
                 const at::optional<at::Tensor> &bias = {},
                 at::IntArrayRef stride = 1,
                 at::IntArrayRef padding = 0,
                 at::IntArrayRef output_padding = 0,
                 at::IntArrayRef dilation = 1,
                 int64_t groups = 1) {
-            C10_LOG_API_USAGE_ONCE("tvdcn.csrc.ops.deform_conv_transpose.deform_conv_transpose2d");
+            C10_LOG_API_USAGE_ONCE("tvdcn.csrc.ops.deform_conv_transpose.deform_conv_transpose2d")
             auto result = DeformConvTranspose2dFunction::apply(
                     input,
                     weight,
-                    offset.value_or(at::zeros({input.size(0), 0}, input.options().requires_grad(false))),
-                    mask.value_or(at::zeros({input.size(0), 0}, input.options().requires_grad(false))),
-                    bias.value_or(at::zeros({weight.size(0)}, input.options().requires_grad(false))),
+                    offset.value_or(input.new_zeros(0)),
+                    mask.value_or(input.new_zeros(0)),
+                    bias.value_or(input.new_zeros(0)),
                     stride,
                     padding,
                     output_padding,
                     dilation,
-                    groups,
-                    offset.has_value(),
-                    mask.has_value());
+                    groups);
             return result[0];
         }
 
         TORCH_LIBRARY_FRAGMENT(tvdcn, m) {
             m.def("tvdcn::deform_conv_transpose2d(Tensor input, Tensor weight, "
                   "Tensor? offset=None, Tensor? mask=None, Tensor? bias=None, "
                   "int[2] stride=1, int[2] padding=0, int[2] output_padding=0, "
```

### Comparing `tvdcn-0.3.0/tvdcn/csrc/ops/deform_conv_transpose3d.cpp` & `tvdcn-0.3.1/tvdcn/csrc/ops/deform_conv_transpose3d.cpp`

 * *Files 6% similar despite different names*

```diff
@@ -66,42 +66,45 @@
 // modified from
 // https://github.com/open-mmlab/mmdetection/blob/master/mmdet/ops/dcn/src/deform_conv_cuda.cpp
 
 // modified from
 // https://github.com/pytorch/vision/blob/master/torchvision/csrc/cpu/deform_conv2d_kernel.cpp
 
 #include <torch/autograd.h>
-#include "utils/parallel_helpers.h"
+
 #include "dispatch/deform_conv3d_kernels.h"
+#include "utils/parallel_helpers.h"
+#include "utils/tensor_utils.h"
 
 namespace tvdcn {
     namespace ops {
         at::Tensor deform_conv_transpose3d_forward(
                 const at::Tensor &input,
                 const at::Tensor &weight,
                 const at::Tensor &offset,
                 const at::Tensor &mask,
                 const at::Tensor &bias,
                 at::IntArrayRef stride,
                 at::IntArrayRef padding,
                 at::IntArrayRef output_padding,
                 at::IntArrayRef dilation,
-                int64_t groups,
-                bool deformable,
-                bool modulated) {
+                int64_t groups) {
             at::CheckedFrom c = "deform_conv_transpose3d_forward";
             auto args = {
                     at::TensorArg(input, "input", 1),
                     at::TensorArg(weight, "weight", 2),
                     at::TensorArg(offset, "offset", 3),
                     at::TensorArg(mask, "mask", 4),
                     at::TensorArg(bias, "bias", 5)};
             at::checkAllSameType(c, args);
-            if (input.device().is_cuda())
-                at::checkAllSameGPU(c, args);
+            at::checkAllSameDevice(c, args);
+
+            bool deformable = offset.defined() && offset.numel();
+            bool modulated = mask.defined() && mask.numel();
+            bool with_bias = bias.defined() && bias.numel();
 
             at::Tensor input_c = input.contiguous();
             at::Tensor weight_c = weight.contiguous();
             at::Tensor offset_c = offset.contiguous();
             at::Tensor mask_c = mask.contiguous();
             at::Tensor bias_c = bias.contiguous();
 
@@ -155,52 +158,58 @@
                     stride_d > 0 && stride_h > 0 && stride_w > 0,
                     " stride_d: ",
                     stride_d,
                     "stride_h: ",
                     stride_h,
                     " stride_w: ",
                     stride_w)
-            TORCH_CHECK(pad_d >= 0 && pad_h >= 0 && pad_w >= 0, "pad_d: ", pad_d, " pad_h: ", pad_h, " pad_w: ", pad_w)
-            TORCH_CHECK(dilation_d > 0 && dilation_h > 0 && dilation_w > 0, "dilation_d: ", dilation_d, " dilation_h: ",
-                        dilation_h, " dilation_w: ", dilation_w)
+            TORCH_CHECK(
+                    pad_d >= 0 && pad_h >= 0 && pad_w >= 0,
+                    "pad_d: ",
+                    pad_d,
+                    " pad_h: ",
+                    pad_h,
+                    " pad_w: ",
+                    pad_w)
+            TORCH_CHECK(
+                    dilation_d > 0 && dilation_h > 0 && dilation_w > 0,
+                    "dilation_d: ",
+                    dilation_d,
+                    " dilation_h: ",
+                    dilation_h,
+                    " dilation_w: ",
+                    dilation_w)
 
             TORCH_CHECK(weight_c.size(1) * groups == out_channels)
             TORCH_CHECK(weight_c.size(0) % groups == 0)
 
-            int64_t offset_groups = offset.size(1) / (3 * weight_d * weight_h * weight_w);
-            int64_t mask_groups = mask.size(1) / (weight_d * weight_h * weight_w);
+            int64_t offset_groups = deformable ? offset.size(1) / (3 * weight_d * weight_h * weight_w) : 0;
+            int64_t mask_groups = modulated ? mask.size(1) / (weight_d * weight_h * weight_w) : 0;
 
-            TORCH_CHECK(!deformable || offset_groups > 0,
-                        "The shape of the offset tensor at dimension 1 is not valid. It should "
-                        "be a multiple of 3 * weight.size(2) * weight.size(3) * weight.size(4).\nGot offset.size(1)=",
-                        offset.size(1),
-                        ", while 3 * weight.size(2) * weight.size(3) * weight.size(3)=",
-                        3 * weight_d * weight_h * weight_w)
+            TORCH_CHECK(
+                    !deformable || offset_c.size(0) == input_c.size(0),
+                    "invalid batch size of offset")
+            TORCH_CHECK(
+                    !deformable || offset_groups > 0,
+                    "The shape of the offset tensor at dimension 1 is not valid. It should "
+                    "be a multiple of 3 * weight.size(2) * weight.size(3) * weight.size(4).\nGot offset.size(1)=",
+                    offset.size(1),
+                    ", while 3 * weight.size(2) * weight.size(3) * weight.size(3)=",
+                    3 * weight_d * weight_h * weight_w)
             TORCH_CHECK(!deformable || input_c.size(1) % offset_groups == 0)
-
-            TORCH_CHECK(!modulated || mask_groups > 0,
-                        "The shape of the mask tensor at dimension 1 is not valid. It should "
-                        "be a multiple of weight.size(2) * weight.size(3) * weight.size(4).\nGot mask.size(1)=",
-                        mask.size(1),
-                        ", while weight.size(2) * weight.size(3) * weight.size(4)=",
-                        weight_d * weight_h * weight_w)
-            TORCH_CHECK(!modulated || input_c.size(1) % mask_groups == 0)
-
             TORCH_CHECK(
-                    (!deformable || offset_c.size(1) == offset_groups * 3 * weight_d * weight_h * weight_w),
+                    !deformable || offset_c.size(1) == offset_groups * 3 * weight_d * weight_h * weight_w,
                     "offset.shape[1] is not valid. got: ",
                     offset_c.size(1),
                     " expected: ",
                     offset_groups * 3 * weight_d * weight_h * weight_w)
             TORCH_CHECK(
-                    (offset_c.size(0) == input_c.size(0)), "invalid batch size of offset")
-            TORCH_CHECK(
-                    (!deformable || (offset_c.size(2) == in_d &&
-                                     offset_c.size(3) == in_h &&
-                                     offset_c.size(4) == in_w)),
+                    !deformable || (offset_c.size(2) == in_d &&
+                                    offset_c.size(3) == in_h &&
+                                    offset_c.size(4) == in_w),
                     "offset input dims: (",
                     offset_c.size(2),
                     ", ",
                     offset_c.size(3),
                     ", ",
                     offset_c.size(4),
                     ") - ",
@@ -209,25 +218,34 @@
                     ", ",
                     in_h,
                     ", ",
                     in_w,
                     ")")
 
             TORCH_CHECK(
-                    (!modulated || mask_c.size(1) == mask_groups * weight_d * weight_h * weight_w),
+                    !modulated || mask_c.size(0) == input_c.size(0),
+                    "invalid batch size of mask")
+            TORCH_CHECK(
+                    !modulated || mask_groups > 0,
+                    "The shape of the mask tensor at dimension 1 is not valid. It should "
+                    "be a multiple of weight.size(2) * weight.size(3) * weight.size(4).\nGot mask.size(1)=",
+                    mask.size(1),
+                    ", while weight.size(2) * weight.size(3) * weight.size(4)=",
+                    weight_d * weight_h * weight_w)
+            TORCH_CHECK(!modulated || input_c.size(1) % mask_groups == 0)
+            TORCH_CHECK(
+                    !modulated || mask_c.size(1) == mask_groups * weight_d * weight_h * weight_w,
                     "mask.shape[1] is not valid. got: ",
                     mask_c.size(1),
                     " expected: ",
                     mask_groups * weight_d * weight_h * weight_w)
             TORCH_CHECK(
-                    (mask_c.size(0) == input_c.size(0)), "invalid batch size of mask")
-            TORCH_CHECK(
-                    (!modulated || (mask_c.size(2) == in_d &&
-                                    mask_c.size(3) == in_h &&
-                                    mask_c.size(4) == in_w)),
+                    !modulated || (mask_c.size(2) == in_d &&
+                                   mask_c.size(3) == in_h &&
+                                   mask_c.size(4) == in_w),
                     "mask input dims: (",
                     mask_c.size(2),
                     ", ",
                     mask_c.size(3),
                     ", ",
                     mask_c.size(4),
                     ") - ",
@@ -350,16 +368,18 @@
                         mask_groups,
                         deformable,
                         modulated,
                         output_b);
             }
 
             output = output.view({batch_sz, out_channels, out_d, out_h, out_w});
+            if (with_bias)
+                output.add_(bias_c.view({1, out_channels, 1, 1, 1}));
 
-            return output + bias_c.view({1, out_channels, 1, 1, 1});
+            return output;
         }
 
         namespace detail {
             std::tuple<at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor>
             _deform_conv_transpose3d_backward(
                     const at::Tensor &grad_out,
                     const at::Tensor &input,
@@ -367,17 +387,19 @@
                     const at::Tensor &offset,
                     const at::Tensor &mask,
                     const at::Tensor &bias,
                     at::IntArrayRef stride,
                     at::IntArrayRef padding,
                     at::IntArrayRef output_padding,
                     at::IntArrayRef dilation,
-                    int64_t groups,
-                    bool deformable,
-                    bool modulated) {
+                    int64_t groups) {
+                bool deformable = offset.defined() && offset.numel();
+                bool modulated = mask.defined() && mask.numel();
+                bool with_bias = bias.defined() && bias.numel();
+
                 at::Tensor grad_out_c = grad_out.contiguous();
                 at::Tensor input_c = input.contiguous();
                 at::Tensor weight_c = weight.contiguous();
                 at::Tensor offset_c = offset.contiguous();
                 at::Tensor mask_c = mask.contiguous();
                 at::Tensor bias_c = bias.contiguous();
 
@@ -410,22 +432,22 @@
                 int64_t dilation_h = dilation[1];
                 int64_t dilation_w = dilation[2];
 
                 int64_t out_d = (in_d - 1) * stride_d - 2 * pad_d + dilation_d * (weight_d - 1) + 1 + out_pad_d;
                 int64_t out_h = (in_h - 1) * stride_h - 2 * pad_h + dilation_h * (weight_h - 1) + 1 + out_pad_h;
                 int64_t out_w = (in_w - 1) * stride_w - 2 * pad_w + dilation_w * (weight_w - 1) + 1 + out_pad_w;
 
-                int64_t offset_groups = offset.size(1) / (3 * weight_d * weight_h * weight_w);
-                int64_t mask_groups = mask.size(1) / (weight_d * weight_h * weight_w);
+                int64_t offset_groups = deformable ? offset.size(1) / (3 * weight_d * weight_h * weight_w) : 0;
+                int64_t mask_groups = modulated ? mask.size(1) / (weight_d * weight_h * weight_w) : 0;
 
                 auto grad_input = at::zeros_like(input_c);
                 auto grad_weight = at::zeros_like(weight_c);
                 auto grad_offset = at::zeros_like(offset_c);
                 auto grad_mask = at::zeros_like(mask_c);
-                auto grad_bias = at::ones_like(bias_c);
+                auto grad_bias = with_bias ? grad_out_c.sum(at::IntArrayRef({0, 2, 3, 4})) : at::zeros_like(bias_c);
 
                 // Separate into blocks
                 grad_out_c = grad_out_c.view({batch_sz / n_parallel_imgs,
                                               n_parallel_imgs,
                                               out_channels,
                                               out_d,
                                               out_h,
@@ -627,15 +649,14 @@
                                                       in_w}).transpose_(1, 2);
                 grad_input.copy_(grad_input_buf);
 
                 grad_input = grad_input.view_as(input);
                 grad_weight = grad_weight.view_as(weight);
                 grad_offset = grad_offset.view_as(offset);
                 grad_mask = grad_mask.view_as(mask);
-                grad_bias *= grad_out.sum(at::IntArrayRef({0, 2, 3, 4}));
 
                 return std::make_tuple(grad_input, grad_weight, grad_offset, grad_mask, grad_bias);
             }
         }
 
         class DeformConvTranspose3dFunction
                 : public torch::autograd::Function<DeformConvTranspose3dFunction> {
@@ -647,40 +668,34 @@
                     const torch::autograd::Variable &offset,
                     const torch::autograd::Variable &mask,
                     const torch::autograd::Variable &bias,
                     at::IntArrayRef stride,
                     at::IntArrayRef padding,
                     at::IntArrayRef output_padding,
                     at::IntArrayRef dilation,
-                    int64_t groups,
-                    bool deformable,
-                    bool modulated) {
+                    int64_t groups) {
                 at::AutoDispatchBelowADInplaceOrView g;
                 auto output = deform_conv_transpose3d_forward(
                         input,
                         weight,
                         offset,
                         mask,
                         bias,
                         stride,
                         padding,
                         output_padding,
                         dilation,
-                        groups,
-                        deformable,
-                        modulated);
+                        groups);
 
                 ctx->save_for_backward({input, weight, offset, mask, bias});
                 ctx->saved_data["stride"] = stride.vec();
                 ctx->saved_data["padding"] = padding.vec();
                 ctx->saved_data["output_padding"] = output_padding.vec();
                 ctx->saved_data["dilation"] = dilation.vec();
                 ctx->saved_data["groups"] = groups;
-                ctx->saved_data["deformable"] = deformable;
-                ctx->saved_data["modulated"] = modulated;
 
                 return {
                         output,
                 };
             }
 
             static torch::autograd::variable_list backward(
@@ -694,31 +709,27 @@
                 auto bias = saved[4];
 
                 auto stride = ctx->saved_data["stride"].toIntVector();
                 auto padding = ctx->saved_data["padding"].toIntVector();
                 auto output_padding = ctx->saved_data["output_padding"].toIntVector();
                 auto dilation = ctx->saved_data["dilation"].toIntVector();
                 auto groups = ctx->saved_data["groups"].toInt();
-                auto deformable = ctx->saved_data["deformable"].toBool();
-                auto modulated = ctx->saved_data["modulated"].toBool();
 
                 auto grads = detail::_deform_conv_transpose3d_backward(
                         grad_output[0],
                         input,
                         weight,
                         offset,
                         mask,
                         bias,
                         stride,
                         padding,
                         output_padding,
                         dilation,
-                        groups,
-                        deformable,
-                        modulated);
+                        groups);
                 auto grad_input = std::get<0>(grads);
                 auto grad_weight = std::get<1>(grads);
                 auto grad_offset = std::get<2>(grads);
                 auto grad_mask = std::get<3>(grads);
                 auto grad_bias = std::get<4>(grads);
 
                 return {
@@ -728,16 +739,14 @@
                         grad_mask,
                         grad_bias,
                         torch::autograd::Variable(),
                         torch::autograd::Variable(),
                         torch::autograd::Variable(),
                         torch::autograd::Variable(),
                         torch::autograd::Variable(),
-                        torch::autograd::Variable(),
-                        torch::autograd::Variable(),
                 };
             }
         };
 
         at::Tensor deform_conv_transpose3d(
                 const at::Tensor &input,
                 const at::Tensor &weight,
@@ -745,28 +754,26 @@
                 const at::optional<at::Tensor> &mask = {},
                 const at::optional<at::Tensor> &bias = {},
                 at::IntArrayRef stride = 1,
                 at::IntArrayRef padding = 0,
                 at::IntArrayRef output_padding = 0,
                 at::IntArrayRef dilation = 1,
                 int64_t groups = 1) {
-            C10_LOG_API_USAGE_ONCE("tvdcn.csrc.ops.deform_conv_transpose.deform_conv_transpose3d");
+            C10_LOG_API_USAGE_ONCE("tvdcn.csrc.ops.deform_conv_transpose.deform_conv_transpose3d")
             auto result = DeformConvTranspose3dFunction::apply(
                     input,
                     weight,
-                    offset.value_or(at::zeros({input.size(0), 0}, input.options().requires_grad(false))),
-                    mask.value_or(at::zeros({input.size(0), 0}, input.options().requires_grad(false))),
-                    bias.value_or(at::zeros({weight.size(0)}, input.options().requires_grad(false))),
+                    offset.value_or(input.new_zeros(0)),
+                    mask.value_or(input.new_zeros(0)),
+                    bias.value_or(input.new_zeros(0)),
                     stride,
                     padding,
                     output_padding,
                     dilation,
-                    groups,
-                    offset.has_value(),
-                    mask.has_value());
+                    groups);
             return result[0];
         }
 
         TORCH_LIBRARY_FRAGMENT(tvdcn, m) {
             m.def("tvdcn::deform_conv_transpose3d(Tensor input, Tensor weight, "
                   "Tensor? offset=None, Tensor? mask=None, Tensor? bias=None, "
                   "int[3] stride=1, int[3] padding=0, int[3] output_padding=0, "
```

### Comparing `tvdcn-0.3.0/tvdcn/csrc/ops/dispatch/deform_conv1d_kernels.cpp` & `tvdcn-0.3.1/tvdcn/csrc/ops/dispatch/deform_conv1d_kernels.cpp`

 * *Files identical despite different names*

### Comparing `tvdcn-0.3.0/tvdcn/csrc/ops/dispatch/deform_conv2d_kernels.cpp` & `tvdcn-0.3.1/tvdcn/csrc/ops/dispatch/deform_conv2d_kernels.cpp`

 * *Files identical despite different names*

### Comparing `tvdcn-0.3.0/tvdcn/csrc/ops/dispatch/deform_conv3d_kernels.cpp` & `tvdcn-0.3.1/tvdcn/csrc/ops/dispatch/deform_conv3d_kernels.cpp`

 * *Files identical despite different names*

### Comparing `tvdcn-0.3.0/tvdcn/csrc/tvdcn.cpp` & `tvdcn-0.3.1/tvdcn/csrc/tvdcn.cpp`

 * *Files identical despite different names*

### Comparing `tvdcn-0.3.0/tvdcn/extension.py` & `tvdcn-0.3.1/tvdcn/extension.py`

 * *Files identical despite different names*

### Comparing `tvdcn-0.3.0/tvdcn/ops/activations/mask_sigmoid.py` & `tvdcn-0.3.1/tvdcn/ops/activations/mask_sigmoid.py`

 * *Files identical despite different names*

### Comparing `tvdcn-0.3.0/tvdcn/ops/activations/mask_softmax.py` & `tvdcn-0.3.1/tvdcn/ops/activations/mask_softmax.py`

 * *Files identical despite different names*

### Comparing `tvdcn-0.3.0/tvdcn/ops/deform_conv.py` & `tvdcn-0.3.1/tvdcn/ops/deform_conv.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,16 +73,17 @@
         Output:
         >>>  torch.Size([4, 5, 8])
     """
     if not torch.jit.is_scripting() and not torch.jit.is_tracing():
         _log_api_usage_once(deform_conv1d)
     _assert_has_ops()
 
-    return torch.ops.tvdcn.deform_conv1d(input, weight, offset, mask, bias,
-                                         stride, padding, dilation, groups)
+    return torch.ops.tvdcn.deform_conv1d(
+        input, weight, offset, mask, bias,
+        stride, padding, dilation, groups)
 
 
 def deform_conv2d(
         input: Tensor,
         weight: Tensor,
         offset: Optional[Tensor] = None,
         mask: Optional[Tensor] = None,
@@ -133,16 +134,17 @@
         Output:
         >>>  torch.Size([4, 5, 8, 8])
     """
     if not torch.jit.is_scripting() and not torch.jit.is_tracing():
         _log_api_usage_once(deform_conv2d)
     _assert_has_ops()
 
-    return torch.ops.tvdcn.deform_conv2d(input, weight, offset, mask, bias,
-                                         stride, padding, dilation, groups)
+    return torch.ops.tvdcn.deform_conv2d(
+        input, weight, offset, mask, bias,
+        stride, padding, dilation, groups)
 
 
 def deform_conv3d(
         input: Tensor,
         weight: Tensor,
         offset: Optional[Tensor] = None,
         mask: Optional[Tensor] = None,
@@ -189,16 +191,17 @@
         Output:
         >>> torch.Size([4, 5, 8, 8, 8])
     """
     if not torch.jit.is_scripting() and not torch.jit.is_tracing():
         _log_api_usage_once(deform_conv3d)
     _assert_has_ops()
 
-    return torch.ops.tvdcn.deform_conv3d(input, weight, offset, mask, bias,
-                                         stride, padding, dilation, groups)
+    return torch.ops.tvdcn.deform_conv3d(
+        input, weight, offset, mask, bias,
+        stride, padding, dilation, groups)
 
 
 ################################################################################
 # Modules
 ################################################################################
 # noinspection PyMethodOverriding
 class _DeformConvNd(_ConvNd):
```

### Comparing `tvdcn-0.3.0/tvdcn/ops/deform_conv_transpose.py` & `tvdcn-0.3.1/tvdcn/ops/deform_conv_transpose.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,16 +74,17 @@
         Output:
         >>>  torch.Size([4, 5, 10])
     """
     if not torch.jit.is_scripting() and not torch.jit.is_tracing():
         _log_api_usage_once(deform_conv_transpose1d)
     _assert_has_ops()
 
-    return torch.ops.tvdcn.deform_conv_transpose1d(input, weight, offset, mask, bias,
-                                                   stride, padding, output_padding, dilation, groups)
+    return torch.ops.tvdcn.deform_conv_transpose1d(
+        input, weight, offset, mask, bias,
+        stride, padding, output_padding, dilation, groups)
 
 
 def deform_conv_transpose2d(
         input: Tensor,
         weight: Tensor,
         offset: Optional[Tensor] = None,
         mask: Optional[Tensor] = None,
@@ -130,16 +131,17 @@
         Output:
         >>>  torch.Size([4, 5, 10, 10])
     """
     if not torch.jit.is_scripting() and not torch.jit.is_tracing():
         _log_api_usage_once(deform_conv_transpose2d)
     _assert_has_ops()
 
-    return torch.ops.tvdcn.deform_conv_transpose2d(input, weight, offset, mask, bias,
-                                                   stride, padding, output_padding, dilation, groups)
+    return torch.ops.tvdcn.deform_conv_transpose2d(
+        input, weight, offset, mask, bias,
+        stride, padding, output_padding, dilation, groups)
 
 
 def deform_conv_transpose3d(
         input: Tensor,
         weight: Tensor,
         offset: Optional[Tensor] = None,
         mask: Optional[Tensor] = None,
@@ -187,16 +189,17 @@
         Output:
         >>> torch.Size([4, 5, 10, 10, 10])
     """
     if not torch.jit.is_scripting() and not torch.jit.is_tracing():
         _log_api_usage_once(deform_conv_transpose3d)
     _assert_has_ops()
 
-    return torch.ops.tvdcn.deform_conv_transpose3d(input, weight, offset, mask, bias,
-                                                   stride, padding, output_padding, dilation, groups)
+    return torch.ops.tvdcn.deform_conv_transpose3d(
+        input, weight, offset, mask, bias,
+        stride, padding, output_padding, dilation, groups)
 
 
 ################################################################################
 # Modules
 ################################################################################
 # noinspection PyMethodOverriding
 class _DeformConvTransposeNd(_DeformConvNd):
```

### Comparing `tvdcn-0.3.0/tvdcn/utils.py` & `tvdcn-0.3.1/tvdcn/utils.py`

 * *Files identical despite different names*

### Comparing `tvdcn-0.3.0/tvdcn.egg-info/PKG-INFO` & `tvdcn-0.3.1/tvdcn.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tvdcn
-Version: 0.3.0
+Version: 0.3.1
 Summary: Torchvision+ Deformable Convolutional Networks
 Home-page: https://github.com/inspiros/tvdcn
 Author: Hoang-Nhat Tran (inspiros)
 Author-email: hnhat.tran@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/inspiros/tvdcn
 Keywords: deform_conv; deformable convolution
```

### Comparing `tvdcn-0.3.0/tvdcn.egg-info/SOURCES.txt` & `tvdcn-0.3.1/tvdcn.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -30,13 +30,14 @@
 tvdcn/csrc/ops/cpu/deform_conv3d_kernels_cpu.cpp
 tvdcn/csrc/ops/cuda/deform_conv1d_kernels_cuda.cu
 tvdcn/csrc/ops/cuda/deform_conv2d_kernels_cuda.cu
 tvdcn/csrc/ops/cuda/deform_conv3d_kernels_cuda.cu
 tvdcn/csrc/ops/dispatch/deform_conv1d_kernels.cpp
 tvdcn/csrc/ops/dispatch/deform_conv2d_kernels.cpp
 tvdcn/csrc/ops/dispatch/deform_conv3d_kernels.cpp
+tvdcn/csrc/ops/utils/tensor_utils.cpp
 tvdcn/ops/__init__.py
 tvdcn/ops/deform_conv.py
 tvdcn/ops/deform_conv_transpose.py
 tvdcn/ops/activations/__init__.py
 tvdcn/ops/activations/mask_sigmoid.py
 tvdcn/ops/activations/mask_softmax.py
```

