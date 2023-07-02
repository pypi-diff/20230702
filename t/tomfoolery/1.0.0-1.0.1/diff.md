# Comparing `tmp/tomfoolery-1.0.0.tar.gz` & `tmp/tomfoolery-1.0.1.tar.gz`

## Comparing `tomfoolery-1.0.0.tar` & `tomfoolery-1.0.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 tomfoolery-1.0.0/CHANGELOG.md
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 tomfoolery-1.0.0/src/tomfoolery/__init__.py
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 tomfoolery-1.0.0/src/tomfoolery/_dump.py
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 tomfoolery-1.0.0/src/tomfoolery/_load.py
--rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 tomfoolery-1.0.0/src/tomfoolery/cli.py
--rw-r--r--   0        0        0     8827 2020-02-02 00:00:00.000000 tomfoolery-1.0.0/src/tomfoolery/engine.py
--rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 tomfoolery-1.0.0/src/tomfoolery/utilities.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 tomfoolery-1.0.0/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 tomfoolery-1.0.0/LICENSE.txt
--rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 tomfoolery-1.0.0/README.md
--rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 tomfoolery-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     1811 2020-02-02 00:00:00.000000 tomfoolery-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 tomfoolery-1.0.1/CHANGELOG.md
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 tomfoolery-1.0.1/src/tomfoolery/__init__.py
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 tomfoolery-1.0.1/src/tomfoolery/_dump.py
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 tomfoolery-1.0.1/src/tomfoolery/_load.py
+-rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 tomfoolery-1.0.1/src/tomfoolery/cli.py
+-rw-r--r--   0        0        0     9837 2020-02-02 00:00:00.000000 tomfoolery-1.0.1/src/tomfoolery/engine.py
+-rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 tomfoolery-1.0.1/src/tomfoolery/utilities.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 tomfoolery-1.0.1/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 tomfoolery-1.0.1/LICENSE.txt
+-rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 tomfoolery-1.0.1/README.md
+-rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 tomfoolery-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 tomfoolery-1.0.1/PKG-INFO
```

### Comparing `tomfoolery-1.0.0/src/tomfoolery/engine.py` & `tomfoolery-1.0.1/src/tomfoolery/engine.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,15 +19,18 @@
     def class_names(self) -> list[str]:
         """List of class names in `self.module.body`."""
         return [node.name for node in self.module.body if type(node) == ast.ClassDef]
 
     @property
     def source(self) -> str:
         """Returns the source code this object represents."""
-        return self.format_str(ast.unparse(self.module))
+        try:
+            return self.format_str(ast.unparse(self.module))
+        except Exception as e:
+            return ast.unparse(self.module)
 
     def format_str(self, code: str) -> str:
         """Sort imports and format with `black`."""
         return black.format_str(isort.api.sort_code_string(code), mode=black.Mode())  # type: ignore
 
     # Seat |===================================== Import Nodes =====================================|
 
@@ -210,7 +213,31 @@
         for node in self.import_nodes:
             if node not in self.module.body:
                 self.module.body.insert(0, node)
         dataclass = self.build_dataclass(name, data, True)
         self.add_dataclass(dataclass)
         self.fix_order()
         return self.source
+
+
+def generate_from_file(datapath: Pathish, outpath: Pathish | None = None):
+    """Generate a `dataclass` named after the file `datapath` points at.
+
+    If `outpath` is not given, the output file will be the same as `datapath`, but with a `.py` extension.
+
+    Can be any `.toml` or `.json` file where all keys are valid Python variable names."""
+
+    datapath = Pathier(datapath)
+    if outpath:
+        outpath = Pathier(outpath)
+    else:
+        outpath = datapath.with_suffix(".py")
+    module = ast.parse(outpath.read_text()) if outpath.exists() else None
+    data = datapath.loads()
+    fool = TomFoolery(module)  # type: ignore
+    source = fool.generate(datapath.stem, data)
+    source = source.replace("filepath", datapath.name)
+    try:
+        source = fool.format_str(source)
+    except Exception as e:
+        print("Unable to format output.")
+    outpath.write_text(source)
```

### Comparing `tomfoolery-1.0.0/src/tomfoolery/utilities.py` & `tomfoolery-1.0.1/src/tomfoolery/utilities.py`

 * *Files identical despite different names*

### Comparing `tomfoolery-1.0.0/LICENSE.txt` & `tomfoolery-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tomfoolery-1.0.0/README.md` & `tomfoolery-1.0.1/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -34,10 +34,8 @@
 >venue.calendar.start_month = "March"
 >venue.dump()
 </pre>
 
 ### Current Caveats
 
 * Only works with `.toml` and `.json` files.
-* All keys must be valid Python variable names.
-* If the schema of your original file changes, you can rerun the tool to update the dataclass;
-however, anything that you have added or modified will be overwritten.
+* All keys must be valid Python variable names.
```

### Comparing `tomfoolery-1.0.0/pyproject.toml` & `tomfoolery-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "tomfoolery"
 description = "CLI to generate Python dataclasses that model and load toml files (or other can-representated-as-a-dict files)"
-version = "1.0.0"
+version = "1.0.1"
 requires-python = ">=3.10"
 dependencies = ["pathier", "black", "dacite", "typing_extensions", "pytest", "isort", "ast_comments"]
 readme = "README.md"
 keywords = ["dataclass", "dataclasses", "toml", "json"]
 classifiers = ["Programming Language :: Python :: 3", "License :: OSI Approved :: MIT License", "Operating System :: OS Independent"]
 
 [[project.authors]]
```

### Comparing `tomfoolery-1.0.0/PKG-INFO` & `tomfoolery-1.0.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tomfoolery
-Version: 1.0.0
+Version: 1.0.1
 Summary: CLI to generate Python dataclasses that model and load toml files (or other can-representated-as-a-dict files)
 Project-URL: Homepage, https://github.com/matt-manes/tomfoolery
 Project-URL: Documentation, https://github.com/matt-manes/tomfoolery/tree/main/docs
 Project-URL: Source code, https://github.com/matt-manes/tomfoolery/tree/main/src/tomfoolery
 Author-email: Matt Manes <mattmanes@pm.me>
 License-File: LICENSE.txt
 Keywords: dataclass,dataclasses,json,toml
@@ -57,10 +57,8 @@
 >venue.calendar.start_month = "March"
 >venue.dump()
 </pre>
 
 ### Current Caveats
 
 * Only works with `.toml` and `.json` files.
-* All keys must be valid Python variable names.
-* If the schema of your original file changes, you can rerun the tool to update the dataclass;
-however, anything that you have added or modified will be overwritten.
+* All keys must be valid Python variable names.
```

