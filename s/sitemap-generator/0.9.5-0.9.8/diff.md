# Comparing `tmp/sitemap-generator-0.9.5.tar.gz` & `tmp/sitemap-generator-0.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\sitemap-generator-0.9.5.tar", last modified: Wed Mar 24 07:41:17 2021, max compression
+gzip compressed data, was "dist\sitemap-generator-0.9.8.tar", last modified: Wed Apr 14 08:39:02 2021, max compression
```

## Comparing `sitemap-generator-0.9.5.tar` & `sitemap-generator-0.9.8.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2021-03-24 07:41:17.138801 sitemap-generator-0.9.5/
--rw-rw-rw-   0        0        0    11547 2021-03-24 07:06:43.000000 sitemap-generator-0.9.5/LICENSE
--rw-rw-rw-   0        0        0       97 2021-03-24 07:20:47.000000 sitemap-generator-0.9.5/MANIFEST.in
--rw-rw-rw-   0        0        0      607 2021-03-24 07:06:43.000000 sitemap-generator-0.9.5/NOTICE
--rw-rw-rw-   0        0        0     2948 2021-03-24 07:41:17.136792 sitemap-generator-0.9.5/PKG-INFO
--rw-rw-rw-   0        0        0     1559 2021-03-24 07:06:43.000000 sitemap-generator-0.9.5/README.rst
-drwxrwxrwx   0        0        0        0 2021-03-24 07:41:17.095677 sitemap-generator-0.9.5/pysitemap/
--rw-rw-rw-   0        0        0      819 2021-03-24 07:06:43.000000 sitemap-generator-0.9.5/pysitemap/__init__.py
-drwxrwxrwx   0        0        0        0 2021-03-24 07:41:17.098675 sitemap-generator-0.9.5/pysitemap/backends/
--rw-rw-rw-   0        0        0        0 2021-03-24 07:06:43.000000 sitemap-generator-0.9.5/pysitemap/backends/__init__.py
--rw-rw-rw-   0        0        0     2395 2021-03-24 07:06:43.000000 sitemap-generator-0.9.5/pysitemap/backends/sqlite_todo.py
--rw-rw-rw-   0        0        0     4010 2021-03-24 07:06:43.000000 sitemap-generator-0.9.5/pysitemap/base_crawler.py
--rw-rw-rw-   0        0        0      889 2021-03-24 07:06:43.000000 sitemap-generator-0.9.5/pysitemap/db.py
-drwxrwxrwx   0        0        0        0 2021-03-24 07:41:17.103676 sitemap-generator-0.9.5/pysitemap/format_processors/
--rw-rw-rw-   0        0        0        0 2021-03-24 07:06:43.000000 sitemap-generator-0.9.5/pysitemap/format_processors/__init__.py
--rw-rw-rw-   0        0        0      425 2021-03-24 07:06:43.000000 sitemap-generator-0.9.5/pysitemap/format_processors/text.py
--rw-rw-rw-   0        0        0      946 2021-03-24 07:06:43.000000 sitemap-generator-0.9.5/pysitemap/format_processors/xml.py
--rw-rw-rw-   0        0        0     2400 2021-03-24 07:06:43.000000 sitemap-generator-0.9.5/pysitemap/models.py
--rw-rw-rw-   0        0        0     4878 2021-03-24 07:06:43.000000 sitemap-generator-0.9.5/pysitemap/rest.py
--rw-rw-rw-   0        0        0     1206 2021-03-24 07:06:43.000000 sitemap-generator-0.9.5/pysitemap/validators.py
--rw-rw-rw-   0        0        0       25 2021-03-24 07:06:43.000000 sitemap-generator-0.9.5/requirements.txt
--rw-rw-rw-   0        0        0       42 2021-03-24 07:41:17.138801 sitemap-generator-0.9.5/setup.cfg
--rw-rw-rw-   0        0        0     1435 2021-03-24 07:06:43.000000 sitemap-generator-0.9.5/setup.py
-drwxrwxrwx   0        0        0        0 2021-03-24 07:41:17.134795 sitemap-generator-0.9.5/sitemap_generator.egg-info/
--rw-rw-rw-   0        0        0     2948 2021-03-24 07:41:16.000000 sitemap-generator-0.9.5/sitemap_generator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      580 2021-03-24 07:41:16.000000 sitemap-generator-0.9.5/sitemap_generator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-03-24 07:41:16.000000 sitemap-generator-0.9.5/sitemap_generator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2021-03-24 07:41:16.000000 sitemap-generator-0.9.5/sitemap_generator.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2021-03-24 07:41:16.000000 sitemap-generator-0.9.5/sitemap_generator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       17 2021-03-24 07:41:07.000000 sitemap-generator-0.9.5/version.py
+drwxrwxrwx   0        0        0        0 2021-04-14 08:39:02.763602 sitemap-generator-0.9.8/
+-rw-rw-rw-   0        0        0    11547 2021-03-24 07:06:43.000000 sitemap-generator-0.9.8/LICENSE
+-rw-rw-rw-   0        0        0       97 2021-03-24 07:20:47.000000 sitemap-generator-0.9.8/MANIFEST.in
+-rw-rw-rw-   0        0        0      607 2021-03-24 07:06:43.000000 sitemap-generator-0.9.8/NOTICE
+-rw-rw-rw-   0        0        0     3333 2021-04-14 08:39:02.762602 sitemap-generator-0.9.8/PKG-INFO
+-rw-rw-rw-   0        0        0     1872 2021-04-14 08:23:23.000000 sitemap-generator-0.9.8/README.rst
+drwxrwxrwx   0        0        0        0 2021-04-14 08:39:02.685599 sitemap-generator-0.9.8/pysitemap/
+-rw-rw-rw-   0        0        0      987 2021-04-14 08:23:22.000000 sitemap-generator-0.9.8/pysitemap/__init__.py
+drwxrwxrwx   0        0        0        0 2021-04-14 08:39:02.689603 sitemap-generator-0.9.8/pysitemap/backends/
+-rw-rw-rw-   0        0        0        0 2021-03-24 07:06:43.000000 sitemap-generator-0.9.8/pysitemap/backends/__init__.py
+-rw-rw-rw-   0        0        0     2395 2021-03-24 07:06:43.000000 sitemap-generator-0.9.8/pysitemap/backends/sqlite_todo.py
+-rw-rw-rw-   0        0        0     4207 2021-04-14 08:23:23.000000 sitemap-generator-0.9.8/pysitemap/base_crawler.py
+-rw-rw-rw-   0        0        0      889 2021-03-24 07:06:43.000000 sitemap-generator-0.9.8/pysitemap/db.py
+drwxrwxrwx   0        0        0        0 2021-04-14 08:39:02.695603 sitemap-generator-0.9.8/pysitemap/format_processors/
+-rw-rw-rw-   0        0        0        0 2021-03-24 07:06:43.000000 sitemap-generator-0.9.8/pysitemap/format_processors/__init__.py
+-rw-rw-rw-   0        0        0      425 2021-03-24 07:06:43.000000 sitemap-generator-0.9.8/pysitemap/format_processors/text.py
+-rw-rw-rw-   0        0        0      946 2021-03-24 07:06:43.000000 sitemap-generator-0.9.8/pysitemap/format_processors/xml.py
+-rw-rw-rw-   0        0        0     2400 2021-03-24 07:06:43.000000 sitemap-generator-0.9.8/pysitemap/models.py
+-rw-rw-rw-   0        0        0     4878 2021-03-24 07:06:43.000000 sitemap-generator-0.9.8/pysitemap/rest.py
+-rw-rw-rw-   0        0        0     1206 2021-03-24 07:06:43.000000 sitemap-generator-0.9.8/pysitemap/validators.py
+-rw-rw-rw-   0        0        0       25 2021-03-24 07:06:43.000000 sitemap-generator-0.9.8/requirements.txt
+-rw-rw-rw-   0        0        0       42 2021-04-14 08:39:02.763602 sitemap-generator-0.9.8/setup.cfg
+-rw-rw-rw-   0        0        0     1435 2021-03-24 07:06:43.000000 sitemap-generator-0.9.8/setup.py
+drwxrwxrwx   0        0        0        0 2021-04-14 08:39:02.760602 sitemap-generator-0.9.8/sitemap_generator.egg-info/
+-rw-rw-rw-   0        0        0     3333 2021-04-14 08:39:02.000000 sitemap-generator-0.9.8/sitemap_generator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      580 2021-04-14 08:39:02.000000 sitemap-generator-0.9.8/sitemap_generator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2021-04-14 08:39:02.000000 sitemap-generator-0.9.8/sitemap_generator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2021-04-14 08:39:02.000000 sitemap-generator-0.9.8/sitemap_generator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2021-04-14 08:39:02.000000 sitemap-generator-0.9.8/sitemap_generator.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       17 2021-04-14 08:23:23.000000 sitemap-generator-0.9.8/version.py
```

### Comparing `sitemap-generator-0.9.5/LICENSE` & `sitemap-generator-0.9.8/LICENSE`

 * *Files identical despite different names*

### Comparing `sitemap-generator-0.9.5/NOTICE` & `sitemap-generator-0.9.8/NOTICE`

 * *Files identical despite different names*

### Comparing `sitemap-generator-0.9.5/PKG-INFO` & `sitemap-generator-0.9.8/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sitemap-generator
-Version: 0.9.5
+Version: 0.9.8
 Summary: web crawler and sitemap generator.
 Home-page: https://github.com/Haikson/sitemap-generator
 Author: Kamo Petrosyan
 Author-email: kamo@haikson.com
 License: GPL3
 Description: pysitemap
         =========
@@ -42,15 +42,15 @@
                     sys.argv.remove('--iocp')
                     logging.info('using iocp')
                     el = windows_events.ProactorEventLoop()
                     events.set_event_loop(el)
         
                 # root_url = sys.argv[1]
                 root_url = 'https://www.haikson.com'
-                crawler(root_url, out_file='sitemap.xml')
+                crawler(root_url, out_file='sitemap.xml', exclude_urls=[".pdf", ".jpg", ".zip"])
         
         TODO
         -----
         
         -  big sites with count of pages more then 100K will use more then 100MB
            memory. Move queue and done lists into database. Write Queue and Done
            backend classes based on
@@ -58,14 +58,23 @@
         -  SQLite database
         -  Redis
         -  Write api for extending by user backends
         
         changelog
         ---------
         
+        v. 0.9.8
+        ''''''''
+        
+        - new **exlude_urls** parameter for pysitemap.crowler
+        - Crawler. **exclude_urls** parameter.
+            System checks for current url not contains each substring from exclude_urls.
+            Default value is empty list
+        - Crawler. **set_exclude_url** method.
+        
         v. 0.9.2
         ''''''''
         
         -  todo queue and done list backends
         -  created very slowest sqlite backend for todo queue and done lists (1000 url writing for 3 minutes)
         -  tests for sqlite_todo backend
```

### Comparing `sitemap-generator-0.9.5/pysitemap/__init__.py` & `sitemap-generator-0.9.8/pysitemap/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 import asyncio
 import signal
 from pysitemap.base_crawler import Crawler
+import logging
+logger = logging.getLogger(__name__)
 
 
-def crawler(root_url, out_file, out_format='xml', maxtasks=100):
+def crawler(root_url, out_file, out_format='xml', maxtasks=100, exclude_urls=None):
     """
     run crowler
     :param root_url: Site root url
     :param out_file: path to the out file
     :param out_format: format of out file [xml, txt]
     :param maxtasks: max count of tasks
     :return:
     """
     loop = asyncio.get_event_loop()
-
     c = Crawler(root_url, out_file=out_file, out_format=out_format, maxtasks=maxtasks)
+    if exclude_urls:
+        c.set_exclude_url(urls_list=exclude_urls)
     loop.run_until_complete(c.run())
 
     try:
         loop.add_signal_handler(signal.SIGINT, loop.stop)
     except RuntimeError:
         pass
-    print('todo_queue:', len(c.todo_queue))
-    print('busy:', len(c.busy))
-    print('done:', len(c.done), '; ok:', sum(c.done.values()))
-    print('tasks:', len(c.tasks))
+    logger.info('todo_queue:', len(c.todo_queue))
+    logger.info('busy:', len(c.busy))
+    logger.info('done:', len(c.done), '; ok:', sum(c.done.values()))
+    logger.info('tasks:', len(c.tasks))
```

### Comparing `sitemap-generator-0.9.5/pysitemap/backends/sqlite_todo.py` & `sitemap-generator-0.9.8/pysitemap/backends/sqlite_todo.py`

 * *Files identical despite different names*

### Comparing `sitemap-generator-0.9.5/pysitemap/base_crawler.py` & `sitemap-generator-0.9.8/pysitemap/base_crawler.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 class Crawler:
 
     format_processors = {
         'xml': XMLWriter,
         'txt': TextWriter
     }
 
+    exclude_urls = []
+
     def __init__(self, rooturl, out_file, out_format='xml', maxtasks=100,
                  todo_queue_backend=set, done_backend=dict):
         """
         Crawler constructor
         :param rooturl: root url of site
         :type rooturl: str
         :param out_file: file to save sitemap result
@@ -58,14 +60,15 @@
         :param urls:
         :return:
         """
         for url, parenturl in urls:
             url = urllib.parse.urljoin(parenturl, url)
             url, frag = urllib.parse.urldefrag(url)
             if (url.startswith(self.rooturl) and
+                    not any(exclude_part in url for exclude_part in self.exclude_urls) and
                     url not in self.busy and
                     url not in self.done and
                     url not in self.todo_queue):
                 self.todo_queue.add(url)
                 # Acquire semaphore
                 await self.sem.acquire()
                 # Create async task
@@ -107,8 +110,9 @@
             resp.close()
             self.done[url] = True
 
         self.busy.remove(url)
         logging.info(len(self.done), 'completed tasks,', len(self.tasks),
               'still pending, todo_queue', len(self.todo_queue))
 
-
+    def set_exclude_url(self, urls_list):
+        self.exclude_urls = urls_list
```

### Comparing `sitemap-generator-0.9.5/pysitemap/db.py` & `sitemap-generator-0.9.8/pysitemap/db.py`

 * *Files identical despite different names*

### Comparing `sitemap-generator-0.9.5/pysitemap/format_processors/xml.py` & `sitemap-generator-0.9.8/pysitemap/format_processors/xml.py`

 * *Files identical despite different names*

### Comparing `sitemap-generator-0.9.5/pysitemap/models.py` & `sitemap-generator-0.9.8/pysitemap/models.py`

 * *Files identical despite different names*

### Comparing `sitemap-generator-0.9.5/pysitemap/rest.py` & `sitemap-generator-0.9.8/pysitemap/rest.py`

 * *Files identical despite different names*

### Comparing `sitemap-generator-0.9.5/pysitemap/validators.py` & `sitemap-generator-0.9.8/pysitemap/validators.py`

 * *Files identical despite different names*

### Comparing `sitemap-generator-0.9.5/setup.py` & `sitemap-generator-0.9.8/setup.py`

 * *Files identical despite different names*

### Comparing `sitemap-generator-0.9.5/sitemap_generator.egg-info/PKG-INFO` & `sitemap-generator-0.9.8/sitemap_generator.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sitemap-generator
-Version: 0.9.5
+Version: 0.9.8
 Summary: web crawler and sitemap generator.
 Home-page: https://github.com/Haikson/sitemap-generator
 Author: Kamo Petrosyan
 Author-email: kamo@haikson.com
 License: GPL3
 Description: pysitemap
         =========
@@ -42,15 +42,15 @@
                     sys.argv.remove('--iocp')
                     logging.info('using iocp')
                     el = windows_events.ProactorEventLoop()
                     events.set_event_loop(el)
         
                 # root_url = sys.argv[1]
                 root_url = 'https://www.haikson.com'
-                crawler(root_url, out_file='sitemap.xml')
+                crawler(root_url, out_file='sitemap.xml', exclude_urls=[".pdf", ".jpg", ".zip"])
         
         TODO
         -----
         
         -  big sites with count of pages more then 100K will use more then 100MB
            memory. Move queue and done lists into database. Write Queue and Done
            backend classes based on
@@ -58,14 +58,23 @@
         -  SQLite database
         -  Redis
         -  Write api for extending by user backends
         
         changelog
         ---------
         
+        v. 0.9.8
+        ''''''''
+        
+        - new **exlude_urls** parameter for pysitemap.crowler
+        - Crawler. **exclude_urls** parameter.
+            System checks for current url not contains each substring from exclude_urls.
+            Default value is empty list
+        - Crawler. **set_exclude_url** method.
+        
         v. 0.9.2
         ''''''''
         
         -  todo queue and done list backends
         -  created very slowest sqlite backend for todo queue and done lists (1000 url writing for 3 minutes)
         -  tests for sqlite_todo backend
```

### Comparing `sitemap-generator-0.9.5/sitemap_generator.egg-info/SOURCES.txt` & `sitemap-generator-0.9.8/sitemap_generator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

