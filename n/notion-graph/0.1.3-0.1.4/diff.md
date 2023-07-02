# Comparing `tmp/notion-graph-0.1.3.tar.gz` & `tmp/notion-graph-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "notion-graph-0.1.3.tar", last modified: Thu May 25 14:03:10 2023, max compression
+gzip compressed data, was "notion-graph-0.1.4.tar", last modified: Sun Jul  2 04:59:55 2023, max compression
```

## Comparing `notion-graph-0.1.3.tar` & `notion-graph-0.1.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1066 2023-05-02 02:00:02.124145 notion-graph-0.1.3/LICENSE
--rw-r--r--   0        0        0     3903 2023-05-21 03:01:12.541854 notion-graph-0.1.3/README.md
--rw-r--r--   0        0        0      634 2023-01-23 09:07:31.524157 notion-graph-0.1.3/notion_graph/__init__.py
--rw-r--r--   0        0        0       61 2023-01-23 09:07:31.524157 notion-graph-0.1.3/notion_graph/__main__.py
--rw-r--r--   0        0        0      762 2023-05-21 03:01:12.541854 notion-graph-0.1.3/notion_graph/cli.py
--rw-r--r--   0        0        0      251 2023-01-23 09:07:31.524157 notion-graph-0.1.3/notion_graph/helper.py
--rw-r--r--   0        0        0    11412 2023-05-25 14:01:51.438113 notion-graph-0.1.3/notion_graph/parser.py
--rw-r--r--   0        0        0      523 2023-05-25 14:02:35.628101 notion-graph-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     4164 1970-01-01 00:00:00.000000 notion-graph-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-05-02 02:00:02.124145 notion-graph-0.1.4/LICENSE
+-rw-r--r--   0        0        0     3903 2023-05-21 03:01:12.541854 notion-graph-0.1.4/README.md
+-rw-r--r--   0        0        0      634 2023-01-23 09:07:31.524157 notion-graph-0.1.4/notion_graph/__init__.py
+-rw-r--r--   0        0        0       61 2023-01-23 09:07:31.524157 notion-graph-0.1.4/notion_graph/__main__.py
+-rw-r--r--   0        0        0      762 2023-05-21 03:01:12.541854 notion-graph-0.1.4/notion_graph/cli.py
+-rw-r--r--   0        0        0      251 2023-01-23 09:07:31.524157 notion-graph-0.1.4/notion_graph/helper.py
+-rw-r--r--   0        0        0    11412 2023-05-25 14:01:51.438113 notion-graph-0.1.4/notion_graph/parser.py
+-rw-r--r--   0        0        0      521 2023-07-02 04:59:33.141565 notion-graph-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     4164 1970-01-01 00:00:00.000000 notion-graph-0.1.4/PKG-INFO
```

### Comparing `notion-graph-0.1.3/LICENSE` & `notion-graph-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `notion-graph-0.1.3/README.md` & `notion-graph-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `notion-graph-0.1.3/notion_graph/__init__.py` & `notion-graph-0.1.4/notion_graph/__init__.py`

 * *Files identical despite different names*

### Comparing `notion-graph-0.1.3/notion_graph/cli.py` & `notion-graph-0.1.4/notion_graph/cli.py`

 * *Files identical despite different names*

### Comparing `notion-graph-0.1.3/notion_graph/parser.py` & `notion-graph-0.1.4/notion_graph/parser.py`

 * *Files identical despite different names*

### Comparing `notion-graph-0.1.3/pyproject.toml` & `notion-graph-0.1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.pdm.scripts]
 start = "python -m notion_graph"
 
 [project]
 name = "notion-graph"
-version = "0.1.3"
+version = "0.1.4"
 description = "Generate a roam research like network graph view from your Notion pages."
 authors = [
     { name = "Steve Sun", email = "sund.chn@gmail.com" },
 ]
 dependencies = [
     "notion-client>=2.0.0",
     "networkx>=3.0",
-    "matplotlib>=3.6.3",
+    "matplotlib>=3.5",
 ]
 requires-python = ">=3.9"
 readme = "README.md"
 
 [project.license]
 text = "MIT"
```

### Comparing `notion-graph-0.1.3/PKG-INFO` & `notion-graph-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: notion-graph
-Version: 0.1.3
+Version: 0.1.4
 Summary: Generate a roam research like network graph view from your Notion pages.
 License: MIT
 Author-email: Steve Sun <sund.chn@gmail.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 ![](images/snap.png)
```

