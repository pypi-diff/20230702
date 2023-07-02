# Comparing `tmp/rmy-0.1.2.tar.gz` & `tmp/rmy-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rmy-0.1.2.tar", max compression
+gzip compressed data, was "rmy-0.3.tar", max compression
```

## Comparing `rmy-0.1.2.tar` & `rmy-0.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    11357 2023-06-11 20:31:23.956812 rmy-0.1.2/LICENSE
--rw-r--r--   0        0        0     1325 2023-06-25 09:49:45.108911 rmy-0.1.2/README.md
--rw-r--r--   0        0        0     1677 2023-06-25 09:53:06.262494 rmy-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      583 2023-06-25 09:52:35.536752 rmy-0.1.2/rmy/__init__.py
--rw-r--r--   0        0        0      554 2023-06-20 06:58:29.140288 rmy-0.1.2/rmy/abc.py
--rw-r--r--   0        0        0    11641 2023-06-24 09:22:09.871746 rmy-0.1.2/rmy/client_async.py
--rw-r--r--   0        0        0     2263 2023-06-24 11:38:31.569083 rmy-0.1.2/rmy/client_sync.py
--rw-r--r--   0        0        0     1325 2023-06-22 15:27:41.453103 rmy-0.1.2/rmy/common.py
--rw-r--r--   0        0        0     2582 2023-06-20 17:35:21.011981 rmy-0.1.2/rmy/connection.py
--rw-r--r--   0        0        0    10248 2023-06-24 10:07:16.682039 rmy-0.1.2/rmy/server.py
--rw-r--r--   0        0        0     1853 1970-01-01 00:00:00.000000 rmy-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-11 20:31:23.956812 rmy-0.3/LICENSE
+-rw-r--r--   0        0        0      657 2023-06-26 21:06:30.806884 rmy-0.3/README.md
+-rw-r--r--   0        0        0     1675 2023-07-02 10:18:17.374579 rmy-0.3/pyproject.toml
+-rw-r--r--   0        0        0      565 2023-07-02 10:18:27.214111 rmy-0.3/rmy/__init__.py
+-rw-r--r--   0        0        0      740 2023-07-01 18:07:30.323702 rmy-0.3/rmy/abc.py
+-rw-r--r--   0        0        0    13202 2023-07-02 10:06:53.386688 rmy-0.3/rmy/client_async.py
+-rw-r--r--   0        0        0     2614 2023-07-02 09:57:00.022299 rmy-0.3/rmy/client_sync.py
+-rw-r--r--   0        0        0     1327 2023-06-30 16:18:33.807606 rmy-0.3/rmy/common.py
+-rw-r--r--   0        0        0     2588 2023-07-01 18:06:09.576974 rmy-0.3/rmy/connection.py
+-rw-r--r--   0        0        0    10830 2023-07-02 10:09:15.894425 rmy-0.3/rmy/server.py
+-rw-r--r--   0        0        0     1183 1970-01-01 00:00:00.000000 rmy-0.3/PKG-INFO
```

### Comparing `rmy-0.1.2/LICENSE` & `rmy-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `rmy-0.1.2/pyproject.toml` & `rmy-0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 relative_files = true
 
 [tool.coverage.report]
 show_missing = true
 
 [tool.poetry]
 name = "rmy"
-version = "0.1.2"
+version = "0.3"
 description = "Stateful rpc for Python"
 authors = ["fdv1 <francois@pytek.io>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4.0"
 anyio = "^3.7.0"
```

### Comparing `rmy-0.1.2/rmy/__init__.py` & `rmy-0.3/rmy/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,20 @@
-__version__ = "0.1.2"
+__version__ = "0.1.3"
 __author__ = "Francois du Vignaud"
 
 __all__ = [
     "AsyncClient",
     "create_async_client",
     "SyncClient",
     "create_sync_client",
-    "UserException",
+    "RemoteException",
     "cancel_task_group_on_signal",
     "scoped_iter",
     "connect_to_tcp_server",
-    "Server",
     "run_tcp_server",
 ]
 
 from .client_async import AsyncClient, create_async_client
 from .client_sync import SyncClient, create_sync_client
-from .common import UserException, cancel_task_group_on_signal, scoped_iter
+from .common import RemoteException, cancel_task_group_on_signal, scoped_iter
 from .connection import connect_to_tcp_server
-from .server import Server, run_tcp_server
+from .server import run_tcp_server
```

### Comparing `rmy-0.1.2/rmy/abc.py` & `rmy-0.3/rmy/abc.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from __future__ import annotations
-
 from abc import ABCMeta, abstractmethod
-from typing import Any, AsyncIterator, Tuple
+from typing import Any, AsyncIterator, Callable, Tuple
 
 
 class Connection(AsyncIterator[Any], metaclass=ABCMeta):
     @abstractmethod
     async def send(self, message: Tuple[Any, ...]):
         ...
 
@@ -17,12 +16,20 @@
     async def drain(self):
         ...
 
     @abstractmethod
     def close(self):
         ...
 
+    @abstractmethod
+    def set_dumps(self, dumps: Callable[[Any], bytes]):
+        ...
+
+    @abstractmethod
+    def set_loads(self, loads: Callable[[bytes], Any]):
+        ...
+
 
 class AsyncSink:
     @abstractmethod
-    def send_nowait(self, value: Any):
+    def set_result(self, value: Any):
         ...
```

### Comparing `rmy-0.1.2/rmy/client_async.py` & `rmy-0.3/rmy/client_async.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,65 +1,73 @@
 from __future__ import annotations
 
 import asyncio
 import contextlib
 import inspect
+import io
+import pickle
 import queue
-from collections.abc import AsyncIterable
 from functools import partial
 from itertools import count
-from typing import TYPE_CHECKING, Any, AsyncIterator, Callable, Dict, Optional
+from typing import TYPE_CHECKING, Any, AsyncIterator, Callable, Optional
 
 import anyio
 import anyio.abc
 import asyncstdlib
 
 from .abc import AsyncSink, Connection
-from .common import UserException, cancel_task_on_exit, scoped_insert
+from .common import cancel_task_on_exit, scoped_insert
 from .connection import connect_to_tcp_server
 
 
 if TYPE_CHECKING:
     from .client_sync import SyncClient
 
 
 OK = "OK"
 CLOSE_SENTINEL = "Close sentinel"
-CANCELLED_TASK = "Cancelled task"
+CANCEL_TASK = "Cancel task"
 EXCEPTION = "Exception"
-USER_EXCEPTION = "UserException"
 CREATE_OBJECT = "Create object"
 DELETE_OBJECT = "Delete object"
 FETCH_OBJECT = "Fetch object"
 GET_ATTRIBUTE = "Get attribute"
 SET_ATTRIBUTE = "Set attribute"
-ASYNC_ITERATOR = "Async iterator"
-MOVE_ASYNC_ITERATOR = "Move Async iterator"
-METHOD = "Function"
-ITER_ASYNC_ITERATOR = "Iter async iterator"
+MOVE_GENERATOR_ITERATOR = "Move Async iterator"
+EVALUATE_METHOD = "Evaluate method"
+ITERATE_GENERATOR = "Iterate generator"
+AWAIT_COROUTINE = "Await coroutine"
 STREAM_BUFFER_SIZE = 10
 
 SERVER_OBJECT_ID = 0
 
 ASYNC_SETATTR_ERROR_MESSAGE = "Cannot set attribute on remote object in async mode. Use setattr method instead. \
 We intentionally do not support setting attributes using assignment operator on remote objects in async mode. \
 This is because it is not a good practice not too wait until a remote operation completes."
 
 ASYNC_GENERATOR_OVERFLOWED_MESSAGE = "Async generator overflowed."
 
-REQUEST_CODES = (METHOD, GET_ATTRIBUTE, CREATE_OBJECT, FETCH_OBJECT, SET_ATTRIBUTE)
+REQUEST_CODES = (
+    EVALUATE_METHOD,
+    GET_ATTRIBUTE,
+    CREATE_OBJECT,
+    FETCH_OBJECT,
+    SET_ATTRIBUTE,
+    ITERATE_GENERATOR,
+    AWAIT_COROUTINE,
+)
 
 
 class IterationBufferSync(AsyncSink):
     def __init__(self, size: int) -> None:
         self._overflowed = False
         self._size = size
         self._queue = queue.SimpleQueue()
 
-    def send_nowait(self, value: Any):
+    def set_result(self, value: Any):
         self._queue.put_nowait(value)
         if self._queue.qsize() >= self._size:
             self._overflowed = True
             raise asyncio.QueueFull()
 
     def __iter__(self):
         return self
@@ -71,15 +79,15 @@
 
 
 class IterationBufferAsync(AsyncSink):
     def __init__(self, size: int) -> None:
         self._overflowed = False
         self._queue = asyncio.Queue(maxsize=size)
 
-    def send_nowait(self, value: Any):
+    def set_result(self, value: Any):
         try:
             self._queue.put_nowait(value)
         except asyncio.QueueFull:
             self._overflowed = True
             raise
 
     def __aiter__(self):
@@ -87,55 +95,100 @@
 
     async def __anext__(self):
         if self._overflowed:
             raise OverflowError(ASYNC_GENERATOR_OVERFLOWED_MESSAGE)
         return await self._queue.get()
 
 
-class AsyncCallResult(AsyncIterable):
+class RemoteValue:
+    def __init__(self, value):
+        self.value_id = value
+
+
+class RemoteAsyncGenerator(RemoteValue):
+    pass
+
+
+class RemoteSyncGenerator(RemoteValue):
+    pass
+
+
+class RemoteCoroutine(RemoteValue):
+    pass
+
+
+class RMYPickler(pickle.Pickler):
+    def persistent_id(self, obj):
+        if isinstance(obj, RemoteValue):
+            return (type(obj).__name__, obj.value_id)
+
+
+class RemoteUnpickler(pickle.Unpickler):
+    def __init__(self, file, client):
+        super().__init__(file)
+        self.client = client
+
+    def persistent_load(self, value):
+        type_tag, payload = value
+        if type_tag in ("RemoteAsyncGenerator", "RemoteSyncGenerator"):
+            synchronize = type_tag == "RemoteSyncGenerator"
+            if self.client.client_sync:
+                return self.client.client_sync._sync_generator_iter(synchronize, payload)
+            return self.client.fetch_values_async(synchronize, payload)
+        elif type_tag == "RemoteCoroutine":
+            return self.client._execute_request(
+                AWAIT_COROUTINE,
+                (payload,),
+                is_cancellable=True,
+                include_code=False,
+            )
+        else:
+            raise pickle.UnpicklingError("Unsupported object")
+
+
+def rmy_dumps(value):
+    file = io.BytesIO()
+    RMYPickler(file).dump(value)
+    return file.getvalue()
+
+
+class AsyncCallResult:
     def __init__(self, client, object_id: int, function: Callable, args, kwargs):
         self.client: AsyncClient = client
         self.object_id = object_id
         self.function = function
         self.args = args
         self.kwargs = kwargs
 
     def __await__(self):
-        return asyncio.create_task(
-            self.client.execute_request(
-                METHOD,
-                (self.object_id, self.function, self.args, self.kwargs),
-                is_cancellable=True,
-                include_code=False,
-            )
+        return self.client._evaluate_async_method(
+            self.object_id, self.function, self.args, self.kwargs
         ).__await__()
 
     def __aiter__(self):
         return self.client._evaluate_async_generator(
             self.object_id, self.function, self.args, self.kwargs
         )
 
 
 def decode_result(code, result, include_code=True):
-    if code in (CANCELLED_TASK, OK, ASYNC_ITERATOR):
+    if code in (CANCEL_TASK, OK):
         return (code, result) if include_code else result
-    if code == USER_EXCEPTION:
-        raise UserException(result)
     if code == EXCEPTION:
-        if isinstance(result, Exception):
-            raise result
-        raise Exception(result)
+        raise result if isinstance(result, Exception) else Exception(result)
     else:
         raise Exception(f"Unexpected code {code} received.")
 
 
 def decode_iteration_result(code, result):
-    if code in (CLOSE_SENTINEL, CANCELLED_TASK):
+    if code in (CLOSE_SENTINEL, CANCEL_TASK):
         return True, None
-    return False, decode_result(code, result, include_code=False)
+    if code == EXCEPTION:
+        raise result
+    return False, result
 
 
 class RemoteObject:
     def __init__(self, client, object_id: int):
         self.client = client
         self.object_id = object_id
 
@@ -144,21 +197,22 @@
     raise AttributeError(ASYNC_SETATTR_ERROR_MESSAGE)
 
 
 class AsyncClient:
     def __init__(
         self, connection: Connection, async_buffer_size: int = STREAM_BUFFER_SIZE
     ) -> None:
+        connection.set_loads(lambda value: RemoteUnpickler(io.BytesIO(value), self).load())
         self.connection = connection
         self._async_buffer_size = async_buffer_size
         self.request_id = count()
         self.object_id = count()
         self.pending_requests = {}
-        self._iteraton_buffers: Dict[int, AsyncSink] = {}
         self.remote_objects = {}
+        self.client_sync: Optional[SyncClient] = None
 
     async def _send(self, *args):
         await self.connection.send(args)
 
     def _send_nowait(self, *args):
         self.connection.send_nowait(args)
 
@@ -166,110 +220,124 @@
         self, task_status: anyio.abc.TaskStatus = anyio.TASK_STATUS_IGNORED
     ):
         task_status.started()
         async for code, message_id, status, result in self.connection:
             if code in REQUEST_CODES:
                 if future := self.pending_requests.get(message_id):
                     future.set_result((status, result))
-            elif code == ITER_ASYNC_ITERATOR:
-                if queue := self._iteraton_buffers.get(message_id):
-                    queue.send_nowait((status, result))
-            elif code == CANCELLED_TASK:
+            elif code == CANCEL_TASK:
                 print("Task cancelled.", message_id, status, result)
             else:
                 print(f"Unexpected code {code} received.")
 
     @contextlib.contextmanager
     def _submit_request(self, code, args, is_cancellable=False):
-        request_id = next(self.request_id)
         future = asyncio.Future()
+        request_id = next(self.request_id)
         with scoped_insert(self.pending_requests, request_id, future):
             self._send_nowait(code, request_id, args)
             try:
                 yield future
             except anyio.get_cancelled_exc_class():
                 if is_cancellable:
                     self._cancel_request_no_wait(request_id)
                 raise
 
-    async def execute_request(self, code, args, is_cancellable=False, include_code=True) -> Any:
+    async def _execute_request(self, code, args, is_cancellable=False, include_code=True) -> Any:
         with self._submit_request(code, args, is_cancellable) as future:
             return decode_result(*(await future), include_code=include_code)
 
     async def _get_attribute(self, object_id: int, name: str):
-        return await self.execute_request(GET_ATTRIBUTE, (object_id, name), include_code=False)
+        return await self._execute_request(GET_ATTRIBUTE, (object_id, name), include_code=False)
 
     async def _set_attribute(self, object_id: int, name: str, value: Any):
-        return await self.execute_request(
+        return await self._execute_request(
             SET_ATTRIBUTE, (object_id, name, value), include_code=False
         )
 
     def _call_method_remotely(self, object_id: int, function: Callable, *args, **kwargs) -> Any:
         return AsyncCallResult(self, object_id, function, args, kwargs)
 
     def _cancel_request_no_wait(self, request_id: int):
-        self._send_nowait(CANCELLED_TASK, request_id, None)
+        self._send_nowait(CANCEL_TASK, request_id, None)
         self.pending_requests.pop(request_id, None)
 
     async def _cancel_request(self, request_id: int):
         self._cancel_request_no_wait(request_id)
         await self.connection.drain()
 
-    async def _evaluate_async_generator(self, object_id, function, args, kwargs):
-        push_or_pull, generator_id = await self.execute_request(
-            METHOD,
+    async def _evaluate_async_method(self, object_id, function, args, kwargs):
+        result = await self._execute_request(
+            EVALUATE_METHOD,
             (object_id, function, args, kwargs),
             is_cancellable=True,
             include_code=False,
         )
+        if inspect.iscoroutine(result):
+            result = await result
+        return result
+
+    async def fetch_values_async(self, synchronize: bool, value_id: int):
         queue = IterationBufferAsync(self._async_buffer_size)
         request_id = next(self.request_id)
-        with scoped_insert(self._iteraton_buffers, request_id, queue):
-            await self._send(ITER_ASYNC_ITERATOR, request_id, (generator_id,))
+        with scoped_insert(self.pending_requests, request_id, queue):
+            await self._send(ITERATE_GENERATOR, request_id, (value_id,))
             try:
                 async for index, (terminated, value) in asyncstdlib.enumerate(
                     asyncstdlib.starmap(decode_iteration_result, queue)
                 ):
                     if terminated:
                         break
                     yield value
-                    if not push_or_pull:
-                        await self._send(MOVE_ASYNC_ITERATOR, generator_id, (index + 1,))
+                    if synchronize:
+                        await self._send(MOVE_GENERATOR_ITERATOR, value_id, (index + 1,))
             finally:
                 await self._cancel_request(request_id)
 
+    async def _evaluate_async_generator(self, object_id, function, args, kwargs):
+        generator = await self._execute_request(
+            EVALUATE_METHOD,
+            (object_id, function, args, kwargs),
+            is_cancellable=True,
+            include_code=False,
+        )
+        async for value in generator:
+            yield value
+
     @contextlib.asynccontextmanager
     async def _remote_sync_generator_iter(self, iterator_id: int):
         queue = IterationBufferSync(self._async_buffer_size)
         request_id = next(self.request_id)
-        with scoped_insert(self._iteraton_buffers, request_id, queue):
+        with scoped_insert(self.pending_requests, request_id, queue):
             try:
-                await self._send(ITER_ASYNC_ITERATOR, request_id, (iterator_id,))
+                await self._send(ITERATE_GENERATOR, request_id, (iterator_id,))
                 yield queue
             finally:
                 await self._cancel_request(request_id)
 
     @contextlib.asynccontextmanager
     async def create_remote_object(
         self, object_class, args=(), kwarg={}, sync_client: Optional[SyncClient] = None
     ):
-        object_id = await self.execute_request(
+        object_id = await self._execute_request(
             CREATE_OBJECT, (object_class, args, kwarg), include_code=False
         )
         try:
             yield await self._fetch_remote_object(object_id, sync_client)
         finally:
             with anyio.CancelScope(shield=True):
                 await self._send(DELETE_OBJECT, 0, object_id)
 
     async def _fetch_remote_object(
         self, object_id: int = SERVER_OBJECT_ID, sync_client: Optional[SyncClient] = None
     ) -> Any:
         if object_id not in self.remote_objects:
-            object_class = await self.execute_request(FETCH_OBJECT, object_id, include_code=False)
+            object_class = await self._execute_request(
+                FETCH_OBJECT, (object_id,), include_code=False
+            )
             setattr = partial(self._set_attribute, object_id)
             __getattr__ = partial(self._get_attribute, object_id)
             if sync_client:
                 __getattr__ = sync_client._wrap_awaitable(__getattr__)
                 setattr = __setattr__ = sync_client._wrap_awaitable(setattr)
             else:
                 __setattr__ = __setattr_forbidden__
```

### Comparing `rmy-0.1.2/rmy/common.py` & `rmy-0.3/rmy/common.py`

 * *Files 8% similar despite different names*

```diff
@@ -53,11 +53,11 @@
             else:
                 print(f"Received signal {signum}, terminating.")
 
             task_group.cancel_scope.cancel()
             return
 
 
-class UserException(Exception):
+class RemoteException(Exception):
     """Use this to signal expected errors to users."""
 
     pass
```

### Comparing `rmy-0.1.2/rmy/server.py` & `rmy-0.3/rmy/server.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,37 +1,42 @@
 from __future__ import annotations
-
 import asyncio
 import contextlib
+import inspect
+import sys
 import traceback
 from itertools import count
 from typing import Any
-import inspect
+
 import anyio
 import anyio.abc
 import asyncstdlib
 
 from .abc import Connection
 from .client_async import (
-    ASYNC_ITERATOR,
-    CANCELLED_TASK,
+    AWAIT_COROUTINE,
+    CANCEL_TASK,
     CLOSE_SENTINEL,
     CREATE_OBJECT,
     DELETE_OBJECT,
+    EVALUATE_METHOD,
     EXCEPTION,
     FETCH_OBJECT,
     GET_ATTRIBUTE,
-    ITER_ASYNC_ITERATOR,
-    MOVE_ASYNC_ITERATOR,
-    METHOD,
+    ITERATE_GENERATOR,
+    MOVE_GENERATOR_ITERATOR,
     OK,
     SET_ATTRIBUTE,
-    USER_EXCEPTION,
+    RemoteAsyncGenerator,
+    RemoteCoroutine,
+    RemoteSyncGenerator,
+    RemoteValue,
+    rmy_dumps,
 )
-from .common import UserException, cancel_task_group_on_signal, scoped_insert
+from .common import RemoteException, cancel_task_group_on_signal, scoped_insert
 from .connection import TCPConnection
 
 
 async def wrap_sync_generator(sync_generator):
     for value in sync_generator:
         yield value
 
@@ -41,69 +46,74 @@
 
 
 class ClientSession:
     def __init__(self, server, task_group, connection: Connection) -> None:
         self.session_manager: Server = server
         self.task_group = task_group
         self.connection = connection
+        connection.set_dumps(rmy_dumps)
         self.running_tasks = {}
-        self.pending_generators = {}
+        self.pending_results = {}
         self.own_objects = set()
         self.synchronization_indexes = {}
+        self.value_id = count(10)
 
     async def send(self, code: str, request_id: int, status: str, value: Any):
         await self.connection.send((code, request_id, status, value))
 
     def send_nowait(self, code: str, request_id: int, status: str, value: Any):
         self.connection.send_nowait((code, request_id, status, value))
 
     async def iterate_through_async_generator_unsync(
         self, request_id: int, iterator_id: int, coroutine_or_async_generator
     ):
         async with asyncstdlib.scoped_iter(coroutine_or_async_generator) as aiter:
             async for value in aiter:
-                await self.send(ITER_ASYNC_ITERATOR, request_id, OK, value)
+                await self.send(ITERATE_GENERATOR, request_id, OK, value)
         return CLOSE_SENTINEL, None
 
     async def iterate_through_async_generator_sync(
         self, request_id: int, iterator_id: int, coroutine_or_async_generator
     ):
         index_and_event = [0, anyio.Event()]
         with scoped_insert(self.synchronization_indexes, iterator_id, index_and_event):
             async with asyncstdlib.scoped_iter(coroutine_or_async_generator) as aiter:
                 async for index, value in asyncstdlib.enumerate(aiter):
-                    await self.send(ITER_ASYNC_ITERATOR, request_id, OK, value)
+                    await self.send(ITERATE_GENERATOR, request_id, OK, value)
                     if index >= index_and_event[0]:
                         await index_and_event[1].wait()
             return CLOSE_SENTINEL, None
 
     def iterate_generator(self, request_id: int, iterator_id: int):
-        if not (generator := self.pending_generators.pop(iterator_id, None)):
+        if not (generator := self.pending_results.pop(iterator_id, None)):
             return
-        push, generator = generator
         method = (
             self.iterate_through_async_generator_unsync
-            if push
+            if inspect.isasyncgen(generator)
             else self.iterate_through_async_generator_sync
         )
         self.cancellable_run_task(
-            request_id, ITER_ASYNC_ITERATOR, method(request_id, iterator_id, generator)
+            request_id, ITERATE_GENERATOR, method(request_id, iterator_id, generator)
         )
 
+    def evaluate_coroutine(self, request_id: int, coroutine_id: int):
+        if not (coroutine := self.pending_results.pop(coroutine_id, None)):
+            return
+        self.cancellable_run_task(request_id, AWAIT_COROUTINE, wrap_coroutine(coroutine))
+
     async def run_task(self, request_id, task_code, coroutine_or_async_generator):
         status, result = EXCEPTION, None
         try:
             status, result = await coroutine_or_async_generator
         except anyio.get_cancelled_exc_class():
-            status = CANCELLED_TASK
+            status = CANCEL_TASK
             raise
-        except UserException as e:
-            status, result = USER_EXCEPTION, e.args[0]
-        except Exception:
-            status, result = EXCEPTION, traceback.format_exc()
+        except Exception as e:
+            _, e, tb = sys.exc_info()
+            status, result = EXCEPTION, RemoteException(e, traceback.extract_tb(tb)[3:])
         finally:
             with anyio.CancelScope(shield=True):
                 await self.send(task_code, request_id, status, result)
 
     def cancellable_run_task(self, request_id, task_code, coroutine_or_async_context):
         async def task():
             task_group = anyio.create_task_group()
@@ -149,53 +159,57 @@
         code, result = OK, None
         try:
             setattr(self.session_manager.objects[object_id], name, value)
         except Exception as e:
             code, result = EXCEPTION, e
         await self.send(SET_ATTRIBUTE, request_id, code, result)
 
-    async def cancel_running_task(self, request_id: int):
+    async def cancel_task(self, request_id: int):
         if running_task := self.running_tasks.get(request_id):
             running_task()
 
     def move_async_generator_index(self, request_id: int, index: int):
         if index_and_event := self.synchronization_indexes.get(request_id, None):
             index_and_event[1].set()
             index_and_event[0] = index
             index_and_event[1] = anyio.Event()
 
-    async def evaluate_method(self, request_id, task_code, object_id, method, args, kwargs):
+    async def evaluate_method(self, request_id, object_id, method, args, kwargs):
         result = method(self.session_manager.objects[object_id], *args, **kwargs)
+        serializable_result = result
         if inspect.iscoroutine(result):
-            self.cancellable_run_task(request_id, task_code, wrap_coroutine(result))
-        elif inspect.isasyncgen(result) or inspect.isgenerator(result):
-            is_async = inspect.isasyncgen(result)
-            self.pending_generators[request_id] = (is_async, result)
-            await self.send(task_code, request_id, ASYNC_ITERATOR, (is_async, request_id))
-        else:
-            await self.send(task_code, request_id, OK, result)
+            serializable_result = RemoteCoroutine(next(self.value_id))
+        elif inspect.isasyncgen(result):
+            serializable_result = RemoteAsyncGenerator(next(self.value_id))
+        elif inspect.isgenerator(result):
+            serializable_result = RemoteSyncGenerator(next(self.value_id))
+        if isinstance(serializable_result, RemoteValue):
+            self.pending_results[serializable_result.value_id] = result
+        await self.send(EVALUATE_METHOD, request_id, OK, serializable_result)
 
     async def process_messages(self):
         async for task_code, request_id, payload in self.connection:
             try:
-                if task_code == METHOD:
-                    await self.evaluate_method(request_id, task_code, *payload)
-                elif task_code == CANCELLED_TASK:
-                    await self.cancel_running_task(request_id)
-                elif task_code == ITER_ASYNC_ITERATOR:
+                if task_code == EVALUATE_METHOD:
+                    await self.evaluate_method(request_id, *payload)
+                elif task_code == CANCEL_TASK:
+                    await self.cancel_task(request_id)
+                elif task_code == ITERATE_GENERATOR:
                     self.iterate_generator(request_id, *payload)
+                elif task_code == AWAIT_COROUTINE:
+                    self.evaluate_coroutine(request_id, *payload)
                 elif task_code == GET_ATTRIBUTE:
                     await self.get_attribute(request_id, *payload)
                 elif task_code == SET_ATTRIBUTE:
                     await self.set_attribute(request_id, *payload)
                 elif task_code == CREATE_OBJECT:
                     await self.create_object(request_id, *payload)
                 elif task_code == FETCH_OBJECT:
-                    await self.fetch_object(request_id, payload)
-                elif task_code == MOVE_ASYNC_ITERATOR:
+                    await self.fetch_object(request_id, *payload)
+                elif task_code == MOVE_GENERATOR_ITERATOR:
                     self.move_async_generator_index(request_id, *payload)
                 elif task_code == DELETE_OBJECT:
                     self.session_manager.objects.pop(payload, None)
                     self.own_objects.discard(payload)
                 else:
                     raise Exception(f"Unknown code {repr(task_code)} with payload {repr(payload)}")
             except anyio.get_cancelled_exc_class():
```

