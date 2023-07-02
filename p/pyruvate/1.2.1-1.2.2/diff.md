# Comparing `tmp/pyruvate-1.2.1.tar.gz` & `tmp/pyruvate-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyruvate-1.2.1.tar", last modified: Thu Dec 22 10:09:35 2022, max compression
+gzip compressed data, was "pyruvate-1.2.2.tar", last modified: Sun Jul  2 17:45:11 2023, max compression
```

## Comparing `pyruvate-1.2.1.tar` & `pyruvate-1.2.2.tar`

### file list

```diff
@@ -1,34 +1,39 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-22 10:09:35.007748 pyruvate-1.2.1/
--rw-rw-rw-   0 root         (0) root         (0)     5218 2022-12-22 10:05:03.000000 pyruvate-1.2.1/CHANGES.rst
--rw-rw-rw-   0 root         (0) root         (0)     1888 2022-12-22 10:05:03.000000 pyruvate-1.2.1/CONTRIBUTING.rst
--rw-rw-rw-   0 root         (0) root         (0)      733 2022-12-22 10:05:03.000000 pyruvate-1.2.1/Cargo.toml
--rw-rw-rw-   0 root         (0) root         (0)    18092 2022-12-22 10:05:03.000000 pyruvate-1.2.1/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       88 2022-12-22 10:05:03.000000 pyruvate-1.2.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    15461 2022-12-22 10:09:35.007748 pyruvate-1.2.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     9081 2022-12-22 10:05:03.000000 pyruvate-1.2.1/README.rst
--rw-rw-rw-   0 root         (0) root         (0)       69 2022-12-22 10:05:03.000000 pyruvate-1.2.1/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-22 10:09:34.998748 pyruvate-1.2.1/pyruvate/
--rw-rw-rw-   0 root         (0) root         (0)      946 2022-12-22 10:05:03.000000 pyruvate-1.2.1/pyruvate/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-22 10:09:35.002748 pyruvate-1.2.1/pyruvate.egg-info/
--rw-r--r--   0 root         (0) root         (0)    15461 2022-12-22 10:09:34.000000 pyruvate-1.2.1/pyruvate.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      532 2022-12-22 10:09:34.000000 pyruvate-1.2.1/pyruvate.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-12-22 10:09:34.000000 pyruvate-1.2.1/pyruvate.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       50 2022-12-22 10:09:34.000000 pyruvate-1.2.1/pyruvate.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-12-22 10:09:18.000000 pyruvate-1.2.1/pyruvate.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       47 2022-12-22 10:09:34.000000 pyruvate-1.2.1/pyruvate.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2022-12-22 10:09:34.000000 pyruvate-1.2.1/pyruvate.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-12-22 10:09:35.007748 pyruvate-1.2.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1950 2022-12-22 10:05:03.000000 pyruvate-1.2.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-22 10:09:35.006748 pyruvate-1.2.1/src/
--rw-rw-rw-   0 root         (0) root         (0)    20455 2022-12-22 10:05:03.000000 pyruvate-1.2.1/src/filewrapper.rs
--rw-rw-rw-   0 root         (0) root         (0)     4673 2022-12-22 10:05:03.000000 pyruvate-1.2.1/src/globals.rs
--rw-rw-rw-   0 root         (0) root         (0)      341 2022-12-22 10:05:03.000000 pyruvate-1.2.1/src/lib.rs
--rw-rw-rw-   0 root         (0) root         (0)     6844 2022-12-22 10:05:03.000000 pyruvate-1.2.1/src/pymodule.rs
--rw-rw-rw-   0 root         (0) root         (0)    22488 2022-12-22 10:05:03.000000 pyruvate-1.2.1/src/pyutils.rs
--rw-rw-rw-   0 root         (0) root         (0)    33261 2022-12-22 10:05:03.000000 pyruvate-1.2.1/src/request.rs
--rw-rw-rw-   0 root         (0) root         (0)    60574 2022-12-22 10:05:03.000000 pyruvate-1.2.1/src/response.rs
--rw-rw-rw-   0 root         (0) root         (0)    26626 2022-12-22 10:05:03.000000 pyruvate-1.2.1/src/server.rs
--rw-rw-rw-   0 root         (0) root         (0)    13699 2022-12-22 10:05:03.000000 pyruvate-1.2.1/src/startresponse.rs
--rw-rw-rw-   0 root         (0) root         (0)    22181 2022-12-22 10:05:03.000000 pyruvate-1.2.1/src/transport.rs
--rw-rw-rw-   0 root         (0) root         (0)     6789 2022-12-22 10:05:03.000000 pyruvate-1.2.1/src/workerpool.rs
--rw-rw-rw-   0 root         (0) root         (0)    24574 2022-12-22 10:05:03.000000 pyruvate-1.2.1/src/workers.rs
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 17:45:11.544105 pyruvate-1.2.2/
+-rw-rw-rw-   0 root         (0) root         (0)     5452 2023-07-02 17:39:43.000000 pyruvate-1.2.2/CHANGES.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1888 2023-07-02 17:39:43.000000 pyruvate-1.2.2/CONTRIBUTING.rst
+-rw-rw-rw-   0 root         (0) root         (0)      750 2023-07-02 17:39:43.000000 pyruvate-1.2.2/Cargo.toml
+-rw-rw-rw-   0 root         (0) root         (0)    18092 2023-07-02 17:39:43.000000 pyruvate-1.2.2/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       88 2023-07-02 17:39:43.000000 pyruvate-1.2.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    16340 2023-07-02 17:45:11.543105 pyruvate-1.2.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     9689 2023-07-02 17:39:43.000000 pyruvate-1.2.2/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)       69 2023-07-02 17:39:43.000000 pyruvate-1.2.2/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 17:45:11.538105 pyruvate-1.2.2/pyruvate/
+-rw-rw-rw-   0 root         (0) root         (0)      946 2023-07-02 17:39:43.000000 pyruvate-1.2.2/pyruvate/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 17:45:11.540105 pyruvate-1.2.2/pyruvate.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    16340 2023-07-02 17:45:11.000000 pyruvate-1.2.2/pyruvate.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      639 2023-07-02 17:45:11.000000 pyruvate-1.2.2/pyruvate.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-02 17:45:11.000000 pyruvate-1.2.2/pyruvate.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       50 2023-07-02 17:45:11.000000 pyruvate-1.2.2/pyruvate.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-02 17:45:02.000000 pyruvate-1.2.2/pyruvate.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       47 2023-07-02 17:45:11.000000 pyruvate-1.2.2/pyruvate.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-07-02 17:45:11.000000 pyruvate-1.2.2/pyruvate.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-02 17:45:11.544105 pyruvate-1.2.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1998 2023-07-02 17:39:43.000000 pyruvate-1.2.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 17:45:11.542106 pyruvate-1.2.2/src/
+-rw-rw-rw-   0 root         (0) root         (0)    20455 2023-07-02 17:39:43.000000 pyruvate-1.2.2/src/filewrapper.rs
+-rw-rw-rw-   0 root         (0) root         (0)     4673 2023-07-02 17:39:43.000000 pyruvate-1.2.2/src/globals.rs
+-rw-rw-rw-   0 root         (0) root         (0)      341 2023-07-02 17:39:43.000000 pyruvate-1.2.2/src/lib.rs
+-rw-rw-rw-   0 root         (0) root         (0)     6844 2023-07-02 17:39:43.000000 pyruvate-1.2.2/src/pymodule.rs
+-rw-rw-rw-   0 root         (0) root         (0)    22488 2023-07-02 17:39:43.000000 pyruvate-1.2.2/src/pyutils.rs
+-rw-rw-rw-   0 root         (0) root         (0)    33261 2023-07-02 17:39:43.000000 pyruvate-1.2.2/src/request.rs
+-rw-rw-rw-   0 root         (0) root         (0)    60574 2023-07-02 17:39:43.000000 pyruvate-1.2.2/src/response.rs
+-rw-rw-rw-   0 root         (0) root         (0)    26626 2023-07-02 17:39:43.000000 pyruvate-1.2.2/src/server.rs
+-rw-rw-rw-   0 root         (0) root         (0)    13699 2023-07-02 17:39:43.000000 pyruvate-1.2.2/src/startresponse.rs
+-rw-rw-rw-   0 root         (0) root         (0)    22181 2023-07-02 17:39:43.000000 pyruvate-1.2.2/src/transport.rs
+-rw-rw-rw-   0 root         (0) root         (0)     6789 2023-07-02 17:39:43.000000 pyruvate-1.2.2/src/workerpool.rs
+-rw-rw-rw-   0 root         (0) root         (0)    24574 2023-07-02 17:39:43.000000 pyruvate-1.2.2/src/workers.rs
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 17:45:11.543105 pyruvate-1.2.2/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     3513 2023-07-02 17:39:43.000000 pyruvate-1.2.2/tests/test_filewrapper.py
+-rw-rw-rw-   0 root         (0) root         (0)     4623 2023-07-02 17:39:43.000000 pyruvate-1.2.2/tests/test_headers.py
+-rw-rw-rw-   0 root         (0) root         (0)     2035 2023-07-02 17:39:43.000000 pyruvate-1.2.2/tests/test_request_queue_monitor.py
+-rw-rw-rw-   0 root         (0) root         (0)     1270 2023-07-02 17:39:43.000000 pyruvate-1.2.2/tests/test_validate.py
```

### Comparing `pyruvate-1.2.1/CHANGES.rst` & `pyruvate-1.2.2/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 Changelog
 =========
 
+1.2.2 (2023-07-02)
+------------------
+
+* Document Unix Domain Socket usage (`#27 <https://gitlab.com/tschorr/pyruvate/-/issues/27>`_)
+* Provide legacy manylinux wheel names (`#26 <https://gitlab.com/tschorr/pyruvate/-/issues/26>`_) 
+
 1.2.1 (2022-12-22)
 ------------------
 
 * Track and remove unfinished responses that did not otherwise error (`#23 <https://gitlab.com/tschorr/pyruvate/-/issues/23>`_)
 * Build musllinux_1_1 wheels (`#24 <https://gitlab.com/tschorr/pyruvate/-/issues/24>`_)
 
 1.2.0 (2022-10-26)
```

### Comparing `pyruvate-1.2.1/CONTRIBUTING.rst` & `pyruvate-1.2.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pyruvate-1.2.1/Cargo.toml` & `pyruvate-1.2.2/Cargo.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "pyruvate"
-version = "1.2.1"
+version = "1.2.2"
 authors = ["tschorr <t_schorr@gmx.de>"]
 edition = "2021"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 
 [lib]
 name = "pyruvate"
@@ -13,14 +13,15 @@
 [dependencies]
 cfg-if = "*"
 cpython = "*"
 crossbeam = "*"
 crossbeam-channel = "*"
 encoding = "*"
 errno = "*"
+grcov = "0.8.18"
 httparse = "*"
 libc = "*"
 log = { version="*", features=["std"] }
 mio = { version="*", features=["os-poll", "net"] }
 nix = "*"
 python3-sys = "*"
 signal-hook = "*"
```

### Comparing `pyruvate-1.2.1/LICENSE` & `pyruvate-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyruvate-1.2.1/PKG-INFO` & `pyruvate-1.2.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyruvate
-Version: 1.2.1
+Version: 1.2.2
 Summary: WSGI server implemented in Rust.
 Home-page: https://gitlab.com/tschorr/pyruvate
 Author: tschorr
 Author-email: t_schorr@gmx.de
 Keywords: WSGI
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
@@ -20,14 +20,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Rust
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Server
+Description-Content-Type: text/x-rst
 Provides-Extra: test
 License-File: LICENSE
 
 Pyruvate WSGI server
 ====================
 
 .. image:: https://gitlab.com/tschorr/pyruvate/badges/main/pipeline.svg
@@ -83,16 +84,16 @@
 * Install Pyruvate, e.g. using pip::
 
     $ pip install -e git+https://gitlab.com/tschorr/pyruvate.git#egg=pyruvate[test]
 
 Using Pyruvate in your WSGI application
 ---------------------------------------
 
-From Python
-+++++++++++
+From Python using a TCP port
+++++++++++++++++++++++++++++
 
 A hello world WSGI application using Pyruvate listening on 127.0.0.1:7878 and using 2 worker threads looks like this:
 
 .. code-block:: python
 
     import pyruvate
 
@@ -101,14 +102,32 @@
         status = '200 OK'
         response_headers = [('Content-type', 'text/plain')]
         start_response(status, response_headers, None)
         return [b"Hello world!\n"]
 
     pyruvate.serve(application, "127.0.0.1:7878", 2)
 
+From Python using a Unix socket
++++++++++++++++++++++++++++++++
+
+A hello world WSGI application using Pyruvate listening on unix:/tmp/pyruvate.socket and using 2 worker threads looks like this:
+
+.. code-block:: python
+
+    import pyruvate
+
+    def application(environ, start_response):
+        """Simplest possible application object"""
+        status = '200 OK'
+        response_headers = [('Content-type', 'text/plain')]
+        start_response(status, response_headers, None)
+        return [b"Hello world!\n"]
+
+    pyruvate.serve(application, "/tmp/pyruvate.socket", 2)
+
 Using PasteDeploy
 +++++++++++++++++
 
 Again listening on 127.0.0.1:7878 and using 2 worker threads::
 
     [server:main]
     use = egg:pyruvate#main
@@ -296,14 +315,20 @@
 
 Nginx doesn't use keepalive connections by default so you will need to `modify your configuration <https://nginx.org/en/docs/http/ngx_http_upstream_module.html#keepalive>`_ if you want persistent connections.
 
 
 Changelog
 =========
 
+1.2.2 (2023-07-02)
+------------------
+
+* Document Unix Domain Socket usage (`#27 <https://gitlab.com/tschorr/pyruvate/-/issues/27>`_)
+* Provide legacy manylinux wheel names (`#26 <https://gitlab.com/tschorr/pyruvate/-/issues/26>`_) 
+
 1.2.1 (2022-12-22)
 ------------------
 
 * Track and remove unfinished responses that did not otherwise error (`#23 <https://gitlab.com/tschorr/pyruvate/-/issues/23>`_)
 * Build musllinux_1_1 wheels (`#24 <https://gitlab.com/tschorr/pyruvate/-/issues/24>`_)
 
 1.2.0 (2022-10-26)
```

### Comparing `pyruvate-1.2.1/README.rst` & `pyruvate-1.2.2/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -54,16 +54,16 @@
 * Install Pyruvate, e.g. using pip::
 
     $ pip install -e git+https://gitlab.com/tschorr/pyruvate.git#egg=pyruvate[test]
 
 Using Pyruvate in your WSGI application
 ---------------------------------------
 
-From Python
-+++++++++++
+From Python using a TCP port
+++++++++++++++++++++++++++++
 
 A hello world WSGI application using Pyruvate listening on 127.0.0.1:7878 and using 2 worker threads looks like this:
 
 .. code-block:: python
 
     import pyruvate
 
@@ -72,14 +72,32 @@
         status = '200 OK'
         response_headers = [('Content-type', 'text/plain')]
         start_response(status, response_headers, None)
         return [b"Hello world!\n"]
 
     pyruvate.serve(application, "127.0.0.1:7878", 2)
 
+From Python using a Unix socket
++++++++++++++++++++++++++++++++
+
+A hello world WSGI application using Pyruvate listening on unix:/tmp/pyruvate.socket and using 2 worker threads looks like this:
+
+.. code-block:: python
+
+    import pyruvate
+
+    def application(environ, start_response):
+        """Simplest possible application object"""
+        status = '200 OK'
+        response_headers = [('Content-type', 'text/plain')]
+        start_response(status, response_headers, None)
+        return [b"Hello world!\n"]
+
+    pyruvate.serve(application, "/tmp/pyruvate.socket", 2)
+
 Using PasteDeploy
 +++++++++++++++++
 
 Again listening on 127.0.0.1:7878 and using 2 worker threads::
 
     [server:main]
     use = egg:pyruvate#main
```

### Comparing `pyruvate-1.2.1/pyruvate/__init__.py` & `pyruvate-1.2.2/pyruvate/__init__.py`

 * *Files identical despite different names*

### Comparing `pyruvate-1.2.1/pyruvate.egg-info/PKG-INFO` & `pyruvate-1.2.2/pyruvate.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyruvate
-Version: 1.2.1
+Version: 1.2.2
 Summary: WSGI server implemented in Rust.
 Home-page: https://gitlab.com/tschorr/pyruvate
 Author: tschorr
 Author-email: t_schorr@gmx.de
 Keywords: WSGI
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
@@ -20,14 +20,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Rust
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Server
+Description-Content-Type: text/x-rst
 Provides-Extra: test
 License-File: LICENSE
 
 Pyruvate WSGI server
 ====================
 
 .. image:: https://gitlab.com/tschorr/pyruvate/badges/main/pipeline.svg
@@ -83,16 +84,16 @@
 * Install Pyruvate, e.g. using pip::
 
     $ pip install -e git+https://gitlab.com/tschorr/pyruvate.git#egg=pyruvate[test]
 
 Using Pyruvate in your WSGI application
 ---------------------------------------
 
-From Python
-+++++++++++
+From Python using a TCP port
+++++++++++++++++++++++++++++
 
 A hello world WSGI application using Pyruvate listening on 127.0.0.1:7878 and using 2 worker threads looks like this:
 
 .. code-block:: python
 
     import pyruvate
 
@@ -101,14 +102,32 @@
         status = '200 OK'
         response_headers = [('Content-type', 'text/plain')]
         start_response(status, response_headers, None)
         return [b"Hello world!\n"]
 
     pyruvate.serve(application, "127.0.0.1:7878", 2)
 
+From Python using a Unix socket
++++++++++++++++++++++++++++++++
+
+A hello world WSGI application using Pyruvate listening on unix:/tmp/pyruvate.socket and using 2 worker threads looks like this:
+
+.. code-block:: python
+
+    import pyruvate
+
+    def application(environ, start_response):
+        """Simplest possible application object"""
+        status = '200 OK'
+        response_headers = [('Content-type', 'text/plain')]
+        start_response(status, response_headers, None)
+        return [b"Hello world!\n"]
+
+    pyruvate.serve(application, "/tmp/pyruvate.socket", 2)
+
 Using PasteDeploy
 +++++++++++++++++
 
 Again listening on 127.0.0.1:7878 and using 2 worker threads::
 
     [server:main]
     use = egg:pyruvate#main
@@ -296,14 +315,20 @@
 
 Nginx doesn't use keepalive connections by default so you will need to `modify your configuration <https://nginx.org/en/docs/http/ngx_http_upstream_module.html#keepalive>`_ if you want persistent connections.
 
 
 Changelog
 =========
 
+1.2.2 (2023-07-02)
+------------------
+
+* Document Unix Domain Socket usage (`#27 <https://gitlab.com/tschorr/pyruvate/-/issues/27>`_)
+* Provide legacy manylinux wheel names (`#26 <https://gitlab.com/tschorr/pyruvate/-/issues/26>`_) 
+
 1.2.1 (2022-12-22)
 ------------------
 
 * Track and remove unfinished responses that did not otherwise error (`#23 <https://gitlab.com/tschorr/pyruvate/-/issues/23>`_)
 * Build musllinux_1_1 wheels (`#24 <https://gitlab.com/tschorr/pyruvate/-/issues/24>`_)
 
 1.2.0 (2022-10-26)
```

### Comparing `pyruvate-1.2.1/pyruvate.egg-info/SOURCES.txt` & `pyruvate-1.2.2/pyruvate.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -21,8 +21,12 @@
 src/pyutils.rs
 src/request.rs
 src/response.rs
 src/server.rs
 src/startresponse.rs
 src/transport.rs
 src/workerpool.rs
-src/workers.rs
+src/workers.rs
+tests/test_filewrapper.py
+tests/test_headers.py
+tests/test_request_queue_monitor.py
+tests/test_validate.py
```

### Comparing `pyruvate-1.2.1/setup.py` & `pyruvate-1.2.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,17 +6,18 @@
     open('README.rst').read(),
     open('CHANGES.rst').read(),
 ])
 
 
 setup(
     name="pyruvate",
-    version="1.2.1",
+    version="1.2.2",
     description="WSGI server implemented in Rust.",
     long_description=long_description,
+    long_description_content_type='text/x-rst',
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Web Environment",
         "Intended Audience :: Developers",
         "Operating System :: POSIX :: Linux",
         "Operating System :: MacOS",
         "Programming Language :: Python",
```

### Comparing `pyruvate-1.2.1/src/filewrapper.rs` & `pyruvate-1.2.2/src/filewrapper.rs`

 * *Files identical despite different names*

### Comparing `pyruvate-1.2.1/src/globals.rs` & `pyruvate-1.2.2/src/globals.rs`

 * *Files identical despite different names*

### Comparing `pyruvate-1.2.1/src/pymodule.rs` & `pyruvate-1.2.2/src/pymodule.rs`

 * *Files identical despite different names*

### Comparing `pyruvate-1.2.1/src/pyutils.rs` & `pyruvate-1.2.2/src/pyutils.rs`

 * *Files identical despite different names*

### Comparing `pyruvate-1.2.1/src/request.rs` & `pyruvate-1.2.2/src/request.rs`

 * *Files identical despite different names*

### Comparing `pyruvate-1.2.1/src/response.rs` & `pyruvate-1.2.2/src/response.rs`

 * *Files identical despite different names*

### Comparing `pyruvate-1.2.1/src/server.rs` & `pyruvate-1.2.2/src/server.rs`

 * *Files identical despite different names*

### Comparing `pyruvate-1.2.1/src/startresponse.rs` & `pyruvate-1.2.2/src/startresponse.rs`

 * *Files identical despite different names*

### Comparing `pyruvate-1.2.1/src/transport.rs` & `pyruvate-1.2.2/src/transport.rs`

 * *Files identical despite different names*

### Comparing `pyruvate-1.2.1/src/workerpool.rs` & `pyruvate-1.2.2/src/workerpool.rs`

 * *Files identical despite different names*

### Comparing `pyruvate-1.2.1/src/workers.rs` & `pyruvate-1.2.2/src/workers.rs`

 * *Files identical despite different names*

