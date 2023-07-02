# Comparing `tmp/threemystic_cloud_data_client-0.1.2.tar.gz` & `tmp/threemystic_cloud_data_client-0.1.3.tar.gz`

## Comparing `threemystic_cloud_data_client-0.1.2.tar` & `threemystic_cloud_data_client-0.1.3.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.2/threemystic_cloud_data_client/__main__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.2/threemystic_cloud_data_client/__version__.py
--rw-r--r--   0        0        0     3895 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.2/threemystic_cloud_data_client/cloud_data_client.py
--rw-r--r--   0        0        0     4150 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.2/threemystic_cloud_data_client/cli/__init__.py
--rw-r--r--   0        0        0     2950 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.2/threemystic_cloud_data_client/cli/actions/base_class/base.py
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.2/threemystic_cloud_data_client/cli/actions/config/__init__.py
--rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.2/threemystic_cloud_data_client/cloud_providers/aws/__init__.py
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.2/threemystic_cloud_data_client/cloud_providers/aws/base_class/base.py
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.2/threemystic_cloud_data_client/cloud_providers/aws/client/__init__.py
--rw-r--r--   0        0        0     3028 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.2/threemystic_cloud_data_client/cloud_providers/aws/config/step_1.py
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.2/threemystic_cloud_data_client/cloud_providers/aws/config/base_class/base.py
--rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.2/threemystic_cloud_data_client/cloud_providers/azure/__init__.py
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.2/threemystic_cloud_data_client/cloud_providers/azure/base_class/base.py
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.2/threemystic_cloud_data_client/cloud_providers/azure/client/__init__.py
--rw-r--r--   0        0        0    13738 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.2/threemystic_cloud_data_client/cloud_providers/azure/client/actions/budget.py
--rw-r--r--   0        0        0     3449 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.2/threemystic_cloud_data_client/cloud_providers/azure/client/actions/cloudstorage.py
--rw-r--r--   0        0        0    12999 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.2/threemystic_cloud_data_client/cloud_providers/azure/client/actions/storage.py
--rw-r--r--   0        0        0    11884 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.2/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vm.py
--rw-r--r--   0        0        0     3174 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.2/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vmss.py
--rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.2/threemystic_cloud_data_client/cloud_providers/azure/client/actions/base_class/base.py
--rw-r--r--   0        0        0     3046 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.2/threemystic_cloud_data_client/cloud_providers/azure/config/step_1.py
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.2/threemystic_cloud_data_client/cloud_providers/azure/config/base_class/base.py
--rw-r--r--   0        0        0     4112 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.2/threemystic_cloud_data_client/cloud_providers/base_class/base.py
--rw-r--r--   0        0        0    10517 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.2/threemystic_cloud_data_client/cloud_providers/base_class/base_client.py
--rw-r--r--   0        0        0    19323 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.2/threemystic_cloud_data_client/cloud_providers/base_class/base_data.py
--rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.2/threemystic_cloud_data_client/cloud_providers/general/__init__.py
--rw-r--r--   0        0        0     3547 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.2/threemystic_cloud_data_client/cloud_providers/general/config/step_1.py
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.2/threemystic_cloud_data_client/cloud_providers/general/config/base_class/base.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.2/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.2/LICENSE
--rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.2/README.md
--rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.2/hatch.toml
--rw-r--r--   0        0        0     3331 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2670 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.3/threemystic_cloud_data_client/__main__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.3/threemystic_cloud_data_client/__version__.py
+-rw-r--r--   0        0        0     3895 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.3/threemystic_cloud_data_client/cloud_data_client.py
+-rw-r--r--   0        0        0     4150 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.3/threemystic_cloud_data_client/cli/__init__.py
+-rw-r--r--   0        0        0     2950 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.3/threemystic_cloud_data_client/cli/actions/base_class/base.py
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.3/threemystic_cloud_data_client/cli/actions/config/__init__.py
+-rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.3/threemystic_cloud_data_client/cloud_providers/aws/__init__.py
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.3/threemystic_cloud_data_client/cloud_providers/aws/base_class/base.py
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.3/threemystic_cloud_data_client/cloud_providers/aws/client/__init__.py
+-rw-r--r--   0        0        0     3028 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.3/threemystic_cloud_data_client/cloud_providers/aws/config/step_1.py
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.3/threemystic_cloud_data_client/cloud_providers/aws/config/base_class/base.py
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.3/threemystic_cloud_data_client/cloud_providers/azure/__init__.py
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.3/threemystic_cloud_data_client/cloud_providers/azure/base_class/base.py
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.3/threemystic_cloud_data_client/cloud_providers/azure/client/__init__.py
+-rw-r--r--   0        0        0    13738 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.3/threemystic_cloud_data_client/cloud_providers/azure/client/actions/budget.py
+-rw-r--r--   0        0        0     3449 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.3/threemystic_cloud_data_client/cloud_providers/azure/client/actions/cloudstorage.py
+-rw-r--r--   0        0        0    13101 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.3/threemystic_cloud_data_client/cloud_providers/azure/client/actions/storage.py
+-rw-r--r--   0        0        0    11884 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.3/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vm.py
+-rw-r--r--   0        0        0     3174 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.3/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vmss.py
+-rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.3/threemystic_cloud_data_client/cloud_providers/azure/client/actions/base_class/base.py
+-rw-r--r--   0        0        0     3046 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.3/threemystic_cloud_data_client/cloud_providers/azure/config/step_1.py
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.3/threemystic_cloud_data_client/cloud_providers/azure/config/base_class/base.py
+-rw-r--r--   0        0        0     4112 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.3/threemystic_cloud_data_client/cloud_providers/base_class/base.py
+-rw-r--r--   0        0        0    10417 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.3/threemystic_cloud_data_client/cloud_providers/base_class/base_client.py
+-rw-r--r--   0        0        0    19682 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.3/threemystic_cloud_data_client/cloud_providers/base_class/base_data.py
+-rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.3/threemystic_cloud_data_client/cloud_providers/general/__init__.py
+-rw-r--r--   0        0        0     3547 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.3/threemystic_cloud_data_client/cloud_providers/general/config/step_1.py
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.3/threemystic_cloud_data_client/cloud_providers/general/config/base_class/base.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.3/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.3/LICENSE
+-rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.3/README.md
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.3/hatch.toml
+-rw-r--r--   0        0        0     3331 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2670 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.3/PKG-INFO
```

### Comparing `threemystic_cloud_data_client-0.1.2/threemystic_cloud_data_client/cloud_data_client.py` & `threemystic_cloud_data_client-0.1.3/threemystic_cloud_data_client/cloud_data_client.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.2/threemystic_cloud_data_client/cli/__init__.py` & `threemystic_cloud_data_client-0.1.3/threemystic_cloud_data_client/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.2/threemystic_cloud_data_client/cli/actions/base_class/base.py` & `threemystic_cloud_data_client-0.1.3/threemystic_cloud_data_client/cli/actions/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.2/threemystic_cloud_data_client/cli/actions/config/__init__.py` & `threemystic_cloud_data_client-0.1.3/threemystic_cloud_data_client/cli/actions/config/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.2/threemystic_cloud_data_client/cloud_providers/aws/__init__.py` & `threemystic_cloud_data_client-0.1.3/threemystic_cloud_data_client/cloud_providers/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.2/threemystic_cloud_data_client/cloud_providers/aws/config/step_1.py` & `threemystic_cloud_data_client-0.1.3/threemystic_cloud_data_client/cloud_providers/aws/config/step_1.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.2/threemystic_cloud_data_client/cloud_providers/azure/__init__.py` & `threemystic_cloud_data_client-0.1.3/threemystic_cloud_data_client/cloud_providers/azure/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.2/threemystic_cloud_data_client/cloud_providers/azure/client/actions/budget.py` & `threemystic_cloud_data_client-0.1.3/threemystic_cloud_data_client/cloud_providers/azure/client/actions/budget.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.2/threemystic_cloud_data_client/cloud_providers/azure/client/actions/cloudstorage.py` & `threemystic_cloud_data_client-0.1.3/threemystic_cloud_data_client/cloud_providers/azure/client/actions/cloudstorage.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.2/threemystic_cloud_data_client/cloud_providers/azure/client/actions/storage.py` & `threemystic_cloud_data_client-0.1.3/threemystic_cloud_data_client/cloud_providers/azure/client/actions/storage.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,26 +69,26 @@
       "common": self.get_common(),
       "logger": self.get_common().get_logger()
     }
     # This is required because #the normal disk command only looks at long lived disks
     vmss_data = vmss_action(
       **base_action_params
     )
-    self.__vmss = await vmss_data.main(pool=pool) 
+    self.__vmss = await vmss_data.main(pool=pool, run_params= self.get_runparam_key(data_key= None)) 
 
     self.__cost_by_resource_query_definition = {
       "MTD": self.__get_cost_by_resource_query_definition_mtd(),
       "YTD": self.__get_cost_by_resource_query_definition_ytd()
     }
 
     vm_data = vm_action(
       **base_action_params
     )
       
-    self.__vm = await vm_data.main(pool=pool)
+    self.__vm = await vm_data.main(pool=pool, run_params= self.get_runparam_key(data_key= None))
       
 
   async def __get_attached_devices_vm_check_os(self, disk, vm_os_disk = None, *args, **kwarg):
     if vm_os_disk is None:
       return False
     
     if vm_os_disk.get("managed_disk") is None:
```

### Comparing `threemystic_cloud_data_client-0.1.2/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vm.py` & `threemystic_cloud_data_client-0.1.3/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vm.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.2/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vmss.py` & `threemystic_cloud_data_client-0.1.3/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vmss.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.2/threemystic_cloud_data_client/cloud_providers/azure/client/actions/base_class/base.py` & `threemystic_cloud_data_client-0.1.3/threemystic_cloud_data_client/cloud_providers/azure/client/actions/base_class/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from threemystic_cloud_data_client.cloud_providers.base_class.base_data import cloud_data_client_provider_base_data as base
 
 class cloud_data_client_azure_client_action_base(base):
   def __init__(self, *args, **kwargs):
     super().__init__(provider= "azure", *args, **kwargs)  
 
   def get_accounts(self, *args, **kwargs):
+
     if len(self.get_runparam_key(data_key= "data_accounts", default_value= [])) < 1:
       return [ 
         account for account in self.get_cloud_client().get_accounts() 
         if account.resource_container ]
     
     return [ 
         account for account in self.get_cloud_client().get_accounts()
```

### Comparing `threemystic_cloud_data_client-0.1.2/threemystic_cloud_data_client/cloud_providers/azure/config/step_1.py` & `threemystic_cloud_data_client-0.1.3/threemystic_cloud_data_client/cloud_providers/azure/config/step_1.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.2/threemystic_cloud_data_client/cloud_providers/base_class/base.py` & `threemystic_cloud_data_client-0.1.3/threemystic_cloud_data_client/cloud_providers/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.2/threemystic_cloud_data_client/cloud_providers/base_class/base_client.py` & `threemystic_cloud_data_client-0.1.3/threemystic_cloud_data_client/cloud_providers/base_class/base_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -162,41 +162,40 @@
     if not self.get_common().helper_type().general().is_type(obj= data_filter, type_check= dict):
       return {}
     
     return data_filter    
   
   
   def _set_arguments_from_parameters(self, data_action = None, data_filter = None, data_hideempty = None, data_accounts = None, *args, **kwargs):
+    """
+    If the values for the data_* params are not either None or an empty string it will override whatever is in the arguments from the script call
+    """
     processed_info = self.__get_action_parser_options().process_opts(
       parser = self._get_action_parser()
     )
 
-    if data_hideempty is None or not self.get_common().helper_type().general().is_type(obj= data_hideempty, type_check= bool):
-      data_hideempty = processed_info["processed_data"].get("data_hideempty")
-    
-    data_hideempty = self.get_common().helper_type().bool().is_true(check_value= data_hideempty)
-
-    if self.get_common().helper_type().string().is_null_or_whitespace(string_value= data_action):
-      data_action = processed_info["processed_data"].get("data_action")
-    if self.get_common().helper_type().string().is_null_or_whitespace(string_value= data_filter):
-      data_filter = processed_info["processed_data"].get("data_filter")
-    if self.get_common().helper_type().string().is_null_or_whitespace(string_value= data_filter):
-      data_filter = {}
-    
-    if self.get_common().helper_type().string().is_null_or_whitespace(string_value= data_action):
-      if not self.get_suppres_parser_help():
-        self._get_action_parser().print_help()
-        return None
-    
     self._data_arg_param_values={
       "data_action": data_action,
-      "data_filter": self._process_data_run_filter(data_filter= data_filter),
+      "data_filter": data_filter,
       "data_hideempty": data_hideempty,
       "data_accounts": data_accounts,
     }
+
+    for key, item in self._data_arg_param_values.items():
+      if item is None or self.get_common().helper_type().string().is_null_or_whitespace(string_value= item):
+        self._data_arg_param_values[key] = processed_info["processed_data"].get(key)
+
+
+    if self.get_common().helper_type().string().is_null_or_whitespace(string_value= self._data_arg_param_values.get("data_action")):
+      if not self.get_suppres_parser_help():
+        self._get_action_parser().print_help()
+        return None
+      
+    self._data_arg_param_values["data_filter"] = self._process_data_run_filter(data_filter= data_filter)
+    self._data_arg_param_values["data_hideempty"] = self.get_common().helper_type().bool().is_true(check_value= self._data_arg_param_values["data_hideempty"])
     
 
   def get_data_action(self, action = None, *args, **kwargs):
     if hasattr(self, "_data_action_data"):
       
       if self.get_common().helper_type().string().is_null_or_whitespace(string_value= action):
         action = self._data_action_data["default"]
```

### Comparing `threemystic_cloud_data_client-0.1.2/threemystic_cloud_data_client/cloud_providers/base_class/base_data.py` & `threemystic_cloud_data_client-0.1.3/threemystic_cloud_data_client/cloud_providers/base_class/base_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,29 +64,35 @@
   def _set_resource_uniqueid_lambda(self, uniqueid_lambda, *args, **kwargs):
     self._uniqueid_lambda = uniqueid_lambda
   
   async def _pre_load_main_process(self, *args, **kwargs):
     pass
   
   def get_base_return_data(self, account= None, resource_id = None, resource = None, region= None, resource_groups= None, *args, **kwargs):
-    return self.get_common().helper_type().dictionary().merge_dictionary([
+    resource_data = self.get_common().helper_type().dictionary().merge_dictionary([
       {},
       {
         "extra_account": self.get_cloud_client().serialize_azresource(resource= account),
         "extra_region": (
           region if not None else (
             self.get_cloud_client().get_azresource_location(resource= resource) if resource is not None else None)),
         "extra_resourcegroups": resource_groups,
         "extra_id": (
           resource_id if not None else (
             self.get_cloud_client().get_azresource_location(resource= resource) if resource is not None else (
             self.get_cloud_client().get_account_id(account= account) if account is not None else  None))),
       },
       self.get_cloud_client().serialize_azresource(resource= resource) if resource is not None else self.get_cloud_client().serialize_azresource(resource= account)
     ])
+
+    resource_data["extra_resourcegroups"] = self.get_common().helper_type().list().unique_list(
+      data= resource_data.get("extra_resourcegroups"),
+      case_sensitive = False
+    )
+    return resource_data
   
   def format_results(self, results, output_format = None, *args, **kwargs):        
     if output_format is None or (self.get_common().helper_type().string().set_case(string_value= output_format, case= "lower") not in self.get_supported_output_format()):
       output_format = "json"
     
     try:
       if output_format == "yaml":
@@ -121,16 +127,18 @@
   async def __main_poolexecutor(self, *args, **kwargs):   
     with concurrent.futures.ThreadPoolExecutor(self.get_max_thread_pool()) as pool:
         return await self.main_process(
           pool= pool,
           **kwargs
         )
   
-  def get_runparam_key(self, data_key, default_value = {}, *args, **kwargs):
-
+  def get_runparam_key(self, data_key = None, default_value = {}, *args, **kwargs):
+    if data_key is None:
+      return self.__run_params
+    
     if data_key is not None and data_key in self.__run_params:
       if self.get_common().helper_type().general().is_type(obj= self.__run_params.get(data_key), type_check= type(default_value)):
         return self.__run_params.get(data_key)
     
     return default_value
   
   def _set_run_params(self, run_params = None, *args, **kwargs):
@@ -141,33 +149,36 @@
     if not self.get_common().helper_type().general().is_type(obj= run_params, type_check= dict):
       self.__run_params = {}
       return
     
     if "data_action" in run_params:
       del run_params["data_action"]
     
+    if "data_filter" in run_params:
+      if not self.get_common().helper_type().general().is_type(obj= run_params.get("data_filter"), type_check= dict):
+        run_params["data_filter"] = {}
+    
+    if "data_accounts" in run_params:
+      if self.get_common().helper_type().general().is_type(obj= run_params.get("data_accounts"), type_check= str):
+        run_params["data_accounts"] = self.get_common().helper_type().string().split(
+          string_value= run_params["data_accounts"],
+          separator= r"[,;\s]"
+        )
+      if not self.get_common().helper_type().general().is_type(obj= run_params.get("data_accounts"), type_check= list):
+        run_params["data_accounts"] = []
+    
     self.__run_params = self.get_common().helper_type().dictionary().merge_dictionary([
       {},
       {
         "data_filter": {},
         "data_hideempty": False,
         "data_accounts": None
       },
       run_params
     ])
-
-    if self.__run_params.get("data_accounts") is not None:
-      if not self.get_common().helper_type().general().is_type(obj= self.__run_params.get("data_accounts"), type_check= str):
-        self.__run_params["data_accounts"] = self.get_common().helper_type().string().split(string_value= self.__run_params.get("data_accounts"), separator= "[,;]")
-
-    if not self.get_common().helper_type().general().is_type(obj= self.__run_params.get("data_accounts"), type_check= list):
-      self.__run_params["data_accounts"] = []
-      
-    if self.__run_params["data_accounts"] is None:
-      self.__run_params["data_accounts"] = []
   
   
   def _process_data_filter_condition_in(self, condition, condition_value, data_value, *args, **kwargs):
     condition_settings = self._process_data_filter_condition_settings("in", condition)
 
     if condition_settings.get("case_insensitive") is True:
       data_value = self.get_common().helper_type().string().set_case(string_value= data_value, case= "lower")
@@ -339,14 +350,15 @@
     if len(self.get_runparam_key(data_key= "data_filter", default_value= {})) < 1:
       return data
     
     return [data_item for data_item in data if self._process_data_filter_is_row_valid(data_item= data_item)]
 
 
   async def main(self, pool= None, run_params = None, *args, **kwargs):   
+
     self._set_run_params(run_params= run_params)
     if pool == None:
       return await self.__main_poolexecutor(*args, **kwargs)
     
     return await self.main_process(
           pool= pool,
           **kwargs
```

### Comparing `threemystic_cloud_data_client-0.1.2/threemystic_cloud_data_client/cloud_providers/general/__init__.py` & `threemystic_cloud_data_client-0.1.3/threemystic_cloud_data_client/cloud_providers/general/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.2/threemystic_cloud_data_client/cloud_providers/general/config/step_1.py` & `threemystic_cloud_data_client-0.1.3/threemystic_cloud_data_client/cloud_providers/general/config/step_1.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.2/.gitignore` & `threemystic_cloud_data_client-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.2/LICENSE` & `threemystic_cloud_data_client-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.2/README.md` & `threemystic_cloud_data_client-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.2/hatch.toml` & `threemystic_cloud_data_client-0.1.3/hatch.toml`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.2/pyproject.toml` & `threemystic_cloud_data_client-0.1.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -23,16 +23,16 @@
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
   "colorama; platform_system == 'Windows'",
-  "threemystic-common >= 0.1.1",
-  "threemystic-cloud-client >= 0.1.2",
+  "threemystic-common >= 0.1.2",
+  "threemystic-cloud-client >= 0.1.3",
   "typing-extensions >= 4.4.0",
   "asyncio >= 3.4.3",
   "tqdm >= 4.65.0",
   "azure-mgmt-subscription >= 3.1.1",
   "azure-mgmt-managementgroups >= 1.0.0",
   "azure-mgmt-resourcegraph >= 8.0.0",
   "azure-mgmt-costmanagement >= 4.0.0",
```

### Comparing `threemystic_cloud_data_client-0.1.2/PKG-INFO` & `threemystic_cloud_data_client-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: threemystic-cloud-data-client
-Version: 0.1.2
+Version: 0.1.3
 Summary: A tool for collecting data from various cloud providers
 Project-URL: Homepage, https://github.com/3MysticApes/3mystic_cloud_data_client
 Project-URL: Bug Tracker, https://github.com/3MysticApes/3mystic_cloud_data_client/issues
 Author: Ron Truex
 License-Expression: MIT
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
@@ -20,16 +20,16 @@
 Requires-Dist: asyncio>=3.4.3
 Requires-Dist: azure-mgmt-costmanagement>=4.0.0
 Requires-Dist: azure-mgmt-managementgroups>=1.0.0
 Requires-Dist: azure-mgmt-network>=23.1.0
 Requires-Dist: azure-mgmt-resourcegraph>=8.0.0
 Requires-Dist: azure-mgmt-subscription>=3.1.1
 Requires-Dist: colorama; platform_system == 'Windows'
-Requires-Dist: threemystic-cloud-client>=0.1.2
-Requires-Dist: threemystic-common>=0.1.1
+Requires-Dist: threemystic-cloud-client>=0.1.3
+Requires-Dist: threemystic-common>=0.1.2
 Requires-Dist: tqdm>=4.65.0
 Requires-Dist: typing-extensions>=4.4.0
 Description-Content-Type: text/markdown
 
 # 3mystic_cloud_data_client
 A set of scripts to help uniformly pull data from the cloud providers for various resources.
 Currently supports AWS/Azure
```

