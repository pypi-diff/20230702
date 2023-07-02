# Comparing `tmp/datascience_cookiecutter-0.3.2.tar.gz` & `tmp/datascience_cookiecutter-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datascience_cookiecutter-0.3.2.tar", last modified: Sun Jul  2 18:16:14 2023, max compression
+gzip compressed data, was "datascience_cookiecutter-0.3.3.tar", last modified: Sun Jul  2 18:39:48 2023, max compression
```

## Comparing `datascience_cookiecutter-0.3.2.tar` & `datascience_cookiecutter-0.3.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     5502 2023-07-02 18:15:31.485468 datascience_cookiecutter-0.3.2/README.md
--rw-r--r--   0        0        0      314 2023-07-02 18:15:53.712932 datascience_cookiecutter-0.3.2/datascience_cookiecutter/__init__.py
--rw-r--r--   0        0        0     2146 2023-07-02 18:04:32.451535 datascience_cookiecutter-0.3.2/datascience_cookiecutter/__main__.py
--rw-r--r--   0        0        0     3910 2023-07-02 18:08:24.296440 datascience_cookiecutter-0.3.2/datascience_cookiecutter/folderbuilder.py
--rw-r--r--   0        0        0     3703 2023-07-02 18:08:35.811440 datascience_cookiecutter-0.3.2/datascience_cookiecutter/templates.py
--rw-r--r--   0        0        0     1113 2023-07-02 18:16:14.677693 datascience_cookiecutter-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     8042 2023-06-30 22:34:34.542238 datascience_cookiecutter-0.3.2/tests/test_datascience_cookiecutter.py
--rw-r--r--   0        0        0     6387 1970-01-01 00:00:00.000000 datascience_cookiecutter-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     6837 2023-07-02 18:37:06.563119 datascience_cookiecutter-0.3.3/README.md
+-rw-r--r--   0        0        0      314 2023-07-02 18:38:44.163783 datascience_cookiecutter-0.3.3/datascience_cookiecutter/__init__.py
+-rw-r--r--   0        0        0     2146 2023-07-02 18:04:32.451535 datascience_cookiecutter-0.3.3/datascience_cookiecutter/__main__.py
+-rw-r--r--   0        0        0     3910 2023-07-02 18:08:24.296440 datascience_cookiecutter-0.3.3/datascience_cookiecutter/folderbuilder.py
+-rw-r--r--   0        0        0     3703 2023-07-02 18:08:35.811440 datascience_cookiecutter-0.3.3/datascience_cookiecutter/templates.py
+-rw-r--r--   0        0        0     1113 2023-07-02 18:39:48.823866 datascience_cookiecutter-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0     8042 2023-06-30 22:34:34.542238 datascience_cookiecutter-0.3.3/tests/test_datascience_cookiecutter.py
+-rw-r--r--   0        0        0     7722 1970-01-01 00:00:00.000000 datascience_cookiecutter-0.3.3/PKG-INFO
```

### Comparing `datascience_cookiecutter-0.3.2/README.md` & `datascience_cookiecutter-0.3.3/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -5,17 +5,19 @@
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 ## Table of Contents
 - [Motivation](#-motivation)
 - [Features](#-features)
 - [Installation](#️-installation)
 - [Basic Usage](#-basic-usage)
-- [Default Template](#default-template)
-- [Makefile](#makefile)
-- [PDM](#pdm)
+- [Default Template](#-default-template)
+- [Customizing Templates](#️-customizing-templates)
+- [Makefile](#️-makefile)
+- [PDM](#️-pdm)
+- [pytest](#-pytest)
 
 # 🍪 Data Science Cookiecutter
 The Data Science Cookiecutter 🍪 is an opinionated, yet configurable, Python project that provides a template for organizing and setting up data science projects. It uses the Cookiecutter project structure to create a standardized and reproducible project layout.
 
 
 ## 🎯 Motivation
 Data science projects often require a well-structured project layout to ensure reproducibility and collaboration. The Data Science Cookiecutter aims to solve this problem by providing a project template. While it follows certain opinions about project organization, it also allows for easy customization to fit different project needs.
@@ -63,16 +65,49 @@
 ├── references       <- Folder for reference materials
 ├── reports          <- Folder for project reports
 │   ├── img          <- Folder for images and visualizations used in reports
 │   └── report.md    <- Sample report file (Markdown format)
 └── tests            <- Folder for project tests
 ```
 
-### 🛠️ Makefile
-Makefile
+## 🛠️ Customizing Templates
+If you want to customize the default template used by `cookiecutter`, you can create a `templates.py` file in your `$HOME/.config/cookiecutter` directory. Follow these steps:
+
+1. Open a text editor and create a new file called `templates.py`.
+2. Import the necessary classes `Folder` and `FileTemplate` by adding the following lines to `templates.py`:
+
+```python
+from datascience_cookiecutter import Folder, FileTemplate
+```
+
+Define your custom template using the Folder and FileTemplate classes. Here's a minimal example:
+```python
+MYTEMPLATE = Folder(
+    name="{{name}}",
+    subfolders=[
+        Folder(name="src", files=[FileTemplate(filename="main.py", content="print('Hello, world!')")]),
+        Folder(name="data"),
+        Folder(name="docs"),
+    ],
+    files=[
+        FileTemplate(filename="README.md", content="# My {{name}}"),
+    ],
+)
+```
+
+Occurences of `{{name}}` will be replaced by the project name as provided
+with `cookiecutter myprojectname`. To use your custom template, simply run the
+cookiecutter command with the `--template` option followed by the name of
+your custom template. For example:
+```bash
+$ cookiecutter myproject --template=MYTEMPLATE
+```
+Enjoy customizing your templates! ✨🧙‍♂️
+
+## 🛠️ Makefile
 A Makefile is a file containing a set of instructions, known as targets, used to automate tasks in software development. It provides a convenient way to define and organize common commands for building, testing, and managing a project.
 
 In the provided Makefile, you have the following targets:
 
 - install: Installs project dependencies using `pdm install`.
 - test: Runs project tests with `pytest`
 - format: Applies code formatting using `isort` and `black`.
@@ -80,15 +115,15 @@
 
 To use the Makefile, open a terminal or command prompt, navigate to your project directory, and run the desired target using the make command followed by the target name. For example:
 
 ```bash
 make install
 ```
 
-### ❤️ PDM
+## ❤️ PDM
 [PDM](https://pdm.fming.dev/latest/) is a Python package manager and build tool that provides an alternative to other package managers like pip or Poetry. It aims to simplify and enhance the management of project dependencies, virtual environments, and building distributions. Follow the link to install it. If you dont want to use it, you can customize the template to create your own Makefile and pyproject.toml.
 
 The template (and PDM) follow the [PEP 621](https://peps.python.org/pep-0621/) standard for project metadata to use a pyproject.toml file instead of setup.py. This file contains the project metadata and dependencies. It also allows you to specify details like the Python version and the project entry point.
 
 ## 🔬 pytest
 Pytest is a Python testing framework that allows you to write simple and scalable tests with a clean and expressive syntax. It provides powerful features like fixtures, test discovery, and test selection.
```

### Comparing `datascience_cookiecutter-0.3.2/datascience_cookiecutter/__main__.py` & `datascience_cookiecutter-0.3.3/datascience_cookiecutter/__main__.py`

 * *Files identical despite different names*

### Comparing `datascience_cookiecutter-0.3.2/datascience_cookiecutter/folderbuilder.py` & `datascience_cookiecutter-0.3.3/datascience_cookiecutter/folderbuilder.py`

 * *Files identical despite different names*

### Comparing `datascience_cookiecutter-0.3.2/datascience_cookiecutter/templates.py` & `datascience_cookiecutter-0.3.3/datascience_cookiecutter/templates.py`

 * *Files identical despite different names*

### Comparing `datascience_cookiecutter-0.3.2/pyproject.toml` & `datascience_cookiecutter-0.3.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "datascience_cookiecutter"
-version = "0.3.2"
+version = "0.3.3"
 description = ""
 authors = [
     { name = "", email = "" },
 ]
 dependencies = [
     "pydantic>=2.0",
     "loguru>=0.7.0",
```

### Comparing `datascience_cookiecutter-0.3.2/tests/test_datascience_cookiecutter.py` & `datascience_cookiecutter-0.3.3/tests/test_datascience_cookiecutter.py`

 * *Files identical despite different names*

### Comparing `datascience_cookiecutter-0.3.2/PKG-INFO` & `datascience_cookiecutter-0.3.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datascience_cookiecutter
-Version: 0.3.2
+Version: 0.3.3
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Environment :: Console
@@ -30,17 +30,19 @@
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 ## Table of Contents
 - [Motivation](#-motivation)
 - [Features](#-features)
 - [Installation](#️-installation)
 - [Basic Usage](#-basic-usage)
-- [Default Template](#default-template)
-- [Makefile](#makefile)
-- [PDM](#pdm)
+- [Default Template](#-default-template)
+- [Customizing Templates](#️-customizing-templates)
+- [Makefile](#️-makefile)
+- [PDM](#️-pdm)
+- [pytest](#-pytest)
 
 # 🍪 Data Science Cookiecutter
 The Data Science Cookiecutter 🍪 is an opinionated, yet configurable, Python project that provides a template for organizing and setting up data science projects. It uses the Cookiecutter project structure to create a standardized and reproducible project layout.
 
 
 ## 🎯 Motivation
 Data science projects often require a well-structured project layout to ensure reproducibility and collaboration. The Data Science Cookiecutter aims to solve this problem by providing a project template. While it follows certain opinions about project organization, it also allows for easy customization to fit different project needs.
@@ -88,16 +90,49 @@
 ├── references       <- Folder for reference materials
 ├── reports          <- Folder for project reports
 │   ├── img          <- Folder for images and visualizations used in reports
 │   └── report.md    <- Sample report file (Markdown format)
 └── tests            <- Folder for project tests
 ```
 
-### 🛠️ Makefile
-Makefile
+## 🛠️ Customizing Templates
+If you want to customize the default template used by `cookiecutter`, you can create a `templates.py` file in your `$HOME/.config/cookiecutter` directory. Follow these steps:
+
+1. Open a text editor and create a new file called `templates.py`.
+2. Import the necessary classes `Folder` and `FileTemplate` by adding the following lines to `templates.py`:
+
+```python
+from datascience_cookiecutter import Folder, FileTemplate
+```
+
+Define your custom template using the Folder and FileTemplate classes. Here's a minimal example:
+```python
+MYTEMPLATE = Folder(
+    name="{{name}}",
+    subfolders=[
+        Folder(name="src", files=[FileTemplate(filename="main.py", content="print('Hello, world!')")]),
+        Folder(name="data"),
+        Folder(name="docs"),
+    ],
+    files=[
+        FileTemplate(filename="README.md", content="# My {{name}}"),
+    ],
+)
+```
+
+Occurences of `{{name}}` will be replaced by the project name as provided
+with `cookiecutter myprojectname`. To use your custom template, simply run the
+cookiecutter command with the `--template` option followed by the name of
+your custom template. For example:
+```bash
+$ cookiecutter myproject --template=MYTEMPLATE
+```
+Enjoy customizing your templates! ✨🧙‍♂️
+
+## 🛠️ Makefile
 A Makefile is a file containing a set of instructions, known as targets, used to automate tasks in software development. It provides a convenient way to define and organize common commands for building, testing, and managing a project.
 
 In the provided Makefile, you have the following targets:
 
 - install: Installs project dependencies using `pdm install`.
 - test: Runs project tests with `pytest`
 - format: Applies code formatting using `isort` and `black`.
@@ -105,15 +140,15 @@
 
 To use the Makefile, open a terminal or command prompt, navigate to your project directory, and run the desired target using the make command followed by the target name. For example:
 
 ```bash
 make install
 ```
 
-### ❤️ PDM
+## ❤️ PDM
 [PDM](https://pdm.fming.dev/latest/) is a Python package manager and build tool that provides an alternative to other package managers like pip or Poetry. It aims to simplify and enhance the management of project dependencies, virtual environments, and building distributions. Follow the link to install it. If you dont want to use it, you can customize the template to create your own Makefile and pyproject.toml.
 
 The template (and PDM) follow the [PEP 621](https://peps.python.org/pep-0621/) standard for project metadata to use a pyproject.toml file instead of setup.py. This file contains the project metadata and dependencies. It also allows you to specify details like the Python version and the project entry point.
 
 ## 🔬 pytest
 Pytest is a Python testing framework that allows you to write simple and scalable tests with a clean and expressive syntax. It provides powerful features like fixtures, test discovery, and test selection.
```

