# Comparing `tmp/aporia-3.0.0a18.tar.gz` & `tmp/aporia-3.0.0a19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aporia-3.0.0a18.tar", max compression
+gzip compressed data, was "aporia-3.0.0a19.tar", max compression
```

## Comparing `aporia-3.0.0a18.tar` & `aporia-3.0.0a19.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     2968 2023-05-22 00:50:02.478388 aporia-3.0.0a18/README.md
--rw-r--r--   0        0        0      833 2023-05-22 00:50:02.478388 aporia-3.0.0a18/pyproject.toml
--rw-r--r--   0        0        0      168 2023-05-22 00:50:02.478388 aporia-3.0.0a18/src/aporia/__init__.py
--rw-r--r--   0        0        0      540 2023-05-22 00:50:02.478388 aporia-3.0.0a18/src/aporia/as_code/__init__.py
--rw-r--r--   0        0        0      926 2023-05-22 00:50:02.478388 aporia-3.0.0a18/src/aporia/as_code/resources/base.py
--rw-r--r--   0        0        0     1410 2023-05-22 00:50:02.478388 aporia-3.0.0a18/src/aporia/as_code/resources/custom_metrics.py
--rw-r--r--   0        0        0     1945 2023-05-22 00:50:02.478388 aporia-3.0.0a18/src/aporia/as_code/resources/data_source.py
--rw-r--r--   0        0        0     7124 2023-05-22 00:50:02.478388 aporia-3.0.0a18/src/aporia/as_code/resources/dataset.py
--rw-r--r--   0        0        0     3779 2023-05-22 00:50:02.478388 aporia-3.0.0a18/src/aporia/as_code/resources/model.py
--rw-r--r--   0        0        0     1344 2023-05-22 00:50:02.478388 aporia-3.0.0a18/src/aporia/as_code/resources/monitor.py
--rw-r--r--   0        0        0     1721 2023-05-22 00:50:02.478388 aporia-3.0.0a18/src/aporia/as_code/resources/segment.py
--rw-r--r--   0        0        0     1885 2023-05-22 00:50:02.478388 aporia-3.0.0a18/src/aporia/as_code/resources/version.py
--rw-r--r--   0        0        0    12757 2023-05-22 00:50:02.478388 aporia-3.0.0a18/src/aporia/as_code/stack.py
--rw-r--r--   0        0        0        0 2023-05-22 00:50:02.478388 aporia-3.0.0a18/src/aporia/sdk/__init__.py
--rw-r--r--   0        0        0     2928 2023-05-22 00:50:02.478388 aporia-3.0.0a18/src/aporia/sdk/aporia_api.py
--rw-r--r--   0        0        0      699 2023-05-22 00:50:02.478388 aporia-3.0.0a18/src/aporia/sdk/base.py
--rw-r--r--   0        0        0     1480 2023-05-22 00:50:02.478388 aporia-3.0.0a18/src/aporia/sdk/client.py
--rw-r--r--   0        0        0     2071 2023-05-22 00:50:02.478388 aporia-3.0.0a18/src/aporia/sdk/custom_metrics.py
--rw-r--r--   0        0        0     1810 2023-05-22 00:50:02.478388 aporia-3.0.0a18/src/aporia/sdk/dashboards.py
--rw-r--r--   0        0        0     3530 2023-05-22 00:50:02.478388 aporia-3.0.0a18/src/aporia/sdk/data_sources.py
--rw-r--r--   0        0        0     6479 2023-05-22 00:50:02.478388 aporia-3.0.0a18/src/aporia/sdk/datasets.py
--rw-r--r--   0        0        0     6077 2023-05-22 00:50:02.478388 aporia-3.0.0a18/src/aporia/sdk/metrics.py
--rw-r--r--   0        0        0     5549 2023-05-22 00:50:02.478388 aporia-3.0.0a18/src/aporia/sdk/models.py
--rw-r--r--   0        0        0    18647 2023-05-22 00:50:02.478388 aporia-3.0.0a18/src/aporia/sdk/monitors.py
--rw-r--r--   0        0        0     2840 2023-05-22 00:50:02.478388 aporia-3.0.0a18/src/aporia/sdk/segments.py
--rw-r--r--   0        0        0     2872 2023-05-22 00:50:02.478388 aporia-3.0.0a18/src/aporia/sdk/versions.py
--rw-r--r--   0        0        0     3378 1970-01-01 00:00:00.000000 aporia-3.0.0a18/PKG-INFO
+-rw-r--r--   0        0        0     2968 2023-06-20 23:37:32.344442 aporia-3.0.0a19/README.md
+-rw-r--r--   0        0        0      832 2023-06-20 23:37:32.348442 aporia-3.0.0a19/pyproject.toml
+-rw-r--r--   0        0        0      168 2023-06-20 23:37:32.348442 aporia-3.0.0a19/src/aporia/__init__.py
+-rw-r--r--   0        0        0      540 2023-06-20 23:37:32.348442 aporia-3.0.0a19/src/aporia/as_code/__init__.py
+-rw-r--r--   0        0        0      939 2023-06-20 23:37:32.348442 aporia-3.0.0a19/src/aporia/as_code/resources/base.py
+-rw-r--r--   0        0        0     1436 2023-06-20 23:37:32.348442 aporia-3.0.0a19/src/aporia/as_code/resources/custom_metrics.py
+-rw-r--r--   0        0        0     1984 2023-06-20 23:37:32.348442 aporia-3.0.0a19/src/aporia/as_code/resources/data_source.py
+-rw-r--r--   0        0        0     7214 2023-06-20 23:37:32.348442 aporia-3.0.0a19/src/aporia/as_code/resources/dataset.py
+-rw-r--r--   0        0        0     3854 2023-06-20 23:37:32.348442 aporia-3.0.0a19/src/aporia/as_code/resources/model.py
+-rw-r--r--   0        0        0     1370 2023-06-20 23:37:32.348442 aporia-3.0.0a19/src/aporia/as_code/resources/monitor.py
+-rw-r--r--   0        0        0     1778 2023-06-20 23:37:32.348442 aporia-3.0.0a19/src/aporia/as_code/resources/segment.py
+-rw-r--r--   0        0        0     1917 2023-06-20 23:37:32.348442 aporia-3.0.0a19/src/aporia/as_code/resources/version.py
+-rw-r--r--   0        0        0    12813 2023-06-20 23:37:32.348442 aporia-3.0.0a19/src/aporia/as_code/stack.py
+-rw-r--r--   0        0        0        0 2023-06-20 23:37:32.348442 aporia-3.0.0a19/src/aporia/sdk/__init__.py
+-rw-r--r--   0        0        0     2975 2023-06-20 23:37:32.348442 aporia-3.0.0a19/src/aporia/sdk/aporia_api.py
+-rw-r--r--   0        0        0      723 2023-06-20 23:37:32.348442 aporia-3.0.0a19/src/aporia/sdk/base.py
+-rw-r--r--   0        0        0     1531 2023-06-20 23:37:32.348442 aporia-3.0.0a19/src/aporia/sdk/client.py
+-rw-r--r--   0        0        0     2115 2023-06-20 23:37:32.348442 aporia-3.0.0a19/src/aporia/sdk/custom_metrics.py
+-rw-r--r--   0        0        0     1822 2023-06-20 23:37:32.348442 aporia-3.0.0a19/src/aporia/sdk/dashboards.py
+-rw-r--r--   0        0        0     3542 2023-06-20 23:37:32.348442 aporia-3.0.0a19/src/aporia/sdk/data_sources.py
+-rw-r--r--   0        0        0     6528 2023-06-20 23:37:32.348442 aporia-3.0.0a19/src/aporia/sdk/datasets.py
+-rw-r--r--   0        0        0     6108 2023-06-20 23:37:32.348442 aporia-3.0.0a19/src/aporia/sdk/metrics.py
+-rw-r--r--   0        0        0     5644 2023-06-20 23:37:32.348442 aporia-3.0.0a19/src/aporia/sdk/models.py
+-rw-r--r--   0        0        0    18814 2023-06-20 23:37:32.348442 aporia-3.0.0a19/src/aporia/sdk/monitors.py
+-rw-r--r--   0        0        0     2936 2023-06-20 23:37:32.348442 aporia-3.0.0a19/src/aporia/sdk/segments.py
+-rw-r--r--   0        0        0     2897 2023-06-20 23:37:32.348442 aporia-3.0.0a19/src/aporia/sdk/versions.py
+-rw-r--r--   0        0        0     3477 1970-01-01 00:00:00.000000 aporia-3.0.0a19/PKG-INFO
```

### Comparing `aporia-3.0.0a18/README.md` & `aporia-3.0.0a19/README.md`

 * *Files identical despite different names*

### Comparing `aporia-3.0.0a18/pyproject.toml` & `aporia-3.0.0a19/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "aporia"
-version = "3.0.0a18"
+version = "3.0.0a19"
 description = ""
 authors = ["Aporia <support@aporia.com>"]
 readme = "README.md"
 packages = [
     { include = "aporia", from = "src" }
 ]
 
 [tool.poetry.dependencies]
-python = ">=3.10, <=3.11"
+python = ">=3.8, <=3.11"
 pydantic = "^1.10"
 requests = "^2.28"
 
 [tool.poetry.group.dev.dependencies]
 black = "^22.12.0"
 isort = "~5.10.1"
 mypy = "~0.982"
```

### Comparing `aporia-3.0.0a18/src/aporia/as_code/__init__.py` & `aporia-3.0.0a19/src/aporia/as_code/__init__.py`

 * *Files identical despite different names*

### Comparing `aporia-3.0.0a18/src/aporia/as_code/resources/base.py` & `aporia-3.0.0a19/src/aporia/as_code/resources/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from abc import ABC, abstractmethod
 from enum import Enum
-from typing import Any
+from typing import Any, Dict, Tuple
 
 from aporia.sdk.client import Client
 
 
 class NonDeletableResourceException(Exception):
     pass
 
@@ -17,29 +17,29 @@
 
 class BaseResource(ABC):
     @abstractmethod
     def __init__(self, resource_name: str, /, **kwargs):
         ...
 
     @abstractmethod
-    def compare(self, resource_data: dict) -> CompareStatus:
+    def compare(self, resource_data: Dict) -> CompareStatus:
         ...
 
     @abstractmethod
     def setarg(self, arg_name: str, arg_value: Any):
         ...
 
     @abstractmethod
-    def create(self, client: Client) -> tuple[str, dict]:
+    def create(self, client: Client) -> Tuple[str, Dict]:
         ...
 
     @abstractmethod
-    def read(self, client: Client, id: str) -> dict:
+    def read(self, client: Client, id: str) -> Dict:
         ...
 
     @abstractmethod
-    def update(self, client: Client, id: str) -> dict:
+    def update(self, client: Client, id: str) -> Dict:
         ...
 
     @abstractmethod
     def delete(self, client: Client, id: str):
         ...
```

### Comparing `aporia-3.0.0a18/src/aporia/as_code/resources/custom_metrics.py` & `aporia-3.0.0a19/src/aporia/as_code/resources/custom_metrics.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-from typing import Any
+from typing import Any, Dict, Optional, Tuple
 
 from aporia.as_code.resources.base import BaseResource, CompareStatus
 from aporia.sdk.client import Client
 from aporia.sdk.custom_metrics import CustomMetric as _CustomMetric
 
 
 class CustomMetric(BaseResource):
-    def __init__(self, resource_name: str, /, *, code: str, name: str | None = None):
+    def __init__(self, resource_name: str, /, *, code: str, name: Optional[str] = None):
         self.name = resource_name
         if name is None:
             name = resource_name
 
         self._args = {"name": name, "code": code}
 
-    def compare(self, resource_data: dict) -> CompareStatus:
+    def compare(self, resource_data: Dict) -> CompareStatus:
         if all([self._args[k] == resource_data[k] for k in self._args.keys()]):
             return CompareStatus.SAME
         return CompareStatus.UPDATEABLE
 
     def setarg(self, arg_name: str, arg_value: Any):
         self._args[arg_name] = arg_value
 
-    def create(self, client: Client) -> tuple[str, dict]:
+    def create(self, client: Client) -> Tuple[str, Dict]:
         custom_metric = _CustomMetric.create(client=client, **self._args)
         return custom_metric.id, custom_metric.raw_data
 
-    def read(self, client: Client, id: str) -> dict:
+    def read(self, client: Client, id: str) -> Dict:
         return _CustomMetric.read(client=client, id=id).raw_data
 
-    def update(self, client: Client, id: str) -> dict:
+    def update(self, client: Client, id: str) -> Dict:
         custom_metric = _CustomMetric.read(client=client, id=id)
         custom_metric.update(**self._args)
         return custom_metric.raw_data
 
     @classmethod
     def delete(cls, client: Client, id: str):
         _CustomMetric.delete_by_id(client=client, id=id)
```

### Comparing `aporia-3.0.0a18/src/aporia/as_code/resources/data_source.py` & `aporia-3.0.0a19/src/aporia/as_code/resources/data_source.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,59 +1,59 @@
-from typing import Any
+from typing import Any, Dict, Optional, Tuple, Union
 
 from aporia.as_code.resources.base import BaseResource, CompareStatus
 from aporia.sdk.client import Client
 from aporia.sdk.data_sources import DataSource as _DataSource
 from aporia.sdk.data_sources import DataSourceType
 
 
 class DataSource(BaseResource):
     def __init__(
         self,
         resource_name: str,
         /,
         *,
-        type: DataSourceType | str,
-        connection_data: dict[str, Any],
-        name: str | None = None,
+        type: Union[DataSourceType, str],
+        connection_data: Dict[str, Any],
+        name: Optional[str] = None,
     ):
         self.dependants = []
         self.name = resource_name
         if name is None:
             name = resource_name
 
         self._args = {
             "name": name,
             "data_source_type": DataSourceType(type),
             "connection_data": connection_data,
         }
 
-    def compare(self, resource_data: dict) -> CompareStatus:
+    def compare(self, resource_data: Dict) -> CompareStatus:
         if all(
             [
                 self._args["name"] == resource_data["name"],
                 self._args["data_source_type"].value == resource_data["type"],
                 # TODO: Data source configuration isn't getable
                 # self._args["connection_data"] == resource_data["connection"],
             ]
         ):
             return CompareStatus.SAME
         return CompareStatus.MISMATCHED
 
     def setarg(self, arg_name: str, arg_value: Any):
         self._args[arg_name] = arg_value
 
-    def create(self, client: Client) -> tuple[str, dict]:
+    def create(self, client: Client) -> Tuple[str, Dict]:
         data_source = _DataSource.create(client=client, **self._args)
         return data_source.id, data_source.raw_data
 
-    def read(self, client: Client, id: str) -> dict:
+    def read(self, client: Client, id: str) -> Dict:
         return _DataSource.read(client=client, id=id).raw_data
 
-    def update(self, client: Client, id: str) -> dict:
+    def update(self, client: Client, id: str) -> Dict:
         data_source = _DataSource.read(client=client, id=id)
         data_source.update(**self._args)
         return data_source.raw_data
 
     @classmethod
     def delete(cls, client: Client, id: str):
         _DataSource.delete_by_id(client=client, id=id)
```

### Comparing `aporia-3.0.0a18/src/aporia/as_code/resources/dataset.py` & `aporia-3.0.0a19/src/aporia/as_code/resources/dataset.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import json
-from typing import Any
+from typing import Any, Dict, Optional, Tuple, Union
 
 from aporia.as_code.resources.base import BaseResource, CompareStatus, NonDeletableResourceException
 from aporia.as_code.resources.data_source import DataSource
 from aporia.sdk.client import Client
 from aporia.sdk.data_sources import DataSource as _DataSource
 from aporia.sdk.datasets import Dataset as _Dataset
 from aporia.sdk.datasets import DatasetSchema, DatasetType, FieldSchema, FieldType
@@ -11,26 +11,26 @@
 
 class Dataset(BaseResource):
     def __init__(
         self,
         resource_name: str,
         /,
         *,
-        type: DatasetType | str,
-        connection_data: dict[str, Any],
-        id_column: str | None = None,
-        timestamp_column: str | None = None,
-        raw_inputs: dict[str, FieldType | str] | None = None,
-        features: dict[str, FieldType | str] | None = None,
-        predictions: dict[str, FieldType | str] | None = None,
-        actuals: dict[str, FieldType | str] | None = None,
-        actual_mappings: dict[str, str] | None = None,
-        data_source_name: str | None = None,
-        data_source_id: str | None = None,
-        data_source: DataSource | None = None,
+        type: Union[DatasetType, str],
+        connection_data: Dict[str, Any],
+        id_column: Optional[str] = None,
+        timestamp_column: Optional[str] = None,
+        raw_inputs: Optional[Dict[str, Union[FieldType, str]]] = None,
+        features: Optional[Dict[str, Union[FieldType, str]]] = None,
+        predictions: Optional[Dict[str, Union[FieldType, str]]] = None,
+        actuals: Optional[Dict[str, Union[FieldType, str]]] = None,
+        actual_mappings: Optional[Dict[str, str]] = None,
+        data_source_name: Optional[str] = None,
+        data_source_id: Optional[str] = None,
+        data_source: Optional[DataSource] = None,
     ):
         self.name = resource_name
         type = DatasetType(type)
 
         schema = DatasetSchema(
             id_column=id_column,
             timestamp_column=timestamp_column,
@@ -106,15 +106,15 @@
 
         self._args = {
             "dataset_type": type,
             "connection_data": connection_data,
             "schema": schema,
         }
 
-    def _compare_schema(self, aporia_schema: dict, compare_metadata: bool = True) -> bool:
+    def _compare_schema(self, aporia_schema: Dict, compare_metadata: bool = True) -> bool:
         schema: DatasetSchema = self._args["schema"]
 
         raw_inputs = {
             raw_input.name: json.loads(raw_input.json()) for raw_input in schema.raw_inputs or []
         }
         features = {feature.name: json.loads(feature.json()) for feature in schema.features or []}
         predictions = {
@@ -141,15 +141,15 @@
             features == schema_features,
             predictions == schema_predictions,
             actuals == schema_actuals,
         ]
 
         return all(checks)
 
-    def compare(self, resource_data: dict) -> CompareStatus:
+    def compare(self, resource_data: Dict) -> CompareStatus:
         if all(
             [
                 self._args["dataset_type"].value == resource_data["stage"],
                 self._args["connection_data"] == resource_data["config"],
                 self._compare_schema(resource_data["schema"]),
                 # TODO: Find a way to validate data source
                 self._args["version_id"] == resource_data["model_version_id"],
@@ -166,22 +166,22 @@
             return CompareStatus.MISMATCHED
         else:
             return CompareStatus.UPDATEABLE
 
     def setarg(self, arg_name: str, arg_value: Any):
         self._args[arg_name] = arg_value
 
-    def create(self, client: Client) -> tuple[str, dict]:
+    def create(self, client: Client) -> Tuple[str, Dict]:
         dataset = _Dataset.create(client=client, **self._args)
         return dataset.id, dataset.raw_data
 
-    def read(self, client: Client, id: str) -> dict:
+    def read(self, client: Client, id: str) -> Dict:
         return _Dataset.read(client=client, id=id).raw_data
 
-    def update(self, client: Client, id: str) -> dict:
+    def update(self, client: Client, id: str) -> Dict:
         dataset = _Dataset.read(client=client, id=id)
         dataset.update(**self._args)
         return dataset.raw_data
 
     @classmethod
     def delete(cls, client: Client, id: str):
         raise NonDeletableResourceException()
```

### Comparing `aporia-3.0.0a18/src/aporia/as_code/resources/model.py` & `aporia-3.0.0a19/src/aporia/as_code/resources/model.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from enum import Enum
-from typing import Any
+from typing import Any, Dict, List, Optional, Tuple, Union
 
 from aporia.as_code.resources.base import BaseResource, CompareStatus
 from aporia.as_code.resources.custom_metrics import CustomMetric
 from aporia.as_code.resources.monitor import Monitor
 from aporia.as_code.resources.segment import Segment
 from aporia.as_code.resources.version import Version
 from aporia.sdk.client import Client
@@ -14,25 +14,25 @@
 class Model(BaseResource):
     def __init__(
         self,
         resource_name: str,
         /,
         *,
         # Model args
-        type: ModelType | str,
-        name: str | None = None,
-        description: str | None = None,
-        icon: ModelIcon | None = None,
-        color: ModelColor | None = None,
-        owner: str | None | NoOwner = NoOwner(),
+        type: Union[ModelType, str],
+        name: Optional[str] = None,
+        description: Optional[str] = None,
+        icon: Optional[ModelIcon] = None,
+        color: Optional[ModelColor] = None,
+        owner: Optional[Union[str, NoOwner]] = NoOwner(),
         # Model sub-resources
-        versions: list[Version] | None = None,
-        segments: list[Segment] | None = None,
-        custom_metrics: list[CustomMetric] | None = None,
-        monitors: list[Monitor] | None = None,
+        versions: Optional[List[Version]] = None,
+        segments: Optional[List[Segment]] = None,
+        custom_metrics: Optional[List[CustomMetric]] = None,
+        monitors: Optional[List[Monitor]] = None,
     ):
         self.sub_resources = []
         self.name = resource_name
         if name is None:
             name = resource_name
 
         type = ModelType(type)
@@ -65,15 +65,15 @@
                 )
             )
         for monitor in monitors or []:
             self.sub_resources.append(
                 (monitor, lambda data, monitor: monitor.setarg("model_id", data["id"]))
             )
 
-    def compare(self, resource_data: dict) -> CompareStatus:
+    def compare(self, resource_data: Dict) -> CompareStatus:
         checks = [
             self._args["name"] == resource_data["name"],
             self._args["model_type"].value == resource_data["type"],
         ]
         for k in ["description", "icon", "color", "owner"]:
             if k in self._args:
                 if isinstance(self._args[k], Enum):
@@ -83,22 +83,22 @@
         if all(checks):
             return CompareStatus.SAME
         return CompareStatus.UPDATEABLE
 
     def setarg(self, arg_name: str, arg_value: Any):
         self._args[arg_name] = arg_value
 
-    def create(self, client: Client) -> tuple[str, dict]:
+    def create(self, client: Client) -> Tuple[str, Dict]:
         model = _Model.create(client=client, **self._args)
         return model.id, model.raw_data
 
-    def read(self, client: Client, id: str) -> dict:
+    def read(self, client: Client, id: str) -> Dict:
         return _Model.read(client=client, id=id).raw_data
 
-    def update(self, client: Client, id: str) -> dict:
+    def update(self, client: Client, id: str) -> Dict:
         model = _Model.read(client=client, id=id)
         model.update(**self._args)
         return model.raw_data
 
     @classmethod
     def delete(cls, client: Client, id: str):
         _Model.delete_by_id(client=client, id=id)
```

### Comparing `aporia-3.0.0a18/src/aporia/as_code/resources/monitor.py` & `aporia-3.0.0a19/src/aporia/as_code/resources/monitor.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-from typing import Any
+from typing import Any, Dict, Optional, Tuple
 
 from aporia.as_code.resources.base import BaseResource, CompareStatus
 from aporia.sdk.client import Client
 from aporia.sdk.monitors import Monitor as _Monitor
 
 
 class Monitor(BaseResource):
-    def __init__(self, resource_name: str, /, *, name: str | None = None):
+    def __init__(self, resource_name: str, /, *, name: Optional[str] = None):
         raise NotImplementedError()
         self.name = resource_name
         if name is None:
             name = resource_name
 
         self._args = {"name": name}
 
     def setarg(self, arg_name: str, arg_value: Any):
         self._args[arg_name] = arg_value
 
-    def compare(self, resource_data: dict) -> CompareStatus:
+    def compare(self, resource_data: Dict) -> CompareStatus:
         if all([self._args[k] == resource_data[k] for k in self._args.keys()]):
             return CompareStatus.SAME
         return CompareStatus.UPDATEABLE
 
-    def create(self, client: Client) -> tuple[str, dict]:
+    def create(self, client: Client) -> Tuple[str, Dict]:
         monitor = _Monitor.create(client=client, **self._args)
         return monitor.id, monitor.raw_data
 
-    def read(self, client: Client, id: str) -> dict:
+    def read(self, client: Client, id: str) -> Dict:
         return _Monitor.read(client=client, id=id).raw_data
 
-    def update(self, client: Client, id: str) -> dict:
+    def update(self, client: Client, id: str) -> Dict:
         monitor = _Monitor.read(client=client, id=id)
         monitor.update(**self._args)
         return monitor.raw_data
 
     @classmethod
     def delete(cls, client: Client, id: str):
         _Monitor.delete_by_id(client=client, id=id)
```

### Comparing `aporia-3.0.0a18/src/aporia/as_code/resources/segment.py` & `aporia-3.0.0a19/src/aporia/as_code/resources/segment.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,52 +1,52 @@
-from typing import Any
+from typing import Any, Dict, List, Optional, Tuple, Union
 
 from aporia.as_code.resources.base import BaseResource, CompareStatus
 from aporia.sdk.client import Client
 from aporia.sdk.segments import Segment as _Segment
 
 
 class Segment(BaseResource):
     def __init__(
         self,
         resource_name: str,
         /,
         *,
-        name: str | None = None,
-        field: str | None = None,
-        values: list[str] | list[float | int] | None = None,
+        name: Optional[str] = None,
+        field: Optional[str] = None,
+        values: Optional[Union[List[str], List[Union[float, int]]]] = None,
         # TODO: Support new custom segment API
     ):
         self.name = resource_name
         if name is None:
             name = resource_name
 
         self._args = {"name": name}
         if field is not None:
             if values is None:
                 raise Exception("Must supply values for automatic segment")
             self._args["field_name"] = field
             self._args["values"] = values
 
-    def compare(self, resource_data: dict) -> CompareStatus:
+    def compare(self, resource_data: Dict) -> CompareStatus:
         if all([self._args[k] == resource_data[k] for k in self._args.keys()]):
             return CompareStatus.SAME
         return CompareStatus.UPDATEABLE
 
     def setarg(self, arg_name: str, arg_value: Any):
         self._args[arg_name] = arg_value
 
-    def create(self, client: Client) -> tuple[str, dict]:
+    def create(self, client: Client) -> Tuple[str, Dict]:
         segment = _Segment.create(client=client, **self._args)
         return segment.id, segment.raw_data
 
-    def read(self, client: Client, id: str) -> dict:
+    def read(self, client: Client, id: str) -> Dict:
         return _Segment.read(client=client, id=id).raw_data
 
-    def update(self, client: Client, id: str) -> dict:
+    def update(self, client: Client, id: str) -> Dict:
         segment = _Segment.read(client=client, id=id)
         segment.update(**self._args)
         return segment.raw_data
 
     @classmethod
     def delete(cls, client: Client, id: str):
         _Segment.delete_by_id(client=client, id=id)
```

### Comparing `aporia-3.0.0a18/src/aporia/as_code/resources/version.py` & `aporia-3.0.0a19/src/aporia/as_code/resources/version.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-from typing import Any
+from typing import Any, Dict, Optional, Tuple
 
 from aporia.as_code.resources.base import BaseResource, CompareStatus, NonDeletableResourceException
 from aporia.as_code.resources.dataset import Dataset
 from aporia.sdk.client import Client
 from aporia.sdk.versions import Version as _Version
 
 
 class Version(BaseResource):
     def __init__(
         self,
         resource_name: str,
         /,
         *,
-        name: str | None = None,
-        serving: Dataset | None = None,
-        training: Dataset | None = None,
+        name: Optional[str] = None,
+        serving: Optional[Dataset] = None,
+        training: Optional[Dataset] = None,
     ):
         self.name = resource_name
         self.sub_resources = []
         if name is None:
             name = resource_name
 
         self._args = {"name": name}
@@ -28,30 +28,30 @@
             dataset.setarg("model_id", data["model_id"])
 
         if serving is not None:
             self.sub_resources.append((serving, apply_args))
         if training is not None:
             self.sub_resources.append((training, apply_args))
 
-    def compare(self, resource_data: dict) -> CompareStatus:
+    def compare(self, resource_data: Dict) -> CompareStatus:
         if all([self._args[k] == resource_data[k] for k in self._args.keys()]):
             return CompareStatus.SAME
         return CompareStatus.UPDATEABLE
 
     def setarg(self, arg_name: str, arg_value: Any):
         self._args[arg_name] = arg_value
 
-    def create(self, client: Client) -> tuple[str, dict]:
+    def create(self, client: Client) -> Tuple[str, Dict]:
         version = _Version.create(client=client, **self._args)
         return version.id, version.raw_data
 
-    def read(self, client: Client, id: str) -> dict:
+    def read(self, client: Client, id: str) -> Dict:
         return _Version.read(client=client, id=id).raw_data
 
-    def update(self, client: Client, id: str) -> dict:
+    def update(self, client: Client, id: str) -> Dict:
         version = _Version.read(client=client, id=id)
         version.update(**self._args)
         return version.raw_data
 
     @classmethod
     def delete(cls, client: Client, id: str):
         raise NonDeletableResourceException()
```

### Comparing `aporia-3.0.0a18/src/aporia/as_code/stack.py` & `aporia-3.0.0a19/src/aporia/as_code/stack.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from collections import OrderedDict
 from dataclasses import dataclass
 from enum import Enum
 import json
 import traceback
+from typing import Dict, List, Optional, Tuple
 
 from aporia.as_code.resources.base import BaseResource, CompareStatus, NonDeletableResourceException
 from aporia.as_code.resources.custom_metrics import CustomMetric
 from aporia.as_code.resources.data_source import DataSource
 from aporia.as_code.resources.dataset import Dataset
 from aporia.as_code.resources.model import Model
 from aporia.as_code.resources.monitor import Monitor
@@ -31,15 +32,15 @@
 
 
 @dataclass
 class Resource:
     resource: BaseResource
     depth: int
     status: ResourceStatus
-    id: str | None = None
+    id: Optional[str] = None
 
 
 RESOURCE_TYPE_TO_RESOURCE_CLASS = {
     CustomMetric.__name__: CustomMetric,
     DataSource.__name__: DataSource,
     Dataset.__name__: Dataset,
     Model.__name__: Model,
@@ -112,15 +113,15 @@
             print("Removed resources:")
         for unique_id in self._delete_resources.keys():
             resource_parts = unique_id.split("/")
             depth = len(resource_parts) - 1
             name = resource_parts[-1]
             print(f"|-{'----' * depth}{name} - delete")
 
-    def __pop_deleted_sub_resources(self, non_deleteable_resources: list[str], unique_id):
+    def __pop_deleted_sub_resources(self, non_deleteable_resources: List[str], unique_id):
         resource_entry = self._resources[unique_id]
         if hasattr(resource_entry.resource, "sub_resources"):
             for resource, _ in resource_entry.resource.sub_resources:
                 sub_resource_unique_id = f"{unique_id}/{resource.name}"
                 if sub_resource_unique_id in non_deleteable_resources:
                     self.__pop_deleted_sub_resources(
                         non_deleteable_resources=non_deleteable_resources,
@@ -128,15 +129,15 @@
                     )
                     self._output.pop(sub_resource_unique_id)
                 elif sub_resource_unique_id in self._output.keys():
                     raise RuntimeError(
                         f"Resource deletion missed for {sub_resource_unique_id}. Stack potentially corrupted."
                     )
 
-    def _create(self) -> tuple[dict, Exception | None]:
+    def _create(self) -> Tuple[Dict, Optional[Exception]]:
         output = self._output or {}
         error = None
         try:
             # Create/update resources
             for (
                 unique_id,
                 resource_entry,
@@ -240,15 +241,15 @@
     def apply(
         self,
         action: StackAction = StackAction.CREATE,
         skip_preview: bool = False,
         yes: bool = False,
         rollback=True,
         yes_rollback=False,
-        config_path: str | None = None,
+        config_path: Optional[str] = None,
     ):
         action = StackAction(action)
         # TODO: Read config_path, and apply diffs. Then write to config_path
         if config_path is not None:
             try:
                 with open(config_path, "r") as f:
                     self._output = json.loads(f.read())
```

### Comparing `aporia-3.0.0a18/src/aporia/sdk/aporia_api.py` & `aporia-3.0.0a19/src/aporia/sdk/aporia_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any
+from typing import Any, Dict, List, Optional, Union
 
 from aporia.sdk.base import BaseAporiaResource
 from aporia.sdk.client import Client
 from aporia.sdk.data_sources import DataSource, DataSourceType
 from aporia.sdk.metrics import AporiaMetrics, MetricParameters
 from aporia.sdk.models import Model, ModelColor, ModelIcon, ModelType, NoOwner
 
@@ -23,50 +23,50 @@
         self.client = Client(
             base_url=f"{base_url}/api/v1/{account_name}/{workspace_name}", token=token, debug=debug
         )
         self.metrics_client = AporiaMetrics(
             token=token, account_name=account_name, workspace_name=workspace_name, base_url=base_url
         )
         self.delete_on_failure = delete_on_failure
-        self._created_resources: list[BaseAporiaResource] = []
+        self._created_resources: List[BaseAporiaResource] = []
 
     def create_model(
         self,
         name: str,
         model_type: ModelType,
-        description: str | None = None,
-        icon: ModelIcon | None = None,
-        color: ModelColor | None = None,
-        owner: str | None | NoOwner = NoOwner,
+        description: Optional[str] = None,
+        icon: Optional[ModelIcon] = None,
+        color: Optional[ModelColor] = None,
+        owner: Optional[Union[str, NoOwner]] = NoOwner,
     ) -> Model:
         model = Model.create(
             client=self.client,
             name=name,
             model_type=model_type,
             description=description,
             icon=icon,
             color=color,
             owner=owner,
         )
         self._created_resources.append(model)
         return model
 
     def create_data_source(
-        self, name: str, data_source_type: DataSourceType, connection_data: dict[str, Any]
+        self, name: str, data_source_type: DataSourceType, connection_data: Dict[str, Any]
     ) -> DataSource:
         data_source = DataSource.create(
             client=self.client,
             name=name,
             data_source_type=data_source_type,
             connection_data=connection_data,
         )
         self._created_resources.append(data_source)
         return data_source
 
-    def query_metrics(self, model_id: str, metrics: list[MetricParameters]) -> list:
+    def query_metrics(self, model_id: str, metrics: List[MetricParameters]) -> List:
         return self.metrics_client.query_batch(model_id=model_id, metrics=metrics)
 
     def delete(self):
         for resource in self._created_resources:
             resource.delete()
 
     def __enter__(self):
```

### Comparing `aporia-3.0.0a18/src/aporia/sdk/base.py` & `aporia-3.0.0a19/src/aporia/sdk/base.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from abc import ABC, abstractclassmethod, abstractmethod, abstractstaticmethod
+from typing import List
 
 from aporia.sdk.client import Client
 
 
 class BaseAporiaResource(ABC):
     @abstractclassmethod
     def create(cls, client: Client, name: str, *args, **kwargs) -> "BaseAporiaResource":
@@ -17,13 +18,13 @@
         ...
 
     @abstractmethod
     def delete(self):
         ...
 
     @abstractclassmethod
-    def get_all(cls, client: Client, **kwargs) -> list["BaseAporiaResource"]:
+    def get_all(cls, client: Client, **kwargs) -> List["BaseAporiaResource"]:
         ...
 
     @abstractstaticmethod
     def delete_by_id(cls, client: Client, id: str):
         ...
```

### Comparing `aporia-3.0.0a18/src/aporia/sdk/client.py` & `aporia-3.0.0a19/src/aporia/sdk/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,25 @@
+from typing import Dict, Optional, Tuple
+
 import requests
 
 
 class Client:
     def __init__(self, base_url: str, token: str, debug: bool = False):
         self.base_url = base_url
         self.token = token
         self.debug = debug
 
     def send_request(
         self,
         url: str,
         method: str,
-        data: dict | None = None,
-        url_override: str | None = None,
-        url_search_replace: tuple[str, str] | None = None,
+        data: Optional[Dict] = None,
+        url_override: Optional[str] = None,
+        url_search_replace: Optional[Tuple[str, str]] = None,
     ):
         if url_override is not None:
             target_url = url_override
         else:
             target_url = self.base_url + url
 
         if url_search_replace is not None:
```

### Comparing `aporia-3.0.0a18/src/aporia/sdk/custom_metrics.py` & `aporia-3.0.0a19/src/aporia/sdk/custom_metrics.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,24 @@
+from typing import Dict, List, Optional
+
 from aporia.sdk.base import BaseAporiaResource
 from aporia.sdk.client import Client
 
 
 class CustomMetric(BaseAporiaResource):
-    def __init__(self, client: Client, data: dict):
+    def __init__(self, client: Client, data: Dict):
         self.client = client
         self.__update_members(data)
 
-    def __update_members(self, data: dict):
+    def __update_members(self, data: Dict):
         self.id = data["id"]
         self.raw_data = data
 
     @classmethod
-    def get_all(cls, client: Client, model_id: str | None = None) -> list["CustomMetric"]:
+    def get_all(cls, client: Client, model_id: Optional[str] = None) -> List["CustomMetric"]:
         response = client.send_request(
             f"/custom-metrics{'' if model_id is None else f'?model_id={model_id}'}", "GET"
         )
 
         client.assert_response(response)
 
         return [cls(client=client, data=entry) for entry in response.json()]
```

### Comparing `aporia-3.0.0a18/src/aporia/sdk/dashboards.py` & `aporia-3.0.0a19/src/aporia/sdk/dashboards.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from enum import Enum
-from typing import Any
+from typing import Any, Dict, Type
 
 from pydantic import BaseModel, validator
 
 
 class WidgetType(Enum):
     METRIC = "metric"
     TIMESERIES = "timeseries"
@@ -32,15 +32,15 @@
     pass
 
 
 class TextWidgetData(BaseWidgetData):
     text: str
 
 
-WIDGET_TYPE_TO_WIDGET_DATA_CLASS: dict[WidgetType, type[BaseWidgetData]] = {
+WIDGET_TYPE_TO_WIDGET_DATA_CLASS: Dict[WidgetType, Type[BaseWidgetData]] = {
     WidgetType.METRIC: MetricWidgetData,
     WidgetType.TIMESERIES: TimeseriesWidgetData,
     WidgetType.DISTRIBUTION: DistributionWidgetData,
     WidgetType.TABLE: TableWidgetData,
     WidgetType.TEXT: TextWidgetData,
 }
 
@@ -49,15 +49,15 @@
     loc_x: int
     loc_y: int
     type: WidgetType
     data: BaseWidgetData
 
     @validator("data", pre=True)
     @classmethod
-    def _parse_data(cls, value: Any, values: dict[str, Any]) -> BaseWidgetData:
+    def _parse_data(cls, value: Any, values: Dict[str, Any]) -> BaseWidgetData:
         """Validates data matches the widget type.
 
         Args:
             value: data dict to validate
             values: other attributes of Widget (type)
 
         Returns:
```

### Comparing `aporia-3.0.0a18/src/aporia/sdk/data_sources.py` & `aporia-3.0.0a19/src/aporia/sdk/data_sources.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from enum import Enum
-from typing import Any
+from typing import Any, Dict, List
 
 from aporia.sdk.base import BaseAporiaResource
 from aporia.sdk.client import Client
 
 
 class DataSourceType(Enum):
     S3 = "s3"
@@ -15,39 +15,39 @@
     REDSHIFT = "redshift"
     DATABRICKS = "databricks"
     AZURE_BLOB_STORAGE = "azure_blob_storage"
     SNOWFLAKE_NATIVE = "snowflake_native"
 
 
 class DataSource(BaseAporiaResource):
-    def __init__(self, client: Client, data: dict):
+    def __init__(self, client: Client, data: Dict):
         self.client = client
         self.__update_members(data)
 
-    def __update_members(self, data: dict):
+    def __update_members(self, data: Dict):
         self.raw_data = data
         self.id = data["id"]
         self.name = data["name"]
         self.type = DataSourceType(data["type"])
 
     @classmethod
-    def get_all(cls, client: Client) -> list["DataSource"]:
+    def get_all(cls, client: Client) -> List["DataSource"]:
         response = client.send_request("/data-sources", "GET")
 
         client.assert_response(response)
 
         return [cls(client=client, data=entry) for entry in response.json()]
 
     @classmethod
     def create(
         cls,
         client: Client,
         name: str,
         data_source_type: DataSourceType,
-        connection_data: dict[str, Any],
+        connection_data: Dict[str, Any],
     ) -> "DataSource":
         existing_data_sources = cls.get_all(client=client)
 
         for data_source in existing_data_sources:
             if data_source.name == name:
                 if data_source.type is data_source_type:
                     raise RuntimeError(
```

### Comparing `aporia-3.0.0a18/src/aporia/sdk/datasets.py` & `aporia-3.0.0a19/src/aporia/sdk/datasets.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from enum import Enum
-from typing import Any
+from typing import Any, Dict, List, Optional
 
 from pydantic import BaseModel
 
 from aporia.sdk.base import BaseAporiaResource
 from aporia.sdk.client import Client
 from aporia.sdk.data_sources import DataSource
 
@@ -22,55 +22,55 @@
     ARRAY = "array"
     EMBEDDING = "embedding"
 
 
 class FieldSchema(BaseModel):
     name: str
     type: FieldType
-    properties: dict[str, Any] | None = None
+    properties: Optional[Dict[str, Any]] = None
 
 
 class DatasetSchema(BaseModel):
     # Null id and timestamp allowed for training
-    id_column: str | None
-    timestamp_column: str | None
-    raw_inputs: list[FieldSchema]
-    features: list[FieldSchema]
-    predictions: list[FieldSchema]
-    actuals: list[FieldSchema]
+    id_column: Optional[str]
+    timestamp_column: Optional[str]
+    raw_inputs: List[FieldSchema]
+    features: List[FieldSchema]
+    predictions: List[FieldSchema]
+    actuals: List[FieldSchema]
 
 
 class Dataset(BaseAporiaResource):
-    def __init__(self, client: Client, data: dict):
+    def __init__(self, client: Client, data: Dict):
         self.client = client
         self.__update_members(data)
 
-    def __update_members(self, data: dict):
+    def __update_members(self, data: Dict):
         self.raw_data = data
         self.id = data["id"]
 
     @classmethod
-    def get_all(cls, client: Client) -> list["Dataset"]:
+    def get_all(cls, client: Client) -> List["Dataset"]:
         response = client.send_request("/datasets", "GET")
 
         client.assert_response(response)
 
         return [cls(client=client, data=entry) for entry in response.json()]
 
     @classmethod
     def create(
         cls,
         client: Client,
         model_id: str,
         version_id: str,
         dataset_type: DatasetType,
-        connection_data: dict[str, Any],
+        connection_data: Dict[str, Any],
         schema: DatasetSchema,
-        data_source: DataSource | None = None,
-        data_source_id: str | None = None,
+        data_source: Optional[DataSource] = None,
+        data_source_id: Optional[str] = None,
     ) -> "Dataset":
         dataset_type = DatasetType(dataset_type)
 
         response = client.send_request(
             "/datasets",
             "POST",
             {
@@ -115,18 +115,18 @@
         response = client.send_request(f"/datasets/{id}", "GET")
         client.assert_response(response)
         return cls(client=client, data=response.json())
 
     def update(
         self,
         # dataset_type: DatasetType | None = None,
-        connection_data: dict[str, Any] | None = None,
-        schema: DatasetSchema | None = None,
-        data_source: DataSource | None = None,
-        data_source_id: str | None = None,
+        connection_data: Optional[Dict[str, Any]] = None,
+        schema: Optional[DatasetSchema] = None,
+        data_source: Optional[DataSource] = None,
+        data_source_id: Optional[str] = None,
         **kwargs,
     ):
         # dataset_type = DatasetType(dataset_type)
 
         args = {}
         # if dataset_type is not None:
         #     args["stage"] = dataset_type.value
```

### Comparing `aporia-3.0.0a18/src/aporia/sdk/metrics.py` & `aporia-3.0.0a19/src/aporia/sdk/metrics.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-from dataclasses import dataclass
 import datetime
-from enum import Enum
-from typing import Any
+from typing import Any, Dict, List, Optional, Union
 
 from pydantic import BaseModel
 
 from aporia.sdk.client import Client
 from aporia.sdk.datasets import DatasetType
 
 
@@ -20,55 +18,55 @@
         }
 
 
 class MetricSegment(BaseModel):
     id: str
     value: str  # TODO: Test with numeric auto segments
 
-    def serialize(self) -> dict:
+    def serialize(self) -> Dict:
         return {"id": self.id, "value": self.value}
 
 
 class MetricDataset(BaseModel):
     dataset_type: DatasetType = DatasetType.SERVING
-    time_range: TimeRange | None = None
-    model_version: str | None = None
-    segment: MetricSegment | None = None
+    time_range: Optional[TimeRange] = None
+    model_version: Optional[str] = None
+    segment: Optional[MetricSegment] = None
 
-    def serialize(self) -> dict:
+    def serialize(self) -> Dict:
         return {
             "dataset_type": self.dataset_type.value,
             "time_range": self.time_range.serialize() if self.time_range is not None else None,
             "model_version": self.model_version,
             "segment": self.segment.serialize() if self.segment is not None else None,
         }
 
 
 class MetricResponse(BaseModel):
     id: str
     value: Any
-    error: dict | list | str | None
-    segment: MetricSegment | None
+    error: Optional[Union[Dict, List, str]]
+    segment: Optional[MetricSegment]
 
 
 class QueryResponse(BaseModel):
-    metrics: list[MetricResponse]
+    metrics: List[MetricResponse]
     time_range: TimeRange
 
 
 class MetricParameters(BaseModel):
     dataset: MetricDataset
     # Metric identifier
     name: str
     # Parameters
-    column: str | None = None
-    k: int | None = None
-    threshold: float | None = None
-    custom_metric_id: str | None = None
-    baseline: MetricDataset | None = None
+    column: Optional[str] = None
+    k: Optional[int] = None
+    threshold: Optional[float] = None
+    custom_metric_id: Optional[str] = None
+    baseline: Optional[MetricDataset] = None
 
 
 class MetricError(Exception):
     def __init__(self, error, parameters: MetricParameters):
         super().__init__(error)
         self.parameters = parameters
 
@@ -76,32 +74,32 @@
 class AporiaMetrics:
     def __init__(
         self,
         token: str,
         account_name: str,
         base_url: str = "https://platform.aporia.com",
         workspace_name: str = "default-workspace",
-    ) -> dict:
+    ) -> Dict:
         self.client = Client(
             base_url=f"{base_url}/api/v1/{account_name}/{workspace_name}", token=token
         )
 
     def query(
         self,
         # Dataset identifiers
         model_id: str,
         dataset: MetricDataset,
         # Metric identifier
         metric_name: str,
-        baseline: MetricDataset | None = None,
+        baseline: Optional[MetricDataset] = None,
         # Parameters
-        column: str | None = None,
-        k: int | None = None,
-        threshold: float | None = None,
-        custom_metric_id: str | None = None,
+        column: Optional[str] = None,
+        k: Optional[int] = None,
+        threshold: Optional[float] = None,
+        custom_metric_id: Optional[str] = None,
     ):
         metric_parameters = {}
         if column is not None:
             metric_parameters["column"] = column
         if k is not None:
             metric_parameters["k"] = k
         if threshold is not None:
@@ -133,15 +131,15 @@
 
         result = [QueryResponse(**entry) for entry in response.json()]
 
         if result[0].metrics[0].error is not None:
             raise Exception(f"Error occured: {result[0].metrics[0].error}")
         return result[0].metrics[0].value
 
-    def query_batch(self, model_id: str, metrics: list[MetricParameters]):
+    def query_batch(self, model_id: str, metrics: List[MetricParameters]) -> List:
         metric_requests = []
         for i, metric in enumerate(metrics):
             metric_parameters = {}
             if metric.column is not None:
                 metric_parameters["column"] = metric.column
             if metric.k is not None:
                 metric_parameters["k"] = metric.k
```

### Comparing `aporia-3.0.0a18/src/aporia/sdk/models.py` & `aporia-3.0.0a19/src/aporia/sdk/models.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from enum import Enum
+from typing import Dict, List, Optional, Union
 
 from aporia.sdk.base import BaseAporiaResource
 from aporia.sdk.client import Client
 from aporia.sdk.custom_metrics import CustomMetric
 from aporia.sdk.dashboards import Widget
 from aporia.sdk.monitors import Monitor, MonitorConfiguration, MonitorType
 from aporia.sdk.segments import Segment
@@ -44,46 +45,46 @@
 
 
 class NoOwner:
     pass
 
 
 class Model(BaseAporiaResource):
-    def __init__(self, client: Client, data: dict):
+    def __init__(self, client: Client, data: Dict):
         self.client = client
         self.__update_members(data)
 
-    def __update_members(self, data: dict):
+    def __update_members(self, data: Dict):
         self.raw_data = data
         self.id = data["id"]
         self.name = data["name"]
         self.type = ModelType(data["type"])
         self.description = data["description"]
         self.color = ModelColor(data["color"])
         self.icon = ModelIcon(data["icon"])
         self.owner = data["owner"]
 
     @classmethod
-    def get_all(cls, client: Client) -> list["Model"]:
+    def get_all(cls, client: Client) -> List["Model"]:
         response = client.send_request("/models", "GET")
 
         client.assert_response(response)
 
         return [cls(client=client, data=entry) for entry in response.json()]
 
     @classmethod
     def create(
         cls,
         client: Client,
         name: str,
         model_type: ModelType,
-        description: str | None = None,
-        icon: ModelIcon | None = None,
-        color: ModelColor | None = None,
-        owner: str | None | NoOwner = NoOwner(),
+        description: Optional[str] = None,
+        icon: Optional[ModelIcon] = None,
+        color: Optional[ModelColor] = None,
+        owner: Optional[Union[str, NoOwner]] = NoOwner(),
     ) -> "Model":
         """Creates a new model in Aporia, and returns a new model descriptor."""
         model_type = ModelType(model_type)
 
         creation_parameters = {"name": name, "type": model_type.value}
 
         if description is not None:
@@ -139,17 +140,17 @@
     def create_custom_metric(self, name: str, code: str) -> CustomMetric:
         metric = CustomMetric.create(client=self.client, name=name, model_id=self.id, code=code)
         return metric
 
     def create_segment(
         self,
         name: str,
-        field_name: str | None = None,
-        values: list[str] | list[float | int] | None = None,
-        term: str | None = None,
+        field_name: Optional[str] = None,
+        values: Optional[Union[List[str], List[Union[float, int]]]] = None,
+        term: Optional[str] = None,
     ) -> Segment:
         segment = Segment.create(
             client=self.client,
             name=name,
             model_id=self.id,
             field_name=field_name,
             values=values,
@@ -158,17 +159,17 @@
         return segment
 
     def create_monitor(
         self,
         name: str,
         monitor_type: MonitorType,
         configuration: MonitorConfiguration,
-        scheduling: str | None = None,
-        comment: str | None = None,
-        creator: str | None = None,
+        scheduling: Optional[str] = None,
+        comment: Optional[str] = None,
+        creator: Optional[str] = None,
         is_active: bool = True,
     ) -> Monitor:
         monitor = Monitor.create(
             client=self.client,
             model_id=self.id,
             name=name,
             monitor_type=monitor_type,
@@ -176,9 +177,9 @@
             configuration=configuration,
             comment=comment,
             creator=creator,
             is_active=is_active,
         )
         return monitor
 
-    def create_dashboard(self, widgets: list[Widget]):
+    def create_dashboard(self, widgets: List[Widget]):
         pass
```

### Comparing `aporia-3.0.0a18/src/aporia/sdk/monitors.py` & `aporia-3.0.0a19/src/aporia/sdk/monitors.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from enum import Enum
+from typing import Dict, List, Optional, Union
 
 from pydantic import BaseModel, root_validator, validator
 
 from aporia.sdk.base import BaseAporiaResource
 from aporia.sdk.client import Client
 
 SEGMENT_ID_ALL_DATA = "ALLDATA"
@@ -48,17 +49,17 @@
     def to_string(self) -> str:
         return f"{self.count}{self.type.value}"
 
 
 # TODO: Rename stuff to match Python conventions
 class FocalConfiguration(BaseModel):
     source: SourceType = SourceType.SERVING
-    timePeriod: TimePeriod | None = None  # Missing for staleness
-    skipPeriod: TimePeriod | None = None
-    alignBinsWithBaseline: bool | None = None  # Needed (as True) for drift/histogram
+    timePeriod: Optional[TimePeriod] = None  # Missing for staleness
+    skipPeriod: Optional[TimePeriod] = None
+    alignBinsWithBaseline: Optional[bool] = None  # Needed (as True) for drift/histogram
 
     @validator("source")
     def _validate_source(cls, value):
         if value is not SourceType.SERVING:
             raise ValueError("For focal, source must always be serving")
         return value
 
@@ -81,18 +82,18 @@
 
         return result
 
 
 class BaselineConfiguration(BaseModel):
     source: SourceType
     timePeriod: TimePeriod  # Actual time to compare to
-    skipPeriod: TimePeriod | None = None  # By default, equal to Focal. Doesn't exist on training
-    aggregationPeriod: TimePeriod | None = None  # Does't exist on drift/histogram
-    segmentValue: str | int | float | None = None
-    segmentGroupId: str | None = None
+    skipPeriod: Optional[TimePeriod] = None  # By default, equal to Focal. Doesn't exist on training
+    aggregationPeriod: Optional[TimePeriod] = None  # Does't exist on drift/histogram
+    segmentValue: Optional[Union[str, int, float]] = None
+    segmentGroupId: Optional[str] = None
 
     @validator("skipPeriod", always=True)
     def _validate_skip_period(cls, value, values):
         if values["source"] is SourceType.TRAINING:
             if value is not None:
                 raise ValueError("For training baseline, skipPeriod must not appear")
         # TODO: This is basically defaulted in the global monitor validator
@@ -129,18 +130,18 @@
     ACCURACY = "accuracy"
     MEAN = "mean"
 
 
 class MetricConfiguration(BaseModel):
     type: MetricType
     # Necessary for custom metrics
-    id: str | None = None
+    id: Optional[str] = None
     # Necessary for general metrics
-    metricAtK: int | None = None  # TODO: Almost always 3 -.- Gubkin
-    threshold: float | None = None
+    metricAtK: Optional[int] = None  # TODO: Almost always 3 -.- Gubkin
+    threshold: Optional[float] = None
     # TODO: Check if more things exist for other metrics
     # TODO: Maybe add class for Aporia metrics
 
     @validator("id", always=True)
     def _validate_id(cls, value, values):
         if values["type"] is MetricType.CUSTOM_METRIC:
             if value is None:
@@ -167,16 +168,16 @@
     RANGE = "RANGE"
     TIME_SERIES_ANOMALY = "TIME_SERIES_ANOMALY"
     APORIA_DRIFT_SCORE = "APORIA_DRIFT_SCORE"
     MODEL_STALENESS = "MODEL_STALENESS"
 
 
 class ThresholdConfiguration(BaseModel):
-    numeric: float | None = None
-    categorical: float | None = None
+    numeric: Optional[float] = None
+    categorical: Optional[float] = None
 
     def to_dict(self):
         result = {}
 
         if self.numeric is not None:
             result["numeric"] = self.numeric
         if self.categorical is not None:
@@ -184,21 +185,21 @@
 
         return result
 
 
 class LogicEvaluationConfiguration(BaseModel):
     name: LogicEvaluationType
     # Needed for range (Both must exist, if one isn't used, it should be null)
-    min: float | None = None
+    min: Optional[float] = None
     # Also needed for ratio (float) and staleness (TimePeriod)
-    max: float | TimePeriod | None = None
+    max: Optional[Union[float, TimePeriod]] = None
     # Needed for timeseries anomaly
-    sensitivity: float | None = None
+    sensitivity: Optional[float] = None
     # Needed for Aporia drift score
-    thresholds: ThresholdConfiguration | None = None
+    thresholds: Optional[ThresholdConfiguration] = None
 
     @root_validator()
     def _validate_logic_evaluation(cls, values):
         if values["name"] is LogicEvaluationType.RANGE:
             if isinstance(values["max"], TimePeriod):
                 raise ValueError("max must be a float or None for Range logic evaluation")
             if values["sensitivity"] is not None or values["thresholds"] is not None:
@@ -263,17 +264,17 @@
     MIN_BASELINE_DATA_POINTS = "MIN_BASELINE_DATA_POINTS"
     FOCAL_DATA_VALUE_IN_RANGE = "FOCAL_DATA_VALUE_IN_RANGE"
 
 
 class PreConditionConfiguration(BaseModel):
     name: PreConditionType
     # Needed for MIN_BASELINE_DATA_POINTS
-    value: int | None = None
+    value: Optional[int] = None
     # Needed for FOCAL_DATA_VALUE_IN_RANGE
-    min: float | None = None
+    min: Optional[float] = None
 
     @root_validator()
     def _validate_pre_condition(cls, values):
         if values["name"] is PreConditionType.MIN_BASELINE_DATA_POINTS:
             if values["value"] is None:
                 raise ValueError("value must appear for MIN_BASELINE_DATA_POINTS PreCondition")
             if values["min"] is not None:
@@ -332,18 +333,18 @@
 
 
 class ActionConfiguration(BaseModel):
     type: ActionType
     severity: Severity
     alertType: AlertType
     description: str  # TODO: Enumize
-    notification: list  # TODO: Look deeper into that
+    notification: List  # TODO: Look deeper into that
     action_schema: str = "v1"  # TODO: Realize what to do with it
-    maxAlertsPerDay: int | None = None
-    visualization: VisualizationType | None = None
+    maxAlertsPerDay: Optional[int] = None
+    visualization: Optional[VisualizationType] = None
 
     def to_dict(self):
         result = {
             "type": self.type.value,
             "severity": self.severity.value,
             "alertType": self.alertType.value,
             "description": self.description,
@@ -357,34 +358,36 @@
             result["visualization"] = self.visualization.value
 
         return result
 
 
 class ModelIdentification(BaseModel):
     id: str
-    version: str | None = None  # None indicates all versions # TODO: Saw one saying "all_versions" as well?? Validate that
+    version: Optional[
+        str
+    ] = None  # None indicates all versions # TODO: Saw one saying "all_versions" as well?? Validate that
 
     def to_dict(self):
         return self.dict()
 
 
 class SegmentIdentification(BaseModel):
-    group: str | None = None
-    value: str | int | float | None = None  # None indicates all segment values
+    group: Optional[str] = None
+    value: Optional[Union[str, int, float]] = None  # None indicates all segment values
 
     def to_dict(self):
         return self.dict()
 
 
 class Identification(BaseModel):
     models: ModelIdentification
     segment: SegmentIdentification
     # TODO: Check for raw inputs and actuals
-    features: list[str] | None = None
-    predictions: list[str] | None = None
+    features: Optional[List[str]] = None
+    predictions: Optional[List[str]] = None
 
     def to_dict(self):
         result = {
             "models": self.models.to_dict(),
             "segment": self.segment.to_dict(),
         }
         if self.features is not None:
@@ -395,18 +398,18 @@
         return result
 
 
 class MonitorConfiguration(BaseModel):
     identification: Identification
     focal: FocalConfiguration
     metric: MetricConfiguration
-    actions: list[ActionConfiguration]
-    baseline: BaselineConfiguration | None = None
-    logicEvaluations: list[LogicEvaluationConfiguration] | None = None
-    preConditions: list[PreConditionConfiguration] | None = None
+    actions: List[ActionConfiguration]
+    baseline: Optional[BaselineConfiguration] = None
+    logicEvaluations: Optional[List[LogicEvaluationConfiguration]] = None
+    preConditions: Optional[List[PreConditionConfiguration]] = None
     # TODO: Add cross-configuration validators
 
     @root_validator()
     def _validate_monitor_configuration(cls, values):
         if values["baseline"] is not None:
             # For non-training monitors, skipPeriod defaults to the focal timePeriod, unless it's per segment
             if values["baseline"].source is SourceType.SERVING:
@@ -441,27 +444,27 @@
                 precondition.to_dict() for precondition in self.preConditions
             ]
 
         return result
 
 
 class Monitor(BaseAporiaResource):
-    def __init__(self, client: Client, data: dict):
+    def __init__(self, client: Client, data: Dict):
         self.client = client
         self.__update_members(data)
 
-    def __update_members(self, data: dict):
+    def __update_members(self, data: Dict):
         self.raw_data = data
         self.id = data["id"]
         self.name = data["name"]
         # TODO: Enum-ize
         self.type = data["type"]
 
     @classmethod
-    def get_all(cls, client: Client) -> list["Monitor"]:
+    def get_all(cls, client: Client) -> List["Monitor"]:
         response = client.send_request("/monitors", "GET")
 
         client.assert_response(response)
 
         return [cls(client=client, data=entry) for entry in response.json()]
 
     @classmethod
@@ -469,16 +472,16 @@
         cls,
         client: Client,
         model_id: str,
         name: str,
         monitor_type: MonitorType,
         scheduling: str,  # TODO: Optionally infer from configuration
         configuration: MonitorConfiguration,
-        comment: str | None = None,
-        creator: str | None = None,
+        comment: Optional[str] = None,
+        creator: Optional[str] = None,
         is_active: bool = True,
     ) -> "Monitor":
         monitor_type = MonitorType(monitor_type)
 
         # TODO: Justify these values
         if scheduling is None:
             if configuration.focal.timePeriod is None:
```

### Comparing `aporia-3.0.0a18/src/aporia/sdk/segments.py` & `aporia-3.0.0a19/src/aporia/sdk/segments.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,43 +1,45 @@
+from typing import Dict, List, Optional, Union
+
 from aporia.sdk.base import BaseAporiaResource
 from aporia.sdk.client import Client
 
 
 class Segment(BaseAporiaResource):
-    def __init__(self, client: Client, data: dict):
+    def __init__(self, client: Client, data: Dict):
         self.client = client
         self.__update_members(data)
 
-    def __update_members(self, data: dict):
+    def __update_members(self, data: Dict):
         self.raw_data = data
         self.id = data["id"]
         self.name = data["name"]
         self.field = data["field"]
         self.values = data["values"]
         self.term = data["term"]
 
     @classmethod
-    def get_all(cls, client: Client, model_id: str | None = None) -> list["Segment"]:
+    def get_all(cls, client: Client, model_id: Optional[str] = None) -> List["Segment"]:
         response = client.send_request(
             f"/data-segments{'' if model_id is None else f'?model_id={model_id}'}", "GET"
         )
 
         client.assert_response(response)
 
         return [cls(client=client, data=entry) for entry in response.json()]
 
     @classmethod
     def create(
         cls,
         client: Client,
         name: str,
         model_id: str,
-        field_name: str | None = None,
-        values: list[str] | list[float | int] | None = None,
-        term: str | None = None,
+        field_name: Optional[str] = None,
+        values: Optional[Union[List[str], List[Union[float, int]]]] = None,
+        term: Optional[str] = None,
     ) -> "Segment":
         segment_data = {}
         if term is not None:
             segment_data["term"] = term
         else:
             segment_data["field_name"] = field_name
             segment_data["values"] = values
@@ -55,18 +57,18 @@
     def read(cls, client: Client, id: str) -> "Segment":
         response = client.send_request(f"/data-segments/{id}", "GET")
         client.assert_response(response)
         return cls(client=client, data=response.json())
 
     def update(
         self,
-        name: str | None = None,
-        field_name: str | None = None,
-        values: list[str] | list[float | int] | None = None,
-        term: str | None = None,
+        name: Optional[str] = None,
+        field_name: Optional[str] = None,
+        values: Optional[Union[List[str], List[Union[float, int]]]] = None,
+        term: Optional[str] = None,
         **kwargs,
     ):
         args = {}
         if name is not None:
             args["name"] = name
         if field_name is not None:
             args["field_name"] = field_name
```

### Comparing `aporia-3.0.0a18/src/aporia/sdk/versions.py` & `aporia-3.0.0a19/src/aporia/sdk/versions.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-from typing import Any
+from typing import Any, Dict, List, Optional
 
 from aporia.sdk.base import BaseAporiaResource
 from aporia.sdk.client import Client
 from aporia.sdk.data_sources import DataSource
 from aporia.sdk.datasets import Dataset, DatasetSchema, DatasetType
 
 
 class Version(BaseAporiaResource):
-    def __init__(self, client: Client, data: dict):
+    def __init__(self, client: Client, data: Dict):
         self.client = client
         self.__update_members(data)
 
-    def __update_members(self, data: dict):
+    def __update_members(self, data: Dict):
         self.raw_data = data
         self.id = data["id"]
         self.name = data["name"]
         self.model_id = data["model_id"]
 
     @classmethod
-    def get_all(cls, client: Client, model_id: str | None = None) -> list["Version"]:
+    def get_all(cls, client: Client, model_id: Optional[str] = None) -> List["Version"]:
         response = client.send_request(
             f"/model-versions{'' if model_id is None else f'?model_id={model_id}'}", "GET"
         )
 
         client.assert_response(response)
 
         return [cls(client=client, data=entry) for entry in response.json()]
@@ -47,15 +47,15 @@
         return cls(client=client, data=response.json())
 
     def create_dataset(
         self,
         name: str,
         dataset_type: DatasetType,
         data_source: DataSource,
-        connection_data: dict[str, Any],
+        connection_data: Dict[str, Any],
         schema: DatasetSchema,
     ) -> Dataset:
         """Creates a new dataset."""
         dataset = Dataset.create(
             client=self.client,
             name=name,
             model_id=self.model_id,
```

### Comparing `aporia-3.0.0a18/PKG-INFO` & `aporia-3.0.0a19/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: aporia
-Version: 3.0.0a18
+Version: 3.0.0a19
 Summary: 
 Author: Aporia
 Author-email: support@aporia.com
-Requires-Python: >=3.10,<=3.11
+Requires-Python: >=3.8,<=3.11
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pydantic (>=1.10,<2.0)
 Requires-Dist: requests (>=2.28,<3.0)
 Description-Content-Type: text/markdown
 
 # Aporia Python SDK
```

