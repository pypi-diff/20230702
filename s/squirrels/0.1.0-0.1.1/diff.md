# Comparing `tmp/squirrels-0.1.0.tar.gz` & `tmp/squirrels-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "squirrels-0.1.0.tar", last modified: Sun Jun 11 17:47:35 2023, max compression
+gzip compressed data, was "squirrels-0.1.1.tar", last modified: Sun Jul  2 18:47:13 2023, max compression
```

## Comparing `squirrels-0.1.0.tar` & `squirrels-0.1.1.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxrwxrwx   0        0        0        0 2023-06-11 17:47:35.319227 squirrels-0.1.0/
--rw-rw-rw-   0        0        0     1088 2023-04-24 03:56:44.000000 squirrels-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     1959 2023-06-11 17:47:35.317227 squirrels-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1705 2023-05-19 13:23:55.000000 squirrels-0.1.0/README.md
--rw-rw-rw-   0        0        0       42 2023-06-11 17:47:35.320229 squirrels-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1407 2023-06-11 17:43:54.000000 squirrels-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-11 17:47:35.180132 squirrels-0.1.0/squirrels/
--rw-rw-rw-   0        0        0      822 2023-06-11 15:20:47.000000 squirrels-0.1.0/squirrels/__init__.py
--rw-rw-rw-   0        0        0     6455 2023-06-11 15:20:47.000000 squirrels-0.1.0/squirrels/_api_server.py
--rw-rw-rw-   0        0        0     5978 2023-06-11 15:20:47.000000 squirrels-0.1.0/squirrels/_command_line.py
--rw-rw-rw-   0        0        0     1901 2023-06-11 15:20:47.000000 squirrels-0.1.0/squirrels/_constants.py
--rw-rw-rw-   0        0        0     3063 2023-05-19 13:23:55.000000 squirrels-0.1.0/squirrels/_credentials_manager.py
--rw-rw-rw-   0        0        0     4839 2023-05-19 13:23:55.000000 squirrels-0.1.0/squirrels/_initializer.py
--rw-rw-rw-   0        0        0     8292 2023-06-11 15:20:47.000000 squirrels-0.1.0/squirrels/_manifest.py
--rw-rw-rw-   0        0        0     1257 2023-05-19 13:23:55.000000 squirrels-0.1.0/squirrels/_module_loader.py
--rw-rw-rw-   0        0        0     6176 2023-06-11 15:20:47.000000 squirrels-0.1.0/squirrels/_parameter_set.py
--rw-rw-rw-   0        0        0    14484 2023-06-11 15:20:47.000000 squirrels-0.1.0/squirrels/_renderer.py
--rw-rw-rw-   0        0        0     1179 2023-05-19 13:23:55.000000 squirrels-0.1.0/squirrels/_timed_imports.py
--rw-rw-rw-   0        0        0     4170 2023-05-19 13:23:55.000000 squirrels-0.1.0/squirrels/_utils.py
--rw-rw-rw-   0        0        0       95 2023-05-19 13:23:55.000000 squirrels-0.1.0/squirrels/_version.py
--rw-rw-rw-   0        0        0     4382 2023-06-11 15:20:47.000000 squirrels-0.1.0/squirrels/connection_set.py
--rw-rw-rw-   0        0        0    12943 2023-05-19 13:23:55.000000 squirrels-0.1.0/squirrels/data_sources.py
--rw-rw-rw-   0        0        0    13433 2023-06-11 17:43:41.000000 squirrels-0.1.0/squirrels/dateutils.py
-drwxrwxrwx   0        0        0        0 2023-06-11 17:47:35.111131 squirrels-0.1.0/squirrels/package_data/
-drwxrwxrwx   0        0        0        0 2023-06-11 17:47:35.223680 squirrels-0.1.0/squirrels/package_data/base_project/
--rw-rw-rw-   0        0        0       40 2023-05-05 13:52:42.000000 squirrels-0.1.0/squirrels/package_data/base_project/.gitignore
--rw-rw-rw-   0        0        0      923 2023-05-30 22:48:25.000000 squirrels-0.1.0/squirrels/package_data/base_project/connections.py
-drwxrwxrwx   0        0        0        0 2023-06-11 17:47:35.231687 squirrels-0.1.0/squirrels/package_data/base_project/database/
--rw-rw-rw-   0        0        0     8192 2023-04-23 00:05:57.000000 squirrels-0.1.0/squirrels/package_data/base_project/database/sample_database.db
--rw-rw-rw-   0        0        0   188416 2023-03-18 14:11:28.000000 squirrels-0.1.0/squirrels/package_data/base_project/database/seattle_weather.db
-drwxrwxrwx   0        0        0        0 2023-06-11 17:47:35.108136 squirrels-0.1.0/squirrels/package_data/base_project/datasets/
-drwxrwxrwx   0        0        0        0 2023-06-11 17:47:35.293707 squirrels-0.1.0/squirrels/package_data/base_project/datasets/sample_dataset/
--rw-rw-rw-   0        0        0      306 2023-06-11 15:20:47.000000 squirrels-0.1.0/squirrels/package_data/base_project/datasets/sample_dataset/context.py
--rw-rw-rw-   0        0        0      929 2023-06-11 15:20:47.000000 squirrels-0.1.0/squirrels/package_data/base_project/datasets/sample_dataset/database_view1.py
--rw-rw-rw-   0        0        0      376 2023-05-09 13:28:24.000000 squirrels-0.1.0/squirrels/package_data/base_project/datasets/sample_dataset/database_view1.sql.j2
--rw-rw-rw-   0        0        0      320 2023-06-11 15:20:47.000000 squirrels-0.1.0/squirrels/package_data/base_project/datasets/sample_dataset/final_view.py
--rw-rw-rw-   0        0        0       31 2023-03-20 06:10:47.000000 squirrels-0.1.0/squirrels/package_data/base_project/datasets/sample_dataset/final_view.sql.j2
--rw-rw-rw-   0        0        0     1429 2023-06-11 15:20:47.000000 squirrels-0.1.0/squirrels/package_data/base_project/datasets/sample_dataset/parameters.py
--rw-rw-rw-   0        0        0      148 2023-06-11 15:20:47.000000 squirrels-0.1.0/squirrels/package_data/base_project/datasets/sample_dataset/selections.cfg
--rw-rw-rw-   0        0        0      728 2023-05-09 13:28:24.000000 squirrels-0.1.0/squirrels/package_data/base_project/squirrels.yaml
-drwxrwxrwx   0        0        0        0 2023-06-11 17:47:35.303696 squirrels-0.1.0/squirrels/package_data/static/
--rw-rw-rw-   0        0        0     4638 2023-03-12 05:51:40.000000 squirrels-0.1.0/squirrels/package_data/static/favicon.ico
--rw-rw-rw-   0        0        0     9179 2023-05-19 13:23:55.000000 squirrels-0.1.0/squirrels/package_data/static/script.js
--rw-rw-rw-   0        0        0     1841 2023-03-12 03:03:14.000000 squirrels-0.1.0/squirrels/package_data/static/style.css
-drwxrwxrwx   0        0        0        0 2023-06-11 17:47:35.314225 squirrels-0.1.0/squirrels/package_data/templates/
--rw-rw-rw-   0        0        0     1276 2023-06-11 15:20:47.000000 squirrels-0.1.0/squirrels/package_data/templates/index.html
--rw-rw-rw-   0        0        0     8281 2023-06-10 21:13:17.000000 squirrels-0.1.0/squirrels/parameter_options.py
--rw-rw-rw-   0        0        0    32879 2023-06-11 17:43:41.000000 squirrels-0.1.0/squirrels/parameters.py
-drwxrwxrwx   0        0        0        0 2023-06-11 17:47:35.214681 squirrels-0.1.0/squirrels.egg-info/
--rw-rw-rw-   0        0        0     1959 2023-06-11 17:47:35.000000 squirrels-0.1.0/squirrels.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1663 2023-06-11 17:47:35.000000 squirrels-0.1.0/squirrels.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-11 17:47:35.000000 squirrels-0.1.0/squirrels.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-06-11 17:47:35.000000 squirrels-0.1.0/squirrels.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       95 2023-06-11 17:47:35.000000 squirrels-0.1.0/squirrels.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-11 17:47:35.000000 squirrels-0.1.0/squirrels.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-02 18:47:13.533400 squirrels-0.1.1/
+-rw-rw-rw-   0        0        0     1088 2023-06-12 00:22:33.000000 squirrels-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     1957 2023-07-02 18:47:13.525877 squirrels-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1705 2023-06-12 01:43:58.000000 squirrels-0.1.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-02 18:47:13.534401 squirrels-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1405 2023-07-02 18:46:44.000000 squirrels-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-02 18:47:13.354318 squirrels-0.1.1/squirrels/
+-rw-rw-rw-   0        0        0      822 2023-06-12 22:56:49.000000 squirrels-0.1.1/squirrels/__init__.py
+-rw-rw-rw-   0        0        0     6455 2023-06-12 01:43:58.000000 squirrels-0.1.1/squirrels/_api_server.py
+-rw-rw-rw-   0        0        0     5978 2023-06-12 01:43:58.000000 squirrels-0.1.1/squirrels/_command_line.py
+-rw-rw-rw-   0        0        0     1901 2023-06-12 01:43:58.000000 squirrels-0.1.1/squirrels/_constants.py
+-rw-rw-rw-   0        0        0     3063 2023-06-12 01:43:58.000000 squirrels-0.1.1/squirrels/_credentials_manager.py
+-rw-rw-rw-   0        0        0     4839 2023-06-12 01:43:58.000000 squirrels-0.1.1/squirrels/_initializer.py
+-rw-rw-rw-   0        0        0     8292 2023-06-12 01:43:58.000000 squirrels-0.1.1/squirrels/_manifest.py
+-rw-rw-rw-   0        0        0     1257 2023-06-12 01:43:58.000000 squirrels-0.1.1/squirrels/_module_loader.py
+-rw-rw-rw-   0        0        0     6176 2023-06-12 01:43:58.000000 squirrels-0.1.1/squirrels/_parameter_set.py
+-rw-rw-rw-   0        0        0    14484 2023-06-12 01:43:58.000000 squirrels-0.1.1/squirrels/_renderer.py
+-rw-rw-rw-   0        0        0     1179 2023-06-12 01:43:58.000000 squirrels-0.1.1/squirrels/_timed_imports.py
+-rw-rw-rw-   0        0        0     4170 2023-06-12 01:43:58.000000 squirrels-0.1.1/squirrels/_utils.py
+-rw-rw-rw-   0        0        0       95 2023-06-24 02:23:18.000000 squirrels-0.1.1/squirrels/_version.py
+-rw-rw-rw-   0        0        0     4382 2023-06-12 22:53:05.000000 squirrels-0.1.1/squirrels/connection_set.py
+-rw-rw-rw-   0        0        0    13401 2023-07-01 14:51:17.000000 squirrels-0.1.1/squirrels/data_sources.py
+-rw-rw-rw-   0        0        0    15823 2023-06-24 02:01:01.000000 squirrels-0.1.1/squirrels/dateutils.py
+drwxrwxrwx   0        0        0        0 2023-07-02 18:47:13.181248 squirrels-0.1.1/squirrels/package_data/
+drwxrwxrwx   0        0        0        0 2023-07-02 18:47:13.437862 squirrels-0.1.1/squirrels/package_data/base_project/
+-rw-rw-rw-   0        0        0       40 2023-06-12 01:43:54.000000 squirrels-0.1.1/squirrels/package_data/base_project/.gitignore
+-rw-rw-rw-   0        0        0      917 2023-06-29 12:35:33.000000 squirrels-0.1.1/squirrels/package_data/base_project/connections.py
+drwxrwxrwx   0        0        0        0 2023-07-02 18:47:13.450863 squirrels-0.1.1/squirrels/package_data/base_project/database/
+-rw-rw-rw-   0        0        0    32768 2023-06-29 13:24:06.000000 squirrels-0.1.1/squirrels/package_data/base_project/database/sample_database.db
+-rw-rw-rw-   0        0        0   188416 2023-06-12 01:43:54.000000 squirrels-0.1.1/squirrels/package_data/base_project/database/seattle_weather.db
+drwxrwxrwx   0        0        0        0 2023-07-02 18:47:13.172234 squirrels-0.1.1/squirrels/package_data/base_project/datasets/
+drwxrwxrwx   0        0        0        0 2023-07-02 18:47:13.503862 squirrels-0.1.1/squirrels/package_data/base_project/datasets/sample_dataset/
+-rw-rw-rw-   0        0        0     1106 2023-06-30 01:06:41.000000 squirrels-0.1.1/squirrels/package_data/base_project/datasets/sample_dataset/context.py
+-rw-rw-rw-   0        0        0      934 2023-06-30 02:53:44.000000 squirrels-0.1.1/squirrels/package_data/base_project/datasets/sample_dataset/database_view1.py
+-rw-rw-rw-   0        0        0      930 2023-06-30 02:01:44.000000 squirrels-0.1.1/squirrels/package_data/base_project/datasets/sample_dataset/database_view1.sql.j2
+-rw-rw-rw-   0        0        0      411 2023-06-30 02:49:03.000000 squirrels-0.1.1/squirrels/package_data/base_project/datasets/sample_dataset/final_view.py
+-rw-rw-rw-   0        0        0      116 2023-06-30 01:09:05.000000 squirrels-0.1.1/squirrels/package_data/base_project/datasets/sample_dataset/final_view.sql.j2
+-rw-rw-rw-   0        0        0     2518 2023-06-29 13:45:06.000000 squirrels-0.1.1/squirrels/package_data/base_project/datasets/sample_dataset/parameters.py
+-rw-rw-rw-   0        0        0      189 2023-06-30 02:18:44.000000 squirrels-0.1.1/squirrels/package_data/base_project/datasets/sample_dataset/selections.cfg
+-rw-rw-rw-   0        0        0      449 2023-06-30 03:03:29.000000 squirrels-0.1.1/squirrels/package_data/base_project/squirrels.yaml
+drwxrwxrwx   0        0        0        0 2023-07-02 18:47:13.514875 squirrels-0.1.1/squirrels/package_data/static/
+-rw-rw-rw-   0        0        0     4638 2023-06-12 01:43:54.000000 squirrels-0.1.1/squirrels/package_data/static/favicon.ico
+-rw-rw-rw-   0        0        0     9179 2023-06-12 01:43:58.000000 squirrels-0.1.1/squirrels/package_data/static/script.js
+-rw-rw-rw-   0        0        0     1841 2023-06-12 01:43:54.000000 squirrels-0.1.1/squirrels/package_data/static/style.css
+drwxrwxrwx   0        0        0        0 2023-07-02 18:47:13.519876 squirrels-0.1.1/squirrels/package_data/templates/
+-rw-rw-rw-   0        0        0     1276 2023-06-12 01:43:58.000000 squirrels-0.1.1/squirrels/package_data/templates/index.html
+-rw-rw-rw-   0        0        0    10155 2023-06-27 11:50:39.000000 squirrels-0.1.1/squirrels/parameter_options.py
+-rw-rw-rw-   0        0        0    34977 2023-06-27 11:46:44.000000 squirrels-0.1.1/squirrels/parameters.py
+drwxrwxrwx   0        0        0        0 2023-07-02 18:47:13.426337 squirrels-0.1.1/squirrels.egg-info/
+-rw-rw-rw-   0        0        0     1957 2023-07-02 18:47:13.000000 squirrels-0.1.1/squirrels.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1663 2023-07-02 18:47:13.000000 squirrels-0.1.1/squirrels.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-02 18:47:13.000000 squirrels-0.1.1/squirrels.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-07-02 18:47:13.000000 squirrels-0.1.1/squirrels.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       95 2023-07-02 18:47:13.000000 squirrels-0.1.1/squirrels.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-02 18:47:13.000000 squirrels-0.1.1/squirrels.egg-info/top_level.txt
```

### Comparing `squirrels-0.1.0/LICENSE` & `squirrels-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `squirrels-0.1.0/PKG-INFO` & `squirrels-0.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: squirrels
-Version: 0.1.0
-Summary: Python Package for Configuring SQL Generating APIs
+Version: 0.1.1
+Summary: Squirrels - Configure REST APIs for BI Analytics
 Author: Tim Huang
 Author-email: tim.yuting@hotmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Squirrels
```

### Comparing `squirrels-0.1.0/README.md` & `squirrels-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `squirrels-0.1.0/setup.py` & `squirrels-0.1.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,17 +16,17 @@
             paths.append(os.path.join('..', path, filename))
     return paths
 
 extra_files = package_files(os.path.join('squirrels', 'package_data'))
 
 setup(
     name='squirrels',
-    version='0.1.0',
+    version='0.1.1',
     packages=find_packages(),
-    description='Python Package for Configuring SQL Generating APIs',
+    description='Squirrels - Configure REST APIs for BI Analytics',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='Tim Huang',
     author_email='tim.yuting@hotmail.com',
     license='MIT',
     install_requires=[
         'openpyxl', 'inquirer', 'pwinput', 'cachetools', 'fastapi', 'uvicorn',
```

### Comparing `squirrels-0.1.0/squirrels/__init__.py` & `squirrels-0.1.1/squirrels/__init__.py`

 * *Files identical despite different names*

### Comparing `squirrels-0.1.0/squirrels/_api_server.py` & `squirrels-0.1.1/squirrels/_api_server.py`

 * *Files identical despite different names*

### Comparing `squirrels-0.1.0/squirrels/_command_line.py` & `squirrels-0.1.1/squirrels/_command_line.py`

 * *Files identical despite different names*

### Comparing `squirrels-0.1.0/squirrels/_constants.py` & `squirrels-0.1.1/squirrels/_constants.py`

 * *Files identical despite different names*

### Comparing `squirrels-0.1.0/squirrels/_credentials_manager.py` & `squirrels-0.1.1/squirrels/_credentials_manager.py`

 * *Files identical despite different names*

### Comparing `squirrels-0.1.0/squirrels/_initializer.py` & `squirrels-0.1.1/squirrels/_initializer.py`

 * *Files identical despite different names*

### Comparing `squirrels-0.1.0/squirrels/_manifest.py` & `squirrels-0.1.1/squirrels/_manifest.py`

 * *Files identical despite different names*

### Comparing `squirrels-0.1.0/squirrels/_module_loader.py` & `squirrels-0.1.1/squirrels/_module_loader.py`

 * *Files identical despite different names*

### Comparing `squirrels-0.1.0/squirrels/_parameter_set.py` & `squirrels-0.1.1/squirrels/_parameter_set.py`

 * *Files identical despite different names*

### Comparing `squirrels-0.1.0/squirrels/_renderer.py` & `squirrels-0.1.1/squirrels/_renderer.py`

 * *Files identical despite different names*

### Comparing `squirrels-0.1.0/squirrels/_timed_imports.py` & `squirrels-0.1.1/squirrels/_timed_imports.py`

 * *Files identical despite different names*

### Comparing `squirrels-0.1.0/squirrels/_utils.py` & `squirrels-0.1.1/squirrels/_utils.py`

 * *Files identical despite different names*

### Comparing `squirrels-0.1.0/squirrels/connection_set.py` & `squirrels-0.1.1/squirrels/connection_set.py`

 * *Files identical despite different names*

### Comparing `squirrels-0.1.0/squirrels/data_sources.py` & `squirrels-0.1.1/squirrels/data_sources.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
-from typing import Type, Tuple, List, Optional
-from dataclasses import dataclass
+from typing import Type, Dict, Tuple, List, Optional
+from dataclasses import dataclass, field
 
 from squirrels import parameters as p, parameter_options as po
 from squirrels._timed_imports import pandas as pd
 from squirrels import _constants as c, _utils
 
 
 @dataclass
@@ -23,15 +23,15 @@
     def get_query(self) -> str:
         """
         Get the "table_or_query" attribute as a select query
 
         Returns:
             str: The converted select query
         """
-        if self.table_or_query.lower().startswith('select '):
+        if self.table_or_query.strip().lower().startswith('select '):
             query = self.table_or_query
         else:
             query = f'SELECT * FROM {self.table_or_query}'
         return query
     
     def convert(self, ds_param: p.DataSourceParameter, df: pd.DataFrame) -> p.Parameter:
         """
@@ -58,27 +58,29 @@
 
 @dataclass
 class SelectionDataSource(DataSource):
     """
     Lookup table for selection parameters (single and multi)
 
     Attributes:
-        connection_name: Name of the connection to use defined in connections.py
         table_or_query: Either the name of the table to use, or a query to run
         id_col: The column name of the id
         options_col: The column name of the options
         order_by_col: The column name to order the options by. Orders by the id_col instead if this is None
         is_default_col: The column name that indicates which options are the default
         parent_id_col: The column name of the parent option id that this option belongs to
+        custom_cols: Dictionary of attribute to column name for custom fields for the SelectParameterOption
+        connection_name: Name of the connection to use defined in connections.py
     """
     id_col: str
     options_col: str
     order_by_col: Optional[str] = None
     is_default_col: Optional[str] = None
     parent_id_col: Optional[str] = None
+    custom_cols: Dict[str, str] = field(default_factory=dict)
     connection_name: str = c.DEFAULT_DB_CONN
 
     def __post_init__(self):
         self.order_by_col = self.order_by_col if self.order_by_col is not None else self.id_col
 
     def convert(self, ds_param: p.DataSourceParameter, df: pd.DataFrame) -> p.Parameter:
         """
@@ -92,39 +94,45 @@
             The converted parameter
         """
         self._validate_parameter_class(ds_param, [p.SingleSelectParameter, p.MultiSelectParameter])
 
         def is_default(row):
             return int(_utils.get_row_value(row, self.is_default_col)) == 1 if self.is_default_col is not None else False
         
+        def get_custom_fields(row):
+            result = {}
+            for key, val in self.custom_cols.items():
+                result[key] = _utils.get_row_value(row, val)
+            return result
+        
         try:
             df.sort_values(self.order_by_col, inplace=True)
         except KeyError as e:
             raise _utils.ConfigurationError(f'Could not sort on column name "{self.order_by_col}" as it does not exist')
         
         options = tuple(
-            po.SelectParameterOption(str(_utils.get_row_value(row, self.id_col)), str(_utils.get_row_value(row, self.options_col)), is_default(row), 
-                                     parent_option_id=self._get_parent(row))
+            po.SelectParameterOption(str(_utils.get_row_value(row, self.id_col)), str(_utils.get_row_value(row, self.options_col)), 
+                                     is_default=is_default(row), parent_option_id=self._get_parent(row), custom_fields=get_custom_fields(row))
             for _, row in df.iterrows()
         )
         
         return ds_param.parameter_class(ds_param.name, ds_param.label, options, is_hidden=ds_param.is_hidden, parent=ds_param.parent)
 
 
 @dataclass
 class DateDataSource(DataSource):
     """
     Lookup table for date parameter default options
 
     Attributes:
-        connection_name: Name of the connection to use defined in connections.py
         table_or_query: Either the name of the table to use, or a query to run
         default_date_col: The column name of the default date
-        date_format: The format of the default date(s). Defaults to '%Y-%m-%d'
         parent_id_col: The column name of the parent option id that the default date belongs to
+        date_format: The format of the default date(s). Defaults to '%Y-%m-%d'
+        connection_name: Name of the connection to use defined in connections.py
     """
     default_date_col: str
     parent_id_col: Optional[str] = None
     date_format: Optional[str] = '%Y-%m-%d'
     connection_name: str = c.DEFAULT_DB_CONN
 
     def convert(self, ds_param: p.DataSourceParameter, df: pd.DataFrame) -> p.DateParameter:
@@ -173,21 +181,21 @@
 
 @dataclass
 class NumberDataSource(_NumericDataSource):
     """
     Lookup table for number parameter default options
 
     Attributes:
-        connection_name: Name of the connection to use defined in connections.py
         table_or_query: Either the name of the table to use, or a query to run
         min_value_col: The column name of the minimum value
         max_value_col: The column name of the maximum value
         increment_col: The column name of the increment value. Defaults to column of 1's if None
         default_value_col: The column name of the default value. Defaults to min_value_col if None
         parent_id_col: The column name of the parent option id that the default value belongs to
+        connection_name: Name of the connection to use defined in connections.py
     """
     default_value_col: Optional[str] = None
     parent_id_col: Optional[str] = None
     connection_name: str = c.DEFAULT_DB_CONN
 
     def convert(self, ds_param: p.DataSourceParameter, df: pd.DataFrame) -> p.NumberParameter:
         """
@@ -224,22 +232,22 @@
 
 @dataclass
 class NumRangeDataSource(_NumericDataSource):
     """
     Lookup table for number range parameter default options
 
     Attributes:
-        connection_name: Name of the connection to use defined in connections.py
         table_or_query: Either the name of the table to use, or a query to run
         min_value_col: The column name of the minimum value
         max_value_col: The column name of the maximum value
         increment_col: The column name of the increment value. Defaults to column of 1's if None
         default_lower_value_col: The column name of the default lower value. Defaults to min_value_col if None
         default_upper_value_col: The column name of the default upper value. Defaults to max_value_col if None
         parent_id_col: The column name of the parent option id that the default value belongs to
+        connection_name: Name of the connection to use defined in connections.py
     """
     default_lower_value_col: Optional[str] = None
     default_upper_value_col: Optional[str] = None
     parent_id_col: Optional[str] = None
     connection_name: str = c.DEFAULT_DB_CONN
 
     def convert(self, ds_param: p.DataSourceParameter, df: pd.DataFrame) -> p.NumRangeParameter:
```

### Comparing `squirrels-0.1.0/squirrels/dateutils.py` & `squirrels-0.1.1/squirrels/dateutils.py`

 * *Files 14% similar despite different names*

```diff
@@ -55,15 +55,15 @@
     """
     Interface for adjusting a date to some day of calendar unit
     """
     idx: int
 
     def __post_init__(self):
         if self.idx == 0:
-            raise _utils.ConfigurationError("The idx attribute of any DateModifier object cannot be zero")
+            raise _utils.ConfigurationError("For constructors of class names that start with DayIdxOf_, idx cannot be zero")
         self.incr = self.idx - 1 if self.idx > 0 else self.idx
 
 
 @dataclass
 class DayIdxOfMonthsCycle(_DayIdxOfCalendarUnit):
     """
     DateModifier class to get the idx-th day of a cycle of months for an input date
@@ -219,52 +219,92 @@
 class DateModPipeline(DateModifier):
     """
     DateModifier class to apply a list of date modifiers to an input date
 
     Attributes:
         modifiers: The list of DateModifier's to apply in sequence.
     """
-    modifiers: Sequence[DateModifier]
+    date_modifiers: Sequence[DateModifier]
 
     def __post_init__(self):
-        self.modifiers = tuple(self.modifiers)
+        self.date_modifiers = tuple(self.date_modifiers)
     
     def modify(self, date: datetime) -> datetime:
-        for modifier in self.modifiers:
+        for modifier in self.date_modifiers:
             date = modifier.modify(date)
         return date
+    
+    def get_joined_modifiers(self, date_modifiers: Sequence[DateModifier]) -> Sequence[DateModifier]:
+        """
+        Create a new sequence of DateModifier by joining the date modifiers in this class 
+        with the input date_modifiers
+
+        Parameters:
+            date_modifiers: The new date modifier sequence to join
+
+        Returns:
+            A new sequence of DateModifier
+        """
+        joined_modifiers = self.date_modifiers + tuple(date_modifiers)
+        return joined_modifiers
+
+    def with_more_modifiers(self, date_modifiers: Sequence[DateModifier]):
+        """
+        Create a new DateModPipeline with more date modifiers
+
+        Parameters:
+            date_modifiers: The additional date modifiers to add
+
+        Returns:
+            A new DateModPipeline
+        """
+        joined_modifiers = self.get_joined_modifiers(date_modifiers)
+        return DateModPipeline(joined_modifiers)
+    
+    def get_date_list(self, start_date: datetime, step: _OffsetUnits) -> Sequence[datetime]:
+        """
+        This method modifies the input date, and returns all dates from the input date to the modified date, 
+        incremented by a DateModifier step.
+
+        If the step is positive and start date is less than end date, then it'll return an increasing list of
+        dates starting from the start date. If the step is positive and start date is less than end date, 
+        then it'll return a decreasing list of dates starting from the start date. Otherwise, an empty list
+        is returned.
+
+        Parameters:
+            start_date: The input date (it's the first date in the output list if step moves towards end date)
+            step: The increment to take (specified as an offset DateModifier). Offset cannot be zero
+
+        Returns:
+            A list of datetime objects
+        """
+        if step.offset == 0:
+            raise _utils.ConfigurationError("The length of 'step' must not be zero")
+        
+        output = []
+        end_date = self.modify(start_date)
+        curr_date = start_date
+        is_not_done_positive_step = lambda: curr_date <= end_date and step.offset > 0
+        is_not_done_negative_step = lambda: curr_date >= end_date and step.offset < 0
+        while is_not_done_positive_step() or is_not_done_negative_step():
+            output.append(curr_date)
+            curr_date = step.modify(curr_date)
+        return output
 
 
 @dataclass
 class _DateRepresentationModifier:
     """
     Abstract class for modifying other representations of dates (such as string or unix timestemp)
     """
     def __init__(self, date_modifiers: Sequence[DateModifier]):
         self.date_modifier = DateModPipeline(date_modifiers)
-    
-    def _get_joined_modifiers(self, date_modifiers: Sequence[DateModifier]) -> Sequence[DateModifier]:
-        joined_modifiers = self.date_modifier.modifiers + tuple(date_modifiers)
-        return joined_modifiers
 
     def with_more_modifiers(self, date_modifiers: Sequence[DateModifier]):
         raise _utils.AbstractMethodCallError(self.__class__, "with_more_modifiers")
-    
-    def get_date_list(self, curr_date: datetime, step: DateModifier) -> Sequence[datetime]:
-        modified_date = self.date_modifier.modify(curr_date)
-        curr_date, end_date = min(curr_date, modified_date), max(curr_date, modified_date)
-        distance = None
-        output = []
-        while curr_date <= end_date:
-            if distance is not None and (end_date - curr_date) >= distance:
-                raise _utils.ConfigurationError("The step must increment forward in time")
-            distance = end_date - curr_date
-            output.append(curr_date)
-            curr_date = step.modify(curr_date)
-        return output
 
 
 @dataclass
 class DateStringModifier(_DateRepresentationModifier):
     """
     Class to modify a string representation of a date given a DateModifier
 
@@ -282,15 +322,15 @@
 
         Parameters:
             date_modifiers: The additional date modifiers to add
 
         Returns:
             A new DateStringModifier
         """
-        joined_modifiers = self._get_joined_modifiers(date_modifiers)
+        joined_modifiers = self.date_modifier.get_joined_modifiers(date_modifiers)
         return DateStringModifier(joined_modifiers, self.date_format)
     
     def _get_input_date_obj(self, date_str: str, input_format: str = None) -> datetime:
         input_format = self.date_format if input_format is None else input_format
         return datetime.strptime(date_str, input_format)
 
     def modify(self, date_str: str, input_format: str = None) -> str:
@@ -303,29 +343,34 @@
         
         Returns:
             The resulting date string
         """
         date_obj = self._get_input_date_obj(date_str, input_format)
         return self.date_modifier.modify(date_obj).strftime(self.date_format)
     
-    def get_date_list(self, date_str: str, step: DateModifier, input_format: str = None) -> Sequence[str]:
+    def get_date_list(self, start_date_str: str, step: DateModifier, input_format: str = None) -> Sequence[str]:
         """
-        This method modifies the input date string, and returns all dates from the earlier to later date, 
-        incremented by a DateModifier step, until the last date is less than or equal to the later date.
+        This method modifies the input date string, and returns all dates as strings from the input date 
+        to the modified date, incremented by a DateModifier step.
+
+        If the step is positive and start date is less than end date, then it'll return an increasing list of
+        dates starting from the start date. If the step is positive and start date is less than end date, 
+        then it'll return a decreasing list of dates starting from the start date. Otherwise, an empty list
+        is returned.
 
         Parameters:
-            date_str: The input date string, usually the first date in the output list
-            step: The increment to take (specified as a DateModifier). It must increment forward in time
+            start_date_str: The input date string (it's the first date in the output list if step moves towards end date)
+            step: The increment to take (specified as an offset DateModifier). Offset cannot be zero
             input_format: The input date format. Defaults to the same as output date format
 
         Returns:
             A list of date strings
         """
-        curr_date = self._get_input_date_obj(date_str, input_format)
-        output = super().get_date_list(curr_date, step)
+        curr_date = self._get_input_date_obj(start_date_str, input_format)
+        output = self.date_modifier.get_date_list(curr_date, step)
         return [x.strftime(self.date_format) for x in output]
 
 
 @dataclass
 class TimestampModifier(_DateRepresentationModifier):
     """
     Class to modify a numeric representation of a date (as Unix/Epoch/POSIX timestamp) given a DateModifier
@@ -343,15 +388,15 @@
 
         Parameters:
             date_modifiers: The additional date modifiers to add
 
         Returns:
             A new TimestampModifier
         """
-        joined_modifiers = self._get_joined_modifiers(date_modifiers)
+        joined_modifiers = self.date_modifier.get_joined_modifiers(date_modifiers)
         return TimestampModifier(joined_modifiers)
 
     def modify(self, timestamp: float) -> float:
         """
         Modifies the input timestamp with the date modifiers
 
         Parameters:
@@ -359,22 +404,27 @@
         
         Returns:
             The resulting timestamp
         """
         date_obj = datetime.fromtimestamp(timestamp)
         return self.date_modifier.modify(date_obj).timestamp()
     
-    def get_date_list(self, timestamp: float, step: DateModifier) -> Sequence[float]:
+    def get_date_list(self, start_timestamp: float, step: DateModifier) -> Sequence[float]:
         """
-        This method modifies the input date string, and returns all dates from the earlier to later date, 
-        incremented by a DateModifier step, until the last date is less than or equal to the later date.
+        This method modifies the input timestamp, and returns all dates as timestampes/floats from the input date 
+        to the modified date, incremented by a DateModifier step.
+
+        If the step is positive and start date is less than end date, then it'll return an increasing list of
+        dates starting from the start date. If the step is positive and start date is less than end date, 
+        then it'll return a decreasing list of dates starting from the start date. Otherwise, an empty list
+        is returned.
 
         Parameters:
-            timestamp: The input timestamp as float, usually the first date in the output list
-            step: The increment to take (specified as a DateModifier). It must increment forward in time
+            start_timestamp: The input timestamp as float (it's the first date in the output list if step moves towards end date)
+            step: The increment to take (specified as an offset DateModifier). Offset cannot be zero
 
         Returns:
             A list of timestamp as floats
         """
-        curr_date = datetime.fromtimestamp(timestamp)
-        output = super().get_date_list(curr_date, step)
+        curr_date = datetime.fromtimestamp(start_timestamp)
+        output = self.date_modifier.get_date_list(curr_date, step)
         return [x.timestamp() for x in output]
```

### Comparing `squirrels-0.1.0/squirrels/package_data/base_project/connections.py` & `squirrels-0.1.1/squirrels/package_data/base_project/connections.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,19 +3,18 @@
 
 from squirrels import get_credential
 
 
 # Note: all connections must be shareable across multiple thread. No writes will occur on them
 def main(proj: Dict[str, Any], *p_args, **kwargs) -> Dict[str, Union[Engine, Pool]]:
 
-    # ## Example of getting the username and password set with "$ squirrels set-credential [key]"
-    # cred = get_credential('my_key')
-    # # Use cred.username and cred.password to access the username and password
+    ## Example of getting the username and password set with "$ squirrels set-credential [key]"
+    # cred = get_credential('my_key') # then use cred.username and cred.password to access the username and password
 
     # Create a connection pool / engine
     pool = create_engine('sqlite:///./database/sample_database.db')
 
-    # ## Example of using QueuePool instead for a custom db connector:
+    ## Example of using QueuePool instead for a custom db connector:
     # connection_creator = lambda: sqlite3.connect('./database/sample_database.db', check_same_thread=False)
     # pool = QueuePool(connection_creator)
     
     return {'default': pool}
```

### Comparing `squirrels-0.1.0/squirrels/package_data/base_project/database/seattle_weather.db` & `squirrels-0.1.1/squirrels/package_data/base_project/database/seattle_weather.db`

 * *Files identical despite different names*

### Comparing `squirrels-0.1.0/squirrels/package_data/static/favicon.ico` & `squirrels-0.1.1/squirrels/package_data/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `squirrels-0.1.0/squirrels/package_data/static/script.js` & `squirrels-0.1.1/squirrels/package_data/static/script.js`

 * *Files identical despite different names*

### Comparing `squirrels-0.1.0/squirrels/package_data/static/style.css` & `squirrels-0.1.1/squirrels/package_data/static/style.css`

 * *Files identical despite different names*

### Comparing `squirrels-0.1.0/squirrels/package_data/templates/index.html` & `squirrels-0.1.1/squirrels/package_data/templates/index.html`

 * *Files identical despite different names*

### Comparing `squirrels-0.1.0/squirrels/parameter_options.py` & `squirrels-0.1.1/squirrels/parameter_options.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Iterable, Optional, Union
+from typing import Iterable, Optional, Union, Dict, Any
 from dataclasses import dataclass, field
 from decimal import Decimal, InvalidOperation as InvalidDecimalConversion
 from datetime import datetime
 
 from squirrels._utils import ConfigurationError
 
 Number = Union[Decimal, int, str]
@@ -41,40 +41,84 @@
 
 @dataclass
 class SelectParameterOption(ParameterOption):
     """
     Parameter option for a select parameter
 
     Attributes:
-        identifier: Unique identifier for this option that never changes over time
-        label: Human readable label that gets shown as a dropdown option
-        is_default: True if this is a default option, False otherwise
-        parent_option_id: Identifier of the parent option, or None if this is a top-level option
-        parent_option_ids: Set of parent option ids (only used if parent_option_id is None), or an empty set if this is a top-level option
     """
     identifier: str
     label: str
     is_default: bool = False
     parent_option_id: Optional[str] = field(default=None, repr=False)
     parent_option_ids: Iterable[str] = frozenset()
 
+    def __init__(self, identifier: str, label: str, *, is_default: bool = False, 
+                 parent_option_id: Optional[str] = None, parent_option_ids: Iterable[str] = frozenset(), 
+                 custom_fields: Dict[str, Any] = {}, **kwargs):
+        """
+        Constructor for SelectParameterOption
+
+        Parameters:
+            identifier: Unique identifier for this option that never changes over time
+            label: Human readable label that gets shown as a dropdown option
+            is_default: True if this is a default option, False otherwise
+            parent_option_id: Identifier of the parent option, or None if this is a top-level option
+            parent_option_ids: Set of parent option ids (only used if parent_option_id is None)
+            custom_fields: Dictionary to associate custom attributes to the parameter option
+            **kwargs: Any additional keyword arguments specified (except the ones above) gets included into custom_fields as well
+        """
+        self.identifier = identifier
+        self.label = label
+        self.is_default = is_default
+        self.parent_option_id = parent_option_id
+        self.parent_option_ids = parent_option_ids
+        self.custom_fields = {
+            **kwargs, **custom_fields, "id": identifier, "label": label
+        }
+        super().__post_init__()
+
+    def get_custom_field(self, field: str, default_field: Optional[str] = None, default: Any = None) -> Any:
+        """
+        Get field value from the custom_fields attribute
+
+        Parameters:
+            field: The key to use to fetch the custom field from "custom_fields"
+            default_field: If field does not exist in "custom_fields", then this is used instead as the field (if not None)
+            default: If field does not exist and default_field is None, then this value is used as default
+        
+        Returns:
+            The type of the custom field
+        """
+        if default_field is not None:
+            default = self.get_custom_field(default_field)
+        try:
+            if default is not None:
+                selected_field = self.custom_fields.get(field, default)
+            else:
+                selected_field = self.custom_fields[field]
+        except KeyError as e:
+            raise ConfigurationError(f"Field '{field}' must exist for parameter option '{self.to_dict()}'") from e
+        
+        return selected_field
+    
     def to_dict(self):
         return {'id': self.identifier, 'label': self.label}
 
 
 @dataclass
 class DateParameterOption(ParameterOption):
     """
     Parameter option for default dates if it varies based on selection of another parameter
 
     Attributes:
         default_date: Default date for this option
         date_format: Format of the default date, default is '%Y-%m-%d'
         parent_option_id: Identifier of the parent option, or None if this is a top-level option
-        parent_option_ids: Set of parent option ids (only used if parent_option_id is None), or an empty set if this is a top-level option
+        parent_option_ids: Set of parent option ids (only used if parent_option_id is None)
     """
     default_date: Union[str, datetime]
     date_format: str = '%Y-%m-%d'
     parent_option_id: Optional[str] = field(default=None, repr=False)
     parent_option_ids: Iterable[str] = frozenset()
 
     def __post_init__(self) -> None:
@@ -144,15 +188,15 @@
 
     Attributes:
         min_value: Minimum selectable value
         max_value: Maximum selectable value
         increment: Increment of selectable values, and must fit evenly between min_value and max_value
         default_value: Default value for this option, and must be selectable based on min_value, max_value, and increment
         parent_option_id: Identifier of the parent option, or None if this is a top-level option
-        parent_option_ids: Set of parent option ids (only used if parent_option_id is None), or an empty set if this is a top-level option
+        parent_option_ids: Set of parent option ids (only used if parent_option_id is None)
     """
     default_value: Decimal
     parent_option_id: Optional[str] = field(default=None, repr=False)
     parent_option_ids: Iterable[str] = frozenset()
 
     def __post_init__(self) -> None:
         super().__post_init__()
@@ -168,15 +212,15 @@
         min_value: Minimum selectable value
         max_value: Maximum selectable value
         increment: Increment of selectable values, and must fit evenly between min_value and max_value
         default_lower_value: Default lower value for this option, and must be selectable based on min_value, max_value, and increment
         default_upper_value: Default upper value for this option, and must be selectable based on min_value, max_value, and increment. 
                 Must also be greater than default_lower_value
         parent_option_id: Identifier of the parent option, or None if this is a top-level option
-        parent_option_ids: Set of parent option ids (only used if parent_option_id is None), or an empty set if this is a top-level option
+        parent_option_ids: Set of parent option ids (only used if parent_option_id is None)
     """
     default_lower_value: Decimal
     default_upper_value: Decimal
     parent_option_id: Optional[str] = field(default=None, repr=False)
     parent_option_ids: Iterable[str] = frozenset()
 
     def __post_init__(self) -> None:
```

### Comparing `squirrels-0.1.0/squirrels/parameters.py` & `squirrels-0.1.1/squirrels/parameters.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from __future__ import annotations
-from typing import Type, Sequence, Dict, List, Iterator, Optional, Union
+from typing import Type, Sequence, Dict, List, Any, Iterator, Optional, Union
 from dataclasses import dataclass
 from datetime import datetime
 from decimal import Decimal
 import copy
 
 from squirrels import parameter_options as po, _utils as u
 from squirrels.data_sources import DataSource
@@ -198,23 +198,35 @@
         Returns:
             A new copy of SingleSelectParameter with the selection applied
         """
         param_copy = copy.copy(self)
         param_copy.selected_id = self._validate_selected_id_in_options(selection)
         param_copy.children = [child.refresh(param_copy) for child in param_copy.children]
         return param_copy
-
-    def get_selected(self) -> po.SelectParameterOption:
+    
+    def get_selected(self, field: Optional[str] = None, *, default_field: Optional[str] = None,
+                     default: Any = None) -> Union[po.SelectParameterOption, str]:
         """
-        Gets the selected single-select option
+        Gets the selected single-select option or selected custom field
+
+        Parameters:
+            field: If field is not None, the method gets this field from the "custom_fields" attribute of the selected option. 
+                Otherwise, returns the class object of the selected option
+            default_field: If field does not exist for a parameter option and default_field is not None, the default_field is used 
+                as the "field" instead. Does nothing if field is None
+            default: If field does not exist for a parameter option, default_field is None, but default is not None, then the default 
+                is returned as the selected field. Does nothing if field is None or default_field is not None
 
         Returns:
-            A SelectParameterOption class object
-        """
-        return next(x for x in self.options if x.identifier == self.selected_id)
+            A SelectParameterOption class object if no field is provided, or the type of the custom field
+        """
+        selected = next(x for x in self.options if x.identifier == self.selected_id)
+        if field is not None:
+            selected = selected.get_custom_field(field, default_field, default)
+        return selected
     
     def get_selected_id(self) -> str:
         """
         Gets the ID of the selected option
 
         Returns:
             A string ID
@@ -324,27 +336,40 @@
         return the full list of options if "include_all" is set to True
 
         Returns:
             A boolean
         """
         return len(self.selected_ids) > 0
 
-    def get_selected_list(self) -> Sequence[po.SelectParameterOption]:
+    def get_selected_list(self, field: Optional[str] = None, *, default_field: Optional[str] = None,
+                          default: Any = None) -> Sequence[Union[po.SelectParameterOption, Any]]:
         """
-        Gets the sequence of the selected option(s)
+        Gets the sequence of the selected option(s) or a sequence of selected custom fields
+
+        Parameters:
+            field: If field is not None, the method gets this field from the "custom_fields" attribute of the selected options. 
+                Otherwise, returns the class objects of the selected options
+            default_field: If field does not exist for a parameter option and default_field is not None, the default_field is used 
+                as the "field" instead. Does nothing if field is None
+            default: If field does not exist for a parameter option, default_field is None, but default is not None, the default 
+                is returned as the selected field. Does nothing if field is None or default_field is not None
 
         Returns:
-            A sequence of SelectParameterOption class objects
+            A sequence of SelectParameterOption class objects or sequence of type of custom field
         """
         if not self.has_non_empty_selection() and self.include_all:
-            result = tuple(self.options)
+            selected_list = self.options
         else:
-            result = tuple(x for x in self.options if x.identifier in self.selected_ids)
-        return result
-    
+            selected_list = (x for x in self.options if x.identifier in self.selected_ids)
+        
+        if field is not None:
+            selected_list = [selected.get_custom_field(field, default_field, default) for selected in selected_list]
+        
+        return tuple(selected_list)
+
     def get_selected_ids_as_list(self) -> Sequence[str]:
         """
         Gets the sequence of ID(s) of the selected option(s)
 
         Returns:
             A sequence of strings
         """
```

### Comparing `squirrels-0.1.0/squirrels.egg-info/PKG-INFO` & `squirrels-0.1.1/squirrels.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: squirrels
-Version: 0.1.0
-Summary: Python Package for Configuring SQL Generating APIs
+Version: 0.1.1
+Summary: Squirrels - Configure REST APIs for BI Analytics
 Author: Tim Huang
 Author-email: tim.yuting@hotmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Squirrels
```

### Comparing `squirrels-0.1.0/squirrels.egg-info/SOURCES.txt` & `squirrels-0.1.1/squirrels.egg-info/SOURCES.txt`

 * *Files identical despite different names*

