# Comparing `tmp/datascience_cookiecutter-0.2.1.tar.gz` & `tmp/datascience_cookiecutter-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datascience_cookiecutter-0.2.1.tar", last modified: Sun Jul  2 17:01:00 2023, max compression
+gzip compressed data, was "datascience_cookiecutter-0.3.tar", last modified: Sun Jul  2 18:09:38 2023, max compression
```

## Comparing `datascience_cookiecutter-0.2.1.tar` & `datascience_cookiecutter-0.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      909 2023-07-01 21:28:19.151138 datascience_cookiecutter-0.2.1/README.md
--rw-r--r--   0        0        0      314 2023-07-02 17:00:51.205297 datascience_cookiecutter-0.2.1/datascience_cookiecutter/__init__.py
--rw-r--r--   0        0        0     2213 2023-07-02 16:54:23.964070 datascience_cookiecutter-0.2.1/datascience_cookiecutter/__main__.py
--rw-r--r--   0        0        0     3910 2023-07-02 17:00:51.250645 datascience_cookiecutter-0.2.1/datascience_cookiecutter/folderbuilder.py
--rw-r--r--   0        0        0     3714 2023-07-02 17:00:42.374646 datascience_cookiecutter-0.2.1/datascience_cookiecutter/templates.py
--rw-r--r--   0        0        0      951 2023-07-02 17:01:00.696431 datascience_cookiecutter-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     8042 2023-06-30 22:34:34.542238 datascience_cookiecutter-0.2.1/tests/test_datascience_cookiecutter.py
--rw-r--r--   0        0        0     1539 1970-01-01 00:00:00.000000 datascience_cookiecutter-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     5498 2023-07-02 18:00:10.845537 datascience_cookiecutter-0.3/README.md
+-rw-r--r--   0        0        0      312 2023-07-02 18:08:24.246473 datascience_cookiecutter-0.3/datascience_cookiecutter/__init__.py
+-rw-r--r--   0        0        0     2146 2023-07-02 18:04:32.451535 datascience_cookiecutter-0.3/datascience_cookiecutter/__main__.py
+-rw-r--r--   0        0        0     3910 2023-07-02 18:08:24.296440 datascience_cookiecutter-0.3/datascience_cookiecutter/folderbuilder.py
+-rw-r--r--   0        0        0     3703 2023-07-02 18:08:35.811440 datascience_cookiecutter-0.3/datascience_cookiecutter/templates.py
+-rw-r--r--   0        0        0     1112 2023-07-02 18:09:38.508660 datascience_cookiecutter-0.3/pyproject.toml
+-rw-r--r--   0        0        0     8042 2023-06-30 22:34:34.542238 datascience_cookiecutter-0.3/tests/test_datascience_cookiecutter.py
+-rw-r--r--   0        0        0     6309 1970-01-01 00:00:00.000000 datascience_cookiecutter-0.3/PKG-INFO
```

### Comparing `datascience_cookiecutter-0.2.1/datascience_cookiecutter/__main__.py` & `datascience_cookiecutter-0.3/datascience_cookiecutter/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,31 +21,29 @@
     # check if settings.configfolder has a templates.py file
     # and load the specified template
     # if it does not. load the default template
     if settings.configfolder.exists():
         templates_file = settings.configfolder / "templates.py"
 
         if templates_file.exists() and template != "default":
-            # Create the templates.template name from the template argument
-            template_name = f"template_{template}"
-
             # Load the module from templates.py
             spec = importlib.util.spec_from_file_location(
                 "templates", templates_file
             )  # type: ignore
             templates_module = importlib.util.module_from_spec(spec)  # type: ignore
             spec.loader.exec_module(templates_module)  # type: ignore
 
             # Check if the template exists in the loaded module
-            if hasattr(templates_module, template_name):
+            if template in dir(templates_module):
                 logger.info(f"Using template {template}")
-                selected_template = getattr(templates_module, template_name)
+                selected_template = getattr(templates_module, template)
                 settings.template = selected_template
             else:
                 logger.warning(f"Template {template} not found in {templates_file}")
+                logger.info(f"found templates: {dir(templates_module)}")
                 logger.info("Using default template")
                 # selected_template = default_template  # Use default template
         else:
             logger.info("Using default template")
             # selected_template = default_template  # Use default template
     else:
         logger.info("Using default template")
```

### Comparing `datascience_cookiecutter-0.2.1/datascience_cookiecutter/folderbuilder.py` & `datascience_cookiecutter-0.3/datascience_cookiecutter/folderbuilder.py`

 * *Files identical despite different names*

### Comparing `datascience_cookiecutter-0.2.1/datascience_cookiecutter/templates.py` & `datascience_cookiecutter-0.3/datascience_cookiecutter/templates.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from enum import Enum
 from pathlib import Path
 from typing import List
 
 from loguru import logger
-from pydantic import BaseModel, Field, validator
+from pydantic import BaseModel, Field, field_validator
 
 
 class Languages(Enum):
     PYTHON = "python"
 
 
 class ReportTypes(Enum):
@@ -160,12 +160,12 @@
     git: bool = True
     template: Folder = DEFAULTTEMPLATE
     lang: Languages = Languages.PYTHON
     report_type: ReportTypes = ReportTypes.MARKDOWN
     force: bool = False
     configfolder: Path = Path.home() / ".config" / "cookiecutter"
 
-    @validator("configfolder", pre=True, always=True)
+    @field_validator("configfolder")
     def create_configfolder(cls, configfolder):
         configfolder.mkdir(parents=True, exist_ok=True)
         logger.info(f"Created config folder {configfolder}")
         return configfolder
```

### Comparing `datascience_cookiecutter-0.2.1/pyproject.toml` & `datascience_cookiecutter-0.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 [project]
 name = "datascience_cookiecutter"
-version = "0.2.1"
+version = "0.3"
 description = ""
 authors = [
     { name = "", email = "" },
 ]
 dependencies = [
     "pydantic>=2.0",
     "loguru>=0.7.0",
     "click>=8.1.3",
 ]
 requires-python = ">=3.7"
 readme = "README.md"
 classifiers = [
-    "Development Status :: 3 - Alpha",
+    "Development Status :: 4 - Beta",
+    "Intended Audience :: Developers",
+    "Operating System :: OS Independent",
+    "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Environment :: Console",
+    "Topic :: Software Development",
     "Typing :: Typed",
 ]
 
 [project.license]
 text = "MIT"
 
 [project.optional-dependencies]
```

### Comparing `datascience_cookiecutter-0.2.1/tests/test_datascience_cookiecutter.py` & `datascience_cookiecutter-0.3/tests/test_datascience_cookiecutter.py`

 * *Files identical despite different names*

