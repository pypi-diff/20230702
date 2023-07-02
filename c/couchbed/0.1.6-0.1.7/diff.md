# Comparing `tmp/couchbed-0.1.6.tar.gz` & `tmp/couchbed-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "couchbed-0.1.6.tar", last modified: Sun Jul  2 04:53:24 2023, max compression
+gzip compressed data, was "couchbed-0.1.7.tar", last modified: Sun Jul  2 04:58:40 2023, max compression
```

## Comparing `couchbed-0.1.6.tar` & `couchbed-0.1.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 shuntaro   (501) staff       (20)        0 2023-07-02 04:53:24.090433 couchbed-0.1.6/
--rw-r--r--   0 shuntaro   (501) staff       (20)     1075 2023-01-22 05:52:37.000000 couchbed-0.1.6/LICENSE.txt
--rw-r--r--   0 shuntaro   (501) staff       (20)        0 2023-07-01 01:19:19.000000 couchbed-0.1.6/MANIFEST.in
--rw-r--r--   0 shuntaro   (501) staff       (20)     2396 2023-07-02 04:53:24.090481 couchbed-0.1.6/PKG-INFO
--rw-r--r--   0 shuntaro   (501) staff       (20)     1930 2023-07-01 14:47:48.000000 couchbed-0.1.6/README.md
--rw-r--r--   0 shuntaro   (501) staff       (20)       94 2023-01-22 06:54:48.000000 couchbed-0.1.6/pyproject.toml
--rw-r--r--   0 shuntaro   (501) staff       (20)      564 2023-07-02 04:53:24.090717 couchbed-0.1.6/setup.cfg
--rw-r--r--   0 shuntaro   (501) staff       (20)       37 2022-12-09 19:04:39.000000 couchbed-0.1.6/setup.py
-drwxr-xr-x   0 shuntaro   (501) staff       (20)        0 2023-07-02 04:53:24.089748 couchbed-0.1.6/src/
--rw-r--r--   0 shuntaro   (501) staff       (20)       30 2023-07-01 02:56:33.000000 couchbed-0.1.6/src/__init__.py
-drwxr-xr-x   0 shuntaro   (501) staff       (20)        0 2023-07-02 04:53:24.090337 couchbed-0.1.6/src/couchbed.egg-info/
--rw-r--r--   0 shuntaro   (501) staff       (20)     2396 2023-07-02 04:53:24.000000 couchbed-0.1.6/src/couchbed.egg-info/PKG-INFO
--rw-r--r--   0 shuntaro   (501) staff       (20)      278 2023-07-02 04:53:24.000000 couchbed-0.1.6/src/couchbed.egg-info/SOURCES.txt
--rw-r--r--   0 shuntaro   (501) staff       (20)        1 2023-07-02 04:53:24.000000 couchbed-0.1.6/src/couchbed.egg-info/dependency_links.txt
--rw-r--r--   0 shuntaro   (501) staff       (20)       13 2023-07-02 04:53:24.000000 couchbed-0.1.6/src/couchbed.egg-info/requires.txt
--rw-r--r--   0 shuntaro   (501) staff       (20)       18 2023-07-02 04:53:24.000000 couchbed-0.1.6/src/couchbed.egg-info/top_level.txt
--rw-r--r--   0 shuntaro   (501) staff       (20)     4366 2023-07-02 04:53:01.000000 couchbed-0.1.6/src/couchbed.py
+drwxr-xr-x   0 shuntaro   (501) staff       (20)        0 2023-07-02 04:58:40.602012 couchbed-0.1.7/
+-rw-r--r--   0 shuntaro   (501) staff       (20)     1075 2023-01-22 05:52:37.000000 couchbed-0.1.7/LICENSE.txt
+-rw-r--r--   0 shuntaro   (501) staff       (20)        0 2023-07-01 01:19:19.000000 couchbed-0.1.7/MANIFEST.in
+-rw-r--r--   0 shuntaro   (501) staff       (20)     2396 2023-07-02 04:58:40.602058 couchbed-0.1.7/PKG-INFO
+-rw-r--r--   0 shuntaro   (501) staff       (20)     1930 2023-07-01 14:47:48.000000 couchbed-0.1.7/README.md
+-rw-r--r--   0 shuntaro   (501) staff       (20)       94 2023-01-22 06:54:48.000000 couchbed-0.1.7/pyproject.toml
+-rw-r--r--   0 shuntaro   (501) staff       (20)      564 2023-07-02 04:58:40.602283 couchbed-0.1.7/setup.cfg
+-rw-r--r--   0 shuntaro   (501) staff       (20)       37 2022-12-09 19:04:39.000000 couchbed-0.1.7/setup.py
+drwxr-xr-x   0 shuntaro   (501) staff       (20)        0 2023-07-02 04:58:40.601317 couchbed-0.1.7/src/
+-rw-r--r--   0 shuntaro   (501) staff       (20)       30 2023-07-01 02:56:33.000000 couchbed-0.1.7/src/__init__.py
+drwxr-xr-x   0 shuntaro   (501) staff       (20)        0 2023-07-02 04:58:40.601875 couchbed-0.1.7/src/couchbed.egg-info/
+-rw-r--r--   0 shuntaro   (501) staff       (20)     2396 2023-07-02 04:58:40.000000 couchbed-0.1.7/src/couchbed.egg-info/PKG-INFO
+-rw-r--r--   0 shuntaro   (501) staff       (20)      278 2023-07-02 04:58:40.000000 couchbed-0.1.7/src/couchbed.egg-info/SOURCES.txt
+-rw-r--r--   0 shuntaro   (501) staff       (20)        1 2023-07-02 04:58:40.000000 couchbed-0.1.7/src/couchbed.egg-info/dependency_links.txt
+-rw-r--r--   0 shuntaro   (501) staff       (20)       13 2023-07-02 04:58:40.000000 couchbed-0.1.7/src/couchbed.egg-info/requires.txt
+-rw-r--r--   0 shuntaro   (501) staff       (20)       18 2023-07-02 04:58:40.000000 couchbed-0.1.7/src/couchbed.egg-info/top_level.txt
+-rw-r--r--   0 shuntaro   (501) staff       (20)     4410 2023-07-02 04:58:17.000000 couchbed-0.1.7/src/couchbed.py
```

### Comparing `couchbed-0.1.6/LICENSE.txt` & `couchbed-0.1.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `couchbed-0.1.6/PKG-INFO` & `couchbed-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: couchbed
-Version: 0.1.6
+Version: 0.1.7
 Summary: Logging into CouchDB.
 Author: chocolate-icecream
 Keywords: CouchDB
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 4 - Beta
```

### Comparing `couchbed-0.1.6/README.md` & `couchbed-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `couchbed-0.1.6/setup.cfg` & `couchbed-0.1.7/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = couchbed
-version = 0.1.6
+version = 0.1.7
 author = chocolate-icecream
 description = Logging into CouchDB.
 long_description = file: README.md
 long_description_content_type = text/markdown
 classifiers = 
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
```

### Comparing `couchbed-0.1.6/src/couchbed.egg-info/PKG-INFO` & `couchbed-0.1.7/src/couchbed.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: couchbed
-Version: 0.1.6
+Version: 0.1.7
 Summary: Logging into CouchDB.
 Author: chocolate-icecream
 Keywords: CouchDB
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 4 - Beta
```

### Comparing `couchbed-0.1.6/src/couchbed.py` & `couchbed-0.1.7/src/couchbed.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 
         self.periodic_task()
     
     def new_book(self):
         if self.couch is None:
             return dict()
         book_id = self.time_str + " " + ''.join(random.choices(string.ascii_lowercase, k=3))
+        book_id = book_id.replace(" ", "_")
         book = CBBook(self, book_id=book_id)
         self.books[book_id] = book
         return book
     
     def get_list(self):
         pass
```

