# Comparing `tmp/granny-pliers-0.0.15.tar.gz` & `tmp/granny-pliers-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "granny-pliers-0.0.15.tar", last modified: Sat Jul  1 23:28:01 2023, max compression
+gzip compressed data, was "granny-pliers-0.0.9.tar", last modified: Wed Jun 14 21:02:38 2023, max compression
```

## Comparing `granny-pliers-0.0.15.tar` & `granny-pliers-0.0.9.tar`

### file list

```diff
@@ -1,75 +1,70 @@
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-07-01 23:28:01.596278 granny-pliers-0.0.15/
--rw-r--r--   0 pd         (501) staff       (20)    11357 2023-06-03 18:43:25.000000 granny-pliers-0.0.15/LICENSE
--rw-r--r--   0 pd         (501) staff       (20)    13701 2023-07-01 23:28:01.595788 granny-pliers-0.0.15/PKG-INFO
--rw-r--r--   0 pd         (501) staff       (20)       16 2023-06-10 17:39:54.000000 granny-pliers-0.0.15/README.md
--rw-r--r--   0 pd         (501) staff       (20)     1620 2023-07-01 23:27:31.000000 granny-pliers-0.0.15/pyproject.toml
--rw-r--r--   0 pd         (501) staff       (20)       38 2023-07-01 23:28:01.596387 granny-pliers-0.0.15/setup.cfg
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-07-01 23:28:01.569915 granny-pliers-0.0.15/src/
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-07-01 23:28:01.573369 granny-pliers-0.0.15/src/granny_pliers/
--rw-r--r--   0 pd         (501) staff       (20)      988 2023-07-01 23:27:31.000000 granny-pliers-0.0.15/src/granny_pliers/__init__.py
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-07-01 23:28:01.578685 granny-pliers-0.0.15/src/granny_pliers/auth/
--rw-r--r--   0 pd         (501) staff       (20)     1228 2023-06-10 13:12:31.000000 granny-pliers-0.0.15/src/granny_pliers/auth/__init__.py
--rw-r--r--   0 pd         (501) staff       (20)     1683 2023-06-10 11:50:56.000000 granny-pliers-0.0.15/src/granny_pliers/auth/auth_config.py
--rw-r--r--   0 pd         (501) staff       (20)      986 2023-06-10 13:13:15.000000 granny-pliers-0.0.15/src/granny_pliers/auth/auth_error.py
--rw-r--r--   0 pd         (501) staff       (20)     1308 2023-06-10 13:13:08.000000 granny-pliers-0.0.15/src/granny_pliers/auth/auth_request.py
--rw-r--r--   0 pd         (501) staff       (20)     1016 2023-06-10 13:11:55.000000 granny-pliers-0.0.15/src/granny_pliers/auth/auth_response.py
--rw-r--r--   0 pd         (501) staff       (20)     6158 2023-06-10 13:18:46.000000 granny-pliers-0.0.15/src/granny_pliers/auth/jwt.py
--rw-r--r--   0 pd         (501) staff       (20)      882 2023-06-10 11:26:21.000000 granny-pliers-0.0.15/src/granny_pliers/auth/permissions.py
--rw-r--r--   0 pd         (501) staff       (20)      828 2023-06-10 11:26:59.000000 granny-pliers-0.0.15/src/granny_pliers/auth/roles.py
--rw-r--r--   0 pd         (501) staff       (20)     9678 2023-06-10 13:14:07.000000 granny-pliers-0.0.15/src/granny_pliers/auth/rsa_codec.py
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-07-01 23:28:01.580888 granny-pliers-0.0.15/src/granny_pliers/config/
--rw-r--r--   0 pd         (501) staff       (20)      985 2023-06-04 16:29:44.000000 granny-pliers-0.0.15/src/granny_pliers/config/__init__.py
--rw-r--r--   0 pd         (501) staff       (20)     3198 2023-06-09 21:43:11.000000 granny-pliers-0.0.15/src/granny_pliers/config/abstract_config.py
--rw-r--r--   0 pd         (501) staff       (20)     1614 2023-06-03 23:39:30.000000 granny-pliers-0.0.15/src/granny_pliers/config/autowired_config.py
--rw-r--r--   0 pd         (501) staff       (20)     6694 2023-06-14 20:55:52.000000 granny-pliers-0.0.15/src/granny_pliers/config/logger_config.py
--rw-r--r--   0 pd         (501) staff       (20)      860 2023-06-03 18:43:25.000000 granny-pliers-0.0.15/src/granny_pliers/config/project_environment.py
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-07-01 23:28:01.582104 granny-pliers-0.0.15/src/granny_pliers/logger/
--rw-r--r--   0 pd         (501) staff       (20)      884 2023-06-04 16:29:44.000000 granny-pliers-0.0.15/src/granny_pliers/logger/__init__.py
--rw-r--r--   0 pd         (501) staff       (20)     1292 2023-06-03 18:43:25.000000 granny-pliers-0.0.15/src/granny_pliers/logger/abstract_logger.py
--rw-r--r--   0 pd         (501) staff       (20)     1253 2023-06-03 18:43:25.000000 granny-pliers-0.0.15/src/granny_pliers/logger/log_processors.py
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-07-01 23:28:01.582655 granny-pliers-0.0.15/src/granny_pliers/models/
--rw-r--r--   0 pd         (501) staff       (20)      620 2023-06-10 11:58:05.000000 granny-pliers-0.0.15/src/granny_pliers/models/__init__.py
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-07-01 23:28:01.583398 granny-pliers-0.0.15/src/granny_pliers/models/auth/
--rw-r--r--   0 pd         (501) staff       (20)      688 2023-06-10 13:33:22.000000 granny-pliers-0.0.15/src/granny_pliers/models/auth/__init__.py
--rw-r--r--   0 pd         (501) staff       (20)     2061 2023-06-10 13:36:39.000000 granny-pliers-0.0.15/src/granny_pliers/models/auth/user.py
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-07-01 23:28:01.584644 granny-pliers-0.0.15/src/granny_pliers/models/metrics/
--rw-r--r--   0 pd         (501) staff       (20)      715 2023-06-10 13:32:44.000000 granny-pliers-0.0.15/src/granny_pliers/models/metrics/__init__.py
--rw-r--r--   0 pd         (501) staff       (20)     2766 2023-06-10 13:33:13.000000 granny-pliers-0.0.15/src/granny_pliers/models/metrics/confusion_matrix.py
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-07-01 23:28:01.585535 granny-pliers-0.0.15/src/granny_pliers/models/web/
--rw-r--r--   0 pd         (501) staff       (20)      729 2023-06-10 13:36:51.000000 granny-pliers-0.0.15/src/granny_pliers/models/web/__init__.py
--rw-r--r--   0 pd         (501) staff       (20)     1645 2023-06-10 11:59:08.000000 granny-pliers-0.0.15/src/granny_pliers/models/web/web_service_health_status.py
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-07-01 23:28:01.587939 granny-pliers-0.0.15/src/granny_pliers/orm/
--rw-r--r--   0 pd         (501) staff       (20)     1222 2023-06-10 13:29:12.000000 granny-pliers-0.0.15/src/granny_pliers/orm/__init__.py
--rw-r--r--   0 pd         (501) staff       (20)     5494 2023-06-10 13:26:46.000000 granny-pliers-0.0.15/src/granny_pliers/orm/abstract_http_client.py
--rw-r--r--   0 pd         (501) staff       (20)     5956 2023-06-10 13:25:56.000000 granny-pliers-0.0.15/src/granny_pliers/orm/abstract_http_repository.py
--rw-r--r--   0 pd         (501) staff       (20)     3296 2023-07-01 23:04:28.000000 granny-pliers-0.0.15/src/granny_pliers/orm/abstract_model.py
--rw-r--r--   0 pd         (501) staff       (20)    20143 2023-07-01 23:15:10.000000 granny-pliers-0.0.15/src/granny_pliers/orm/abstract_mongo_repository.py
--rw-r--r--   0 pd         (501) staff       (20)     7787 2023-07-01 23:12:10.000000 granny-pliers-0.0.15/src/granny_pliers/orm/abstract_repository.py
--rw-r--r--   0 pd         (501) staff       (20)    14519 2023-06-10 17:09:48.000000 granny-pliers-0.0.15/src/granny_pliers/orm/restful_http_client.py
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-07-01 23:28:01.589884 granny-pliers-0.0.15/src/granny_pliers/scheduler/
--rw-r--r--   0 pd         (501) staff       (20)      194 2023-06-25 17:48:19.000000 granny-pliers-0.0.15/src/granny_pliers/scheduler/__init__.py
--rw-r--r--   0 pd         (501) staff       (20)     1154 2023-06-25 17:47:45.000000 granny-pliers-0.0.15/src/granny_pliers/scheduler/abstract_schedule_object.py
--rw-r--r--   0 pd         (501) staff       (20)     7068 2023-06-25 17:47:10.000000 granny-pliers-0.0.15/src/granny_pliers/scheduler/abstract_scheduler.py
--rw-r--r--   0 pd         (501) staff       (20)     4916 2023-06-25 17:44:42.000000 granny-pliers-0.0.15/src/granny_pliers/scheduler/time_table.py
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-07-01 23:28:01.591627 granny-pliers-0.0.15/src/granny_pliers/testing/
--rw-r--r--   0 pd         (501) staff       (20)      806 2023-06-04 16:29:44.000000 granny-pliers-0.0.15/src/granny_pliers/testing/__init__.py
--rw-r--r--   0 pd         (501) staff       (20)     1998 2023-06-10 12:35:19.000000 granny-pliers-0.0.15/src/granny_pliers/testing/abstract_test_case.py
--rw-r--r--   0 pd         (501) staff       (20)      914 2023-06-10 12:35:55.000000 granny-pliers-0.0.15/src/granny_pliers/testing/async_abstract_test_case.py
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-07-01 23:28:01.592264 granny-pliers-0.0.15/src/granny_pliers/tools/
--rw-r--r--   0 pd         (501) staff       (20)      711 2023-06-10 13:15:39.000000 granny-pliers-0.0.15/src/granny_pliers/tools/__init__.py
--rw-r--r--   0 pd         (501) staff       (20)     2271 2023-06-10 17:09:40.000000 granny-pliers-0.0.15/src/granny_pliers/tools/datetime_helper.py
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-07-01 23:28:01.594377 granny-pliers-0.0.15/src/granny_pliers/web/
--rw-r--r--   0 pd         (501) staff       (20)     1041 2023-06-10 13:18:21.000000 granny-pliers-0.0.15/src/granny_pliers/web/__init__.py
--rw-r--r--   0 pd         (501) staff       (20)     2135 2023-06-10 17:09:00.000000 granny-pliers-0.0.15/src/granny_pliers/web/abstract_status_web_service.py
--rw-r--r--   0 pd         (501) staff       (20)     4235 2023-06-10 13:21:16.000000 granny-pliers-0.0.15/src/granny_pliers/web/abstract_web_application.py
--rw-r--r--   0 pd         (501) staff       (20)    11869 2023-06-10 13:32:23.000000 granny-pliers-0.0.15/src/granny_pliers/web/abstract_web_service.py
--rw-r--r--   0 pd         (501) staff       (20)     1575 2023-06-15 19:06:25.000000 granny-pliers-0.0.15/src/granny_pliers/web/web_application_config.py
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-07-01 23:28:01.595160 granny-pliers-0.0.15/src/granny_pliers/worker/
--rw-r--r--   0 pd         (501) staff       (20)      713 2023-06-04 16:29:44.000000 granny-pliers-0.0.15/src/granny_pliers/worker/__init__.py
--rw-r--r--   0 pd         (501) staff       (20)     5086 2023-06-04 16:29:44.000000 granny-pliers-0.0.15/src/granny_pliers/worker/abstract_worker.py
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-07-01 23:28:01.575087 granny-pliers-0.0.15/src/granny_pliers.egg-info/
--rw-r--r--   0 pd         (501) staff       (20)    13701 2023-07-01 23:28:01.000000 granny-pliers-0.0.15/src/granny_pliers.egg-info/PKG-INFO
--rw-r--r--   0 pd         (501) staff       (20)     2275 2023-07-01 23:28:01.000000 granny-pliers-0.0.15/src/granny_pliers.egg-info/SOURCES.txt
--rw-r--r--   0 pd         (501) staff       (20)        1 2023-07-01 23:28:01.000000 granny-pliers-0.0.15/src/granny_pliers.egg-info/dependency_links.txt
--rw-r--r--   0 pd         (501) staff       (20)      230 2023-07-01 23:28:01.000000 granny-pliers-0.0.15/src/granny_pliers.egg-info/requires.txt
--rw-r--r--   0 pd         (501) staff       (20)       14 2023-07-01 23:28:01.000000 granny-pliers-0.0.15/src/granny_pliers.egg-info/top_level.txt
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-06-14 21:02:38.471133 granny-pliers-0.0.9/
+-rw-r--r--   0 pd         (501) staff       (20)    11357 2023-06-03 18:43:25.000000 granny-pliers-0.0.9/LICENSE
+-rw-r--r--   0 pd         (501) staff       (20)    13700 2023-06-14 21:02:38.470754 granny-pliers-0.0.9/PKG-INFO
+-rw-r--r--   0 pd         (501) staff       (20)       16 2023-06-10 17:39:54.000000 granny-pliers-0.0.9/README.md
+-rw-r--r--   0 pd         (501) staff       (20)     1619 2023-06-14 20:50:52.000000 granny-pliers-0.0.9/pyproject.toml
+-rw-r--r--   0 pd         (501) staff       (20)       38 2023-06-14 21:02:38.471227 granny-pliers-0.0.9/setup.cfg
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-06-14 21:02:38.437214 granny-pliers-0.0.9/src/
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-06-14 21:02:38.440162 granny-pliers-0.0.9/src/granny_pliers/
+-rw-r--r--   0 pd         (501) staff       (20)      987 2023-06-14 20:51:00.000000 granny-pliers-0.0.9/src/granny_pliers/__init__.py
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-06-14 21:02:38.448122 granny-pliers-0.0.9/src/granny_pliers/auth/
+-rw-r--r--   0 pd         (501) staff       (20)     1228 2023-06-10 13:12:31.000000 granny-pliers-0.0.9/src/granny_pliers/auth/__init__.py
+-rw-r--r--   0 pd         (501) staff       (20)     1683 2023-06-10 11:50:56.000000 granny-pliers-0.0.9/src/granny_pliers/auth/auth_config.py
+-rw-r--r--   0 pd         (501) staff       (20)      986 2023-06-10 13:13:15.000000 granny-pliers-0.0.9/src/granny_pliers/auth/auth_error.py
+-rw-r--r--   0 pd         (501) staff       (20)     1308 2023-06-10 13:13:08.000000 granny-pliers-0.0.9/src/granny_pliers/auth/auth_request.py
+-rw-r--r--   0 pd         (501) staff       (20)     1016 2023-06-10 13:11:55.000000 granny-pliers-0.0.9/src/granny_pliers/auth/auth_response.py
+-rw-r--r--   0 pd         (501) staff       (20)     6158 2023-06-10 13:18:46.000000 granny-pliers-0.0.9/src/granny_pliers/auth/jwt.py
+-rw-r--r--   0 pd         (501) staff       (20)      882 2023-06-10 11:26:21.000000 granny-pliers-0.0.9/src/granny_pliers/auth/permissions.py
+-rw-r--r--   0 pd         (501) staff       (20)      828 2023-06-10 11:26:59.000000 granny-pliers-0.0.9/src/granny_pliers/auth/roles.py
+-rw-r--r--   0 pd         (501) staff       (20)     9678 2023-06-10 13:14:07.000000 granny-pliers-0.0.9/src/granny_pliers/auth/rsa_codec.py
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-06-14 21:02:38.450537 granny-pliers-0.0.9/src/granny_pliers/config/
+-rw-r--r--   0 pd         (501) staff       (20)      985 2023-06-04 16:29:44.000000 granny-pliers-0.0.9/src/granny_pliers/config/__init__.py
+-rw-r--r--   0 pd         (501) staff       (20)     3198 2023-06-09 21:43:11.000000 granny-pliers-0.0.9/src/granny_pliers/config/abstract_config.py
+-rw-r--r--   0 pd         (501) staff       (20)     1614 2023-06-03 23:39:30.000000 granny-pliers-0.0.9/src/granny_pliers/config/autowired_config.py
+-rw-r--r--   0 pd         (501) staff       (20)     6694 2023-06-14 20:55:52.000000 granny-pliers-0.0.9/src/granny_pliers/config/logger_config.py
+-rw-r--r--   0 pd         (501) staff       (20)      860 2023-06-03 18:43:25.000000 granny-pliers-0.0.9/src/granny_pliers/config/project_environment.py
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-06-14 21:02:38.452701 granny-pliers-0.0.9/src/granny_pliers/logger/
+-rw-r--r--   0 pd         (501) staff       (20)      884 2023-06-04 16:29:44.000000 granny-pliers-0.0.9/src/granny_pliers/logger/__init__.py
+-rw-r--r--   0 pd         (501) staff       (20)     1292 2023-06-03 18:43:25.000000 granny-pliers-0.0.9/src/granny_pliers/logger/abstract_logger.py
+-rw-r--r--   0 pd         (501) staff       (20)     1253 2023-06-03 18:43:25.000000 granny-pliers-0.0.9/src/granny_pliers/logger/log_processors.py
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-06-14 21:02:38.453438 granny-pliers-0.0.9/src/granny_pliers/models/
+-rw-r--r--   0 pd         (501) staff       (20)      620 2023-06-10 11:58:05.000000 granny-pliers-0.0.9/src/granny_pliers/models/__init__.py
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-06-14 21:02:38.454935 granny-pliers-0.0.9/src/granny_pliers/models/auth/
+-rw-r--r--   0 pd         (501) staff       (20)      688 2023-06-10 13:33:22.000000 granny-pliers-0.0.9/src/granny_pliers/models/auth/__init__.py
+-rw-r--r--   0 pd         (501) staff       (20)     2061 2023-06-10 13:36:39.000000 granny-pliers-0.0.9/src/granny_pliers/models/auth/user.py
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-06-14 21:02:38.456903 granny-pliers-0.0.9/src/granny_pliers/models/metrics/
+-rw-r--r--   0 pd         (501) staff       (20)      715 2023-06-10 13:32:44.000000 granny-pliers-0.0.9/src/granny_pliers/models/metrics/__init__.py
+-rw-r--r--   0 pd         (501) staff       (20)     2766 2023-06-10 13:33:13.000000 granny-pliers-0.0.9/src/granny_pliers/models/metrics/confusion_matrix.py
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-06-14 21:02:38.458526 granny-pliers-0.0.9/src/granny_pliers/models/web/
+-rw-r--r--   0 pd         (501) staff       (20)      729 2023-06-10 13:36:51.000000 granny-pliers-0.0.9/src/granny_pliers/models/web/__init__.py
+-rw-r--r--   0 pd         (501) staff       (20)     1645 2023-06-10 11:59:08.000000 granny-pliers-0.0.9/src/granny_pliers/models/web/web_service_health_status.py
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-06-14 21:02:38.462837 granny-pliers-0.0.9/src/granny_pliers/orm/
+-rw-r--r--   0 pd         (501) staff       (20)     1222 2023-06-10 13:29:12.000000 granny-pliers-0.0.9/src/granny_pliers/orm/__init__.py
+-rw-r--r--   0 pd         (501) staff       (20)     5494 2023-06-10 13:26:46.000000 granny-pliers-0.0.9/src/granny_pliers/orm/abstract_http_client.py
+-rw-r--r--   0 pd         (501) staff       (20)     5956 2023-06-10 13:25:56.000000 granny-pliers-0.0.9/src/granny_pliers/orm/abstract_http_repository.py
+-rw-r--r--   0 pd         (501) staff       (20)     2990 2023-06-10 13:38:35.000000 granny-pliers-0.0.9/src/granny_pliers/orm/abstract_model.py
+-rw-r--r--   0 pd         (501) staff       (20)    19833 2023-06-10 13:36:11.000000 granny-pliers-0.0.9/src/granny_pliers/orm/abstract_mongo_repository.py
+-rw-r--r--   0 pd         (501) staff       (20)     7523 2023-06-09 21:46:56.000000 granny-pliers-0.0.9/src/granny_pliers/orm/abstract_repository.py
+-rw-r--r--   0 pd         (501) staff       (20)    14519 2023-06-10 17:09:48.000000 granny-pliers-0.0.9/src/granny_pliers/orm/restful_http_client.py
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-06-14 21:02:38.464681 granny-pliers-0.0.9/src/granny_pliers/testing/
+-rw-r--r--   0 pd         (501) staff       (20)      806 2023-06-04 16:29:44.000000 granny-pliers-0.0.9/src/granny_pliers/testing/__init__.py
+-rw-r--r--   0 pd         (501) staff       (20)     1998 2023-06-10 12:35:19.000000 granny-pliers-0.0.9/src/granny_pliers/testing/abstract_test_case.py
+-rw-r--r--   0 pd         (501) staff       (20)      914 2023-06-10 12:35:55.000000 granny-pliers-0.0.9/src/granny_pliers/testing/async_abstract_test_case.py
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-06-14 21:02:38.466108 granny-pliers-0.0.9/src/granny_pliers/tools/
+-rw-r--r--   0 pd         (501) staff       (20)      711 2023-06-10 13:15:39.000000 granny-pliers-0.0.9/src/granny_pliers/tools/__init__.py
+-rw-r--r--   0 pd         (501) staff       (20)     2271 2023-06-10 17:09:40.000000 granny-pliers-0.0.9/src/granny_pliers/tools/datetime_helper.py
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-06-14 21:02:38.468181 granny-pliers-0.0.9/src/granny_pliers/web/
+-rw-r--r--   0 pd         (501) staff       (20)     1041 2023-06-10 13:18:21.000000 granny-pliers-0.0.9/src/granny_pliers/web/__init__.py
+-rw-r--r--   0 pd         (501) staff       (20)     2135 2023-06-10 17:09:00.000000 granny-pliers-0.0.9/src/granny_pliers/web/abstract_status_web_service.py
+-rw-r--r--   0 pd         (501) staff       (20)     4235 2023-06-10 13:21:16.000000 granny-pliers-0.0.9/src/granny_pliers/web/abstract_web_application.py
+-rw-r--r--   0 pd         (501) staff       (20)    11869 2023-06-10 13:32:23.000000 granny-pliers-0.0.9/src/granny_pliers/web/abstract_web_service.py
+-rw-r--r--   0 pd         (501) staff       (20)     1499 2023-06-10 12:04:19.000000 granny-pliers-0.0.9/src/granny_pliers/web/web_application_config.py
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-06-14 21:02:38.469771 granny-pliers-0.0.9/src/granny_pliers/worker/
+-rw-r--r--   0 pd         (501) staff       (20)      713 2023-06-04 16:29:44.000000 granny-pliers-0.0.9/src/granny_pliers/worker/__init__.py
+-rw-r--r--   0 pd         (501) staff       (20)     5086 2023-06-04 16:29:44.000000 granny-pliers-0.0.9/src/granny_pliers/worker/abstract_worker.py
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-06-14 21:02:38.441760 granny-pliers-0.0.9/src/granny_pliers.egg-info/
+-rw-r--r--   0 pd         (501) staff       (20)    13700 2023-06-14 21:02:38.000000 granny-pliers-0.0.9/src/granny_pliers.egg-info/PKG-INFO
+-rw-r--r--   0 pd         (501) staff       (20)     2087 2023-06-14 21:02:38.000000 granny-pliers-0.0.9/src/granny_pliers.egg-info/SOURCES.txt
+-rw-r--r--   0 pd         (501) staff       (20)        1 2023-06-14 21:02:38.000000 granny-pliers-0.0.9/src/granny_pliers.egg-info/dependency_links.txt
+-rw-r--r--   0 pd         (501) staff       (20)      230 2023-06-14 21:02:38.000000 granny-pliers-0.0.9/src/granny_pliers.egg-info/requires.txt
+-rw-r--r--   0 pd         (501) staff       (20)       14 2023-06-14 21:02:38.000000 granny-pliers-0.0.9/src/granny_pliers.egg-info/top_level.txt
```

### Comparing `granny-pliers-0.0.15/LICENSE` & `granny-pliers-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `granny-pliers-0.0.15/PKG-INFO` & `granny-pliers-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: granny-pliers
-Version: 0.0.15
+Version: 0.0.9
 Summary: Set of tools
 Author-email: Dmytro Stepanenko <dmitrijstepanenko@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `granny-pliers-0.0.15/pyproject.toml` & `granny-pliers-0.0.9/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "granny-pliers"
-version = "0.0.15"
+version = "0.0.9"
 
 authors = [
     { name = "Dmytro Stepanenko", email = "dmitrijstepanenko@gmail.com" },
 ]
 
 license = { file = "LICENSE" }
 
@@ -37,24 +37,24 @@
     "colorama>=0.4.6",
     "jsonplus>=0.8.0",
     "cryptography>=41.0.1",
     "aiohttp>=3.8.4",
     "aiofiles>=23.1.0",
     "dateparser>=1.1.8",
     "PyYAML>=6.0",
-    "motor==3.2.0",
+    "motor==3.1.2",
 ]
 
 [project.optional-dependencies]
 # Dev dependencies.
 dev = [
     "black>=22.3.0",
     "pylint>=2.17.4",
     "coverage>=7.2.7",
-    "pytest>=7.4.0",
+    "pytest>=7.3.1",
     "pytest-cov==4.1.0"
 ]
 
 [project.urls]
 "Homepage" = "https://gitlab.com/stepanenko-family/shared/granny-pliers.git"
 
 [tool.black]
```

### Comparing `granny-pliers-0.0.15/src/granny_pliers/__init__.py` & `granny-pliers-0.0.9/src/granny_pliers/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,13 +11,13 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 """Granny Pliers is a Python library that contains a collection of useful
 and helpful tools, designed to simplify developers' lives."""
 
-__version__ = "0.0.15"
+__version__ = "0.0.9"
 __author__ = "Dmytro Stepanenko"
 __copyright__ = "Copyright 2022, Dmytro Stepanenko, Granny Pliers"
 __credits__ = ["Dmytro Stepanenko"]
 __license__ = "Apache License Version 2.0"
 __email__ = "dmitrijstepanenko@gmail.com"
```

### Comparing `granny-pliers-0.0.15/src/granny_pliers/auth/__init__.py` & `granny-pliers-0.0.9/src/granny_pliers/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `granny-pliers-0.0.15/src/granny_pliers/auth/auth_config.py` & `granny-pliers-0.0.9/src/granny_pliers/auth/auth_config.py`

 * *Files identical despite different names*

### Comparing `granny-pliers-0.0.15/src/granny_pliers/auth/auth_error.py` & `granny-pliers-0.0.9/src/granny_pliers/auth/auth_error.py`

 * *Files identical despite different names*

### Comparing `granny-pliers-0.0.15/src/granny_pliers/auth/auth_request.py` & `granny-pliers-0.0.9/src/granny_pliers/auth/auth_request.py`

 * *Files identical despite different names*

### Comparing `granny-pliers-0.0.15/src/granny_pliers/auth/auth_response.py` & `granny-pliers-0.0.9/src/granny_pliers/auth/auth_response.py`

 * *Files identical despite different names*

### Comparing `granny-pliers-0.0.15/src/granny_pliers/auth/jwt.py` & `granny-pliers-0.0.9/src/granny_pliers/auth/jwt.py`

 * *Files identical despite different names*

### Comparing `granny-pliers-0.0.15/src/granny_pliers/auth/permissions.py` & `granny-pliers-0.0.9/src/granny_pliers/auth/permissions.py`

 * *Files identical despite different names*

### Comparing `granny-pliers-0.0.15/src/granny_pliers/auth/roles.py` & `granny-pliers-0.0.9/src/granny_pliers/auth/roles.py`

 * *Files identical despite different names*

### Comparing `granny-pliers-0.0.15/src/granny_pliers/auth/rsa_codec.py` & `granny-pliers-0.0.9/src/granny_pliers/auth/rsa_codec.py`

 * *Files identical despite different names*

### Comparing `granny-pliers-0.0.15/src/granny_pliers/config/__init__.py` & `granny-pliers-0.0.9/src/granny_pliers/config/__init__.py`

 * *Files identical despite different names*

### Comparing `granny-pliers-0.0.15/src/granny_pliers/config/abstract_config.py` & `granny-pliers-0.0.9/src/granny_pliers/config/abstract_config.py`

 * *Files identical despite different names*

### Comparing `granny-pliers-0.0.15/src/granny_pliers/config/autowired_config.py` & `granny-pliers-0.0.9/src/granny_pliers/config/autowired_config.py`

 * *Files identical despite different names*

### Comparing `granny-pliers-0.0.15/src/granny_pliers/config/logger_config.py` & `granny-pliers-0.0.9/src/granny_pliers/config/logger_config.py`

 * *Files identical despite different names*

### Comparing `granny-pliers-0.0.15/src/granny_pliers/config/project_environment.py` & `granny-pliers-0.0.9/src/granny_pliers/config/project_environment.py`

 * *Files identical despite different names*

### Comparing `granny-pliers-0.0.15/src/granny_pliers/logger/__init__.py` & `granny-pliers-0.0.9/src/granny_pliers/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `granny-pliers-0.0.15/src/granny_pliers/logger/abstract_logger.py` & `granny-pliers-0.0.9/src/granny_pliers/logger/abstract_logger.py`

 * *Files identical despite different names*

### Comparing `granny-pliers-0.0.15/src/granny_pliers/logger/log_processors.py` & `granny-pliers-0.0.9/src/granny_pliers/logger/log_processors.py`

 * *Files identical despite different names*

### Comparing `granny-pliers-0.0.15/src/granny_pliers/models/__init__.py` & `granny-pliers-0.0.9/src/granny_pliers/models/__init__.py`

 * *Files identical despite different names*

### Comparing `granny-pliers-0.0.15/src/granny_pliers/models/auth/__init__.py` & `granny-pliers-0.0.9/src/granny_pliers/models/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `granny-pliers-0.0.15/src/granny_pliers/models/auth/user.py` & `granny-pliers-0.0.9/src/granny_pliers/models/auth/user.py`

 * *Files identical despite different names*

### Comparing `granny-pliers-0.0.15/src/granny_pliers/models/metrics/__init__.py` & `granny-pliers-0.0.9/src/granny_pliers/models/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `granny-pliers-0.0.15/src/granny_pliers/models/metrics/confusion_matrix.py` & `granny-pliers-0.0.9/src/granny_pliers/models/metrics/confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `granny-pliers-0.0.15/src/granny_pliers/models/web/__init__.py` & `granny-pliers-0.0.9/src/granny_pliers/models/web/__init__.py`

 * *Files identical despite different names*

### Comparing `granny-pliers-0.0.15/src/granny_pliers/models/web/web_service_health_status.py` & `granny-pliers-0.0.9/src/granny_pliers/models/web/web_service_health_status.py`

 * *Files identical despite different names*

### Comparing `granny-pliers-0.0.15/src/granny_pliers/orm/__init__.py` & `granny-pliers-0.0.9/src/granny_pliers/orm/__init__.py`

 * *Files identical despite different names*

### Comparing `granny-pliers-0.0.15/src/granny_pliers/orm/abstract_http_client.py` & `granny-pliers-0.0.9/src/granny_pliers/orm/abstract_http_client.py`

 * *Files identical despite different names*

### Comparing `granny-pliers-0.0.15/src/granny_pliers/orm/abstract_http_repository.py` & `granny-pliers-0.0.9/src/granny_pliers/orm/abstract_http_repository.py`

 * *Files identical despite different names*

### Comparing `granny-pliers-0.0.15/src/granny_pliers/orm/abstract_model.py` & `granny-pliers-0.0.9/src/granny_pliers/orm/abstract_model.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 """BaseModel"""
 
 from dataclasses import dataclass, fields, field
 from datetime import datetime
-from enum import Enum
 from typing import TypeVar, Generic
 
 import jsonplus
 
 __all__ = ["BaseModel", "base_model_encoder", "AbstractModel", "ModelsPage", "ModelsCount"]
 
 from bson import ObjectId
@@ -51,15 +50,15 @@
 
     @id.setter
     def id(self, value: None | str | ObjectId):  # pylint: disable=C0103
         """id"""
         match value:
             case ObjectId():
                 self._id = value
-            case None | "None":
+            case None:
                 self._id = ObjectId()
             case str():
                 self._id = ObjectId() if value == "" else ObjectId(value)
 
     @property
     def created_at(self) -> datetime:
         """ObjectID"""
@@ -105,19 +104,13 @@
 
     :param obj:
     :return: dict
     """
     obj_dict = {}
     for cls_field in fields(obj):
         if cls_field.type is ObjectId:
-            value = str(getattr(obj, cls_field.name))
-            if value is None:
-                obj_dict[cls_field.name] = None
-            else:
-                obj_dict[cls_field.name] = str(getattr(obj, cls_field.name))
+            obj_dict[cls_field.name] = str(getattr(obj, cls_field.name))
         elif cls_field.type is tuple:
             obj_dict[cls_field.name] = str(getattr(obj, cls_field.name))
-        elif issubclass(cls_field.type, Enum):
-            obj_dict[cls_field.name] = getattr(obj, cls_field.name).value
         else:
             obj_dict[cls_field.name] = getattr(obj, cls_field.name)
     return obj_dict
```

### Comparing `granny-pliers-0.0.15/src/granny_pliers/orm/abstract_mongo_repository.py` & `granny-pliers-0.0.9/src/granny_pliers/orm/abstract_mongo_repository.py`

 * *Files 2% similar despite different names*

```diff
@@ -138,15 +138,15 @@
         if self.__client is not None:
             self.__client.close()
             self.__client = None
 
     def _fallback_encoder(self, value):
         try:
             if isinstance(value, Enum):
-                return value.value
+                return asdict(value.value)
             else:
                 # Python datetime to BSON DateTime encoder
                 return setup_datetime(value)
         except TypeError as error:
             self.log.error("_fallback_encoder", error=error)
 
     @staticmethod
@@ -179,22 +179,22 @@
         try:
             insert_result: InsertOneResult = await self.collection.insert_one(document=asdict(obj))
 
             if insert_result.acknowledged is None:
                 self.log.error("Can not save %s", self.model_class_name)
                 return None
 
-            result = await self.collection.find_one(filter=insert_result.inserted_id)
+            resource = await self.collection.find_one(filter=insert_result.inserted_id)
 
-            if result is None:
+            if resource is None:
                 self.log.error("Saved %s not found", self.model_class_name)
                 return None
             if verbose:
-                self.log.info("Saved %s: %s", self.model_class_name, result.get("_id", None))
-            return self.model_class(**self.filter_model_class_fields(result))
+                self.log.info("Saved %s: %s", self.model_class_name, resource.get("_id"))
+            return self.model_class(**resource)
 
         except (DuplicateKeyError, OperationFailure, TypeError) as error:
             self.log.error("Can not save %s", self.model_class_name, error=error)
             return None
 
     async def save_if_not_exists(self, obj: ModelT, conditions: dict = None) -> Optional[ModelT]:
         """save_if_not_exists"""
@@ -238,15 +238,15 @@
                 return_document=ReturnDocument.AFTER,
             )
 
             if result is None:
                 self.log.error("Can not update %s: %s", self.model_class_name, obj.id)
                 return None
             self.log.info("Updated %s: %s", self.model_class_name, obj.id)
-            return self.model_class(**self.filter_model_class_fields(result))
+            return self.model_class(**result)
         except (OperationFailure, TypeError) as error:
             self.log.error("Can not update %s: %s", self.model_class_name, obj.id, error=error)
             return None
 
     async def update_many(self, objects: list[ModelT]) -> int:
         if len(objects) == 0:
             self.log.info("Updated 0 %ss", self.model_class_name)
@@ -293,15 +293,15 @@
                 return_document=ReturnDocument.AFTER,
             )
 
             if result is None:
                 self.log.error("Can not patch %s: %s", self.model_class_name, obj_id)
                 return None
             self.log.info("Patched %s: %s", self.model_class_name, obj_id)
-            return self.model_class(**self.filter_model_class_fields(result))
+            return self.model_class(**result)
         except (OperationFailure, TypeError) as error:
             self.log.error("Can not patch %s", self.model_class_name, obj_id=obj_id, error=error)
             return None
 
     async def patch_many_by_id(self, obj_ids: list[Any], resources: dict) -> int:
         if len(obj_ids) == 0:
             self.log.info("Patched 0 %ss", self.model_class_name)
@@ -365,19 +365,15 @@
                 result = await self.collection.find_one_and_delete(dict(_id=mongo_obj_id))
                 self.log.info("Hard deleted %s: %s", self.model_class_name, mongo_obj_id)
 
             if result is None:
                 self.log.error("Can not delete %s", self.model_class_name, obj_id=mongo_obj_id)
                 return None
 
-            return (
-                result
-                if isinstance(result, self._model_class)
-                else self.model_class(**self.filter_model_class_fields(result))
-            )
+            return result if isinstance(result, self._model_class) else self.model_class(**result)
         except (OperationFailure, TypeError) as error:
             self.log.error("Can not delete %s", self.model_class_name, obj_id=obj_id, error=error)
             return None
 
     async def delete_all(self, soft: bool = True) -> int:
         try:
             if soft:
@@ -412,15 +408,15 @@
 
             if result is None:
                 return None
 
             if verbose:
                 self.log.info("Found %s: %s", self.model_class_name, result.get("_id"))
 
-            return self.model_class(**self.filter_model_class_fields(result))
+            return self.model_class(**result)
         except (OperationFailure, TypeError) as error:
             self.log.error(
                 "Can not execute find for %s",
                 self.model_class_name,
                 conditions=conditions,
                 error=error,
             )
@@ -432,15 +428,15 @@
 
             result = await self.collection.find_one(filter=mongo_obj_id)
             if result is None:
                 self.log.info("Not found %s: %s", self.model_class_name, mongo_obj_id)
                 return None
 
             self.log.info("Found %s: %s", self.model_class_name, result.get("_id"))
-            return self.model_class(**self.filter_model_class_fields(result))
+            return self.model_class(**result)
         except (OperationFailure, TypeError) as error:
             self.log.error(
                 "Can not execute find_by_id %s",
                 self.model_class_name,
                 obj_id=obj_id,
                 error=error,
             )
@@ -451,15 +447,15 @@
             result = await self.collection.find_one(filter=conditions, limit=1, sort=[("_id", -1)])
 
             if result is None:
                 self.log.info("Last not found %s, collection is empty", self.model_class_name)
                 return None
 
             self.log.info("Found %s: %s", self.model_class_name, result.get("_id"))
-            return self.model_class(**self.filter_model_class_fields(result))
+            return self.model_class(**result)
         except (OperationFailure, TypeError) as error:
             self.log.error("Can not find %s", self.model_class_name, error=error)
             return None
 
     async def count(self, conditions: dict = None) -> int:
         """
         Calculate number of objects
@@ -493,15 +489,15 @@
         limit = page_size
         try:
             cursor = self.collection.find(filter=conditions, skip=skip, limit=limit, sort=sort, projection=projection)
 
             result = await cursor.to_list(None)
             if verbose:
                 self.log.info("Found %d %ss", len(result), self.model_class_name)
-            return list(map(lambda t: self.model_class(**self.filter_model_class_fields(t)), result))
+            return list(map(lambda t: self.model_class(**t), result))
         except (OperationFailure, TypeError, Exception) as error:
             self.log.error("Can not find %s", self.model_class_name, error=error)
             return []
 
     @staticmethod
     def helper_symbol_date_condition(symbol: str, date: datetime) -> dict:
         """helper_symbol_date_condition"""
```

### Comparing `granny-pliers-0.0.15/src/granny_pliers/orm/abstract_repository.py` & `granny-pliers-0.0.9/src/granny_pliers/orm/abstract_repository.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 """Abstract Repository"""
 
 import abc
-from dataclasses import fields
 from types import TracebackType
 from typing import TypeVar, Generic, Optional, Any, Type
 
 from granny_pliers.logger import AbstractLogger
 
 __all__ = ["AbstractRepository"]
 ModelT = TypeVar("ModelT")
@@ -27,18 +26,14 @@
 
 class AbstractRepository(Generic[ModelT], AbstractLogger):
     """AbstractRepository"""
 
     def __init__(self, model_class: Type[ModelT]):
         super().__init__()
         self._model_class = model_class
-        self.model_class_fields_names = [f.name for f in fields(model_class)]
-
-    def filter_model_class_fields(self, resource: dict) -> dict:
-        return {k: v for k, v in resource.items() if k in self.model_class_fields_names}
 
     async def __aenter__(self):
         """__aenter__"""
         return self
 
     async def __aexit__(
         self,
```

### Comparing `granny-pliers-0.0.15/src/granny_pliers/orm/restful_http_client.py` & `granny-pliers-0.0.9/src/granny_pliers/orm/restful_http_client.py`

 * *Files identical despite different names*

### Comparing `granny-pliers-0.0.15/src/granny_pliers/testing/__init__.py` & `granny-pliers-0.0.9/src/granny_pliers/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `granny-pliers-0.0.15/src/granny_pliers/testing/abstract_test_case.py` & `granny-pliers-0.0.9/src/granny_pliers/testing/abstract_test_case.py`

 * *Files identical despite different names*

### Comparing `granny-pliers-0.0.15/src/granny_pliers/testing/async_abstract_test_case.py` & `granny-pliers-0.0.9/src/granny_pliers/testing/async_abstract_test_case.py`

 * *Files identical despite different names*

### Comparing `granny-pliers-0.0.15/src/granny_pliers/tools/__init__.py` & `granny-pliers-0.0.9/src/granny_pliers/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `granny-pliers-0.0.15/src/granny_pliers/tools/datetime_helper.py` & `granny-pliers-0.0.9/src/granny_pliers/tools/datetime_helper.py`

 * *Files identical despite different names*

### Comparing `granny-pliers-0.0.15/src/granny_pliers/web/__init__.py` & `granny-pliers-0.0.9/src/granny_pliers/web/__init__.py`

 * *Files identical despite different names*

### Comparing `granny-pliers-0.0.15/src/granny_pliers/web/abstract_status_web_service.py` & `granny-pliers-0.0.9/src/granny_pliers/web/abstract_status_web_service.py`

 * *Files identical despite different names*

### Comparing `granny-pliers-0.0.15/src/granny_pliers/web/abstract_web_application.py` & `granny-pliers-0.0.9/src/granny_pliers/web/abstract_web_application.py`

 * *Files identical despite different names*

### Comparing `granny-pliers-0.0.15/src/granny_pliers/web/abstract_web_service.py` & `granny-pliers-0.0.9/src/granny_pliers/web/abstract_web_service.py`

 * *Files identical despite different names*

### Comparing `granny-pliers-0.0.15/src/granny_pliers/web/web_application_config.py` & `granny-pliers-0.0.9/src/granny_pliers/web/web_application_config.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,18 +22,15 @@
 __all__ = ["WebApplicationConfig"]
 
 
 @dataclass()
 class WebApplicationConfig(AbstractConfig):
     """WebApplicationConfig"""
 
-    auth: AuthConfig = field(
-        default="localhost",
-        metadata={"type": AuthConfig},
-    )
+    auth: AuthConfig = None
 
     host: str = field(
         default="localhost",
         metadata={"env_var_name": "WEB_HOST", "type": str},
     )
     port: int = field(
         default=8080,
```

### Comparing `granny-pliers-0.0.15/src/granny_pliers/worker/__init__.py` & `granny-pliers-0.0.9/src/granny_pliers/worker/__init__.py`

 * *Files identical despite different names*

### Comparing `granny-pliers-0.0.15/src/granny_pliers/worker/abstract_worker.py` & `granny-pliers-0.0.9/src/granny_pliers/worker/abstract_worker.py`

 * *Files identical despite different names*

### Comparing `granny-pliers-0.0.15/src/granny_pliers.egg-info/PKG-INFO` & `granny-pliers-0.0.9/src/granny_pliers.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: granny-pliers
-Version: 0.0.15
+Version: 0.0.9
 Summary: Set of tools
 Author-email: Dmytro Stepanenko <dmitrijstepanenko@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `granny-pliers-0.0.15/src/granny_pliers.egg-info/SOURCES.txt` & `granny-pliers-0.0.9/src/granny_pliers.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -34,18 +34,14 @@
 src/granny_pliers/orm/__init__.py
 src/granny_pliers/orm/abstract_http_client.py
 src/granny_pliers/orm/abstract_http_repository.py
 src/granny_pliers/orm/abstract_model.py
 src/granny_pliers/orm/abstract_mongo_repository.py
 src/granny_pliers/orm/abstract_repository.py
 src/granny_pliers/orm/restful_http_client.py
-src/granny_pliers/scheduler/__init__.py
-src/granny_pliers/scheduler/abstract_schedule_object.py
-src/granny_pliers/scheduler/abstract_scheduler.py
-src/granny_pliers/scheduler/time_table.py
 src/granny_pliers/testing/__init__.py
 src/granny_pliers/testing/abstract_test_case.py
 src/granny_pliers/testing/async_abstract_test_case.py
 src/granny_pliers/tools/__init__.py
 src/granny_pliers/tools/datetime_helper.py
 src/granny_pliers/web/__init__.py
 src/granny_pliers/web/abstract_status_web_service.py
```

