# Comparing `tmp/htagweb-0.0.2.tar.gz` & `tmp/htagweb-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "htagweb-0.0.2.tar", max compression
+gzip compressed data, was "htagweb-0.0.3.tar", max compression
```

## Comparing `htagweb-0.0.2.tar` & `htagweb-0.0.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1065 2023-07-02 11:23:30.832444 htagweb-0.0.2/LICENSE
--rw-r--r--   0        0        0     2666 2023-07-02 11:23:30.832444 htagweb-0.0.2/README.md
--rw-r--r--   0        0        0    11075 2023-07-02 11:23:31.112445 htagweb-0.0.2/htagweb/__init__.py
--rw-r--r--   0        0        0     2519 2023-07-02 11:23:30.832444 htagweb-0.0.2/htagweb/crypto.py
--rw-r--r--   0        0        0    10269 2023-07-02 11:23:30.832444 htagweb-0.0.2/htagweb/manager.py
--rw-r--r--   0        0        0      625 2023-07-02 11:23:30.832444 htagweb-0.0.2/htagweb/shm.py
--rw-r--r--   0        0        0     1085 2023-07-02 11:23:31.112445 htagweb-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     3868 1970-01-01 00:00:00.000000 htagweb-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-07-02 14:30:33.700061 htagweb-0.0.3/LICENSE
+-rw-r--r--   0        0        0     2666 2023-07-02 14:30:33.700061 htagweb-0.0.3/README.md
+-rw-r--r--   0        0        0    11430 2023-07-02 14:30:34.004066 htagweb-0.0.3/htagweb/__init__.py
+-rw-r--r--   0        0        0     2519 2023-07-02 14:30:33.700061 htagweb-0.0.3/htagweb/crypto.py
+-rw-r--r--   0        0        0    10382 2023-07-02 14:30:33.700061 htagweb-0.0.3/htagweb/manager.py
+-rw-r--r--   0        0        0      625 2023-07-02 14:30:33.700061 htagweb-0.0.3/htagweb/shm.py
+-rw-r--r--   0        0        0     1085 2023-07-02 14:30:34.004066 htagweb-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     3868 1970-01-01 00:00:00.000000 htagweb-0.0.3/PKG-INFO
```

### Comparing `htagweb-0.0.2/LICENSE` & `htagweb-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `htagweb-0.0.2/README.md` & `htagweb-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `htagweb-0.0.2/htagweb/__init__.py` & `htagweb-0.0.3/htagweb/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,21 @@
 # Copyright (C) 2023 manatlan manatlan[at]gmail(dot)com
 #
 # MIT licence
 #
 # https://github.com/manatlan/htag
 # #############################################################################
 
-__version__ = "0.0.2" # auto updated
+__version__ = "0.0.3" # auto updated
+
+try:
+    import uvloop
+    raise Exception("htagweb is not compatible with uvloop, yet")
+except ImportError:
+    pass
 
 """
 WebServer & WebServerWS
 ~~~~~~~~~~~~~~~~~~~~~~~~
 - new versions of oldest WebHTTP & WebWS (nearly compatibles)
 - concept of an htag app application server (manager), which communicate with child process, with queue (web workers communicate with the manager using tcp socket)
 - Htag App runned in its own process, per user (real isolation!)
@@ -105,15 +111,19 @@
                 headers.append("Set-Cookie", header_value)
             await send(message)
 
         await self.app(scope, receive, send_wrapper)
 
 #=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=
 def startManager(port,timeout): #sec (timeout session)
-    Manager(port).run(timeout)
+    try:
+        Manager(port).run(timeout)
+        print("Manager started!")
+    except Exception as e:
+        print("Manager can't started (already running?)")
 #=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=
 
 
 class ManagerClient:
     def __init__(self,port):
         self.port=port
 
@@ -171,15 +181,18 @@
         self.manager = ManagerClient(port)
 
         async def _startManager():
             import multiprocessing
             p = multiprocessing.Process(target=startManager,args=(port,timeout,),name="ManagerServer")
             p.start()
 
-        Starlette.__init__(self,debug=True, on_startup=[_startManager,],routes=routes)
+        async def _stopManager():
+            await self.manager.shutdown()
+
+        Starlette.__init__(self,debug=True, on_startup=[_startManager,],on_shutdown=[_stopManager],routes=routes)
 
         if obj:
             async def handleHome(request):
                 return await self.serve(request,obj)
             self.add_route( '/', handleHome )
 
         Starlette.add_middleware(self,WebServerSession )
```

### Comparing `htagweb-0.0.2/htagweb/crypto.py` & `htagweb-0.0.3/htagweb/crypto.py`

 * *Files identical despite different names*

### Comparing `htagweb-0.0.2/htagweb/manager.py` & `htagweb-0.0.3/htagweb/manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -249,24 +249,29 @@
                 self.seskeeper(max)
 
 
         loop=asyncio.new_event_loop()
         asyncio.set_event_loop(loop)    # force a new loop ;'(
 
         try:
-            server = loop.run_until_complete( asyncio.start_server( handle_server, '127.0.0.1', self.port) )
+            servertask = asyncio.start_server( handle_server, '127.0.0.1', self.port)
+            loop.create_task( servertask )
 
             # one server started, so we can tun the sessions keeper
-            asyncio.ensure_future( loopSesKeeper(timeout) )
+            loop.create_task( loopSesKeeper(timeout) )
 
-            log('MANAGER SERVER Serving on {}'.format(server.sockets[0].getsockname()))
+            log('MANAGER SERVER Serving on {}'.format(self.port))
             loop.run_forever()
         except KeyboardInterrupt:
             pass
-        server.close()
+        finally:
+            loop.close()
+
+    async def shutdown(self):
+        print("TODO: IMPLEMENT MANAGER SHUTDOWN (it's running now!)")
 
     async def ht_render(self, uid:str,fqn:str,init_params,js:str, renew=False) -> str:
 
         appkey = hashlib.sha1(f"{fqn} {init_params} {js}".encode()).hexdigest()
 
         user=self.users.get_user(uid)
         if user:
```

### Comparing `htagweb-0.0.2/htagweb/shm.py` & `htagweb-0.0.3/htagweb/shm.py`

 * *Files identical despite different names*

### Comparing `htagweb-0.0.2/pyproject.toml` & `htagweb-0.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "htagweb"
-version = "0.0.2" # auto-updated
+version = "0.0.3" # auto-updated
 description = "It's a robust webserver (http/ws) for hosting htag apps on the web (a process by user)"
 authors = ["manatlan <manatlan@gmail.com>"]
 readme = 'README.md'
 license="MIT"
 keywords=['htag','webserver']
 homepage = "https://github.com/manatlan/htagweb"
 repository = "https://github.com/manatlan/htagweb"
```

### Comparing `htagweb-0.0.2/PKG-INFO` & `htagweb-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: htagweb
-Version: 0.0.2
+Version: 0.0.3
 Summary: It's a robust webserver (http/ws) for hosting htag apps on the web (a process by user)
 Home-page: https://github.com/manatlan/htagweb
 License: MIT
 Keywords: htag,webserver
 Author: manatlan
 Author-email: manatlan@gmail.com
 Requires-Python: >=3.8,<4.0
```

