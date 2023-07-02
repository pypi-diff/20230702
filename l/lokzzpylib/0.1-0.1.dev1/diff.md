# Comparing `tmp/lokzzpylib-0.1.tar.gz` & `tmp/lokzzpylib-0.1.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lokzzpylib-0.1.tar", last modified: Sun Jul  2 01:43:47 2023, max compression
+gzip compressed data, was "lokzzpylib-0.1.dev1.tar", last modified: Sat Jul  1 16:19:14 2023, max compression
```

## Comparing `lokzzpylib-0.1.tar` & `lokzzpylib-0.1.dev1.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 01:43:47.603886 lokzzpylib-0.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 01:43:47.599886 lokzzpylib-0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 01:43:47.599886 lokzzpylib-0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-07-02 01:43:25.000000 lokzzpylib-0.1/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-02 01:43:25.000000 lokzzpylib-0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-02 01:43:25.000000 lokzzpylib-0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-07-02 01:43:47.603886 lokzzpylib-0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-02 01:43:25.000000 lokzzpylib-0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 01:43:47.599886 lokzzpylib-0.1/lokzzpylib/
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-02 01:43:25.000000 lokzzpylib-0.1/lokzzpylib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-07-02 01:43:25.000000 lokzzpylib-0.1/lokzzpylib/library.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 01:43:47.603886 lokzzpylib-0.1/lokzzpylib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-07-02 01:43:47.000000 lokzzpylib-0.1/lokzzpylib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-02 01:43:47.000000 lokzzpylib-0.1/lokzzpylib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 01:43:47.000000 lokzzpylib-0.1/lokzzpylib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-02 01:43:47.000000 lokzzpylib-0.1/lokzzpylib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-02 01:43:47.000000 lokzzpylib-0.1/lokzzpylib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-07-02 01:43:25.000000 lokzzpylib-0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 01:43:47.603886 lokzzpylib-0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 16:19:14.085306 lokzzpylib-0.1.dev1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 16:19:14.081306 lokzzpylib-0.1.dev1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 16:19:14.085306 lokzzpylib-0.1.dev1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-01 16:18:49.000000 lokzzpylib-0.1.dev1/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-01 16:18:49.000000 lokzzpylib-0.1.dev1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-01 16:18:49.000000 lokzzpylib-0.1.dev1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-01 16:19:14.085306 lokzzpylib-0.1.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-01 16:18:49.000000 lokzzpylib-0.1.dev1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 16:19:14.085306 lokzzpylib-0.1.dev1/lokzzpylib/
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-01 16:18:49.000000 lokzzpylib-0.1.dev1/lokzzpylib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-07-01 16:18:49.000000 lokzzpylib-0.1.dev1/lokzzpylib/library.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 16:19:14.085306 lokzzpylib-0.1.dev1/lokzzpylib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-01 16:19:14.000000 lokzzpylib-0.1.dev1/lokzzpylib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-07-01 16:19:14.000000 lokzzpylib-0.1.dev1/lokzzpylib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 16:19:14.000000 lokzzpylib-0.1.dev1/lokzzpylib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-01 16:19:14.000000 lokzzpylib-0.1.dev1/lokzzpylib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-01 16:19:14.000000 lokzzpylib-0.1.dev1/lokzzpylib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-07-01 16:18:49.000000 lokzzpylib-0.1.dev1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 16:19:14.085306 lokzzpylib-0.1.dev1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-01 16:18:49.000000 lokzzpylib-0.1.dev1/upload.bat
```

### Comparing `lokzzpylib-0.1/.github/workflows/python-publish.yml` & `lokzzpylib-0.1.dev1/.github/workflows/python-publish.yml`

 * *Files 17% similar despite different names*

```diff
@@ -15,20 +15,19 @@
 
 jobs:
   deploy:
 
     runs-on: ubuntu-latest
 
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v3
     - name: Set up Python
       uses: actions/setup-python@v3
       with:
         python-version: '3.10.7'
-        fetch-depth: 0
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         pip install build
     - name: Build package
       run: python -m build
     - name: Publish package
```

### Comparing `lokzzpylib-0.1/lokzzpylib/library.py` & `lokzzpylib-0.1.dev1/lokzzpylib/library.py`

 * *Files identical despite different names*

### Comparing `lokzzpylib-0.1/pyproject.toml` & `lokzzpylib-0.1.dev1/pyproject.toml`

 * *Files identical despite different names*

