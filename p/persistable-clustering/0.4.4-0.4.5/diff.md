# Comparing `tmp/persistable-clustering-0.4.4.tar.gz` & `tmp/persistable-clustering-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "persistable-clustering-0.4.4.tar", last modified: Wed Mar 29 20:25:22 2023, max compression
+gzip compressed data, was "persistable-clustering-0.4.5.tar", last modified: Sun Jul  2 18:46:30 2023, max compression
```

## Comparing `persistable-clustering-0.4.4.tar` & `persistable-clustering-0.4.5.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-29 20:25:22.804845 persistable-clustering-0.4.4/
--rw-r--r--   0 runner    (1001) docker     (116)     3198 2023-03-29 20:24:32.000000 persistable-clustering-0.4.4/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (116)     1469 2023-03-29 20:24:32.000000 persistable-clustering-0.4.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)      116 2023-03-29 20:24:32.000000 persistable-clustering-0.4.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)     8125 2023-03-29 20:25:22.804845 persistable-clustering-0.4.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     7186 2023-03-29 20:24:32.000000 persistable-clustering-0.4.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-29 20:25:22.800845 persistable-clustering-0.4.4/persistable/
--rw-r--r--   0 runner    (1001) docker     (116)       97 2023-03-29 20:24:32.000000 persistable-clustering-0.4.4/persistable/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     3411 2023-03-29 20:24:32.000000 persistable-clustering-0.4.4/persistable/_vineyard.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-29 20:25:22.800845 persistable-clustering-0.4.4/persistable/assets/
--rw-r--r--   0 runner    (1001) docker     (116)     4286 2023-03-29 20:24:32.000000 persistable-clustering-0.4.4/persistable/assets/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (116)     3325 2023-03-29 20:24:32.000000 persistable-clustering-0.4.4/persistable/assets/style.css
--rw-r--r--   0 runner    (1001) docker     (116)     1203 2023-03-29 20:24:32.000000 persistable-clustering-0.4.4/persistable/auxiliary.pyx
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-29 20:25:22.804845 persistable-clustering-0.4.4/persistable/borrowed/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-03-29 20:24:32.000000 persistable-clustering-0.4.4/persistable/borrowed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      568 2023-03-29 20:24:32.000000 persistable-clustering-0.4.4/persistable/borrowed/_hdbscan_boruvka.pxd
--rw-r--r--   0 runner    (1001) docker     (116)    52745 2023-03-29 20:24:32.000000 persistable-clustering-0.4.4/persistable/borrowed/_hdbscan_boruvka.pyx
--rw-r--r--   0 runner    (1001) docker     (116)     2314 2023-03-29 20:24:32.000000 persistable-clustering-0.4.4/persistable/borrowed/dense_mst.pyx
--rw-r--r--   0 runner    (1001) docker     (116)     2626 2023-03-29 20:24:32.000000 persistable-clustering-0.4.4/persistable/borrowed/dist_metrics.pxd
--rw-r--r--   0 runner    (1001) docker     (116)    41067 2023-03-29 20:24:32.000000 persistable-clustering-0.4.4/persistable/borrowed/dist_metrics.pyx
--rw-r--r--   0 runner    (1001) docker     (116)     5280 2023-03-29 20:24:32.000000 persistable-clustering-0.4.4/persistable/borrowed/prim_mst.pyx
--rw-r--r--   0 runner    (1001) docker     (116)    55336 2023-03-29 20:24:32.000000 persistable-clustering-0.4.4/persistable/persistable.py
--rw-r--r--   0 runner    (1001) docker     (116)   122713 2023-03-29 20:24:32.000000 persistable-clustering-0.4.4/persistable/persistable_interactive.py
--rw-r--r--   0 runner    (1001) docker     (116)     4376 2023-03-29 20:24:32.000000 persistable-clustering-0.4.4/persistable/persistence_diagram_h0.pyx
--rw-r--r--   0 runner    (1001) docker     (116)     1731 2023-03-29 20:24:32.000000 persistable-clustering-0.4.4/persistable/signed_betti_numbers.pyx
--rw-r--r--   0 runner    (1001) docker     (116)     3430 2023-03-29 20:24:32.000000 persistable-clustering-0.4.4/persistable/subsampling.pyx
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-29 20:25:22.804845 persistable-clustering-0.4.4/persistable/test/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-03-29 20:24:32.000000 persistable-clustering-0.4.4/persistable/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    21684 2023-03-29 20:24:32.000000 persistable-clustering-0.4.4/persistable/test/test_persistable.py
--rw-r--r--   0 runner    (1001) docker     (116)     4706 2023-03-29 20:24:32.000000 persistable-clustering-0.4.4/persistable/test/test_ui.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-29 20:25:22.804845 persistable-clustering-0.4.4/persistable_clustering.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     8125 2023-03-29 20:25:22.000000 persistable-clustering-0.4.4/persistable_clustering.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      979 2023-03-29 20:25:22.000000 persistable-clustering-0.4.4/persistable_clustering.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2023-03-29 20:25:22.000000 persistable-clustering-0.4.4/persistable_clustering.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)      141 2023-03-29 20:25:22.000000 persistable-clustering-0.4.4/persistable_clustering.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       12 2023-03-29 20:25:22.000000 persistable-clustering-0.4.4/persistable_clustering.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)       95 2023-03-29 20:24:32.000000 persistable-clustering-0.4.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (116)      142 2023-03-29 20:24:32.000000 persistable-clustering-0.4.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (116)       38 2023-03-29 20:25:22.804845 persistable-clustering-0.4.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     4375 2023-03-29 20:24:32.000000 persistable-clustering-0.4.4/setup.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-02 18:46:30.282355 persistable-clustering-0.4.5/
+-rw-r--r--   0 runner     (501) staff       (20)     3198 2023-07-02 18:45:23.000000 persistable-clustering-0.4.5/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner     (501) staff       (20)     1469 2023-07-02 18:45:23.000000 persistable-clustering-0.4.5/LICENSE
+-rw-r--r--   0 runner     (501) staff       (20)      116 2023-07-02 18:45:23.000000 persistable-clustering-0.4.5/MANIFEST.in
+-rw-r--r--   0 runner     (501) staff       (20)     8352 2023-07-02 18:46:30.281520 persistable-clustering-0.4.5/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)     7413 2023-07-02 18:45:23.000000 persistable-clustering-0.4.5/README.md
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-02 18:46:30.265897 persistable-clustering-0.4.5/persistable/
+-rw-r--r--   0 runner     (501) staff       (20)       97 2023-07-02 18:45:23.000000 persistable-clustering-0.4.5/persistable/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     3411 2023-07-02 18:45:23.000000 persistable-clustering-0.4.5/persistable/_vineyard.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-02 18:46:30.266962 persistable-clustering-0.4.5/persistable/assets/
+-rw-r--r--   0 runner     (501) staff       (20)     4286 2023-07-02 18:45:23.000000 persistable-clustering-0.4.5/persistable/assets/favicon.ico
+-rw-r--r--   0 runner     (501) staff       (20)     3325 2023-07-02 18:45:23.000000 persistable-clustering-0.4.5/persistable/assets/style.css
+-rw-r--r--   0 runner     (501) staff       (20)     1203 2023-07-02 18:45:23.000000 persistable-clustering-0.4.5/persistable/auxiliary.pyx
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-02 18:46:30.274051 persistable-clustering-0.4.5/persistable/borrowed/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-02 18:45:23.000000 persistable-clustering-0.4.5/persistable/borrowed/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      568 2023-07-02 18:45:23.000000 persistable-clustering-0.4.5/persistable/borrowed/_hdbscan_boruvka.pxd
+-rw-r--r--   0 runner     (501) staff       (20)    52745 2023-07-02 18:45:23.000000 persistable-clustering-0.4.5/persistable/borrowed/_hdbscan_boruvka.pyx
+-rw-r--r--   0 runner     (501) staff       (20)     2314 2023-07-02 18:45:23.000000 persistable-clustering-0.4.5/persistable/borrowed/dense_mst.pyx
+-rw-r--r--   0 runner     (501) staff       (20)     2626 2023-07-02 18:45:23.000000 persistable-clustering-0.4.5/persistable/borrowed/dist_metrics.pxd
+-rw-r--r--   0 runner     (501) staff       (20)    41067 2023-07-02 18:45:23.000000 persistable-clustering-0.4.5/persistable/borrowed/dist_metrics.pyx
+-rw-r--r--   0 runner     (501) staff       (20)     5280 2023-07-02 18:45:23.000000 persistable-clustering-0.4.5/persistable/borrowed/prim_mst.pyx
+-rw-r--r--   0 runner     (501) staff       (20)    55743 2023-07-02 18:45:23.000000 persistable-clustering-0.4.5/persistable/persistable.py
+-rw-r--r--   0 runner     (501) staff       (20)   122713 2023-07-02 18:45:23.000000 persistable-clustering-0.4.5/persistable/persistable_interactive.py
+-rw-r--r--   0 runner     (501) staff       (20)     4376 2023-07-02 18:45:23.000000 persistable-clustering-0.4.5/persistable/persistence_diagram_h0.pyx
+-rw-r--r--   0 runner     (501) staff       (20)     1731 2023-07-02 18:45:23.000000 persistable-clustering-0.4.5/persistable/signed_betti_numbers.pyx
+-rw-r--r--   0 runner     (501) staff       (20)     3430 2023-07-02 18:45:23.000000 persistable-clustering-0.4.5/persistable/subsampling.pyx
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-02 18:46:30.277234 persistable-clustering-0.4.5/persistable/test/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-02 18:45:23.000000 persistable-clustering-0.4.5/persistable/test/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)    21684 2023-07-02 18:45:23.000000 persistable-clustering-0.4.5/persistable/test/test_persistable.py
+-rw-r--r--   0 runner     (501) staff       (20)     4706 2023-07-02 18:45:23.000000 persistable-clustering-0.4.5/persistable/test/test_ui.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-02 18:46:30.280880 persistable-clustering-0.4.5/persistable_clustering.egg-info/
+-rw-r--r--   0 runner     (501) staff       (20)     8352 2023-07-02 18:46:30.000000 persistable-clustering-0.4.5/persistable_clustering.egg-info/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)      979 2023-07-02 18:46:30.000000 persistable-clustering-0.4.5/persistable_clustering.egg-info/SOURCES.txt
+-rw-r--r--   0 runner     (501) staff       (20)        1 2023-07-02 18:46:30.000000 persistable-clustering-0.4.5/persistable_clustering.egg-info/dependency_links.txt
+-rw-r--r--   0 runner     (501) staff       (20)      141 2023-07-02 18:46:30.000000 persistable-clustering-0.4.5/persistable_clustering.egg-info/requires.txt
+-rw-r--r--   0 runner     (501) staff       (20)       12 2023-07-02 18:46:30.000000 persistable-clustering-0.4.5/persistable_clustering.egg-info/top_level.txt
+-rw-r--r--   0 runner     (501) staff       (20)       95 2023-07-02 18:45:23.000000 persistable-clustering-0.4.5/pyproject.toml
+-rw-r--r--   0 runner     (501) staff       (20)      142 2023-07-02 18:45:23.000000 persistable-clustering-0.4.5/requirements.txt
+-rw-r--r--   0 runner     (501) staff       (20)       38 2023-07-02 18:46:30.282464 persistable-clustering-0.4.5/setup.cfg
+-rw-r--r--   0 runner     (501) staff       (20)     4375 2023-07-02 18:45:23.000000 persistable-clustering-0.4.5/setup.py
```

### Comparing `persistable-clustering-0.4.4/CODE_OF_CONDUCT.md` & `persistable-clustering-0.4.5/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `persistable-clustering-0.4.4/LICENSE` & `persistable-clustering-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `persistable-clustering-0.4.4/PKG-INFO` & `persistable-clustering-0.4.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: persistable-clustering
-Version: 0.4.4
+Version: 0.4.5
 Summary: Density-based clustering for exploratory data analysis based on multi-parameter persistence
 Home-page: https://github.com/LuisScoccola/persistable
 Maintainer: Luis Scoccola
 Maintainer-email: luis.scoccola@gmail.com
 License: 3-clause BSD
 Keywords: clustering density hierarchical persistence TDA
 Classifier: Development Status :: 4 - Beta
@@ -20,14 +20,15 @@
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 [![PyPI](https://img.shields.io/pypi/v/persistable-clustering?color=green)](https://pypi.org/project/persistable-clustering)
+[![Downloads](https://static.pepy.tech/personalized-badge/persistable-clustering?period=total&units=international_system&left_color=grey&right_color=green&left_text=Downloads)](https://pepy.tech/project/persistable-clustering)
 [![tests](https://github.com/LuisScoccola/persistable/actions/workflows/run_tests.yaml/badge.svg)](https://github.com/LuisScoccola/persistable/actions/workflows/run_tests.yaml)
 [![coverage](https://codecov.io/gh/LuisScoccola/persistable/branch/main/graph/badge.svg)](https://codecov.io/gh/LuisScoccola/persistable)
 [![docs](https://readthedocs.org/projects/persistable/badge/?version=latest)](https://persistable.readthedocs.io/)
 [![status](https://joss.theoj.org/papers/63d612cd4730c3aa708e3a47eb2c50f3/status.svg)](https://joss.theoj.org/papers/63d612cd4730c3aa708e3a47eb2c50f3)
 [![license](https://img.shields.io/github/license/LuisScoccola/persistable)](https://github.com/LuisScoccola/persistable/blob/main/LICENSE)
 ---
```

### Comparing `persistable-clustering-0.4.4/README.md` & `persistable-clustering-0.4.5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 
 [![PyPI](https://img.shields.io/pypi/v/persistable-clustering?color=green)](https://pypi.org/project/persistable-clustering)
+[![Downloads](https://static.pepy.tech/personalized-badge/persistable-clustering?period=total&units=international_system&left_color=grey&right_color=green&left_text=Downloads)](https://pepy.tech/project/persistable-clustering)
 [![tests](https://github.com/LuisScoccola/persistable/actions/workflows/run_tests.yaml/badge.svg)](https://github.com/LuisScoccola/persistable/actions/workflows/run_tests.yaml)
 [![coverage](https://codecov.io/gh/LuisScoccola/persistable/branch/main/graph/badge.svg)](https://codecov.io/gh/LuisScoccola/persistable)
 [![docs](https://readthedocs.org/projects/persistable/badge/?version=latest)](https://persistable.readthedocs.io/)
 [![status](https://joss.theoj.org/papers/63d612cd4730c3aa708e3a47eb2c50f3/status.svg)](https://joss.theoj.org/papers/63d612cd4730c3aa708e3a47eb2c50f3)
 [![license](https://img.shields.io/github/license/LuisScoccola/persistable)](https://github.com/LuisScoccola/persistable/blob/main/LICENSE)
 ---
```

### Comparing `persistable-clustering-0.4.4/persistable/_vineyard.py` & `persistable-clustering-0.4.5/persistable/_vineyard.py`

 * *Files identical despite different names*

### Comparing `persistable-clustering-0.4.4/persistable/assets/favicon.ico` & `persistable-clustering-0.4.5/persistable/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `persistable-clustering-0.4.4/persistable/assets/style.css` & `persistable-clustering-0.4.5/persistable/assets/style.css`

 * *Files identical despite different names*

### Comparing `persistable-clustering-0.4.4/persistable/auxiliary.pyx` & `persistable-clustering-0.4.5/persistable/auxiliary.pyx`

 * *Files identical despite different names*

### Comparing `persistable-clustering-0.4.4/persistable/borrowed/_hdbscan_boruvka.pxd` & `persistable-clustering-0.4.5/persistable/borrowed/_hdbscan_boruvka.pxd`

 * *Files identical despite different names*

### Comparing `persistable-clustering-0.4.4/persistable/borrowed/_hdbscan_boruvka.pyx` & `persistable-clustering-0.4.5/persistable/borrowed/_hdbscan_boruvka.pyx`

 * *Files identical despite different names*

### Comparing `persistable-clustering-0.4.4/persistable/borrowed/dense_mst.pyx` & `persistable-clustering-0.4.5/persistable/borrowed/dense_mst.pyx`

 * *Files identical despite different names*

### Comparing `persistable-clustering-0.4.4/persistable/borrowed/dist_metrics.pxd` & `persistable-clustering-0.4.5/persistable/borrowed/dist_metrics.pxd`

 * *Files identical despite different names*

### Comparing `persistable-clustering-0.4.4/persistable/borrowed/dist_metrics.pyx` & `persistable-clustering-0.4.5/persistable/borrowed/dist_metrics.pyx`

 * *Files identical despite different names*

### Comparing `persistable-clustering-0.4.4/persistable/borrowed/prim_mst.pyx` & `persistable-clustering-0.4.5/persistable/borrowed/prim_mst.pyx`

 * *Files identical despite different names*

### Comparing `persistable-clustering-0.4.4/persistable/persistable.py` & `persistable-clustering-0.4.5/persistable/persistable.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,19 +26,34 @@
     minimum_spanning_tree as sparse_matrix_minimum_spanning_tree,
 )
 from scipy.stats import mode
 from joblib import Parallel, delayed
 from joblib.parallel import cpu_count
 
 
+
+# TODO: eventually default to newer version and add version number in dependencies
+from packaging.version import Version
+import sklearn
+
+if Version(sklearn.__version__) >= Version("1.3.0"):
+    kdtree_valid_metrics = KDTree.valid_metrics()
+    balltree_valid_metrics = BallTree.valid_metrics()
+else:
+    kdtree_valid_metrics = KDTree.valid_metrics
+    balltree_valid_metrics = BallTree.valid_metrics
+#
+
 _TOL = 1e-08
 # starting when we consider a dataset large
 _MANY_POINTS = 40000
 
 
+
+
 def parallel_computation(function, inputs, n_jobs, debug=False, threading=False):
     if n_jobs == 1:
         return [function(inp) for inp in inputs]
     else:
         verbose = 11 if debug else 0
         n_jobs = min(cpu_count(), n_jobs)
         if threading:
@@ -62,15 +77,15 @@
 
     X: ndarray (n_samples, n_features)
         A numpy vector of shape (samples, features) or a distance matrix.
 
     metric: string, optional, default is "minkowski"
         A string determining which metric is used to compute distances
         between the points in X. It can be a metric in ``KDTree.valid_metrics``
-        or ``BallTree.valid_metric`` (which can be found by
+        or ``BallTree.valid_metrics`` (which can be found by
         ``from sklearn.neighbors import KDTree, BallTree``) or ``"precomputed"``
         if X is a distance matrix.
 
     measure: None or ndarray(n_samples), default is None
         A numpy vector of length (samples) of non-negative numbers, which is
         intepreted as a measure on the data points.
         If None, the uniform measure where each point has weight 1/samples is used.
@@ -836,24 +851,24 @@
             self._points = X
         else:
             self._points = np.array(range(self._size))
 
         # save metric and spatial tree
         self._metric = metric
         self._leaf_size = leaf_size
-        if metric in KDTree.valid_metrics + BallTree.valid_metrics:
+        if metric in kdtree_valid_metrics + balltree_valid_metrics:
             leaf_size_boruvka = 3 if self._leaf_size < 3 else self._leaf_size // 3
-            if metric in KDTree.valid_metrics:
+            if metric in kdtree_valid_metrics:
                 self._nn_tree = KDTree(
                     X, metric=metric, leaf_size=self._leaf_size, **kwargs
                 )
                 self._boruvka_tree = KDTree(
                     X, metric=metric, leaf_size=leaf_size_boruvka, **kwargs
                 )
-            elif metric in BallTree.valid_metrics:
+            elif metric in balltree_valid_metrics:
                 self._nn_tree = BallTree(
                     X, metric=metric, leaf_size=self._leaf_size, **kwargs
                 )
                 self._boruvka_tree = BallTree(
                     X, metric=metric, leaf_size=leaf_size_boruvka, **kwargs
                 )
 
@@ -862,15 +877,15 @@
             self._dist_mat = np.array(X)
             self._dist_metric = self._dist_mat
         else:
             raise ValueError("Metric given is not supported.")
 
     def _fit_nn(self, n_neighbors):
         self._n_neighbors = n_neighbors
-        if self._metric in BallTree.valid_metrics + KDTree.valid_metrics:
+        if self._metric in balltree_valid_metrics + kdtree_valid_metrics:
 
             def query_neighbors(points):
                 return self._nn_tree.query(
                     points,
                     self._n_neighbors,
                     return_distance=True,
                     sort_results=True,
@@ -907,38 +922,38 @@
             ].transpose()
         self._fitted_nn = True
 
         self._nn_indices = np.array(neighbors, dtype=np.int_)
         self._nn_distance = np.array(_nn_distance)
 
     ####def distance(self, i,j):
-    ####    if self._metric in KDTree.valid_metrics + BallTree.valid_metrics:
+    ####    if self._metric in kdtree_valid_metrics + balltree_valid_metrics:
     ####        return self._dist_metric.dist(self._points[i], self._points[j], self._dimension)
     ####    else:
     ####        return self._dist_mat[i,j]
 
     def size(self):
         return self._size
 
     def generalized_single_linkage(self, core_distances):
-        if self._metric in KDTree.valid_metrics:
+        if self._metric in kdtree_valid_metrics:
             if self._dimension > self._MAX_DIM_USE_BORUVKA:
                 X = self._points
                 if not X.flags["C_CONTIGUOUS"]:
                     X = np.array(X, dtype=np.double, order="C")
                 sl = mst_linkage_core_vector(X, core_distances, self._dist_metric)
             else:
                 sl = KDTreeBoruvkaAlgorithm(
                     self._boruvka_tree,
                     core_distances,
                     self._nn_indices,
                     metric=self._metric,
                     **self._kwargs
                 ).spanning_tree()
-        elif self._metric in BallTree.valid_metrics:
+        elif self._metric in balltree_valid_metrics:
             if self._dimension > self._MAX_DIM_USE_BORUVKA:
                 X = self._points
                 if not X.flags["C_CONTIGUOUS"]:
                     X = np.array(X, dtype=np.double, order="C")
                 sl = mst_linkage_core_vector(X, core_distances, self._dist_metric)
             else:
                 sl = BallTreeBoruvkaAlgorithm(
@@ -962,15 +977,15 @@
     def hierarchical_clustering_filtered_rips_graph(self, k_births, rips_radius):
         shift = min(k_births) + 1
         # must shift to strictly positive births (sparse matrix mst routine treats
         # edges with zero and very small weight as not there (i.e., as having infinite weight))
         k_births = k_births + shift
 
         # metric tree case
-        if self._metric in KDTree.valid_metrics + BallTree.valid_metrics:
+        if self._metric in kdtree_valid_metrics + balltree_valid_metrics:
             s_neighbors = self._nn_tree.query_radius(self._points, rips_radius)
         # dense distance matrix case
         elif self._metric == "precomputed":
             s_neighbors = []
             for i in range(self.size()):
                 s_neighbors.append(np.argwhere(self._dist_mat[i] <= rips_radius)[:, 0])
         else:
@@ -1020,15 +1035,15 @@
 
         if euclidean:
             return self._close_subsample_euclidean(subsample_size)
 
         np.random.seed(seed)
         random_start = np.random.randint(0, self.size())
 
-        if self._metric in KDTree.valid_metrics + BallTree.valid_metrics:
+        if self._metric in kdtree_valid_metrics + balltree_valid_metrics:
             X = self._points
             if not X.flags["C_CONTIGUOUS"]:
                 X = np.array(X, dtype=np.double, order="C")
             return close_subsample_fast_metric(
                 subsample_size, X, self._dist_metric, random_start=random_start
             )
         elif self._metric == "precomputed":
```

### Comparing `persistable-clustering-0.4.4/persistable/persistable_interactive.py` & `persistable-clustering-0.4.5/persistable/persistable_interactive.py`

 * *Files identical despite different names*

### Comparing `persistable-clustering-0.4.4/persistable/persistence_diagram_h0.pyx` & `persistable-clustering-0.4.5/persistable/persistence_diagram_h0.pyx`

 * *Files identical despite different names*

### Comparing `persistable-clustering-0.4.4/persistable/signed_betti_numbers.pyx` & `persistable-clustering-0.4.5/persistable/signed_betti_numbers.pyx`

 * *Files identical despite different names*

### Comparing `persistable-clustering-0.4.4/persistable/subsampling.pyx` & `persistable-clustering-0.4.5/persistable/subsampling.pyx`

 * *Files identical despite different names*

### Comparing `persistable-clustering-0.4.4/persistable/test/test_persistable.py` & `persistable-clustering-0.4.5/persistable/test/test_persistable.py`

 * *Files identical despite different names*

### Comparing `persistable-clustering-0.4.4/persistable/test/test_ui.py` & `persistable-clustering-0.4.5/persistable/test/test_ui.py`

 * *Files identical despite different names*

### Comparing `persistable-clustering-0.4.4/persistable_clustering.egg-info/PKG-INFO` & `persistable-clustering-0.4.5/persistable_clustering.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: persistable-clustering
-Version: 0.4.4
+Version: 0.4.5
 Summary: Density-based clustering for exploratory data analysis based on multi-parameter persistence
 Home-page: https://github.com/LuisScoccola/persistable
 Maintainer: Luis Scoccola
 Maintainer-email: luis.scoccola@gmail.com
 License: 3-clause BSD
 Keywords: clustering density hierarchical persistence TDA
 Classifier: Development Status :: 4 - Beta
@@ -20,14 +20,15 @@
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 [![PyPI](https://img.shields.io/pypi/v/persistable-clustering?color=green)](https://pypi.org/project/persistable-clustering)
+[![Downloads](https://static.pepy.tech/personalized-badge/persistable-clustering?period=total&units=international_system&left_color=grey&right_color=green&left_text=Downloads)](https://pepy.tech/project/persistable-clustering)
 [![tests](https://github.com/LuisScoccola/persistable/actions/workflows/run_tests.yaml/badge.svg)](https://github.com/LuisScoccola/persistable/actions/workflows/run_tests.yaml)
 [![coverage](https://codecov.io/gh/LuisScoccola/persistable/branch/main/graph/badge.svg)](https://codecov.io/gh/LuisScoccola/persistable)
 [![docs](https://readthedocs.org/projects/persistable/badge/?version=latest)](https://persistable.readthedocs.io/)
 [![status](https://joss.theoj.org/papers/63d612cd4730c3aa708e3a47eb2c50f3/status.svg)](https://joss.theoj.org/papers/63d612cd4730c3aa708e3a47eb2c50f3)
 [![license](https://img.shields.io/github/license/LuisScoccola/persistable)](https://github.com/LuisScoccola/persistable/blob/main/LICENSE)
 ---
```

### Comparing `persistable-clustering-0.4.4/persistable_clustering.egg-info/SOURCES.txt` & `persistable-clustering-0.4.5/persistable_clustering.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `persistable-clustering-0.4.4/setup.py` & `persistable-clustering-0.4.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -101,15 +101,15 @@
 
 def readme():
     with open("README.md") as readme_file:
         return readme_file.read()
 
 setup(
     name="persistable-clustering",
-    version="0.4.4",
+    version="0.4.5",
     description="Density-based clustering for exploratory data analysis based on multi-parameter persistence",
     long_description=readme(),
     long_description_content_type="text/markdown",
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Science/Research",
         "Intended Audience :: Developers",
```

