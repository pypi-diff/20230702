# Comparing `tmp/lambda_handler-1.2.1.tar.gz` & `tmp/lambda_handler-2.0.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lambda_handler-1.2.1.tar", max compression
+gzip compressed data, was "lambda_handler-2.0.0a1.tar", max compression
```

## Comparing `lambda_handler-1.2.1.tar` & `lambda_handler-2.0.0a1.tar`

### file list

```diff
@@ -1,16 +1,17 @@
--rw-r--r--   0        0        0    11357 2022-11-09 08:54:28.803833 lambda_handler-1.2.1/LICENSE
--rw-r--r--   0        0        0     4647 2023-07-01 19:01:26.885296 lambda_handler-1.2.1/README.md
--rw-r--r--   0        0        0      369 2023-07-01 19:41:25.684954 lambda_handler-1.2.1/lambda_handler/__init__.py
--rw-r--r--   0        0        0     2820 2022-11-09 09:08:20.229164 lambda_handler-1.2.1/lambda_handler/dependencies.py
--rw-r--r--   0        0        0    13929 2022-11-09 09:56:48.497145 lambda_handler-1.2.1/lambda_handler/handler.py
--rw-r--r--   0        0        0      560 2022-11-09 09:08:20.233470 lambda_handler-1.2.1/lambda_handler/model/__init__.py
--rw-r--r--   0        0        0     5927 2022-11-09 09:08:20.236865 lambda_handler-1.2.1/lambda_handler/model/base.py
--rw-r--r--   0        0        0     2134 2022-11-09 09:08:20.231006 lambda_handler-1.2.1/lambda_handler/model/direct_invocation.py
--rw-r--r--   0        0        0     3206 2022-11-09 09:08:20.234983 lambda_handler-1.2.1/lambda_handler/model/event_bridge.py
--rw-r--r--   0        0        0     3511 2023-07-01 19:40:46.187213 lambda_handler-1.2.1/lambda_handler/model/sns.py
--rw-r--r--   0        0        0     4394 2022-11-09 09:57:24.033450 lambda_handler-1.2.1/lambda_handler/model/sqs.py
--rw-r--r--   0        0        0        0 2022-11-09 09:59:06.433379 lambda_handler-1.2.1/lambda_handler/py.typed
--rw-r--r--   0        0        0     2624 2022-11-09 09:35:27.330005 lambda_handler-1.2.1/lambda_handler/types.py
--rw-r--r--   0        0        0     9375 2022-11-09 09:36:45.711163 lambda_handler-1.2.1/lambda_handler/utils.py
--rw-r--r--   0        0        0     1700 2023-07-01 19:41:25.685184 lambda_handler-1.2.1/pyproject.toml
--rw-r--r--   0        0        0     5438 1970-01-01 00:00:00.000000 lambda_handler-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2022-11-09 08:54:28.803833 lambda_handler-2.0.0a1/LICENSE
+-rw-r--r--   0        0        0     4647 2023-07-01 19:01:26.885296 lambda_handler-2.0.0a1/README.md
+-rw-r--r--   0        0        0      371 2023-07-02 08:11:43.754414 lambda_handler-2.0.0a1/lambda_handler/__init__.py
+-rw-r--r--   0        0        0     2820 2022-11-09 09:08:20.229164 lambda_handler-2.0.0a1/lambda_handler/dependencies.py
+-rw-r--r--   0        0        0    16074 2023-07-02 08:09:25.240089 lambda_handler-2.0.0a1/lambda_handler/handler.py
+-rw-r--r--   0        0        0      594 2023-07-02 08:06:36.734615 lambda_handler-2.0.0a1/lambda_handler/model/__init__.py
+-rw-r--r--   0        0        0     5927 2022-11-09 09:08:20.236865 lambda_handler-2.0.0a1/lambda_handler/model/base.py
+-rw-r--r--   0        0        0     2134 2022-11-09 09:08:20.231006 lambda_handler-2.0.0a1/lambda_handler/model/direct_invocation.py
+-rw-r--r--   0        0        0     3206 2022-11-09 09:08:20.234983 lambda_handler-2.0.0a1/lambda_handler/model/event_bridge.py
+-rw-r--r--   0        0        0     4833 2023-07-02 08:06:14.514853 lambda_handler-2.0.0a1/lambda_handler/model/s3.py
+-rw-r--r--   0        0        0     3511 2023-07-01 19:40:46.187213 lambda_handler-2.0.0a1/lambda_handler/model/sns.py
+-rw-r--r--   0        0        0     4394 2022-11-09 09:57:24.033450 lambda_handler-2.0.0a1/lambda_handler/model/sqs.py
+-rw-r--r--   0        0        0        0 2022-11-09 09:59:06.433379 lambda_handler-2.0.0a1/lambda_handler/py.typed
+-rw-r--r--   0        0        0     2624 2022-11-09 09:35:27.330005 lambda_handler-2.0.0a1/lambda_handler/types.py
+-rw-r--r--   0        0        0     9375 2022-11-09 09:36:45.711163 lambda_handler-2.0.0a1/lambda_handler/utils.py
+-rw-r--r--   0        0        0     1704 2023-07-02 08:11:43.754985 lambda_handler-2.0.0a1/pyproject.toml
+-rw-r--r--   0        0        0     5440 1970-01-01 00:00:00.000000 lambda_handler-2.0.0a1/PKG-INFO
```

### Comparing `lambda_handler-1.2.1/LICENSE` & `lambda_handler-2.0.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `lambda_handler-1.2.1/README.md` & `lambda_handler-2.0.0a1/README.md`

 * *Files identical despite different names*

### Comparing `lambda_handler-1.2.1/lambda_handler/dependencies.py` & `lambda_handler-2.0.0a1/lambda_handler/dependencies.py`

 * *Files identical despite different names*

### Comparing `lambda_handler-1.2.1/lambda_handler/handler.py` & `lambda_handler-2.0.0a1/lambda_handler/handler.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 """Defines the main `LambdaHandler` class"""
 
+import re
+
 from lambda_handler.model import (
     ApiGatewayEvent,
     AwsEvent,
     DataT,
     DirectInvocationEvent,
     EventBridgeEvent,
     LambdaResponse,
+    S3Event,
     SnsEvent,
     SqsEvent,
 )
 from lambda_handler.types import (
     AwsEventRawCallable,
     FastApiInterface,
     LambdaContext,
@@ -42,14 +45,15 @@
 _T = TypeVar("_T")
 _P = ParamSpec("_P")
 
 
 VALID_EVENTS = [
     "DirectInvocationEvent",
     "EventBridgeEvent",
+    "S3Event",
     "SqsEvent",
     "SnsEvent",
 ]
 
 
 class InvalidRouteError(Exception):
     """Raised when a route is not registered with the handler"""
@@ -95,18 +99,17 @@
     def handle_mytopic(event: SnsEvent) -> LambdaResponse:
         body = frobincate()
         return LambdaResponse(status_code=200, body=body)
     ```
     """
 
     def __init__(self, fastapi_app: Optional[FastApiInterface] = None):
-
-        self._events_dict: Dict[
-            Tuple[str, str], AwsEventRawCallable
-        ] = OnetimeDictionary()
+        self._events_dict: Dict[Tuple[str, str], AwsEventRawCallable] = (
+            OnetimeDictionary()
+        )
         self._fastapi_app: Optional[FastApiInterface] = None
         self._mangum: Optional[MangumInterface] = None
 
         if fastapi_app is not None:
             try:
                 #: pylint: disable=import-outside-toplevel
                 from fastapi import FastAPI
@@ -160,14 +163,47 @@
         Returns
         -------
         Optional[MangumInterface]
             Mangum app instance, if there is one
         """
         return self._mangum
 
+    def _find_function(
+        self, event_type_name: str, event_key: str
+    ) -> AwsEventRawCallable:
+        """Find the handling function for the given event type and key
+
+        Parameters
+        ----------
+        event_type_name : str
+            Name of the event class
+        event_key : str
+            Event key
+
+        Returns
+        -------
+        AwsEventRawCallable
+            Event handling function
+
+        Raises
+        ------
+        InvalidRouteError
+            If no handling function is found
+        """
+
+        for (event_type, key), func in self._events_dict.items():
+            if event_type == event_type_name:
+                if re.match(key, event_key):
+                    return func
+
+        raise InvalidRouteError(
+            f"No valid route for event type `{event_type_name}` and event key"
+            f" `{event_key}`"
+        )
+
     def process_event(
         self, event: Dict[str, Any], context: LambdaContext
     ) -> Dict[str, Any]:
         """Process an event into an `AwsEvent` instance and pass it to its
         handling function
 
         Parameters
@@ -186,24 +222,17 @@
         ------
         InvalidRouteError
             Raised when there is no valid route for the event
         """
         parsed_event = parse_lambda_event(event)
 
         if not isinstance(parsed_event, ApiGatewayEvent):
-
             event_type_name = type(parsed_event).__qualname__.split("[")[0]
 
-            func = self._events_dict.get((event_type_name, parsed_event.event_key))
-
-            if func is None:
-                raise InvalidRouteError(
-                    f"No valid route for event type `{event_type_name}` "
-                    f"and event key `{parsed_event.event_key}`"
-                )
+            func = self._find_function(event_type_name, parsed_event.event_key)
 
             # The function itself parses the event so we don't need to
             # pass the parsed event
 
             return func(event)
 
         if self.mangum is None:
@@ -384,14 +413,67 @@
             handler=self,
             event_type=EventBridgeEvent,
             event_key=resource_name,
             raw=raw,
         )
 
     @overload
+    def s3(
+        self, event_name: str, raw: Literal[False]
+    ) -> Callable[
+        [Callable[Concatenate[AwsEvent[S3Event], _P], LambdaResponse]],
+        AwsEventRawCallable,
+    ]:
+        ...
+
+    @overload
+    def s3(
+        self, event_name: str, raw: Literal[True]
+    ) -> Callable[
+        [Callable[Concatenate[Dict[str, Any], _P], Dict[str, Any]]],
+        AwsEventRawCallable,
+    ]:
+        ...
+
+    def s3(
+        self, event_name: str, raw: Bool = False
+    ) -> Union[
+        Callable[
+            [Callable[Concatenate[AwsEvent[S3Event], _P], LambdaResponse]],
+            AwsEventRawCallable,
+        ],
+        Callable[
+            [Callable[Concatenate[Dict[str, Any], _P], Dict[str, Any]]],
+            AwsEventRawCallable,
+        ],
+    ]:
+        """Handles S3 events
+
+        Parameters
+        ----------
+        event_name : str
+            Name of the S3 event, which may be a regular expression such as `ObjectCreated:.*`
+        raw : bool = `False`
+            Indicates that the wrapped function accepts and returns a Dict[str, Any]
+            instead of an `S3Event` and `LambdaResponse`
+
+        Returns
+        -------
+        AwsEventTypedCallable[S3Event]
+            A callable that handles an SqsEvent, or a Dict[str, Any]
+        """
+
+        return create_wrapper(
+            handler=self,
+            event_type=S3Event,
+            event_key=event_name,
+            raw=raw,
+        )
+
+    @overload
     def sns(
         self,
         topic_name: str,
         raw: Literal[False] = False,
     ) -> Callable[
         [Callable[Concatenate[SnsEvent[DataT], _P], LambdaResponse]],
         AwsEventRawCallable,
```

### Comparing `lambda_handler-1.2.1/lambda_handler/model/__init__.py` & `lambda_handler-2.0.0a1/lambda_handler/model/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     DataT,
     LambdaResponse,
     UnparseableResposeDictionary,
 )
 from .direct_invocation import DirectInvocationDetail  # noqa: F401
 from .direct_invocation import DirectInvocationEvent
 from .event_bridge import EventBridgeEvent, EventBridgeResource  # noqa: F401
+from .s3 import S3Event, S3Record
 from .sns import SnsEvent, SnsMessage, SnsMsgAttributeModel, SnsRecord  # noqa: F401
 from .sqs import (  # noqa: F401
     SqsEvent,
     SqsMesssageAttributes,
     SqsRecord,
     SqsRecordAttributes,
 )
```

### Comparing `lambda_handler-1.2.1/lambda_handler/model/base.py` & `lambda_handler-2.0.0a1/lambda_handler/model/base.py`

 * *Files identical despite different names*

### Comparing `lambda_handler-1.2.1/lambda_handler/model/direct_invocation.py` & `lambda_handler-2.0.0a1/lambda_handler/model/direct_invocation.py`

 * *Files identical despite different names*

### Comparing `lambda_handler-1.2.1/lambda_handler/model/event_bridge.py` & `lambda_handler-2.0.0a1/lambda_handler/model/event_bridge.py`

 * *Files identical despite different names*

### Comparing `lambda_handler-1.2.1/lambda_handler/model/sns.py` & `lambda_handler-2.0.0a1/lambda_handler/model/sns.py`

 * *Files identical despite different names*

### Comparing `lambda_handler-1.2.1/lambda_handler/model/sqs.py` & `lambda_handler-2.0.0a1/lambda_handler/model/sqs.py`

 * *Files identical despite different names*

### Comparing `lambda_handler-1.2.1/lambda_handler/types.py` & `lambda_handler-2.0.0a1/lambda_handler/types.py`

 * *Files identical despite different names*

### Comparing `lambda_handler-1.2.1/lambda_handler/utils.py` & `lambda_handler-2.0.0a1/lambda_handler/utils.py`

 * *Files identical despite different names*

### Comparing `lambda_handler-1.2.1/pyproject.toml` & `lambda_handler-2.0.0a1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lambda-handler"
-version = "1.2.1"
+version = "2.0.0a1"
 description = "A Python package for routing and validating AWS events inside a Lambda function"
 authors = ["Matthew Badger <matt@branchenergy.com>"]
 homepage = "https://github.com/branchenergy/lambda-handler"
 repository = "https://github.com/branchenergy/lambda-handler"
 license = "Apache 2.0"
 packages = [
   {include = "lambda_handler"},
@@ -47,9 +47,9 @@
     "invalid-name"                    # Calm down Pylint
 ]
 
 [tool.pytest.ini_options]
 addopts = "--cov=lambda_handler --cov-report term-missing"
 
 [build-system]
-requires = ["poetry-core>=1.2.1"]
+requires = ["poetry-core>=2.0.0a1"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `lambda_handler-1.2.1/PKG-INFO` & `lambda_handler-2.0.0a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lambda-handler
-Version: 1.2.1
+Version: 2.0.0a1
 Summary: A Python package for routing and validating AWS events inside a Lambda function
 Home-page: https://github.com/branchenergy/lambda-handler
 License: Apache 2.0
 Author: Matthew Badger
 Author-email: matt@branchenergy.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
```

