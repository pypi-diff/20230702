# Comparing `tmp/firenze-0.1.2.tar.gz` & `tmp/firenze-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "firenze-0.1.2.tar", max compression
+gzip compressed data, was "firenze-0.1.3.tar", max compression
```

## Comparing `firenze-0.1.2.tar` & `firenze-0.1.3.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0     1089 2023-06-21 14:33:40.045938 firenze-0.1.2/LICENSE.md
--rw-r--r--   0        0        0     1362 2023-06-21 14:33:40.045938 firenze-0.1.2/README.md
--rw-r--r--   0        0        0        0 2023-06-21 14:33:40.045938 firenze-0.1.2/firenze/__init__.py
--rw-r--r--   0        0        0     1343 2023-06-21 14:57:04.808324 firenze-0.1.2/firenze/cli.py
--rw-r--r--   0        0        0       51 2023-06-21 14:33:40.045938 firenze-0.1.2/firenze/exceptions.py
--rw-r--r--   0        0        0     4151 2023-06-21 15:41:47.999876 firenze-0.1.2/firenze/notebook.py
--rw-r--r--   0        0        0      923 2023-06-22 18:08:10.471934 firenze-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2312 1970-01-01 00:00:00.000000 firenze-0.1.2/setup.py
--rw-r--r--   0        0        0     2239 1970-01-01 00:00:00.000000 firenze-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1089 2023-07-02 15:27:46.609703 firenze-0.1.3/LICENSE.md
+-rw-r--r--   0        0        0     2162 2023-07-02 15:27:46.609703 firenze-0.1.3/README.md
+-rw-r--r--   0        0        0        0 2023-07-02 15:27:46.613704 firenze-0.1.3/firenze/__init__.py
+-rw-r--r--   0        0        0     1880 2023-07-02 15:27:46.613704 firenze-0.1.3/firenze/cli.py
+-rw-r--r--   0        0        0       51 2023-07-02 15:27:46.613704 firenze-0.1.3/firenze/exceptions.py
+-rw-r--r--   0        0        0     4604 2023-07-02 15:27:46.613704 firenze-0.1.3/firenze/notebook.py
+-rw-r--r--   0        0        0     1221 2023-07-02 15:27:46.613704 firenze-0.1.3/firenze/progress.py
+-rw-r--r--   0        0        0      923 2023-07-02 15:27:46.613704 firenze-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     3122 1970-01-01 00:00:00.000000 firenze-0.1.3/setup.py
+-rw-r--r--   0        0        0     3039 1970-01-01 00:00:00.000000 firenze-0.1.3/PKG-INFO
```

### Comparing `firenze-0.1.2/LICENSE.md` & `firenze-0.1.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `firenze-0.1.2/README.md` & `firenze-0.1.3/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,11 +1,21 @@
 # Firenze
 
 Firenze is a lean jupyter notebook executor, that generates the notebook output in a single HTML
-file. You can also parameterize the notebooks without any modification to the notebook itself.
+file.
+
+[![CI](https://github.com/pabloalcain/firenze/actions/workflows/ci.yaml/badge.svg)](https://github.com/pabloalcain/firenze/actions/workflows/ci.yaml)
+[![Coverage](https://codecov.io/gh/pabloalcain/firenze/branch/main/graph/badge.svg?token=VJGXI1MVOF)](https://codecov.io/gh/pabloalcain/firenze)
+[![License](https://img.shields.io/badge/license-MIT-blue)](https://github.com/pabloalcain/firenze/blob/main/LICENSE.md)
+[![Python](https://img.shields.io/pypi/pyversions/firenze)](https://pypi.org/project/firenze/)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-black.svg)](https://github.com/ambv/black)
+[![PyPI](https://img.shields.io/pypi/v/firenze)](https://pypi.org/project/firenze/)
+[![Downloads](https://img.shields.io/pypi/dm/firenze)](https://pypi.org/project/firenze/)
+
+You can also parameterize the notebooks without any modification to the notebook itself.
 It supports local files and `s3` paths, both for the notebook and for the output.
 
 ## As a Library
 You can use `firenze` as a library in your own project. Install it through `pip`
 
 ```bash
 pip install firenze
```

### Comparing `firenze-0.1.2/firenze/notebook.py` & `firenze-0.1.3/firenze/notebook.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,59 +1,71 @@
 import ast
+import asyncio
+import logging
 import pathlib
 from typing import Any, Optional
 
 import boto3
 import nbformat
 from nbclient import NotebookClient
 from nbconvert import HTMLExporter
 
+from firenze import progress
 from firenze.exceptions import VariableAssignmentError
 
 
 class Notebook:
     def __init__(
         self,
         notebook: nbformat.notebooknode.NotebookNode,
         client: Optional[NotebookClient] = None,
     ):
         if client is None:
-            client = NotebookClient(notebook, timeout=600)
+            client = NotebookClient(notebook, timeout=None)
         self.client = client
         self.jupyter_notebook = notebook
 
-    def execute(self, **kwargs):
+    def execute(self):
+        asyncio.run(self.async_execute())
+
+    async def async_execute(self):
+        async with self.client.async_setup_kernel():
+            for index, cell in enumerate(progress.with_logging(self.cells)):
+                execution = self.client.async_execute_cell(cell, index)
+                if logging.getLogger().isEnabledFor(logging.INFO):
+                    await progress.add_elapsed(execution)
+                else:
+                    await execution
+
+    def set_parameters(self, **kwargs):
         for key, value in kwargs.items():
             self.set_first_assignment_of_variable(key, value)
-        with self.client.setup_kernel():
-            for index, cell in enumerate(self.jupyter_notebook.cells):
-                self.client.execute_cell(cell, index)
 
     @property
     def cells(self):
         return self.jupyter_notebook.cells
 
     @property
     def code_cells(self):
         return [c for c in self.cells if c["cell_type"] == "code"]
 
     @property
     def html(self) -> str:
         return HTMLExporter().from_notebook_node(self.jupyter_notebook)[0]
 
     def is_clean(self) -> bool:
-        return all([c["outputs"] == [] for c in self.cells])
+        return all([c["outputs"] == [] for c in self.cells]) and all(
+            c["execution_count"] is None for c in self.code_cells
+        )
 
     def clean(self):
         for cell in self.jupyter_notebook.cells:
             cell["outputs"] = []
-            try:
-                del cell["execution_count"]
-            except KeyError:
-                pass
+            if cell["cell_type"] == "code":
+                cell["execution_count"] = None
 
     @classmethod
     def from_path(cls, notebook_path, client: Optional[NotebookClient] = None):
         if str(notebook_path).startswith("s3://"):
             return cls.from_s3(notebook_path)
         return cls.from_local(client, notebook_path)
```

### Comparing `firenze-0.1.2/pyproject.toml` & `firenze-0.1.3/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "firenze"
-version = "0.1.2"
+version = "0.1.3"
 description = "A lean executor for jupyter notebooks."
 authors = ["Pablo Alcain <pabloalcain@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/pabloalcain/firenze"
 keywords = ["jupyter", "notebook"]
```

### Comparing `firenze-0.1.2/PKG-INFO` & `firenze-0.1.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: firenze
-Version: 0.1.2
+Version: 0.1.3
 Summary: A lean executor for jupyter notebooks.
 Home-page: https://github.com/pabloalcain/firenze
 License: MIT
 Keywords: jupyter,notebook
 Author: Pablo Alcain
 Author-email: pabloalcain@gmail.com
 Requires-Python: >=3.9,<4.0
@@ -21,15 +21,25 @@
 Requires-Dist: nbformat (>=5.8.0,<6.0.0)
 Project-URL: Repository, https://github.com/pabloalcain/firenze
 Description-Content-Type: text/markdown
 
 # Firenze
 
 Firenze is a lean jupyter notebook executor, that generates the notebook output in a single HTML
-file. You can also parameterize the notebooks without any modification to the notebook itself.
+file.
+
+[![CI](https://github.com/pabloalcain/firenze/actions/workflows/ci.yaml/badge.svg)](https://github.com/pabloalcain/firenze/actions/workflows/ci.yaml)
+[![Coverage](https://codecov.io/gh/pabloalcain/firenze/branch/main/graph/badge.svg?token=VJGXI1MVOF)](https://codecov.io/gh/pabloalcain/firenze)
+[![License](https://img.shields.io/badge/license-MIT-blue)](https://github.com/pabloalcain/firenze/blob/main/LICENSE.md)
+[![Python](https://img.shields.io/pypi/pyversions/firenze)](https://pypi.org/project/firenze/)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-black.svg)](https://github.com/ambv/black)
+[![PyPI](https://img.shields.io/pypi/v/firenze)](https://pypi.org/project/firenze/)
+[![Downloads](https://img.shields.io/pypi/dm/firenze)](https://pypi.org/project/firenze/)
+
+You can also parameterize the notebooks without any modification to the notebook itself.
 It supports local files and `s3` paths, both for the notebook and for the output.
 
 ## As a Library
 You can use `firenze` as a library in your own project. Install it through `pip`
 
 ```bash
 pip install firenze
```

