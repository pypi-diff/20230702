# Comparing `tmp/nsj_rest_lib-1.2.1.tar.gz` & `tmp/nsj_rest_lib-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nsj_rest_lib-1.2.1.tar", last modified: Thu Jun 29 22:13:11 2023, max compression
+gzip compressed data, was "nsj_rest_lib-1.3.0.tar", last modified: Sun Jul  2 01:03:11 2023, max compression
```

## Comparing `nsj_rest_lib-1.2.1.tar` & `nsj_rest_lib-1.3.0.tar`

### file list

```diff
@@ -1,57 +1,58 @@
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-06-29 22:13:11.484819 nsj_rest_lib-1.2.1/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      743 2023-06-29 22:13:11.484819 nsj_rest_lib-1.2.1/PKG-INFO
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      130 2023-06-29 21:26:20.000000 nsj_rest_lib-1.2.1/README.md
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      103 2023-06-29 21:26:20.000000 nsj_rest_lib-1.2.1/pyproject.toml
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      888 2023-06-29 22:13:11.488819 nsj_rest_lib-1.2.1/setup.cfg
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-06-29 22:13:11.476819 nsj_rest_lib-1.2.1/src/
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-06-29 22:13:11.476819 nsj_rest_lib-1.2.1/src/nsj_rest_lib/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-06-29 21:26:20.000000 nsj_rest_lib-1.2.1/src/nsj_rest_lib/__init__.py
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-06-29 22:13:11.480819 nsj_rest_lib-1.2.1/src/nsj_rest_lib/controller/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-06-29 21:26:20.000000 nsj_rest_lib-1.2.1/src/nsj_rest_lib/controller/__init__.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)       75 2023-06-29 21:26:20.000000 nsj_rest_lib-1.2.1/src/nsj_rest_lib/controller/controller_util.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     3298 2023-06-29 22:11:32.000000 nsj_rest_lib-1.2.1/src/nsj_rest_lib/controller/delete_route.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      944 2023-06-29 21:26:20.000000 nsj_rest_lib-1.2.1/src/nsj_rest_lib/controller/funtion_route_wrapper.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     3907 2023-06-29 22:11:52.000000 nsj_rest_lib-1.2.1/src/nsj_rest_lib/controller/get_route.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     4483 2023-06-29 22:09:09.000000 nsj_rest_lib-1.2.1/src/nsj_rest_lib/controller/list_route.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     4351 2023-06-29 22:09:50.000000 nsj_rest_lib-1.2.1/src/nsj_rest_lib/controller/patch_route.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     3931 2023-06-29 22:10:22.000000 nsj_rest_lib-1.2.1/src/nsj_rest_lib/controller/post_route.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     4341 2023-06-29 22:10:52.000000 nsj_rest_lib-1.2.1/src/nsj_rest_lib/controller/put_route.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     4664 2023-06-29 21:26:20.000000 nsj_rest_lib-1.2.1/src/nsj_rest_lib/controller/route_base.py
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-06-29 22:13:11.480819 nsj_rest_lib-1.2.1/src/nsj_rest_lib/dao/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-06-29 21:26:20.000000 nsj_rest_lib-1.2.1/src/nsj_rest_lib/dao/__init__.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)    17770 2023-06-29 21:26:20.000000 nsj_rest_lib-1.2.1/src/nsj_rest_lib/dao/dao_base.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     1223 2023-06-29 21:26:20.000000 nsj_rest_lib-1.2.1/src/nsj_rest_lib/db_pool_config.py
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-06-29 22:13:11.480819 nsj_rest_lib-1.2.1/src/nsj_rest_lib/decorator/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-06-29 21:26:20.000000 nsj_rest_lib-1.2.1/src/nsj_rest_lib/decorator/__init__.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     3987 2023-06-29 21:26:20.000000 nsj_rest_lib-1.2.1/src/nsj_rest_lib/decorator/dto.py
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-06-29 22:13:11.484819 nsj_rest_lib-1.2.1/src/nsj_rest_lib/descriptor/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-06-29 21:26:20.000000 nsj_rest_lib-1.2.1/src/nsj_rest_lib/descriptor/__init__.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     9827 2023-06-29 21:26:20.000000 nsj_rest_lib-1.2.1/src/nsj_rest_lib/descriptor/dto_field.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     7563 2023-06-29 21:26:20.000000 nsj_rest_lib-1.2.1/src/nsj_rest_lib/descriptor/dto_field_validators.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     5408 2023-06-29 21:26:20.000000 nsj_rest_lib-1.2.1/src/nsj_rest_lib/descriptor/dto_list_field.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      293 2023-06-29 21:26:20.000000 nsj_rest_lib-1.2.1/src/nsj_rest_lib/descriptor/filter_operator.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     2295 2023-06-29 21:26:20.000000 nsj_rest_lib-1.2.1/src/nsj_rest_lib/doc_route_generator.py
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-06-29 22:13:11.484819 nsj_rest_lib-1.2.1/src/nsj_rest_lib/dto/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-06-29 21:26:20.000000 nsj_rest_lib-1.2.1/src/nsj_rest_lib/dto/__init__.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     7290 2023-06-29 21:26:20.000000 nsj_rest_lib-1.2.1/src/nsj_rest_lib/dto/dto_base.py
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-06-29 22:13:11.484819 nsj_rest_lib-1.2.1/src/nsj_rest_lib/entity/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-06-29 21:26:20.000000 nsj_rest_lib-1.2.1/src/nsj_rest_lib/entity/__init__.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      710 2023-06-29 21:26:20.000000 nsj_rest_lib-1.2.1/src/nsj_rest_lib/entity/entity_base.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      322 2023-06-29 21:26:20.000000 nsj_rest_lib-1.2.1/src/nsj_rest_lib/entity/filter.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      483 2023-06-29 21:26:20.000000 nsj_rest_lib-1.2.1/src/nsj_rest_lib/exception.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     2856 2023-06-29 21:26:20.000000 nsj_rest_lib-1.2.1/src/nsj_rest_lib/healthcheck_config.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      825 2023-06-29 21:26:20.000000 nsj_rest_lib-1.2.1/src/nsj_rest_lib/injector_factory_base.py
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-06-29 22:13:11.484819 nsj_rest_lib-1.2.1/src/nsj_rest_lib/service/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-06-29 21:26:20.000000 nsj_rest_lib-1.2.1/src/nsj_rest_lib/service/__init__.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)    23612 2023-06-29 21:26:20.000000 nsj_rest_lib-1.2.1/src/nsj_rest_lib/service/service_base.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      707 2023-06-29 21:53:20.000000 nsj_rest_lib-1.2.1/src/nsj_rest_lib/settings.py
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-06-29 22:13:11.484819 nsj_rest_lib-1.2.1/src/nsj_rest_lib/validator/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-06-29 21:26:20.000000 nsj_rest_lib-1.2.1/src/nsj_rest_lib/validator/__init__.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     4196 2023-06-29 21:26:20.000000 nsj_rest_lib-1.2.1/src/nsj_rest_lib/validator/cpf_cnpj.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      527 2023-06-29 21:26:20.000000 nsj_rest_lib-1.2.1/src/nsj_rest_lib/validator/validate_data.py
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-06-29 22:13:11.480819 nsj_rest_lib-1.2.1/src/nsj_rest_lib.egg-info/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      743 2023-06-29 22:13:11.000000 nsj_rest_lib-1.2.1/src/nsj_rest_lib.egg-info/PKG-INFO
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     1652 2023-06-29 22:13:11.000000 nsj_rest_lib-1.2.1/src/nsj_rest_lib.egg-info/SOURCES.txt
--rw-rw-r--   0 sergio    (1000) sergio    (1000)        1 2023-06-29 22:13:11.000000 nsj_rest_lib-1.2.1/src/nsj_rest_lib.egg-info/dependency_links.txt
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      113 2023-06-29 22:13:11.000000 nsj_rest_lib-1.2.1/src/nsj_rest_lib.egg-info/requires.txt
--rw-rw-r--   0 sergio    (1000) sergio    (1000)       13 2023-06-29 22:13:11.000000 nsj_rest_lib-1.2.1/src/nsj_rest_lib.egg-info/top_level.txt
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-07-02 01:03:11.882687 nsj_rest_lib-1.3.0/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      743 2023-07-02 01:03:11.882687 nsj_rest_lib-1.3.0/PKG-INFO
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      130 2023-06-29 21:26:20.000000 nsj_rest_lib-1.3.0/README.md
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      103 2023-06-29 21:26:20.000000 nsj_rest_lib-1.3.0/pyproject.toml
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      888 2023-07-02 01:03:11.882687 nsj_rest_lib-1.3.0/setup.cfg
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-07-02 01:03:11.866687 nsj_rest_lib-1.3.0/src/
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-07-02 01:03:11.870687 nsj_rest_lib-1.3.0/src/nsj_rest_lib/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-06-29 21:26:20.000000 nsj_rest_lib-1.3.0/src/nsj_rest_lib/__init__.py
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-07-02 01:03:11.874687 nsj_rest_lib-1.3.0/src/nsj_rest_lib/controller/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-06-29 21:26:20.000000 nsj_rest_lib-1.3.0/src/nsj_rest_lib/controller/__init__.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)       75 2023-06-29 21:26:20.000000 nsj_rest_lib-1.3.0/src/nsj_rest_lib/controller/controller_util.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     3298 2023-06-29 22:11:32.000000 nsj_rest_lib-1.3.0/src/nsj_rest_lib/controller/delete_route.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      944 2023-06-29 21:26:20.000000 nsj_rest_lib-1.3.0/src/nsj_rest_lib/controller/funtion_route_wrapper.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     3907 2023-06-29 22:11:52.000000 nsj_rest_lib-1.3.0/src/nsj_rest_lib/controller/get_route.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     4590 2023-07-01 23:25:08.000000 nsj_rest_lib-1.3.0/src/nsj_rest_lib/controller/list_route.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     4351 2023-06-29 22:09:50.000000 nsj_rest_lib-1.3.0/src/nsj_rest_lib/controller/patch_route.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     3931 2023-06-29 22:10:22.000000 nsj_rest_lib-1.3.0/src/nsj_rest_lib/controller/post_route.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     4341 2023-06-29 22:10:52.000000 nsj_rest_lib-1.3.0/src/nsj_rest_lib/controller/put_route.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     4664 2023-06-29 21:26:20.000000 nsj_rest_lib-1.3.0/src/nsj_rest_lib/controller/route_base.py
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-07-02 01:03:11.874687 nsj_rest_lib-1.3.0/src/nsj_rest_lib/dao/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-06-29 21:26:20.000000 nsj_rest_lib-1.3.0/src/nsj_rest_lib/dao/__init__.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)    21249 2023-07-02 00:37:26.000000 nsj_rest_lib-1.3.0/src/nsj_rest_lib/dao/dao_base.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     1223 2023-06-29 21:26:20.000000 nsj_rest_lib-1.3.0/src/nsj_rest_lib/db_pool_config.py
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-07-02 01:03:11.878687 nsj_rest_lib-1.3.0/src/nsj_rest_lib/decorator/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-06-29 21:26:20.000000 nsj_rest_lib-1.3.0/src/nsj_rest_lib/decorator/__init__.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     4737 2023-07-01 22:57:27.000000 nsj_rest_lib-1.3.0/src/nsj_rest_lib/decorator/dto.py
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-07-02 01:03:11.878687 nsj_rest_lib-1.3.0/src/nsj_rest_lib/descriptor/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-06-29 21:26:20.000000 nsj_rest_lib-1.3.0/src/nsj_rest_lib/descriptor/__init__.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      418 2023-07-01 22:04:56.000000 nsj_rest_lib-1.3.0/src/nsj_rest_lib/descriptor/conjunto_type.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)    13010 2023-07-02 00:10:05.000000 nsj_rest_lib-1.3.0/src/nsj_rest_lib/descriptor/dto_field.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     7563 2023-06-29 21:26:20.000000 nsj_rest_lib-1.3.0/src/nsj_rest_lib/descriptor/dto_field_validators.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     5408 2023-06-29 21:26:20.000000 nsj_rest_lib-1.3.0/src/nsj_rest_lib/descriptor/dto_list_field.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      320 2023-07-02 00:29:03.000000 nsj_rest_lib-1.3.0/src/nsj_rest_lib/descriptor/filter_operator.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     2295 2023-06-29 21:26:20.000000 nsj_rest_lib-1.3.0/src/nsj_rest_lib/doc_route_generator.py
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-07-02 01:03:11.878687 nsj_rest_lib-1.3.0/src/nsj_rest_lib/dto/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-06-29 21:26:20.000000 nsj_rest_lib-1.3.0/src/nsj_rest_lib/dto/__init__.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     7570 2023-07-01 22:55:41.000000 nsj_rest_lib-1.3.0/src/nsj_rest_lib/dto/dto_base.py
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-07-02 01:03:11.878687 nsj_rest_lib-1.3.0/src/nsj_rest_lib/entity/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-06-29 21:26:20.000000 nsj_rest_lib-1.3.0/src/nsj_rest_lib/entity/__init__.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      710 2023-06-29 21:26:20.000000 nsj_rest_lib-1.3.0/src/nsj_rest_lib/entity/entity_base.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      322 2023-06-29 21:26:20.000000 nsj_rest_lib-1.3.0/src/nsj_rest_lib/entity/filter.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      483 2023-06-29 21:26:20.000000 nsj_rest_lib-1.3.0/src/nsj_rest_lib/exception.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     2856 2023-06-29 21:26:20.000000 nsj_rest_lib-1.3.0/src/nsj_rest_lib/healthcheck_config.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      825 2023-06-29 21:26:20.000000 nsj_rest_lib-1.3.0/src/nsj_rest_lib/injector_factory_base.py
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-07-02 01:03:11.882687 nsj_rest_lib-1.3.0/src/nsj_rest_lib/service/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-06-29 21:26:20.000000 nsj_rest_lib-1.3.0/src/nsj_rest_lib/service/__init__.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)    24073 2023-07-02 00:47:53.000000 nsj_rest_lib-1.3.0/src/nsj_rest_lib/service/service_base.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      707 2023-06-29 21:53:20.000000 nsj_rest_lib-1.3.0/src/nsj_rest_lib/settings.py
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-07-02 01:03:11.882687 nsj_rest_lib-1.3.0/src/nsj_rest_lib/validator/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-06-29 21:26:20.000000 nsj_rest_lib-1.3.0/src/nsj_rest_lib/validator/__init__.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     4196 2023-06-29 21:26:20.000000 nsj_rest_lib-1.3.0/src/nsj_rest_lib/validator/cpf_cnpj.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      527 2023-06-29 21:26:20.000000 nsj_rest_lib-1.3.0/src/nsj_rest_lib/validator/validate_data.py
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-07-02 01:03:11.870687 nsj_rest_lib-1.3.0/src/nsj_rest_lib.egg-info/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      743 2023-07-02 01:03:11.000000 nsj_rest_lib-1.3.0/src/nsj_rest_lib.egg-info/PKG-INFO
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     1697 2023-07-02 01:03:11.000000 nsj_rest_lib-1.3.0/src/nsj_rest_lib.egg-info/SOURCES.txt
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        1 2023-07-02 01:03:11.000000 nsj_rest_lib-1.3.0/src/nsj_rest_lib.egg-info/dependency_links.txt
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      113 2023-07-02 01:03:11.000000 nsj_rest_lib-1.3.0/src/nsj_rest_lib.egg-info/requires.txt
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)       13 2023-07-02 01:03:11.000000 nsj_rest_lib-1.3.0/src/nsj_rest_lib.egg-info/top_level.txt
```

### Comparing `nsj_rest_lib-1.2.1/PKG-INFO` & `nsj_rest_lib-1.3.0/src/nsj_rest_lib.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: nsj_rest_lib
-Version: 1.2.1
+Name: nsj-rest-lib
+Version: 1.3.0
 Summary: Biblioteca para construção de APIs Rest Python, de acordo com o guidelines interno, e com paradigma declarativo.
 Home-page: https://github.com/Nasajon/nsj_rest_lib
 Author: Nasajon Sistemas
 Author-email: contact.dev@nasajon.com.br
 Project-URL: Source, https://github.com/Nasajon/nsj_rest_lib
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `nsj_rest_lib-1.2.1/setup.cfg` & `nsj_rest_lib-1.3.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = nsj_rest_lib
-version = 1.2.1
+version = 1.3.0
 author = Nasajon Sistemas
 author_email = contact.dev@nasajon.com.br
 description = Biblioteca para construção de APIs Rest Python, de acordo com o guidelines interno, e com paradigma declarativo.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/Nasajon/nsj_rest_lib
 project_urls =
```

### Comparing `nsj_rest_lib-1.2.1/src/nsj_rest_lib/controller/delete_route.py` & `nsj_rest_lib-1.3.0/src/nsj_rest_lib/controller/delete_route.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-1.2.1/src/nsj_rest_lib/controller/funtion_route_wrapper.py` & `nsj_rest_lib-1.3.0/src/nsj_rest_lib/controller/funtion_route_wrapper.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-1.2.1/src/nsj_rest_lib/controller/get_route.py` & `nsj_rest_lib-1.3.0/src/nsj_rest_lib/controller/get_route.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-1.2.1/src/nsj_rest_lib/controller/list_route.py` & `nsj_rest_lib-1.3.0/src/nsj_rest_lib/controller/list_route.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,56 +42,58 @@
         """
 
         with self._injector_factory() as factory:
             try:
                 # Recuperando os parâmetros básicos
                 base_url = request.base_url
                 args = request.args
-                limit = int(args.get('limit', DEFAULT_PAGE_SIZE))
-                current_after = args.get('after') or args.get('offset')
+                limit = int(args.get("limit", DEFAULT_PAGE_SIZE))
+                current_after = args.get("after") or args.get("offset")
 
                 # Tratando dos fields
-                fields = args.get('fields')
+                fields = args.get("fields")
                 fields = self._parse_fields(fields)
 
                 # Tratando dos filters
                 filters = {}
                 for arg in args:
-                    if arg in ['limit', 'after', 'offset', 'fields', 'tenant', 'grupo_empresarial']:
+                    if arg in ["limit", "after", "offset", "fields"]:
+                        continue
+
+                    if arg in self._dto_class.partition_fields:
                         continue
 
                     filters[arg] = args.get(arg)
 
                 # Tratando campos de particionamento
                 for field in self._dto_class.partition_fields:
                     value = args.get(field)
                     if value is None:
                         raise MissingParameterException(field)
-                    
+
                     filters[field] = value
 
                 # Construindo os objetos
                 service = self._get_service(factory)
 
                 # Chamando o service (método list)
                 # TODO Rever parametro order_fields abaixo
-                data = service.list(current_after, limit,
-                                    fields, None, filters)
+                data = service.list(current_after, limit, fields, None, filters)
 
                 # Convertendo para o formato de dicionário (permitindo omitir campos do DTO)
                 dict_data = [dto.convert_to_dict(fields) for dto in data]
 
                 # Construindo o corpo da página
                 page = page_body(
                     base_url=base_url,
                     limit=limit,
                     current_after=current_after,
                     current_before=None,
                     result=dict_data,
-                    id_field='id'  # TODO Rever esse parâmetro
+                    id_field="id",  # TODO Rever esse parâmetro
                 )
 
                 # Retornando a resposta da requuisição
                 return (json_dumps(page), 200, {**DEFAULT_RESP_HEADERS})
             except MissingParameterException as e:
                 get_logger().warning(e)
                 if self._handle_exception is not None:
@@ -105,8 +107,12 @@
                 else:
                     return (format_json_error(e), 400, {**DEFAULT_RESP_HEADERS})
             except Exception as e:
                 get_logger().exception(e)
                 if self._handle_exception is not None:
                     return self._handle_exception(e)
                 else:
-                    return (format_json_error(f'Erro desconhecido: {e}'), 500, {**DEFAULT_RESP_HEADERS})
+                    return (
+                        format_json_error(f"Erro desconhecido: {e}"),
+                        500,
+                        {**DEFAULT_RESP_HEADERS},
+                    )
```

### Comparing `nsj_rest_lib-1.2.1/src/nsj_rest_lib/controller/patch_route.py` & `nsj_rest_lib-1.3.0/src/nsj_rest_lib/controller/patch_route.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-1.2.1/src/nsj_rest_lib/controller/post_route.py` & `nsj_rest_lib-1.3.0/src/nsj_rest_lib/controller/post_route.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-1.2.1/src/nsj_rest_lib/controller/put_route.py` & `nsj_rest_lib-1.3.0/src/nsj_rest_lib/controller/put_route.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-1.2.1/src/nsj_rest_lib/controller/route_base.py` & `nsj_rest_lib-1.3.0/src/nsj_rest_lib/controller/route_base.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-1.2.1/src/nsj_rest_lib/dao/dao_base.py` & `nsj_rest_lib-1.3.0/src/nsj_rest_lib/dao/dao_base.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import enum
 import uuid
 
 from typing import Any, Dict, List, Tuple
 
+from nsj_rest_lib.descriptor.conjunto_type import ConjuntoType
 from nsj_rest_lib.descriptor.filter_operator import FilterOperator
 from nsj_rest_lib.entity.entity_base import EntityBase, EMPTY
 from nsj_rest_lib.entity.filter import Filter
 from nsj_rest_lib.exception import NotFoundException, AfterRecordNotFoundException
 
 from nsj_gcf_utils.db_adapter2 import DBAdapter2
 from nsj_gcf_utils.json_util import convert_to_dumps
@@ -14,19 +15,15 @@
 from nsj_rest_lib.settings import USE_SQL_RETURNING_CLAUSE
 
 
 class DAOBase:
     _db: DBAdapter2
     _entity_class: EntityBase
 
-    def __init__(
-        self,
-        db: DBAdapter2,
-        entity_class: EntityBase
-    ):
+    def __init__(self, db: DBAdapter2, entity_class: EntityBase):
         self._db = db
         self._entity_class = entity_class
 
     def begin(self):
         """
         Inicia uma transação no banco de dados
         """
@@ -61,18 +58,21 @@
         """
 
         # Creating entity instance
         entity = self._entity_class()
 
         # Building SQL fields
         if fields is None:
-            fields = [f"t0.{k}" for k in entity.__dict__ if not callable(
-                getattr(entity, k, None)) and not k.startswith('_')]
+            fields = [
+                f"t0.{k}"
+                for k in entity.__dict__
+                if not callable(getattr(entity, k, None)) and not k.startswith("_")
+            ]
 
-        return ', '.join(fields)
+        return ", ".join(fields)
 
     def get(self, id: uuid.UUID, fields: List[str] = None, filters=None) -> EntityBase:
         """
         Returns an entity instance by its ID.
         """
 
         # Creating a entity instance
@@ -89,39 +89,41 @@
             {entity.get_table_name()} as t0
         where
             t0.{entity.get_pk_field()} = :id
             {filters_where}
         """
         values = {"id": id}
         values.update(filter_values_map)
-                
+
         # Running query
-        resp = self._db.execute_query_to_model(
-            sql,
-            self._entity_class,
-            **values
-        )
+        resp = self._db.execute_query_to_model(sql, self._entity_class, **values)
 
         # Checking if ID was found
         if len(resp) <= 0:
             raise NotFoundException(
-                f'{self._entity_class.__name__} com id {id} não encontrado.')
+                f"{self._entity_class.__name__} com id {id} não encontrado."
+            )
 
         return resp[0]
 
-    def _make_filters_sql(self, filters: Dict[str, List[Filter]], with_and: bool = True, use_table_alias: bool = True) -> Tuple[str, Dict[str, Any]]:
+    def _make_filters_sql(
+        self,
+        filters: Dict[str, List[Filter]],
+        with_and: bool = True,
+        use_table_alias: bool = True,
+    ) -> Tuple[str, Dict[str, Any]]:
         """
         Interpreta os filtros, retornando uma tupla com formato (filters_where, filter_values_map), onde
         filters_where: Parte do SQL, a ser adicionada na cláusula where, para realização dos filtros
         filter_values_map: Dicionário com os valores dos filtros, a serem enviados na excução da query
 
         Se receber o parâmetro filters nulo ou vazio, retorna ('', {}).
         """
 
-        filters_where = ''
+        filters_where = ""
         filter_values_map = {}
         if filters is not None:
             filters_where = []
 
             # Iterating fields with filters
             for filter_field in filters:
                 field_filter_where_or = []
@@ -144,43 +146,56 @@
                         operator = ">="
                     elif condiction.operator == FilterOperator.LESS_OR_EQUAL_THAN:
                         operator = "<="
                     elif condiction.operator == FilterOperator.LIKE:
                         operator = "like"
                     elif condiction.operator == FilterOperator.ILIKE:
                         operator = "ilike"
+                    elif condiction.operator == FilterOperator.NOT_NULL:
+                        operator = "is not null"
 
                     # Making condiction alias
-                    condiction_alias = (
-                        f"ft_{condiction.operator.value}_{filter_field}_{idx}"
-                    )
+                    if not (condiction.operator == FilterOperator.NOT_NULL):
+                        condiction_alias = (
+                            f"ft_{condiction.operator.value}_{filter_field}_{idx}"
+                        )
+                        condiction_alias_subtituir = f":{condiction_alias}"
+                    else:
+                        condiction_alias = ""
+                        condiction_alias_subtituir = ""
 
                     # Making condiction buffer
                     if use_table_alias:
                         condiction_buffer = (
-                            f"t0.{filter_field} {operator} :{condiction_alias}"
+                            f"t0.{filter_field} {operator} {condiction_alias_subtituir}"
                         )
                     else:
                         condiction_buffer = (
-                            f"{filter_field} {operator} :{condiction_alias}"
+                            f"{filter_field} {operator} {condiction_alias_subtituir}"
                         )
 
                     # Storing field filter where
                     if operator == "=" or operator == "like" or operator == "ilike":
                         field_filter_where_or.append(condiction_buffer)
                     else:
                         field_filter_where_and.append(condiction_buffer)
 
                     # Storing condiction value
-                    if condiction.value is not None and isinstance(
-                        condiction.value.__class__, enum.EnumMeta
-                    ):
-                        filter_values_map[condiction_alias] = condiction.value.value
-                    else:
-                        filter_values_map[condiction_alias] = condiction.value
+                    if condiction.value is not None:
+                        if isinstance(condiction.value.__class__, enum.EnumMeta):
+                            if isinstance(condiction.value.value, tuple):
+                                filter_values_map[
+                                    condiction_alias
+                                ] = condiction.value.value[1]
+                            else:
+                                filter_values_map[
+                                    condiction_alias
+                                ] = condiction.value.value
+                        else:
+                            filter_values_map[condiction_alias] = condiction.value
 
                     if operator == "like" or operator == "ilike":
                         filter_values_map[
                             condiction_alias
                         ] = f"%{filter_values_map[condiction_alias]}%"
 
                 # Formating condictions (with OR)
@@ -191,27 +206,29 @@
                     filters_where.append(field_filter_where_or)
 
                 if field_filter_where_and.strip() != "":
                     field_filter_where_and = f"({field_filter_where_and})"
                     filters_where.append(field_filter_where_and)
 
             # Formating all filters (with AND)
-            filters_where = '\n and '.join(filters_where)
-            if filters_where.strip() != '' and with_and:
+            filters_where = "\n and ".join(filters_where)
+            if filters_where.strip() != "" and with_and:
                 filters_where = f"and {filters_where}"
 
         return (filters_where, filter_values_map)
 
     def list(
         self,
         after: uuid.UUID,
         limit: int,
         fields: List[str],
         order_fields: List[str],
-        filters: Dict[str, List[Filter]]
+        filters: Dict[str, List[Filter]],
+        conjunto_type: ConjuntoType = None,
+        conjunto_field: str = None,
     ) -> List[EntityBase]:
         """
         Returns a paginated entity list.
         """
 
         # Creating a entity instance
         entity = self._entity_class()
@@ -227,113 +244,180 @@
         order_map = {field: None for field in order_fields}
 
         if after is not None:
             try:
                 after_obj = self.get(after)
             except NotFoundException as e:
                 raise AfterRecordNotFoundException(
-                    f'Identificador recebido no parâmetro after {id}, não encontrado para a entidade {self._entity_class.__name__}.')
+                    f"Identificador recebido no parâmetro after {id}, não encontrado para a entidade {self._entity_class.__name__}."
+                )
 
             if after_obj is not None:
                 for field in order_fields:
                     order_map[field] = getattr(after_obj, field, None)
 
         # Making default order by clause
         order_by = f"""
             {', '.join(order_fields_alias)}
         """
 
         # Organizando o where da paginação
-        pagination_where = ''
+        pagination_where = ""
         if after is not None:
-
             # Making a list of pagination condictions
             list_page_where = []
             old_fields = []
             for field in order_fields:
                 # Making equals condictions
-                buffer_old_fields = 'true'
+                buffer_old_fields = "true"
                 for of in old_fields:
                     buffer_old_fields += f" and t0.{of} = :{of}"
 
                 # Making current more than condiction
                 list_page_where.append(
-                    f"({buffer_old_fields} and t0.{field} > :{field})")
+                    f"({buffer_old_fields} and t0.{field} > :{field})"
+                )
 
                 # Storing current field as old
                 old_fields.append(field)
 
             # Making SQL page condiction
             pagination_where = f"""
                 and (
                     false
                     or {' or '.join(list_page_where)}
                 )
             """
 
+        # Resulvendo o join de conjuntos (se houver)
+        with_conjunto = ""
+        fields_conjunto = ""
+        join_conjuntos = ""
+        conjunto_map = {}
+        if conjunto_type is not None:
+            (
+                join_conjuntos,
+                with_conjunto,
+                fields_conjunto,
+                conjunto_map,
+            ) = self._make_conjunto_sql(conjunto_type, entity, filters, conjunto_field)
+
         # Organizando o where dos filtros
         filters_where, filter_values_map = self._make_filters_sql(filters)
 
         # Montando a query em si
         sql = f"""
+        {with_conjunto}
         select
 
+            {fields_conjunto}
             {self._sql_fields(fields)}
 
         from
             {entity.get_table_name()} as t0
+            {join_conjuntos}
+
         where
             true
             {pagination_where}
             {filters_where}
+
         order by
             {order_by}
         """
 
         # Adding limit if received
         if limit is not None:
             sql += f"        limit {limit}"
 
         # Making the values dict
-        kwargs = {
-            **order_map,
-            **filter_values_map
-        }
+        kwargs = {**order_map, **filter_values_map, **conjunto_map}
 
         # Running the SQL query
-        resp = self._db.execute_query_to_model(
-            sql,
-            self._entity_class,
-            **kwargs
-        )
+        resp = self._db.execute_query_to_model(sql, self._entity_class, **kwargs)
 
         return resp
 
+    def _make_conjunto_sql(
+        self,
+        conjunto_type: ConjuntoType,
+        entity: EntityBase,
+        filters: Dict[str, List[Filter]],
+        conjunto_field: str = None,
+    ):
+        tabela_conjunto = f"ns.conjuntos{conjunto_type.name.lower()}"
+        cadastro = conjunto_type.value
+
+        with_conjunto = f"""
+            with grupos_conjuntos as (
+                select
+                    gemp0.grupoempresarial as grupo_empresarial_pk,
+                    gemp0.codigo as grupo_empresarial_codigo,
+                    est_c0.conjunto
+                from ns.gruposempresariais gemp0
+                join ns.empresas emp0 on (emp0.grupoempresarial = gemp0.grupoempresarial and gemp0.codigo in :grupo_empresarial_conjunto_codigo)
+                join ns.estabelecimentos est0 on (est0.empresa = emp0.empresa)
+                join ns.estabelecimentosconjuntos est_c0 on (
+                    est_c0.estabelecimento = est0.estabelecimento
+                    and est_c0.cadastro = :conjunto_cadastro
+                )
+                group by gemp0.grupoempresarial, gemp0.codigo, est_c0.conjunto
+            )    
+            """
+
+        join_conjuntos = f"""
+            join {tabela_conjunto} as cr0 on (t0.{entity.get_pk_field()} = cr0.registro)
+            join grupos_conjuntos as gc0 on (gc0.conjunto = cr0.conjunto)
+            """
+
+        fields_conjunto = f"""
+            gc0.grupo_empresarial_pk,
+            gc0.grupo_empresarial_codigo,
+            gc0.conjunto as conjunto,
+            """
+
+        # Motando os parâmetros de conjuntos para a query
+        valores_filtro = []
+        for filtro in filters[conjunto_field]:
+            valores_filtro.append(filtro.value)
+
+        conjunto_map = {
+            "conjunto_cadastro": cadastro,
+            "grupo_empresarial_conjunto_codigo": tuple(valores_filtro),
+        }
+
+        del filters[conjunto_field]
+
+        return join_conjuntos, with_conjunto, fields_conjunto, conjunto_map
+
     def _sql_insert_fields(self) -> str:
         """
         Retorna uma tupla com duas partes: (sql_fields, sql_ref_values), onde:
         - sql_fields: Lista de campos a inserir no insert
         - sql_ref_values: Lista das referências aos campos, a inserir no insert (parte values)
         """
 
         # Creating entity instance
         entity = self._entity_class()
 
         # Building SQL fields
-        fields = [f"{k}" for k in entity.__dict__ if not callable(
-            getattr(entity, k, None)) and not k.startswith('_')]
-        ref_values = [f":{k}" for k in entity.__dict__ if not callable(
-            getattr(entity, k, None)) and not k.startswith('_')]
+        fields = [
+            f"{k}"
+            for k in entity.__dict__
+            if not callable(getattr(entity, k, None)) and not k.startswith("_")
+        ]
+        ref_values = [
+            f":{k}"
+            for k in entity.__dict__
+            if not callable(getattr(entity, k, None)) and not k.startswith("_")
+        ]
 
-        return (', '.join(fields), ', '.join(ref_values))
+        return (", ".join(fields), ", ".join(ref_values))
 
-    def insert(
-        self,
-        entity: EntityBase
-    ):
+    def insert(self, entity: EntityBase):
         """
         Insere o objeto de entidade "entity" no banco de dados
         """
 
         # Montando as cláusulas dos campos
         sql_fields, sql_ref_values = self._sql_insert_fields()
 
@@ -350,31 +434,29 @@
         )
         """
 
         # Montando as cláusulas returning
         returning_fields = entity.get_insert_returning_fields()
 
         if returning_fields is not None and USE_SQL_RETURNING_CLAUSE:
-            sql_returning = ', '.join(returning_fields)
+            sql_returning = ", ".join(returning_fields)
 
             sql += "\n"
             sql += f"returning {sql_returning}"
 
         # Montando um dicionário com valores das propriedades
         values_map = convert_to_dumps(entity)
 
         # Realizando o insert no BD
-        rowcount, returning = self._db.execute(
-            sql,
-            **values_map
-        )
+        rowcount, returning = self._db.execute(sql, **values_map)
 
         if rowcount <= 0:
             raise Exception(
-                f"Erro inserindo {entity.__class__.__name__} no banco de dados")
+                f"Erro inserindo {entity.__class__.__name__} no banco de dados"
+            )
 
         # Complementando o objeto com os dados de retorno
         if returning_fields is not None and USE_SQL_RETURNING_CLAUSE:
             for field in returning_fields:
                 setattr(entity, field, returning[0][field])
 
         return entity
@@ -382,43 +464,54 @@
     def _sql_update_fields(self, entity: EntityBase, ignore_nones: bool = False) -> str:
         """
         Retorna lista com os campos para update, no padrão "field = :field"
         """
 
         # Building SQL fields
         if ignore_nones:
-            fields = [f"{k} = :{k}" for k in entity.__dict__ if not callable(
-                getattr(entity, k, None)) and not k.startswith('_') and getattr(entity, k) is not None and k not in entity.get_const_fields()]
+            fields = [
+                f"{k} = :{k}"
+                for k in entity.__dict__
+                if not callable(getattr(entity, k, None))
+                and not k.startswith("_")
+                and getattr(entity, k) is not None
+                and k not in entity.get_const_fields()
+            ]
         else:
-            fields = [f"{k} = :{k}" for k in entity.__dict__ if not callable(
-                getattr(entity, k, None)) and not k.startswith('_') and k not in entity.get_const_fields()]
+            fields = [
+                f"{k} = :{k}"
+                for k in entity.__dict__
+                if not callable(getattr(entity, k, None))
+                and not k.startswith("_")
+                and k not in entity.get_const_fields()
+            ]
 
-        return ', '.join(fields)
+        return ", ".join(fields)
 
     def update(
         self,
         entity: EntityBase,
         filters: Dict[str, List[Filter]],
-        partial_update: bool = False
+        partial_update: bool = False,
     ):
         """
         Atualiza o objeto de entidade "entity" no banco de dados
         """
 
         # Montando a cláusula dos campos
         sql_fields = self._sql_update_fields(entity, partial_update)
 
         # Organizando o where dos filtros
-        filters_where, filter_values_map = self._make_filters_sql(
-            filters, False, False)
+        filters_where, filter_values_map = self._make_filters_sql(filters, False, False)
 
         # CUIDADO PARA NÂO ATUALIZAR O QUE NÃO DEVE
-        if filters_where is None or filters_where.strip() == '':
+        if filters_where is None or filters_where.strip() == "":
             raise NotFoundException(
-                f'{self._entity_class.__name__} não encontrado. Filtros: {filters}')
+                f"{self._entity_class.__name__} não encontrado. Filtros: {filters}"
+            )
 
         # Montando a query principal
         sql = f"""
         update {entity.get_table_name()} set
 
             {sql_fields}
 
@@ -427,43 +520,38 @@
             {filters_where}
         """
 
         # Montando as cláusulas returning
         returning_fields = entity.get_update_returning_fields()
 
         if returning_fields is not None and USE_SQL_RETURNING_CLAUSE:
-            sql_returning = ', '.join(returning_fields)
+            sql_returning = ", ".join(returning_fields)
 
             sql += "\n"
             sql += f"returning {sql_returning}"
 
         # Montando um dicionário com valores das propriedades
         values_map = convert_to_dumps(entity)
 
         # Convertendo EMPTY para None, se necessário
         if partial_update:
             for key in values_map:
                 if values_map[key] == EMPTY:
                     values_map[key] = None
 
         # Montado o map de valores a passar no update
-        kwargs = {
-            **values_map,
-            **filter_values_map
-        }
+        kwargs = {**values_map, **filter_values_map}
 
         # Realizando o update no BD
-        rowcount, returning = self._db.execute(
-            sql,
-            **kwargs
-        )
+        rowcount, returning = self._db.execute(sql, **kwargs)
 
         if rowcount <= 0:
             raise NotFoundException(
-                f'{self._entity_class.__name__} com id {values_map[self._entity_class().get_pk_field()]} não encontrado.')
+                f"{self._entity_class.__name__} com id {values_map[self._entity_class().get_pk_field()]} não encontrado."
+            )
 
         # Complementando o objeto com os dados de retorno
         if returning_fields is not None and USE_SQL_RETURNING_CLAUSE:
             for field in returning_fields:
                 setattr(entity, field, returning[0][field])
 
         return entity
@@ -488,18 +576,15 @@
 
         # Montando a query
         sql = f"""
         select {pk_field} from {entity.get_table_name()} as t0 where true {filters_where}
         """
 
         # Executando a query
-        resp = self._db.execute_query(
-            sql,
-            **filter_values_map
-        )
+        resp = self._db.execute_query(sql, **filter_values_map)
 
         # Retornando em formato de lista de IDs
         if resp is None:
             return None
         else:
             return [item[pk_field] for item in resp]
 
@@ -507,36 +592,35 @@
         """
         Exclui registros de acordo com os filtros recebidos.
         """
 
         # Retorna None, se não receber filtros
         if filters is None or len(filters) <= 0:
             raise NotFoundException(
-                f'{self._entity_class.__name__} não encontrado. Filtros: {filters}')
+                f"{self._entity_class.__name__} não encontrado. Filtros: {filters}"
+            )
 
         # Montando uma entity fake
         entity = self._entity_class()
 
         # Organizando o where dos filtros
-        filters_where, filter_values_map = self._make_filters_sql(
-            filters, False, False)
+        filters_where, filter_values_map = self._make_filters_sql(filters, False, False)
 
         # CUIDADO PARA NÂO EXCLUIR O QUE NÃO DEVE
-        if filters_where is None or filters_where.strip() == '':
+        if filters_where is None or filters_where.strip() == "":
             raise NotFoundException(
-                f'{self._entity_class.__name__} não encontrado. Filtros: {filters}')
+                f"{self._entity_class.__name__} não encontrado. Filtros: {filters}"
+            )
 
         # Montando a query
         sql = f"""
         delete from {entity.get_table_name()} where {filters_where}
         """
 
         # Executando a query
-        rowcount, _ = self._db.execute(
-            sql,
-            **filter_values_map
-        )
+        rowcount, _ = self._db.execute(sql, **filter_values_map)
 
         # Verificando se houve alguma deleção
         if rowcount <= 0:
             raise NotFoundException(
-                f'{self._entity_class.__name__} não encontrado. Filtros: {filters}')
+                f"{self._entity_class.__name__} não encontrado. Filtros: {filters}"
+            )
```

### Comparing `nsj_rest_lib-1.2.1/src/nsj_rest_lib/db_pool_config.py` & `nsj_rest_lib-1.3.0/src/nsj_rest_lib/db_pool_config.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-1.2.1/src/nsj_rest_lib/descriptor/dto_field_validators.py` & `nsj_rest_lib-1.3.0/src/nsj_rest_lib/descriptor/dto_field_validators.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-1.2.1/src/nsj_rest_lib/descriptor/dto_list_field.py` & `nsj_rest_lib-1.3.0/src/nsj_rest_lib/descriptor/dto_list_field.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-1.2.1/src/nsj_rest_lib/doc_route_generator.py` & `nsj_rest_lib-1.3.0/src/nsj_rest_lib/doc_route_generator.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-1.2.1/src/nsj_rest_lib/dto/dto_base.py` & `nsj_rest_lib-1.3.0/src/nsj_rest_lib/dto/dto_base.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,33 +1,41 @@
 import abc
 import copy
+
 # import uuid
 
 from typing import Any, Dict, List, Set, Union
 
 from nsj_rest_lib.entity.entity_base import EMPTY, EntityBase
+from nsj_rest_lib.descriptor.conjunto_type import ConjuntoType
 from nsj_rest_lib.descriptor.dto_field import DTOField, DTOFieldFilter
 
 
 class DTOBase(abc.ABC):
     resume_fields: Set[str] = set()
     partition_fields: Set[str] = set()
     fields_map: Dict[str, DTOField] = {}
     list_fields_map: dict = {}
     field_filters_map: Dict[str, DTOFieldFilter]
     # TODO Refatorar para suportar PK composto
     pk_field: str
     fixed_filters: Dict[str, Any]
+    conjunto_type: ConjuntoType
+    conjunto_field: str
 
     def __init__(self, entity: Union[EntityBase, dict] = None, **kwargs) -> None:
         super().__init__()
 
         # Transformando a entity em dict (se houver uma entity)
         if entity is not None:
-            kwargs =  copy.deepcopy(entity) if type(entity) is dict else copy.deepcopy(entity.__dict__)
+            kwargs = (
+                copy.deepcopy(entity)
+                if type(entity) is dict
+                else copy.deepcopy(entity.__dict__)
+            )
 
         # Setando os campos registrados como fields simples
         for field in self.__class__.fields_map:
             # Recuperando a configuração do campo
             dto_field = self.__class__.fields_map[field]
 
             # Tratando do valor default
@@ -35,46 +43,60 @@
                 default_value = dto_field.default_value
                 if callable(dto_field.default_value):
                     default_value = dto_field.default_value()
                 kwargs[field] = default_value
 
             # Verificando se é preciso converter o nome do field para o nome correspondente no Entity
             entity_field = field
-            if entity is not None:
-                if dto_field.entity_field is not None:
-                    entity_field = dto_field.entity_field
+            if dto_field.entity_field is not None:
+                entity_field = dto_field.entity_field
 
+            # Verificando se o campo carece de conversão customizada
+            if dto_field.convert_from_entity is not None:
+                fields_converted = dto_field.convert_from_entity(
+                    kwargs[entity_field], kwargs
+                )
+                if field not in fields_converted:
+                    setattr(self, field, None)
+
+                for converted_key in fields_converted:
+                    setattr(self, converted_key, fields_converted[converted_key])
+
+                continue
+
+            # Atribuindo o valor à propriedade do DTO
             if entity_field in kwargs:
                 setattr(self, field, kwargs[entity_field])
             else:
                 setattr(self, field, None)
 
         # Setando os campos registrados como fields de lista
         if entity is None:
             for field in self.__class__.list_fields_map:
                 dto_list_field = self.__class__.list_fields_map[field]
 
                 if field in kwargs:
                     if not isinstance(kwargs[field], list):
                         raise ValueError(
-                            f"O campo {field} deveria ser uma lista do tipo {dto_list_field.dto_type}.")
+                            f"O campo {field} deveria ser uma lista do tipo {dto_list_field.dto_type}."
+                        )
 
                     related_itens = []
                     for item in kwargs[field]:
                         # Preenchendo os campos de particionanmento, se necessário (normalmente: tenant e grupo_empresarial)
                         for partition_field in self.__class__.partition_fields:
                             if (
                                 (
                                     not (partition_field in item)
                                     or item[partition_field] is None
                                 )
-                                and partition_field in dto_list_field.dto_type.partition_fields
+                                and partition_field
+                                in dto_list_field.dto_type.partition_fields
                             ):
-                                partition_value = getattr(
-                                    self, partition_field)
+                                partition_value = getattr(self, partition_field)
                                 item[partition_field] = partition_value
 
                         # Criando o DTO relacionado
                         item_dto = dto_list_field.dto_type(**item)
 
                         # Adicionando o DTO na lista do relacionamento
                         related_itens.append(item_dto)
@@ -84,48 +106,14 @@
                     setattr(self, field, None)
 
         # Tratando do ID automático
         # if generate_pk_uuid:
         #     if getattr(self, self.__class__.pk_field) is None:
         #         setattr(self, self.__class__.pk_field, uuid.uuid4())
 
-    def convert_from_entity(self, obj: EntityBase):
-        """
-        Popula DTO a partir de um objeto de entidade (considerando
-        apenas as propriedades descritas como DTOFields).
-
-        Este método retorna self (a própria referencia ao objeto).
-        """
-
-        for attribute in self.__dict__:
-
-            # Ignoring non DTO fields
-            if not (attribute in self.__class__.fields_map):
-                continue
-
-            # Getting DTO field config
-            dto_field = self.__class__.fields_map[attribute]
-
-            # Checking if exists a different name to equivalent field in entity class
-            attr_name = attribute
-            if dto_field.entity_field is not None:
-                attr_name = dto_field.entity_field
-
-            # Checking if exists the equivalent attribute in entity object (skiping, if not)
-            if not hasattr(obj, attr_name):
-                continue
-
-            # Getting entity attribute
-            entity_attr = getattr(obj, attr_name, None)
-
-            # Setting value localy
-            setattr(self, attribute, entity_attr)
-
-        return self
-
     def convert_to_entity(self, entity_class: EntityBase, none_as_empty: bool = False):
         """
         Cria uma instância da entidade, e a popula com os dados do DTO
         corrente.
 
         É importante notar que as equivalências dos nomes dos campos
         são tratadas neste método.
@@ -142,60 +130,77 @@
             # Verificando se o campo existe na entity
             if not hasattr(entity, entity_field):
                 continue
 
             # Recuperando o valor
             value = getattr(self, field)
 
+            # Verificando se é necessária uma conversão customizada
+            if dto_field.convert_to_entity is not None:
+                fields_converted = dto_field.convert_to_entity(value, self)
+                if entity_field not in fields_converted:
+                    setattr(entity, entity_field, None if not none_as_empty else EMPTY)
+
+                for converted_key in fields_converted:
+                    value = fields_converted[converted_key]
+                    if value is None and none_as_empty:
+                        value = EMPTY
+                    setattr(entity, converted_key, value)
+
+                continue
+
             # Convertendo None para EMPTY (se desejado)
             if value is None and none_as_empty:
                 value = EMPTY
 
             # Setando na entidade
             setattr(entity, entity_field, value)
 
         return entity
 
-    def convert_to_dict(self, fields: Dict[str, List[str]] = None, just_resume: bool = False):
+    def convert_to_dict(
+        self, fields: Dict[str, List[str]] = None, just_resume: bool = False
+    ):
         """
         Converte DTO para dict
         """
 
         # Resolving fields to use
         if fields is None:
-            fields = {'root': self.resume_fields}
+            fields = {"root": self.resume_fields}
 
         if just_resume:
-            fields = {'root': self.resume_fields}
+            fields = {"root": self.resume_fields}
         else:
-            fields['root'] = fields['root'].union(self.resume_fields)
+            fields["root"] = fields["root"].union(self.resume_fields)
 
         # Making result maps
         result = {}
 
         # Converting simple fields
         for field in self.fields_map:
-            if not field in fields['root']:
+            if not field in fields["root"]:
                 continue
 
             result[field] = getattr(self, field)
 
         # Converting list fields
         for field in self.list_fields_map:
-            if not field in fields['root']:
+            if not field in fields["root"]:
                 continue
 
             # Criando o mapa de fileds para a entidade aninhada
             internal_fields = None
             if field in fields:
-                internal_fields = {'root': fields[field]}
+                internal_fields = {"root": fields[field]}
 
             # Recuperando o valor do atributo
             value = getattr(self, field)
             if value is None:
                 value = []
 
             # Convetendo a lista de DTOs aninhados
-            result[field] = [item.convert_to_dict(
-                internal_fields, just_resume) for item in value]
+            result[field] = [
+                item.convert_to_dict(internal_fields, just_resume) for item in value
+            ]
 
         return result
```

### Comparing `nsj_rest_lib-1.2.1/src/nsj_rest_lib/entity/entity_base.py` & `nsj_rest_lib-1.3.0/src/nsj_rest_lib/entity/entity_base.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-1.2.1/src/nsj_rest_lib/healthcheck_config.py` & `nsj_rest_lib-1.3.0/src/nsj_rest_lib/healthcheck_config.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-1.2.1/src/nsj_rest_lib/injector_factory_base.py` & `nsj_rest_lib-1.3.0/src/nsj_rest_lib/injector_factory_base.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-1.2.1/src/nsj_rest_lib/service/service_base.py` & `nsj_rest_lib-1.3.0/src/nsj_rest_lib/service/service_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,21 +69,29 @@
         """
         Convert a list of fields names to a list of entity fiedls names.
         """
 
         if fields is None:
             return None
 
+        # TODO Refatorar para não precisar deste objeto só por conta das propriedades da classe
+        # (um decorator na classe, poderia armazenar os fields na mesma, como é feito no DTO)
+        entity = self._entity_class()
+
         entity_fields = []
         for field in fields:
             # Skipping not DTO fields
             if not (field in self._dto_class.fields_map):
                 continue
 
             entity_field_name = self._convert_to_entity_field(field)
+            # Skipping not Entity fields
+            if not (entity_field_name in entity.__dict__):
+                continue
+
             entity_fields.append(entity_field_name)
 
         return entity_fields
 
     def _convert_to_entity_field(self, field: str) -> str:
         """
         Convert a field name to a entity field name.
@@ -106,30 +114,33 @@
 
         if filters is None:
             return None
 
         entity_filters = {}
         for filter in filters:
             is_entity_filter = False
+            is_conjunto_filter = False
             if filter in self._dto_class.field_filters_map:
                 # Retrieving filter config
                 field_filter = self._dto_class.field_filters_map[filter]
+            elif filter == self._dto_class.conjunto_field:
+                is_conjunto_filter = True
             elif filter in self._dto_class.fields_map:
                 # Creating filter config to a DTOField (equals operator)
                 field_filter = DTOFieldFilter(filter)
                 field_filter.set_field_name(filter)
             # TODO Refatorar para usar um mapa de fields do entity
             elif filter in self._entity_class().__dict__:
                 is_entity_filter = True
             else:
                 # Ignoring not declared filters (or filter for not existent DTOField)
                 continue
 
             # Resolving entity field name (to filter)
-            if not is_entity_filter:
+            if not is_entity_filter and not is_conjunto_filter:
                 entity_field_name = self._convert_to_entity_field(
                     field_filter.field_name
                 )
             else:
                 entity_field_name = filter
 
             # Creating entity filters (one for each value - separated by comma)
@@ -138,15 +149,15 @@
             else:
                 values = [filters[filter]]
 
             for value in values:
                 if isinstance(value, str):
                     value = value.strip()
 
-                if not is_entity_filter:
+                if not is_entity_filter and not is_conjunto_filter:
                     entity_filter = Filter(field_filter.operator, value)
                 else:
                     entity_filter = Filter(FilterOperator.EQUALS, value)
 
                 # Storing filter in dict
                 filter_list = entity_filters.setdefault(entity_field_name, [])
                 filter_list.append(entity_filter)
@@ -159,16 +170,15 @@
         """
 
         # Resolving fields
         if fields is None:
             result = {"root": set()}
         else:
             result = copy.deepcopy(fields)
-            result["root"] = result["root"].union(
-                self._dto_class.resume_fields)
+            result["root"] = result["root"].union(self._dto_class.resume_fields)
 
         return result
 
     def list(
         self,
         after: uuid.UUID,
         limit: int,
@@ -192,19 +202,24 @@
         if self._dto_class.fixed_filters is not None:
             all_filters.update(self._dto_class.fixed_filters)
 
         entity_filters = self._create_entity_filters(all_filters)
 
         # Retrieving from DAO
         entity_list = self._dao.list(
-            after, limit, entity_fields, order_fields, entity_filters)
+            after,
+            limit,
+            entity_fields,
+            order_fields,
+            entity_filters,
+            conjunto_type=self._dto_class.conjunto_type,
+            conjunto_field=self._dto_class.conjunto_field,
+        )
 
         # Convertendo para uma lista de DTOs
-        # dto_list = [self._dto_class().convert_from_entity(entity)
-        #             for entity in entity_list]
         dto_list = [self._dto_class(entity) for entity in entity_list]
 
         # Retrieving related lists
         if len(self._dto_class.list_fields_map) > 0:
             self._retrieve_related_lists(dto_list, fields)
 
         # Returning
@@ -370,16 +385,15 @@
                     )
                 else:
                     aditional_entity_filters = {}
 
                 entity_filters = {**id_filters, **aditional_entity_filters}
 
                 # Executando o update pelo DAO
-                entity = self._dao.update(
-                    entity, entity_filters, partial_update)
+                entity = self._dao.update(entity, entity_filters, partial_update)
 
             # Convertendo a entity para o DTO de resposta (se houver um)
             if self._dto_post_response_class is not None:
                 response_dto = self._dto_post_response_class(entity)
             else:
                 # Retorna None, se não se espera um DTO de resposta
                 response_dto = None
@@ -531,29 +545,27 @@
                 response_dto is not None
                 and master_dto_field in response_dto.list_fields_map
                 and list_field.dto_post_response_type is not None
             ):
                 setattr(response_dto, master_dto_field, response_list)
 
     def delete(self, id: Any, additional_filters: Dict[str, Any] = None) -> DTOBase:
-        self._delete(id, manage_transaction=True,
-                     additional_filters=additional_filters)
+        self._delete(id, manage_transaction=True, additional_filters=additional_filters)
 
     def entity_exists(self, entity: EntityBase, partition_fields: Dict[str, Any]):
         # Getting values
         entity_pk_field = entity.get_pk_field()
         entity_pk_value = getattr(entity, entity_pk_field)
 
         if entity_pk_value is None:
             return False
 
         # Searching entity in DB
         try:
-            self._dao.get(entity_pk_value, [
-                          entity.get_pk_field()], partition_fields)
+            self._dao.get(entity_pk_value, [entity.get_pk_field()], partition_fields)
         except NotFoundException as e:
             return False
 
         return True
 
     def _delete(
         self,
@@ -564,16 +576,15 @@
         try:
             if manage_transaction:
                 self._dao.begin()
 
             # Convertendo os filtros para os filtros de entidade
             entity_filters = {}
             if additional_filters is not None:
-                entity_filters = self._create_entity_filters(
-                    additional_filters)
+                entity_filters = self._create_entity_filters(additional_filters)
 
             # Adicionando o ID nos filtros
             id_condiction = Filter(FilterOperator.EQUALS, id)
 
             pk_field = self._entity_class().get_pk_field()
             entity_filters[pk_field] = [id_condiction]
 
@@ -595,29 +606,27 @@
     def _delete_related_lists(self, id, additional_filters: Dict[str, Any] = None):
         # Handling each related list
         for _, list_field in self._dto_class.list_fields_map.items():
             # Getting service instance
             # TODO Refatorar para suportar services customizados
             service = ServiceBase(
                 self._injector_factory,
-                DAOBase(self._injector_factory.db_adapter(),
-                        list_field.entity_type),
+                DAOBase(self._injector_factory.db_adapter(), list_field.entity_type),
                 list_field.dto_type,
                 list_field.entity_type,
             )
 
             # Making filter to relation
             filters = {
                 # TODO Adicionar os campos de particionamento de dados
                 list_field.related_entity_field: id
             }
 
             # Getting related data
-            related_dto_list = service.list(
-                None, None, {"root": set()}, None, filters)
+            related_dto_list = service.list(None, None, {"root": set()}, None, filters)
 
             # Excluindo cada entidade detalhe
             for related_dto in related_dto_list:
                 # Checking if pk_field exists
                 if list_field.dto_type.pk_field is None:
                     raise DTOListFieldConfigException(
                         f"PK field not found in class: {self._dto_class}"
```

### Comparing `nsj_rest_lib-1.2.1/src/nsj_rest_lib/settings.py` & `nsj_rest_lib-1.3.0/src/nsj_rest_lib/settings.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-1.2.1/src/nsj_rest_lib/validator/cpf_cnpj.py` & `nsj_rest_lib-1.3.0/src/nsj_rest_lib/validator/cpf_cnpj.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-1.2.1/src/nsj_rest_lib/validator/validate_data.py` & `nsj_rest_lib-1.3.0/src/nsj_rest_lib/validator/validate_data.py`

 * *Files identical despite different names*

### Comparing `nsj_rest_lib-1.2.1/src/nsj_rest_lib.egg-info/PKG-INFO` & `nsj_rest_lib-1.3.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: nsj-rest-lib
-Version: 1.2.1
+Name: nsj_rest_lib
+Version: 1.3.0
 Summary: Biblioteca para construção de APIs Rest Python, de acordo com o guidelines interno, e com paradigma declarativo.
 Home-page: https://github.com/Nasajon/nsj_rest_lib
 Author: Nasajon Sistemas
 Author-email: contact.dev@nasajon.com.br
 Project-URL: Source, https://github.com/Nasajon/nsj_rest_lib
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `nsj_rest_lib-1.2.1/src/nsj_rest_lib.egg-info/SOURCES.txt` & `nsj_rest_lib-1.3.0/src/nsj_rest_lib.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 src/nsj_rest_lib/controller/put_route.py
 src/nsj_rest_lib/controller/route_base.py
 src/nsj_rest_lib/dao/__init__.py
 src/nsj_rest_lib/dao/dao_base.py
 src/nsj_rest_lib/decorator/__init__.py
 src/nsj_rest_lib/decorator/dto.py
 src/nsj_rest_lib/descriptor/__init__.py
+src/nsj_rest_lib/descriptor/conjunto_type.py
 src/nsj_rest_lib/descriptor/dto_field.py
 src/nsj_rest_lib/descriptor/dto_field_validators.py
 src/nsj_rest_lib/descriptor/dto_list_field.py
 src/nsj_rest_lib/descriptor/filter_operator.py
 src/nsj_rest_lib/dto/__init__.py
 src/nsj_rest_lib/dto/dto_base.py
 src/nsj_rest_lib/entity/__init__.py
```

