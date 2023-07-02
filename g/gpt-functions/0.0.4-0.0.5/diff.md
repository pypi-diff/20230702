# Comparing `tmp/gpt_functions-0.0.4.tar.gz` & `tmp/gpt_functions-0.0.5.tar.gz`

## Comparing `gpt_functions-0.0.4.tar` & `gpt_functions-0.0.5.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gpt_functions-0.0.4/src/gpt_functions/__init__.py
--rw-r--r--   0        0        0     7554 2020-02-02 00:00:00.000000 gpt_functions-0.0.4/src/gpt_functions/meta.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 gpt_functions-0.0.4/.gitignore
--rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 gpt_functions-0.0.4/LICENSE
--rw-r--r--   0        0        0    14708 2020-02-02 00:00:00.000000 gpt_functions-0.0.4/README.md
--rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 gpt_functions-0.0.4/pyproject.toml
--rw-r--r--   0        0        0    15361 2020-02-02 00:00:00.000000 gpt_functions-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gpt_functions-0.0.5/src/gpt_functions/__init__.py
+-rw-r--r--   0        0        0    10613 2020-02-02 00:00:00.000000 gpt_functions-0.0.5/src/gpt_functions/meta.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 gpt_functions-0.0.5/.gitignore
+-rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 gpt_functions-0.0.5/LICENSE
+-rw-r--r--   0        0        0    14708 2020-02-02 00:00:00.000000 gpt_functions-0.0.5/README.md
+-rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 gpt_functions-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0    15361 2020-02-02 00:00:00.000000 gpt_functions-0.0.5/PKG-INFO
```

### Comparing `gpt_functions-0.0.4/src/gpt_functions/meta.py` & `gpt_functions-0.0.5/src/gpt_functions/meta.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from dataclasses import dataclass, field
 from typing import Optional, List, Callable, get_type_hints
 import re
 import inspect
 import warnings
+import json
 
 @dataclass
 class Parameter:
     name: str = field(metadata={"description": "The name of the function parameter."})
     type: str = field(metadata={"description": "The type of the function parameter."})
     description: str = field(default="", metadata={"description": "The description of the function parameter."})
     enum: Optional[List[str]] = field(default=None, metadata={"description": "A list of possible values for the function parameter."})
@@ -201,7 +202,96 @@
                 description=Function.extract_variable_definition(parameter_name, description)[:character_limit],
                 required=inspect.signature(function).parameters[parameter_name].default is inspect.Parameter.empty,
             )
             parameters.append(parameter)
         description = description.strip()[:character_limit]
         return Function(name=name, description=description, parameters=parameters)
 
+class Library:
+    def __init__(self):
+        self.function_mapping = {}
+
+    def add_function(self, function: Function):
+        """
+        Adds a Function instance to the Library class.
+
+        Args:
+            function (Function): The Function instance to add.
+        """
+        self.function_mapping[function.name] = function
+
+    def remove_function(self, function_name: str):
+        """
+        Removes a function from the Library instance.
+
+        Args:
+            function_name (str): The name of the function to remove.
+
+        Raises:
+            KeyError: If the specified function name is not found.
+        """
+        if function_name not in self.function_mapping:
+            raise KeyError(f"Function '{function_name}' not found.")
+
+        del self.function_mapping[function_name]
+
+    def execute_function(self, function_name: str, arguments: str):
+        """
+        Executes a specific function based on the given function name and arguments.
+
+        Args:
+            function_name (str): The name of the function to execute.
+            arguments (str): The JSON-formatted arguments for the function.
+
+        Returns:
+            Any: The result of executing the function.
+
+        Raises:
+            KeyError: If the specified function name is not found.
+        """
+        if function_name not in self.function_mapping:
+            raise KeyError(f"Function '{function_name}' not found.")
+
+        function = self.function_mapping[function_name]
+        parsed_arguments = json.loads(arguments)
+
+        # Execute the function with the parsed arguments
+        return self._execute(function, parsed_arguments)
+
+    def _execute(self, function: Function, arguments: dict):
+        """
+        Executes a function with the provided arguments.
+
+        Args:
+            function (Function): The Function instance to execute.
+            arguments (dict): The parsed arguments for the function.
+
+        Returns:
+            Any: The result of executing the function.
+        """
+        # Prepare the function arguments
+        function_arguments = {}
+
+        for parameter in function.parameters:
+            if parameter.name not in arguments:
+                if parameter.required:
+                    raise ValueError(f"Missing required argument '{parameter.name}' for function '{function.name}'.")
+                continue
+
+            function_arguments[parameter.name] = arguments[parameter.name]
+
+        # Execute the function
+        # Replace the print statement with your desired implementation
+        function_to_call = globals()[function.name]
+        return function_to_call(**function_arguments)    
+
+    def get_function_list(self):
+        """
+        Returns a list of Function instances as dictionaries.
+
+        Returns:
+            List[dict]: A list of dictionaries, each representing a Function instance.
+        """
+        function_list = []
+        for function in self.function_mapping.values():
+            function_list.append(function.to_dict())
+        return function_list
```

### Comparing `gpt_functions-0.0.4/.gitignore` & `gpt_functions-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `gpt_functions-0.0.4/LICENSE` & `gpt_functions-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `gpt_functions-0.0.4/README.md` & `gpt_functions-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `gpt_functions-0.0.4/pyproject.toml` & `gpt_functions-0.0.5/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "gpt_functions"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Lindo Khoza", email="willkhoza@gmail.com" },
   { name="Emito Khoza", email="emito.khoza@gmail.com"}
 ]
 description = "A Python package that provides a simple interface for producing function data in a structured format for the OpenAI GPT models."
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `gpt_functions-0.0.4/PKG-INFO` & `gpt_functions-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt_functions
-Version: 0.0.4
+Version: 0.0.5
 Summary: A Python package that provides a simple interface for producing function data in a structured format for the OpenAI GPT models.
 Project-URL: Homepage, https://github.com/willkhoza/gpt_functions
 Project-URL: Bug Tracker, https://github.com/willkhoza/gpt_functions/issues
 Author-email: Lindo Khoza <willkhoza@gmail.com>, Emito Khoza <emito.khoza@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

