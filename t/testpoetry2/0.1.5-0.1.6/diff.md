# Comparing `tmp/testpoetry2-0.1.5.tar.gz` & `tmp/testpoetry2-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testpoetry2-0.1.5.tar", max compression
+gzip compressed data, was "testpoetry2-0.1.6.tar", max compression
```

## Comparing `testpoetry2-0.1.5.tar` & `testpoetry2-0.1.6.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      356 2023-07-02 14:54:36.088685 testpoetry2-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     1438 2023-07-02 13:58:42.684298 testpoetry2-0.1.5/README.md
--rw-r--r--   0        0        0      269 2023-07-02 21:10:54.783989 testpoetry2-0.1.5/testpoetry2/__init__.py
--rw-r--r--   0        0        0      118 2023-07-02 15:03:07.864639 testpoetry2-0.1.5/testpoetry2/__main__.py
--rw-r--r--   0        0        0       23 2023-07-02 14:55:03.430333 testpoetry2-0.1.5/testpoetry2/__version__.py
--rw-r--r--   0        0        0        0 2023-07-01 17:53:06.262853 testpoetry2-0.1.5/testpoetry2/console/__init__.py
--rw-r--r--   0        0        0     4475 2023-07-02 21:10:54.804990 testpoetry2-0.1.5/testpoetry2/console/application.py
--rw-r--r--   0        0        0     7732 2023-07-02 21:10:54.792991 testpoetry2-0.1.5/testpoetry2/pwgen.py
--rw-r--r--   0        0        0     1803 1970-01-01 00:00:00.000000 testpoetry2-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0      390 2023-07-02 21:29:55.254124 testpoetry2-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     1438 2023-07-02 13:58:42.684298 testpoetry2-0.1.6/README.md
+-rw-r--r--   0        0        0      269 2023-07-02 21:10:54.783989 testpoetry2-0.1.6/testpoetry2/__init__.py
+-rw-r--r--   0        0        0      118 2023-07-02 15:03:07.864639 testpoetry2-0.1.6/testpoetry2/__main__.py
+-rw-r--r--   0        0        0       23 2023-07-02 21:29:55.249136 testpoetry2-0.1.6/testpoetry2/__version__.py
+-rw-r--r--   0        0        0        0 2023-07-01 17:53:06.262853 testpoetry2-0.1.6/testpoetry2/console/__init__.py
+-rw-r--r--   0        0        0     4475 2023-07-02 21:10:54.804990 testpoetry2-0.1.6/testpoetry2/console/application.py
+-rw-r--r--   0        0        0     7732 2023-07-02 21:10:54.792991 testpoetry2-0.1.6/testpoetry2/pwgen.py
+-rw-r--r--   0        0        0     1837 1970-01-01 00:00:00.000000 testpoetry2-0.1.6/PKG-INFO
```

### Comparing `testpoetry2-0.1.5/README.md` & `testpoetry2-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `testpoetry2-0.1.5/testpoetry2/console/application.py` & `testpoetry2-0.1.6/testpoetry2/console/application.py`

 * *Files identical despite different names*

### Comparing `testpoetry2-0.1.5/testpoetry2/pwgen.py` & `testpoetry2-0.1.6/testpoetry2/pwgen.py`

 * *Files identical despite different names*

### Comparing `testpoetry2-0.1.5/PKG-INFO` & `testpoetry2-0.1.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: testpoetry2
-Version: 0.1.5
-Summary: 
+Version: 0.1.6
+Summary: Password generator CLI and library
 Author: Bill.Avramenko
 Author-email: billavramenko@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: questionary (>=1.10.0,<2.0.0)
```

