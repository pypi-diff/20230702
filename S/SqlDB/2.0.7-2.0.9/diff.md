# Comparing `tmp/SqlDB-2.0.7.tar.gz` & `tmp/SqlDB-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/SqlDB-2.0.7.tar", last modified: Thu Mar 24 16:00:06 2022, max compression
+gzip compressed data, was "dist/SqlDB-2.0.9.tar", last modified: Thu Jul 28 14:47:34 2022, max compression
```

## Comparing `SqlDB-2.0.7.tar` & `SqlDB-2.0.9.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 kage      (1000) kage      (1000)        0 2022-03-24 16:00:06.000000 SqlDB-2.0.7/
-drwxrwxr-x   0 kage      (1000) kage      (1000)        0 2022-03-24 16:00:06.000000 SqlDB-2.0.7/SqlDB/
--rw-r--r--   0 kage      (1000) kage      (1000)    26120 2022-03-24 15:58:24.000000 SqlDB-2.0.7/SqlDB/__init__.py
-drwxrwxr-x   0 kage      (1000) kage      (1000)        0 2022-03-24 16:00:06.000000 SqlDB-2.0.7/SqlDB.egg-info/
--rw-rw-r--   0 kage      (1000) kage      (1000)      612 2022-03-24 16:00:06.000000 SqlDB-2.0.7/SqlDB.egg-info/PKG-INFO
--rw-rw-r--   0 kage      (1000) kage      (1000)      152 2022-03-24 16:00:06.000000 SqlDB-2.0.7/SqlDB.egg-info/SOURCES.txt
--rw-rw-r--   0 kage      (1000) kage      (1000)        1 2022-03-24 16:00:06.000000 SqlDB-2.0.7/SqlDB.egg-info/dependency_links.txt
--rw-rw-r--   0 kage      (1000) kage      (1000)        6 2022-03-24 16:00:06.000000 SqlDB-2.0.7/SqlDB.egg-info/top_level.txt
--rw-rw-r--   0 kage      (1000) kage      (1000)      110 2021-12-19 02:12:49.000000 SqlDB-2.0.7/README.md
--rw-rw-r--   0 kage      (1000) kage      (1000)     1970 2021-12-17 05:58:00.000000 SqlDB-2.0.7/setup.py
--rw-rw-r--   0 kage      (1000) kage      (1000)      612 2022-03-24 16:00:06.000000 SqlDB-2.0.7/PKG-INFO
--rw-rw-r--   0 kage      (1000) kage      (1000)       38 2022-03-24 16:00:06.000000 SqlDB-2.0.7/setup.cfg
+drwxrwxr-x   0 kage      (1000) kage      (1000)        0 2022-07-28 14:47:34.000000 SqlDB-2.0.9/
+drwxrwxr-x   0 kage      (1000) kage      (1000)        0 2022-07-28 14:47:34.000000 SqlDB-2.0.9/SqlDB/
+-rw-r--r--   0 kage      (1000) kage      (1000)    26655 2022-07-28 14:45:59.000000 SqlDB-2.0.9/SqlDB/__init__.py
+drwxrwxr-x   0 kage      (1000) kage      (1000)        0 2022-07-28 14:47:34.000000 SqlDB-2.0.9/SqlDB.egg-info/
+-rw-rw-r--   0 kage      (1000) kage      (1000)      612 2022-07-28 14:47:34.000000 SqlDB-2.0.9/SqlDB.egg-info/PKG-INFO
+-rw-rw-r--   0 kage      (1000) kage      (1000)      152 2022-07-28 14:47:34.000000 SqlDB-2.0.9/SqlDB.egg-info/SOURCES.txt
+-rw-rw-r--   0 kage      (1000) kage      (1000)        1 2022-07-28 14:47:34.000000 SqlDB-2.0.9/SqlDB.egg-info/dependency_links.txt
+-rw-rw-r--   0 kage      (1000) kage      (1000)        6 2022-07-28 14:47:34.000000 SqlDB-2.0.9/SqlDB.egg-info/top_level.txt
+-rw-rw-r--   0 kage      (1000) kage      (1000)      110 2021-12-19 02:12:49.000000 SqlDB-2.0.9/README.md
+-rw-rw-r--   0 kage      (1000) kage      (1000)     1970 2021-12-17 05:58:00.000000 SqlDB-2.0.9/setup.py
+-rw-rw-r--   0 kage      (1000) kage      (1000)      612 2022-07-28 14:47:34.000000 SqlDB-2.0.9/PKG-INFO
+-rw-rw-r--   0 kage      (1000) kage      (1000)       38 2022-07-28 14:47:34.000000 SqlDB-2.0.9/setup.cfg
```

### Comparing `SqlDB-2.0.7/SqlDB/__init__.py` & `SqlDB-2.0.9/SqlDB/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 #Kage Park
 import kmisc as km
 from kmport import *
 import sys
 import traceback
+import time
 #SQLite3
 #import sqlite3
 #Postgresql
 #import psycopg2
 #import psycopg2.extras
+
 try:
     # yum install sqlcipher
     # pip3 install pysqlcipher3
     from pysqlcipher3 import dbapi2 as sqlcipher
     enc=True
 except:
     enc=False
@@ -210,15 +212,30 @@
             con_info['cur'].row_factory = lambda c,r:dict([(col[0], r[idx]) for idx, col in enumerate(con_info['cur'].description)])
         else:
             con_info['cur'].row_factory=None
     rt=[]
     if mode.lower() in ['put','save','commit','update']:
         con_info['cur'].execute('select last_insert_rowid();')
         idx=con_info['cur'].fetchone()
-        con_info['conn'].commit()
+        try:
+            con_info['conn'].commit()
+        except sqlite3.OperationalError as e:
+            ok=0
+            for i in range(0,10):
+                #print('>> retry({}/5) DB commit after 1 second for {}'.format(i,e))
+                time.sleep(1)
+                try:
+                    con_info['conn'].commit()
+                    ok=1
+                    break
+                except sqlite3.OperationalError as e:
+                    pass
+            if ok == 0:
+                con_info['conn'].close()
+                return False,e
         if idx:
             rt=idx[0]
         else:
             rt=True
     elif mode.lower() in ['one','single','get_one','get_single','fetchone']:
         rt=[i for i in con_info['cur'].fetchone()]
     else:
```

### Comparing `SqlDB-2.0.7/SqlDB.egg-info/PKG-INFO` & `SqlDB-2.0.9/SqlDB.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SqlDB
-Version: 2.0.7
+Version: 2.0.9
 Summary: SQL Family DB handler
 Home-page: https://github.com/kagepark/SqlDB
 Author: Kage Park
 License: MIT
 Description: # SQL Family handler
         - Support DB
           - SqLite3
```

### Comparing `SqlDB-2.0.7/setup.py` & `SqlDB-2.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `SqlDB-2.0.7/PKG-INFO` & `SqlDB-2.0.9/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SqlDB
-Version: 2.0.7
+Version: 2.0.9
 Summary: SQL Family DB handler
 Home-page: https://github.com/kagepark/SqlDB
 Author: Kage Park
 License: MIT
 Description: # SQL Family handler
         - Support DB
           - SqLite3
```

