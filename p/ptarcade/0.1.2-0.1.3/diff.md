# Comparing `tmp/ptarcade-0.1.2.tar.gz` & `tmp/ptarcade-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ptarcade-0.1.2.tar", max compression
+gzip compressed data, was "ptarcade-0.1.3.tar", max compression
```

## Comparing `ptarcade-0.1.2.tar` & `ptarcade-0.1.3.tar`

### file list

```diff
@@ -1,15 +1,16 @@
--rw-r--r--   0        0        0      673 2023-06-29 23:09:28.232412 ptarcade-0.1.2/README.md
--rw-r--r--   0        0        0     3313 2023-06-30 21:13:19.488677 ptarcade-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      555 2023-06-29 05:37:13.771628 ptarcade-0.1.2/src/ptarcade/__init__.py
--rw-r--r--   0        0        0    32466 2023-06-29 05:37:13.771628 ptarcade-0.1.2/src/ptarcade/chains_utils.py
--rw-r--r--   0        0        0       23 2023-06-29 05:37:13.771628 ptarcade-0.1.2/src/ptarcade/data/__init__.py
--rw-r--r--   0        0        0     1026 2023-06-30 21:13:04.270655 ptarcade-0.1.2/src/ptarcade/data/default_config.py
--rw-r--r--   0        0        0    29964 2023-06-29 05:37:13.771628 ptarcade-0.1.2/src/ptarcade/data/g_star.dat
--rw-r--r--   0        0        0     4182 2023-06-29 05:37:13.771628 ptarcade-0.1.2/src/ptarcade/fast_interpolate.py
--rw-r--r--   0        0        0    15036 2023-06-29 05:37:13.771628 ptarcade-0.1.2/src/ptarcade/input_handler.py
--rw-r--r--   0        0        0    17354 2023-06-29 05:37:13.771628 ptarcade-0.1.2/src/ptarcade/models_utils.py
--rw-r--r--   0        0        0    30151 2023-06-29 05:37:13.771628 ptarcade-0.1.2/src/ptarcade/plot_utils.py
--rw-r--r--   0        0        0     6885 2023-06-30 21:13:19.488677 ptarcade-0.1.2/src/ptarcade/pta_importer.py
--rw-r--r--   0        0        0    11573 2023-06-29 23:54:58.423893 ptarcade-0.1.2/src/ptarcade/sampler.py
--rw-r--r--   0        0        0    18088 2023-06-30 21:26:10.379417 ptarcade-0.1.2/src/ptarcade/signal_builder.py
--rw-r--r--   0        0        0     2645 1970-01-01 00:00:00.000000 ptarcade-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-06-30 22:17:44.000000 ptarcade-0.1.3/LICENSE
+-rw-r--r--   0        0        0      673 2023-06-29 23:09:28.232412 ptarcade-0.1.3/README.md
+-rw-r--r--   0        0        0     3313 2023-07-02 17:53:09.136777 ptarcade-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      555 2023-07-02 01:53:08.893492 ptarcade-0.1.3/src/ptarcade/__init__.py
+-rw-r--r--   0        0        0    32466 2023-06-29 05:37:13.771628 ptarcade-0.1.3/src/ptarcade/chains_utils.py
+-rw-r--r--   0        0        0       23 2023-06-29 05:37:13.771628 ptarcade-0.1.3/src/ptarcade/data/__init__.py
+-rw-r--r--   0        0        0     1026 2023-06-30 21:13:04.270655 ptarcade-0.1.3/src/ptarcade/data/default_config.py
+-rw-r--r--   0        0        0    29964 2023-06-29 05:37:13.771628 ptarcade-0.1.3/src/ptarcade/data/g_star.dat
+-rw-r--r--   0        0        0     4994 2023-07-02 16:09:59.530041 ptarcade-0.1.3/src/ptarcade/fast_interpolate.py
+-rw-r--r--   0        0        0    15036 2023-07-02 03:08:58.531872 ptarcade-0.1.3/src/ptarcade/input_handler.py
+-rw-r--r--   0        0        0    17354 2023-06-29 05:37:13.771628 ptarcade-0.1.3/src/ptarcade/models_utils.py
+-rw-r--r--   0        0        0    30151 2023-06-29 05:37:13.771628 ptarcade-0.1.3/src/ptarcade/plot_utils.py
+-rw-r--r--   0        0        0     6885 2023-06-30 21:13:19.488677 ptarcade-0.1.3/src/ptarcade/pta_importer.py
+-rw-r--r--   0        0        0    11542 2023-07-02 16:09:59.530041 ptarcade-0.1.3/src/ptarcade/sampler.py
+-rw-r--r--   0        0        0    18088 2023-06-30 21:26:10.379417 ptarcade-0.1.3/src/ptarcade/signal_builder.py
+-rw-r--r--   0        0        0     2645 1970-01-01 00:00:00.000000 ptarcade-0.1.3/PKG-INFO
```

### Comparing `ptarcade-0.1.2/README.md` & `ptarcade-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `ptarcade-0.1.2/pyproject.toml` & `ptarcade-0.1.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -96,15 +96,15 @@
   "doc/build/*.py",
   "doc/temp/*.py",
   ".eggs/*.py",
 ]
 
 [tool.poetry]
 name = "PTArcade"
-version = "0.1.2"
+version = "0.1.3"
 description = "PTArcade provides an interface to the ENTERPRISE analysis suite and allows for simple implementation of new-physics searches in PTA data."
 readme = "README.md"
 authors = ["Andrea Mitridate <andrea.mitridate@nanograv.org>",]
 keywords = ["ptarcade"]
 repository = "https://github.com/andrea-mitridate/PTArcade"
 documentation = "https://andrea-mitridate.github.io/PTArcade/"
 classifiers = [
```

### Comparing `ptarcade-0.1.2/src/ptarcade/__init__.py` & `ptarcade-0.1.3/src/ptarcade/__init__.py`

 * *Files identical despite different names*

### Comparing `ptarcade-0.1.2/src/ptarcade/chains_utils.py` & `ptarcade-0.1.3/src/ptarcade/chains_utils.py`

 * *Files identical despite different names*

### Comparing `ptarcade-0.1.2/src/ptarcade/data/default_config.py` & `ptarcade-0.1.3/src/ptarcade/data/default_config.py`

 * *Files identical despite different names*

### Comparing `ptarcade-0.1.2/src/ptarcade/data/g_star.dat` & `ptarcade-0.1.3/src/ptarcade/data/g_star.dat`

 * *Files identical despite different names*

### Comparing `ptarcade-0.1.2/src/ptarcade/fast_interpolate.py` & `ptarcade-0.1.3/src/ptarcade/fast_interpolate.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Utilities for fast interpolation of spectra."""
 from __future__ import annotations
 
 import h5py
 import numpy as np
+from numpy._typing import _ArrayLikeFloat_co as array_like
 from numpy.typing import NDArray
 
 
 def load_data(file: str) -> tuple[list[tuple[str, float, float]], NDArray]:
     """Load HDF5 file.
 
     Read data from an HDF5 file and use it for interpolation of the spectrum.
@@ -31,15 +32,15 @@
     """
     with h5py.File(file) as h5:
         info = [(par, h5[par][0], h5[par][1]) for par in h5['parameter_names'].asstr()]
         spectrum = np.array(h5['spectrum'])
         return (info, spectrum)
 
 
-def interp(info: list[tuple[float, float, float]], data: NDArray) -> NDArray:
+def interp(info: list[tuple[float, float, array_like]], data: NDArray) -> NDArray:
     """Do interpolation.
 
     Called with info: list of (start, step, value) and multidimensional array of data points. Multiple values
     (in an np.array) are OK for the last value, but not earlier ones or else we will get confusion about
     array indexes.
 
     Parameters
@@ -55,15 +56,28 @@
     NDArray
         Interpolated values
 
     """
     if len(info) == 0:       # Nothing to do: just return element
         return data
     x0, dx, x = info[0]
-    (fract, index) = np.modf((x - x0) / dx)
+    # This function exploits single integer vs array of integer indexing.
+    # Ceffyl returns an array, even if it only contains a single element.
+    # Enterprise doesn't experience this issue.
+    # The type of `x` below can change the type of `index` s.t. it breaks
+    # this function (i.e. `index` will become [3] instead of just 3).
+    # So, here we cast all single element arrays `x` to their
+    # scalar representations.
+    # We use getattr as a quick test for the type (if it's not an
+    # array it won't have the attribute) and to get the shape
+    # if it is an array.
+    # There is probably a much more intelligent way to solve this issue
+    if getattr(x, "shape", None)==(1,):
+        x = x.item() # type: ignore
+    (fract, index) = np.modf((x - x0) / dx) # type: ignore
     index = index.astype(int)
     # Call ourselves to interpolate over remaining variables if any
     # then combine results linearly
     return (interp(info[1:], data[index]) * (1-fract)
             + interp(info[1:], data[index+1]) * fract)
```

### Comparing `ptarcade-0.1.2/src/ptarcade/input_handler.py` & `ptarcade-0.1.3/src/ptarcade/input_handler.py`

 * *Files identical despite different names*

### Comparing `ptarcade-0.1.2/src/ptarcade/models_utils.py` & `ptarcade-0.1.3/src/ptarcade/models_utils.py`

 * *Files identical despite different names*

### Comparing `ptarcade-0.1.2/src/ptarcade/plot_utils.py` & `ptarcade-0.1.3/src/ptarcade/plot_utils.py`

 * *Files identical despite different names*

### Comparing `ptarcade-0.1.2/src/ptarcade/pta_importer.py` & `ptarcade-0.1.3/src/ptarcade/pta_importer.py`

 * *Files identical despite different names*

### Comparing `ptarcade-0.1.2/src/ptarcade/sampler.py` & `ptarcade-0.1.3/src/ptarcade/sampler.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,16 +108,14 @@
     emp_dist : array_like | None
         The empirical distribution to use for sampling
 
     """
     # import pta data
     psrs, noise_params, emp_dist = pta_importer.pta_data_importer(inputs['config'].pta_data)
 
-    print(f"\tloaded {len(psrs)} pulsars\n")
-    
     return psrs, noise_params, emp_dist
 
 
 def initialize_pta(inputs: dict[str, Any], psrs: list[Pulsar] | None, noise_params : dict | None ) -> dict[int, PTA]:
     """Initialize the PTA with the user input
 
     Parameters
@@ -331,15 +329,15 @@
 
     if inputs["config"].mode == "enterprise":
         with console.status("Loading Pulsars and noise data...", spinner="bouncingBall"):
 
             # import pta data
             psrs, noise_params, emp_dist = get_user_pta_data(inputs)
 
-            console.rule("[bold green]Done loading Pulsars and noise data :heavy_check_mark-emoji:")
+            console.print(f"[bold green]Done loading [blue]{len(psrs)}[/] Pulsars and noise data :heavy_check_mark:\n")
 
 
     with console.status("Initializing PTA...", spinner="bouncingBall"):
         pta = initialize_pta(inputs, psrs, noise_params)
         console.print("[bold green]Done initializing PTA :heavy_check_mark:\n")
```

### Comparing `ptarcade-0.1.2/src/ptarcade/signal_builder.py` & `ptarcade-0.1.3/src/ptarcade/signal_builder.py`

 * *Files identical despite different names*

### Comparing `ptarcade-0.1.2/PKG-INFO` & `ptarcade-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ptarcade
-Version: 0.1.2
+Version: 0.1.3
 Summary: PTArcade provides an interface to the ENTERPRISE analysis suite and allows for simple implementation of new-physics searches in PTA data.
 Home-page: https://github.com/andrea-mitridate/PTArcade
 Keywords: ptarcade
 Author: Andrea Mitridate
 Author-email: andrea.mitridate@nanograv.org
 Requires-Python: >=3.9,<3.11
 Classifier: Intended Audience :: Developers
```

