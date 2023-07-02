# Comparing `tmp/rmy-0.1.3.tar.gz` & `tmp/rmy-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rmy-0.1.3.tar", max compression
+gzip compressed data, was "rmy-0.3.tar", max compression
```

## Comparing `rmy-0.1.3.tar` & `rmy-0.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    11357 2023-06-11 20:31:23.956812 rmy-0.1.3/LICENSE
--rw-r--r--   0        0        0      657 2023-06-26 21:06:30.806884 rmy-0.1.3/README.md
--rw-r--r--   0        0        0     1677 2023-07-02 10:33:04.456072 rmy-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      565 2023-07-02 10:18:27.214111 rmy-0.1.3/rmy/__init__.py
--rw-r--r--   0        0        0      740 2023-07-01 18:07:30.323702 rmy-0.1.3/rmy/abc.py
--rw-r--r--   0        0        0    13202 2023-07-02 10:06:53.386688 rmy-0.1.3/rmy/client_async.py
--rw-r--r--   0        0        0     2614 2023-07-02 09:57:00.022299 rmy-0.1.3/rmy/client_sync.py
--rw-r--r--   0        0        0     1327 2023-06-30 16:18:33.807606 rmy-0.1.3/rmy/common.py
--rw-r--r--   0        0        0     2588 2023-07-01 18:06:09.576974 rmy-0.1.3/rmy/connection.py
--rw-r--r--   0        0        0    10830 2023-07-02 10:09:15.894425 rmy-0.1.3/rmy/server.py
--rw-r--r--   0        0        0     1185 1970-01-01 00:00:00.000000 rmy-0.1.3/PKG-INFO
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

### Comparing `rmy-0.1.3/LICENSE` & `rmy-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `rmy-0.1.3/README.md` & `rmy-0.3/README.md`

 * *Files identical despite different names*

### Comparing `rmy-0.1.3/pyproject.toml` & `rmy-0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 relative_files = true
 
 [tool.coverage.report]
 show_missing = true
 
 [tool.poetry]
 name = "rmy"
-version = "0.1.3"
+version = "0.3"
 description = "Stateful rpc for Python"
 authors = ["fdv1 <francois@pytek.io>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4.0"
 anyio = "^3.7.0"
```

### Comparing `rmy-0.1.3/rmy/__init__.py` & `rmy-0.3/rmy/__init__.py`

 * *Files identical despite different names*

### Comparing `rmy-0.1.3/rmy/abc.py` & `rmy-0.3/rmy/abc.py`

 * *Files identical despite different names*

### Comparing `rmy-0.1.3/rmy/client_async.py` & `rmy-0.3/rmy/client_async.py`

 * *Files identical despite different names*

### Comparing `rmy-0.1.3/rmy/client_sync.py` & `rmy-0.3/rmy/client_sync.py`

 * *Files identical despite different names*

### Comparing `rmy-0.1.3/rmy/common.py` & `rmy-0.3/rmy/common.py`

 * *Files identical despite different names*

### Comparing `rmy-0.1.3/rmy/connection.py` & `rmy-0.3/rmy/connection.py`

 * *Files identical despite different names*

### Comparing `rmy-0.1.3/rmy/server.py` & `rmy-0.3/rmy/server.py`

 * *Files identical despite different names*

### Comparing `rmy-0.1.3/PKG-INFO` & `rmy-0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rmy
-Version: 0.1.3
+Version: 0.3
 Summary: Stateful rpc for Python
 Author: fdv1
 Author-email: francois@pytek.io
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

