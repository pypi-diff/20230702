# Comparing `tmp/upstash_ratelimit-0.3.2.tar.gz` & `tmp/upstash_ratelimit-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "upstash_ratelimit-0.3.2.tar", max compression
+gzip compressed data, was "upstash_ratelimit-0.3.4.tar", max compression
```

## Comparing `upstash_ratelimit-0.3.2.tar` & `upstash_ratelimit-0.3.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1072 2023-07-02 12:33:15.080415 upstash_ratelimit-0.3.2/LICENSE
--rw-r--r--   0        0        0     7542 2023-07-02 12:33:15.080415 upstash_ratelimit-0.3.2/README.md
--rw-r--r--   0        0        0      475 2023-07-02 12:33:15.084415 upstash_ratelimit-0.3.2/pyproject.toml
--rw-r--r--   0        0        0       78 2023-07-02 12:33:15.084415 upstash_ratelimit-0.3.2/upstash_ratelimit/__init__.py
--rw-r--r--   0        0        0     1853 2023-07-02 12:33:15.084415 upstash_ratelimit-0.3.2/upstash_ratelimit/algorithms/algorithm.py
--rw-r--r--   0        0        0     3243 2023-07-02 12:33:15.084415 upstash_ratelimit-0.3.2/upstash_ratelimit/algorithms/fixed_window_core.py
--rw-r--r--   0        0        0     5777 2023-07-02 12:33:15.084415 upstash_ratelimit-0.3.2/upstash_ratelimit/algorithms/sliding_window_core.py
--rw-r--r--   0        0        0     5231 2023-07-02 12:33:15.084415 upstash_ratelimit-0.3.2/upstash_ratelimit/algorithms/token_bucket_core.py
--rw-r--r--   0        0        0       86 2023-07-02 12:33:15.084415 upstash_ratelimit-0.3.2/upstash_ratelimit/asyncio/__init__.py
--rw-r--r--   0        0        0     1161 2023-07-02 12:33:15.084415 upstash_ratelimit-0.3.2/upstash_ratelimit/asyncio/async_blocker.py
--rw-r--r--   0        0        0     2981 2023-07-02 12:33:15.084415 upstash_ratelimit-0.3.2/upstash_ratelimit/asyncio/fixed_window.py
--rw-r--r--   0        0        0     3506 2023-07-02 12:33:15.084415 upstash_ratelimit-0.3.2/upstash_ratelimit/asyncio/limiter.py
--rw-r--r--   0        0        0     3788 2023-07-02 12:33:15.084415 upstash_ratelimit-0.3.2/upstash_ratelimit/asyncio/sliding_window.py
--rw-r--r--   0        0        0     3399 2023-07-02 12:33:15.084415 upstash_ratelimit-0.3.2/upstash_ratelimit/asyncio/token_bucket.py
--rw-r--r--   0        0        0      172 2023-07-02 12:33:15.084415 upstash_ratelimit-0.3.2/upstash_ratelimit/config.py
--rw-r--r--   0        0        0     3489 2023-07-02 12:33:15.084415 upstash_ratelimit-0.3.2/upstash_ratelimit/limiter.py
--rw-r--r--   0        0        0        0 2023-07-02 12:33:15.084415 upstash_ratelimit-0.3.2/upstash_ratelimit/py.typed
--rw-r--r--   0        0        0      475 2023-07-02 12:33:15.084415 upstash_ratelimit-0.3.2/upstash_ratelimit/schema/response.py
--rw-r--r--   0        0        0     2824 2023-07-02 12:33:15.084415 upstash_ratelimit-0.3.2/upstash_ratelimit/sync/fixed_window.py
--rw-r--r--   0        0        0     3477 2023-07-02 12:33:15.084415 upstash_ratelimit-0.3.2/upstash_ratelimit/sync/sliding_window.py
--rw-r--r--   0        0        0     1111 2023-07-02 12:33:15.084415 upstash_ratelimit-0.3.2/upstash_ratelimit/sync/sync_blocker.py
--rw-r--r--   0        0        0     3185 2023-07-02 12:33:15.084415 upstash_ratelimit-0.3.2/upstash_ratelimit/sync/token_bucket.py
--rw-r--r--   0        0        0      392 2023-07-02 12:33:15.084415 upstash_ratelimit-0.3.2/upstash_ratelimit/utils/time.py
--rw-r--r--   0        0        0     8175 1970-01-01 00:00:00.000000 upstash_ratelimit-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-07-02 16:42:37.005036 upstash_ratelimit-0.3.4/LICENSE
+-rw-r--r--   0        0        0     7542 2023-07-02 16:42:37.005036 upstash_ratelimit-0.3.4/README.md
+-rw-r--r--   0        0        0      475 2023-07-02 16:42:37.005036 upstash_ratelimit-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0       78 2023-07-02 16:42:37.005036 upstash_ratelimit-0.3.4/upstash_ratelimit/__init__.py
+-rw-r--r--   0        0        0     1853 2023-07-02 16:42:37.005036 upstash_ratelimit-0.3.4/upstash_ratelimit/algorithms/algorithm.py
+-rw-r--r--   0        0        0     3243 2023-07-02 16:42:37.005036 upstash_ratelimit-0.3.4/upstash_ratelimit/algorithms/fixed_window_core.py
+-rw-r--r--   0        0        0     5777 2023-07-02 16:42:37.005036 upstash_ratelimit-0.3.4/upstash_ratelimit/algorithms/sliding_window_core.py
+-rw-r--r--   0        0        0     5231 2023-07-02 16:42:37.005036 upstash_ratelimit-0.3.4/upstash_ratelimit/algorithms/token_bucket_core.py
+-rw-r--r--   0        0        0       86 2023-07-02 16:42:37.005036 upstash_ratelimit-0.3.4/upstash_ratelimit/asyncio/__init__.py
+-rw-r--r--   0        0        0     1161 2023-07-02 16:42:37.005036 upstash_ratelimit-0.3.4/upstash_ratelimit/asyncio/async_blocker.py
+-rw-r--r--   0        0        0     2981 2023-07-02 16:42:37.005036 upstash_ratelimit-0.3.4/upstash_ratelimit/asyncio/fixed_window.py
+-rw-r--r--   0        0        0     3506 2023-07-02 16:42:37.005036 upstash_ratelimit-0.3.4/upstash_ratelimit/asyncio/limiter.py
+-rw-r--r--   0        0        0     3788 2023-07-02 16:42:37.005036 upstash_ratelimit-0.3.4/upstash_ratelimit/asyncio/sliding_window.py
+-rw-r--r--   0        0        0     3399 2023-07-02 16:42:37.005036 upstash_ratelimit-0.3.4/upstash_ratelimit/asyncio/token_bucket.py
+-rw-r--r--   0        0        0      172 2023-07-02 16:42:37.005036 upstash_ratelimit-0.3.4/upstash_ratelimit/config.py
+-rw-r--r--   0        0        0     3489 2023-07-02 16:42:37.005036 upstash_ratelimit-0.3.4/upstash_ratelimit/limiter.py
+-rw-r--r--   0        0        0        0 2023-07-02 16:42:37.005036 upstash_ratelimit-0.3.4/upstash_ratelimit/py.typed
+-rw-r--r--   0        0        0      475 2023-07-02 16:42:37.005036 upstash_ratelimit-0.3.4/upstash_ratelimit/schema/response.py
+-rw-r--r--   0        0        0     2824 2023-07-02 16:42:37.005036 upstash_ratelimit-0.3.4/upstash_ratelimit/sync/fixed_window.py
+-rw-r--r--   0        0        0     3477 2023-07-02 16:42:37.005036 upstash_ratelimit-0.3.4/upstash_ratelimit/sync/sliding_window.py
+-rw-r--r--   0        0        0     1111 2023-07-02 16:42:37.005036 upstash_ratelimit-0.3.4/upstash_ratelimit/sync/sync_blocker.py
+-rw-r--r--   0        0        0     3185 2023-07-02 16:42:37.005036 upstash_ratelimit-0.3.4/upstash_ratelimit/sync/token_bucket.py
+-rw-r--r--   0        0        0      392 2023-07-02 16:42:37.009036 upstash_ratelimit-0.3.4/upstash_ratelimit/utils/time.py
+-rw-r--r--   0        0        0     8175 1970-01-01 00:00:00.000000 upstash_ratelimit-0.3.4/PKG-INFO
```

### Comparing `upstash_ratelimit-0.3.2/LICENSE` & `upstash_ratelimit-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `upstash_ratelimit-0.3.2/README.md` & `upstash_ratelimit-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `upstash_ratelimit-0.3.2/upstash_ratelimit/algorithms/algorithm.py` & `upstash_ratelimit-0.3.4/upstash_ratelimit/algorithms/algorithm.py`

 * *Files identical despite different names*

### Comparing `upstash_ratelimit-0.3.2/upstash_ratelimit/algorithms/fixed_window_core.py` & `upstash_ratelimit-0.3.4/upstash_ratelimit/algorithms/fixed_window_core.py`

 * *Files identical despite different names*

### Comparing `upstash_ratelimit-0.3.2/upstash_ratelimit/algorithms/sliding_window_core.py` & `upstash_ratelimit-0.3.4/upstash_ratelimit/algorithms/sliding_window_core.py`

 * *Files identical despite different names*

### Comparing `upstash_ratelimit-0.3.2/upstash_ratelimit/algorithms/token_bucket_core.py` & `upstash_ratelimit-0.3.4/upstash_ratelimit/algorithms/token_bucket_core.py`

 * *Files identical despite different names*

### Comparing `upstash_ratelimit-0.3.2/upstash_ratelimit/asyncio/async_blocker.py` & `upstash_ratelimit-0.3.4/upstash_ratelimit/asyncio/async_blocker.py`

 * *Files identical despite different names*

### Comparing `upstash_ratelimit-0.3.2/upstash_ratelimit/asyncio/fixed_window.py` & `upstash_ratelimit-0.3.4/upstash_ratelimit/asyncio/fixed_window.py`

 * *Files identical despite different names*

### Comparing `upstash_ratelimit-0.3.2/upstash_ratelimit/asyncio/limiter.py` & `upstash_ratelimit-0.3.4/upstash_ratelimit/asyncio/limiter.py`

 * *Files identical despite different names*

### Comparing `upstash_ratelimit-0.3.2/upstash_ratelimit/asyncio/sliding_window.py` & `upstash_ratelimit-0.3.4/upstash_ratelimit/asyncio/sliding_window.py`

 * *Files identical despite different names*

### Comparing `upstash_ratelimit-0.3.2/upstash_ratelimit/asyncio/token_bucket.py` & `upstash_ratelimit-0.3.4/upstash_ratelimit/asyncio/token_bucket.py`

 * *Files identical despite different names*

### Comparing `upstash_ratelimit-0.3.2/upstash_ratelimit/limiter.py` & `upstash_ratelimit-0.3.4/upstash_ratelimit/limiter.py`

 * *Files identical despite different names*

### Comparing `upstash_ratelimit-0.3.2/upstash_ratelimit/sync/fixed_window.py` & `upstash_ratelimit-0.3.4/upstash_ratelimit/sync/fixed_window.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,15 +62,15 @@
 
     def reset(self, identifier: str) -> int:
         """
         Determine the unix time in milliseconds when the next window begins.
 
         If the identifier is not rate-limited, the returned value will be -1.
         """
-        exists = self.redis.exists(self.find_key(identifier)) != 1 # The identifier hasn't made any request in the current window.
+        exists = self.redis.exists(self.find_key(identifier)) == 1 # The identifier hasn't made any request in the current window.
 
         return super().reset(exists)
     
     def find_key(self, identifier: str) -> str:
         return f"{self.prefix}:{identifier}:{self.current_window}"
```

### Comparing `upstash_ratelimit-0.3.2/upstash_ratelimit/sync/sliding_window.py` & `upstash_ratelimit-0.3.4/upstash_ratelimit/sync/sliding_window.py`

 * *Files identical despite different names*

### Comparing `upstash_ratelimit-0.3.2/upstash_ratelimit/sync/sync_blocker.py` & `upstash_ratelimit-0.3.4/upstash_ratelimit/sync/sync_blocker.py`

 * *Files identical despite different names*

### Comparing `upstash_ratelimit-0.3.2/upstash_ratelimit/sync/token_bucket.py` & `upstash_ratelimit-0.3.4/upstash_ratelimit/sync/token_bucket.py`

 * *Files identical despite different names*

### Comparing `upstash_ratelimit-0.3.2/PKG-INFO` & `upstash_ratelimit-0.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: upstash-ratelimit
-Version: 0.3.2
+Version: 0.3.4
 Summary: Serverless ratelimiting package from Upstash
 Author: Zgîmbău Tudor
 Author-email: tudor.zgimbau@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pytest (>=7.3.0,<8.0.0)
 Requires-Dist: pytest-asyncio (>=0.21.0,<0.22.0)
-Requires-Dist: upstash-redis (>=0.13.0,<0.14.0)
+Requires-Dist: upstash-redis (>=0.13.2,<0.14.0)
 Description-Content-Type: text/markdown
 
 # Upstash Rate Limit - python edition
 
 upstash-ratelimit is a connectionless rate limiting library for python, designed to be used in serverless environments such as:
 - AWS Lambda
 - Vercel Serverless
```

