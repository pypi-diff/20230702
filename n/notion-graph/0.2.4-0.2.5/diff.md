# Comparing `tmp/notion-graph-0.2.4.tar.gz` & `tmp/notion-graph-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "notion-graph-0.2.4.tar", last modified: Sun Jul  2 09:42:12 2023, max compression
+gzip compressed data, was "notion-graph-0.2.5.tar", last modified: Sun Jul  2 11:55:38 2023, max compression
```

## Comparing `notion-graph-0.2.4.tar` & `notion-graph-0.2.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1066 2023-05-02 02:00:02.124145 notion-graph-0.2.4/LICENSE
--rw-r--r--   0        0        0     3435 2023-07-02 09:38:08.986188 notion-graph-0.2.4/README.md
--rw-r--r--   0        0        0      636 2023-07-02 08:41:31.147282 notion-graph-0.2.4/notion_graph/__init__.py
--rw-r--r--   0        0        0       61 2023-01-23 09:07:31.524157 notion-graph-0.2.4/notion_graph/__main__.py
--rw-r--r--   0        0        0      641 2023-07-02 08:22:59.337641 notion-graph-0.2.4/notion_graph/cli.py
--rw-r--r--   0        0        0      426 2023-07-02 07:53:07.888215 notion-graph-0.2.4/notion_graph/helper.py
--rw-r--r--   0        0        0    11160 2023-07-02 09:41:23.606129 notion-graph-0.2.4/notion_graph/parser.py
--rw-r--r--   0        0        0      497 2023-07-02 09:41:48.616120 notion-graph-0.2.4/pyproject.toml
--rw-r--r--   0        0        0     3696 1970-01-01 00:00:00.000000 notion-graph-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-05-02 02:00:02.124145 notion-graph-0.2.5/LICENSE
+-rw-r--r--   0        0        0     3451 2023-07-02 11:40:22.213830 notion-graph-0.2.5/README.md
+-rw-r--r--   0        0        0      636 2023-07-02 09:44:33.956068 notion-graph-0.2.5/notion_graph/__init__.py
+-rw-r--r--   0        0        0       61 2023-01-23 09:07:31.524157 notion-graph-0.2.5/notion_graph/__main__.py
+-rw-r--r--   0        0        0      641 2023-07-02 09:44:33.956068 notion-graph-0.2.5/notion_graph/cli.py
+-rw-r--r--   0        0        0      426 2023-07-02 09:44:33.956068 notion-graph-0.2.5/notion_graph/helper.py
+-rw-r--r--   0        0        0    12242 2023-07-02 11:55:19.633539 notion-graph-0.2.5/notion_graph/parser.py
+-rw-r--r--   0        0        0      497 2023-07-02 11:53:13.083580 notion-graph-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0     3712 1970-01-01 00:00:00.000000 notion-graph-0.2.5/PKG-INFO
```

### Comparing `notion-graph-0.2.4/LICENSE` & `notion-graph-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `notion-graph-0.2.4/README.md` & `notion-graph-0.2.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+Metadata-Version: 2.1
+Name: notion-graph
+Version: 0.2.5
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
@@ -94,13 +103,14 @@
 | child_database     | ✔️       | ✔️   |
 | embed              |          |      |
 | callout            | ✔️       | ✔️   |
 | quote              | ✔️       | ✔️   |
 | heading_1          | ✔️       | ✔️   |
 | heading_2          | ✔️       | ✔️   |
 | heading_3          | ✔️       | ✔️   |
-| column             |          |      |
-| column_list        |          |      |
+| column             | ✔️       | ✔️   |
+| column_list        | ✔️       | ✔️   |
 | synced_block       |          |      |
 | link_to_page       |          |      |
 | table              | ✔️       | ✔️   |
 | table_row          | ✔️       | ✔️   |
+
```

### Comparing `notion-graph-0.2.4/notion_graph/__init__.py` & `notion-graph-0.2.5/notion_graph/__init__.py`

 * *Files identical despite different names*

### Comparing `notion-graph-0.2.4/notion_graph/cli.py` & `notion-graph-0.2.5/notion_graph/cli.py`

 * *Files identical despite different names*

### Comparing `notion-graph-0.2.4/notion_graph/parser.py` & `notion-graph-0.2.5/notion_graph/parser.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,26 +4,28 @@
 block -> children_page, children_database, rich_text object, cells object, children blocks
 databse -> title, pages
 page -> title, property objects
 property object -> relation object | mention object
 rich_text | title -> mention objects
 relation object -> page titles
 mention object -> database title | page title
+column_list -> column -> block
+table -> table_row -> block
 '''
 
-from notion_client import Client
+from notion_client import Client, APIResponseError
 from pyvis.network import Network
 from .helper import contains_mention_or_relation_type, is_same_block_id
 
 __all__ = ["Parser"]
 
 # All heading blocks("heading_1", "heading_2", and "heading_3") support children when the is_toggleable property is true.
 SUPPORTED_BLOCK_TYPES = [
     "paragraph", "bulleted_list_item", "numbered_list_item", "toggle", "to_do", "quote", "callout",
-    "column", "child_page", "child_database", "table", "table_row", "heading_1", "heading_2",  "heading_3"
+    "column_list", "column", "child_page", "child_database", "table", "table_row", "heading_1", "heading_2",  "heading_3"
 ]
 
 SUPPORTED_PAGE_PROPERTY_TYPES = [
     "relation", "rich_text", "title"
 ]
 
 
@@ -39,37 +41,46 @@
                               )
 
     def parse(self, root_id: str) -> Network:
         self._parse_block(root_id)
         return self._graph
 
     def export_to_html(self, file_path: str):
-        print('Graph is generated at:', file_path)
+        print('Graph is generated at:', file_path, end='\r', flush=True)
         self._graph.repulsion(node_distance=200, spring_length=200)
         self._graph.show(file_path)
 
     def _parse_block(self, root_id: str, obj: dict = None) -> None:
         if obj is None:
-            obj = self._notion.blocks.retrieve(root_id)
+            try:
+                obj = self._notion.blocks.retrieve(root_id)
+            except APIResponseError:
+                return
 
         self._parse_block_object(obj, root_id)
 
     def _parse_database(self, id: str, obj: dict = None, parent_page_or_database_id: str = None) -> None:
         if obj is None:
-            obj = self._notion.databases.retrieve(id)
+            try:
+                obj = self._notion.databases.retrieve(id)
+            except APIResponseError:
+                return
 
         if obj['archived']:
             return
 
         self._retrieve_page_or_database_title(id, parent_page_or_database_id)
         self._parse_database_pages(id)
 
     def _parse_page(self, id: str, obj: dict = None, parent_page_or_database_id: str = None) -> None:
         if obj is None:
-            obj = self._notion.pages.retrieve(id)
+            try:
+                obj = self._notion.pages.retrieve(id)
+            except APIResponseError:
+                return
 
         if obj['archived']:
             return
 
         self._retrieve_page_or_database_title(id, parent_page_or_database_id)
         self._parse_page_properties(obj['properties'], id)
 
@@ -149,23 +160,30 @@
 
         if obj['type'] == 'child_page':
             self._parse_page(obj['id'], None, parent_page_or_database_id)
             if obj['has_children']:
                 self._parse_block_children(obj['id'], obj['id'])
             return
 
+        # column_list -> column -> block
+        if obj['type'] == 'column_list' or obj['type'] == 'column':
+            if obj['has_children']:
+                self._parse_block_children(
+                    obj['id'], parent_page_or_database_id)
+            return
+
         obj_value = obj[obj['type']]
         # For the supported types with rich_text
         rich_text_list = obj_value.get(
             'rich_text', None)
         if rich_text_list:
             self._parse_rich_text_list(
                 rich_text_list, parent_page_or_database_id)
 
-        # For table -> table_row -> cells
+        # table -> table_row -> cells
         cells_metrics = obj_value.get('cells', None)
         if cells_metrics:
             self._parse_cells_metrics(
                 cells_metrics, parent_page_or_database_id)
 
         if obj.get('is_toggleable', False) or obj.get('has_children', False):
             self._parse_block_children(obj['id'], parent_page_or_database_id)
@@ -190,24 +208,32 @@
                 self._parse_rich_text_list(
                     i[i['type']], parent_page_or_database_id)
 
     def _parse_database_pages(self, database_id: str) -> None:
         has_more = True
         next_cursor = None
         while has_more:
-            data = self._notion.databases.query(
-                database_id, page_size=100, start_cursor=next_cursor)
+            try:
+                data = self._notion.databases.query(
+                    database_id, page_size=100, start_cursor=next_cursor)
+            except APIResponseError:
+                return
+
             pages = data['results']
             has_more = data['has_more']
             next_cursor = data['next_cursor']
             for page in pages:
                 self._parse_page(page['id'], None, database_id)
 
     def _parse_block_children(self, block_id: str, parent_page_or_database_id: str) -> None:
-        list_object = self._notion.blocks.children.list(block_id)
+        try:
+            list_object = self._notion.blocks.children.list(block_id)
+        except APIResponseError:
+            return
+
         block_list = list_object['results']
 
         for block in block_list:
             self._parse_block_object(block, parent_page_or_database_id)
 
     def _parse_cells_metrics(self, cells_metrics: list, parent_page_or_database_id: str) -> None:
         for row_cells in cells_metrics:
@@ -252,40 +278,51 @@
         [
             {
                 "id": "7d2d2701-5f09-48af-a1c5-d0b17b160a8a"
             }
         ]
         '''
         for relation_obj in relation_list:
-            block = self._notion.blocks.retrieve(relation_obj['id'])
+            try:
+                block = self._notion.blocks.retrieve(relation_obj['id'])
+            except APIResponseError:
+                continue
+
             title = block[block['type']]['title']
-            print('Found relation node:', title)
+            print('Found relation node:', title, end='\r', flush=True)
             self._graph.add_node(block['id'], label=title)
             self._graph.add_edge(parent_page_or_database_id, block['id'])
 
     def _retrieve_mention_object_title(self, mention_obj: dict, parent_page_or_database_id: str):
         '''Example:
 
         {
             "type": "page",
             "page": {
                 "id": "960ce6bd-eeb8-4674-bf79-996ff40e14f8"
             }
         }
         '''
         if mention_obj['type'] == 'page':
-            block = self._notion.blocks.retrieve(
-                mention_obj[mention_obj['type']]['id'])
+            try:
+                block = self._notion.blocks.retrieve(
+                    mention_obj[mention_obj['type']]['id'])
+            except APIResponseError:
+                return
 
             title = block[block['type']]['title']
-            print('Found mention node:', title)
+            print('Found mention node:', title, end='\r', flush=True)
             self._graph.add_node(block['id'], label=title)
             self._graph.add_edge(parent_page_or_database_id, block['id'])
 
     def _retrieve_page_or_database_title(self, page_or_database_id: str, parent_page_or_database_id: str):
-        block = self._notion.blocks.retrieve(page_or_database_id)
+        try:
+            block = self._notion.blocks.retrieve(page_or_database_id)
+        except APIResponseError:
+            return
+
         title = block[block['type']]['title']
-        print('Found node:', title)
+        print('Found node:', title, end='\r', flush=True)
         self._graph.add_node(page_or_database_id, label=title)
         if not is_same_block_id(page_or_database_id, parent_page_or_database_id):
             self._graph.add_edge(
                 parent_page_or_database_id, page_or_database_id)
```

### Comparing `notion-graph-0.2.4/PKG-INFO` & `notion-graph-0.2.5/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,7 @@
-Metadata-Version: 2.1
-Name: notion-graph
-Version: 0.2.4
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
@@ -103,14 +94,13 @@
 | child_database     | ✔️       | ✔️   |
 | embed              |          |      |
 | callout            | ✔️       | ✔️   |
 | quote              | ✔️       | ✔️   |
 | heading_1          | ✔️       | ✔️   |
 | heading_2          | ✔️       | ✔️   |
 | heading_3          | ✔️       | ✔️   |
-| column             |          |      |
-| column_list        |          |      |
+| column             | ✔️       | ✔️   |
+| column_list        | ✔️       | ✔️   |
 | synced_block       |          |      |
 | link_to_page       |          |      |
 | table              | ✔️       | ✔️   |
 | table_row          | ✔️       | ✔️   |
-
```

