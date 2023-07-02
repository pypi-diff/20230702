# Comparing `tmp/threemystic_cmdb-0.1.2.tar.gz` & `tmp/threemystic_cmdb-0.1.3.tar.gz`

## Comparing `threemystic_cmdb-0.1.2.tar` & `threemystic_cmdb-0.1.3.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.2/threemystic_cloud_cmdb/__main__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.2/threemystic_cloud_cmdb/__version__.py
--rw-r--r--   0        0        0     3560 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.2/threemystic_cloud_cmdb/cloud_cmdb_client.py
--rw-r--r--   0        0        0     4484 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.2/threemystic_cloud_cmdb/cli/__init__.py
--rw-r--r--   0        0        0     2910 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.2/threemystic_cloud_cmdb/cli/actions/base_class/base.py
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.2/threemystic_cloud_cmdb/cli/actions/config/__init__.py
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.2/threemystic_cloud_cmdb/cloud_providers/aws/__init__.py
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.2/threemystic_cloud_cmdb/cloud_providers/aws/base_class/base.py
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.2/threemystic_cloud_cmdb/cloud_providers/aws/client/__init__.py
--rw-r--r--   0        0        0     3018 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.2/threemystic_cloud_cmdb/cloud_providers/aws/config/step_1.py
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.2/threemystic_cloud_cmdb/cloud_providers/aws/config/base_class/base.py
--rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.2/threemystic_cloud_cmdb/cloud_providers/azure/__init__.py
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.2/threemystic_cloud_cmdb/cloud_providers/azure/base_class/base.py
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.2/threemystic_cloud_cmdb/cloud_providers/azure/client/__init__.py
--rw-r--r--   0        0        0     2387 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.2/threemystic_cloud_cmdb/cloud_providers/azure/client/actions/budget.py
--rw-r--r--   0        0        0     2674 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.2/threemystic_cloud_cmdb/cloud_providers/azure/client/actions/cloudstorage.py
--rw-r--r--   0        0        0     2666 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.2/threemystic_cloud_cmdb/cloud_providers/azure/client/actions/storage.py
--rw-r--r--   0        0        0    20906 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.2/threemystic_cloud_cmdb/cloud_providers/azure/client/actions/vm.py
--rw-r--r--   0        0        0     5201 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.2/threemystic_cloud_cmdb/cloud_providers/azure/client/actions/base_class/base.py
--rw-r--r--   0        0        0     3023 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.2/threemystic_cloud_cmdb/cloud_providers/azure/config/step_1.py
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.2/threemystic_cloud_cmdb/cloud_providers/azure/config/base_class/base.py
--rw-r--r--   0        0        0     4597 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.2/threemystic_cloud_cmdb/cloud_providers/base_class/base.py
--rw-r--r--   0        0        0     7789 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.2/threemystic_cloud_cmdb/cloud_providers/base_class/base_client.py
--rw-r--r--   0        0        0    19280 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.2/threemystic_cloud_cmdb/cloud_providers/base_class/base_cmdb.py
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.2/threemystic_cloud_cmdb/cloud_providers/general/__init__.py
--rw-r--r--   0        0        0     1006 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.2/threemystic_cloud_cmdb/cloud_providers/general/cmdb_connector/auto_cmdb_connector.py
--rw-r--r--   0        0        0    30792 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.2/threemystic_cloud_cmdb/cloud_providers/general/cmdb_connector/ms365.py
--rw-r--r--   0        0        0    13128 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.2/threemystic_cloud_cmdb/cloud_providers/general/cmdb_connector/base_class/base.py
--rw-r--r--   0        0        0     2888 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.2/threemystic_cloud_cmdb/cloud_providers/general/config/step_1.py
--rw-r--r--   0        0        0     5774 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.2/threemystic_cloud_cmdb/cloud_providers/general/config/step_2.py
--rw-r--r--   0        0        0    18353 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.2/threemystic_cloud_cmdb/cloud_providers/general/config/step_2_cloud_share.py
--rw-r--r--   0        0        0     5751 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.2/threemystic_cloud_cmdb/cloud_providers/general/config/step_3.py
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.2/threemystic_cloud_cmdb/cloud_providers/general/config/base_class/base.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.2/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.2/LICENSE
--rw-r--r--   0        0        0     1300 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.2/README.md
--rw-r--r--   0        0        0     3176 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2602 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.3/threemystic_cloud_cmdb/__main__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.3/threemystic_cloud_cmdb/__version__.py
+-rw-r--r--   0        0        0     3560 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.3/threemystic_cloud_cmdb/cloud_cmdb_client.py
+-rw-r--r--   0        0        0     4484 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.3/threemystic_cloud_cmdb/cli/__init__.py
+-rw-r--r--   0        0        0     2910 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.3/threemystic_cloud_cmdb/cli/actions/base_class/base.py
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.3/threemystic_cloud_cmdb/cli/actions/config/__init__.py
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.3/threemystic_cloud_cmdb/cloud_providers/aws/__init__.py
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.3/threemystic_cloud_cmdb/cloud_providers/aws/base_class/base.py
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.3/threemystic_cloud_cmdb/cloud_providers/aws/client/__init__.py
+-rw-r--r--   0        0        0     3018 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.3/threemystic_cloud_cmdb/cloud_providers/aws/config/step_1.py
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.3/threemystic_cloud_cmdb/cloud_providers/aws/config/base_class/base.py
+-rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.3/threemystic_cloud_cmdb/cloud_providers/azure/__init__.py
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.3/threemystic_cloud_cmdb/cloud_providers/azure/base_class/base.py
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.3/threemystic_cloud_cmdb/cloud_providers/azure/client/__init__.py
+-rw-r--r--   0        0        0     2663 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.3/threemystic_cloud_cmdb/cloud_providers/azure/client/actions/budget.py
+-rw-r--r--   0        0        0     2674 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.3/threemystic_cloud_cmdb/cloud_providers/azure/client/actions/cloudstorage.py
+-rw-r--r--   0        0        0     3309 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.3/threemystic_cloud_cmdb/cloud_providers/azure/client/actions/storage.py
+-rw-r--r--   0        0        0    21346 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.3/threemystic_cloud_cmdb/cloud_providers/azure/client/actions/vm.py
+-rw-r--r--   0        0        0     5201 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.3/threemystic_cloud_cmdb/cloud_providers/azure/client/actions/base_class/base.py
+-rw-r--r--   0        0        0     3023 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.3/threemystic_cloud_cmdb/cloud_providers/azure/config/step_1.py
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.3/threemystic_cloud_cmdb/cloud_providers/azure/config/base_class/base.py
+-rw-r--r--   0        0        0     4597 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.3/threemystic_cloud_cmdb/cloud_providers/base_class/base.py
+-rw-r--r--   0        0        0     7789 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.3/threemystic_cloud_cmdb/cloud_providers/base_class/base_client.py
+-rw-r--r--   0        0        0    20199 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.3/threemystic_cloud_cmdb/cloud_providers/base_class/base_cmdb.py
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.3/threemystic_cloud_cmdb/cloud_providers/general/__init__.py
+-rw-r--r--   0        0        0     1006 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.3/threemystic_cloud_cmdb/cloud_providers/general/cmdb_connector/auto_cmdb_connector.py
+-rw-r--r--   0        0        0    30767 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.3/threemystic_cloud_cmdb/cloud_providers/general/cmdb_connector/ms365.py
+-rw-r--r--   0        0        0    13381 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.3/threemystic_cloud_cmdb/cloud_providers/general/cmdb_connector/base_class/base.py
+-rw-r--r--   0        0        0     2888 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.3/threemystic_cloud_cmdb/cloud_providers/general/config/step_1.py
+-rw-r--r--   0        0        0     5774 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.3/threemystic_cloud_cmdb/cloud_providers/general/config/step_2.py
+-rw-r--r--   0        0        0    18353 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.3/threemystic_cloud_cmdb/cloud_providers/general/config/step_2_cloud_share.py
+-rw-r--r--   0        0        0     5751 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.3/threemystic_cloud_cmdb/cloud_providers/general/config/step_3.py
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.3/threemystic_cloud_cmdb/cloud_providers/general/config/base_class/base.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.3/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.3/LICENSE
+-rw-r--r--   0        0        0     1300 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.3/README.md
+-rw-r--r--   0        0        0     3137 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2555 2020-02-02 00:00:00.000000 threemystic_cmdb-0.1.3/PKG-INFO
```

### Comparing `threemystic_cmdb-0.1.2/threemystic_cloud_cmdb/cloud_cmdb_client.py` & `threemystic_cmdb-0.1.3/threemystic_cloud_cmdb/cloud_cmdb_client.py`

 * *Files identical despite different names*

### Comparing `threemystic_cmdb-0.1.2/threemystic_cloud_cmdb/cli/__init__.py` & `threemystic_cmdb-0.1.3/threemystic_cloud_cmdb/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cmdb-0.1.2/threemystic_cloud_cmdb/cli/actions/base_class/base.py` & `threemystic_cmdb-0.1.3/threemystic_cloud_cmdb/cli/actions/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cmdb-0.1.2/threemystic_cloud_cmdb/cli/actions/config/__init__.py` & `threemystic_cmdb-0.1.3/threemystic_cloud_cmdb/cli/actions/config/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cmdb-0.1.2/threemystic_cloud_cmdb/cloud_providers/aws/__init__.py` & `threemystic_cmdb-0.1.3/threemystic_cloud_cmdb/cloud_providers/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cmdb-0.1.2/threemystic_cloud_cmdb/cloud_providers/aws/config/step_1.py` & `threemystic_cmdb-0.1.3/threemystic_cloud_cmdb/cloud_providers/aws/config/step_1.py`

 * *Files identical despite different names*

### Comparing `threemystic_cmdb-0.1.2/threemystic_cloud_cmdb/cloud_providers/azure/__init__.py` & `threemystic_cmdb-0.1.3/threemystic_cloud_cmdb/cloud_providers/azure/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cmdb-0.1.2/threemystic_cloud_cmdb/cloud_providers/azure/client/actions/budget.py` & `threemystic_cmdb-0.1.3/threemystic_cloud_cmdb/cloud_providers/azure/client/actions/budget.py`

 * *Files 13% similar despite different names*

```diff
@@ -33,14 +33,21 @@
   
   def _load_cmdb_column_data(self, *args, **kwargs):
     if hasattr(self, "_cmdb_column_data_loaded"):
       return self._cmdb_column_data_loaded
     
     self._cmdb_column_data_loaded = {
       self.get_cmdb_data_action(): {
+        "last_run":{
+          "display": "LastRun",
+          "handler": lambda item: self.get_common().helper_type().datetime().remove_tzinfo(dt= self.get_data_start()),
+          "cmdb": {
+              "handler": lambda item: self.get_data_start(),
+          }
+        },
         "last_seven_days":{
           "display": "Last7Days",
           "handler": lambda item: self.get_item_data_value(item_data= item, value_key="last_seven_days")
         },
         "month_to_date":{
           "display": "MonthToDate",
           "handler": lambda item: self.get_item_data_value(item_data= item, value_key="month_to_date")
```

### Comparing `threemystic_cmdb-0.1.2/threemystic_cloud_cmdb/cloud_providers/azure/client/actions/cloudstorage.py` & `threemystic_cmdb-0.1.3/threemystic_cloud_cmdb/cloud_providers/azure/client/actions/cloudstorage.py`

 * *Files identical despite different names*

### Comparing `threemystic_cmdb-0.1.2/threemystic_cloud_cmdb/cloud_providers/azure/client/actions/storage.py` & `threemystic_cmdb-0.1.3/threemystic_cloud_cmdb/cloud_providers/azure/client/actions/storage.py`

 * *Files 8% similar despite different names*

```diff
@@ -36,19 +36,25 @@
         },
         "Name":{
           "display": "Name",
           "handler": lambda item: self.get_item_data_value(item_data= item, value_key=["name"])
         },
         "Size":{
           "display": "Size_Gib",
-          "handler": lambda item: self.get_item_data_value(item_data= item, value_key=["diskSizeGB"])
+          "handler": lambda item: (self.get_item_data_value(item_data= item, value_key=["diskSizeGB"])
+                                   if not self.get_common().helper_type().string().is_null_or_whitespace(string_value= self.get_item_data_value(item_data= item, value_key=["diskSizeGB"])) else
+                                   self.get_item_data_value(item_data= item, value_key=["properties", "diskSizeGB"])
+          )
         },
         "Attached":{
           "display": "Attached",
-          "handler": lambda item:  self.get_item_data_value(item_data= item, value_key=["diskState"])
+          "handler": lambda item: (self.get_item_data_value(item_data= item, value_key=["diskState"])
+                                   if not self.get_common().helper_type().string().is_null_or_whitespace(string_value= self.get_item_data_value(item_data= item, value_key=["diskState"])) else
+                                   self.get_item_data_value(item_data= item, value_key=["properties", "diskState"])
+          )
         },
         "GroupType":{
           "display": "GroupType",
           "handler": lambda item: None # item["Storage"].get("group_type") if item["Storage"] is not None and item["Storage"].get("group_type") else None
         },
         "Group":{
           "display": "Group",
```

### Comparing `threemystic_cmdb-0.1.2/threemystic_cloud_cmdb/cloud_providers/azure/client/actions/vm.py` & `threemystic_cmdb-0.1.3/threemystic_cloud_cmdb/cloud_providers/azure/client/actions/vm.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,15 +66,18 @@
         },
         "InstanceType": {
           "display": "Instance Type",
           "handler": lambda item: self.get_item_data_value(item_data= item, value_key=["sku", "name"])
         },
         "AMIID": {
           "display": "AMI ID",
-          "handler": lambda item: self.get_common().helper_type().string().join(separator= ".", str_array= [self.get_item_data_value(item_data= item, value_key=["properties", "virtualMachineProfile", "storageProfile","imageReference","publisher"]), self.get_item_data_value(item_data= item, value_key=["properties", "virtualMachineProfile", "storageProfile","imageReference","sku"])]) 
+          "handler": lambda item: (self.get_item_data_value(item_data= item, value_key=["properties", "virtualMachineProfile", "storageProfile","imageReference","id"]) 
+                                   if not self.get_common().helper_type().string().is_null_or_whitespace(string_value= self.get_item_data_value(item_data= item, value_key=["properties", "virtualMachineProfile", "storageProfile","imageReference","id"])) else 
+                                   self.get_common().helper_type().string().join(separator= ".", str_array= [self.get_item_data_value(item_data= item, value_key=["properties", "virtualMachineProfile", "storageProfile","imageReference","publisher"]), self.get_item_data_value(item_data= item, value_key=["properties", "virtualMachineProfile", "storageProfile","imageReference","sku"])])
+          )
         },
         "AMIName": {
           "display": "AMI Name",
           "handler": lambda item: self.get_common().helper_type().string().join(separator= ".", str_array= [self.get_item_data_value(item_data= item, value_key=["properties", "virtualMachineProfile", "storageProfile","imageReference","publisher"]), self.get_item_data_value(item_data= item, value_key=["properties", "virtualMachineProfile", "storageProfile","imageReference","sku"]), self.get_item_data_value(item_data= item, value_key=["properties", "virtualMachineProfile", "storageProfile","imageReference","version"])])  
         },
         "AMIDescription": {
           "display": "AMI Description",
```

### Comparing `threemystic_cmdb-0.1.2/threemystic_cloud_cmdb/cloud_providers/azure/client/actions/base_class/base.py` & `threemystic_cmdb-0.1.3/threemystic_cloud_cmdb/cloud_providers/azure/client/actions/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cmdb-0.1.2/threemystic_cloud_cmdb/cloud_providers/azure/config/step_1.py` & `threemystic_cmdb-0.1.3/threemystic_cloud_cmdb/cloud_providers/azure/config/step_1.py`

 * *Files identical despite different names*

### Comparing `threemystic_cmdb-0.1.2/threemystic_cloud_cmdb/cloud_providers/base_class/base.py` & `threemystic_cmdb-0.1.3/threemystic_cloud_cmdb/cloud_providers/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cmdb-0.1.2/threemystic_cloud_cmdb/cloud_providers/base_class/base_client.py` & `threemystic_cmdb-0.1.3/threemystic_cloud_cmdb/cloud_providers/base_class/base_client.py`

 * *Files identical despite different names*

### Comparing `threemystic_cmdb-0.1.2/threemystic_cloud_cmdb/cloud_providers/base_class/base_cmdb.py` & `threemystic_cmdb-0.1.3/threemystic_cloud_cmdb/cloud_providers/base_class/base_cmdb.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from threemystic_common.base_class.base_provider import base
 import asyncio, concurrent.futures
 from abc import abstractmethod
+from openpyxl import Workbook,worksheet
 
 class cloud_cmdb_provider_base_cmdb(base):
   def __init__(self, *args, **kwargs):
     super().__init__(*args, **kwargs)
     
     self._set_max_process_pool(*args, **kwargs)
     self._set_max_thread_pool(*args, **kwargs)
@@ -68,26 +69,39 @@
     return [
       column.get("display") for column in self._get_default_columns_raw(*args, **kwargs) if column.get("hidden") != True
     ]
 
   def get_item_data_value(self, item_data, value_key, *args, **kwargs):
     return self.get_common().helper_type().general().get_container_value(container= item_data, value_key= value_key)
   
-  async def save_report(self, *args, **kwargs):
+  def save_excel_report_path(self, *args, **kwargs):
+    if hasattr(self, "_excel_report_path_save" ):
+      return self._excel_report_path_save
+
     report_name = f'{self.get_client_name()}-{self.get_common().helper_type().datetime().datetime_as_string(dt= self.get_data_start(), dt_format= "%Y%m%d")}.xlsx'
-    report_path = self.get_cloud_cmdb().get_cmdb_report_path().joinpath(f'{self._get_cloud_cmdb_raw().get_provider()}/{report_name}')
-    if not report_path.parent.exists():
-      report_path.parent.mkdir(parents= True)
+    self._excel_report_path_save = self.get_cloud_cmdb().get_cmdb_report_path().joinpath(f'{self._get_cloud_cmdb_raw().get_provider()}/{report_name}')
+    if not self._excel_report_path_save.parent.exists():
+      self._excel_report_path_save.parent.mkdir(parents= True)
+    
+    return self.save_excel_report_path()
+  
+  async def save_excel_report_only(self, close_connection = False, *args, **kwargs):
+    self._get_excel().save(self._excel_report_path_save)
+    
+    if close_connection is True:
+      self._excel_close()
+
+  async def save_report(self, *args, **kwargs):
+    
     
     if len(self._get_excel().sheetnames) < 1:
       print(f'No Report Saved - No Data')
       return  
-    print(f'Report saved at: {report_path}')
-    self._get_excel().save(report_path)
-    self._excel_close()
+    print(f'Report saved at: {self.save_excel_report_path()}')
+    await self.save_excel_report_only(close_connection= True)
     
   
   async def save_report_cmdb(self, *args, **kwargs):    
     if not self.get_cloud_cmdb().has_cloud_share_configured():
       return None
     
     print(f'Saving report in Shared CMDB')
@@ -158,50 +172,61 @@
     await self._process_report_data(
       data= {
         sheet_key: await data.main(pool= pool, loop= loop) for sheet_key, data in self._get_data_action_by_key().items()
       }
     )
 
   async def _process_report_data(self, data, *args, **kwargs):
-    report_data = {}
+    
+    save_task = None
     for sheet_key, main_report_data in data.items():
       for _, report_data in main_report_data.items():
         if report_data is None:
           continue
         
-        for report_data_item in report_data:
+        while len(report_data) > 0:
+          report_data_item=report_data.pop(0)
           self.get_excel_workbook(sheet_key= sheet_key).append(
             self.get_report_default_row(
               sheet_key= sheet_key,
               account= report_data_item.get("extra_account"), 
               resource= report_data_item,  
               region= report_data_item.get("extra_region"), 
               resource_groups = report_data_item.get("extra_resourcegroups"),
               is_cmdb= False
               ) +
             [self.get_handler_column_data(column_data= column_data, is_cmdb= False)(report_data_item) for _, column_data in self.get_workbook_columns()[sheet_key].items()] +
             self.generate_tag_columns(
-              account=report_data_item.get("extra_account"), 
+              account=report_data_item.get("extra_account"),
               resource= report_data_item,
               is_cmdb= False)
           )
           self.save_cmdb_workbook_item(sheet_key= sheet_key, account= report_data_item.get("extra_account"), report_data_item= report_data_item)
+          
+          report_data_len = len(report_data)
+          if ( report_data_len % 1000) == 0 and report_data_len > 0:
+            if save_task is not None:
+              await asyncio.wait([save_task])
+
+            save_task = asyncio.get_event_loop().create_task(self.save_excel_report_only(close_connection= False))
+    
+    if save_task is not None:
+      await asyncio.wait([save_task])
 
   def _excel_close(self, *args, **kwargs):    
     self._get_excel().close()
     self.get_excel_workbook(unset= True)
     self._get_excel(unset= True)
 
   def _get_excel(self, unset = False, *args, **kwargs):    
     if hasattr(self, "_workbook_excel_main"):
       if unset:
         return delattr(self, "_workbook_excel_main")
       return self._workbook_excel_main
     
-    from openpyxl import Workbook
     self._workbook_excel_main = Workbook(write_only=True)
     
     while len(self._workbook_excel_main.sheetnames) > 0:
       self._workbook_excel_main.remove(self._workbook_excel_main[self._workbook_excel_main.sheetnames[0]])
     return self._get_excel()
 
   def get_cmdb_workbook(self, sheet_key= None, *args, **kwargs):
```

### Comparing `threemystic_cmdb-0.1.2/threemystic_cloud_cmdb/cloud_providers/general/__init__.py` & `threemystic_cmdb-0.1.3/threemystic_cloud_cmdb/cloud_providers/general/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cmdb-0.1.2/threemystic_cloud_cmdb/cloud_providers/general/cmdb_connector/auto_cmdb_connector.py` & `threemystic_cmdb-0.1.3/threemystic_cloud_cmdb/cloud_providers/general/cmdb_connector/auto_cmdb_connector.py`

 * *Files identical despite different names*

### Comparing `threemystic_cmdb-0.1.2/threemystic_cloud_cmdb/cloud_providers/general/cmdb_connector/ms365.py` & `threemystic_cmdb-0.1.3/threemystic_cloud_cmdb/cloud_providers/general/cmdb_connector/ms365.py`

 * *Files 0% similar despite different names*

```diff
@@ -563,15 +563,15 @@
         delete_index = self.get_existing_columns_sorted_by_index()[sheet_key].index(self.get_cmdb_data_containers_columns_raw_byid_display()[sheet_key]["deleted"])
         while len(existing_data) > 0:
           _, deleted_data = existing_data.popitem()
           
           if not self.get_common().helper_type().string().is_null_or_whitespace(string_value= deleted_data.get("values")[0][delete_index]):
             continue
 
-          deleted_data.get("values")[0][delete_index] = self.get_common().helper_type().datetime().get()
+          deleted_data.get("values")[0][delete_index] = self._get_delete_time()
           update_data.append(deleted_data)
       
       self.__sync_data_update_data(sheet_key= sheet_key, update_data= update_data)
       self.__sync_data_add_data(sheet_key= sheet_key, insert_data= insert_data)
 
   def __sync_data_update_data_process(self, sheet_key, update_data, *args, **kwargs):
```

### Comparing `threemystic_cmdb-0.1.2/threemystic_cloud_cmdb/cloud_providers/general/cmdb_connector/base_class/base.py` & `threemystic_cmdb-0.1.3/threemystic_cloud_cmdb/cloud_providers/general/cmdb_connector/base_class/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,20 @@
   def _validate_cmdb_init(self, *args, **kwargs):
     pass
 
   @abstractmethod
   def _sync_data(self, *args, **kwargs):
     pass
   
+  def _get_delete_time(self, *args, **kwargs):
+    if hasattr(self, "_general_delete_time"):
+      return self._general_delete_time
+    
+    self._general_delete_time = self.get_common().helper_type().datetime().get()
+    return self._get_delete_time()
   def _get_number_of_groups_batchsize(self, total_items,  batch_size = 500, *args, **kwargs):
     groups = total_items / Decimal(batch_size)
     return int(floor(groups)) + 1
 
   def _get_cmdb_default_column_settings(self, *args, **kwargs):    
     if hasattr(self, "_cmdb_default_column_settings"):
       return self._cmdb_default_column_settings
```

### Comparing `threemystic_cmdb-0.1.2/threemystic_cloud_cmdb/cloud_providers/general/config/step_1.py` & `threemystic_cmdb-0.1.3/threemystic_cloud_cmdb/cloud_providers/general/config/step_1.py`

 * *Files identical despite different names*

### Comparing `threemystic_cmdb-0.1.2/threemystic_cloud_cmdb/cloud_providers/general/config/step_2.py` & `threemystic_cmdb-0.1.3/threemystic_cloud_cmdb/cloud_providers/general/config/step_2.py`

 * *Files identical despite different names*

### Comparing `threemystic_cmdb-0.1.2/threemystic_cloud_cmdb/cloud_providers/general/config/step_2_cloud_share.py` & `threemystic_cmdb-0.1.3/threemystic_cloud_cmdb/cloud_providers/general/config/step_2_cloud_share.py`

 * *Files identical despite different names*

### Comparing `threemystic_cmdb-0.1.2/threemystic_cloud_cmdb/cloud_providers/general/config/step_3.py` & `threemystic_cmdb-0.1.3/threemystic_cloud_cmdb/cloud_providers/general/config/step_3.py`

 * *Files identical despite different names*

### Comparing `threemystic_cmdb-0.1.2/.gitignore` & `threemystic_cmdb-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `threemystic_cmdb-0.1.2/LICENSE` & `threemystic_cmdb-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `threemystic_cmdb-0.1.2/README.md` & `threemystic_cmdb-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `threemystic_cmdb-0.1.2/pyproject.toml` & `threemystic_cmdb-0.1.3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -23,17 +23,16 @@
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
   "colorama; platform_system == 'Windows'",
-  "threemystic-common >= 0.1.1",
-  "threemystic-cloud-client >= 0.1.2",
-  "threemystic-cloud-data-client >= 0.1.2",
+  "threemystic-common >= 0.1.2",
+  "threemystic-cloud-data-client >= 0.1.3",
   "typing-extensions >= 4.4.0",
   "asyncio >= 3.4.3",
   "tqdm >= 4.65.0",
   "openpyxl >= 3.1.2",
   "msgraph-sdk >= 1.0.0a12",
   "lxml >= 4.9.2"
```

### Comparing `threemystic_cmdb-0.1.2/PKG-INFO` & `threemystic_cmdb-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: threemystic-cmdb
-Version: 0.1.2
+Version: 0.1.3
 Summary: A lightweight CMDB to help you track your cloud resources from various providers
 Project-URL: Homepage, https://github.com/3MysticApes/3mystic_cloud_cmdb
 Project-URL: Bug Tracker, https://github.com/3MysticApes/3mystic_cloud_cmdb/issues
 Author: Ron Truex
 License-Expression: MIT
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
@@ -18,17 +18,16 @@
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.8
 Requires-Dist: asyncio>=3.4.3
 Requires-Dist: colorama; platform_system == 'Windows'
 Requires-Dist: lxml>=4.9.2
 Requires-Dist: msgraph-sdk>=1.0.0a12
 Requires-Dist: openpyxl>=3.1.2
-Requires-Dist: threemystic-cloud-client>=0.1.2
-Requires-Dist: threemystic-cloud-data-client>=0.1.2
-Requires-Dist: threemystic-common>=0.1.1
+Requires-Dist: threemystic-cloud-data-client>=0.1.3
+Requires-Dist: threemystic-common>=0.1.2
 Requires-Dist: tqdm>=4.65.0
 Requires-Dist: typing-extensions>=4.4.0
 Description-Content-Type: text/markdown
 
 # 3mystic_cmdb
 A Lightweight Multi Cloud CMDB (Configuration management database)
 Currently supports AWS/Azure
```

