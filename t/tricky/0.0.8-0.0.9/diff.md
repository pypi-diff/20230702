# Comparing `tmp/tricky-0.0.8.tar.gz` & `tmp/tricky-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tricky-0.0.8.tar", max compression
+gzip compressed data, was "tricky-0.0.9.tar", max compression
```

## Comparing `tricky-0.0.8.tar` & `tricky-0.0.9.tar`

### file list

```diff
@@ -1,12 +1,11 @@
--rw-r--r--   0        0        0     1078 2023-01-23 14:52:53.743984 tricky-0.0.8/LICENSE
--rw-r--r--   0        0        0     1728 2023-02-21 21:33:34.735742 tricky-0.0.8/README.md
--rw-r--r--   0        0        0     1580 2023-02-21 21:38:57.798991 tricky-0.0.8/pyproject.toml
--rw-r--r--   0        0        0       72 2023-02-21 21:39:29.343308 tricky-0.0.8/tricky/__init__.py
--rw-r--r--   0        0        0      697 2023-01-30 11:47:31.003851 tricky-0.0.8/tricky/iterables.py
--rw-r--r--   0        0        0       54 2023-01-30 10:30:57.933034 tricky-0.0.8/tricky/pydantic/__init__.py
--rw-r--r--   0        0        0      646 2023-01-25 11:15:21.061563 tricky-0.0.8/tricky/pydantic/types.py
--rw-r--r--   0        0        0     3393 2023-02-21 21:26:28.683449 tricky-0.0.8/tricky/typing.py
--rw-r--r--   0        0        0       47 2023-02-20 20:59:58.518907 tricky-0.0.8/tricky/utils/__init__.py
--rw-r--r--   0        0        0      769 2023-02-20 20:59:58.526908 tricky-0.0.8/tricky/utils/decorators.py
--rw-r--r--   0        0        0     2657 1970-01-01 00:00:00.000000 tricky-0.0.8/setup.py
--rw-r--r--   0        0        0     2826 1970-01-01 00:00:00.000000 tricky-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1078 2023-01-23 14:52:53.743984 tricky-0.0.9/LICENSE
+-rw-r--r--   0        0        0     1728 2023-02-21 21:33:34.735742 tricky-0.0.9/README.md
+-rw-r--r--   0        0        0     1580 2023-03-19 18:59:10.824366 tricky-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0       72 2023-03-19 18:59:51.560620 tricky-0.0.9/tricky/__init__.py
+-rw-r--r--   0        0        0      672 2023-02-22 15:39:01.290098 tricky-0.0.9/tricky/iterables.py
+-rw-r--r--   0        0        0       59 2023-02-27 11:33:42.501786 tricky-0.0.9/tricky/pydantic/__init__.py
+-rw-r--r--   0        0        0     1357 2023-02-27 11:36:53.493198 tricky-0.0.9/tricky/pydantic/types.py
+-rw-r--r--   0        0        0     4160 2023-03-19 18:46:55.515786 tricky-0.0.9/tricky/typing.py
+-rw-r--r--   0        0        0       47 2023-02-20 20:59:58.518907 tricky-0.0.9/tricky/utils/__init__.py
+-rw-r--r--   0        0        0      769 2023-02-20 20:59:58.526908 tricky-0.0.9/tricky/utils/decorators.py
+-rw-r--r--   0        0        0     2826 1970-01-01 00:00:00.000000 tricky-0.0.9/PKG-INFO
```

### Comparing `tricky-0.0.8/LICENSE` & `tricky-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `tricky-0.0.8/README.md` & `tricky-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `tricky-0.0.8/pyproject.toml` & `tricky-0.0.9/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tricky"
-version = "0.0.8"
+version = "0.0.9"
 
 authors = ["Alexander Walther <alexander.walther.engineering@gmail.com>"]
 
 description = "A set of useful features to make working with your code easier."
 documentation = ""
 homepage = "https://github.com/Walther-s-Engineering/tricky"
 keywords = ["tools"]
```

### Comparing `tricky-0.0.8/tricky/iterables.py` & `tricky-0.0.9/tricky/iterables.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 import typing as t
 
-from .typing import Bool
+from .typing import Bool, List
 
 __all__ = (
     'filter_item',
     'remove_values_from_iterable',
 )
 
-Item = t.TypeVar('Item', bound=t.Any)
-Iterables = t.Iterable[t.Any]
+Item = t.TypeVar('Item')
+Iterables = t.Iterable[Item]
 
 
 def filter_item(
     items: Iterables,
     condition: t.Callable[..., t.Union[Bool, bool]],
     default: t.Optional[Item] = None,
 ) -> t.Any:
     return next(
         (item for item in items if condition(item) is True),
         default,
     )
 
 
 def remove_values_from_iterable(
-    initial_values: t.Iterable[t.Any],
-    values_to_remove: t.Iterable[t.Any],
-) -> t.List[t.Any]:
+    initial_values: Iterables,
+    values_to_remove: Iterables,
+) -> t.List[Item]:
     return [
         initial_value
         for initial_value in initial_values
         if initial_value not in values_to_remove
     ]
```

### Comparing `tricky-0.0.8/tricky/pydantic/types.py` & `tricky-0.0.9/tricky/pydantic/types.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,51 @@
 import typing as t
 
+from datetime import datetime, timezone
+
 from pydantic.validators import str_validator
+from pydantic.datetime_parse import parse_datetime
+
 from tricky.typing import String
 
 __all__ = (
-    'CommaSeparatedString',
+    'CommaSeparatedStringField',
 )
 
 CallableGenerator = t.Generator[t.Callable[..., t.Any], None, None]
 
 
-class CommaSeparatedString(String):
+class CommaSeparatedStringField(String):
     @classmethod
     def __modify_schema__(cls, field_schema: t.Dict[String, t.Any]) -> None:
         pass
 
     @classmethod
     def __get_validators__(cls) -> CallableGenerator:
         yield str_validator
         yield cls.validate
 
     @classmethod
     def validate(cls, value: t.Union[String]) -> t.List[String]:
         return list(String(val.strip().strip('"')) for val in value.split(','))
+
+
+class UTCDatetimeField(datetime):
+    @classmethod
+    def __modify_schema__(cls, field_schema: t.Dict[String, t.Any]):
+        pass
+
+    @classmethod
+    def __get_validators__(cls) -> CallableGenerator:
+        yield parse_datetime
+        yield cls.ensure_tzinfo
+        yield cls.validate
+
+    @classmethod
+    def ensure_tzinfo(cls, value: datetime) -> datetime:
+        if value.tzinfo is None:
+            return value.replace(tzinfo=timezone.utc)
+        return value.astimezone(timezone.utc)
+
+    @staticmethod
+    def validate(date_time: datetime) -> String:
+        return date_time.isoformat()
```

### Comparing `tricky-0.0.8/tricky/utils/decorators.py` & `tricky-0.0.9/tricky/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `tricky-0.0.8/setup.py` & `tricky-0.0.9/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,34 +1,89 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: tricky
+Version: 0.0.9
+Summary: A set of useful features to make working with your code easier.
+Home-page: https://github.com/Walther-s-Engineering/tricky
+License: MIT
+Keywords: tools
+Author: Alexander Walther
+Author-email: alexander.walther.engineering@gmail.com
+Requires-Python: >=3.8,<4.0
+Classifier: Development Status :: 1 - Planning
+Classifier: Environment :: Console
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Topic :: Utilities
+Provides-Extra: pydantic
+Requires-Dist: pydantic (==1.10.4) ; extra == "pydantic"
+Requires-Dist: typing-extensions (>=4.5.0)
+Description-Content-Type: text/markdown
+
+# tricky - that's about python.
+
+This module is simply a collection of useful code, utilities, and functions to simplify your work with the language and the tasks you solve.
+
+## Collection:
+1. Iterables module `tricky.iterables`
+2. Typing `tricky.typing` (wip)
+
+
+## Examples:
+
+### Iterables
+1. Example of **iterables.filter_item**
+ ```python
+ from tricky.iterables import filter_item
+ 
+ numbers = range(1000)
+ result: int = filter_item(
+     numbers,  # the iterable
+     lambda number: number == 342,  # condition to get your item
+     None,  # the default value to return, if condition not met
+ )
+ print(result)
+ # 342
+ ```
+
+### Typing
+
+1. An example of a simple use of a **TypedList**:
+```python
+from tricky.typing import TypedList
+
+numbers = TypedList[int](1, 2, 3, 4, 5)
+assert isinstance(numbers, (list, TypedList))  # True
+```
+
+But if an element with a different type is passed to the list, an exception will be thrown:
+```python
+from tricky.typing import TypedList
+
+numbers = TypedList[int](1, 2, 3, 'string', 5)
+# ValueError: Passed item "string" of sequence has type <class 'str'>, but annotated type is <class 'int'>
+```
+
+2. An example of a simple use of a **AnnotatedString**
+```python
+from tricky.typing import AnnotatedString
+
+expecting_value = 'example'
+annotated_string = AnnotatedString['example'](expecting_value)
+assert isinstance(AnnotatedString['example'](expecting_value), (str, AnnotatedString))
+```
+But if the annotated value does not match the one passed, an exception will be thrown
+```python
+from tricky.typing import AnnotatedString
+
+bad_value = 'bad_value'
+annotated_string = AnnotatedString['example'](bad_value)
+# ValueError: Annotated and passed values are not equal 'bad_value' != 'example'
+```
 
-packages = \
-['tricky', 'tricky.pydantic', 'tricky.utils']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['typing-extensions>=4.5.0']
-
-extras_require = \
-{'pydantic': ['pydantic==1.10.4']}
-
-setup_kwargs = {
-    'name': 'tricky',
-    'version': '0.0.8',
-    'description': 'A set of useful features to make working with your code easier.',
-    'long_description': '# tricky - that\'s about python.\n\nThis module is simply a collection of useful code, utilities, and functions to simplify your work with the language and the tasks you solve.\n\n## Collection:\n1. Iterables module `tricky.iterables`\n2. Typing `tricky.typing` (wip)\n\n\n## Examples:\n\n### Iterables\n1. Example of **iterables.filter_item**\n ```python\n from tricky.iterables import filter_item\n \n numbers = range(1000)\n result: int = filter_item(\n     numbers,  # the iterable\n     lambda number: number == 342,  # condition to get your item\n     None,  # the default value to return, if condition not met\n )\n print(result)\n # 342\n ```\n\n### Typing\n\n1. An example of a simple use of a **TypedList**:\n```python\nfrom tricky.typing import TypedList\n\nnumbers = TypedList[int](1, 2, 3, 4, 5)\nassert isinstance(numbers, (list, TypedList))  # True\n```\n\nBut if an element with a different type is passed to the list, an exception will be thrown:\n```python\nfrom tricky.typing import TypedList\n\nnumbers = TypedList[int](1, 2, 3, \'string\', 5)\n# ValueError: Passed item "string" of sequence has type <class \'str\'>, but annotated type is <class \'int\'>\n```\n\n2. An example of a simple use of a **AnnotatedString**\n```python\nfrom tricky.typing import AnnotatedString\n\nexpecting_value = \'example\'\nannotated_string = AnnotatedString[\'example\'](expecting_value)\nassert isinstance(AnnotatedString[\'example\'](expecting_value), (str, AnnotatedString))\n```\nBut if the annotated value does not match the one passed, an exception will be thrown\n```python\nfrom tricky.typing import AnnotatedString\n\nbad_value = \'bad_value\'\nannotated_string = AnnotatedString[\'example\'](bad_value)\n# ValueError: Annotated and passed values are not equal \'bad_value\' != \'example\'\n```\n',
-    'author': 'Alexander Walther',
-    'author_email': 'alexander.walther.engineering@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/Walther-s-Engineering/tricky',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'python_requires': '>=3.8,<4.0',
-}
-
-
-setup(**setup_kwargs)
```

