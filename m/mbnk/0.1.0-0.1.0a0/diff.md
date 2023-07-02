# Comparing `tmp/mbnk-0.1.0.tar.gz` & `tmp/mbnk-0.1.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mbnk-0.1.0.tar", max compression
+gzip compressed data, was "mbnk-0.1.0a0.tar", max compression
```

## Comparing `mbnk-0.1.0.tar` & `mbnk-0.1.0a0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1420 2023-07-02 05:05:53.695059 mbnk-0.1.0/README.md
--rw-r--r--   0        0        0      359 2023-07-02 05:26:34.519609 mbnk-0.1.0/mbnk/__init__.py
--rw-r--r--   0        0        0    14803 2023-07-02 18:44:15.060560 mbnk-0.1.0/mbnk/api.py
--rw-r--r--   0        0        0      101 2023-07-02 05:26:15.783700 mbnk-0.1.0/mbnk/asyncio/__init__.py
--rw-r--r--   0        0        0      323 2023-07-02 17:30:10.132706 mbnk-0.1.0/mbnk/asyncio/mbnk.py
--rw-r--r--   0        0        0     2710 2023-07-02 17:32:57.818194 mbnk-0.1.0/mbnk/decorators.py
--rw-r--r--   0        0        0     1697 2023-07-02 05:20:44.513374 mbnk-0.1.0/mbnk/enums.py
--rw-r--r--   0        0        0      300 2023-07-02 01:07:19.623331 mbnk-0.1.0/mbnk/exceptions.py
--rw-r--r--   0        0        0     2164 2023-07-02 18:13:15.452507 mbnk-0.1.0/mbnk/instances.py
--rw-r--r--   0        0        0      315 2023-07-02 18:14:01.695715 mbnk-0.1.0/mbnk/mbnk.py
--rw-r--r--   0        0        0     2217 2023-07-01 23:15:46.030057 mbnk-0.1.0/mbnk/responses.py
--rw-r--r--   0        0        0       97 2023-07-01 23:23:24.859301 mbnk-0.1.0/mbnk/utils/__init__.py
--rw-r--r--   0        0        0      269 2023-07-01 23:23:25.011300 mbnk-0.1.0/mbnk/utils/builders.py
--rw-r--r--   0        0        0      839 2023-07-02 18:14:30.643213 mbnk-0.1.0/mbnk/utils/format.py
--rw-r--r--   0        0        0      389 2023-07-02 01:04:35.544706 mbnk-0.1.0/mbnk/utils/is_exception.py
--rw-r--r--   0        0        0      466 2023-07-01 22:05:58.624489 mbnk-0.1.0/mbnk/utils/webhook.py
--rw-r--r--   0        0        0      313 2023-07-02 19:00:38.691108 mbnk-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1951 1970-01-01 00:00:00.000000 mbnk-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1420 2023-07-02 05:05:53.695059 mbnk-0.1.0a0/README.md
+-rw-r--r--   0        0        0      359 2023-07-02 05:26:34.519609 mbnk-0.1.0a0/mbnk/__init__.py
+-rw-r--r--   0        0        0    14803 2023-07-02 18:44:15.060560 mbnk-0.1.0a0/mbnk/api.py
+-rw-r--r--   0        0        0      101 2023-07-02 05:26:15.783700 mbnk-0.1.0a0/mbnk/asyncio/__init__.py
+-rw-r--r--   0        0        0      323 2023-07-02 17:30:10.132706 mbnk-0.1.0a0/mbnk/asyncio/mbnk.py
+-rw-r--r--   0        0        0     2710 2023-07-02 17:32:57.818194 mbnk-0.1.0a0/mbnk/decorators.py
+-rw-r--r--   0        0        0     1697 2023-07-02 05:20:44.513374 mbnk-0.1.0a0/mbnk/enums.py
+-rw-r--r--   0        0        0      300 2023-07-02 01:07:19.623331 mbnk-0.1.0a0/mbnk/exceptions.py
+-rw-r--r--   0        0        0     2164 2023-07-02 18:13:15.452507 mbnk-0.1.0a0/mbnk/instances.py
+-rw-r--r--   0        0        0      315 2023-07-02 18:14:01.695715 mbnk-0.1.0a0/mbnk/mbnk.py
+-rw-r--r--   0        0        0     2217 2023-07-01 23:15:46.030057 mbnk-0.1.0a0/mbnk/responses.py
+-rw-r--r--   0        0        0       97 2023-07-01 23:23:24.859301 mbnk-0.1.0a0/mbnk/utils/__init__.py
+-rw-r--r--   0        0        0      269 2023-07-01 23:23:25.011300 mbnk-0.1.0a0/mbnk/utils/builders.py
+-rw-r--r--   0        0        0      839 2023-07-02 18:14:30.643213 mbnk-0.1.0a0/mbnk/utils/format.py
+-rw-r--r--   0        0        0      389 2023-07-02 01:04:35.544706 mbnk-0.1.0a0/mbnk/utils/is_exception.py
+-rw-r--r--   0        0        0      466 2023-07-01 22:05:58.624489 mbnk-0.1.0a0/mbnk/utils/webhook.py
+-rw-r--r--   0        0        0      315 2023-07-02 18:55:37.617760 mbnk-0.1.0a0/pyproject.toml
+-rw-r--r--   0        0        0     1953 1970-01-01 00:00:00.000000 mbnk-0.1.0a0/PKG-INFO
```

### Comparing `mbnk-0.1.0/README.md` & `mbnk-0.1.0a0/README.md`

 * *Files identical despite different names*

### Comparing `mbnk-0.1.0/mbnk/api.py` & `mbnk-0.1.0a0/mbnk/api.py`

 * *Files identical despite different names*

### Comparing `mbnk-0.1.0/mbnk/decorators.py` & `mbnk-0.1.0a0/mbnk/decorators.py`

 * *Files identical despite different names*

### Comparing `mbnk-0.1.0/mbnk/enums.py` & `mbnk-0.1.0a0/mbnk/enums.py`

 * *Files identical despite different names*

### Comparing `mbnk-0.1.0/mbnk/instances.py` & `mbnk-0.1.0a0/mbnk/instances.py`

 * *Files identical despite different names*

### Comparing `mbnk-0.1.0/mbnk/responses.py` & `mbnk-0.1.0a0/mbnk/responses.py`

 * *Files identical despite different names*

### Comparing `mbnk-0.1.0/mbnk/utils/format.py` & `mbnk-0.1.0a0/mbnk/utils/format.py`

 * *Files identical despite different names*

### Comparing `mbnk-0.1.0/PKG-INFO` & `mbnk-0.1.0a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mbnk
-Version: 0.1.0
+Version: 0.1.0a0
 Summary: Sync/Async version monobank api
 License: MIT
 Author: yeghorkikhai
 Author-email: yeghorkikhai@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

