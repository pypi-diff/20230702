# Comparing `tmp/lambda_handler-2.0.0a3.tar.gz` & `tmp/lambda_handler-2.0.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lambda_handler-2.0.0a3.tar", max compression
+gzip compressed data, was "lambda_handler-2.0.0a4.tar", max compression
```

## Comparing `lambda_handler-2.0.0a3.tar` & `lambda_handler-2.0.0a4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0    11357 2022-11-09 08:54:28.803833 lambda_handler-2.0.0a3/LICENSE
--rw-r--r--   0        0        0     4647 2023-07-01 19:01:26.885296 lambda_handler-2.0.0a3/README.md
--rw-r--r--   0        0        0      384 2023-07-02 08:25:09.367641 lambda_handler-2.0.0a3/lambda_handler/__init__.py
--rw-r--r--   0        0        0     2820 2022-11-09 09:08:20.229164 lambda_handler-2.0.0a3/lambda_handler/dependencies.py
--rw-r--r--   0        0        0    16074 2023-07-02 08:09:25.240089 lambda_handler-2.0.0a3/lambda_handler/handler.py
--rw-r--r--   0        0        0      594 2023-07-02 08:06:36.734615 lambda_handler-2.0.0a3/lambda_handler/model/__init__.py
--rw-r--r--   0        0        0     5927 2022-11-09 09:08:20.236865 lambda_handler-2.0.0a3/lambda_handler/model/base.py
--rw-r--r--   0        0        0     2134 2022-11-09 09:08:20.231006 lambda_handler-2.0.0a3/lambda_handler/model/direct_invocation.py
--rw-r--r--   0        0        0     3206 2022-11-09 09:08:20.234983 lambda_handler-2.0.0a3/lambda_handler/model/event_bridge.py
--rw-r--r--   0        0        0     4833 2023-07-02 08:06:14.514853 lambda_handler-2.0.0a3/lambda_handler/model/s3.py
--rw-r--r--   0        0        0     3511 2023-07-01 19:40:46.187213 lambda_handler-2.0.0a3/lambda_handler/model/sns.py
--rw-r--r--   0        0        0     4394 2022-11-09 09:57:24.033450 lambda_handler-2.0.0a3/lambda_handler/model/sqs.py
--rw-r--r--   0        0        0        0 2022-11-09 09:59:06.433379 lambda_handler-2.0.0a3/lambda_handler/py.typed
--rw-r--r--   0        0        0     2624 2022-11-09 09:35:27.330005 lambda_handler-2.0.0a3/lambda_handler/types.py
--rw-r--r--   0        0        0     9375 2022-11-09 09:36:45.711163 lambda_handler-2.0.0a3/lambda_handler/utils.py
--rw-r--r--   0        0        0     1704 2023-07-02 08:25:09.367860 lambda_handler-2.0.0a3/pyproject.toml
--rw-r--r--   0        0        0     5440 1970-01-01 00:00:00.000000 lambda_handler-2.0.0a3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2022-11-09 08:54:28.803833 lambda_handler-2.0.0a4/LICENSE
+-rw-r--r--   0        0        0     4647 2023-07-01 19:01:26.885296 lambda_handler-2.0.0a4/README.md
+-rw-r--r--   0        0        0      384 2023-07-02 08:37:55.550495 lambda_handler-2.0.0a4/lambda_handler/__init__.py
+-rw-r--r--   0        0        0     2820 2022-11-09 09:08:20.229164 lambda_handler-2.0.0a4/lambda_handler/dependencies.py
+-rw-r--r--   0        0        0    16074 2023-07-02 08:09:25.240089 lambda_handler-2.0.0a4/lambda_handler/handler.py
+-rw-r--r--   0        0        0      594 2023-07-02 08:06:36.734615 lambda_handler-2.0.0a4/lambda_handler/model/__init__.py
+-rw-r--r--   0        0        0     5927 2022-11-09 09:08:20.236865 lambda_handler-2.0.0a4/lambda_handler/model/base.py
+-rw-r--r--   0        0        0     2134 2022-11-09 09:08:20.231006 lambda_handler-2.0.0a4/lambda_handler/model/direct_invocation.py
+-rw-r--r--   0        0        0     3206 2022-11-09 09:08:20.234983 lambda_handler-2.0.0a4/lambda_handler/model/event_bridge.py
+-rw-r--r--   0        0        0     4936 2023-07-02 08:34:56.412686 lambda_handler-2.0.0a4/lambda_handler/model/s3.py
+-rw-r--r--   0        0        0     3511 2023-07-01 19:40:46.187213 lambda_handler-2.0.0a4/lambda_handler/model/sns.py
+-rw-r--r--   0        0        0     4394 2022-11-09 09:57:24.033450 lambda_handler-2.0.0a4/lambda_handler/model/sqs.py
+-rw-r--r--   0        0        0        0 2022-11-09 09:59:06.433379 lambda_handler-2.0.0a4/lambda_handler/py.typed
+-rw-r--r--   0        0        0     2624 2022-11-09 09:35:27.330005 lambda_handler-2.0.0a4/lambda_handler/types.py
+-rw-r--r--   0        0        0     9427 2023-07-02 08:37:14.372250 lambda_handler-2.0.0a4/lambda_handler/utils.py
+-rw-r--r--   0        0        0     1704 2023-07-02 08:37:55.551131 lambda_handler-2.0.0a4/pyproject.toml
+-rw-r--r--   0        0        0     5440 1970-01-01 00:00:00.000000 lambda_handler-2.0.0a4/PKG-INFO
```

### Comparing `lambda_handler-2.0.0a3/LICENSE` & `lambda_handler-2.0.0a4/LICENSE`

 * *Files identical despite different names*

### Comparing `lambda_handler-2.0.0a3/README.md` & `lambda_handler-2.0.0a4/README.md`

 * *Files identical despite different names*

### Comparing `lambda_handler-2.0.0a3/lambda_handler/dependencies.py` & `lambda_handler-2.0.0a4/lambda_handler/dependencies.py`

 * *Files identical despite different names*

### Comparing `lambda_handler-2.0.0a3/lambda_handler/handler.py` & `lambda_handler-2.0.0a4/lambda_handler/handler.py`

 * *Files identical despite different names*

### Comparing `lambda_handler-2.0.0a3/lambda_handler/model/__init__.py` & `lambda_handler-2.0.0a4/lambda_handler/model/__init__.py`

 * *Files identical despite different names*

### Comparing `lambda_handler-2.0.0a3/lambda_handler/model/base.py` & `lambda_handler-2.0.0a4/lambda_handler/model/base.py`

 * *Files identical despite different names*

### Comparing `lambda_handler-2.0.0a3/lambda_handler/model/direct_invocation.py` & `lambda_handler-2.0.0a4/lambda_handler/model/direct_invocation.py`

 * *Files identical despite different names*

### Comparing `lambda_handler-2.0.0a3/lambda_handler/model/event_bridge.py` & `lambda_handler-2.0.0a4/lambda_handler/model/event_bridge.py`

 * *Files identical despite different names*

### Comparing `lambda_handler-2.0.0a3/lambda_handler/model/s3.py` & `lambda_handler-2.0.0a4/lambda_handler/model/s3.py`

 * *Files 14% similar despite different names*

```diff
@@ -52,74 +52,74 @@
             #: pylint: disable=unused-argument
             ...
 
 else:
     from pydantic import Json
 
 
-class S3EventRecordGlacierRestoreEventData(BaseModel):
+class S3EventRecordGlacierRestoreEventData(BranchBaseModel):
     lifecycle_restoration_expiry_time: dt.datetime
     lifecycle_restore_storage_class: str
 
 
-class S3EventRecordGlacierEventData(BaseModel):
+class S3EventRecordGlacierEventData(BranchBaseModel):
     restore_event_data: S3EventRecordGlacierRestoreEventData
 
 
-class S3Identity(BaseModel):
+class S3Identity(BranchBaseModel):
     principal_id: str
 
 
-class S3RequestParameters(BaseModel):
+class S3RequestParameters(BranchBaseModel):
     source_ip_address: IPvAnyNetwork = Field(alias="sourceIPAddress")
 
 
-class S3ResponseElements(BaseModel):
+class S3ResponseElements(BranchBaseModel):
     x_amz_request_id: str = Field(None, alias="x-amz-request-id")
     x_amz_id_2: str = Field(None, alias="x-amz-id-2")
 
 
-class S3OwnerIdentify(BaseModel):
+class S3OwnerIdentify(BranchBaseModel):
     principal_id: str
 
 
-class S3Bucket(BaseModel):
+class S3Bucket(BranchBaseModel):
     name: str
     owner_identity: S3OwnerIdentify
     arn: str
 
 
-class S3Object(BaseModel):
+class S3Object(BranchBaseModel):
     key: str
     size: Optional[NonNegativeFloat]
     etag: Optional[str] = Field(alias="eTag")
     sequencer: str
     version_id: Optional[str]
 
 
-class S3Message(BaseModel):
+class S3Message(BranchBaseModel):
     s3_schema_version: str
     configuration_id: str
     bucket: S3Bucket
     object: S3Object  # noqa: A003,VNE003
 
 
-class S3EventNotificationObject(BaseModel):
+class S3EventNotificationObject(BranchBaseModel):
     key: str
     size: Optional[NonNegativeFloat]
     etag: str
     version_id: str = Field(None, alias="version-id")
     sequencer: Optional[str]
 
 
-class S3EventNotificationEventBridgeBucket(BaseModel):
+class S3EventNotificationEventBridgeBucket(BranchBaseModel):
     name: str
 
 
-class S3EventNotificationEventBridgeDetail(BaseModel):
+class S3EventNotificationEventBridgeDetail(BranchBaseModel):
     version: str
     bucket: S3EventNotificationEventBridgeBucket
     object: S3EventNotificationObject  # noqa: A003,VNE003
     request_id: str = Field(None, alias="request-id")
     requester: str
     source_ip_address: str = Field(None, alias="source-ip-address")
     reason: Optional[str]
@@ -143,15 +143,15 @@
     region: str
     resources: List[str]
     detail_type: str = Field(None, alias="detail-type")
     detail: S3EventNotificationEventBridgeDetail
     replay_name: Optional[str] = Field(None, alias="replay-name")
 
 
-class S3Record(BaseModel):
+class S3Record(BranchBaseModel):
     event_version: str
     event_source: Literal["aws:s3"]
     aws_region: str
     event_time: dt.datetime
     event_name: str
     user_identity: S3Identity
     request_parameters: S3RequestParameters
@@ -165,15 +165,15 @@
 
     Parameters
     ----------
     records : List[S3Record]
         List of S3 records
     """
 
-    records: List[S3Record]
+    records: List[S3Record] = Field(alias="Records")
 
     @property
     def event_name(self) -> str:
         """S3 event name
 
         Returns
         -------
```

### Comparing `lambda_handler-2.0.0a3/lambda_handler/model/sns.py` & `lambda_handler-2.0.0a4/lambda_handler/model/sns.py`

 * *Files identical despite different names*

### Comparing `lambda_handler-2.0.0a3/lambda_handler/model/sqs.py` & `lambda_handler-2.0.0a4/lambda_handler/model/sqs.py`

 * *Files identical despite different names*

### Comparing `lambda_handler-2.0.0a3/lambda_handler/types.py` & `lambda_handler-2.0.0a4/lambda_handler/types.py`

 * *Files identical despite different names*

### Comparing `lambda_handler-2.0.0a3/lambda_handler/utils.py` & `lambda_handler-2.0.0a4/lambda_handler/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 """Utility functions"""
 
 import inspect
 import logging
+import re
 from functools import wraps
 
 from lambda_handler.dependencies import DependencyC
 
 #: pylint: disable=duplicate-code
 from lambda_handler.model import (
     ApiGatewayEvent,
     AwsEvent,
     DirectInvocationEvent,
     EventBridgeEvent,
     LambdaResponse,
+    S3Event,
     SnsEvent,
     SqsEvent,
 )
 from lambda_handler.types import (
     AwsEventCallable,
     AwsEventRawCallable,
     AwsEventType,
@@ -214,15 +216,15 @@
             dependencies: Dict[str, Any] = {
                 k: p.default()
                 for k, p in sig.parameters.items()
                 if isinstance(p.default, DependencyC)
             }
 
             parsed_event = concrete_event_type.parse_obj(event)
-            if parsed_event.event_key != event_key:
+            if not re.match(event_key, parsed_event.event_key):
                 raise EventKeyMismatch(
                     f"Event key mismatch! `'{parsed_event.event_key}' != '{event_key}'`"
                 )
             return func(parsed_event, **dependencies).dict()
 
         handler.add_event_func(event_type, event_key, inner)
 
@@ -346,14 +348,15 @@
     UnknownEventType
         If it cannot parse `event`
     """
     event_types: List[Type[AwsEvent]] = [
         ApiGatewayEvent,
         DirectInvocationEvent,
         EventBridgeEvent,
+        S3Event,
         SnsEvent,
         SqsEvent,
     ]
 
     for event_type in event_types:
         if event_type.matches_event_type(event):
             name = event_type.__qualname__
```

### Comparing `lambda_handler-2.0.0a3/pyproject.toml` & `lambda_handler-2.0.0a4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lambda-handler"
-version = "2.0.0a3"
+version = "2.0.0a4"
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
-requires = ["poetry-core>=2.0.0a3"]
+requires = ["poetry-core>=2.0.0a4"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `lambda_handler-2.0.0a3/PKG-INFO` & `lambda_handler-2.0.0a4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lambda-handler
-Version: 2.0.0a3
+Version: 2.0.0a4
 Summary: A Python package for routing and validating AWS events inside a Lambda function
 Home-page: https://github.com/branchenergy/lambda-handler
 License: Apache 2.0
 Author: Matthew Badger
 Author-email: matt@branchenergy.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
```

