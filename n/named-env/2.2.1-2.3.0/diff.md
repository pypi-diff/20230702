# Comparing `tmp/named_env-2.2.1.tar.gz` & `tmp/named_env-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "named_env-2.2.1.tar", max compression
+gzip compressed data, was "named_env-2.3.0.tar", max compression
```

## Comparing `named_env-2.2.1.tar` & `named_env-2.3.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1057 2023-06-27 15:25:43.958896 named_env-2.2.1/LICENSE
--rw-r--r--   0        0        0      525 2023-06-27 15:25:43.958958 named_env-2.2.1/README.md
--rw-r--r--   0        0        0     3738 2023-07-02 14:03:09.568072 named_env-2.2.1/pyproject.toml
--rw-r--r--   0        0        0      439 2023-06-27 16:12:37.375261 named_env-2.2.1/src/named_env/__init__.py
--rw-r--r--   0        0        0      674 2023-06-27 16:12:37.372785 named_env-2.2.1/src/named_env/exceptions.py
--rw-r--r--   0        0        0      436 2023-06-27 15:25:43.959639 named_env-2.2.1/src/named_env/namespace.py
--rw-r--r--   0        0        0        0 2023-06-27 15:25:43.959664 named_env-2.2.1/src/named_env/py.typed
--rw-r--r--   0        0        0     5659 2023-07-02 13:41:06.947540 named_env-2.2.1/src/named_env/variables.py
--rw-r--r--   0        0        0      328 2023-06-27 15:25:43.959804 named_env-2.2.1/src/named_env/version.py
--rw-r--r--   0        0        0     1198 1970-01-01 00:00:00.000000 named_env-2.2.1/setup.py
--rw-r--r--   0        0        0     1216 1970-01-01 00:00:00.000000 named_env-2.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1057 2023-06-27 15:25:43.958896 named_env-2.3.0/LICENSE
+-rw-r--r--   0        0        0      525 2023-06-27 15:25:43.958958 named_env-2.3.0/README.md
+-rw-r--r--   0        0        0     3738 2023-07-02 20:29:33.035596 named_env-2.3.0/pyproject.toml
+-rw-r--r--   0        0        0      439 2023-06-27 16:12:37.375261 named_env-2.3.0/src/named_env/__init__.py
+-rw-r--r--   0        0        0      674 2023-06-27 16:12:37.372785 named_env-2.3.0/src/named_env/exceptions.py
+-rw-r--r--   0        0        0      534 2023-07-02 20:13:19.168908 named_env-2.3.0/src/named_env/namespace.py
+-rw-r--r--   0        0        0        0 2023-06-27 15:25:43.959664 named_env-2.3.0/src/named_env/py.typed
+-rw-r--r--   0        0        0     5925 2023-07-02 20:13:19.174173 named_env-2.3.0/src/named_env/variables.py
+-rw-r--r--   0        0        0      328 2023-06-27 15:25:43.959804 named_env-2.3.0/src/named_env/version.py
+-rw-r--r--   0        0        0     1198 1970-01-01 00:00:00.000000 named_env-2.3.0/setup.py
+-rw-r--r--   0        0        0     1216 1970-01-01 00:00:00.000000 named_env-2.3.0/PKG-INFO
```

### Comparing `named_env-2.2.1/LICENSE` & `named_env-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `named_env-2.2.1/README.md` & `named_env-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `named_env-2.2.1/pyproject.toml` & `named_env-2.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "named-env"
-version = "2.2.1"
+version = "2.3.0"
 description = "Class-based environment variables typed specification"
 license = "MIT"
 authors = [
     "Artem Novikov <artnew@list.ru>",
 ]
 readme = "README.md"
 repository = "https://github.com/reartnew/named-env"
```

### Comparing `named_env-2.2.1/src/named_env/exceptions.py` & `named_env-2.3.0/src/named_env/exceptions.py`

 * *Files identical despite different names*

### Comparing `named_env-2.2.1/src/named_env/variables.py` & `named_env-2.3.0/src/named_env/variables.py`

 * *Files 16% similar despite different names*

```diff
@@ -29,26 +29,28 @@
 
 
 class BaseVariableMixin:
     """Common ancestor for all variables classes"""
 
     _choice: t.Optional[t.Sequence] = None
 
-    def __set_name__(self, owner, name):
-        self._name = name
+    def __set_name__(self, owner: type, name: str):
+        self._name: t.Optional[str] = name
+        self._namespace = owner if issubclass(owner, EnvironmentNamespace) else None
 
     def __get__(self, obj, objtype=None):
-        if self._value is sentinel:
-            env = (
-                obj.environ
-                if isinstance(obj, EnvironmentNamespace)
-                else objtype.environ
-                if issubclass(objtype, EnvironmentNamespace)
-                else os.environ
-            )
+        namespace: t.Union[t.Type[EnvironmentNamespace], EnvironmentNamespace, None] = (
+            obj
+            if isinstance(obj, EnvironmentNamespace)
+            else objtype
+            if issubclass(objtype, EnvironmentNamespace)
+            else None
+        )
+        if self._value is sentinel or namespace is not None and not namespace.cache_values:
+            env = (namespace or os).environ
             if self._name in env:
                 self._set_value(env[self._name])
             elif isinstance(self, OptionalVariableMixin):
                 self._set_value(self.default)
             elif isinstance(self, RequiredVariableMixin):
                 raise MissingVariableError(variable=self._name, description=self.description)
         return self._value
@@ -74,14 +76,15 @@
     def __new__(cls, *args, **kwargs) -> t.Any:
         choice: t.Optional[t.Sequence] = kwargs.pop("choice", None)
         if choice is not None and not isinstance(choice, t.Sequence):
             raise ValueError(f"'choice' argument must be a sequence (got {type(choice)!r})")
         obj = cls._get_base_class().__new__(cls, *args, **kwargs)  # noqa
         obj._choice = choice
         obj._name = None
+        obj._namespace = None
         obj._value = sentinel
         return obj
 
     @classmethod
     def cast(cls, value):
         """Transform environment string value into desired type"""
         return cls._get_base_class()(value)
```

### Comparing `named_env-2.2.1/setup.py` & `named_env-2.3.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 ['named_env']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'named-env',
-    'version': '2.2.1',
+    'version': '2.3.0',
     'description': 'Class-based environment variables typed specification',
     'long_description': '# named-env\n\nClass-based environment variables typed specification.\n\n## Installation\n\n```shell\npip install named-env\n```\n\n## Usage example\n\n```python\nfrom named_env import EnvironmentNamespace, RequiredInteger\nimport os\n\n\nclass WebApplicationEnvironmentNamespace(EnvironmentNamespace):\n    WEB_SERVER_PORT = RequiredInteger()\n\n\nenv = WebApplicationEnvironmentNamespace()\n\nif __name__ == "__main__":\n    os.environ["WEB_SERVER_PORT"] = "80"\n    print(env.WEB_SERVER_PORT)  # 80\n    print(type(env.WEB_SERVER_PORT))  # int\n```\n',
     'author': 'Artem Novikov',
     'author_email': 'artnew@list.ru',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/reartnew/named-env',
```

### Comparing `named_env-2.2.1/PKG-INFO` & `named_env-2.3.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: named-env
-Version: 2.2.1
+Version: 2.3.0
 Summary: Class-based environment variables typed specification
 Home-page: https://github.com/reartnew/named-env
 License: MIT
 Author: Artem Novikov
 Author-email: artnew@list.ru
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

