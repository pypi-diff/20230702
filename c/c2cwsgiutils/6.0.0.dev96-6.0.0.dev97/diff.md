# Comparing `tmp/c2cwsgiutils-6.0.0.dev96.tar.gz` & `tmp/c2cwsgiutils-6.0.0.dev97.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "c2cwsgiutils-6.0.0.dev96.tar", max compression
+gzip compressed data, was "c2cwsgiutils-6.0.0.dev97.tar", max compression
```

## Comparing `c2cwsgiutils-6.0.0.dev96.tar` & `c2cwsgiutils-6.0.0.dev97.tar`

### file list

```diff
@@ -1,61 +1,61 @@
--rw-r--r--   0        0        0     1304 2023-07-01 19:56:35.103718 c2cwsgiutils-6.0.0.dev96/LICENSE
--rw-r--r--   0        0        0    29129 2023-07-01 19:56:35.103718 c2cwsgiutils-6.0.0.dev96/README.md
--rw-r--r--   0        0        0     3997 2023-07-01 19:56:35.103718 c2cwsgiutils-6.0.0.dev96/c2cwsgiutils/__init__.py
--rw-r--r--   0        0        0     1500 2023-07-01 19:56:35.103718 c2cwsgiutils-6.0.0.dev96/c2cwsgiutils/acceptance/__init__.py
--rw-r--r--   0        0        0     5331 2023-07-01 19:56:35.103718 c2cwsgiutils-6.0.0.dev96/c2cwsgiutils/acceptance/composition.py
--rw-r--r--   0        0        0     9109 2023-07-01 19:56:35.103718 c2cwsgiutils-6.0.0.dev96/c2cwsgiutils/acceptance/connection.py
--rw-r--r--   0        0        0     4701 2023-07-01 19:56:35.103718 c2cwsgiutils-6.0.0.dev96/c2cwsgiutils/acceptance/image.py
--rw-r--r--   0        0        0     2329 2023-07-01 19:56:35.103718 c2cwsgiutils-6.0.0.dev96/c2cwsgiutils/acceptance/print.py
--rw-r--r--   0        0        0     2078 2023-07-01 19:56:35.103718 c2cwsgiutils-6.0.0.dev96/c2cwsgiutils/acceptance/utils.py
--rw-r--r--   0        0        0     9313 2023-07-01 19:56:35.103718 c2cwsgiutils-6.0.0.dev96/c2cwsgiutils/auth.py
--rw-r--r--   0        0        0     4372 2023-07-01 19:56:35.107718 c2cwsgiutils-6.0.0.dev96/c2cwsgiutils/broadcast/__init__.py
--rw-r--r--   0        0        0      615 2023-07-01 19:56:35.107718 c2cwsgiutils-6.0.0.dev96/c2cwsgiutils/broadcast/interface.py
--rw-r--r--   0        0        0     1062 2023-07-01 19:56:35.107718 c2cwsgiutils-6.0.0.dev96/c2cwsgiutils/broadcast/local.py
--rw-r--r--   0        0        0     5064 2023-07-01 19:56:35.107718 c2cwsgiutils-6.0.0.dev96/c2cwsgiutils/broadcast/redis.py
--rw-r--r--   0        0        0      272 2023-07-01 19:56:35.107718 c2cwsgiutils-6.0.0.dev96/c2cwsgiutils/broadcast/utils.py
--rw-r--r--   0        0        0     3050 2023-07-01 19:56:35.107718 c2cwsgiutils-6.0.0.dev96/c2cwsgiutils/client_info.py
--rw-r--r--   0        0        0     1496 2023-07-01 19:56:35.107718 c2cwsgiutils-6.0.0.dev96/c2cwsgiutils/config_utils.py
--rw-r--r--   0        0        0      839 2023-07-01 19:56:35.107718 c2cwsgiutils-6.0.0.dev96/c2cwsgiutils/coverage_setup.py
--rw-r--r--   0        0        0    16140 2023-07-01 19:56:35.107718 c2cwsgiutils-6.0.0.dev96/c2cwsgiutils/db.py
--rw-r--r--   0        0        0     3049 2023-07-01 19:56:35.107718 c2cwsgiutils-6.0.0.dev96/c2cwsgiutils/db_maintenance_view.py
--rw-r--r--   0        0        0     1239 2023-07-01 19:56:35.107718 c2cwsgiutils-6.0.0.dev96/c2cwsgiutils/debug/__init__.py
--rw-r--r--   0        0        0     4370 2023-07-01 19:56:35.107718 c2cwsgiutils-6.0.0.dev96/c2cwsgiutils/debug/_listeners.py
--rw-r--r--   0        0        0     7507 2023-07-01 19:56:35.107718 c2cwsgiutils-6.0.0.dev96/c2cwsgiutils/debug/_views.py
--rw-r--r--   0        0        0     2328 2023-07-01 19:56:35.107718 c2cwsgiutils-6.0.0.dev96/c2cwsgiutils/debug/utils.py
--rw-r--r--   0        0        0     6723 2023-07-01 19:56:35.107718 c2cwsgiutils-6.0.0.dev96/c2cwsgiutils/errors.py
--rw-r--r--   0        0        0    20028 2023-07-01 19:56:35.107718 c2cwsgiutils-6.0.0.dev96/c2cwsgiutils/health_check.py
--rw-r--r--   0        0        0    17356 2023-07-01 19:56:35.107718 c2cwsgiutils-6.0.0.dev96/c2cwsgiutils/index.py
--rw-r--r--   0        0        0      628 2023-07-01 19:56:35.107718 c2cwsgiutils-6.0.0.dev96/c2cwsgiutils/loader.py
--rw-r--r--   0        0        0     3337 2023-07-01 19:56:35.107718 c2cwsgiutils-6.0.0.dev96/c2cwsgiutils/logging_view.py
--rw-r--r--   0        0        0     2691 2023-07-01 19:56:35.107718 c2cwsgiutils-6.0.0.dev96/c2cwsgiutils/models_graph.py
--rw-r--r--   0        0        0     1698 2023-07-01 19:56:35.107718 c2cwsgiutils-6.0.0.dev96/c2cwsgiutils/pretty_json.py
--rw-r--r--   0        0        0      739 2023-07-01 19:56:35.107718 c2cwsgiutils-6.0.0.dev96/c2cwsgiutils/profiler.py
--rw-r--r--   0        0        0     6599 2023-07-01 19:56:35.107718 c2cwsgiutils-6.0.0.dev96/c2cwsgiutils/prometheus.py
--rw-r--r--   0        0        0        0 2023-07-01 19:56:35.107718 c2cwsgiutils-6.0.0.dev96/c2cwsgiutils/py.typed
--rw-r--r--   0        0        0     1388 2023-07-01 19:56:35.107718 c2cwsgiutils-6.0.0.dev96/c2cwsgiutils/pyramid.py
--rw-r--r--   0        0        0     3703 2023-07-01 19:56:35.107718 c2cwsgiutils-6.0.0.dev96/c2cwsgiutils/pyramid_logging.py
--rw-r--r--   0        0        0     1545 2023-07-01 19:56:35.107718 c2cwsgiutils-6.0.0.dev96/c2cwsgiutils/redis_stats.py
--rw-r--r--   0        0        0     4689 2023-07-01 19:56:35.107718 c2cwsgiutils-6.0.0.dev96/c2cwsgiutils/redis_utils.py
--rw-r--r--   0        0        0     4025 2023-07-01 19:56:35.107718 c2cwsgiutils-6.0.0.dev96/c2cwsgiutils/request_tracking/__init__.py
--rw-r--r--   0        0        0      577 2023-07-01 19:56:35.107718 c2cwsgiutils-6.0.0.dev96/c2cwsgiutils/request_tracking/_sql.py
--rw-r--r--   0        0        0        0 2023-07-01 19:56:35.107718 c2cwsgiutils-6.0.0.dev96/c2cwsgiutils/scripts/__init__.py
--rwxr-xr-x   0        0        0     1998 2023-07-01 19:56:35.107718 c2cwsgiutils-6.0.0.dev96/c2cwsgiutils/scripts/genversion.py
--rwxr-xr-x   0        0        0    10445 2023-07-01 19:56:35.107718 c2cwsgiutils-6.0.0.dev96/c2cwsgiutils/scripts/stats_db.py
--rwxr-xr-x   0        0        0     2096 2023-07-01 19:56:35.107718 c2cwsgiutils-6.0.0.dev96/c2cwsgiutils/scripts/test_print.py
--rw-r--r--   0        0        0     5002 2023-07-01 19:56:35.107718 c2cwsgiutils-6.0.0.dev96/c2cwsgiutils/sentry.py
--rw-r--r--   0        0        0     1567 2023-07-01 19:56:35.107718 c2cwsgiutils-6.0.0.dev96/c2cwsgiutils/services.py
--rw-r--r--   0        0        0     3434 2023-07-01 19:56:35.107718 c2cwsgiutils-6.0.0.dev96/c2cwsgiutils/setup_process.py
--rw-r--r--   0        0        0      876 2023-07-01 19:56:35.107718 c2cwsgiutils-6.0.0.dev96/c2cwsgiutils/sql_profiler/__init__.py
--rw-r--r--   0        0        0     3680 2023-07-01 19:56:35.107718 c2cwsgiutils-6.0.0.dev96/c2cwsgiutils/sql_profiler/_impl.py
--rw-r--r--   0        0        0     1552 2023-07-01 19:56:35.107718 c2cwsgiutils-6.0.0.dev96/c2cwsgiutils/sqlalchemylogger/README.md
--rw-r--r--   0        0        0        0 2023-07-01 19:56:35.107718 c2cwsgiutils-6.0.0.dev96/c2cwsgiutils/sqlalchemylogger/__init__.py
--rw-r--r--   0        0        0      752 2023-07-01 19:56:35.107718 c2cwsgiutils-6.0.0.dev96/c2cwsgiutils/sqlalchemylogger/_filters.py
--rw-r--r--   0        0        0     1477 2023-07-01 19:56:35.107718 c2cwsgiutils-6.0.0.dev96/c2cwsgiutils/sqlalchemylogger/_models.py
--rw-r--r--   0        0        0      460 2023-07-01 19:56:35.107718 c2cwsgiutils-6.0.0.dev96/c2cwsgiutils/sqlalchemylogger/examples/example.py
--rw-r--r--   0        0        0     4813 2023-07-01 19:56:35.107718 c2cwsgiutils-6.0.0.dev96/c2cwsgiutils/sqlalchemylogger/handlers.py
--rw-r--r--   0        0        0      747 2023-07-01 19:56:35.107718 c2cwsgiutils-6.0.0.dev96/c2cwsgiutils/stats_pyramid/__init__.py
--rw-r--r--   0        0        0     2917 2023-07-01 19:56:35.107718 c2cwsgiutils-6.0.0.dev96/c2cwsgiutils/stats_pyramid/_db_spy.py
--rw-r--r--   0        0        0     3209 2023-07-01 19:56:35.107718 c2cwsgiutils-6.0.0.dev96/c2cwsgiutils/stats_pyramid/_pyramid_spy.py
--rw-r--r--   0        0        0     2876 2023-07-01 19:56:35.107718 c2cwsgiutils-6.0.0.dev96/c2cwsgiutils/version.py
--rw-r--r--   0        0        0     5186 2023-07-01 20:04:55.669233 c2cwsgiutils-6.0.0.dev96/pyproject.toml
--rw-r--r--   0        0        0    31984 1970-01-01 00:00:00.000000 c2cwsgiutils-6.0.0.dev96/PKG-INFO
+-rw-r--r--   0        0        0     1304 2023-07-01 21:57:50.589738 c2cwsgiutils-6.0.0.dev97/LICENSE
+-rw-r--r--   0        0        0    29129 2023-07-01 21:57:50.589738 c2cwsgiutils-6.0.0.dev97/README.md
+-rw-r--r--   0        0        0     3997 2023-07-01 21:57:50.593738 c2cwsgiutils-6.0.0.dev97/c2cwsgiutils/__init__.py
+-rw-r--r--   0        0        0     1500 2023-07-01 21:57:50.593738 c2cwsgiutils-6.0.0.dev97/c2cwsgiutils/acceptance/__init__.py
+-rw-r--r--   0        0        0     5331 2023-07-01 21:57:50.593738 c2cwsgiutils-6.0.0.dev97/c2cwsgiutils/acceptance/composition.py
+-rw-r--r--   0        0        0     9109 2023-07-01 21:57:50.593738 c2cwsgiutils-6.0.0.dev97/c2cwsgiutils/acceptance/connection.py
+-rw-r--r--   0        0        0     4701 2023-07-01 21:57:50.593738 c2cwsgiutils-6.0.0.dev97/c2cwsgiutils/acceptance/image.py
+-rw-r--r--   0        0        0     2329 2023-07-01 21:57:50.593738 c2cwsgiutils-6.0.0.dev97/c2cwsgiutils/acceptance/print.py
+-rw-r--r--   0        0        0     2078 2023-07-01 21:57:50.593738 c2cwsgiutils-6.0.0.dev97/c2cwsgiutils/acceptance/utils.py
+-rw-r--r--   0        0        0     9313 2023-07-01 21:57:50.593738 c2cwsgiutils-6.0.0.dev97/c2cwsgiutils/auth.py
+-rw-r--r--   0        0        0     4372 2023-07-01 21:57:50.593738 c2cwsgiutils-6.0.0.dev97/c2cwsgiutils/broadcast/__init__.py
+-rw-r--r--   0        0        0      615 2023-07-01 21:57:50.593738 c2cwsgiutils-6.0.0.dev97/c2cwsgiutils/broadcast/interface.py
+-rw-r--r--   0        0        0     1062 2023-07-01 21:57:50.593738 c2cwsgiutils-6.0.0.dev97/c2cwsgiutils/broadcast/local.py
+-rw-r--r--   0        0        0     5064 2023-07-01 21:57:50.593738 c2cwsgiutils-6.0.0.dev97/c2cwsgiutils/broadcast/redis.py
+-rw-r--r--   0        0        0      272 2023-07-01 21:57:50.593738 c2cwsgiutils-6.0.0.dev97/c2cwsgiutils/broadcast/utils.py
+-rw-r--r--   0        0        0     3050 2023-07-01 21:57:50.593738 c2cwsgiutils-6.0.0.dev97/c2cwsgiutils/client_info.py
+-rw-r--r--   0        0        0     1496 2023-07-01 21:57:50.593738 c2cwsgiutils-6.0.0.dev97/c2cwsgiutils/config_utils.py
+-rw-r--r--   0        0        0      839 2023-07-01 21:57:50.593738 c2cwsgiutils-6.0.0.dev97/c2cwsgiutils/coverage_setup.py
+-rw-r--r--   0        0        0    16140 2023-07-01 21:57:50.593738 c2cwsgiutils-6.0.0.dev97/c2cwsgiutils/db.py
+-rw-r--r--   0        0        0     3049 2023-07-01 21:57:50.593738 c2cwsgiutils-6.0.0.dev97/c2cwsgiutils/db_maintenance_view.py
+-rw-r--r--   0        0        0     1239 2023-07-01 21:57:50.593738 c2cwsgiutils-6.0.0.dev97/c2cwsgiutils/debug/__init__.py
+-rw-r--r--   0        0        0     4370 2023-07-01 21:57:50.593738 c2cwsgiutils-6.0.0.dev97/c2cwsgiutils/debug/_listeners.py
+-rw-r--r--   0        0        0     7507 2023-07-01 21:57:50.593738 c2cwsgiutils-6.0.0.dev97/c2cwsgiutils/debug/_views.py
+-rw-r--r--   0        0        0     2328 2023-07-01 21:57:50.593738 c2cwsgiutils-6.0.0.dev97/c2cwsgiutils/debug/utils.py
+-rw-r--r--   0        0        0     6723 2023-07-01 21:57:50.593738 c2cwsgiutils-6.0.0.dev97/c2cwsgiutils/errors.py
+-rw-r--r--   0        0        0    20028 2023-07-01 21:57:50.593738 c2cwsgiutils-6.0.0.dev97/c2cwsgiutils/health_check.py
+-rw-r--r--   0        0        0    17356 2023-07-01 21:57:50.597739 c2cwsgiutils-6.0.0.dev97/c2cwsgiutils/index.py
+-rw-r--r--   0        0        0      628 2023-07-01 21:57:50.597739 c2cwsgiutils-6.0.0.dev97/c2cwsgiutils/loader.py
+-rw-r--r--   0        0        0     3337 2023-07-01 21:57:50.597739 c2cwsgiutils-6.0.0.dev97/c2cwsgiutils/logging_view.py
+-rw-r--r--   0        0        0     2691 2023-07-01 21:57:50.597739 c2cwsgiutils-6.0.0.dev97/c2cwsgiutils/models_graph.py
+-rw-r--r--   0        0        0     1698 2023-07-01 21:57:50.597739 c2cwsgiutils-6.0.0.dev97/c2cwsgiutils/pretty_json.py
+-rw-r--r--   0        0        0      739 2023-07-01 21:57:50.597739 c2cwsgiutils-6.0.0.dev97/c2cwsgiutils/profiler.py
+-rw-r--r--   0        0        0     6599 2023-07-01 21:57:50.597739 c2cwsgiutils-6.0.0.dev97/c2cwsgiutils/prometheus.py
+-rw-r--r--   0        0        0        0 2023-07-01 21:57:50.597739 c2cwsgiutils-6.0.0.dev97/c2cwsgiutils/py.typed
+-rw-r--r--   0        0        0     1388 2023-07-01 21:57:50.597739 c2cwsgiutils-6.0.0.dev97/c2cwsgiutils/pyramid.py
+-rw-r--r--   0        0        0     3703 2023-07-01 21:57:50.597739 c2cwsgiutils-6.0.0.dev97/c2cwsgiutils/pyramid_logging.py
+-rw-r--r--   0        0        0     1545 2023-07-01 21:57:50.597739 c2cwsgiutils-6.0.0.dev97/c2cwsgiutils/redis_stats.py
+-rw-r--r--   0        0        0     4689 2023-07-01 21:57:50.597739 c2cwsgiutils-6.0.0.dev97/c2cwsgiutils/redis_utils.py
+-rw-r--r--   0        0        0     4025 2023-07-01 21:57:50.597739 c2cwsgiutils-6.0.0.dev97/c2cwsgiutils/request_tracking/__init__.py
+-rw-r--r--   0        0        0      577 2023-07-01 21:57:50.597739 c2cwsgiutils-6.0.0.dev97/c2cwsgiutils/request_tracking/_sql.py
+-rw-r--r--   0        0        0        0 2023-07-01 21:57:50.597739 c2cwsgiutils-6.0.0.dev97/c2cwsgiutils/scripts/__init__.py
+-rwxr-xr-x   0        0        0     1998 2023-07-01 21:57:50.597739 c2cwsgiutils-6.0.0.dev97/c2cwsgiutils/scripts/genversion.py
+-rwxr-xr-x   0        0        0    10445 2023-07-01 21:57:50.597739 c2cwsgiutils-6.0.0.dev97/c2cwsgiutils/scripts/stats_db.py
+-rwxr-xr-x   0        0        0     2096 2023-07-01 21:57:50.597739 c2cwsgiutils-6.0.0.dev97/c2cwsgiutils/scripts/test_print.py
+-rw-r--r--   0        0        0     5002 2023-07-01 21:57:50.597739 c2cwsgiutils-6.0.0.dev97/c2cwsgiutils/sentry.py
+-rw-r--r--   0        0        0     1567 2023-07-01 21:57:50.597739 c2cwsgiutils-6.0.0.dev97/c2cwsgiutils/services.py
+-rw-r--r--   0        0        0     3434 2023-07-01 21:57:50.597739 c2cwsgiutils-6.0.0.dev97/c2cwsgiutils/setup_process.py
+-rw-r--r--   0        0        0      876 2023-07-01 21:57:50.597739 c2cwsgiutils-6.0.0.dev97/c2cwsgiutils/sql_profiler/__init__.py
+-rw-r--r--   0        0        0     3680 2023-07-01 21:57:50.597739 c2cwsgiutils-6.0.0.dev97/c2cwsgiutils/sql_profiler/_impl.py
+-rw-r--r--   0        0        0     1552 2023-07-01 21:57:50.597739 c2cwsgiutils-6.0.0.dev97/c2cwsgiutils/sqlalchemylogger/README.md
+-rw-r--r--   0        0        0        0 2023-07-01 21:57:50.597739 c2cwsgiutils-6.0.0.dev97/c2cwsgiutils/sqlalchemylogger/__init__.py
+-rw-r--r--   0        0        0      752 2023-07-01 21:57:50.597739 c2cwsgiutils-6.0.0.dev97/c2cwsgiutils/sqlalchemylogger/_filters.py
+-rw-r--r--   0        0        0     1477 2023-07-01 21:57:50.597739 c2cwsgiutils-6.0.0.dev97/c2cwsgiutils/sqlalchemylogger/_models.py
+-rw-r--r--   0        0        0      460 2023-07-01 21:57:50.597739 c2cwsgiutils-6.0.0.dev97/c2cwsgiutils/sqlalchemylogger/examples/example.py
+-rw-r--r--   0        0        0     4813 2023-07-01 21:57:50.597739 c2cwsgiutils-6.0.0.dev97/c2cwsgiutils/sqlalchemylogger/handlers.py
+-rw-r--r--   0        0        0      747 2023-07-01 21:57:50.597739 c2cwsgiutils-6.0.0.dev97/c2cwsgiutils/stats_pyramid/__init__.py
+-rw-r--r--   0        0        0     2917 2023-07-01 21:57:50.597739 c2cwsgiutils-6.0.0.dev97/c2cwsgiutils/stats_pyramid/_db_spy.py
+-rw-r--r--   0        0        0     3209 2023-07-01 21:57:50.597739 c2cwsgiutils-6.0.0.dev97/c2cwsgiutils/stats_pyramid/_pyramid_spy.py
+-rw-r--r--   0        0        0     2876 2023-07-01 21:57:50.597739 c2cwsgiutils-6.0.0.dev97/c2cwsgiutils/version.py
+-rw-r--r--   0        0        0     5186 2023-07-01 22:06:48.085708 c2cwsgiutils-6.0.0.dev97/pyproject.toml
+-rw-r--r--   0        0        0    31984 1970-01-01 00:00:00.000000 c2cwsgiutils-6.0.0.dev97/PKG-INFO
```

### Comparing `c2cwsgiutils-6.0.0.dev96/LICENSE` & `c2cwsgiutils-6.0.0.dev97/LICENSE`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-6.0.0.dev96/README.md` & `c2cwsgiutils-6.0.0.dev97/README.md`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-6.0.0.dev96/c2cwsgiutils/__init__.py` & `c2cwsgiutils-6.0.0.dev97/c2cwsgiutils/__init__.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-6.0.0.dev96/c2cwsgiutils/acceptance/__init__.py` & `c2cwsgiutils-6.0.0.dev97/c2cwsgiutils/acceptance/__init__.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-6.0.0.dev96/c2cwsgiutils/acceptance/composition.py` & `c2cwsgiutils-6.0.0.dev97/c2cwsgiutils/acceptance/composition.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-6.0.0.dev96/c2cwsgiutils/acceptance/connection.py` & `c2cwsgiutils-6.0.0.dev97/c2cwsgiutils/acceptance/connection.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-6.0.0.dev96/c2cwsgiutils/acceptance/image.py` & `c2cwsgiutils-6.0.0.dev97/c2cwsgiutils/acceptance/image.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-6.0.0.dev96/c2cwsgiutils/acceptance/print.py` & `c2cwsgiutils-6.0.0.dev97/c2cwsgiutils/acceptance/print.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-6.0.0.dev96/c2cwsgiutils/acceptance/utils.py` & `c2cwsgiutils-6.0.0.dev97/c2cwsgiutils/acceptance/utils.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-6.0.0.dev96/c2cwsgiutils/auth.py` & `c2cwsgiutils-6.0.0.dev97/c2cwsgiutils/auth.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-6.0.0.dev96/c2cwsgiutils/broadcast/__init__.py` & `c2cwsgiutils-6.0.0.dev97/c2cwsgiutils/broadcast/__init__.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-6.0.0.dev96/c2cwsgiutils/broadcast/interface.py` & `c2cwsgiutils-6.0.0.dev97/c2cwsgiutils/broadcast/interface.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-6.0.0.dev96/c2cwsgiutils/broadcast/local.py` & `c2cwsgiutils-6.0.0.dev97/c2cwsgiutils/broadcast/local.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-6.0.0.dev96/c2cwsgiutils/broadcast/redis.py` & `c2cwsgiutils-6.0.0.dev97/c2cwsgiutils/broadcast/redis.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-6.0.0.dev96/c2cwsgiutils/client_info.py` & `c2cwsgiutils-6.0.0.dev97/c2cwsgiutils/client_info.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-6.0.0.dev96/c2cwsgiutils/config_utils.py` & `c2cwsgiutils-6.0.0.dev97/c2cwsgiutils/config_utils.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-6.0.0.dev96/c2cwsgiutils/coverage_setup.py` & `c2cwsgiutils-6.0.0.dev97/c2cwsgiutils/coverage_setup.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-6.0.0.dev96/c2cwsgiutils/db.py` & `c2cwsgiutils-6.0.0.dev97/c2cwsgiutils/db.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-6.0.0.dev96/c2cwsgiutils/db_maintenance_view.py` & `c2cwsgiutils-6.0.0.dev97/c2cwsgiutils/db_maintenance_view.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-6.0.0.dev96/c2cwsgiutils/debug/__init__.py` & `c2cwsgiutils-6.0.0.dev97/c2cwsgiutils/debug/__init__.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-6.0.0.dev96/c2cwsgiutils/debug/_listeners.py` & `c2cwsgiutils-6.0.0.dev97/c2cwsgiutils/debug/_listeners.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-6.0.0.dev96/c2cwsgiutils/debug/_views.py` & `c2cwsgiutils-6.0.0.dev97/c2cwsgiutils/debug/_views.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-6.0.0.dev96/c2cwsgiutils/debug/utils.py` & `c2cwsgiutils-6.0.0.dev97/c2cwsgiutils/debug/utils.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-6.0.0.dev96/c2cwsgiutils/errors.py` & `c2cwsgiutils-6.0.0.dev97/c2cwsgiutils/errors.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-6.0.0.dev96/c2cwsgiutils/health_check.py` & `c2cwsgiutils-6.0.0.dev97/c2cwsgiutils/health_check.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-6.0.0.dev96/c2cwsgiutils/index.py` & `c2cwsgiutils-6.0.0.dev97/c2cwsgiutils/index.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-6.0.0.dev96/c2cwsgiutils/loader.py` & `c2cwsgiutils-6.0.0.dev97/c2cwsgiutils/loader.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-6.0.0.dev96/c2cwsgiutils/logging_view.py` & `c2cwsgiutils-6.0.0.dev97/c2cwsgiutils/logging_view.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-6.0.0.dev96/c2cwsgiutils/models_graph.py` & `c2cwsgiutils-6.0.0.dev97/c2cwsgiutils/models_graph.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-6.0.0.dev96/c2cwsgiutils/pretty_json.py` & `c2cwsgiutils-6.0.0.dev97/c2cwsgiutils/pretty_json.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-6.0.0.dev96/c2cwsgiutils/profiler.py` & `c2cwsgiutils-6.0.0.dev97/c2cwsgiutils/profiler.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-6.0.0.dev96/c2cwsgiutils/prometheus.py` & `c2cwsgiutils-6.0.0.dev97/c2cwsgiutils/prometheus.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-6.0.0.dev96/c2cwsgiutils/pyramid.py` & `c2cwsgiutils-6.0.0.dev97/c2cwsgiutils/pyramid.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-6.0.0.dev96/c2cwsgiutils/pyramid_logging.py` & `c2cwsgiutils-6.0.0.dev97/c2cwsgiutils/pyramid_logging.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-6.0.0.dev96/c2cwsgiutils/redis_stats.py` & `c2cwsgiutils-6.0.0.dev97/c2cwsgiutils/redis_stats.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-6.0.0.dev96/c2cwsgiutils/redis_utils.py` & `c2cwsgiutils-6.0.0.dev97/c2cwsgiutils/redis_utils.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-6.0.0.dev96/c2cwsgiutils/request_tracking/__init__.py` & `c2cwsgiutils-6.0.0.dev97/c2cwsgiutils/request_tracking/__init__.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-6.0.0.dev96/c2cwsgiutils/request_tracking/_sql.py` & `c2cwsgiutils-6.0.0.dev97/c2cwsgiutils/request_tracking/_sql.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-6.0.0.dev96/c2cwsgiutils/scripts/genversion.py` & `c2cwsgiutils-6.0.0.dev97/c2cwsgiutils/scripts/genversion.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-6.0.0.dev96/c2cwsgiutils/scripts/stats_db.py` & `c2cwsgiutils-6.0.0.dev97/c2cwsgiutils/scripts/stats_db.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-6.0.0.dev96/c2cwsgiutils/scripts/test_print.py` & `c2cwsgiutils-6.0.0.dev97/c2cwsgiutils/scripts/test_print.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-6.0.0.dev96/c2cwsgiutils/sentry.py` & `c2cwsgiutils-6.0.0.dev97/c2cwsgiutils/sentry.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-6.0.0.dev96/c2cwsgiutils/services.py` & `c2cwsgiutils-6.0.0.dev97/c2cwsgiutils/services.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-6.0.0.dev96/c2cwsgiutils/setup_process.py` & `c2cwsgiutils-6.0.0.dev97/c2cwsgiutils/setup_process.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-6.0.0.dev96/c2cwsgiutils/sql_profiler/__init__.py` & `c2cwsgiutils-6.0.0.dev97/c2cwsgiutils/sql_profiler/__init__.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-6.0.0.dev96/c2cwsgiutils/sql_profiler/_impl.py` & `c2cwsgiutils-6.0.0.dev97/c2cwsgiutils/sql_profiler/_impl.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-6.0.0.dev96/c2cwsgiutils/sqlalchemylogger/README.md` & `c2cwsgiutils-6.0.0.dev97/c2cwsgiutils/sqlalchemylogger/README.md`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-6.0.0.dev96/c2cwsgiutils/sqlalchemylogger/_filters.py` & `c2cwsgiutils-6.0.0.dev97/c2cwsgiutils/sqlalchemylogger/_filters.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-6.0.0.dev96/c2cwsgiutils/sqlalchemylogger/_models.py` & `c2cwsgiutils-6.0.0.dev97/c2cwsgiutils/sqlalchemylogger/_models.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-6.0.0.dev96/c2cwsgiutils/sqlalchemylogger/handlers.py` & `c2cwsgiutils-6.0.0.dev97/c2cwsgiutils/sqlalchemylogger/handlers.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-6.0.0.dev96/c2cwsgiutils/stats_pyramid/__init__.py` & `c2cwsgiutils-6.0.0.dev97/c2cwsgiutils/stats_pyramid/__init__.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-6.0.0.dev96/c2cwsgiutils/stats_pyramid/_db_spy.py` & `c2cwsgiutils-6.0.0.dev97/c2cwsgiutils/stats_pyramid/_db_spy.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-6.0.0.dev96/c2cwsgiutils/stats_pyramid/_pyramid_spy.py` & `c2cwsgiutils-6.0.0.dev97/c2cwsgiutils/stats_pyramid/_pyramid_spy.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-6.0.0.dev96/c2cwsgiutils/version.py` & `c2cwsgiutils-6.0.0.dev97/c2cwsgiutils/version.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-6.0.0.dev96/pyproject.toml` & `c2cwsgiutils-6.0.0.dev97/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 warn_redundant_casts = true
 warn_unused_ignores = true
 warn_return_any = true
 strict = true
 
 [tool.poetry]
 name = "c2cwsgiutils"
-version = "6.0.0.dev96"
+version = "6.0.0.dev97"
 description = "Common utilities for Camptocamp WSGI applications"
 readme = "README.md"
 authors = ["Camptocamp <info@camptocamp.com>"]
 keywords = ["geo", "gis", "sqlalchemy", "orm", "wsgi"]
 repository = "https://github.com/camptocamp/c2cwsgiutils"
 license = "BSD-2-Clause"
 classifiers = [
@@ -64,35 +64,35 @@
 [tool.poetry.dependencies]
 python = ">=3.8,<4.0"
 requests = { version = "2.31.0" }
 pyyaml = { version = "6.0" }
 alembic = { version = "1.11.1", optional = true }
 boltons = { version = "23.0.0", optional = true }
 cornice = { version = "6.0.1", optional = true }
-redis = { version = "4.5.4", optional = true }
+redis = { version = "4.6.0", optional = true }
 gunicorn = { version = "20.1.0", optional = true }
 lxml = { version = "4.9.2", optional = true }
 netifaces = { version = "0.11.0", optional = true }
-objgraph = { version = "3.5.0", optional = true }
+objgraph = { version = "3.6.0", optional = true }
 psycopg2 = { version = "2.9.6", optional = true }
 pyramid = { version = "2.0.1", optional = true }
 pyramid-tm = { version = "2.5", optional = true }
-sentry-sdk = { version = "1.24.0", optional = true }
-ujson = { version = "5.7.0", optional = true }
+sentry-sdk = { version = "1.26.0", optional = true }
+ujson = { version = "5.8.0", optional = true }
 cee_syslog_handler = { version = "0.6.0", optional = true }
 SQLAlchemy = { version = "2.0.15", optional = true }
 SQLAlchemy-Utils = { version = "0.41.1", optional = true }
 "zope.interface" = { version = "6.0", optional = true }
 "zope.sqlalchemy" = { version = "3.0", optional = true }
 pyjwt = { version = "2.7.0", optional = true }
 requests-oauthlib = { version = "1.3.1", optional = true }
 waitress = { version = "2.1.2", optional = true }
-scikit-image = { version = "0.20.0", optional = true }
+scikit-image = { version = "0.21.0", optional = true }
 certifi = "2023.5.7"
-prometheus-client = "0.16.0"
+prometheus-client = "0.17.0"
 
 [tool.poetry.extras]
 standard = [
   "alembic",
   "boltons",
   "cornice",
   "redis",
@@ -141,23 +141,23 @@
 test_images = ["scikit-image"]
 
 [tool.poetry.dev-dependencies]
 # pylint = { version = "2.15.6" }
 prospector = { extras = ["with_bandit", "with_mypy", "with_pyroma"], version = "1.10.2" }
 coverage = "7.2.7"
 junit2html = "30.1.3"
-pytest = "7.3.1"
+pytest = "7.4.0"
 pytest-cov = "4.1.0"
 pytest-html = "3.2.0"
 types-pyyaml = "6.0.12.10"
 types-requests = "2.31.0.1"
-types-redis = "4.5.4.1"
-types-ujson = "5.7.0.5"
+types-redis = "4.6.0.1"
+types-ujson = "5.8.0.0"
 types-python-dateutil = "2.8.19.13"
-typing_extensions = "4.6.3"
+typing_extensions = "4.7.0"
 
 [build-system]
 requires = [
   "poetry-core>=1.0.0",
   "poetry-dynamic-versioning[plugin]",
   "poetry-plugin-tweak-dependencies-version"
 ]
```

### Comparing `c2cwsgiutils-6.0.0.dev96/PKG-INFO` & `c2cwsgiutils-6.0.0.dev97/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: c2cwsgiutils
-Version: 6.0.0.dev96
+Version: 6.0.0.dev97
 Summary: Common utilities for Camptocamp WSGI applications
 Home-page: https://github.com/camptocamp/c2cwsgiutils
 License: BSD-2-Clause
 Keywords: geo,gis,sqlalchemy,orm,wsgi
 Author: Camptocamp
 Author-email: info@camptocamp.com
 Requires-Python: >=3.8,<4.0
```

