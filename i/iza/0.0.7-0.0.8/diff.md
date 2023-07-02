# Comparing `tmp/iza-0.0.7.tar.gz` & `tmp/iza-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iza-0.0.7.tar", last modified: Sat Jul  1 14:54:34 2023, max compression
+gzip compressed data, was "iza-0.0.8.tar", last modified: Sat Jul  1 15:15:03 2023, max compression
```

## Comparing `iza-0.0.7.tar` & `iza-0.0.8.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-07-01 14:54:34.453100 iza-0.0.7/
--rw-rw-r--   0 solst      (501) staff       (20)    11337 2023-04-27 10:12:58.000000 iza-0.0.7/LICENSE
--rw-rw-r--   0 solst      (501) staff       (20)      111 2023-04-27 10:12:58.000000 iza-0.0.7/MANIFEST.in
--rw-r--r--   0 solst      (501) staff       (20)     1969 2023-07-01 14:54:34.452969 iza-0.0.7/PKG-INFO
--rw-r--r--   0 solst      (501) staff       (20)     1348 2023-06-24 20:51:36.000000 iza-0.0.7/README.md
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-07-01 14:54:34.451694 iza-0.0.7/iza/
--rw-r--r--   0 solst      (501) staff       (20)       22 2023-07-01 14:53:52.000000 iza-0.0.7/iza/__init__.py
--rw-r--r--   0 solst      (501) staff       (20)    20856 2023-07-01 14:53:52.000000 iza-0.0.7/iza/_modidx.py
--rw-r--r--   0 solst      (501) staff       (20)     2046 2023-07-01 14:53:52.000000 iza-0.0.7/iza/commands.py
--rw-r--r--   0 solst      (501) staff       (20)     2264 2023-07-01 14:53:52.000000 iza-0.0.7/iza/imp.py
--rw-r--r--   0 solst      (501) staff       (20)    14824 2023-07-01 14:53:52.000000 iza-0.0.7/iza/nbs.py
--rw-r--r--   0 solst      (501) staff       (20)     4983 2023-07-01 14:53:52.000000 iza-0.0.7/iza/plots.py
--rw-r--r--   0 solst      (501) staff       (20)      448 2023-07-01 14:53:52.000000 iza-0.0.7/iza/rich.py
--rw-r--r--   0 solst      (501) staff       (20)     8199 2023-07-01 14:53:52.000000 iza-0.0.7/iza/static.py
--rw-r--r--   0 solst      (501) staff       (20)      191 2023-07-01 14:53:52.000000 iza-0.0.7/iza/typer.py
--rw-r--r--   0 solst      (501) staff       (20)     4395 2023-07-01 14:53:52.000000 iza-0.0.7/iza/types.py
--rw-r--r--   0 solst      (501) staff       (20)    54797 2023-07-01 14:53:52.000000 iza-0.0.7/iza/utils.py
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-07-01 14:54:34.452751 iza-0.0.7/iza.egg-info/
--rw-r--r--   0 solst      (501) staff       (20)     1969 2023-07-01 14:54:34.000000 iza-0.0.7/iza.egg-info/PKG-INFO
--rw-r--r--   0 solst      (501) staff       (20)      388 2023-07-01 14:54:34.000000 iza-0.0.7/iza.egg-info/SOURCES.txt
--rw-r--r--   0 solst      (501) staff       (20)        1 2023-07-01 14:54:34.000000 iza-0.0.7/iza.egg-info/dependency_links.txt
--rw-r--r--   0 solst      (501) staff       (20)       70 2023-07-01 14:54:34.000000 iza-0.0.7/iza.egg-info/entry_points.txt
--rw-r--r--   0 solst      (501) staff       (20)        1 2023-06-24 20:04:21.000000 iza-0.0.7/iza.egg-info/not-zip-safe
--rw-r--r--   0 solst      (501) staff       (20)       80 2023-07-01 14:54:34.000000 iza-0.0.7/iza.egg-info/requires.txt
--rw-r--r--   0 solst      (501) staff       (20)        4 2023-07-01 14:54:34.000000 iza-0.0.7/iza.egg-info/top_level.txt
--rw-r--r--   0 solst      (501) staff       (20)      905 2023-07-01 14:53:49.000000 iza-0.0.7/settings.ini
--rw-r--r--   0 solst      (501) staff       (20)       38 2023-07-01 14:54:34.453143 iza-0.0.7/setup.cfg
--rw-rw-r--   0 solst      (501) staff       (20)     2596 2023-06-27 21:50:00.000000 iza-0.0.7/setup.py
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-07-01 15:15:03.479404 iza-0.0.8/
+-rw-rw-r--   0 solst      (501) staff       (20)    11337 2023-04-27 10:12:58.000000 iza-0.0.8/LICENSE
+-rw-rw-r--   0 solst      (501) staff       (20)      111 2023-04-27 10:12:58.000000 iza-0.0.8/MANIFEST.in
+-rw-r--r--   0 solst      (501) staff       (20)     2036 2023-07-01 15:15:03.479277 iza-0.0.8/PKG-INFO
+-rw-r--r--   0 solst      (501) staff       (20)     1415 2023-07-01 15:14:40.000000 iza-0.0.8/README.md
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-07-01 15:15:03.478139 iza-0.0.8/iza/
+-rw-r--r--   0 solst      (501) staff       (20)       22 2023-07-01 15:14:49.000000 iza-0.0.8/iza/__init__.py
+-rw-r--r--   0 solst      (501) staff       (20)    20856 2023-07-01 15:14:49.000000 iza-0.0.8/iza/_modidx.py
+-rw-r--r--   0 solst      (501) staff       (20)     2046 2023-07-01 15:14:49.000000 iza-0.0.8/iza/commands.py
+-rw-r--r--   0 solst      (501) staff       (20)     2264 2023-07-01 15:14:49.000000 iza-0.0.8/iza/imp.py
+-rw-r--r--   0 solst      (501) staff       (20)    14824 2023-07-01 15:14:49.000000 iza-0.0.8/iza/nbs.py
+-rw-r--r--   0 solst      (501) staff       (20)     4983 2023-07-01 15:14:49.000000 iza-0.0.8/iza/plots.py
+-rw-r--r--   0 solst      (501) staff       (20)      448 2023-07-01 15:14:49.000000 iza-0.0.8/iza/rich.py
+-rw-r--r--   0 solst      (501) staff       (20)     9068 2023-07-01 15:14:49.000000 iza-0.0.8/iza/static.py
+-rw-r--r--   0 solst      (501) staff       (20)      191 2023-07-01 15:14:49.000000 iza-0.0.8/iza/typer.py
+-rw-r--r--   0 solst      (501) staff       (20)     4395 2023-07-01 15:14:49.000000 iza-0.0.8/iza/types.py
+-rw-r--r--   0 solst      (501) staff       (20)    54797 2023-07-01 15:14:49.000000 iza-0.0.8/iza/utils.py
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-07-01 15:15:03.479107 iza-0.0.8/iza.egg-info/
+-rw-r--r--   0 solst      (501) staff       (20)     2036 2023-07-01 15:15:03.000000 iza-0.0.8/iza.egg-info/PKG-INFO
+-rw-r--r--   0 solst      (501) staff       (20)      388 2023-07-01 15:15:03.000000 iza-0.0.8/iza.egg-info/SOURCES.txt
+-rw-r--r--   0 solst      (501) staff       (20)        1 2023-07-01 15:15:03.000000 iza-0.0.8/iza.egg-info/dependency_links.txt
+-rw-r--r--   0 solst      (501) staff       (20)       70 2023-07-01 15:15:03.000000 iza-0.0.8/iza.egg-info/entry_points.txt
+-rw-r--r--   0 solst      (501) staff       (20)        1 2023-06-24 20:04:21.000000 iza-0.0.8/iza.egg-info/not-zip-safe
+-rw-r--r--   0 solst      (501) staff       (20)       86 2023-07-01 15:15:03.000000 iza-0.0.8/iza.egg-info/requires.txt
+-rw-r--r--   0 solst      (501) staff       (20)        4 2023-07-01 15:15:03.000000 iza-0.0.8/iza.egg-info/top_level.txt
+-rw-r--r--   0 solst      (501) staff       (20)      911 2023-07-01 15:14:43.000000 iza-0.0.8/settings.ini
+-rw-r--r--   0 solst      (501) staff       (20)       38 2023-07-01 15:15:03.479441 iza-0.0.8/setup.cfg
+-rw-rw-r--   0 solst      (501) staff       (20)     2596 2023-06-27 21:50:00.000000 iza-0.0.8/setup.py
```

### Comparing `iza-0.0.7/LICENSE` & `iza-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `iza-0.0.7/PKG-INFO` & `iza-0.0.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iza
-Version: 0.0.7
+Version: 0.0.8
 Summary: chaos package of utilities; a nod to izalith
 Home-page: https://github.com/dsm-72/iza
 Author: dsm-72
 Author-email: sumner.magruder@yale.edu
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
@@ -62,14 +62,15 @@
 
 ``` sh
 # publish to pypi
 $ nbdev_pypi
 
 # publish to conda
 $ nbdev_conda --build_args '-c conda-forge'
+$ nbdev_conda --mambabuild --build_args '-c conda-forge -c dsm-72'
 ```
 
 # Usage
 
 ## Installation
 
 Install latest from the GitHub
```

### Comparing `iza-0.0.7/README.md` & `iza-0.0.8/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -43,14 +43,15 @@
 
 ``` sh
 # publish to pypi
 $ nbdev_pypi
 
 # publish to conda
 $ nbdev_conda --build_args '-c conda-forge'
+$ nbdev_conda --mambabuild --build_args '-c conda-forge -c dsm-72'
 ```
 
 # Usage
 
 ## Installation
 
 Install latest from the GitHub
```

### Comparing `iza-0.0.7/iza/_modidx.py` & `iza-0.0.8/iza/_modidx.py`

 * *Files identical despite different names*

### Comparing `iza-0.0.7/iza/commands.py` & `iza-0.0.8/iza/commands.py`

 * *Files identical despite different names*

### Comparing `iza-0.0.7/iza/imp.py` & `iza-0.0.8/iza/imp.py`

 * *Files identical despite different names*

### Comparing `iza-0.0.7/iza/nbs.py` & `iza-0.0.8/iza/nbs.py`

 * *Files identical despite different names*

### Comparing `iza-0.0.7/iza/plots.py` & `iza-0.0.8/iza/plots.py`

 * *Files identical despite different names*

### Comparing `iza-0.0.7/iza/static.py` & `iza-0.0.8/iza/static.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/01_static.ipynb.
 
 # %% auto 0
 __all__ = ['NBKS_DIR', 'ROOT_DIR', 'EXPL_DIR', 'DATA_DIR', 'RESULTS_DIR', 'FIGURES_DIR', 'IZALITH_DATA_DIR', 'GIBBS_DATA_DIR',
-           'PERIOD', 'GZ', 'H5', 'CSV', 'MTX', 'TAR', 'TSV', 'PY', 'NPY', 'NPZ', 'TXT', 'JSON', 'ZIP', 'IPYNB',
-           'EXT_GZ', 'EXT_H5', 'EXT_CSV', 'EXT_MTX', 'EXT_TAR', 'EXT_TSV', 'EXT_TAR_GZ', 'EXT_PY', 'EXT_NPY', 'EXT_NPZ',
-           'EXT_TXT', 'EXT_JSON', 'EXT_ZIP', 'EXT_IPYNB', 'SEED', 'ITEM', 'TIME', 'LABEL', 'SERIES', 'SAMPLE',
-           'SAMPLES', 'CONDITION', 'CONDITIONS', 'HVG', 'PCA', 'UMAP', 'TSNE', 'PHATE', 'MAGIC', 'CELL', 'BARCODE',
-           'BARCODES', 'ID', 'MITO', 'RIBO', 'GENE', 'GENE_ID', 'GENE_IDS', 'GENE_SYMBOL', 'HIGHLY_VARIABLE', 'ENSEMBL',
-           'ENSEMBL_ID', 'HUMAN', 'MOUSE', 'HUMAN_TF', 'MOUSE_TF', 'HUMAN_GENE_SYMBOL', 'HUMAN_ENSEMBLE_ID',
-           'MOUSE_ENSEMBLE_ID', 'BATCH', 'TIMEPOINT', 'TOTAL_COUNTS', 'DOUBLET', 'DOUBLET_SCORES', 'PREDICTED_DOUBLETS',
-           'PRENORM', 'DETECTED', 'SCALED_NORMALIZED', 'COUNTS', 'PCT', 'PERCENT', 'PCT_COUNTS', 'PCT_COUNTS_MITO',
-           'PCT_COUNTS_RIBO', 'X', 'X_', 'X_PRENORM', 'X_DETECTED', 'X_SCALED_NORMALIZED', 'X_MAGIC', 'X_PCA',
-           'X_PCA_HVG', 'X_PHATE', 'X_PHATE_HVG', 'ADATA', 'MATRIX', 'FEATURES', 'SENSITIVITY',
-           'AMAZON_BUCKET_FLUENTBIO', 'LINEAGE_ESC', 'LINEAGE_PREGERM', 'LINEAGE_NEURAL_CREST', 'LINEAGE_NEURAL_PROG',
-           'LINEAGE_ENDO', 'LINEAGE_MESO', 'LINEAGE_CARDIAC', 'LINEAGE_HEMA', 'LINEAGE_SOMITES', 'LINEAGE_TROPHOBLAST',
-           'LINEAGE_ALL', 'LINEAGE_NAMES', 'MARKERS_ESC', 'MARKERS_PREGERM', 'MARKERS_NEURAL_CREST',
-           'MARKERS_NEURAL_PROG', 'MARKERS_ENDO', 'MARKERS_MESO', 'MARKERS_CARDIAC', 'MARKERS_HEMA', 'MARKERS_SOMITES',
-           'MARKERS_TROPHOBLAST', 'MARKERS_LISTS', 'MARKERS_ALL', 'LINEAGE_MARKERS', 'RC_PARAMS']
+           'PERIOD', 'GZ', 'H5', 'PT', 'PY', 'BED', 'CSV', 'MTX', 'TAR', 'TSV', 'NPY', 'NPZ', 'TXT', 'PIP', 'PTH',
+           'ZIP', 'JSON', 'H5AD', 'IPYNB', 'ARROW', 'FASTA', 'PARQUET', 'EXT_GZ', 'EXT_H5', 'EXT_PT', 'EXT_PY',
+           'EXT_BED', 'EXT_CSV', 'EXT_MTX', 'EXT_TAR', 'EXT_TSV', 'EXT_NPY', 'EXT_NPZ', 'EXT_TXT', 'EXT_PIP', 'EXT_PTH',
+           'EXT_ZIP', 'EXT_JSON', 'EXT_H5AD', 'EXT_IPYNB', 'EXT_ARROW', 'EXT_FASTA', 'EXT_PARQUET', 'EXT_TAR_GZ',
+           'SEED', 'ITEM', 'TIME', 'LABEL', 'SERIES', 'SAMPLE', 'SAMPLES', 'CONDITION', 'CONDITIONS', 'HVG', 'PCA',
+           'UMAP', 'TSNE', 'PHATE', 'MAGIC', 'CELL', 'CELLS', 'BARCODE', 'BARCODES', 'ID', 'MITO', 'RIBO', 'GENE',
+           'GENE_ID', 'GENE_IDS', 'GENE_SYMBOL', 'HIGHLY_VARIABLE', 'ENSEMBL', 'ENSEMBL_ID', 'HUMAN', 'MOUSE',
+           'HUMAN_TF', 'MOUSE_TF', 'HUMAN_GENE_SYMBOL', 'HUMAN_ENSEMBLE_ID', 'MOUSE_ENSEMBLE_ID', 'BATCH', 'TIMEPOINT',
+           'TIMEPOINTS', 'TOTAL_COUNTS', 'DOUBLET', 'DOUBLET_SCORES', 'PREDICTED_DOUBLETS', 'PRENORM', 'DETECTED',
+           'SCALED_NORMALIZED', 'COUNTS', 'PCT', 'PERCENT', 'PCT_COUNTS', 'PCT_COUNTS_MITO', 'PCT_COUNTS_RIBO', 'X',
+           'X_', 'X_PRENORM', 'X_DETECTED', 'X_SCALED_NORMALIZED', 'X_MAGIC', 'X_PCA', 'X_PCA_HVG', 'X_PHATE',
+           'X_PHATE_HVG', 'ADATA', 'MATRIX', 'FEATURES', 'SENSITIVITY', 'AMAZON_BUCKET_FLUENTBIO', 'LINEAGE_ESC',
+           'LINEAGE_PREGERM', 'LINEAGE_NEURAL_CREST', 'LINEAGE_NEURAL_PROG', 'LINEAGE_ENDO', 'LINEAGE_MESO',
+           'LINEAGE_CARDIAC', 'LINEAGE_HEMA', 'LINEAGE_SOMITES', 'LINEAGE_TROPHOBLAST', 'LINEAGE_ALL', 'LINEAGE_NAMES',
+           'MARKERS_ESC', 'MARKERS_PREGERM', 'MARKERS_NEURAL_CREST', 'MARKERS_NEURAL_PROG', 'MARKERS_ENDO',
+           'MARKERS_MESO', 'MARKERS_CARDIAC', 'MARKERS_HEMA', 'MARKERS_SOMITES', 'MARKERS_TROPHOBLAST', 'MARKERS_LISTS',
+           'MARKERS_ALL', 'LINEAGE_MARKERS', 'RC_PARAMS', 'SEQRUN', 'SEQRUNS', 'TREATMENT', 'TREATMENTS', 'SENS',
+           'SENSITIVITIES']
 
 # %% ../nbs/01_static.ipynb 5
 import os, sys, pkg_resources
 
 # %% ../nbs/01_static.ipynb 6
 '''----------------------------------------------------
 NOTE: RELATIVE DEFINITIONS
@@ -50,68 +53,94 @@
 
 # %% ../nbs/01_static.ipynb 9
 PERIOD = '.'
 
 # %% ../nbs/01_static.ipynb 10
 GZ = f'gz'
 H5 = f'h5'
+PT = f'pt'
+PY = f'py'
+
+BED = f'bed'
 CSV = f'csv'
 MTX = f'mtx'
 TAR = f'tar'
 TSV = f'tsv'
-PY = f'py'
 NPY = f'npy'
 NPZ = f'npz'
 TXT = f'txt'
-JSON = f'json'
+PIP = f'pip'
+PTH = f'pth'
 ZIP = f'zip'
+
+JSON = f'json'
+H5AD = f'h5ad'
 IPYNB = f'ipynb'
 
+ARROW = 'arrow'
+FASTA = 'fasta'
+PARQUET = 'parquet'
+
+
 # %% ../nbs/01_static.ipynb 11
 EXT_GZ = f'{PERIOD}{GZ}'
 EXT_H5 = f'{PERIOD}{H5}'
+EXT_PT = f'{PERIOD}{PT}'
+EXT_PY = f'{PERIOD}{PY}'
+
+EXT_BED = f'{PERIOD}{BED}'
 EXT_CSV = f'{PERIOD}{CSV}'
 EXT_MTX = f'{PERIOD}{MTX}'
 EXT_TAR = f'{PERIOD}{TAR}'
 EXT_TSV = f'{PERIOD}{TSV}'
-EXT_TAR_GZ = f'{EXT_TAR}{EXT_GZ}'
-EXT_PY = f'{PERIOD}{PY}'
 EXT_NPY = f'{PERIOD}{NPY}'
 EXT_NPZ = f'{PERIOD}{NPZ}'
 EXT_TXT = f'{PERIOD}{TXT}'
-EXT_JSON = f'{PERIOD}{JSON}'
+EXT_PIP = f'{PERIOD}{PIP}'
+EXT_PTH = f'{PERIOD}{PTH}'
 EXT_ZIP = f'{PERIOD}{ZIP}'
+
+EXT_JSON = f'{PERIOD}{JSON}'
+EXT_H5AD = f'{PERIOD}{H5AD}'
 EXT_IPYNB = f'{PERIOD}{IPYNB}'
 
+EXT_ARROW = f'{PERIOD}{ARROW}'
+EXT_FASTA = f'{PERIOD}{FASTA}'
+
+EXT_PARQUET = f'{PERIOD}{PARQUET}'
+
+EXT_TAR_GZ = f'{EXT_TAR}{EXT_GZ}'
+
 # %% ../nbs/01_static.ipynb 15
 SEED = 'seed'
 ITEM = 'item'
 TIME = 'time'
 LABEL = 'label'
 SERIES = 'series'
 SAMPLE = 'sample'
 SAMPLES = 'samples'
 CONDITION = 'condition'
 CONDITIONS = f'{CONDITION}s'
 
-# %% ../nbs/01_static.ipynb 19
+# %% ../nbs/01_static.ipynb 21
 HVG = 'hvg'
 
 PCA = 'pca'
 UMAP = 'umap'
 TSNE = 'tsne'
 PHATE = 'phate'
 MAGIC = 'magic'
 
-# %% ../nbs/01_static.ipynb 21
+# %% ../nbs/01_static.ipynb 23
 CELL = 'cell'
+CELLS = f'{CELL}s'
 BARCODE = 'barcode'
 BARCODES = f'{BARCODE}s'
 
-# %% ../nbs/01_static.ipynb 23
+# %% ../nbs/01_static.ipynb 25
 ID = 'id'
 MITO = 'mito'
 RIBO = 'ribo'
 GENE = 'gene'
 GENE_ID = f'{GENE}_id'
 GENE_IDS = f'{GENE_ID}s'
 GENE_SYMBOL = f'{GENE}_symbol'
@@ -128,14 +157,15 @@
 
 HUMAN_GENE_SYMBOL = f'{HUMAN}GeneSymbol'
 HUMAN_ENSEMBLE_ID = f'{HUMAN}EnsemblID'
 MOUSE_ENSEMBLE_ID = f'{MOUSE}EnsemblID'
 
 BATCH = 'batch'
 TIMEPOINT = 'timepoint'
+TIMEPOINTS = f'{TIMEPOINT}s'
 TOTAL_COUNTS = 'total_counts'
 DOUBLET = 'doublet'
 DOUBLET_SCORES = f'{DOUBLET}_scores'
 PREDICTED_DOUBLETS = f'predicted_{DOUBLET}s'
 
 PRENORM = 'prenorm'
 DETECTED = 'detected'
@@ -145,20 +175,20 @@
 COUNTS = 'counts'
 PCT = 'pct'
 PERCENT = 'percent'
 PCT_COUNTS = f'{PCT}_{COUNTS}'
 PCT_COUNTS_MITO = f'{PCT}_{COUNTS}_{MITO}'
 PCT_COUNTS_RIBO = f'{PCT}_{COUNTS}_{RIBO}'
 
-# %% ../nbs/01_static.ipynb 24
+# %% ../nbs/01_static.ipynb 26
 _ = '_'
 X = 'X'
 X_ = f'{X}{_}'
 
-# %% ../nbs/01_static.ipynb 25
+# %% ../nbs/01_static.ipynb 27
 # Layer storing prenormalized counts in adata.layers
 X_PRENORM = f'{X_}{PRENORM}'
 
 # Layer storing values where prenormalized counts is at least 0 in adata.layers
 X_DETECTED = f'{X_}{DETECTED}'
 
 # Layer storing counts normalized
@@ -175,73 +205,73 @@
 
 # Layer storing PHATE embedding just in adata.obsm
 X_PHATE = f'{X_}{PHATE}'
 
 # Layer storing PHATE embedding just on HVGs in adata.obsm
 X_PHATE_HVG = f'{X_}{PHATE}_{HVG}'
 
-# %% ../nbs/01_static.ipynb 27
+# %% ../nbs/01_static.ipynb 29
 ADATA = 'adata'
 MATRIX = 'matrix'
 FEATURES = 'features'
 SENSITIVITY = 'sensitivity'
 
-# %% ../nbs/01_static.ipynb 29
+# %% ../nbs/01_static.ipynb 31
 AMAZON_BUCKET_FLUENTBIO = 'https://fbs-public.s3.us-east-2.amazonaws.com'
 
-# %% ../nbs/01_static.ipynb 31
+# %% ../nbs/01_static.ipynb 33
 import itertools
 
-# %% ../nbs/01_static.ipynb 33
+# %% ../nbs/01_static.ipynb 35
 LINEAGE_ESC = 'esc'
 LINEAGE_PREGERM = 'pregerm'
 LINEAGE_NEURAL_CREST = 'neural_crest'
 LINEAGE_NEURAL_PROG = 'neural_prog'
 LINEAGE_ENDO = 'endo'
 LINEAGE_MESO = 'meso'
 LINEAGE_CARDIAC = 'cardiac'
 LINEAGE_HEMA = 'hema'
 LINEAGE_SOMITES = 'somites'
 LINEAGE_TROPHOBLAST = 'trophblast'
 LINEAGE_ALL = 'all'
 
-# %% ../nbs/01_static.ipynb 34
+# %% ../nbs/01_static.ipynb 36
 LINEAGE_NAMES = [
     LINEAGE_ESC, LINEAGE_PREGERM, LINEAGE_NEURAL_CREST,
     LINEAGE_NEURAL_PROG, LINEAGE_ENDO, LINEAGE_MESO,
     LINEAGE_CARDIAC, LINEAGE_HEMA, LINEAGE_SOMITES,
     LINEAGE_TROPHOBLAST, LINEAGE_ALL
 ]
 
-# %% ../nbs/01_static.ipynb 36
+# %% ../nbs/01_static.ipynb 38
 MARKERS_ESC = ['POU5F1', 'PRDM14', 'NANOG', 'SOX2', 'DPPA4', 'NR2F6', 'OTX2']
 MARKERS_PREGERM = ['TP53','NR6A1','GBX2','ZIC2','ZIC5']
 MARKERS_NEURAL_CREST = ['PAX3','FOXD3','ITGA4','EDNRB','SOX9','SOX10']
 MARKERS_NEURAL_PROG = ['NES','MAP2','PAX6','SOX1','ZBTB16','ONECUT1', 'ONECUT2','NR2F1','ISL1','NPAS1','EN2','SOX2','NEUROD1']
 MARKERS_ENDO = ['EOMES','FOXA2','SOX17','GATA4','GATA6','HHEX']
 MARKERS_MESO = ['MIXL1','CER1']
 MARKERS_CARDIAC = ['NKX2-5','GATA4','MYBPC2','TTN','TNNT2','MYH6','TBX5']
 MARKERS_HEMA = ['NKX2-5','TAL1','SOX17','CD34','PECAM1','CD69','CXCR4','CDH5','KDR','LMO2']
 MARKERS_SOMITES = ['WT1','TBX18','TBX15','PDGFRA','SIX2','TBX5']
 MARKERS_TROPHOBLAST = ['GATA3','TP63','ITGA6','CDH1']
 
-# %% ../nbs/01_static.ipynb 37
+# %% ../nbs/01_static.ipynb 39
 MARKERS_LISTS =  [
     MARKERS_ESC, MARKERS_PREGERM, MARKERS_NEURAL_CREST,
     MARKERS_NEURAL_PROG, MARKERS_ENDO, MARKERS_MESO, 
     MARKERS_CARDIAC, MARKERS_HEMA, MARKERS_SOMITES, 
     MARKERS_TROPHOBLAST,
 ]
 MARKERS_ALL = list(itertools.chain(*MARKERS_LISTS))
 MARKERS_LISTS.append(MARKERS_ALL)
 
-# %% ../nbs/01_static.ipynb 39
+# %% ../nbs/01_static.ipynb 41
 LINEAGE_MARKERS = dict(zip(LINEAGE_NAMES, MARKERS_LISTS))
 
-# %% ../nbs/01_static.ipynb 42
+# %% ../nbs/01_static.ipynb 44
 RC_PARAMS = {
     'axes.axisbelow': False,
     'axes.edgecolor': 'lightgrey',
     'axes.facecolor': 'None',
     'axes.grid': False,
     'axes.labelcolor': 'dimgrey',
     'axes.spines.right': False,
@@ -259,7 +289,16 @@
     'ytick.direction': 'out',
     'ytick.left': False,
     'ytick.right': False,
     'font.size': 12,
     'axes.titlesize': 10,
     'axes.labelsize': 12
 }
+
+# %% ../nbs/01_static.ipynb 48
+SEQRUN = 'seqrun'
+SEQRUNS = f'{SEQRUN}s'
+TREATMENT = f'treatment'
+TREATMENTS = f'{TREATMENT}s'
+
+SENS = 'sens'
+SENSITIVITIES = 'sensitivities'
```

### Comparing `iza-0.0.7/iza/types.py` & `iza-0.0.8/iza/types.py`

 * *Files identical despite different names*

### Comparing `iza-0.0.7/iza/utils.py` & `iza-0.0.8/iza/utils.py`

 * *Files identical despite different names*

### Comparing `iza-0.0.7/iza.egg-info/PKG-INFO` & `iza-0.0.8/iza.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iza
-Version: 0.0.7
+Version: 0.0.8
 Summary: chaos package of utilities; a nod to izalith
 Home-page: https://github.com/dsm-72/iza
 Author: dsm-72
 Author-email: sumner.magruder@yale.edu
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
@@ -62,14 +62,15 @@
 
 ``` sh
 # publish to pypi
 $ nbdev_pypi
 
 # publish to conda
 $ nbdev_conda --build_args '-c conda-forge'
+$ nbdev_conda --mambabuild --build_args '-c conda-forge -c dsm-72'
 ```
 
 # Usage
 
 ## Installation
 
 Install latest from the GitHub
```

### Comparing `iza-0.0.7/settings.ini` & `iza-0.0.8/settings.ini`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = iza
 lib_name = iza
-version = 0.0.7
+version = 0.0.8
 min_python = 3.10
 license = apache2
 black_formatting = False
 doc_path = _docs
 lib_path = iza
 nbs_path = nbs
 recursive = True
@@ -30,9 +30,9 @@
 console_scripts = iza=iza.commands:app
 readme_nb = index.ipynb
 allowed_metadata_keys = 
 allowed_cell_metadata_keys = 
 jupyter_hooks = True
 clean_ids = True
 clear_all = False
-requirements = pandas seaborn scikit-learn numpy nbformat rich typer requests tqdm ipos
+requirements = pandas seaborn scikit-learn numpy>=1.22 nbformat rich typer requests tqdm ipos
```

### Comparing `iza-0.0.7/setup.py` & `iza-0.0.8/setup.py`

 * *Files identical despite different names*

