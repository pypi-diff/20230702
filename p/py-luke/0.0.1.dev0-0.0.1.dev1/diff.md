# Comparing `tmp/py_luke-0.0.1.dev0.tar.gz` & `tmp/py_luke-0.0.1.dev1.tar.gz`

## Comparing `py_luke-0.0.1.dev0.tar` & `py_luke-0.0.1.dev1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 py_luke-0.0.1.dev0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 py_luke-0.0.1.dev0/.github/workflows/test-suite.yml
--rw-r--r--   0        0        0    22090 2020-02-02 00:00:00.000000 py_luke-0.0.1.dev0/examples/pet_store.yaml
--rw-r--r--   0        0        0    84785 2020-02-02 00:00:00.000000 py_luke-0.0.1.dev0/images/luke.png
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 py_luke-0.0.1.dev0/luke/__init__.py
--rw-r--r--   0        0        0     4686 2020-02-02 00:00:00.000000 py_luke-0.0.1.dev0/luke/data_generators.py
--rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 py_luke-0.0.1.dev0/luke/format.py
--rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 py_luke-0.0.1.dev0/luke/main.py
--rw-r--r--   0        0        0     3368 2020-02-02 00:00:00.000000 py_luke-0.0.1.dev0/luke/openapi.py
--rw-r--r--   0        0        0     1482 2020-02-02 00:00:00.000000 py_luke-0.0.1.dev0/luke/server_generator.py
--rwxr-xr-x   0        0        0      143 2020-02-02 00:00:00.000000 py_luke-0.0.1.dev0/scripts/build
--rwxr-xr-x   0        0        0      190 2020-02-02 00:00:00.000000 py_luke-0.0.1.dev0/scripts/check
--rwxr-xr-x   0        0        0       23 2020-02-02 00:00:00.000000 py_luke-0.0.1.dev0/scripts/clean
--rwxr-xr-x   0        0        0      150 2020-02-02 00:00:00.000000 py_luke-0.0.1.dev0/scripts/coverage
--rwxr-xr-x   0        0        0      346 2020-02-02 00:00:00.000000 py_luke-0.0.1.dev0/scripts/install
--rwxr-xr-x   0        0        0      239 2020-02-02 00:00:00.000000 py_luke-0.0.1.dev0/scripts/test
--rw-r--r--   0        0        0      927 2020-02-02 00:00:00.000000 py_luke-0.0.1.dev0/tests/test_data_generators.py
--rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 py_luke-0.0.1.dev0/.gitignore
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 py_luke-0.0.1.dev0/LICENSE
--rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 py_luke-0.0.1.dev0/README.md
--rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 py_luke-0.0.1.dev0/pyproject.toml
--rw-r--r--   0        0        0     2205 2020-02-02 00:00:00.000000 py_luke-0.0.1.dev0/PKG-INFO
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 py_luke-0.0.1.dev1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    22090 2020-02-02 00:00:00.000000 py_luke-0.0.1.dev1/pet-store-openapi.yaml
+-rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 py_luke-0.0.1.dev1/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 py_luke-0.0.1.dev1/.github/workflows/test-suite.yml
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 py_luke-0.0.1.dev1/luke/__init__.py
+-rw-r--r--   0        0        0     4687 2020-02-02 00:00:00.000000 py_luke-0.0.1.dev1/luke/data_generators.py
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 py_luke-0.0.1.dev1/luke/format.py
+-rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 py_luke-0.0.1.dev1/luke/main.py
+-rw-r--r--   0        0        0     3368 2020-02-02 00:00:00.000000 py_luke-0.0.1.dev1/luke/openapi.py
+-rw-r--r--   0        0        0     1482 2020-02-02 00:00:00.000000 py_luke-0.0.1.dev1/luke/server_generator.py
+-rwxr-xr-x   0        0        0      143 2020-02-02 00:00:00.000000 py_luke-0.0.1.dev1/scripts/build
+-rwxr-xr-x   0        0        0      190 2020-02-02 00:00:00.000000 py_luke-0.0.1.dev1/scripts/check
+-rwxr-xr-x   0        0        0       31 2020-02-02 00:00:00.000000 py_luke-0.0.1.dev1/scripts/clean
+-rwxr-xr-x   0        0        0      150 2020-02-02 00:00:00.000000 py_luke-0.0.1.dev1/scripts/coverage
+-rwxr-xr-x   0        0        0      346 2020-02-02 00:00:00.000000 py_luke-0.0.1.dev1/scripts/install
+-rwxr-xr-x   0        0        0      273 2020-02-02 00:00:00.000000 py_luke-0.0.1.dev1/scripts/test
+-rw-r--r--   0        0        0     4162 2020-02-02 00:00:00.000000 py_luke-0.0.1.dev1/tests/test_data_generators.py
+-rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 py_luke-0.0.1.dev1/.gitignore
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 py_luke-0.0.1.dev1/LICENSE
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 py_luke-0.0.1.dev1/README.md
+-rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 py_luke-0.0.1.dev1/pyproject.toml
+-rw-r--r--   0        0        0     2115 2020-02-02 00:00:00.000000 py_luke-0.0.1.dev1/PKG-INFO
```

### Comparing `py_luke-0.0.1.dev0/.github/workflows/test-suite.yml` & `py_luke-0.0.1.dev1/.github/workflows/test-suite.yml`

 * *Files identical despite different names*

### Comparing `py_luke-0.0.1.dev0/examples/pet_store.yaml` & `py_luke-0.0.1.dev1/pet-store-openapi.yaml`

 * *Files identical despite different names*

### Comparing `py_luke-0.0.1.dev0/luke/data_generators.py` & `py_luke-0.0.1.dev1/luke/data_generators.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 MAXIMUM_INT32 = 32_767
 MINIMUM_INT64 =  -2_147_483_648
 MAXIMUM_INT64 = 2_147_483_647
 
 
 class FieldGenerator:
     def gen_data(self, spec: dict) -> Any:
-        raise NotImplementedError()
+        raise NotImplementedError()   # pragma: no cover
 
 
 def register_field_generator(name: str, generator: Type[FieldGenerator]):
     global _field_generator_registry
     _field_generator_registry[name] = generator
 
 
@@ -50,16 +50,15 @@
             maximum = spec.get("maximum", MAXIMUM_INT32)
 
         return int(super().gen_data({"minimum": minimum, "maximum": maximum, "format": format}))
 
 
 class FloatFieldGenerator(NumberFieldGenerator):
     def gen_data(self, spec) -> float:
-        format = spec.get("format", "float")
-        return super().gen_data({**spec, "format": format})
+        return super().gen_data({**spec, "format": "float"})
 
 
 class StringFieldGenerator(FieldGenerator):
     def gen_data(self, spec) -> str:
         pattern = spec.get("pattern")
         
         if pattern:
@@ -115,15 +114,15 @@
             item = generator_cls().gen_data(item_spec)
             items.append(item)
         return items
 
 
 class BooleanFieldGenerator(FieldGenerator):
     def gen_data(self, spec):
-        return True
+        return random.choice([True, False])
 
 
 class Generator:
     def gen_data(self, spec: dict):
         data_type = spec.get("type")
         if data_type is None:
             raise ValueError("Type is missing")
```

### Comparing `py_luke-0.0.1.dev0/luke/format.py` & `py_luke-0.0.1.dev1/luke/format.py`

 * *Files identical despite different names*

### Comparing `py_luke-0.0.1.dev0/luke/main.py` & `py_luke-0.0.1.dev1/luke/main.py`

 * *Files identical despite different names*

### Comparing `py_luke-0.0.1.dev0/luke/openapi.py` & `py_luke-0.0.1.dev1/luke/openapi.py`

 * *Files identical despite different names*

### Comparing `py_luke-0.0.1.dev0/luke/server_generator.py` & `py_luke-0.0.1.dev1/luke/server_generator.py`

 * *Files identical despite different names*

### Comparing `py_luke-0.0.1.dev0/.gitignore` & `py_luke-0.0.1.dev1/.gitignore`

 * *Files identical despite different names*

### Comparing `py_luke-0.0.1.dev0/LICENSE` & `py_luke-0.0.1.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `py_luke-0.0.1.dev0/README.md` & `py_luke-0.0.1.dev1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-![Lucky Luke](./images/luke.png)
+![Lucky Luke](https://i.ibb.co/vL1MmML/luke.png)
 
 ![GitHub Workflow Status (with event)](https://img.shields.io/github/actions/workflow/status/magiskboy/luke/test-suite.yml)
 ![GitHub commit activity (branch)](https://img.shields.io/github/commit-activity/w/magiskboy/luke)
 ![Codecov](https://img.shields.io/codecov/c/github/magiskboy/luke)
 ![PyPI - Downloads](https://img.shields.io/pypi/dd/py-luke)
 ![GitHub](https://img.shields.io/github/license/magiskboy/luke)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/py-luke)
```

### Comparing `py_luke-0.0.1.dev0/pyproject.toml` & `py_luke-0.0.1.dev1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -42,31 +42,25 @@
     "mypy",
     "ruff",
     "pytest==7.3.1",
     "pytest-cov==4.0.0",
     "types-PyYAML",
 ]
 
-publish = [
-    "twine",
-    "build"
-]
-
 [project.scripts]
 luke = "luke.main:cli"
 
 [project-urls]
 Homepage = "https://github.com/magiskboy/luke"
 
 [tool.hatch.version]
 path = "luke/__init__.py"
 
 [tool.mypy]
 ignore_missing_imports = true
-# explicit_package_bases = true
 check_untyped_defs = true
 
 [tool.coverage.run]
 omit = ["tests/*"]
 
 [tool.coverage.path]
 source = "luke"
```

### Comparing `py_luke-0.0.1.dev0/PKG-INFO` & `py_luke-0.0.1.dev1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-luke
-Version: 0.0.1.dev0
+Version: 0.0.1.dev1
 Summary: Mock server for OpenAPI documentation
 Author-email: Nguyen Khac Thanh <nguyenkhacthanh244@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
 Classifier: Framework :: AnyIO
@@ -28,20 +28,17 @@
 Provides-Extra: dev
 Requires-Dist: mypy; extra == 'dev'
 Requires-Dist: pre-commit; extra == 'dev'
 Requires-Dist: pytest-cov==4.0.0; extra == 'dev'
 Requires-Dist: pytest==7.3.1; extra == 'dev'
 Requires-Dist: ruff; extra == 'dev'
 Requires-Dist: types-pyyaml; extra == 'dev'
-Provides-Extra: publish
-Requires-Dist: build; extra == 'publish'
-Requires-Dist: twine; extra == 'publish'
 Description-Content-Type: text/markdown
 
-![Lucky Luke](./images/luke.png)
+![Lucky Luke](https://i.ibb.co/vL1MmML/luke.png)
 
 ![GitHub Workflow Status (with event)](https://img.shields.io/github/actions/workflow/status/magiskboy/luke/test-suite.yml)
 ![GitHub commit activity (branch)](https://img.shields.io/github/commit-activity/w/magiskboy/luke)
 ![Codecov](https://img.shields.io/codecov/c/github/magiskboy/luke)
 ![PyPI - Downloads](https://img.shields.io/pypi/dd/py-luke)
 ![GitHub](https://img.shields.io/github/license/magiskboy/luke)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/py-luke)
```

