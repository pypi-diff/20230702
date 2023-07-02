# Comparing `tmp/bnpm-0.2.0.tar.gz` & `tmp/bnpm-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/bnpm-0.2.0.tar", last modified: Fri Jun  9 23:44:12 2023, max compression
+gzip compressed data, was "bnpm-0.2.1.tar", last modified: Sun Jul  2 00:20:47 2023, max compression
```

## Comparing `bnpm-0.2.0.tar` & `bnpm-0.2.1.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-09 23:44:12.776153 bnpm-0.2.0/
--rwxrwxrwx   0 root         (0) root         (0)     1068 2022-09-13 02:36:53.000000 bnpm-0.2.0/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)     3084 2023-06-09 23:44:12.776241 bnpm-0.2.0/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     2725 2023-06-09 23:20:45.000000 bnpm-0.2.0/README.md
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-09 23:44:12.774622 bnpm-0.2.0/bnpm/
--rwxrwxrwx   0 root         (0) root         (0)      907 2023-06-09 23:26:05.000000 bnpm-0.2.0/bnpm/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    37134 2023-05-18 20:21:08.000000 bnpm-0.2.0/bnpm/ca2p_preprocessing.py
--rwxrwxrwx   0 root         (0) root         (0)     4444 2023-06-08 15:16:51.000000 bnpm-0.2.0/bnpm/classification.py
--rwxrwxrwx   0 root         (0) root         (0)    55191 2023-05-14 23:41:40.000000 bnpm-0.2.0/bnpm/clustering.py
--rwxrwxrwx   0 root         (0) root         (0)    10099 2023-04-24 20:00:51.000000 bnpm-0.2.0/bnpm/container_helpers.py
--rwxrwxrwx   0 root         (0) root         (0)     4477 2021-12-28 22:22:14.000000 bnpm-0.2.0/bnpm/cross_validation.py
--rwxrwxrwx   0 root         (0) root         (0)      940 2021-12-28 19:03:39.000000 bnpm-0.2.0/bnpm/cupy_helpers.py
--rwxrwxrwx   0 root         (0) root         (0)    16674 2023-03-19 21:48:35.000000 bnpm-0.2.0/bnpm/decomposition.py
--rwxrwxrwx   0 root         (0) root         (0)     5310 2021-12-28 19:04:57.000000 bnpm-0.2.0/bnpm/dtw.py
--rwxrwxrwx   0 root         (0) root         (0)     1753 2022-11-15 17:45:20.000000 bnpm-0.2.0/bnpm/email_helpers.py
--rwxrwxrwx   0 root         (0) root         (0)    19171 2023-06-08 15:16:54.000000 bnpm-0.2.0/bnpm/featurization.py
--rwxrwxrwx   0 root         (0) root         (0)    21239 2023-06-05 05:36:55.000000 bnpm-0.2.0/bnpm/file_helpers.py
--rwxrwxrwx   0 root         (0) root         (0)    11693 2023-06-08 14:03:50.000000 bnpm-0.2.0/bnpm/h5_handling.py
--rwxrwxrwx   0 root         (0) root         (0)    52633 2023-05-31 04:24:13.000000 bnpm-0.2.0/bnpm/image_processing.py
--rwxrwxrwx   0 root         (0) root         (0)    22721 2023-06-09 18:03:17.000000 bnpm-0.2.0/bnpm/indexing.py
--rwxrwxrwx   0 root         (0) root         (0)    17856 2023-03-05 00:44:40.000000 bnpm-0.2.0/bnpm/linear_regression.py
--rwxrwxrwx   0 root         (0) root         (0)     8317 2023-04-21 04:21:03.000000 bnpm-0.2.0/bnpm/math_functions.py
--rwxrwxrwx   0 root         (0) root         (0)     9514 2023-06-09 18:43:59.000000 bnpm-0.2.0/bnpm/misc.py
--rwxrwxrwx   0 root         (0) root         (0)     4623 2023-05-12 16:20:07.000000 bnpm-0.2.0/bnpm/optimization.py
--rwxrwxrwx   0 root         (0) root         (0)     6922 2023-04-28 21:19:30.000000 bnpm-0.2.0/bnpm/other_peoples_code.py
--rwxrwxrwx   0 root         (0) root         (0)     4442 2023-04-29 05:04:13.000000 bnpm-0.2.0/bnpm/parallel_helpers.py
--rwxrwxrwx   0 root         (0) root         (0)     6370 2022-10-27 16:16:53.000000 bnpm-0.2.0/bnpm/path_helpers.py
--rwxrwxrwx   0 root         (0) root         (0)    29499 2023-06-09 06:50:59.000000 bnpm-0.2.0/bnpm/plotting_helpers.py
--rwxrwxrwx   0 root         (0) root         (0)     9811 2023-05-18 20:31:06.000000 bnpm-0.2.0/bnpm/resource_tracking.py
--rwxrwxrwx   0 root         (0) root         (0)    34626 2023-04-21 22:51:53.000000 bnpm-0.2.0/bnpm/server.py
--rwxrwxrwx   0 root         (0) root         (0)    30842 2023-04-27 15:12:19.000000 bnpm-0.2.0/bnpm/similarity.py
--rwxrwxrwx   0 root         (0) root         (0)    22842 2023-05-11 22:58:37.000000 bnpm-0.2.0/bnpm/spectral.py
--rwxrwxrwx   0 root         (0) root         (0)     1130 2023-05-18 04:27:38.000000 bnpm-0.2.0/bnpm/stats.py
--rwxrwxrwx   0 root         (0) root         (0)    36813 2023-06-09 23:34:38.000000 bnpm-0.2.0/bnpm/timeSeries.py
--rwxrwxrwx   0 root         (0) root         (0)    13395 2023-02-28 17:16:58.000000 bnpm-0.2.0/bnpm/torch_helpers.py
--rwxrwxrwx   0 root         (0) root         (0)    46632 2023-06-09 23:30:37.000000 bnpm-0.2.0/bnpm/video.py
--rwxrwxrwx   0 root         (0) root         (0)     3338 2021-12-28 19:07:58.000000 bnpm-0.2.0/bnpm/welford_moving.py
--rwxrwxrwx   0 root         (0) root         (0)     4882 2021-05-05 20:10:58.000000 bnpm-0.2.0/bnpm/welford_moving_2D.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-09 23:44:12.775745 bnpm-0.2.0/bnpm.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)     3084 2023-06-09 23:44:12.000000 bnpm-0.2.0/bnpm.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      895 2023-06-09 23:44:12.000000 bnpm-0.2.0/bnpm.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2023-06-09 23:44:12.000000 bnpm-0.2.0/bnpm.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)      326 2023-06-09 23:44:12.000000 bnpm-0.2.0/bnpm.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)        5 2023-06-09 23:44:12.000000 bnpm-0.2.0/bnpm.egg-info/top_level.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-09 23:44:12.775964 bnpm-0.2.0/demos/
--rwxrwxrwx   0 root         (0) root         (0)     1902 2022-05-10 23:33:18.000000 bnpm-0.2.0/demos/slurmDispatcher.py
--rwxrwxrwx   0 root         (0) root         (0)       79 2023-06-09 23:44:12.776564 bnpm-0.2.0/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     2952 2023-06-09 23:42:29.000000 bnpm-0.2.0/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-02 00:20:47.644057 bnpm-0.2.1/
+-rwxrwxrwx   0 root         (0) root         (0)     1068 2022-09-13 02:36:53.000000 bnpm-0.2.1/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)     3330 2023-07-02 00:20:47.644194 bnpm-0.2.1/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     2971 2023-06-16 05:27:34.000000 bnpm-0.2.1/README.md
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-02 00:20:47.642288 bnpm-0.2.1/bnpm/
+-rwxrwxrwx   0 root         (0) root         (0)      907 2023-07-02 00:16:12.000000 bnpm-0.2.1/bnpm/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    37134 2023-05-18 20:21:08.000000 bnpm-0.2.1/bnpm/ca2p_preprocessing.py
+-rwxrwxrwx   0 root         (0) root         (0)     4603 2023-06-25 23:47:42.000000 bnpm-0.2.1/bnpm/classification.py
+-rwxrwxrwx   0 root         (0) root         (0)    49222 2023-06-17 04:47:40.000000 bnpm-0.2.1/bnpm/clustering.py
+-rwxrwxrwx   0 root         (0) root         (0)    10138 2023-06-28 13:37:49.000000 bnpm-0.2.1/bnpm/container_helpers.py
+-rwxrwxrwx   0 root         (0) root         (0)     4477 2021-12-28 22:22:14.000000 bnpm-0.2.1/bnpm/cross_validation.py
+-rwxrwxrwx   0 root         (0) root         (0)      940 2021-12-28 19:03:39.000000 bnpm-0.2.1/bnpm/cupy_helpers.py
+-rwxrwxrwx   0 root         (0) root         (0)    16674 2023-03-19 21:48:35.000000 bnpm-0.2.1/bnpm/decomposition.py
+-rwxrwxrwx   0 root         (0) root         (0)     5310 2021-12-28 19:04:57.000000 bnpm-0.2.1/bnpm/dtw.py
+-rwxrwxrwx   0 root         (0) root         (0)     1753 2022-11-15 17:45:20.000000 bnpm-0.2.1/bnpm/email_helpers.py
+-rwxrwxrwx   0 root         (0) root         (0)    19171 2023-06-08 15:16:54.000000 bnpm-0.2.1/bnpm/featurization.py
+-rwxrwxrwx   0 root         (0) root         (0)    23399 2023-06-29 05:55:34.000000 bnpm-0.2.1/bnpm/file_helpers.py
+-rwxrwxrwx   0 root         (0) root         (0)    11769 2023-06-10 18:47:53.000000 bnpm-0.2.1/bnpm/h5_handling.py
+-rwxrwxrwx   0 root         (0) root         (0)    57594 2023-07-01 01:57:59.000000 bnpm-0.2.1/bnpm/image_processing.py
+-rwxrwxrwx   0 root         (0) root         (0)    22721 2023-06-09 18:03:17.000000 bnpm-0.2.1/bnpm/indexing.py
+-rwxrwxrwx   0 root         (0) root         (0)    17856 2023-03-05 00:44:40.000000 bnpm-0.2.1/bnpm/linear_regression.py
+-rwxrwxrwx   0 root         (0) root         (0)     8317 2023-04-21 04:21:03.000000 bnpm-0.2.1/bnpm/math_functions.py
+-rwxrwxrwx   0 root         (0) root         (0)     6202 2023-06-17 04:51:49.000000 bnpm-0.2.1/bnpm/misc.py
+-rwxrwxrwx   0 root         (0) root         (0)    10034 2023-06-24 16:25:12.000000 bnpm-0.2.1/bnpm/optimization.py
+-rwxrwxrwx   0 root         (0) root         (0)     6922 2023-04-28 21:19:30.000000 bnpm-0.2.1/bnpm/other_peoples_code.py
+-rwxrwxrwx   0 root         (0) root         (0)     4442 2023-04-29 05:04:13.000000 bnpm-0.2.1/bnpm/parallel_helpers.py
+-rwxrwxrwx   0 root         (0) root         (0)     6370 2022-10-27 16:16:53.000000 bnpm-0.2.1/bnpm/path_helpers.py
+-rwxrwxrwx   0 root         (0) root         (0)    38452 2023-06-17 22:18:41.000000 bnpm-0.2.1/bnpm/plotting_helpers.py
+-rwxrwxrwx   0 root         (0) root         (0)     9811 2023-05-18 20:31:06.000000 bnpm-0.2.1/bnpm/resource_tracking.py
+-rwxrwxrwx   0 root         (0) root         (0)    34625 2023-06-19 08:21:29.000000 bnpm-0.2.1/bnpm/server.py
+-rwxrwxrwx   0 root         (0) root         (0)    29980 2023-06-17 04:30:32.000000 bnpm-0.2.1/bnpm/similarity.py
+-rwxrwxrwx   0 root         (0) root         (0)    22632 2023-06-17 04:28:34.000000 bnpm-0.2.1/bnpm/spectral.py
+-rwxrwxrwx   0 root         (0) root         (0)     1130 2023-05-18 04:27:38.000000 bnpm-0.2.1/bnpm/stats.py
+-rwxrwxrwx   0 root         (0) root         (0)    35757 2023-06-17 04:42:40.000000 bnpm-0.2.1/bnpm/timeSeries.py
+-rwxrwxrwx   0 root         (0) root         (0)    13307 2023-06-17 04:43:28.000000 bnpm-0.2.1/bnpm/torch_helpers.py
+-rwxrwxrwx   0 root         (0) root         (0)    50036 2023-06-16 03:39:42.000000 bnpm-0.2.1/bnpm/video.py
+-rwxrwxrwx   0 root         (0) root         (0)     3338 2021-12-28 19:07:58.000000 bnpm-0.2.1/bnpm/welford_moving.py
+-rwxrwxrwx   0 root         (0) root         (0)     4882 2021-05-05 20:10:58.000000 bnpm-0.2.1/bnpm/welford_moving_2D.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-02 00:20:47.643578 bnpm-0.2.1/bnpm.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)     3330 2023-07-02 00:20:47.000000 bnpm-0.2.1/bnpm.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      895 2023-07-02 00:20:47.000000 bnpm-0.2.1/bnpm.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-07-02 00:20:47.000000 bnpm-0.2.1/bnpm.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)      326 2023-07-02 00:20:47.000000 bnpm-0.2.1/bnpm.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)        5 2023-07-02 00:20:47.000000 bnpm-0.2.1/bnpm.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-02 00:20:47.643836 bnpm-0.2.1/demos/
+-rwxrwxrwx   0 root         (0) root         (0)     1902 2022-05-10 23:33:18.000000 bnpm-0.2.1/demos/slurmDispatcher.py
+-rwxrwxrwx   0 root         (0) root         (0)       79 2023-07-02 00:20:47.644610 bnpm-0.2.1/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     2952 2023-06-10 00:46:32.000000 bnpm-0.2.1/setup.py
```

### Comparing `bnpm-0.2.0/LICENSE` & `bnpm-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bnpm-0.2.0/PKG-INFO` & `bnpm-0.2.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,39 @@
 Metadata-Version: 2.1
 Name: bnpm
-Version: 0.2.0
+Version: 0.2.1
 Summary: A library of useful modules for data analysis.
 Home-page: https://github.com/RichieHakim/basic_neural_processing_modules
 Author: Richard Hakim
 License: LICENSE
 Keywords: data analysis,machine learning,neuroscience
 Description-Content-Type: text/markdown
 Provides-Extra: advanced
 License-File: LICENSE
 
+[![PyPI version](https://badge.fury.io/py/bnpm.svg)](https://badge.fury.io/py/bnpm)
+[![Downloads](https://pepy.tech/badge/bnpm)](https://pepy.tech/project/bnpm)
 [![repo size](https://img.shields.io/github/repo-size/RichieHakim/basic_neural_processing_modules)](https://github.com/RichieHakim/basic_neural_processing_modules/)
 
 #  basic_neural_processing_modules 
 Personal library of functions used in analyzing neural data.
 If you find a bug or just want to reach out: RichHakim@gmail.com
 
 ## Installation 
 Normal installation of `bnpm` does not install all possible dependencies; there are some specific functions that wrap libraries that may need to be installed separately on a case-by-case basis.
 
-`pip install git+https://github.com/RichieHakim/basic_neural_processing_modules.git`
+Install stable version:
+```
+pip install bnpm
+```
+
+Install development version:
+```
+pip install git+https://github.com/RichieHakim/basic_neural_processing_modules.git
+```
 
 import with: `import bnpm`
 
 
 ## Usage 
 My favorites:
 - **`featurization.Toeplitz_convolution2d`**
```

### Comparing `bnpm-0.2.0/README.md` & `bnpm-0.2.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,27 @@
+[![PyPI version](https://badge.fury.io/py/bnpm.svg)](https://badge.fury.io/py/bnpm)
+[![Downloads](https://pepy.tech/badge/bnpm)](https://pepy.tech/project/bnpm)
 [![repo size](https://img.shields.io/github/repo-size/RichieHakim/basic_neural_processing_modules)](https://github.com/RichieHakim/basic_neural_processing_modules/)
 
 #  basic_neural_processing_modules 
 Personal library of functions used in analyzing neural data.
 If you find a bug or just want to reach out: RichHakim@gmail.com
 
 ## Installation 
 Normal installation of `bnpm` does not install all possible dependencies; there are some specific functions that wrap libraries that may need to be installed separately on a case-by-case basis.
 
-`pip install git+https://github.com/RichieHakim/basic_neural_processing_modules.git`
+Install stable version:
+```
+pip install bnpm
+```
+
+Install development version:
+```
+pip install git+https://github.com/RichieHakim/basic_neural_processing_modules.git
+```
 
 import with: `import bnpm`
 
 
 ## Usage 
 My favorites:
 - **`featurization.Toeplitz_convolution2d`**
```

### Comparing `bnpm-0.2.0/bnpm/__init__.py` & `bnpm-0.2.1/bnpm/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,8 +29,8 @@
             'torch_helpers',
             'video',
         ]
 
 for pkg in __all__:
     exec('from . import ' + pkg)
 
-__version__ = '0.2.0'
+__version__ = '0.2.1'
```

### Comparing `bnpm-0.2.0/bnpm/ca2p_preprocessing.py` & `bnpm-0.2.1/bnpm/ca2p_preprocessing.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.2.0/bnpm/classification.py` & `bnpm-0.2.1/bnpm/classification.py`

 * *Files 4% similar despite different names*

```diff
@@ -101,39 +101,44 @@
     ## Make an array of repeated arange(len(arr)) vector
     indices = arange(n_classes)[None,:]
     ## Compare each element of arr to each element of indices
     oneHot = arr[:,None] == indices
     return oneHot
 
 
-def convert_stringArray_to_oneHot(seq, strs=['A','C','G','T'], safe=False):
+def convert_stringArray_to_oneHot(seq, strs=None, safe=False):
     """
     Convert a sequence of string elements to a one-hot matrix.
     RH 2022
 
     Args:
         seq (str):
             Sequence of string elements.
             example ['A','C','G','T','A','C','G','T']
         strs (list):
             List of string elements to use.
             Number of output columns will be len(strs).
             example: ['A','C','G','T','N','R','Y','S','W','K','M','B','D','H','V']
+            If None, will use np.unique(seq) to get all unique elements.
         safe (bool):
             If True, will check that all string elements in seq
              are in strs.
 
     Returns:
         oneHot (np.ndarray):
             2-D array of one-hot vectors.
             Columns correspond to string elements, rows to
              positions in seq.
     """
     seq_arr = np.char.upper(np.array(seq, dtype='U1'))
+
+    if strs is None:
+        strs = np.unique(seq_arr)
+    strs = np.char.upper(np.array(strs, dtype='U1'))
     
-    assert np.all(np.isin(seq_arr, strs)), "Some characters in sequence are not in allowable_chars" if safe else None
+    if not safe:
+        assert np.all(np.isin(seq_arr, strs)), "Some characters in sequence are not in strs"
     
     nuc_ints = np.array(strs).view(np.uint32)
     seq_ints = seq_arr.view(np.uint32)
     oneHot = np.vstack([seq_ints==n for n in nuc_ints]).T
-    return oneHot
-
+    return oneHot
```

### Comparing `bnpm-0.2.0/bnpm/clustering.py` & `bnpm-0.2.1/bnpm/clustering.py`

 * *Files 10% similar despite different names*

```diff
@@ -219,184 +219,14 @@
         )
         self.clusters_idx_unique = np.array(cluster_idx, dtype=object)[idx]
         self.clusters_idx_unique_freq = c
 
         return self.clusters_idx_unique, self.clusters_idx_unique_freq
 
 
-# def cluster_silhouette_score(
-#     s,
-#     h,
-#     locality=1,
-#     return_inAndOut=False,
-#     method_in='mean',
-#     method_out='max',
-# ):
-#     """
-#     Function to compute the aggregated silhouette score of clusters.
-#     Here, the score measures the similarity between samples within
-#      a cluster and between samples within a cluster and all other samples.
-#     To compute a true silhouette score, use:
-#      method_in='mean' and method_out='max'.
-
-#     RH 2022
-
-#     Args:
-#         s (torch.Tensor, dtype float):
-#             The similarity matrix.
-#             shape: (n_samples, n_samples)
-#         h (torch.Tensor, dtype bool):
-#             The cluster membership matrix.
-#             shape: (n_samples, n_clusters)
-#         locality (float):
-#             The exponent applied to the similarity matrix.
-#             Higher values make the score more dependent on local 
-#              similarity. 
-#             Setting method_out to 'mean' and using a high locality 
-#              value can result in something similar to a silhouette
-#              score.
-#         return_inAndOut (bool):
-#             If True then the in and out scores are returned.
-
-#     """
-
-#     if h.dtype != torch.bool:
-#         raise ValueError('h must be a boolean tensor.')
-
-#     n_clusters = h.shape[1]
-#     n_samples = h.shape[0]
-    
-#     DEVICE = s.device
-#     s_tu = (s**locality).type(torch.float32)
-#     s_tu[torch.arange(n_samples).to(DEVICE), torch.arange(n_samples).to(DEVICE)] = torch.nan
-#     h_tu = h.to(DEVICE)
-    
-#     if method_in == 'mean':
-#         fn_mi = torch.nanmean
-#     elif method_in == 'max':
-#         fn_mi = torch_helpers.nanmax
-#     elif method_in == 'min':
-#         fn_mi = torch_helpers.nanmin
-#     else:
-#         raise ValueError('method_in must be one of "mean", "max", "min".')
-
-#     if method_out == 'mean':
-#         fn_mo = torch.nanmean
-#     elif method_out == 'max':
-#         fn_mo = torch_helpers.nanmax
-#     elif method_out == 'min':
-#         fn_mo = torch_helpers.nanmin
-#     else:
-#         raise ValueError('method_out must be one of "mean", "max", "min".')
-        
-#     cs_in  = torch.as_tensor([fn_mi(s_tu[h_tu[:,ii]][:, h_tu[:,ii]]) for ii in range(n_clusters)], device=DEVICE)
-#     cs_out = torch.as_tensor([fn_mo(s_tu[h_tu[:,ii]][:,~h_tu[:,ii]]) for ii in range(n_clusters)], device=DEVICE)
-    
-#     cs = cs_in / cs_out
-
-#     if return_inAndOut:
-#         return cs, cs_in, cs_out
-#     else:
-#         return cs
-
-
-# def cluster_similarity_score(
-#     s,
-#     h,
-#     locality=1,
-#     method_in='mean',
-#     method_out='max',
-# ):
-#     """
-#     Function to compute the aggregated similarity / dispersion score 
-#      of clusters.
-#     Here, the score measures the similarity between samples within
-#      a cluster and between samples within a cluster and all other samples.
-#     To compute a true silhouette score, use:
-#      method_in='mean' and method_out='max'.
-#     For a score similar to complete linkage, use:
-#      method_in='min' and method_out='max'.
-
-#     RH 2022
-
-#     Args:
-#         s (torch.Tensor, dtype float):
-#             The similarity matrix.
-#             shape: (n_samples, n_samples)
-#         h (torch.Tensor, dtype bool):
-#             The cluster membership matrix.
-#             shape: (n_samples, n_clusters)
-#         locality (float):
-#             The exponent applied to the similarity matrix.
-#             Higher values make the score more dependent on local 
-#              similarity. 
-#             Setting method_out to 'mean' and using a high locality 
-#              value can result in something similar to a silhouette
-#              score.
-#         method_in (str):
-#             The method used to compute the within-cluster similarity.
-#             Must be one of "mean", "max", "min".
-#         method_out (str):
-#             The method used to compute the between-cluster similarity.
-#             Must be one of "mean", "max", "min".
-#     """
-
-
-#     n_clusters = h.shape[1]
-#     n_samples = h.shape[0]
-    
-#     DEVICE = s.device
-#     s_tu = (s**locality).type(torch.float32)
-#     h_tu = h.to(DEVICE)
-
- 
-#     ii_normFactor = lambda i   : i * (i-1)
-#     ij_normFactor = lambda i,j : i * j
-
-#     yy, xx = torch.meshgrid(torch.arange(n_clusters), torch.arange(n_clusters), indexing='ij')
-#     yyf, xxf = yy.reshape(-1), xx.reshape(-1)
-
-#     sizes_clusters = h_tu.sum(0)
-
-#     if method_in=='mean' and method_out=='mean':
-#         s_tu[torch.arange(n_samples).to(DEVICE), torch.arange(n_samples).to(DEVICE)] = 0
-#         c = torch.einsum('ab, ac, bd -> cd', s_tu, h_tu, h_tu)  /  \
-#             ( (torch.eye(n_clusters).to(DEVICE) * ii_normFactor(sizes_clusters)) + ((1-torch.eye(n_clusters).to(DEVICE)) * (sizes_clusters[None,:] * sizes_clusters[:,None])) )
-#         return c
-
-
-#     if h.dtype != torch.bool:
-#         raise ValueError('h must be a boolean tensor.')
-
-#     s_tu[torch.arange(n_samples).to(DEVICE), torch.arange(n_samples).to(DEVICE)] = torch.nan
-    
-#     if method_in == 'mean':
-#         fn_mi = torch.nanmean
-#     elif method_in == 'max':
-#         fn_mi = torch_helpers.nanmax
-#     elif method_in == 'min':
-#         fn_mi = torch_helpers.nanmin
-#     else:
-#         raise ValueError('method_in must be one of "mean", "max", "min".')
-
-#     if method_out == 'mean':
-#         fn_mo = torch.nanmean
-#     elif method_out == 'max':
-#         fn_mo = torch_helpers.nanmax
-#     elif method_out == 'min':
-#         fn_mo = torch_helpers.nanmin
-#     else:
-#         raise ValueError('method_out must be one of "mean", "max", "min".')
-
-#     c = torch.as_tensor([fn_mo(s_tu[h_tu[:,ii]][:, h_tu[:,jj]]) for ii,jj in tqdm(zip(yyf, xxf), total=len(yyf))], device=DEVICE).reshape(n_clusters, n_clusters)
-#     c[torch.eye(n_clusters, dtype=torch.bool)] = torch.as_tensor([fn_mi(s_tu[h_tu[:,ii]][:, h_tu[:,ii]]) for ii in range(n_clusters)], device=DEVICE)
-
-#     return c
-
-
 # class Constrained_rich_clustering:
 #     """
 #     Class to perform constrained cluster assignment.
 #     This method takes in putative clusters, a cluster similarity matrix,
 #      and a vector of cluster 'scores' describing how valuable each
 #      cluster is. It then attempts to find an optimal combination of
 #      clusters. This is done by minimizing inclusion of similar clusters
```

### Comparing `bnpm-0.2.0/bnpm/container_helpers.py` & `bnpm-0.2.1/bnpm/container_helpers.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,61 +1,64 @@
 import re
 import copy
 from collections.abc import MutableMapping
+from typing import Any, Optional, Union, List, Dict, Tuple, Callable, Iterable, Sequence
 
 import numpy as np
 
 """
 This module is intended to have minimal dependencies.
 It is called by server.py which is intended to run
  outside of a specialized environment, so no weird
  libraries should be required.
 RH 2022
 """
 
-class Lazy_repeat_item():
+class lazy_repeat_obj():
     """
-    Makes a lazy iterator that repeats an item.
-    Very similar to itertools.repeat, but allows
-     for a pseudo length to be specified.
-     RH 2021
+    Makes a lazy iterator that repeats an object.
+    RH 2021
+
+    Args:
+        obj (Any):
+            Object to repeat.
+        pseudo_length (int):
+            length of the iterator.
     """
-    def __init__(self, item, pseudo_length=None):
+    def __init__(
+        self, 
+        obj: Any, 
+        pseudo_length: Optional[int] = None,
+    ):
         """
-        Args:
-            item (any object):
-                item to repeat
-            pseudo_length (int):
-                length of the iterator.
+        Initializes the lazy iterator.
         """
-        super().__init__()
-        self.item = item
+        self.obj = obj
         self.pseudo_length = pseudo_length
 
     def __getitem__(self, i):
         """
         Args:
             i (int):
                 index of item to return.
                 Ignored if pseudo_length is None.
         """
         if self.pseudo_length is None:
-            return self.item
+            return self.obj
         elif i < self.pseudo_length:
-            return self.item
+            return self.obj
         else:
             raise IndexError('Index out of bounds')
 
-
     def __len__(self):
         return self.pseudo_length
 
     def __repr__(self):
         return repr(self.item)
-
+    
 
 def flatten_list(irregular_list):
     """
     Flattens a list of lists into a single list.
     Stolen from https://stackabuse.com/python-how-to-flatten-list-of-lists/
     RH 2022
```

### Comparing `bnpm-0.2.0/bnpm/cross_validation.py` & `bnpm-0.2.1/bnpm/cross_validation.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.2.0/bnpm/cupy_helpers.py` & `bnpm-0.2.1/bnpm/cupy_helpers.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.2.0/bnpm/decomposition.py` & `bnpm-0.2.1/bnpm/decomposition.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.2.0/bnpm/dtw.py` & `bnpm-0.2.1/bnpm/dtw.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.2.0/bnpm/email_helpers.py` & `bnpm-0.2.1/bnpm/email_helpers.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.2.0/bnpm/featurization.py` & `bnpm-0.2.1/bnpm/featurization.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.2.0/bnpm/file_helpers.py` & `bnpm-0.2.1/bnpm/file_helpers.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 import pickle
 import json
 import yaml
 from pathlib import Path
 import zipfile
 
 from tqdm import tqdm
@@ -592,14 +591,73 @@
     try:
         hasher.update(bytes.fromhex(hash_hex))
     except ValueError:
         return False
     return True
 
 
+def compare_file_hashes(
+    hash_dict_true,
+    dir_files_test=None,
+    paths_files_test=None,
+    verbose=True,
+):
+    """
+    Compares hashes of files in a directory or list of paths
+     to user provided hashes.
+    RH 2022
+
+    Args:
+        hash_dict_true (dict):
+            Dictionary of hashes to compare to.
+            Each entry should be:
+                {'key': ('filename', 'hash')}
+        dir_files_test (str):
+            Path to directory to compare hashes of files in.
+            Unused if paths_files_test is not None.
+        paths_files_test (list of str):
+            List of paths to files to compare hashes of.
+            Optional. dir_files_test is used if None.
+        verbose (bool):
+            Whether or not to print out failed comparisons.
+
+    Returns:
+        total_result (bool):
+            Whether or not all hashes were matched.
+        individual_results (list of bool):
+            Whether or not each hash was matched.
+        paths_matching (dict):
+            Dictionary of paths that matched.
+            Each entry is:
+                {'key': 'path'}
+    """
+    if paths_files_test is None:
+        if dir_files_test is None:
+            raise ValueError('Must provide either dir_files_test or path_files_test.')
+        
+        ## make a dict of {filename: path} for each file in dir_files_test
+        files_test = {filename: (Path(dir_files_test).resolve() / filename).as_posix() for filename in path_helpers.get_dir_contents(dir_files_test)[1]} 
+    
+    paths_matching = {}
+    results_matching = {}
+    for key, (filename, hash) in hash_dict_true.items():
+        match = True
+        if filename not in files_test:
+            print(f'{filename} not found in test directory: {dir_files_test}.') if verbose else None
+            match = False
+        elif hash != hash_file(files_test[filename]):
+            print(f'{filename} hash mismatch with {key, filename}.') if verbose else None
+            match = False
+        if match:
+            paths_matching[key] = files_test[filename]
+        results_matching[key] = match
+
+    return all(results_matching.values()), results_matching, paths_matching
+
+
 def extract_zip(
     path_zipFile,
     path_extract=None,
     mkdir=True,
     verbose=True,
 ):
     """
```

### Comparing `bnpm-0.2.0/bnpm/h5_handling.py` & `bnpm-0.2.1/bnpm/h5_handling.py`

 * *Files 0% similar despite different names*

```diff
@@ -205,15 +205,17 @@
                     sub_dict[keys[-1]] = node[...]
                 elif isinstance(node, h5py.Group):
                     sub_dict.setdefault(keys[-1], {})
 
             h5_file.visititems(visitor_func)            
             return result
     else:
-        return h5py.File(filepath, 'r')
+        result = h5py.File(filepath, 'r')
+        show_item_tree(result) if verbose else None
+        return result
 
 def h5Obj_to_dict(hObj):
     '''
     Converts an h5py object to a python dict object
     RH 2023
     '''
     h5_dict = {}
```

### Comparing `bnpm-0.2.0/bnpm/image_processing.py` & `bnpm-0.2.1/bnpm/image_processing.py`

 * *Files 7% similar despite different names*

```diff
@@ -455,14 +455,78 @@
         return warped_sparse_image
     
     wsi_partial = partial(warp_sparse_image, remappingIdx=remappingIdx)
     ims_sparse_out = parallel_helpers.map_parallel(func=wsi_partial, args=(ims_sparse,), method='multithreading', workers=n_workers, prog_bar=verbose)
     return ims_sparse_out
 
 
+def remap_points(
+    points: np.ndarray, 
+    remappingIdx: np.ndarray,
+    interpolation: str = 'linear',
+    fill_value: float = None,
+) -> np.ndarray:
+    """
+    Remaps a set of points using an index map.
+
+    Args:
+        points (np.ndarray): 
+            Array of points to be remapped. It should be a 2D array with the
+            shape *(n_points, 2)*, where each point is represented by a pair of
+            floating point coordinates within the image.
+        remappingIdx (np.ndarray): 
+            Index map for the remapping. It should be a 3D array with the shape
+            *(height, width, 2)*. The data type should be a floating point
+            subtype.
+        interpolation (str):
+            Interpolation method to use.
+            See scipy.interpolate.RegularGridInterpolator. Can be:
+                * ``'linear'``
+                * ``'nearest'``
+                * ``'slinear'``
+                * ``'cubic'``
+                * ``'quintic'``
+                * ``'pchip'``
+        fill_value (float, optional):
+            Value used to fill points outside the convex hull. If ``None``, values
+            outside the convex hull are extrapolated.
+
+    Returns:
+        (np.ndarray): 
+            points_remap (np.ndarray): 
+                Remapped points array. It has the same shape as the input.
+    """
+    ### Assert points is a 2D numpy.ndarray of shape (n_points, 2) and that all points are within the image and that points are float
+    assert isinstance(points, np.ndarray), 'points must be a numpy.ndarray'
+    assert points.ndim == 2, 'points must be a 2D numpy.ndarray'
+    assert points.shape[1] == 2, 'points must be of shape (n_points, 2)'
+    assert np.issubdtype(points.dtype, np.floating), 'points must be a float subtype'
+
+    assert isinstance(remappingIdx, np.ndarray), 'remappingIdx must be a numpy.ndarray'
+    assert remappingIdx.ndim == 3, 'remappingIdx must be a 3D numpy.ndarray'
+    assert remappingIdx.shape[2] == 2, 'remappingIdx must be of shape (height, width, 2)'
+    assert np.issubdtype(remappingIdx.dtype, np.floating), 'remappingIdx must be a float subtype'
+
+    ## Make grid of indices for image remapping
+    dims = remappingIdx.shape
+    x_arange, y_arange = np.arange(0., dims[1]).astype(np.float32), np.arange(0., dims[0]).astype(np.float32)
+
+    ## Use RegularGridInterpolator to remap points
+    warper = scipy.interpolate.RegularGridInterpolator(
+        points=(y_arange, x_arange),
+        values=remappingIdx,
+        method=interpolation,
+        bounds_error=False,
+        fill_value=fill_value,
+    )
+    points_remap = warper(xi=(points[:, 1], points[:, 0]))
+
+    return points_remap
+
+
 def invert_remappingIdx(
     remappingIdx: np.ndarray, 
     method: str = 'linear', 
     fill_value: typing.Optional[float] = np.nan
 ) -> np.ndarray:
     """
     Inverts a remapping index field.
@@ -725,15 +789,14 @@
     assert isinstance(ri, torch.Tensor), f"ri must be a torch.Tensor. Got {type(ri)}"
     im_shape = torch.flipud(torch.as_tensor(ri.shape[:2], dtype=torch.float32, device=ri.device))  ## (W, H)
     normgrid = ((ri / (im_shape[None, None, :] - 1)) - 0.5) * 2  ## PyTorch's grid_sample expects grid values in [-1, 1] because it's a relative offset from the center pixel. CV2's remap expects grid values in [0, 1] because it's an absolute offset from the top-left pixel.
     ## note also that pytorch's grid_sample expects align_corners=True to correspond to cv2's default behavior.
     return normgrid
 
 
-
 @torch.jit.script
 def phase_correlation_helper(
     im_template,
     im_moving,
     mask_fft=None, 
     compute_maskFFT: bool=False, 
     template_precomputed: bool=False,
@@ -1355,15 +1418,19 @@
     
     if font is None:
         font = cv2.FONT_HERSHEY_SIMPLEX
     
     images_cp = copy.deepcopy(images)
     for i_f, frame in enumerate(images_cp):
         for i_t, t in enumerate(text[i_f]):
-            cv2.putText(frame, t, [position[0] , position[1] + i_t*font_size*30], font, font_size, color, line_width)
+            fn_putText = lambda frame_gray: cv2.putText(frame_gray, t, [position[0] , position[1] + i_t*font_size*30], font, font_size, color, line_width)
+            if frame.ndim == 3:
+                [fn_putText(frame[:,:,ii]) for ii in range(frame.shape[2])]
+            else:
+                fn_putText(frame)
         if show:
             cv2.imshow('add_text_to_images', frame)
             cv2.waitKey(int(1000/frameRate))
     
     if show:
         cv2.destroyWindow('add_text_to_images')
     return images_cp
@@ -1466,8 +1533,78 @@
     workers = mp.cpu_count() if workers == -1 else workers
     n_args = len(images)
 
     if workers == 1:
         return np.stack([apply_shifts_frame(*args) for args in zip(images, xShifts, yShifts)], axis=0)
 
     with ThreadPoolExecutor(workers) as ex:
-        return np.stack(list(tqdm(ex.map(apply_shifts_frame, *(images, xShifts, yShifts)), total=n_args, disable=prog_bar!=True)), axis=0)
+        return np.stack(list(tqdm(ex.map(apply_shifts_frame, *(images, xShifts, yShifts)), total=n_args, disable=prog_bar!=True)), axis=0)
+    
+
+def resize_images(
+    images, 
+    new_shape=(100,100),
+    interpolation='linear',
+    antialias=False,
+    align_corners=False,
+    device='cpu',
+):
+    """
+    Resize images.
+    Uses torch.nn.functional.interpolate.
+    RH 2023
+
+    Args:
+        images (np.array or list):
+            frames of video or images.
+            Can be 2D, 3D, or 4D
+            2D shape: (height, width)
+            3D shape: (n_frames, height, width)
+            4D shape: (n_frames, height, width, n_channels)
+        new_shape (tuple):
+            (height, width) of resized images.
+        interpolation (str):
+            interpolation method to use.
+            See torch.nn.functional.interpolate for options.
+        antialias (bool):
+            if True, then will use antialiasing.
+        align_corners (bool):
+            if True, then will align corners.
+            See torch.nn.functional.interpolate for details.
+        device (str):
+            device to use for torch.nn.functional.interpolate.
+            
+    Returns:
+        images_resized (np.array):
+            frames of video or images with overlay added.
+    """
+    if isinstance(images, list):
+        images = np.stack(images, axis=0)
+    
+    if images.ndim == 2:
+        images = images[None,:,:]
+    elif images.ndim == 3:
+        images = images
+    elif images.ndim == 4:
+        images = images.transpose(0,3,1,2)
+    else:
+        raise ValueError('images must be 2D, 3D, or 4D.')
+    
+    images_torch = torch.as_tensor(images, device=device)
+    images_torch = torch.nn.functional.interpolate(
+        images_torch, 
+        size=tuple(np.array(new_shape, dtype=int)), 
+        mode=interpolation,
+        align_corners=align_corners,
+        recompute_scale_factor=None,
+        antialias=antialias,
+    )
+    images_resized = images_torch.cpu().numpy()
+    
+    if images.ndim == 2:
+        images_resized = images_resized[0,:,:]
+    elif images.ndim == 3:
+        images_resized = images_resized
+    elif images.ndim == 4:
+        images_resized = images_resized.transpose(0,2,3,1)
+    
+    return images_resized
```

### Comparing `bnpm-0.2.0/bnpm/indexing.py` & `bnpm-0.2.1/bnpm/indexing.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.2.0/bnpm/linear_regression.py` & `bnpm-0.2.1/bnpm/linear_regression.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.2.0/bnpm/math_functions.py` & `bnpm-0.2.1/bnpm/math_functions.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.2.0/bnpm/misc.py` & `bnpm-0.2.1/bnpm/misc.py`

 * *Files 22% similar despite different names*

```diff
@@ -132,119 +132,14 @@
         nums (np.array):
             List of numbers found in the string.
 
     """
     return np.array([float(i) for i in re.findall(r'\-?\d+\.?\d*', str_in)], dtype=dtype_out)
 
 
-def hash_file(path, type_hash='MD5', buffer_size=65536):
-    """
-    Gets hash of a file.
-    Based on: https://stackoverflow.com/questions/22058048/hashing-a-file-in-python
-    RH 2022
-
-    Args:
-        path (str):
-            Path to file to be hashed.
-        type_hash (str):
-            Type of hash to use. Can be:
-                'MD5'
-                'SHA1'
-                'SHA256'
-                'SHA512'
-        buffer_size (int):
-            Buffer size for reading file.
-            65536 corresponds to 64KB.
-
-    Returns:
-        hash (str):
-            Hash of file.
-    """
-
-    if type_hash == 'MD5':
-        hasher = hashlib.md5()
-    elif type_hash == 'SHA1':
-        hasher = hashlib.sha1()
-    elif type_hash == 'SHA256':
-        hasher = hashlib.sha256()
-    elif type_hash == 'SHA512':
-        hasher = hashlib.sha512()
-    else:
-        raise ValueError(f'{type_hash} is not a valid hash type.')
-
-    with open(path, 'rb') as f:
-        while True:
-            data = f.read(buffer_size)
-            if not data:
-                break
-            hasher.update(data)
-
-    hash = hasher.hexdigest()
-        
-    return hash
-
-
-def compare_file_hashes(
-    hash_dict_true,
-    dir_files_test=None,
-    paths_files_test=None,
-    verbose=True,
-):
-    """
-    Compares hashes of files in a directory or list of paths
-     to user provided hashes.
-    RH 2022
-
-    Args:
-        hash_dict_true (dict):
-            Dictionary of hashes to compare to.
-            Each entry should be:
-                {'key': ('filename', 'hash')}
-        dir_files_test (str):
-            Path to directory to compare hashes of files in.
-            Unused if paths_files_test is not None.
-        paths_files_test (list of str):
-            List of paths to files to compare hashes of.
-            Optional. dir_files_test is used if None.
-        verbose (bool):
-            Whether or not to print out failed comparisons.
-
-    Returns:
-        total_result (bool):
-            Whether or not all hashes were matched.
-        individual_results (list of bool):
-            Whether or not each hash was matched.
-        paths_matching (dict):
-            Dictionary of paths that matched.
-            Each entry is:
-                {'key': 'path'}
-    """
-    if paths_files_test is None:
-        if dir_files_test is None:
-            raise ValueError('Must provide either dir_files_test or path_files_test.')
-        
-        ## make a dict of {filename: path} for each file in dir_files_test
-        files_test = {filename: (Path(dir_files_test).resolve() / filename).as_posix() for filename in path_helpers.get_dir_contents(dir_files_test)[1]} 
-    
-    paths_matching = {}
-    results_matching = {}
-    for key, (filename, hash) in hash_dict_true.items():
-        match = True
-        if filename not in files_test:
-            print(f'{filename} not found in test directory: {dir_files_test}.') if verbose else None
-            match = False
-        elif hash != hash_file(files_test[filename]):
-            print(f'{filename} hash mismatch with {key, filename}.') if verbose else None
-            match = False
-        if match:
-            paths_matching[key] = files_test[filename]
-        results_matching[key] = match
-
-    return all(results_matching.values()), results_matching, paths_matching
-
 def write_to_log(
     text, 
     path_log, 
     mode='a', 
     start_on_new_line=True, 
     pref_print=True, 
     pref_save=True
```

### Comparing `bnpm-0.2.0/bnpm/other_peoples_code.py` & `bnpm-0.2.1/bnpm/other_peoples_code.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.2.0/bnpm/parallel_helpers.py` & `bnpm-0.2.1/bnpm/parallel_helpers.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.2.0/bnpm/path_helpers.py` & `bnpm-0.2.1/bnpm/path_helpers.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.2.0/bnpm/plotting_helpers.py` & `bnpm-0.2.1/bnpm/plotting_helpers.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,17 @@
+from pathlib import Path
+import tkinter as tk
+import PIL
+from PIL import ImageTk
+import csv
+
 from matplotlib import pyplot as plt
 import numpy as np
-
 import cv2
 
-from tqdm.notebook import tqdm
-
-from ipywidgets import widgets
-import IPython.display as Disp
-
-from pathlib import Path
-
 
 ###############
 #### PLOTS ####
 ###############
 
 def plot_image_grid(images, labels=None, grid_shape=(10,10), show_axis='off', cmap=None, kwargs_subplots={}, kwargs_imshow={}):
     """
@@ -43,20 +41,20 @@
         axs:
             Axes
     """
     if cmap is None:
         cmap = 'viridis'
 
     fig, axs = plt.subplots(nrows=grid_shape[0], ncols=grid_shape[1], **kwargs_subplots)
-    idx_axs = get_subplot_indices(axs)
-    for ii,idx_ax in enumerate(idx_axs):
-        axs[idx_ax].imshow(images[ii], cmap=cmap, **kwargs_imshow);
+    axs_flat = axs.flatten(order='F') if isinstance(axs, np.ndarray) else [axs]
+    for ii, ax in enumerate(axs_flat[:len(images)]):
+        ax.imshow(images[ii], cmap=cmap, **kwargs_imshow);
         if labels is not None:
-            axs[idx_ax].set_title(labels[ii]);
-        axs[idx_ax].axis(show_axis);
+            ax.set_title(labels[ii]);
+        ax.axis(show_axis);
     return fig, axs
 
 
 def widget_toggle_image_stack(images, labels=None, clim=None, figsize=None):
     """
     Scrub through iamges in a stack using a slider.
     Requires %matplotlib notebook or %matplotlib widget
@@ -582,47 +580,24 @@
 
         ## Get colors
         colors = self.fn_conj_cmap(x)
         colors = (colors * (self.normalization_range[1] - self.normalization_range[0]) + self.normalization_range[0]).astype(self.dtype_out)
 
         return colors
 
-def savefig(path, dpi=300, mkdir=True, **kwargs_savefig):
-    """
-    Save figure.
-    RH 2022
-
-    Args:
-        path (str):
-            Path to save figure to.
-            Format is inferred from path suffix.
-        dpi (int):
-            DPI of figure.
-        **kwargs_savefig:
-            Keyword arguments to pass to `matplotlib.pyplot.savefig`.
-    """
-
-    assert len(Path(path).suffix) > 0, 'RH Error: Path must have a suffix'
-    kind = Path(path).suffix[1:]
-
-    if mkdir:
-        Path(path).parent.mkdir(exist_ok=True, parents=True)
-
-    plt.savefig(path, format=kind, dpi=dpi, **kwargs_savefig)
-
 
 class Figure_Saver:
     """
     Class for saving figures
     RH 2022
     """
     def __init__(
         self,
         dir_save: str=None,
-        format_save: list=['png'],
+        format_save: list=['png', 'svg'],
         kwargs_savefig: dict={
             'bbox_inches': 'tight',
             'pad_inches': 0.1,
             'transparent': True,
             'dpi': 300,
         },
         overwrite: bool=False,
@@ -873,8 +848,243 @@
     def _new_ROI(self, _):
         """
         Start a new ROI.
         """
         self.selected_points.append(self._selected_points_last_ROI)
         self._selected_points_last_ROI = []
         
+    
+class Image_labeler:
+    """
+    A simple graphical interface for labeling image classes.
+    Use this class with a context manager to ensure that the
+     window is closed properly. See demo below.
+    This class provides a tkinter window which displays images
+     from a provided numpy array one by one and lets you classify
+     each image by pressing a key. 
+    The title of the window is the image index.
+    The classification label and image index are stored as
+     self.labels_ and saved to a CSV file in self.path_csv.
+    RH 2023
+
+    Demo:
+    with Image_labeler(images, start_index=0, resize_factor=4.0, key_end='Escape') as labeler:
+        labeler.run()
+    path_csv, labels = labeler.path_csv, labeler.labels_
+
+    Args:
+        images (np.ndarray): 
+            A numpy array of images.
+            Either 3D: (n_images, height, width) or
+             4D: (n_images, height, width, n_channels).
+            Images should be scaled between 0 and 255 and will be
+             converted to uint8.
+        start_index (int): 
+            The index of the first image to display. Default is 0.
+        path_csv (str): 
+            A string of the path to the CSV file for saving results.
+            If None, results will not be saved.
+        save_csv (bool):
+            A boolean indicating whether to save the results to a CSV.
+        resize_factor (float): 
+            A scaling factor indicating the fractional change in 
+             image size. Default is 1.0 (no change).
+        key_end (str): 
+            A string of the key to press to end the session.
+        key_prev (str):
+            A string of the key to press to go back to the previous
+             image.
+        key_next (str):
+            A string of the key to press to go to the next image.
+        normalize_images (bool):
+            A boolean indicating whether to normalize the images
+             between min and max values. Default is True.
+        verbose (bool):
+            A boolean indicating whether to print status updates.
+    """
+
+    def __init__(
+        self, 
+        image_array: np.ndarray, 
+        start_index: int=0,
+        path_csv: str=None, 
+        save_csv: bool=True,
+        resize_factor: float=10.0, 
+        normalize_images: bool=True,
+        verbose: bool=True,
+        key_end: str='Escape', 
+        key_prev: str='Left',
+        key_next: str='Right',
+    ):
+        """
+        Initializes class with images, path to save csv and UI
+         elements.
+        Binds keys for classifying images and ending the session.
+        """
+        import tempfile
+        import datetime
+        ## Set attributes
+        self.images = image_array
+        self._resize_factor = resize_factor
+        self._index = start_index - 1  ## -1 because we increment before displaying
+        self.path_csv = path_csv if path_csv is not None else str(Path(tempfile.gettempdir()) / ('roicat_labels_' + datetime.datetime.now().strftime("%Y%m%d_%H%M%S") + '.csv'))
+        self._save_csv = save_csv
+        self.labels_ = {}
+        self._img_tk = None
+        self._key_end = key_end if key_end is not None else None
+        self._key_prev = key_prev if key_prev is not None else None
+        self._key_next = key_next if key_next is not None else None
+        self._normalize_images = normalize_images
+        self._verbose = verbose
+
+        self.__call__ = self.run
         
+    def run(self):
+        """
+        Runs the image labeler. Opens a tkinter window and displays
+         the first image.
+        """
+        try:
+            self._root = tk.Tk()
+            self._img_label = tk.Label(self._root)
+            self._img_label.pack()
+
+            ## Bind keys
+            self._root.bind("<Key>", self.classify)
+            self._root.bind('<Key-' + self._key_end + '>', self.end_session) if self._key_end is not None else None
+            self._root.bind('<Key-' + self._key_prev + '>', self.prev_img) if self._key_prev is not None else None
+            self._root.bind('<Key-' + self._key_next + '>', self.next_img) if self._key_next is not None else None
+
+            ## Start the session
+            self.next_img()
+            self._root.mainloop()
+        except Exception as e:
+            warnings.warn('Error initializing image labeler: ' + str(e))
+
+    def __enter__(self):
+        return self
+    def __exit__(self, exc_type, exc_value, traceback):
+        self.end_session(None)
+
+    def next_img(self, event=None):
+        """Displays the next image in the array, and resizes the image."""
+        ## Display the image
+        ### End the session if there are no more images
+        self._index += 1
+        if self._index < len(self.images):
+            im = self.images[self._index]
+            im = (im / np.max(im)) * 255 if self._normalize_images else im
+            pil_img = PIL.Image.fromarray(np.uint8(im))  ## Convert to uint8 and PIL image
+            ## Resize image
+            width, height = pil_img.size
+            new_width = int(width * self._resize_factor)
+            new_height = int(height * self._resize_factor)
+            pil_img = pil_img.resize((new_width, new_height), resample=PIL.Image.LANCZOS)
+            ## Display image
+            self._img_tk = ImageTk.PhotoImage(pil_img)
+            self._img_label.image = self._img_tk  # keep a reference to the PhotoImage object
+            self._img_label.config(image=self._img_label.image)
+        else:
+            self.end_session(None)
+        
+        self._root.title(str(self._index))  # update the window title to the current image index
+
+    def prev_img(self, event=None):
+        """
+        Displays the previous image in the array.
+        """
+        self._index -= 2
+        self.next_img()
+
+    def classify(self, event):
+        """
+        Adds the current image index and pressed key as a label.
+        Then saves the results and moves to the next image.
+
+        Args:
+            event (tkinter.Event):
+                A tkinter event object.
+        """
+        label = event.char
+        if label != '':
+            print(f'Image {self._index}: {label}') if self._verbose else None
+            self.labels_.update({self._index: str(label)})  ## Store the label
+            self.save_classification() if self._save_csv else None ## Save the results
+            self.next_img()  ## Move to the next image
+
+    def end_session(self, event):
+        """Ends the classification session by destroying the tkinter window."""
+        self._img_tk = None
+        self._root.destroy() if self._root is not None else None
+        self._root = None
+        
+        import gc
+        gc.collect()
+        gc.collect()
+
+    def save_classification(self):
+        """
+        Saves the classification results to a CSV file.
+        This function does not append, it overwrites the entire file.
+        The file contains two columns: 'image_index' and 'label'.
+        """
+        ## make directory if it doesn't exist
+        Path(self.path_csv).parent.mkdir(parents=True, exist_ok=True)
+        ## Save the results
+        with open(self.path_csv, 'w', newline='') as f:
+            writer = csv.writer(f)
+            writer.writerow(('image_index', 'label'))
+            writer.writerows(self.labels_.items())
+
+    def get_labels(self, kind='dict',):
+        """
+        Returns a dictionary of the labels.
+        The keys are the image indices and the values are the labels.
+
+        Args:
+            kind (str):
+                A string indicating the type of object to return.
+                'dict': {idx: label, idx: label, ...}
+                'list': [(idx, label), (idx, label), ...]
+                'dataframe': {'index': [idx, idx, ...], 'label': [label, label, ...]}
+                    This can be converted to a pandas dataframe with:
+                     pd.DataFrame(self.get_labels('dataframe'))
+        """
+        ## if the dict is empty, return None
+        if len(self.labels_) == 0:
+            return None
+        
+        if kind == 'dict':
+            # out = dict(self.labels_)
+            # ## Check for duplicate indices
+            # if len(out) != len(self.labels_):
+            #     warnings.warn('Duplicate indices found in labels. Only the last label for each index is returned.')
+            # return out
+            return self.labels_
+        elif kind == 'list':
+            # return self.labels_
+            return self.labels_.items()
+        elif kind == 'dataframe':
+            # return {'index': np.array([x[0] for x in self.labels_], dtype=np.int64), 'label': np.array([x[1] for x in self.labels_])}
+            return {'index': np.array(list(self.labels_.keys()), dtype=np.int64), 'label': np.array(list(self.labels_.values()), dtype=str)}
+
+
+########################################################################################################################
+########################################## OTHER PLOTTING LIBRARIES ####################################################
+########################################################################################################################
+
+def export_svg_hv_bokeh(obj, path_save):
+    """
+    Save a scatterplot from holoviews as an svg file.
+    RH 2023
+
+    Args:
+        obj (holoviews.plotting.bokeh.ElementPlot):
+            Holoviews plot object.
+        path_save (str):
+            Path to save the svg file.
+    """
+    import holoviews as hv
+    import bokeh
+    plot_state = hv.renderer('bokeh').get_plot(obj).state
+    plot_state.output_backend = 'svg'
+    bokeh.io.export_svgs(plot_state, filename=path_save)
```

### Comparing `bnpm-0.2.0/bnpm/resource_tracking.py` & `bnpm-0.2.1/bnpm/resource_tracking.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.2.0/bnpm/server.py` & `bnpm-0.2.1/bnpm/server.py`

 * *Files 0% similar despite different names*

```diff
@@ -123,15 +123,15 @@
     n_jobs = max(len(paths_scripts), len(params_list), len(sbatch_config_list))
     if max_n_jobs is not None:
         if n_jobs > max_n_jobs:
             raise ValueError(f'Too many jobs requested: max_n_jobs={max_n_jobs} > n_jobs={n_jobs}')
 
     def rep_inputs(item, n_jobs):
         if len(item)==1 and (n_jobs>1):
-            return container_helpers.Lazy_repeat_item(item[0], pseudo_length=n_jobs)
+            return container_helpers.Lazy_repeat_obj(item[0], pseudo_length=n_jobs)
         else:
             return item
 
     paths_scripts      = rep_inputs(paths_scripts,   n_jobs)
     params_list        = rep_inputs(params_list,  n_jobs)
     sbatch_config_list = rep_inputs(sbatch_config_list, n_jobs)
     name_save          = rep_inputs([name_save], n_jobs)
```

### Comparing `bnpm-0.2.0/bnpm/similarity.py` & `bnpm-0.2.1/bnpm/similarity.py`

 * *Files 6% similar despite different names*

```diff
@@ -812,40 +812,7 @@
     for n in path_membership: 
         problem += pulp.lpSum(path_vars[path] for path in path_membership[n]) <= 1
         
     # solve and extract results
     problem.solve()
     matching = [p for p,v in path_vars.items() if v.value()==1]
     return matching
-
-
-##############################################################
-######### NUMBA implementations of simple algorithms #########
-##############################################################
-
-@njit(parallel=True)
-def vectorProjection_numba(v1, v2):
-    proj_score = np.dot(v1, v2) / (np.linalg.norm(v2)**2)
-    proj_vec = v2 * proj_score
-    return proj_vec, proj_score
-
-@njit(parallel=True)
-def mean_numba(X):
-    Y = np.zeros(X.shape[0], dtype=X.dtype)
-    for ii in prange(X.shape[0]):
-        Y[ii] = np.mean(X[ii,:])
-    return Y
-
-@njit(parallel=True)
-def sum_numba(X):
-    Y = np.zeros(X.shape[0], dtype=X.dtype)
-    for ii in prange(X.shape[0]):
-        Y[ii] = np.sum(X[ii,:])
-    return Y
-
-@njit(parallel=True)
-def var_numba(X):
-    Y = np.zeros(X.shape[0], dtype=X.dtype)
-    for ii in prange(X.shape[0]):
-        Y[ii] = np.var(X[ii,:])
-    return Y
-
```

### Comparing `bnpm-0.2.0/bnpm/spectral.py` & `bnpm-0.2.1/bnpm/spectral.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,12 @@
-'''
-Table of Contents
-
-Functions and Interdependencies:
-    butter_bandpass
-    butter_bandpass_filter
-        - butter_bandpass
-    mtaper_specgram
-    simple_cwt
-'''
-
-import math
-from re import S
 import scipy.signal
 import numpy as np
 import matplotlib.pyplot as plt
 import torch
-from . import math_functions, timeSeries, indexing
+from . import math_functions, indexing
 from tqdm import tqdm
 
 
 def design_butter_bandpass(lowcut, highcut, fs, order=5, plot_pref=True):
     '''
     designs a butterworth bandpass filter.
     Makes a lowpass filter if lowcut is 0.
```

### Comparing `bnpm-0.2.0/bnpm/stats.py` & `bnpm-0.2.1/bnpm/stats.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.2.0/bnpm/timeSeries.py` & `bnpm-0.2.1/bnpm/timeSeries.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from typing import Any
 import numpy as np
 import time
 from matplotlib import pyplot as plt
 import copy
 from numba import njit, jit, prange
 import pandas as pd
 import torch
@@ -10,15 +9,14 @@
 from . import parallel_helpers
 from .parallel_helpers import multiprocessing_pool_along_axis
 from . import cross_validation
 from .math_functions import polar2cartesian, cartesian2polar, gaussian
 from . import indexing
 
 
-
 def convolve_along_axis(
     array,
     kernel, 
     axis=1 , 
     mode='same', 
     correct_edge_effects=True,
     multicore_pref=False, 
@@ -961,56 +959,8 @@
     remember to flip k
     '''
     y = np.empty_like(X)
     y.fill(np.nan)
     k_hs = k.size//2
     for ii in prange( k_hs , len(X)-(k_hs) ):
         y[ii] = np.dot(X[0+ii-k_hs : 1+ii+k_hs], k)
-    return y
-    
-
-@njit(parallel=True)
-def mean_numba(X):
-    Y = np.zeros(X.shape[0], dtype=X.dtype)
-    for ii in prange(X.shape[0]):
-        Y[ii] = np.mean(X[ii,:])
-    return Y
-
-
-@njit(parallel=True)
-def var_numba(X):
-    Y = np.zeros(X.shape[0], dtype=X.dtype)
-    for ii in prange(X.shape[0]):
-        Y[ii] = np.var(X[ii,:])
-    return Y
-
-
-@njit(parallel=True)
-def std_numba(X):
-    Y = np.zeros(X.shape[0], dtype=X.dtype)
-    for ii in prange(X.shape[0]):
-        Y[ii] = np.std(X[ii,:])
-    return Y
-
-
-@njit(parallel=True)
-def min_numba(X):
-    output = np.zeros(X.shape[0])
-    for ii in prange(X.shape[0]):
-        output[ii] = np.min(X[ii])
-    return output
-
-
-@njit(parallel=True)
-def max_numba(X):
-    output = np.zeros(X.shape[0])
-    for ii in prange(X.shape[0]):
-        output[ii] = np.max(X[ii])
-    return output
-
-@njit(parallel=True)
-def round_numba(x):
-    output = np.zeros_like(x)
-    for ii in prange(x.shape[0]):
-        for jj in prange(x.shape[1]):
-            output[ii,jj] = np.round(x[ii,jj])
-    return output
+    return y
```

### Comparing `bnpm-0.2.0/bnpm/torch_helpers.py` & `bnpm-0.2.1/bnpm/torch_helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -137,19 +137,14 @@
 
 def set_device(use_GPU=True, device_num=0, verbose=True):
     """
     Set torch.cuda device to use.
     Assumes that only one GPU is available or
      that you wish to use cuda:0 only.
     RH 2021
-
-    Args:
-        use_GPU (int):
-            If 1, use GPU.
-            If 0, use CPU.
     """
     if use_GPU:
         print(f'devices available: {[torch.cuda.get_device_properties(ii) for ii in range(torch.cuda.device_count())]}') if verbose else None
         device = f"cuda:{device_num}" if torch.cuda.is_available() else "cpu"
         if device == "cpu":
             print("no GPU available. Using CPU.") if verbose else None
         else:
```

### Comparing `bnpm-0.2.0/bnpm/video.py` & `bnpm-0.2.1/bnpm/video.py`

 * *Files 8% similar despite different names*

```diff
@@ -144,14 +144,100 @@
     if path_save is not None:
         writer.release()
         print('Video saved')
     if show:
         cv2.destroyWindow('handle')
 
 
+def grayscale_to_rgb(array):
+    """
+    Convert a grayscale image (2D array) or movie (3D array) to
+     RGB (3D or 4D array).
+    RH 2023
+
+    Args:
+        array (np.ndarray or torch.Tensor or list):
+            2D or 3D array of grayscale images
+    """
+    if isinstance(array, list):
+        if isinstance(array[0], np.ndarray):
+            array = np.stack(array, axis=0)
+        elif isinstance(array[0], torch.Tensor):
+            array = torch.stack(array, axis=0)
+        else:
+            raise Exception(f'Failed to convert list of type {type(array[0])} to array')
+    if isinstance(array, np.ndarray):
+        return np.stack([array, array, array], axis=-1)
+    elif isinstance(array, torch.Tensor):
+        return torch.stack([array, array, array], dim=-1)
+    
+
+def save_gif(
+    array, 
+    path, 
+    frameRate=5.0, 
+    loop=0, 
+    backend='PIL', 
+    kwargs_backend={},
+):
+    """
+    Save an array of images as a gif.
+    RH 2023
+
+    Args:
+        array (np.ndarray or list):
+            3D (grayscale) or 4D (color) array of images.
+            - if dtype is float type then scale from 0 to 1.
+            - if dtype is integer then scale from 0 to 255.
+        path (str):
+            Path to save the gif.
+        frameRate (float):
+            Frame rate of the gif.
+        loop (int):
+            Number of times to loop the gif.
+            0 mean loop forever
+            1 mean play once
+            2 means play twice (loop once)
+            etc.
+        backend (str):
+            Which backend to use.
+            Options: 'imageio' or 'PIL'
+        kwargs_backend (dict):
+            Keyword arguments for the backend.
+    """
+    array = np.stack(array, axis=0) if isinstance(array, list) else array
+    array = grayscale_to_rgb(array) if array.ndim == 3 else array
+    if np.issubdtype(array.dtype, np.floating):
+        array = (array*255).astype('uint8')
+    
+    kwargs_backend.update({'loop': loop} if loop != 1 else {})
+
+    if backend == 'imageio':
+        import imageio
+        imageio.mimsave(
+            path, 
+            array, 
+            format='GIF',
+            duration=1000/frameRate, 
+            **kwargs_backend,
+        )
+    elif backend == 'PIL':
+        from PIL import Image
+        frames = [Image.fromarray(array[i_frame]) for i_frame in range(array.shape[0])]
+        frames[0].save(
+            path, 
+            format='GIF', 
+            append_images=frames[1:], 
+            save_all=True, 
+            duration=1000/frameRate, 
+            **kwargs_backend,
+        )
+    else:
+        raise Exception(f'Unsupported backend {backend}')
+
 
 class VideoReaderWrapper(decord.VideoReader):
     """
     Used to fix a memory leak bug in decord.VideoReader
     Taken from here.
     https://github.com/dmlc/decord/issues/208#issuecomment-1157632702
     """
@@ -304,14 +390,17 @@
         self.method_getitem = method_getitem
 
         ## Get metadata about videos: lengths, fps, frame size, etc.
         self.metadata, self.num_frames_total, self.frame_rate, self.frame_height_width, self.num_channels = self._get_metadata(self.video_readers)
         ## Get number of videos
         self.num_videos = len(self.video_readers)
 
+        ## Set shape
+        self.shape = (self.num_frames_total, *self.frame_height_width, self.num_channels)
+
         ## Set iterator starting frame
         print(f"FR: Setting iterator starting frame to {starting_seek_position}") if self._verbose > 1 else None
         self.set_iterator_frame_idx(starting_seek_position)
 
         ## Initialize the buffer
         ### Make a list containing a slot for each buffer chunk
         self.slots = [[None] * np.ceil(len(d)/self.buffer_size).astype(int) for d in self.video_readers]
@@ -586,36 +675,37 @@
         idx_slot_lookuptable = np.where((self.lookup['video']==idx_slots[-1][0]) * (self.lookup['slot']==idx_slots[-1][1]))[0][0]
         if self.prefetch > 0:
             idx_slots_prefetch = [(self.lookup['video'][ii], self.lookup['slot'][ii]) for ii in range(idx_slot_lookuptable+1, idx_slot_lookuptable+self.prefetch+1) if ii < len(self.lookup)]
         else:
             idx_slots_prefetch = []
         ## Load the slots
         self._load_slots(idx_slots + idx_slots_prefetch, wait_for_load=[True]*len(idx_slots) + [False]*len(idx_slots_prefetch))
-        ## Delete the slots that are no longer needed. 
-        ### Find slots before the posthold to delete
-        idx_slots_delete = [(self.lookup['video'][ii], self.lookup['slot'][ii]) for ii in range(idx_slot_lookuptable-self.posthold) if ii >= 0]
-        ### Delete all previous slots
-        self._delete_slots(idx_slots_delete)
-        # ### All slots from old videos should be deleted.
-        # self._delete_slots([idx_slot for idx_slot in self.loaded if idx_slot[0] < idx_video])
-        # ### All slots from previous buffers should be deleted.
-        # self._delete_slots([idx_slot for idx_slot in self.loaded if idx_slot[0] == idx_video and idx_slot[1] < idx_frame_start // self.buffer_size])
 
         ## Get the frames from the slots
         idx_frames_slots = [slice(max(idx_frame_start - self.boundaries[idx_slot[0]][idx_slot[1]][0], 0), min(idx_frame_end - self.boundaries[idx_slot[0]][idx_slot[1]][0], self.buffer_size), idx_frame_step) for idx_slot in idx_slots]
         print(f"FR: Frames within slots: {idx_frames_slots}") if self._verbose > 1 else None
 
         ## Get the frames. Then concatenate them along the first dimension using torch.cat
         ### Skip the concatenation if there is only one slot
         if len(idx_slots) == 1:
             frames = self.slots[idx_slots[0][0]][idx_slots[0][1]][idx_frames_slots[0]]
         else:
             print(f"FR: Warning. Slicing across multiple slots is SLOW. Consider increasing buffer size or adjusting batching method.") if self._verbose > 1 else None
             frames = torch.cat([self.slots[idx_slot[0]][idx_slot[1]][idx_frames_slot] for idx_slot, idx_frames_slot in zip(idx_slots, idx_frames_slots)], dim=0)
         
+        ## Delete the slots that are no longer needed. 
+        ### Find slots before the posthold to delete
+        idx_slots_delete = [(self.lookup['video'][ii], self.lookup['slot'][ii]) for ii in range(idx_slot_lookuptable-self.posthold) if ii >= 0]
+        ### Delete all previous slots
+        self._delete_slots(idx_slots_delete)
+        # ### All slots from old videos should be deleted.
+        # self._delete_slots([idx_slot for idx_slot in self.loaded if idx_slot[0] < idx_video])
+        # ### All slots from previous buffers should be deleted.
+        # self._delete_slots([idx_slot for idx_slot in self.loaded if idx_slot[0] == idx_video and idx_slot[1] < idx_frame_start // self.buffer_size])
+
         # ## Squeeze if there is only one frame
         # frames = frames.squeeze(0) if frames.shape[0] == 1 else frames
 
         return frames
 
     def get_frames_from_continuous_index(self, idx):
         """
@@ -672,16 +762,30 @@
                  is the index of the frame in the entire sequence 
                  of frames.
         """
         self._iterator_frame = idx
         
     def __getitem__(self, idx):
         if self.method_getitem == 'by_video':
+            ## handle None values in the slice idx
+            if isinstance(idx, slice):
+                idx = slice(
+                    idx.start if idx.start is not None else 0,
+                    idx.stop if idx.stop is not None else self.num_videos,
+                    idx.step if idx.step is not None else 1,
+                )
             return self.get_frames_from_single_video_index(idx)
         elif self.method_getitem == 'continuous':
+            ## handle None values in the slice idx
+            if isinstance(idx, slice):
+                idx = slice(
+                    idx.start if idx.start is not None else 0,
+                    idx.stop if idx.stop is not None else self.num_frames_total,
+                    idx.step if idx.step is not None else 1,
+                )
             return self.get_frames_from_continuous_index(idx)
         else:
             raise ValueError(f"Invalid method_getitem: {self.method_getitem}")
 
     def __len__(self): 
         if self.method_getitem == 'by_video':
             return len(self.video_readers)
```

### Comparing `bnpm-0.2.0/bnpm/welford_moving.py` & `bnpm-0.2.1/bnpm/welford_moving.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.2.0/bnpm/welford_moving_2D.py` & `bnpm-0.2.1/bnpm/welford_moving_2D.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.2.0/bnpm.egg-info/PKG-INFO` & `bnpm-0.2.1/bnpm.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,39 @@
 Metadata-Version: 2.1
 Name: bnpm
-Version: 0.2.0
+Version: 0.2.1
 Summary: A library of useful modules for data analysis.
 Home-page: https://github.com/RichieHakim/basic_neural_processing_modules
 Author: Richard Hakim
 License: LICENSE
 Keywords: data analysis,machine learning,neuroscience
 Description-Content-Type: text/markdown
 Provides-Extra: advanced
 License-File: LICENSE
 
+[![PyPI version](https://badge.fury.io/py/bnpm.svg)](https://badge.fury.io/py/bnpm)
+[![Downloads](https://pepy.tech/badge/bnpm)](https://pepy.tech/project/bnpm)
 [![repo size](https://img.shields.io/github/repo-size/RichieHakim/basic_neural_processing_modules)](https://github.com/RichieHakim/basic_neural_processing_modules/)
 
 #  basic_neural_processing_modules 
 Personal library of functions used in analyzing neural data.
 If you find a bug or just want to reach out: RichHakim@gmail.com
 
 ## Installation 
 Normal installation of `bnpm` does not install all possible dependencies; there are some specific functions that wrap libraries that may need to be installed separately on a case-by-case basis.
 
-`pip install git+https://github.com/RichieHakim/basic_neural_processing_modules.git`
+Install stable version:
+```
+pip install bnpm
+```
+
+Install development version:
+```
+pip install git+https://github.com/RichieHakim/basic_neural_processing_modules.git
+```
 
 import with: `import bnpm`
 
 
 ## Usage 
 My favorites:
 - **`featurization.Toeplitz_convolution2d`**
```

### Comparing `bnpm-0.2.0/bnpm.egg-info/SOURCES.txt` & `bnpm-0.2.1/bnpm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bnpm-0.2.0/demos/slurmDispatcher.py` & `bnpm-0.2.1/demos/slurmDispatcher.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.2.0/setup.py` & `bnpm-0.2.1/setup.py`

 * *Files identical despite different names*

