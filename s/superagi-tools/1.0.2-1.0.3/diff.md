# Comparing `tmp/superagi_tools-1.0.2.tar.gz` & `tmp/superagi_tools-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "superagi_tools-1.0.2.tar", last modified: Sun Jul  2 04:54:06 2023, max compression
+gzip compressed data, was "superagi_tools-1.0.3.tar", last modified: Sun Jul  2 05:56:15 2023, max compression
```

## Comparing `superagi_tools-1.0.2.tar` & `superagi_tools-1.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 abhijeet  (1000) abhijeet  (1000)        0 2023-07-02 04:54:06.912764 superagi_tools-1.0.2/
--rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)     1054 2023-07-02 04:53:24.000000 superagi_tools-1.0.2/LICENSE
--rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)      187 2023-07-02 04:54:06.912764 superagi_tools-1.0.2/PKG-INFO
--rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)       76 2023-06-28 12:10:34.000000 superagi_tools-1.0.2/README.md
--rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)       38 2023-07-02 04:54:06.912764 superagi_tools-1.0.2/setup.cfg
--rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)      319 2023-07-02 04:52:07.000000 superagi_tools-1.0.2/setup.py
-drwxrwxr-x   0 abhijeet  (1000) abhijeet  (1000)        0 2023-07-02 04:54:06.896764 superagi_tools-1.0.2/superagi/
--rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)        0 2023-06-29 00:44:17.000000 superagi_tools-1.0.2/superagi/__init__.py
-drwxrwxr-x   0 abhijeet  (1000) abhijeet  (1000)        0 2023-07-02 04:54:06.896764 superagi_tools-1.0.2/superagi/tools/
--rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)        0 2023-06-29 00:51:45.000000 superagi_tools-1.0.2/superagi/tools/__init__.py
--rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)     6603 2023-06-30 05:10:33.000000 superagi_tools-1.0.2/superagi/tools/base_tool.py
-drwxrwxr-x   0 abhijeet  (1000) abhijeet  (1000)        0 2023-07-02 04:54:06.912764 superagi_tools-1.0.2/superagi_tools.egg-info/
--rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)      187 2023-07-02 04:54:06.000000 superagi_tools-1.0.2/superagi_tools.egg-info/PKG-INFO
--rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)      291 2023-07-02 04:54:06.000000 superagi_tools-1.0.2/superagi_tools.egg-info/SOURCES.txt
--rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)        1 2023-07-02 04:54:06.000000 superagi_tools-1.0.2/superagi_tools.egg-info/dependency_links.txt
--rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)       29 2023-07-02 04:54:06.000000 superagi_tools-1.0.2/superagi_tools.egg-info/requires.txt
--rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)        9 2023-07-02 04:54:06.000000 superagi_tools-1.0.2/superagi_tools.egg-info/top_level.txt
+drwxrwxr-x   0 abhijeet  (1000) abhijeet  (1000)        0 2023-07-02 05:56:15.632614 superagi_tools-1.0.3/
+-rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)     1054 2023-07-02 04:53:24.000000 superagi_tools-1.0.3/LICENSE
+-rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)      187 2023-07-02 05:56:15.632614 superagi_tools-1.0.3/PKG-INFO
+-rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)       76 2023-06-28 12:10:34.000000 superagi_tools-1.0.3/README.md
+-rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)       38 2023-07-02 05:56:15.632614 superagi_tools-1.0.3/setup.cfg
+-rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)      319 2023-07-02 05:55:57.000000 superagi_tools-1.0.3/setup.py
+drwxrwxr-x   0 abhijeet  (1000) abhijeet  (1000)        0 2023-07-02 05:56:15.632614 superagi_tools-1.0.3/superagi/
+-rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)        0 2023-06-29 00:44:17.000000 superagi_tools-1.0.3/superagi/__init__.py
+drwxrwxr-x   0 abhijeet  (1000) abhijeet  (1000)        0 2023-07-02 05:56:15.632614 superagi_tools-1.0.3/superagi/tools/
+-rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)        0 2023-06-29 00:51:45.000000 superagi_tools-1.0.3/superagi/tools/__init__.py
+-rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)     6589 2023-07-02 05:55:43.000000 superagi_tools-1.0.3/superagi/tools/base_tool.py
+drwxrwxr-x   0 abhijeet  (1000) abhijeet  (1000)        0 2023-07-02 05:56:15.632614 superagi_tools-1.0.3/superagi_tools.egg-info/
+-rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)      187 2023-07-02 05:56:15.000000 superagi_tools-1.0.3/superagi_tools.egg-info/PKG-INFO
+-rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)      291 2023-07-02 05:56:15.000000 superagi_tools-1.0.3/superagi_tools.egg-info/SOURCES.txt
+-rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)        1 2023-07-02 05:56:15.000000 superagi_tools-1.0.3/superagi_tools.egg-info/dependency_links.txt
+-rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)       29 2023-07-02 05:56:15.000000 superagi_tools-1.0.3/superagi_tools.egg-info/requires.txt
+-rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)        9 2023-07-02 05:56:15.000000 superagi_tools-1.0.3/superagi_tools.egg-info/top_level.txt
```

### Comparing `superagi_tools-1.0.2/LICENSE` & `superagi_tools-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `superagi_tools-1.0.2/superagi/tools/base_tool.py` & `superagi_tools-1.0.3/superagi/tools/base_tool.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,16 @@
     return _construct_model_subset(
         f"{schema_name}Schema", inferred_type, list(valid_parameters)
     )
 
 
 class BaseToolkitConfiguration:
 
-    def get_tool_config(key: str):
+    @property
+    def get_tool_config(self, key: str):
         # Default implementation of the tool configuration retrieval logic
         with open("config.yaml") as file:
             config = yaml.safe_load(file)
 
         # Retrieve the value associated with the given key
         return config.get(key)
 
@@ -86,16 +87,15 @@
 
     @abstractmethod
     def _execute(self, *args: Any, **kwargs: Any):
         pass
 
     @property
     def max_token_limit(self):
-        token_limit = 600
-        return token_limit
+        return 600
 
     def _parse_input(
             self,
             tool_input: Union[str, Dict],
     ) -> Union[str, Dict[str, Any]]:
         """Convert tool input to pydantic model."""
         input_args = self.args_schema
```

