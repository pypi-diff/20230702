# Comparing `tmp/couchbed-0.1.5.tar.gz` & `tmp/couchbed-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "couchbed-0.1.5.tar", last modified: Sat Jul  1 21:45:54 2023, max compression
+gzip compressed data, was "couchbed-0.1.6.tar", last modified: Sun Jul  2 04:53:24 2023, max compression
```

## Comparing `couchbed-0.1.5.tar` & `couchbed-0.1.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 shuntaro   (501) staff       (20)        0 2023-07-01 21:45:54.106412 couchbed-0.1.5/
--rw-r--r--   0 shuntaro   (501) staff       (20)     1075 2023-01-22 05:52:37.000000 couchbed-0.1.5/LICENSE.txt
--rw-r--r--   0 shuntaro   (501) staff       (20)        0 2023-07-01 01:19:19.000000 couchbed-0.1.5/MANIFEST.in
--rw-r--r--   0 shuntaro   (501) staff       (20)     2396 2023-07-01 21:45:54.106455 couchbed-0.1.5/PKG-INFO
--rw-r--r--   0 shuntaro   (501) staff       (20)     1930 2023-07-01 14:47:48.000000 couchbed-0.1.5/README.md
--rw-r--r--   0 shuntaro   (501) staff       (20)       94 2023-01-22 06:54:48.000000 couchbed-0.1.5/pyproject.toml
--rw-r--r--   0 shuntaro   (501) staff       (20)      564 2023-07-01 21:45:54.106730 couchbed-0.1.5/setup.cfg
--rw-r--r--   0 shuntaro   (501) staff       (20)       37 2022-12-09 19:04:39.000000 couchbed-0.1.5/setup.py
-drwxr-xr-x   0 shuntaro   (501) staff       (20)        0 2023-07-01 21:45:54.105766 couchbed-0.1.5/src/
--rw-r--r--   0 shuntaro   (501) staff       (20)       30 2023-07-01 02:56:33.000000 couchbed-0.1.5/src/__init__.py
-drwxr-xr-x   0 shuntaro   (501) staff       (20)        0 2023-07-01 21:45:54.106316 couchbed-0.1.5/src/couchbed.egg-info/
--rw-r--r--   0 shuntaro   (501) staff       (20)     2396 2023-07-01 21:45:54.000000 couchbed-0.1.5/src/couchbed.egg-info/PKG-INFO
--rw-r--r--   0 shuntaro   (501) staff       (20)      278 2023-07-01 21:45:54.000000 couchbed-0.1.5/src/couchbed.egg-info/SOURCES.txt
--rw-r--r--   0 shuntaro   (501) staff       (20)        1 2023-07-01 21:45:54.000000 couchbed-0.1.5/src/couchbed.egg-info/dependency_links.txt
--rw-r--r--   0 shuntaro   (501) staff       (20)       13 2023-07-01 21:45:54.000000 couchbed-0.1.5/src/couchbed.egg-info/requires.txt
--rw-r--r--   0 shuntaro   (501) staff       (20)       18 2023-07-01 21:45:54.000000 couchbed-0.1.5/src/couchbed.egg-info/top_level.txt
--rw-r--r--   0 shuntaro   (501) staff       (20)     4362 2023-07-01 21:45:34.000000 couchbed-0.1.5/src/couchbed.py
+drwxr-xr-x   0 shuntaro   (501) staff       (20)        0 2023-07-02 04:53:24.090433 couchbed-0.1.6/
+-rw-r--r--   0 shuntaro   (501) staff       (20)     1075 2023-01-22 05:52:37.000000 couchbed-0.1.6/LICENSE.txt
+-rw-r--r--   0 shuntaro   (501) staff       (20)        0 2023-07-01 01:19:19.000000 couchbed-0.1.6/MANIFEST.in
+-rw-r--r--   0 shuntaro   (501) staff       (20)     2396 2023-07-02 04:53:24.090481 couchbed-0.1.6/PKG-INFO
+-rw-r--r--   0 shuntaro   (501) staff       (20)     1930 2023-07-01 14:47:48.000000 couchbed-0.1.6/README.md
+-rw-r--r--   0 shuntaro   (501) staff       (20)       94 2023-01-22 06:54:48.000000 couchbed-0.1.6/pyproject.toml
+-rw-r--r--   0 shuntaro   (501) staff       (20)      564 2023-07-02 04:53:24.090717 couchbed-0.1.6/setup.cfg
+-rw-r--r--   0 shuntaro   (501) staff       (20)       37 2022-12-09 19:04:39.000000 couchbed-0.1.6/setup.py
+drwxr-xr-x   0 shuntaro   (501) staff       (20)        0 2023-07-02 04:53:24.089748 couchbed-0.1.6/src/
+-rw-r--r--   0 shuntaro   (501) staff       (20)       30 2023-07-01 02:56:33.000000 couchbed-0.1.6/src/__init__.py
+drwxr-xr-x   0 shuntaro   (501) staff       (20)        0 2023-07-02 04:53:24.090337 couchbed-0.1.6/src/couchbed.egg-info/
+-rw-r--r--   0 shuntaro   (501) staff       (20)     2396 2023-07-02 04:53:24.000000 couchbed-0.1.6/src/couchbed.egg-info/PKG-INFO
+-rw-r--r--   0 shuntaro   (501) staff       (20)      278 2023-07-02 04:53:24.000000 couchbed-0.1.6/src/couchbed.egg-info/SOURCES.txt
+-rw-r--r--   0 shuntaro   (501) staff       (20)        1 2023-07-02 04:53:24.000000 couchbed-0.1.6/src/couchbed.egg-info/dependency_links.txt
+-rw-r--r--   0 shuntaro   (501) staff       (20)       13 2023-07-02 04:53:24.000000 couchbed-0.1.6/src/couchbed.egg-info/requires.txt
+-rw-r--r--   0 shuntaro   (501) staff       (20)       18 2023-07-02 04:53:24.000000 couchbed-0.1.6/src/couchbed.egg-info/top_level.txt
+-rw-r--r--   0 shuntaro   (501) staff       (20)     4366 2023-07-02 04:53:01.000000 couchbed-0.1.6/src/couchbed.py
```

### Comparing `couchbed-0.1.5/LICENSE.txt` & `couchbed-0.1.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `couchbed-0.1.5/PKG-INFO` & `couchbed-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: couchbed
-Version: 0.1.5
+Version: 0.1.6
 Summary: Logging into CouchDB.
 Author: chocolate-icecream
 Keywords: CouchDB
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 4 - Beta
```

### Comparing `couchbed-0.1.5/README.md` & `couchbed-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `couchbed-0.1.5/setup.cfg` & `couchbed-0.1.6/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = couchbed
-version = 0.1.5
+version = 0.1.6
 author = chocolate-icecream
 description = Logging into CouchDB.
 long_description = file: README.md
 long_description_content_type = text/markdown
 classifiers = 
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
```

### Comparing `couchbed-0.1.5/src/couchbed.egg-info/PKG-INFO` & `couchbed-0.1.6/src/couchbed.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: couchbed
-Version: 0.1.5
+Version: 0.1.6
 Summary: Logging into CouchDB.
 Author: chocolate-icecream
 Keywords: CouchDB
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 4 - Beta
```

### Comparing `couchbed-0.1.5/src/couchbed.py` & `couchbed-0.1.6/src/couchbed.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
     def save(self):
         if self.couch is None:
             return
         for book_id, book in self.books.items():
             if not book.write_flag:
                 continue
             self.db[book_id] = book.content
-            self.db.save(self.content)
+            self.db.save(self.db[book_id])
             book.write_flag = False
 
     @property
     def time_str(self):
         return datetime.datetime.now().strftime("%y-%m-%d %H-%M-%S")
     
     @property
```

