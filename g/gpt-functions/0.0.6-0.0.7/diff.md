# Comparing `tmp/gpt_functions-0.0.6.tar.gz` & `tmp/gpt_functions-0.0.7.tar.gz`

## Comparing `gpt_functions-0.0.6.tar` & `gpt_functions-0.0.7.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gpt_functions-0.0.6/src/gpt_functions/__init__.py
--rw-r--r--   0        0        0    10817 2020-02-02 00:00:00.000000 gpt_functions-0.0.6/src/gpt_functions/meta.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 gpt_functions-0.0.6/.gitignore
--rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 gpt_functions-0.0.6/LICENSE
--rw-r--r--   0        0        0    14708 2020-02-02 00:00:00.000000 gpt_functions-0.0.6/README.md
--rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 gpt_functions-0.0.6/pyproject.toml
--rw-r--r--   0        0        0    15361 2020-02-02 00:00:00.000000 gpt_functions-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gpt_functions-0.0.7/src/gpt_functions/__init__.py
+-rw-r--r--   0        0        0    10814 2020-02-02 00:00:00.000000 gpt_functions-0.0.7/src/gpt_functions/meta.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 gpt_functions-0.0.7/.gitignore
+-rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 gpt_functions-0.0.7/LICENSE
+-rw-r--r--   0        0        0    14708 2020-02-02 00:00:00.000000 gpt_functions-0.0.7/README.md
+-rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 gpt_functions-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0    15361 2020-02-02 00:00:00.000000 gpt_functions-0.0.7/PKG-INFO
```

### Comparing `gpt_functions-0.0.6/src/gpt_functions/meta.py` & `gpt_functions-0.0.7/src/gpt_functions/meta.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 
         Returns:
             str: The string representation of the Function instance.
         """
         if self.parameters is None:
             return f"Function(name={self.name}, description={self.description})"
         else:
-            return f"Function(name={self.name}, description={self.description}, parameters={[parameter.name for parameter in self.parameters]}"
+            return f"Function(name={self.name}, description={self.description}, parameters={[parameter.name for parameter in self.parameters]})"
 
     def to_dict(self) -> dict:
         """
         Converts the Function instance to a dictionary.
 
         Returns:
             dict: The Function instance as a dictionary.
@@ -277,17 +277,18 @@
                 if parameter.required:
                     raise ValueError(f"Missing required argument '{parameter.name}' for function '{function.name}'.")
                 continue
 
             function_arguments[parameter.name] = arguments[parameter.name]
 
         # Execute the function
-        # Replace the print statement with your desired implementation
-        function_to_call = globals()[function.name]
-        return function_to_call(**function_arguments)    
+        caller_globals = inspect.currentframe().f_back.f_globals
+        function_to_call = caller_globals[function.name]
+        return function_to_call(**function_arguments)
+
 
     def get_function_list(self):
         """
         Returns a list of Function instances as dictionaries.
 
         Returns:
             List[dict]: A list of dictionaries, each representing a Function instance.
```

### Comparing `gpt_functions-0.0.6/.gitignore` & `gpt_functions-0.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `gpt_functions-0.0.6/LICENSE` & `gpt_functions-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `gpt_functions-0.0.6/README.md` & `gpt_functions-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `gpt_functions-0.0.6/pyproject.toml` & `gpt_functions-0.0.7/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "gpt_functions"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="Lindo Khoza", email="willkhoza@gmail.com" },
   { name="Emito Khoza", email="emito.khoza@gmail.com"}
 ]
 description = "A Python package that provides a simple interface for producing function data in a structured format for the OpenAI GPT models."
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `gpt_functions-0.0.6/PKG-INFO` & `gpt_functions-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt_functions
-Version: 0.0.6
+Version: 0.0.7
 Summary: A Python package that provides a simple interface for producing function data in a structured format for the OpenAI GPT models.
 Project-URL: Homepage, https://github.com/willkhoza/gpt_functions
 Project-URL: Bug Tracker, https://github.com/willkhoza/gpt_functions/issues
 Author-email: Lindo Khoza <willkhoza@gmail.com>, Emito Khoza <emito.khoza@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

