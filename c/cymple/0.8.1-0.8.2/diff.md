# Comparing `tmp/cymple-0.8.1.tar.gz` & `tmp/cymple-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cymple-0.8.1.tar", last modified: Wed May 17 08:19:35 2023, max compression
+gzip compressed data, was "cymple-0.8.2.tar", last modified: Sun Jul  2 08:17:03 2023, max compression
```

## Comparing `cymple-0.8.1.tar` & `cymple-0.8.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 08:19:35.969019 cymple-0.8.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-17 08:19:21.000000 cymple-0.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7465 2023-05-17 08:19:35.969019 cymple-0.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7445 2023-05-17 08:19:21.000000 cymple-0.8.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-17 08:19:21.000000 cymple-0.8.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-17 08:19:35.969019 cymple-0.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-17 08:19:21.000000 cymple-0.8.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 08:19:35.969019 cymple-0.8.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 08:19:35.969019 cymple-0.8.1/src/cymple/
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-17 08:19:21.000000 cymple-0.8.1/src/cymple/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-17 08:19:21.000000 cymple-0.8.1/src/cymple/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36687 2023-05-17 08:19:21.000000 cymple-0.8.1/src/cymple/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-05-17 08:19:21.000000 cymple-0.8.1/src/cymple/typedefs.py
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-17 08:19:21.000000 cymple-0.8.1/src/cymple/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 08:19:35.969019 cymple-0.8.1/src/cymple.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7465 2023-05-17 08:19:35.000000 cymple-0.8.1/src/cymple.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-17 08:19:35.000000 cymple-0.8.1/src/cymple.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 08:19:35.000000 cymple-0.8.1/src/cymple.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-17 08:19:35.000000 cymple-0.8.1/src/cymple.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 08:17:03.969011 cymple-0.8.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-02 08:16:50.000000 cymple-0.8.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7465 2023-07-02 08:17:03.969011 cymple-0.8.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7445 2023-07-02 08:16:50.000000 cymple-0.8.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-02 08:16:50.000000 cymple-0.8.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-02 08:17:03.969011 cymple-0.8.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-02 08:16:50.000000 cymple-0.8.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 08:17:03.965011 cymple-0.8.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 08:17:03.969011 cymple-0.8.2/src/cymple/
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-02 08:16:50.000000 cymple-0.8.2/src/cymple/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-02 08:16:50.000000 cymple-0.8.2/src/cymple/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36959 2023-07-02 08:16:50.000000 cymple-0.8.2/src/cymple/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-07-02 08:16:50.000000 cymple-0.8.2/src/cymple/typedefs.py
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-02 08:16:50.000000 cymple-0.8.2/src/cymple/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 08:17:03.969011 cymple-0.8.2/src/cymple.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7465 2023-07-02 08:17:03.000000 cymple-0.8.2/src/cymple.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-02 08:17:03.000000 cymple-0.8.2/src/cymple.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 08:17:03.000000 cymple-0.8.2/src/cymple.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-02 08:17:03.000000 cymple-0.8.2/src/cymple.egg-info/top_level.txt
```

### Comparing `cymple-0.8.1/LICENSE` & `cymple-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cymple-0.8.1/PKG-INFO` & `cymple-0.8.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cymple
-Version: 0.8.1
+Version: 0.8.2
 Summary: A productivity enhancer for creating Cypher queries in Python
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8
 License-File: LICENSE
 
 # Cymple - Cypher Modular Pythonic Language Extension
```

### Comparing `cymple-0.8.1/README.md` & `cymple-0.8.2/README.md`

 * *Files identical despite different names*

### Comparing `cymple-0.8.1/setup.cfg` & `cymple-0.8.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `cymple-0.8.1/src/cymple/builder.py` & `cymple-0.8.2/src/cymple/builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -652,15 +652,20 @@
         :type properties: dict
         :param escape_values: Determines whether the properties values should be escaped or not, defaults to True
         :type escape_values: bool
 
         :return: A Query object with a query that contains the new clause.
         :rtype: SetAvailable
         """
-        query = self.query + ' SET ' + Properties(properties).to_str("=", ", ", escape_values)
+        if isinstance(properties, dict):
+            _properties = Properties(properties).to_str("=", ", ", escape_values)
+        else:
+            _properties = str(properties)
+
+        query = self.query + ' SET ' + _properties
 
         if isinstance(self, NodeAfterMergeAvailable) or isinstance(self, OnCreateAvailable) or isinstance(self, OnMatchAvailable) or isinstance(self, SetAfterMergeAvailable):
             return SetAfterMergeAvailable(query)
 
         return SetAvailable(query)
 
 
@@ -674,15 +679,20 @@
         :type properties: dict
         :param escape_values: Determines whether the properties values should be escaped or not, defaults to True
         :type escape_values: bool
 
         :return: A Query object with a query that contains the new clause.
         :rtype: SetAfterMergeAvailable
         """
-        query = self.query + ' SET ' + Properties(properties).to_str("=", ", ", escape_values)
+        if isinstance(properties, dict):
+            _properties = Properties(properties).to_str("=", ", ", escape_values)
+        else:
+            _properties = str(properties)
+
+        query = self.query + ' SET ' + _properties
 
         if isinstance(self, NodeAfterMergeAvailable) or isinstance(self, OnCreateAvailable) or isinstance(self, OnMatchAvailable) or isinstance(self, SetAfterMergeAvailable):
             return SetAfterMergeAvailable(query)
 
         return SetAvailable(query)
```

### Comparing `cymple-0.8.1/src/cymple/typedefs.py` & `cymple-0.8.2/src/cymple/typedefs.py`

 * *Files identical despite different names*

### Comparing `cymple-0.8.1/src/cymple.egg-info/PKG-INFO` & `cymple-0.8.2/src/cymple.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cymple
-Version: 0.8.1
+Version: 0.8.2
 Summary: A productivity enhancer for creating Cypher queries in Python
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8
 License-File: LICENSE
 
 # Cymple - Cypher Modular Pythonic Language Extension
```

