# Comparing `tmp/upstash_redis-0.13.0.tar.gz` & `tmp/upstash_redis-0.13.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "upstash_redis-0.13.0.tar", max compression
+gzip compressed data, was "upstash_redis-0.13.1.tar", max compression
```

## Comparing `upstash_redis-0.13.0.tar` & `upstash_redis-0.13.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     1070 2023-05-24 13:48:44.535163 upstash_redis-0.13.0/LICENSE
--rw-r--r--   0        0        0     9173 2023-06-12 07:56:37.090873 upstash_redis-0.13.0/README.md
--rw-r--r--   0        0        0      467 2023-07-02 09:22:06.079913 upstash_redis-0.13.0/pyproject.toml
--rw-r--r--   0        0        0      150 2023-06-30 10:23:27.543198 upstash_redis-0.13.0/upstash_redis/__init__.py
--rw-r--r--   0        0        0       68 2023-06-29 09:51:44.031185 upstash_redis-0.13.0/upstash_redis/asyncio/__init__.py
--rw-r--r--   0        0        0     4782 2023-07-01 22:51:26.915848 upstash_redis-0.13.0/upstash_redis/asyncio/client.py
--rw-r--r--   0        0        0     4999 2023-07-01 22:51:14.000967 upstash_redis-0.13.0/upstash_redis/client.py
--rw-r--r--   0        0        0       82 2023-07-01 09:47:03.295810 upstash_redis-0.13.0/upstash_redis/commands/__init__.py
--rw-r--r--   0        0        0       78 2023-07-01 09:47:03.278399 upstash_redis-0.13.0/upstash_redis/commands/async_commands.py
--rw-r--r--   0        0        0    22111 2023-07-01 23:27:47.297643 upstash_redis-0.13.0/upstash_redis/commands/async_commands.pyi
--rw-r--r--   0        0        0    71548 2023-07-01 23:27:46.350521 upstash_redis-0.13.0/upstash_redis/commands/commands.py
--rw-r--r--   0        0        0    21221 2023-07-01 23:27:46.330353 upstash_redis-0.13.0/upstash_redis/commands/commands.pyi
--rw-r--r--   0        0        0      283 2023-06-12 07:56:37.096624 upstash_redis-0.13.0/upstash_redis/config.py
--rw-r--r--   0        0        0       44 2023-06-12 07:56:37.096683 upstash_redis-0.13.0/upstash_redis/exception.py
--rw-r--r--   0        0        0      834 2023-06-22 15:12:55.454825 upstash_redis-0.13.0/upstash_redis/http/decode.py
--rw-r--r--   0        0        0     5478 2023-07-01 02:19:38.193972 upstash_redis-0.13.0/upstash_redis/http/execute.py
--rw-r--r--   0        0        0      431 2023-06-22 15:12:55.456040 upstash_redis-0.13.0/upstash_redis/schema/commands/parameters.py
--rw-r--r--   0        0        0      738 2023-07-01 18:41:41.722004 upstash_redis-0.13.0/upstash_redis/schema/commands/returns.py
--rw-r--r--   0        0        0      752 2023-06-22 15:12:55.456727 upstash_redis-0.13.0/upstash_redis/schema/http.py
--rw-r--r--   0        0        0      154 2023-06-12 07:56:37.097241 upstash_redis-0.13.0/upstash_redis/schema/telemetry.py
--rw-r--r--   0        0        0      172 2023-07-01 02:24:32.912661 upstash_redis-0.13.0/upstash_redis/typing.py
--rw-r--r--   0        0        0      107 2023-06-12 07:56:37.097319 upstash_redis-0.13.0/upstash_redis/utils/base.py
--rw-r--r--   0        0        0      242 2023-06-12 07:56:37.097393 upstash_redis-0.13.0/upstash_redis/utils/comparison.py
--rw-r--r--   0        0        0     3756 2023-06-22 15:12:55.457479 upstash_redis-0.13.0/upstash_redis/utils/exception.py
--rw-r--r--   0        0        0     9368 2023-07-01 22:51:44.121000 upstash_redis-0.13.0/upstash_redis/utils/format.py
--rw-r--r--   0        0        0     9832 1970-01-01 00:00:00.000000 upstash_redis-0.13.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-02 12:48:09.145678 upstash_redis-0.13.1/LICENSE
+-rw-r--r--   0        0        0     9173 2023-07-02 12:48:09.145678 upstash_redis-0.13.1/README.md
+-rw-r--r--   0        0        0      500 2023-07-02 12:48:09.145678 upstash_redis-0.13.1/pyproject.toml
+-rw-r--r--   0        0        0      150 2023-07-02 12:48:09.149678 upstash_redis-0.13.1/upstash_redis/__init__.py
+-rw-r--r--   0        0        0       68 2023-07-02 12:48:09.149678 upstash_redis-0.13.1/upstash_redis/asyncio/__init__.py
+-rw-r--r--   0        0        0     4782 2023-07-02 12:48:09.149678 upstash_redis-0.13.1/upstash_redis/asyncio/client.py
+-rw-r--r--   0        0        0     5052 2023-07-02 12:48:09.149678 upstash_redis-0.13.1/upstash_redis/client.py
+-rw-r--r--   0        0        0       82 2023-07-02 12:48:09.149678 upstash_redis-0.13.1/upstash_redis/commands/__init__.py
+-rw-r--r--   0        0        0       78 2023-07-02 12:48:09.153678 upstash_redis-0.13.1/upstash_redis/commands/async_commands.py
+-rw-r--r--   0        0        0    22111 2023-07-02 12:48:09.153678 upstash_redis-0.13.1/upstash_redis/commands/async_commands.pyi
+-rw-r--r--   0        0        0    71548 2023-07-02 12:48:09.153678 upstash_redis-0.13.1/upstash_redis/commands/commands.py
+-rw-r--r--   0        0        0    21221 2023-07-02 12:48:09.153678 upstash_redis-0.13.1/upstash_redis/commands/commands.pyi
+-rw-r--r--   0        0        0      283 2023-07-02 12:48:09.153678 upstash_redis-0.13.1/upstash_redis/config.py
+-rw-r--r--   0        0        0       44 2023-07-02 12:48:09.153678 upstash_redis-0.13.1/upstash_redis/exception.py
+-rw-r--r--   0        0        0      834 2023-07-02 12:48:09.153678 upstash_redis-0.13.1/upstash_redis/http/decode.py
+-rw-r--r--   0        0        0     5478 2023-07-02 12:48:09.153678 upstash_redis-0.13.1/upstash_redis/http/execute.py
+-rw-r--r--   0        0        0      431 2023-07-02 12:48:09.153678 upstash_redis-0.13.1/upstash_redis/schema/commands/parameters.py
+-rw-r--r--   0        0        0      738 2023-07-02 12:48:09.153678 upstash_redis-0.13.1/upstash_redis/schema/commands/returns.py
+-rw-r--r--   0        0        0      752 2023-07-02 12:48:09.153678 upstash_redis-0.13.1/upstash_redis/schema/http.py
+-rw-r--r--   0        0        0      154 2023-07-02 12:48:09.153678 upstash_redis-0.13.1/upstash_redis/schema/telemetry.py
+-rw-r--r--   0        0        0      172 2023-07-02 12:48:09.153678 upstash_redis-0.13.1/upstash_redis/typing.py
+-rw-r--r--   0        0        0      107 2023-07-02 12:48:09.153678 upstash_redis-0.13.1/upstash_redis/utils/base.py
+-rw-r--r--   0        0        0      242 2023-07-02 12:48:09.153678 upstash_redis-0.13.1/upstash_redis/utils/comparison.py
+-rw-r--r--   0        0        0     3756 2023-07-02 12:48:09.153678 upstash_redis-0.13.1/upstash_redis/utils/exception.py
+-rw-r--r--   0        0        0     9368 2023-07-02 12:48:09.153678 upstash_redis-0.13.1/upstash_redis/utils/format.py
+-rw-r--r--   0        0        0     9853 1970-01-01 00:00:00.000000 upstash_redis-0.13.1/PKG-INFO
```

### Comparing `upstash_redis-0.13.0/LICENSE` & `upstash_redis-0.13.1/LICENSE`

 * *Files identical despite different names*

### Comparing `upstash_redis-0.13.0/README.md` & `upstash_redis-0.13.1/README.md`

 * *Files identical despite different names*

### Comparing `upstash_redis-0.13.0/upstash_redis/asyncio/client.py` & `upstash_redis-0.13.1/upstash_redis/asyncio/client.py`

 * *Files identical despite different names*

### Comparing `upstash_redis-0.13.0/upstash_redis/client.py` & `upstash_redis-0.13.1/upstash_redis/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -134,7 +134,9 @@
 
         if (self.format_return or main_command == "HSCAN" or main_command == "SMEMBERS" or main_command == "SDIFF" or main_command == "SINTER" or main_command == "SSCAN" or main_command == "SUNION" or main_command == "ZSCAN") and (main_command in self.FORMATTERS):
             return self.FORMATTERS[main_command](res, command)
 
         return res
         
 
+
+# TODO: get platform from env variable for telemetry
```

### Comparing `upstash_redis-0.13.0/upstash_redis/commands/async_commands.pyi` & `upstash_redis-0.13.1/upstash_redis/commands/async_commands.pyi`

 * *Files identical despite different names*

### Comparing `upstash_redis-0.13.0/upstash_redis/commands/commands.py` & `upstash_redis-0.13.1/upstash_redis/commands/commands.py`

 * *Files identical despite different names*

### Comparing `upstash_redis-0.13.0/upstash_redis/commands/commands.pyi` & `upstash_redis-0.13.1/upstash_redis/commands/commands.pyi`

 * *Files identical despite different names*

### Comparing `upstash_redis-0.13.0/upstash_redis/http/decode.py` & `upstash_redis-0.13.1/upstash_redis/http/decode.py`

 * *Files identical despite different names*

### Comparing `upstash_redis-0.13.0/upstash_redis/http/execute.py` & `upstash_redis-0.13.1/upstash_redis/http/execute.py`

 * *Files identical despite different names*

### Comparing `upstash_redis-0.13.0/upstash_redis/schema/commands/returns.py` & `upstash_redis-0.13.1/upstash_redis/schema/commands/returns.py`

 * *Files identical despite different names*

### Comparing `upstash_redis-0.13.0/upstash_redis/schema/http.py` & `upstash_redis-0.13.1/upstash_redis/schema/http.py`

 * *Files identical despite different names*

### Comparing `upstash_redis-0.13.0/upstash_redis/utils/exception.py` & `upstash_redis-0.13.1/upstash_redis/utils/exception.py`

 * *Files identical despite different names*

### Comparing `upstash_redis-0.13.0/upstash_redis/utils/format.py` & `upstash_redis-0.13.1/upstash_redis/utils/format.py`

 * *Files identical despite different names*

### Comparing `upstash_redis-0.13.0/PKG-INFO` & `upstash_redis-0.13.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: upstash-redis
-Version: 0.13.0
-Summary: 
-Author: Zgîmbău Tudor
-Author-email: tudor.zgimbau@gmail.com
+Version: 0.13.1
+Summary: Serverless Redis Sdk from Upstash
+Author: Upstash
+Author-email: support@upstash.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

