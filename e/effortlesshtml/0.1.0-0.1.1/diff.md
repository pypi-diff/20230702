# Comparing `tmp/effortlesshtml-0.1.0.tar.gz` & `tmp/effortlesshtml-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "effortlesshtml-0.1.0.tar", max compression
+gzip compressed data, was "effortlesshtml-0.1.1.tar", max compression
```

## Comparing `effortlesshtml-0.1.0.tar` & `effortlesshtml-0.1.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1074 2023-07-02 06:24:58.648948 effortlesshtml-0.1.0/LICENSE
--rwxr-xr-x   0        0        0     2076 2023-07-02 13:17:02.524325 effortlesshtml-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-07-02 13:04:46.461078 effortlesshtml-0.1.0/effortlessHTML/__init__.py
--rw-r--r--   0        0        0       46 2023-07-02 13:04:46.461525 effortlesshtml-0.1.0/effortlessHTML/attributes/__init__.py
--rw-r--r--   0        0        0      725 2023-07-02 13:04:46.461809 effortlesshtml-0.1.0/effortlessHTML/attributes/base.py
--rw-r--r--   0        0        0       63 2023-07-02 13:04:46.462130 effortlesshtml-0.1.0/effortlessHTML/elements/__init__.py
--rw-r--r--   0        0        0     2673 2023-07-02 13:17:02.521154 effortlesshtml-0.1.0/effortlessHTML/elements/base.py
--rw-r--r--   0        0        0      647 2023-07-02 13:17:02.532176 effortlesshtml-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2409 1970-01-01 00:00:00.000000 effortlesshtml-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-07-02 13:37:13.753533 effortlesshtml-0.1.1/LICENSE
+-rwxr-xr-x   0        0        0     2076 2023-07-02 13:37:13.753533 effortlesshtml-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-07-02 13:37:13.753533 effortlesshtml-0.1.1/effortlessHTML/__init__.py
+-rw-r--r--   0        0        0       46 2023-07-02 13:37:13.753533 effortlesshtml-0.1.1/effortlessHTML/attributes/__init__.py
+-rw-r--r--   0        0        0      725 2023-07-02 13:37:13.753533 effortlesshtml-0.1.1/effortlessHTML/attributes/base.py
+-rw-r--r--   0        0        0       72 2023-07-02 13:37:13.753533 effortlesshtml-0.1.1/effortlessHTML/elements/__init__.py
+-rw-r--r--   0        0        0     2732 2023-07-02 13:37:13.753533 effortlesshtml-0.1.1/effortlessHTML/elements/base.py
+-rw-r--r--   0        0        0      647 2023-07-02 13:37:13.757533 effortlesshtml-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2409 1970-01-01 00:00:00.000000 effortlesshtml-0.1.1/PKG-INFO
```

### Comparing `effortlesshtml-0.1.0/LICENSE` & `effortlesshtml-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `effortlesshtml-0.1.0/README.md` & `effortlesshtml-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `effortlesshtml-0.1.0/effortlessHTML/attributes/base.py` & `effortlesshtml-0.1.1/effortlessHTML/attributes/base.py`

 * *Files identical despite different names*

### Comparing `effortlesshtml-0.1.0/effortlessHTML/elements/base.py` & `effortlesshtml-0.1.1/effortlessHTML/elements/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -79,7 +79,11 @@
 
 class span(HTMLElement):
     ELEMENT_TYPE = "span"
 
 
 class strong(HTMLElement):
     ELEMENT_TYPE = "strong"
+
+
+class section(HTMLElement):
+    ELEMENT_TYPE = "section"
```

### Comparing `effortlesshtml-0.1.0/pyproject.toml` & `effortlesshtml-0.1.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "effortlessHTML"
-version = "0.1.0"
+version = "0.1.1"
 description = "Simple python templating engine for html"
 authors = ["Togo <TogoTheBlackDog@panther.com>"]
 readme = "README.md"
 packages = [{include = "effortlessHTML"}]
 
 [tool.poetry.group.dev.dependencies]
 ipython = "*"
```

### Comparing `effortlesshtml-0.1.0/PKG-INFO` & `effortlesshtml-0.1.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: effortlesshtml
-Version: 0.1.0
+Version: 0.1.1
 Summary: Simple python templating engine for html
 Author: Togo
 Author-email: TogoTheBlackDog@panther.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
```

