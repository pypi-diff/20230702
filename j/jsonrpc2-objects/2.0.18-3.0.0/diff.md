# Comparing `tmp/jsonrpc2_objects-2.0.18.tar.gz` & `tmp/jsonrpc2-objects-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsonrpc2_objects-2.0.18.tar", max compression
+gzip compressed data, was "jsonrpc2-objects-3.0.0.tar", max compression
```

## Comparing `jsonrpc2_objects-2.0.18.tar` & `jsonrpc2-objects-3.0.0.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0     1072 2023-03-14 02:43:40.279946 jsonrpc2_objects-2.0.18/LICENSE
--rw-r--r--   0        0        0     1329 2023-03-14 02:43:40.279946 jsonrpc2_objects-2.0.18/README.md
--rw-r--r--   0        0        0       68 2023-03-14 02:43:40.279946 jsonrpc2_objects-2.0.18/jsonrpcobjects/__init__.py
--rw-r--r--   0        0        0     3183 2023-03-14 02:43:40.279946 jsonrpc2_objects-2.0.18/jsonrpcobjects/errors.py
--rw-r--r--   0        0        0     1912 2023-03-14 02:43:40.279946 jsonrpc2_objects-2.0.18/jsonrpcobjects/objects.py
--rw-r--r--   0        0        0        0 2023-03-14 02:43:40.279946 jsonrpc2_objects-2.0.18/jsonrpcobjects/py.typed
--rw-r--r--   0        0        0      715 2023-03-14 02:43:40.279946 jsonrpc2_objects-2.0.18/pyproject.toml
--rw-r--r--   0        0        0     2077 1970-01-01 00:00:00.000000 jsonrpc2_objects-2.0.18/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-07-01 18:36:37.418807 jsonrpc2-objects-3.0.0/LICENSE
+-rw-r--r--   0        0        0     1097 2023-07-02 16:48:38.497302 jsonrpc2-objects-3.0.0/README.md
+-rw-r--r--   0        0        0       68 2023-07-01 18:36:37.418807 jsonrpc2-objects-3.0.0/jsonrpcobjects/__init__.py
+-rw-r--r--   0        0        0     3150 2023-07-02 01:17:33.004977 jsonrpc2-objects-3.0.0/jsonrpcobjects/errors.py
+-rw-r--r--   0        0        0     1699 2023-07-02 16:52:42.538425 jsonrpc2-objects-3.0.0/jsonrpcobjects/objects.py
+-rw-r--r--   0        0        0        0 2023-07-01 18:36:37.418807 jsonrpc2-objects-3.0.0/jsonrpcobjects/py.typed
+-rw-r--r--   0        0        0     1302 2023-07-02 16:52:39.382410 jsonrpc2-objects-3.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1895 2023-07-02 17:39:56.654662 jsonrpc2-objects-3.0.0/setup.py
+-rw-r--r--   0        0        0     1741 2023-07-02 17:39:56.654791 jsonrpc2-objects-3.0.0/PKG-INFO
```

### Comparing `jsonrpc2_objects-2.0.18/LICENSE` & `jsonrpc2-objects-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jsonrpc2_objects-2.0.18/README.md` & `jsonrpc2-objects-3.0.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -4,44 +4,39 @@
 [![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://mit-license.org/)
 
 A collection of objects for use in JSON-RPC 2.0 implementations.
 
 ## Installation
 
 ```shell
-pip install jsonrpc2-objects
+poetry add jsonrpc2-objects
 ```
 
 ```shell
-poetry add jsonrpc2-objects
+pip install jsonrpc2-objects
 ```
 
 ## Objects
 
 Available in `objects` are the following:
 
-| Object                   | Description                 |
-|--------------------------|-----------------------------|
-| RequestObjectParams      | Request with params         |
-| RequestObject            | Request without params      |
-| NotificationObjectParams | Notification with params    |
-| NotificationObject       | Notification without params |
-| ErrorResponseObject      | Response with result        |
-| ResultResponseObject     | Response with error         |
+| Object             | Description                 |
+|--------------------|-----------------------------|
+| ParamsRequest      | Request with params         |
+| Request            | Request without params      |
+| ParamsNotification | Notification with params    |
+| Notification       | Notification without params |
+| ErrorResponse      | Response with result        |
+| ResultResponse     | Response with error         |
 
 ## Errors
 
 Python exceptions are available for each JSON-RPC 2.0 error. Each error
 extends `JSONRPCError`.
 
-Example use with a client implementing these errors:
-
-```python
-from jsonrpcobjects.errors import JSONRPCError, MethodNotFound
-
-try:
-    client.example_method(params)
-except MethodNotFound:
-    print("Handle method not found")
-except JSONRPCError:
-    print("Handle any JSON RPC error.")
-```
+- JSONRPCError
+- InternalError
+- InvalidParams
+- InvalidRequest
+- MethodNotFound
+- ParseError
+- ServerError
```

### Comparing `jsonrpc2_objects-2.0.18/jsonrpcobjects/errors.py` & `jsonrpc2-objects-3.0.0/jsonrpcobjects/errors.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 """This module provides exceptions for each JSON-RPC 2.0 error.
 
 There is one Exception defined for each pre-defined JSON-RPC 2.0 error.
 Additionally, there is a ServerError for implementation-defined errors.
 
 Each exception extends a base exception JSONRPCError.
 """
-from typing import Optional, Type
-
-from jsonrpcobjects.objects import ErrorObject, ErrorObjectData, ErrorType
 
 __all__ = (
     "INTERNAL_ERROR",
     "INVALID_PARAMS",
     "INVALID_REQUEST",
     "InternalError",
     "InvalidParams",
@@ -21,28 +18,32 @@
     "MethodNotFound",
     "PARSE_ERROR",
     "ParseError",
     "ServerError",
     "get_exception_by_code",
 )
 
-INVALID_REQUEST = ErrorObject(code=-32600, message="Invalid Request")
-METHOD_NOT_FOUND = ErrorObject(code=-32601, message="Method not found")
-INVALID_PARAMS = ErrorObject(code=-32602, message="Invalid params")
-INTERNAL_ERROR = ErrorObject(code=-32603, message="Internal error")
-PARSE_ERROR = ErrorObject(code=-32700, message="Parse error")
+from typing import Optional, Type
+
+from jsonrpcobjects.objects import DataError, Error, ErrorType
+
+INVALID_REQUEST = Error(code=-32600, message="Invalid Request")
+METHOD_NOT_FOUND = Error(code=-32601, message="Method not found")
+INVALID_PARAMS = Error(code=-32602, message="Invalid params")
+INTERNAL_ERROR = Error(code=-32603, message="Internal error")
+PARSE_ERROR = Error(code=-32700, message="Parse error")
 
 
 class JSONRPCError(Exception):
     """Base error that all JSON RPC exceptions extend."""
 
     def __init__(self, error: ErrorType) -> None:
         msg = f"{error.code}: {error.message}"
         self.rpc_error = error
-        if isinstance(error, ErrorObjectData):
+        if isinstance(error, DataError):
             msg += f"\nError Data: {error.data}"
         super(JSONRPCError, self).__init__(msg)
 
 
 class ParseError(JSONRPCError):
     """Error raised when invalid JSON was received by the server."""
 
@@ -81,16 +82,16 @@
 class ServerError(JSONRPCError):
     """Error raised when a server error occurs."""
 
     def __init__(self, error: ErrorType) -> None:
         super(ServerError, self).__init__(error)
 
 
-def get_exception_by_code(code: int) -> Optional[Type]:
-    """Get the JSON-RPC error corresponding to an error Code.
+def get_exception_by_code(code: int) -> Optional[Type[JSONRPCError]]:
+    """Get the JSON-RPC error corresponding to an error code.
 
     :param code: The JSON-RPC error code.
     :return: JSON RPC error object or None.
     """
     return {
         -32600: InvalidRequest,
         -32601: MethodNotFound,
```

### Comparing `jsonrpc2_objects-2.0.18/jsonrpcobjects/objects.py` & `jsonrpc2-objects-3.0.0/jsonrpcobjects/objects.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,87 +1,88 @@
 """JSON-RPC 2.0 spec objects."""
-from typing import Any, Optional, Union
-
-from pydantic import BaseModel, StrictInt, StrictStr
 
 __all__ = (
+    "DataError",
+    "Error",
+    "ErrorResponse",
     "ErrorType",
+    "Notification",
     "NotificationType",
+    "ParamsNotification",
+    "ParamsRequest",
+    "Request",
     "RequestType",
     "ResponseType",
-    "ErrorObject",
-    "ErrorObjectData",
-    "ErrorResponseObject",
-    "NotificationObject",
-    "NotificationObjectParams",
-    "RequestObject",
-    "RequestObjectParams",
-    "ResultResponseObject",
+    "ResultResponse",
 )
 
-ErrorType = Union["ErrorObjectData", "ErrorObject"]
-NotificationType = Union["NotificationObject", "NotificationObjectParams"]
-RequestType = Union["RequestObjectParams", "RequestObject"]
-ResponseType = Union["ErrorResponseObject", "ResultResponseObject"]
+from typing import Any, Optional, Union
+
+from pydantic import BaseModel
+
+ErrorType = Union["DataError", "Error"]
+NotificationType = Union["Notification", "ParamsNotification"]
+RequestType = Union["ParamsRequest", "Request"]
+ResponseType = Union["ErrorResponse", "ResultResponse"]
 
 
-class RequestObjectParams(BaseModel):
+class ParamsRequest(BaseModel):
     """JSON-RPC 2.0 request object with parameters."""
 
-    id: Union[StrictInt, StrictStr]
+    id: Union[int, str]
     method: str
     params: Union[list, dict]
     jsonrpc: str = "2.0"
 
 
-class RequestObject(BaseModel):
+class Request(BaseModel):
     """JSON-RPC 2.0 request object."""
 
-    id: Union[StrictInt, StrictStr]
+    id: Union[int, str]
     method: str
     jsonrpc: str = "2.0"
 
 
-class NotificationObjectParams(BaseModel):
+class ParamsNotification(BaseModel):
     """JSON-RPC 2.0 notification object with parameters."""
 
     method: str
     params: Union[list, dict]
     jsonrpc: str = "2.0"
 
 
-class NotificationObject(BaseModel):
+class Notification(BaseModel):
     """JSON-RPC 2.0 notification object."""
 
     method: str
     jsonrpc: str = "2.0"
 
 
-class ErrorObjectData(BaseModel):
+class DataError(BaseModel):
     """JSON-RPC 2.0 error object with data."""
 
     code: int
     message: str
     data: Any
 
 
-class ErrorObject(BaseModel):
+class Error(BaseModel):
     """JSON-RPC 2.0 error object."""
 
     code: int
     message: str
 
 
-class ErrorResponseObject(BaseModel):
+class ErrorResponse(BaseModel):
     """JSON-RPC 2.0 error response object."""
 
-    id: Optional[Union[StrictInt, StrictStr]]
+    id: Optional[Union[int, str]]
     error: ErrorType
     jsonrpc: str = "2.0"
 
 
-class ResultResponseObject(BaseModel):
+class ResultResponse(BaseModel):
     """JSON-RPC 2.0 result response object."""
 
-    id: Union[StrictInt, StrictStr]
+    id: Union[int, str]
     result: Any
     jsonrpc: str = "2.0"
```

### Comparing `jsonrpc2_objects-2.0.18/pyproject.toml` & `jsonrpc2-objects-3.0.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,51 @@
 [tool.poetry]
 name = "jsonrpc2-objects"
-version = "2.0.18"
+version = "3.0.0"
 description = "A collection of objects for use in JSON-RPC 2.0 implementations."
 readme = "README.md"
 repository = "https://gitlab.com/mburkard/jsonrpc2-objects"
 homepage = "https://gitlab.com/mburkard/jsonrpc2-objects"
 license = "MIT"
 authors = ["Matthew Burkard <matthewjburkard@gmail.com>"]
 classifiers = ["Programming Language :: Python :: 3"]
 packages = [
     { include = "jsonrpcobjects/**/*.py" },
     { include = "jsonrpcobjects/py.typed" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
-pydantic = "^1.9.2"
+pydantic = "^2.0"
 
 [tool.poetry.dev-dependencies]
 mypy = "^1.1.1"
+ruff = "^0.0.275"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
+
+[tool.ruff]
+select = [
+    # Pyflakes
+    "F",
+    # Pycodestyle
+    "E",
+    "W",
+    # isort
+    "I001"
+]
+ignore = []
+
+fixable = ["A", "B", "C", "D", "E", "F", "G", "I", "N", "Q", "S", "T", "W", "ANN", "ARG", "BLE", "COM", "DJ", "DTZ", "EM", "ERA", "EXE", "FBT", "ICN", "INP", "ISC", "NPY", "PD", "PGH", "PIE", "PL", "PT", "PTH", "PYI", "RET", "RSE", "RUF", "SIM", "SLF", "TCH", "TID", "TRY", "UP", "YTT"]
+unfixable = []
+exclude = [
+    ".eggs",
+    ".git",
+    ".git-rewrite",
+    ".mypy_cache",
+    ".ruff_cache",
+    "__pypackages__",
+    "dist",
+]
+line-length = 88
```

### Comparing `jsonrpc2_objects-2.0.18/PKG-INFO` & `jsonrpc2-objects-3.0.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,67 +1,60 @@
 Metadata-Version: 2.1
 Name: jsonrpc2-objects
-Version: 2.0.18
+Version: 3.0.0
 Summary: A collection of objects for use in JSON-RPC 2.0 implementations.
 Home-page: https://gitlab.com/mburkard/jsonrpc2-objects
 License: MIT
 Author: Matthew Burkard
 Author-email: matthewjburkard@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Requires-Dist: pydantic (>=1.9.2,<2.0.0)
+Classifier: Programming Language :: Python :: 3.9
+Requires-Dist: pydantic (>=2.0,<3.0)
 Project-URL: Repository, https://gitlab.com/mburkard/jsonrpc2-objects
 Description-Content-Type: text/markdown
 
 # JSON-RPC 2.0 Objects
 
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://mit-license.org/)
 
 A collection of objects for use in JSON-RPC 2.0 implementations.
 
 ## Installation
 
 ```shell
-pip install jsonrpc2-objects
+poetry add jsonrpc2-objects
 ```
 
 ```shell
-poetry add jsonrpc2-objects
+pip install jsonrpc2-objects
 ```
 
 ## Objects
 
 Available in `objects` are the following:
 
-| Object                   | Description                 |
-|--------------------------|-----------------------------|
-| RequestObjectParams      | Request with params         |
-| RequestObject            | Request without params      |
-| NotificationObjectParams | Notification with params    |
-| NotificationObject       | Notification without params |
-| ErrorResponseObject      | Response with result        |
-| ResultResponseObject     | Response with error         |
+| Object             | Description                 |
+|--------------------|-----------------------------|
+| ParamsRequest      | Request with params         |
+| Request            | Request without params      |
+| ParamsNotification | Notification with params    |
+| Notification       | Notification without params |
+| ErrorResponse      | Response with result        |
+| ResultResponse     | Response with error         |
 
 ## Errors
 
 Python exceptions are available for each JSON-RPC 2.0 error. Each error
 extends `JSONRPCError`.
 
-Example use with a client implementing these errors:
-
-```python
-from jsonrpcobjects.errors import JSONRPCError, MethodNotFound
-
-try:
-    client.example_method(params)
-except MethodNotFound:
-    print("Handle method not found")
-except JSONRPCError:
-    print("Handle any JSON RPC error.")
-```
+- JSONRPCError
+- InternalError
+- InvalidParams
+- InvalidRequest
+- MethodNotFound
+- ParseError
+- ServerError
```

