# Comparing `tmp/exactonline_prefect_tasks-0.0.8.tar.gz` & `tmp/exactonline_prefect_tasks-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exactonline_prefect_tasks-0.0.8.tar", last modified: Sat Apr 30 19:12:50 2022, max compression
+gzip compressed data, was "exactonline_prefect_tasks-0.0.9.tar", last modified: Sat Apr 30 20:22:09 2022, max compression
```

## Comparing `exactonline_prefect_tasks-0.0.8.tar` & `exactonline_prefect_tasks-0.0.9.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 carlospaiva   (501) staff       (20)        0 2022-04-30 19:12:50.996230 exactonline_prefect_tasks-0.0.8/
--rw-r--r--   0 carlospaiva   (501) staff       (20)    35148 2021-01-11 11:45:24.000000 exactonline_prefect_tasks-0.0.8/LICENSE
--rw-r--r--   0 carlospaiva   (501) staff       (20)      196 2022-04-26 10:46:59.000000 exactonline_prefect_tasks-0.0.8/MANIFEST.in
--rw-r--r--   0 carlospaiva   (501) staff       (20)      463 2022-04-30 19:12:50.996354 exactonline_prefect_tasks-0.0.8/PKG-INFO
--rw-r--r--   0 carlospaiva   (501) staff       (20)       30 2022-04-26 09:06:16.000000 exactonline_prefect_tasks-0.0.8/README.rst
--rw-r--r--   0 carlospaiva   (501) staff       (20)      151 2022-04-26 20:42:36.000000 exactonline_prefect_tasks-0.0.8/requirements.txt
--rw-r--r--   0 carlospaiva   (501) staff       (20)      232 2022-04-30 19:12:50.996813 exactonline_prefect_tasks-0.0.8/setup.cfg
--rw-r--r--   0 carlospaiva   (501) staff       (20)      870 2022-02-17 20:14:30.000000 exactonline_prefect_tasks-0.0.8/setup.py
-drwxr-xr-x   0 carlospaiva   (501) staff       (20)        0 2022-04-30 19:12:50.983685 exactonline_prefect_tasks-0.0.8/src/
-drwxr-xr-x   0 carlospaiva   (501) staff       (20)        0 2022-04-30 19:12:50.997110 exactonline_prefect_tasks-0.0.8/src/exactonline_prefect_tasks/
--rw-r--r--   0 carlospaiva   (501) staff       (20)      507 2022-04-26 09:12:56.000000 exactonline_prefect_tasks-0.0.8/src/exactonline_prefect_tasks/__init__.py
--rw-r--r--   0 carlospaiva   (501) staff       (20)      497 2022-04-30 19:12:50.997177 exactonline_prefect_tasks-0.0.8/src/exactonline_prefect_tasks/_version.py
--rw-r--r--   0 carlospaiva   (501) staff       (20)     2518 2022-04-26 16:58:38.000000 exactonline_prefect_tasks-0.0.8/src/exactonline_prefect_tasks/api.py
-drwxr-xr-x   0 carlospaiva   (501) staff       (20)        0 2022-04-30 19:12:50.991093 exactonline_prefect_tasks-0.0.8/src/exactonline_prefect_tasks/aws/
--rw-r--r--   0 carlospaiva   (501) staff       (20)      180 2022-04-22 13:52:41.000000 exactonline_prefect_tasks-0.0.8/src/exactonline_prefect_tasks/aws/__init__.py
--rw-r--r--   0 carlospaiva   (501) staff       (20)      881 2022-04-14 16:57:45.000000 exactonline_prefect_tasks-0.0.8/src/exactonline_prefect_tasks/aws/s3_client.py
--rw-r--r--   0 carlospaiva   (501) staff       (20)     2477 2022-03-30 15:25:57.000000 exactonline_prefect_tasks-0.0.8/src/exactonline_prefect_tasks/aws/s3_storage.py
--rw-r--r--   0 carlospaiva   (501) staff       (20)     7944 2022-04-25 13:39:57.000000 exactonline_prefect_tasks-0.0.8/src/exactonline_prefect_tasks/aws/secretsmanager_client.py
--rw-r--r--   0 carlospaiva   (501) staff       (20)     2280 2022-04-30 19:11:58.000000 exactonline_prefect_tasks-0.0.8/src/exactonline_prefect_tasks/aws/secretsmanager_storage.py
-drwxr-xr-x   0 carlospaiva   (501) staff       (20)        0 2022-04-30 19:12:50.992713 exactonline_prefect_tasks-0.0.8/src/exactonline_prefect_tasks/exceptions/
--rw-r--r--   0 carlospaiva   (501) staff       (20)      213 2022-04-14 13:59:17.000000 exactonline_prefect_tasks-0.0.8/src/exactonline_prefect_tasks/exceptions/__init__.py
--rw-r--r--   0 carlospaiva   (501) staff       (20)      382 2020-11-24 16:08:17.000000 exactonline_prefect_tasks-0.0.8/src/exactonline_prefect_tasks/exceptions/api_exception.py
--rw-r--r--   0 carlospaiva   (501) staff       (20)      164 2022-04-18 15:41:33.000000 exactonline_prefect_tasks-0.0.8/src/exactonline_prefect_tasks/exceptions/auth_exception.py
--rw-r--r--   0 carlospaiva   (501) staff       (20)      312 2020-12-03 16:17:53.000000 exactonline_prefect_tasks-0.0.8/src/exactonline_prefect_tasks/exceptions/missing_parameters_exception.py
--rw-r--r--   0 carlospaiva   (501) staff       (20)      287 2020-12-04 18:28:17.000000 exactonline_prefect_tasks-0.0.8/src/exactonline_prefect_tasks/exceptions/no_record_found_exception.py
-drwxr-xr-x   0 carlospaiva   (501) staff       (20)        0 2022-04-30 19:12:50.995887 exactonline_prefect_tasks-0.0.8/src/exactonline_prefect_tasks/tasks/
--rw-r--r--   0 carlospaiva   (501) staff       (20)      163 2022-04-26 09:12:56.000000 exactonline_prefect_tasks-0.0.8/src/exactonline_prefect_tasks/tasks/__init__.py
--rw-r--r--   0 carlospaiva   (501) staff       (20)     1335 2022-04-25 14:45:58.000000 exactonline_prefect_tasks-0.0.8/src/exactonline_prefect_tasks/tasks/create.py
--rw-r--r--   0 carlospaiva   (501) staff       (20)     1328 2020-12-18 15:01:05.000000 exactonline_prefect_tasks-0.0.8/src/exactonline_prefect_tasks/tasks/delete.py
--rw-r--r--   0 carlospaiva   (501) staff       (20)     1447 2020-12-18 15:01:05.000000 exactonline_prefect_tasks-0.0.8/src/exactonline_prefect_tasks/tasks/get_all.py
--rw-r--r--   0 carlospaiva   (501) staff       (20)     1921 2020-12-17 14:37:51.000000 exactonline_prefect_tasks-0.0.8/src/exactonline_prefect_tasks/tasks/get_by_id.py
--rw-r--r--   0 carlospaiva   (501) staff       (20)     1466 2020-12-16 17:09:01.000000 exactonline_prefect_tasks-0.0.8/src/exactonline_prefect_tasks/tasks/read.py
--rw-r--r--   0 carlospaiva   (501) staff       (20)     2498 2022-04-25 21:55:04.000000 exactonline_prefect_tasks-0.0.8/src/exactonline_prefect_tasks/tasks/search.py
--rw-r--r--   0 carlospaiva   (501) staff       (20)     1192 2020-12-08 15:27:38.000000 exactonline_prefect_tasks-0.0.8/src/exactonline_prefect_tasks/tasks/update.py
--rw-r--r--   0 carlospaiva   (501) staff       (20)     1548 2020-12-08 15:27:38.000000 exactonline_prefect_tasks-0.0.8/src/exactonline_prefect_tasks/tasks/xml_upload.py
--rw-r--r--   0 carlospaiva   (501) staff       (20)     1310 2021-11-16 20:11:28.000000 exactonline_prefect_tasks-0.0.8/src/exactonline_prefect_tasks/utils.py
-drwxr-xr-x   0 carlospaiva   (501) staff       (20)        0 2022-04-30 19:12:50.989421 exactonline_prefect_tasks-0.0.8/src/exactonline_prefect_tasks.egg-info/
--rw-r--r--   0 carlospaiva   (501) staff       (20)      463 2022-04-30 19:12:50.000000 exactonline_prefect_tasks-0.0.8/src/exactonline_prefect_tasks.egg-info/PKG-INFO
--rw-r--r--   0 carlospaiva   (501) staff       (20)     1499 2022-04-30 19:12:50.000000 exactonline_prefect_tasks-0.0.8/src/exactonline_prefect_tasks.egg-info/SOURCES.txt
--rw-r--r--   0 carlospaiva   (501) staff       (20)        1 2022-04-30 19:12:50.000000 exactonline_prefect_tasks-0.0.8/src/exactonline_prefect_tasks.egg-info/dependency_links.txt
--rw-r--r--   0 carlospaiva   (501) staff       (20)      152 2022-04-30 19:12:50.000000 exactonline_prefect_tasks-0.0.8/src/exactonline_prefect_tasks.egg-info/requires.txt
--rw-r--r--   0 carlospaiva   (501) staff       (20)       26 2022-04-30 19:12:50.000000 exactonline_prefect_tasks-0.0.8/src/exactonline_prefect_tasks.egg-info/top_level.txt
--rw-r--r--   0 carlospaiva   (501) staff       (20)    70144 2021-11-09 12:20:05.000000 exactonline_prefect_tasks-0.0.8/versioneer.py
+drwxr-xr-x   0 carlospaiva   (501) staff       (20)        0 2022-04-30 20:22:09.641477 exactonline_prefect_tasks-0.0.9/
+-rw-r--r--   0 carlospaiva   (501) staff       (20)    35148 2021-01-11 11:45:24.000000 exactonline_prefect_tasks-0.0.9/LICENSE
+-rw-r--r--   0 carlospaiva   (501) staff       (20)      196 2022-04-26 10:46:59.000000 exactonline_prefect_tasks-0.0.9/MANIFEST.in
+-rw-r--r--   0 carlospaiva   (501) staff       (20)      463 2022-04-30 20:22:09.641584 exactonline_prefect_tasks-0.0.9/PKG-INFO
+-rw-r--r--   0 carlospaiva   (501) staff       (20)       30 2022-04-26 09:06:16.000000 exactonline_prefect_tasks-0.0.9/README.rst
+-rw-r--r--   0 carlospaiva   (501) staff       (20)      151 2022-04-26 20:42:36.000000 exactonline_prefect_tasks-0.0.9/requirements.txt
+-rw-r--r--   0 carlospaiva   (501) staff       (20)      232 2022-04-30 20:22:09.641993 exactonline_prefect_tasks-0.0.9/setup.cfg
+-rw-r--r--   0 carlospaiva   (501) staff       (20)      870 2022-02-17 20:14:30.000000 exactonline_prefect_tasks-0.0.9/setup.py
+drwxr-xr-x   0 carlospaiva   (501) staff       (20)        0 2022-04-30 20:22:09.632006 exactonline_prefect_tasks-0.0.9/src/
+drwxr-xr-x   0 carlospaiva   (501) staff       (20)        0 2022-04-30 20:22:09.642219 exactonline_prefect_tasks-0.0.9/src/exactonline_prefect_tasks/
+-rw-r--r--   0 carlospaiva   (501) staff       (20)      507 2022-04-26 09:12:56.000000 exactonline_prefect_tasks-0.0.9/src/exactonline_prefect_tasks/__init__.py
+-rw-r--r--   0 carlospaiva   (501) staff       (20)      497 2022-04-30 20:22:09.642285 exactonline_prefect_tasks-0.0.9/src/exactonline_prefect_tasks/_version.py
+-rw-r--r--   0 carlospaiva   (501) staff       (20)     2518 2022-04-30 20:14:58.000000 exactonline_prefect_tasks-0.0.9/src/exactonline_prefect_tasks/api.py
+drwxr-xr-x   0 carlospaiva   (501) staff       (20)        0 2022-04-30 20:22:09.637777 exactonline_prefect_tasks-0.0.9/src/exactonline_prefect_tasks/aws/
+-rw-r--r--   0 carlospaiva   (501) staff       (20)      180 2022-04-22 13:52:41.000000 exactonline_prefect_tasks-0.0.9/src/exactonline_prefect_tasks/aws/__init__.py
+-rw-r--r--   0 carlospaiva   (501) staff       (20)      881 2022-04-14 16:57:45.000000 exactonline_prefect_tasks-0.0.9/src/exactonline_prefect_tasks/aws/s3_client.py
+-rw-r--r--   0 carlospaiva   (501) staff       (20)     2477 2022-03-30 15:25:57.000000 exactonline_prefect_tasks-0.0.9/src/exactonline_prefect_tasks/aws/s3_storage.py
+-rw-r--r--   0 carlospaiva   (501) staff       (20)     7944 2022-04-25 13:39:57.000000 exactonline_prefect_tasks-0.0.9/src/exactonline_prefect_tasks/aws/secretsmanager_client.py
+-rw-r--r--   0 carlospaiva   (501) staff       (20)     2390 2022-04-30 20:13:51.000000 exactonline_prefect_tasks-0.0.9/src/exactonline_prefect_tasks/aws/secretsmanager_storage.py
+drwxr-xr-x   0 carlospaiva   (501) staff       (20)        0 2022-04-30 20:22:09.639041 exactonline_prefect_tasks-0.0.9/src/exactonline_prefect_tasks/exceptions/
+-rw-r--r--   0 carlospaiva   (501) staff       (20)      213 2022-04-14 13:59:17.000000 exactonline_prefect_tasks-0.0.9/src/exactonline_prefect_tasks/exceptions/__init__.py
+-rw-r--r--   0 carlospaiva   (501) staff       (20)      382 2020-11-24 16:08:17.000000 exactonline_prefect_tasks-0.0.9/src/exactonline_prefect_tasks/exceptions/api_exception.py
+-rw-r--r--   0 carlospaiva   (501) staff       (20)      164 2022-04-18 15:41:33.000000 exactonline_prefect_tasks-0.0.9/src/exactonline_prefect_tasks/exceptions/auth_exception.py
+-rw-r--r--   0 carlospaiva   (501) staff       (20)      312 2020-12-03 16:17:53.000000 exactonline_prefect_tasks-0.0.9/src/exactonline_prefect_tasks/exceptions/missing_parameters_exception.py
+-rw-r--r--   0 carlospaiva   (501) staff       (20)      287 2020-12-04 18:28:17.000000 exactonline_prefect_tasks-0.0.9/src/exactonline_prefect_tasks/exceptions/no_record_found_exception.py
+drwxr-xr-x   0 carlospaiva   (501) staff       (20)        0 2022-04-30 20:22:09.641263 exactonline_prefect_tasks-0.0.9/src/exactonline_prefect_tasks/tasks/
+-rw-r--r--   0 carlospaiva   (501) staff       (20)      163 2022-04-26 09:12:56.000000 exactonline_prefect_tasks-0.0.9/src/exactonline_prefect_tasks/tasks/__init__.py
+-rw-r--r--   0 carlospaiva   (501) staff       (20)     1335 2022-04-25 14:45:58.000000 exactonline_prefect_tasks-0.0.9/src/exactonline_prefect_tasks/tasks/create.py
+-rw-r--r--   0 carlospaiva   (501) staff       (20)     1328 2020-12-18 15:01:05.000000 exactonline_prefect_tasks-0.0.9/src/exactonline_prefect_tasks/tasks/delete.py
+-rw-r--r--   0 carlospaiva   (501) staff       (20)     1447 2020-12-18 15:01:05.000000 exactonline_prefect_tasks-0.0.9/src/exactonline_prefect_tasks/tasks/get_all.py
+-rw-r--r--   0 carlospaiva   (501) staff       (20)     1921 2020-12-17 14:37:51.000000 exactonline_prefect_tasks-0.0.9/src/exactonline_prefect_tasks/tasks/get_by_id.py
+-rw-r--r--   0 carlospaiva   (501) staff       (20)     1466 2020-12-16 17:09:01.000000 exactonline_prefect_tasks-0.0.9/src/exactonline_prefect_tasks/tasks/read.py
+-rw-r--r--   0 carlospaiva   (501) staff       (20)     2498 2022-04-25 21:55:04.000000 exactonline_prefect_tasks-0.0.9/src/exactonline_prefect_tasks/tasks/search.py
+-rw-r--r--   0 carlospaiva   (501) staff       (20)     1192 2020-12-08 15:27:38.000000 exactonline_prefect_tasks-0.0.9/src/exactonline_prefect_tasks/tasks/update.py
+-rw-r--r--   0 carlospaiva   (501) staff       (20)     1548 2020-12-08 15:27:38.000000 exactonline_prefect_tasks-0.0.9/src/exactonline_prefect_tasks/tasks/xml_upload.py
+-rw-r--r--   0 carlospaiva   (501) staff       (20)     1310 2021-11-16 20:11:28.000000 exactonline_prefect_tasks-0.0.9/src/exactonline_prefect_tasks/utils.py
+drwxr-xr-x   0 carlospaiva   (501) staff       (20)        0 2022-04-30 20:22:09.636485 exactonline_prefect_tasks-0.0.9/src/exactonline_prefect_tasks.egg-info/
+-rw-r--r--   0 carlospaiva   (501) staff       (20)      463 2022-04-30 20:22:09.000000 exactonline_prefect_tasks-0.0.9/src/exactonline_prefect_tasks.egg-info/PKG-INFO
+-rw-r--r--   0 carlospaiva   (501) staff       (20)     1499 2022-04-30 20:22:09.000000 exactonline_prefect_tasks-0.0.9/src/exactonline_prefect_tasks.egg-info/SOURCES.txt
+-rw-r--r--   0 carlospaiva   (501) staff       (20)        1 2022-04-30 20:22:09.000000 exactonline_prefect_tasks-0.0.9/src/exactonline_prefect_tasks.egg-info/dependency_links.txt
+-rw-r--r--   0 carlospaiva   (501) staff       (20)      152 2022-04-30 20:22:09.000000 exactonline_prefect_tasks-0.0.9/src/exactonline_prefect_tasks.egg-info/requires.txt
+-rw-r--r--   0 carlospaiva   (501) staff       (20)       26 2022-04-30 20:22:09.000000 exactonline_prefect_tasks-0.0.9/src/exactonline_prefect_tasks.egg-info/top_level.txt
+-rw-r--r--   0 carlospaiva   (501) staff       (20)    70144 2021-11-09 12:20:05.000000 exactonline_prefect_tasks-0.0.9/versioneer.py
```

### Comparing `exactonline_prefect_tasks-0.0.8/LICENSE` & `exactonline_prefect_tasks-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `exactonline_prefect_tasks-0.0.8/setup.py` & `exactonline_prefect_tasks-0.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `exactonline_prefect_tasks-0.0.8/src/exactonline_prefect_tasks/api.py` & `exactonline_prefect_tasks-0.0.9/src/exactonline_prefect_tasks/api.py`

 * *Files identical despite different names*

### Comparing `exactonline_prefect_tasks-0.0.8/src/exactonline_prefect_tasks/aws/s3_client.py` & `exactonline_prefect_tasks-0.0.9/src/exactonline_prefect_tasks/aws/s3_client.py`

 * *Files identical despite different names*

### Comparing `exactonline_prefect_tasks-0.0.8/src/exactonline_prefect_tasks/aws/s3_storage.py` & `exactonline_prefect_tasks-0.0.9/src/exactonline_prefect_tasks/aws/s3_storage.py`

 * *Files identical despite different names*

### Comparing `exactonline_prefect_tasks-0.0.8/src/exactonline_prefect_tasks/aws/secretsmanager_client.py` & `exactonline_prefect_tasks-0.0.9/src/exactonline_prefect_tasks/aws/secretsmanager_client.py`

 * *Files identical despite different names*

### Comparing `exactonline_prefect_tasks-0.0.8/src/exactonline_prefect_tasks/aws/secretsmanager_storage.py` & `exactonline_prefect_tasks-0.0.9/src/exactonline_prefect_tasks/aws/secretsmanager_storage.py`

 * *Files 6% similar despite different names*

```diff
@@ -56,10 +56,11 @@
             self.add_section(section)
             super(ExactOnlineConfig, self).set(section, option, value)
 
         # Save automatically!
         self.save()
 
     def save(self):
-        if self.get_access_expiry():
-            if time() + 10 > self.get_access_expiry():
-                self.secretsmanager_client.put_value(secret_value=json.dumps({s: dict(self.items(s)) for s in self.sections()}))
+        if self.secret.get('transient'):
+            if self.secret.get('transient').get('access_expiry'):
+                if time() + 10 > float(self.secret.get('transient').get('access_expiry')):
+                    self.secretsmanager_client.put_value(secret_value=json.dumps({s: dict(self.items(s)) for s in self.sections()}))
```

### Comparing `exactonline_prefect_tasks-0.0.8/src/exactonline_prefect_tasks/tasks/create.py` & `exactonline_prefect_tasks-0.0.9/src/exactonline_prefect_tasks/tasks/create.py`

 * *Files identical despite different names*

### Comparing `exactonline_prefect_tasks-0.0.8/src/exactonline_prefect_tasks/tasks/delete.py` & `exactonline_prefect_tasks-0.0.9/src/exactonline_prefect_tasks/tasks/delete.py`

 * *Files identical despite different names*

### Comparing `exactonline_prefect_tasks-0.0.8/src/exactonline_prefect_tasks/tasks/get_all.py` & `exactonline_prefect_tasks-0.0.9/src/exactonline_prefect_tasks/tasks/get_all.py`

 * *Files identical despite different names*

### Comparing `exactonline_prefect_tasks-0.0.8/src/exactonline_prefect_tasks/tasks/get_by_id.py` & `exactonline_prefect_tasks-0.0.9/src/exactonline_prefect_tasks/tasks/get_by_id.py`

 * *Files identical despite different names*

### Comparing `exactonline_prefect_tasks-0.0.8/src/exactonline_prefect_tasks/tasks/read.py` & `exactonline_prefect_tasks-0.0.9/src/exactonline_prefect_tasks/tasks/read.py`

 * *Files identical despite different names*

### Comparing `exactonline_prefect_tasks-0.0.8/src/exactonline_prefect_tasks/tasks/search.py` & `exactonline_prefect_tasks-0.0.9/src/exactonline_prefect_tasks/tasks/search.py`

 * *Files identical despite different names*

### Comparing `exactonline_prefect_tasks-0.0.8/src/exactonline_prefect_tasks/tasks/update.py` & `exactonline_prefect_tasks-0.0.9/src/exactonline_prefect_tasks/tasks/update.py`

 * *Files identical despite different names*

### Comparing `exactonline_prefect_tasks-0.0.8/src/exactonline_prefect_tasks/tasks/xml_upload.py` & `exactonline_prefect_tasks-0.0.9/src/exactonline_prefect_tasks/tasks/xml_upload.py`

 * *Files identical despite different names*

### Comparing `exactonline_prefect_tasks-0.0.8/src/exactonline_prefect_tasks/utils.py` & `exactonline_prefect_tasks-0.0.9/src/exactonline_prefect_tasks/utils.py`

 * *Files identical despite different names*

### Comparing `exactonline_prefect_tasks-0.0.8/src/exactonline_prefect_tasks.egg-info/SOURCES.txt` & `exactonline_prefect_tasks-0.0.9/src/exactonline_prefect_tasks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `exactonline_prefect_tasks-0.0.8/versioneer.py` & `exactonline_prefect_tasks-0.0.9/versioneer.py`

 * *Files identical despite different names*

