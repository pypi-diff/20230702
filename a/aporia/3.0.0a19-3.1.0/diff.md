# Comparing `tmp/aporia-3.0.0a19.tar.gz` & `tmp/aporia-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aporia-3.0.0a19.tar", max compression
+gzip compressed data, was "aporia-3.1.0.tar", max compression
```

## Comparing `aporia-3.0.0a19.tar` & `aporia-3.1.0.tar`

### file list

```diff
@@ -1,27 +1,28 @@
--rw-r--r--   0        0        0     2968 2023-06-20 23:37:32.344442 aporia-3.0.0a19/README.md
--rw-r--r--   0        0        0      832 2023-06-20 23:37:32.348442 aporia-3.0.0a19/pyproject.toml
--rw-r--r--   0        0        0      168 2023-06-20 23:37:32.348442 aporia-3.0.0a19/src/aporia/__init__.py
--rw-r--r--   0        0        0      540 2023-06-20 23:37:32.348442 aporia-3.0.0a19/src/aporia/as_code/__init__.py
--rw-r--r--   0        0        0      939 2023-06-20 23:37:32.348442 aporia-3.0.0a19/src/aporia/as_code/resources/base.py
--rw-r--r--   0        0        0     1436 2023-06-20 23:37:32.348442 aporia-3.0.0a19/src/aporia/as_code/resources/custom_metrics.py
--rw-r--r--   0        0        0     1984 2023-06-20 23:37:32.348442 aporia-3.0.0a19/src/aporia/as_code/resources/data_source.py
--rw-r--r--   0        0        0     7214 2023-06-20 23:37:32.348442 aporia-3.0.0a19/src/aporia/as_code/resources/dataset.py
--rw-r--r--   0        0        0     3854 2023-06-20 23:37:32.348442 aporia-3.0.0a19/src/aporia/as_code/resources/model.py
--rw-r--r--   0        0        0     1370 2023-06-20 23:37:32.348442 aporia-3.0.0a19/src/aporia/as_code/resources/monitor.py
--rw-r--r--   0        0        0     1778 2023-06-20 23:37:32.348442 aporia-3.0.0a19/src/aporia/as_code/resources/segment.py
--rw-r--r--   0        0        0     1917 2023-06-20 23:37:32.348442 aporia-3.0.0a19/src/aporia/as_code/resources/version.py
--rw-r--r--   0        0        0    12813 2023-06-20 23:37:32.348442 aporia-3.0.0a19/src/aporia/as_code/stack.py
--rw-r--r--   0        0        0        0 2023-06-20 23:37:32.348442 aporia-3.0.0a19/src/aporia/sdk/__init__.py
--rw-r--r--   0        0        0     2975 2023-06-20 23:37:32.348442 aporia-3.0.0a19/src/aporia/sdk/aporia_api.py
--rw-r--r--   0        0        0      723 2023-06-20 23:37:32.348442 aporia-3.0.0a19/src/aporia/sdk/base.py
--rw-r--r--   0        0        0     1531 2023-06-20 23:37:32.348442 aporia-3.0.0a19/src/aporia/sdk/client.py
--rw-r--r--   0        0        0     2115 2023-06-20 23:37:32.348442 aporia-3.0.0a19/src/aporia/sdk/custom_metrics.py
--rw-r--r--   0        0        0     1822 2023-06-20 23:37:32.348442 aporia-3.0.0a19/src/aporia/sdk/dashboards.py
--rw-r--r--   0        0        0     3542 2023-06-20 23:37:32.348442 aporia-3.0.0a19/src/aporia/sdk/data_sources.py
--rw-r--r--   0        0        0     6528 2023-06-20 23:37:32.348442 aporia-3.0.0a19/src/aporia/sdk/datasets.py
--rw-r--r--   0        0        0     6108 2023-06-20 23:37:32.348442 aporia-3.0.0a19/src/aporia/sdk/metrics.py
--rw-r--r--   0        0        0     5644 2023-06-20 23:37:32.348442 aporia-3.0.0a19/src/aporia/sdk/models.py
--rw-r--r--   0        0        0    18814 2023-06-20 23:37:32.348442 aporia-3.0.0a19/src/aporia/sdk/monitors.py
--rw-r--r--   0        0        0     2936 2023-06-20 23:37:32.348442 aporia-3.0.0a19/src/aporia/sdk/segments.py
--rw-r--r--   0        0        0     2897 2023-06-20 23:37:32.348442 aporia-3.0.0a19/src/aporia/sdk/versions.py
--rw-r--r--   0        0        0     3477 1970-01-01 00:00:00.000000 aporia-3.0.0a19/PKG-INFO
+-rw-r--r--   0        0        0     2968 2023-07-02 17:07:50.080201 aporia-3.1.0/README.md
+-rw-r--r--   0        0        0      829 2023-07-02 17:07:50.084201 aporia-3.1.0/pyproject.toml
+-rw-r--r--   0        0        0      168 2023-07-02 17:07:50.084201 aporia-3.1.0/src/aporia/__init__.py
+-rw-r--r--   0        0        0      925 2023-07-02 17:07:50.084201 aporia-3.1.0/src/aporia/as_code/__init__.py
+-rw-r--r--   0        0        0      939 2023-07-02 17:07:50.084201 aporia-3.1.0/src/aporia/as_code/resources/base.py
+-rw-r--r--   0        0        0     1465 2023-07-02 17:07:50.084201 aporia-3.1.0/src/aporia/as_code/resources/custom_metrics.py
+-rw-r--r--   0        0        0     1984 2023-07-02 17:07:50.084201 aporia-3.1.0/src/aporia/as_code/resources/data_source.py
+-rw-r--r--   0        0        0     7206 2023-07-02 17:07:50.084201 aporia-3.1.0/src/aporia/as_code/resources/dataset.py
+-rw-r--r--   0        0        0     3854 2023-07-02 17:07:50.084201 aporia-3.1.0/src/aporia/as_code/resources/model.py
+-rw-r--r--   0        0        0    11048 2023-07-02 17:07:50.084201 aporia-3.1.0/src/aporia/as_code/resources/monitor.py
+-rw-r--r--   0        0        0     2831 2023-07-02 17:07:50.084201 aporia-3.1.0/src/aporia/as_code/resources/segment.py
+-rw-r--r--   0        0        0     1946 2023-07-02 17:07:50.084201 aporia-3.1.0/src/aporia/as_code/resources/version.py
+-rw-r--r--   0        0        0    34719 2023-07-02 17:07:50.084201 aporia-3.1.0/src/aporia/as_code/stack.py
+-rw-r--r--   0        0        0        0 2023-07-02 17:07:50.084201 aporia-3.1.0/src/aporia/sdk/__init__.py
+-rw-r--r--   0        0        0     3233 2023-07-02 17:07:50.084201 aporia-3.1.0/src/aporia/sdk/aporia_api.py
+-rw-r--r--   0        0        0      723 2023-07-02 17:07:50.084201 aporia-3.1.0/src/aporia/sdk/base.py
+-rw-r--r--   0        0        0     1531 2023-07-02 17:07:50.084201 aporia-3.1.0/src/aporia/sdk/client.py
+-rw-r--r--   0        0        0     2148 2023-07-02 17:07:50.084201 aporia-3.1.0/src/aporia/sdk/custom_metrics.py
+-rw-r--r--   0        0        0     1822 2023-07-02 17:07:50.084201 aporia-3.1.0/src/aporia/sdk/dashboards.py
+-rw-r--r--   0        0        0     3610 2023-07-02 17:07:50.084201 aporia-3.1.0/src/aporia/sdk/data_sources.py
+-rw-r--r--   0        0        0     6709 2023-07-02 17:07:50.084201 aporia-3.1.0/src/aporia/sdk/datasets.py
+-rw-r--r--   0        0        0     1844 2023-07-02 17:07:50.084201 aporia-3.1.0/src/aporia/sdk/messaging.py
+-rw-r--r--   0        0        0     6108 2023-07-02 17:07:50.084201 aporia-3.1.0/src/aporia/sdk/metrics.py
+-rw-r--r--   0        0        0     6326 2023-07-02 17:07:50.084201 aporia-3.1.0/src/aporia/sdk/models.py
+-rw-r--r--   0        0        0    85066 2023-07-02 17:07:50.084201 aporia-3.1.0/src/aporia/sdk/monitors.py
+-rw-r--r--   0        0        0     3506 2023-07-02 17:07:50.084201 aporia-3.1.0/src/aporia/sdk/segments.py
+-rw-r--r--   0        0        0     3048 2023-07-02 17:07:50.084201 aporia-3.1.0/src/aporia/sdk/versions.py
+-rw-r--r--   0        0        0     3474 1970-01-01 00:00:00.000000 aporia-3.1.0/PKG-INFO
```

### Comparing `aporia-3.0.0a19/README.md` & `aporia-3.1.0/README.md`

 * *Files identical despite different names*

### Comparing `aporia-3.0.0a19/pyproject.toml` & `aporia-3.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aporia"
-version = "3.0.0a19"
+version = "3.1.0"
 description = ""
 authors = ["Aporia <support@aporia.com>"]
 readme = "README.md"
 packages = [
     { include = "aporia", from = "src" }
 ]
```

### Comparing `aporia-3.0.0a19/src/aporia/as_code/resources/base.py` & `aporia-3.1.0/src/aporia/as_code/resources/base.py`

 * *Files identical despite different names*

### Comparing `aporia-3.0.0a19/src/aporia/as_code/resources/custom_metrics.py` & `aporia-3.1.0/src/aporia/as_code/resources/custom_metrics.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from aporia.sdk.client import Client
 from aporia.sdk.custom_metrics import CustomMetric as _CustomMetric
 
 
 class CustomMetric(BaseResource):
     def __init__(self, resource_name: str, /, *, code: str, name: Optional[str] = None):
         self.name = resource_name
+        self.dependants = []
         if name is None:
             name = resource_name
 
         self._args = {"name": name, "code": code}
 
     def compare(self, resource_data: Dict) -> CompareStatus:
         if all([self._args[k] == resource_data[k] for k in self._args.keys()]):
```

### Comparing `aporia-3.0.0a19/src/aporia/as_code/resources/data_source.py` & `aporia-3.1.0/src/aporia/as_code/resources/data_source.py`

 * *Files identical despite different names*

### Comparing `aporia-3.0.0a19/src/aporia/as_code/resources/dataset.py` & `aporia-3.1.0/src/aporia/as_code/resources/dataset.py`

 * *Files 11% similar despite different names*

```diff
@@ -34,35 +34,35 @@
         schema = DatasetSchema(
             id_column=id_column,
             timestamp_column=timestamp_column,
             raw_inputs=[
                 FieldSchema(name=name, type=FieldType(type)) for name, type in raw_inputs.items()
             ]
             if raw_inputs is not None
-            else None,
+            else [],
             features=[
                 FieldSchema(name=name, type=FieldType(type)) for name, type in features.items()
             ]
             if features is not None
-            else None,
+            else [],
             predictions=[
                 FieldSchema(name=name, type=FieldType(type)) for name, type in predictions.items()
             ]
             if predictions is not None
-            else None,
+            else [],
             actuals=[
                 FieldSchema(
                     name=name,
                     type=FieldType(type),
                     properties={"prediction": actual_mappings[name]},
                 )
                 for name, type in actuals.items()
             ]
             if actuals is not None
-            else None,
+            else [],
         )
 
         if data_source_id is None and data_source_name is None and data_source is None:
             raise ValueError("Must supply data source")
 
         if 1 != sum(
             [
@@ -73,14 +73,20 @@
                     data_source_name,
                 ]
                 if data_source_identifier is not None
             ]
         ):
             raise ValueError("Must supply only one method to find data source")
 
+        self._args = {
+            "dataset_type": type,
+            "connection_data": connection_data,
+            "schema": schema,
+        }
+
         if data_source is not None:
             data_source.dependants.append(
                 (
                     self,
                     lambda data, dataset: dataset.setarg("data_source_id", data["id"]),
                 )
             )
@@ -100,20 +106,14 @@
                         f"Found {len(same_named_data_sources)} data sources named {data_source_name}"
                     )
                 data_source = same_named_data_sources[0]
                 resource.setarg("data_source_id", data_source.id)
 
             self.deferred_load = deferred_load
 
-        self._args = {
-            "dataset_type": type,
-            "connection_data": connection_data,
-            "schema": schema,
-        }
-
     def _compare_schema(self, aporia_schema: Dict, compare_metadata: bool = True) -> bool:
         schema: DatasetSchema = self._args["schema"]
 
         raw_inputs = {
             raw_input.name: json.loads(raw_input.json()) for raw_input in schema.raw_inputs or []
         }
         features = {feature.name: json.loads(feature.json()) for feature in schema.features or []}
```

### Comparing `aporia-3.0.0a19/src/aporia/as_code/resources/model.py` & `aporia-3.1.0/src/aporia/as_code/resources/model.py`

 * *Files identical despite different names*

### Comparing `aporia-3.0.0a19/src/aporia/as_code/resources/segment.py` & `aporia-3.1.0/src/aporia/as_code/resources/version.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,52 +1,58 @@
-from typing import Any, Dict, List, Optional, Tuple, Union
+from typing import Any, Dict, Optional, Tuple
 
-from aporia.as_code.resources.base import BaseResource, CompareStatus
+from aporia.as_code.resources.base import BaseResource, CompareStatus, NonDeletableResourceException
+from aporia.as_code.resources.dataset import Dataset
 from aporia.sdk.client import Client
-from aporia.sdk.segments import Segment as _Segment
+from aporia.sdk.versions import Version as _Version
 
 
-class Segment(BaseResource):
+class Version(BaseResource):
     def __init__(
         self,
         resource_name: str,
         /,
         *,
         name: Optional[str] = None,
-        field: Optional[str] = None,
-        values: Optional[Union[List[str], List[Union[float, int]]]] = None,
-        # TODO: Support new custom segment API
+        serving: Optional[Dataset] = None,
+        training: Optional[Dataset] = None,
     ):
         self.name = resource_name
+        self.dependants = []
+        self.sub_resources = []
         if name is None:
             name = resource_name
 
         self._args = {"name": name}
-        if field is not None:
-            if values is None:
-                raise Exception("Must supply values for automatic segment")
-            self._args["field_name"] = field
-            self._args["values"] = values
+
+        def apply_args(data, dataset):
+            dataset.setarg("version_id", data["id"])
+            dataset.setarg("model_id", data["model_id"])
+
+        if serving is not None:
+            self.sub_resources.append((serving, apply_args))
+        if training is not None:
+            self.sub_resources.append((training, apply_args))
 
     def compare(self, resource_data: Dict) -> CompareStatus:
         if all([self._args[k] == resource_data[k] for k in self._args.keys()]):
             return CompareStatus.SAME
         return CompareStatus.UPDATEABLE
 
     def setarg(self, arg_name: str, arg_value: Any):
         self._args[arg_name] = arg_value
 
     def create(self, client: Client) -> Tuple[str, Dict]:
-        segment = _Segment.create(client=client, **self._args)
-        return segment.id, segment.raw_data
+        version = _Version.create(client=client, **self._args)
+        return version.id, version.raw_data
 
     def read(self, client: Client, id: str) -> Dict:
-        return _Segment.read(client=client, id=id).raw_data
+        return _Version.read(client=client, id=id).raw_data
 
     def update(self, client: Client, id: str) -> Dict:
-        segment = _Segment.read(client=client, id=id)
-        segment.update(**self._args)
-        return segment.raw_data
+        version = _Version.read(client=client, id=id)
+        version.update(**self._args)
+        return version.raw_data
 
     @classmethod
     def delete(cls, client: Client, id: str):
-        _Segment.delete_by_id(client=client, id=id)
+        raise NonDeletableResourceException()
```

### Comparing `aporia-3.0.0a19/src/aporia/sdk/aporia_api.py` & `aporia-3.1.0/src/aporia/sdk/aporia_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -61,14 +61,22 @@
         )
         self._created_resources.append(data_source)
         return data_source
 
     def query_metrics(self, model_id: str, metrics: List[MetricParameters]) -> List:
         return self.metrics_client.query_batch(model_id=model_id, metrics=metrics)
 
+    def get_models(self) -> List[Model]:
+        models = Model.get_all(client=self.client)
+        return models
+
+    def get_data_sources(self) -> List[DataSource]:
+        data_sources = DataSource.get_all(client=self.client)
+        return data_sources
+
     def delete(self):
         for resource in self._created_resources:
             resource.delete()
 
     def __enter__(self):
         return self
```

### Comparing `aporia-3.0.0a19/src/aporia/sdk/base.py` & `aporia-3.1.0/src/aporia/sdk/base.py`

 * *Files identical despite different names*

### Comparing `aporia-3.0.0a19/src/aporia/sdk/client.py` & `aporia-3.1.0/src/aporia/sdk/client.py`

 * *Files identical despite different names*

### Comparing `aporia-3.0.0a19/src/aporia/sdk/custom_metrics.py` & `aporia-3.1.0/src/aporia/sdk/custom_metrics.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 class CustomMetric(BaseAporiaResource):
     def __init__(self, client: Client, data: Dict):
         self.client = client
         self.__update_members(data)
 
     def __update_members(self, data: Dict):
         self.id = data["id"]
+        self.name = data["name"]
         self.raw_data = data
 
     @classmethod
     def get_all(cls, client: Client, model_id: Optional[str] = None) -> List["CustomMetric"]:
         response = client.send_request(
             f"/custom-metrics{'' if model_id is None else f'?model_id={model_id}'}", "GET"
         )
```

### Comparing `aporia-3.0.0a19/src/aporia/sdk/dashboards.py` & `aporia-3.1.0/src/aporia/sdk/dashboards.py`

 * *Files identical despite different names*

### Comparing `aporia-3.0.0a19/src/aporia/sdk/data_sources.py` & `aporia-3.1.0/src/aporia/sdk/data_sources.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,16 @@
     BIGQUERY = "bigquery"
     POSTGRES = "postgres"
     SNOWFLAKE = "snowflake"
     REDSHIFT = "redshift"
     DATABRICKS = "databricks"
     AZURE_BLOB_STORAGE = "azure_blob_storage"
     SNOWFLAKE_NATIVE = "snowflake_native"
+    GOOGLE_CLOUD_STORAGE = "google_cloud_storage"
+    HIVE = "hive"
 
 
 class DataSource(BaseAporiaResource):
     def __init__(self, client: Client, data: Dict):
         self.client = client
         self.__update_members(data)
 
@@ -45,15 +47,15 @@
         data_source_type: DataSourceType,
         connection_data: Dict[str, Any],
     ) -> "DataSource":
         existing_data_sources = cls.get_all(client=client)
 
         for data_source in existing_data_sources:
             if data_source.name == name:
-                if data_source.type is data_source_type:
+                if data_source.type != data_source_type:
                     raise RuntimeError(
                         f"Data source {name} already exists but is of different type (expected {data_source_type.value}, received {data_source.type.value})"
                     )
                 print(f"Data source {name} already exists! Using it. Check configuration")
                 return data_source
 
         response = client.send_request(
```

### Comparing `aporia-3.0.0a19/src/aporia/sdk/datasets.py` & `aporia-3.1.0/src/aporia/sdk/datasets.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     BOOLEAN = "boolean"
     NUMERIC = "numeric"
     DATETIME = "datetime"
     CATEGORICAL = "categorical"
     TEXT = "text"
     ARRAY = "array"
     EMBEDDING = "embedding"
+    IMAGE_URL = "image_url"
 
 
 class FieldSchema(BaseModel):
     name: str
     type: FieldType
     properties: Optional[Dict[str, Any]] = None
 
@@ -45,16 +46,19 @@
         self.__update_members(data)
 
     def __update_members(self, data: Dict):
         self.raw_data = data
         self.id = data["id"]
 
     @classmethod
-    def get_all(cls, client: Client) -> List["Dataset"]:
-        response = client.send_request("/datasets", "GET")
+    def get_all(cls, client: Client, model_version_id: Optional[str] = None) -> List["Dataset"]:
+        response = client.send_request(
+            f"/datasets{'' if model_version_id is None else f'?model_version_id={model_version_id}'}",
+            "GET",
+        )
 
         client.assert_response(response)
 
         return [cls(client=client, data=entry) for entry in response.json()]
 
     @classmethod
     def create(
```

### Comparing `aporia-3.0.0a19/src/aporia/sdk/metrics.py` & `aporia-3.1.0/src/aporia/sdk/metrics.py`

 * *Files identical despite different names*

### Comparing `aporia-3.0.0a19/src/aporia/sdk/models.py` & `aporia-3.1.0/src/aporia/sdk/models.py`

 * *Files 9% similar despite different names*

```diff
@@ -55,15 +55,18 @@
 
     def __update_members(self, data: Dict):
         self.raw_data = data
         self.id = data["id"]
         self.name = data["name"]
         self.type = ModelType(data["type"])
         self.description = data["description"]
-        self.color = ModelColor(data["color"])
+        try:
+            self.color = ModelColor(data["color"])
+        except Exception:
+            self.color = data["color"]
         self.icon = ModelIcon(data["icon"])
         self.owner = data["owner"]
 
     @classmethod
     def get_all(cls, client: Client) -> List["Model"]:
         response = client.send_request("/models", "GET")
 
@@ -179,7 +182,23 @@
             creator=creator,
             is_active=is_active,
         )
         return monitor
 
     def create_dashboard(self, widgets: List[Widget]):
         pass
+
+    def get_versions(self) -> List[Version]:
+        versions = Version.get_all(client=self.client, model_id=self.id)
+        return versions
+
+    def get_segments(self) -> List[Segment]:
+        segments = Segment.get_all(client=self.client, model_id=self.id)
+        return segments
+
+    def get_custom_metrics(self) -> List[CustomMetric]:
+        custom_metrics = CustomMetric.get_all(client=self.client, model_id=self.id)
+        return custom_metrics
+
+    def get_monitors(self) -> List[Monitor]:
+        monitors = Monitor.get_all(client=self.client, model_id=self.id)
+        return monitors
```

### Comparing `aporia-3.0.0a19/src/aporia/sdk/segments.py` & `aporia-3.1.0/src/aporia/sdk/segments.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from typing import Dict, List, Optional, Union
+from typing import Dict, List, Optional, Tuple, Union
+from urllib.parse import urlencode
 
 from aporia.sdk.base import BaseAporiaResource
 from aporia.sdk.client import Client
 
 
 class Segment(BaseAporiaResource):
     def __init__(self, client: Client, data: Dict):
@@ -14,36 +15,45 @@
         self.id = data["id"]
         self.name = data["name"]
         self.field = data["field"]
         self.values = data["values"]
         self.term = data["term"]
 
     @classmethod
-    def get_all(cls, client: Client, model_id: Optional[str] = None) -> List["Segment"]:
+    def get_all(
+        cls, client: Client, model_id: Optional[str] = None, manual_only: bool = True
+    ) -> List["Segment"]:
+        url_params = {}
+        if manual_only:
+            url_params["is_manually_created"] = "true"
+        if model_id is not None:
+            url_params["model_id"] = model_id
+        encoded_url_params = urlencode(url_params)
         response = client.send_request(
-            f"/data-segments{'' if model_id is None else f'?model_id={model_id}'}", "GET"
+            f"/data-segments{f'?{encoded_url_params}' if len(url_params) > 0 else f''}",
+            "GET",
         )
 
         client.assert_response(response)
 
         return [cls(client=client, data=entry) for entry in response.json()]
 
     @classmethod
     def create(
         cls,
         client: Client,
         name: str,
         model_id: str,
         field_name: Optional[str] = None,
         values: Optional[Union[List[str], List[Union[float, int]]]] = None,
-        term: Optional[str] = None,
+        terms: Optional[List[Tuple[str, str]]] = None,
     ) -> "Segment":
         segment_data = {}
-        if term is not None:
-            segment_data["term"] = term
+        if terms is not None:
+            segment_data["terms_values"] = terms
         else:
             segment_data["field_name"] = field_name
             segment_data["values"] = values
         response = client.send_request(
             "/data-segments",
             "POST",
             {"name": name, "model_id": model_id, **segment_data},
@@ -58,29 +68,35 @@
         response = client.send_request(f"/data-segments/{id}", "GET")
         client.assert_response(response)
         return cls(client=client, data=response.json())
 
     def update(
         self,
         name: Optional[str] = None,
-        field_name: Optional[str] = None,
+        # field_name: Optional[str] = None,
         values: Optional[Union[List[str], List[Union[float, int]]]] = None,
         term: Optional[str] = None,
         **kwargs,
     ):
         args = {}
         if name is not None:
             args["name"] = name
-        if field_name is not None:
-            args["field_name"] = field_name
+        # if field_name is not None:
+        #     args["field_name"] = field_name
         if values is not None:
             args["values"] = values
         if term is not None:
             args["term"] = term
-        response = self.client.send_request(f"/data-segments/{self.id}", "PUT", args)
+        response = self.client.send_request(
+            f"/data-segments/{self.id}",
+            "POST",
+            args,
+            url_search_replace=("/api/v1/", "/v1/crud-service/"),
+        )
+        # response = self.client.send_request(f"/data-segments/{self.id}", "PUT", args)
         self.client.assert_response(response)
         self.__update_members(response.json())
 
     def delete(self):
         response = self.client.send_request(f"/data-segments/{self.id}", "DELETE")
         self.client.assert_response(response)
```

### Comparing `aporia-3.0.0a19/src/aporia/sdk/versions.py` & `aporia-3.1.0/src/aporia/sdk/versions.py`

 * *Files 8% similar despite different names*

```diff
@@ -85,7 +85,11 @@
 
     def delete(self):
         raise NotImplementedError()
 
     @staticmethod
     def delete_by_id(client: Client, id: str):
         raise NotImplementedError()
+
+    def get_datasets(self) -> list[Dataset]:
+        datasets = Dataset.get_all(client=self.client, model_version_id=self.id)
+        return datasets
```

### Comparing `aporia-3.0.0a19/PKG-INFO` & `aporia-3.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aporia
-Version: 3.0.0a19
+Version: 3.1.0
 Summary: 
 Author: Aporia
 Author-email: support@aporia.com
 Requires-Python: >=3.8,<=3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

