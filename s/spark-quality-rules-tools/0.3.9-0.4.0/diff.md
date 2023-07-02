# Comparing `tmp/spark_quality_rules_tools-0.3.9.tar.gz` & `tmp/spark_quality_rules_tools-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spark_quality_rules_tools-0.3.9.tar", last modified: Sun Jul  2 03:08:49 2023, max compression
+gzip compressed data, was "spark_quality_rules_tools-0.4.0.tar", last modified: Sun Jul  2 03:11:43 2023, max compression
```

## Comparing `spark_quality_rules_tools-0.3.9.tar` & `spark_quality_rules_tools-0.4.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-07-02 03:08:49.596964 spark_quality_rules_tools-0.3.9/
--rw-rw-rw-   0        0        0     1092 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.3.9/LICENSE
--rw-rw-rw-   0        0        0       50 2023-06-14 13:33:57.000000 spark_quality_rules_tools-0.3.9/MANIFEST.in
--rw-rw-rw-   0        0        0     4041 2023-07-02 03:08:49.597964 spark_quality_rules_tools-0.3.9/PKG-INFO
--rw-rw-rw-   0        0        0     3242 2023-06-14 13:39:58.000000 spark_quality_rules_tools-0.3.9/README.md
--rw-rw-rw-   0        0        0      685 2023-07-01 22:58:24.000000 spark_quality_rules_tools-0.3.9/pyproject.toml
--rw-rw-rw-   0        0        0       86 2023-07-02 03:08:49.598965 spark_quality_rules_tools-0.3.9/setup.cfg
--rw-rw-rw-   0        0        0     1210 2023-07-02 03:08:37.000000 spark_quality_rules_tools-0.3.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-02 03:08:49.580961 spark_quality_rules_tools-0.3.9/spark_quality_rules_tools/
--rw-rw-rw-   0        0        0     2550 2023-07-02 03:08:37.000000 spark_quality_rules_tools-0.3.9/spark_quality_rules_tools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-02 03:08:49.591962 spark_quality_rules_tools-0.3.9/spark_quality_rules_tools/functions/
--rw-rw-rw-   0        0        0        0 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.3.9/spark_quality_rules_tools/functions/__init__.py
--rw-rw-rw-   0        0        0    49261 2023-07-02 03:08:37.000000 spark_quality_rules_tools-0.3.9/spark_quality_rules_tools/functions/generator.py
-drwxrwxrwx   0        0        0        0 2023-07-02 03:08:49.594964 spark_quality_rules_tools-0.3.9/spark_quality_rules_tools/utils/
--rw-rw-rw-   0        0        0       75 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.3.9/spark_quality_rules_tools/utils/__init__.py
--rw-rw-rw-   0        0        0      416 2023-04-12 03:25:49.000000 spark_quality_rules_tools-0.3.9/spark_quality_rules_tools/utils/color.py
--rw-rw-rw-   0        0        0     2138 2023-06-30 23:04:24.000000 spark_quality_rules_tools-0.3.9/spark_quality_rules_tools/utils/resolve.py
-drwxrwxrwx   0        0        0        0 2023-07-02 03:08:49.596964 spark_quality_rules_tools-0.3.9/spark_quality_rules_tools/utils/resource/
--rw-rw-rw-   0        0        0      532 2023-06-30 23:04:24.000000 spark_quality_rules_tools-0.3.9/spark_quality_rules_tools/utils/resource/resolve_edge.conf
--rw-rw-rw-   0        0        0      742 2023-06-30 23:04:24.000000 spark_quality_rules_tools-0.3.9/spark_quality_rules_tools/utils/resource/resolve_sandbox.conf
--rw-rw-rw-   0        0        0    25817 2023-07-02 01:22:13.000000 spark_quality_rules_tools-0.3.9/spark_quality_rules_tools/utils/resource/rules.json
--rw-rw-rw-   0        0        0     3742 2023-06-30 23:04:24.000000 spark_quality_rules_tools-0.3.9/spark_quality_rules_tools/utils/rules.py
-drwxrwxrwx   0        0        0        0 2023-07-02 03:08:49.590963 spark_quality_rules_tools-0.3.9/spark_quality_rules_tools.egg-info/
--rw-rw-rw-   0        0        0     4041 2023-07-02 03:08:49.000000 spark_quality_rules_tools-0.3.9/spark_quality_rules_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      784 2023-07-02 03:08:49.000000 spark_quality_rules_tools-0.3.9/spark_quality_rules_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-02 03:08:49.000000 spark_quality_rules_tools-0.3.9/spark_quality_rules_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      205 2023-07-02 03:08:49.000000 spark_quality_rules_tools-0.3.9/spark_quality_rules_tools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2023-07-02 03:08:49.000000 spark_quality_rules_tools-0.3.9/spark_quality_rules_tools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-02 03:11:43.858638 spark_quality_rules_tools-0.4.0/
+-rw-rw-rw-   0        0        0     1092 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.4.0/LICENSE
+-rw-rw-rw-   0        0        0       50 2023-06-14 13:33:57.000000 spark_quality_rules_tools-0.4.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     4041 2023-07-02 03:11:43.858638 spark_quality_rules_tools-0.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3242 2023-06-14 13:39:58.000000 spark_quality_rules_tools-0.4.0/README.md
+-rw-rw-rw-   0        0        0      685 2023-07-01 22:58:24.000000 spark_quality_rules_tools-0.4.0/pyproject.toml
+-rw-rw-rw-   0        0        0       86 2023-07-02 03:11:43.859639 spark_quality_rules_tools-0.4.0/setup.cfg
+-rw-rw-rw-   0        0        0     1210 2023-07-02 03:11:34.000000 spark_quality_rules_tools-0.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-02 03:11:43.840633 spark_quality_rules_tools-0.4.0/spark_quality_rules_tools/
+-rw-rw-rw-   0        0        0     2550 2023-07-02 03:08:37.000000 spark_quality_rules_tools-0.4.0/spark_quality_rules_tools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-02 03:11:43.853637 spark_quality_rules_tools-0.4.0/spark_quality_rules_tools/functions/
+-rw-rw-rw-   0        0        0        0 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.4.0/spark_quality_rules_tools/functions/__init__.py
+-rw-rw-rw-   0        0        0    49277 2023-07-02 03:11:34.000000 spark_quality_rules_tools-0.4.0/spark_quality_rules_tools/functions/generator.py
+drwxrwxrwx   0        0        0        0 2023-07-02 03:11:43.856638 spark_quality_rules_tools-0.4.0/spark_quality_rules_tools/utils/
+-rw-rw-rw-   0        0        0       75 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.4.0/spark_quality_rules_tools/utils/__init__.py
+-rw-rw-rw-   0        0        0      416 2023-04-12 03:25:49.000000 spark_quality_rules_tools-0.4.0/spark_quality_rules_tools/utils/color.py
+-rw-rw-rw-   0        0        0     2138 2023-06-30 23:04:24.000000 spark_quality_rules_tools-0.4.0/spark_quality_rules_tools/utils/resolve.py
+drwxrwxrwx   0        0        0        0 2023-07-02 03:11:43.858638 spark_quality_rules_tools-0.4.0/spark_quality_rules_tools/utils/resource/
+-rw-rw-rw-   0        0        0      532 2023-06-30 23:04:24.000000 spark_quality_rules_tools-0.4.0/spark_quality_rules_tools/utils/resource/resolve_edge.conf
+-rw-rw-rw-   0        0        0      742 2023-06-30 23:04:24.000000 spark_quality_rules_tools-0.4.0/spark_quality_rules_tools/utils/resource/resolve_sandbox.conf
+-rw-rw-rw-   0        0        0    25817 2023-07-02 01:22:13.000000 spark_quality_rules_tools-0.4.0/spark_quality_rules_tools/utils/resource/rules.json
+-rw-rw-rw-   0        0        0     3742 2023-06-30 23:04:24.000000 spark_quality_rules_tools-0.4.0/spark_quality_rules_tools/utils/rules.py
+drwxrwxrwx   0        0        0        0 2023-07-02 03:11:43.851636 spark_quality_rules_tools-0.4.0/spark_quality_rules_tools.egg-info/
+-rw-rw-rw-   0        0        0     4041 2023-07-02 03:11:43.000000 spark_quality_rules_tools-0.4.0/spark_quality_rules_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      784 2023-07-02 03:11:43.000000 spark_quality_rules_tools-0.4.0/spark_quality_rules_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-02 03:11:43.000000 spark_quality_rules_tools-0.4.0/spark_quality_rules_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      205 2023-07-02 03:11:43.000000 spark_quality_rules_tools-0.4.0/spark_quality_rules_tools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2023-07-02 03:11:43.000000 spark_quality_rules_tools-0.4.0/spark_quality_rules_tools.egg-info/top_level.txt
```

### Comparing `spark_quality_rules_tools-0.3.9/LICENSE` & `spark_quality_rules_tools-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.3.9/PKG-INFO` & `spark_quality_rules_tools-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spark_quality_rules_tools
-Version: 0.3.9
+Version: 0.4.0
 Summary: spark_quality_rules_tools
 Home-page: https://github.com/jonaqp/spark_quality_rules_tools/
 Author: Jonathan Quiza
 Author-email: jony327@gmail.com
 License: UNKNOWN
 Download-URL: https://github.com/jonaqp/spark_quality_rules_tools/archive/main.zip
 Keywords: spark,dq,rules,hammurabies
```

### Comparing `spark_quality_rules_tools-0.3.9/README.md` & `spark_quality_rules_tools-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.3.9/pyproject.toml` & `spark_quality_rules_tools-0.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.3.9/setup.py` & `spark_quality_rules_tools-0.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from setuptools import find_packages
 
 setuppath = os.path.dirname(os.path.abspath(__file__))
 
 setup(
     name='spark_quality_rules_tools',
     packages=find_packages(),
-    version='0.3.9',
+    version='0.4.0',
     description='spark_quality_rules_tools',
     long_description=open(os.path.join(setuppath, 'README.md')).read(),
     long_description_content_type="text/markdown",
     author='Jonathan Quiza',
     author_email='jony327@gmail.com',
     url='https://github.com/jonaqp/spark_quality_rules_tools/',
     download_url='https://github.com/jonaqp/spark_quality_rules_tools/archive/main.zip',
```

### Comparing `spark_quality_rules_tools-0.3.9/spark_quality_rules_tools/__init__.py` & `spark_quality_rules_tools-0.4.0/spark_quality_rules_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.3.9/spark_quality_rules_tools/functions/generator.py` & `spark_quality_rules_tools-0.4.0/spark_quality_rules_tools/functions/generator.py`

 * *Files 0% similar despite different names*

```diff
@@ -963,14 +963,15 @@
 
 
 def dq_generated_rules(rule_id=None,
                        table_name=None):
     import os
     import sys
     import json
+    import ast
     from pyhocon import ConfigFactory
     from pyhocon.converter import HOCONConverter
     from pprint import pprint
     from spark_quality_rules_tools.utils.color import get_color_b, get_color
     from spark_quality_rules_tools.utils import BASE_DIR
 
     is_windows = sys.platform.startswith('win')
```

### Comparing `spark_quality_rules_tools-0.3.9/spark_quality_rules_tools/utils/resolve.py` & `spark_quality_rules_tools-0.4.0/spark_quality_rules_tools/utils/resolve.py`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.3.9/spark_quality_rules_tools/utils/resource/resolve_edge.conf` & `spark_quality_rules_tools-0.4.0/spark_quality_rules_tools/utils/resource/resolve_edge.conf`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.3.9/spark_quality_rules_tools/utils/resource/resolve_sandbox.conf` & `spark_quality_rules_tools-0.4.0/spark_quality_rules_tools/utils/resource/resolve_sandbox.conf`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.3.9/spark_quality_rules_tools/utils/resource/rules.json` & `spark_quality_rules_tools-0.4.0/spark_quality_rules_tools/utils/resource/rules.json`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.3.9/spark_quality_rules_tools/utils/rules.py` & `spark_quality_rules_tools-0.4.0/spark_quality_rules_tools/utils/rules.py`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.3.9/spark_quality_rules_tools.egg-info/PKG-INFO` & `spark_quality_rules_tools-0.4.0/spark_quality_rules_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spark-quality-rules-tools
-Version: 0.3.9
+Version: 0.4.0
 Summary: spark_quality_rules_tools
 Home-page: https://github.com/jonaqp/spark_quality_rules_tools/
 Author: Jonathan Quiza
 Author-email: jony327@gmail.com
 License: UNKNOWN
 Download-URL: https://github.com/jonaqp/spark_quality_rules_tools/archive/main.zip
 Keywords: spark,dq,rules,hammurabies
```

### Comparing `spark_quality_rules_tools-0.3.9/spark_quality_rules_tools.egg-info/SOURCES.txt` & `spark_quality_rules_tools-0.4.0/spark_quality_rules_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

