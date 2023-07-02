# Comparing `tmp/lokzzpylib-0.1.dev1.tar.gz` & `tmp/lokzzpylib-0.2.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lokzzpylib-0.1.dev1.tar", last modified: Sat Jul  1 16:19:14 2023, max compression
+gzip compressed data, was "lokzzpylib-0.2.dev2.tar", last modified: Sun Jul  2 01:48:18 2023, max compression
```

## Comparing `lokzzpylib-0.1.dev1.tar` & `lokzzpylib-0.2.dev2.tar`

### file list

```diff
@@ -1,20 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 16:19:14.085306 lokzzpylib-0.1.dev1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 16:19:14.081306 lokzzpylib-0.1.dev1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 16:19:14.085306 lokzzpylib-0.1.dev1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-01 16:18:49.000000 lokzzpylib-0.1.dev1/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-01 16:18:49.000000 lokzzpylib-0.1.dev1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-01 16:18:49.000000 lokzzpylib-0.1.dev1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-01 16:19:14.085306 lokzzpylib-0.1.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-01 16:18:49.000000 lokzzpylib-0.1.dev1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 16:19:14.085306 lokzzpylib-0.1.dev1/lokzzpylib/
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-01 16:18:49.000000 lokzzpylib-0.1.dev1/lokzzpylib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-07-01 16:18:49.000000 lokzzpylib-0.1.dev1/lokzzpylib/library.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 16:19:14.085306 lokzzpylib-0.1.dev1/lokzzpylib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-01 16:19:14.000000 lokzzpylib-0.1.dev1/lokzzpylib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-07-01 16:19:14.000000 lokzzpylib-0.1.dev1/lokzzpylib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 16:19:14.000000 lokzzpylib-0.1.dev1/lokzzpylib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-01 16:19:14.000000 lokzzpylib-0.1.dev1/lokzzpylib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-01 16:19:14.000000 lokzzpylib-0.1.dev1/lokzzpylib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-07-01 16:18:49.000000 lokzzpylib-0.1.dev1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 16:19:14.085306 lokzzpylib-0.1.dev1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-01 16:18:49.000000 lokzzpylib-0.1.dev1/upload.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 01:48:18.331812 lokzzpylib-0.2.dev2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 01:48:18.327812 lokzzpylib-0.2.dev2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 01:48:18.327812 lokzzpylib-0.2.dev2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-02 01:47:57.000000 lokzzpylib-0.2.dev2/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-02 01:47:57.000000 lokzzpylib-0.2.dev2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-02 01:47:57.000000 lokzzpylib-0.2.dev2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-02 01:48:18.331812 lokzzpylib-0.2.dev2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-02 01:47:57.000000 lokzzpylib-0.2.dev2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 01:48:18.327812 lokzzpylib-0.2.dev2/lokzzpylib/
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-02 01:47:57.000000 lokzzpylib-0.2.dev2/lokzzpylib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-07-02 01:47:57.000000 lokzzpylib-0.2.dev2/lokzzpylib/library.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 01:48:18.331812 lokzzpylib-0.2.dev2/lokzzpylib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-02 01:48:18.000000 lokzzpylib-0.2.dev2/lokzzpylib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-02 01:48:18.000000 lokzzpylib-0.2.dev2/lokzzpylib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 01:48:18.000000 lokzzpylib-0.2.dev2/lokzzpylib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-02 01:48:18.000000 lokzzpylib-0.2.dev2/lokzzpylib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-02 01:48:18.000000 lokzzpylib-0.2.dev2/lokzzpylib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-07-02 01:47:57.000000 lokzzpylib-0.2.dev2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 01:48:18.331812 lokzzpylib-0.2.dev2/setup.cfg
```

### Comparing `lokzzpylib-0.1.dev1/.github/workflows/python-publish.yml` & `lokzzpylib-0.2.dev2/.github/workflows/python-publish.yml`

 * *Files 9% similar despite different names*

```diff
@@ -15,15 +15,17 @@
 
 jobs:
   deploy:
 
     runs-on: ubuntu-latest
 
     steps:
-    - uses: actions/checkout@v3
+    - uses: actions/checkout@v2
+      with:
+        fetch-depth: 0
     - name: Set up Python
       uses: actions/setup-python@v3
       with:
         python-version: '3.10.7'
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
```

### Comparing `lokzzpylib-0.1.dev1/lokzzpylib/library.py` & `lokzzpylib-0.2.dev2/lokzzpylib/library.py`

 * *Files identical despite different names*

### Comparing `lokzzpylib-0.1.dev1/pyproject.toml` & `lokzzpylib-0.2.dev2/pyproject.toml`

 * *Files identical despite different names*

