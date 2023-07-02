# Comparing `tmp/objectory-0.0.4.tar.gz` & `tmp/objectory-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "objectory-0.0.4.tar", max compression
+gzip compressed data, was "objectory-0.0.5.tar", max compression
```

## Comparing `objectory-0.0.4.tar` & `objectory-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1501 2023-07-01 20:37:13.092293 objectory-0.0.4/LICENSE
--rw-r--r--   0        0        0     4516 2023-07-01 20:37:13.092293 objectory-0.0.4/README.md
--rw-r--r--   0        0        0     3829 2023-07-01 20:37:13.096293 objectory-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      280 2023-07-01 20:37:13.096293 objectory-0.0.4/src/objectory/__init__.py
--rw-r--r--   0        0        0    13109 2023-07-01 20:37:13.096293 objectory-0.0.4/src/objectory/abstract_factory.py
--rw-r--r--   0        0        0      138 2023-07-01 20:37:13.096293 objectory-0.0.4/src/objectory/constants.py
--rw-r--r--   0        0        0     1511 2023-07-01 20:37:13.096293 objectory-0.0.4/src/objectory/errors.py
--rw-r--r--   0        0        0    16099 2023-07-01 20:37:13.096293 objectory-0.0.4/src/objectory/registry.py
--rw-r--r--   0        0        0     1290 2023-07-01 20:37:13.096293 objectory-0.0.4/src/objectory/universal.py
--rw-r--r--   0        0        0      449 2023-07-01 20:37:13.096293 objectory-0.0.4/src/objectory/utils/__init__.py
--rw-r--r--   0        0        0     1047 2023-07-01 20:37:13.096293 objectory-0.0.4/src/objectory/utils/config.py
--rw-r--r--   0        0        0     3192 2023-07-01 20:37:13.096293 objectory-0.0.4/src/objectory/utils/name_resolution.py
--rw-r--r--   0        0        0     7469 2023-07-01 20:37:13.096293 objectory-0.0.4/src/objectory/utils/object_helpers.py
--rw-r--r--   0        0        0     5571 1970-01-01 00:00:00.000000 objectory-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1501 2023-07-02 18:47:15.537530 objectory-0.0.5/LICENSE
+-rw-r--r--   0        0        0     4516 2023-07-02 18:47:15.537530 objectory-0.0.5/README.md
+-rw-r--r--   0        0        0     3829 2023-07-02 18:47:15.537530 objectory-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      280 2023-07-02 18:47:15.537530 objectory-0.0.5/src/objectory/__init__.py
+-rw-r--r--   0        0        0    13109 2023-07-02 18:47:15.537530 objectory-0.0.5/src/objectory/abstract_factory.py
+-rw-r--r--   0        0        0      138 2023-07-02 18:47:15.537530 objectory-0.0.5/src/objectory/constants.py
+-rw-r--r--   0        0        0     1511 2023-07-02 18:47:15.537530 objectory-0.0.5/src/objectory/errors.py
+-rw-r--r--   0        0        0    16099 2023-07-02 18:47:15.541530 objectory-0.0.5/src/objectory/registry.py
+-rw-r--r--   0        0        0     1290 2023-07-02 18:47:15.541530 objectory-0.0.5/src/objectory/universal.py
+-rw-r--r--   0        0        0      449 2023-07-02 18:47:15.541530 objectory-0.0.5/src/objectory/utils/__init__.py
+-rw-r--r--   0        0        0     1334 2023-07-02 18:47:15.541530 objectory-0.0.5/src/objectory/utils/config.py
+-rw-r--r--   0        0        0     3192 2023-07-02 18:47:15.541530 objectory-0.0.5/src/objectory/utils/name_resolution.py
+-rw-r--r--   0        0        0     7469 2023-07-02 18:47:15.541530 objectory-0.0.5/src/objectory/utils/object_helpers.py
+-rw-r--r--   0        0        0     5571 1970-01-01 00:00:00.000000 objectory-0.0.5/PKG-INFO
```

### Comparing `objectory-0.0.4/LICENSE` & `objectory-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `objectory-0.0.4/README.md` & `objectory-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `objectory-0.0.4/pyproject.toml` & `objectory-0.0.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "objectory"
-version = "0.0.4"
+version = "0.0.5"
 description = "A light library for general purpose object factories"
 readme = "README.md"
 authors = ["Thibaut Durand <durand.tibo+gh@gmail.com>"]
 homepage = "https://github.com/durandtibo/objectory"
 repository = "https://github.com/durandtibo/objectory"
 keywords = ["factory", "abstract factory", "registry"]
 license = "BSD-3-Clause"
```

### Comparing `objectory-0.0.4/src/objectory/abstract_factory.py` & `objectory-0.0.5/src/objectory/abstract_factory.py`

 * *Files identical despite different names*

### Comparing `objectory-0.0.4/src/objectory/errors.py` & `objectory-0.0.5/src/objectory/errors.py`

 * *Files identical despite different names*

### Comparing `objectory-0.0.4/src/objectory/registry.py` & `objectory-0.0.5/src/objectory/registry.py`

 * *Files identical despite different names*

### Comparing `objectory-0.0.4/src/objectory/universal.py` & `objectory-0.0.5/src/objectory/universal.py`

 * *Files identical despite different names*

### Comparing `objectory-0.0.4/src/objectory/utils/config.py` & `objectory-0.0.5/src/objectory/utils/config.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,26 @@
 from __future__ import annotations
 
 __all__ = ["is_object_config"]
 
+import inspect
+import typing
+
 from objectory.constants import OBJECT_TARGET
 from objectory.utils.object_helpers import import_object
 
 
 def is_object_config(config: dict, cls: type[object]) -> bool:
     r"""Indicate if the input configuration is a configuration for a
     given class.
 
     This function only checks if the value of the key  ``_target_``
-    is valid. It does not check the other values.
+    is valid. It does not check the other values. If ``_target_``
+    indicates a function, the returned type hint is used to check
+    the class.
 
     Args:
     ----
         config (dict): Specifies the configuration to check.
         cls (type): Specifies the object class.
 
     Returns:
@@ -30,8 +35,13 @@
         >>> from objectory.utils import is_object_config
         >>> is_object_config({"_target_": "collections.Counter", "iterable": [1, 2, 1, 3]})
         True
     """
     target = config.get(OBJECT_TARGET)
     if target is None:
         return False
-    return cls in import_object(target).__mro__
+    target = import_object(target)
+    if inspect.isfunction(target):
+        target = typing.get_type_hints(target).get("return")
+    if target is None:
+        return False
+    return cls in target.__mro__
```

### Comparing `objectory-0.0.4/src/objectory/utils/name_resolution.py` & `objectory-0.0.5/src/objectory/utils/name_resolution.py`

 * *Files identical despite different names*

### Comparing `objectory-0.0.4/src/objectory/utils/object_helpers.py` & `objectory-0.0.5/src/objectory/utils/object_helpers.py`

 * *Files identical despite different names*

### Comparing `objectory-0.0.4/PKG-INFO` & `objectory-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: objectory
-Version: 0.0.4
+Version: 0.0.5
 Summary: A light library for general purpose object factories
 Home-page: https://github.com/durandtibo/objectory
 License: BSD-3-Clause
 Keywords: factory,abstract factory,registry
 Author: Thibaut Durand
 Author-email: durand.tibo+gh@gmail.com
 Requires-Python: >=3.9,<4.0
```

