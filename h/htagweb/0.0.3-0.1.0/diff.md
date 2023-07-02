# Comparing `tmp/htagweb-0.0.3.tar.gz` & `tmp/htagweb-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "htagweb-0.0.3.tar", max compression
+gzip compressed data, was "htagweb-0.1.0.tar", max compression
```

## Comparing `htagweb-0.0.3.tar` & `htagweb-0.1.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1065 2023-07-02 14:30:33.700061 htagweb-0.0.3/LICENSE
--rw-r--r--   0        0        0     2666 2023-07-02 14:30:33.700061 htagweb-0.0.3/README.md
--rw-r--r--   0        0        0    11430 2023-07-02 14:30:34.004066 htagweb-0.0.3/htagweb/__init__.py
--rw-r--r--   0        0        0     2519 2023-07-02 14:30:33.700061 htagweb-0.0.3/htagweb/crypto.py
--rw-r--r--   0        0        0    10382 2023-07-02 14:30:33.700061 htagweb-0.0.3/htagweb/manager.py
--rw-r--r--   0        0        0      625 2023-07-02 14:30:33.700061 htagweb-0.0.3/htagweb/shm.py
--rw-r--r--   0        0        0     1085 2023-07-02 14:30:34.004066 htagweb-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     3868 1970-01-01 00:00:00.000000 htagweb-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-07-02 14:54:01.041032 htagweb-0.1.0/LICENSE
+-rw-r--r--   0        0        0     3028 2023-07-02 14:54:01.041032 htagweb-0.1.0/README.md
+-rw-r--r--   0        0        0    11430 2023-07-02 14:54:01.389034 htagweb-0.1.0/htagweb/__init__.py
+-rw-r--r--   0        0        0     2519 2023-07-02 14:54:01.041032 htagweb-0.1.0/htagweb/crypto.py
+-rw-r--r--   0        0        0    10365 2023-07-02 14:54:01.041032 htagweb-0.1.0/htagweb/manager.py
+-rw-r--r--   0        0        0      625 2023-07-02 14:54:01.041032 htagweb-0.1.0/htagweb/shm.py
+-rw-r--r--   0        0        0     1085 2023-07-02 14:54:01.389034 htagweb-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     4230 1970-01-01 00:00:00.000000 htagweb-0.1.0/PKG-INFO
```

### Comparing `htagweb-0.0.3/LICENSE` & `htagweb-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `htagweb-0.0.3/README.md` & `htagweb-0.1.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -31,16 +31,25 @@
 
 The concepts are the same :
 
  - one user can run only one instance(process) of an htag app at one time (like in desktop mode).
  - All user's instances(process) are destroyed, after an inactivity timeout (not like in desktop mode, to preserve healthy of the webserver)
  - the "session" live as long as the server live (may not be a problem on many hosting service (where they shutdown the server after inactivities))
 
+## Roadmap / futur
 
-----
+- make it uvloop compatible
+- better logging !!!!
+- graceful shutdown of the manager
+- more parameters (session size, etc ...)
+- parano mode
+- perhaps a bi-modal version (use ws, and fallback to http when ws com error)
+
+
+## Examples
 
 A "hello world" could be :
 
 ```python
 from htag import Tag
 
 class App(Tag.div):
@@ -66,8 +75,12 @@
 
 and run server :
 
 ```bash
 gunicorn -w 4 -k uvicorn.workers.UvicornH11Worker -b localhost:8000 --preload server:app
 ```
 
-See more in "examples" folder
+See a more advanced example in [examples folder](https://github.com/manatlan/htagweb/tree/master/examples)
+
+```bash
+python3 examples/main.py
+```
```

### Comparing `htagweb-0.0.3/htagweb/__init__.py` & `htagweb-0.1.0/htagweb/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Copyright (C) 2023 manatlan manatlan[at]gmail(dot)com
 #
 # MIT licence
 #
 # https://github.com/manatlan/htag
 # #############################################################################
 
-__version__ = "0.0.3" # auto updated
+__version__ = "0.1.0" # auto updated
 
 try:
     import uvloop
     raise Exception("htagweb is not compatible with uvloop, yet")
 except ImportError:
     pass
```

### Comparing `htagweb-0.0.3/htagweb/crypto.py` & `htagweb-0.1.0/htagweb/crypto.py`

 * *Files identical despite different names*

### Comparing `htagweb-0.0.3/htagweb/manager.py` & `htagweb-0.1.0/htagweb/manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -248,27 +248,24 @@
                 await asyncio.sleep(60) # check sessions every minute
                 self.seskeeper(max)
 
 
         loop=asyncio.new_event_loop()
         asyncio.set_event_loop(loop)    # force a new loop ;'(
 
+        server = loop.run_until_complete( asyncio.start_server( handle_server, '127.0.0.1', self.port) )
         try:
-            servertask = asyncio.start_server( handle_server, '127.0.0.1', self.port)
-            loop.create_task( servertask )
-
             # one server started, so we can tun the sessions keeper
-            loop.create_task( loopSesKeeper(timeout) )
+            asyncio.ensure_future( loopSesKeeper(timeout) )
 
-            log('MANAGER SERVER Serving on {}'.format(self.port))
+            log('MANAGER SERVER Serving on {}'.format(server.sockets[0].getsockname()))
             loop.run_forever()
         except KeyboardInterrupt:
             pass
-        finally:
-            loop.close()
+        server.close()
 
     async def shutdown(self):
         print("TODO: IMPLEMENT MANAGER SHUTDOWN (it's running now!)")
 
     async def ht_render(self, uid:str,fqn:str,init_params,js:str, renew=False) -> str:
 
         appkey = hashlib.sha1(f"{fqn} {init_params} {js}".encode()).hexdigest()
```

### Comparing `htagweb-0.0.3/htagweb/shm.py` & `htagweb-0.1.0/htagweb/shm.py`

 * *Files identical despite different names*

### Comparing `htagweb-0.0.3/pyproject.toml` & `htagweb-0.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "htagweb"
-version = "0.0.3" # auto-updated
+version = "0.1.0" # auto-updated
 description = "It's a robust webserver (http/ws) for hosting htag apps on the web (a process by user)"
 authors = ["manatlan <manatlan@gmail.com>"]
 readme = 'README.md'
 license="MIT"
 keywords=['htag','webserver']
 homepage = "https://github.com/manatlan/htagweb"
 repository = "https://github.com/manatlan/htagweb"
```

### Comparing `htagweb-0.0.3/PKG-INFO` & `htagweb-0.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: htagweb
-Version: 0.0.3
+Version: 0.1.0
 Summary: It's a robust webserver (http/ws) for hosting htag apps on the web (a process by user)
 Home-page: https://github.com/manatlan/htagweb
 License: MIT
 Keywords: htag,webserver
 Author: manatlan
 Author-email: manatlan@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -60,16 +60,25 @@
 
 The concepts are the same :
 
  - one user can run only one instance(process) of an htag app at one time (like in desktop mode).
  - All user's instances(process) are destroyed, after an inactivity timeout (not like in desktop mode, to preserve healthy of the webserver)
  - the "session" live as long as the server live (may not be a problem on many hosting service (where they shutdown the server after inactivities))
 
+## Roadmap / futur
 
-----
+- make it uvloop compatible
+- better logging !!!!
+- graceful shutdown of the manager
+- more parameters (session size, etc ...)
+- parano mode
+- perhaps a bi-modal version (use ws, and fallback to http when ws com error)
+
+
+## Examples
 
 A "hello world" could be :
 
 ```python
 from htag import Tag
 
 class App(Tag.div):
@@ -95,9 +104,13 @@
 
 and run server :
 
 ```bash
 gunicorn -w 4 -k uvicorn.workers.UvicornH11Worker -b localhost:8000 --preload server:app
 ```
 
-See more in "examples" folder
+See a more advanced example in [examples folder](https://github.com/manatlan/htagweb/tree/master/examples)
+
+```bash
+python3 examples/main.py
+```
```

