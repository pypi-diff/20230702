# Comparing `tmp/sincei-0.3.tar.gz` & `tmp/sincei-0.3.1.tar.gz`

## Comparing `sincei-0.3.tar` & `sincei-0.3.1.tar`

### file list

```diff
@@ -1,32 +1,39 @@
--rw-r--r--   0        0        0    12178 2020-02-02 00:00:00.000000 sincei-0.3/sincei/ExponentialFamily.py
--rw-r--r--   0        0        0     5103 2020-02-02 00:00:00.000000 sincei-0.3/sincei/FragmentFFT.py
--rw-r--r--   0        0        0     9326 2020-02-02 00:00:00.000000 sincei-0.3/sincei/GLMPCA.py
--rw-r--r--   0        0        0     4902 2020-02-02 00:00:00.000000 sincei-0.3/sincei/GetStats.py
--rw-r--r--   0        0        0    21422 2020-02-02 00:00:00.000000 sincei-0.3/sincei/ParserCommon.py
--rw-r--r--   0        0        0    52482 2020-02-02 00:00:00.000000 sincei-0.3/sincei/ReadCounter.py
--rw-r--r--   0        0        0     2835 2020-02-02 00:00:00.000000 sincei-0.3/sincei/RegionQuery.py
--rw-r--r--   0        0        0     4061 2020-02-02 00:00:00.000000 sincei-0.3/sincei/TopicModels.py
--rw-r--r--   0        0        0     8624 2020-02-02 00:00:00.000000 sincei-0.3/sincei/Utilities.py
--rw-r--r--   0        0        0    12696 2020-02-02 00:00:00.000000 sincei-0.3/sincei/WriteBedGraph.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 sincei-0.3/sincei/__init__.py
--rw-r--r--   0        0        0     6411 2020-02-02 00:00:00.000000 sincei-0.3/sincei/_deprecated.py
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 sincei-0.3/sincei/_version.py
--rw-r--r--   0        0        0     6015 2020-02-02 00:00:00.000000 sincei-0.3/sincei/multimodalClustering.py
--rwxr-xr-x   0        0        0    16039 2020-02-02 00:00:00.000000 sincei-0.3/sincei/scBAMops.py
--rwxr-xr-x   0        0        0    20499 2020-02-02 00:00:00.000000 sincei-0.3/sincei/scBulkCoverage.py
--rwxr-xr-x   0        0        0     7812 2020-02-02 00:00:00.000000 sincei-0.3/sincei/scClusterCells.py
--rwxr-xr-x   0        0        0     4748 2020-02-02 00:00:00.000000 sincei-0.3/sincei/scCombineCounts.py
--rwxr-xr-x   0        0        0     9502 2020-02-02 00:00:00.000000 sincei-0.3/sincei/scCountQC.py
--rwxr-xr-x   0        0        0     8048 2020-02-02 00:00:00.000000 sincei-0.3/sincei/scCountReads.py
--rwxr-xr-x   0        0        0     7377 2020-02-02 00:00:00.000000 sincei-0.3/sincei/scFilterBarcodes.py
--rwxr-xr-x   0        0        0    11377 2020-02-02 00:00:00.000000 sincei-0.3/sincei/scFilterStats.py
--rwxr-xr-x   0        0        0     5176 2020-02-02 00:00:00.000000 sincei-0.3/sincei/scJSD.py
--rwxr-xr-x   0        0        0      385 2020-02-02 00:00:00.000000 sincei-0.3/sincei/scPlotRegion
--rwxr-xr-x   0        0        0     2126 2020-02-02 00:00:00.000000 sincei-0.3/sincei/sincei.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sincei-0.3/sincei/test/__init__.py
--rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 sincei-0.3/sincei/test/test_tools.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 sincei-0.3/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 sincei-0.3/LICENCE.txt
--rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 sincei-0.3/README.md
--rw-r--r--   0        0        0     2584 2020-02-02 00:00:00.000000 sincei-0.3/pyproject.toml
--rw-r--r--   0        0        0     4279 2020-02-02 00:00:00.000000 sincei-0.3/PKG-INFO
+-rw-r--r--   0        0        0    12178 2020-02-02 00:00:00.000000 sincei-0.3.1/sincei/ExponentialFamily.py
+-rw-r--r--   0        0        0     5103 2020-02-02 00:00:00.000000 sincei-0.3.1/sincei/FragmentFFT.py
+-rw-r--r--   0        0        0     9326 2020-02-02 00:00:00.000000 sincei-0.3.1/sincei/GLMPCA.py
+-rw-r--r--   0        0        0     4902 2020-02-02 00:00:00.000000 sincei-0.3.1/sincei/GetStats.py
+-rw-r--r--   0        0        0    21596 2020-02-02 00:00:00.000000 sincei-0.3.1/sincei/ParserCommon.py
+-rw-r--r--   0        0        0    52460 2020-02-02 00:00:00.000000 sincei-0.3.1/sincei/ReadCounter.py
+-rw-r--r--   0        0        0     2835 2020-02-02 00:00:00.000000 sincei-0.3.1/sincei/RegionQuery.py
+-rw-r--r--   0        0        0     4041 2020-02-02 00:00:00.000000 sincei-0.3.1/sincei/TopicModels.py
+-rw-r--r--   0        0        0     8770 2020-02-02 00:00:00.000000 sincei-0.3.1/sincei/Utilities.py
+-rw-r--r--   0        0        0    12696 2020-02-02 00:00:00.000000 sincei-0.3.1/sincei/WriteBedGraph.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 sincei-0.3.1/sincei/__init__.py
+-rw-r--r--   0        0        0     6411 2020-02-02 00:00:00.000000 sincei-0.3.1/sincei/_deprecated.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 sincei-0.3.1/sincei/_version.py
+-rw-r--r--   0        0        0     6015 2020-02-02 00:00:00.000000 sincei-0.3.1/sincei/multimodalClustering.py
+-rwxr-xr-x   0        0        0    16039 2020-02-02 00:00:00.000000 sincei-0.3.1/sincei/scBAMops.py
+-rwxr-xr-x   0        0        0    20515 2020-02-02 00:00:00.000000 sincei-0.3.1/sincei/scBulkCoverage.py
+-rwxr-xr-x   0        0        0     7812 2020-02-02 00:00:00.000000 sincei-0.3.1/sincei/scClusterCells.py
+-rwxr-xr-x   0        0        0     4651 2020-02-02 00:00:00.000000 sincei-0.3.1/sincei/scCombineCounts.py
+-rwxr-xr-x   0        0        0     9502 2020-02-02 00:00:00.000000 sincei-0.3.1/sincei/scCountQC.py
+-rwxr-xr-x   0        0        0     8114 2020-02-02 00:00:00.000000 sincei-0.3.1/sincei/scCountReads.py
+-rwxr-xr-x   0        0        0     7377 2020-02-02 00:00:00.000000 sincei-0.3.1/sincei/scFilterBarcodes.py
+-rwxr-xr-x   0        0        0    11588 2020-02-02 00:00:00.000000 sincei-0.3.1/sincei/scFilterStats.py
+-rwxr-xr-x   0        0        0     5176 2020-02-02 00:00:00.000000 sincei-0.3.1/sincei/scJSD.py
+-rwxr-xr-x   0        0        0      385 2020-02-02 00:00:00.000000 sincei-0.3.1/sincei/scPlotRegion
+-rwxr-xr-x   0        0        0     2126 2020-02-02 00:00:00.000000 sincei-0.3.1/sincei/sincei.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sincei-0.3.1/sincei/tests/__init__.py
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 sincei-0.3.1/sincei/tests/test_tools.py
+-rw-r--r--   0        0        0    23597 2020-02-02 00:00:00.000000 sincei-0.3.1/sincei/tests/_data/Ogfrl.gtf
+-rw-r--r--   0        0        0     6634 2020-02-02 00:00:00.000000 sincei-0.3.1/sincei/tests/_data/SL2-1.bam
+-rw-r--r--   0        0        0    13392 2020-02-02 00:00:00.000000 sincei-0.3.1/sincei/tests/_data/SL2-1.bam.bai
+-rw-r--r--   0        0        0     6035 2020-02-02 00:00:00.000000 sincei-0.3.1/sincei/tests/_data/SL2-2.bam
+-rw-r--r--   0        0        0    13368 2020-02-02 00:00:00.000000 sincei-0.3.1/sincei/tests/_data/SL2-2.bam.bai
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 sincei-0.3.1/sincei/tests/_data/test_barcodes.txt
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 sincei-0.3.1/sincei/tests/_data/test_regions.bed
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 sincei-0.3.1/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 sincei-0.3.1/LICENCE.txt
+-rw-r--r--   0        0        0     2292 2020-02-02 00:00:00.000000 sincei-0.3.1/README.md
+-rw-r--r--   0        0        0     2604 2020-02-02 00:00:00.000000 sincei-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     5062 2020-02-02 00:00:00.000000 sincei-0.3.1/PKG-INFO
```

### Comparing `sincei-0.3/sincei/ExponentialFamily.py` & `sincei-0.3.1/sincei/ExponentialFamily.py`

 * *Files identical despite different names*

### Comparing `sincei-0.3/sincei/FragmentFFT.py` & `sincei-0.3.1/sincei/FragmentFFT.py`

 * *Files identical despite different names*

### Comparing `sincei-0.3/sincei/GLMPCA.py` & `sincei-0.3.1/sincei/GLMPCA.py`

 * *Files identical despite different names*

### Comparing `sincei-0.3/sincei/GetStats.py` & `sincei-0.3.1/sincei/GetStats.py`

 * *Files identical despite different names*

### Comparing `sincei-0.3/sincei/ParserCommon.py` & `sincei-0.3.1/sincei/ParserCommon.py`

 * *Files 1% similar despite different names*

```diff
@@ -293,15 +293,15 @@
         "-m",
         metavar="STR",
         help=show_or_hide(
             "Check whether a given motif is present in the read and the corresponding reference genome. "
             "This option checks for the motif at the 5-end of the read and at the 5-overhang in the genome, "
             "which is useful in identifying reads properly cut by a restriction-enzyme or MNAse. "
             'For example, if you want to search for an "A" at the 5\'-end of the read and "TA" at 5\'-overhang, '
-            "use \"-m 'A,TA'\". Reads not containing the given motif are discarded. ",
+            "use \"-m 'A,TA'\". Reads not containing the given motif are filtered out. ",
             "motifFilter",
             suppress_args,
         ),
         type=str,
         nargs="+",
         default=None,
     )
@@ -320,16 +320,18 @@
     )
 
     group.add_argument(
         "--GCcontentFilter",
         "-gc",
         metavar="STR",
         help=show_or_hide(
-            "Check whether the GC content of the read falls within the provided range. "
-            "If the GC content of the reads fall outside the range, they are discarded. ",
+            "Check whether the GC content of the read falls within the provided range "
+            "Input format must be '<low>,<high>' , where <low> is the lower bound and <high> is the "
+            "upper bound in the fraction of GC (eg. '0.1,0.9' ). "
+            "If the GC content of the reads fall outside the range, they are filtered out. ",
             "GCcontentFilter",
             suppress_args,
         ),
         type=str,
         default=None,
     )
```

### Comparing `sincei-0.3/sincei/ReadCounter.py` & `sincei-0.3.1/sincei/ReadCounter.py`

 * *Files 0% similar despite different names*

```diff
@@ -661,15 +661,15 @@
         ## prepare list of regions
         regionList = []
         idx = 0
         for i, trans in enumerate(transcriptsToConsider):
             if regionNames is not None:
                 bedname = regionNames[i]
             else:
-                bedname = ""
+                bedname = None
 
             if len(trans[0]) != 3:
                 starts = ",".join([str(x[0]) for x in trans])
                 ends = ",".join([str(x[1]) for x in trans])
                 name = "{}_{}_{}::{}".format(chrom, starts, ends, bedname)
                 regionList.append(name)
                 # _file.write(name + "\n")
@@ -888,18 +888,19 @@
                 if bc not in self.barcodes:
                     if self.verbose:
                         print("Encountered barcode: {}, not in provided whitelist. skipping..".format(bc))
                     continue
                 # get rid of duplicate reads with same barcode, startpos and optionally, endpos/umi
                 if self.duplicateFilter:
                     tup = getDupFilterTuple(read, new_bc, self.duplicateFilter)
-                    if lpos is not None and lpos == read.reference_start and tup in prev_pos:
-                        continue
-                    if lpos != read.reference_start:
-                        prev_pos.clear()
+                    if lpos is not None:
+                        if tup in prev_pos:
+                            continue
+                        else:
+                            prev_pos.clear()
                     lpos = read.reference_start
                     prev_pos.add(tup)
 
                 # since reads can be split (e.g. RNA-seq reads) each part of the
                 # read that maps is called a position block.
                 try:
                     position_blocks = fragmentFromRead_func(read)
```

### Comparing `sincei-0.3/sincei/RegionQuery.py` & `sincei-0.3.1/sincei/RegionQuery.py`

 * *Files identical despite different names*

### Comparing `sincei-0.3/sincei/TopicModels.py` & `sincei-0.3.1/sincei/TopicModels.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 # topic models
 import numpy as np
 import pandas as pd
-import scanpy as sc
 from gensim import corpora, matutils, models
 import copy
 
 # Louvain clustering and UMAP
 from networkx import convert_matrix
 from sklearn.metrics import pairwise_distances
 import leidenalg as la
```

### Comparing `sincei-0.3/sincei/Utilities.py` & `sincei-0.3.1/sincei/Utilities.py`

 * *Files 2% similar despite different names*

```diff
@@ -209,15 +209,15 @@
             "#9b2532",
         ],
     }
 
     return colors[name]
 
 
-def getDupFilterTuple(read, bc, filter):
+def getDupFilterTuple(read, bc, filterArg):
     r"""
     Returns a tuple with the information needed to filter duplicates, based on read and filter type.
     The tuple is composed of the barcode, the umi, the start and end positions
     and the chromosome name.
 
     Parameters
     ----------
@@ -244,37 +244,44 @@
     >>> test = Tester()
     >>> read = test.bamFile1.fetch().next()
     >>> getDupFilterTuple(read, 'ATCG', 'end_umi')
     ('ATCG', 'ATCG', None, None, 0, False)
     """
 
     tLenDup = getTLen(read, notAbs=True)
-    filt = filter.split("_")
-    ## get read (or fragment) start/end
+    filt = filterArg.split("_")
+
     # get fragment start and end for that read
     if tLenDup >= 0:
         s = read.pos
         e = s + tLenDup
     else:
         s = read.pnext
         e = s - tLenDup
-    if read.reference_id != read.next_reference_id:
-        e = read.pnext
+
     if "end" not in filt:
-        # use only read (or fragment) start
+        # ignore read/fragment end and mate information
+        mate_refid = read.reference_id
         if read.is_reverse:
             s = None
         else:
             e = None
-    ## get UMI if asked
+    else:
+        # use mate info, reset fragment end to mate pos if read is chimeric
+        if read.reference_id != read.next_reference_id:
+            e = read.pnext
+        mate_refid = read.next_reference_id
+
+    # get UMI if asked
     if "umi" in filt:
         umi = read.get_tag("RX")
     else:
         umi = None
-    tup = (bc, umi, s, e, read.next_reference_id, read.is_reverse)
+
+    tup = (bc, umi, s, e, mate_refid, read.is_reverse)
     return tup
 
 
 def gini(i, X):
     r"""Computes the Gini coefficient for each row of a sparse matrix (Obs*Var).
 
     Parameters
```

### Comparing `sincei-0.3/sincei/WriteBedGraph.py` & `sincei-0.3.1/sincei/WriteBedGraph.py`

 * *Files identical despite different names*

### Comparing `sincei-0.3/sincei/_deprecated.py` & `sincei-0.3.1/sincei/_deprecated.py`

 * *Files identical despite different names*

### Comparing `sincei-0.3/sincei/multimodalClustering.py` & `sincei-0.3.1/sincei/multimodalClustering.py`

 * *Files identical despite different names*

### Comparing `sincei-0.3/sincei/scBAMops.py` & `sincei-0.3.1/sincei/scBAMops.py`

 * *Files identical despite different names*

### Comparing `sincei-0.3/sincei/scBulkCoverage.py` & `sincei-0.3.1/sincei/scBulkCoverage.py`

 * *Files 0% similar despite different names*

```diff
@@ -142,28 +142,30 @@
     global debug
     if args.verbose:
         sys.stderr.write("Specified --scaleFactor: {}\n".format(args.scaleFactor))
         debug = 1
     else:
         debug = 0
 
-    ## read the group info file (make it more robust)
+    ## read the group info file (TODO: write a validator)
+    df_err = """ *Error*:No. of columns in --groupInfo file not recognized.
+             Please provide either 3 (sample, barcode, group) or 4 (sample::barcode, umap1, umap2, group) column file"""
     ## if the no. of columns are 3, expect "sample", "barcode", "cluster", if 4, expect sample:bc, umap1, umap2, cluster
     df = pd.read_csv(args.groupInfo, sep="\t", index_col=None, comment="#")
     if len(df.columns) == 3:
         df.columns = ["sample", "barcode", "cluster"]
     elif len(df.columns) == 4:
-        df.columns = ["barcode", "umap1", "umap2", "cluster"]
-        df["sample"] = [x.split("::")[:-1] for x in df.barcode]
-        df["barcode"] = [x.split("::")[-1] for x in df.barcode]
+        df.columns = ["Cell_ID", "umap1", "umap2", "cluster"]
+        try:
+            df[["sample", "barcode"]] = df.Cell_ID.str.split("::", expand=True)
+        except:
+            sys.exit(df_err)
     else:
-        sys.exit(
-            "*Error*:No. of columns in --groupInfo file not recognized. "
-            "Please provide either 3 (sample, barcode, group) or 4 (sample::barcode, umap1, umap2, group) column file"
-        )
+        sys.exit(df_err)
+
     df.index = df[["sample", "barcode"]].apply(lambda x: "::".join(x), axis=1)
     # barcodes = groupInfo.barcode.unique().tolist()
 
     ## match the sample labels with groupInfo labels before proceeding
     ## create new DF with user-provided bam+labels (this would match the counts)
 
     # check that sample names in df and --labels match
```

### Comparing `sincei-0.3/sincei/scClusterCells.py` & `sincei-0.3.1/sincei/scClusterCells.py`

 * *Files 0% similar despite different names*

```diff
@@ -200,15 +200,15 @@
     if args.outFileUMAP:
         ## plot UMAP
         fig = sc.pl.umap(adata, color="leiden", legend_loc="on data", return_fig=True, show=False)
         fig.savefig(args.outFileUMAP, dpi=200, format=args.plotFileFormat)
         prefix = args.outFileUMAP.split(".")[0]
         umap_lsi = pd.DataFrame(adata.obsm["X_umap"], columns=["UMAP1", "UMAP2"], index=adata.obs.index)
         umap_lsi["cluster"] = adata.obs["leiden"]
-        umap_lsi.to_csv(prefix + ".tsv", sep="\t", index_label="cell_id")
+        umap_lsi.to_csv(prefix + ".tsv", sep="\t", index_label="Cell_ID")
         # plt.rcParams['font.size'] = 8.0
         # convert cm values to inches
         # fig = plt.figure(figsize=(args.plotWidth / 2.54, args.plotHeight / 2.54))
         # fig.suptitle('LSA-UMAP', y=(1 - (0.06 / args.plotHeight)))
         # plt.scatter(umap_lsi.UMAP1, umap_lsi.UMAP2, s=5, alpha = 0.8, c=[sns.color_palette()[x] for x in list(umap_lsi.cluster)])
         # plt.tight_layout()
         # plt.savefig(args.outFileUMAP, dpi=200, format=args.plotFileFormat)
```

### Comparing `sincei-0.3/sincei/scCombineCounts.py` & `sincei-0.3.1/sincei/scCombineCounts.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,18 +97,15 @@
         sys.stderr.write("Only multi-sample method is currently implemented")
         sys.exit(1)
 
     if args.labels and len(args.input) != len(args.labels):
         print("The number of labels does not match the number of input files.")
         sys.exit(1)
     if not args.labels:
-        if args.smartLabels:
-            args.labels = smartLabels(args.input)
-        else:
-            args.labels = [os.path.basename(x) for x in args.input]
+        args.labels = [os.path.basename(x) for x in args.input]
     adata_list = [sc.read_loom(x, obs_names="obs_names", var_names="var_names") for x in args.input]
 
     ## concatenate labels and match chrom, start, end
     var_list = []
     var_cols = ["chrom", "start", "end"]
     for lab, ad in zip(args.labels, adata_list):
         obs = ad.obs_names.to_list()
```

### Comparing `sincei-0.3/sincei/scCountQC.py` & `sincei-0.3.1/sincei/scCountQC.py`

 * *Files 1% similar despite different names*

```diff
@@ -194,16 +194,16 @@
     gini_list = [gini(i, adata.X) for i in range(adata.shape[0])]
     adata.obs["gini_coefficient"] = gini_list
 
     if args.outMetrics:
         mat = re.sub(".txt|.tsv|.csv", "", args.outMetrics)
         obs_tsv = mat + ".cells.tsv"
         var_tsv = mat + ".regions.tsv"
-        adata.obs.to_csv(obs_tsv, sep="\t", index_label="cell_id")
-        adata.var.to_csv(var_tsv, sep="\t", index_label="feature_id")
+        adata.obs.to_csv(obs_tsv, sep="\t", index_label="Cell_ID")
+        adata.var.to_csv(var_tsv, sep="\t", index_label="Feature_ID")
 
     # if --describe is asked, only print the numeric vars and obs columns
     if args.describe:
         is_num_col = [(pd.api.types.is_float_dtype(x) | pd.api.types.is_integer_dtype(x)) for x in adata.obs.dtypes]
         cols = adata.obs.loc[:, is_num_col]
         sys.stdout.write("\n Cell metrics: \n")
         sys.stdout.write("Total cells: {} \n".format(adata.shape[0]))
```

### Comparing `sincei-0.3/sincei/scCountReads.py` & `sincei-0.3.1/sincei/scCountReads.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 import sys
 import argparse
 import numpy as np
 from scipy import sparse, io
 import re
 import pandas as pd
 import anndata as ad
-import scanpy as sc
 from deeptools import parserCommon
 from deeptools.utilities import smartLabels
 import warnings
 
 warnings.simplefilter(action="ignore", category=FutureWarning)
 
 # own functions
@@ -225,14 +224,15 @@
 
         rows = list(regionList)
 
         adata.var = pd.DataFrame(
             {
                 "chrom": [x.split("_")[0] for x in rows],
                 "start": [x.split("_")[1] for x in rows],
-                "end": [x.split("_")[2] for x in rows],
+                "end": [y.split("::")[0] for y in [x.split("_")[2] for x in rows]],
+                "name": [x.split("::")[1] for x in rows],
             },
             index=rows,
         )
 
         # export as loom
         adata.write_loom(args.outFilePrefix + ".loom")
```

### Comparing `sincei-0.3/sincei/scFilterBarcodes.py` & `sincei-0.3.1/sincei/scFilterBarcodes.py`

 * *Files identical despite different names*

### Comparing `sincei-0.3/sincei/scFilterStats.py` & `sincei-0.3.1/sincei/scFilterStats.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 
 def parseArguments():
     filterParser = ParserCommon.filterOptions()
 
     io_args = ParserCommon.inputOutputOptions(opts=["bamfiles", "barcodes", "outFile"], requiredOpts=["barcodes"])
     bam_args = ParserCommon.bamOptions(
-        suppress_args=["region"],
+        suppress_args=["region", "groupTag"],
         default_opts={"binSize": 100000, "distanceBetweenBins": 1000000},
     )
     filter_args = ParserCommon.filterOptions()
     read_args = ParserCommon.readOptions(
         suppress_args=[
             "minFragmentLength",
             "maxFragmentLength",
@@ -110,27 +110,27 @@
         minAlignedFraction = {}
         # trackers
         nFiltered = {}
         total = {}  # This is only used to estimate the percentage affected
         filtered = {}
 
         for b in args.barcodes:
+            total[b] = 0  # This is only used to estimate the percentage affected
+            nFiltered[b] = 0
             blacklisted[b] = 0
             minMapq[b] = 0
             samFlagInclude[b] = 0
             samFlagExclude[b] = 0
             internalDupes[b] = 0
             externalDupes[b] = 0
             singletons[b] = 0
             filterRNAstrand[b] = 0
             filterMotifs[b] = 0
             filterGC[b] = 0
             minAlignedFraction[b] = 0
-            nFiltered[b] = 0
-            total[b] = 0  # This is only used to estimate the percentage affected
 
         for read in fh.fetch(chromUse, start, end):
             bc = read.get_tag(args.cellTag)
             # also keep a counter for barcodes not in whitelist?
             if bc not in args.barcodes:
                 continue
 
@@ -271,15 +271,20 @@
     for bam in args.bamfiles:
         x = bamHandler.openBam(bam, returnStats=True, nThreads=args.numberOfProcessors)[0]
         chrom_sizes = list(zip(x.references, x.lengths))
 
         checkBAMtag(x, bam, args.cellTag)
         if args.groupTag:
             checkBAMtag(x, bam, args.groupTag)
-            sys.stderr.write("--groupTag is not implemented for scFilterStats yet! \n")
+            sys.stderr.write(
+                "--groupTag is not implemented for scFilterStats yet! \
+            Please split your BAM file by {} and re-run scFilterStats. \n".format(
+                    args.groupTag
+                )
+            )
             exit(1)
         x.close()
 
     # Get the remaining metrics
     res = mapReduce(
         [args],
         getFiltered_worker,
@@ -307,14 +312,15 @@
         "Wrong_strand",
         "Wrong_motif",
         "Unwanted_GC_content",
         "Low_aligned_fraction",
     ]
 
     final_df = pd.DataFrame(data=np.concatenate(final_array), index=rowLabels, columns=colLabels)
+    final_df.index.name = "Cell_ID"
     ## since stats are approximate, present results as %
     final_df.iloc[:, 1:] = final_df.iloc[:, 1:].div(final_df.Total_sampled, axis=0) * 100
 
     if args.outFile is not None:
         final_df.to_csv(args.outFile, sep="\t")
     else:
         print(final_df)
```

### Comparing `sincei-0.3/sincei/scJSD.py` & `sincei-0.3.1/sincei/scJSD.py`

 * *Files identical despite different names*

### Comparing `sincei-0.3/sincei/sincei.py` & `sincei-0.3.1/sincei/sincei.py`

 * *Files identical despite different names*

### Comparing `sincei-0.3/LICENCE.txt` & `sincei-0.3.1/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `sincei-0.3/README.md` & `sincei-0.3.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,45 @@
 
 ## sincei: A user-friendly toolkit for QC, counting, clustering and plotting of single-cell (epi)genomics data.
 
 [![DOI](https://zenodo.org/badge/271841139.svg)](https://zenodo.org/badge/latestdoi/271841139) [![Documentation Status](https://readthedocs.org/projects/sincei/badge/?version=latest)](https://sincei.readthedocs.io/en/latest/?badge=latest) [![PyPI Version](https://img.shields.io/pypi/v/sincei.svg?style=plastic)](https://pypi.org/project/sincei/) [![test](https://github.com/vivekbhr/sincei/actions/workflows/test.yml/badge.svg)](https://github.com/vivekbhr/sincei/actions/workflows/test.yml) [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
-## [Full Documentation](http://sincei.rtfd.io/).
+## Features
+
+sincei provides a flexible, easy-to-use command-line interface to work with single-cell data directly from BAM files. It can:
+
+ - Aggregate signal in bins, genes or any feature of interest from single-cells.
+ - Perform read-level and count-level quality control.
+ - Perform dimentionality reduction and clustering of all kinds of single-cell data (open chromatin, histone marks, methylation, gene expression etc..).
+ - Create coverage files (bigwigs) for visualization.
+
+## [Full Documentation](http://sincei.rtfd.io/)
 
 ## Installation
 
 sincei is a command line toolkit based on python3, and can be installed using [conda](https://conda.io/projects/conda/en/latest/user-guide/install/index.html).
 
 Create a new conda environment and install sincei stable release from github using:
 
 ```
 conda create -n sincei -c anaconda python=3.8
 conda activate sincei
-(sincei): pip install sincei
+(sincei): pip install --editable=git+https://github.com/vivekbhr/sincei.git@master#egg=sincei
 ```
 
-For the latest development version, try:
+For the development version, try:
 
 ```
-(sincei): pip install git+https://github.com/vivekbhr/sincei.git@develop#egg=sincei
+(sincei): pip install --editable=git+https://github.com/vivekbhr/sincei.git@develop#egg=sincei
 ```
 
 ## Usage
 
 **Get the tool list with `sincei --help`**
 
 Each tool begins with the prefix sc<tool_name>, such as:
 
- $ scBulkCoverage -b file1.bam -i groupinfo.txt -o coverage
+ $ scBulkCoverage -b file1.bam -g groupinfo.txt -o coverage
 
+## Questions and discussions
 
+To ask  a question related to sincei or start a new discussion, please use our [github discussion forum](https://github.com/vivekbhr/sincei/discussions).
```

### Comparing `sincei-0.3/pyproject.toml` & `sincei-0.3.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -65,14 +65,15 @@
     "sphinx>=4",
     "sphinx-book-theme>=0.3.3",
     "myst-nb",
     "sphinxcontrib-bibtex>=1.0.0",
     "sphinx-autodoc-typehints",
     "readthedocs-sphinx-ext",
     "sphinx-argparse",
+    "sphinx_toolbox"
     # For notebooks
  #   "ipykernel",
  #   "ipython",
  #   "sphinx-copybutton",
 ]
 test = [
     "pytest"
@@ -118,8 +119,7 @@
     | _build
     | buck-out
     | build
     | dist
   )/
 )
 '''
-
```

### Comparing `sincei-0.3/PKG-INFO` & `sincei-0.3.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sincei
-Version: 0.3
+Version: 0.3.1
 Summary: A user-friendly toolkit for QC, counting, clustering and plotting of single-cell (epi)genomics data 
 Project-URL: Documentation, https://sincei.readthedocs.io/
 Project-URL: Source, https://github.com/vivekbhr/sincei
 Project-URL: Home-page, https://github.com/vivekbhr/sincei
 Author: Vivek Bhardwaj
 Maintainer-email: Vivek Bhardwaj <vivbhr@gmail.com>
 License: MIT license:
@@ -41,47 +41,59 @@
 Requires-Dist: twine>=4.0.2; extra == 'dev'
 Provides-Extra: doc
 Requires-Dist: myst-nb; extra == 'doc'
 Requires-Dist: readthedocs-sphinx-ext; extra == 'doc'
 Requires-Dist: sphinx-argparse; extra == 'doc'
 Requires-Dist: sphinx-autodoc-typehints; extra == 'doc'
 Requires-Dist: sphinx-book-theme>=0.3.3; extra == 'doc'
+Requires-Dist: sphinx-toolbox; extra == 'doc'
 Requires-Dist: sphinx>=4; extra == 'doc'
 Requires-Dist: sphinxcontrib-bibtex>=1.0.0; extra == 'doc'
 Provides-Extra: test
 Requires-Dist: pytest; extra == 'test'
 Description-Content-Type: text/markdown
 
 
 ## sincei: A user-friendly toolkit for QC, counting, clustering and plotting of single-cell (epi)genomics data.
 
 [![DOI](https://zenodo.org/badge/271841139.svg)](https://zenodo.org/badge/latestdoi/271841139) [![Documentation Status](https://readthedocs.org/projects/sincei/badge/?version=latest)](https://sincei.readthedocs.io/en/latest/?badge=latest) [![PyPI Version](https://img.shields.io/pypi/v/sincei.svg?style=plastic)](https://pypi.org/project/sincei/) [![test](https://github.com/vivekbhr/sincei/actions/workflows/test.yml/badge.svg)](https://github.com/vivekbhr/sincei/actions/workflows/test.yml) [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
-## [Full Documentation](http://sincei.rtfd.io/).
+## Features
+
+sincei provides a flexible, easy-to-use command-line interface to work with single-cell data directly from BAM files. It can:
+
+ - Aggregate signal in bins, genes or any feature of interest from single-cells.
+ - Perform read-level and count-level quality control.
+ - Perform dimentionality reduction and clustering of all kinds of single-cell data (open chromatin, histone marks, methylation, gene expression etc..).
+ - Create coverage files (bigwigs) for visualization.
+
+## [Full Documentation](http://sincei.rtfd.io/)
 
 ## Installation
 
 sincei is a command line toolkit based on python3, and can be installed using [conda](https://conda.io/projects/conda/en/latest/user-guide/install/index.html).
 
 Create a new conda environment and install sincei stable release from github using:
 
 ```
 conda create -n sincei -c anaconda python=3.8
 conda activate sincei
-(sincei): pip install sincei
+(sincei): pip install --editable=git+https://github.com/vivekbhr/sincei.git@master#egg=sincei
 ```
 
-For the latest development version, try:
+For the development version, try:
 
 ```
-(sincei): pip install git+https://github.com/vivekbhr/sincei.git@develop#egg=sincei
+(sincei): pip install --editable=git+https://github.com/vivekbhr/sincei.git@develop#egg=sincei
 ```
 
 ## Usage
 
 **Get the tool list with `sincei --help`**
 
 Each tool begins with the prefix sc<tool_name>, such as:
 
- $ scBulkCoverage -b file1.bam -i groupinfo.txt -o coverage
+ $ scBulkCoverage -b file1.bam -g groupinfo.txt -o coverage
 
+## Questions and discussions
 
+To ask  a question related to sincei or start a new discussion, please use our [github discussion forum](https://github.com/vivekbhr/sincei/discussions).
```

