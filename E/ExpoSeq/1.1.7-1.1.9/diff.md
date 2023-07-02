# Comparing `tmp/ExpoSeq-1.1.7.tar.gz` & `tmp/ExpoSeq-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ExpoSeq-1.1.7.tar", last modified: Tue Jun 27 08:06:35 2023, max compression
+gzip compressed data, was "ExpoSeq-1.1.9.tar", last modified: Sun Jul  2 11:46:32 2023, max compression
```

## Comparing `ExpoSeq-1.1.7.tar` & `ExpoSeq-1.1.9.tar`

### file list

```diff
@@ -1,91 +1,91 @@
-drwxrwxrwx   0        0        0        0 2023-06-27 08:06:35.436818 ExpoSeq-1.1.7/
--rw-rw-rw-   0        0        0     1090 2023-05-30 20:50:39.000000 ExpoSeq-1.1.7/LICENSE
--rw-rw-rw-   0        0        0       59 2023-05-30 20:50:39.000000 ExpoSeq-1.1.7/MANIFEST.in
--rw-rw-rw-   0        0        0     4091 2023-06-27 08:06:35.436818 ExpoSeq-1.1.7/PKG-INFO
--rw-rw-rw-   0        0        0     3725 2023-05-30 20:50:39.000000 ExpoSeq-1.1.7/README.md
--rw-rw-rw-   0        0        0       42 2023-06-27 08:06:35.436818 ExpoSeq-1.1.7/setup.cfg
--rw-rw-rw-   0        0        0     1320 2023-06-27 07:58:35.000000 ExpoSeq-1.1.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-27 08:06:35.151687 ExpoSeq-1.1.7/src/
-drwxrwxrwx   0        0        0        0 2023-06-27 08:06:35.183124 ExpoSeq-1.1.7/src/ExpoSeq/
--rw-rw-rw-   0        0        0        0 2023-06-12 12:03:02.000000 ExpoSeq-1.1.7/src/ExpoSeq/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-27 08:06:35.230135 ExpoSeq-1.1.7/src/ExpoSeq/augment_data/
--rw-rw-rw-   0        0        0        0 2023-06-12 12:03:02.000000 ExpoSeq-1.1.7/src/ExpoSeq/augment_data/__init__.py
--rw-rw-rw-   0        0        0     1007 2023-06-12 12:03:02.000000 ExpoSeq-1.1.7/src/ExpoSeq/augment_data/binding_data.py
--rw-rw-rw-   0        0        0      858 2023-06-12 12:03:02.000000 ExpoSeq-1.1.7/src/ExpoSeq/augment_data/check_reports.py
--rw-rw-rw-   0        0        0      913 2023-06-12 12:03:02.000000 ExpoSeq-1.1.7/src/ExpoSeq/augment_data/load_data.py
--rw-rw-rw-   0        0        0     4616 2023-06-12 12:03:02.000000 ExpoSeq-1.1.7/src/ExpoSeq/augment_data/loop_collect_reports.py
--rw-rw-rw-   0        0        0     7915 2023-06-12 12:03:02.000000 ExpoSeq-1.1.7/src/ExpoSeq/augment_data/mixcr_cl.py
--rw-rw-rw-   0        0        0    10406 2023-06-12 12:03:02.000000 ExpoSeq-1.1.7/src/ExpoSeq/augment_data/mixcr_nils.py
--rw-rw-rw-   0        0        0     6830 2023-06-22 09:23:10.000000 ExpoSeq-1.1.7/src/ExpoSeq/augment_data/randomizer.py
--rw-rw-rw-   0        0        0      580 2023-06-12 12:03:02.000000 ExpoSeq-1.1.7/src/ExpoSeq/augment_data/read_raw_data.py
--rw-rw-rw-   0        0        0     3646 2023-06-12 12:03:02.000000 ExpoSeq-1.1.7/src/ExpoSeq/augment_data/structure_files.py
--rw-rw-rw-   0        0        0      519 2023-06-12 12:03:02.000000 ExpoSeq-1.1.7/src/ExpoSeq/augment_data/trimming.py
--rw-rw-rw-   0        0        0    17254 2023-06-16 09:31:36.000000 ExpoSeq-1.1.7/src/ExpoSeq/augment_data/uploader.py
--rw-rw-rw-   0        0        0    10290 2023-06-12 12:16:56.000000 ExpoSeq-1.1.7/src/ExpoSeq/full_pipe.py
--rw-rw-rw-   0        0        0    36600 2023-06-22 09:17:03.000000 ExpoSeq-1.1.7/src/ExpoSeq/pipeline.py
-drwxrwxrwx   0        0        0        0 2023-06-27 08:06:35.279743 ExpoSeq-1.1.7/src/ExpoSeq/plots/
--rw-rw-rw-   0        0        0        0 2023-06-12 12:03:02.000000 ExpoSeq-1.1.7/src/ExpoSeq/plots/__init__.py
--rw-rw-rw-   0        0        0     2061 2023-06-12 12:03:02.000000 ExpoSeq-1.1.7/src/ExpoSeq/plots/barplot.py
--rw-rw-rw-   0        0        0     1666 2023-06-12 12:03:02.000000 ExpoSeq-1.1.7/src/ExpoSeq/plots/cluster_embedding.py
--rw-rw-rw-   0        0        0     4363 2023-06-12 12:03:02.000000 ExpoSeq-1.1.7/src/ExpoSeq/plots/embedding_with_binding.py
--rw-rw-rw-   0        0        0     3444 2023-06-12 12:03:02.000000 ExpoSeq-1.1.7/src/ExpoSeq/plots/length_distribution.py
--rw-rw-rw-   0        0        0     7669 2023-06-12 12:03:02.000000 ExpoSeq-1.1.7/src/ExpoSeq/plots/levenshtein_clustering.py
--rw-rw-rw-   0        0        0     4379 2023-06-12 12:03:02.000000 ExpoSeq-1.1.7/src/ExpoSeq/plots/logo_plot.py
--rw-rw-rw-   0        0        0     3383 2023-06-16 09:49:51.000000 ExpoSeq-1.1.7/src/ExpoSeq/plots/plt_heatmap.py
--rw-rw-rw-   0        0        0     2524 2023-06-12 12:03:02.000000 ExpoSeq-1.1.7/src/ExpoSeq/plots/protvec.py
--rw-rw-rw-   0        0        0     1470 2023-06-12 12:03:02.000000 ExpoSeq-1.1.7/src/ExpoSeq/plots/relative_sequence_abundance.py
--rw-rw-rw-   0        0        0     1634 2023-06-12 12:03:02.000000 ExpoSeq-1.1.7/src/ExpoSeq/plots/saveFig.py
--rw-rw-rw-   0        0        0     1064 2023-06-12 12:03:02.000000 ExpoSeq-1.1.7/src/ExpoSeq/plots/stacked_aa_distribution.py
--rw-rw-rw-   0        0        0     2542 2023-06-12 12:03:02.000000 ExpoSeq-1.1.7/src/ExpoSeq/plots/usq_plot.py
--rw-rw-rw-   0        0        0     3019 2023-06-12 12:03:02.000000 ExpoSeq-1.1.7/src/ExpoSeq/reset.py
--rw-rw-rw-   0        0        0      288 2023-06-12 12:03:02.000000 ExpoSeq-1.1.7/src/ExpoSeq/run.py
-drwxrwxrwx   0        0        0        0 2023-06-27 08:06:35.311106 ExpoSeq-1.1.7/src/ExpoSeq/settings/
--rw-rw-rw-   0        0        0        0 2023-06-12 12:03:02.000000 ExpoSeq-1.1.7/src/ExpoSeq/settings/__init__.py
--rw-rw-rw-   0        0        0     2086 2023-06-12 12:03:02.000000 ExpoSeq-1.1.7/src/ExpoSeq/settings/blosum_62.txt
--rw-rw-rw-   0        0        0     1883 2023-06-12 12:03:02.000000 ExpoSeq-1.1.7/src/ExpoSeq/settings/change_save_settings.py
--rw-rw-rw-   0        0        0       94 2023-06-12 12:10:03.000000 ExpoSeq-1.1.7/src/ExpoSeq/settings/colorbar.txt
--rw-rw-rw-   0        0        0       86 2023-06-12 12:10:03.000000 ExpoSeq-1.1.7/src/ExpoSeq/settings/font_settings.txt
--rw-rw-rw-   0        0        0       57 2023-06-12 12:10:03.000000 ExpoSeq-1.1.7/src/ExpoSeq/settings/global_vars.txt
--rw-rw-rw-   0        0        0      179 2023-06-12 12:10:03.000000 ExpoSeq-1.1.7/src/ExpoSeq/settings/legend_settings.txt
--rw-rw-rw-   0        0        0     8133 2023-06-12 12:03:02.000000 ExpoSeq-1.1.7/src/ExpoSeq/settings/plot_styler.py
--rw-rw-rw-   0        0        0       42 2023-06-12 12:10:03.000000 ExpoSeq-1.1.7/src/ExpoSeq/settings/save_settings.txt
-drwxrwxrwx   0        0        0        0 2023-06-27 08:06:35.311106 ExpoSeq-1.1.7/src/ExpoSeq/test_data/
--rw-rw-rw-   0        0        0        0 2023-06-12 12:03:02.000000 ExpoSeq-1.1.7/src/ExpoSeq/test_data/__init__.py
--rw-rw-rw-   0        0        0    20748 2023-06-12 12:03:02.000000 ExpoSeq-1.1.7/src/ExpoSeq/test_data/all_alignment_reports.pickle
-drwxrwxrwx   0        0        0        0 2023-06-27 08:06:35.342356 ExpoSeq-1.1.7/src/ExpoSeq/test_data/test_files/
--rw-rw-rw-   0        0        0     3578 2023-06-12 12:03:02.000000 ExpoSeq-1.1.7/src/ExpoSeq/test_data/test_files/Chris_main_df.csv
--rw-rw-rw-   0        0        0        0 2023-06-12 12:03:02.000000 ExpoSeq-1.1.7/src/ExpoSeq/test_data/test_files/__init__.py
--rw-rw-rw-   0        0        0    11375 2023-06-16 09:43:27.000000 ExpoSeq-1.1.7/src/ExpoSeq/test_data/test_files/binding_data.csv
--rw-rw-rw-   0        0        0      566 2023-06-16 09:43:29.000000 ExpoSeq-1.1.7/src/ExpoSeq/test_data/test_files/experiment_names.pickle
--rw-rw-rw-   0        0        0 17354490 2023-06-16 09:43:29.000000 ExpoSeq-1.1.7/src/ExpoSeq/test_data/test_files/sequencing_report.csv
--rw-rw-rw-   0        0        0    87391 2023-06-12 12:03:02.000000 ExpoSeq-1.1.7/src/ExpoSeq/test_data/test_files/test1.fastq
--rw-rw-rw-   0        0        0   210829 2023-06-12 12:03:02.000000 ExpoSeq-1.1.7/src/ExpoSeq/test_data/test_files/test2.fastq
--rw-rw-rw-   0        0        0    94420 2023-06-12 12:03:02.000000 ExpoSeq-1.1.7/src/ExpoSeq/test_data/test_files/test3.fastq
--rw-rw-rw-   0        0        0     2632 2023-06-12 12:05:40.000000 ExpoSeq-1.1.7/src/ExpoSeq/test_uploader.py
-drwxrwxrwx   0        0        0        0 2023-06-27 08:06:35.389823 ExpoSeq-1.1.7/src/ExpoSeq/tidy_data/
--rw-rw-rw-   0        0        0        0 2023-06-12 12:03:02.000000 ExpoSeq-1.1.7/src/ExpoSeq/tidy_data/__init__.py
--rw-rw-rw-   0        0        0     2176 2023-06-12 12:03:02.000000 ExpoSeq-1.1.7/src/ExpoSeq/tidy_data/aminoacid_distribution.py
--rw-rw-rw-   0        0        0     2228 2023-06-12 12:03:02.000000 ExpoSeq-1.1.7/src/ExpoSeq/tidy_data/barplot.py
--rw-rw-rw-   0        0        0     1152 2023-06-12 12:03:02.000000 ExpoSeq-1.1.7/src/ExpoSeq/tidy_data/clustering.py
-drwxrwxrwx   0        0        0        0 2023-06-27 08:06:35.421205 ExpoSeq-1.1.7/src/ExpoSeq/tidy_data/heatmaps/
--rw-rw-rw-   0        0        0        0 2023-06-12 12:03:02.000000 ExpoSeq-1.1.7/src/ExpoSeq/tidy_data/heatmaps/__init__.py
--rw-rw-rw-   0        0        0     1509 2023-06-12 12:03:02.000000 ExpoSeq-1.1.7/src/ExpoSeq/tidy_data/heatmaps/bool_sequences_matrix.py
--rw-rw-rw-   0        0        0     1818 2023-06-12 12:03:02.000000 ExpoSeq-1.1.7/src/ExpoSeq/tidy_data/heatmaps/tidy_heatmap_share.py
--rw-rw-rw-   0        0        0     1673 2023-06-12 12:03:02.000000 ExpoSeq-1.1.7/src/ExpoSeq/tidy_data/heatmaps/tidy_jaccard.py
--rw-rw-rw-   0        0        0     5139 2023-06-12 12:03:02.000000 ExpoSeq-1.1.7/src/ExpoSeq/tidy_data/heatmaps/tidy_morosita_horn.py
--rw-rw-rw-   0        0        0     1597 2023-06-12 12:03:02.000000 ExpoSeq-1.1.7/src/ExpoSeq/tidy_data/heatmaps/tidy_sorensen.py
--rw-rw-rw-   0        0        0      678 2023-06-12 12:03:02.000000 ExpoSeq-1.1.7/src/ExpoSeq/tidy_data/interpret_data.py
--rw-rw-rw-   0        0        0     3907 2023-06-12 12:03:02.000000 ExpoSeq-1.1.7/src/ExpoSeq/tidy_data/read_extract_data.py
--rw-rw-rw-   0        0        0      440 2023-06-12 12:03:02.000000 ExpoSeq-1.1.7/src/ExpoSeq/tidy_data/tidy_USQ_plot_.py
--rw-rw-rw-   0        0        0     1217 2023-06-12 12:03:02.000000 ExpoSeq-1.1.7/src/ExpoSeq/tidy_data/tidy_alignment_reports.py
--rw-rw-rw-   0        0        0     1461 2023-06-12 12:03:02.000000 ExpoSeq-1.1.7/src/ExpoSeq/tidy_data/tidy_cluster_embedding.py
--rw-rw-rw-   0        0        0      391 2023-06-12 12:03:02.000000 ExpoSeq-1.1.7/src/ExpoSeq/tidy_data/tidy_library.py
--rw-rw-rw-   0        0        0     1992 2023-06-12 12:03:02.000000 ExpoSeq-1.1.7/src/ExpoSeq/tidy_data/tidy_rel_sequence_abun.py
--rw-rw-rw-   0        0        0     1599 2023-06-12 12:03:02.000000 ExpoSeq-1.1.7/src/ExpoSeq/tidy_data/tidy_seqlogoPlot.py
--rw-rw-rw-   0        0        0     1299 2023-06-12 12:03:02.000000 ExpoSeq-1.1.7/src/ExpoSeq/tidy_data/tidy_stacked_aa_distr.py
-drwxrwxrwx   0        0        0        0 2023-06-27 08:06:35.183124 ExpoSeq-1.1.7/src/ExpoSeq.egg-info/
--rw-rw-rw-   0        0        0     4091 2023-06-27 08:06:35.000000 ExpoSeq-1.1.7/src/ExpoSeq.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2971 2023-06-27 08:06:35.000000 ExpoSeq-1.1.7/src/ExpoSeq.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-27 08:06:35.000000 ExpoSeq-1.1.7/src/ExpoSeq.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      188 2023-06-27 08:06:35.000000 ExpoSeq-1.1.7/src/ExpoSeq.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-27 08:06:35.000000 ExpoSeq-1.1.7/src/ExpoSeq.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-02 11:46:32.467532 ExpoSeq-1.1.9/
+-rw-rw-rw-   0        0        0    11558 2023-06-30 13:21:19.000000 ExpoSeq-1.1.9/LICENSE
+-rw-rw-rw-   0        0        0       59 2023-05-30 20:50:39.000000 ExpoSeq-1.1.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     4106 2023-07-02 11:46:32.467532 ExpoSeq-1.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     3725 2023-05-30 20:50:39.000000 ExpoSeq-1.1.9/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-02 11:46:32.467532 ExpoSeq-1.1.9/setup.cfg
+-rw-rw-rw-   0        0        0     1335 2023-07-02 11:45:04.000000 ExpoSeq-1.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-02 11:46:30.006376 ExpoSeq-1.1.9/src/
+drwxrwxrwx   0        0        0        0 2023-07-02 11:46:30.203584 ExpoSeq-1.1.9/src/ExpoSeq/
+-rw-rw-rw-   0        0        0        0 2023-06-12 12:03:02.000000 ExpoSeq-1.1.9/src/ExpoSeq/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-02 11:46:30.754801 ExpoSeq-1.1.9/src/ExpoSeq/augment_data/
+-rw-rw-rw-   0        0        0        0 2023-06-12 12:03:02.000000 ExpoSeq-1.1.9/src/ExpoSeq/augment_data/__init__.py
+-rw-rw-rw-   0        0        0     1007 2023-06-12 12:03:02.000000 ExpoSeq-1.1.9/src/ExpoSeq/augment_data/binding_data.py
+-rw-rw-rw-   0        0        0      858 2023-06-12 12:03:02.000000 ExpoSeq-1.1.9/src/ExpoSeq/augment_data/check_reports.py
+-rw-rw-rw-   0        0        0      913 2023-06-12 12:03:02.000000 ExpoSeq-1.1.9/src/ExpoSeq/augment_data/load_data.py
+-rw-rw-rw-   0        0        0     4616 2023-06-12 12:03:02.000000 ExpoSeq-1.1.9/src/ExpoSeq/augment_data/loop_collect_reports.py
+-rw-rw-rw-   0        0        0     7915 2023-06-12 12:03:02.000000 ExpoSeq-1.1.9/src/ExpoSeq/augment_data/mixcr_cl.py
+-rw-rw-rw-   0        0        0    10619 2023-06-29 12:41:04.000000 ExpoSeq-1.1.9/src/ExpoSeq/augment_data/mixcr_nils.py
+-rw-rw-rw-   0        0        0     6814 2023-07-02 11:44:34.000000 ExpoSeq-1.1.9/src/ExpoSeq/augment_data/randomizer.py
+-rw-rw-rw-   0        0        0      580 2023-06-12 12:03:02.000000 ExpoSeq-1.1.9/src/ExpoSeq/augment_data/read_raw_data.py
+-rw-rw-rw-   0        0        0     3646 2023-06-12 12:03:02.000000 ExpoSeq-1.1.9/src/ExpoSeq/augment_data/structure_files.py
+-rw-rw-rw-   0        0        0      519 2023-06-12 12:03:02.000000 ExpoSeq-1.1.9/src/ExpoSeq/augment_data/trimming.py
+-rw-rw-rw-   0        0        0    17434 2023-06-29 12:43:18.000000 ExpoSeq-1.1.9/src/ExpoSeq/augment_data/uploader.py
+-rw-rw-rw-   0        0        0    10290 2023-06-12 12:16:56.000000 ExpoSeq-1.1.9/src/ExpoSeq/full_pipe.py
+-rw-rw-rw-   0        0        0    39362 2023-07-02 09:18:41.000000 ExpoSeq-1.1.9/src/ExpoSeq/pipeline.py
+drwxrwxrwx   0        0        0        0 2023-07-02 11:46:31.245005 ExpoSeq-1.1.9/src/ExpoSeq/plots/
+-rw-rw-rw-   0        0        0        0 2023-06-12 12:03:02.000000 ExpoSeq-1.1.9/src/ExpoSeq/plots/__init__.py
+-rw-rw-rw-   0        0        0     2061 2023-06-12 12:03:02.000000 ExpoSeq-1.1.9/src/ExpoSeq/plots/barplot.py
+-rw-rw-rw-   0        0        0     1666 2023-06-12 12:03:02.000000 ExpoSeq-1.1.9/src/ExpoSeq/plots/cluster_embedding.py
+-rw-rw-rw-   0        0        0     4363 2023-07-02 09:18:51.000000 ExpoSeq-1.1.9/src/ExpoSeq/plots/embedding_with_binding.py
+-rw-rw-rw-   0        0        0     3444 2023-06-12 12:03:02.000000 ExpoSeq-1.1.9/src/ExpoSeq/plots/length_distribution.py
+-rw-rw-rw-   0        0        0     7669 2023-06-12 12:03:02.000000 ExpoSeq-1.1.9/src/ExpoSeq/plots/levenshtein_clustering.py
+-rw-rw-rw-   0        0        0     4379 2023-06-12 12:03:02.000000 ExpoSeq-1.1.9/src/ExpoSeq/plots/logo_plot.py
+-rw-rw-rw-   0        0        0     3383 2023-06-16 09:49:51.000000 ExpoSeq-1.1.9/src/ExpoSeq/plots/plt_heatmap.py
+-rw-rw-rw-   0        0        0     2524 2023-06-12 12:03:02.000000 ExpoSeq-1.1.9/src/ExpoSeq/plots/protvec.py
+-rw-rw-rw-   0        0        0     1470 2023-06-12 12:03:02.000000 ExpoSeq-1.1.9/src/ExpoSeq/plots/relative_sequence_abundance.py
+-rw-rw-rw-   0        0        0     1634 2023-06-12 12:03:02.000000 ExpoSeq-1.1.9/src/ExpoSeq/plots/saveFig.py
+-rw-rw-rw-   0        0        0     1064 2023-06-12 12:03:02.000000 ExpoSeq-1.1.9/src/ExpoSeq/plots/stacked_aa_distribution.py
+-rw-rw-rw-   0        0        0     2542 2023-06-12 12:03:02.000000 ExpoSeq-1.1.9/src/ExpoSeq/plots/usq_plot.py
+-rw-rw-rw-   0        0        0     3019 2023-06-12 12:03:02.000000 ExpoSeq-1.1.9/src/ExpoSeq/reset.py
+-rw-rw-rw-   0        0        0      288 2023-06-12 12:03:02.000000 ExpoSeq-1.1.9/src/ExpoSeq/run.py
+drwxrwxrwx   0        0        0        0 2023-07-02 11:46:31.411195 ExpoSeq-1.1.9/src/ExpoSeq/settings/
+-rw-rw-rw-   0        0        0        0 2023-06-12 12:03:02.000000 ExpoSeq-1.1.9/src/ExpoSeq/settings/__init__.py
+-rw-rw-rw-   0        0        0     2086 2023-06-12 12:03:02.000000 ExpoSeq-1.1.9/src/ExpoSeq/settings/blosum_62.txt
+-rw-rw-rw-   0        0        0     1883 2023-06-12 12:03:02.000000 ExpoSeq-1.1.9/src/ExpoSeq/settings/change_save_settings.py
+-rw-rw-rw-   0        0        0       94 2023-06-12 12:10:03.000000 ExpoSeq-1.1.9/src/ExpoSeq/settings/colorbar.txt
+-rw-rw-rw-   0        0        0       86 2023-06-12 12:10:03.000000 ExpoSeq-1.1.9/src/ExpoSeq/settings/font_settings.txt
+-rw-rw-rw-   0        0        0       57 2023-06-12 12:10:03.000000 ExpoSeq-1.1.9/src/ExpoSeq/settings/global_vars.txt
+-rw-rw-rw-   0        0        0      179 2023-06-12 12:10:03.000000 ExpoSeq-1.1.9/src/ExpoSeq/settings/legend_settings.txt
+-rw-rw-rw-   0        0        0     8133 2023-06-12 12:03:02.000000 ExpoSeq-1.1.9/src/ExpoSeq/settings/plot_styler.py
+-rw-rw-rw-   0        0        0       42 2023-06-12 12:10:03.000000 ExpoSeq-1.1.9/src/ExpoSeq/settings/save_settings.txt
+drwxrwxrwx   0        0        0        0 2023-07-02 11:46:31.451101 ExpoSeq-1.1.9/src/ExpoSeq/test_data/
+-rw-rw-rw-   0        0        0        0 2023-06-12 12:03:02.000000 ExpoSeq-1.1.9/src/ExpoSeq/test_data/__init__.py
+-rw-rw-rw-   0        0        0    20748 2023-06-12 12:03:02.000000 ExpoSeq-1.1.9/src/ExpoSeq/test_data/all_alignment_reports.pickle
+drwxrwxrwx   0        0        0        0 2023-07-02 11:46:31.547379 ExpoSeq-1.1.9/src/ExpoSeq/test_data/test_files/
+-rw-rw-rw-   0        0        0     3578 2023-06-12 12:03:02.000000 ExpoSeq-1.1.9/src/ExpoSeq/test_data/test_files/Chris_main_df.csv
+-rw-rw-rw-   0        0        0        0 2023-06-12 12:03:02.000000 ExpoSeq-1.1.9/src/ExpoSeq/test_data/test_files/__init__.py
+-rw-rw-rw-   0        0        0    11375 2023-06-16 09:43:27.000000 ExpoSeq-1.1.9/src/ExpoSeq/test_data/test_files/binding_data.csv
+-rw-rw-rw-   0        0        0      566 2023-06-16 09:43:29.000000 ExpoSeq-1.1.9/src/ExpoSeq/test_data/test_files/experiment_names.pickle
+-rw-rw-rw-   0        0        0 17354490 2023-06-16 09:43:29.000000 ExpoSeq-1.1.9/src/ExpoSeq/test_data/test_files/sequencing_report.csv
+-rw-rw-rw-   0        0        0    87391 2023-06-12 12:03:02.000000 ExpoSeq-1.1.9/src/ExpoSeq/test_data/test_files/test1.fastq
+-rw-rw-rw-   0        0        0   210829 2023-06-12 12:03:02.000000 ExpoSeq-1.1.9/src/ExpoSeq/test_data/test_files/test2.fastq
+-rw-rw-rw-   0        0        0    94420 2023-06-12 12:03:02.000000 ExpoSeq-1.1.9/src/ExpoSeq/test_data/test_files/test3.fastq
+-rw-rw-rw-   0        0        0     2632 2023-06-12 12:05:40.000000 ExpoSeq-1.1.9/src/ExpoSeq/test_uploader.py
+drwxrwxrwx   0        0        0        0 2023-07-02 11:46:32.145820 ExpoSeq-1.1.9/src/ExpoSeq/tidy_data/
+-rw-rw-rw-   0        0        0        0 2023-06-12 12:03:02.000000 ExpoSeq-1.1.9/src/ExpoSeq/tidy_data/__init__.py
+-rw-rw-rw-   0        0        0     2176 2023-06-12 12:03:02.000000 ExpoSeq-1.1.9/src/ExpoSeq/tidy_data/aminoacid_distribution.py
+-rw-rw-rw-   0        0        0     2228 2023-06-12 12:03:02.000000 ExpoSeq-1.1.9/src/ExpoSeq/tidy_data/barplot.py
+-rw-rw-rw-   0        0        0     1152 2023-06-12 12:03:02.000000 ExpoSeq-1.1.9/src/ExpoSeq/tidy_data/clustering.py
+drwxrwxrwx   0        0        0        0 2023-07-02 11:46:32.427345 ExpoSeq-1.1.9/src/ExpoSeq/tidy_data/heatmaps/
+-rw-rw-rw-   0        0        0        0 2023-06-12 12:03:02.000000 ExpoSeq-1.1.9/src/ExpoSeq/tidy_data/heatmaps/__init__.py
+-rw-rw-rw-   0        0        0     1509 2023-06-12 12:03:02.000000 ExpoSeq-1.1.9/src/ExpoSeq/tidy_data/heatmaps/bool_sequences_matrix.py
+-rw-rw-rw-   0        0        0     1818 2023-06-12 12:03:02.000000 ExpoSeq-1.1.9/src/ExpoSeq/tidy_data/heatmaps/tidy_heatmap_share.py
+-rw-rw-rw-   0        0        0     1673 2023-06-12 12:03:02.000000 ExpoSeq-1.1.9/src/ExpoSeq/tidy_data/heatmaps/tidy_jaccard.py
+-rw-rw-rw-   0        0        0     5139 2023-06-12 12:03:02.000000 ExpoSeq-1.1.9/src/ExpoSeq/tidy_data/heatmaps/tidy_morosita_horn.py
+-rw-rw-rw-   0        0        0     1597 2023-06-12 12:03:02.000000 ExpoSeq-1.1.9/src/ExpoSeq/tidy_data/heatmaps/tidy_sorensen.py
+-rw-rw-rw-   0        0        0      678 2023-06-12 12:03:02.000000 ExpoSeq-1.1.9/src/ExpoSeq/tidy_data/interpret_data.py
+-rw-rw-rw-   0        0        0     3907 2023-06-12 12:03:02.000000 ExpoSeq-1.1.9/src/ExpoSeq/tidy_data/read_extract_data.py
+-rw-rw-rw-   0        0        0      440 2023-06-12 12:03:02.000000 ExpoSeq-1.1.9/src/ExpoSeq/tidy_data/tidy_USQ_plot_.py
+-rw-rw-rw-   0        0        0     1217 2023-06-12 12:03:02.000000 ExpoSeq-1.1.9/src/ExpoSeq/tidy_data/tidy_alignment_reports.py
+-rw-rw-rw-   0        0        0     1461 2023-06-12 12:03:02.000000 ExpoSeq-1.1.9/src/ExpoSeq/tidy_data/tidy_cluster_embedding.py
+-rw-rw-rw-   0        0        0      391 2023-06-12 12:03:02.000000 ExpoSeq-1.1.9/src/ExpoSeq/tidy_data/tidy_library.py
+-rw-rw-rw-   0        0        0     1992 2023-06-12 12:03:02.000000 ExpoSeq-1.1.9/src/ExpoSeq/tidy_data/tidy_rel_sequence_abun.py
+-rw-rw-rw-   0        0        0     1599 2023-06-12 12:03:02.000000 ExpoSeq-1.1.9/src/ExpoSeq/tidy_data/tidy_seqlogoPlot.py
+-rw-rw-rw-   0        0        0     1299 2023-06-12 12:03:02.000000 ExpoSeq-1.1.9/src/ExpoSeq/tidy_data/tidy_stacked_aa_distr.py
+drwxrwxrwx   0        0        0        0 2023-07-02 11:46:30.271065 ExpoSeq-1.1.9/src/ExpoSeq.egg-info/
+-rw-rw-rw-   0        0        0     4106 2023-07-02 11:46:29.000000 ExpoSeq-1.1.9/src/ExpoSeq.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2971 2023-07-02 11:46:29.000000 ExpoSeq-1.1.9/src/ExpoSeq.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-02 11:46:29.000000 ExpoSeq-1.1.9/src/ExpoSeq.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      188 2023-07-02 11:46:29.000000 ExpoSeq-1.1.9/src/ExpoSeq.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-02 11:46:29.000000 ExpoSeq-1.1.9/src/ExpoSeq.egg-info/top_level.txt
```

### Comparing `ExpoSeq-1.1.7/PKG-INFO` & `ExpoSeq-1.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: ExpoSeq
-Version: 1.1.7
+Version: 1.1.9
 Summary: A pacakge which provides various ways to analyze NGS data from phage display campaigns
 Home-page: https://github.com/nilshof01/ExpoSeq
 Author: Nils Hofmann
 Author-email: n.hofmann.99@web.de
-License: MIT
+License: Apache License 2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Welcome to ExpoSeq
 
 ExpoSeq is a powerful pipeline for processing and analyzing FASTQ files from sequencing phage Display panning samples.It utilizes [MiXCR](https://docs.milaboratories.com/mixcr/getting-started/installation/) to align and assemble the data which you can subsequently analyze in multiple plots. The pipeline focuses on analysing the identity between samples but also applies various clustering techniques to analyse the relation between the sequences. Besides, you can add binding data to relate the clusters to affinity.  ![overview](expoSeq_overview.png)
```

### Comparing `ExpoSeq-1.1.7/README.md` & `ExpoSeq-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.7/setup.py` & `ExpoSeq-1.1.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name = "ExpoSeq",
-    version = "1.1.7",
+    version = "1.1.9",
     description = "A pacakge which provides various ways to analyze NGS data from phage display campaigns",
     long_description=long_description,
     long_description_content_type = "text/markdown",
     url = "https://github.com/nilshof01/ExpoSeq",
     author = "Nils Hofmann",
     author_email = "n.hofmann.99@web.de",
-    license = "MIT",
+    license = "Apache License 2.0",
     package_data={
         "ExpoSeq": ["settings/*.txt", "test_data/test_files/*", "test_data/*"]
     },
     install_requires = [
                         "numpy>=1.23.5",
                         "pandas>=1.5.3",
                         "matplotlib>=3.6.3",
```

### Comparing `ExpoSeq-1.1.7/src/ExpoSeq/augment_data/binding_data.py` & `ExpoSeq-1.1.9/src/ExpoSeq/augment_data/binding_data.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.7/src/ExpoSeq/augment_data/check_reports.py` & `ExpoSeq-1.1.9/src/ExpoSeq/augment_data/check_reports.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.7/src/ExpoSeq/augment_data/load_data.py` & `ExpoSeq-1.1.9/src/ExpoSeq/augment_data/load_data.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.7/src/ExpoSeq/augment_data/loop_collect_reports.py` & `ExpoSeq-1.1.9/src/ExpoSeq/augment_data/loop_collect_reports.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.7/src/ExpoSeq/augment_data/mixcr_cl.py` & `ExpoSeq-1.1.9/src/ExpoSeq/augment_data/mixcr_cl.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.7/src/ExpoSeq/augment_data/mixcr_nils.py` & `ExpoSeq-1.1.9/src/ExpoSeq/augment_data/mixcr_nils.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,22 +56,25 @@
 
     return filenames
 
 
 def process_mixcr(experiment, method, testing, paired_end_sequencing):
     pkg_path = pkg_resources.resource_filename("ExpoSeq", "")
     module_dir = os.path.abspath("")
+    
     if not testing:
         print("Choose the directory where you store your fastq files")
         while True:
             filenames = add_fastq_files()
             if len(filenames) == 0:
                 print("You have not added any fastq files the preprocessing is cancelled now.")
             else:
                 break
+        if not os.path.isdir(os.path.join(module_dir, "my_experiments", experiment, "alignment_reports")):
+            os.mkdir(os.path.join(module_dir, "my_experiments", experiment, "alignment_reports"))
 
     else:
 
         filenames = glob(os.path.join(pkg_path,"test_data","test_files", "*.fastq"))
         print(filenames)
         experiment = "test_directory"
     settings_dir = os.path.join(pkg_path,
```

### Comparing `ExpoSeq-1.1.7/src/ExpoSeq/augment_data/randomizer.py` & `ExpoSeq-1.1.9/src/ExpoSeq/augment_data/randomizer.py`

 * *Files 0% similar despite different names*

```diff
@@ -88,15 +88,14 @@
 
 
 
 def create_binding_report(sequencing_report, num_antigen):
     threshold_aa_seq = 5
     sampled_df = sequencing_report[~sequencing_report.duplicated(subset='aaSeqCDR3', keep=False)]
     sampled_df = sampled_df.groupby("Experiment").sample(frac = 0.01)
-    sampled_df
     sampled_df = sampled_df[sampled_df['aaSeqCDR3'].apply(len) >= threshold_aa_seq]
     aaSeq = sampled_df["aaSeqCDR3"].to_list()
     fractions = sampled_df.clonesFraction
     binding_values = []
     for i in fractions:
         random_binding = random.randint(1000000, 10000000000)
         binding_value = i * random_binding
```

### Comparing `ExpoSeq-1.1.7/src/ExpoSeq/augment_data/read_raw_data.py` & `ExpoSeq-1.1.9/src/ExpoSeq/augment_data/read_raw_data.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.7/src/ExpoSeq/augment_data/structure_files.py` & `ExpoSeq-1.1.9/src/ExpoSeq/augment_data/structure_files.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.7/src/ExpoSeq/augment_data/trimming.py` & `ExpoSeq-1.1.9/src/ExpoSeq/augment_data/trimming.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.7/src/ExpoSeq/augment_data/uploader.py` & `ExpoSeq-1.1.9/src/ExpoSeq/augment_data/uploader.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
-
-from .mixcr_nils import process_mixcr
+from ExpoSeq.augment_data.mixcr_nils import process_mixcr
 from ast import literal_eval
 import os
-from .loop_collect_reports import load_mixed_files, load_alignment_reports
+from ExpoSeq.augment_data.loop_collect_reports import load_mixed_files, load_alignment_reports
 import pandas as pd
 from glob import glob
 from ExpoSeq.augment_data.check_reports import check_completeness
 import sys
 import pickle
 import pkg_resources
 from ExpoSeq.augment_data.trimming import trimming
@@ -27,15 +26,15 @@
 def pull_seq_align_repo(testing, testing_value):
     if not testing:
         try:
             print("choose the directory where you store your alignment reports and your sequencing report")
             filenames_dir = filedialog.askdirectory()
             assert os.path.isdir(filenames_dir), "Please enter a valid directory."
             filenames = glob(filenames_dir + "//*")
-            
+           
         except:
             filenames_dir = input(
                 "Enter the directory where you store the alignment reports and your sequencing report manually. You should have one file for the sequencing report and multiple files for the alignment reports.")
             while True:
                 if os.path.isdir(filenames_dir):
                     break
                 else:
@@ -64,41 +63,45 @@
             experiment = input("How do you want to call your new experiment?")
             if os.path.isdir(os.path.join(module_dir, "my_experiments", experiment)) == True:
                 replace = input("The given directory already exists. Do you want to replace it? (Y/n)")
                 if replace in ["Y", "y", "n", "N"]:
                     break
                 else:
                     print("Please enter another name.")
+                if replace in ["Y", "y"]:
+                    shutil.rmtree(os.path.join(module_dir, "my_experiments", experiment))
+                    os.mkdir(os.path.join(module_dir, "my_experiments", experiment))
             else:
                 break
-        if replace in ["Y", "y"]:
-            shutil.rmtree(os.path.join(module_dir, "my_experiments", experiment))
-            os.mkdir(os.path.join(module_dir, "my_experiments", experiment))
-    else: 
+
+
+    else:
         experiment = get_random_string(10)
-    
+   
     os.mkdir(os.path.join(module_dir,
                     "my_experiments",
                     experiment))
     return experiment
 
 def method_one(experiment, repo_path, module_dir, testing, paired_end_test = "n"):
+    if repo_path == "":
+        repo_path = os.path.join(module_dir, "my_experiments", experiment, "sequencing_report.csv")
     if not testing:
         use_method = input(
             "Per default you will align your data with the following method: milab-human-tcr-dna-multiplex-cdr3 . Press enter if you want to continue. Otherwise type in the method of your choice which. It has to be the exact same string which is given on the Mixcr documentation.")
     else:
         use_method = ""
     if use_method == "":
         method = "milab-human-tcr-dna-multiplex-cdr3"
     else:
         method = use_method
     if not testing:
         paired_end = input("Do you want to analyze paired_end_sequencing data? (Y/n)")
-        
-    else: 
+       
+    else:
         paired_end = 'n'
     while True:
         if paired_end in ["Y", "y", "n", "N"]:
             break
         else:
             print("Please enter a correct value.")
             paired_end = input("Do you want to analyze paired_end_sequencing data? (Y/n)")
@@ -249,15 +252,15 @@
 
         last_experiment = data["last_experiment"]
         if last_experiment == "":
             print("You have no experiments in your folder.")
             repo_path = ""
         else:
             repo_path = os.path.join(module_dir,
-                                    "my_experiments",
+                                   "my_experiments",
                                     last_experiment,
                                     "sequencing_report.csv")
     else:
         repo_path = os.path.join(module_dir,
                                 "my_experiments",
                                 "test_directory",
                                 "sequencing_report.csv")
@@ -285,22 +288,22 @@
     return processing
 
 def get_experiment_name_input(testing = False):
     if not testing:
         experiment_name = input("Enter the name of the experiment you want to analyze")
     else:
         experiment_name = get_random_string(10)
-    return experiment_name  
+    return experiment_name 
 
 def upload_new_experiment(module_dir, repo_path, testing, testing_value, paired_end_test, experiment_column):
     experiment = check_experiment(module_dir, testing)
     choose_method = get_choose_method_input(testing, testing_value)
-    
+   
     if choose_method == "1":
-        
+       
         sequencing_report, all_alignment_reports = method_one(experiment, repo_path,module_dir,testing, paired_end_test )
     elif choose_method == "2":
         sequencing_report, all_alignment_reports = method_two(module_dir, experiment,testing, experiment_column)
     elif choose_method == "3":
         sequencing_report, all_alignment_reports, experiment = method_three(module_dir, experiment, testing)
     else:
         raise ValueError("Invalid option")
@@ -308,15 +311,15 @@
     return sequencing_report, all_alignment_reports, experiment
 
 def choose_existing_experiment(module_dir, testing):
     if not testing:
         while True:
             user_input = get_experiment_name_input()
             spec_exp_name_path = os.path.join(module_dir, "my_experiments", user_input)
-            if os.path.isdir(spec_exp_name_path): 
+            if os.path.isdir(spec_exp_name_path):
                 break
             else:
                 print("The experiment name does not exist in my_experiments. Please enter the correct name")
     else:
         user_input = "test_directory"
     return user_input  # experiment
 
@@ -371,8 +374,8 @@
                 raise ValueError("Invalid option")
         else:
             sequencing_report, all_alignment_reports, experiment = process_data_with_last_experiment(module_dir, last_experiment, testing)
     else:
         sequencing_report, all_alignment_reports, experiment = upload_new_experiment(module_dir, repo_path, testing, upload_type, paired_end_test, experiment_column)
     if testing and experiment != "test_directory":
         shutil.rmtree(os.path.join(module_dir, "my_experiments", experiment))
-    return sequencing_report, all_alignment_reports, experiment
+    return sequencing_report, all_alignment_reports, experiment
```

### Comparing `ExpoSeq-1.1.7/src/ExpoSeq/full_pipe.py` & `ExpoSeq-1.1.9/src/ExpoSeq/full_pipe.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.7/src/ExpoSeq/pipeline.py` & `ExpoSeq-1.1.9/src/ExpoSeq/pipeline.py`

 * *Files 11% similar despite different names*

```diff
@@ -144,14 +144,15 @@
 
     def change_experiment_names(self, specific = None, change_whole_dic = False):
         """
         :param specific: optional parameter. You can use this function to change the names of a specific sample.
         :param change_whole_dic: optional Parameter. In general the renaming is done be using a dictionary and map it to the labels. You can change the whole dictionary for ExpoSeq your original labels by adding the new dictionary for this parameter.
         :return:You can use this function to change the name of your samples. Thus, you can change the labels of your plots.
         """
+
         if specific != None:
             assert type(specific) == str, "You have to give a string (inside: "") as input for the specific sample you want to change"
         if change_whole_dic != False:
             assert type(change_whole_dic) == dict, "You have to give a dictionary as input for the specific sample you want to change"
         if change_whole_dic == False:
             if specific == None:
                 for key in self.unique_experiments:
@@ -171,14 +172,17 @@
 
     def alignment_quality(self, log_transformation = False):
         """
 
         :param log_transformation: optional parameter. You can set it to True if you want to log transform your data
         :return: Creates a figure where you can see the Overall Reads per sample and the number of reads which could be aligned.
         """
+        if not plt.fignum_exists(1):
+            self.fig = plt.figure(1)
+            print("Please do not close the window for the figure while the plot is loading")
         assert log_transformation in [True, False], "You have to give True or False as input for the log transformation"
         self.fig.clear()
         self.ax = self.fig.gca()
         try:
             barplot(self.ax,
                     self.alignment_report,
                     self.sequencing_report,
@@ -196,14 +200,17 @@
     def aa_distribution(self, sample, region, protein = True):
         """
         :param sample: The sample you would like to analyze
         :param region: the region you would like to analyze
         :param protein: Default True. If you would like to analyze nucleotide sequences, set it to False
         :return: Returns a plot which shows the amino acid distribution in the given sequence range.
         """
+        if not plt.fignum_exists(1):
+            self.fig = plt.figure(1)
+            print("Please do not close the window for the figure while the plot is loading")
         assert sample in self.experiments_list, "The provided sample name is not in your sequencing report. Please check the spelling or use the print_samples function to see the names of your samples"
         assert type(sample), "You have to give a string as input for the sample"
         assert type(region), "You have to give a list with the start and end position of the region you want to analyze. For instance: [3,7]"
         assert protein in [True, False], "You have to give True or False as input for the protein parameter"
         self.fig.clear()
         self.ax = self.fig.gca()
         stacked_aa_distr(self.ax,
@@ -219,14 +226,17 @@
         figManager = plt.get_current_fig_manager()
         figManager.window.showMaximized()
     def usqPlot(self, samples):
         """
         :param samples: you insert a list which contains the sample names
         :return: USQ stands for unique sequences quality and the plot shows you the depth of unique sequences which can be used for evaluating your sequencing quality.
         """
+        if not plt.fignum_exists(1):
+            self.fig = plt.figure(1)
+            print("Please do not close the window for the figure while the plot is loading")
         incorrect_samples = [x for x in samples if x not in self.experiments_list]
         assert not incorrect_samples, f"The following sample(s) are not in your sequencing report: {', '.join(incorrect_samples)}. Please check the spelling or use the print_samples function to see the names of your samples"
 
         if type(samples) != list:
             print("You have to give the sample names in the list, also if it is only one! A list is a container which is marked through:[] . Please try again.")
         else:
             self.fig.clear()
@@ -251,14 +261,17 @@
         """
         :param sample: insert the sample name
         :param highlight_specific_pos: optional. you can highlight a specific position
         :param highlight_pos_range: optional. you can highlight a position range
         :param chosen_seq_length: 16 per default. You always analyze online one sequence length! You can change it if you would like to.
         :return: A logo Plot which shows you the composition of aminoacids per position
         """
+        if not plt.fignum_exists(1):
+            self.fig = plt.figure(1)
+            print("Please do not close the window for the figure while the plot is loading")
         assert sample in self.experiments_list, "The provided sample name is not in your sequencing report. Please check the spelling or use the print_samples function to see the names of your samples"
         assert type(sample) == str, "You have to give a string as input for the sample"
         if highlight_specific_pos != False:
             assert type(highlight_specific_pos) == int, "You have to give an integer as input for the specific position you want to highlight"
         if highlight_pos_range != False:
             assert type(highlight_pos_range) == list, "You have to give a list with the start and end position of the region you want to highlight. For instance: [3,7]"
         assert type(chosen_seq_length) == int, "You have to give an integer as input for the sequence length you want to analyze"
@@ -283,14 +296,17 @@
                  chosen_seq_length = 16,
                     ):
         """
         :param samples: You analyze all samples per default. If you want to analyze specific samples it has to be a list with the corresponding sample names
         :param chosen_seq_length: 16 per default. You always analyze online one sequence length! You can change it if you would like
         :return: Gives you in one figure one logoPlot per sample.
         """
+        if not plt.fignum_exists(1):
+            self.fig = plt.figure(1)
+            print("Please do not close the window for the figure while the plot is loading")
         if samples != "all":
             assert type(samples) == list, "You have to give a list with the samples you want to analyze"
             incorrect_samples = [x for x in samples if x not in self.experiments_list]
             assert not incorrect_samples, f"The following sample(s) are not in your sequencing report: {', '.join(incorrect_samples)}. Please check the spelling or use the print_samples function to see the names of your samples"
         assert type(chosen_seq_length) == int, "You have to give an integer as input for the sequence length you want to analyze"
         self.fig.clear()
         plot_logo_multi(self.fig,
@@ -310,14 +326,17 @@
 
     def lengthDistribution_single(self, sample):
         """
 
         :param sample: name of the sample from which you would like to see the length distribution
         :return: Shows you the length Distribution of your sequences of the given sample
         """
+        if not plt.fignum_exists(1):
+            self.fig = plt.figure(1)
+            print("Please do not close the window for the figure while the plot is loading")
         assert type(sample) == str, "You have to give a string as input for the sample"
         assert sample in self.experiments_list, "The provided sample name is not in your sequencing report. Please check the spelling or use the print_samples function to see the names of your samples"
         self.fig.clear()
         self.ax = self.fig.gca()
         length_distribution_single(self.fig,
                                    self.ax,
                                    self.sequencing_report,
@@ -330,14 +349,17 @@
         figManager.window.showMaximized()
 
     def lengthDistribution_multi(self, samples = "all"):
         """
         :param samples: You analyze ExpoSeq samples per default. If you want to analyze specific samples it has to be a list with the corresponding sample names
         :return: Outputs one figurewith one subplot per sample which shows you the distribution of sequence length
         """
+        if not plt.fignum_exists(1):
+            self.fig = plt.figure(1)
+            print("Please do not close the window for the figure while the plot is loading")
         if samples != "all":
             assert type(samples) == list, "You have to give a list with the samples you want to analyze"
             incorrect_samples = [x for x in samples if x not in self.experiments_list]
             assert not incorrect_samples, f"The following sample(s) are not in your sequencing report: {', '.join(incorrect_samples)}. Please check the spelling or use the print_samples function to see the names of your samples"
         self.fig.clear()
         length_distribution_multi(self.fig,
                             self.sequencing_report,
@@ -357,14 +379,17 @@
 
         :param samples: For a qualitative analysis choose samples from the same panning experiment. Input is a list
         :param max_levenshtein_distance: Default is 0. You can change it to see increased fraction with increased variability of certain sequences
         :param length_filter: Default is 0. You should change it if you change the levenshtein distance. Otherwise your results will be biased.
         :param batch: Default is 3000. The size of the sample which is chosen. The higher it is, the more computational intense.
         :return: Shows you a Bar Plot of the frequences of the most abundant sequences. You can introduce the levenshtein distance to see how the frequency changes with higher variability of the sequences.
         """
+        if not plt.fignum_exists(1):
+            self.fig = plt.figure(1)
+            print("Please do not close the window for the figure while the plot is loading")
         incorrect_samples = [x for x in samples if x not in self.experiments_list]
         assert not incorrect_samples, f"The following sample(s) are not in your sequencing report: {', '.join(incorrect_samples)}. Please check the spelling or use the print_samples function to see the names of your samples"
         assert type(samples) == list, "You have to give a list with the samples you want to analyze"
         assert type(max_levenshtein_distance), "You have to give an integer as input for the maximum levenshtein distance"
         assert type(length_filter), "You have to give an integer as input for the length filter"
         assert type(batch) == int, "You have to give an integer as input for the batch size"
         self.fig.clear()
@@ -385,14 +410,17 @@
 
 
     def basic_cluster(self, sample,max_ld = 1, min_ld = 0, second_figure = False):
         """
         :param sample: type in a sample name you want to analyze
         :return:
         """
+        if not plt.fignum_exists(1):
+            self.fig = plt.figure(1)
+            print("Please do not close the window for the figure while the plot is loading")
         assert sample in self.experiments_list, "The provided sample name is not in your sequencing report. Please check the spelling or use the print_samples function to see the names of your samples"
         assert type(sample) == str, "You have to give a string as input for the sample"
         assert type(max_ld) == int, "You have to give an integer as input for the maximum levenshtein distance"
         assert type(min_ld) == int, "You have to give an integer as input for the minimum levenshtein distance"
         assert type(second_figure) == bool, "You have to give True or False as input for the second figure"
         self.fig.clear()
         self.ax = self.fig.gca()
@@ -422,14 +450,17 @@
 
         :param antigen: is the name of the antigen you would like to analyze
         :param max_ld: optional Parameter where its default is 1. Is the maximum Levenshtein distance you allow per cluster
         :param min_ld: optional Parameter where its default is 0. Is the minimum Levenshtein distance between sequences you allow
         :param specific_experiments: optional Parameter. You can give the names of specific samples in a list if you want
         :return: Creates a figure where sequences are clustered based on Levenshtein distance. Additionally the binding data of the sequences against a specific antigen is given.
         """
+        if not plt.fignum_exists(1):
+            self.fig = plt.figure(1)
+            print("Please do not close the window for the figure while the plot is loading")
         assert self.binding_data is not None, "You have not given binding data. You can add it with the add_binding_data function"
         assert type(antigen) == str, "You have to give a string as input for the antigen"
         assert type(max_ld) == int, "You have to give an integer as input for the maximum levenshtein distance"
         assert type(min_ld) == int, "You have to give an integer as input for the minimum levenshtein distance"
         assert type(specific_experiments) == list, "You have to give a list with the samples you want to analyze"
         self.fig.clear()
         cluster_single_AG(self.fig,
@@ -446,21 +477,24 @@
         self.style = PlotStyle(self.ax, self.plot_type)
         figManager = plt.get_current_fig_manager()
         figManager.window.showMaximized()
 
     def tsne_cluster_AG(self, sample, antigen,antigen_names = True, pca_components = 70, perplexity = 25, iterations_tsne = 2500):
         """
         :param sample: the sample you would like to analyze
-        :param toxins: the toxins you would like to cluster
-        :param toxin_names: Default is True. Prints the name of the toxin for the corresponding embedded sequence in the plot
+        :param antigen: the toxins you would like to cluster
+        :param antigen_names: Default is True. Prints the name of the toxin for the corresponding embedded sequence in the plot
         :param pca_components: optional. Default is 70
         :param perplexity: optional. Default 25
         :param iterations_tsne: optional. Default is 2500
         :return: It first embeds the sequences in a vector space and then clusters them with PCA and TSNE. The sequences with the binding data are processed with the input sequences, to enable the plotting of the binding data.
         """
+        if not plt.fignum_exists(1):
+            self.fig = plt.figure(1)
+            print("Please do not close the window for the figure while the plot is loading")
         assert self.binding_data is not None, "You have not given binding data. You can add it with the add_binding_data function"
         assert type(sample) == str, "You have to give a string as input for the sample"
         assert sample in self.experiments_list, "The provided sample name is not in your sequencing report. Please check the spelling or use the print_samples function to see the names of your samples"
         assert antigen_names in [True, False], "You have to give True or False as input for the antigen_names parameter"
         assert type(pca_components) == int, "You have to give an integer as input for the pca_components"
         assert type(perplexity) == int, "You have to give an integer as input for the perplexity"
         assert type(iterations_tsne) == int, "You have to give an integer as input for the iterations_tsne"
@@ -500,14 +534,17 @@
         :param samples: the samples you would like to compare towards their sequences
         :param strands: Default is True. It means that you will plot a batch of the strands in your plot
         :param pca_components: Default is 80. Has to be applied for better accuracy of t-SNE. You can indirectly change the described variance with this.
         :param perplexity: Default is 30. It roughly determines the number of nearest neighbors that are considered in the embedding. A higher perplexity value results in a more global structure in the low-dimensional embedding, while a lower perplexity value emphasizes local structure. The optimal perplexity value for a given dataset depends on the dataset's intrinsic dimensionality, and it is usually determined by trial and err
         :param iterations_tsne: Default is 2500. number of times that the algorithm will repeat the optimization process for reducing the cost function. The optimization process aims to minimize the difference between the high-dimensional and low-dimensional representations of the data. More iterations result in a more optimized low-dimensional representation, but also increases the computational cost.
         :return: Returns a plot where the sequences of the input samples are transformed in a vector space. Dimension reduction such as PCA and following t-SNE is used to plot it on a two dimensional space. The different colors indicate the different samples.
         """
+        if not plt.fignum_exists(1):
+            self.fig = plt.figure(1)
+            print("Please do not close the window for the figure while the plot is loading")
         incorrect_samples = [x for x in samples if x not in self.experiments_list]
         assert not incorrect_samples, f"The following sample(s) are not in your sequencing report: {', '.join(incorrect_samples)}. Please check the spelling or use the print_samples function to see the names of your samples"
         assert type(samples) == list, "You have to give a list with the samples you want to analyze"
         assert type(strands) == bool, "You have to give True or False as input for the strands parameter"
         assert type(pca_components) == int, "You have to give an integer as input for the pca_components"
         assert type(perplexity) == int, "You have to give an integer as input for the perplexity"
         assert type(iterations_tsne) == int, "You have to give an integer as input for the iterations_tsne"
@@ -529,14 +566,17 @@
         figManager = plt.get_current_fig_manager()
         figManager.window.showMaximized()
     def morosita_horn(self, specific_samples = False):
         """
         :param specific_experiments: you can give a list with specific experiments
         :return: Returns a matrix of the identity between your samples based on the Morosita Horn Index
         """
+        if not plt.fignum_exists(1):
+            self.fig = plt.figure(1)
+            print("Please do not close the window for the figure while the plot is loading")
         if specific_samples != False:
             assert type(specific_samples) == list, "You have to give a list with the samples you want to analyze"
             incorrect_samples = [x for x in samples if x not in self.experiments_list]
             assert not incorrect_samples, f"The following sample(s) are not in your sequencing report: {', '.join(incorrect_samples)}. Please check the spelling or use the print_samples function to see the names of your samples"
         self.fig.clear()
         self.ax = self.fig.gca()
         plot_heatmap(self.sequencing_report,
@@ -548,21 +588,25 @@
                      specific_experiments = specific_samples,
                      )
         self.plot_type = "single"
         self.ax = self.fig.gca()
         self.style = PlotStyle(self.ax, self.plot_type)
         figManager = plt.get_current_fig_manager()
         figManager.window.showMaximized()
+        return self.fig
 
-
+            
     def jaccard(self, specific_samples = False):
         """
         :param specific_experiments: give a list with specific samples you would like to analyze
         :return: Returns a matrix of the identity between your samples based on the Jaccard Index
         """
+        if not plt.fignum_exists(1):
+            self.fig = plt.figure(1)
+            print("Please do not close the window for the figure while the plot is loading")
         if specific_samples != False:
             assert type(specific_samples) == list, "You have to give a list with the samples you want to analyze"
             incorrect_samples = [x for x in samples if x not in self.experiments_list]
             assert not incorrect_samples, f"The following sample(s) are not in your sequencing report: {', '.join(incorrect_samples)}. Please check the spelling or use the print_samples function to see the names of your samples"
         self.fig.clear()
         self.ax = self.fig.gca()
         plot_heatmap(self.sequencing_report,
@@ -580,14 +624,17 @@
         figManager.window.showMaximized()
 
     def sorensen(self, specific_samples = False):
         """
         :param specific_samples: give a list with specific samples you would like to analyze
         :return: Returns a matrix of the identity between your samples based on the Sorensen Dice Index
         """
+        if not plt.fignum_exists(1):
+            self.fig = plt.figure(1)
+            print("Please do not close the window for the figure while the plot is loading")
         if specific_samples != False:
             assert type(specific_samples) == list, "You have to give a list with the samples you want to analyze"
             incorrect_samples = [x for x in samples if x not in self.experiments_list]
             assert not incorrect_samples, f"The following sample(s) are not in your sequencing report: {', '.join(incorrect_samples)}. Please check the spelling or use the print_samples function to see the names of your samples"
         self.fig.clear()
         self.ax = self.fig.gca()
         plot_heatmap(self.sequencing_report,
@@ -605,14 +652,17 @@
         figManager.window.showMaximized()
 
     def relative(self, specific_samples = False):
         """
         :param specific_samples: give a list with specific samples you would like to analyze
         :return: Returns a matrix of the identity between your samples based on the proportion of identical sequences
         """
+        if not plt.fignum_exists(1):
+            self.fig = plt.figure(1)
+            print("Please do not close the window for the figure while the plot is loading")
         if specific_samples != False:
             assert type(specific_samples) == list, "You have to give a list with the samples you want to analyze"
             incorrect_samples = [x for x in samples if x not in self.experiments_list]
             assert not incorrect_samples, f"The following sample(s) are not in your sequencing report: {', '.join(incorrect_samples)}. Please check the spelling or use the print_samples function to see the names of your samples"
         self.fig.clear()
         self.ax = self.fig.gca()
         plot_heatmap(self.sequencing_report,
```

### Comparing `ExpoSeq-1.1.7/src/ExpoSeq/plots/barplot.py` & `ExpoSeq-1.1.9/src/ExpoSeq/plots/barplot.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.7/src/ExpoSeq/plots/cluster_embedding.py` & `ExpoSeq-1.1.9/src/ExpoSeq/plots/cluster_embedding.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.7/src/ExpoSeq/plots/embedding_with_binding.py` & `ExpoSeq-1.1.9/src/ExpoSeq/plots/embedding_with_binding.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.7/src/ExpoSeq/plots/length_distribution.py` & `ExpoSeq-1.1.9/src/ExpoSeq/plots/length_distribution.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.7/src/ExpoSeq/plots/levenshtein_clustering.py` & `ExpoSeq-1.1.9/src/ExpoSeq/plots/levenshtein_clustering.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.7/src/ExpoSeq/plots/logo_plot.py` & `ExpoSeq-1.1.9/src/ExpoSeq/plots/logo_plot.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.7/src/ExpoSeq/plots/plt_heatmap.py` & `ExpoSeq-1.1.9/src/ExpoSeq/plots/plt_heatmap.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.7/src/ExpoSeq/plots/protvec.py` & `ExpoSeq-1.1.9/src/ExpoSeq/plots/protvec.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.7/src/ExpoSeq/plots/relative_sequence_abundance.py` & `ExpoSeq-1.1.9/src/ExpoSeq/plots/relative_sequence_abundance.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.7/src/ExpoSeq/plots/saveFig.py` & `ExpoSeq-1.1.9/src/ExpoSeq/plots/saveFig.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.7/src/ExpoSeq/plots/stacked_aa_distribution.py` & `ExpoSeq-1.1.9/src/ExpoSeq/plots/stacked_aa_distribution.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.7/src/ExpoSeq/plots/usq_plot.py` & `ExpoSeq-1.1.9/src/ExpoSeq/plots/usq_plot.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.7/src/ExpoSeq/reset.py` & `ExpoSeq-1.1.9/src/ExpoSeq/reset.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.7/src/ExpoSeq/settings/blosum_62.txt` & `ExpoSeq-1.1.9/src/ExpoSeq/settings/blosum_62.txt`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.7/src/ExpoSeq/settings/change_save_settings.py` & `ExpoSeq-1.1.9/src/ExpoSeq/settings/change_save_settings.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.7/src/ExpoSeq/settings/plot_styler.py` & `ExpoSeq-1.1.9/src/ExpoSeq/settings/plot_styler.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.7/src/ExpoSeq/test_data/all_alignment_reports.pickle` & `ExpoSeq-1.1.9/src/ExpoSeq/test_data/all_alignment_reports.pickle`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.7/src/ExpoSeq/test_data/test_files/Chris_main_df.csv` & `ExpoSeq-1.1.9/src/ExpoSeq/test_data/test_files/Chris_main_df.csv`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.7/src/ExpoSeq/test_data/test_files/binding_data.csv` & `ExpoSeq-1.1.9/src/ExpoSeq/test_data/test_files/binding_data.csv`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.7/src/ExpoSeq/test_data/test_files/experiment_names.pickle` & `ExpoSeq-1.1.9/src/ExpoSeq/test_data/test_files/experiment_names.pickle`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.7/src/ExpoSeq/test_data/test_files/sequencing_report.csv` & `ExpoSeq-1.1.9/src/ExpoSeq/test_data/test_files/sequencing_report.csv`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.7/src/ExpoSeq/test_data/test_files/test1.fastq` & `ExpoSeq-1.1.9/src/ExpoSeq/test_data/test_files/test1.fastq`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.7/src/ExpoSeq/test_data/test_files/test2.fastq` & `ExpoSeq-1.1.9/src/ExpoSeq/test_data/test_files/test2.fastq`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.7/src/ExpoSeq/test_data/test_files/test3.fastq` & `ExpoSeq-1.1.9/src/ExpoSeq/test_data/test_files/test3.fastq`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.7/src/ExpoSeq/test_uploader.py` & `ExpoSeq-1.1.9/src/ExpoSeq/test_uploader.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.7/src/ExpoSeq/tidy_data/aminoacid_distribution.py` & `ExpoSeq-1.1.9/src/ExpoSeq/tidy_data/aminoacid_distribution.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.7/src/ExpoSeq/tidy_data/barplot.py` & `ExpoSeq-1.1.9/src/ExpoSeq/tidy_data/barplot.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.7/src/ExpoSeq/tidy_data/clustering.py` & `ExpoSeq-1.1.9/src/ExpoSeq/tidy_data/clustering.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.7/src/ExpoSeq/tidy_data/heatmaps/bool_sequences_matrix.py` & `ExpoSeq-1.1.9/src/ExpoSeq/tidy_data/heatmaps/bool_sequences_matrix.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.7/src/ExpoSeq/tidy_data/heatmaps/tidy_heatmap_share.py` & `ExpoSeq-1.1.9/src/ExpoSeq/tidy_data/heatmaps/tidy_heatmap_share.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.7/src/ExpoSeq/tidy_data/heatmaps/tidy_jaccard.py` & `ExpoSeq-1.1.9/src/ExpoSeq/tidy_data/heatmaps/tidy_jaccard.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.7/src/ExpoSeq/tidy_data/heatmaps/tidy_morosita_horn.py` & `ExpoSeq-1.1.9/src/ExpoSeq/tidy_data/heatmaps/tidy_morosita_horn.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.7/src/ExpoSeq/tidy_data/heatmaps/tidy_sorensen.py` & `ExpoSeq-1.1.9/src/ExpoSeq/tidy_data/heatmaps/tidy_sorensen.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.7/src/ExpoSeq/tidy_data/interpret_data.py` & `ExpoSeq-1.1.9/src/ExpoSeq/tidy_data/interpret_data.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.7/src/ExpoSeq/tidy_data/read_extract_data.py` & `ExpoSeq-1.1.9/src/ExpoSeq/tidy_data/read_extract_data.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.7/src/ExpoSeq/tidy_data/tidy_alignment_reports.py` & `ExpoSeq-1.1.9/src/ExpoSeq/tidy_data/tidy_alignment_reports.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.7/src/ExpoSeq/tidy_data/tidy_cluster_embedding.py` & `ExpoSeq-1.1.9/src/ExpoSeq/tidy_data/tidy_cluster_embedding.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.7/src/ExpoSeq/tidy_data/tidy_rel_sequence_abun.py` & `ExpoSeq-1.1.9/src/ExpoSeq/tidy_data/tidy_rel_sequence_abun.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.7/src/ExpoSeq/tidy_data/tidy_seqlogoPlot.py` & `ExpoSeq-1.1.9/src/ExpoSeq/tidy_data/tidy_seqlogoPlot.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.7/src/ExpoSeq/tidy_data/tidy_stacked_aa_distr.py` & `ExpoSeq-1.1.9/src/ExpoSeq/tidy_data/tidy_stacked_aa_distr.py`

 * *Files identical despite different names*

### Comparing `ExpoSeq-1.1.7/src/ExpoSeq.egg-info/PKG-INFO` & `ExpoSeq-1.1.9/src/ExpoSeq.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: ExpoSeq
-Version: 1.1.7
+Version: 1.1.9
 Summary: A pacakge which provides various ways to analyze NGS data from phage display campaigns
 Home-page: https://github.com/nilshof01/ExpoSeq
 Author: Nils Hofmann
 Author-email: n.hofmann.99@web.de
-License: MIT
+License: Apache License 2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Welcome to ExpoSeq
 
 ExpoSeq is a powerful pipeline for processing and analyzing FASTQ files from sequencing phage Display panning samples.It utilizes [MiXCR](https://docs.milaboratories.com/mixcr/getting-started/installation/) to align and assemble the data which you can subsequently analyze in multiple plots. The pipeline focuses on analysing the identity between samples but also applies various clustering techniques to analyse the relation between the sequences. Besides, you can add binding data to relate the clusters to affinity.  ![overview](expoSeq_overview.png)
```

### Comparing `ExpoSeq-1.1.7/src/ExpoSeq.egg-info/SOURCES.txt` & `ExpoSeq-1.1.9/src/ExpoSeq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

