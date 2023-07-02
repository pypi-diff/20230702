# Comparing `tmp/kaiju_tasks-2.1.2-py3-none-any.whl.zip` & `tmp/kaiju_tasks-2.1.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 18305 bytes, number of entries: 15
--rw-r--r--  2.0 unx      131 b- defN 23-Jun-30 16:29 kaiju_tasks/__init__.py
--rw-r--r--  2.0 unx    37518 b- defN 23-Jun-30 16:29 kaiju_tasks/services.py
--rw-r--r--  2.0 unx     4360 b- defN 23-Jun-30 16:29 kaiju_tasks/types.py
--rw-r--r--  2.0 unx       38 b- defN 23-Jun-30 16:29 kaiju_tasks/tasks_gui/__init__.py
--rw-r--r--  2.0 unx     2011 b- defN 23-Jun-30 16:29 kaiju_tasks/tasks_gui/models.py
--rw-r--r--  2.0 unx     4272 b- defN 23-Jun-30 16:29 kaiju_tasks/tasks_gui/service.py
--rw-r--r--  2.0 unx      350 b- defN 23-Jun-30 16:29 kaiju_tasks/tasks_gui/validators.py
--rw-r--r--  2.0 unx       42 b- defN 23-Jun-30 16:29 kaiju_tasks/tests/__init__.py
--rw-r--r--  2.0 unx     2058 b- defN 23-Jun-30 16:29 kaiju_tasks/tests/fixtures.py
--rw-r--r--  2.0 unx    12224 b- defN 23-Jun-30 16:29 kaiju_tasks/tests/test_tasks.py
--rw-rw-rw-  2.0 unx      610 b- defN 23-Jun-30 16:30 kaiju_tasks-2.1.2.dist-info/LICENSE
--rw-r--r--  2.0 unx     3056 b- defN 23-Jun-30 16:30 kaiju_tasks-2.1.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-30 16:30 kaiju_tasks-2.1.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 23-Jun-30 16:30 kaiju_tasks-2.1.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1257 b- defN 23-Jun-30 16:30 kaiju_tasks-2.1.2.dist-info/RECORD
-15 files, 68031 bytes uncompressed, 16213 bytes compressed:  76.2%
+Zip file size: 18291 bytes, number of entries: 15
+-rw-r--r--  2.0 unx      131 b- defN 23-Jul-02 13:03 kaiju_tasks/__init__.py
+-rw-r--r--  2.0 unx    37494 b- defN 23-Jul-02 13:03 kaiju_tasks/services.py
+-rw-r--r--  2.0 unx     4360 b- defN 23-Jul-02 13:03 kaiju_tasks/types.py
+-rw-r--r--  2.0 unx       38 b- defN 23-Jul-02 13:03 kaiju_tasks/tasks_gui/__init__.py
+-rw-r--r--  2.0 unx     2011 b- defN 23-Jul-02 13:03 kaiju_tasks/tasks_gui/models.py
+-rw-r--r--  2.0 unx     4272 b- defN 23-Jul-02 13:03 kaiju_tasks/tasks_gui/service.py
+-rw-r--r--  2.0 unx      350 b- defN 23-Jul-02 13:03 kaiju_tasks/tasks_gui/validators.py
+-rw-r--r--  2.0 unx       42 b- defN 23-Jul-02 13:03 kaiju_tasks/tests/__init__.py
+-rw-r--r--  2.0 unx     2058 b- defN 23-Jul-02 13:03 kaiju_tasks/tests/fixtures.py
+-rw-r--r--  2.0 unx    12224 b- defN 23-Jul-02 13:03 kaiju_tasks/tests/test_tasks.py
+-rw-rw-rw-  2.0 unx      610 b- defN 23-Jul-02 13:03 kaiju_tasks-2.1.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2944 b- defN 23-Jul-02 13:03 kaiju_tasks-2.1.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-02 13:03 kaiju_tasks-2.1.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 23-Jul-02 13:03 kaiju_tasks-2.1.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1257 b- defN 23-Jul-02 13:03 kaiju_tasks-2.1.3.dist-info/RECORD
+15 files, 67895 bytes uncompressed, 16199 bytes compressed:  76.1%
```

## zipnote {}

```diff
@@ -24,23 +24,23 @@
 
 Filename: kaiju_tasks/tests/fixtures.py
 Comment: 
 
 Filename: kaiju_tasks/tests/test_tasks.py
 Comment: 
 
-Filename: kaiju_tasks-2.1.2.dist-info/LICENSE
+Filename: kaiju_tasks-2.1.3.dist-info/LICENSE
 Comment: 
 
-Filename: kaiju_tasks-2.1.2.dist-info/METADATA
+Filename: kaiju_tasks-2.1.3.dist-info/METADATA
 Comment: 
 
-Filename: kaiju_tasks-2.1.2.dist-info/WHEEL
+Filename: kaiju_tasks-2.1.3.dist-info/WHEEL
 Comment: 
 
-Filename: kaiju_tasks-2.1.2.dist-info/top_level.txt
+Filename: kaiju_tasks-2.1.3.dist-info/top_level.txt
 Comment: 
 
-Filename: kaiju_tasks-2.1.2.dist-info/RECORD
+Filename: kaiju_tasks-2.1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## kaiju_tasks/__init__.py

```diff
@@ -1,6 +1,6 @@
 from .types import *
 from .services import *
 
-__version__ = '2.1.2'
+__version__ = '2.1.3'
 __python_version__ = '3.8'
 __author__ = 'antonnidhoggr@me.com'
```

## kaiju_tasks/services.py

```diff
@@ -5,15 +5,15 @@
 from typing import Any, List
 
 import sqlalchemy as sa
 import sqlalchemy.dialects.postgresql as sa_pg
 from croniter import croniter
 
 import kaiju_tools.jsonschema as j
-from kaiju_tools.app import ContextableService, Scheduler, service_class_registry
+from kaiju_tools.app import ContextableService, Scheduler, SERVICE_CLASS_REGISTRY
 from kaiju_tools.exceptions import ValidationError, InternalError
 from kaiju_tools.interfaces import PublicInterface
 from kaiju_tools.functions import get_short_uid, retry
 from kaiju_tools.streams import StreamRPCClient, Topic
 from kaiju_tools.templates import Template
 from kaiju_tools.rpc import JSONRPCServer, JSONRPCHeaders, RPCError
 from kaiju_tools.types import Scope
@@ -911,11 +911,11 @@
             ),
             retries=3,
             retry_timeout=1,
             logger=self.logger,
         )
 
 
-service_class_registry.register_class(TaskService)
-service_class_registry.register_class(NotificationService)
-service_class_registry.register_class(TaskManager)
-service_class_registry.register_class(TaskExecutor)
+SERVICE_CLASS_REGISTRY.register(TaskService)
+SERVICE_CLASS_REGISTRY.register(NotificationService)
+SERVICE_CLASS_REGISTRY.register(TaskManager)
+SERVICE_CLASS_REGISTRY.register(TaskExecutor)
```

## Comparing `kaiju_tasks-2.1.2.dist-info/LICENSE` & `kaiju_tasks-2.1.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `kaiju_tasks-2.1.2.dist-info/METADATA` & `kaiju_tasks-2.1.3.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kaiju-tasks
-Version: 2.1.2
+Version: 2.1.3
 Summary: Service and user task management
 Home-page: https://gitlab.com/kaiju-python/kaiju-tasks
 Author: antonnidhoggr@me.com
 Author-email: antonnidhoggr@me.com
 License: Apache Software License 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
@@ -21,30 +21,27 @@
 Requires-Dist: croniter (>=1.4.1)
 Requires-Dist: kaiju-tools (<3,>=2)
 Requires-Dist: kaiju-db (<3,>=2)
 Requires-Dist: kaiju-redis (<3,>=2)
 Provides-Extra: dev
 Requires-Dist: bump2version (>=1.0) ; extra == 'dev'
 Requires-Dist: pyroma (>=4.1) ; extra == 'dev'
-Requires-Dist: bandit (==1.7) ; extra == 'dev'
+Requires-Dist: bandit (>=1.7) ; extra == 'dev'
 Requires-Dist: black (>=22.12) ; extra == 'dev'
 Requires-Dist: flake8 (>=6.0) ; extra == 'dev'
 Requires-Dist: pyproject-flake8 ; extra == 'dev'
 Requires-Dist: pre-commit (>=3.1) ; extra == 'dev'
 Requires-Dist: pydocstyle (>=6.2) ; extra == 'dev'
 Requires-Dist: setup-cfg-fmt (>=2.2) ; extra == 'dev'
 Requires-Dist: restructuredtext-lint (>=1.4) ; extra == 'dev'
 Requires-Dist: tox (>=3.28) ; extra == 'dev'
 Requires-Dist: tox-pyenv (>=1.1) ; extra == 'dev'
 Requires-Dist: pip-tools (>=6.13) ; extra == 'dev'
 Requires-Dist: towncrier (>=23.6) ; extra == 'dev'
 Requires-Dist: pyupgrade (>=3.4) ; extra == 'dev'
-Provides-Extra: docs
-Requires-Dist: sphinx ; extra == 'docs'
-Requires-Dist: python-docs-theme ; extra == 'docs'
 Provides-Extra: test
 Requires-Dist: pytest (>=7.2) ; extra == 'test'
 Requires-Dist: pytest-asyncio (>=0.20) ; extra == 'test'
 Requires-Dist: docker (>=6.0) ; extra == 'test'
 Requires-Dist: pytest-timeout (>=2.1) ; extra == 'test'
```

## Comparing `kaiju_tasks-2.1.2.dist-info/RECORD` & `kaiju_tasks-2.1.3.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-kaiju_tasks/__init__.py,sha256=8DSTDuF26lO6QQluj4ZgjADvGIXDPHlNRgW9scwh6HE,131
-kaiju_tasks/services.py,sha256=dDqf5ydswVbQxaxB-SmIUl-r-2ineSabshAx14goJ_w,37518
+kaiju_tasks/__init__.py,sha256=27X9yp9XJDz9_Cm77AJ7szUnYjKOJghF8AHKDNpRYvs,131
+kaiju_tasks/services.py,sha256=UY3LvImaGK222lNdySKyJUo8D7lzJjqAFvkUSCvj--Q,37494
 kaiju_tasks/types.py,sha256=tp6fm6GJv8B5B6YhhiiZIbf00ahIBHUqaZNEQJFXEuw,4360
 kaiju_tasks/tasks_gui/__init__.py,sha256=_gDfM5r8uxCvydv3NOUN21imwJW_NW9R16UXWExQAE8,38
 kaiju_tasks/tasks_gui/models.py,sha256=iXqYnYYh8TJ7jkVxyEmMeykfpmoNfEfEERW-1jwzjsk,2011
 kaiju_tasks/tasks_gui/service.py,sha256=_qCURg-h6I9OI5uZdTGYCzJglXPXomcqAt6D7ODLRmU,4272
 kaiju_tasks/tasks_gui/validators.py,sha256=QybfHwKMWJq9AcGlXO7F5fuEGLssjHN2jcAV0UI6FPc,350
 kaiju_tasks/tests/__init__.py,sha256=WlPruePOcaMi5ikqn6GheE1Z-zYcysb9M1dj6SteWGY,42
 kaiju_tasks/tests/fixtures.py,sha256=1WRWnb5aCklCpRo0iqp1rquZSB8qgKBULv5MhaO2rck,2058
 kaiju_tasks/tests/test_tasks.py,sha256=YvmLscWAwko7eQ2Jw4vXTrO7SkefFu_P8eOEMNT-lkk,12224
-kaiju_tasks-2.1.2.dist-info/LICENSE,sha256=XIlN2qA8UqpBDA-PteoYP4hTU0qBW0G9PRB__khO2zc,610
-kaiju_tasks-2.1.2.dist-info/METADATA,sha256=V5-rqyn0UshFZEgXiCOxubapGze8tv5CKme92ncDRMU,3056
-kaiju_tasks-2.1.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-kaiju_tasks-2.1.2.dist-info/top_level.txt,sha256=QyLogqOVVajJlalq6RfikGx5VGn_lLeTANJEsfZZlM0,12
-kaiju_tasks-2.1.2.dist-info/RECORD,,
+kaiju_tasks-2.1.3.dist-info/LICENSE,sha256=XIlN2qA8UqpBDA-PteoYP4hTU0qBW0G9PRB__khO2zc,610
+kaiju_tasks-2.1.3.dist-info/METADATA,sha256=kWbYaN2uD1LzooXo7bX4T3LocT4vvz-tsoIH4_2fxwY,2944
+kaiju_tasks-2.1.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+kaiju_tasks-2.1.3.dist-info/top_level.txt,sha256=QyLogqOVVajJlalq6RfikGx5VGn_lLeTANJEsfZZlM0,12
+kaiju_tasks-2.1.3.dist-info/RECORD,,
```

