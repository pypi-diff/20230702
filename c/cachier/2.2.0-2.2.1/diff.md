# Comparing `tmp/cachier-2.2.0.tar.gz` & `tmp/cachier-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cachier-2.2.0.tar", last modified: Fri Jun 30 13:52:05 2023, max compression
+gzip compressed data, was "cachier-2.2.1.tar", last modified: Sun Jul  2 09:23:49 2023, max compression
```

## Comparing `cachier-2.2.0.tar` & `cachier-2.2.1.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 shaypalachy   (501) staff       (20)        0 2023-06-30 13:52:05.519251 cachier-2.2.0/
--rw-r--r--   0 shaypalachy   (501) staff       (20)      447 2021-06-17 12:08:06.000000 cachier-2.2.0/.codecov.yml
--rw-r--r--   0 shaypalachy   (501) staff       (20)      394 2023-04-09 05:18:24.000000 cachier-2.2.0/.coveragerc
--rw-r--r--   0 shaypalachy   (501) staff       (20)      195 2021-06-17 12:08:06.000000 cachier-2.2.0/.deepsource.toml
--rw-r--r--   0 shaypalachy   (501) staff       (20)       30 2021-10-10 23:14:34.000000 cachier-2.2.0/.fdignore
--rw-r--r--   0 shaypalachy   (501) staff       (20)      202 2022-12-02 11:10:23.000000 cachier-2.2.0/.flake8
--rw-r--r--   0 shaypalachy   (501) staff       (20)       33 2021-06-17 12:08:06.000000 cachier-2.2.0/.gitattributes
-drwxr-xr-x   0 shaypalachy   (501) staff       (20)        0 2023-06-30 13:52:05.491686 cachier-2.2.0/.github/
-drwxr-xr-x   0 shaypalachy   (501) staff       (20)        0 2023-06-30 13:52:05.507514 cachier-2.2.0/.github/workflows/
--rw-r--r--   0 shaypalachy   (501) staff       (20)      680 2023-03-16 11:40:57.000000 cachier-2.2.0/.github/workflows/checkdocs.yml
--rw-r--r--   0 shaypalachy   (501) staff       (20)      775 2023-06-30 12:48:49.000000 cachier-2.2.0/.github/workflows/lint.yml
--rw-r--r--   0 shaypalachy   (501) staff       (20)      981 2023-06-30 12:48:49.000000 cachier-2.2.0/.github/workflows/test.yml
--rw-r--r--   0 shaypalachy   (501) staff       (20)     1249 2021-06-17 12:08:06.000000 cachier-2.2.0/.gitignore
--rw-r--r--   0 shaypalachy   (501) staff       (20)       67 2022-12-02 11:08:24.000000 cachier-2.2.0/.ignore
--rw-r--r--   0 shaypalachy   (501) staff       (20)     8489 2021-10-10 23:14:34.000000 cachier-2.2.0/.pylintrc
--rw-r--r--   0 shaypalachy   (501) staff       (20)     1069 2021-06-17 12:08:06.000000 cachier-2.2.0/LICENSE
--rw-r--r--   0 shaypalachy   (501) staff       (20)       50 2021-06-17 12:08:06.000000 cachier-2.2.0/MANIFEST.in
--rw-r--r--   0 shaypalachy   (501) staff       (20)    17490 2023-06-30 13:52:05.519438 cachier-2.2.0/PKG-INFO
--rw-r--r--   0 shaypalachy   (501) staff       (20)    16447 2023-06-30 12:49:12.000000 cachier-2.2.0/README.rst
-drwxr-xr-x   0 shaypalachy   (501) staff       (20)        0 2023-06-30 13:52:05.520260 cachier-2.2.0/cachier/
--rw-r--r--   0 shaypalachy   (501) staff       (20)      232 2023-04-09 05:18:24.000000 cachier-2.2.0/cachier/__init__.py
--rw-r--r--   0 shaypalachy   (501) staff       (20)      471 2023-06-30 13:52:05.520316 cachier-2.2.0/cachier/_version.py
--rw-r--r--   0 shaypalachy   (501) staff       (20)     3062 2023-04-09 05:18:24.000000 cachier-2.2.0/cachier/base_core.py
--rw-r--r--   0 shaypalachy   (501) staff       (20)    14505 2023-06-30 12:49:12.000000 cachier-2.2.0/cachier/core.py
--rw-r--r--   0 shaypalachy   (501) staff       (20)     2846 2023-04-09 05:18:24.000000 cachier-2.2.0/cachier/memory_core.py
--rw-r--r--   0 shaypalachy   (501) staff       (20)     5022 2023-04-09 05:18:24.000000 cachier-2.2.0/cachier/mongo_core.py
--rw-r--r--   0 shaypalachy   (501) staff       (20)    10068 2023-04-09 05:18:24.000000 cachier-2.2.0/cachier/pickle_core.py
--rw-r--r--   0 shaypalachy   (501) staff       (20)        0 2023-06-30 12:48:49.000000 cachier-2.2.0/cachier/py.typed
-drwxr-xr-x   0 shaypalachy   (501) staff       (20)        0 2023-06-30 13:52:05.513238 cachier-2.2.0/cachier/scripts/
--rw-r--r--   0 shaypalachy   (501) staff       (20)        0 2021-06-17 12:08:06.000000 cachier-2.2.0/cachier/scripts/__init__.py
--rw-r--r--   0 shaypalachy   (501) staff       (20)      429 2021-06-17 12:08:06.000000 cachier-2.2.0/cachier/scripts/cli.py
-drwxr-xr-x   0 shaypalachy   (501) staff       (20)        0 2023-06-30 13:52:05.512829 cachier-2.2.0/cachier.egg-info/
--rw-r--r--   0 shaypalachy   (501) staff       (20)    17490 2023-06-30 13:52:05.000000 cachier-2.2.0/cachier.egg-info/PKG-INFO
--rw-r--r--   0 shaypalachy   (501) staff       (20)      932 2023-06-30 13:52:05.000000 cachier-2.2.0/cachier.egg-info/SOURCES.txt
--rw-r--r--   0 shaypalachy   (501) staff       (20)        1 2023-06-30 13:52:05.000000 cachier-2.2.0/cachier.egg-info/dependency_links.txt
--rw-r--r--   0 shaypalachy   (501) staff       (20)       52 2023-06-30 13:52:05.000000 cachier-2.2.0/cachier.egg-info/entry_points.txt
--rw-r--r--   0 shaypalachy   (501) staff       (20)      220 2023-06-30 13:52:05.000000 cachier-2.2.0/cachier.egg-info/requires.txt
--rw-r--r--   0 shaypalachy   (501) staff       (20)        8 2023-06-30 13:52:05.000000 cachier-2.2.0/cachier.egg-info/top_level.txt
--rw-r--r--   0 shaypalachy   (501) staff       (20)      227 2023-06-30 12:48:49.000000 cachier-2.2.0/mypy.ini
--rw-r--r--   0 shaypalachy   (501) staff       (20)      308 2023-04-09 05:18:24.000000 cachier-2.2.0/pytest.ini
--rw-r--r--   0 shaypalachy   (501) staff       (20)      269 2023-06-30 13:52:05.519994 cachier-2.2.0/setup.cfg
--rw-r--r--   0 shaypalachy   (501) staff       (20)     2615 2023-06-30 12:48:49.000000 cachier-2.2.0/setup.py
-drwxr-xr-x   0 shaypalachy   (501) staff       (20)        0 2023-06-30 13:52:05.518782 cachier-2.2.0/tests/
--rw-r--r--   0 shaypalachy   (501) staff       (20)        0 2021-06-17 12:08:06.000000 cachier-2.2.0/tests/__init__.py
--rw-r--r--   0 shaypalachy   (501) staff       (20)     1903 2023-03-22 22:40:25.000000 cachier-2.2.0/tests/speed_eval.py
--rw-r--r--   0 shaypalachy   (501) staff       (20)      168 2023-03-31 07:33:42.000000 cachier-2.2.0/tests/standalone_script.py
--rw-r--r--   0 shaypalachy   (501) staff       (20)     1122 2023-06-30 12:49:12.000000 cachier-2.2.0/tests/test_core_lookup.py
--rw-r--r--   0 shaypalachy   (501) staff       (20)     6545 2023-06-30 12:49:12.000000 cachier-2.2.0/tests/test_defaults.py
--rw-r--r--   0 shaypalachy   (501) staff       (20)     7272 2023-06-30 12:49:12.000000 cachier-2.2.0/tests/test_general.py
--rw-r--r--   0 shaypalachy   (501) staff       (20)     8879 2023-03-31 07:33:42.000000 cachier-2.2.0/tests/test_memory_core.py
--rw-r--r--   0 shaypalachy   (501) staff       (20)     8963 2023-06-30 12:48:49.000000 cachier-2.2.0/tests/test_mongo_core.py
--rw-r--r--   0 shaypalachy   (501) staff       (20)    18211 2023-06-30 12:48:49.000000 cachier-2.2.0/tests/test_pickle_core.py
--rw-r--r--   0 shaypalachy   (501) staff       (20)      482 2023-03-22 22:40:25.000000 cachier-2.2.0/tests/test_quality.py
--rw-r--r--   0 shaypalachy   (501) staff       (20)      577 2023-03-22 22:40:25.000000 cachier-2.2.0/tests/test_security.py
--rw-r--r--   0 shaypalachy   (501) staff       (20)    65788 2023-06-30 12:48:49.000000 cachier-2.2.0/versioneer.py
+drwxr-xr-x   0 shaypalachy   (501) staff       (20)        0 2023-07-02 09:23:49.149724 cachier-2.2.1/
+-rw-r--r--   0 shaypalachy   (501) staff       (20)      447 2021-06-17 12:08:06.000000 cachier-2.2.1/.codecov.yml
+-rw-r--r--   0 shaypalachy   (501) staff       (20)      465 2023-07-02 09:22:38.000000 cachier-2.2.1/.coveragerc
+-rw-r--r--   0 shaypalachy   (501) staff       (20)      195 2021-06-17 12:08:06.000000 cachier-2.2.1/.deepsource.toml
+-rw-r--r--   0 shaypalachy   (501) staff       (20)       30 2021-10-10 23:14:34.000000 cachier-2.2.1/.fdignore
+-rw-r--r--   0 shaypalachy   (501) staff       (20)      202 2022-12-02 11:10:23.000000 cachier-2.2.1/.flake8
+-rw-r--r--   0 shaypalachy   (501) staff       (20)       33 2021-06-17 12:08:06.000000 cachier-2.2.1/.gitattributes
+drwxr-xr-x   0 shaypalachy   (501) staff       (20)        0 2023-07-02 09:23:49.119253 cachier-2.2.1/.github/
+drwxr-xr-x   0 shaypalachy   (501) staff       (20)        0 2023-07-02 09:23:49.135205 cachier-2.2.1/.github/workflows/
+-rw-r--r--   0 shaypalachy   (501) staff       (20)      680 2023-03-16 11:40:57.000000 cachier-2.2.1/.github/workflows/checkdocs.yml
+-rw-r--r--   0 shaypalachy   (501) staff       (20)      775 2023-06-30 12:48:49.000000 cachier-2.2.1/.github/workflows/lint.yml
+-rw-r--r--   0 shaypalachy   (501) staff       (20)      981 2023-06-30 12:48:49.000000 cachier-2.2.1/.github/workflows/test.yml
+-rw-r--r--   0 shaypalachy   (501) staff       (20)     1249 2021-06-17 12:08:06.000000 cachier-2.2.1/.gitignore
+-rw-r--r--   0 shaypalachy   (501) staff       (20)       67 2022-12-02 11:08:24.000000 cachier-2.2.1/.ignore
+-rw-r--r--   0 shaypalachy   (501) staff       (20)     8489 2021-10-10 23:14:34.000000 cachier-2.2.1/.pylintrc
+-rw-r--r--   0 shaypalachy   (501) staff       (20)     1069 2021-06-17 12:08:06.000000 cachier-2.2.1/LICENSE
+-rw-r--r--   0 shaypalachy   (501) staff       (20)       50 2021-06-17 12:08:06.000000 cachier-2.2.1/MANIFEST.in
+-rw-r--r--   0 shaypalachy   (501) staff       (20)    17490 2023-07-02 09:23:49.150039 cachier-2.2.1/PKG-INFO
+-rw-r--r--   0 shaypalachy   (501) staff       (20)    16447 2023-06-30 12:49:12.000000 cachier-2.2.1/README.rst
+drwxr-xr-x   0 shaypalachy   (501) staff       (20)        0 2023-07-02 09:23:49.151632 cachier-2.2.1/cachier/
+-rw-r--r--   0 shaypalachy   (501) staff       (20)      232 2023-04-09 05:18:24.000000 cachier-2.2.1/cachier/__init__.py
+-rw-r--r--   0 shaypalachy   (501) staff       (20)      471 2023-07-02 09:23:49.151725 cachier-2.2.1/cachier/_version.py
+-rw-r--r--   0 shaypalachy   (501) staff       (20)     3062 2023-04-09 05:18:24.000000 cachier-2.2.1/cachier/base_core.py
+-rw-r--r--   0 shaypalachy   (501) staff       (20)    14548 2023-07-02 09:22:38.000000 cachier-2.2.1/cachier/core.py
+-rw-r--r--   0 shaypalachy   (501) staff       (20)     2846 2023-04-09 05:18:24.000000 cachier-2.2.1/cachier/memory_core.py
+-rw-r--r--   0 shaypalachy   (501) staff       (20)     5022 2023-04-09 05:18:24.000000 cachier-2.2.1/cachier/mongo_core.py
+-rw-r--r--   0 shaypalachy   (501) staff       (20)    10068 2023-04-09 05:18:24.000000 cachier-2.2.1/cachier/pickle_core.py
+-rw-r--r--   0 shaypalachy   (501) staff       (20)        0 2023-06-30 12:48:49.000000 cachier-2.2.1/cachier/py.typed
+drwxr-xr-x   0 shaypalachy   (501) staff       (20)        0 2023-07-02 09:23:49.143854 cachier-2.2.1/cachier/scripts/
+-rw-r--r--   0 shaypalachy   (501) staff       (20)        0 2021-06-17 12:08:06.000000 cachier-2.2.1/cachier/scripts/__init__.py
+-rw-r--r--   0 shaypalachy   (501) staff       (20)      429 2021-06-17 12:08:06.000000 cachier-2.2.1/cachier/scripts/cli.py
+drwxr-xr-x   0 shaypalachy   (501) staff       (20)        0 2023-07-02 09:23:49.142787 cachier-2.2.1/cachier.egg-info/
+-rw-r--r--   0 shaypalachy   (501) staff       (20)    17490 2023-07-02 09:23:48.000000 cachier-2.2.1/cachier.egg-info/PKG-INFO
+-rw-r--r--   0 shaypalachy   (501) staff       (20)      932 2023-07-02 09:23:48.000000 cachier-2.2.1/cachier.egg-info/SOURCES.txt
+-rw-r--r--   0 shaypalachy   (501) staff       (20)        1 2023-07-02 09:23:48.000000 cachier-2.2.1/cachier.egg-info/dependency_links.txt
+-rw-r--r--   0 shaypalachy   (501) staff       (20)       52 2023-07-02 09:23:48.000000 cachier-2.2.1/cachier.egg-info/entry_points.txt
+-rw-r--r--   0 shaypalachy   (501) staff       (20)      220 2023-07-02 09:23:48.000000 cachier-2.2.1/cachier.egg-info/requires.txt
+-rw-r--r--   0 shaypalachy   (501) staff       (20)        8 2023-07-02 09:23:48.000000 cachier-2.2.1/cachier.egg-info/top_level.txt
+-rw-r--r--   0 shaypalachy   (501) staff       (20)      227 2023-06-30 12:48:49.000000 cachier-2.2.1/mypy.ini
+-rw-r--r--   0 shaypalachy   (501) staff       (20)      308 2023-04-09 05:18:24.000000 cachier-2.2.1/pytest.ini
+-rw-r--r--   0 shaypalachy   (501) staff       (20)      269 2023-07-02 09:23:49.151233 cachier-2.2.1/setup.cfg
+-rw-r--r--   0 shaypalachy   (501) staff       (20)     2615 2023-06-30 12:48:49.000000 cachier-2.2.1/setup.py
+drwxr-xr-x   0 shaypalachy   (501) staff       (20)        0 2023-07-02 09:23:49.149383 cachier-2.2.1/tests/
+-rw-r--r--   0 shaypalachy   (501) staff       (20)        0 2021-06-17 12:08:06.000000 cachier-2.2.1/tests/__init__.py
+-rw-r--r--   0 shaypalachy   (501) staff       (20)     1903 2023-03-22 22:40:25.000000 cachier-2.2.1/tests/speed_eval.py
+-rw-r--r--   0 shaypalachy   (501) staff       (20)      168 2023-03-31 07:33:42.000000 cachier-2.2.1/tests/standalone_script.py
+-rw-r--r--   0 shaypalachy   (501) staff       (20)     1122 2023-06-30 12:49:12.000000 cachier-2.2.1/tests/test_core_lookup.py
+-rw-r--r--   0 shaypalachy   (501) staff       (20)     6545 2023-06-30 12:49:12.000000 cachier-2.2.1/tests/test_defaults.py
+-rw-r--r--   0 shaypalachy   (501) staff       (20)     7272 2023-06-30 12:49:12.000000 cachier-2.2.1/tests/test_general.py
+-rw-r--r--   0 shaypalachy   (501) staff       (20)     8879 2023-03-31 07:33:42.000000 cachier-2.2.1/tests/test_memory_core.py
+-rw-r--r--   0 shaypalachy   (501) staff       (20)     8963 2023-06-30 12:48:49.000000 cachier-2.2.1/tests/test_mongo_core.py
+-rw-r--r--   0 shaypalachy   (501) staff       (20)    18211 2023-06-30 12:48:49.000000 cachier-2.2.1/tests/test_pickle_core.py
+-rw-r--r--   0 shaypalachy   (501) staff       (20)      482 2023-03-22 22:40:25.000000 cachier-2.2.1/tests/test_quality.py
+-rw-r--r--   0 shaypalachy   (501) staff       (20)      577 2023-03-22 22:40:25.000000 cachier-2.2.1/tests/test_security.py
+-rw-r--r--   0 shaypalachy   (501) staff       (20)    65788 2023-06-30 12:48:49.000000 cachier-2.2.1/versioneer.py
```

### Comparing `cachier-2.2.0/.github/workflows/checkdocs.yml` & `cachier-2.2.1/.github/workflows/checkdocs.yml`

 * *Files identical despite different names*

### Comparing `cachier-2.2.0/.github/workflows/lint.yml` & `cachier-2.2.1/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `cachier-2.2.0/.github/workflows/test.yml` & `cachier-2.2.1/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `cachier-2.2.0/.gitignore` & `cachier-2.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `cachier-2.2.0/.pylintrc` & `cachier-2.2.1/.pylintrc`

 * *Files identical despite different names*

### Comparing `cachier-2.2.0/LICENSE` & `cachier-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cachier-2.2.0/PKG-INFO` & `cachier-2.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cachier
-Version: 2.2.0
+Version: 2.2.1
 Summary: Persistent, stale-free, local and cross-machine caching for Python functions.
 Home-page: https://github.com/python-cachier/cachier
 Author: Shay Palachy
 Author-email: shay.palachy@gmail.com
 License: MIT
 Keywords: cache,persistence,mongo,memoization,decorator
 Platform: linux
```

### Comparing `cachier-2.2.0/README.rst` & `cachier-2.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `cachier-2.2.0/cachier/base_core.py` & `cachier-2.2.1/cachier/base_core.py`

 * *Files identical despite different names*

### Comparing `cachier-2.2.0/cachier/core.py` & `cachier-2.2.1/cachier/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,24 +13,26 @@
 import datetime
 import functools
 import hashlib
 import os
 import pickle
 from concurrent.futures import ThreadPoolExecutor
 from functools import wraps
-from typing import Callable, Literal, Optional, TypedDict, Union
+from typing import TYPE_CHECKING, Callable, Literal, Optional, TypedDict, Union
 from warnings import warn
 
-from pymongo.collection import Collection
-
 from .base_core import RecalculationNeeded, _BaseCore
 from .memory_core import _MemoryCore
 from .mongo_core import _MongoCore
 from .pickle_core import _PickleCore
 
+if TYPE_CHECKING:
+    import pymongo.collection
+
+
 MAX_WORKERS_ENVAR_NAME = 'CACHIER_MAX_WORKERS'
 DEFAULT_MAX_WORKERS = 8
 
 
 def _max_workers():
     try:
         return int(os.environ[MAX_WORKERS_ENVAR_NAME])
@@ -88,15 +90,15 @@
 
 
 class MissingMongetter(ValueError):
     """Thrown when the mongetter keyword argument is missing."""
 
 
 HashFunc = Callable[..., str]
-Mongetter = Callable[[], Collection]
+Mongetter = Callable[[], "pymongo.collection.Collection"]
 Backend = Literal["pickle", "mongo", "memory"]
 
 
 class Params(TypedDict):
     caching_enabled: bool
     hash_func: HashFunc
     backend: Backend
```

### Comparing `cachier-2.2.0/cachier/memory_core.py` & `cachier-2.2.1/cachier/memory_core.py`

 * *Files identical despite different names*

### Comparing `cachier-2.2.0/cachier/mongo_core.py` & `cachier-2.2.1/cachier/mongo_core.py`

 * *Files identical despite different names*

### Comparing `cachier-2.2.0/cachier/pickle_core.py` & `cachier-2.2.1/cachier/pickle_core.py`

 * *Files identical despite different names*

### Comparing `cachier-2.2.0/cachier.egg-info/PKG-INFO` & `cachier-2.2.1/cachier.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cachier
-Version: 2.2.0
+Version: 2.2.1
 Summary: Persistent, stale-free, local and cross-machine caching for Python functions.
 Home-page: https://github.com/python-cachier/cachier
 Author: Shay Palachy
 Author-email: shay.palachy@gmail.com
 License: MIT
 Keywords: cache,persistence,mongo,memoization,decorator
 Platform: linux
```

### Comparing `cachier-2.2.0/cachier.egg-info/SOURCES.txt` & `cachier-2.2.1/cachier.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cachier-2.2.0/setup.py` & `cachier-2.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `cachier-2.2.0/tests/speed_eval.py` & `cachier-2.2.1/tests/speed_eval.py`

 * *Files identical despite different names*

### Comparing `cachier-2.2.0/tests/test_core_lookup.py` & `cachier-2.2.1/tests/test_core_lookup.py`

 * *Files identical despite different names*

### Comparing `cachier-2.2.0/tests/test_defaults.py` & `cachier-2.2.1/tests/test_defaults.py`

 * *Files identical despite different names*

### Comparing `cachier-2.2.0/tests/test_general.py` & `cachier-2.2.1/tests/test_general.py`

 * *Files identical despite different names*

### Comparing `cachier-2.2.0/tests/test_memory_core.py` & `cachier-2.2.1/tests/test_memory_core.py`

 * *Files identical despite different names*

### Comparing `cachier-2.2.0/tests/test_mongo_core.py` & `cachier-2.2.1/tests/test_mongo_core.py`

 * *Files identical despite different names*

### Comparing `cachier-2.2.0/tests/test_pickle_core.py` & `cachier-2.2.1/tests/test_pickle_core.py`

 * *Files identical despite different names*

### Comparing `cachier-2.2.0/tests/test_security.py` & `cachier-2.2.1/tests/test_security.py`

 * *Files identical despite different names*

### Comparing `cachier-2.2.0/versioneer.py` & `cachier-2.2.1/versioneer.py`

 * *Files identical despite different names*

