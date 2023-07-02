# Comparing `tmp/pysigma_backend_sentinelone-0.1.1.tar.gz` & `tmp/pysigma_backend_sentinelone-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysigma_backend_sentinelone-0.1.1.tar", max compression
+gzip compressed data, was "pysigma_backend_sentinelone-0.1.2.tar", max compression
```

## Comparing `pysigma_backend_sentinelone-0.1.1.tar` & `pysigma_backend_sentinelone-0.1.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1067 2023-04-29 03:10:09.489647 pysigma_backend_sentinelone-0.1.1/LICENSE
--rw-r--r--   0        0        0      574 2023-04-29 03:10:09.489647 pysigma_backend_sentinelone-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       98 2023-04-29 03:10:09.489647 pysigma_backend_sentinelone-0.1.1/sigma/backends/sentinelone/__init__.py
--rw-r--r--   0        0        0     7792 2023-04-29 03:10:09.489647 pysigma_backend_sentinelone-0.1.1/sigma/backends/sentinelone/sentinelone.py
--rw-r--r--   0        0        0      112 2023-04-29 03:10:09.489647 pysigma_backend_sentinelone-0.1.1/sigma/pipelines/sentinelone/__init__.py
--rw-r--r--   0        0        0    14568 2023-04-29 03:10:09.489647 pysigma_backend_sentinelone-0.1.1/sigma/pipelines/sentinelone/sentinelone.py
--rw-r--r--   0        0        0      696 1970-01-01 00:00:00.000000 pysigma_backend_sentinelone-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-07-02 00:15:33.890138 pysigma_backend_sentinelone-0.1.2/LICENSE
+-rw-r--r--   0        0        0      574 2023-07-02 00:15:33.890138 pysigma_backend_sentinelone-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0       98 2023-07-02 00:15:33.890138 pysigma_backend_sentinelone-0.1.2/sigma/backends/sentinelone/__init__.py
+-rw-r--r--   0        0        0     7792 2023-07-02 00:15:33.890138 pysigma_backend_sentinelone-0.1.2/sigma/backends/sentinelone/sentinelone.py
+-rw-r--r--   0        0        0      112 2023-07-02 00:15:33.890138 pysigma_backend_sentinelone-0.1.2/sigma/pipelines/sentinelone/__init__.py
+-rw-r--r--   0        0        0    15072 2023-07-02 00:15:33.890138 pysigma_backend_sentinelone-0.1.2/sigma/pipelines/sentinelone/sentinelone.py
+-rw-r--r--   0        0        0      696 1970-01-01 00:00:00.000000 pysigma_backend_sentinelone-0.1.2/PKG-INFO
```

### Comparing `pysigma_backend_sentinelone-0.1.1/LICENSE` & `pysigma_backend_sentinelone-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pysigma_backend_sentinelone-0.1.1/pyproject.toml` & `pysigma_backend_sentinelone-0.1.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pySigma-backend-sentinelone"
-version = "0.1.1"
+version = "0.1.2"
 description = "pySigma SentinelOne backend"
 authors = ["Cori Smith <cs2718281@gmail.com>"]
 license = "MIT"
 repository = "https://github.com/7RedViolin/pySigma-backend-sentinelone"
 packages = [
     { include = "sigma" }
 ]
```

### Comparing `pysigma_backend_sentinelone-0.1.1/sigma/backends/sentinelone/sentinelone.py` & `pysigma_backend_sentinelone-0.1.2/sigma/backends/sentinelone/sentinelone.py`

 * *Files identical despite different names*

### Comparing `pysigma_backend_sentinelone-0.1.1/sigma/pipelines/sentinelone/sentinelone.py` & `pysigma_backend_sentinelone-0.1.2/sigma/pipelines/sentinelone/sentinelone.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,14 +12,25 @@
     """
 
     def apply_detection_item(self, detection_item: SigmaDetectionItem) -> None:
         field_name = detection_item.field
         self.message = f"Invalid SigmaDetectionItem field name encountered: {field_name}. " + self.message
         raise SigmaTransformationError(self.message)
 
+
+def _flatten(items, seqtypes=(list, tuple)):
+    """Private function to flatten lists for Field mapping errors"""
+    try:
+        for i, x in enumerate(items):
+            while isinstance(items[i], seqtypes):
+                items[i:i+1] = items[i]
+    except IndexError:
+        pass
+    return items
+
 def sentinelone_pipeline() -> ProcessingPipeline:
 
     general_supported_fields = [
         'ObjectType',
         'EventType'
     ]
 
@@ -358,17 +369,23 @@
         )
     ]
 
     unsupported_field_name = [
         ProcessingItem(
             identifier='s1_fail_field_not_supported',
             transformation=InvalidFieldTransformation("This pipeline only supports the following fields:\n{" + 
-            '}, {'.join(sorted(set(sum([list(translation_dict[x].keys()) for x in translation_dict.keys()],[])))) + '}'),
+            '}, {'.join(sorted(set(
+                list(_flatten([[k,v] for t in translation_dict.keys() for k, v in
+                               translation_dict[t].items()])) + general_supported_fields
+            )))),
             field_name_conditions=[
-                ExcludeFieldCondition(fields=list(set(sum([list(translation_dict[x].keys()) for x in translation_dict.keys()],[]))) + general_supported_fields)
+                ExcludeFieldCondition(fields=list(set(
+                    list(_flatten([[k, v] for t in translation_dict.keys() for k, v in
+                                   translation_dict[t].items()])) + general_supported_fields
+                )))
             ]
         )
     ]
 
     return ProcessingPipeline(
         name="SentinelOne pipeline",
         priority=50,
```

### Comparing `pysigma_backend_sentinelone-0.1.1/PKG-INFO` & `pysigma_backend_sentinelone-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysigma-backend-sentinelone
-Version: 0.1.1
+Version: 0.1.2
 Summary: pySigma SentinelOne backend
 Home-page: https://github.com/7RedViolin/pySigma-backend-sentinelone
 License: MIT
 Author: Cori Smith
 Author-email: cs2718281@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

