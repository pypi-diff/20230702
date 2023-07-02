# Comparing `tmp/spark_quality_rules_tools-0.3.6.tar.gz` & `tmp/spark_quality_rules_tools-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spark_quality_rules_tools-0.3.6.tar", last modified: Sat Jul  1 21:41:31 2023, max compression
+gzip compressed data, was "spark_quality_rules_tools-0.3.7.tar", last modified: Sun Jul  2 02:34:52 2023, max compression
```

## Comparing `spark_quality_rules_tools-0.3.6.tar` & `spark_quality_rules_tools-0.3.7.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-07-01 21:41:31.686282 spark_quality_rules_tools-0.3.6/
--rw-rw-rw-   0        0        0     1092 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.3.6/LICENSE
--rw-rw-rw-   0        0        0       50 2023-06-14 13:33:57.000000 spark_quality_rules_tools-0.3.6/MANIFEST.in
--rw-rw-rw-   0        0        0     4041 2023-07-01 21:41:31.686282 spark_quality_rules_tools-0.3.6/PKG-INFO
--rw-rw-rw-   0        0        0     3242 2023-06-14 13:39:58.000000 spark_quality_rules_tools-0.3.6/README.md
--rw-rw-rw-   0        0        0      661 2023-07-01 21:30:21.000000 spark_quality_rules_tools-0.3.6/pyproject.toml
--rw-rw-rw-   0        0        0       86 2023-07-01 21:41:31.687282 spark_quality_rules_tools-0.3.6/setup.cfg
--rw-rw-rw-   0        0        0     1210 2023-07-01 21:41:18.000000 spark_quality_rules_tools-0.3.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-01 21:41:31.663278 spark_quality_rules_tools-0.3.6/spark_quality_rules_tools/
--rw-rw-rw-   0        0        0     2342 2023-07-01 21:41:18.000000 spark_quality_rules_tools-0.3.6/spark_quality_rules_tools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-01 21:41:31.682282 spark_quality_rules_tools-0.3.6/spark_quality_rules_tools/functions/
--rw-rw-rw-   0        0        0        0 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.3.6/spark_quality_rules_tools/functions/__init__.py
--rw-rw-rw-   0        0        0    45106 2023-07-01 21:41:18.000000 spark_quality_rules_tools-0.3.6/spark_quality_rules_tools/functions/generator.py
-drwxrwxrwx   0        0        0        0 2023-07-01 21:41:31.684282 spark_quality_rules_tools-0.3.6/spark_quality_rules_tools/utils/
--rw-rw-rw-   0        0        0       75 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.3.6/spark_quality_rules_tools/utils/__init__.py
--rw-rw-rw-   0        0        0      416 2023-04-12 03:25:49.000000 spark_quality_rules_tools-0.3.6/spark_quality_rules_tools/utils/color.py
--rw-rw-rw-   0        0        0     2138 2023-06-30 23:04:24.000000 spark_quality_rules_tools-0.3.6/spark_quality_rules_tools/utils/resolve.py
-drwxrwxrwx   0        0        0        0 2023-07-01 21:41:31.686282 spark_quality_rules_tools-0.3.6/spark_quality_rules_tools/utils/resource/
--rw-rw-rw-   0        0        0      532 2023-06-30 23:04:24.000000 spark_quality_rules_tools-0.3.6/spark_quality_rules_tools/utils/resource/resolve_edge.conf
--rw-rw-rw-   0        0        0      742 2023-06-30 23:04:24.000000 spark_quality_rules_tools-0.3.6/spark_quality_rules_tools/utils/resource/resolve_sandbox.conf
--rw-rw-rw-   0        0        0    25817 2023-04-12 03:25:49.000000 spark_quality_rules_tools-0.3.6/spark_quality_rules_tools/utils/resource/rules.json
--rw-rw-rw-   0        0        0     3742 2023-06-30 23:04:24.000000 spark_quality_rules_tools-0.3.6/spark_quality_rules_tools/utils/rules.py
-drwxrwxrwx   0        0        0        0 2023-07-01 21:41:31.680281 spark_quality_rules_tools-0.3.6/spark_quality_rules_tools.egg-info/
--rw-rw-rw-   0        0        0     4041 2023-07-01 21:41:31.000000 spark_quality_rules_tools-0.3.6/spark_quality_rules_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      784 2023-07-01 21:41:31.000000 spark_quality_rules_tools-0.3.6/spark_quality_rules_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-01 21:41:31.000000 spark_quality_rules_tools-0.3.6/spark_quality_rules_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      186 2023-07-01 21:41:31.000000 spark_quality_rules_tools-0.3.6/spark_quality_rules_tools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2023-07-01 21:41:31.000000 spark_quality_rules_tools-0.3.6/spark_quality_rules_tools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-02 02:34:52.770294 spark_quality_rules_tools-0.3.7/
+-rw-rw-rw-   0        0        0     1092 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.3.7/LICENSE
+-rw-rw-rw-   0        0        0       50 2023-06-14 13:33:57.000000 spark_quality_rules_tools-0.3.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     4041 2023-07-02 02:34:52.770294 spark_quality_rules_tools-0.3.7/PKG-INFO
+-rw-rw-rw-   0        0        0     3242 2023-06-14 13:39:58.000000 spark_quality_rules_tools-0.3.7/README.md
+-rw-rw-rw-   0        0        0      685 2023-07-01 22:58:24.000000 spark_quality_rules_tools-0.3.7/pyproject.toml
+-rw-rw-rw-   0        0        0       86 2023-07-02 02:34:52.771295 spark_quality_rules_tools-0.3.7/setup.cfg
+-rw-rw-rw-   0        0        0     1210 2023-07-02 02:34:37.000000 spark_quality_rules_tools-0.3.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-02 02:34:52.747290 spark_quality_rules_tools-0.3.7/spark_quality_rules_tools/
+-rw-rw-rw-   0        0        0     2342 2023-07-01 21:41:18.000000 spark_quality_rules_tools-0.3.7/spark_quality_rules_tools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-02 02:34:52.765293 spark_quality_rules_tools-0.3.7/spark_quality_rules_tools/functions/
+-rw-rw-rw-   0        0        0        0 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.3.7/spark_quality_rules_tools/functions/__init__.py
+-rw-rw-rw-   0        0        0    45890 2023-07-01 23:29:25.000000 spark_quality_rules_tools-0.3.7/spark_quality_rules_tools/functions/generator.py
+drwxrwxrwx   0        0        0        0 2023-07-02 02:34:52.767294 spark_quality_rules_tools-0.3.7/spark_quality_rules_tools/utils/
+-rw-rw-rw-   0        0        0       75 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.3.7/spark_quality_rules_tools/utils/__init__.py
+-rw-rw-rw-   0        0        0      416 2023-04-12 03:25:49.000000 spark_quality_rules_tools-0.3.7/spark_quality_rules_tools/utils/color.py
+-rw-rw-rw-   0        0        0     2138 2023-06-30 23:04:24.000000 spark_quality_rules_tools-0.3.7/spark_quality_rules_tools/utils/resolve.py
+drwxrwxrwx   0        0        0        0 2023-07-02 02:34:52.769295 spark_quality_rules_tools-0.3.7/spark_quality_rules_tools/utils/resource/
+-rw-rw-rw-   0        0        0      532 2023-06-30 23:04:24.000000 spark_quality_rules_tools-0.3.7/spark_quality_rules_tools/utils/resource/resolve_edge.conf
+-rw-rw-rw-   0        0        0      742 2023-06-30 23:04:24.000000 spark_quality_rules_tools-0.3.7/spark_quality_rules_tools/utils/resource/resolve_sandbox.conf
+-rw-rw-rw-   0        0        0    25817 2023-07-02 01:22:13.000000 spark_quality_rules_tools-0.3.7/spark_quality_rules_tools/utils/resource/rules.json
+-rw-rw-rw-   0        0        0     3742 2023-06-30 23:04:24.000000 spark_quality_rules_tools-0.3.7/spark_quality_rules_tools/utils/rules.py
+drwxrwxrwx   0        0        0        0 2023-07-02 02:34:52.763293 spark_quality_rules_tools-0.3.7/spark_quality_rules_tools.egg-info/
+-rw-rw-rw-   0        0        0     4041 2023-07-02 02:34:52.000000 spark_quality_rules_tools-0.3.7/spark_quality_rules_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      784 2023-07-02 02:34:52.000000 spark_quality_rules_tools-0.3.7/spark_quality_rules_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-02 02:34:52.000000 spark_quality_rules_tools-0.3.7/spark_quality_rules_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      205 2023-07-02 02:34:52.000000 spark_quality_rules_tools-0.3.7/spark_quality_rules_tools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2023-07-02 02:34:52.000000 spark_quality_rules_tools-0.3.7/spark_quality_rules_tools.egg-info/top_level.txt
```

### Comparing `spark_quality_rules_tools-0.3.6/LICENSE` & `spark_quality_rules_tools-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.3.6/PKG-INFO` & `spark_quality_rules_tools-0.3.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spark_quality_rules_tools
-Version: 0.3.6
+Version: 0.3.7
 Summary: spark_quality_rules_tools
 Home-page: https://github.com/jonaqp/spark_quality_rules_tools/
 Author: Jonathan Quiza
 Author-email: jony327@gmail.com
 License: UNKNOWN
 Download-URL: https://github.com/jonaqp/spark_quality_rules_tools/archive/main.zip
 Keywords: spark,dq,rules,hammurabies
```

### Comparing `spark_quality_rules_tools-0.3.6/README.md` & `spark_quality_rules_tools-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.3.6/pyproject.toml` & `spark_quality_rules_tools-0.3.7/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 pyarrow = "12.0.0"
 setuptools = "58.2.0"
 wheel = "0.40.0"
 spark-dataframe-tools = "^0.2.0"
 color-tools = "^0.0.2"
 pyhocon = "^0.3.60"
 tqdm = "^4.65.0"
+prettytable = "^3.8.0"
 
 
 [tool.poetry.group.dev.dependencies]
 jupyterlab = "^4.0.0"
 twine = "^4.0.2"
 
 [build-system]
```

### Comparing `spark_quality_rules_tools-0.3.6/setup.py` & `spark_quality_rules_tools-0.3.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from setuptools import find_packages
 
 setuppath = os.path.dirname(os.path.abspath(__file__))
 
 setup(
     name='spark_quality_rules_tools',
     packages=find_packages(),
-    version='0.3.6',
+    version='0.3.7',
     description='spark_quality_rules_tools',
     long_description=open(os.path.join(setuppath, 'README.md')).read(),
     long_description_content_type="text/markdown",
     author='Jonathan Quiza',
     author_email='jony327@gmail.com',
     url='https://github.com/jonaqp/spark_quality_rules_tools/',
     download_url='https://github.com/jonaqp/spark_quality_rules_tools/archive/main.zip',
```

### Comparing `spark_quality_rules_tools-0.3.6/spark_quality_rules_tools/__init__.py` & `spark_quality_rules_tools-0.3.7/spark_quality_rules_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.3.6/spark_quality_rules_tools/functions/generator.py` & `spark_quality_rules_tools-0.3.7/spark_quality_rules_tools/functions/generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -931,7 +931,27 @@
     rule_id = str(id_split[-2])
     rule_correlative = str(id_split[-1])
 
     dir_hocons_filename = os.path.join(dir_hocons_name, uuaa_name, f"{url_conf_name}_{rule_country}_{rule_type}_{rule_id}_{rule_correlative}.conf")
     if is_windows:
         dir_hocons_filename = dir_hocons_filename.replace("\\", "/")
     get_validate_rules(hocons_dir=dir_hocons_filename)
+
+
+def get_rules_list():
+    import os
+    import json
+    from prettytable import PrettyTable
+    from spark_quality_rules_tools.utils.color import get_color_b
+    from spark_quality_rules_tools.utils import BASE_DIR
+    json_resource_rules = os.path.join(BASE_DIR, "utils", "resource", "rules.json")
+
+    with open(json_resource_rules) as f:
+        default_rules = json.load(f)
+    rules_config = default_rules.get("rules_config", None)
+
+    t = PrettyTable()
+    t.field_names = [get_color_b("DQ NAME"), get_color_b("VERSION"), get_color_b("DESCRIPTION")]
+    for k, v in rules_config.items():
+        for key_name, value_name in v.items():
+            t.add_row([key_name, value_name[0].get("rules_version"), value_name[0].get("rules_name")])
+        print(t)
```

### Comparing `spark_quality_rules_tools-0.3.6/spark_quality_rules_tools/utils/resolve.py` & `spark_quality_rules_tools-0.3.7/spark_quality_rules_tools/utils/resolve.py`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.3.6/spark_quality_rules_tools/utils/resource/resolve_edge.conf` & `spark_quality_rules_tools-0.3.7/spark_quality_rules_tools/utils/resource/resolve_edge.conf`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.3.6/spark_quality_rules_tools/utils/resource/resolve_sandbox.conf` & `spark_quality_rules_tools-0.3.7/spark_quality_rules_tools/utils/resource/resolve_sandbox.conf`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.3.6/spark_quality_rules_tools/utils/resource/rules.json` & `spark_quality_rules_tools-0.3.7/spark_quality_rules_tools/utils/resource/rules.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9357771364630739%*

 * *Differences: {"'rules_common_properties'": "{0: {'id': {insert: [(1, 'True')], delete: [1]}}}",*

 * * "'rules_config'": "{'availability': {'DateRangeFileRule': {0: {'rules_columns': {0: {'column': "*

 * *                   "{insert: [(1, 'True')], delete: [1]}, 'value': {insert: [(1, 'True')], delete: "*

 * *                   "[1]}, 'acceptanceMin': {insert: [(1, 'False')], delete: [1]}, 'minThreshold': "*

 * *                   "{insert: [(1, 'False')], delete: [1]}, 'targetThreshold': {insert: [(1, "*

 * *                   "'False')], delet […]*

```diff
@@ -1,94 +1,94 @@
 {
     "rules_common_properties": [
         {
             "id": [
                 "String",
-                "true",
+                "True",
                 ""
             ]
         }
     ],
     "rules_config": {
         "accuracy": {
             "DynamicRatingVariationRule": [
                 {
                     "apply_rules_common": true,
                     "rules_class": "com.datio.hammurabi.rules.accuracy.DynamicRatingVariationRule",
                     "rules_columns": [
                         {
                             "acceptanceMin": [
                                 "Double",
-                                "false",
+                                "False",
                                 "100"
                             ],
                             "column": [
                                 "String",
-                                "true",
+                                "True",
                                 ""
                             ],
                             "dataValues": [
                                 "Dict",
-                                "true",
+                                "True",
                                 ""
                             ],
                             "dataValuesSubset": [
                                 "String",
-                                "true",
+                                "True",
                                 ""
                             ],
                             "drillDown": [
                                 "Array[String]",
-                                "false",
+                                "False",
                                 "None"
                             ],
                             "isCritical": [
                                 "Boolean",
-                                "false",
-                                "false"
+                                "False",
+                                "False"
                             ],
                             "keyColumns": [
                                 "Array[Dict]",
-                                "true",
+                                "True",
                                 ""
                             ],
                             "minThreshold": [
                                 "Double",
-                                "true",
+                                "True",
                                 "100"
                             ],
                             "notches": [
                                 "Integer",
-                                "true",
+                                "True",
                                 ""
                             ],
                             "notchesColumn": [
                                 "String",
-                                "true",
+                                "True",
                                 ""
                             ],
                             "notchesColumnValues": [
                                 "String",
-                                "true",
+                                "True",
                                 ""
                             ],
                             "ratings": [
                                 "Dict",
-                                "true",
+                                "True",
                                 ""
                             ],
                             "targetThreshold": [
                                 "Double",
-                                "true",
+                                "True",
                                 "100"
                             ],
                             "withRefusals": [
                                 "Boolean",
-                                "false",
-                                "false"
+                                "False",
+                                "False"
                             ]
                         }
                     ],
                     "rules_name": "Comparison of the value of the same data between periods, with the maximum variation referred to a dynamic catalogue",
                     "rules_version": "6.10"
                 }
             ],
@@ -96,60 +96,60 @@
                 {
                     "apply_rules_common": true,
                     "rules_class": "com.datio.hammurabi.rules.accuracy.HerfindahlRule",
                     "rules_columns": [
                         {
                             "acceptanceMin": [
                                 "Double",
-                                "false",
+                                "False",
                                 "100"
                             ],
                             "column": [
                                 "String",
-                                "true",
+                                "True",
                                 ""
                             ],
                             "dataValues": [
                                 "Dict",
-                                "true",
+                                "True",
                                 ""
                             ],
                             "dataValuesSubset": [
                                 "String",
-                                "true",
+                                "True",
                                 ""
                             ],
                             "drillDown": [
                                 "Array[String]",
-                                "false",
+                                "False",
                                 "None"
                             ],
                             "isCritical": [
                                 "Boolean",
-                                "false",
-                                "true"
+                                "False",
+                                "True"
                             ],
                             "maxValue": [
                                 "Double",
-                                "false",
+                                "False",
                                 ""
                             ],
                             "minThreshold": [
                                 "Double",
-                                "false",
+                                "False",
                                 "100"
                             ],
                             "minValue": [
                                 "Double",
-                                "false",
+                                "False",
                                 ""
                             ],
                             "targetThreshold": [
                                 "Double",
-                                "false",
+                                "False",
                                 "100"
                             ]
                         }
                     ],
                     "rules_name": "Herfindahl",
                     "rules_version": "6.11"
                 }
@@ -158,76 +158,76 @@
                 {
                     "apply_rules_common": true,
                     "rules_class": "com.datio.hammurabi.rules.accuracy.StaticGatheringRule",
                     "rules_columns": [
                         {
                             "acceptanceMinBalance": [
                                 "Double",
-                                "false",
+                                "False",
                                 "100"
                             ],
                             "balanceIds": [
                                 "Array[String]",
-                                "false",
+                                "False",
                                 "None"
                             ],
                             "column": [
                                 "String",
-                                "true",
+                                "True",
                                 ""
                             ],
                             "drillDown": [
                                 "Array[String]",
-                                "false",
+                                "False",
                                 "None"
                             ],
                             "isCritical": [
                                 "Boolean",
-                                "false",
-                                "false"
+                                "False",
+                                "False"
                             ],
                             "keyColumns": [
                                 "Array",
-                                "true",
+                                "True",
                                 ""
                             ],
                             "lowerBound": [
                                 "String",
-                                "false",
+                                "False",
                                 ""
                             ],
                             "minThreshold": [
                                 "Double",
-                                "false",
+                                "False",
                                 "100"
                             ],
                             "subset": [
                                 "String",
-                                "false",
+                                "False",
                                 "None"
                             ],
                             "targetThreshold": [
                                 "Double",
-                                "false",
+                                "False",
                                 "100"
                             ],
                             "upperBound": [
                                 "String",
-                                "false",
+                                "False",
                                 ""
                             ],
                             "values": [
                                 "Array[String]",
-                                "true",
+                                "True",
                                 ""
                             ],
                             "withRefusals": [
                                 "Boolean",
-                                "false",
-                                "false"
+                                "False",
+                                "False"
                             ]
                         }
                     ],
                     "rules_name": "Check gathering of values for a static catalog",
                     "rules_version": "6.1"
                 }
             ],
@@ -235,71 +235,71 @@
                 {
                     "apply_rules_common": true,
                     "rules_class": "com.datio.hammurabi.rules.accuracy.ValueSensitivityThresholdRule",
                     "rules_columns": [
                         {
                             "acceptanceMin": [
                                 "Double",
-                                "false",
+                                "False",
                                 "100"
                             ],
                             "aggregation": [
                                 "Array",
-                                "true",
+                                "True",
                                 ""
                             ],
                             "column": [
                                 "String",
-                                "true",
+                                "True",
                                 ""
                             ],
                             "drillDown": [
                                 "Array[String]",
-                                "false",
+                                "False",
                                 "None"
                             ],
                             "isCritical": [
                                 "Boolean",
-                                "false",
-                                "false"
+                                "False",
+                                "False"
                             ],
                             "keyColumns": [
                                 "Array[String]",
-                                "true",
+                                "True",
                                 ""
                             ],
                             "lowerBound": [
                                 "Long",
-                                "false",
+                                "False",
                                 ""
                             ],
                             "minThreshold": [
                                 "Double",
-                                "true",
+                                "True",
                                 "100"
                             ],
                             "subset": [
                                 "String",
-                                "false",
+                                "False",
                                 "None"
                             ],
                             "targetThreshold": [
                                 "Double",
-                                "true",
+                                "True",
                                 "100"
                             ],
                             "upperBound": [
                                 "Long",
-                                "false",
+                                "False",
                                 ""
                             ],
                             "withRefusals": [
                                 "Boolean",
-                                "false",
-                                "false"
+                                "False",
+                                "False"
                             ]
                         }
                     ],
                     "rules_name": "Check the sensitivity of a value to a given threshold",
                     "rules_version": "6.2"
                 }
             ],
@@ -307,86 +307,86 @@
                 {
                     "apply_rules_common": true,
                     "rules_class": "com.datio.hammurabi.rules.accuracy.ValueVariationRule",
                     "rules_columns": [
                         {
                             "acceptanceMin": [
                                 "Double",
-                                "false",
+                                "False",
                                 "100"
                             ],
                             "acceptanceMinBalance": [
                                 "Double",
-                                "false",
+                                "False",
                                 "100"
                             ],
                             "aggregation": [
                                 "String",
-                                "true",
+                                "True",
                                 ""
                             ],
                             "balanceIds": [
                                 "Array[String]",
-                                "false",
+                                "False",
                                 "None"
                             ],
                             "column": [
                                 "String",
-                                "true",
+                                "True",
                                 ""
                             ],
                             "dataValues": [
                                 "Dict",
-                                "true",
+                                "True",
                                 ""
                             ],
                             "dataValuesSubset": [
                                 "String",
-                                "true",
+                                "True",
                                 ""
                             ],
                             "drillDown": [
                                 "Array[String]",
-                                "false",
+                                "False",
                                 "None"
                             ],
                             "isCritical": [
                                 "Boolean",
-                                "false",
-                                "false"
+                                "False",
+                                "False"
                             ],
                             "keyColumns": [
                                 "Array[String]",
-                                "true",
+                                "True",
                                 ""
                             ],
                             "minThreshold": [
                                 "Double",
-                                "true",
+                                "True",
                                 "100"
                             ],
                             "subset": [
                                 "String",
-                                "false",
+                                "False",
                                 "None"
                             ],
                             "targetThreshold": [
                                 "Double",
-                                "true",
+                                "True",
                                 "100"
                             ],
                             "variationAllowed": [
                                 "Double",
-                                "true",
+                                "True",
                                 ""
                             ],
                             "withRefusals": [
                                 "Boolean",
-                                "false",
-                                "false"
+                                "False",
+                                "False"
                             ]
                         }
                     ],
                     "rules_name": "Check the variation of a value between periods",
                     "rules_version": "6.4"
                 }
             ],
@@ -394,76 +394,76 @@
                 {
                     "apply_rules_common": true,
                     "rules_class": "com.datio.hammurabi.rules.accuracy.VolumetricTrendRule",
                     "rules_columns": [
                         {
                             "acceptanceMin": [
                                 "Double",
-                                "false",
+                                "False",
                                 "100"
                             ],
                             "dataValues": [
                                 "Dict",
-                                "true",
+                                "True",
                                 ""
                             ],
                             "dataValuesSubset": [
                                 "String",
-                                "true",
+                                "True",
                                 ""
                             ],
                             "drillDown": [
                                 "Array[String]",
-                                "false",
+                                "False",
                                 "None"
                             ],
                             "isCritical": [
                                 "Boolean",
-                                "false",
-                                "false"
+                                "False",
+                                "False"
                             ],
                             "lowerBound": [
                                 "Double",
-                                "false",
+                                "False",
                                 ""
                             ],
                             "maxValue": [
                                 "Double",
-                                "false",
+                                "False",
                                 ""
                             ],
                             "minThreshold": [
                                 "Double",
-                                "true",
+                                "True",
                                 "100"
                             ],
                             "minValue": [
                                 "Double",
-                                "false",
+                                "False",
                                 ""
                             ],
                             "subset": [
                                 "String",
-                                "false",
+                                "False",
                                 "None"
                             ],
                             "targetThreshold": [
                                 "Double",
-                                "true",
+                                "True",
                                 "100"
                             ],
                             "upperBound": [
                                 "Double",
-                                "false",
+                                "False",
                                 ""
                             ],
                             "withRefusals": [
                                 "Boolean",
-                                "false",
-                                "false"
+                                "False",
+                                "False"
                             ]
                         }
                     ],
                     "rules_name": "Check volumetric trend",
                     "rules_version": "6.9"
                 }
             ]
@@ -473,56 +473,56 @@
                 {
                     "apply_rules_common": true,
                     "rules_class": "com.datio.hammurabi.rules.availability.DateRangeFileRule",
                     "rules_columns": [
                         {
                             "acceptanceMin": [
                                 "Double",
-                                "false",
+                                "False",
                                 "100"
                             ],
                             "column": [
                                 "String",
-                                "true",
+                                "True",
                                 ""
                             ],
                             "drillDown": [
                                 "Array[String]",
-                                "false",
+                                "False",
                                 "None"
                             ],
                             "isCritical": [
                                 "Boolean",
-                                "false",
-                                "false"
+                                "False",
+                                "False"
                             ],
                             "minThreshold": [
                                 "Double",
-                                "false",
+                                "False",
                                 "100"
                             ],
                             "subset": [
                                 "String",
-                                "false",
+                                "False",
                                 "None"
                             ],
                             "targetThreshold": [
                                 "Double",
-                                "false",
+                                "False",
                                 "100"
                             ],
                             "value": [
                                 "Timestamp",
-                                "true",
+                                "True",
                                 ""
                             ],
                             "withRefusals": [
                                 "Boolean",
-                                "false",
-                                "false"
+                                "False",
+                                "False"
                             ]
                         }
                     ],
                     "rules_name": "Date file value within range",
                     "rules_version": "1.1"
                 }
             ],
@@ -530,61 +530,61 @@
                 {
                     "apply_rules_common": true,
                     "rules_class": "com.datio.hammurabi.rules.availability.DateValidationRule",
                     "rules_columns": [
                         {
                             "acceptanceMin": [
                                 "Double",
-                                "false",
+                                "False",
                                 "100"
                             ],
                             "column": [
                                 "String",
-                                "true",
+                                "True",
                                 ""
                             ],
                             "drillDown": [
                                 "Array[String]",
-                                "false",
+                                "False",
                                 "None"
                             ],
                             "format": [
                                 "String",
-                                "false",
+                                "False",
                                 "yyyy-MM-dd"
                             ],
                             "isCritical": [
                                 "Boolean",
-                                "false",
-                                "false"
+                                "False",
+                                "False"
                             ],
                             "minThreshold": [
                                 "Double",
-                                "false",
+                                "False",
                                 "100"
                             ],
                             "subset": [
                                 "String",
-                                "false",
+                                "False",
                                 "None"
                             ],
                             "targetThreshold": [
                                 "Double",
-                                "false",
+                                "False",
                                 "100"
                             ],
                             "value": [
                                 "String",
-                                "true",
+                                "True",
                                 ""
                             ],
                             "withRefusals": [
                                 "Boolean",
-                                "false",
-                                "false"
+                                "False",
+                                "False"
                             ]
                         }
                     ],
                     "rules_name": "Updating the value of the data on the required date",
                     "rules_version": "1.2"
                 }
             ]
@@ -594,45 +594,45 @@
                 {
                     "apply_rules_common": true,
                     "rules_class": "com.datio.hammurabi.rules.completeness.BasicPerimeterCompletenessRule",
                     "rules_columns": [
                         {
                             "acceptanceMin": [
                                 "Double",
-                                "false",
+                                "False",
                                 "100"
                             ],
                             "dataValues": [
                                 "Dict",
-                                "true",
+                                "True",
                                 ""
                             ],
                             "drillDown": [
                                 "Array[String]",
-                                "false",
+                                "False",
                                 "None"
                             ],
                             "isCritical": [
                                 "Boolean",
-                                "false",
-                                "false"
+                                "False",
+                                "False"
                             ],
                             "minThreshold": [
                                 "Double",
-                                "false",
+                                "False",
                                 "100"
                             ],
                             "subset": [
                                 "String",
-                                "false",
+                                "False",
                                 "None"
                             ],
                             "targetThreshold": [
                                 "Double",
-                                "false",
+                                "False",
                                 "100"
                             ]
                         }
                     ],
                     "rules_name": "Perimeter Completeness",
                     "rules_version": "2.2-1"
                 }
@@ -641,45 +641,45 @@
                 {
                     "apply_rules_common": true,
                     "rules_class": "com.datio.hammurabi.rules.completeness.BasicPerimeterVariationCompletenessRule",
                     "rules_columns": [
                         {
                             "acceptanceMin": [
                                 "Double",
-                                "false",
+                                "False",
                                 "100"
                             ],
                             "dataValues": [
                                 "Dict",
-                                "true",
+                                "True",
                                 ""
                             ],
                             "drillDown": [
                                 "Array[String]",
-                                "false",
+                                "False",
                                 "None"
                             ],
                             "isCritical": [
                                 "Boolean",
-                                "false",
-                                "false"
+                                "False",
+                                "False"
                             ],
                             "minThreshold": [
                                 "Double",
-                                "false",
+                                "False",
                                 "100"
                             ],
                             "subset": [
                                 "String",
-                                "false",
+                                "False",
                                 "None"
                             ],
                             "targetThreshold": [
                                 "Double",
-                                "false",
+                                "False",
                                 "100"
                             ]
                         }
                     ],
                     "rules_name": "Perimeter Completeness",
                     "rules_version": "2.2-2"
                 }
@@ -688,35 +688,35 @@
                 {
                     "apply_rules_common": true,
                     "rules_class": "com.datio.hammurabi.rules.completeness.CompletenessRule",
                     "rules_columns": [
                         {
                             "acceptanceMin": [
                                 "Double",
-                                "false",
+                                "False",
                                 "100"
                             ],
                             "drillDown": [
                                 "Array[String]",
-                                "false",
+                                "False",
                                 "None"
                             ],
                             "isCritical": [
                                 "Boolean",
-                                "false",
-                                "true"
+                                "False",
+                                "True"
                             ],
                             "minThreshold": [
                                 "Double",
-                                "false",
+                                "False",
                                 "100"
                             ],
                             "targetThreshold": [
                                 "Double",
-                                "false",
+                                "False",
                                 "100"
                             ]
                         }
                     ],
                     "rules_name": "Records Completeness",
                     "rules_version": "2.1"
                 }
@@ -725,50 +725,50 @@
                 {
                     "apply_rules_common": true,
                     "rules_class": "com.datio.hammurabi.rules.completeness.ConditionalPerimeterCompletenessRule",
                     "rules_columns": [
                         {
                             "acceptanceMin": [
                                 "Double",
-                                "false",
+                                "False",
                                 "100"
                             ],
                             "condition": [
                                 "String",
-                                "true",
+                                "True",
                                 ""
                             ],
                             "dataValues": [
                                 "Dict",
-                                "true",
+                                "True",
                                 ""
                             ],
                             "drillDown": [
                                 "Array[String]",
-                                "false",
+                                "False",
                                 "None"
                             ],
                             "isCritical": [
                                 "Boolean",
-                                "false",
-                                "true"
+                                "False",
+                                "True"
                             ],
                             "minThreshold": [
                                 "Double",
-                                "false",
+                                "False",
                                 "100"
                             ],
                             "subset": [
                                 "String",
-                                "false",
+                                "False",
                                 "None"
                             ],
                             "targetThreshold": [
                                 "Double",
-                                "false",
+                                "False",
                                 "100"
                             ]
                         }
                     ],
                     "rules_name": "Perimeter completeness with a filter",
                     "rules_version": "2.3-1"
                 }
@@ -777,45 +777,45 @@
                 {
                     "apply_rules_common": true,
                     "rules_class": "com.datio.hammurabi.rules.completeness.MetadataCompletenessRule",
                     "rules_columns": [
                         {
                             "acceptanceMin": [
                                 "Double",
-                                "false",
+                                "False",
                                 "100"
                             ],
                             "dataValues": [
                                 "Dict",
-                                "true",
+                                "True",
                                 ""
                             ],
                             "drillDown": [
                                 "Array[String]",
-                                "false",
+                                "False",
                                 "None"
                             ],
                             "isCritical": [
                                 "Boolean",
-                                "false",
-                                "true"
+                                "False",
+                                "True"
                             ],
                             "minThreshold": [
                                 "Double",
-                                "false",
+                                "False",
                                 "100"
                             ],
                             "subset": [
                                 "String",
-                                "false",
+                                "False",
                                 "None"
                             ],
                             "targetThreshold": [
                                 "Double",
-                                "false",
+                                "False",
                                 "100"
                             ]
                         }
                     ],
                     "rules_name": "Metadata completeness",
                     "rules_version": "2.4"
                 }
@@ -826,51 +826,51 @@
                 {
                     "apply_rules_common": true,
                     "rules_class": "com.datio.hammurabi.rules.consistence.DuplicateRule",
                     "rules_columns": [
                         {
                             "acceptanceMin": [
                                 "Double",
-                                "false",
+                                "False",
                                 "100"
                             ],
                             "columns": [
                                 "Array[String]",
-                                "true",
+                                "True",
                                 ""
                             ],
                             "drillDown": [
                                 "Array[String]",
-                                "false",
+                                "False",
                                 "None"
                             ],
                             "isCritical": [
                                 "Boolean",
-                                "false",
-                                "true"
+                                "False",
+                                "True"
                             ],
                             "minThreshold": [
                                 "Double",
-                                "false",
+                                "False",
                                 "100"
                             ],
                             "subset": [
                                 "String",
-                                "false",
+                                "False",
                                 "None"
                             ],
                             "targetThreshold": [
                                 "Double",
-                                "false",
+                                "False",
                                 "100"
                             ],
                             "withRefusals": [
                                 "Boolean",
-                                "false",
-                                "false"
+                                "False",
+                                "False"
                             ]
                         }
                     ],
                     "rules_name": "No duplicate values",
                     "rules_version": "4.2"
                 }
             ],
@@ -878,81 +878,81 @@
                 {
                     "apply_rules_common": true,
                     "rules_class": "com.datio.hammurabi.rules.consistence.ValueConciliationRule",
                     "rules_columns": [
                         {
                             "acceptanceMin": [
                                 "Double",
-                                "false",
+                                "False",
                                 "100"
                             ],
                             "acceptanceMinBalance": [
                                 "Double",
-                                "false",
+                                "False",
                                 "100"
                             ],
                             "balanceIds": [
                                 "Array[String]",
-                                "false",
+                                "False",
                                 "None"
                             ],
                             "column": [
                                 "String",
-                                "true",
+                                "True",
                                 ""
                             ],
                             "dataSystemId": [
                                 "String",
-                                "true",
+                                "True",
                                 ""
                             ],
                             "dataValues": [
                                 "Dict",
-                                "true",
+                                "True",
                                 ""
                             ],
                             "dataValuesSubset": [
                                 "String",
-                                "true",
+                                "True",
                                 ""
                             ],
                             "drillDown": [
                                 "Array[String]",
-                                "false",
+                                "False",
                                 "None"
                             ],
                             "isCritical": [
                                 "Boolean",
-                                "false",
-                                "false"
+                                "False",
+                                "False"
                             ],
                             "keyColumns": [
                                 "Array[Dict]",
-                                "true",
+                                "True",
                                 ""
                             ],
                             "minThreshold": [
                                 "Double",
-                                "false",
+                                "False",
                                 "100"
                             ],
                             "subset": [
                                 "String",
-                                "false",
+                                "False",
                                 "None"
                             ],
                             "targetThreshold": [
                                 "Double",
-                                "false",
+                                "False",
                                 "100"
                             ],
                             "withRefusals": [
                                 "Boolean",
-                                "false",
-                                "false"
+                                "False",
+                                "False"
                             ]
                         }
                     ],
                     "rules_name": "Reconciliation of the same/different data between different tables / repositories in the same moment of tim",
                     "rules_version": "4.3"
                 }
             ]
@@ -962,25 +962,25 @@
                 {
                     "apply_rules_common": true,
                     "rules_class": "com.datio.hammurabi.rules.integrity.ConcatRule",
                     "rules_columns": [
                         {
                             "columns": [
                                 "Array[String]",
-                                "true",
+                                "True",
                                 ""
                             ],
                             "delimiter": [
                                 "String",
-                                "true",
+                                "True",
                                 ""
                             ],
                             "referenceColumn": [
                                 "String",
-                                "true",
+                                "True",
                                 ""
                             ]
                         }
                     ],
                     "rules_name": "Concat Object Rule",
                     "rules_version": "5.6-1"
                 }
@@ -989,61 +989,61 @@
                 {
                     "apply_rules_common": true,
                     "rules_class": "com.datio.hammurabi.rules.integrity.ConcatRuleByColumn",
                     "rules_columns": [
                         {
                             "acceptanceMin": [
                                 "Double",
-                                "false",
+                                "False",
                                 "100"
                             ],
                             "columns": [
                                 "Array[String]",
-                                "true",
+                                "True",
                                 ""
                             ],
                             "delimiter": [
                                 "String",
-                                "true",
+                                "True",
                                 ""
                             ],
                             "drillDown": [
                                 "Array[String]",
-                                "false",
+                                "False",
                                 "None"
                             ],
                             "isCritical": [
                                 "Boolean",
-                                "false",
-                                "false"
+                                "False",
+                                "False"
                             ],
                             "minThreshold": [
                                 "Double",
-                                "false",
+                                "False",
                                 "100"
                             ],
                             "subset": [
                                 "String",
-                                "false",
+                                "False",
                                 "None"
                             ],
                             "targetThreshold": [
                                 "Double",
-                                "false",
+                                "False",
                                 "100"
                             ],
                             "value": [
                                 "String",
-                                "true",
+                                "True",
                                 ""
                             ],
                             "withRefusals": [
                                 "Boolean",
-                                "false",
-                                "false"
+                                "False",
+                                "False"
                             ]
                         }
                     ],
                     "rules_name": "ConcatByColumn Object Rule",
                     "rules_version": "5.6-2"
                 }
             ],
@@ -1051,40 +1051,40 @@
                 {
                     "apply_rules_common": true,
                     "rules_class": "com.datio.hammurabi.rules.integrity.ConditionalExpressionObjectRule",
                     "rules_columns": [
                         {
                             "condition": [
                                 "String",
-                                "true",
+                                "True",
                                 ""
                             ],
                             "drillDown": [
                                 "Array[String]",
-                                "false",
+                                "False",
                                 "None"
                             ],
                             "isCritical": [
                                 "Boolean",
-                                "false",
-                                "false"
+                                "False",
+                                "False"
                             ],
                             "minThreshold": [
                                 "Double",
-                                "false",
+                                "False",
                                 "100"
                             ],
                             "subset": [
                                 "String",
-                                "false",
+                                "False",
                                 "None"
                             ],
                             "targetThreshold": [
                                 "Double",
-                                "false",
+                                "False",
                                 "100"
                             ]
                         }
                     ],
                     "rules_name": "Conditional Expression Object Rule",
                     "rules_version": "5.4"
                 }
@@ -1093,55 +1093,55 @@
                 {
                     "apply_rules_common": true,
                     "rules_class": "com.datio.hammurabi.rules.integrity.ConditionalExpressionObjectsRule",
                     "rules_columns": [
                         {
                             "condition": [
                                 "String",
-                                "true",
+                                "True",
                                 ""
                             ],
                             "dataValues": [
                                 "Dict",
-                                "true",
+                                "True",
                                 ""
                             ],
                             "dataValuesSubset": [
                                 "String",
-                                "true",
+                                "True",
                                 ""
                             ],
                             "drillDown": [
                                 "Array[String]",
-                                "false",
+                                "False",
                                 "None"
                             ],
                             "isCritical": [
                                 "Boolean",
-                                "false",
-                                "false"
+                                "False",
+                                "False"
                             ],
                             "keyColumns": [
                                 "Array[Dict]",
-                                "true",
+                                "True",
                                 ""
                             ],
                             "minThreshold": [
                                 "Double",
-                                "false",
+                                "False",
                                 "100"
                             ],
                             "subset": [
                                 "String",
-                                "false",
+                                "False",
                                 "None"
                             ],
                             "targetThreshold": [
                                 "Double",
-                                "false",
+                                "False",
                                 "100"
                             ]
                         }
                     ],
                     "rules_name": "Conditional Expression Objects Rule",
                     "rules_version": "5.5"
                 }
@@ -1150,61 +1150,61 @@
                 {
                     "apply_rules_common": true,
                     "rules_class": "com.datio.hammurabi.rules.integrity.SameValueComparisonRule",
                     "rules_columns": [
                         {
                             "acceptanceMin": [
                                 "Double",
-                                "false",
+                                "False",
                                 "100"
                             ],
                             "column": [
                                 "Array[String], ",
-                                "true",
+                                "True",
                                 ""
                             ],
                             "condition": [
                                 "String",
-                                "true",
+                                "True",
                                 ""
                             ],
                             "drillDown": [
                                 "Array[String]",
-                                "false",
+                                "False",
                                 "None"
                             ],
                             "isCritical": [
                                 "Boolean",
-                                "false",
-                                "false"
+                                "False",
+                                "False"
                             ],
                             "keyColumns": [
                                 "Array[Dict]",
-                                "true",
+                                "True",
                                 ""
                             ],
                             "minThreshold": [
                                 "Double",
-                                "true",
+                                "True",
                                 "100"
                             ],
                             "subset": [
                                 "String",
-                                "false",
+                                "False",
                                 "None"
                             ],
                             "targetThreshold": [
                                 "Double",
-                                "true",
+                                "True",
                                 "100"
                             ],
                             "withRefusals": [
                                 "Boolean",
-                                "false",
-                                "false"
+                                "False",
+                                "False"
                             ]
                         }
                     ],
                     "rules_name": "Comparison of related data values that must fulfill a condition",
                     "rules_version": "5.3"
                 }
             ],
@@ -1212,86 +1212,86 @@
                 {
                     "apply_rules_common": true,
                     "rules_class": "com.datio.hammurabi.rules.integrity.ValueComparisonRule",
                     "rules_columns": [
                         {
                             "acceptanceMin": [
                                 "Double",
-                                "false",
+                                "False",
                                 "100"
                             ],
                             "acceptanceMinBalance": [
                                 "Double",
-                                "false",
+                                "False",
                                 "100"
                             ],
                             "balanceIds": [
                                 "Array[String]",
-                                "false",
+                                "False",
                                 "None"
                             ],
                             "column": [
                                 "String",
-                                "true",
+                                "True",
                                 ""
                             ],
                             "comparison": [
                                 "String",
-                                "true",
+                                "True",
                                 ""
                             ],
                             "condition": [
                                 "String",
-                                "true",
+                                "True",
                                 ""
                             ],
                             "dataValues": [
                                 "Dict",
-                                "true",
+                                "True",
                                 ""
                             ],
                             "dataValuesSubset": [
                                 "String",
-                                "true",
+                                "True",
                                 ""
                             ],
                             "drillDown": [
                                 "Array[String]",
-                                "false",
+                                "False",
                                 "None"
                             ],
                             "isCritical": [
                                 "Boolean",
-                                "false",
-                                "false"
+                                "False",
+                                "False"
                             ],
                             "keyColumns": [
                                 "Array[Dict]",
-                                "true",
+                                "True",
                                 ""
                             ],
                             "minThreshold": [
                                 "Double",
-                                "true",
+                                "True",
                                 "100"
                             ],
                             "subset": [
                                 "String",
-                                "false",
+                                "False",
                                 "None"
                             ],
                             "targetThreshold": [
                                 "Double",
-                                "true",
+                                "True",
                                 "100"
                             ],
                             "withRefusals": [
                                 "Boolean",
-                                "false",
-                                "false"
+                                "False",
+                                "False"
                             ]
                         }
                     ],
                     "rules_name": "Comparison of related data values that must fulfill a condition",
                     "rules_version": "5.2"
                 }
             ]
@@ -1301,76 +1301,76 @@
                 {
                     "apply_rules_common": true,
                     "rules_class": "com.datio.hammurabi.rules.validity.DynamicCatalogRule",
                     "rules_columns": [
                         {
                             "acceptanceMin": [
                                 "Double",
-                                "false",
+                                "False",
                                 "100"
                             ],
                             "acceptanceMinBalance": [
                                 "Double",
-                                "false",
+                                "False",
                                 "100"
                             ],
                             "balanceIds": [
                                 "Array[String]",
-                                "false",
+                                "False",
                                 "None"
                             ],
                             "columns": [
                                 "Array[String]",
-                                "true",
+                                "True",
                                 ""
                             ],
                             "dataValues": [
                                 "Dict",
-                                "true",
+                                "True",
                                 ""
                             ],
                             "dataValuesColumn": [
                                 "String",
-                                "true",
+                                "True",
                                 ""
                             ],
                             "dataValuesSubset": [
                                 "String",
-                                "true",
+                                "True",
                                 ""
                             ],
                             "drillDown": [
                                 "Array[String]",
-                                "false",
+                                "False",
                                 "None"
                             ],
                             "isCritical": [
                                 "Boolean",
-                                "false",
-                                "true"
+                                "False",
+                                "True"
                             ],
                             "minThreshold": [
                                 "Double",
-                                "false",
+                                "False",
                                 "100"
                             ],
                             "subset": [
                                 "String",
-                                "false",
+                                "False",
                                 "None"
                             ],
                             "targetThreshold": [
                                 "Double",
-                                "false",
+                                "False",
                                 "100"
                             ],
                             "withRefusals": [
                                 "Boolean",
-                                "false",
-                                "false"
+                                "False",
+                                "False"
                             ]
                         }
                     ],
                     "rules_name": "Check whether the data is in a specific dynamic catalog",
                     "rules_version": "3.5-2"
                 }
             ],
@@ -1378,56 +1378,56 @@
                 {
                     "apply_rules_common": true,
                     "rules_class": "com.datio.hammurabi.rules.validity.FormatValidationRule",
                     "rules_columns": [
                         {
                             "acceptanceMin": [
                                 "Double",
-                                "false",
+                                "False",
                                 "100"
                             ],
                             "columns": [
                                 "Array[String]",
-                                "true",
+                                "True",
                                 ""
                             ],
                             "drillDown": [
                                 "Array[String]",
-                                "false",
+                                "False",
                                 "None"
                             ],
                             "format": [
                                 "String",
-                                "true",
+                                "True",
                                 ""
                             ],
                             "isCritical": [
                                 "Boolean",
-                                "false",
-                                "true"
+                                "False",
+                                "True"
                             ],
                             "minThreshold": [
                                 "Double",
-                                "false",
+                                "False",
                                 "100"
                             ],
                             "subset": [
                                 "String",
-                                "false",
+                                "False",
                                 "None"
                             ],
                             "targetThreshold": [
                                 "Double",
-                                "false",
+                                "False",
                                 "100"
                             ],
                             "withRefusals": [
                                 "Boolean",
-                                "false",
-                                "false"
+                                "False",
+                                "False"
                             ]
                         }
                     ],
                     "rules_name": "Check the format",
                     "rules_version": "3.2"
                 }
             ],
@@ -1435,61 +1435,61 @@
                 {
                     "apply_rules_common": true,
                     "rules_class": "com.datio.hammurabi.rules.validity.NotNullValidationRule",
                     "rules_columns": [
                         {
                             "acceptanceMin": [
                                 "Double",
-                                "false",
+                                "False",
                                 "100"
                             ],
                             "acceptanceMinBalance": [
                                 "Double",
-                                "false",
+                                "False",
                                 "100"
                             ],
                             "balanceIds": [
                                 "Array[String]",
-                                "false",
+                                "False",
                                 "None"
                             ],
                             "columns": [
                                 "Array[String]",
-                                "true",
+                                "True",
                                 ""
                             ],
                             "drillDown": [
                                 "Array[String]",
-                                "false",
+                                "False",
                                 "None"
                             ],
                             "isCritical": [
                                 "Boolean",
-                                "false",
-                                "true"
+                                "False",
+                                "True"
                             ],
                             "minThreshold": [
                                 "Double",
-                                "false",
+                                "False",
                                 "100"
                             ],
                             "subset": [
                                 "String",
-                                "false",
+                                "False",
                                 "None"
                             ],
                             "targetThreshold": [
                                 "Double",
-                                "false",
+                                "False",
                                 "100"
                             ],
                             "withRefusals": [
                                 "Boolean",
-                                "false",
-                                "false"
+                                "False",
+                                "False"
                             ]
                         }
                     ],
                     "rules_name": "Not null or empty values",
                     "rules_version": "3.1"
                 }
             ],
@@ -1497,71 +1497,71 @@
                 {
                     "apply_rules_common": true,
                     "rules_class": "com.datio.hammurabi.rules.validity.NumericRangeRule",
                     "rules_columns": [
                         {
                             "acceptanceMin": [
                                 "Double",
-                                "false",
+                                "False",
                                 "100"
                             ],
                             "acceptanceMinBalance": [
                                 "Double",
-                                "false",
+                                "False",
                                 "100"
                             ],
                             "balanceIds": [
                                 "Array[String]",
-                                "false",
+                                "False",
                                 "None"
                             ],
                             "columns": [
                                 "Array[String]",
-                                "true",
+                                "True",
                                 ""
                             ],
                             "drillDown": [
                                 "Array[String]",
-                                "false",
+                                "False",
                                 "None"
                             ],
                             "isCritical": [
                                 "Boolean",
-                                "false",
-                                "true"
+                                "False",
+                                "True"
                             ],
                             "lowerBound": [
                                 "Double",
-                                "true",
+                                "True",
                                 ""
                             ],
                             "minThreshold": [
                                 "Double",
-                                "false",
+                                "False",
                                 "100"
                             ],
                             "subset": [
                                 "String",
-                                "false",
+                                "False",
                                 "None"
                             ],
                             "targetThreshold": [
                                 "Double",
-                                "false",
+                                "False",
                                 "100"
                             ],
                             "upperBound": [
                                 "Double",
-                                "true",
+                                "True",
                                 ""
                             ],
                             "withRefusals": [
                                 "Boolean",
-                                "false",
-                                "false"
+                                "False",
+                                "False"
                             ]
                         }
                     ],
                     "rules_name": "Numeric values within range",
                     "rules_version": "3.4"
                 }
             ],
@@ -1569,66 +1569,66 @@
                 {
                     "apply_rules_common": true,
                     "rules_class": "com.datio.hammurabi.rules.validity.StaticCatalogRule",
                     "rules_columns": [
                         {
                             "acceptanceMin": [
                                 "Double",
-                                "false",
+                                "False",
                                 "100"
                             ],
                             "acceptanceMinBalance": [
                                 "Double",
-                                "false",
+                                "False",
                                 "100"
                             ],
                             "balanceIds": [
                                 "Array[String]",
-                                "false",
+                                "False",
                                 "None"
                             ],
                             "columns": [
                                 "Array[String]",
-                                "true",
+                                "True",
                                 ""
                             ],
                             "drillDown": [
                                 "Array[String]",
-                                "false",
+                                "False",
                                 "None"
                             ],
                             "isCritical": [
                                 "Boolean",
-                                "false",
-                                "true"
+                                "False",
+                                "True"
                             ],
                             "minThreshold": [
                                 "Double",
-                                "false",
+                                "False",
                                 "100"
                             ],
                             "subset": [
                                 "String",
-                                "false",
+                                "False",
                                 "None"
                             ],
                             "targetThreshold": [
                                 "Double",
-                                "false",
+                                "False",
                                 "100"
                             ],
                             "values": [
                                 "Array[String]",
-                                "true",
+                                "True",
                                 ""
                             ],
                             "withRefusals": [
                                 "Boolean",
-                                "false",
-                                "false"
+                                "False",
+                                "False"
                             ]
                         }
                     ],
                     "rules_name": "Check whether the data is in a specific static catalog",
                     "rules_version": "3.5-1"
                 }
             ],
@@ -1636,56 +1636,56 @@
                 {
                     "apply_rules_common": true,
                     "rules_class": "com.datio.hammurabi.rules.validity.StaticForbiddenValuesRule",
                     "rules_columns": [
                         {
                             "acceptanceMin": [
                                 "Double",
-                                "false",
+                                "False",
                                 "100"
                             ],
                             "columns": [
                                 "Array[String]",
-                                "true",
+                                "True",
                                 ""
                             ],
                             "drillDown": [
                                 "Array[String]",
-                                "false",
+                                "False",
                                 "None"
                             ],
                             "isCritical": [
                                 "Boolean",
-                                "false",
-                                "false"
+                                "False",
+                                "False"
                             ],
                             "minThreshold": [
                                 "Double",
-                                "false",
+                                "False",
                                 "100"
                             ],
                             "subset": [
                                 "String",
-                                "false",
+                                "False",
                                 "None"
                             ],
                             "targetThreshold": [
                                 "Double",
-                                "false",
+                                "False",
                                 "100"
                             ],
                             "values": [
                                 "Array[String]",
-                                "true",
+                                "True",
                                 ""
                             ],
                             "withRefusals": [
                                 "Boolean",
-                                "false",
-                                "false"
+                                "False",
+                                "False"
                             ]
                         }
                     ],
                     "rules_name": "Check whether the data is not in a specific static forbidden values catalog",
                     "rules_version": "3.3"
                 }
             ]
```

### Comparing `spark_quality_rules_tools-0.3.6/spark_quality_rules_tools/utils/rules.py` & `spark_quality_rules_tools-0.3.7/spark_quality_rules_tools/utils/rules.py`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.3.6/spark_quality_rules_tools.egg-info/PKG-INFO` & `spark_quality_rules_tools-0.3.7/spark_quality_rules_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spark-quality-rules-tools
-Version: 0.3.6
+Version: 0.3.7
 Summary: spark_quality_rules_tools
 Home-page: https://github.com/jonaqp/spark_quality_rules_tools/
 Author: Jonathan Quiza
 Author-email: jony327@gmail.com
 License: UNKNOWN
 Download-URL: https://github.com/jonaqp/spark_quality_rules_tools/archive/main.zip
 Keywords: spark,dq,rules,hammurabies
```

### Comparing `spark_quality_rules_tools-0.3.6/spark_quality_rules_tools.egg-info/SOURCES.txt` & `spark_quality_rules_tools-0.3.7/spark_quality_rules_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

