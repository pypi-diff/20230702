# Comparing `tmp/datascience_cookiecutter-0.3.1.tar.gz` & `tmp/datascience_cookiecutter-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datascience_cookiecutter-0.3.1.tar", last modified: Sun Jul  2 18:14:40 2023, max compression
+gzip compressed data, was "datascience_cookiecutter-0.3.2.tar", last modified: Sun Jul  2 18:16:14 2023, max compression
```

## Comparing `datascience_cookiecutter-0.3.1.tar` & `datascience_cookiecutter-0.3.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     5498 2023-07-02 18:00:10.845537 datascience_cookiecutter-0.3.1/README.md
--rw-r--r--   0        0        0      314 2023-07-02 18:14:09.082334 datascience_cookiecutter-0.3.1/datascience_cookiecutter/__init__.py
--rw-r--r--   0        0        0     2146 2023-07-02 18:04:32.451535 datascience_cookiecutter-0.3.1/datascience_cookiecutter/__main__.py
--rw-r--r--   0        0        0     3910 2023-07-02 18:08:24.296440 datascience_cookiecutter-0.3.1/datascience_cookiecutter/folderbuilder.py
--rw-r--r--   0        0        0     3703 2023-07-02 18:08:35.811440 datascience_cookiecutter-0.3.1/datascience_cookiecutter/templates.py
--rw-r--r--   0        0        0     1113 2023-07-02 18:14:40.783428 datascience_cookiecutter-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     8042 2023-06-30 22:34:34.542238 datascience_cookiecutter-0.3.1/tests/test_datascience_cookiecutter.py
--rw-r--r--   0        0        0     6383 1970-01-01 00:00:00.000000 datascience_cookiecutter-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     5502 2023-07-02 18:15:31.485468 datascience_cookiecutter-0.3.2/README.md
+-rw-r--r--   0        0        0      314 2023-07-02 18:15:53.712932 datascience_cookiecutter-0.3.2/datascience_cookiecutter/__init__.py
+-rw-r--r--   0        0        0     2146 2023-07-02 18:04:32.451535 datascience_cookiecutter-0.3.2/datascience_cookiecutter/__main__.py
+-rw-r--r--   0        0        0     3910 2023-07-02 18:08:24.296440 datascience_cookiecutter-0.3.2/datascience_cookiecutter/folderbuilder.py
+-rw-r--r--   0        0        0     3703 2023-07-02 18:08:35.811440 datascience_cookiecutter-0.3.2/datascience_cookiecutter/templates.py
+-rw-r--r--   0        0        0     1113 2023-07-02 18:16:14.677693 datascience_cookiecutter-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     8042 2023-06-30 22:34:34.542238 datascience_cookiecutter-0.3.2/tests/test_datascience_cookiecutter.py
+-rw-r--r--   0        0        0     6387 1970-01-01 00:00:00.000000 datascience_cookiecutter-0.3.2/PKG-INFO
```

### Comparing `datascience_cookiecutter-0.3.1/README.md` & `datascience_cookiecutter-0.3.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 
 1. Open a terminal or command prompt.
 2. `cd` to the directory where you want to create the project.
 3. Run the following command: `cookiecutter myproject` where `myproject` is the name of your project.
 4. profit 🎉
 
 ## 📁 Default Template
-```bash
+```markdown
 .
 ├── Makefile         <- Makefile for project automation
 ├── README.md        <- Project documentation and instructions
 ├── pyproject.toml   <- Configuration file for dependencies and project metadata
 ├── data             <- Folder to store data
 │   ├── final        <- Folder for final processed data
 │   ├── processed    <- Folder for intermediate processed data
```

### Comparing `datascience_cookiecutter-0.3.1/datascience_cookiecutter/__main__.py` & `datascience_cookiecutter-0.3.2/datascience_cookiecutter/__main__.py`

 * *Files identical despite different names*

### Comparing `datascience_cookiecutter-0.3.1/datascience_cookiecutter/folderbuilder.py` & `datascience_cookiecutter-0.3.2/datascience_cookiecutter/folderbuilder.py`

 * *Files identical despite different names*

### Comparing `datascience_cookiecutter-0.3.1/datascience_cookiecutter/templates.py` & `datascience_cookiecutter-0.3.2/datascience_cookiecutter/templates.py`

 * *Files identical despite different names*

### Comparing `datascience_cookiecutter-0.3.1/pyproject.toml` & `datascience_cookiecutter-0.3.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "datascience_cookiecutter"
-version = "0.3.1"
+version = "0.3.2"
 description = ""
 authors = [
     { name = "", email = "" },
 ]
 dependencies = [
     "pydantic>=2.0",
     "loguru>=0.7.0",
```

### Comparing `datascience_cookiecutter-0.3.1/tests/test_datascience_cookiecutter.py` & `datascience_cookiecutter-0.3.2/tests/test_datascience_cookiecutter.py`

 * *Files identical despite different names*

### Comparing `datascience_cookiecutter-0.3.1/PKG-INFO` & `datascience_cookiecutter-0.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datascience_cookiecutter
-Version: 0.3.1
+Version: 0.3.2
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Environment :: Console
@@ -64,15 +64,15 @@
 
 1. Open a terminal or command prompt.
 2. `cd` to the directory where you want to create the project.
 3. Run the following command: `cookiecutter myproject` where `myproject` is the name of your project.
 4. profit 🎉
 
 ## 📁 Default Template
-```bash
+```markdown
 .
 ├── Makefile         <- Makefile for project automation
 ├── README.md        <- Project documentation and instructions
 ├── pyproject.toml   <- Configuration file for dependencies and project metadata
 ├── data             <- Folder to store data
 │   ├── final        <- Folder for final processed data
 │   ├── processed    <- Folder for intermediate processed data
```

