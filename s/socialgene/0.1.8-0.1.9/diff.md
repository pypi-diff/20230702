# Comparing `tmp/socialgene-0.1.8.tar.gz` & `tmp/socialgene-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "socialgene-0.1.8.tar", last modified: Thu Jun 22 18:04:03 2023, max compression
+gzip compressed data, was "socialgene-0.1.9.tar", last modified: Sun Jul  2 17:07:30 2023, max compression
```

## Comparing `socialgene-0.1.8.tar` & `socialgene-0.1.9.tar`

### file list

```diff
@@ -1,106 +1,105 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:04:03.621478 socialgene-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-22 18:03:50.000000 socialgene-0.1.8/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-06-22 18:04:03.621478 socialgene-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-06-22 18:03:50.000000 socialgene-0.1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-06-22 18:03:50.000000 socialgene-0.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-06-22 18:04:03.621478 socialgene-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-06-22 18:03:50.000000 socialgene-0.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:04:03.605477 socialgene-0.1.8/socialgene/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:03:50.000000 socialgene-0.1.8/socialgene/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:04:03.605477 socialgene-0.1.8/socialgene/base/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:03:50.000000 socialgene-0.1.8/socialgene/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8612 2023-06-22 18:03:50.000000 socialgene-0.1.8/socialgene/base/compare_protein.py
--rw-r--r--   0 runner    (1001) docker     (123)    20436 2023-06-22 18:03:50.000000 socialgene-0.1.8/socialgene/base/molbio.py
--rw-r--r--   0 runner    (1001) docker     (123)    26075 2023-06-22 18:03:50.000000 socialgene-0.1.8/socialgene/base/socialgene.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:04:03.609477 socialgene-0.1.8/socialgene/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:03:50.000000 socialgene-0.1.8/socialgene/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-06-22 18:03:50.000000 socialgene-0.1.8/socialgene/cli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-06-22 18:03:50.000000 socialgene-0.1.8/socialgene/cli/clean_hmms.py
--rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-06-22 18:03:50.000000 socialgene-0.1.8/socialgene/cli/create_neo4j_db.py
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-06-22 18:03:50.000000 socialgene-0.1.8/socialgene/cli/export_neo4j_header_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-06-22 18:03:50.000000 socialgene-0.1.8/socialgene/cli/export_protein_loci_assembly_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-06-22 18:03:50.000000 socialgene-0.1.8/socialgene/cli/parameter_export.py
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-06-22 18:03:50.000000 socialgene-0.1.8/socialgene/cli/parse_ncbi_feature_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-06-22 18:03:50.000000 socialgene-0.1.8/socialgene/cli/parse_ncbi_taxonomy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-06-22 18:03:50.000000 socialgene-0.1.8/socialgene/cli/process_domtblout.py
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-06-22 18:03:50.000000 socialgene-0.1.8/socialgene/cli/protein_sqlite.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-06-22 18:03:50.000000 socialgene-0.1.8/socialgene/cli/socialgene_hmm_tsv_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:04:03.609477 socialgene-0.1.8/socialgene/clustermap/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:03:50.000000 socialgene-0.1.8/socialgene/clustermap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9860 2023-06-22 18:03:50.000000 socialgene-0.1.8/socialgene/clustermap/clustermap.py
--rw-r--r--   0 runner    (1001) docker     (123)     4128 2023-06-22 18:03:50.000000 socialgene-0.1.8/socialgene/common_parameters.env
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-06-22 18:03:50.000000 socialgene-0.1.8/socialgene/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:04:03.609477 socialgene-0.1.8/socialgene/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:03:50.000000 socialgene-0.1.8/socialgene/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8067 2023-06-22 18:03:50.000000 socialgene-0.1.8/socialgene/data/biosample_attributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:04:03.609477 socialgene-0.1.8/socialgene/findmybgc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:03:50.000000 socialgene-0.1.8/socialgene/findmybgc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10106 2023-06-22 18:03:50.000000 socialgene-0.1.8/socialgene/findmybgc/findmybgc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:04:03.609477 socialgene-0.1.8/socialgene/hashing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:03:50.000000 socialgene-0.1.8/socialgene/hashing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-06-22 18:03:50.000000 socialgene-0.1.8/socialgene/hashing/hashing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:04:03.609477 socialgene-0.1.8/socialgene/hmm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:03:50.000000 socialgene-0.1.8/socialgene/hmm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6020 2023-06-22 18:03:50.000000 socialgene-0.1.8/socialgene/hmm/hmmer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-06-22 18:03:50.000000 socialgene-0.1.8/socialgene/hmm/hmminfo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:04:03.613478 socialgene-0.1.8/socialgene/mmseqs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:03:50.000000 socialgene-0.1.8/socialgene/mmseqs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-06-22 18:03:50.000000 socialgene-0.1.8/socialgene/mmseqs/create_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-06-22 18:03:50.000000 socialgene-0.1.8/socialgene/mmseqs/index_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-06-22 18:03:50.000000 socialgene-0.1.8/socialgene/mmseqs/search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:04:03.613478 socialgene-0.1.8/socialgene/neo4j/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:03:50.000000 socialgene-0.1.8/socialgene/neo4j/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10195 2023-06-22 18:03:50.000000 socialgene-0.1.8/socialgene/neo4j/admin_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-06-22 18:03:50.000000 socialgene-0.1.8/socialgene/neo4j/ingest_from_neo4j.py
--rw-r--r--   0 runner    (1001) docker     (123)     4656 2023-06-22 18:03:50.000000 socialgene-0.1.8/socialgene/neo4j/neo4j.py
--rw-r--r--   0 runner    (1001) docker     (123)    12681 2023-06-22 18:03:50.000000 socialgene-0.1.8/socialgene/neo4j/queries.cypher
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:04:03.613478 socialgene-0.1.8/socialgene/neo4j/schema/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:03:50.000000 socialgene-0.1.8/socialgene/neo4j/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-06-22 18:03:50.000000 socialgene-0.1.8/socialgene/neo4j/schema/define_modules.py
--rw-r--r--   0 runner    (1001) docker     (123)     5564 2023-06-22 18:03:50.000000 socialgene-0.1.8/socialgene/neo4j/schema/define_nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     7445 2023-06-22 18:03:50.000000 socialgene-0.1.8/socialgene/neo4j/schema/define_relationships.py
--rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-06-22 18:03:50.000000 socialgene-0.1.8/socialgene/neo4j/schema/node_relationship_class.py
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-06-22 18:03:50.000000 socialgene-0.1.8/socialgene/neo4j/schema/socialgene_modules.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:04:03.613478 socialgene-0.1.8/socialgene/neo4j/search/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:03:50.000000 socialgene-0.1.8/socialgene/neo4j/search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-06-22 18:03:50.000000 socialgene-0.1.8/socialgene/neo4j/search/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-06-22 18:03:50.000000 socialgene-0.1.8/socialgene/neo4j/single_protein_search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:04:03.613478 socialgene-0.1.8/socialgene/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:03:50.000000 socialgene-0.1.8/socialgene/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4705 2023-06-22 18:03:50.000000 socialgene-0.1.8/socialgene/parsers/datasets_parse.py
--rw-r--r--   0 runner    (1001) docker     (123)     5719 2023-06-22 18:03:50.000000 socialgene-0.1.8/socialgene/parsers/hmmer_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    17259 2023-06-22 18:03:50.000000 socialgene-0.1.8/socialgene/parsers/hmmmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-06-22 18:03:50.000000 socialgene-0.1.8/socialgene/parsers/ncbi_feature_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-06-22 18:03:50.000000 socialgene-0.1.8/socialgene/parsers/ncbi_taxonomy.py
--rw-r--r--   0 runner    (1001) docker     (123)    13954 2023-06-22 18:03:50.000000 socialgene-0.1.8/socialgene/parsers/sequence_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:04:03.617478 socialgene-0.1.8/socialgene/scoring/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:03:50.000000 socialgene-0.1.8/socialgene/scoring/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-06-22 18:03:50.000000 socialgene-0.1.8/socialgene/scoring/scoring.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:04:03.617478 socialgene-0.1.8/socialgene/taxonomy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:03:50.000000 socialgene-0.1.8/socialgene/taxonomy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:04:03.617478 socialgene-0.1.8/socialgene/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:03:50.000000 socialgene-0.1.8/socialgene/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-06-22 18:03:50.000000 socialgene-0.1.8/socialgene/utils/chunker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-06-22 18:03:50.000000 socialgene-0.1.8/socialgene/utils/file_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-06-22 18:03:50.000000 socialgene-0.1.8/socialgene/utils/get_ncbi_biosample_attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)     5092 2023-06-22 18:03:50.000000 socialgene-0.1.8/socialgene/utils/goterms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-06-22 18:03:50.000000 socialgene-0.1.8/socialgene/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-06-22 18:03:50.000000 socialgene-0.1.8/socialgene/utils/ncbi_ftp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-06-22 18:03:50.000000 socialgene-0.1.8/socialgene/utils/nextflow_test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-22 18:03:50.000000 socialgene-0.1.8/socialgene/utils/np_json_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-06-22 18:03:50.000000 socialgene-0.1.8/socialgene/utils/pandas_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-22 18:03:50.000000 socialgene-0.1.8/socialgene/utils/ping.py
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-06-22 18:03:50.000000 socialgene-0.1.8/socialgene/utils/prep_ncbi_biosample_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-06-22 18:03:50.000000 socialgene-0.1.8/socialgene/utils/protein_sqlite.py
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-06-22 18:03:50.000000 socialgene-0.1.8/socialgene/utils/run_subprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-06-22 18:03:50.000000 socialgene-0.1.8/socialgene/utils/simple_math.py
--rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-06-22 18:03:50.000000 socialgene-0.1.8/socialgene/utils/untargz.py
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-22 18:03:50.000000 socialgene-0.1.8/socialgene/utils/version.py
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-22 18:03:50.000000 socialgene-0.1.8/socialgene/utils/writers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:04:03.605477 socialgene-0.1.8/socialgene.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-06-22 18:04:03.000000 socialgene-0.1.8/socialgene.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-06-22 18:04:03.000000 socialgene-0.1.8/socialgene.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 18:04:03.000000 socialgene-0.1.8/socialgene.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-22 18:04:03.000000 socialgene-0.1.8/socialgene.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-22 18:04:03.000000 socialgene-0.1.8/socialgene.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-22 18:04:03.000000 socialgene-0.1.8/socialgene.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 17:07:30.828457 socialgene-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-02 17:07:20.000000 socialgene-0.1.9/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-07-02 17:07:30.828457 socialgene-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-07-02 17:07:20.000000 socialgene-0.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-07-02 17:07:20.000000 socialgene-0.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-07-02 17:07:30.828457 socialgene-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-07-02 17:07:20.000000 socialgene-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 17:07:30.820457 socialgene-0.1.9/socialgene/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 17:07:20.000000 socialgene-0.1.9/socialgene/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 17:07:30.820457 socialgene-0.1.9/socialgene/base/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 17:07:20.000000 socialgene-0.1.9/socialgene/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8612 2023-07-02 17:07:20.000000 socialgene-0.1.9/socialgene/base/compare_protein.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20508 2023-07-02 17:07:20.000000 socialgene-0.1.9/socialgene/base/molbio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26042 2023-07-02 17:07:20.000000 socialgene-0.1.9/socialgene/base/socialgene.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 17:07:30.820457 socialgene-0.1.9/socialgene/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 17:07:20.000000 socialgene-0.1.9/socialgene/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-07-02 17:07:20.000000 socialgene-0.1.9/socialgene/cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-07-02 17:07:20.000000 socialgene-0.1.9/socialgene/cli/clean_hmms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-07-02 17:07:20.000000 socialgene-0.1.9/socialgene/cli/create_neo4j_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-07-02 17:07:20.000000 socialgene-0.1.9/socialgene/cli/export_neo4j_header_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-07-02 17:07:20.000000 socialgene-0.1.9/socialgene/cli/export_protein_loci_assembly_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-07-02 17:07:20.000000 socialgene-0.1.9/socialgene/cli/parameter_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-07-02 17:07:20.000000 socialgene-0.1.9/socialgene/cli/parse_ncbi_feature_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-07-02 17:07:20.000000 socialgene-0.1.9/socialgene/cli/parse_ncbi_taxonomy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-07-02 17:07:20.000000 socialgene-0.1.9/socialgene/cli/process_domtblout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-07-02 17:07:20.000000 socialgene-0.1.9/socialgene/cli/protein_sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-07-02 17:07:20.000000 socialgene-0.1.9/socialgene/cli/socialgene_hmm_tsv_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 17:07:30.824457 socialgene-0.1.9/socialgene/clustermap/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 17:07:20.000000 socialgene-0.1.9/socialgene/clustermap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9860 2023-07-02 17:07:20.000000 socialgene-0.1.9/socialgene/clustermap/clustermap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4131 2023-07-02 17:07:20.000000 socialgene-0.1.9/socialgene/common_parameters.env
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-07-02 17:07:20.000000 socialgene-0.1.9/socialgene/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 17:07:30.824457 socialgene-0.1.9/socialgene/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 17:07:20.000000 socialgene-0.1.9/socialgene/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8067 2023-07-02 17:07:20.000000 socialgene-0.1.9/socialgene/data/biosample_attributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 17:07:30.824457 socialgene-0.1.9/socialgene/findmybgc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 17:07:20.000000 socialgene-0.1.9/socialgene/findmybgc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10106 2023-07-02 17:07:20.000000 socialgene-0.1.9/socialgene/findmybgc/findmybgc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 17:07:30.824457 socialgene-0.1.9/socialgene/hashing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 17:07:20.000000 socialgene-0.1.9/socialgene/hashing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-07-02 17:07:20.000000 socialgene-0.1.9/socialgene/hashing/hashing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 17:07:30.824457 socialgene-0.1.9/socialgene/hmm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 17:07:20.000000 socialgene-0.1.9/socialgene/hmm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6020 2023-07-02 17:07:20.000000 socialgene-0.1.9/socialgene/hmm/hmmer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-07-02 17:07:20.000000 socialgene-0.1.9/socialgene/hmm/hmminfo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 17:07:30.824457 socialgene-0.1.9/socialgene/mmseqs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 17:07:20.000000 socialgene-0.1.9/socialgene/mmseqs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-07-02 17:07:20.000000 socialgene-0.1.9/socialgene/mmseqs/create_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-07-02 17:07:20.000000 socialgene-0.1.9/socialgene/mmseqs/index_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-07-02 17:07:20.000000 socialgene-0.1.9/socialgene/mmseqs/search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 17:07:30.824457 socialgene-0.1.9/socialgene/neo4j/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 17:07:20.000000 socialgene-0.1.9/socialgene/neo4j/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10195 2023-07-02 17:07:20.000000 socialgene-0.1.9/socialgene/neo4j/admin_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-07-02 17:07:20.000000 socialgene-0.1.9/socialgene/neo4j/ingest_from_neo4j.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4656 2023-07-02 17:07:20.000000 socialgene-0.1.9/socialgene/neo4j/neo4j.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12681 2023-07-02 17:07:20.000000 socialgene-0.1.9/socialgene/neo4j/queries.cypher
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 17:07:30.824457 socialgene-0.1.9/socialgene/neo4j/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 17:07:20.000000 socialgene-0.1.9/socialgene/neo4j/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-07-02 17:07:20.000000 socialgene-0.1.9/socialgene/neo4j/schema/define_modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5587 2023-07-02 17:07:20.000000 socialgene-0.1.9/socialgene/neo4j/schema/define_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7454 2023-07-02 17:07:20.000000 socialgene-0.1.9/socialgene/neo4j/schema/define_relationships.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-07-02 17:07:20.000000 socialgene-0.1.9/socialgene/neo4j/schema/node_relationship_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-07-02 17:07:20.000000 socialgene-0.1.9/socialgene/neo4j/schema/socialgene_modules.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 17:07:30.824457 socialgene-0.1.9/socialgene/neo4j/search/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 17:07:20.000000 socialgene-0.1.9/socialgene/neo4j/search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-07-02 17:07:20.000000 socialgene-0.1.9/socialgene/neo4j/search/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-07-02 17:07:20.000000 socialgene-0.1.9/socialgene/neo4j/single_protein_search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 17:07:30.824457 socialgene-0.1.9/socialgene/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 17:07:20.000000 socialgene-0.1.9/socialgene/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4705 2023-07-02 17:07:20.000000 socialgene-0.1.9/socialgene/parsers/datasets_parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5719 2023-07-02 17:07:20.000000 socialgene-0.1.9/socialgene/parsers/hmmer_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17259 2023-07-02 17:07:20.000000 socialgene-0.1.9/socialgene/parsers/hmmmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-07-02 17:07:20.000000 socialgene-0.1.9/socialgene/parsers/ncbi_feature_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-07-02 17:07:20.000000 socialgene-0.1.9/socialgene/parsers/ncbi_taxonomy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13954 2023-07-02 17:07:20.000000 socialgene-0.1.9/socialgene/parsers/sequence_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 17:07:30.824457 socialgene-0.1.9/socialgene/scoring/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 17:07:20.000000 socialgene-0.1.9/socialgene/scoring/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-07-02 17:07:20.000000 socialgene-0.1.9/socialgene/scoring/scoring.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 17:07:30.828457 socialgene-0.1.9/socialgene/taxonomy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 17:07:20.000000 socialgene-0.1.9/socialgene/taxonomy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 17:07:30.828457 socialgene-0.1.9/socialgene/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 17:07:20.000000 socialgene-0.1.9/socialgene/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-07-02 17:07:20.000000 socialgene-0.1.9/socialgene/utils/chunker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3587 2023-07-02 17:07:20.000000 socialgene-0.1.9/socialgene/utils/file_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-07-02 17:07:20.000000 socialgene-0.1.9/socialgene/utils/get_ncbi_biosample_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5092 2023-07-02 17:07:20.000000 socialgene-0.1.9/socialgene/utils/goterms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-07-02 17:07:20.000000 socialgene-0.1.9/socialgene/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-07-02 17:07:20.000000 socialgene-0.1.9/socialgene/utils/ncbi_ftp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-07-02 17:07:20.000000 socialgene-0.1.9/socialgene/utils/nextflow_test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-07-02 17:07:20.000000 socialgene-0.1.9/socialgene/utils/np_json_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-07-02 17:07:20.000000 socialgene-0.1.9/socialgene/utils/pandas_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-07-02 17:07:20.000000 socialgene-0.1.9/socialgene/utils/ping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-07-02 17:07:20.000000 socialgene-0.1.9/socialgene/utils/prep_ncbi_biosample_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-07-02 17:07:20.000000 socialgene-0.1.9/socialgene/utils/protein_sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-07-02 17:07:20.000000 socialgene-0.1.9/socialgene/utils/run_subprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-07-02 17:07:20.000000 socialgene-0.1.9/socialgene/utils/simple_math.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-07-02 17:07:20.000000 socialgene-0.1.9/socialgene/utils/untargz.py
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-02 17:07:20.000000 socialgene-0.1.9/socialgene/utils/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 17:07:30.820457 socialgene-0.1.9/socialgene.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-07-02 17:07:30.000000 socialgene-0.1.9/socialgene.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-07-02 17:07:30.000000 socialgene-0.1.9/socialgene.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 17:07:30.000000 socialgene-0.1.9/socialgene.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-07-02 17:07:30.000000 socialgene-0.1.9/socialgene.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-02 17:07:30.000000 socialgene-0.1.9/socialgene.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-02 17:07:30.000000 socialgene-0.1.9/socialgene.egg-info/top_level.txt
```

### Comparing `socialgene-0.1.8/LICENSE.md` & `socialgene-0.1.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.8/PKG-INFO` & `socialgene-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: socialgene
-Version: 0.1.8
+Version: 0.1.9
 Summary: Creating and interacting with graph databases of protein domains and their genome coordinates
 Author-email: "Chase M. Clark" <chasingmicrobes@gmail.com>
 License: MIT
 Project-URL: repository, https://github.com/socialgene/sgpy
 Project-URL: homepage, https://socialgene.github.io
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `socialgene-0.1.8/README.md` & `socialgene-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.8/pyproject.toml` & `socialgene-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "socialgene"
-version = "0.1.8"
+version = "0.1.9"
 description = "Creating and interacting with graph databases of protein domains and their genome coordinates"
 readme = "README.md"
 authors =  [
     {name = "Chase M. Clark", email = "chasingmicrobes@gmail.com"},
 ]
 keywords = []  #! TODO
 # Pypi classifiers: https://pypi.org/classifiers/
```

### Comparing `socialgene-0.1.8/setup.cfg` & `socialgene-0.1.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.8/setup.py` & `socialgene-0.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.8/socialgene/base/compare_protein.py` & `socialgene-0.1.9/socialgene/base/compare_protein.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.8/socialgene/base/molbio.py` & `socialgene-0.1.9/socialgene/base/molbio.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,15 +93,15 @@
         "Z",
         "J",
         "U",
         "B",
         "O",
         "*",
     ]
-    __slots__ = ["hash_id", "sequence"]
+    __slots__ = ["hash_id", "md5", "sequence"]
 
     def __init__(self, sequence: str = None, hash_id: str = None):
         """Class for holding an amino acid sequence (protein)
 
         Args:
             sequence (str, optional): amino acid sequence
             hash_id (str, optional): a hash_id can be provided if a sequence isn't
@@ -144,14 +144,15 @@
                 [str(self.sequence.count(i)) for i in self._one_letter_amino_acids()]
             )
 
     def _assign_hash(self):
         """Hash the amino acid sequence"""
         self._standardize_sequence()
         self.hash_id = hasher.hash_aminos(self.sequence)
+        self.md5 = hasher.hash_aminos(self.sequence, algo="md5")
 
     def _standardize_sequence(self):
         """Check an input AA sequence for expected characters
 
         Raises:
             ValueError: "Unknown character/letter in protein sequence
         """
```

### Comparing `socialgene-0.1.8/socialgene/base/socialgene.py` & `socialgene-0.1.9/socialgene/base/socialgene.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 from typing import List
 
 import csv
-import gzip
+
 import itertools
 import pickle
 import tempfile
 from collections import defaultdict
 from copy import deepcopy
-from functools import partial
 from multiprocessing import cpu_count
 from operator import attrgetter
 from pathlib import Path
 
 import pandas as pd
 from rich.progress import Progress
 
@@ -21,14 +20,15 @@
 from socialgene.hmm.hmmer import HMMER
 from socialgene.neo4j.neo4j import Neo4jQuery
 from socialgene.neo4j.search.basic import search_protein_hash
 from socialgene.parsers.hmmer_parser import HmmerParser
 from socialgene.parsers.sequence_parser import SequenceParser
 from socialgene.scoring.scoring import mod_score
 from socialgene.utils.chunker import chunk_a_list_with_numpy
+from socialgene.utils.file_handling import open_write
 from socialgene.utils.logging import log
 
 
 class SocialGene(Molbio, CompareProtein, SequenceParser, Neo4jQuery, HmmerParser):
     """Main class for building, sotring, working with protein and genomic info"""
 
     _genomic_info_export_tablenames = [
@@ -240,17 +240,17 @@
             self.proteins[result["protein_id"]].external_protein_id = result["name"]
             self.proteins[result["protein_id"]].description = result["description"]
 
     ########################################
     # File Outputs
     ########################################
 
-    def export_all_domains_as_tsv(self, outpath):
+    def export_all_domains_as_tsv(self, outpath, **kwargs):
         _domain_counter = 0
-        with open(outpath, "a") as f:
+        with open_write(outpath, **kwargs) as f:
             tsv_writer = csv.writer(f, delimiter="\t")
             # sort to standardize the write order
             ordered_prot_ids = list(self.proteins.keys())
             ordered_prot_ids.sort()
             for prot_id in ordered_prot_ids:
                 # sort to standardize the write order
                 for domain in self.proteins[
@@ -283,29 +283,26 @@
         return ((k, v) for k, v in self.proteins.items() if k in hash_list)
 
     def write_fasta(
         self,
         outpath,
         hash_list: List = None,
         external_protein_id: bool = False,
-        gz: bool = False,
+        **kwargs,
     ):
         """Write proteins to a FASTA file
 
         Args:
             outpath (str): path of file that FASTA entries will be appended to
             hash_list (List, optional): hash id of the protein(s) to export. Defaults to None.
             external_protein_id (bool, optional): Write protein identifiers as the hash (True) or the original identifier (False). Defaults to False.
-            gz (bool, optional): Write as gzip?. Defaults to False.
+            **kwargs: see print(open_write.__doc__)
         """
-        if gz:
-            _open = partial(gzip.open, mode="at")
-        else:
-            _open = partial(open, mode="a")
-        with _open(outpath) as handle:
+
+        with open_write(filepath=outpath, **kwargs) as handle:
             counter = 0
             if hash_list:
                 temp_iter = self.filter_proteins(hash_list)
             else:
                 temp_iter = self.proteins.items()
             for k, v in temp_iter:
                 if v.sequence is not None:
@@ -324,33 +321,36 @@
             hash_id (str): hash id of protein to export
 
         Returns:
             str: fasta string
         """
         return f">{self.proteins[hash_id].hash_id}\n{self.proteins[hash_id].sequence}"
 
-    def write_n_fasta(self, outdir, n_splits=1, mode="a"):
+    def write_n_fasta(self, outdir, n_splits=1, **kwargs):
         """Export protein sequences split into n-number of fasta files
 
         Args:
             outdir (str): Directory to save fasta files into
             n_splits (int, optional): Defaults to 1.
+            **kwargs: see print(open_write.__doc__)
         """
 
         def split(a, n):
             # https://stackoverflow.com/a/2135920
             k, m = divmod(len(a), n)
             return (
                 a[i * k + min(i, m) : (i + 1) * k + min(i + 1, m)] for i in range(n)
             )
 
         protein_list = split(list(self.proteins.keys()), n_splits)
         counter = 1
         for protein_group in protein_list:
-            with open(Path(outdir, f"fasta_split_{counter}.faa"), mode) as handle:
+            with open_write(
+                Path(outdir, f"fasta_split_{counter}.faa"), **kwargs
+            ) as handle:
                 for k, v in {
                     key: self.proteins.get(key) for key in sorted(protein_group)
                 }.items():
                     handle.writelines(f">{k}\n{v.sequence}\n")
             counter += 1
 
     def _merge_proteins(self, sg_object):
@@ -459,24 +459,24 @@
     # OUTPUTS FOR NEXTFLOW
     ########################################
     @staticmethod
     def _create_internal_locus_id(assembly_id, locus_id):
         # because locus id can't be assured to be unique across assemblies
         return hasher(f"{assembly_id}___{locus_id}")
 
-    def write_table(self, outdir: str, tablename: str, filename: str = None, mode="a"):
+    def write_table(self, outdir: str, tablename: str, filename: str = None, **kwargs):
         if not filename:
             filename = tablename
         if not hasattr(self, tablename):
             raise ValueError(
                 f"tablename must be one of: {self._genomic_info_export_tablenames}"
             )
         else:
             outpath = Path(outdir, filename)
-            with open(outpath, mode) as handle:
+            with open_write(outpath, **kwargs) as handle:
                 tsv_writer = csv.writer(
                     handle, delimiter="\t", quotechar='"', quoting=csv.QUOTE_MINIMAL
                 )
                 for i in getattr(self, tablename)():
                     tsv_writer.writerow(i)
 
     def protein_to_go_table(self):
@@ -530,18 +530,18 @@
         for protein in self.proteins.values():
             if protein.sequence is None:
                 prot_len = None
             else:
                 prot_len = len(protein.sequence)
             yield (
                 protein.hash_id,
-                # TODO: add database "source" of protein?
+                protein.md5,
                 protein.external_protein_id,
                 protein.description,
-                prot_len,  # protein length
+                prot_len,
             )
 
     def protein_ids_table(self):
         """Protein id table for import into Neo4j
 
         Args:
             outdir (str, optional): Defaults to ".".
```

### Comparing `socialgene-0.1.8/socialgene/cli/__main__.py` & `socialgene-0.1.9/socialgene/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.8/socialgene/cli/clean_hmms.py` & `socialgene-0.1.9/socialgene/cli/clean_hmms.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.8/socialgene/cli/create_neo4j_db.py` & `socialgene-0.1.9/socialgene/cli/create_neo4j_db.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.8/socialgene/cli/export_neo4j_header_files.py` & `socialgene-0.1.9/socialgene/cli/export_neo4j_header_files.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.8/socialgene/cli/export_protein_loci_assembly_tables.py` & `socialgene-0.1.9/socialgene/cli/export_protein_loci_assembly_tables.py`

 * *Files 26% similar despite different names*

```diff
@@ -42,28 +42,43 @@
     "--collect_tables_in_memory",
     metavar="bool",
     help="Should all tables be collected in RAM before writing to disk?",
     required=False,
     default=False,
     action=argparse.BooleanOptionalAction,
 )
+parser.add_argument(
+    "--compression",
+    metavar="bool",
+    help="Gzip compress output?",
+    required=False,
+    default=False,
+    action=argparse.BooleanOptionalAction,
+)
 
 
-def _writer(socialgene_object, outdir, n_fasta_splits):
-    socialgene_object.write_n_fasta(outdir=outdir, n_splits=n_fasta_splits, mode="a")
+def _writer(socialgene_object, outdir, n_fasta_splits, compression):
+    socialgene_object.write_n_fasta(
+        outdir=outdir, n_splits=n_fasta_splits, mode="a", compression=compression
+    )
     for i in SocialGene._genomic_info_export_tablenames:
         socialgene_object.write_table(
-            outdir=outdir, tablename=i, filename=i.removesuffix("_table"), mode="a"
+            outdir=outdir,
+            tablename=i,
+            filename=i.removesuffix("_table"),
+            mode="a",
+            compression=compression,
         )
 
 
 def export_tables(
     outdir: str,
     n_fasta_splits: int,
     collect_tables_in_memory: bool,
+    compression: str,
     file_list: List = None,
     sequence_files_glob: str = "",
 ):
     outdir = Path(outdir)
     sequence_files = list()
     # find files using the input glob
     if sequence_files_glob:
@@ -79,30 +94,37 @@
     for i in sequence_files:
         socialgene_object.parse(Path(i))
         if not collect_tables_in_memory:
             _writer(
                 socialgene_object=socialgene_object,
                 outdir=outdir,
                 n_fasta_splits=n_fasta_splits,
+                compression=compression,
             )
             socialgene_object = SocialGene()
     if collect_tables_in_memory:
         _writer(
             socialgene_object=socialgene_object,
             outdir=outdir,
             n_fasta_splits=n_fasta_splits,
+            compression=compression,
         )
 
 
 def main():
     args = parser.parse_args()
     log.info(f"Socialgene variables: \n{env_vars}")
+    if args.compression:
+        compression = "gzip"
+    else:
+        compression = None
     export_tables(
         sequence_files_glob=args.sequence_files_glob,
         outdir=args.outdir,
         n_fasta_splits=int(args.n_fasta_splits),
         collect_tables_in_memory=args.collect_tables_in_memory,
+        compression=compression,
     )
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `socialgene-0.1.8/socialgene/cli/parameter_export.py` & `socialgene-0.1.9/socialgene/cli/parameter_export.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.8/socialgene/cli/parse_ncbi_feature_tables.py` & `socialgene-0.1.9/socialgene/cli/parse_ncbi_feature_tables.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.8/socialgene/cli/parse_ncbi_taxonomy.py` & `socialgene-0.1.9/socialgene/cli/parse_ncbi_taxonomy.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.8/socialgene/cli/process_domtblout.py` & `socialgene-0.1.9/socialgene/cli/process_domtblout.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.8/socialgene/cli/protein_sqlite.py` & `socialgene-0.1.9/socialgene/cli/protein_sqlite.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.8/socialgene/cli/socialgene_hmm_tsv_parser.py` & `socialgene-0.1.9/socialgene/cli/socialgene_hmm_tsv_parser.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.8/socialgene/clustermap/clustermap.py` & `socialgene-0.1.9/socialgene/clustermap/clustermap.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.8/socialgene/common_parameters.env` & `socialgene-0.1.9/socialgene/common_parameters.env`

 * *Files 2% similar despite different names*

```diff
@@ -96,19 +96,17 @@
 # NCBI ENTREZ INFO
 # https://ncbiinsights.ncbi.nlm.nih.gov/2017/11/02/new-api-keys-for-the-e-utilities/
 ######################################################################
 
 ENTREZ_EMAIL=emailhere
 ENTREZ_API_KEY=apikeyhere
 
-
-
 ######################################################################
 # PYTHON LIBRARY
 ######################################################################
 
 # controls which hashing algorithm is used (https://github.com/socialgene/sgpy/blob/main/socialgene/hashing/hashing.py)
-HASHING_ALGORITHM=crc64
+HASHING_ALGORITHM=sha512t24u
 
 # controls what log messages are printed (https://github.com/socialgene/sgpy/blob/main/socialgene/utils/logging.py)
 SOCIALGENE_LOGLEVEL=DEBUG
```

### Comparing `socialgene-0.1.8/socialgene/config.py` & `socialgene-0.1.9/socialgene/config.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.8/socialgene/data/biosample_attributes` & `socialgene-0.1.9/socialgene/data/biosample_attributes`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.8/socialgene/findmybgc/findmybgc.py` & `socialgene-0.1.9/socialgene/findmybgc/findmybgc.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.8/socialgene/hashing/hashing.py` & `socialgene-0.1.9/socialgene/hashing/hashing.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     required=True,
 )
 
 
 def sha512t24u(input):
     # https://www.ncbi.nlm.nih.gov/pmc/articles/PMC7714221/
     # To standardize to caps-only input, use hash_aminos()
-    sha512_digest = use_hashlib(input=input, algo="sha512").digest()[:24]
+    sha512_digest = hashlib.sha512(bytes(input, "utf8")).digest()[:24]
     sha512t24u = base64.urlsafe_b64encode(sha512_digest).decode("ascii")
     return sha512t24u
 
 
 def hash_aminos(input, **kwargs):
     # make sure everything is uppercase before hashing
     return hasher(input=input.upper(), **kwargs)
@@ -30,19 +30,20 @@
 
 def use_hashlib(input, algo):
     allow_algos = ("sha512", "sha256", "sha384", "md5", "sha224")
     if algo not in allow_algos:
         # TODO: this should also output the sha512t24u ans crc algos
         raise ValueError(f"algo must be one of: {allow_algos}")
     hasher = getattr(hashlib, algo)
-    return hasher(bytes(input, "utf8"))
+    return hasher(bytes(input, "utf8")).hexdigest()
 
 
-def hasher(input):
-    algo = env_vars["HASHING_ALGORITHM"]
+def hasher(input, algo=None):
+    if not algo:
+        algo = env_vars["HASHING_ALGORITHM"]
     match algo:
         case "sha512t24u":
             return sha512t24u(input)
         case "crc64":
             return CheckSum.crc64(input).removeprefix("CRC-")
         case "crc32":
             return CheckSum.crc32(input)
```

### Comparing `socialgene-0.1.8/socialgene/hmm/hmmer.py` & `socialgene-0.1.9/socialgene/hmm/hmmer.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.8/socialgene/hmm/hmminfo.py` & `socialgene-0.1.9/socialgene/hmm/hmminfo.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 class HmmInfo:
     def __init__(self, all_hmms_path):
         self.columns = list(HmmModel()._tsv_dict().keys())
         self.all_hmms_path = all_hmms_path
         self.all_hmms_data = list()
 
     def read_tsv(self):
-        with fh.open_file(self.all_hmms_path) as h:
+        with fh.open_read(self.all_hmms_path) as h:
             for line in h:
                 line_vals = [
                     None if v.strip() == '""' else v.strip() for v in line.split("\t")
                 ]
                 if not len(line_vals) == 16:
                     raise ValueError(f"Expected 16 columns, not {len(line_vals)}")
                 if not line_vals == self.columns:
```

### Comparing `socialgene-0.1.8/socialgene/mmseqs/create_database.py` & `socialgene-0.1.9/socialgene/mmseqs/create_database.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.8/socialgene/mmseqs/index_database.py` & `socialgene-0.1.9/socialgene/mmseqs/index_database.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.8/socialgene/mmseqs/search.py` & `socialgene-0.1.9/socialgene/mmseqs/search.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.8/socialgene/neo4j/admin_import.py` & `socialgene-0.1.9/socialgene/neo4j/admin_import.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.8/socialgene/neo4j/ingest_from_neo4j.py` & `socialgene-0.1.9/socialgene/neo4j/ingest_from_neo4j.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.8/socialgene/neo4j/neo4j.py` & `socialgene-0.1.9/socialgene/neo4j/neo4j.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.8/socialgene/neo4j/queries.cypher` & `socialgene-0.1.9/socialgene/neo4j/queries.cypher`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.8/socialgene/neo4j/schema/define_modules.py` & `socialgene-0.1.9/socialgene/neo4j/schema/define_modules.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.8/socialgene/neo4j/schema/define_nodes.py` & `socialgene-0.1.9/socialgene/neo4j/schema/define_nodes.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,14 +58,15 @@
         self.add_node(
             neo4j_label="protein",
             header_filename="protein_ids.header",
             target_subdirectory="protein_info",
             target_extension="protein_ids",
             header=[
                 "uid:ID(protein)",
+                "md5",
             ],
         )
         self.add_node(
             neo4j_label="goterm",
             header_filename="goterms.header",
             target_subdirectory="goterms",
             target_extension="goterms",
```

### Comparing `socialgene-0.1.8/socialgene/neo4j/schema/define_relationships.py` & `socialgene-0.1.9/socialgene/neo4j/schema/define_relationships.py`

 * *Files 0% similar despite different names*

```diff
@@ -150,15 +150,15 @@
         )
 
         self.add_relationship(
             neo4j_label="MMSEQS2",
             header_filename="mmseqs2.header",
             target_subdirectory="mmseqs2_cluster",
             target_extension="mmseqs2_results_cluster.tsv",
-            header=[":START_ID(protein)", ":END_ID(protein)"],
+            header=[":START_ID(protein)", ":END_ID(protein)", ":TYPE"],
         )
 
         self.add_relationship(
             neo4j_label="CLUSTER_TO_FILE",
             header_filename="cluster_to_source_file.header",
             target_subdirectory="paired_omics",
             target_extension="cluster_to_source_file",
```

### Comparing `socialgene-0.1.8/socialgene/neo4j/schema/node_relationship_class.py` & `socialgene-0.1.9/socialgene/neo4j/schema/node_relationship_class.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.8/socialgene/neo4j/schema/socialgene_modules.py` & `socialgene-0.1.9/socialgene/neo4j/schema/socialgene_modules.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.8/socialgene/neo4j/search/basic.py` & `socialgene-0.1.9/socialgene/neo4j/search/basic.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.8/socialgene/neo4j/single_protein_search.py` & `socialgene-0.1.9/socialgene/neo4j/single_protein_search.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.8/socialgene/parsers/datasets_parse.py` & `socialgene-0.1.9/socialgene/parsers/datasets_parse.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.8/socialgene/parsers/hmmer_parser.py` & `socialgene-0.1.9/socialgene/parsers/hmmer_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,15 +69,15 @@
             "acc",
             "desc",
         )
 
         input_path = Path(input_path)
         if not input_path.exists():
             raise FileNotFoundError(input_path)
-        with fh.open_file(input_path) as f:
+        with fh.open_read(input_path) as f:
             for line in f:
                 if line.startswith("#"):
                     pass
                 else:
                     yield dict(zip(all_columns, line.split()))
 
 
@@ -85,15 +85,15 @@
     """For HMMER domtblout files already processed and rewritten with class Domtblout()"""
 
     def __init__(self):
         pass
 
     def parse_parseddomtblout(self, input_path):
         input_path = Path(input_path)
-        with fh.open_file(input_path) as f:
+        with fh.open_read(input_path) as f:
             for line in f:
                 line = line.strip().split("\t")
                 self.add_protein(
                     hash_id=line[0],
                 )
                 self.proteins[line[0]].add_domain(
                     hash_id=line[1],
@@ -142,30 +142,30 @@
     Args:
         filepath (str): path to sequence file
 
     Returns:
         bool: true/false
     """
     log.info(filepath)
-    with fh.open_file(filepath) as f:
+    with fh.open_read(filepath) as f:
         l1 = f.readline()
         l2 = f.readline()
         a = l1.count("\t")
         b = l2.count("\t")
     return all(i == 13 for i in [a, b])
 
 
 def check_if_domtblout(filepath):
     """Check if headers are from a HMMER domtblout file
     Args:
         filepath: file path of file to guess
     Returns:
         bool: true/false
     """
-    with fh.open_file(filepath) as f:
+    with fh.open_read(filepath) as f:
         l1 = f.readline()
         l2 = f.readline()
     expected_header = "#---fullsequence-----------------thisdomain-------------hmmcoordalicoordenvcoord\n"
     if l1.replace(" ", "") == expected_header:
         if (
             l2.replace(" ", "")
             == "#targetnameaccessiontlenquerynameaccessionqlenE-valuescorebias#ofc-Evaluei-Evaluescorebiasfromtofromtofromtoaccdescriptionoftarget\n"
```

### Comparing `socialgene-0.1.8/socialgene/parsers/hmmmodel.py` & `socialgene-0.1.9/socialgene/parsers/hmmmodel.py`

 * *Files 0% similar despite different names*

```diff
@@ -285,15 +285,15 @@
         self.temp_model = HmmModel()
 
     def read(self, filepath, base_dir=None):
         # _temp is used to switch from attribute addition to HMM model additon by switching the function
         # to HMM model's functon after seeing "HMM ", to the end of the model
         # then switch back before the next model starts
         _temp = self.temp_model.add_attr
-        with fh.open_file(filepath) as h:
+        with fh.open_read(filepath) as h:
             self.temp_model._base_dir = base_dir
             self.temp_model._abs_path = filepath
             self.temp_model._assign_relative_path()
             self.temp_model.assign_category()
             for line in h:
                 if line.startswith("HMM "):
                     _temp = self.temp_model.add_model
```

### Comparing `socialgene-0.1.8/socialgene/parsers/ncbi_feature_table.py` & `socialgene-0.1.9/socialgene/parsers/ncbi_feature_table.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.8/socialgene/parsers/ncbi_taxonomy.py` & `socialgene-0.1.9/socialgene/parsers/ncbi_taxonomy.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.8/socialgene/parsers/sequence_parser.py` & `socialgene-0.1.9/socialgene/parsers/sequence_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -231,15 +231,15 @@
                             self._parse_genbank(
                                 handle=handle,
                                 input_path=input_path,
                             )
                     except Exception as e:
                         log.debug(e)
         else:
-            with fh.open_file(input_path) as handle:
+            with fh.open_read(input_path) as handle:
                 self._parse_genbank(
                     handle=handle,
                     input_path=input_path,
                     **kwargs,
                 )
         log.info(
             f"'{input_path}' features {dict(sorted(dict(self._count_loci_in_file).items(), key=lambda item: item[1], reverse=True))}"
```

### Comparing `socialgene-0.1.8/socialgene/scoring/scoring.py` & `socialgene-0.1.9/socialgene/scoring/scoring.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.8/socialgene/utils/chunker.py` & `socialgene-0.1.9/socialgene/utils/chunker.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.8/socialgene/utils/get_ncbi_biosample_attributes.py` & `socialgene-0.1.9/socialgene/utils/get_ncbi_biosample_attributes.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.8/socialgene/utils/goterms.py` & `socialgene-0.1.9/socialgene/utils/goterms.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.8/socialgene/utils/logging.py` & `socialgene-0.1.9/socialgene/utils/logging.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.8/socialgene/utils/ncbi_ftp.py` & `socialgene-0.1.9/socialgene/utils/ncbi_ftp.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.8/socialgene/utils/nextflow_test_utils.py` & `socialgene-0.1.9/socialgene/utils/nextflow_test_utils.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.8/socialgene/utils/pandas_utils.py` & `socialgene-0.1.9/socialgene/utils/pandas_utils.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.8/socialgene/utils/prep_ncbi_biosample_data.py` & `socialgene-0.1.9/socialgene/utils/prep_ncbi_biosample_data.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.8/socialgene/utils/protein_sqlite.py` & `socialgene-0.1.9/socialgene/utils/protein_sqlite.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.8/socialgene/utils/run_subprocess.py` & `socialgene-0.1.9/socialgene/utils/run_subprocess.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.8/socialgene/utils/untargz.py` & `socialgene-0.1.9/socialgene/utils/untargz.py`

 * *Files identical despite different names*

### Comparing `socialgene-0.1.8/socialgene.egg-info/PKG-INFO` & `socialgene-0.1.9/socialgene.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: socialgene
-Version: 0.1.8
+Version: 0.1.9
 Summary: Creating and interacting with graph databases of protein domains and their genome coordinates
 Author-email: "Chase M. Clark" <chasingmicrobes@gmail.com>
 License: MIT
 Project-URL: repository, https://github.com/socialgene/sgpy
 Project-URL: homepage, https://socialgene.github.io
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `socialgene-0.1.8/socialgene.egg-info/SOURCES.txt` & `socialgene-0.1.9/socialgene.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -79,9 +79,8 @@
 socialgene/utils/pandas_utils.py
 socialgene/utils/ping.py
 socialgene/utils/prep_ncbi_biosample_data.py
 socialgene/utils/protein_sqlite.py
 socialgene/utils/run_subprocess.py
 socialgene/utils/simple_math.py
 socialgene/utils/untargz.py
-socialgene/utils/version.py
-socialgene/utils/writers.py
+socialgene/utils/version.py
```

### Comparing `socialgene-0.1.8/socialgene.egg-info/entry_points.txt` & `socialgene-0.1.9/socialgene.egg-info/entry_points.txt`

 * *Files identical despite different names*

