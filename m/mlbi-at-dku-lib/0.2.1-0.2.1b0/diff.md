# Comparing `tmp/mlbi_at_dku_lib-0.2.1.tar.gz` & `tmp/mlbi_at_dku_lib-0.2.1b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlbi_at_dku_lib-0.2.1.tar", last modified: Sun Jun 18 14:43:56 2023, max compression
+gzip compressed data, was "mlbi_at_dku_lib-0.2.1b0.tar", last modified: Sun Jul  2 06:48:06 2023, max compression
```

## Comparing `mlbi_at_dku_lib-0.2.1.tar` & `mlbi_at_dku_lib-0.2.1b0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-06-18 14:43:56.528264 mlbi_at_dku_lib-0.2.1/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    35821 2023-05-23 01:43:50.000000 mlbi_at_dku_lib-0.2.1/LICENSE
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       60 2023-05-23 01:43:50.000000 mlbi_at_dku_lib-0.2.1/MANIFEST.in
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      832 2023-06-18 14:43:56.528264 mlbi_at_dku_lib-0.2.1/PKG-INFO
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      175 2023-05-23 01:43:50.000000 mlbi_at_dku_lib-0.2.1/README.md
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-06-18 14:43:56.508265 mlbi_at_dku_lib-0.2.1/mlbi_at_dku_lib/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      163 2023-05-22 09:19:00.000000 mlbi_at_dku_lib-0.2.1/mlbi_at_dku_lib/__init__.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    17825 2023-06-17 08:33:06.000000 mlbi_at_dku_lib-0.2.1/mlbi_at_dku_lib/cpdb.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)     6012 2023-06-15 08:56:21.000000 mlbi_at_dku_lib-0.2.1/mlbi_at_dku_lib/deiso.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    12716 2023-05-23 01:44:36.000000 mlbi_at_dku_lib-0.2.1/mlbi_at_dku_lib/gsea.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    36565 2023-06-18 14:40:16.000000 mlbi_at_dku_lib-0.2.1/mlbi_at_dku_lib/icnv.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    37323 2023-06-15 04:24:26.000000 mlbi_at_dku_lib-0.2.1/mlbi_at_dku_lib/misc.py
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-06-18 14:43:56.520265 mlbi_at_dku_lib-0.2.1/mlbi_at_dku_lib.egg-info/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      832 2023-06-18 14:43:56.000000 mlbi_at_dku_lib-0.2.1/mlbi_at_dku_lib.egg-info/PKG-INFO
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      447 2023-06-18 14:43:56.000000 mlbi_at_dku_lib-0.2.1/mlbi_at_dku_lib.egg-info/SOURCES.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)        1 2023-06-18 14:43:56.000000 mlbi_at_dku_lib-0.2.1/mlbi_at_dku_lib.egg-info/dependency_links.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)        1 2023-06-08 06:54:08.000000 mlbi_at_dku_lib-0.2.1/mlbi_at_dku_lib.egg-info/not-zip-safe
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       27 2023-06-18 14:43:56.000000 mlbi_at_dku_lib-0.2.1/mlbi_at_dku_lib.egg-info/requires.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       22 2023-06-18 14:43:56.000000 mlbi_at_dku_lib-0.2.1/mlbi_at_dku_lib.egg-info/top_level.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       79 2023-06-18 14:43:56.532264 mlbi_at_dku_lib-0.2.1/setup.cfg
--rw-rw-r--   0 syoon     (1001) syoon     (1001)     2823 2023-06-18 14:43:13.000000 mlbi_at_dku_lib-0.2.1/setup.py
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-06-18 14:43:56.520265 mlbi_at_dku_lib-0.2.1/tests/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      124 2023-05-22 09:19:00.000000 mlbi_at_dku_lib-0.2.1/tests/__init__.py
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-02 06:48:06.837368 mlbi_at_dku_lib-0.2.1b0/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    35821 2023-07-02 05:13:01.000000 mlbi_at_dku_lib-0.2.1b0/LICENSE
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       95 2023-07-02 05:13:01.000000 mlbi_at_dku_lib-0.2.1b0/MANIFEST.in
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    41233 2023-07-02 06:48:06.837368 mlbi_at_dku_lib-0.2.1b0/PKG-INFO
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      175 2023-07-02 05:13:01.000000 mlbi_at_dku_lib-0.2.1b0/README.md
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      828 2023-07-02 06:47:35.000000 mlbi_at_dku_lib-0.2.1b0/pyproject.toml
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       38 2023-07-02 06:48:06.837368 mlbi_at_dku_lib-0.2.1b0/setup.cfg
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       49 2023-07-02 05:17:52.000000 mlbi_at_dku_lib-0.2.1b0/setup.py
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-02 06:48:06.829368 mlbi_at_dku_lib-0.2.1b0/src/
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-02 06:48:06.833368 mlbi_at_dku_lib-0.2.1b0/src/mlbi_at_dku_lib/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      163 2023-07-02 05:13:02.000000 mlbi_at_dku_lib-0.2.1b0/src/mlbi_at_dku_lib/__init__.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    17825 2023-07-02 05:13:01.000000 mlbi_at_dku_lib-0.2.1b0/src/mlbi_at_dku_lib/cpdb.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)     6012 2023-07-02 05:13:01.000000 mlbi_at_dku_lib-0.2.1b0/src/mlbi_at_dku_lib/deiso.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    12716 2023-07-02 05:13:02.000000 mlbi_at_dku_lib-0.2.1b0/src/mlbi_at_dku_lib/gsea.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    36548 2023-07-02 05:13:02.000000 mlbi_at_dku_lib-0.2.1b0/src/mlbi_at_dku_lib/icnv.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    37762 2023-07-02 06:36:14.000000 mlbi_at_dku_lib-0.2.1b0/src/mlbi_at_dku_lib/misc.py
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-02 06:48:06.837368 mlbi_at_dku_lib-0.2.1b0/src/mlbi_at_dku_lib.egg-info/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    41233 2023-07-02 06:48:06.000000 mlbi_at_dku_lib-0.2.1b0/src/mlbi_at_dku_lib.egg-info/PKG-INFO
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      486 2023-07-02 06:48:06.000000 mlbi_at_dku_lib-0.2.1b0/src/mlbi_at_dku_lib.egg-info/SOURCES.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)        1 2023-07-02 06:48:06.000000 mlbi_at_dku_lib-0.2.1b0/src/mlbi_at_dku_lib.egg-info/dependency_links.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       52 2023-07-02 06:48:06.000000 mlbi_at_dku_lib-0.2.1b0/src/mlbi_at_dku_lib.egg-info/entry_points.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       54 2023-07-02 06:48:06.000000 mlbi_at_dku_lib-0.2.1b0/src/mlbi_at_dku_lib.egg-info/requires.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       16 2023-07-02 06:48:06.000000 mlbi_at_dku_lib-0.2.1b0/src/mlbi_at_dku_lib.egg-info/top_level.txt
```

### Comparing `mlbi_at_dku_lib-0.2.1/LICENSE` & `mlbi_at_dku_lib-0.2.1b0/LICENSE`

 * *Files identical despite different names*

### Comparing `mlbi_at_dku_lib-0.2.1/mlbi_at_dku_lib/cpdb.py` & `mlbi_at_dku_lib-0.2.1b0/src/mlbi_at_dku_lib/cpdb.py`

 * *Files identical despite different names*

### Comparing `mlbi_at_dku_lib-0.2.1/mlbi_at_dku_lib/deiso.py` & `mlbi_at_dku_lib-0.2.1b0/src/mlbi_at_dku_lib/deiso.py`

 * *Files identical despite different names*

### Comparing `mlbi_at_dku_lib-0.2.1/mlbi_at_dku_lib/gsea.py` & `mlbi_at_dku_lib-0.2.1b0/src/mlbi_at_dku_lib/gsea.py`

 * *Files identical despite different names*

### Comparing `mlbi_at_dku_lib-0.2.1/mlbi_at_dku_lib/icnv.py` & `mlbi_at_dku_lib-0.2.1b0/src/mlbi_at_dku_lib/icnv.py`

 * *Files 0% similar despite different names*

```diff
@@ -997,16 +997,16 @@
         return cluster_label, km
     '''
 
 def detect_tumor_cells(X_cnv, ref_ind, pca = False, use_cnv_score = False, 
                        clust = None, Clustering_resolution = 1, N_clusters = 30,
                        # cluster_key = 'cnv_leiden', score_key = 'tumor_score', 
                        gmm_N_comp = 20, th_min = 0, refp_min = 0.9, p_exc = 0.1, 
-                       dec_margin = 0.05, clustering_res = 4, n_neighbors = 10, gcm = 0.05,
-                       plot_stat = False, use_cnv_cluster = True, use_ref = True, 
+                       dec_margin = 0.05, n_neighbors = 10, gcm = 0.05,
+                       plot_stat = False, use_ref = True, 
                        suffix = '', Data = None):
     
     score_key = 'tumor_score' + suffix
     cluster_key = 'cnv_cluster' 
     ## Get X_pca for ref_type cells
 
     start_time = time.time()
@@ -1026,15 +1026,15 @@
     else: 
         X_pca = np.array(X_cnv.copy(deep = True)) #.copy(deep = True)
             
     if clust:      
         y_clust = list(clust)
     else:
         y_clust, cobj = clustering_alg(X_pca, clust_algo = CLUSTERING_AGO, N_clusters = N_clusters, 
-                                resolution = Clustering_resolution)
+                                resolution = Clustering_resolution, N_neighbors = n_neighbors)
         
     cnv_clust_lst = list(set(y_clust))
     df[cluster_key] = y_clust
         
     if use_ref:
         cnv_clust_lst.sort()
         b_inc = []
```

### Comparing `mlbi_at_dku_lib-0.2.1/mlbi_at_dku_lib/misc.py` & `mlbi_at_dku_lib-0.2.1b0/src/mlbi_at_dku_lib/misc.py`

 * *Files 5% similar despite different names*

```diff
@@ -1099,7 +1099,22 @@
     else:
         adj = kneighbors_graph(X_pca, int(N_neighbors), mode='connectivity', include_self=True)
         louvain = Louvain(resolution = resolution)
         cluster_label = louvain.fit_transform(adj)        
         return cluster_label, louvain
 
     return
+
+
+from importlib_resources import files
+
+def load_GTmap( target = 'hg38' ):
+    
+    if target in ['hg38', 'hg19', 'mm10']:
+        path = files('mlbi_at_dku_lib.data').joinpath('GTmap_%s.csv' % target)
+        return pd.read_csv(path, index_col = 0)
+    else:
+        print('ERROR: cannot find the data file %s.' % ('GTmap_%s.csv' % target))
+        print('You can choose one of hg38, hg19, mm10')
+        return None
+    
+    return None
```

