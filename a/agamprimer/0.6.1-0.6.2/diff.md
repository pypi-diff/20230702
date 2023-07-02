# Comparing `tmp/agamprimer-0.6.1.tar.gz` & `tmp/agamprimer-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agamprimer-0.6.1.tar", max compression
+gzip compressed data, was "agamprimer-0.6.2.tar", max compression
```

## Comparing `agamprimer-0.6.1.tar` & `agamprimer-0.6.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    35048 2023-06-01 12:44:13.709658 agamprimer-0.6.1/AgamPrimer/AgamPrimer.py
--rw-r--r--   0        0        0       66 2022-12-19 20:36:15.048061 agamprimer-0.6.1/AgamPrimer/__init__.py
--rw-r--r--   0        0        0      761 2023-05-30 16:51:46.998781 agamprimer-0.6.1/AgamPrimer/agamPrimer.egg-info/PKG-INFO
--rw-r--r--   0        0        0        0 2023-05-30 16:51:46.998781 agamprimer-0.6.1/AgamPrimer/agamPrimer.egg-info/SOURCES.txt
--rw-r--r--   0        0        0        0 2023-05-30 16:51:46.998781 agamprimer-0.6.1/AgamPrimer/agamPrimer.egg-info/dependency_links.txt
--rw-r--r--   0        0        0       11 2023-05-30 16:51:46.998781 agamprimer-0.6.1/AgamPrimer/agamPrimer.egg-info/top_level.txt
--rw-r--r--   0        0        0     1079 2022-10-08 11:18:21.612054 agamprimer-0.6.1/LICENSE
--rw-r--r--   0        0        0      730 2023-06-01 12:44:13.713658 agamprimer-0.6.1/pyproject.toml
--rw-r--r--   0        0        0      739 1970-01-01 00:00:00.000000 agamprimer-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0    35766 2023-07-02 20:25:19.636906 agamprimer-0.6.2/AgamPrimer/AgamPrimer.py
+-rw-r--r--   0        0        0       66 2022-12-19 20:36:15.048061 agamprimer-0.6.2/AgamPrimer/__init__.py
+-rw-r--r--   0        0        0      761 2023-05-30 16:51:46.998781 agamprimer-0.6.2/AgamPrimer/agamPrimer.egg-info/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-30 16:51:46.998781 agamprimer-0.6.2/AgamPrimer/agamPrimer.egg-info/SOURCES.txt
+-rw-r--r--   0        0        0        0 2023-05-30 16:51:46.998781 agamprimer-0.6.2/AgamPrimer/agamPrimer.egg-info/dependency_links.txt
+-rw-r--r--   0        0        0       11 2023-05-30 16:51:46.998781 agamprimer-0.6.2/AgamPrimer/agamPrimer.egg-info/top_level.txt
+-rw-r--r--   0        0        0     1079 2022-10-08 11:18:21.612054 agamprimer-0.6.2/LICENSE
+-rw-r--r--   0        0        0      730 2023-07-02 20:22:33.331225 agamprimer-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0      739 1970-01-01 00:00:00.000000 agamprimer-0.6.2/PKG-INFO
```

### Comparing `agamprimer-0.6.1/AgamPrimer/AgamPrimer.py` & `agamprimer-0.6.2/AgamPrimer/AgamPrimer.py`

 * *Files 2% similar despite different names*

```diff
@@ -558,14 +558,15 @@
         primer_df : pandas.DataFrame
             A pandas DataFrame containing the primer sequences and their information.
         blat_df : pandas.DataFrame
             A pandas DataFrame containing the BLAT alignment information for the primers.
     """
 
     # check target is valid for assay type and find contig
+    oligos, _ = _return_oligo_list(assay_type)
     contig, target = check_and_split_target(target=target, assay_type=assay_type)
     amplicon_size_range = [[min_amplicon_size, max_amplicon_size]]
 
     # adds some necessary parameters depending on assay type
     if primer_parameters == "default":
         primer_parameters = primer_params(
             primer_parameters=None,
@@ -608,43 +609,63 @@
             )
             print(primer3_run_statistics(primer_dict, assay_type))
             return (None, None)
 
     # AgamPrimer.primer3_run_statistics(primer_dict, assay_type)
     primer_df = primer3_to_pandas(primer_dict=primer_dict, assay_type=assay_type)
 
-    # write primer3 output to file
-    if out_dir:
-        primer_df.to_csv(f"{out_dir}/{assay_name}.{assay_type}.tsv", sep="\t")
-        primer_df.to_excel(f"{out_dir}/{assay_name}.{assay_type}.xlsx")
-
     # plot frequencies of alleles in primer pairs
     results_dict = plot_primer_ag3_frequencies(
         primer_df=primer_df,
         gdna_pos=gdna_pos,
         contig=contig,
         sample_sets=sample_sets,
         sample_query=sample_query,
         assay_type=assay_type,
         seq_parameters=seq_parameters,
         out_dir=out_dir,
     )
+
     # plot primer locations on genome
     plot_primer_locs(
         primer_res_dict=results_dict,
         primer_df=primer_df,
         assay_type=assay_type,
         contig=contig,
         seq_parameters=seq_parameters,
         legend_loc="lower left",
         out_dir=out_dir,
     )
+
+    # add genomic span to primer_df
+    spans = []
+    for oligo in oligos:
+        for i in range(len(primer_df.columns)):
+            start = int(results_dict[i][oligo]["position"].min())
+            end = int(results_dict[i][oligo]["position"].max())
+            span = f"{contig}:{start}-{end}"
+            spans.append(span)
+
+    spans = np.array(spans).reshape(len(oligos), len(primer_df.columns))
+    spans_df = pd.DataFrame(spans)
+    spans_df.index = [f"{o}_genomic_span" for o in oligos]
+    spans_df.columns = primer_df.columns
+    primer_df = pd.concat([primer_df, spans_df], axis=0).drop(
+        index=[f"primer_{o}" for o in oligos]
+    )
+
     # check primers for specificity against the genome and write to file
     blat_df = gget_blat_genome(primer_df, assay_type, assembly="anoGam3")
-    blat_df.to_csv(f"{out_dir}/{assay_name}.{assay_type}.blat.tsv", sep="\t")
+
+    # write primer3 and blat output to file
+    if out_dir:
+        primer_df.to_csv(f"{out_dir}/{assay_name}.{assay_type}.tsv", sep="\t")
+        primer_df.to_excel(f"{out_dir}/{assay_name}.{assay_type}.xlsx")
+        blat_df.to_csv(f"{out_dir}/{assay_name}.{assay_type}.blat.tsv", sep="\t")
+
     return (primer_df, blat_df)
 
 
 def _get_primer_arrays(contig, gdna_pos, sample_sets, assay_type, sample_query=None):
     if any(item in assay_type for item in ["gDNA", "probe"]):
         span_str = f"{contig}:{gdna_pos.min()}-{gdna_pos.max()}"
         snps = ag3.snp_calls(
```

### Comparing `agamprimer-0.6.1/AgamPrimer/agamPrimer.egg-info/PKG-INFO` & `agamprimer-0.6.2/AgamPrimer/agamPrimer.egg-info/PKG-INFO`

 * *Files identical despite different names*

### Comparing `agamprimer-0.6.1/LICENSE` & `agamprimer-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `agamprimer-0.6.1/pyproject.toml` & `agamprimer-0.6.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "AgamPrimer"
-version = "0.6.1"
+version = "0.6.2"
 description = "A package to design primers in Anopheles gambiae whilst considering genetic variation with malariagen_data"
 authors = [
     "Sanjay Nagi <sanjay.nagi@lstmed.ac.uk>",
     ]
 packages = [
     { include = "AgamPrimer" }
 ]
```

### Comparing `agamprimer-0.6.1/PKG-INFO` & `agamprimer-0.6.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agamprimer
-Version: 0.6.1
+Version: 0.6.2
 Summary: A package to design primers in Anopheles gambiae whilst considering genetic variation with malariagen_data
 License: MIT
 Author: Sanjay Nagi
 Author-email: sanjay.nagi@lstmed.ac.uk
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

