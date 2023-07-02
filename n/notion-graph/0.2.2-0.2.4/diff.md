# Comparing `tmp/notion-graph-0.2.2.tar.gz` & `tmp/notion-graph-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "notion-graph-0.2.2.tar", last modified: Sun Jul  2 09:22:25 2023, max compression
+gzip compressed data, was "notion-graph-0.2.4.tar", last modified: Sun Jul  2 09:42:12 2023, max compression
```

## Comparing `notion-graph-0.2.2.tar` & `notion-graph-0.2.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1066 2023-05-02 02:00:02.124145 notion-graph-0.2.2/LICENSE
--rw-r--r--   0        0        0     3290 2023-07-02 08:57:00.186981 notion-graph-0.2.2/README.md
--rw-r--r--   0        0        0      636 2023-07-02 08:41:31.147282 notion-graph-0.2.2/notion_graph/__init__.py
--rw-r--r--   0        0        0       61 2023-01-23 09:07:31.524157 notion-graph-0.2.2/notion_graph/__main__.py
--rw-r--r--   0        0        0      641 2023-07-02 08:22:59.337641 notion-graph-0.2.2/notion_graph/cli.py
--rw-r--r--   0        0        0      426 2023-07-02 07:53:07.888215 notion-graph-0.2.2/notion_graph/helper.py
--rw-r--r--   0        0        0    11153 2023-07-02 09:20:21.666533 notion-graph-0.2.2/notion_graph/parser.py
--rw-r--r--   0        0        0      497 2023-07-02 09:20:37.756528 notion-graph-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     3551 1970-01-01 00:00:00.000000 notion-graph-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-05-02 02:00:02.124145 notion-graph-0.2.4/LICENSE
+-rw-r--r--   0        0        0     3435 2023-07-02 09:38:08.986188 notion-graph-0.2.4/README.md
+-rw-r--r--   0        0        0      636 2023-07-02 08:41:31.147282 notion-graph-0.2.4/notion_graph/__init__.py
+-rw-r--r--   0        0        0       61 2023-01-23 09:07:31.524157 notion-graph-0.2.4/notion_graph/__main__.py
+-rw-r--r--   0        0        0      641 2023-07-02 08:22:59.337641 notion-graph-0.2.4/notion_graph/cli.py
+-rw-r--r--   0        0        0      426 2023-07-02 07:53:07.888215 notion-graph-0.2.4/notion_graph/helper.py
+-rw-r--r--   0        0        0    11160 2023-07-02 09:41:23.606129 notion-graph-0.2.4/notion_graph/parser.py
+-rw-r--r--   0        0        0      497 2023-07-02 09:41:48.616120 notion-graph-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     3696 1970-01-01 00:00:00.000000 notion-graph-0.2.4/PKG-INFO
```

### Comparing `notion-graph-0.2.2/LICENSE` & `notion-graph-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `notion-graph-0.2.2/README.md` & `notion-graph-0.2.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+Metadata-Version: 2.1
+Name: notion-graph
+Version: 0.2.4
+Summary: Generate a roam research like network graph view from your Notion pages.
+License: MIT
+Author-email: Steve Sun <sund.chn@gmail.com>
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+
 ![](images/snap.png)
 
 # Notion Graph View
 
 ![github](https://img.shields.io/badge/python-3.9-blue.svg) ![github](https://img.shields.io/badge/license-MIT-green.svg) ![github](https://img.shields.io/badge/notion_version-2022.06.28-lightgrey.svg)
 
 Export [Notion](https://notion.so) pages to a Roam-Research like graph view.
@@ -43,23 +52,27 @@
 
 `graph_out.html` would be generated at your specific path.
 
 ### Importing as a Python Library
 
 You can also import `notion_graph` as a library.
 
-For instance, drawing your own diagram in Jupyter Notebook by [pyvis](https://pyvis.readthedocs.io/en/latest/).
+For instance, drawing your own diagram in Jupyter Notebook.
 
 ```python
 import notion_graph as ng
 
 my_ng = ng.NotionGraph(bearer_token="secret_b8p7uLp3j3n95IDgofC9GviXP111Skx6NOt2d20U8e")
-graph = my_ng.parse(page_id="856391c93ae64bd1b7ebf699ca0cd861")
-# graph is a pyvis.network.Network object
-graph.show("graph.html", notebook=True)
+network = my_ng.parse(page_id="856391c93ae64bd1b7ebf699ca0cd861")
+# `network` is a `pyvis.network.Network` object, see more attributes: https://pyvis.readthedocs.io/en/latest/documentation.html
+network.repulsion(node_distance=200, spring_length=200)
+# this line is for jupeter notebook only
+network.prep_notebook()
+
+network.show("graph.html")
 ```
 
 ## Testing Environment
 
 The testing page is [Notion-grap-view-demo](https://sund.notion.site/Notion-graph-view-Demo-856391c93ae64bd1b7ebf699ca0cd861). You can duplicate the page to your Notion account and run the project to test if everything goes well.
 
 ## Development Guide
@@ -96,7 +109,8 @@
 | heading_3          | ✔️       | ✔️   |
 | column             |          |      |
 | column_list        |          |      |
 | synced_block       |          |      |
 | link_to_page       |          |      |
 | table              | ✔️       | ✔️   |
 | table_row          | ✔️       | ✔️   |
+
```

### Comparing `notion-graph-0.2.2/notion_graph/__init__.py` & `notion-graph-0.2.4/notion_graph/__init__.py`

 * *Files identical despite different names*

### Comparing `notion-graph-0.2.2/notion_graph/cli.py` & `notion-graph-0.2.4/notion_graph/cli.py`

 * *Files identical despite different names*

### Comparing `notion-graph-0.2.2/notion_graph/parser.py` & `notion-graph-0.2.4/notion_graph/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,16 +30,16 @@
 class Parser:
     def __init__(self, notion_version: str, bearer_token: str) -> None:
         self._notion = Client(notion_version=notion_version, auth=bearer_token)
         self._graph = Network(bgcolor="#222222",
                               font_color="white",
                               height="750px",
                               width="100%",
+                              cdn_resources="in_line",
                               select_menu=True,
-                              filter_menu=True,
                               )
 
     def parse(self, root_id: str) -> Network:
         self._parse_block(root_id)
         return self._graph
 
     def export_to_html(self, file_path: str):
```

### Comparing `notion-graph-0.2.2/PKG-INFO` & `notion-graph-0.2.4/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,7 @@
-Metadata-Version: 2.1
-Name: notion-graph
-Version: 0.2.2
-Summary: Generate a roam research like network graph view from your Notion pages.
-License: MIT
-Author-email: Steve Sun <sund.chn@gmail.com>
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-
 ![](images/snap.png)
 
 # Notion Graph View
 
 ![github](https://img.shields.io/badge/python-3.9-blue.svg) ![github](https://img.shields.io/badge/license-MIT-green.svg) ![github](https://img.shields.io/badge/notion_version-2022.06.28-lightgrey.svg)
 
 Export [Notion](https://notion.so) pages to a Roam-Research like graph view.
@@ -52,23 +43,27 @@
 
 `graph_out.html` would be generated at your specific path.
 
 ### Importing as a Python Library
 
 You can also import `notion_graph` as a library.
 
-For instance, drawing your own diagram in Jupyter Notebook by [pyvis](https://pyvis.readthedocs.io/en/latest/).
+For instance, drawing your own diagram in Jupyter Notebook.
 
 ```python
 import notion_graph as ng
 
 my_ng = ng.NotionGraph(bearer_token="secret_b8p7uLp3j3n95IDgofC9GviXP111Skx6NOt2d20U8e")
-graph = my_ng.parse(page_id="856391c93ae64bd1b7ebf699ca0cd861")
-# graph is a pyvis.network.Network object
-graph.show("graph.html", notebook=True)
+network = my_ng.parse(page_id="856391c93ae64bd1b7ebf699ca0cd861")
+# `network` is a `pyvis.network.Network` object, see more attributes: https://pyvis.readthedocs.io/en/latest/documentation.html
+network.repulsion(node_distance=200, spring_length=200)
+# this line is for jupeter notebook only
+network.prep_notebook()
+
+network.show("graph.html")
 ```
 
 ## Testing Environment
 
 The testing page is [Notion-grap-view-demo](https://sund.notion.site/Notion-graph-view-Demo-856391c93ae64bd1b7ebf699ca0cd861). You can duplicate the page to your Notion account and run the project to test if everything goes well.
 
 ## Development Guide
@@ -105,8 +100,7 @@
 | heading_3          | ✔️       | ✔️   |
 | column             |          |      |
 | column_list        |          |      |
 | synced_block       |          |      |
 | link_to_page       |          |      |
 | table              | ✔️       | ✔️   |
 | table_row          | ✔️       | ✔️   |
-
```

