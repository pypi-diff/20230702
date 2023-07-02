# Comparing `tmp/threemystic_common-0.1.1.tar.gz` & `tmp/threemystic_common-0.1.2.tar.gz`

## Comparing `threemystic_common-0.1.1.tar` & `threemystic_common-0.1.2.tar`

### file list

```diff
@@ -1,56 +1,56 @@
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 threemystic_common-0.1.1/threemystic_common/__main__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 threemystic_common-0.1.1/threemystic_common/__version__.py
--rw-r--r--   0        0        0     7303 2020-02-02 00:00:00.000000 threemystic_common-0.1.1/threemystic_common/common.py
--rw-r--r--   0        0        0     3171 2020-02-02 00:00:00.000000 threemystic_common-0.1.1/threemystic_common/base_class/base.py
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 threemystic_common-0.1.1/threemystic_common/base_class/base_common.py
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 threemystic_common-0.1.1/threemystic_common/base_class/base_general.py
--rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 threemystic_common-0.1.1/threemystic_common/base_class/base_provider.py
--rw-r--r--   0        0        0     2516 2020-02-02 00:00:00.000000 threemystic_common-0.1.1/threemystic_common/base_class/base_script_options.py
--rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 threemystic_common-0.1.1/threemystic_common/base_class/generate_data/generate_data_handlers.py
--rw-r--r--   0        0        0     6720 2020-02-02 00:00:00.000000 threemystic_common-0.1.1/threemystic_common/base_class/generate_data/handlers/base.py
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 threemystic_common-0.1.1/threemystic_common/cli/__init__.py
--rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 threemystic_common-0.1.1/threemystic_common/domain/app_monitoring/common.py
--rw-r--r--   0        0        0     3197 2020-02-02 00:00:00.000000 threemystic_common-0.1.1/threemystic_common/domain/app_monitoring/performance.py
--rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 threemystic_common-0.1.1/threemystic_common/domain/cmdb/aws.py
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 threemystic_common-0.1.1/threemystic_common/domain/cmdb/azure.py
--rw-r--r--   0        0        0     2122 2020-02-02 00:00:00.000000 threemystic_common-0.1.1/threemystic_common/domain/cmdb/common.py
--rw-r--r--   0        0        0    15045 2020-02-02 00:00:00.000000 threemystic_common-0.1.1/threemystic_common/domain/cmdb/base_class/base.py
--rw-r--r--   0        0        0     1203 2020-02-02 00:00:00.000000 threemystic_common-0.1.1/threemystic_common/domain/encryption/common.py
--rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 threemystic_common-0.1.1/threemystic_common/domain/encryption/hash.py
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 threemystic_common-0.1.1/threemystic_common/domain/exception/argument.py
--rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 threemystic_common-0.1.1/threemystic_common/domain/exception/common.py
--rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 threemystic_common-0.1.1/threemystic_common/domain/exception/function.py
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 threemystic_common-0.1.1/threemystic_common/domain/exception/generic.py
--rw-r--r--   0        0        0     4674 2020-02-02 00:00:00.000000 threemystic_common-0.1.1/threemystic_common/domain/exception/base_class/base.py
--rw-r--r--   0        0        0     3597 2020-02-02 00:00:00.000000 threemystic_common-0.1.1/threemystic_common/domain/generate_data/generate.py
--rw-r--r--   0        0        0     1868 2020-02-02 00:00:00.000000 threemystic_common-0.1.1/threemystic_common/domain/graph/common.py
--rw-r--r--   0        0        0     9330 2020-02-02 00:00:00.000000 threemystic_common-0.1.1/threemystic_common/domain/graph/msgraph.py
--rw-r--r--   0        0        0    11209 2020-02-02 00:00:00.000000 threemystic_common-0.1.1/threemystic_common/domain/graph/base_class/base.py
--rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 threemystic_common-0.1.1/threemystic_common/domain/graph/config/msgraph.py
--rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 threemystic_common-0.1.1/threemystic_common/domain/hashicorp/common.py
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 threemystic_common-0.1.1/threemystic_common/domain/hashicorp/vault.py
--rw-r--r--   0        0        0     2599 2020-02-02 00:00:00.000000 threemystic_common-0.1.1/threemystic_common/domain/helpers/app.py
--rw-r--r--   0        0        0     4725 2020-02-02 00:00:00.000000 threemystic_common-0.1.1/threemystic_common/domain/helpers/config.py
--rw-r--r--   0        0        0     2462 2020-02-02 00:00:00.000000 threemystic_common-0.1.1/threemystic_common/domain/helpers/json.py
--rw-r--r--   0        0        0     1869 2020-02-02 00:00:00.000000 threemystic_common-0.1.1/threemystic_common/domain/helpers/parallel_processing.py
--rw-r--r--   0        0        0     3027 2020-02-02 00:00:00.000000 threemystic_common-0.1.1/threemystic_common/domain/helpers/path.py
--rw-r--r--   0        0        0     2058 2020-02-02 00:00:00.000000 threemystic_common-0.1.1/threemystic_common/domain/helpers/yaml.py
--rw-r--r--   0        0        0     2245 2020-02-02 00:00:00.000000 threemystic_common-0.1.1/threemystic_common/domain/helpers/type/bool.py
--rw-r--r--   0        0        0     4091 2020-02-02 00:00:00.000000 threemystic_common-0.1.1/threemystic_common/domain/helpers/type/common.py
--rw-r--r--   0        0        0    10148 2020-02-02 00:00:00.000000 threemystic_common-0.1.1/threemystic_common/domain/helpers/type/datetime.py
--rw-r--r--   0        0        0     2359 2020-02-02 00:00:00.000000 threemystic_common-0.1.1/threemystic_common/domain/helpers/type/dictionary.py
--rw-r--r--   0        0        0     2360 2020-02-02 00:00:00.000000 threemystic_common-0.1.1/threemystic_common/domain/helpers/type/general.py
--rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 threemystic_common-0.1.1/threemystic_common/domain/helpers/type/int.py
--rw-r--r--   0        0        0     3225 2020-02-02 00:00:00.000000 threemystic_common-0.1.1/threemystic_common/domain/helpers/type/list.py
--rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 threemystic_common-0.1.1/threemystic_common/domain/helpers/type/logging.py
--rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 threemystic_common-0.1.1/threemystic_common/domain/helpers/type/openpyxl.py
--rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 threemystic_common-0.1.1/threemystic_common/domain/helpers/type/regex.py
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 threemystic_common-0.1.1/threemystic_common/domain/helpers/type/requests.py
--rw-r--r--   0        0        0     4827 2020-02-02 00:00:00.000000 threemystic_common-0.1.1/threemystic_common/domain/helpers/type/string.py
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 threemystic_common-0.1.1/threemystic_common/exceptions/generate_data/quit.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 threemystic_common-0.1.1/.gitignore
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 threemystic_common-0.1.1/LICENSE
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 threemystic_common-0.1.1/README.md
--rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 threemystic_common-0.1.1/hatch.toml
--rw-r--r--   0        0        0     3033 2020-02-02 00:00:00.000000 threemystic_common-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2312 2020-02-02 00:00:00.000000 threemystic_common-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 threemystic_common-0.1.2/threemystic_common/__main__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 threemystic_common-0.1.2/threemystic_common/__version__.py
+-rw-r--r--   0        0        0     7303 2020-02-02 00:00:00.000000 threemystic_common-0.1.2/threemystic_common/common.py
+-rw-r--r--   0        0        0     3171 2020-02-02 00:00:00.000000 threemystic_common-0.1.2/threemystic_common/base_class/base.py
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 threemystic_common-0.1.2/threemystic_common/base_class/base_common.py
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 threemystic_common-0.1.2/threemystic_common/base_class/base_general.py
+-rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 threemystic_common-0.1.2/threemystic_common/base_class/base_provider.py
+-rw-r--r--   0        0        0     2516 2020-02-02 00:00:00.000000 threemystic_common-0.1.2/threemystic_common/base_class/base_script_options.py
+-rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 threemystic_common-0.1.2/threemystic_common/base_class/generate_data/generate_data_handlers.py
+-rw-r--r--   0        0        0     6720 2020-02-02 00:00:00.000000 threemystic_common-0.1.2/threemystic_common/base_class/generate_data/handlers/base.py
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 threemystic_common-0.1.2/threemystic_common/cli/__init__.py
+-rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 threemystic_common-0.1.2/threemystic_common/domain/app_monitoring/common.py
+-rw-r--r--   0        0        0     3197 2020-02-02 00:00:00.000000 threemystic_common-0.1.2/threemystic_common/domain/app_monitoring/performance.py
+-rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 threemystic_common-0.1.2/threemystic_common/domain/cmdb/aws.py
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 threemystic_common-0.1.2/threemystic_common/domain/cmdb/azure.py
+-rw-r--r--   0        0        0     2122 2020-02-02 00:00:00.000000 threemystic_common-0.1.2/threemystic_common/domain/cmdb/common.py
+-rw-r--r--   0        0        0    15045 2020-02-02 00:00:00.000000 threemystic_common-0.1.2/threemystic_common/domain/cmdb/base_class/base.py
+-rw-r--r--   0        0        0     1203 2020-02-02 00:00:00.000000 threemystic_common-0.1.2/threemystic_common/domain/encryption/common.py
+-rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 threemystic_common-0.1.2/threemystic_common/domain/encryption/hash.py
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 threemystic_common-0.1.2/threemystic_common/domain/exception/argument.py
+-rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 threemystic_common-0.1.2/threemystic_common/domain/exception/common.py
+-rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 threemystic_common-0.1.2/threemystic_common/domain/exception/function.py
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 threemystic_common-0.1.2/threemystic_common/domain/exception/generic.py
+-rw-r--r--   0        0        0     4674 2020-02-02 00:00:00.000000 threemystic_common-0.1.2/threemystic_common/domain/exception/base_class/base.py
+-rw-r--r--   0        0        0     3597 2020-02-02 00:00:00.000000 threemystic_common-0.1.2/threemystic_common/domain/generate_data/generate.py
+-rw-r--r--   0        0        0     1868 2020-02-02 00:00:00.000000 threemystic_common-0.1.2/threemystic_common/domain/graph/common.py
+-rw-r--r--   0        0        0     9330 2020-02-02 00:00:00.000000 threemystic_common-0.1.2/threemystic_common/domain/graph/msgraph.py
+-rw-r--r--   0        0        0    11209 2020-02-02 00:00:00.000000 threemystic_common-0.1.2/threemystic_common/domain/graph/base_class/base.py
+-rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 threemystic_common-0.1.2/threemystic_common/domain/graph/config/msgraph.py
+-rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 threemystic_common-0.1.2/threemystic_common/domain/hashicorp/common.py
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 threemystic_common-0.1.2/threemystic_common/domain/hashicorp/vault.py
+-rw-r--r--   0        0        0     2599 2020-02-02 00:00:00.000000 threemystic_common-0.1.2/threemystic_common/domain/helpers/app.py
+-rw-r--r--   0        0        0     4725 2020-02-02 00:00:00.000000 threemystic_common-0.1.2/threemystic_common/domain/helpers/config.py
+-rw-r--r--   0        0        0     2462 2020-02-02 00:00:00.000000 threemystic_common-0.1.2/threemystic_common/domain/helpers/json.py
+-rw-r--r--   0        0        0     1869 2020-02-02 00:00:00.000000 threemystic_common-0.1.2/threemystic_common/domain/helpers/parallel_processing.py
+-rw-r--r--   0        0        0     3027 2020-02-02 00:00:00.000000 threemystic_common-0.1.2/threemystic_common/domain/helpers/path.py
+-rw-r--r--   0        0        0     2058 2020-02-02 00:00:00.000000 threemystic_common-0.1.2/threemystic_common/domain/helpers/yaml.py
+-rw-r--r--   0        0        0     2245 2020-02-02 00:00:00.000000 threemystic_common-0.1.2/threemystic_common/domain/helpers/type/bool.py
+-rw-r--r--   0        0        0     4091 2020-02-02 00:00:00.000000 threemystic_common-0.1.2/threemystic_common/domain/helpers/type/common.py
+-rw-r--r--   0        0        0    10148 2020-02-02 00:00:00.000000 threemystic_common-0.1.2/threemystic_common/domain/helpers/type/datetime.py
+-rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 threemystic_common-0.1.2/threemystic_common/domain/helpers/type/dictionary.py
+-rw-r--r--   0        0        0     2360 2020-02-02 00:00:00.000000 threemystic_common-0.1.2/threemystic_common/domain/helpers/type/general.py
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 threemystic_common-0.1.2/threemystic_common/domain/helpers/type/int.py
+-rw-r--r--   0        0        0     3681 2020-02-02 00:00:00.000000 threemystic_common-0.1.2/threemystic_common/domain/helpers/type/list.py
+-rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 threemystic_common-0.1.2/threemystic_common/domain/helpers/type/logging.py
+-rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 threemystic_common-0.1.2/threemystic_common/domain/helpers/type/openpyxl.py
+-rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 threemystic_common-0.1.2/threemystic_common/domain/helpers/type/regex.py
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 threemystic_common-0.1.2/threemystic_common/domain/helpers/type/requests.py
+-rw-r--r--   0        0        0     4832 2020-02-02 00:00:00.000000 threemystic_common-0.1.2/threemystic_common/domain/helpers/type/string.py
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 threemystic_common-0.1.2/threemystic_common/exceptions/generate_data/quit.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 threemystic_common-0.1.2/.gitignore
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 threemystic_common-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 threemystic_common-0.1.2/README.md
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 threemystic_common-0.1.2/hatch.toml
+-rw-r--r--   0        0        0     3033 2020-02-02 00:00:00.000000 threemystic_common-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2312 2020-02-02 00:00:00.000000 threemystic_common-0.1.2/PKG-INFO
```

### Comparing `threemystic_common-0.1.1/threemystic_common/common.py` & `threemystic_common-0.1.2/threemystic_common/common.py`

 * *Files identical despite different names*

### Comparing `threemystic_common-0.1.1/threemystic_common/base_class/base.py` & `threemystic_common-0.1.2/threemystic_common/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_common-0.1.1/threemystic_common/base_class/base_provider.py` & `threemystic_common-0.1.2/threemystic_common/base_class/base_provider.py`

 * *Files identical despite different names*

### Comparing `threemystic_common-0.1.1/threemystic_common/base_class/base_script_options.py` & `threemystic_common-0.1.2/threemystic_common/base_class/base_script_options.py`

 * *Files identical despite different names*

### Comparing `threemystic_common-0.1.1/threemystic_common/base_class/generate_data/handlers/base.py` & `threemystic_common-0.1.2/threemystic_common/base_class/generate_data/handlers/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_common-0.1.1/threemystic_common/domain/app_monitoring/common.py` & `threemystic_common-0.1.2/threemystic_common/domain/app_monitoring/common.py`

 * *Files identical despite different names*

### Comparing `threemystic_common-0.1.1/threemystic_common/domain/app_monitoring/performance.py` & `threemystic_common-0.1.2/threemystic_common/domain/app_monitoring/performance.py`

 * *Files identical despite different names*

### Comparing `threemystic_common-0.1.1/threemystic_common/domain/cmdb/aws.py` & `threemystic_common-0.1.2/threemystic_common/domain/cmdb/aws.py`

 * *Files identical despite different names*

### Comparing `threemystic_common-0.1.1/threemystic_common/domain/cmdb/common.py` & `threemystic_common-0.1.2/threemystic_common/domain/cmdb/common.py`

 * *Files identical despite different names*

### Comparing `threemystic_common-0.1.1/threemystic_common/domain/cmdb/base_class/base.py` & `threemystic_common-0.1.2/threemystic_common/domain/cmdb/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_common-0.1.1/threemystic_common/domain/encryption/common.py` & `threemystic_common-0.1.2/threemystic_common/domain/encryption/common.py`

 * *Files identical despite different names*

### Comparing `threemystic_common-0.1.1/threemystic_common/domain/encryption/hash.py` & `threemystic_common-0.1.2/threemystic_common/domain/encryption/hash.py`

 * *Files identical despite different names*

### Comparing `threemystic_common-0.1.1/threemystic_common/domain/exception/common.py` & `threemystic_common-0.1.2/threemystic_common/domain/exception/common.py`

 * *Files identical despite different names*

### Comparing `threemystic_common-0.1.1/threemystic_common/domain/exception/base_class/base.py` & `threemystic_common-0.1.2/threemystic_common/domain/exception/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_common-0.1.1/threemystic_common/domain/generate_data/generate.py` & `threemystic_common-0.1.2/threemystic_common/domain/generate_data/generate.py`

 * *Files identical despite different names*

### Comparing `threemystic_common-0.1.1/threemystic_common/domain/graph/common.py` & `threemystic_common-0.1.2/threemystic_common/domain/graph/common.py`

 * *Files identical despite different names*

### Comparing `threemystic_common-0.1.1/threemystic_common/domain/graph/msgraph.py` & `threemystic_common-0.1.2/threemystic_common/domain/graph/msgraph.py`

 * *Files identical despite different names*

### Comparing `threemystic_common-0.1.1/threemystic_common/domain/graph/base_class/base.py` & `threemystic_common-0.1.2/threemystic_common/domain/graph/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_common-0.1.1/threemystic_common/domain/graph/config/msgraph.py` & `threemystic_common-0.1.2/threemystic_common/domain/graph/config/msgraph.py`

 * *Files identical despite different names*

### Comparing `threemystic_common-0.1.1/threemystic_common/domain/hashicorp/common.py` & `threemystic_common-0.1.2/threemystic_common/domain/hashicorp/common.py`

 * *Files identical despite different names*

### Comparing `threemystic_common-0.1.1/threemystic_common/domain/helpers/app.py` & `threemystic_common-0.1.2/threemystic_common/domain/helpers/app.py`

 * *Files identical despite different names*

### Comparing `threemystic_common-0.1.1/threemystic_common/domain/helpers/config.py` & `threemystic_common-0.1.2/threemystic_common/domain/helpers/config.py`

 * *Files identical despite different names*

### Comparing `threemystic_common-0.1.1/threemystic_common/domain/helpers/json.py` & `threemystic_common-0.1.2/threemystic_common/domain/helpers/json.py`

 * *Files identical despite different names*

### Comparing `threemystic_common-0.1.1/threemystic_common/domain/helpers/parallel_processing.py` & `threemystic_common-0.1.2/threemystic_common/domain/helpers/parallel_processing.py`

 * *Files identical despite different names*

### Comparing `threemystic_common-0.1.1/threemystic_common/domain/helpers/path.py` & `threemystic_common-0.1.2/threemystic_common/domain/helpers/path.py`

 * *Files identical despite different names*

### Comparing `threemystic_common-0.1.1/threemystic_common/domain/helpers/yaml.py` & `threemystic_common-0.1.2/threemystic_common/domain/helpers/yaml.py`

 * *Files identical despite different names*

### Comparing `threemystic_common-0.1.1/threemystic_common/domain/helpers/type/bool.py` & `threemystic_common-0.1.2/threemystic_common/domain/helpers/type/bool.py`

 * *Files identical despite different names*

### Comparing `threemystic_common-0.1.1/threemystic_common/domain/helpers/type/common.py` & `threemystic_common-0.1.2/threemystic_common/domain/helpers/type/common.py`

 * *Files identical despite different names*

### Comparing `threemystic_common-0.1.1/threemystic_common/domain/helpers/type/datetime.py` & `threemystic_common-0.1.2/threemystic_common/domain/helpers/type/datetime.py`

 * *Files identical despite different names*

### Comparing `threemystic_common-0.1.1/threemystic_common/domain/helpers/type/dictionary.py` & `threemystic_common-0.1.2/threemystic_common/domain/helpers/type/dictionary.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,53 +15,70 @@
       if item is None:
         continue
       
       return idx + 1
     
     return -1
 
-  def merge_dictionary(self, dict1, dict2 = None, replace_on_merge = False, custom_handlers = {}, unique_list = False, update_first_dictionary = True):
+  def _merge_dictionary_update_new_dictionary(self, dict1, *args, **kwargs):
+    tmp_dict = {}
+    tmp_dict.update(dict1)
+    return tmp_dict
+  
+  def merge_dictionary(self, dict1, dict2 = None, replace_on_merge = False, unique_list = False, update_first_dictionary = True, *args, **kwargs):
     if dict1 is None and dict2 is None:
       return None
     if dict1 is None and dict2 is not None:
       return dict2
 
     if self._main_reference.helper_type().general().is_type(dict1, list):
       main_dict_index = self._merge_dictionary_find_main_dictionary_index(dicts= dict1)
       if main_dict_index < 0:
         return None
       
-      return_dict = dict1[main_dict_index] if update_first_dictionary else {}.update(dict1[main_dict_index])      
-      if (main_dict_index + 1) == len(dict1):
+      return_dict = dict1[main_dict_index] if update_first_dictionary else self._merge_dictionary_update_new_dictionary(dict1[main_dict_index])    
+      
+      main_dict_index += 1
+      if (main_dict_index) == len(dict1):
         return return_dict
 
       for dict_item in dict1[main_dict_index:]:
-        self.merge_dictionary(dict1= return_dict, dict2=dict_item,)
+        return_dict = self.merge_dictionary(dict1= return_dict, dict2=dict_item, unique_list= unique_list, update_first_dictionary = True)
+
       return return_dict
 
     if dict2 is None:
       return dict1
     
-    update_dictionary = dict1 if update_first_dictionary else {}.update(dict1)
-    if replace_on_merge:
+    update_dictionary = dict1 if update_first_dictionary else self._merge_dictionary_update_new_dictionary(dict1)
+ 
+    if replace_on_merge or len(update_dictionary) < 1:
       update_dictionary.update(dict2)
       return update_dictionary
 
     dict2_copy = self._main_reference.helper_type().general().copy_object(object_copy= dict2)
 
     for key, item in update_dictionary.items():
       if self._main_reference.helper_type().general().is_type(item, dict):
         if key in dict2_copy:
-          self.merge_dictionary(item, dict2_copy[key])
+          self.merge_dictionary(item, dict2_copy[key], unique_list= unique_list, update_first_dictionary = True)
           dict2_copy.pop(key, None)
         continue
       if self._main_reference.helper_type().general().is_type(item, list):
         if key in dict2_copy:
           item += dict2_copy[key]
-          if unique_list:
+
+          if unique_list is not None and unique_list is not False:
+            if self._main_reference.helper_type().general().is_type(unique_list, str):
+              if key != unique_list:
+                continue
+            if self._main_reference.helper_type().general().is_type(unique_list, list):
+              if key not in unique_list:
+                continue
+
             item = self._main_reference.helper_type().list().unique_list(item)
           dict2_copy.pop(key, None)
           
         continue
       
     update_dictionary.update(dict2_copy)
```

### Comparing `threemystic_common-0.1.1/threemystic_common/domain/helpers/type/general.py` & `threemystic_common-0.1.2/threemystic_common/domain/helpers/type/general.py`

 * *Files identical despite different names*

### Comparing `threemystic_common-0.1.1/threemystic_common/domain/helpers/type/list.py` & `threemystic_common-0.1.2/threemystic_common/domain/helpers/type/list.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,23 +17,34 @@
     raise self._main_reference.exception().exception(
       exception_type = "argument"
     ).type_error(
       logger = self._main_reference.get_common().get_logger(),
       name = "data",
       message = f"Data is None"
     )
-  def unique_list(self, data, *args, **kwargs):
+  def unique_list(self, data, case_sensitive = True, *args, **kwargs):
+    if data is None or not self._main_reference.helper_type().general().is_type(data, list):
+      return data
+    
     if len(data) < 2:
       return data
       
     unique_data = {}
     for item in data:
-      unique_data[self._main_reference.encryption().hash(hash_method="sha1").generate_hash(self._main_reference.helper_json().dumps(data= item))] = item
+      if case_sensitive:
+        unique_data[self._main_reference.encryption().hash(hash_method="sha1").generate_hash(self._main_reference.helper_json().dumps(data= item))] = item
+        continue
+      unique_data[(self._main_reference.encryption().hash(hash_method="sha1").generate_hash(
+        self._main_reference.helper_type().string().set_case(
+          string_value= self._main_reference.helper_json().dumps(data= item),
+          case = "lower"
+        ))
+      )] = item
 
-    return [ val for val in unique_data.values()]
+    return list(unique_data.values())
   
   def __flatten(self, data, flatten_list, recursive= True, *args, **kwargs):
     if not self._main_reference.helper_type().general().is_type(data, list):
       raise self._main_reference.exception().exception(
         exception_type = "argument"
       ).type_error(
         logger = self._main_reference.get_common().get_logger(),
```

### Comparing `threemystic_common-0.1.1/threemystic_common/domain/helpers/type/logging.py` & `threemystic_common-0.1.2/threemystic_common/domain/helpers/type/logging.py`

 * *Files identical despite different names*

### Comparing `threemystic_common-0.1.1/threemystic_common/domain/helpers/type/regex.py` & `threemystic_common-0.1.2/threemystic_common/domain/helpers/type/regex.py`

 * *Files identical despite different names*

### Comparing `threemystic_common-0.1.1/threemystic_common/domain/helpers/type/requests.py` & `threemystic_common-0.1.2/threemystic_common/domain/helpers/type/requests.py`

 * *Files identical despite different names*

### Comparing `threemystic_common-0.1.1/threemystic_common/domain/helpers/type/string.py` & `threemystic_common-0.1.2/threemystic_common/domain/helpers/type/string.py`

 * *Files 0% similar despite different names*

```diff
@@ -117,14 +117,15 @@
     if str(string_value).strip() == "":
       return True
     
     return False
   
   # split_string
   def split(self, string_value, trim_data = True, remove_empty = True, separator = "[,;]", regex_split = True, *args, **kwargs):
+    
     if regex_split:
       return self._main_reference.helper_type().regex().split(
         string_value= string_value,
         trim_data= trim_data,
         remove_empty= remove_empty,
         separator= separator
       )
```

### Comparing `threemystic_common-0.1.1/.gitignore` & `threemystic_common-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `threemystic_common-0.1.1/LICENSE` & `threemystic_common-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `threemystic_common-0.1.1/README.md` & `threemystic_common-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `threemystic_common-0.1.1/hatch.toml` & `threemystic_common-0.1.2/hatch.toml`

 * *Files identical despite different names*

### Comparing `threemystic_common-0.1.1/pyproject.toml` & `threemystic_common-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `threemystic_common-0.1.1/PKG-INFO` & `threemystic_common-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: threemystic-common
-Version: 0.1.1
+Version: 0.1.2
 Summary: Common Library for for various tool sets
 Project-URL: Homepage, https://github.com/3MysticApes/3mystic_common
 Project-URL: Bug Tracker, https://github.com/3MysticApes/3mystic_common/issues
 Author: Ron Truex
 License-Expression: MIT
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
```

