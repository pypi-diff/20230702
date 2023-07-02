# Comparing `tmp/aleksis-2023.6b1.tar.gz` & `tmp/aleksis-2023.6b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aleksis-2023.6b1.tar", max compression
+gzip compressed data, was "aleksis-2023.6b2.tar", max compression
```

## Comparing `aleksis-2023.6b1.tar` & `aleksis-2023.6b2.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     6489 2023-05-28 12:04:44.365658 aleksis-2023.6b1/README.rst
--rw-r--r--   0        0        0        0 2023-05-28 12:04:44.365658 aleksis-2023.6b1/aleksis_meta/__init__.py
--rw-r--r--   0        0        0     1296 2023-05-28 12:22:47.072994 aleksis-2023.6b1/pyproject.toml
--rw-r--r--   0        0        0     8025 1970-01-01 00:00:00.000000 aleksis-2023.6b1/PKG-INFO
+-rw-r--r--   0        0        0     6489 2023-06-26 19:07:09.539206 aleksis-2023.6b2/README.rst
+-rw-r--r--   0        0        0        0 2023-06-26 19:07:09.539206 aleksis-2023.6b2/aleksis_meta/__init__.py
+-rw-r--r--   0        0        0     1290 2023-07-02 09:25:27.181736 aleksis-2023.6b2/pyproject.toml
+-rw-r--r--   0        0        0     8025 1970-01-01 00:00:00.000000 aleksis-2023.6b2/PKG-INFO
```

### Comparing `aleksis-2023.6b1/README.rst` & `aleksis-2023.6b2/README.rst`

 * *Files identical despite different names*

### Comparing `aleksis-2023.6b1/pyproject.toml` & `aleksis-2023.6b2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 [tool.poetry]
 name = "AlekSIS"
-version = "2023.6b1"
-packages = [ { include = "aleksis_meta" } ]
+version = "2023.6b2"
+packages = [{ include = "aleksis_meta" }]
 include = ["LICNECE.rst"]
 readme = "README.rst"
 
 description = "Free School Information System Distribution"
 authors = ["Dominik George <dominik.george@teckids.org>"]
-maintainers = ["Jonathan Weth <wethjo@katharineum.de>", "Dominik George <dominik.george@teckids.org>"]
+maintainers = [
+  "Jonathan Weth <wethjo@katharineum.de>",
+  "Dominik George <dominik.george@teckids.org>",
+]
 license = "EUPL-1.2-or-later"
 homepage = "https://aleksis.org/"
 repository = "https://edugit.org/AlekSIS/official/AlekSIS"
 keywords = ["SIS", "education", "school", "digitisation", "school apps"]
 classifiers = [
-    "Development Status :: 5 - Production/Stable",
-    "Environment :: Web Environment",
-    "Framework :: Django :: 3.0",
-    "Intended Audience :: Developers",
-    "Intended Audience :: Education",
-    "Topic :: Education",
+  "Development Status :: 5 - Production/Stable",
+  "Environment :: Web Environment",
+  "Framework :: Django :: 3.0",
+  "Intended Audience :: Developers",
+  "Intended Audience :: Education",
+  "Topic :: Education",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
-aleksis-core = { version = "~3.0", extras = ["ldap", "s3", "sentry"]}
+aleksis-core = { version = "~3.1", extras = ["ldap", "s3", "sentry"] }
 aleksis-app-alsijil = "~3.0"
 aleksis-app-chronos = "~3.0"
 aleksis-app-csvimport = "~3.0"
 aleksis-app-dashboardfeeds = "~3.0"
 aleksis-app-hjelp = "~3.0"
 aleksis-app-ldap = "~3.0"
 aleksis-app-resint = "~3.0"
```

### Comparing `aleksis-2023.6b1/PKG-INFO` & `aleksis-2023.6b2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aleksis
-Version: 2023.6b1
+Version: 2023.6b2
 Summary: Free School Information System Distribution
 Home-page: https://aleksis.org/
 License: EUPL-1.2-or-later
 Keywords: SIS,education,school,digitisation,school apps
 Author: Dominik George
 Author-email: dominik.george@teckids.org
 Maintainer: Jonathan Weth
@@ -27,15 +27,15 @@
 Requires-Dist: aleksis-app-dashboardfeeds (>=3.0,<3.1)
 Requires-Dist: aleksis-app-hjelp (>=3.0,<3.1)
 Requires-Dist: aleksis-app-ldap (>=3.0,<3.1)
 Requires-Dist: aleksis-app-matrix (>=2.0,<2.1)
 Requires-Dist: aleksis-app-resint (>=3.0,<3.1)
 Requires-Dist: aleksis-app-stoelindeling (>=2.0,<2.1)
 Requires-Dist: aleksis-app-untis (>=3.0,<3.1)
-Requires-Dist: aleksis-core[ldap,s3,sentry] (>=3.0,<3.1)
+Requires-Dist: aleksis-core[ldap,s3,sentry] (>=3.1,<3.2)
 Project-URL: Repository, https://edugit.org/AlekSIS/official/AlekSIS
 Description-Content-Type: text/x-rst
 
 AlekSIS® — All-libre extensible kit for school information systems
 ==================================================================
 
 What AlekSIS® is
```

