# Comparing `tmp/aporia-3.1.0.tar.gz` & `tmp/aporia-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aporia-3.1.0.tar", max compression
+gzip compressed data, was "aporia-3.2.0.tar", max compression
```

## Comparing `aporia-3.1.0.tar` & `aporia-3.2.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     2968 2023-07-02 17:07:50.080201 aporia-3.1.0/README.md
--rw-r--r--   0        0        0      829 2023-07-02 17:07:50.084201 aporia-3.1.0/pyproject.toml
--rw-r--r--   0        0        0      168 2023-07-02 17:07:50.084201 aporia-3.1.0/src/aporia/__init__.py
--rw-r--r--   0        0        0      925 2023-07-02 17:07:50.084201 aporia-3.1.0/src/aporia/as_code/__init__.py
--rw-r--r--   0        0        0      939 2023-07-02 17:07:50.084201 aporia-3.1.0/src/aporia/as_code/resources/base.py
--rw-r--r--   0        0        0     1465 2023-07-02 17:07:50.084201 aporia-3.1.0/src/aporia/as_code/resources/custom_metrics.py
--rw-r--r--   0        0        0     1984 2023-07-02 17:07:50.084201 aporia-3.1.0/src/aporia/as_code/resources/data_source.py
--rw-r--r--   0        0        0     7206 2023-07-02 17:07:50.084201 aporia-3.1.0/src/aporia/as_code/resources/dataset.py
--rw-r--r--   0        0        0     3854 2023-07-02 17:07:50.084201 aporia-3.1.0/src/aporia/as_code/resources/model.py
--rw-r--r--   0        0        0    11048 2023-07-02 17:07:50.084201 aporia-3.1.0/src/aporia/as_code/resources/monitor.py
--rw-r--r--   0        0        0     2831 2023-07-02 17:07:50.084201 aporia-3.1.0/src/aporia/as_code/resources/segment.py
--rw-r--r--   0        0        0     1946 2023-07-02 17:07:50.084201 aporia-3.1.0/src/aporia/as_code/resources/version.py
--rw-r--r--   0        0        0    34719 2023-07-02 17:07:50.084201 aporia-3.1.0/src/aporia/as_code/stack.py
--rw-r--r--   0        0        0        0 2023-07-02 17:07:50.084201 aporia-3.1.0/src/aporia/sdk/__init__.py
--rw-r--r--   0        0        0     3233 2023-07-02 17:07:50.084201 aporia-3.1.0/src/aporia/sdk/aporia_api.py
--rw-r--r--   0        0        0      723 2023-07-02 17:07:50.084201 aporia-3.1.0/src/aporia/sdk/base.py
--rw-r--r--   0        0        0     1531 2023-07-02 17:07:50.084201 aporia-3.1.0/src/aporia/sdk/client.py
--rw-r--r--   0        0        0     2148 2023-07-02 17:07:50.084201 aporia-3.1.0/src/aporia/sdk/custom_metrics.py
--rw-r--r--   0        0        0     1822 2023-07-02 17:07:50.084201 aporia-3.1.0/src/aporia/sdk/dashboards.py
--rw-r--r--   0        0        0     3610 2023-07-02 17:07:50.084201 aporia-3.1.0/src/aporia/sdk/data_sources.py
--rw-r--r--   0        0        0     6709 2023-07-02 17:07:50.084201 aporia-3.1.0/src/aporia/sdk/datasets.py
--rw-r--r--   0        0        0     1844 2023-07-02 17:07:50.084201 aporia-3.1.0/src/aporia/sdk/messaging.py
--rw-r--r--   0        0        0     6108 2023-07-02 17:07:50.084201 aporia-3.1.0/src/aporia/sdk/metrics.py
--rw-r--r--   0        0        0     6326 2023-07-02 17:07:50.084201 aporia-3.1.0/src/aporia/sdk/models.py
--rw-r--r--   0        0        0    85066 2023-07-02 17:07:50.084201 aporia-3.1.0/src/aporia/sdk/monitors.py
--rw-r--r--   0        0        0     3506 2023-07-02 17:07:50.084201 aporia-3.1.0/src/aporia/sdk/segments.py
--rw-r--r--   0        0        0     3048 2023-07-02 17:07:50.084201 aporia-3.1.0/src/aporia/sdk/versions.py
--rw-r--r--   0        0        0     3474 1970-01-01 00:00:00.000000 aporia-3.1.0/PKG-INFO
+-rw-r--r--   0        0        0     2968 2023-07-02 19:20:47.418690 aporia-3.2.0/README.md
+-rw-r--r--   0        0        0      829 2023-07-02 19:20:47.418690 aporia-3.2.0/pyproject.toml
+-rw-r--r--   0        0        0      168 2023-07-02 19:20:47.418690 aporia-3.2.0/src/aporia/__init__.py
+-rw-r--r--   0        0        0      925 2023-07-02 19:20:47.418690 aporia-3.2.0/src/aporia/as_code/__init__.py
+-rw-r--r--   0        0        0     1025 2023-07-02 19:20:47.418690 aporia-3.2.0/src/aporia/as_code/resources/base.py
+-rw-r--r--   0        0        0     1706 2023-07-02 19:20:47.418690 aporia-3.2.0/src/aporia/as_code/resources/custom_metrics.py
+-rw-r--r--   0        0        0     2370 2023-07-02 19:20:47.418690 aporia-3.2.0/src/aporia/as_code/resources/data_source.py
+-rw-r--r--   0        0        0     7465 2023-07-02 19:20:47.422690 aporia-3.2.0/src/aporia/as_code/resources/dataset.py
+-rw-r--r--   0        0        0     4660 2023-07-02 19:20:47.422690 aporia-3.2.0/src/aporia/as_code/resources/model.py
+-rw-r--r--   0        0        0    12069 2023-07-02 19:20:47.422690 aporia-3.2.0/src/aporia/as_code/resources/monitor.py
+-rw-r--r--   0        0        0     3052 2023-07-02 19:20:47.422690 aporia-3.2.0/src/aporia/as_code/resources/segment.py
+-rw-r--r--   0        0        0     2187 2023-07-02 19:20:47.422690 aporia-3.2.0/src/aporia/as_code/resources/version.py
+-rw-r--r--   0        0        0    37893 2023-07-02 19:20:47.422690 aporia-3.2.0/src/aporia/as_code/stack.py
+-rw-r--r--   0        0        0        0 2023-07-02 19:20:47.422690 aporia-3.2.0/src/aporia/sdk/__init__.py
+-rw-r--r--   0        0        0     3233 2023-07-02 19:20:47.422690 aporia-3.2.0/src/aporia/sdk/aporia_api.py
+-rw-r--r--   0        0        0      723 2023-07-02 19:20:47.422690 aporia-3.2.0/src/aporia/sdk/base.py
+-rw-r--r--   0        0        0     1531 2023-07-02 19:20:47.422690 aporia-3.2.0/src/aporia/sdk/client.py
+-rw-r--r--   0        0        0     2148 2023-07-02 19:20:47.422690 aporia-3.2.0/src/aporia/sdk/custom_metrics.py
+-rw-r--r--   0        0        0     1822 2023-07-02 19:20:47.422690 aporia-3.2.0/src/aporia/sdk/dashboards.py
+-rw-r--r--   0        0        0     3610 2023-07-02 19:20:47.422690 aporia-3.2.0/src/aporia/sdk/data_sources.py
+-rw-r--r--   0        0        0     6709 2023-07-02 19:20:47.422690 aporia-3.2.0/src/aporia/sdk/datasets.py
+-rw-r--r--   0        0        0     1844 2023-07-02 19:20:47.422690 aporia-3.2.0/src/aporia/sdk/messaging.py
+-rw-r--r--   0        0        0     6108 2023-07-02 19:20:47.422690 aporia-3.2.0/src/aporia/sdk/metrics.py
+-rw-r--r--   0        0        0     6326 2023-07-02 19:20:47.422690 aporia-3.2.0/src/aporia/sdk/models.py
+-rw-r--r--   0        0        0    86057 2023-07-02 19:20:47.422690 aporia-3.2.0/src/aporia/sdk/monitors.py
+-rw-r--r--   0        0        0     3506 2023-07-02 19:20:47.422690 aporia-3.2.0/src/aporia/sdk/segments.py
+-rw-r--r--   0        0        0     3048 2023-07-02 19:20:47.422690 aporia-3.2.0/src/aporia/sdk/versions.py
+-rw-r--r--   0        0        0     3474 1970-01-01 00:00:00.000000 aporia-3.2.0/PKG-INFO
```

### Comparing `aporia-3.1.0/README.md` & `aporia-3.2.0/README.md`

 * *Files identical despite different names*

### Comparing `aporia-3.1.0/pyproject.toml` & `aporia-3.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aporia"
-version = "3.1.0"
+version = "3.2.0"
 description = ""
 authors = ["Aporia <support@aporia.com>"]
 readme = "README.md"
 packages = [
     { include = "aporia", from = "src" }
 ]
```

### Comparing `aporia-3.1.0/src/aporia/as_code/__init__.py` & `aporia-3.2.0/src/aporia/as_code/__init__.py`

 * *Files identical despite different names*

### Comparing `aporia-3.1.0/src/aporia/as_code/resources/base.py` & `aporia-3.2.0/src/aporia/as_code/resources/base.py`

 * *Files 7% similar despite different names*

```diff
@@ -39,7 +39,11 @@
     @abstractmethod
     def update(self, client: Client, id: str) -> Dict:
         ...
 
     @abstractmethod
     def delete(self, client: Client, id: str):
         ...
+
+    @abstractmethod
+    def get_diff(self, resource_data: Dict) -> Dict:
+        ...
```

### Comparing `aporia-3.1.0/src/aporia/as_code/resources/custom_metrics.py` & `aporia-3.2.0/src/aporia/as_code/resources/custom_metrics.py`

 * *Files 14% similar despite different names*

```diff
@@ -33,7 +33,14 @@
         custom_metric = _CustomMetric.read(client=client, id=id)
         custom_metric.update(**self._args)
         return custom_metric.raw_data
 
     @classmethod
     def delete(cls, client: Client, id: str):
         _CustomMetric.delete_by_id(client=client, id=id)
+
+    def get_diff(self, resource_data: Dict) -> Dict:
+        diffs = {}
+        for k in self._args.keys():
+            if self._args[k] != resource_data[k]:
+                diffs[k] = (resource_data[k], self._args[k])
+        return diffs
```

### Comparing `aporia-3.1.0/src/aporia/as_code/resources/data_source.py` & `aporia-3.2.0/src/aporia/as_code/resources/segment.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,59 +1,84 @@
-from typing import Any, Dict, Optional, Tuple, Union
+from typing import Any, Dict, List, Optional, Tuple, Union
 
 from aporia.as_code.resources.base import BaseResource, CompareStatus
 from aporia.sdk.client import Client
-from aporia.sdk.data_sources import DataSource as _DataSource
-from aporia.sdk.data_sources import DataSourceType
+from aporia.sdk.segments import Segment as _Segment
 
 
-class DataSource(BaseResource):
+class Segment(BaseResource):
     def __init__(
         self,
         resource_name: str,
         /,
         *,
-        type: Union[DataSourceType, str],
-        connection_data: Dict[str, Any],
         name: Optional[str] = None,
+        field: Optional[str] = None,
+        values: Optional[Union[List[str], List[Union[float, int]]]] = None,
+        terms: Optional[List[Tuple[str, str]]] = None,
     ):
-        self.dependants = []
         self.name = resource_name
+        self.dependants = []
         if name is None:
             name = resource_name
 
-        self._args = {
-            "name": name,
-            "data_source_type": DataSourceType(type),
-            "connection_data": connection_data,
-        }
+        self._args = {"name": name}
+        if field is not None:
+            if values is None:
+                raise Exception("Must supply values for automatic segment")
+            self._args["field_name"] = field
+            self._args["values"] = values
+        elif terms is not None:
+            if values is not None:
+                raise Exception("For custom segments, only specify the terms parameter")
+            self._args["terms"] = terms
+        else:
+            raise Exception("Supply either field+values or terms")
 
     def compare(self, resource_data: Dict) -> CompareStatus:
+        values = self._args.get("values", [])
+        if "terms" in self._args.keys():
+            values = [term[1] for term in self._args["terms"]]
         if all(
             [
+                self._args.get("terms") == resource_data["terms_values"],
+                self._args.get("field_name") == (resource_data["field"] or {}).get("name"),
+                values == resource_data["values"],
                 self._args["name"] == resource_data["name"],
-                self._args["data_source_type"].value == resource_data["type"],
-                # TODO: Data source configuration isn't getable
-                # self._args["connection_data"] == resource_data["connection"],
             ]
         ):
             return CompareStatus.SAME
-        return CompareStatus.MISMATCHED
+        elif any(
+            [
+                self._args.get("terms") != resource_data["terms_values"],
+                self._args.get("field_name") != (resource_data["field"] or {}).get("name"),
+                values != resource_data["values"],
+            ]
+        ):
+            return CompareStatus.MISMATCHED
+        else:
+            return CompareStatus.UPDATEABLE
 
     def setarg(self, arg_name: str, arg_value: Any):
         self._args[arg_name] = arg_value
 
     def create(self, client: Client) -> Tuple[str, Dict]:
-        data_source = _DataSource.create(client=client, **self._args)
-        return data_source.id, data_source.raw_data
+        segment = _Segment.create(client=client, **self._args)
+        return segment.id, segment.raw_data
 
     def read(self, client: Client, id: str) -> Dict:
-        return _DataSource.read(client=client, id=id).raw_data
+        return _Segment.read(client=client, id=id).raw_data
 
     def update(self, client: Client, id: str) -> Dict:
-        data_source = _DataSource.read(client=client, id=id)
-        data_source.update(**self._args)
-        return data_source.raw_data
+        segment = _Segment.read(client=client, id=id)
+        segment.update(**self._args)
+        return segment.raw_data
 
     @classmethod
     def delete(cls, client: Client, id: str):
-        _DataSource.delete_by_id(client=client, id=id)
+        _Segment.delete_by_id(client=client, id=id)
+
+    def get_diff(self, resource_data: Dict) -> Dict:
+        diffs = {}
+        if self._args["name"] != resource_data["name"]:
+            diffs["name"] = (resource_data["name"], self._args["name"])
+        return diffs
```

### Comparing `aporia-3.1.0/src/aporia/as_code/resources/dataset.py` & `aporia-3.2.0/src/aporia/as_code/resources/dataset.py`

 * *Files 4% similar despite different names*

```diff
@@ -181,7 +181,13 @@
         dataset = _Dataset.read(client=client, id=id)
         dataset.update(**self._args)
         return dataset.raw_data
 
     @classmethod
     def delete(cls, client: Client, id: str):
         raise NonDeletableResourceException()
+
+    def get_diff(self, resource_data: Dict) -> Dict:
+        diffs = {}
+        if self._args["connection_data"] != resource_data["config"]:
+            diffs["connection_data"] = (resource_data["config"], self._args["connection_data"])
+        return diffs
```

### Comparing `aporia-3.1.0/src/aporia/as_code/resources/model.py` & `aporia-3.2.0/src/aporia/as_code/resources/model.py`

 * *Files 19% similar despite different names*

```diff
@@ -98,7 +98,23 @@
         model = _Model.read(client=client, id=id)
         model.update(**self._args)
         return model.raw_data
 
     @classmethod
     def delete(cls, client: Client, id: str):
         _Model.delete_by_id(client=client, id=id)
+
+    def get_diff(self, resource_data: Dict) -> Dict:
+        diffs = {}
+        if self._args["name"] != resource_data["name"]:
+            diffs["name"] = (resource_data["name"], self._args["name"])
+        if self._args["model_type"].value != resource_data["type"]:
+            diffs["model_type"] = (resource_data["type"], self._args["model_type"])
+        for k in ["description", "icon", "color", "owner"]:
+            if k in self._args:
+                if isinstance(self._args[k], Enum):
+                    if self._args[k].value != resource_data[k]:
+                        diffs[k] = (resource_data[k], self._args[k].value)
+                else:
+                    if self._args[k] != resource_data[k]:
+                        diffs[k] = (resource_data[k], self._args[k])
+        return diffs
```

### Comparing `aporia-3.1.0/src/aporia/as_code/resources/monitor.py` & `aporia-3.2.0/src/aporia/as_code/resources/monitor.py`

 * *Files 13% similar despite different names*

```diff
@@ -74,19 +74,21 @@
         baseline: Optional[BaselineConfiguration] = None,
         baseline_segment: Optional[Segment] = None,
         dataset: Optional[Dataset] = None,
         raw_inputs: Optional[List[str]] = None,
         features: Optional[List[str]] = None,
         predictions: Optional[List[str]] = None,
         is_embedding_monitor: bool = False,
-        min_prediction_count: Optional[int] = None,
+        min_focal_prediction_count: Optional[int] = None,
+        min_baseline_prediction_count: Optional[int] = None,
         # Optional Logic Evaluation Parameters
         percentage: Optional[int] = None,
         thresholds: Optional[ThresholdConfiguration] = None,
         sensitivity: Optional[float] = None,
+        alert_on_increase_only: Optional[bool] = None,
         min: Optional[int] = None,
         max: Optional[int] = None,
         staleness_period: Optional[TimePeriod] = None,
         distance: Optional[float] = None,
         new_values_ratio_threshold: Optional[float] = None,
         new_values_count_threshold: Optional[int] = None,
         # Optional Metric Parameters
@@ -150,18 +152,20 @@
             features=features if use_features else None,
             predictions=predictions if use_predictions else None,
             is_embedding_monitor=is_embedding_monitor,
             metric=metric,
             percentage=percentage,
             thresholds=thresholds,
             sensitivity=sensitivity,
+            alert_on_increase_only=alert_on_increase_only,
             min=min,
             max=max,
             staleness_period=staleness_period,
-            min_prediction_count=min_prediction_count,
+            min_focal_prediction_count=min_focal_prediction_count,
+            min_baseline_prediction_count=min_baseline_prediction_count,
             custom_metric_id=custom_metric.name
             if custom_metric is not None
             else custom_metric_id
             if custom_metric_id is not None
             else None,
             distance=distance,
             new_values_count_threshold=new_values_count_threshold,
@@ -272,7 +276,20 @@
         monitor = _Monitor.read(client=client, id=id)
         monitor.update(**self._args)
         return monitor.raw_data
 
     @classmethod
     def delete(cls, client: Client, id: str):
         _Monitor.delete_by_id(client=client, id=id)
+
+    def get_diff(self, resource_data: Dict) -> Dict:
+        diffs = {}
+        if self._args["name"] != resource_data["name"]:
+            diffs["name"] = (resource_data["name"], self._args["name"])
+        if "comment" in self._args:
+            if self._args["comment"] != resource_data["comment"]:
+                diffs["comment"] = (resource_data["comment"], self._args["comment"])
+        if self._args["is_active"] != resource_data["is_active"]:
+            diffs["is_active"] = (resource_data["is_active"], self._args["is_active"])
+        if self._args["configuration"].to_dict() != resource_data["configuration"]:
+            diffs["configuration"] = (resource_data["configuration"], self._args["configuration"].to_dict())
+        return diffs
```

### Comparing `aporia-3.1.0/src/aporia/as_code/resources/segment.py` & `aporia-3.2.0/src/aporia/as_code/resources/version.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,78 +1,65 @@
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
-        terms: Optional[List[Tuple[str, str]]] = None,
+        serving: Optional[Dataset] = None,
+        training: Optional[Dataset] = None,
     ):
         self.name = resource_name
         self.dependants = []
+        self.sub_resources = []
         if name is None:
             name = resource_name
 
         self._args = {"name": name}
-        if field is not None:
-            if values is None:
-                raise Exception("Must supply values for automatic segment")
-            self._args["field_name"] = field
-            self._args["values"] = values
-        elif terms is not None:
-            if values is not None:
-                raise Exception("For custom segments, only specify the terms parameter")
-            self._args["terms"] = terms
-        else:
-            raise Exception("Supply either field+values or terms")
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
-        values = self._args.get("values", [])
-        if "terms" in self._args.keys():
-            values = [term[1] for term in self._args["terms"]]
-        if all(
-            [
-                self._args.get("terms") == resource_data["terms_values"],
-                self._args.get("field_name") == (resource_data["field"] or {}).get("name"),
-                values == resource_data["values"],
-                self._args["name"] == resource_data["name"],
-            ]
-        ):
+        if all([self._args[k] == resource_data[k] for k in self._args.keys()]):
             return CompareStatus.SAME
-        elif any(
-            [
-                self._args.get("terms") != resource_data["terms_values"],
-                self._args.get("field_name") != (resource_data["field"] or {}).get("name"),
-                values != resource_data["values"],
-            ]
-        ):
-            return CompareStatus.MISMATCHED
-        else:
-            return CompareStatus.UPDATEABLE
+        return CompareStatus.UPDATEABLE
 
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
+
+    def get_diff(self, resource_data: Dict) -> Dict:
+        diffs = {}
+        for k in self._args.keys():
+            if self._args[k] != resource_data[k]:
+                diffs[k] = (resource_data[k], self._args[k])
+        return diffs
```

### Comparing `aporia-3.1.0/src/aporia/as_code/stack.py` & `aporia-3.2.0/src/aporia/as_code/stack.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 
 
 class StackAction(Enum):
     CREATE = "create"
     DELETE = "delete"
     PREVIEW = "preview"
     REFRESH = "refresh"
+    DIFF = "diff"
 
 
 class ResourceStatus(Enum):
     CREATED = "created"  # Found in config file
     MISSING = "missing"  # Not found in config file, create
     DEPRECATED = "deprecated"  # Found in config file, definition changed
     # TODO: Support that
@@ -137,14 +138,34 @@
             print("Removed resources:")
         for unique_id in self._delete_resources.keys():
             resource_parts = unique_id.split("/")
             depth = len(resource_parts) - 1
             name = resource_parts[-1]
             print(f"|-{'----' * depth}{name} - delete")
 
+    def _get_diff_config(self, output_format: str = "print"):
+        diffs = {}
+        for unique_id, resource_entry in self._resources.items():
+            if resource_entry.status is not ResourceStatus.DEPRECATED:
+                continue
+            resource_data = self._output[unique_id]
+            resource_diff = resource_entry.resource.get_diff(resource_data=resource_data)
+            diffs[unique_id] = {}
+            for config_name, (old, new) in resource_diff.items():
+                diffs[unique_id][config_name] = {"old": old, "new": new}
+        if output_format == "json":
+            print(json.dumps(diffs))
+        elif output_format == "print":
+            for unique_id, diffed_configs in diffs.items():
+                print(f"Resource '{unique_id}' changed. Changes:")
+                for config_name, config_diffs in diffed_configs.items():
+                    print(
+                        f"    Configuration '{config_name}' changed.\n        Old: {config_diffs['old']}\n        New: {config_diffs['new']}"
+                    )
+
     def __pop_deleted_sub_resources(self, non_deleteable_resources: List[str], unique_id):
         resource_entry = self._resources[unique_id]
         if hasattr(resource_entry.resource, "sub_resources"):
             for resource, _ in resource_entry.resource.sub_resources:
                 sub_resource_unique_id = f"{unique_id}/{resource.name}"
                 if sub_resource_unique_id in non_deleteable_resources:
                     self.__pop_deleted_sub_resources(
@@ -267,15 +288,20 @@
             [c if c in (string.ascii_letters + string.digits + "_") else "_" for c in name]
         ).lower()
         if result[0] in string.digits:
             result = f"_{result}"
         return result
 
     def __create_python_representation(
-        self, resource: SDKBaseAporiaResource, index: int
+        self,
+        resource: SDKBaseAporiaResource,
+        index: int,
+        version_id_to_object: Optional[Dict[str, str]] = None,
+        segment_id_to_object: Optional[Dict[str, str]] = None,
+        custom_metric_id_to_object: Optional[Dict[str, str]] = None,
     ) -> Tuple[str, str]:
         if isinstance(resource, SDKSegment):
             code = f"""{self.__resource_name_to_python_name(resource.name)} = aporia.Segment(
     "{resource.name}",
 """
             if resource.raw_data["field"] is not None:
                 code += f"""\tfield="{resource.raw_data["field"]["name"]}",\n"""
@@ -361,18 +387,26 @@
             if parsed_config.identification.predictions is not None:
                 predictions = parsed_config.identification.predictions
                 predictions_array = (
                     f"""[{', '.join(f'"{prediction}"' for prediction in predictions)}]"""
                 )
                 code += f"\tpredictions={predictions_array},\n"
             if parsed_config.identification.models.version is not None:
-                code += f'\tversion_id="{parsed_config.identification.models.version}",\n'
+                version_id = parsed_config.identification.models.version
+                if version_id in (version_id_to_object or {}):
+                    code += f"\tversion={version_id_to_object[version_id]},\n"
+                else:
+                    code += f'\tversion_id="{version_id}",\n'
 
             if parsed_config.identification.segment.group is not None:
-                code += f'\tsegment_id="{parsed_config.identification.segment.group}",\n'
+                segment_id = parsed_config.identification.segment.group
+                if segment_id in (segment_id_to_object or {}):
+                    code += f"\tsegment={segment_id_to_object[segment_id]},\n"
+                else:
+                    code += f'\tsegment_id="{segment_id}",\n'
 
             if parsed_config.identification.segment.value is not None:
                 segment_value = parsed_config.identification.segment.value
                 if isinstance(segment_value, str):
                     segment_value = f'"{segment_value}"'
                 code += f"\tsegment_value={segment_value},\n"
 
@@ -382,15 +416,19 @@
                 code += f"\tbaseline=aporia.BaselineConfiguration(**{parsed_config.baseline.to_dict()}),\n"
 
             # Metric Configuration
             if resource.type in [MonitorType.PERFORMANCE_DEGRADATION, MonitorType.METRIC_CHANGE]:
                 code += f"\tmetric=aporia.MetricType.{parsed_config.metric.type.name},\n"
             metric_config = parsed_config.metric
             if metric_config.id is not None:
-                code += f'\tcustom_metric_id="{metric_config.id}",\n'
+                custom_metric_id = parsed_config.identification.models.custom_metric
+                if custom_metric_id in (custom_metric_id_to_object or {}):
+                    code += f"\tcustom_metric={custom_metric_id_to_object[custom_metric_id]},\n"
+                else:
+                    code += f'\tcustom_metric_id="{custom_metric_id}",\n'
             if metric_config.average is not None:
                 code += f"\taverage_method=aporia.AverageMethod.{metric_config.average.name},\n"
             if metric_config.metricAtK is not None:
                 code += f"\tk={metric_config.metricAtK},\n"
             if metric_config.threshold is not None:
                 code += f"\tprediction_threshold={metric_config.threshold},\n"
             if metric_config.metricPerClass is not None:
@@ -425,14 +463,18 @@
                     code += (
                         f'\tstaleness_period="{logic_evaluation_configuration.max.to_string()}",\n'
                     )
                 else:
                     code += f"\tmax={logic_evaluation_configuration.max},\n"
             if logic_evaluation_configuration.sensitivity is not None:
                 code += f"\tsensitivity={logic_evaluation_configuration.sensitivity},\n"
+            if logic_evaluation_configuration.testOnlyIncrease is not None:
+                code += (
+                    f"\talert_on_increase_only={logic_evaluation_configuration.testOnlyIncrease},\n"
+                )
             if logic_evaluation_configuration.thresholds is not None:
                 code += f"\tthresholds=aporia.ThresholdConfiguration(**{logic_evaluation_configuration.thresholds.to_dict()}),\n"
             if logic_evaluation_configuration.distance is not None:
                 code += f"\tdistance={logic_evaluation_configuration.distance},\n"
             if logic_evaluation_configuration.new_values_count_threshold is not None:
                 code += f"\tnew_values_count_threshold={logic_evaluation_configuration.new_values_count_threshold},\n"
             if logic_evaluation_configuration.new_values_ratio_threshold is not None:
@@ -462,27 +504,29 @@
                             code += f"\tmessaging={messaging},\n"
                         added_alert = True
                         if action.maxAlertsPerDay is not None:
                             code += f"\tmax_alerts_per_day={action.maxAlertsPerDay},\n"
 
             # Precondition Configuration
             added_min = False
-            added_min_datapoints = False
+            added_min_focal_datapoints = False
+            added_min_baseline_datapoints = False
             for precondition in parsed_config.preConditions or []:
                 if precondition.name is PreConditionType.FOCAL_DATA_VALUE_IN_RANGE:
                     if not added_min:
                         code += f"\tmin={precondition.min},\n"
                         added_min = True
-                if precondition.name in [
-                    PreConditionType.MIN_BASELINE_DATA_POINTS,
-                    PreConditionType.MIN_FOCAL_DATA_POINTS,
-                ]:
-                    if not added_min_datapoints:
-                        code += f"\tmin_prediction_count={precondition.value},\n"
-                        added_min_datapoints = True
+                if precondition.name is PreConditionType.MIN_FOCAL_DATA_POINTS:
+                    if not added_min_focal_datapoints:
+                        code += f"\tmin_focal_prediction_count={precondition.value},\n"
+                        added_min_focal_datapoints = True
+                if precondition.name is PreConditionType.MIN_BASELINE_DATA_POINTS:
+                    if not added_min_baseline_datapoints:
+                        code += f"\tmin_baseline_prediction_count={precondition.value},\n"
+                        added_min_baseline_datapoints = True
 
             code += ")"
             return code, self.__resource_name_to_python_name(resource.name)
         elif isinstance(resource, SDKModel):
             return f"""{self.__resource_name_to_python_name(resource.name)} = aporia.Model(
     "{resource.name}",
     type=aporia.ModelType.{resource.type.name},
@@ -510,34 +554,46 @@
         model_segments = []
         model_custom_metrics = []
         model_monitors = []
         versions_code = []
         segments_code = []
         custom_metrics_code = []
         monitors_code = []
+        version_id_to_object = {}
+        segment_id_to_object = {}
+        custom_metric_id_to_object = {}
         for index, (version, datasets) in enumerate(versions):
             datasets_code = [
                 self.__create_python_representation(dataset, index=index)[0] for dataset in datasets
             ]
             version_code, version_name = self.__create_python_representation(version, index=index)
+            version_id_to_object[version.id] = version_name
             full_version_code = "\n".join([*datasets_code, version_code])
             versions_code.append(full_version_code)
             model_versions.append(version_name)
         for index, segment in enumerate(segments):
             segment_code, segment_name = self.__create_python_representation(segment, index=index)
+            segment_id_to_object[segment.id] = segment_name
             segments_code.append(segment_code)
             model_segments.append(segment_name)
         for index, custom_metric in enumerate(custom_metrics):
             custom_metric_code, custom_metric_name = self.__create_python_representation(
                 custom_metric, index=index
             )
+            custom_metric_id_to_object[custom_metric.id] = custom_metric_name
             custom_metrics_code.append(custom_metric_code)
             model_custom_metrics.append(custom_metric_name)
         for index, monitor in enumerate(monitors):
-            monitor_code, monitor_name = self.__create_python_representation(monitor, index=index)
+            monitor_code, monitor_name = self.__create_python_representation(
+                monitor,
+                index=index,
+                version_id_to_object=version_id_to_object,
+                segment_id_to_object=segment_id_to_object,
+                custom_metric_id_to_object=custom_metric_id_to_object,
+            )
             monitors_code.append(monitor_code)
             model_monitors.append(monitor_name)
 
         model_code = model_code.replace("versions=[]", f"versions=[{', '.join(model_versions)}]")
         model_code = model_code.replace("segments=[]", f"segments=[{', '.join(model_segments)}]")
         model_code = model_code.replace(
             "custom_metrics=[]", f"custom_metrics=[{', '.join(model_custom_metrics)}]"
@@ -711,14 +767,15 @@
         action: StackAction = StackAction.CREATE,
         skip_preview: bool = False,
         yes: bool = False,
         rollback=True,
         yes_rollback=False,
         config_path: Optional[str] = None,
         debug: Optional[bool] = False,
+        diff_format: str = "print",
     ):
         action = StackAction(action)
         # TODO: Read config_path, and apply diffs. Then write to config_path
         if config_path is not None:
             try:
                 with open(config_path, "r") as f:
                     self._output = json.loads(f.read())
@@ -764,14 +821,17 @@
                     return
             error = self._destroy()
             if error is not None:
                 if debug:
                     traceback.print_exception(error)
                 else:
                     print(error)
+        elif action is StackAction.DIFF:
+            self._get_diff_config(output_format=diff_format)
+            return
         else:
             raise ValueError("Unknown action")
 
         if config_path is not None:
             with open(config_path, "w") as f:
                 f.write(json.dumps(self._output))
```

### Comparing `aporia-3.1.0/src/aporia/sdk/aporia_api.py` & `aporia-3.2.0/src/aporia/sdk/aporia_api.py`

 * *Files identical despite different names*

### Comparing `aporia-3.1.0/src/aporia/sdk/base.py` & `aporia-3.2.0/src/aporia/sdk/base.py`

 * *Files identical despite different names*

### Comparing `aporia-3.1.0/src/aporia/sdk/client.py` & `aporia-3.2.0/src/aporia/sdk/client.py`

 * *Files identical despite different names*

### Comparing `aporia-3.1.0/src/aporia/sdk/custom_metrics.py` & `aporia-3.2.0/src/aporia/sdk/custom_metrics.py`

 * *Files identical despite different names*

### Comparing `aporia-3.1.0/src/aporia/sdk/dashboards.py` & `aporia-3.2.0/src/aporia/sdk/dashboards.py`

 * *Files identical despite different names*

### Comparing `aporia-3.1.0/src/aporia/sdk/data_sources.py` & `aporia-3.2.0/src/aporia/sdk/data_sources.py`

 * *Files identical despite different names*

### Comparing `aporia-3.1.0/src/aporia/sdk/datasets.py` & `aporia-3.2.0/src/aporia/sdk/datasets.py`

 * *Files identical despite different names*

### Comparing `aporia-3.1.0/src/aporia/sdk/messaging.py` & `aporia-3.2.0/src/aporia/sdk/messaging.py`

 * *Files identical despite different names*

### Comparing `aporia-3.1.0/src/aporia/sdk/metrics.py` & `aporia-3.2.0/src/aporia/sdk/metrics.py`

 * *Files identical despite different names*

### Comparing `aporia-3.1.0/src/aporia/sdk/models.py` & `aporia-3.2.0/src/aporia/sdk/models.py`

 * *Files identical despite different names*

### Comparing `aporia-3.1.0/src/aporia/sdk/monitors.py` & `aporia-3.2.0/src/aporia/sdk/monitors.py`

 * *Files 2% similar despite different names*

```diff
@@ -297,14 +297,15 @@
     name: LogicEvaluationType
     # Needed for range (Both must exist, if one isn't used, it should be null)
     min: Optional[float] = None
     # Also needed for ratio (float) and staleness (TimePeriod)
     max: Optional[Union[float, TimePeriod]] = None
     # Needed for timeseries anomaly
     sensitivity: Optional[float] = None
+    testOnlyIncrease: Optional[bool] = None
     # Needed for Aporia drift score
     thresholds: Optional[ThresholdConfiguration] = None
     # Needed for non-absolute Value range
     distance: Optional[float] = None
     # Needed for new-values value range
     new_values_count_threshold: Optional[int] = None
     new_values_ratio_threshold: Optional[float] = None
@@ -318,44 +319,51 @@
     @root_validator()
     def _validate_logic_evaluation(cls, values):
         if values["name"] is LogicEvaluationType.RANGE:
             if isinstance(values["max"], TimePeriod):
                 raise ValueError("max must be a float or None for Range logic evaluation")
             if (
                 values["sensitivity"] is not None
+                or values["testOnlyIncrease"] is not None
                 or values["thresholds"] is not None
                 or values["distance"] is not None
             ):
                 raise ValueError("Only min and max can appear for Range logic evaluation")
 
         if values["name"] is LogicEvaluationType.VALUES_RANGE:
             if isinstance(values["max"], TimePeriod):
                 raise ValueError("max must be a float or None for Range logic evaluation")
             if isinstance(values["min"], TimePeriod):
                 raise ValueError("min must be a float or None for Range logic evaluation")
-            if values["sensitivity"] is not None or values["thresholds"] is not None:
+            if (
+                values["sensitivity"] is not None
+                or values["thresholds"] is not None
+                or values["testOnlyIncrease"] is not None
+            ):
                 raise ValueError("Only min and max can appear for Value Range logic evaluation")
 
         if values["name"] is LogicEvaluationType.RATIO:
             if isinstance(values["max"], TimePeriod):
                 raise ValueError("max must be a float for Ratio logic evaluation")
             if (
                 values["sensitivity"] is not None
+                or values["testOnlyIncrease"] is not None
                 or values["thresholds"] is not None
                 or values["distance"] is not None
                 or values["new_values_count_threshold"] is not None
                 or values["new_values_ratio_threshold"] is not None
             ):
                 raise ValueError("Only min and max can appear for Ratio logic evaluation")
 
         if values["name"] is LogicEvaluationType.MODEL_STALENESS:
             if not isinstance(values["max"], TimePeriod):
                 raise ValueError("max must be a TimePeriod for Stalenss logic evaluation")
             if (
                 values["sensitivity"] is not None
+                or values["testOnlyIncrease"] is not None
                 or values["thresholds"] is not None
                 or values["distance"] is not None
                 or values["new_values_count_threshold"] is not None
                 or values["new_values_ratio_threshold"] is not None
                 or values["min"] is not None
             ):
                 raise ValueError("Only max can appear for Staleness logic evaluation")
@@ -378,14 +386,15 @@
         if values["name"] is LogicEvaluationType.APORIA_DRIFT_SCORE:
             if values["thresholds"] is None:
                 raise ValueError("thresholds must appear for Aporia Drift Score Logic Evaluation")
             if (
                 values["max"] is not None
                 or values["min"] is not None
                 or values["sensitivity"] is not None
+                or values["testOnlyIncrease"] is not None
                 or values["distance"] is not None
                 or values["new_values_count_threshold"] is not None
                 or values["new_values_ratio_threshold"] is not None
             ):
                 raise ValueError(
                     "Only thresholds can appear for Aporia Drift Score logic evaluation"
                 )
@@ -400,14 +409,16 @@
         if self.max is not None:
             if isinstance(self.max, TimePeriod):
                 result["max"] = self.max.to_string()
             else:
                 result["max"] = self.max
         if self.sensitivity is not None:
             result["sensitivity"] = self.sensitivity
+        if self.testOnlyIncrease is not None:
+            result["testOnlyIncrease"] = self.testOnlyIncrease
         if self.thresholds is not None:
             result["thresholds"] = self.thresholds.to_dict()
 
         if self.distance is not None:
             result["distance"] = self.distance
 
         if self.new_values_count_threshold is not None:
@@ -579,25 +590,22 @@
     def _validate_monitor_configuration(cls, values):
         if values.get("baseline") is not None:
             # For non-training monitors, skipPeriod defaults to the focal timePeriod, unless it's per segment
             if values["baseline"].source is SourceType.SERVING:
                 # TODO: Fix that, as this sets skipPeriod even when using segments
                 # TODO: CRITICAL BUG! This ruins the type infering
                 if (
-                    values["identification"].segment.group is None
-                    and values["identification"].segment.value is None
-                    and values["baseline"].segmentValue is None
+                    values["baseline"].segmentValue is None
                     and values["baseline"].segmentGroupId is None
                 ):
                     if values["baseline"].skipPeriod is None:
                         values["baseline"].skipPeriod = values["focal"].timePeriod
 
-            # For non-histogram monitors, aggregationPeriod defaults to timePeriod
-            # TODO: Verify when it appears
-            if values["metric"].type not in [MetricType.HISTOGRAM, MetricType.EUCLIDEAN_DISTANCE]:
+            # For anomaly detection monitors, aggregationPeriod defaults to timePeriod
+            if values["logicEvaluations"][0].name is LogicEvaluationType.TIME_SERIES_ANOMALY:
                 if values["baseline"].aggregationPeriod is None:
                     values["baseline"].aggregationPeriod = values["focal"].timePeriod
 
         return values
 
     def to_dict(self):
         result = {
@@ -847,15 +855,17 @@
     MonitorType.MODEL_ACTIVITY: {
         DetectionMethod.ANOMALY: _MonitorParamBuilder(
             metric_builder=lambda **kw: MetricConfiguration(type=MetricType.COUNT),
             alert_type=AlertType.MODEL_ACTIVITY_ANOMALY,
             visualization_builder=lambda **kw: VisualizationType.RANGE_LINE_CHART,
             description_builder=lambda **kw: "An anomaly in the number of total predictions was detected. <br /> The anomaly was observed in the <b>{model}</b> model, in version <b>{model_version}</b> for the <b>last {focal_time_period} ({focal_times})</b> <b>{focal_segment}</b>. <br /><br /> Based on total predictions count history, the count was expected to be between <b>{last_lower_bound}</b> to <b>{last_upper_bound}</b>, but <b>{focal_value}</b> was received. <br /><br /> Total prediction anomaly might occur because: <ul><li>Natural changes in model invocations</li><li>Serving environment fault</li><li>Malicious attempt to analyse model behaviour</li></ul>",
             logic_evaluation_builder=lambda **kw: LogicEvaluationConfiguration(
-                name=LogicEvaluationType.TIME_SERIES_ANOMALY, sensitivity=kw["sensitivity"]
+                name=LogicEvaluationType.TIME_SERIES_ANOMALY,
+                sensitivity=kw["sensitivity"],
+                testOnlyIncrease=kw["testOnlyIncrease"],
             ),
             needed_args=["sensitivity", "baseline"],
         ),
         DetectionMethod.PERCENTAGE: _MonitorParamBuilder(
             metric_builder=lambda **kw: MetricConfiguration(type=MetricType.COUNT),
             alert_type=AlertType.MODEL_ACTIVITY_CHANGE,
             visualization_builder=lambda **kw: VisualizationType.VALUE_OVER_TIME,
@@ -900,15 +910,15 @@
             logic_evaluation_builder=lambda **kw: LogicEvaluationConfiguration(
                 name=LogicEvaluationType.RANGE, min=0, max=kw["max"]
             )
             if kw["is_embedding"]
             else LogicEvaluationConfiguration(
                 name=LogicEvaluationType.APORIA_DRIFT_SCORE, thresholds=kw["thresholds"]
             ),
-            description_builder=lambda **kw: f"A data drift was detected in feature <b>'{{field}}'</b> {{importance}}.{'{drift_score_text}' if kw['is_embedding'] else ''}<br /> The drift was observed in the <b>{{model}}</b> model, in version <b>{{model_version}}</b> for the <b>last {{focal_time_period}} ({{focal_times}})</b> <b>{{focal_segment}}</b> compared to the <b>last {{baseline_time_period}} ({{baseline_times}})</b>. <br /><br /> Data drift can have a significant effect on model behavior and may lead to unexpected results.<br /><br /> Data drift might occur because: <ul><li>Natural changes in data</li><li>Data store / provider schema changes</li><li>Data store / provider issues</li><li>Data processing issues</li></ul>",
+            description_builder=lambda **kw: f"A data drift was detected in feature <b>'{{field}}'</b> {{importance}}.{'' if kw['is_embedding'] else '{drift_score_text}'}<br /> The drift was observed in the <b>{{model}}</b> model, in version <b>{{model_version}}</b> for the <b>last {{focal_time_period}} ({{focal_times}})</b> <b>{{focal_segment}}</b> compared to the <b>last {{baseline_time_period}} ({{baseline_times}})</b>. <br /><br /> Data drift can have a significant effect on model behavior and may lead to unexpected results.<br /><br /> Data drift might occur because: <ul><li>Natural changes in data</li><li>Data store / provider schema changes</li><li>Data store / provider issues</li><li>Data processing issues</li></ul>",
             needed_args=[["thresholds", "max"], "baseline"],
         ),
         DetectionMethod.COMPARED_TO_SEGMENT: _MonitorParamBuilder(
             alert_type=AlertType.DATA_DRIFT_SEGMENT_CHANGE,
             visualization_builder=lambda **kw: VisualizationType.EMBEDDING_DRIFT_CHART
             if kw["is_embedding"]
             else VisualizationType.DISTRIBUTION_COMPARE_CHART,
@@ -918,15 +928,15 @@
             logic_evaluation_builder=lambda **kw: LogicEvaluationConfiguration(
                 name=LogicEvaluationType.RANGE, min=0, max=kw["max"]
             )
             if kw["is_embedding"]
             else LogicEvaluationConfiguration(
                 name=LogicEvaluationType.APORIA_DRIFT_SCORE, thresholds=kw["thresholds"]
             ),
-            description_builder=lambda **kw: f"A data drift was detected in feature <b>'{{field}}'</b> {{importance}}.{'{drift_score_text}' if kw['is_embedding'] else ''}<br /> The drift was observed in the <b>{{model}}</b> model, in version <b>{{model_version}}</b> for the <b>last {{focal_time_period}} ({{focal_times}})</b> <b>{{focal_segment}}</b> compared to the <b>last {{baseline_time_period}} ({{baseline_times}})</b> <b>{{baseline_segment}}</b>. <br /><br /> Data drift can have a significant effect on model behavior and may lead to unexpected results.<br /><br /> Data drift might occur because: <ul><li>Natural changes in data</li><li>Data store / provider schema changes</li><li>Data store / provider issues</li><li>Data processing issues</li></ul>",
+            description_builder=lambda **kw: f"A data drift was detected in feature <b>'{{field}}'</b> {{importance}}.{'' if kw['is_embedding'] else '{drift_score_text}'}<br /> The drift was observed in the <b>{{model}}</b> model, in version <b>{{model_version}}</b> for the <b>last {{focal_time_period}} ({{focal_times}})</b> <b>{{focal_segment}}</b> compared to the <b>last {{baseline_time_period}} ({{baseline_times}})</b> <b>{{baseline_segment}}</b>. <br /><br /> Data drift can have a significant effect on model behavior and may lead to unexpected results.<br /><br /> Data drift might occur because: <ul><li>Natural changes in data</li><li>Data store / provider schema changes</li><li>Data store / provider issues</li><li>Data processing issues</li></ul>",
             needed_args=[["thresholds", "max"], "baseline"],
         ),
         DetectionMethod.COMPARED_TO_TRAINING: _MonitorParamBuilder(
             alert_type=AlertType.DATA_DRIFT_TRAINING,
             visualization_builder=lambda **kw: VisualizationType.EMBEDDING_DRIFT_CHART
             if kw["is_embedding"]
             else VisualizationType.DISTRIBUTION_COMPARE_CHART,
@@ -936,15 +946,15 @@
             logic_evaluation_builder=lambda **kw: LogicEvaluationConfiguration(
                 name=LogicEvaluationType.RANGE, min=0, max=kw["max"]
             )
             if kw["is_embedding"]
             else LogicEvaluationConfiguration(
                 name=LogicEvaluationType.APORIA_DRIFT_SCORE, thresholds=kw["thresholds"]
             ),
-            description_builder=lambda **kw: f"A data drift was detected in feature <b>'{{field}}'</b> {{importance}}.{'{drift_score_text}' if kw['is_embedding'] else ''}<br /> The drift was observed in the <b>{{model}}</b> model, in version <b>{{model_version}}</b> for the <b>last {{focal_time_period}} ({{focal_times}})</b> <b>{{focal_segment}}</b> compared to the <b>Training</b> data. <br /><br /> Data drift can have a significant effect on model behavior and may lead to unexpected results.<br /><br /> Data drift might occur because: <ul><li>Natural changes in data</li><li>Data store / provider schema changes</li><li>Data store / provider issues</li><li>Data processing issues</li></ul>",
+            description_builder=lambda **kw: f"A data drift was detected in feature <b>'{{field}}'</b> {{importance}}.{'' if kw['is_embedding'] else '{drift_score_text}'}<br /> The drift was observed in the <b>{{model}}</b> model, in version <b>{{model_version}}</b> for the <b>last {{focal_time_period}} ({{focal_times}})</b> <b>{{focal_segment}}</b> compared to the <b>Training</b> data. <br /><br /> Data drift can have a significant effect on model behavior and may lead to unexpected results.<br /><br /> Data drift might occur because: <ul><li>Natural changes in data</li><li>Data store / provider schema changes</li><li>Data store / provider issues</li><li>Data processing issues</li></ul>",
             needed_args=[["thresholds", "max"], "baseline"],
         ),
     },
     MonitorType.PREDICTION_DRIFT: {
         DetectionMethod.ANOMALY: _MonitorParamBuilder(
             alert_type=AlertType.PREDICTION_DRIFT_ANOMALY,
             visualization_builder=lambda **kw: VisualizationType.EMBEDDING_DRIFT_CHART
@@ -956,15 +966,15 @@
             logic_evaluation_builder=lambda **kw: LogicEvaluationConfiguration(
                 name=LogicEvaluationType.RANGE, min=0, max=kw["max"]
             )
             if kw["is_embedding"]
             else LogicEvaluationConfiguration(
                 name=LogicEvaluationType.APORIA_DRIFT_SCORE, thresholds=kw["thresholds"]
             ),
-            description_builder=lambda **kw: f"A prediction drift was detected in prediction <b>'{{field}}'</b> {{importance}}.{'{drift_score_text}' if kw['is_embedding'] else ''}<br /> The drift was observed in the <b>{{model}}</b> model, in version <b>{{model_version}}</b> for the <b>last {{focal_time_period}} ({{focal_times}})</b> <b>{{focal_segment}}</b> compared to the <b>last {{baseline_time_period}} ({{baseline_times}})</b>. <br /><br /> Prediction drift indicates a significant change in model's behavior. In some cases, it is a strong indicator for concept drift.<br /><br /> Prediction drift might occur because: <ul><li>Natural changes in data</li><li>Data store / provider schema changes</li><li>Data store / provider issues</li><li>Data processing issues</li></ul>",
+            description_builder=lambda **kw: f"A prediction drift was detected in prediction <b>'{{field}}'</b> {{importance}}.{'' if kw['is_embedding'] else '{drift_score_text}'}<br /> The drift was observed in the <b>{{model}}</b> model, in version <b>{{model_version}}</b> for the <b>last {{focal_time_period}} ({{focal_times}})</b> <b>{{focal_segment}}</b> compared to the <b>last {{baseline_time_period}} ({{baseline_times}})</b>. <br /><br /> Prediction drift indicates a significant change in model's behavior. In some cases, it is a strong indicator for concept drift.<br /><br /> Prediction drift might occur because: <ul><li>Natural changes in data</li><li>Data store / provider schema changes</li><li>Data store / provider issues</li><li>Data processing issues</li></ul>",
             needed_args=[["thresholds", "max"], "baseline"],
         ),
         DetectionMethod.COMPARED_TO_SEGMENT: _MonitorParamBuilder(
             alert_type=AlertType.PREDICTION_DRIFT_SEGMENT_CHANGE,
             visualization_builder=lambda **kw: VisualizationType.EMBEDDING_DRIFT_CHART
             if kw["is_embedding"]
             else VisualizationType.DISTRIBUTION_COMPARE_CHART,
@@ -974,15 +984,15 @@
             logic_evaluation_builder=lambda **kw: LogicEvaluationConfiguration(
                 name=LogicEvaluationType.RANGE, min=0, max=kw["max"]
             )
             if kw["is_embedding"]
             else LogicEvaluationConfiguration(
                 name=LogicEvaluationType.APORIA_DRIFT_SCORE, thresholds=kw["thresholds"]
             ),
-            description_builder=lambda **kw: f"A prediction drift was detected in prediction <b>'{{field}}'</b> {{importance}}.{'{drift_score_text}' if kw['is_embedding'] else ''}<br /> The drift was observed in the <b>{{model}}</b> model, in version <b>{{model_version}}</b> for the <b>last {{focal_time_period}} ({{focal_times}})</b> <b>{{focal_segment}}</b> compared to the <b>last {{baseline_time_period}} ({{baseline_times}})</b> <b>{{baseline_segment}}</b>. <br /><br /> Prediction drift indicates a significant change in model's behavior. In some cases, it is a strong indicator for concept drift.<br /><br /> Prediction drift might occur because: <ul><li>Natural changes in data</li><li>Data store / provider schema changes</li><li>Data store / provider issues</li><li>Data processing issues</li></ul>",
+            description_builder=lambda **kw: f"A prediction drift was detected in prediction <b>'{{field}}'</b> {{importance}}.{'' if kw['is_embedding'] else '{drift_score_text}'}<br /> The drift was observed in the <b>{{model}}</b> model, in version <b>{{model_version}}</b> for the <b>last {{focal_time_period}} ({{focal_times}})</b> <b>{{focal_segment}}</b> compared to the <b>last {{baseline_time_period}} ({{baseline_times}})</b> <b>{{baseline_segment}}</b>. <br /><br /> Prediction drift indicates a significant change in model's behavior. In some cases, it is a strong indicator for concept drift.<br /><br /> Prediction drift might occur because: <ul><li>Natural changes in data</li><li>Data store / provider schema changes</li><li>Data store / provider issues</li><li>Data processing issues</li></ul>",
             needed_args=[["thresholds", "max"], "baseline"],
         ),
         DetectionMethod.COMPARED_TO_TRAINING: _MonitorParamBuilder(
             alert_type=AlertType.PREDICTION_DRIFT_TRAINING,
             visualization_builder=lambda **kw: VisualizationType.EMBEDDING_DRIFT_CHART
             if kw["is_embedding"]
             else VisualizationType.DISTRIBUTION_COMPARE_CHART,
@@ -992,26 +1002,28 @@
             logic_evaluation_builder=lambda **kw: LogicEvaluationConfiguration(
                 name=LogicEvaluationType.RANGE, min=0, max=kw["max"]
             )
             if kw["is_embedding"]
             else LogicEvaluationConfiguration(
                 name=LogicEvaluationType.APORIA_DRIFT_SCORE, thresholds=kw["thresholds"]
             ),
-            description_builder=lambda **kw: f"A prediction drift was detected in prediction <b>'{{field}}'</b> {{importance}}.{'{drift_score_text}' if kw['is_embedding'] else ''}<br /> The drift was observed in the <b>{{model}}</b> model, in version <b>{{model_version}}</b> for the <b>last {{focal_time_period}} ({{focal_times}})</b> <b>{{focal_segment}}</b> compared to the <b>Training</b> data. <br /><br /> Prediction drift indicates a significant change in model's behavior. In some cases, it is a strong indicator for concept drift.<br /><br /> Prediction drift might occur because: <ul><li>Natural changes in data</li><li>Data store / provider schema changes</li><li>Data store / provider issues</li><li>Data processing issues</li></ul>",
+            description_builder=lambda **kw: f"A prediction drift was detected in prediction <b>'{{field}}'</b> {{importance}}.{'' if kw['is_embedding'] else '{drift_score_text}'}<br /> The drift was observed in the <b>{{model}}</b> model, in version <b>{{model_version}}</b> for the <b>last {{focal_time_period}} ({{focal_times}})</b> <b>{{focal_segment}}</b> compared to the <b>Training</b> data. <br /><br /> Prediction drift indicates a significant change in model's behavior. In some cases, it is a strong indicator for concept drift.<br /><br /> Prediction drift might occur because: <ul><li>Natural changes in data</li><li>Data store / provider schema changes</li><li>Data store / provider issues</li><li>Data processing issues</li></ul>",
             needed_args=[["thresholds", "max"], "baseline"],
         ),
     },
     MonitorType.MISSING_VALUES: {
         DetectionMethod.ANOMALY: _MonitorParamBuilder(
             metric_builder=lambda **kw: MetricConfiguration(type=MetricType.MISSING_RATIO),
             alert_type=AlertType.FEATURE_MISSING_VALUES_ANOMALY,
             visualization_builder=lambda **kw: VisualizationType.RANGE_LINE_CHART,
             description_builder=lambda **kw: "An anomaly was detected in the ratio of missing values of feature <b>'{field}'</b> {importance}.<br /> The anomaly was observed in the <b>{model}</b> model, in version <b>{model_version}</b> for the <b>last {focal_time_period} ({focal_times})</b> <b>{focal_segment}</b>. <br /><br /> Based on missing ratio history, the ratio was expected to be between <b>{last_lower_bound}</b> to <b>{last_upper_bound}</b>, but <b>{focal_value}</b> was received. <br /><br /> Missing data can have a significant effect on model behavior and may lead to unexpected results. <br /><br /> Missing data might occur because: <ul><li>Serving environment fault</li><li>Data store / provider schema changes</li><li>Changes in internal API</li><li>Changes in model subject input</li></ul>",
             logic_evaluation_builder=lambda **kw: LogicEvaluationConfiguration(
-                name=LogicEvaluationType.TIME_SERIES_ANOMALY, sensitivity=kw["sensitivity"]
+                name=LogicEvaluationType.TIME_SERIES_ANOMALY,
+                sensitivity=kw["sensitivity"],
+                testOnlyIncrease=kw["testOnlyIncrease"],
             ),
             precondition_builder=lambda **kw: (
                 PreConditionConfiguration(
                     name=PreConditionType.FOCAL_DATA_VALUE_IN_RANGE, min=kw["min"]
                 )
                 if kw["min"] is not None
                 else None
@@ -1097,15 +1109,17 @@
             description_builder=lambda **kw: (
                 "An anomaly in the value of the <b>'{metric}'</b> "
                 + __get_alert_field_description_if_needed(MetricType(kw["metric"]))
                 + "was detected. <br /> The anomaly was observed in the <b>{model}</b> model, in version <b>{model_version}</b> for the <b>last {focal_time_period} ({focal_times})</b> <b>{focal_segment}</b>. <br /><br /> Based on metric history, the ratio was expected to be "
                 + "between <b>{last_lower_bound}</b> to <b>{last_upper_bound}</b>, but <b>{focal_value}</b> was received."
             ),
             logic_evaluation_builder=lambda **kw: LogicEvaluationConfiguration(
-                name=LogicEvaluationType.TIME_SERIES_ANOMALY, sensitivity=kw["sensitivity"]
+                name=LogicEvaluationType.TIME_SERIES_ANOMALY,
+                sensitivity=kw["sensitivity"],
+                testOnlyIncrease=kw["testOnlyIncrease"],
             ),
             needed_args=["metric", "sensitivity", "baseline"],
         ),
         DetectionMethod.PERCENTAGE: _MonitorParamBuilder(
             visualization_builder=lambda **kw: VisualizationType.VALUE_OVER_TIME,
             alert_type=AlertType.METRIC_CHANGE,
             metric_builder=lambda **kw: MetricConfiguration(
@@ -1222,15 +1236,17 @@
             description_builder=lambda **kw: (
                 "An anomaly in the value of the <b>'{metric}'</b> "
                 + __get_alert_field_description_if_needed(MetricType(kw["metric"]))
                 + "was detected. <br /> The anomaly was observed in the <b>{model}</b> model, in version <b>{model_version}</b> for the <b>last {focal_time_period} ({focal_times})</b> <b>{focal_segment}</b>. <br /><br /> Based on metric history, the ratio was expected to be "
                 + "between <b>{last_lower_bound}</b> to <b>{last_upper_bound}</b>, but <b>{focal_value}</b> was received."
             ),
             logic_evaluation_builder=lambda **kw: LogicEvaluationConfiguration(
-                name=LogicEvaluationType.TIME_SERIES_ANOMALY, sensitivity=kw["sensitivity"]
+                name=LogicEvaluationType.TIME_SERIES_ANOMALY,
+                sensitivity=kw["sensitivity"],
+                testOnlyIncrease=kw["testOnlyIncrease"],
             ),
             needed_args=["metric", "baseline", "sensitivity"],
         ),
         DetectionMethod.PERCENTAGE: _MonitorParamBuilder(
             visualization_builder=lambda **kw: VisualizationType.VALUE_OVER_TIME,
             alert_type=AlertType.METRIC_CHANGE,
             metric_builder=lambda **kw: MetricConfiguration(
@@ -1352,15 +1368,17 @@
             description_builder=lambda **kw: (
                 "An anomaly in the value of the <b>'{metric}'</b> "
                 + __get_alert_field_description_if_needed(MetricType.CUSTOM_METRIC)
                 + "was detected. <br /> The anomaly was observed in the <b>{model}</b> model, in version <b>{model_version}</b> for the <b>last {focal_time_period} ({focal_times})</b> <b>{focal_segment}</b>. <br /><br /> Based on metric history, the ratio was expected to be "
                 + "between <b>{last_lower_bound}</b> to <b>{last_upper_bound}</b>, but <b>{focal_value}</b> was received."
             ),
             logic_evaluation_builder=lambda **kw: LogicEvaluationConfiguration(
-                name=LogicEvaluationType.TIME_SERIES_ANOMALY, sensitivity=kw["sensitivity"]
+                name=LogicEvaluationType.TIME_SERIES_ANOMALY,
+                sensitivity=kw["sensitivity"],
+                testOnlyIncrease=kw["testOnlyIncrease"],
             ),
             needed_args=["custom_metric_id", "baseline", "sensitivity"],
         ),
         DetectionMethod.PERCENTAGE: _MonitorParamBuilder(
             visualization_builder=lambda **kw: VisualizationType.VALUE_OVER_TIME,
             alert_type=AlertType.METRIC_CHANGE,
             metric_builder=lambda **kw: MetricConfiguration(
@@ -1491,21 +1509,23 @@
     features: Optional[List[str]] = None,
     predictions: Optional[List[str]] = None,
     is_embedding_monitor: bool = False,
     metric: Optional[Union[MetricType, str]] = None,
     percentage: Optional[int] = None,
     thresholds: Optional[ThresholdConfiguration] = None,
     sensitivity: Optional[float] = None,
+    alert_on_increase_only: Optional[bool] = None,
     min: Optional[int] = None,
     max: Optional[int] = None,
     distance: Optional[float] = None,
     new_values_ratio_threshold: Optional[float] = None,
     new_values_count_threshold: Optional[int] = None,
     staleness_period: Optional[TimePeriod] = None,
-    min_prediction_count: Optional[int] = None,
+    min_focal_prediction_count: Optional[int] = None,
+    min_baseline_prediction_count: Optional[int] = None,
     version: Optional[str] = None,
     segment_identification: Optional[SegmentIdentification] = None,
     messaging: Optional[Dict[MessagingIntegrationType, List[str]]] = None,
     emails: Optional[List[str]] = None,
     max_alerts_per_day: Optional[int] = None,
     k: Optional[int] = None,
     prediction_class: Optional[Any] = None,
@@ -1519,31 +1539,34 @@
 
     monitor_type = MonitorType(monitor_type)
     detection_method = DetectionMethod(detection_method)
     severity = Severity(severity)
 
     preconditions = []
 
-    if min_prediction_count is not None:
-        if baseline is not None:
-            preconditions.append(
-                PreConditionConfiguration(
-                    name=PreConditionType.MIN_BASELINE_DATA_POINTS, value=min_prediction_count
-                )
+    if min_baseline_prediction_count is not None:
+        if baseline is None:
+            raise ValueError("Can't specify min_baseline_prediction_count for monitors with no baseline")
+        preconditions.append(
+            PreConditionConfiguration(
+                name=PreConditionType.MIN_BASELINE_DATA_POINTS, value=min_baseline_prediction_count
             )
+        )
+    if min_focal_prediction_count is not None:
         preconditions.append(
             PreConditionConfiguration(
-                name=PreConditionType.MIN_FOCAL_DATA_POINTS, value=min_prediction_count
+                name=PreConditionType.MIN_FOCAL_DATA_POINTS, value=min_focal_prediction_count
             )
         )
 
     monitor_params = _MONITOR_PARAMETERS[monitor_type][detection_method](
         percentage=percentage,
         thresholds=thresholds,
         sensitivity=sensitivity,
+        testOnlyIncrease=alert_on_increase_only,
         min=min,
         max=max,
         new_values_count_threshold=new_values_count_threshold,
         new_values_ratio_threshold=new_values_ratio_threshold,
         distance=distance,
         staleness_period=staleness_period,
         baseline=baseline,
```

### Comparing `aporia-3.1.0/src/aporia/sdk/segments.py` & `aporia-3.2.0/src/aporia/sdk/segments.py`

 * *Files identical despite different names*

### Comparing `aporia-3.1.0/src/aporia/sdk/versions.py` & `aporia-3.2.0/src/aporia/sdk/versions.py`

 * *Files identical despite different names*

### Comparing `aporia-3.1.0/PKG-INFO` & `aporia-3.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aporia
-Version: 3.1.0
+Version: 3.2.0
 Summary: 
 Author: Aporia
 Author-email: support@aporia.com
 Requires-Python: >=3.8,<=3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

