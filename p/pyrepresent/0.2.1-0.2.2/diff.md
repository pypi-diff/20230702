# Comparing `tmp/pyrepresent-0.2.1.tar.gz` & `tmp/pyrepresent-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrepresent-0.2.1.tar", last modified: Sun Jul  2 15:56:31 2023, max compression
+gzip compressed data, was "pyrepresent-0.2.2.tar", last modified: Sun Jul  2 16:45:02 2023, max compression
```

## Comparing `pyrepresent-0.2.1.tar` & `pyrepresent-0.2.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-02 15:56:31.869062 pyrepresent-0.2.1/
--rw-rw-rw-   0        0        0      115 2023-07-02 15:56:31.000000 pyrepresent-0.2.1/MANIFEST.in
--rw-rw-rw-   0        0        0     2548 2023-07-02 15:56:31.869062 pyrepresent-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     1669 2023-07-01 08:58:26.000000 pyrepresent-0.2.1/README.md
--rw-rw-rw-   0        0        0    12920 2023-03-17 11:12:17.000000 pyrepresent-0.2.1/build.py
--rw-rw-rw-   0        0        0      715 2023-07-02 15:49:05.000000 pyrepresent-0.2.1/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-07-02 15:56:31.864223 pyrepresent-0.2.1/pyrepresent.egg-info/
--rw-rw-rw-   0        0        0     2548 2023-07-02 15:56:31.000000 pyrepresent-0.2.1/pyrepresent.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      385 2023-07-02 15:56:31.000000 pyrepresent-0.2.1/pyrepresent.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-02 15:56:31.000000 pyrepresent-0.2.1/pyrepresent.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2023-07-02 15:56:31.000000 pyrepresent-0.2.1/pyrepresent.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-02 15:56:31.000000 pyrepresent-0.2.1/pyrepresent.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-02 15:56:31.868037 pyrepresent-0.2.1/represent/
--rw-rw-rw-   0        0        0      178 2023-07-02 15:44:48.000000 pyrepresent-0.2.1/represent/__init__.py
--rw-rw-rw-   0        0        0     8718 2023-07-02 15:44:34.000000 pyrepresent-0.2.1/represent/colors.py
--rw-rw-rw-   0        0        0     2133 2023-05-15 13:38:04.000000 pyrepresent-0.2.1/represent/indentation.py
--rw-rw-rw-   0        0        0    13888 2023-07-02 15:55:22.000000 pyrepresent-0.2.1/represent/object.py
--rw-rw-rw-   0        0        0    14548 2023-07-02 15:54:50.000000 pyrepresent-0.2.1/represent/structures.py
--rw-rw-rw-   0        0        0       30 2023-03-28 10:51:56.000000 pyrepresent-0.2.1/requirements-dev.txt
--rw-rw-rw-   0        0        0       21 2023-03-28 10:51:53.000000 pyrepresent-0.2.1/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-02 15:56:31.869062 pyrepresent-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0     1682 2023-07-02 15:49:01.000000 pyrepresent-0.2.1/setup.py
--rw-rw-rw-   0        0        0     1361 2023-07-02 15:56:18.000000 pyrepresent-0.2.1/test.py
+drwxrwxrwx   0        0        0        0 2023-07-02 16:45:02.224856 pyrepresent-0.2.2/
+-rw-rw-rw-   0        0        0      115 2023-07-02 16:45:01.000000 pyrepresent-0.2.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     2548 2023-07-02 16:45:02.223848 pyrepresent-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1669 2023-07-01 08:58:26.000000 pyrepresent-0.2.2/README.md
+-rw-rw-rw-   0        0        0    12920 2023-03-17 11:12:17.000000 pyrepresent-0.2.2/build.py
+-rw-rw-rw-   0        0        0      715 2023-07-02 16:45:01.000000 pyrepresent-0.2.2/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-07-02 16:45:02.219946 pyrepresent-0.2.2/pyrepresent.egg-info/
+-rw-rw-rw-   0        0        0     2548 2023-07-02 16:45:02.000000 pyrepresent-0.2.2/pyrepresent.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      385 2023-07-02 16:45:02.000000 pyrepresent-0.2.2/pyrepresent.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-02 16:45:02.000000 pyrepresent-0.2.2/pyrepresent.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2023-07-02 16:45:02.000000 pyrepresent-0.2.2/pyrepresent.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-02 16:45:02.000000 pyrepresent-0.2.2/pyrepresent.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-02 16:45:02.223848 pyrepresent-0.2.2/represent/
+-rw-rw-rw-   0        0        0      178 2023-07-02 15:44:48.000000 pyrepresent-0.2.2/represent/__init__.py
+-rw-rw-rw-   0        0        0     8718 2023-07-02 15:44:34.000000 pyrepresent-0.2.2/represent/colors.py
+-rw-rw-rw-   0        0        0     2133 2023-05-15 13:38:04.000000 pyrepresent-0.2.2/represent/indentation.py
+-rw-rw-rw-   0        0        0    14681 2023-07-02 16:44:39.000000 pyrepresent-0.2.2/represent/object.py
+-rw-rw-rw-   0        0        0    14396 2023-07-02 16:43:30.000000 pyrepresent-0.2.2/represent/structures.py
+-rw-rw-rw-   0        0        0       30 2023-03-28 10:51:56.000000 pyrepresent-0.2.2/requirements-dev.txt
+-rw-rw-rw-   0        0        0       21 2023-03-28 10:51:53.000000 pyrepresent-0.2.2/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-02 16:45:02.224856 pyrepresent-0.2.2/setup.cfg
+-rw-rw-rw-   0        0        0     1682 2023-07-02 16:45:00.000000 pyrepresent-0.2.2/setup.py
+-rw-rw-rw-   0        0        0     1361 2023-07-02 15:56:18.000000 pyrepresent-0.2.2/test.py
```

### Comparing `pyrepresent-0.2.1/PKG-INFO` & `pyrepresent-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrepresent
-Version: 0.2.1
+Version: 0.2.2
 Summary: A module for object and model representations as strings, with vast configurations, colors, hidden and protected values, assignment operations, memory addresses and more.
 Home-page: https://github.com/Shahaf-F-S/represent
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyrepresent-0.2.1/README.md` & `pyrepresent-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `pyrepresent-0.2.1/build.py` & `pyrepresent-0.2.2/build.py`

 * *Files identical despite different names*

### Comparing `pyrepresent-0.2.1/pyproject.toml` & `pyrepresent-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'pyrepresent'
-version = '0.2.1'
+version = '0.2.2'
 description = 'A module for object and model representations as strings, with vast configurations, colors, hidden and protected values, assignment operations, memory addresses and more.'
 classifiers = [
 	'Intended Audience :: Developers',
 	'License :: OSI Approved :: MIT License',
 	'Programming Language :: Python',
 	'Programming Language :: Python :: 3',
 	'Programming Language :: Python :: 3.8',
```

### Comparing `pyrepresent-0.2.1/pyrepresent.egg-info/PKG-INFO` & `pyrepresent-0.2.2/pyrepresent.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrepresent
-Version: 0.2.1
+Version: 0.2.2
 Summary: A module for object and model representations as strings, with vast configurations, colors, hidden and protected values, assignment operations, memory addresses and more.
 Home-page: https://github.com/Shahaf-F-S/represent
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyrepresent-0.2.1/represent/colors.py` & `pyrepresent-0.2.2/represent/colors.py`

 * *Files identical despite different names*

### Comparing `pyrepresent-0.2.1/represent/indentation.py` & `pyrepresent-0.2.2/represent/indentation.py`

 * *Files identical despite different names*

### Comparing `pyrepresent-0.2.1/represent/object.py` & `pyrepresent-0.2.2/represent/object.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 import numpy as np
 
 from represent.indentation import indent
 from represent.colors import colorize
 from represent.structures import (
     structures, HiddenStructure, StringWrapper,
     CircularReferenceStructure, TypeStructure,
-    ObjectStructure, FunctionStructure, hashable_structures
+    FunctionStructure, hashable_structures
 )
 
 __all__ = [
     "to_string",
     "BaseModel",
     "Modifiers",
     "unwrap"
@@ -306,14 +306,55 @@
         )
 
     else:
         ids[data_id] = (data if legalize else StringWrapper(repr(data)))
     # end if
 # end early_cache
 
+def wrap_object(
+        data: Any, /, *,
+        assignment: Optional[Any] = None,
+        assign: Optional[bool] = None,
+        legalize: Optional[bool] = None,
+        color: Optional[bool] = None
+) -> Any:
+    """
+    Wraps the object with the wrapper class.
+
+    :param data: The data of the object.
+    :param assignment: The assignment value.
+    :param assign: The value to assign values to classes and attributes.
+    :param legalize: The value to legalize the output repr.
+    :param color: The value to color the repr.
+
+    :return: The wrapped object.
+    """
+
+    if assign and (data is not None):
+        if type(data) in hashable_structures:
+            data = hashable_structures[type(data)](data)
+
+        else:
+            data = structures[type(data)](data)
+        # end if
+
+        if assignment is not None:
+            data.__type__ = assignment
+
+            if not legalize:
+                data.__value__ = assignment
+            # end if
+        # end if
+
+        data.__color__ = color
+    # end if
+
+    return data
+# end wrap_object
+
 def unwrap(
         data: Any, /, *,
         assign: Optional[bool] = False,
         protected: Optional[bool] = False,
         legalize: Optional[bool] = False,
         force: Optional[bool] = False,
         defined: Optional[bool] = None,
@@ -379,15 +420,18 @@
             return repr(data)
         # end if
 
         return FunctionStructure(data)
     # end if
 
     if isinstance(data, (pd.DataFrame, np.ndarray)):
-        return ObjectStructure(data) if not (legalize and assign) else data
+        return wrap_object(
+            data, assignment=data, assign=assign,
+            legalize=legalize, color=color
+        )
     # end if
 
     if isinstance(data, (HiddenStructure, StringWrapper)):
         return repr(data) if legalize else StringWrapper(repr(data))
     # end if
 
     ids = ids or {}
@@ -465,32 +509,18 @@
                 )
             )
         # end for
 
         results = type(data)(results)
     # end if
 
-    if assign and (results is not None):
-        if type(results) in hashable_structures:
-            results = hashable_structures[type(results)](results)
-
-        else:
-            results = structures[type(results)](results)
-        # end if
-
-        if assignment is not None:
-            results.__type__ = assignment
-
-            if not legalize:
-                results.__value__ = assignment
-            # end if
-        # end if
-
-        results.__color__ = color
-    # end if
+    results = wrap_object(
+        results, assignment=assignment, assign=assign,
+        legalize=legalize, color=color
+    )
 
     ids[data_id] = results
 
     return results
 # end unwrap
 
 def to_string(obj: Any, /, modifiers: Optional[Modifiers] = None) -> str:
@@ -511,13 +541,13 @@
         else:
             modifiers = Modifiers()
         # end if
     # end if
 
     data = indent(str(unwrap(obj, **modifiers)))
 
-    if modifiers.color:
+    if modifiers.assign and modifiers.color:
         data = colorize(data)
     # end if
 
     return data
 # end to_string
```

### Comparing `pyrepresent-0.2.1/represent/structures.py` & `pyrepresent-0.2.2/represent/structures.py`

 * *Files 9% similar despite different names*

```diff
@@ -204,45 +204,36 @@
     def __init__(self, value: object) -> None:
         """
         Defines the class attributes.
 
         :param value: The value to hold.
         """
 
-        self.value = value
+        self.__value__ = value
+        self.__type__ = type(value)
     # end __init__
 
     def __str__(self) -> str:
         """
         Returns a string to represent the object.
 
         :return: A string representation for the commands of the object.
         """
 
         string = (
-            f"<{type(self.value).__module__}."
-            f"{type(self.value).__name__} "
-            f"object at 0x00000{str(hex(id(self.value))).upper()[2:]}>"
+            f"<{type(self.__value__).__module__}."
+            f"{type(self.__value__).__name__} "
+            f"object at 0x00000{str(hex(id(self.__value__))).upper()[2:]}>"
         )
 
-        data = Colors.color_class(string)
-        data = Colors.color_repr_address(data)
-        data = Colors.color_repr(data, self.value)
-
-        content = ""
-
-        if isinstance(self.value, pd.DataFrame):
-            content = ', '.join([f'|{row}|' for row in str(self.value).split('\n')])
-
-        elif isinstance(self.value, np.ndarray):
-            # noinspection PyUnresolvedReferences
-            content = str(self.value.tolist())
-        # end if
+        data = Colors.color_class(string, color=self.__color__)
+        data = Colors.color_repr_address(data, color=self.__color__)
+        data = Colors.color_repr(data, self.__value__, color=self.__color__)
 
-        return f"{data}({content})"
+        return f"{data}()"
     # end __str__
 # end ObjectStructure
 
 class SetStructure(DataStructure, set):
     """A class to represent a structure."""
 
     def __str__(self) -> str:
@@ -551,14 +542,15 @@
     list: HashableList,
     set: HashableSet
 }
 
 structures = {
     set: SetStructure, list: ListStructure,
     tuple: TupleStructure, dict: DictStructure,
-    type: TypeStructure, types.FunctionType: FunctionStructure
+    type: TypeStructure, types.FunctionType: FunctionStructure,
+    pd.DataFrame: ObjectStructure, np.ndarray: ObjectStructure
 }
 
 structure_types = (
     SetStructure, DictStructure, ListStructure,
     TupleStructure, FunctionStructure
 )
```

### Comparing `pyrepresent-0.2.1/setup.py` & `pyrepresent-0.2.2/setup.py`

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
-        version='0.2.1',
+        version='0.2.2',
         description=(
             "A module for object and model representations as strings, "
             "with vast configurations, colors, hidden and protected values, "
             "assignment operations, memory addresses and more."
         ),
         license='MIT',
         author="Shahaf Frank-Shapir",
```

### Comparing `pyrepresent-0.2.1/test.py` & `pyrepresent-0.2.2/test.py`

 * *Files identical despite different names*

