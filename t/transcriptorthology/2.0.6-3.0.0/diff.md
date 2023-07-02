# Comparing `tmp/transcriptorthology-2.0.6.tar.gz` & `tmp/transcriptorthology-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/transcriptorthology-2.0.6.tar", last modified: Mon Jun 26 06:21:30 2023, max compression
+gzip compressed data, was "dist/transcriptorthology-3.0.0.tar", last modified: Sun Jul  2 03:16:48 2023, max compression
```

## Comparing `transcriptorthology-2.0.6.tar` & `transcriptorthology-3.0.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 ouew2201 (1811316550) domain^users (1810891265)        0 2023-06-26 06:21:30.000000 transcriptorthology-2.0.6/
-drwxr-xr-x   0 ouew2201 (1811316550) domain^users (1810891265)        0 2023-06-26 06:21:30.000000 transcriptorthology-2.0.6/transcriptorthology/
--rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)    23446 2023-06-26 06:21:09.000000 transcriptorthology-2.0.6/transcriptorthology/tsmComputing.py
--rw-------   0 ouew2201 (1811316550) domain^users (1810891265)      123 2023-06-26 06:21:16.000000 transcriptorthology-2.0.6/transcriptorthology/__init__.py
--rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)     2915 2023-06-26 06:21:03.000000 transcriptorthology-2.0.6/transcriptorthology/transcriptOrthology.py
--rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)    15635 2023-06-26 06:20:56.000000 transcriptorthology-2.0.6/transcriptorthology/Tclustering.py
--rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)     1071 2023-06-26 06:20:45.000000 transcriptorthology-2.0.6/setup.py
--rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)     2833 2023-06-26 06:21:30.000000 transcriptorthology-2.0.6/PKG-INFO
--rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)       38 2023-06-26 06:21:30.000000 transcriptorthology-2.0.6/setup.cfg
-drwxr-xr-x   0 ouew2201 (1811316550) domain^users (1810891265)        0 2023-06-26 06:21:30.000000 transcriptorthology-2.0.6/transcriptorthology.egg-info/
--rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)        1 2023-06-26 06:21:30.000000 transcriptorthology-2.0.6/transcriptorthology.egg-info/dependency_links.txt
--rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)      378 2023-06-26 06:21:30.000000 transcriptorthology-2.0.6/transcriptorthology.egg-info/SOURCES.txt
--rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)       41 2023-06-26 06:21:30.000000 transcriptorthology-2.0.6/transcriptorthology.egg-info/requires.txt
--rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)     2833 2023-06-26 06:21:30.000000 transcriptorthology-2.0.6/transcriptorthology.egg-info/PKG-INFO
--rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)       20 2023-06-26 06:21:30.000000 transcriptorthology-2.0.6/transcriptorthology.egg-info/top_level.txt
--rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)     2180 2023-06-26 05:12:33.000000 transcriptorthology-2.0.6/README.md
+drwxr-xr-x   0 ouew2201 (1811316550) domain^users (1810891265)        0 2023-07-02 03:16:48.000000 transcriptorthology-3.0.0/
+drwxr-xr-x   0 ouew2201 (1811316550) domain^users (1810891265)        0 2023-07-02 03:16:48.000000 transcriptorthology-3.0.0/transcriptorthology/
+-rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)    23446 2023-07-02 03:13:19.000000 transcriptorthology-3.0.0/transcriptorthology/tsmComputing.py
+-rw-------   0 ouew2201 (1811316550) domain^users (1810891265)      123 2023-06-26 06:21:16.000000 transcriptorthology-3.0.0/transcriptorthology/__init__.py
+-rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)     2915 2023-07-02 03:13:10.000000 transcriptorthology-3.0.0/transcriptorthology/transcriptOrthology.py
+-rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)    14592 2023-07-02 03:12:59.000000 transcriptorthology-3.0.0/transcriptorthology/Tclustering.py
+-rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)     1071 2023-07-02 03:13:46.000000 transcriptorthology-3.0.0/setup.py
+-rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)     2774 2023-07-02 03:16:48.000000 transcriptorthology-3.0.0/PKG-INFO
+-rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)       38 2023-07-02 03:16:48.000000 transcriptorthology-3.0.0/setup.cfg
+drwxr-xr-x   0 ouew2201 (1811316550) domain^users (1810891265)        0 2023-07-02 03:16:48.000000 transcriptorthology-3.0.0/transcriptorthology.egg-info/
+-rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)        1 2023-07-02 03:16:48.000000 transcriptorthology-3.0.0/transcriptorthology.egg-info/dependency_links.txt
+-rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)      378 2023-07-02 03:16:48.000000 transcriptorthology-3.0.0/transcriptorthology.egg-info/SOURCES.txt
+-rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)       41 2023-07-02 03:16:48.000000 transcriptorthology-3.0.0/transcriptorthology.egg-info/requires.txt
+-rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)     2774 2023-07-02 03:16:48.000000 transcriptorthology-3.0.0/transcriptorthology.egg-info/PKG-INFO
+-rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)       20 2023-07-02 03:16:48.000000 transcriptorthology-3.0.0/transcriptorthology.egg-info/top_level.txt
+-rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)     2121 2023-07-02 03:15:58.000000 transcriptorthology-3.0.0/README.md
```

### Comparing `transcriptorthology-2.0.6/transcriptorthology/tsmComputing.py` & `transcriptorthology-3.0.0/transcriptorthology/tsmComputing.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 ======
     https://github.com/UdeS-CoBIUS/TranscriptOrthology
 """
 __authors__ = ("Wend Yam Donald Davy Ouedraogo")
 __contact__ = ("wend.yam.donald.davy.usherbrooke.ca")
 __copyright__ = "CoBIUS lab at Université de Sherbrooke, QC, CANADA"
 __date__ = "2023-06-26"
-__version__= "2.0.6"
+__version__= "3.0.0"
 
 import pandas as pd
 import argparse
 import time
 import numpy as np
 
 def build_arg_parser():
```

### Comparing `transcriptorthology-2.0.6/transcriptorthology/transcriptOrthology.py` & `transcriptorthology-3.0.0/transcriptorthology/transcriptOrthology.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 ======
     https://github.com/UdeS-CoBIUS/TranscriptOrthology
 """
 __authors__ = ("Wend Yam Donald Davy Ouedraogo")
 __contact__ = ("wend.yam.donald.davy.usherbrooke.ca")
 __copyright__ = "CoBIUS lab at Université de Sherbrooke, QC, CANADA"
 __date__ = "2023-06-26"
-__version__= "2.0.6"
+__version__= "3.0.0"
 
 
 import argparse
 from .Tclustering import get_orthology_graph
 from .tsmComputing import get_matrix
```

### Comparing `transcriptorthology-2.0.6/transcriptorthology/Tclustering.py` & `transcriptorthology-3.0.0/transcriptorthology/Tclustering.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 ======
     https://github.com/UdeS-CoBIUS/TranscriptOrthology
 """
 __authors__ = ("Wend Yam Donald Davy Ouedraogo")
 __contact__ = ("wend.yam.donald.davy.usherbrooke.ca")
 __copyright__ = "CoBIUS lab at Université de Sherbrooke, QC, CANADA"
 __date__ = "2023-06-26"
-__version__= "2.0.6"
+__version__= "3.0.0"
 
 import pandas as pd
 import networkx as nx
 import time
 from ete3 import Tree
 import matplotlib.pyplot as plt
 import argparse
@@ -197,61 +197,43 @@
     if is_saving:
         nx.draw(G, with_labels=True)
         plt.savefig('{}/start_orthology_graph.pdf'.format(output_folder))
         #plt.show(G)
 
 
     edges_data = edges_data.sort_values(by=['score'], ascending=False)
-
+    
     for index_edge, row_edge in edges_data.iterrows():
         transcript_id = row_edge['pair_id']
         transcript_ref = row_edge['pair_ref']
-
+        
+        # get the CC of the two transcripts
         adj_trID_with_weight = G.adj[transcript_id]
         adj_trID = [ _ for _ in list(adj_trID_with_weight.keys()) if _ != transcript_ref]
+        
         adj_trREF_with_weight = G.adj[transcript_ref]
         adj_trREF = [ _ for _ in list(adj_trREF_with_weight.keys()) if _ != transcript_id]
-        
-        genes_adj_trID = list(set([g[g['id_transcript']==tr].id_gene.values[0] for tr in adj_trID]))
-        genes_adj_trREF = list(set([g[g['id_transcript']==tr].id_gene.values[0] for tr in adj_trREF]))
-
-        intersect_genes = list(set(genes_adj_trID).intersection(set(genes_adj_trREF)))
-
-        if len(intersect_genes) == 0:
+                
+        if set(adj_trREF) == set(adj_trID):
             G.add_edge(transcript_id, transcript_ref)
         else:
-            for intersect_gene in intersect_genes:
-                spes_adj_trID = [ _ for _ in adj_trID if g[g['id_transcript']==_].id_gene.values[0]==intersect_gene]
-                spes_adj_trREF = [ _ for _ in adj_trREF if g[g['id_transcript']==_].id_gene.values[0]==intersect_gene]
+            merge = True
+            current_edges =list(G.edges())
+            for transcript_adj_ref in adj_trREF:
+                gene_transcript_adj_ref = g[g['id_transcript']==transcript_adj_ref].id_gene.values
+                for transcript_adj_id in adj_trID:
+                    gene_transcript_adj_id = g[g['id_transcript']==transcript_adj_id].id_gene.values
+                    if transcript_adj_id != transcript_adj_ref:
+                        current_edge = (transcript_adj_id, transcript_adj_ref)
+                        if (gene_transcript_adj_id == gene_transcript_adj_ref) and (current_edge not in current_edges):
+                            merge = False
+                            break
+            if merge:
+                G.add_edge(transcript_id, transcript_ref)
 
-                
-                list_inParalogs_adj_trID = []
-                inParalogs_adj_trID = [inParalogs[_] for _ in spes_adj_trID]
-                for spe_adj_trID in spes_adj_trID:
-                    inParalogs_adj_trID = inParalogs[spe_adj_trID]
-                    for inparalog_adj_trID in inParalogs_adj_trID:
-                        list_inParalogs_adj_trID.append(inparalog_adj_trID)
-                
-                list_inParalogs_adj_trREF = []
-                inParalogs_adj_trREF = [inParalogs[_] for _ in spes_adj_trREF]
-                for spe_adj_trREF in spes_adj_trREF:
-                    inParalogs_adj_trREF = inParalogs[spe_adj_trREF]
-                    for inparalog_adj_trREF in inParalogs_adj_trREF:
-                        list_inParalogs_adj_trREF.append(inparalog_adj_trREF)
-
-                list_inParalogs_adj_trID.extend(spes_adj_trID)
-                list_inParalogs_adj_trREF.extend(spes_adj_trREF)
-                set_id = set(list_inParalogs_adj_trID)
-                set_ref =set(list_inParalogs_adj_trREF)
-
-                inter_set = set_id.intersection(set_ref)
-
-                if len(inter_set) == len(set_id) and len(inter_set) == len(set_ref):
-                #if len(inter_set) == max(len(set_id), len(set_ref)):
-                    G.add_edge(transcript_id, transcript_ref)
     if is_saving:
         plt.clf()
         nx.draw(G, with_labels=True)
         #plt.show(G)
         plt.savefig('{}/end_orthology_graph.pdf'.format(output_folder))
     clusters_components = [list(G.subgraph(c).copy()) for c in nx.connected_components(G)]
     return clusters_components
```

### Comparing `transcriptorthology-2.0.6/setup.py` & `transcriptorthology-3.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
-VERSION = '2.0.6'
+VERSION = '3.0.0'
 DESCRIPTION = 'A transcript orthologies inferring package'
 
 setup(
     name="transcriptorthology",
     version=VERSION,
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
```

### Comparing `transcriptorthology-2.0.6/PKG-INFO` & `transcriptorthology-3.0.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,56 +1,56 @@
 Metadata-Version: 2.1
 Name: transcriptorthology
-Version: 2.0.6
+Version: 3.0.0
 Summary: A transcript orthologies inferring package
 Home-page: https://github.com/UdeS-CoBIUS/TranscriptOrthology
 Author: Wend Yam Donald Davy Ouedraogo
 Author-email: wend.yam.donald.davy.ouedraogo@usherbrooke.ca
 License: MIT
 Keywords: clustering,alternative-splicing,orthoogy-inference,isoorthology,algorithm,evolution,computational-biology
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 
 
-# :dna: Inferring clusters of orthologous and paralogous transcripts
+# Inferring clusters of orthologous and paralogous transcripts
 
 ``Algorithm to infer clusters of isoorthologous transcripts using gene-level homology relationships and a Reciprocal Best Hits approach``
 
 ![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png)
 
 <!-- ABOUT THE PROJECT -->
-<h2 id="about-the-project"> :pencil: About The Project</h2>
+<h2 id="about-the-project">About The Project</h2>
 
 
 <!-- OVERVIEW -->
-<h3 id="overview"> :cloud: Overview</h3>
+<h3 id="overview">Overview</h3>
 
-`A graph-based method to infer isoorthology & recent paralogy relations in a set of homologous transcripts:dna:`
+`A graph-based method to infer isoorthology & recent paralogy relations in a set of homologous transcripts`
 
 ---
 
 
 <!-- Requirements -->
-<h3 id="requirements"> :hammer_and_pick: Requirements</h3>
+<h3 id="requirements"> Requirements</h3>
 
 *   __`python3 (at leat python 3.6)`__
 *   __`NetworkX`__
 *   __`Pandas`__
 *   __`Numpy`__
 *   __`ETE toolkit`__
 
 
 ![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png)
 
 <!-- Package -->
-<h3 id="package"> :package: About the package</h3>
+<h3 id="package">About the package</h3>
 
 ``install the package``
 <pre><code>pip3 install transcriptorthology</code></pre>
 
 ``import package and use the main function``
 <pre><code>from transcriptorthology.transcriptOrthology import inferring_transcripts_isoorthology
```

### Comparing `transcriptorthology-2.0.6/transcriptorthology.egg-info/PKG-INFO` & `transcriptorthology-3.0.0/transcriptorthology.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,56 +1,56 @@
 Metadata-Version: 2.1
 Name: transcriptorthology
-Version: 2.0.6
+Version: 3.0.0
 Summary: A transcript orthologies inferring package
 Home-page: https://github.com/UdeS-CoBIUS/TranscriptOrthology
 Author: Wend Yam Donald Davy Ouedraogo
 Author-email: wend.yam.donald.davy.ouedraogo@usherbrooke.ca
 License: MIT
 Keywords: clustering,alternative-splicing,orthoogy-inference,isoorthology,algorithm,evolution,computational-biology
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 
 
-# :dna: Inferring clusters of orthologous and paralogous transcripts
+# Inferring clusters of orthologous and paralogous transcripts
 
 ``Algorithm to infer clusters of isoorthologous transcripts using gene-level homology relationships and a Reciprocal Best Hits approach``
 
 ![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png)
 
 <!-- ABOUT THE PROJECT -->
-<h2 id="about-the-project"> :pencil: About The Project</h2>
+<h2 id="about-the-project">About The Project</h2>
 
 
 <!-- OVERVIEW -->
-<h3 id="overview"> :cloud: Overview</h3>
+<h3 id="overview">Overview</h3>
 
-`A graph-based method to infer isoorthology & recent paralogy relations in a set of homologous transcripts:dna:`
+`A graph-based method to infer isoorthology & recent paralogy relations in a set of homologous transcripts`
 
 ---
 
 
 <!-- Requirements -->
-<h3 id="requirements"> :hammer_and_pick: Requirements</h3>
+<h3 id="requirements"> Requirements</h3>
 
 *   __`python3 (at leat python 3.6)`__
 *   __`NetworkX`__
 *   __`Pandas`__
 *   __`Numpy`__
 *   __`ETE toolkit`__
 
 
 ![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png)
 
 <!-- Package -->
-<h3 id="package"> :package: About the package</h3>
+<h3 id="package">About the package</h3>
 
 ``install the package``
 <pre><code>pip3 install transcriptorthology</code></pre>
 
 ``import package and use the main function``
 <pre><code>from transcriptorthology.transcriptOrthology import inferring_transcripts_isoorthology
```

### Comparing `transcriptorthology-2.0.6/README.md` & `transcriptorthology-3.0.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 
-# :dna: Inferring clusters of orthologous and paralogous transcripts
+# Inferring clusters of orthologous and paralogous transcripts
 
 ``Algorithm to infer clusters of isoorthologous transcripts using gene-level homology relationships and a Reciprocal Best Hits approach``
 
 ![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png)
 
 <!-- ABOUT THE PROJECT -->
-<h2 id="about-the-project"> :pencil: About The Project</h2>
+<h2 id="about-the-project">About The Project</h2>
 
 
 <!-- OVERVIEW -->
-<h3 id="overview"> :cloud: Overview</h3>
+<h3 id="overview">Overview</h3>
 
-`A graph-based method to infer isoorthology & recent paralogy relations in a set of homologous transcripts:dna:`
+`A graph-based method to infer isoorthology & recent paralogy relations in a set of homologous transcripts`
 
 ---
 
 
 <!-- Requirements -->
-<h3 id="requirements"> :hammer_and_pick: Requirements</h3>
+<h3 id="requirements"> Requirements</h3>
 
 *   __`python3 (at leat python 3.6)`__
 *   __`NetworkX`__
 *   __`Pandas`__
 *   __`Numpy`__
 *   __`ETE toolkit`__
 
 
 ![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png)
 
 <!-- Package -->
-<h3 id="package"> :package: About the package</h3>
+<h3 id="package">About the package</h3>
 
 ``install the package``
 <pre><code>pip3 install transcriptorthology</code></pre>
 
 ``import package and use the main function``
 <pre><code>from transcriptorthology.transcriptOrthology import inferring_transcripts_isoorthology
```

