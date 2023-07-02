# Comparing `tmp/GMM_Demux-0.2.2.0.tar.gz` & `tmp/GMM_Demux-0.2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/GMM_Demux-0.2.2.0.tar", last modified: Tue Jun 27 16:22:04 2023, max compression
+gzip compressed data, was "dist/GMM_Demux-0.2.2.1.tar", last modified: Sun Jul  2 14:45:24 2023, max compression
```

## Comparing `GMM_Demux-0.2.2.0.tar` & `GMM_Demux-0.2.2.1.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 hxin      (1000) hxin      (1000)        0 2023-06-27 16:22:04.502512 GMM_Demux-0.2.2.0/
-drwxr-xr-x   0 hxin      (1000) hxin      (1000)        0 2023-06-27 16:22:04.442159 GMM_Demux-0.2.2.0/GMM_Demux/
--rw-r--r--   0 hxin      (1000) hxin      (1000)    13604 2023-06-27 16:20:06.000000 GMM_Demux-0.2.2.0/GMM_Demux/GMM_Demux.py
--rw-rw-rw-   0 hxin      (1000) hxin      (1000)     2243 2020-08-05 11:03:41.000000 GMM_Demux-0.2.2.0/GMM_Demux/GMM_IO.py
--rw-rw-rw-   0 hxin      (1000) hxin      (1000)        0 2020-08-05 11:03:41.000000 GMM_Demux-0.2.2.0/GMM_Demux/__init__.py
--rw-rw-rw-   0 hxin      (1000) hxin      (1000)     1084 2020-08-05 11:03:41.000000 GMM_Demux-0.2.2.0/GMM_Demux/check_multi_comp.py
--rw-r--r--   0 hxin      (1000) hxin      (1000)     7166 2023-06-27 16:20:06.000000 GMM_Demux-0.2.2.0/GMM_Demux/classify_drops.py
--rw-rw-rw-   0 hxin      (1000) hxin      (1000)     7544 2020-08-05 11:03:41.000000 GMM_Demux-0.2.2.0/GMM_Demux/compute_venn.py
--rw-rw-rw-   0 hxin      (1000) hxin      (1000)     9214 2020-08-05 11:03:41.000000 GMM_Demux-0.2.2.0/GMM_Demux/estimator.py
-drwxr-xr-x   0 hxin      (1000) hxin      (1000)        0 2023-06-27 16:22:04.466183 GMM_Demux-0.2.2.0/GMM_Demux.egg-info/
--rw-r--r--   0 hxin      (1000) hxin      (1000)    12896 2023-06-27 16:22:03.000000 GMM_Demux-0.2.2.0/GMM_Demux.egg-info/PKG-INFO
--rw-r--r--   0 hxin      (1000) hxin      (1000)     1439 2023-06-27 16:22:04.000000 GMM_Demux-0.2.2.0/GMM_Demux.egg-info/SOURCES.txt
--rw-r--r--   0 hxin      (1000) hxin      (1000)        1 2023-06-27 16:22:03.000000 GMM_Demux-0.2.2.0/GMM_Demux.egg-info/dependency_links.txt
--rw-r--r--   0 hxin      (1000) hxin      (1000)       55 2023-06-27 16:22:03.000000 GMM_Demux-0.2.2.0/GMM_Demux.egg-info/entry_points.txt
--rw-r--r--   0 hxin      (1000) hxin      (1000)       81 2023-06-27 16:22:04.000000 GMM_Demux-0.2.2.0/GMM_Demux.egg-info/requires.txt
--rw-r--r--   0 hxin      (1000) hxin      (1000)       10 2023-06-27 16:22:04.000000 GMM_Demux-0.2.2.0/GMM_Demux.egg-info/top_level.txt
--rw-rw-rw-   0 hxin      (1000) hxin      (1000)  1009859 2020-08-05 11:03:41.000000 GMM_Demux-0.2.2.0/GMM_simplified.png
--rw-rw-rw-   0 hxin      (1000) hxin      (1000)     1072 2020-08-05 11:03:41.000000 GMM_Demux-0.2.2.0/LICENSE
--rw-r--r--   0 hxin      (1000) hxin      (1000)    12896 2023-06-27 16:22:04.498525 GMM_Demux-0.2.2.0/PKG-INFO
--rw-rw-rw-   0 hxin      (1000) hxin      (1000)    12436 2020-08-05 11:03:41.000000 GMM_Demux-0.2.2.0/README.md
--rw-rw-rw-   0 hxin      (1000) hxin      (1000)    12053 2020-08-05 11:03:41.000000 GMM_Demux-0.2.2.0/class_output.png
-drwxr-xr-x   0 hxin      (1000) hxin      (1000)        0 2023-06-27 16:22:04.478833 GMM_Demux-0.2.2.0/example_cell_types/
--rw-rw-rw-   0 hxin      (1000) hxin      (1000)     3382 2020-08-05 11:03:41.000000 GMM_Demux-0.2.2.0/example_cell_types/CD11+CD14-CD16-.txt
--rw-rw-rw-   0 hxin      (1000) hxin      (1000)     5225 2020-08-05 11:03:41.000000 GMM_Demux-0.2.2.0/example_cell_types/CD14+CD16+.txt
--rw-rw-rw-   0 hxin      (1000) hxin      (1000)    37449 2020-08-05 11:03:41.000000 GMM_Demux-0.2.2.0/example_cell_types/CD14+CD16-.txt
--rw-rw-rw-   0 hxin      (1000) hxin      (1000)     7923 2020-08-05 11:03:41.000000 GMM_Demux-0.2.2.0/example_cell_types/CD19+.txt
--rw-rw-rw-   0 hxin      (1000) hxin      (1000)   183445 2020-08-05 11:03:41.000000 GMM_Demux-0.2.2.0/example_cell_types/CD3+.txt
--rw-rw-rw-   0 hxin      (1000) hxin      (1000)   110238 2020-08-05 11:03:41.000000 GMM_Demux-0.2.2.0/example_cell_types/CD3+CD4+.txt
--rw-rw-rw-   0 hxin      (1000) hxin      (1000)    37316 2020-08-05 11:03:41.000000 GMM_Demux-0.2.2.0/example_cell_types/CD3+CD8+.txt
--rw-rw-rw-   0 hxin      (1000) hxin      (1000)    24491 2020-08-05 11:03:41.000000 GMM_Demux-0.2.2.0/example_cell_types/CD56+CD16+.txt
--rw-rw-rw-   0 hxin      (1000) hxin      (1000)     2451 2020-08-05 11:03:41.000000 GMM_Demux-0.2.2.0/example_cell_types/CD56+CD16-.txt
-drwxr-xr-x   0 hxin      (1000) hxin      (1000)        0 2023-06-27 16:22:04.494516 GMM_Demux-0.2.2.0/example_cell_types/Doublets/
--rw-rw-rw-   0 hxin      (1000) hxin      (1000)     1216 2020-08-05 11:03:41.000000 GMM_Demux-0.2.2.0/example_cell_types/Doublets/CD14+CD56+.txt
--rw-rw-rw-   0 hxin      (1000) hxin      (1000)     8550 2020-08-05 11:03:41.000000 GMM_Demux-0.2.2.0/example_cell_types/Doublets/CD3+CD4+CD14+.txt
--rw-rw-rw-   0 hxin      (1000) hxin      (1000)      247 2020-08-05 11:03:41.000000 GMM_Demux-0.2.2.0/example_cell_types/Doublets/CD3+CD4+CD14+CD56+.txt
--rw-rw-rw-   0 hxin      (1000) hxin      (1000)     1976 2020-08-05 11:03:41.000000 GMM_Demux-0.2.2.0/example_cell_types/Doublets/CD3+CD4+CD19+.txt
--rw-rw-rw-   0 hxin      (1000) hxin      (1000)     5282 2020-08-05 11:03:41.000000 GMM_Demux-0.2.2.0/example_cell_types/Doublets/CD3+CD4+CD56+.txt
--rw-rw-rw-   0 hxin      (1000) hxin      (1000)     8702 2020-08-05 11:03:41.000000 GMM_Demux-0.2.2.0/example_cell_types/Doublets/CD3+CD4+CD8+.txt
--rw-rw-rw-   0 hxin      (1000) hxin      (1000)     2698 2020-08-05 11:03:41.000000 GMM_Demux-0.2.2.0/example_cell_types/Doublets/CD3+CD8+CD14+.txt
--rw-rw-rw-   0 hxin      (1000) hxin      (1000)      798 2020-08-05 11:03:41.000000 GMM_Demux-0.2.2.0/example_cell_types/Doublets/CD3+CD8+CD19+.txt
--rw-rw-rw-   0 hxin      (1000) hxin      (1000)     1007 2020-08-05 11:03:41.000000 GMM_Demux-0.2.2.0/example_cell_types/Doublets/CD3+CD8+CD56+.txt
--rw-rw-rw-   0 hxin      (1000) hxin      (1000)   517818 2020-08-05 11:03:41.000000 GMM_Demux-0.2.2.0/example_hto.csv
-drwxr-xr-x   0 hxin      (1000) hxin      (1000)        0 2023-06-27 16:22:04.412660 GMM_Demux-0.2.2.0/example_input/
-drwxr-xr-x   0 hxin      (1000) hxin      (1000)        0 2023-06-27 16:22:04.412660 GMM_Demux-0.2.2.0/example_input/outs/
-drwxr-xr-x   0 hxin      (1000) hxin      (1000)        0 2023-06-27 16:22:04.498525 GMM_Demux-0.2.2.0/example_input/outs/filtered_feature_bc_matrix/
--rw-rw-rw-   0 hxin      (1000) hxin      (1000)    60384 2020-08-05 11:03:41.000000 GMM_Demux-0.2.2.0/example_input/outs/filtered_feature_bc_matrix/barcodes.tsv.gz
--rw-rw-rw-   0 hxin      (1000) hxin      (1000)       80 2020-08-05 11:03:41.000000 GMM_Demux-0.2.2.0/example_input/outs/filtered_feature_bc_matrix/features.tsv.gz
--rw-rw-rw-   0 hxin      (1000) hxin      (1000)   237570 2020-08-05 11:03:41.000000 GMM_Demux-0.2.2.0/example_input/outs/filtered_feature_bc_matrix/matrix.mtx.gz
--rw-rw-rw-   0 hxin      (1000) hxin      (1000)     6489 2020-08-05 11:03:41.000000 GMM_Demux-0.2.2.0/features.png
--rw-rw-rw-   0 hxin      (1000) hxin      (1000)  1785236 2020-08-05 11:03:41.000000 GMM_Demux-0.2.2.0/path.png
--rw-rw-rw-   0 hxin      (1000) hxin      (1000)   453771 2020-08-05 11:03:41.000000 GMM_Demux-0.2.2.0/phony.png
--rw-rw-rw-   0 hxin      (1000) hxin      (1000)    65191 2020-08-05 11:03:41.000000 GMM_Demux-0.2.2.0/phony_type.png
--rw-rw-rw-   0 hxin      (1000) hxin      (1000)   105559 2020-08-05 11:03:41.000000 GMM_Demux-0.2.2.0/planner.png
--rw-rw-rw-   0 hxin      (1000) hxin      (1000)    63771 2020-08-05 11:03:41.000000 GMM_Demux-0.2.2.0/pure_type.png
--rw-r--r--   0 hxin      (1000) hxin      (1000)       38 2023-06-27 16:22:04.502512 GMM_Demux-0.2.2.0/setup.cfg
--rw-r--r--   0 hxin      (1000) hxin      (1000)      989 2023-06-27 16:20:35.000000 GMM_Demux-0.2.2.0/setup.py
--rw-rw-rw-   0 hxin      (1000) hxin      (1000)    24413 2020-08-05 11:03:41.000000 GMM_Demux-0.2.2.0/summary.png
--rw-rw-rw-   0 hxin      (1000) hxin      (1000)   212591 2020-08-05 11:03:41.000000 GMM_Demux-0.2.2.0/term.png
+drwxr-xr-x   0 hxin      (1000) hxin      (1000)        0 2023-07-02 14:45:24.943363 GMM_Demux-0.2.2.1/
+drwxr-xr-x   0 hxin      (1000) hxin      (1000)        0 2023-07-02 14:45:24.418315 GMM_Demux-0.2.2.1/GMM_Demux/
+-rw-r--r--   0 hxin      (1000) hxin      (1000)    13604 2023-06-27 16:20:06.000000 GMM_Demux-0.2.2.1/GMM_Demux/GMM_Demux.py
+-rw-rw-rw-   0 hxin      (1000) hxin      (1000)     2243 2020-08-05 11:03:41.000000 GMM_Demux-0.2.2.1/GMM_Demux/GMM_IO.py
+-rw-rw-rw-   0 hxin      (1000) hxin      (1000)        0 2020-08-05 11:03:41.000000 GMM_Demux-0.2.2.1/GMM_Demux/__init__.py
+-rw-rw-rw-   0 hxin      (1000) hxin      (1000)     1084 2020-08-05 11:03:41.000000 GMM_Demux-0.2.2.1/GMM_Demux/check_multi_comp.py
+-rw-r--r--   0 hxin      (1000) hxin      (1000)     6720 2023-07-02 14:24:19.000000 GMM_Demux-0.2.2.1/GMM_Demux/classify_drops.py
+-rw-rw-rw-   0 hxin      (1000) hxin      (1000)     7544 2020-08-05 11:03:41.000000 GMM_Demux-0.2.2.1/GMM_Demux/compute_venn.py
+-rw-rw-rw-   0 hxin      (1000) hxin      (1000)     9214 2020-08-05 11:03:41.000000 GMM_Demux-0.2.2.1/GMM_Demux/estimator.py
+drwxr-xr-x   0 hxin      (1000) hxin      (1000)        0 2023-07-02 14:45:24.513283 GMM_Demux-0.2.2.1/GMM_Demux.egg-info/
+-rw-r--r--   0 hxin      (1000) hxin      (1000)    12896 2023-07-02 14:45:21.000000 GMM_Demux-0.2.2.1/GMM_Demux.egg-info/PKG-INFO
+-rw-r--r--   0 hxin      (1000) hxin      (1000)     1439 2023-07-02 14:45:23.000000 GMM_Demux-0.2.2.1/GMM_Demux.egg-info/SOURCES.txt
+-rw-r--r--   0 hxin      (1000) hxin      (1000)        1 2023-07-02 14:45:21.000000 GMM_Demux-0.2.2.1/GMM_Demux.egg-info/dependency_links.txt
+-rw-r--r--   0 hxin      (1000) hxin      (1000)       55 2023-07-02 14:45:21.000000 GMM_Demux-0.2.2.1/GMM_Demux.egg-info/entry_points.txt
+-rw-r--r--   0 hxin      (1000) hxin      (1000)       81 2023-07-02 14:45:21.000000 GMM_Demux-0.2.2.1/GMM_Demux.egg-info/requires.txt
+-rw-r--r--   0 hxin      (1000) hxin      (1000)       10 2023-07-02 14:45:22.000000 GMM_Demux-0.2.2.1/GMM_Demux.egg-info/top_level.txt
+-rw-rw-rw-   0 hxin      (1000) hxin      (1000)  1009859 2020-08-05 11:03:41.000000 GMM_Demux-0.2.2.1/GMM_simplified.png
+-rw-rw-rw-   0 hxin      (1000) hxin      (1000)     1072 2020-08-05 11:03:41.000000 GMM_Demux-0.2.2.1/LICENSE
+-rw-r--r--   0 hxin      (1000) hxin      (1000)    12896 2023-07-02 14:45:24.943363 GMM_Demux-0.2.2.1/PKG-INFO
+-rw-rw-rw-   0 hxin      (1000) hxin      (1000)    12436 2020-08-05 11:03:41.000000 GMM_Demux-0.2.2.1/README.md
+-rw-rw-rw-   0 hxin      (1000) hxin      (1000)    12053 2020-08-05 11:03:41.000000 GMM_Demux-0.2.2.1/class_output.png
+drwxr-xr-x   0 hxin      (1000) hxin      (1000)        0 2023-07-02 14:45:24.730933 GMM_Demux-0.2.2.1/example_cell_types/
+-rw-rw-rw-   0 hxin      (1000) hxin      (1000)     3382 2020-08-05 11:03:41.000000 GMM_Demux-0.2.2.1/example_cell_types/CD11+CD14-CD16-.txt
+-rw-rw-rw-   0 hxin      (1000) hxin      (1000)     5225 2020-08-05 11:03:41.000000 GMM_Demux-0.2.2.1/example_cell_types/CD14+CD16+.txt
+-rw-rw-rw-   0 hxin      (1000) hxin      (1000)    37449 2020-08-05 11:03:41.000000 GMM_Demux-0.2.2.1/example_cell_types/CD14+CD16-.txt
+-rw-rw-rw-   0 hxin      (1000) hxin      (1000)     7923 2020-08-05 11:03:41.000000 GMM_Demux-0.2.2.1/example_cell_types/CD19+.txt
+-rw-rw-rw-   0 hxin      (1000) hxin      (1000)   183445 2020-08-05 11:03:41.000000 GMM_Demux-0.2.2.1/example_cell_types/CD3+.txt
+-rw-rw-rw-   0 hxin      (1000) hxin      (1000)   110238 2020-08-05 11:03:41.000000 GMM_Demux-0.2.2.1/example_cell_types/CD3+CD4+.txt
+-rw-rw-rw-   0 hxin      (1000) hxin      (1000)    37316 2020-08-05 11:03:41.000000 GMM_Demux-0.2.2.1/example_cell_types/CD3+CD8+.txt
+-rw-rw-rw-   0 hxin      (1000) hxin      (1000)    24491 2020-08-05 11:03:41.000000 GMM_Demux-0.2.2.1/example_cell_types/CD56+CD16+.txt
+-rw-rw-rw-   0 hxin      (1000) hxin      (1000)     2451 2020-08-05 11:03:41.000000 GMM_Demux-0.2.2.1/example_cell_types/CD56+CD16-.txt
+drwxr-xr-x   0 hxin      (1000) hxin      (1000)        0 2023-07-02 14:45:24.927879 GMM_Demux-0.2.2.1/example_cell_types/Doublets/
+-rw-rw-rw-   0 hxin      (1000) hxin      (1000)     1216 2020-08-05 11:03:41.000000 GMM_Demux-0.2.2.1/example_cell_types/Doublets/CD14+CD56+.txt
+-rw-rw-rw-   0 hxin      (1000) hxin      (1000)     8550 2020-08-05 11:03:41.000000 GMM_Demux-0.2.2.1/example_cell_types/Doublets/CD3+CD4+CD14+.txt
+-rw-rw-rw-   0 hxin      (1000) hxin      (1000)      247 2020-08-05 11:03:41.000000 GMM_Demux-0.2.2.1/example_cell_types/Doublets/CD3+CD4+CD14+CD56+.txt
+-rw-rw-rw-   0 hxin      (1000) hxin      (1000)     1976 2020-08-05 11:03:41.000000 GMM_Demux-0.2.2.1/example_cell_types/Doublets/CD3+CD4+CD19+.txt
+-rw-rw-rw-   0 hxin      (1000) hxin      (1000)     5282 2020-08-05 11:03:41.000000 GMM_Demux-0.2.2.1/example_cell_types/Doublets/CD3+CD4+CD56+.txt
+-rw-rw-rw-   0 hxin      (1000) hxin      (1000)     8702 2020-08-05 11:03:41.000000 GMM_Demux-0.2.2.1/example_cell_types/Doublets/CD3+CD4+CD8+.txt
+-rw-rw-rw-   0 hxin      (1000) hxin      (1000)     2698 2020-08-05 11:03:41.000000 GMM_Demux-0.2.2.1/example_cell_types/Doublets/CD3+CD8+CD14+.txt
+-rw-rw-rw-   0 hxin      (1000) hxin      (1000)      798 2020-08-05 11:03:41.000000 GMM_Demux-0.2.2.1/example_cell_types/Doublets/CD3+CD8+CD19+.txt
+-rw-rw-rw-   0 hxin      (1000) hxin      (1000)     1007 2020-08-05 11:03:41.000000 GMM_Demux-0.2.2.1/example_cell_types/Doublets/CD3+CD8+CD56+.txt
+-rw-rw-rw-   0 hxin      (1000) hxin      (1000)   517818 2020-08-05 11:03:41.000000 GMM_Demux-0.2.2.1/example_hto.csv
+drwxr-xr-x   0 hxin      (1000) hxin      (1000)        0 2023-07-02 14:45:23.977133 GMM_Demux-0.2.2.1/example_input/
+drwxr-xr-x   0 hxin      (1000) hxin      (1000)        0 2023-07-02 14:45:23.978609 GMM_Demux-0.2.2.1/example_input/outs/
+drwxr-xr-x   0 hxin      (1000) hxin      (1000)        0 2023-07-02 14:45:24.943363 GMM_Demux-0.2.2.1/example_input/outs/filtered_feature_bc_matrix/
+-rw-rw-rw-   0 hxin      (1000) hxin      (1000)    60384 2020-08-05 11:03:41.000000 GMM_Demux-0.2.2.1/example_input/outs/filtered_feature_bc_matrix/barcodes.tsv.gz
+-rw-rw-rw-   0 hxin      (1000) hxin      (1000)       80 2020-08-05 11:03:41.000000 GMM_Demux-0.2.2.1/example_input/outs/filtered_feature_bc_matrix/features.tsv.gz
+-rw-rw-rw-   0 hxin      (1000) hxin      (1000)   237570 2020-08-05 11:03:41.000000 GMM_Demux-0.2.2.1/example_input/outs/filtered_feature_bc_matrix/matrix.mtx.gz
+-rw-rw-rw-   0 hxin      (1000) hxin      (1000)     6489 2020-08-05 11:03:41.000000 GMM_Demux-0.2.2.1/features.png
+-rw-rw-rw-   0 hxin      (1000) hxin      (1000)  1785236 2020-08-05 11:03:41.000000 GMM_Demux-0.2.2.1/path.png
+-rw-rw-rw-   0 hxin      (1000) hxin      (1000)   453771 2020-08-05 11:03:41.000000 GMM_Demux-0.2.2.1/phony.png
+-rw-rw-rw-   0 hxin      (1000) hxin      (1000)    65191 2020-08-05 11:03:41.000000 GMM_Demux-0.2.2.1/phony_type.png
+-rw-rw-rw-   0 hxin      (1000) hxin      (1000)   105559 2020-08-05 11:03:41.000000 GMM_Demux-0.2.2.1/planner.png
+-rw-rw-rw-   0 hxin      (1000) hxin      (1000)    63771 2020-08-05 11:03:41.000000 GMM_Demux-0.2.2.1/pure_type.png
+-rw-r--r--   0 hxin      (1000) hxin      (1000)       38 2023-07-02 14:45:24.943363 GMM_Demux-0.2.2.1/setup.cfg
+-rw-r--r--   0 hxin      (1000) hxin      (1000)      989 2023-07-02 14:36:46.000000 GMM_Demux-0.2.2.1/setup.py
+-rw-rw-rw-   0 hxin      (1000) hxin      (1000)    24413 2020-08-05 11:03:41.000000 GMM_Demux-0.2.2.1/summary.png
+-rw-rw-rw-   0 hxin      (1000) hxin      (1000)   212591 2020-08-05 11:03:41.000000 GMM_Demux-0.2.2.1/term.png
```

### Comparing `GMM_Demux-0.2.2.0/GMM_Demux/GMM_Demux.py` & `GMM_Demux-0.2.2.1/GMM_Demux/GMM_Demux.py`

 * *Files identical despite different names*

### Comparing `GMM_Demux-0.2.2.0/GMM_Demux/GMM_IO.py` & `GMM_Demux-0.2.2.1/GMM_Demux/GMM_IO.py`

 * *Files identical despite different names*

### Comparing `GMM_Demux-0.2.2.0/GMM_Demux/check_multi_comp.py` & `GMM_Demux-0.2.2.1/GMM_Demux/check_multi_comp.py`

 * *Files identical despite different names*

### Comparing `GMM_Demux-0.2.2.0/GMM_Demux/classify_drops.py` & `GMM_Demux-0.2.2.1/GMM_Demux/classify_drops.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,35 +16,23 @@
     high_array = []
     low_array = []
 
     for i in range(data.shape[1]):
         X = data.iloc[:,i].values[:, np.newaxis]
 
         # GMM values
-<<<<<<< HEAD
         gmm.append(GaussianMixture(2).fit(X))
         # x = np.linspace(-6, 6, 1000)[:, np.newaxis]
         # logprob= gmm[-1].score_samples(x)
         # responsibilities = gmm[-1].predict_proba(x)
         # pdf = np.exp(logprob)
         # pdf_individual = responsibilities * pdf[:, np.newaxis]
         # print(pdf_individual)
         # print(gmm[-1].means_)
         # print(gmm[-1].covariances_)
-=======
-        gmm.append(GaussianMixture(2, random_state = random_seed).fit(X))
-        x = np.linspace(-6, 6, 1000)[:, np.newaxis]
-        logprob= gmm[-1].score_samples(x)
-        responsibilities = gmm[-1].predict_proba(x)
-        pdf = np.exp(logprob)
-        pdf_individual = responsibilities * pdf[:, np.newaxis]
-        #print(pdf_individual)
-
-        #print(gmm[-1].means_)
->>>>>>> fdd6aec963298f6429498db06ad43c000df219c9
 
         # Extract prob
         high_idx = np.argmax(gmm[-1].means_, axis=0)[0]
         post_prob = gmm[-1].predict_proba(X)
 
         high_array.append(post_prob[np.arange(post_prob.shape[0]), np.full(post_prob.shape[0], high_idx)])
```

### Comparing `GMM_Demux-0.2.2.0/GMM_Demux/compute_venn.py` & `GMM_Demux-0.2.2.1/GMM_Demux/compute_venn.py`

 * *Files identical despite different names*

### Comparing `GMM_Demux-0.2.2.0/GMM_Demux/estimator.py` & `GMM_Demux-0.2.2.1/GMM_Demux/estimator.py`

 * *Files identical despite different names*

### Comparing `GMM_Demux-0.2.2.0/GMM_Demux.egg-info/PKG-INFO` & `GMM_Demux-0.2.2.1/GMM_Demux.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GMM-Demux
-Version: 0.2.2.0
+Version: 0.2.2.1
 Summary: A multiplet removal tool for processing cell hashing data
 Home-page: https://github.com/CHPGenetics/GMM-demux
 Author: Hongyi Xin
 Author-email: gohongyi@gmail.com
 Classifier: Programming Language :: Python :: 3.6
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `GMM_Demux-0.2.2.0/GMM_Demux.egg-info/SOURCES.txt` & `GMM_Demux-0.2.2.1/GMM_Demux.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `GMM_Demux-0.2.2.0/GMM_simplified.png` & `GMM_Demux-0.2.2.1/GMM_simplified.png`

 * *Files identical despite different names*

### Comparing `GMM_Demux-0.2.2.0/LICENSE` & `GMM_Demux-0.2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `GMM_Demux-0.2.2.0/PKG-INFO` & `GMM_Demux-0.2.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GMM_Demux
-Version: 0.2.2.0
+Version: 0.2.2.1
 Summary: A multiplet removal tool for processing cell hashing data
 Home-page: https://github.com/CHPGenetics/GMM-demux
 Author: Hongyi Xin
 Author-email: gohongyi@gmail.com
 Classifier: Programming Language :: Python :: 3.6
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `GMM_Demux-0.2.2.0/README.md` & `GMM_Demux-0.2.2.1/README.md`

 * *Files identical despite different names*

### Comparing `GMM_Demux-0.2.2.0/class_output.png` & `GMM_Demux-0.2.2.1/class_output.png`

 * *Files identical despite different names*

### Comparing `GMM_Demux-0.2.2.0/example_cell_types/CD11+CD14-CD16-.txt` & `GMM_Demux-0.2.2.1/example_cell_types/CD11+CD14-CD16-.txt`

 * *Files identical despite different names*

### Comparing `GMM_Demux-0.2.2.0/example_cell_types/CD14+CD16+.txt` & `GMM_Demux-0.2.2.1/example_cell_types/CD14+CD16+.txt`

 * *Files identical despite different names*

### Comparing `GMM_Demux-0.2.2.0/example_cell_types/CD14+CD16-.txt` & `GMM_Demux-0.2.2.1/example_cell_types/CD14+CD16-.txt`

 * *Files identical despite different names*

### Comparing `GMM_Demux-0.2.2.0/example_cell_types/CD19+.txt` & `GMM_Demux-0.2.2.1/example_cell_types/CD19+.txt`

 * *Files identical despite different names*

### Comparing `GMM_Demux-0.2.2.0/example_cell_types/CD3+.txt` & `GMM_Demux-0.2.2.1/example_cell_types/CD3+.txt`

 * *Files identical despite different names*

### Comparing `GMM_Demux-0.2.2.0/example_cell_types/CD3+CD4+.txt` & `GMM_Demux-0.2.2.1/example_cell_types/CD3+CD4+.txt`

 * *Files identical despite different names*

### Comparing `GMM_Demux-0.2.2.0/example_cell_types/CD3+CD8+.txt` & `GMM_Demux-0.2.2.1/example_cell_types/CD3+CD8+.txt`

 * *Files identical despite different names*

### Comparing `GMM_Demux-0.2.2.0/example_cell_types/CD56+CD16+.txt` & `GMM_Demux-0.2.2.1/example_cell_types/CD56+CD16+.txt`

 * *Files identical despite different names*

### Comparing `GMM_Demux-0.2.2.0/example_cell_types/CD56+CD16-.txt` & `GMM_Demux-0.2.2.1/example_cell_types/CD56+CD16-.txt`

 * *Files identical despite different names*

### Comparing `GMM_Demux-0.2.2.0/example_cell_types/Doublets/CD14+CD56+.txt` & `GMM_Demux-0.2.2.1/example_cell_types/Doublets/CD14+CD56+.txt`

 * *Files identical despite different names*

### Comparing `GMM_Demux-0.2.2.0/example_cell_types/Doublets/CD3+CD4+CD14+.txt` & `GMM_Demux-0.2.2.1/example_cell_types/Doublets/CD3+CD4+CD14+.txt`

 * *Files identical despite different names*

### Comparing `GMM_Demux-0.2.2.0/example_cell_types/Doublets/CD3+CD4+CD19+.txt` & `GMM_Demux-0.2.2.1/example_cell_types/Doublets/CD3+CD4+CD19+.txt`

 * *Files identical despite different names*

### Comparing `GMM_Demux-0.2.2.0/example_cell_types/Doublets/CD3+CD4+CD56+.txt` & `GMM_Demux-0.2.2.1/example_cell_types/Doublets/CD3+CD4+CD56+.txt`

 * *Files identical despite different names*

### Comparing `GMM_Demux-0.2.2.0/example_cell_types/Doublets/CD3+CD4+CD8+.txt` & `GMM_Demux-0.2.2.1/example_cell_types/Doublets/CD3+CD4+CD8+.txt`

 * *Files identical despite different names*

### Comparing `GMM_Demux-0.2.2.0/example_cell_types/Doublets/CD3+CD8+CD14+.txt` & `GMM_Demux-0.2.2.1/example_cell_types/Doublets/CD3+CD8+CD14+.txt`

 * *Files identical despite different names*

### Comparing `GMM_Demux-0.2.2.0/example_cell_types/Doublets/CD3+CD8+CD19+.txt` & `GMM_Demux-0.2.2.1/example_cell_types/Doublets/CD3+CD8+CD19+.txt`

 * *Files identical despite different names*

### Comparing `GMM_Demux-0.2.2.0/example_cell_types/Doublets/CD3+CD8+CD56+.txt` & `GMM_Demux-0.2.2.1/example_cell_types/Doublets/CD3+CD8+CD56+.txt`

 * *Files identical despite different names*

### Comparing `GMM_Demux-0.2.2.0/example_hto.csv` & `GMM_Demux-0.2.2.1/example_hto.csv`

 * *Files identical despite different names*

### Comparing `GMM_Demux-0.2.2.0/example_input/outs/filtered_feature_bc_matrix/barcodes.tsv.gz` & `GMM_Demux-0.2.2.1/example_input/outs/filtered_feature_bc_matrix/barcodes.tsv.gz`

 * *Files identical despite different names*

### Comparing `GMM_Demux-0.2.2.0/example_input/outs/filtered_feature_bc_matrix/matrix.mtx.gz` & `GMM_Demux-0.2.2.1/example_input/outs/filtered_feature_bc_matrix/matrix.mtx.gz`

 * *Files identical despite different names*

### Comparing `GMM_Demux-0.2.2.0/features.png` & `GMM_Demux-0.2.2.1/features.png`

 * *Files identical despite different names*

### Comparing `GMM_Demux-0.2.2.0/path.png` & `GMM_Demux-0.2.2.1/path.png`

 * *Files identical despite different names*

### Comparing `GMM_Demux-0.2.2.0/phony.png` & `GMM_Demux-0.2.2.1/phony.png`

 * *Files identical despite different names*

### Comparing `GMM_Demux-0.2.2.0/phony_type.png` & `GMM_Demux-0.2.2.1/phony_type.png`

 * *Files identical despite different names*

### Comparing `GMM_Demux-0.2.2.0/planner.png` & `GMM_Demux-0.2.2.1/planner.png`

 * *Files identical despite different names*

### Comparing `GMM_Demux-0.2.2.0/pure_type.png` & `GMM_Demux-0.2.2.1/pure_type.png`

 * *Files identical despite different names*

### Comparing `GMM_Demux-0.2.2.0/setup.py` & `GMM_Demux-0.2.2.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="GMM_Demux",
-    version="0.2.2.0",
+    version="0.2.2.1",
     author="Hongyi Xin",
     author_email="gohongyi@gmail.com",
     description="A multiplet removal tool for processing cell hashing data",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/CHPGenetics/GMM-demux",
     packages=setuptools.find_packages(),
```

### Comparing `GMM_Demux-0.2.2.0/summary.png` & `GMM_Demux-0.2.2.1/summary.png`

 * *Files identical despite different names*

### Comparing `GMM_Demux-0.2.2.0/term.png` & `GMM_Demux-0.2.2.1/term.png`

 * *Files identical despite different names*

