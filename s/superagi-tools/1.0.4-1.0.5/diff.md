# Comparing `tmp/superagi_tools-1.0.4.tar.gz` & `tmp/superagi_tools-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "superagi_tools-1.0.4.tar", last modified: Sun Jul  2 06:07:00 2023, max compression
+gzip compressed data, was "superagi_tools-1.0.5.tar", last modified: Sun Jul  2 07:02:05 2023, max compression
```

## Comparing `superagi_tools-1.0.4.tar` & `superagi_tools-1.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 abhijeet  (1000) abhijeet  (1000)        0 2023-07-02 06:07:00.896818 superagi_tools-1.0.4/
--rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)     1054 2023-07-02 04:53:24.000000 superagi_tools-1.0.4/LICENSE
--rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)      187 2023-07-02 06:07:00.896818 superagi_tools-1.0.4/PKG-INFO
--rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)       76 2023-06-28 12:10:34.000000 superagi_tools-1.0.4/README.md
--rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)       38 2023-07-02 06:07:00.896818 superagi_tools-1.0.4/setup.cfg
--rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)      319 2023-07-02 06:06:06.000000 superagi_tools-1.0.4/setup.py
-drwxrwxr-x   0 abhijeet  (1000) abhijeet  (1000)        0 2023-07-02 06:07:00.896818 superagi_tools-1.0.4/superagi/
--rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)        0 2023-06-29 00:44:17.000000 superagi_tools-1.0.4/superagi/__init__.py
-drwxrwxr-x   0 abhijeet  (1000) abhijeet  (1000)        0 2023-07-02 06:07:00.896818 superagi_tools-1.0.4/superagi/tools/
--rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)        0 2023-06-29 00:51:45.000000 superagi_tools-1.0.4/superagi/tools/__init__.py
--rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)     6575 2023-07-02 06:04:52.000000 superagi_tools-1.0.4/superagi/tools/base_tool.py
-drwxrwxr-x   0 abhijeet  (1000) abhijeet  (1000)        0 2023-07-02 06:07:00.896818 superagi_tools-1.0.4/superagi_tools.egg-info/
--rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)      187 2023-07-02 06:07:00.000000 superagi_tools-1.0.4/superagi_tools.egg-info/PKG-INFO
--rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)      291 2023-07-02 06:07:00.000000 superagi_tools-1.0.4/superagi_tools.egg-info/SOURCES.txt
--rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)        1 2023-07-02 06:07:00.000000 superagi_tools-1.0.4/superagi_tools.egg-info/dependency_links.txt
--rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)       29 2023-07-02 06:07:00.000000 superagi_tools-1.0.4/superagi_tools.egg-info/requires.txt
--rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)        9 2023-07-02 06:07:00.000000 superagi_tools-1.0.4/superagi_tools.egg-info/top_level.txt
+drwxrwxr-x   0 abhijeet  (1000) abhijeet  (1000)        0 2023-07-02 07:02:05.392867 superagi_tools-1.0.5/
+-rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)     1054 2023-07-02 04:53:24.000000 superagi_tools-1.0.5/LICENSE
+-rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)      187 2023-07-02 07:02:05.392867 superagi_tools-1.0.5/PKG-INFO
+-rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)       76 2023-06-28 12:10:34.000000 superagi_tools-1.0.5/README.md
+-rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)       38 2023-07-02 07:02:05.392867 superagi_tools-1.0.5/setup.cfg
+-rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)      319 2023-07-02 07:01:28.000000 superagi_tools-1.0.5/setup.py
+drwxrwxr-x   0 abhijeet  (1000) abhijeet  (1000)        0 2023-07-02 07:02:05.388871 superagi_tools-1.0.5/superagi/
+-rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)        0 2023-06-29 00:44:17.000000 superagi_tools-1.0.5/superagi/__init__.py
+drwxrwxr-x   0 abhijeet  (1000) abhijeet  (1000)        0 2023-07-02 07:02:05.388871 superagi_tools-1.0.5/superagi/tools/
+-rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)        0 2023-06-29 00:51:45.000000 superagi_tools-1.0.5/superagi/tools/__init__.py
+-rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)     7283 2023-07-02 07:00:37.000000 superagi_tools-1.0.5/superagi/tools/base_tool.py
+drwxrwxr-x   0 abhijeet  (1000) abhijeet  (1000)        0 2023-07-02 07:02:05.388871 superagi_tools-1.0.5/superagi_tools.egg-info/
+-rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)      187 2023-07-02 07:02:05.000000 superagi_tools-1.0.5/superagi_tools.egg-info/PKG-INFO
+-rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)      291 2023-07-02 07:02:05.000000 superagi_tools-1.0.5/superagi_tools.egg-info/SOURCES.txt
+-rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)        1 2023-07-02 07:02:05.000000 superagi_tools-1.0.5/superagi_tools.egg-info/dependency_links.txt
+-rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)       29 2023-07-02 07:02:05.000000 superagi_tools-1.0.5/superagi_tools.egg-info/requires.txt
+-rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)        9 2023-07-02 07:02:05.000000 superagi_tools-1.0.5/superagi_tools.egg-info/top_level.txt
```

### Comparing `superagi_tools-1.0.4/LICENSE` & `superagi_tools-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `superagi_tools-1.0.4/superagi/tools/base_tool.py` & `superagi_tools-1.0.5/superagi/tools/base_tool.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import os
 from abc import abstractmethod
 from functools import wraps
 from inspect import signature
 from typing import List
 from typing import Optional, Type, Callable, Any, Union, Dict, Tuple
 
 import yaml
@@ -53,16 +54,31 @@
         f"{schema_name}Schema", inferred_type, list(valid_parameters)
     )
 
 
 class BaseToolkitConfiguration:
 
     def get_tool_config(self, key: str):
+        # Get the directory of the current module
+        module_dir = os.path.dirname(os.path.abspath(__file__))
+
+        # Traverse up the directory structure until reaching the root directory
+        while True:
+            config_path = os.path.join(module_dir, "config.yaml")
+            if os.path.isfile(config_path):
+                # Found the config.yaml file in the current directory
+                break
+            parent_dir = os.path.dirname(module_dir)
+            if parent_dir == module_dir:
+                # Reached the root directory without finding the config.yaml file
+                raise FileNotFoundError("config.yaml file not found")
+            module_dir = parent_dir
+
         # Default implementation of the tool configuration retrieval logic
-        with open("config.yaml") as file:
+        with open(config_path) as file:
             config = yaml.safe_load(file)
 
         # Retrieve the value associated with the given key
         return config.get(key)
 
 
 class BaseTool(BaseModel):
```

