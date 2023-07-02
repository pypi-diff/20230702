# Comparing `tmp/qmp-0.0.1.tar.gz` & `tmp/qmp-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/qmp-0.0.1.tar", last modified: Sat Mar 30 15:31:28 2019, max compression
+gzip compressed data, was "qmp-1.0.0.tar", last modified: Sun Jul  2 20:45:45 2023, max compression
```

## Comparing `qmp-0.0.1.tar` & `qmp-1.0.0.tar`

### file list

```diff
@@ -1,11 +1,12 @@
-drwxr-xr-x   0 abogdanenko  (1000) abogdanenko  (1000)        0 2019-03-30 15:31:28.000000 qmp-0.0.1/
--rw-r--r--   0 abogdanenko  (1000) abogdanenko  (1000)     1278 2019-03-30 15:31:28.000000 qmp-0.0.1/PKG-INFO
--rw-r--r--   0 abogdanenko  (1000) abogdanenko  (1000)      672 2019-03-30 08:09:21.000000 qmp-0.0.1/README.md
-drwxr-xr-x   0 abogdanenko  (1000) abogdanenko  (1000)        0 2019-03-30 15:31:28.000000 qmp-0.0.1/qmp.egg-info/
--rw-r--r--   0 abogdanenko  (1000) abogdanenko  (1000)     1278 2019-03-30 15:31:28.000000 qmp-0.0.1/qmp.egg-info/PKG-INFO
--rw-r--r--   0 abogdanenko  (1000) abogdanenko  (1000)      133 2019-03-30 15:31:28.000000 qmp-0.0.1/qmp.egg-info/SOURCES.txt
--rw-r--r--   0 abogdanenko  (1000) abogdanenko  (1000)        1 2019-03-30 15:31:28.000000 qmp-0.0.1/qmp.egg-info/dependency_links.txt
--rw-r--r--   0 abogdanenko  (1000) abogdanenko  (1000)        4 2019-03-30 15:31:28.000000 qmp-0.0.1/qmp.egg-info/top_level.txt
--rw-r--r--   0 abogdanenko  (1000) abogdanenko  (1000)     8244 2019-03-24 07:49:40.000000 qmp-0.0.1/qmp.py
--rw-r--r--   0 abogdanenko  (1000) abogdanenko  (1000)       38 2019-03-30 15:31:28.000000 qmp-0.0.1/setup.cfg
--rw-r--r--   0 abogdanenko  (1000) abogdanenko  (1000)      596 2019-03-30 13:49:18.000000 qmp-0.0.1/setup.py
+drwxr-xr-x   0 abogdanenko  (1000) abogdanenko  (1000)        0 2023-07-02 20:45:45.177517 qmp-1.0.0/
+-rw-r--r--   0 abogdanenko  (1000) abogdanenko  (1000)    18092 2023-07-02 20:10:38.000000 qmp-1.0.0/LICENSE
+-rw-r--r--   0 abogdanenko  (1000) abogdanenko  (1000)     1954 2023-07-02 20:45:45.177517 qmp-1.0.0/PKG-INFO
+-rw-r--r--   0 abogdanenko  (1000) abogdanenko  (1000)      984 2023-07-02 20:10:18.000000 qmp-1.0.0/README.md
+-rw-r--r--   0 abogdanenko  (1000) abogdanenko  (1000)     1038 2023-07-02 20:44:14.000000 qmp-1.0.0/pyproject.toml
+drwxr-xr-x   0 abogdanenko  (1000) abogdanenko  (1000)        0 2023-07-02 20:45:45.177517 qmp-1.0.0/qmp.egg-info/
+-rw-r--r--   0 abogdanenko  (1000) abogdanenko  (1000)     1954 2023-07-02 20:45:45.000000 qmp-1.0.0/qmp.egg-info/PKG-INFO
+-rw-r--r--   0 abogdanenko  (1000) abogdanenko  (1000)      147 2023-07-02 20:45:45.000000 qmp-1.0.0/qmp.egg-info/SOURCES.txt
+-rw-r--r--   0 abogdanenko  (1000) abogdanenko  (1000)        1 2023-07-02 20:45:45.000000 qmp-1.0.0/qmp.egg-info/dependency_links.txt
+-rw-r--r--   0 abogdanenko  (1000) abogdanenko  (1000)        4 2023-07-02 20:45:45.000000 qmp-1.0.0/qmp.egg-info/top_level.txt
+-rw-r--r--   0 abogdanenko  (1000) abogdanenko  (1000)     8244 2023-07-02 12:55:24.000000 qmp-1.0.0/qmp.py
+-rw-r--r--   0 abogdanenko  (1000) abogdanenko  (1000)       38 2023-07-02 20:45:45.177517 qmp-1.0.0/setup.cfg
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `qmp-0.0.1/qmp.py` & `qmp-1.0.0/qmp.py`

 * *Files identical despite different names*

