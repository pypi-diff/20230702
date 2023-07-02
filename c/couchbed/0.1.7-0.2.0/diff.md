# Comparing `tmp/couchbed-0.1.7.tar.gz` & `tmp/couchbed-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "couchbed-0.1.7.tar", last modified: Sun Jul  2 04:58:40 2023, max compression
+gzip compressed data, was "couchbed-0.2.0.tar", last modified: Sun Jul  2 08:19:41 2023, max compression
```

## Comparing `couchbed-0.1.7.tar` & `couchbed-0.2.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 shuntaro   (501) staff       (20)        0 2023-07-02 04:58:40.602012 couchbed-0.1.7/
--rw-r--r--   0 shuntaro   (501) staff       (20)     1075 2023-01-22 05:52:37.000000 couchbed-0.1.7/LICENSE.txt
--rw-r--r--   0 shuntaro   (501) staff       (20)        0 2023-07-01 01:19:19.000000 couchbed-0.1.7/MANIFEST.in
--rw-r--r--   0 shuntaro   (501) staff       (20)     2396 2023-07-02 04:58:40.602058 couchbed-0.1.7/PKG-INFO
--rw-r--r--   0 shuntaro   (501) staff       (20)     1930 2023-07-01 14:47:48.000000 couchbed-0.1.7/README.md
--rw-r--r--   0 shuntaro   (501) staff       (20)       94 2023-01-22 06:54:48.000000 couchbed-0.1.7/pyproject.toml
--rw-r--r--   0 shuntaro   (501) staff       (20)      564 2023-07-02 04:58:40.602283 couchbed-0.1.7/setup.cfg
--rw-r--r--   0 shuntaro   (501) staff       (20)       37 2022-12-09 19:04:39.000000 couchbed-0.1.7/setup.py
-drwxr-xr-x   0 shuntaro   (501) staff       (20)        0 2023-07-02 04:58:40.601317 couchbed-0.1.7/src/
--rw-r--r--   0 shuntaro   (501) staff       (20)       30 2023-07-01 02:56:33.000000 couchbed-0.1.7/src/__init__.py
-drwxr-xr-x   0 shuntaro   (501) staff       (20)        0 2023-07-02 04:58:40.601875 couchbed-0.1.7/src/couchbed.egg-info/
--rw-r--r--   0 shuntaro   (501) staff       (20)     2396 2023-07-02 04:58:40.000000 couchbed-0.1.7/src/couchbed.egg-info/PKG-INFO
--rw-r--r--   0 shuntaro   (501) staff       (20)      278 2023-07-02 04:58:40.000000 couchbed-0.1.7/src/couchbed.egg-info/SOURCES.txt
--rw-r--r--   0 shuntaro   (501) staff       (20)        1 2023-07-02 04:58:40.000000 couchbed-0.1.7/src/couchbed.egg-info/dependency_links.txt
--rw-r--r--   0 shuntaro   (501) staff       (20)       13 2023-07-02 04:58:40.000000 couchbed-0.1.7/src/couchbed.egg-info/requires.txt
--rw-r--r--   0 shuntaro   (501) staff       (20)       18 2023-07-02 04:58:40.000000 couchbed-0.1.7/src/couchbed.egg-info/top_level.txt
--rw-r--r--   0 shuntaro   (501) staff       (20)     4410 2023-07-02 04:58:17.000000 couchbed-0.1.7/src/couchbed.py
+drwxr-xr-x   0 shuntaro   (501) staff       (20)        0 2023-07-02 08:19:41.896069 couchbed-0.2.0/
+-rw-r--r--   0 shuntaro   (501) staff       (20)     1075 2023-01-22 05:52:37.000000 couchbed-0.2.0/LICENSE.txt
+-rw-r--r--   0 shuntaro   (501) staff       (20)        0 2023-07-01 01:19:19.000000 couchbed-0.2.0/MANIFEST.in
+-rw-r--r--   0 shuntaro   (501) staff       (20)     2396 2023-07-02 08:19:41.896128 couchbed-0.2.0/PKG-INFO
+-rw-r--r--   0 shuntaro   (501) staff       (20)     1930 2023-07-01 14:47:48.000000 couchbed-0.2.0/README.md
+-rw-r--r--   0 shuntaro   (501) staff       (20)       94 2023-01-22 06:54:48.000000 couchbed-0.2.0/pyproject.toml
+-rw-r--r--   0 shuntaro   (501) staff       (20)      564 2023-07-02 08:19:41.896366 couchbed-0.2.0/setup.cfg
+-rw-r--r--   0 shuntaro   (501) staff       (20)       37 2022-12-09 19:04:39.000000 couchbed-0.2.0/setup.py
+drwxr-xr-x   0 shuntaro   (501) staff       (20)        0 2023-07-02 08:19:41.895404 couchbed-0.2.0/src/
+-rw-r--r--   0 shuntaro   (501) staff       (20)       30 2023-07-01 02:56:33.000000 couchbed-0.2.0/src/__init__.py
+drwxr-xr-x   0 shuntaro   (501) staff       (20)        0 2023-07-02 08:19:41.895957 couchbed-0.2.0/src/couchbed.egg-info/
+-rw-r--r--   0 shuntaro   (501) staff       (20)     2396 2023-07-02 08:19:41.000000 couchbed-0.2.0/src/couchbed.egg-info/PKG-INFO
+-rw-r--r--   0 shuntaro   (501) staff       (20)      278 2023-07-02 08:19:41.000000 couchbed-0.2.0/src/couchbed.egg-info/SOURCES.txt
+-rw-r--r--   0 shuntaro   (501) staff       (20)        1 2023-07-02 08:19:41.000000 couchbed-0.2.0/src/couchbed.egg-info/dependency_links.txt
+-rw-r--r--   0 shuntaro   (501) staff       (20)       13 2023-07-02 08:19:41.000000 couchbed-0.2.0/src/couchbed.egg-info/requires.txt
+-rw-r--r--   0 shuntaro   (501) staff       (20)       18 2023-07-02 08:19:41.000000 couchbed-0.2.0/src/couchbed.egg-info/top_level.txt
+-rw-r--r--   0 shuntaro   (501) staff       (20)     4228 2023-07-02 08:17:28.000000 couchbed-0.2.0/src/couchbed.py
```

### Comparing `couchbed-0.1.7/LICENSE.txt` & `couchbed-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `couchbed-0.1.7/PKG-INFO` & `couchbed-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: couchbed
-Version: 0.1.7
+Version: 0.2.0
 Summary: Logging into CouchDB.
 Author: chocolate-icecream
 Keywords: CouchDB
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 4 - Beta
```

### Comparing `couchbed-0.1.7/README.md` & `couchbed-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `couchbed-0.1.7/setup.cfg` & `couchbed-0.2.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = couchbed
-version = 0.1.7
+version = 0.2.0
 author = chocolate-icecream
 description = Logging into CouchDB.
 long_description = file: README.md
 long_description_content_type = text/markdown
 classifiers = 
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
```

### Comparing `couchbed-0.1.7/src/couchbed.egg-info/PKG-INFO` & `couchbed-0.2.0/src/couchbed.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: couchbed
-Version: 0.1.7
+Version: 0.2.0
 Summary: Logging into CouchDB.
 Author: chocolate-icecream
 Keywords: CouchDB
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 4 - Beta
```

### Comparing `couchbed-0.1.7/src/couchbed.py` & `couchbed-0.2.0/src/couchbed.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,25 +35,25 @@
         if self.couch is None:
             return
         t = threading.Timer(self.SAVE_PERIOD, self.periodic_task)
         t.daemon = True
         t.start()
         try:
             self.save()
-        except:
+        except Exception as e:
+            print(f"Exception: {e}")
             pass
 
     def save(self):
         if self.couch is None:
             return
-        for book_id, book in self.books.items():
+        for book in self.books.values():
             if not book.write_flag:
                 continue
-            self.db[book_id] = book.content
-            self.db.save(self.db[book_id])
+            self.db.save(book.content)
             book.write_flag = False
 
     @property
     def time_str(self):
         return datetime.datetime.now().strftime("%y-%m-%d %H-%M-%S")
     
     @property
@@ -63,64 +63,65 @@
 class CBBook:
     def __init__(self, cbed, book_id):
         self.cbed = cbed
         self.book_id = book_id
         self.stopwatch_dict = {"startup": time.time()}
         self.log_dict = {}
         self.write_flag = False
-        self.content = {"msg": [], "log": [], "setting": {}, "created": self.cbed.iso_time_str, "last_updated": self.cbed.iso_time_str, "result": {}}
+        cbed.db[book_id] = {"msg": [], "log": [], "setting": {}, "created": self.cbed.iso_time_str, "last_updated": self.cbed.iso_time_str, "result": {}}
+        self.content = cbed.db[book_id]
 
     def __call__(self, *args):
         self.message(" ".join([f"{x}" for x in args]))
 
     def message(self, msg):
         time_stamped_msg = self.cbed.time_str +": "+ msg
         self.content["msg"].append(time_stamped_msg)
-        self.write_flag = True
-        self.content["last_updated"] = self.cbed.iso_time_str
+        self._updated()
         print(time_stamped_msg)
     
     def start_stopwatch(self, watch_name):
         self.stopwatch_dict[watch_name] = time.time()
 
     def record_stopwatch(self, watch_name="startup", msg=None):
         if watch_name in self.stopwatch_dict:
             dt = time.time() - self.stopwatch_dict[watch_name]
             self.message(f"{watch_name} -> {dt} {f'({msg})' if msg is not None else ''}")
     
     def set(self, setting_dict):
         self.content["setting"].update(self.sanitize(setting_dict))
-        self.write_flag = True
-        self.content["last_updated"] = self.cbed.iso_time_str
+        self._updated()
 
     def __setitem__(self, key, value):
         self.content["setting"][key] = self.sanitize(value)
-        self.write_flag = True
-        self.content["last_updated"] = self.cbed.iso_time_str
+        self._updated()
 
     def __getitem__(self, key):
         if key in self.content["setting"]:
             return self.content["setting"][key]
         return None
 
     def log(self, log_dict):
         log_dict = self.sanitize(log_dict)
         log_dict["_time"] = self.cbed.iso_time_str
         self.content["log"].append(log_dict)
+        self._updated()
         print(", ".join([f"{key}:{value}" for key, value in log_dict.items()]))
+        
+
+    
+    def _updated(self):
         self.content["last_updated"] = self.cbed.iso_time_str
         self.write_flag = True
-        
     
     def result(self, result_dict):
         result_dict = self.sanitize(result_dict)
         result_dict["_time"] = self.cbed.iso_time_str
         self.content["result"].update(result_dict)
-        self.content["last_updated"] = self.cbed.iso_time_str
-        self.write_flag = True
+        self._updated()
         
 
     def save(self):
         self.cbed.save()
 
     def sanitize(self, value):
         if isinstance(value, (str, float, int)):
```

