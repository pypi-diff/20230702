# Comparing `tmp/py-robocopy-0.0.4.tar.gz` & `tmp/py-robocopy-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-robocopy-0.0.4.tar", last modified: Sun Jul  2 18:02:09 2023, max compression
+gzip compressed data, was "py-robocopy-0.0.5.tar", last modified: Sun Jul  2 19:08:45 2023, max compression
```

## Comparing `py-robocopy-0.0.4.tar` & `py-robocopy-0.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 18:02:09.958781 py-robocopy-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-02 18:01:54.000000 py-robocopy-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-07-02 18:02:09.958781 py-robocopy-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-07-02 18:01:54.000000 py-robocopy-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-07-02 18:01:54.000000 py-robocopy-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 18:02:09.958781 py-robocopy-0.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 18:02:09.958781 py-robocopy-0.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 18:02:09.958781 py-robocopy-0.0.4/src/py_robocopy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-07-02 18:02:09.000000 py-robocopy-0.0.4/src/py_robocopy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-02 18:02:09.000000 py-robocopy-0.0.4/src/py_robocopy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 18:02:09.000000 py-robocopy-0.0.4/src/py_robocopy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-02 18:02:09.000000 py-robocopy-0.0.4/src/py_robocopy.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 18:02:09.958781 py-robocopy-0.0.4/src/robocopy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 18:01:54.000000 py-robocopy-0.0.4/src/robocopy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-02 18:01:54.000000 py-robocopy-0.0.4/src/robocopy/robocopy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 19:08:45.102780 py-robocopy-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-02 19:08:22.000000 py-robocopy-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16409 2023-07-02 19:08:45.102780 py-robocopy-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15859 2023-07-02 19:08:22.000000 py-robocopy-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-02 19:08:22.000000 py-robocopy-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 19:08:45.102780 py-robocopy-0.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 19:08:45.098780 py-robocopy-0.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 19:08:45.098780 py-robocopy-0.0.5/src/py_robocopy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16409 2023-07-02 19:08:45.000000 py-robocopy-0.0.5/src/py_robocopy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-02 19:08:45.000000 py-robocopy-0.0.5/src/py_robocopy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 19:08:45.000000 py-robocopy-0.0.5/src/py_robocopy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-02 19:08:45.000000 py-robocopy-0.0.5/src/py_robocopy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 19:08:45.102780 py-robocopy-0.0.5/src/robocopy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 19:08:22.000000 py-robocopy-0.0.5/src/robocopy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-02 19:08:22.000000 py-robocopy-0.0.5/src/robocopy/robocopy.py
```

### Comparing `py-robocopy-0.0.4/LICENSE` & `py-robocopy-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `py-robocopy-0.0.4/pyproject.toml` & `py-robocopy-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [project]
 name = "py-robocopy"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Suyash Sonkesaria", email="suyashsonkesaria@gmail.com" },
 ]
 description = "Copies file data from one location to another."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/suyashsonkesaria/robocopy"
-"Bug Tracker" = "https://github.com/suyashsonkesaria/robocopy/issues"
+"Bug Tracker" = "https://github.com/suyashsonkesaria/robocopy/issues"
```

