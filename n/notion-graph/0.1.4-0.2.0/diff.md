# Comparing `tmp/notion-graph-0.1.4.tar.gz` & `tmp/notion-graph-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "notion-graph-0.1.4.tar", last modified: Sun Jul  2 04:59:55 2023, max compression
+gzip compressed data, was "notion-graph-0.2.0.tar", last modified: Sun Jul  2 08:30:17 2023, max compression
```

## Comparing `notion-graph-0.1.4.tar` & `notion-graph-0.2.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1066 2023-05-02 02:00:02.124145 notion-graph-0.1.4/LICENSE
--rw-r--r--   0        0        0     3903 2023-05-21 03:01:12.541854 notion-graph-0.1.4/README.md
--rw-r--r--   0        0        0      634 2023-01-23 09:07:31.524157 notion-graph-0.1.4/notion_graph/__init__.py
--rw-r--r--   0        0        0       61 2023-01-23 09:07:31.524157 notion-graph-0.1.4/notion_graph/__main__.py
--rw-r--r--   0        0        0      762 2023-05-21 03:01:12.541854 notion-graph-0.1.4/notion_graph/cli.py
--rw-r--r--   0        0        0      251 2023-01-23 09:07:31.524157 notion-graph-0.1.4/notion_graph/helper.py
--rw-r--r--   0        0        0    11412 2023-05-25 14:01:51.438113 notion-graph-0.1.4/notion_graph/parser.py
--rw-r--r--   0        0        0      521 2023-07-02 04:59:33.141565 notion-graph-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     4164 1970-01-01 00:00:00.000000 notion-graph-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-05-02 02:00:02.124145 notion-graph-0.2.0/LICENSE
+-rw-r--r--   0        0        0     3907 2023-07-02 08:12:18.277844 notion-graph-0.2.0/README.md
+-rw-r--r--   0        0        0      623 2023-07-02 08:24:45.007607 notion-graph-0.2.0/notion_graph/__init__.py
+-rw-r--r--   0        0        0       61 2023-01-23 09:07:31.524157 notion-graph-0.2.0/notion_graph/__main__.py
+-rw-r--r--   0        0        0      641 2023-07-02 08:22:59.337641 notion-graph-0.2.0/notion_graph/cli.py
+-rw-r--r--   0        0        0      426 2023-07-02 07:53:07.888215 notion-graph-0.2.0/notion_graph/helper.py
+-rw-r--r--   0        0        0    11159 2023-07-02 08:28:53.627532 notion-graph-0.2.0/notion_graph/parser.py
+-rw-r--r--   0        0        0      497 2023-07-02 08:24:54.467604 notion-graph-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4168 1970-01-01 00:00:00.000000 notion-graph-0.2.0/PKG-INFO
```

### Comparing `notion-graph-0.1.4/LICENSE` & `notion-graph-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `notion-graph-0.1.4/README.md` & `notion-graph-0.2.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -34,25 +34,25 @@
 ```shell
 python -m notion_graph -p <Page ID> -t <Integration Token> -o <PNG file path to export>
 ```
 
 For instance,
 
 ```shell
-python -m notion_graph -p 856391c93ae64bd1b7ebf699ca0cd861 -t secret_b8p7uLp3j3n95IDgofC9GviXP111Skx6NOt2d20U8e -o ./graph_out.png
+python -m notion_graph -p 856391c93ae64bd1b7ebf699ca0cd861 -t secret_b8p7uLp3j3n95IDgofC9GviXP111Skx6NOt2d20U8e -o ./graph_out.html
 ```
 
-`graph_out.png` would be generated at your specific path.
+`graph_out.html` would be generated at your specific path.
 
 ### Specific Font Family
 
 Matplotlib by default does not support displaying Unicode characters. To resolve this issue, specify your local font family by using `-f`:
 
 ```shell
-python -m notion_graph -p 856391c93ae64bd1b7ebf699ca0cd861 -t secret_b8p7uLp3j3n95IDgofC9GviXP111Skx6NOt2d20U8e -o ./graph_out.png -f 'SimSun'
+python -m notion_graph -p 856391c93ae64bd1b7ebf699ca0cd861 -t secret_b8p7uLp3j3n95IDgofC9GviXP111Skx6NOt2d20U8e -o ./graph_out.html -f 'SimSun'
 ```
 
 ### Importing as a Python Library
 
 You can also import `notion_graph` as a library.
 
 For instance, drawing your own diagram by [matplotlib](https://matplotlib.org/).
@@ -94,15 +94,15 @@
 brew install pdm
 pdm install
 ```
 
 Running the project by:
 
 ```shell
-pdm run start -p <page_id> -t <notion_token> -o ./graph_out.png
+pdm run start -p <page_id> -t <notion_token> -o ./graph_out.html
 ```
 
 ## 🔗 Supported Links
 
 |                    | database | page |
 | ------------------ | -------- | ---- |
 | paragraph          | ✔️       | ✔️   |
```

### Comparing `notion-graph-0.1.4/notion_graph/__init__.py` & `notion-graph-0.2.0/notion_graph/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,10 +13,10 @@
     def __init__(self, bearer_token: str) -> None:
         self._parser = Parser(NOTION_VERSION, bearer_token)
 
     def parse(self, page_id: str) -> nx.Graph:
         """Parse a given Notion page, get the Networkx graph data object"""
         return self._parser.parse(page_id)
 
-    def export(self, png_file_path):
-        """Export the Networkx graph to a png file"""
-        return self._parser.export_to_png(png_file_path)
+    def export(self, file_path):
+        """Export the Networkx graph to a file"""
+        return self._parser.export_to_html(file_path)
```

### Comparing `notion-graph-0.1.4/notion_graph/cli.py` & `notion-graph-0.2.0/notion_graph/cli.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,18 +6,16 @@
 def main():
     parser = argparse.ArgumentParser(prog="notion-graph")
 
     parser.add_argument('--page', '-p', help='Notion page ID', required=True)
     parser.add_argument(
         '--token', '-t', help='Notion integration token', required=True)
     parser.add_argument(
-        '--out', '-o', help='Image output path, e.g. `./graph_out.png`', required=False, default="./graph_out.png")
-    parser.add_argument(
-        '--font', '-f', help='Specify font family e.g. `SimSun`', required=False)
+        '--out', '-o', help='Output path, e.g. `./graph_out.html`', required=False, default="./graph_out.html")
     args = parser.parse_args()
     parser = Parser(NOTION_VERSION, args.token)
     parser.parse(args.page)
-    parser.export_to_png(args.out, args.font)
+    parser.export_to_html(args.out)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `notion-graph-0.1.4/notion_graph/parser.py` & `notion-graph-0.2.0/notion_graph/parser.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,17 +7,16 @@
 property object -> relation object | mention object
 rich_text | title -> mention objects
 relation object -> page titles
 mention object -> database title | page title
 '''
 
 from notion_client import Client
-import networkx as nx
-import matplotlib.pyplot as plt
-from .helper import contains_mention_or_relation_type
+from pyvis.network import Network
+from .helper import contains_mention_or_relation_type, is_same_block_id
 
 __all__ = ["Parser"]
 
 # All heading blocks("heading_1", "heading_2", and "heading_3") support children when the is_toggleable property is true.
 SUPPORTED_BLOCK_TYPES = [
     "paragraph", "bulleted_list_item", "numbered_list_item", "toggle", "to_do", "quote", "callout",
     "column", "child_page", "child_database", "table", "table_row", "heading_1", "heading_2",  "heading_3"
@@ -27,46 +26,30 @@
     "relation", "rich_text", "title"
 ]
 
 
 class Parser:
     def __init__(self, notion_version: str, bearer_token: str) -> None:
         self._notion = Client(notion_version=notion_version, auth=bearer_token)
-        self._graph = nx.Graph()
-        self._caching_ids = set()
+        self._graph = Network(bgcolor="#222222",
+                              font_color="white",
+                              height="750px",
+                              width="100%",
+                              select_menu=True,
+                              filter_menu=True,
+                              )
 
-    def parse(self, root_id: str) -> nx.Graph:
+    def parse(self, root_id: str) -> Network:
         self._parse_block(root_id)
         return self._graph
 
-    def export_to_png(self, png_path: str, font: str):
-        pos = nx.spring_layout(self._graph)
-        labels = nx.get_node_attributes(self._graph, 'title')
-        font_family = 'sans-serif'
-        if font:
-            font_family = font
-
-        options = {
-            "node_size": 10,
-            "node_color": "black",
-            "edge_color": "tab:gray",
-            "linewidths": 0.5,
-            "font_family": font_family,
-            "font_size": 6,
-            "font_color": "black",
-            "width": 0.5,
-            "with_labels": True,
-            "labels": labels,
-            "alpha": 0.7,
-            "verticalalignment": 'bottom',
-        }
-
-        nx.draw(self._graph, pos, **options)
-        plt.savefig(png_path, dpi=300)
-        print('Graph image is generated at:', png_path)
+    def export_to_html(self, file_path: str):
+        print('Graph is generated at:', file_path)
+        self._graph.repulsion(node_distance=200, spring_length=200)
+        self._graph.save_graph(file_path)
 
     def _parse_block(self, root_id: str, obj: dict = None) -> None:
         if obj is None:
             obj = self._notion.blocks.retrieve(root_id)
 
         self._parse_block_object(obj, root_id)
 
@@ -272,15 +255,15 @@
             }
         ]
         '''
         for relation_obj in relation_list:
             block = self._notion.blocks.retrieve(relation_obj['id'])
             title = block[block['type']]['title']
             print('Found relation node:', title)
-            self._graph.add_node(block['id'], title=title)
+            self._graph.add_node(block['id'], label=title)
             self._graph.add_edge(parent_page_or_database_id, block['id'])
 
     def _retrieve_mention_object_title(self, mention_obj: dict, parent_page_or_database_id: str):
         '''Example:
 
         {
             "type": "page",
@@ -291,16 +274,18 @@
         '''
         if mention_obj['type'] == 'page':
             block = self._notion.blocks.retrieve(
                 mention_obj[mention_obj['type']]['id'])
 
             title = block[block['type']]['title']
             print('Found mention node:', title)
-            self._graph.add_node(block['id'], title=title)
+            self._graph.add_node(block['id'], label=title)
             self._graph.add_edge(parent_page_or_database_id, block['id'])
 
     def _retrieve_page_or_database_title(self, page_or_database_id: str, parent_page_or_database_id: str):
         block = self._notion.blocks.retrieve(page_or_database_id)
         title = block[block['type']]['title']
         print('Found node:', title)
-        self._graph.add_node(page_or_database_id, title=title)
-        self._graph.add_edge(parent_page_or_database_id, page_or_database_id)
+        self._graph.add_node(page_or_database_id, label=title)
+        if not is_same_block_id(page_or_database_id, parent_page_or_database_id):
+            self._graph.add_edge(
+                parent_page_or_database_id, page_or_database_id)
```

### Comparing `notion-graph-0.1.4/PKG-INFO` & `notion-graph-0.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: notion-graph
-Version: 0.1.4
+Version: 0.2.0
 Summary: Generate a roam research like network graph view from your Notion pages.
 License: MIT
 Author-email: Steve Sun <sund.chn@gmail.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 ![](images/snap.png)
@@ -43,25 +43,25 @@
 ```shell
 python -m notion_graph -p <Page ID> -t <Integration Token> -o <PNG file path to export>
 ```
 
 For instance,
 
 ```shell
-python -m notion_graph -p 856391c93ae64bd1b7ebf699ca0cd861 -t secret_b8p7uLp3j3n95IDgofC9GviXP111Skx6NOt2d20U8e -o ./graph_out.png
+python -m notion_graph -p 856391c93ae64bd1b7ebf699ca0cd861 -t secret_b8p7uLp3j3n95IDgofC9GviXP111Skx6NOt2d20U8e -o ./graph_out.html
 ```
 
-`graph_out.png` would be generated at your specific path.
+`graph_out.html` would be generated at your specific path.
 
 ### Specific Font Family
 
 Matplotlib by default does not support displaying Unicode characters. To resolve this issue, specify your local font family by using `-f`:
 
 ```shell
-python -m notion_graph -p 856391c93ae64bd1b7ebf699ca0cd861 -t secret_b8p7uLp3j3n95IDgofC9GviXP111Skx6NOt2d20U8e -o ./graph_out.png -f 'SimSun'
+python -m notion_graph -p 856391c93ae64bd1b7ebf699ca0cd861 -t secret_b8p7uLp3j3n95IDgofC9GviXP111Skx6NOt2d20U8e -o ./graph_out.html -f 'SimSun'
 ```
 
 ### Importing as a Python Library
 
 You can also import `notion_graph` as a library.
 
 For instance, drawing your own diagram by [matplotlib](https://matplotlib.org/).
@@ -103,15 +103,15 @@
 brew install pdm
 pdm install
 ```
 
 Running the project by:
 
 ```shell
-pdm run start -p <page_id> -t <notion_token> -o ./graph_out.png
+pdm run start -p <page_id> -t <notion_token> -o ./graph_out.html
 ```
 
 ## 🔗 Supported Links
 
 |                    | database | page |
 | ------------------ | -------- | ---- |
 | paragraph          | ✔️       | ✔️   |
```

