# Comparing `tmp/empatches-0.2.2.tar.gz` & `tmp/empatches-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "empatches-0.2.2.tar", last modified: Wed Nov 30 11:24:52 2022, max compression
+gzip compressed data, was "empatches-0.2.3.tar", last modified: Sun Jul  2 00:42:06 2023, max compression
```

## Comparing `empatches-0.2.2.tar` & `empatches-0.2.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2022-11-30 11:24:52.795145 empatches-0.2.2/
--rw-rw-rw-   0        0        0    10677 2022-11-30 11:24:52.794147 empatches-0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     9991 2022-11-30 11:23:24.000000 empatches-0.2.2/README.md
-drwxrwxrwx   0        0        0        0 2022-11-30 11:24:52.768145 empatches-0.2.2/empatches/
--rw-rw-rw-   0        0        0       66 2022-10-28 00:08:36.000000 empatches-0.2.2/empatches/__init__.py
--rw-rw-rw-   0        0        0    23293 2022-11-30 11:08:53.000000 empatches-0.2.2/empatches/empatches.py
-drwxrwxrwx   0        0        0        0 2022-11-30 11:24:52.792644 empatches-0.2.2/empatches.egg-info/
--rw-rw-rw-   0        0        0    10677 2022-11-30 11:24:52.000000 empatches-0.2.2/empatches.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      227 2022-11-30 11:24:52.000000 empatches-0.2.2/empatches.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-11-30 11:24:52.000000 empatches-0.2.2/empatches.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2022-11-30 11:24:52.000000 empatches-0.2.2/empatches.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2022-11-30 11:24:52.000000 empatches-0.2.2/empatches.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-11-30 11:24:52.795145 empatches-0.2.2/setup.cfg
--rw-rw-rw-   0        0        0     1279 2022-11-30 11:24:08.000000 empatches-0.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-02 00:42:06.192194 empatches-0.2.3/
+-rw-rw-rw-   0        0        0    10764 2023-07-02 00:42:06.191695 empatches-0.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0    10117 2023-07-02 00:38:44.000000 empatches-0.2.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-02 00:42:06.169694 empatches-0.2.3/empatches/
+-rw-rw-rw-   0        0        0       66 2022-10-28 00:08:36.000000 empatches-0.2.3/empatches/__init__.py
+-rw-rw-rw-   0        0        0    23295 2023-07-02 00:39:49.000000 empatches-0.2.3/empatches/empatches.py
+drwxrwxrwx   0        0        0        0 2023-07-02 00:42:06.189724 empatches-0.2.3/empatches.egg-info/
+-rw-rw-rw-   0        0        0    10764 2023-07-02 00:42:05.000000 empatches-0.2.3/empatches.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      227 2023-07-02 00:42:06.000000 empatches-0.2.3/empatches.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-02 00:42:05.000000 empatches-0.2.3/empatches.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-07-02 00:42:05.000000 empatches-0.2.3/empatches.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-02 00:42:05.000000 empatches-0.2.3/empatches.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-02 00:42:06.192194 empatches-0.2.3/setup.cfg
+-rw-rw-rw-   0        0        0     1279 2023-07-02 00:39:57.000000 empatches-0.2.3/setup.py
```

### Comparing `empatches-0.2.2/PKG-INFO` & `empatches-0.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 Metadata-Version: 2.1
 Name: empatches
-Version: 0.2.2
+Version: 0.2.3
 Summary: Extract and Merge Batches/Image patches (tf/torch) for easy, fast and self-contained digital image processing and deep learning model training.
 Home-page: https://github.com/Mr-TalhaIlyas/EMPatches
 Author: Talha Ilyas
 Author-email: mr.talhailyas@gmail.com
-License: UNKNOWN
 Keywords: python,extract image patches,merge image patches,patchify,sliding window
-Platform: UNKNOWN
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT)
- [![Generic badge](https://img.shields.io/badge/Version-0.2.2-<COLOR>.svg)](https://shields.io/) [![Downloads](https://pepy.tech/badge/empatches)](https://pepy.tech/project/empatches)  [![Hits](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fpypi.org%2Fproject%2Fempatches%2F&count_bg=%2379C83D&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=hits&edge_flat=false)](https://hits.seeyoufarm.com)
+ [![Generic badge](https://img.shields.io/badge/Version-0.2.3-<COLOR>.svg)](https://shields.io/) [![Downloads](https://pepy.tech/badge/empatches)](https://pepy.tech/project/empatches)  [![Hits](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fpypi.org%2Fproject%2Fempatches%2F&count_bg=%2379C83D&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=hits&edge_flat=false)](https://hits.seeyoufarm.com)
 
 # Extract and Merge Image Patches (EMPatches)
 
 Extract and Merge Batches/Image patches (tf/torch), fast and self-contained digital image processing and deep learning model training.
 
 * **Extract** patches
 * **Merge** the extracted patches to obtain the original image back.
+### *Upadate 0.2.3 (Bug Fix)*
+* While merging tensors.\
+thanks [MRLBradley](https://github.com/MRLBradley) for noticing.
+
 ### *Upadate 0.2.2 (New Functionalities)*
 
 * Handling 1D spectral and 3D volumetric data structures, thanks to [antonyvam](https://github.com/antonyvam).
 * Batch processing support for 1D, 2D, 3D (image/pixel + voxel/volumetric) data added.
 * Bug fixes for multi-dimensional image patch merging for `C > 3`.
 
 ### *Update 0.2.0*
@@ -283,8 +285,7 @@
 plt.imshow(tiled.astype(np.uint8))
 plt.title('patching via providing indices')
 ```
 
 ![alt text](https://github.com/Mr-TalhaIlyas/EMPatches/raw/main/screens/p_via_indices.png)
 
 For more infomration visit Homepage.
-
```

### Comparing `empatches-0.2.2/README.md` & `empatches-0.2.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT)
- [![Generic badge](https://img.shields.io/badge/Version-0.2.2-<COLOR>.svg)](https://shields.io/) [![Downloads](https://pepy.tech/badge/empatches)](https://pepy.tech/project/empatches)  [![Hits](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fpypi.org%2Fproject%2Fempatches%2F&count_bg=%2379C83D&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=hits&edge_flat=false)](https://hits.seeyoufarm.com)
+ [![Generic badge](https://img.shields.io/badge/Version-0.2.3-<COLOR>.svg)](https://shields.io/) [![Downloads](https://pepy.tech/badge/empatches)](https://pepy.tech/project/empatches)  [![Hits](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fpypi.org%2Fproject%2Fempatches%2F&count_bg=%2379C83D&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=hits&edge_flat=false)](https://hits.seeyoufarm.com)
 
 # Extract and Merge Image Patches (EMPatches)
 
 Extract and Merge Batches/Image patches (tf/torch), fast and self-contained digital image processing and deep learning model training.
 
 * **Extract** patches
 * **Merge** the extracted patches to obtain the original image back.
+### *Upadate 0.2.3 (Bug Fix)*
+* While merging tensors.\
+thanks [MRLBradley](https://github.com/MRLBradley) for noticing.
+
 ### *Upadate 0.2.2 (New Functionalities)*
 
 * Handling 1D spectral and 3D volumetric data structures, thanks to [antonyvam](https://github.com/antonyvam).
 * Batch processing support for 1D, 2D, 3D (image/pixel + voxel/volumetric) data added.
 * Bug fixes for multi-dimensional image patch merging for `C > 3`.
 
 ### *Update 0.2.0*
```

### Comparing `empatches-0.2.2/empatches/empatches.py` & `empatches-0.2.3/empatches/empatches.py`

 * *Files 1% similar despite different names*

```diff
@@ -445,15 +445,15 @@
         for p, i in zip(b_patches, b_indices):
             m = super().merge_patches(p, i, mode)
             m_patches.append(m)
 
         m_patches = np.asarray(m_patches)
         
         if self.typ == 'torch':
-            m_patches = m_patches.permute(0,3,2,1)
+            m_patches = m_patches.transpose(0,3,2,1)
 
         return m_patches
         
 
 def patch_via_indices(data, indices):
     '''
         Parameters
```

### Comparing `empatches-0.2.2/empatches.egg-info/PKG-INFO` & `empatches-0.2.3/empatches.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 Metadata-Version: 2.1
 Name: empatches
-Version: 0.2.2
+Version: 0.2.3
 Summary: Extract and Merge Batches/Image patches (tf/torch) for easy, fast and self-contained digital image processing and deep learning model training.
 Home-page: https://github.com/Mr-TalhaIlyas/EMPatches
 Author: Talha Ilyas
 Author-email: mr.talhailyas@gmail.com
-License: UNKNOWN
 Keywords: python,extract image patches,merge image patches,patchify,sliding window
-Platform: UNKNOWN
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT)
- [![Generic badge](https://img.shields.io/badge/Version-0.2.2-<COLOR>.svg)](https://shields.io/) [![Downloads](https://pepy.tech/badge/empatches)](https://pepy.tech/project/empatches)  [![Hits](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fpypi.org%2Fproject%2Fempatches%2F&count_bg=%2379C83D&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=hits&edge_flat=false)](https://hits.seeyoufarm.com)
+ [![Generic badge](https://img.shields.io/badge/Version-0.2.3-<COLOR>.svg)](https://shields.io/) [![Downloads](https://pepy.tech/badge/empatches)](https://pepy.tech/project/empatches)  [![Hits](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fpypi.org%2Fproject%2Fempatches%2F&count_bg=%2379C83D&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=hits&edge_flat=false)](https://hits.seeyoufarm.com)
 
 # Extract and Merge Image Patches (EMPatches)
 
 Extract and Merge Batches/Image patches (tf/torch), fast and self-contained digital image processing and deep learning model training.
 
 * **Extract** patches
 * **Merge** the extracted patches to obtain the original image back.
+### *Upadate 0.2.3 (Bug Fix)*
+* While merging tensors.\
+thanks [MRLBradley](https://github.com/MRLBradley) for noticing.
+
 ### *Upadate 0.2.2 (New Functionalities)*
 
 * Handling 1D spectral and 3D volumetric data structures, thanks to [antonyvam](https://github.com/antonyvam).
 * Batch processing support for 1D, 2D, 3D (image/pixel + voxel/volumetric) data added.
 * Bug fixes for multi-dimensional image patch merging for `C > 3`.
 
 ### *Update 0.2.0*
@@ -283,8 +285,7 @@
 plt.imshow(tiled.astype(np.uint8))
 plt.title('patching via providing indices')
 ```
 
 ![alt text](https://github.com/Mr-TalhaIlyas/EMPatches/raw/main/screens/p_via_indices.png)
 
 For more infomration visit Homepage.
-
```

### Comparing `empatches-0.2.2/setup.py` & `empatches-0.2.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup, find_packages
 
-VERSION = '0.2.2'
+VERSION = '0.2.3'
 DESCRIPTION = "Extract and Merge Batches/Image patches (tf/torch) for easy, fast and self-contained digital image processing and deep learning model training."
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
     
 INSTALL_REQUIRES = [
                     'numpy'
```

