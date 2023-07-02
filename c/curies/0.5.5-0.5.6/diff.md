# Comparing `tmp/curies-0.5.5.tar.gz` & `tmp/curies-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "curies-0.5.5.tar", last modified: Mon May 15 10:40:42 2023, max compression
+gzip compressed data, was "curies-0.5.6.tar", last modified: Sun Jul  2 15:23:44 2023, max compression
```

## Comparing `curies-0.5.5.tar` & `curies-0.5.6.tar`

### file list

```diff
@@ -1,63 +1,62 @@
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-05-15 10:40:42.855506 curies-0.5.5/
--rw-r--r--   0 cthoyt     (501) staff       (20)     1076 2022-07-31 23:04:00.000000 curies-0.5.5/LICENSE
--rw-r--r--   0 cthoyt     (501) staff       (20)      394 2023-04-28 13:05:54.000000 curies-0.5.5/MANIFEST.in
--rw-r--r--   0 cthoyt     (501) staff       (20)    11827 2023-05-15 10:40:42.855681 curies-0.5.5/PKG-INFO
--rw-r--r--   0 cthoyt     (501) staff       (20)    10308 2023-05-05 11:46:12.000000 curies-0.5.5/README.md
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-05-15 10:40:42.823165 curies-0.5.5/docs/
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-05-15 10:40:42.827618 curies-0.5.5/docs/source/
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-05-15 10:40:42.839925 curies-0.5.5/docs/source/api/
--rw-r--r--   0 cthoyt     (501) staff       (20)     1864 2023-04-13 07:20:08.000000 curies-0.5.5/docs/source/api/curies.Converter.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      101 2023-04-13 07:20:08.000000 curies-0.5.5/docs/source/api/curies.DuplicatePrefixes.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      110 2023-04-13 07:20:08.000000 curies-0.5.5/docs/source/api/curies.DuplicateURIPrefixes.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      107 2023-04-13 07:20:08.000000 curies-0.5.5/docs/source/api/curies.DuplicateValueError.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)       86 2023-04-13 07:20:08.000000 curies-0.5.5/docs/source/api/curies.Record.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)       64 2023-04-13 07:20:08.000000 curies-0.5.5/docs/source/api/curies.chain.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      124 2023-04-13 07:20:08.000000 curies-0.5.5/docs/source/api/curies.get_bioregistry_converter.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)       94 2023-04-13 07:20:08.000000 curies-0.5.5/docs/source/api/curies.get_fastapi_app.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      103 2023-04-13 07:20:08.000000 curies-0.5.5/docs/source/api/curies.get_fastapi_router.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)       88 2023-04-13 07:20:08.000000 curies-0.5.5/docs/source/api/curies.get_flask_app.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      106 2023-04-13 07:20:08.000000 curies-0.5.5/docs/source/api/curies.get_flask_blueprint.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)       97 2023-04-13 07:20:08.000000 curies-0.5.5/docs/source/api/curies.get_go_converter.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      112 2023-04-13 07:20:08.000000 curies-0.5.5/docs/source/api/curies.get_monarch_converter.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      100 2023-04-13 07:20:08.000000 curies-0.5.5/docs/source/api/curies.get_obo_converter.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      130 2023-04-13 07:20:08.000000 curies-0.5.5/docs/source/api/curies.get_prefixcommons_converter.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)       82 2023-04-13 07:20:08.000000 curies-0.5.5/docs/source/api/curies.get_version.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      141 2023-04-13 07:20:08.000000 curies-0.5.5/docs/source/api/curies.mapping_service.MappingServiceGraph.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      332 2023-04-13 07:20:08.000000 curies-0.5.5/docs/source/api/curies.mapping_service.MappingServiceSPARQLProcessor.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      134 2023-04-13 07:20:08.000000 curies-0.5.5/docs/source/api/curies.mapping_service.get_fastapi_mapping_app.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      119 2023-04-13 07:20:08.000000 curies-0.5.5/docs/source/api/curies.mapping_service.get_fastapi_router.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      128 2023-04-13 07:20:08.000000 curies-0.5.5/docs/source/api/curies.mapping_service.get_flask_mapping_app.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      146 2023-04-13 07:20:08.000000 curies-0.5.5/docs/source/api/curies.mapping_service.get_flask_mapping_blueprint.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)     7469 2023-05-15 10:40:41.000000 curies-0.5.5/docs/source/conf.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     2538 2023-03-10 11:58:39.000000 curies-0.5.5/docs/source/index.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      385 2022-12-09 17:27:17.000000 curies-0.5.5/pyproject.toml
--rw-r--r--   0 cthoyt     (501) staff       (20)     2678 2023-05-15 10:40:42.856773 curies-0.5.5/setup.cfg
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-05-15 10:40:42.823737 curies-0.5.5/src/
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-05-15 10:40:42.846252 curies-0.5.5/src/curies/
--rw-r--r--   0 cthoyt     (501) staff       (20)     1015 2023-05-15 10:11:51.000000 curies-0.5.5/src/curies/__init__.py
--rw-r--r--   0 cthoyt     (501) staff       (20)      146 2023-02-21 22:19:21.000000 curies-0.5.5/src/curies/__main__.py
--rw-r--r--   0 cthoyt     (501) staff       (20)    44040 2023-05-15 10:23:41.000000 curies-0.5.5/src/curies/api.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     5065 2023-04-13 07:17:14.000000 curies-0.5.5/src/curies/cli.py
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-05-15 10:40:42.851173 curies-0.5.5/src/curies/mapping_service/
--rw-r--r--   0 cthoyt     (501) staff       (20)     4478 2023-04-13 07:57:38.000000 curies-0.5.5/src/curies/mapping_service/__init__.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     8224 2023-05-05 11:46:12.000000 curies-0.5.5/src/curies/mapping_service/api.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     3343 2023-03-26 20:29:12.000000 curies-0.5.5/src/curies/mapping_service/rdflib_custom.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     4637 2023-05-05 11:46:12.000000 curies-0.5.5/src/curies/mapping_service/utils.py
--rw-r--r--   0 cthoyt     (501) staff       (20)        1 2022-07-31 23:04:01.000000 curies-0.5.5/src/curies/py.typed
--rw-r--r--   0 cthoyt     (501) staff       (20)     2033 2023-03-04 12:32:17.000000 curies-0.5.5/src/curies/sources.py
--rw-r--r--   0 cthoyt     (501) staff       (20)      255 2023-05-15 10:40:41.000000 curies-0.5.5/src/curies/version.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     9666 2023-04-13 06:43:24.000000 curies-0.5.5/src/curies/web.py
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-05-15 10:40:42.848960 curies-0.5.5/src/curies.egg-info/
--rw-r--r--   0 cthoyt     (501) staff       (20)    11827 2023-05-15 10:40:42.000000 curies-0.5.5/src/curies.egg-info/PKG-INFO
--rw-r--r--   0 cthoyt     (501) staff       (20)     1853 2023-05-15 10:40:42.000000 curies-0.5.5/src/curies.egg-info/SOURCES.txt
--rw-r--r--   0 cthoyt     (501) staff       (20)        1 2023-05-15 10:40:42.000000 curies-0.5.5/src/curies.egg-info/dependency_links.txt
--rw-r--r--   0 cthoyt     (501) staff       (20)        1 2022-07-31 23:04:24.000000 curies-0.5.5/src/curies.egg-info/not-zip-safe
--rw-r--r--   0 cthoyt     (501) staff       (20)      282 2023-05-15 10:40:42.000000 curies-0.5.5/src/curies.egg-info/requires.txt
--rw-r--r--   0 cthoyt     (501) staff       (20)        7 2023-05-15 10:40:42.000000 curies-0.5.5/src/curies.egg-info/top_level.txt
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-05-15 10:40:42.854958 curies-0.5.5/tests/
--rw-r--r--   0 cthoyt     (501) staff       (20)       56 2022-07-31 23:04:00.000000 curies-0.5.5/tests/__init__.py
--rw-r--r--   0 cthoyt     (501) staff       (20)        0 2023-03-23 13:16:42.000000 curies-0.5.5/tests/rules.log
--rw-r--r--   0 cthoyt     (501) staff       (20)    18891 2023-05-15 10:20:25.000000 curies-0.5.5/tests/test_api.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     5198 2023-04-13 10:20:39.000000 curies-0.5.5/tests/test_federated_sparql.py
--rw-r--r--   0 cthoyt     (501) staff       (20)    13426 2023-04-13 07:57:38.000000 curies-0.5.5/tests/test_mapping_service.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     3271 2023-04-13 06:37:08.000000 curies-0.5.5/tests/test_web.py
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-07-02 15:23:44.821307 curies-0.5.6/
+-rw-r--r--   0 cthoyt     (501) staff       (20)     1076 2022-07-31 23:04:00.000000 curies-0.5.6/LICENSE
+-rw-r--r--   0 cthoyt     (501) staff       (20)      394 2023-04-28 13:05:54.000000 curies-0.5.6/MANIFEST.in
+-rw-r--r--   0 cthoyt     (501) staff       (20)    11777 2023-07-02 15:23:44.821477 curies-0.5.6/PKG-INFO
+-rw-r--r--   0 cthoyt     (501) staff       (20)    10308 2023-05-05 11:46:12.000000 curies-0.5.6/README.md
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-07-02 15:23:44.793667 curies-0.5.6/docs/
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-07-02 15:23:44.797014 curies-0.5.6/docs/source/
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-07-02 15:23:44.808138 curies-0.5.6/docs/source/api/
+-rw-r--r--   0 cthoyt     (501) staff       (20)     1864 2023-04-13 07:20:08.000000 curies-0.5.6/docs/source/api/curies.Converter.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      101 2023-04-13 07:20:08.000000 curies-0.5.6/docs/source/api/curies.DuplicatePrefixes.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      110 2023-04-13 07:20:08.000000 curies-0.5.6/docs/source/api/curies.DuplicateURIPrefixes.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      107 2023-04-13 07:20:08.000000 curies-0.5.6/docs/source/api/curies.DuplicateValueError.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)       86 2023-04-13 07:20:08.000000 curies-0.5.6/docs/source/api/curies.Record.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)       64 2023-04-13 07:20:08.000000 curies-0.5.6/docs/source/api/curies.chain.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      124 2023-04-13 07:20:08.000000 curies-0.5.6/docs/source/api/curies.get_bioregistry_converter.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)       94 2023-04-13 07:20:08.000000 curies-0.5.6/docs/source/api/curies.get_fastapi_app.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      103 2023-04-13 07:20:08.000000 curies-0.5.6/docs/source/api/curies.get_fastapi_router.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)       88 2023-04-13 07:20:08.000000 curies-0.5.6/docs/source/api/curies.get_flask_app.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      106 2023-04-13 07:20:08.000000 curies-0.5.6/docs/source/api/curies.get_flask_blueprint.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)       97 2023-04-13 07:20:08.000000 curies-0.5.6/docs/source/api/curies.get_go_converter.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      112 2023-04-13 07:20:08.000000 curies-0.5.6/docs/source/api/curies.get_monarch_converter.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      100 2023-04-13 07:20:08.000000 curies-0.5.6/docs/source/api/curies.get_obo_converter.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      130 2023-04-13 07:20:08.000000 curies-0.5.6/docs/source/api/curies.get_prefixcommons_converter.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)       82 2023-04-13 07:20:08.000000 curies-0.5.6/docs/source/api/curies.get_version.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      141 2023-04-13 07:20:08.000000 curies-0.5.6/docs/source/api/curies.mapping_service.MappingServiceGraph.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      332 2023-04-13 07:20:08.000000 curies-0.5.6/docs/source/api/curies.mapping_service.MappingServiceSPARQLProcessor.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      134 2023-04-13 07:20:08.000000 curies-0.5.6/docs/source/api/curies.mapping_service.get_fastapi_mapping_app.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      119 2023-04-13 07:20:08.000000 curies-0.5.6/docs/source/api/curies.mapping_service.get_fastapi_router.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      128 2023-04-13 07:20:08.000000 curies-0.5.6/docs/source/api/curies.mapping_service.get_flask_mapping_app.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      146 2023-04-13 07:20:08.000000 curies-0.5.6/docs/source/api/curies.mapping_service.get_flask_mapping_blueprint.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)     7469 2023-07-02 15:23:43.000000 curies-0.5.6/docs/source/conf.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     2538 2023-03-10 11:58:39.000000 curies-0.5.6/docs/source/index.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      377 2023-07-02 15:23:36.000000 curies-0.5.6/pyproject.toml
+-rw-r--r--   0 cthoyt     (501) staff       (20)     2647 2023-07-02 15:23:44.822775 curies-0.5.6/setup.cfg
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-07-02 15:23:44.794270 curies-0.5.6/src/
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-07-02 15:23:44.813037 curies-0.5.6/src/curies/
+-rw-r--r--   0 cthoyt     (501) staff       (20)     1015 2023-05-15 10:11:51.000000 curies-0.5.6/src/curies/__init__.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)      146 2023-02-21 22:19:21.000000 curies-0.5.6/src/curies/__main__.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)    44040 2023-07-02 08:04:48.000000 curies-0.5.6/src/curies/api.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     5065 2023-04-13 07:17:14.000000 curies-0.5.6/src/curies/cli.py
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-07-02 15:23:44.817556 curies-0.5.6/src/curies/mapping_service/
+-rw-r--r--   0 cthoyt     (501) staff       (20)     4478 2023-04-13 07:57:38.000000 curies-0.5.6/src/curies/mapping_service/__init__.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     8224 2023-05-05 11:46:12.000000 curies-0.5.6/src/curies/mapping_service/api.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     3343 2023-03-26 20:29:12.000000 curies-0.5.6/src/curies/mapping_service/rdflib_custom.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     4637 2023-05-05 11:46:12.000000 curies-0.5.6/src/curies/mapping_service/utils.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)        1 2022-07-31 23:04:01.000000 curies-0.5.6/src/curies/py.typed
+-rw-r--r--   0 cthoyt     (501) staff       (20)     2033 2023-03-04 12:32:17.000000 curies-0.5.6/src/curies/sources.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)      255 2023-07-02 15:23:43.000000 curies-0.5.6/src/curies/version.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     9669 2023-07-02 15:23:36.000000 curies-0.5.6/src/curies/web.py
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-07-02 15:23:44.815203 curies-0.5.6/src/curies.egg-info/
+-rw-r--r--   0 cthoyt     (501) staff       (20)    11777 2023-07-02 15:23:44.000000 curies-0.5.6/src/curies.egg-info/PKG-INFO
+-rw-r--r--   0 cthoyt     (501) staff       (20)     1837 2023-07-02 15:23:44.000000 curies-0.5.6/src/curies.egg-info/SOURCES.txt
+-rw-r--r--   0 cthoyt     (501) staff       (20)        1 2023-07-02 15:23:44.000000 curies-0.5.6/src/curies.egg-info/dependency_links.txt
+-rw-r--r--   0 cthoyt     (501) staff       (20)        1 2022-07-31 23:04:24.000000 curies-0.5.6/src/curies.egg-info/not-zip-safe
+-rw-r--r--   0 cthoyt     (501) staff       (20)      290 2023-07-02 15:23:44.000000 curies-0.5.6/src/curies.egg-info/requires.txt
+-rw-r--r--   0 cthoyt     (501) staff       (20)        7 2023-07-02 15:23:44.000000 curies-0.5.6/src/curies.egg-info/top_level.txt
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-07-02 15:23:44.821037 curies-0.5.6/tests/
+-rw-r--r--   0 cthoyt     (501) staff       (20)       56 2022-07-31 23:04:00.000000 curies-0.5.6/tests/__init__.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)    18891 2023-05-15 10:20:25.000000 curies-0.5.6/tests/test_api.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     5198 2023-04-13 10:20:39.000000 curies-0.5.6/tests/test_federated_sparql.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)    13426 2023-04-13 07:57:38.000000 curies-0.5.6/tests/test_mapping_service.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     3273 2023-07-02 15:23:36.000000 curies-0.5.6/tests/test_web.py
```

### Comparing `curies-0.5.5/LICENSE` & `curies-0.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `curies-0.5.5/PKG-INFO` & `curies-0.5.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: curies
-Version: 0.5.5
+Version: 0.5.6
 Summary: Idiomatic conversion between URIs and compact URIs (CURIEs).
 Home-page: https://github.com/cthoyt/curies
 Download-URL: https://github.com/cthoyt/curies/releases
 Author: Charles Tapley Hoyt
 Author-email: cthoyt@gmail.com
 Maintainer: Charles Tapley Hoyt
 Maintainer-email: cthoyt@gmail.com
@@ -17,21 +17,20 @@
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Framework :: Pytest
 Classifier: Framework :: tox
 Classifier: Framework :: Sphinx
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 Provides-Extra: pandas
 Provides-Extra: bioregistry
 Provides-Extra: flask
 Provides-Extra: fastapi
 Provides-Extra: rdflib
```

#### html2text {}

```diff
@@ -1,27 +1,27 @@
-Metadata-Version: 2.1 Name: curies Version: 0.5.5 Summary: Idiomatic conversion
+Metadata-Version: 2.1 Name: curies Version: 0.5.6 Summary: Idiomatic conversion
 between URIs and compact URIs (CURIEs). Home-page: https://github.com/cthoyt/
 curies Download-URL: https://github.com/cthoyt/curies/releases Author: Charles
 Tapley Hoyt Author-email: cthoyt@gmail.com Maintainer: Charles Tapley Hoyt
 Maintainer-email: cthoyt@gmail.com License: MIT Project-URL: Bug Tracker,
 https://github.com/cthoyt/curies/issues Project-URL: Source Code, https://
 github.com/cthoyt/curies Keywords: snekpack,cookiecutter,semantic web,compact
 uniform resource identifiers,uniform resource identifiers,curies Classifier:
 Development Status :: 1 - Planning Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: MIT License Classifier: Operating System :: OS Independent Classifier:
 Framework :: Pytest Classifier: Framework :: tox Classifier: Framework ::
 Sphinx Classifier: Programming Language :: Python Classifier: Programming
-Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
-Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3 :: Only Requires-Python: >=3.7
-Description-Content-Type: text/markdown Provides-Extra: tests Provides-Extra:
-pandas Provides-Extra: bioregistry Provides-Extra: flask Provides-Extra:
-fastapi Provides-Extra: rdflib Provides-Extra: docs License-File: LICENSE
+Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3 ::
+Only Requires-Python: >=3.8 Description-Content-Type: text/markdown Provides-
+Extra: tests Provides-Extra: pandas Provides-Extra: bioregistry Provides-Extra:
+flask Provides-Extra: fastapi Provides-Extra: rdflib Provides-Extra: docs
+License-File: LICENSE
                              ****** curies ******
 [Tests] [PyPI] [PyPI_-_Python_Version] [PyPI_-_License] [Documentation_Status]
   [Codecov_status] [Cookiecutter_template_from_@cthoyt] [Code_style:_black]
                          [Contributor_Covenant] [DOI]
 Idiomatic conversion between URIs and compact URIs (CURIEs). ```python from
 curies import Converter converter = Converter.from_prefix_map({ "CHEBI": "http:
 //purl.obolibrary.org/obo/CHEBI_", "MONDO": "http://purl.obolibrary.org/obo/
```

### Comparing `curies-0.5.5/README.md` & `curies-0.5.6/README.md`

 * *Files identical despite different names*

### Comparing `curies-0.5.5/docs/source/api/curies.Converter.rst` & `curies-0.5.6/docs/source/api/curies.Converter.rst`

 * *Files identical despite different names*

### Comparing `curies-0.5.5/docs/source/conf.py` & `curies-0.5.6/docs/source/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 # -- Project information -----------------------------------------------------
 
 project = "curies"
 copyright = f"{date.today().year}, Charles Tapley Hoyt"
 author = "Charles Tapley Hoyt"
 
 # The full version, including alpha/beta/rc tags.
-release = "0.5.5"
+release = "0.5.6"
 
 # The short X.Y version.
 parsed_version = re.match(
     "(?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(?:-(?P<release>[0-9A-Za-z-]+(?:\.[0-9A-Za-z-]+)*))?(?:\+(?P<build>[0-9A-Za-z-]+(?:\.[0-9A-Za-z-]+)*))?",
     release,
 )
 version = parsed_version.expand("\g<major>.\g<minor>.\g<patch>")
```

### Comparing `curies-0.5.5/docs/source/index.rst` & `curies-0.5.6/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `curies-0.5.5/setup.cfg` & `curies-0.5.6/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = curies
-version = 0.5.5
+version = 0.5.6
 description = Idiomatic conversion between URIs and compact URIs (CURIEs).
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/cthoyt/curies
 download_url = https://github.com/cthoyt/curies/releases
 project_urls = 
 	Bug Tracker = https://github.com/cthoyt/curies/issues
@@ -22,15 +22,14 @@
 	Intended Audience :: Developers
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 	Framework :: Pytest
 	Framework :: tox
 	Framework :: Sphinx
 	Programming Language :: Python
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 	Programming Language :: Python :: 3 :: Only
 keywords = 
 	snekpack
@@ -39,19 +38,19 @@
 	compact uniform resource identifiers
 	uniform resource identifiers
 	curies
 
 [options]
 install_requires = 
 	pytrie
-	pydantic
+	pydantic<2.0
 	requests
 zip_safe = false
 include_package_data = True
-python_requires = >=3.7
+python_requires = >=3.8
 packages = find:
 package_dir = 
 	= src
 
 [options.packages.find]
 where = src
 
@@ -71,15 +70,15 @@
 	python-multipart
 	httpx
 	defusedxml
 	uvicorn
 rdflib = 
 	rdflib
 docs = 
-	sphinx
+	sphinx<7.0
 	sphinx-rtd-theme
 	sphinx-autodoc-typehints
 	sphinx_automodapi
 
 [doc8]
 max-line-length = 120
```

### Comparing `curies-0.5.5/src/curies/__init__.py` & `curies-0.5.6/src/curies/__init__.py`

 * *Files identical despite different names*

### Comparing `curies-0.5.5/src/curies/api.py` & `curies-0.5.6/src/curies/api.py`

 * *Files identical despite different names*

### Comparing `curies-0.5.5/src/curies/cli.py` & `curies-0.5.6/src/curies/cli.py`

 * *Files identical despite different names*

### Comparing `curies-0.5.5/src/curies/mapping_service/__init__.py` & `curies-0.5.6/src/curies/mapping_service/__init__.py`

 * *Files identical despite different names*

### Comparing `curies-0.5.5/src/curies/mapping_service/api.py` & `curies-0.5.6/src/curies/mapping_service/api.py`

 * *Files identical despite different names*

### Comparing `curies-0.5.5/src/curies/mapping_service/rdflib_custom.py` & `curies-0.5.6/src/curies/mapping_service/rdflib_custom.py`

 * *Files identical despite different names*

### Comparing `curies-0.5.5/src/curies/mapping_service/utils.py` & `curies-0.5.6/src/curies/mapping_service/utils.py`

 * *Files identical despite different names*

### Comparing `curies-0.5.5/src/curies/sources.py` & `curies-0.5.6/src/curies/sources.py`

 * *Files identical despite different names*

### Comparing `curies-0.5.5/src/curies/web.py` & `curies-0.5.6/src/curies/web.py`

 * *Files 1% similar despite different names*

```diff
@@ -202,15 +202,15 @@
     api_router = APIRouter(**kwargs)
 
     @api_router.get(f"/{{prefix}}{converter.delimiter}{{identifier}}")  # type:ignore
     def resolve(
         prefix: str = Path(  # noqa:B008
             title="Prefix",
             description="The Bioregistry prefix corresponding to an identifier resource.",
-            example="doid",
+            examples=["doid"],
         ),
         identifier: str = Path(  # noqa:B008
             title="Local Unique Identifier",
             description="The local unique identifier in the identifier resource referenced by the prefix.",
         ),
     ) -> RedirectResponse:
         """Resolve a CURIE."""
```

### Comparing `curies-0.5.5/src/curies.egg-info/PKG-INFO` & `curies-0.5.6/src/curies.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: curies
-Version: 0.5.5
+Version: 0.5.6
 Summary: Idiomatic conversion between URIs and compact URIs (CURIEs).
 Home-page: https://github.com/cthoyt/curies
 Download-URL: https://github.com/cthoyt/curies/releases
 Author: Charles Tapley Hoyt
 Author-email: cthoyt@gmail.com
 Maintainer: Charles Tapley Hoyt
 Maintainer-email: cthoyt@gmail.com
@@ -17,21 +17,20 @@
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Framework :: Pytest
 Classifier: Framework :: tox
 Classifier: Framework :: Sphinx
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 Provides-Extra: pandas
 Provides-Extra: bioregistry
 Provides-Extra: flask
 Provides-Extra: fastapi
 Provides-Extra: rdflib
```

#### html2text {}

```diff
@@ -1,27 +1,27 @@
-Metadata-Version: 2.1 Name: curies Version: 0.5.5 Summary: Idiomatic conversion
+Metadata-Version: 2.1 Name: curies Version: 0.5.6 Summary: Idiomatic conversion
 between URIs and compact URIs (CURIEs). Home-page: https://github.com/cthoyt/
 curies Download-URL: https://github.com/cthoyt/curies/releases Author: Charles
 Tapley Hoyt Author-email: cthoyt@gmail.com Maintainer: Charles Tapley Hoyt
 Maintainer-email: cthoyt@gmail.com License: MIT Project-URL: Bug Tracker,
 https://github.com/cthoyt/curies/issues Project-URL: Source Code, https://
 github.com/cthoyt/curies Keywords: snekpack,cookiecutter,semantic web,compact
 uniform resource identifiers,uniform resource identifiers,curies Classifier:
 Development Status :: 1 - Planning Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: MIT License Classifier: Operating System :: OS Independent Classifier:
 Framework :: Pytest Classifier: Framework :: tox Classifier: Framework ::
 Sphinx Classifier: Programming Language :: Python Classifier: Programming
-Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
-Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3 :: Only Requires-Python: >=3.7
-Description-Content-Type: text/markdown Provides-Extra: tests Provides-Extra:
-pandas Provides-Extra: bioregistry Provides-Extra: flask Provides-Extra:
-fastapi Provides-Extra: rdflib Provides-Extra: docs License-File: LICENSE
+Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3 ::
+Only Requires-Python: >=3.8 Description-Content-Type: text/markdown Provides-
+Extra: tests Provides-Extra: pandas Provides-Extra: bioregistry Provides-Extra:
+flask Provides-Extra: fastapi Provides-Extra: rdflib Provides-Extra: docs
+License-File: LICENSE
                              ****** curies ******
 [Tests] [PyPI] [PyPI_-_Python_Version] [PyPI_-_License] [Documentation_Status]
   [Codecov_status] [Cookiecutter_template_from_@cthoyt] [Code_style:_black]
                          [Contributor_Covenant] [DOI]
 Idiomatic conversion between URIs and compact URIs (CURIEs). ```python from
 curies import Converter converter = Converter.from_prefix_map({ "CHEBI": "http:
 //purl.obolibrary.org/obo/CHEBI_", "MONDO": "http://purl.obolibrary.org/obo/
```

### Comparing `curies-0.5.5/src/curies.egg-info/SOURCES.txt` & `curies-0.5.6/src/curies.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -42,12 +42,11 @@
 src/curies.egg-info/requires.txt
 src/curies.egg-info/top_level.txt
 src/curies/mapping_service/__init__.py
 src/curies/mapping_service/api.py
 src/curies/mapping_service/rdflib_custom.py
 src/curies/mapping_service/utils.py
 tests/__init__.py
-tests/rules.log
 tests/test_api.py
 tests/test_federated_sparql.py
 tests/test_mapping_service.py
 tests/test_web.py
```

### Comparing `curies-0.5.5/tests/test_api.py` & `curies-0.5.6/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `curies-0.5.5/tests/test_federated_sparql.py` & `curies-0.5.6/tests/test_federated_sparql.py`

 * *Files identical despite different names*

### Comparing `curies-0.5.5/tests/test_mapping_service.py` & `curies-0.5.6/tests/test_mapping_service.py`

 * *Files identical despite different names*

### Comparing `curies-0.5.5/tests/test_web.py` & `curies-0.5.6/tests/test_web.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,21 +38,21 @@
         super().setUp()
         self.app = get_fastapi_app(self.converter)
         self.client = TestClient(self.app)
 
     def test_resolve_success(self):
         """Test resolution for a valid CURIE redirects properly."""
         curie = self.converter.format_curie("GO", "1234567")
-        res = self.client.get(f"/{curie}", allow_redirects=False)
+        res = self.client.get(f"/{curie}", follow_redirects=False)
         self.assertEqual(302, res.status_code, msg=res.text)
 
     def test_resolve_failure(self):
         """Test resolution for an invalid CURIE aborts with 404."""
         curie = self.converter.format_curie("NOPREFIX", "NOIDENTIFIER")
-        res = self.client.get(f"/{curie}", allow_redirects=False)
+        res = self.client.get(f"/{curie}", follow_redirects=False)
         self.assertEqual(FAILURE_CODE, res.status_code, msg=res.text)
 
 
 class TestFastAPISlashed(TestFastAPI):
     """Test the FastAPI router with an alternate delimiter."""
 
     delimiter = "/"
```

