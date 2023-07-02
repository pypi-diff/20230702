# Comparing `tmp/datascience_cookiecutter-0.1.3.tar.gz` & `tmp/datascience_cookiecutter-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datascience_cookiecutter-0.1.3.tar", last modified: Sat Jul  1 21:46:21 2023, max compression
+gzip compressed data, was "datascience_cookiecutter-0.2.0.tar", last modified: Sun Jul  2 08:46:37 2023, max compression
```

## Comparing `datascience_cookiecutter-0.1.3.tar` & `datascience_cookiecutter-0.2.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      909 2023-07-01 21:28:19.151138 datascience_cookiecutter-0.1.3/README.md
--rw-r--r--   0        0        0      582 2023-07-01 21:45:57.445080 datascience_cookiecutter-0.1.3/datascience_cookiecutter/__init__.py
--rw-r--r--   0        0        0       49 2023-07-01 21:45:00.054585 datascience_cookiecutter-0.1.3/datascience_cookiecutter/__main__.py
--rw-r--r--   0        0        0     3910 2023-07-01 21:45:52.573254 datascience_cookiecutter-0.1.3/datascience_cookiecutter/folderbuilder.py
--rw-r--r--   0        0        0     3363 2023-07-01 20:48:08.567048 datascience_cookiecutter-0.1.3/datascience_cookiecutter/templates.py
--rw-r--r--   0        0        0      834 2023-07-01 21:46:21.745340 datascience_cookiecutter-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     8042 2023-06-30 22:34:34.542238 datascience_cookiecutter-0.1.3/tests/test_datascience_cookiecutter.py
--rw-r--r--   0        0        0     1539 1970-01-01 00:00:00.000000 datascience_cookiecutter-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      909 2023-07-01 21:28:19.151138 datascience_cookiecutter-0.2.0/README.md
+-rw-r--r--   0        0        0      191 2023-07-02 08:46:17.968395 datascience_cookiecutter-0.2.0/datascience_cookiecutter/__init__.py
+-rw-r--r--   0        0        0      522 2023-07-02 08:41:17.870000 datascience_cookiecutter-0.2.0/datascience_cookiecutter/__main__.py
+-rw-r--r--   0        0        0     3910 2023-07-01 21:45:52.573254 datascience_cookiecutter-0.2.0/datascience_cookiecutter/folderbuilder.py
+-rw-r--r--   0        0        0     3363 2023-07-01 20:48:08.567048 datascience_cookiecutter-0.2.0/datascience_cookiecutter/templates.py
+-rw-r--r--   0        0        0      823 2023-07-02 08:46:37.237182 datascience_cookiecutter-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     8042 2023-06-30 22:34:34.542238 datascience_cookiecutter-0.2.0/tests/test_datascience_cookiecutter.py
+-rw-r--r--   0        0        0     1539 1970-01-01 00:00:00.000000 datascience_cookiecutter-0.2.0/PKG-INFO
```

### Comparing `datascience_cookiecutter-0.1.3/README.md` & `datascience_cookiecutter-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `datascience_cookiecutter-0.1.3/datascience_cookiecutter/__init__.py` & `datascience_cookiecutter-0.2.0/datascience_cookiecutter/__main__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,28 +1,19 @@
-from pathlib import Path
-
 import click
-
-from datascience_cookiecutter.folderbuilder import Cookiecutter, CookiecutterSettings
-
-__all__ = ["Cookiecutter", "CookiecutterSettings"]
-
-__version__ = "0.1.3"
-
+from pathlib import Path
+from datascience_cookiecutter import Cookiecutter, CookiecutterSettings
 
 @click.command()
 @click.argument("projectname")
-def main(projectname: str) -> None:
+def create_project(projectname: str) -> None:
     # Set the default settings
+    if projectname is None:
+        projectname = "my_project"
     settings = CookiecutterSettings(
         name=projectname,
         path=Path("."),
         git=True,
     )
 
     # Create the cookiecutter instance and execute
     cookiecutter = Cookiecutter(settings)
-    cookiecutter()
-
-
-if __name__ == "__main__":
-    main()
+    cookiecutter()
```

### Comparing `datascience_cookiecutter-0.1.3/datascience_cookiecutter/folderbuilder.py` & `datascience_cookiecutter-0.2.0/datascience_cookiecutter/folderbuilder.py`

 * *Files identical despite different names*

### Comparing `datascience_cookiecutter-0.1.3/datascience_cookiecutter/templates.py` & `datascience_cookiecutter-0.2.0/datascience_cookiecutter/templates.py`

 * *Files identical despite different names*

### Comparing `datascience_cookiecutter-0.1.3/pyproject.toml` & `datascience_cookiecutter-0.2.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
-name = "datascience-cookiecutter"
-version = "0.1.3"
+name = "datascience_cookiecutter"
+version = "0.2.0"
 description = ""
 authors = [
     { name = "", email = "" },
 ]
 dependencies = [
     "pydantic>=2.0",
     "loguru>=0.7.0",
@@ -27,21 +27,18 @@
     "pytest>=7.4.0",
     "ruff>=0.0.275",
     "black>=23.3.0",
     "isort>=5.11.5",
     "mypy>=1.4.1",
 ]
 
+[project.scripts]
+cookiecutter = "datascience_cookiecutter.__main__:create_project"
+
 [tool.pdm.urls]
 GitHub = "https://github.com/raoulg/datascience-cookiecutter"
 
-[tool.pdm.scripts.cookiecutter]
-call = "datascience_cookiecutter:main"
-deps = [
-    "click",
-]
-
 [build-system]
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
```

### Comparing `datascience_cookiecutter-0.1.3/tests/test_datascience_cookiecutter.py` & `datascience_cookiecutter-0.2.0/tests/test_datascience_cookiecutter.py`

 * *Files identical despite different names*

### Comparing `datascience_cookiecutter-0.1.3/PKG-INFO` & `datascience_cookiecutter-0.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: datascience-cookiecutter
-Version: 0.1.3
+Name: datascience_cookiecutter
+Version: 0.2.0
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python
 Classifier: Environment :: Console
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Requires-Dist: pydantic>=2.0
```

