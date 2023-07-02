# Comparing `tmp/ediri_azapi-1.6.0.tar.gz` & `tmp/ediri_azapi-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ediri_azapi-1.6.0.tar", last modified: Sat May 20 20:22:10 2023, max compression
+gzip compressed data, was "ediri_azapi-1.7.0.tar", last modified: Sun Jul  2 07:59:39 2023, max compression
```

## Comparing `ediri_azapi-1.6.0.tar` & `ediri_azapi-1.7.0.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 20:22:10.359404 ediri_azapi-1.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)     5668 2023-05-20 20:22:10.359404 ediri_azapi-1.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5289 2023-05-20 20:22:09.000000 ediri_azapi-1.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 20:22:10.359404 ediri_azapi-1.6.0/ediri_azapi/
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-05-20 20:22:09.000000 ediri_azapi-1.6.0/ediri_azapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6273 2023-05-20 20:22:09.000000 ediri_azapi-1.6.0/ediri_azapi/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8122 2023-05-20 20:22:09.000000 ediri_azapi-1.6.0/ediri_azapi/_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 20:22:10.359404 ediri_azapi-1.6.0/ediri_azapi/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-20 20:22:09.000000 ediri_azapi-1.6.0/ediri_azapi/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4935 2023-05-20 20:22:09.000000 ediri_azapi-1.6.0/ediri_azapi/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)    11429 2023-05-20 20:22:09.000000 ediri_azapi-1.6.0/ediri_azapi/get_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     8540 2023-05-20 20:22:10.000000 ediri_azapi-1.6.0/ediri_azapi/get_resource_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     5815 2023-05-20 20:22:10.000000 ediri_azapi-1.6.0/ediri_azapi/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    30697 2023-05-20 20:22:10.000000 ediri_azapi-1.6.0/ediri_azapi/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-20 20:22:10.000000 ediri_azapi-1.6.0/ediri_azapi/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 20:22:10.000000 ediri_azapi-1.6.0/ediri_azapi/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    46394 2023-05-20 20:22:10.000000 ediri_azapi-1.6.0/ediri_azapi/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    24128 2023-05-20 20:22:10.000000 ediri_azapi-1.6.0/ediri_azapi/resource_action.py
--rw-r--r--   0 runner    (1001) docker     (123)    37211 2023-05-20 20:22:10.000000 ediri_azapi-1.6.0/ediri_azapi/update_resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 20:22:10.359404 ediri_azapi-1.6.0/ediri_azapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5668 2023-05-20 20:22:10.000000 ediri_azapi-1.6.0/ediri_azapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-20 20:22:10.000000 ediri_azapi-1.6.0/ediri_azapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 20:22:10.000000 ediri_azapi-1.6.0/ediri_azapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 20:22:10.000000 ediri_azapi-1.6.0/ediri_azapi.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-20 20:22:10.000000 ediri_azapi-1.6.0/ediri_azapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-20 20:22:10.000000 ediri_azapi-1.6.0/ediri_azapi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 20:22:10.359404 ediri_azapi-1.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-05-20 20:22:10.000000 ediri_azapi-1.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 07:59:39.718711 ediri_azapi-1.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     5668 2023-07-02 07:59:39.718711 ediri_azapi-1.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5289 2023-07-02 07:59:39.000000 ediri_azapi-1.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 07:59:39.718711 ediri_azapi-1.7.0/ediri_azapi/
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-07-02 07:59:39.000000 ediri_azapi-1.7.0/ediri_azapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6273 2023-07-02 07:59:39.000000 ediri_azapi-1.7.0/ediri_azapi/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8122 2023-07-02 07:59:39.000000 ediri_azapi-1.7.0/ediri_azapi/_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 07:59:39.718711 ediri_azapi-1.7.0/ediri_azapi/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-02 07:59:39.000000 ediri_azapi-1.7.0/ediri_azapi/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5700 2023-07-02 07:59:39.000000 ediri_azapi-1.7.0/ediri_azapi/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51844 2023-07-02 07:59:39.000000 ediri_azapi-1.7.0/ediri_azapi/data_plane_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12217 2023-07-02 07:59:39.000000 ediri_azapi-1.7.0/ediri_azapi/get_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9492 2023-07-02 07:59:39.000000 ediri_azapi-1.7.0/ediri_azapi/get_resource_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5815 2023-07-02 07:59:39.000000 ediri_azapi-1.7.0/ediri_azapi/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35332 2023-07-02 07:59:39.000000 ediri_azapi-1.7.0/ediri_azapi/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-02 07:59:39.000000 ediri_azapi-1.7.0/ediri_azapi/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 07:59:39.000000 ediri_azapi-1.7.0/ediri_azapi/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    48794 2023-07-02 07:59:39.000000 ediri_azapi-1.7.0/ediri_azapi/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26399 2023-07-02 07:59:39.000000 ediri_azapi-1.7.0/ediri_azapi/resource_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39567 2023-07-02 07:59:39.000000 ediri_azapi-1.7.0/ediri_azapi/update_resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 07:59:39.718711 ediri_azapi-1.7.0/ediri_azapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5668 2023-07-02 07:59:39.000000 ediri_azapi-1.7.0/ediri_azapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-02 07:59:39.000000 ediri_azapi-1.7.0/ediri_azapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 07:59:39.000000 ediri_azapi-1.7.0/ediri_azapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 07:59:39.000000 ediri_azapi-1.7.0/ediri_azapi.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-02 07:59:39.000000 ediri_azapi-1.7.0/ediri_azapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-02 07:59:39.000000 ediri_azapi-1.7.0/ediri_azapi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 07:59:39.718711 ediri_azapi-1.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-07-02 07:59:39.000000 ediri_azapi-1.7.0/setup.py
```

### Comparing `ediri_azapi-1.6.0/PKG-INFO` & `ediri_azapi-1.7.0/ediri_azapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: ediri_azapi
-Version: 1.6.0
+Name: ediri-azapi
+Version: 1.7.0
 Summary: A Pulumi package for creating and managing Azapi resources
 Home-page: https://github.com/dirien/pulumi-azapi
 License: Apache-2.0
 Project-URL: Repository, https://github.com/dirien/pulumi-azapi
 Keywords: pulumi azapi category/cloud
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `ediri_azapi-1.6.0/README.md` & `ediri_azapi-1.7.0/README.md`

 * *Files identical despite different names*

### Comparing `ediri_azapi-1.6.0/ediri_azapi/__init__.py` & `ediri_azapi-1.7.0/ediri_azapi/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
 from . import _utilities
 import typing
 # Export this package's modules as members:
+from .data_plane_resource import *
 from .get_resource import *
 from .get_resource_action import *
 from .provider import *
 from .resource import *
 from .resource_action import *
 from .update_resource import *
 from ._inputs import *
@@ -22,14 +23,22 @@
     config = _utilities.lazy_import('ediri_azapi.config')
 
 _utilities.register(
     resource_modules="""
 [
  {
   "pkg": "azapi",
+  "mod": "index/dataPlaneResource",
+  "fqn": "ediri_azapi",
+  "classes": {
+   "azapi:index/dataPlaneResource:DataPlaneResource": "DataPlaneResource"
+  }
+ },
+ {
+  "pkg": "azapi",
   "mod": "index/resource",
   "fqn": "ediri_azapi",
   "classes": {
    "azapi:index/resource:Resource": "Resource"
   }
  },
  {
```

### Comparing `ediri_azapi-1.6.0/ediri_azapi/_inputs.py` & `ediri_azapi-1.7.0/ediri_azapi/_inputs.py`

 * *Files identical despite different names*

### Comparing `ediri_azapi-1.6.0/ediri_azapi/_utilities.py` & `ediri_azapi-1.7.0/ediri_azapi/_utilities.py`

 * *Files identical despite different names*

### Comparing `ediri_azapi-1.6.0/ediri_azapi/config/vars.py` & `ediri_azapi-1.7.0/ediri_azapi/config/vars.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,14 +12,18 @@
 import types
 
 __config__ = pulumi.Config('azapi')
 
 
 class _ExportableConfig(types.ModuleType):
     @property
+    def auxiliary_tenant_ids(self) -> Optional[str]:
+        return __config__.get('auxiliaryTenantIds')
+
+    @property
     def client_certificate_password(self) -> Optional[str]:
         """
         The password associated with the Client Certificate. For use when authenticating as a Service Principal using a Client
         Certificate
         """
         return __config__.get('clientCertificatePassword')
 
@@ -42,14 +46,21 @@
     def client_secret(self) -> Optional[str]:
         """
         The Client Secret which should be used. For use When authenticating as a Service Principal using a Client Secret.
         """
         return __config__.get('clientSecret')
 
     @property
+    def custom_correlation_request_id(self) -> Optional[str]:
+        """
+        The value of the x-ms-correlation-request-id header (otherwise an auto-generated UUID will be used).
+        """
+        return __config__.get('customCorrelationRequestId')
+
+    @property
     def default_location(self) -> Optional[str]:
         return __config__.get('defaultLocation')
 
     @property
     def default_name(self) -> Optional[str]:
         return __config__.get('defaultName')
 
@@ -141,13 +152,27 @@
     def tenant_id(self) -> Optional[str]:
         """
         The Tenant ID which should be used.
         """
         return __config__.get('tenantId')
 
     @property
+    def use_cli(self) -> Optional[bool]:
+        """
+        Allow Azure CLI to be used for Authentication.
+        """
+        return __config__.get_bool('useCli')
+
+    @property
+    def use_msi(self) -> Optional[bool]:
+        """
+        Allow Managed Service Identity to be used for Authentication.
+        """
+        return __config__.get_bool('useMsi')
+
+    @property
     def use_oidc(self) -> Optional[bool]:
         """
         Allow OpenID Connect to be used for authentication
         """
         return __config__.get_bool('useOidc')
```

### Comparing `ediri_azapi-1.6.0/ediri_azapi/get_resource.py` & `ediri_azapi-1.7.0/ediri_azapi/get_resource.py`

 * *Files 7% similar despite different names*

```diff
@@ -85,14 +85,19 @@
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def output(self) -> str:
         """
         The output json containing the properties specified in `response_export_values`. Here're some examples to decode json and extract the value.
+        ```
+        // it will output "registry1.azurecr.io"
+        output "login_server" {
+        value = jsondecode(azapi_resource.example.output).properties.loginServer
+        }
         """
         return pulumi.get(self, "output")
 
     @property
     @pulumi.getter(name="parentId")
     def parent_id(self) -> Optional[str]:
         return pulumi.get(self, "parent_id")
@@ -148,14 +153,16 @@
                  resource_id: Optional[str] = None,
                  response_export_values: Optional[Sequence[str]] = None,
                  type: Optional[str] = None,
                  opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetResourceResult:
     """
     This resource can access any existing Azure resource manager resource.
 
+    ## Example Usage
+
 
     :param pulumi.InputType['GetResourceIdentityArgs'] identity: An `identity` block as defined below, which contains the Managed Service Identity information for this azure resource.
     :param str name: Specifies the name of the azure resource.
     :param str parent_id: The ID of the azure resource in which this resource is created. It supports different kinds of deployment scope for **top level** resources: 
            - resource group scope: `parent_id` should be the ID of a resource group, it's recommended to manage a resource group by azurerm_resource_group.
            - management group scope: `parent_id` should be the ID of a management group, it's recommended to manage a management group by azurerm_management_group.
            - extension scope: `parent_id` should be the ID of the resource you're adding the extension to.
@@ -165,16 +172,25 @@
            For child level resources, the `parent_id` should be the ID of its parent resource, for example, subnet resource's `parent_id` is the ID of the vnet.
     :param str resource_id: The ID of an existing azure source.
            
            > **Note:** Configuring `name` and `parent_id` is an alternative way to configure `resource_id`.
     :param Sequence[str] response_export_values: A list of path that needs to be exported from response body.
            Setting it to `["*"]` will export the full response body.
            Here's an example. If it sets to `["properties.loginServer", "properties.policies.quarantinePolicy.status"]`, it will set the following json to computed property `output`.
-           ```python
-           import pulumi
+           ```
+           {
+           "properties" : {
+           "loginServer" : "registry1.azurecr.io"
+           "policies" : {
+           "quarantinePolicy" = {
+           "status" = "disabled"
+           }
+           }
+           }
+           }
            ```
     :param str type: It is in a format like `<resource-type>@<api-version>`. `<resource-type>` is the Azure resource type, for example, `Microsoft.Storage/storageAccounts`.
            `<api-version>` is version of the API used to manage this azure resource.
     """
     __args__ = dict()
     __args__['identity'] = identity
     __args__['name'] = name
@@ -182,37 +198,39 @@
     __args__['resourceId'] = resource_id
     __args__['responseExportValues'] = response_export_values
     __args__['type'] = type
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('azapi:index/getResource:getResource', __args__, opts=opts, typ=GetResourceResult).value
 
     return AwaitableGetResourceResult(
-        id=__ret__.id,
-        identity=__ret__.identity,
-        location=__ret__.location,
-        name=__ret__.name,
-        output=__ret__.output,
-        parent_id=__ret__.parent_id,
-        resource_id=__ret__.resource_id,
-        response_export_values=__ret__.response_export_values,
-        tags=__ret__.tags,
-        type=__ret__.type)
+        id=pulumi.get(__ret__, 'id'),
+        identity=pulumi.get(__ret__, 'identity'),
+        location=pulumi.get(__ret__, 'location'),
+        name=pulumi.get(__ret__, 'name'),
+        output=pulumi.get(__ret__, 'output'),
+        parent_id=pulumi.get(__ret__, 'parent_id'),
+        resource_id=pulumi.get(__ret__, 'resource_id'),
+        response_export_values=pulumi.get(__ret__, 'response_export_values'),
+        tags=pulumi.get(__ret__, 'tags'),
+        type=pulumi.get(__ret__, 'type'))
 
 
 @_utilities.lift_output_func(get_resource)
 def get_resource_output(identity: Optional[pulumi.Input[Optional[pulumi.InputType['GetResourceIdentityArgs']]]] = None,
                         name: Optional[pulumi.Input[Optional[str]]] = None,
                         parent_id: Optional[pulumi.Input[Optional[str]]] = None,
                         resource_id: Optional[pulumi.Input[Optional[str]]] = None,
                         response_export_values: Optional[pulumi.Input[Optional[Sequence[str]]]] = None,
                         type: Optional[pulumi.Input[str]] = None,
                         opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetResourceResult]:
     """
     This resource can access any existing Azure resource manager resource.
 
+    ## Example Usage
+
 
     :param pulumi.InputType['GetResourceIdentityArgs'] identity: An `identity` block as defined below, which contains the Managed Service Identity information for this azure resource.
     :param str name: Specifies the name of the azure resource.
     :param str parent_id: The ID of the azure resource in which this resource is created. It supports different kinds of deployment scope for **top level** resources: 
            - resource group scope: `parent_id` should be the ID of a resource group, it's recommended to manage a resource group by azurerm_resource_group.
            - management group scope: `parent_id` should be the ID of a management group, it's recommended to manage a management group by azurerm_management_group.
            - extension scope: `parent_id` should be the ID of the resource you're adding the extension to.
@@ -222,14 +240,23 @@
            For child level resources, the `parent_id` should be the ID of its parent resource, for example, subnet resource's `parent_id` is the ID of the vnet.
     :param str resource_id: The ID of an existing azure source.
            
            > **Note:** Configuring `name` and `parent_id` is an alternative way to configure `resource_id`.
     :param Sequence[str] response_export_values: A list of path that needs to be exported from response body.
            Setting it to `["*"]` will export the full response body.
            Here's an example. If it sets to `["properties.loginServer", "properties.policies.quarantinePolicy.status"]`, it will set the following json to computed property `output`.
-           ```python
-           import pulumi
+           ```
+           {
+           "properties" : {
+           "loginServer" : "registry1.azurecr.io"
+           "policies" : {
+           "quarantinePolicy" = {
+           "status" = "disabled"
+           }
+           }
+           }
+           }
            ```
     :param str type: It is in a format like `<resource-type>@<api-version>`. `<resource-type>` is the Azure resource type, for example, `Microsoft.Storage/storageAccounts`.
            `<api-version>` is version of the API used to manage this azure resource.
     """
     ...
```

### Comparing `ediri_azapi-1.6.0/ediri_azapi/get_resource_action.py` & `ediri_azapi-1.7.0/ediri_azapi/get_resource_action.py`

 * *Files 18% similar despite different names*

```diff
@@ -71,14 +71,19 @@
         return pulumi.get(self, "method")
 
     @property
     @pulumi.getter
     def output(self) -> str:
         """
         The output json containing the properties specified in `response_export_values`. Here are some examples to decode json and extract the value.
+        ```hcl
+        // it will output "nHGYNd******i4wdug=="
+        output "primary_key" {
+        value = jsondecode(azapi_resource_action.test.output).keys.0.Value
+        }
         """
         return pulumi.get(self, "output")
 
     @property
     @pulumi.getter(name="resourceId")
     def resource_id(self) -> Optional[str]:
         return pulumi.get(self, "resource_id")
@@ -118,24 +123,39 @@
                         type: Optional[str] = None,
                         opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetResourceActionResult:
     """
     This resource can perform resource action which gets information from an existing resource.
     It's recommended to use `ResourceAction` data source to perform readonly action, please use `ResourceAction` resource,
     if user wants to perform actions which change a resource's state.
 
+    ## Example Usage
+
 
     :param str action: The name of the resource action. It's also possible to make Http requests towards the resource ID if leave this field empty.
     :param str body: A JSON object that contains the request body.
     :param str method: Specifies the Http method of the azure resource action. Allowed values are `POST` and `GET`. Defaults to `POST`.
     :param str resource_id: The ID of an existing azure source.
     :param Sequence[str] response_export_values: A list of path that needs to be exported from response body.
            Setting it to `["*"]` will export the full response body.
            Here's an example. If it sets to `["keys"]`, it will set the following json to computed property `output`.
-           ```python
-           import pulumi
+           ```
+           {
+           "keys": [
+           {
+           "KeyName": "Primary",
+           "Permissions": "Full",
+           "Value": "nHGYNd******i4wdug=="
+           },
+           {
+           "KeyName": "Secondary",
+           "Permissions": "Full",
+           "Value": "6yoCad******SLzKzg=="
+           }
+           ]
+           }
            ```
     :param str type: It is in a format like `<resource-type>@<api-version>`. `<resource-type>` is the Azure resource type, for example, `Microsoft.Storage/storageAccounts`.
            `<api-version>` is version of the API used to manage this azure resource.
     """
     __args__ = dict()
     __args__['action'] = action
     __args__['body'] = body
@@ -143,22 +163,22 @@
     __args__['resourceId'] = resource_id
     __args__['responseExportValues'] = response_export_values
     __args__['type'] = type
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('azapi:index/getResourceAction:getResourceAction', __args__, opts=opts, typ=GetResourceActionResult).value
 
     return AwaitableGetResourceActionResult(
-        action=__ret__.action,
-        body=__ret__.body,
-        id=__ret__.id,
-        method=__ret__.method,
-        output=__ret__.output,
-        resource_id=__ret__.resource_id,
-        response_export_values=__ret__.response_export_values,
-        type=__ret__.type)
+        action=pulumi.get(__ret__, 'action'),
+        body=pulumi.get(__ret__, 'body'),
+        id=pulumi.get(__ret__, 'id'),
+        method=pulumi.get(__ret__, 'method'),
+        output=pulumi.get(__ret__, 'output'),
+        resource_id=pulumi.get(__ret__, 'resource_id'),
+        response_export_values=pulumi.get(__ret__, 'response_export_values'),
+        type=pulumi.get(__ret__, 'type'))
 
 
 @_utilities.lift_output_func(get_resource_action)
 def get_resource_action_output(action: Optional[pulumi.Input[Optional[str]]] = None,
                                body: Optional[pulumi.Input[Optional[str]]] = None,
                                method: Optional[pulumi.Input[Optional[str]]] = None,
                                resource_id: Optional[pulumi.Input[Optional[str]]] = None,
@@ -166,22 +186,37 @@
                                type: Optional[pulumi.Input[str]] = None,
                                opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetResourceActionResult]:
     """
     This resource can perform resource action which gets information from an existing resource.
     It's recommended to use `ResourceAction` data source to perform readonly action, please use `ResourceAction` resource,
     if user wants to perform actions which change a resource's state.
 
+    ## Example Usage
+
 
     :param str action: The name of the resource action. It's also possible to make Http requests towards the resource ID if leave this field empty.
     :param str body: A JSON object that contains the request body.
     :param str method: Specifies the Http method of the azure resource action. Allowed values are `POST` and `GET`. Defaults to `POST`.
     :param str resource_id: The ID of an existing azure source.
     :param Sequence[str] response_export_values: A list of path that needs to be exported from response body.
            Setting it to `["*"]` will export the full response body.
            Here's an example. If it sets to `["keys"]`, it will set the following json to computed property `output`.
-           ```python
-           import pulumi
+           ```
+           {
+           "keys": [
+           {
+           "KeyName": "Primary",
+           "Permissions": "Full",
+           "Value": "nHGYNd******i4wdug=="
+           },
+           {
+           "KeyName": "Secondary",
+           "Permissions": "Full",
+           "Value": "6yoCad******SLzKzg=="
+           }
+           ]
+           }
            ```
     :param str type: It is in a format like `<resource-type>@<api-version>`. `<resource-type>` is the Azure resource type, for example, `Microsoft.Storage/storageAccounts`.
            `<api-version>` is version of the API used to manage this azure resource.
     """
     ...
```

### Comparing `ediri_azapi-1.6.0/ediri_azapi/outputs.py` & `ediri_azapi-1.7.0/ediri_azapi/outputs.py`

 * *Files identical despite different names*

### Comparing `ediri_azapi-1.6.0/ediri_azapi/provider.py` & `ediri_azapi-1.7.0/ediri_azapi/provider.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,18 +11,20 @@
 
 __all__ = ['ProviderArgs', 'Provider']
 
 @pulumi.input_type
 class ProviderArgs:
     def __init__(__self__, *,
                  environment: pulumi.Input[str],
+                 auxiliary_tenant_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  client_certificate_password: Optional[pulumi.Input[str]] = None,
                  client_certificate_path: Optional[pulumi.Input[str]] = None,
                  client_id: Optional[pulumi.Input[str]] = None,
                  client_secret: Optional[pulumi.Input[str]] = None,
+                 custom_correlation_request_id: Optional[pulumi.Input[str]] = None,
                  default_location: Optional[pulumi.Input[str]] = None,
                  default_name: Optional[pulumi.Input[str]] = None,
                  default_naming_prefix: Optional[pulumi.Input[str]] = None,
                  default_naming_suffix: Optional[pulumi.Input[str]] = None,
                  default_tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  disable_correlation_request_id: Optional[pulumi.Input[bool]] = None,
                  disable_terraform_partner_id: Optional[pulumi.Input[bool]] = None,
@@ -30,47 +32,56 @@
                  oidc_request_url: Optional[pulumi.Input[str]] = None,
                  oidc_token: Optional[pulumi.Input[str]] = None,
                  oidc_token_file_path: Optional[pulumi.Input[str]] = None,
                  partner_id: Optional[pulumi.Input[str]] = None,
                  skip_provider_registration: Optional[pulumi.Input[bool]] = None,
                  subscription_id: Optional[pulumi.Input[str]] = None,
                  tenant_id: Optional[pulumi.Input[str]] = None,
+                 use_cli: Optional[pulumi.Input[bool]] = None,
+                 use_msi: Optional[pulumi.Input[bool]] = None,
                  use_oidc: Optional[pulumi.Input[bool]] = None):
         """
         The set of arguments for constructing a Provider resource.
         :param pulumi.Input[str] environment: The Cloud Environment which should be used. Possible values are public, usgovernment and china. Defaults to public.
         :param pulumi.Input[str] client_certificate_password: The password associated with the Client Certificate. For use when authenticating as a Service Principal using a Client
                Certificate
         :param pulumi.Input[str] client_certificate_path: The path to the Client Certificate associated with the Service Principal for use when authenticating as a Service
                Principal using a Client Certificate.
         :param pulumi.Input[str] client_id: The Client ID which should be used.
         :param pulumi.Input[str] client_secret: The Client Secret which should be used. For use When authenticating as a Service Principal using a Client Secret.
+        :param pulumi.Input[str] custom_correlation_request_id: The value of the x-ms-correlation-request-id header (otherwise an auto-generated UUID will be used).
         :param pulumi.Input[bool] disable_correlation_request_id: This will disable the x-ms-correlation-request-id header.
         :param pulumi.Input[bool] disable_terraform_partner_id: This will disable the Terraform Partner ID which is used if a custom `partner_id` isn't specified.
         :param pulumi.Input[str] oidc_request_token: The bearer token for the request to the OIDC provider. For use When authenticating as a Service Principal using OpenID
                Connect.
         :param pulumi.Input[str] oidc_request_url: The URL for the OIDC provider from which to request an ID token. For use When authenticating as a Service Principal
                using OpenID Connect.
         :param pulumi.Input[str] oidc_token: The OIDC ID token for use when authenticating as a Service Principal using OpenID Connect.
         :param pulumi.Input[str] oidc_token_file_path: The path to a file containing an OIDC ID token for use when authenticating as a Service Principal using OpenID Connect.
         :param pulumi.Input[str] partner_id: A GUID/UUID that is registered with Microsoft to facilitate partner resource usage attribution.
         :param pulumi.Input[bool] skip_provider_registration: Should the Provider skip registering all of the Resource Providers that it supports, if they're not already registered?
         :param pulumi.Input[str] subscription_id: The Subscription ID which should be used.
         :param pulumi.Input[str] tenant_id: The Tenant ID which should be used.
+        :param pulumi.Input[bool] use_cli: Allow Azure CLI to be used for Authentication.
+        :param pulumi.Input[bool] use_msi: Allow Managed Service Identity to be used for Authentication.
         :param pulumi.Input[bool] use_oidc: Allow OpenID Connect to be used for authentication
         """
         pulumi.set(__self__, "environment", environment)
+        if auxiliary_tenant_ids is not None:
+            pulumi.set(__self__, "auxiliary_tenant_ids", auxiliary_tenant_ids)
         if client_certificate_password is not None:
             pulumi.set(__self__, "client_certificate_password", client_certificate_password)
         if client_certificate_path is not None:
             pulumi.set(__self__, "client_certificate_path", client_certificate_path)
         if client_id is not None:
             pulumi.set(__self__, "client_id", client_id)
         if client_secret is not None:
             pulumi.set(__self__, "client_secret", client_secret)
+        if custom_correlation_request_id is not None:
+            pulumi.set(__self__, "custom_correlation_request_id", custom_correlation_request_id)
         if default_location is not None:
             pulumi.set(__self__, "default_location", default_location)
         if default_name is not None:
             pulumi.set(__self__, "default_name", default_name)
         if default_naming_prefix is not None:
             pulumi.set(__self__, "default_naming_prefix", default_naming_prefix)
         if default_naming_suffix is not None:
@@ -93,14 +104,18 @@
             pulumi.set(__self__, "partner_id", partner_id)
         if skip_provider_registration is not None:
             pulumi.set(__self__, "skip_provider_registration", skip_provider_registration)
         if subscription_id is not None:
             pulumi.set(__self__, "subscription_id", subscription_id)
         if tenant_id is not None:
             pulumi.set(__self__, "tenant_id", tenant_id)
+        if use_cli is not None:
+            pulumi.set(__self__, "use_cli", use_cli)
+        if use_msi is not None:
+            pulumi.set(__self__, "use_msi", use_msi)
         if use_oidc is not None:
             pulumi.set(__self__, "use_oidc", use_oidc)
 
     @property
     @pulumi.getter
     def environment(self) -> pulumi.Input[str]:
         """
@@ -109,14 +124,23 @@
         return pulumi.get(self, "environment")
 
     @environment.setter
     def environment(self, value: pulumi.Input[str]):
         pulumi.set(self, "environment", value)
 
     @property
+    @pulumi.getter(name="auxiliaryTenantIds")
+    def auxiliary_tenant_ids(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+        return pulumi.get(self, "auxiliary_tenant_ids")
+
+    @auxiliary_tenant_ids.setter
+    def auxiliary_tenant_ids(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+        pulumi.set(self, "auxiliary_tenant_ids", value)
+
+    @property
     @pulumi.getter(name="clientCertificatePassword")
     def client_certificate_password(self) -> Optional[pulumi.Input[str]]:
         """
         The password associated with the Client Certificate. For use when authenticating as a Service Principal using a Client
         Certificate
         """
         return pulumi.get(self, "client_certificate_password")
@@ -159,14 +183,26 @@
         return pulumi.get(self, "client_secret")
 
     @client_secret.setter
     def client_secret(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "client_secret", value)
 
     @property
+    @pulumi.getter(name="customCorrelationRequestId")
+    def custom_correlation_request_id(self) -> Optional[pulumi.Input[str]]:
+        """
+        The value of the x-ms-correlation-request-id header (otherwise an auto-generated UUID will be used).
+        """
+        return pulumi.get(self, "custom_correlation_request_id")
+
+    @custom_correlation_request_id.setter
+    def custom_correlation_request_id(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "custom_correlation_request_id", value)
+
+    @property
     @pulumi.getter(name="defaultLocation")
     def default_location(self) -> Optional[pulumi.Input[str]]:
         return pulumi.get(self, "default_location")
 
     @default_location.setter
     def default_location(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "default_location", value)
@@ -326,14 +362,38 @@
         return pulumi.get(self, "tenant_id")
 
     @tenant_id.setter
     def tenant_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "tenant_id", value)
 
     @property
+    @pulumi.getter(name="useCli")
+    def use_cli(self) -> Optional[pulumi.Input[bool]]:
+        """
+        Allow Azure CLI to be used for Authentication.
+        """
+        return pulumi.get(self, "use_cli")
+
+    @use_cli.setter
+    def use_cli(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "use_cli", value)
+
+    @property
+    @pulumi.getter(name="useMsi")
+    def use_msi(self) -> Optional[pulumi.Input[bool]]:
+        """
+        Allow Managed Service Identity to be used for Authentication.
+        """
+        return pulumi.get(self, "use_msi")
+
+    @use_msi.setter
+    def use_msi(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "use_msi", value)
+
+    @property
     @pulumi.getter(name="useOidc")
     def use_oidc(self) -> Optional[pulumi.Input[bool]]:
         """
         Allow OpenID Connect to be used for authentication
         """
         return pulumi.get(self, "use_oidc")
 
@@ -343,18 +403,20 @@
 
 
 class Provider(pulumi.ProviderResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
+                 auxiliary_tenant_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  client_certificate_password: Optional[pulumi.Input[str]] = None,
                  client_certificate_path: Optional[pulumi.Input[str]] = None,
                  client_id: Optional[pulumi.Input[str]] = None,
                  client_secret: Optional[pulumi.Input[str]] = None,
+                 custom_correlation_request_id: Optional[pulumi.Input[str]] = None,
                  default_location: Optional[pulumi.Input[str]] = None,
                  default_name: Optional[pulumi.Input[str]] = None,
                  default_naming_prefix: Optional[pulumi.Input[str]] = None,
                  default_naming_suffix: Optional[pulumi.Input[str]] = None,
                  default_tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  disable_correlation_request_id: Optional[pulumi.Input[bool]] = None,
                  disable_terraform_partner_id: Optional[pulumi.Input[bool]] = None,
@@ -363,14 +425,16 @@
                  oidc_request_url: Optional[pulumi.Input[str]] = None,
                  oidc_token: Optional[pulumi.Input[str]] = None,
                  oidc_token_file_path: Optional[pulumi.Input[str]] = None,
                  partner_id: Optional[pulumi.Input[str]] = None,
                  skip_provider_registration: Optional[pulumi.Input[bool]] = None,
                  subscription_id: Optional[pulumi.Input[str]] = None,
                  tenant_id: Optional[pulumi.Input[str]] = None,
+                 use_cli: Optional[pulumi.Input[bool]] = None,
+                 use_msi: Optional[pulumi.Input[bool]] = None,
                  use_oidc: Optional[pulumi.Input[bool]] = None,
                  __props__=None):
         """
         The provider type for the azapi package. By default, resources use package-wide configuration
         settings, however an explicit `Provider` instance may be created and passed during resource
         construction to achieve fine-grained programmatic control over provider settings. See the
         [documentation](https://www.pulumi.com/docs/reference/programming-model/#providers) for more information.
@@ -379,27 +443,30 @@
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] client_certificate_password: The password associated with the Client Certificate. For use when authenticating as a Service Principal using a Client
                Certificate
         :param pulumi.Input[str] client_certificate_path: The path to the Client Certificate associated with the Service Principal for use when authenticating as a Service
                Principal using a Client Certificate.
         :param pulumi.Input[str] client_id: The Client ID which should be used.
         :param pulumi.Input[str] client_secret: The Client Secret which should be used. For use When authenticating as a Service Principal using a Client Secret.
+        :param pulumi.Input[str] custom_correlation_request_id: The value of the x-ms-correlation-request-id header (otherwise an auto-generated UUID will be used).
         :param pulumi.Input[bool] disable_correlation_request_id: This will disable the x-ms-correlation-request-id header.
         :param pulumi.Input[bool] disable_terraform_partner_id: This will disable the Terraform Partner ID which is used if a custom `partner_id` isn't specified.
         :param pulumi.Input[str] environment: The Cloud Environment which should be used. Possible values are public, usgovernment and china. Defaults to public.
         :param pulumi.Input[str] oidc_request_token: The bearer token for the request to the OIDC provider. For use When authenticating as a Service Principal using OpenID
                Connect.
         :param pulumi.Input[str] oidc_request_url: The URL for the OIDC provider from which to request an ID token. For use When authenticating as a Service Principal
                using OpenID Connect.
         :param pulumi.Input[str] oidc_token: The OIDC ID token for use when authenticating as a Service Principal using OpenID Connect.
         :param pulumi.Input[str] oidc_token_file_path: The path to a file containing an OIDC ID token for use when authenticating as a Service Principal using OpenID Connect.
         :param pulumi.Input[str] partner_id: A GUID/UUID that is registered with Microsoft to facilitate partner resource usage attribution.
         :param pulumi.Input[bool] skip_provider_registration: Should the Provider skip registering all of the Resource Providers that it supports, if they're not already registered?
         :param pulumi.Input[str] subscription_id: The Subscription ID which should be used.
         :param pulumi.Input[str] tenant_id: The Tenant ID which should be used.
+        :param pulumi.Input[bool] use_cli: Allow Azure CLI to be used for Authentication.
+        :param pulumi.Input[bool] use_msi: Allow Managed Service Identity to be used for Authentication.
         :param pulumi.Input[bool] use_oidc: Allow OpenID Connect to be used for authentication
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: ProviderArgs,
@@ -421,18 +488,20 @@
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
+                 auxiliary_tenant_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  client_certificate_password: Optional[pulumi.Input[str]] = None,
                  client_certificate_path: Optional[pulumi.Input[str]] = None,
                  client_id: Optional[pulumi.Input[str]] = None,
                  client_secret: Optional[pulumi.Input[str]] = None,
+                 custom_correlation_request_id: Optional[pulumi.Input[str]] = None,
                  default_location: Optional[pulumi.Input[str]] = None,
                  default_name: Optional[pulumi.Input[str]] = None,
                  default_naming_prefix: Optional[pulumi.Input[str]] = None,
                  default_naming_suffix: Optional[pulumi.Input[str]] = None,
                  default_tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  disable_correlation_request_id: Optional[pulumi.Input[bool]] = None,
                  disable_terraform_partner_id: Optional[pulumi.Input[bool]] = None,
@@ -441,28 +510,32 @@
                  oidc_request_url: Optional[pulumi.Input[str]] = None,
                  oidc_token: Optional[pulumi.Input[str]] = None,
                  oidc_token_file_path: Optional[pulumi.Input[str]] = None,
                  partner_id: Optional[pulumi.Input[str]] = None,
                  skip_provider_registration: Optional[pulumi.Input[bool]] = None,
                  subscription_id: Optional[pulumi.Input[str]] = None,
                  tenant_id: Optional[pulumi.Input[str]] = None,
+                 use_cli: Optional[pulumi.Input[bool]] = None,
+                 use_msi: Optional[pulumi.Input[bool]] = None,
                  use_oidc: Optional[pulumi.Input[bool]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = ProviderArgs.__new__(ProviderArgs)
 
+            __props__.__dict__["auxiliary_tenant_ids"] = pulumi.Output.from_input(auxiliary_tenant_ids).apply(pulumi.runtime.to_json) if auxiliary_tenant_ids is not None else None
             __props__.__dict__["client_certificate_password"] = client_certificate_password
             __props__.__dict__["client_certificate_path"] = client_certificate_path
             __props__.__dict__["client_id"] = client_id
             __props__.__dict__["client_secret"] = client_secret
+            __props__.__dict__["custom_correlation_request_id"] = custom_correlation_request_id
             __props__.__dict__["default_location"] = default_location
             __props__.__dict__["default_name"] = default_name
             __props__.__dict__["default_naming_prefix"] = default_naming_prefix
             __props__.__dict__["default_naming_suffix"] = default_naming_suffix
             __props__.__dict__["default_tags"] = pulumi.Output.from_input(default_tags).apply(pulumi.runtime.to_json) if default_tags is not None else None
             __props__.__dict__["disable_correlation_request_id"] = pulumi.Output.from_input(disable_correlation_request_id).apply(pulumi.runtime.to_json) if disable_correlation_request_id is not None else None
             __props__.__dict__["disable_terraform_partner_id"] = pulumi.Output.from_input(disable_terraform_partner_id).apply(pulumi.runtime.to_json) if disable_terraform_partner_id is not None else None
@@ -473,14 +546,16 @@
             __props__.__dict__["oidc_request_url"] = oidc_request_url
             __props__.__dict__["oidc_token"] = oidc_token
             __props__.__dict__["oidc_token_file_path"] = oidc_token_file_path
             __props__.__dict__["partner_id"] = partner_id
             __props__.__dict__["skip_provider_registration"] = pulumi.Output.from_input(skip_provider_registration).apply(pulumi.runtime.to_json) if skip_provider_registration is not None else None
             __props__.__dict__["subscription_id"] = subscription_id
             __props__.__dict__["tenant_id"] = tenant_id
+            __props__.__dict__["use_cli"] = pulumi.Output.from_input(use_cli).apply(pulumi.runtime.to_json) if use_cli is not None else None
+            __props__.__dict__["use_msi"] = pulumi.Output.from_input(use_msi).apply(pulumi.runtime.to_json) if use_msi is not None else None
             __props__.__dict__["use_oidc"] = pulumi.Output.from_input(use_oidc).apply(pulumi.runtime.to_json) if use_oidc is not None else None
         super(Provider, __self__).__init__(
             'azapi',
             resource_name,
             __props__,
             opts)
 
@@ -515,14 +590,22 @@
     def client_secret(self) -> pulumi.Output[Optional[str]]:
         """
         The Client Secret which should be used. For use When authenticating as a Service Principal using a Client Secret.
         """
         return pulumi.get(self, "client_secret")
 
     @property
+    @pulumi.getter(name="customCorrelationRequestId")
+    def custom_correlation_request_id(self) -> pulumi.Output[Optional[str]]:
+        """
+        The value of the x-ms-correlation-request-id header (otherwise an auto-generated UUID will be used).
+        """
+        return pulumi.get(self, "custom_correlation_request_id")
+
+    @property
     @pulumi.getter(name="defaultLocation")
     def default_location(self) -> pulumi.Output[Optional[str]]:
         return pulumi.get(self, "default_location")
 
     @property
     @pulumi.getter(name="defaultName")
     def default_name(self) -> pulumi.Output[Optional[str]]:
```

### Comparing `ediri_azapi-1.6.0/ediri_azapi/resource.py` & `ediri_azapi-1.7.0/ediri_azapi/resource.py`

 * *Files 6% similar despite different names*

```diff
@@ -48,16 +48,25 @@
         :param pulumi.Input[str] location: The Azure Region where the azure resource should exist.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] locks: A list of ARM resource IDs which are used to avoid create/modify/delete azapi resources at the same time.
         :param pulumi.Input[str] name: Specifies the name of the azure resource. Changing this forces a new resource to be created.
         :param pulumi.Input[bool] removing_special_chars: Whether to remove special characters in resource name. Defaults to `false`.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] response_export_values: A list of path that needs to be exported from response body.
                Setting it to `["*"]` will export the full response body.
                Here's an example. If it sets to `["properties.loginServer", "properties.policies.quarantinePolicy.status"]`, it will set the following json to computed property `output`.
-               ```python
-               import pulumi
+               ```
+               {
+               "properties" : {
+               "loginServer" : "registry1.azurecr.io"
+               "policies" : {
+               "quarantinePolicy" = {
+               "status" = "disabled"
+               }
+               }
+               }
+               }
                ```
         :param pulumi.Input[bool] schema_validation_enabled: Whether enabled the validation on `type` and `body` with embedded schema. Defaults to `true`.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: A mapping of tags which should be assigned to the azure resource.
         """
         pulumi.set(__self__, "parent_id", parent_id)
         pulumi.set(__self__, "type", type)
         if body is not None:
@@ -214,16 +223,25 @@
     @property
     @pulumi.getter(name="responseExportValues")
     def response_export_values(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
         A list of path that needs to be exported from response body.
         Setting it to `["*"]` will export the full response body.
         Here's an example. If it sets to `["properties.loginServer", "properties.policies.quarantinePolicy.status"]`, it will set the following json to computed property `output`.
-        ```python
-        import pulumi
+        ```
+        {
+        "properties" : {
+        "loginServer" : "registry1.azurecr.io"
+        "policies" : {
+        "quarantinePolicy" = {
+        "status" = "disabled"
+        }
+        }
+        }
+        }
         ```
         """
         return pulumi.get(self, "response_export_values")
 
     @response_export_values.setter
     def response_export_values(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "response_export_values", value)
@@ -276,28 +294,42 @@
         :param pulumi.Input['ResourceIdentityArgs'] identity: A `identity` block as defined below.
         :param pulumi.Input[bool] ignore_casing: Whether ignore incorrect casing returned in `body` to suppress plan-diff. Defaults to `false`.
         :param pulumi.Input[bool] ignore_missing_property: Whether ignore not returned properties like credentials in `body` to suppress plan-diff. Defaults to `true`.
         :param pulumi.Input[str] location: The Azure Region where the azure resource should exist.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] locks: A list of ARM resource IDs which are used to avoid create/modify/delete azapi resources at the same time.
         :param pulumi.Input[str] name: Specifies the name of the azure resource. Changing this forces a new resource to be created.
         :param pulumi.Input[str] output: The output json containing the properties specified in `response_export_values`. Here're some examples to decode json and extract the value.
+               ```
+               // it will output "registry1.azurecr.io"
+               output "login_server" {
+               value = jsondecode(azapi_resource.example.output).properties.loginServer
+               }
         :param pulumi.Input[str] parent_id: The ID of the azure resource in which this resource is created. Changing this forces a new resource to be created. It supports different kinds of deployment scope for **top level** resources: 
                - resource group scope: `parent_id` should be the ID of a resource group, it's recommended to manage a resource group by azurerm_resource_group.
                - management group scope: `parent_id` should be the ID of a management group, it's recommended to manage a management group by azurerm_management_group.
                - extension scope: `parent_id` should be the ID of the resource you're adding the extension to.
                - subscription scope: `parent_id` should be like `/subscriptions/00000000-0000-0000-0000-000000000000`
                - tenant scope: `parent_id` should be `/`
                
                For child level resources, the `parent_id` should be the ID of its parent resource, for example, subnet resource's `parent_id` is the ID of the vnet.
         :param pulumi.Input[bool] removing_special_chars: Whether to remove special characters in resource name. Defaults to `false`.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] response_export_values: A list of path that needs to be exported from response body.
                Setting it to `["*"]` will export the full response body.
                Here's an example. If it sets to `["properties.loginServer", "properties.policies.quarantinePolicy.status"]`, it will set the following json to computed property `output`.
-               ```python
-               import pulumi
+               ```
+               {
+               "properties" : {
+               "loginServer" : "registry1.azurecr.io"
+               "policies" : {
+               "quarantinePolicy" = {
+               "status" = "disabled"
+               }
+               }
+               }
+               }
                ```
         :param pulumi.Input[bool] schema_validation_enabled: Whether enabled the validation on `type` and `body` with embedded schema. Defaults to `true`.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: A mapping of tags which should be assigned to the azure resource.
         :param pulumi.Input[str] type: It is in a format like `<resource-type>@<api-version>`. `<resource-type>` is the Azure resource type, for example, `Microsoft.Storage/storageAccounts`.
                `<api-version>` is version of the API used to manage this azure resource.
         """
         if body is not None:
@@ -414,14 +446,19 @@
         pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter
     def output(self) -> Optional[pulumi.Input[str]]:
         """
         The output json containing the properties specified in `response_export_values`. Here're some examples to decode json and extract the value.
+        ```
+        // it will output "registry1.azurecr.io"
+        output "login_server" {
+        value = jsondecode(azapi_resource.example.output).properties.loginServer
+        }
         """
         return pulumi.get(self, "output")
 
     @output.setter
     def output(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "output", value)
 
@@ -459,16 +496,25 @@
     @property
     @pulumi.getter(name="responseExportValues")
     def response_export_values(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
         A list of path that needs to be exported from response body.
         Setting it to `["*"]` will export the full response body.
         Here's an example. If it sets to `["properties.loginServer", "properties.policies.quarantinePolicy.status"]`, it will set the following json to computed property `output`.
-        ```python
-        import pulumi
+        ```
+        {
+        "properties" : {
+        "loginServer" : "registry1.azurecr.io"
+        "policies" : {
+        "quarantinePolicy" = {
+        "status" = "disabled"
+        }
+        }
+        }
+        }
         ```
         """
         return pulumi.get(self, "response_export_values")
 
     @response_export_values.setter
     def response_export_values(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "response_export_values", value)
@@ -529,27 +575,19 @@
                  schema_validation_enabled: Optional[pulumi.Input[bool]] = None,
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  type: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         This resource can manage any Azure resource manager resource.
 
-        ## Import
-
-        Azure resource can be imported using the `resource id`, e.g.
-
-        ```sh
-         $ pulumi import azapi:index/resource:Resource example /subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/resGroup1/providers/Microsoft.MachineLearningServices/workspaces/workspace1/computes/cluster1
-        ```
+        ## Example Usage
 
-         It also supports specifying API version by using the `resource id` with `api-version` as a query parameter, e.g.
+        ## Import
 
-        ```sh
-         $ pulumi import azapi:index/resource:Resource example /subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/resGroup1/providers/Microsoft.MachineLearningServices/workspaces/workspace1/computes/cluster1?api-version=2021-07-01
-        ```
+        Azure resource can be imported using the `resource id`, e.g. <break><break>```sh<break> $ pulumi import azapi:index/resource:Resource example /subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/resGroup1/providers/Microsoft.MachineLearningServices/workspaces/workspace1/computes/cluster1 <break>```<break><break> It also supports specifying API version by using the `resource id` with `api-version` as a query parameter, e.g. <break><break>```sh<break> $ pulumi import azapi:index/resource:Resource example /subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/resGroup1/providers/Microsoft.MachineLearningServices/workspaces/workspace1/computes/cluster1?api-version=2021-07-01 <break>```<break><break>
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] body: A JSON object that contains the request body used to create and update azure resource.
         :param pulumi.Input[pulumi.InputType['ResourceIdentityArgs']] identity: A `identity` block as defined below.
         :param pulumi.Input[bool] ignore_casing: Whether ignore incorrect casing returned in `body` to suppress plan-diff. Defaults to `false`.
         :param pulumi.Input[bool] ignore_missing_property: Whether ignore not returned properties like credentials in `body` to suppress plan-diff. Defaults to `true`.
@@ -564,16 +602,25 @@
                - tenant scope: `parent_id` should be `/`
                
                For child level resources, the `parent_id` should be the ID of its parent resource, for example, subnet resource's `parent_id` is the ID of the vnet.
         :param pulumi.Input[bool] removing_special_chars: Whether to remove special characters in resource name. Defaults to `false`.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] response_export_values: A list of path that needs to be exported from response body.
                Setting it to `["*"]` will export the full response body.
                Here's an example. If it sets to `["properties.loginServer", "properties.policies.quarantinePolicy.status"]`, it will set the following json to computed property `output`.
-               ```python
-               import pulumi
+               ```
+               {
+               "properties" : {
+               "loginServer" : "registry1.azurecr.io"
+               "policies" : {
+               "quarantinePolicy" = {
+               "status" = "disabled"
+               }
+               }
+               }
+               }
                ```
         :param pulumi.Input[bool] schema_validation_enabled: Whether enabled the validation on `type` and `body` with embedded schema. Defaults to `true`.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: A mapping of tags which should be assigned to the azure resource.
         :param pulumi.Input[str] type: It is in a format like `<resource-type>@<api-version>`. `<resource-type>` is the Azure resource type, for example, `Microsoft.Storage/storageAccounts`.
                `<api-version>` is version of the API used to manage this azure resource.
         """
         ...
@@ -581,27 +628,19 @@
     def __init__(__self__,
                  resource_name: str,
                  args: ResourceArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         This resource can manage any Azure resource manager resource.
 
-        ## Import
-
-        Azure resource can be imported using the `resource id`, e.g.
+        ## Example Usage
 
-        ```sh
-         $ pulumi import azapi:index/resource:Resource example /subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/resGroup1/providers/Microsoft.MachineLearningServices/workspaces/workspace1/computes/cluster1
-        ```
+        ## Import
 
-         It also supports specifying API version by using the `resource id` with `api-version` as a query parameter, e.g.
-
-        ```sh
-         $ pulumi import azapi:index/resource:Resource example /subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/resGroup1/providers/Microsoft.MachineLearningServices/workspaces/workspace1/computes/cluster1?api-version=2021-07-01
-        ```
+        Azure resource can be imported using the `resource id`, e.g. <break><break>```sh<break> $ pulumi import azapi:index/resource:Resource example /subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/resGroup1/providers/Microsoft.MachineLearningServices/workspaces/workspace1/computes/cluster1 <break>```<break><break> It also supports specifying API version by using the `resource id` with `api-version` as a query parameter, e.g. <break><break>```sh<break> $ pulumi import azapi:index/resource:Resource example /subscriptions/00000000-0000-0000-0000-000000000000/resourceGroups/resGroup1/providers/Microsoft.MachineLearningServices/workspaces/workspace1/computes/cluster1?api-version=2021-07-01 <break>```<break><break>
 
         :param str resource_name: The name of the resource.
         :param ResourceArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
@@ -689,28 +728,42 @@
         :param pulumi.Input[pulumi.InputType['ResourceIdentityArgs']] identity: A `identity` block as defined below.
         :param pulumi.Input[bool] ignore_casing: Whether ignore incorrect casing returned in `body` to suppress plan-diff. Defaults to `false`.
         :param pulumi.Input[bool] ignore_missing_property: Whether ignore not returned properties like credentials in `body` to suppress plan-diff. Defaults to `true`.
         :param pulumi.Input[str] location: The Azure Region where the azure resource should exist.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] locks: A list of ARM resource IDs which are used to avoid create/modify/delete azapi resources at the same time.
         :param pulumi.Input[str] name: Specifies the name of the azure resource. Changing this forces a new resource to be created.
         :param pulumi.Input[str] output: The output json containing the properties specified in `response_export_values`. Here're some examples to decode json and extract the value.
+               ```
+               // it will output "registry1.azurecr.io"
+               output "login_server" {
+               value = jsondecode(azapi_resource.example.output).properties.loginServer
+               }
         :param pulumi.Input[str] parent_id: The ID of the azure resource in which this resource is created. Changing this forces a new resource to be created. It supports different kinds of deployment scope for **top level** resources: 
                - resource group scope: `parent_id` should be the ID of a resource group, it's recommended to manage a resource group by azurerm_resource_group.
                - management group scope: `parent_id` should be the ID of a management group, it's recommended to manage a management group by azurerm_management_group.
                - extension scope: `parent_id` should be the ID of the resource you're adding the extension to.
                - subscription scope: `parent_id` should be like `/subscriptions/00000000-0000-0000-0000-000000000000`
                - tenant scope: `parent_id` should be `/`
                
                For child level resources, the `parent_id` should be the ID of its parent resource, for example, subnet resource's `parent_id` is the ID of the vnet.
         :param pulumi.Input[bool] removing_special_chars: Whether to remove special characters in resource name. Defaults to `false`.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] response_export_values: A list of path that needs to be exported from response body.
                Setting it to `["*"]` will export the full response body.
                Here's an example. If it sets to `["properties.loginServer", "properties.policies.quarantinePolicy.status"]`, it will set the following json to computed property `output`.
-               ```python
-               import pulumi
+               ```
+               {
+               "properties" : {
+               "loginServer" : "registry1.azurecr.io"
+               "policies" : {
+               "quarantinePolicy" = {
+               "status" = "disabled"
+               }
+               }
+               }
+               }
                ```
         :param pulumi.Input[bool] schema_validation_enabled: Whether enabled the validation on `type` and `body` with embedded schema. Defaults to `true`.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: A mapping of tags which should be assigned to the azure resource.
         :param pulumi.Input[str] type: It is in a format like `<resource-type>@<api-version>`. `<resource-type>` is the Azure resource type, for example, `Microsoft.Storage/storageAccounts`.
                `<api-version>` is version of the API used to manage this azure resource.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
@@ -790,14 +843,19 @@
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def output(self) -> pulumi.Output[str]:
         """
         The output json containing the properties specified in `response_export_values`. Here're some examples to decode json and extract the value.
+        ```
+        // it will output "registry1.azurecr.io"
+        output "login_server" {
+        value = jsondecode(azapi_resource.example.output).properties.loginServer
+        }
         """
         return pulumi.get(self, "output")
 
     @property
     @pulumi.getter(name="parentId")
     def parent_id(self) -> pulumi.Output[str]:
         """
@@ -823,16 +881,25 @@
     @property
     @pulumi.getter(name="responseExportValues")
     def response_export_values(self) -> pulumi.Output[Optional[Sequence[str]]]:
         """
         A list of path that needs to be exported from response body.
         Setting it to `["*"]` will export the full response body.
         Here's an example. If it sets to `["properties.loginServer", "properties.policies.quarantinePolicy.status"]`, it will set the following json to computed property `output`.
-        ```python
-        import pulumi
+        ```
+        {
+        "properties" : {
+        "loginServer" : "registry1.azurecr.io"
+        "policies" : {
+        "quarantinePolicy" = {
+        "status" = "disabled"
+        }
+        }
+        }
+        }
         ```
         """
         return pulumi.get(self, "response_export_values")
 
     @property
     @pulumi.getter(name="schemaValidationEnabled")
     def schema_validation_enabled(self) -> pulumi.Output[Optional[bool]]:
```

### Comparing `ediri_azapi-1.6.0/ediri_azapi/resource_action.py` & `ediri_azapi-1.7.0/ediri_azapi/resource_action.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,16 +29,29 @@
         :param pulumi.Input[str] action: The name of the resource action. It's also possible to make Http requests towards the resource ID if leave this field empty.
         :param pulumi.Input[str] body: A JSON object that contains the request body.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] locks: A list of ARM resource IDs which are used to avoid modify azapi resources at the same time.
         :param pulumi.Input[str] method: Specifies the Http method of the azure resource action. Allowed values are `POST`, `PATCH`, `PUT` and `DELETE`. Defaults to `POST`.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] response_export_values: A list of path that needs to be exported from response body.
                Setting it to `["*"]` will export the full response body.
                Here's an example. If it sets to `["keys"]`, it will set the following json to computed property `output`.
-               ```python
-               import pulumi
+               ```
+               {
+               "keys": [
+               {
+               "KeyName": "Primary",
+               "Permissions": "Full",
+               "Value": "nHGYNd******i4wdug=="
+               },
+               {
+               "KeyName": "Secondary",
+               "Permissions": "Full",
+               "Value": "6yoCad******SLzKzg=="
+               }
+               ]
+               }
                ```
         """
         pulumi.set(__self__, "resource_id", resource_id)
         pulumi.set(__self__, "type", type)
         if action is not None:
             pulumi.set(__self__, "action", action)
         if body is not None:
@@ -126,16 +139,29 @@
     @property
     @pulumi.getter(name="responseExportValues")
     def response_export_values(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
         A list of path that needs to be exported from response body.
         Setting it to `["*"]` will export the full response body.
         Here's an example. If it sets to `["keys"]`, it will set the following json to computed property `output`.
-        ```python
-        import pulumi
+        ```
+        {
+        "keys": [
+        {
+        "KeyName": "Primary",
+        "Permissions": "Full",
+        "Value": "nHGYNd******i4wdug=="
+        },
+        {
+        "KeyName": "Secondary",
+        "Permissions": "Full",
+        "Value": "6yoCad******SLzKzg=="
+        }
+        ]
+        }
         ```
         """
         return pulumi.get(self, "response_export_values")
 
     @response_export_values.setter
     def response_export_values(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "response_export_values", value)
@@ -159,16 +185,29 @@
         :param pulumi.Input[Sequence[pulumi.Input[str]]] locks: A list of ARM resource IDs which are used to avoid modify azapi resources at the same time.
         :param pulumi.Input[str] method: Specifies the Http method of the azure resource action. Allowed values are `POST`, `PATCH`, `PUT` and `DELETE`. Defaults to `POST`.
         :param pulumi.Input[str] output: The output json containing the properties specified in `response_export_values`. Here are some examples to decode json and extract the value.
         :param pulumi.Input[str] resource_id: The ID of an existing azure source.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] response_export_values: A list of path that needs to be exported from response body.
                Setting it to `["*"]` will export the full response body.
                Here's an example. If it sets to `["keys"]`, it will set the following json to computed property `output`.
-               ```python
-               import pulumi
+               ```
+               {
+               "keys": [
+               {
+               "KeyName": "Primary",
+               "Permissions": "Full",
+               "Value": "nHGYNd******i4wdug=="
+               },
+               {
+               "KeyName": "Secondary",
+               "Permissions": "Full",
+               "Value": "6yoCad******SLzKzg=="
+               }
+               ]
+               }
                ```
         :param pulumi.Input[str] type: It is in a format like `<resource-type>@<api-version>`. `<resource-type>` is the Azure resource type, for example, `Microsoft.Storage/storageAccounts`.
                `<api-version>` is version of the API used to manage this azure resource.
         """
         if action is not None:
             pulumi.set(__self__, "action", action)
         if body is not None:
@@ -261,16 +300,29 @@
     @property
     @pulumi.getter(name="responseExportValues")
     def response_export_values(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
         A list of path that needs to be exported from response body.
         Setting it to `["*"]` will export the full response body.
         Here's an example. If it sets to `["keys"]`, it will set the following json to computed property `output`.
-        ```python
-        import pulumi
+        ```
+        {
+        "keys": [
+        {
+        "KeyName": "Primary",
+        "Permissions": "Full",
+        "Value": "nHGYNd******i4wdug=="
+        },
+        {
+        "KeyName": "Secondary",
+        "Permissions": "Full",
+        "Value": "6yoCad******SLzKzg=="
+        }
+        ]
+        }
         ```
         """
         return pulumi.get(self, "response_export_values")
 
     @response_export_values.setter
     def response_export_values(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "response_export_values", value)
@@ -305,26 +357,41 @@
         """
         This resource can perform any Azure resource manager resource action.
         It's recommended to use `ResourceAction` resource to perform actions which change a resource's state, please use `ResourceAction` data source,
         if user wants to perform readonly action.
 
         > **Note** When delete `ResourceAction`, no operation will be performed.
 
+        ## Example Usage
+
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] action: The name of the resource action. It's also possible to make Http requests towards the resource ID if leave this field empty.
         :param pulumi.Input[str] body: A JSON object that contains the request body.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] locks: A list of ARM resource IDs which are used to avoid modify azapi resources at the same time.
         :param pulumi.Input[str] method: Specifies the Http method of the azure resource action. Allowed values are `POST`, `PATCH`, `PUT` and `DELETE`. Defaults to `POST`.
         :param pulumi.Input[str] resource_id: The ID of an existing azure source.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] response_export_values: A list of path that needs to be exported from response body.
                Setting it to `["*"]` will export the full response body.
                Here's an example. If it sets to `["keys"]`, it will set the following json to computed property `output`.
-               ```python
-               import pulumi
+               ```
+               {
+               "keys": [
+               {
+               "KeyName": "Primary",
+               "Permissions": "Full",
+               "Value": "nHGYNd******i4wdug=="
+               },
+               {
+               "KeyName": "Secondary",
+               "Permissions": "Full",
+               "Value": "6yoCad******SLzKzg=="
+               }
+               ]
+               }
                ```
         :param pulumi.Input[str] type: It is in a format like `<resource-type>@<api-version>`. `<resource-type>` is the Azure resource type, for example, `Microsoft.Storage/storageAccounts`.
                `<api-version>` is version of the API used to manage this azure resource.
         """
         ...
     @overload
     def __init__(__self__,
@@ -334,14 +401,16 @@
         """
         This resource can perform any Azure resource manager resource action.
         It's recommended to use `ResourceAction` resource to perform actions which change a resource's state, please use `ResourceAction` data source,
         if user wants to perform readonly action.
 
         > **Note** When delete `ResourceAction`, no operation will be performed.
 
+        ## Example Usage
+
         :param str resource_name: The name of the resource.
         :param ResourceActionArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
         resource_args, opts = _utilities.get_resource_args_opts(ResourceActionArgs, pulumi.ResourceOptions, *args, **kwargs)
@@ -411,16 +480,29 @@
         :param pulumi.Input[Sequence[pulumi.Input[str]]] locks: A list of ARM resource IDs which are used to avoid modify azapi resources at the same time.
         :param pulumi.Input[str] method: Specifies the Http method of the azure resource action. Allowed values are `POST`, `PATCH`, `PUT` and `DELETE`. Defaults to `POST`.
         :param pulumi.Input[str] output: The output json containing the properties specified in `response_export_values`. Here are some examples to decode json and extract the value.
         :param pulumi.Input[str] resource_id: The ID of an existing azure source.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] response_export_values: A list of path that needs to be exported from response body.
                Setting it to `["*"]` will export the full response body.
                Here's an example. If it sets to `["keys"]`, it will set the following json to computed property `output`.
-               ```python
-               import pulumi
+               ```
+               {
+               "keys": [
+               {
+               "KeyName": "Primary",
+               "Permissions": "Full",
+               "Value": "nHGYNd******i4wdug=="
+               },
+               {
+               "KeyName": "Secondary",
+               "Permissions": "Full",
+               "Value": "6yoCad******SLzKzg=="
+               }
+               ]
+               }
                ```
         :param pulumi.Input[str] type: It is in a format like `<resource-type>@<api-version>`. `<resource-type>` is the Azure resource type, for example, `Microsoft.Storage/storageAccounts`.
                `<api-version>` is version of the API used to manage this azure resource.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _ResourceActionState.__new__(_ResourceActionState)
@@ -486,16 +568,29 @@
     @property
     @pulumi.getter(name="responseExportValues")
     def response_export_values(self) -> pulumi.Output[Optional[Sequence[str]]]:
         """
         A list of path that needs to be exported from response body.
         Setting it to `["*"]` will export the full response body.
         Here's an example. If it sets to `["keys"]`, it will set the following json to computed property `output`.
-        ```python
-        import pulumi
+        ```
+        {
+        "keys": [
+        {
+        "KeyName": "Primary",
+        "Permissions": "Full",
+        "Value": "nHGYNd******i4wdug=="
+        },
+        {
+        "KeyName": "Secondary",
+        "Permissions": "Full",
+        "Value": "6yoCad******SLzKzg=="
+        }
+        ]
+        }
         ```
         """
         return pulumi.get(self, "response_export_values")
 
     @property
     @pulumi.getter
     def type(self) -> pulumi.Output[str]:
```

### Comparing `ediri_azapi-1.6.0/ediri_azapi/update_resource.py` & `ediri_azapi-1.7.0/ediri_azapi/update_resource.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,16 +42,25 @@
                For child level resources, the `parent_id` should be the ID of its parent resource, for example, subnet resource's `parent_id` is the ID of the vnet.
         :param pulumi.Input[str] resource_id: The ID of an existing azure source. Changing this forces a new azure resource to be created.
                
                > **Note:** Configuring `name` and `parent_id` is an alternative way to configure `resource_id`.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] response_export_values: A list of path that needs to be exported from response body.
                Setting it to `["*"]` will export the full response body.
                Here's an example. If it sets to `["properties.loginServer", "properties.policies.quarantinePolicy.status"]`, it will set the following json to computed property `output`.
-               ```python
-               import pulumi
+               ```
+               {
+               "properties" : {
+               "loginServer" : "registry1.azurecr.io"
+               "policies" : {
+               "quarantinePolicy" = {
+               "status" = "disabled"
+               }
+               }
+               }
+               }
                ```
         """
         pulumi.set(__self__, "type", type)
         if body is not None:
             pulumi.set(__self__, "body", body)
         if ignore_casing is not None:
             pulumi.set(__self__, "ignore_casing", ignore_casing)
@@ -177,16 +186,25 @@
     @property
     @pulumi.getter(name="responseExportValues")
     def response_export_values(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
         A list of path that needs to be exported from response body.
         Setting it to `["*"]` will export the full response body.
         Here's an example. If it sets to `["properties.loginServer", "properties.policies.quarantinePolicy.status"]`, it will set the following json to computed property `output`.
-        ```python
-        import pulumi
+        ```
+        {
+        "properties" : {
+        "loginServer" : "registry1.azurecr.io"
+        "policies" : {
+        "quarantinePolicy" = {
+        "status" = "disabled"
+        }
+        }
+        }
+        }
         ```
         """
         return pulumi.get(self, "response_export_values")
 
     @response_export_values.setter
     def response_export_values(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "response_export_values", value)
@@ -209,30 +227,44 @@
         Input properties used for looking up and filtering UpdateResource resources.
         :param pulumi.Input[str] body: A JSON object that contains the request body used to add on an existing azure resource.
         :param pulumi.Input[bool] ignore_casing: Whether ignore incorrect casing returned in `body` to suppress plan-diff. Defaults to `false`.
         :param pulumi.Input[bool] ignore_missing_property: Whether ignore not returned properties like credentials in `body` to suppress plan-diff. Defaults to `true`.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] locks: A list of ARM resource IDs which are used to avoid create/modify/delete azapi resources at the same time.
         :param pulumi.Input[str] name: Specifies the name of the azure resource. Changing this forces a new resource to be created.
         :param pulumi.Input[str] output: The output json containing the properties specified in `response_export_values`. Here're some examples to decode json and extract the value.
+               ```
+               // it will output "registry1.azurecr.io"
+               output "login_server" {
+               value = jsondecode(azapi_resource.example.output).properties.loginServer
+               }
         :param pulumi.Input[str] parent_id: The ID of the azure resource in which this resource is created. Changing this forces a new resource to be created. It supports different kinds of deployment scope for **top level** resources: 
                - resource group scope: `parent_id` should be the ID of a resource group, it's recommended to manage a resource group by azurerm_resource_group.
                - management group scope: `parent_id` should be the ID of a management group, it's recommended to manage a management group by azurerm_management_group.
                - extension scope: `parent_id` should be the ID of the resource you're adding the extension to.
                - subscription scope: `parent_id` should be like `/subscriptions/00000000-0000-0000-0000-000000000000`
                - tenant scope: `parent_id` should be `/`
                
                For child level resources, the `parent_id` should be the ID of its parent resource, for example, subnet resource's `parent_id` is the ID of the vnet.
         :param pulumi.Input[str] resource_id: The ID of an existing azure source. Changing this forces a new azure resource to be created.
                
                > **Note:** Configuring `name` and `parent_id` is an alternative way to configure `resource_id`.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] response_export_values: A list of path that needs to be exported from response body.
                Setting it to `["*"]` will export the full response body.
                Here's an example. If it sets to `["properties.loginServer", "properties.policies.quarantinePolicy.status"]`, it will set the following json to computed property `output`.
-               ```python
-               import pulumi
+               ```
+               {
+               "properties" : {
+               "loginServer" : "registry1.azurecr.io"
+               "policies" : {
+               "quarantinePolicy" = {
+               "status" = "disabled"
+               }
+               }
+               }
+               }
                ```
         :param pulumi.Input[str] type: It is in a format like `<resource-type>@<api-version>`. `<resource-type>` is the Azure resource type, for example, `Microsoft.Storage/storageAccounts`.
                `<api-version>` is version of the API used to manage this azure resource.
         """
         if body is not None:
             pulumi.set(__self__, "body", body)
         if ignore_casing is not None:
@@ -315,14 +347,19 @@
         pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter
     def output(self) -> Optional[pulumi.Input[str]]:
         """
         The output json containing the properties specified in `response_export_values`. Here're some examples to decode json and extract the value.
+        ```
+        // it will output "registry1.azurecr.io"
+        output "login_server" {
+        value = jsondecode(azapi_resource.example.output).properties.loginServer
+        }
         """
         return pulumi.get(self, "output")
 
     @output.setter
     def output(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "output", value)
 
@@ -362,16 +399,25 @@
     @property
     @pulumi.getter(name="responseExportValues")
     def response_export_values(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
         A list of path that needs to be exported from response body.
         Setting it to `["*"]` will export the full response body.
         Here's an example. If it sets to `["properties.loginServer", "properties.policies.quarantinePolicy.status"]`, it will set the following json to computed property `output`.
-        ```python
-        import pulumi
+        ```
+        {
+        "properties" : {
+        "loginServer" : "registry1.azurecr.io"
+        "policies" : {
+        "quarantinePolicy" = {
+        "status" = "disabled"
+        }
+        }
+        }
+        }
         ```
         """
         return pulumi.get(self, "response_export_values")
 
     @response_export_values.setter
     def response_export_values(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "response_export_values", value)
@@ -408,14 +454,16 @@
         """
         This resource can manage a subset of any existing Azure resource manager resource's properties.
 
         > **Note** This resource is used to add or modify properties on an existing resource.
         When delete `UpdateResource`, no operation will be performed, and these properties will stay unchanged.
         If you want to restore the modified properties to some values, you must apply the restored properties before deleting.
 
+        ## Example Usage
+
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] body: A JSON object that contains the request body used to add on an existing azure resource.
         :param pulumi.Input[bool] ignore_casing: Whether ignore incorrect casing returned in `body` to suppress plan-diff. Defaults to `false`.
         :param pulumi.Input[bool] ignore_missing_property: Whether ignore not returned properties like credentials in `body` to suppress plan-diff. Defaults to `true`.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] locks: A list of ARM resource IDs which are used to avoid create/modify/delete azapi resources at the same time.
         :param pulumi.Input[str] name: Specifies the name of the azure resource. Changing this forces a new resource to be created.
@@ -429,16 +477,25 @@
                For child level resources, the `parent_id` should be the ID of its parent resource, for example, subnet resource's `parent_id` is the ID of the vnet.
         :param pulumi.Input[str] resource_id: The ID of an existing azure source. Changing this forces a new azure resource to be created.
                
                > **Note:** Configuring `name` and `parent_id` is an alternative way to configure `resource_id`.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] response_export_values: A list of path that needs to be exported from response body.
                Setting it to `["*"]` will export the full response body.
                Here's an example. If it sets to `["properties.loginServer", "properties.policies.quarantinePolicy.status"]`, it will set the following json to computed property `output`.
-               ```python
-               import pulumi
+               ```
+               {
+               "properties" : {
+               "loginServer" : "registry1.azurecr.io"
+               "policies" : {
+               "quarantinePolicy" = {
+               "status" = "disabled"
+               }
+               }
+               }
+               }
                ```
         :param pulumi.Input[str] type: It is in a format like `<resource-type>@<api-version>`. `<resource-type>` is the Azure resource type, for example, `Microsoft.Storage/storageAccounts`.
                `<api-version>` is version of the API used to manage this azure resource.
         """
         ...
     @overload
     def __init__(__self__,
@@ -448,14 +505,16 @@
         """
         This resource can manage a subset of any existing Azure resource manager resource's properties.
 
         > **Note** This resource is used to add or modify properties on an existing resource.
         When delete `UpdateResource`, no operation will be performed, and these properties will stay unchanged.
         If you want to restore the modified properties to some values, you must apply the restored properties before deleting.
 
+        ## Example Usage
+
         :param str resource_name: The name of the resource.
         :param UpdateResourceArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
         resource_args, opts = _utilities.get_resource_args_opts(UpdateResourceArgs, pulumi.ResourceOptions, *args, **kwargs)
@@ -526,30 +585,44 @@
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] body: A JSON object that contains the request body used to add on an existing azure resource.
         :param pulumi.Input[bool] ignore_casing: Whether ignore incorrect casing returned in `body` to suppress plan-diff. Defaults to `false`.
         :param pulumi.Input[bool] ignore_missing_property: Whether ignore not returned properties like credentials in `body` to suppress plan-diff. Defaults to `true`.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] locks: A list of ARM resource IDs which are used to avoid create/modify/delete azapi resources at the same time.
         :param pulumi.Input[str] name: Specifies the name of the azure resource. Changing this forces a new resource to be created.
         :param pulumi.Input[str] output: The output json containing the properties specified in `response_export_values`. Here're some examples to decode json and extract the value.
+               ```
+               // it will output "registry1.azurecr.io"
+               output "login_server" {
+               value = jsondecode(azapi_resource.example.output).properties.loginServer
+               }
         :param pulumi.Input[str] parent_id: The ID of the azure resource in which this resource is created. Changing this forces a new resource to be created. It supports different kinds of deployment scope for **top level** resources: 
                - resource group scope: `parent_id` should be the ID of a resource group, it's recommended to manage a resource group by azurerm_resource_group.
                - management group scope: `parent_id` should be the ID of a management group, it's recommended to manage a management group by azurerm_management_group.
                - extension scope: `parent_id` should be the ID of the resource you're adding the extension to.
                - subscription scope: `parent_id` should be like `/subscriptions/00000000-0000-0000-0000-000000000000`
                - tenant scope: `parent_id` should be `/`
                
                For child level resources, the `parent_id` should be the ID of its parent resource, for example, subnet resource's `parent_id` is the ID of the vnet.
         :param pulumi.Input[str] resource_id: The ID of an existing azure source. Changing this forces a new azure resource to be created.
                
                > **Note:** Configuring `name` and `parent_id` is an alternative way to configure `resource_id`.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] response_export_values: A list of path that needs to be exported from response body.
                Setting it to `["*"]` will export the full response body.
                Here's an example. If it sets to `["properties.loginServer", "properties.policies.quarantinePolicy.status"]`, it will set the following json to computed property `output`.
-               ```python
-               import pulumi
+               ```
+               {
+               "properties" : {
+               "loginServer" : "registry1.azurecr.io"
+               "policies" : {
+               "quarantinePolicy" = {
+               "status" = "disabled"
+               }
+               }
+               }
+               }
                ```
         :param pulumi.Input[str] type: It is in a format like `<resource-type>@<api-version>`. `<resource-type>` is the Azure resource type, for example, `Microsoft.Storage/storageAccounts`.
                `<api-version>` is version of the API used to manage this azure resource.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _UpdateResourceState.__new__(_UpdateResourceState)
@@ -607,14 +680,19 @@
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def output(self) -> pulumi.Output[str]:
         """
         The output json containing the properties specified in `response_export_values`. Here're some examples to decode json and extract the value.
+        ```
+        // it will output "registry1.azurecr.io"
+        output "login_server" {
+        value = jsondecode(azapi_resource.example.output).properties.loginServer
+        }
         """
         return pulumi.get(self, "output")
 
     @property
     @pulumi.getter(name="parentId")
     def parent_id(self) -> pulumi.Output[str]:
         """
@@ -642,16 +720,25 @@
     @property
     @pulumi.getter(name="responseExportValues")
     def response_export_values(self) -> pulumi.Output[Optional[Sequence[str]]]:
         """
         A list of path that needs to be exported from response body.
         Setting it to `["*"]` will export the full response body.
         Here's an example. If it sets to `["properties.loginServer", "properties.policies.quarantinePolicy.status"]`, it will set the following json to computed property `output`.
-        ```python
-        import pulumi
+        ```
+        {
+        "properties" : {
+        "loginServer" : "registry1.azurecr.io"
+        "policies" : {
+        "quarantinePolicy" = {
+        "status" = "disabled"
+        }
+        }
+        }
+        }
         ```
         """
         return pulumi.get(self, "response_export_values")
 
     @property
     @pulumi.getter
     def type(self) -> pulumi.Output[str]:
```

### Comparing `ediri_azapi-1.6.0/ediri_azapi.egg-info/PKG-INFO` & `ediri_azapi-1.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: ediri-azapi
-Version: 1.6.0
+Name: ediri_azapi
+Version: 1.7.0
 Summary: A Pulumi package for creating and managing Azapi resources
 Home-page: https://github.com/dirien/pulumi-azapi
 License: Apache-2.0
 Project-URL: Repository, https://github.com/dirien/pulumi-azapi
 Keywords: pulumi azapi category/cloud
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `ediri_azapi-1.6.0/ediri_azapi.egg-info/SOURCES.txt` & `ediri_azapi-1.7.0/ediri_azapi.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 README.md
 setup.py
 ediri_azapi/__init__.py
 ediri_azapi/_inputs.py
 ediri_azapi/_utilities.py
+ediri_azapi/data_plane_resource.py
 ediri_azapi/get_resource.py
 ediri_azapi/get_resource_action.py
 ediri_azapi/outputs.py
 ediri_azapi/provider.py
 ediri_azapi/pulumi-plugin.json
 ediri_azapi/py.typed
 ediri_azapi/resource.py
```

### Comparing `ediri_azapi-1.6.0/setup.py` & `ediri_azapi-1.7.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "1.6.0"
-PLUGIN_VERSION = "1.6.0"
+VERSION = "1.7.0"
+PLUGIN_VERSION = "1.7.0"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'azapi', PLUGIN_VERSION, '--server', 'github://api.github.com/dirien/pulumi-azapi'])
         except OSError as error:
```

