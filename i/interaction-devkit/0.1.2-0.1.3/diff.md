# Comparing `tmp/interaction-devkit-0.1.2.tar.gz` & `tmp/interaction-devkit-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "interaction-devkit-0.1.2.tar", last modified: Sun Jul  2 08:48:16 2023, max compression
+gzip compressed data, was "interaction-devkit-0.1.3.tar", last modified: Sun Jul  2 09:10:26 2023, max compression
```

## Comparing `interaction-devkit-0.1.2.tar` & `interaction-devkit-0.1.3.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 08:48:16.627198 interaction-devkit-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-07-02 08:48:07.000000 interaction-devkit-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-07-02 08:48:16.627198 interaction-devkit-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-02 08:48:07.000000 interaction-devkit-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 08:48:16.623198 interaction-devkit-0.1.2/interaction/
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-02 08:48:07.000000 interaction-devkit-0.1.2/interaction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-02 08:48:07.000000 interaction-devkit-0.1.2/interaction/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 08:48:16.623198 interaction-devkit-0.1.2/interaction/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-07-02 08:48:07.000000 interaction-devkit-0.1.2/interaction/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32670 2023-07-02 08:48:07.000000 interaction-devkit-0.1.2/interaction/dataset/map_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 08:48:16.623198 interaction-devkit-0.1.2/interaction/dataset/maps/
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-07-02 08:48:07.000000 interaction-devkit-0.1.2/interaction/dataset/maps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9518 2023-07-02 08:48:07.000000 interaction-devkit-0.1.2/interaction/dataset/maps/elements.py
--rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-07-02 08:48:07.000000 interaction-devkit-0.1.2/interaction/dataset/maps/projector.py
--rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-07-02 08:48:07.000000 interaction-devkit-0.1.2/interaction/dataset/maps/speed_limit.py
--rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-07-02 08:48:07.000000 interaction-devkit-0.1.2/interaction/dataset/maps/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)    10400 2023-07-02 08:48:07.000000 interaction-devkit-0.1.2/interaction/dataset/maps/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8817 2023-07-02 08:48:07.000000 interaction-devkit-0.1.2/interaction/dataset/track_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 08:48:16.627198 interaction-devkit-0.1.2/interaction/dataset/tracks/
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-02 08:48:07.000000 interaction-devkit-0.1.2/interaction/dataset/tracks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20023 2023-07-02 08:48:07.000000 interaction-devkit-0.1.2/interaction/dataset/tracks/container.py
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-07-02 08:48:07.000000 interaction-devkit-0.1.2/interaction/dataset/tracks/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-07-02 08:48:07.000000 interaction-devkit-0.1.2/interaction/dataset/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 08:48:16.627198 interaction-devkit-0.1.2/interaction_devkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-07-02 08:48:16.000000 interaction-devkit-0.1.2/interaction_devkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-07-02 08:48:16.000000 interaction-devkit-0.1.2/interaction_devkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 08:48:16.000000 interaction-devkit-0.1.2/interaction_devkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-02 08:48:16.000000 interaction-devkit-0.1.2/interaction_devkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-02 08:48:16.000000 interaction-devkit-0.1.2/interaction_devkit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-07-02 08:48:07.000000 interaction-devkit-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-02 08:48:16.627198 interaction-devkit-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-02 08:48:07.000000 interaction-devkit-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 08:48:16.627198 interaction-devkit-0.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 08:48:07.000000 interaction-devkit-0.1.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4095 2023-07-02 08:48:07.000000 interaction-devkit-0.1.2/tests/test_map_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    13433 2023-07-02 08:48:07.000000 interaction-devkit-0.1.2/tests/test_map_components.py
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-02 08:48:07.000000 interaction-devkit-0.1.2/tests/test_track_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-07-02 08:48:07.000000 interaction-devkit-0.1.2/tests/test_track_components.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:10:26.321074 interaction-devkit-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-07-02 09:10:15.000000 interaction-devkit-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-07-02 09:10:26.321074 interaction-devkit-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-02 09:10:15.000000 interaction-devkit-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:10:26.317074 interaction-devkit-0.1.3/interaction/
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-07-02 09:10:15.000000 interaction-devkit-0.1.3/interaction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-02 09:10:15.000000 interaction-devkit-0.1.3/interaction/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:10:26.317074 interaction-devkit-0.1.3/interaction/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-07-02 09:10:15.000000 interaction-devkit-0.1.3/interaction/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32670 2023-07-02 09:10:15.000000 interaction-devkit-0.1.3/interaction/dataset/map_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:10:26.317074 interaction-devkit-0.1.3/interaction/dataset/maps/
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-07-02 09:10:15.000000 interaction-devkit-0.1.3/interaction/dataset/maps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9518 2023-07-02 09:10:15.000000 interaction-devkit-0.1.3/interaction/dataset/maps/elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-07-02 09:10:15.000000 interaction-devkit-0.1.3/interaction/dataset/maps/projector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-07-02 09:10:15.000000 interaction-devkit-0.1.3/interaction/dataset/maps/speed_limit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-07-02 09:10:15.000000 interaction-devkit-0.1.3/interaction/dataset/maps/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10400 2023-07-02 09:10:15.000000 interaction-devkit-0.1.3/interaction/dataset/maps/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8817 2023-07-02 09:10:15.000000 interaction-devkit-0.1.3/interaction/dataset/track_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:10:26.321074 interaction-devkit-0.1.3/interaction/dataset/tracks/
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-02 09:10:15.000000 interaction-devkit-0.1.3/interaction/dataset/tracks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20023 2023-07-02 09:10:15.000000 interaction-devkit-0.1.3/interaction/dataset/tracks/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-07-02 09:10:15.000000 interaction-devkit-0.1.3/interaction/dataset/tracks/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-07-02 09:10:15.000000 interaction-devkit-0.1.3/interaction/dataset/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:10:26.321074 interaction-devkit-0.1.3/interaction_devkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-07-02 09:10:26.000000 interaction-devkit-0.1.3/interaction_devkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-07-02 09:10:26.000000 interaction-devkit-0.1.3/interaction_devkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 09:10:26.000000 interaction-devkit-0.1.3/interaction_devkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-02 09:10:26.000000 interaction-devkit-0.1.3/interaction_devkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-02 09:10:26.000000 interaction-devkit-0.1.3/interaction_devkit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-07-02 09:10:15.000000 interaction-devkit-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-02 09:10:26.321074 interaction-devkit-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-02 09:10:15.000000 interaction-devkit-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:10:26.321074 interaction-devkit-0.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 09:10:15.000000 interaction-devkit-0.1.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4095 2023-07-02 09:10:15.000000 interaction-devkit-0.1.3/tests/test_map_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13433 2023-07-02 09:10:15.000000 interaction-devkit-0.1.3/tests/test_map_components.py
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-02 09:10:15.000000 interaction-devkit-0.1.3/tests/test_track_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-07-02 09:10:15.000000 interaction-devkit-0.1.3/tests/test_track_components.py
```

### Comparing `interaction-devkit-0.1.2/LICENSE` & `interaction-devkit-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `interaction-devkit-0.1.2/PKG-INFO` & `interaction-devkit-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: interaction-devkit
-Version: 0.1.2
+Version: 0.1.3
 Summary: A toolkit for building interactive applications.
 Author-email: Juanwu Lu <juanwu@purdue.edu>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, Juanwu Lu
         
         Redistribution and use in source and binary forms, with or without
```

### Comparing `interaction-devkit-0.1.2/README.md` & `interaction-devkit-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `interaction-devkit-0.1.2/interaction/dataset/map_api.py` & `interaction-devkit-0.1.3/interaction/dataset/map_api.py`

 * *Files identical despite different names*

### Comparing `interaction-devkit-0.1.2/interaction/dataset/maps/__init__.py` & `interaction-devkit-0.1.3/interaction/dataset/maps/__init__.py`

 * *Files identical despite different names*

### Comparing `interaction-devkit-0.1.2/interaction/dataset/maps/elements.py` & `interaction-devkit-0.1.3/interaction/dataset/maps/elements.py`

 * *Files identical despite different names*

### Comparing `interaction-devkit-0.1.2/interaction/dataset/maps/projector.py` & `interaction-devkit-0.1.3/interaction/dataset/maps/projector.py`

 * *Files identical despite different names*

### Comparing `interaction-devkit-0.1.2/interaction/dataset/maps/speed_limit.py` & `interaction-devkit-0.1.3/interaction/dataset/maps/speed_limit.py`

 * *Files identical despite different names*

### Comparing `interaction-devkit-0.1.2/interaction/dataset/maps/typing.py` & `interaction-devkit-0.1.3/interaction/dataset/maps/typing.py`

 * *Files identical despite different names*

### Comparing `interaction-devkit-0.1.2/interaction/dataset/maps/utils.py` & `interaction-devkit-0.1.3/interaction/dataset/maps/utils.py`

 * *Files identical despite different names*

### Comparing `interaction-devkit-0.1.2/interaction/dataset/track_api.py` & `interaction-devkit-0.1.3/interaction/dataset/track_api.py`

 * *Files identical despite different names*

### Comparing `interaction-devkit-0.1.2/interaction/dataset/tracks/container.py` & `interaction-devkit-0.1.3/interaction/dataset/tracks/container.py`

 * *Files identical despite different names*

### Comparing `interaction-devkit-0.1.2/interaction/dataset/tracks/typing.py` & `interaction-devkit-0.1.3/interaction/dataset/tracks/typing.py`

 * *Files identical despite different names*

### Comparing `interaction-devkit-0.1.2/interaction/dataset/utils.py` & `interaction-devkit-0.1.3/interaction/dataset/utils.py`

 * *Files identical despite different names*

### Comparing `interaction-devkit-0.1.2/interaction_devkit.egg-info/PKG-INFO` & `interaction-devkit-0.1.3/interaction_devkit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: interaction-devkit
-Version: 0.1.2
+Version: 0.1.3
 Summary: A toolkit for building interactive applications.
 Author-email: Juanwu Lu <juanwu@purdue.edu>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, Juanwu Lu
         
         Redistribution and use in source and binary forms, with or without
```

### Comparing `interaction-devkit-0.1.2/interaction_devkit.egg-info/SOURCES.txt` & `interaction-devkit-0.1.3/interaction_devkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `interaction-devkit-0.1.2/pyproject.toml` & `interaction-devkit-0.1.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 
 [project]
 name = "interaction-devkit"
-version = "0.1.2"
+version = "0.1.3"
 description = "A toolkit for building interactive applications."
 readme = "README.md"
 authors = [{name="Juanwu Lu", email="juanwu@purdue.edu"}]
 license = {file = "LICENSE"}
 requires-python = ">=3.9"
 dependencies = [
     "defusedxml",
@@ -28,15 +28,15 @@
 [tool.isort]
 known_first_party = "interaction-devkit"
 
 line_length = 79
 profile = "black"
 
 [tool.bumpver]
-current_version = "0.1.2"
+current_version = "0.1.3"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "Bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `interaction-devkit-0.1.2/tests/test_map_api.py` & `interaction-devkit-0.1.3/tests/test_map_api.py`

 * *Files identical despite different names*

### Comparing `interaction-devkit-0.1.2/tests/test_map_components.py` & `interaction-devkit-0.1.3/tests/test_map_components.py`

 * *Files identical despite different names*

### Comparing `interaction-devkit-0.1.2/tests/test_track_components.py` & `interaction-devkit-0.1.3/tests/test_track_components.py`

 * *Files identical despite different names*

