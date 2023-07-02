# Comparing `tmp/warframe.py-0.5.0.tar.gz` & `tmp/warframe.py-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "warframe.py-0.5.0.tar", last modified: Sun Jul  2 07:38:07 2023, max compression
+gzip compressed data, was "warframe.py-0.6.0.tar", last modified: Sun Jul  2 18:10:42 2023, max compression
```

## Comparing `warframe.py-0.5.0.tar` & `warframe.py-0.6.0.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 07:38:07.117260 warframe.py-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-07-02 07:37:32.000000 warframe.py-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-07-02 07:38:07.117260 warframe.py-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-07-02 07:37:32.000000 warframe.py-0.5.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-02 07:37:32.000000 warframe.py-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-02 07:38:07.117260 warframe.py-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-07-02 07:37:32.000000 warframe.py-0.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 07:38:07.113260 warframe.py-0.5.0/warframe/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 07:38:07.117260 warframe.py-0.5.0/warframe/worldstate/
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-02 07:37:32.000000 warframe.py-0.5.0/warframe/worldstate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10385 2023-07-02 07:37:32.000000 warframe.py-0.5.0/warframe/worldstate/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 07:38:07.117260 warframe.py-0.5.0/warframe/worldstate/common/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-02 07:37:32.000000 warframe.py-0.5.0/warframe/worldstate/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-07-02 07:37:32.000000 warframe.py-0.5.0/warframe/worldstate/common/core.py
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-07-02 07:37:32.000000 warframe.py-0.5.0/warframe/worldstate/common/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-07-02 07:37:32.000000 warframe.py-0.5.0/warframe/worldstate/common/types_.py
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-07-02 07:37:32.000000 warframe.py-0.5.0/warframe/worldstate/endpoints.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 07:38:07.117260 warframe.py-0.5.0/warframe/worldstate/enums/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-02 07:37:32.000000 warframe.py-0.5.0/warframe/worldstate/enums/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-02 07:37:32.000000 warframe.py-0.5.0/warframe/worldstate/enums/faction.py
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-02 07:37:32.000000 warframe.py-0.5.0/warframe/worldstate/enums/language.py
--rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-07-02 07:37:32.000000 warframe.py-0.5.0/warframe/worldstate/enums/mission_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-07-02 07:37:32.000000 warframe.py-0.5.0/warframe/worldstate/enums/syndicate.py
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-07-02 07:37:32.000000 warframe.py-0.5.0/warframe/worldstate/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 07:38:07.117260 warframe.py-0.5.0/warframe/worldstate/models/
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-07-02 07:37:32.000000 warframe.py-0.5.0/warframe/worldstate/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-07-02 07:37:32.000000 warframe.py-0.5.0/warframe/worldstate/models/alert.py
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-02 07:37:32.000000 warframe.py-0.5.0/warframe/worldstate/models/arbitration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-07-02 07:37:32.000000 warframe.py-0.5.0/warframe/worldstate/models/archon_hunt.py
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-02 07:37:32.000000 warframe.py-0.5.0/warframe/worldstate/models/cambion_drift.py
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-07-02 07:37:32.000000 warframe.py-0.5.0/warframe/worldstate/models/cetus.py
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-02 07:37:32.000000 warframe.py-0.5.0/warframe/worldstate/models/counted_item.py
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-02 07:37:32.000000 warframe.py-0.5.0/warframe/worldstate/models/daily_deal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-07-02 07:37:32.000000 warframe.py-0.5.0/warframe/worldstate/models/event.py
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-07-02 07:37:32.000000 warframe.py-0.5.0/warframe/worldstate/models/fissure.py
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-07-02 07:37:32.000000 warframe.py-0.5.0/warframe/worldstate/models/flash_sale.py
--rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-07-02 07:37:32.000000 warframe.py-0.5.0/warframe/worldstate/models/invasion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-07-02 07:37:32.000000 warframe.py-0.5.0/warframe/worldstate/models/mission.py
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-07-02 07:37:32.000000 warframe.py-0.5.0/warframe/worldstate/models/orb_vallis.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-02 07:37:32.000000 warframe.py-0.5.0/warframe/worldstate/models/reward.py
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-02 07:37:32.000000 warframe.py-0.5.0/warframe/worldstate/models/sortie.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-02 07:37:32.000000 warframe.py-0.5.0/warframe/worldstate/models/void_trader.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 07:37:32.000000 warframe.py-0.5.0/warframe/worldstate/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 07:38:07.117260 warframe.py-0.5.0/warframe.py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-07-02 07:38:07.000000 warframe.py-0.5.0/warframe.py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-07-02 07:38:07.000000 warframe.py-0.5.0/warframe.py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 07:38:07.000000 warframe.py-0.5.0/warframe.py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-02 07:38:07.000000 warframe.py-0.5.0/warframe.py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-02 07:38:07.000000 warframe.py-0.5.0/warframe.py.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 18:10:42.974908 warframe.py-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-07-02 18:10:07.000000 warframe.py-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-07-02 18:10:42.974908 warframe.py-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-07-02 18:10:07.000000 warframe.py-0.6.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-02 18:10:07.000000 warframe.py-0.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-02 18:10:42.978908 warframe.py-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-07-02 18:10:07.000000 warframe.py-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 18:10:42.970908 warframe.py-0.6.0/warframe/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 18:10:42.974908 warframe.py-0.6.0/warframe/worldstate/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-02 18:10:07.000000 warframe.py-0.6.0/warframe/worldstate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11113 2023-07-02 18:10:07.000000 warframe.py-0.6.0/warframe/worldstate/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 18:10:42.974908 warframe.py-0.6.0/warframe/worldstate/common/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-02 18:10:07.000000 warframe.py-0.6.0/warframe/worldstate/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-07-02 18:10:07.000000 warframe.py-0.6.0/warframe/worldstate/common/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-07-02 18:10:07.000000 warframe.py-0.6.0/warframe/worldstate/common/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-07-02 18:10:07.000000 warframe.py-0.6.0/warframe/worldstate/common/types_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-07-02 18:10:07.000000 warframe.py-0.6.0/warframe/worldstate/endpoints.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 18:10:42.974908 warframe.py-0.6.0/warframe/worldstate/enums/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-02 18:10:07.000000 warframe.py-0.6.0/warframe/worldstate/enums/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-02 18:10:07.000000 warframe.py-0.6.0/warframe/worldstate/enums/faction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-02 18:10:07.000000 warframe.py-0.6.0/warframe/worldstate/enums/language.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-07-02 18:10:07.000000 warframe.py-0.6.0/warframe/worldstate/enums/mission_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-07-02 18:10:07.000000 warframe.py-0.6.0/warframe/worldstate/enums/syndicate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-07-02 18:10:07.000000 warframe.py-0.6.0/warframe/worldstate/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 18:10:42.974908 warframe.py-0.6.0/warframe/worldstate/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-07-02 18:10:07.000000 warframe.py-0.6.0/warframe/worldstate/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-07-02 18:10:07.000000 warframe.py-0.6.0/warframe/worldstate/models/alert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-02 18:10:07.000000 warframe.py-0.6.0/warframe/worldstate/models/arbitration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-07-02 18:10:07.000000 warframe.py-0.6.0/warframe/worldstate/models/archon_hunt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-02 18:10:07.000000 warframe.py-0.6.0/warframe/worldstate/models/cambion_drift.py
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-07-02 18:10:07.000000 warframe.py-0.6.0/warframe/worldstate/models/cetus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-02 18:10:07.000000 warframe.py-0.6.0/warframe/worldstate/models/counted_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-02 18:10:07.000000 warframe.py-0.6.0/warframe/worldstate/models/daily_deal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-07-02 18:10:07.000000 warframe.py-0.6.0/warframe/worldstate/models/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-07-02 18:10:07.000000 warframe.py-0.6.0/warframe/worldstate/models/fissure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-07-02 18:10:07.000000 warframe.py-0.6.0/warframe/worldstate/models/flash_sale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-07-02 18:10:07.000000 warframe.py-0.6.0/warframe/worldstate/models/invasion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-07-02 18:10:07.000000 warframe.py-0.6.0/warframe/worldstate/models/mission.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-07-02 18:10:07.000000 warframe.py-0.6.0/warframe/worldstate/models/orb_vallis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-02 18:10:07.000000 warframe.py-0.6.0/warframe/worldstate/models/reward.py
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-02 18:10:07.000000 warframe.py-0.6.0/warframe/worldstate/models/sortie.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-02 18:10:07.000000 warframe.py-0.6.0/warframe/worldstate/models/void_trader.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 18:10:07.000000 warframe.py-0.6.0/warframe/worldstate/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 18:10:42.974908 warframe.py-0.6.0/warframe.py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-07-02 18:10:42.000000 warframe.py-0.6.0/warframe.py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-07-02 18:10:42.000000 warframe.py-0.6.0/warframe.py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 18:10:42.000000 warframe.py-0.6.0/warframe.py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-02 18:10:42.000000 warframe.py-0.6.0/warframe.py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-02 18:10:42.000000 warframe.py-0.6.0/warframe.py.egg-info/top_level.txt
```

### Comparing `warframe.py-0.5.0/LICENSE` & `warframe.py-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `warframe.py-0.5.0/PKG-INFO` & `warframe.py-0.6.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: warframe.py
-Version: 0.5.0
+Version: 0.6.0
 Summary: An asynchronous Python API wrapper for the Warframestat API and (later) the warframe.market API.
 Home-page: https://github.com/WFCD/warframe.py
 Author: Mettwasser
 License: MIT
 Keywords: Warframe API worldstate market wrapper
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
@@ -34,29 +34,48 @@
 This library is in its early states. The goal is to make it the best and most up-to-date Python Warframe API wrapper.
 
 Quickstart
 ----------
 
 .. code-block:: python
 
+    # queries are just another way to get the data to the corresponding objects.
+    # this is really just personal preference.
+
     import asyncio
+    import logging
 
-    from warframe.worldstate import Language, WorldstateClient
+    from warframe.worldstate import WorldstateClient, WorldstateLogger
+    
+    # import the models you want to use
+    from warframe.worldstate.models import Cetus
 
 
     async def main():
-        async with WorldstateClient() as client:
-            cetus = await client.get_cetus(language=Language.English)  # english is default
-            print(cetus.short_string)
+        # Note that the default logger is pretty much empty (nothing will be logged)
+        # so if you want to make use of the logger, make your own:
+        logger = WorldstateLogger("name whatever you want", logging.DEBUG)
+        logger.addHandler(logging.StreamHandler())
+
+        async with WorldstateClient(logger=logger) as client:  # pass the logger
+            cetus = await client.get_cetus()
+            # or ...
+
+            # just throw the model into `query(type)`
+            # note that for stuff like fissures you need `query_list_of(type)`
+            cetus = await client.query(Cetus)
+
+            print(cetus)
 
 
     if __name__ == "__main__":
         loop = asyncio.new_event_loop()
         loop.run_until_complete(main())
 
+
 Installing
 ----------
 
 To install the library, use the following command:
 
 .. code-block:: bash
```

### Comparing `warframe.py-0.5.0/setup.py` & `warframe.py-0.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `warframe.py-0.5.0/warframe/worldstate/client.py` & `warframe.py-0.6.0/warframe/worldstate/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,35 +3,46 @@
 from functools import wraps
 from typing import (
     Any,
     Callable,
     ClassVar,
     Coroutine,
     List,
-    NamedTuple,
     Optional,
     Protocol,
     Type,
     TypeVar,
 )
 
 import aiohttp
 import msgspec
 
-from .common import MultiQueryModel, SingleQueryModel, TimedEvent, WorldstateObject
+from .common import (
+    MultiQueryModel,
+    SingleQueryModel,
+    TimedEvent,
+    WorldstateLogger,
+    WorldstateObject,
+)
 from .endpoints import Language, build_endpoint
 from .exceptions import ErrorMessage, SessionNotFound, WorldstateAPIError
 from .models import Alert, CambionDrift, Cetus, OrbVallis
 
 __all__ = ["WorldstateClient"]
 
 SupportsSingleQuery = TypeVar("SupportsSingleQuery", bound=SingleQueryModel)
 SupportsMultiQuery = TypeVar("SupportsMultiQuery", bound=MultiQueryModel)
 
 
+def _get_default_logger() -> WorldstateLogger:
+    logger = WorldstateLogger("main_wsclient_logger")
+
+    return logger
+
+
 class _TaskHelper:
     def __init__(self, loop: Callable[..., Coroutine[Any, Any, None]]) -> None:
         self._loop_function = loop
         self._task: Optional[asyncio.Task] = None
 
     def start(self) -> None:
         if self._task is None:
@@ -86,109 +97,146 @@
     """
 
     def __init__(
         self,
         *,
         session: Optional[aiohttp.ClientSession] = None,
         default_language: Language = Language.EN,
+        logger: Optional[WorldstateLogger] = None,
     ) -> None:
+        """
+        Parameters
+        ----------
+        session : Optional[aiohttp.ClientSession], optional
+            The `aiohttp.ClientSession` the client will perform the requests on, by default None
+        default_language : Language, optional
+            The default language the objects will be in, by default `Language.EN`
+        logger : Optional[WorldstateLogger], optional
+            The logger that will log messages, by default None
+        """
         self._session = session
         self._session_created = False
 
         self._default_lang = default_language
 
-        self._debug = True
+        self._logger = logger or _get_default_logger()
 
     #
     # Request
     #
 
     async def _request(self, endpoint: str, language: Optional[Language]) -> str:
-        """Sends a request to the given `endpoint` and returns its JSON content as string.
-
-        Args:
-            endpoint (str): The endpoint to send the request to.
-            language (Optional[Language]): The language of the response.
-
-        Raises:
-            SessionNotFound: When the client's session is gone / None for some reason.
-            WorldstateAPIError: When the API returns a faulty response.
+        """
+        Sends a request to the given `endpoint` and returns its JSON content as string.
 
-        Returns:
-            str: The JSON content as string.
+        Parameters
+        ----------
+        endpoint : str
+            The endpoint to send the request to.
+        language : Optional[Language], optional
+            The language of the response, by default None
+
+        Raises
+        ------
+        SessionNotFound
+            When the client's session is gone / None for some reason.
+        WorldstateAPIError
+            When the API returns a faulty response.
+
+        Returns
+        -------
+        str
+            The JSON content as string.
         """
+
         if not self._session:
             self._session = aiohttp.ClientSession()
             self._session_created = True
 
         if self._session.closed:
             raise SessionNotFound("The WorldstateClient's session is closed.")
 
         language = language or self._default_lang
 
         url = build_endpoint(endpoint, language)
 
-        if self._debug:
-            print(f"[WorldstateClient DEBUG] Sending request to {url}...")
+        self._logger.debug(f"Sending request to {url}...")
 
         async with self._session.get(url) as response:
             response_text = await response.text()
 
             if response.status != 200:
                 raise WorldstateAPIError(
                     msgspec.json.decode(response_text, type=ErrorMessage)
                 )
 
-            if self._debug:
-                print(f"[WorldstateClient DEBUG] Got request:\n{response_text}")
+            self._logger.debug(f"Got request:\n{response_text}")
 
             return response_text
 
     #
     # Queries
     #
 
     async def query(
         self, cls: Type[SupportsSingleQuery], language: Optional[Language] = None
     ) -> SupportsSingleQuery:
-        """Queries the model of type `SingleQueryModel` to return its corresponding object.
-
-        Args:
-            cls (Type[SupportsSingleQuery]): The model to query.
-            language (Optional[Language], optional): The language to return the object in. Defaults to None.
-
-        Raises:
-            UnsupportedSingleQueryError: When the passed type `cls` is not a subclass of `SingleQueryModel`.
+        """
+        Queries the model of type `SingleQueryModel` to return its corresponding object.
 
-        Returns:
-            SupportsSingleQuery: The queried model.
+        Parameters
+        ----------
+        cls : Type[SupportsSingleQuery]
+            The model to query.
+        language : Optional[Language], optional
+            The language to return the object in, by default None.
+
+        Raises
+        ------
+        UnsupportedSingleQueryError
+            When the passed type `cls` is not a subclass of `SingleQueryModel`.
+
+        Returns
+        -------
+        SupportsSingleQuery
+            The queried model.
         """
+
         if not issubclass(cls, SingleQueryModel):
             raise TypeError(
                 f"{cls.__name__} is required to be of type SingleQueryModel."
             )
         json = await self._request(cls.__endpoint__, language)
 
         return cls._from_json(json)
 
     async def query_list_of(
         self, cls: Type[SupportsMultiQuery], language: Optional[Language] = None
     ) -> List[SupportsMultiQuery]:
-        """Queries the model of type `MultiQueryModel` to return its corresponding object.
-
-        Args:
-            cls (Type[SupportsSingleQuery]): The model to query.
-            language (Optional[Language], optional): The language to return the object in. Defaults to None.
-
-        Raises:
-            UnsupportedSingleQueryError: When the passed type `cls` is not a subclass of `SingleQueryModel`.
+        """
+        Queries the model of type `MultiQueryModel` to return its corresponding object.
 
-        Returns:
-            Optional[List[SupportsMultiQuery]]: A list of the queried model.
+        Parameters
+        ----------
+        cls : Type[SupportsSingleQuery]
+            The model to query.
+        language : Optional[Language], optional
+            The language to return the object in, by default None.
+
+        Raises
+        ------
+        UnsupportedSingleQueryError
+            When the passed type `cls` is not a subclass of `SingleQueryModel`.
+
+        Returns
+        -------
+        Optional[List[SupportsMultiQuery]]
+            A list of the queried model.
         """
+
         if not issubclass(cls, MultiQueryModel):
             raise TypeError(
                 f"{cls.__name__} is required to be of type MultiQueryModel."
             )
         json = await self._request(cls.__endpoint__, language)
 
         return cls._from_json(json)
@@ -239,48 +287,44 @@
             raise TypeError(
                 f"{type.__name__} has to implement SingleQueryModel and TimedEvent"
             )
 
         def decorator(func: Callable[..., Coroutine[Any, Any, None]]) -> _TaskHelper:
             @wraps(func)
             async def inner() -> None:
-                item: Optional[TimedEvent] = None  # type: ignore
+                item: _SingleQueryTimedEvent = await self.query(type)  # type: ignore
                 while True:
                     try:
-                        # first cycle
-                        if item is None:
-                            item: TimedEvent = await self.query(type)  # type: ignore
-
                         # check if the event is over, if so, retry in 1 minute (API doesn't refresh at the exact point of expiry)
                         if item.expiry <= datetime.now(tz=timezone.utc):
-                            if self._debug:
-                                print(
-                                    f"[WorldstateClient DEBUG : listener : {type}] Retry started. Looking for state change from the API"
-                                )
+                            self._logger.listener_debug(
+                                "Retry started. Looking for state change from the API",
+                                type,
+                            )
 
                             await asyncio.sleep(60)
 
-                            new_item: TimedEvent = await self.query(type)  # type: ignore
+                            new_item: _SingleQueryTimedEvent = await self.query(type)  # type: ignore
 
                             if item.expiry < new_item.expiry:
                                 # we now know that it is a different event, so we can call the callback function
                                 # with the new item after the last one's expiry
                                 await func(new_item)
 
                                 # we called the function, so we need to update the "last used item"
                                 item = new_item
 
                         # calculate seconds until next event triggers
                         seconds_to_wait = (
                             item.expiry - datetime.now(tz=timezone.utc)
                         ).total_seconds()
 
-                        if self._debug:
-                            print(
-                                f"[WorldstateClient DEBUG : listener : {type}] Sleeping {seconds_to_wait} seconds"
+                        if seconds_to_wait > 0:
+                            self._logger.listener_debug(
+                                f"Sleeping {seconds_to_wait} seconds", type
                             )
                         await asyncio.sleep(
                             seconds_to_wait
                             + 1  # to avoid slight offsets resulting in this part being called a ton of times
                         )
 
                     except asyncio.CancelledError:
```

### Comparing `warframe.py-0.5.0/warframe/worldstate/common/core.py` & `warframe.py-0.6.0/warframe/worldstate/common/core.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 from datetime import datetime, timezone
 from typing import Any, ClassVar, List, Type, TypeVar
 
 import msgspec
 
-__all__ = [
-    "MultiQueryModel",
-    "SingleQueryModel",
-    "WorldstateObject",
-    "TimedEvent",
-]
+__all__ = ["MultiQueryModel", "SingleQueryModel", "WorldstateObject", "TimedEvent"]
 
 
 def _decode_hook(type: Type, obj: Any) -> Any:
     if isinstance(type, datetime) and isinstance(obj, str):
         return datetime.fromisoformat(obj.strip("Z"))
 
     return obj
 
 
 def _get_short_format_time_string(dt: datetime) -> str:
-    """Returns a short time formatted string based on the now and the dt.
-
-    Args:
-        dt (datetime): The time the Event XYZ started/ends
+    """
+    Returns a short time formatted string based on the current time and the specified datetime.
 
-    Returns:
-        str: The short time formatted string of the time in between now and when the dt.
+    Parameters
+    ----------
+    dt : datetime
+        The time the event started/ended.
+
+    Returns
+    -------
+    str
+        The short time formatted string representing the time difference between now and the specified datetime.
     """
+
     now = datetime.now(tz=timezone.utc)
     time_in_between = now - dt if now > dt else dt - now
 
     days = time_in_between.days
     hours, remainder = divmod(time_in_between.seconds, 3600)
     minutes, seconds = divmod(remainder, 60)
 
@@ -86,38 +87,52 @@
     Base class for giving models an indicator whether they can only come from a JSON array.
     """
 
     __endpoint__: ClassVar[str]
 
     @classmethod
     def _from_json(cls: Type[T], response: str) -> List[T]:
-        """Decodes a JSON string to an list of object of T.
-
-        Args:
-            cls (Type[T]): The type T.
-            response (str): The raw JSON as string.
+        """
+        Decodes a JSON string to a list of objects of type T.
 
-        Returns:
-            List[T]: A list of objects of T.
+        Parameters
+        ----------
+        cls : Type[T]
+            The type T.
+        response : str
+            The raw JSON as a string.
+
+        Returns
+        -------
+        List[T]
+            A list of objects of type T.
         """
+
         return msgspec.json.decode(response, type=List[cls], dec_hook=_decode_hook)
 
 
 class SingleQueryModel(WorldstateObject):
     """
     Base class for giving models an indicator whether they can only come from a single JSON object.
     """
 
     __endpoint__: ClassVar[str]
 
     @classmethod
     def _from_json(cls: Type[T], response: str) -> T:
-        """Decodes a JSON string to an object of T.
-
-        Args:
-            cls (Type[T]): The type T.
-            response (str): The raw JSON as string.
+        """
+        Decodes a JSON string to an object of type T.
 
-        Returns:
-            T: The object of T
+        Parameters
+        ----------
+        cls : Type[T]
+            The type T.
+        response : str
+            The raw JSON as a string.
+
+        Returns
+        -------
+        T
+            The object of type T.
         """
+
         return msgspec.json.decode(response, type=cls, dec_hook=_decode_hook)
```

### Comparing `warframe.py-0.5.0/warframe/worldstate/common/logger.py` & `warframe.py-0.6.0/warframe/worldstate/common/logger.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,28 +1,25 @@
+from __future__ import annotations
+
 from logging import Logger
-from typing import TYPE_CHECKING, Union
+from typing import TYPE_CHECKING, Type, Union
 
 if TYPE_CHECKING:
-    # as soon as state listeners are merged
-    # from ..client import _SingleQueryTimedEvent
-    pass
+    from ..client import _SingleQueryTimedEvent
+
 
 __all__ = ["WorldstateLogger"]
 
 
 class WorldstateLogger(Logger):
     def __init__(self, name: str, level: Union[str, int] = 0) -> None:
         super().__init__(name, level)
 
     def debug(self, msg: object, *args: object) -> None:
         return super().debug(f"[WorldstateClient DEBUG] {msg}", *args)
 
-    # def listener_debug(
-    #         self,
-    #         msg: object,
-    #         *args: object,
-    #         listener_cls: Type[_SingleQueryTimedEvent]
-    # ) -> None:
-    #     return super().debug(
-    #         f"[WorldstateClient DEBUG : listener : {listener_cls}] {msg}",
-    #         *args
-    #     )
+    def listener_debug(
+        self, msg: object, listener_cls: Type[_SingleQueryTimedEvent], *args: object
+    ) -> None:
+        return super().debug(
+            f"[WorldstateClient DEBUG : listener : {listener_cls}] {msg}", *args
+        )
```

### Comparing `warframe.py-0.5.0/warframe/worldstate/common/types_.py` & `warframe.py-0.6.0/warframe/worldstate/common/types_.py`

 * *Files identical despite different names*

### Comparing `warframe.py-0.5.0/warframe/worldstate/endpoints.py` & `warframe.py-0.6.0/warframe/worldstate/endpoints.py`

 * *Files 7% similar despite different names*

```diff
@@ -30,17 +30,24 @@
     Riven = "/rivens"
     SentientOutpost = "/sentientOutposts"
     Sanctuary = "/simaris"
     SyndicateMission = "/syndicateMissions"
 
 
 def build_endpoint(endpoint: str, language: Language = Language.EN) -> str:
-    """Returns an URL based on the endpoint and language
+    """
+    Returns an URL based on the endpoint and language.
 
-    Args:
-        endpoint (str): The endpoint of the request.
-        language (Language, optional): The language the API should respond in. Defaults to Language.EN.
+    Parameters
+    ----------
+    endpoint : str
+        The endpoint of the request.
+    language : Language, optional
+        The language the API should respond in, by default Language.EN.
 
-    Returns:
-        str: The built URL.
+    Returns
+    -------
+    str
+        The built URL.
     """
+
     return f"{BASE_URL}{endpoint}/?language={language.value}"
```

### Comparing `warframe.py-0.5.0/warframe/worldstate/enums/mission_type.py` & `warframe.py-0.6.0/warframe/worldstate/enums/mission_type.py`

 * *Files identical despite different names*

### Comparing `warframe.py-0.5.0/warframe/worldstate/exceptions.py` & `warframe.py-0.6.0/warframe/worldstate/exceptions.py`

 * *Files identical despite different names*

### Comparing `warframe.py-0.5.0/warframe/worldstate/models/arbitration.py` & `warframe.py-0.6.0/warframe/worldstate/models/arbitration.py`

 * *Files identical despite different names*

### Comparing `warframe.py-0.5.0/warframe/worldstate/models/archon_hunt.py` & `warframe.py-0.6.0/warframe/worldstate/models/archon_hunt.py`

 * *Files identical despite different names*

### Comparing `warframe.py-0.5.0/warframe/worldstate/models/daily_deal.py` & `warframe.py-0.6.0/warframe/worldstate/models/daily_deal.py`

 * *Files identical despite different names*

### Comparing `warframe.py-0.5.0/warframe/worldstate/models/event.py` & `warframe.py-0.6.0/warframe/worldstate/models/event.py`

 * *Files identical despite different names*

### Comparing `warframe.py-0.5.0/warframe/worldstate/models/fissure.py` & `warframe.py-0.6.0/warframe/worldstate/models/fissure.py`

 * *Files identical despite different names*

### Comparing `warframe.py-0.5.0/warframe/worldstate/models/flash_sale.py` & `warframe.py-0.6.0/warframe/worldstate/models/flash_sale.py`

 * *Files identical despite different names*

### Comparing `warframe.py-0.5.0/warframe/worldstate/models/invasion.py` & `warframe.py-0.6.0/warframe/worldstate/models/invasion.py`

 * *Files identical despite different names*

### Comparing `warframe.py-0.5.0/warframe/worldstate/models/mission.py` & `warframe.py-0.6.0/warframe/worldstate/models/mission.py`

 * *Files identical despite different names*

### Comparing `warframe.py-0.5.0/warframe/worldstate/models/reward.py` & `warframe.py-0.6.0/warframe/worldstate/models/reward.py`

 * *Files identical despite different names*

### Comparing `warframe.py-0.5.0/warframe/worldstate/models/sortie.py` & `warframe.py-0.6.0/warframe/worldstate/models/sortie.py`

 * *Files identical despite different names*

### Comparing `warframe.py-0.5.0/warframe/worldstate/models/void_trader.py` & `warframe.py-0.6.0/warframe/worldstate/models/void_trader.py`

 * *Files identical despite different names*

### Comparing `warframe.py-0.5.0/warframe.py.egg-info/PKG-INFO` & `warframe.py-0.6.0/warframe.py.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: warframe.py
-Version: 0.5.0
+Version: 0.6.0
 Summary: An asynchronous Python API wrapper for the Warframestat API and (later) the warframe.market API.
 Home-page: https://github.com/WFCD/warframe.py
 Author: Mettwasser
 License: MIT
 Keywords: Warframe API worldstate market wrapper
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
@@ -34,29 +34,48 @@
 This library is in its early states. The goal is to make it the best and most up-to-date Python Warframe API wrapper.
 
 Quickstart
 ----------
 
 .. code-block:: python
 
+    # queries are just another way to get the data to the corresponding objects.
+    # this is really just personal preference.
+
     import asyncio
+    import logging
 
-    from warframe.worldstate import Language, WorldstateClient
+    from warframe.worldstate import WorldstateClient, WorldstateLogger
+    
+    # import the models you want to use
+    from warframe.worldstate.models import Cetus
 
 
     async def main():
-        async with WorldstateClient() as client:
-            cetus = await client.get_cetus(language=Language.English)  # english is default
-            print(cetus.short_string)
+        # Note that the default logger is pretty much empty (nothing will be logged)
+        # so if you want to make use of the logger, make your own:
+        logger = WorldstateLogger("name whatever you want", logging.DEBUG)
+        logger.addHandler(logging.StreamHandler())
+
+        async with WorldstateClient(logger=logger) as client:  # pass the logger
+            cetus = await client.get_cetus()
+            # or ...
+
+            # just throw the model into `query(type)`
+            # note that for stuff like fissures you need `query_list_of(type)`
+            cetus = await client.query(Cetus)
+
+            print(cetus)
 
 
     if __name__ == "__main__":
         loop = asyncio.new_event_loop()
         loop.run_until_complete(main())
 
+
 Installing
 ----------
 
 To install the library, use the following command:
 
 .. code-block:: bash
```

### Comparing `warframe.py-0.5.0/warframe.py.egg-info/SOURCES.txt` & `warframe.py-0.6.0/warframe.py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

