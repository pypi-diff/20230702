# Comparing `tmp/oarepo-model-builder-ui-4.0.5.tar.gz` & `tmp/oarepo-model-builder-ui-4.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oarepo-model-builder-ui-4.0.5.tar", last modified: Wed May 31 09:02:33 2023, max compression
+gzip compressed data, was "oarepo-model-builder-ui-4.0.6.tar", last modified: Sun Jul  2 16:29:54 2023, max compression
```

## Comparing `oarepo-model-builder-ui-4.0.5.tar` & `oarepo-model-builder-ui-4.0.6.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:02:33.553760 oarepo-model-builder-ui-4.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-31 08:59:43.000000 oarepo-model-builder-ui-4.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-05-31 09:02:33.553760 oarepo-model-builder-ui-4.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-05-31 08:59:43.000000 oarepo-model-builder-ui-4.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:02:33.549760 oarepo-model-builder-ui-4.0.5/oarepo_model_builder_ui/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 08:59:43.000000 oarepo-model-builder-ui-4.0.5/oarepo_model_builder_ui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:02:33.553760 oarepo-model-builder-ui-4.0.5/oarepo_model_builder_ui/builders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 08:59:43.000000 oarepo-model-builder-ui-4.0.5/oarepo_model_builder_ui/builders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-05-31 08:59:43.000000 oarepo-model-builder-ui-4.0.5/oarepo_model_builder_ui/builders/i18n.py
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-31 08:59:43.000000 oarepo-model-builder-ui-4.0.5/oarepo_model_builder_ui/builders/i18n_setup_cfg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-05-31 08:59:43.000000 oarepo-model-builder-ui-4.0.5/oarepo_model_builder_ui/builders/layout.py
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-05-31 08:59:43.000000 oarepo-model-builder-ui-4.0.5/oarepo_model_builder_ui/builders/layout_setup_cfg.py
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-31 08:59:43.000000 oarepo-model-builder-ui-4.0.5/oarepo_model_builder_ui/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:02:33.553760 oarepo-model-builder-ui-4.0.5/oarepo_model_builder_ui/datatypes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 08:59:43.000000 oarepo-model-builder-ui-4.0.5/oarepo_model_builder_ui/datatypes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:02:33.553760 oarepo-model-builder-ui-4.0.5/oarepo_model_builder_ui/datatypes/components/
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-05-31 08:59:43.000000 oarepo-model-builder-ui-4.0.5/oarepo_model_builder_ui/datatypes/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-05-31 08:59:43.000000 oarepo-model-builder-ui-4.0.5/oarepo_model_builder_ui/datatypes/components/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:02:33.553760 oarepo-model-builder-ui-4.0.5/oarepo_model_builder_ui/outputs/
--rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-05-31 08:59:43.000000 oarepo-model-builder-ui-4.0.5/oarepo_model_builder_ui/outputs/i18n.py
--rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-05-31 08:59:43.000000 oarepo-model-builder-ui-4.0.5/oarepo_model_builder_ui/outputs/layout.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:02:33.553760 oarepo-model-builder-ui-4.0.5/oarepo_model_builder_ui/validation/
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-31 08:59:43.000000 oarepo-model-builder-ui-4.0.5/oarepo_model_builder_ui/validation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:02:33.549760 oarepo-model-builder-ui-4.0.5/oarepo_model_builder_ui.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-05-31 09:02:33.000000 oarepo-model-builder-ui-4.0.5/oarepo_model_builder_ui.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-05-31 09:02:33.000000 oarepo-model-builder-ui-4.0.5/oarepo_model_builder_ui.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 09:02:33.000000 oarepo-model-builder-ui-4.0.5/oarepo_model_builder_ui.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-05-31 09:02:33.000000 oarepo-model-builder-ui-4.0.5/oarepo_model_builder_ui.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-31 09:02:33.000000 oarepo-model-builder-ui-4.0.5/oarepo_model_builder_ui.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-31 09:02:33.000000 oarepo-model-builder-ui-4.0.5/oarepo_model_builder_ui.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-31 08:59:43.000000 oarepo-model-builder-ui-4.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-05-31 09:02:33.553760 oarepo-model-builder-ui-4.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 08:59:43.000000 oarepo-model-builder-ui-4.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 16:29:54.795013 oarepo-model-builder-ui-4.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-02 16:26:50.000000 oarepo-model-builder-ui-4.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-07-02 16:29:54.795013 oarepo-model-builder-ui-4.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-07-02 16:26:50.000000 oarepo-model-builder-ui-4.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 16:29:54.791012 oarepo-model-builder-ui-4.0.6/oarepo_model_builder_ui/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 16:26:50.000000 oarepo-model-builder-ui-4.0.6/oarepo_model_builder_ui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 16:29:54.795013 oarepo-model-builder-ui-4.0.6/oarepo_model_builder_ui/builders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 16:26:50.000000 oarepo-model-builder-ui-4.0.6/oarepo_model_builder_ui/builders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-07-02 16:26:50.000000 oarepo-model-builder-ui-4.0.6/oarepo_model_builder_ui/builders/i18n.py
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-07-02 16:26:50.000000 oarepo-model-builder-ui-4.0.6/oarepo_model_builder_ui/builders/i18n_setup_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-07-02 16:26:50.000000 oarepo-model-builder-ui-4.0.6/oarepo_model_builder_ui/builders/layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-07-02 16:26:50.000000 oarepo-model-builder-ui-4.0.6/oarepo_model_builder_ui/builders/layout_setup_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-02 16:26:50.000000 oarepo-model-builder-ui-4.0.6/oarepo_model_builder_ui/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 16:29:54.795013 oarepo-model-builder-ui-4.0.6/oarepo_model_builder_ui/datatypes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 16:26:50.000000 oarepo-model-builder-ui-4.0.6/oarepo_model_builder_ui/datatypes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 16:29:54.795013 oarepo-model-builder-ui-4.0.6/oarepo_model_builder_ui/datatypes/components/
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-07-02 16:26:50.000000 oarepo-model-builder-ui-4.0.6/oarepo_model_builder_ui/datatypes/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-07-02 16:26:50.000000 oarepo-model-builder-ui-4.0.6/oarepo_model_builder_ui/datatypes/components/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 16:29:54.795013 oarepo-model-builder-ui-4.0.6/oarepo_model_builder_ui/outputs/
+-rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-07-02 16:26:50.000000 oarepo-model-builder-ui-4.0.6/oarepo_model_builder_ui/outputs/i18n.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-07-02 16:26:50.000000 oarepo-model-builder-ui-4.0.6/oarepo_model_builder_ui/outputs/layout.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 16:29:54.795013 oarepo-model-builder-ui-4.0.6/oarepo_model_builder_ui/validation/
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-02 16:26:50.000000 oarepo-model-builder-ui-4.0.6/oarepo_model_builder_ui/validation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 16:29:54.791012 oarepo-model-builder-ui-4.0.6/oarepo_model_builder_ui.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-07-02 16:29:54.000000 oarepo-model-builder-ui-4.0.6/oarepo_model_builder_ui.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-07-02 16:29:54.000000 oarepo-model-builder-ui-4.0.6/oarepo_model_builder_ui.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 16:29:54.000000 oarepo-model-builder-ui-4.0.6/oarepo_model_builder_ui.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-07-02 16:29:54.000000 oarepo-model-builder-ui-4.0.6/oarepo_model_builder_ui.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-02 16:29:54.000000 oarepo-model-builder-ui-4.0.6/oarepo_model_builder_ui.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-02 16:29:54.000000 oarepo-model-builder-ui-4.0.6/oarepo_model_builder_ui.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-02 16:26:50.000000 oarepo-model-builder-ui-4.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-07-02 16:29:54.795013 oarepo-model-builder-ui-4.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 16:26:50.000000 oarepo-model-builder-ui-4.0.6/setup.py
```

### Comparing `oarepo-model-builder-ui-4.0.5/PKG-INFO` & `oarepo-model-builder-ui-4.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oarepo-model-builder-ui
-Version: 4.0.5
+Version: 4.0.6
 Summary: Model builder plugin for oarepo-ui
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 
 <!--
  Copyright (c) 2022 CESNET
```

### Comparing `oarepo-model-builder-ui-4.0.5/README.md` & `oarepo-model-builder-ui-4.0.6/README.md`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-ui-4.0.5/oarepo_model_builder_ui/builders/i18n.py` & `oarepo-model-builder-ui-4.0.6/oarepo_model_builder_ui/builders/i18n.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-ui-4.0.5/oarepo_model_builder_ui/builders/i18n_setup_cfg.py` & `oarepo-model-builder-ui-4.0.6/oarepo_model_builder_ui/builders/i18n_setup_cfg.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-ui-4.0.5/oarepo_model_builder_ui/builders/layout.py` & `oarepo-model-builder-ui-4.0.6/oarepo_model_builder_ui/builders/layout.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-ui-4.0.5/oarepo_model_builder_ui/builders/layout_setup_cfg.py` & `oarepo-model-builder-ui-4.0.6/oarepo_model_builder_ui/builders/layout_setup_cfg.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-ui-4.0.5/oarepo_model_builder_ui/datatypes/components/__init__.py` & `oarepo-model-builder-ui-4.0.6/oarepo_model_builder_ui/datatypes/components/__init__.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-ui-4.0.5/oarepo_model_builder_ui/datatypes/components/model.py` & `oarepo-model-builder-ui-4.0.6/oarepo_model_builder_ui/datatypes/components/model.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-ui-4.0.5/oarepo_model_builder_ui/outputs/i18n.py` & `oarepo-model-builder-ui-4.0.6/oarepo_model_builder_ui/outputs/i18n.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-ui-4.0.5/oarepo_model_builder_ui/outputs/layout.py` & `oarepo-model-builder-ui-4.0.6/oarepo_model_builder_ui/outputs/layout.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-ui-4.0.5/oarepo_model_builder_ui.egg-info/PKG-INFO` & `oarepo-model-builder-ui-4.0.6/oarepo_model_builder_ui.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oarepo-model-builder-ui
-Version: 4.0.5
+Version: 4.0.6
 Summary: Model builder plugin for oarepo-ui
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 
 <!--
  Copyright (c) 2022 CESNET
```

### Comparing `oarepo-model-builder-ui-4.0.5/oarepo_model_builder_ui.egg-info/SOURCES.txt` & `oarepo-model-builder-ui-4.0.6/oarepo_model_builder_ui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-ui-4.0.5/oarepo_model_builder_ui.egg-info/entry_points.txt` & `oarepo-model-builder-ui-4.0.6/oarepo_model_builder_ui.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-ui-4.0.5/setup.cfg` & `oarepo-model-builder-ui-4.0.6/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 [metadata]
 name = oarepo-model-builder-ui
-version = 4.0.5
+version = 4.0.6
 description = Model builder plugin for oarepo-ui
 authors = 
 readme = README.md
 long_description = file:README.md
 long_description_content_type = text/markdown
 
 [options]
 python = >=3.9,<4.0
 install_requires = 
 	langcodes>=3.3.0
 	oarepo-model-builder>=4.0.0
 	polib
-	inflect
+	pydantic<2.0.0
+	inflect<=6.0.4
 
 [options.packages.find]
 exclude = 
 	tests
 	mock_record
 
 [options.extras_require]
```

