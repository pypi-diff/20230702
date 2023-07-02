# Comparing `tmp/typedload-2.8.tar.gz` & `tmp/typedload-2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typedload-2.8.tar", last modified: Sun Jun 20 08:31:49 2021, max compression
+gzip compressed data, was "typedload-2.9.tar", last modified: Fri Aug 27 14:16:40 2021, max compression
```

## Comparing `typedload-2.8.tar` & `typedload-2.9.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 salvo     (1000) salvo     (1000)        0 2021-06-20 08:31:49.334049 typedload-2.8/
--rw-r--r--   0 salvo     (1000) salvo     (1000)     1359 2021-06-20 08:31:49.338049 typedload-2.8/PKG-INFO
--rwxr-xr-x   0 salvo     (1000) salvo     (1000)     2203 2021-06-20 07:16:29.542227 typedload-2.8/setup.py
-drwxr-xr-x   0 salvo     (1000) salvo     (1000)        0 2021-06-20 08:31:49.334049 typedload-2.8/typedload/
--rw-r--r--   0 salvo     (1000) salvo     (1000)     5566 2021-01-31 12:33:07.213145 typedload-2.8/typedload/__init__.py
--rw-r--r--   0 salvo     (1000) salvo     (1000)     7978 2021-02-16 14:05:36.536312 typedload-2.8/typedload/datadumper.py
--rw-r--r--   0 salvo     (1000) salvo     (1000)    22786 2021-06-20 07:16:29.542227 typedload-2.8/typedload/dataloader.py
--rw-r--r--   0 salvo     (1000) salvo     (1000)     5263 2021-04-06 18:04:15.718275 typedload-2.8/typedload/exceptions.py
--rw-r--r--   0 salvo     (1000) salvo     (1000)     1039 2021-02-16 14:05:36.536312 typedload-2.8/typedload/helpers.py
--rw-r--r--   0 salvo     (1000) salvo     (1000)        0 2021-01-31 12:33:07.217145 typedload-2.8/typedload/py.typed
--rw-r--r--   0 salvo     (1000) salvo     (1000)     6099 2021-02-04 06:59:41.458457 typedload-2.8/typedload/typechecks.py
+drwxr-xr-x   0 salvo     (1000) salvo     (1000)        0 2021-08-27 14:16:40.895133 typedload-2.9/
+-rw-r--r--   0 salvo     (1000) salvo     (1000)     5092 2021-08-27 14:16:40.895133 typedload-2.9/PKG-INFO
+-rwxr-xr-x   0 salvo     (1000) salvo     (1000)     2725 2021-08-27 14:16:33.903133 typedload-2.9/setup.py
+drwxr-xr-x   0 salvo     (1000) salvo     (1000)        0 2021-08-27 14:16:40.895133 typedload-2.9/typedload/
+-rw-r--r--   0 salvo     (1000) salvo     (1000)     5566 2021-08-27 14:16:14.151133 typedload-2.9/typedload/__init__.py
+-rw-r--r--   0 salvo     (1000) salvo     (1000)     7945 2021-08-27 14:16:14.151133 typedload-2.9/typedload/datadumper.py
+-rw-r--r--   0 salvo     (1000) salvo     (1000)    22777 2021-08-27 14:16:14.151133 typedload-2.9/typedload/dataloader.py
+-rw-r--r--   0 salvo     (1000) salvo     (1000)     5263 2021-08-27 14:16:14.151133 typedload-2.9/typedload/exceptions.py
+-rw-r--r--   0 salvo     (1000) salvo     (1000)     1039 2021-08-27 14:16:14.151133 typedload-2.9/typedload/helpers.py
+-rw-r--r--   0 salvo     (1000) salvo     (1000)        0 2021-08-27 14:16:14.151133 typedload-2.9/typedload/py.typed
+-rw-r--r--   0 salvo     (1000) salvo     (1000)     6103 2021-08-27 14:16:14.151133 typedload-2.9/typedload/typechecks.py
```

### Comparing `typedload-2.8/typedload/__init__.py` & `typedload-2.9/typedload/__init__.py`

 * *Files identical despite different names*

### Comparing `typedload-2.8/typedload/datadumper.py` & `typedload-2.9/typedload/datadumper.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,25 +23,22 @@
 import datetime
 import ipaddress
 from enum import Enum
 import pathlib
 from typing import *
 
 from .exceptions import TypedloadValueError
-from .typechecks import is_attrs
+from .typechecks import is_attrs, NONETYPE
 
 
 __all__ = [
     'Dumper',
 ]
 
 
-NONETYPE = type(None)  # type: Type[Any]
-
-
 class Dumper:
 
     def __init__(self, **kwargs):
         """
         This dumps data structures recursively using only
         basic types, lists and dictionaries.
```

### Comparing `typedload-2.8/typedload/dataloader.py` & `typedload-2.9/typedload/dataloader.py`

 * *Files 0% similar despite different names*

```diff
@@ -289,15 +289,15 @@
 
         if self.dictequivalence:
             # Convert argparse.Namespace to dictionary
             if hasattr(value, '_get_kwargs'):
                 value = {k: v for k,v in value._get_kwargs()}
 
         try:
-            return cast(T, func(self, value, type_))
+            return func(self, value, type_)
         except Exception as e:
             assert isinstance(e, TypedloadException)
             e.trace.insert(0, TraceItem(value, type_, annotation))
             raise e
 
 
 def _forwardrefload(l: Loader, value: Any, type_: type) -> Any:
```

### Comparing `typedload-2.8/typedload/exceptions.py` & `typedload-2.9/typedload/exceptions.py`

 * *Files identical despite different names*

### Comparing `typedload-2.8/typedload/helpers.py` & `typedload-2.9/typedload/helpers.py`

 * *Files identical despite different names*

### Comparing `typedload-2.8/typedload/typechecks.py` & `typedload-2.9/typedload/typechecks.py`

 * *Files 1% similar despite different names*

```diff
@@ -228,15 +228,15 @@
     return set(type_.__args__)
 
 
 def is_literal(type_: Type[Any]) -> bool:
     '''
     Check if the type is a typing.Literal
     '''
-    return getattr(type_, '__origin__', None) == Literal and Literal != None
+    return getattr(type_, '__origin__', None) == Literal and Literal is not None
 
 
 def is_typeddict(type_: Type[Any]) -> bool:
     '''
     Check if it is a typing.TypedDict
     '''
     if _TypedDictMeta:
```

