# Comparing `tmp/degiroasync-0.16.0.tar.gz` & `tmp/degiroasync-0.17.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "degiroasync-0.16.0.tar", last modified: Tue May 24 16:36:53 2022, max compression
+gzip compressed data, was "degiroasync-0.17.0.tar", last modified: Sun Jul  2 20:30:08 2023, max compression
```

## Comparing `degiroasync-0.16.0.tar` & `degiroasync-0.17.0.tar`

### file list

```diff
@@ -1,37 +1,38 @@
-drwxrwxr-x   0 laumas    (1000) laumas    (1000)        0 2022-05-24 16:36:53.034070 degiroasync-0.16.0/
--rw-rw-r--   0 laumas    (1000) laumas    (1000)     1075 2022-01-20 21:38:48.000000 degiroasync-0.16.0/LICENSE
--rw-rw-r--   0 laumas    (1000) laumas    (1000)     5243 2022-05-24 16:36:53.034070 degiroasync-0.16.0/PKG-INFO
--rw-rw-r--   0 laumas    (1000) laumas    (1000)     4551 2022-04-30 07:09:43.000000 degiroasync-0.16.0/README.md
-drwxrwxr-x   0 laumas    (1000) laumas    (1000)        0 2022-05-24 16:36:53.026071 degiroasync-0.16.0/degiroasync/
--rw-rw-r--   0 laumas    (1000) laumas    (1000)      692 2022-04-13 19:10:04.000000 degiroasync-0.16.0/degiroasync/__init__.py
-drwxrwxr-x   0 laumas    (1000) laumas    (1000)        0 2022-05-24 16:36:53.030071 degiroasync-0.16.0/degiroasync/api/
--rw-rw-r--   0 laumas    (1000) laumas    (1000)     4268 2022-04-13 18:57:09.000000 degiroasync-0.16.0/degiroasync/api/__init__.py
--rw-rw-r--   0 laumas    (1000) laumas    (1000)     8334 2022-05-12 19:40:07.000000 degiroasync-0.16.0/degiroasync/api/orders.py
--rw-rw-r--   0 laumas    (1000) laumas    (1000)    26181 2022-04-29 20:17:34.000000 degiroasync-0.16.0/degiroasync/api/product.py
--rw-rw-r--   0 laumas    (1000) laumas    (1000)     7065 2022-03-27 17:10:51.000000 degiroasync-0.16.0/degiroasync/api/session.py
-drwxrwxr-x   0 laumas    (1000) laumas    (1000)        0 2022-05-24 16:36:53.030071 degiroasync-0.16.0/degiroasync/core/
--rw-rw-r--   0 laumas    (1000) laumas    (1000)     1330 2022-04-01 17:26:25.000000 degiroasync-0.16.0/degiroasync/core/__init__.py
--rw-rw-r--   0 laumas    (1000) laumas    (1000)     6581 2022-05-02 14:15:42.000000 degiroasync-0.16.0/degiroasync/core/constants.py
--rw-rw-r--   0 laumas    (1000) laumas    (1000)    10999 2022-03-30 18:33:17.000000 degiroasync-0.16.0/degiroasync/core/core.py
--rw-rw-r--   0 laumas    (1000) laumas    (1000)        0 2022-03-08 13:07:34.000000 degiroasync-0.16.0/degiroasync/core/exceptions.py
--rw-rw-r--   0 laumas    (1000) laumas    (1000)    11694 2022-05-12 15:30:54.000000 degiroasync-0.16.0/degiroasync/core/helpers.py
-drwxrwxr-x   0 laumas    (1000) laumas    (1000)        0 2022-05-24 16:36:53.030071 degiroasync-0.16.0/degiroasync/webapi/
--rw-rw-r--   0 laumas    (1000) laumas    (1000)     1853 2022-04-05 15:36:45.000000 degiroasync-0.16.0/degiroasync/webapi/__init__.py
--rw-rw-r--   0 laumas    (1000) laumas    (1000)     5996 2022-04-29 20:35:07.000000 degiroasync-0.16.0/degiroasync/webapi/login.py
--rw-rw-r--   0 laumas    (1000) laumas    (1000)    12168 2022-05-12 19:37:59.000000 degiroasync-0.16.0/degiroasync/webapi/orders.py
--rw-rw-r--   0 laumas    (1000) laumas    (1000)    27804 2022-04-05 15:31:08.000000 degiroasync-0.16.0/degiroasync/webapi/product.py
-drwxrwxr-x   0 laumas    (1000) laumas    (1000)        0 2022-05-24 16:36:53.030071 degiroasync-0.16.0/degiroasync.egg-info/
--rw-rw-r--   0 laumas    (1000) laumas    (1000)     5243 2022-05-24 16:36:52.000000 degiroasync-0.16.0/degiroasync.egg-info/PKG-INFO
--rw-rw-r--   0 laumas    (1000) laumas    (1000)      716 2022-05-24 16:36:53.000000 degiroasync-0.16.0/degiroasync.egg-info/SOURCES.txt
--rw-rw-r--   0 laumas    (1000) laumas    (1000)        1 2022-05-24 16:36:52.000000 degiroasync-0.16.0/degiroasync.egg-info/dependency_links.txt
--rw-rw-r--   0 laumas    (1000) laumas    (1000)      251 2022-05-24 16:36:52.000000 degiroasync-0.16.0/degiroasync.egg-info/requires.txt
--rw-rw-r--   0 laumas    (1000) laumas    (1000)       18 2022-05-24 16:36:52.000000 degiroasync-0.16.0/degiroasync.egg-info/top_level.txt
--rw-rw-r--   0 laumas    (1000) laumas    (1000)      108 2022-02-26 15:27:30.000000 degiroasync-0.16.0/pyproject.toml
--rw-rw-r--   0 laumas    (1000) laumas    (1000)       38 2022-05-24 16:36:53.034070 degiroasync-0.16.0/setup.cfg
--rw-rw-r--   0 laumas    (1000) laumas    (1000)     2098 2022-05-12 19:06:49.000000 degiroasync-0.16.0/setup.py
-drwxrwxr-x   0 laumas    (1000) laumas    (1000)        0 2022-05-24 16:36:53.034070 degiroasync-0.16.0/tests/
--rw-rw-r--   0 laumas    (1000) laumas    (1000)        0 2022-02-13 11:54:37.000000 degiroasync-0.16.0/tests/__init__.py
--rw-rw-r--   0 laumas    (1000) laumas    (1000)     3946 2022-04-03 18:59:19.000000 degiroasync-0.16.0/tests/test_core.py
--rw-rw-r--   0 laumas    (1000) laumas    (1000)    29070 2022-05-12 19:39:59.000000 degiroasync-0.16.0/tests/test_degiroapi.py
--rw-rw-r--   0 laumas    (1000) laumas    (1000)    16375 2022-05-12 19:40:51.000000 degiroasync-0.16.0/tests/test_degirowebapi.py
--rw-rw-r--   0 laumas    (1000) laumas    (1000)      153 2022-01-27 15:50:02.000000 degiroasync-0.16.0/tests/test_setup.py
+drwxrwxr-x   0 laumas    (1000) laumas    (1000)        0 2023-07-02 20:30:08.498612 degiroasync-0.17.0/
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)     1075 2022-01-20 21:38:48.000000 degiroasync-0.17.0/LICENSE
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)     5242 2023-07-02 20:30:08.498612 degiroasync-0.17.0/PKG-INFO
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)     4550 2022-07-26 12:50:54.000000 degiroasync-0.17.0/README.md
+drwxrwxr-x   0 laumas    (1000) laumas    (1000)        0 2023-07-02 20:30:08.494612 degiroasync-0.17.0/degiroasync/
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)      692 2022-04-13 19:10:04.000000 degiroasync-0.17.0/degiroasync/__init__.py
+drwxrwxr-x   0 laumas    (1000) laumas    (1000)        0 2023-07-02 20:30:08.494612 degiroasync-0.17.0/degiroasync/api/
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)     4268 2022-04-13 18:57:09.000000 degiroasync-0.17.0/degiroasync/api/__init__.py
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)     8334 2022-05-12 19:40:07.000000 degiroasync-0.17.0/degiroasync/api/orders.py
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)    26358 2023-07-01 19:46:09.000000 degiroasync-0.17.0/degiroasync/api/product.py
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)     8975 2023-07-02 19:55:02.000000 degiroasync-0.17.0/degiroasync/api/session.py
+drwxrwxr-x   0 laumas    (1000) laumas    (1000)        0 2023-07-02 20:30:08.494612 degiroasync-0.17.0/degiroasync/core/
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)     1551 2023-03-13 17:53:33.000000 degiroasync-0.17.0/degiroasync/core/__init__.py
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)     6509 2023-07-01 20:41:23.000000 degiroasync-0.17.0/degiroasync/core/constants.py
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)    13962 2023-07-02 17:26:14.000000 degiroasync-0.17.0/degiroasync/core/core.py
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)      547 2023-03-13 16:44:13.000000 degiroasync-0.17.0/degiroasync/core/exceptions.py
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)    16478 2023-07-02 19:53:38.000000 degiroasync-0.17.0/degiroasync/core/helpers.py
+drwxrwxr-x   0 laumas    (1000) laumas    (1000)        0 2023-07-02 20:30:08.494612 degiroasync-0.17.0/degiroasync/webapi/
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)     1853 2022-04-05 15:36:45.000000 degiroasync-0.17.0/degiroasync/webapi/__init__.py
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)     5780 2023-07-02 17:18:01.000000 degiroasync-0.17.0/degiroasync/webapi/login.py
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)    12060 2023-07-02 17:18:26.000000 degiroasync-0.17.0/degiroasync/webapi/orders.py
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)    27905 2023-07-02 17:49:05.000000 degiroasync-0.17.0/degiroasync/webapi/product.py
+drwxrwxr-x   0 laumas    (1000) laumas    (1000)        0 2023-07-02 20:30:08.494612 degiroasync-0.17.0/degiroasync.egg-info/
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)     5242 2023-07-02 20:30:08.000000 degiroasync-0.17.0/degiroasync.egg-info/PKG-INFO
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)      743 2023-07-02 20:30:08.000000 degiroasync-0.17.0/degiroasync.egg-info/SOURCES.txt
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)        1 2023-07-02 20:30:08.000000 degiroasync-0.17.0/degiroasync.egg-info/dependency_links.txt
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)      251 2023-07-02 20:30:08.000000 degiroasync-0.17.0/degiroasync.egg-info/requires.txt
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)       18 2023-07-02 20:30:08.000000 degiroasync-0.17.0/degiroasync.egg-info/top_level.txt
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)      108 2022-02-26 15:27:30.000000 degiroasync-0.17.0/pyproject.toml
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)       38 2023-07-02 20:30:08.498612 degiroasync-0.17.0/setup.cfg
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)     2098 2022-07-26 12:37:58.000000 degiroasync-0.17.0/setup.py
+drwxrwxr-x   0 laumas    (1000) laumas    (1000)        0 2023-07-02 20:30:08.498612 degiroasync-0.17.0/tests/
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)        0 2023-07-02 12:58:48.000000 degiroasync-0.17.0/tests/__init__.py
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)     1504 2023-07-02 16:37:29.000000 degiroasync-0.17.0/tests/integration_login.py
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)     4825 2023-07-02 16:47:13.000000 degiroasync-0.17.0/tests/test_core.py
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)    29523 2023-07-02 18:01:35.000000 degiroasync-0.17.0/tests/test_degiroapi.py
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)    18372 2023-07-02 17:46:52.000000 degiroasync-0.17.0/tests/test_degirowebapi.py
+-rw-rw-r--   0 laumas    (1000) laumas    (1000)      153 2022-01-27 15:50:02.000000 degiroasync-0.17.0/tests/test_setup.py
```

### Comparing `degiroasync-0.16.0/LICENSE` & `degiroasync-0.17.0/LICENSE`

 * *Files identical despite different names*

### Comparing `degiroasync-0.16.0/PKG-INFO` & `degiroasync-0.17.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: degiroasync
-Version: 0.16.0
+Version: 0.17.0
 Summary: A Python asynchronous library for Degiro trading service.
 Home-page: https://github.com/OhMajesticLama/degiroasync
 Author-email: ohmajesticlama@gmail.com
 Project-URL: Documentation, https://ohmajesticlama.github.io/degiroasync/index.html
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -133,19 +133,20 @@
 # Integration tests & Unittests
 DEGIROASYNC_INTEGRATION=1 pytest --color yes
 ```
 
 ### Tests coverage
 For example, leverage `coverage` module:
 ```bash
-coverage run --include='./degiroasync/*' -m pytest
-# To exclude webapi module
-#coverage run --include='./degiroasync/*' --omit='./degiroasync/webapi/*' -m pytest
+pytest --cov
 ```
 
+Please note that the coverage will or will not include integration tests if
+`DEGIROASYNC_INTEGRATION` environment variable is set to 1 or not set.
+
 
 ## Other Python Degiro Libraries
 
 Check-out those other Python Degiro libraries - non-exhaustive list - to assess
 which best fits your needs:
 - https://github.com/Chavithra/degiro-connector
 - https://github.com/lolokraus/DegiroAPI
```

### Comparing `degiroasync-0.16.0/README.md` & `degiroasync-0.17.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -116,19 +116,20 @@
 # Integration tests & Unittests
 DEGIROASYNC_INTEGRATION=1 pytest --color yes
 ```
 
 ### Tests coverage
 For example, leverage `coverage` module:
 ```bash
-coverage run --include='./degiroasync/*' -m pytest
-# To exclude webapi module
-#coverage run --include='./degiroasync/*' --omit='./degiroasync/webapi/*' -m pytest
+pytest --cov
 ```
 
+Please note that the coverage will or will not include integration tests if
+`DEGIROASYNC_INTEGRATION` environment variable is set to 1 or not set.
+
 
 ## Other Python Degiro Libraries
 
 Check-out those other Python Degiro libraries - non-exhaustive list - to assess
 which best fits your needs:
 - https://github.com/Chavithra/degiro-connector
 - https://github.com/lolokraus/DegiroAPI
```

### Comparing `degiroasync-0.16.0/degiroasync/__init__.py` & `degiroasync-0.17.0/degiroasync/__init__.py`

 * *Files identical despite different names*

### Comparing `degiroasync-0.16.0/degiroasync/api/__init__.py` & `degiroasync-0.17.0/degiroasync/api/__init__.py`

 * *Files identical despite different names*

### Comparing `degiroasync-0.16.0/degiroasync/api/orders.py` & `degiroasync-0.17.0/degiroasync/api/orders.py`

 * *Files identical despite different names*

### Comparing `degiroasync-0.16.0/degiroasync/api/product.py` & `degiroasync-0.17.0/degiroasync/api/product.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,14 +81,18 @@
         force_init
             If this is set to True, allow init of product. Use only if you know
             what you're doing.
         """
         if not force_init:
             raise NotImplementedError("Please use ProductFactory.init_batch.")
 
+    def __repr__(self):
+        return (f'<degiroasync.api.product.{self.__class__.__name__} '
+                f'[self.info.name | self.info.symbol]>')
+
 
 class ProductFactory:
     @classmethod
     async def init_batch(
             cls,
             session: SessionCore,
             attributes_iter: Iterable[Dict[str, Any]],
@@ -204,15 +208,15 @@
 
         products_info
             This dictionary keys and values will be assigned to the `info`
             attribute of the instantiated product.
         """
         LOGGER.debug("__products_from_attrs| products_info %s",
                      products_info)
-        products_dict = {}
+        products_dict: Dict[str, ProductBase] = {}
 
         # Instantiate products
         for product_base in products_base_iter:
             LOGGER.debug("__products_from_attrs| product_base %s",
                          product_base)
             product_id = product_base['id']
             if product_id in products_dict:
```

### Comparing `degiroasync-0.16.0/degiroasync/core/__init__.py` & `degiroasync-0.17.0/degiroasync/core/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -26,17 +26,21 @@
 from .core import check_session_client
 from .core import check_session_config
 from .core import Credentials
 from .core import Config
 from .core import SessionCore
 from .core import URLs
 from .core import PAClient
-from .constants import ResponseError
+from .exceptions import ResponseError
+from .exceptions import BadCredentialsError
+from .exceptions import ContextError
 
-__all__ = [obj.__name__ for obj in (
+
+# Fail at module import if an attribute is missing __name__: ignore mypy here.
+__all__ = [obj.__name__ for obj in (  # type: ignore
     join_url,
     lru_cache_timed,
     camelcase_to_snake,
     camelcase_dict_to_snake,
     set_params,
     PRODUCT,
     ORDER,
@@ -44,13 +48,15 @@
     POSITION,
     PRICE,
     Credentials,
     Config,
     check_session_client,
     check_session_config,
     ResponseError,
+    BadCredentialsError,
+    ContextError,
     SessionCore,
     PAClient,
     URLs,
     )] + [
         LOGGER_NAME
     ]
```

### Comparing `degiroasync-0.16.0/degiroasync/core/constants.py` & `degiroasync-0.17.0/degiroasync/core/constants.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,18 +12,14 @@
             return str.__str__(self)
 
 
 # Used to get same Logger instance across submodules.
 LOGGER_NAME = 'degiroasync'
 
 
-class ResponseError(Exception):
-    "Raised when bad response has been received from server."
-
-
 class _EnumBase(enum.Enum):
     """
     Base class for Enums that should behave as str or other types.
 
     >>> class StrEnum(str, _EnumBase):
     ...     pass
     ...
@@ -97,14 +93,15 @@
     At this date, only one has been noticed and documented.
 
     TOTP_NEEDED
         This flag is set when one-time-password is required to log in the
         account.
     """
     TOTP_NEEDED = 6
+    BAD_CREDENTIALS = 3
 
 
 class ORDER:
     """
     Constants for orders in web API.
     """
     class ACTION(StrEnum):
```

### Comparing `degiroasync-0.16.0/degiroasync/core/core.py` & `degiroasync-0.17.0/degiroasync/core/core.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,29 +1,34 @@
 from __future__ import annotations
 import logging
 import dataclasses
 try:
-    from enum import StrEnum
+    # Ignore type here: will fail w/ Python version <3.11
+    from enum import StrEnum  # type: ignore
 except ImportError:
     import enum
     # Exists only starting Python 3.11
     # Reimplement what we need from it here.
 
-    class StrEnum(str, enum.Enum):
+    # Type warning 'already defined', this statement is executed if prior
+    # import failed: no risk of redefinition.
+    class StrEnum(str, enum.Enum):  # type: ignore
         def __str__(self):
             return str.__str__(self)
 
-from typing import Union, Optional
+from typing import Union, Optional, Any
 
 import httpx
 from jsonloader import JSONclass
 
 from .helpers import join_url
 from .constants import LOGGER_NAME
 from .constants import PRODUCT
+from ..core.helpers import ThrottlingClient
+from .exceptions import ContextError
 
 LOGGER = logging.getLogger(LOGGER_NAME)
 LOGGER.setLevel(logging.DEBUG)
 
 
 @dataclasses.dataclass
 class Credentials:
@@ -41,54 +46,67 @@
     """
     username: str
     password: str
 
     totp_secret: Union[str, None] = None
     one_time_password: Union[str, None] = None
 
+    def __hash__(self) -> int:
+        return hash(
+            '|'.join(
+                ':'.join((str(k), str(v)))
+                for k, v in self.__dict__.items())
+                )
+
+    def __eq__(self, other: Any) -> bool:
+        if not isinstance(other, Credentials):
+            raise AttributeError(
+                    "other is not `Credentials` instance.")
+        return hash(self) == hash(other)
+
 
 @JSONclass(annotations=True, annotations_type=True)
 class Config:
     """
     SessionCore config, as returned by endpoint.
     """
     client_id: int
     companies_service_url: Union[str, None]
     dictionary_url: str
-    i18n_url: Union[str, None]
-    landing_path: Union[str, None]
-    latest_searched_products_url: Union[str, None]
+    i18n_url: Optional[str]
+    landing_path: Optional[str]
+    latest_searched_products_url: Optional[str]
     login_url: str
-    mobile_landing_path: Union[str, None]
+    mobile_landing_path: Optional[str]
     pa_url: str
-    payment_service_url: Union[str, None]
-    product_notes_url: Union[str, None]
+    payment_service_url: Optional[str]
+    product_notes_url: Optional[str]
     product_search_url: str
     product_types_url: str
-    refinitiv_agenda_url: Union[str, None]
-    refinitiv_clips_url: Union[str, None]
-    refinitiv_company_profile_url: Union[str, None]
-    refinitiv_company_ratios_url: Union[str, None]
-    refinitiv_esgs_url: Union[str, None]
-    refinitiv_estimates_url: Union[str, None]
-    refinitiv_financial_statements_url: Union[str, None]
-    refinitiv_insider_transactions_url: Union[str, None]
-    refinitiv_insiders_report_url: Union[str, None]
-    refinitiv_investor_url: Union[str, None]
-    refinitiv_news_url: Union[str, None]
-    refinitiv_shareholders_url: Union[str, None]
-    refinitiv_top_news_categories_url: Union[str, None]
-    reporting_url: Union[str, None]
-    session_id: Union[str, None]
-    task_manager_url: Union[str, None]
-    trading_url: Union[str, None]
-    translations_url: Union[str, None]
-    vwd_gossips_url: Union[str, None]
-    vwd_news_url: Union[str, None]
-    vwd_quotecast_service_url: Union[str, None]
+    refinitiv_agenda_url: Optional[str]
+    refinitiv_clips_url: Optional[str]
+    refinitiv_company_profile_url: Optional[str]
+    refinitiv_company_ratios_url: Optional[str]
+    refinitiv_esgs_url: Optional[str]
+    refinitiv_estimates_url: Optional[str]
+    refinitiv_financial_statements_url: Optional[str]
+    refinitiv_insider_transactions_url: Optional[str]
+    refinitiv_insiders_report_url: Optional[str]
+    refinitiv_investor_url: Optional[str]
+    refinitiv_news_url: Optional[str]
+    refinitiv_shareholders_url: Optional[str]
+    refinitiv_top_news_categories_url: Optional[str]
+    reporting_url: Optional[str]
+    session_id: Optional[str]
+    task_manager_url: Optional[str]
+    trading_url: Optional[str]
+    translations_url: Optional[str]
+    vwd_gossips_url: Optional[str]
+    vwd_news_url: Optional[str]
+    vwd_quotecast_service_url: Optional[str]
 
 
 @JSONclass(annotations=True, annotations_type=True)
 class PAClient:
     """
     Data Structure for PA Client
     """
@@ -132,88 +150,130 @@
     #    iban = Union[str, None]
     # }
     id: Union[str, None]
     int_account: Union[int, None]
     is_allocation_available: Union[bool, None]
     is_am_client_active: Union[bool, None]
 
-    # def set_data(self, data: dict):
-    #    check_keys(data, ('intAccount', 'id'))
-    #    setattrs(self, **data)
-    #    return self
-
 
 @dataclasses.dataclass
 class SessionCore:
     JSESSIONID = 'JSESSIONID'
 
     config: Optional[Config] = None
     client: Optional[PAClient] = None
 
+    _max_requests_default: int = 30
+    _period_seconds_default: int = 1
+
     # Cookies
     # Wrap to not leak httpx
-    _cookies: Union[httpx.Cookies, None] = None
+    _cookies: Optional[httpx.Cookies] = None
+    _http_client: Optional[ThrottlingClient] = None
 
     @property
     def cookies(self):
         return dict(self._cookies)
 
+    def update_throttling(
+            self,
+            max_requests: int = 20,
+            period_seconds: float = 1
+            ):
+        "Update throttling parameters. No limit if max_requests <= 0."
+        if self._http_client is None:
+            self._max_requests_default = max_requests
+            self._period_seconds_default = period_seconds
+        else:
+            self._http_client._max_requests = max_requests
+            self._http_client._period_s = period_seconds
+
     @cookies.setter
     def cookies(self, cookies: dict):
         self._cookies = httpx.Cookies(cookies)
 
     def __hash__(self):
         return hash(self.__dict__.values())
 
+    async def __aenter__(self) -> ThrottlingClient:
+        if self._http_client is None:
+            self._http_client = ThrottlingClient(
+                    max_requests=self._max_requests_default,
+                    period_seconds=self._period_seconds_default
+                    )
+        return await self._http_client.__aenter__()
+
+    async def __aexit__(self, exc_type, exc_val, exc_tb):
+        await self._http_client.__aexit__(exc_type, exc_val, exc_tb)
+
 
 class URLs:
     BASE = 'https://trader.degiro.nl'
     LOGIN = join_url(BASE, '/login/secure/login')
     LOGIN_TOTP = join_url(BASE, '/login/secure/login/totp')
     CONFIG = join_url(BASE, '/login/secure/config')
     ACCOUNT_INFO = join_url(BASE, '/trading/secure/v5/account/info')
 
     @staticmethod
     def get_news_by_company_url(session: SessionCore) -> str:
         "Build news_by_company url"
-        check_session_config(session)
-        return join_url(session.config.refinitiv_news_url, 'news-by-company')
+        config = check_session_config(session)
+        if config.refinitiv_news_url is None:
+            raise ContextError(
+                    "Session attribute 'refinitiv_news_url' is not set."
+                    )
+        return join_url(config.refinitiv_news_url, 'news-by-company')
 
     @staticmethod
     def get_client_info_url(session: SessionCore) -> str:
         """
         Build client info url.
         """
-        check_session_config(session)
-        return join_url(session.config.pa_url, 'client')
+        config = check_session_config(session)
+        if config.pa_url is None:
+            raise ContextError(
+                    "Session attribute 'pa_url' is not set."
+                    )
+        return join_url(config.pa_url, 'client')
 
     @staticmethod
     def get_portfolio_url(session: SessionCore) -> str:
         """
         Build portfolio url, also used for orders.
         """
-        check_session_config(session)
-        check_session_client(session)
+        config = check_session_config(session)
+        client = check_session_client(session)
+
+        if session._cookies is None:
+            raise ContextError("_cookies not set in session.")
 
         jsessionid = session._cookies[session.JSESSIONID]
 
+        if config.trading_url is None:
+            raise ContextError(
+                    "Session attribute 'trading_url' is not set."
+                    )
         url = join_url(
-            session.config.trading_url,
-            f'v5/update/{session.client.int_account}',
+            config.trading_url,
+            f'v5/update/{client.int_account}',
             f';jsessionid={jsessionid}')
         LOGGER.debug('get_portfolio_url| %s', url)
         return url
 
     @staticmethod
     def get_reporting_url(session: SessionCore) -> str:
         """
         Get reporting URL. Used for orders history and transactions.
         """
-        check_session_config(session)
-        url = session.config.reporting_url
+        config = check_session_config(session)
+        url = config.reporting_url
+        if url is None:
+            raise ContextError(
+                    "Session attribute 'reporting_url' is not set."
+                    )
         LOGGER.debug('get_reporting_url| %s', url)
         return url
 
     @classmethod
     def get_orders_history_url(cls, session: SessionCore) -> str:
         """
         Get reporting URL. Used for orders history.
@@ -242,18 +302,18 @@
         .. code-block:: python
 
             confirmation_id = '98741234kjaskdjfz098234'
             confirm_order_url_base = URLs.get_confirm_order_url(session)
             join_url(confirm_order_url_base, confirmation_id)
 
         """
-        check_session_config(session)
+        config = check_session_config(session)
 
         return join_url(
-            session.config.trading_url,
+            config.trading_url,
             'v5/order'
         )
 
     @classmethod
     def get_orders_url(cls, session: SessionCore) -> str:
         """
         Build Get Orders url
@@ -262,20 +322,20 @@
         return cls.get_portfolio_url(session)
 
     @classmethod
     def get_check_order_url(cls, session: SessionCore) -> str:
         """
         Get check order URL.
         """
-        check_session_config(session)
+        config = check_session_config(session)
 
-        jsessionid = session._cookies[session.JSESSIONID]
+        jsessionid = check_session_cookies(session)[session.JSESSIONID]
 
         url = join_url(
-            session.config.trading_url,
+            config.trading_url,
             f'v5/checkOrder;jsessionid={jsessionid}'
         )
         LOGGER.debug('get_check_order_url| %s', url)
         return url
 
     @staticmethod
     def get_price_data_url(session: SessionCore) -> str:
@@ -293,64 +353,81 @@
         FUNDS = 'funds'
         LEVERAGED_PRODUCTS = 'leverageds'
         WARRANTS = 'warrants'
 
     @staticmethod
     def get_product_search_url(
             session: SessionCore,
-            product_type_id: Union[PRODUCT.TYPEID, None] = None) -> str:
-        specialization = {
+            product_type_id: Optional[PRODUCT.TYPEID] = None) -> str:
+        specialization: Union[str, URLs.PRODUCT_SEARCH_TYPE] = {
             PRODUCT.TYPEID.STOCK:
                 URLs.PRODUCT_SEARCH_TYPE.STOCKS,
             PRODUCT.TYPEID.ETFS:
                 URLs.PRODUCT_SEARCH_TYPE.ETFS,
             PRODUCT.TYPEID.OPTIONS:
                 URLs.PRODUCT_SEARCH_TYPE.OPTIONS,
             PRODUCT.TYPEID.BONDS:
                 URLs.PRODUCT_SEARCH_TYPE.BONDS,
             PRODUCT.TYPEID.FUNDS:
                 URLs.PRODUCT_SEARCH_TYPE.FUNDS,
             PRODUCT.TYPEID.LEVERAGE_PRODUCTS:
                 URLs.PRODUCT_SEARCH_TYPE.LEVERAGED_PRODUCTS,
             PRODUCT.TYPEID.WARRANTS:
                 URLs.PRODUCT_SEARCH_TYPE.WARRANTS,
-        }.get(product_type_id, URLs.PRODUCT_SEARCH_TYPE.GENERIC)
-        check_session_config(session)
+            # mypy doesn't handle well the error management in dict.get:
+            # here we rely on dict.get to provide default value if
+            # product_type_id is not found or None.
+        }.get(
+            product_type_id,  # type: ignore
+            URLs.PRODUCT_SEARCH_TYPE.GENERIC
+        )
+        config = check_session_config(session)
         url = join_url(
-            session.config.product_search_url,
+            config.product_search_url,
             'v5',
             specialization)
         LOGGER.debug('get_product_search_url: %s', url)
         return url
 
     @staticmethod
     def get_product_dictionary_url(session: SessionCore) -> str:
-        check_session_config(session)
-        url = session.config.dictionary_url
+        config = check_session_config(session)
+        url = config.dictionary_url
         LOGGER.debug('get_product_search_url: %s', url)
         return url
 
     @classmethod
     def get_account_info_url(cls, session: SessionCore) -> str:
-        check_session_client(session)
-        url = join_url(URLs.ACCOUNT_INFO, str(session.client.int_account))
+        client = check_session_client(session)
+        url = join_url(URLs.ACCOUNT_INFO, str(client.int_account))
         return cls._add_jsessionid(session, url)
 
     @classmethod
     def _add_jsessionid(cls, session: SessionCore, url: str) -> str:
         check_session_config(session)
+        cookies = check_session_cookies(session)
         return url + ';jsessionid={}'.format(
-            session._cookies[session.JSESSIONID])
+            cookies[session.JSESSIONID])
 
 
-def check_session_config(session: SessionCore):
+def check_session_config(session: SessionCore) -> Config:
     "Raise an exception if session.config is not set"
     if session.config is None:
         raise AssertionError(
             "session.config is not set. Call get_config first.")
+    return session.config
 
 
-def check_session_client(session: SessionCore):
+def check_session_client(session: SessionCore) -> PAClient:
     "Raise an exception if session.client is not set"
-    if session.config is None:
+    if session.client is None:
         raise AssertionError(
             "session.client is not set. Call get_client_info first.")
+    return session.client
+
+
+def check_session_cookies(session: SessionCore) -> httpx.Cookies:
+    "Helper to get cookies from a session."
+    if session._cookies is not None:
+        return session._cookies
+    else:
+        raise ContextError("Cookies not set in session. Abort.")
```

### Comparing `degiroasync-0.16.0/degiroasync/webapi/__init__.py` & `degiroasync-0.17.0/degiroasync/webapi/__init__.py`

 * *Files identical despite different names*

### Comparing `degiroasync-0.16.0/degiroasync/webapi/login.py` & `degiroasync-0.17.0/degiroasync/webapi/login.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,16 +11,14 @@
 
 from ..core.constants import LOGGER_NAME
 from ..core.constants import LOGIN
 from ..core.constants import TIMEOUT
 from ..core import Credentials, SessionCore, URLs, Config, PAClient
 from ..core import check_session_config
 from ..core.helpers import check_response
-from ..core.helpers import join_url
-from ..core.helpers import camelcase_to_snake
 from ..core.helpers import camelcase_dict_to_snake
 
 LOGGER = logging.getLogger(LOGGER_NAME)
 
 
 async def login(
         credentials: Credentials,
@@ -35,15 +33,15 @@
     payload = {
         "username": credentials.username,
         "password": credentials.password,
         "isRedirectToMobile": False,
         "isPassCodeReset": '',
         "queryParams": {"reason": "session_expired"}
     }
-    async with httpx.AsyncClient(timeout=TIMEOUT) as client:
+    async with session as client:
         LOGGER.debug("login| url %s", url)
         response = await client.post(url, content=json.dumps(payload))
         LOGGER.debug("login| response %s", response.__dict__)
 
         response_load = response.json()
 
         if response_load['status'] == LOGIN.TOTP_NEEDED:
@@ -81,15 +79,15 @@
 
 
 async def get_config(session: SessionCore) -> SessionCore:
     """
     Populate session with configuration
     """
     _check_active_session(session)
-    async with httpx.AsyncClient(timeout=TIMEOUT) as client:
+    async with session as client:
         res = await client.get(URLs.CONFIG, cookies=session._cookies)
 
     check_response(res)
     config = Config(camelcase_dict_to_snake(res.json()['data']))
 
     session.config = config
 
@@ -97,15 +95,16 @@
 
 
 async def get_client_info(session: SessionCore) -> SessionCore:
     """
     Get client information.
     """
     url = URLs.get_client_info_url(session)
-    async with httpx.AsyncClient(timeout=TIMEOUT) as client:
+
+    async with session as client:
         res = await client.get(
             url,
             params={'sessionId': session._cookies[session.JSESSIONID]},
             cookies=session._cookies)
 
     check_response(res)
     resp_data = res.json()['data']
@@ -117,15 +116,15 @@
 
 async def get_account_info(session: SessionCore) -> SessionCore:
     """
 
     """
     _check_active_session(session)
     url = URLs.get_account_info_url(session)
-    async with httpx.AsyncClient(timeout=TIMEOUT) as client:
+    async with session as client:
         res = await client.get(url,
                                cookies=session._cookies
                                )
     check_response(res)
     res_json = res.json()
     LOGGER.debug("get_account_info| res_json %s", res_json)
     return res_json
@@ -143,15 +142,15 @@
     """
     check_session_config(session)
     url = URLs.get_product_dictionary_url(session)
     params = dict(
         intAccount=session.client.int_account,
         sessionId=session.config.session_id
     )
-    async with httpx.AsyncClient(timeout=TIMEOUT) as client:
+    async with session as client:
         response = await client.get(url,
                                     cookies=session._cookies,
                                     params=params
                                     )
     check_response(response)
     LOGGER.debug("webapi.get_product_dictionary response| %s", response.json())
     return response.json()
```

### Comparing `degiroasync-0.16.0/degiroasync/webapi/orders.py` & `degiroasync-0.17.0/degiroasync/webapi/orders.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,15 +99,15 @@
         buySell=buy_sell,
         orderType=order_type,
         price=price,
         productId=product_id,
         timeType=time_type
     )
 
-    async with httpx.AsyncClient(timeout=TIMEOUT) as client:
+    async with session as client:
         response = await client.post(
             url,
             params=params,
             json=data,
         )
     check_response(response)
     resp_json = response.json()
@@ -223,15 +223,15 @@
         orderType=order_type,
         price=price,
         productId=product_id,
         size=size,
         timeType=time_type
     )
     LOGGER.debug("check_order data| %s", data)
-    async with httpx.AsyncClient(timeout=TIMEOUT) as client:
+    async with session as client:
         response = await client.post(
             url,
             params=params,
             json=data,
             headers={
                 'content-type': 'application/json;charset=UTF-8'
             },
@@ -349,15 +349,15 @@
     params = dict(
         fromDate=from_date,
         toDate=to_date,
         intAccount=session.client.int_account,
         sessionId=jsessionid
     )
 
-    async with httpx.AsyncClient(timeout=TIMEOUT) as client:
+    async with session as client:
         response = await client.get(
             url,
             params=params,
             headers={
                 'content-type': 'application/json'
             },
             cookies=session._cookies
@@ -423,15 +423,15 @@
         toDate=to_date,
         intAccount=session.client.int_account,
         sessionId=jsessionid,
         groupTransactionsByOrder=False
     )
 
     LOGGER.debug('get_transactions params| %s', params)
-    async with httpx.AsyncClient(timeout=TIMEOUT) as client:
+    async with session as client:
         response = await client.get(
             url,
             params=params,
             headers={
                 'content-type': 'application/json'
             },
             cookies=session._cookies
```

### Comparing `degiroasync-0.16.0/degiroasync/webapi/product.py` & `degiroasync-0.17.0/degiroasync/webapi/product.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from typing import Union, Any, List, Dict
 
 import httpx
 
 from ..core import SessionCore, URLs
 from ..core import join_url
 from ..core import check_session_config
+from ..core import check_session_client
 from ..core.constants import LOGGER_NAME
 from ..core.constants import PRICE
 from ..core.constants import PRODUCT
 from ..core.constants import TIMEOUT
 from ..core.helpers import check_response
 
 
@@ -538,28 +539,30 @@
 
 async def get_products_info(
         session: SessionCore,
         products_ids: List[str]) -> Dict[str, Any]:
     """
     Get Product info Web API call.
     """
-    if session.config.product_search_url is None:
+    config = check_session_config(session)
+    client = check_session_client(session)
+    if config.product_search_url is None:
         raise AssertionError("productSearchUrl is None:"
                              " have you called get_config?")
 
     LOGGER.debug('get_products_info products_ids| %s', products_ids)
-    url = join_url(session.config.product_search_url,
+    url = join_url(config.product_search_url,
                    'v5/products/info')
-    async with httpx.AsyncClient(timeout=TIMEOUT) as client:
-        response = await client.post(
+    async with session as httpxclient:
+        response = await httpxclient.post(
             url,
             cookies=session.cookies,
             params={
-                'intAccount': session.client.int_account,
-                'sessionId': session.config.session_id
+                'intAccount': client.int_account,
+                'sessionId': config.session_id
             },
             json=products_ids
         )
         try:
             check_response(response)
         except Exception:
             LOGGER.error('get_products_info response| %s', response)
@@ -576,24 +579,27 @@
         session: SessionCore,
         isin: str) -> Dict[str, Any]:
     """
     Get company profile.
     """
     # should this url be taken from config as well?
 
+    client = check_session_client(session)
+    config = check_session_config(session)
+
     # Look for dgtbxdsservice in network logs for financial statements etc.
     # might have intraday data as well
     url = join_url(URLs.BASE, 'dgtbxdsservice/company-profile/v2', isin)
-    async with httpx.AsyncClient(timeout=TIMEOUT) as client:
-        response = await client.get(
+    async with session as httpclient:
+        response = await httpclient.get(
             url,
             cookies=session.cookies,
             params={
-                'intAccount': session.client.int_account,
-                'sessionId': session.config.session_id
+                'intAccount': client.int_account,
+                'sessionId': config.session_id
             })
     check_response(response)
     LOGGER.debug(response.json())
     return response.json()
 
 
 async def get_news_by_company(
@@ -602,26 +608,28 @@
         limit: int = 10,
         languages: List[str] = ['en'],
         offset: int = 0
 ) -> Dict[str, Any]:
     """
     Get news for a company.
     """
+    client = check_session_client(session)
+    config = check_session_config(session)
     url = URLs.get_news_by_company_url(session)
-    async with httpx.AsyncClient(timeout=TIMEOUT) as client:
-        response = await client.get(
+    async with session as httpxclient:
+        response = await httpxclient.get(
             url,
             cookies=session.cookies,
             params={
                 'isin': isin,
                 'limit': limit,
                 'languages': languages,
                 'offset': offset,
-                'intAccount': session.client.int_account,
-                'sessionId': session.config.session_id
+                'intAccount': client.int_account,
+                'sessionId': config.session_id
             })
     check_response(response)
     resp_json = response.json()
     LOGGER.debug("get_news_by_company| %s", resp_json)
     return resp_json
 
 
@@ -739,15 +747,15 @@
         'culture': culture,
         'period': period,
         'series': f'price:{vwdIdentifierType}:{vwdId}',
         'format': 'json',
         'userToken': session.config.client_id
     }
     LOGGER.debug('get_price_data params| %s', params)
-    async with httpx.AsyncClient(timeout=TIMEOUT) as client:
+    async with session as client:
         response = await client.get(url,
                                     cookies=session.cookies,
                                     params=params)
     check_response(response)
     resp_json = response.json()
     LOGGER.debug('get_price_data response| %s', resp_json)
     return resp_json
@@ -771,15 +779,15 @@
         Current orders.
     - 'historicalOrders': 0
         Closed orders.
     - 'transactions': 0
         Executed transactions.
     """
     url = URLs.get_portfolio_url(session)
-    async with httpx.AsyncClient(timeout=TIMEOUT) as client:
+    async with session as client:
         response = await client.get(url,
                                     cookies=session._cookies,
                                     params=params)
 
     check_response(response)
     LOGGER.debug("get_trading_update| %s", response.json())
     return response.json()
@@ -862,15 +870,15 @@
         searchText=search_txt,
         intAccount=session.client.int_account,
         sessionId=session.config.session_id
     )
     if product_type_id is not None:
         params['productTypeId'] = product_type_id
     LOGGER.debug("webapi.search_product params| %s", params)
-    async with httpx.AsyncClient(timeout=TIMEOUT) as client:
+    async with session as client:
         response = await client.get(url,
                                     cookies=session._cookies,
                                     params=params)
     check_response(response)
     LOGGER.debug("webapi.search_product response| %s", response.json())
     return response.json()
```

### Comparing `degiroasync-0.16.0/degiroasync.egg-info/PKG-INFO` & `degiroasync-0.17.0/degiroasync.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: degiroasync
-Version: 0.16.0
+Version: 0.17.0
 Summary: A Python asynchronous library for Degiro trading service.
 Home-page: https://github.com/OhMajesticLama/degiroasync
 Author-email: ohmajesticlama@gmail.com
 Project-URL: Documentation, https://ohmajesticlama.github.io/degiroasync/index.html
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -133,19 +133,20 @@
 # Integration tests & Unittests
 DEGIROASYNC_INTEGRATION=1 pytest --color yes
 ```
 
 ### Tests coverage
 For example, leverage `coverage` module:
 ```bash
-coverage run --include='./degiroasync/*' -m pytest
-# To exclude webapi module
-#coverage run --include='./degiroasync/*' --omit='./degiroasync/webapi/*' -m pytest
+pytest --cov
 ```
 
+Please note that the coverage will or will not include integration tests if
+`DEGIROASYNC_INTEGRATION` environment variable is set to 1 or not set.
+
 
 ## Other Python Degiro Libraries
 
 Check-out those other Python Degiro libraries - non-exhaustive list - to assess
 which best fits your needs:
 - https://github.com/Chavithra/degiro-connector
 - https://github.com/lolokraus/DegiroAPI
```

### Comparing `degiroasync-0.16.0/degiroasync.egg-info/SOURCES.txt` & `degiroasync-0.17.0/degiroasync.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -18,11 +18,12 @@
 degiroasync/core/exceptions.py
 degiroasync/core/helpers.py
 degiroasync/webapi/__init__.py
 degiroasync/webapi/login.py
 degiroasync/webapi/orders.py
 degiroasync/webapi/product.py
 tests/__init__.py
+tests/integration_login.py
 tests/test_core.py
 tests/test_degiroapi.py
 tests/test_degirowebapi.py
 tests/test_setup.py
```

### Comparing `degiroasync-0.16.0/setup.py` & `degiroasync-0.17.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     description = "A Python asynchronous library for Degiro trading service."
     readme_path = os.path.join(os.path.dirname(__file__), 'README.md')
     with open(readme_path, "r") as fh:
         long_description = fh.read()
 
     setuptools.setup(
         name="degiroasync",
-        version="0.16.0",
+        version="0.17.0",
         author_email="ohmajesticlama@gmail.com",
         description=description,
         long_description=long_description,
         long_description_content_type='text/markdown',
         url="https://github.com/OhMajesticLama/degiroasync",
         project_urls={
             'Documentation':
```

### Comparing `degiroasync-0.16.0/tests/test_degiroapi.py` & `degiroasync-0.17.0/tests/test_degiroapi.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,51 +1,41 @@
 import unittest
 import itertools
 import logging
 import os
 import pprint
-import asyncio
 import unittest.mock
 import sys
 import datetime
 from unittest.mock import MagicMock
+from typing import Sequence
 
 
 import degiroasync
 import degiroasync.webapi
 import degiroasync.api
+import degiroasync.webapi
 import degiroasync.core
 import degiroasync.core.helpers
-from degiroasync.core import join_url
-from degiroasync.core import SessionCore
-from degiroasync.core.helpers import set_params
-from degiroasync.core.helpers import camelcase_to_snake
-from degiroasync.core.helpers import camelcase_dict_to_snake
-from degiroasync.webapi import get_config
-from degiroasync.webapi import get_client_info
-from degiroasync.webapi import get_products_info
-from degiroasync.webapi import get_company_profile
-from degiroasync.webapi import get_news_by_company
+from degiroasync.core import Credentials
 from degiroasync.api.product import convert_time_series
-from degiroasync.api import ProductBase
 from degiroasync.api import ProductFactory
-from degiroasync.api import Stock
-from degiroasync.api import Currency
 from degiroasync.api import Order
 from degiroasync.api import ORDER
 from degiroasync.api import Exchange
 from degiroasync.core.constants import PRODUCT
 from degiroasync.core.constants import PRICE
+from degiroasync.core import BadCredentialsError
 
-from .test_degirowebapi import _get_credentials
+from tests.integration_login import _get_credentials
+from tests.integration_login import _IntegrationLogin
 
 
 LOGGER = logging.getLogger(degiroasync.core.LOGGER_NAME)
 LOGGER.setLevel(logging.DEBUG)
-#degiroasync.core.helpers.set_logs(LOGGER, logging.DEBUG)
 
 LOGGER.debug('Python Version: %s', sys.version)
 
 RUN_INTEGRATION_TESTS = 0
 try:
     _env_var = os.environ.get('DEGIROASYNC_INTEGRATION')
     RUN_INTEGRATION_TESTS = int(_env_var)
@@ -54,14 +44,55 @@
 del _env_var
 
 
 #############
 # Unittests #
 #############
 
+class TestDegiroAsyncLogin(unittest.IsolatedAsyncioTestCase):
+    @unittest.mock.patch('degiroasync.webapi.get_client_info')
+    @unittest.mock.patch('degiroasync.webapi.get_config')
+    @unittest.mock.patch('degiroasync.webapi.login')
+    async def test_bad_credentials(
+            self,
+            login_m: MagicMock,
+            get_config_m: MagicMock,
+            *stubs: Sequence[MagicMock]
+            ):
+        """
+        Verify that BadCredentialsError is raised in case of bad credentials
+        and that default behavior does not try to log in again with previously
+        failed credentials.
+        """
+        login_m.side_effect = BadCredentialsError()
+        # This should never be called as we're supposed to raise an exception
+        # before. Raise exception in case we make it to get_config.
+        get_config_m.side_effect = RuntimeError("This should not happen.")
+
+        credentials = Credentials(
+            username='dummyaccount123456',
+            password='dummydummy'
+                )
+        with self.assertRaises(BadCredentialsError):
+            await degiroasync.api.login(credentials)
+        # There should be exactly one call made to webapi.login
+        login_m.assert_called_once()
+
+        # Attempt a second login with same credentials.
+        credentials = Credentials(
+            username='dummyaccount123456',
+            password='dummydummy'
+                )
+        # BadCredentialsError should still be raised.
+        with self.assertRaises(BadCredentialsError):
+            await degiroasync.api.login(credentials)
+
+        # There should be no new call to webapi.login.
+        login_m.assert_called_once()
+
 
 class TestDegiroAsyncOrders(unittest.IsolatedAsyncioTestCase):
     def setUp(self):
         self.get_orders_mock = MagicMock()
         self._orders_dummy = {
                 'orders': [
                         {
@@ -162,16 +193,14 @@
                 })
 
 
 class TestExchangeDictionary(unittest.IsolatedAsyncioTestCase):
     "Unittest for api.ExchangeDictionary"
     def setUp(self):
         resp_mock = unittest.mock.MagicMock()
-        #resp_mock.json = unittest.mock.MagicMock()
-        #resp_mock.return_value = {
         self._product_dictionary_dummy = {
                 "regions": [
                     {
                         "id": 1,
                         "name": "Europe",
                         "translation": "translation.label.117"
                     },
@@ -293,14 +322,15 @@
                     },
                 ))
         products = [p async for p in products_gen]
         self.assertEqual(len(products), 1)
         self.assertEqual(products[0].base.id, '123')
         self.assertEqual(products[0].info.name, 'foo')
         self.assertEqual(products[0].info.symbol, 'FOO')
+        self.assertIsInstance(repr(products[0]), str)  # don't raise exception
 
     @unittest.mock.patch('degiroasync.webapi.get_products_info')
     async def test_product_no_batch(self, wapi_prodinfo_m):
         # Same as test_product but with size=1 to test corner case.
         # Mock get_products_info
         #resp = MagicMock()
         #resp.json = MagicMock(return_value={'data': {
@@ -349,53 +379,38 @@
 
 #####################
 # Integration tests #
 #####################
 if RUN_INTEGRATION_TESTS:
     LOGGER.info('degiroasync.api integration tests will run.')
 
-    class _IntegrationLogin:
-        """
-        Internal helper, can be inherited to make login for integration tests
-        easier.
-        """
-        async def asyncSetUp(self):
-            self._lock = asyncio.Lock()
-
-        async def _login(self):
-            async with self._lock:
-                if not hasattr(self, 'session'):
-                    credentials = _get_credentials()
-                    self.session = await degiroasync.api.login(credentials)
-            return self.session
-
     class TestDegiroasyncIntegrationLogin(
             _IntegrationLogin,
             unittest.IsolatedAsyncioTestCase):
         async def test_login(self):
             credentials = _get_credentials()
             session = await degiroasync.api.login(credentials)
             self.assertIsNotNone(session.config)
             self.assertIsNotNone(session.client)
 
     class TestDegiroasyncIntegrationPortfolio(
             _IntegrationLogin,
             unittest.IsolatedAsyncioTestCase):
         async def test_get_portfolio_total(self):
-            session = await self._login()
+            session = await _IntegrationLogin._login()
             total = await degiroasync.api.get_portfolio_total(session)
             LOGGER.debug("test_get_portfolio_total: %s", total.__dict__)
             self.assertIsNotNone(total.degiro_cash)
             self.assertIsNotNone(total.total_cash)
             self.assertIsNotNone(total.free_space_new)
             self.assertIsNotNone(total.report_portf_value)
             self.assertIsNotNone(total.report_cash_bal)
 
         async def test_get_portfolio_products_info(self):
-            session = await self._login()
+            session = await _IntegrationLogin._login()
             positions = await degiroasync.api.get_portfolio(session)
             LOGGER.debug("test_get_portfolio_products_info: %s",
                          pprint.pformat(tuple(p.__dict__ for p in positions)))
 
             self.assertGreaterEqual(
                     len(positions), 1,
                     "If there is no product in portfolio, this is expected to "
@@ -412,15 +427,15 @@
                                       f"{product.base.id}:{product.info.name}")
 
     class TestDegiroasyncIntegrationPrice(
             _IntegrationLogin,
             unittest.IsolatedAsyncioTestCase):
 
         async def test_get_price_data(self):
-            session = await self._login()
+            session = await _IntegrationLogin._login()
             products = await degiroasync.api.search_product(
                     session,
                     by_isin='NL0000235190',
                     product_type_id=PRODUCT.TYPEID.STOCK
                     )
             #products_awaitable = [p.await_product_info() for p in products]
             #LOGGER.debug('test_get_price_data products_awaitable| %s', products_awaitable)
@@ -460,15 +475,15 @@
             LOGGER.debug('test_get_price_data price_data 2| %s',
                          price_data)
             self.assertGreaterEqual(len(price_data.price), 1)
             self.assertGreaterEqual(len(price_data.date), 1)
 
         async def test_get_price_data_symbol_exchange(self):
             # First get product
-            session = await self._login()
+            session = await _IntegrationLogin._login()
             symbol = 'FGR'
             exchange = 'EPA'
             products = await degiroasync.api.search_product(
                     session,
                     by_symbol=symbol,
                     by_exchange=exchange,
                     product_type_id=PRODUCT.TYPEID.STOCK)
@@ -483,15 +498,15 @@
             self.assertGreaterEqual(len(price_data.date), 1)
 
             date = price_data.date
             price = price_data.price
             self.assertEqual(len(date), len(price))
 
         async def test_get_price_data_day_resolution(self):
-            session = await self._login()
+            session = await _IntegrationLogin._login()
             products = await degiroasync.api.search_product(
                     session,
                     by_isin='NL0000235190',
                     by_exchange='EPA',
                     product_type_id=PRODUCT.TYPEID.STOCK
                     )
             LOGGER.debug('test_get_price_data_day_resolution| products %s',
@@ -531,92 +546,79 @@
             self.assertGreaterEqual(
                     len(date_series), 15,
                     "We should have daily data for a month with one sample "
                     "per day.")
 
             # We entered PT1D resolution, check that we have one data point
             # per day at most
-            start = datetime.datetime.now() - datetime.timedelta(days=32)
+            start = datetime.datetime.now() - datetime.timedelta(days=60)
             prior_day = datetime.datetime(start.year, start.month, start.day)
             for date_str in date_series:
                 date = datetime.datetime.fromisoformat(date_str)
                 day = datetime.datetime(date.year, date.month, date.day)
                 delta_days = (day - prior_day).days
                 self.assertGreaterEqual(
                         delta_days, 1,
                         "day {}, prior_day {}".format(
                             day.isoformat(),
                             prior_day.isoformat()
                             ))
 
                 prior_day = day
 
-
-        #async def test_get_price_data_bulk(self):
-        #    raise NotImplementedError
-        #    session = await self._login()
-        #    #degiroasync.api.Product
-        #    _, products = await degiroasync.api.get_portfolio(session)
-        #    # In a context where we'd want to optimize, we want to 
-        #    # build the pipeline by awaiting on each product instead of a bulk
-        #    # gather to not block execution while we wait for data on some
-        #    # of the products.
-        #    await asyncio.gather(await p.await_product_info() for p in products)
-        #    products = filter(lambda p: p.info.productType == ProductConst.Type.STOCKS, products)
-        #    price_data = await degiroasync.api.get_price_data_bulk(session, products)
-
     class TestDegiroasyncIntegrationSearch(
             _IntegrationLogin,
             unittest.IsolatedAsyncioTestCase):
         async def test_search_product_isin(self):
-            session = await self._login()
+            session = await _IntegrationLogin._login()
             isin = 'NL0000235190'  # Airbus ISIN
-            products = await degiroasync.api.search_product(session,
+            products = await degiroasync.api.search_product(
+                    session,
                     by_isin=isin)
             self.assertGreaterEqual(len(products), 1)
             for product in products:
                 # We should only have airbus products here
                 self.assertTrue('airbus' in product.info.name.lower())
 
         async def test_search_product_symbol(self):
-            session = await self._login()
+            session = await _IntegrationLogin._login()
             symbol = 'AIR'
             products = await degiroasync.api.search_product(session,
                                                             by_symbol=symbol)
             self.assertGreaterEqual(len(products), 1)
             for product in products:
                 self.assertEqual(symbol, product.info.symbol, product.info)
                 # We should only have airbus products here
                 #self.assertTrue('airbus' in product.info.name.lower(),
                 #               product.info)
 
-        async def test_search_product_symbol_gne(self):
-            session = await self._login()
-            symbol = 'GNE'  # GE symbol on EPA
+        async def test_search_product_symbol_air(self):
+            session = await _IntegrationLogin._login()
+            symbol = 'AIR'  # GE symbol on EPA
             products = await degiroasync.api.search_product(session,
                                                             by_symbol=symbol,
                                                             by_exchange='EPA')
             self.assertGreaterEqual(len(products), 1)
             for product in products:
                 # We should only have airbus products here
                 self.assertTrue(
-                        'general electric' in product.info.name.lower())
+                        'airbus' in product.info.name.lower())
 
         async def test_search_product_text(self):
-            session = await self._login()
+            session = await _IntegrationLogin._login()
             products = await degiroasync.api.search_product(
                     session,
                     by_text='airbus')
             self.assertGreaterEqual(len(products), 1)
             for product in products:
                 # We should only have airbus products here
                 self.assertTrue('airbus' in product.info.name.lower())
 
         async def test_search_product_symbol_exchange(self):
-            session = await self._login()
+            session = await _IntegrationLogin._login()
             symbol = 'AIR'  # Airbus symbol
             exchange_hiq = 'EPA'
             products = await degiroasync.api.search_product(
                     session,
                     by_symbol=symbol,
                     by_exchange=exchange_hiq)
             # The point of implementing filtering on symbol and exchange
@@ -627,44 +629,44 @@
                 # We should only have airbus products here
                 self.assertTrue('airbus' in product.info.name.lower())
 
     class TestDegiroasyncIntegrationExchangeDictionary(
             _IntegrationLogin,
             unittest.IsolatedAsyncioTestCase):
         async def test_product_dictionary_attributes(self):
-            session = await self._login()
+            session = await _IntegrationLogin._login()
             dictionary = await degiroasync.api.ExchangeDictionary(session)
 
             regions = dictionary.regions
             self.assertIn('Europe', (r.name for r in regions))
             countries = dictionary.countries
             self.assertIn('NL', (c.name for c in countries))
             exchanges = dictionary.exchanges
             self.assertIn('XAMS', (e.mic_code for e in exchanges))
 
         async def test_product_dictionary_exchange_by(self):
-            session = await self._login()
+            session = await _IntegrationLogin._login()
             dictionary = await degiroasync.api.ExchangeDictionary(session)
             eam_exc = dictionary.exchange_by(hiq_abbr='EAM')
             self.assertEqual(eam_exc.mic_code, 'XAMS')
             self.assertEqual(eam_exc.country_name, 'NL')
 
     class TestDegiroasyncIntegrationOrders(
             _IntegrationLogin,
             unittest.IsolatedAsyncioTestCase):
         async def test_get_orders(self):
-            session = await self._login()
+            session = await _IntegrationLogin._login()
             orders, orders_hist = await degiroasync.api.get_orders(session)
             LOGGER.debug("test_get_orders orders| %s", orders)
             LOGGER.debug("test_get_orders orders hist| %s", orders_hist)
             for o in itertools.chain(orders, orders_hist):
                 self.assertTrue(isinstance(o, Order))
 
         async def test_get_transactions(self):
-            session = await self._login()
+            session = await _IntegrationLogin._login()
             to_date = datetime.datetime.today()
             from_date = datetime.datetime(year=to_date.year - 2,
                                           month=1,
                                           day=1)
             LOGGER.debug("test_get_transactions params| %s",
                          (from_date, to_date))
             transactions = await degiroasync.api.get_transactions(
@@ -682,15 +684,15 @@
             for trans in transactions:
                 self.assertTrue(hasattr(trans, 'product'))
                 self.assertTrue(hasattr(trans, 'price'))
                 self.assertTrue(hasattr(trans, 'quantity'))
                 self.assertTrue(hasattr(trans, 'fx_rate'))
 
         async def test_check_orders(self):
-            session = await self._login()
+            session = await _IntegrationLogin._login()
             products = await degiroasync.api.search_product(
                     session,
                     by_symbol='AIR',
                     by_exchange='EPA',
                     product_type_id=PRODUCT.TYPEID.STOCK
             )
             self.assertEqual(len(products), 1)
@@ -702,7 +704,18 @@
                     buy_sell=ORDER.ACTION.BUY,
                     time_type=ORDER.TIME.DAY,
                     order_type=ORDER.TYPE.LIMITED,
                     size=1,
                     price=80
             )
             self.assertIn('confirmation_id', order_check)
+
+if __name__ == '__main__':
+    handler = logging.StreamHandler()
+    handler.setLevel(logging.DEBUG)
+    formatter = logging.Formatter(
+            "%(asctime)s-%(name)s-%(levelname)s-%(message)",
+            "%Y%m%d"
+            )
+    LOGGER.addHandler(handler)
+    LOGGER.setLevel(logging.DEBUG)
+    unittest.main()
```

### Comparing `degiroasync-0.16.0/tests/test_degirowebapi.py` & `degiroasync-0.17.0/tests/test_degirowebapi.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,178 +1,209 @@
 import unittest
 import logging
 import os
 import pprint
 import asyncio
 import datetime
+from typing import Optional
+import unittest.mock
+from unittest.mock import MagicMock
 
+import httpx
 
 import degiroasync
 import degiroasync.webapi
 import degiroasync.core
 import degiroasync.core.helpers
 from degiroasync.core import Credentials
+from degiroasync.core import SessionCore
 from degiroasync.core.constants import PRODUCT
 from degiroasync.core.constants import PRICE
 from degiroasync.core.constants import ORDER
+from degiroasync.core.constants import LOGIN
+from degiroasync.core import ResponseError
+from degiroasync.core import BadCredentialsError
 from degiroasync.webapi import get_config
 from degiroasync.webapi import get_products_info
 from degiroasync.webapi import get_company_profile
 from degiroasync.webapi import get_news_by_company
 
 
 LOGGER = logging.getLogger(degiroasync.core.LOGGER_NAME)
-#degiroasync.core.helpers.set_logs(LOGGER, logging.DEBUG)
 
 RUN_INTEGRATION_TESTS = 0
 try:
     _env_var = os.environ.get('DEGIROASYNC_INTEGRATION')
     RUN_INTEGRATION_TESTS = int(_env_var)
-except ValueError:
+except (ValueError, TypeError):
     LOGGER.info('degiroasync integration tests will *not* run.')
 
 
-def _get_credentials():
-    """
-    Helper to get credentials for integration tests
-    """
-    username = os.environ.get('DEGIRO_USERNAME')
-    password = os.environ.get('DEGIRO_PASSWORD')
-    assert username is not None, (
-        'DEGIRO_USERNAME environment variable not defined.')
-    assert password is not None, (
-        'DEGIRO_PASSWORD environment variable not defined.')
-    totp_secret = os.environ.get('DEGIRO_TOTP_SECRET')
-
-    return Credentials(username, password, totp_secret)
-
-
-#def mock_asyncclient(mock):
-#    pass
-#
-#
-#class TestDegiroWebAPIUnit(unittest.IsolatedAsyncioTestCase):
-#    @unittest.mock.patch('httpx.AsyncClient')
-#    async def test_confirm_order(self, asyncclient_mock):
-#        pass
+class TestDegiroAsyncWebAPI(unittest.IsolatedAsyncioTestCase):
+    @unittest.mock.patch('httpx.AsyncClient.post')
+    async def test_login_bad_credentials(
+            self,
+            post_m
+            ):
+        """
+        Verify that BadCredentialsError is raised when endpoint returns a bad
+        credentials error.
+        """
+        post_m.return_value = MagicMock()
+        response = post_m.return_value
+        response.json = MagicMock(
+                return_value={
+                    'status': LOGIN.BAD_CREDENTIALS,
+                    'content': 'badCredentials'})
+        response.status_code = httpx.codes.BAD_REQUEST
+
+        credentials = Credentials(
+            username='dummyaccount123456',
+            password='dummydummy'
+                )
+        with self.assertRaises(BadCredentialsError):
+            await degiroasync.webapi.login(credentials)
 
 
 if RUN_INTEGRATION_TESTS:
     LOGGER.info('degiroasync.webapi integration tests will run.')
+    from tests.integration_login import _IntegrationLogin
 
-    class _IntegrationWebLogin:
-        """
-        Internal helper, can be inherited to make login for integration tests
-        easier.
-        """
-        async def asyncSetUp(self):
-            self._lock = asyncio.Lock()
+    #class _IntegrationWebLogin:
+    #    """
+    #    Internal helper, can be inherited to make login for integration tests
+    #    easier.
+    #    """
+    #    async def asyncSetUp(self):
+    #        self._lock = asyncio.Lock()
+    #        _IntegrationLogin._login_attempted = False
+    #        self.session: Optional[SessionCore] = None
+
+    #    async def _login(self):
+    #        if self.session is not None:
+    #            return self.session
+    #        async with self._lock:
+    #            if not _IntegrationLogin._login_attempted and not self.session:
+    #                _IntegrationLogin._login_attempted = True
+    #                credentials = _get_credentials()
+    #                import degiroasync.api
+    #                # Use api.login here to benefit from wrong password check:
+    #                # if provided credentials are incorrect, don't try again
+    #                # This will block the degiro account.
+    #                self.session = await degiroasync.api.login(
+    #                        credentials)
+    #            else:
+    #                LOGGER.warning(
+    #                        "Log in already attempted without success, skip.")
+    #        if not self.session:
+    #            raise ResponseError("No session available.")
+    #        return self.session
 
-        async def _login(self):
-            async with self._lock:
-                if not hasattr(self, 'session'):
-                    credentials = _get_credentials()
-                    self.session = await degiroasync.webapi.login(credentials)
-                    await degiroasync.webapi.get_config(self.session)
-                    await degiroasync.webapi.get_client_info(self.session)
-            return self.session
-
-    class TestDegiroWebAPIIntegration(
-            _IntegrationWebLogin,
+    class TestDegiroAsyncWebAPIIntegration(
+            _IntegrationLogin,
             unittest.IsolatedAsyncioTestCase):
 
         async def test_login(self):
-            session = await self._login()
+            session = await _IntegrationLogin._login()
             self.assertTrue('JSESSIONID' in session.cookies,
                             "No JSESSIONID found.")
 
+        async def test_login_bad_credentials(self):
+            credentials = Credentials(
+                username='dummyaccount123456',
+                password='dummydummy'
+                    )
+            with self.assertRaises(BadCredentialsError):
+                await degiroasync.webapi.login(credentials)
+
         async def test_config(self):
-            session = await self._login()
+            session = await _IntegrationLogin._login()
             await get_config(session)
             LOGGER.debug('test_config| %s', session.config)
-            self.assertTrue(session.config.pa_url is not None,
+            self.assertTrue(
+                    session.config.pa_url is not None,
                     "paUrl not defined.")
-            self.assertTrue(session.config.product_search_url is not None,
+            self.assertTrue(
+                    session.config.product_search_url is not None,
                     "productSearchUrl not defined.")
-            self.assertTrue(session.config.trading_url is not None,
+            self.assertTrue(
+                    session.config.trading_url is not None,
                     "tradingUrl not defined.")
 
-        async def test_porfolio(self):
-            session = await self._login()
+        async def test_portfolio(self):
+            session = await _IntegrationLogin._login()
 
             resp_json = await degiroasync.webapi.get_portfolio(session)
             LOGGER.debug("test_portfolio| %s", resp_json)
             self.assertTrue('portfolio' in resp_json)
             self.assertTrue('value' in resp_json['portfolio'])
 
-        async def test_porfolio_total(self):
-            session = await self._login()
+        async def test_portfolio_total(self):
+            session = await _IntegrationLogin._login()
 
             resp_json = await degiroasync.webapi.get_portfolio_total(session)
             LOGGER.debug("test_portfolio_total| %s", resp_json)
-            #self.assertIn(response.status_code, (200, 201))
             self.assertTrue('totalPortfolio' in resp_json)
             self.assertTrue('value' in resp_json['totalPortfolio'])
 
         async def test_get_products_info(self):
-            session = await self._login()
+            session = await _IntegrationLogin._login()
 
             resp_json = await degiroasync.webapi.get_portfolio(session)
             portfolio = resp_json['portfolio']
             product_ids = filter(lambda x: x is not None,
                                  (product.get('id')
                                   for product in portfolio['value']))
             response = await get_products_info(session,
                                                [p for p in product_ids])
-            #self.assertEqual(response.status_code, 200)
             self.assertIsInstance(response, dict)
 
             response = await degiroasync.webapi.get_products_info(session,
                                                                   ["72906"])
             self.assertIsInstance(response, dict)
             LOGGER.debug('webapi.test_get_products_info| %s',
                          pprint.pformat(response))
 
         async def test_get_company_profile(self):
-            session = await self._login()
+            session = await _IntegrationLogin._login()
 
-            isin = "FR0010242511"
+            isin = "NL0000235190"
             resp_json = await get_company_profile(session, isin)
             self.assertTrue('data' in resp_json, resp_json)
             self.assertTrue('businessSummary' in resp_json['data'], resp_json)
             LOGGER.debug('webapi.test_get_company_profile| %s',
                          pprint.pformat(resp_json))
 
         async def test_get_news_by_company(self):
-            session = await self._login()
+            session = await _IntegrationLogin._login()
 
-            isin = "FR0010242511"
+            isin = "NL0000235190"
             resp_json = await get_news_by_company(session, isin)
             self.assertTrue('data' in resp_json, resp_json)
             self.assertTrue('items' in resp_json['data'], resp_json)
 
         async def test_get_price_data(self):
             """
             Simply check that we don't have an error and data is not empty.
             """
-            session = await self._login()
+            session = await _IntegrationLogin._login()
 
             vwdId = '360114899'
 
             resp_json = await degiroasync.webapi.get_price_data(
                     session,
                     vwdId=vwdId,
                     vwdIdentifierType='issueid')
             LOGGER.debug('get_price_data response: %s', resp_json)
             LOGGER.debug(resp_json)
             self.assertIn('series', resp_json)
             self.assertIn('data', resp_json['series'][0])
 
         async def test_get_price_data_month(self):
-            session = await self._login()
+            session = await _IntegrationLogin._login()
 
             vwdId = '360114899'
 
             resp_json = await degiroasync.webapi.get_price_data(
                     session,
                     vwdId=vwdId,
                     period=PRICE.PERIOD.P1MONTH,
@@ -181,15 +212,15 @@
             LOGGER.debug(resp_json)
             self.assertIn('resolution', resp_json)
             self.assertEqual(resp_json['resolution'], PRICE.RESOLUTION.PT1M)
             self.assertIn('series', resp_json)
             self.assertIn('data', resp_json['series'][0])
 
         async def test_get_price_data_month_pt1d(self):
-            session = await self._login()
+            session = await _IntegrationLogin._login()
 
             vwdId = '360114899'
 
             resp_json = await degiroasync.webapi.get_price_data(
                     session,
                     vwdId=vwdId,
                     period=PRICE.PERIOD.P1MONTH,
@@ -200,60 +231,62 @@
             LOGGER.debug(resp_json)
             self.assertIn('resolution', resp_json)
             self.assertEqual(resp_json['resolution'], PRICE.RESOLUTION.PT1D)
             self.assertIn('series', resp_json)
             self.assertIn('data', resp_json['series'][0])
 
         async def test_search_product(self):
-            session = await self._login()
+            session = await _IntegrationLogin._login()
 
             search = "AIRBUS"
             resp_json = await degiroasync.webapi.search_product(
                     session,
                     search)
             self.assertIn('products', resp_json, resp_json)
             self.assertGreaterEqual(len(resp_json['products']), 1)
             self.assertIn('id', resp_json['products'][0], resp_json)
             self.assertIn('isin', resp_json['products'][0], resp_json)
             self.assertIn('name', resp_json['products'][0], resp_json)
 
         async def test_product_dictionary(self):
-            session = await self._login()
+            session = await _IntegrationLogin._login()
 
-            resp_json = await degiroasync.webapi.get_product_dictionary(session)
+            resp_json = await degiroasync.webapi.get_product_dictionary(
+                    session
+                    )
 
             self.assertIn('exchanges', resp_json)
             self.assertIn('countries', resp_json)
             self.assertIn('regions', resp_json)
 
             # Not used by degiroasync.api at the time this test was written.
             self.assertIn('bondExchanges', resp_json)
             self.assertIn('cfdExchanges', resp_json)
             self.assertIn('combinationExchanges', resp_json)
             self.assertIn('etfAggregateTypes', resp_json)
             self.assertIn('etfFeeTypes', resp_json)
             self.assertIn('eurexCountries', resp_json)
 
     class TestDegiroWebAPIOrdersIntegration(
-            _IntegrationWebLogin,
+            _IntegrationLogin,
             unittest.IsolatedAsyncioTestCase):
         """
         Set Orders will *not* be tested: this would imply being charged every
         time tests are executed.
         """
         async def test_get_orders(self):
-            session = await self._login()
+            session = await _IntegrationLogin._login()
 
             resp_json = await degiroasync.webapi.get_orders(session)
             LOGGER.debug("test_get_orders| %s", pprint.pformat(resp_json))
             self.assertIn('orders', resp_json)
             self.assertIsInstance(resp_json['orders'], list)
 
         async def test_check_order(self):
-            session = await self._login()
+            session = await _IntegrationLogin._login()
 
             # Leverage api.search_product to get a specific product_id
             # as example for integration testing of check_order.
             # This is introducing a dependency on api module, but is easier
             # to manage. Future improvement opportunit for this test: implement
             # required query and filter here using only webapi.
             from degiroasync import api
@@ -307,26 +340,26 @@
             self.assertIn('freeSpaceNew', resp_json['data'])
             self.assertTrue(
                     'transactionFee' in resp_json['data']
                     or 'transactionOppositeFee' in resp_json['data'],
                     resp_json['data'])
 
         async def test_get_account_info(self):
-            session = await self._login()
+            session = await _IntegrationLogin._login()
             resp_json = await degiroasync.webapi.get_account_info(session)
             LOGGER.debug("test_get_account_info| response: %s", resp_json)
 
             self.assertIn('data', resp_json)
             self.assertIn('clientId', resp_json['data'])
             self.assertIn('baseCurrency', resp_json['data'])
             # Not sure what more to test here. To be extended when this call
             # usage has been identified.
 
         async def test_get_orders_history(self):
-            session = await self._login()
+            session = await _IntegrationLogin._login()
             to_date = datetime.datetime.today()
             from_date = datetime.datetime.today() - datetime.timedelta(days=7)
             date_format = degiroasync.webapi.orders.ORDER_DATE_FORMAT
             resp_json = await degiroasync.webapi.get_orders_history(
                     session,
                     from_date=from_date.strftime(date_format),
                     to_date=to_date.strftime(date_format)
@@ -349,23 +382,23 @@
                 self.assertIn('status', order)
                 self.assertIn('last', order)
                 self.assertIn('isActive', order)
                 self.assertIn('currentTradedSize', order)
                 self.assertIn('totalTradedSize', order)
 
         async def test_get_orders_history_date_check(self):
-            session = await self._login()
+            session = await _IntegrationLogin._login()
             with self.assertRaises(ValueError):
                 await degiroasync.webapi.get_orders_history(
                     session,
                     from_date='garbage',
                     to_date='garbage')
 
         async def test_get_transactions(self):
-            session = await self._login()
+            session = await _IntegrationLogin._login()
             to_date = datetime.datetime.today()
             from_date = datetime.datetime.today() - datetime.timedelta(days=7)
             date_format = degiroasync.webapi.orders.ORDER_DATE_FORMAT
             resp_json = await degiroasync.webapi.get_transactions(
                     session,
                     from_date=from_date.strftime(date_format),
                     to_date=to_date.strftime(date_format)
@@ -383,13 +416,25 @@
                 self.assertIn('nettFxRate', trans)
                 self.assertIn('transfered', trans)
                 self.assertIn('buysell', trans)
                 self.assertIn(trans['buysell'], ('B', 'S'))
                 self.assertIn('transactionTypeId', trans)
 
         async def test_get_transactions_date_check(self):
-            session = await self._login()
+            session = await _IntegrationLogin._login()
             with self.assertRaises(ValueError):
                 await degiroasync.webapi.get_orders_history(
                     session,
                     from_date='garbage',
                     to_date='garbage')
+
+
+if __name__ == '__main__':
+    handler = logging.StreamHandler()
+    handler.setLevel(logging.DEBUG)
+    formatter = logging.Formatter(
+            "%(asctime)s-%(name)s-%(levelname)s-%(message)",
+            "%Y%m%d"
+            )
+    LOGGER.addHandler(handler)
+    LOGGER.setLevel(logging.DEBUG)
+    unittest.main()
```

