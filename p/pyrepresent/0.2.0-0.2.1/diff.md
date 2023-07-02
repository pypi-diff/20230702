# Comparing `tmp/pyrepresent-0.2.0.tar.gz` & `tmp/pyrepresent-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrepresent-0.2.0.tar", last modified: Sun Jul  2 15:37:13 2023, max compression
+gzip compressed data, was "pyrepresent-0.2.1.tar", last modified: Sun Jul  2 15:56:31 2023, max compression
```

## Comparing `pyrepresent-0.2.0.tar` & `pyrepresent-0.2.1.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-02 15:37:13.074620 pyrepresent-0.2.0/
--rw-rw-rw-   0        0        0      115 2023-07-02 15:37:11.000000 pyrepresent-0.2.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2548 2023-07-02 15:37:13.073619 pyrepresent-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     1669 2023-07-01 08:58:26.000000 pyrepresent-0.2.0/README.md
--rw-rw-rw-   0        0        0    12920 2023-03-17 11:12:17.000000 pyrepresent-0.2.0/build.py
--rw-rw-rw-   0        0        0      715 2023-07-02 15:37:11.000000 pyrepresent-0.2.0/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-07-02 15:37:13.069619 pyrepresent-0.2.0/pyrepresent.egg-info/
--rw-rw-rw-   0        0        0     2548 2023-07-02 15:37:13.000000 pyrepresent-0.2.0/pyrepresent.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      365 2023-07-02 15:37:13.000000 pyrepresent-0.2.0/pyrepresent.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-02 15:37:13.000000 pyrepresent-0.2.0/pyrepresent.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2023-07-02 15:37:13.000000 pyrepresent-0.2.0/pyrepresent.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-02 15:37:13.000000 pyrepresent-0.2.0/pyrepresent.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-02 15:37:13.072619 pyrepresent-0.2.0/represent/
--rw-rw-rw-   0        0        0      182 2023-07-02 15:27:45.000000 pyrepresent-0.2.0/represent/__init__.py
--rw-rw-rw-   0        0        0     2133 2023-05-15 13:38:04.000000 pyrepresent-0.2.0/represent/indentation.py
--rw-rw-rw-   0        0        0    13656 2023-07-02 15:24:15.000000 pyrepresent-0.2.0/represent/object.py
--rw-rw-rw-   0        0        0    22999 2023-07-02 15:34:31.000000 pyrepresent-0.2.0/represent/structures.py
--rw-rw-rw-   0        0        0       30 2023-03-28 10:51:56.000000 pyrepresent-0.2.0/requirements-dev.txt
--rw-rw-rw-   0        0        0       21 2023-03-28 10:51:53.000000 pyrepresent-0.2.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-02 15:37:13.074620 pyrepresent-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1682 2023-07-02 15:35:07.000000 pyrepresent-0.2.0/setup.py
--rw-rw-rw-   0        0        0     1258 2023-07-02 15:34:44.000000 pyrepresent-0.2.0/test.py
+drwxrwxrwx   0        0        0        0 2023-07-02 15:56:31.869062 pyrepresent-0.2.1/
+-rw-rw-rw-   0        0        0      115 2023-07-02 15:56:31.000000 pyrepresent-0.2.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     2548 2023-07-02 15:56:31.869062 pyrepresent-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1669 2023-07-01 08:58:26.000000 pyrepresent-0.2.1/README.md
+-rw-rw-rw-   0        0        0    12920 2023-03-17 11:12:17.000000 pyrepresent-0.2.1/build.py
+-rw-rw-rw-   0        0        0      715 2023-07-02 15:49:05.000000 pyrepresent-0.2.1/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-07-02 15:56:31.864223 pyrepresent-0.2.1/pyrepresent.egg-info/
+-rw-rw-rw-   0        0        0     2548 2023-07-02 15:56:31.000000 pyrepresent-0.2.1/pyrepresent.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      385 2023-07-02 15:56:31.000000 pyrepresent-0.2.1/pyrepresent.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-02 15:56:31.000000 pyrepresent-0.2.1/pyrepresent.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2023-07-02 15:56:31.000000 pyrepresent-0.2.1/pyrepresent.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-02 15:56:31.000000 pyrepresent-0.2.1/pyrepresent.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-02 15:56:31.868037 pyrepresent-0.2.1/represent/
+-rw-rw-rw-   0        0        0      178 2023-07-02 15:44:48.000000 pyrepresent-0.2.1/represent/__init__.py
+-rw-rw-rw-   0        0        0     8718 2023-07-02 15:44:34.000000 pyrepresent-0.2.1/represent/colors.py
+-rw-rw-rw-   0        0        0     2133 2023-05-15 13:38:04.000000 pyrepresent-0.2.1/represent/indentation.py
+-rw-rw-rw-   0        0        0    13888 2023-07-02 15:55:22.000000 pyrepresent-0.2.1/represent/object.py
+-rw-rw-rw-   0        0        0    14548 2023-07-02 15:54:50.000000 pyrepresent-0.2.1/represent/structures.py
+-rw-rw-rw-   0        0        0       30 2023-03-28 10:51:56.000000 pyrepresent-0.2.1/requirements-dev.txt
+-rw-rw-rw-   0        0        0       21 2023-03-28 10:51:53.000000 pyrepresent-0.2.1/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-02 15:56:31.869062 pyrepresent-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     1682 2023-07-02 15:49:01.000000 pyrepresent-0.2.1/setup.py
+-rw-rw-rw-   0        0        0     1361 2023-07-02 15:56:18.000000 pyrepresent-0.2.1/test.py
```

### Comparing `pyrepresent-0.2.0/PKG-INFO` & `pyrepresent-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrepresent
-Version: 0.2.0
+Version: 0.2.1
 Summary: A module for object and model representations as strings, with vast configurations, colors, hidden and protected values, assignment operations, memory addresses and more.
 Home-page: https://github.com/Shahaf-F-S/represent
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyrepresent-0.2.0/README.md` & `pyrepresent-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `pyrepresent-0.2.0/build.py` & `pyrepresent-0.2.1/build.py`

 * *Files identical despite different names*

### Comparing `pyrepresent-0.2.0/pyproject.toml` & `pyrepresent-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'pyrepresent'
-version = '0.2.0'
+version = '0.2.1'
 description = 'A module for object and model representations as strings, with vast configurations, colors, hidden and protected values, assignment operations, memory addresses and more.'
 classifiers = [
 	'Intended Audience :: Developers',
 	'License :: OSI Approved :: MIT License',
 	'Programming Language :: Python',
 	'Programming Language :: Python :: 3',
 	'Programming Language :: Python :: 3.8',
```

### Comparing `pyrepresent-0.2.0/pyrepresent.egg-info/PKG-INFO` & `pyrepresent-0.2.1/pyrepresent.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrepresent
-Version: 0.2.0
+Version: 0.2.1
 Summary: A module for object and model representations as strings, with vast configurations, colors, hidden and protected values, assignment operations, memory addresses and more.
 Home-page: https://github.com/Shahaf-F-S/represent
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyrepresent-0.2.0/represent/indentation.py` & `pyrepresent-0.2.1/represent/indentation.py`

 * *Files identical despite different names*

### Comparing `pyrepresent-0.2.0/represent/object.py` & `pyrepresent-0.2.1/represent/object.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,17 +11,18 @@
     Any, Optional, Union, Iterable, Type, Dict
 )
 
 import pandas as pd
 import numpy as np
 
 from represent.indentation import indent
+from represent.colors import colorize
 from represent.structures import (
-    structures, HiddenStructure, StringWrapper, colorize,
-    CircularReferenceStructure, DataStructure, TypeStructure,
+    structures, HiddenStructure, StringWrapper,
+    CircularReferenceStructure, TypeStructure,
     ObjectStructure, FunctionStructure, hashable_structures
 )
 
 __all__ = [
     "to_string",
     "BaseModel",
     "Modifiers",
@@ -50,14 +51,15 @@
     """A class to represent the modifiers of structures."""
 
     assign: bool = True
     protected: bool = False
     force: bool = False
     legalize: bool = False
     defined: bool = True
+    color: bool = True
 
     excluded: Iterable[Any] = field(default_factory=lambda: ['modifiers'])
     hidden: Iterable[Any] = field(default_factory=lambda: [])
     properties: Union[bool, Iterable[str]] = field(default_factory=lambda: [])
 
     def __setattr__(self, key: str, value: Any) -> None:
         """
@@ -311,28 +313,30 @@
 def unwrap(
         data: Any, /, *,
         assign: Optional[bool] = False,
         protected: Optional[bool] = False,
         legalize: Optional[bool] = False,
         force: Optional[bool] = False,
         defined: Optional[bool] = None,
+        color: Optional[bool] = None,
         properties: Optional[Union[bool, Iterable[str]]] = False,
         hidden: Optional[Union[Dict[Any, Any], Iterable[Any]]] = None,
         excluded: Optional[Iterable[Union[str, Type]]] = None,
         ids: Optional[Dict[int, Any]] = None
 ) -> Any:
     """
     Unwraps the models to get the valid_values as dictionaries.
 
     :param assign: The value to assign a type name to each commands' structure.
     :param data: The commands to process.
     :param ids: The ids of the collected objects.
     :param excluded: The keys to exclude from the commands structure.
     :param properties: The value to extract properties.
     :param protected: The value to extract hidden attributes.
+    :param color: The valur to color the object.
     :param legalize: The value to legalize the written valid_values to be strings.
     :param hidden: The valid_values of hidden keywords.
     :param force: The value to force the settings of the parsing.
     :param defined: The value to show only defined valid_values.
 
     :return: The dictionary of unwrapped objects.
     """
@@ -360,14 +364,15 @@
         assign = modifiers.assign
         excluded = modifiers.excluded
         properties = modifiers.properties
         protected = modifiers.protected
         hidden = modifiers.hidden
         legalize = modifiers.legalize
         defined = modifiers.defined
+        color = modifiers.color
     # end if
 
     if (
         inspect.isfunction(data) or
         inspect.ismethod(data)
     ):
         if is_bound_method(data) and legalize:
@@ -431,36 +436,36 @@
                 value = hidden_value(key=key, hide=hide, hidden=hidden)
             # end if
 
             key = unwrap(
                 key, assign=assign, ids=ids, excluded=excluded,
                 properties=properties, protected=protected,
                 hidden=hidden, legalize=legalize, force=force,
-                defined=defined
+                defined=defined, color=color
             )
             # end if
 
             results[key] = unwrap(
                 value, assign=assign, ids=ids, excluded=excluded,
                 properties=properties, protected=protected,
                 hidden=hidden, legalize=legalize, force=force,
-                defined=defined
+                defined=defined, color=color
             )
         # end for
 
     elif isinstance(data, (tuple, list, set)):
         results = []
 
         for value in data:
             results.append(
                 unwrap(
                     value, assign=assign, ids=ids, excluded=excluded,
                     properties=properties, protected=protected,
                     hidden=hidden, legalize=legalize, force=force,
-                    defined=defined
+                    defined=defined, color=color
                 )
             )
         # end for
 
         results = type(data)(results)
     # end if
 
@@ -475,14 +480,16 @@
         if assignment is not None:
             results.__type__ = assignment
 
             if not legalize:
                 results.__value__ = assignment
             # end if
         # end if
+
+        results.__color__ = color
     # end if
 
     ids[data_id] = results
 
     return results
 # end unwrap
 
@@ -504,13 +511,13 @@
         else:
             modifiers = Modifiers()
         # end if
     # end if
 
     data = indent(str(unwrap(obj, **modifiers)))
 
-    if DataStructure.color:
+    if modifiers.color:
         data = colorize(data)
     # end if
 
     return data
 # end to_string
```

### Comparing `pyrepresent-0.2.0/setup.py` & `pyrepresent-0.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         ],
         include=[
             "test.py"
         ],
         requirements="requirements.txt",
         dev_requirements="requirements-dev.txt",
         name='pyrepresent',
-        version='0.2.0',
+        version='0.2.1',
         description=(
             "A module for object and model representations as strings, "
             "with vast configurations, colors, hidden and protected values, "
             "assignment operations, memory addresses and more."
         ),
         license='MIT',
         author="Shahaf Frank-Shapir",
```

### Comparing `pyrepresent-0.2.0/test.py` & `pyrepresent-0.2.1/test.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,24 @@
 # test.py
 
+import datetime as dt
+
 import pandas as pd
 import numpy as np
 
 from represent import BaseModel, indent, unwrap, colorize, to_string
 
 class Model(BaseModel):
 
     def __init__(self) -> None:
 
+        self.datetime = dt.datetime.now()
+        self.date = self.datetime.date()
+        self.time = self.datetime.time()
+
         self.self = self
         self.type = type(self)
 
         self.values = [1, 2, 3]
 
         self.objects = {
             'self': self.self,
@@ -42,15 +48,14 @@
 # end Data
 
 def main() -> None:
     """Tests the module."""
 
     print(Model())
     print(Data())
-    print(to_string(unwrap(Data(), assign=True)))
     print(colorize(indent(str(unwrap({Data(): 0, Data(): 1}, assign=True)))))
     print(to_string(unwrap(Data(), assign=False)))
     print(to_string(unwrap({Data(): 0, Data(): 1}, assign=False)))
 # end main
 
 if __name__ == "__main__":
     main()
```

