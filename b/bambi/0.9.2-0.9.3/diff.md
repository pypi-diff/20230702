# Comparing `tmp/bambi-0.9.2.tar.gz` & `tmp/bambi-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bambi-0.9.2.tar", last modified: Fri Dec  9 15:52:53 2022, max compression
+gzip compressed data, was "bambi-0.9.3.tar", last modified: Wed Dec 21 12:50:43 2022, max compression
```

## Comparing `bambi-0.9.2.tar` & `bambi-0.9.3.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-09 15:52:53.945051 bambi-0.9.2/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2022-12-09 15:52:46.000000 bambi-0.9.2/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     6319 2022-12-09 15:52:46.000000 bambi-0.9.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    13737 2022-12-09 15:52:46.000000 bambi-0.9.2/Changelog.md
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2022-12-09 15:52:46.000000 bambi-0.9.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       19 2022-12-09 15:52:46.000000 bambi-0.9.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5826 2022-12-09 15:52:53.945051 bambi-0.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4542 2022-12-09 15:52:46.000000 bambi-0.9.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-09 15:52:53.941051 bambi-0.9.2/bambi/
--rw-r--r--   0 runner    (1001) docker     (123)      568 2022-12-09 15:52:46.000000 bambi-0.9.2/bambi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-09 15:52:53.941051 bambi-0.9.2/bambi/backend/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2022-12-09 15:52:46.000000 bambi-0.9.2/bambi/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2022-12-09 15:52:46.000000 bambi-0.9.2/bambi/backend/links.py
--rw-r--r--   0 runner    (1001) docker     (123)    22237 2022-12-09 15:52:46.000000 bambi-0.9.2/bambi/backend/pymc.py
--rw-r--r--   0 runner    (1001) docker     (123)     9461 2022-12-09 15:52:46.000000 bambi-0.9.2/bambi/backend/terms.py
--rw-r--r--   0 runner    (1001) docker     (123)      542 2022-12-09 15:52:46.000000 bambi-0.9.2/bambi/backend/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-09 15:52:53.941051 bambi-0.9.2/bambi/data/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2022-12-09 15:52:46.000000 bambi-0.9.2/bambi/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8026 2022-12-09 15:52:46.000000 bambi-0.9.2/bambi/data/datasets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-09 15:52:53.941051 bambi-0.9.2/bambi/defaults/
--rw-r--r--   0 runner    (1001) docker     (123)      175 2022-12-09 15:52:46.000000 bambi-0.9.2/bambi/defaults/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9033 2022-12-09 15:52:46.000000 bambi-0.9.2/bambi/defaults/defaults.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-09 15:52:53.945051 bambi-0.9.2/bambi/families/
--rw-r--r--   0 runner    (1001) docker     (123)      187 2022-12-09 15:52:46.000000 bambi-0.9.2/bambi/families/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2700 2022-12-09 15:52:46.000000 bambi-0.9.2/bambi/families/family.py
--rw-r--r--   0 runner    (1001) docker     (123)     4830 2022-12-09 15:52:46.000000 bambi-0.9.2/bambi/families/likelihood.py
--rw-r--r--   0 runner    (1001) docker     (123)     5284 2022-12-09 15:52:46.000000 bambi-0.9.2/bambi/families/link.py
--rw-r--r--   0 runner    (1001) docker     (123)     8287 2022-12-09 15:52:46.000000 bambi-0.9.2/bambi/families/multivariate.py
--rw-r--r--   0 runner    (1001) docker     (123)     6960 2022-12-09 15:52:46.000000 bambi-0.9.2/bambi/families/univariate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2662 2022-12-09 15:52:46.000000 bambi-0.9.2/bambi/formula.py
--rw-r--r--   0 runner    (1001) docker     (123)    43374 2022-12-09 15:52:46.000000 bambi-0.9.2/bambi/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-09 15:52:53.945051 bambi-0.9.2/bambi/plots/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2022-12-09 15:52:46.000000 bambi-0.9.2/bambi/plots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15786 2022-12-09 15:52:46.000000 bambi-0.9.2/bambi/plots/plot_cap.py
--rw-r--r--   0 runner    (1001) docker     (123)      782 2022-12-09 15:52:46.000000 bambi-0.9.2/bambi/plots/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-09 15:52:53.945051 bambi-0.9.2/bambi/priors/
--rw-r--r--   0 runner    (1001) docker     (123)      187 2022-12-09 15:52:46.000000 bambi-0.9.2/bambi/priors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2022-12-09 15:52:46.000000 bambi-0.9.2/bambi/priors/prior.py
--rw-r--r--   0 runner    (1001) docker     (123)     4019 2022-12-09 15:52:46.000000 bambi-0.9.2/bambi/priors/scaler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-09 15:52:53.945051 bambi-0.9.2/bambi/terms/
--rw-r--r--   0 runner    (1001) docker     (123)      264 2022-12-09 15:52:46.000000 bambi-0.9.2/bambi/terms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1686 2022-12-09 15:52:46.000000 bambi-0.9.2/bambi/terms/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2460 2022-12-09 15:52:46.000000 bambi-0.9.2/bambi/terms/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     3531 2022-12-09 15:52:46.000000 bambi-0.9.2/bambi/terms/group_specific.py
--rw-r--r--   0 runner    (1001) docker     (123)      875 2022-12-09 15:52:46.000000 bambi-0.9.2/bambi/terms/offset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2449 2022-12-09 15:52:46.000000 bambi-0.9.2/bambi/terms/response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2022-12-09 15:52:46.000000 bambi-0.9.2/bambi/terms/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4126 2022-12-09 15:52:46.000000 bambi-0.9.2/bambi/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2022-12-09 15:52:46.000000 bambi-0.9.2/bambi/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-09 15:52:53.941051 bambi-0.9.2/bambi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5826 2022-12-09 15:52:53.000000 bambi-0.9.2/bambi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2022-12-09 15:52:53.000000 bambi-0.9.2/bambi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-09 15:52:53.000000 bambi-0.9.2/bambi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      161 2022-12-09 15:52:53.000000 bambi-0.9.2/bambi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2022-12-09 15:52:53.000000 bambi-0.9.2/bambi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2022-12-09 15:52:46.000000 bambi-0.9.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      231 2022-12-09 15:52:46.000000 bambi-0.9.2/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2022-12-09 15:52:46.000000 bambi-0.9.2/requirements-optional.txt
--rw-r--r--   0 runner    (1001) docker     (123)       97 2022-12-09 15:52:46.000000 bambi-0.9.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2022-12-09 15:52:53.945051 bambi-0.9.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1990 2022-12-09 15:52:46.000000 bambi-0.9.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 12:50:43.367217 bambi-0.9.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2022-12-21 12:50:34.000000 bambi-0.9.3/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6319 2022-12-21 12:50:34.000000 bambi-0.9.3/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    13861 2022-12-21 12:50:34.000000 bambi-0.9.3/Changelog.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2022-12-21 12:50:34.000000 bambi-0.9.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2022-12-21 12:50:34.000000 bambi-0.9.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5826 2022-12-21 12:50:43.367217 bambi-0.9.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4542 2022-12-21 12:50:34.000000 bambi-0.9.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 12:50:43.363216 bambi-0.9.3/bambi/
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2022-12-21 12:50:34.000000 bambi-0.9.3/bambi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 12:50:43.367217 bambi-0.9.3/bambi/backend/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2022-12-21 12:50:34.000000 bambi-0.9.3/bambi/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2022-12-21 12:50:34.000000 bambi-0.9.3/bambi/backend/links.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22276 2022-12-21 12:50:34.000000 bambi-0.9.3/bambi/backend/pymc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9468 2022-12-21 12:50:34.000000 bambi-0.9.3/bambi/backend/terms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2022-12-21 12:50:34.000000 bambi-0.9.3/bambi/backend/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 12:50:43.367217 bambi-0.9.3/bambi/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2022-12-21 12:50:34.000000 bambi-0.9.3/bambi/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8026 2022-12-21 12:50:34.000000 bambi-0.9.3/bambi/data/datasets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 12:50:43.367217 bambi-0.9.3/bambi/defaults/
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2022-12-21 12:50:34.000000 bambi-0.9.3/bambi/defaults/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9033 2022-12-21 12:50:34.000000 bambi-0.9.3/bambi/defaults/defaults.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 12:50:43.367217 bambi-0.9.3/bambi/families/
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2022-12-21 12:50:34.000000 bambi-0.9.3/bambi/families/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2700 2022-12-21 12:50:34.000000 bambi-0.9.3/bambi/families/family.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4830 2022-12-21 12:50:34.000000 bambi-0.9.3/bambi/families/likelihood.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5286 2022-12-21 12:50:34.000000 bambi-0.9.3/bambi/families/link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8289 2022-12-21 12:50:34.000000 bambi-0.9.3/bambi/families/multivariate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6960 2022-12-21 12:50:34.000000 bambi-0.9.3/bambi/families/univariate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2662 2022-12-21 12:50:34.000000 bambi-0.9.3/bambi/formula.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43374 2022-12-21 12:50:34.000000 bambi-0.9.3/bambi/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 12:50:43.367217 bambi-0.9.3/bambi/plots/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2022-12-21 12:50:34.000000 bambi-0.9.3/bambi/plots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15786 2022-12-21 12:50:34.000000 bambi-0.9.3/bambi/plots/plot_cap.py
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2022-12-21 12:50:34.000000 bambi-0.9.3/bambi/plots/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 12:50:43.367217 bambi-0.9.3/bambi/priors/
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2022-12-21 12:50:34.000000 bambi-0.9.3/bambi/priors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2022-12-21 12:50:34.000000 bambi-0.9.3/bambi/priors/prior.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4019 2022-12-21 12:50:34.000000 bambi-0.9.3/bambi/priors/scaler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 12:50:43.367217 bambi-0.9.3/bambi/terms/
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2022-12-21 12:50:34.000000 bambi-0.9.3/bambi/terms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1686 2022-12-21 12:50:34.000000 bambi-0.9.3/bambi/terms/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2460 2022-12-21 12:50:34.000000 bambi-0.9.3/bambi/terms/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3531 2022-12-21 12:50:34.000000 bambi-0.9.3/bambi/terms/group_specific.py
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2022-12-21 12:50:34.000000 bambi-0.9.3/bambi/terms/offset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2449 2022-12-21 12:50:34.000000 bambi-0.9.3/bambi/terms/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2022-12-21 12:50:34.000000 bambi-0.9.3/bambi/terms/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4126 2022-12-21 12:50:34.000000 bambi-0.9.3/bambi/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2022-12-21 12:50:34.000000 bambi-0.9.3/bambi/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-21 12:50:43.367217 bambi-0.9.3/bambi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5826 2022-12-21 12:50:43.000000 bambi-0.9.3/bambi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2022-12-21 12:50:43.000000 bambi-0.9.3/bambi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-21 12:50:43.000000 bambi-0.9.3/bambi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2022-12-21 12:50:43.000000 bambi-0.9.3/bambi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2022-12-21 12:50:43.000000 bambi-0.9.3/bambi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2022-12-21 12:50:35.000000 bambi-0.9.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2022-12-21 12:50:35.000000 bambi-0.9.3/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2022-12-21 12:50:35.000000 bambi-0.9.3/requirements-optional.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2022-12-21 12:50:35.000000 bambi-0.9.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2022-12-21 12:50:43.367217 bambi-0.9.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2022-12-21 12:50:35.000000 bambi-0.9.3/setup.py
```

### Comparing `bambi-0.9.2/CODE_OF_CONDUCT.md` & `bambi-0.9.3/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `bambi-0.9.2/CONTRIBUTING.md` & `bambi-0.9.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `bambi-0.9.2/Changelog.md` & `bambi-0.9.3/Changelog.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,20 @@
 
 ### Maintenance and fixes
 
 ### Documentation
 
 ### Deprecation
 
+## 0.9.3
+
+### Maintenance and fixes
+
+* Update to PyMC >= 5, which means we use PyTensor instead of Aesara now (#613, #614)
+
 ## 0.9.2
 
 ### New features
 
 * Implement `censored()` (#581)
 * Add `Formula` class (#585)
 * Add common numpy transforms to extra_namespace (#589)
```

### Comparing `bambi-0.9.2/LICENSE` & `bambi-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bambi-0.9.2/PKG-INFO` & `bambi-0.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: bambi
-Version: 0.9.2
+Version: 0.9.3
 Summary: BAyesian Model Building Interface in Python
 Home-page: http://github.com/bambinos/bambi
 Maintainer: Tomas Capretto
 Maintainer-email: tomicapretto@gmail.com
 License: MIT
-Download-URL: https://github.com/bambinos/bambi/archive/0.9.2.tar.gz
+Download-URL: https://github.com/bambinos/bambi/archive/0.9.3.tar.gz
 Description: <img src="https://raw.githubusercontent.com/bambinos/bambi/main/docs/logos/RGB/Bambi_logo.png" width=200></img>
         
         [![PyPi version](https://badge.fury.io/py/bambi.svg)](https://badge.fury.io/py/bambi)
         [![Build Status](https://github.com/bambinos/bambi/actions/workflows/test.yml/badge.svg)](https://github.com/bambinos/bambi/actions/workflows/test.yml)
         [![codecov](https://codecov.io/gh/bambinos/bambi/branch/master/graph/badge.svg?token=ZqH0KCLKAE)](https://codecov.io/gh/bambinos/bambi)
         [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
```

### Comparing `bambi-0.9.2/README.md` & `bambi-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `bambi-0.9.2/bambi/__init__.py` & `bambi-0.9.3/bambi/__init__.py`

 * *Files identical despite different names*

### Comparing `bambi-0.9.2/bambi/backend/links.py` & `bambi-0.9.3/bambi/backend/links.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 import numpy as np
-import aesara.tensor as at
+import pytensor.tensor as pt
 
 
 def probit(x):
     """Probit function that ensures result is in (0, 1)"""
     eps = np.finfo(float).eps
-    result = 0.5 + 0.5 * at.erf(x / at.sqrt(2))
-    result = at.switch(at.eq(result, 0), eps, result)
-    result = at.switch(at.eq(result, 1), 1 - eps, result)
+    result = 0.5 + 0.5 * pt.erf(x / pt.sqrt(2))
+    result = pt.switch(pt.eq(result, 0), eps, result)
+    result = pt.switch(pt.eq(result, 1), 1 - eps, result)
 
     return result
 
 
 def cloglog(x):
     """Cloglog function that ensures result is in (0, 1)"""
     eps = np.finfo(float).eps
-    result = 1 - at.exp(-at.exp(x))
-    result = at.switch(at.eq(result, 0), eps, result)
-    result = at.switch(at.eq(result, 1), 1 - eps, result)
+    result = 1 - pt.exp(-pt.exp(x))
+    result = pt.switch(pt.eq(result, 0), eps, result)
+    result = pt.switch(pt.eq(result, 1), 1 - eps, result)
 
     return result
 
 
 def logit(x):
     """Logit function that ensures result is in (0, 1)"""
     eps = np.finfo(float).eps
-    result = at.sigmoid(x)
-    result = at.switch(at.eq(result, 0), eps, result)
-    result = at.switch(at.eq(result, 1), 1 - eps, result)
+    result = pt.sigmoid(x)
+    result = pt.switch(pt.eq(result, 0), eps, result)
+    result = pt.switch(pt.eq(result, 1), 1 - eps, result)
     return result
 
 
 def identity(x):
     return x
 
 
 def inverse_squared(x):
-    return at.reciprocal(at.sqrt(x))
+    return pt.reciprocal(pt.sqrt(x))
 
 
 def arctan_2(x):
-    return 2 * at.arctan(x)
+    return 2 * pt.arctan(x)
```

### Comparing `bambi-0.9.2/bambi/backend/pymc.py` & `bambi-0.9.3/bambi/backend/pymc.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,17 @@
 import traceback
 
 from copy import deepcopy
 
 import numpy as np
 import pymc as pm
 
-import aesara.tensor as at
+import pytensor.tensor as pt
+from pytensor.tensor.special import softmax
+
 
 from bambi import version
 
 from bambi.backend.links import cloglog, identity, inverse_squared, logit, probit, arctan_2
 from bambi.backend.terms import CommonTerm, GroupSpecificTerm, InterceptTerm, ResponseTerm
 from bambi.families.multivariate import MultivariateFamily
 
@@ -21,20 +23,20 @@
 class PyMCModel:
     """PyMC model-fitting backend."""
 
     INVLINKS = {
         "cloglog": cloglog,
         "identity": identity,
         "inverse_squared": inverse_squared,
-        "inverse": at.reciprocal,
-        "log": at.exp,
+        "inverse": pt.reciprocal,
+        "log": pt.exp,
         "logit": logit,
         "probit": probit,
         "tan_2": arctan_2,
-        "softmax": functools.partial(at.nnet.softmax, axis=-1),
+        "softmax": functools.partial(softmax, axis=-1),
     }
 
     def __init__(self):
         self.name = pm.__name__
         self.version = pm.__version__
 
         # Attributes defined elsewhere
@@ -155,27 +157,27 @@
 
                 # Build
                 coef, data = common_term.build(spec)
                 coefs.append(coef)
                 columns.append(data)
 
             # Column vector of coefficients and design matrix
-            coefs = at.concatenate(coefs)
+            coefs = pt.concatenate(coefs)
 
             # Design matrix
             data = np.column_stack(columns)
 
             # If there's an intercept, center the data
             # Also store the design matrix without the intercept to uncenter the intercept later
             if self.has_intercept:
                 self._design_matrix_without_intercept = data
                 data = data - data.mean(0)
 
             # Add term to linear predictor
-            self.mu += at.dot(data, coefs)
+            self.mu += pt.dot(data, coefs)
 
     def _build_group_specific_terms(self, spec):
         """Add group-specific (random or varying) terms to the PyMC model.
 
         We have linear predictors of the form 'X @ b + Z @ u'.
         This creates the 'u' parameter vector in PyMC, computes `Z @ u`, and adds it to ``self.mu``.
 
@@ -572,15 +574,15 @@
         eta=eta,
         sd_dist=sigma,
         compute_corr=True,
         store_in_trace=False,
     )
 
     coefs_offset = pm.Normal("_LKJ_" + grouper + "_offset", mu=0, sigma=1, shape=(rows, cols))
-    coefs = at.dot(lkj_decomp, coefs_offset).T
+    coefs = pt.dot(lkj_decomp, coefs_offset).T
 
     ## Separate group-specific terms
     start = 0
     for term in terms:
         label = term.name
         dims = list(term.coords)
```

### Comparing `bambi-0.9.2/bambi/backend/terms.py` & `bambi-0.9.3/bambi/backend/terms.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import numpy as np
 import pymc as pm
-import aesara.tensor as at
+
+import pytensor.tensor as pt
 
 from bambi.backend.utils import has_hyperprior, get_distribution
 from bambi.families.multivariate import MultivariateFamily
 from bambi.priors import Prior
 
 
 class CommonTerm:
@@ -53,15 +54,15 @@
             if data.ndim == 1:
                 shape = None
             elif data.shape[1] == 1:
                 shape = None
             else:
                 shape = data.shape[1]
             coef = distribution(label, shape=shape, **args)
-            coef = at.atleast_1d(coef)  # If only a single numeric column it won't be 1D
+            coef = pt.atleast_1d(coef)  # If only a single numeric column it won't be 1D
 
         # Prepends one dimension if response is multivariate and the predictor is 1D
         if response_dims and len(dims) == 1:
             coef = coef[np.newaxis, :]
 
         return coef, data
 
@@ -200,19 +201,19 @@
     def __init__(self, term, family):
         self.term = term
         self.family = family
 
     def build(self, nu, invlinks):
         """Create and return the response distribution for the PyMC model.
 
-        nu : aesara.tensor.var.TensorVariable
+        nu : pytensor.tensor.var.TensorVariable
             The linear predictor in the PyMC model.
         invlinks : dict
             A dictionary where names are names of inverse link functions and values are functions
-            that can operate with Aesara tensors.
+            that can operate with PyTensor tensors.
         """
         data = np.squeeze(self.term.data)
 
         # Take the inverse link function that maps from linear predictor to the mean of likelihood
         if self.family.link.name in invlinks:
             linkinv = invlinks[self.family.link.name]
         else:
```

### Comparing `bambi-0.9.2/bambi/data/datasets.py` & `bambi-0.9.3/bambi/data/datasets.py`

 * *Files identical despite different names*

### Comparing `bambi-0.9.2/bambi/defaults/defaults.py` & `bambi-0.9.3/bambi/defaults/defaults.py`

 * *Files identical despite different names*

### Comparing `bambi-0.9.2/bambi/families/family.py` & `bambi-0.9.3/bambi/families/family.py`

 * *Files identical despite different names*

### Comparing `bambi-0.9.2/bambi/families/likelihood.py` & `bambi-0.9.3/bambi/families/likelihood.py`

 * *Files identical despite different names*

### Comparing `bambi-0.9.2/bambi/families/link.py` & `bambi-0.9.3/bambi/families/link.py`

 * *Files 0% similar despite different names*

```diff
@@ -135,15 +135,15 @@
         A function that maps the response to the linear predictor. Known as the :math:`g` function
         in GLM jargon. Does not need to be specified when ``name`` is a known name.
     linkinv: function
         A function that maps the linear predictor to the response. Known as the :math:`g^{-1}`
         function in GLM jargon. Does not need to be specified when ``name`` is a known name.
     linkinv_backend: function
         Same than ``linkinv`` but must be something that works with PyMC backend (i.e. it must
-        work with Aesara tensors). Does not need to be specified when ``name`` is a known
+        work with PyTensor tensors). Does not need to be specified when ``name`` is a known
         name.
     """
 
     def __init__(self, name, link=None, linkinv=None, linkinv_backend=None):
         self.name = name
         self.link = link
         self.linkinv = linkinv
```

### Comparing `bambi-0.9.2/bambi/families/multivariate.py` & `bambi-0.9.3/bambi/families/multivariate.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # pylint: disable=unused-argument
-import aesara.tensor as at
+import pytensor.tensor as pt
 import numpy as np
 import xarray as xr
 
 from bambi.families.family import Family
 from bambi.utils import extract_argument_names, extra_namespace
 
 
@@ -102,15 +102,15 @@
     @staticmethod
     def transform_backend_nu(nu, data):
         # Add column of zeros to the linear predictor for the reference level (the first one)
         shape = (data.shape[0], 1)
 
         # The first line makes sure the intercept-only models work
         nu = np.ones(shape) * nu  # (response_levels, ) -> (n, response_levels)
-        nu = at.concatenate([np.zeros(shape), nu], axis=1)
+        nu = pt.concatenate([np.zeros(shape), nu], axis=1)
         return nu
 
 
 class Multinomial(MultivariateFamily):
     SUPPORTED_LINKS = ["softmax"]
 
     def predict(self, model, posterior, linear_predictor):
@@ -194,15 +194,15 @@
     @staticmethod
     def transform_backend_nu(nu, data):
         # Add column of zeros to the linear predictor for the reference level (the first one)
         shape = (data.shape[0], 1)
 
         # The first line makes sure the intercept-only models work
         nu = np.ones(shape) * nu  # (response_levels, ) -> (n, response_levels)
-        nu = at.concatenate([np.zeros(shape), nu], axis=1)
+        nu = pt.concatenate([np.zeros(shape), nu], axis=1)
         return nu
 
 
 # pylint: disable = protected-access
 def get_reference_level(term):
     if term.kind != "categoric":
         return None
```

### Comparing `bambi-0.9.2/bambi/families/univariate.py` & `bambi-0.9.3/bambi/families/univariate.py`

 * *Files identical despite different names*

### Comparing `bambi-0.9.2/bambi/formula.py` & `bambi-0.9.3/bambi/formula.py`

 * *Files identical despite different names*

### Comparing `bambi-0.9.2/bambi/models.py` & `bambi-0.9.3/bambi/models.py`

 * *Files identical despite different names*

### Comparing `bambi-0.9.2/bambi/plots/plot_cap.py` & `bambi-0.9.3/bambi/plots/plot_cap.py`

 * *Files identical despite different names*

### Comparing `bambi-0.9.2/bambi/plots/utils.py` & `bambi-0.9.3/bambi/plots/utils.py`

 * *Files identical despite different names*

### Comparing `bambi-0.9.2/bambi/priors/prior.py` & `bambi-0.9.3/bambi/priors/prior.py`

 * *Files identical despite different names*

### Comparing `bambi-0.9.2/bambi/priors/scaler.py` & `bambi-0.9.3/bambi/priors/scaler.py`

 * *Files identical despite different names*

### Comparing `bambi-0.9.2/bambi/terms/base.py` & `bambi-0.9.3/bambi/terms/base.py`

 * *Files identical despite different names*

### Comparing `bambi-0.9.2/bambi/terms/common.py` & `bambi-0.9.3/bambi/terms/common.py`

 * *Files identical despite different names*

### Comparing `bambi-0.9.2/bambi/terms/group_specific.py` & `bambi-0.9.3/bambi/terms/group_specific.py`

 * *Files identical despite different names*

### Comparing `bambi-0.9.2/bambi/terms/offset.py` & `bambi-0.9.3/bambi/terms/offset.py`

 * *Files identical despite different names*

### Comparing `bambi-0.9.2/bambi/terms/response.py` & `bambi-0.9.3/bambi/terms/response.py`

 * *Files identical despite different names*

### Comparing `bambi-0.9.2/bambi/terms/utils.py` & `bambi-0.9.3/bambi/terms/utils.py`

 * *Files identical despite different names*

### Comparing `bambi-0.9.2/bambi/utils.py` & `bambi-0.9.3/bambi/utils.py`

 * *Files identical despite different names*

### Comparing `bambi-0.9.2/bambi.egg-info/PKG-INFO` & `bambi-0.9.3/bambi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: bambi
-Version: 0.9.2
+Version: 0.9.3
 Summary: BAyesian Model Building Interface in Python
 Home-page: http://github.com/bambinos/bambi
 Maintainer: Tomas Capretto
 Maintainer-email: tomicapretto@gmail.com
 License: MIT
-Download-URL: https://github.com/bambinos/bambi/archive/0.9.2.tar.gz
+Download-URL: https://github.com/bambinos/bambi/archive/0.9.3.tar.gz
 Description: <img src="https://raw.githubusercontent.com/bambinos/bambi/main/docs/logos/RGB/Bambi_logo.png" width=200></img>
         
         [![PyPi version](https://badge.fury.io/py/bambi.svg)](https://badge.fury.io/py/bambi)
         [![Build Status](https://github.com/bambinos/bambi/actions/workflows/test.yml/badge.svg)](https://github.com/bambinos/bambi/actions/workflows/test.yml)
         [![codecov](https://codecov.io/gh/bambinos/bambi/branch/master/graph/badge.svg?token=ZqH0KCLKAE)](https://codecov.io/gh/bambinos/bambi)
         [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
```

### Comparing `bambi-0.9.2/bambi.egg-info/SOURCES.txt` & `bambi-0.9.3/bambi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bambi-0.9.2/setup.py` & `bambi-0.9.3/setup.py`

 * *Files identical despite different names*

