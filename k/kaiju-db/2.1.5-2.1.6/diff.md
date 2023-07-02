# Comparing `tmp/kaiju_db-2.1.5-py3-none-any.whl.zip` & `tmp/kaiju_db-2.1.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 19995 bytes, number of entries: 12
--rw-r--r--  2.0 unx      183 b- defN 23-Jun-30 16:21 kaiju_db/__init__.py
--rw-r--r--  2.0 unx     3665 b- defN 23-Jun-30 16:21 kaiju_db/functions.py
--rw-r--r--  2.0 unx    58628 b- defN 23-Jun-30 16:21 kaiju_db/services.py
--rw-r--r--  2.0 unx      453 b- defN 23-Jun-30 16:21 kaiju_db/types.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-30 16:21 kaiju_db/tests/__init__.py
--rw-r--r--  2.0 unx     3292 b- defN 23-Jun-30 16:21 kaiju_db/tests/fixtures.py
--rw-r--r--  2.0 unx     4831 b- defN 23-Jun-30 16:21 kaiju_db/tests/test_db.py
--rw-rw-rw-  2.0 unx      610 b- defN 23-Jun-30 16:21 kaiju_db-2.1.5.dist-info/LICENSE
--rw-r--r--  2.0 unx     3090 b- defN 23-Jun-30 16:21 kaiju_db-2.1.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-30 16:21 kaiju_db-2.1.5.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 23-Jun-30 16:21 kaiju_db-2.1.5.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      939 b- defN 23-Jun-30 16:21 kaiju_db-2.1.5.dist-info/RECORD
-12 files, 75792 bytes uncompressed, 18423 bytes compressed:  75.7%
+Zip file size: 20047 bytes, number of entries: 12
+-rw-r--r--  2.0 unx      183 b- defN 23-Jul-02 12:41 kaiju_db/__init__.py
+-rw-r--r--  2.0 unx     3740 b- defN 23-Jul-02 12:41 kaiju_db/functions.py
+-rw-r--r--  2.0 unx    58600 b- defN 23-Jul-02 12:41 kaiju_db/services.py
+-rw-r--r--  2.0 unx      453 b- defN 23-Jul-02 12:41 kaiju_db/types.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-02 12:41 kaiju_db/tests/__init__.py
+-rw-r--r--  2.0 unx     3292 b- defN 23-Jul-02 12:41 kaiju_db/tests/fixtures.py
+-rw-r--r--  2.0 unx     4831 b- defN 23-Jul-02 12:41 kaiju_db/tests/test_db.py
+-rw-rw-rw-  2.0 unx      610 b- defN 23-Jul-02 12:41 kaiju_db-2.1.6.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3090 b- defN 23-Jul-02 12:41 kaiju_db-2.1.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-02 12:41 kaiju_db-2.1.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 23-Jul-02 12:41 kaiju_db-2.1.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      939 b- defN 23-Jul-02 12:41 kaiju_db-2.1.6.dist-info/RECORD
+12 files, 75839 bytes uncompressed, 18475 bytes compressed:  75.6%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: kaiju_db/tests/fixtures.py
 Comment: 
 
 Filename: kaiju_db/tests/test_db.py
 Comment: 
 
-Filename: kaiju_db-2.1.5.dist-info/LICENSE
+Filename: kaiju_db-2.1.6.dist-info/LICENSE
 Comment: 
 
-Filename: kaiju_db-2.1.5.dist-info/METADATA
+Filename: kaiju_db-2.1.6.dist-info/METADATA
 Comment: 
 
-Filename: kaiju_db-2.1.5.dist-info/WHEEL
+Filename: kaiju_db-2.1.6.dist-info/WHEEL
 Comment: 
 
-Filename: kaiju_db-2.1.5.dist-info/top_level.txt
+Filename: kaiju_db-2.1.6.dist-info/top_level.txt
 Comment: 
 
-Filename: kaiju_db-2.1.5.dist-info/RECORD
+Filename: kaiju_db-2.1.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## kaiju_db/__init__.py

```diff
@@ -1,8 +1,8 @@
 from .types import *
 from .functions import *
 from .services import *
 
-__version__ = '2.1.5'
+__version__ = '2.1.6'
 __python_version__ = '3.8'
 __author__ = 'antonnidhoggr@me.com'
 __service_package__ = True
```

## kaiju_db/functions.py

```diff
@@ -1,15 +1,17 @@
+from typing import Tuple, Type
+
 from sqlalchemy import DDL
 from sqlalchemy.event import listen
 from sqlalchemy.sql.functions import GenericFunction
 
-from kaiju_tools.class_registry import AbstractClassRegistry
+from kaiju_tools.registry import ClassRegistry
 
 
-__all__ = ['DDL', 'UserFunction', 'FunctionsRegistry', 'functions_registry']
+__all__ = ['DDL', 'UserFunction', 'SQLFunctionsRegistry', 'SQL_FUNCTIONS']
 
 
 def DDL(target, identifier, body):  # noqa
     """
     Specifies literal SQL DDL to be executed by the database.  DDL objects
     function as DDL event listeners, and can be subscribed to those events
     listed in :class:`.DDLEvents`, using either :class:`.Table` or
@@ -112,18 +114,20 @@
         if not body.lower().startswith('function'):
             body = f'FUNCTION {body}'
         if not body.endswith(';'):
             body += ';'
         return body
 
 
-class FunctionsRegistry(AbstractClassRegistry):
+class SQLFunctionsRegistry(ClassRegistry):
     """A simple registry for SQL functions."""
 
-    base_classes = (UserFunction,)
+    @classmethod
+    def get_base_classes(cls) -> Tuple[Type, ...]:
+        return (UserFunction,)
 
-    @staticmethod
-    def class_key(obj) -> str:
+    @classmethod
+    def get_key(cls, obj) -> str:
         return obj.name
 
 
-functions_registry = FunctionsRegistry(raise_if_exists=False)
+SQL_FUNCTIONS = SQLFunctionsRegistry(raise_if_exists=False)
```

## kaiju_db/services.py

```diff
@@ -21,19 +21,19 @@
 import sqlalchemy as sa
 import sqlalchemy.dialects.postgresql as sa_pg
 from sqlalchemy.exc import IntegrityError
 from sqlalchemy.sql.expression import nullslast
 from sqlalchemy import MetaData, text, Table  # noqa pycharm
 from sqlalchemy.ext.asyncio import create_async_engine  # noqa pycharm
 
-from kaiju_tools.app import ContextableService, service_class_registry, Service
+from kaiju_tools.app import ContextableService, SERVICE_CLASS_REGISTRY, Service
 from kaiju_tools.interfaces import DataStore, Locks
 from kaiju_tools.exceptions import ValidationError, NotFound, Conflict, InternalError, MethodNotAllowed
 from kaiju_tools.serialization import dumps, loads, load
-from kaiju_db.functions import functions_registry, UserFunction
+from kaiju_db.functions import SQL_FUNCTIONS, UserFunction
 
 __all__ = ['DatabaseService', 'SQLService', 'FixtureService', 'DatabaseMigrationService']
 
 
 class DatabaseService(ContextableService):
     """Postgresql database transport service.
 
@@ -57,15 +57,15 @@
         root_database: str = 'postgres',
         metadata: MetaData = None,
         init_db: bool = True,
         init_tables: bool = True,
         pool_size: int = 10,
         idle_connection_lifetime: int = 3600,
         extensions: List[str] = None,
-        functions=functions_registry,
+        functions=SQL_FUNCTIONS,
         logger=None,
     ):
         """Initialize.
 
         :param app:
         :param host: db url or address
         :param port: db port
@@ -1514,10 +1514,10 @@
             await self._db.execute(sql)
             state_id = self._null_state
         else:
             state_id = state['value']
         return state_id
 
 
-service_class_registry.register_class(DatabaseService)
-service_class_registry.register_class(DatabaseMigrationService)
-service_class_registry.register_class(FixtureService)
+SERVICE_CLASS_REGISTRY.register(DatabaseService)
+SERVICE_CLASS_REGISTRY.register(DatabaseMigrationService)
+SERVICE_CLASS_REGISTRY.register(FixtureService)
```

## Comparing `kaiju_db-2.1.5.dist-info/LICENSE` & `kaiju_db-2.1.6.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `kaiju_db-2.1.5.dist-info/METADATA` & `kaiju_db-2.1.6.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kaiju-db
-Version: 2.1.5
+Version: 2.1.6
 Summary: Postgresql db services and tools
 Home-page: https://gitlab.com/kaiju-python/kaiju-db
 Author: antonnidhoggr@me.com
 Author-email: antonnidhoggr@me.com
 License: Apache Software License 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: asyncpg (>=0.27)
 Requires-Dist: greenlet (>=2.0.2)
-Requires-Dist: sqlalchemy[asyncio] (>=2.0.16)
+Requires-Dist: sqlalchemy[asyncio] (>=2.0.17)
 Requires-Dist: sqlalchemy-utils (>=0.41)
 Requires-Dist: kaiju-tools (<3,>=2)
 Provides-Extra: dev
 Requires-Dist: bump2version (>=1.0) ; extra == 'dev'
 Requires-Dist: pyroma (>=4.1) ; extra == 'dev'
 Requires-Dist: bandit (>=1.7) ; extra == 'dev'
 Requires-Dist: black (>=22.12) ; extra == 'dev'
```

## Comparing `kaiju_db-2.1.5.dist-info/RECORD` & `kaiju_db-2.1.6.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-kaiju_db/__init__.py,sha256=1K0i6dyo1Hy5aXGpN0c8F-7sdpRJMbdlm21LX_SCqJI,183
-kaiju_db/functions.py,sha256=0E7H85QZkRvPBMa6H5n9eC5tJlCvKXPvKT6e5O-nuGQ,3665
-kaiju_db/services.py,sha256=z8s2dv_4GpSbwwsnddVDtGnWLAET2NUuk5reKb3gYro,58628
+kaiju_db/__init__.py,sha256=2MOZHhk3aIA1AoTXcMAaxtqt0zC7zbSW-2IVff_KfNk,183
+kaiju_db/functions.py,sha256=JUHNd5uYbEtziTsihE-iPctYraUC-S3pfC2mo3EmtPo,3740
+kaiju_db/services.py,sha256=HZb-sQ46dcho6BuFm-lcolpb3j4jdJh3otj7ZbuoVvU,58600
 kaiju_db/types.py,sha256=0ORvc2CaCcKUNibTR5o9EI5DOFQjM_uDg5S58aF8MyU,453
 kaiju_db/tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 kaiju_db/tests/fixtures.py,sha256=XtkmjBFFPbcBdUWNJBiGanrHjrPQW1yYzoC61sxxzD4,3292
 kaiju_db/tests/test_db.py,sha256=0ZAp4UbhAo2sVTCzFa1BhsV5IaXoV2YN3Wr8bzX0vVw,4831
-kaiju_db-2.1.5.dist-info/LICENSE,sha256=XIlN2qA8UqpBDA-PteoYP4hTU0qBW0G9PRB__khO2zc,610
-kaiju_db-2.1.5.dist-info/METADATA,sha256=3GJR2xKkqtFhZdcr8a7874lLkErNlcy0tGPQigsbDaw,3090
-kaiju_db-2.1.5.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-kaiju_db-2.1.5.dist-info/top_level.txt,sha256=-jcfPgSkIz8rxFCPp_XIg5g9tVsDmBd1wdxayb_mkNU,9
-kaiju_db-2.1.5.dist-info/RECORD,,
+kaiju_db-2.1.6.dist-info/LICENSE,sha256=XIlN2qA8UqpBDA-PteoYP4hTU0qBW0G9PRB__khO2zc,610
+kaiju_db-2.1.6.dist-info/METADATA,sha256=uYrOsAZOS3oX7AVSYM_WSNs_N81bZaK_togZGUGNFZM,3090
+kaiju_db-2.1.6.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+kaiju_db-2.1.6.dist-info/top_level.txt,sha256=-jcfPgSkIz8rxFCPp_XIg5g9tVsDmBd1wdxayb_mkNU,9
+kaiju_db-2.1.6.dist-info/RECORD,,
```

