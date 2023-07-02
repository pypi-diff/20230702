# Comparing `tmp/py-graphql-mapper-1.1.0.tar.gz` & `tmp/py-graphql-mapper-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-graphql-mapper-1.1.0.tar", last modified: Fri Feb 10 10:45:13 2023, max compression
+gzip compressed data, was "py-graphql-mapper-1.1.1.tar", last modified: Sun Jul  2 15:07:46 2023, max compression
```

## Comparing `py-graphql-mapper-1.1.0.tar` & `py-graphql-mapper-1.1.1.tar`

### file list

```diff
@@ -1,59 +1,63 @@
-drwxrwxrwx   0        0        0        0 2023-02-10 10:45:13.253096 py-graphql-mapper-1.1.0/
--rw-rw-rw-   0        0        0     1085 2023-01-02 12:59:57.000000 py-graphql-mapper-1.1.0/LICENSE
--rw-rw-rw-   0        0        0       44 2023-01-07 21:47:38.000000 py-graphql-mapper-1.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0     7246 2023-02-10 10:45:13.252099 py-graphql-mapper-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     5079 2023-02-10 10:27:27.000000 py-graphql-mapper-1.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-02-10 10:45:13.181881 py-graphql-mapper-1.1.0/codegen/
--rw-rw-rw-   0        0        0        0 2023-01-02 12:59:57.000000 py-graphql-mapper-1.1.0/codegen/__init__.py
--rw-rw-rw-   0        0        0     6215 2023-01-11 18:09:48.000000 py-graphql-mapper-1.1.0/codegen/__main__.py
--rw-rw-rw-   0        0        0     1119 2023-02-01 05:50:35.000000 py-graphql-mapper-1.1.0/codegen/generator.py
--rw-rw-rw-   0        0        0     1557 2023-01-11 18:09:48.000000 py-graphql-mapper-1.1.0/codegen/network.py
--rw-rw-rw-   0        0        0     3761 2023-01-11 18:09:48.000000 py-graphql-mapper-1.1.0/codegen/query_presets.py
-drwxrwxrwx   0        0        0        0 2023-02-10 10:45:13.194791 py-graphql-mapper-1.1.0/codegen/src/
--rw-rw-rw-   0        0        0        0 2023-01-02 12:59:57.000000 py-graphql-mapper-1.1.0/codegen/src/__init__.py
--rw-rw-rw-   0        0        0     4984 2023-02-01 03:53:53.000000 py-graphql-mapper-1.1.0/codegen/src/base_class.py
--rw-rw-rw-   0        0        0      861 2023-02-01 05:29:19.000000 py-graphql-mapper-1.1.0/codegen/src/consts.py
--rw-rw-rw-   0        0        0     1153 2023-02-01 01:59:08.000000 py-graphql-mapper-1.1.0/codegen/src/enums.py
--rw-rw-rw-   0        0        0    39822 2023-02-01 05:38:55.000000 py-graphql-mapper-1.1.0/codegen/src/extractor.py
--rw-rw-rw-   0        0        0     3838 2023-02-01 05:29:17.000000 py-graphql-mapper-1.1.0/codegen/src/printer.py
--rw-rw-rw-   0        0        0      910 2023-02-01 01:59:08.000000 py-graphql-mapper-1.1.0/codegen/src/priority.py
--rw-rw-rw-   0        0        0     8228 2023-01-15 14:20:43.000000 py-graphql-mapper-1.1.0/codegen/src/sp_builder.py
--rw-rw-rw-   0        0        0     1585 2023-02-01 01:59:08.000000 py-graphql-mapper-1.1.0/codegen/src/sp_schema.py
-drwxrwxrwx   0        0        0        0 2023-02-10 10:45:13.203911 py-graphql-mapper-1.1.0/codegen/src/templates/
--rw-rw-rw-   0        0        0       21 2023-01-21 13:54:23.000000 py-graphql-mapper-1.1.0/codegen/src/templates/enum_template.py
--rw-rw-rw-   0        0        0      190 2023-02-01 01:59:08.000000 py-graphql-mapper-1.1.0/codegen/src/templates/mutation_template.py
--rw-rw-rw-   0        0        0      185 2023-02-01 01:59:08.000000 py-graphql-mapper-1.1.0/codegen/src/templates/query_template.py
--rw-rw-rw-   0        0        0       32 2023-02-01 01:59:08.000000 py-graphql-mapper-1.1.0/codegen/src/templates/scalar_template.py
--rw-rw-rw-   0        0        0      233 2023-02-01 01:59:08.000000 py-graphql-mapper-1.1.0/codegen/src/templates/simple_type_template.py
--rw-rw-rw-   0        0        0      112 2023-02-01 01:59:08.000000 py-graphql-mapper-1.1.0/codegen/src/templates/type_refs_template.py
--rw-rw-rw-   0        0        0      301 2023-02-01 01:59:08.000000 py-graphql-mapper-1.1.0/codegen/src/templates/type_template.py
--rw-rw-rw-   0        0        0     2642 2023-02-01 05:12:44.000000 py-graphql-mapper-1.1.0/codegen/src/utils.py
-drwxrwxrwx   0        0        0        0 2023-02-10 10:45:13.226548 py-graphql-mapper-1.1.0/py_graphql_mapper.egg-info/
--rw-rw-rw-   0        0        0     7246 2023-02-10 10:45:13.000000 py-graphql-mapper-1.1.0/py_graphql_mapper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1309 2023-02-10 10:45:13.000000 py-graphql-mapper-1.1.0/py_graphql_mapper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-10 10:45:13.000000 py-graphql-mapper-1.1.0/py_graphql_mapper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2023-02-10 10:45:13.000000 py-graphql-mapper-1.1.0/py_graphql_mapper.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       17 2023-02-10 10:45:13.000000 py-graphql-mapper-1.1.0/py_graphql_mapper.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-02-10 10:45:13.237657 py-graphql-mapper-1.1.0/pygqlmap/
--rw-rw-rw-   0        0        0       51 2023-02-01 01:59:08.000000 py-graphql-mapper-1.1.0/pygqlmap/__init__.py
--rw-rw-rw-   0        0        0     6468 2023-02-01 01:59:08.000000 py-graphql-mapper-1.1.0/pygqlmap/components.py
--rw-rw-rw-   0        0        0       47 2023-01-08 01:49:50.000000 py-graphql-mapper-1.1.0/pygqlmap/config.ini
--rw-rw-rw-   0        0        0      200 2023-01-11 18:09:48.000000 py-graphql-mapper-1.1.0/pygqlmap/enums.py
--rw-rw-rw-   0        0        0      832 2023-01-20 14:12:28.000000 py-graphql-mapper-1.1.0/pygqlmap/gql_operations.py
--rw-rw-rw-   0        0        0      237 2023-02-01 01:59:08.000000 py-graphql-mapper-1.1.0/pygqlmap/gql_types.py
--rw-rw-rw-   0        0        0      830 2023-01-12 21:17:54.000000 py-graphql-mapper-1.1.0/pygqlmap/helper.py
--rw-rw-rw-   0        0        0     3697 2023-01-12 21:06:25.000000 py-graphql-mapper-1.1.0/pygqlmap/network.py
-drwxrwxrwx   0        0        0        0 2023-02-10 10:45:13.251102 py-graphql-mapper-1.1.0/pygqlmap/src/
--rw-rw-rw-   0        0        0        0 2023-01-08 07:30:53.000000 py-graphql-mapper-1.1.0/pygqlmap/src/__init__.py
--rw-rw-rw-   0        0        0      893 2023-02-01 01:59:08.000000 py-graphql-mapper-1.1.0/pygqlmap/src/arg_builtin.py
--rw-rw-rw-   0        0        0     5670 2023-02-01 01:59:08.000000 py-graphql-mapper-1.1.0/pygqlmap/src/base.py
--rw-rw-rw-   0        0        0     5094 2023-02-01 01:59:08.000000 py-graphql-mapper-1.1.0/pygqlmap/src/builder.py
--rw-rw-rw-   0        0        0     1540 2023-02-01 01:59:08.000000 py-graphql-mapper-1.1.0/pygqlmap/src/components.py
--rw-rw-rw-   0        0        0      507 2023-02-01 01:59:08.000000 py-graphql-mapper-1.1.0/pygqlmap/src/consts.py
--rw-rw-rw-   0        0        0      286 2023-01-11 18:09:48.000000 py-graphql-mapper-1.1.0/pygqlmap/src/enums.py
--rw-rw-rw-   0        0        0    11813 2023-02-01 01:59:08.000000 py-graphql-mapper-1.1.0/pygqlmap/src/gql_init.py
--rw-rw-rw-   0        0        0    11238 2023-02-01 01:59:08.000000 py-graphql-mapper-1.1.0/pygqlmap/src/translator.py
--rw-rw-rw-   0        0        0     3594 2023-02-01 01:59:08.000000 py-graphql-mapper-1.1.0/pygqlmap/src/utils.py
--rw-rw-rw-   0        0        0      917 2023-02-10 10:24:48.000000 py-graphql-mapper-1.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-02-10 10:45:13.253096 py-graphql-mapper-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0      730 2023-02-10 10:44:59.000000 py-graphql-mapper-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-02 15:07:46.676561 py-graphql-mapper-1.1.1/
+-rw-rw-rw-   0        0        0     1085 2023-01-02 12:59:57.000000 py-graphql-mapper-1.1.1/LICENSE
+-rw-rw-rw-   0        0        0       44 2023-01-07 21:47:38.000000 py-graphql-mapper-1.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     7343 2023-07-02 15:07:46.675562 py-graphql-mapper-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     5212 2023-07-02 13:13:10.000000 py-graphql-mapper-1.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-02 15:07:46.568038 py-graphql-mapper-1.1.1/codegen/
+-rw-rw-rw-   0        0        0        0 2023-01-02 12:59:57.000000 py-graphql-mapper-1.1.1/codegen/__init__.py
+-rw-rw-rw-   0        0        0     6215 2023-01-11 18:09:48.000000 py-graphql-mapper-1.1.1/codegen/__main__.py
+-rw-rw-rw-   0        0        0     1119 2023-02-01 05:50:35.000000 py-graphql-mapper-1.1.1/codegen/generator.py
+-rw-rw-rw-   0        0        0     1557 2023-01-11 18:09:48.000000 py-graphql-mapper-1.1.1/codegen/network.py
+-rw-rw-rw-   0        0        0     3761 2023-01-11 18:09:48.000000 py-graphql-mapper-1.1.1/codegen/query_presets.py
+drwxrwxrwx   0        0        0        0 2023-07-02 15:07:46.590151 py-graphql-mapper-1.1.1/codegen/src/
+-rw-rw-rw-   0        0        0        0 2023-01-02 12:59:57.000000 py-graphql-mapper-1.1.1/codegen/src/__init__.py
+-rw-rw-rw-   0        0        0     4995 2023-07-02 12:05:42.000000 py-graphql-mapper-1.1.1/codegen/src/base_class.py
+-rw-rw-rw-   0        0        0      861 2023-02-01 05:29:19.000000 py-graphql-mapper-1.1.1/codegen/src/consts.py
+-rw-rw-rw-   0        0        0     1153 2023-02-01 01:59:08.000000 py-graphql-mapper-1.1.1/codegen/src/enums.py
+-rw-rw-rw-   0        0        0    39959 2023-07-02 12:06:43.000000 py-graphql-mapper-1.1.1/codegen/src/extractor.py
+-rw-rw-rw-   0        0        0     3838 2023-02-01 05:29:17.000000 py-graphql-mapper-1.1.1/codegen/src/printer.py
+-rw-rw-rw-   0        0        0      910 2023-02-01 01:59:08.000000 py-graphql-mapper-1.1.1/codegen/src/priority.py
+-rw-rw-rw-   0        0        0     9316 2023-07-02 12:06:43.000000 py-graphql-mapper-1.1.1/codegen/src/sp_builder.py
+-rw-rw-rw-   0        0        0     1575 2023-07-02 12:06:43.000000 py-graphql-mapper-1.1.1/codegen/src/sp_schema.py
+drwxrwxrwx   0        0        0        0 2023-07-02 15:07:46.606137 py-graphql-mapper-1.1.1/codegen/src/templates/
+-rw-rw-rw-   0        0        0       21 2023-01-21 13:54:23.000000 py-graphql-mapper-1.1.1/codegen/src/templates/enum_template.py
+-rw-rw-rw-   0        0        0      190 2023-02-01 01:59:08.000000 py-graphql-mapper-1.1.1/codegen/src/templates/mutation_template.py
+-rw-rw-rw-   0        0        0      185 2023-02-01 01:59:08.000000 py-graphql-mapper-1.1.1/codegen/src/templates/query_template.py
+-rw-rw-rw-   0        0        0       32 2023-02-01 01:59:08.000000 py-graphql-mapper-1.1.1/codegen/src/templates/scalar_template.py
+-rw-rw-rw-   0        0        0      233 2023-02-01 01:59:08.000000 py-graphql-mapper-1.1.1/codegen/src/templates/simple_type_template.py
+-rw-rw-rw-   0        0        0      112 2023-02-01 01:59:08.000000 py-graphql-mapper-1.1.1/codegen/src/templates/type_refs_template.py
+-rw-rw-rw-   0        0        0      301 2023-02-01 01:59:08.000000 py-graphql-mapper-1.1.1/codegen/src/templates/type_template.py
+-rw-rw-rw-   0        0        0     2642 2023-02-01 05:12:44.000000 py-graphql-mapper-1.1.1/codegen/src/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-02 15:07:46.631803 py-graphql-mapper-1.1.1/py_graphql_mapper.egg-info/
+-rw-rw-rw-   0        0        0     7343 2023-07-02 15:07:46.000000 py-graphql-mapper-1.1.1/py_graphql_mapper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1371 2023-07-02 15:07:46.000000 py-graphql-mapper-1.1.1/py_graphql_mapper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-02 15:07:46.000000 py-graphql-mapper-1.1.1/py_graphql_mapper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2023-07-02 15:07:46.000000 py-graphql-mapper-1.1.1/py_graphql_mapper.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       17 2023-07-02 15:07:46.000000 py-graphql-mapper-1.1.1/py_graphql_mapper.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-02 15:07:46.647187 py-graphql-mapper-1.1.1/pygqlmap/
+-rw-rw-rw-   0        0        0       68 2023-07-02 12:05:42.000000 py-graphql-mapper-1.1.1/pygqlmap/__init__.py
+-rw-rw-rw-   0        0        0     6520 2023-07-02 12:06:43.000000 py-graphql-mapper-1.1.1/pygqlmap/components.py
+-rw-rw-rw-   0        0        0       47 2023-01-08 01:49:50.000000 py-graphql-mapper-1.1.1/pygqlmap/config.ini
+-rw-rw-rw-   0        0        0      235 2023-07-02 12:05:42.000000 py-graphql-mapper-1.1.1/pygqlmap/enums.py
+-rw-rw-rw-   0        0        0     1187 2023-07-02 12:05:42.000000 py-graphql-mapper-1.1.1/pygqlmap/gql_operations.py
+-rw-rw-rw-   0        0        0      206 2023-06-26 21:20:33.000000 py-graphql-mapper-1.1.1/pygqlmap/gql_types.py
+-rw-rw-rw-   0        0        0      830 2023-01-12 21:17:54.000000 py-graphql-mapper-1.1.1/pygqlmap/helper.py
+-rw-rw-rw-   0        0        0     3699 2023-07-02 12:33:29.000000 py-graphql-mapper-1.1.1/pygqlmap/network.py
+drwxrwxrwx   0        0        0        0 2023-07-02 15:07:46.667964 py-graphql-mapper-1.1.1/pygqlmap/src/
+-rw-rw-rw-   0        0        0        0 2023-01-08 07:30:53.000000 py-graphql-mapper-1.1.1/pygqlmap/src/__init__.py
+-rw-rw-rw-   0        0        0      893 2023-02-01 01:59:08.000000 py-graphql-mapper-1.1.1/pygqlmap/src/arg_builtin.py
+-rw-rw-rw-   0        0        0     6514 2023-07-02 12:06:43.000000 py-graphql-mapper-1.1.1/pygqlmap/src/base.py
+-rw-rw-rw-   0        0        0     5972 2023-07-02 12:27:17.000000 py-graphql-mapper-1.1.1/pygqlmap/src/builder.py
+-rw-rw-rw-   0        0        0     1540 2023-02-01 01:59:08.000000 py-graphql-mapper-1.1.1/pygqlmap/src/components.py
+-rw-rw-rw-   0        0        0      507 2023-02-01 01:59:08.000000 py-graphql-mapper-1.1.1/pygqlmap/src/consts.py
+-rw-rw-rw-   0        0        0      286 2023-01-11 18:09:48.000000 py-graphql-mapper-1.1.1/pygqlmap/src/enums.py
+-rw-rw-rw-   0        0        0    12480 2023-07-02 12:05:42.000000 py-graphql-mapper-1.1.1/pygqlmap/src/gql_init.py
+-rw-rw-rw-   0        0        0    11332 2023-07-02 12:06:43.000000 py-graphql-mapper-1.1.1/pygqlmap/src/translator.py
+-rw-rw-rw-   0        0        0     3594 2023-02-01 01:59:08.000000 py-graphql-mapper-1.1.1/pygqlmap/src/utils.py
+-rw-rw-rw-   0        0        0      889 2023-07-02 14:05:26.000000 py-graphql-mapper-1.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-02 15:07:46.676561 py-graphql-mapper-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      676 2023-07-02 15:06:41.000000 py-graphql-mapper-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-02 15:07:46.673560 py-graphql-mapper-1.1.1/tests/
+-rw-rw-rw-   0        0        0     4345 2023-02-01 01:59:08.000000 py-graphql-mapper-1.1.1/tests/test_cli.py
+-rw-rw-rw-   0        0        0      973 2023-02-01 01:59:08.000000 py-graphql-mapper-1.1.1/tests/test_codegen.py
+-rw-rw-rw-   0        0        0    11212 2023-07-02 12:06:43.000000 py-graphql-mapper-1.1.1/tests/test_mapping.py
```

### Comparing `py-graphql-mapper-1.1.0/LICENSE` & `py-graphql-mapper-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `py-graphql-mapper-1.1.0/PKG-INFO` & `py-graphql-mapper-1.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-graphql-mapper
-Version: 1.1.0
+Version: 1.1.1
 Summary: A python library to call GraphQL APIs without using hardcoded strings
 Home-page: https://github.com/dapalex/py-graphql-mapper/
 Author: Alex Dap
 Author-email: Alex Dap <shlisi2017@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 dapalex
@@ -27,19 +27,18 @@
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: Homepage, https://github.com/dapalex/py-graphql-mapper/
 Project-URL: Source Code, https://github.com/dapalex/py-graphql-mapper/
 Project-URL: Bug Tracker, https://github.com/dapalex/py-graphql-mapper/issues
 Project-URL: Release Notes, https://github.com/dapalex/py-graphql-mapper/blob/develop/RELEASE_NOTES.MD
-Keywords: graphql,mapper
+Keywords: python,graphql,mapping
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Development Status :: 4 - Beta
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![Python package](https://github.com/dapalex/py-graphql-mapper/actions/workflows/python-package.yml/badge.svg)](https://github.com/dapalex/py-graphql-mapper/actions/workflows/python-package.yml)
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/280533e425784f7da9ecb0f6e529886b)](https://www.codacy.com/gh/dapalex/py-graphql-mapper/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=dapalex/py-graphql-mapper&amp;utm_campaign=Badge_Grade)
 --------------------------------------------------------------------------------
@@ -52,17 +51,17 @@
 ## Introduction
 
 This library acts as a mapper between python and GraphQL languages for GraphQL clients, allowing a code-first approach when calling a GraphQL API server.
 It translates GraphQL entities into python objects and viceversa in order to avoid working with massive "copy&paste"s.
 
 This document contains a quick overview of the functionalities, for more details and options you can read here:
 
-* [Code Generation](https://github.com/dapalex/py-graphql-mapper/blob/main/codegen/README.MD)
-* [Core Mapper](https://github.com/dapalex/py-graphql-mapper/blob/main/pygqlmap/README.MD)
-* [Use Cases](https://github.com/dapalex/py-graphql-mapper/blob/main/tests/README.MD)
+* [Code Generation](https://github.com/dapalex/py-graphql-mapper/blob/develop/codegen/README.MD)
+* [Core Mapper](https://github.com/dapalex/py-graphql-mapper/blob/develop/pygqlmap/README.MD)
+* [Use Cases](https://github.com/dapalex/py-graphql-mapper/blob/develop/tests/README.MD)
 
 
 The package does not use any third-party libraries, it relies only on python 3 (3.10+) standard libraries.
 
 
 ## Usage in a nutshell
 
@@ -76,43 +75,43 @@
 
 
 ### Generate python code from schema
 
 To generate the code execute the following command:
 
 ```
-pgmcodegen generate ./pathToOutputFolder -apiArgs ./pathToArgsFile/generatorArgs.json
+pgmcodegen generate ./pathToOutputFolder -apiArgs ./<pathToArgsFile>/generatorArgs.json
 ```
 
 This command requires a json file containing the parameters needed to get the GraphQL schema
 
-![image](https://github.com/dapalex/py-graphql-mapper/blob/main/docs/cli_args_nutshell.png)
+![image](https://github.com/dapalex/py-graphql-mapper/blob/develop/docs/cli_args_nutshell.png)
 
-A sample is availabe in the main folder 'cli_args.json'
+A sample is available in the main folder ['cli_args.json'](https://github.com/dapalex/py-graphql-mapper/blob/develop/cli_args.json).
 
 The following python files will be generated:
 
 * enums.py
 * scalars.py
 * gql_simple_types.py
 * gql_types.py
 * type_refs.py
 * queries.py
 * mutations.py
 
-These links show code generated using the library [Github GraphQL API](https://github.com/dapalex/py-graphql-mapper/blob/main/tests/output/github), [Rapid GraphQL API](https://github.com/dapalex/py-graphql-mapper/blob/main/tests/output/rapidapi) and [GeoDBCities API](https://github.com/dapalex/py-graphql-mapper/blob/main/tests/output/gdbc)
+These links show code generated using the library [Github GraphQL API](https://github.com/dapalex/py-graphql-mapper/blob/develop/tests/output/github), [Rapid GraphQL API](https://github.com/dapalex/py-graphql-mapper/blob/develop/tests/output/rapidapi) and [GeoDBCities API](https://github.com/dapalex/py-graphql-mapper/blob/develop/tests/output/gdbc)
 
-More command options are available [here](https://github.com/dapalex/py-graphql-mapper/blob/main/codegen/README.MD)
+More command options are available [here](https://github.com/dapalex/py-graphql-mapper/blob/develop/codegen/README.MD#usage-via-command-line)
 
 
 ### Execution of a query
 
 Choose the query class you want to use from the generated file queries.py (or a mutation from mutations.py):
 
-Instantiate it adding GraphQL arguments as parameters:
+Instantiate it adding GraphQL arguments if needed:
 ```python
 from .output.gdbc.queries import currencies
 
 my_currencies = currencies(last=7, before='MTE=')
 ```
 or add them using the field _args_
 
@@ -132,15 +131,15 @@
                                     "content-type": "application/json",
                                         "X-RapidAPI-Key": '123402mmri02fni230iif32jr420',
                                         "X-RapidAPI-Host": "geodb-cities-graphql.p.rapidapi.com"
                                     }
                             )
 ```
 
-More details on how to set a query [here](https://github.com/dapalex/py-graphql-mapper/blob/main/pygqlmap/README.MD#executing-an-operation)
+More details on how to set a query [here](https://github.com/dapalex/py-graphql-mapper/blob/develop/pygqlmap/README.MD#creation-of-an-operation)
 
 
 ### Retrieval of a response
 
 Obtained the response from the GraphQL API the following code will map the received json payload into the python object
 
 ```python
@@ -149,14 +148,13 @@
 gqlResponse = GQLResponse(response)
 
 gqlResponse.map_gqldata_to_obj(myCurrenciesQuery.type)
 
 print('Result object: ' + str(gqlResponse.result_obj))
 ```
 
-The mapped response from the GraphQL server will be available within _gqlResponse_ object: _gqlResponse.result_obj_
+The mapped response from the GraphQL server will be available within _gqlResponse_ object: `_gqlResponse.result_obj_`
 
-More details [here](https://github.com/dapalex/py-graphql-mapper/blob/main/pygqlmap/README.MD#parsing-of-a-response)
+More details [here](https://github.com/dapalex/py-graphql-mapper/blob/develop/pygqlmap/README.MD#parsing-of-a-response)
 
 
-
-A suite of use cases [here](https://github.com/dapalex/py-graphql-mapper/blob/main/tests/README.MD)
+A suite of use cases [here](https://github.com/dapalex/py-graphql-mapper/blob/develop/tests/README.MD)
```

### Comparing `py-graphql-mapper-1.1.0/README.md` & `py-graphql-mapper-1.1.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -10,17 +10,17 @@
 ## Introduction
 
 This library acts as a mapper between python and GraphQL languages for GraphQL clients, allowing a code-first approach when calling a GraphQL API server.
 It translates GraphQL entities into python objects and viceversa in order to avoid working with massive "copy&paste"s.
 
 This document contains a quick overview of the functionalities, for more details and options you can read here:
 
-* [Code Generation](https://github.com/dapalex/py-graphql-mapper/blob/main/codegen/README.MD)
-* [Core Mapper](https://github.com/dapalex/py-graphql-mapper/blob/main/pygqlmap/README.MD)
-* [Use Cases](https://github.com/dapalex/py-graphql-mapper/blob/main/tests/README.MD)
+* [Code Generation](https://github.com/dapalex/py-graphql-mapper/blob/develop/codegen/README.MD)
+* [Core Mapper](https://github.com/dapalex/py-graphql-mapper/blob/develop/pygqlmap/README.MD)
+* [Use Cases](https://github.com/dapalex/py-graphql-mapper/blob/develop/tests/README.MD)
 
 
 The package does not use any third-party libraries, it relies only on python 3 (3.10+) standard libraries.
 
 
 ## Usage in a nutshell
 
@@ -34,43 +34,43 @@
 
 
 ### Generate python code from schema
 
 To generate the code execute the following command:
 
 ```
-pgmcodegen generate ./pathToOutputFolder -apiArgs ./pathToArgsFile/generatorArgs.json
+pgmcodegen generate ./pathToOutputFolder -apiArgs ./<pathToArgsFile>/generatorArgs.json
 ```
 
 This command requires a json file containing the parameters needed to get the GraphQL schema
 
-![image](https://github.com/dapalex/py-graphql-mapper/blob/main/docs/cli_args_nutshell.png)
+![image](https://github.com/dapalex/py-graphql-mapper/blob/develop/docs/cli_args_nutshell.png)
 
-A sample is availabe in the main folder 'cli_args.json'
+A sample is available in the main folder ['cli_args.json'](https://github.com/dapalex/py-graphql-mapper/blob/develop/cli_args.json).
 
 The following python files will be generated:
 
 * enums.py
 * scalars.py
 * gql_simple_types.py
 * gql_types.py
 * type_refs.py
 * queries.py
 * mutations.py
 
-These links show code generated using the library [Github GraphQL API](https://github.com/dapalex/py-graphql-mapper/blob/main/tests/output/github), [Rapid GraphQL API](https://github.com/dapalex/py-graphql-mapper/blob/main/tests/output/rapidapi) and [GeoDBCities API](https://github.com/dapalex/py-graphql-mapper/blob/main/tests/output/gdbc)
+These links show code generated using the library [Github GraphQL API](https://github.com/dapalex/py-graphql-mapper/blob/develop/tests/output/github), [Rapid GraphQL API](https://github.com/dapalex/py-graphql-mapper/blob/develop/tests/output/rapidapi) and [GeoDBCities API](https://github.com/dapalex/py-graphql-mapper/blob/develop/tests/output/gdbc)
 
-More command options are available [here](https://github.com/dapalex/py-graphql-mapper/blob/main/codegen/README.MD)
+More command options are available [here](https://github.com/dapalex/py-graphql-mapper/blob/develop/codegen/README.MD#usage-via-command-line)
 
 
 ### Execution of a query
 
 Choose the query class you want to use from the generated file queries.py (or a mutation from mutations.py):
 
-Instantiate it adding GraphQL arguments as parameters:
+Instantiate it adding GraphQL arguments if needed:
 ```python
 from .output.gdbc.queries import currencies
 
 my_currencies = currencies(last=7, before='MTE=')
 ```
 or add them using the field _args_
 
@@ -90,15 +90,15 @@
                                     "content-type": "application/json",
                                         "X-RapidAPI-Key": '123402mmri02fni230iif32jr420',
                                         "X-RapidAPI-Host": "geodb-cities-graphql.p.rapidapi.com"
                                     }
                             )
 ```
 
-More details on how to set a query [here](https://github.com/dapalex/py-graphql-mapper/blob/main/pygqlmap/README.MD#executing-an-operation)
+More details on how to set a query [here](https://github.com/dapalex/py-graphql-mapper/blob/develop/pygqlmap/README.MD#creation-of-an-operation)
 
 
 ### Retrieval of a response
 
 Obtained the response from the GraphQL API the following code will map the received json payload into the python object
 
 ```python
@@ -107,14 +107,13 @@
 gqlResponse = GQLResponse(response)
 
 gqlResponse.map_gqldata_to_obj(myCurrenciesQuery.type)
 
 print('Result object: ' + str(gqlResponse.result_obj))
 ```
 
-The mapped response from the GraphQL server will be available within _gqlResponse_ object: _gqlResponse.result_obj_
+The mapped response from the GraphQL server will be available within _gqlResponse_ object: `_gqlResponse.result_obj_`
 
-More details [here](https://github.com/dapalex/py-graphql-mapper/blob/main/pygqlmap/README.MD#parsing-of-a-response)
+More details [here](https://github.com/dapalex/py-graphql-mapper/blob/develop/pygqlmap/README.MD#parsing-of-a-response)
 
 
-
-A suite of use cases [here](https://github.com/dapalex/py-graphql-mapper/blob/main/tests/README.MD)
+A suite of use cases [here](https://github.com/dapalex/py-graphql-mapper/blob/develop/tests/README.MD)
```

### Comparing `py-graphql-mapper-1.1.0/codegen/__main__.py` & `py-graphql-mapper-1.1.1/codegen/__main__.py`

 * *Files identical despite different names*

### Comparing `py-graphql-mapper-1.1.0/codegen/generator.py` & `py-graphql-mapper-1.1.1/codegen/generator.py`

 * *Files identical despite different names*

### Comparing `py-graphql-mapper-1.1.0/codegen/network.py` & `py-graphql-mapper-1.1.1/codegen/network.py`

 * *Files identical despite different names*

### Comparing `py-graphql-mapper-1.1.0/codegen/query_presets.py` & `py-graphql-mapper-1.1.1/codegen/query_presets.py`

 * *Files identical despite different names*

### Comparing `py-graphql-mapper-1.1.0/codegen/src/base_class.py` & `py-graphql-mapper-1.1.1/codegen/src/base_class.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
             try:
                 py_type = Translate.to_python_type(type_def)
                 if py_type == TypeKind.NON_NULL.name:
                     is_nonnull = True
                     continue
                 elif py_type == TypeKind.LIST.name:
                     is_list = True
-                    type_out += (NON_NULL_PREFIX if is_nonnull else '') + GQLLIST_PREFIX
+                    type_out += (NON_NULL_PREFIX if is_nonnull and is_arg else '') + GQLLIST_PREFIX
                     if is_nonnull: is_nonnull = False
                     continue
 
                 if is_list:
                     if py_type in STRING_GQLLIST_BUILTIN or 'ENUM' in self.get_used_typekinds():
                         type_out = type_out.removesuffix('_')
                         type_out += '['
```

### Comparing `py-graphql-mapper-1.1.0/codegen/src/consts.py` & `py-graphql-mapper-1.1.1/codegen/src/consts.py`

 * *Files identical despite different names*

### Comparing `py-graphql-mapper-1.1.0/codegen/src/enums.py` & `py-graphql-mapper-1.1.1/codegen/src/enums.py`

 * *Files identical despite different names*

### Comparing `py-graphql-mapper-1.1.0/codegen/src/extractor.py` & `py-graphql-mapper-1.1.1/codegen/src/extractor.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,18 +89,18 @@
                 currentType = self.schema.types.popitem()
                 if self.log_progress: logger.info('Started extraction of type ' + currentType[0])
                 if currentType[0].startswith('__'):
                     continue
                 if currentType[1].kind == TypeKind.SCALAR.name:
                     self.scalars.update({ currentType[0]: currentType[1] })
                     continue
-                if currentType[0] == 'Query':
+                if hasattr(self.schema.queryType, "name") and currentType[0] == self.schema.queryType.name:
                     self.queries = currentType[1]
                     continue
-                if currentType[0] == 'Mutation':
+                if hasattr(self.schema.mutationType, "name") and currentType[0] == self.schema.mutationType.name:
                     self.mutations = currentType[1]
                     continue
                 if currentType[1].kind == TypeKind.ENUM.name:
                     self.enums.update({ currentType[0]: currentType[1] })
                     continue
                 else:
                     tempTypes.update({ currentType[0]: currentType[1] })
@@ -667,16 +667,17 @@
                 if (
                     py_inline_type.__contains__((gqllist_type := (NON_NULL_PREFIX + GQLLIST_PREFIX + py_el_tp))) or \
                     py_inline_type.__contains__((gqllist_type := (GQLLIST_PREFIX + py_el_tp)))
                     or \
                     (
                     circ_ref_utilizer and \
                     (
-                    py_inline_type.__contains__((gqllist_type := (GQLLIST_PREFIX + new_type))) or \
-                    py_inline_type.__contains__((gqllist_type := (NON_NULL_PREFIX + GQLLIST_PREFIX + new_type)))
+                        py_inline_type.__contains__((gqllist_type := (NON_NULL_PREFIX + GQLLIST_PREFIX + new_type))) or \
+                        py_inline_type.__contains__((gqllist_type := (GQLLIST_PREFIX + new_type)))
+
                     )
                     )
                 ) \
                 and \
                 not py_el_tp in STRING_GQLLIST_BUILTIN:
                     if circ_ref_utilizer:
                         py_inline_split = py_inline_type.split(gqllist_type)
```

### Comparing `py-graphql-mapper-1.1.0/codegen/src/printer.py` & `py-graphql-mapper-1.1.1/codegen/src/printer.py`

 * *Files identical despite different names*

### Comparing `py-graphql-mapper-1.1.0/codegen/src/priority.py` & `py-graphql-mapper-1.1.1/codegen/src/priority.py`

 * *Files identical despite different names*

### Comparing `py-graphql-mapper-1.1.0/codegen/src/sp_builder.py` & `py-graphql-mapper-1.1.1/codegen/src/sp_builder.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 
 import copy
 from pygqlmap.src.builder import Builder
+from pygqlmap.src.enums import BuildingType
+import logging as logger
 from .sp_schema import GQLSchema, SCArg, SCType, SCDirective, SCField, SCEnumValue, SCInterface, SCInputField, SCOperationType,  SCArgType, SCOfType,  SCFieldType
 
 class SchemaTypeBuilder(Builder):
 
     def build(self, data_input, py_obj):
         inputType = data_input['__type']
 
@@ -56,28 +58,28 @@
                     raise Exception("Error during extraction of inputField" + ' - ' + ex.args[0])
         except Exception as ex:
             raise Exception("Exception during Schema Type building" + ' - ' + ex.args[0])
 
         return schemaType
 
     def build_scoftype(dataInput):
-        field = SCOfType()
+        ofType = SCOfType()
 
         try:
             while len(dataInput.items()) > 0:
                 fieldField = dataInput.popitem()
                 if fieldField[0] == 'ofType' and fieldField[1]: ##SKIPPING NON NULL MANAGEMENT, it will be back!
-                    return  SchemaTypeBuilder.build_scoftype(fieldField[1])
+                    ofType.ofType = SchemaTypeBuilder.build_scoftype(fieldField[1])
                 else:
-                    setattr(field, fieldField[0], fieldField[1])
+                    setattr(ofType, fieldField[0], fieldField[1])
 
         except Exception as ex:
             raise Exception("Exception during OfType building" + ' - ' + ex.args[0])
 
-        return field
+        return ofType
 
     def build_scfieldtype(dataInput):
         field = SCFieldType()
 
         try:
             while len(dataInput.items()) > 0:
                 fieldField = dataInput.popitem()
@@ -189,7 +191,29 @@
     def buildDirective(self, dataInput):
         directive = SCDirective()
         while len(dataInput.items()) > 0:
             inputField = dataInput.popitem()
             setattr(directive, inputField[0], SchemaTypeBuilder.buildArgsOrInputFields(inputField[1], False) if inputField[0] == 'args' else inputField[1])
 
         return directive
+
+    def set_py_fields(self, dataInput, opObject, customObject=None):
+        """  for internal use only    """
+        newObjModelDict = opObject.__dataclass_fields__ ##maybe asdict better
+        attr_to_del = []
+
+        if type(dataInput) == list:
+            for dataEl in dataInput:
+                if not dataEl: continue
+                self.set_py_fields_inner(newObjModelDict, dataEl, opObject, customObject, attr_to_del)
+        else:
+            self.set_py_fields_inner(newObjModelDict, dataInput, opObject, customObject, attr_to_del)
+
+        for a in attr_to_del:
+            if a in opObject.__dict__.keys():
+                if self.build_sctype == BuildingType.STANDARD:
+                    attr = getattr(opObject, a)
+                    del attr
+                elif self.build_sctype == BuildingType.ALTERCLASS:
+                    logger.info('delete attribute from class')
+                else:
+                    logger.info('should do nothing in new object')
```

### Comparing `py-graphql-mapper-1.1.0/codegen/src/sp_schema.py` & `py-graphql-mapper-1.1.1/codegen/src/sp_schema.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     name: str
     description: str
     isDeprecated: bool
 
 class SCOfType(SchemaTypeManager):
     kind: str
     name: str
-    ofType: any #SCOfType || SCType
+    ofType: any #SCOfType
 
 class SCArgType(SchemaTypeManager):
     kind: TypeKind
     name: str
     ofType: SCOfType
 
 class SCArg(SchemaTypeManager):
```

### Comparing `py-graphql-mapper-1.1.0/codegen/src/utils.py` & `py-graphql-mapper-1.1.1/codegen/src/utils.py`

 * *Files identical despite different names*

### Comparing `py-graphql-mapper-1.1.0/py_graphql_mapper.egg-info/PKG-INFO` & `py-graphql-mapper-1.1.1/py_graphql_mapper.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-graphql-mapper
-Version: 1.1.0
+Version: 1.1.1
 Summary: A python library to call GraphQL APIs without using hardcoded strings
 Home-page: https://github.com/dapalex/py-graphql-mapper/
 Author: Alex Dap
 Author-email: Alex Dap <shlisi2017@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 dapalex
@@ -27,19 +27,18 @@
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: Homepage, https://github.com/dapalex/py-graphql-mapper/
 Project-URL: Source Code, https://github.com/dapalex/py-graphql-mapper/
 Project-URL: Bug Tracker, https://github.com/dapalex/py-graphql-mapper/issues
 Project-URL: Release Notes, https://github.com/dapalex/py-graphql-mapper/blob/develop/RELEASE_NOTES.MD
-Keywords: graphql,mapper
+Keywords: python,graphql,mapping
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Development Status :: 4 - Beta
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![Python package](https://github.com/dapalex/py-graphql-mapper/actions/workflows/python-package.yml/badge.svg)](https://github.com/dapalex/py-graphql-mapper/actions/workflows/python-package.yml)
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/280533e425784f7da9ecb0f6e529886b)](https://www.codacy.com/gh/dapalex/py-graphql-mapper/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=dapalex/py-graphql-mapper&amp;utm_campaign=Badge_Grade)
 --------------------------------------------------------------------------------
@@ -52,17 +51,17 @@
 ## Introduction
 
 This library acts as a mapper between python and GraphQL languages for GraphQL clients, allowing a code-first approach when calling a GraphQL API server.
 It translates GraphQL entities into python objects and viceversa in order to avoid working with massive "copy&paste"s.
 
 This document contains a quick overview of the functionalities, for more details and options you can read here:
 
-* [Code Generation](https://github.com/dapalex/py-graphql-mapper/blob/main/codegen/README.MD)
-* [Core Mapper](https://github.com/dapalex/py-graphql-mapper/blob/main/pygqlmap/README.MD)
-* [Use Cases](https://github.com/dapalex/py-graphql-mapper/blob/main/tests/README.MD)
+* [Code Generation](https://github.com/dapalex/py-graphql-mapper/blob/develop/codegen/README.MD)
+* [Core Mapper](https://github.com/dapalex/py-graphql-mapper/blob/develop/pygqlmap/README.MD)
+* [Use Cases](https://github.com/dapalex/py-graphql-mapper/blob/develop/tests/README.MD)
 
 
 The package does not use any third-party libraries, it relies only on python 3 (3.10+) standard libraries.
 
 
 ## Usage in a nutshell
 
@@ -76,43 +75,43 @@
 
 
 ### Generate python code from schema
 
 To generate the code execute the following command:
 
 ```
-pgmcodegen generate ./pathToOutputFolder -apiArgs ./pathToArgsFile/generatorArgs.json
+pgmcodegen generate ./pathToOutputFolder -apiArgs ./<pathToArgsFile>/generatorArgs.json
 ```
 
 This command requires a json file containing the parameters needed to get the GraphQL schema
 
-![image](https://github.com/dapalex/py-graphql-mapper/blob/main/docs/cli_args_nutshell.png)
+![image](https://github.com/dapalex/py-graphql-mapper/blob/develop/docs/cli_args_nutshell.png)
 
-A sample is availabe in the main folder 'cli_args.json'
+A sample is available in the main folder ['cli_args.json'](https://github.com/dapalex/py-graphql-mapper/blob/develop/cli_args.json).
 
 The following python files will be generated:
 
 * enums.py
 * scalars.py
 * gql_simple_types.py
 * gql_types.py
 * type_refs.py
 * queries.py
 * mutations.py
 
-These links show code generated using the library [Github GraphQL API](https://github.com/dapalex/py-graphql-mapper/blob/main/tests/output/github), [Rapid GraphQL API](https://github.com/dapalex/py-graphql-mapper/blob/main/tests/output/rapidapi) and [GeoDBCities API](https://github.com/dapalex/py-graphql-mapper/blob/main/tests/output/gdbc)
+These links show code generated using the library [Github GraphQL API](https://github.com/dapalex/py-graphql-mapper/blob/develop/tests/output/github), [Rapid GraphQL API](https://github.com/dapalex/py-graphql-mapper/blob/develop/tests/output/rapidapi) and [GeoDBCities API](https://github.com/dapalex/py-graphql-mapper/blob/develop/tests/output/gdbc)
 
-More command options are available [here](https://github.com/dapalex/py-graphql-mapper/blob/main/codegen/README.MD)
+More command options are available [here](https://github.com/dapalex/py-graphql-mapper/blob/develop/codegen/README.MD#usage-via-command-line)
 
 
 ### Execution of a query
 
 Choose the query class you want to use from the generated file queries.py (or a mutation from mutations.py):
 
-Instantiate it adding GraphQL arguments as parameters:
+Instantiate it adding GraphQL arguments if needed:
 ```python
 from .output.gdbc.queries import currencies
 
 my_currencies = currencies(last=7, before='MTE=')
 ```
 or add them using the field _args_
 
@@ -132,15 +131,15 @@
                                     "content-type": "application/json",
                                         "X-RapidAPI-Key": '123402mmri02fni230iif32jr420',
                                         "X-RapidAPI-Host": "geodb-cities-graphql.p.rapidapi.com"
                                     }
                             )
 ```
 
-More details on how to set a query [here](https://github.com/dapalex/py-graphql-mapper/blob/main/pygqlmap/README.MD#executing-an-operation)
+More details on how to set a query [here](https://github.com/dapalex/py-graphql-mapper/blob/develop/pygqlmap/README.MD#creation-of-an-operation)
 
 
 ### Retrieval of a response
 
 Obtained the response from the GraphQL API the following code will map the received json payload into the python object
 
 ```python
@@ -149,14 +148,13 @@
 gqlResponse = GQLResponse(response)
 
 gqlResponse.map_gqldata_to_obj(myCurrenciesQuery.type)
 
 print('Result object: ' + str(gqlResponse.result_obj))
 ```
 
-The mapped response from the GraphQL server will be available within _gqlResponse_ object: _gqlResponse.result_obj_
+The mapped response from the GraphQL server will be available within _gqlResponse_ object: `_gqlResponse.result_obj_`
 
-More details [here](https://github.com/dapalex/py-graphql-mapper/blob/main/pygqlmap/README.MD#parsing-of-a-response)
+More details [here](https://github.com/dapalex/py-graphql-mapper/blob/develop/pygqlmap/README.MD#parsing-of-a-response)
 
 
-
-A suite of use cases [here](https://github.com/dapalex/py-graphql-mapper/blob/main/tests/README.MD)
+A suite of use cases [here](https://github.com/dapalex/py-graphql-mapper/blob/develop/tests/README.MD)
```

### Comparing `py-graphql-mapper-1.1.0/py_graphql_mapper.egg-info/SOURCES.txt` & `py-graphql-mapper-1.1.1/py_graphql_mapper.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -43,8 +43,11 @@
 pygqlmap/src/base.py
 pygqlmap/src/builder.py
 pygqlmap/src/components.py
 pygqlmap/src/consts.py
 pygqlmap/src/enums.py
 pygqlmap/src/gql_init.py
 pygqlmap/src/translator.py
-pygqlmap/src/utils.py
+pygqlmap/src/utils.py
+tests/test_cli.py
+tests/test_codegen.py
+tests/test_mapping.py
```

### Comparing `py-graphql-mapper-1.1.0/pygqlmap/components.py` & `py-graphql-mapper-1.1.1/pygqlmap/components.py`

 * *Files 2% similar despite different names*

```diff
@@ -123,42 +123,42 @@
             prefix = self.obj_type.value + ' ' + self.name + ' '
             self.type.log_progress = self.log_progress
 
             ##Arguments of the operation are arguments of the root object
             if hasattr(self, ARGS_DECLARE):
                 setattr(self.type, ARGS_DECLARE, getattr(self, ARGS_DECLARE))
 
-            #Update all objects args with the argument type requested
-            self.manage_args(self.type)
+            #Update all payload arguments (NESTED ARGUMENTS) with the argument type requested
+            self.manage_nested_args(self.type)
             # self.setArgsLocations(self.type, None, rootName, '')
 
             if self._args_type == ArgType.VARIABLES:
                 if hasattr(self, ARGS_DECLARE) and self.arguments:
                     prefix += '(' + self.export_gqlarg_keys + ')'
 
             return prefix + ' { ' + self.__class__.__name__ + self.type.export_gql_source + ' } '
         except Exception as ex:
             raise handle_recursive_ex(ex, 'Issue during export of ' + self.name)
 
-    def manage_args(self, currentObj):
+    def manage_nested_args(self, currentObj):
         if not self.arguments: self.arguments = {}
         try:
             if isinstance(currentObj, list): #if it is I have to set the elements as well?
                 for list_el in currentObj:
-                    self.manage_args(list_el)
+                    self.manage_nested_args(list_el)
 
             #if obj contains field with arg name, add arg
             if type(currentObj) in PRIMITIVES or not hasattr(currentObj, '__dataclass_fields__'):
                 return
 
             if hasattr(currentObj, ARGS_DECLARE):
                 currentObj._args._args_type = self._args_type
                 for arg in currentObj._args.__dataclass_fields__:
                     argValue = getattr(currentObj._args, arg)
                     if is_empty_field(argValue): continue
                     self.arguments.update({arg: (argValue, currentObj._args.__dataclass_fields__[arg].type)})
 
             for subObj in currentObj.__dataclass_fields__:
                 if subObj == ARGS_DECLARE:  continue
-                self.manage_args(getattr(currentObj, subObj))
+                self.manage_nested_args(getattr(currentObj, subObj))
         except Exception as ex:
             raise handle_recursive_ex(ex, 'Error during args type propagation - ')
```

### Comparing `py-graphql-mapper-1.1.0/pygqlmap/gql_operations.py` & `py-graphql-mapper-1.1.1/pygqlmap/gql_operations.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from dataclasses import dataclass
 from pygqlmap.components import GQLOperation
 from pygqlmap.enums import ArgType, OperationType
-from pygqlmap.src.gql_init import _query_init, _mutation_init
+from pygqlmap.src.gql_init import _query_init, _mutation_init, _subscription_init
 
 class GQLQuery(GQLOperation):
 
     def __init_subclass__(cls):
         cls = dataclass(cls)
         cls.__init__ = _query_init
 
@@ -20,7 +20,18 @@
         cls = dataclass(cls)
         cls.__init__ = _mutation_init
 
     def __init__(self):
         if hasattr(self, 'args'):
             self._args = self.args
         super().__init__(OperationType.MUTATION, self.type, ArgType.LITERAL_VALUES)
+
+class GQLSubscription(GQLOperation):
+
+    def __init_subclass__(cls):
+        cls = dataclass(cls)
+        cls.__init__ = _subscription_init
+
+    def __init__(self):
+        if hasattr(self, 'args'):
+            self._args = self.args
+        super().__init__(OperationType.SUBSCRIPTION, self.type, ArgType.LITERAL_VALUES)
```

### Comparing `py-graphql-mapper-1.1.0/pygqlmap/helper.py` & `py-graphql-mapper-1.1.1/pygqlmap/helper.py`

 * *Files identical despite different names*

### Comparing `py-graphql-mapper-1.1.0/pygqlmap/network.py` & `py-graphql-mapper-1.1.1/pygqlmap/network.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import json
 from urllib import request
 from urllib.error import HTTPError
 import logging as logger
-from .src.builder import QueryBuilder
+from .src.builder import ResultBuilder
 from .src.enums import BuildingType
 
 def send_http_request(api_url, payload, httpHeaders):
     try:
         body = json.dumps(payload, indent=2).encode('ascii')
         req = request.Request(api_url, data=body)
         for http_header_key, http_header_val in httpHeaders.items():
@@ -45,15 +45,15 @@
 
         Args:
             mappedPyObject (_type_, optional): python object mapped from a GraphQL type
                                                A reference can be found in the GQLOperation object created as <queryObject>.type
             build_sctype (BuildingType, optional): Options not yet implemented. Defaults to BuildingType.STANDARD.
         """
         if hasattr(self, 'data') and self.data:
-            myBuilder = QueryBuilder(build_type, self.log_progress)
+            myBuilder = ResultBuilder(build_type, self.log_progress)
             self.result_obj = myBuilder.build(self.data, mapped_py_obj)
         else:
             self.result_obj = None
 
     def print_msg_out(self):
         """!This function works with built-in python module urllib3 and requests library
```

### Comparing `py-graphql-mapper-1.1.0/pygqlmap/src/arg_builtin.py` & `py-graphql-mapper-1.1.1/pygqlmap/src/arg_builtin.py`

 * *Files identical despite different names*

### Comparing `py-graphql-mapper-1.1.0/pygqlmap/src/base.py` & `py-graphql-mapper-1.1.1/pygqlmap/src/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,14 +23,40 @@
                 for field in self._fieldsshow:
                     self._fieldsshow[field] = True
             except Exception as ex:
                raise handle_recursive_ex(ex, 'Error during fieldShow initialization for field ' + field)
         except Exception as ex:
            raise handle_recursive_ex(ex, 'Error during fieldShow initialization')
 
+class Builder():
+    @abstractmethod
+    def build(self, dataInput, pyObject):
+        pass
+
+    @abstractmethod
+    def set_py_fields(self, dataInput, opObject, customObject=None):
+        pass
+
+    def build(self, inputDict: dict, pyObject: any):
+        """  for internal use only    """
+
+        try:
+            if self.log_progress: logger.info('Started building of python object: ' + pyObject.__class__.__name__)
+            item = inputDict.popitem() ##extract the KV pair containing object name and content
+
+            if not item[1] == None:
+                self.set_py_fields(item[1], pyObject)
+            else:
+                logger.info(item[0] + ' has no content')
+
+        except Exception as ex:
+            logger.error('Building of python object failed - ' + ex.args[0])
+
+        return pyObject
+
 class GQLExporter():
 
     log_progress: bool
 
     @property
     def export_gql_source(self):
         gqlArgs, outputGqlDict = self.export_gql_dict
```

### Comparing `py-graphql-mapper-1.1.0/pygqlmap/src/builder.py` & `py-graphql-mapper-1.1.1/pygqlmap/src/builder.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,52 +1,61 @@
-from abc import abstractmethod
 from enum import Enum
 import logging as logger
+from pygqlmap.src.base import Builder
 from .enums import BuildingType
 from .consts import GQL_BUILTIN
-
-class Builder():
-    @abstractmethod
-    def build(self, dataInput, pyObject):
-        pass
+import inspect
 
 class QueryBuilder(Builder):
     """  for internal use only    """
     build_sctype: BuildingType
     log_progress: bool
 
     def __init__(self, build_sctype: BuildingType, log_progress: bool = False):
         self.build_sctype = build_sctype
         self.log_progress = log_progress
 
         super().__init__()
 
-    def build(self, inputDict: dict, pyObject: any):
+    def set_py_fields(self, dataInput, opObject, customObject=None):
         """  for internal use only    """
+        newObjModelDict = opObject.__dataclass_fields__ ##maybe asdict better
+        attr_to_del = []
 
-        try:
-            if self.log_progress: logger.info('Started building of python object: ' + pyObject.__class__.__name__)
-            item = inputDict.popitem() ##extract the KV pair containing object name and content
-
-            if not item[1] == None:
-                self.set_py_fields(item[1], pyObject)
-            else:
-                logger.info(item[0] + ' has no content')
-
-        except Exception as ex:
-            logger.error('Building of python object failed - ' + ex.args[0])
-
-        return pyObject
+        if type(dataInput) == list:
+            ##get element type
+            self.set_py_list_fields(dataInput, opObject, customObject, attr_to_del)
+        else:
+            self.set_py_fields_inner(newObjModelDict, dataInput, opObject, customObject, attr_to_del)
 
-    def set_py_fields(self, dataInput, opObject, customObject=None):
-        """  for internal use only    """
-        newObjDict = opObject.__dataclass_fields__ ##maybe asdict better
-        attrToDel = []
+        # for a in attr_to_del:
+        #     if a in opObject.__dict__.keys():
+        #         if self.build_sctype == BuildingType.STANDARD:
+        #             attr = getattr(opObject, a)
+        #             del attr
+        #         elif self.build_sctype == BuildingType.ALTERCLASS:
+        #             logger.info('delete attribute from class')
+        #         else:
+        #             logger.info('should do nothing in new object')
+
+    def set_py_list_fields(self, dataInput, opObject, customObject, attr_to_del):
+        for t in inspect.getmro(type(opObject)):
+            if t == type(opObject): continue
+            if t == list: continue
+            eltype = t
+            break
+
+        for dataEl in dataInput:
+            if not dataEl: continue
+            element = eltype()
+            self.set_py_fields_inner(element.__dataclass_fields__, dataEl, element, customObject, attr_to_del)
+            opObject.append(element)
 
-        for el in newObjDict:
+    def set_py_fields_inner(self, newObjModelDict, dataInput, opObject, customObject, attr_to_del):
+        for el in newObjModelDict:
             try:
                 if self.log_progress: logger.info('Started building of field: ' + el)
 
                 if  (not el in opObject.fieldsshow.keys() or not opObject.fieldsshow[el]):
                     if self.log_progress: logger.warning('Field ' + el + ' in ' + opObject + 'not present in fieldsshow')
                     continue
 
@@ -69,47 +78,55 @@
                                     self.set_py_fields(subEl, subElObject)
                                     listObjectElement.append(subElObject)
                             else:
                                 setattr(opObject, el, self.build({ el: dataInput[el] }, attribute))   #, newObject
                         else:
                             self.set_py_field_value(opObject, el, dataInput[el])
                 else:
-                    self.clean_py_value(opObject, el, attrToDel)
+                    self.clean_py_value(opObject, el, attr_to_del)
 
             except Exception as ex:
                 logger.error('Setting value for element ' + el + ' failed - ' + ex.args[0])
 
-        for a in attrToDel:
-            if a in opObject.__dict__.keys():
-                if self.build_sctype == BuildingType.STANDARD:
-                    attr = getattr(opObject, a)
-                    del attr
-                elif self.build_sctype == BuildingType.ALTERCLASS:
-                    logger.info('delete attribute from class')
-                else:
-                    logger.info('should do nothing in new object')
-
     def set_py_field_value(self, obj, attr, value):
         """  for internal use only    """
         if self.log_progress: logger.info('Setting value of: ' + attr)
         try:
             if obj.fieldsshow:
                 if obj.fieldsshow[attr]:
                     if self.build_sctype == BuildingType.STANDARD or self.build_sctype == BuildingType.ALTERCLASS:
                         setattr(obj, attr, value)
                     else:
                         logger.info('new object management')
         except Exception as ex:
             logger.error('Setting value of: ' + attr + ' failed - ' + ex.args[0])
 
-    def clean_py_value(self, obj, field, attrToDel):
+    def clean_py_value(self, obj, field, attr_to_del):
         """  for internal use only    """
         if self.log_progress: logger.info('Cleaning value of: ' + field)
         if self.build_sctype == BuildingType.STANDARD:
             setattr(obj, field, None)
         elif self.build_sctype == BuildingType.ALTERCLASS:
             logger.info('alter class to delete field')
-            attrToDel.append(field)
+            attr_to_del.append(field)
         elif self.build_sctype == BuildingType.CREATENEWCLASS:
             logger.info('do nothing in new class')
         else:
             raise Exception('build_sctype not assigned')
+
+class ResultBuilder(QueryBuilder):
+    def set_py_list_fields(self, dataInput, opObject, customObject, attr_to_del):
+        for t in inspect.getmro(type(opObject)):
+            if t == type(opObject): continue
+            if t == list: continue
+            eltype = t
+            break
+
+        for dataEl in dataInput:
+            if not dataEl: continue
+            element = eltype()
+            self.set_py_fields_inner(element.__dataclass_fields__, dataEl, element, customObject, attr_to_del)
+            opObject.append(element)
+
+        for d_field in opObject.__dataclass_fields__:
+            delattr(opObject, d_field)
+        return
```

### Comparing `py-graphql-mapper-1.1.0/pygqlmap/src/components.py` & `py-graphql-mapper-1.1.1/pygqlmap/src/components.py`

 * *Files identical despite different names*

### Comparing `py-graphql-mapper-1.1.0/pygqlmap/src/gql_init.py` & `py-graphql-mapper-1.1.1/pygqlmap/src/gql_init.py`

 * *Files 3% similar despite different names*

```diff
@@ -157,14 +157,15 @@
             obj._args = obj.args
         from pygqlmap.enums import ArgType, OperationType
         from pygqlmap import GQLMutation
         super(GQLMutation, obj).__init__(op_type=OperationType.MUTATION, dataType=obj.type, argsType=ArgType.LITERAL_VALUES)
     except Exception as ex:
         raise handle_recursive_ex(ex, 'Error during Mutation init execution for ' + obj.__class__.__name__)
 
+##Sure need 2 copies?
 def _query_init(obj, **kwargs):
     global currentPath, circularRefs, mergedClasses
     currentPath = None
     mergedClasses = {}
     circularRefs = {}
     try:
         _sub_class_init(obj, **kwargs)
@@ -172,14 +173,29 @@
             obj._args = obj.args
         from pygqlmap.enums import ArgType, OperationType
         from pygqlmap import GQLQuery
         super(GQLQuery, obj).__init__(op_type=OperationType.QUERY, dataType=obj.type, argsType=ArgType.LITERAL_VALUES)
     except Exception as ex:
         raise handle_recursive_ex(ex, 'Error during Query init execution for ' + obj.__class__.__name__)
 
+def _subscription_init(obj, **kwargs):
+    global currentPath, circularRefs, mergedClasses
+    currentPath = None
+    mergedClasses = {}
+    circularRefs = {}
+    try:
+        _sub_class_init(obj, **kwargs)
+        if hasattr(obj, 'args'):
+            obj._args = obj.args
+        from pygqlmap.enums import ArgType, OperationType
+        from pygqlmap import GQLQuery
+        super(GQLQuery, obj).__init__(op_type=OperationType.SUBSCRIPTION, dataType=obj.type, argsType=ArgType.LITERAL_VALUES)
+    except Exception as ex:
+        raise handle_recursive_ex(ex, 'Error during Query init execution for ' + obj.__class__.__name__)
+
 def _add_circular_ref(fieldType):
     global circularRefs, currentPath
     try:
         for circRefType,  circRefPath in circularRefs.keys():
             if circRefType == fieldType.__name__:
                 if currentPath.__contains__(circRefPath):
                     return
```

### Comparing `py-graphql-mapper-1.1.0/pygqlmap/src/translator.py` & `py-graphql-mapper-1.1.1/pygqlmap/src/translator.py`

 * *Files 1% similar despite different names*

```diff
@@ -223,481 +223,487 @@
 00000de0: 7267 735f 5f0d 0a20 2020 2020 2020 2020  rgs__..         
 00000df0: 2020 2020 2020 2066 726f 6d20 7079 6771         from pygq
 00000e00: 6c6d 6170 2e63 6f6d 706f 6e65 6e74 7320  lmap.components 
 00000e10: 696d 706f 7274 2047 514c 4f62 6a65 6374  import GQLObject
 00000e20: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
 00000e30: 2020 6966 2061 6c6c 285b 7479 7065 2865    if all([type(e
 00000e40: 6c29 2069 6e20 5052 494d 4954 4956 4553  l) in PRIMITIVES
-00000e50: 2066 6f72 2065 6c20 696e 2065 6c65 6d65   for el in eleme
-00000e60: 6e74 735d 293a 0d0a 2020 2020 2020 2020  nts]):..        
-00000e70: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00000e80: 726e 2073 7472 2870 7956 6172 6961 626c  rn str(pyVariabl
-00000e90: 6529 2e72 6570 6c61 6365 2827 5c27 272c  e).replace('\'',
-00000ea0: 2027 5c22 2729 0d0a 2020 2020 2020 2020   '\"')..        
-00000eb0: 2020 2020 2020 2020 656c 6966 2061 6c6c          elif all
-00000ec0: 285b 4751 4c4f 626a 6563 7420 696e 2069  ([GQLObject in i
-00000ed0: 6e73 7065 6374 2e67 6574 6d72 6f28 7479  nspect.getmro(ty
-00000ee0: 7065 2865 6c29 2920 666f 7220 656c 2069  pe(el)) for el i
-00000ef0: 6e20 656c 656d 656e 7473 5d29 3a0d 0a20  n elements]):.. 
-00000f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000f10: 2020 2072 6574 7572 6e20 2720 5b20 2720     return ' [ ' 
-00000f20: 2b20 272c 2027 2e6a 6f69 6e28 5b54 7261  + ', '.join([Tra
-00000f30: 6e73 6c61 7465 2e74 6f5f 6a73 6f6e 5f76  nslate.to_json_v
-00000f40: 6172 7328 6173 6469 6374 2865 6c29 2920  ars(asdict(el)) 
-00000f50: 666f 7220 656c 2069 6e20 656c 656d 656e  for el in elemen
-00000f60: 7473 5d29 202b 2027 205d 2027 0d0a 2020  ts]) + ' ] '..  
-00000f70: 2020 2020 2020 2020 2020 2020 2020 656c                el
-00000f80: 6966 2061 6e79 285b 7479 7065 2865 6c29  if any([type(el)
-00000f90: 2069 6e20 5052 494d 4954 4956 4553 2066   in PRIMITIVES f
-00000fa0: 6f72 2065 6c20 696e 2065 6c65 6d65 6e74  or el in element
-00000fb0: 735d 293a 0d0a 2020 2020 2020 2020 2020  s]):..          
-00000fc0: 2020 2020 2020 2020 2020 7061 7373 2023            pass #
-00000fd0: 7069 7461 0d0a 2020 2020 2020 2020 2020  pita..          
-00000fe0: 2020 2020 2020 656c 7365 3a0d 0a20 2020        else:..   
-00000ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001000: 2070 6173 7320 2377 6861 740d 0a20 2020   pass #what..   
-00001010: 2020 2020 2020 2020 2065 6c69 6620 2063           elif  c
-00001020: 7572 725f 7479 7065 203d 3d20 7479 7065  urr_type == type
-00001030: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00001040: 2020 2072 6574 7572 6e20 275c 2227 202b     return '\"' +
-00001050: 2073 7472 2870 7956 6172 6961 626c 6529   str(pyVariable)
-00001060: 2e72 6570 6c61 6365 2827 5c27 272c 2027  .replace('\'', '
-00001070: 5c22 2729 202b 2027 5c22 270d 0a20 2020  \"') + '\"'..   
-00001080: 2020 2020 2020 2020 2065 6c69 6620 456e           elif En
-00001090: 756d 2069 6e20 696e 7370 6563 742e 6765  um in inspect.ge
-000010a0: 746d 726f 2863 7572 725f 7479 7065 293a  tmro(curr_type):
-000010b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000010c0: 2020 7265 7475 726e 275c 2227 202b 2020    return'\"' +  
-000010d0: 7079 5661 7269 6162 6c65 2e76 616c 7565  pyVariable.value
-000010e0: 202b 2027 5c22 270d 0a20 2020 2020 2020   + '\"'..       
-000010f0: 2020 2020 2065 6c69 6620 6375 7272 5f74       elif curr_t
-00001100: 7970 6520 3d3d 2064 6963 743a 0d0a 2020  ype == dict:..  
-00001110: 2020 2020 2020 2020 2020 2020 2020 6f75                ou
-00001120: 7470 7574 203d 2027 207b 2027 0d0a 2020  tput = ' { '..  
-00001130: 2020 2020 2020 2020 2020 2020 2020 666f                fo
-00001140: 7220 7661 724b 6579 2c20 7661 7256 616c  r varKey, varVal
-00001150: 7565 2069 6e20 7079 5661 7269 6162 6c65  ue in pyVariable
-00001160: 2e69 7465 6d73 2829 3a0d 0a20 2020 2020  .items():..     
-00001170: 2020 2020 2020 2020 2020 2020 2020 206f                 o
-00001180: 7574 7075 7420 2b3d 2054 7261 6e73 6c61  utput += Transla
-00001190: 7465 2e74 6f5f 6772 6170 6871 6c5f 6669  te.to_graphql_fi
-000011a0: 656c 645f 6e61 6d65 2876 6172 4b65 7929  eld_name(varKey)
-000011b0: 202b 2027 3a20 2720 2b20 5472 616e 736c   + ': ' + Transl
-000011c0: 6174 652e 746f 5f67 7261 7068 716c 5f76  ate.to_graphql_v
-000011d0: 616c 7565 2876 6172 5661 6c75 6529 202b  alue(varValue) +
-000011e0: 2043 4f4d 4d41 5f43 4f4e 4341 540d 0a0d   COMMA_CONCAT...
-000011f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001200: 206f 7574 7075 7420 3d20 6f75 7470 7574   output = output
-00001210: 2e72 656d 6f76 6573 7566 6669 7828 434f  .removesuffix(CO
-00001220: 4d4d 415f 434f 4e43 4154 290d 0a20 2020  MMA_CONCAT)..   
-00001230: 2020 2020 2020 2020 2020 2020 206f 7574               out
-00001240: 7075 7420 2b3d 2027 207d 2027 0d0a 2020  put += ' } '..  
-00001250: 2020 2020 2020 2020 2020 2020 2020 7265                re
-00001260: 7475 726e 206f 7574 7075 740d 0a20 2020  turn output..   
-00001270: 2020 2020 2020 2020 2065 6c73 653a 0d0a           else:..
-00001280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001290: 6c6f 6767 6572 2e77 6172 6e69 6e67 2827  logger.warning('
-000012a0: 746f 206d 616e 6167 6527 290d 0a20 2020  to manage')..   
-000012b0: 2020 2020 2065 7863 6570 7420 4578 6365       except Exce
-000012c0: 7074 696f 6e20 6173 2065 783a 0d0a 2020  ption as ex:..  
-000012d0: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-000012e0: 6861 6e64 6c65 5f72 6563 7572 7369 7665  handle_recursive
-000012f0: 5f65 7828 6578 2c20 2745 7272 6f72 2064  _ex(ex, 'Error d
-00001300: 7572 696e 6720 666f 726d 6174 7469 6e67  uring formatting
-00001310: 206f 6620 6772 6170 6871 6c20 7661 6c75   of graphql valu
-00001320: 6520 666f 7220 2720 2b20 7079 5661 7269  e for ' + pyVari
-00001330: 6162 6c65 290d 0a0d 0a20 2020 2064 6566  able)....    def
-00001340: 2074 6f5f 6772 6170 6871 6c5f 7479 7065   to_graphql_type
-00001350: 2870 7956 6172 6961 626c 652c 2076 6172  (pyVariable, var
-00001360: 5f74 7970 6520 3d20 4e6f 6e65 293a 0d0a  _type = None):..
-00001370: 2020 2020 2020 2020 6375 7272 5f74 7970          curr_typ
-00001380: 6520 3d20 7079 5661 7269 6162 6c65 2e5f  e = pyVariable._
-00001390: 5f63 6c61 7373 5f5f 2069 6620 6e6f 7420  _class__ if not 
-000013a0: 7661 725f 7479 7065 2065 6c73 6520 7661  var_type else va
-000013b0: 725f 7479 7065 0d0a 2020 2020 2020 2020  r_type..        
-000013c0: 6772 6170 6871 6c5f 7479 7065 203d 2027  graphql_type = '
-000013d0: 270d 0a20 2020 2020 2020 2069 735f 6e6f  '..        is_no
-000013e0: 6e5f 6e75 6c6c 203d 2046 616c 7365 0d0a  n_null = False..
-000013f0: 2020 2020 2020 2020 6966 2074 7970 6528          if type(
-00001400: 7079 5661 7269 6162 6c65 2920 3d3d 2047  pyVariable) == G
-00001410: 656e 6572 6963 416c 6961 733a 0d0a 2020  enericAlias:..  
-00001420: 2020 2020 2020 2020 2020 6966 2070 7956            if pyV
-00001430: 6172 6961 626c 652e 5f5f 6e61 6d65 5f5f  ariable.__name__
-00001440: 2e73 7461 7274 7377 6974 6828 4e4f 4e5f  .startswith(NON_
-00001450: 4e55 4c4c 5f50 5245 4649 5829 3a0d 0a20  NULL_PREFIX):.. 
-00001460: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00001470: 735f 6e6f 6e5f 6e75 6c6c 203d 2054 7275  s_non_null = Tru
-00001480: 650d 0a20 2020 2020 2020 2020 2020 2020  e..             
-00001490: 2020 2063 7572 725f 7479 7065 203d 2069     curr_type = i
-000014a0: 6e73 7065 6374 2e67 6574 6d72 6f28 7079  nspect.getmro(py
-000014b0: 5661 7269 6162 6c65 2e5f 5f6f 7269 6769  Variable.__origi
-000014c0: 6e5f 5f29 5b31 5d20 2367 6574 2070 6172  n__)[1] #get par
-000014d0: 656e 740d 0a20 2020 2020 2020 2020 2020  ent..           
-000014e0: 2020 2020 2063 7572 725f 7479 7065 5f65       curr_type_e
-000014f0: 6c20 3d20 7079 5661 7269 6162 6c65 2e5f  l = pyVariable._
-00001500: 5f61 7267 735f 5f5b 305d 0d0a 2020 2020  _args__[0]..    
-00001510: 2020 2020 6966 2063 7572 725f 7479 7065      if curr_type
-00001520: 2e5f 5f6e 616d 655f 5f2e 7374 6172 7473  .__name__.starts
-00001530: 7769 7468 284e 4f4e 5f4e 554c 4c5f 5052  with(NON_NULL_PR
-00001540: 4546 4958 293a 0d0a 2020 2020 2020 2020  EFIX):..        
-00001550: 2020 2020 6973 5f6e 6f6e 5f6e 756c 6c20      is_non_null 
-00001560: 3d20 5472 7565 0d0a 2020 2020 2020 2020  = True..        
-00001570: 2020 2020 6375 7272 5f74 7970 6520 3d20      curr_type = 
-00001580: 696e 7370 6563 742e 6765 746d 726f 2863  inspect.getmro(c
-00001590: 7572 725f 7479 7065 295b 315d 0d0a 2020  urr_type)[1]..  
-000015a0: 2020 2020 2020 6966 2067 7261 7068 716c        if graphql
-000015b0: 5f74 7970 6520 3a3d 2073 7769 7463 685f  _type := switch_
-000015c0: 7079 5f67 716c 5f74 7970 652e 6765 7428  py_gql_type.get(
-000015d0: 6375 7272 5f74 7970 652e 5f5f 6e61 6d65  curr_type.__name
-000015e0: 5f5f 2c20 4e6f 6e65 293a 0d0a 2020 2020  __, None):..    
-000015f0: 2020 2020 2020 2020 7061 7373 0d0a 2020          pass..  
-00001600: 2020 2020 2020 656c 6966 2063 7572 725f        elif curr_
-00001610: 7479 7065 203d 3d20 6c69 7374 3a20 2377  type == list: #w
-00001620: 6865 6e20 6361 6c6c 696e 6720 746f 5f67  hen calling to_g
-00001630: 7261 7068 716c 5f74 7970 6520 6e6f 6e20  raphql_type non 
-00001640: 6e75 6c6c 206f 626a 6563 7420 6973 2061  null object is a
-00001650: 6c72 6561 6479 2065 7870 6563 7465 6420  lready expected 
-00001660: 6265 6361 7573 6520 6f66 2063 6865 636b  because of check
-00001670: 5f61 7267 5f0d 0a20 2020 2020 2020 2020  _arg_..         
-00001680: 2020 2067 7261 7068 716c 5f74 7970 6520     graphql_type 
-00001690: 3d20 275b 2720 2b20 5472 616e 736c 6174  = '[' + Translat
-000016a0: 652e 746f 5f67 7261 7068 716c 5f74 7970  e.to_graphql_typ
-000016b0: 6528 7079 5661 7269 6162 6c65 5b30 5d20  e(pyVariable[0] 
-000016c0: 6966 206e 6f74 2069 735f 6e6f 6e5f 6e75  if not is_non_nu
-000016d0: 6c6c 2065 6c73 6520 6375 7272 5f74 7970  ll else curr_typ
-000016e0: 655f 656c 2920 2b20 275d 270d 0a20 2020  e_el) + ']'..   
-000016f0: 2020 2020 2065 6c69 6620 6375 7272 5f74       elif curr_t
-00001700: 7970 6520 3d3d 2074 7970 653a 2023 7368  ype == type: #sh
-00001710: 6f75 6c64 206e 6576 6572 2067 6574 2069  ould never get i
-00001720: 6e0d 0a20 2020 2020 2020 2020 2020 2067  n..            g
-00001730: 7261 7068 716c 5f74 7970 6520 3d20 2754  raphql_type = 'T
-00001740: 7970 6527 0d0a 2020 2020 2020 2020 656c  ype'..        el
-00001750: 6966 2063 7572 725f 7479 7065 203d 3d20  if curr_type == 
-00001760: 6469 6374 3a0d 0a20 2020 2020 2020 2020  dict:..         
-00001770: 2020 206f 7574 7075 7420 3d20 2720 7b20     output = ' { 
-00001780: 270d 0a20 2020 2020 2020 2020 2020 2066  '..            f
-00001790: 6f72 2076 6172 4b65 792c 2076 6172 5661  or varKey, varVa
-000017a0: 6c75 6520 696e 2070 7956 6172 6961 626c  lue in pyVariabl
-000017b0: 652e 6974 656d 7328 293a 0d0a 2020 2020  e.items():..    
-000017c0: 2020 2020 2020 2020 2020 2020 6f75 7470              outp
-000017d0: 7574 202b 3d20 2724 2720 2b20 5472 616e  ut += '$' + Tran
-000017e0: 736c 6174 652e 746f 5f67 7261 7068 716c  slate.to_graphql
-000017f0: 5f66 6965 6c64 5f6e 616d 6528 7661 724b  _field_name(varK
-00001800: 6579 2920 2b20 273a 2027 202b 2054 7261  ey) + ': ' + Tra
-00001810: 6e73 6c61 7465 2e74 6f5f 6772 6170 6871  nslate.to_graphq
-00001820: 6c5f 7479 7065 2876 6172 5661 6c75 6529  l_type(varValue)
-00001830: 202b 2043 4f4d 4d41 5f43 4f4e 4341 540d   + COMMA_CONCAT.
-00001840: 0a0d 0a20 2020 2020 2020 2020 2020 206f  ...            o
-00001850: 7574 7075 7420 3d20 6f75 7470 7574 2e72  utput = output.r
-00001860: 656d 6f76 6573 7566 6669 7828 434f 4d4d  emovesuffix(COMM
-00001870: 415f 434f 4e43 4154 290d 0a20 2020 2020  A_CONCAT)..     
-00001880: 2020 2020 2020 206f 7574 7075 7420 2b3d         output +=
-00001890: 2027 207d 2027 0d0a 2020 2020 2020 2020   ' } '..        
-000018a0: 2020 2020 7265 7475 726e 206f 7574 7075      return outpu
-000018b0: 740d 0a20 2020 2020 2020 2065 6c69 6620  t..        elif 
-000018c0: 456e 756d 2069 6e20 696e 7370 6563 742e  Enum in inspect.
-000018d0: 6765 746d 726f 2863 7572 725f 7479 7065  getmro(curr_type
-000018e0: 2920 6f72 2069 6e73 7065 6374 2e69 7363  ) or inspect.isc
-000018f0: 6c61 7373 2863 7572 725f 7479 7065 293a  lass(curr_type):
-00001900: 0d0a 2020 2020 2020 2020 2020 2020 6772  ..            gr
-00001910: 6170 6871 6c5f 7479 7065 203d 2063 7572  aphql_type = cur
-00001920: 725f 7479 7065 2e5f 5f6e 616d 655f 5f0d  r_type.__name__.
-00001930: 0a20 2020 2020 2020 2065 6c73 653a 0d0a  .        else:..
-00001940: 2020 2020 2020 2020 2020 2020 7261 6973              rais
-00001950: 6520 6861 6e64 6c65 5f72 6563 7572 7369  e handle_recursi
-00001960: 7665 5f65 7828 4578 6365 7074 696f 6e28  ve_ex(Exception(
-00001970: 2774 7970 6520 6e6f 7420 6d61 6e61 6765  'type not manage
-00001980: 6421 2729 2c20 2727 290d 0a0d 0a20 2020  d!'), '')....   
-00001990: 2020 2020 2072 6574 7572 6e20 6772 6170       return grap
-000019a0: 6871 6c5f 7479 7065 202b 2028 2721 2720  hql_type + ('!' 
-000019b0: 6966 2069 735f 6e6f 6e5f 6e75 6c6c 2065  if is_non_null e
-000019c0: 6c73 6520 2727 290d 0a0d 0a20 2020 2064  lse '')....    d
-000019d0: 6566 2074 6f5f 7079 7468 6f6e 5f74 7970  ef to_python_typ
-000019e0: 6528 7479 7065 4e61 6d65 293a 0d0a 2020  e(typeName):..  
-000019f0: 2020 2020 2020 7265 7475 726e 2073 7769        return swi
-00001a00: 7463 685f 6771 6c5f 7079 5f74 7970 652e  tch_gql_py_type.
-00001a10: 6765 7428 7479 7065 4e61 6d65 2c20 7479  get(typeName, ty
-00001a20: 7065 4e61 6d65 290d 0a0d 0a20 2020 2064  peName)....    d
-00001a30: 6566 2074 6f5f 6a73 6f6e 5f76 6172 7328  ef to_json_vars(
-00001a40: 6669 656c 6473 3a20 6469 6374 293a 0d0a  fields: dict):..
-00001a50: 2020 2020 2020 2020 6f75 7470 7574 203d          output =
-00001a60: 2027 270d 0a20 2020 2020 2020 2074 7279   ''..        try
-00001a70: 3a0d 0a20 2020 2020 2020 2020 2020 2066  :..            f
-00001a80: 6f72 2066 6965 6c64 4e61 6d65 2c20 6669  or fieldName, fi
-00001a90: 656c 6456 616c 7565 2069 6e20 6669 656c  eldValue in fiel
-00001aa0: 6473 2e69 7465 6d73 2829 3a0d 0a20 2020  ds.items():..   
-00001ab0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00001ac0: 6973 5f65 6d70 7479 5f66 6965 6c64 2866  is_empty_field(f
-00001ad0: 6965 6c64 5661 6c75 6529 3a20 636f 6e74  ieldValue): cont
-00001ae0: 696e 7565 0d0a 2020 2020 2020 2020 2020  inue..          
-00001af0: 2020 2020 2020 7472 793a 0d0a 2020 2020        try:..    
-00001b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001b10: 6f75 7470 7574 202b 3d20 272c 2027 2069  output += ', ' i
-00001b20: 6620 6f75 7470 7574 2e73 7461 7274 7377  f output.startsw
-00001b30: 6974 6828 277b 2729 2065 6c73 6520 277b  ith('{') else '{
-00001b40: 2027 0d0a 2020 2020 2020 2020 2020 2020   '..            
-00001b50: 2020 2020 2020 2020 6f75 7470 7574 202b          output +
-00001b60: 3d20 275c 2227 202b 2054 7261 6e73 6c61  = '\"' + Transla
-00001b70: 7465 2e74 6f5f 6772 6170 6871 6c5f 6669  te.to_graphql_fi
-00001b80: 656c 645f 6e61 6d65 2866 6965 6c64 4e61  eld_name(fieldNa
-00001b90: 6d65 2920 2b20 2027 5c22 203a 270d 0a20  me) +  '\" :'.. 
-00001ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001bb0: 2020 2066 726f 6d20 7079 6771 6c6d 6170     from pygqlmap
-00001bc0: 2e63 6f6d 706f 6e65 6e74 7320 696d 706f  .components impo
-00001bd0: 7274 2047 514c 4f62 6a65 6374 0d0a 2020  rt GQLObject..  
-00001be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001bf0: 2020 6966 2047 514c 4f62 6a65 6374 2069    if GQLObject i
-00001c00: 6e20 696e 7370 6563 742e 6765 746d 726f  n inspect.getmro
-00001c10: 2874 7970 6528 6669 656c 6456 616c 7565  (type(fieldValue
-00001c20: 2929 3a0d 0a20 2020 2020 2020 2020 2020  )):..           
-00001c30: 2020 2020 2020 2020 2020 2020 206f 7574               out
-00001c40: 7075 7420 2b3d 2054 7261 6e73 6c61 7465  put += Translate
-00001c50: 2e74 6f5f 6a73 6f6e 5f76 6172 7328 6669  .to_json_vars(fi
-00001c60: 656c 6456 616c 7565 2e5f 5f64 6963 745f  eldValue.__dict_
-00001c70: 5f29 0d0a 2020 2020 2020 2020 2020 2020  _)..            
-00001c80: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
-00001c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001ca0: 2020 2020 2020 206f 7574 7075 7420 2b3d         output +=
-00001cb0: 2054 7261 6e73 6c61 7465 2e74 6f5f 6a73   Translate.to_js
-00001cc0: 6f6e 5f76 616c 7565 2866 6965 6c64 5661  on_value(fieldVa
-00001cd0: 6c75 6529 0d0a 2020 2020 2020 2020 2020  lue)..          
-00001ce0: 2020 2020 2020 6578 6365 7074 2045 7863        except Exc
-00001cf0: 6570 7469 6f6e 2061 7320 6578 3a0d 0a20  eption as ex:.. 
-00001d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001d10: 2020 2072 6169 7365 2068 616e 646c 655f     raise handle_
-00001d20: 7265 6375 7273 6976 655f 6578 2865 782c  recursive_ex(ex,
-00001d30: 2027 4973 7375 6520 6578 706f 7274 696e   'Issue exportin
-00001d40: 6720 7661 7269 6162 6c65 2066 6f72 3a20  g variable for: 
-00001d50: 2720 2b20 6669 656c 644e 616d 6529 0d0a  ' + fieldName)..
-00001d60: 0d0a 2020 2020 2020 2020 2020 2020 6f75  ..            ou
-00001d70: 7470 7574 2e72 656d 6f76 6573 7566 6669  tput.removesuffi
-00001d80: 7828 434f 4d4d 415f 434f 4e43 4154 290d  x(COMMA_CONCAT).
-00001d90: 0a20 2020 2020 2020 2065 7863 6570 7420  .        except 
-00001da0: 4578 6365 7074 696f 6e20 6173 2065 783a  Exception as ex:
-00001db0: 0d0a 2020 2020 2020 2020 2020 2020 7261  ..            ra
-00001dc0: 6973 6520 6861 6e64 6c65 5f72 6563 7572  ise handle_recur
-00001dd0: 7369 7665 5f65 7828 6578 2c20 2749 7373  sive_ex(ex, 'Iss
-00001de0: 7565 2077 6974 6820 6974 656d 7320 6578  ue with items ex
-00001df0: 706f 7274 696e 6720 7661 7269 6162 6c65  porting variable
-00001e00: 2729 0d0a 0d0a 2020 2020 2020 2020 6f75  ')....        ou
-00001e10: 7470 7574 202b 3d20 2720 7d27 0d0a 2020  tput += ' }'..  
-00001e20: 2020 2020 2020 7265 7475 726e 206f 7574        return out
-00001e30: 7075 740d 0a0d 0a20 2020 2064 6566 2067  put....    def g
-00001e40: 7261 7068 716c 697a 6528 696e 7075 7453  raphqlize(inputS
-00001e50: 6f75 7263 6544 6963 742c 2061 7267 7354  ourceDict, argsT
-00001e60: 6f49 676e 6f72 6520 3d20 4e6f 6e65 293a  oIgnore = None):
-00001e70: 0d0a 2020 2020 2020 2020 7472 793a 0d0a  ..        try:..
-00001e80: 2020 2020 2020 2020 2020 2020 6f75 7470              outp
-00001e90: 7574 3d20 2727 0d0a 2020 2020 2020 2020  ut= ''..        
-00001ea0: 2020 2020 666f 7220 696e 7075 7453 6f75      for inputSou
-00001eb0: 7263 654b 6579 2c20 696e 7075 7453 6f75  rceKey, inputSou
-00001ec0: 7263 6556 616c 7565 2069 6e20 696e 7075  rceValue in inpu
-00001ed0: 7453 6f75 7263 6544 6963 742e 6974 656d  tSourceDict.item
-00001ee0: 7328 293a 0d0a 2020 2020 2020 2020 2020  s():..          
-00001ef0: 2020 2020 2020 6966 2069 7369 6e73 7461        if isinsta
-00001f00: 6e63 6528 696e 7075 7453 6f75 7263 6556  nce(inputSourceV
-00001f10: 616c 7565 2c20 6469 6374 293a 0d0a 2020  alue, dict):..  
-00001f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001f30: 2020 7072 696e 7428 2747 6574 7469 6e67    print('Getting
-00001f40: 2069 6e74 6f20 2720 2b20 696e 7075 7453   into ' + inputS
-00001f50: 6f75 7263 654b 6579 290d 0a20 2020 2020  ourceKey)..     
-00001f60: 2020 2020 2020 2020 2020 2020 2020 206f                 o
-00001f70: 7574 7075 7420 2b3d 2069 6e70 7574 536f  utput += inputSo
-00001f80: 7572 6365 4b65 7920 2b20 2861 7267 7354  urceKey + (argsT
-00001f90: 6f49 676e 6f72 6520 6966 2061 7267 7354  oIgnore if argsT
-00001fa0: 6f49 676e 6f72 6520 656c 7365 2027 2729  oIgnore else '')
-00001fb0: 202b 2027 207b 2027 202b 2054 7261 6e73   + ' { ' + Trans
-00001fc0: 6c61 7465 2e67 7261 7068 716c 697a 6528  late.graphqlize(
-00001fd0: 696e 7075 7453 6f75 7263 6556 616c 7565  inputSourceValue
-00001fe0: 2920 2b20 2720 7d20 270d 0a20 2020 2020  ) + ' } '..     
-00001ff0: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
-00002000: 6973 696e 7374 616e 6365 2869 6e70 7574  isinstance(input
-00002010: 536f 7572 6365 5661 6c75 652c 2074 7570  SourceValue, tup
-00002020: 6c65 293a 0d0a 2020 2020 2020 2020 2020  le):..          
-00002030: 2020 2020 2020 2020 2020 6966 2069 7369            if isi
-00002040: 6e73 7461 6e63 6528 696e 7075 7453 6f75  nstance(inputSou
-00002050: 7263 6556 616c 7565 5b31 5d2c 2064 6963  rceValue[1], dic
-00002060: 7429 3a0d 0a20 2020 2020 2020 2020 2020  t):..           
-00002070: 2020 2020 2020 2020 2020 2020 206f 7574               out
-00002080: 7075 7420 2b3d 2069 6e70 7574 536f 7572  put += inputSour
-00002090: 6365 4b65 7920 2b20 696e 7075 7453 6f75  ceKey + inputSou
-000020a0: 7263 6556 616c 7565 5b30 5d20 2b20 2720  rceValue[0] + ' 
-000020b0: 7b20 2720 2b20 5472 616e 736c 6174 652e  { ' + Translate.
-000020c0: 6772 6170 6871 6c69 7a65 2869 6e70 7574  graphqlize(input
-000020d0: 536f 7572 6365 5661 6c75 655b 315d 2920  SourceValue[1]) 
-000020e0: 2b20 2720 7d20 270d 0a20 2020 2020 2020  + ' } '..       
-000020f0: 2020 2020 2020 2020 2065 6c73 653a 0d0a           else:..
-00002100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002110: 2020 2020 6f75 7470 7574 202b 3d20 6578      output += ex
-00002120: 6563 7574 655f 7265 6765 7828 2220 2220  ecute_regex(" " 
-00002130: 2b20 696e 7075 7453 6f75 7263 654b 6579  + inputSourceKey
-00002140: 202b 2022 2022 290d 0a20 2020 2020 2020   + " ")..       
-00002150: 2065 7863 6570 7420 4578 6365 7074 696f   except Exceptio
-00002160: 6e20 6173 2065 783a 0d0a 2020 2020 2020  n as ex:..      
-00002170: 2020 2020 2020 7261 6973 6520 6861 6e64        raise hand
-00002180: 6c65 5f72 6563 7572 7369 7665 5f65 7828  le_recursive_ex(
-00002190: 6578 2c20 2745 7863 6570 7469 6f6e 2064  ex, 'Exception d
-000021a0: 7572 696e 6720 6772 6170 6871 6c69 7a69  uring graphqlizi
-000021b0: 6e67 206f 6620 2720 2b20 7374 7228 696e  ng of ' + str(in
-000021c0: 7075 7453 6f75 7263 6544 6963 7429 290d  putSourceDict)).
-000021d0: 0a0d 0a20 2020 2020 2020 2072 6574 7572  ...        retur
-000021e0: 6e20 6f75 7470 7574 0d0a 0d0a 2020 2020  n output....    
-000021f0: 6465 6620 6578 636c 7564 655f 6172 6773  def exclude_args
-00002200: 5f73 7562 7374 7269 6e67 2864 6174 6149  _substring(dataI
-00002210: 6e70 7574 3a20 7374 722c 2061 7267 7354  nput: str, argsT
-00002220: 6f49 676e 6f72 653a 206c 6973 7429 3a0d  oIgnore: list):.
-00002230: 0a20 2020 2020 2020 2066 6f72 2061 7267  .        for arg
-00002240: 7320 696e 2061 7267 7354 6f49 676e 6f72  s in argsToIgnor
-00002250: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-00002260: 7472 793a 0d0a 2020 2020 2020 2020 2020  try:..          
-00002270: 2020 2020 2020 6966 2073 7472 2864 6174        if str(dat
-00002280: 6149 6e70 7574 292e 5f5f 636f 6e74 6169  aInput).__contai
-00002290: 6e73 5f5f 2861 7267 7329 3a0d 0a20 2020  ns__(args):..   
-000022a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000022b0: 206c 6f67 6765 722e 696e 666f 2827 7370   logger.info('sp
-000022c0: 6c69 7474 696e 6720 2720 2b20 6461 7461  litting ' + data
-000022d0: 496e 7075 7429 0d0a 2020 2020 2020 2020  Input)..        
-000022e0: 2020 2020 2020 2020 2020 2020 696e 7075              inpu
-000022f0: 744c 6973 7420 3d20 6461 7461 496e 7075  tList = dataInpu
-00002300: 742e 7370 6c69 7428 6172 6773 290d 0a20  t.split(args).. 
-00002310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002320: 2020 2072 6574 7572 6e20 6172 6773 2e6a     return args.j
-00002330: 6f69 6e28 5472 616e 736c 6174 652e 6578  oin(Translate.ex
-00002340: 636c 7564 655f 6172 6773 5f73 7562 7374  clude_args_subst
-00002350: 7269 6e67 2878 2c20 6172 6773 546f 4967  ring(x, argsToIg
-00002360: 6e6f 7265 2920 666f 7220 7820 696e 2069  nore) for x in i
-00002370: 6e70 7574 4c69 7374 290d 0a20 2020 2020  nputList)..     
-00002380: 2020 2020 2020 2065 7863 6570 7420 4578         except Ex
-00002390: 6365 7074 696f 6e20 6173 2065 783a 0d0a  ception as ex:..
-000023a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000023b0: 7261 6973 6520 6861 6e64 6c65 5f72 6563  raise handle_rec
-000023c0: 7572 7369 7665 5f65 7828 6578 2c20 2745  ursive_ex(ex, 'E
-000023d0: 7863 6570 7469 6f6e 2064 7572 696e 6720  xception during 
-000023e0: 6172 6773 2065 7863 6c75 7369 6f6e 2066  args exclusion f
-000023f0: 726f 6d20 6772 6170 6871 6c69 7a65 2066  rom graphqlize f
-00002400: 6f72 2073 7562 7374 7269 6e67 2027 202b  or substring ' +
-00002410: 2064 6174 6149 6e70 7574 290d 0a0d 0a20   dataInput).... 
-00002420: 2020 2020 2020 2072 6574 7572 6e20 6578         return ex
-00002430: 6563 7574 655f 7265 6765 7828 6461 7461  ecute_regex(data
-00002440: 496e 7075 7429 0d0a 0d0a 2020 2020 6465  Input)....    de
-00002450: 6620 746f 5f67 7261 7068 716c 5f61 7267  f to_graphql_arg
-00002460: 7373 6574 5f64 6566 696e 6974 696f 6e28  sset_definition(
-00002470: 7079 4f62 6a65 6374 293a 0d0a 2020 2020  pyObject):..    
-00002480: 2020 2020 6f75 7470 7574 203d 2027 270d      output = ''.
-00002490: 0a0d 0a20 2020 2020 2020 2074 7279 3a0d  ...        try:.
-000024a0: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
-000024b0: 2066 6965 6c64 2069 6e20 7079 4f62 6a65   field in pyObje
-000024c0: 6374 2e5f 5f64 6174 6163 6c61 7373 5f66  ct.__dataclass_f
-000024d0: 6965 6c64 735f 5f3a 0d0a 2020 2020 2020  ields__:..      
-000024e0: 2020 2020 2020 2020 2020 6f62 6a65 6374            object
-000024f0: 4669 656c 6420 3d20 6765 7461 7474 7228  Field = getattr(
-00002500: 7079 4f62 6a65 6374 2c20 6669 656c 6429  pyObject, field)
-00002510: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00002520: 2020 6966 2069 735f 656d 7074 795f 6669    if is_empty_fi
-00002530: 656c 6428 6f62 6a65 6374 4669 656c 6429  eld(objectField)
-00002540: 3a20 636f 6e74 696e 7565 0d0a 2020 2020  : continue..    
-00002550: 2020 2020 2020 2020 2020 2020 7472 793a              try:
-00002560: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00002570: 2020 2020 2020 6672 6f6d 2070 7967 716c        from pygql
-00002580: 6d61 702e 636f 6d70 6f6e 656e 7473 2069  map.components i
-00002590: 6d70 6f72 7420 4751 4c4f 626a 6563 740d  mport GQLObject.
-000025a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000025b0: 2020 2020 2069 6620 4751 4c4f 626a 6563       if GQLObjec
-000025c0: 7420 696e 2069 6e73 7065 6374 2e67 6574  t in inspect.get
-000025d0: 6d72 6f28 7479 7065 286f 626a 6563 7446  mro(type(objectF
-000025e0: 6965 6c64 2929 3a0d 0a20 2020 2020 2020  ield)):..       
-000025f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002600: 206f 7574 7075 7420 2b3d 2066 6965 6c64   output += field
-00002610: 202b 2027 3a20 7b20 2720 2b20 5472 616e   + ': { ' + Tran
-00002620: 736c 6174 652e 746f 5f67 7261 7068 716c  slate.to_graphql
-00002630: 5f61 7267 7373 6574 5f64 6566 696e 6974  _argsset_definit
-00002640: 696f 6e28 6f62 6a65 6374 4669 656c 6429  ion(objectField)
-00002650: 202b 2027 207d 2027 0d0a 2020 2020 2020   + ' } '..      
-00002660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002670: 2020 6f75 7470 7574 202b 3d20 434f 4d4d    output += COMM
-00002680: 415f 434f 4e43 4154 0d0a 2020 2020 2020  A_CONCAT..      
-00002690: 2020 2020 2020 2020 2020 2020 2020 656c                el
-000026a0: 6966 2069 7369 6e73 7461 6e63 6528 6f62  if isinstance(ob
-000026b0: 6a65 6374 4669 656c 642c 206c 6973 7429  jectField, list)
-000026c0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-000026d0: 2020 2020 2020 2020 2020 206f 7574 7075             outpu
-000026e0: 7420 2b3d 2066 6965 6c64 202b 2027 3a20  t += field + ': 
-000026f0: 5b20 270d 0a20 2020 2020 2020 2020 2020  [ '..           
-00002700: 2020 2020 2020 2020 2020 2020 2066 6f72               for
-00002710: 2065 6c65 6d65 6e74 4c69 7374 2069 6e20   elementList in 
-00002720: 6f62 6a65 6374 4669 656c 643a 0d0a 2020  objectField:..  
-00002730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002740: 2020 2020 2020 2020 2020 6966 2047 514c            if GQL
-00002750: 4f62 6a65 6374 2069 6e20 696e 7370 6563  Object in inspec
-00002760: 742e 6765 746d 726f 2874 7970 6528 656c  t.getmro(type(el
-00002770: 656d 656e 744c 6973 7429 293a 0d0a 2020  ementList)):..  
-00002780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002790: 2020 2020 2020 2020 2020 2020 2020 6f75                ou
-000027a0: 7470 7574 202b 3d20 2720 7b20 2720 2b20  tput += ' { ' + 
-000027b0: 5472 616e 736c 6174 652e 746f 5f67 7261  Translate.to_gra
-000027c0: 7068 716c 5f61 7267 7373 6574 5f64 6566  phql_argsset_def
-000027d0: 696e 6974 696f 6e28 656c 656d 656e 744c  inition(elementL
-000027e0: 6973 7429 202b 2027 207d 2027 202b 2043  ist) + ' } ' + C
-000027f0: 4f4d 4d41 5f43 4f4e 4341 540d 0a20 2020  OMMA_CONCAT..   
-00002800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002810: 2020 2020 2020 2020 2065 6c73 653a 0d0a           else:..
-00002820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002840: 6f75 7470 7574 202b 3d20 5472 616e 736c  output += Transl
-00002850: 6174 652e 746f 5f67 7261 7068 716c 5f76  ate.to_graphql_v
-00002860: 616c 7565 2865 6c65 6d65 6e74 4c69 7374  alue(elementList
-00002870: 2920 2b20 434f 4d4d 415f 434f 4e43 4154  ) + COMMA_CONCAT
-00002880: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00002890: 2020 2020 2020 2020 2020 6f75 7470 7574            output
-000028a0: 203d 206f 7574 7075 742e 7265 6d6f 7665   = output.remove
-000028b0: 7375 6666 6978 2843 4f4d 4d41 5f43 4f4e  suffix(COMMA_CON
-000028c0: 4341 5429 0d0a 2020 2020 2020 2020 2020  CAT)..          
-000028d0: 2020 2020 2020 2020 2020 2020 2020 6f75                ou
-000028e0: 7470 7574 202b 3d20 2720 5d20 2720 2b20  tput += ' ] ' + 
-000028f0: 434f 4d4d 415f 434f 4e43 4154 0d0a 2020  COMMA_CONCAT..  
-00002900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002910: 2020 656c 7365 3a0d 0a20 2020 2020 2020    else:..       
-00002920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002930: 2069 6620 6861 7361 7474 7228 7079 4f62   if hasattr(pyOb
-00002940: 6a65 6374 2c20 6669 656c 6429 2061 6e64  ject, field) and
-00002950: 206e 6f74 206f 626a 6563 7446 6965 6c64   not objectField
-00002960: 203d 3d20 4e6f 6e65 3a0d 0a20 2020 2020   == None:..     
-00002970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002980: 2020 2020 2020 206f 7574 7075 7420 2b3d         output +=
-00002990: 2054 7261 6e73 6c61 7465 2e74 6f5f 6772   Translate.to_gr
-000029a0: 6170 6871 6c5f 6172 675f 6465 6669 6e69  aphql_arg_defini
-000029b0: 7469 6f6e 2866 6965 6c64 2c20 6f62 6a65  tion(field, obje
-000029c0: 6374 4669 656c 6429 0d0a 2020 2020 2020  ctField)..      
-000029d0: 2020 2020 2020 2020 2020 6578 6365 7074            except
-000029e0: 2045 7863 6570 7469 6f6e 2061 7320 6578   Exception as ex
-000029f0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00002a00: 2020 2020 2020 2072 6169 7365 2068 616e         raise han
-00002a10: 646c 655f 7265 6375 7273 6976 655f 6578  dle_recursive_ex
-00002a20: 2865 782c 2027 4973 7375 6520 6475 7269  (ex, 'Issue duri
-00002a30: 6e67 2065 7870 6f72 7420 6f66 206e 616d  ng export of nam
-00002a40: 6520 616e 6420 7661 6c75 6520 666f 723a  e and value for:
-00002a50: 2027 202b 206f 626a 6563 7446 6965 6c64   ' + objectField
-00002a60: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
-00002a70: 206f 7574 7075 7420 3d20 6f75 7470 7574   output = output
-00002a80: 2e72 656d 6f76 6573 7566 6669 7828 434f  .removesuffix(CO
-00002a90: 4d4d 415f 434f 4e43 4154 290d 0a0d 0a20  MMA_CONCAT).... 
-00002aa0: 2020 2020 2020 2065 7863 6570 7420 4578         except Ex
-00002ab0: 6365 7074 696f 6e20 6173 2065 783a 0d0a  ception as ex:..
-00002ac0: 2020 2020 2020 2020 2020 2020 7261 6973              rais
-00002ad0: 6520 6861 6e64 6c65 5f72 6563 7572 7369  e handle_recursi
-00002ae0: 7665 5f65 7828 6578 2c20 2745 7272 6f72  ve_ex(ex, 'Error
-00002af0: 2064 7572 696e 6720 7472 616e 736c 6174   during translat
-00002b00: 696f 6e20 6f66 2061 7267 756d 656e 7420  ion of argument 
-00002b10: 7365 7420 6465 6669 6e69 7469 6f6e 2729  set definition')
-00002b20: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-00002b30: 206f 7574 7075 740d 0a0d 0a20 2020 2064   output....    d
-00002b40: 6566 2074 6f5f 6772 6170 6871 6c5f 6172  ef to_graphql_ar
-00002b50: 675f 6465 6669 6e69 7469 6f6e 2866 6965  g_definition(fie
-00002b60: 6c64 4e61 6d65 2c20 6669 656c 6429 3a0d  ldName, field):.
-00002b70: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00002b80: 5472 616e 736c 6174 652e 746f 5f67 7261  Translate.to_gra
-00002b90: 7068 716c 5f66 6965 6c64 5f6e 616d 6528  phql_field_name(
-00002ba0: 6669 656c 644e 616d 6529 202b 2027 3a20  fieldName) + ': 
-00002bb0: 2720 2b20 5472 616e 736c 6174 652e 746f  ' + Translate.to
-00002bc0: 5f67 7261 7068 716c 5f76 616c 7565 2866  _graphql_value(f
-00002bd0: 6965 6c64 2920 2b20 434f 4d4d 415f 434f  ield) + COMMA_CO
-00002be0: 4e43 4154 0d0a                           NCAT..
+00000e50: 206f 7220 4944 2069 6e20 696e 7370 6563   or ID in inspec
+00000e60: 742e 6765 746d 726f 2874 7970 6528 656c  t.getmro(type(el
+00000e70: 2929 2066 6f72 2065 6c20 696e 2065 6c65  )) for el in ele
+00000e80: 6d65 6e74 735d 293a 0d0a 2020 2020 2020  ments]):..      
+00000e90: 2020 2020 2020 2020 2020 2020 2020 7265                re
+00000ea0: 7475 726e 2073 7472 2870 7956 6172 6961  turn str(pyVaria
+00000eb0: 626c 6529 2e72 6570 6c61 6365 2827 5c27  ble).replace('\'
+00000ec0: 272c 2027 5c22 2729 0d0a 2020 2020 2020  ', '\"')..      
+00000ed0: 2020 2020 2020 2020 2020 656c 6966 2061            elif a
+00000ee0: 6c6c 285b 4751 4c4f 626a 6563 7420 696e  ll([GQLObject in
+00000ef0: 2069 6e73 7065 6374 2e67 6574 6d72 6f28   inspect.getmro(
+00000f00: 7479 7065 2865 6c29 2920 666f 7220 656c  type(el)) for el
+00000f10: 2069 6e20 656c 656d 656e 7473 5d29 3a0d   in elements]):.
+00000f20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000f30: 2020 2020 2072 6574 7572 6e20 2720 5b20       return ' [ 
+00000f40: 2720 2b20 272c 2027 2e6a 6f69 6e28 5b54  ' + ', '.join([T
+00000f50: 7261 6e73 6c61 7465 2e74 6f5f 6a73 6f6e  ranslate.to_json
+00000f60: 5f76 6172 7328 6173 6469 6374 2865 6c29  _vars(asdict(el)
+00000f70: 2920 666f 7220 656c 2069 6e20 656c 656d  ) for el in elem
+00000f80: 656e 7473 5d29 202b 2027 205d 2027 0d0a  ents]) + ' ] '..
+00000f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000fa0: 656c 6966 2061 6e79 285b 7479 7065 2865  elif any([type(e
+00000fb0: 6c29 2069 6e20 5052 494d 4954 4956 4553  l) in PRIMITIVES
+00000fc0: 2066 6f72 2065 6c20 696e 2065 6c65 6d65   for el in eleme
+00000fd0: 6e74 735d 293a 0d0a 2020 2020 2020 2020  nts]):..        
+00000fe0: 2020 2020 2020 2020 2020 2020 6c6f 6767              logg
+00000ff0: 6572 2e77 6172 6e69 6e67 2827 4c69 7374  er.warning('List
+00001000: 206f 6620 6879 6272 6964 2074 7970 6573   of hybrid types
+00001010: 2729 0d0a 2020 2020 2020 2020 2020 2020  ')..            
+00001020: 2020 2020 2020 2020 7061 7373 2023 7069          pass #pi
+00001030: 7461 0d0a 2020 2020 2020 2020 2020 2020  ta..            
+00001040: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
+00001050: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+00001060: 6173 7320 2377 6861 740d 0a20 2020 2020  ass #what..     
+00001070: 2020 2020 2020 2065 6c69 6620 2063 7572         elif  cur
+00001080: 725f 7479 7065 203d 3d20 7479 7065 3a0d  r_type == type:.
+00001090: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000010a0: 2072 6574 7572 6e20 275c 2227 202b 2073   return '\"' + s
+000010b0: 7472 2870 7956 6172 6961 626c 6529 2e72  tr(pyVariable).r
+000010c0: 6570 6c61 6365 2827 5c27 272c 2027 5c22  eplace('\'', '\"
+000010d0: 2729 202b 2027 5c22 270d 0a20 2020 2020  ') + '\"'..     
+000010e0: 2020 2020 2020 2065 6c69 6620 456e 756d         elif Enum
+000010f0: 2069 6e20 696e 7370 6563 742e 6765 746d   in inspect.getm
+00001100: 726f 2863 7572 725f 7479 7065 293a 0d0a  ro(curr_type):..
+00001110: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001120: 7265 7475 726e 275c 2227 202b 2020 7079  return'\"' +  py
+00001130: 5661 7269 6162 6c65 2e76 616c 7565 202b  Variable.value +
+00001140: 2027 5c22 270d 0a20 2020 2020 2020 2020   '\"'..         
+00001150: 2020 2065 6c69 6620 6375 7272 5f74 7970     elif curr_typ
+00001160: 6520 3d3d 2064 6963 743a 0d0a 2020 2020  e == dict:..    
+00001170: 2020 2020 2020 2020 2020 2020 6f75 7470              outp
+00001180: 7574 203d 2027 207b 2027 0d0a 2020 2020  ut = ' { '..    
+00001190: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+000011a0: 7661 724b 6579 2c20 7661 7256 616c 7565  varKey, varValue
+000011b0: 2069 6e20 7079 5661 7269 6162 6c65 2e69   in pyVariable.i
+000011c0: 7465 6d73 2829 3a0d 0a20 2020 2020 2020  tems():..       
+000011d0: 2020 2020 2020 2020 2020 2020 206f 7574               out
+000011e0: 7075 7420 2b3d 2054 7261 6e73 6c61 7465  put += Translate
+000011f0: 2e74 6f5f 6772 6170 6871 6c5f 6669 656c  .to_graphql_fiel
+00001200: 645f 6e61 6d65 2876 6172 4b65 7929 202b  d_name(varKey) +
+00001210: 2027 3a20 2720 2b20 5472 616e 736c 6174   ': ' + Translat
+00001220: 652e 746f 5f67 7261 7068 716c 5f76 616c  e.to_graphql_val
+00001230: 7565 2876 6172 5661 6c75 6529 202b 2043  ue(varValue) + C
+00001240: 4f4d 4d41 5f43 4f4e 4341 540d 0a0d 0a20  OMMA_CONCAT.... 
+00001250: 2020 2020 2020 2020 2020 2020 2020 206f                 o
+00001260: 7574 7075 7420 3d20 6f75 7470 7574 2e72  utput = output.r
+00001270: 656d 6f76 6573 7566 6669 7828 434f 4d4d  emovesuffix(COMM
+00001280: 415f 434f 4e43 4154 290d 0a20 2020 2020  A_CONCAT)..     
+00001290: 2020 2020 2020 2020 2020 206f 7574 7075             outpu
+000012a0: 7420 2b3d 2027 207d 2027 0d0a 2020 2020  t += ' } '..    
+000012b0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+000012c0: 726e 206f 7574 7075 740d 0a20 2020 2020  rn output..     
+000012d0: 2020 2020 2020 2065 6c73 653a 0d0a 2020         else:..  
+000012e0: 2020 2020 2020 2020 2020 2020 2020 6c6f                lo
+000012f0: 6767 6572 2e77 6172 6e69 6e67 2827 746f  gger.warning('to
+00001300: 206d 616e 6167 6527 290d 0a20 2020 2020   manage')..     
+00001310: 2020 2065 7863 6570 7420 4578 6365 7074     except Except
+00001320: 696f 6e20 6173 2065 783a 0d0a 2020 2020  ion as ex:..    
+00001330: 2020 2020 2020 2020 7261 6973 6520 6861          raise ha
+00001340: 6e64 6c65 5f72 6563 7572 7369 7665 5f65  ndle_recursive_e
+00001350: 7828 6578 2c20 2745 7272 6f72 2064 7572  x(ex, 'Error dur
+00001360: 696e 6720 666f 726d 6174 7469 6e67 206f  ing formatting o
+00001370: 6620 6772 6170 6871 6c20 7661 6c75 6520  f graphql value 
+00001380: 666f 7220 2720 2b20 7079 5661 7269 6162  for ' + pyVariab
+00001390: 6c65 290d 0a0d 0a20 2020 2064 6566 2074  le)....    def t
+000013a0: 6f5f 6772 6170 6871 6c5f 7479 7065 2870  o_graphql_type(p
+000013b0: 7956 6172 6961 626c 652c 2076 6172 5f74  yVariable, var_t
+000013c0: 7970 6520 3d20 4e6f 6e65 293a 0d0a 2020  ype = None):..  
+000013d0: 2020 2020 2020 6375 7272 5f74 7970 6520        curr_type 
+000013e0: 3d20 7079 5661 7269 6162 6c65 2e5f 5f63  = pyVariable.__c
+000013f0: 6c61 7373 5f5f 2069 6620 6e6f 7420 7661  lass__ if not va
+00001400: 725f 7479 7065 2065 6c73 6520 7661 725f  r_type else var_
+00001410: 7479 7065 0d0a 2020 2020 2020 2020 6772  type..        gr
+00001420: 6170 6871 6c5f 7479 7065 203d 2027 270d  aphql_type = ''.
+00001430: 0a20 2020 2020 2020 2069 735f 6e6f 6e5f  .        is_non_
+00001440: 6e75 6c6c 203d 2046 616c 7365 0d0a 2020  null = False..  
+00001450: 2020 2020 2020 6966 2074 7970 6528 7079        if type(py
+00001460: 5661 7269 6162 6c65 2920 3d3d 2047 656e  Variable) == Gen
+00001470: 6572 6963 416c 6961 733a 0d0a 2020 2020  ericAlias:..    
+00001480: 2020 2020 2020 2020 6966 2070 7956 6172          if pyVar
+00001490: 6961 626c 652e 5f5f 6e61 6d65 5f5f 2e73  iable.__name__.s
+000014a0: 7461 7274 7377 6974 6828 4e4f 4e5f 4e55  tartswith(NON_NU
+000014b0: 4c4c 5f50 5245 4649 5829 3a0d 0a20 2020  LL_PREFIX):..   
+000014c0: 2020 2020 2020 2020 2020 2020 2069 735f               is_
+000014d0: 6e6f 6e5f 6e75 6c6c 203d 2054 7275 650d  non_null = True.
+000014e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000014f0: 2063 7572 725f 7479 7065 203d 2069 6e73   curr_type = ins
+00001500: 7065 6374 2e67 6574 6d72 6f28 7079 5661  pect.getmro(pyVa
+00001510: 7269 6162 6c65 2e5f 5f6f 7269 6769 6e5f  riable.__origin_
+00001520: 5f29 5b31 5d20 2367 6574 2070 6172 656e  _)[1] #get paren
+00001530: 740d 0a20 2020 2020 2020 2020 2020 2020  t..             
+00001540: 2020 2063 7572 725f 7479 7065 5f65 6c20     curr_type_el 
+00001550: 3d20 7079 5661 7269 6162 6c65 2e5f 5f61  = pyVariable.__a
+00001560: 7267 735f 5f5b 305d 0d0a 2020 2020 2020  rgs__[0]..      
+00001570: 2020 6966 2063 7572 725f 7479 7065 2e5f    if curr_type._
+00001580: 5f6e 616d 655f 5f2e 7374 6172 7473 7769  _name__.startswi
+00001590: 7468 284e 4f4e 5f4e 554c 4c5f 5052 4546  th(NON_NULL_PREF
+000015a0: 4958 293a 0d0a 2020 2020 2020 2020 2020  IX):..          
+000015b0: 2020 6973 5f6e 6f6e 5f6e 756c 6c20 3d20    is_non_null = 
+000015c0: 5472 7565 0d0a 2020 2020 2020 2020 2020  True..          
+000015d0: 2020 6375 7272 5f74 7970 6520 3d20 696e    curr_type = in
+000015e0: 7370 6563 742e 6765 746d 726f 2863 7572  spect.getmro(cur
+000015f0: 725f 7479 7065 295b 315d 0d0a 2020 2020  r_type)[1]..    
+00001600: 2020 2020 6966 2067 7261 7068 716c 5f74      if graphql_t
+00001610: 7970 6520 3a3d 2073 7769 7463 685f 7079  ype := switch_py
+00001620: 5f67 716c 5f74 7970 652e 6765 7428 6375  _gql_type.get(cu
+00001630: 7272 5f74 7970 652e 5f5f 6e61 6d65 5f5f  rr_type.__name__
+00001640: 2c20 4e6f 6e65 293a 0d0a 2020 2020 2020  , None):..      
+00001650: 2020 2020 2020 7061 7373 0d0a 2020 2020        pass..    
+00001660: 2020 2020 656c 6966 2063 7572 725f 7479      elif curr_ty
+00001670: 7065 203d 3d20 6c69 7374 3a20 2377 6865  pe == list: #whe
+00001680: 6e20 6361 6c6c 696e 6720 746f 5f67 7261  n calling to_gra
+00001690: 7068 716c 5f74 7970 6520 6e6f 6e20 6e75  phql_type non nu
+000016a0: 6c6c 206f 626a 6563 7420 6973 2061 6c72  ll object is alr
+000016b0: 6561 6479 2065 7870 6563 7465 6420 6265  eady expected be
+000016c0: 6361 7573 6520 6f66 2063 6865 636b 5f61  cause of check_a
+000016d0: 7267 5f0d 0a20 2020 2020 2020 2020 2020  rg_..           
+000016e0: 2067 7261 7068 716c 5f74 7970 6520 3d20   graphql_type = 
+000016f0: 275b 2720 2b20 5472 616e 736c 6174 652e  '[' + Translate.
+00001700: 746f 5f67 7261 7068 716c 5f74 7970 6528  to_graphql_type(
+00001710: 7079 5661 7269 6162 6c65 5b30 5d20 6966  pyVariable[0] if
+00001720: 206e 6f74 2069 735f 6e6f 6e5f 6e75 6c6c   not is_non_null
+00001730: 2065 6c73 6520 6375 7272 5f74 7970 655f   else curr_type_
+00001740: 656c 2920 2b20 275d 270d 0a20 2020 2020  el) + ']'..     
+00001750: 2020 2065 6c69 6620 6375 7272 5f74 7970     elif curr_typ
+00001760: 6520 3d3d 2074 7970 653a 2023 7368 6f75  e == type: #shou
+00001770: 6c64 206e 6576 6572 2067 6574 2069 6e0d  ld never get in.
+00001780: 0a20 2020 2020 2020 2020 2020 2067 7261  .            gra
+00001790: 7068 716c 5f74 7970 6520 3d20 2754 7970  phql_type = 'Typ
+000017a0: 6527 0d0a 2020 2020 2020 2020 656c 6966  e'..        elif
+000017b0: 2063 7572 725f 7479 7065 203d 3d20 6469   curr_type == di
+000017c0: 6374 3a0d 0a20 2020 2020 2020 2020 2020  ct:..           
+000017d0: 206f 7574 7075 7420 3d20 2720 7b20 270d   output = ' { '.
+000017e0: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
+000017f0: 2076 6172 4b65 792c 2076 6172 5661 6c75   varKey, varValu
+00001800: 6520 696e 2070 7956 6172 6961 626c 652e  e in pyVariable.
+00001810: 6974 656d 7328 293a 0d0a 2020 2020 2020  items():..      
+00001820: 2020 2020 2020 2020 2020 6f75 7470 7574            output
+00001830: 202b 3d20 2724 2720 2b20 5472 616e 736c   += '$' + Transl
+00001840: 6174 652e 746f 5f67 7261 7068 716c 5f66  ate.to_graphql_f
+00001850: 6965 6c64 5f6e 616d 6528 7661 724b 6579  ield_name(varKey
+00001860: 2920 2b20 273a 2027 202b 2054 7261 6e73  ) + ': ' + Trans
+00001870: 6c61 7465 2e74 6f5f 6772 6170 6871 6c5f  late.to_graphql_
+00001880: 7479 7065 2876 6172 5661 6c75 6529 202b  type(varValue) +
+00001890: 2043 4f4d 4d41 5f43 4f4e 4341 540d 0a0d   COMMA_CONCAT...
+000018a0: 0a20 2020 2020 2020 2020 2020 206f 7574  .            out
+000018b0: 7075 7420 3d20 6f75 7470 7574 2e72 656d  put = output.rem
+000018c0: 6f76 6573 7566 6669 7828 434f 4d4d 415f  ovesuffix(COMMA_
+000018d0: 434f 4e43 4154 290d 0a20 2020 2020 2020  CONCAT)..       
+000018e0: 2020 2020 206f 7574 7075 7420 2b3d 2027       output += '
+000018f0: 207d 2027 0d0a 2020 2020 2020 2020 2020   } '..          
+00001900: 2020 7265 7475 726e 206f 7574 7075 740d    return output.
+00001910: 0a20 2020 2020 2020 2065 6c69 6620 456e  .        elif En
+00001920: 756d 2069 6e20 696e 7370 6563 742e 6765  um in inspect.ge
+00001930: 746d 726f 2863 7572 725f 7479 7065 2920  tmro(curr_type) 
+00001940: 6f72 2069 6e73 7065 6374 2e69 7363 6c61  or inspect.iscla
+00001950: 7373 2863 7572 725f 7479 7065 293a 0d0a  ss(curr_type):..
+00001960: 2020 2020 2020 2020 2020 2020 6772 6170              grap
+00001970: 6871 6c5f 7479 7065 203d 2063 7572 725f  hql_type = curr_
+00001980: 7479 7065 2e5f 5f6e 616d 655f 5f0d 0a20  type.__name__.. 
+00001990: 2020 2020 2020 2065 6c73 653a 0d0a 2020         else:..  
+000019a0: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+000019b0: 6861 6e64 6c65 5f72 6563 7572 7369 7665  handle_recursive
+000019c0: 5f65 7828 4578 6365 7074 696f 6e28 2774  _ex(Exception('t
+000019d0: 7970 6520 6e6f 7420 6d61 6e61 6765 6421  ype not managed!
+000019e0: 2729 2c20 2727 290d 0a0d 0a20 2020 2020  '), '')....     
+000019f0: 2020 2072 6574 7572 6e20 6772 6170 6871     return graphq
+00001a00: 6c5f 7479 7065 202b 2028 2721 2720 6966  l_type + ('!' if
+00001a10: 2069 735f 6e6f 6e5f 6e75 6c6c 2065 6c73   is_non_null els
+00001a20: 6520 2727 290d 0a0d 0a20 2020 2064 6566  e '')....    def
+00001a30: 2074 6f5f 7079 7468 6f6e 5f74 7970 6528   to_python_type(
+00001a40: 7479 7065 4e61 6d65 293a 0d0a 2020 2020  typeName):..    
+00001a50: 2020 2020 7265 7475 726e 2073 7769 7463      return switc
+00001a60: 685f 6771 6c5f 7079 5f74 7970 652e 6765  h_gql_py_type.ge
+00001a70: 7428 7479 7065 4e61 6d65 2c20 7479 7065  t(typeName, type
+00001a80: 4e61 6d65 290d 0a0d 0a20 2020 2064 6566  Name)....    def
+00001a90: 2074 6f5f 6a73 6f6e 5f76 6172 7328 6669   to_json_vars(fi
+00001aa0: 656c 6473 3a20 6469 6374 293a 0d0a 2020  elds: dict):..  
+00001ab0: 2020 2020 2020 6f75 7470 7574 203d 2027        output = '
+00001ac0: 270d 0a20 2020 2020 2020 2074 7279 3a0d  '..        try:.
+00001ad0: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
+00001ae0: 2066 6965 6c64 4e61 6d65 2c20 6669 656c   fieldName, fiel
+00001af0: 6456 616c 7565 2069 6e20 6669 656c 6473  dValue in fields
+00001b00: 2e69 7465 6d73 2829 3a0d 0a20 2020 2020  .items():..     
+00001b10: 2020 2020 2020 2020 2020 2069 6620 6973             if is
+00001b20: 5f65 6d70 7479 5f66 6965 6c64 2866 6965  _empty_field(fie
+00001b30: 6c64 5661 6c75 6529 3a20 636f 6e74 696e  ldValue): contin
+00001b40: 7565 0d0a 2020 2020 2020 2020 2020 2020  ue..            
+00001b50: 2020 2020 7472 793a 0d0a 2020 2020 2020      try:..      
+00001b60: 2020 2020 2020 2020 2020 2020 2020 6f75                ou
+00001b70: 7470 7574 202b 3d20 272c 2027 2069 6620  tput += ', ' if 
+00001b80: 6f75 7470 7574 2e73 7461 7274 7377 6974  output.startswit
+00001b90: 6828 277b 2729 2065 6c73 6520 277b 2027  h('{') else '{ '
+00001ba0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00001bb0: 2020 2020 2020 6f75 7470 7574 202b 3d20        output += 
+00001bc0: 275c 2227 202b 2054 7261 6e73 6c61 7465  '\"' + Translate
+00001bd0: 2e74 6f5f 6772 6170 6871 6c5f 6669 656c  .to_graphql_fiel
+00001be0: 645f 6e61 6d65 2866 6965 6c64 4e61 6d65  d_name(fieldName
+00001bf0: 2920 2b20 2027 5c22 203a 270d 0a20 2020  ) +  '\" :'..   
+00001c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001c10: 2066 726f 6d20 7079 6771 6c6d 6170 2e63   from pygqlmap.c
+00001c20: 6f6d 706f 6e65 6e74 7320 696d 706f 7274  omponents import
+00001c30: 2047 514c 4f62 6a65 6374 0d0a 2020 2020   GQLObject..    
+00001c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001c50: 6966 2047 514c 4f62 6a65 6374 2069 6e20  if GQLObject in 
+00001c60: 696e 7370 6563 742e 6765 746d 726f 2874  inspect.getmro(t
+00001c70: 7970 6528 6669 656c 6456 616c 7565 2929  ype(fieldValue))
+00001c80: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00001c90: 2020 2020 2020 2020 2020 206f 7574 7075             outpu
+00001ca0: 7420 2b3d 2054 7261 6e73 6c61 7465 2e74  t += Translate.t
+00001cb0: 6f5f 6a73 6f6e 5f76 6172 7328 6669 656c  o_json_vars(fiel
+00001cc0: 6456 616c 7565 2e5f 5f64 6963 745f 5f29  dValue.__dict__)
+00001cd0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00001ce0: 2020 2020 2020 656c 7365 3a0d 0a20 2020        else:..   
+00001cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001d00: 2020 2020 206f 7574 7075 7420 2b3d 2054       output += T
+00001d10: 7261 6e73 6c61 7465 2e74 6f5f 6a73 6f6e  ranslate.to_json
+00001d20: 5f76 616c 7565 2866 6965 6c64 5661 6c75  _value(fieldValu
+00001d30: 6529 0d0a 2020 2020 2020 2020 2020 2020  e)..            
+00001d40: 2020 2020 6578 6365 7074 2045 7863 6570      except Excep
+00001d50: 7469 6f6e 2061 7320 6578 3a0d 0a20 2020  tion as ex:..   
+00001d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001d70: 2072 6169 7365 2068 616e 646c 655f 7265   raise handle_re
+00001d80: 6375 7273 6976 655f 6578 2865 782c 2027  cursive_ex(ex, '
+00001d90: 4973 7375 6520 6578 706f 7274 696e 6720  Issue exporting 
+00001da0: 7661 7269 6162 6c65 2066 6f72 3a20 2720  variable for: ' 
+00001db0: 2b20 6669 656c 644e 616d 6529 0d0a 0d0a  + fieldName)....
+00001dc0: 2020 2020 2020 2020 2020 2020 6f75 7470              outp
+00001dd0: 7574 2e72 656d 6f76 6573 7566 6669 7828  ut.removesuffix(
+00001de0: 434f 4d4d 415f 434f 4e43 4154 290d 0a20  COMMA_CONCAT).. 
+00001df0: 2020 2020 2020 2065 7863 6570 7420 4578         except Ex
+00001e00: 6365 7074 696f 6e20 6173 2065 783a 0d0a  ception as ex:..
+00001e10: 2020 2020 2020 2020 2020 2020 7261 6973              rais
+00001e20: 6520 6861 6e64 6c65 5f72 6563 7572 7369  e handle_recursi
+00001e30: 7665 5f65 7828 6578 2c20 2749 7373 7565  ve_ex(ex, 'Issue
+00001e40: 2077 6974 6820 6974 656d 7320 6578 706f   with items expo
+00001e50: 7274 696e 6720 7661 7269 6162 6c65 2729  rting variable')
+00001e60: 0d0a 0d0a 2020 2020 2020 2020 6f75 7470  ....        outp
+00001e70: 7574 202b 3d20 2720 7d27 0d0a 2020 2020  ut += ' }'..    
+00001e80: 2020 2020 7265 7475 726e 206f 7574 7075      return outpu
+00001e90: 740d 0a0d 0a20 2020 2064 6566 2067 7261  t....    def gra
+00001ea0: 7068 716c 697a 6528 696e 7075 7453 6f75  phqlize(inputSou
+00001eb0: 7263 6544 6963 742c 2061 7267 7354 6f49  rceDict, argsToI
+00001ec0: 676e 6f72 6520 3d20 4e6f 6e65 293a 0d0a  gnore = None):..
+00001ed0: 2020 2020 2020 2020 7472 793a 0d0a 2020          try:..  
+00001ee0: 2020 2020 2020 2020 2020 6f75 7470 7574            output
+00001ef0: 3d20 2727 0d0a 2020 2020 2020 2020 2020  = ''..          
+00001f00: 2020 666f 7220 696e 7075 7453 6f75 7263    for inputSourc
+00001f10: 654b 6579 2c20 696e 7075 7453 6f75 7263  eKey, inputSourc
+00001f20: 6556 616c 7565 2069 6e20 696e 7075 7453  eValue in inputS
+00001f30: 6f75 7263 6544 6963 742e 6974 656d 7328  ourceDict.items(
+00001f40: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+00001f50: 2020 2020 6966 2069 7369 6e73 7461 6e63      if isinstanc
+00001f60: 6528 696e 7075 7453 6f75 7263 6556 616c  e(inputSourceVal
+00001f70: 7565 2c20 6469 6374 293a 0d0a 2020 2020  ue, dict):..    
+00001f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001f90: 7072 696e 7428 2747 6574 7469 6e67 2069  print('Getting i
+00001fa0: 6e74 6f20 2720 2b20 696e 7075 7453 6f75  nto ' + inputSou
+00001fb0: 7263 654b 6579 290d 0a20 2020 2020 2020  rceKey)..       
+00001fc0: 2020 2020 2020 2020 2020 2020 206f 7574               out
+00001fd0: 7075 7420 2b3d 2069 6e70 7574 536f 7572  put += inputSour
+00001fe0: 6365 4b65 7920 2b20 2861 7267 7354 6f49  ceKey + (argsToI
+00001ff0: 676e 6f72 6520 6966 2061 7267 7354 6f49  gnore if argsToI
+00002000: 676e 6f72 6520 656c 7365 2027 2729 202b  gnore else '') +
+00002010: 2027 207b 2027 202b 2054 7261 6e73 6c61   ' { ' + Transla
+00002020: 7465 2e67 7261 7068 716c 697a 6528 696e  te.graphqlize(in
+00002030: 7075 7453 6f75 7263 6556 616c 7565 2920  putSourceValue) 
+00002040: 2b20 2720 7d20 270d 0a20 2020 2020 2020  + ' } '..       
+00002050: 2020 2020 2020 2020 2065 6c69 6620 6973           elif is
+00002060: 696e 7374 616e 6365 2869 6e70 7574 536f  instance(inputSo
+00002070: 7572 6365 5661 6c75 652c 2074 7570 6c65  urceValue, tuple
+00002080: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+00002090: 2020 2020 2020 2020 6966 2069 7369 6e73          if isins
+000020a0: 7461 6e63 6528 696e 7075 7453 6f75 7263  tance(inputSourc
+000020b0: 6556 616c 7565 5b31 5d2c 2064 6963 7429  eValue[1], dict)
+000020c0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+000020d0: 2020 2020 2020 2020 2020 206f 7574 7075             outpu
+000020e0: 7420 2b3d 2069 6e70 7574 536f 7572 6365  t += inputSource
+000020f0: 4b65 7920 2b20 696e 7075 7453 6f75 7263  Key + inputSourc
+00002100: 6556 616c 7565 5b30 5d20 2b20 2720 7b20  eValue[0] + ' { 
+00002110: 2720 2b20 5472 616e 736c 6174 652e 6772  ' + Translate.gr
+00002120: 6170 6871 6c69 7a65 2869 6e70 7574 536f  aphqlize(inputSo
+00002130: 7572 6365 5661 6c75 655b 315d 2920 2b20  urceValue[1]) + 
+00002140: 2720 7d20 270d 0a20 2020 2020 2020 2020  ' } '..         
+00002150: 2020 2020 2020 2065 6c73 653a 0d0a 2020         else:..  
+00002160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002170: 2020 6f75 7470 7574 202b 3d20 6578 6563    output += exec
+00002180: 7574 655f 7265 6765 7828 2220 2220 2b20  ute_regex(" " + 
+00002190: 696e 7075 7453 6f75 7263 654b 6579 202b  inputSourceKey +
+000021a0: 2022 2022 290d 0a20 2020 2020 2020 2065   " ")..        e
+000021b0: 7863 6570 7420 4578 6365 7074 696f 6e20  xcept Exception 
+000021c0: 6173 2065 783a 0d0a 2020 2020 2020 2020  as ex:..        
+000021d0: 2020 2020 7261 6973 6520 6861 6e64 6c65      raise handle
+000021e0: 5f72 6563 7572 7369 7665 5f65 7828 6578  _recursive_ex(ex
+000021f0: 2c20 2745 7863 6570 7469 6f6e 2064 7572  , 'Exception dur
+00002200: 696e 6720 6772 6170 6871 6c69 7a69 6e67  ing graphqlizing
+00002210: 206f 6620 2720 2b20 7374 7228 696e 7075   of ' + str(inpu
+00002220: 7453 6f75 7263 6544 6963 7429 290d 0a0d  tSourceDict))...
+00002230: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00002240: 6f75 7470 7574 0d0a 0d0a 2020 2020 6465  output....    de
+00002250: 6620 6578 636c 7564 655f 6172 6773 5f73  f exclude_args_s
+00002260: 7562 7374 7269 6e67 2864 6174 6149 6e70  ubstring(dataInp
+00002270: 7574 3a20 7374 722c 2061 7267 7354 6f49  ut: str, argsToI
+00002280: 676e 6f72 653a 206c 6973 7429 3a0d 0a20  gnore: list):.. 
+00002290: 2020 2020 2020 2066 6f72 2061 7267 7320         for args 
+000022a0: 696e 2061 7267 7354 6f49 676e 6f72 653a  in argsToIgnore:
+000022b0: 0d0a 2020 2020 2020 2020 2020 2020 7472  ..            tr
+000022c0: 793a 0d0a 2020 2020 2020 2020 2020 2020  y:..            
+000022d0: 2020 2020 6966 2073 7472 2864 6174 6149      if str(dataI
+000022e0: 6e70 7574 292e 5f5f 636f 6e74 6169 6e73  nput).__contains
+000022f0: 5f5f 2861 7267 7329 3a0d 0a20 2020 2020  __(args):..     
+00002300: 2020 2020 2020 2020 2020 2020 2020 206c                 l
+00002310: 6f67 6765 722e 696e 666f 2827 7370 6c69  ogger.info('spli
+00002320: 7474 696e 6720 2720 2b20 6461 7461 496e  tting ' + dataIn
+00002330: 7075 7429 0d0a 2020 2020 2020 2020 2020  put)..          
+00002340: 2020 2020 2020 2020 2020 696e 7075 744c            inputL
+00002350: 6973 7420 3d20 6461 7461 496e 7075 742e  ist = dataInput.
+00002360: 7370 6c69 7428 6172 6773 290d 0a20 2020  split(args)..   
+00002370: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002380: 2072 6574 7572 6e20 6172 6773 2e6a 6f69   return args.joi
+00002390: 6e28 5472 616e 736c 6174 652e 6578 636c  n(Translate.excl
+000023a0: 7564 655f 6172 6773 5f73 7562 7374 7269  ude_args_substri
+000023b0: 6e67 2878 2c20 6172 6773 546f 4967 6e6f  ng(x, argsToIgno
+000023c0: 7265 2920 666f 7220 7820 696e 2069 6e70  re) for x in inp
+000023d0: 7574 4c69 7374 290d 0a20 2020 2020 2020  utList)..       
+000023e0: 2020 2020 2065 7863 6570 7420 4578 6365       except Exce
+000023f0: 7074 696f 6e20 6173 2065 783a 0d0a 2020  ption as ex:..  
+00002400: 2020 2020 2020 2020 2020 2020 2020 7261                ra
+00002410: 6973 6520 6861 6e64 6c65 5f72 6563 7572  ise handle_recur
+00002420: 7369 7665 5f65 7828 6578 2c20 2745 7863  sive_ex(ex, 'Exc
+00002430: 6570 7469 6f6e 2064 7572 696e 6720 6172  eption during ar
+00002440: 6773 2065 7863 6c75 7369 6f6e 2066 726f  gs exclusion fro
+00002450: 6d20 6772 6170 6871 6c69 7a65 2066 6f72  m graphqlize for
+00002460: 2073 7562 7374 7269 6e67 2027 202b 2064   substring ' + d
+00002470: 6174 6149 6e70 7574 290d 0a0d 0a20 2020  ataInput)....   
+00002480: 2020 2020 2072 6574 7572 6e20 6578 6563       return exec
+00002490: 7574 655f 7265 6765 7828 6461 7461 496e  ute_regex(dataIn
+000024a0: 7075 7429 0d0a 0d0a 2020 2020 6465 6620  put)....    def 
+000024b0: 746f 5f67 7261 7068 716c 5f61 7267 7373  to_graphql_argss
+000024c0: 6574 5f64 6566 696e 6974 696f 6e28 7079  et_definition(py
+000024d0: 4f62 6a65 6374 293a 0d0a 2020 2020 2020  Object):..      
+000024e0: 2020 6f75 7470 7574 203d 2027 270d 0a0d    output = ''...
+000024f0: 0a20 2020 2020 2020 2074 7279 3a0d 0a20  .        try:.. 
+00002500: 2020 2020 2020 2020 2020 2066 6f72 2066             for f
+00002510: 6965 6c64 2069 6e20 7079 4f62 6a65 6374  ield in pyObject
+00002520: 2e5f 5f64 6174 6163 6c61 7373 5f66 6965  .__dataclass_fie
+00002530: 6c64 735f 5f3a 0d0a 2020 2020 2020 2020  lds__:..        
+00002540: 2020 2020 2020 2020 6f62 6a65 6374 4669          objectFi
+00002550: 656c 6420 3d20 6765 7461 7474 7228 7079  eld = getattr(py
+00002560: 4f62 6a65 6374 2c20 6669 656c 6429 0d0a  Object, field)..
+00002570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002580: 6966 2069 735f 656d 7074 795f 6669 656c  if is_empty_fiel
+00002590: 6428 6f62 6a65 6374 4669 656c 6429 3a20  d(objectField): 
+000025a0: 636f 6e74 696e 7565 0d0a 2020 2020 2020  continue..      
+000025b0: 2020 2020 2020 2020 2020 7472 793a 0d0a            try:..
+000025c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000025d0: 2020 2020 6672 6f6d 2070 7967 716c 6d61      from pygqlma
+000025e0: 702e 636f 6d70 6f6e 656e 7473 2069 6d70  p.components imp
+000025f0: 6f72 7420 4751 4c4f 626a 6563 740d 0a20  ort GQLObject.. 
+00002600: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002610: 2020 2069 6620 6973 696e 7374 616e 6365     if isinstance
+00002620: 286f 626a 6563 7446 6965 6c64 2c20 6c69  (objectField, li
+00002630: 7374 293a 0d0a 2020 2020 2020 2020 2020  st):..          
+00002640: 2020 2020 2020 2020 2020 2020 2020 6f75                ou
+00002650: 7470 7574 202b 3d20 6669 656c 6420 2b20  tput += field + 
+00002660: 273a 205b 2027 0d0a 2020 2020 2020 2020  ': [ '..        
+00002670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002680: 666f 7220 656c 656d 656e 744c 6973 7420  for elementList 
+00002690: 696e 206f 626a 6563 7446 6965 6c64 3a0d  in objectField:.
+000026a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000026b0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+000026c0: 4751 4c4f 626a 6563 7420 696e 2069 6e73  GQLObject in ins
+000026d0: 7065 6374 2e67 6574 6d72 6f28 7479 7065  pect.getmro(type
+000026e0: 2865 6c65 6d65 6e74 4c69 7374 2929 3a0d  (elementList)):.
+000026f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002700: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002710: 206f 7574 7075 7420 2b3d 2027 207b 2027   output += ' { '
+00002720: 202b 2054 7261 6e73 6c61 7465 2e74 6f5f   + Translate.to_
+00002730: 6772 6170 6871 6c5f 6172 6773 7365 745f  graphql_argsset_
+00002740: 6465 6669 6e69 7469 6f6e 2865 6c65 6d65  definition(eleme
+00002750: 6e74 4c69 7374 2920 2b20 2720 7d20 2720  ntList) + ' } ' 
+00002760: 2b20 434f 4d4d 415f 434f 4e43 4154 0d0a  + COMMA_CONCAT..
+00002770: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002780: 2020 2020 2020 2020 2020 2020 656c 7365              else
+00002790: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+000027a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000027b0: 2020 206f 7574 7075 7420 2b3d 2054 7261     output += Tra
+000027c0: 6e73 6c61 7465 2e74 6f5f 6772 6170 6871  nslate.to_graphq
+000027d0: 6c5f 7661 6c75 6528 656c 656d 656e 744c  l_value(elementL
+000027e0: 6973 7429 202b 2043 4f4d 4d41 5f43 4f4e  ist) + COMMA_CON
+000027f0: 4341 540d 0a20 2020 2020 2020 2020 2020  CAT..           
+00002800: 2020 2020 2020 2020 2020 2020 206f 7574               out
+00002810: 7075 7420 3d20 6f75 7470 7574 2e72 656d  put = output.rem
+00002820: 6f76 6573 7566 6669 7828 434f 4d4d 415f  ovesuffix(COMMA_
+00002830: 434f 4e43 4154 290d 0a20 2020 2020 2020  CONCAT)..       
+00002840: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002850: 206f 7574 7075 7420 2b3d 2027 205d 2027   output += ' ] '
+00002860: 202b 2043 4f4d 4d41 5f43 4f4e 4341 540d   + COMMA_CONCAT.
+00002870: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002880: 2020 2020 2065 6c69 6620 4751 4c4f 626a       elif GQLObj
+00002890: 6563 7420 696e 2069 6e73 7065 6374 2e67  ect in inspect.g
+000028a0: 6574 6d72 6f28 7479 7065 286f 626a 6563  etmro(type(objec
+000028b0: 7446 6965 6c64 2929 3a0d 0a20 2020 2020  tField)):..     
+000028c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000028d0: 2020 206f 7574 7075 7420 2b3d 2066 6965     output += fie
+000028e0: 6c64 202b 2027 3a20 7b20 2720 2b20 5472  ld + ': { ' + Tr
+000028f0: 616e 736c 6174 652e 746f 5f67 7261 7068  anslate.to_graph
+00002900: 716c 5f61 7267 7373 6574 5f64 6566 696e  ql_argsset_defin
+00002910: 6974 696f 6e28 6f62 6a65 6374 4669 656c  ition(objectFiel
+00002920: 6429 202b 2027 207d 2027 0d0a 2020 2020  d) + ' } '..    
+00002930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002940: 2020 2020 6f75 7470 7574 202b 3d20 434f      output += CO
+00002950: 4d4d 415f 434f 4e43 4154 0d0a 2020 2020  MMA_CONCAT..    
+00002960: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002970: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
+00002980: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00002990: 6620 6861 7361 7474 7228 7079 4f62 6a65  f hasattr(pyObje
+000029a0: 6374 2c20 6669 656c 6429 2061 6e64 206e  ct, field) and n
+000029b0: 6f74 206f 626a 6563 7446 6965 6c64 203d  ot objectField =
+000029c0: 3d20 4e6f 6e65 3a0d 0a20 2020 2020 2020  = None:..       
+000029d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000029e0: 2020 2020 206f 7574 7075 7420 2b3d 2054       output += T
+000029f0: 7261 6e73 6c61 7465 2e74 6f5f 6772 6170  ranslate.to_grap
+00002a00: 6871 6c5f 6172 675f 6465 6669 6e69 7469  hql_arg_definiti
+00002a10: 6f6e 2866 6965 6c64 2c20 6f62 6a65 6374  on(field, object
+00002a20: 4669 656c 6429 0d0a 2020 2020 2020 2020  Field)..        
+00002a30: 2020 2020 2020 2020 6578 6365 7074 2045          except E
+00002a40: 7863 6570 7469 6f6e 2061 7320 6578 3a0d  xception as ex:.
+00002a50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002a60: 2020 2020 2072 6169 7365 2068 616e 646c       raise handl
+00002a70: 655f 7265 6375 7273 6976 655f 6578 2865  e_recursive_ex(e
+00002a80: 782c 2027 4973 7375 6520 6475 7269 6e67  x, 'Issue during
+00002a90: 2065 7870 6f72 7420 6f66 206e 616d 6520   export of name 
+00002aa0: 616e 6420 7661 6c75 6520 666f 723a 2027  and value for: '
+00002ab0: 202b 206f 626a 6563 7446 6965 6c64 290d   + objectField).
+00002ac0: 0a0d 0a20 2020 2020 2020 2020 2020 206f  ...            o
+00002ad0: 7574 7075 7420 3d20 6f75 7470 7574 2e72  utput = output.r
+00002ae0: 656d 6f76 6573 7566 6669 7828 434f 4d4d  emovesuffix(COMM
+00002af0: 415f 434f 4e43 4154 290d 0a0d 0a20 2020  A_CONCAT)....   
+00002b00: 2020 2020 2065 7863 6570 7420 4578 6365       except Exce
+00002b10: 7074 696f 6e20 6173 2065 783a 0d0a 2020  ption as ex:..  
+00002b20: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+00002b30: 6861 6e64 6c65 5f72 6563 7572 7369 7665  handle_recursive
+00002b40: 5f65 7828 6578 2c20 2745 7272 6f72 2064  _ex(ex, 'Error d
+00002b50: 7572 696e 6720 7472 616e 736c 6174 696f  uring translatio
+00002b60: 6e20 6f66 2061 7267 756d 656e 7420 7365  n of argument se
+00002b70: 7420 6465 6669 6e69 7469 6f6e 2729 0d0a  t definition')..
+00002b80: 2020 2020 2020 2020 7265 7475 726e 206f          return o
+00002b90: 7574 7075 740d 0a0d 0a20 2020 2064 6566  utput....    def
+00002ba0: 2074 6f5f 6772 6170 6871 6c5f 6172 675f   to_graphql_arg_
+00002bb0: 6465 6669 6e69 7469 6f6e 2866 6965 6c64  definition(field
+00002bc0: 4e61 6d65 2c20 6669 656c 6429 3a0d 0a20  Name, field):.. 
+00002bd0: 2020 2020 2020 2072 6574 7572 6e20 5472         return Tr
+00002be0: 616e 736c 6174 652e 746f 5f67 7261 7068  anslate.to_graph
+00002bf0: 716c 5f66 6965 6c64 5f6e 616d 6528 6669  ql_field_name(fi
+00002c00: 656c 644e 616d 6529 202b 2027 3a20 2720  eldName) + ': ' 
+00002c10: 2b20 5472 616e 736c 6174 652e 746f 5f67  + Translate.to_g
+00002c20: 7261 7068 716c 5f76 616c 7565 2866 6965  raphql_value(fie
+00002c30: 6c64 2920 2b20 434f 4d4d 415f 434f 4e43  ld) + COMMA_CONC
+00002c40: 4154 0d0a                                AT..
```

### Comparing `py-graphql-mapper-1.1.0/pygqlmap/src/utils.py` & `py-graphql-mapper-1.1.1/pygqlmap/src/utils.py`

 * *Files identical despite different names*

### Comparing `py-graphql-mapper-1.1.0/pyproject.toml` & `py-graphql-mapper-1.1.1/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -4,22 +4,21 @@
 
 [project]
 name = "py-graphql-mapper"
 authors = [
   { name="Alex Dap", email="shlisi2017@gmail.com" },
 ]
 readme = "README.md"
-keywords = ["graphql", "mapper"]
+keywords = ["python", "graphql", "mapping"]
 license = { file = "LICENSE" }
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
-    "Development Status :: 4 - Beta",
 ]
 dynamic = ["version", "description"]
 
 [project.scripts]
 pgmcodegen = "codegen.__main__:main"
 
 [project.urls]
```

### Comparing `py-graphql-mapper-1.1.0/setup.py` & `py-graphql-mapper-1.1.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,19 @@
-from setuptools import find_packages, setup
+from setuptools import setup
 
 setup(
     name='pygqlmap',
-    version='1.1.0',
+    version='1.1.1',
     url='https://github.com/dapalex/py-graphql-mapper/',
     author='Alex Dap',
     author_email='shlisi2017@gmail.com',
     description='A python library to call GraphQL APIs without using hardcoded strings',
     include_package_data=True,
     packages=['pygqlmap', 'pygqlmap.src', 'codegen', 'codegen.src', 'codegen.src.templates'],
     data_files=[('', ['pygqlmap/config.ini'])],
     python_requires='>=3.10',
     classifiers=[
-    "Development Status :: 4 - Beta",
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
     ],
 )
```

