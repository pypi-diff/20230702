# Comparing `tmp/ask-orex-1.1.0.tar.gz` & `tmp/ask-orex-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ask-orex-1.1.0.tar", last modified: Sun Jul  2 18:51:53 2023, max compression
+gzip compressed data, was "ask-orex-1.1.1.tar", last modified: Sun Jul  2 19:03:28 2023, max compression
```

## Comparing `ask-orex-1.1.0.tar` & `ask-orex-1.1.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 arvid      (502) staff       (20)        0 2023-07-02 18:51:53.604514 ask-orex-1.1.0/
--rw-r--r--   0 arvid      (502) staff       (20)     3089 2023-06-11 19:55:46.000000 ask-orex-1.1.0/.gitignore
--rw-r--r--   0 arvid      (502) staff       (20)      892 2023-06-06 22:22:33.000000 ask-orex-1.1.0/.pre-commit-config.yaml
--rw-r--r--   0 arvid      (502) staff       (20)     1065 2023-06-06 22:12:25.000000 ask-orex-1.1.0/LICENSE
--rw-r--r--   0 arvid      (502) staff       (20)     4927 2023-07-02 18:51:53.604622 ask-orex-1.1.0/PKG-INFO
--rw-r--r--   0 arvid      (502) staff       (20)     4444 2023-07-02 18:47:32.000000 ask-orex-1.1.0/README.md
--rw-r--r--   0 arvid      (502) staff       (20)        0 2023-06-20 20:06:33.000000 ask-orex-1.1.0/__init__.py
--rw-r--r--   0 arvid      (502) staff       (20)     1064 2023-07-02 18:51:23.000000 ask-orex-1.1.0/pyproject.toml
--rw-r--r--   0 arvid      (502) staff       (20)      340 2023-07-01 19:48:43.000000 ask-orex-1.1.0/requirements.txt
--rw-r--r--   0 arvid      (502) staff       (20)      492 2023-07-02 18:51:53.604955 ask-orex-1.1.0/setup.cfg
-drwxr-xr-x   0 arvid      (502) staff       (20)        0 2023-07-02 18:51:53.601495 ask-orex-1.1.0/src/
-drwxr-xr-x   0 arvid      (502) staff       (20)        0 2023-07-02 18:51:53.603158 ask-orex-1.1.0/src/ask_orex/
--rw-r--r--   0 arvid      (502) staff       (20)       47 2023-07-02 18:47:54.000000 ask-orex-1.1.0/src/ask_orex/__init__.py
--rw-r--r--   0 arvid      (502) staff       (20)       65 2023-07-01 19:26:20.000000 ask-orex-1.1.0/src/ask_orex/__main__.py
--rw-r--r--   0 arvid      (502) staff       (20)      698 2023-07-01 19:03:51.000000 ask-orex-1.1.0/src/ask_orex/constants.py
--rw-r--r--   0 arvid      (502) staff       (20)     5587 2023-07-02 18:46:47.000000 ask-orex-1.1.0/src/ask_orex/orex.py
-drwxr-xr-x   0 arvid      (502) staff       (20)        0 2023-07-02 18:51:53.604213 ask-orex-1.1.0/src/ask_orex.egg-info/
--rw-r--r--   0 arvid      (502) staff       (20)     4927 2023-07-02 18:51:53.000000 ask-orex-1.1.0/src/ask_orex.egg-info/PKG-INFO
--rw-r--r--   0 arvid      (502) staff       (20)      405 2023-07-02 18:51:53.000000 ask-orex-1.1.0/src/ask_orex.egg-info/SOURCES.txt
--rw-r--r--   0 arvid      (502) staff       (20)        1 2023-07-02 18:51:53.000000 ask-orex-1.1.0/src/ask_orex.egg-info/dependency_links.txt
--rw-r--r--   0 arvid      (502) staff       (20)       51 2023-07-02 18:51:53.000000 ask-orex-1.1.0/src/ask_orex.egg-info/requires.txt
--rw-r--r--   0 arvid      (502) staff       (20)        9 2023-07-02 18:51:53.000000 ask-orex-1.1.0/src/ask_orex.egg-info/top_level.txt
-drwxr-xr-x   0 arvid      (502) staff       (20)        0 2023-07-02 18:51:53.604370 ask-orex-1.1.0/tests/
--rw-r--r--   0 arvid      (502) staff       (20)    14756 2023-07-02 18:46:18.000000 ask-orex-1.1.0/tests/test_concepts.py
+drwxr-xr-x   0 arvid      (502) staff       (20)        0 2023-07-02 19:03:28.191554 ask-orex-1.1.1/
+-rw-r--r--   0 arvid      (502) staff       (20)     3089 2023-06-11 19:55:46.000000 ask-orex-1.1.1/.gitignore
+-rw-r--r--   0 arvid      (502) staff       (20)      892 2023-06-06 22:22:33.000000 ask-orex-1.1.1/.pre-commit-config.yaml
+-rw-r--r--   0 arvid      (502) staff       (20)     1065 2023-06-06 22:12:25.000000 ask-orex-1.1.1/LICENSE
+-rw-r--r--   0 arvid      (502) staff       (20)     4927 2023-07-02 19:03:28.191652 ask-orex-1.1.1/PKG-INFO
+-rw-r--r--   0 arvid      (502) staff       (20)     4444 2023-07-02 18:47:32.000000 ask-orex-1.1.1/README.md
+-rw-r--r--   0 arvid      (502) staff       (20)        0 2023-06-20 20:06:33.000000 ask-orex-1.1.1/__init__.py
+-rw-r--r--   0 arvid      (502) staff       (20)     1064 2023-07-02 19:02:58.000000 ask-orex-1.1.1/pyproject.toml
+-rw-r--r--   0 arvid      (502) staff       (20)      340 2023-07-01 19:48:43.000000 ask-orex-1.1.1/requirements.txt
+-rw-r--r--   0 arvid      (502) staff       (20)      492 2023-07-02 19:03:28.191949 ask-orex-1.1.1/setup.cfg
+drwxr-xr-x   0 arvid      (502) staff       (20)        0 2023-07-02 19:03:28.189028 ask-orex-1.1.1/src/
+drwxr-xr-x   0 arvid      (502) staff       (20)        0 2023-07-02 19:03:28.190595 ask-orex-1.1.1/src/ask_orex/
+-rw-r--r--   0 arvid      (502) staff       (20)       47 2023-07-02 18:47:54.000000 ask-orex-1.1.1/src/ask_orex/__init__.py
+-rw-r--r--   0 arvid      (502) staff       (20)       65 2023-07-01 19:26:20.000000 ask-orex-1.1.1/src/ask_orex/__main__.py
+-rw-r--r--   0 arvid      (502) staff       (20)     5587 2023-07-02 19:01:35.000000 ask-orex-1.1.1/src/ask_orex/ask_orex.py
+-rw-r--r--   0 arvid      (502) staff       (20)      698 2023-07-01 19:03:51.000000 ask-orex-1.1.1/src/ask_orex/constants.py
+drwxr-xr-x   0 arvid      (502) staff       (20)        0 2023-07-02 19:03:28.191300 ask-orex-1.1.1/src/ask_orex.egg-info/
+-rw-r--r--   0 arvid      (502) staff       (20)     4927 2023-07-02 19:03:28.000000 ask-orex-1.1.1/src/ask_orex.egg-info/PKG-INFO
+-rw-r--r--   0 arvid      (502) staff       (20)      409 2023-07-02 19:03:28.000000 ask-orex-1.1.1/src/ask_orex.egg-info/SOURCES.txt
+-rw-r--r--   0 arvid      (502) staff       (20)        1 2023-07-02 19:03:28.000000 ask-orex-1.1.1/src/ask_orex.egg-info/dependency_links.txt
+-rw-r--r--   0 arvid      (502) staff       (20)       51 2023-07-02 19:03:28.000000 ask-orex-1.1.1/src/ask_orex.egg-info/requires.txt
+-rw-r--r--   0 arvid      (502) staff       (20)        9 2023-07-02 19:03:28.000000 ask-orex-1.1.1/src/ask_orex.egg-info/top_level.txt
+drwxr-xr-x   0 arvid      (502) staff       (20)        0 2023-07-02 19:03:28.191443 ask-orex-1.1.1/tests/
+-rw-r--r--   0 arvid      (502) staff       (20)    14756 2023-07-02 18:46:18.000000 ask-orex-1.1.1/tests/test_concepts.py
```

### Comparing `ask-orex-1.1.0/.gitignore` & `ask-orex-1.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `ask-orex-1.1.0/.pre-commit-config.yaml` & `ask-orex-1.1.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ask-orex-1.1.0/LICENSE` & `ask-orex-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ask-orex-1.1.0/PKG-INFO` & `ask-orex-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ask-orex
-Version: 1.1.0
+Version: 1.1.1
 Summary: ASK-Orex: Ordinary human-friendly Regular Expressions
 Author: Fernando Egoavil Cisneros
 Author-email: "Arvid J. Kingl" <akingl2016@gmail.com>
 Project-URL: Homepage, https://github.com/HCelion/orex
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ask-orex-1.1.0/README.md` & `ask-orex-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `ask-orex-1.1.0/pyproject.toml` & `ask-orex-1.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 name = "ask-orex"
 description = "ASK-Orex: Ordinary human-friendly Regular Expressions"
 readme = "README.md"
 authors = [{ name = "Arvid J. Kingl", email = "akingl2016@gmail.com" }, {name='Fernando Egoavil Cisneros'}]
 dependencies = [
     "pytest",
 ]
-version = "1.1.0"
+version = "1.1.1"
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
 
 [project.optional-dependencies]
@@ -23,15 +23,15 @@
 [project.urls]
 Homepage = "https://github.com/HCelion/orex"
 
 [tool.setuptools.packages.find]
 where = ["src"]
 
 [tool.bumpver]
-current_version = "1.1.0"
+current_version = "1.1.1"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `ask-orex-1.1.0/src/ask_orex/constants.py` & `ask-orex-1.1.1/src/ask_orex/constants.py`

 * *Files identical despite different names*

### Comparing `ask-orex-1.1.0/src/ask_orex/orex.py` & `ask-orex-1.1.1/src/ask_orex/ask_orex.py`

 * *Files identical despite different names*

### Comparing `ask-orex-1.1.0/src/ask_orex.egg-info/PKG-INFO` & `ask-orex-1.1.1/src/ask_orex.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ask-orex
-Version: 1.1.0
+Version: 1.1.1
 Summary: ASK-Orex: Ordinary human-friendly Regular Expressions
 Author: Fernando Egoavil Cisneros
 Author-email: "Arvid J. Kingl" <akingl2016@gmail.com>
 Project-URL: Homepage, https://github.com/HCelion/orex
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ask-orex-1.1.0/tests/test_concepts.py` & `ask-orex-1.1.1/tests/test_concepts.py`

 * *Files identical despite different names*

