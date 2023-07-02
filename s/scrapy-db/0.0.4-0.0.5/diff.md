# Comparing `tmp/scrapy_db-0.0.4.tar.gz` & `tmp/scrapy_db-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrapy_db-0.0.4.tar", max compression
+gzip compressed data, was "scrapy_db-0.0.5.tar", max compression
```

## Comparing `scrapy_db-0.0.4.tar` & `scrapy_db-0.0.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    35149 2023-06-29 01:32:10.048413 scrapy_db-0.0.4/LICENSE
--rw-r--r--   0        0        0     1759 2023-06-29 01:32:10.048413 scrapy_db-0.0.4/README.md
--rw-r--r--   0        0        0     1216 2023-06-29 01:32:10.048413 scrapy_db-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      107 2023-06-29 01:32:10.048413 scrapy_db-0.0.4/scrapy_db/__init__.py
--rw-r--r--   0        0        0     5202 2023-06-29 01:32:10.048413 scrapy_db-0.0.4/scrapy_db/db.py
--rw-r--r--   0        0        0      475 2023-06-29 01:32:10.048413 scrapy_db-0.0.4/scrapy_db/defaults.py
--rw-r--r--   0        0        0     3258 2023-06-29 01:32:10.048413 scrapy_db-0.0.4/scrapy_db/dupefilter.py
--rw-r--r--   0        0        0     2490 2023-06-29 01:32:10.048413 scrapy_db-0.0.4/scrapy_db/queue.py
--rw-r--r--   0        0        0     4381 2023-06-29 01:32:10.048413 scrapy_db-0.0.4/scrapy_db/scheduler.py
--rw-r--r--   0        0        0     4705 2023-06-29 01:32:10.048413 scrapy_db-0.0.4/scrapy_db/spiders.py
--rw-r--r--   0        0        0     1089 2023-06-29 01:32:10.048413 scrapy_db-0.0.4/scrapy_db/utils.py
--rw-r--r--   0        0        0     2851 1970-01-01 00:00:00.000000 scrapy_db-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-02 10:38:22.498935 scrapy_db-0.0.5/LICENSE
+-rw-r--r--   0        0        0     1759 2023-07-02 10:38:22.498935 scrapy_db-0.0.5/README.md
+-rw-r--r--   0        0        0     1216 2023-07-02 10:38:22.502935 scrapy_db-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      107 2023-07-02 10:38:22.502935 scrapy_db-0.0.5/scrapy_db/__init__.py
+-rw-r--r--   0        0        0     5202 2023-07-02 10:38:22.502935 scrapy_db-0.0.5/scrapy_db/db.py
+-rw-r--r--   0        0        0      475 2023-07-02 10:38:22.502935 scrapy_db-0.0.5/scrapy_db/defaults.py
+-rw-r--r--   0        0        0     3285 2023-07-02 10:38:22.502935 scrapy_db-0.0.5/scrapy_db/dupefilter.py
+-rw-r--r--   0        0        0     2490 2023-07-02 10:38:22.502935 scrapy_db-0.0.5/scrapy_db/queue.py
+-rw-r--r--   0        0        0     4381 2023-07-02 10:38:22.502935 scrapy_db-0.0.5/scrapy_db/scheduler.py
+-rw-r--r--   0        0        0     4705 2023-07-02 10:38:22.502935 scrapy_db-0.0.5/scrapy_db/spiders.py
+-rw-r--r--   0        0        0     1089 2023-07-02 10:38:22.502935 scrapy_db-0.0.5/scrapy_db/utils.py
+-rw-r--r--   0        0        0     2851 1970-01-01 00:00:00.000000 scrapy_db-0.0.5/PKG-INFO
```

### Comparing `scrapy_db-0.0.4/LICENSE` & `scrapy_db-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `scrapy_db-0.0.4/README.md` & `scrapy_db-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `scrapy_db-0.0.4/pyproject.toml` & `scrapy_db-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "scrapy-db"
-version = "0.0.4"
+version = "0.0.5"
 description = "Similar to [scrapy-redis](https://github.com/rmax/scrapy-redis), using the database as a queue, database-based scrapy components."
 authors = ["libra146 <shumeipai146@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "scrapy_db" }]
 license = "GPL-3.0-only"
 homepage = "https://github.com/libra146/scrapy-db/blob/main/README.md"
 repository = "https://github.com/libra146/scrapy-db"
```

### Comparing `scrapy_db-0.0.4/scrapy_db/db.py` & `scrapy_db-0.0.5/scrapy_db/db.py`

 * *Files identical despite different names*

### Comparing `scrapy_db-0.0.4/scrapy_db/dupefilter.py` & `scrapy_db-0.0.5/scrapy_db/dupefilter.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,16 @@
 
         :param request: Request object
         :return: Whether the request has been made
         """
         # request_fingerprint remove warnings
         fp = fingerprint(request).hex()
         added = self.table.db.select().where(self.table.db.key_ == fp).count()
-        self.table.push(**{'key_': fp})
+        if added == 0:
+            self.table.push(**{'key_': fp})
         return added != 0
 
     @classmethod
     def from_spider(cls, spider):
         """
         Create an instance through spider
```

### Comparing `scrapy_db-0.0.4/scrapy_db/queue.py` & `scrapy_db-0.0.5/scrapy_db/queue.py`

 * *Files identical despite different names*

### Comparing `scrapy_db-0.0.4/scrapy_db/scheduler.py` & `scrapy_db-0.0.5/scrapy_db/scheduler.py`

 * *Files identical despite different names*

### Comparing `scrapy_db-0.0.4/scrapy_db/spiders.py` & `scrapy_db-0.0.5/scrapy_db/spiders.py`

 * *Files identical despite different names*

### Comparing `scrapy_db-0.0.4/scrapy_db/utils.py` & `scrapy_db-0.0.5/scrapy_db/utils.py`

 * *Files identical despite different names*

### Comparing `scrapy_db-0.0.4/PKG-INFO` & `scrapy_db-0.0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapy-db
-Version: 0.0.4
+Version: 0.0.5
 Summary: Similar to [scrapy-redis](https://github.com/rmax/scrapy-redis), using the database as a queue, database-based scrapy components.
 Home-page: https://github.com/libra146/scrapy-db/blob/main/README.md
 License: GPL-3.0-only
 Author: libra146
 Author-email: shumeipai146@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

