# Comparing `tmp/threemystic_cloud_client-0.0.2.tar.gz` & `tmp/threemystic_cloud_client-0.1.0.tar.gz`

## Comparing `threemystic_cloud_client-0.0.2.tar` & `threemystic_cloud_client-0.1.0.tar`

### file list

```diff
@@ -1,22 +1,38 @@
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.0.2/threemystic_cloud_client/__main__.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.0.2/threemystic_cloud_client/__version__.py
--rw-r--r--   0        0        0     2079 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.0.2/threemystic_cloud_client/cloud_client.py
--rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.0.2/threemystic_cloud_client/base_class/base.py
--rw-r--r--   0        0        0     1902 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.0.2/threemystic_cloud_client/cli/__init__.py
--rw-r--r--   0        0        0     2145 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.0.2/threemystic_cloud_client/cli/actions/config/__init__.py
--rw-r--r--   0        0        0     3001 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.0.2/threemystic_cloud_client/cloud_providers/aws/__init__.py
--rw-r--r--   0        0        0     9109 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.0.2/threemystic_cloud_client/cloud_providers/aws/base_class/base.py
--rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.0.2/threemystic_cloud_client/cloud_providers/aws/config/base.py
--rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.0.2/threemystic_cloud_client/cloud_providers/aws/config/step_1.py
--rw-r--r--   0        0        0    14232 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.0.2/threemystic_cloud_client/cloud_providers/aws/config/step_2.py
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.0.2/threemystic_cloud_client/cloud_providers/azure/__init__.py
--rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.0.2/threemystic_cloud_client/cloud_providers/base_class/base.py
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.0.2/threemystic_cloud_client/domain/aws/client_sso.py
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.0.2/threemystic_cloud_client/domain/aws/controller.py
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.0.2/threemystic_cloud_client/domain/azure/client.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.0.2/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.0.2/LICENSE
--rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.0.2/README.md
--rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.0.2/hatch.toml
--rw-r--r--   0        0        0     2949 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     2020 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.0/threemystic_cloud_client/__main__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.0/threemystic_cloud_client/__version__.py
+-rw-r--r--   0        0        0     3168 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.0/threemystic_cloud_client/cloud_client.py
+-rw-r--r--   0        0        0     4011 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.0/threemystic_cloud_client/cli/__init__.py
+-rw-r--r--   0        0        0     2519 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.0/threemystic_cloud_client/cli/actions/base_class/base.py
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.0/threemystic_cloud_client/cli/actions/config/__init__.py
+-rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.0/threemystic_cloud_client/cli/actions/test/__init__.py
+-rw-r--r--   0        0        0     4074 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.0/threemystic_cloud_client/cli/actions/token/__init__.py
+-rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.0/threemystic_cloud_client/cloud_providers/aws/__init__.py
+-rw-r--r--   0        0        0     3591 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.0/threemystic_cloud_client/cloud_providers/aws/base_class/base.py
+-rw-r--r--   0        0        0     2045 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.0/threemystic_cloud_client/cloud_providers/aws/client/auto_client.py
+-rw-r--r--   0        0        0    12041 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.0/threemystic_cloud_client/cloud_providers/aws/client/sso.py
+-rw-r--r--   0        0        0    21250 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.0/threemystic_cloud_client/cloud_providers/aws/client/base_class/base.py
+-rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.0/threemystic_cloud_client/cloud_providers/aws/config/step_1.py
+-rw-r--r--   0        0        0    15698 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.0/threemystic_cloud_client/cloud_providers/aws/config/step_2.py
+-rw-r--r--   0        0        0     3451 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.0/threemystic_cloud_client/cloud_providers/aws/config/base_class/base.py
+-rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.0/threemystic_cloud_client/cloud_providers/aws/test/step_1.py
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.0/threemystic_cloud_client/cloud_providers/aws/test/step_2.py
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.0/threemystic_cloud_client/cloud_providers/aws/test/base_class/base.py
+-rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.0/threemystic_cloud_client/cloud_providers/azure/__init__.py
+-rw-r--r--   0        0        0    13846 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.0/threemystic_cloud_client/cloud_providers/azure/base_class/base.py
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.0/threemystic_cloud_client/cloud_providers/azure/client/auto_client.py
+-rw-r--r--   0        0        0     1478 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.0/threemystic_cloud_client/cloud_providers/azure/client/cli.py
+-rw-r--r--   0        0        0    13524 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.0/threemystic_cloud_client/cloud_providers/azure/client/base_class/base.py
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.0/threemystic_cloud_client/cloud_providers/azure/config/step_1.py
+-rw-r--r--   0        0        0     2739 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.0/threemystic_cloud_client/cloud_providers/azure/config/base_class/base.py
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.0/threemystic_cloud_client/cloud_providers/azure/test/step_1.py
+-rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.0/threemystic_cloud_client/cloud_providers/azure/test/base_class/base.py
+-rw-r--r--   0        0        0     4923 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.0/threemystic_cloud_client/cloud_providers/base_class/base.py
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.0/threemystic_cloud_client/domain/aws/client_sso.py
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.0/threemystic_cloud_client/domain/aws/controller.py
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.0/threemystic_cloud_client/domain/azure/client.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.0/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.0/LICENSE
+-rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.0/README.md
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.0/hatch.toml
+-rw-r--r--   0        0        0     3287 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2558 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.0/PKG-INFO
```

### Comparing `threemystic_cloud_client-0.0.2/threemystic_cloud_client/cloud_client.py` & `threemystic_cloud_client-0.1.0/threemystic_cloud_client/cloud_client.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,62 +1,81 @@
-from threemystic_cloud_client.base_class.base import base
+from threemystic_common.base_class.base_provider import base
 
 
 class cloud_client(base): 
   """This is a library to help with the interaction with the cloud providers"""
 
   def __init__(self, logger = None, common = None, *args, **kwargs) -> None: 
-    super().__init__(common= common, logger_name= "cloud_client", logger= logger, *args, **kwargs)
+    super().__init__(provider= "", common= common, logger_name= "cloud_client", logger= logger, *args, **kwargs)
     
   def version(self, *args, **kwargs):
     if hasattr(self, "_version"):
       return self._version
     import threemystic_cloud_client.__version__ as __version__
     self._version = __version__.__version__
     return self.version()
     
   def get_supported_providers(self, *args, **kwargs):
-    return ["aws", "azure"]
+    return super().get_supported_providers()
+
+  def __set_provider_azure(self, provider, *args, **kwargs):
+    from threemystic_cloud_client.cloud_providers.azure.client.auto_client import cloud_client_azure_client_auto as client
+    self._client[provider] = client(
+      common= self.get_common(), *args, **kwargs
+    ).get_client()
+  
+  def __set_provider_aws(self, provider, *args, **kwargs):
+    from threemystic_cloud_client.cloud_providers.aws.client.auto_client import cloud_client_aws_client_auto as client
+    self._client[provider] = client(
+      common= self.get_common(), *args, **kwargs
+    ).get_client()
 
   def init_client(self, provider, *args, **kwargs):
-    provider = provider.lower() if provider is not None else ""
+    provider = self.get_common().helper_type().string().set_case(string_value= provider, case= "lower") if provider is not None else ""
 
     if provider not in self.get_supported_providers():
-      raise self.get_common().exception(
-        exception_type = "generic"
+      raise self.get_common().exception().exception(
+        exception_type = "argument"
       ).not_implemented(
-        logger = self.logger,
+        logger = self.get_common().get_logger(),
         name = "provider",
         message = f"Unknown Cloud Provided: {provider}.\nSupported Cloud Providers{self.get_supported_providers()}"
       )
 
     if not hasattr(self, "_client"):
       self._client = {}
 
+    if self._client.get(provider) is not None:
+      return
+
     if provider == "azure":
-      from domain.azure.client import client_azure as client
-      self._client[provider] = client(
-        common= self.get_common()
-      )
+      self.__set_provider_azure(provider= provider)
       return
     
     if provider == "aws":
-      from domain.aws.controller import client_controller as client
-      self._client[provider] = client(
-        common= self.get_common()
-      )
-      return
-
-  def client(self, provider, *args, **kwargs):
-    provider = provider.lower() if provider is not None else ""
-
-    if hasattr(self, "_client"):
-      if self._client.get(provider) is not None:
-        return self._client[provider]
-   
+      self.__set_provider_aws(provider= provider)
+      return  
+       
     raise self.get_common().exception().exception(
-      exception_type = "generic"
+      exception_type = "argument"
     ).not_implemented(
-      logger = self.logger,
+      logger = self.get_common().get_logger(),
       name = "provider",
       message = f"Unknown Cloud Provided: {provider}.\nSupported Cloud Providers{self.get_supported_providers()}"
-    )
+    )
+
+  def client(self, provider, *args, **kwargs):
+    if self.get_common().helper_type().string().is_null_or_whitespace(string_value= provider):
+      raise self.get_common().exception().exception(
+        exception_type = "argument"
+      ).not_implemented(
+        logger = self.get_common().get_logger(),
+        name = "provider",
+        message = f"provider cannot be null or whitespace"
+      )
+  
+    provider = self.get_common().helper_type().string().set_case(string_value= provider, case= "lower")
+    if not hasattr(self, "_client"):
+      self.init_client(provider= provider,  *args, **kwargs)
+      return self.client(provider= provider, *args, **kwargs)
+    
+    return self._client.get(provider)
```

### Comparing `threemystic_cloud_client-0.0.2/threemystic_cloud_client/cli/actions/config/__init__.py` & `threemystic_cloud_client-0.1.0/threemystic_cloud_client/cli/actions/base_class/base.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,45 +1,59 @@
 import sys
+from abc import abstractmethod
 from threemystic_common.base_class.generate_data.generate_data_handlers import generate_data_handlers
 
 
-class cloud_client_config():
-  def __init__(self, cloud_client, *args, **kwargs):
-    self._cloud_client = cloud_client
-
-  def main(self, *args, **kwargs):
-    response = self._cloud_client.get_common().generate_data().generate(
-      generate_data_config = {
-        "provider": {
-            "validation": lambda item: self._cloud_client.get_common().helper_type().string().trim(self._cloud_client.get_common().helper_type().string().set_case(string_value= item, case= "lower")) in self._cloud_client.get_supported_providers(),
-            "messages":{
-              "validation": f"Valid Provider Options: {self._cloud_client.get_supported_providers()}",
-            },
-            "conversion": lambda item: self._cloud_client.get_common().helper_type().string().trim(string_value= self._cloud_client.get_common().helper_type().string().set_case(string_value= item, case= "lower")) if item is not None else None,
-            "desc": f"Which provider should we configure\nvalid options are {self._cloud_client.get_supported_providers()}",
-            "default": None,
-            "handler": generate_data_handlers.get_handler(handler= "base"),
-            "optional": True
-        }
-      }
-    )
+class cloud_client_action_base():
+  def __init__(self, cloud_client = None, *args, **kwargs):
+    self._cloud_client = cloud_client 
+    if self._cloud_client is None:
+      from threemystic_cloud_client.cloud_client import cloud_client
+      self._cloud_client = cloud_client()
+    
     
-    provider = self.__get_provider(response).lower()
+    
+
+  def main(self, provider = None, *args, **kwargs):
+    if self._cloud_client.get_common().helper_type().string().is_null_or_whitespace(string_value= provider):
+      response = self._cloud_client.get_common().generate_data().generate(
+        generate_data_config = {
+          "provider": {
+              "validation": lambda item: self._cloud_client.get_common().helper_type().string().trim(self._cloud_client.get_common().helper_type().string().set_case(string_value= item, case= "lower")) in self._cloud_client.get_supported_providers(),
+              "messages":{
+                "validation": f"Valid Provider Options: {self._cloud_client.get_supported_providers()}",
+              },
+              "conversion": lambda item: self._cloud_client.get_common().helper_type().string().trim(string_value= self._cloud_client.get_common().helper_type().string().set_case(string_value= item, case= "lower")) if item is not None else None,
+              "desc": f"Which provider should we configure\nvalid options are {self._cloud_client.get_supported_providers()}",
+              "default": None,
+              "handler": generate_data_handlers.get_handler(handler= "base"),
+              "optional": True
+          }
+        }
+      )
+      
+      provider = self._cloud_client.get_common().helper_type().string().set_case(string_value= self.__get_provider(response), case= "lower")
     if provider not in self._cloud_client.get_supported_providers():
       return
     
     if provider == "azure":
-      from threemystic_cloud_client.cloud_providers.azure import cloud_client_azure as client
-      client(common= self._cloud_client.get_common()).config()
+      self._process_provider_azure()
 
     
     if provider == "aws":
-      from threemystic_cloud_client.cloud_providers.aws  import cloud_client_aws as client
-      client(common= self._cloud_client.get_common()).config()
+      self._process_provider_aws()
   
+  @abstractmethod
+  def _process_provider_aws(self, *args, **kwargs):
+    pass
+
+  @abstractmethod
+  def _process_provider_azure(self, *args, **kwargs):
+    pass
+
   def __get_provider(self, provider, *args, **kwargs):
     if provider is None:
       return ""
 
     if provider.get("provider") is not None:
       return self.__get_provider(provider= provider.get("provider"))
```

### Comparing `threemystic_cloud_client-0.0.2/threemystic_cloud_client/cloud_providers/aws/__init__.py` & `threemystic_cloud_client-0.1.0/threemystic_cloud_client/cloud_providers/azure/config/base_class/base.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,61 +1,64 @@
-from threemystic_cloud_client.cloud_providers.aws.base_class.base import cloud_client_provider_aws_base as base
+from threemystic_cloud_client.cloud_providers.azure.base_class.base import cloud_client_provider_azure_base as base
 from threemystic_common.base_class.generate_data.generate_data_handlers import generate_data_handlers
-from threemystic_cloud_client.cloud_providers.aws.config.step_1 import cloud_client_aws_config_step_1 as step
 
-
-class cloud_client_aws(base):
+class cloud_client_azure_config_base(base):
   def __init__(self, *args, **kwargs):
-    super().__init__(logger_name= "cloud_client_aws", provider= "aws", *args, **kwargs)
-  
-  # There is not post init when in Config Mode
-  def _post_init(self, *args, **kwargs):
-    pass
+    super().__init__(*args, **kwargs)
 
-  def config(self, *args, **kwargs):
-    cli_doc_link = "https://docs.aws.amazon.com/cli/latest/userguide/getting-started-install.html"
-    ssm_doc_link = "https://docs.aws.amazon.com/systems-manager/latest/userguide/session-manager-working-with-install-plugin.html"
-    saml2aws_doc_link = "https://github.com/Versent/saml2aws"
-
-    
-    config = self._load_config()
-    next_step = step(common= self.get_common(), logger= self.get_logger())
-    print("The aws cli is required for setup.")
-    print()
-    print(f"if you need to install the cli you can goto here: {cli_doc_link}\nIt is also highly recommended to install the ssm plugin here: {ssm_doc_link}")
-    print()
-    print(f"If you are using saml2aws you need to also install {saml2aws_doc_link}")
-    print()
-    print()
-    print("-----------------------------")
-    
-    if config.get("cli_installed") != True:
-      config["cli_installed"] = self._is_aws_installed()
-    
-    if config["cli_installed"] is None:
-      return
+  
+  def update_is_cli_installed(self, is_cli_installed, *args, **kwargs):
+    config = self.get_config()
+    if(config is None):
+      config = {}
     
-    if self.is_cli_installed(config= config) != True:
-      print("Please install the aws cli and if needed saml2aws before continuing")
-      return
+    config["cli_installed"] = is_cli_installed
+
+    self._save_config()
+  
+  def update_sdk_auth(self, sdk_auth = "cli", *args, **kwargs):
+    config = self.get_config()
     
-    next_step.step(config= config)
+    config["sdk_auth"] = sdk_auth
+
+    self._save_config()
+     
+  def step(self, force_cli_installed_prompt = False, *args, **kwargs):
+    
+    if (self.is_cli_installed() != True or force_cli_installed_prompt):   
+      print("The azure cli is required for setup.")
+      print()
+      print(f"if you need to install the cli you can goto here: {self.links['cli_doc_link']}")
+      print("To ensure your base configuration please run: az configure")
+      print()
+      print()
+      print("-----------------------------")
+      
+      self.update_is_cli_installed(is_cli_installed= self._is_azure_installed())
+      self.update_sdk_auth()
+      print("cli state updated")
+      print("-----------------------------")
+      
+      if self.is_cli_installed() != True:
+        print("Please install the azure cli")
+        return False
 
+    return True
 
-  def _is_aws_installed(self):
+  def _is_azure_installed(self):
     response = self.get_common().generate_data().generate(
       generate_data_config = {
         "installed": {
             "validation": lambda item: self.get_common().helper_type().bool().is_bool(check_value= item),
             "messages":{
               "validation": f"Valid options for Yes are: {self.get_common().helper_type().bool().is_true_values()}",
             },
             "conversion": lambda item: self.get_common().helper_type().bool().is_true(check_value= item),
-            "desc": f"Have you already installed the aws cli and saml2aws if needed?\nValid Options: {self.get_common().helper_type().bool().is_true_values()}",
-            "default": False,
+            "desc": f"Have you already installed the azure cli?\nValid Options: {self.get_common().helper_type().bool().is_true_values()}",
+            "default": self.is_cli_installed(),
             "handler": generate_data_handlers.get_handler(handler= "base"),
             "optional": True
         }
       }
     )
 
     
@@ -64,11 +67,8 @@
   def __get_installed(self, installed, *args, **kwargs):
     if installed is None:
       return ""
     
     if installed.get("installed") is not None:
       return self.__get_installed(installed= installed.get("installed"))
     
-    return installed.get("formated") if installed.get("formated") is not None else False
-    
-    
-  
+    return installed.get("formated") if installed.get("formated") is not None else False
```

### Comparing `threemystic_cloud_client-0.0.2/threemystic_cloud_client/cloud_providers/aws/config/step_1.py` & `threemystic_cloud_client-0.1.0/threemystic_cloud_client/cloud_providers/aws/config/step_1.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,22 @@
-from threemystic_cloud_client.cloud_providers.aws.config.base import cloud_client_aws_config_base as base
+from threemystic_cloud_client.cloud_providers.aws.config.base_class.base import cloud_client_aws_config_base as base
 from threemystic_common.base_class.generate_data.generate_data_handlers import generate_data_handlers
-from threemystic_cloud_client.cloud_providers.aws.config.step_2 import cloud_client_aws_config_step_2 as step
+from threemystic_cloud_client.cloud_providers.aws.config.step_2 import cloud_client_aws_config_step_2 as nextstep
 
 
 class cloud_client_aws_config_step_1(base):
   def __init__(self, *args, **kwargs):
-    super().__init__(logger_name= "cloud_client_aws_config_step_1", provider= "aws", *args, **kwargs)
+    super().__init__(logger_name= "cloud_client_aws_config_step_1", *args, **kwargs)
     
 
-  def step(self, config, *args, **kwargs):
+  def step(self, *args, **kwargs):
     
-    if not super().step(config= config):
+    if not super().step(force_cli_installed_prompt= True):
       return
     
-    
     response = self.get_common().generate_data().generate(
       generate_data_config = {
         "type": {
             "validation": lambda item: self.get_common().helper_type().bool().is_bool(check_value= item),
             "messages":{
               "validation": f"Valid options for Yes are: {self.get_common().helper_type().bool().is_true_values()}",
             },
@@ -29,10 +28,10 @@
         }
       }
     )
 
     if response is None:
       return
 
-    step(init_object = self).step(config= config, is_new_config= response["type"].get("formated") == True)
+    nextstep(init_object = self).step(is_new_config= response["type"].get("formated") == True)
```

### Comparing `threemystic_cloud_client-0.0.2/threemystic_cloud_client/cloud_providers/aws/config/step_2.py` & `threemystic_cloud_client-0.1.0/threemystic_cloud_client/cloud_providers/aws/config/step_2.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,273 +1,302 @@
-from threemystic_cloud_client.cloud_providers.aws.config.base import cloud_client_aws_config_base as base
+from threemystic_cloud_client.cloud_providers.aws.config.base_class.base import cloud_client_aws_config_base as base
 from threemystic_common.base_class.generate_data.generate_data_handlers import generate_data_handlers
 import configparser
 
 class cloud_client_aws_config_step_2(base):
   def __init__(self, *args, **kwargs):
-    super().__init__(logger_name= "cloud_client_aws_config_step_2", provider= "aws", *args, **kwargs)
+    super().__init__(logger_name= "cloud_client_aws_config_step_2", *args, **kwargs)
 
-  def step(self, config, is_new_config, *args, **kwargs):
+  def step(self, is_new_config, *args, **kwargs):
 
-    if not super().step(config= config):
+    if not super().step():
       return
 
     if is_new_config:
-      self.__step_new(config= config)
+      self.__step_new()
       return
     
-    self.__step_existing(config= config)
+    self.__step_existing()
 
-  def __get_profile_data_geerationn(self, *args, **kwargs):
-    return {
-      "profile_name": {
-        "validation": lambda item: self.get_common().helper_type().regex().get(pattern= "^[a-z][a-z0-9_-]{1,}$").fullmatch(self.get_common().helper_type().string().trim(string_value= str(item))) if item is not None else False,
-        "messages":{
-          "validation": f"It should be alphanumeric and can have underscores or dashes and must start with a letter and be at lest 2 characters ^[a-z][a-z0-9_-]\{1,}$",
-        },
-        "conversion": lambda item: self.get_common().helper_type().string().trim(string_value= self.get_common().helper_type().string().set_case(string_value= item, case= "lower")) if item is not None else None,
-        "desc": f"Profile Name (it will be converted to all lowercase)\nRequirments: alphanumeric and can have underscores or dashes and must start with a letter and be at lest 2 characters ^[a-z][a-z0-9_-]\{1,}$",
-        "handler": generate_data_handlers.get_handler(handler= "base"),
-        "optional": False
-      }
-    }
-  
-  def __get_response_item(self, key, response, *args, **kwargs):
-    if response is None:
-      return None
-
-    if response.get(key) is not None:
-      return self.__get_response_item(key= key, response= response.get(key))
-    
-    return self.get_common().helper_type().string().set_case(string_value= response.get("formated"), case= "lower")   
-    
-  def __step_existing(self, config, *args, **kwargs):
-    if self.get_existing_profiles(config= config) is None:
-      print("No existing profiles please run new")
-      return
-    
-    response = self.get_common().generate_data().generate(
-      generate_data_config = self.__get_profile_data_geerationn()
-    )
-    
-    profile_name = self.__get_response_item(key= "profile_name", response= response)
+  def __step_new(self, *args, **kwargs):
 
-    if profile_name is None:
+    if not super().step():
       return
     
-    running_config = None
-    for existing_profile_name, existing_config in self.get_existing_profiles(config= config).items():
-      if existing_profile_name == profile_name:
-        running_config = existing_config
-        break
-
-    if running_config is None:
-      print("Profile not found")
-      return
-
-    if running_config.get("auth_method") == "sso":
-      self.__step_process_sso(
-        config= config,
-        profile_name= profile_name,
-        running_config= running_config
-      )
-
-  def __step_new(self, config, *args, **kwargs):
-
-    if not super().step(config= config):
-      return
-    
-    running_config = {}
+    profile_data = {}
     response = self.get_common().generate_data().generate(
       generate_data_config = self.get_common().helper_type().dictionary().merge_dictionary([
         {}, 
-        self.__get_profile_data_geerationn(),
+        self.__get_profile_data_genrationn(),
         {
           "auth_method": {
             "validation": lambda item: self.get_common().helper_type().string().set_case(string_value= item, case= "lower") in self.valid_auth_options(),
             "messages":{
               "validation": f"Valid Options: {self.valid_auth_options()}",
             },
             "conversion": lambda item: self.get_common().helper_type().string().trim(string_value= self.get_common().helper_type().string().trim(string_value= self.get_common().helper_type().string().set_case(string_value= item, case= "lower"))) if item is not None else None,
-            "desc": f"Which provider should we configure\nvalid options are {self.valid_auth_options()}",
+            "desc": f"Which provider authentication\nvalid options are {self.valid_auth_options()}",
             "handler": generate_data_handlers.get_handler(handler= "base"),
             "optional": False
           }
         }
       ])
     )
 
     if response is None:
       return
     
     profile_name = self.__get_response_item(key= "profile_name", response= response)
     if self.get_common().helper_type().string().is_null_or_whitespace(string_value= profile_name):
       print("Profile Name was empty.")
-      return
+      return     
       
-    running_config["auth_method"] = self.__get_response_item(key= "auth_method", response= response)   
-    if self.get_common().helper_type().string().is_null_or_whitespace(string_value= running_config["auth_method"]):
+    profile_data["auth_method"] = self.__get_response_item(key= "auth_method", response= response)   
+    if self.get_common().helper_type().string().is_null_or_whitespace(string_value= profile_data["auth_method"]):
       print("Auth Method was empty.")
       return 
+
+    if(self.config_profile_name_exists(profile_name= profile_name)):
+      response_existing = self.get_common().generate_data().generate(
+        generate_data_config = {
+          "update_existing": {
+            "validation": lambda item: self.get_common().helper_type().bool().is_bool(check_value= item),
+            "allow_empty": True,
+            "messages":{
+              "validation": f"Valid options for Yes are: {self.get_common().helper_type().bool().is_true_values()}\nValid options for No are: {self.get_common().helper_type().bool().is_false_values()}",
+            },
+            "conversion": lambda item: self.get_common().helper_type().bool().is_true(check_value= item),
+            "desc": f"Profile Name {profile_name} already exists.\nDo you want to update the existing profile?\nValid optiond for yes: {self.get_common().helper_type().bool().is_true_values()}{self.__get_existing_text(exiting_value= profile_data.get('default_profile'))}",
+            "handler": generate_data_handlers.get_handler(handler= "base"),
+            "default": False,
+            "optional": True
+          }
+        }
+      )
+      if(self.__get_response_item(key= "update_existing", response= response_existing) == False):
+        print("Please rerun config and use a different profile name")
+        return
+
+      profile_data = self.get_config_profile_name(profile_name= profile_name)
+      profile_data["auth_method"] = self.__get_response_item(key= "auth_method", response= response) 
     
     self.__step_process_sso(
-      config= config,
       profile_name= profile_name,
-      running_config= running_config
+      profile_data= profile_data
+    )
+  
+  def __step_existing(self, *args, **kwargs):
+    if not self.has_config_profiles():
+      print("No existing profiles please run new")
+      return
+    
+    response = self.get_common().generate_data().generate(
+      generate_data_config = self.__get_profile_data_genrationn()
     )
+    
+    profile_name = self.__get_response_item(key= "profile_name", response= response)
+
+    if self.get_common().helper_type().string().is_null_or_whitespace(string_value= profile_name):      
+      print(f"Profile Name was not valid: {profile_name}")
+      return
+    
+    profile_data = self.get_config_profile_name(profile_name= profile_name)
+    
+    if profile_data is None:
+      print("Profile not found")
+      return
+
+    if profile_data.get("auth_method") == "sso":
+      self.__step_process_sso(
+        profile_name= profile_name,
+        profile_data= profile_data
+      )
+
+  def __get_profile_data_genrationn(self, *args, **kwargs):
+    return {
+      "profile_name": {
+        "validation": lambda item: self.get_common().helper_type().regex().get(pattern= "^[a-z][a-z0-9_-]{1,}$").fullmatch(self.get_common().helper_type().string().trim(string_value= str(item))) if item is not None else False,
+        "messages":{
+          "validation": f"It should be alphanumeric and can have underscores or dashes and must start with a letter and be at lest 2 characters ^[a-z][a-z0-9_-]\{1,}$",
+        },
+        "conversion": lambda item: self.get_common().helper_type().string().trim(string_value= self.get_common().helper_type().string().set_case(string_value= item, case= "lower")) if item is not None else None,
+        "desc": f"Profile Name (it will be converted to all lowercase)\nRequirments: alphanumeric and can have underscores or dashes and must start with a letter and be at lest 2 characters ^[a-z][a-z0-9_-]\{1,}$",
+        "handler": generate_data_handlers.get_handler(handler= "base"),
+        "optional": False
+      }
+    }
+  
+  def __get_response_item(self, key, response, *args, **kwargs):
+    if response is None:
+      return None
+
+    if response.get(key) is not None:
+      return self.__get_response_item(key= key, response= response.get(key))
+    
+    return self.get_common().helper_type().string().set_case(string_value= response.get("formated"), case= "lower")   
+    
+  
+
+ 
   
   def __step_process_sso_valid_profile(self, profile_name, existing_profile, *args, **kwargs):
 
     if self.get_common().helper_type().string().is_null_or_whitespace(string_value= profile_name):
       return False if self.get_common().helper_type().string().is_null_or_whitespace(string_value= existing_profile) else True
       
     
     profile_name = self.get_common().helper_type().string().trim(string_value= profile_name)  
     config_parser = configparser.ConfigParser()
-    if(self.get_common().helper_path().path_exists(path= self.aws_config_path())):
-      with self.get_common().helper_path().expandpath_user(path= self.aws_config_path()).open(mode="r") as config_file:
+    if(self.get_common().helper_path().path_exists(path= self.get_aws_user_path_config())):
+      with self.get_common().helper_path().expandpath_user(path= self.get_aws_user_path_config()).open(mode="r") as config_file:
         config_parser.read_file(config_file)
     else:
-      print(f"AWW config path not found: {self.aws_config_path()}")
+      print()
+      print()
+      print("*********************************************************")
+      print(f"AWS config path not found: {self.get_aws_user_path_config()}")
       print("setup will not work until aws is configured")
+      print("*********************************************************")
+      print()
+      print()
+      
       return True
     return config_parser.has_section(f"profile {profile_name}")
 
-  def get_default_default_profile(self, config, profile_name, running_config):
-    if running_config.get("default_profile") == True:
-      return True
+  def get_default_profile_setting(self, profile_name, profile_data):
+    if profile_data is not None:
+      return profile_data.get("default_profile") == True
     
-    if self.get_existing_profiles(config= config) is None:
+    if self.get_default_profile() is None:
       return True
 
-    for profile, details in self.get_existing_profiles(config= config).items():
-      if profile.lower() == profile_name:
-        continue
-
-      if details.get("default_profile") != True:
-        continue
-      
-      return False
+    existing_profile = self.get_config_profile_name(profile_name= profile_name)
+    if(existing_profile is not None):
+      return existing_profile.get("default_profile") == True
+    
     
-    return True
+    return False
     
 
   def __get_existing_text(self, exiting_value):
     return (f"\n(If empty it will use the existing: {exiting_value})"
       if not self.get_common().helper_type().string().is_null_or_whitespace(string_value=exiting_value) else ""
     )
-  def __step_process_sso(self, config, profile_name = None, running_config = {}, *args, **kwargs):
-    
-    existing_sso_profile_name = running_config.get("sso_profile_name")
+
+  def __step_process_sso(self, profile_name = None, profile_data = {}, *args, **kwargs):
+    if(profile_data is None):
+      profile_data = {}
+
+    existing_sso_profile_name = profile_data.get("sso_profile_name")
     
     response = self.get_common().generate_data().generate(
       generate_data_config = {
         "use_cli_profile": {
           "validation": lambda item: self.get_common().helper_type().bool().is_bool(check_value= item),
           "allow_empty": True,
           "messages":{
             "validation": f"Valid options for Yes are: {self.get_common().helper_type().bool().is_true_values()}\nValid options for No are: {self.get_common().helper_type().bool().is_false_values()}",
           },
           "conversion": lambda item: self.get_common().helper_type().bool().is_true(check_value= item),
-          "desc": f"Use preconfigured aws cli sso profile (created with aws configure sso --profile <profile_name>)\nValid optiond for yes: {self.get_common().helper_type().bool().is_true_values()}{self.__get_existing_text(exiting_value= running_config.get('use_cli_profile'))}",
+          "desc": f"Use preconfigured aws cli sso profile (created with aws configure sso --profile <profile_name>)\nValid optiond for yes: {self.get_common().helper_type().bool().is_true_values()}{self.__get_existing_text(exiting_value= profile_data.get('use_cli_profile'))}",
           "handler": generate_data_handlers.get_handler(handler= "base"),
-          "default": running_config.get("use_cli_profile"),
+          "default": profile_data.get("use_cli_profile") == True,
           "optional": False
         },
         "sso_profile_name": {
           "validation": lambda item: self.__step_process_sso_valid_profile(profile_name= item, existing_profile= existing_sso_profile_name),
           "allow_empty": True,
           "skip": lambda item: item.get("use_cli_profile").get("formatted") if item is not None and item.get("use_cli_profile") is not None else False,
           "messages":{
             "validation": f"Could not find profile.",
           },
           "conversion": lambda item: self.get_common().helper_type().string().trim(string_value= item),
           "desc": f"Enter the SSO Profile Name{self.__get_existing_text(exiting_value= existing_sso_profile_name)}",
           "handler": generate_data_handlers.get_handler(handler= "base"),
-          "default": running_config.get("sso_profile_name"),
+          "default": profile_data.get("sso_profile_name"),
           "optional": False
         },
         "sso_start_url": {
           "validation": lambda item: item,
           "skip": lambda item: not item.get("use_cli_profile").get("formatted") if item is not None and item.get("use_cli_profile") is not None else True,
           "messages":{},
           "conversion": lambda item: self.get_common().helper_type().string().trim(item),
           "desc": f"Enter the SSO start url (ex: https://<aws_id>.awsapps.com/start",
           "handler": generate_data_handlers.get_handler(handler= "base"),
-          "default": running_config.get("sso_start_url"),
-          "optional": not self.get_common().helper_type().string().is_null_or_whitespace(string_value= running_config.get("sso_start_url"))
+          "default": profile_data.get("sso_start_url"),
+          "optional": not self.get_common().helper_type().string().is_null_or_whitespace(string_value= profile_data.get("sso_start_url"))
         },
         "sso_region": {
           "validation": lambda item: item,
           "skip": lambda item: not item.get("use_cli_profile").get("formatted") if item is not None and item.get("use_cli_profile") is not None else True,
           "allow_empty": True,
           "messages":{},
           "conversion": lambda item: self.get_common().helper_type().string().trim(item),
-          "desc": f"Enter the default region to use{self.__get_existing_text(exiting_value= running_config.get('sso_region'))}",
+          "desc": f"Enter the default region to use{self.__get_existing_text(exiting_value= profile_data.get('sso_region'))}",
           "handler": generate_data_handlers.get_handler(handler= "base"),
-          "default": running_config.get("sso_region") if not self.get_common().helper_type().string().is_null_or_whitespace(string_value= running_config.get("sso_region")) else "us-east-1",
+          "default": profile_data.get("sso_region") if not self.get_common().helper_type().string().is_null_or_whitespace(string_value= profile_data.get("sso_region")) else "us-east-1",
           "optional": False
         },
         "sso_account_id": {
           "validation": lambda item: self.get_common().helper_type().regex().get(pattern= "^[0-9]{12,}$").fullmatch(str(item)) if item is not None else False,
           "skip": lambda item: not item.get("use_cli_profile").get("formatted") if item is not None and item.get("use_cli_profile") is not None else True,
           "allow_empty": True,
           "messages":{
             "validation": f"It should be a 12 digit string (if its under 12 characters it should have leading zeros) ex. 000000000001",
           },
           "conversion": lambda item: item,
-          "desc": f"Enter the organization account id (main account id)\n It should be 12 numeric characters.{self.__get_existing_text(exiting_value= running_config.get('sso_account_id'))}",
+          "desc": f"Enter the organization account id (main account id)\n It should be 12 numeric characters.{self.__get_existing_text(exiting_value= profile_data.get('sso_account_id'))}",
           "handler": generate_data_handlers.get_handler(handler= "base"),
-          "default": running_config.get("sso_account_id"),
+          "default": profile_data.get("sso_account_id"),
           "optional": False
         },
         "sso_role_name": {
           "validation": lambda item: item,
           "skip": lambda item: not item.get("use_cli_profile").get("formatted") if item is not None and item.get("use_cli_profile") is not None else True,
           "allow_empty": True,
           "messages":{},
           "conversion": lambda item: self.get_common().helper_type().string().trim(item),
-          "desc": f"Enter the role to use{self.__get_existing_text(exiting_value= running_config.get('sso_account_id'))}",
+          "desc": f"Enter the role to use{self.__get_existing_text(exiting_value= profile_data.get('sso_account_id'))}",
           "handler": generate_data_handlers.get_handler(handler= "base"),
-          "default": running_config.get("sso_role_name"),
+          "default": profile_data.get("sso_role_name"),
           "optional": False
         },
         "output": {
           "validation": lambda item: item,
           "skip": lambda item: not item.get("use_cli_profile").get("formatted") if item is not None and item.get("use_cli_profile") is not None else True,
           "allow_empty": True,
           "messages":{},
           "conversion": lambda item: self.get_common().helper_type().string().trim(item),
-          "desc": f"Enter a valid output format. For a full list goto:\nhttps://docs.aws.amazon.com/cli/latest/userguide/cli-usage-output-format.html{self.__get_existing_text(exiting_value= running_config.get('output'))}",
+          "desc": f"Enter a valid output format. For a full list goto:\nhttps://docs.aws.amazon.com/cli/latest/userguide/cli-usage-output-format.html{self.__get_existing_text(exiting_value= profile_data.get('output'))}",
           "handler": generate_data_handlers.get_handler(handler= "base"),
-          "default": running_config.get("output") if not self.get_common().helper_type().string().is_null_or_whitespace(string_value= running_config.get("output")) else "json",
+          "default": profile_data.get("output") if not self.get_common().helper_type().string().is_null_or_whitespace(string_value= profile_data.get("output")) else "json",
           "optional": False
         },        
         "default_profile": {
           "validation": lambda item: self.get_common().helper_type().bool().is_bool(check_value= item),
           "allow_empty": True,
           "messages":{
             "validation": f"Valid options for Yes are: {self.get_common().helper_type().bool().is_true_values()}\nValid options for No are: {self.get_common().helper_type().bool().is_false_values()}",
           },
           "conversion": lambda item: self.get_common().helper_type().bool().is_true(check_value= item),
-          "desc": f"Is this the default profile 3mystic apps should use when profile is not passed. You can only have one profile,\nValid optiond for yes: {self.get_common().helper_type().bool().is_true_values()}{self.__get_existing_text(exiting_value= running_config.get('default_profile'))}",
+          "desc": f"Is this the default profile 3mystic apps should use when profile is not passed. You can only have one profile,\nValid optiond for yes: {self.get_common().helper_type().bool().is_true_values()}{self.__get_existing_text(exiting_value= profile_data.get('default_profile'))}",
           "handler": generate_data_handlers.get_handler(handler= "base"),
-          "default": self.get_default_default_profile(config = config, profile_name= profile_name, running_config= running_config),
+          "default": self.get_default_profile_setting(profile_name= profile_name, profile_data= profile_data),
           "optional": False
         }
       }
     )
     
     if response is None:
       return
 
     for key, item in response.items():
-      running_config[key] = item.get("formated") if item is not None else ""
+      profile_data[key] = item.get("formated") if item is not None else ""
     
-    if self.get_common().helper_type().string().is_null_or_whitespace(string_value=running_config.get("sso_profile_name")):
-      running_config["sso_profile_name"] = existing_sso_profile_name
+    if self.get_common().helper_type().string().is_null_or_whitespace(string_value=profile_data.get("sso_profile_name")):
+      profile_data["sso_profile_name"] = existing_sso_profile_name
     
-    self.update_config_profile(config= config, profile_name= profile_name, running_config= running_config)
+    self.update_config_profile(profile_name= profile_name, profile_data= profile_data)
     print(f"Profile ({profile_name} saved/updated)")
```

### Comparing `threemystic_cloud_client-0.0.2/.gitignore` & `threemystic_cloud_client-0.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.0.2/LICENSE` & `threemystic_cloud_client-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.0.2/README.md` & `threemystic_cloud_client-0.1.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 # 3mystic_cloud_client
-A set of common files that are used for the various projects under 3 Mystic Apes
+A tool to help uniform the connection to the cloud providers.
+Currently supports AWS/Azure
 
 # Install
 
 ## pip
 
 This project is currently designed to be installed via pip
+Currently the project is under development and is not in PyPI. 
+So you need to install the following packages <br/>
+pip install https://github.com/3MysticApes/3mystic_common <br/>
 pip install https://github.com/3MysticApes/3mystic_cloud_client
 
 Once installed you will get the following command:
 3mystic_cloud_client
 
 The above command allows you to configure the cloud client.
```

### Comparing `threemystic_cloud_client-0.0.2/hatch.toml` & `threemystic_cloud_client-0.1.0/hatch.toml`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.0.2/pyproject.toml` & `threemystic_cloud_client-0.1.0/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 [build-system]
 requires = ["hatchling>=1.11.0"]
 build-backend = "hatchling.build"
 
 [project]
 name = "threemystic-cloud-client"
-description = "Common Library for for various tool sets"
+description = "A tool to help facilitate the communication with various cloud providers"
 readme = "README.md"
 license = "MIT"
 requires-python = ">=3.8"
 authors = [
   { name="Ron Truex" },
 ]
 classifiers = [
@@ -23,27 +23,38 @@
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
   "colorama; platform_system == 'Windows'",
-  "threemystic-common >= 0.0.3",
-  "boto3 >= 1.21.41",
-  "typing-extensions >= 4.4.0"
+  "threemystic-common >= 0.1.0",
+  "polling2 >= 0.5.0",
+  "typing-extensions >= 4.4.0",
+  "boto3 >= 1.26.151",
+  "botocore >= 1.29.151",
+  "azure-common >= 1.1.28",
+  "azure-cli >= 2.49.0",
+  "azure-identity >= 1.13.0",
+  "azure-mgmt-subscription >= 3.1.1",
+  "azure-mgmt-managementgroups >= 1.0.0",
+  "azure-mgmt-resourcegraph >= 8.0.0"
 ]
 dynamic = ["version"]
 
 [project.urls]
 "Homepage" = "https://github.com/3MysticApes/3mystic_cloud_client"
 "Bug Tracker" = "https://github.com/3MysticApes/3mystic_cloud_client/issues"
 
 [project.scripts]
 3mystic_cloud_client = "threemystic_cloud_client.cli:main"
 
+[tool.hatch.metadata]
+allow-direct-references = true
+
 [tool.hatch.version]
 path = "threemystic_cloud_client/__version__.py"
 
 [tool.hatch.build.targets.sdist]
 exclude = [
   "/.github",
   "/docs",
```

### Comparing `threemystic_cloud_client-0.0.2/PKG-INFO` & `threemystic_cloud_client-0.1.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: threemystic-cloud-client
-Version: 0.0.2
-Summary: Common Library for for various tool sets
+Version: 0.1.0
+Summary: A tool to help facilitate the communication with various cloud providers
 Project-URL: Homepage, https://github.com/3MysticApes/3mystic_cloud_client
 Project-URL: Bug Tracker, https://github.com/3MysticApes/3mystic_cloud_client/issues
 Author: Ron Truex
 License-Expression: MIT
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
@@ -13,28 +13,40 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.8
-Requires-Dist: boto3>=1.21.41
+Requires-Dist: azure-cli>=2.49.0
+Requires-Dist: azure-common>=1.1.28
+Requires-Dist: azure-identity>=1.13.0
+Requires-Dist: azure-mgmt-managementgroups>=1.0.0
+Requires-Dist: azure-mgmt-resourcegraph>=8.0.0
+Requires-Dist: azure-mgmt-subscription>=3.1.1
+Requires-Dist: boto3>=1.26.151
+Requires-Dist: botocore>=1.29.151
 Requires-Dist: colorama; platform_system == 'Windows'
-Requires-Dist: threemystic-common>=0.0.3
+Requires-Dist: polling2>=0.5.0
+Requires-Dist: threemystic-common>=0.1.0
 Requires-Dist: typing-extensions>=4.4.0
 Description-Content-Type: text/markdown
 
 # 3mystic_cloud_client
-A set of common files that are used for the various projects under 3 Mystic Apes
+A tool to help uniform the connection to the cloud providers.
+Currently supports AWS/Azure
 
 # Install
 
 ## pip
 
 This project is currently designed to be installed via pip
+Currently the project is under development and is not in PyPI. 
+So you need to install the following packages <br/>
+pip install https://github.com/3MysticApes/3mystic_common <br/>
 pip install https://github.com/3MysticApes/3mystic_cloud_client
 
 Once installed you will get the following command:
 3mystic_cloud_client
 
 The above command allows you to configure the cloud client.
```

