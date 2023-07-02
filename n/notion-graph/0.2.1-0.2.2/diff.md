# Comparing `tmp/notion-graph-0.2.1.tar.gz` & `tmp/notion-graph-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "notion-graph-0.2.1.tar", last modified: Sun Jul  2 08:46:28 2023, max compression
+gzip compressed data, was "notion-graph-0.2.2.tar", last modified: Sun Jul  2 09:22:25 2023, max compression
```

## Comparing `notion-graph-0.2.1.tar` & `notion-graph-0.2.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1066 2023-05-02 02:00:02.124145 notion-graph-0.2.1/LICENSE
--rw-r--r--   0        0        0     3270 2023-07-02 08:46:13.727193 notion-graph-0.2.1/README.md
--rw-r--r--   0        0        0      636 2023-07-02 08:41:31.147282 notion-graph-0.2.1/notion_graph/__init__.py
--rw-r--r--   0        0        0       61 2023-01-23 09:07:31.524157 notion-graph-0.2.1/notion_graph/__main__.py
--rw-r--r--   0        0        0      641 2023-07-02 08:22:59.337641 notion-graph-0.2.1/notion_graph/cli.py
--rw-r--r--   0        0        0      426 2023-07-02 07:53:07.888215 notion-graph-0.2.1/notion_graph/helper.py
--rw-r--r--   0        0        0    11159 2023-07-02 08:36:34.967377 notion-graph-0.2.1/notion_graph/parser.py
--rw-r--r--   0        0        0      497 2023-07-02 08:40:25.397301 notion-graph-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     3531 1970-01-01 00:00:00.000000 notion-graph-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-05-02 02:00:02.124145 notion-graph-0.2.2/LICENSE
+-rw-r--r--   0        0        0     3290 2023-07-02 08:57:00.186981 notion-graph-0.2.2/README.md
+-rw-r--r--   0        0        0      636 2023-07-02 08:41:31.147282 notion-graph-0.2.2/notion_graph/__init__.py
+-rw-r--r--   0        0        0       61 2023-01-23 09:07:31.524157 notion-graph-0.2.2/notion_graph/__main__.py
+-rw-r--r--   0        0        0      641 2023-07-02 08:22:59.337641 notion-graph-0.2.2/notion_graph/cli.py
+-rw-r--r--   0        0        0      426 2023-07-02 07:53:07.888215 notion-graph-0.2.2/notion_graph/helper.py
+-rw-r--r--   0        0        0    11153 2023-07-02 09:20:21.666533 notion-graph-0.2.2/notion_graph/parser.py
+-rw-r--r--   0        0        0      497 2023-07-02 09:20:37.756528 notion-graph-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     3551 1970-01-01 00:00:00.000000 notion-graph-0.2.2/PKG-INFO
```

### Comparing `notion-graph-0.2.1/LICENSE` & `notion-graph-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `notion-graph-0.2.1/README.md` & `notion-graph-0.2.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 
 `graph_out.html` would be generated at your specific path.
 
 ### Importing as a Python Library
 
 You can also import `notion_graph` as a library.
 
-For instance, drawing your own diagram by [pyvis](https://pyvis.readthedocs.io/en/latest/).
+For instance, drawing your own diagram in Jupyter Notebook by [pyvis](https://pyvis.readthedocs.io/en/latest/).
 
 ```python
 import notion_graph as ng
 
 my_ng = ng.NotionGraph(bearer_token="secret_b8p7uLp3j3n95IDgofC9GviXP111Skx6NOt2d20U8e")
 graph = my_ng.parse(page_id="856391c93ae64bd1b7ebf699ca0cd861")
 # graph is a pyvis.network.Network object
```

### Comparing `notion-graph-0.2.1/notion_graph/__init__.py` & `notion-graph-0.2.2/notion_graph/__init__.py`

 * *Files identical despite different names*

### Comparing `notion-graph-0.2.1/notion_graph/cli.py` & `notion-graph-0.2.2/notion_graph/cli.py`

 * *Files identical despite different names*

### Comparing `notion-graph-0.2.1/notion_graph/parser.py` & `notion-graph-0.2.2/notion_graph/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     def parse(self, root_id: str) -> Network:
         self._parse_block(root_id)
         return self._graph
 
     def export_to_html(self, file_path: str):
         print('Graph is generated at:', file_path)
         self._graph.repulsion(node_distance=200, spring_length=200)
-        self._graph.save_graph(file_path)
+        self._graph.show(file_path)
 
     def _parse_block(self, root_id: str, obj: dict = None) -> None:
         if obj is None:
             obj = self._notion.blocks.retrieve(root_id)
 
         self._parse_block_object(obj, root_id)
```

### Comparing `notion-graph-0.2.1/PKG-INFO` & `notion-graph-0.2.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: notion-graph
-Version: 0.2.1
+Version: 0.2.2
 Summary: Generate a roam research like network graph view from your Notion pages.
 License: MIT
 Author-email: Steve Sun <sund.chn@gmail.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 ![](images/snap.png)
@@ -52,15 +52,15 @@
 
 `graph_out.html` would be generated at your specific path.
 
 ### Importing as a Python Library
 
 You can also import `notion_graph` as a library.
 
-For instance, drawing your own diagram by [pyvis](https://pyvis.readthedocs.io/en/latest/).
+For instance, drawing your own diagram in Jupyter Notebook by [pyvis](https://pyvis.readthedocs.io/en/latest/).
 
 ```python
 import notion_graph as ng
 
 my_ng = ng.NotionGraph(bearer_token="secret_b8p7uLp3j3n95IDgofC9GviXP111Skx6NOt2d20U8e")
 graph = my_ng.parse(page_id="856391c93ae64bd1b7ebf699ca0cd861")
 # graph is a pyvis.network.Network object
```

