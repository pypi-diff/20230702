# Comparing `tmp/pyphetools-0.4.1.tar.gz` & `tmp/pyphetools-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyphetools-0.4.1.tar", last modified: Thu Jun 29 14:19:20 2023, max compression
+gzip compressed data, was "pyphetools-0.4.5.tar", last modified: Sun Jul  2 16:47:00 2023, max compression
```

## Comparing `pyphetools-0.4.1.tar` & `pyphetools-0.4.5.tar`

### file list

```diff
@@ -1,84 +1,87 @@
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-06-29 14:19:20.275547 pyphetools-0.4.1/
--rw-rw-r--   0 peter     (1000) peter     (1000)     1079 2023-02-05 19:04:48.000000 pyphetools-0.4.1/LICENSE
--rw-rw-r--   0 peter     (1000) peter     (1000)        0 2022-12-16 00:09:56.000000 pyphetools-0.4.1/MANIFEST.in
--rw-rw-r--   0 peter     (1000) peter     (1000)     2846 2023-06-29 14:19:20.275547 pyphetools-0.4.1/PKG-INFO
--rw-rw-r--   0 peter     (1000) peter     (1000)      767 2023-06-26 23:11:02.000000 pyphetools-0.4.1/README.md
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-06-29 14:19:20.267547 pyphetools-0.4.1/docs/
--rw-rw-r--   0 peter     (1000) peter     (1000)     4165 2023-06-25 22:31:24.000000 pyphetools-0.4.1/docs/conf.py
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-06-29 14:19:20.267547 pyphetools-0.4.1/pyphetools/
--rw-rw-r--   0 peter     (1000) peter     (1000)       11 2023-02-05 19:04:48.000000 pyphetools-0.4.1/pyphetools/__init__.py
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-06-29 14:19:20.267547 pyphetools-0.4.1/pyphetools/analyze/
--rw-rw-r--   0 peter     (1000) peter     (1000)       36 2023-02-05 19:04:48.000000 pyphetools-0.4.1/pyphetools/analyze/__init__.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     3062 2023-06-25 22:31:24.000000 pyphetools-0.4.1/pyphetools/analyze/downsampler.py
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-06-29 14:19:20.271546 pyphetools-0.4.1/pyphetools/creation/
--rw-rw-r--   0 peter     (1000) peter     (1000)      882 2023-06-29 12:30:59.000000 pyphetools-0.4.1/pyphetools/creation/__init__.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     4873 2023-05-11 10:59:47.000000 pyphetools-0.4.1/pyphetools/creation/age_column_mapper.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     7929 2023-06-29 13:53:18.000000 pyphetools-0.4.1/pyphetools/creation/case_encoder.py
--rw-rw-r--   0 peter     (1000) peter     (1000)    10828 2023-06-29 12:55:59.000000 pyphetools-0.4.1/pyphetools/creation/cohort_encoder.py
--rw-rw-r--   0 peter     (1000) peter     (1000)      531 2023-05-10 19:30:33.000000 pyphetools-0.4.1/pyphetools/creation/column_mapper.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     2339 2023-06-25 22:31:24.000000 pyphetools-0.4.1/pyphetools/creation/constant_column_mapper.py
--rw-rw-r--   0 peter     (1000) peter     (1000)      308 2023-05-07 14:22:13.000000 pyphetools-0.4.1/pyphetools/creation/constants.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     3014 2023-05-11 13:07:39.000000 pyphetools-0.4.1/pyphetools/creation/custom_column_mapper.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     5506 2023-06-29 11:35:00.000000 pyphetools-0.4.1/pyphetools/creation/hgvs_variant.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     3281 2023-06-25 20:29:31.000000 pyphetools-0.4.1/pyphetools/creation/hp_term.py
--rw-rw-r--   0 peter     (1000) peter     (1000)      740 2023-05-11 10:59:47.000000 pyphetools-0.4.1/pyphetools/creation/hpo_cr.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     7207 2023-06-27 16:06:41.000000 pyphetools-0.4.1/pyphetools/creation/hpo_exact_cr.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     6926 2023-06-27 17:37:13.000000 pyphetools-0.4.1/pyphetools/creation/hpo_parser.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     7515 2023-06-29 13:36:57.000000 pyphetools-0.4.1/pyphetools/creation/individual.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     5795 2023-06-25 22:31:24.000000 pyphetools-0.4.1/pyphetools/creation/metadata.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     3541 2023-06-26 12:01:47.000000 pyphetools-0.4.1/pyphetools/creation/option_column_mapper.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     2194 2023-05-17 14:42:11.000000 pyphetools-0.4.1/pyphetools/creation/sex_column_mapper.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     4678 2023-05-13 00:28:58.000000 pyphetools-0.4.1/pyphetools/creation/simple_column_mapper.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     6969 2023-06-29 11:43:08.000000 pyphetools-0.4.1/pyphetools/creation/structural_variant.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     2656 2023-05-11 11:04:54.000000 pyphetools-0.4.1/pyphetools/creation/thresholded_column_mapper.py
--rw-rw-r--   0 peter     (1000) peter     (1000)      268 2023-06-29 11:43:15.000000 pyphetools-0.4.1/pyphetools/creation/variant.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     5641 2023-06-29 13:35:41.000000 pyphetools-0.4.1/pyphetools/creation/variant_column_mapper.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     3240 2023-06-29 12:52:03.000000 pyphetools-0.4.1/pyphetools/creation/variant_validator.py
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-06-29 14:19:20.271546 pyphetools-0.4.1/pyphetools/output/
--rw-rw-r--   0 peter     (1000) peter     (1000)      327 2023-06-24 19:26:58.000000 pyphetools-0.4.1/pyphetools/output/__init__.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     3067 2023-06-25 22:31:24.000000 pyphetools-0.4.1/pyphetools/output/detailed_suppl_table.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     5727 2023-06-25 22:31:24.000000 pyphetools-0.4.1/pyphetools/output/focus_count_table.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     2980 2023-02-05 19:04:49.000000 pyphetools-0.4.1/pyphetools/output/hpo_category.py
--rw-rw-r--   0 peter     (1000) peter     (1000)      894 2023-02-05 19:04:49.000000 pyphetools-0.4.1/pyphetools/output/phenopacket_ingestor.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     2154 2023-06-24 20:06:45.000000 pyphetools-0.4.1/pyphetools/output/phenopacket_table.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     4960 2023-06-24 20:15:49.000000 pyphetools-0.4.1/pyphetools/output/simple_patient.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     3310 2023-06-24 20:23:41.000000 pyphetools-0.4.1/pyphetools/output/simple_variant.py
--rw-rw-r--   0 peter     (1000) peter     (1000)      569 2023-05-11 10:59:47.000000 pyphetools-0.4.1/pyphetools/output/term_count.py
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-06-29 14:19:20.271546 pyphetools-0.4.1/pyphetools/validation/
--rw-rw-r--   0 peter     (1000) peter     (1000)        8 2023-06-25 22:31:24.000000 pyphetools-0.4.1/pyphetools/validation/__init__.py
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-06-29 14:19:20.267547 pyphetools-0.4.1/pyphetools.egg-info/
--rw-rw-r--   0 peter     (1000) peter     (1000)     2846 2023-06-29 14:19:20.000000 pyphetools-0.4.1/pyphetools.egg-info/PKG-INFO
--rw-rw-r--   0 peter     (1000) peter     (1000)     2193 2023-06-29 14:19:20.000000 pyphetools-0.4.1/pyphetools.egg-info/SOURCES.txt
--rw-rw-r--   0 peter     (1000) peter     (1000)        1 2023-06-29 14:19:20.000000 pyphetools-0.4.1/pyphetools.egg-info/dependency_links.txt
--rw-rw-r--   0 peter     (1000) peter     (1000)       81 2023-06-29 14:19:20.000000 pyphetools-0.4.1/pyphetools.egg-info/requires.txt
--rw-rw-r--   0 peter     (1000) peter     (1000)       56 2023-06-29 14:19:20.000000 pyphetools-0.4.1/pyphetools.egg-info/top_level.txt
--rw-rw-r--   0 peter     (1000) peter     (1000)     1367 2023-06-29 14:18:46.000000 pyphetools-0.4.1/pyproject.toml
--rw-rw-r--   0 peter     (1000) peter     (1000)       38 2023-06-29 14:19:20.275547 pyphetools-0.4.1/setup.cfg
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-06-29 14:19:20.271546 pyphetools-0.4.1/test/
--rw-rw-r--   0 peter     (1000) peter     (1000)     3297 2023-02-05 19:04:49.000000 pyphetools-0.4.1/test/test_age_column_mapper.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     3370 2023-06-29 13:58:19.000000 pyphetools-0.4.1/test/test_case_encoder.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     4553 2023-05-10 22:56:45.000000 pyphetools-0.4.1/test/test_column_mapper.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     1156 2023-05-12 23:59:19.000000 pyphetools-0.4.1/test/test_constant_column_mapper.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     2745 2023-05-14 12:05:29.000000 pyphetools-0.4.1/test/test_custom_column_mapper.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     1430 2023-06-23 21:44:02.000000 pyphetools-0.4.1/test/test_hp_term.py
--rw-rw-r--   0 peter     (1000) peter     (1000)      914 2023-02-05 19:04:49.000000 pyphetools-0.4.1/test/test_hpo_category.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     5966 2023-05-11 14:18:42.000000 pyphetools-0.4.1/test/test_hpo_cr.py
--rw-rw-r--   0 peter     (1000) peter     (1000)      835 2023-06-27 16:07:00.000000 pyphetools-0.4.1/test/test_hpo_parser.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     5385 2023-06-26 12:00:47.000000 pyphetools-0.4.1/test/test_option_column_mapper.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     1648 2023-06-28 18:34:15.000000 pyphetools-0.4.1/test/test_structural_variant.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     1856 2023-05-11 14:18:42.000000 pyphetools-0.4.1/test/test_threshold_column_mapper.py
--rw-rw-r--   0 peter     (1000) peter     (1000)     1447 2023-06-29 12:31:36.000000 pyphetools-0.4.1/test/test_variant.py
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-06-29 14:19:20.267547 pyphetools-0.4.1/venv/
-drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-06-29 14:19:20.275547 pyphetools-0.4.1/venv/bin/
--rwxrwxr-x   0 peter     (1000) peter     (1000)      621 2022-12-06 12:58:50.000000 pyphetools-0.4.1/venv/bin/rst2html.py
--rwxrwxr-x   0 peter     (1000) peter     (1000)      741 2022-12-06 12:58:50.000000 pyphetools-0.4.1/venv/bin/rst2html4.py
--rwxrwxr-x   0 peter     (1000) peter     (1000)     1109 2022-12-06 12:58:50.000000 pyphetools-0.4.1/venv/bin/rst2html5.py
--rwxrwxr-x   0 peter     (1000) peter     (1000)      818 2022-12-06 12:58:50.000000 pyphetools-0.4.1/venv/bin/rst2latex.py
--rwxrwxr-x   0 peter     (1000) peter     (1000)      626 2022-12-06 12:58:50.000000 pyphetools-0.4.1/venv/bin/rst2man.py
--rwxrwxr-x   0 peter     (1000) peter     (1000)      791 2022-12-06 12:58:50.000000 pyphetools-0.4.1/venv/bin/rst2odt.py
--rwxrwxr-x   0 peter     (1000) peter     (1000)     1753 2022-12-06 12:58:50.000000 pyphetools-0.4.1/venv/bin/rst2odt_prepstyles.py
--rwxrwxr-x   0 peter     (1000) peter     (1000)      628 2022-12-06 12:58:50.000000 pyphetools-0.4.1/venv/bin/rst2pseudoxml.py
--rwxrwxr-x   0 peter     (1000) peter     (1000)      664 2022-12-06 12:58:50.000000 pyphetools-0.4.1/venv/bin/rst2s5.py
--rwxrwxr-x   0 peter     (1000) peter     (1000)      898 2022-12-06 12:58:50.000000 pyphetools-0.4.1/venv/bin/rst2xetex.py
--rwxrwxr-x   0 peter     (1000) peter     (1000)      629 2022-12-06 12:58:50.000000 pyphetools-0.4.1/venv/bin/rst2xml.py
--rwxrwxr-x   0 peter     (1000) peter     (1000)      697 2022-12-06 12:58:50.000000 pyphetools-0.4.1/venv/bin/rstpep2html.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-07-02 16:47:00.007690 pyphetools-0.4.5/
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1079 2023-02-05 19:04:48.000000 pyphetools-0.4.5/LICENSE
+-rw-rw-r--   0 peter     (1000) peter     (1000)        0 2022-12-16 00:09:56.000000 pyphetools-0.4.5/MANIFEST.in
+-rw-rw-r--   0 peter     (1000) peter     (1000)     2846 2023-07-02 16:47:00.007690 pyphetools-0.4.5/PKG-INFO
+-rw-rw-r--   0 peter     (1000) peter     (1000)      767 2023-06-26 23:11:02.000000 pyphetools-0.4.5/README.md
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-07-02 16:46:59.963690 pyphetools-0.4.5/docs/
+-rw-rw-r--   0 peter     (1000) peter     (1000)     4165 2023-06-25 22:31:24.000000 pyphetools-0.4.5/docs/conf.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-07-02 16:46:59.963690 pyphetools-0.4.5/pyphetools/
+-rw-rw-r--   0 peter     (1000) peter     (1000)       11 2023-02-05 19:04:48.000000 pyphetools-0.4.5/pyphetools/__init__.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-07-02 16:46:59.963690 pyphetools-0.4.5/pyphetools/analyze/
+-rw-rw-r--   0 peter     (1000) peter     (1000)       36 2023-02-05 19:04:48.000000 pyphetools-0.4.5/pyphetools/analyze/__init__.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     3062 2023-06-25 22:31:24.000000 pyphetools-0.4.5/pyphetools/analyze/downsampler.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-07-02 16:46:59.967690 pyphetools-0.4.5/pyphetools/creation/
+-rw-rw-r--   0 peter     (1000) peter     (1000)      882 2023-06-29 12:30:59.000000 pyphetools-0.4.5/pyphetools/creation/__init__.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     4873 2023-05-11 10:59:47.000000 pyphetools-0.4.5/pyphetools/creation/age_column_mapper.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     7929 2023-06-29 13:53:18.000000 pyphetools-0.4.5/pyphetools/creation/case_encoder.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)    10828 2023-06-29 12:55:59.000000 pyphetools-0.4.5/pyphetools/creation/cohort_encoder.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)      531 2023-05-10 19:30:33.000000 pyphetools-0.4.5/pyphetools/creation/column_mapper.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     2339 2023-06-25 22:31:24.000000 pyphetools-0.4.5/pyphetools/creation/constant_column_mapper.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)      308 2023-05-07 14:22:13.000000 pyphetools-0.4.5/pyphetools/creation/constants.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     3014 2023-05-11 13:07:39.000000 pyphetools-0.4.5/pyphetools/creation/custom_column_mapper.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     5506 2023-06-29 11:35:00.000000 pyphetools-0.4.5/pyphetools/creation/hgvs_variant.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     3281 2023-06-25 20:29:31.000000 pyphetools-0.4.5/pyphetools/creation/hp_term.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)      740 2023-05-11 10:59:47.000000 pyphetools-0.4.5/pyphetools/creation/hpo_cr.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     7207 2023-06-27 16:06:41.000000 pyphetools-0.4.5/pyphetools/creation/hpo_exact_cr.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     6926 2023-06-27 17:37:13.000000 pyphetools-0.4.5/pyphetools/creation/hpo_parser.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     7515 2023-06-29 13:36:57.000000 pyphetools-0.4.5/pyphetools/creation/individual.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     6402 2023-06-29 15:58:37.000000 pyphetools-0.4.5/pyphetools/creation/metadata.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     6257 2023-07-02 16:29:47.000000 pyphetools-0.4.5/pyphetools/creation/option_column_mapper.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     2194 2023-05-17 14:42:11.000000 pyphetools-0.4.5/pyphetools/creation/sex_column_mapper.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     4678 2023-05-13 00:28:58.000000 pyphetools-0.4.5/pyphetools/creation/simple_column_mapper.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     6969 2023-06-29 11:43:08.000000 pyphetools-0.4.5/pyphetools/creation/structural_variant.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     2656 2023-05-11 11:04:54.000000 pyphetools-0.4.5/pyphetools/creation/thresholded_column_mapper.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)      268 2023-06-29 11:43:15.000000 pyphetools-0.4.5/pyphetools/creation/variant.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     5641 2023-06-29 13:35:41.000000 pyphetools-0.4.5/pyphetools/creation/variant_column_mapper.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     3240 2023-06-29 12:52:03.000000 pyphetools-0.4.5/pyphetools/creation/variant_validator.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-07-02 16:46:59.967690 pyphetools-0.4.5/pyphetools/output/
+-rw-rw-r--   0 peter     (1000) peter     (1000)      327 2023-06-24 19:26:58.000000 pyphetools-0.4.5/pyphetools/output/__init__.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     3067 2023-06-25 22:31:24.000000 pyphetools-0.4.5/pyphetools/output/detailed_suppl_table.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     5727 2023-06-25 22:31:24.000000 pyphetools-0.4.5/pyphetools/output/focus_count_table.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     2980 2023-02-05 19:04:49.000000 pyphetools-0.4.5/pyphetools/output/hpo_category.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)      894 2023-02-05 19:04:49.000000 pyphetools-0.4.5/pyphetools/output/phenopacket_ingestor.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     2154 2023-06-24 20:06:45.000000 pyphetools-0.4.5/pyphetools/output/phenopacket_table.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     4960 2023-06-24 20:15:49.000000 pyphetools-0.4.5/pyphetools/output/simple_patient.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     3310 2023-06-24 20:23:41.000000 pyphetools-0.4.5/pyphetools/output/simple_variant.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)      569 2023-05-11 10:59:47.000000 pyphetools-0.4.5/pyphetools/output/term_count.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-07-02 16:46:59.967690 pyphetools-0.4.5/pyphetools/validation/
+-rw-rw-r--   0 peter     (1000) peter     (1000)      111 2023-06-29 14:50:29.000000 pyphetools-0.4.5/pyphetools/validation/__init__.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     3792 2023-06-29 17:31:14.000000 pyphetools-0.4.5/pyphetools/validation/content_validator.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)      187 2023-06-29 14:49:26.000000 pyphetools-0.4.5/pyphetools/validation/phenopacket_validator.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1115 2023-06-29 17:46:07.000000 pyphetools-0.4.5/pyphetools/validation/validation_result.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-07-02 16:46:59.963690 pyphetools-0.4.5/pyphetools.egg-info/
+-rw-rw-r--   0 peter     (1000) peter     (1000)     2846 2023-07-02 16:46:59.000000 pyphetools-0.4.5/pyphetools.egg-info/PKG-INFO
+-rw-rw-r--   0 peter     (1000) peter     (1000)     2326 2023-07-02 16:46:59.000000 pyphetools-0.4.5/pyphetools.egg-info/SOURCES.txt
+-rw-rw-r--   0 peter     (1000) peter     (1000)        1 2023-07-02 16:46:59.000000 pyphetools-0.4.5/pyphetools.egg-info/dependency_links.txt
+-rw-rw-r--   0 peter     (1000) peter     (1000)       81 2023-07-02 16:46:59.000000 pyphetools-0.4.5/pyphetools.egg-info/requires.txt
+-rw-rw-r--   0 peter     (1000) peter     (1000)       56 2023-07-02 16:46:59.000000 pyphetools-0.4.5/pyphetools.egg-info/top_level.txt
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1367 2023-07-02 16:30:04.000000 pyphetools-0.4.5/pyproject.toml
+-rw-rw-r--   0 peter     (1000) peter     (1000)       38 2023-07-02 16:47:00.007690 pyphetools-0.4.5/setup.cfg
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-07-02 16:46:59.967690 pyphetools-0.4.5/test/
+-rw-rw-r--   0 peter     (1000) peter     (1000)     3297 2023-02-05 19:04:49.000000 pyphetools-0.4.5/test/test_age_column_mapper.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     3370 2023-06-29 13:58:19.000000 pyphetools-0.4.5/test/test_case_encoder.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     4553 2023-05-10 22:56:45.000000 pyphetools-0.4.5/test/test_column_mapper.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1156 2023-05-12 23:59:19.000000 pyphetools-0.4.5/test/test_constant_column_mapper.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     2745 2023-05-14 12:05:29.000000 pyphetools-0.4.5/test/test_custom_column_mapper.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1430 2023-06-23 21:44:02.000000 pyphetools-0.4.5/test/test_hp_term.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)      914 2023-02-05 19:04:49.000000 pyphetools-0.4.5/test/test_hpo_category.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     5966 2023-05-11 14:18:42.000000 pyphetools-0.4.5/test/test_hpo_cr.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)      835 2023-06-27 16:07:00.000000 pyphetools-0.4.5/test/test_hpo_parser.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     5385 2023-06-26 12:00:47.000000 pyphetools-0.4.5/test/test_option_column_mapper.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1648 2023-06-28 18:34:15.000000 pyphetools-0.4.5/test/test_structural_variant.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1856 2023-05-11 14:18:42.000000 pyphetools-0.4.5/test/test_threshold_column_mapper.py
+-rw-rw-r--   0 peter     (1000) peter     (1000)     1447 2023-06-29 12:31:36.000000 pyphetools-0.4.5/test/test_variant.py
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-07-02 16:46:59.963690 pyphetools-0.4.5/venv/
+drwxrwxr-x   0 peter     (1000) peter     (1000)        0 2023-07-02 16:47:00.007690 pyphetools-0.4.5/venv/bin/
+-rwxrwxr-x   0 peter     (1000) peter     (1000)      621 2022-12-06 12:58:50.000000 pyphetools-0.4.5/venv/bin/rst2html.py
+-rwxrwxr-x   0 peter     (1000) peter     (1000)      741 2022-12-06 12:58:50.000000 pyphetools-0.4.5/venv/bin/rst2html4.py
+-rwxrwxr-x   0 peter     (1000) peter     (1000)     1109 2022-12-06 12:58:50.000000 pyphetools-0.4.5/venv/bin/rst2html5.py
+-rwxrwxr-x   0 peter     (1000) peter     (1000)      818 2022-12-06 12:58:50.000000 pyphetools-0.4.5/venv/bin/rst2latex.py
+-rwxrwxr-x   0 peter     (1000) peter     (1000)      626 2022-12-06 12:58:50.000000 pyphetools-0.4.5/venv/bin/rst2man.py
+-rwxrwxr-x   0 peter     (1000) peter     (1000)      791 2022-12-06 12:58:50.000000 pyphetools-0.4.5/venv/bin/rst2odt.py
+-rwxrwxr-x   0 peter     (1000) peter     (1000)     1753 2022-12-06 12:58:50.000000 pyphetools-0.4.5/venv/bin/rst2odt_prepstyles.py
+-rwxrwxr-x   0 peter     (1000) peter     (1000)      628 2022-12-06 12:58:50.000000 pyphetools-0.4.5/venv/bin/rst2pseudoxml.py
+-rwxrwxr-x   0 peter     (1000) peter     (1000)      664 2022-12-06 12:58:50.000000 pyphetools-0.4.5/venv/bin/rst2s5.py
+-rwxrwxr-x   0 peter     (1000) peter     (1000)      898 2022-12-06 12:58:50.000000 pyphetools-0.4.5/venv/bin/rst2xetex.py
+-rwxrwxr-x   0 peter     (1000) peter     (1000)      629 2022-12-06 12:58:50.000000 pyphetools-0.4.5/venv/bin/rst2xml.py
+-rwxrwxr-x   0 peter     (1000) peter     (1000)      697 2022-12-06 12:58:50.000000 pyphetools-0.4.5/venv/bin/rstpep2html.py
```

### Comparing `pyphetools-0.4.1/LICENSE` & `pyphetools-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.1/PKG-INFO` & `pyphetools-0.4.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyphetools
-Version: 0.4.1
+Version: 0.4.5
 Summary: Generate and work with GA4GH phenopackets
 Author-email: Peter Robinson <peter.robinson@jax.org>
 License: MIT License
         
         Copyright (c) 2023, The Monarch Initiative
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pyphetools-0.4.1/README.md` & `pyphetools-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.1/docs/conf.py` & `pyphetools-0.4.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.1/pyphetools/analyze/downsampler.py` & `pyphetools-0.4.5/pyphetools/analyze/downsampler.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.1/pyphetools/creation/__init__.py` & `pyphetools-0.4.5/pyphetools/creation/__init__.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.1/pyphetools/creation/age_column_mapper.py` & `pyphetools-0.4.5/pyphetools/creation/age_column_mapper.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.1/pyphetools/creation/case_encoder.py` & `pyphetools-0.4.5/pyphetools/creation/case_encoder.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.1/pyphetools/creation/cohort_encoder.py` & `pyphetools-0.4.5/pyphetools/creation/cohort_encoder.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.1/pyphetools/creation/column_mapper.py` & `pyphetools-0.4.5/pyphetools/creation/column_mapper.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.1/pyphetools/creation/constant_column_mapper.py` & `pyphetools-0.4.5/pyphetools/creation/constant_column_mapper.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.1/pyphetools/creation/custom_column_mapper.py` & `pyphetools-0.4.5/pyphetools/creation/custom_column_mapper.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.1/pyphetools/creation/hgvs_variant.py` & `pyphetools-0.4.5/pyphetools/creation/hgvs_variant.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.1/pyphetools/creation/hp_term.py` & `pyphetools-0.4.5/pyphetools/creation/hp_term.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.1/pyphetools/creation/hpo_cr.py` & `pyphetools-0.4.5/pyphetools/creation/hpo_cr.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.1/pyphetools/creation/hpo_exact_cr.py` & `pyphetools-0.4.5/pyphetools/creation/hpo_exact_cr.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.1/pyphetools/creation/hpo_parser.py` & `pyphetools-0.4.5/pyphetools/creation/hpo_parser.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.1/pyphetools/creation/individual.py` & `pyphetools-0.4.5/pyphetools/creation/individual.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.1/pyphetools/creation/metadata.py` & `pyphetools-0.4.5/pyphetools/creation/metadata.py`

 * *Files 7% similar despite different names*

```diff
@@ -49,15 +49,16 @@
 # of the HPO and users can get that from the HPO file and this should be
 # provided in the constructor of metadata
 
 default_versions = {
     'geno': '2022-03-05',
     'hgnc': '06/01/23',
     'omim': 'January 4, 2023',
-    'mondo': 'v2023-01-04'
+    'mondo': 'v2023-01-04',
+    'so': "2021-11-22"
 }
 
 
 class MetaData:
     """
     A representation of the MetaData element of the GA4GH Phenopacket Schema
     """
@@ -71,14 +72,15 @@
         """
         Add resources for HPO (with specified version), GENO, HGNC, and OMIM (with default versions)
         The HPO version can be easily obtained from the HpoParser using the get_version() function
         """
         self.geno()
         self.hgnc()
         self.omim()
+        self.sequence_ontology()
         self.hpo(version=version)
 
     def hpo(self, version):
         self._resource_d["hp"] = Resource(resource_id="hp",
                                           name="human phenotype ontology",
                                           namespace_prefix="HP",
                                           iriprefix="http://purl.obolibrary.org/obo/HP_",
@@ -121,14 +123,23 @@
     def mondo(self, version=default_versions.get('mondo')):
         self._resource_d["mondo"] = Resource(resource_id="mondo",
                                              name="Mondo Disease Ontology",
                                              namespace_prefix="MONDO",
                                              iriprefix="http://purl.obolibrary.org/obo/MONDO_",
                                              url="http://purl.obolibrary.org/obo/mondo.obo",
                                              version=version)
+        
+    def sequence_ontology(self, version=default_versions.get("so")):
+        self._resource_d["so"] = Resource(resource_id="so",
+                                             name="Sequence types and features ontology",
+                                             namespace_prefix="SO",
+                                             iriprefix="http://purl.obolibrary.org/obo/SO_",
+                                             url="http://purl.obolibrary.org/obo/so.obo",
+                                             version=version)
+        
 
     def to_ga4gh(self):
         """
         Use a time stamp for the current instant
         """
         metadata = phenopackets.MetaData()
         metadata.created_by = self._created_by
```

### Comparing `pyphetools-0.4.1/pyphetools/creation/sex_column_mapper.py` & `pyphetools-0.4.5/pyphetools/creation/sex_column_mapper.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.1/pyphetools/creation/simple_column_mapper.py` & `pyphetools-0.4.5/pyphetools/creation/simple_column_mapper.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.1/pyphetools/creation/structural_variant.py` & `pyphetools-0.4.5/pyphetools/creation/structural_variant.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.1/pyphetools/creation/thresholded_column_mapper.py` & `pyphetools-0.4.5/pyphetools/creation/thresholded_column_mapper.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.1/pyphetools/creation/variant_column_mapper.py` & `pyphetools-0.4.5/pyphetools/creation/variant_column_mapper.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.1/pyphetools/creation/variant_validator.py` & `pyphetools-0.4.5/pyphetools/creation/variant_validator.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.1/pyphetools/output/detailed_suppl_table.py` & `pyphetools-0.4.5/pyphetools/output/detailed_suppl_table.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.1/pyphetools/output/focus_count_table.py` & `pyphetools-0.4.5/pyphetools/output/focus_count_table.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.1/pyphetools/output/hpo_category.py` & `pyphetools-0.4.5/pyphetools/output/hpo_category.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.1/pyphetools/output/phenopacket_ingestor.py` & `pyphetools-0.4.5/pyphetools/output/phenopacket_ingestor.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.1/pyphetools/output/phenopacket_table.py` & `pyphetools-0.4.5/pyphetools/output/phenopacket_table.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.1/pyphetools/output/simple_patient.py` & `pyphetools-0.4.5/pyphetools/output/simple_patient.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.1/pyphetools/output/simple_variant.py` & `pyphetools-0.4.5/pyphetools/output/simple_variant.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.1/pyphetools/output/term_count.py` & `pyphetools-0.4.5/pyphetools/output/term_count.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.1/pyphetools.egg-info/PKG-INFO` & `pyphetools-0.4.5/pyphetools.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyphetools
-Version: 0.4.1
+Version: 0.4.5
 Summary: Generate and work with GA4GH phenopackets
 Author-email: Peter Robinson <peter.robinson@jax.org>
 License: MIT License
         
         Copyright (c) 2023, The Monarch Initiative
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pyphetools-0.4.1/pyphetools.egg-info/SOURCES.txt` & `pyphetools-0.4.5/pyphetools.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -40,14 +40,17 @@
 pyphetools/output/hpo_category.py
 pyphetools/output/phenopacket_ingestor.py
 pyphetools/output/phenopacket_table.py
 pyphetools/output/simple_patient.py
 pyphetools/output/simple_variant.py
 pyphetools/output/term_count.py
 pyphetools/validation/__init__.py
+pyphetools/validation/content_validator.py
+pyphetools/validation/phenopacket_validator.py
+pyphetools/validation/validation_result.py
 test/test_age_column_mapper.py
 test/test_case_encoder.py
 test/test_column_mapper.py
 test/test_constant_column_mapper.py
 test/test_custom_column_mapper.py
 test/test_hp_term.py
 test/test_hpo_category.py
```

### Comparing `pyphetools-0.4.1/pyproject.toml` & `pyphetools-0.4.5/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 [tool.setuptools.packages.find]
 where = ["."]
 exclude = ["notebooks", "test"]
 
 [project]
 name = "pyphetools"
-version = "0.4.1"
+version = "0.4.5"
 requires-python = ">=3.5"
 description = "Generate and work with GA4GH phenopackets"
 readme = "README.md"
 authors = [
     {name = "Peter Robinson", email="peter.robinson@jax.org"},
      ]
 license = { file = "LICENSE" }
```

### Comparing `pyphetools-0.4.1/test/test_age_column_mapper.py` & `pyphetools-0.4.5/test/test_age_column_mapper.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.1/test/test_case_encoder.py` & `pyphetools-0.4.5/test/test_case_encoder.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.1/test/test_column_mapper.py` & `pyphetools-0.4.5/test/test_column_mapper.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.1/test/test_constant_column_mapper.py` & `pyphetools-0.4.5/test/test_constant_column_mapper.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.1/test/test_custom_column_mapper.py` & `pyphetools-0.4.5/test/test_custom_column_mapper.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.1/test/test_hp_term.py` & `pyphetools-0.4.5/test/test_hp_term.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.1/test/test_hpo_category.py` & `pyphetools-0.4.5/test/test_hpo_category.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.1/test/test_hpo_cr.py` & `pyphetools-0.4.5/test/test_hpo_cr.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.1/test/test_hpo_parser.py` & `pyphetools-0.4.5/test/test_hpo_parser.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.1/test/test_option_column_mapper.py` & `pyphetools-0.4.5/test/test_option_column_mapper.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.1/test/test_structural_variant.py` & `pyphetools-0.4.5/test/test_structural_variant.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.1/test/test_threshold_column_mapper.py` & `pyphetools-0.4.5/test/test_threshold_column_mapper.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.1/test/test_variant.py` & `pyphetools-0.4.5/test/test_variant.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.1/venv/bin/rst2html.py` & `pyphetools-0.4.5/venv/bin/rst2html.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.1/venv/bin/rst2html4.py` & `pyphetools-0.4.5/venv/bin/rst2html4.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.1/venv/bin/rst2html5.py` & `pyphetools-0.4.5/venv/bin/rst2html5.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.1/venv/bin/rst2latex.py` & `pyphetools-0.4.5/venv/bin/rst2latex.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.1/venv/bin/rst2man.py` & `pyphetools-0.4.5/venv/bin/rst2man.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.1/venv/bin/rst2odt.py` & `pyphetools-0.4.5/venv/bin/rst2odt.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.1/venv/bin/rst2odt_prepstyles.py` & `pyphetools-0.4.5/venv/bin/rst2odt_prepstyles.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.1/venv/bin/rst2pseudoxml.py` & `pyphetools-0.4.5/venv/bin/rst2pseudoxml.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.1/venv/bin/rst2s5.py` & `pyphetools-0.4.5/venv/bin/rst2s5.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.1/venv/bin/rst2xetex.py` & `pyphetools-0.4.5/venv/bin/rst2xetex.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.1/venv/bin/rst2xml.py` & `pyphetools-0.4.5/venv/bin/rst2xml.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.4.1/venv/bin/rstpep2html.py` & `pyphetools-0.4.5/venv/bin/rstpep2html.py`

 * *Files identical despite different names*

