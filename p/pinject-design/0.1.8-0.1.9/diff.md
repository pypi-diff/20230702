# Comparing `tmp/pinject-design-0.1.8.tar.gz` & `tmp/pinject-design-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pinject-design-0.1.8.tar", max compression
+gzip compressed data, was "pinject-design-0.1.9.tar", max compression
```

## Comparing `pinject-design-0.1.8.tar` & `pinject-design-0.1.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1066 2022-03-23 09:24:51.954701 pinject-design-0.1.8/LICENSE
--rw-r--r--   0        0        0        0 2022-01-27 17:14:04.355211 pinject-design-0.1.8/pinject_design/__init__.py
--rw-r--r--   0        0        0        0 2021-03-31 10:36:27.000000 pinject-design-0.1.8/pinject_design/di/__init__.py
--rw-r--r--   0        0        0     7144 2022-04-27 08:04:25.209057 pinject-design-0.1.8/pinject_design/di/design.py
--rw-r--r--   0        0        0     2155 2022-01-27 18:10:42.819773 pinject-design-0.1.8/pinject_design/di/graph.py
--rw-r--r--   0        0        0    13823 2022-04-30 05:26:53.150771 pinject-design-0.1.8/pinject_design/di/injected.py
--rw-r--r--   0        0        0      416 2021-07-14 13:45:34.000000 pinject-design-0.1.8/pinject_design/di/provider.py
--rw-r--r--   0        0        0    23372 2022-04-27 10:14:06.845469 pinject-design-0.1.8/pinject_design/di/util.py
--rw-r--r--   0        0        0        0 2022-04-27 03:40:35.011226 pinject-design-0.1.8/pinject_design/viz/__init__.py
--rw-r--r--   0        0        0       78 2022-04-27 03:51:47.513177 pinject-design-0.1.8/pinject_design/viz/graph.py
--rw-r--r--   0        0        0      463 2022-05-01 18:45:20.020953 pinject-design-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      755 2022-05-01 18:45:23.562201 pinject-design-0.1.8/setup.py
--rw-r--r--   0        0        0      703 2022-05-01 18:45:23.562370 pinject-design-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1066 2022-03-23 09:24:51.954701 pinject-design-0.1.9/LICENSE
+-rw-r--r--   0        0        0        0 2022-01-27 17:14:04.355211 pinject-design-0.1.9/pinject_design/__init__.py
+-rw-r--r--   0        0        0        0 2021-03-31 10:36:27.000000 pinject-design-0.1.9/pinject_design/di/__init__.py
+-rw-r--r--   0        0        0     7144 2022-04-27 08:04:25.209057 pinject-design-0.1.9/pinject_design/di/design.py
+-rw-r--r--   0        0        0     2155 2022-01-27 18:10:42.819773 pinject-design-0.1.9/pinject_design/di/graph.py
+-rw-r--r--   0        0        0    13823 2022-04-30 05:26:53.150771 pinject-design-0.1.9/pinject_design/di/injected.py
+-rw-r--r--   0        0        0      416 2021-07-14 13:45:34.000000 pinject-design-0.1.9/pinject_design/di/provider.py
+-rw-r--r--   0        0        0    23372 2022-04-27 10:14:06.845469 pinject-design-0.1.9/pinject_design/di/util.py
+-rw-r--r--   0        0        0        0 2022-04-27 03:40:35.011226 pinject-design-0.1.9/pinject_design/viz/__init__.py
+-rw-r--r--   0        0        0       78 2022-04-27 03:51:47.513177 pinject-design-0.1.9/pinject_design/viz/graph.py
+-rw-r--r--   0        0        0      463 2022-05-01 19:21:00.339822 pinject-design-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      755 2022-05-01 19:21:10.151308 pinject-design-0.1.9/setup.py
+-rw-r--r--   0        0        0      703 2022-05-01 19:21:10.151485 pinject-design-0.1.9/PKG-INFO
```

### Comparing `pinject-design-0.1.8/LICENSE` & `pinject-design-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pinject-design-0.1.8/pinject_design/di/design.py` & `pinject-design-0.1.9/pinject_design/di/design.py`

 * *Files identical despite different names*

### Comparing `pinject-design-0.1.8/pinject_design/di/graph.py` & `pinject-design-0.1.9/pinject_design/di/graph.py`

 * *Files identical despite different names*

### Comparing `pinject-design-0.1.8/pinject_design/di/injected.py` & `pinject-design-0.1.9/pinject_design/di/injected.py`

 * *Files identical despite different names*

### Comparing `pinject-design-0.1.8/pinject_design/di/util.py` & `pinject-design-0.1.9/pinject_design/di/util.py`

 * *Files identical despite different names*

### Comparing `pinject-design-0.1.8/setup.py` & `pinject-design-0.1.9/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,15 +16,15 @@
  'pampy',
  'pinject',
  'returns',
  'tabulate']
 
 setup_kwargs = {
     'name': 'pinject-design',
-    'version': '0.1.8',
+    'version': '0.1.9',
     'description': 'immutable wrapper for pinject',
     'long_description': None,
     'author': 'proboscis',
     'author_email': 'nameissoap@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `pinject-design-0.1.8/PKG-INFO` & `pinject-design-0.1.9/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pinject-design
-Version: 0.1.8
+Version: 0.1.9
 Summary: immutable wrapper for pinject
 License: MIT
 Author: proboscis
 Author-email: nameissoap@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

