# Comparing `tmp/LZGraphs-0.25.tar.gz` & `tmp/LZGraphs-0.26.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LZGraphs-0.25.tar", last modified: Mon Jun 12 07:19:22 2023, max compression
+gzip compressed data, was "LZGraphs-0.26.tar", last modified: Sun Jul  2 13:19:53 2023, max compression
```

## Comparing `LZGraphs-0.25.tar` & `LZGraphs-0.26.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 07:19:22.392632 LZGraphs-0.25/
--rw-rw-rw-   0        0        0     1079 2021-01-04 22:48:55.000000 LZGraphs-0.25/LICENSE
-drwxrwxrwx   0        0        0        0 2023-06-12 07:19:22.379170 LZGraphs-0.25/LZGraphs/
--rw-rw-rw-   0        0        0    27173 2023-06-12 07:08:25.000000 LZGraphs-0.25/LZGraphs/AminoAcidPositional.py
--rw-rw-rw-   0        0        0     4625 2023-06-12 07:08:25.000000 LZGraphs-0.25/LZGraphs/BOWEncoder.py
--rw-rw-rw-   0        0        0    34741 2023-06-12 07:08:25.000000 LZGraphs-0.25/LZGraphs/LZGraphBase.py
--rw-rw-rw-   0        0        0    28270 2023-06-12 07:08:25.000000 LZGraphs-0.25/LZGraphs/Naive.py
--rw-rw-rw-   0        0        0     6600 2023-06-12 07:08:25.000000 LZGraphs-0.25/LZGraphs/NodeEdgeSaturationProbe.py
--rw-rw-rw-   0        0        0    23649 2023-06-12 07:08:25.000000 LZGraphs-0.25/LZGraphs/NucleotideDoublePositional.py
--rw-rw-rw-   0        0        0     6842 2023-06-12 07:08:25.000000 LZGraphs-0.25/LZGraphs/Utilities.py
--rw-rw-rw-   0        0        0     6387 2023-06-12 07:08:25.000000 LZGraphs-0.25/LZGraphs/Visualize.py
--rw-rw-rw-   0        0        0      356 2023-06-12 07:08:25.000000 LZGraphs-0.25/LZGraphs/__init__.py
--rw-rw-rw-   0        0        0     1041 2023-05-21 15:14:59.000000 LZGraphs-0.25/LZGraphs/decomposition.py
--rw-rw-rw-   0        0        0     2380 2023-06-12 07:08:25.000000 LZGraphs-0.25/LZGraphs/misc.py
-drwxrwxrwx   0        0        0        0 2023-06-12 07:19:22.392136 LZGraphs-0.25/LZGraphs.egg-info/
--rw-rw-rw-   0        0        0     4117 2023-06-12 07:19:21.000000 LZGraphs-0.25/LZGraphs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      502 2023-06-12 07:19:22.000000 LZGraphs-0.25/LZGraphs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 07:19:21.000000 LZGraphs-0.25/LZGraphs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       83 2023-06-12 07:19:21.000000 LZGraphs-0.25/LZGraphs.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-12 07:19:22.000000 LZGraphs-0.25/LZGraphs.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       85 2021-01-04 22:48:55.000000 LZGraphs-0.25/MANIFEST.in
--rw-rw-rw-   0        0        0     4117 2023-06-12 07:19:22.393127 LZGraphs-0.25/PKG-INFO
--rw-rw-rw-   0        0        0     3434 2023-06-12 07:09:33.000000 LZGraphs-0.25/README.md
--rw-rw-rw-   0        0        0       98 2021-01-04 22:48:55.000000 LZGraphs-0.25/pyproject.toml
--rw-rw-rw-   0        0        0      119 2023-06-12 07:19:22.393624 LZGraphs-0.25/setup.cfg
--rw-rw-rw-   0        0        0     1331 2023-06-12 07:17:07.000000 LZGraphs-0.25/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-02 13:19:53.471274 LZGraphs-0.26/
+-rw-rw-rw-   0        0        0     1079 2021-01-04 22:48:55.000000 LZGraphs-0.26/LICENSE
+drwxrwxrwx   0        0        0        0 2023-07-02 13:19:53.456890 LZGraphs-0.26/LZGraphs/
+-rw-rw-rw-   0        0        0    27173 2023-06-12 07:08:25.000000 LZGraphs-0.26/LZGraphs/AminoAcidPositional.py
+-rw-rw-rw-   0        0        0     4625 2023-06-12 07:08:25.000000 LZGraphs-0.26/LZGraphs/BOWEncoder.py
+-rw-rw-rw-   0        0        0    34741 2023-06-12 07:08:25.000000 LZGraphs-0.26/LZGraphs/LZGraphBase.py
+-rw-rw-rw-   0        0        0     2883 2023-06-28 14:34:19.000000 LZGraphs-0.26/LZGraphs/Metrics.py
+-rw-rw-rw-   0        0        0    28270 2023-06-12 07:08:25.000000 LZGraphs-0.26/LZGraphs/Naive.py
+-rw-rw-rw-   0        0        0     6661 2023-06-28 14:29:07.000000 LZGraphs-0.26/LZGraphs/NodeEdgeSaturationProbe.py
+-rw-rw-rw-   0        0        0    23649 2023-06-12 07:08:25.000000 LZGraphs-0.26/LZGraphs/NucleotideDoublePositional.py
+-rw-rw-rw-   0        0        0     6841 2023-06-28 14:18:33.000000 LZGraphs-0.26/LZGraphs/Utilities.py
+-rw-rw-rw-   0        0        0     6387 2023-06-12 07:08:25.000000 LZGraphs-0.26/LZGraphs/Visualize.py
+-rw-rw-rw-   0        0        0      356 2023-06-12 07:08:25.000000 LZGraphs-0.26/LZGraphs/__init__.py
+-rw-rw-rw-   0        0        0     1041 2023-05-21 15:14:59.000000 LZGraphs-0.26/LZGraphs/decomposition.py
+-rw-rw-rw-   0        0        0     2380 2023-06-12 07:08:25.000000 LZGraphs-0.26/LZGraphs/misc.py
+drwxrwxrwx   0        0        0        0 2023-07-02 13:19:53.470777 LZGraphs-0.26/LZGraphs.egg-info/
+-rw-rw-rw-   0        0        0     8222 2023-07-02 13:19:52.000000 LZGraphs-0.26/LZGraphs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      522 2023-07-02 13:19:53.000000 LZGraphs-0.26/LZGraphs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-02 13:19:52.000000 LZGraphs-0.26/LZGraphs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       83 2023-07-02 13:19:53.000000 LZGraphs-0.26/LZGraphs.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-02 13:19:53.000000 LZGraphs-0.26/LZGraphs.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       85 2021-01-04 22:48:55.000000 LZGraphs-0.26/MANIFEST.in
+-rw-rw-rw-   0        0        0     8222 2023-07-02 13:19:53.471274 LZGraphs-0.26/PKG-INFO
+-rw-rw-rw-   0        0        0     6712 2023-07-02 13:04:37.000000 LZGraphs-0.26/README.md
+-rw-rw-rw-   0        0        0       98 2021-01-04 22:48:55.000000 LZGraphs-0.26/pyproject.toml
+-rw-rw-rw-   0        0        0      119 2023-07-02 13:19:53.472266 LZGraphs-0.26/setup.cfg
+-rw-rw-rw-   0        0        0     1912 2023-07-02 13:15:56.000000 LZGraphs-0.26/setup.py
```

### Comparing `LZGraphs-0.25/LICENSE` & `LZGraphs-0.26/LICENSE`

 * *Files identical despite different names*

### Comparing `LZGraphs-0.25/LZGraphs/AminoAcidPositional.py` & `LZGraphs-0.26/LZGraphs/AminoAcidPositional.py`

 * *Files identical despite different names*

### Comparing `LZGraphs-0.25/LZGraphs/BOWEncoder.py` & `LZGraphs-0.26/LZGraphs/BOWEncoder.py`

 * *Files identical despite different names*

### Comparing `LZGraphs-0.25/LZGraphs/LZGraphBase.py` & `LZGraphs-0.26/LZGraphs/LZGraphBase.py`

 * *Files identical despite different names*

### Comparing `LZGraphs-0.25/LZGraphs/Naive.py` & `LZGraphs-0.26/LZGraphs/Naive.py`

 * *Files identical despite different names*

### Comparing `LZGraphs-0.25/LZGraphs/NodeEdgeSaturationProbe.py` & `LZGraphs-0.26/LZGraphs/NodeEdgeSaturationProbe.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,14 +36,16 @@
         self.node_function = None
         if node_function == 'naive':
             self.node_function = self.naive_node_extractor
         elif node_function == 'ndp':
             self.node_function = self.ndp_node_extractor
         elif node_function == 'aap':
             self.node_function = self.aap_node_extractor
+        else:
+            self.node_function = node_function
 
     def log(self, args):
         if self.log_level == 1:
             self.log_memory[args] = {'nodes': len(self.nodes), 'edges': len(self.edges)}
 
     @staticmethod
     def naive_node_extractor(seq):
```

### Comparing `LZGraphs-0.25/LZGraphs/NucleotideDoublePositional.py` & `LZGraphs-0.26/LZGraphs/NucleotideDoublePositional.py`

 * *Files identical despite different names*

### Comparing `LZGraphs-0.25/LZGraphs/Utilities.py` & `LZGraphs-0.26/LZGraphs/Utilities.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,14 @@
             jgs.append(col)
 
     column[vgs] *= vsum
     column[jgs] *= jsum
 
     return column
 
-
 def renormalize_edege_genes(column):
     """ This function is used during the graph union operation, it normalizes the gene counts by the total number
     of observed v / j genes/alleles.
                     Args:
                         column (pandas Series): An LZGraph
                     Returns:
                         pandas Series: padnas series of v and j counts instead of probabilites
```

### Comparing `LZGraphs-0.25/LZGraphs/Visualize.py` & `LZGraphs-0.26/LZGraphs/Visualize.py`

 * *Files identical despite different names*

### Comparing `LZGraphs-0.25/LZGraphs/decomposition.py` & `LZGraphs-0.26/LZGraphs/decomposition.py`

 * *Files identical despite different names*

### Comparing `LZGraphs-0.25/LZGraphs/misc.py` & `LZGraphs-0.26/LZGraphs/misc.py`

 * *Files identical despite different names*

