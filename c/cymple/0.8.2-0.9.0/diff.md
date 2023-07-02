# Comparing `tmp/cymple-0.8.2.tar.gz` & `tmp/cymple-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cymple-0.8.2.tar", last modified: Sun Jul  2 08:17:03 2023, max compression
+gzip compressed data, was "cymple-0.9.0.tar", last modified: Sun Jul  2 09:21:48 2023, max compression
```

## Comparing `cymple-0.8.2.tar` & `cymple-0.9.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 08:17:03.969011 cymple-0.8.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-02 08:16:50.000000 cymple-0.8.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7465 2023-07-02 08:17:03.969011 cymple-0.8.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7445 2023-07-02 08:16:50.000000 cymple-0.8.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-02 08:16:50.000000 cymple-0.8.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-02 08:17:03.969011 cymple-0.8.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-02 08:16:50.000000 cymple-0.8.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 08:17:03.965011 cymple-0.8.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 08:17:03.969011 cymple-0.8.2/src/cymple/
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-02 08:16:50.000000 cymple-0.8.2/src/cymple/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-02 08:16:50.000000 cymple-0.8.2/src/cymple/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36959 2023-07-02 08:16:50.000000 cymple-0.8.2/src/cymple/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-07-02 08:16:50.000000 cymple-0.8.2/src/cymple/typedefs.py
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-02 08:16:50.000000 cymple-0.8.2/src/cymple/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 08:17:03.969011 cymple-0.8.2/src/cymple.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7465 2023-07-02 08:17:03.000000 cymple-0.8.2/src/cymple.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-02 08:17:03.000000 cymple-0.8.2/src/cymple.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 08:17:03.000000 cymple-0.8.2/src/cymple.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-02 08:17:03.000000 cymple-0.8.2/src/cymple.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:21:48.414285 cymple-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-02 09:21:37.000000 cymple-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7465 2023-07-02 09:21:48.414285 cymple-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7445 2023-07-02 09:21:37.000000 cymple-0.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-02 09:21:37.000000 cymple-0.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-02 09:21:48.414285 cymple-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-02 09:21:37.000000 cymple-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:21:48.410285 cymple-0.9.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:21:48.414285 cymple-0.9.0/src/cymple/
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-02 09:21:37.000000 cymple-0.9.0/src/cymple/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-02 09:21:37.000000 cymple-0.9.0/src/cymple/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37845 2023-07-02 09:21:37.000000 cymple-0.9.0/src/cymple/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-07-02 09:21:37.000000 cymple-0.9.0/src/cymple/typedefs.py
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-02 09:21:37.000000 cymple-0.9.0/src/cymple/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:21:48.414285 cymple-0.9.0/src/cymple.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7465 2023-07-02 09:21:48.000000 cymple-0.9.0/src/cymple.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-02 09:21:48.000000 cymple-0.9.0/src/cymple.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 09:21:48.000000 cymple-0.9.0/src/cymple.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-02 09:21:48.000000 cymple-0.9.0/src/cymple.egg-info/top_level.txt
```

### Comparing `cymple-0.8.2/LICENSE` & `cymple-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cymple-0.8.2/PKG-INFO` & `cymple-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cymple
-Version: 0.8.2
+Version: 0.9.0
 Summary: A productivity enhancer for creating Cypher queries in Python
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8
 License-File: LICENSE
 
 # Cymple - Cypher Modular Pythonic Language Extension
```

### Comparing `cymple-0.8.2/README.md` & `cymple-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `cymple-0.8.2/setup.cfg` & `cymple-0.9.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `cymple-0.8.2/src/cymple/builder.py` & `cymple-0.9.0/src/cymple/builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -408,33 +408,40 @@
         :type **kwargs
 
         :return: A Query object with a query that contains the new clause.
         :rtype: RelationAvailable
         """
         return RelationAvailable(self.query + self._directed_relation('backward', label, ref_name, properties, **kwargs))
 
-    def related_variable_len(self, min_hops: int = -1, max_hops: int = -1):
+    def related_variable_len(self, label: str = None, ref_name: str = None, min_hops: int = -1, max_hops: int = -1):
         """Concatenate a uni-directional graph Relationship, with a variable path length.
 
+        :param label: The relationship label (type) in the DB, defaults to None
+        :type label: str
+        :param ref_name: A reference name to be used later in the rest of the query, defaults to None
+        :type ref_name: str
         :param min_hops: The minimal desired number of hops (set -1 for maximum boundary only), defaults to -1
         :type min_hops: int
         :param max_hops: The maximal desired number of hops (set -1 for minimal boundary only), defaults to -1
         :type max_hops: int
 
         :return: A Query object with a query that contains the new clause.
         :rtype: RelationAvailable
         """
         min_hops_str = '' if min_hops == -1 else str(min_hops)
         max_hops_str = '' if max_hops == -1 else str(max_hops)
 
+        relation_type = '' if label is None else f': {label}'
+        relation_ref_name = '' if ref_name is None else f'{ref_name}'
+
         relation_length = '*' if min_hops == -1 and max_hops == - \
             1 else (f'*{min_hops_str}'if min_hops == max_hops else f'*{min_hops_str}..{max_hops_str}')
 
         if relation_length:
-            realtion_str = f'[{relation_length}]'
+            realtion_str = f'[{relation_ref_name}{relation_type}{relation_length}]'
         else:
             realtion_str = ''
 
         return RelationAvailable(self.query + f'-{realtion_str}-')
 
     def _directed_relation(self, direction: str, label: str, ref_name: str = None, properties: dict = {}, **kwargs):
         """Concatenate a graph Relationship (private method).
@@ -524,33 +531,40 @@
         :type **kwargs
 
         :return: A Query object with a query that contains the new clause.
         :rtype: RelationAfterMergeAvailable
         """
         return RelationAvailable(self.query + self._directed_relation('backward', label, ref_name, properties, **kwargs))
 
-    def related_variable_len(self, min_hops: int = -1, max_hops: int = -1):
+    def related_variable_len(self, label: str = None, ref_name: str = None, min_hops: int = -1, max_hops: int = -1):
         """Concatenate a uni-directional graph Relationship, with a variable path length.
 
+        :param label: The relationship label (type) in the DB, defaults to None
+        :type label: str
+        :param ref_name: A reference name to be used later in the rest of the query, defaults to None
+        :type ref_name: str
         :param min_hops: The minimal desired number of hops (set -1 for maximum boundary only), defaults to -1
         :type min_hops: int
         :param max_hops: The maximal desired number of hops (set -1 for minimal boundary only), defaults to -1
         :type max_hops: int
 
         :return: A Query object with a query that contains the new clause.
         :rtype: RelationAfterMergeAvailable
         """
         min_hops_str = '' if min_hops == -1 else str(min_hops)
         max_hops_str = '' if max_hops == -1 else str(max_hops)
 
+        relation_type = '' if label is None else f': {label}'
+        relation_ref_name = '' if ref_name is None else f'{ref_name}'
+
         relation_length = '*' if min_hops == -1 and max_hops == - \
             1 else (f'*{min_hops_str}'if min_hops == max_hops else f'*{min_hops_str}..{max_hops_str}')
 
         if relation_length:
-            realtion_str = f'[{relation_length}]'
+            realtion_str = f'[{relation_ref_name}{relation_type}{relation_length}]'
         else:
             realtion_str = ''
 
         return RelationAvailable(self.query + f'-{realtion_str}-')
 
     def _directed_relation(self, direction: str, label: str, ref_name: str = None, properties: dict = {}, **kwargs):
         """Concatenate a graph Relationship (private method).
```

### Comparing `cymple-0.8.2/src/cymple/typedefs.py` & `cymple-0.9.0/src/cymple/typedefs.py`

 * *Files identical despite different names*

### Comparing `cymple-0.8.2/src/cymple.egg-info/PKG-INFO` & `cymple-0.9.0/src/cymple.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cymple
-Version: 0.8.2
+Version: 0.9.0
 Summary: A productivity enhancer for creating Cypher queries in Python
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8
 License-File: LICENSE
 
 # Cymple - Cypher Modular Pythonic Language Extension
```

