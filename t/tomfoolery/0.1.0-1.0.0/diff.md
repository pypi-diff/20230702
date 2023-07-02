# Comparing `tmp/tomfoolery-0.1.0.tar.gz` & `tmp/tomfoolery-1.0.0.tar.gz`

## Comparing `tomfoolery-0.1.0.tar` & `tomfoolery-1.0.0.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 tomfoolery-0.1.0/src/tomfoolery/__init__.py
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 tomfoolery-0.1.0/src/tomfoolery/_dump.py
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 tomfoolery-0.1.0/src/tomfoolery/_load.py
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 tomfoolery-0.1.0/src/tomfoolery/cli.py
--rw-r--r--   0        0        0     6276 2020-02-02 00:00:00.000000 tomfoolery-0.1.0/src/tomfoolery/engine.py
--rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 tomfoolery-0.1.0/src/tomfoolery/utilities.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 tomfoolery-0.1.0/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 tomfoolery-0.1.0/LICENSE.txt
--rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 tomfoolery-0.1.0/README.md
--rw-r--r--   0        0        0     1164 2020-02-02 00:00:00.000000 tomfoolery-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1783 2020-02-02 00:00:00.000000 tomfoolery-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 tomfoolery-1.0.0/CHANGELOG.md
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 tomfoolery-1.0.0/src/tomfoolery/__init__.py
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 tomfoolery-1.0.0/src/tomfoolery/_dump.py
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 tomfoolery-1.0.0/src/tomfoolery/_load.py
+-rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 tomfoolery-1.0.0/src/tomfoolery/cli.py
+-rw-r--r--   0        0        0     8827 2020-02-02 00:00:00.000000 tomfoolery-1.0.0/src/tomfoolery/engine.py
+-rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 tomfoolery-1.0.0/src/tomfoolery/utilities.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 tomfoolery-1.0.0/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 tomfoolery-1.0.0/LICENSE.txt
+-rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 tomfoolery-1.0.0/README.md
+-rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 tomfoolery-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1811 2020-02-02 00:00:00.000000 tomfoolery-1.0.0/PKG-INFO
```

### Comparing `tomfoolery-0.1.0/src/tomfoolery/engine.py` & `tomfoolery-1.0.0/src/tomfoolery/engine.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,33 @@
-import ast
 from typing import Any
 
+import ast_comments as ast
 import black
 import isort
 from pathier import Pathier, Pathish
 
 from tomfoolery import utilities
 
 root = Pathier(__file__).parent
 
 
 class TomFoolery:
-    def __init__(self):
-        self.module = ast.Module([], [])
-        self.imports: list[ast.ImportFrom | ast.Import] = []
-        self.classes: list[ast.ClassDef] = []
+    def __init__(self, module: ast.Module | None = None):
+        """If no `module` is given, an empty new one will be created."""
+        self.module: ast.Module = module or ast.Module([], [])
+
+    @property
+    def class_names(self) -> list[str]:
+        """List of class names in `self.module.body`."""
+        return [node.name for node in self.module.body if type(node) == ast.ClassDef]
 
     @property
     def source(self) -> str:
         """Returns the source code this object represents."""
-        self.module.body = [self.imports, self.classes]  # type: ignore
-        return ast.unparse(self.module)
+        return self.format_str(ast.unparse(self.module))
 
     def format_str(self, code: str) -> str:
         """Sort imports and format with `black`."""
         return black.format_str(isort.api.sort_code_string(code), mode=black.Mode())  # type: ignore
 
     # Seat |===================================== Import Nodes =====================================|
 
@@ -63,39 +66,106 @@
     def dataclass_node(self) -> ast.Name:
         """A node representing `@dataclass`."""
         return ast.Name("dataclass", ast.Load())
 
     @property
     def dump_node(self) -> ast.FunctionDef:
         """The dumping function for the generated `dataclass`."""
-        return self.nodes_from_file(root / "_dump.py")[0]  # type: ignore
+        dump = self.nodes_from_file(root / "_dump.py")[0]
+        return dump if isinstance(dump, ast.FunctionDef) else ast.FunctionDef()
 
     @property
     def load_node(self) -> ast.FunctionDef:
         """The loading function for the generated `dataclass`."""
-        return self.nodes_from_file(root / "_load.py")[0]  # type: ignore
+        load = self.nodes_from_file(root / "_load.py")[0]
+        return load if isinstance(load, ast.FunctionDef) else ast.FunctionDef()
+
+    def add_dataclass(self, dataclass: ast.ClassDef):
+        """Add or merge `dataclass` into `self.module.body`."""
+        if dataclass.name not in self.class_names:
+            self.module.body.append(dataclass)
+        else:
+            classdex = self.class_index(dataclass.name)
+            self.module.body[classdex] = self.merge_dataclasses(self.module.body[classdex], dataclass)  # type: ignore
+
+    def class_index(self, class_name: str) -> int:
+        """Return the `self.module.body` index for a class with `class_name`."""
+        for i, node in enumerate(self.module.body):
+            if isinstance(node, ast.ClassDef) and node.name == class_name:
+                return i
+        return len(self.module.body)
+
+    def fix_order(self):
+        """Reorder `self.module.body` so that definitions preceede instances.
+
+        i.e. A newly added class is defined before another class creates an instance."""
+        new_body = []
+        for node in self.module.body:
+            if isinstance(node, ast.ClassDef):
+                placed = False
+                for i, new_node in enumerate(new_body):
+                    if node.name in ast.unparse(new_node):
+                        new_body.insert(i, node)
+                        placed = True
+                        break
+                if not placed:
+                    new_body.append(node)
+            else:
+                new_body.append(node)
+        self.module.body = new_body
+
+    def last_annassign_index(self, node: ast.ClassDef) -> int:
+        """Return the `node.body` index of the last annotated assignment node.
+        Assumes all annotated assignments are sequential and the first elements of `node`."""
+        for i, child in enumerate(node.body):
+            if not isinstance(child, ast.AnnAssign):
+                return i - 1
+        return len(node.body)
+
+    def merge_dataclasses(
+        self, class1: ast.ClassDef, class2: ast.ClassDef
+    ) -> ast.ClassDef:
+        """Add annotated assignments and functions from `class2` to `class1` and return the result."""
+        funcs = [node.name for node in class1.body if isinstance(node, ast.FunctionDef)]
+        assigns = [
+            node.target.id
+            for node in class1.body
+            if isinstance(node, ast.AnnAssign) and isinstance(node.target, ast.Name)
+        ]
+        for node in class2.body:
+            if isinstance(node, ast.FunctionDef) and node.name not in funcs:
+                class1.body.append(node)
+            elif (
+                isinstance(node, ast.AnnAssign)
+                and isinstance(node.target, ast.Name)
+                and (node.target.id not in assigns)
+            ):
+                class1.body.insert(self.last_annassign_index(class1) + 1, node)
+        return class1
 
     def nodes_from_file(self, file: Pathish) -> list[ast.stmt]:
         """Return ast-parsed module body from `file`."""
-        return ast.parse(Pathier(file).read_text()).body
+        node = ast.parse(Pathier(file).read_text())
+        return node.body if isinstance(node, ast.Module) else []
 
     # Seat |======================================= Builders =======================================|
 
     def annotated_assignments_from_dict(
         self, data: dict[str, Any]
     ) -> list[ast.AnnAssign]:
         """Return a list of annotated assignment nodes built from `data`.
 
         Any values in `data` that are themselves a dictionary, will have a `dataclass` built and inserted in `self.classes`.
 
         The field for that value will be annotated as an instance of that secondary `dataclass`."""
         assigns = []
         for key, val in data.items():
-            if type(val) == dict:
-                self.classes.append(self.build_dataclass(key, val))
+            if isinstance(val, dict):
+                dataclass = self.build_dataclass(key, val)
+                self.add_dataclass(dataclass)
                 assigns.append(
                     self.build_annotated_assignment(
                         key, utilities.key_to_classname(key), False
                     )
                 )
             else:
                 assigns.append(self.build_annotated_assignment(key, val))
@@ -120,42 +190,27 @@
         """Build a `dataclass` with `name` from `data` and insert it into `self.classes`.
 
         If `add_methods` is `True`, `load()` and `dump()` functions will be added to the class."""
         class_ = ast.ClassDef(
             utilities.key_to_classname(name),
             [],
             [],
-            [self.annotated_assignments_from_dict(data)],
+            self.annotated_assignments_from_dict(data),
             [self.dataclass_node],
         )
         if add_methods:
             class_.body.extend([self.load_node, self.dump_node])
         return class_
 
     # Seat |======================================== Main ========================================|
 
     def generate(self, name: str, data: dict[str, Any]) -> str:
         """Generate a `dataclass` with `name` from `data` and return the source code.
 
         Currently, all keys in `data` and any of its nested dictionaries must be valid Python variable names."""
         for node in self.import_nodes:
-            if node not in self.imports:
-                self.imports.append(node)
+            if node not in self.module.body:
+                self.module.body.insert(0, node)
         dataclass = self.build_dataclass(name, data, True)
-        self.classes.append(dataclass)
+        self.add_dataclass(dataclass)
+        self.fix_order()
         return self.source
-
-    def generate_from_file(self, path: Pathish, write_result: bool = False) -> str:
-        """Generate a `dataclass` named after the file `path` points at and return the source code.
-
-        Can be any `.toml` or `.json` file where all keys are valid Python variable names.
-
-        If `write_result` is `True`, the source code will be written to a file of the same name as `path`, but with a `.py` extension."""
-        path = Pathier(path)
-        name = path.stem
-        data = path.loads()
-        src = self.generate(name, data)
-        src = src.replace("filepath", path.name)
-        src = self.format_str(src)
-        if write_result:
-            path.with_suffix(".py").write_text(src)
-        return src
```

### Comparing `tomfoolery-0.1.0/src/tomfoolery/utilities.py` & `tomfoolery-1.0.0/src/tomfoolery/utilities.py`

 * *Files identical despite different names*

### Comparing `tomfoolery-0.1.0/LICENSE.txt` & `tomfoolery-1.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tomfoolery-0.1.0/README.md` & `tomfoolery-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `tomfoolery-0.1.0/pyproject.toml` & `tomfoolery-1.0.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "tomfoolery"
 description = "CLI to generate Python dataclasses that model and load toml files (or other can-representated-as-a-dict files)"
-version = "0.1.0"
+version = "1.0.0"
 requires-python = ">=3.10"
-dependencies = ["pathier", "black", "dacite", "typing_extensions", "pytest", "isort"]
+dependencies = ["pathier", "black", "dacite", "typing_extensions", "pytest", "isort", "ast_comments"]
 readme = "README.md"
 keywords = ["dataclass", "dataclasses", "toml", "json"]
 classifiers = ["Programming Language :: Python :: 3", "License :: OSI Approved :: MIT License", "Operating System :: OS Independent"]
 
 [[project.authors]]
 name = "Matt Manes"
 email = "mattmanes@pm.me"
```

### Comparing `tomfoolery-0.1.0/PKG-INFO` & `tomfoolery-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: tomfoolery
-Version: 0.1.0
+Version: 1.0.0
 Summary: CLI to generate Python dataclasses that model and load toml files (or other can-representated-as-a-dict files)
 Project-URL: Homepage, https://github.com/matt-manes/tomfoolery
 Project-URL: Documentation, https://github.com/matt-manes/tomfoolery/tree/main/docs
 Project-URL: Source code, https://github.com/matt-manes/tomfoolery/tree/main/src/tomfoolery
 Author-email: Matt Manes <mattmanes@pm.me>
 License-File: LICENSE.txt
 Keywords: dataclass,dataclasses,json,toml
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
+Requires-Dist: ast-comments
 Requires-Dist: black
 Requires-Dist: dacite
 Requires-Dist: isort
 Requires-Dist: pathier
 Requires-Dist: pytest
 Requires-Dist: typing-extensions
 Description-Content-Type: text/markdown
```

