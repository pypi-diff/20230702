# Comparing `tmp/threemystic_common-0.0.3.tar.gz` & `tmp/threemystic_common-0.1.0.tar.gz`

## Comparing `threemystic_common-0.0.3.tar` & `threemystic_common-0.1.0.tar`

### file list

```diff
@@ -1,53 +1,56 @@
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 threemystic_common-0.0.3/threemystic_common/__main__.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 threemystic_common-0.0.3/threemystic_common/__version__.py
--rw-r--r--   0        0        0     6341 2020-02-02 00:00:00.000000 threemystic_common-0.0.3/threemystic_common/common.py
--rw-r--r--   0        0        0     2276 2020-02-02 00:00:00.000000 threemystic_common-0.0.3/threemystic_common/base_class/base.py
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 threemystic_common-0.0.3/threemystic_common/base_class/base_common.py
--rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 threemystic_common-0.0.3/threemystic_common/base_class/base_general.py
--rw-r--r--   0        0        0     2516 2020-02-02 00:00:00.000000 threemystic_common-0.0.3/threemystic_common/base_class/base_script_options.py
--rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 threemystic_common-0.0.3/threemystic_common/base_class/generate_data/generate_data_handlers.py
--rw-r--r--   0        0        0     5517 2020-02-02 00:00:00.000000 threemystic_common-0.0.3/threemystic_common/base_class/generate_data/handlers/base.py
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 threemystic_common-0.0.3/threemystic_common/cli/__init__.py
--rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 threemystic_common-0.0.3/threemystic_common/domain/app_monitoring/common.py
--rw-r--r--   0        0        0     3081 2020-02-02 00:00:00.000000 threemystic_common-0.0.3/threemystic_common/domain/app_monitoring/performance.py
--rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 threemystic_common-0.0.3/threemystic_common/domain/cmdb/aws.py
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 threemystic_common-0.0.3/threemystic_common/domain/cmdb/azure.py
--rw-r--r--   0        0        0     2064 2020-02-02 00:00:00.000000 threemystic_common-0.0.3/threemystic_common/domain/cmdb/common.py
--rw-r--r--   0        0        0    14579 2020-02-02 00:00:00.000000 threemystic_common-0.0.3/threemystic_common/domain/cmdb/base_class/base.py
--rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 threemystic_common-0.0.3/threemystic_common/domain/encryption/common.py
--rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 threemystic_common-0.0.3/threemystic_common/domain/encryption/hash.py
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 threemystic_common-0.0.3/threemystic_common/domain/exception/argument.py
--rw-r--r--   0        0        0     1725 2020-02-02 00:00:00.000000 threemystic_common-0.0.3/threemystic_common/domain/exception/common.py
--rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 threemystic_common-0.0.3/threemystic_common/domain/exception/function.py
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 threemystic_common-0.0.3/threemystic_common/domain/exception/generic.py
--rw-r--r--   0        0        0     3600 2020-02-02 00:00:00.000000 threemystic_common-0.0.3/threemystic_common/domain/exception/base_class/base.py
--rw-r--r--   0        0        0     3447 2020-02-02 00:00:00.000000 threemystic_common-0.0.3/threemystic_common/domain/generate_data/generate.py
--rw-r--r--   0        0        0     1937 2020-02-02 00:00:00.000000 threemystic_common-0.0.3/threemystic_common/domain/graph/common.py
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 threemystic_common-0.0.3/threemystic_common/domain/graph/msgraph.py
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 threemystic_common-0.0.3/threemystic_common/domain/graph/base_class/base.py
--rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 threemystic_common-0.0.3/threemystic_common/domain/graph/config/msgraph.py
--rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 threemystic_common-0.0.3/threemystic_common/domain/hashicorp/common.py
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 threemystic_common-0.0.3/threemystic_common/domain/hashicorp/vault.py
--rw-r--r--   0        0        0     2599 2020-02-02 00:00:00.000000 threemystic_common-0.0.3/threemystic_common/domain/helpers/app.py
--rw-r--r--   0        0        0     4871 2020-02-02 00:00:00.000000 threemystic_common-0.0.3/threemystic_common/domain/helpers/config.py
--rw-r--r--   0        0        0     2242 2020-02-02 00:00:00.000000 threemystic_common-0.0.3/threemystic_common/domain/helpers/json.py
--rw-r--r--   0        0        0     1868 2020-02-02 00:00:00.000000 threemystic_common-0.0.3/threemystic_common/domain/helpers/parallel_processing.py
--rw-r--r--   0        0        0     2618 2020-02-02 00:00:00.000000 threemystic_common-0.0.3/threemystic_common/domain/helpers/path.py
--rw-r--r--   0        0        0     2014 2020-02-02 00:00:00.000000 threemystic_common-0.0.3/threemystic_common/domain/helpers/yaml.py
--rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 threemystic_common-0.0.3/threemystic_common/domain/helpers/type/bool.py
--rw-r--r--   0        0        0     3331 2020-02-02 00:00:00.000000 threemystic_common-0.0.3/threemystic_common/domain/helpers/type/common.py
--rw-r--r--   0        0        0     7489 2020-02-02 00:00:00.000000 threemystic_common-0.0.3/threemystic_common/domain/helpers/type/datetime.py
--rw-r--r--   0        0        0     2360 2020-02-02 00:00:00.000000 threemystic_common-0.0.3/threemystic_common/domain/helpers/type/dictionary.py
--rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 threemystic_common-0.0.3/threemystic_common/domain/helpers/type/general.py
--rw-r--r--   0        0        0     3023 2020-02-02 00:00:00.000000 threemystic_common-0.0.3/threemystic_common/domain/helpers/type/list.py
--rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 threemystic_common-0.0.3/threemystic_common/domain/helpers/type/logging.py
--rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 threemystic_common-0.0.3/threemystic_common/domain/helpers/type/openpyxl.py
--rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 threemystic_common-0.0.3/threemystic_common/domain/helpers/type/regex.py
--rw-r--r--   0        0        0     2827 2020-02-02 00:00:00.000000 threemystic_common-0.0.3/threemystic_common/domain/helpers/type/string.py
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 threemystic_common-0.0.3/threemystic_common/exceptions/generate_data/quit.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 threemystic_common-0.0.3/.gitignore
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 threemystic_common-0.0.3/LICENSE
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 threemystic_common-0.0.3/README.md
--rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 threemystic_common-0.0.3/hatch.toml
--rw-r--r--   0        0        0     2974 2020-02-02 00:00:00.000000 threemystic_common-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     2235 2020-02-02 00:00:00.000000 threemystic_common-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 threemystic_common-0.1.0/threemystic_common/__main__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 threemystic_common-0.1.0/threemystic_common/__version__.py
+-rw-r--r--   0        0        0     7303 2020-02-02 00:00:00.000000 threemystic_common-0.1.0/threemystic_common/common.py
+-rw-r--r--   0        0        0     3171 2020-02-02 00:00:00.000000 threemystic_common-0.1.0/threemystic_common/base_class/base.py
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 threemystic_common-0.1.0/threemystic_common/base_class/base_common.py
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 threemystic_common-0.1.0/threemystic_common/base_class/base_general.py
+-rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 threemystic_common-0.1.0/threemystic_common/base_class/base_provider.py
+-rw-r--r--   0        0        0     2516 2020-02-02 00:00:00.000000 threemystic_common-0.1.0/threemystic_common/base_class/base_script_options.py
+-rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 threemystic_common-0.1.0/threemystic_common/base_class/generate_data/generate_data_handlers.py
+-rw-r--r--   0        0        0     6720 2020-02-02 00:00:00.000000 threemystic_common-0.1.0/threemystic_common/base_class/generate_data/handlers/base.py
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 threemystic_common-0.1.0/threemystic_common/cli/__init__.py
+-rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 threemystic_common-0.1.0/threemystic_common/domain/app_monitoring/common.py
+-rw-r--r--   0        0        0     3197 2020-02-02 00:00:00.000000 threemystic_common-0.1.0/threemystic_common/domain/app_monitoring/performance.py
+-rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 threemystic_common-0.1.0/threemystic_common/domain/cmdb/aws.py
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 threemystic_common-0.1.0/threemystic_common/domain/cmdb/azure.py
+-rw-r--r--   0        0        0     2122 2020-02-02 00:00:00.000000 threemystic_common-0.1.0/threemystic_common/domain/cmdb/common.py
+-rw-r--r--   0        0        0    15045 2020-02-02 00:00:00.000000 threemystic_common-0.1.0/threemystic_common/domain/cmdb/base_class/base.py
+-rw-r--r--   0        0        0     1203 2020-02-02 00:00:00.000000 threemystic_common-0.1.0/threemystic_common/domain/encryption/common.py
+-rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 threemystic_common-0.1.0/threemystic_common/domain/encryption/hash.py
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 threemystic_common-0.1.0/threemystic_common/domain/exception/argument.py
+-rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 threemystic_common-0.1.0/threemystic_common/domain/exception/common.py
+-rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 threemystic_common-0.1.0/threemystic_common/domain/exception/function.py
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 threemystic_common-0.1.0/threemystic_common/domain/exception/generic.py
+-rw-r--r--   0        0        0     4674 2020-02-02 00:00:00.000000 threemystic_common-0.1.0/threemystic_common/domain/exception/base_class/base.py
+-rw-r--r--   0        0        0     3597 2020-02-02 00:00:00.000000 threemystic_common-0.1.0/threemystic_common/domain/generate_data/generate.py
+-rw-r--r--   0        0        0     1868 2020-02-02 00:00:00.000000 threemystic_common-0.1.0/threemystic_common/domain/graph/common.py
+-rw-r--r--   0        0        0     9330 2020-02-02 00:00:00.000000 threemystic_common-0.1.0/threemystic_common/domain/graph/msgraph.py
+-rw-r--r--   0        0        0    11209 2020-02-02 00:00:00.000000 threemystic_common-0.1.0/threemystic_common/domain/graph/base_class/base.py
+-rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 threemystic_common-0.1.0/threemystic_common/domain/graph/config/msgraph.py
+-rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 threemystic_common-0.1.0/threemystic_common/domain/hashicorp/common.py
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 threemystic_common-0.1.0/threemystic_common/domain/hashicorp/vault.py
+-rw-r--r--   0        0        0     2599 2020-02-02 00:00:00.000000 threemystic_common-0.1.0/threemystic_common/domain/helpers/app.py
+-rw-r--r--   0        0        0     4725 2020-02-02 00:00:00.000000 threemystic_common-0.1.0/threemystic_common/domain/helpers/config.py
+-rw-r--r--   0        0        0     2462 2020-02-02 00:00:00.000000 threemystic_common-0.1.0/threemystic_common/domain/helpers/json.py
+-rw-r--r--   0        0        0     1869 2020-02-02 00:00:00.000000 threemystic_common-0.1.0/threemystic_common/domain/helpers/parallel_processing.py
+-rw-r--r--   0        0        0     3027 2020-02-02 00:00:00.000000 threemystic_common-0.1.0/threemystic_common/domain/helpers/path.py
+-rw-r--r--   0        0        0     2058 2020-02-02 00:00:00.000000 threemystic_common-0.1.0/threemystic_common/domain/helpers/yaml.py
+-rw-r--r--   0        0        0     2245 2020-02-02 00:00:00.000000 threemystic_common-0.1.0/threemystic_common/domain/helpers/type/bool.py
+-rw-r--r--   0        0        0     4091 2020-02-02 00:00:00.000000 threemystic_common-0.1.0/threemystic_common/domain/helpers/type/common.py
+-rw-r--r--   0        0        0    10148 2020-02-02 00:00:00.000000 threemystic_common-0.1.0/threemystic_common/domain/helpers/type/datetime.py
+-rw-r--r--   0        0        0     2359 2020-02-02 00:00:00.000000 threemystic_common-0.1.0/threemystic_common/domain/helpers/type/dictionary.py
+-rw-r--r--   0        0        0     2360 2020-02-02 00:00:00.000000 threemystic_common-0.1.0/threemystic_common/domain/helpers/type/general.py
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 threemystic_common-0.1.0/threemystic_common/domain/helpers/type/int.py
+-rw-r--r--   0        0        0     3225 2020-02-02 00:00:00.000000 threemystic_common-0.1.0/threemystic_common/domain/helpers/type/list.py
+-rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 threemystic_common-0.1.0/threemystic_common/domain/helpers/type/logging.py
+-rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 threemystic_common-0.1.0/threemystic_common/domain/helpers/type/openpyxl.py
+-rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 threemystic_common-0.1.0/threemystic_common/domain/helpers/type/regex.py
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 threemystic_common-0.1.0/threemystic_common/domain/helpers/type/requests.py
+-rw-r--r--   0        0        0     4827 2020-02-02 00:00:00.000000 threemystic_common-0.1.0/threemystic_common/domain/helpers/type/string.py
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 threemystic_common-0.1.0/threemystic_common/exceptions/generate_data/quit.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 threemystic_common-0.1.0/.gitignore
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 threemystic_common-0.1.0/LICENSE
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 threemystic_common-0.1.0/README.md
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 threemystic_common-0.1.0/hatch.toml
+-rw-r--r--   0        0        0     3033 2020-02-02 00:00:00.000000 threemystic_common-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2312 2020-02-02 00:00:00.000000 threemystic_common-0.1.0/PKG-INFO
```

### Comparing `threemystic_common-0.0.3/threemystic_common/common.py` & `threemystic_common-0.1.0/threemystic_common/common.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,22 +13,39 @@
     super().__init__(*args, **kwargs)
     self._logger = self.helper_type().logging().get_child_logger(
       child_logger_name= "3mystic_common_lib_logger",
       logger= logger
     )
     self.update_configuration(config_path= config_path)
   
-  def get_threemystic_config_path(self, *args, **kwargs):
+  
+  def get_threemystic_public_directory(self, *args, **kwargs):
+    general_path = self.helper_path().expandpath_user(
+      path= "~/3mystic_general"
+    )
+    if not general_path.exists():
+      general_path.mkdir(parents= True)
+    
+    return general_path
+  
+  def get_threemystic_directory(self, *args, **kwargs):
     general_path = self.helper_path().expandpath_user(
       path= "~/.3mystic"
     )
     if not general_path.exists():
       general_path.mkdir(parents= True)
     
     return general_path
+  
+  def get_threemystic_directory_config(self, *args, **kwargs):
+    config_path = self.get_threemystic_directory().joinpath("config")
+    if not config_path.exists():
+      config_path.mkdir(parents= True)
+    
+    return config_path
 
   def version(self):
     if hasattr(self, "_version"):
       return self._version
     import threemystic_common.__version__ as __version__
     self._version = __version__.__version__
     return self.version()
@@ -40,27 +57,45 @@
     
     self._config_data = {}
     # Add load data code by path
 
   def get_configuration(self, *args, **kwargs):
     return self._config_data
   
-  def exception(self, *args, **kwargs):
+  def graph(self, unset = False, *args, **kwargs):
+    if(unset):
+      self._unset("_graph")
+      return
+    
+    if hasattr(self, "_graph"):
+      return self._graph
+    
+    from threemystic_common.domain.graph.common import graph_common as graph        
+    self._graph = graph(
+      main_reference= self, *args, **kwargs
+    )
+    return self.graph(*args, **kwargs)
+  
+  def exception(self, unset = False, *args, **kwargs):
+    if(unset):
+      self._unset("_exception")
+      return
+    
     if hasattr(self, "_exception"):
-      return self._monitoring
+      return self._exception
     
     from threemystic_common.domain.exception.common import exception_common as exception        
-    self._monitoring = exception(
+    self._exception = exception(
       main_reference= self, *args, **kwargs
     )
     return self.exception(*args, **kwargs)
 
   def app_monitoring(self, unset = False, *args, **kwargs):
     if(unset):
-      self._unset("_exception")
+      self._unset("_monitoring")
       return
     
     if hasattr(self, "_monitoring"):
       return self._monitoring
     
     from threemystic_common.domain.app_monitoring.common import \
         app_monitoring_common as app_monitoring
@@ -85,18 +120,18 @@
   
   def encryption(self, unset = False, *args, **kwargs):
     if(unset):
       self._unset("_encryption")
       return
     
     if hasattr(self, "_encryption"):
-      return self._helper_dictionary
+      return self._encryption
     
-    from threemystic_common.domain.encryption import encryption_common as encryption
-    self._helper_dictionary = encryption(
+    from threemystic_common.domain.encryption.common import encryption_common as encryption
+    self._encryption = encryption(
       main_reference= self, *args, **kwargs
     )
     return self.encryption(*args, **kwargs)
   
   def cmdb(self, unset = False, *args, **kwargs):
     if(unset):
       self._unset("_cmdb")
@@ -175,15 +210,15 @@
     if hasattr(self, "_helper_parallel_processing"):
       return self._helper_parallel_processing
     
     from threemystic_common.domain.helpers.parallel_processing import helper_parallel_processing as helper
     self._helper_parallel_processing = helper(
       main_reference= self, *args, **kwargs
     )
-    return self.helper_json(*args, **kwargs)
+    return self.helper_parallel_processing(*args, **kwargs)
   
   def helper_config(self, unset = False, *args, **kwargs):
     if(unset):
       self._unset("_helper_config")
       return
     
     if hasattr(self, "_helper_config"):
```

### Comparing `threemystic_common-0.0.3/threemystic_common/base_class/base.py` & `threemystic_common-0.1.0/threemystic_common/base_class/base.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,43 +1,47 @@
-import abc
+from abc import ABC
 from logging import Logger
 
-class base(abc.ABC): 
+class base(ABC): 
   """This is a set of library wrappers to help general python apps"""
 
   def __init__(self, *args, **kwargs) -> None:
     super().__init__()
     self._custom_init_pre()
 
   def _custom_init_pre(self, *args, **kwargs):
     pass    
    
   
-  def __init_main(self, main_reference, *args, **kwargs):
+  def _init_main(self, main_reference, *args, **kwargs):
     if main_reference is not None:
       self._main_reference = main_reference
   
   def get_main(self, *args, **kwargs):
     if not hasattr(self, "_main_reference"):
       return self._main_reference
     
     return None
 
-  def __logger_init(self, logger_name, logger = None, init_object = None,  refresh = False, *args, **kwargs):
+  def _logger_init(self, logger_name, logger = None, init_object = None,  refresh = False, *args, **kwargs):
     if hasattr(self, "_logger") and not refresh:
       if self._logger is not None:
         return
 
     if logger is not None or init_object is not None:
       self._logger = self.get_common().helper_type().logging().get_child_logger(
         child_logger_name= logger_name,
         logger= logger if init_object is None else init_object.get_logger()
       )
 
   def get_logger(self) -> Logger:
+    if hasattr(self, "_main_reference"):      
+      if self._main_reference is not None:
+        return self._main_reference.get_common().get_logger()
+    
     if hasattr(self, "_logger"):
       return self._logger
     
     if hasattr(self, "_logger_name"):
       self._logger = self.get_main().get_logger().getChild(self._logger_name)
       return self.get_logger()
     
@@ -46,29 +50,46 @@
 
   def _unset(self, attribute, *args, **kwargs):
       if not hasattr(self, attribute):
         return
 
       delattr(self, attribute)
   
-  def __init_common(self, init_object = None, common = None, refresh = False, force_skip_getcommon = False, *args, **kwargs):
+  def _init_common(self, init_object = None, common = None, refresh = False, force_skip_getcommon = False, *args, **kwargs):
     if hasattr(self, "_common") and not refresh:
       if self._common is not None:
         return self.get_common()
 
     if init_object is not None and hasattr(init_object, "get_common") and not force_skip_getcommon:
       self._common = init_object.get_common()
       return self.get_common()
     
+    from threemystic_common.common import common as threemystic_common
+    if common is not None:
+      if isinstance(common, threemystic_common):
+        self._common = common
+        return self.get_common()
+      if hasattr(common, "get_common") and not refresh:
+        if self.get_common() is not None and isinstance(common.get_common(), threemystic_common):
+          self._common = common.get_common()
+          return self.get_common()
+      if hasattr(common, "_common") and not refresh:
+        if self._common is not None and isinstance(common, threemystic_common):
+          self._common = common._common
+          return self.get_common()
+        
     if common is None:
-      from threemystic_common.common import common as threemystic_common
       self._common = threemystic_common()
-      self.get_common()
+      return self.get_common()
   
-  def get_common(self, *args, **kwargs):
+  def get_common(self, *args, **kwargs):    
+    if hasattr(self, "_main_reference"):
+      if self._main_reference is not None:
+        return self._main_reference.get_common()
+    
     if hasattr(self, "_common"):
       if self._common is not None:
         return self._common
     
-    self.__init_common(force_skip_getcommon= True)
+    self._init_common(force_skip_getcommon= True)
     return self.get_common()
```

### Comparing `threemystic_common-0.0.3/threemystic_common/base_class/base_script_options.py` & `threemystic_common-0.1.0/threemystic_common/base_class/base_script_options.py`

 * *Files identical despite different names*

### Comparing `threemystic_common-0.0.3/threemystic_common/base_class/generate_data/handlers/base.py` & `threemystic_common-0.1.0/threemystic_common/base_class/generate_data/handlers/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from threemystic_common.exceptions.generate_data.quit import quit_exception
 
 class base_handler:
   def __init__(self, *args, **kwargs):
-    pass
+    self.__is_array = False
   
   def _response_allow_empty(self, item, *args, **kwargs):
     return item.get("allow_empty") == True
 
   def _response_is_valid(self, response_value, item, *args, **kwargs):
+
     if self._response_allow_empty(item= item) and self._is_response_empty(response_value= response_value):
       return True
 
     if self._response_is_required(item= item) and self._is_response_empty(response_value= response_value):
       return False
     
     if item.get("validation") is not None:
@@ -22,19 +23,24 @@
   def _quit_options(self, *args, **kwargs):
     return ["exit", "quit"]
   
   def _quit_display_text(self, allow_quit, *args, **kwargs):
     if allow_quit or self._is_array():
       print(f"To exit please type one of the following:\n{self._quit_options()}")
 
-  def _type(self, *args, **kwargs):
+  def _type(self, item, *args, **kwargs):
+    if item.get("type") is not None:
+      if item.get("type") == list:
+        self.__is_array = True
+      return item.get("type")
+
     return None
 
   def _is_array(self, *args, **kwargs):
-    return False
+    return self.__is_array
     
   def _is_response_empty(self, response_value):
     if not response_value:
       return True
     
     if not str(response_value).strip():
       return True
@@ -108,15 +114,15 @@
     self._get_user_input_header_prompt(attribute_name= attribute_name, item= item)
     print()
     if self._response_is_required(item= item):
       self._response_is_required_required(item= item, *args, **kwargs)
     else:
       self._response_is_required_not_required(item= item, *args, **kwargs)
 
-  def _process_type_none(self, item, allow_quit, *args, **kwargs):
+  def _prompt_user(self, item, allow_quit, *args, **kwargs):
     return_value = self._get_user_input_prompt()
 
     if allow_quit and return_value.lower() in self._quit_options():
       raise quit_exception()
 
     if not self._response_is_required(item= item):
       return return_value if self._response_is_valid(response_value= return_value, item= item) else self._get_default(item= item)
@@ -130,31 +136,65 @@
       return_value = self._get_user_input_prompt()
       if allow_quit and return_value.lower() in self._quit_options():
         raise quit_exception()
         
     
     return return_value
 
-  def _get_user_input(self, item, allow_quit, *args, **kwargs):
-    return_value = None
-    
-    if self._type() == None:
-      try:
-        return_value = self._process_type_none(item= item, allow_quit= allow_quit)
+  def _process_type_list(self, item, allow_quit, *args, **kwargs):
+    try:
+      
+      if self._type(item) == list:
+        return_value = self._prompt_user(item= item, allow_quit= allow_quit)
         if self._response_allow_empty(item= item) and self._is_response_empty(response_value= return_value):
           if "default" in item:
             return_value = item.get("default")
-      
         
         return {
           "raw": return_value,
           "formated": self._get_formated(return_value= return_value, item= item)
         }
-      except quit_exception:
-        return {"quit": True}
+      return None
+    except quit_exception:
+      return {"quit": True}
+    except KeyboardInterrupt:
+      return {"quit": True}
+
+  def _process_type_default(self, item, allow_quit, *args, **kwargs):
+    try:
+      return_value = self._prompt_user(item= item, allow_quit= allow_quit)
+      if self._response_allow_empty(item= item) and self._is_response_empty(response_value= return_value):
+        if "default" in item:
+          return_value = item.get("default")
+      
+      return {
+        "raw": return_value,
+        "formated": self._get_formated(return_value= return_value, item= item)
+      }
+      
+    except quit_exception:
+      return {"quit": True}
+    except KeyboardInterrupt:
+      return {"quit": True}
+  
+  def _process_type(self, item, *args, **kwargs):
+    if self._type(item) == list:
+      return self._process_type_list(item= item, *args, **kwargs)
+
+    return self._process_type_default(item= item, *args, **kwargs)
+
+
+  def _get_user_input(self, item, allow_quit, *args, **kwargs):
+
+    return self._process_type(
+      item= item,
+      allow_quit= allow_quit, 
+      *args, **kwargs
+    )
+    
 
   def _get_user_input_prompt(self, *args, **kwargs):
     print("-------------------------------------------------------------------------\n")
     return input("$: ")
 
   def generate(self, attribute_name, item, allow_quit = True, *args, **kwargs):
     self._get_user_input_header(attribute_name= attribute_name, item= item, allow_quit= allow_quit)
```

### Comparing `threemystic_common-0.0.3/threemystic_common/domain/app_monitoring/common.py` & `threemystic_common-0.1.0/threemystic_common/domain/app_monitoring/common.py`

 * *Files identical despite different names*

### Comparing `threemystic_common-0.0.3/threemystic_common/domain/app_monitoring/performance.py` & `threemystic_common-0.1.0/threemystic_common/domain/app_monitoring/performance.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,26 +27,26 @@
     if hasattr(self, "_memory"):
       return self._memory
     
     if raise_exception_not_init:
       raise self._main_reference.exception().exception(
         exception_type = "generic"
       ).type_error(
-        logger = self.get_logger(),
+        logger = self._main_reference.get_common().get_logger(),
         message = f"Memory tracing not defined"
       )
     return None
 
   def startstop_tracemalloc(self, action = None, *args, **kwargs):
     memory_performance = self.memory_performance(raise_exception_not_init= False)
     if memory_performance is None:
       raise self._main_reference.exception().exception(
         exception_type = "generic"
       ).type_error(
-        logger = self.get_logger(),
+        logger = self._main_reference.get_common().get_logger(),
         message = f"Memory tracing not defined"
       )
     if action is None:
       if memory_performance.is_tracing():
         return memory_performance.stop()
       return memory_performance.start()
     
@@ -64,30 +64,30 @@
   
   def performance_monitoring_memory_snapshot(self, clear_tracing = False):    
     memory_performance = self.memory_performance(raise_exception_not_init= False)
     if memory_performance is None:
       raise self._main_reference.exception().exception(
         exception_type = "generic"
       ).type_error(
-        logger = self.get_logger(),
+        logger = self._main_reference.get_common().get_logger(),
         message = f"Memory tracing not defined"
       )
 
     snapshot = memory_performance.take_snapshot()
     if clear_tracing:
       memory_performance.clear_traces()
     return snapshot
   
   def performance_monitoring_memory(self, *args, **kwargs):
     memory_performance = self.memory_performance(raise_exception_not_init= False)
     if memory_performance is None:
       raise self._main_reference.exception().exception(
         exception_type = "generic"
       ).type_error(
-        logger = self.get_logger(),
+        logger = self._main_reference.get_common().get_logger(),
         message = f"Memory tracing not defined"
       )
 
     return {
       "traced_memory": memory_performance.get_traced_memory(),
       "tracemalloc_memory": memory_performance.get_tracemalloc_memory()
     }
```

### Comparing `threemystic_common-0.0.3/threemystic_common/domain/cmdb/aws.py` & `threemystic_common-0.1.0/threemystic_common/domain/cmdb/aws.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from threemystic_common.domain.cmdb.base_class.base import cmdb_base as base
 
 
 class cmdb_aws(base): 
   """This is a common set of methods and libraries"""
 
   def __init__(self, *args, **kwargs) -> None:
-    super().__init(logger_name= "cmdb_aws", *args, **kwargs)
+    super().__init__(logger_name= "cmdb_aws", *args, **kwargs)
   
   def get_source(self, *args, **kwargs):
     return "aws"
   
   def __generate_resource_tags_csv_tag(self, tag, tag_attributes, tag_attribute_seperator):
     return tag_attribute_seperator.join([str(tag[attr]) for attr in tag if attr in tag_attributes])
```

### Comparing `threemystic_common-0.0.3/threemystic_common/domain/cmdb/common.py` & `threemystic_common-0.1.0/threemystic_common/domain/cmdb/common.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,24 +22,24 @@
           
       return 
     
     if self._main_reference.helper_type().string().is_null_or_whitespace(cloud_source):
       raise self._main_reference.exception().exception(
         exception_type = "argument"
       ).type_error(
-        logger = self.get_logger(),
+        logger = self._main_reference.get_common().get_logger(),
         name = "cloud_source",
         message = "cloud_source is None"
       )
     
     if cloud_source.lower() not in self.__supported_cloud_source:
       raise self._main_reference.exception().exception(
         exception_type = "argument"
       ).exception(
-        logger = self.get_logger(),
+        logger = self._main_reference.get_common().get_logger(),
         name = "cloud_source",
         message = f"Unknown cloud_source: {cloud_source}"
       )
     
     cloud_source = cloud_source.lower()
     if cloud_source == "aws":
       if self._cmdb.get(cloud_source) is not None:
```

### Comparing `threemystic_common-0.0.3/threemystic_common/domain/cmdb/base_class/base.py` & `threemystic_common-0.1.0/threemystic_common/domain/cmdb/base_class/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import abc
+from abc import abstractmethod
 import asyncio
 from threemystic_common.base_class.base_common import base
 from openpyxl import Workbook
 
 class cmdb_base(base): 
   """This is a set of library wrappers to help create a cmdb"""
 
@@ -38,31 +38,31 @@
 
     return {
       "no_region": prepend + ["Account ID", "Account Name"],
       "region": prepend + ["Account ID", "Account Name", "Region" ]
     }
 
   # get_cmdb_source
-  @abc.abstractmethod
+  @abstractmethod
   def get_source(self, *args, **kwargs):
     raise self._main_reference.exception().exception(
       exception_type = "function"
     ).not_implemented(
-      logger = self.get_logger(),
+      logger = self._main_reference.get_common().get_logger(),
       name = "get_source",
       message = f"Not Implemented"
     )
 
   # aws_get_resource_groups
-  @abc.abstractmethod
+  @abstractmethod
   def get_resource_groups(self, *args, **kwargs):    
     raise self._main_reference.exception().exception(
       exception_type = "function"
     ).not_implemented(
-      logger = self.get_logger(),
+      logger = self._main_reference.get_common().get_logger(),
       name = "get_resource_groups",
       message = f"Not Implemented"
     )
 
   def get_report_default_columns(self, data_item, *args, **kwargs):
     if self._main_reference.helper_type().general().is_type(data_item["default_columns"], dict):
       return data_item["default_columns"]["default"]
@@ -96,15 +96,15 @@
     return cmdb_data
   
   # compare_cmdb_account_ids
   def compare_account_ids(self, account1, account2, *args, **kwargs):
     raise self._main_reference.exception().exception(
       exception_type = "function"
     ).not_implemented(
-      logger = self.get_logger(),
+      logger = self._main_reference.get_common().get_logger(),
       name = "compare_account_ids",
       message = f"Not Implemented"
     )
   
   # compare_cmdb_string_possible_numeric
   def compare_string_possible_numeric(cls, str1, str2, *args, **kwargs):
     str1 = str(str1).strip(" '")
@@ -112,46 +112,46 @@
     if not str1.lower().startswith("=text("):
       str1 = f'=Text("{str1}", "?")'
     if not str2.lower().startswith("=text("):
       str2 = f'=Text("{str2}", "?")'
 
     return str1.lower() == str2.lower()
 
-  @abc.abstractmethod
+  @abstractmethod
   def generate_resource_tags_csv(self, *args, **kwargs): 
     raise self._main_reference.exception().exception(
         exception_type = "function"
       ).not_implemented(
-        logger = self.get_logger(),
+        logger = self._main_reference.get_common().get_logger(),
         name = "generate_resource_tags_csv",
         message = f"Not Implemented"
       )
   
   # generate_tag_columns_cmdb
   # generate_tag_columns
-  @abc.abstractmethod
+  @abstractmethod
   def generate_tag_columns(self, *args, **kwargs):
     # This will combine the 2 methods into one. I just would need to pass a variable to indicate if it should contain the source column
     raise self._main_reference.exception().exception(
       exception_type = "function"
     ).not_implemented(
-      logger = self.get_logger(),
+      logger = self._main_reference.get_common().get_logger(),
       name = "generate_tag_columns",
       message = f"Not Implemented"
     )
   
   # generate_tag_columns_cmdb_basic
   # generate_tag_columns_basic
-  @abc.abstractmethod
+  @abstractmethod
   def generate_tag_columns_basic(self, *args, **kwargs):
     # This will combine the 2 methods into one. I just would need to pass a variable to indicate if it should contain the source column
     raise self._main_reference.exception().exception(
       exception_type = "function"
     ).not_implemented(
-      logger = self.get_logger(),
+      logger = self._main_reference.get_common().get_logger(),
       name = "generate_tag_columns_basic",
       message = f"Not Implemented"
     )
   
   def get_tags_as_dict(self, *args, **kwargs):
     # the tags passed into the generate_tag_columns should be a standardized dictionary of {Key:Value}
     raise self._main_reference.exception().exception(
@@ -170,15 +170,15 @@
 
   def add_custom_require_tags(self, custom_require_tags, merge_if_existing = True, *args, **kwargs):
     
     if not self._main_reference.helper_type().general().is_type(custom_require_tags, dict):
       raise self._main_reference.exception().exception(
         exception_type = "argument"
       ).type_error(
-        logger = self.get_logger(),
+        logger = self._main_reference.get_common().get_logger(),
         name = "custom_require_tags",
         message = f"custom_require_tags is of type {type(custom_require_tags)}"
       )
 
     if merge_if_existing:
       self._custom_require_tags = self._main_reference.helper_type().dictionary().merge_dictionary(
         [
@@ -199,15 +199,15 @@
   
   def remove_custom_require_tags(self, custom_require_tag_key, raise_exception = False, *args, **kwargs):    
     if custom_require_tag_key not in self.get_custom_require_tags():
       if raise_exception:
         raise self._main_reference.exception().exception(
           exception_type = "generic"
         ).key_error(
-          logger = self.get_logger(),
+          logger = self._main_reference.get_common().get_logger(),
           name = "custom_require_tags",
           message = f"key not found: {custom_require_tag_key}"
         )
       return None
     
     return self._custom_require_tags.pop(custom_require_tag_key)
 
@@ -221,25 +221,25 @@
     )
   
   # init_report_workbook_cmdb_header_row
   def init_report_workbook_header_row(self, datasheet, inventory_data_column_info, *args, **kwargs):
     raise self._main_reference.exception().exception(
       exception_type = "function"
     ).not_implemented(
-      logger = self.get_logger(),
+      logger = self._main_reference.get_common().get_logger(),
       name = "compare_account_ids",
       message = f"Not Implemented"
     )
 
   # init_report_workbook_cmdb
   def init_report_workbook(self, InventoryDataSheet, inventory_data_column_info, lambda_create, include_deleted_column = False, *args, **kwargs):
     raise self._main_reference.exception().exception(
       exception_type = "function"
     ).not_implemented(
-      logger = self.get_logger(),
+      logger = self._main_reference.get_common().get_logger(),
       name = "compare_account_ids",
       message = f"Not Implemented"
     )
   
   def get_workbook_column_header_display_dict(self, column_display, default, existing_header = None, *args, **kwargs):
     if self._main_reference.helper_type().general().is_type(column_display, str):
       return column_display
@@ -264,81 +264,81 @@
     
     raise Exception(f"unknown inventory_data_column_info_column - {self._main_reference.helper_json().dumps(inventory_data_column_info_column)}")
   
   def pre_init_report_workbook(self, *args, **kwargs):
     raise self._main_reference.exception().exception(
       exception_type = "function"
     ).not_implemented(
-      logger = self.get_logger(),
+      logger = self._main_reference.get_common().get_logger(),
       name = "compare_account_ids",
       message = f"Not Implemented"
     )
   
   def init_report_workbook(self, InventoryDataSheet, inventory_data_column_info, lambda_create, *args, **kwargs):
     raise self._main_reference.exception().exception(
       exception_type = "function"
     ).not_implemented(
-      logger = self.get_logger(),
+      logger = self._main_reference.get_common().get_logger(),
       name = "compare_account_ids",
       message = f"Not Implemented"
     )
   
   def get_tag_report_columns(self, InventoryDataSheet, *args, **kwargs):
     raise self._main_reference.exception().exception(
       exception_type = "function"
     ).not_implemented(
-      logger = self.get_logger(),
+      logger = self._main_reference.get_common().get_logger(),
       name = "compare_account_ids",
       message = f"Not Implemented"
     )
 
   def get_default_report_columns(self, InventoryDataSheet, *args, **kwargs):
     raise self._main_reference.exception().exception(
       exception_type = "function"
     ).not_implemented(
-      logger = self.get_logger(),
+      logger = self._main_reference.get_common().get_logger(),
       name = "compare_account_ids",
       message = f"Not Implemented"
     )
 
   def get_default_report_columns_cmdb(self, InventoryDataSheet, *args, **kwargs):
     raise self._main_reference.exception().exception(
       exception_type = "function"
     ).not_implemented(
-      logger = self.get_logger(),
+      logger = self._main_reference.get_common().get_logger(),
       name = "compare_account_ids",
       message = f"Not Implemented"
     )
 
   # get_report_default_row_cmdb
-  @abc.abstractmethod
+  @abstractmethod
   def get_report_default_row(self, *args, **kwargs):
     raise self._main_reference.exception().exception(
         exception_type = "function"
       ).not_implemented(
-        logger = self.get_logger(),
+        logger = self._main_reference.get_common().get_logger(),
         name = "generate_resource_tags_csv",
         message = f"Not Implemented"
       )
   
-  @abc.abstractmethod
+  @abstractmethod
   def get_account_environment(self, *args, **kwargs):
     raise self._main_reference.exception().exception(
         exception_type = "function"
       ).not_implemented(
-        logger = self.get_logger(),
+        logger = self._main_reference.get_common().get_logger(),
         name = "generate_resource_tags_csv",
         message = f"Not Implemented"
       )
 
   # save_report
   def save_report(self, report_dir, report_name, workbook, show_output = True):
     date_now = self._main_reference.helper_type().datetime().get(time_zone = "local")
 
-    report_name = report_name.format(self._main_reference.helper_type().datetime().datetime_as_string(datetime_format = "%Y%M%d%H%M", datetime_format = date_now))
+    report_name = report_name.format(self._main_reference.helper_type().datetime().datetime_as_string(dt_format = "%Y%M%d%H%M", dt = date_now))
     # report_directory_path_info = Path("{}/".format(report_dir)).resolve()    
     report_directory_path_info = self._main_reference.helper_path().get(path = f"{report_dir}/")
     report_path = report_directory_path_info.joinpath(f"{report_name}")
     
     if not report_directory_path_info.exists():
       report_directory_path_info.mkdir(parents=True, exist_ok=True)
```

### Comparing `threemystic_common-0.0.3/threemystic_common/domain/encryption/common.py` & `threemystic_common-0.1.0/threemystic_common/domain/encryption/common.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,22 +16,22 @@
       if hasattr(self, "_hash_method"):
         if self._hash_method.get(hash_method) is not None:
           self._hash_method.pop(hash_method)
           
       return 
     
     hash_method = hash_method.lower() if hash_method is not None else ""
-    if not hasattr(self, "_hash_method"):
+    if hasattr(self, "_hash_method"):
       if self._hash_method.get(hash_method) is not None:
         return self._hash_method[hash_method]
     
     if not hasattr(self, "_hash"):
       from threemystic_common.domain.encryption.hash import encryption_hash as encryption
       self._hash = encryption
       self._hash_method = {}
     
     self._hash_method[hash_method] = self._hash(
       main_reference= self._main_reference,
       hash_method= hash_method
     )
-    return self.hash(*args, **kwargs)
+    return self.hash(hash_method= hash_method, *args, **kwargs)
```

### Comparing `threemystic_common-0.0.3/threemystic_common/domain/encryption/hash.py` & `threemystic_common-0.1.0/threemystic_common/domain/encryption/hash.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,19 +4,19 @@
   """This is a set of library wrappers to help monitor performance"""
 
   def __init__(self, *args, **kwargs) -> None:
     super().__init__(logger_name= "encryption_hash", *args, **kwargs)
     self._hash_method = self.__get_hash_method(*args, **kwargs)
   
   def __get_hash_method(self, hash_method, *args, **kwargs):
-    if self._main_reference.helper_type().general().is_null_or_whitespace(hash_method):
+    if self._main_reference.helper_type().string().is_null_or_whitespace(hash_method):
       raise self._main_reference.exception().exception(
         exception_type = "argument"
       ).not_implemented(
-        logger = self.get_logger(),
+        logger = self._main_reference.get_common().get_logger(),
         name = "hash_method",
         message = f"argument not provided"
       )
 
     if hash_method.lower() == "sha1":
       from hashlib import sha1
       return sha1
@@ -28,15 +28,15 @@
     if hash_method.lower() == "md5":
       from hashlib import md5
       return md5
     
     raise self._main_reference.exception().exception(
         exception_type = "generic"
       ).not_implemented(
-        logger = self.get_logger(),
+        logger = self._main_reference.get_common().get_logger(),
         name = "hash_method",
         message = f"Unknown Hash Method Provided: {hash_method}"
       )
     
   # generate_hash_fromobject
   def generate_hash(self, data, *args, **kwargs):
     if self._main_reference.helper_type().general().is_type(data, str):
```

### Comparing `threemystic_common-0.0.3/threemystic_common/domain/exception/common.py` & `threemystic_common-0.1.0/threemystic_common/domain/exception/common.py`

 * *Files 16% similar despite different names*

```diff
@@ -17,30 +17,30 @@
     return [
       "argument",
       "function"
     ]
 
   def exception(self, exception_type, *args, **kwargs):
     
-    if self.helper_type().string().is_null_or_whitespace(exception_type):
+    if self._main_reference.helper_type().string().is_null_or_whitespace(exception_type):
       return self._exception.get("generic")
 
     exception_type = exception_type.lower()
     if exception_type not in self._custom_exceptions():
-      return self._exception.get("generic")
+      return self._exception.get("generic")(main_reference= self._main_reference, exception_type= exception_type, *args, **kwargs)
     
     if exception_type == "argument":
       if self._exception.get(exception_type):
-        return self._exception[exception_type].exception(exception_type= exception_type, *args, **kwargs)
+        return self._exception[exception_type](main_reference= self._main_reference, exception_type= exception_type, *args, **kwargs)
       
       from threemystic_common.domain.exception.argument import exception_argument as exception
       self._exception[exception_type] = exception
       return self.exception(exception_type= exception_type, *args, **kwargs)
     
     if exception_type == "function":
       if self._exception.get(exception_type):
-        return self._exception[exception_type].exception(exception_type= exception_type, *args, **kwargs)
+        return self._exception[exception_type](main_reference= self._main_reference, exception_type= exception_type, *args, **kwargs)
       
       from threemystic_common.domain.exception.function import exception_function as exception
       self._exception[exception_type] = exception
       return self.exception(exception_type= exception_type, *args, **kwargs)
```

### Comparing `threemystic_common-0.0.3/threemystic_common/domain/generate_data/generate.py` & `threemystic_common-0.1.0/threemystic_common/domain/generate_data/generate.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,29 +21,29 @@
     return_data = {}
     
     for key, item in generate_data_config.items():
       if key.lower() in self._get_restricted_keynames() and not is_child_elemement:
         raise self._main_reference.exception().exception(
           exception_type = "argument"
         ).exception(
-          logger = self.get_logger(),
+          logger = self._main_reference.get_common().get_logger(),
           name = "generate_data_config",
           message = f"Contains an element using a reserved key: {key}. Reserved Keys: {self._get_restricted_keynames()}"
         )   
 
       if item.get("skip"):
         if item["skip"](return_data):
           return_data[key] = None
           continue
 
       if item.get("handler") is None:
         raise self._main_reference.exception().exception(
             exception_type = "argument"
           ).type_error(
-            logger = self.get_logger(),
+            logger = self._main_reference.get_common().get_logger(),
             name = "generate_data_config",
             message = f"Handler cannot be None for key: {key}."
           )
         
       if item.get("children") is not None:
         item.get("handler").print_descrinption(item)
 
@@ -58,34 +58,34 @@
             
           continue
         
         if key.lower() in self._get_restricted_keynames() and not is_child_elemement:
           raise self._main_reference.exception().exception(
             exception_type = "argument"
           ).type_error(
-            logger = self.get_logger(),
+            logger = self._main_reference.get_common().get_logger(),
             name = "generate_data_config",
             message = f"Unknown children type. Should be either a Dictrionary of children or a list. Got Type {type(item['children'])}"
           )
         continue
       
       return_data[key] = item.get("handler").generate(
         attribute_name= key, 
         item= item
       )
-
-      if return_data[key].get("quit") == True:
+      
+      if return_data[key] is None or return_data[key].get("quit") == True:
         print("Exiting now. No Data Saved")
         return None
 
       if "raw" not in return_data[key] is None or "formated" not in return_data[key] is None:
         raise self._main_reference.exception().exception(
             exception_type = "function"
           ).exception(
-            logger = self.get_logger(),
+            logger = self._main_reference.get_common().get_logger(),
             name = "handler",
             message = f"Handler for Key: {key} did not return proper response. Should return a dictionary with raw and formated"
           )
     
     return return_data
```

### Comparing `threemystic_common-0.0.3/threemystic_common/domain/graph/common.py` & `threemystic_common-0.1.0/threemystic_common/domain/graph/common.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,52 +6,48 @@
 
   def __init__(self, *args, **kwargs) -> None:
     super().__init__(logger_name= f"graph", *args, **kwargs)
   
   def __get_supported_graphs(self):
     return ["msgraph"]
   
-  def init_graph(self, graph_method, graph_config, *args, **kwargs):    
+  def init_graph(self, graph_method, *args, **kwargs):    
     graph_method = graph_method.lower() if graph_method is not None else ""
     
     if graph_method not in self.__get_supported_graphs():
       raise self._main_reference.exception().exception(
         exception_type = "generic"
       ).not_implemented(
-        logger = self.get_logger(),
+        logger = self._main_reference.get_common().get_logger(),
         name = "graph_method",
         message = f"Unknown Graph Provided: {graph_method}.\nSupported Graph Providers{self.__get_supported_graphs()}"
       )
 
     if not hasattr(self, "_graph_method"):
       self._graph_method = {}
-
+    
     if graph_method == "msgraph":
       from threemystic_common.domain.graph.msgraph import graph_msgraph as graph
       self._graph_method[graph_method] = graph(
-        config = graph_config
+        main_reference= self._main_reference,
+        *args, **kwargs
       )
 
   def graph(self, graph_method, unset = False, *args, **kwargs):
     if(unset):
       if graph_method is None:
         self._unset("_graph_method")
         return
       if hasattr(self, "_graph_method"):
         if self._graph_method.get(graph_method) is not None:
           self._graph_method.pop(graph_method)
 
       return    
     
     graph_method = graph_method.lower() if graph_method is not None else ""
-    if not hasattr(self, "_graph_method"):
+    if hasattr(self, "_graph_method"):
       if self._graph_method.get(graph_method) is not None:
         return self._graph_method[graph_method]
    
-    raise self._main_reference.exception().exception(
-      exception_type = "generic"
-    ).not_implemented(
-      logger = self.get_logger(),
-      name = "graph_method",
-      message = f"Graph not inited: {graph_method}.\nPlease run init_graph}"
-    )
+    self.init_graph(graph_method= graph_method, *args, **kwargs)
+    return self.graph(graph_method= graph_method, *args, **kwargs)
```

### Comparing `threemystic_common-0.0.3/threemystic_common/domain/graph/config/msgraph.py` & `threemystic_common-0.1.0/threemystic_common/domain/graph/config/msgraph.py`

 * *Files identical despite different names*

### Comparing `threemystic_common-0.0.3/threemystic_common/domain/hashicorp/common.py` & `threemystic_common-0.1.0/threemystic_common/domain/hashicorp/common.py`

 * *Files identical despite different names*

### Comparing `threemystic_common-0.0.3/threemystic_common/domain/helpers/app.py` & `threemystic_common-0.1.0/threemystic_common/domain/helpers/app.py`

 * *Files identical despite different names*

### Comparing `threemystic_common-0.0.3/threemystic_common/domain/helpers/config.py` & `threemystic_common-0.1.0/threemystic_common/domain/helpers/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,24 +13,24 @@
 
   # load_defaults_config
   def load(self, config_type = "yaml", *args, **kwargs):
     if self._main_reference.helper_type().string().is_null_or_whitespace(config_type):
       raise self._main_reference.exception().exception(
         exception_type = "argument"
       ).type_error(
-        logger = self.get_logger(),
+        logger = self._main_reference.get_common().get_logger(),
         name = "config_type",
         message = f"config_type is either None or an empty string"
       )
     
     if config_type.lower() not in self._get_known_config_types():
       raise self._main_reference.exception().exception(
         exception_type = "generic"
       ).not_implemented(
-        logger = self.get_logger(),
+        logger = self._main_reference.get_common().get_logger(),
         name = "config_type",
         message = f"config_type not known, known values: {self._get_known_config_types()}"
       )
     
     if config_type.lower() == "config":
       return self._load_defaults_config_config(config_type= config_type, *args, **kwargs)
     
@@ -48,20 +48,20 @@
       return path.joinpath(config_name)
     
     if not self._main_reference.helper_path().is_file(path=path):
       return None
       
     return path
 
-  def _load_defaults_config_config(self, path, config_key = None, config_name = None, *args, **kwargs):
+  def _load_defaults_config_config(self, path, *args, **kwargs):
     config_parser = configparser.ConfigParser()
-    if self._main_reference.helper_type().string().is_null_or_whitespace(path) or self._main_reference.helper_type().string().is_null_or_whitespace(config_key) or self._main_reference.helper_type().string().is_null_or_whitespace(config_name):
+    if self._main_reference.helper_type().string().is_null_or_whitespace(path):
       return config_parser
     
-    config_path = Path(f'{path}/{config_key}/{config_name}').resolve()
+    config_path = self._main_reference.helper_path().get(path=path )
     if not config_path.exists():
       return config_parser
 
     with config_path.open("r") as config_stream:
       config_parser.read_file(config_stream)
     
     return config_parser
```

### Comparing `threemystic_common-0.0.3/threemystic_common/domain/helpers/json.py` & `threemystic_common-0.1.0/threemystic_common/domain/helpers/json.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import json
 from datetime import datetime
 from zoneinfo import ZoneInfo
 
 import dateutil.tz as dateutil_tz
+import decimal
 from threemystic_common.base_class.base_common import base
 
 
 class helper_json(base): 
   """This is a set of library wrappers to help around expending json libary"""
 
   def __init__(self, *args, **kwargs) -> None:
@@ -21,35 +22,40 @@
   # json_dumps_serializable_default
   def serializable_default(self, data, *args, **kwargs):
     if self._main_reference.helper_type().general().is_type(data, datetime) or self._main_reference.helper_type().general().is_type(data, type(datetime.now().time())):
       return data.isoformat()
 
     if self._main_reference.helper_type().general().is_type(data, [ dateutil_tz.tz.tzutc,  dateutil_tz.tz.tzlocal, ZoneInfo]):
       return self.__get_offset_from_zoneinfo(data)
+    
+    if self._main_reference.helper_type().general().is_type(data, decimal.Decimal):
+      return str(data)
     try:
       json.dumps(data)
     except:
       if hasattr(data, "__dict__"):
         return data.__dict__
       raise
 
     return data
 
   def dumps(self, data, default_encoder_function = None, *args, **kwargs):   
-    return json.dumps(data, default= self.serializable_default if default_encoder_function is None else default_encoder_function)
+    if kwargs.get("default") is None:
+      kwargs["default"] = self.serializable_default if default_encoder_function is None else default_encoder_function
+    return json.dumps(data, **kwargs)
   
   def loads(self, data, return_empty_on_null = True,  *args, **kwargs):   
     if data is None:
       return {} if return_empty_on_null else None
 
     if not self._main_reference.helper_type().general().is_type(data, str):
       raise self._main_reference.exception().exception(
         exception_type = "argument"
       ).type_error(
-        logger = self.get_logger(),
+        logger = self._main_reference.get_common().get_logger(),
         name = "data",
         message = f"attribute is not of type string - {type(data)}"
       )
 
     return json.loads(data)
 
   def load_file(self, path, return_empty_on_null = True, *args, **kwargs):
```

### Comparing `threemystic_common-0.0.3/threemystic_common/domain/helpers/parallel_processing.py` & `threemystic_common-0.1.0/threemystic_common/domain/helpers/parallel_processing.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 class helper_parallel_processing(base): 
   """This is a set of library wrappers to help around expending json libary"""
 
   def __init__(self, *args, **kwargs) -> None:
     super().__init__(logger_name= f"helper_parallel_processing", *args, **kwargs)
   
-  async def ensure_all_tasks_complete(self, done_function, done_function_params, total_tasks = None, current_running_total = None, verbose = True):
+  async def ensure_all_tasks_complete(self, done_function, done_function_params, total_tasks = None, current_running_total = None, verbose = False):
     running_done_count = current_running_total if current_running_total is not None else 0
     
     return_data = None
     pending_tasks = None
     process_result_data = []
     while pending_tasks is None or len(pending_tasks) > 0:
       await asyncio.sleep(.5)
```

### Comparing `threemystic_common-0.0.3/threemystic_common/domain/helpers/path.py` & `threemystic_common-0.1.0/threemystic_common/domain/helpers/type/bool.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,91 +1,65 @@
-from pathlib import Path  
 from threemystic_common.base_class.base_common import base
 
-class helper_path(base): 
-  """This is a set of library wrappers to help around expending json libary"""
+
+class helper_type_bool(base): 
+  """This is a set of library wrappers to help around expending bool libary"""
 
   def __init__(self, *args, **kwargs) -> None:
-    super().__init__(logger_name= f"helper_path", *args, **kwargs)
+    super().__init__(logger_name= f"helper_type_bool", *args, **kwargs)
+  
+  def is_true_values(self, *args, **kwargs):
+    return ["true", "t", "yes", "y", "1"]
   
-  # report_directory
-  def get(self, path = None, *args, **kwargs)->Path:
-    if path is None:
-      return None
-    if self._main_reference.helper_type().general().is_type(path, Path):
-      return path
+  def is_false_values(self, *args, **kwargs):
+    return ["false", "f", "no", "n", "0"]
 
-    if not self._main_reference.helper_type().general().is_type(path, str):
-      raise self._main_reference.exception().exception(
-        exception_type = "argument"
-      ).type_error(
-        logger = self.get_logger(),
-        name = "path",
-        message = f"Unknown type ({type(path)})"
-      )
+  def is_bool(self, check_value, *args, **kwargs):
+    return self.is_true(check_value= check_value) or self.is_false(check_value= check_value)
+
+  def is_true(self, check_value, *args, **kwargs):
+    if self._main_reference.helper_type().general().is_type(check_value, bool):
+      return check_value == True
+    
+    if self._main_reference.helper_type().general().is_type(check_value, int):
+      return check_value > 0
     
-    if self._main_reference.helper_type().string().is_null_or_whitespace(path):
+    if not self._main_reference.helper_type().general().is_type(check_value, str):
+      if check_value is None:
+        return False
       raise self._main_reference.exception().exception(
         exception_type = "argument"
       ).type_error(
-        logger = self.get_logger(),
-        name = "path",
-        message = f"path is either None or an empty string"
+        logger = self._main_reference.get_logger(),
+        name = "check_value",
+        message = f"Unknown type for comparison ({type(check_value)})"
       )
+
+    check_value = check_value.lower()
+    if check_value in self.is_true_values():
+      return True
     
-    return Path(path)
-  
-  def expandpath_user(self, path) -> Path:
-    if self._main_reference.helper_type().general().is_type(path, Path):
-      return path
-    return self.get(path).expanduser()
-  
-  def path_exists(self, path):
-    if self._main_reference.helper_type().general().is_type(path, Path):
-      return path.exists()
+    return False
 
-    if not self._main_reference.helper_type().general().is_type(path, str):
-      raise self._main_reference.exception().exception(
-        exception_type = "argument"
-      ).type_error(
-        logger = self.get_logger(),
-        name = "path",
-        message = f"path is not a string or Path type"
-      )  
+  def is_false(self, check_value, *args, **kwargs):
+    if self._main_reference.helper_type().general().is_type(check_value, bool):
+      return check_value == True
+    
+    if self._main_reference.helper_type().general().is_type(check_value, int):
+      return check_value > 0
     
-    if self._main_reference.helper_type().string().is_null_or_whitespace(path):
+    if not self._main_reference.helper_type().general().is_type(check_value, str):
+      if check_value is None:
+        return True
       raise self._main_reference.exception().exception(
         exception_type = "argument"
       ).type_error(
-        logger = self.get_logger(),
-        name = "path",
-        message = f"path is either None or an empty string"
+        logger = self._main_reference.get_logger(),
+        name = "check_value",
+        message = f"Unknown type for comparison ({type(check_value)})"
       )
 
-    path = self.get(path= path)
-    if path is None: 
-      return False
-
-    return path.exists()
-
-  def is_file(self, path):
-    path = self.get(path= path)
-    if path is None: 
-      return False
-
-    if not path.exists(): 
-      return False
-
-    return Path.is_file(self.get(path= path))
-  
-  def is_dir(self, path):
-    path = self.get(path= path)
-    if path is None: 
-      return False
-
-    if not path.exists(): 
-      return False
-
-    return Path.is_dir(self.get(path= path))
-  
-  
+    check_value = check_value.lower()
+    if check_value in self.is_false_values():
+      return True
     
+    return False
```

### Comparing `threemystic_common-0.0.3/threemystic_common/domain/helpers/yaml.py` & `threemystic_common-0.1.0/threemystic_common/domain/helpers/yaml.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import yaml
+import ruamel.yaml as yaml
 
 from threemystic_common.base_class.base_common import base
 
 
 class helper_yaml(base): 
   """This is a set of library wrappers to help around expending json libary"""
 
@@ -19,15 +19,15 @@
     if data is None:
       return {} if return_empty_on_null else None
 
     if not self._main_reference.helper_type().general().is_type(data, str):
       raise self._main_reference.exception().exception(
         exception_type = "argument"
       ).type_error(
-        logger = self.get_logger(),
+        logger = self._main_reference.get_common().get_logger(),
         name = "data",
         message = f"attribute is not of type string - {type(data)}"
       )
     from io import StringIO
     yaml_stream = StringIO(data)
     return self._load_stream(yaml_stream= yaml_stream, multiple_documents= multiple_documents, use_safe= use_safe)
```

### Comparing `threemystic_common-0.0.3/threemystic_common/domain/helpers/type/common.py` & `threemystic_common-0.1.0/threemystic_common/domain/helpers/type/common.py`

 * *Files 12% similar despite different names*

```diff
@@ -26,14 +26,42 @@
       return self._general
     
     from threemystic_common.domain.helpers.type.general import helper_type_general as helper
     self._general = helper(
       main_reference= self._main_reference
     )
     return self.general(*args, **kwargs)
+  
+  def requests(self, unset = False, *args, **kwargs):
+    if(unset):
+      self._unset("_requests")
+      return
+
+    if hasattr(self, "_requests"):
+      return self._requests
+    
+    from threemystic_common.domain.helpers.type.requests import helper_type_requests as helper
+    self._requests = helper(
+      main_reference= self._main_reference
+    )
+    return self.requests(*args, **kwargs)
+  
+  def int(self, unset = False, *args, **kwargs):
+    if(unset):
+      self._unset("_int")
+      return
+
+    if hasattr(self, "_int"):
+      return self._int
+    
+    from threemystic_common.domain.helpers.type.int import helper_type_int as helper
+    self._int = helper(
+      main_reference= self._main_reference
+    )
+    return self.int(*args, **kwargs)
 
   def string(self, unset = False, *args, **kwargs):
     if(unset):
       self._unset("_string")
       return      
     
     if hasattr(self, "_string"):
```

### Comparing `threemystic_common-0.0.3/threemystic_common/domain/helpers/type/datetime.py` & `threemystic_common-0.1.0/threemystic_common/domain/helpers/type/datetime.py`

 * *Files 22% similar despite different names*

```diff
@@ -15,29 +15,42 @@
   
   # get_utc_datetime
   # get_utc
   def get(self, time_zone = "utc", *args, **kwargs):    
     utc = self.convert_to_utc(dt=datetime.utcnow(), default_utctime= True)
     return self.convert_time_zone(dt= utc, time_zone= time_zone)
   
+  def time_delta(self, microseconds = 0, milliseconds= 0, seconds = 0, minutes =0, hours = 0, days = 0, weeks = 0, time_zone="utc", *args, **kwargs):    
+    return timedelta(
+      microseconds= microseconds,milliseconds= milliseconds,
+      seconds= seconds, minutes= minutes, hours= hours,
+      days= days, weeks= weeks )
+  
+  def time_delta_seconds(self, total_seconds = 300, time_zone="utc", *args, **kwargs):    
+    return self.time_delta(
+      total_seconds= total_seconds,
+      time_zone= time_zone,
+      *args, **kwargs
+    )
+  
   def get_epoch(self, *args, **kwargs):    
-    return datetime.utcfromtimestamp(0)
+    return self.convert_to_utc(dt= datetime.utcfromtimestamp(0))
 
   # convert_datetime_utc
   def convert_to_utc(self, dt, default_utctime = True, *args, **kwargs):   
     if dt.tzinfo is None:
       dt = (dt.replace(tzinfo=dateutil_tz.tzutc() if default_utctime else dateutil_tz.tzlocal()))
           
     return dt.astimezone(dateutil_tz.tzutc())
   
-  def datetime_as_string(self, datetime_format = "%Y%M%d%H%M%S", datetime_to_format = None, *args, **kwargs):    
-    if datetime_to_format is None:
-      datetime_to_format = self.get()
+  def datetime_as_string(self, dt_format = "%Y%m%d%H%M%S", dt = None, time_zone="utc", *args, **kwargs):    
+    if dt is None:
+      dt = self.get(time_zone= time_zone)
     
-    return datetime_to_format.strftime(datetime_format)
+    return dt.strftime(dt_format)
   
   # get_tzinfo_from_datetime
   def get_tzinfo(self, check_datetime, default_tz, *args, **kwargs):
     
     if check_datetime.tzinfo is not None:
       return check_datetime.tzinfo
     
@@ -68,15 +81,20 @@
   def convert_time_24hours(self, time_str, error_missing_ampm= False, *args, **kwargs):   
     is_am = False
     if time_str[-2].lower() == "am" or time_str[-1].lower() == "a":
       is_am = True
     
     if not is_am and time_str[-2].lower() != "pm" and time_str[-1].lower() != "p":
       if error_missing_ampm:
-        raise Exception("missing am/pm indicator")
+        raise self._main_reference.exception().exception(
+        exception_type = "generic"
+        ).type_error(
+          logger = self._main_reference.get_common().get_logger(),
+          message = f"missing am/pm indicator"
+        )
       return time_str
     
     time_parts = self._main_reference.helper_type().string().split(string_value=time_str.rstrip(" amp"), separator=":")
     for idx,part in enumerate(time_parts):
       time_parts[idx]=int(part)
     
     if not is_am:
@@ -87,29 +105,55 @@
     
     if len(time_parts) <3:
       time_parts.append("00")
     
     return ":".join(time_parts)
       
   # get_datetime_nearest_minute
-  def get_nearest_minute(self, dt, minute = 15, *args, **kwargs):    
+  def get_nearest_minute(self, dt = None, minute = 15, time_zone= "utc", *args, **kwargs):    
+    if dt is None:
+      dt = self.get(time_zone= time_zone)
+
     return datetime(year=dt.year, month=dt.month, day=dt.day, hour=dt.hour,minute=minute*int(math.floor((dt.minute / minute))), tzinfo= dt.tzinfo)
 
   # get_datetime_nearest_next_minute
-  def get_nearest_next_minute(cls, dt, minute = 15, *args, **kwargs):  
+  def get_nearest_next_minute(self, dt = None, minute = 15, time_zone= "utc", *args, **kwargs):  
+    if dt is None:
+      dt = self.get(time_zone= time_zone)
+
     next_nearest_minute = minute*(int(math.floor((dt.minute / minute)))+ 1)
     if next_nearest_minute < 60:
       return datetime(year=dt.year, month=dt.month, day=dt.day, hour=dt.hour,minute=next_nearest_minute, tzinfo= dt.tzinfo)
     
-    return dt + timedelta(seconds=((next_nearest_minute - dt.minute) * 60))
+    return dt + self.time_delta(seconds=((next_nearest_minute - dt.minute) * 60))
+
+  def datetime_from_string(self, dt_string, dt_format="%Y/%m/%d", *args, **kwargs):    
+    if self._main_reference.helper_type().general().is_type(dt_format, str):
+      try:
+        return self.convert_to_utc(dt= datetime.strptime(dt_string, dt_format ))
+      except:
+        return None
+    
+    if self._main_reference.helper_type().general().is_type(dt_format, list):
+      for format in dt_format:
+        try:
+          format_value = self.datetime_from_string(dt_string= dt_string, dt_format=format)
+          if format_value is not None:
+            return format_value
+        except:
+          continue
+
+    return None
+    
 
   # parse_datetime_iso
   def parse_iso(self, iso_datetime_str, *args, **kwargs):    
-    if iso_datetime_str.lower()[-1] == "Z":
+    if self._main_reference.helper_type().string().set_case(string_value= iso_datetime_str, case= "lower")[-1] == "z":
       iso_datetime_str = f"{iso_datetime_str[0:len(iso_datetime_str) - 1]}+00:00"
+    
     return datetime.fromisoformat(iso_datetime_str)
 
   # convert_datetime_utc
   def convert_utc(self, dt, default_utctime = True):   
     if dt.tzinfo is None:
       dt = (dt.replace(tzinfo=dateutil_tz.tzutc() if default_utctime else dateutil_tz.tzlocal()))
           
@@ -125,31 +169,31 @@
       return dt
 
     dt =  dt.replace(tzinfo=self.get_time_zone(time_zone))
     return dt
 
 
   # convert_datetime
-  def convert_time_zone(self, dt = None, time_zone = None, base_time_zone = "utc", *args, **kwargs):    
+  def convert_time_zone(self, dt = None, time_zone = "utc", base_time_zone = "utc", *args, **kwargs):    
     if dt is None:
-      dt = self.get()
+      dt = self.get(time_zone= time_zone)
     
     dt_time_zone = self.get_tzinfo(check_datetime= dt, default_tz= base_time_zone)
     self.set_tzinfo(dt= dt, time_zone=dt_time_zone, force_replace= True)
     time_zone = self.get_time_zone(time_zone= time_zone)
     return dt.astimezone(time_zone) 
 
   # remove_tzinfo_datetime
   def remove_tzinfo(self, dt, default_utctime = True, *args, **kwargs):         
     return self.convert_to_utc(dt= dt, default_utctime= default_utctime).replace(tzinfo=None)
 
   # convert_datetime_local
-  def convert_local(self, dt, *args, **kwargs):
+  def convert_local(self, dt, time_zone= "utc", *args, **kwargs):
     if dt is None:
-      dt = self.get()
+      dt = self.get(time_zone= time_zone)
     
     dt_time_zone = self.get_tzinfo(check_datetime= dt, default_tz= None)
     self.set_tzinfo(dt= dt, time_zone=dt_time_zone, force_replace= True)
     return self.convert_time_zone(
       dt= dt,
       time_zone = "local"
     )
@@ -165,26 +209,56 @@
 
   # datetime_ticks
   def ticks(self, dt, tick_startdate = datetime(year= 1, month= 1, day= 1, hour= 0, minute= 0, tzinfo= dateutil_tz.tzutc()), *args, **kwargs):
     return self.datetime_ticks_as_seconds(dt= dt, tick_startdate= tick_startdate) * 10**7
   
   # isTokenExpired_Now
   def is_token_expired_now(self, compare_datetime, buffer_delta = timedelta(seconds=300)):   
-    return (self.convert_utc(compare_datetime) <= (self.convert_utc(datetime.now()) + buffer_delta))
+    return (self.convert_utc(compare_datetime) <= (self.convert_utc(self.get(time_zone= "local")) - buffer_delta))
 
   # isTokenExpired_Duration
-  def is_token_expired(self, token_life_duration, start_time = None, buffer_delta = timedelta(seconds=60), *args, **kwargs):  
+  def is_token_expired(self, token_life_duration, start_time = None, buffer_delta = timedelta(seconds=60), time_zone= "utc", *args, **kwargs):  
     if start_time is None:
-      start_time = self.get()
-    return (start_time + token_life_duration) <= (self.get() + buffer_delta)
+      start_time = self.get(time_zone= time_zone)
+    return (start_time + token_life_duration) <= (self.get(time_zone= time_zone - buffer_delta))
   
   # isTokenExpiredEpoch_Duration
-  def is_token_expired_epoch(self, token_life_duration, start_time = None, buffer_delta = timedelta(seconds=300), *args, **kwargs):  
+  def is_token_expired_epoch(self, token_life_duration, start_time = None, buffer_delta = timedelta(seconds=300), time_zone= "utc", *args, **kwargs):  
     if start_time is None:
       start_time = self.get_epoch()
-    return (start_time + token_life_duration) <= (datetime.utcnow() + buffer_delta)
+    return self.token_expired_epoch(token_life_duration= token_life_duration, start_time= start_time) <= (self.get(time_zone= time_zone) - buffer_delta)
   
   # GetTokenExpiredEpoch_Duration
-  def GetTokenExpiredEpoch_Duration(self, token_life_duration, start_time = None):  
+  def token_expired_epoch(self, token_life_duration, start_time = None, *args, **kwargs):  
     if start_time is None:
       start_time = self.get_epoch()
-    return (start_time + token_life_duration)
+    return (start_time + token_life_duration)
+  
+  def get_month_as_2digits(self, month, *args, **kwargs):  
+    if int(month) < 10:
+      return f'0{month}'
+    
+    return month
+
+  def get_day_as_2digits(self, day, *args, **kwargs):  
+    if int(day) < 10:
+      return f'0{day}'
+    
+    return day
+  
+  def yesterday(self, dt = None, *args, **kwargs):  
+    if dt is None:
+      dt = self.get(*args, **kwargs)
+    return (dt - timedelta(days= 1))
+  
+  def last_day_month(self, month, *args, **kwargs):  
+    year = self.get().year
+    month = int(month) + 1
+    if month > 12:
+      month = 1
+      year = (year) + 1
+
+    dt = self.datetime_from_string(f"{year}/{self.get_month_as_2digits(month= month)}/01")
+    return (dt - timedelta(days= 1))
+  
+  def last_day_month_day(self, month, *args, **kwargs):      
+    return self.last_day_month(month= month).day
```

### Comparing `threemystic_common-0.0.3/threemystic_common/domain/helpers/type/dictionary.py` & `threemystic_common-0.1.0/threemystic_common/domain/helpers/type/dictionary.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -61,8 +61,8 @@
             item = self._main_reference.helper_type().list().unique_list(item)
           dict2_copy.pop(key, None)
           
         continue
       
     update_dictionary.update(dict2_copy)
     
-    return update_dictionary
+    return update_dictionary
```

### Comparing `threemystic_common-0.0.3/threemystic_common/domain/helpers/type/general.py` & `threemystic_common-0.1.0/threemystic_common/domain/helpers/type/general.py`

 * *Files 23% similar despite different names*

```diff
@@ -46,8 +46,38 @@
   def copy_object(self, object_copy, deep_copy = True, *args, **kwargs):
     if object_copy is None:
       return None
 
     if deep_copy:
       return copy.deepcopy(object_copy)
     
-    return copy.copy(object_copy)
+    return copy.copy(object_copy)
+  
+  
+
+  def get_container_value(self, container, value_key, *args, **kwargs):
+    if self.get_common().helper_type().general().is_type(value_key, str):
+      if hasattr(container, value_key):
+        return getattr(container, value_key)
+      if value_key in container:
+        return container[value_key]
+      
+      return None
+    
+    if not self.get_common().helper_type().general().is_type(value_key, list):
+      raise self.get_common().exception().exception(
+        exception_type = "argument"
+      ).not_implemented(
+        logger = self.get_common().get_logger(),
+        name = "value_key",
+        message = f"value_key must be either a string or an array. Got Type: {type(value_key)}"
+      )
+    
+    if len(value_key) < 1:
+      return None
+    
+    for key_value in value_key:
+      container = self.get_container_value(container= container, value_key= key_value, *args, **kwargs)
+      if container is None:
+        return container
+
+    return container
```

### Comparing `threemystic_common-0.0.3/threemystic_common/domain/helpers/type/list.py` & `threemystic_common-0.1.0/threemystic_common/domain/helpers/type/list.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,79 +13,76 @@
     
     if return_empty:
       return []
     
     raise self._main_reference.exception().exception(
       exception_type = "argument"
     ).type_error(
-      logger = self.get_logger(),
+      logger = self._main_reference.get_common().get_logger(),
       name = "data",
       message = f"Data is None"
     )
   def unique_list(self, data, *args, **kwargs):
     if len(data) < 2:
       return data
       
     unique_data = {}
     for item in data:
       unique_data[self._main_reference.encryption().hash(hash_method="sha1").generate_hash(self._main_reference.helper_json().dumps(data= item))] = item
 
     return [ val for val in unique_data.values()]
   
-  def __flatten(self, data, flatten_list, *args, **kwargs):
-    if self._main_reference.helper_type().general().is_type(data, list):
+  def __flatten(self, data, flatten_list, recursive= True, *args, **kwargs):
+    if not self._main_reference.helper_type().general().is_type(data, list):
       raise self._main_reference.exception().exception(
         exception_type = "argument"
       ).type_error(
-        logger = self.get_logger(),
+        logger = self._main_reference.get_common().get_logger(),
         name = "data",
         message = f"Unknown type: {type(data)}\n expected list"
       )
-    
-    flatten_list = []
 
     for item in data:
-      if self._main_reference.helper_type().general().is_type(item, list):
-        self.flatten(data = item, flatten_list = flatten_list)
+      if self._main_reference.helper_type().general().is_type(item, list) and recursive:
+        flatten_list += self.flatten(data = item, flatten_list = flatten_list, recursive= recursive)
         continue
       
       flatten_list.append(item)
     
     return flatten_list
 
-  def flatten(self, data, *args, **kwargs):
-    if self._main_reference.helper_type().general().is_type(data, list):
+  def flatten(self, data, recursive= True, *args, **kwargs):
+    if not self._main_reference.helper_type().general().is_type(data, list):
       raise self._main_reference.exception().exception(
         exception_type = "argument"
       ).type_error(
-        logger = self.get_logger(),
+        logger = self._main_reference.get_common().get_logger(),
         name = "data",
         message = f"Unknown type: {type(data)}\n expected list"
       )
     
-    flatten_list = []
-    return self.__flatten(data= data, flatten_list= flatten_list)
+    return self.__flatten(data= data, flatten_list= [], recursive= recursive)
   
   # flatten_array_length
   def flatten_length(self, *args, **kwargs):
     # this shouldn't be needed I Can just do a len off the flatten
     raise self._main_reference.exception().exception(
       exception_type = "function"
     ).exception(
-        logger = self.get_logger(),
+        logger = self._main_reference.get_common().get_logger(),
       name = "flatten_length",
       message = f"Not Needed"
     )
   
   def array_chucked(self, data, chunk_size):
     if self._main_reference.helper_type().general().is_type(data, list):
       raise self._main_reference.exception().exception(
         exception_type = "argument"
       ).type_error(
-        logger = self.get_logger(),
+        logger = self._main_reference.get_common().get_logger(),
         name = "data",
         message = f"Unknown type: {type(data)}\n expected list"
       )
     
     return [data[index:index + chunk_size] for index in range(0, len(data), chunk_size)]
 
   # FindListItem
```

### Comparing `threemystic_common-0.0.3/threemystic_common/domain/helpers/type/logging.py` & `threemystic_common-0.1.0/threemystic_common/domain/helpers/type/logging.py`

 * *Files identical despite different names*

### Comparing `threemystic_common-0.0.3/threemystic_common/domain/helpers/type/regex.py` & `threemystic_common-0.1.0/threemystic_common/domain/helpers/type/regex.py`

 * *Files identical despite different names*

### Comparing `threemystic_common-0.0.3/.gitignore` & `threemystic_common-0.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `threemystic_common-0.0.3/LICENSE` & `threemystic_common-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `threemystic_common-0.0.3/README.md` & `threemystic_common-0.1.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # 3mystic_common
 A set of common files that are used for the various projects under 3 Mystic Apes
 
 # Install
 
 ## pip
 
-This project is currently designed to be installed via pip
+This project is currently designed to be installed via pip <br/>
 pip install https://github.com/3MysticApes/3mystic_common
 
 Once installed you will get the following command:
 3mystic_common
 
 The above command currently just lets you know the scripts have been installed and are usable for reference. It also will let you know what version of the toolset is installed.
```

### Comparing `threemystic_common-0.0.3/hatch.toml` & `threemystic_common-0.1.0/hatch.toml`

 * *Files identical despite different names*

### Comparing `threemystic_common-0.0.3/pyproject.toml` & `threemystic_common-0.1.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -23,30 +23,32 @@
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
   "colorama; platform_system == 'Windows'",
+  "ruamel.yaml >= 0.17.31",
   "asyncio >= 3.4.3",
   "python-dateutil >= 2.8.2",
   "openpyxl >= 3.0.9",
   "pycryptodomex >= 3.14.1",
   "requests >= 2.27.1",
   "cryptography >= 38.0.3",
-  "typing-extensions >= 4.4.0"
+  "typing-extensions >= 4.4.0",
+  "pathvalidate >= 3.0.0"
 ]
 dynamic = ["version"]
 
 [project.urls]
 "Homepage" = "https://github.com/3MysticApes/3mystic_common"
 "Bug Tracker" = "https://github.com/3MysticApes/3mystic_common/issues"
 
-[project.scripts]
-3mystic_common = "threemystic_common.cli:main"
+# [project.scripts]
+# 3mystic_common = "threemystic_common.cli:main"
 
 [tool.hatch.version]
 path = "threemystic_common/__version__.py"
 
 [tool.hatch.build.targets.sdist]
 exclude = [
   "/.github",
```

### Comparing `threemystic_common-0.0.3/PKG-INFO` & `threemystic_common-0.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: threemystic-common
-Version: 0.0.3
+Version: 0.1.0
 Summary: Common Library for for various tool sets
 Project-URL: Homepage, https://github.com/3MysticApes/3mystic_common
 Project-URL: Bug Tracker, https://github.com/3MysticApes/3mystic_common/issues
 Author: Ron Truex
 License-Expression: MIT
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
@@ -17,28 +17,30 @@
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.8
 Requires-Dist: asyncio>=3.4.3
 Requires-Dist: colorama; platform_system == 'Windows'
 Requires-Dist: cryptography>=38.0.3
 Requires-Dist: openpyxl>=3.0.9
+Requires-Dist: pathvalidate>=3.0.0
 Requires-Dist: pycryptodomex>=3.14.1
 Requires-Dist: python-dateutil>=2.8.2
 Requires-Dist: requests>=2.27.1
+Requires-Dist: ruamel-yaml>=0.17.31
 Requires-Dist: typing-extensions>=4.4.0
 Description-Content-Type: text/markdown
 
 # 3mystic_common
 A set of common files that are used for the various projects under 3 Mystic Apes
 
 # Install
 
 ## pip
 
-This project is currently designed to be installed via pip
+This project is currently designed to be installed via pip <br/>
 pip install https://github.com/3MysticApes/3mystic_common
 
 Once installed you will get the following command:
 3mystic_common
 
 The above command currently just lets you know the scripts have been installed and are usable for reference. It also will let you know what version of the toolset is installed.
```

