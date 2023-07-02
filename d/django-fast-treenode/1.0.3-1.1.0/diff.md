# Comparing `tmp/django-fast-treenode-1.0.3.tar.gz` & `tmp/django-fast-treenode-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-fast-treenode-1.0.3.tar", last modified: Wed Jun 28 09:32:50 2023, max compression
+gzip compressed data, was "django-fast-treenode-1.1.0.tar", last modified: Sun Jul  2 16:52:45 2023, max compression
```

## Comparing `django-fast-treenode-1.0.3.tar` & `django-fast-treenode-1.1.0.tar`

### file list

```diff
@@ -1,50 +1,51 @@
-drwxrwxrwx   0        0        0        0 2023-06-28 09:32:50.000000 django-fast-treenode-1.0.3/
--rw-rw-rw-   0        0        0     1091 2023-06-28 08:53:50.000000 django-fast-treenode-1.0.3/LICENSE
--rw-rw-rw-   0        0        0      147 2023-06-01 20:20:34.000000 django-fast-treenode-1.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0    17715 2023-06-28 09:32:52.000000 django-fast-treenode-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0    16805 2023-06-01 20:22:12.000000 django-fast-treenode-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-28 09:32:50.000000 django-fast-treenode-1.0.3/django_fast_treenode.egg-info/
--rw-rw-rw-   0        0        0    17715 2023-06-28 09:32:50.000000 django-fast-treenode-1.0.3/django_fast_treenode.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1062 2023-06-28 09:32:50.000000 django-fast-treenode-1.0.3/django_fast_treenode.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-28 09:32:50.000000 django-fast-treenode-1.0.3/django_fast_treenode.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-06-28 09:32:50.000000 django-fast-treenode-1.0.3/django_fast_treenode.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-28 09:32:50.000000 django-fast-treenode-1.0.3/django_fast_treenode.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       90 2023-05-31 11:15:42.000000 django-fast-treenode-1.0.3/pyproject.toml
--rw-rw-rw-   0        0        0      935 2023-06-28 09:32:52.000000 django-fast-treenode-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0       39 2023-05-31 11:20:32.000000 django-fast-treenode-1.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-28 09:32:50.000000 django-fast-treenode-1.0.3/treenode/
--rw-rw-rw-   0        0        0      171 2022-01-20 08:49:18.000000 django-fast-treenode-1.0.3/treenode/__init__.py
--rw-rw-rw-   0        0        0     5857 2022-02-12 08:55:00.000000 django-fast-treenode-1.0.3/treenode/admin.py
--rw-rw-rw-   0        0        0      154 2022-01-18 11:38:14.000000 django-fast-treenode-1.0.3/treenode/apps.py
--rw-rw-rw-   0        0        0      185 2022-01-16 20:42:14.000000 django-fast-treenode-1.0.3/treenode/compat.py
-drwxrwxrwx   0        0        0        0 2023-06-28 09:32:50.000000 django-fast-treenode-1.0.3/treenode/docs/
--rw-rw-rw-   0        0        0    16716 2023-05-31 12:12:12.000000 django-fast-treenode-1.0.3/treenode/docs/README.txt
--rw-rw-rw-   0        0        0     1942 2022-01-22 19:52:32.000000 django-fast-treenode-1.0.3/treenode/factory.py
--rw-rw-rw-   0        0        0      907 2022-02-11 19:19:44.000000 django-fast-treenode-1.0.3/treenode/forms.py
--rw-rw-rw-   0        0        0     1590 2022-02-11 16:45:34.000000 django-fast-treenode-1.0.3/treenode/managers.py
--rw-rw-rw-   0        0        0    20048 2023-06-28 08:50:54.000000 django-fast-treenode-1.0.3/treenode/models.py
-drwxrwxrwx   0        0        0        0 2023-06-28 09:32:50.000000 django-fast-treenode-1.0.3/treenode/static/
--rw-rw-rw-   0        0        0        0 2022-02-17 13:47:48.000000 django-fast-treenode-1.0.3/treenode/static/.gitkeep
-drwxrwxrwx   0        0        0        0 2023-06-28 09:32:50.000000 django-fast-treenode-1.0.3/treenode/static/select2tree/
--rw-rw-rw-   0        0        0        0 2022-02-17 13:47:48.000000 django-fast-treenode-1.0.3/treenode/static/select2tree/.gitkeep
--rw-rw-rw-   0        0        0     4234 2022-01-23 15:49:16.000000 django-fast-treenode-1.0.3/treenode/static/select2tree/select2tree.css
--rw-rw-rw-   0        0        0     5948 2022-01-23 15:13:46.000000 django-fast-treenode-1.0.3/treenode/static/select2tree/select2tree.js
-drwxrwxrwx   0        0        0        0 2023-06-28 09:32:50.000000 django-fast-treenode-1.0.3/treenode/static/treenode/
--rw-rw-rw-   0        0        0        0 2022-02-17 13:47:48.000000 django-fast-treenode-1.0.3/treenode/static/treenode/.gitkeep
-drwxrwxrwx   0        0        0        0 2023-06-28 09:32:50.000000 django-fast-treenode-1.0.3/treenode/static/treenode/css/
--rw-rw-rw-   0        0        0        0 2022-02-17 13:47:48.000000 django-fast-treenode-1.0.3/treenode/static/treenode/css/.gitkeep
--rw-rw-rw-   0        0        0     1637 2022-01-16 20:42:14.000000 django-fast-treenode-1.0.3/treenode/static/treenode/css/treenode.css
-drwxrwxrwx   0        0        0        0 2023-06-28 09:32:50.000000 django-fast-treenode-1.0.3/treenode/static/treenode/js/
--rw-rw-rw-   0        0        0        0 2022-02-17 13:47:48.000000 django-fast-treenode-1.0.3/treenode/static/treenode/js/.gitkeep
--rw-rw-rw-   0        0        0     7797 2022-01-21 17:23:48.000000 django-fast-treenode-1.0.3/treenode/static/treenode/js/treenode.js
-drwxrwxrwx   0        0        0        0 2023-06-28 09:32:50.000000 django-fast-treenode-1.0.3/treenode/templates/
--rw-rw-rw-   0        0        0        0 2022-02-17 13:47:48.000000 django-fast-treenode-1.0.3/treenode/templates/.gitkeep
-drwxrwxrwx   0        0        0        0 2023-06-28 09:32:50.000000 django-fast-treenode-1.0.3/treenode/templates/widgets/
--rw-rw-rw-   0        0        0        0 2022-02-17 13:47:48.000000 django-fast-treenode-1.0.3/treenode/templates/widgets/.gitkeep
--rw-rw-rw-   0        0        0      217 2021-12-13 08:39:40.000000 django-fast-treenode-1.0.3/treenode/templates/widgets/attrs.html
--rw-rw-rw-   0        0        0      288 2021-12-13 08:37:06.000000 django-fast-treenode-1.0.3/treenode/templates/widgets/options.html
--rw-rw-rw-   0        0        0      675 2022-01-22 16:59:06.000000 django-fast-treenode-1.0.3/treenode/templates/widgets/select2tree.html
--rw-rw-rw-   0        0        0       63 2022-01-18 11:38:14.000000 django-fast-treenode-1.0.3/treenode/tests.py
--rw-rw-rw-   0        0        0       50 2022-01-23 14:09:38.000000 django-fast-treenode-1.0.3/treenode/version.py
--rw-rw-rw-   0        0        0       66 2022-02-10 10:11:48.000000 django-fast-treenode-1.0.3/treenode/views.py
--rw-rw-rw-   0        0        0     1189 2022-01-28 12:26:52.000000 django-fast-treenode-1.0.3/treenode/widgets.py
+drwxrwxrwx   0        0        0        0 2023-07-02 16:52:44.000000 django-fast-treenode-1.1.0/
+-rw-rw-rw-   0        0        0     1091 2023-06-28 08:53:50.000000 django-fast-treenode-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0      146 2023-07-02 16:40:36.000000 django-fast-treenode-1.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0    17051 2023-07-02 16:52:46.000000 django-fast-treenode-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0    16141 2023-07-02 16:37:32.000000 django-fast-treenode-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-02 16:52:44.000000 django-fast-treenode-1.1.0/django_fast_treenode.egg-info/
+-rw-rw-rw-   0        0        0    17051 2023-07-02 16:52:44.000000 django-fast-treenode-1.1.0/django_fast_treenode.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1088 2023-07-02 16:52:44.000000 django-fast-treenode-1.1.0/django_fast_treenode.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-02 16:52:44.000000 django-fast-treenode-1.1.0/django_fast_treenode.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-07-02 16:52:44.000000 django-fast-treenode-1.1.0/django_fast_treenode.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-02 16:52:44.000000 django-fast-treenode-1.1.0/django_fast_treenode.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       90 2023-05-31 11:15:42.000000 django-fast-treenode-1.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0      935 2023-07-02 16:52:46.000000 django-fast-treenode-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0       39 2023-05-31 11:20:32.000000 django-fast-treenode-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-02 16:52:44.000000 django-fast-treenode-1.1.0/treenode/
+-rw-rw-rw-   0        0        0      171 2023-07-01 02:29:18.000000 django-fast-treenode-1.1.0/treenode/__init__.py
+-rw-rw-rw-   0        0        0     5374 2023-07-02 11:48:12.000000 django-fast-treenode-1.1.0/treenode/admin.py
+-rw-rw-rw-   0        0        0      154 2023-07-01 02:29:18.000000 django-fast-treenode-1.1.0/treenode/apps.py
+-rw-rw-rw-   0        0        0      185 2023-07-01 02:29:18.000000 django-fast-treenode-1.1.0/treenode/compat.py
+drwxrwxrwx   0        0        0        0 2023-07-02 16:52:44.000000 django-fast-treenode-1.1.0/treenode/docs/
+-rw-rw-rw-   0        0        0        1 2023-07-01 02:29:18.000000 django-fast-treenode-1.1.0/treenode/docs/.gitkeep
+-rw-rw-rw-   0        0        0    16141 2023-07-02 16:37:32.000000 django-fast-treenode-1.1.0/treenode/docs/Documentation
+-rw-rw-rw-   0        0        0     1942 2023-07-01 02:29:18.000000 django-fast-treenode-1.1.0/treenode/factory.py
+-rw-rw-rw-   0        0        0      907 2023-07-01 02:29:18.000000 django-fast-treenode-1.1.0/treenode/forms.py
+-rw-rw-rw-   0        0        0     2210 2023-07-02 11:42:06.000000 django-fast-treenode-1.1.0/treenode/managers.py
+-rw-rw-rw-   0        0        0    20653 2023-07-02 16:25:56.000000 django-fast-treenode-1.1.0/treenode/models.py
+drwxrwxrwx   0        0        0        0 2023-07-02 16:52:44.000000 django-fast-treenode-1.1.0/treenode/static/
+-rw-rw-rw-   0        0        0        0 2023-07-01 02:29:18.000000 django-fast-treenode-1.1.0/treenode/static/.gitkeep
+drwxrwxrwx   0        0        0        0 2023-07-02 16:52:44.000000 django-fast-treenode-1.1.0/treenode/static/select2tree/
+-rw-rw-rw-   0        0        0        1 2023-07-01 02:29:18.000000 django-fast-treenode-1.1.0/treenode/static/select2tree/.gitkeep
+-rw-rw-rw-   0        0        0     4234 2023-07-02 11:53:28.000000 django-fast-treenode-1.1.0/treenode/static/select2tree/select2tree.css
+-rw-rw-rw-   0        0        0     5948 2023-07-01 02:29:18.000000 django-fast-treenode-1.1.0/treenode/static/select2tree/select2tree.js
+drwxrwxrwx   0        0        0        0 2023-07-02 16:52:44.000000 django-fast-treenode-1.1.0/treenode/static/treenode/
+-rw-rw-rw-   0        0        0        1 2023-07-01 02:29:18.000000 django-fast-treenode-1.1.0/treenode/static/treenode/.gitkeep
+drwxrwxrwx   0        0        0        0 2023-07-02 16:52:44.000000 django-fast-treenode-1.1.0/treenode/static/treenode/css/
+-rw-rw-rw-   0        0        0        1 2023-07-01 02:29:18.000000 django-fast-treenode-1.1.0/treenode/static/treenode/css/.gitkeep
+-rw-rw-rw-   0        0        0     1637 2023-07-01 02:29:18.000000 django-fast-treenode-1.1.0/treenode/static/treenode/css/treenode.css
+drwxrwxrwx   0        0        0        0 2023-07-02 16:52:44.000000 django-fast-treenode-1.1.0/treenode/static/treenode/js/
+-rw-rw-rw-   0        0        0        1 2023-07-01 02:29:18.000000 django-fast-treenode-1.1.0/treenode/static/treenode/js/.gitkeep
+-rw-rw-rw-   0        0        0     7797 2023-07-01 02:29:18.000000 django-fast-treenode-1.1.0/treenode/static/treenode/js/treenode.js
+drwxrwxrwx   0        0        0        0 2023-07-02 16:52:44.000000 django-fast-treenode-1.1.0/treenode/templates/
+-rw-rw-rw-   0        0        0        1 2023-07-01 02:29:18.000000 django-fast-treenode-1.1.0/treenode/templates/.gitkeep
+drwxrwxrwx   0        0        0        0 2023-07-02 16:52:44.000000 django-fast-treenode-1.1.0/treenode/templates/widgets/
+-rw-rw-rw-   0        0        0        1 2023-07-01 02:29:18.000000 django-fast-treenode-1.1.0/treenode/templates/widgets/.gitkeep
+-rw-rw-rw-   0        0        0      217 2023-07-01 02:29:18.000000 django-fast-treenode-1.1.0/treenode/templates/widgets/attrs.html
+-rw-rw-rw-   0        0        0      288 2023-07-01 02:29:18.000000 django-fast-treenode-1.1.0/treenode/templates/widgets/options.html
+-rw-rw-rw-   0        0        0      675 2023-07-01 02:29:18.000000 django-fast-treenode-1.1.0/treenode/templates/widgets/select2tree.html
+-rw-rw-rw-   0        0        0       63 2023-07-01 02:29:18.000000 django-fast-treenode-1.1.0/treenode/tests.py
+-rw-rw-rw-   0        0        0       50 2023-07-02 16:28:58.000000 django-fast-treenode-1.1.0/treenode/version.py
+-rw-rw-rw-   0        0        0       66 2023-07-01 02:29:18.000000 django-fast-treenode-1.1.0/treenode/views.py
+-rw-rw-rw-   0        0        0     1189 2023-07-01 02:29:18.000000 django-fast-treenode-1.1.0/treenode/widgets.py
```

### Comparing `django-fast-treenode-1.0.3/LICENSE` & `django-fast-treenode-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-fast-treenode-1.0.3/PKG-INFO` & `django-fast-treenode-1.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-fast-treenode
-Version: 1.0.3
+Version: 1.1.0
 Summary: Application for supporting tree (hierarchical) data structure in Django projects
 Home-page: https://github.com/TimurKady/fast-treenode
 Author: Timur Kady
 Author-email: timurkady@yandex.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
@@ -21,23 +21,23 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Django-fast-treenode 
 __Combination of Adjacency List and Closure Table__
 
-## Features
+## Functions
 Application for supporting tree (hierarchical) data structure in Django projects
-* faster,
-* synced: in-memory model instances are automatically updated,
-* compatibility: you can easily add treenode to existing projects,
+* Faster: resource-intensive operations are cached; bulk operations are used for inserts and changes,
+* synchronized: model instances in memory are automatically updated,
+* compatibility: you can easily add a tree node to existing projects using TreeNode without changing the code,
 * no dependencies,
-* easy configuration: just extend the abstract model / model-admin,
-* admin integration: visualization options (accordion, breadcrumbs or indentation),
-* widget: build-in Select2-to-Tree extends Select2 to support arbitrary level of nesting.
+* easy setup: just extend the abstract model/model-admin,
+* admin integration: visualization options (accordion, breadcrumbs or padding),
+* widget: Built-in Select2-to-Tree extends Select2 to support arbitrary nesting levels.
 
 ## Debut idea
 This is a modification of the reusable [django-treenode](https://github.com/fabiocaccamo/django-treenode) application developed by [Fabio Caccamo](https://github.com/fabiocaccamo).
 The original application has significant advantages over other analogues, and indeed, is one of the best implementations of support for hierarchical structures for Django. 
 
 Fabio's idea was to use the Adjacency List method to store the data tree. The most probable and time-consuming requests are calculated in advance and stored in the database. Also, most requests are cached. As a result, query processing is carried out in one call to the database or without it at all.
 
@@ -177,15 +177,14 @@
 -   [`get_descendants_tree`](#get_descendants_tree)
 -   [`get_descendants_tree_display`](#get_descendants_tree_display)
 -   [`get_first_child`](#get_first_child)
 -   [`get_index`](#get_index)
 -   [`get_last_child`](#get_last_child)
 -   [`get_level`](#get_level)
 -   [`get_order`](#get_order)
--   [`get_ordered_queryset`](#get_ordered_queryset)
 -   [`get_parent`](#get_parent)
 -   [`get_parent_pk`](#get_parent_pk)
 -   [`set_parent`](#set_parent)
 -   [`get_path`](#get_path)
 -   [`get_priority`](#get_priority)
 -   [`set_priority`](#set_priority)
 -   [`get_root`](#get_root)
@@ -381,31 +380,14 @@
 Get the **order value** used for ordering:
 ```python
 obj.get_order()
 # or
 obj.order
 ```
 
-#### `get_ordered_queryset`
-Returns a queryset of nodes ordered by tn_priority each node. 
-```python
-cls.get_ordered_queryset()
-```
-For example:
-- A.1
-- A.1.1
-- A.1.1.1
-- A.1.1.2
-- A.2
-- A.2.1
-- ...
-
-This method uses a lot of memory, ```RawSQL()``` and ```.extra()``` QuerySet method. Use of this method is deprecated due to concerns that Django's ```.extra()``` method **will be deprecated in the future**. 
-Use it only if you cannot otherwise assemble an ordered tree from an Adjacency Table and a Closure Table. In most cases, the data in one Adjacency Table is sufficient for such an assembly. You can easily find the corresponding algorithms (two-pass and one-pass) on the Internet.
-
 #### `get_parent`
 Get the **parent node**:
 ```python
 obj.get_parent()
 # or
 obj.parent
 ```
@@ -599,16 +581,15 @@
 *  [django-treenode](https://github.com/fabiocaccamo/django-treenode) by [Fabio Caccamo](https://github.com/fabiocaccamo);
 *  [Select2-to-Tree](https://github.com/clivezhg/select2-to-tree) Select2 extension by [clivezhg](https://github.com/clivezhg)
 
 Special thanks to [Mathieu Leplatre](https://blog.mathieu-leplatre.info/pages/about.html) for the advice used in writing this application
 
 ## To do
 Future plans:
-* drug-and-drop support;
-* may be will restore caching;
 * may be will add the ability to determine the priority of the parent by any field, for example, by creation date or alphabetical order;
+* drug-and-drop support;
 * to be happy, to don't worry, until die.
 
 
 Your wishes, objections, comments are welcome.
```

### Comparing `django-fast-treenode-1.0.3/README.md` & `django-fast-treenode-1.1.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # Django-fast-treenode 
 __Combination of Adjacency List and Closure Table__
 
-## Features
+## Functions
 Application for supporting tree (hierarchical) data structure in Django projects
-* faster,
-* synced: in-memory model instances are automatically updated,
-* compatibility: you can easily add treenode to existing projects,
+* Faster: resource-intensive operations are cached; bulk operations are used for inserts and changes,
+* synchronized: model instances in memory are automatically updated,
+* compatibility: you can easily add a tree node to existing projects using TreeNode without changing the code,
 * no dependencies,
-* easy configuration: just extend the abstract model / model-admin,
-* admin integration: visualization options (accordion, breadcrumbs or indentation),
-* widget: build-in Select2-to-Tree extends Select2 to support arbitrary level of nesting.
+* easy setup: just extend the abstract model/model-admin,
+* admin integration: visualization options (accordion, breadcrumbs or padding),
+* widget: Built-in Select2-to-Tree extends Select2 to support arbitrary nesting levels.
 
 ## Debut idea
 This is a modification of the reusable [django-treenode](https://github.com/fabiocaccamo/django-treenode) application developed by [Fabio Caccamo](https://github.com/fabiocaccamo).
 The original application has significant advantages over other analogues, and indeed, is one of the best implementations of support for hierarchical structures for Django. 
 
 Fabio's idea was to use the Adjacency List method to store the data tree. The most probable and time-consuming requests are calculated in advance and stored in the database. Also, most requests are cached. As a result, query processing is carried out in one call to the database or without it at all.
 
@@ -153,15 +153,14 @@
 -   [`get_descendants_tree`](#get_descendants_tree)
 -   [`get_descendants_tree_display`](#get_descendants_tree_display)
 -   [`get_first_child`](#get_first_child)
 -   [`get_index`](#get_index)
 -   [`get_last_child`](#get_last_child)
 -   [`get_level`](#get_level)
 -   [`get_order`](#get_order)
--   [`get_ordered_queryset`](#get_ordered_queryset)
 -   [`get_parent`](#get_parent)
 -   [`get_parent_pk`](#get_parent_pk)
 -   [`set_parent`](#set_parent)
 -   [`get_path`](#get_path)
 -   [`get_priority`](#get_priority)
 -   [`set_priority`](#set_priority)
 -   [`get_root`](#get_root)
@@ -357,31 +356,14 @@
 Get the **order value** used for ordering:
 ```python
 obj.get_order()
 # or
 obj.order
 ```
 
-#### `get_ordered_queryset`
-Returns a queryset of nodes ordered by tn_priority each node. 
-```python
-cls.get_ordered_queryset()
-```
-For example:
-- A.1
-- A.1.1
-- A.1.1.1
-- A.1.1.2
-- A.2
-- A.2.1
-- ...
-
-This method uses a lot of memory, ```RawSQL()``` and ```.extra()``` QuerySet method. Use of this method is deprecated due to concerns that Django's ```.extra()``` method **will be deprecated in the future**. 
-Use it only if you cannot otherwise assemble an ordered tree from an Adjacency Table and a Closure Table. In most cases, the data in one Adjacency Table is sufficient for such an assembly. You can easily find the corresponding algorithms (two-pass and one-pass) on the Internet.
-
 #### `get_parent`
 Get the **parent node**:
 ```python
 obj.get_parent()
 # or
 obj.parent
 ```
@@ -575,14 +557,13 @@
 *  [django-treenode](https://github.com/fabiocaccamo/django-treenode) by [Fabio Caccamo](https://github.com/fabiocaccamo);
 *  [Select2-to-Tree](https://github.com/clivezhg/select2-to-tree) Select2 extension by [clivezhg](https://github.com/clivezhg)
 
 Special thanks to [Mathieu Leplatre](https://blog.mathieu-leplatre.info/pages/about.html) for the advice used in writing this application
 
 ## To do
 Future plans:
-* drug-and-drop support;
-* may be will restore caching;
 * may be will add the ability to determine the priority of the parent by any field, for example, by creation date or alphabetical order;
+* drug-and-drop support;
 * to be happy, to don't worry, until die.
 
 
 Your wishes, objections, comments are welcome.
```

### Comparing `django-fast-treenode-1.0.3/django_fast_treenode.egg-info/PKG-INFO` & `django-fast-treenode-1.1.0/django_fast_treenode.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-fast-treenode
-Version: 1.0.3
+Version: 1.1.0
 Summary: Application for supporting tree (hierarchical) data structure in Django projects
 Home-page: https://github.com/TimurKady/fast-treenode
 Author: Timur Kady
 Author-email: timurkady@yandex.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
@@ -21,23 +21,23 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Django-fast-treenode 
 __Combination of Adjacency List and Closure Table__
 
-## Features
+## Functions
 Application for supporting tree (hierarchical) data structure in Django projects
-* faster,
-* synced: in-memory model instances are automatically updated,
-* compatibility: you can easily add treenode to existing projects,
+* Faster: resource-intensive operations are cached; bulk operations are used for inserts and changes,
+* synchronized: model instances in memory are automatically updated,
+* compatibility: you can easily add a tree node to existing projects using TreeNode without changing the code,
 * no dependencies,
-* easy configuration: just extend the abstract model / model-admin,
-* admin integration: visualization options (accordion, breadcrumbs or indentation),
-* widget: build-in Select2-to-Tree extends Select2 to support arbitrary level of nesting.
+* easy setup: just extend the abstract model/model-admin,
+* admin integration: visualization options (accordion, breadcrumbs or padding),
+* widget: Built-in Select2-to-Tree extends Select2 to support arbitrary nesting levels.
 
 ## Debut idea
 This is a modification of the reusable [django-treenode](https://github.com/fabiocaccamo/django-treenode) application developed by [Fabio Caccamo](https://github.com/fabiocaccamo).
 The original application has significant advantages over other analogues, and indeed, is one of the best implementations of support for hierarchical structures for Django. 
 
 Fabio's idea was to use the Adjacency List method to store the data tree. The most probable and time-consuming requests are calculated in advance and stored in the database. Also, most requests are cached. As a result, query processing is carried out in one call to the database or without it at all.
 
@@ -177,15 +177,14 @@
 -   [`get_descendants_tree`](#get_descendants_tree)
 -   [`get_descendants_tree_display`](#get_descendants_tree_display)
 -   [`get_first_child`](#get_first_child)
 -   [`get_index`](#get_index)
 -   [`get_last_child`](#get_last_child)
 -   [`get_level`](#get_level)
 -   [`get_order`](#get_order)
--   [`get_ordered_queryset`](#get_ordered_queryset)
 -   [`get_parent`](#get_parent)
 -   [`get_parent_pk`](#get_parent_pk)
 -   [`set_parent`](#set_parent)
 -   [`get_path`](#get_path)
 -   [`get_priority`](#get_priority)
 -   [`set_priority`](#set_priority)
 -   [`get_root`](#get_root)
@@ -381,31 +380,14 @@
 Get the **order value** used for ordering:
 ```python
 obj.get_order()
 # or
 obj.order
 ```
 
-#### `get_ordered_queryset`
-Returns a queryset of nodes ordered by tn_priority each node. 
-```python
-cls.get_ordered_queryset()
-```
-For example:
-- A.1
-- A.1.1
-- A.1.1.1
-- A.1.1.2
-- A.2
-- A.2.1
-- ...
-
-This method uses a lot of memory, ```RawSQL()``` and ```.extra()``` QuerySet method. Use of this method is deprecated due to concerns that Django's ```.extra()``` method **will be deprecated in the future**. 
-Use it only if you cannot otherwise assemble an ordered tree from an Adjacency Table and a Closure Table. In most cases, the data in one Adjacency Table is sufficient for such an assembly. You can easily find the corresponding algorithms (two-pass and one-pass) on the Internet.
-
 #### `get_parent`
 Get the **parent node**:
 ```python
 obj.get_parent()
 # or
 obj.parent
 ```
@@ -599,16 +581,15 @@
 *  [django-treenode](https://github.com/fabiocaccamo/django-treenode) by [Fabio Caccamo](https://github.com/fabiocaccamo);
 *  [Select2-to-Tree](https://github.com/clivezhg/select2-to-tree) Select2 extension by [clivezhg](https://github.com/clivezhg)
 
 Special thanks to [Mathieu Leplatre](https://blog.mathieu-leplatre.info/pages/about.html) for the advice used in writing this application
 
 ## To do
 Future plans:
-* drug-and-drop support;
-* may be will restore caching;
 * may be will add the ability to determine the priority of the parent by any field, for example, by creation date or alphabetical order;
+* drug-and-drop support;
 * to be happy, to don't worry, until die.
 
 
 Your wishes, objections, comments are welcome.
```

### Comparing `django-fast-treenode-1.0.3/django_fast_treenode.egg-info/SOURCES.txt` & `django-fast-treenode-1.1.0/django_fast_treenode.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -17,15 +17,16 @@
 treenode/forms.py
 treenode/managers.py
 treenode/models.py
 treenode/tests.py
 treenode/version.py
 treenode/views.py
 treenode/widgets.py
-treenode/docs/README.txt
+treenode/docs/.gitkeep
+treenode/docs/Documentation
 treenode/static/.gitkeep
 treenode/static/select2tree/.gitkeep
 treenode/static/select2tree/select2tree.css
 treenode/static/select2tree/select2tree.js
 treenode/static/treenode/.gitkeep
 treenode/static/treenode/css/.gitkeep
 treenode/static/treenode/css/treenode.css
```

### Comparing `django-fast-treenode-1.0.3/setup.cfg` & `django-fast-treenode-1.1.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 00000000: 5b65 6767 5f69 6e66 6f5d 0d0a 7461 675f  [egg_info]..tag_
 00000010: 6275 696c 6420 3d20 0d0a 7461 675f 6461  build = ..tag_da
 00000020: 7465 203d 2030 0d0a 0d0a 5b6d 6574 6164  te = 0....[metad
 00000030: 6174 615d 0d0a 6e61 6d65 203d 2064 6a61  ata]..name = dja
 00000040: 6e67 6f2d 6661 7374 2d74 7265 656e 6f64  ngo-fast-treenod
-00000050: 650d 0a76 6572 7369 6f6e 203d 2031 2e30  e..version = 1.0
-00000060: 2e33 0d0a 6465 7363 7269 7074 696f 6e20  .3..description 
+00000050: 650d 0a76 6572 7369 6f6e 203d 2031 2e31  e..version = 1.1
+00000060: 2e30 0d0a 6465 7363 7269 7074 696f 6e20  .0..description 
 00000070: 3d20 4170 706c 6963 6174 696f 6e20 666f  = Application fo
 00000080: 7220 7375 7070 6f72 7469 6e67 2074 7265  r supporting tre
 00000090: 6520 2868 6965 7261 7263 6869 6361 6c29  e (hierarchical)
 000000a0: 2064 6174 6120 7374 7275 6374 7572 6520   data structure 
 000000b0: 696e 2044 6a61 6e67 6f20 7072 6f6a 6563  in Django projec
 000000c0: 7473 0d0a 6c6f 6e67 5f64 6573 6372 6970  ts..long_descrip
 000000d0: 7469 6f6e 5f63 6f6e 7465 6e74 5f74 7970  tion_content_typ
```

### Comparing `django-fast-treenode-1.0.3/treenode/admin.py` & `django-fast-treenode-1.1.0/treenode/admin.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,28 +14,16 @@
     def get_ordering(self, request, queryset):
         rv = super().get_ordering(request, queryset)
         rv = list(rv)
         rv.remove('-pk') if '-pk' in rv else None
         return tuple()
 
     def get_queryset(self, request):
-        qs = super().get_queryset(request)
-        order = sorted([node for node in qs], key=lambda x: x.tn_order)
-        pk_list = [node.pk for node in order]
-
-        table = self.model._meta.db_table
-        clauses = ' '.join(
-            ['WHEN %s.id=%s THEN %s' % (table, pk, i)
-             for i, pk in enumerate(pk_list)]
-        )
-        order = 'CASE %s END' % clauses
-        queryset = self.model.objects.filter(pk__in=pk_list).extra(
-            select={'ordering': order}, order_by=('ordering',))
-
-        return queryset.select_related('tn_parent')
+        qs = self.model.objects.all()
+        return qs.select_related('tn_parent')
 
 
 class TreeNodeModelAdmin(admin.ModelAdmin):
 
     TREENODE_DISPLAY_MODE_ACCORDION = 'accordion'
     TREENODE_DISPLAY_MODE_BREADCRUMBS = 'breadcrumbs'
     TREENODE_DISPLAY_MODE_INDENTATION = 'indentation'
```

### Comparing `django-fast-treenode-1.0.3/treenode/docs/README.txt` & `django-fast-treenode-1.1.0/treenode/docs/Documentation`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,19 @@
-# Django Fast Treenode 
+# Django-fast-treenode 
 __Combination of Adjacency List and Closure Table__
 
-## Features
-* faster,
-* synced: in-memory model instances are automatically updated,
-* compatibility: you can easily add treenode to existing projects,
+## Functions
+Application for supporting tree (hierarchical) data structure in Django projects
+* Faster: resource-intensive operations are cached; bulk operations are used for inserts and changes,
+* synchronized: model instances in memory are automatically updated,
+* compatibility: you can easily add a tree node to existing projects using TreeNode without changing the code,
 * no dependencies,
-* easy configuration: just extend the abstract model / model-admin,
-* admin integration: visualization options (accordion, breadcrumbs or indentation),
-* widget: build-in Select2-to-Tree extends Select2 to support arbitrary level of nesting.
+* easy setup: just extend the abstract model/model-admin,
+* admin integration: visualization options (accordion, breadcrumbs or padding),
+* widget: Built-in Select2-to-Tree extends Select2 to support arbitrary nesting levels.
 
 ## Debut idea
 This is a modification of the reusable [django-treenode](https://github.com/fabiocaccamo/django-treenode) application developed by [Fabio Caccamo](https://github.com/fabiocaccamo).
 The original application has significant advantages over other analogues, and indeed, is one of the best implementations of support for hierarchical structures for Django. 
 
 Fabio's idea was to use the Adjacency List method to store the data tree. The most probable and time-consuming requests are calculated in advance and stored in the database. Also, most requests are cached. As a result, query processing is carried out in one call to the database or without it at all.
 
@@ -38,30 +39,29 @@
 * [presentation](https://www.slideshare.net/billkarwin/models-for-hierarchical-data) by Bill Karwin;
 * [article](https://dirtsimple.org/2010/11/simplest-way-to-do-tree-based-queries.html) by blogger Dirt Simple;
 * [article](https://towardsdatascience.com/closure-table-pattern-to-model-hierarchies-in-nosql-c1be6a87e05b) by Andriy Zabavskyy.
 
 You can easily find additional information on your own on the Internet.
 
 ## Quick start
-1. Run pip install django-treenode
-2. Add fast-treenode to settings.INSTALLED_APPS
-3. Make your model inherit from treenode.models.TreeNodeModel (described below)
-4. Make your model-admin inherit from treenode.admin.TreeNodeModelAdmin (described below)
-5. Run python manage.py makemigrations and python manage.py migrate
+1. Run ```pip install django-fast-treenode```
+2. Add ```treenode``` to ```settings.INSTALLED_APPS```
+3. Make your model inherit from ```treenode.models.TreeNodeModel``` (described below)
+4. Make your model-admin inherit from ```treenode.admin.TreeNodeModelAdmin``` (described below)
+5. Run python manage.py makemigrations and ```python manage.py migrate```
 
 When updating an existing project, simply call ```cls.update_tree()``` function once. 
 It will automatically build a new and complete Closure Table for your tree.
 
 ## Configuration
 ### `models.py`
 Make your model class inherit from `treenode.models.TreeNodeModel`:
 
 ```python
 from django.db import models
-
 from treenode.models import TreeNodeModel
 
 
 class Category(TreeNodeModel):
 
     # the field used to display the model instance
     # default value 'pk'
@@ -72,18 +72,14 @@
     class Meta(TreeNodeModel.Meta):
         verbose_name = "Category"
         verbose_name_plural = "Categories"
 ```
 
 The `TreeNodeModel` abstract class adds many fields (prefixed with `tn_` to prevent direct access) and public methods to your models.
 
-:warning: **If you are extending a model that already has some fields, please ensure that your model existing fields names don't clash with `TreeNodeModel` public [methods/properties](#methodsproperties) names.**
-
----
-
 ### `admin.py`
 Make your model-admin class inherit from `treenode.admin.TreeNodeModelAdmin`.
 
 ```python
 from django.contrib import admin
 
 from treenode.admin import TreeNodeModelAdmin
@@ -119,14 +115,24 @@
         "LOCATION": "...",
     },
     "treenode": {
         "BACKEND": "django.core.cache.backends.locmem.LocMemCache",
     },
 }
 ```
+### `forms.py`
+
+```
+class YoursForm(TreeNodeForm):
+
+    class Meta:
+        widgets = {
+            'tn_parent': TreeWidget(attrs={'style': 'min-width:400px'}),
+        }
+```
 
 ## Usage
 
 ### Methods/Properties
 
 -   [`delete`](#delete)
 -   [`delete_tree`](#delete_tree)
@@ -150,14 +156,15 @@
 -   [`get_index`](#get_index)
 -   [`get_last_child`](#get_last_child)
 -   [`get_level`](#get_level)
 -   [`get_order`](#get_order)
 -   [`get_parent`](#get_parent)
 -   [`get_parent_pk`](#get_parent_pk)
 -   [`set_parent`](#set_parent)
+-   [`get_path`](#get_path)
 -   [`get_priority`](#get_priority)
 -   [`set_priority`](#set_priority)
 -   [`get_root`](#get_root)
 -   [`get_root_pk`](#get_root_pk)
 -   [`get_roots`](#get_roots)
 -   [`get_roots_queryset`](#get_roots_queryset)
 -   [`get_siblings`](#get_siblings)
@@ -173,17 +180,14 @@
 -   [`is_last_child`](#is_last_child)
 -   [`is_leaf`](#is_leaf)
 -   [`is_parent_of`](#is_parent_of)
 -   [`is_root`](#is_root)
 -   [`is_root_of`](#is_root_of)
 -   [`is_sibling_of`](#is_sibling_of)
 -   [`update_tree`](#update_tree)
--   [`get_ordered_queryset`](#get_ordered_queryset)
--   [`get_path`](#get_path)
-
 
 #### `delete`
 **Delete a node** if `cascade=True` (default behaviour), children and descendants will be deleted too,
 otherwise children's parent will be set to `None` (then children become roots):
 ```python
 obj.delete(cascade=True)
 ```
@@ -381,14 +385,19 @@
 #### `get_priority`
 Get the **node priority**:
 ```python
 obj.get_priority()
 # or
 obj.priority
 ```
+#### `get_path`
+Added the function of decorating a **materialized path**. The path is formed according to the value of the `tn_priority` field.
+```python
+cls.get_path(prefix='', suffix='', delimiter='.', format_str='')
+```
 
 #### `set_priority`
 Set the **node priority**:
 ```python
 obj.set_priority(100)
 ```
 
@@ -531,38 +540,16 @@
 
 #### `update_tree`
 **Update tree** manually, useful after **bulk updates**:
 ```python
 cls.update_tree()
 ```
 
-### `get_ordered_queryset`
-Returns a queryset of nodes ordered by tn_priority each node. 
-```python
-cls.get_ordered_queryset()
-```
-For example:
-- N.1
-- N.1.1
-- N.1.1.1
-- N.1.1.2
-- N.2
-- N.2.1
-- ...
-
-This method uses a lot of memory, RawSQL() and .extra() QuerySet method. It's possible I'll change this method due to concerns about aiming to deprecate .extra() method from Django in the future. Use it only if you cannot otherwise assemble an ordered tree from an Adjacency Table and a Closure Table. In most cases, the data in one Adjacency Table is sufficient for such an assembly. You can easily find the corresponding algorithms (two-pass and one-pass) on the Internet.
-
-### get_path
-Added the function of decorating a **materialized path**. The path is formed according to the value of the `tn_priority` field.
-```python
-cls.get_path(prefix='', suffix='', delimiter='.', format_str='')
-```
-
 ## License
-Released under MIT License.
+Released under [MIT License](https://github.com/TimurKady/django-fast-treenode/blob/main/LICENSE).
 
 ## Cautions
 The code provided is intended for testing by developers and is not recommended for use in production projects. Only general tests were carried out. The risk of using the code lies entirely with you.
 
 Don't access treenode fields directly! Most of them have been removed as unnecessary. Use functions documented in the [source application](https://github.com/fabiocaccamo/django-treenode).
 
 ## Credits
@@ -570,15 +557,13 @@
 *  [django-treenode](https://github.com/fabiocaccamo/django-treenode) by [Fabio Caccamo](https://github.com/fabiocaccamo);
 *  [Select2-to-Tree](https://github.com/clivezhg/select2-to-tree) Select2 extension by [clivezhg](https://github.com/clivezhg)
 
 Special thanks to [Mathieu Leplatre](https://blog.mathieu-leplatre.info/pages/about.html) for the advice used in writing this application
 
 ## To do
 Future plans:
-* catch bugs and finish full testing;
-* may be will restore caching;
 * may be will add the ability to determine the priority of the parent by any field, for example, by creation date or alphabetical order;
-* to perform final code optimization;
-* to be happy, to don't worry, until die;
-* drug-and-drop support.
+* drug-and-drop support;
+* to be happy, to don't worry, until die.
+
 
-Your wishes, objections, comments are welcome.
+Your wishes, objections, comments are welcome.
```

### Comparing `django-fast-treenode-1.0.3/treenode/factory.py` & `django-fast-treenode-1.1.0/treenode/factory.py`

 * *Files identical despite different names*

### Comparing `django-fast-treenode-1.0.3/treenode/forms.py` & `django-fast-treenode-1.1.0/treenode/forms.py`

 * *Files identical despite different names*

### Comparing `django-fast-treenode-1.0.3/treenode/managers.py` & `django-fast-treenode-1.1.0/treenode/managers.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # -*- coding: utf-8 -*-
 """
 TreeNode Managers Module
 
 """
 
 from django.db import models
+from django.db.models import Case, When, Value
 
 
 class TreeNodeQuerySet(models.QuerySet):
     """TreeNode Manager QuerySet Class"""
 
     def __init__(self, model=None, query=None, using=None, hints=None):
         self.closure_model = model.closure_model
@@ -44,11 +45,25 @@
         return objs
 
 
 class TreeNodeManager(models.Manager):
     """TreeNode Manager Class"""
 
     def get_queryset(self):
-        return TreeNodeQuerySet(self.model, using=self._db)
-
+        """
+        Forms a QuerySet ordered by the materialized path.
+        """
+
+        qs = TreeNodeQuerySet(self.model, using=self._db)
+        node_list = sorted([node for node in qs], key=lambda x: x.tn_order)
+        pk_list = [node.pk for node in node_list]
+
+        # Retrieve the queryset with the desired ordering
+        return qs.filter(pk__in=pk_list).order_by(
+            Case(*[When(pk=pk, then=Value(ordering))
+                   for ordering, pk in enumerate(pk_list)],
+                 default=Value(len(pk_list)),
+                 output_field=models.IntegerField(),
+                 )
+        )
 
 # End
```

### Comparing `django-fast-treenode-1.0.3/treenode/models.py` & `django-fast-treenode-1.1.0/treenode/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,14 +10,43 @@
 from django.utils.translation import gettext_lazy as _
 from six import with_metaclass
 from . import classproperty
 from .compat import force_str
 from .factory import TreeFactory
 from .managers import TreeNodeManager
 
+from django.core.cache import cache
+
+
+def cached_tree_method(func):
+    """
+    Decorator to cache the results of tree methods
+
+    The decorator caches the results of the decorated method using the
+    closure_path of the node as part of the cache key. If the cache is
+    cleared or invalidated, the cached results will be recomputed.
+
+    Usage:
+        @cached_tree_method
+        def my_tree_method(self):
+            # Tree method logic
+    """
+
+    def wrapper(self, *args, **kwargs):
+        cache_key = f"{self.__class__.__name__}_{self.pk}_tree_{func.__name__}"
+        result = cache.get(cache_key)
+
+        if result is None:
+            result = func(self, *args, **kwargs)
+            cache.set(cache_key, result)
+
+        return result
+
+    return wrapper
+
 
 class TreeNodeModel(with_metaclass(TreeFactory, models.Model)):
 
     treenode_display_field = None
 
     tn_parent = models.ForeignKey(
         'self',
@@ -38,65 +67,54 @@
     class Meta:
         abstract = True
 
     def __str__(self):
         if self.treenode_display_field:
             return str(getattr(self, self.treenode_display_field))
         else:
-            return 'Node %d' % str(self.pk)
+            return 'Node %d' % self.pk
 
     # Public methods
 
     @classmethod
     def get_roots(cls):
         """Get a list with all root nodes"""
-        return list(item for item in cls.objects.filter(tn_parent=None))
+        return list(item for item in cls.get_roots_queryset())
 
     @classmethod
+    @cached_tree_method
     def get_roots_queryset(cls):
         """Get root nodes queryset"""
         return cls.objects.filter(tn_parent=None)
 
     @classmethod
-    def get_ordered_queryset(cls):
-        """Returns a set of nodes sorted by tn_priority"""
-
-        qs = cls.objects.all()
-        table = cls._meta.db_table
-        pk_list = sorted([node.pk for node in qs], key=lambda x: x.tn_order)
-        clauses = ' '.join(
-            ['WHEN %s.id=%s THEN %s' % (table, pk, i)
-             for i, pk in enumerate(pk_list)]
-        )
-        order = 'CASE %s END' % clauses
-        queryset = cls.objects.filter(pk__in=pk_list).extra(
-            select={'ordering': order}, order_by=('ordering',))
-        return queryset
-
-    @classmethod
+    @cached_tree_method
     def get_tree(cls, instance=None):
         """Get a n-dimensional dict representing the model tree"""
 
         objs_list = list(instance,) if instance else cls.get_roots()
         objs_tree = list()
         for item in objs_list:
             objs_tree.append(item.object2dict(item, []))
         return objs_tree
 
     @classmethod
+    @cached_tree_method
     def get_tree_display(cls, cache=True):
         """Get a multiline string representing the model tree"""
 
         objs = list(cls.objects.all())
         return '\n'.join(['%s' % (obj,) for obj in objs])
 
     @classmethod
     def update_tree(cls):
         """Update tree manually, useful after bulk updates"""
 
+        cache.clear()
+
         cls.closure_model.objects.all().delete()
 
         # Apparently later, you should think about using iterators to reduce
         # the amount of memory used.
         # I'm sorry, I don't have time for that right now.
 
         cls.closure_model.objects.bulk_create([
@@ -125,15 +143,15 @@
             ]
             cls.closure_model.objects.bulk_create(objects)
         cls._update_orders()
 
     @classmethod
     def delete_tree(cls):
         """Delete the whole tree for the current node class"""
-
+        cache.clear()
         cls.closure_model.objects.all().delete()
         cls.objects.all().delete()
 
     def get_ancestors(self, include_self=True, depth=None):
         """Get a list with all ancestors (ordered from root to self/parent)"""
 
         options = dict(child_id=self.pk, depth__gte=0 if include_self else 1)
@@ -156,26 +174,28 @@
         if depth:
             options.update({'depth__lte': depth})
 
         qs = self._closure_model.objects.filter(**options).order_by('-depth')
 
         return list(item.parent.pk for item in qs)
 
+    @cached_tree_method
     def get_ancestors_queryset(self, include_self=True, depth=None):
         """Get the ancestors queryset (self, ordered from parent to root)"""
 
         options = dict(child_id=self.pk, depth__gte=0 if include_self else 1)
         if depth:
             options.update({'depth__lte': depth})
 
         qs = self._closure_model.objects.filter(**options).order_by('-depth')
         select = list(item.parent.pk for item in qs)
         resurt = self._meta.model.objects.filter(pk__in=select)
         return resurt
 
+    @cached_tree_method
     def get_breadcrumbs(self, attr=None):
         """Get the breadcrumbs to current node (self, included)"""
 
         qs = self._closure_model.objects.filter(child=self).order_by('-depth')
         if attr:
             return list(getattr(item.parent, attr) for item in qs)
         else:
@@ -192,14 +212,15 @@
         return self.get_children_queryset().count()
 
     def get_children_pks(self):
         """Get the children pks list"""
 
         return [ch.pk for ch in self.get_children_queryset()]
 
+    @cached_tree_method
     def get_children_queryset(self):
         """Get the children queryset"""
         return self._meta.model.objects.filter(tn_paren=self.id)
 
     def get_depth(self):
         """Get the node depth (self, how many levels of descendants)"""
 
@@ -222,14 +243,15 @@
         options = dict(parent_id=self.pk, depth__gte=0 if include_self else 1)
         if depth:
             options.update({'depth__lte': depth})
 
         qs = self._closure_model.objects.filter(**options)
         return [ch.child.pk for ch in qs] if qs else []
 
+    @cached_tree_method
     def get_descendants_queryset(self, include_self=False, depth=None):
         """Get the descendants queryset"""
 
         pks = self.get_descendants_pks(include_self, depth)
         return self._meta.model.objects.filter(**pks)
 
     def get_descendants_tree(self):
@@ -309,14 +331,15 @@
         """Get the siblings count"""
         return self.get_siblings_queryset().count()
 
     def get_siblings_pks(self):
         """Get the siblings pks list"""
         return [item.pk for item in self.get_siblings_queryset()]
 
+    @cached_tree_method
     def get_siblings_queryset(self):
         """Get the siblings queryset"""
         if self.tn_parent:
             queryset = self.tn_parent.tn_children.all()
         else:
             queryset = self._meta.model.objects.filter(tn_parent__isnull=True)
         return queryset.exclude(pk=self.pk)
@@ -497,16 +520,17 @@
     @property
     def _closure_model(self):
         return self._meta.model.closure_model
 
     @property
     def tn_order(self):
         path = self.get_breadcrumbs(attr='tn_priority')
-        return '.'.join(['{:0>6g}'.format(i) for i in path])
+        return ''.join(['{:0>6g}'.format(i) for i in path])
 
+    @cached_tree_method
     def object2dict(self, instance, exclude=[]):
         """Convert Class Object to python dict"""
 
         result = dict()
 
         if not hasattr(instance, '__dict__'):
             return instance
@@ -523,21 +547,23 @@
                 'children': [
                     obj.object2dict(obj, exclude)
                     for obj in childs.all()]
             })
         result.update({'path': instance.get_path(format_str=':d')})
         return result
 
+    @cached_tree_method
     def get_display(self, indent=True, mark='— '):
         indentation = (mark * self.tn_ancestors_count) if indent else ''
         indentation = force_str(indentation)
         text = self.get_display_text()
         text = force_str(text)
         return indentation + text
 
+    @cached_tree_method
     def get_display_text(self):
         """
         Gets the text that will be indented in `get_display` method.
         Returns the `treenode_display_field` value if specified,
         otherwise falls back on the model's pk.
         Override this method to return another field or a computed value. #27
         """
@@ -550,14 +576,16 @@
             text = self.pk
         return force_str(text)
 
     @transaction.atomic
     def _insert(self):
         """Adds a new entry to the Adjacency Table and the Closure Table"""
 
+        cache.clear()
+
         instance = self._closure_model.objects.create(
             parent=self,
             child=self,
             depth=0
         )
         instance.save()
 
@@ -573,14 +601,16 @@
             for p in parents
             for c in children
         ]
         self._closure_model.objects.bulk_create(objects)
 
     @transaction.atomic
     def _move_to(self, old_parent):
+        cache.clear()
+
         target = self.tn_parent
         qs = self._closure_model.objects.all()
         subtree = qs.filter(parent=self).values('child', 'depth')
         supertree = qs.filter(child=target).values('parent', 'depth')
 
         # Step 1. Delete
         subtree_pks = [node.child.pk for node in qs.filter(parent=self)]
@@ -597,14 +627,16 @@
             for p in supertree
             for c in subtree
         ]
         self._closure_model.objects.bulk_create(objects)
 
     def _order(self):
 
+        cache.clear()
+
         queryset = self.get_siblings_queryset()
 
         if self.tn_priority > queryset.count():
             self.tn_priority = queryset.count()
 
         siblings = list(node for node in queryset)
         sorted_siblings = sorted(siblings, key=lambda x: x.tn_priority)
@@ -613,14 +645,15 @@
         for index in range(len(sorted_siblings)):
             sorted_siblings[index].tn_priority = index
 
         self._meta.model.objects.bulk_update(
             sorted_siblings, ('tn_priority', ))
 
     def save(self, force_insert=False, *args, **kwargs):
+        cache.clear()
 
         try:
             old = self._meta.model.objects.get(pk=self.pk)
             old_parent = old.tn_parent
         except:
             force_insert = True
```

### Comparing `django-fast-treenode-1.0.3/treenode/static/select2tree/select2tree.css` & `django-fast-treenode-1.1.0/treenode/static/select2tree/select2tree.css`

 * *Files identical despite different names*

### Comparing `django-fast-treenode-1.0.3/treenode/static/select2tree/select2tree.js` & `django-fast-treenode-1.1.0/treenode/static/select2tree/select2tree.js`

 * *Files identical despite different names*

### Comparing `django-fast-treenode-1.0.3/treenode/static/treenode/css/treenode.css` & `django-fast-treenode-1.1.0/treenode/static/treenode/css/treenode.css`

 * *Files identical despite different names*

### Comparing `django-fast-treenode-1.0.3/treenode/static/treenode/js/treenode.js` & `django-fast-treenode-1.1.0/treenode/static/treenode/js/treenode.js`

 * *Files identical despite different names*

### Comparing `django-fast-treenode-1.0.3/treenode/templates/widgets/select2tree.html` & `django-fast-treenode-1.1.0/treenode/templates/widgets/select2tree.html`

 * *Files identical despite different names*

### Comparing `django-fast-treenode-1.0.3/treenode/widgets.py` & `django-fast-treenode-1.1.0/treenode/widgets.py`

 * *Files identical despite different names*

