# Comparing `tmp/notebook_setup-1.0.tar.gz` & `tmp/notebook_setup-1.1.tar.gz`

## Comparing `notebook_setup-1.0.tar` & `notebook_setup-1.1.tar`

### file list

```diff
@@ -1,10 +1,9 @@
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 notebook_setup-1.0/.python-version
--rw-r--r--   0        0        0     2216 2020-02-02 00:00:00.000000 notebook_setup-1.0/Example.ipynb
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 notebook_setup-1.0/temp.py
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 notebook_setup-1.0/.vscode/settings.json
--rw-r--r--   0        0        0     3091 2020-02-02 00:00:00.000000 notebook_setup-1.0/notebook_setup/__init__.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 notebook_setup-1.0/.gitignore
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 notebook_setup-1.0/LICENSE
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 notebook_setup-1.0/README.md
--rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 notebook_setup-1.0/pyproject.toml
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 notebook_setup-1.0/PKG-INFO
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 notebook_setup-1.1/.python-version
+-rw-r--r--   0        0        0     2216 2020-02-02 00:00:00.000000 notebook_setup-1.1/Example.ipynb
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 notebook_setup-1.1/temp.py
+-rw-r--r--   0        0        0     3100 2020-02-02 00:00:00.000000 notebook_setup-1.1/notebook_setup/__init__.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 notebook_setup-1.1/.gitignore
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 notebook_setup-1.1/LICENSE
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 notebook_setup-1.1/README.md
+-rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 notebook_setup-1.1/pyproject.toml
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 notebook_setup-1.1/PKG-INFO
```

### Comparing `notebook_setup-1.0/Example.ipynb` & `notebook_setup-1.1/Example.ipynb`

 * *Files identical despite different names*

### Comparing `notebook_setup-1.0/notebook_setup/__init__.py` & `notebook_setup-1.1/notebook_setup/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,25 +19,27 @@
             .jp-OutputArea-output {background-color: transparent;}
             </style>
             """,
         )
 
 
 def notebook_config_plotly_rendering(
-    force_small_file: bool = True, global_renderer: str = None, verbose=True
+    force_small_file: bool = True,
+    global_renderer: str = None,
+    verbose=True,
 ):
     """
     Configures the behavior of Plotly figures in Jupyter notebooks. -> Make small files and render on GitHub.
     Only figures with fig.show() are effected by this configuration.
-    This function monkey patches (modefies at runtime) behavior of fig.show(). Tested with VS Code.
+    This function monkey patches (modifies at runtime) behavior of fig.show(). Tested with VS Code.
 
     Args:
         force_small_file: If True, Plotly figures are not saved inside the notebook.
         global_renderer (str, optional): Specifies a custom global renderer for the figures.
-            - None: Default renderer (depeding on environment)
+            - None: Default renderer (depending on environment)
             - "svg": static vector plot (small file)
             - "png": static raster plot (small file)
             - "notebook"
             - "vscode"
             - "browser": opens all plots in a browser window
             for more options see: https://plotly.com/python/renderers/
 
@@ -68,16 +70,15 @@
                 )
 
         if verbose and global_renderer:
             msg = f"""global_renderer="{global_renderer}" has no effect, set force_small_file=False"""
             display(HTML(f"""<span style="color:red">Warning: </span>{msg}"""))
 
     else:
+        if global_renderer:
+            pio.renderers.default = global_renderer
 
         def show(self, *args, **kwargs):
             "Plotly default implementation"
             return pio.show(self, *args, **kwargs)
 
-        if global_renderer:
-            pio.renderers.default = global_renderer
-
     BaseFigure.show = show
```

### Comparing `notebook_setup-1.0/.gitignore` & `notebook_setup-1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `notebook_setup-1.0/LICENSE` & `notebook_setup-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `notebook_setup-1.0/pyproject.toml` & `notebook_setup-1.1/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -5,16 +5,24 @@
 [project]
 description = 'Tools to setup and configure jupyter notebooks (ipynb files) with line and cell magic'
 keywords = ["ipynb", "notebook", "jupyter", "line magic", "cell magic", "autoreload", "plotly render"]
 license = "MIT"
 name = "notebook_setup"
 readme = "README.md"
 requires-python = ">=3.7"
-version = "1.0"
+version = "1.1"
 
 dependencies = ["ipython", "ipykernel"]
 
 [project.urls]
 homepage = "https://github.com/1081/notebook_setup"
 
 [tool.hatch.build.targets.wheel]
 packages = ["notebook_setup"]
+
+[tool.ruff]
+ignore = ["E501", "C408", "PD901"]
+select = ["E", "W", "N", "I", "UP", "F", "B", "C4", "SIM", "TCH", "PD", "NPY", "DTZ"]
+show-fixes = true
+
+[tool.black]
+line-length = 120
```

### Comparing `notebook_setup-1.0/PKG-INFO` & `notebook_setup-1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: notebook_setup
-Version: 1.0
+Version: 1.1
 Summary: Tools to setup and configure jupyter notebooks (ipynb files) with line and cell magic
 Project-URL: homepage, https://github.com/1081/notebook_setup
 License-Expression: MIT
 License-File: LICENSE
 Keywords: autoreload,cell magic,ipynb,jupyter,line magic,notebook,plotly render
 Requires-Python: >=3.7
 Requires-Dist: ipykernel
```

