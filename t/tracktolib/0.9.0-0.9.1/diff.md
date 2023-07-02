# Comparing `tmp/tracktolib-0.9.0.tar.gz` & `tmp/tracktolib-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tracktolib-0.9.0.tar", max compression
+gzip compressed data, was "tracktolib-0.9.1.tar", max compression
```

## Comparing `tracktolib-0.9.0.tar` & `tracktolib-0.9.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1081 2022-11-18 08:55:03.805383 tracktolib-0.9.0/LICENSE
--rw-r--r--   0        0        0     1441 2022-11-18 08:55:03.805383 tracktolib-0.9.0/README.md
--rw-r--r--   0        0        0     1515 2022-11-18 08:55:07.757393 tracktolib-0.9.0/pyproject.toml
--rw-r--r--   0        0        0        0 2022-11-18 08:55:03.809383 tracktolib-0.9.0/tracktolib/__init__.py
--rw-r--r--   0        0        0     3980 2022-11-18 08:55:03.809383 tracktolib-0.9.0/tracktolib/api.py
--rw-r--r--   0        0        0     1138 2022-11-18 08:55:03.809383 tracktolib-0.9.0/tracktolib/http.py
--rw-r--r--   0        0        0     2392 2022-11-18 08:55:03.809383 tracktolib-0.9.0/tracktolib/logs.py
--rw-r--r--   0        0        0     3229 2022-11-18 08:55:03.809383 tracktolib-0.9.0/tracktolib/pg_sync.py
--rw-r--r--   0        0        0        0 2022-11-18 08:55:03.809383 tracktolib-0.9.0/tracktolib/s3/__init__.py
--rw-r--r--   0        0        0     1249 2022-11-18 08:55:03.809383 tracktolib-0.9.0/tracktolib/s3/minio.py
--rw-r--r--   0        0        0     1431 2022-11-18 08:55:03.809383 tracktolib-0.9.0/tracktolib/s3/s3.py
--rw-r--r--   0        0        0      387 2022-11-18 08:55:03.809383 tracktolib-0.9.0/tracktolib/tests.py
--rw-r--r--   0        0        0     1540 2022-11-18 08:55:03.809383 tracktolib-0.9.0/tracktolib/utils.py
--rw-r--r--   0        0        0     2181 1970-01-01 00:00:00.000000 tracktolib-0.9.0/setup.py
--rw-r--r--   0        0        0     2110 1970-01-01 00:00:00.000000 tracktolib-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1081 2022-11-18 16:12:17.346751 tracktolib-0.9.1/LICENSE
+-rw-r--r--   0        0        0     1441 2022-11-18 16:12:17.346751 tracktolib-0.9.1/README.md
+-rw-r--r--   0        0        0     1668 2022-11-18 16:12:22.770756 tracktolib-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-11-18 16:12:17.350751 tracktolib-0.9.1/tracktolib/__init__.py
+-rw-r--r--   0        0        0     3980 2022-11-18 16:12:17.350751 tracktolib-0.9.1/tracktolib/api.py
+-rw-r--r--   0        0        0     1138 2022-11-18 16:12:17.350751 tracktolib-0.9.1/tracktolib/http.py
+-rw-r--r--   0        0        0     2503 2022-11-18 16:12:17.350751 tracktolib-0.9.1/tracktolib/logs.py
+-rw-r--r--   0        0        0     3209 2022-11-18 16:12:17.350751 tracktolib-0.9.1/tracktolib/pg_sync.py
+-rw-r--r--   0        0        0        0 2022-11-18 16:12:17.350751 tracktolib-0.9.1/tracktolib/s3/__init__.py
+-rw-r--r--   0        0        0     1249 2022-11-18 16:12:17.350751 tracktolib-0.9.1/tracktolib/s3/minio.py
+-rw-r--r--   0        0        0     1431 2022-11-18 16:12:17.350751 tracktolib-0.9.1/tracktolib/s3/s3.py
+-rw-r--r--   0        0        0      387 2022-11-18 16:12:17.350751 tracktolib-0.9.1/tracktolib/tests.py
+-rw-r--r--   0        0        0     1517 2022-11-18 16:12:17.350751 tracktolib-0.9.1/tracktolib/utils.py
+-rw-r--r--   0        0        0     2413 1970-01-01 00:00:00.000000 tracktolib-0.9.1/setup.py
+-rw-r--r--   0        0        0     2633 1970-01-01 00:00:00.000000 tracktolib-0.9.1/PKG-INFO
```

### Comparing `tracktolib-0.9.0/LICENSE` & `tracktolib-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tracktolib-0.9.0/README.md` & `tracktolib-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `tracktolib-0.9.0/tracktolib/api.py` & `tracktolib-0.9.1/tracktolib/api.py`

 * *Files identical despite different names*

### Comparing `tracktolib-0.9.0/tracktolib/http.py` & `tracktolib-0.9.1/tracktolib/http.py`

 * *Files identical despite different names*

### Comparing `tracktolib-0.9.0/tracktolib/logs.py` & `tracktolib-0.9.1/tracktolib/logs.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 import logging
 from typing import Literal, overload, Any, TypeGuard
-from pythonjsonlogger import jsonlogger
 from dataclasses import dataclass
 
+try:
+    from pythonjsonlogger import jsonlogger
+except ImportError:
+    raise ImportError('Please install tracktolib with "log" to use this module')
+
 LogFormat = Literal['json', 'console']
 
 
 @dataclass
 class CustomJsonFormatter(jsonlogger.JsonFormatter):
     version: str
```

### Comparing `tracktolib-0.9.0/tracktolib/pg_sync.py` & `tracktolib-0.9.1/tracktolib/pg_sync.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Iterable, Any
+from typing import Iterable, Any, overload, Literal
 
 try:
     from psycopg2.errors import InvalidCatalogName
     from psycopg2.extensions import connection
 except ImportError:
     raise ImportError('Please install tracktolib with "pg-sync" to use this module')
 
@@ -22,17 +22,14 @@
     with engine.cursor() as cur:
         cur.execute(query)
         count = cur.fetchone()
 
     return count[0] if count else None
 
 
-from typing import overload, Literal
-
-
 @overload
 def fetch_one(engine: connection, query: str, *args,
               required: Literal[False]) -> dict | None: ...
 
 
 @overload
 def fetch_one(engine: connection, query: str, *args,
```

### Comparing `tracktolib-0.9.0/tracktolib/s3/minio.py` & `tracktolib-0.9.1/tracktolib/s3/minio.py`

 * *Files identical despite different names*

### Comparing `tracktolib-0.9.0/tracktolib/s3/s3.py` & `tracktolib-0.9.1/tracktolib/s3/s3.py`

 * *Files identical despite different names*

### Comparing `tracktolib-0.9.0/tracktolib/utils.py` & `tracktolib-0.9.1/tracktolib/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,11 +43,9 @@
         yield d if not as_list else list(d)
 
 
 def json_serial(obj):
     """ JSON serializer for objects not serializable by default json code """
     if isinstance(obj, (dt.datetime, dt.date)):
         return obj.isoformat()
-    else:
-        pass
 
     raise TypeError(f"Type '{type(obj)}' not serializable")
```

### Comparing `tracktolib-0.9.0/setup.py` & `tracktolib-0.9.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,28 +3,34 @@
 
 packages = \
 ['tracktolib', 'tracktolib.s3']
 
 package_data = \
 {'': ['*']}
 
-install_requires = \
-['python-json-logger>=2.0.4,<3.0.0']
+extras_require = \
+{'api': ['fastapi>=0.87.0,<0.88.0'],
+ 'http': ['httpx>=0.23.0,<0.24.0'],
+ 'logs': ['python-json-logger>=2.0.4,<3.0.0'],
+ 'pg-sync': ['psycopg2>=2.9.5,<3.0.0'],
+ 's3': ['aiobotocore>=2.4.0,<3.0.0'],
+ 's3-minio': ['minio>=7.1.12,<8.0.0'],
+ 'tests': ['deepdiff>=6.2.1,<7.0.0']}
 
 setup_kwargs = {
     'name': 'tracktolib',
-    'version': '0.9.0',
+    'version': '0.9.1',
     'description': 'Utility library for python',
     'long_description': '# Tracktolib\n\n[![Python versions](https://img.shields.io/pypi/pyversions/tracktolib)](https://pypi.python.org/pypi/tracktolib)\n[![Latest PyPI version](https://img.shields.io/pypi/v/tracktolib?logo=pypi)](https://pypi.python.org/pypi/tracktolib)\n[![CircleCI](https://circleci.com/gh/Tracktor/tracktolib/tree/master.svg?style=shield)](https://app.circleci.com/pipelines/github/Tracktor/tracktolib?branch=master)\n\nUtility library for python\n\n# Installation\n\nYou can choose to not install all the dependencies by specifying\nthe [extra](https://python-poetry.org/docs/cli/#options-4) parameter such as:\n\n```bash\npoetry add tracktolib@latest -E pg-sync -E tests --group dev \n```\n\nHere we only install the utilities using `psycopg2` (pg-sync) and `deepdiff` (tests) for the dev environment.\n\n# Utilities\n\n- **pg-sync**\n\nUtility functions based on psycopg2 such as `fetch_one`, `insert_many`, `fetch_count` ...\n\n- **tests**\n\nUtility functions for tests such as `get_uuid` (that generates a test uuid based on an integer)\n\n- **s3-minio**\n\nUtility functions for [minio](https://min.io/docs/minio/linux/developers/python/API.html)\n\n- **s3**\n\nUtility functions for [aiobotocore](https://github.com/aio-libs/aiobotocore)\n\n- **logs**\n\nUtility functions to initialize the logging formatting and streams\n\n- **http**\n\nUtility functions using [httpx](https://www.python-httpx.org/)\n\n- **api**\n\nUtility functions using [fastapi](https://fastapi.tiangolo.com/)\n',
     'author': 'Julien Brayere',
     'author_email': 'julien.brayere@tracktor.fr',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/tracktor/tracktolib',
     'packages': packages,
     'package_data': package_data,
-    'install_requires': install_requires,
+    'extras_require': extras_require,
     'python_requires': '>=3.10,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

