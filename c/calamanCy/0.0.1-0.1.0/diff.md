# Comparing `tmp/calamanCy-0.0.1.tar.gz` & `tmp/calamanCy-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "calamanCy-0.0.1.tar", last modified: Tue Feb 14 12:57:09 2023, max compression
+gzip compressed data, was "calamanCy-0.1.0.tar", last modified: Sun Jul  2 02:26:07 2023, max compression
```

## Comparing `calamanCy-0.0.1.tar` & `calamanCy-0.1.0.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 lj        (1000) lj        (1000)        0 2023-02-14 12:57:09.127225 calamanCy-0.0.1/
--rw-r--r--   0 lj        (1000) lj        (1000)     1094 2023-02-14 12:07:40.000000 calamanCy-0.0.1/LICENSE
--rw-r--r--   0 lj        (1000) lj        (1000)     5642 2023-02-14 12:57:09.127225 calamanCy-0.0.1/PKG-INFO
--rw-r--r--   0 lj        (1000) lj        (1000)     4618 2023-02-14 12:52:36.000000 calamanCy-0.0.1/README.md
-drwxr-xr-x   0 lj        (1000) lj        (1000)        0 2023-02-14 12:57:09.127225 calamanCy-0.0.1/calamanCy.egg-info/
--rw-r--r--   0 lj        (1000) lj        (1000)     5642 2023-02-14 12:57:09.000000 calamanCy-0.0.1/calamanCy.egg-info/PKG-INFO
--rw-r--r--   0 lj        (1000) lj        (1000)      218 2023-02-14 12:57:09.000000 calamanCy-0.0.1/calamanCy.egg-info/SOURCES.txt
--rw-r--r--   0 lj        (1000) lj        (1000)        1 2023-02-14 12:57:09.000000 calamanCy-0.0.1/calamanCy.egg-info/dependency_links.txt
--rw-r--r--   0 lj        (1000) lj        (1000)       40 2023-02-14 12:57:09.000000 calamanCy-0.0.1/calamanCy.egg-info/requires.txt
--rw-r--r--   0 lj        (1000) lj        (1000)       10 2023-02-14 12:57:09.000000 calamanCy-0.0.1/calamanCy.egg-info/top_level.txt
-drwxr-xr-x   0 lj        (1000) lj        (1000)        0 2023-02-14 12:57:09.127225 calamanCy-0.0.1/calamancy/
--rw-r--r--   0 lj        (1000) lj        (1000)       22 2023-02-14 12:56:20.000000 calamanCy-0.0.1/calamancy/__init__.py
--rw-r--r--   0 lj        (1000) lj        (1000)     1537 2023-02-14 12:56:20.000000 calamanCy-0.0.1/pyproject.toml
--rw-r--r--   0 lj        (1000) lj        (1000)       38 2023-02-14 12:57:09.127225 calamanCy-0.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 02:26:07.359783 calamanCy-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-07-02 02:25:57.000000 calamanCy-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-07-02 02:26:07.359783 calamanCy-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-07-02 02:25:57.000000 calamanCy-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 02:26:07.359783 calamanCy-0.1.0/calamanCy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-07-02 02:26:07.000000 calamanCy-0.1.0/calamanCy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-02 02:26:07.000000 calamanCy-0.1.0/calamanCy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 02:26:07.000000 calamanCy-0.1.0/calamanCy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-02 02:26:07.000000 calamanCy-0.1.0/calamanCy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-02 02:26:07.000000 calamanCy-0.1.0/calamanCy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 02:26:07.359783 calamanCy-0.1.0/calamancy/
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-02 02:25:57.000000 calamanCy-0.1.0/calamancy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-07-02 02:25:57.000000 calamanCy-0.1.0/calamancy/loaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-07-02 02:25:57.000000 calamanCy-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 02:26:07.359783 calamanCy-0.1.0/setup.cfg
```

### Comparing `calamanCy-0.0.1/LICENSE` & `calamanCy-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `calamanCy-0.0.1/pyproject.toml` & `calamanCy-0.1.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "calamanCy"
-version = "0.0.1"
+version = "0.1.0"
 authors = [
     {name = "Lj V. Miranda", email = "ljvmiranda@gmail.com"}
 ]
 description = "NLP Pipelines for Tagalog"
 readme = {file = "README.md", content-type = "text/markdown"}
 license = {text = "MIT License"}
 keywords = ["nlp", "natural language processing", "language technology", "tagalog"]
@@ -22,35 +22,49 @@
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Topic :: Scientific/Engineering"
 ]
 requires-python = ">=3.7"
 dependencies = [
-    "spacy>=3.4.0",
+    "spacy>=3.5.0",
     "wasabi>=0.9.1",
     "typer>=0.4.2"
 ]
 
+[project.optional-dependencies]
+dev = [
+    "black>=23.1.0",
+    "isort>=5.0.0",
+    "ruff>=0.0.272",
+    "mypy>=1.0.0",
+    "pytest"
+]
+
 [project.urls]
 "Repository" = "https://github.com/ljvmiranda921/calamanCy"
 "Bug Tracker" = "https://github.com/ljvmiranda921/calamanCy/issues"
 "Release Notes" = "https://github.com/ljvmiranda921/calamanCy/releases"
 
 [tool.setuptools]
 packages = ["calamancy"]
 
 [tool.isort]
 profile = "black"
 
 [tool.pylint.format]
 max-line-length = 88
 
-[tool.flake8]
-ignore = ["E203", "E266", "E501", "E731", "W503", "E741", "F541"]
-max-line-length = 88
-select = ["B", "C", "E", "F", "W", "T4", "B9"]
-exclude = [
-    ".env*",
-    ".git",
-    "__pycache__"
+[tool.ruff]
+ignore = ["E203", "E266", "E501", "E731", "E741", "F541"]
+select = [
+    "E",    # pycodestyle errors
+    "W",    # pycodestyle warnings
+    "F",    # Pyflakes
+    "Q",    # flake8-quotes
+    "T201"  # flake8-print
 ]
+
+[tool.mypy]
+ignore_missing_imports = true
+no_implicit_optional = true
+allow_redefinition = true
```

