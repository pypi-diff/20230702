# Comparing `tmp/htagweb-0.0.1.tar.gz` & `tmp/htagweb-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "htagweb-0.0.1.tar", max compression
+gzip compressed data, was "htagweb-0.0.2.tar", max compression
```

## Comparing `htagweb-0.0.1.tar` & `htagweb-0.0.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1065 2023-07-02 06:44:17.046130 htagweb-0.0.1/LICENSE
--rw-r--r--   0        0        0     2310 2023-07-02 06:44:17.046130 htagweb-0.0.1/README.md
--rw-r--r--   0        0        0    11216 2023-07-02 06:44:17.330134 htagweb-0.0.1/htagweb/__init__.py
--rw-r--r--   0        0        0     2519 2023-07-02 06:44:17.046130 htagweb-0.0.1/htagweb/crypto.py
--rw-r--r--   0        0        0    10511 2023-07-02 06:44:17.046130 htagweb-0.0.1/htagweb/manager.py
--rw-r--r--   0        0        0      625 2023-07-02 06:44:17.046130 htagweb-0.0.1/htagweb/shm.py
--rw-r--r--   0        0        0     1060 2023-07-02 06:44:17.330134 htagweb-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     3512 1970-01-01 00:00:00.000000 htagweb-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-07-02 11:23:30.832444 htagweb-0.0.2/LICENSE
+-rw-r--r--   0        0        0     2666 2023-07-02 11:23:30.832444 htagweb-0.0.2/README.md
+-rw-r--r--   0        0        0    11075 2023-07-02 11:23:31.112445 htagweb-0.0.2/htagweb/__init__.py
+-rw-r--r--   0        0        0     2519 2023-07-02 11:23:30.832444 htagweb-0.0.2/htagweb/crypto.py
+-rw-r--r--   0        0        0    10269 2023-07-02 11:23:30.832444 htagweb-0.0.2/htagweb/manager.py
+-rw-r--r--   0        0        0      625 2023-07-02 11:23:30.832444 htagweb-0.0.2/htagweb/shm.py
+-rw-r--r--   0        0        0     1085 2023-07-02 11:23:31.112445 htagweb-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     3868 1970-01-01 00:00:00.000000 htagweb-0.0.2/PKG-INFO
```

### Comparing `htagweb-0.0.1/LICENSE` & `htagweb-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `htagweb-0.0.1/README.md` & `htagweb-0.0.2/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 # htagweb
 
-## NOT READY
+[![Test](https://github.com/manatlan/htagweb/actions/workflows/on_commit_do_all_unittests.yml/badge.svg)](https://github.com/manatlan/htagweb/actions/workflows/on_commit_do_all_unittests.yml)
 
+<a href="https://pypi.org/project/htagweb/">
+    <img src="https://badge.fury.io/py/htagweb.svg?x" alt="Package version">
+</a>
 
+**IMPORTANT**: not compatible with **uvloop** !!!
 
 This "htagweb" module provides two htag's "runners":
 
  * WebServer     : for http only exchanges
- * WebServerWS   ! for http/ws exchanges (first rendering is on http)
+ * WebServerWS   : for http/ws exchanges (first rendering is on http)
 
 Theses runners are a lot more complete than the defaults ones (WebHTTP & WebWS, provided nativly with htag)
 If you want to expose your HTag apps on the web : **they are the only real/official solutions**.
 Theses are a lot robust and IRL tested.
 
  * based on [starlette](https://pypi.org/project/starlette/)
  * each htag app is runned in its own process, per user (real isolation!)
```

### Comparing `htagweb-0.0.1/htagweb/__init__.py` & `htagweb-0.0.2/htagweb/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Copyright (C) 2023 manatlan manatlan[at]gmail(dot)com
 #
 # MIT licence
 #
 # https://github.com/manatlan/htag
 # #############################################################################
 
-__version__ = "0.0.1" # auto updated
+__version__ = "0.0.2" # auto updated
 
 """
 WebServer & WebServerWS
 ~~~~~~~~~~~~~~~~~~~~~~~~
 - new versions of oldest WebHTTP & WebWS (nearly compatibles)
 - concept of an htag app application server (manager), which communicate with child process, with queue (web workers communicate with the manager using tcp socket)
 - Htag App runned in its own process, per user (real isolation!)
@@ -102,23 +102,18 @@
                     max_age=f"Max-Age={self.max_age}; " if self.max_age else "",
                     security_flags=self.security_flags,
                 )
                 headers.append("Set-Cookie", header_value)
             await send(message)
 
         await self.app(scope, receive, send_wrapper)
-#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=
 
+#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=
 def startManager(port,timeout): #sec (timeout session)
-    asyncio.set_event_loop(asyncio.new_event_loop())
-    try:
-        Manager(port).run(timeout)
-    except Exception as e:
-        print("ERROR, can't start Manager:",e)
-
+    Manager(port).run(timeout)
 #=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=#=
 
 
 class ManagerClient:
     def __init__(self,port):
         self.port=port
```

### Comparing `htagweb-0.0.1/htagweb/crypto.py` & `htagweb-0.0.2/htagweb/crypto.py`

 * *Files identical despite different names*

### Comparing `htagweb-0.0.1/htagweb/manager.py` & `htagweb-0.0.2/htagweb/manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -245,25 +245,16 @@
 
         async def loopSesKeeper(max):
             while 1:
                 await asyncio.sleep(60) # check sessions every minute
                 self.seskeeper(max)
 
 
-        # https://stackoverflow.com/a/73884759/1284499
-        if sys.version_info < (3, 10):
-            loop = asyncio.get_event_loop()
-        else:
-            try:
-                loop = asyncio.get_running_loop()
-            except RuntimeError:
-                loop = asyncio.new_event_loop()
-
-            asyncio.set_event_loop(loop)
-
+        loop=asyncio.new_event_loop()
+        asyncio.set_event_loop(loop)    # force a new loop ;'(
 
         try:
             server = loop.run_until_complete( asyncio.start_server( handle_server, '127.0.0.1', self.port) )
 
             # one server started, so we can tun the sessions keeper
             asyncio.ensure_future( loopSesKeeper(timeout) )
```

### Comparing `htagweb-0.0.1/htagweb/shm.py` & `htagweb-0.0.2/htagweb/shm.py`

 * *Files identical despite different names*

### Comparing `htagweb-0.0.1/pyproject.toml` & `htagweb-0.0.2/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "htagweb"
-version = "0.0.1" # auto-updated
+version = "0.0.2" # auto-updated
 description = "It's a robust webserver (http/ws) for hosting htag apps on the web (a process by user)"
 authors = ["manatlan <manatlan@gmail.com>"]
 readme = 'README.md'
 license="MIT"
 keywords=['htag','webserver']
 homepage = "https://github.com/manatlan/htagweb"
 repository = "https://github.com/manatlan/htagweb"
@@ -22,13 +22,14 @@
 htag = ">= 0.9.44"
 starlette = ">= 0.21.0"
 uvicorn = ">= 0.22.0"
 pycryptodomex = ">= 3.0.0"
 shared_memory_dict = ">= 0.7.2"
 
 [tool.poetry.dev-dependencies]
-pytest = "^3.0"
-pytest-cov = "^2.6"
+pytest = "^7.0"
+pytest-cov = "^4.1"
+pytest-asyncio = "^0.21"
 
 [build-system]
 requires = ["poetry>=0.12"]
 build-backend = "poetry.masonry.api"
```

### Comparing `htagweb-0.0.1/PKG-INFO` & `htagweb-0.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: htagweb
-Version: 0.0.1
+Version: 0.0.2
 Summary: It's a robust webserver (http/ws) for hosting htag apps on the web (a process by user)
 Home-page: https://github.com/manatlan/htagweb
 License: MIT
 Keywords: htag,webserver
 Author: manatlan
 Author-email: manatlan@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -25,22 +25,26 @@
 Requires-Dist: uvicorn (>=0.22.0)
 Project-URL: Documentation, https://github.com/manatlan/htagweb
 Project-URL: Repository, https://github.com/manatlan/htagweb
 Description-Content-Type: text/markdown
 
 # htagweb
 
-## NOT READY
+[![Test](https://github.com/manatlan/htagweb/actions/workflows/on_commit_do_all_unittests.yml/badge.svg)](https://github.com/manatlan/htagweb/actions/workflows/on_commit_do_all_unittests.yml)
 
+<a href="https://pypi.org/project/htagweb/">
+    <img src="https://badge.fury.io/py/htagweb.svg?x" alt="Package version">
+</a>
 
+**IMPORTANT**: not compatible with **uvloop** !!!
 
 This "htagweb" module provides two htag's "runners":
 
  * WebServer     : for http only exchanges
- * WebServerWS   ! for http/ws exchanges (first rendering is on http)
+ * WebServerWS   : for http/ws exchanges (first rendering is on http)
 
 Theses runners are a lot more complete than the defaults ones (WebHTTP & WebWS, provided nativly with htag)
 If you want to expose your HTag apps on the web : **they are the only real/official solutions**.
 Theses are a lot robust and IRL tested.
 
  * based on [starlette](https://pypi.org/project/starlette/)
  * each htag app is runned in its own process, per user (real isolation!)
```

