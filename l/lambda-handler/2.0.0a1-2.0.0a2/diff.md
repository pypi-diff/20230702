# Comparing `tmp/lambda_handler-2.0.0a1.tar.gz` & `tmp/lambda_handler-2.0.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lambda_handler-2.0.0a1.tar", max compression
+gzip compressed data, was "lambda_handler-2.0.0a2.tar", max compression
```

## Comparing `lambda_handler-2.0.0a1.tar` & `lambda_handler-2.0.0a2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0    11357 2022-11-09 08:54:28.803833 lambda_handler-2.0.0a1/LICENSE
--rw-r--r--   0        0        0     4647 2023-07-01 19:01:26.885296 lambda_handler-2.0.0a1/README.md
--rw-r--r--   0        0        0      371 2023-07-02 08:11:43.754414 lambda_handler-2.0.0a1/lambda_handler/__init__.py
--rw-r--r--   0        0        0     2820 2022-11-09 09:08:20.229164 lambda_handler-2.0.0a1/lambda_handler/dependencies.py
--rw-r--r--   0        0        0    16074 2023-07-02 08:09:25.240089 lambda_handler-2.0.0a1/lambda_handler/handler.py
--rw-r--r--   0        0        0      594 2023-07-02 08:06:36.734615 lambda_handler-2.0.0a1/lambda_handler/model/__init__.py
--rw-r--r--   0        0        0     5927 2022-11-09 09:08:20.236865 lambda_handler-2.0.0a1/lambda_handler/model/base.py
--rw-r--r--   0        0        0     2134 2022-11-09 09:08:20.231006 lambda_handler-2.0.0a1/lambda_handler/model/direct_invocation.py
--rw-r--r--   0        0        0     3206 2022-11-09 09:08:20.234983 lambda_handler-2.0.0a1/lambda_handler/model/event_bridge.py
--rw-r--r--   0        0        0     4833 2023-07-02 08:06:14.514853 lambda_handler-2.0.0a1/lambda_handler/model/s3.py
--rw-r--r--   0        0        0     3511 2023-07-01 19:40:46.187213 lambda_handler-2.0.0a1/lambda_handler/model/sns.py
--rw-r--r--   0        0        0     4394 2022-11-09 09:57:24.033450 lambda_handler-2.0.0a1/lambda_handler/model/sqs.py
--rw-r--r--   0        0        0        0 2022-11-09 09:59:06.433379 lambda_handler-2.0.0a1/lambda_handler/py.typed
--rw-r--r--   0        0        0     2624 2022-11-09 09:35:27.330005 lambda_handler-2.0.0a1/lambda_handler/types.py
--rw-r--r--   0        0        0     9375 2022-11-09 09:36:45.711163 lambda_handler-2.0.0a1/lambda_handler/utils.py
--rw-r--r--   0        0        0     1704 2023-07-02 08:11:43.754985 lambda_handler-2.0.0a1/pyproject.toml
--rw-r--r--   0        0        0     5440 1970-01-01 00:00:00.000000 lambda_handler-2.0.0a1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2022-11-09 08:54:28.803833 lambda_handler-2.0.0a2/LICENSE
+-rw-r--r--   0        0        0     4647 2023-07-01 19:01:26.885296 lambda_handler-2.0.0a2/README.md
+-rw-r--r--   0        0        0      384 2023-07-02 08:17:18.752556 lambda_handler-2.0.0a2/lambda_handler/__init__.py
+-rw-r--r--   0        0        0     2820 2022-11-09 09:08:20.229164 lambda_handler-2.0.0a2/lambda_handler/dependencies.py
+-rw-r--r--   0        0        0    16074 2023-07-02 08:09:25.240089 lambda_handler-2.0.0a2/lambda_handler/handler.py
+-rw-r--r--   0        0        0      594 2023-07-02 08:06:36.734615 lambda_handler-2.0.0a2/lambda_handler/model/__init__.py
+-rw-r--r--   0        0        0     5927 2022-11-09 09:08:20.236865 lambda_handler-2.0.0a2/lambda_handler/model/base.py
+-rw-r--r--   0        0        0     2134 2022-11-09 09:08:20.231006 lambda_handler-2.0.0a2/lambda_handler/model/direct_invocation.py
+-rw-r--r--   0        0        0     3206 2022-11-09 09:08:20.234983 lambda_handler-2.0.0a2/lambda_handler/model/event_bridge.py
+-rw-r--r--   0        0        0     4833 2023-07-02 08:06:14.514853 lambda_handler-2.0.0a2/lambda_handler/model/s3.py
+-rw-r--r--   0        0        0     3511 2023-07-01 19:40:46.187213 lambda_handler-2.0.0a2/lambda_handler/model/sns.py
+-rw-r--r--   0        0        0     4394 2022-11-09 09:57:24.033450 lambda_handler-2.0.0a2/lambda_handler/model/sqs.py
+-rw-r--r--   0        0        0        0 2022-11-09 09:59:06.433379 lambda_handler-2.0.0a2/lambda_handler/py.typed
+-rw-r--r--   0        0        0     2624 2022-11-09 09:35:27.330005 lambda_handler-2.0.0a2/lambda_handler/types.py
+-rw-r--r--   0        0        0     9375 2022-11-09 09:36:45.711163 lambda_handler-2.0.0a2/lambda_handler/utils.py
+-rw-r--r--   0        0        0     1704 2023-07-02 08:17:18.752808 lambda_handler-2.0.0a2/pyproject.toml
+-rw-r--r--   0        0        0     5440 1970-01-01 00:00:00.000000 lambda_handler-2.0.0a2/PKG-INFO
```

### Comparing `lambda_handler-2.0.0a1/LICENSE` & `lambda_handler-2.0.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `lambda_handler-2.0.0a1/README.md` & `lambda_handler-2.0.0a2/README.md`

 * *Files identical despite different names*

### Comparing `lambda_handler-2.0.0a1/lambda_handler/dependencies.py` & `lambda_handler-2.0.0a2/lambda_handler/dependencies.py`

 * *Files identical despite different names*

### Comparing `lambda_handler-2.0.0a1/lambda_handler/handler.py` & `lambda_handler-2.0.0a2/lambda_handler/handler.py`

 * *Files identical despite different names*

### Comparing `lambda_handler-2.0.0a1/lambda_handler/model/__init__.py` & `lambda_handler-2.0.0a2/lambda_handler/model/__init__.py`

 * *Files identical despite different names*

### Comparing `lambda_handler-2.0.0a1/lambda_handler/model/base.py` & `lambda_handler-2.0.0a2/lambda_handler/model/base.py`

 * *Files identical despite different names*

### Comparing `lambda_handler-2.0.0a1/lambda_handler/model/direct_invocation.py` & `lambda_handler-2.0.0a2/lambda_handler/model/direct_invocation.py`

 * *Files identical despite different names*

### Comparing `lambda_handler-2.0.0a1/lambda_handler/model/event_bridge.py` & `lambda_handler-2.0.0a2/lambda_handler/model/event_bridge.py`

 * *Files identical despite different names*

### Comparing `lambda_handler-2.0.0a1/lambda_handler/model/s3.py` & `lambda_handler-2.0.0a2/lambda_handler/model/s3.py`

 * *Files identical despite different names*

### Comparing `lambda_handler-2.0.0a1/lambda_handler/model/sns.py` & `lambda_handler-2.0.0a2/lambda_handler/model/sns.py`

 * *Files identical despite different names*

### Comparing `lambda_handler-2.0.0a1/lambda_handler/model/sqs.py` & `lambda_handler-2.0.0a2/lambda_handler/model/sqs.py`

 * *Files identical despite different names*

### Comparing `lambda_handler-2.0.0a1/lambda_handler/types.py` & `lambda_handler-2.0.0a2/lambda_handler/types.py`

 * *Files identical despite different names*

### Comparing `lambda_handler-2.0.0a1/lambda_handler/utils.py` & `lambda_handler-2.0.0a2/lambda_handler/utils.py`

 * *Files identical despite different names*

### Comparing `lambda_handler-2.0.0a1/pyproject.toml` & `lambda_handler-2.0.0a2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lambda-handler"
-version = "2.0.0a1"
+version = "2.0.0a2"
 description = "A Python package for routing and validating AWS events inside a Lambda function"
 authors = ["Matthew Badger <matt@branchenergy.com>"]
 homepage = "https://github.com/branchenergy/lambda-handler"
 repository = "https://github.com/branchenergy/lambda-handler"
 license = "Apache 2.0"
 packages = [
   {include = "lambda_handler"},
@@ -47,9 +47,9 @@
     "invalid-name"                    # Calm down Pylint
 ]
 
 [tool.pytest.ini_options]
 addopts = "--cov=lambda_handler --cov-report term-missing"
 
 [build-system]
-requires = ["poetry-core>=2.0.0a1"]
+requires = ["poetry-core>=2.0.0a2"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `lambda_handler-2.0.0a1/PKG-INFO` & `lambda_handler-2.0.0a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lambda-handler
-Version: 2.0.0a1
+Version: 2.0.0a2
 Summary: A Python package for routing and validating AWS events inside a Lambda function
 Home-page: https://github.com/branchenergy/lambda-handler
 License: Apache 2.0
 Author: Matthew Badger
 Author-email: matt@branchenergy.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
```

