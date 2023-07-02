# Comparing `tmp/threemystic_cloud_client-0.1.2.tar.gz` & `tmp/threemystic_cloud_client-0.1.3.tar.gz`

## Comparing `threemystic_cloud_client-0.1.2.tar` & `threemystic_cloud_client-0.1.3.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.2/threemystic_cloud_client/__main__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.2/threemystic_cloud_client/__version__.py
--rw-r--r--   0        0        0     3168 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.2/threemystic_cloud_client/cloud_client.py
--rw-r--r--   0        0        0     4011 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.2/threemystic_cloud_client/cli/__init__.py
--rw-r--r--   0        0        0     2519 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.2/threemystic_cloud_client/cli/actions/base_class/base.py
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.2/threemystic_cloud_client/cli/actions/config/__init__.py
--rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.2/threemystic_cloud_client/cli/actions/test/__init__.py
--rw-r--r--   0        0        0     4074 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.2/threemystic_cloud_client/cli/actions/token/__init__.py
--rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.2/threemystic_cloud_client/cloud_providers/aws/__init__.py
--rw-r--r--   0        0        0     3591 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.2/threemystic_cloud_client/cloud_providers/aws/base_class/base.py
--rw-r--r--   0        0        0     2045 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.2/threemystic_cloud_client/cloud_providers/aws/client/auto_client.py
--rw-r--r--   0        0        0    12041 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.2/threemystic_cloud_client/cloud_providers/aws/client/sso.py
--rw-r--r--   0        0        0    21250 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.2/threemystic_cloud_client/cloud_providers/aws/client/base_class/base.py
--rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.2/threemystic_cloud_client/cloud_providers/aws/config/step_1.py
--rw-r--r--   0        0        0    15698 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.2/threemystic_cloud_client/cloud_providers/aws/config/step_2.py
--rw-r--r--   0        0        0     3451 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.2/threemystic_cloud_client/cloud_providers/aws/config/base_class/base.py
--rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.2/threemystic_cloud_client/cloud_providers/aws/test/step_1.py
--rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.2/threemystic_cloud_client/cloud_providers/aws/test/step_2.py
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.2/threemystic_cloud_client/cloud_providers/aws/test/base_class/base.py
--rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.2/threemystic_cloud_client/cloud_providers/azure/__init__.py
--rw-r--r--   0        0        0    13846 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.2/threemystic_cloud_client/cloud_providers/azure/base_class/base.py
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.2/threemystic_cloud_client/cloud_providers/azure/client/auto_client.py
--rw-r--r--   0        0        0     1478 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.2/threemystic_cloud_client/cloud_providers/azure/client/cli.py
--rw-r--r--   0        0        0    13524 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.2/threemystic_cloud_client/cloud_providers/azure/client/base_class/base.py
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.2/threemystic_cloud_client/cloud_providers/azure/config/step_1.py
--rw-r--r--   0        0        0     2739 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.2/threemystic_cloud_client/cloud_providers/azure/config/base_class/base.py
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.2/threemystic_cloud_client/cloud_providers/azure/test/step_1.py
--rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.2/threemystic_cloud_client/cloud_providers/azure/test/base_class/base.py
--rw-r--r--   0        0        0     4923 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.2/threemystic_cloud_client/cloud_providers/base_class/base.py
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.2/threemystic_cloud_client/domain/aws/client_sso.py
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.2/threemystic_cloud_client/domain/aws/controller.py
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.2/threemystic_cloud_client/domain/azure/client.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.2/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.2/LICENSE
--rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.2/README.md
--rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.2/hatch.toml
--rw-r--r--   0        0        0     3317 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2595 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.3/threemystic_cloud_client/__main__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.3/threemystic_cloud_client/__version__.py
+-rw-r--r--   0        0        0     3168 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.3/threemystic_cloud_client/cloud_client.py
+-rw-r--r--   0        0        0     4011 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.3/threemystic_cloud_client/cli/__init__.py
+-rw-r--r--   0        0        0     2519 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.3/threemystic_cloud_client/cli/actions/base_class/base.py
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.3/threemystic_cloud_client/cli/actions/config/__init__.py
+-rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.3/threemystic_cloud_client/cli/actions/test/__init__.py
+-rw-r--r--   0        0        0     4074 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.3/threemystic_cloud_client/cli/actions/token/__init__.py
+-rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.3/threemystic_cloud_client/cloud_providers/aws/__init__.py
+-rw-r--r--   0        0        0     3591 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.3/threemystic_cloud_client/cloud_providers/aws/base_class/base.py
+-rw-r--r--   0        0        0     2045 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.3/threemystic_cloud_client/cloud_providers/aws/client/auto_client.py
+-rw-r--r--   0        0        0    12041 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.3/threemystic_cloud_client/cloud_providers/aws/client/sso.py
+-rw-r--r--   0        0        0    21250 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.3/threemystic_cloud_client/cloud_providers/aws/client/base_class/base.py
+-rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.3/threemystic_cloud_client/cloud_providers/aws/config/step_1.py
+-rw-r--r--   0        0        0    15698 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.3/threemystic_cloud_client/cloud_providers/aws/config/step_2.py
+-rw-r--r--   0        0        0     3451 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.3/threemystic_cloud_client/cloud_providers/aws/config/base_class/base.py
+-rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.3/threemystic_cloud_client/cloud_providers/aws/test/step_1.py
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.3/threemystic_cloud_client/cloud_providers/aws/test/step_2.py
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.3/threemystic_cloud_client/cloud_providers/aws/test/base_class/base.py
+-rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.3/threemystic_cloud_client/cloud_providers/azure/__init__.py
+-rw-r--r--   0        0        0    13846 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.3/threemystic_cloud_client/cloud_providers/azure/base_class/base.py
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.3/threemystic_cloud_client/cloud_providers/azure/client/auto_client.py
+-rw-r--r--   0        0        0     1478 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.3/threemystic_cloud_client/cloud_providers/azure/client/cli.py
+-rw-r--r--   0        0        0    13524 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.3/threemystic_cloud_client/cloud_providers/azure/client/base_class/base.py
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.3/threemystic_cloud_client/cloud_providers/azure/config/step_1.py
+-rw-r--r--   0        0        0     2739 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.3/threemystic_cloud_client/cloud_providers/azure/config/base_class/base.py
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.3/threemystic_cloud_client/cloud_providers/azure/test/step_1.py
+-rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.3/threemystic_cloud_client/cloud_providers/azure/test/base_class/base.py
+-rw-r--r--   0        0        0     4923 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.3/threemystic_cloud_client/cloud_providers/base_class/base.py
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.3/threemystic_cloud_client/domain/aws/client_sso.py
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.3/threemystic_cloud_client/domain/aws/controller.py
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.3/threemystic_cloud_client/domain/azure/client.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.3/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.3/LICENSE
+-rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.3/README.md
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.3/hatch.toml
+-rw-r--r--   0        0        0     3317 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2595 2020-02-02 00:00:00.000000 threemystic_cloud_client-0.1.3/PKG-INFO
```

### Comparing `threemystic_cloud_client-0.1.2/threemystic_cloud_client/cloud_client.py` & `threemystic_cloud_client-0.1.3/threemystic_cloud_client/cloud_client.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.2/threemystic_cloud_client/cli/__init__.py` & `threemystic_cloud_client-0.1.3/threemystic_cloud_client/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.2/threemystic_cloud_client/cli/actions/base_class/base.py` & `threemystic_cloud_client-0.1.3/threemystic_cloud_client/cli/actions/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.2/threemystic_cloud_client/cli/actions/config/__init__.py` & `threemystic_cloud_client-0.1.3/threemystic_cloud_client/cli/actions/config/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.2/threemystic_cloud_client/cli/actions/test/__init__.py` & `threemystic_cloud_client-0.1.3/threemystic_cloud_client/cli/actions/test/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.2/threemystic_cloud_client/cli/actions/token/__init__.py` & `threemystic_cloud_client-0.1.3/threemystic_cloud_client/cli/actions/token/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.2/threemystic_cloud_client/cloud_providers/aws/__init__.py` & `threemystic_cloud_client-0.1.3/threemystic_cloud_client/cloud_providers/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.2/threemystic_cloud_client/cloud_providers/aws/base_class/base.py` & `threemystic_cloud_client-0.1.3/threemystic_cloud_client/cloud_providers/aws/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.2/threemystic_cloud_client/cloud_providers/aws/client/auto_client.py` & `threemystic_cloud_client-0.1.3/threemystic_cloud_client/cloud_providers/aws/client/auto_client.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.2/threemystic_cloud_client/cloud_providers/aws/client/sso.py` & `threemystic_cloud_client-0.1.3/threemystic_cloud_client/cloud_providers/aws/client/sso.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.2/threemystic_cloud_client/cloud_providers/aws/client/base_class/base.py` & `threemystic_cloud_client-0.1.3/threemystic_cloud_client/cloud_providers/aws/client/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.2/threemystic_cloud_client/cloud_providers/aws/config/step_1.py` & `threemystic_cloud_client-0.1.3/threemystic_cloud_client/cloud_providers/aws/config/step_1.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.2/threemystic_cloud_client/cloud_providers/aws/config/step_2.py` & `threemystic_cloud_client-0.1.3/threemystic_cloud_client/cloud_providers/aws/config/step_2.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.2/threemystic_cloud_client/cloud_providers/aws/config/base_class/base.py` & `threemystic_cloud_client-0.1.3/threemystic_cloud_client/cloud_providers/aws/config/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.2/threemystic_cloud_client/cloud_providers/aws/test/step_1.py` & `threemystic_cloud_client-0.1.3/threemystic_cloud_client/cloud_providers/aws/test/step_1.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.2/threemystic_cloud_client/cloud_providers/aws/test/step_2.py` & `threemystic_cloud_client-0.1.3/threemystic_cloud_client/cloud_providers/aws/test/step_2.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.2/threemystic_cloud_client/cloud_providers/aws/test/base_class/base.py` & `threemystic_cloud_client-0.1.3/threemystic_cloud_client/cloud_providers/aws/test/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.2/threemystic_cloud_client/cloud_providers/azure/__init__.py` & `threemystic_cloud_client-0.1.3/threemystic_cloud_client/cloud_providers/azure/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.2/threemystic_cloud_client/cloud_providers/azure/base_class/base.py` & `threemystic_cloud_client-0.1.3/threemystic_cloud_client/cloud_providers/azure/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.2/threemystic_cloud_client/cloud_providers/azure/client/cli.py` & `threemystic_cloud_client-0.1.3/threemystic_cloud_client/cloud_providers/azure/client/cli.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.2/threemystic_cloud_client/cloud_providers/azure/client/base_class/base.py` & `threemystic_cloud_client-0.1.3/threemystic_cloud_client/cloud_providers/azure/client/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.2/threemystic_cloud_client/cloud_providers/azure/config/step_1.py` & `threemystic_cloud_client-0.1.3/threemystic_cloud_client/cloud_providers/azure/config/step_1.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.2/threemystic_cloud_client/cloud_providers/azure/config/base_class/base.py` & `threemystic_cloud_client-0.1.3/threemystic_cloud_client/cloud_providers/azure/config/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.2/threemystic_cloud_client/cloud_providers/azure/test/step_1.py` & `threemystic_cloud_client-0.1.3/threemystic_cloud_client/cloud_providers/azure/test/step_1.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.2/threemystic_cloud_client/cloud_providers/azure/test/base_class/base.py` & `threemystic_cloud_client-0.1.3/threemystic_cloud_client/cloud_providers/azure/test/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.2/threemystic_cloud_client/cloud_providers/base_class/base.py` & `threemystic_cloud_client-0.1.3/threemystic_cloud_client/cloud_providers/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.2/.gitignore` & `threemystic_cloud_client-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.2/LICENSE` & `threemystic_cloud_client-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.2/README.md` & `threemystic_cloud_client-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.2/hatch.toml` & `threemystic_cloud_client-0.1.3/hatch.toml`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_client-0.1.2/pyproject.toml` & `threemystic_cloud_client-0.1.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
   "colorama; platform_system == 'Windows'",
-  "threemystic-common >= 0.1.1",
+  "threemystic-common >= 0.1.2",
   "polling2 >= 0.5.0",
   "typing-extensions >= 4.4.0",
   "boto3 >= 1.26.151",
   "botocore >= 1.29.151",
   "azure-common >= 1.1.28",
   "azure-cli >= 2.49.0",
   "azure-identity >= 1.13.0",
```

### Comparing `threemystic_cloud_client-0.1.2/PKG-INFO` & `threemystic_cloud_client-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: threemystic-cloud-client
-Version: 0.1.2
+Version: 0.1.3
 Summary: A tool to help facilitate the communication with various cloud providers
 Project-URL: Homepage, https://github.com/3MysticApes/3mystic_cloud_client
 Project-URL: Bug Tracker, https://github.com/3MysticApes/3mystic_cloud_client/issues
 Author: Ron Truex
 License-Expression: MIT
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
@@ -24,15 +24,15 @@
 Requires-Dist: azure-mgmt-resourcegraph>=8.0.0
 Requires-Dist: azure-mgmt-sql>=3.0.1
 Requires-Dist: azure-mgmt-subscription>=3.1.1
 Requires-Dist: boto3>=1.26.151
 Requires-Dist: botocore>=1.29.151
 Requires-Dist: colorama; platform_system == 'Windows'
 Requires-Dist: polling2>=0.5.0
-Requires-Dist: threemystic-common>=0.1.1
+Requires-Dist: threemystic-common>=0.1.2
 Requires-Dist: typing-extensions>=4.4.0
 Description-Content-Type: text/markdown
 
 # 3mystic_cloud_client
 A tool to help uniform the connection to the cloud providers.
 Currently supports AWS/Azure
```

