# Comparing `tmp/PSNAWP-1.2.3.tar.gz` & `tmp/PSNAWP-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PSNAWP-1.2.3.tar", last modified: Sat Apr  8 21:27:22 2023, max compression
+gzip compressed data, was "PSNAWP-1.3.0.tar", last modified: Sun Jul  2 05:18:28 2023, max compression
```

## Comparing `PSNAWP-1.2.3.tar` & `PSNAWP-1.3.0.tar`

### file list

```diff
@@ -1,47 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 21:27:22.072305 PSNAWP-1.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)     5036 2023-04-08 21:27:12.000000 PSNAWP-1.2.3/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-04-08 21:27:12.000000 PSNAWP-1.2.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    13300 2023-04-08 21:27:22.072305 PSNAWP-1.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12200 2023-04-08 21:27:12.000000 PSNAWP-1.2.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-08 21:27:12.000000 PSNAWP-1.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-08 21:27:12.000000 PSNAWP-1.2.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4498 2023-04-08 21:27:12.000000 PSNAWP-1.2.3/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-04-08 21:27:22.072305 PSNAWP-1.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-08 21:27:12.000000 PSNAWP-1.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 21:27:22.068305 PSNAWP-1.2.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 21:27:22.068305 PSNAWP-1.2.3/src/PSNAWP.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13300 2023-04-08 21:27:22.000000 PSNAWP-1.2.3/src/PSNAWP.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-04-08 21:27:22.000000 PSNAWP-1.2.3/src/PSNAWP.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 21:27:22.000000 PSNAWP-1.2.3/src/PSNAWP.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 21:27:22.000000 PSNAWP-1.2.3/src/PSNAWP.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-04-08 21:27:22.000000 PSNAWP-1.2.3/src/PSNAWP.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-08 21:27:22.000000 PSNAWP-1.2.3/src/PSNAWP.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 21:27:22.072305 PSNAWP-1.2.3/src/psnawp_api/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-08 21:27:12.000000 PSNAWP-1.2.3/src/psnawp_api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 21:27:22.072305 PSNAWP-1.2.3/src/psnawp_api/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 21:27:12.000000 PSNAWP-1.2.3/src/psnawp_api/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5015 2023-04-08 21:27:12.000000 PSNAWP-1.2.3/src/psnawp_api/core/authenticator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-04-08 21:27:12.000000 PSNAWP-1.2.3/src/psnawp_api/core/psnawp_exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 21:27:22.072305 PSNAWP-1.2.3/src/psnawp_api/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 21:27:12.000000 PSNAWP-1.2.3/src/psnawp_api/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14995 2023-04-08 21:27:12.000000 PSNAWP-1.2.3/src/psnawp_api/models/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5124 2023-04-08 21:27:12.000000 PSNAWP-1.2.3/src/psnawp_api/models/game_title.py
--rw-r--r--   0 runner    (1001) docker     (123)     7388 2023-04-08 21:27:12.000000 PSNAWP-1.2.3/src/psnawp_api/models/group.py
--rw-r--r--   0 runner    (1001) docker     (123)     5165 2023-04-08 21:27:12.000000 PSNAWP-1.2.3/src/psnawp_api/models/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     3843 2023-04-08 21:27:12.000000 PSNAWP-1.2.3/src/psnawp_api/models/title_stats.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 21:27:22.072305 PSNAWP-1.2.3/src/psnawp_api/models/trophies/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 21:27:12.000000 PSNAWP-1.2.3/src/psnawp_api/models/trophies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12474 2023-04-08 21:27:12.000000 PSNAWP-1.2.3/src/psnawp_api/models/trophies/trophy.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-08 21:27:12.000000 PSNAWP-1.2.3/src/psnawp_api/models/trophies/trophy_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    10398 2023-04-08 21:27:12.000000 PSNAWP-1.2.3/src/psnawp_api/models/trophies/trophy_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-04-08 21:27:12.000000 PSNAWP-1.2.3/src/psnawp_api/models/trophies/trophy_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)    10573 2023-04-08 21:27:12.000000 PSNAWP-1.2.3/src/psnawp_api/models/trophies/trophy_titles.py
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-08 21:27:12.000000 PSNAWP-1.2.3/src/psnawp_api/models/trophies/utility_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    14869 2023-04-08 21:27:12.000000 PSNAWP-1.2.3/src/psnawp_api/models/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     6680 2023-04-08 21:27:12.000000 PSNAWP-1.2.3/src/psnawp_api/psnawp.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 21:27:12.000000 PSNAWP-1.2.3/src/psnawp_api/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 21:27:22.072305 PSNAWP-1.2.3/src/psnawp_api/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 21:27:12.000000 PSNAWP-1.2.3/src/psnawp_api/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-04-08 21:27:12.000000 PSNAWP-1.2.3/src/psnawp_api/utils/endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-04-08 21:27:12.000000 PSNAWP-1.2.3/src/psnawp_api/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6106 2023-04-08 21:27:12.000000 PSNAWP-1.2.3/src/psnawp_api/utils/request_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 05:18:28.182672 PSNAWP-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     5036 2023-07-02 05:18:19.000000 PSNAWP-1.3.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-07-02 05:18:19.000000 PSNAWP-1.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    14436 2023-07-02 05:18:28.182672 PSNAWP-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13336 2023-07-02 05:18:19.000000 PSNAWP-1.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-07-02 05:18:19.000000 PSNAWP-1.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-07-02 05:18:19.000000 PSNAWP-1.3.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4498 2023-07-02 05:18:19.000000 PSNAWP-1.3.0/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-07-02 05:18:28.182672 PSNAWP-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-02 05:18:19.000000 PSNAWP-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 05:18:28.178672 PSNAWP-1.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 05:18:28.178672 PSNAWP-1.3.0/src/PSNAWP.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14436 2023-07-02 05:18:28.000000 PSNAWP-1.3.0/src/PSNAWP.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-07-02 05:18:28.000000 PSNAWP-1.3.0/src/PSNAWP.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 05:18:28.000000 PSNAWP-1.3.0/src/PSNAWP.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 05:18:28.000000 PSNAWP-1.3.0/src/PSNAWP.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-07-02 05:18:28.000000 PSNAWP-1.3.0/src/PSNAWP.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-02 05:18:28.000000 PSNAWP-1.3.0/src/PSNAWP.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 05:18:28.182672 PSNAWP-1.3.0/src/psnawp_api/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-02 05:18:19.000000 PSNAWP-1.3.0/src/psnawp_api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 05:18:28.182672 PSNAWP-1.3.0/src/psnawp_api/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 05:18:19.000000 PSNAWP-1.3.0/src/psnawp_api/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5015 2023-07-02 05:18:19.000000 PSNAWP-1.3.0/src/psnawp_api/core/authenticator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-07-02 05:18:19.000000 PSNAWP-1.3.0/src/psnawp_api/core/psnawp_exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 05:18:28.182672 PSNAWP-1.3.0/src/psnawp_api/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 05:18:19.000000 PSNAWP-1.3.0/src/psnawp_api/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15438 2023-07-02 05:18:19.000000 PSNAWP-1.3.0/src/psnawp_api/models/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5124 2023-07-02 05:18:19.000000 PSNAWP-1.3.0/src/psnawp_api/models/game_title.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7388 2023-07-02 05:18:19.000000 PSNAWP-1.3.0/src/psnawp_api/models/group.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 05:18:28.182672 PSNAWP-1.3.0/src/psnawp_api/models/listing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 05:18:19.000000 PSNAWP-1.3.0/src/psnawp_api/models/listing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-07-02 05:18:19.000000 PSNAWP-1.3.0/src/psnawp_api/models/listing/listing_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-07-02 05:18:19.000000 PSNAWP-1.3.0/src/psnawp_api/models/listing/pagination_arguments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5165 2023-07-02 05:18:19.000000 PSNAWP-1.3.0/src/psnawp_api/models/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5977 2023-07-02 05:18:19.000000 PSNAWP-1.3.0/src/psnawp_api/models/title_stats.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 05:18:28.182672 PSNAWP-1.3.0/src/psnawp_api/models/trophies/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 05:18:19.000000 PSNAWP-1.3.0/src/psnawp_api/models/trophies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12474 2023-07-02 05:18:19.000000 PSNAWP-1.3.0/src/psnawp_api/models/trophies/trophy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-07-02 05:18:19.000000 PSNAWP-1.3.0/src/psnawp_api/models/trophies/trophy_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10386 2023-07-02 05:18:19.000000 PSNAWP-1.3.0/src/psnawp_api/models/trophies/trophy_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-07-02 05:18:19.000000 PSNAWP-1.3.0/src/psnawp_api/models/trophies/trophy_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10573 2023-07-02 05:18:19.000000 PSNAWP-1.3.0/src/psnawp_api/models/trophies/trophy_titles.py
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-02 05:18:19.000000 PSNAWP-1.3.0/src/psnawp_api/models/trophies/utility_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15316 2023-07-02 05:18:19.000000 PSNAWP-1.3.0/src/psnawp_api/models/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6680 2023-07-02 05:18:19.000000 PSNAWP-1.3.0/src/psnawp_api/psnawp.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 05:18:19.000000 PSNAWP-1.3.0/src/psnawp_api/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 05:18:28.182672 PSNAWP-1.3.0/src/psnawp_api/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 05:18:19.000000 PSNAWP-1.3.0/src/psnawp_api/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-07-02 05:18:19.000000 PSNAWP-1.3.0/src/psnawp_api/utils/endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-07-02 05:18:19.000000 PSNAWP-1.3.0/src/psnawp_api/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6106 2023-07-02 05:18:19.000000 PSNAWP-1.3.0/src/psnawp_api/utils/request_builder.py
```

### Comparing `PSNAWP-1.2.3/LICENSE.md` & `PSNAWP-1.3.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `PSNAWP-1.2.3/PKG-INFO` & `PSNAWP-1.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PSNAWP
-Version: 1.2.3
+Version: 1.3.0
 Summary: Python API Wrapper for PlayStation Network API
 Home-page: https://github.com/isFakeAccount/psnawp
 Author: Yoshikage Kira (@isFakeAccount)
 Author-email: trevorphillips@gmx.us
 License: MIT
 Project-URL: Bug Tracker, https://github.com/isFakeAccount/psnawp/issues
 Project-URL: Changelog, https://github.com/isFakeAccount/psnawp/blob/master/CHANGELOG.md
@@ -38,15 +38,15 @@
 [![pytest](https://github.com/isFakeAccount/psnawp/actions/workflows/pytest.yaml/badge.svg)](https://github.com/isFakeAccount/psnawp/actions/workflows/pytest.yaml)
 [![pre-commit](https://github.com/isFakeAccount/psnawp/actions/workflows/pre-commit.yaml/badge.svg)](https://github.com/isFakeAccount/psnawp/actions/workflows/pre-commit.yaml)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Documentation Status](https://readthedocs.org/projects/psnawp/badge/?version=latest)](https://psnawp.readthedocs.io/en/latest/?badge=latest)
 [![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
 
 <!-- Pytest Coverage Comment:Begin -->
-<a href="https://github.com/isFakeAccount/psnawp/blob/main/README.md"><img alt="Coverage" src="https://img.shields.io/badge/Coverage-98%25-brightgreen.svg" /></a><details><summary>Coverage Report </summary><table><tr><th>File</th><th>Stmts</th><th>Miss</th><th>Cover</th><th>Missing</th></tr><tbody><tr><td colspan="5"><b>/opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/psnawp_api</b></td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/psnawp_api/__init__.py">__init__.py</a></td><td>1</td><td>0</td><td>100%</td><td>&nbsp;</td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/psnawp_api/psnawp.py">psnawp.py</a></td><td>35</td><td>0</td><td>100%</td><td>&nbsp;</td></tr><tr><td colspan="5"><b>/opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/psnawp_api/core</b></td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/psnawp_api/core/__init__.py">__init__.py</a></td><td>0</td><td>0</td><td>100%</td><td>&nbsp;</td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/psnawp_api/core/authenticator.py">authenticator.py</a></td><td>46</td><td>3</td><td>3</td><td><a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/psnawp_api/core/authenticator.py#L 93%"> 93%</a></td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/psnawp_api/core/psnawp_exceptions.py">psnawp_exceptions.py</a></td><td>9</td><td>0</td><td>100%</td><td>&nbsp;</td></tr><tr><td colspan="5"><b>/opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/psnawp_api/models</b></td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/psnawp_api/models/__init__.py">__init__.py</a></td><td>0</td><td>0</td><td>100%</td><td>&nbsp;</td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/psnawp_api/models/client.py">client.py</a></td><td>68</td><td>0</td><td>100%</td><td>&nbsp;</td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/psnawp_api/models/game_title.py">game_title.py</a></td><td>22</td><td>0</td><td>100%</td><td>&nbsp;</td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/psnawp_api/models/group.py">group.py</a></td><td>52</td><td>0</td><td>100%</td><td>&nbsp;</td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/psnawp_api/models/search.py">search.py</a></td><td>22</td><td>0</td><td>100%</td><td>&nbsp;</td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/psnawp_api/models/title_stats.py">title_stats.py</a></td><td>64</td><td>2</td><td>2</td><td><a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/psnawp_api/models/title_stats.py#L 97%"> 97%</a></td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/psnawp_api/models/user.py">user.py</a></td><td>69</td><td>0</td><td>100%</td><td>&nbsp;</td></tr><tr><td colspan="5"><b>/opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/psnawp_api/models/trophies</b></td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/psnawp_api/models/trophies/__init__.py">__init__.py</a></td><td>0</td><td>0</td><td>100%</td><td>&nbsp;</td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/psnawp_api/models/trophies/trophy.py">trophy.py</a></td><td>112</td><td>0</td><td>100%</td><td>&nbsp;</td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/psnawp_api/models/trophies/trophy_constants.py">trophy_constants.py</a></td><td>25</td><td>0</td><td>100%</td><td>&nbsp;</td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/psnawp_api/models/trophies/trophy_group.py">trophy_group.py</a></td><td>89</td><td>0</td><td>100%</td><td>&nbsp;</td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/psnawp_api/models/trophies/trophy_summary.py">trophy_summary.py</a></td><td>25</td><td>0</td><td>100%</td><td>&nbsp;</td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/psnawp_api/models/trophies/trophy_titles.py">trophy_titles.py</a></td><td>86</td><td>0</td><td>100%</td><td>&nbsp;</td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/psnawp_api/models/trophies/utility_functions.py">utility_functions.py</a></td><td>7</td><td>0</td><td>100%</td><td>&nbsp;</td></tr><tr><td colspan="5"><b>/opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/psnawp_api/utils</b></td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/psnawp_api/utils/__init__.py">__init__.py</a></td><td>0</td><td>0</td><td>100%</td><td>&nbsp;</td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/psnawp_api/utils/endpoints.py">endpoints.py</a></td><td>2</td><td>0</td><td>100%</td><td>&nbsp;</td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/psnawp_api/utils/misc.py">misc.py</a></td><td>35</td><td>0</td><td>100%</td><td>&nbsp;</td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/psnawp_api/utils/request_builder.py">request_builder.py</a></td><td>72</td><td>15</td><td>15</td><td><a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/psnawp_api/utils/request_builder.py#L 79%"> 79%</a></td></tr><tr><td><b>TOTAL</b></td><td><b>841</b></td><td><b>20</b></td><td><b>98%</b></td><td>&nbsp;</td></tr></tbody></table></details>
+<a href="https://github.com/isFakeAccount/psnawp/blob/main/README.md"><img alt="Coverage" src="https://img.shields.io/badge/Coverage-95%25-brightgreen.svg" /></a><details><summary>Coverage Report </summary><table><tr><th>File</th><th>Stmts</th><th>Miss</th><th>Cover</th><th>Missing</th></tr><tbody><tr><td colspan="5"><b>/opt/hostedtoolcache/Python/3.11.4/x64/lib/python3.11/site-packages/psnawp_api</b></td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.4/x64/lib/python3.11/site-packages/psnawp_api/__init__.py">__init__.py</a></td><td>1</td><td>0</td><td>100%</td><td>&nbsp;</td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.4/x64/lib/python3.11/site-packages/psnawp_api/psnawp.py">psnawp.py</a></td><td>35</td><td>0</td><td>100%</td><td>&nbsp;</td></tr><tr><td colspan="5"><b>/opt/hostedtoolcache/Python/3.11.4/x64/lib/python3.11/site-packages/psnawp_api/core</b></td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.4/x64/lib/python3.11/site-packages/psnawp_api/core/__init__.py">__init__.py</a></td><td>0</td><td>0</td><td>100%</td><td>&nbsp;</td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.4/x64/lib/python3.11/site-packages/psnawp_api/core/authenticator.py">authenticator.py</a></td><td>46</td><td>3</td><td>3</td><td><a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.4/x64/lib/python3.11/site-packages/psnawp_api/core/authenticator.py#L 93%"> 93%</a></td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.4/x64/lib/python3.11/site-packages/psnawp_api/core/psnawp_exceptions.py">psnawp_exceptions.py</a></td><td>9</td><td>0</td><td>100%</td><td>&nbsp;</td></tr><tr><td colspan="5"><b>/opt/hostedtoolcache/Python/3.11.4/x64/lib/python3.11/site-packages/psnawp_api/models</b></td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.4/x64/lib/python3.11/site-packages/psnawp_api/models/__init__.py">__init__.py</a></td><td>0</td><td>0</td><td>100%</td><td>&nbsp;</td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.4/x64/lib/python3.11/site-packages/psnawp_api/models/client.py">client.py</a></td><td>70</td><td>0</td><td>100%</td><td>&nbsp;</td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.4/x64/lib/python3.11/site-packages/psnawp_api/models/game_title.py">game_title.py</a></td><td>22</td><td>0</td><td>100%</td><td>&nbsp;</td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.4/x64/lib/python3.11/site-packages/psnawp_api/models/group.py">group.py</a></td><td>52</td><td>0</td><td>100%</td><td>&nbsp;</td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.4/x64/lib/python3.11/site-packages/psnawp_api/models/search.py">search.py</a></td><td>22</td><td>0</td><td>100%</td><td>&nbsp;</td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.4/x64/lib/python3.11/site-packages/psnawp_api/models/title_stats.py">title_stats.py</a></td><td>84</td><td>23</td><td>23</td><td><a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.4/x64/lib/python3.11/site-packages/psnawp_api/models/title_stats.py#L 73%"> 73%</a></td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.4/x64/lib/python3.11/site-packages/psnawp_api/models/user.py">user.py</a></td><td>71</td><td>0</td><td>100%</td><td>&nbsp;</td></tr><tr><td colspan="5"><b>/opt/hostedtoolcache/Python/3.11.4/x64/lib/python3.11/site-packages/psnawp_api/models/listing</b></td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.4/x64/lib/python3.11/site-packages/psnawp_api/models/listing/__init__.py">__init__.py</a></td><td>0</td><td>0</td><td>100%</td><td>&nbsp;</td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.4/x64/lib/python3.11/site-packages/psnawp_api/models/listing/listing_generator.py">listing_generator.py</a></td><td>36</td><td>5</td><td>5</td><td><a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.4/x64/lib/python3.11/site-packages/psnawp_api/models/listing/listing_generator.py#L 86%"> 86%</a></td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.4/x64/lib/python3.11/site-packages/psnawp_api/models/listing/pagination_arguments.py">pagination_arguments.py</a></td><td>15</td><td>0</td><td>100%</td><td>&nbsp;</td></tr><tr><td colspan="5"><b>/opt/hostedtoolcache/Python/3.11.4/x64/lib/python3.11/site-packages/psnawp_api/models/trophies</b></td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.4/x64/lib/python3.11/site-packages/psnawp_api/models/trophies/__init__.py">__init__.py</a></td><td>0</td><td>0</td><td>100%</td><td>&nbsp;</td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.4/x64/lib/python3.11/site-packages/psnawp_api/models/trophies/trophy.py">trophy.py</a></td><td>112</td><td>0</td><td>100%</td><td>&nbsp;</td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.4/x64/lib/python3.11/site-packages/psnawp_api/models/trophies/trophy_constants.py">trophy_constants.py</a></td><td>25</td><td>0</td><td>100%</td><td>&nbsp;</td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.4/x64/lib/python3.11/site-packages/psnawp_api/models/trophies/trophy_group.py">trophy_group.py</a></td><td>89</td><td>0</td><td>100%</td><td>&nbsp;</td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.4/x64/lib/python3.11/site-packages/psnawp_api/models/trophies/trophy_summary.py">trophy_summary.py</a></td><td>25</td><td>0</td><td>100%</td><td>&nbsp;</td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.4/x64/lib/python3.11/site-packages/psnawp_api/models/trophies/trophy_titles.py">trophy_titles.py</a></td><td>86</td><td>0</td><td>100%</td><td>&nbsp;</td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.4/x64/lib/python3.11/site-packages/psnawp_api/models/trophies/utility_functions.py">utility_functions.py</a></td><td>7</td><td>0</td><td>100%</td><td>&nbsp;</td></tr><tr><td colspan="5"><b>/opt/hostedtoolcache/Python/3.11.4/x64/lib/python3.11/site-packages/psnawp_api/utils</b></td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.4/x64/lib/python3.11/site-packages/psnawp_api/utils/__init__.py">__init__.py</a></td><td>0</td><td>0</td><td>100%</td><td>&nbsp;</td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.4/x64/lib/python3.11/site-packages/psnawp_api/utils/endpoints.py">endpoints.py</a></td><td>2</td><td>0</td><td>100%</td><td>&nbsp;</td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.4/x64/lib/python3.11/site-packages/psnawp_api/utils/misc.py">misc.py</a></td><td>35</td><td>0</td><td>100%</td><td>&nbsp;</td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.4/x64/lib/python3.11/site-packages/psnawp_api/utils/request_builder.py">request_builder.py</a></td><td>72</td><td>15</td><td>15</td><td><a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.4/x64/lib/python3.11/site-packages/psnawp_api/utils/request_builder.py#L 79%"> 79%</a></td></tr><tr><td><b>TOTAL</b></td><td><b>916</b></td><td><b>46</b></td><td><b>95%</b></td><td>&nbsp;</td></tr></tbody></table></details>
 <!-- Pytest Coverage Comment:End -->
 
 ## How to install
 
 ### From PyPI
 
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: PSNAWP Version: 1.2.3 Summary: Python API Wrapper
+Metadata-Version: 2.1 Name: PSNAWP Version: 1.3.0 Summary: Python API Wrapper
 for PlayStation Network API Home-page: https://github.com/isFakeAccount/psnawp
 Author: Yoshikage Kira (@isFakeAccount) Author-email: trevorphillips@gmx.us
 License: MIT Project-URL: Bug Tracker, https://github.com/isFakeAccount/psnawp/
 issues Project-URL: Changelog, https://github.com/isFakeAccount/psnawp/blob/
 master/CHANGELOG.md Project-URL: Source Code, https://github.com/isFakeAccount/
 psnawp Project-URL: Documentation, https://psnawp.readthedocs.io/en/latest/
 Keywords: PSN API Platform: any Classifier: Development Status :: 4 - Beta
@@ -25,49 +25,54 @@
 psnawp/actions/workflows/pre-commit.yaml/badge.svg)](https://github.com/
 isFakeAccount/psnawp/actions/workflows/pre-commit.yaml) [![Code style: black]
 (https://img.shields.io/badge/code%20style-black-000000.svg)](https://
 github.com/psf/black) [![Documentation Status](https://readthedocs.org/
 projects/psnawp/badge/?version=latest)](https://psnawp.readthedocs.io/en/
 latest/?badge=latest) [![License: MIT](https://img.shields.io/badge/License-
 MIT-blue.svg)](https://opensource.org/licenses/MIT)  [Coverage]Coverage Report
-File                    Stmts Miss Cover Missing
-/opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/
+File                       Stmts Miss Cover Missing
+/opt/hostedtoolcache/Python/3.11.4/x64/lib/python3.11/site-packages/
 psnawp_api
-   __init__.py        1     0    100%   
-   psnawp.py          35    0    100%   
-/opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/
+   __init__.py           1     0    100%   
+   psnawp.py             35    0    100%   
+/opt/hostedtoolcache/Python/3.11.4/x64/lib/python3.11/site-packages/
 psnawp_api/core
-   __init__.py        0     0    100%   
-   authenticator.py   46    3    3     93%
-   psnawp_exceptions.p9     0    100%   
-/opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/
+   __init__.py           0     0    100%   
+   authenticator.py      46    3    3     93%
+   psnawp_exceptions.py  9     0    100%   
+/opt/hostedtoolcache/Python/3.11.4/x64/lib/python3.11/site-packages/
 psnawp_api/models
-   __init__.py        0     0    100%   
-   client.py          68    0    100%   
-   game_title.py      22    0    100%   
-   group.py           52    0    100%   
-   search.py          22    0    100%   
-   title_stats.py     64    2    2     97%
-   user.py            69    0    100%   
-/opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/
+   __init__.py           0     0    100%   
+   client.py             70    0    100%   
+   game_title.py         22    0    100%   
+   group.py              52    0    100%   
+   search.py             22    0    100%   
+   title_stats.py        84    23   23    73%
+   user.py               71    0    100%   
+/opt/hostedtoolcache/Python/3.11.4/x64/lib/python3.11/site-packages/
+psnawp_api/models/listing
+   __init__.py           0     0    100%   
+   listing_generator.py  36    5    5     86%
+   pagination_arguments.p15    0    100%   
+/opt/hostedtoolcache/Python/3.11.4/x64/lib/python3.11/site-packages/
 psnawp_api/models/trophies
-   __init__.py        0     0    100%   
-   trophy.py          112   0    100%   
-   trophy_constants.py25    0    100%   
-   trophy_group.py    89    0    100%   
-   trophy_summary.py  25    0    100%   
-   trophy_titles.py   86    0    100%   
-   utility_functions.p7     0    100%   
-/opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/
+   __init__.py           0     0    100%   
+   trophy.py             112   0    100%   
+   trophy_constants.py   25    0    100%   
+   trophy_group.py       89    0    100%   
+   trophy_summary.py     25    0    100%   
+   trophy_titles.py      86    0    100%   
+   utility_functions.py  7     0    100%   
+/opt/hostedtoolcache/Python/3.11.4/x64/lib/python3.11/site-packages/
 psnawp_api/utils
-   __init__.py        0     0    100%   
-   endpoints.py       2     0    100%   
-   misc.py            35    0    100%   
-   request_builder.py 72    15   15    79%
-TOTAL                   841   20   98%    
+   __init__.py           0     0    100%   
+   endpoints.py          2     0    100%   
+   misc.py               35    0    100%   
+   request_builder.py    72    15   15    79%
+TOTAL                      916   46   95%    
  ## How to install ### From PyPI ``` pip install PSNAWP ``` ### Using
 `setup.py` To install the library into python. First you need to clone the repo
 at your local machine and run the following command from the root directory of
 the repo ``` python setup.py install ``` ## Important Links > PyPI: https://
 pypi.org/project/PSNAWP/ > > Read the Docs: https://psnawp.readthedocs.io/en/
 latest/ ## Getting Started To get started you need to obtain npsso <64
 character code>. You need to follow the following steps 1. Login into your [My
```

### Comparing `PSNAWP-1.2.3/README.md` & `PSNAWP-1.3.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 [![pytest](https://github.com/isFakeAccount/psnawp/actions/workflows/pytest.yaml/badge.svg)](https://github.com/isFakeAccount/psnawp/actions/workflows/pytest.yaml)
 [![pre-commit](https://github.com/isFakeAccount/psnawp/actions/workflows/pre-commit.yaml/badge.svg)](https://github.com/isFakeAccount/psnawp/actions/workflows/pre-commit.yaml)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Documentation Status](https://readthedocs.org/projects/psnawp/badge/?version=latest)](https://psnawp.readthedocs.io/en/latest/?badge=latest)
 [![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
 
 <!-- Pytest Coverage Comment:Begin -->
-<a href="https://github.com/isFakeAccount/psnawp/blob/main/README.md"><img alt="Coverage" src="https://img.shields.io/badge/Coverage-98%25-brightgreen.svg" /></a><details><summary>Coverage Report </summary><table><tr><th>File</th><th>Stmts</th><th>Miss</th><th>Cover</th><th>Missing</th></tr><tbody><tr><td colspan="5"><b>/opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/psnawp_api</b></td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/psnawp_api/__init__.py">__init__.py</a></td><td>1</td><td>0</td><td>100%</td><td>&nbsp;</td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/psnawp_api/psnawp.py">psnawp.py</a></td><td>35</td><td>0</td><td>100%</td><td>&nbsp;</td></tr><tr><td colspan="5"><b>/opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/psnawp_api/core</b></td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/psnawp_api/core/__init__.py">__init__.py</a></td><td>0</td><td>0</td><td>100%</td><td>&nbsp;</td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/psnawp_api/core/authenticator.py">authenticator.py</a></td><td>46</td><td>3</td><td>3</td><td><a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/psnawp_api/core/authenticator.py#L 93%"> 93%</a></td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/psnawp_api/core/psnawp_exceptions.py">psnawp_exceptions.py</a></td><td>9</td><td>0</td><td>100%</td><td>&nbsp;</td></tr><tr><td colspan="5"><b>/opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/psnawp_api/models</b></td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/psnawp_api/models/__init__.py">__init__.py</a></td><td>0</td><td>0</td><td>100%</td><td>&nbsp;</td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/psnawp_api/models/client.py">client.py</a></td><td>68</td><td>0</td><td>100%</td><td>&nbsp;</td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/psnawp_api/models/game_title.py">game_title.py</a></td><td>22</td><td>0</td><td>100%</td><td>&nbsp;</td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/psnawp_api/models/group.py">group.py</a></td><td>52</td><td>0</td><td>100%</td><td>&nbsp;</td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/psnawp_api/models/search.py">search.py</a></td><td>22</td><td>0</td><td>100%</td><td>&nbsp;</td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/psnawp_api/models/title_stats.py">title_stats.py</a></td><td>64</td><td>2</td><td>2</td><td><a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/psnawp_api/models/title_stats.py#L 97%"> 97%</a></td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/psnawp_api/models/user.py">user.py</a></td><td>69</td><td>0</td><td>100%</td><td>&nbsp;</td></tr><tr><td colspan="5"><b>/opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/psnawp_api/models/trophies</b></td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/psnawp_api/models/trophies/__init__.py">__init__.py</a></td><td>0</td><td>0</td><td>100%</td><td>&nbsp;</td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/psnawp_api/models/trophies/trophy.py">trophy.py</a></td><td>112</td><td>0</td><td>100%</td><td>&nbsp;</td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/psnawp_api/models/trophies/trophy_constants.py">trophy_constants.py</a></td><td>25</td><td>0</td><td>100%</td><td>&nbsp;</td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/psnawp_api/models/trophies/trophy_group.py">trophy_group.py</a></td><td>89</td><td>0</td><td>100%</td><td>&nbsp;</td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/psnawp_api/models/trophies/trophy_summary.py">trophy_summary.py</a></td><td>25</td><td>0</td><td>100%</td><td>&nbsp;</td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/psnawp_api/models/trophies/trophy_titles.py">trophy_titles.py</a></td><td>86</td><td>0</td><td>100%</td><td>&nbsp;</td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/psnawp_api/models/trophies/utility_functions.py">utility_functions.py</a></td><td>7</td><td>0</td><td>100%</td><td>&nbsp;</td></tr><tr><td colspan="5"><b>/opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/psnawp_api/utils</b></td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/psnawp_api/utils/__init__.py">__init__.py</a></td><td>0</td><td>0</td><td>100%</td><td>&nbsp;</td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/psnawp_api/utils/endpoints.py">endpoints.py</a></td><td>2</td><td>0</td><td>100%</td><td>&nbsp;</td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/psnawp_api/utils/misc.py">misc.py</a></td><td>35</td><td>0</td><td>100%</td><td>&nbsp;</td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/psnawp_api/utils/request_builder.py">request_builder.py</a></td><td>72</td><td>15</td><td>15</td><td><a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/psnawp_api/utils/request_builder.py#L 79%"> 79%</a></td></tr><tr><td><b>TOTAL</b></td><td><b>841</b></td><td><b>20</b></td><td><b>98%</b></td><td>&nbsp;</td></tr></tbody></table></details>
+<a href="https://github.com/isFakeAccount/psnawp/blob/main/README.md"><img alt="Coverage" src="https://img.shields.io/badge/Coverage-95%25-brightgreen.svg" /></a><details><summary>Coverage Report </summary><table><tr><th>File</th><th>Stmts</th><th>Miss</th><th>Cover</th><th>Missing</th></tr><tbody><tr><td colspan="5"><b>/opt/hostedtoolcache/Python/3.11.4/x64/lib/python3.11/site-packages/psnawp_api</b></td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.4/x64/lib/python3.11/site-packages/psnawp_api/__init__.py">__init__.py</a></td><td>1</td><td>0</td><td>100%</td><td>&nbsp;</td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.4/x64/lib/python3.11/site-packages/psnawp_api/psnawp.py">psnawp.py</a></td><td>35</td><td>0</td><td>100%</td><td>&nbsp;</td></tr><tr><td colspan="5"><b>/opt/hostedtoolcache/Python/3.11.4/x64/lib/python3.11/site-packages/psnawp_api/core</b></td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.4/x64/lib/python3.11/site-packages/psnawp_api/core/__init__.py">__init__.py</a></td><td>0</td><td>0</td><td>100%</td><td>&nbsp;</td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.4/x64/lib/python3.11/site-packages/psnawp_api/core/authenticator.py">authenticator.py</a></td><td>46</td><td>3</td><td>3</td><td><a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.4/x64/lib/python3.11/site-packages/psnawp_api/core/authenticator.py#L 93%"> 93%</a></td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.4/x64/lib/python3.11/site-packages/psnawp_api/core/psnawp_exceptions.py">psnawp_exceptions.py</a></td><td>9</td><td>0</td><td>100%</td><td>&nbsp;</td></tr><tr><td colspan="5"><b>/opt/hostedtoolcache/Python/3.11.4/x64/lib/python3.11/site-packages/psnawp_api/models</b></td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.4/x64/lib/python3.11/site-packages/psnawp_api/models/__init__.py">__init__.py</a></td><td>0</td><td>0</td><td>100%</td><td>&nbsp;</td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.4/x64/lib/python3.11/site-packages/psnawp_api/models/client.py">client.py</a></td><td>70</td><td>0</td><td>100%</td><td>&nbsp;</td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.4/x64/lib/python3.11/site-packages/psnawp_api/models/game_title.py">game_title.py</a></td><td>22</td><td>0</td><td>100%</td><td>&nbsp;</td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.4/x64/lib/python3.11/site-packages/psnawp_api/models/group.py">group.py</a></td><td>52</td><td>0</td><td>100%</td><td>&nbsp;</td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.4/x64/lib/python3.11/site-packages/psnawp_api/models/search.py">search.py</a></td><td>22</td><td>0</td><td>100%</td><td>&nbsp;</td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.4/x64/lib/python3.11/site-packages/psnawp_api/models/title_stats.py">title_stats.py</a></td><td>84</td><td>23</td><td>23</td><td><a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.4/x64/lib/python3.11/site-packages/psnawp_api/models/title_stats.py#L 73%"> 73%</a></td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.4/x64/lib/python3.11/site-packages/psnawp_api/models/user.py">user.py</a></td><td>71</td><td>0</td><td>100%</td><td>&nbsp;</td></tr><tr><td colspan="5"><b>/opt/hostedtoolcache/Python/3.11.4/x64/lib/python3.11/site-packages/psnawp_api/models/listing</b></td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.4/x64/lib/python3.11/site-packages/psnawp_api/models/listing/__init__.py">__init__.py</a></td><td>0</td><td>0</td><td>100%</td><td>&nbsp;</td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.4/x64/lib/python3.11/site-packages/psnawp_api/models/listing/listing_generator.py">listing_generator.py</a></td><td>36</td><td>5</td><td>5</td><td><a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.4/x64/lib/python3.11/site-packages/psnawp_api/models/listing/listing_generator.py#L 86%"> 86%</a></td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.4/x64/lib/python3.11/site-packages/psnawp_api/models/listing/pagination_arguments.py">pagination_arguments.py</a></td><td>15</td><td>0</td><td>100%</td><td>&nbsp;</td></tr><tr><td colspan="5"><b>/opt/hostedtoolcache/Python/3.11.4/x64/lib/python3.11/site-packages/psnawp_api/models/trophies</b></td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.4/x64/lib/python3.11/site-packages/psnawp_api/models/trophies/__init__.py">__init__.py</a></td><td>0</td><td>0</td><td>100%</td><td>&nbsp;</td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.4/x64/lib/python3.11/site-packages/psnawp_api/models/trophies/trophy.py">trophy.py</a></td><td>112</td><td>0</td><td>100%</td><td>&nbsp;</td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.4/x64/lib/python3.11/site-packages/psnawp_api/models/trophies/trophy_constants.py">trophy_constants.py</a></td><td>25</td><td>0</td><td>100%</td><td>&nbsp;</td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.4/x64/lib/python3.11/site-packages/psnawp_api/models/trophies/trophy_group.py">trophy_group.py</a></td><td>89</td><td>0</td><td>100%</td><td>&nbsp;</td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.4/x64/lib/python3.11/site-packages/psnawp_api/models/trophies/trophy_summary.py">trophy_summary.py</a></td><td>25</td><td>0</td><td>100%</td><td>&nbsp;</td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.4/x64/lib/python3.11/site-packages/psnawp_api/models/trophies/trophy_titles.py">trophy_titles.py</a></td><td>86</td><td>0</td><td>100%</td><td>&nbsp;</td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.4/x64/lib/python3.11/site-packages/psnawp_api/models/trophies/utility_functions.py">utility_functions.py</a></td><td>7</td><td>0</td><td>100%</td><td>&nbsp;</td></tr><tr><td colspan="5"><b>/opt/hostedtoolcache/Python/3.11.4/x64/lib/python3.11/site-packages/psnawp_api/utils</b></td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.4/x64/lib/python3.11/site-packages/psnawp_api/utils/__init__.py">__init__.py</a></td><td>0</td><td>0</td><td>100%</td><td>&nbsp;</td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.4/x64/lib/python3.11/site-packages/psnawp_api/utils/endpoints.py">endpoints.py</a></td><td>2</td><td>0</td><td>100%</td><td>&nbsp;</td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.4/x64/lib/python3.11/site-packages/psnawp_api/utils/misc.py">misc.py</a></td><td>35</td><td>0</td><td>100%</td><td>&nbsp;</td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.4/x64/lib/python3.11/site-packages/psnawp_api/utils/request_builder.py">request_builder.py</a></td><td>72</td><td>15</td><td>15</td><td><a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.4/x64/lib/python3.11/site-packages/psnawp_api/utils/request_builder.py#L 79%"> 79%</a></td></tr><tr><td><b>TOTAL</b></td><td><b>916</b></td><td><b>46</b></td><td><b>95%</b></td><td>&nbsp;</td></tr></tbody></table></details>
 <!-- Pytest Coverage Comment:End -->
 
 ## How to install
 
 ### From PyPI
 
 ```
```

#### html2text {}

```diff
@@ -10,49 +10,54 @@
 badge.svg)](https://github.com/isFakeAccount/psnawp/actions/workflows/pre-
 commit.yaml) [![Code style: black](https://img.shields.io/badge/code%20style-
 black-000000.svg)](https://github.com/psf/black) [![Documentation Status]
 (https://readthedocs.org/projects/psnawp/badge/?version=latest)](https://
 psnawp.readthedocs.io/en/latest/?badge=latest) [![License: MIT](https://
 img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/
 MIT)  [Coverage]Coverage Report
-File                    Stmts Miss Cover Missing
-/opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/
+File                       Stmts Miss Cover Missing
+/opt/hostedtoolcache/Python/3.11.4/x64/lib/python3.11/site-packages/
 psnawp_api
-   __init__.py        1     0    100%   
-   psnawp.py          35    0    100%   
-/opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/
+   __init__.py           1     0    100%   
+   psnawp.py             35    0    100%   
+/opt/hostedtoolcache/Python/3.11.4/x64/lib/python3.11/site-packages/
 psnawp_api/core
-   __init__.py        0     0    100%   
-   authenticator.py   46    3    3     93%
-   psnawp_exceptions.p9     0    100%   
-/opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/
+   __init__.py           0     0    100%   
+   authenticator.py      46    3    3     93%
+   psnawp_exceptions.py  9     0    100%   
+/opt/hostedtoolcache/Python/3.11.4/x64/lib/python3.11/site-packages/
 psnawp_api/models
-   __init__.py        0     0    100%   
-   client.py          68    0    100%   
-   game_title.py      22    0    100%   
-   group.py           52    0    100%   
-   search.py          22    0    100%   
-   title_stats.py     64    2    2     97%
-   user.py            69    0    100%   
-/opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/
+   __init__.py           0     0    100%   
+   client.py             70    0    100%   
+   game_title.py         22    0    100%   
+   group.py              52    0    100%   
+   search.py             22    0    100%   
+   title_stats.py        84    23   23    73%
+   user.py               71    0    100%   
+/opt/hostedtoolcache/Python/3.11.4/x64/lib/python3.11/site-packages/
+psnawp_api/models/listing
+   __init__.py           0     0    100%   
+   listing_generator.py  36    5    5     86%
+   pagination_arguments.p15    0    100%   
+/opt/hostedtoolcache/Python/3.11.4/x64/lib/python3.11/site-packages/
 psnawp_api/models/trophies
-   __init__.py        0     0    100%   
-   trophy.py          112   0    100%   
-   trophy_constants.py25    0    100%   
-   trophy_group.py    89    0    100%   
-   trophy_summary.py  25    0    100%   
-   trophy_titles.py   86    0    100%   
-   utility_functions.p7     0    100%   
-/opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/
+   __init__.py           0     0    100%   
+   trophy.py             112   0    100%   
+   trophy_constants.py   25    0    100%   
+   trophy_group.py       89    0    100%   
+   trophy_summary.py     25    0    100%   
+   trophy_titles.py      86    0    100%   
+   utility_functions.py  7     0    100%   
+/opt/hostedtoolcache/Python/3.11.4/x64/lib/python3.11/site-packages/
 psnawp_api/utils
-   __init__.py        0     0    100%   
-   endpoints.py       2     0    100%   
-   misc.py            35    0    100%   
-   request_builder.py 72    15   15    79%
-TOTAL                   841   20   98%    
+   __init__.py           0     0    100%   
+   endpoints.py          2     0    100%   
+   misc.py               35    0    100%   
+   request_builder.py    72    15   15    79%
+TOTAL                      916   46   95%    
  ## How to install ### From PyPI ``` pip install PSNAWP ``` ### Using
 `setup.py` To install the library into python. First you need to clone the repo
 at your local machine and run the following command from the root directory of
 the repo ``` python setup.py install ``` ## Important Links > PyPI: https://
 pypi.org/project/PSNAWP/ > > Read the Docs: https://psnawp.readthedocs.io/en/
 latest/ ## Getting Started To get started you need to obtain npsso <64
 character code>. You need to follow the following steps 1. Login into your [My
```

### Comparing `PSNAWP-1.2.3/pyproject.toml` & `PSNAWP-1.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `PSNAWP-1.2.3/requirements.txt` & `PSNAWP-1.3.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `PSNAWP-1.2.3/requirements_dev.txt` & `PSNAWP-1.3.0/requirements_dev.txt`

 * *Files identical despite different names*

### Comparing `PSNAWP-1.2.3/setup.cfg` & `PSNAWP-1.3.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = PSNAWP
-version = 1.2.3
+version = 1.3.0
 author = Yoshikage Kira (@isFakeAccount)
 author_email = trevorphillips@gmx.us
 url = https://github.com/isFakeAccount/psnawp
 description = Python API Wrapper for PlayStation Network API
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = MIT
@@ -42,15 +42,15 @@
 
 [options.packages.find]
 where = src
 
 [options.extras_require]
 testing = file: requirements_dev.txt
 docs = 
-	sphinx==5.3.0
+	sphinx==7.0.1
 	sphinx-materialdesign-theme==0.1.11
 
 [options.package_data]
 psnawp_api = py.typed
 
 [egg_info]
 tag_build =
```

### Comparing `PSNAWP-1.2.3/src/PSNAWP.egg-info/PKG-INFO` & `PSNAWP-1.3.0/src/PSNAWP.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PSNAWP
-Version: 1.2.3
+Version: 1.3.0
 Summary: Python API Wrapper for PlayStation Network API
 Home-page: https://github.com/isFakeAccount/psnawp
 Author: Yoshikage Kira (@isFakeAccount)
 Author-email: trevorphillips@gmx.us
 License: MIT
 Project-URL: Bug Tracker, https://github.com/isFakeAccount/psnawp/issues
 Project-URL: Changelog, https://github.com/isFakeAccount/psnawp/blob/master/CHANGELOG.md
@@ -38,15 +38,15 @@
 [![pytest](https://github.com/isFakeAccount/psnawp/actions/workflows/pytest.yaml/badge.svg)](https://github.com/isFakeAccount/psnawp/actions/workflows/pytest.yaml)
 [![pre-commit](https://github.com/isFakeAccount/psnawp/actions/workflows/pre-commit.yaml/badge.svg)](https://github.com/isFakeAccount/psnawp/actions/workflows/pre-commit.yaml)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Documentation Status](https://readthedocs.org/projects/psnawp/badge/?version=latest)](https://psnawp.readthedocs.io/en/latest/?badge=latest)
 [![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
 
 <!-- Pytest Coverage Comment:Begin -->
-<a href="https://github.com/isFakeAccount/psnawp/blob/main/README.md"><img alt="Coverage" src="https://img.shields.io/badge/Coverage-98%25-brightgreen.svg" /></a><details><summary>Coverage Report </summary><table><tr><th>File</th><th>Stmts</th><th>Miss</th><th>Cover</th><th>Missing</th></tr><tbody><tr><td colspan="5"><b>/opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/psnawp_api</b></td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/psnawp_api/__init__.py">__init__.py</a></td><td>1</td><td>0</td><td>100%</td><td>&nbsp;</td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/psnawp_api/psnawp.py">psnawp.py</a></td><td>35</td><td>0</td><td>100%</td><td>&nbsp;</td></tr><tr><td colspan="5"><b>/opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/psnawp_api/core</b></td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/psnawp_api/core/__init__.py">__init__.py</a></td><td>0</td><td>0</td><td>100%</td><td>&nbsp;</td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/psnawp_api/core/authenticator.py">authenticator.py</a></td><td>46</td><td>3</td><td>3</td><td><a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/psnawp_api/core/authenticator.py#L 93%"> 93%</a></td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/psnawp_api/core/psnawp_exceptions.py">psnawp_exceptions.py</a></td><td>9</td><td>0</td><td>100%</td><td>&nbsp;</td></tr><tr><td colspan="5"><b>/opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/psnawp_api/models</b></td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/psnawp_api/models/__init__.py">__init__.py</a></td><td>0</td><td>0</td><td>100%</td><td>&nbsp;</td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/psnawp_api/models/client.py">client.py</a></td><td>68</td><td>0</td><td>100%</td><td>&nbsp;</td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/psnawp_api/models/game_title.py">game_title.py</a></td><td>22</td><td>0</td><td>100%</td><td>&nbsp;</td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/psnawp_api/models/group.py">group.py</a></td><td>52</td><td>0</td><td>100%</td><td>&nbsp;</td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/psnawp_api/models/search.py">search.py</a></td><td>22</td><td>0</td><td>100%</td><td>&nbsp;</td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/psnawp_api/models/title_stats.py">title_stats.py</a></td><td>64</td><td>2</td><td>2</td><td><a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/psnawp_api/models/title_stats.py#L 97%"> 97%</a></td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/psnawp_api/models/user.py">user.py</a></td><td>69</td><td>0</td><td>100%</td><td>&nbsp;</td></tr><tr><td colspan="5"><b>/opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/psnawp_api/models/trophies</b></td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/psnawp_api/models/trophies/__init__.py">__init__.py</a></td><td>0</td><td>0</td><td>100%</td><td>&nbsp;</td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/psnawp_api/models/trophies/trophy.py">trophy.py</a></td><td>112</td><td>0</td><td>100%</td><td>&nbsp;</td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/psnawp_api/models/trophies/trophy_constants.py">trophy_constants.py</a></td><td>25</td><td>0</td><td>100%</td><td>&nbsp;</td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/psnawp_api/models/trophies/trophy_group.py">trophy_group.py</a></td><td>89</td><td>0</td><td>100%</td><td>&nbsp;</td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/psnawp_api/models/trophies/trophy_summary.py">trophy_summary.py</a></td><td>25</td><td>0</td><td>100%</td><td>&nbsp;</td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/psnawp_api/models/trophies/trophy_titles.py">trophy_titles.py</a></td><td>86</td><td>0</td><td>100%</td><td>&nbsp;</td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/psnawp_api/models/trophies/utility_functions.py">utility_functions.py</a></td><td>7</td><td>0</td><td>100%</td><td>&nbsp;</td></tr><tr><td colspan="5"><b>/opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/psnawp_api/utils</b></td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/psnawp_api/utils/__init__.py">__init__.py</a></td><td>0</td><td>0</td><td>100%</td><td>&nbsp;</td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/psnawp_api/utils/endpoints.py">endpoints.py</a></td><td>2</td><td>0</td><td>100%</td><td>&nbsp;</td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/psnawp_api/utils/misc.py">misc.py</a></td><td>35</td><td>0</td><td>100%</td><td>&nbsp;</td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/psnawp_api/utils/request_builder.py">request_builder.py</a></td><td>72</td><td>15</td><td>15</td><td><a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/psnawp_api/utils/request_builder.py#L 79%"> 79%</a></td></tr><tr><td><b>TOTAL</b></td><td><b>841</b></td><td><b>20</b></td><td><b>98%</b></td><td>&nbsp;</td></tr></tbody></table></details>
+<a href="https://github.com/isFakeAccount/psnawp/blob/main/README.md"><img alt="Coverage" src="https://img.shields.io/badge/Coverage-95%25-brightgreen.svg" /></a><details><summary>Coverage Report </summary><table><tr><th>File</th><th>Stmts</th><th>Miss</th><th>Cover</th><th>Missing</th></tr><tbody><tr><td colspan="5"><b>/opt/hostedtoolcache/Python/3.11.4/x64/lib/python3.11/site-packages/psnawp_api</b></td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.4/x64/lib/python3.11/site-packages/psnawp_api/__init__.py">__init__.py</a></td><td>1</td><td>0</td><td>100%</td><td>&nbsp;</td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.4/x64/lib/python3.11/site-packages/psnawp_api/psnawp.py">psnawp.py</a></td><td>35</td><td>0</td><td>100%</td><td>&nbsp;</td></tr><tr><td colspan="5"><b>/opt/hostedtoolcache/Python/3.11.4/x64/lib/python3.11/site-packages/psnawp_api/core</b></td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.4/x64/lib/python3.11/site-packages/psnawp_api/core/__init__.py">__init__.py</a></td><td>0</td><td>0</td><td>100%</td><td>&nbsp;</td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.4/x64/lib/python3.11/site-packages/psnawp_api/core/authenticator.py">authenticator.py</a></td><td>46</td><td>3</td><td>3</td><td><a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.4/x64/lib/python3.11/site-packages/psnawp_api/core/authenticator.py#L 93%"> 93%</a></td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.4/x64/lib/python3.11/site-packages/psnawp_api/core/psnawp_exceptions.py">psnawp_exceptions.py</a></td><td>9</td><td>0</td><td>100%</td><td>&nbsp;</td></tr><tr><td colspan="5"><b>/opt/hostedtoolcache/Python/3.11.4/x64/lib/python3.11/site-packages/psnawp_api/models</b></td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.4/x64/lib/python3.11/site-packages/psnawp_api/models/__init__.py">__init__.py</a></td><td>0</td><td>0</td><td>100%</td><td>&nbsp;</td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.4/x64/lib/python3.11/site-packages/psnawp_api/models/client.py">client.py</a></td><td>70</td><td>0</td><td>100%</td><td>&nbsp;</td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.4/x64/lib/python3.11/site-packages/psnawp_api/models/game_title.py">game_title.py</a></td><td>22</td><td>0</td><td>100%</td><td>&nbsp;</td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.4/x64/lib/python3.11/site-packages/psnawp_api/models/group.py">group.py</a></td><td>52</td><td>0</td><td>100%</td><td>&nbsp;</td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.4/x64/lib/python3.11/site-packages/psnawp_api/models/search.py">search.py</a></td><td>22</td><td>0</td><td>100%</td><td>&nbsp;</td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.4/x64/lib/python3.11/site-packages/psnawp_api/models/title_stats.py">title_stats.py</a></td><td>84</td><td>23</td><td>23</td><td><a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.4/x64/lib/python3.11/site-packages/psnawp_api/models/title_stats.py#L 73%"> 73%</a></td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.4/x64/lib/python3.11/site-packages/psnawp_api/models/user.py">user.py</a></td><td>71</td><td>0</td><td>100%</td><td>&nbsp;</td></tr><tr><td colspan="5"><b>/opt/hostedtoolcache/Python/3.11.4/x64/lib/python3.11/site-packages/psnawp_api/models/listing</b></td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.4/x64/lib/python3.11/site-packages/psnawp_api/models/listing/__init__.py">__init__.py</a></td><td>0</td><td>0</td><td>100%</td><td>&nbsp;</td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.4/x64/lib/python3.11/site-packages/psnawp_api/models/listing/listing_generator.py">listing_generator.py</a></td><td>36</td><td>5</td><td>5</td><td><a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.4/x64/lib/python3.11/site-packages/psnawp_api/models/listing/listing_generator.py#L 86%"> 86%</a></td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.4/x64/lib/python3.11/site-packages/psnawp_api/models/listing/pagination_arguments.py">pagination_arguments.py</a></td><td>15</td><td>0</td><td>100%</td><td>&nbsp;</td></tr><tr><td colspan="5"><b>/opt/hostedtoolcache/Python/3.11.4/x64/lib/python3.11/site-packages/psnawp_api/models/trophies</b></td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.4/x64/lib/python3.11/site-packages/psnawp_api/models/trophies/__init__.py">__init__.py</a></td><td>0</td><td>0</td><td>100%</td><td>&nbsp;</td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.4/x64/lib/python3.11/site-packages/psnawp_api/models/trophies/trophy.py">trophy.py</a></td><td>112</td><td>0</td><td>100%</td><td>&nbsp;</td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.4/x64/lib/python3.11/site-packages/psnawp_api/models/trophies/trophy_constants.py">trophy_constants.py</a></td><td>25</td><td>0</td><td>100%</td><td>&nbsp;</td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.4/x64/lib/python3.11/site-packages/psnawp_api/models/trophies/trophy_group.py">trophy_group.py</a></td><td>89</td><td>0</td><td>100%</td><td>&nbsp;</td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.4/x64/lib/python3.11/site-packages/psnawp_api/models/trophies/trophy_summary.py">trophy_summary.py</a></td><td>25</td><td>0</td><td>100%</td><td>&nbsp;</td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.4/x64/lib/python3.11/site-packages/psnawp_api/models/trophies/trophy_titles.py">trophy_titles.py</a></td><td>86</td><td>0</td><td>100%</td><td>&nbsp;</td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.4/x64/lib/python3.11/site-packages/psnawp_api/models/trophies/utility_functions.py">utility_functions.py</a></td><td>7</td><td>0</td><td>100%</td><td>&nbsp;</td></tr><tr><td colspan="5"><b>/opt/hostedtoolcache/Python/3.11.4/x64/lib/python3.11/site-packages/psnawp_api/utils</b></td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.4/x64/lib/python3.11/site-packages/psnawp_api/utils/__init__.py">__init__.py</a></td><td>0</td><td>0</td><td>100%</td><td>&nbsp;</td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.4/x64/lib/python3.11/site-packages/psnawp_api/utils/endpoints.py">endpoints.py</a></td><td>2</td><td>0</td><td>100%</td><td>&nbsp;</td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.4/x64/lib/python3.11/site-packages/psnawp_api/utils/misc.py">misc.py</a></td><td>35</td><td>0</td><td>100%</td><td>&nbsp;</td></tr><tr><td>&nbsp; &nbsp;<a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.4/x64/lib/python3.11/site-packages/psnawp_api/utils/request_builder.py">request_builder.py</a></td><td>72</td><td>15</td><td>15</td><td><a href="https://github.com/isFakeAccount/psnawp/blob/main//opt/hostedtoolcache/Python/3.11.4/x64/lib/python3.11/site-packages/psnawp_api/utils/request_builder.py#L 79%"> 79%</a></td></tr><tr><td><b>TOTAL</b></td><td><b>916</b></td><td><b>46</b></td><td><b>95%</b></td><td>&nbsp;</td></tr></tbody></table></details>
 <!-- Pytest Coverage Comment:End -->
 
 ## How to install
 
 ### From PyPI
 
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: PSNAWP Version: 1.2.3 Summary: Python API Wrapper
+Metadata-Version: 2.1 Name: PSNAWP Version: 1.3.0 Summary: Python API Wrapper
 for PlayStation Network API Home-page: https://github.com/isFakeAccount/psnawp
 Author: Yoshikage Kira (@isFakeAccount) Author-email: trevorphillips@gmx.us
 License: MIT Project-URL: Bug Tracker, https://github.com/isFakeAccount/psnawp/
 issues Project-URL: Changelog, https://github.com/isFakeAccount/psnawp/blob/
 master/CHANGELOG.md Project-URL: Source Code, https://github.com/isFakeAccount/
 psnawp Project-URL: Documentation, https://psnawp.readthedocs.io/en/latest/
 Keywords: PSN API Platform: any Classifier: Development Status :: 4 - Beta
@@ -25,49 +25,54 @@
 psnawp/actions/workflows/pre-commit.yaml/badge.svg)](https://github.com/
 isFakeAccount/psnawp/actions/workflows/pre-commit.yaml) [![Code style: black]
 (https://img.shields.io/badge/code%20style-black-000000.svg)](https://
 github.com/psf/black) [![Documentation Status](https://readthedocs.org/
 projects/psnawp/badge/?version=latest)](https://psnawp.readthedocs.io/en/
 latest/?badge=latest) [![License: MIT](https://img.shields.io/badge/License-
 MIT-blue.svg)](https://opensource.org/licenses/MIT)  [Coverage]Coverage Report
-File                    Stmts Miss Cover Missing
-/opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/
+File                       Stmts Miss Cover Missing
+/opt/hostedtoolcache/Python/3.11.4/x64/lib/python3.11/site-packages/
 psnawp_api
-   __init__.py        1     0    100%   
-   psnawp.py          35    0    100%   
-/opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/
+   __init__.py           1     0    100%   
+   psnawp.py             35    0    100%   
+/opt/hostedtoolcache/Python/3.11.4/x64/lib/python3.11/site-packages/
 psnawp_api/core
-   __init__.py        0     0    100%   
-   authenticator.py   46    3    3     93%
-   psnawp_exceptions.p9     0    100%   
-/opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/
+   __init__.py           0     0    100%   
+   authenticator.py      46    3    3     93%
+   psnawp_exceptions.py  9     0    100%   
+/opt/hostedtoolcache/Python/3.11.4/x64/lib/python3.11/site-packages/
 psnawp_api/models
-   __init__.py        0     0    100%   
-   client.py          68    0    100%   
-   game_title.py      22    0    100%   
-   group.py           52    0    100%   
-   search.py          22    0    100%   
-   title_stats.py     64    2    2     97%
-   user.py            69    0    100%   
-/opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/
+   __init__.py           0     0    100%   
+   client.py             70    0    100%   
+   game_title.py         22    0    100%   
+   group.py              52    0    100%   
+   search.py             22    0    100%   
+   title_stats.py        84    23   23    73%
+   user.py               71    0    100%   
+/opt/hostedtoolcache/Python/3.11.4/x64/lib/python3.11/site-packages/
+psnawp_api/models/listing
+   __init__.py           0     0    100%   
+   listing_generator.py  36    5    5     86%
+   pagination_arguments.p15    0    100%   
+/opt/hostedtoolcache/Python/3.11.4/x64/lib/python3.11/site-packages/
 psnawp_api/models/trophies
-   __init__.py        0     0    100%   
-   trophy.py          112   0    100%   
-   trophy_constants.py25    0    100%   
-   trophy_group.py    89    0    100%   
-   trophy_summary.py  25    0    100%   
-   trophy_titles.py   86    0    100%   
-   utility_functions.p7     0    100%   
-/opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/
+   __init__.py           0     0    100%   
+   trophy.py             112   0    100%   
+   trophy_constants.py   25    0    100%   
+   trophy_group.py       89    0    100%   
+   trophy_summary.py     25    0    100%   
+   trophy_titles.py      86    0    100%   
+   utility_functions.py  7     0    100%   
+/opt/hostedtoolcache/Python/3.11.4/x64/lib/python3.11/site-packages/
 psnawp_api/utils
-   __init__.py        0     0    100%   
-   endpoints.py       2     0    100%   
-   misc.py            35    0    100%   
-   request_builder.py 72    15   15    79%
-TOTAL                   841   20   98%    
+   __init__.py           0     0    100%   
+   endpoints.py          2     0    100%   
+   misc.py               35    0    100%   
+   request_builder.py    72    15   15    79%
+TOTAL                      916   46   95%    
  ## How to install ### From PyPI ``` pip install PSNAWP ``` ### Using
 `setup.py` To install the library into python. First you need to clone the repo
 at your local machine and run the following command from the root directory of
 the repo ``` python setup.py install ``` ## Important Links > PyPI: https://
 pypi.org/project/PSNAWP/ > > Read the Docs: https://psnawp.readthedocs.io/en/
 latest/ ## Getting Started To get started you need to obtain npsso <64
 character code>. You need to follow the following steps 1. Login into your [My
```

### Comparing `PSNAWP-1.2.3/src/PSNAWP.egg-info/SOURCES.txt` & `PSNAWP-1.3.0/src/PSNAWP.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -21,14 +21,17 @@
 src/psnawp_api/models/__init__.py
 src/psnawp_api/models/client.py
 src/psnawp_api/models/game_title.py
 src/psnawp_api/models/group.py
 src/psnawp_api/models/search.py
 src/psnawp_api/models/title_stats.py
 src/psnawp_api/models/user.py
+src/psnawp_api/models/listing/__init__.py
+src/psnawp_api/models/listing/listing_generator.py
+src/psnawp_api/models/listing/pagination_arguments.py
 src/psnawp_api/models/trophies/__init__.py
 src/psnawp_api/models/trophies/trophy.py
 src/psnawp_api/models/trophies/trophy_constants.py
 src/psnawp_api/models/trophies/trophy_group.py
 src/psnawp_api/models/trophies/trophy_summary.py
 src/psnawp_api/models/trophies/trophy_titles.py
 src/psnawp_api/models/trophies/utility_functions.py
```

### Comparing `PSNAWP-1.2.3/src/PSNAWP.egg-info/requires.txt` & `PSNAWP-1.3.0/src/PSNAWP.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 chardet==5.1.0
 charset-normalizer==3.0.1
 idna==3.4
 requests==2.28.2
 urllib3==1.26.14
 
 [docs]
-sphinx==5.3.0
+sphinx==7.0.1
 sphinx-materialdesign-theme==0.1.11
 
 [testing]
 alabaster==0.7.13
 attrs==22.2.0
 babel==2.11.0
 bleach==6.0.0
```

### Comparing `PSNAWP-1.2.3/src/psnawp_api/core/authenticator.py` & `PSNAWP-1.3.0/src/psnawp_api/core/authenticator.py`

 * *Files identical despite different names*

### Comparing `PSNAWP-1.2.3/src/psnawp_api/core/psnawp_exceptions.py` & `PSNAWP-1.3.0/src/psnawp_api/core/psnawp_exceptions.py`

 * *Files identical despite different names*

### Comparing `PSNAWP-1.2.3/src/psnawp_api/models/client.py` & `PSNAWP-1.3.0/src/psnawp_api/models/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 
 from typing import Any, Iterator, Optional, Literal
 
 from psnawp_api.models.group import Group
-from psnawp_api.models.title_stats import TitleStats
+from psnawp_api.models.listing.pagination_arguments import PaginationArguments
+from psnawp_api.models.title_stats import TitleStatsListing
 from psnawp_api.models.trophies.trophy import Trophy, TrophyBuilder
 from psnawp_api.models.trophies.trophy_group import (
     TrophyGroupsSummary,
     TrophyGroupsSummaryBuilder,
 )
 from psnawp_api.models.trophies.trophy_summary import TrophySummary
 from psnawp_api.models.trophies.trophy_titles import TrophyTitles, TrophyTitle
@@ -365,33 +366,38 @@
             ).user_trophy_groups_summary(account_id="me", platform=platform)
         else:
             return TrophyGroupsSummaryBuilder(
                 request_builder=self._request_builder,
                 np_communication_id=np_communication_id,
             ).user_trophy_groups_summary_with_metadata(account_id="me", platform=platform)
 
-    def title_stats(self, limit: Optional[int] = None) -> Iterator[TitleStats]:
+    def title_stats(self, *, limit: Optional[int] = None, offset: int = 0, page_size: int = 200) -> TitleStatsListing:
         """Retrieve a list of titles with their stats and basic meta-data
 
         :param limit: Limit of titles returned.
         :type limit: Optional[int]
+        :param page_size: The number of items to receive per api request.
+        :type page_size: int
+        :param offset: Specifies the offset for paginator
+        :type offset: int
 
         .. warning::
 
             Only returns data for PS4 games and above.
 
-        :returns: List of Titles with their play times
-        :rtype: Iterator[TitleStats]
+        :returns: Iterator class for TitleStats
+        :rtype: Iterator[TitleStatsListing]
 
         .. code-block:: Python
 
-            client = psnawp.me()
-            titles = client.title_stats()
+            user_example = psnawp.client()
+            titles = list(user_example.title_stats())
 
         """
-        return TitleStats.from_endpoint(request_builder=self._request_builder, account_id="me", limit=limit)
+        pg_args = PaginationArguments(total_limit=limit, offset=offset, page_size=page_size)
+        return TitleStatsListing(request_builder=self._request_builder, account_id="me", pagination_arguments=pg_args)
 
     def __repr__(self) -> str:
         return f"<User online_id:{self.online_id} account_id:{self.account_id}>"
 
     def __str__(self) -> str:
         return f"Online ID: {self.online_id} Account ID: {self.account_id}"
```

### Comparing `PSNAWP-1.2.3/src/psnawp_api/models/game_title.py` & `PSNAWP-1.3.0/src/psnawp_api/models/game_title.py`

 * *Files identical despite different names*

### Comparing `PSNAWP-1.2.3/src/psnawp_api/models/group.py` & `PSNAWP-1.3.0/src/psnawp_api/models/group.py`

 * *Files identical despite different names*

### Comparing `PSNAWP-1.2.3/src/psnawp_api/models/search.py` & `PSNAWP-1.3.0/src/psnawp_api/models/search.py`

 * *Files identical despite different names*

### Comparing `PSNAWP-1.2.3/src/psnawp_api/models/trophies/trophy.py` & `PSNAWP-1.3.0/src/psnawp_api/models/trophies/trophy.py`

 * *Files identical despite different names*

### Comparing `PSNAWP-1.2.3/src/psnawp_api/models/trophies/trophy_constants.py` & `PSNAWP-1.3.0/src/psnawp_api/models/trophies/trophy_constants.py`

 * *Files identical despite different names*

### Comparing `PSNAWP-1.2.3/src/psnawp_api/models/trophies/trophy_group.py` & `PSNAWP-1.3.0/src/psnawp_api/models/trophies/trophy_group.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,22 +76,22 @@
             trophy_group_icon_url=trophy_group.get("trophyGroupIconUrl"),
             defined_trophies=TrophySet(
                 **trophy_group.get(
                     "definedTrophies",
                     {"bronze": 0, "silver": 0, "gold": 0, "platinum": 0},
                 )
             ),
-            progress=trophy_groups_dict.get("progress"),
+            progress=trophy_group.get("progress"),
             earned_trophies=TrophySet(
                 **trophy_group.get(
                     "earnedTrophies",
                     {"bronze": 0, "silver": 0, "gold": 0, "platinum": 0},
                 )
             ),
-            last_updated_datetime=trophy_groups_dict.get("lastUpdatedDateTime"),
+            last_updated_datetime=trophy_group.get("lastUpdatedDateTime"),
         )
         trophy_groups.append(trophy_group_instance)
 
     trophy_group_summary = TrophyGroupsSummary(
         trophy_set_version=trophy_groups_dict.get("trophySetVersion"),
         trophy_title_name=trophy_groups_dict.get("trophyTitleName"),
         trophy_title_detail=trophy_groups_dict.get("trophyTitleDetail"),
```

### Comparing `PSNAWP-1.2.3/src/psnawp_api/models/trophies/trophy_summary.py` & `PSNAWP-1.3.0/src/psnawp_api/models/trophies/trophy_summary.py`

 * *Files identical despite different names*

### Comparing `PSNAWP-1.2.3/src/psnawp_api/models/trophies/trophy_titles.py` & `PSNAWP-1.3.0/src/psnawp_api/models/trophies/trophy_titles.py`

 * *Files identical despite different names*

### Comparing `PSNAWP-1.2.3/src/psnawp_api/models/user.py` & `PSNAWP-1.3.0/src/psnawp_api/models/user.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,22 +3,23 @@
 from typing import Optional, Any, Iterator, Literal
 
 from psnawp_api.core.psnawp_exceptions import (
     PSNAWPNotFound,
     PSNAWPForbidden,
     PSNAWPBadRequest,
 )
+from psnawp_api.models.listing.pagination_arguments import PaginationArguments
+from psnawp_api.models.title_stats import TitleStatsListing
 from psnawp_api.models.trophies.trophy import TrophyBuilder, Trophy
 from psnawp_api.models.trophies.trophy_group import (
     TrophyGroupsSummary,
     TrophyGroupsSummaryBuilder,
 )
 from psnawp_api.models.trophies.trophy_summary import TrophySummary
 from psnawp_api.models.trophies.trophy_titles import TrophyTitles, TrophyTitle
-from psnawp_api.models.title_stats import TitleStats
 from psnawp_api.utils.endpoints import BASE_PATH, API_PATH
 from psnawp_api.utils.request_builder import RequestBuilder
 
 
 class User:
     """This class will contain the information about the PSN ID you passed in when creating object"""
 
@@ -337,33 +338,39 @@
             ).user_trophy_groups_summary(account_id=self.account_id, platform=platform)
         else:
             return TrophyGroupsSummaryBuilder(
                 request_builder=self._request_builder,
                 np_communication_id=np_communication_id,
             ).user_trophy_groups_summary_with_metadata(account_id=self.account_id, platform=platform)
 
-    def title_stats(self, limit: Optional[int] = None) -> Iterator[TitleStats]:
+    def title_stats(self, *, limit: Optional[int] = None, offset: int = 0, page_size: int = 200) -> TitleStatsListing:
         """Retrieve a list of titles with their stats and basic meta-data
 
         :param limit: Limit of titles returned.
         :type limit: Optional[int]
+        :param page_size: The number of items to receive per api request.
+        :type page_size: int
+        :param offset: Specifies the offset for paginator
+        :type offset: int
 
         .. warning::
 
             Only returns data for PS4 games and above.
 
-        :returns: List of Titles with their play times
-        :rtype: Iterator[TitleStats]
+        :returns: Iterator class for TitleStats
+        :rtype: Iterator[TitleStatsListing]
 
         .. code-block:: Python
 
             user_example = psnawp.user(online_id='jeranther')
-            titles = user_example.title_stats()
+            for title in user_example.title_stats():
+                ...
 
         """
-        return TitleStats.from_endpoint(request_builder=self._request_builder, account_id=self.account_id, limit=limit)
+        pg_args = PaginationArguments(total_limit=limit, offset=offset, page_size=page_size)
+        return TitleStatsListing(request_builder=self._request_builder, account_id=self.account_id, pagination_arguments=pg_args)
 
     def __repr__(self) -> str:
         return f"<User online_id:{self.online_id} account_id:{self.account_id}>"
 
     def __str__(self) -> str:
         return f"Online ID: {self.online_id} Account ID: {self.account_id}"
```

### Comparing `PSNAWP-1.2.3/src/psnawp_api/psnawp.py` & `PSNAWP-1.3.0/src/psnawp_api/psnawp.py`

 * *Files identical despite different names*

### Comparing `PSNAWP-1.2.3/src/psnawp_api/utils/endpoints.py` & `PSNAWP-1.3.0/src/psnawp_api/utils/endpoints.py`

 * *Files identical despite different names*

### Comparing `PSNAWP-1.2.3/src/psnawp_api/utils/misc.py` & `PSNAWP-1.3.0/src/psnawp_api/utils/misc.py`

 * *Files identical despite different names*

### Comparing `PSNAWP-1.2.3/src/psnawp_api/utils/request_builder.py` & `PSNAWP-1.3.0/src/psnawp_api/utils/request_builder.py`

 * *Files identical despite different names*

