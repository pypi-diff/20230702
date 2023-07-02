# Comparing `tmp/pyrepresent-0.1.4.tar.gz` & `tmp/pyrepresent-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrepresent-0.1.4.tar", last modified: Sat Jul  1 08:08:55 2023, max compression
+gzip compressed data, was "pyrepresent-0.2.0.tar", last modified: Sun Jul  2 15:37:13 2023, max compression
```

## Comparing `pyrepresent-0.1.4.tar` & `pyrepresent-0.2.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-07-01 08:08:55.463804 pyrepresent-0.1.4/
--rw-rw-rw-   0        0        0      115 2023-07-01 08:08:55.000000 pyrepresent-0.1.4/MANIFEST.in
--rw-rw-rw-   0        0        0     5268 2023-07-01 08:08:55.463804 pyrepresent-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     4389 2023-03-21 18:58:55.000000 pyrepresent-0.1.4/README.md
--rw-rw-rw-   0        0        0    12920 2023-03-17 11:12:17.000000 pyrepresent-0.1.4/build.py
--rw-rw-rw-   0        0        0      715 2023-07-01 08:08:45.000000 pyrepresent-0.1.4/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-07-01 08:08:55.459803 pyrepresent-0.1.4/pyrepresent.egg-info/
--rw-rw-rw-   0        0        0     5268 2023-07-01 08:08:55.000000 pyrepresent-0.1.4/pyrepresent.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      365 2023-07-01 08:08:55.000000 pyrepresent-0.1.4/pyrepresent.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-01 08:08:55.000000 pyrepresent-0.1.4/pyrepresent.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2023-07-01 08:08:55.000000 pyrepresent-0.1.4/pyrepresent.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-01 08:08:55.000000 pyrepresent-0.1.4/pyrepresent.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-01 08:08:55.462804 pyrepresent-0.1.4/represent/
--rw-rw-rw-   0        0        0       85 2023-03-09 09:17:11.000000 pyrepresent-0.1.4/represent/__init__.py
--rw-rw-rw-   0        0        0     2133 2023-05-15 13:38:04.000000 pyrepresent-0.1.4/represent/indentation.py
--rw-rw-rw-   0        0        0    20230 2023-07-01 08:07:33.000000 pyrepresent-0.1.4/represent/object.py
--rw-rw-rw-   0        0        0    21509 2023-07-01 08:08:23.000000 pyrepresent-0.1.4/represent/structures.py
--rw-rw-rw-   0        0        0       30 2023-03-28 10:51:56.000000 pyrepresent-0.1.4/requirements-dev.txt
--rw-rw-rw-   0        0        0       21 2023-03-28 10:51:53.000000 pyrepresent-0.1.4/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-01 08:08:55.464804 pyrepresent-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0     1682 2023-07-01 08:08:41.000000 pyrepresent-0.1.4/setup.py
--rw-rw-rw-   0        0        0     1028 2023-06-30 19:49:35.000000 pyrepresent-0.1.4/test.py
+drwxrwxrwx   0        0        0        0 2023-07-02 15:37:13.074620 pyrepresent-0.2.0/
+-rw-rw-rw-   0        0        0      115 2023-07-02 15:37:11.000000 pyrepresent-0.2.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2548 2023-07-02 15:37:13.073619 pyrepresent-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1669 2023-07-01 08:58:26.000000 pyrepresent-0.2.0/README.md
+-rw-rw-rw-   0        0        0    12920 2023-03-17 11:12:17.000000 pyrepresent-0.2.0/build.py
+-rw-rw-rw-   0        0        0      715 2023-07-02 15:37:11.000000 pyrepresent-0.2.0/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-07-02 15:37:13.069619 pyrepresent-0.2.0/pyrepresent.egg-info/
+-rw-rw-rw-   0        0        0     2548 2023-07-02 15:37:13.000000 pyrepresent-0.2.0/pyrepresent.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      365 2023-07-02 15:37:13.000000 pyrepresent-0.2.0/pyrepresent.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-02 15:37:13.000000 pyrepresent-0.2.0/pyrepresent.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2023-07-02 15:37:13.000000 pyrepresent-0.2.0/pyrepresent.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-02 15:37:13.000000 pyrepresent-0.2.0/pyrepresent.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-02 15:37:13.072619 pyrepresent-0.2.0/represent/
+-rw-rw-rw-   0        0        0      182 2023-07-02 15:27:45.000000 pyrepresent-0.2.0/represent/__init__.py
+-rw-rw-rw-   0        0        0     2133 2023-05-15 13:38:04.000000 pyrepresent-0.2.0/represent/indentation.py
+-rw-rw-rw-   0        0        0    13656 2023-07-02 15:24:15.000000 pyrepresent-0.2.0/represent/object.py
+-rw-rw-rw-   0        0        0    22999 2023-07-02 15:34:31.000000 pyrepresent-0.2.0/represent/structures.py
+-rw-rw-rw-   0        0        0       30 2023-03-28 10:51:56.000000 pyrepresent-0.2.0/requirements-dev.txt
+-rw-rw-rw-   0        0        0       21 2023-03-28 10:51:53.000000 pyrepresent-0.2.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-02 15:37:13.074620 pyrepresent-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1682 2023-07-02 15:35:07.000000 pyrepresent-0.2.0/setup.py
+-rw-rw-rw-   0        0        0     1258 2023-07-02 15:34:44.000000 pyrepresent-0.2.0/test.py
```

### Comparing `pyrepresent-0.1.4/build.py` & `pyrepresent-0.2.0/build.py`

 * *Files identical despite different names*

### Comparing `pyrepresent-0.1.4/pyproject.toml` & `pyrepresent-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'pyrepresent'
-version = '0.1.4'
+version = '0.2.0'
 description = 'A module for object and model representations as strings, with vast configurations, colors, hidden and protected values, assignment operations, memory addresses and more.'
 classifiers = [
 	'Intended Audience :: Developers',
 	'License :: OSI Approved :: MIT License',
 	'Programming Language :: Python',
 	'Programming Language :: Python :: 3',
 	'Programming Language :: Python :: 3.8',
```

### Comparing `pyrepresent-0.1.4/represent/indentation.py` & `pyrepresent-0.2.0/represent/indentation.py`

 * *Files identical despite different names*

### Comparing `pyrepresent-0.1.4/represent/structures.py` & `pyrepresent-0.2.0/represent/structures.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # structures.py
 
 import datetime as dt
 import types
 import subprocess
 import os
-from typing import Union, Any, Optional, Callable
+from typing import Any, Optional, Callable
 from functools import wraps
 
 from colorama import Fore, Style
 
 import pandas as pd
 import numpy as np
 
@@ -25,15 +25,20 @@
     "TupleStructure",
     "structures",
     "structure_types",
     "colorize",
     "decolorize",
     "TypeStructure",
     "ObjectStructure",
-    "FunctionStructure"
+    "FunctionStructure",
+    "HashableDict",
+    "HashableSet",
+    "HashableList",
+    "FrozenHashable",
+    "hashable_structures"
 ]
 
 def is_proxy_process() -> bool:
     """
     Returns True if the process is running from an IDE.
 
     :return: The boolean value.
@@ -356,26 +361,27 @@
         :param args: Any positional arguments.
         :param kwargs: Any keyword arguments
 
         :returns: The model object.
         """
 
         try:
-            return (
-                constructor(*args, **kwargs).
-                replace("END$$(", Colors.END + "(").
-                replace("END$$,", Colors.END + ",").
-                replace("END$$[", Colors.END + "[").
-                replace("END$${", Colors.END + "{").
+            result: str = constructor(*args, **kwargs)
+            result = (
+                result.
+                replace(")()", ")").
+                replace("}()", "}").
+                replace("]()", "]").
+                replace("$END$$E$END$ND$", Colors.END).
                 replace(Colors.END + Colors.END, Colors.END).
-                replace(f">{Colors.END}END$$(", ">(").
-                replace(f"$E{Colors.END}ND$", Colors.END).
                 replace(Colors.RED + Colors.RED, Colors.RED)
             )
 
+            return result
+
         except RecursionError:
             return repr(CircularReferenceStructure(*args, **kwargs))
         # end try
     # end __str__
 
     return __str__
 # end construct
@@ -467,15 +473,15 @@
         """
         Returns a string to represent the object.
 
         :return: A string representation for the commands of the object.
         """
 
         data = Colors.color_class(repr(self.value).replace("'", ''))
-        data = data.replace('<class', f"<{Colors.CYAN}class{Colors.END} ")
+        data = data.replace('<class', f"<{Colors.CYAN}class{Colors.END}")
         data = Colors.color_repr_address(data)
 
         return data
     # end __str__
 # end TypeStructure
 
 class ObjectStructure(DataStructure):
@@ -571,16 +577,27 @@
             wrapper = ""
         # end if
 
         separator = Colors.color_pairing_operator(
             separator, color=self.color
         )
 
-        content = ', '.join(
-            [
+        addresses = []
+        pairs = []
+
+        for key, value in self.items():
+            if type(key) in hashable_structures:
+                if key.__value__ in addresses:
+                    continue
+                # end if
+
+                addresses.append(key.__value__)
+            # end if
+
+            pairs.append(
                 (
                     str(key) if (type(key) != str)
                     else (
                         Colors.color_key_name(
                             f"{wrapper}{key}{wrapper}", color=self.color
                         )
                         if wrapper == "'" else
@@ -589,17 +606,18 @@
                         )
                     )
                 ) + separator +
                 Colors.color_builtin_value(
                     str(value) if (type(value) != str) else repr(value),
                     value, color=self.color
                 )
-                for key, value in self.items()
-            ]
-        )
+            )
+        # end for
+
+        content = ', '.join(pairs)
 
         if self.__type__ is None:
             return "{" + content + "}"
         # end if
 
         return f"{self.name}({content})"
     # end __str__
@@ -723,18 +741,18 @@
         Returns a string to represent the object.
 
         :return: A string representation for the commands of the object.
         """
 
         return Colors.color_repr_address(
             (
-                    f"<{Colors.CYAN}function{Colors.END}" +
-                    self.name[self.name.find(' '):self.name.find(self.__value__.__name__)] +
-                    f"{Colors.GREEN}{self.__value__.__name__}{Colors.END}" +
-                    self.name[self.name.find(" at "):]
+                f"<{Colors.CYAN}function{Colors.END}" +
+                self.name[self.name.find(' '):self.name.find(self.__value__.__name__)] +
+                f"{Colors.GREEN}{self.__value__.__name__}{Colors.END}" +
+                self.name[self.name.find(" at "):]
             ),
             color=self.color
         )
     # end __str__
 # end FunctionStructure
 
 class CircularReferenceStructure(DataStructure):
@@ -761,14 +779,65 @@
 
         return Colors.color_repr_address(
             f"<circular referenced object: {self.name}>", color=self.color
         )
     # end __str__
 # end CircularReferenceStructure
 
+class FrozenHashable:
+    """A hashable dict structure."""
+
+    def __hash__(self) -> int:
+        """
+        Returns the hash of the signature for hashing the object.
+
+        :return: The hash of the object.
+        """
+
+        return id(self)
+    # end __hash__
+
+    def _immutable(self, *args: Any, **kwargs: Any) -> None:
+        """
+        Collects any arguments and raises an error.
+
+        :param args: Any positional arguments.
+        :param kwargs: Any keyword arguments.
+        """
+
+        raise TypeError(f"{self} is an immutable object if type {type(self)}.")
+    # end __immutable
+
+    __setitem__ = _immutable
+    __delitem__ = _immutable
+    clear = _immutable
+    update = _immutable
+    setdefault = _immutable
+    pop = _immutable
+    popitem = _immutable
+# end HashableDict
+
+class HashableDict(FrozenHashable, DictStructure, dict):
+    """A hashable dict structure."""
+# end HashableDict
+
+class HashableList(FrozenHashable, ListStructure, list):
+    """A hashable list structure."""
+# end HashableDict
+
+class HashableSet(FrozenHashable, SetStructure, set):
+    """A hashable list structure."""
+# end HashableDict
+
+hashable_structures = {
+    dict: HashableDict,
+    list: HashableList,
+    set: HashableSet
+}
+
 def colorize(content: str, /) -> str:
     """
     Colors the string with the pre-written color codes.
 
     :param content: The string to color.
 
     :return: The colored string.
@@ -794,17 +863,14 @@
         content = content.replace(key, "")
         content = content.replace(value, "")
     # end for
 
     return content
 # end uncolor
 
-Structure = Union[
-    SetStructure, DictStructure, ListStructure, TupleStructure
-]
 structures = {
     set: SetStructure, list: ListStructure,
     tuple: TupleStructure, dict: DictStructure,
     type: TypeStructure, types.FunctionType: FunctionStructure
 }
 
 structure_types = (
```

### Comparing `pyrepresent-0.1.4/setup.py` & `pyrepresent-0.2.0/setup.py`

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
-        version='0.1.4',
+        version='0.2.0',
         description=(
             "A module for object and model representations as strings, "
             "with vast configurations, colors, hidden and protected values, "
             "assignment operations, memory addresses and more."
         ),
         license='MIT',
         author="Shahaf Frank-Shapir",
```

### Comparing `pyrepresent-0.1.4/test.py` & `pyrepresent-0.2.0/test.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # test.py
 
 import pandas as pd
 import numpy as np
 
-from represent import BaseModel, to_string
+from represent import BaseModel, indent, unwrap, colorize, to_string
 
 class Model(BaseModel):
 
     def __init__(self) -> None:
 
         self.self = self
         self.type = type(self)
@@ -42,13 +42,16 @@
 # end Data
 
 def main() -> None:
     """Tests the module."""
 
     print(Model())
     print(Data())
-    print(to_string({Data(): 0, Data(): 1}))
+    print(to_string(unwrap(Data(), assign=True)))
+    print(colorize(indent(str(unwrap({Data(): 0, Data(): 1}, assign=True)))))
+    print(to_string(unwrap(Data(), assign=False)))
+    print(to_string(unwrap({Data(): 0, Data(): 1}, assign=False)))
 # end main
 
 if __name__ == "__main__":
     main()
 # end if
```

