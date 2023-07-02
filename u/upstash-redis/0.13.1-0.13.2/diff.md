# Comparing `tmp/upstash_redis-0.13.1.tar.gz` & `tmp/upstash_redis-0.13.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "upstash_redis-0.13.1.tar", max compression
+gzip compressed data, was "upstash_redis-0.13.2.tar", max compression
```

## Comparing `upstash_redis-0.13.1.tar` & `upstash_redis-0.13.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     1070 2023-07-02 12:48:09.145678 upstash_redis-0.13.1/LICENSE
--rw-r--r--   0        0        0     9173 2023-07-02 12:48:09.145678 upstash_redis-0.13.1/README.md
--rw-r--r--   0        0        0      500 2023-07-02 12:48:09.145678 upstash_redis-0.13.1/pyproject.toml
--rw-r--r--   0        0        0      150 2023-07-02 12:48:09.149678 upstash_redis-0.13.1/upstash_redis/__init__.py
--rw-r--r--   0        0        0       68 2023-07-02 12:48:09.149678 upstash_redis-0.13.1/upstash_redis/asyncio/__init__.py
--rw-r--r--   0        0        0     4782 2023-07-02 12:48:09.149678 upstash_redis-0.13.1/upstash_redis/asyncio/client.py
--rw-r--r--   0        0        0     5052 2023-07-02 12:48:09.149678 upstash_redis-0.13.1/upstash_redis/client.py
--rw-r--r--   0        0        0       82 2023-07-02 12:48:09.149678 upstash_redis-0.13.1/upstash_redis/commands/__init__.py
--rw-r--r--   0        0        0       78 2023-07-02 12:48:09.153678 upstash_redis-0.13.1/upstash_redis/commands/async_commands.py
--rw-r--r--   0        0        0    22111 2023-07-02 12:48:09.153678 upstash_redis-0.13.1/upstash_redis/commands/async_commands.pyi
--rw-r--r--   0        0        0    71548 2023-07-02 12:48:09.153678 upstash_redis-0.13.1/upstash_redis/commands/commands.py
--rw-r--r--   0        0        0    21221 2023-07-02 12:48:09.153678 upstash_redis-0.13.1/upstash_redis/commands/commands.pyi
--rw-r--r--   0        0        0      283 2023-07-02 12:48:09.153678 upstash_redis-0.13.1/upstash_redis/config.py
--rw-r--r--   0        0        0       44 2023-07-02 12:48:09.153678 upstash_redis-0.13.1/upstash_redis/exception.py
--rw-r--r--   0        0        0      834 2023-07-02 12:48:09.153678 upstash_redis-0.13.1/upstash_redis/http/decode.py
--rw-r--r--   0        0        0     5478 2023-07-02 12:48:09.153678 upstash_redis-0.13.1/upstash_redis/http/execute.py
--rw-r--r--   0        0        0      431 2023-07-02 12:48:09.153678 upstash_redis-0.13.1/upstash_redis/schema/commands/parameters.py
--rw-r--r--   0        0        0      738 2023-07-02 12:48:09.153678 upstash_redis-0.13.1/upstash_redis/schema/commands/returns.py
--rw-r--r--   0        0        0      752 2023-07-02 12:48:09.153678 upstash_redis-0.13.1/upstash_redis/schema/http.py
--rw-r--r--   0        0        0      154 2023-07-02 12:48:09.153678 upstash_redis-0.13.1/upstash_redis/schema/telemetry.py
--rw-r--r--   0        0        0      172 2023-07-02 12:48:09.153678 upstash_redis-0.13.1/upstash_redis/typing.py
--rw-r--r--   0        0        0      107 2023-07-02 12:48:09.153678 upstash_redis-0.13.1/upstash_redis/utils/base.py
--rw-r--r--   0        0        0      242 2023-07-02 12:48:09.153678 upstash_redis-0.13.1/upstash_redis/utils/comparison.py
--rw-r--r--   0        0        0     3756 2023-07-02 12:48:09.153678 upstash_redis-0.13.1/upstash_redis/utils/exception.py
--rw-r--r--   0        0        0     9368 2023-07-02 12:48:09.153678 upstash_redis-0.13.1/upstash_redis/utils/format.py
--rw-r--r--   0        0        0     9853 1970-01-01 00:00:00.000000 upstash_redis-0.13.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-02 16:06:38.621153 upstash_redis-0.13.2/LICENSE
+-rw-r--r--   0        0        0     9173 2023-07-02 16:06:38.621153 upstash_redis-0.13.2/README.md
+-rw-r--r--   0        0        0      500 2023-07-02 16:06:38.621153 upstash_redis-0.13.2/pyproject.toml
+-rw-r--r--   0        0        0      150 2023-07-02 16:06:38.629153 upstash_redis-0.13.2/upstash_redis/__init__.py
+-rw-r--r--   0        0        0       68 2023-07-02 16:06:38.629153 upstash_redis-0.13.2/upstash_redis/asyncio/__init__.py
+-rw-r--r--   0        0        0     4782 2023-07-02 16:06:38.629153 upstash_redis-0.13.2/upstash_redis/asyncio/client.py
+-rw-r--r--   0        0        0     5052 2023-07-02 16:06:38.629153 upstash_redis-0.13.2/upstash_redis/client.py
+-rw-r--r--   0        0        0       82 2023-07-02 16:06:38.629153 upstash_redis-0.13.2/upstash_redis/commands/__init__.py
+-rw-r--r--   0        0        0       78 2023-07-02 16:06:38.629153 upstash_redis-0.13.2/upstash_redis/commands/async_commands.py
+-rw-r--r--   0        0        0    22111 2023-07-02 16:06:38.629153 upstash_redis-0.13.2/upstash_redis/commands/async_commands.pyi
+-rw-r--r--   0        0        0    71548 2023-07-02 16:06:38.629153 upstash_redis-0.13.2/upstash_redis/commands/commands.py
+-rw-r--r--   0        0        0    21221 2023-07-02 16:06:38.629153 upstash_redis-0.13.2/upstash_redis/commands/commands.pyi
+-rw-r--r--   0        0        0      283 2023-07-02 16:06:38.629153 upstash_redis-0.13.2/upstash_redis/config.py
+-rw-r--r--   0        0        0       44 2023-07-02 16:06:38.629153 upstash_redis-0.13.2/upstash_redis/exception.py
+-rw-r--r--   0        0        0      834 2023-07-02 16:06:38.629153 upstash_redis-0.13.2/upstash_redis/http/decode.py
+-rw-r--r--   0        0        0     5478 2023-07-02 16:06:38.629153 upstash_redis-0.13.2/upstash_redis/http/execute.py
+-rw-r--r--   0        0        0      431 2023-07-02 16:06:38.629153 upstash_redis-0.13.2/upstash_redis/schema/commands/parameters.py
+-rw-r--r--   0        0        0      738 2023-07-02 16:06:38.629153 upstash_redis-0.13.2/upstash_redis/schema/commands/returns.py
+-rw-r--r--   0        0        0      752 2023-07-02 16:06:38.629153 upstash_redis-0.13.2/upstash_redis/schema/http.py
+-rw-r--r--   0        0        0      154 2023-07-02 16:06:38.629153 upstash_redis-0.13.2/upstash_redis/schema/telemetry.py
+-rw-r--r--   0        0        0      172 2023-07-02 16:06:38.629153 upstash_redis-0.13.2/upstash_redis/typing.py
+-rw-r--r--   0        0        0      107 2023-07-02 16:06:38.629153 upstash_redis-0.13.2/upstash_redis/utils/base.py
+-rw-r--r--   0        0        0      242 2023-07-02 16:06:38.629153 upstash_redis-0.13.2/upstash_redis/utils/comparison.py
+-rw-r--r--   0        0        0     3756 2023-07-02 16:06:38.629153 upstash_redis-0.13.2/upstash_redis/utils/exception.py
+-rw-r--r--   0        0        0     9368 2023-07-02 16:06:38.629153 upstash_redis-0.13.2/upstash_redis/utils/format.py
+-rw-r--r--   0        0        0     9853 1970-01-01 00:00:00.000000 upstash_redis-0.13.2/PKG-INFO
```

### Comparing `upstash_redis-0.13.1/LICENSE` & `upstash_redis-0.13.2/LICENSE`

 * *Files identical despite different names*

### Comparing `upstash_redis-0.13.1/README.md` & `upstash_redis-0.13.2/README.md`

 * *Files identical despite different names*

### Comparing `upstash_redis-0.13.1/upstash_redis/asyncio/client.py` & `upstash_redis-0.13.2/upstash_redis/asyncio/client.py`

 * *Files identical despite different names*

### Comparing `upstash_redis-0.13.1/upstash_redis/client.py` & `upstash_redis-0.13.2/upstash_redis/client.py`

 * *Files identical despite different names*

### Comparing `upstash_redis-0.13.1/upstash_redis/commands/async_commands.pyi` & `upstash_redis-0.13.2/upstash_redis/commands/async_commands.pyi`

 * *Files identical despite different names*

### Comparing `upstash_redis-0.13.1/upstash_redis/commands/commands.py` & `upstash_redis-0.13.2/upstash_redis/commands/commands.py`

 * *Files identical despite different names*

### Comparing `upstash_redis-0.13.1/upstash_redis/commands/commands.pyi` & `upstash_redis-0.13.2/upstash_redis/commands/commands.pyi`

 * *Files identical despite different names*

### Comparing `upstash_redis-0.13.1/upstash_redis/http/decode.py` & `upstash_redis-0.13.2/upstash_redis/http/decode.py`

 * *Files identical despite different names*

### Comparing `upstash_redis-0.13.1/upstash_redis/http/execute.py` & `upstash_redis-0.13.2/upstash_redis/http/execute.py`

 * *Files identical despite different names*

### Comparing `upstash_redis-0.13.1/upstash_redis/schema/commands/returns.py` & `upstash_redis-0.13.2/upstash_redis/schema/commands/returns.py`

 * *Files identical despite different names*

### Comparing `upstash_redis-0.13.1/upstash_redis/schema/http.py` & `upstash_redis-0.13.2/upstash_redis/schema/http.py`

 * *Files identical despite different names*

### Comparing `upstash_redis-0.13.1/upstash_redis/utils/exception.py` & `upstash_redis-0.13.2/upstash_redis/utils/exception.py`

 * *Files identical despite different names*

### Comparing `upstash_redis-0.13.1/upstash_redis/utils/format.py` & `upstash_redis-0.13.2/upstash_redis/utils/format.py`

 * *Files 0% similar despite different names*

```diff
@@ -116,15 +116,15 @@
     """
     Format the raw output returned by "TIME".
     """
 
     return {"seconds": int(raw[0]), "microseconds": int(raw[1])}
 
 
-def format_sorted_set_return(raw: List[str], command=None) -> list[Tuple[str, float]]:
+def format_sorted_set_return(raw: List[str], command=None) -> List[Tuple[str, float]]:
     """
     Format the raw output given by Sorted Set commands, usually the ones that return the member-score
     pairs of Sorted Sets.
     """
     it = iter(raw)
     return list(zip(it, map(float, it)))
```

### Comparing `upstash_redis-0.13.1/PKG-INFO` & `upstash_redis-0.13.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: upstash-redis
-Version: 0.13.1
+Version: 0.13.2
 Summary: Serverless Redis Sdk from Upstash
 Author: Upstash
 Author-email: support@upstash.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

