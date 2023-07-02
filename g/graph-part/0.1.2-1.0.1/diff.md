# Comparing `tmp/graph-part-0.1.2.tar.gz` & `tmp/graph-part-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graph-part-0.1.2.tar", last modified: Wed Mar 29 17:02:41 2023, max compression
+gzip compressed data, was "graph-part-1.0.1.tar", last modified: Sun Jul  2 18:28:49 2023, max compression
```

## Comparing `graph-part-0.1.2.tar` & `graph-part-1.0.1.tar`

### file list

```diff
@@ -1,25 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 17:02:41.833455 graph-part-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)    12885 2023-03-29 17:02:41.833455 graph-part-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12628 2023-03-29 17:02:29.000000 graph-part-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 17:02:41.833455 graph-part-0.1.2/graph_part/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-03-29 17:02:30.000000 graph-part-0.1.2/graph_part/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 17:02:30.000000 graph-part-0.1.2/graph_part/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13020 2023-03-29 17:02:30.000000 graph-part-0.1.2/graph_part/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    10118 2023-03-29 17:02:30.000000 graph-part-0.1.2/graph_part/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    27116 2023-03-29 17:02:30.000000 graph-part-0.1.2/graph_part/graph_part.py
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-03-29 17:02:30.000000 graph-part-0.1.2/graph_part/mmseqs_fake_prefilter.sh
--rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-03-29 17:02:30.000000 graph-part-0.1.2/graph_part/mmseqs_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11860 2023-03-29 17:02:30.000000 graph-part-0.1.2/graph_part/molecules.py
--rw-r--r--   0 runner    (1001) docker     (123)    15836 2023-03-29 17:02:30.000000 graph-part-0.1.2/graph_part/needle_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-03-29 17:02:30.000000 graph-part-0.1.2/graph_part/precomputed_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8376 2023-03-29 17:02:30.000000 graph-part-0.1.2/graph_part/train_val_test_split.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-03-29 17:02:30.000000 graph-part-0.1.2/graph_part/transformations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 17:02:41.833455 graph-part-0.1.2/graph_part.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12885 2023-03-29 17:02:41.000000 graph-part-0.1.2/graph_part.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-03-29 17:02:41.000000 graph-part-0.1.2/graph_part.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-29 17:02:41.000000 graph-part-0.1.2/graph_part.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-03-29 17:02:41.000000 graph-part-0.1.2/graph_part.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-03-29 17:02:41.000000 graph-part-0.1.2/graph_part.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-29 17:02:41.000000 graph-part-0.1.2/graph_part.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-29 17:02:41.833455 graph-part-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-03-29 17:02:30.000000 graph-part-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 18:28:49.178811 graph-part-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-07-02 18:28:38.000000 graph-part-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17029 2023-07-02 18:28:49.178811 graph-part-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16735 2023-07-02 18:28:38.000000 graph-part-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 18:28:49.178811 graph-part-1.0.1/graph_part/
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-02 18:28:38.000000 graph-part-1.0.1/graph_part/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 18:28:38.000000 graph-part-1.0.1/graph_part/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13608 2023-07-02 18:28:38.000000 graph-part-1.0.1/graph_part/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13160 2023-07-02 18:28:38.000000 graph-part-1.0.1/graph_part/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30192 2023-07-02 18:28:38.000000 graph-part-1.0.1/graph_part/graph_part.py
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-07-02 18:28:38.000000 graph-part-1.0.1/graph_part/mmseqs_fake_prefilter.sh
+-rw-r--r--   0 runner    (1001) docker     (123)    17171 2023-07-02 18:28:38.000000 graph-part-1.0.1/graph_part/mmseqs_needle_combined_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-07-02 18:28:38.000000 graph-part-1.0.1/graph_part/mmseqs_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11860 2023-07-02 18:28:38.000000 graph-part-1.0.1/graph_part/molecules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15836 2023-07-02 18:28:38.000000 graph-part-1.0.1/graph_part/needle_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-07-02 18:28:38.000000 graph-part-1.0.1/graph_part/precomputed_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8376 2023-07-02 18:28:38.000000 graph-part-1.0.1/graph_part/train_val_test_split.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-07-02 18:28:38.000000 graph-part-1.0.1/graph_part/transformations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 18:28:49.178811 graph-part-1.0.1/graph_part.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17029 2023-07-02 18:28:49.000000 graph-part-1.0.1/graph_part.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-02 18:28:49.000000 graph-part-1.0.1/graph_part.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 18:28:49.000000 graph-part-1.0.1/graph_part.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-02 18:28:49.000000 graph-part-1.0.1/graph_part.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-02 18:28:49.000000 graph-part-1.0.1/graph_part.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-02 18:28:49.000000 graph-part-1.0.1/graph_part.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 18:28:49.178811 graph-part-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-07-02 18:28:38.000000 graph-part-1.0.1/setup.py
```

### Comparing `graph-part-0.1.2/PKG-INFO` & `graph-part-1.0.1/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,22 @@
-Metadata-Version: 2.1
-Name: graph-part
-Version: 0.1.2
-Summary: Graph-based partitioning of biological sequence data
-Home-page: https://healthtech.dtu.dk
-Author: F. Teufel and M.H. Gislason
-Requires-Python: >=3.6, <4
-Description-Content-Type: text/markdown
-
 # GraphPart
-Biological sequence dataset partitioning pipeline
+
+[![PyPI version](https://badge.fury.io/py/graph-part.svg)](https://badge.fury.io/py/graph-part)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/graph-part)
+[![PyPIDownloadsTotal](https://pepy.tech/badge/graph-part)](https://pepy.tech/project/graph-part)
+[![Stars](https://img.shields.io/github/stars/graph-part/graph-part?logo=GitHub&color=yellow)](https://github.com/graph-part/graph-part/stargazers)
+
+
+
+**Biological sequence dataset partitioning method**
+
 
 Graph-Part is a Python package for generating partitions (i.e. train-test splits, or splits for cross-validation) of biological sequence datasets. It ensures minimal homology between different partitions, while balancing partitions for labels or other desired criteria.
 
+Preprint: https://www.biorxiv.org/content/10.1101/2023.04.14.536886v1
 
 ## Installation
 
 GraphPart relies on [needleall](https://www.bioinformatics.nl/cgi-bin/emboss/help/needleall) from the [EMBOSS](http://emboss.sourceforge.net/) package for Needleman-Wunsch alignments of sequences. Please refer to the official EMBOSS documentation for installation methods.
 Additionally, GraphPart supports [MMseqs2](https://github.com/soedinglab/MMseqs2) for alignments. To use other algorithms that compute pairwise similarity measures, please refer to the `precomputed` mode.
 
 We recommend to install GraphPart in a conda environment, and install EMBOSS from [bioconda](https://anaconda.org/bioconda/emboss). The same goes for [MMseqs2](https://anaconda.org/bioconda/mmseqs2).
@@ -121,15 +122,15 @@
 Long                    | Short | Description
 ------------------------|-------|------------
 `--denominator`         |`-dn`  | Denominator to use for percent sequence identity computation. The number of perfect matching positions is divided by the result of this operation. Can be any of `shortest`, `longest`, `mean`, `full`, `no_gaps`. The first three options are computed from the original lengths of the aligned sequences. `full` refers to the full length of the alignment, including gaps, and is the default. `no_gaps` subtracts gaps from the full alignment length.
 `--threads`             |`-nt`  | The number of threads to run in parallel. If `-1`, will use all available resources. Defaults to 1.
 `--chunks`              |`-nc`  | The number of chunks into which to split the fasta file for multithreaded alignment. Defaults to 10.
 `--parallel-mode`       |`-pm`  | The Python parallelization strategy to use. `multithread` or `multiprocess`. Multiprocessing is potentially faster (especially for short sequences), but increases memory usage.
 `--nucleotide`          |`-nu`  | Use this flag if the input contains nucleotide sequences. By default, assumes proteins.
-`--triangular`          |`-tr`  | Only compute triangular of the full distance matrix. Twice as fast, but can yield slightly different results if an alignment has two different solutions with the same score, but different identities.
+`--triangular`          |`-tr`  | Only compute triangular of the full distance matrix. Twice as fast, but can yield slightly different results if an alignment has two different solutions with the same score, but different identities. In some cases, a pairwise identity can be slightly above the threshold in one solution, and slightly below in another (e.g A:B = 29.8%, B:A = 30.4%).
 `--gapopen`             |`-gapopen`     | [10.0 for any sequence] The gap open penalty is the score taken away when a gap is created. The best value depends on the choice of comparison matrix. The default value assumes you are using the EBLOSUM62 matrix. (Floating point number from 1.0 to 100.0)
 `--gapextend`           |`-gapextend`   | [0.5 for any sequence] The gap extension penalty is added to the standard gap penalty for each base or residue in the gap. This is how long gaps are penalized. Usually you will expect a few long gaps rather than many short gaps, so the gap extension penalty should be lower than the gap penalty. An exception is where one or both sequences are single reads with possible sequencing errors in which case you would expect many single base gaps. You can get this result by setting the gap open penalty to zero (or very low) and using the gap extension penalty to control gap scoring. (Floating point number from 0.0 to 10.0)
 `--endextend`           |`-endextend`   | [0.5 for any sequence] The end gap extension, penalty is added to the end gap penalty for each base or residue in the end gap. This is how long end gaps are penalized. (Floating point number from 0.0 to 10.0)
 `--endweight`           |`-endweight`   | Flag. Apply end gap penalties.
 `--endopen`             |`-endopen`     | [10.0 for any sequence] The end gap open penalty is the score taken away when an end gap is created. The best value depends on the choice of comparison matrix. The default value assumes you are using the EBLOSUM62 matrix for protein sequences. (Floating point number from 1.0 to 100.0)
 `--matrix`              |`-datafile`    | This is the scoring matrix file used when comparing sequences. By default it is the file 'EBLOSUM62'. These files are found in the 'data' directory of the EMBOSS installation.
 
@@ -147,15 +148,42 @@
   
 
 Long                    | Short | Description
 ------------------------|-------|------------
 `--edge-file`           |`-ef`  | Path to a comma separated file containing precomputed pairwise metrics, the first two columns should contain sequence identifiers specified in the  `--fasta-file`. This is can be used to run GraphPart with an alignment tool different from the default `needleall` and `mmseqs`.
 `--metric-column`       |`-mc`  | Specifies in which column the metric is found. Indexing starts at 0, defaults to 2 when left unspecified.
 
+#### mmseqs2needle
+
+This mode combines `needle` and `mmseqs2`. After a first run of `mmseqs2`, all pairwise alignments with an indentity below `recompute-threshold` are computed using `needle`. Only then the partitioning is performed. Note that if `recompute-threshold` is very low, it can be faster to just run in `needle` mode. All arguments for the two modes are reused here, with the following exceptions:
+
+Long                    | Short | Description
+------------------------|-------|------------
+`--recompute-threshold` | `-re` | The threshold for MMseqs2 above which alignments should be recomputed using needleall. Has to be a number lower than `--threshold`.
+`--denominator-mmseqs`  | `-dnm`| Replaces `--denominator`. Applies to the mmseqs2 alignment step.
+`--denominator-needle`  | `-dnn`| Replaces `--denominator`. Applies to the needle alignment step.
+## Citation
+
+    GraphPart: Homology partitioning for biological sequence analysis
+    Felix Teufel, Magnús Halldór Gíslason, José Juan Almagro Armenteros, Alexander Rosenberg Johansen, Ole Winther, Henrik Nielsen
+    bioRxiv 2023.04.14.536886; doi: https://doi.org/10.1101/2023.04.14.536886
+
 ## FAQ
 
 - **How should I pick `chunks` ?**  
 `chunks` should be picked so that all `threads` are utilized. Each chunk is aligned to each other chunk, so `threads` <= `chunks`*`chunks` results in full utilization.
 
 - **I want to test multiple thresholds and partitioning parameters - How can I do this efficiently ?**  
 When constructing the graph, we only retain identities that are larger than the selected `threshold`, as only those form relevant edges for partitioning the data. All other similarities are discarded as they are computed. To test multiple thresholds, the most efficient way is to first try the lowest threshold to be considered and save the edge list by specifying `--save-checkpoint-path EDGELIST.csv`. In the next run, use `graphpart precomputed -ef EDGELIST.csv` to start directly from the previous alignment result.
 
+- **GraphPart starts with nicely balanced partitions, but after homology removal the sizes are very imbalanced.**  
+By default, GraphPart tries to retain as many sequences as possible. In cases where the initialization clustering is far away from a valid solution (this happens when there are a lot of classes, with potentially small counts, and when there is high overall sequence similarity in the data), moving sequences between partitions will cause some partitions to grow large at the expense of others. You can try `--no-moving` to prevent this behaviour. 
+
+
+- **I want to use a different similarity metric than sequence identity.**
+GraphPart can be used with any similarity or distance metric. To do so, you need to provide a list of precomputed pairwise similarities in the `precomputed` mode. The first two columns of the file should contain the sequence identifiers specified in the `--fasta-file`. The third column should contain the similarity metric. The `--metric-column` argument can be used to specify the column index. If you want to use a similarity metric, you need to specify a transformation using `--transformation`. See the [source](graph_part/transformations.py) for definitions. As an example, when operating with sequence identities ranging from 0 to 1, the transformation `one-minus` yields corresponding distances. If your metric is a distance, you can use `--transformation None` to skip the transformation step.
+
+- **I want to use a different alignment tool than EMBOSS needleall or MMseqs.**
+This is supported by the [precomputed](#precomputed) mode. Please refer to the answer above.
+
+- **How does the moving step decide to which partition to move a sequence to?**
+After initialization of the partitions, GraphPart iteratively moves sequences between partitions and removes sequences from the data to achieve homology separation. For each sequence, we compute how many connections it has to sequences in each other partition. If there are partitions with more connections than the current partition, the sequence is moved to the partition with the maximum number of connections. If there is a tie in the number of connections, the sequence is moved to the partition that appeared first when iterating the underlying graph data structure. We do not explicitly control this order.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `graph-part-0.1.2/README.md` & `graph-part-1.0.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,32 @@
+Metadata-Version: 2.1
+Name: graph-part
+Version: 1.0.1
+Summary: Graph-based partitioning of biological sequence data
+Home-page: https://github.com/graph-part/graph-part
+Author: F. Teufel and M.H. Gislason
+Requires-Python: >=3.6, <4
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # GraphPart
-Biological sequence dataset partitioning pipeline
+
+[![PyPI version](https://badge.fury.io/py/graph-part.svg)](https://badge.fury.io/py/graph-part)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/graph-part)
+[![PyPIDownloadsTotal](https://pepy.tech/badge/graph-part)](https://pepy.tech/project/graph-part)
+[![Stars](https://img.shields.io/github/stars/graph-part/graph-part?logo=GitHub&color=yellow)](https://github.com/graph-part/graph-part/stargazers)
+
+
+
+**Biological sequence dataset partitioning method**
+
 
 Graph-Part is a Python package for generating partitions (i.e. train-test splits, or splits for cross-validation) of biological sequence datasets. It ensures minimal homology between different partitions, while balancing partitions for labels or other desired criteria.
 
+Preprint: https://www.biorxiv.org/content/10.1101/2023.04.14.536886v1
 
 ## Installation
 
 GraphPart relies on [needleall](https://www.bioinformatics.nl/cgi-bin/emboss/help/needleall) from the [EMBOSS](http://emboss.sourceforge.net/) package for Needleman-Wunsch alignments of sequences. Please refer to the official EMBOSS documentation for installation methods.
 Additionally, GraphPart supports [MMseqs2](https://github.com/soedinglab/MMseqs2) for alignments. To use other algorithms that compute pairwise similarity measures, please refer to the `precomputed` mode.
 
 We recommend to install GraphPart in a conda environment, and install EMBOSS from [bioconda](https://anaconda.org/bioconda/emboss). The same goes for [MMseqs2](https://anaconda.org/bioconda/mmseqs2).
@@ -112,15 +132,15 @@
 Long                    | Short | Description
 ------------------------|-------|------------
 `--denominator`         |`-dn`  | Denominator to use for percent sequence identity computation. The number of perfect matching positions is divided by the result of this operation. Can be any of `shortest`, `longest`, `mean`, `full`, `no_gaps`. The first three options are computed from the original lengths of the aligned sequences. `full` refers to the full length of the alignment, including gaps, and is the default. `no_gaps` subtracts gaps from the full alignment length.
 `--threads`             |`-nt`  | The number of threads to run in parallel. If `-1`, will use all available resources. Defaults to 1.
 `--chunks`              |`-nc`  | The number of chunks into which to split the fasta file for multithreaded alignment. Defaults to 10.
 `--parallel-mode`       |`-pm`  | The Python parallelization strategy to use. `multithread` or `multiprocess`. Multiprocessing is potentially faster (especially for short sequences), but increases memory usage.
 `--nucleotide`          |`-nu`  | Use this flag if the input contains nucleotide sequences. By default, assumes proteins.
-`--triangular`          |`-tr`  | Only compute triangular of the full distance matrix. Twice as fast, but can yield slightly different results if an alignment has two different solutions with the same score, but different identities.
+`--triangular`          |`-tr`  | Only compute triangular of the full distance matrix. Twice as fast, but can yield slightly different results if an alignment has two different solutions with the same score, but different identities. In some cases, a pairwise identity can be slightly above the threshold in one solution, and slightly below in another (e.g A:B = 29.8%, B:A = 30.4%).
 `--gapopen`             |`-gapopen`     | [10.0 for any sequence] The gap open penalty is the score taken away when a gap is created. The best value depends on the choice of comparison matrix. The default value assumes you are using the EBLOSUM62 matrix. (Floating point number from 1.0 to 100.0)
 `--gapextend`           |`-gapextend`   | [0.5 for any sequence] The gap extension penalty is added to the standard gap penalty for each base or residue in the gap. This is how long gaps are penalized. Usually you will expect a few long gaps rather than many short gaps, so the gap extension penalty should be lower than the gap penalty. An exception is where one or both sequences are single reads with possible sequencing errors in which case you would expect many single base gaps. You can get this result by setting the gap open penalty to zero (or very low) and using the gap extension penalty to control gap scoring. (Floating point number from 0.0 to 10.0)
 `--endextend`           |`-endextend`   | [0.5 for any sequence] The end gap extension, penalty is added to the end gap penalty for each base or residue in the end gap. This is how long end gaps are penalized. (Floating point number from 0.0 to 10.0)
 `--endweight`           |`-endweight`   | Flag. Apply end gap penalties.
 `--endopen`             |`-endopen`     | [10.0 for any sequence] The end gap open penalty is the score taken away when an end gap is created. The best value depends on the choice of comparison matrix. The default value assumes you are using the EBLOSUM62 matrix for protein sequences. (Floating point number from 1.0 to 100.0)
 `--matrix`              |`-datafile`    | This is the scoring matrix file used when comparing sequences. By default it is the file 'EBLOSUM62'. These files are found in the 'data' directory of the EMBOSS installation.
 
@@ -138,15 +158,42 @@
   
 
 Long                    | Short | Description
 ------------------------|-------|------------
 `--edge-file`           |`-ef`  | Path to a comma separated file containing precomputed pairwise metrics, the first two columns should contain sequence identifiers specified in the  `--fasta-file`. This is can be used to run GraphPart with an alignment tool different from the default `needleall` and `mmseqs`.
 `--metric-column`       |`-mc`  | Specifies in which column the metric is found. Indexing starts at 0, defaults to 2 when left unspecified.
 
+#### mmseqs2needle
+
+This mode combines `needle` and `mmseqs2`. After a first run of `mmseqs2`, all pairwise alignments with an indentity below `recompute-threshold` are computed using `needle`. Only then the partitioning is performed. Note that if `recompute-threshold` is very low, it can be faster to just run in `needle` mode. All arguments for the two modes are reused here, with the following exceptions:
+
+Long                    | Short | Description
+------------------------|-------|------------
+`--recompute-threshold` | `-re` | The threshold for MMseqs2 above which alignments should be recomputed using needleall. Has to be a number lower than `--threshold`.
+`--denominator-mmseqs`  | `-dnm`| Replaces `--denominator`. Applies to the mmseqs2 alignment step.
+`--denominator-needle`  | `-dnn`| Replaces `--denominator`. Applies to the needle alignment step.
+## Citation
+
+    GraphPart: Homology partitioning for biological sequence analysis
+    Felix Teufel, Magnús Halldór Gíslason, José Juan Almagro Armenteros, Alexander Rosenberg Johansen, Ole Winther, Henrik Nielsen
+    bioRxiv 2023.04.14.536886; doi: https://doi.org/10.1101/2023.04.14.536886
+
 ## FAQ
 
 - **How should I pick `chunks` ?**  
 `chunks` should be picked so that all `threads` are utilized. Each chunk is aligned to each other chunk, so `threads` <= `chunks`*`chunks` results in full utilization.
 
 - **I want to test multiple thresholds and partitioning parameters - How can I do this efficiently ?**  
 When constructing the graph, we only retain identities that are larger than the selected `threshold`, as only those form relevant edges for partitioning the data. All other similarities are discarded as they are computed. To test multiple thresholds, the most efficient way is to first try the lowest threshold to be considered and save the edge list by specifying `--save-checkpoint-path EDGELIST.csv`. In the next run, use `graphpart precomputed -ef EDGELIST.csv` to start directly from the previous alignment result.
 
+- **GraphPart starts with nicely balanced partitions, but after homology removal the sizes are very imbalanced.**  
+By default, GraphPart tries to retain as many sequences as possible. In cases where the initialization clustering is far away from a valid solution (this happens when there are a lot of classes, with potentially small counts, and when there is high overall sequence similarity in the data), moving sequences between partitions will cause some partitions to grow large at the expense of others. You can try `--no-moving` to prevent this behaviour. 
+
+
+- **I want to use a different similarity metric than sequence identity.**
+GraphPart can be used with any similarity or distance metric. To do so, you need to provide a list of precomputed pairwise similarities in the `precomputed` mode. The first two columns of the file should contain the sequence identifiers specified in the `--fasta-file`. The third column should contain the similarity metric. The `--metric-column` argument can be used to specify the column index. If you want to use a similarity metric, you need to specify a transformation using `--transformation`. See the [source](graph_part/transformations.py) for definitions. As an example, when operating with sequence identities ranging from 0 to 1, the transformation `one-minus` yields corresponding distances. If your metric is a distance, you can use `--transformation None` to skip the transformation step.
+
+- **I want to use a different alignment tool than EMBOSS needleall or MMseqs.**
+This is supported by the [precomputed](#precomputed) mode. Please refer to the answer above.
+
+- **How does the moving step decide to which partition to move a sequence to?**
+After initialization of the partitions, GraphPart iteratively moves sequences between partitions and removes sequences from the data to achieve homology separation. For each sequence, we compute how many connections it has to sequences in each other partition. If there are partitions with more connections than the current partition, the sequence is moved to the partition with the maximum number of connections. If there is a tie in the number of connections, the sequence is moved to the partition that appeared first when iterating the underlying graph data structure. We do not explicitly control this order.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `graph-part-0.1.2/graph_part/api.py` & `graph-part-1.0.1/graph_part/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,14 +80,15 @@
                      alignment_mode: str = 'mmseqs2',
                      initialization_mode: str = 'slow-nn',
                      no_moving: bool = False,
                      remove_same: bool = False,
                      save_checkpoint_path: str = None,
                      denominator: str = 'full',
                      nucleotide: bool = False,
+                     prefilter: bool = False,
                      triangular: bool = False,
                      threads: int = 4,
                      chunks: int = 10,
                      parallel_mode: str = 'multithread',
                      gapopen: float = 10,
                      gapextend: float = 0.5,
                      endweight: bool = False,
@@ -146,14 +147,15 @@
         "no_moving": no_moving,
         "remove_same": remove_same,
         "test_ratio": 0,
         "val_ratio": 0,
         "save_checkpoint_path": save_checkpoint_path,
         "denominator": denominator,
         "nucleotide": nucleotide,
+        "prefilter": prefilter,
         "triangular": triangular,
         "threads": threads,
         "chunks": chunks,
         "parallel_mode": parallel_mode,
         "gapopen": gapopen,
         "gapextend": gapextend,
         "endweight": endweight,
@@ -168,14 +170,22 @@
 
     # 3. Partition
     partition_assignment_df = run_partitioning(config, write_output_file=False, write_json_report=False, verbose=False)
     os.remove(config['fasta_file'])
 
     # 4. Make output lists.
     partition_assignment_df = partition_assignment_df.reset_index()
+
+    # 'AC' will be type string. But potentially the original 'AC' were ints.
+    if type(next(sequences.keys())) == int:
+        try:
+            partition_assignment_df['AC'] = partition_assignment_df['AC'].astype(int)
+        except:
+            pass
+
     outs = []
     # iterate over all created folds and add to the output list.
     for _, sub_df in partition_assignment_df.groupby('cluster'):
 
         if original_type in [np.ndarray, list]:
             outs.append(sub_df.index.tolist())
         else:
@@ -301,14 +311,22 @@
 
     # 3. Partition
     partition_assignment_df = run_partitioning(config, write_output_file=False, write_json_report=False, verbose=False)
     os.remove(config['fasta_file'])
 
     # 4. Make output lists.
     partition_assignment_df = partition_assignment_df.reset_index()
+
+    # 'AC' will be type string. But potentially the original 'AC' were ints.
+    if type(next(sequences.keys())) == int:
+        try:
+            partition_assignment_df['AC'] = partition_assignment_df['AC'].astype(int)
+        except:
+            pass
+
     outs = []
     # iterate over all created folds and add to the output list.
     for _, sub_df in partition_assignment_df.groupby('cluster'):
 
         if original_type in [np.ndarray, list]:
             outs.append(sub_df.index.tolist())
         else:
```

### Comparing `graph-part-0.1.2/graph_part/graph_part.py` & `graph-part-1.0.1/graph_part/graph_part.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 import networkx as nx
 from typing import Dict, List, Tuple, Any, Union
 import time
 from collections import Counter
 from itertools import product
 import time
 
+from tqdm import tqdm
+
 from .transformations import TRANSFORMATIONS
 from .train_val_test_split import train_val_test_split
 
 #TODO update new arg names here
 """
 This program partitions an entity set according to a single pairwise distance metric
 and some desired threshold the partitions should fullfill.
@@ -179,15 +181,15 @@
     ## AC, cluster, label
     acs = []
     clusters = []
     labels = []
     print("Initialization mode", mode)
 
     ## Initialize the initialization
-    for ind, AC in enumerate(part_graph.nodes()):
+    for ind, AC in tqdm(enumerate(part_graph.nodes()), desc='Initializing'):
         label_counts = np.zeros(len(label_limits), dtype=int)
         label_counts[full_graph.nodes[AC]['label-val']] = 1
         cluster_nr = ind
         
         if mode == 'simple':
             d = full_graph.nodes[AC]
             acs.append(AC)
@@ -200,15 +202,46 @@
                 'label-counts': label_counts
             }
         })
 
     ## Restricted closest neighbour linkage
     if mode in ['slow-nn', 'fast-nn']:
         ## Linking entities, if restrictions allow
-        for qry, lib, data in sorted(full_graph.edges(data=True), key=lambda x: x[2]['metric']):
+
+
+        # NOTE sorting the networkx edges using sorted() becomes extremely slow on large graphs.
+        # partly, because .edges takes forever to yield its EdgeView
+        # workaround by instead extracting all the metric values into a numpy vector and argsorting this.
+        # tested on ~400m edges, np.argsort 10 min vs. sorted() multiple hours
+        queries = []
+        libs = []
+        metrics = []
+                
+        start = time.perf_counter()
+
+        for qry, lib, data in full_graph.edges(data=True):
+            queries.append(qry)
+            libs.append(lib)
+            metrics.append(data['metric'])
+
+        elapsed_align = time.perf_counter() - start
+        print(f"Edge iteration completed in {elapsed_align:0.2f} seconds.")
+        
+        
+        metrics = np.array(metrics)
+        inds = np.argsort(metrics)
+        elapsed_align = time.perf_counter() - start
+        print(f"Edge sorting competed at {elapsed_align:0.2f} seconds.")
+        for idx in tqdm(inds, desc='clustering'):
+            qry, lib = queries[idx], libs[idx]
+            data = full_graph.edges[qry, lib]
+
+            ### continue as below
+
+        # for qry, lib, data in tqdm(sorted(full_graph.edges(data=True), key=lambda x: x[2]['metric']), desc='Clustering'):
             if data['metric'] > threshold:
                 ## No need to continue if threshold reached.
                 break
             
             if part_graph.has_edge(qry, lib):
                 ## Update edge if it exists
                 if part_graph[qry][lib]['metric'] > data['metric']:
@@ -234,17 +267,17 @@
             nx.set_node_attributes(part_graph, {qry:attr})
             part_graph.add_edge(qry, lib, metric=data['metric'])
 
             for descendant in nx.descendants(part_graph, qry):
                 nx.set_node_attributes(part_graph, {descendant:attr})
 
             count += 1
-            if count % 10000 == 0:
-                print("edges:", part_graph.number_of_edges()) 
-                print (attr, data)
+            #if count % 10000 == 0:
+            #    print("edges:", part_graph.number_of_edges()) 
+            #    print (attr, data)
         #with open('graph_part_miniclusters.txt','w+') as outf:
         for cc_nr, cc in enumerate(nx.connected_components(part_graph)):
             for n in cc:
                 d = full_graph.nodes[n]
                 acs.append(n)
                 clusters.append(cc_nr)
                 labels.append(d['label-val'])
@@ -472,14 +505,42 @@
         print('Computing pairwise sequence identities.')
         generate_edges(config['fasta_file'],full_graph, config['transformation'], threshold, denominator=config['denominator'], delimiter='|',
                             is_nucleotide=config['nucleotide'], gapopen=config['gapopen'], gapextend=config['gapextend'], endweight=config['endweight'], endopen=config['endopen'], endextend=config['endextend'], matrix=config['matrix'])
         elapsed_align = time.perf_counter() - json_dict['time_script_start'] 
         if verbose:
             print(f"Pairwise alignment executed in {elapsed_align:0.2f} seconds.")
 
+    elif config['alignment_mode'] == 'mmseqs2needle':
+        from .mmseqs_needle_combined_utils import generate_edges_mmseqs_needle_combined
+        recompute_threshold = TRANSFORMATIONS[config['transformation']](config['recompute_threshold'])
+        print('Computing pairwise sequence identities.')
+        generate_edges_mmseqs_needle_combined(
+            config['fasta_file'],
+            full_graph,
+            transformation=config['transformation'],
+            threshold=threshold,
+            recompute_threshold=recompute_threshold,
+            denominator_needle=config['denominator_needle'],
+            denominator_mmseqs=config['denominator_mmseqs'],
+            n_procs=config['threads'],
+            parallel_mode=config['parallel_mode'],
+            triangular=config['triangular'],
+            delimiter='|',
+            is_nucleotide=config['nucleotide'],
+            use_prefilter=config['prefilter'],
+            gapopen=config['gapopen'],
+            gapextend=config['gapextend'],
+            endweight=config['endweight'],
+            endopen=config['endopen'],
+            endextend=config['endextend'],
+            matrix=config['matrix']
+        )
+        # generate_edges_mmseqs_needle_combined(config['fasta_file'], full_graph, config['transformation'], threshold, recompute_threshold, config['threshold'], denominator_needle=config['denominator_needle'], denominator_mmseqs=config['denominator_mmseqs'], n_procs=config['threads'], parallel_mode=config['parallel_mode'], triangular=config['triangular'], delimiter='|', 
+                                            #   is_nucleotide=config['nucleotide'], use_prefilter=config['prefilter'], gapopen=config['gapopen'], gapextend=config['gapextend'], endweight=config['endweight'], endopen=config['endopen'], endextend=config['endextend'], matrix=config['matrix'])
+
     else:
         raise NotImplementedError('Encountered unspecified alignment mode. This should never happen.')
 
     
     return full_graph, part_graph, labels
```

### Comparing `graph-part-0.1.2/graph_part/mmseqs_fake_prefilter.sh` & `graph-part-1.0.1/graph_part/mmseqs_fake_prefilter.sh`

 * *Files identical despite different names*

### Comparing `graph-part-0.1.2/graph_part/mmseqs_utils.py` & `graph-part-1.0.1/graph_part/mmseqs_utils.py`

 * *Files identical despite different names*

### Comparing `graph-part-0.1.2/graph_part/molecules.py` & `graph-part-1.0.1/graph_part/molecules.py`

 * *Files identical despite different names*

### Comparing `graph-part-0.1.2/graph_part/needle_utils.py` & `graph-part-1.0.1/graph_part/needle_utils.py`

 * *Files identical despite different names*

### Comparing `graph-part-0.1.2/graph_part/precomputed_utils.py` & `graph-part-1.0.1/graph_part/precomputed_utils.py`

 * *Files identical despite different names*

### Comparing `graph-part-0.1.2/graph_part/train_val_test_split.py` & `graph-part-1.0.1/graph_part/train_val_test_split.py`

 * *Files identical despite different names*

### Comparing `graph-part-0.1.2/graph_part/transformations.py` & `graph-part-1.0.1/graph_part/transformations.py`

 * *Files identical despite different names*

### Comparing `graph-part-0.1.2/graph_part.egg-info/PKG-INFO` & `graph-part-1.0.1/graph_part.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,32 @@
 Metadata-Version: 2.1
 Name: graph-part
-Version: 0.1.2
+Version: 1.0.1
 Summary: Graph-based partitioning of biological sequence data
-Home-page: https://healthtech.dtu.dk
+Home-page: https://github.com/graph-part/graph-part
 Author: F. Teufel and M.H. Gislason
 Requires-Python: >=3.6, <4
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # GraphPart
-Biological sequence dataset partitioning pipeline
+
+[![PyPI version](https://badge.fury.io/py/graph-part.svg)](https://badge.fury.io/py/graph-part)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/graph-part)
+[![PyPIDownloadsTotal](https://pepy.tech/badge/graph-part)](https://pepy.tech/project/graph-part)
+[![Stars](https://img.shields.io/github/stars/graph-part/graph-part?logo=GitHub&color=yellow)](https://github.com/graph-part/graph-part/stargazers)
+
+
+
+**Biological sequence dataset partitioning method**
+
 
 Graph-Part is a Python package for generating partitions (i.e. train-test splits, or splits for cross-validation) of biological sequence datasets. It ensures minimal homology between different partitions, while balancing partitions for labels or other desired criteria.
 
+Preprint: https://www.biorxiv.org/content/10.1101/2023.04.14.536886v1
 
 ## Installation
 
 GraphPart relies on [needleall](https://www.bioinformatics.nl/cgi-bin/emboss/help/needleall) from the [EMBOSS](http://emboss.sourceforge.net/) package for Needleman-Wunsch alignments of sequences. Please refer to the official EMBOSS documentation for installation methods.
 Additionally, GraphPart supports [MMseqs2](https://github.com/soedinglab/MMseqs2) for alignments. To use other algorithms that compute pairwise similarity measures, please refer to the `precomputed` mode.
 
 We recommend to install GraphPart in a conda environment, and install EMBOSS from [bioconda](https://anaconda.org/bioconda/emboss). The same goes for [MMseqs2](https://anaconda.org/bioconda/mmseqs2).
@@ -121,15 +132,15 @@
 Long                    | Short | Description
 ------------------------|-------|------------
 `--denominator`         |`-dn`  | Denominator to use for percent sequence identity computation. The number of perfect matching positions is divided by the result of this operation. Can be any of `shortest`, `longest`, `mean`, `full`, `no_gaps`. The first three options are computed from the original lengths of the aligned sequences. `full` refers to the full length of the alignment, including gaps, and is the default. `no_gaps` subtracts gaps from the full alignment length.
 `--threads`             |`-nt`  | The number of threads to run in parallel. If `-1`, will use all available resources. Defaults to 1.
 `--chunks`              |`-nc`  | The number of chunks into which to split the fasta file for multithreaded alignment. Defaults to 10.
 `--parallel-mode`       |`-pm`  | The Python parallelization strategy to use. `multithread` or `multiprocess`. Multiprocessing is potentially faster (especially for short sequences), but increases memory usage.
 `--nucleotide`          |`-nu`  | Use this flag if the input contains nucleotide sequences. By default, assumes proteins.
-`--triangular`          |`-tr`  | Only compute triangular of the full distance matrix. Twice as fast, but can yield slightly different results if an alignment has two different solutions with the same score, but different identities.
+`--triangular`          |`-tr`  | Only compute triangular of the full distance matrix. Twice as fast, but can yield slightly different results if an alignment has two different solutions with the same score, but different identities. In some cases, a pairwise identity can be slightly above the threshold in one solution, and slightly below in another (e.g A:B = 29.8%, B:A = 30.4%).
 `--gapopen`             |`-gapopen`     | [10.0 for any sequence] The gap open penalty is the score taken away when a gap is created. The best value depends on the choice of comparison matrix. The default value assumes you are using the EBLOSUM62 matrix. (Floating point number from 1.0 to 100.0)
 `--gapextend`           |`-gapextend`   | [0.5 for any sequence] The gap extension penalty is added to the standard gap penalty for each base or residue in the gap. This is how long gaps are penalized. Usually you will expect a few long gaps rather than many short gaps, so the gap extension penalty should be lower than the gap penalty. An exception is where one or both sequences are single reads with possible sequencing errors in which case you would expect many single base gaps. You can get this result by setting the gap open penalty to zero (or very low) and using the gap extension penalty to control gap scoring. (Floating point number from 0.0 to 10.0)
 `--endextend`           |`-endextend`   | [0.5 for any sequence] The end gap extension, penalty is added to the end gap penalty for each base or residue in the end gap. This is how long end gaps are penalized. (Floating point number from 0.0 to 10.0)
 `--endweight`           |`-endweight`   | Flag. Apply end gap penalties.
 `--endopen`             |`-endopen`     | [10.0 for any sequence] The end gap open penalty is the score taken away when an end gap is created. The best value depends on the choice of comparison matrix. The default value assumes you are using the EBLOSUM62 matrix for protein sequences. (Floating point number from 1.0 to 100.0)
 `--matrix`              |`-datafile`    | This is the scoring matrix file used when comparing sequences. By default it is the file 'EBLOSUM62'. These files are found in the 'data' directory of the EMBOSS installation.
 
@@ -147,15 +158,42 @@
   
 
 Long                    | Short | Description
 ------------------------|-------|------------
 `--edge-file`           |`-ef`  | Path to a comma separated file containing precomputed pairwise metrics, the first two columns should contain sequence identifiers specified in the  `--fasta-file`. This is can be used to run GraphPart with an alignment tool different from the default `needleall` and `mmseqs`.
 `--metric-column`       |`-mc`  | Specifies in which column the metric is found. Indexing starts at 0, defaults to 2 when left unspecified.
 
+#### mmseqs2needle
+
+This mode combines `needle` and `mmseqs2`. After a first run of `mmseqs2`, all pairwise alignments with an indentity below `recompute-threshold` are computed using `needle`. Only then the partitioning is performed. Note that if `recompute-threshold` is very low, it can be faster to just run in `needle` mode. All arguments for the two modes are reused here, with the following exceptions:
+
+Long                    | Short | Description
+------------------------|-------|------------
+`--recompute-threshold` | `-re` | The threshold for MMseqs2 above which alignments should be recomputed using needleall. Has to be a number lower than `--threshold`.
+`--denominator-mmseqs`  | `-dnm`| Replaces `--denominator`. Applies to the mmseqs2 alignment step.
+`--denominator-needle`  | `-dnn`| Replaces `--denominator`. Applies to the needle alignment step.
+## Citation
+
+    GraphPart: Homology partitioning for biological sequence analysis
+    Felix Teufel, Magnús Halldór Gíslason, José Juan Almagro Armenteros, Alexander Rosenberg Johansen, Ole Winther, Henrik Nielsen
+    bioRxiv 2023.04.14.536886; doi: https://doi.org/10.1101/2023.04.14.536886
+
 ## FAQ
 
 - **How should I pick `chunks` ?**  
 `chunks` should be picked so that all `threads` are utilized. Each chunk is aligned to each other chunk, so `threads` <= `chunks`*`chunks` results in full utilization.
 
 - **I want to test multiple thresholds and partitioning parameters - How can I do this efficiently ?**  
 When constructing the graph, we only retain identities that are larger than the selected `threshold`, as only those form relevant edges for partitioning the data. All other similarities are discarded as they are computed. To test multiple thresholds, the most efficient way is to first try the lowest threshold to be considered and save the edge list by specifying `--save-checkpoint-path EDGELIST.csv`. In the next run, use `graphpart precomputed -ef EDGELIST.csv` to start directly from the previous alignment result.
 
+- **GraphPart starts with nicely balanced partitions, but after homology removal the sizes are very imbalanced.**  
+By default, GraphPart tries to retain as many sequences as possible. In cases where the initialization clustering is far away from a valid solution (this happens when there are a lot of classes, with potentially small counts, and when there is high overall sequence similarity in the data), moving sequences between partitions will cause some partitions to grow large at the expense of others. You can try `--no-moving` to prevent this behaviour. 
+
+
+- **I want to use a different similarity metric than sequence identity.**
+GraphPart can be used with any similarity or distance metric. To do so, you need to provide a list of precomputed pairwise similarities in the `precomputed` mode. The first two columns of the file should contain the sequence identifiers specified in the `--fasta-file`. The third column should contain the similarity metric. The `--metric-column` argument can be used to specify the column index. If you want to use a similarity metric, you need to specify a transformation using `--transformation`. See the [source](graph_part/transformations.py) for definitions. As an example, when operating with sequence identities ranging from 0 to 1, the transformation `one-minus` yields corresponding distances. If your metric is a distance, you can use `--transformation None` to skip the transformation step.
+
+- **I want to use a different alignment tool than EMBOSS needleall or MMseqs.**
+This is supported by the [precomputed](#precomputed) mode. Please refer to the answer above.
+
+- **How does the moving step decide to which partition to move a sequence to?**
+After initialization of the partitions, GraphPart iteratively moves sequences between partitions and removes sequences from the data to achieve homology separation. For each sequence, we compute how many connections it has to sequences in each other partition. If there are partitions with more connections than the current partition, the sequence is moved to the partition with the maximum number of connections. If there is a tie in the number of connections, the sequence is moved to the partition that appeared first when iterating the underlying graph data structure. We do not explicitly control this order.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `graph-part-0.1.2/graph_part.egg-info/SOURCES.txt` & `graph-part-1.0.1/graph_part.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,17 @@
+LICENSE
 README.md
 setup.py
 graph_part/__init__.py
 graph_part/__main__.py
 graph_part/api.py
 graph_part/cli.py
 graph_part/graph_part.py
 graph_part/mmseqs_fake_prefilter.sh
+graph_part/mmseqs_needle_combined_utils.py
 graph_part/mmseqs_utils.py
 graph_part/molecules.py
 graph_part/needle_utils.py
 graph_part/precomputed_utils.py
 graph_part/train_val_test_split.py
 graph_part/transformations.py
 graph_part.egg-info/PKG-INFO
```

### Comparing `graph-part-0.1.2/setup.py` & `graph-part-1.0.1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,19 +13,19 @@
 ]
 
 
 
 
 setup(
     name="graph-part",
-    version='0.1.2',
+    version='1.0.1',
     description="Graph-based partitioning of biological sequence data",
     long_description=readme,
     long_description_content_type="text/markdown",
-    url="https://healthtech.dtu.dk",
+    url="https://github.com/graph-part/graph-part",
     author="F. Teufel and M.H. Gislason",
     packages=['graph_part'],
     python_requires=">=3.6, <4",
     install_requires=requirements,
     scripts=['graph_part/mmseqs_fake_prefilter.sh'],
     entry_points = {"console_scripts":['graphpart=graph_part:run_graph_part']},
 )
```

