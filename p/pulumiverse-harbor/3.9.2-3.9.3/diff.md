# Comparing `tmp/pulumiverse_harbor-3.9.2.tar.gz` & `tmp/pulumiverse_harbor-3.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumiverse_harbor-3.9.2.tar", last modified: Sun Jun 11 10:54:08 2023, max compression
+gzip compressed data, was "pulumiverse_harbor-3.9.3.tar", last modified: Sun Jul  2 08:26:58 2023, max compression
```

## Comparing `pulumiverse_harbor-3.9.2.tar` & `pulumiverse_harbor-3.9.3.tar`

### file list

```diff
@@ -1,44 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 10:54:08.391210 pulumiverse_harbor-3.9.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-06-11 10:54:08.391210 pulumiverse_harbor-3.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-06-11 10:54:08.000000 pulumiverse_harbor-3.9.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 10:54:08.387210 pulumiverse_harbor-3.9.2/pulumiverse_harbor/
--rw-r--r--   0 runner    (1001) docker     (123)     4487 2023-06-11 10:54:08.000000 pulumiverse_harbor-3.9.2/pulumiverse_harbor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12767 2023-06-11 10:54:08.000000 pulumiverse_harbor-3.9.2/pulumiverse_harbor/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8128 2023-06-11 10:54:08.000000 pulumiverse_harbor-3.9.2/pulumiverse_harbor/_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 10:54:08.391210 pulumiverse_harbor-3.9.2/pulumiverse_harbor/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-11 10:54:08.000000 pulumiverse_harbor-3.9.2/pulumiverse_harbor/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-06-11 10:54:08.000000 pulumiverse_harbor-3.9.2/pulumiverse_harbor/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)    45640 2023-06-11 10:54:08.000000 pulumiverse_harbor-3.9.2/pulumiverse_harbor/config_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)    14192 2023-06-11 10:54:08.000000 pulumiverse_harbor-3.9.2/pulumiverse_harbor/config_email.py
--rw-r--r--   0 runner    (1001) docker     (123)    13040 2023-06-11 10:54:08.000000 pulumiverse_harbor-3.9.2/pulumiverse_harbor/config_security.py
--rw-r--r--   0 runner    (1001) docker     (123)    12607 2023-06-11 10:54:08.000000 pulumiverse_harbor-3.9.2/pulumiverse_harbor/config_system.py
--rw-r--r--   0 runner    (1001) docker     (123)     6975 2023-06-11 10:54:08.000000 pulumiverse_harbor-3.9.2/pulumiverse_harbor/garbage_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3905 2023-06-11 10:54:08.000000 pulumiverse_harbor-3.9.2/pulumiverse_harbor/get_project.py
--rw-r--r--   0 runner    (1001) docker     (123)     4819 2023-06-11 10:54:08.000000 pulumiverse_harbor-3.9.2/pulumiverse_harbor/get_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     8584 2023-06-11 10:54:08.000000 pulumiverse_harbor-3.9.2/pulumiverse_harbor/group.py
--rw-r--r--   0 runner    (1001) docker     (123)    15948 2023-06-11 10:54:08.000000 pulumiverse_harbor-3.9.2/pulumiverse_harbor/immutable_tag_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     9424 2023-06-11 10:54:08.000000 pulumiverse_harbor-3.9.2/pulumiverse_harbor/interrogation_services.py
--rw-r--r--   0 runner    (1001) docker     (123)    10793 2023-06-11 10:54:08.000000 pulumiverse_harbor-3.9.2/pulumiverse_harbor/label.py
--rw-r--r--   0 runner    (1001) docker     (123)    10263 2023-06-11 10:54:08.000000 pulumiverse_harbor-3.9.2/pulumiverse_harbor/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    29919 2023-06-11 10:54:08.000000 pulumiverse_harbor-3.9.2/pulumiverse_harbor/project.py
--rw-r--r--   0 runner    (1001) docker     (123)    13597 2023-06-11 10:54:08.000000 pulumiverse_harbor-3.9.2/pulumiverse_harbor/project_member_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     9627 2023-06-11 10:54:08.000000 pulumiverse_harbor-3.9.2/pulumiverse_harbor/project_member_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    24030 2023-06-11 10:54:08.000000 pulumiverse_harbor-3.9.2/pulumiverse_harbor/project_webhook.py
--rw-r--r--   0 runner    (1001) docker     (123)     6949 2023-06-11 10:54:08.000000 pulumiverse_harbor-3.9.2/pulumiverse_harbor/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-11 10:54:08.000000 pulumiverse_harbor-3.9.2/pulumiverse_harbor/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 10:54:08.000000 pulumiverse_harbor-3.9.2/pulumiverse_harbor/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    15487 2023-06-11 10:54:08.000000 pulumiverse_harbor-3.9.2/pulumiverse_harbor/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)    24011 2023-06-11 10:54:08.000000 pulumiverse_harbor-3.9.2/pulumiverse_harbor/replication.py
--rw-r--r--   0 runner    (1001) docker     (123)    12510 2023-06-11 10:54:08.000000 pulumiverse_harbor-3.9.2/pulumiverse_harbor/retention_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)    22423 2023-06-11 10:54:08.000000 pulumiverse_harbor-3.9.2/pulumiverse_harbor/robot_account.py
--rw-r--r--   0 runner    (1001) docker     (123)     5715 2023-06-11 10:54:08.000000 pulumiverse_harbor-3.9.2/pulumiverse_harbor/tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)    12154 2023-06-11 10:54:08.000000 pulumiverse_harbor-3.9.2/pulumiverse_harbor/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 10:54:08.391210 pulumiverse_harbor-3.9.2/pulumiverse_harbor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-06-11 10:54:08.000000 pulumiverse_harbor-3.9.2/pulumiverse_harbor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-06-11 10:54:08.000000 pulumiverse_harbor-3.9.2/pulumiverse_harbor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 10:54:08.000000 pulumiverse_harbor-3.9.2/pulumiverse_harbor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 10:54:08.000000 pulumiverse_harbor-3.9.2/pulumiverse_harbor.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-11 10:54:08.000000 pulumiverse_harbor-3.9.2/pulumiverse_harbor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-11 10:54:08.000000 pulumiverse_harbor-3.9.2/pulumiverse_harbor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 10:54:08.391210 pulumiverse_harbor-3.9.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-06-11 10:54:08.000000 pulumiverse_harbor-3.9.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 08:26:58.430092 pulumiverse_harbor-3.9.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-07-02 08:26:58.430092 pulumiverse_harbor-3.9.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-07-02 08:26:58.000000 pulumiverse_harbor-3.9.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 08:26:58.426092 pulumiverse_harbor-3.9.3/pulumiverse_harbor/
+-rw-r--r--   0 runner    (1001) docker     (123)     4689 2023-07-02 08:26:58.000000 pulumiverse_harbor-3.9.3/pulumiverse_harbor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12767 2023-07-02 08:26:58.000000 pulumiverse_harbor-3.9.3/pulumiverse_harbor/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8128 2023-07-02 08:26:58.000000 pulumiverse_harbor-3.9.3/pulumiverse_harbor/_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 08:26:58.430092 pulumiverse_harbor-3.9.3/pulumiverse_harbor/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-02 08:26:58.000000 pulumiverse_harbor-3.9.3/pulumiverse_harbor/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-07-02 08:26:58.000000 pulumiverse_harbor-3.9.3/pulumiverse_harbor/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45640 2023-07-02 08:26:58.000000 pulumiverse_harbor-3.9.3/pulumiverse_harbor/config_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13736 2023-07-02 08:26:58.000000 pulumiverse_harbor-3.9.3/pulumiverse_harbor/config_email.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12496 2023-07-02 08:26:58.000000 pulumiverse_harbor-3.9.3/pulumiverse_harbor/config_security.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12057 2023-07-02 08:26:58.000000 pulumiverse_harbor-3.9.3/pulumiverse_harbor/config_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6555 2023-07-02 08:26:58.000000 pulumiverse_harbor-3.9.3/pulumiverse_harbor/garbage_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-07-02 08:26:58.000000 pulumiverse_harbor-3.9.3/pulumiverse_harbor/get_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-07-02 08:26:58.000000 pulumiverse_harbor-3.9.3/pulumiverse_harbor/get_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8156 2023-07-02 08:26:58.000000 pulumiverse_harbor-3.9.3/pulumiverse_harbor/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15274 2023-07-02 08:26:58.000000 pulumiverse_harbor-3.9.3/pulumiverse_harbor/immutable_tag_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9054 2023-07-02 08:26:58.000000 pulumiverse_harbor-3.9.3/pulumiverse_harbor/interrogation_services.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9703 2023-07-02 08:26:58.000000 pulumiverse_harbor-3.9.3/pulumiverse_harbor/label.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10263 2023-07-02 08:26:58.000000 pulumiverse_harbor-3.9.3/pulumiverse_harbor/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28683 2023-07-02 08:26:58.000000 pulumiverse_harbor-3.9.3/pulumiverse_harbor/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12861 2023-07-02 08:26:58.000000 pulumiverse_harbor-3.9.3/pulumiverse_harbor/project_member_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8949 2023-07-02 08:26:58.000000 pulumiverse_harbor-3.9.3/pulumiverse_harbor/project_member_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22644 2023-07-02 08:26:58.000000 pulumiverse_harbor-3.9.3/pulumiverse_harbor/project_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6949 2023-07-02 08:26:58.000000 pulumiverse_harbor-3.9.3/pulumiverse_harbor/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-02 08:26:58.000000 pulumiverse_harbor-3.9.3/pulumiverse_harbor/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8424 2023-07-02 08:26:58.000000 pulumiverse_harbor-3.9.3/pulumiverse_harbor/purge_audit_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 08:26:58.000000 pulumiverse_harbor-3.9.3/pulumiverse_harbor/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    15039 2023-07-02 08:26:58.000000 pulumiverse_harbor-3.9.3/pulumiverse_harbor/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21185 2023-07-02 08:26:58.000000 pulumiverse_harbor-3.9.3/pulumiverse_harbor/replication.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11052 2023-07-02 08:26:58.000000 pulumiverse_harbor-3.9.3/pulumiverse_harbor/retention_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16975 2023-07-02 08:26:58.000000 pulumiverse_harbor-3.9.3/pulumiverse_harbor/robot_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5377 2023-07-02 08:26:58.000000 pulumiverse_harbor-3.9.3/pulumiverse_harbor/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11616 2023-07-02 08:26:58.000000 pulumiverse_harbor-3.9.3/pulumiverse_harbor/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 08:26:58.430092 pulumiverse_harbor-3.9.3/pulumiverse_harbor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-07-02 08:26:58.000000 pulumiverse_harbor-3.9.3/pulumiverse_harbor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-07-02 08:26:58.000000 pulumiverse_harbor-3.9.3/pulumiverse_harbor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 08:26:58.000000 pulumiverse_harbor-3.9.3/pulumiverse_harbor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 08:26:58.000000 pulumiverse_harbor-3.9.3/pulumiverse_harbor.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-02 08:26:58.000000 pulumiverse_harbor-3.9.3/pulumiverse_harbor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-02 08:26:58.000000 pulumiverse_harbor-3.9.3/pulumiverse_harbor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 08:26:58.430092 pulumiverse_harbor-3.9.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-07-02 08:26:58.000000 pulumiverse_harbor-3.9.3/setup.py
```

### Comparing `pulumiverse_harbor-3.9.2/PKG-INFO` & `pulumiverse_harbor-3.9.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumiverse_harbor
-Version: 3.9.2
+Version: 3.9.3
 Summary: A Pulumi package for creating and managing Harbor resources.
 Home-page: https://www.pulumi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumiverse/pulumi-harbor
 Keywords: pulumi harbor category/utility
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumiverse_harbor-3.9.2/README.md` & `pulumiverse_harbor-3.9.3/README.md`

 * *Files identical despite different names*

### Comparing `pulumiverse_harbor-3.9.2/pulumiverse_harbor/__init__.py` & `pulumiverse_harbor-3.9.3/pulumiverse_harbor/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 from .interrogation_services import *
 from .label import *
 from .project import *
 from .project_member_group import *
 from .project_member_user import *
 from .project_webhook import *
 from .provider import *
+from .purge_audit_log import *
 from .registry import *
 from .replication import *
 from .retention_policy import *
 from .robot_account import *
 from .tasks import *
 from .user import *
 from ._inputs import *
@@ -142,14 +143,22 @@
   "fqn": "pulumiverse_harbor",
   "classes": {
    "harbor:index/projectWebhook:ProjectWebhook": "ProjectWebhook"
   }
  },
  {
   "pkg": "harbor",
+  "mod": "index/purgeAuditLog",
+  "fqn": "pulumiverse_harbor",
+  "classes": {
+   "harbor:index/purgeAuditLog:PurgeAuditLog": "PurgeAuditLog"
+  }
+ },
+ {
+  "pkg": "harbor",
   "mod": "index/registry",
   "fqn": "pulumiverse_harbor",
   "classes": {
    "harbor:index/registry:Registry": "Registry"
   }
  },
  {
```

### Comparing `pulumiverse_harbor-3.9.2/pulumiverse_harbor/_inputs.py` & `pulumiverse_harbor-3.9.3/pulumiverse_harbor/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_harbor-3.9.2/pulumiverse_harbor/_utilities.py` & `pulumiverse_harbor-3.9.3/pulumiverse_harbor/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_harbor-3.9.2/pulumiverse_harbor/config/vars.py` & `pulumiverse_harbor-3.9.3/pulumiverse_harbor/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_harbor-3.9.2/pulumiverse_harbor/config_auth.py` & `pulumiverse_harbor-3.9.3/pulumiverse_harbor/config_auth.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_harbor-3.9.2/pulumiverse_harbor/config_email.py` & `pulumiverse_harbor-3.9.3/pulumiverse_harbor/config_email.py`

 * *Files 4% similar despite different names*

```diff
@@ -205,44 +205,26 @@
                  email_port: Optional[pulumi.Input[int]] = None,
                  email_ssl: Optional[pulumi.Input[bool]] = None,
                  email_username: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         ## Example Usage
 
-        ```python
-        import pulumi
-        import pulumiverse_harbor as harbor
-
-        main = harbor.ConfigEmail("main",
-            email_from="dont_reply@acme.com",
-            email_host="server.acme.com")
-        ```
-
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: ConfigEmailArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         ## Example Usage
 
-        ```python
-        import pulumi
-        import pulumiverse_harbor as harbor
-
-        main = harbor.ConfigEmail("main",
-            email_from="dont_reply@acme.com",
-            email_host="server.acme.com")
-        ```
-
         :param str resource_name: The name of the resource.
         :param ConfigEmailArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
         resource_args, opts = _utilities.get_resource_args_opts(ConfigEmailArgs, pulumi.ResourceOptions, *args, **kwargs)
```

### Comparing `pulumiverse_harbor-3.9.2/pulumiverse_harbor/config_security.py` & `pulumiverse_harbor-3.9.3/pulumiverse_harbor/config_security.py`

 * *Files 12% similar despite different names*

```diff
@@ -129,35 +129,17 @@
                  opts: Optional[pulumi.ResourceOptions] = None,
                  cve_allowlists: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  expires_at: Optional[pulumi.Input[int]] = None,
                  __props__=None):
         """
         ## Example Usage
 
-        ```python
-        import pulumi
-        import pulumiverse_harbor as harbor
-
-        main = harbor.ConfigSecurity("main",
-            cve_allowlists=[
-                "CVE-456",
-                "CVE-123",
-            ],
-            expires_at=1701167767)
-        ```
-
         ## Import
 
-        The list can be imported using the `id` eg, `
-
-        ```sh
-         $ pulumi import harbor:index/configSecurity:ConfigSecurity main "7"
-        ```
-
-         ` > Note that at this point of time Harbor doesn't has any api endpoint for deleting this list. Only updating the records.
+        The list can be imported using the `id` eg, `<break><break>```sh<break> $ pulumi import harbor:index/configSecurity:ConfigSecurity main "7" <break>```<break><break>` > Note that at this point of time Harbor doesn't has any api endpoint for deleting this list. Only updating the records.
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] cve_allowlists: System allowlist. Vulnerabilities in this list will be ignored when pushing and pulling images. Should be in the format or `["CVE-123", "CVE-145"]` or `["CVE-123"]`
         :param pulumi.Input[int] expires_at: The time for expiration of the allowlist, in the form of seconds since epoch. This is an optional attribute, if it's not set the CVE allowlist does not expire.
         """
         ...
@@ -165,35 +147,17 @@
     def __init__(__self__,
                  resource_name: str,
                  args: ConfigSecurityArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         ## Example Usage
 
-        ```python
-        import pulumi
-        import pulumiverse_harbor as harbor
-
-        main = harbor.ConfigSecurity("main",
-            cve_allowlists=[
-                "CVE-456",
-                "CVE-123",
-            ],
-            expires_at=1701167767)
-        ```
-
         ## Import
 
-        The list can be imported using the `id` eg, `
-
-        ```sh
-         $ pulumi import harbor:index/configSecurity:ConfigSecurity main "7"
-        ```
-
-         ` > Note that at this point of time Harbor doesn't has any api endpoint for deleting this list. Only updating the records.
+        The list can be imported using the `id` eg, `<break><break>```sh<break> $ pulumi import harbor:index/configSecurity:ConfigSecurity main "7" <break>```<break><break>` > Note that at this point of time Harbor doesn't has any api endpoint for deleting this list. Only updating the records.
 
         :param str resource_name: The name of the resource.
         :param ConfigSecurityArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
```

### Comparing `pulumiverse_harbor-3.9.2/pulumiverse_harbor/config_system.py` & `pulumiverse_harbor-3.9.3/pulumiverse_harbor/config_system.py`

 * *Files 3% similar despite different names*

```diff
@@ -157,46 +157,26 @@
                  robot_name_prefix: Optional[pulumi.Input[str]] = None,
                  robot_token_expiration: Optional[pulumi.Input[int]] = None,
                  scanner_skip_update_pulltime: Optional[pulumi.Input[bool]] = None,
                  __props__=None):
         """
         ## Example Usage
 
-        ```python
-        import pulumi
-        import pulumiverse_harbor as harbor
-
-        main = harbor.ConfigSystem("main",
-            project_creation_restriction="adminonly",
-            robot_name_prefix="harbor@",
-            robot_token_expiration=30)
-        ```
-
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: Optional[ConfigSystemArgs] = None,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         ## Example Usage
 
-        ```python
-        import pulumi
-        import pulumiverse_harbor as harbor
-
-        main = harbor.ConfigSystem("main",
-            project_creation_restriction="adminonly",
-            robot_name_prefix="harbor@",
-            robot_token_expiration=30)
-        ```
-
         :param str resource_name: The name of the resource.
         :param ConfigSystemArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
         resource_args, opts = _utilities.get_resource_args_opts(ConfigSystemArgs, pulumi.ResourceOptions, *args, **kwargs)
```

### Comparing `pulumiverse_harbor-3.9.2/pulumiverse_harbor/garbage_collection.py` & `pulumiverse_harbor-3.9.3/pulumiverse_harbor/garbage_collection.py`

 * *Files 6% similar despite different names*

```diff
@@ -81,44 +81,26 @@
                  opts: Optional[pulumi.ResourceOptions] = None,
                  delete_untagged: Optional[pulumi.Input[bool]] = None,
                  schedule: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         ## Example Usage
 
-        ```python
-        import pulumi
-        import pulumiverse_harbor as harbor
-
-        main = harbor.GarbageCollection("main",
-            delete_untagged=True,
-            schedule="Daily")
-        ```
-
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: GarbageCollectionArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         ## Example Usage
 
-        ```python
-        import pulumi
-        import pulumiverse_harbor as harbor
-
-        main = harbor.GarbageCollection("main",
-            delete_untagged=True,
-            schedule="Daily")
-        ```
-
         :param str resource_name: The name of the resource.
         :param GarbageCollectionArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
         resource_args, opts = _utilities.get_resource_args_opts(GarbageCollectionArgs, pulumi.ResourceOptions, *args, **kwargs)
```

### Comparing `pulumiverse_harbor-3.9.2/pulumiverse_harbor/get_project.py` & `pulumiverse_harbor-3.9.3/pulumiverse_harbor/get_project.py`

 * *Files 24% similar despite different names*

```diff
@@ -80,44 +80,28 @@
             vulnerability_scanning=self.vulnerability_scanning)
 
 
 def get_project(name: Optional[str] = None,
                 opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetProjectResult:
     """
     ## Example Usage
-
-    ```python
-    import pulumi
-    import pulumi_harbor as harbor
-
-    main = harbor.get_project(name="library")
-    pulumi.export("projectId", main.id)
-    ```
     """
     __args__ = dict()
     __args__['name'] = name
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('harbor:index/getProject:getProject', __args__, opts=opts, typ=GetProjectResult).value
 
     return AwaitableGetProjectResult(
-        id=__ret__.id,
-        name=__ret__.name,
-        project_id=__ret__.project_id,
-        public=__ret__.public,
-        vulnerability_scanning=__ret__.vulnerability_scanning)
+        id=pulumi.get(__ret__, 'id'),
+        name=pulumi.get(__ret__, 'name'),
+        project_id=pulumi.get(__ret__, 'project_id'),
+        public=pulumi.get(__ret__, 'public'),
+        vulnerability_scanning=pulumi.get(__ret__, 'vulnerability_scanning'))
 
 
 @_utilities.lift_output_func(get_project)
 def get_project_output(name: Optional[pulumi.Input[str]] = None,
                        opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetProjectResult]:
     """
     ## Example Usage
-
-    ```python
-    import pulumi
-    import pulumi_harbor as harbor
-
-    main = harbor.get_project(name="library")
-    pulumi.export("projectId", main.id)
-    ```
     """
     ...
```

### Comparing `pulumiverse_harbor-3.9.2/pulumiverse_harbor/get_registry.py` & `pulumiverse_harbor-3.9.3/pulumiverse_harbor/get_registry.py`

 * *Files 4% similar despite different names*

```diff
@@ -107,47 +107,31 @@
             url=self.url)
 
 
 def get_registry(name: Optional[str] = None,
                  opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetRegistryResult:
     """
     ## Example Usage
-
-    ```python
-    import pulumi
-    import pulumi_harbor as harbor
-
-    main = harbor.get_registry(name="test_docker_harbor")
-    pulumi.export("harborRegistryId", main.id)
-    ```
     """
     __args__ = dict()
     __args__['name'] = name
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('harbor:index/getRegistry:getRegistry', __args__, opts=opts, typ=GetRegistryResult).value
 
     return AwaitableGetRegistryResult(
-        description=__ret__.description,
-        id=__ret__.id,
-        insecure=__ret__.insecure,
-        name=__ret__.name,
-        registry_id=__ret__.registry_id,
-        status=__ret__.status,
-        type=__ret__.type,
-        url=__ret__.url)
+        description=pulumi.get(__ret__, 'description'),
+        id=pulumi.get(__ret__, 'id'),
+        insecure=pulumi.get(__ret__, 'insecure'),
+        name=pulumi.get(__ret__, 'name'),
+        registry_id=pulumi.get(__ret__, 'registry_id'),
+        status=pulumi.get(__ret__, 'status'),
+        type=pulumi.get(__ret__, 'type'),
+        url=pulumi.get(__ret__, 'url'))
 
 
 @_utilities.lift_output_func(get_registry)
 def get_registry_output(name: Optional[pulumi.Input[str]] = None,
                         opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetRegistryResult]:
     """
     ## Example Usage
-
-    ```python
-    import pulumi
-    import pulumi_harbor as harbor
-
-    main = harbor.get_registry(name="test_docker_harbor")
-    pulumi.export("harborRegistryId", main.id)
-    ```
     """
     ...
```

### Comparing `pulumiverse_harbor-3.9.2/pulumiverse_harbor/group.py` & `pulumiverse_harbor-3.9.3/pulumiverse_harbor/group.py`

 * *Files 7% similar despite different names*

```diff
@@ -105,63 +105,33 @@
                  group_name: Optional[pulumi.Input[str]] = None,
                  group_type: Optional[pulumi.Input[int]] = None,
                  ldap_group_dn: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         ## Example Usage
 
-        ```python
-        import pulumi
-        import pulumiverse_harbor as harbor
-
-        storage_group = harbor.Group("storage-group",
-            group_name="storage-group",
-            group_type=3)
-        ```
-
         ## Import
 
-        An OIDC group can be imported using the `group id` eg, `
-
-        ```sh
-         $ pulumi import harbor:index/group:Group storage-group /usergroups/19
-        ```
-
-         `
+        An OIDC group can be imported using the `group id` eg, `<break><break>```sh<break> $ pulumi import harbor:index/group:Group storage-group /usergroups/19 <break>```<break><break>`
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: GroupArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         ## Example Usage
 
-        ```python
-        import pulumi
-        import pulumiverse_harbor as harbor
-
-        storage_group = harbor.Group("storage-group",
-            group_name="storage-group",
-            group_type=3)
-        ```
-
         ## Import
 
-        An OIDC group can be imported using the `group id` eg, `
-
-        ```sh
-         $ pulumi import harbor:index/group:Group storage-group /usergroups/19
-        ```
-
-         `
+        An OIDC group can be imported using the `group id` eg, `<break><break>```sh<break> $ pulumi import harbor:index/group:Group storage-group /usergroups/19 <break>```<break><break>`
 
         :param str resource_name: The name of the resource.
         :param GroupArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
```

### Comparing `pulumiverse_harbor-3.9.2/pulumiverse_harbor/immutable_tag_rule.py` & `pulumiverse_harbor-3.9.3/pulumiverse_harbor/immutable_tag_rule.py`

 * *Files 2% similar despite different names*

```diff
@@ -221,34 +221,17 @@
                  repo_matching: Optional[pulumi.Input[str]] = None,
                  tag_excluding: Optional[pulumi.Input[str]] = None,
                  tag_matching: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         ## Example Usage
 
-        ```python
-        import pulumi
-        import pulumiverse_harbor as harbor
-
-        main_project = harbor.Project("mainProject")
-        main_immutable_tag_rule = harbor.ImmutableTagRule("mainImmutableTagRule",
-            project_id=main_project.id,
-            repo_matching="**",
-            tag_excluding="latest")
-        ```
-
         ## Import
 
-        Harbor immutable tag rule can be imported using the `project and immutabletagrule ids` eg, `
-
-        ```sh
-         $ pulumi import harbor:index/immutableTagRule:ImmutableTagRule main /projects/4/immutabletagrules/25
-        ```
-
-         `
+        Harbor immutable tag rule can be imported using the `project and immutabletagrule ids` eg, `<break><break>```sh<break> $ pulumi import harbor:index/immutableTagRule:ImmutableTagRule main /projects/4/immutabletagrules/25 <break>```<break><break>`
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[bool] disabled: Specify if the rule is disable or not. Defaults to `false`
         :param pulumi.Input[str] repo_excluding: For the repositories excuding.
         :param pulumi.Input[str] repo_matching: For the repositories matching.
         :param pulumi.Input[str] tag_excluding: For the tag excuding.
@@ -259,34 +242,17 @@
     def __init__(__self__,
                  resource_name: str,
                  args: ImmutableTagRuleArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         ## Example Usage
 
-        ```python
-        import pulumi
-        import pulumiverse_harbor as harbor
-
-        main_project = harbor.Project("mainProject")
-        main_immutable_tag_rule = harbor.ImmutableTagRule("mainImmutableTagRule",
-            project_id=main_project.id,
-            repo_matching="**",
-            tag_excluding="latest")
-        ```
-
         ## Import
 
-        Harbor immutable tag rule can be imported using the `project and immutabletagrule ids` eg, `
-
-        ```sh
-         $ pulumi import harbor:index/immutableTagRule:ImmutableTagRule main /projects/4/immutabletagrules/25
-        ```
-
-         `
+        Harbor immutable tag rule can be imported using the `project and immutabletagrule ids` eg, `<break><break>```sh<break> $ pulumi import harbor:index/immutableTagRule:ImmutableTagRule main /projects/4/immutabletagrules/25 <break>```<break><break>`
 
         :param str resource_name: The name of the resource.
         :param ImmutableTagRuleArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
```

### Comparing `pulumiverse_harbor-3.9.2/pulumiverse_harbor/interrogation_services.py` & `pulumiverse_harbor-3.9.3/pulumiverse_harbor/interrogation_services.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,42 +97,28 @@
                  opts: Optional[pulumi.ResourceOptions] = None,
                  default_scanner: Optional[pulumi.Input[str]] = None,
                  vulnerability_scan_policy: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         ## Example Usage
 
-        ```python
-        import pulumi
-        import pulumiverse_harbor as harbor
-
-        main = harbor.InterrogationServices("main", vulnerability_scan_policy="Daily")
-        ```
-
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] default_scanner: Sets the default interrogation service **Clair**
         :param pulumi.Input[str] vulnerability_scan_policy: The frequency of the vulnerability scanning is done. This can be `Daily`, `Weekly`, `Monthly` or can be a custom cron string.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: InterrogationServicesArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         ## Example Usage
 
-        ```python
-        import pulumi
-        import pulumiverse_harbor as harbor
-
-        main = harbor.InterrogationServices("main", vulnerability_scan_policy="Daily")
-        ```
-
         :param str resource_name: The name of the resource.
         :param InterrogationServicesArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
         resource_args, opts = _utilities.get_resource_args_opts(InterrogationServicesArgs, pulumi.ResourceOptions, *args, **kwargs)
```

### Comparing `pulumiverse_harbor-3.9.2/pulumiverse_harbor/label.py` & `pulumiverse_harbor-3.9.3/pulumiverse_harbor/label.py`

 * *Files 17% similar despite different names*

```diff
@@ -145,88 +145,40 @@
                  name: Optional[pulumi.Input[str]] = None,
                  project_id: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         ## Example Usage
 
         * Create a global label within harbor
-        ```python
-        import pulumi
-        import pulumiverse_harbor as harbor
-
-        main = harbor.Label("main",
-            color="#FF0000",
-            description="Description to for acceptance test")
-        ```
 
         * Creates a label for project
-        ```python
-        import pulumi
-        import pulumiverse_harbor as harbor
-
-        main_project = harbor.Project("mainProject")
-        main_label = harbor.Label("mainLabel",
-            color="#FFFFFF",
-            description="Description for acceptance test",
-            project_id=main_project.id)
-        ```
 
         ## Import
 
-        Harbor label can be imported using the `label id` eg, `
-
-        ```sh
-         $ pulumi import harbor:index/label:Label main /labels/1
-        ```
-
-         `
+        Harbor label can be imported using the `label id` eg, `<break><break>```sh<break> $ pulumi import harbor:index/label:Label main /labels/1 <break>```<break><break>`
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: Optional[LabelArgs] = None,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         ## Example Usage
 
         * Create a global label within harbor
-        ```python
-        import pulumi
-        import pulumiverse_harbor as harbor
-
-        main = harbor.Label("main",
-            color="#FF0000",
-            description="Description to for acceptance test")
-        ```
 
         * Creates a label for project
-        ```python
-        import pulumi
-        import pulumiverse_harbor as harbor
-
-        main_project = harbor.Project("mainProject")
-        main_label = harbor.Label("mainLabel",
-            color="#FFFFFF",
-            description="Description for acceptance test",
-            project_id=main_project.id)
-        ```
 
         ## Import
 
-        Harbor label can be imported using the `label id` eg, `
-
-        ```sh
-         $ pulumi import harbor:index/label:Label main /labels/1
-        ```
-
-         `
+        Harbor label can be imported using the `label id` eg, `<break><break>```sh<break> $ pulumi import harbor:index/label:Label main /labels/1 <break>```<break><break>`
 
         :param str resource_name: The name of the resource.
         :param LabelArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
```

### Comparing `pulumiverse_harbor-3.9.2/pulumiverse_harbor/outputs.py` & `pulumiverse_harbor-3.9.3/pulumiverse_harbor/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_harbor-3.9.2/pulumiverse_harbor/project.py` & `pulumiverse_harbor-3.9.3/pulumiverse_harbor/project.py`

 * *Files 3% similar despite different names*

```diff
@@ -345,45 +345,19 @@
                  registry_id: Optional[pulumi.Input[int]] = None,
                  storage_quota: Optional[pulumi.Input[int]] = None,
                  vulnerability_scanning: Optional[pulumi.Input[bool]] = None,
                  __props__=None):
         """
         ## Example Usage
 
-        ```python
-        import pulumi
-        import pulumiverse_harbor as harbor
-
-        main = harbor.Project("main",
-            enable_content_trust=True,
-            public="false",
-            vulnerability_scanning=True)
-        # (Optional) Default vale is true. Automatically scan images on push
-        ```
         ## Harbor project example as proxy cache
 
-        ```python
-        import pulumi
-        import pulumiverse_harbor as harbor
-
-        docker = harbor.Registry("docker",
-            provider_name="docker-hub",
-            endpoint_url="https://hub.docker.com")
-        main = harbor.Project("main", registry_id=docker.registry_id)
-        ```
-
         ## Import
 
-        Harbor project can be imported using the `project id` eg, `
-
-        ```sh
-         $ pulumi import harbor:index/project:Project main /projects/1
-        ```
-
-         `
+        Harbor project can be imported using the `project id` eg, `<break><break>```sh<break> $ pulumi import harbor:index/project:Project main /projects/1 <break>```<break><break>`
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] cve_allowlists: Project allowlist allows vulnerabilities in this list to be ignored in this project when pushing and pulling images. Should be in the format or `["CVE-123", "CVE-145"]` or `["CVE-123"]`
         :param pulumi.Input[str] deployment_security: Prevent deployment of images with vulnerability severity equal or higher than the specified value. Images must be scanned before this takes effect. Possible values: `critical`, `high`, `medium`, `low`, `none`. (Default: `""` - empty)
         :param pulumi.Input[bool] enable_content_trust: Enables Content Trust for project. When enabled it queries the embedded docker notary server. Can be set to `"true"` or `"false"` (Default: false)
         :param pulumi.Input[bool] force_destroy: A boolean that indicates all repositories should be deleted from the project so that the project can be destroyed without error. These repositories are *not* recoverable.
@@ -398,45 +372,19 @@
     def __init__(__self__,
                  resource_name: str,
                  args: Optional[ProjectArgs] = None,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         ## Example Usage
 
-        ```python
-        import pulumi
-        import pulumiverse_harbor as harbor
-
-        main = harbor.Project("main",
-            enable_content_trust=True,
-            public="false",
-            vulnerability_scanning=True)
-        # (Optional) Default vale is true. Automatically scan images on push
-        ```
         ## Harbor project example as proxy cache
 
-        ```python
-        import pulumi
-        import pulumiverse_harbor as harbor
-
-        docker = harbor.Registry("docker",
-            provider_name="docker-hub",
-            endpoint_url="https://hub.docker.com")
-        main = harbor.Project("main", registry_id=docker.registry_id)
-        ```
-
         ## Import
 
-        Harbor project can be imported using the `project id` eg, `
-
-        ```sh
-         $ pulumi import harbor:index/project:Project main /projects/1
-        ```
-
-         `
+        Harbor project can be imported using the `project id` eg, `<break><break>```sh<break> $ pulumi import harbor:index/project:Project main /projects/1 <break>```<break><break>`
 
         :param str resource_name: The name of the resource.
         :param ProjectArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
```

### Comparing `pulumiverse_harbor-3.9.2/pulumiverse_harbor/project_member_group.py` & `pulumiverse_harbor-3.9.3/pulumiverse_harbor/project_member_group.py`

 * *Files 6% similar despite different names*

```diff
@@ -191,69 +191,33 @@
                  project_id: Optional[pulumi.Input[str]] = None,
                  role: Optional[pulumi.Input[str]] = None,
                  type: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         ## Example Usage
 
-        ```python
-        import pulumi
-        import pulumiverse_harbor as harbor
-
-        main_project = harbor.Project("mainProject")
-        main_project_member_group = harbor.ProjectMemberGroup("mainProjectMemberGroup",
-            project_id=main_project.id,
-            group_name="testing1",
-            role="projectadmin",
-            type="oidc")
-        ```
-
         ## Import
 
-        Harbor project member group can be imported using the `project id` and `member id` eg, `
-
-        ```sh
-         $ pulumi import harbor:index/projectMemberGroup:ProjectMemberGroup main /projects/10/members/200
-        ```
-
-         `
+        Harbor project member group can be imported using the `project id` and `member id` eg, `<break><break>```sh<break> $ pulumi import harbor:index/projectMemberGroup:ProjectMemberGroup main /projects/10/members/200 <break>```<break><break>`
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: ProjectMemberGroupArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         ## Example Usage
 
-        ```python
-        import pulumi
-        import pulumiverse_harbor as harbor
-
-        main_project = harbor.Project("mainProject")
-        main_project_member_group = harbor.ProjectMemberGroup("mainProjectMemberGroup",
-            project_id=main_project.id,
-            group_name="testing1",
-            role="projectadmin",
-            type="oidc")
-        ```
-
         ## Import
 
-        Harbor project member group can be imported using the `project id` and `member id` eg, `
-
-        ```sh
-         $ pulumi import harbor:index/projectMemberGroup:ProjectMemberGroup main /projects/10/members/200
-        ```
-
-         `
+        Harbor project member group can be imported using the `project id` and `member id` eg, `<break><break>```sh<break> $ pulumi import harbor:index/projectMemberGroup:ProjectMemberGroup main /projects/10/members/200 <break>```<break><break>`
 
         :param str resource_name: The name of the resource.
         :param ProjectMemberGroupArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
```

### Comparing `pulumiverse_harbor-3.9.2/pulumiverse_harbor/project_member_user.py` & `pulumiverse_harbor-3.9.3/pulumiverse_harbor/project_member_user.py`

 * *Files 7% similar despite different names*

```diff
@@ -116,67 +116,33 @@
                  project_id: Optional[pulumi.Input[str]] = None,
                  role: Optional[pulumi.Input[str]] = None,
                  user_name: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         ## Example Usage
 
-        ```python
-        import pulumi
-        import pulumiverse_harbor as harbor
-
-        main_project = harbor.Project("mainProject")
-        main_project_member_user = harbor.ProjectMemberUser("mainProjectMemberUser",
-            project_id=main_project.id,
-            user_name="testing1",
-            role="projectadmin")
-        ```
-
         ## Import
 
-        Harbor project member user can be imported using the `project id` and `member id` eg, `
-
-        ```sh
-         $ pulumi import harbor:index/projectMemberUser:ProjectMemberUser main /projects/10/members/200
-        ```
-
-         `
+        Harbor project member user can be imported using the `project id` and `member id` eg, `<break><break>```sh<break> $ pulumi import harbor:index/projectMemberUser:ProjectMemberUser main /projects/10/members/200 <break>```<break><break>`
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: ProjectMemberUserArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         ## Example Usage
 
-        ```python
-        import pulumi
-        import pulumiverse_harbor as harbor
-
-        main_project = harbor.Project("mainProject")
-        main_project_member_user = harbor.ProjectMemberUser("mainProjectMemberUser",
-            project_id=main_project.id,
-            user_name="testing1",
-            role="projectadmin")
-        ```
-
         ## Import
 
-        Harbor project member user can be imported using the `project id` and `member id` eg, `
-
-        ```sh
-         $ pulumi import harbor:index/projectMemberUser:ProjectMemberUser main /projects/10/members/200
-        ```
-
-         `
+        Harbor project member user can be imported using the `project id` and `member id` eg, `<break><break>```sh<break> $ pulumi import harbor:index/projectMemberUser:ProjectMemberUser main /projects/10/members/200 <break>```<break><break>`
 
         :param str resource_name: The name of the resource.
         :param ProjectMemberUserArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
```

### Comparing `pulumiverse_harbor-3.9.2/pulumiverse_harbor/project_webhook.py` & `pulumiverse_harbor-3.9.3/pulumiverse_harbor/project_webhook.py`

 * *Files 4% similar despite different names*

```diff
@@ -325,36 +325,14 @@
                  notify_type: Optional[pulumi.Input[str]] = None,
                  project_id: Optional[pulumi.Input[str]] = None,
                  skip_cert_verify: Optional[pulumi.Input[bool]] = None,
                  __props__=None):
         """
         ## Example Usage
 
-        ```python
-        import pulumi
-        import pulumiverse_harbor as harbor
-
-        main_project = harbor.Project("mainProject")
-        main_project_webhook = harbor.ProjectWebhook("mainProjectWebhook",
-            address="https://webhook.domain.com",
-            project_id=main_project.id,
-            notify_type="http",
-            events_types=[
-                "DELETE_ARTIFACT",
-                "PULL_ARTIFACT",
-                "PUSH_ARTIFACT",
-                "QUOTA_EXCEED",
-                "QUOTA_WARNING",
-                "REPLICATION",
-                "SCANNING_FAILED",
-                "SCANNING_COMPLETED",
-                "TAG_RETENTION",
-            ])
-        ```
-
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] address: The address of the webhook
         :param pulumi.Input[str] auth_header: authentication header for you the webhook
         :param pulumi.Input[str] description: _ (Optional, string) A description of the webhook
         :param pulumi.Input[bool] enabled: , To enable / disable the webhook. Default `true`
         :param pulumi.Input[Sequence[pulumi.Input[str]]] events_types: ) The type events you want to subscript to can be `DELETE_ARTIFACT`, `PULL_ARTIFACT`, `PUSH_ARTIFACT`, `QUOTA_EXCEED`, `QUOTA_WARNING`, `REPLICATION`, `SCANNING_FAILED`, `SCANNING_COMPLETED`, `TAG_RETENTION`
@@ -368,36 +346,14 @@
     def __init__(__self__,
                  resource_name: str,
                  args: ProjectWebhookArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         ## Example Usage
 
-        ```python
-        import pulumi
-        import pulumiverse_harbor as harbor
-
-        main_project = harbor.Project("mainProject")
-        main_project_webhook = harbor.ProjectWebhook("mainProjectWebhook",
-            address="https://webhook.domain.com",
-            project_id=main_project.id,
-            notify_type="http",
-            events_types=[
-                "DELETE_ARTIFACT",
-                "PULL_ARTIFACT",
-                "PUSH_ARTIFACT",
-                "QUOTA_EXCEED",
-                "QUOTA_WARNING",
-                "REPLICATION",
-                "SCANNING_FAILED",
-                "SCANNING_COMPLETED",
-                "TAG_RETENTION",
-            ])
-        ```
-
         :param str resource_name: The name of the resource.
         :param ProjectWebhookArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
         resource_args, opts = _utilities.get_resource_args_opts(ProjectWebhookArgs, pulumi.ResourceOptions, *args, **kwargs)
```

### Comparing `pulumiverse_harbor-3.9.2/pulumiverse_harbor/provider.py` & `pulumiverse_harbor-3.9.3/pulumiverse_harbor/provider.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_harbor-3.9.2/pulumiverse_harbor/registry.py` & `pulumiverse_harbor-3.9.3/pulumiverse_harbor/registry.py`

 * *Files 11% similar despite different names*

```diff
@@ -229,63 +229,33 @@
                  insecure: Optional[pulumi.Input[bool]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  provider_name: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         ## Example Usage
 
-        ```python
-        import pulumi
-        import pulumiverse_harbor as harbor
-
-        main = harbor.Registry("main",
-            endpoint_url="https://hub.docker.com",
-            provider_name="docker-hub")
-        ```
-
         ## Import
 
-        Harbor project can be imported using the `registry id` eg, `
-
-        ```sh
-         $ pulumi import harbor:index/registry:Registry main /registries/7
-        ```
-
-         `
+        Harbor project can be imported using the `registry id` eg, `<break><break>```sh<break> $ pulumi import harbor:index/registry:Registry main /registries/7 <break>```<break><break>`
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: RegistryArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         ## Example Usage
 
-        ```python
-        import pulumi
-        import pulumiverse_harbor as harbor
-
-        main = harbor.Registry("main",
-            endpoint_url="https://hub.docker.com",
-            provider_name="docker-hub")
-        ```
-
         ## Import
 
-        Harbor project can be imported using the `registry id` eg, `
-
-        ```sh
-         $ pulumi import harbor:index/registry:Registry main /registries/7
-        ```
-
-         `
+        Harbor project can be imported using the `registry id` eg, `<break><break>```sh<break> $ pulumi import harbor:index/registry:Registry main /registries/7 <break>```<break><break>`
 
         :param str resource_name: The name of the resource.
         :param RegistryArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
```

### Comparing `pulumiverse_harbor-3.9.2/pulumiverse_harbor/replication.py` & `pulumiverse_harbor-3.9.3/pulumiverse_harbor/replication.py`

 * *Files 11% similar despite different names*

```diff
@@ -344,129 +344,33 @@
                  registry_id: Optional[pulumi.Input[int]] = None,
                  schedule: Optional[pulumi.Input[str]] = None,
                  speed: Optional[pulumi.Input[int]] = None,
                  __props__=None):
         """
         ## Example Usage
 
-        ```python
-        import pulumi
-        import pulumiverse_harbor as harbor
-
-        main = harbor.Registry("main",
-            provider_name="docker-hub",
-            endpoint_url="https://hub.docker.com")
-        push = harbor.Replication("push",
-            action="push",
-            registry_id=main.registry_id)
-        alpine_replication = harbor.Replication("alpineReplication",
-            action="pull",
-            registry_id=main.registry_id,
-            schedule="* 0/15 * * * *",
-            filters=[
-                harbor.ReplicationFilterArgs(
-                    name="library/alpine",
-                ),
-                harbor.ReplicationFilterArgs(
-                    tag="3.*.*",
-                ),
-                harbor.ReplicationFilterArgs(
-                    resource="artifact",
-                ),
-                harbor.ReplicationFilterArgs(
-                    labels=["qa"],
-                ),
-            ])
-        alpine_index_replication_replication = harbor.Replication("alpineIndex/replicationReplication",
-            action="pull",
-            registry_id=main.registry_id,
-            schedule="event_based",
-            filters=[
-                harbor.ReplicationFilterArgs(
-                    name="library/alpine",
-                ),
-                harbor.ReplicationFilterArgs(
-                    tag="3.*.*",
-                ),
-            ])
-        ```
-
         ## Import
 
-        Harbor project can be imported using the `replication id` eg, `
-
-        ```sh
-         $ pulumi import harbor:index/replication:Replication main /replication/policies/1
-        ```
-
-         `
+        Harbor project can be imported using the `replication id` eg, `<break><break>```sh<break> $ pulumi import harbor:index/replication:Replication main /replication/policies/1 <break>```<break><break>`
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: ReplicationArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         ## Example Usage
 
-        ```python
-        import pulumi
-        import pulumiverse_harbor as harbor
-
-        main = harbor.Registry("main",
-            provider_name="docker-hub",
-            endpoint_url="https://hub.docker.com")
-        push = harbor.Replication("push",
-            action="push",
-            registry_id=main.registry_id)
-        alpine_replication = harbor.Replication("alpineReplication",
-            action="pull",
-            registry_id=main.registry_id,
-            schedule="* 0/15 * * * *",
-            filters=[
-                harbor.ReplicationFilterArgs(
-                    name="library/alpine",
-                ),
-                harbor.ReplicationFilterArgs(
-                    tag="3.*.*",
-                ),
-                harbor.ReplicationFilterArgs(
-                    resource="artifact",
-                ),
-                harbor.ReplicationFilterArgs(
-                    labels=["qa"],
-                ),
-            ])
-        alpine_index_replication_replication = harbor.Replication("alpineIndex/replicationReplication",
-            action="pull",
-            registry_id=main.registry_id,
-            schedule="event_based",
-            filters=[
-                harbor.ReplicationFilterArgs(
-                    name="library/alpine",
-                ),
-                harbor.ReplicationFilterArgs(
-                    tag="3.*.*",
-                ),
-            ])
-        ```
-
         ## Import
 
-        Harbor project can be imported using the `replication id` eg, `
-
-        ```sh
-         $ pulumi import harbor:index/replication:Replication main /replication/policies/1
-        ```
-
-         `
+        Harbor project can be imported using the `replication id` eg, `<break><break>```sh<break> $ pulumi import harbor:index/replication:Replication main /replication/policies/1 <break>```<break><break>`
 
         :param str resource_name: The name of the resource.
         :param ReplicationArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
```

### Comparing `pulumiverse_harbor-3.9.2/pulumiverse_harbor/retention_policy.py` & `pulumiverse_harbor-3.9.3/pulumiverse_harbor/retention_policy.py`

 * *Files 4% similar despite different names*

```diff
@@ -131,45 +131,17 @@
                  rules: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['RetentionPolicyRuleArgs']]]]] = None,
                  schedule: Optional[pulumi.Input[str]] = None,
                  scope: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         ## Example Usage
 
-        ```python
-        import pulumi
-        import pulumiverse_harbor as harbor
-
-        main_project = harbor.Project("mainProject")
-        main_retention_policy = harbor.RetentionPolicy("mainRetentionPolicy",
-            scope=main_project.id,
-            schedule="Daily",
-            rules=[
-                harbor.RetentionPolicyRuleArgs(
-                    n_days_since_last_pull=5,
-                    repo_matching="**",
-                    tag_matching="latest",
-                ),
-                harbor.RetentionPolicyRuleArgs(
-                    n_days_since_last_push=10,
-                    repo_matching="**",
-                    tag_matching="{latest,snapshot}",
-                ),
-            ])
-        ```
-
         ## Import
 
-        Harbor retention policy can be imported using the `retention_policy id` eg, `
-
-        ```sh
-         $ pulumi import harbor:index/retentionPolicy:RetentionPolicy main /retentions/10
-        ```
-
-         `
+        Harbor retention policy can be imported using the `retention_policy id` eg, `<break><break>```sh<break> $ pulumi import harbor:index/retentionPolicy:RetentionPolicy main /retentions/10 <break>```<break><break>`
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['RetentionPolicyRuleArgs']]]] rules: Al collection of rule blocks as documented below.
         :param pulumi.Input[str] schedule: The schedule of when you would like the policy to run. This can be `Hourly`, `Daily`, `Weekly` or can be a custom cron string.
         :param pulumi.Input[str] scope: The project id of which you would like to apply this policy.
         """
@@ -178,45 +150,17 @@
     def __init__(__self__,
                  resource_name: str,
                  args: RetentionPolicyArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         ## Example Usage
 
-        ```python
-        import pulumi
-        import pulumiverse_harbor as harbor
-
-        main_project = harbor.Project("mainProject")
-        main_retention_policy = harbor.RetentionPolicy("mainRetentionPolicy",
-            scope=main_project.id,
-            schedule="Daily",
-            rules=[
-                harbor.RetentionPolicyRuleArgs(
-                    n_days_since_last_pull=5,
-                    repo_matching="**",
-                    tag_matching="latest",
-                ),
-                harbor.RetentionPolicyRuleArgs(
-                    n_days_since_last_push=10,
-                    repo_matching="**",
-                    tag_matching="{latest,snapshot}",
-                ),
-            ])
-        ```
-
         ## Import
 
-        Harbor retention policy can be imported using the `retention_policy id` eg, `
-
-        ```sh
-         $ pulumi import harbor:index/retentionPolicy:RetentionPolicy main /retentions/10
-        ```
-
-         `
+        Harbor retention policy can be imported using the `retention_policy id` eg, `<break><break>```sh<break> $ pulumi import harbor:index/retentionPolicy:RetentionPolicy main /retentions/10 <break>```<break><break>`
 
         :param str resource_name: The name of the resource.
         :param RetentionPolicyArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
```

### Comparing `pulumiverse_harbor-3.9.2/pulumiverse_harbor/robot_account.py` & `pulumiverse_harbor-3.9.3/pulumiverse_harbor/robot_account.py`

 * *Files 16% similar despite different names*

```diff
@@ -234,102 +234,29 @@
                  __props__=None):
         """
         ## # Resource: RobotAccount
 
         Harbor supports different levels of robot accounts. Currently `system` and `project` level robot accounts are supported.
 
         ## Example Usage
+
         ### System Level
         Introduced in harbor 2.2.0, system level robot accounts can have basically [all available permissions](https://github.com/goharbor/harbor/blob/-/src/common/rbac/const.go) in harbor and are not dependent on a single project.
 
-        ```python
-        import pulumi
-        import pulumi_random as random
-        import pulumiverse_harbor as harbor
-
-        password = random.RandomPassword("password",
-            length=12,
-            special=False)
-        main = harbor.Project("main")
-        system = harbor.RobotAccount("system",
-            description="system level robot account",
-            level="system",
-            secret=resource["random_password"]["password"]["result"],
-            permissions=[
-                harbor.RobotAccountPermissionArgs(
-                    accesses=[harbor.RobotAccountPermissionAccessArgs(
-                        action="create",
-                        resource="labels",
-                    )],
-                    kind="system",
-                    namespace="/",
-                ),
-                harbor.RobotAccountPermissionArgs(
-                    accesses=[
-                        harbor.RobotAccountPermissionAccessArgs(
-                            action="push",
-                            resource="repository",
-                        ),
-                        harbor.RobotAccountPermissionAccessArgs(
-                            action="read",
-                            resource="helm-chart",
-                        ),
-                        harbor.RobotAccountPermissionAccessArgs(
-                            action="read",
-                            resource="helm-chart-version",
-                        ),
-                    ],
-                    kind="project",
-                    namespace=main.name,
-                ),
-                harbor.RobotAccountPermissionArgs(
-                    accesses=[harbor.RobotAccountPermissionAccessArgs(
-                        action="pull",
-                        resource="repository",
-                    )],
-                    kind="project",
-                    namespace="*",
-                ),
-            ])
-        ```
-
         The above example, creates a system level robot account with permissions to
         - permission to create labels on system level
         - pull repository across all projects
         - push repository to project "my-project-name"
         - read helm-chart and helm-chart-version in project "my-project-name"
+
         ### Project Level
 
         Other than system level robot accounts, project level robot accounts can interact on project level only.
         The [available permissions](https://github.com/goharbor/harbor/blob/-/src/common/rbac/const.go) are mostly the same as for system level robots.
 
-        ```python
-        import pulumi
-        import pulumiverse_harbor as harbor
-
-        main = harbor.Project("main")
-        project = harbor.RobotAccount("project",
-            description="project level robot account",
-            level="project",
-            permissions=[harbor.RobotAccountPermissionArgs(
-                accesses=[
-                    harbor.RobotAccountPermissionAccessArgs(
-                        action="pull",
-                        resource="repository",
-                    ),
-                    harbor.RobotAccountPermissionAccessArgs(
-                        action="push",
-                        resource="repository",
-                    ),
-                ],
-                kind="project",
-                namespace=main.name,
-            )])
-        ```
-
         The above example creates a project level robot account with permissions to
         - pull repository on project "main"
         - push repository on project "main"
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
@@ -341,102 +268,29 @@
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         ## # Resource: RobotAccount
 
         Harbor supports different levels of robot accounts. Currently `system` and `project` level robot accounts are supported.
 
         ## Example Usage
+
         ### System Level
         Introduced in harbor 2.2.0, system level robot accounts can have basically [all available permissions](https://github.com/goharbor/harbor/blob/-/src/common/rbac/const.go) in harbor and are not dependent on a single project.
 
-        ```python
-        import pulumi
-        import pulumi_random as random
-        import pulumiverse_harbor as harbor
-
-        password = random.RandomPassword("password",
-            length=12,
-            special=False)
-        main = harbor.Project("main")
-        system = harbor.RobotAccount("system",
-            description="system level robot account",
-            level="system",
-            secret=resource["random_password"]["password"]["result"],
-            permissions=[
-                harbor.RobotAccountPermissionArgs(
-                    accesses=[harbor.RobotAccountPermissionAccessArgs(
-                        action="create",
-                        resource="labels",
-                    )],
-                    kind="system",
-                    namespace="/",
-                ),
-                harbor.RobotAccountPermissionArgs(
-                    accesses=[
-                        harbor.RobotAccountPermissionAccessArgs(
-                            action="push",
-                            resource="repository",
-                        ),
-                        harbor.RobotAccountPermissionAccessArgs(
-                            action="read",
-                            resource="helm-chart",
-                        ),
-                        harbor.RobotAccountPermissionAccessArgs(
-                            action="read",
-                            resource="helm-chart-version",
-                        ),
-                    ],
-                    kind="project",
-                    namespace=main.name,
-                ),
-                harbor.RobotAccountPermissionArgs(
-                    accesses=[harbor.RobotAccountPermissionAccessArgs(
-                        action="pull",
-                        resource="repository",
-                    )],
-                    kind="project",
-                    namespace="*",
-                ),
-            ])
-        ```
-
         The above example, creates a system level robot account with permissions to
         - permission to create labels on system level
         - pull repository across all projects
         - push repository to project "my-project-name"
         - read helm-chart and helm-chart-version in project "my-project-name"
+
         ### Project Level
 
         Other than system level robot accounts, project level robot accounts can interact on project level only.
         The [available permissions](https://github.com/goharbor/harbor/blob/-/src/common/rbac/const.go) are mostly the same as for system level robots.
 
-        ```python
-        import pulumi
-        import pulumiverse_harbor as harbor
-
-        main = harbor.Project("main")
-        project = harbor.RobotAccount("project",
-            description="project level robot account",
-            level="project",
-            permissions=[harbor.RobotAccountPermissionArgs(
-                accesses=[
-                    harbor.RobotAccountPermissionAccessArgs(
-                        action="pull",
-                        resource="repository",
-                    ),
-                    harbor.RobotAccountPermissionAccessArgs(
-                        action="push",
-                        resource="repository",
-                    ),
-                ],
-                kind="project",
-                namespace=main.name,
-            )])
-        ```
-
         The above example creates a project level robot account with permissions to
         - pull repository on project "main"
         - push repository on project "main"
 
         :param str resource_name: The name of the resource.
         :param RobotAccountArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
```

### Comparing `pulumiverse_harbor-3.9.2/pulumiverse_harbor/tasks.py` & `pulumiverse_harbor-3.9.3/pulumiverse_harbor/tasks.py`

 * *Files 4% similar despite different names*

```diff
@@ -56,40 +56,26 @@
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  vulnerability_scan_policy: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         ## Example Usage
 
-        ```python
-        import pulumi
-        import pulumiverse_harbor as harbor
-
-        main = harbor.Tasks("main", vulnerability_scan_policy="daily")
-        ```
-
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: TasksArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         ## Example Usage
 
-        ```python
-        import pulumi
-        import pulumiverse_harbor as harbor
-
-        main = harbor.Tasks("main", vulnerability_scan_policy="daily")
-        ```
-
         :param str resource_name: The name of the resource.
         :param TasksArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
         resource_args, opts = _utilities.get_resource_args_opts(TasksArgs, pulumi.ResourceOptions, *args, **kwargs)
```

### Comparing `pulumiverse_harbor-3.9.2/pulumiverse_harbor/user.py` & `pulumiverse_harbor-3.9.3/pulumiverse_harbor/user.py`

 * *Files 4% similar despite different names*

```diff
@@ -178,67 +178,33 @@
                  full_name: Optional[pulumi.Input[str]] = None,
                  password: Optional[pulumi.Input[str]] = None,
                  username: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         ## Example Usage
 
-        ```python
-        import pulumi
-        import pulumiverse_harbor as harbor
-
-        main = harbor.User("main",
-            email="john@smith.com",
-            full_name="John Smith",
-            password="Password12345!",
-            username="john")
-        ```
-
         ## Import
 
-        An internal user harbor user can be imported using the `user id` eg, `
-
-        ```sh
-         $ pulumi import harbor:index/user:User main /users/19
-        ```
-
-         `
+        An internal user harbor user can be imported using the `user id` eg, `<break><break>```sh<break> $ pulumi import harbor:index/user:User main /users/19 <break>```<break><break>`
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: UserArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         ## Example Usage
 
-        ```python
-        import pulumi
-        import pulumiverse_harbor as harbor
-
-        main = harbor.User("main",
-            email="john@smith.com",
-            full_name="John Smith",
-            password="Password12345!",
-            username="john")
-        ```
-
         ## Import
 
-        An internal user harbor user can be imported using the `user id` eg, `
-
-        ```sh
-         $ pulumi import harbor:index/user:User main /users/19
-        ```
-
-         `
+        An internal user harbor user can be imported using the `user id` eg, `<break><break>```sh<break> $ pulumi import harbor:index/user:User main /users/19 <break>```<break><break>`
 
         :param str resource_name: The name of the resource.
         :param UserArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
```

### Comparing `pulumiverse_harbor-3.9.2/pulumiverse_harbor.egg-info/PKG-INFO` & `pulumiverse_harbor-3.9.3/pulumiverse_harbor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumiverse-harbor
-Version: 3.9.2
+Version: 3.9.3
 Summary: A Pulumi package for creating and managing Harbor resources.
 Home-page: https://www.pulumi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumiverse/pulumi-harbor
 Keywords: pulumi harbor category/utility
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumiverse_harbor-3.9.2/pulumiverse_harbor.egg-info/SOURCES.txt` & `pulumiverse_harbor-3.9.3/pulumiverse_harbor.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 pulumiverse_harbor/outputs.py
 pulumiverse_harbor/project.py
 pulumiverse_harbor/project_member_group.py
 pulumiverse_harbor/project_member_user.py
 pulumiverse_harbor/project_webhook.py
 pulumiverse_harbor/provider.py
 pulumiverse_harbor/pulumi-plugin.json
+pulumiverse_harbor/purge_audit_log.py
 pulumiverse_harbor/py.typed
 pulumiverse_harbor/registry.py
 pulumiverse_harbor/replication.py
 pulumiverse_harbor/retention_policy.py
 pulumiverse_harbor/robot_account.py
 pulumiverse_harbor/tasks.py
 pulumiverse_harbor/user.py
```

### Comparing `pulumiverse_harbor-3.9.2/setup.py` & `pulumiverse_harbor-3.9.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "3.9.2"
-PLUGIN_VERSION = "3.9.2"
+VERSION = "3.9.3"
+PLUGIN_VERSION = "3.9.3"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'harbor', PLUGIN_VERSION, '--server', 'github://api.github.com/pulumiverse/pulumi-harbor'])
         except OSError as error:
```

