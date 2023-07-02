# Comparing `tmp/alchemiscale-0.1.2.tar.gz` & `tmp/alchemiscale-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alchemiscale-0.1.2.tar", last modified: Sun Apr 23 04:25:24 2023, max compression
+gzip compressed data, was "alchemiscale-0.1.3.tar", last modified: Sun Jul  2 03:12:12 2023, max compression
```

## Comparing `alchemiscale-0.1.2.tar` & `alchemiscale-0.1.3.tar`

### file list

```diff
@@ -1,51 +1,48 @@
-drwxr-xr-x   0 david     (1001) david     (1001)        0 2023-04-23 04:25:24.946013 alchemiscale-0.1.2/
--rw-r--r--   0 david     (1001) david     (1001)     1084 2022-02-15 17:06:19.000000 alchemiscale-0.1.2/LICENSE
--rw-r--r--   0 david     (1001) david     (1001)       55 2023-02-15 05:25:44.000000 alchemiscale-0.1.2/MANIFEST.in
--rw-r--r--   0 david     (1001) david     (1001)     1195 2023-04-23 04:25:24.946013 alchemiscale-0.1.2/PKG-INFO
--rw-r--r--   0 david     (1001) david     (1001)      610 2023-03-23 07:15:07.000000 alchemiscale-0.1.2/README.md
-drwxr-xr-x   0 david     (1001) david     (1001)        0 2023-04-23 04:25:24.946013 alchemiscale-0.1.2/alchemiscale/
--rw-r--r--   0 david     (1001) david     (1001)      153 2023-02-15 05:25:44.000000 alchemiscale-0.1.2/alchemiscale/__init__.py
--rw-r--r--   0 david     (1001) david     (1001)      498 2023-04-23 04:25:24.946013 alchemiscale-0.1.2/alchemiscale/_version.py
-drwxr-xr-x   0 david     (1001) david     (1001)        0 2023-04-23 04:25:24.939346 alchemiscale-0.1.2/alchemiscale/base/
--rw-r--r--   0 david     (1001) david     (1001)        0 2023-04-18 06:27:03.000000 alchemiscale-0.1.2/alchemiscale/base/__init__.py
--rw-r--r--   0 david     (1001) david     (1001)     6804 2023-04-17 19:03:58.000000 alchemiscale-0.1.2/alchemiscale/base/api.py
--rw-r--r--   0 david     (1001) david     (1001)     8197 2023-04-17 19:03:58.000000 alchemiscale-0.1.2/alchemiscale/base/client.py
--rw-r--r--   0 david     (1001) david     (1001)    17195 2023-04-17 19:03:58.000000 alchemiscale-0.1.2/alchemiscale/cli.py
--rw-r--r--   0 david     (1001) david     (1001)      929 2023-04-17 19:03:58.000000 alchemiscale-0.1.2/alchemiscale/cli_utils.py
-drwxr-xr-x   0 david     (1001) david     (1001)        0 2023-04-23 04:25:24.939346 alchemiscale-0.1.2/alchemiscale/compute/
--rw-r--r--   0 david     (1001) david     (1001)       46 2023-02-15 05:25:44.000000 alchemiscale-0.1.2/alchemiscale/compute/__init__.py
--rw-r--r--   0 david     (1001) david     (1001)     7369 2023-04-19 19:27:01.000000 alchemiscale-0.1.2/alchemiscale/compute/api.py
--rw-r--r--   0 david     (1001) david     (1001)     3699 2023-04-19 18:53:57.000000 alchemiscale-0.1.2/alchemiscale/compute/client.py
--rw-r--r--   0 david     (1001) david     (1001)    16905 2023-04-22 03:05:51.000000 alchemiscale-0.1.2/alchemiscale/compute/service.py
-drwxr-xr-x   0 david     (1001) david     (1001)        0 2023-04-23 04:25:24.942679 alchemiscale-0.1.2/alchemiscale/interface/
--rw-r--r--   0 david     (1001) david     (1001)       39 2023-02-15 05:25:44.000000 alchemiscale-0.1.2/alchemiscale/interface/__init__.py
--rw-r--r--   0 david     (1001) david     (1001)    13870 2023-04-17 19:03:58.000000 alchemiscale-0.1.2/alchemiscale/interface/api.py
--rw-r--r--   0 david     (1001) david     (1001)    18306 2023-04-19 20:37:27.000000 alchemiscale-0.1.2/alchemiscale/interface/client.py
--rw-r--r--   0 david     (1001) david     (1001)     5712 2023-04-16 23:49:41.000000 alchemiscale-0.1.2/alchemiscale/models.py
-drwxr-xr-x   0 david     (1001) david     (1001)        0 2023-04-23 04:25:24.942679 alchemiscale-0.1.2/alchemiscale/security/
--rw-r--r--   0 david     (1001) david     (1001)        0 2023-04-14 20:41:38.000000 alchemiscale-0.1.2/alchemiscale/security/__init__.py
--rw-r--r--   0 david     (1001) david     (1001)     2036 2023-04-16 23:49:41.000000 alchemiscale-0.1.2/alchemiscale/security/auth.py
--rw-r--r--   0 david     (1001) david     (1001)     1565 2023-04-16 23:49:41.000000 alchemiscale-0.1.2/alchemiscale/security/models.py
--rw-r--r--   0 david     (1001) david     (1001)     2552 2023-04-16 23:49:41.000000 alchemiscale-0.1.2/alchemiscale/settings.py
-drwxr-xr-x   0 david     (1001) david     (1001)        0 2023-04-23 04:25:24.946013 alchemiscale-0.1.2/alchemiscale/storage/
--rw-r--r--   0 david     (1001) david     (1001)        0 2023-04-14 20:41:38.000000 alchemiscale-0.1.2/alchemiscale/storage/__init__.py
--rw-r--r--   0 david     (1001) david     (1001)     7000 2023-04-19 19:27:27.000000 alchemiscale-0.1.2/alchemiscale/storage/models.py
--rw-r--r--   0 david     (1001) david     (1001)     8921 2023-04-19 19:26:45.000000 alchemiscale-0.1.2/alchemiscale/storage/objectstore.py
--rw-r--r--   0 david     (1001) david     (1001)    69559 2023-04-17 00:02:33.000000 alchemiscale-0.1.2/alchemiscale/storage/statestore.py
-drwxr-xr-x   0 david     (1001) david     (1001)        0 2023-04-23 04:25:24.946013 alchemiscale-0.1.2/alchemiscale/strategies/
--rw-r--r--   0 david     (1001) david     (1001)       27 2023-02-15 05:25:44.000000 alchemiscale-0.1.2/alchemiscale/strategies/__init__.py
--rw-r--r--   0 david     (1001) david     (1001)      371 2023-04-16 23:49:41.000000 alchemiscale-0.1.2/alchemiscale/strategies/base.py
-drwxr-xr-x   0 david     (1001) david     (1001)        0 2023-04-23 04:25:24.946013 alchemiscale-0.1.2/alchemiscale/strategist/
--rw-r--r--   0 david     (1001) david     (1001)        0 2023-04-18 06:27:53.000000 alchemiscale-0.1.2/alchemiscale/strategist/__init__.py
--rw-r--r--   0 david     (1001) david     (1001)      213 2023-04-16 23:49:41.000000 alchemiscale-0.1.2/alchemiscale/strategist/service.py
-drwxr-xr-x   0 david     (1001) david     (1001)        0 2023-04-23 04:25:24.936013 alchemiscale-0.1.2/alchemiscale.egg-info/
--rw-r--r--   0 david     (1001) david     (1001)     1195 2023-04-23 04:25:24.000000 alchemiscale-0.1.2/alchemiscale.egg-info/PKG-INFO
--rw-r--r--   0 david     (1001) david     (1001)     1134 2023-04-23 04:25:24.000000 alchemiscale-0.1.2/alchemiscale.egg-info/SOURCES.txt
--rw-r--r--   0 david     (1001) david     (1001)        1 2023-04-23 04:25:24.000000 alchemiscale-0.1.2/alchemiscale.egg-info/dependency_links.txt
--rw-r--r--   0 david     (1001) david     (1001)       54 2023-04-23 04:25:24.000000 alchemiscale-0.1.2/alchemiscale.egg-info/entry_points.txt
--rw-r--r--   0 david     (1001) david     (1001)        1 2023-04-23 04:25:24.000000 alchemiscale-0.1.2/alchemiscale.egg-info/not-zip-safe
--rw-r--r--   0 david     (1001) david     (1001)       28 2023-04-23 04:25:24.000000 alchemiscale-0.1.2/alchemiscale.egg-info/requires.txt
--rw-r--r--   0 david     (1001) david     (1001)       13 2023-04-23 04:25:24.000000 alchemiscale-0.1.2/alchemiscale.egg-info/top_level.txt
--rw-r--r--   0 david     (1001) david     (1001)     1052 2023-04-23 04:25:24.946013 alchemiscale-0.1.2/setup.cfg
--rw-r--r--   0 david     (1001) david     (1001)      136 2022-11-18 18:18:33.000000 alchemiscale-0.1.2/setup.py
--rw-r--r--   0 david     (1001) david     (1001)    81180 2023-03-16 05:35:03.000000 alchemiscale-0.1.2/versioneer.py
+drwxr-xr-x   0 david     (1001) david     (1001)        0 2023-07-02 03:12:12.417745 alchemiscale-0.1.3/
+-rw-r--r--   0 david     (1001) david     (1001)     1084 2022-02-15 17:06:19.000000 alchemiscale-0.1.3/LICENSE
+-rw-r--r--   0 david     (1001) david     (1001)     1247 2023-07-02 03:12:12.417745 alchemiscale-0.1.3/PKG-INFO
+-rw-r--r--   0 david     (1001) david     (1001)      610 2023-03-23 07:15:07.000000 alchemiscale-0.1.3/README.md
+drwxr-xr-x   0 david     (1001) david     (1001)        0 2023-07-02 03:12:12.411079 alchemiscale-0.1.3/alchemiscale/
+-rw-r--r--   0 david     (1001) david     (1001)      158 2023-06-30 16:23:14.000000 alchemiscale-0.1.3/alchemiscale/__init__.py
+drwxr-xr-x   0 david     (1001) david     (1001)        0 2023-07-02 03:12:12.411079 alchemiscale-0.1.3/alchemiscale/base/
+-rw-r--r--   0 david     (1001) david     (1001)        0 2023-04-18 06:27:03.000000 alchemiscale-0.1.3/alchemiscale/base/__init__.py
+-rw-r--r--   0 david     (1001) david     (1001)     8089 2023-06-30 16:23:14.000000 alchemiscale-0.1.3/alchemiscale/base/api.py
+-rw-r--r--   0 david     (1001) david     (1001)    16777 2023-06-30 16:23:14.000000 alchemiscale-0.1.3/alchemiscale/base/client.py
+-rw-r--r--   0 david     (1001) david     (1001)    17195 2023-04-17 19:03:58.000000 alchemiscale-0.1.3/alchemiscale/cli.py
+-rw-r--r--   0 david     (1001) david     (1001)      929 2023-04-17 19:03:58.000000 alchemiscale-0.1.3/alchemiscale/cli_utils.py
+drwxr-xr-x   0 david     (1001) david     (1001)        0 2023-07-02 03:12:12.414412 alchemiscale-0.1.3/alchemiscale/compute/
+-rw-r--r--   0 david     (1001) david     (1001)       46 2023-02-15 05:25:44.000000 alchemiscale-0.1.3/alchemiscale/compute/__init__.py
+-rw-r--r--   0 david     (1001) david     (1001)     7537 2023-06-30 16:23:14.000000 alchemiscale-0.1.3/alchemiscale/compute/api.py
+-rw-r--r--   0 david     (1001) david     (1001)     3699 2023-06-03 01:14:25.000000 alchemiscale-0.1.3/alchemiscale/compute/client.py
+-rw-r--r--   0 david     (1001) david     (1001)    17113 2023-06-30 16:23:14.000000 alchemiscale-0.1.3/alchemiscale/compute/service.py
+drwxr-xr-x   0 david     (1001) david     (1001)        0 2023-07-02 03:12:12.414412 alchemiscale-0.1.3/alchemiscale/interface/
+-rw-r--r--   0 david     (1001) david     (1001)       39 2023-02-15 05:25:44.000000 alchemiscale-0.1.3/alchemiscale/interface/__init__.py
+-rw-r--r--   0 david     (1001) david     (1001)    22202 2023-06-30 16:23:14.000000 alchemiscale-0.1.3/alchemiscale/interface/api.py
+-rw-r--r--   0 david     (1001) david     (1001)    37140 2023-06-30 16:23:14.000000 alchemiscale-0.1.3/alchemiscale/interface/client.py
+-rw-r--r--   0 david     (1001) david     (1001)     5925 2023-06-30 16:23:14.000000 alchemiscale-0.1.3/alchemiscale/models.py
+drwxr-xr-x   0 david     (1001) david     (1001)        0 2023-07-02 03:12:12.414412 alchemiscale-0.1.3/alchemiscale/security/
+-rw-r--r--   0 david     (1001) david     (1001)        0 2023-04-14 20:41:38.000000 alchemiscale-0.1.3/alchemiscale/security/__init__.py
+-rw-r--r--   0 david     (1001) david     (1001)     2037 2023-06-30 16:23:14.000000 alchemiscale-0.1.3/alchemiscale/security/auth.py
+-rw-r--r--   0 david     (1001) david     (1001)     1565 2023-04-16 23:49:41.000000 alchemiscale-0.1.3/alchemiscale/security/models.py
+-rw-r--r--   0 david     (1001) david     (1001)     2552 2023-04-16 23:49:41.000000 alchemiscale-0.1.3/alchemiscale/settings.py
+drwxr-xr-x   0 david     (1001) david     (1001)        0 2023-07-02 03:12:12.414412 alchemiscale-0.1.3/alchemiscale/storage/
+-rw-r--r--   0 david     (1001) david     (1001)        0 2023-04-14 20:41:38.000000 alchemiscale-0.1.3/alchemiscale/storage/__init__.py
+-rw-r--r--   0 david     (1001) david     (1001)     7000 2023-04-19 19:27:27.000000 alchemiscale-0.1.3/alchemiscale/storage/models.py
+-rw-r--r--   0 david     (1001) david     (1001)     8921 2023-04-19 19:26:45.000000 alchemiscale-0.1.3/alchemiscale/storage/objectstore.py
+-rw-r--r--   0 david     (1001) david     (1001)    76684 2023-06-30 16:23:14.000000 alchemiscale-0.1.3/alchemiscale/storage/statestore.py
+drwxr-xr-x   0 david     (1001) david     (1001)        0 2023-07-02 03:12:12.417745 alchemiscale-0.1.3/alchemiscale/strategies/
+-rw-r--r--   0 david     (1001) david     (1001)       27 2023-02-15 05:25:44.000000 alchemiscale-0.1.3/alchemiscale/strategies/__init__.py
+-rw-r--r--   0 david     (1001) david     (1001)      371 2023-04-16 23:49:41.000000 alchemiscale-0.1.3/alchemiscale/strategies/base.py
+drwxr-xr-x   0 david     (1001) david     (1001)        0 2023-07-02 03:12:12.417745 alchemiscale-0.1.3/alchemiscale/strategist/
+-rw-r--r--   0 david     (1001) david     (1001)        0 2023-04-18 06:27:53.000000 alchemiscale-0.1.3/alchemiscale/strategist/__init__.py
+-rw-r--r--   0 david     (1001) david     (1001)      213 2023-04-16 23:49:41.000000 alchemiscale-0.1.3/alchemiscale/strategist/service.py
+drwxr-xr-x   0 david     (1001) david     (1001)        0 2023-07-02 03:12:12.411079 alchemiscale-0.1.3/alchemiscale.egg-info/
+-rw-r--r--   0 david     (1001) david     (1001)     1247 2023-07-02 03:12:12.000000 alchemiscale-0.1.3/alchemiscale.egg-info/PKG-INFO
+-rw-r--r--   0 david     (1001) david     (1001)     1079 2023-07-02 03:12:12.000000 alchemiscale-0.1.3/alchemiscale.egg-info/SOURCES.txt
+-rw-r--r--   0 david     (1001) david     (1001)        1 2023-07-02 03:12:12.000000 alchemiscale-0.1.3/alchemiscale.egg-info/dependency_links.txt
+-rw-r--r--   0 david     (1001) david     (1001)       54 2023-07-02 03:12:12.000000 alchemiscale-0.1.3/alchemiscale.egg-info/entry_points.txt
+-rw-r--r--   0 david     (1001) david     (1001)        1 2023-04-23 04:25:24.000000 alchemiscale-0.1.3/alchemiscale.egg-info/not-zip-safe
+-rw-r--r--   0 david     (1001) david     (1001)       28 2023-07-02 03:12:12.000000 alchemiscale-0.1.3/alchemiscale.egg-info/requires.txt
+-rw-r--r--   0 david     (1001) david     (1001)       13 2023-07-02 03:12:12.000000 alchemiscale-0.1.3/alchemiscale.egg-info/top_level.txt
+-rw-r--r--   0 david     (1001) david     (1001)     1714 2023-06-30 16:23:14.000000 alchemiscale-0.1.3/pyproject.toml
+-rw-r--r--   0 david     (1001) david     (1001)       38 2023-07-02 03:12:12.417745 alchemiscale-0.1.3/setup.cfg
```

### Comparing `alchemiscale-0.1.2/LICENSE` & `alchemiscale-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `alchemiscale-0.1.2/PKG-INFO` & `alchemiscale-0.1.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: alchemiscale
-Version: 0.1.2
-Home-page: https://github.com/openforcefield/alchemiscale
+Version: 0.1.3
 Author: OpenFE and OpenFF developers
 License: MIT
+Project-URL: Homepage, https://github.com/openforcefield/alchemiscale
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Requires-Python: >=3.9
+Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 # alchemiscale
 
 [![build](https://github.com/openforcefield/alchemiscale/actions/workflows/ci-integration.yml/badge.svg)](https://github.com/openforcefield/alchemiscale/actions/workflows/ci-integration.yml)
 [![coverage](https://codecov.io/gh/openforcefield/alchemiscale/branch/main/graph/badge.svg)](https://codecov.io/gh/openforcefield/alchemiscale)
```

### Comparing `alchemiscale-0.1.2/README.md` & `alchemiscale-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `alchemiscale-0.1.2/alchemiscale/base/api.py` & `alchemiscale-0.1.3/alchemiscale/base/api.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,20 +2,22 @@
 Reusable components for API services. --- :mod:`alchemiscale.base.api`
 ======================================================================
 
 """
 
 
 from functools import lru_cache
-from typing import Any, Union, Dict, List
+from typing import Any, Union, Dict, List, Callable
 import os
 import json
+import gzip
 
 from starlette.responses import JSONResponse
-from fastapi import APIRouter, Depends, HTTPException, status
+from fastapi import APIRouter, Depends, HTTPException, status, Request, Response
+from fastapi.routing import APIRoute
 from fastapi.security import OAuth2PasswordRequestForm
 from py2neo import Graph
 from gufe import AlchemicalNetwork, ChemicalSystem, Transformation
 from gufe.tokenization import JSON_HANDLER, GufeTokenizable
 
 from ..settings import (
     JWTSettings,
@@ -50,37 +52,53 @@
             detail=(
                 f"Targeted scope '{scope}' not accessible via scopes for this identity: {token.scopes}."
             ),
             headers={"WWW-Authenticate": "Bearer"},
         )
 
 
+def minimize_scope_space(scopes: List[Scope]) -> List[Scope]:
+    """Remove redundant Scopes from a list of Scopes."""
+    scopes = sorted(scopes)
+
+    minimal_scope_space = []
+    for scope in scopes:
+        if not any(
+            other_scope.is_superset(scope) for other_scope in minimal_scope_space
+        ):
+            minimal_scope_space.append(scope)
+
+    return minimal_scope_space
+
+
 def validate_scopes_query(
     query_scope: Scope, token: TokenData, as_str: bool = False
 ) -> Union[list[Scope], list[str]]:
     """
     Create the intersection of queried scopes and token, where query scopes may include 'all' / wildcard (`None`).
     No scopes outside of those included in token will be included in scopes returned.
 
     If as_str is True, returns a list of str rather than list of Scopes.
 
     """
+    token_scopes = sorted({Scope.from_str(ts) for ts in token.scopes})
 
-    token_scopes = [Scope.from_str(ts) for ts in token.scopes]
-
-    # we want to return all (and only) authorized token scopes that fall within
-    # the query_scope
-    scope_space = {ts for ts in token_scopes if query_scope.is_superset(ts)}
+    # start by minimizing the scope space
+    token_scope_space = minimize_scope_space(token_scopes)
 
-    # we also want to return the query_scope if it is a subset of any of the
+    # we just want to return the query_scope if it is a subset of any of the
     # authorized token scopes
-    if any([Scope.from_str(ts).is_superset(query_scope) for ts in token.scopes]):
-        scope_space.add(query_scope)
-
-    scope_space = list(scope_space)
+    if any([scope.is_superset(query_scope) for scope in token_scope_space]):
+        scope_space = [query_scope]
+    else:
+        # otherwise, we want to return all (and only) authorized token scopes
+        # that fall within the query_scope
+        scope_space = [
+            scope for scope in token_scope_space if query_scope.is_superset(scope)
+        ]
 
     if as_str:
         scope_space = [str(s) for s in scope_space]
     return scope_space
 
 
 def gufe_to_json(obj: GufeTokenizable):
@@ -126,14 +144,35 @@
 class GufeJSONResponse(JSONResponse):
     media_type = "application/json"
 
     def render(self, content: Any) -> bytes:
         return json.dumps(content, cls=JSON_HANDLER.encoder).encode("utf-8")
 
 
+class GzipRequest(Request):
+    async def body(self) -> bytes:
+        if not hasattr(self, "_body"):
+            body = await super().body()
+            if "gzip" in self.headers.getlist("Content-Encoding"):
+                body = gzip.decompress(body)
+            self._body = body
+        return self._body
+
+
+class GzipRoute(APIRoute):
+    def get_route_handler(self) -> Callable:
+        original_route_handler = super().get_route_handler()
+
+        async def custom_route_handler(request: Request) -> Response:
+            request = GzipRequest(request.scope, request.receive)
+            return await original_route_handler(request)
+
+        return custom_route_handler
+
+
 def scope_params(org: str = None, campaign: str = None, project: str = None):
     try:
         return Scope(org=org, campaign=campaign, project=project)
     except (AttributeError, ValueError):
         raise HTTPException(
             status_code=status.HTTP_400_BAD_REQUEST,
             detail=(
```

### Comparing `alchemiscale-0.1.2/alchemiscale/cli.py` & `alchemiscale-0.1.3/alchemiscale/cli.py`

 * *Files identical despite different names*

### Comparing `alchemiscale-0.1.2/alchemiscale/cli_utils.py` & `alchemiscale-0.1.3/alchemiscale/cli_utils.py`

 * *Files identical despite different names*

### Comparing `alchemiscale-0.1.2/alchemiscale/compute/api.py` & `alchemiscale-0.1.3/alchemiscale/compute/api.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 from typing import Any, Dict, List, Optional
 import os
 import json
 from datetime import datetime, timedelta
 
 from fastapi import FastAPI, APIRouter, Body, Depends, HTTPException, status
+from fastapi.middleware.gzip import GZipMiddleware
 from gufe.tokenization import GufeTokenizable, JSON_HANDLER
 
 from ..base.api import (
     GufeJSONResponse,
     QueryGUFEHandler,
     scope_params,
     get_token_data_depends,
@@ -21,14 +22,15 @@
     get_s3os_depends,
     base_router,
     get_cred_entity,
     validate_scopes,
     validate_scopes_query,
     _check_store_connectivity,
     gufe_to_json,
+    GzipRoute,
 )
 from ..settings import (
     get_base_api_settings,
     get_compute_api_settings,
     ComputeAPISettings,
 )
 from ..storage.statestore import Neo4jStore, get_n4js
@@ -47,26 +49,28 @@
     CredentialedComputeIdentity,
 )
 
 
 app = FastAPI(title="AlchemiscaleComputeAPI")
 app.dependency_overrides[get_base_api_settings] = get_compute_api_settings
 app.include_router(base_router)
+app.add_middleware(GZipMiddleware, minimum_size=1000, compresslevel=5)
 
 
 def get_cred_compute():
     return CredentialedComputeIdentity
 
 
 app.dependency_overrides[get_cred_entity] = get_cred_compute
 
 
 router = APIRouter(
     dependencies=[Depends(get_token_data_depends)],
 )
+router.route_class = GzipRoute
 
 
 @app.get("/ping")
 def ping():
     return {"api": "AlchemiscaleComputeAPI"}
```

### Comparing `alchemiscale-0.1.2/alchemiscale/compute/client.py` & `alchemiscale-0.1.3/alchemiscale/compute/client.py`

 * *Files identical despite different names*

### Comparing `alchemiscale-0.1.2/alchemiscale/compute/service.py` & `alchemiscale-0.1.3/alchemiscale/compute/service.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,14 +88,15 @@
         scopes: Optional[List[Scope]] = None,
         claim_limit: int = 1,
         loglevel="WARN",
         logfile: Optional[Path] = None,
         client_max_retries=5,
         client_retry_base_seconds=2.0,
         client_retry_max_seconds=60.0,
+        client_verify=True,
     ):
         """Create a `SynchronousComputeService` instance.
 
         Parameters
         ----------
         api_url
             URL of the compute API to execute Tasks for.
@@ -139,29 +140,32 @@
             continue indefinitely until success.
         client_retry_base_seconds
             The base number of seconds to use for exponential backoff.
             Must be greater than 1.0.
         client_retry_max_seconds
             Maximum number of seconds to sleep between retries; avoids runaway
             exponential backoff while allowing for many retries.
+        client_verify
+            Whether to verify SSL certificate presented by the API server.
 
         """
         self.api_url = api_url
         self.name = name
         self.sleep_interval = sleep_interval
         self.heartbeat_interval = heartbeat_interval
         self.claim_limit = claim_limit
 
         self.client = AlchemiscaleComputeClient(
             api_url,
             identifier,
             key,
-            client_max_retries,
-            client_retry_base_seconds,
-            client_retry_max_seconds,
+            max_retries=client_max_retries,
+            retry_base_seconds=client_retry_base_seconds,
+            retry_max_seconds=client_retry_max_seconds,
+            verify=client_verify,
         )
 
         if scopes is None:
             self.scopes = [Scope()]
         else:
             self.scopes = scopes
```

### Comparing `alchemiscale-0.1.2/alchemiscale/interface/api.py` & `alchemiscale-0.1.3/alchemiscale/interface/api.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,16 +5,18 @@
 
 """
 
 
 from typing import Any, Dict, List, Optional, Union
 import os
 import json
+from collections import Counter
 
 from fastapi import FastAPI, APIRouter, Body, Depends, HTTPException, status
+from fastapi.middleware.gzip import GZipMiddleware
 from gufe import AlchemicalNetwork, ChemicalSystem, Transformation
 from gufe.protocols import ProtocolDAGResult
 from gufe.tokenization import GufeTokenizable, JSON_HANDLER
 
 from ..base.api import (
     GufeJSONResponse,
     QueryGUFEHandler,
@@ -24,39 +26,42 @@
     get_s3os_depends,
     base_router,
     get_cred_entity,
     validate_scopes,
     validate_scopes_query,
     _check_store_connectivity,
     gufe_to_json,
+    GzipRoute,
 )
 from ..settings import get_api_settings
 from ..settings import get_base_api_settings, get_api_settings
 from ..storage.statestore import Neo4jStore
 from ..storage.objectstore import S3ObjectStore
 from ..storage.models import ProtocolDAGResultRef, TaskStatusEnum
 from ..models import Scope, ScopedKey
 from ..security.auth import get_token_data, oauth2_scheme
 from ..security.models import Token, TokenData, CredentialedUserIdentity
 
 
 app = FastAPI(title="AlchemiscaleAPI")
 app.dependency_overrides[get_base_api_settings] = get_api_settings
 app.include_router(base_router)
+app.add_middleware(GZipMiddleware, minimum_size=1000, compresslevel=5)
 
 
 def get_cred_user():
     return CredentialedUserIdentity
 
 
 app.dependency_overrides[get_cred_entity] = get_cred_user
 
 router = APIRouter(
     dependencies=[Depends(get_token_data_depends)],
 )
+router.route_class = GzipRoute
 
 
 @app.get("/ping")
 def ping():
     return {"api": "AlchemiscaleAPI"}
 
 
@@ -98,14 +103,33 @@
 ):
     sk = ScopedKey.from_str(scoped_key)
     validate_scopes(sk.scope, token)
 
     return n4js.check_existence(scoped_key=sk)
 
 
+@router.post("/networks", response_model=ScopedKey)
+def create_network(
+    *,
+    network: Dict = Body(...),
+    scope: Scope,
+    n4js: Neo4jStore = Depends(get_n4js_depends),
+    token: TokenData = Depends(get_token_data_depends),
+):
+    validate_scopes(scope, token)
+
+    an = AlchemicalNetwork.from_dict(network)
+    an_sk = n4js.create_network(network=an, scope=scope)
+
+    # create taskhub for this network
+    n4js.create_taskhub(an_sk)
+
+    return an_sk
+
+
 @router.get("/networks", response_class=GufeJSONResponse)
 def query_networks(
     *,
     name: str = None,
     return_gufe: bool = False,
     scope: Scope = Depends(scope_params),
     n4js: Neo4jStore = Depends(get_n4js_depends),
@@ -114,61 +138,157 @@
     # Intersect query scopes with accessible scopes in the token
     query_scopes = validate_scopes_query(scope, token)
     networks_handler = QueryGUFEHandler(return_gufe)
 
     # query each scope
     # loop might be removable in the future with a Union like operator on scopes
     for single_query_scope in query_scopes:
-        # add new networks
         networks_handler.update_results(
             n4js.query_networks(
                 name=name, scope=single_query_scope, return_gufe=return_gufe
             )
         )
 
     return networks_handler.format_return()
 
 
-@router.get("/networks/{network_scoped_key}", response_class=GufeJSONResponse)
-def get_network(
+@router.get("/transformations")
+def query_transformations(
+    *,
+    name: str = None,
+    scope: Scope = Depends(scope_params),
+    n4js: Neo4jStore = Depends(get_n4js_depends),
+    token: TokenData = Depends(get_token_data_depends),
+):
+    # Intersect query scopes with accessible scopes in the token
+    query_scopes = validate_scopes_query(scope, token)
+
+    # query each scope
+    # loop might be removable in the future with a Union like operator on scopes
+    results = []
+    for single_query_scope in query_scopes:
+        results.extend(n4js.query_transformations(name=name, scope=single_query_scope))
+
+    return [str(sk) for sk in results]
+
+
+@router.get("/chemicalsystems")
+def query_chemicalsystems(
+    *,
+    name: str = None,
+    scope: Scope = Depends(scope_params),
+    n4js: Neo4jStore = Depends(get_n4js_depends),
+    token: TokenData = Depends(get_token_data_depends),
+):
+    # Intersect query scopes with accessible scopes in the token
+    query_scopes = validate_scopes_query(scope, token)
+
+    # query each scope
+    # loop might be removable in the future with a Union like operator on scopes
+    results = []
+    for single_query_scope in query_scopes:
+        results.extend(n4js.query_chemicalsystems(name=name, scope=single_query_scope))
+
+    return [str(sk) for sk in results]
+
+
+@router.get("/networks/{network_scoped_key}/transformations")
+def get_network_transformations(
     network_scoped_key,
     *,
     n4js: Neo4jStore = Depends(get_n4js_depends),
     token: TokenData = Depends(get_token_data_depends),
 ):
-    # Get scope from scoped key provided by user, uniquely identifying the network
     sk = ScopedKey.from_str(network_scoped_key)
     validate_scopes(sk.scope, token)
 
-    network = n4js.get_gufe(scoped_key=sk)
-    return gufe_to_json(network)
+    return [str(sk) for sk in n4js.get_network_transformations(network=sk)]
 
 
-@router.post("/networks", response_model=ScopedKey)
-def create_network(
+@router.get("/transformations/{transformation_scoped_key}/networks")
+def get_transformation_networks(
+    transformation_scoped_key,
     *,
-    network: Dict = Body(...),
-    scope: Scope,
     n4js: Neo4jStore = Depends(get_n4js_depends),
     token: TokenData = Depends(get_token_data_depends),
 ):
-    validate_scopes(scope, token)
+    sk = ScopedKey.from_str(transformation_scoped_key)
+    validate_scopes(sk.scope, token)
 
-    an = AlchemicalNetwork.from_dict(network)
-    an_sk = n4js.create_network(network=an, scope=scope)
+    return [str(sk) for sk in n4js.get_transformation_networks(transformation=sk)]
 
-    # create taskhub for this network
-    n4js.create_taskhub(an_sk)
 
-    return an_sk
+@router.get("/networks/{network_scoped_key}/chemicalsystems")
+def get_network_chemicalsystems(
+    network_scoped_key,
+    *,
+    n4js: Neo4jStore = Depends(get_n4js_depends),
+    token: TokenData = Depends(get_token_data_depends),
+):
+    sk = ScopedKey.from_str(network_scoped_key)
+    validate_scopes(sk.scope, token)
 
+    return [str(sk) for sk in n4js.get_network_chemicalsystems(network=sk)]
 
-@router.get("/transformations")
-def query_transformations():
-    return {"message": "nothing yet"}
+
+@router.get("/chemicalsystems/{chemicalsystem_scoped_key}/networks")
+def get_chemicalsystem_networks(
+    chemicalsystem_scoped_key,
+    *,
+    n4js: Neo4jStore = Depends(get_n4js_depends),
+    token: TokenData = Depends(get_token_data_depends),
+):
+    sk = ScopedKey.from_str(chemicalsystem_scoped_key)
+    validate_scopes(sk.scope, token)
+
+    return [str(sk) for sk in n4js.get_chemicalsystem_networks(chemicalsystem=sk)]
+
+
+@router.get("/transformations/{transformation_scoped_key}/chemicalsystems")
+def get_transformation_chemicalsystems(
+    transformation_scoped_key,
+    *,
+    n4js: Neo4jStore = Depends(get_n4js_depends),
+    token: TokenData = Depends(get_token_data_depends),
+):
+    sk = ScopedKey.from_str(transformation_scoped_key)
+    validate_scopes(sk.scope, token)
+
+    return [
+        str(sk) for sk in n4js.get_transformation_chemicalsystems(transformation=sk)
+    ]
+
+
+@router.get("/chemicalsystems/{chemicalsystem_scoped_key}/transformations")
+def get_chemicalsystem_transformations(
+    chemicalsystem_scoped_key,
+    *,
+    n4js: Neo4jStore = Depends(get_n4js_depends),
+    token: TokenData = Depends(get_token_data_depends),
+):
+    sk = ScopedKey.from_str(chemicalsystem_scoped_key)
+    validate_scopes(sk.scope, token)
+
+    return [
+        str(sk) for sk in n4js.get_chemicalsystem_transformations(chemicalsystem=sk)
+    ]
+
+
+@router.get("/networks/{network_scoped_key}", response_class=GufeJSONResponse)
+def get_network(
+    network_scoped_key,
+    *,
+    n4js: Neo4jStore = Depends(get_n4js_depends),
+    token: TokenData = Depends(get_token_data_depends),
+):
+    sk = ScopedKey.from_str(network_scoped_key)
+    validate_scopes(sk.scope, token)
+
+    network = n4js.get_gufe(scoped_key=sk)
+    return gufe_to_json(network)
 
 
 @router.get(
     "/transformations/{transformation_scoped_key}", response_class=GufeJSONResponse
 )
 def get_transformation(
     transformation_scoped_key,
@@ -179,19 +299,14 @@
     sk = ScopedKey.from_str(transformation_scoped_key)
     validate_scopes(sk.scope, token)
 
     transformation = n4js.get_gufe(scoped_key=sk)
     return gufe_to_json(transformation)
 
 
-@router.get("/chemicalsystems")
-def query_chemicalsystems():
-    return {"message": "nothing yet"}
-
-
 @router.get(
     "/chemicalsystems/{chemicalsystem_scoped_key}", response_class=GufeJSONResponse
 )
 def get_chemicalsystem(
     chemicalsystem_scoped_key,
     *,
     n4js: Neo4jStore = Depends(get_n4js_depends),
@@ -229,27 +344,84 @@
         task_sks.append(
             n4js.create_task(transformation=sk, extends=extends, creator=token.entity)
         )
 
     return [str(sk) for sk in task_sks]
 
 
+@router.get("/tasks")
+def query_tasks(
+    *,
+    status: str = None,
+    scope: Scope = Depends(scope_params),
+    n4js: Neo4jStore = Depends(get_n4js_depends),
+    token: TokenData = Depends(get_token_data_depends),
+):
+    # Intersect query scopes with accessible scopes in the token
+    query_scopes = validate_scopes_query(scope, token)
+
+    # query each scope
+    # loop might be removable in the future with a Union like operator on scopes
+    results = []
+    for single_query_scope in query_scopes:
+        results.extend(n4js.query_tasks(status=status, scope=single_query_scope))
+
+    return [str(sk) for sk in results]
+
+
+@router.get("/networks/{network_scoped_key}/tasks")
+def get_network_tasks(
+    network_scoped_key,
+    *,
+    status: str = None,
+    n4js: Neo4jStore = Depends(get_n4js_depends),
+    token: TokenData = Depends(get_token_data_depends),
+):
+    # Get scope from scoped key provided by user, uniquely identifying the network
+    sk = ScopedKey.from_str(network_scoped_key)
+    validate_scopes(sk.scope, token)
+
+    if status is not None:
+        status = TaskStatusEnum(status)
+
+    return [str(sk) for sk in n4js.get_network_tasks(network=sk, status=status)]
+
+
+@router.get("/tasks/{task_scoped_key}/networks")
+def get_task_networks(
+    task_scoped_key,
+    *,
+    n4js: Neo4jStore = Depends(get_n4js_depends),
+    token: TokenData = Depends(get_token_data_depends),
+):
+    sk = ScopedKey.from_str(task_scoped_key)
+    validate_scopes(sk.scope, token)
+
+    return [str(sk) for sk in n4js.get_task_networks(task=sk)]
+
+
 @router.get("/transformations/{transformation_scoped_key}/tasks")
-def get_tasks(
+def get_transformation_tasks(
     transformation_scoped_key,
     *,
     extends: str = None,
     return_as: str = "list",
+    status: str = None,
     n4js: Neo4jStore = Depends(get_n4js_depends),
     token: TokenData = Depends(get_token_data_depends),
 ):
     sk = ScopedKey.from_str(transformation_scoped_key)
     validate_scopes(sk.scope, token)
 
-    task_sks = n4js.get_tasks(sk, extends=extends, return_as=return_as)
+    if status is not None:
+        status = TaskStatusEnum(status)
+
+    task_sks = n4js.get_transformation_tasks(
+        sk, extends=extends, return_as=return_as, status=status
+    )
 
     if return_as == "list":
         return [str(sk) for sk in task_sks]
     elif return_as == "graph":
         return {
             str(sk): str(extends) if extends is not None else None
             for sk, extends in task_sks.items()
@@ -257,14 +429,61 @@
     else:
         raise HTTPException(
             status_code=status.HTTP_400_BAD_REQUEST,
             detail=f"`return_as` takes 'list' or 'graph', not '{return_as}'",
         )
 
 
+@router.get("/scopes/{scope}/status")
+def get_scope_status(
+    scope,
+    *,
+    n4js: Neo4jStore = Depends(get_n4js_depends),
+    token: TokenData = Depends(get_token_data_depends),
+):
+    scope = Scope.from_str(scope)
+    scope_space = validate_scopes_query(scope, token)
+
+    status_counts = Counter()
+    for single_scope in scope_space:
+        status_counts.update(n4js.get_scope_status(single_scope))
+
+    return dict(status_counts)
+
+
+@router.get("/networks/{network_scoped_key}/status")
+def get_network_status(
+    network_scoped_key,
+    *,
+    n4js: Neo4jStore = Depends(get_n4js_depends),
+    token: TokenData = Depends(get_token_data_depends),
+):
+    sk = ScopedKey.from_str(network_scoped_key)
+    validate_scopes(sk.scope, token)
+
+    status_counts = n4js.get_network_status(network_scoped_key)
+
+    return status_counts
+
+
+@router.get("/transformations/{transformation_scoped_key}/status")
+def get_transformation_status(
+    transformation_scoped_key,
+    *,
+    n4js: Neo4jStore = Depends(get_n4js_depends),
+    token: TokenData = Depends(get_token_data_depends),
+):
+    sk = ScopedKey.from_str(transformation_scoped_key)
+    validate_scopes(sk.scope, token)
+
+    status_counts = n4js.get_transformation_status(transformation_scoped_key)
+
+    return status_counts
+
+
 @router.post("/networks/{network_scoped_key}/tasks/action")
 def action_tasks(
     network_scoped_key,
     *,
     tasks: List[ScopedKey] = Body(embed=True),
     n4js: Neo4jStore = Depends(get_n4js_depends),
     token: TokenData = Depends(get_token_data_depends),
@@ -291,14 +510,66 @@
 
     taskhub_sk = n4js.get_taskhub(sk)
     canceled_sks = n4js.cancel_tasks(tasks, taskhub_sk)
 
     return [str(sk) if sk is not None else None for sk in canceled_sks]
 
 
+@router.post("/bulk/tasks/status/get")
+def tasks_status_get(
+    *,
+    tasks: List[ScopedKey] = Body(embed=True),
+    n4js: Neo4jStore = Depends(get_n4js_depends),
+    token: TokenData = Depends(get_token_data_depends),
+) -> List[Union[str, None]]:
+    valid_tasks = []
+    for task_sk in tasks:
+        try:
+            validate_scopes(task_sk.scope, token)
+            valid_tasks.append(task_sk)
+        except HTTPException:
+            valid_tasks.append(None)
+
+    statuses = n4js.get_task_status(valid_tasks)
+
+    return [status.value if status is not None else None for status in statuses]
+
+
+@router.post("/bulk/tasks/status/set")
+def tasks_status_set(
+    *,
+    tasks: List[ScopedKey] = Body(),
+    status: str = Body(),
+    n4js: Neo4jStore = Depends(get_n4js_depends),
+    token: TokenData = Depends(get_token_data_depends),
+) -> List[Union[str, None]]:
+    status = TaskStatusEnum(status)
+    if status not in (
+        TaskStatusEnum.waiting,
+        TaskStatusEnum.invalid,
+        TaskStatusEnum.deleted,
+    ):
+        raise HTTPException(
+            status_code=status.HTTP_400_BAD_REQUEST,
+            detail=f"Cannot set status to '{status}', must be one of 'waiting', 'invalid', 'deleted'",
+        )
+
+    valid_tasks = []
+    for task_sk in tasks:
+        try:
+            validate_scopes(task_sk.scope, token)
+            valid_tasks.append(task_sk)
+        except HTTPException:
+            valid_tasks.append(None)
+
+    tasks_updated = n4js.set_task_status(valid_tasks, status)
+
+    return [str(t) if t is not None else None for t in tasks_updated]
+
+
 @router.post("/tasks/{task_scoped_key}/status")
 def set_task_status(
     task_scoped_key,
     status: str = Body(),
     n4js: Neo4jStore = Depends(get_n4js_depends),
     token: TokenData = Depends(get_token_data_depends),
 ):
@@ -329,14 +600,34 @@
     validate_scopes(task_sk.scope, token)
 
     status = n4js.get_task_status([task_sk])
 
     return status[0].value
 
 
+@router.get("/tasks/{task_scoped_key}/transformation", response_class=GufeJSONResponse)
+def get_task_transformation(
+    task_scoped_key,
+    *,
+    n4js: Neo4jStore = Depends(get_n4js_depends),
+    token: TokenData = Depends(get_token_data_depends),
+):
+    sk = ScopedKey.from_str(task_scoped_key)
+    validate_scopes(sk.scope, token)
+
+    transformation: ScopedKey
+
+    transformation, protocoldagresultref = n4js.get_task_transformation(
+        task=task_scoped_key,
+        return_gufe=False,
+    )
+
+    return str(transformation)
+
+
 ### results
 
 
 @router.get(
     "/transformations/{transformation_scoped_key}/results",
     response_class=GufeJSONResponse,
 )
@@ -418,34 +709,14 @@
     # we leave each ProtocolDAGResult in string form to avoid
     # deserializing/reserializing here; just passing through to client
     pdr: str = s3os.pull_protocoldagresult(sk, tf_sk, return_as="json", ok=False)
 
     return [pdr]
 
 
-@router.get("/tasks/{task_scoped_key}/transformation", response_class=GufeJSONResponse)
-def get_task_transformation(
-    task_scoped_key,
-    *,
-    n4js: Neo4jStore = Depends(get_n4js_depends),
-    token: TokenData = Depends(get_token_data_depends),
-):
-    sk = ScopedKey.from_str(task_scoped_key)
-    validate_scopes(sk.scope, token)
-
-    transformation: ScopedKey
-
-    transformation, protocoldagresultref = n4js.get_task_transformation(
-        task=task_scoped_key,
-        return_gufe=False,
-    )
-
-    return str(transformation)
-
-
 @router.get(
     "/tasks/{task_scoped_key}/results",
     response_class=GufeJSONResponse,
 )
 def get_task_results(
     task_scoped_key,
     *,
```

### Comparing `alchemiscale-0.1.2/alchemiscale/models.py` & `alchemiscale-0.1.3/alchemiscale/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,23 @@
 
     def __str__(self):
         triple = (
             i if i is not None else "*" for i in (self.org, self.campaign, self.project)
         )
         return "-".join(triple)
 
+    def __lt__(self, other):
+        return str(self) < str(other)
+
+    def __eq__(self, other):
+        if not isinstance(other, self.__class__):
+            return False
+
+        return str(self) == str(other)
+
     class Config:
         frozen = True
 
     @staticmethod
     def _validate_component(v, component):
         """
         Use regex to check that the component:
```

### Comparing `alchemiscale-0.1.2/alchemiscale/security/auth.py` & `alchemiscale-0.1.3/alchemiscale/security/auth.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 
 
 def create_access_token(
     *,
     data: dict,
     secret_key: str,
     expires_seconds: Optional[int] = 900,
-    jwt_algorithm: Optional[str] = "HS256"
+    jwt_algorithm: Optional[str] = "HS256",
 ) -> str:
     to_encode = data.copy()
 
     expire = datetime.utcnow() + timedelta(seconds=expires_seconds)
     to_encode.update({"exp": expire})
 
     encoded_jwt = jwt.encode(to_encode, secret_key, algorithm=jwt_algorithm)
```

### Comparing `alchemiscale-0.1.2/alchemiscale/security/models.py` & `alchemiscale-0.1.3/alchemiscale/security/models.py`

 * *Files identical despite different names*

### Comparing `alchemiscale-0.1.2/alchemiscale/settings.py` & `alchemiscale-0.1.3/alchemiscale/settings.py`

 * *Files identical despite different names*

### Comparing `alchemiscale-0.1.2/alchemiscale/storage/models.py` & `alchemiscale-0.1.3/alchemiscale/storage/models.py`

 * *Files identical despite different names*

### Comparing `alchemiscale-0.1.2/alchemiscale/storage/objectstore.py` & `alchemiscale-0.1.3/alchemiscale/storage/objectstore.py`

 * *Files identical despite different names*

### Comparing `alchemiscale-0.1.2/alchemiscale/storage/statestore.py` & `alchemiscale-0.1.3/alchemiscale/storage/statestore.py`

 * *Files 5% similar despite different names*

```diff
@@ -552,24 +552,25 @@
             q += """
             OPTIONAL MATCH p = (n)-[r:DEPENDS_ON*]->(m)
             WHERE NOT (m)-[:DEPENDS_ON]->()
             RETURN n,p
             """
         else:
             q += """
-            RETURN n
+            RETURN DISTINCT n
+            ORDER BY n._org, n._campaign, n._project, n._gufe_key
             """
         with self.transaction() as tx:
             res = tx.run(q)
 
-        nodes = set()
+        nodes = list()
         subgraph = Subgraph()
 
         for record in res:
-            nodes.add(record["n"])
+            nodes.append(record["n"])
             if return_gufe and record["p"] is not None:
                 subgraph = subgraph | record["p"]
             else:
                 subgraph = record["n"]
 
         if return_gufe:
             return {
@@ -671,75 +672,159 @@
             qualname="AlchemicalNetwork",
             additional=additional,
             key=key,
             scope=scope,
             return_gufe=return_gufe,
         )
 
-    def query_transformations(
-        self, *, name=None, key=None, scope: Scope = Scope(), chemical_systems=None
-    ):
+    def query_transformations(self, *, name=None, key=None, scope: Scope = Scope()):
         """Query for `Transformation`\s matching given attributes."""
         additional = {"name": name}
         return self._query(
             qualname="Transformation", additional=additional, key=key, scope=scope
         )
 
-    def query_chemicalsystems(
-        self, *, name=None, key=None, scope: Scope = Scope(), transformations=None
-    ):
+    def query_chemicalsystems(self, *, name=None, key=None, scope: Scope = Scope()):
         """Query for `ChemicalSystem`\s matching given attributes."""
         additional = {"name": name}
         return self._query(
             qualname="ChemicalSystem", additional=additional, key=key, scope=scope
         )
 
-    def get_transformations_for_chemicalsystem(self):
-        ...
+    def get_network_transformations(self, network: ScopedKey) -> List[ScopedKey]:
+        """List ScopedKeys for Transformations associated with the given AlchemicalNetwork."""
+        q = f"""
+        MATCH (:AlchemicalNetwork {{_scoped_key: '{network}'}})-[:DEPENDS_ON]->(t:Transformation)
+        WITH t._scoped_key as sk
+        RETURN sk
+        """
+        sks = []
+        with self.transaction() as tx:
+            res = tx.run(q)
+            for rec in res:
+                sks.append(rec["sk"])
+
+        return [ScopedKey.from_str(sk) for sk in sks]
+
+    def get_transformation_networks(self, transformation: ScopedKey) -> List[ScopedKey]:
+        """List ScopedKeys for AlchemicalNetworks associated with the given Transformation."""
+        q = f"""
+        MATCH (:Transformation {{_scoped_key: '{transformation}'}})<-[:DEPENDS_ON]-(an:AlchemicalNetwork)
+        WITH an._scoped_key as sk
+        RETURN sk
+        """
+        sks = []
+        with self.transaction() as tx:
+            res = tx.run(q)
+            for rec in res:
+                sks.append(rec["sk"])
+
+        return [ScopedKey.from_str(sk) for sk in sks]
+
+    def get_network_chemicalsystems(self, network: ScopedKey) -> List[ScopedKey]:
+        """List ScopedKeys for ChemicalSystems associated with the given AlchemicalNetwork."""
+        q = f"""
+        MATCH (:AlchemicalNetwork {{_scoped_key: '{network}'}})-[:DEPENDS_ON]->(cs:ChemicalSystem)
+        WITH cs._scoped_key as sk
+        RETURN sk
+        """
+        sks = []
+        with self.transaction() as tx:
+            res = tx.run(q)
+            for rec in res:
+                sks.append(rec["sk"])
+
+        return [ScopedKey.from_str(sk) for sk in sks]
+
+    def get_chemicalsystem_networks(self, chemicalsystem: ScopedKey) -> List[ScopedKey]:
+        """List ScopedKeys for AlchemicalNetworks associated with the given ChemicalSystem."""
+        q = f"""
+        MATCH (:ChemicalSystem {{_scoped_key: '{chemicalsystem}'}})<-[:DEPENDS_ON]-(an:AlchemicalNetwork)
+        WITH an._scoped_key as sk
+        RETURN sk
+        """
+        sks = []
+        with self.transaction() as tx:
+            res = tx.run(q)
+            for rec in res:
+                sks.append(rec["sk"])
+
+        return [ScopedKey.from_str(sk) for sk in sks]
+
+    def get_transformation_chemicalsystems(
+        self, transformation: ScopedKey
+    ) -> List[ScopedKey]:
+        """List ScopedKeys for the ChemicalSystems associated with the given Transformation."""
+        q = f"""
+        MATCH (:Transformation {{_scoped_key: '{transformation}'}})-[:DEPENDS_ON]->(cs:ChemicalSystem)
+        WITH cs._scoped_key as sk
+        RETURN sk
+        """
+        sks = []
+        with self.transaction() as tx:
+            res = tx.run(q)
+            for rec in res:
+                sks.append(rec["sk"])
 
-    def get_networks_for_transformation(self):
-        ...
+        return [ScopedKey.from_str(sk) for sk in sks]
 
-    def _get_protocoldagresultrefs(self, q):
+    def get_chemicalsystem_transformations(
+        self, chemicalsystem: ScopedKey
+    ) -> List[ScopedKey]:
+        """List ScopedKeys for the Transformations associated with the given ChemicalSystem."""
+        q = f"""
+        MATCH (:ChemicalSystem {{_scoped_key: '{chemicalsystem}'}})<-[:DEPENDS_ON]-(t:Transformation)
+        WITH t._scoped_key as sk
+        RETURN sk
+        """
+        sks = []
         with self.transaction() as tx:
             res = tx.run(q)
+            for rec in res:
+                sks.append(rec["sk"])
+
+        return [ScopedKey.from_str(sk) for sk in sks]
+
+    def _get_protocoldagresultrefs(self, q: str, scoped_key: ScopedKey):
+        with self.transaction() as tx:
+            res = tx.run(q, scoped_key=str(scoped_key))
 
         protocoldagresultrefs = []
         subgraph = Subgraph()
         for record in res:
             protocoldagresultrefs.append(record["res"])
             subgraph = subgraph | record["res"]
 
         return list(self._subgraph_to_gufe(protocoldagresultrefs, subgraph).values())
 
     def get_transformation_results(
         self, transformation: ScopedKey
     ) -> List[ProtocolDAGResultRef]:
         # get all task result protocoldagresultrefs corresponding to given transformation
         # returned in no particular order
-        q = f"""
-        MATCH (trans:Transformation {{_scoped_key: "{transformation}"}}),
+        q = """
+        MATCH (trans:Transformation {_scoped_key: $scoped_key}),
               (trans)<-[:PERFORMS]-(:Task)-[:RESULTS_IN]->(res:ProtocolDAGResultRef)
         WHERE res.ok = true
         RETURN res
         """
-        return self._get_protocoldagresultrefs(q)
+        return self._get_protocoldagresultrefs(q, transformation)
 
     def get_transformation_failures(
         self, transformation: ScopedKey
     ) -> List[ProtocolDAGResultRef]:
         # get all task failure protocoldagresultrefs corresponding to given transformation
         # returned in no particular order
-        q = f"""
-        MATCH (trans:Transformation {{_scoped_key: "{transformation}"}}),
+        q = """
+        MATCH (trans:Transformation {_scoped_key: $scoped_key}),
               (trans)<-[:PERFORMS]-(:Task)-[:RESULTS_IN]->(res:ProtocolDAGResultRef)
         WHERE res.ok = false
         RETURN res
         """
-        return self._get_protocoldagresultrefs(q)
+        return self._get_protocoldagresultrefs(q, transformation)
 
     ## compute
 
     def set_strategy(
         self,
         strategy: Strategy,
         network: ScopedKey,
@@ -1391,60 +1476,67 @@
         )
 
         with self.transaction() as tx:
             tx.create(subgraph)
 
         return scoped_key
 
-    def set_tasks(
-        self,
-        transformation: ScopedKey,
-        extends: Optional[Task] = None,
-        count: int = 1,
-    ) -> ScopedKey:
-        """Set a fixed number of Tasks against the given Transformation if not
-        already present.
+    def query_tasks(self, *, status=None, key=None, scope: Scope = Scope()):
+        """Query for `Task`\s matching given attributes."""
+        additional = {"status": status}
+        return self._query(qualname="Task", additional=additional, key=key, scope=scope)
+
+    def get_network_tasks(
+        self, network: ScopedKey, status: Optional[TaskStatusEnum] = None
+    ) -> List[ScopedKey]:
+        """List ScopedKeys for all Tasks associated with the given AlchemicalNetwork."""
+        q = f"""
+        MATCH (an:AlchemicalNetwork {{_scoped_key: "{network}"}})-[:DEPENDS_ON]->(tf:Transformation),
+              (tf)<-[:PERFORMS]-(t:Task)
+        """
 
-        Note: Tasks created by this method are not added to any TaskHubs.
+        if status is not None:
+            q += f"""
+            WHERE t.status = '{status.value}'
+            """
 
-        Parameters
-        ----------
-        transformation
-            The Transformation to compute.
-        scope
-            The scope the Transformation is in; ignored if `transformation` is a ScopedKey.
-        extends
-            The Task to use as a starting point for this Task.
-            Will use the `ProtocolDAGResult` from the given Task as the
-            `extends` input for the Task's eventual call to `Protocol.create`.
-        count
-            The total number of tasks that should exist corresponding to the
-            specified `transformation`, `scope`, and `extends`.
+        q += """
+        WITH t._scoped_key as sk
+        RETURN sk
         """
-        raise NotImplementedError
-        # TODO: finish this one out when we have a reasonable approach to locking
-        # too hard to perform in a single Cypher query; unclear how to create many nodes in a loop
-        transformation_node = self._get_node_from_obj_or_sk(
-            transformation, Transformation, scope
-        )
+        sks = []
+        with self.transaction() as tx:
+            res = tx.run(q)
+            for rec in res:
+                sks.append(rec["sk"])
 
-    def set_task_priority(self, task: ScopedKey, priority: int):
+        return [ScopedKey.from_str(sk) for sk in sks]
+
+    def get_task_networks(self, task: ScopedKey) -> List[ScopedKey]:
+        """List ScopedKeys for AlchemicalNetworks associated with the given Task."""
         q = f"""
-        MATCH (t:Task {{_scoped_key: "{task}"}})
-        SET t.priority = {priority}
-        RETURN t
+        MATCH (t:Task {{_scoped_key: '{task}'}})-[:PERFORMS]->(tf:Transformation),
+              (tf)<-[:DEPENDS_ON]-(an:AlchemicalNetwork)
+        WITH an._scoped_key as sk
+        RETURN sk
         """
+        sks = []
         with self.transaction() as tx:
-            tx.run(q)
+            res = tx.run(q)
+            for rec in res:
+                sks.append(rec["sk"])
+
+        return [ScopedKey.from_str(sk) for sk in sks]
 
-    def get_tasks(
+    def get_transformation_tasks(
         self,
         transformation: ScopedKey,
         extends: Optional[ScopedKey] = None,
         return_as: str = "list",
+        status: Optional[TaskStatusEnum] = None,
     ) -> Union[List[ScopedKey], Dict[ScopedKey, Optional[ScopedKey]]]:
         """Get all Tasks that perform the given Transformation.
 
         If a Task ScopedKey is given for `extends`, then only those Tasks
         that follow via any number of EXTENDS relationships will be returned.
 
         `return_as` takes either `list` or `graph` as input.
@@ -1458,14 +1550,19 @@
         extends
 
         """
         q = f"""
         MATCH (trans:Transformation {{_scoped_key: '{transformation}'}})<-[:PERFORMS]-(task:Task)
         """
 
+        if status is not None:
+            q += f"""
+            WHERE task.status = '{status.value}'
+            """
+
         if extends:
             q += f"""
             MATCH (trans)<-[:PERFORMS]-(extends:Task {{_scoped_key: '{extends}'}})
             WHERE (task)-[:EXTENDS*]->(extends)
             RETURN task
             """
         else:
@@ -1486,38 +1583,14 @@
             return {
                 ScopedKey.from_str(t["_scoped_key"]): ScopedKey.from_str(t["extends"])
                 if t["extends"] is not None
                 else None
                 for t in tasks
             }
 
-    def query_tasks(
-        self,
-        scope: Optional[Scope] = None,
-        network: Optional[ScopedKey] = None,
-        transformation: Optional[ScopedKey] = None,
-        extends: Optional[ScopedKey] = None,
-        status: Optional[List[TaskStatusEnum]] = None,
-    ):
-        raise NotImplementedError
-
-    def delete_task(
-        self,
-        task: ScopedKey,
-    ) -> Task:
-        """Remove a compute Task from a Transformation.
-
-        This will also remove the Task from all TaskHubs it is a part of.
-
-        This method is intended for administrator use; generally Tasks should
-        instead have their tasks set to 'deleted' and retained.
-
-        """
-        raise NotImplementedError
-
     def get_task_transformation(
         self,
         task: ScopedKey,
         return_gufe=True,
     ) -> Union[
         Tuple[Transformation, Optional[ProtocolDAGResultRef]],
         Tuple[ScopedKey, Optional[ScopedKey]],
@@ -1566,14 +1639,119 @@
                 self.get_gufe(protocoldagresultref)
                 if protocoldagresultref is not None
                 else None,
             )
 
         return transformation, protocoldagresultref
 
+    def set_tasks(
+        self,
+        transformation: ScopedKey,
+        extends: Optional[Task] = None,
+        count: int = 1,
+    ) -> ScopedKey:
+        """Set a fixed number of Tasks against the given Transformation if not
+        already present.
+
+        Note: Tasks created by this method are not added to any TaskHubs.
+
+        Parameters
+        ----------
+        transformation
+            The Transformation to compute.
+        scope
+            The scope the Transformation is in; ignored if `transformation` is a ScopedKey.
+        extends
+            The Task to use as a starting point for this Task.
+            Will use the `ProtocolDAGResult` from the given Task as the
+            `extends` input for the Task's eventual call to `Protocol.create`.
+        count
+            The total number of tasks that should exist corresponding to the
+            specified `transformation`, `scope`, and `extends`.
+        """
+        raise NotImplementedError
+        # TODO: finish this one out when we have a reasonable approach to locking
+        # too hard to perform in a single Cypher query; unclear how to create many nodes in a loop
+        transformation_node = self._get_node_from_obj_or_sk(
+            transformation, Transformation, scope
+        )
+
+    def set_task_priority(self, task: ScopedKey, priority: int):
+        q = f"""
+        MATCH (t:Task {{_scoped_key: "{task}"}})
+        SET t.priority = {priority}
+        RETURN t
+        """
+        with self.transaction() as tx:
+            tx.run(q)
+
+    def delete_task(
+        self,
+        task: ScopedKey,
+    ) -> Task:
+        """Remove a compute Task from a Transformation.
+
+        This will also remove the Task from all TaskHubs it is a part of.
+
+        This method is intended for administrator use; generally Tasks should
+        instead have their tasks set to 'deleted' and retained.
+
+        """
+        raise NotImplementedError
+
+    def get_scope_status(self, scope: Scope) -> Dict[str, int]:
+        """Return status counts for all Tasks within the given Scope."""
+
+        properties = {
+            "_org": scope.org,
+            "_campaign": scope.campaign,
+            "_project": scope.project,
+        }
+
+        prop_string = ", ".join(
+            "{}: '{}'".format(key, value)
+            for key, value in properties.items()
+            if value is not None
+        )
+
+        q = f"""
+        MATCH (n:Task {{{prop_string}}})
+        RETURN n.status AS status, count(n) as counts
+        """
+        with self.transaction() as tx:
+            res = tx.run(q)
+            counts = {rec["status"]: rec["counts"] for rec in res}
+
+        return counts
+
+    def get_network_status(self, network: ScopedKey) -> Dict[str, int]:
+        """Return status counts for all Tasks associated with the given AlchemicalNetwork."""
+        q = f"""
+        MATCH (:AlchemicalNetwork {{_scoped_key: "{network}"}})-[:DEPENDS_ON]->(tf:Transformation),
+              (tf)<-[:PERFORMS]-(t:Task)
+        RETURN t.status AS status, count(t) as counts
+        """
+        with self.transaction() as tx:
+            res = tx.run(q)
+            counts = {rec["status"]: rec["counts"] for rec in res}
+
+        return counts
+
+    def get_transformation_status(self, transformation: ScopedKey) -> Dict[str, int]:
+        """Return status counts for all Tasks associated with the given Transformation."""
+        q = f"""
+        MATCH (:Transformation {{_scoped_key: "{transformation}"}})<-[:PERFORMS]-(t:Task)
+        RETURN t.status AS status, count(t) as counts
+        """
+        with self.transaction() as tx:
+            res = tx.run(q)
+            counts = {rec["status"]: rec["counts"] for rec in res}
+
+        return counts
+
     def set_task_result(
         self, task: ScopedKey, protocoldagresultref: ProtocolDAGResultRef
     ) -> ScopedKey:
         """Set a `ProtocolDAGResultRef` pointing to a `ProtocolDAGResult` for the given `Task`."""
 
         if task.qualname != "Task":
             raise ValueError("`task` ScopedKey does not correspond to a `Task`")
@@ -1600,32 +1778,32 @@
             tx.merge(subgraph, "GufeTokenizable", "_scoped_key")
 
         return scoped_key
 
     def get_task_results(self, task: ScopedKey) -> List[ProtocolDAGResultRef]:
         # get all task result protocoldagresultrefs corresponding to given task
         # returned in no particular order
-        q = f"""
-        MATCH (task:Task {{_scoped_key: "{task}"}}),
+        q = """
+        MATCH (task:Task {_scoped_key: $scoped_key}),
               (task)-[:RESULTS_IN]->(res:ProtocolDAGResultRef)
         WHERE res.ok = true
         RETURN res
         """
-        return self._get_protocoldagresultrefs(q)
+        return self._get_protocoldagresultrefs(q, task)
 
     def get_task_failures(self, task: ScopedKey) -> List[ProtocolDAGResultRef]:
         # get all task failure protocoldagresultrefs corresponding to given task
         # returned in no particular order
-        q = f"""
-        MATCH (task:Task {{_scoped_key: "{task}"}}),
+        q = """
+        MATCH (task:Task {_scoped_key: $scoped_key}),
               (task)-[:RESULTS_IN]->(res:ProtocolDAGResultRef)
         WHERE res.ok = false
         RETURN res
         """
-        return self._get_protocoldagresultrefs(q)
+        return self._get_protocoldagresultrefs(q, task)
 
     def set_task_status(
         self, tasks: List[ScopedKey], status: TaskStatusEnum, raise_error: bool = False
     ) -> List[Optional[ScopedKey]]:
         """Set the status of a list of Tasks.
 
         This is a master method that calls the appropriate method for the
@@ -1659,82 +1837,85 @@
             The list of Tasks to get the status for.
 
         Returns
         -------
         Dict[ScopedKey,TaskStatusEnum]
             A dictionary of Tasks and their statuses.
         """
-
         statuses = []
         with self.transaction() as tx:
-            for t in tasks:
-                q = f"""
-                MATCH (t:Task {{_scoped_key: '{t}'}})
-                RETURN t
-                """
-                task = tx.run(q).to_subgraph()
-                if task is None:
-                    statuses.append(None)
-                else:
-                    status = task.get("status")
-                    statuses.append(TaskStatusEnum(status))
+            q = """
+            WITH $scoped_keys AS batch
+            UNWIND batch AS scoped_key
+            OPTIONAL MATCH (t:Task)
+            WHERE t._scoped_key = scoped_key
+            RETURN t.status as status
+            """
+            res = tx.run(q, scoped_keys=[str(t) for t in tasks])
+
+            for rec in res:
+                status = rec["status"]
+                statuses.append(TaskStatusEnum(status) if status is not None else None)
 
         return statuses
 
-    def _set_task_status(self, tasks, q_func, err_msg_func, raise_error):
+    def _set_task_status(
+        self, tasks, q: str, err_msg_func, raise_error
+    ) -> List[Optional[ScopedKey]]:
         tasks_statused = []
         with self.transaction() as tx:
-            for t in tasks:
-                res = tx.run(q_func(t))
-                # we only need the first record to get the info we need
-                for record in res:
-                    task_i = record["t"]
-                    task_set = record["t_"]
-                    break
+            res = tx.run(q, scoped_keys=[str(t) for t in tasks])
+
+            for record in res:
+                task_i = record["t"]
+                task_set = record["t_"]
+                scoped_key = record["scoped_key"]
 
                 if task_set is None:
                     if raise_error:
                         status = task_i["status"]
-                        raise ValueError(err_msg_func(t, status))
+                        raise ValueError(err_msg_func(scoped_key, status))
                     tasks_statused.append(None)
                 elif task_i is None:
                     if raise_error:
                         raise ValueError("No such task {t}")
                     tasks_statused.append(None)
                 else:
-                    tasks_statused.append(t)
+                    tasks_statused.append(ScopedKey.from_str(scoped_key))
 
         return tasks_statused
 
     def set_task_waiting(
         self, tasks: List[ScopedKey], raise_error: bool = False
     ) -> List[Optional[ScopedKey]]:
         """Set the status of a list of Tasks to `waiting`.
 
         Only Tasks with status `error` or `running` can be set to `waiting`.
 
         """
 
-        def q(t):
-            return f"""
-            MATCH (t:Task {{_scoped_key: '{t}'}})
-
-            OPTIONAL MATCH (t_:Task {{_scoped_key: '{t}'}})
-            WHERE t_.status IN ['waiting', 'running', 'error']
-            SET t_.status = '{TaskStatusEnum.waiting.value}'
-
-            WITH t, t_
-
-            // if we changed the status to waiting,
-            // drop CLAIMS relationship
-            OPTIONAL MATCH (t_)<-[cl:CLAIMS]-(csreg:ComputeServiceRegistration)
-            DELETE cl
+        q = """
+        WITH $scoped_keys AS batch
+        UNWIND batch AS scoped_key
 
-            RETURN t, t_
-            """
+        OPTIONAL MATCH (t:Task {_scoped_key: scoped_key})
+
+        OPTIONAL MATCH (t_:Task {_scoped_key: scoped_key})
+        WHERE t_.status IN ['waiting', 'running', 'error']
+        SET t_.status = 'waiting'
+
+        WITH scoped_key, t, t_
+
+        // if we changed the status to waiting,
+        // drop CLAIMS relationship
+        OPTIONAL MATCH (t_)<-[cl:CLAIMS]-(csreg:ComputeServiceRegistration)
+        DELETE cl
+
+        RETURN scoped_key, t, t_
+        """
 
         def err_msg(t, status):
             return f"Cannot set task {t} with current status: {status} to `waiting` as it is not currently `error` or `running`."
 
         return self._set_task_status(tasks, q, err_msg, raise_error=raise_error)
 
     def set_task_running(
@@ -1742,24 +1923,26 @@
     ) -> List[Optional[ScopedKey]]:
         """Set the status of a list of Tasks to `running`.
 
         Only Tasks with status `waiting` can be set to `running`.
 
         """
 
-        def q(t):
-            return f"""
-            MATCH (t:Task {{_scoped_key: '{t}'}})
-
-            OPTIONAL MATCH (t_:Task {{_scoped_key: '{t}'}})
-            WHERE t_.status IN ['running', 'waiting']
-            SET t_.status = '{TaskStatusEnum.running.value}'
+        q = """
+        WITH $scoped_keys AS batch
+        UNWIND batch AS scoped_key
 
-            RETURN t, t_
-            """
+        OPTIONAL MATCH (t:Task {_scoped_key: scoped_key})
+
+        OPTIONAL MATCH (t_:Task {_scoped_key: scoped_key})
+        WHERE t_.status IN ['running', 'waiting']
+        SET t_.status = 'running'
+
+        RETURN scoped_key, t, t_
+        """
 
         def err_msg(t, status):
             return f"Cannot set task {t} with current status: {status} to `running` as it is not currently `waiting`."
 
         return self._set_task_status(tasks, q, err_msg, raise_error=raise_error)
 
     def set_task_complete(
@@ -1767,38 +1950,40 @@
     ) -> List[Optional[ScopedKey]]:
         """Set the status of a list of Tasks to `complete`.
 
         Only `running` Tasks can be set to `complete`.
 
         """
 
-        def q(t):
-            return f"""
-            MATCH (t:Task {{_scoped_key: '{t}'}})
+        q = """
+        WITH $scoped_keys AS batch
+        UNWIND batch AS scoped_key
 
-            OPTIONAL MATCH (t_:Task {{_scoped_key: '{t}'}})
-            WHERE t_.status IN ['complete', 'running']
-            SET t_.status = '{TaskStatusEnum.complete.value}'
+        OPTIONAL MATCH (t:Task {_scoped_key: scoped_key})
 
-            WITH t, t_
+        OPTIONAL MATCH (t_:Task {_scoped_key: scoped_key})
+        WHERE t_.status IN ['complete', 'running']
+        SET t_.status = 'complete'
 
-            // if we changed the status to complete,
-            // drop all ACTIONS relationships
-            OPTIONAL MATCH (t_)<-[ar:ACTIONS]-(th:TaskHub)
-            DELETE ar
+        WITH scoped_key, t, t_
 
-            WITH t, t_
+        // if we changed the status to complete,
+        // drop all ACTIONS relationships
+        OPTIONAL MATCH (t_)<-[ar:ACTIONS]-(th:TaskHub)
+        DELETE ar
 
-            // if we changed the status to complete,
-            // drop CLAIMS relationship
-            OPTIONAL MATCH (t_)<-[cl:CLAIMS]-(csreg:ComputeServiceRegistration)
-            DELETE cl
+        WITH scoped_key, t, t_
 
-            RETURN t, t_
-            """
+        // if we changed the status to complete,
+        // drop CLAIMS relationship
+        OPTIONAL MATCH (t_)<-[cl:CLAIMS]-(csreg:ComputeServiceRegistration)
+        DELETE cl
+
+        RETURN scoped_key, t, t_
+        """
 
         def err_msg(t, status):
             return f"Cannot set task {t} with current status: {status} to `complete` as it is not currently `running`."
 
         return self._set_task_status(tasks, q, err_msg, raise_error=raise_error)
 
     def set_task_error(
@@ -1806,31 +1991,33 @@
     ) -> List[Optional[ScopedKey]]:
         """Set the status of a list of Tasks to `error`.
 
         Only `running` Tasks can be set to `error`.
 
         """
 
-        def q(t):
-            return f"""
-            MATCH (t:Task {{_scoped_key: '{t}'}})
-
-            OPTIONAL MATCH (t_:Task {{_scoped_key: '{t}'}})
-            WHERE t_.status IN ['error', 'running']
-            SET t_.status = '{TaskStatusEnum.error.value}'
-
-            WITH t, t_
-
-            // if we changed the status to error,
-            // drop CLAIMS relationship
-            OPTIONAL MATCH (t_)<-[cl:CLAIMS]-(csreg:ComputeServiceRegistration)
-            DELETE cl
+        q = """
+        WITH $scoped_keys AS batch
+        UNWIND batch AS scoped_key
 
-            RETURN t, t_
-            """
+        OPTIONAL MATCH (t:Task {_scoped_key: scoped_key})
+
+        OPTIONAL MATCH (t_:Task {_scoped_key: scoped_key})
+        WHERE t_.status IN ['error', 'running']
+        SET t_.status = 'error'
+
+        WITH scoped_key, t, t_
+
+        // if we changed the status to error,
+        // drop CLAIMS relationship
+        OPTIONAL MATCH (t_)<-[cl:CLAIMS]-(csreg:ComputeServiceRegistration)
+        DELETE cl
+
+        RETURN scoped_key, t, t_
+        """
 
         def err_msg(t, status):
             return f"Cannot set task {t} with current status: {status} to `error` as it is not currently `running`."
 
         return self._set_task_status(tasks, q, err_msg, raise_error=raise_error)
 
     def set_task_invalid(
@@ -1839,83 +2026,103 @@
         """Set the status of a list of Tasks to `invalid`.
 
         Any Task can be set to `invalid`; an `invalid` Task cannot change to
         any other status.
 
         """
 
-        with self.transaction() as tx:
-            for t in tasks:
-                # set the status and delete the ACTIONS relationship
-                # make sure we follow the extends chain and set all tasks to invalid
-                # and remove actions relationships
-                q = f"""
-                MATCH (t:Task {{_scoped_key: '{t}'}})
+        # set the status and delete the ACTIONS relationship
+        # make sure we follow the extends chain and set all tasks to invalid
+        # and remove actions relationships
+        q = """
+        WITH $scoped_keys AS batch
+        UNWIND batch AS scoped_key
 
-                // EXTENDS* used to get all tasks in the extends chain
-                OPTIONAL MATCH (t)<-[er:EXTENDS*]-(extends_task:Task)
-                SET t.status = '{TaskStatusEnum.invalid.value}'
-                SET extends_task.status = '{TaskStatusEnum.invalid.value}'
-                WITH t, extends_task
+        OPTIONAL MATCH (t:Task {_scoped_key: scoped_key})
 
-                OPTIONAL MATCH (t)<-[ar:ACTIONS]-(th:TaskHub)
-                OPTIONAL MATCH (extends_task)<-[are:ACTIONS]-(th:TaskHub)
+        OPTIONAL MATCH (t_:Task {_scoped_key: scoped_key})
+        WHERE NOT t_.status IN ['deleted']
+        SET t_.status = 'invalid'
 
-                DELETE ar
-                DELETE are
+        WITH scoped_key, t, t_
 
-                WITH t
+        OPTIONAL MATCH (t_)<-[er:EXTENDS*]-(extends_task:Task)
+        SET extends_task.status = 'invalid'
 
-                // drop CLAIMS relationship if present
-                OPTIONAL MATCH (t)<-[cl:CLAIMS]-(csreg:ComputeServiceRegistration)
-                DELETE cl
-                """
-                tx.run(q)
+        WITH scoped_key, t, t_, extends_task
 
-        return tasks
+        OPTIONAL MATCH (t_)<-[ar:ACTIONS]-(th:TaskHub)
+        OPTIONAL MATCH (extends_task)<-[are:ACTIONS]-(th:TaskHub)
+
+        DELETE ar
+        DELETE are
+
+        WITH scoped_key, t, t_
+
+        // drop CLAIMS relationship if present
+        OPTIONAL MATCH (t_)<-[cl:CLAIMS]-(csreg:ComputeServiceRegistration)
+        DELETE cl
+
+        RETURN scoped_key, t, t_
+        """
+
+        def err_msg(t, status):
+            return f"Cannot set task {t} with current status: {status} to `invalid` as it is `deleted`."
+
+        return self._set_task_status(tasks, q, err_msg, raise_error=raise_error)
 
     def set_task_deleted(
         self, tasks: List[ScopedKey], raise_error: bool = False
     ) -> List[Optional[ScopedKey]]:
         """Set the status of a list of Tasks to `deleted`.
 
         Any Task can be set to `deleted`; a `deleted` Task cannot change to
         any other status.
 
         """
 
-        with self.transaction() as tx:
-            for t in tasks:
-                # set the status and delete the ACTIONS relationship
-                # make sure we follow the extends chain and set all tasks to deleted
-                # and remove actions relationships
-                q = f"""
-                MATCH (t:Task {{_scoped_key: '{t}'}})
+        # set the status and delete the ACTIONS relationship
+        # make sure we follow the extends chain and set all tasks to deleted
+        # and remove actions relationships
+        q = """
+        WITH $scoped_keys AS batch
+        UNWIND batch AS scoped_key
 
-                // EXTENDS* used to get all tasks in the extends chain
-                OPTIONAL MATCH (t)<-[er:EXTENDS*]-(extends_task:Task)
-                SET t.status = '{TaskStatusEnum.deleted.value}'
-                SET extends_task.status = '{TaskStatusEnum.deleted.value}'
-                WITH t, extends_task
+        OPTIONAL MATCH (t:Task {_scoped_key: scoped_key})
 
-                OPTIONAL MATCH (t)<-[ar:ACTIONS]-(th:TaskHub)
-                OPTIONAL MATCH (extends_task)<-[are:ACTIONS]-(th:TaskHub)
+        OPTIONAL MATCH (t_:Task {_scoped_key: scoped_key})
+        WHERE NOT t_.status IN ['invalid']
+        SET t_.status = 'deleted'
 
-                DELETE ar
-                DELETE are
+        WITH scoped_key, t, t_
 
-                WITH t
+        OPTIONAL MATCH (t_)<-[er:EXTENDS*]-(extends_task:Task)
+        SET extends_task.status = 'deleted'
 
-                // drop CLAIMS relationship if present
-                OPTIONAL MATCH (t)<-[cl:CLAIMS]-(csreg:ComputeServiceRegistration)
-                DELETE cl
-                """
-                tx.run(q)
+        WITH scoped_key, t, t_, extends_task
+
+        OPTIONAL MATCH (t_)<-[ar:ACTIONS]-(th:TaskHub)
+        OPTIONAL MATCH (extends_task)<-[are:ACTIONS]-(th:TaskHub)
+
+        DELETE ar
+        DELETE are
 
-        return tasks
+        WITH scoped_key, t, t_
+
+        // drop CLAIMS relationship if present
+        OPTIONAL MATCH (t_)<-[cl:CLAIMS]-(csreg:ComputeServiceRegistration)
+        DELETE cl
+
+        RETURN scoped_key, t, t_
+        """
+
+        def err_msg(t, status):
+            return f"Cannot set task {t} with current status: {status} to `deleted` as it is `invalid`."
+
+        return self._set_task_status(tasks, q, err_msg, raise_error=raise_error)
 
     ## authentication
 
     def create_credentialed_entity(self, entity: CredentialedEntity):
         """Create a new credentialed entity, such as a user or compute identity.
 
         If an entity of this type with the same `identifier` already exists,
```

### Comparing `alchemiscale-0.1.2/alchemiscale.egg-info/PKG-INFO` & `alchemiscale-0.1.3/alchemiscale.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: alchemiscale
-Version: 0.1.2
-Home-page: https://github.com/openforcefield/alchemiscale
+Version: 0.1.3
 Author: OpenFE and OpenFF developers
 License: MIT
+Project-URL: Homepage, https://github.com/openforcefield/alchemiscale
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Requires-Python: >=3.9
+Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 # alchemiscale
 
 [![build](https://github.com/openforcefield/alchemiscale/actions/workflows/ci-integration.yml/badge.svg)](https://github.com/openforcefield/alchemiscale/actions/workflows/ci-integration.yml)
 [![coverage](https://codecov.io/gh/openforcefield/alchemiscale/branch/main/graph/badge.svg)](https://codecov.io/gh/openforcefield/alchemiscale)
```

### Comparing `alchemiscale-0.1.2/alchemiscale.egg-info/SOURCES.txt` & `alchemiscale-0.1.3/alchemiscale.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,11 @@
 LICENSE
-MANIFEST.in
 README.md
-setup.cfg
-setup.py
-versioneer.py
+pyproject.toml
 alchemiscale/__init__.py
-alchemiscale/_version.py
 alchemiscale/cli.py
 alchemiscale/cli_utils.py
 alchemiscale/models.py
 alchemiscale/settings.py
 alchemiscale.egg-info/PKG-INFO
 alchemiscale.egg-info/SOURCES.txt
 alchemiscale.egg-info/dependency_links.txt
```

