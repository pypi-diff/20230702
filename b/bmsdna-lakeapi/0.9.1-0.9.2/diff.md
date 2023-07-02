# Comparing `tmp/bmsdna_lakeapi-0.9.1.tar.gz` & `tmp/bmsdna_lakeapi-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bmsdna_lakeapi-0.9.1.tar", max compression
+gzip compressed data, was "bmsdna_lakeapi-0.9.2.tar", max compression
```

## Comparing `bmsdna_lakeapi-0.9.1.tar` & `bmsdna_lakeapi-0.9.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0     1081 2023-07-02 09:04:36.989733 bmsdna_lakeapi-0.9.1/LICENSE
--rw-r--r--   0        0        0     9068 2023-07-02 09:04:36.989733 bmsdna_lakeapi-0.9.1/README.md
--rw-r--r--   0        0        0      380 2023-07-02 09:04:36.989733 bmsdna_lakeapi-0.9.1/bmsdna/lakeapi/__init__.py
--rw-r--r--   0        0        0        0 2023-07-02 09:04:36.989733 bmsdna_lakeapi-0.9.1/bmsdna/lakeapi/api/__init__.py
--rw-r--r--   0        0        0     1138 2023-07-02 09:04:36.989733 bmsdna_lakeapi-0.9.1/bmsdna/lakeapi/api/api.py
--rw-r--r--   0        0        0      625 2023-07-02 09:04:36.993734 bmsdna_lakeapi-0.9.1/bmsdna/lakeapi/context/__init__.py
--rw-r--r--   0        0        0     7186 2023-07-02 09:04:36.993734 bmsdna_lakeapi-0.9.1/bmsdna/lakeapi/context/df_base.py
--rw-r--r--   0        0        0    10634 2023-07-02 09:04:36.993734 bmsdna_lakeapi-0.9.1/bmsdna/lakeapi/context/df_duckdb.py
--rw-r--r--   0        0        0     6256 2023-07-02 09:04:36.993734 bmsdna_lakeapi-0.9.1/bmsdna/lakeapi/context/df_polars.py
--rw-r--r--   0        0        0        0 2023-07-02 09:04:36.993734 bmsdna_lakeapi-0.9.1/bmsdna/lakeapi/core/__init__.py
--rw-r--r--   0        0        0    11183 2023-07-02 09:04:36.993734 bmsdna_lakeapi-0.9.1/bmsdna/lakeapi/core/config.py
--rw-r--r--   0        0        0    12623 2023-07-02 09:04:36.993734 bmsdna_lakeapi-0.9.1/bmsdna/lakeapi/core/datasource.py
--rw-r--r--   0        0        0     6839 2023-07-02 09:04:36.993734 bmsdna_lakeapi-0.9.1/bmsdna/lakeapi/core/detail_endpoint.py
--rw-r--r--   0        0        0     9907 2023-07-02 09:04:36.993734 bmsdna_lakeapi-0.9.1/bmsdna/lakeapi/core/endpoint.py
--rw-r--r--   0        0        0      187 2023-07-02 09:04:36.993734 bmsdna_lakeapi-0.9.1/bmsdna/lakeapi/core/env.py
--rw-r--r--   0        0        0     1012 2023-07-02 09:04:36.993734 bmsdna_lakeapi-0.9.1/bmsdna/lakeapi/core/log.py
--rw-r--r--   0        0        0     6891 2023-07-02 09:04:36.993734 bmsdna_lakeapi-0.9.1/bmsdna/lakeapi/core/model.py
--rw-r--r--   0        0        0     1479 2023-07-02 09:04:36.993734 bmsdna_lakeapi-0.9.1/bmsdna/lakeapi/core/partition_utils.py
--rw-r--r--   0        0        0     6813 2023-07-02 09:04:36.993734 bmsdna_lakeapi-0.9.1/bmsdna/lakeapi/core/response.py
--rw-r--r--   0        0        0     4443 2023-07-02 09:04:36.993734 bmsdna_lakeapi-0.9.1/bmsdna/lakeapi/core/route.py
--rw-r--r--   0        0        0     3770 2023-07-02 09:04:36.993734 bmsdna_lakeapi-0.9.1/bmsdna/lakeapi/core/sql_endpoint.py
--rw-r--r--   0        0        0     3040 2023-07-02 09:04:36.993734 bmsdna_lakeapi-0.9.1/bmsdna/lakeapi/core/types.py
--rw-r--r--   0        0        0     2409 2023-07-02 09:04:36.993734 bmsdna_lakeapi-0.9.1/bmsdna/lakeapi/core/uservalidation.py
--rw-r--r--   0        0        0      215 2023-07-02 09:04:36.993734 bmsdna_lakeapi-0.9.1/bmsdna/lakeapi/core/yaml.py
--rw-r--r--   0        0        0        0 2023-07-02 09:04:36.993734 bmsdna_lakeapi-0.9.1/bmsdna/lakeapi/polars_extensions/__init__.py
--rw-r--r--   0        0        0     1837 2023-07-02 09:04:36.993734 bmsdna_lakeapi-0.9.1/bmsdna/lakeapi/polars_extensions/delta.py
--rw-r--r--   0        0        0      339 2023-07-02 09:04:36.993734 bmsdna_lakeapi-0.9.1/bmsdna/lakeapi/standalone/__init__.py
--rw-r--r--   0        0        0     1784 2023-07-02 09:04:36.993734 bmsdna_lakeapi-0.9.1/bmsdna/lakeapi/tools/useradd.py
--rw-r--r--   0        0        0     1084 2023-07-02 09:04:36.993734 bmsdna_lakeapi-0.9.1/bmsdna/lakeapi/tools/validateschema.py
--rw-r--r--   0        0        0     3535 2023-07-02 09:04:36.993734 bmsdna_lakeapi-0.9.1/bmsdna/lakeapi/utils/fast_api_utils.py
--rw-r--r--   0        0        0     2017 2023-07-02 09:04:36.993734 bmsdna_lakeapi-0.9.1/pyproject.toml
--rw-r--r--   0        0        0    10267 1970-01-01 00:00:00.000000 bmsdna_lakeapi-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-07-02 18:19:02.131434 bmsdna_lakeapi-0.9.2/LICENSE
+-rw-r--r--   0        0        0     9068 2023-07-02 18:19:02.131434 bmsdna_lakeapi-0.9.2/README.md
+-rw-r--r--   0        0        0      380 2023-07-02 18:19:02.131434 bmsdna_lakeapi-0.9.2/bmsdna/lakeapi/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-02 18:19:02.131434 bmsdna_lakeapi-0.9.2/bmsdna/lakeapi/api/__init__.py
+-rw-r--r--   0        0        0     1138 2023-07-02 18:19:02.131434 bmsdna_lakeapi-0.9.2/bmsdna/lakeapi/api/api.py
+-rw-r--r--   0        0        0      625 2023-07-02 18:19:02.131434 bmsdna_lakeapi-0.9.2/bmsdna/lakeapi/context/__init__.py
+-rw-r--r--   0        0        0     7186 2023-07-02 18:19:02.131434 bmsdna_lakeapi-0.9.2/bmsdna/lakeapi/context/df_base.py
+-rw-r--r--   0        0        0    10634 2023-07-02 18:19:02.131434 bmsdna_lakeapi-0.9.2/bmsdna/lakeapi/context/df_duckdb.py
+-rw-r--r--   0        0        0     6256 2023-07-02 18:19:02.131434 bmsdna_lakeapi-0.9.2/bmsdna/lakeapi/context/df_polars.py
+-rw-r--r--   0        0        0        0 2023-07-02 18:19:02.131434 bmsdna_lakeapi-0.9.2/bmsdna/lakeapi/core/__init__.py
+-rw-r--r--   0        0        0    11183 2023-07-02 18:19:02.131434 bmsdna_lakeapi-0.9.2/bmsdna/lakeapi/core/config.py
+-rw-r--r--   0        0        0    12584 2023-07-02 18:19:02.131434 bmsdna_lakeapi-0.9.2/bmsdna/lakeapi/core/datasource.py
+-rw-r--r--   0        0        0     6839 2023-07-02 18:19:02.131434 bmsdna_lakeapi-0.9.2/bmsdna/lakeapi/core/detail_endpoint.py
+-rw-r--r--   0        0        0     9907 2023-07-02 18:19:02.131434 bmsdna_lakeapi-0.9.2/bmsdna/lakeapi/core/endpoint.py
+-rw-r--r--   0        0        0      187 2023-07-02 18:19:02.131434 bmsdna_lakeapi-0.9.2/bmsdna/lakeapi/core/env.py
+-rw-r--r--   0        0        0     1012 2023-07-02 18:19:02.131434 bmsdna_lakeapi-0.9.2/bmsdna/lakeapi/core/log.py
+-rw-r--r--   0        0        0     6891 2023-07-02 18:19:02.131434 bmsdna_lakeapi-0.9.2/bmsdna/lakeapi/core/model.py
+-rw-r--r--   0        0        0     1479 2023-07-02 18:19:02.131434 bmsdna_lakeapi-0.9.2/bmsdna/lakeapi/core/partition_utils.py
+-rw-r--r--   0        0        0     6813 2023-07-02 18:19:02.131434 bmsdna_lakeapi-0.9.2/bmsdna/lakeapi/core/response.py
+-rw-r--r--   0        0        0     4443 2023-07-02 18:19:02.131434 bmsdna_lakeapi-0.9.2/bmsdna/lakeapi/core/route.py
+-rw-r--r--   0        0        0     3770 2023-07-02 18:19:02.131434 bmsdna_lakeapi-0.9.2/bmsdna/lakeapi/core/sql_endpoint.py
+-rw-r--r--   0        0        0     3040 2023-07-02 18:19:02.135434 bmsdna_lakeapi-0.9.2/bmsdna/lakeapi/core/types.py
+-rw-r--r--   0        0        0     2409 2023-07-02 18:19:02.135434 bmsdna_lakeapi-0.9.2/bmsdna/lakeapi/core/uservalidation.py
+-rw-r--r--   0        0        0      215 2023-07-02 18:19:02.135434 bmsdna_lakeapi-0.9.2/bmsdna/lakeapi/core/yaml.py
+-rw-r--r--   0        0        0        0 2023-07-02 18:19:02.135434 bmsdna_lakeapi-0.9.2/bmsdna/lakeapi/polars_extensions/__init__.py
+-rw-r--r--   0        0        0     1837 2023-07-02 18:19:02.135434 bmsdna_lakeapi-0.9.2/bmsdna/lakeapi/polars_extensions/delta.py
+-rw-r--r--   0        0        0      339 2023-07-02 18:19:02.135434 bmsdna_lakeapi-0.9.2/bmsdna/lakeapi/standalone/__init__.py
+-rw-r--r--   0        0        0     1784 2023-07-02 18:19:02.135434 bmsdna_lakeapi-0.9.2/bmsdna/lakeapi/tools/useradd.py
+-rw-r--r--   0        0        0     1084 2023-07-02 18:19:02.135434 bmsdna_lakeapi-0.9.2/bmsdna/lakeapi/tools/validateschema.py
+-rw-r--r--   0        0        0     3535 2023-07-02 18:19:02.135434 bmsdna_lakeapi-0.9.2/bmsdna/lakeapi/utils/fast_api_utils.py
+-rw-r--r--   0        0        0     2017 2023-07-02 18:19:02.135434 bmsdna_lakeapi-0.9.2/pyproject.toml
+-rw-r--r--   0        0        0    10267 1970-01-01 00:00:00.000000 bmsdna_lakeapi-0.9.2/PKG-INFO
```

### Comparing `bmsdna_lakeapi-0.9.1/LICENSE` & `bmsdna_lakeapi-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.9.1/README.md` & `bmsdna_lakeapi-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.9.1/bmsdna/lakeapi/api/api.py` & `bmsdna_lakeapi-0.9.2/bmsdna/lakeapi/api/api.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.9.1/bmsdna/lakeapi/context/__init__.py` & `bmsdna_lakeapi-0.9.2/bmsdna/lakeapi/context/__init__.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.9.1/bmsdna/lakeapi/context/df_base.py` & `bmsdna_lakeapi-0.9.2/bmsdna/lakeapi/context/df_base.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.9.1/bmsdna/lakeapi/context/df_duckdb.py` & `bmsdna_lakeapi-0.9.2/bmsdna/lakeapi/context/df_duckdb.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.9.1/bmsdna/lakeapi/context/df_polars.py` & `bmsdna_lakeapi-0.9.2/bmsdna/lakeapi/context/df_polars.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.9.1/bmsdna/lakeapi/core/config.py` & `bmsdna_lakeapi-0.9.2/bmsdna/lakeapi/core/config.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.9.1/bmsdna/lakeapi/core/datasource.py` & `bmsdna_lakeapi-0.9.2/bmsdna/lakeapi/core/datasource.py`

 * *Files 4% similar despite different names*

```diff
@@ -243,14 +243,18 @@
             if inner_expr is None:
                 inner_expr = pypika.Field(ck) == cv if cv or cv == 0 else pypika.Field(ck).isnull()
             else:
                 inner_expr = inner_expr & (pypika.Field(ck) == cv if cv or cv == 0 else pypika.Field(ck).isnull())
     return inner_expr
 
 
+def flatten(l):
+    return [item for sublist in l for item in sublist]
+
+
 @cache
 async def filter_df_based_on_params(
     params: dict[str, Any],
     param_def: list[Union[Param, str]],
     columns: Optional[list[str]],
 ) -> Optional[pypika.Criterion]:
     expr: Optional[pypika.Criterion] = None
@@ -262,28 +266,24 @@
         prmdef_and_op = await get_param_def(key, param_def)
         if prmdef_and_op is None:
             raise ValueError(f"thats not parameter: {key}")
         prmdef, op = prmdef_and_op
         colname = prmdef.colname or prmdef.name
 
         if prmdef.combi:
-            outer_expr: Optional[pypika.Criterion] = None
-            tasks = []
-            for e in value:
-                task = asyncio.create_task(_create_inner_expr(columns, prmdef, e))
-                tasks.append(task)
-            results = await asyncio.gather(*tasks)
-            for inner_expr in results:
-                if inner_expr is not None:
-                    if outer_expr is None:
-                        outer_expr = inner_expr
-                    else:
-                        outer_expr = outer_expr | (inner_expr)
-            if outer_expr is not None:
-                exprs.append(outer_expr)
+            from pypika import functions as F
+
+            null_string = "###%$**###"
+            combi_params = [c for c in prmdef.combi]
+            search_keys = [(",".join([str(v.get(c, null_string)) for c in combi_params])) for v in value]
+            concats = flatten(list(zip([fn.Field(c) for c in combi_params], [","] * len(combi_params))))[:-1]
+            expr = F.Concat(*concats).as_("__combi_field_search").isin(search_keys)
+
+            if expr is not None:
+                exprs.append(expr)
 
         elif columns and not colname in columns:
             pass
 
         else:
             match op:
                 case "<":
```

### Comparing `bmsdna_lakeapi-0.9.1/bmsdna/lakeapi/core/detail_endpoint.py` & `bmsdna_lakeapi-0.9.2/bmsdna/lakeapi/core/detail_endpoint.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.9.1/bmsdna/lakeapi/core/endpoint.py` & `bmsdna_lakeapi-0.9.2/bmsdna/lakeapi/core/endpoint.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.9.1/bmsdna/lakeapi/core/log.py` & `bmsdna_lakeapi-0.9.2/bmsdna/lakeapi/core/log.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.9.1/bmsdna/lakeapi/core/model.py` & `bmsdna_lakeapi-0.9.2/bmsdna/lakeapi/core/model.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.9.1/bmsdna/lakeapi/core/partition_utils.py` & `bmsdna_lakeapi-0.9.2/bmsdna/lakeapi/core/partition_utils.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.9.1/bmsdna/lakeapi/core/response.py` & `bmsdna_lakeapi-0.9.2/bmsdna/lakeapi/core/response.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.9.1/bmsdna/lakeapi/core/route.py` & `bmsdna_lakeapi-0.9.2/bmsdna/lakeapi/core/route.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.9.1/bmsdna/lakeapi/core/sql_endpoint.py` & `bmsdna_lakeapi-0.9.2/bmsdna/lakeapi/core/sql_endpoint.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.9.1/bmsdna/lakeapi/core/types.py` & `bmsdna_lakeapi-0.9.2/bmsdna/lakeapi/core/types.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.9.1/bmsdna/lakeapi/core/uservalidation.py` & `bmsdna_lakeapi-0.9.2/bmsdna/lakeapi/core/uservalidation.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.9.1/bmsdna/lakeapi/polars_extensions/delta.py` & `bmsdna_lakeapi-0.9.2/bmsdna/lakeapi/polars_extensions/delta.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.9.1/bmsdna/lakeapi/tools/useradd.py` & `bmsdna_lakeapi-0.9.2/bmsdna/lakeapi/tools/useradd.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.9.1/bmsdna/lakeapi/tools/validateschema.py` & `bmsdna_lakeapi-0.9.2/bmsdna/lakeapi/tools/validateschema.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.9.1/bmsdna/lakeapi/utils/fast_api_utils.py` & `bmsdna_lakeapi-0.9.2/bmsdna/lakeapi/utils/fast_api_utils.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.9.1/pyproject.toml` & `bmsdna_lakeapi-0.9.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bmsdna-lakeapi"
-version = "0.9.1"
+version = "0.9.2"
 description = ""
 authors = ["DWH Team <you@example.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "bmsdna"}]
 
 [tool.poetry.dependencies]
```

### Comparing `bmsdna_lakeapi-0.9.1/PKG-INFO` & `bmsdna_lakeapi-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bmsdna-lakeapi
-Version: 0.9.1
+Version: 0.9.2
 Summary: 
 License: MIT
 Author: DWH Team
 Author-email: you@example.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

