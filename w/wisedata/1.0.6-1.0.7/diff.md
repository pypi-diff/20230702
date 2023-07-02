# Comparing `tmp/wisedata-1.0.6.tar.gz` & `tmp/wisedata-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wisedata-1.0.6.tar", max compression
+gzip compressed data, was "wisedata-1.0.7.tar", max compression
```

## Comparing `wisedata-1.0.6.tar` & `wisedata-1.0.7.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11357 2023-06-16 12:22:48.812559 wisedata-1.0.6/LICENSE
--rw-r--r--   0        0        0     9918 2023-06-27 11:13:55.101088 wisedata-1.0.6/README.md
--rw-r--r--   0        0        0      687 2023-06-28 01:23:50.003491 wisedata-1.0.6/pyproject.toml
--rw-r--r--   0        0        0     8358 2023-06-26 17:46:41.469930 wisedata-1.0.6/wisedata/__init__.py
--rw-r--r--   0        0        0      704 2023-06-26 12:18:32.144558 wisedata-1.0.6/wisedata/exceptions.py
--rw-r--r--   0        0        0    10550 1970-01-01 00:00:00.000000 wisedata-1.0.6/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-16 12:22:48.812559 wisedata-1.0.7/LICENSE
+-rw-r--r--   0        0        0     9918 2023-06-27 11:13:55.101088 wisedata-1.0.7/README.md
+-rw-r--r--   0        0        0      653 2023-07-02 14:23:26.226850 wisedata-1.0.7/pyproject.toml
+-rw-r--r--   0        0        0     8685 2023-07-02 14:20:46.130452 wisedata-1.0.7/wisedata/__init__.py
+-rw-r--r--   0        0        0      745 2023-07-02 14:10:35.982308 wisedata-1.0.7/wisedata/exceptions.py
+-rw-r--r--   0        0        0    10550 1970-01-01 00:00:00.000000 wisedata-1.0.7/PKG-INFO
```

### Comparing `wisedata-1.0.6/LICENSE` & `wisedata-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `wisedata-1.0.6/README.md` & `wisedata-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `wisedata-1.0.6/pyproject.toml` & `wisedata-1.0.7/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 [tool.poetry]
 name = "wisedata"
-version = "1.0.6"
+version = "1.0.7"
 description = "AI Assistant for Python Data Analytics"
 authors = ["WiseData Team <wisedata.help@gmail.com>"]
-url = "https://www.wisedata.app/"
 homepage = "https://www.wisedata.app/"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9.0"
 python-dotenv = "^1.0.0"
 requests = "2.31.0"
```

### Comparing `wisedata-1.0.6/wisedata/__init__.py` & `wisedata-1.0.7/wisedata/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,22 +32,26 @@
       Dictionary of dataframes to be transformed.
       The key is the dataframe name and the value is the dataframe itself.
       Example:
       {"customers_df": customers_df, "employees_df": employees_df}
     Code: bool
       Whether to print/log the pandas code used to transformed dataframes or not.
     """
-    return self._sql(query, dataframes, code=code)
+    try:
+      return self._sql(query, dataframes, code=code)
+    except TranslationError as e:
+      logging.error(e.msg)
+    except WiseDataInternalError as e:
+      logging.error(f"{e.msg}. Try to run this code again.")
 
   @retry(exceptions=(RequestException, WiseDataInternalError), tries=3, delay=2)
   def _sql(self, query, dataframes, error=None, code=False, num_retries=0, prev_code=None):
     if not (type(dataframes) is dict): raise Exception("dataframes needs to be a dictionary with key being dataframe name and value being the dataframe.")
     if num_retries >= 2:
-      logging.error(f"We couldn't translate your query. Here is python code we attempted to generate: \n{prev_code}")
-      raise TranslationError()
+      raise TranslationError(f"Here is python code we attempted to generate: \n{prev_code}")
 
     data = {
       "dataframe": "\n".join([f"{idx+1}. Dataframe named {key} with columns {value.columns.tolist()}" for idx, (key, value) in enumerate(dataframes.items())]),
       "sql": query,
       "error": error
     }
 
@@ -100,23 +104,27 @@
       Dictionary of dataframes to be transformed.
       The key is the dataframe name and the value is the dataframe itself.
       Example:
       {"customers_df": customers_df, "employees_df": employees_df}
     Code: bool
       Whether to print/log the pandas code used to generate visualization or not.
     """
-    return self._transform(prompt, dataframes, code=code)
+    try:
+      return self._transform(prompt, dataframes, code=code)
+    except TranslationError as e:
+      logging.error(e.msg)
+    except WiseDataInternalError as e:
+      logging.error(f"{e.msg}. Try to run this code again.")
   
   @retry(exceptions=(RequestException, WiseDataInternalError), tries=3, delay=2)
   def _transform(self, prompt, dataframes, code=False, error=None, num_retries=0, prev_code=None):
     if not (type(dataframes) is dict): raise Exception("dataframes needs to be a dictionary with key being dataframe name and value being the dataframe.")
 
     if num_retries >= 2:
-      logging.error(f"We couldn't translate your prompt. Here is python code we attempted to generate: \n{prev_code}")
-      raise TranslationError()
+      raise TranslationError(f"Here is python code we attempted to generate: \n{prev_code}")
     
     data = {
       "dataframe": "\n".join([f"{idx+1}. Dataframe named {key} with columns={value.columns.tolist()} {'and index=[' + value.index.name + ']' if value.index.name else ''}." for idx, (key, value) in enumerate(dataframes.items())]),
       "nl": prompt,
       "error": error
     }
 
@@ -168,23 +176,27 @@
       Dictionary of dataframes to be transformed.
       The key is the dataframe name and the value is the dataframe itself.
       Example:
       {"customers_df": customers_df, "employees_df": employees_df}
     Code: bool
       Whether to print/log the pandas code used to generate visualization or not.
     """
-    return self._viz(prompt, dataframes, code=code)
+    try:
+      return self._viz(prompt, dataframes, code=code)
+    except TranslationError as e:
+      logging.error(e.msg)
+    except WiseDataInternalError as e:
+      logging.error(f"{e.msg}. Try to run this code again.")
 
   @retry(exceptions=(RequestException, WiseDataInternalError), tries=3, delay=2)
   def _viz(self, prompt, dataframes, code=False, error=None, num_retries=0, prev_code=None):
     if not (type(dataframes) is dict): raise Exception("dataframes needs to be a dictionary with key being dataframe name and value being the dataframe.")
 
     if num_retries >= 2:
-      logging.error(f"We couldn't translate your prompt into visualization. Here is python code we attempted to generate: \n{prev_code}")
-      raise TranslationError()
+      raise TranslationError(f"Here is python code we attempted to generate: \n{prev_code}")
     
     data = {
       "dataframe": "\n".join([f"{idx+1}. Dataframe named {key} with columns={value.columns.tolist()} {'and index=[' + value.index.name + ']' if value.index.name else ''}." for idx, (key, value) in enumerate(dataframes.items())]),
       "nl": prompt,
       "error": error
     }
```

### Comparing `wisedata-1.0.6/wisedata/exceptions.py` & `wisedata-1.0.7/wisedata/exceptions.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     self.msg = msg
     super().__init__(f"Error: {self.msg}")
 
 class WiseDataInternalError(WiseDataError):
   """
   Raised when an internal error occurs
   """
-  def __init__(self, error_msg=""):
+  def __init__(self, error_msg="Oops! Something went wrong with WiseData."):
     super().__init__(error_msg)
 
 class BadRequestError(WiseDataError):
   """
   Raised when a bad request happens
   """
   def __init__(self, error_msg=""):
```

### Comparing `wisedata-1.0.6/PKG-INFO` & `wisedata-1.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wisedata
-Version: 1.0.6
+Version: 1.0.7
 Summary: AI Assistant for Python Data Analytics
 Home-page: https://www.wisedata.app/
 Author: WiseData Team
 Author-email: wisedata.help@gmail.com
 Requires-Python: >=3.9.0,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

