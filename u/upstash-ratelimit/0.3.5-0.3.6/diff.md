# Comparing `tmp/upstash_ratelimit-0.3.5.tar.gz` & `tmp/upstash_ratelimit-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "upstash_ratelimit-0.3.5.tar", max compression
+gzip compressed data, was "upstash_ratelimit-0.3.6.tar", max compression
```

## Comparing `upstash_ratelimit-0.3.5.tar` & `upstash_ratelimit-0.3.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1072 2023-07-02 16:58:47.297966 upstash_ratelimit-0.3.5/LICENSE
--rw-r--r--   0        0        0     7542 2023-07-02 16:58:47.297966 upstash_ratelimit-0.3.5/README.md
--rw-r--r--   0        0        0      475 2023-07-02 16:58:47.297966 upstash_ratelimit-0.3.5/pyproject.toml
--rw-r--r--   0        0        0       78 2023-07-02 16:58:47.301967 upstash_ratelimit-0.3.5/upstash_ratelimit/__init__.py
--rw-r--r--   0        0        0     1853 2023-07-02 16:58:47.301967 upstash_ratelimit-0.3.5/upstash_ratelimit/algorithms/algorithm.py
--rw-r--r--   0        0        0     3243 2023-07-02 16:58:47.301967 upstash_ratelimit-0.3.5/upstash_ratelimit/algorithms/fixed_window_core.py
--rw-r--r--   0        0        0     5777 2023-07-02 16:58:47.301967 upstash_ratelimit-0.3.5/upstash_ratelimit/algorithms/sliding_window_core.py
--rw-r--r--   0        0        0     5231 2023-07-02 16:58:47.301967 upstash_ratelimit-0.3.5/upstash_ratelimit/algorithms/token_bucket_core.py
--rw-r--r--   0        0        0       86 2023-07-02 16:58:47.301967 upstash_ratelimit-0.3.5/upstash_ratelimit/asyncio/__init__.py
--rw-r--r--   0        0        0     1161 2023-07-02 16:58:47.301967 upstash_ratelimit-0.3.5/upstash_ratelimit/asyncio/async_blocker.py
--rw-r--r--   0        0        0     2981 2023-07-02 16:58:47.301967 upstash_ratelimit-0.3.5/upstash_ratelimit/asyncio/fixed_window.py
--rw-r--r--   0        0        0     3506 2023-07-02 16:58:47.301967 upstash_ratelimit-0.3.5/upstash_ratelimit/asyncio/limiter.py
--rw-r--r--   0        0        0     3788 2023-07-02 16:58:47.301967 upstash_ratelimit-0.3.5/upstash_ratelimit/asyncio/sliding_window.py
--rw-r--r--   0        0        0     3399 2023-07-02 16:58:47.301967 upstash_ratelimit-0.3.5/upstash_ratelimit/asyncio/token_bucket.py
--rw-r--r--   0        0        0      172 2023-07-02 16:58:47.301967 upstash_ratelimit-0.3.5/upstash_ratelimit/config.py
--rw-r--r--   0        0        0     3489 2023-07-02 16:58:47.301967 upstash_ratelimit-0.3.5/upstash_ratelimit/limiter.py
--rw-r--r--   0        0        0        0 2023-07-02 16:58:47.301967 upstash_ratelimit-0.3.5/upstash_ratelimit/py.typed
--rw-r--r--   0        0        0      475 2023-07-02 16:58:47.301967 upstash_ratelimit-0.3.5/upstash_ratelimit/schema/response.py
--rw-r--r--   0        0        0     2824 2023-07-02 16:58:47.301967 upstash_ratelimit-0.3.5/upstash_ratelimit/sync/fixed_window.py
--rw-r--r--   0        0        0     3477 2023-07-02 16:58:47.301967 upstash_ratelimit-0.3.5/upstash_ratelimit/sync/sliding_window.py
--rw-r--r--   0        0        0     1111 2023-07-02 16:58:47.301967 upstash_ratelimit-0.3.5/upstash_ratelimit/sync/sync_blocker.py
--rw-r--r--   0        0        0     3185 2023-07-02 16:58:47.301967 upstash_ratelimit-0.3.5/upstash_ratelimit/sync/token_bucket.py
--rw-r--r--   0        0        0      392 2023-07-02 16:58:47.301967 upstash_ratelimit-0.3.5/upstash_ratelimit/utils/time.py
--rw-r--r--   0        0        0     8175 1970-01-01 00:00:00.000000 upstash_ratelimit-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-07-02 16:59:30.254577 upstash_ratelimit-0.3.6/LICENSE
+-rw-r--r--   0        0        0     7542 2023-07-02 16:59:30.254577 upstash_ratelimit-0.3.6/README.md
+-rw-r--r--   0        0        0      475 2023-07-02 16:59:30.258577 upstash_ratelimit-0.3.6/pyproject.toml
+-rw-r--r--   0        0        0       78 2023-07-02 16:59:30.258577 upstash_ratelimit-0.3.6/upstash_ratelimit/__init__.py
+-rw-r--r--   0        0        0     1853 2023-07-02 16:59:30.258577 upstash_ratelimit-0.3.6/upstash_ratelimit/algorithms/algorithm.py
+-rw-r--r--   0        0        0     3243 2023-07-02 16:59:30.258577 upstash_ratelimit-0.3.6/upstash_ratelimit/algorithms/fixed_window_core.py
+-rw-r--r--   0        0        0     5777 2023-07-02 16:59:30.258577 upstash_ratelimit-0.3.6/upstash_ratelimit/algorithms/sliding_window_core.py
+-rw-r--r--   0        0        0     5231 2023-07-02 16:59:30.258577 upstash_ratelimit-0.3.6/upstash_ratelimit/algorithms/token_bucket_core.py
+-rw-r--r--   0        0        0       86 2023-07-02 16:59:30.258577 upstash_ratelimit-0.3.6/upstash_ratelimit/asyncio/__init__.py
+-rw-r--r--   0        0        0     1161 2023-07-02 16:59:30.258577 upstash_ratelimit-0.3.6/upstash_ratelimit/asyncio/async_blocker.py
+-rw-r--r--   0        0        0     2981 2023-07-02 16:59:30.258577 upstash_ratelimit-0.3.6/upstash_ratelimit/asyncio/fixed_window.py
+-rw-r--r--   0        0        0     3506 2023-07-02 16:59:30.258577 upstash_ratelimit-0.3.6/upstash_ratelimit/asyncio/limiter.py
+-rw-r--r--   0        0        0     3788 2023-07-02 16:59:30.258577 upstash_ratelimit-0.3.6/upstash_ratelimit/asyncio/sliding_window.py
+-rw-r--r--   0        0        0     3399 2023-07-02 16:59:30.258577 upstash_ratelimit-0.3.6/upstash_ratelimit/asyncio/token_bucket.py
+-rw-r--r--   0        0        0      172 2023-07-02 16:59:30.258577 upstash_ratelimit-0.3.6/upstash_ratelimit/config.py
+-rw-r--r--   0        0        0     3489 2023-07-02 16:59:30.258577 upstash_ratelimit-0.3.6/upstash_ratelimit/limiter.py
+-rw-r--r--   0        0        0        0 2023-07-02 16:59:30.258577 upstash_ratelimit-0.3.6/upstash_ratelimit/py.typed
+-rw-r--r--   0        0        0      475 2023-07-02 16:59:30.262577 upstash_ratelimit-0.3.6/upstash_ratelimit/schema/response.py
+-rw-r--r--   0        0        0     2824 2023-07-02 16:59:30.262577 upstash_ratelimit-0.3.6/upstash_ratelimit/sync/fixed_window.py
+-rw-r--r--   0        0        0     3477 2023-07-02 16:59:30.262577 upstash_ratelimit-0.3.6/upstash_ratelimit/sync/sliding_window.py
+-rw-r--r--   0        0        0     1111 2023-07-02 16:59:30.262577 upstash_ratelimit-0.3.6/upstash_ratelimit/sync/sync_blocker.py
+-rw-r--r--   0        0        0     3185 2023-07-02 16:59:30.262577 upstash_ratelimit-0.3.6/upstash_ratelimit/sync/token_bucket.py
+-rw-r--r--   0        0        0      392 2023-07-02 16:59:30.262577 upstash_ratelimit-0.3.6/upstash_ratelimit/utils/time.py
+-rw-r--r--   0        0        0     8163 1970-01-01 00:00:00.000000 upstash_ratelimit-0.3.6/PKG-INFO
```

### Comparing `upstash_ratelimit-0.3.5/LICENSE` & `upstash_ratelimit-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `upstash_ratelimit-0.3.5/README.md` & `upstash_ratelimit-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `upstash_ratelimit-0.3.5/upstash_ratelimit/algorithms/algorithm.py` & `upstash_ratelimit-0.3.6/upstash_ratelimit/algorithms/algorithm.py`

 * *Files identical despite different names*

### Comparing `upstash_ratelimit-0.3.5/upstash_ratelimit/algorithms/fixed_window_core.py` & `upstash_ratelimit-0.3.6/upstash_ratelimit/algorithms/fixed_window_core.py`

 * *Files identical despite different names*

### Comparing `upstash_ratelimit-0.3.5/upstash_ratelimit/algorithms/sliding_window_core.py` & `upstash_ratelimit-0.3.6/upstash_ratelimit/algorithms/sliding_window_core.py`

 * *Files identical despite different names*

### Comparing `upstash_ratelimit-0.3.5/upstash_ratelimit/algorithms/token_bucket_core.py` & `upstash_ratelimit-0.3.6/upstash_ratelimit/algorithms/token_bucket_core.py`

 * *Files identical despite different names*

### Comparing `upstash_ratelimit-0.3.5/upstash_ratelimit/asyncio/async_blocker.py` & `upstash_ratelimit-0.3.6/upstash_ratelimit/asyncio/async_blocker.py`

 * *Files identical despite different names*

### Comparing `upstash_ratelimit-0.3.5/upstash_ratelimit/asyncio/fixed_window.py` & `upstash_ratelimit-0.3.6/upstash_ratelimit/asyncio/fixed_window.py`

 * *Files identical despite different names*

### Comparing `upstash_ratelimit-0.3.5/upstash_ratelimit/asyncio/limiter.py` & `upstash_ratelimit-0.3.6/upstash_ratelimit/asyncio/limiter.py`

 * *Files identical despite different names*

### Comparing `upstash_ratelimit-0.3.5/upstash_ratelimit/asyncio/sliding_window.py` & `upstash_ratelimit-0.3.6/upstash_ratelimit/asyncio/sliding_window.py`

 * *Files identical despite different names*

### Comparing `upstash_ratelimit-0.3.5/upstash_ratelimit/asyncio/token_bucket.py` & `upstash_ratelimit-0.3.6/upstash_ratelimit/asyncio/token_bucket.py`

 * *Files identical despite different names*

### Comparing `upstash_ratelimit-0.3.5/upstash_ratelimit/limiter.py` & `upstash_ratelimit-0.3.6/upstash_ratelimit/limiter.py`

 * *Files identical despite different names*

### Comparing `upstash_ratelimit-0.3.5/upstash_ratelimit/sync/fixed_window.py` & `upstash_ratelimit-0.3.6/upstash_ratelimit/sync/fixed_window.py`

 * *Files identical despite different names*

### Comparing `upstash_ratelimit-0.3.5/upstash_ratelimit/sync/sliding_window.py` & `upstash_ratelimit-0.3.6/upstash_ratelimit/sync/sliding_window.py`

 * *Files identical despite different names*

### Comparing `upstash_ratelimit-0.3.5/upstash_ratelimit/sync/sync_blocker.py` & `upstash_ratelimit-0.3.6/upstash_ratelimit/sync/sync_blocker.py`

 * *Files identical despite different names*

### Comparing `upstash_ratelimit-0.3.5/upstash_ratelimit/sync/token_bucket.py` & `upstash_ratelimit-0.3.6/upstash_ratelimit/sync/token_bucket.py`

 * *Files identical despite different names*

### Comparing `upstash_ratelimit-0.3.5/PKG-INFO` & `upstash_ratelimit-0.3.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: upstash-ratelimit
-Version: 0.3.5
+Version: 0.3.6
 Summary: Serverless ratelimiting package from Upstash
-Author: Zgîmbău Tudor
-Author-email: tudor.zgimbau@gmail.com
+Author: Upstash
+Author-email: support@upstash.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pytest (>=7.3.0,<8.0.0)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

