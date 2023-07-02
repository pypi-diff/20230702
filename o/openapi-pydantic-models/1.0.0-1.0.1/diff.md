# Comparing `tmp/openapi-pydantic-models-1.0.0.tar.gz` & `tmp/openapi-pydantic-models-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openapi-pydantic-models-1.0.0.tar", last modified: Sat Jul  1 07:11:18 2023, max compression
+gzip compressed data, was "openapi-pydantic-models-1.0.1.tar", last modified: Sun Jul  2 16:51:36 2023, max compression
```

## Comparing `openapi-pydantic-models-1.0.0.tar` & `openapi-pydantic-models-1.0.1.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 07:11:18.111245 openapi-pydantic-models-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-01 07:11:03.000000 openapi-pydantic-models-1.0.0/.bumpversion.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-01 07:11:03.000000 openapi-pydantic-models-1.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-01 07:11:03.000000 openapi-pydantic-models-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-07-01 07:11:03.000000 openapi-pydantic-models-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4908 2023-07-01 07:11:18.111245 openapi-pydantic-models-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4041 2023-07-01 07:11:03.000000 openapi-pydantic-models-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2650 2023-07-01 07:11:03.000000 openapi-pydantic-models-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 07:11:18.111245 openapi-pydantic-models-1.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 07:11:18.095245 openapi-pydantic-models-1.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 07:11:18.099245 openapi-pydantic-models-1.0.0/src/openapi_pydantic_models/
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-01 07:11:03.000000 openapi-pydantic-models-1.0.0/src/openapi_pydantic_models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 07:11:18.099245 openapi-pydantic-models-1.0.0/src/openapi_pydantic_models/commons/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-01 07:11:03.000000 openapi-pydantic-models-1.0.0/src/openapi_pydantic_models/commons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-07-01 07:11:03.000000 openapi-pydantic-models-1.0.0/src/openapi_pydantic_models/commons/base_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-07-01 07:11:03.000000 openapi-pydantic-models-1.0.0/src/openapi_pydantic_models/commons/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 07:11:18.111245 openapi-pydantic-models-1.0.0/src/openapi_pydantic_models/openapi_3_1/
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-07-01 07:11:03.000000 openapi-pydantic-models-1.0.0/src/openapi_pydantic_models/openapi_3_1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3642 2023-07-01 07:11:03.000000 openapi-pydantic-models-1.0.0/src/openapi_pydantic_models/openapi_3_1/callback_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-07-01 07:11:03.000000 openapi-pydantic-models-1.0.0/src/openapi_pydantic_models/openapi_3_1/components_object.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-01 07:11:03.000000 openapi-pydantic-models-1.0.0/src/openapi_pydantic_models/openapi_3_1/contact_object.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-07-01 07:11:03.000000 openapi-pydantic-models-1.0.0/src/openapi_pydantic_models/openapi_3_1/encoding_object.py
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-01 07:11:03.000000 openapi-pydantic-models-1.0.0/src/openapi_pydantic_models/openapi_3_1/example_object.py
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-01 07:11:03.000000 openapi-pydantic-models-1.0.0/src/openapi_pydantic_models/openapi_3_1/external_documentation_object.py
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-07-01 07:11:03.000000 openapi-pydantic-models-1.0.0/src/openapi_pydantic_models/openapi_3_1/header_object.py
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-07-01 07:11:03.000000 openapi-pydantic-models-1.0.0/src/openapi_pydantic_models/openapi_3_1/info_object.py
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-01 07:11:03.000000 openapi-pydantic-models-1.0.0/src/openapi_pydantic_models/openapi_3_1/license_object.py
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-01 07:11:03.000000 openapi-pydantic-models-1.0.0/src/openapi_pydantic_models/openapi_3_1/link_object.py
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-01 07:11:03.000000 openapi-pydantic-models-1.0.0/src/openapi_pydantic_models/openapi_3_1/locations.py
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-07-01 07:11:03.000000 openapi-pydantic-models-1.0.0/src/openapi_pydantic_models/openapi_3_1/media_type_object.py
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-01 07:11:03.000000 openapi-pydantic-models-1.0.0/src/openapi_pydantic_models/openapi_3_1/oauth_flow_object.py
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-01 07:11:03.000000 openapi-pydantic-models-1.0.0/src/openapi_pydantic_models/openapi_3_1/oauth_flows_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-07-01 07:11:03.000000 openapi-pydantic-models-1.0.0/src/openapi_pydantic_models/openapi_3_1/openapi_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-07-01 07:11:03.000000 openapi-pydantic-models-1.0.0/src/openapi_pydantic_models/openapi_3_1/operation_object.py
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-07-01 07:11:03.000000 openapi-pydantic-models-1.0.0/src/openapi_pydantic_models/openapi_3_1/parameter_object.py
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-07-01 07:11:03.000000 openapi-pydantic-models-1.0.0/src/openapi_pydantic_models/openapi_3_1/path_item_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-07-01 07:11:03.000000 openapi-pydantic-models-1.0.0/src/openapi_pydantic_models/openapi_3_1/paths_object.py
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-01 07:11:03.000000 openapi-pydantic-models-1.0.0/src/openapi_pydantic_models/openapi_3_1/reference_object.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-01 07:11:03.000000 openapi-pydantic-models-1.0.0/src/openapi_pydantic_models/openapi_3_1/request_body_object.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-01 07:11:03.000000 openapi-pydantic-models-1.0.0/src/openapi_pydantic_models/openapi_3_1/response_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     3947 2023-07-01 07:11:03.000000 openapi-pydantic-models-1.0.0/src/openapi_pydantic_models/openapi_3_1/responses_object.py
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-07-01 07:11:03.000000 openapi-pydantic-models-1.0.0/src/openapi_pydantic_models/openapi_3_1/schema_object.py
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-01 07:11:03.000000 openapi-pydantic-models-1.0.0/src/openapi_pydantic_models/openapi_3_1/security_requirement_object.py
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-07-01 07:11:03.000000 openapi-pydantic-models-1.0.0/src/openapi_pydantic_models/openapi_3_1/security_scheme_object.py
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-01 07:11:03.000000 openapi-pydantic-models-1.0.0/src/openapi_pydantic_models/openapi_3_1/server_object.py
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-01 07:11:03.000000 openapi-pydantic-models-1.0.0/src/openapi_pydantic_models/openapi_3_1/server_variable_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-07-01 07:11:03.000000 openapi-pydantic-models-1.0.0/src/openapi_pydantic_models/openapi_3_1/specification_extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-01 07:11:03.000000 openapi-pydantic-models-1.0.0/src/openapi_pydantic_models/openapi_3_1/styles.py
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-01 07:11:03.000000 openapi-pydantic-models-1.0.0/src/openapi_pydantic_models/openapi_3_1/tag_object.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 07:11:18.099245 openapi-pydantic-models-1.0.0/src/openapi_pydantic_models.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4908 2023-07-01 07:11:18.000000 openapi-pydantic-models-1.0.0/src/openapi_pydantic_models.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-07-01 07:11:18.000000 openapi-pydantic-models-1.0.0/src/openapi_pydantic_models.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 07:11:18.000000 openapi-pydantic-models-1.0.0/src/openapi_pydantic_models.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 07:11:17.000000 openapi-pydantic-models-1.0.0/src/openapi_pydantic_models.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-01 07:11:18.000000 openapi-pydantic-models-1.0.0/src/openapi_pydantic_models.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-01 07:11:18.000000 openapi-pydantic-models-1.0.0/src/openapi_pydantic_models.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 16:51:36.757181 openapi-pydantic-models-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-02 16:51:25.000000 openapi-pydantic-models-1.0.1/.bumpversion.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-02 16:51:25.000000 openapi-pydantic-models-1.0.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-02 16:51:25.000000 openapi-pydantic-models-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-07-02 16:51:25.000000 openapi-pydantic-models-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4908 2023-07-02 16:51:36.757181 openapi-pydantic-models-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4041 2023-07-02 16:51:25.000000 openapi-pydantic-models-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2650 2023-07-02 16:51:25.000000 openapi-pydantic-models-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 16:51:36.757181 openapi-pydantic-models-1.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 16:51:36.749180 openapi-pydantic-models-1.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 16:51:36.749180 openapi-pydantic-models-1.0.1/src/openapi_pydantic_models/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-02 16:51:25.000000 openapi-pydantic-models-1.0.1/src/openapi_pydantic_models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 16:51:36.753181 openapi-pydantic-models-1.0.1/src/openapi_pydantic_models/commons/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-02 16:51:25.000000 openapi-pydantic-models-1.0.1/src/openapi_pydantic_models/commons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-07-02 16:51:25.000000 openapi-pydantic-models-1.0.1/src/openapi_pydantic_models/commons/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-07-02 16:51:25.000000 openapi-pydantic-models-1.0.1/src/openapi_pydantic_models/commons/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 16:51:36.757181 openapi-pydantic-models-1.0.1/src/openapi_pydantic_models/openapi_3_1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-07-02 16:51:25.000000 openapi-pydantic-models-1.0.1/src/openapi_pydantic_models/openapi_3_1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3552 2023-07-02 16:51:25.000000 openapi-pydantic-models-1.0.1/src/openapi_pydantic_models/openapi_3_1/callback_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-07-02 16:51:25.000000 openapi-pydantic-models-1.0.1/src/openapi_pydantic_models/openapi_3_1/components_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-02 16:51:25.000000 openapi-pydantic-models-1.0.1/src/openapi_pydantic_models/openapi_3_1/contact_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-07-02 16:51:25.000000 openapi-pydantic-models-1.0.1/src/openapi_pydantic_models/openapi_3_1/encoding_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-02 16:51:25.000000 openapi-pydantic-models-1.0.1/src/openapi_pydantic_models/openapi_3_1/example_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-02 16:51:25.000000 openapi-pydantic-models-1.0.1/src/openapi_pydantic_models/openapi_3_1/external_documentation_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-07-02 16:51:25.000000 openapi-pydantic-models-1.0.1/src/openapi_pydantic_models/openapi_3_1/header_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-07-02 16:51:25.000000 openapi-pydantic-models-1.0.1/src/openapi_pydantic_models/openapi_3_1/info_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-02 16:51:25.000000 openapi-pydantic-models-1.0.1/src/openapi_pydantic_models/openapi_3_1/license_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-02 16:51:25.000000 openapi-pydantic-models-1.0.1/src/openapi_pydantic_models/openapi_3_1/link_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-02 16:51:25.000000 openapi-pydantic-models-1.0.1/src/openapi_pydantic_models/openapi_3_1/locations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-07-02 16:51:25.000000 openapi-pydantic-models-1.0.1/src/openapi_pydantic_models/openapi_3_1/media_type_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-02 16:51:25.000000 openapi-pydantic-models-1.0.1/src/openapi_pydantic_models/openapi_3_1/oauth_flow_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-02 16:51:25.000000 openapi-pydantic-models-1.0.1/src/openapi_pydantic_models/openapi_3_1/oauth_flows_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-07-02 16:51:25.000000 openapi-pydantic-models-1.0.1/src/openapi_pydantic_models/openapi_3_1/openapi_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-07-02 16:51:25.000000 openapi-pydantic-models-1.0.1/src/openapi_pydantic_models/openapi_3_1/operation_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-07-02 16:51:25.000000 openapi-pydantic-models-1.0.1/src/openapi_pydantic_models/openapi_3_1/parameter_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-07-02 16:51:25.000000 openapi-pydantic-models-1.0.1/src/openapi_pydantic_models/openapi_3_1/path_item_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-07-02 16:51:25.000000 openapi-pydantic-models-1.0.1/src/openapi_pydantic_models/openapi_3_1/paths_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-02 16:51:25.000000 openapi-pydantic-models-1.0.1/src/openapi_pydantic_models/openapi_3_1/reference_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-02 16:51:25.000000 openapi-pydantic-models-1.0.1/src/openapi_pydantic_models/openapi_3_1/request_body_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-02 16:51:25.000000 openapi-pydantic-models-1.0.1/src/openapi_pydantic_models/openapi_3_1/response_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4151 2023-07-02 16:51:25.000000 openapi-pydantic-models-1.0.1/src/openapi_pydantic_models/openapi_3_1/responses_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-07-02 16:51:25.000000 openapi-pydantic-models-1.0.1/src/openapi_pydantic_models/openapi_3_1/schema_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-02 16:51:25.000000 openapi-pydantic-models-1.0.1/src/openapi_pydantic_models/openapi_3_1/security_requirement_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-07-02 16:51:25.000000 openapi-pydantic-models-1.0.1/src/openapi_pydantic_models/openapi_3_1/security_scheme_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-02 16:51:25.000000 openapi-pydantic-models-1.0.1/src/openapi_pydantic_models/openapi_3_1/server_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-02 16:51:25.000000 openapi-pydantic-models-1.0.1/src/openapi_pydantic_models/openapi_3_1/server_variable_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-07-02 16:51:25.000000 openapi-pydantic-models-1.0.1/src/openapi_pydantic_models/openapi_3_1/specification_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-02 16:51:25.000000 openapi-pydantic-models-1.0.1/src/openapi_pydantic_models/openapi_3_1/styles.py
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-02 16:51:25.000000 openapi-pydantic-models-1.0.1/src/openapi_pydantic_models/openapi_3_1/tag_object.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 16:51:36.753181 openapi-pydantic-models-1.0.1/src/openapi_pydantic_models.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4908 2023-07-02 16:51:36.000000 openapi-pydantic-models-1.0.1/src/openapi_pydantic_models.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-07-02 16:51:36.000000 openapi-pydantic-models-1.0.1/src/openapi_pydantic_models.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 16:51:36.000000 openapi-pydantic-models-1.0.1/src/openapi_pydantic_models.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 16:51:36.000000 openapi-pydantic-models-1.0.1/src/openapi_pydantic_models.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-02 16:51:36.000000 openapi-pydantic-models-1.0.1/src/openapi_pydantic_models.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-02 16:51:36.000000 openapi-pydantic-models-1.0.1/src/openapi_pydantic_models.egg-info/top_level.txt
```

### Comparing `openapi-pydantic-models-1.0.0/.gitignore` & `openapi-pydantic-models-1.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `openapi-pydantic-models-1.0.0/LICENSE` & `openapi-pydantic-models-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `openapi-pydantic-models-1.0.0/MANIFEST.in` & `openapi-pydantic-models-1.0.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `openapi-pydantic-models-1.0.0/PKG-INFO` & `openapi-pydantic-models-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openapi-pydantic-models
-Version: 1.0.0
+Version: 1.0.1
 Summary: pydantic models for OpeanAPI Specification 3.1.0 objects.
 Author-email: Tomislav Adamic <tomislav.adamic@gmail.com>
 License: MIT
 Project-URL: Source, https://github.com/tadams42/openapi-pydantic-models
 Keywords: OpenAPI OAS
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `openapi-pydantic-models-1.0.0/README.md` & `openapi-pydantic-models-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `openapi-pydantic-models-1.0.0/pyproject.toml` & `openapi-pydantic-models-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=65", "wheel"]
 
 
 [project]
 name = "openapi-pydantic-models"
-version = "1.0.0"
+version = "1.0.1"
 description = "pydantic models for OpeanAPI Specification 3.1.0 objects."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "License :: OSI Approved :: MIT License",
     "Operating System :: POSIX :: Linux",
```

### Comparing `openapi-pydantic-models-1.0.0/src/openapi_pydantic_models/commons/utilities.py` & `openapi-pydantic-models-1.0.1/src/openapi_pydantic_models/commons/utilities.py`

 * *Files identical despite different names*

### Comparing `openapi-pydantic-models-1.0.0/src/openapi_pydantic_models/openapi_3_1/__init__.py` & `openapi-pydantic-models-1.0.1/src/openapi_pydantic_models/openapi_3_1/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -29,7 +29,13 @@
     SecuritySchemeTypes,
 )
 from .server_object import ServerObject
 from .server_variable_object import ServerVariableObject
 from .specification_extensions import ExtensionsStorage, SpecificationExtendable
 from .styles import Styles
 from .tag_object import TagObject
+
+
+OperationObject.model_rebuild()
+MediaTypeObject.model_rebuild()
+PathItemObject.model_rebuild()
+OpenAPIObject.model_rebuild()
```

### Comparing `openapi-pydantic-models-1.0.0/src/openapi_pydantic_models/openapi_3_1/callback_object.py` & `openapi-pydantic-models-1.0.1/src/openapi_pydantic_models/openapi_3_1/callback_object.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from __future__ import annotations
 
 import itertools
 from typing import Any, Iterator, MutableMapping
 
-from pydantic import PrivateAttr
+from pydantic import PrivateAttr, model_serializer
 
 from ..commons import BaseModel, exclude_blanks
 from .path_item_object import PathItemObject
 from .reference_object import ReferenceObject
 from .specification_extensions import ExtensionsStorage
 
 
-class CallbackObject(MutableMapping[str, PathItemObject | ReferenceObject], BaseModel):
+class CallbackObject(BaseModel, MutableMapping[str, PathItemObject | ReferenceObject]):
     """
     Model for OpenAPI CallbackObject.
 
     This object MAY be extended with with [4.9 Specification
     Extensions](https://spec.openapis.org/oas/v3.1.0#specificationExtensions).
     """
 
@@ -96,23 +96,20 @@
                     else v
                     for k, v in self._data.items()
                 }
             )
             + ")"
         )
 
-    def model_dump(
-        self, *, by_alias: bool = True, exclude_none: bool = True, **kwargs
-    ) -> dict[str, Any]:
-        retv = {
-            k: (
-                v.model_dump(by_alias=by_alias, exclude_none=exclude_none, **kwargs)
+    @model_serializer
+    def ser_model(self) -> dict[str, Any]:
+        retv = dict()
+        for k, v in itertools.chain(self._data.items(), self._ext.items()):
+            retv[k] = (
+                v.model_dump(by_alias=True, exclude_none=True)
                 if isinstance(v, (ReferenceObject, PathItemObject))
                 else v
             )
-            for k, v in itertools.chain(self._data.items(), self._ext.items())
-        }
 
-        if exclude_none:
-            retv = exclude_blanks(retv)
+        retv = exclude_blanks(retv)
 
         return retv or dict()
```

### Comparing `openapi-pydantic-models-1.0.0/src/openapi_pydantic_models/openapi_3_1/components_object.py` & `openapi-pydantic-models-1.0.1/src/openapi_pydantic_models/openapi_3_1/components_object.py`

 * *Files identical despite different names*

### Comparing `openapi-pydantic-models-1.0.0/src/openapi_pydantic_models/openapi_3_1/encoding_object.py` & `openapi-pydantic-models-1.0.1/src/openapi_pydantic_models/openapi_3_1/encoding_object.py`

 * *Files identical despite different names*

### Comparing `openapi-pydantic-models-1.0.0/src/openapi_pydantic_models/openapi_3_1/header_object.py` & `openapi-pydantic-models-1.0.1/src/openapi_pydantic_models/openapi_3_1/header_object.py`

 * *Files identical despite different names*

### Comparing `openapi-pydantic-models-1.0.0/src/openapi_pydantic_models/openapi_3_1/media_type_object.py` & `openapi-pydantic-models-1.0.1/src/openapi_pydantic_models/openapi_3_1/media_type_object.py`

 * *Files identical despite different names*

### Comparing `openapi-pydantic-models-1.0.0/src/openapi_pydantic_models/openapi_3_1/openapi_object.py` & `openapi-pydantic-models-1.0.1/src/openapi_pydantic_models/openapi_3_1/openapi_object.py`

 * *Files identical despite different names*

### Comparing `openapi-pydantic-models-1.0.0/src/openapi_pydantic_models/openapi_3_1/operation_object.py` & `openapi-pydantic-models-1.0.1/src/openapi_pydantic_models/openapi_3_1/operation_object.py`

 * *Files identical despite different names*

### Comparing `openapi-pydantic-models-1.0.0/src/openapi_pydantic_models/openapi_3_1/parameter_object.py` & `openapi-pydantic-models-1.0.1/src/openapi_pydantic_models/openapi_3_1/parameter_object.py`

 * *Files identical despite different names*

### Comparing `openapi-pydantic-models-1.0.0/src/openapi_pydantic_models/openapi_3_1/path_item_object.py` & `openapi-pydantic-models-1.0.1/src/openapi_pydantic_models/openapi_3_1/path_item_object.py`

 * *Files identical despite different names*

### Comparing `openapi-pydantic-models-1.0.0/src/openapi_pydantic_models/openapi_3_1/paths_object.py` & `openapi-pydantic-models-1.0.1/src/openapi_pydantic_models/openapi_3_1/paths_object.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import itertools
 from typing import Any, Iterator, MutableMapping
 
-from pydantic import PrivateAttr
+from pydantic import PrivateAttr, model_serializer
 
 from ..commons import BaseModel, exclude_blanks
 from .path_item_object import PathItemObject
 from .specification_extensions import ExtensionsStorage
 
 
-class PathsObject(MutableMapping[str, PathItemObject], BaseModel):
+class PathsObject(BaseModel, MutableMapping[str, PathItemObject]):
     """
     Model for OpenAPI Paths Object. This object is mapping of path template strings
     with PathItemObject.
 
     This object MAY be extended with with [4.9 Specification
     Extensions](https://spec.openapis.org/oas/v3.1.0#specificationExtensions).
 
@@ -106,23 +106,20 @@
                     else v
                     for k, v in self._data.items()
                 }
             )
             + ")"
         )
 
-    def model_dump(
-        self, *, by_alias: bool = True, exclude_none: bool = True, **kwargs
-    ) -> dict[str, Any]:
-        retv = {
-            k: (
-                v.model_dump(by_alias=by_alias, exclude_none=exclude_none, **kwargs)
+    @model_serializer
+    def ser_model(self) -> dict[str, Any]:
+        retv = dict()
+        for k, v in itertools.chain(self._data.items(), self._ext.items()):
+            retv[k] = (
+                v.model_dump(by_alias=True, exclude_none=True)
                 if isinstance(v, PathItemObject)
                 else v
             )
-            for k, v in itertools.chain(self._data.items(), self._ext.items())
-        }
 
-        if exclude_none:
-            retv = exclude_blanks(retv)
+        retv = exclude_blanks(retv)
 
         return retv or dict()
```

### Comparing `openapi-pydantic-models-1.0.0/src/openapi_pydantic_models/openapi_3_1/responses_object.py` & `openapi-pydantic-models-1.0.1/src/openapi_pydantic_models/openapi_3_1/responses_object.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,40 +1,41 @@
 from __future__ import annotations
 
 import itertools
-from typing import Any, Iterator, MutableMapping
+from collections.abc import MutableMapping
+from typing import Any, Iterator
 
-from pydantic import PrivateAttr
+from pydantic import PrivateAttr, Field, model_serializer
 
 from ..commons import BaseModel, exclude_blanks
 from .reference_object import ReferenceObject
 from .response_object import ResponseObject
 from .specification_extensions import ExtensionsStorage
 
 
-class ResponsesObject(MutableMapping[str, ResponseObject | ReferenceObject], BaseModel):
+class ResponsesObject(BaseModel, MutableMapping[str, ResponseObject | ReferenceObject]):
     """
     Model for OpenAPI ResponsesObject. This object is mapping of HTTP status codes
     with responses.
 
     This object MAY be extended with with [4.9 Specification
     Extensions](https://spec.openapis.org/oas/v3.1.0#specificationExtensions).
     """
 
-    default: ResponseObject | ReferenceObject | None = None
+    default_: ResponseObject | ReferenceObject | None = Field(
+        default=None, alias="default"
+    )
     _data: dict[str, ResponseObject | ReferenceObject] = PrivateAttr(
         default_factory=dict
     )
     _ext: ExtensionsStorage = PrivateAttr(default_factory=ExtensionsStorage)
 
-    def __init__(
-        self, *, default: ResponseObject | ReferenceObject | None = None, **kwargs
-    ):
-        super().__init__(default=default)
-        raw_data = dict(**kwargs)
+    def __init__(self, **kwargs):
+        super().__init__(**{k: v for k, v in kwargs.items() if k == "default"})
+        raw_data = dict(**{k: v for k, v in kwargs.items() if k != "default"})
         self._ext = ExtensionsStorage(raw_data)
         for k, v in raw_data.items():
             if not ExtensionsStorage.is_key(str(k)):
                 self.__setitem__(k, v)
 
     @property
     def extensions(self) -> ExtensionsStorage:
@@ -84,40 +85,45 @@
         data = {
             k: v.model_dump(by_alias=True, exclude_none=False)
             if isinstance(v, (ReferenceObject, ResponseObject))
             else v
             for k, v in self._data.items()
         }
 
-        if self.default:
-            data["default"] = self.default.model_dump(by_alias=True, exclude_none=False)
+        if self.default_:
+            data["default"] = self.default_.model_dump(
+                by_alias=True, exclude_none=False
+            )
 
         return str(data)
 
     def __repr__(self) -> str:
         data = {
             k: v.model_dump(by_alias=True, exclude_none=False)
             if isinstance(v, (ReferenceObject, ResponseObject))
             else v
             for k, v in self._data.items()
         }
-        if self.default:
-            data["default"] = self.default.model_dump(by_alias=True, exclude_none=False)
+        if self.default_:
+            data["default"] = self.default_.model_dump(
+                by_alias=True, exclude_none=False
+            )
 
         return f"{self.__class__.__name__}({repr(data)})"
 
-    def model_dump(
-        self, *, by_alias: bool = True, exclude_none: bool = True, **kwargs
-    ) -> dict[str, Any]:
+    @model_serializer
+    def ser_model(self) -> dict[str, Any]:
         retv = {
-            k: (
-                v.model_dump(by_alias=by_alias, exclude_none=exclude_none, **kwargs)
+            "default": (self.default_.model_dump(by_alias=True, exclude_none=True))
+            if self.default_
+            else None
+        }
+        for k, v in itertools.chain(self._data.items(), self._ext.items()):
+            retv[k] = (
+                v.model_dump(by_alias=True, exclude_none=True)
                 if isinstance(v, (ReferenceObject, ResponseObject))
                 else v
             )
-            for k, v in itertools.chain(self._data.items(), self._ext.items())
-        }
 
-        if exclude_none:
-            retv = exclude_blanks(retv)
+        retv = exclude_blanks(retv)
 
         return retv or dict()
```

### Comparing `openapi-pydantic-models-1.0.0/src/openapi_pydantic_models/openapi_3_1/security_scheme_object.py` & `openapi-pydantic-models-1.0.1/src/openapi_pydantic_models/openapi_3_1/security_scheme_object.py`

 * *Files identical despite different names*

### Comparing `openapi-pydantic-models-1.0.0/src/openapi_pydantic_models/openapi_3_1/specification_extensions.py` & `openapi-pydantic-models-1.0.1/src/openapi_pydantic_models/openapi_3_1/specification_extensions.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import re
 from collections.abc import MutableMapping
 from typing import Any, Iterator
 
-from pydantic import PrivateAttr
+from pydantic import BaseModel as PydanticBaseModel
+from pydantic import ConfigDict, PrivateAttr
 
 from ..commons import BaseModel, exclude_blanks
 
 
 class ExtensionsStorage(MutableMapping[str, Any]):
     _RE_KEYS = re.compile(r"^x-")
 
@@ -50,15 +51,15 @@
         return (
             f"{self.__class__.__name__}("
             + repr({k: v for k, v in self._data.items()})
             + ")"
         )
 
 
-class SpecificationExtendable(BaseModel):
+class SpecificationExtendable(PydanticBaseModel):
     """
     Base model class for models that can be extended via OpenAPI specification
     extensions.
 
     Inheriting from this class will:
 
     - add property ``extensions``
@@ -91,14 +92,21 @@
         >>> SomeModel(attr='...')
         repr(obj.extensions)
         >>> "ExtensionsStorage({'x-foo': 42, 'x-bar': ['baz']})"
         obj.model_dump()
         >>> {'attr': '...', 'x-foo': 42, 'x-bar': ['baz']}
     """
 
+    model_config = ConfigDict(
+        from_attributes=True,
+        str_strip_whitespace=True,
+        extra="forbid",
+        use_enum_values=True,
+    )
+
     _ext: ExtensionsStorage = PrivateAttr(default_factory=ExtensionsStorage)
 
     def __init__(self, **data):
         super().__init__(
             **{k: v for k, v in data.items() if not ExtensionsStorage.is_key(str(k))}
         )
         self._ext = ExtensionsStorage(data)
@@ -107,18 +115,17 @@
     def extensions(self) -> ExtensionsStorage:
         return self._ext
 
     def model_dump(
         self, *, by_alias: bool = True, exclude_none: bool = True, **kwargs
     ) -> dict[str, Any]:
         retv = (
-            super().model_dump(exclude_none=exclude_none, by_alias=by_alias, **kwargs)
+            super().model_dump(by_alias=by_alias, exclude_none=exclude_none, **kwargs)
             or dict()
         )
-
         for k, v in self._ext.items():
             retv[str(k)] = v
 
         if exclude_none:
             retv = exclude_blanks(retv)
 
         return retv or dict()
```

### Comparing `openapi-pydantic-models-1.0.0/src/openapi_pydantic_models.egg-info/PKG-INFO` & `openapi-pydantic-models-1.0.1/src/openapi_pydantic_models.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openapi-pydantic-models
-Version: 1.0.0
+Version: 1.0.1
 Summary: pydantic models for OpeanAPI Specification 3.1.0 objects.
 Author-email: Tomislav Adamic <tomislav.adamic@gmail.com>
 License: MIT
 Project-URL: Source, https://github.com/tadams42/openapi-pydantic-models
 Keywords: OpenAPI OAS
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `openapi-pydantic-models-1.0.0/src/openapi_pydantic_models.egg-info/SOURCES.txt` & `openapi-pydantic-models-1.0.1/src/openapi_pydantic_models.egg-info/SOURCES.txt`

 * *Files identical despite different names*

