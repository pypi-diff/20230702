# Comparing `tmp/newrelic_sb_sdk-0.8.0.tar.gz` & `tmp/newrelic_sb_sdk-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "newrelic_sb_sdk-0.8.0.tar", max compression
+gzip compressed data, was "newrelic_sb_sdk-0.9.0.tar", max compression
```

## Comparing `newrelic_sb_sdk-0.8.0.tar` & `newrelic_sb_sdk-0.9.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     1529 2023-07-01 07:27:04.765278 newrelic_sb_sdk-0.8.0/CHANGELOG.md
--rw-r--r--   0        0        0     1070 2023-03-04 20:34:24.170848 newrelic_sb_sdk-0.8.0/LICENSE.txt
--rw-r--r--   0        0        0     3001 2023-07-01 07:20:37.782587 newrelic_sb_sdk-0.8.0/README.md
--rw-r--r--   0        0        0     2923 2023-07-01 07:27:04.765278 newrelic_sb_sdk-0.8.0/pyproject.toml
--rw-r--r--   0        0        0       22 2023-07-01 07:27:04.769277 newrelic_sb_sdk-0.8.0/src/newrelic_sb_sdk/__init__.py
--rw-r--r--   0        0        0   389324 2023-07-01 07:06:47.079444 newrelic_sb_sdk-0.8.0/src/newrelic_sb_sdk/_modidx.py
--rw-r--r--   0        0        0     4902 2023-06-06 01:14:25.651692 newrelic_sb_sdk-0.8.0/src/newrelic_sb_sdk/alerts/__init__.py
--rw-r--r--   0        0        0     1541 2023-03-12 12:22:19.009570 newrelic_sb_sdk-0.8.0/src/newrelic_sb_sdk/alerts/enums.py
--rw-r--r--   0        0        0      769 2023-06-05 12:25:15.706671 newrelic_sb_sdk-0.8.0/src/newrelic_sb_sdk/alerts/utils.py
--rw-r--r--   0        0        0     2024 2023-06-12 17:56:42.971757 newrelic_sb_sdk-0.8.0/src/newrelic_sb_sdk/client/__init__.py
--rw-r--r--   0        0        0        0 2023-03-10 03:57:33.224743 newrelic_sb_sdk-0.8.0/src/newrelic_sb_sdk/core/__init__.py
--rw-r--r--   0        0        0      372 2023-03-10 03:57:33.224743 newrelic_sb_sdk-0.8.0/src/newrelic_sb_sdk/core/base.py
--rw-r--r--   0        0        0      747 2023-03-10 03:57:33.224743 newrelic_sb_sdk-0.8.0/src/newrelic_sb_sdk/core/encoders.py
--rw-r--r--   0        0        0     2235 2023-06-06 01:14:25.651692 newrelic_sb_sdk-0.8.0/src/newrelic_sb_sdk/core/mixins.py
--rw-r--r--   0        0        0     1175 2023-06-06 01:14:25.651692 newrelic_sb_sdk-0.8.0/src/newrelic_sb_sdk/dashboards/__init__.py
--rw-r--r--   0        0        0     1095 2023-03-10 03:57:33.224743 newrelic_sb_sdk-0.8.0/src/newrelic_sb_sdk/dashboards/enums.py
--rw-r--r--   0        0        0     1006 2023-06-06 01:14:25.651692 newrelic_sb_sdk-0.8.0/src/newrelic_sb_sdk/dashboards/pages.py
--rw-r--r--   0        0        0      593 2023-06-06 01:14:25.651692 newrelic_sb_sdk-0.8.0/src/newrelic_sb_sdk/dashboards/utils.py
--rw-r--r--   0        0        0     3583 2023-06-06 01:14:25.651692 newrelic_sb_sdk-0.8.0/src/newrelic_sb_sdk/dashboards/widgets.py
--rw-r--r--   0        0        0      200 2023-03-10 03:57:33.224743 newrelic_sb_sdk-0.8.0/src/newrelic_sb_sdk/graphql/__init__.py
--rw-r--r--   0        0        0    58745 2023-07-01 07:06:47.079444 newrelic_sb_sdk-0.8.0/src/newrelic_sb_sdk/graphql/enums.py
--rw-r--r--   0        0        0   362780 2023-07-01 07:06:47.079444 newrelic_sb_sdk-0.8.0/src/newrelic_sb_sdk/graphql/input_objects.py
--rw-r--r--   0        0        0   753602 2023-07-01 07:06:47.083444 newrelic_sb_sdk-0.8.0/src/newrelic_sb_sdk/graphql/objects.py
--rw-r--r--   0        0        0     3054 2023-06-10 11:02:34.187465 newrelic_sb_sdk-0.8.0/src/newrelic_sb_sdk/graphql/scalars.py
--rw-r--r--   0        0        0        0 2023-03-10 03:57:33.232743 newrelic_sb_sdk-0.8.0/src/newrelic_sb_sdk/utils/__init__.py
--rw-r--r--   0        0        0      329 2023-06-12 17:56:42.971757 newrelic_sb_sdk-0.8.0/src/newrelic_sb_sdk/utils/query.py
--rw-r--r--   0        0        0      787 2023-06-06 01:14:25.651692 newrelic_sb_sdk-0.8.0/src/newrelic_sb_sdk/utils/response.py
--rw-r--r--   0        0        0     1901 2023-03-10 03:57:33.232743 newrelic_sb_sdk-0.8.0/src/newrelic_sb_sdk/utils/text.py
--rw-r--r--   0        0        0     4748 1970-01-01 00:00:00.000000 newrelic_sb_sdk-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1678 2023-07-02 18:58:11.350663 newrelic_sb_sdk-0.9.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1070 2023-07-01 07:22:37.111976 newrelic_sb_sdk-0.9.0/LICENSE.txt
+-rw-r--r--   0        0        0     3001 2023-07-01 07:22:37.111976 newrelic_sb_sdk-0.9.0/README.md
+-rw-r--r--   0        0        0     3036 2023-07-02 18:58:11.350663 newrelic_sb_sdk-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-07-02 18:58:11.350663 newrelic_sb_sdk-0.9.0/src/newrelic_sb_sdk/__init__.py
+-rw-r--r--   0        0        0   389324 2023-07-01 07:22:37.151974 newrelic_sb_sdk-0.9.0/src/newrelic_sb_sdk/_modidx.py
+-rw-r--r--   0        0        0     4902 2023-07-01 07:22:37.151974 newrelic_sb_sdk-0.9.0/src/newrelic_sb_sdk/alerts/__init__.py
+-rw-r--r--   0        0        0     1541 2023-07-01 07:22:37.151974 newrelic_sb_sdk-0.9.0/src/newrelic_sb_sdk/alerts/enums.py
+-rw-r--r--   0        0        0      769 2023-07-01 07:22:37.151974 newrelic_sb_sdk-0.9.0/src/newrelic_sb_sdk/alerts/utils.py
+-rw-r--r--   0        0        0     2024 2023-07-01 07:22:37.151974 newrelic_sb_sdk-0.9.0/src/newrelic_sb_sdk/client/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-01 07:22:37.151974 newrelic_sb_sdk-0.9.0/src/newrelic_sb_sdk/core/__init__.py
+-rw-r--r--   0        0        0      372 2023-07-01 07:22:37.151974 newrelic_sb_sdk-0.9.0/src/newrelic_sb_sdk/core/base.py
+-rw-r--r--   0        0        0      747 2023-07-01 07:22:37.151974 newrelic_sb_sdk-0.9.0/src/newrelic_sb_sdk/core/encoders.py
+-rw-r--r--   0        0        0     2235 2023-07-01 07:22:37.151974 newrelic_sb_sdk-0.9.0/src/newrelic_sb_sdk/core/mixins.py
+-rw-r--r--   0        0        0     1175 2023-07-01 07:22:37.151974 newrelic_sb_sdk-0.9.0/src/newrelic_sb_sdk/dashboards/__init__.py
+-rw-r--r--   0        0        0     1095 2023-07-01 07:22:37.151974 newrelic_sb_sdk-0.9.0/src/newrelic_sb_sdk/dashboards/enums.py
+-rw-r--r--   0        0        0     1006 2023-07-01 07:22:37.151974 newrelic_sb_sdk-0.9.0/src/newrelic_sb_sdk/dashboards/pages.py
+-rw-r--r--   0        0        0      593 2023-07-01 07:22:37.151974 newrelic_sb_sdk-0.9.0/src/newrelic_sb_sdk/dashboards/utils.py
+-rw-r--r--   0        0        0     3583 2023-07-01 07:22:37.151974 newrelic_sb_sdk-0.9.0/src/newrelic_sb_sdk/dashboards/widgets.py
+-rw-r--r--   0        0        0      200 2023-07-01 07:22:37.151974 newrelic_sb_sdk-0.9.0/src/newrelic_sb_sdk/graphql/__init__.py
+-rw-r--r--   0        0        0    58745 2023-07-01 07:22:37.155974 newrelic_sb_sdk-0.9.0/src/newrelic_sb_sdk/graphql/enums.py
+-rw-r--r--   0        0        0   362780 2023-07-01 07:22:37.155974 newrelic_sb_sdk-0.9.0/src/newrelic_sb_sdk/graphql/input_objects.py
+-rw-r--r--   0        0        0   753602 2023-07-01 07:22:37.159973 newrelic_sb_sdk-0.9.0/src/newrelic_sb_sdk/graphql/objects.py
+-rw-r--r--   0        0        0     3054 2023-07-01 07:22:37.159973 newrelic_sb_sdk-0.9.0/src/newrelic_sb_sdk/graphql/scalars.py
+-rw-r--r--   0        0        0        0 2023-07-01 07:22:37.159973 newrelic_sb_sdk-0.9.0/src/newrelic_sb_sdk/utils/__init__.py
+-rw-r--r--   0        0        0      329 2023-07-01 07:22:37.159973 newrelic_sb_sdk-0.9.0/src/newrelic_sb_sdk/utils/query.py
+-rw-r--r--   0        0        0      787 2023-07-01 07:22:37.159973 newrelic_sb_sdk-0.9.0/src/newrelic_sb_sdk/utils/response.py
+-rw-r--r--   0        0        0     1901 2023-07-01 07:22:37.159973 newrelic_sb_sdk-0.9.0/src/newrelic_sb_sdk/utils/text.py
+-rw-r--r--   0        0        0     4748 1970-01-01 00:00:00.000000 newrelic_sb_sdk-0.9.0/PKG-INFO
```

### Comparing `newrelic_sb_sdk-0.8.0/CHANGELOG.md` & `newrelic_sb_sdk-0.9.0/CHANGELOG.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,23 @@
 # Changelog
 
 ## [Unreleased]
 
+## [0.9.0] - 2023-07-02
+
+* Report test execution to Gitlab
+* Update Gitlab CI/CD pipelines
+* Restore docs building and publishing to Gitlab Pages
+
 ## [0.8.0] - 2023-07-01
 
 * Update GraphQL submodule with a fresh schema version.
 * Update dependencies
 * Add tests
-* Add autoplush with GitLab CI/CD
+* Add autopublish with GitLab CI/CD
 
 ## [0.7.0] - 2023-06-12
 
 * Rename arguments in NewRelicGqlClient.build_query method and build_query function from `query_params` to `params` and  `query_string` to `template`.
 * Update graphql module.
 * Add metadata about language info in GraphQL notebook.
 * Add new clasifiers for PyPi.
```

### Comparing `newrelic_sb_sdk-0.8.0/LICENSE.txt` & `newrelic_sb_sdk-0.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `newrelic_sb_sdk-0.8.0/README.md` & `newrelic_sb_sdk-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `newrelic_sb_sdk-0.8.0/pyproject.toml` & `newrelic_sb_sdk-0.9.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "newrelic-sb-sdk"
-version = "0.8.0"
+version = "0.9.0"
 description = "New Relic SDK to interact with Nerdgraph API."
 authors = [
   "SoftButterfly Development Team <dev@softbutterfly.io>",
   "zodiacfireworks <martin.vuelta@gmail.com>"
 ]
 license = "MIT License"
 readme = "README.md"
@@ -39,15 +39,15 @@
 ]
 include = [
   "LICENSE.txt",
   "CHANGELOG.md",
 ]
 
 [tool.poetry.urls]
-"Download" = "https://gitlab.com/softbutterfly/open-source/newrelic-sb-sdk/-/archive/v0.8.0/newrelic-sb-sdk-v0.8.0.tar.gz"
+"Download" = "https://gitlab.com/softbutterfly/open-source/newrelic-sb-sdk/-/archive/v0.9.0/newrelic-sb-sdk-v0.9.0.tar.gz"
 "Bug Tracker" = "https://gitlab.com/softbutterfly/open-source/newrelic-sb-sdk/-/issues"
 
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0.0"
 python-dotenv = "^1.0.0"
 requests = "^2.31.0"
@@ -110,14 +110,18 @@
   "**/test_*.py",
 ]
 filterwarnings =[
   "ignore::DeprecationWarning",
   "ignore::PendingDeprecationWarning"
 ]
 addopts = [
+  "--cov=newrelic_sb_sdk",
+  "--cov-report=xml:cobertura.xml",
+  "--cov-report=term",
   "--import-mode=importlib",
+  "--junitxml=report.xml",
   "--nbmake",
 ]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `newrelic_sb_sdk-0.8.0/src/newrelic_sb_sdk/_modidx.py` & `newrelic_sb_sdk-0.9.0/src/newrelic_sb_sdk/_modidx.py`

 * *Files identical despite different names*

### Comparing `newrelic_sb_sdk-0.8.0/src/newrelic_sb_sdk/alerts/__init__.py` & `newrelic_sb_sdk-0.9.0/src/newrelic_sb_sdk/alerts/__init__.py`

 * *Files identical despite different names*

### Comparing `newrelic_sb_sdk-0.8.0/src/newrelic_sb_sdk/alerts/enums.py` & `newrelic_sb_sdk-0.9.0/src/newrelic_sb_sdk/alerts/enums.py`

 * *Files identical despite different names*

### Comparing `newrelic_sb_sdk-0.8.0/src/newrelic_sb_sdk/alerts/utils.py` & `newrelic_sb_sdk-0.9.0/src/newrelic_sb_sdk/alerts/utils.py`

 * *Files identical despite different names*

### Comparing `newrelic_sb_sdk-0.8.0/src/newrelic_sb_sdk/client/__init__.py` & `newrelic_sb_sdk-0.9.0/src/newrelic_sb_sdk/client/__init__.py`

 * *Files identical despite different names*

### Comparing `newrelic_sb_sdk-0.8.0/src/newrelic_sb_sdk/core/encoders.py` & `newrelic_sb_sdk-0.9.0/src/newrelic_sb_sdk/core/encoders.py`

 * *Files identical despite different names*

### Comparing `newrelic_sb_sdk-0.8.0/src/newrelic_sb_sdk/core/mixins.py` & `newrelic_sb_sdk-0.9.0/src/newrelic_sb_sdk/core/mixins.py`

 * *Files identical despite different names*

### Comparing `newrelic_sb_sdk-0.8.0/src/newrelic_sb_sdk/dashboards/__init__.py` & `newrelic_sb_sdk-0.9.0/src/newrelic_sb_sdk/dashboards/__init__.py`

 * *Files identical despite different names*

### Comparing `newrelic_sb_sdk-0.8.0/src/newrelic_sb_sdk/dashboards/enums.py` & `newrelic_sb_sdk-0.9.0/src/newrelic_sb_sdk/dashboards/enums.py`

 * *Files identical despite different names*

### Comparing `newrelic_sb_sdk-0.8.0/src/newrelic_sb_sdk/dashboards/pages.py` & `newrelic_sb_sdk-0.9.0/src/newrelic_sb_sdk/dashboards/pages.py`

 * *Files identical despite different names*

### Comparing `newrelic_sb_sdk-0.8.0/src/newrelic_sb_sdk/dashboards/utils.py` & `newrelic_sb_sdk-0.9.0/src/newrelic_sb_sdk/dashboards/utils.py`

 * *Files identical despite different names*

### Comparing `newrelic_sb_sdk-0.8.0/src/newrelic_sb_sdk/dashboards/widgets.py` & `newrelic_sb_sdk-0.9.0/src/newrelic_sb_sdk/dashboards/widgets.py`

 * *Files identical despite different names*

### Comparing `newrelic_sb_sdk-0.8.0/src/newrelic_sb_sdk/graphql/enums.py` & `newrelic_sb_sdk-0.9.0/src/newrelic_sb_sdk/graphql/enums.py`

 * *Files identical despite different names*

### Comparing `newrelic_sb_sdk-0.8.0/src/newrelic_sb_sdk/graphql/input_objects.py` & `newrelic_sb_sdk-0.9.0/src/newrelic_sb_sdk/graphql/input_objects.py`

 * *Files identical despite different names*

### Comparing `newrelic_sb_sdk-0.8.0/src/newrelic_sb_sdk/graphql/objects.py` & `newrelic_sb_sdk-0.9.0/src/newrelic_sb_sdk/graphql/objects.py`

 * *Files identical despite different names*

### Comparing `newrelic_sb_sdk-0.8.0/src/newrelic_sb_sdk/graphql/scalars.py` & `newrelic_sb_sdk-0.9.0/src/newrelic_sb_sdk/graphql/scalars.py`

 * *Files identical despite different names*

### Comparing `newrelic_sb_sdk-0.8.0/src/newrelic_sb_sdk/utils/response.py` & `newrelic_sb_sdk-0.9.0/src/newrelic_sb_sdk/utils/response.py`

 * *Files identical despite different names*

### Comparing `newrelic_sb_sdk-0.8.0/src/newrelic_sb_sdk/utils/text.py` & `newrelic_sb_sdk-0.9.0/src/newrelic_sb_sdk/utils/text.py`

 * *Files identical despite different names*

### Comparing `newrelic_sb_sdk-0.8.0/PKG-INFO` & `newrelic_sb_sdk-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: newrelic-sb-sdk
-Version: 0.8.0
+Version: 0.9.0
 Summary: New Relic SDK to interact with Nerdgraph API.
 Home-page: https://gitlab.com/softbutterfly/open-source/newrelic-sb-sdk
 License: MIT
 Keywords: Softbutterfly,New Relic,SDK
 Author: SoftButterfly Development Team
 Author-email: dev@softbutterfly.io
 Requires-Python: >=3.8.1,<4.0.0
@@ -26,15 +26,15 @@
 Classifier: Topic :: System :: Monitoring
 Classifier: Topic :: System :: Networking :: Monitoring
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: sgqlc (>=16.1,<17.0)
 Project-URL: Bug Tracker, https://gitlab.com/softbutterfly/open-source/newrelic-sb-sdk/-/issues
 Project-URL: Documentation, https://softbutterfly.gitlab.io/open-source/newrelic-sb-sdk/
-Project-URL: Download, https://gitlab.com/softbutterfly/open-source/newrelic-sb-sdk/-/archive/v0.8.0/newrelic-sb-sdk-v0.8.0.tar.gz
+Project-URL: Download, https://gitlab.com/softbutterfly/open-source/newrelic-sb-sdk/-/archive/v0.9.0/newrelic-sb-sdk-v0.9.0.tar.gz
 Project-URL: Repository, https://gitlab.com/softbutterfly/open-source/newrelic-sb-sdk
 Description-Content-Type: text/markdown
 
 ![Community-Project](https://gitlab.com/softbutterfly/open-source/open-source-office/-/raw/master/banners/softbutterfly-open-source--banner--community-project.png)
 
 ![PyPI - Supported versions](https://img.shields.io/pypi/pyversions/newrelic-sb-sdk)
 ![PyPI - Package version](https://img.shields.io/pypi/v/newrelic-sb-sdk)
```

