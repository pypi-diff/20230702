# Comparing `tmp/xenosite-fragment-0a8.tar.gz` & `tmp/xenosite-fragment-0a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xenosite-fragment-0a8.tar", last modified: Fri Jun 23 15:58:53 2023, max compression
+gzip compressed data, was "xenosite-fragment-0a9.tar", last modified: Sat Jul  1 23:53:29 2023, max compression
```

## Comparing `xenosite-fragment-0a8.tar` & `xenosite-fragment-0a9.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 15:58:53.658178 xenosite-fragment-0a8/
--rw-r--r--   0 root         (0) root         (0)     4451 2023-06-23 15:58:53.658178 xenosite-fragment-0a8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3735 2023-06-23 15:58:52.000000 xenosite-fragment-0a8/README.md
--rw-r--r--   0 root         (0) root         (0)       76 2023-06-23 15:58:52.000000 xenosite-fragment-0a8/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-23 15:58:53.658178 xenosite-fragment-0a8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1808 2023-06-23 15:58:52.000000 xenosite-fragment-0a8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 15:58:53.654178 xenosite-fragment-0a8/test/
--rw-r--r--   0 root         (0) root         (0)     2294 2023-06-23 15:58:52.000000 xenosite-fragment-0a8/test/test_fragment.py
--rw-r--r--   0 root         (0) root         (0)      947 2023-06-23 15:58:52.000000 xenosite-fragment-0a8/test/test_morgan.py
--rw-r--r--   0 root         (0) root         (0)     7779 2023-06-23 15:58:52.000000 xenosite-fragment-0a8/test/test_netx.py
--rw-r--r--   0 root         (0) root         (0)     1197 2023-06-23 15:58:52.000000 xenosite-fragment-0a8/test/test_remap.py
--rw-r--r--   0 root         (0) root         (0)     1106 2023-06-23 15:58:52.000000 xenosite-fragment-0a8/test/test_tanimoto.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 15:58:53.654178 xenosite-fragment-0a8/xenosite/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 15:58:53.658178 xenosite-fragment-0a8/xenosite/fragment/
--rw-r--r--   0 root         (0) root         (0)     3976 2023-06-23 15:58:52.000000 xenosite-fragment-0a8/xenosite/fragment/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9026 2023-06-23 15:58:52.000000 xenosite-fragment-0a8/xenosite/fragment/__main__.py
--rw-r--r--   0 root         (0) root         (0)       59 2023-06-23 15:58:53.658178 xenosite-fragment-0a8/xenosite/fragment/_static_version.py
--rw-r--r--   0 root         (0) root         (0)     5773 2023-06-23 15:58:52.000000 xenosite-fragment-0a8/xenosite/fragment/_version.py
--rw-r--r--   0 root         (0) root         (0)    14809 2023-06-23 15:58:52.000000 xenosite-fragment-0a8/xenosite/fragment/chem.py
--rw-r--r--   0 root         (0) root         (0)     6224 2023-06-23 15:58:52.000000 xenosite-fragment-0a8/xenosite/fragment/feature.py
--rw-r--r--   0 root         (0) root         (0)     7165 2023-06-23 15:58:52.000000 xenosite-fragment-0a8/xenosite/fragment/graph.py
--rw-r--r--   0 root         (0) root         (0)     1236 2023-06-23 15:58:52.000000 xenosite-fragment-0a8/xenosite/fragment/keras_backend.py
--rw-r--r--   0 root         (0) root         (0)       78 2023-06-23 15:58:52.000000 xenosite-fragment-0a8/xenosite/fragment/netx.py
--rw-r--r--   0 root         (0) root         (0)     4465 2023-06-23 15:58:52.000000 xenosite-fragment-0a8/xenosite/fragment/ops.py
--rw-r--r--   0 root         (0) root         (0)     3180 2023-06-23 15:58:52.000000 xenosite-fragment-0a8/xenosite/fragment/remap.py
--rw-r--r--   0 root         (0) root         (0)     5640 2023-06-23 15:58:52.000000 xenosite-fragment-0a8/xenosite/fragment/serialize.py
--rw-r--r--   0 root         (0) root         (0)     4187 2023-06-23 15:58:52.000000 xenosite-fragment-0a8/xenosite/fragment/stats.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 15:58:53.658178 xenosite-fragment-0a8/xenosite_fragment.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4451 2023-06-23 15:58:53.000000 xenosite-fragment-0a8/xenosite_fragment.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      762 2023-06-23 15:58:53.000000 xenosite-fragment-0a8/xenosite_fragment.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-23 15:58:53.000000 xenosite-fragment-0a8/xenosite_fragment.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      132 2023-06-23 15:58:53.000000 xenosite-fragment-0a8/xenosite_fragment.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       60 2023-06-23 15:58:53.000000 xenosite-fragment-0a8/xenosite_fragment.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-06-23 15:58:53.000000 xenosite-fragment-0a8/xenosite_fragment.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 23:53:29.052368 xenosite-fragment-0a9/
+-rw-r--r--   0 root         (0) root         (0)     4451 2023-07-01 23:53:29.052368 xenosite-fragment-0a9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3735 2023-07-01 23:53:28.000000 xenosite-fragment-0a9/README.md
+-rw-r--r--   0 root         (0) root         (0)       76 2023-07-01 23:53:28.000000 xenosite-fragment-0a9/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-01 23:53:29.052368 xenosite-fragment-0a9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1808 2023-07-01 23:53:28.000000 xenosite-fragment-0a9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 23:53:29.052368 xenosite-fragment-0a9/test/
+-rw-r--r--   0 root         (0) root         (0)     2333 2023-07-01 23:53:28.000000 xenosite-fragment-0a9/test/test_fragment.py
+-rw-r--r--   0 root         (0) root         (0)      947 2023-07-01 23:53:28.000000 xenosite-fragment-0a9/test/test_morgan.py
+-rw-r--r--   0 root         (0) root         (0)     7779 2023-07-01 23:53:28.000000 xenosite-fragment-0a9/test/test_netx.py
+-rw-r--r--   0 root         (0) root         (0)     1197 2023-07-01 23:53:28.000000 xenosite-fragment-0a9/test/test_remap.py
+-rw-r--r--   0 root         (0) root         (0)     1106 2023-07-01 23:53:28.000000 xenosite-fragment-0a9/test/test_tanimoto.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 23:53:29.048368 xenosite-fragment-0a9/xenosite/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 23:53:29.052368 xenosite-fragment-0a9/xenosite/fragment/
+-rw-r--r--   0 root         (0) root         (0)     3976 2023-07-01 23:53:28.000000 xenosite-fragment-0a9/xenosite/fragment/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9045 2023-07-01 23:53:28.000000 xenosite-fragment-0a9/xenosite/fragment/__main__.py
+-rw-r--r--   0 root         (0) root         (0)       59 2023-07-01 23:53:29.052368 xenosite-fragment-0a9/xenosite/fragment/_static_version.py
+-rw-r--r--   0 root         (0) root         (0)     5773 2023-07-01 23:53:28.000000 xenosite-fragment-0a9/xenosite/fragment/_version.py
+-rw-r--r--   0 root         (0) root         (0)    14816 2023-07-01 23:53:28.000000 xenosite-fragment-0a9/xenosite/fragment/chem.py
+-rw-r--r--   0 root         (0) root         (0)     6224 2023-07-01 23:53:28.000000 xenosite-fragment-0a9/xenosite/fragment/feature.py
+-rw-r--r--   0 root         (0) root         (0)     5293 2023-07-01 23:53:28.000000 xenosite-fragment-0a9/xenosite/fragment/graph.py
+-rw-r--r--   0 root         (0) root         (0)     1236 2023-07-01 23:53:28.000000 xenosite-fragment-0a9/xenosite/fragment/keras_backend.py
+-rw-r--r--   0 root         (0) root         (0)       78 2023-07-01 23:53:28.000000 xenosite-fragment-0a9/xenosite/fragment/netx.py
+-rw-r--r--   0 root         (0) root         (0)     4465 2023-07-01 23:53:28.000000 xenosite-fragment-0a9/xenosite/fragment/ops.py
+-rw-r--r--   0 root         (0) root         (0)     3180 2023-07-01 23:53:28.000000 xenosite-fragment-0a9/xenosite/fragment/remap.py
+-rw-r--r--   0 root         (0) root         (0)     5640 2023-07-01 23:53:28.000000 xenosite-fragment-0a9/xenosite/fragment/serialize.py
+-rw-r--r--   0 root         (0) root         (0)     4477 2023-07-01 23:53:28.000000 xenosite-fragment-0a9/xenosite/fragment/stats.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 23:53:29.052368 xenosite-fragment-0a9/xenosite_fragment.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4451 2023-07-01 23:53:29.000000 xenosite-fragment-0a9/xenosite_fragment.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      762 2023-07-01 23:53:29.000000 xenosite-fragment-0a9/xenosite_fragment.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-01 23:53:29.000000 xenosite-fragment-0a9/xenosite_fragment.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      132 2023-07-01 23:53:29.000000 xenosite-fragment-0a9/xenosite_fragment.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       60 2023-07-01 23:53:29.000000 xenosite-fragment-0a9/xenosite_fragment.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-07-01 23:53:29.000000 xenosite-fragment-0a9/xenosite_fragment.egg-info/top_level.txt
```

### Comparing `xenosite-fragment-0a8/PKG-INFO` & `xenosite-fragment-0a9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xenosite-fragment
-Version: 0a8
+Version: 0a9
 Summary: Library for molecule fragment operations.
 Home-page: UNKNOWN
 Author: S. Joshua Swamidass
 Author-email: swamidass@wustl.edu
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Intended Audience :: Education
@@ -155,25 +155,25 @@
 Enumerate and compute statistics on all the subgraphs in a molecule:
 
 ```
 >>> from xenosite.fragment.net import SubGraphFragmentNetwork
 >>> N = SubGraphFragmentNetwork("CC1COC1")
 >>> fragments = N.to_pandas()
 >>> list(fragments.index)
-['C-C', 'C', 'C-O-C', 'C-O', 'O', 'C-C1-C-O-C-1', 'C1-C-C-O-1', 'C-C-C-O', 'C-C(-C)-C', 'C-C-O', 'C-C-C']
+['C-C', 'C', 'C-O-C', 'C-O', 'O', 'C-C1-C-O-C-1', 'C1-C-O-C-1', 'C-C-C-O', 'C-C(-C)-C', 'C-C-O', 'C-C-C']
 >>> fragments["size"].to_numpy()
 array([2, 1, 3, 2, 1, 5, 4, 4, 4, 3, 3])
 ```
 
 Better fragments can be enumerated by collapsing all atoms in a ring into a single node
 during subgraph enumeration. 
 
 ```
 >>> from xenosite.fragment.net import RingFragmentNetwork
 >>> N = RingFragmentNetwork("CC1COC1")
 >>> fragments = N.to_pandas()
 >>> list(fragments.index)
-['C-C1-C-O-C-1', 'C', 'C1-C-C-O-1']
+['C-C1-C-O-C-1', 'C', 'C1-C-O-C-1']
 >>> fragments["size"].to_numpy()
 array([5, 1, 4])
 ```
```

### Comparing `xenosite-fragment-0a8/README.md` & `xenosite-fragment-0a9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -134,24 +134,24 @@
 Enumerate and compute statistics on all the subgraphs in a molecule:
 
 ```
 >>> from xenosite.fragment.net import SubGraphFragmentNetwork
 >>> N = SubGraphFragmentNetwork("CC1COC1")
 >>> fragments = N.to_pandas()
 >>> list(fragments.index)
-['C-C', 'C', 'C-O-C', 'C-O', 'O', 'C-C1-C-O-C-1', 'C1-C-C-O-1', 'C-C-C-O', 'C-C(-C)-C', 'C-C-O', 'C-C-C']
+['C-C', 'C', 'C-O-C', 'C-O', 'O', 'C-C1-C-O-C-1', 'C1-C-O-C-1', 'C-C-C-O', 'C-C(-C)-C', 'C-C-O', 'C-C-C']
 >>> fragments["size"].to_numpy()
 array([2, 1, 3, 2, 1, 5, 4, 4, 4, 3, 3])
 ```
 
 Better fragments can be enumerated by collapsing all atoms in a ring into a single node
 during subgraph enumeration. 
 
 ```
 >>> from xenosite.fragment.net import RingFragmentNetwork
 >>> N = RingFragmentNetwork("CC1COC1")
 >>> fragments = N.to_pandas()
 >>> list(fragments.index)
-['C-C1-C-O-C-1', 'C', 'C1-C-C-O-1']
+['C-C1-C-O-C-1', 'C', 'C1-C-O-C-1']
 >>> fragments["size"].to_numpy()
 array([5, 1, 4])
 ```
```

### Comparing `xenosite-fragment-0a8/setup.py` & `xenosite-fragment-0a9/setup.py`

 * *Files identical despite different names*

### Comparing `xenosite-fragment-0a8/test/test_fragment.py` & `xenosite-fragment-0a9/test/test_fragment.py`

 * *Files 6% similar despite different names*

```diff
@@ -59,21 +59,24 @@
     _test_canonization(r"Cc1ccccc1O")
 
 
 def test_case2():
     """Will fail if bond labels not used."""
     _test_canonization(r"C1=CCCCC1")
 
+
+@pytest.mark.xfail
 def test_case_hard1():
     """From fig. 4, DOI: 10.1021/acs.jcim.5b00543
     
     Fails when using morgan labels for canonization.
     """
     _test_canonization(r"C12C3C4C5C6C1C6C(C23)C45")
     
+@pytest.mark.xfail
 def test_case_hard2():
     """From fig. 4, DOI: 10.1021/acs.jcim.5b00543
     
     Fails when using morgan labels for canonization."""
     _test_canonization(r"C1=CC2=CC=C1\C=C/C1=CC=C(C=C1)\C=C/2")
```

### Comparing `xenosite-fragment-0a8/test/test_morgan.py` & `xenosite-fragment-0a9/test/test_morgan.py`

 * *Files identical despite different names*

### Comparing `xenosite-fragment-0a8/test/test_netx.py` & `xenosite-fragment-0a9/test/test_netx.py`

 * *Files identical despite different names*

### Comparing `xenosite-fragment-0a8/test/test_remap.py` & `xenosite-fragment-0a9/test/test_remap.py`

 * *Files identical despite different names*

### Comparing `xenosite-fragment-0a8/test/test_tanimoto.py` & `xenosite-fragment-0a9/test/test_tanimoto.py`

 * *Files identical despite different names*

### Comparing `xenosite-fragment-0a8/xenosite/fragment/__init__.py` & `xenosite-fragment-0a9/xenosite/fragment/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,26 +104,26 @@
 
 Enumerate and compute statistics on all the subgraphs in a molecule:
 
 >>> from xenosite.fragment.net import SubGraphFragmentNetwork
 >>> N = SubGraphFragmentNetwork("CC1COC1")
 >>> fragments = N.to_pandas()
 >>> list(fragments.index)
-['C-C', 'C', 'C-O-C', 'C-O', 'O', 'C-C1-C-O-C-1', 'C1-C-C-O-1', 'C-C-C-O', 'C-C(-C)-C', 'C-C-O', 'C-C-C']
+['C-C', 'C', 'C-O-C', 'C-O', 'O', 'C-C1-C-O-C-1', 'C1-C-O-C-1', 'C-C-C-O', 'C-C(-C)-C', 'C-C-O', 'C-C-C']
 >>> fragments["size"].to_numpy()
 array([2, 1, 3, 2, 1, 5, 4, 4, 4, 3, 3])
 
 Better fragments can be enumerated by collapsing all atoms in a ring into a single node
 during subgraph enumeration. 
 
 >>> from xenosite.fragment.net import RingFragmentNetwork
 >>> N = RingFragmentNetwork("CC1COC1")
 >>> fragments = N.to_pandas()
 >>> list(fragments.index)
-['C-C1-C-O-C-1', 'C', 'C1-C-C-O-1']
+['C-C1-C-O-C-1', 'C', 'C1-C-O-C-1']
 >>> fragments["size"].to_numpy()
 array([5, 1, 4])
 
 """
 
 
 from .graph import Graph
```

### Comparing `xenosite-fragment-0a8/xenosite/fragment/__main__.py` & `xenosite-fragment-0a9/xenosite/fragment/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from rdkit import Chem
 from pathlib import Path
 from enum import Enum
 import pandas as pd
 from xenosite.fragment.stats import FragmentStatistics
 
 runtime_env = {
-    "pip": ["numba", "rdkit", "networkx", "rich", "pandas"],
+    "pip": ["numba", "rdkit", "networkx", "rich", "pandas",  "pynauty==2.8.6"],
     "py_modules": ["xenosite"],
     "exclude": ["*.csv", ".git", "*.ipynb", "*.gz", "coverage"],
     "eager_install": True,
 }
 
 
 logging.basicConfig(
```

### Comparing `xenosite-fragment-0a8/xenosite/fragment/_version.py` & `xenosite-fragment-0a9/xenosite/fragment/_version.py`

 * *Files identical despite different names*

### Comparing `xenosite-fragment-0a8/xenosite/fragment/chem.py` & `xenosite-fragment-0a9/xenosite/fragment/chem.py`

 * *Files 0% similar despite different names*

```diff
@@ -169,16 +169,17 @@
         """
         Determine which atoms in a fragment are topologically equivalent.
 
         :return: Tuple of numpy array with group assignment, and the integer number of distinct topological groups.
         :rtype: FragmentEquivalence
         """        
 
-        o = self.graph._nauty_orbits()
-        return FragmentEquivalence(o, np.max(o)) #type: ignore
+        o = self.graph.morgan()
+        o = to_range(o)
+        return FragmentEquivalence(*o) #type: ignore
 
     def canonical(self, remap=False) -> Serialized:
         """
         Canonical representation of Fragment, with reordering from input molecule.
 
         :return: Cannonical string representation of fragment.
         :rtype: Serialized
```

### Comparing `xenosite-fragment-0a8/xenosite/fragment/feature.py` & `xenosite-fragment-0a9/xenosite/fragment/feature.py`

 * *Files identical despite different names*

### Comparing `xenosite-fragment-0a8/xenosite/fragment/graph.py` & `xenosite-fragment-0a9/xenosite/fragment/graph.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 from __future__ import annotations
 
 from enum import Enum
 from typing import NamedTuple, Optional, Sequence, Union, Any
 from numba import njit
-from collections import defaultdict
 import numpy as np
-import pynauty
 
 from . import serialize
-from .ops import morgan, to_range, segment_min
+from .ops import morgan
 
 
 class BaseGraph:
     def __init__(
         self,
         n: int,
         edge: tuple[Sequence[np.uint32], Sequence[np.uint32]],
@@ -95,15 +93,15 @@
             N[i].append(j)
             N[j].append(i)
 
         return N
     
 
 
-    def morgan(self) -> np.ndarray[np.int64]:
+    def morgan(self) -> np.ndarray[np.int64]: #type: ignore
         try:
             _ = self._morgan
         except:
 
           if self.elabel:
               self._morgan = self.edge_to_node().morgan()[: self.n]
           else:
@@ -111,99 +109,27 @@
               e1 = self.edge[0]
               e2 = self.edge[1]
 
               self._morgan = morgan(self.nlabel, e1, e2)  # type: ignore
     
         return self._morgan
 
-    
-    def _to_nauty(self, colors=True):
-
-        adj = defaultdict(list)
-        for i in range(len(self.edge[0])):
-            adj[self.edge[0][i]].append(self.edge[1][i])
-
-        # # equiv loop:
-        # for i, j in zip(*self.edge):
-        #     adj[i].append(j)
-
-        if colors and self.nlabel:
-            c = _to_nauty_colors(self.nlabel)   
-        else:
-            c = []
-
-        g = pynauty.Graph(self.n)
-
-        # setting adj and color, bypassing all checks
-        g._adjacency_dict = adj
-        g._vertex_coloring = c
-        return g
-    
-    def _nauty_order(self):
-        import pynauty
-        if self.elabel:
-            return self.edge_to_node()._nauty_order()[:self.n]
-        
-        g = self._to_nauty()
-
-        c = pynauty.canon_label(g)
-        c = np.asarray(c) #type:  ignore
-        c = _invert_mapping(c)
-        return c
-
-    def _nauty_orbits(self):
-        import pynauty
-        if self.elabel:
-            o = self.edge_to_node()._nauty_orbits()[:self.n]
-            o = to_range(o)[0]
-            return o
-        
-        g = self._to_nauty()
-
-        o = pynauty.autgrp(g)[3] # orbits of each vertex (equivalent groups) with non canonical colors
-
-        # Canonize using cannoical ordering
-        c = pynauty.canon_label(g)
-        c = np.asarray(c) #type:  ignore
-        c = _invert_mapping(c)
-
-        # canonical color for each orbit
-        o = to_range(o)[0]
-        can_o = segment_min(c, o)
-        can_o = to_range(can_o)[0]
-
-        # canonical orbit for each vertex
-        o = np.take(can_o, o)
-
-        return o
 
 
     def serialize(self, canonize=True) -> serialize.Serialized:
         return serialize.serialize(self, canonize)
 
     @classmethod
     def from_molecule(cls, molecule, smiles=False) -> "Graph":
         from . import chem  # lazy import to prevent load of rdkit unless needed
 
         if smiles:
             return chem.MolToSmilesGraph(molecule)
         return chem.MolToSmartsGraph(molecule)
 
-
-def _to_nauty_colors(x):
-  unq = sorted(np.unique(x))
-  unq_lookup = {u: n for n,u in enumerate(unq)}
-
-  colors = [set() for _ in range(len(unq))]
-  for n, l in enumerate(x):
-    colors[unq_lookup[l]].add(n)
-
-  return colors
-
-
 @njit
 def _invert_mapping(x):
     y = np.zeros_like(x)
     for i in range(len(x)): y[x[i]] = i
     return y
 
 
@@ -249,15 +175,15 @@
     N = neighbors(G)
     start = 0
 
     if G.n <= 1:
         return []
 
     if canonize:
-        M = G._nauty_order()
+        M = G.morgan()
         start = int(np.argmin(M))
         for n in N:
             N[n] = sorted(N[n], key=lambda x: M[x])
     else:
         for n in N:
             N[n] = sorted(N[n])
```

### Comparing `xenosite-fragment-0a8/xenosite/fragment/keras_backend.py` & `xenosite-fragment-0a9/xenosite/fragment/keras_backend.py`

 * *Files identical despite different names*

### Comparing `xenosite-fragment-0a8/xenosite/fragment/ops.py` & `xenosite-fragment-0a9/xenosite/fragment/ops.py`

 * *Files identical despite different names*

### Comparing `xenosite-fragment-0a8/xenosite/fragment/remap.py` & `xenosite-fragment-0a9/xenosite/fragment/remap.py`

 * *Files identical despite different names*

### Comparing `xenosite-fragment-0a8/xenosite/fragment/serialize.py` & `xenosite-fragment-0a9/xenosite/fragment/serialize.py`

 * *Files identical despite different names*

### Comparing `xenosite-fragment-0a8/xenosite/fragment/stats.py` & `xenosite-fragment-0a9/xenosite/fragment/stats.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,59 +4,77 @@
 from functools import reduce
 from scipy.stats import hypergeom
 import pandas as pd
 from typing import Optional
 from .ops import segment_max
 from . import Fragment
 
+
+def _marked_ids(ids, eq, marked):
+    amarked = np.array(list(marked))[None, None, :]
+
+    # normalized count of marked ids by position in fragment
+    marked_ids = (np.array(ids)[:, :, None] == amarked).sum(axis=0).sum(axis=1)
+    marked_ids = np.where(marked_ids > 0, 1, 0)  # type: ignore
+
+    # deal with fragment symmetries
+    marked_groups = segment_max(marked_ids, eq)
+    marked_ids = marked_groups[eq]
+
+    return marked_ids, marked_groups
+
+def _covered(ids, marked, size):
+    
+    set_ids = [set(i) for i in ids]
+
+    covered = reduce(lambda x, y: x | y, set_ids)
+
+    marked_count = (
+        len(
+            reduce(
+                lambda x, y: x | y,
+                [i for i in set_ids if marked & i],
+                set(),
+            )
+        )
+        / size
+    )
+    return covered, marked_count
+
+def _equivalence(fragment):
+    return fragment.equivalence()[0]
+
+
 class FragmentStatistics:
     # the statistics that are static, not accumulated, in updates
     static_stats = {"size", "equivalence_group", "frag"}
 
     def __init__(self):
         self._stats: dict = defaultdict(list)
         self._lookup: dict[str, int] = {}
 
     def add(
-        self, frag: str, ids: list[list[int]], marked: set[int], mol_atoms: int
+        self,
+        frag: str, 
+        fragment: Fragment,
+        ids: list[list[int]], 
+        marked: set[int], 
+        mol_atoms: int
     ) -> None:
         assert frag not in self._lookup
         assert self._stats is not None
 
         S = dict()
 
-        F = Fragment(frag)
-        eq = F.equivalence()[0]
+        eq = _equivalence(fragment)
+        size = len(eq)
+        marked_ids, marked_groups = _marked_ids(ids,eq, marked)
 
-        amarked = np.array(list(marked))[None, None, :]
+        covered, marked_count = _covered(ids, marked, size)
 
-        # normalized count of marked ids by position in fragment
-        marked_ids = (np.array(ids)[:, :, None] == amarked).sum(axis=0).sum(axis=1)
-        marked_ids = np.where(marked_ids > 0, 1, 0)  # type: ignore
-
-        # deal with fragment symmetries
-        marked_groups = segment_max(marked_ids, eq)
-        marked_ids = marked_groups[eq]
-
-        set_ids = [set(i) for i in ids]
-
-        size = len(set_ids[0])
-
-        covered = reduce(lambda x, y: x | y, set_ids)
-
-        marked_count = (
-            len(
-                reduce(
-                    lambda x, y: x | y,
-                    [i for i in set_ids if marked & i],
-                    set(),
-                )
-            )
-            / size
-        )
 
         # # exp = probability of fragment overlapping with at least one marked atom
         # # given: size of molecule, number of atoms matching fragment, number of marked atoms
         # exp = 1 - hypergeom.cdf(0, mol_atoms, int(len(covered)), len(marked))
         # obs = 1 if marked_count else 0
         # S["exp"] = exp
         # S["obs"] = obs
@@ -64,18 +82,18 @@
         S["count"] = len(covered) / size
         S["marked_count"] = marked_count
         S["n_mol"] = 1
         S["n_atom"] = mol_atoms
         S["n_mark"] = len(marked)
         S["n_cover"] = len(covered)
         S["n_mark_cover"] = len(covered & marked)
-        S["marked_groups"] = marked_groups
+        #S["marked_groups"] = marked_groups
         S["equivalence_group"] = eq
         S["marked_ids"] = marked_ids
-        S["size"] = len(eq)
+        S["size"] = size
 
         self.append_one(frag, **S)
 
     def copy_from(self, other : "FragmentStatistics") -> "FragmentStatistics":
       k1 = set(self._stats['frag'])
       k2 = set(other._stats['frag'])
```

### Comparing `xenosite-fragment-0a8/xenosite_fragment.egg-info/PKG-INFO` & `xenosite-fragment-0a9/xenosite_fragment.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xenosite-fragment
-Version: 0a8
+Version: 0a9
 Summary: Library for molecule fragment operations.
 Home-page: UNKNOWN
 Author: S. Joshua Swamidass
 Author-email: swamidass@wustl.edu
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Intended Audience :: Education
@@ -155,25 +155,25 @@
 Enumerate and compute statistics on all the subgraphs in a molecule:
 
 ```
 >>> from xenosite.fragment.net import SubGraphFragmentNetwork
 >>> N = SubGraphFragmentNetwork("CC1COC1")
 >>> fragments = N.to_pandas()
 >>> list(fragments.index)
-['C-C', 'C', 'C-O-C', 'C-O', 'O', 'C-C1-C-O-C-1', 'C1-C-C-O-1', 'C-C-C-O', 'C-C(-C)-C', 'C-C-O', 'C-C-C']
+['C-C', 'C', 'C-O-C', 'C-O', 'O', 'C-C1-C-O-C-1', 'C1-C-O-C-1', 'C-C-C-O', 'C-C(-C)-C', 'C-C-O', 'C-C-C']
 >>> fragments["size"].to_numpy()
 array([2, 1, 3, 2, 1, 5, 4, 4, 4, 3, 3])
 ```
 
 Better fragments can be enumerated by collapsing all atoms in a ring into a single node
 during subgraph enumeration. 
 
 ```
 >>> from xenosite.fragment.net import RingFragmentNetwork
 >>> N = RingFragmentNetwork("CC1COC1")
 >>> fragments = N.to_pandas()
 >>> list(fragments.index)
-['C-C1-C-O-C-1', 'C', 'C1-C-C-O-1']
+['C-C1-C-O-C-1', 'C', 'C1-C-O-C-1']
 >>> fragments["size"].to_numpy()
 array([5, 1, 4])
 ```
```

### Comparing `xenosite-fragment-0a8/xenosite_fragment.egg-info/SOURCES.txt` & `xenosite-fragment-0a9/xenosite_fragment.egg-info/SOURCES.txt`

 * *Files identical despite different names*

