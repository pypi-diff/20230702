# Comparing `tmp/superagi_tools-1.0.5.tar.gz` & `tmp/superagi_tools-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "superagi_tools-1.0.5.tar", last modified: Sun Jul  2 07:02:05 2023, max compression
+gzip compressed data, was "superagi_tools-1.0.6.tar", last modified: Sun Jul  2 08:28:04 2023, max compression
```

## Comparing `superagi_tools-1.0.5.tar` & `superagi_tools-1.0.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 abhijeet  (1000) abhijeet  (1000)        0 2023-07-02 07:02:05.392867 superagi_tools-1.0.5/
--rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)     1054 2023-07-02 04:53:24.000000 superagi_tools-1.0.5/LICENSE
--rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)      187 2023-07-02 07:02:05.392867 superagi_tools-1.0.5/PKG-INFO
--rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)       76 2023-06-28 12:10:34.000000 superagi_tools-1.0.5/README.md
--rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)       38 2023-07-02 07:02:05.392867 superagi_tools-1.0.5/setup.cfg
--rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)      319 2023-07-02 07:01:28.000000 superagi_tools-1.0.5/setup.py
-drwxrwxr-x   0 abhijeet  (1000) abhijeet  (1000)        0 2023-07-02 07:02:05.388871 superagi_tools-1.0.5/superagi/
--rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)        0 2023-06-29 00:44:17.000000 superagi_tools-1.0.5/superagi/__init__.py
-drwxrwxr-x   0 abhijeet  (1000) abhijeet  (1000)        0 2023-07-02 07:02:05.388871 superagi_tools-1.0.5/superagi/tools/
--rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)        0 2023-06-29 00:51:45.000000 superagi_tools-1.0.5/superagi/tools/__init__.py
--rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)     7283 2023-07-02 07:00:37.000000 superagi_tools-1.0.5/superagi/tools/base_tool.py
-drwxrwxr-x   0 abhijeet  (1000) abhijeet  (1000)        0 2023-07-02 07:02:05.388871 superagi_tools-1.0.5/superagi_tools.egg-info/
--rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)      187 2023-07-02 07:02:05.000000 superagi_tools-1.0.5/superagi_tools.egg-info/PKG-INFO
--rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)      291 2023-07-02 07:02:05.000000 superagi_tools-1.0.5/superagi_tools.egg-info/SOURCES.txt
--rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)        1 2023-07-02 07:02:05.000000 superagi_tools-1.0.5/superagi_tools.egg-info/dependency_links.txt
--rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)       29 2023-07-02 07:02:05.000000 superagi_tools-1.0.5/superagi_tools.egg-info/requires.txt
--rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)        9 2023-07-02 07:02:05.000000 superagi_tools-1.0.5/superagi_tools.egg-info/top_level.txt
+drwxrwxr-x   0 abhijeet  (1000) abhijeet  (1000)        0 2023-07-02 08:28:04.338078 superagi_tools-1.0.6/
+-rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)     1054 2023-07-02 04:53:24.000000 superagi_tools-1.0.6/LICENSE
+-rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)      187 2023-07-02 08:28:04.338078 superagi_tools-1.0.6/PKG-INFO
+-rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)       76 2023-06-28 12:10:34.000000 superagi_tools-1.0.6/README.md
+-rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)       38 2023-07-02 08:28:04.338078 superagi_tools-1.0.6/setup.cfg
+-rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)      319 2023-07-02 08:27:56.000000 superagi_tools-1.0.6/setup.py
+drwxrwxr-x   0 abhijeet  (1000) abhijeet  (1000)        0 2023-07-02 08:28:04.338078 superagi_tools-1.0.6/superagi/
+-rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)        0 2023-06-29 00:44:17.000000 superagi_tools-1.0.6/superagi/__init__.py
+drwxrwxr-x   0 abhijeet  (1000) abhijeet  (1000)        0 2023-07-02 08:28:04.338078 superagi_tools-1.0.6/superagi/tools/
+-rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)        0 2023-06-29 00:51:45.000000 superagi_tools-1.0.6/superagi/tools/__init__.py
+-rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)     7485 2023-07-02 08:27:41.000000 superagi_tools-1.0.6/superagi/tools/base_tool.py
+drwxrwxr-x   0 abhijeet  (1000) abhijeet  (1000)        0 2023-07-02 08:28:04.338078 superagi_tools-1.0.6/superagi_tools.egg-info/
+-rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)      187 2023-07-02 08:28:04.000000 superagi_tools-1.0.6/superagi_tools.egg-info/PKG-INFO
+-rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)      291 2023-07-02 08:28:04.000000 superagi_tools-1.0.6/superagi_tools.egg-info/SOURCES.txt
+-rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)        1 2023-07-02 08:28:04.000000 superagi_tools-1.0.6/superagi_tools.egg-info/dependency_links.txt
+-rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)       29 2023-07-02 08:28:04.000000 superagi_tools-1.0.6/superagi_tools.egg-info/requires.txt
+-rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)        9 2023-07-02 08:28:04.000000 superagi_tools-1.0.6/superagi_tools.egg-info/top_level.txt
```

### Comparing `superagi_tools-1.0.5/LICENSE` & `superagi_tools-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `superagi_tools-1.0.5/superagi/tools/base_tool.py` & `superagi_tools-1.0.6/superagi/tools/base_tool.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import inspect
 import os
 from abc import abstractmethod
 from functools import wraps
 from inspect import signature
 from typing import List
 from typing import Optional, Type, Callable, Any, Union, Dict, Tuple
 
@@ -53,36 +54,36 @@
     return _construct_model_subset(
         f"{schema_name}Schema", inferred_type, list(valid_parameters)
     )
 
 
 class BaseToolkitConfiguration:
 
-    def get_tool_config(self, key: str):
-        # Get the directory of the current module
-        module_dir = os.path.dirname(os.path.abspath(__file__))
+    def get_tool_config(self, key: str, module_dir):
+        config_path = self.__find_config_file(module_dir)
+        config = self.__load_config(config_path)
+        return config.get(key)
 
-        # Traverse up the directory structure until reaching the root directory
+    def __find_config_file(self, module_dir):
+        root_dir = module_dir
         while True:
-            config_path = os.path.join(module_dir, "config.yaml")
+            config_path = os.path.join(root_dir, "config.yaml")
             if os.path.isfile(config_path):
                 # Found the config.yaml file in the current directory
-                break
-            parent_dir = os.path.dirname(module_dir)
-            if parent_dir == module_dir:
+                return config_path
+            parent_dir = os.path.dirname(root_dir)
+            if parent_dir == root_dir:
                 # Reached the root directory without finding the config.yaml file
                 raise FileNotFoundError("config.yaml file not found")
-            module_dir = parent_dir
+            root_dir = parent_dir
 
-        # Default implementation of the tool configuration retrieval logic
+    def __load_config(self, config_path):
         with open(config_path) as file:
             config = yaml.safe_load(file)
-
-        # Retrieve the value associated with the given key
-        return config.get(key)
+        return config
 
 
 class BaseTool(BaseModel):
     name: str = None
     description: str
     args_schema: Type[BaseModel] = None
     permission_required: bool = True
@@ -154,15 +155,19 @@
     def from_function(cls, func: Callable, args_schema: Type[BaseModel] = None):
         if args_schema:
             return cls(description=func.__doc__, args_schema=args_schema)
         else:
             return cls(description=func.__doc__)
 
     def get_tool_config(self, key):
-        return self.toolkit_config.get_tool_config(key=key)
+        caller_frame = inspect.currentframe().f_back
+        caller_module = inspect.getmodule(caller_frame)
+        caller_file = inspect.getfile(caller_module)
+        caller_dir = os.path.dirname(os.path.abspath(caller_file))
+        return self.toolkit_config.get_tool_config(key=key, module_dir=caller_dir)
 
 
 class FunctionalTool(BaseTool):
     name: str = None
     description: str
     func: Callable
     args_schema: Type[BaseModel] = None
```

