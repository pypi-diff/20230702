# Comparing `tmp/py_tfl-0.4.4.tar.gz` & `tmp/py_tfl-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_tfl-0.4.4.tar", max compression
+gzip compressed data, was "py_tfl-0.5.0.tar", max compression
```

## Comparing `py_tfl-0.4.4.tar` & `py_tfl-0.5.0.tar`

### file list

```diff
@@ -1,19 +1,23 @@
--rw-r--r--   0        0        0     1068 2023-07-02 11:35:36.999147 py_tfl-0.4.4/LICENSE
--rw-r--r--   0        0        0     4414 2023-07-02 11:35:36.999147 py_tfl-0.4.4/README.md
--rw-r--r--   0        0        0     2347 2023-07-02 11:35:37.003147 py_tfl-0.4.4/pyproject.toml
--rw-r--r--   0        0        0      128 2023-07-02 11:35:37.003147 py_tfl-0.4.4/tfl/__init__.py
--rw-r--r--   0        0        0       68 2023-07-02 11:35:37.003147 py_tfl-0.4.4/tfl/cli/__init__.py
--rw-r--r--   0        0        0     1345 2023-07-02 11:35:37.003147 py_tfl-0.4.4/tfl/cli/_async_typer.py
--rw-r--r--   0        0        0     3578 2023-07-02 11:35:37.003147 py_tfl-0.4.4/tfl/cli/main.py
--rw-r--r--   0        0        0        0 2023-07-02 11:35:37.003147 py_tfl-0.4.4/tfl/cli/py.typed
--rw-r--r--   0        0        0      415 2023-07-02 11:35:37.003147 py_tfl-0.4.4/tfl/clients/__init__.py
--rw-r--r--   0        0        0     4650 2023-07-02 11:35:37.003147 py_tfl-0.4.4/tfl/clients/_accident_stats_client.py
--rw-r--r--   0        0        0     4484 2023-07-02 11:35:37.003147 py_tfl-0.4.4/tfl/clients/_air_quality_client.py
--rw-r--r--   0        0        0     1696 2023-07-02 11:35:37.003147 py_tfl-0.4.4/tfl/clients/_auth.py
--rw-r--r--   0        0        0     5000 2023-07-02 11:35:37.003147 py_tfl-0.4.4/tfl/clients/_client.py
--rw-r--r--   0        0        0     4913 2023-07-02 11:35:37.003147 py_tfl-0.4.4/tfl/clients/_crowding_client.py
--rw-r--r--   0        0        0     4463 2023-07-02 11:35:37.003147 py_tfl-0.4.4/tfl/clients/_lift_disruptions_client.py
--rw-r--r--   0        0        0        0 2023-07-02 11:35:37.003147 py_tfl-0.4.4/tfl/clients/py.typed
--rw-r--r--   0        0        0      561 2023-07-02 11:35:37.003147 py_tfl-0.4.4/tfl/enums.py
--rw-r--r--   0        0        0        0 2023-07-02 11:35:37.003147 py_tfl-0.4.4/tfl/py.typed
--rw-r--r--   0        0        0     5386 1970-01-01 00:00:00.000000 py_tfl-0.4.4/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-07-02 18:27:08.074074 py_tfl-0.5.0/LICENSE
+-rw-r--r--   0        0        0     4480 2023-07-02 18:27:08.074074 py_tfl-0.5.0/README.md
+-rw-r--r--   0        0        0     2347 2023-07-02 18:27:08.078074 py_tfl-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0      128 2023-07-02 18:27:08.078074 py_tfl-0.5.0/tfl/__init__.py
+-rw-r--r--   0        0        0       70 2023-07-02 18:27:08.078074 py_tfl-0.5.0/tfl/base/__init__.py
+-rw-r--r--   0        0        0      574 2023-07-02 18:27:08.078074 py_tfl-0.5.0/tfl/base/_base_handler.py
+-rw-r--r--   0        0        0       67 2023-07-02 18:27:08.078074 py_tfl-0.5.0/tfl/cli/__init__.py
+-rw-r--r--   0        0        0     1345 2023-07-02 18:27:08.078074 py_tfl-0.5.0/tfl/cli/_async_typer.py
+-rw-r--r--   0        0        0     4311 2023-07-02 18:27:08.078074 py_tfl-0.5.0/tfl/cli/main.py
+-rw-r--r--   0        0        0        0 2023-07-02 18:27:08.078074 py_tfl-0.5.0/tfl/cli/py.typed
+-rw-r--r--   0        0        0      104 2023-07-02 18:27:08.078074 py_tfl-0.5.0/tfl/clients/__init__.py
+-rw-r--r--   0        0        0     1696 2023-07-02 18:27:08.078074 py_tfl-0.5.0/tfl/clients/_auth.py
+-rw-r--r--   0        0        0     5564 2023-07-02 18:27:08.078074 py_tfl-0.5.0/tfl/clients/_client.py
+-rw-r--r--   0        0        0       98 2023-07-02 18:27:08.078074 py_tfl-0.5.0/tfl/clients/handlers/__init__.py
+-rw-r--r--   0        0        0      992 2023-07-02 18:27:08.078074 py_tfl-0.5.0/tfl/clients/handlers/_accident_stats_handler.py
+-rw-r--r--   0        0        0      835 2023-07-02 18:27:08.078074 py_tfl-0.5.0/tfl/clients/handlers/_air_quality_handler.py
+-rw-r--r--   0        0        0      987 2023-07-02 18:27:08.078074 py_tfl-0.5.0/tfl/clients/handlers/_client_handlers.py
+-rw-r--r--   0        0        0     1268 2023-07-02 18:27:08.078074 py_tfl-0.5.0/tfl/clients/handlers/_crowding_handler.py
+-rw-r--r--   0        0        0      891 2023-07-02 18:27:08.078074 py_tfl-0.5.0/tfl/clients/handlers/_lift_disruptions_handler.py
+-rw-r--r--   0        0        0        0 2023-07-02 18:27:08.078074 py_tfl-0.5.0/tfl/clients/py.typed
+-rw-r--r--   0        0        0      561 2023-07-02 18:27:08.078074 py_tfl-0.5.0/tfl/enums.py
+-rw-r--r--   0        0        0        0 2023-07-02 18:27:08.078074 py_tfl-0.5.0/tfl/py.typed
+-rw-r--r--   0        0        0     5452 1970-01-01 00:00:00.000000 py_tfl-0.5.0/PKG-INFO
```

### Comparing `py_tfl-0.4.4/LICENSE` & `py_tfl-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `py_tfl-0.4.4/README.md` & `py_tfl-0.5.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -54,16 +54,16 @@
 authentication and rate limiting for you. The client is built on top of [HTTPX](https://www.python-httpx.org/), which
 provides a fast, async HTTP client.
 
 ```python
 from tfl import clients
 
 
-async with clients.LiftDisruptionsV2Client() as client:
-    response = await client.get_lift_disruptions()
+async with clients.TFLClient(auth=clients.Auth(key="<your-tfl-api-key>")) as client:
+    response = await client.handlers.lift_disruptions_v2_handler.get_lift_disruptions()
 
 print(response.json())
 ```
 
 ## 📈 Releases
 
 You can see the list of available releases on the [GitHub Releases](https://github.com/Ce11an/tfl/releases)
```

### Comparing `py_tfl-0.4.4/pyproject.toml` & `py_tfl-0.5.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "py-tfl"
-version = "0.4.4"
+version = "0.5.0"
 description = "A Python package for the Transport for London (TFL) API."
 authors = ["Cellan Hall <hallcellan@gmail.com>"]
 readme = "README.md"
 packages = [
     {include = "tfl"},
 ]
 homepage = "https://ce11an.github.io/tfl/"
```

### Comparing `py_tfl-0.4.4/tfl/cli/_async_typer.py` & `py_tfl-0.5.0/tfl/cli/_async_typer.py`

 * *Files identical despite different names*

### Comparing `py_tfl-0.4.4/tfl/cli/main.py` & `py_tfl-0.5.0/tfl/cli/main.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Main module for the tfl CLI."""
+
 from typing import Any, Dict, Optional, Tuple
 
 import rich
 import typer
 from rich.console import Console
 from rich.table import Table
 from typing_extensions import Annotated
@@ -29,16 +30,16 @@
     """Get current lift disruptions."""
 
     def _create_table_row(resp_json: Dict[str, Any]) -> Tuple[str, str]:
         """Create a table row from a disruption."""
         split_message = resp_json["message"].split(":")
         return split_message[0], split_message[1].replace(" No Step Free Access - ", "")
 
-    async with clients.LiftDisruptionsV2Client(auth=tfl.clients.Auth(key=key) if key else None) as client:
-        response = await client.get_lift_disruptions()
+    async with clients.TFLClient(auth=tfl.clients.Auth(key=key) if key else None) as client:
+        response = await client.handlers.lift_disruptions_v2_handler.get_lift_disruptions()
     table = Table(
         "Station",
         "Message",
         title="Lift Disruptions",
         caption="Current TFL lift disruptions.",
         expand=True,
         padding=(1, 1),
@@ -51,16 +52,16 @@
 
 @app.async_command()
 async def accident_stats(
     year: Annotated[int, typer.Argument(help="The year to get accident stats for.")],
     key: Annotated[Optional[str], typer.Argument(envvar="TFL_API_KEY", help="TFL API key.")] = None,
 ) -> None:
     """Gets all accident details for accidents occurring in the specified year."""
-    async with clients.AccidentStatsClient(auth=tfl.clients.Auth(key=key) if key else None) as client:
-        response = await client.get_accident_stats(year=year)
+    async with clients.TFLClient(auth=tfl.clients.Auth(key=key) if key else None) as client:
+        response = await client.handlers.accident_stats_handler.get_accident_stats(year=year)
     rich.print(response.json())
     raise typer.Exit()
 
 
 @app.async_command()
 async def crowding(
     naptan_code: Annotated[str, typer.Argument(help="The NAPTAN code of the station to get crowding for.")],
@@ -71,28 +72,46 @@
             "'Sun', 'Live'."
         ),
     ] = None,
     key: Annotated[Optional[str], typer.Argument(envvar="TFL_API_KEY", help="TFL API key.")] = None,
 ) -> None:
     """Information about crowding levels within TFL stations."""
     day = tfl.enums.DayOfWeekEnum(day) if day else None
-    async with clients.CrowdingClient(auth=tfl.clients.Auth(key=key) if key else None) as client:
-        response = await client.get_crowding(naptan_code=naptan_code, day=day)
+    async with clients.TFLClient(auth=tfl.clients.Auth(key=key) if key else None) as client:
+        response = await client.handlers.crowding_handler.get_crowding(naptan_code=naptan_code, day=day)
     rich.print(response.json())
     raise typer.Exit()
 
 
 @app.async_command()
 async def air_quality(
     key: Annotated[Optional[str], typer.Argument(envvar="TFL_API_KEY", help="TFL API key.")] = None,
 ) -> None:
     """Get air quality data feed."""
-    async with clients.AirQualityClient(auth=tfl.clients.Auth(key=key) if key else None) as client:
-        response = await client.get_air_quality()
-    rich.print(response.json())
+
+    def _create_table_row(resp_json: Dict[str, Any]) -> Tuple[str, str]:
+        """Create a table row from a air quality response."""
+        current_forecast = resp_json["currentForecast"][0]
+        return current_forecast["forecastBand"], current_forecast["forecastSummary"]
+
+    async with clients.TFLClient(auth=tfl.clients.Auth(key=key) if key else None) as client:
+        response = await client.handlers.air_quality_handler.get_air_quality()
+
+    data = response.json()
+    table = Table(
+        "Air Pollution Banding",
+        "Summary",
+        title="Today's Air Quality",
+        caption=f"{data['disclaimerText']} \n\nFor more information, please visit: {data['forecastURL']}",
+        expand=True,
+        padding=(1, 1),
+        caption_justify="left",
+    )
+    table.add_row(*_create_table_row(data))
+    console.print(table)
     raise typer.Exit()
 
 
 # noinspection PyUnusedLocal
 @app.callback()
 def main(
     version: Annotated[
```

### Comparing `py_tfl-0.4.4/tfl/clients/_accident_stats_client.py` & `py_tfl-0.5.0/tfl/clients/_client.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,34 @@
-"""Client to interact with the accident stats API."""
+"""A client to interact with the TFL API.
+
+The `TFLClient` class is a subclass of [httpx.AsyncClient](https://www.python-httpx.org/api/#asyncclient) that is used
+to interact with the TFL API. Using the `TFLClient` class, you can send requests to the TFL API.
+
+The `TFLClient` allows for the `Auth` class to be passed in as an argument. This will add the API key to the request
+URL as a query parameter. If no `Auth` class is passed in, the request will be sent without an API key. This will
+result in a rate limit of 50 requests per hour.
+
+Also, the `base_url` is set to the TFL API base URL. This means that when a request is sent, the URL will be appended
+to the base URL. For example, if the `base_url` is set to `https://api.tfl.gov.uk/`, and the request URL is set to
+`Disruptions/Lifts/v2`, the request URL will be `https://api.tfl.gov.uk/Disruptions/Lifts/v2`.
+
+Using the `TFLClient`, you can access all of TFL API through handlers. For example, to access the Lift Disruptions
+V2 API, you can use the `LiftDisruptionsV2Handler`:
+
+```python
+from tfl import clients
+
+async with clients.TFLClient() as client:
+    response = await client.handlers.lift_disruptions_v2_handler.get_lift_disruptions()
+
+print(response.json())
+```
+
+Check out [Handlers](handlers) for more information on the available handlers.
+"""
 
 from typing import Any, Callable, List, Mapping, Optional, Union
 
 import httpx
 from httpx import AsyncBaseTransport
 
 # noinspection PyProtectedMember
@@ -15,25 +41,22 @@
     HeaderTypes,
     ProxiesTypes,
     QueryParamTypes,
     TimeoutTypes,
     VerifyTypes,
 )
 
-from tfl.clients import Auth, TFLClient
-
-__all__ = ["AccidentStatsClient"]
-
+from tfl.clients import Auth
+from tfl.clients.handlers import TFLHandlers
 
-class AccidentStatsClient(TFLClient):
-    """Client to interact with the accident stats API.
+__all__ = ["TFLClient"]
 
-    [API reference](https://api-portal.tfl.gov.uk/api-details#api=AccidentStats&operation=AccidentStats_Get)
 
-    As it stands, the API does not include data between 2020 and 2023.
+class TFLClient(httpx.AsyncClient):
+    """Client to interact with the TFL API.
 
     Args:
         auth: TFL authentication class to use when sending requests.
         params: Query parameters to include in request URLs, as a string, dictionary, or sequence of two-tuples.
         headers: Dictionary of HTTP headers to include when sending requests.
         cookies: Dictionary of Cookie items to include when sending requests.
         verify: SSL certificates (a.k.a CA bundle) used to verify the identity of requested hosts. Either `True`
@@ -53,17 +76,16 @@
             in a response Content-Type header. Set to a callable for automatic character set detection. Default:
             "utf-8".
 
     Example:
         ```python
         from tfl.clients import Auth
 
-
-        async with AccidentStatsClient(auth=Auth(key="<your-tfl-api-key>")) as client:
-            response = await client.get_accident_stats(year=2019)
+        async with TFLClient(auth=Auth(key="<your-tfl-api-key>")) as client:
+            response = await client.handlers.lift_disruptions_v2_handler.get_lift_disruptions()
 
         print(response.json())
         ```
     """
 
     def __init__(
         self,
@@ -93,27 +115,21 @@
             params=params,
             headers=headers,
             cookies=cookies,
             timeout=timeout,
             follow_redirects=follow_redirects,
             max_redirects=max_redirects,
             event_hooks=event_hooks,
+            base_url="https://api.tfl.gov.uk",
             trust_env=trust_env,
             default_encoding=default_encoding,
             verify=verify,
             cert=cert,
             http1=http1,
             http2=http2,
             proxies=proxies,
             mounts=mounts,
             limits=limits,
             transport=transport,
             app=app,
         )
-
-    async def get_accident_stats(self, year: int) -> httpx.Response:
-        """Gets all accident details for accidents occurring in the specified year.
-
-        Returns:
-            The response from the API.
-        """
-        return await self.get(url=f"/AccidentStats/{year}")
+        self.handlers = TFLHandlers(self)
```

### Comparing `py_tfl-0.4.4/tfl/clients/_auth.py` & `py_tfl-0.5.0/tfl/clients/_auth.py`

 * *Files identical despite different names*

### Comparing `py_tfl-0.4.4/tfl/enums.py` & `py_tfl-0.5.0/tfl/enums.py`

 * *Files identical despite different names*

### Comparing `py_tfl-0.4.4/PKG-INFO` & `py_tfl-0.5.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-tfl
-Version: 0.4.4
+Version: 0.5.0
 Summary: A Python package for the Transport for London (TFL) API.
 Home-page: https://ce11an.github.io/tfl/
 Author: Cellan Hall
 Author-email: hallcellan@gmail.com
 Requires-Python: >=3.8,<3.12
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -78,16 +78,16 @@
 authentication and rate limiting for you. The client is built on top of [HTTPX](https://www.python-httpx.org/), which
 provides a fast, async HTTP client.
 
 ```python
 from tfl import clients
 
 
-async with clients.LiftDisruptionsV2Client() as client:
-    response = await client.get_lift_disruptions()
+async with clients.TFLClient(auth=clients.Auth(key="<your-tfl-api-key>")) as client:
+    response = await client.handlers.lift_disruptions_v2_handler.get_lift_disruptions()
 
 print(response.json())
 ```
 
 ## 📈 Releases
 
 You can see the list of available releases on the [GitHub Releases](https://github.com/Ce11an/tfl/releases)
```

