# Comparing `tmp/taxpasta-0.3.0.tar.gz` & `tmp/taxpasta-0.4.0.tar.gz`

## Comparing `taxpasta-0.3.0.tar` & `taxpasta-0.4.0.tar`

### file list

```diff
@@ -1,116 +1,123 @@
--rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 taxpasta-0.3.0/src/taxpasta/__init__.py
--rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 taxpasta-0.3.0/src/taxpasta/__main__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 taxpasta-0.3.0/src/taxpasta/_version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 taxpasta-0.3.0/src/taxpasta/py.typed
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 taxpasta-0.3.0/src/taxpasta/application/__init__.py
--rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 taxpasta-0.3.0/src/taxpasta/application/consensus_application.py
--rw-r--r--   0        0        0     6353 2020-02-02 00:00:00.000000 taxpasta-0.3.0/src/taxpasta/application/sample_merging_application.py
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 taxpasta-0.3.0/src/taxpasta/application/error/__init__.py
--rw-r--r--   0        0        0     1260 2020-02-02 00:00:00.000000 taxpasta-0.3.0/src/taxpasta/application/error/standardisation_error.py
--rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 taxpasta-0.3.0/src/taxpasta/application/error/taxpasta_error.py
--rw-r--r--   0        0        0     1126 2020-02-02 00:00:00.000000 taxpasta-0.3.0/src/taxpasta/application/service/__init__.py
--rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 taxpasta-0.3.0/src/taxpasta/application/service/_types.py
--rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 taxpasta-0.3.0/src/taxpasta/application/service/profile_reader.py
--rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 taxpasta-0.3.0/src/taxpasta/application/service/profile_standardisation_service.py
--rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 taxpasta-0.3.0/src/taxpasta/application/service/standard_profile_writer.py
--rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 taxpasta-0.3.0/src/taxpasta/application/service/table_reader.py
--rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 taxpasta-0.3.0/src/taxpasta/application/service/tidy_observation_table_writer.py
--rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 taxpasta-0.3.0/src/taxpasta/application/service/wide_observation_table_writer.py
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 taxpasta-0.3.0/src/taxpasta/domain/__init__.py
--rw-r--r--   0        0        0      888 2020-02-02 00:00:00.000000 taxpasta-0.3.0/src/taxpasta/domain/model/__init__.py
--rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 taxpasta-0.3.0/src/taxpasta/domain/model/sample.py
--rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 taxpasta-0.3.0/src/taxpasta/domain/model/standard_profile.py
--rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 taxpasta-0.3.0/src/taxpasta/domain/model/tidy_observation_table.py
--rw-r--r--   0        0        0     1292 2020-02-02 00:00:00.000000 taxpasta-0.3.0/src/taxpasta/domain/model/wide_observation_table.py
--rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 taxpasta-0.3.0/src/taxpasta/domain/service/__init__.py
--rw-r--r--   0        0        0     1247 2020-02-02 00:00:00.000000 taxpasta-0.3.0/src/taxpasta/domain/service/consensus_builder.py
--rw-r--r--   0        0        0     4067 2020-02-02 00:00:00.000000 taxpasta-0.3.0/src/taxpasta/domain/service/sample_merging_service.py
--rw-r--r--   0        0        0     2892 2020-02-02 00:00:00.000000 taxpasta-0.3.0/src/taxpasta/domain/service/taxonomy_service.py
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 taxpasta-0.3.0/src/taxpasta/infrastructure/__init__.py
--rw-r--r--   0        0        0     2230 2020-02-02 00:00:00.000000 taxpasta-0.3.0/src/taxpasta/infrastructure/application/__init__.py
--rw-r--r--   0        0        0     4592 2020-02-02 00:00:00.000000 taxpasta-0.3.0/src/taxpasta/infrastructure/application/_dependency_check_mixin.py
--rw-r--r--   0        0        0    12231 2020-02-02 00:00:00.000000 taxpasta-0.3.0/src/taxpasta/infrastructure/application/application_service_registry.py
--rw-r--r--   0        0        0     3787 2020-02-02 00:00:00.000000 taxpasta-0.3.0/src/taxpasta/infrastructure/application/sample_etl_application.py
--rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 taxpasta-0.3.0/src/taxpasta/infrastructure/application/sample_sheet.py
--rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 taxpasta-0.3.0/src/taxpasta/infrastructure/application/standard_profile_file_format.py
--rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 taxpasta-0.3.0/src/taxpasta/infrastructure/application/supported_profiler.py
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 taxpasta-0.3.0/src/taxpasta/infrastructure/application/table_reader_file_format.py
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 taxpasta-0.3.0/src/taxpasta/infrastructure/application/tidy_observation_table_file_format.py
--rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 taxpasta-0.3.0/src/taxpasta/infrastructure/application/wide_observation_table_file_format.py
--rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 taxpasta-0.3.0/src/taxpasta/infrastructure/application/bracken/__init__.py
--rw-r--r--   0        0        0     2218 2020-02-02 00:00:00.000000 taxpasta-0.3.0/src/taxpasta/infrastructure/application/bracken/bracken_profile.py
--rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 taxpasta-0.3.0/src/taxpasta/infrastructure/application/bracken/bracken_profile_reader.py
--rw-r--r--   0        0        0     2096 2020-02-02 00:00:00.000000 taxpasta-0.3.0/src/taxpasta/infrastructure/application/bracken/bracken_profile_standardisation_service.py
--rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 taxpasta-0.3.0/src/taxpasta/infrastructure/application/centrifuge/__init__.py
--rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 taxpasta-0.3.0/src/taxpasta/infrastructure/application/centrifuge/centrifuge_profile.py
--rw-r--r--   0        0        0     2040 2020-02-02 00:00:00.000000 taxpasta-0.3.0/src/taxpasta/infrastructure/application/centrifuge/centrifuge_profile_reader.py
--rw-r--r--   0        0        0     1992 2020-02-02 00:00:00.000000 taxpasta-0.3.0/src/taxpasta/infrastructure/application/centrifuge/centrifuge_profile_standardisation_service.py
--rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 taxpasta-0.3.0/src/taxpasta/infrastructure/application/diamond/__init__.py
--rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 taxpasta-0.3.0/src/taxpasta/infrastructure/application/diamond/diamond_profile.py
--rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 taxpasta-0.3.0/src/taxpasta/infrastructure/application/diamond/diamond_profile_reader.py
--rw-r--r--   0        0        0     1960 2020-02-02 00:00:00.000000 taxpasta-0.3.0/src/taxpasta/infrastructure/application/diamond/diamond_profile_standardisation_service.py
--rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 taxpasta-0.3.0/src/taxpasta/infrastructure/application/kaiju/__init__.py
--rw-r--r--   0        0        0     1886 2020-02-02 00:00:00.000000 taxpasta-0.3.0/src/taxpasta/infrastructure/application/kaiju/kaiju_profile.py
--rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 taxpasta-0.3.0/src/taxpasta/infrastructure/application/kaiju/kaiju_profile_reader.py
--rw-r--r--   0        0        0     2672 2020-02-02 00:00:00.000000 taxpasta-0.3.0/src/taxpasta/infrastructure/application/kaiju/kaiju_profile_standardisation_service.py
--rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 taxpasta-0.3.0/src/taxpasta/infrastructure/application/kraken2/__init__.py
--rw-r--r--   0        0        0     2194 2020-02-02 00:00:00.000000 taxpasta-0.3.0/src/taxpasta/infrastructure/application/kraken2/kraken2_profile.py
--rw-r--r--   0        0        0     2748 2020-02-02 00:00:00.000000 taxpasta-0.3.0/src/taxpasta/infrastructure/application/kraken2/kraken2_profile_reader.py
--rw-r--r--   0        0        0     1871 2020-02-02 00:00:00.000000 taxpasta-0.3.0/src/taxpasta/infrastructure/application/kraken2/kraken2_profile_standardisation_service.py
--rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 taxpasta-0.3.0/src/taxpasta/infrastructure/application/krakenuniq/__init__.py
--rw-r--r--   0        0        0     1580 2020-02-02 00:00:00.000000 taxpasta-0.3.0/src/taxpasta/infrastructure/application/krakenuniq/krakenuniq_profile.py
--rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 taxpasta-0.3.0/src/taxpasta/infrastructure/application/krakenuniq/krakenuniq_profile_reader.py
--rw-r--r--   0        0        0     1873 2020-02-02 00:00:00.000000 taxpasta-0.3.0/src/taxpasta/infrastructure/application/krakenuniq/krakenuniq_profile_standardisation_service.py
--rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 taxpasta-0.3.0/src/taxpasta/infrastructure/application/megan6/__init__.py
--rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 taxpasta-0.3.0/src/taxpasta/infrastructure/application/megan6/megan6_profile.py
--rw-r--r--   0        0        0     1489 2020-02-02 00:00:00.000000 taxpasta-0.3.0/src/taxpasta/infrastructure/application/megan6/megan6_profile_reader.py
--rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 taxpasta-0.3.0/src/taxpasta/infrastructure/application/megan6/megan6_profile_standardisation_service.py
--rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 taxpasta-0.3.0/src/taxpasta/infrastructure/application/metaphlan/__init__.py
--rw-r--r--   0        0        0     1949 2020-02-02 00:00:00.000000 taxpasta-0.3.0/src/taxpasta/infrastructure/application/metaphlan/metaphlan_profile.py
--rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 taxpasta-0.3.0/src/taxpasta/infrastructure/application/metaphlan/metaphlan_profile_reader.py
--rw-r--r--   0        0        0     3670 2020-02-02 00:00:00.000000 taxpasta-0.3.0/src/taxpasta/infrastructure/application/metaphlan/metaphlan_profile_standardisation_service.py
--rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 taxpasta-0.3.0/src/taxpasta/infrastructure/application/motus/__init__.py
--rw-r--r--   0        0        0     1217 2020-02-02 00:00:00.000000 taxpasta-0.3.0/src/taxpasta/infrastructure/application/motus/motus_profile.py
--rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 taxpasta-0.3.0/src/taxpasta/infrastructure/application/motus/motus_profile_reader.py
--rw-r--r--   0        0        0     3367 2020-02-02 00:00:00.000000 taxpasta-0.3.0/src/taxpasta/infrastructure/application/motus/motus_profile_standardisation_service.py
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 taxpasta-0.3.0/src/taxpasta/infrastructure/application/standard_profile_writer/__init__.py
--rw-r--r--   0        0        0     1292 2020-02-02 00:00:00.000000 taxpasta-0.3.0/src/taxpasta/infrastructure/application/standard_profile_writer/arrow_standard_profile_writer.py
--rw-r--r--   0        0        0     1257 2020-02-02 00:00:00.000000 taxpasta-0.3.0/src/taxpasta/infrastructure/application/standard_profile_writer/csv_standard_profile_writer.py
--rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 taxpasta-0.3.0/src/taxpasta/infrastructure/application/standard_profile_writer/ods_standard_profile_writer.py
--rw-r--r--   0        0        0     1298 2020-02-02 00:00:00.000000 taxpasta-0.3.0/src/taxpasta/infrastructure/application/standard_profile_writer/parquet_standard_profile_writer.py
--rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 taxpasta-0.3.0/src/taxpasta/infrastructure/application/standard_profile_writer/tsv_standard_profile_writer.py
--rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 taxpasta-0.3.0/src/taxpasta/infrastructure/application/standard_profile_writer/xlsx_standard_profile_writer.py
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 taxpasta-0.3.0/src/taxpasta/infrastructure/application/table_reader/__init__.py
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 taxpasta-0.3.0/src/taxpasta/infrastructure/application/table_reader/arrow_table_reader.py
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 taxpasta-0.3.0/src/taxpasta/infrastructure/application/table_reader/csv_table_reader.py
--rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 taxpasta-0.3.0/src/taxpasta/infrastructure/application/table_reader/ods_table_reader.py
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 taxpasta-0.3.0/src/taxpasta/infrastructure/application/table_reader/parquet_table_reader.py
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 taxpasta-0.3.0/src/taxpasta/infrastructure/application/table_reader/tsv_table_reader.py
--rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 taxpasta-0.3.0/src/taxpasta/infrastructure/application/table_reader/xlsx_table_reader.py
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 taxpasta-0.3.0/src/taxpasta/infrastructure/application/tidy_observation_table_writer/__init__.py
--rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 taxpasta-0.3.0/src/taxpasta/infrastructure/application/tidy_observation_table_writer/arrow_table_writer.py
--rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 taxpasta-0.3.0/src/taxpasta/infrastructure/application/tidy_observation_table_writer/csv_table_writer.py
--rw-r--r--   0        0        0     1330 2020-02-02 00:00:00.000000 taxpasta-0.3.0/src/taxpasta/infrastructure/application/tidy_observation_table_writer/ods_table_writer.py
--rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 taxpasta-0.3.0/src/taxpasta/infrastructure/application/tidy_observation_table_writer/parquet_table_writer.py
--rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 taxpasta-0.3.0/src/taxpasta/infrastructure/application/tidy_observation_table_writer/tsv_table_writer.py
--rw-r--r--   0        0        0     1338 2020-02-02 00:00:00.000000 taxpasta-0.3.0/src/taxpasta/infrastructure/application/tidy_observation_table_writer/xlsx_table_writer.py
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 taxpasta-0.3.0/src/taxpasta/infrastructure/application/wide_observation_table_writer/__init__.py
--rw-r--r--   0        0        0     1313 2020-02-02 00:00:00.000000 taxpasta-0.3.0/src/taxpasta/infrastructure/application/wide_observation_table_writer/arrow_wide_observation_table_writer.py
--rw-r--r--   0        0        0     2346 2020-02-02 00:00:00.000000 taxpasta-0.3.0/src/taxpasta/infrastructure/application/wide_observation_table_writer/biom_wide_observation_table_writer.py
--rw-r--r--   0        0        0     1265 2020-02-02 00:00:00.000000 taxpasta-0.3.0/src/taxpasta/infrastructure/application/wide_observation_table_writer/csv_wide_observation_table_writer.py
--rw-r--r--   0        0        0     1332 2020-02-02 00:00:00.000000 taxpasta-0.3.0/src/taxpasta/infrastructure/application/wide_observation_table_writer/ods_wide_observation_table_writer.py
--rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 taxpasta-0.3.0/src/taxpasta/infrastructure/application/wide_observation_table_writer/parquet_wide_observation_table_writer.py
--rw-r--r--   0        0        0     1276 2020-02-02 00:00:00.000000 taxpasta-0.3.0/src/taxpasta/infrastructure/application/wide_observation_table_writer/tsv_wide_observation_table_writer.py
--rw-r--r--   0        0        0     1340 2020-02-02 00:00:00.000000 taxpasta-0.3.0/src/taxpasta/infrastructure/application/wide_observation_table_writer/xlsx_wide_observation_table_writer.py
--rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 taxpasta-0.3.0/src/taxpasta/infrastructure/cli/__init__.py
--rw-r--r--   0        0        0    16826 2020-02-02 00:00:00.000000 taxpasta-0.3.0/src/taxpasta/infrastructure/cli/merge.py
--rw-r--r--   0        0        0     9408 2020-02-02 00:00:00.000000 taxpasta-0.3.0/src/taxpasta/infrastructure/cli/standardise.py
--rw-r--r--   0        0        0     2582 2020-02-02 00:00:00.000000 taxpasta-0.3.0/src/taxpasta/infrastructure/cli/taxpasta.py
--rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 taxpasta-0.3.0/src/taxpasta/infrastructure/domain/__init__.py
--rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 taxpasta-0.3.0/src/taxpasta/infrastructure/domain/service/__init__.py
--rw-r--r--   0        0        0     6972 2020-02-02 00:00:00.000000 taxpasta-0.3.0/src/taxpasta/infrastructure/domain/service/taxopy_taxonomy_service.py
--rw-r--r--   0        0        0    13853 2020-02-02 00:00:00.000000 taxpasta-0.3.0/.gitignore
--rw-r--r--   0        0        0    10174 2020-02-02 00:00:00.000000 taxpasta-0.3.0/LICENSE
--rw-r--r--   0        0        0     8118 2020-02-02 00:00:00.000000 taxpasta-0.3.0/README.md
--rw-r--r--   0        0        0     3874 2020-02-02 00:00:00.000000 taxpasta-0.3.0/pyproject.toml
--rw-r--r--   0        0        0    10675 2020-02-02 00:00:00.000000 taxpasta-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/__init__.py
+-rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/__main__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/_version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/py.typed
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/application/__init__.py
+-rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/application/consensus_application.py
+-rw-r--r--   0        0        0     6348 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/application/sample_merging_application.py
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/application/error/__init__.py
+-rw-r--r--   0        0        0     1260 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/application/error/standardisation_error.py
+-rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/application/error/taxpasta_error.py
+-rw-r--r--   0        0        0     1126 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/application/service/__init__.py
+-rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/application/service/_types.py
+-rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/application/service/profile_reader.py
+-rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/application/service/profile_standardisation_service.py
+-rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/application/service/standard_profile_writer.py
+-rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/application/service/table_reader.py
+-rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/application/service/tidy_observation_table_writer.py
+-rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/application/service/wide_observation_table_writer.py
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/domain/__init__.py
+-rw-r--r--   0        0        0      888 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/domain/model/__init__.py
+-rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/domain/model/sample.py
+-rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/domain/model/standard_profile.py
+-rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/domain/model/tidy_observation_table.py
+-rw-r--r--   0        0        0     1292 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/domain/model/wide_observation_table.py
+-rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/domain/service/__init__.py
+-rw-r--r--   0        0        0     1247 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/domain/service/consensus_builder.py
+-rw-r--r--   0        0        0     4067 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/domain/service/sample_merging_service.py
+-rw-r--r--   0        0        0     2892 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/domain/service/taxonomy_service.py
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/__init__.py
+-rw-r--r--   0        0        0     2336 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/__init__.py
+-rw-r--r--   0        0        0     4592 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/_dependency_check_mixin.py
+-rw-r--r--   0        0        0    12542 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/application_service_registry.py
+-rw-r--r--   0        0        0     3774 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/sample_etl_application.py
+-rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/sample_sheet.py
+-rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/standard_profile_file_format.py
+-rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/supported_profiler.py
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/table_reader_file_format.py
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/tidy_observation_table_file_format.py
+-rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/wide_observation_table_file_format.py
+-rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/bracken/__init__.py
+-rw-r--r--   0        0        0     2084 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/bracken/bracken_profile.py
+-rw-r--r--   0        0        0     1750 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/bracken/bracken_profile_reader.py
+-rw-r--r--   0        0        0     2096 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/bracken/bracken_profile_standardisation_service.py
+-rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/centrifuge/__init__.py
+-rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/centrifuge/centrifuge_profile.py
+-rw-r--r--   0        0        0     2133 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/centrifuge/centrifuge_profile_reader.py
+-rw-r--r--   0        0        0     1992 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/centrifuge/centrifuge_profile_standardisation_service.py
+-rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/diamond/__init__.py
+-rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/diamond/diamond_profile.py
+-rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/diamond/diamond_profile_reader.py
+-rw-r--r--   0        0        0     1960 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/diamond/diamond_profile_standardisation_service.py
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/ganon/__init__.py
+-rw-r--r--   0        0        0     1993 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/ganon/ganon_profile.py
+-rw-r--r--   0        0        0     2166 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/ganon/ganon_profile_reader.py
+-rw-r--r--   0        0        0     3057 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/ganon/ganon_profile_standardisation_service.py
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/kaiju/__init__.py
+-rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/kaiju/kaiju_profile.py
+-rw-r--r--   0        0        0     1769 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/kaiju/kaiju_profile_reader.py
+-rw-r--r--   0        0        0     2672 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/kaiju/kaiju_profile_standardisation_service.py
+-rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/kraken2/__init__.py
+-rw-r--r--   0        0        0     2097 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/kraken2/kraken2_profile.py
+-rw-r--r--   0        0        0     2841 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/kraken2/kraken2_profile_reader.py
+-rw-r--r--   0        0        0     1871 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/kraken2/kraken2_profile_standardisation_service.py
+-rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/krakenuniq/__init__.py
+-rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/krakenuniq/krakenuniq_profile.py
+-rw-r--r--   0        0        0     1858 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/krakenuniq/krakenuniq_profile_reader.py
+-rw-r--r--   0        0        0     1873 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/krakenuniq/krakenuniq_profile_standardisation_service.py
+-rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/megan6/__init__.py
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/megan6/megan6_profile.py
+-rw-r--r--   0        0        0     1551 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/megan6/megan6_profile_reader.py
+-rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/megan6/megan6_profile_standardisation_service.py
+-rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/metaphlan/__init__.py
+-rw-r--r--   0        0        0     1868 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/metaphlan/metaphlan_profile.py
+-rw-r--r--   0        0        0     3475 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/metaphlan/metaphlan_profile_reader.py
+-rw-r--r--   0        0        0     3671 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/metaphlan/metaphlan_profile_standardisation_service.py
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/motus/__init__.py
+-rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/motus/motus_profile.py
+-rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/motus/motus_profile_reader.py
+-rw-r--r--   0        0        0     3367 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/motus/motus_profile_standardisation_service.py
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/standard_profile_writer/__init__.py
+-rw-r--r--   0        0        0     1292 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/standard_profile_writer/arrow_standard_profile_writer.py
+-rw-r--r--   0        0        0     1257 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/standard_profile_writer/csv_standard_profile_writer.py
+-rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/standard_profile_writer/ods_standard_profile_writer.py
+-rw-r--r--   0        0        0     1298 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/standard_profile_writer/parquet_standard_profile_writer.py
+-rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/standard_profile_writer/tsv_standard_profile_writer.py
+-rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/standard_profile_writer/xlsx_standard_profile_writer.py
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/table_reader/__init__.py
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/table_reader/arrow_table_reader.py
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/table_reader/csv_table_reader.py
+-rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/table_reader/ods_table_reader.py
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/table_reader/parquet_table_reader.py
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/table_reader/tsv_table_reader.py
+-rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/table_reader/xlsx_table_reader.py
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/tidy_observation_table_writer/__init__.py
+-rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/tidy_observation_table_writer/arrow_table_writer.py
+-rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/tidy_observation_table_writer/csv_table_writer.py
+-rw-r--r--   0        0        0     1330 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/tidy_observation_table_writer/ods_table_writer.py
+-rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/tidy_observation_table_writer/parquet_table_writer.py
+-rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/tidy_observation_table_writer/tsv_table_writer.py
+-rw-r--r--   0        0        0     1338 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/tidy_observation_table_writer/xlsx_table_writer.py
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/wide_observation_table_writer/__init__.py
+-rw-r--r--   0        0        0     1313 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/wide_observation_table_writer/arrow_wide_observation_table_writer.py
+-rw-r--r--   0        0        0     2346 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/wide_observation_table_writer/biom_wide_observation_table_writer.py
+-rw-r--r--   0        0        0     1265 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/wide_observation_table_writer/csv_wide_observation_table_writer.py
+-rw-r--r--   0        0        0     1332 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/wide_observation_table_writer/ods_wide_observation_table_writer.py
+-rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/wide_observation_table_writer/parquet_wide_observation_table_writer.py
+-rw-r--r--   0        0        0     1276 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/wide_observation_table_writer/tsv_wide_observation_table_writer.py
+-rw-r--r--   0        0        0     1340 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/application/wide_observation_table_writer/xlsx_wide_observation_table_writer.py
+-rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/cli/__init__.py
+-rw-r--r--   0        0        0    17017 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/cli/merge.py
+-rw-r--r--   0        0        0     9599 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/cli/standardise.py
+-rw-r--r--   0        0        0     2582 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/cli/taxpasta.py
+-rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/domain/__init__.py
+-rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/domain/service/__init__.py
+-rw-r--r--   0        0        0     6972 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/domain/service/taxopy_taxonomy_service.py
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/helpers/__init__.py
+-rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/helpers/base_data_frame_model.py
+-rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 taxpasta-0.4.0/src/taxpasta/infrastructure/helpers/decorators.py
+-rw-r--r--   0        0        0    13853 2020-02-02 00:00:00.000000 taxpasta-0.4.0/.gitignore
+-rw-r--r--   0        0        0    10174 2020-02-02 00:00:00.000000 taxpasta-0.4.0/LICENSE
+-rw-r--r--   0        0        0     8947 2020-02-02 00:00:00.000000 taxpasta-0.4.0/README.md
+-rw-r--r--   0        0        0     4045 2020-02-02 00:00:00.000000 taxpasta-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0    11594 2020-02-02 00:00:00.000000 taxpasta-0.4.0/PKG-INFO
```

### Comparing `taxpasta-0.3.0/src/taxpasta/__init__.py` & `taxpasta-0.4.0/src/taxpasta/__init__.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.3.0/src/taxpasta/__main__.py` & `taxpasta-0.4.0/src/taxpasta/__main__.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.3.0/src/taxpasta/application/__init__.py` & `taxpasta-0.4.0/src/taxpasta/application/__init__.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.3.0/src/taxpasta/application/consensus_application.py` & `taxpasta-0.4.0/src/taxpasta/application/consensus_application.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.3.0/src/taxpasta/application/sample_merging_application.py` & `taxpasta-0.4.0/src/taxpasta/application/sample_merging_application.py`

 * *Files 0% similar despite different names*

```diff
@@ -144,15 +144,15 @@
                     ) from errors
             except ValueError as error:
                 if ignore_error:
                     logger.error("Sample %s: %s", name, str(error))
                     continue
                 else:
                     raise StandardisationError(
-                        sample=name, profile=profile, message=str(error.args)
+                        sample=name, profile=profile, message=str(error)
                     ) from error
         return result
 
     def _summarise_samples(
         self, samples: List[Sample], rank: str, ignore_error: bool
     ) -> List[Sample]:
         """Summarise samples at a given taxonomic rank."""
```

### Comparing `taxpasta-0.3.0/src/taxpasta/application/error/__init__.py` & `taxpasta-0.4.0/src/taxpasta/application/error/__init__.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.3.0/src/taxpasta/application/error/standardisation_error.py` & `taxpasta-0.4.0/src/taxpasta/application/error/standardisation_error.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.3.0/src/taxpasta/application/error/taxpasta_error.py` & `taxpasta-0.4.0/src/taxpasta/application/error/taxpasta_error.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.3.0/src/taxpasta/application/service/__init__.py` & `taxpasta-0.4.0/src/taxpasta/application/service/__init__.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.3.0/src/taxpasta/application/service/_types.py` & `taxpasta-0.4.0/src/taxpasta/application/service/_types.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.3.0/src/taxpasta/application/service/profile_reader.py` & `taxpasta-0.4.0/src/taxpasta/application/service/profile_reader.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.3.0/src/taxpasta/application/service/profile_standardisation_service.py` & `taxpasta-0.4.0/src/taxpasta/application/service/profile_standardisation_service.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.3.0/src/taxpasta/application/service/standard_profile_writer.py` & `taxpasta-0.4.0/src/taxpasta/application/service/standard_profile_writer.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.3.0/src/taxpasta/application/service/table_reader.py` & `taxpasta-0.4.0/src/taxpasta/application/service/table_reader.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.3.0/src/taxpasta/application/service/tidy_observation_table_writer.py` & `taxpasta-0.4.0/src/taxpasta/application/service/tidy_observation_table_writer.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.3.0/src/taxpasta/application/service/wide_observation_table_writer.py` & `taxpasta-0.4.0/src/taxpasta/application/service/wide_observation_table_writer.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.3.0/src/taxpasta/domain/__init__.py` & `taxpasta-0.4.0/src/taxpasta/domain/__init__.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.3.0/src/taxpasta/domain/model/__init__.py` & `taxpasta-0.4.0/src/taxpasta/domain/model/__init__.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.3.0/src/taxpasta/domain/model/sample.py` & `taxpasta-0.4.0/src/taxpasta/domain/model/sample.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.3.0/src/taxpasta/domain/model/standard_profile.py` & `taxpasta-0.4.0/src/taxpasta/domain/model/standard_profile.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.3.0/src/taxpasta/domain/model/tidy_observation_table.py` & `taxpasta-0.4.0/src/taxpasta/domain/model/tidy_observation_table.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.3.0/src/taxpasta/domain/model/wide_observation_table.py` & `taxpasta-0.4.0/src/taxpasta/domain/model/wide_observation_table.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.3.0/src/taxpasta/domain/service/__init__.py` & `taxpasta-0.4.0/src/taxpasta/domain/service/__init__.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.3.0/src/taxpasta/domain/service/consensus_builder.py` & `taxpasta-0.4.0/src/taxpasta/domain/service/consensus_builder.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.3.0/src/taxpasta/domain/service/sample_merging_service.py` & `taxpasta-0.4.0/src/taxpasta/domain/service/sample_merging_service.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.3.0/src/taxpasta/domain/service/taxonomy_service.py` & `taxpasta-0.4.0/src/taxpasta/domain/service/taxonomy_service.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.3.0/src/taxpasta/infrastructure/__init__.py` & `taxpasta-0.4.0/src/taxpasta/infrastructure/__init__.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.3.0/src/taxpasta/infrastructure/application/__init__.py` & `taxpasta-0.4.0/src/taxpasta/infrastructure/application/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -27,14 +27,19 @@
     CentrifugeProfileStandardisationService,
 )
 from .diamond import (
     DiamondProfile,
     DiamondProfileReader,
     DiamondProfileStandardisationService,
 )
+from .ganon import (
+    GanonProfile,
+    GanonProfileReader,
+    GanonProfileStandardisationService,
+)
 from .kaiju import (
     KaijuProfile,
     KaijuProfileReader,
     KaijuProfileStandardisationService,
 )
 from .kraken2 import (
     Kraken2Profile,
@@ -57,14 +62,15 @@
     MetaphlanProfileStandardisationService,
 )
 from .motus import (
     MotusProfile,
     MotusProfileReader,
     MotusProfileStandardisationService,
 )
+
 from .sample_etl_application import SampleETLApplication
 from .standard_profile_file_format import StandardProfileFileFormat
 from .table_reader_file_format import TableReaderFileFormat
 from .tidy_observation_table_file_format import TidyObservationTableFileFormat
 from .wide_observation_table_file_format import WideObservationTableFileFormat
 from .supported_profiler import SupportedProfiler
 from .application_service_registry import ApplicationServiceRegistry
```

### Comparing `taxpasta-0.3.0/src/taxpasta/infrastructure/application/_dependency_check_mixin.py` & `taxpasta-0.4.0/src/taxpasta/infrastructure/application/_dependency_check_mixin.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.3.0/src/taxpasta/infrastructure/application/application_service_registry.py` & `taxpasta-0.4.0/src/taxpasta/infrastructure/application/application_service_registry.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,14 +52,18 @@
             from .centrifuge import CentrifugeProfileReader
 
             return CentrifugeProfileReader
         elif profiler is SupportedProfiler.diamond:
             from .diamond import DiamondProfileReader
 
             return DiamondProfileReader
+        elif profiler is SupportedProfiler.ganon:
+            from .ganon import GanonProfileReader
+
+            return GanonProfileReader
         elif profiler is SupportedProfiler.kaiju:
             from .kaiju import KaijuProfileReader
 
             return KaijuProfileReader
         elif profiler is SupportedProfiler.kraken2:
             from .kraken2 import Kraken2ProfileReader
 
@@ -118,14 +122,19 @@
             from .motus import MotusProfileStandardisationService
 
             return MotusProfileStandardisationService
         elif profiler is SupportedProfiler.metaphlan:
             from .metaphlan import MetaphlanProfileStandardisationService
 
             return MetaphlanProfileStandardisationService
+        elif profiler is SupportedProfiler.ganon:
+            from .ganon import GanonProfileStandardisationService
+
+            return GanonProfileStandardisationService
+
         else:
             raise ValueError("Unexpected")
 
     @classmethod
     def standard_profile_writer(
         cls, file_format: StandardProfileFileFormat
     ) -> Type[StandardProfileWriter]:
```

### Comparing `taxpasta-0.3.0/src/taxpasta/infrastructure/application/sample_etl_application.py` & `taxpasta-0.4.0/src/taxpasta/infrastructure/application/sample_etl_application.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,19 +92,19 @@
         """
         if name is None:
             name = profile.stem
         try:
             result = self.standardiser.transform(self.reader.read(profile))
         except SchemaErrors as errors:
             raise StandardisationError(
-                sample=profile.stem, profile=profile, message=str(errors.failure_cases)
+                sample=name, profile=profile, message=str(errors.failure_cases)
             ) from errors
         except ValueError as error:
             raise StandardisationError(
-                sample=name, profile=profile, message=str(error.args)
+                sample=name, profile=profile, message=str(error)
             ) from error
 
         if summarise_at is not None:
             assert self.taxonomy is not None  # nosec assert_used
 
             result = self.taxonomy.summarise_at(result, summarise_at)
```

### Comparing `taxpasta-0.3.0/src/taxpasta/infrastructure/application/sample_sheet.py` & `taxpasta-0.4.0/src/taxpasta/infrastructure/application/sample_sheet.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.3.0/src/taxpasta/infrastructure/application/standard_profile_file_format.py` & `taxpasta-0.4.0/src/taxpasta/infrastructure/application/standard_profile_file_format.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.3.0/src/taxpasta/infrastructure/application/supported_profiler.py` & `taxpasta-0.4.0/src/taxpasta/infrastructure/application/supported_profiler.py`

 * *Files 9% similar despite different names*

```diff
@@ -25,13 +25,14 @@
 @unique
 class SupportedProfiler(str, Enum):
     """Define supported taxonomic profilers."""
 
     bracken = "bracken"
     centrifuge = "centrifuge"
     diamond = "diamond"
+    ganon = "ganon"
     kaiju = "kaiju"
     kraken2 = "kraken2"
     krakenuniq = "krakenuniq"
     megan6 = "megan6"
     metaphlan = "metaphlan"
     motus = "motus"
```

### Comparing `taxpasta-0.3.0/src/taxpasta/infrastructure/application/table_reader_file_format.py` & `taxpasta-0.4.0/src/taxpasta/infrastructure/application/table_reader_file_format.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.3.0/src/taxpasta/infrastructure/application/tidy_observation_table_file_format.py` & `taxpasta-0.4.0/src/taxpasta/infrastructure/application/tidy_observation_table_file_format.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.3.0/src/taxpasta/infrastructure/application/wide_observation_table_file_format.py` & `taxpasta-0.4.0/src/taxpasta/infrastructure/application/wide_observation_table_file_format.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.3.0/src/taxpasta/infrastructure/application/bracken/__init__.py` & `taxpasta-0.4.0/src/taxpasta/infrastructure/application/bracken/__init__.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.3.0/src/taxpasta/infrastructure/application/bracken/bracken_profile.py` & `taxpasta-0.4.0/src/taxpasta/infrastructure/application/bracken/bracken_profile.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,47 +16,39 @@
 # limitations under the License.
 
 
 """Provide a description of the Bracken profile format."""
 
 
 import numpy as np
-import pandas as pd
 import pandera as pa
 from pandera.typing import DataFrame, Series
 
+from taxpasta.infrastructure.helpers import BaseDataFrameModel
 
-class BrackenProfile(pa.DataFrameModel):
+
+class BrackenProfile(BaseDataFrameModel):
     """Define the expected Bracken profile format."""
 
     name: Series[str] = pa.Field()
     taxonomy_id: Series[int] = pa.Field(ge=0)
-    taxonomy_lvl: Series[pd.CategoricalDtype] = pa.Field()
+    taxonomy_lvl: Series[str] = pa.Field()
     kraken_assigned_reads: Series[int] = pa.Field(ge=0)
     added_reads: Series[int] = pa.Field(ge=0)
     new_est_reads: Series[int] = pa.Field(ge=0)
     fraction_total_reads: Series[float] = pa.Field(ge=0.0, le=1.0)
 
     @pa.check("fraction_total_reads", name="compositionality")
-    @classmethod
     def check_compositionality(cls, fraction_total_reads: Series[float]) -> bool:
         """Check that the fractions of reads add up to one."""
         # Bracken reports fractions with five decimals but rounding errors accumulate.
         return fraction_total_reads.empty or bool(
             np.isclose(fraction_total_reads.sum(), 1.0, atol=0.02)
         )
 
     @pa.dataframe_check
-    @classmethod
     def check_added_reads_consistency(cls, profile: DataFrame) -> Series[bool]:
         """Check that Bracken added reads are consistent."""
         return (
             profile[cls.kraken_assigned_reads] + profile[cls.added_reads]
             == profile[cls.new_est_reads]
         )
-
-    class Config:
-        """Configure the schema model."""
-
-        coerce = True
-        ordered = True
-        strict = True
```

### Comparing `taxpasta-0.3.0/src/taxpasta/infrastructure/application/bracken/bracken_profile_reader.py` & `taxpasta-0.4.0/src/taxpasta/infrastructure/application/kaiju/kaiju_profile_reader.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,42 +12,45 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-"""Provide a reader for Bracken profiles."""
+"""Provide a reader for kaiju profiles."""
 
 
 import pandas as pd
 from pandera.typing import DataFrame
 
 from taxpasta.application.service import BufferOrFilepath, ProfileReader
+from taxpasta.infrastructure.helpers import raise_parser_warnings
 
-from .bracken_profile import BrackenProfile
+from .kaiju_profile import KaijuProfile
 
 
-class BrackenProfileReader(ProfileReader):
-    """Define a reader for Bracken profiles."""
+class KaijuProfileReader(ProfileReader):
+    """Define a reader for kaiju profiles."""
 
     @classmethod
-    def read(cls, profile: BufferOrFilepath) -> DataFrame[BrackenProfile]:
+    @raise_parser_warnings
+    def read(cls, profile: BufferOrFilepath) -> DataFrame[KaijuProfile]:
         """
-        Read a Bracken taxonomic profile from the given source.
+        Read a kaiju taxonomic profile from the given source.
 
         Args:
             profile: A source that contains a tab-separated taxonomic profile generated
-                by Bracken.
+                by kaiju.
 
         Returns:
-            A data frame representation of the Bracken profile.
+            A data frame representation of the kaiju profile.
 
         """
         result = pd.read_table(
             filepath_or_buffer=profile,
             sep="\t",
+            header=0,
             index_col=False,
-            skipinitialspace=True,
+            dtype={KaijuProfile.taxon_id: "Int64"},
         )
-        cls._check_num_columns(result, BrackenProfile)
+        cls._check_num_columns(result, KaijuProfile)
         return result
```

### Comparing `taxpasta-0.3.0/src/taxpasta/infrastructure/application/bracken/bracken_profile_standardisation_service.py` & `taxpasta-0.4.0/src/taxpasta/infrastructure/application/bracken/bracken_profile_standardisation_service.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.3.0/src/taxpasta/infrastructure/application/centrifuge/__init__.py` & `taxpasta-0.4.0/src/taxpasta/infrastructure/application/centrifuge/__init__.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.3.0/src/taxpasta/infrastructure/application/centrifuge/centrifuge_profile.py` & `taxpasta-0.4.0/src/taxpasta/infrastructure/application/centrifuge/centrifuge_profile.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,34 +16,27 @@
 # limitations under the License.
 
 
 """Provide a description of the centrifuge profile format."""
 
 
 import numpy as np
-import pandas as pd
 import pandera as pa
 from pandera.typing import Series
 
+from taxpasta.infrastructure.helpers import BaseDataFrameModel
 
-class CentrifugeProfile(pa.DataFrameModel):
+
+class CentrifugeProfile(BaseDataFrameModel):
     """Define the expected centrifuge profile format."""
 
     percent: Series[float] = pa.Field(ge=0.0, le=100.0)
     clade_assigned_reads: Series[int] = pa.Field(ge=0)
     direct_assigned_reads: Series[int] = pa.Field(ge=0)
-    taxonomy_level: Series[pd.CategoricalDtype] = pa.Field()
+    taxonomy_level: Series[str] = pa.Field()
     taxonomy_id: Series[int] = pa.Field(ge=0)
     name: Series[str] = pa.Field()
 
     @pa.check("percent", name="compositionality")
-    @classmethod
     def check_compositionality(cls, percent: Series[float]) -> bool:
         """Check that the percent of 'unclassified' and 'root' add up to a hundred."""
         return percent.empty or bool(np.isclose(percent[:2].sum(), 100.0, atol=1.0))
-
-    class Config:
-        """Configure the schema model."""
-
-        coerce = True
-        ordered = True
-        strict = True
```

### Comparing `taxpasta-0.3.0/src/taxpasta/infrastructure/application/centrifuge/centrifuge_profile_reader.py` & `taxpasta-0.4.0/src/taxpasta/infrastructure/application/centrifuge/centrifuge_profile_reader.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,22 +19,24 @@
 """Provide a reader for Centrifuge profiles."""
 
 
 import pandas as pd
 from pandera.typing import DataFrame
 
 from taxpasta.application.service import BufferOrFilepath, ProfileReader
+from taxpasta.infrastructure.helpers import raise_parser_warnings
 
 from .centrifuge_profile import CentrifugeProfile
 
 
 class CentrifugeProfileReader(ProfileReader):
     """Define a reader for centrifuge profiles."""
 
     @classmethod
+    @raise_parser_warnings
     def read(cls, profile: BufferOrFilepath) -> DataFrame[CentrifugeProfile]:
         """
         Read a centrifuge taxonomic profile from the given source.
 
         Args:
             profile: A source that contains a tab-separated taxonomic profile generated
                 by centrifuge.
```

### Comparing `taxpasta-0.3.0/src/taxpasta/infrastructure/application/centrifuge/centrifuge_profile_standardisation_service.py` & `taxpasta-0.4.0/src/taxpasta/infrastructure/application/centrifuge/centrifuge_profile_standardisation_service.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.3.0/src/taxpasta/infrastructure/application/diamond/__init__.py` & `taxpasta-0.4.0/src/taxpasta/infrastructure/application/diamond/__init__.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.3.0/src/taxpasta/infrastructure/application/diamond/diamond_profile.py` & `taxpasta-0.4.0/src/taxpasta/infrastructure/application/motus/motus_profile.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,27 +12,23 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-"""Provide a description of the diamond profile format."""
+"""Provide a description of the mOTUs profile format."""
 
 
+import pandas as pd
 import pandera as pa
 from pandera.typing import Series
 
+from taxpasta.infrastructure.helpers import BaseDataFrameModel
 
-class DiamondProfile(pa.DataFrameModel):
-    """Define the expected diamond profile format."""
 
-    query_id: Series[str] = pa.Field()
-    taxonomy_id: Series[int] = pa.Field(ge=0)
-    e_value: Series[float] = pa.Field(ge=0.0, le=1.0)
-
-    class Config:
-        """Configure the schema model."""
-
-        coerce = True
-        ordered = True
-        strict = True
+class MotusProfile(BaseDataFrameModel):
+    """Define the expected mOTUs profile format."""
+
+    consensus_taxonomy: Series[str] = pa.Field()
+    ncbi_tax_id: Series[pd.Int64Dtype] = pa.Field(nullable=True)
+    read_count: Series[int] = pa.Field(ge=0)
```

### Comparing `taxpasta-0.3.0/src/taxpasta/infrastructure/application/diamond/diamond_profile_reader.py` & `taxpasta-0.4.0/src/taxpasta/infrastructure/application/diamond/diamond_profile_reader.py`

 * *Files 16% similar despite different names*

```diff
@@ -18,32 +18,33 @@
 
 """Provide a reader for diamond profiles."""
 
 import pandas as pd
 from pandera.typing import DataFrame
 
 from taxpasta.application.service import BufferOrFilepath, ProfileReader
+from taxpasta.infrastructure.helpers import raise_parser_warnings
 
 from .diamond_profile import DiamondProfile
 
 
 class DiamondProfileReader(ProfileReader):
     """Define a reader for Diamond profiles."""
 
-    LARGE_INTEGER = int(10e6)
-
     @classmethod
+    @raise_parser_warnings
     def read(cls, profile: BufferOrFilepath) -> DataFrame[DiamondProfile]:
         """Read a diamond taxonomic profile from a file."""
         result = pd.read_table(
             filepath_or_buffer=profile,
             sep="\t",
             header=None,
             index_col=False,
             names=[
                 DiamondProfile.query_id,
                 DiamondProfile.taxonomy_id,
                 DiamondProfile.e_value,
             ],
+            dtype={DiamondProfile.e_value: float},
         )
         cls._check_num_columns(result, DiamondProfile)
         return result
```

### Comparing `taxpasta-0.3.0/src/taxpasta/infrastructure/application/diamond/diamond_profile_standardisation_service.py` & `taxpasta-0.4.0/src/taxpasta/infrastructure/application/diamond/diamond_profile_standardisation_service.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.3.0/src/taxpasta/infrastructure/application/kaiju/__init__.py` & `taxpasta-0.4.0/src/taxpasta/infrastructure/application/kaiju/__init__.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.3.0/src/taxpasta/infrastructure/application/kaiju/kaiju_profile.py` & `taxpasta-0.4.0/src/taxpasta/infrastructure/application/kaiju/kaiju_profile.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,36 +20,29 @@
 
 
 import numpy as np
 import pandas as pd
 import pandera as pa
 from pandera.typing import Series
 
+from taxpasta.infrastructure.helpers import BaseDataFrameModel
 
-class KaijuProfile(pa.DataFrameModel):
+
+class KaijuProfile(BaseDataFrameModel):
     """Define the expected kaiju profile format."""
 
     file: Series[str] = pa.Field()
     percent: Series[float] = pa.Field(ge=0.0, le=100.0)
     reads: Series[int] = pa.Field(ge=0)
     taxon_id: Series[pd.Int64Dtype] = pa.Field(nullable=True)
     taxon_name: Series[str] = pa.Field()
 
     @pa.check("percent", name="compositionality")
-    @classmethod
     def check_compositionality(cls, percent: Series[float]) -> bool:
         """Check that the percentages add up to a hundred."""
         # Kaiju reports percentages with sixth decimals
         return percent.empty or bool(np.isclose(percent.sum(), 100.0, atol=1.0))
 
     @pa.check("file", name="unique_filename")
-    @classmethod
     def check_unique_filename(cls, file_col: Series[str]) -> bool:
         """Check that Kaiju filename is unique."""
         return file_col.empty or file_col.nunique() == 1
-
-    class Config:
-        """Configure the schema model."""
-
-        coerce = True
-        ordered = True
-        strict = True
```

### Comparing `taxpasta-0.3.0/src/taxpasta/infrastructure/application/kaiju/kaiju_profile_reader.py` & `taxpasta-0.4.0/src/taxpasta/infrastructure/application/motus/motus_profile_reader.py`

 * *Files 15% similar despite different names*

```diff
@@ -12,43 +12,41 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-"""Provide a reader for kaiju profiles."""
+"""Provide a reader for motus profiles."""
 
 
 import pandas as pd
 from pandera.typing import DataFrame
 
 from taxpasta.application.service import BufferOrFilepath, ProfileReader
+from taxpasta.infrastructure.helpers import raise_parser_warnings
 
-from .kaiju_profile import KaijuProfile
+from .motus_profile import MotusProfile
 
 
-class KaijuProfileReader(ProfileReader):
-    """Define a reader for kaiju profiles."""
+class MotusProfileReader(ProfileReader):
+    """Define a reader for mOTUS profiles."""
 
     @classmethod
-    def read(cls, profile: BufferOrFilepath) -> DataFrame[KaijuProfile]:
-        """
-        Read a kaiju taxonomic profile from the given source.
-
-        Args:
-            profile: A source that contains a tab-separated taxonomic profile generated
-                by kaiju.
-
-        Returns:
-            A data frame representation of the kaiju profile.
-
-        """
+    @raise_parser_warnings
+    def read(cls, profile: BufferOrFilepath) -> DataFrame[MotusProfile]:
+        """Read a mOTUs taxonomic profile from a file."""
         result = pd.read_table(
             filepath_or_buffer=profile,
             sep="\t",
-            header=0,
+            skiprows=3,
+            header=None,
+            names=[
+                MotusProfile.consensus_taxonomy,
+                MotusProfile.ncbi_tax_id,
+                MotusProfile.read_count,
+            ],
             index_col=False,
-            dtype={KaijuProfile.taxon_id: str},
+            dtype={MotusProfile.ncbi_tax_id: "Int64"},
         )
-        cls._check_num_columns(result, KaijuProfile)
+        cls._check_num_columns(result, MotusProfile)
         return result
```

### Comparing `taxpasta-0.3.0/src/taxpasta/infrastructure/application/kaiju/kaiju_profile_standardisation_service.py` & `taxpasta-0.4.0/src/taxpasta/infrastructure/application/kaiju/kaiju_profile_standardisation_service.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.3.0/src/taxpasta/infrastructure/application/kraken2/__init__.py` & `taxpasta-0.4.0/src/taxpasta/infrastructure/application/kraken2/__init__.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.3.0/src/taxpasta/infrastructure/application/kraken2/kraken2_profile.py` & `taxpasta-0.4.0/src/taxpasta/infrastructure/application/kraken2/kraken2_profile.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,43 +22,37 @@
 from typing import Optional
 
 import numpy as np
 import pandas as pd
 import pandera as pa
 from pandera.typing import Series
 
+from taxpasta.infrastructure.helpers import BaseDataFrameModel
 
-class Kraken2Profile(pa.DataFrameModel):
+
+class Kraken2Profile(BaseDataFrameModel):
     """Define the expected kraken2 profile format."""
 
     percent: Series[float] = pa.Field(ge=0.0, le=100.0)
     clade_assigned_reads: Series[int] = pa.Field(ge=0)
     direct_assigned_reads: Series[int] = pa.Field(ge=0)
     num_minimizers: Optional[Series[int]] = pa.Field(ge=0)
     distinct_minimizers: Optional[Series[int]] = pa.Field(ge=0)
-    taxonomy_lvl: Series[pd.CategoricalDtype] = pa.Field()
+    taxonomy_lvl: Series[str] = pa.Field()
     taxonomy_id: Series[int] = pa.Field(ge=0)
     name: Series[str] = pa.Field()
 
     @pa.dataframe_check
-    @classmethod
     def check_compositionality(cls, profile: pd.DataFrame) -> bool:
         """Check that the percent of 'unclassified' and 'root' add up to a hundred."""
         # Kraken2 reports percentages only to the second decimal, so we expect
         # some deviation.
         # If 100% of reads are assigned, unclassified reads are not reported at all.
         return profile.empty or bool(
             np.isclose(
                 profile.loc[
                     profile[cls.taxonomy_lvl].isin(["U", "R"]), cls.percent
                 ].sum(),
                 100.0,
                 atol=1.0,
             )
         )
-
-    class Config:
-        """Configure the schema model."""
-
-        coerce = True
-        ordered = True
-        strict = True
```

### Comparing `taxpasta-0.3.0/src/taxpasta/infrastructure/application/kraken2/kraken2_profile_reader.py` & `taxpasta-0.4.0/src/taxpasta/infrastructure/application/kraken2/kraken2_profile_reader.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,22 +19,24 @@
 """Provide a reader for kraken2 profiles."""
 
 
 import pandas as pd
 from pandera.typing import DataFrame
 
 from taxpasta.application.service import BufferOrFilepath, ProfileReader
+from taxpasta.infrastructure.helpers import raise_parser_warnings
 
 from .kraken2_profile import Kraken2Profile
 
 
 class Kraken2ProfileReader(ProfileReader):
     """Define a reader for kraken2 profiles."""
 
     @classmethod
+    @raise_parser_warnings
     def read(cls, profile: BufferOrFilepath) -> DataFrame[Kraken2Profile]:
         """
         Read a kraken2 taxonomic profile from the given source.
 
         Args:
             profile: A source that contains a tab-separated taxonomic profile generated
                 by kraken2.
```

### Comparing `taxpasta-0.3.0/src/taxpasta/infrastructure/application/kraken2/kraken2_profile_standardisation_service.py` & `taxpasta-0.4.0/src/taxpasta/infrastructure/application/kraken2/kraken2_profile_standardisation_service.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.3.0/src/taxpasta/infrastructure/application/krakenuniq/__init__.py` & `taxpasta-0.4.0/src/taxpasta/infrastructure/application/krakenuniq/__init__.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.3.0/src/taxpasta/infrastructure/application/krakenuniq/krakenuniq_profile.py` & `taxpasta-0.4.0/src/taxpasta/infrastructure/application/krakenuniq/krakenuniq_profile.py`

 * *Files 22% similar despite different names*

```diff
@@ -15,31 +15,25 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
 """Provide a description of the KrakenUniq profile format."""
 
 
-import pandas as pd
 import pandera as pa
 from pandera.typing import Series
 
+from taxpasta.infrastructure.helpers import BaseDataFrameModel
 
-class KrakenUniqProfile(pa.DataFrameModel):
+
+class KrakenUniqProfile(BaseDataFrameModel):
     """Define the expected KrakenUniq profile format."""
 
     percent: Series[float] = pa.Field(ge=0.0, le=100.0, alias="%")
     reads: Series[int] = pa.Field(ge=0)
     tax_reads: Series[int] = pa.Field(ge=0, alias="taxReads")
     kmers: Series[int] = pa.Field(ge=0)
     duplicates: Series[float] = pa.Field(ge=0.0, alias="dup")
     coverage: Series[float] = pa.Field(ge=0.0, nullable=True, alias="cov")
     tax_id: Series[int] = pa.Field(alias="taxID", ge=0)
-    rank: Series[pd.CategoricalDtype] = pa.Field()
+    rank: Series[str] = pa.Field()
     tax_name: Series[str] = pa.Field(alias="taxName")
-
-    class Config:
-        """Configure the schema model."""
-
-        coerce = True
-        ordered = True
-        strict = True
```

### Comparing `taxpasta-0.3.0/src/taxpasta/infrastructure/application/krakenuniq/krakenuniq_profile_reader.py` & `taxpasta-0.4.0/src/taxpasta/infrastructure/application/krakenuniq/krakenuniq_profile_reader.py`

 * *Files 11% similar despite different names*

```diff
@@ -19,22 +19,24 @@
 """Provide a reader for KrakenUniq profiles."""
 
 
 import pandas as pd
 from pandera.typing import DataFrame
 
 from taxpasta.application.service import BufferOrFilepath, ProfileReader
+from taxpasta.infrastructure.helpers import raise_parser_warnings
 
 from .krakenuniq_profile import KrakenUniqProfile
 
 
 class KrakenUniqProfileReader(ProfileReader):
     """Define a reader for KrakenUniq profiles."""
 
     @classmethod
+    @raise_parser_warnings
     def read(cls, profile: BufferOrFilepath) -> DataFrame[KrakenUniqProfile]:
         """
         Read a krakenUniq taxonomic profile from the given source.
 
         Args:
             profile: A source that contains a tab-separated taxonomic profile generated
                 by KrakenUniq.
@@ -46,10 +48,11 @@
         result = pd.read_table(
             filepath_or_buffer=profile,
             sep="\t",
             skiprows=2,
             header=0,
             index_col=False,
             skipinitialspace=True,
+            dtype={"%": float},
         )
         cls._check_num_columns(result, KrakenUniqProfile)
         return result
```

### Comparing `taxpasta-0.3.0/src/taxpasta/infrastructure/application/krakenuniq/krakenuniq_profile_standardisation_service.py` & `taxpasta-0.4.0/src/taxpasta/infrastructure/application/krakenuniq/krakenuniq_profile_standardisation_service.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.3.0/src/taxpasta/infrastructure/application/megan6/__init__.py` & `taxpasta-0.4.0/src/taxpasta/infrastructure/application/megan6/__init__.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.3.0/src/taxpasta/infrastructure/application/megan6/megan6_profile.py` & `taxpasta-0.4.0/src/taxpasta/infrastructure/application/megan6/megan6_profile.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,20 +18,15 @@
 
 """Provide a description of the MEGAN6 rma2info profile format."""
 
 
 import pandera as pa
 from pandera.typing import Series
 
+from taxpasta.infrastructure.helpers import BaseDataFrameModel
 
-class Megan6Profile(pa.DataFrameModel):
+
+class Megan6Profile(BaseDataFrameModel):
     """Define the expected MEGAN6 rma2info profile format."""
 
     taxonomy_id: Series[int] = pa.Field(ge=0)
-    count: Series[int] = pa.Field(ge=0.0)
-
-    class Config:
-        """Configure the schema model."""
-
-        coerce = True
-        ordered = True
-        strict = True
+    count: Series[float] = pa.Field(ge=0.0)
```

### Comparing `taxpasta-0.3.0/src/taxpasta/infrastructure/application/megan6/megan6_profile_reader.py` & `taxpasta-0.4.0/src/taxpasta/infrastructure/application/megan6/megan6_profile_reader.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,24 +19,24 @@
 """Provide a reader for megan6 profiles."""
 
 
 import pandas as pd
 from pandera.typing import DataFrame
 
 from taxpasta.application.service import BufferOrFilepath, ProfileReader
+from taxpasta.infrastructure.helpers import raise_parser_warnings
 
 from .megan6_profile import Megan6Profile
 
 
 class Megan6ProfileReader(ProfileReader):
     """Define a reader for MEGAN6 rma2info profiles."""
 
-    LARGE_INTEGER = int(10e6)
-
     @classmethod
+    @raise_parser_warnings
     def read(cls, profile: BufferOrFilepath) -> DataFrame[Megan6Profile]:
         """Read a MEGAN6 rma2info taxonomic profile from a file."""
         result = pd.read_table(
             filepath_or_buffer=profile,
             sep="\t",
             names=[Megan6Profile.taxonomy_id, Megan6Profile.count],
             index_col=False,
```

### Comparing `taxpasta-0.3.0/src/taxpasta/infrastructure/application/megan6/megan6_profile_standardisation_service.py` & `taxpasta-0.4.0/src/taxpasta/infrastructure/application/megan6/megan6_profile_standardisation_service.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.3.0/src/taxpasta/infrastructure/application/metaphlan/__init__.py` & `taxpasta-0.4.0/src/taxpasta/infrastructure/application/metaphlan/__init__.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.3.0/src/taxpasta/infrastructure/application/metaphlan/metaphlan_profile.py` & `taxpasta-0.4.0/src/taxpasta/infrastructure/application/metaphlan/metaphlan_profile.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,37 +22,31 @@
 from typing import Optional
 
 import numpy as np
 import pandas as pd
 import pandera as pa
 from pandera.typing import Series
 
+from taxpasta.infrastructure.helpers import BaseDataFrameModel
 
-class MetaphlanProfile(pa.DataFrameModel):
+
+class MetaphlanProfile(BaseDataFrameModel):
     """Define the expected metaphlan profile format."""
 
     clade_name: Series[str] = pa.Field()
     # MetaPhlan provides the full lineage of tax IDs in this field.
     ncbi_tax_id: Series[str] = pa.Field(alias="NCBI_tax_id")
     relative_abundance: Series[float] = pa.Field(ge=0.0, le=100.0)
     additional_species: Optional[Series[str]] = pa.Field(nullable=True)
 
     @pa.dataframe_check
-    @classmethod
     def check_compositionality(cls, profile: pd.DataFrame) -> bool:
         """Check that the percentages per rank add up to a hundred."""
         # Parse the rank from the given lineage.
         rank = profile[cls.clade_name].str.rsplit("|", n=1).str[-1].str[0]
         return profile.empty or bool(
             np.allclose(
                 profile.groupby(rank, sort=False)[cls.relative_abundance].sum(),
                 100.0,
                 atol=1.0,
             )
         )
-
-    class Config:
-        """Configure the schema model."""
-
-        coerce = True
-        ordered = True
-        strict = True
```

### Comparing `taxpasta-0.3.0/src/taxpasta/infrastructure/application/metaphlan/metaphlan_profile_reader.py` & `taxpasta-0.4.0/src/taxpasta/infrastructure/application/ganon/ganon_profile_reader.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,50 +1,67 @@
-# Copyright (c) 2022 Moritz E. Beber
-# Copyright (c) 2022 Maxime Borry
-# Copyright (c) 2022 James A. Fellows Yates
-# Copyright (c) 2022 Sofia Stamouli.
+# Copyright (c) 2023 Moritz E. Beber
+# Copyright (c) 2023 Maxime Borry
+# Copyright (c) 2023 James A. Fellows Yates
+# Copyright (c) 2023 Sofia Stamouli.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-"""Provide a reader for metaphlan profiles."""
+"""Provide a reader for ganon profiles."""
+
 
 import pandas as pd
 from pandera.typing import DataFrame
 
 from taxpasta.application.service import BufferOrFilepath, ProfileReader
+from taxpasta.infrastructure.helpers import raise_parser_warnings
 
-from .metaphlan_profile import MetaphlanProfile
+from .ganon_profile import GanonProfile
 
 
-class MetaphlanProfileReader(ProfileReader):
-    """Define a reader for Metaphlan profiles."""
+class GanonProfileReader(ProfileReader):
+    """Define a reader for ganon profiles."""
 
     @classmethod
-    def read(cls, profile: BufferOrFilepath) -> DataFrame[MetaphlanProfile]:
-        """Read a metaphlan taxonomic profile from a file."""
+    @raise_parser_warnings
+    def read(cls, profile: BufferOrFilepath) -> DataFrame[GanonProfile]:
+        """
+        Read a ganon taxonomic profile from the given source.
+
+        Args:
+            profile: A source that contains a tab-separated taxonomic profile generated
+                by ganon.
+
+        Returns:
+            A data frame representation of the ganon profile.
+
+        """
         result = pd.read_table(
             filepath_or_buffer=profile,
             sep="\t",
-            skiprows=4,
             header=None,
             index_col=False,
+            skipinitialspace=True,
             names=[
-                MetaphlanProfile.clade_name,
-                MetaphlanProfile.ncbi_tax_id,
-                MetaphlanProfile.relative_abundance,
-                MetaphlanProfile.additional_species,
+                GanonProfile.rank,
+                GanonProfile.target,
+                GanonProfile.lineage,
+                GanonProfile.name,
+                GanonProfile.number_unique,
+                GanonProfile.number_shared,
+                GanonProfile.number_children,
+                GanonProfile.number_cumulative,
+                GanonProfile.percent_cumulative,
             ],
-            dtype={MetaphlanProfile.ncbi_tax_id: str},
         )
-        cls._check_num_columns(result, MetaphlanProfile)
+        cls._check_num_columns(result, GanonProfile)
         return result
```

### Comparing `taxpasta-0.3.0/src/taxpasta/infrastructure/application/metaphlan/metaphlan_profile_standardisation_service.py` & `taxpasta-0.4.0/src/taxpasta/infrastructure/application/metaphlan/metaphlan_profile_standardisation_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 logger = logging.getLogger(__name__)
 
 
 class MetaphlanProfileStandardisationService(ProfileStandardisationService):
     """Define a standardisation service for metaphlan profiles."""
 
     # Metaphlan only reports up to six decimals so this number should be large enough.
-    LARGE_INTEGER = int(1e6)
+    LARGE_INTEGER = 1_000_000
 
     @classmethod
     @pa.check_types(lazy=True)
     def transform(
         cls, profile: DataFrame[MetaphlanProfile]
     ) -> DataFrame[StandardProfile]:
         """
```

### Comparing `taxpasta-0.3.0/src/taxpasta/infrastructure/application/motus/__init__.py` & `taxpasta-0.4.0/src/taxpasta/infrastructure/application/motus/__init__.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.3.0/src/taxpasta/infrastructure/application/motus/motus_profile.py` & `taxpasta-0.4.0/src/taxpasta/infrastructure/application/table_reader/tsv_table_reader.py`

 * *Files 22% similar despite different names*

```diff
@@ -12,28 +12,22 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-"""Provide a description of the mOTUs profile format."""
+"""Provide a TSV reader."""
 
 
 import pandas as pd
-import pandera as pa
-from pandera.typing import Series
 
+from taxpasta.application.service import BufferOrFilepath, TableReader
 
-class MotusProfile(pa.DataFrameModel):
-    """Define the expected mOTUs profile format."""
 
-    consensus_taxonomy: Series[str] = pa.Field()
-    ncbi_tax_id: Series[pd.Int64Dtype] = pa.Field(nullable=True)
-    read_count: Series[int] = pa.Field(ge=0)
+class TSVTableReader(TableReader):
+    """Define the TSV reader."""
 
-    class Config:
-        """Configure the schema model."""
-
-        coerce = True
-        ordered = True
-        strict = True
+    @classmethod
+    def read(cls, source: BufferOrFilepath, **kwargs) -> pd.DataFrame:
+        """Read TSV from the given source."""
+        return pd.read_table(source, sep="\t", **kwargs)
```

### Comparing `taxpasta-0.3.0/src/taxpasta/infrastructure/application/motus/motus_profile_reader.py` & `taxpasta-0.4.0/src/taxpasta/infrastructure/application/wide_observation_table_writer/csv_wide_observation_table_writer.py`

 * *Files 24% similar despite different names*

```diff
@@ -12,39 +12,25 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-"""Provide a reader for motus profiles."""
+"""Provide a CSV writer."""
 
 
-import pandas as pd
 from pandera.typing import DataFrame
 
-from taxpasta.application.service import BufferOrFilepath, ProfileReader
+from taxpasta.application.service import BufferOrFilepath, WideObservationTableWriter
+from taxpasta.domain.model import WideObservationTable
 
-from .motus_profile import MotusProfile
 
-
-class MotusProfileReader(ProfileReader):
-    """Define a reader for mOTUS profiles."""
+class CSVWideObservationTableWriter(WideObservationTableWriter):
+    """Define the CSV writer."""
 
     @classmethod
-    def read(cls, profile: BufferOrFilepath) -> DataFrame[MotusProfile]:
-        """Read a mOTUs taxonomic profile from a file."""
-        result = pd.read_table(
-            filepath_or_buffer=profile,
-            sep="\t",
-            skiprows=3,
-            header=None,
-            names=[
-                MotusProfile.consensus_taxonomy,
-                MotusProfile.ncbi_tax_id,
-                MotusProfile.read_count,
-            ],
-            index_col=False,
-            dtype={MotusProfile.ncbi_tax_id: str},
-        )
-        cls._check_num_columns(result, MotusProfile)
-        return result
+    def write(
+        cls, matrix: DataFrame[WideObservationTable], target: BufferOrFilepath, **kwargs
+    ) -> None:
+        """Write the given table to the given buffer or file."""
+        matrix.to_csv(target, index=False, **kwargs)
```

### Comparing `taxpasta-0.3.0/src/taxpasta/infrastructure/application/motus/motus_profile_standardisation_service.py` & `taxpasta-0.4.0/src/taxpasta/infrastructure/application/motus/motus_profile_standardisation_service.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.3.0/src/taxpasta/infrastructure/application/standard_profile_writer/__init__.py` & `taxpasta-0.4.0/src/taxpasta/infrastructure/application/standard_profile_writer/__init__.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.3.0/src/taxpasta/infrastructure/application/standard_profile_writer/arrow_standard_profile_writer.py` & `taxpasta-0.4.0/src/taxpasta/infrastructure/application/standard_profile_writer/arrow_standard_profile_writer.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.3.0/src/taxpasta/infrastructure/application/standard_profile_writer/csv_standard_profile_writer.py` & `taxpasta-0.4.0/src/taxpasta/infrastructure/application/standard_profile_writer/csv_standard_profile_writer.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.3.0/src/taxpasta/infrastructure/application/standard_profile_writer/ods_standard_profile_writer.py` & `taxpasta-0.4.0/src/taxpasta/infrastructure/application/standard_profile_writer/ods_standard_profile_writer.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.3.0/src/taxpasta/infrastructure/application/standard_profile_writer/parquet_standard_profile_writer.py` & `taxpasta-0.4.0/src/taxpasta/infrastructure/application/standard_profile_writer/parquet_standard_profile_writer.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.3.0/src/taxpasta/infrastructure/application/standard_profile_writer/tsv_standard_profile_writer.py` & `taxpasta-0.4.0/src/taxpasta/infrastructure/application/standard_profile_writer/tsv_standard_profile_writer.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.3.0/src/taxpasta/infrastructure/application/standard_profile_writer/xlsx_standard_profile_writer.py` & `taxpasta-0.4.0/src/taxpasta/infrastructure/application/standard_profile_writer/xlsx_standard_profile_writer.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.3.0/src/taxpasta/infrastructure/application/table_reader/__init__.py` & `taxpasta-0.4.0/src/taxpasta/infrastructure/application/table_reader/__init__.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.3.0/src/taxpasta/infrastructure/application/table_reader/arrow_table_reader.py` & `taxpasta-0.4.0/src/taxpasta/infrastructure/application/table_reader/arrow_table_reader.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.3.0/src/taxpasta/infrastructure/application/table_reader/csv_table_reader.py` & `taxpasta-0.4.0/src/taxpasta/infrastructure/application/table_reader/csv_table_reader.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.3.0/src/taxpasta/infrastructure/application/table_reader/ods_table_reader.py` & `taxpasta-0.4.0/src/taxpasta/infrastructure/application/table_reader/ods_table_reader.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.3.0/src/taxpasta/infrastructure/application/table_reader/parquet_table_reader.py` & `taxpasta-0.4.0/src/taxpasta/infrastructure/application/table_reader/parquet_table_reader.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.3.0/src/taxpasta/infrastructure/application/table_reader/tsv_table_reader.py` & `taxpasta-0.4.0/src/taxpasta/infrastructure/application/table_reader/xlsx_table_reader.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,22 +12,22 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-"""Provide a TSV reader."""
+"""Provide an XLSX reader."""
 
 
 import pandas as pd
 
-from taxpasta.application.service import BufferOrFilepath, TableReader
+from taxpasta.application.service import BinaryBufferOrFilepath, TableReader
 
 
-class TSVTableReader(TableReader):
-    """Define the TSV reader."""
+class XLSXTableReader(TableReader):
+    """Define the XLSX reader."""
 
     @classmethod
-    def read(cls, source: BufferOrFilepath, **kwargs) -> pd.DataFrame:
-        """Read TSV from the given source."""
-        return pd.read_table(source, sep="\t", **kwargs)
+    def read(cls, source: BinaryBufferOrFilepath, **kwargs) -> pd.DataFrame:
+        """Read XLSX from the given source."""
+        return pd.read_excel(source, engine="openpyxl", **kwargs)
```

### Comparing `taxpasta-0.3.0/src/taxpasta/infrastructure/application/table_reader/xlsx_table_reader.py` & `taxpasta-0.4.0/src/taxpasta/infrastructure/application/wide_observation_table_writer/tsv_wide_observation_table_writer.py`

 * *Files 20% similar despite different names*

```diff
@@ -12,22 +12,25 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-"""Provide an XLSX reader."""
+"""Provide an TSV writer."""
 
 
-import pandas as pd
+from pandera.typing import DataFrame
 
-from taxpasta.application.service import BinaryBufferOrFilepath, TableReader
+from taxpasta.application.service import BufferOrFilepath, WideObservationTableWriter
+from taxpasta.domain.model import WideObservationTable
 
 
-class XLSXTableReader(TableReader):
-    """Define the XLSX reader."""
+class TSVWideObservationTableWriter(WideObservationTableWriter):
+    """Define the TSV writer."""
 
     @classmethod
-    def read(cls, source: BinaryBufferOrFilepath, **kwargs) -> pd.DataFrame:
-        """Read XLSX from the given source."""
-        return pd.read_excel(source, engine="openpyxl", **kwargs)
+    def write(
+        cls, matrix: DataFrame[WideObservationTable], target: BufferOrFilepath, **kwargs
+    ) -> None:
+        """Write the given table to the given buffer or file."""
+        matrix.to_csv(target, sep="\t", index=False, **kwargs)
```

### Comparing `taxpasta-0.3.0/src/taxpasta/infrastructure/application/tidy_observation_table_writer/__init__.py` & `taxpasta-0.4.0/src/taxpasta/infrastructure/application/tidy_observation_table_writer/__init__.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.3.0/src/taxpasta/infrastructure/application/tidy_observation_table_writer/arrow_table_writer.py` & `taxpasta-0.4.0/src/taxpasta/infrastructure/application/tidy_observation_table_writer/arrow_table_writer.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.3.0/src/taxpasta/infrastructure/application/tidy_observation_table_writer/csv_table_writer.py` & `taxpasta-0.4.0/src/taxpasta/infrastructure/application/tidy_observation_table_writer/csv_table_writer.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.3.0/src/taxpasta/infrastructure/application/tidy_observation_table_writer/ods_table_writer.py` & `taxpasta-0.4.0/src/taxpasta/infrastructure/application/tidy_observation_table_writer/ods_table_writer.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.3.0/src/taxpasta/infrastructure/application/tidy_observation_table_writer/parquet_table_writer.py` & `taxpasta-0.4.0/src/taxpasta/infrastructure/application/tidy_observation_table_writer/parquet_table_writer.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.3.0/src/taxpasta/infrastructure/application/tidy_observation_table_writer/tsv_table_writer.py` & `taxpasta-0.4.0/src/taxpasta/infrastructure/application/tidy_observation_table_writer/tsv_table_writer.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.3.0/src/taxpasta/infrastructure/application/tidy_observation_table_writer/xlsx_table_writer.py` & `taxpasta-0.4.0/src/taxpasta/infrastructure/application/tidy_observation_table_writer/xlsx_table_writer.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.3.0/src/taxpasta/infrastructure/application/wide_observation_table_writer/__init__.py` & `taxpasta-0.4.0/src/taxpasta/infrastructure/application/wide_observation_table_writer/__init__.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.3.0/src/taxpasta/infrastructure/application/wide_observation_table_writer/arrow_wide_observation_table_writer.py` & `taxpasta-0.4.0/src/taxpasta/infrastructure/application/wide_observation_table_writer/arrow_wide_observation_table_writer.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.3.0/src/taxpasta/infrastructure/application/wide_observation_table_writer/biom_wide_observation_table_writer.py` & `taxpasta-0.4.0/src/taxpasta/infrastructure/application/wide_observation_table_writer/biom_wide_observation_table_writer.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.3.0/src/taxpasta/infrastructure/application/wide_observation_table_writer/csv_wide_observation_table_writer.py` & `taxpasta-0.4.0/src/taxpasta/infrastructure/application/wide_observation_table_writer/xlsx_wide_observation_table_writer.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,25 +12,31 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-"""Provide a CSV writer."""
+"""Provide an XLSX writer."""
 
 
 from pandera.typing import DataFrame
 
-from taxpasta.application.service import BufferOrFilepath, WideObservationTableWriter
+from taxpasta.application.service import (
+    BinaryBufferOrFilepath,
+    WideObservationTableWriter,
+)
 from taxpasta.domain.model import WideObservationTable
 
 
-class CSVWideObservationTableWriter(WideObservationTableWriter):
-    """Define the CSV writer."""
+class XLSXWideObservationTableWriter(WideObservationTableWriter):
+    """Define the XLSX writer."""
 
     @classmethod
     def write(
-        cls, matrix: DataFrame[WideObservationTable], target: BufferOrFilepath, **kwargs
+        cls,
+        matrix: DataFrame[WideObservationTable],
+        target: BinaryBufferOrFilepath,
+        **kwargs,
     ) -> None:
         """Write the given table to the given buffer or file."""
-        matrix.to_csv(target, index=False, **kwargs)
+        matrix.to_excel(target, index=False, engine="openpyxl", **kwargs)
```

### Comparing `taxpasta-0.3.0/src/taxpasta/infrastructure/application/wide_observation_table_writer/ods_wide_observation_table_writer.py` & `taxpasta-0.4.0/src/taxpasta/infrastructure/application/wide_observation_table_writer/ods_wide_observation_table_writer.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.3.0/src/taxpasta/infrastructure/application/wide_observation_table_writer/parquet_wide_observation_table_writer.py` & `taxpasta-0.4.0/src/taxpasta/infrastructure/application/wide_observation_table_writer/parquet_wide_observation_table_writer.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.3.0/src/taxpasta/infrastructure/application/wide_observation_table_writer/tsv_wide_observation_table_writer.py` & `taxpasta-0.4.0/src/taxpasta/infrastructure/helpers/base_data_frame_model.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,36 +1,39 @@
-# Copyright (c) 2022 Moritz E. Beber
-# Copyright (c) 2022 Maxime Borry
-# Copyright (c) 2022 James A. Fellows Yates
-# Copyright (c) 2022 Sofia Stamouli.
+# Copyright (c) 2023 Moritz E. Beber
+# Copyright (c) 2023 Maxime Borry
+# Copyright (c) 2023 James A. Fellows Yates
+# Copyright (c) 2023 Sofia Stamouli.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-"""Provide an TSV writer."""
+"""Provide a base data frame model for general checks and configuration."""
 
 
-from pandera.typing import DataFrame
+import pandas as pd
+import pandera as pa
 
-from taxpasta.application.service import BufferOrFilepath, WideObservationTableWriter
-from taxpasta.domain.model import WideObservationTable
 
+class BaseDataFrameModel(pa.DataFrameModel):
+    """Define the base data frame model for general checks and configuration."""
 
-class TSVWideObservationTableWriter(WideObservationTableWriter):
-    """Define the TSV writer."""
+    @pa.dataframe_check
+    def check_not_empty(cls, profile: pd.DataFrame) -> bool:
+        """Check that the read in profile is *not* empty."""
+        return not profile.empty
 
-    @classmethod
-    def write(
-        cls, matrix: DataFrame[WideObservationTable], target: BufferOrFilepath, **kwargs
-    ) -> None:
-        """Write the given table to the given buffer or file."""
-        matrix.to_csv(target, sep="\t", index=False, **kwargs)
+    class Config:
+        """Configure the schema model."""
+
+        coerce = False
+        ordered = True
+        strict = True
```

### Comparing `taxpasta-0.3.0/src/taxpasta/infrastructure/cli/__init__.py` & `taxpasta-0.4.0/src/taxpasta/infrastructure/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.3.0/src/taxpasta/infrastructure/cli/merge.py` & `taxpasta-0.4.0/src/taxpasta/infrastructure/cli/merge.py`

 * *Files 1% similar despite different names*

```diff
@@ -238,25 +238,27 @@
         "file name but can be set explicitly.",
     ),
     output: Path = typer.Option(  # noqa: B008
         ...,
         "--output",
         "-o",
         help="The desired output file. By default, the file extension will be used to "
-        "determine the output format.",
+        "determine the output format, but when setting the format explicitly using "
+        "the --output-format option, automatic detection is disabled.",
         show_default=False,
     ),
     output_format: Optional[
         WideObservationTableFileFormat
     ] = typer.Option(  # noqa: B008
         None,
         case_sensitive=False,
         help="The desired output format. Depending on the choice, additional package "
-        "dependencies may apply. Will be parsed from the output file name but can be "
-        "set explicitly.",
+        "dependencies may apply. By default it will be parsed from the output file "
+        "name but it can be set explicitly and will then disable the automatic "
+        "detection.",
     ),
     wide_format: bool = typer.Option(  # noqa: B008
         True,
         "--wide/--long",
         help="Output merged abundance data in either wide or (tidy) long format. "
         "Ignored when the desired output format is BIOM.",
     ),
```

### Comparing `taxpasta-0.3.0/src/taxpasta/infrastructure/cli/standardise.py` & `taxpasta-0.4.0/src/taxpasta/infrastructure/cli/standardise.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,23 +102,25 @@
         show_default=False,
     ),
     output: Path = typer.Option(  # noqa: B008
         ...,
         "--output",
         "-o",
         help="The desired output file. By default, the file extension will be used to "
-        "determine the output format.",
+        "determine the output format, but when setting the format explicitly using "
+        "the --output-format option, automatic detection is disabled.",
         show_default=False,
     ),
     output_format: Optional[StandardProfileFileFormat] = typer.Option(  # noqa: B008
         None,
         case_sensitive=False,
         help="The desired output format. Depending on the choice, additional package "
-        "dependencies may apply. Will be parsed from the output file name but can be "
-        "set explicitly.",
+        "dependencies may apply. By default it will be parsed from the output file "
+        "name but it can be set explicitly and will then disable the automatic "
+        "detection.",
     ),
     summarise_at: Optional[str] = typer.Option(  # noqa: B008
         None,
         "--summarise-at",
         "--summarize-at",
         help="Summarise abundance profiles at higher taxonomic rank. The provided "
         "option must match a rank in the taxonomy exactly. This is akin to the clade "
```

### Comparing `taxpasta-0.3.0/src/taxpasta/infrastructure/cli/taxpasta.py` & `taxpasta-0.4.0/src/taxpasta/infrastructure/cli/taxpasta.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.3.0/src/taxpasta/infrastructure/domain/__init__.py` & `taxpasta-0.4.0/src/taxpasta/infrastructure/domain/__init__.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.3.0/src/taxpasta/infrastructure/domain/service/__init__.py` & `taxpasta-0.4.0/src/taxpasta/infrastructure/domain/service/__init__.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.3.0/src/taxpasta/infrastructure/domain/service/taxopy_taxonomy_service.py` & `taxpasta-0.4.0/src/taxpasta/infrastructure/domain/service/taxopy_taxonomy_service.py`

 * *Files identical despite different names*

### Comparing `taxpasta-0.3.0/.gitignore` & `taxpasta-0.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `taxpasta-0.3.0/LICENSE` & `taxpasta-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `taxpasta-0.3.0/README.md` & `taxpasta-0.4.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,47 +1,43 @@
 # TAXPASTA
 
-|            |                                                                                                                                                                                                                                                                                                                                                                                                                                     |
-| ---------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
-| Package    | [![Latest PyPI Version](https://img.shields.io/pypi/v/taxpasta.svg)](https://pypi.org/project/taxpasta/) [![Supported Python Versions](https://img.shields.io/pypi/pyversions/taxpasta.svg)](https://pypi.org/project/taxpasta/) [![DOI](https://zenodo.org/badge/499589621.svg)](https://zenodo.org/badge/latestdoi/499589621)                                                                                                     |
-| Meta       | [![Apache-2.0](https://img.shields.io/pypi/l/taxpasta.svg)](LICENSE) [![Code of Conduct](https://img.shields.io/badge/Contributor%20Covenant-v2.0%20adopted-ff69b4.svg)](.github/CODE_OF_CONDUCT.md) [![Code Style Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)                                                                                                               |
-| Automation | [![GitHub Workflow](https://github.com/taxprofiler/taxpasta/workflows/CI-CD/badge.svg)](https://github.com/taxprofiler/taxpasta/workflows/CI-CD) [![Documentation](https://readthedocs.org/projects/taxpasta/badge/?version=latest)](https://taxpasta.readthedocs.io/en/latest/?badge=latest) [![Code Coverage](https://codecov.io/gh/taxprofiler/taxpasta/branch/dev/graph/badge.svg)](https://codecov.io/gh/taxprofiler/taxpasta) |
+|            |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
+| ---------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
+| Package    | [![Latest PyPI Version](https://img.shields.io/pypi/v/taxpasta.svg)](https://pypi.org/project/taxpasta/) [![Supported Python Versions](https://img.shields.io/pypi/pyversions/taxpasta.svg)](https://pypi.org/project/taxpasta/) [![DOI](https://zenodo.org/badge/499589621.svg)](https://zenodo.org/badge/latestdoi/499589621)                                                                                                                                                                                              |
+| Meta       | [![Project Status: Active – The project has reached a stable, usable state and is being actively developed.](https://www.repostatus.org/badges/latest/active.svg)](https://www.repostatus.org/#active) [![Apache-2.0](https://img.shields.io/pypi/l/taxpasta.svg)](LICENSE) [![Code of Conduct](https://img.shields.io/badge/Contributor%20Covenant-v2.0%20adopted-ff69b4.svg)](.github/CODE_OF_CONDUCT.md) [![Code Style Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black) |
+| Automation | [![GitHub Workflow](https://github.com/taxprofiler/taxpasta/workflows/CI-CD/badge.svg)](https://github.com/taxprofiler/taxpasta/workflows/CI-CD) [![Documentation](https://readthedocs.org/projects/taxpasta/badge/?version=latest)](https://taxpasta.readthedocs.io/en/latest/?badge=latest) [![Code Coverage](https://codecov.io/gh/taxprofiler/taxpasta/branch/dev/graph/badge.svg)](https://codecov.io/gh/taxprofiler/taxpasta)                                                                                          |
 
 _TAXonomic Profile Aggregation and STAndardisation_
 
 ## About
 
 The main purpose of taxpasta is to _standardise_ taxonomic profiles created by a
 range of bioinformatics tools. We call those tools taxonomic profilers. They
 each come with their own particular tabular output format. Across the profilers,
 relative abundances can be reported in read counts, fractions, or percentages,
 as well as any number of additional columns with extra information. We therefore
 decided to take [the lessons learnt](https://xkcd.com/927/) to heart and provide
 our own solution to deal with this pasticcio. With taxpasta you can ingest all
 of those formats and, at a minimum, output taxonomy identifiers and their
-integer counts.
-
-Taxpasta can not only standardise profiles but also _merge_ them across samples
-for the same profiler into a single table. In future, we also intend to offer
-methods for forming a _consensus_ for the same sample analyzed by different
-profilers.
+integer counts. Taxpasta can not only standardise profiles but also _merge_ them
+across samples for the _same_ profiler into a single table.
 
 ### Supported Taxonomic Profilers
 
 Taxpasta currently supports standardisation and generation of comparable
 taxonomic tables for:
 
 -   [Bracken](https://ccb.jhu.edu/software/bracken/)
 -   [Centrifuge](https://ccb.jhu.edu/software/centrifuge/)
 -   [DIAMOND](https://github.com/bbuchfink/diamond)
 -   [Kaiju](https://kaiju.binf.ku.dk/)
 -   [Kraken2](https://ccb.jhu.edu/software/kraken2/)
 -   [KrakenUniq](https://github.com/fbreitwieser/krakenuniq)
 -   [MEGAN6](http://www-ab.informatik.uni-tuebingen.de/software/megan6)/[MALT](https://uni-tuebingen.de/fakultaeten/mathematisch-naturwissenschaftliche-fakultaet/fachbereiche/informatik/lehrstuehle/algorithms-in-bioinformatics/software/malt/)
--   [MetaPhlAn](https://segatalab.cibio.unitn.it/tools/metaphlan/index.html)
+-   [MetaPhlAn](https://huttenhower.sph.harvard.edu/metaphlan)
 -   [mOTUs](https://motu-tool.org/)
 
 See [supported profilers](https://taxpasta.readthedocs.io/en/latest/supported_profilers/)
 for more information.
 
 ## Install
 
@@ -89,58 +85,64 @@
 
 ```shell
 taxpasta -h
 ```
 
 Taxpasta currently offers two commands corresponding to the main
 [use-cases](#about). You can find out more in the [commands'
-documentation](https://taxpasta.readthedocs.io/en/latest/commands/).
+documentation](https://taxpasta.readthedocs.io/en/latest/commands).
 
 ### Standardise
 
 Since the [supported profilers](#supported-taxonomic-profilers) all produce
 their own flavour of tabular output, a quick way to normalize such files, is to
 standardise them with taxpasta. You need to let taxpasta know what tool the file
 was created by. As an example, let's standardise a MetaPhlAn profile. (You can
 find an example file in our [test
-data](https://raw.githubusercontent.com/taxprofiler/taxpasta/dev/tests/data/metaphlan/MOCK_002_Illumina_Hiseq_3000_se_metaphlan3-db.metaphlan3_profile.txt).)
+data](https://raw.githubusercontent.com/taxprofiler/taxpasta/main/tests/data/metaphlan/MOCK_002_Illumina_Hiseq_3000_se_metaphlan3-db.metaphlan3_profile.txt).)
 
 ```shell
+curl -O https://raw.githubusercontent.com/taxprofiler/taxpasta/main/tests/data/metaphlan/MOCK_002_Illumina_Hiseq_3000_se_metaphlan3-db.metaphlan3_profile.txt
 taxpasta standardise -p metaphlan -o standardised.tsv MOCK_002_Illumina_Hiseq_3000_se_metaphlan3-db.metaphlan3_profile.txt
 ```
 
 With these minimal arguments, taxpasta produces a two column output consisting of
 
 | taxonomy_id | count |
 | ----------- | ----- |
 |             |       |
 
 You can count on the second column being integers :wink:. Having such a simple
 and tidy table should make your downstream analysis much smoother to start out
 with. Please have a look at the full [getting
-started](https://taxpasta.readthedocs.io/en/latest/tutorials/getting-started.md)
+started](https://taxpasta.readthedocs.io/en/latest/tutorials/getting-started)
 tutorial for a more thorough introduction.
 
 ### Merge
 
 Converting single tables is nice, but hopefully you have many shiny samples to
 analyze. The `taxpasta merge` command works similarly to `standardise` except
 that you provide multiple profiles as input. You can grab a few more 'MOCK' examples from
 our [test
-data](https://github.com/taxprofiler/taxpasta/tree/dev/tests/data/metaphlan) and
+data](https://github.com/taxprofiler/taxpasta/tree/main/tests/data/metaphlan) and
 try it out.
 
 ```shell
+LOCATION=https://raw.githubusercontent.com/taxprofiler/taxpasta/main/tests/data/metaphlan
+curl -O "${LOCATION}/MOCK_001_Illumina_Hiseq_3000_se_metaphlan3-db.metaphlan3_profile.txt"
+curl -O "${LOCATION}/MOCK_002_Illumina_Hiseq_3000_se_metaphlan3-db.metaphlan3_profile.txt"
+curl -O "${LOCATION}/MOCK_003_Illumina_Hiseq_3000_se_metaphlan3-db.metaphlan3_profile.txt"
+
 taxpasta merge -p metaphlan -o merged.tsv MOCK_*.metaphlan3_profile.txt
 ```
 
 The output of the `merge` command has one column for the taxonomic identifier and
 one more column for each input profile. Again, have a look at the full
 [getting
-started](https://taxpasta.readthedocs.io/en/latest/tutorials/getting-started.md)
+started](https://taxpasta.readthedocs.io/en/latest/tutorials/getting-started)
 tutorial for a more thorough introduction.
 
 ## Copyright
 
 -   Copyright © 2022, 2023, Moritz E. Beber, Maxime Borry, James A. Fellows
     Yates, and Sofia Stamouli.
 -   Free software distributed under the [Apache Software License
```

### Comparing `taxpasta-0.3.0/pyproject.toml` & `taxpasta-0.4.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -32,15 +32,25 @@
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Scientific/Engineering :: Bio-Informatics"
 ]
-keywords = ["taxonomic profile", "standardisation"]
+keywords = [
+    "bioinformatics",
+    "metagenomics",
+    "profiling",
+    "classification",
+    "taxonomy",
+    "metagenomic profile",
+    "taxonomic profile",
+    "standardisation",
+    "merging",
+]
 dynamic = ["version"]
 dependencies = [
     "depinfo ~=2.2",
     "numpy ~=1.20",
     "pandas ~=1.4",
     "pandera ~=0.14",
     "taxopy ~=0.10",
@@ -141,14 +151,15 @@
     "biom",
     "biom.table",
     "biom.util",
     "numpy",
     "odf",
     "openpyxl",
     "pandas",
+    "pandas.errors",
     "pandera",
     "pandera.errors",
     "pandera.typing",
     "pyarrow",
     "rich.logging",
     "taxopy",
     "taxopy.exceptions",
```

### Comparing `taxpasta-0.3.0/PKG-INFO` & `taxpasta-0.4.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: taxpasta
-Version: 0.3.0
+Version: 0.4.0
 Summary: TAXonomic Profile Aggregation and STAndardisation
 Project-URL: Homepage, https://github.com/taxprofiler/taxpasta
 Project-URL: Documentation, https://taxpasta.readthedocs.io
 Project-URL: Source Code, https://github.com/taxprofiler/taxpasta
 Project-URL: Bug Tracker, https://github.com/taxprofiler/taxpasta/issues
 Project-URL: Download, https://pypi.org/project/taxpasta/#files
 Author-email: "Moritz E. Beber" <moritz.beber@posteo.de>, Maxime Borry <maxime_borry@eva.mpg.de>, "James A. Fellows Yates" <jfy133@gmail.com>, Sofia Stamouli <sofia.stamouli@scilifelab.se>
 License-Expression: Apache-2.0
 License-File: LICENSE
-Keywords: standardisation,taxonomic profile
+Keywords: bioinformatics,classification,merging,metagenomic profile,metagenomics,profiling,standardisation,taxonomic profile,taxonomy
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
@@ -57,52 +57,48 @@
 Requires-Dist: rich; extra == 'rich'
 Provides-Extra: xlsx
 Requires-Dist: openpyxl; extra == 'xlsx'
 Description-Content-Type: text/markdown
 
 # TAXPASTA
 
-|            |                                                                                                                                                                                                                                                                                                                                                                                                                                     |
-| ---------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
-| Package    | [![Latest PyPI Version](https://img.shields.io/pypi/v/taxpasta.svg)](https://pypi.org/project/taxpasta/) [![Supported Python Versions](https://img.shields.io/pypi/pyversions/taxpasta.svg)](https://pypi.org/project/taxpasta/) [![DOI](https://zenodo.org/badge/499589621.svg)](https://zenodo.org/badge/latestdoi/499589621)                                                                                                     |
-| Meta       | [![Apache-2.0](https://img.shields.io/pypi/l/taxpasta.svg)](LICENSE) [![Code of Conduct](https://img.shields.io/badge/Contributor%20Covenant-v2.0%20adopted-ff69b4.svg)](.github/CODE_OF_CONDUCT.md) [![Code Style Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)                                                                                                               |
-| Automation | [![GitHub Workflow](https://github.com/taxprofiler/taxpasta/workflows/CI-CD/badge.svg)](https://github.com/taxprofiler/taxpasta/workflows/CI-CD) [![Documentation](https://readthedocs.org/projects/taxpasta/badge/?version=latest)](https://taxpasta.readthedocs.io/en/latest/?badge=latest) [![Code Coverage](https://codecov.io/gh/taxprofiler/taxpasta/branch/dev/graph/badge.svg)](https://codecov.io/gh/taxprofiler/taxpasta) |
+|            |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
+| ---------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
+| Package    | [![Latest PyPI Version](https://img.shields.io/pypi/v/taxpasta.svg)](https://pypi.org/project/taxpasta/) [![Supported Python Versions](https://img.shields.io/pypi/pyversions/taxpasta.svg)](https://pypi.org/project/taxpasta/) [![DOI](https://zenodo.org/badge/499589621.svg)](https://zenodo.org/badge/latestdoi/499589621)                                                                                                                                                                                              |
+| Meta       | [![Project Status: Active – The project has reached a stable, usable state and is being actively developed.](https://www.repostatus.org/badges/latest/active.svg)](https://www.repostatus.org/#active) [![Apache-2.0](https://img.shields.io/pypi/l/taxpasta.svg)](LICENSE) [![Code of Conduct](https://img.shields.io/badge/Contributor%20Covenant-v2.0%20adopted-ff69b4.svg)](.github/CODE_OF_CONDUCT.md) [![Code Style Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black) |
+| Automation | [![GitHub Workflow](https://github.com/taxprofiler/taxpasta/workflows/CI-CD/badge.svg)](https://github.com/taxprofiler/taxpasta/workflows/CI-CD) [![Documentation](https://readthedocs.org/projects/taxpasta/badge/?version=latest)](https://taxpasta.readthedocs.io/en/latest/?badge=latest) [![Code Coverage](https://codecov.io/gh/taxprofiler/taxpasta/branch/dev/graph/badge.svg)](https://codecov.io/gh/taxprofiler/taxpasta)                                                                                          |
 
 _TAXonomic Profile Aggregation and STAndardisation_
 
 ## About
 
 The main purpose of taxpasta is to _standardise_ taxonomic profiles created by a
 range of bioinformatics tools. We call those tools taxonomic profilers. They
 each come with their own particular tabular output format. Across the profilers,
 relative abundances can be reported in read counts, fractions, or percentages,
 as well as any number of additional columns with extra information. We therefore
 decided to take [the lessons learnt](https://xkcd.com/927/) to heart and provide
 our own solution to deal with this pasticcio. With taxpasta you can ingest all
 of those formats and, at a minimum, output taxonomy identifiers and their
-integer counts.
-
-Taxpasta can not only standardise profiles but also _merge_ them across samples
-for the same profiler into a single table. In future, we also intend to offer
-methods for forming a _consensus_ for the same sample analyzed by different
-profilers.
+integer counts. Taxpasta can not only standardise profiles but also _merge_ them
+across samples for the _same_ profiler into a single table.
 
 ### Supported Taxonomic Profilers
 
 Taxpasta currently supports standardisation and generation of comparable
 taxonomic tables for:
 
 -   [Bracken](https://ccb.jhu.edu/software/bracken/)
 -   [Centrifuge](https://ccb.jhu.edu/software/centrifuge/)
 -   [DIAMOND](https://github.com/bbuchfink/diamond)
 -   [Kaiju](https://kaiju.binf.ku.dk/)
 -   [Kraken2](https://ccb.jhu.edu/software/kraken2/)
 -   [KrakenUniq](https://github.com/fbreitwieser/krakenuniq)
 -   [MEGAN6](http://www-ab.informatik.uni-tuebingen.de/software/megan6)/[MALT](https://uni-tuebingen.de/fakultaeten/mathematisch-naturwissenschaftliche-fakultaet/fachbereiche/informatik/lehrstuehle/algorithms-in-bioinformatics/software/malt/)
--   [MetaPhlAn](https://segatalab.cibio.unitn.it/tools/metaphlan/index.html)
+-   [MetaPhlAn](https://huttenhower.sph.harvard.edu/metaphlan)
 -   [mOTUs](https://motu-tool.org/)
 
 See [supported profilers](https://taxpasta.readthedocs.io/en/latest/supported_profilers/)
 for more information.
 
 ## Install
 
@@ -150,58 +146,64 @@
 
 ```shell
 taxpasta -h
 ```
 
 Taxpasta currently offers two commands corresponding to the main
 [use-cases](#about). You can find out more in the [commands'
-documentation](https://taxpasta.readthedocs.io/en/latest/commands/).
+documentation](https://taxpasta.readthedocs.io/en/latest/commands).
 
 ### Standardise
 
 Since the [supported profilers](#supported-taxonomic-profilers) all produce
 their own flavour of tabular output, a quick way to normalize such files, is to
 standardise them with taxpasta. You need to let taxpasta know what tool the file
 was created by. As an example, let's standardise a MetaPhlAn profile. (You can
 find an example file in our [test
-data](https://raw.githubusercontent.com/taxprofiler/taxpasta/dev/tests/data/metaphlan/MOCK_002_Illumina_Hiseq_3000_se_metaphlan3-db.metaphlan3_profile.txt).)
+data](https://raw.githubusercontent.com/taxprofiler/taxpasta/main/tests/data/metaphlan/MOCK_002_Illumina_Hiseq_3000_se_metaphlan3-db.metaphlan3_profile.txt).)
 
 ```shell
+curl -O https://raw.githubusercontent.com/taxprofiler/taxpasta/main/tests/data/metaphlan/MOCK_002_Illumina_Hiseq_3000_se_metaphlan3-db.metaphlan3_profile.txt
 taxpasta standardise -p metaphlan -o standardised.tsv MOCK_002_Illumina_Hiseq_3000_se_metaphlan3-db.metaphlan3_profile.txt
 ```
 
 With these minimal arguments, taxpasta produces a two column output consisting of
 
 | taxonomy_id | count |
 | ----------- | ----- |
 |             |       |
 
 You can count on the second column being integers :wink:. Having such a simple
 and tidy table should make your downstream analysis much smoother to start out
 with. Please have a look at the full [getting
-started](https://taxpasta.readthedocs.io/en/latest/tutorials/getting-started.md)
+started](https://taxpasta.readthedocs.io/en/latest/tutorials/getting-started)
 tutorial for a more thorough introduction.
 
 ### Merge
 
 Converting single tables is nice, but hopefully you have many shiny samples to
 analyze. The `taxpasta merge` command works similarly to `standardise` except
 that you provide multiple profiles as input. You can grab a few more 'MOCK' examples from
 our [test
-data](https://github.com/taxprofiler/taxpasta/tree/dev/tests/data/metaphlan) and
+data](https://github.com/taxprofiler/taxpasta/tree/main/tests/data/metaphlan) and
 try it out.
 
 ```shell
+LOCATION=https://raw.githubusercontent.com/taxprofiler/taxpasta/main/tests/data/metaphlan
+curl -O "${LOCATION}/MOCK_001_Illumina_Hiseq_3000_se_metaphlan3-db.metaphlan3_profile.txt"
+curl -O "${LOCATION}/MOCK_002_Illumina_Hiseq_3000_se_metaphlan3-db.metaphlan3_profile.txt"
+curl -O "${LOCATION}/MOCK_003_Illumina_Hiseq_3000_se_metaphlan3-db.metaphlan3_profile.txt"
+
 taxpasta merge -p metaphlan -o merged.tsv MOCK_*.metaphlan3_profile.txt
 ```
 
 The output of the `merge` command has one column for the taxonomic identifier and
 one more column for each input profile. Again, have a look at the full
 [getting
-started](https://taxpasta.readthedocs.io/en/latest/tutorials/getting-started.md)
+started](https://taxpasta.readthedocs.io/en/latest/tutorials/getting-started)
 tutorial for a more thorough introduction.
 
 ## Copyright
 
 -   Copyright © 2022, 2023, Moritz E. Beber, Maxime Borry, James A. Fellows
     Yates, and Sofia Stamouli.
 -   Free software distributed under the [Apache Software License
```

