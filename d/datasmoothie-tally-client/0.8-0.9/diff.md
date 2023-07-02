# Comparing `tmp/datasmoothie-tally-client-0.8.tar.gz` & `tmp/datasmoothie-tally-client-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datasmoothie-tally-client-0.8.tar", last modified: Wed Oct  6 10:55:13 2021, max compression
+gzip compressed data, was "datasmoothie-tally-client-0.9.tar", last modified: Fri Mar 11 13:15:30 2022, max compression
```

## Comparing `datasmoothie-tally-client-0.8.tar` & `datasmoothie-tally-client-0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2021-10-06 10:55:13.115015 datasmoothie-tally-client-0.8/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)    11357 2021-10-06 10:06:51.000000 datasmoothie-tally-client-0.8/LICENSE
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)      509 2021-10-06 10:55:13.115015 datasmoothie-tally-client-0.8/PKG-INFO
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     2179 2021-10-06 10:06:51.000000 datasmoothie-tally-client-0.8/README.md
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2021-10-06 10:55:13.115015 datasmoothie-tally-client-0.8/datasmoothie_tally_client.egg-info/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)      509 2021-10-06 10:55:12.000000 datasmoothie-tally-client-0.8/datasmoothie_tally_client.egg-info/PKG-INFO
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)      340 2021-10-06 10:55:12.000000 datasmoothie-tally-client-0.8/datasmoothie_tally_client.egg-info/SOURCES.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)        1 2021-10-06 10:55:12.000000 datasmoothie-tally-client-0.8/datasmoothie_tally_client.egg-info/dependency_links.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       13 2021-10-06 10:55:12.000000 datasmoothie-tally-client-0.8/datasmoothie_tally_client.egg-info/requires.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)        6 2021-10-06 10:55:12.000000 datasmoothie-tally-client-0.8/datasmoothie_tally_client.egg-info/top_level.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       38 2021-10-06 10:55:13.115015 datasmoothie-tally-client-0.8/setup.cfg
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)      693 2021-10-06 10:45:52.000000 datasmoothie-tally-client-0.8/setup.py
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2021-10-06 10:55:13.115015 datasmoothie-tally-client-0.8/tally/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       63 2021-10-06 10:06:51.000000 datasmoothie-tally-client-0.8/tally/__init__.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     8360 2021-10-06 10:42:19.000000 datasmoothie-tally-client-0.8/tally/dataset.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)      664 2021-10-06 10:06:51.000000 datasmoothie-tally-client-0.8/tally/decorators.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     6169 2021-10-06 10:06:51.000000 datasmoothie-tally-client-0.8/tally/tally.py
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2022-03-11 13:15:30.655825 datasmoothie-tally-client-0.9/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)    11357 2022-03-11 12:24:30.000000 datasmoothie-tally-client-0.9/LICENSE
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      509 2022-03-11 13:15:30.655825 datasmoothie-tally-client-0.9/PKG-INFO
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     2179 2022-03-11 12:24:30.000000 datasmoothie-tally-client-0.9/README.md
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2022-03-11 13:15:30.655825 datasmoothie-tally-client-0.9/datasmoothie_tally_client.egg-info/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      509 2022-03-11 13:15:30.000000 datasmoothie-tally-client-0.9/datasmoothie_tally_client.egg-info/PKG-INFO
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      340 2022-03-11 13:15:30.000000 datasmoothie-tally-client-0.9/datasmoothie_tally_client.egg-info/SOURCES.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)        1 2022-03-11 13:15:30.000000 datasmoothie-tally-client-0.9/datasmoothie_tally_client.egg-info/dependency_links.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       13 2022-03-11 13:15:30.000000 datasmoothie-tally-client-0.9/datasmoothie_tally_client.egg-info/requires.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)        6 2022-03-11 13:15:30.000000 datasmoothie-tally-client-0.9/datasmoothie_tally_client.egg-info/top_level.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       38 2022-03-11 13:15:30.655825 datasmoothie-tally-client-0.9/setup.cfg
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      693 2022-03-11 13:12:59.000000 datasmoothie-tally-client-0.9/setup.py
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2022-03-11 13:15:30.655825 datasmoothie-tally-client-0.9/tally/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       63 2022-03-11 12:24:30.000000 datasmoothie-tally-client-0.9/tally/__init__.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     9227 2022-03-11 12:58:48.000000 datasmoothie-tally-client-0.9/tally/dataset.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      664 2022-03-11 12:24:30.000000 datasmoothie-tally-client-0.9/tally/decorators.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     6169 2022-03-11 12:24:30.000000 datasmoothie-tally-client-0.9/tally/tally.py
```

### Comparing `datasmoothie-tally-client-0.8/LICENSE` & `datasmoothie-tally-client-0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `datasmoothie-tally-client-0.8/README.md` & `datasmoothie-tally-client-0.9/README.md`

 * *Files identical despite different names*

### Comparing `datasmoothie-tally-client-0.8/setup.py` & `datasmoothie-tally-client-0.9/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 setuptools.setup(
     name="datasmoothie-tally-client",
     packages=setuptools.find_packages(),
     install_requires=[
         'numpy',
         'pandas',
     ],
-    version="0.8",
+    version="0.9",
     license='MIT',
     include_package_data=True,
     url="https://github.com/datasmoothie/datasmoothie-tally-client",
     author="Geir Freysson",
     author_email="geir@datasmoothie.com",
     description="Python wrapper for the Tally API.",
     keywords=['surveys', 'market research', 'weighting', 'significance tests'],
```

### Comparing `datasmoothie-tally-client-0.8/tally/dataset.py` & `datasmoothie-tally-client-0.9/tally/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,14 +92,38 @@
         }
         response = self.tally.post_request('tally', 'convert_data_to_csv_json', payload)
         result = json.loads(response.content)
         self.qp_meta = json.dumps(result['json'])
         self.qp_data = result['csv']
         self.dataset_type = 'quantipy'
 
+    def use_parquet(self, pq_data_filename, pq_meta_filename=None):
+
+        with open(pq_data_filename, mode='rb') as file:
+            fileContent_data = file.read()
+        
+        payload={}
+
+        files=[ 
+            ('pq', (pq_data_filename,io.BytesIO(fileContent_data), 'application/x-parquet')) 
+        ]
+
+        if pq_meta_filename is not None:
+            with open(pq_meta_filename, mode='rb') as file:
+                fileContent_meta = file.read()
+            files.append(
+                ('pq_meta',(pq_meta_filename,io.BytesIO(fileContent_meta),'text/plain')),
+            )
+        response = self.tally.post_request('tally', 'convert_data_to_csv_json', payload, files)
+        result = json.loads(response.content)
+        self.qp_meta = json.dumps(result['json'])
+        self.qp_data = result['csv']
+        self.dataset_type = 'quantipy'
+
+
     def use_unicom(self, mdd_filename, ddf_filename):
         with open(mdd_filename, mode='rb') as file:
             fileContent_mdd = file.read()
 
         with open(ddf_filename, mode='rb') as file:
             fileContent_ddf = file.read()
```

### Comparing `datasmoothie-tally-client-0.8/tally/decorators.py` & `datasmoothie-tally-client-0.9/tally/decorators.py`

 * *Files identical despite different names*

### Comparing `datasmoothie-tally-client-0.8/tally/tally.py` & `datasmoothie-tally-client-0.9/tally/tally.py`

 * *Files identical despite different names*

