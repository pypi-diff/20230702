# Comparing `tmp/sniimapp-0.0.31.tar.gz` & `tmp/sniimapp-0.0.32.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sniimapp-0.0.31.tar", last modified: Fri Jun 30 18:53:51 2023, max compression
+gzip compressed data, was "sniimapp-0.0.32.tar", last modified: Sun Jul  2 06:27:51 2023, max compression
```

## Comparing `sniimapp-0.0.31.tar` & `sniimapp-0.0.32.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-30 18:53:51.342967 sniimapp-0.0.31/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1074 2023-06-29 18:21:41.000000 sniimapp-0.0.31/LICENSE
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1370 2023-06-30 18:53:51.342967 sniimapp-0.0.31/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      843 2023-06-29 22:13:57.000000 sniimapp-0.0.31/README.md
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      516 2023-06-30 18:53:22.000000 sniimapp-0.0.31/pyproject.toml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-06-30 18:53:51.342967 sniimapp-0.0.31/setup.cfg
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-30 18:53:51.342967 sniimapp-0.0.31/sniimapp.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1370 2023-06-30 18:53:51.000000 sniimapp-0.0.31/sniimapp.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      172 2023-06-30 18:53:51.000000 sniimapp-0.0.31/sniimapp.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-06-30 18:53:51.000000 sniimapp-0.0.31/sniimapp.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        9 2023-06-30 18:53:51.000000 sniimapp-0.0.31/sniimapp.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1195 2023-06-30 18:43:31.000000 sniimapp-0.0.31/sniimapp.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 06:27:51.893252 sniimapp-0.0.32/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1074 2023-06-29 18:21:41.000000 sniimapp-0.0.32/LICENSE
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1690 2023-07-02 06:27:51.893252 sniimapp-0.0.32/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1163 2023-07-02 06:27:13.000000 sniimapp-0.0.32/README.md
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      516 2023-07-02 06:27:38.000000 sniimapp-0.0.32/pyproject.toml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-07-02 06:27:51.893252 sniimapp-0.0.32/setup.cfg
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 06:27:51.889253 sniimapp-0.0.32/sniimapp.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1690 2023-07-02 06:27:51.000000 sniimapp-0.0.32/sniimapp.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      172 2023-07-02 06:27:51.000000 sniimapp-0.0.32/sniimapp.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-07-02 06:27:51.000000 sniimapp-0.0.32/sniimapp.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        9 2023-07-02 06:27:51.000000 sniimapp-0.0.32/sniimapp.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1402 2023-07-02 06:18:38.000000 sniimapp-0.0.32/sniimapp.py
```

### Comparing `sniimapp-0.0.31/LICENSE` & `sniimapp-0.0.32/LICENSE`

 * *Files identical despite different names*

### Comparing `sniimapp-0.0.31/PKG-INFO` & `sniimapp-0.0.32/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sniimapp
-Version: 0.0.31
+Version: 0.0.32
 Summary: Libreria para extraccion de precios SNIIM
 Author-email: Rodolfo Lopez <1803672F@umich.mx>
 Project-URL: Homepage, https://github.com/rodolfolopezfcca/sniimapp_2
 Project-URL: Bug Tracker, https://github.com/rodolfolopezfcca/sniimapp_2
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -25,18 +25,21 @@
 ### Requerimientos:
 
 - pip install pymongo
 
 ### Uso:
 
 - import sniimapp
+
+Los parametros obligatorios para hacer una busqueda son el tipo de mecado **granos**, **fyh**, **fecha inicial** y **fecha final**:
 - sniim = sniimapp.SNIIM('granos', '01/01/2018', '22/01/2018')
-- data = sniim.get_data()
+- sniim = sniimapp.SNIIM('fyh', '01/01/2018', '22/01/2018')
 
-- print(data[1])
-- print(data.explain())
+Se pueden utilizar los parametros de **producto** y **origen** para afinar la busqueda:
+- sniim = sniimapp.SNIIM('granos', '01/01/2018', '22/01/2018', 'Alubia')
+- sniim = sniimapp.SNIIM('granos', '01/01/2018', '22/01/2018', 'Alubia', 'Durango')
 
-Para hacer una consulta se debe crear un objeto SNIIM(producto[fyh,granos], fecha_inicial, fecha_fina):
-- sniim = sniimapp.SNIIM('fyh', '01/01/2018', '22/01/2018')
+Una vez creado el objeto, se utiliza la funcion **get_data()** para obtener los datos:
+- data = sniim.get_data()
 
 La funcion get_data() regresa un objeto cursor Mongo con el cual se puede interactur con los datos.
 Para mas informaciion sobre cursor Mongo visite [Tools for iterating over MongoDB query results](https://pymongo.readthedocs.io/en/stable/api/pymongo/cursor.html#pymongo.cursor.Cursor.address)
```

### Comparing `sniimapp-0.0.31/README.md` & `sniimapp-0.0.32/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -11,18 +11,21 @@
 ### Requerimientos:
 
 - pip install pymongo
 
 ### Uso:
 
 - import sniimapp
+
+Los parametros obligatorios para hacer una busqueda son el tipo de mecado **granos**, **fyh**, **fecha inicial** y **fecha final**:
 - sniim = sniimapp.SNIIM('granos', '01/01/2018', '22/01/2018')
-- data = sniim.get_data()
+- sniim = sniimapp.SNIIM('fyh', '01/01/2018', '22/01/2018')
 
-- print(data[1])
-- print(data.explain())
+Se pueden utilizar los parametros de **producto** y **origen** para afinar la busqueda:
+- sniim = sniimapp.SNIIM('granos', '01/01/2018', '22/01/2018', 'Alubia')
+- sniim = sniimapp.SNIIM('granos', '01/01/2018', '22/01/2018', 'Alubia', 'Durango')
 
-Para hacer una consulta se debe crear un objeto SNIIM(producto[fyh,granos], fecha_inicial, fecha_fina):
-- sniim = sniimapp.SNIIM('fyh', '01/01/2018', '22/01/2018')
+Una vez creado el objeto, se utiliza la funcion **get_data()** para obtener los datos:
+- data = sniim.get_data()
 
 La funcion get_data() regresa un objeto cursor Mongo con el cual se puede interactur con los datos.
 Para mas informaciion sobre cursor Mongo visite [Tools for iterating over MongoDB query results](https://pymongo.readthedocs.io/en/stable/api/pymongo/cursor.html#pymongo.cursor.Cursor.address)
```

### Comparing `sniimapp-0.0.31/pyproject.toml` & `sniimapp-0.0.32/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "sniimapp"
-version = "0.0.31"
+version = "0.0.32"
 authors = [
   { name="Rodolfo Lopez", email="1803672F@umich.mx" },
 ]
 description = "Libreria para extraccion de precios SNIIM"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `sniimapp-0.0.31/sniimapp.egg-info/PKG-INFO` & `sniimapp-0.0.32/sniimapp.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sniimapp
-Version: 0.0.31
+Version: 0.0.32
 Summary: Libreria para extraccion de precios SNIIM
 Author-email: Rodolfo Lopez <1803672F@umich.mx>
 Project-URL: Homepage, https://github.com/rodolfolopezfcca/sniimapp_2
 Project-URL: Bug Tracker, https://github.com/rodolfolopezfcca/sniimapp_2
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -25,18 +25,21 @@
 ### Requerimientos:
 
 - pip install pymongo
 
 ### Uso:
 
 - import sniimapp
+
+Los parametros obligatorios para hacer una busqueda son el tipo de mecado **granos**, **fyh**, **fecha inicial** y **fecha final**:
 - sniim = sniimapp.SNIIM('granos', '01/01/2018', '22/01/2018')
-- data = sniim.get_data()
+- sniim = sniimapp.SNIIM('fyh', '01/01/2018', '22/01/2018')
 
-- print(data[1])
-- print(data.explain())
+Se pueden utilizar los parametros de **producto** y **origen** para afinar la busqueda:
+- sniim = sniimapp.SNIIM('granos', '01/01/2018', '22/01/2018', 'Alubia')
+- sniim = sniimapp.SNIIM('granos', '01/01/2018', '22/01/2018', 'Alubia', 'Durango')
 
-Para hacer una consulta se debe crear un objeto SNIIM(producto[fyh,granos], fecha_inicial, fecha_fina):
-- sniim = sniimapp.SNIIM('fyh', '01/01/2018', '22/01/2018')
+Una vez creado el objeto, se utiliza la funcion **get_data()** para obtener los datos:
+- data = sniim.get_data()
 
 La funcion get_data() regresa un objeto cursor Mongo con el cual se puede interactur con los datos.
 Para mas informaciion sobre cursor Mongo visite [Tools for iterating over MongoDB query results](https://pymongo.readthedocs.io/en/stable/api/pymongo/cursor.html#pymongo.cursor.Cursor.address)
```

### Comparing `sniimapp-0.0.31/sniimapp.py` & `sniimapp-0.0.32/sniimapp.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 import datetime
 from pymongo import MongoClient
 import os
+import re
 
 class SNIIM():
 
-    def __init__(self, product, start_date, end_date):
-        self.product = product
-        self.start_date = datetime.datetime.strptime(start_date, "%d/%m/%Y").strftime('%d/%m/%Y')
-        self.end_date   = datetime.datetime.strptime(end_date,   "%d/%m/%Y").strftime('%d/%m/%Y')
+    def __init__(self, collection, start_date, end_date, product='.*', origin='.*' ):
+        self.start_date = datetime.datetime.strptime(start_date, "%Y-%m-%d")
+        self.end_date   = datetime.datetime.strptime(end_date,   "%Y-%m-%d")
         self.MONGO_HOST = '18.215.228.120'
         self.MONGO_PORT = 27017    
         self.MONGO_USER = 'sniim_read'  
         self.MONGO_PASSW ='sniim_read_x59m'    
         self.client = MongoClient(self._connection_string)
         self.MONGO_DB = 'sniim'                
-        if product == 'fyh':
+        if collection == 'fyh':
             self.db_collection = 'sniim_fyh'
-        if product == 'granos':
+        if collection == 'granos':
             self.db_collection = 'sniim_granos'
         self.db = self.client[self.MONGO_DB]
         self.collection = self.db[self.db_collection]
+        self.origin = origin
+        self.product = product
 
     def get_data(self):
-        result = self.collection.find({"fecha":{"$gte":self.start_date,"$lte":self.end_date}})
-        return result
+        product = rgx = re.compile('.*'+str(self.product)+'.*', re.IGNORECASE)  
+        origin  = rgx = re.compile('.*'+str(self.origin)+'.*', re.IGNORECASE)
+        return self.collection.find({"fecha":{"$gte":self.start_date,"$lte":self.end_date}, "producto":product, "origen":origin })
 
     @property
     def _connection_string(self):
         return "mongodb://{0}:{1}@{2}:{3}".format(self.MONGO_USER, self.MONGO_PASSW, self.MONGO_HOST, self.MONGO_PORT)
```

