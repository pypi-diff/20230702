# Comparing `tmp/wisedata-1.0.8.tar.gz` & `tmp/wisedata-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wisedata-1.0.8.tar", max compression
+gzip compressed data, was "wisedata-1.0.9.tar", max compression
```

## Comparing `wisedata-1.0.8.tar` & `wisedata-1.0.9.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11357 2023-06-16 12:22:48.812559 wisedata-1.0.8/LICENSE
--rw-r--r--   0        0        0     9918 2023-06-27 11:13:55.101088 wisedata-1.0.8/README.md
--rw-r--r--   0        0        0      653 2023-07-02 14:44:58.597399 wisedata-1.0.8/pyproject.toml
--rw-r--r--   0        0        0     8793 2023-07-02 14:44:54.410876 wisedata-1.0.8/wisedata/__init__.py
--rw-r--r--   0        0        0      745 2023-07-02 14:10:35.982308 wisedata-1.0.8/wisedata/exceptions.py
--rw-r--r--   0        0        0    10550 1970-01-01 00:00:00.000000 wisedata-1.0.8/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-16 12:22:48.812559 wisedata-1.0.9/LICENSE
+-rw-r--r--   0        0        0     9918 2023-06-27 11:13:55.101088 wisedata-1.0.9/README.md
+-rw-r--r--   0        0        0      653 2023-07-02 15:02:10.166578 wisedata-1.0.9/pyproject.toml
+-rw-r--r--   0        0        0     8861 2023-07-02 15:01:47.684572 wisedata-1.0.9/wisedata/__init__.py
+-rw-r--r--   0        0        0      745 2023-07-02 14:10:35.982308 wisedata-1.0.9/wisedata/exceptions.py
+-rw-r--r--   0        0        0    10550 1970-01-01 00:00:00.000000 wisedata-1.0.9/PKG-INFO
```

### Comparing `wisedata-1.0.8/LICENSE` & `wisedata-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `wisedata-1.0.8/README.md` & `wisedata-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `wisedata-1.0.8/pyproject.toml` & `wisedata-1.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "wisedata"
-version = "1.0.8"
+version = "1.0.9"
 description = "AI Assistant for Python Data Analytics"
 authors = ["WiseData Team <wisedata.help@gmail.com>"]
 homepage = "https://www.wisedata.app/"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9.0"
```

### Comparing `wisedata-1.0.8/wisedata/__init__.py` & `wisedata-1.0.9/wisedata/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,17 +35,17 @@
       {"customers_df": customers_df, "employees_df": employees_df}
     Code: bool
       Whether to print/log the pandas code used to transformed dataframes or not.
     """
     try:
       return self._sql(query, dataframes, code=code)
     except TranslationError as e:
-      logging.error(f"{e.msg}\nTry to run this code again.")
+      logging.error(f"{e.msg}\nTry to run .sql() again.")
     except WiseDataInternalError as e:
-      logging.error(f"{e.msg}. Try to run this code again.")
+      logging.error(f"{e.msg}. Try to run .sql() again.")
 
   # @retry(exceptions=(RequestException, WiseDataInternalError), tries=3, delay=2)
   def _sql(self, query, dataframes, error=None, code=False, num_retries=0, prev_code=None):
     if not (type(dataframes) is dict): raise Exception("dataframes needs to be a dictionary with key being dataframe name and value being the dataframe.")
     if num_retries >= 2:
       raise TranslationError(f"Here is python code we attempted to generate: \n{prev_code}")
 
@@ -107,20 +107,21 @@
       {"customers_df": customers_df, "employees_df": employees_df}
     Code: bool
       Whether to print/log the pandas code used to generate visualization or not.
     """
     try:
       return self._transform(prompt, dataframes, code=code)
     except TranslationError as e:
-      logging.error(f"{e.msg}\nTry to run this code again.")
+      logging.error(f"{e.msg}\nTry to run .transform() again.")
     except WiseDataInternalError as e:
-      logging.error(f"{e.msg}. Try to run this code again.")
+      logging.error(f"{e.msg}. Try to run .transform() again.")
   
   # @retry(exceptions=(RequestException, WiseDataInternalError), tries=3, delay=2)
   def _transform(self, prompt, dataframes, code=False, error=None, num_retries=0, prev_code=None):
+    if(num_retries > 0): logging.error(f"Retrying with prompt: {prompt}")
     if not (type(dataframes) is dict): raise Exception("dataframes needs to be a dictionary with key being dataframe name and value being the dataframe.")
 
     if num_retries >= 2:
       raise TranslationError(f"Here is python code we attempted to generate: \n{prev_code}")
     
     data = {
       "dataframe": "\n".join([f"{idx+1}. Dataframe named {key} with columns={value.columns.tolist()} {'and index=[' + value.index.name + ']' if value.index.name else ''}." for idx, (key, value) in enumerate(dataframes.items())]),
@@ -179,17 +180,17 @@
       {"customers_df": customers_df, "employees_df": employees_df}
     Code: bool
       Whether to print/log the pandas code used to generate visualization or not.
     """
     try:
       return self._viz(prompt, dataframes, code=code)
     except TranslationError as e:
-      logging.error(f"{e.msg}\nTry to run this code again.")
+      logging.error(f"{e.msg}\nTry to run .viz() again.")
     except WiseDataInternalError as e:
-      logging.error(f"{e.msg}. Try to run this code again.")
+      logging.error(f"{e.msg}. Try to run .viz() again.")
 
   # @retry(exceptions=(RequestException, WiseDataInternalError), tries=3, delay=2)
   def _viz(self, prompt, dataframes, code=False, error=None, num_retries=0, prev_code=None):
     if not (type(dataframes) is dict): raise Exception("dataframes needs to be a dictionary with key being dataframe name and value being the dataframe.")
 
     if num_retries >= 2:
       raise TranslationError(f"Here is python code we attempted to generate: \n{prev_code}")
```

### Comparing `wisedata-1.0.8/wisedata/exceptions.py` & `wisedata-1.0.9/wisedata/exceptions.py`

 * *Files identical despite different names*

### Comparing `wisedata-1.0.8/PKG-INFO` & `wisedata-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wisedata
-Version: 1.0.8
+Version: 1.0.9
 Summary: AI Assistant for Python Data Analytics
 Home-page: https://www.wisedata.app/
 Author: WiseData Team
 Author-email: wisedata.help@gmail.com
 Requires-Python: >=3.9.0,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

