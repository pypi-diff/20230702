# Comparing `tmp/stability_matrix_tools-0.1.8.tar.gz` & `tmp/stability_matrix_tools-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stability_matrix_tools-0.1.8.tar", max compression
+gzip compressed data, was "stability_matrix_tools-0.1.9.tar", max compression
```

## Comparing `stability_matrix_tools-0.1.8.tar` & `stability_matrix_tools-0.1.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0    35163 2023-06-30 22:15:25.032480 stability_matrix_tools-0.1.8/LICENSE
--rw-r--r--   0        0        0      632 2023-07-02 05:02:27.430441 stability_matrix_tools-0.1.8/pyproject.toml
--rw-r--r--   0        0        0       47 2023-06-30 22:15:24.995957 stability_matrix_tools-0.1.8/README.md
--rw-r--r--   0        0        0        0 2023-06-30 19:14:24.481835 stability_matrix_tools-0.1.8/src/stability_matrix_tools/__init__.py
--rw-r--r--   0        0        0     2329 2023-07-01 03:50:14.086249 stability_matrix_tools-0.1.8/src/stability_matrix_tools/b2.py
--rw-r--r--   0        0        0      380 2023-07-01 04:29:55.594056 stability_matrix_tools-0.1.8/src/stability_matrix_tools/cf.py
--rw-r--r--   0        0        0     3068 2023-07-01 07:09:28.831003 stability_matrix_tools-0.1.8/src/stability_matrix_tools/keys.py
--rw-r--r--   0        0        0      245 2023-07-01 06:42:59.756522 stability_matrix_tools-0.1.8/src/stability_matrix_tools/main.py
--rw-r--r--   0        0        0        0 2023-06-30 19:29:16.679181 stability_matrix_tools-0.1.8/src/stability_matrix_tools/models/__init__.py
--rw-r--r--   0        0        0      518 2023-07-01 03:35:42.001028 stability_matrix_tools-0.1.8/src/stability_matrix_tools/models/settings.py
--rw-r--r--   0        0        0     1529 2023-07-02 05:02:18.271653 stability_matrix_tools-0.1.8/src/stability_matrix_tools/models/update_info.py
--rw-r--r--   0        0        0      325 2023-06-30 21:06:10.076637 stability_matrix_tools-0.1.8/src/stability_matrix_tools/models/version.py
--rw-r--r--   0        0        0     5371 2023-07-01 09:09:16.670644 stability_matrix_tools-0.1.8/src/stability_matrix_tools/updates.py
--rw-r--r--   0        0        0        0 2023-07-01 02:42:39.117279 stability_matrix_tools-0.1.8/src/stability_matrix_tools/utils/__init__.py
--rw-r--r--   0        0        0      588 2023-07-01 04:29:34.632450 stability_matrix_tools-0.1.8/src/stability_matrix_tools/utils/cf_cache.py
--rw-r--r--   0        0        0     1634 2023-06-30 21:18:44.596055 stability_matrix_tools-0.1.8/src/stability_matrix_tools/utils/progress.py
--rw-r--r--   0        0        0     1948 2023-07-01 06:57:32.338302 stability_matrix_tools-0.1.8/src/stability_matrix_tools/utils/signing.py
--rw-r--r--   0        0        0      709 2023-07-01 08:56:22.308456 stability_matrix_tools-0.1.8/src/stability_matrix_tools/utils/stream_hash.py
--rw-r--r--   0        0        0     2051 2023-07-01 08:34:51.103754 stability_matrix_tools-0.1.8/src/stability_matrix_tools/utils/uploader.py
--rw-r--r--   0        0        0     1162 1970-01-01 00:00:00.000000 stability_matrix_tools-0.1.8/setup.py
--rw-r--r--   0        0        0      811 1970-01-01 00:00:00.000000 stability_matrix_tools-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0    35163 2023-06-30 22:15:25.032480 stability_matrix_tools-0.1.9/LICENSE
+-rw-r--r--   0        0        0      632 2023-07-02 05:05:03.292780 stability_matrix_tools-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0       47 2023-06-30 22:15:24.995957 stability_matrix_tools-0.1.9/README.md
+-rw-r--r--   0        0        0        0 2023-06-30 19:14:24.481835 stability_matrix_tools-0.1.9/src/stability_matrix_tools/__init__.py
+-rw-r--r--   0        0        0     2329 2023-07-01 03:50:14.086249 stability_matrix_tools-0.1.9/src/stability_matrix_tools/b2.py
+-rw-r--r--   0        0        0      380 2023-07-01 04:29:55.594056 stability_matrix_tools-0.1.9/src/stability_matrix_tools/cf.py
+-rw-r--r--   0        0        0     3068 2023-07-01 07:09:28.831003 stability_matrix_tools-0.1.9/src/stability_matrix_tools/keys.py
+-rw-r--r--   0        0        0      245 2023-07-01 06:42:59.756522 stability_matrix_tools-0.1.9/src/stability_matrix_tools/main.py
+-rw-r--r--   0        0        0        0 2023-06-30 19:29:16.679181 stability_matrix_tools-0.1.9/src/stability_matrix_tools/models/__init__.py
+-rw-r--r--   0        0        0      518 2023-07-01 03:35:42.001028 stability_matrix_tools-0.1.9/src/stability_matrix_tools/models/settings.py
+-rw-r--r--   0        0        0     1529 2023-07-02 05:02:18.271653 stability_matrix_tools-0.1.9/src/stability_matrix_tools/models/update_info.py
+-rw-r--r--   0        0        0      325 2023-06-30 21:06:10.076637 stability_matrix_tools-0.1.9/src/stability_matrix_tools/models/version.py
+-rw-r--r--   0        0        0     5386 2023-07-02 05:05:03.290781 stability_matrix_tools-0.1.9/src/stability_matrix_tools/updates.py
+-rw-r--r--   0        0        0        0 2023-07-01 02:42:39.117279 stability_matrix_tools-0.1.9/src/stability_matrix_tools/utils/__init__.py
+-rw-r--r--   0        0        0      588 2023-07-01 04:29:34.632450 stability_matrix_tools-0.1.9/src/stability_matrix_tools/utils/cf_cache.py
+-rw-r--r--   0        0        0     1634 2023-06-30 21:18:44.596055 stability_matrix_tools-0.1.9/src/stability_matrix_tools/utils/progress.py
+-rw-r--r--   0        0        0     1948 2023-07-01 06:57:32.338302 stability_matrix_tools-0.1.9/src/stability_matrix_tools/utils/signing.py
+-rw-r--r--   0        0        0      709 2023-07-01 08:56:22.308456 stability_matrix_tools-0.1.9/src/stability_matrix_tools/utils/stream_hash.py
+-rw-r--r--   0        0        0     2051 2023-07-01 08:34:51.103754 stability_matrix_tools-0.1.9/src/stability_matrix_tools/utils/uploader.py
+-rw-r--r--   0        0        0     1162 1970-01-01 00:00:00.000000 stability_matrix_tools-0.1.9/setup.py
+-rw-r--r--   0        0        0      811 1970-01-01 00:00:00.000000 stability_matrix_tools-0.1.9/PKG-INFO
```

### Comparing `stability_matrix_tools-0.1.8/LICENSE` & `stability_matrix_tools-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `stability_matrix_tools-0.1.8/pyproject.toml` & `stability_matrix_tools-0.1.9/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "stability-matrix-tools"
-version = "0.1.8"
+version = "0.1.9"
 description = ""
 authors = ["Ionite <dev@ionite.io>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.10, <3.12"
 typer = {extras = ["all"], version = "^0.9.0"}
```

### Comparing `stability_matrix_tools-0.1.8/src/stability_matrix_tools/b2.py` & `stability_matrix_tools-0.1.9/src/stability_matrix_tools/b2.py`

 * *Files identical despite different names*

### Comparing `stability_matrix_tools-0.1.8/src/stability_matrix_tools/keys.py` & `stability_matrix_tools-0.1.9/src/stability_matrix_tools/keys.py`

 * *Files identical despite different names*

### Comparing `stability_matrix_tools-0.1.8/src/stability_matrix_tools/models/settings.py` & `stability_matrix_tools-0.1.9/src/stability_matrix_tools/models/settings.py`

 * *Files identical despite different names*

### Comparing `stability_matrix_tools-0.1.8/src/stability_matrix_tools/models/update_info.py` & `stability_matrix_tools-0.1.9/src/stability_matrix_tools/models/update_info.py`

 * *Files identical despite different names*

### Comparing `stability_matrix_tools-0.1.8/src/stability_matrix_tools/updates.py` & `stability_matrix_tools-0.1.9/src/stability_matrix_tools/updates.py`

 * *Files 1% similar despite different names*

```diff
@@ -147,15 +147,15 @@
         changelog=changelog,
         hashBlake3=hash_blake3,
         signature=signature,
         type=update_type,
     )
 
     # Print and ask for confirmation
-    json = info.model_dump_json(indent=4)
+    json = info.model_dump_json(indent=4, by_alias=True)
     cp(f"Update Info JSON: {json}")
 
     if not typer.confirm("Publish update?"):
         raise typer.Abort()
 
     # Save json to a temporary file
     with TemporaryDirectory() as temp_dir:
```

### Comparing `stability_matrix_tools-0.1.8/src/stability_matrix_tools/utils/cf_cache.py` & `stability_matrix_tools-0.1.9/src/stability_matrix_tools/utils/cf_cache.py`

 * *Files identical despite different names*

### Comparing `stability_matrix_tools-0.1.8/src/stability_matrix_tools/utils/progress.py` & `stability_matrix_tools-0.1.9/src/stability_matrix_tools/utils/progress.py`

 * *Files identical despite different names*

### Comparing `stability_matrix_tools-0.1.8/src/stability_matrix_tools/utils/signing.py` & `stability_matrix_tools-0.1.9/src/stability_matrix_tools/utils/signing.py`

 * *Files identical despite different names*

### Comparing `stability_matrix_tools-0.1.8/src/stability_matrix_tools/utils/stream_hash.py` & `stability_matrix_tools-0.1.9/src/stability_matrix_tools/utils/stream_hash.py`

 * *Files identical despite different names*

### Comparing `stability_matrix_tools-0.1.8/src/stability_matrix_tools/utils/uploader.py` & `stability_matrix_tools-0.1.9/src/stability_matrix_tools/utils/uploader.py`

 * *Files identical despite different names*

### Comparing `stability_matrix_tools-0.1.8/setup.py` & `stability_matrix_tools-0.1.9/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -25,15 +25,15 @@
  'typer[all]>=0.9.0,<0.10.0']
 
 entry_points = \
 {'console_scripts': ['sm-tools = stability_matrix_tools.main:app']}
 
 setup_kwargs = {
     'name': 'stability-matrix-tools',
-    'version': '0.1.8',
+    'version': '0.1.9',
     'description': '',
     'long_description': '# sm-tools\n Stability Matrix development tools\n',
     'author': 'Ionite',
     'author_email': 'dev@ionite.io',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `stability_matrix_tools-0.1.8/PKG-INFO` & `stability_matrix_tools-0.1.9/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stability-matrix-tools
-Version: 0.1.8
+Version: 0.1.9
 Summary: 
 Author: Ionite
 Author-email: dev@ionite.io
 Requires-Python: >=3.10,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

