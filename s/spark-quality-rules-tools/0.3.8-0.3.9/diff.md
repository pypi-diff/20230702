# Comparing `tmp/spark_quality_rules_tools-0.3.8.tar.gz` & `tmp/spark_quality_rules_tools-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spark_quality_rules_tools-0.3.8.tar", last modified: Sun Jul  2 03:06:27 2023, max compression
+gzip compressed data, was "spark_quality_rules_tools-0.3.9.tar", last modified: Sun Jul  2 03:08:49 2023, max compression
```

## Comparing `spark_quality_rules_tools-0.3.8.tar` & `spark_quality_rules_tools-0.3.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-07-02 03:06:27.940249 spark_quality_rules_tools-0.3.8/
--rw-rw-rw-   0        0        0     1092 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.3.8/LICENSE
--rw-rw-rw-   0        0        0       50 2023-06-14 13:33:57.000000 spark_quality_rules_tools-0.3.8/MANIFEST.in
--rw-rw-rw-   0        0        0     4041 2023-07-02 03:06:27.941248 spark_quality_rules_tools-0.3.8/PKG-INFO
--rw-rw-rw-   0        0        0     3242 2023-06-14 13:39:58.000000 spark_quality_rules_tools-0.3.8/README.md
--rw-rw-rw-   0        0        0      685 2023-07-01 22:58:24.000000 spark_quality_rules_tools-0.3.8/pyproject.toml
--rw-rw-rw-   0        0        0       86 2023-07-02 03:06:27.942248 spark_quality_rules_tools-0.3.8/setup.cfg
--rw-rw-rw-   0        0        0     1210 2023-07-02 03:05:51.000000 spark_quality_rules_tools-0.3.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-02 03:06:27.881235 spark_quality_rules_tools-0.3.8/spark_quality_rules_tools/
--rw-rw-rw-   0        0        0     2445 2023-07-02 02:49:16.000000 spark_quality_rules_tools-0.3.8/spark_quality_rules_tools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-02 03:06:27.903240 spark_quality_rules_tools-0.3.8/spark_quality_rules_tools/functions/
--rw-rw-rw-   0        0        0        0 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.3.8/spark_quality_rules_tools/functions/__init__.py
--rw-rw-rw-   0        0        0    49261 2023-07-02 03:05:51.000000 spark_quality_rules_tools-0.3.8/spark_quality_rules_tools/functions/generator.py
-drwxrwxrwx   0        0        0        0 2023-07-02 03:06:27.925245 spark_quality_rules_tools-0.3.8/spark_quality_rules_tools/utils/
--rw-rw-rw-   0        0        0       75 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.3.8/spark_quality_rules_tools/utils/__init__.py
--rw-rw-rw-   0        0        0      416 2023-04-12 03:25:49.000000 spark_quality_rules_tools-0.3.8/spark_quality_rules_tools/utils/color.py
--rw-rw-rw-   0        0        0     2138 2023-06-30 23:04:24.000000 spark_quality_rules_tools-0.3.8/spark_quality_rules_tools/utils/resolve.py
-drwxrwxrwx   0        0        0        0 2023-07-02 03:06:27.940249 spark_quality_rules_tools-0.3.8/spark_quality_rules_tools/utils/resource/
--rw-rw-rw-   0        0        0      532 2023-06-30 23:04:24.000000 spark_quality_rules_tools-0.3.8/spark_quality_rules_tools/utils/resource/resolve_edge.conf
--rw-rw-rw-   0        0        0      742 2023-06-30 23:04:24.000000 spark_quality_rules_tools-0.3.8/spark_quality_rules_tools/utils/resource/resolve_sandbox.conf
--rw-rw-rw-   0        0        0    25817 2023-07-02 01:22:13.000000 spark_quality_rules_tools-0.3.8/spark_quality_rules_tools/utils/resource/rules.json
--rw-rw-rw-   0        0        0     3742 2023-06-30 23:04:24.000000 spark_quality_rules_tools-0.3.8/spark_quality_rules_tools/utils/rules.py
-drwxrwxrwx   0        0        0        0 2023-07-02 03:06:27.902240 spark_quality_rules_tools-0.3.8/spark_quality_rules_tools.egg-info/
--rw-rw-rw-   0        0        0     4041 2023-07-02 03:06:27.000000 spark_quality_rules_tools-0.3.8/spark_quality_rules_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      784 2023-07-02 03:06:27.000000 spark_quality_rules_tools-0.3.8/spark_quality_rules_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-02 03:06:27.000000 spark_quality_rules_tools-0.3.8/spark_quality_rules_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      205 2023-07-02 03:06:27.000000 spark_quality_rules_tools-0.3.8/spark_quality_rules_tools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2023-07-02 03:06:27.000000 spark_quality_rules_tools-0.3.8/spark_quality_rules_tools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-02 03:08:49.596964 spark_quality_rules_tools-0.3.9/
+-rw-rw-rw-   0        0        0     1092 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.3.9/LICENSE
+-rw-rw-rw-   0        0        0       50 2023-06-14 13:33:57.000000 spark_quality_rules_tools-0.3.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     4041 2023-07-02 03:08:49.597964 spark_quality_rules_tools-0.3.9/PKG-INFO
+-rw-rw-rw-   0        0        0     3242 2023-06-14 13:39:58.000000 spark_quality_rules_tools-0.3.9/README.md
+-rw-rw-rw-   0        0        0      685 2023-07-01 22:58:24.000000 spark_quality_rules_tools-0.3.9/pyproject.toml
+-rw-rw-rw-   0        0        0       86 2023-07-02 03:08:49.598965 spark_quality_rules_tools-0.3.9/setup.cfg
+-rw-rw-rw-   0        0        0     1210 2023-07-02 03:08:37.000000 spark_quality_rules_tools-0.3.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-02 03:08:49.580961 spark_quality_rules_tools-0.3.9/spark_quality_rules_tools/
+-rw-rw-rw-   0        0        0     2550 2023-07-02 03:08:37.000000 spark_quality_rules_tools-0.3.9/spark_quality_rules_tools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-02 03:08:49.591962 spark_quality_rules_tools-0.3.9/spark_quality_rules_tools/functions/
+-rw-rw-rw-   0        0        0        0 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.3.9/spark_quality_rules_tools/functions/__init__.py
+-rw-rw-rw-   0        0        0    49261 2023-07-02 03:08:37.000000 spark_quality_rules_tools-0.3.9/spark_quality_rules_tools/functions/generator.py
+drwxrwxrwx   0        0        0        0 2023-07-02 03:08:49.594964 spark_quality_rules_tools-0.3.9/spark_quality_rules_tools/utils/
+-rw-rw-rw-   0        0        0       75 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.3.9/spark_quality_rules_tools/utils/__init__.py
+-rw-rw-rw-   0        0        0      416 2023-04-12 03:25:49.000000 spark_quality_rules_tools-0.3.9/spark_quality_rules_tools/utils/color.py
+-rw-rw-rw-   0        0        0     2138 2023-06-30 23:04:24.000000 spark_quality_rules_tools-0.3.9/spark_quality_rules_tools/utils/resolve.py
+drwxrwxrwx   0        0        0        0 2023-07-02 03:08:49.596964 spark_quality_rules_tools-0.3.9/spark_quality_rules_tools/utils/resource/
+-rw-rw-rw-   0        0        0      532 2023-06-30 23:04:24.000000 spark_quality_rules_tools-0.3.9/spark_quality_rules_tools/utils/resource/resolve_edge.conf
+-rw-rw-rw-   0        0        0      742 2023-06-30 23:04:24.000000 spark_quality_rules_tools-0.3.9/spark_quality_rules_tools/utils/resource/resolve_sandbox.conf
+-rw-rw-rw-   0        0        0    25817 2023-07-02 01:22:13.000000 spark_quality_rules_tools-0.3.9/spark_quality_rules_tools/utils/resource/rules.json
+-rw-rw-rw-   0        0        0     3742 2023-06-30 23:04:24.000000 spark_quality_rules_tools-0.3.9/spark_quality_rules_tools/utils/rules.py
+drwxrwxrwx   0        0        0        0 2023-07-02 03:08:49.590963 spark_quality_rules_tools-0.3.9/spark_quality_rules_tools.egg-info/
+-rw-rw-rw-   0        0        0     4041 2023-07-02 03:08:49.000000 spark_quality_rules_tools-0.3.9/spark_quality_rules_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      784 2023-07-02 03:08:49.000000 spark_quality_rules_tools-0.3.9/spark_quality_rules_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-02 03:08:49.000000 spark_quality_rules_tools-0.3.9/spark_quality_rules_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      205 2023-07-02 03:08:49.000000 spark_quality_rules_tools-0.3.9/spark_quality_rules_tools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2023-07-02 03:08:49.000000 spark_quality_rules_tools-0.3.9/spark_quality_rules_tools.egg-info/top_level.txt
```

### Comparing `spark_quality_rules_tools-0.3.8/LICENSE` & `spark_quality_rules_tools-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.3.8/PKG-INFO` & `spark_quality_rules_tools-0.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spark_quality_rules_tools
-Version: 0.3.8
+Version: 0.3.9
 Summary: spark_quality_rules_tools
 Home-page: https://github.com/jonaqp/spark_quality_rules_tools/
 Author: Jonathan Quiza
 Author-email: jony327@gmail.com
 License: UNKNOWN
 Download-URL: https://github.com/jonaqp/spark_quality_rules_tools/archive/main.zip
 Keywords: spark,dq,rules,hammurabies
```

### Comparing `spark_quality_rules_tools-0.3.8/README.md` & `spark_quality_rules_tools-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.3.8/pyproject.toml` & `spark_quality_rules_tools-0.3.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.3.8/setup.py` & `spark_quality_rules_tools-0.3.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from setuptools import find_packages
 
 setuppath = os.path.dirname(os.path.abspath(__file__))
 
 setup(
     name='spark_quality_rules_tools',
     packages=find_packages(),
-    version='0.3.8',
+    version='0.3.9',
     description='spark_quality_rules_tools',
     long_description=open(os.path.join(setuppath, 'README.md')).read(),
     long_description_content_type="text/markdown",
     author='Jonathan Quiza',
     author_email='jony327@gmail.com',
     url='https://github.com/jonaqp/spark_quality_rules_tools/',
     download_url='https://github.com/jonaqp/spark_quality_rules_tools/archive/main.zip',
```

### Comparing `spark_quality_rules_tools-0.3.8/spark_quality_rules_tools/__init__.py` & `spark_quality_rules_tools-0.3.9/spark_quality_rules_tools/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,26 +10,28 @@
 from spark_quality_rules_tools.functions.generator import dq_validate_artifactory
 from spark_quality_rules_tools.functions.generator import dq_validate_artifactory_with_rules
 from spark_quality_rules_tools.functions.generator import dq_validate_conf_artifactory
 from spark_quality_rules_tools.functions.generator import dq_validate_conf_file
 from spark_quality_rules_tools.functions.generator import dq_validate_file
 from spark_quality_rules_tools.functions.generator import dq_validate_file_with_rules
 from spark_quality_rules_tools.functions.generator import dq_get_rules_list
+from spark_quality_rules_tools.functions.generator import dq_generated_rules
 from spark_quality_rules_tools.utils import BASE_DIR
 from spark_quality_rules_tools.utils.color import get_color
 from spark_quality_rules_tools.utils.color import get_color_b
 from spark_quality_rules_tools.utils.resolve import get_replace_resolve_parameter
 from spark_quality_rules_tools.utils.rules import get_validate_rules
 
 generator_all = [
     "dq_creating_directory",
     "dq_spark_session",
     "dq_path_workspace",
     "dq_download_jar",
-    "dq_get_rules_list"
+    "dq_get_rules_list",
+    "dq_generated_rules"
 ]
 generator_artifactory = [
     "dq_validate_conf_artifactory",
     "dq_extract_parameters_artifactory",
     "dq_run_sandbox_artifactory",
     "dq_validate_rules_artifactory",
     "dq_validate_artifactory",
```

### Comparing `spark_quality_rules_tools-0.3.8/spark_quality_rules_tools/functions/generator.py` & `spark_quality_rules_tools-0.3.9/spark_quality_rules_tools/functions/generator.py`

 * *Files 0% similar despite different names*

```diff
@@ -958,15 +958,15 @@
     t.field_names = [get_color_b("DQ NAME"), get_color_b("VERSION"), get_color_b("DESCRIPTION")]
     for k, v in rules_config.items():
         for key_name, value_name in v.items():
             t.add_row([key_name, value_name[0].get("rules_version"), value_name[0].get("rules_name")])
         print(t)
 
 
-def dq_generate_rules_(rule_id=None,
+def dq_generated_rules(rule_id=None,
                        table_name=None):
     import os
     import sys
     import json
     from pyhocon import ConfigFactory
     from pyhocon.converter import HOCONConverter
     from pprint import pprint
```

### Comparing `spark_quality_rules_tools-0.3.8/spark_quality_rules_tools/utils/resolve.py` & `spark_quality_rules_tools-0.3.9/spark_quality_rules_tools/utils/resolve.py`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.3.8/spark_quality_rules_tools/utils/resource/resolve_edge.conf` & `spark_quality_rules_tools-0.3.9/spark_quality_rules_tools/utils/resource/resolve_edge.conf`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.3.8/spark_quality_rules_tools/utils/resource/resolve_sandbox.conf` & `spark_quality_rules_tools-0.3.9/spark_quality_rules_tools/utils/resource/resolve_sandbox.conf`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.3.8/spark_quality_rules_tools/utils/resource/rules.json` & `spark_quality_rules_tools-0.3.9/spark_quality_rules_tools/utils/resource/rules.json`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.3.8/spark_quality_rules_tools/utils/rules.py` & `spark_quality_rules_tools-0.3.9/spark_quality_rules_tools/utils/rules.py`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.3.8/spark_quality_rules_tools.egg-info/PKG-INFO` & `spark_quality_rules_tools-0.3.9/spark_quality_rules_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spark-quality-rules-tools
-Version: 0.3.8
+Version: 0.3.9
 Summary: spark_quality_rules_tools
 Home-page: https://github.com/jonaqp/spark_quality_rules_tools/
 Author: Jonathan Quiza
 Author-email: jony327@gmail.com
 License: UNKNOWN
 Download-URL: https://github.com/jonaqp/spark_quality_rules_tools/archive/main.zip
 Keywords: spark,dq,rules,hammurabies
```

### Comparing `spark_quality_rules_tools-0.3.8/spark_quality_rules_tools.egg-info/SOURCES.txt` & `spark_quality_rules_tools-0.3.9/spark_quality_rules_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

