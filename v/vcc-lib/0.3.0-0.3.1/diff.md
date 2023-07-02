# Comparing `tmp/vcc_lib-0.3.0-py3-none-any.whl.zip` & `tmp/vcc_lib-0.3.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 12409 bytes, number of entries: 12
+Zip file size: 12501 bytes, number of entries: 12
 -rw-r--r--  2.0 unx      223 b- defN 23-Jun-28 02:28 vcc/__init__.py
 -rw-r--r--  2.0 unx      180 b- defN 23-Jun-28 02:31 vcc/__main__.py
 -rw-r--r--  2.0 unx     2055 b- defN 23-Jun-30 07:34 vcc/protocol.py
--rw-r--r--  2.0 unx     9764 b- defN 23-Jun-30 07:34 vcc/service.py
+-rw-r--r--  2.0 unx    10045 b- defN 23-Jul-01 14:43 vcc/service.py
 -rw-r--r--  2.0 unx      165 b- defN 23-Jun-28 03:09 vcc/test.py
 -rw-r--r--  2.0 unx     3210 b- defN 23-Jun-30 07:35 vcc/tools.py
--rw-r--r--  2.0 unx    25087 b- defN 23-Jun-30 07:42 vcc/vcc.py
--rw-r--r--  2.0 unx     1059 b- defN 23-Jun-30 07:55 vcc_lib-0.3.0.dist-info/LICENCE
--rw-r--r--  2.0 unx       95 b- defN 23-Jun-30 07:55 vcc_lib-0.3.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-30 07:55 vcc_lib-0.3.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        4 b- defN 23-Jun-30 07:55 vcc_lib-0.3.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      872 b- defN 23-Jun-30 07:55 vcc_lib-0.3.0.dist-info/RECORD
-12 files, 42806 bytes uncompressed, 10973 bytes compressed:  74.4%
+-rw-r--r--  2.0 unx    25087 b- defN 23-Jul-01 07:56 vcc/vcc.py
+-rw-r--r--  2.0 unx     1059 b- defN 23-Jul-02 01:26 vcc_lib-0.3.1.dist-info/LICENCE
+-rw-r--r--  2.0 unx       95 b- defN 23-Jul-02 01:26 vcc_lib-0.3.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-02 01:26 vcc_lib-0.3.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        4 b- defN 23-Jul-02 01:26 vcc_lib-0.3.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      873 b- defN 23-Jul-02 01:26 vcc_lib-0.3.1.dist-info/RECORD
+12 files, 43088 bytes uncompressed, 11065 bytes compressed:  74.3%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: vcc/tools.py
 Comment: 
 
 Filename: vcc/vcc.py
 Comment: 
 
-Filename: vcc_lib-0.3.0.dist-info/LICENCE
+Filename: vcc_lib-0.3.1.dist-info/LICENCE
 Comment: 
 
-Filename: vcc_lib-0.3.0.dist-info/METADATA
+Filename: vcc_lib-0.3.1.dist-info/METADATA
 Comment: 
 
-Filename: vcc_lib-0.3.0.dist-info/WHEEL
+Filename: vcc_lib-0.3.1.dist-info/WHEEL
 Comment: 
 
-Filename: vcc_lib-0.3.0.dist-info/top_level.txt
+Filename: vcc_lib-0.3.1.dist-info/top_level.txt
 Comment: 
 
-Filename: vcc_lib-0.3.0.dist-info/RECORD
+Filename: vcc_lib-0.3.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## vcc/service.py

```diff
@@ -1,10 +1,10 @@
 
 from __future__ import annotations
-
+import os
 import asyncio
 import inspect
 import json
 import functools
 import typing
 import logging
 import traceback
@@ -14,15 +14,15 @@
     from . import tools
 except ImportError:
     import tools
 # from twisted.internet import task ### No more twisted
 # from twisted.internet.defer import Deferred
 # from twisted.internet.protocol import ClientFactory
 # from twisted.protocols.basic import LineReceiver
-
+call_verbose=bool(os.getenv("VCC_CALL_VERBOSE"))
 log = logging.getLogger(__name__)
 log.addHandler(logging.NullHandler())
 RpcServiceRole = enum.Enum("RpcServiceRole", ["SERVER", "CLIENT"])
 request_context=tools.ContextObject()
 
 class ServiceExport:
     def __init__(self, func=None, async_mode=False, thread=False, instance=None):
@@ -116,22 +116,24 @@
     def connection_made(self, transport):
         self.transport = transport
         if self.role == RpcServiceRole.SERVER:
             if "rpc" in self.factory.services:
                 capacity=list(self.factory.services["rpc"].keys())
             else:
                 capacity=[]
-            self.send(type="connect",  capacity=capacity))
+            self.send(type="connect",  capacity=capacity)
         else:
             self.factory.connections.append(self)
     def connection_lost(self, exc: Exception | None):
         if self.role == RpcServiceRole.CLIENT:
             self.factory.on_con_lost.set_result(True)
 
     async def call(self, namespace, service, kwargs):
+        if call_verbose:
+            print(f'Call {namespace}.{service}({kwargs})')
         jobid = str(uuid.uuid4())
         future = asyncio.Future()
         self.jobs[jobid] = future
         self.send(
             type="call", jobid=jobid, namespace=namespace, service=service, data=kwargs
         )
         return await future
@@ -181,15 +183,15 @@
             return
         match data.get("type", None):
             case "call":
                 asyncio.create_task(self.a_do_request(data))
             case "connect":
                 if self.role == RpcServiceRole.CLIENT:
                     if "register" in data["capacity"]:
-                        print(self.factory.superservice)
+                        print(self.factory.services.rpc)
                         asyncio.get_running_loop().create_task(self.factory.services.rpc.register(namespace=list(self.factory.services.keys())))
             case "respond":
                 self.make_respond(data["jobid"], data["data"])
 
 
 class ServiceTable(dict):
     def __init__(self, factory):
@@ -201,15 +203,19 @@
             superservice: Service = self.factory.superservice
             return type(
                 name,
                 (),
                 {
                     "__getitem__": lambda self, n: functools.partial(
                         superservice.send, name, n
+                    ),
+                    "__getattr__": lambda self, n: lambda **x: superservice.call(
+                        name, n, x
                     )
+
                 },
             )()
         raise KeyError()
     def __getitem__(self, name):
         return self._get(name)
     def __setitem__(self, name, value):
         dict.__setitem__(self, name, value)
```

## Comparing `vcc_lib-0.3.0.dist-info/LICENCE` & `vcc_lib-0.3.1.dist-info/LICENCE`

 * *Files identical despite different names*

## Comparing `vcc_lib-0.3.0.dist-info/RECORD` & `vcc_lib-0.3.1.dist-info/RECORD`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 vcc/__init__.py,sha256=SWP73Z2KDELHZbCw5rfrDb5pLT2NdUUHeYg4OxMqooQ,223
 vcc/__main__.py,sha256=X3Q1SR4yke1OH5T7GIQCHg5Z9ToddIV4dTSowN7M2KU,180
 vcc/protocol.py,sha256=dE7T7s7IjiJKqW1CCzk0aq5ue6Nm1UYU2rXbZLsZB84,2055
-vcc/service.py,sha256=8tPYW5GdeikDtJzKlLOLBZ8hcHXOBJEkit4ibI-v_Yg,9764
+vcc/service.py,sha256=-ZaYVnLFf_dKP57Qyli97tORaTLqdZkm3aE_bnNOXDM,10045
 vcc/test.py,sha256=3-K3B97K3HSh7c-krQ-dvnvSJTWdvqbAl11Bphk-b-c,165
 vcc/tools.py,sha256=AweITDv38zqpRCudI2uFKqJrQ5a3qrqCsoezPZTe3zc,3210
 vcc/vcc.py,sha256=8Pzdlj4DlD1uNQAof29JeTQvNsTOiuv1jg_5lsJdepc,25087
-vcc_lib-0.3.0.dist-info/LICENCE,sha256=MftGbLni_zEdTcKvQ3GG8bnVQXInDQ3Tvcz4u6F-sbs,1059
-vcc_lib-0.3.0.dist-info/METADATA,sha256=5M3g29rq7-RmCtsmmxFxXqtn8cMMPCDi0tOLwS-nbcM,95
-vcc_lib-0.3.0.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-vcc_lib-0.3.0.dist-info/top_level.txt,sha256=tGqVZ1HPtvJIngQXk2bgf2CDFjONXf_wgMeCcQvD7gM,4
-vcc_lib-0.3.0.dist-info/RECORD,,
+vcc_lib-0.3.1.dist-info/LICENCE,sha256=MftGbLni_zEdTcKvQ3GG8bnVQXInDQ3Tvcz4u6F-sbs,1059
+vcc_lib-0.3.1.dist-info/METADATA,sha256=zW8DClAo2Jl8SUJ7kv9wEpEqHXZoOdAgocatm6wx3Cs,95
+vcc_lib-0.3.1.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+vcc_lib-0.3.1.dist-info/top_level.txt,sha256=tGqVZ1HPtvJIngQXk2bgf2CDFjONXf_wgMeCcQvD7gM,4
+vcc_lib-0.3.1.dist-info/RECORD,,
```

