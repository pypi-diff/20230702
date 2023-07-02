# Comparing `tmp/veleslibrary-0.0.0.tar.gz` & `tmp/veleslibrary-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "veleslibrary-0.0.0.tar", max compression
+gzip compressed data, was "veleslibrary-0.1.0.tar", max compression
```

## Comparing `veleslibrary-0.0.0.tar` & `veleslibrary-0.1.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       15 2023-07-01 13:27:28.732749 veleslibrary-0.0.0/README.md
--rw-r--r--   0        0        0      443 2023-07-01 13:35:04.048814 veleslibrary-0.0.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-01 13:30:07.625883 veleslibrary-0.0.0/veleslibrary/__init__.py
--rw-r--r--   0        0        0       30 2023-07-01 13:05:10.164733 veleslibrary-0.0.0/veleslibrary/questionnaires/__init__.py
--rw-r--r--   0        0        0       63 2023-07-01 13:05:10.164733 veleslibrary-0.0.0/veleslibrary/questionnaires/pl/__init__.py
--rw-r--r--   0        0        0     3113 2023-07-01 13:05:10.164733 veleslibrary-0.0.0/veleslibrary/questionnaires/pl/questionnaires.py
--rw-r--r--   0        0        0     2289 2023-07-01 13:08:05.247807 veleslibrary-0.0.0/veleslibrary/questionnaires/questionnaires.py
--rw-r--r--   0        0        0      410 1970-01-01 00:00:00.000000 veleslibrary-0.0.0/PKG-INFO
+-rw-r--r--   0        0        0       15 2023-07-02 09:53:57.546823 veleslibrary-0.1.0/README.md
+-rw-r--r--   0        0        0      443 2023-07-02 09:54:41.619713 veleslibrary-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-02 09:53:57.550823 veleslibrary-0.1.0/veleslibrary/__init__.py
+-rw-r--r--   0        0        0       30 2023-07-02 09:53:57.550823 veleslibrary-0.1.0/veleslibrary/questionnaires/__init__.py
+-rw-r--r--   0        0        0       63 2023-07-02 09:53:57.550823 veleslibrary-0.1.0/veleslibrary/questionnaires/pl/__init__.py
+-rw-r--r--   0        0        0     3113 2023-07-02 09:53:57.550823 veleslibrary-0.1.0/veleslibrary/questionnaires/pl/questionnaires.py
+-rw-r--r--   0        0        0     2289 2023-07-02 09:53:57.550823 veleslibrary-0.1.0/veleslibrary/questionnaires/questionnaires.py
+-rw-r--r--   0        0        0      410 1970-01-01 00:00:00.000000 veleslibrary-0.1.0/PKG-INFO
```

### Comparing `veleslibrary-0.0.0/veleslibrary/questionnaires/pl/questionnaires.py` & `veleslibrary-0.1.0/veleslibrary/questionnaires/pl/questionnaires.py`

 * *Files identical despite different names*

### Comparing `veleslibrary-0.0.0/veleslibrary/questionnaires/questionnaires.py` & `veleslibrary-0.1.0/veleslibrary/questionnaires/questionnaires.py`

 * *Files identical despite different names*

