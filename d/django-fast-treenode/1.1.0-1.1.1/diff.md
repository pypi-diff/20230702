# Comparing `tmp/django-fast-treenode-1.1.0.tar.gz` & `tmp/django-fast-treenode-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-fast-treenode-1.1.0.tar", last modified: Sun Jul  2 16:52:45 2023, max compression
+gzip compressed data, was "django-fast-treenode-1.1.1.tar", last modified: Sun Jul  2 17:48:58 2023, max compression
```

## Comparing `django-fast-treenode-1.1.0.tar` & `django-fast-treenode-1.1.1.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxrwxrwx   0        0        0        0 2023-07-02 16:52:44.000000 django-fast-treenode-1.1.0/
--rw-rw-rw-   0        0        0     1091 2023-06-28 08:53:50.000000 django-fast-treenode-1.1.0/LICENSE
--rw-rw-rw-   0        0        0      146 2023-07-02 16:40:36.000000 django-fast-treenode-1.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0    17051 2023-07-02 16:52:46.000000 django-fast-treenode-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0    16141 2023-07-02 16:37:32.000000 django-fast-treenode-1.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-02 16:52:44.000000 django-fast-treenode-1.1.0/django_fast_treenode.egg-info/
--rw-rw-rw-   0        0        0    17051 2023-07-02 16:52:44.000000 django-fast-treenode-1.1.0/django_fast_treenode.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1088 2023-07-02 16:52:44.000000 django-fast-treenode-1.1.0/django_fast_treenode.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-02 16:52:44.000000 django-fast-treenode-1.1.0/django_fast_treenode.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-07-02 16:52:44.000000 django-fast-treenode-1.1.0/django_fast_treenode.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-02 16:52:44.000000 django-fast-treenode-1.1.0/django_fast_treenode.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       90 2023-05-31 11:15:42.000000 django-fast-treenode-1.1.0/pyproject.toml
--rw-rw-rw-   0        0        0      935 2023-07-02 16:52:46.000000 django-fast-treenode-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0       39 2023-05-31 11:20:32.000000 django-fast-treenode-1.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-02 16:52:44.000000 django-fast-treenode-1.1.0/treenode/
--rw-rw-rw-   0        0        0      171 2023-07-01 02:29:18.000000 django-fast-treenode-1.1.0/treenode/__init__.py
--rw-rw-rw-   0        0        0     5374 2023-07-02 11:48:12.000000 django-fast-treenode-1.1.0/treenode/admin.py
--rw-rw-rw-   0        0        0      154 2023-07-01 02:29:18.000000 django-fast-treenode-1.1.0/treenode/apps.py
--rw-rw-rw-   0        0        0      185 2023-07-01 02:29:18.000000 django-fast-treenode-1.1.0/treenode/compat.py
-drwxrwxrwx   0        0        0        0 2023-07-02 16:52:44.000000 django-fast-treenode-1.1.0/treenode/docs/
--rw-rw-rw-   0        0        0        1 2023-07-01 02:29:18.000000 django-fast-treenode-1.1.0/treenode/docs/.gitkeep
--rw-rw-rw-   0        0        0    16141 2023-07-02 16:37:32.000000 django-fast-treenode-1.1.0/treenode/docs/Documentation
--rw-rw-rw-   0        0        0     1942 2023-07-01 02:29:18.000000 django-fast-treenode-1.1.0/treenode/factory.py
--rw-rw-rw-   0        0        0      907 2023-07-01 02:29:18.000000 django-fast-treenode-1.1.0/treenode/forms.py
--rw-rw-rw-   0        0        0     2210 2023-07-02 11:42:06.000000 django-fast-treenode-1.1.0/treenode/managers.py
--rw-rw-rw-   0        0        0    20653 2023-07-02 16:25:56.000000 django-fast-treenode-1.1.0/treenode/models.py
-drwxrwxrwx   0        0        0        0 2023-07-02 16:52:44.000000 django-fast-treenode-1.1.0/treenode/static/
--rw-rw-rw-   0        0        0        0 2023-07-01 02:29:18.000000 django-fast-treenode-1.1.0/treenode/static/.gitkeep
-drwxrwxrwx   0        0        0        0 2023-07-02 16:52:44.000000 django-fast-treenode-1.1.0/treenode/static/select2tree/
--rw-rw-rw-   0        0        0        1 2023-07-01 02:29:18.000000 django-fast-treenode-1.1.0/treenode/static/select2tree/.gitkeep
--rw-rw-rw-   0        0        0     4234 2023-07-02 11:53:28.000000 django-fast-treenode-1.1.0/treenode/static/select2tree/select2tree.css
--rw-rw-rw-   0        0        0     5948 2023-07-01 02:29:18.000000 django-fast-treenode-1.1.0/treenode/static/select2tree/select2tree.js
-drwxrwxrwx   0        0        0        0 2023-07-02 16:52:44.000000 django-fast-treenode-1.1.0/treenode/static/treenode/
--rw-rw-rw-   0        0        0        1 2023-07-01 02:29:18.000000 django-fast-treenode-1.1.0/treenode/static/treenode/.gitkeep
-drwxrwxrwx   0        0        0        0 2023-07-02 16:52:44.000000 django-fast-treenode-1.1.0/treenode/static/treenode/css/
--rw-rw-rw-   0        0        0        1 2023-07-01 02:29:18.000000 django-fast-treenode-1.1.0/treenode/static/treenode/css/.gitkeep
--rw-rw-rw-   0        0        0     1637 2023-07-01 02:29:18.000000 django-fast-treenode-1.1.0/treenode/static/treenode/css/treenode.css
-drwxrwxrwx   0        0        0        0 2023-07-02 16:52:44.000000 django-fast-treenode-1.1.0/treenode/static/treenode/js/
--rw-rw-rw-   0        0        0        1 2023-07-01 02:29:18.000000 django-fast-treenode-1.1.0/treenode/static/treenode/js/.gitkeep
--rw-rw-rw-   0        0        0     7797 2023-07-01 02:29:18.000000 django-fast-treenode-1.1.0/treenode/static/treenode/js/treenode.js
-drwxrwxrwx   0        0        0        0 2023-07-02 16:52:44.000000 django-fast-treenode-1.1.0/treenode/templates/
--rw-rw-rw-   0        0        0        1 2023-07-01 02:29:18.000000 django-fast-treenode-1.1.0/treenode/templates/.gitkeep
-drwxrwxrwx   0        0        0        0 2023-07-02 16:52:44.000000 django-fast-treenode-1.1.0/treenode/templates/widgets/
--rw-rw-rw-   0        0        0        1 2023-07-01 02:29:18.000000 django-fast-treenode-1.1.0/treenode/templates/widgets/.gitkeep
--rw-rw-rw-   0        0        0      217 2023-07-01 02:29:18.000000 django-fast-treenode-1.1.0/treenode/templates/widgets/attrs.html
--rw-rw-rw-   0        0        0      288 2023-07-01 02:29:18.000000 django-fast-treenode-1.1.0/treenode/templates/widgets/options.html
--rw-rw-rw-   0        0        0      675 2023-07-01 02:29:18.000000 django-fast-treenode-1.1.0/treenode/templates/widgets/select2tree.html
--rw-rw-rw-   0        0        0       63 2023-07-01 02:29:18.000000 django-fast-treenode-1.1.0/treenode/tests.py
--rw-rw-rw-   0        0        0       50 2023-07-02 16:28:58.000000 django-fast-treenode-1.1.0/treenode/version.py
--rw-rw-rw-   0        0        0       66 2023-07-01 02:29:18.000000 django-fast-treenode-1.1.0/treenode/views.py
--rw-rw-rw-   0        0        0     1189 2023-07-01 02:29:18.000000 django-fast-treenode-1.1.0/treenode/widgets.py
+drwxrwxrwx   0        0        0        0 2023-07-02 17:48:58.000000 django-fast-treenode-1.1.1/
+-rw-rw-rw-   0        0        0     1091 2023-06-28 08:53:50.000000 django-fast-treenode-1.1.1/LICENSE
+-rw-rw-rw-   0        0        0      146 2023-07-02 16:40:36.000000 django-fast-treenode-1.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0    17300 2023-07-02 17:49:00.000000 django-fast-treenode-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0    16390 2023-07-02 17:12:02.000000 django-fast-treenode-1.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-02 17:48:58.000000 django-fast-treenode-1.1.1/django_fast_treenode.egg-info/
+-rw-rw-rw-   0        0        0    17300 2023-07-02 17:48:58.000000 django-fast-treenode-1.1.1/django_fast_treenode.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1088 2023-07-02 17:48:58.000000 django-fast-treenode-1.1.1/django_fast_treenode.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-02 17:48:58.000000 django-fast-treenode-1.1.1/django_fast_treenode.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-07-02 17:48:58.000000 django-fast-treenode-1.1.1/django_fast_treenode.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-02 17:48:58.000000 django-fast-treenode-1.1.1/django_fast_treenode.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       90 2023-05-31 11:15:42.000000 django-fast-treenode-1.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0      935 2023-07-02 17:49:00.000000 django-fast-treenode-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      112 2023-07-02 17:12:04.000000 django-fast-treenode-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-02 17:48:58.000000 django-fast-treenode-1.1.1/treenode/
+-rw-rw-rw-   0        0        0      171 2023-07-01 02:29:18.000000 django-fast-treenode-1.1.1/treenode/__init__.py
+-rw-rw-rw-   0        0        0     5374 2023-07-02 11:48:12.000000 django-fast-treenode-1.1.1/treenode/admin.py
+-rw-rw-rw-   0        0        0      154 2023-07-01 02:29:18.000000 django-fast-treenode-1.1.1/treenode/apps.py
+-rw-rw-rw-   0        0        0      185 2023-07-01 02:29:18.000000 django-fast-treenode-1.1.1/treenode/compat.py
+drwxrwxrwx   0        0        0        0 2023-07-02 17:48:58.000000 django-fast-treenode-1.1.1/treenode/docs/
+-rw-rw-rw-   0        0        0        1 2023-07-01 02:29:18.000000 django-fast-treenode-1.1.1/treenode/docs/.gitkeep
+-rw-rw-rw-   0        0        0    16141 2023-07-02 16:37:32.000000 django-fast-treenode-1.1.1/treenode/docs/Documentation
+-rw-rw-rw-   0        0        0     1942 2023-07-01 02:29:18.000000 django-fast-treenode-1.1.1/treenode/factory.py
+-rw-rw-rw-   0        0        0      907 2023-07-01 02:29:18.000000 django-fast-treenode-1.1.1/treenode/forms.py
+-rw-rw-rw-   0        0        0     2210 2023-07-02 11:42:06.000000 django-fast-treenode-1.1.1/treenode/managers.py
+-rw-rw-rw-   0        0        0    20763 2023-07-02 17:33:20.000000 django-fast-treenode-1.1.1/treenode/models.py
+drwxrwxrwx   0        0        0        0 2023-07-02 17:48:58.000000 django-fast-treenode-1.1.1/treenode/static/
+-rw-rw-rw-   0        0        0        0 2023-07-01 02:29:18.000000 django-fast-treenode-1.1.1/treenode/static/.gitkeep
+drwxrwxrwx   0        0        0        0 2023-07-02 17:48:58.000000 django-fast-treenode-1.1.1/treenode/static/select2tree/
+-rw-rw-rw-   0        0        0        1 2023-07-01 02:29:18.000000 django-fast-treenode-1.1.1/treenode/static/select2tree/.gitkeep
+-rw-rw-rw-   0        0        0     4234 2023-07-02 11:53:28.000000 django-fast-treenode-1.1.1/treenode/static/select2tree/select2tree.css
+-rw-rw-rw-   0        0        0     5948 2023-07-01 02:29:18.000000 django-fast-treenode-1.1.1/treenode/static/select2tree/select2tree.js
+drwxrwxrwx   0        0        0        0 2023-07-02 17:48:58.000000 django-fast-treenode-1.1.1/treenode/static/treenode/
+-rw-rw-rw-   0        0        0        1 2023-07-01 02:29:18.000000 django-fast-treenode-1.1.1/treenode/static/treenode/.gitkeep
+drwxrwxrwx   0        0        0        0 2023-07-02 17:48:58.000000 django-fast-treenode-1.1.1/treenode/static/treenode/css/
+-rw-rw-rw-   0        0        0        1 2023-07-01 02:29:18.000000 django-fast-treenode-1.1.1/treenode/static/treenode/css/.gitkeep
+-rw-rw-rw-   0        0        0     1637 2023-07-01 02:29:18.000000 django-fast-treenode-1.1.1/treenode/static/treenode/css/treenode.css
+drwxrwxrwx   0        0        0        0 2023-07-02 17:48:58.000000 django-fast-treenode-1.1.1/treenode/static/treenode/js/
+-rw-rw-rw-   0        0        0        1 2023-07-01 02:29:18.000000 django-fast-treenode-1.1.1/treenode/static/treenode/js/.gitkeep
+-rw-rw-rw-   0        0        0     7797 2023-07-01 02:29:18.000000 django-fast-treenode-1.1.1/treenode/static/treenode/js/treenode.js
+drwxrwxrwx   0        0        0        0 2023-07-02 17:48:58.000000 django-fast-treenode-1.1.1/treenode/templates/
+-rw-rw-rw-   0        0        0        1 2023-07-01 02:29:18.000000 django-fast-treenode-1.1.1/treenode/templates/.gitkeep
+drwxrwxrwx   0        0        0        0 2023-07-02 17:48:58.000000 django-fast-treenode-1.1.1/treenode/templates/widgets/
+-rw-rw-rw-   0        0        0        1 2023-07-01 02:29:18.000000 django-fast-treenode-1.1.1/treenode/templates/widgets/.gitkeep
+-rw-rw-rw-   0        0        0      217 2023-07-01 02:29:18.000000 django-fast-treenode-1.1.1/treenode/templates/widgets/attrs.html
+-rw-rw-rw-   0        0        0      288 2023-07-01 02:29:18.000000 django-fast-treenode-1.1.1/treenode/templates/widgets/options.html
+-rw-rw-rw-   0        0        0      675 2023-07-01 02:29:18.000000 django-fast-treenode-1.1.1/treenode/templates/widgets/select2tree.html
+-rw-rw-rw-   0        0        0       63 2023-07-01 02:29:18.000000 django-fast-treenode-1.1.1/treenode/tests.py
+-rw-rw-rw-   0        0        0       50 2023-07-02 17:26:36.000000 django-fast-treenode-1.1.1/treenode/version.py
+-rw-rw-rw-   0        0        0       66 2023-07-01 02:29:18.000000 django-fast-treenode-1.1.1/treenode/views.py
+-rw-rw-rw-   0        0        0     1189 2023-07-01 02:29:18.000000 django-fast-treenode-1.1.1/treenode/widgets.py
```

### Comparing `django-fast-treenode-1.1.0/LICENSE` & `django-fast-treenode-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-fast-treenode-1.1.0/PKG-INFO` & `django-fast-treenode-1.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-fast-treenode
-Version: 1.1.0
+Version: 1.1.1
 Summary: Application for supporting tree (hierarchical) data structure in Django projects
 Home-page: https://github.com/TimurKady/fast-treenode
 Author: Timur Kady
 Author-email: timurkady@yandex.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
@@ -23,15 +23,17 @@
 License-File: LICENSE
 
 # Django-fast-treenode 
 __Combination of Adjacency List and Closure Table__
 
 ## Functions
 Application for supporting tree (hierarchical) data structure in Django projects
-* Faster: resource-intensive operations are cached; bulk operations are used for inserts and changes,
+Application for supporting tree (hierarchical) data structure in Django projects
+* fast: the fastest of the two methods is used to process requests, combining the advantages of an **Adjacency Table** and a **Closure Table**,
+* even faster: the main resource-intensive operations are **cached**; **bulk operations** are used for inserts and changes,
 * synchronized: model instances in memory are automatically updated,
 * compatibility: you can easily add a tree node to existing projects using TreeNode without changing the code,
 * no dependencies,
 * easy setup: just extend the abstract model/model-admin,
 * admin integration: visualization options (accordion, breadcrumbs or padding),
 * widget: Built-in Select2-to-Tree extends Select2 to support arbitrary nesting levels.
```

### Comparing `django-fast-treenode-1.1.0/README.md` & `django-fast-treenode-1.1.1/treenode/docs/Documentation`

 * *Files identical despite different names*

### Comparing `django-fast-treenode-1.1.0/django_fast_treenode.egg-info/PKG-INFO` & `django-fast-treenode-1.1.1/django_fast_treenode.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-fast-treenode
-Version: 1.1.0
+Version: 1.1.1
 Summary: Application for supporting tree (hierarchical) data structure in Django projects
 Home-page: https://github.com/TimurKady/fast-treenode
 Author: Timur Kady
 Author-email: timurkady@yandex.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
@@ -23,15 +23,17 @@
 License-File: LICENSE
 
 # Django-fast-treenode 
 __Combination of Adjacency List and Closure Table__
 
 ## Functions
 Application for supporting tree (hierarchical) data structure in Django projects
-* Faster: resource-intensive operations are cached; bulk operations are used for inserts and changes,
+Application for supporting tree (hierarchical) data structure in Django projects
+* fast: the fastest of the two methods is used to process requests, combining the advantages of an **Adjacency Table** and a **Closure Table**,
+* even faster: the main resource-intensive operations are **cached**; **bulk operations** are used for inserts and changes,
 * synchronized: model instances in memory are automatically updated,
 * compatibility: you can easily add a tree node to existing projects using TreeNode without changing the code,
 * no dependencies,
 * easy setup: just extend the abstract model/model-admin,
 * admin integration: visualization options (accordion, breadcrumbs or padding),
 * widget: Built-in Select2-to-Tree extends Select2 to support arbitrary nesting levels.
```

### Comparing `django-fast-treenode-1.1.0/django_fast_treenode.egg-info/SOURCES.txt` & `django-fast-treenode-1.1.1/django_fast_treenode.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-fast-treenode-1.1.0/setup.cfg` & `django-fast-treenode-1.1.1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 00000000: 5b65 6767 5f69 6e66 6f5d 0d0a 7461 675f  [egg_info]..tag_
 00000010: 6275 696c 6420 3d20 0d0a 7461 675f 6461  build = ..tag_da
 00000020: 7465 203d 2030 0d0a 0d0a 5b6d 6574 6164  te = 0....[metad
 00000030: 6174 615d 0d0a 6e61 6d65 203d 2064 6a61  ata]..name = dja
 00000040: 6e67 6f2d 6661 7374 2d74 7265 656e 6f64  ngo-fast-treenod
 00000050: 650d 0a76 6572 7369 6f6e 203d 2031 2e31  e..version = 1.1
-00000060: 2e30 0d0a 6465 7363 7269 7074 696f 6e20  .0..description 
+00000060: 2e31 0d0a 6465 7363 7269 7074 696f 6e20  .1..description 
 00000070: 3d20 4170 706c 6963 6174 696f 6e20 666f  = Application fo
 00000080: 7220 7375 7070 6f72 7469 6e67 2074 7265  r supporting tre
 00000090: 6520 2868 6965 7261 7263 6869 6361 6c29  e (hierarchical)
 000000a0: 2064 6174 6120 7374 7275 6374 7572 6520   data structure 
 000000b0: 696e 2044 6a61 6e67 6f20 7072 6f6a 6563  in Django projec
 000000c0: 7473 0d0a 6c6f 6e67 5f64 6573 6372 6970  ts..long_descrip
 000000d0: 7469 6f6e 5f63 6f6e 7465 6e74 5f74 7970  tion_content_typ
```

### Comparing `django-fast-treenode-1.1.0/treenode/admin.py` & `django-fast-treenode-1.1.1/treenode/admin.py`

 * *Files identical despite different names*

### Comparing `django-fast-treenode-1.1.0/treenode/docs/Documentation` & `django-fast-treenode-1.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # Django-fast-treenode 
 __Combination of Adjacency List and Closure Table__
 
 ## Functions
 Application for supporting tree (hierarchical) data structure in Django projects
-* Faster: resource-intensive operations are cached; bulk operations are used for inserts and changes,
+Application for supporting tree (hierarchical) data structure in Django projects
+* fast: the fastest of the two methods is used to process requests, combining the advantages of an **Adjacency Table** and a **Closure Table**,
+* even faster: the main resource-intensive operations are **cached**; **bulk operations** are used for inserts and changes,
 * synchronized: model instances in memory are automatically updated,
 * compatibility: you can easily add a tree node to existing projects using TreeNode without changing the code,
 * no dependencies,
 * easy setup: just extend the abstract model/model-admin,
 * admin integration: visualization options (accordion, breadcrumbs or padding),
 * widget: Built-in Select2-to-Tree extends Select2 to support arbitrary nesting levels.
```

### Comparing `django-fast-treenode-1.1.0/treenode/factory.py` & `django-fast-treenode-1.1.1/treenode/factory.py`

 * *Files identical despite different names*

### Comparing `django-fast-treenode-1.1.0/treenode/forms.py` & `django-fast-treenode-1.1.1/treenode/forms.py`

 * *Files identical despite different names*

### Comparing `django-fast-treenode-1.1.0/treenode/managers.py` & `django-fast-treenode-1.1.1/treenode/managers.py`

 * *Files identical despite different names*

### Comparing `django-fast-treenode-1.1.0/treenode/models.py` & `django-fast-treenode-1.1.1/treenode/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,23 +3,24 @@
 TreeNode Models Module
 
 """
 
 
 from django.db import models
 from django.db import transaction
+from django.core.cache import caches
 from django.utils.translation import gettext_lazy as _
 from six import with_metaclass
 from . import classproperty
 from .compat import force_str
 from .factory import TreeFactory
 from .managers import TreeNodeManager
 
-from django.core.cache import cache
 
+treenode_cache = caches['treenode']
 
 def cached_tree_method(func):
     """
     Decorator to cache the results of tree methods
 
     The decorator caches the results of the decorated method using the
     closure_path of the node as part of the cache key. If the cache is
@@ -29,19 +30,19 @@
         @cached_tree_method
         def my_tree_method(self):
             # Tree method logic
     """
 
     def wrapper(self, *args, **kwargs):
         cache_key = f"{self.__class__.__name__}_{self.pk}_tree_{func.__name__}"
-        result = cache.get(cache_key)
+        result = treenode_cache.get(cache_key)
 
         if result is None:
             result = func(self, *args, **kwargs)
-            cache.set(cache_key, result)
+            treenode_cache.set(cache_key, result)
 
         return result
 
     return wrapper
 
 
 class TreeNodeModel(with_metaclass(TreeFactory, models.Model)):
@@ -105,15 +106,15 @@
         objs = list(cls.objects.all())
         return '\n'.join(['%s' % (obj,) for obj in objs])
 
     @classmethod
     def update_tree(cls):
         """Update tree manually, useful after bulk updates"""
 
-        cache.clear()
+        treenode_cache.clear()
 
         cls.closure_model.objects.all().delete()
 
         # Apparently later, you should think about using iterators to reduce
         # the amount of memory used.
         # I'm sorry, I don't have time for that right now.
 
@@ -143,15 +144,15 @@
             ]
             cls.closure_model.objects.bulk_create(objects)
         cls._update_orders()
 
     @classmethod
     def delete_tree(cls):
         """Delete the whole tree for the current node class"""
-        cache.clear()
+        treenode_cache.clear()
         cls.closure_model.objects.all().delete()
         cls.objects.all().delete()
 
     def get_ancestors(self, include_self=True, depth=None):
         """Get a list with all ancestors (ordered from root to self/parent)"""
 
         options = dict(child_id=self.pk, depth__gte=0 if include_self else 1)
@@ -576,15 +577,15 @@
             text = self.pk
         return force_str(text)
 
     @transaction.atomic
     def _insert(self):
         """Adds a new entry to the Adjacency Table and the Closure Table"""
 
-        cache.clear()
+        treenode_cache.clear()
 
         instance = self._closure_model.objects.create(
             parent=self,
             child=self,
             depth=0
         )
         instance.save()
@@ -601,15 +602,15 @@
             for p in parents
             for c in children
         ]
         self._closure_model.objects.bulk_create(objects)
 
     @transaction.atomic
     def _move_to(self, old_parent):
-        cache.clear()
+        treenode_cache.clear()
 
         target = self.tn_parent
         qs = self._closure_model.objects.all()
         subtree = qs.filter(parent=self).values('child', 'depth')
         supertree = qs.filter(child=target).values('parent', 'depth')
 
         # Step 1. Delete
@@ -627,15 +628,15 @@
             for p in supertree
             for c in subtree
         ]
         self._closure_model.objects.bulk_create(objects)
 
     def _order(self):
 
-        cache.clear()
+        treenode_cache.clear()
 
         queryset = self.get_siblings_queryset()
 
         if self.tn_priority > queryset.count():
             self.tn_priority = queryset.count()
 
         siblings = list(node for node in queryset)
@@ -645,15 +646,15 @@
         for index in range(len(sorted_siblings)):
             sorted_siblings[index].tn_priority = index
 
         self._meta.model.objects.bulk_update(
             sorted_siblings, ('tn_priority', ))
 
     def save(self, force_insert=False, *args, **kwargs):
-        cache.clear()
+        treenode_cache.clear()
 
         try:
             old = self._meta.model.objects.get(pk=self.pk)
             old_parent = old.tn_parent
         except:
             force_insert = True
```

### Comparing `django-fast-treenode-1.1.0/treenode/static/select2tree/select2tree.css` & `django-fast-treenode-1.1.1/treenode/static/select2tree/select2tree.css`

 * *Files identical despite different names*

### Comparing `django-fast-treenode-1.1.0/treenode/static/select2tree/select2tree.js` & `django-fast-treenode-1.1.1/treenode/static/select2tree/select2tree.js`

 * *Files identical despite different names*

### Comparing `django-fast-treenode-1.1.0/treenode/static/treenode/css/treenode.css` & `django-fast-treenode-1.1.1/treenode/static/treenode/css/treenode.css`

 * *Files identical despite different names*

### Comparing `django-fast-treenode-1.1.0/treenode/static/treenode/js/treenode.js` & `django-fast-treenode-1.1.1/treenode/static/treenode/js/treenode.js`

 * *Files identical despite different names*

### Comparing `django-fast-treenode-1.1.0/treenode/templates/widgets/select2tree.html` & `django-fast-treenode-1.1.1/treenode/templates/widgets/select2tree.html`

 * *Files identical despite different names*

### Comparing `django-fast-treenode-1.1.0/treenode/widgets.py` & `django-fast-treenode-1.1.1/treenode/widgets.py`

 * *Files identical despite different names*

