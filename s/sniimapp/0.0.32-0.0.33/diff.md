# Comparing `tmp/sniimapp-0.0.32.tar.gz` & `tmp/sniimapp-0.0.33.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sniimapp-0.0.32.tar", last modified: Sun Jul  2 06:27:51 2023, max compression
+gzip compressed data, was "sniimapp-0.0.33.tar", last modified: Sun Jul  2 06:32:55 2023, max compression
```

## Comparing `sniimapp-0.0.32.tar` & `sniimapp-0.0.33.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 06:27:51.893252 sniimapp-0.0.32/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1074 2023-06-29 18:21:41.000000 sniimapp-0.0.32/LICENSE
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1690 2023-07-02 06:27:51.893252 sniimapp-0.0.32/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1163 2023-07-02 06:27:13.000000 sniimapp-0.0.32/README.md
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      516 2023-07-02 06:27:38.000000 sniimapp-0.0.32/pyproject.toml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-07-02 06:27:51.893252 sniimapp-0.0.32/setup.cfg
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 06:27:51.889253 sniimapp-0.0.32/sniimapp.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1690 2023-07-02 06:27:51.000000 sniimapp-0.0.32/sniimapp.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      172 2023-07-02 06:27:51.000000 sniimapp-0.0.32/sniimapp.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-07-02 06:27:51.000000 sniimapp-0.0.32/sniimapp.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        9 2023-07-02 06:27:51.000000 sniimapp-0.0.32/sniimapp.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1402 2023-07-02 06:18:38.000000 sniimapp-0.0.32/sniimapp.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 06:32:55.356493 sniimapp-0.0.33/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1074 2023-06-29 18:21:41.000000 sniimapp-0.0.33/LICENSE
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1690 2023-07-02 06:32:55.356493 sniimapp-0.0.33/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1163 2023-07-02 06:32:13.000000 sniimapp-0.0.33/README.md
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      516 2023-07-02 06:32:33.000000 sniimapp-0.0.33/pyproject.toml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-07-02 06:32:55.356493 sniimapp-0.0.33/setup.cfg
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-02 06:32:55.356493 sniimapp-0.0.33/sniimapp.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1690 2023-07-02 06:32:55.000000 sniimapp-0.0.33/sniimapp.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      172 2023-07-02 06:32:55.000000 sniimapp-0.0.33/sniimapp.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-07-02 06:32:55.000000 sniimapp-0.0.33/sniimapp.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        9 2023-07-02 06:32:55.000000 sniimapp-0.0.33/sniimapp.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1402 2023-07-02 06:18:38.000000 sniimapp-0.0.33/sniimapp.py
```

### Comparing `sniimapp-0.0.32/LICENSE` & `sniimapp-0.0.33/LICENSE`

 * *Files identical despite different names*

### Comparing `sniimapp-0.0.32/PKG-INFO` & `sniimapp-0.0.33/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sniimapp
-Version: 0.0.32
+Version: 0.0.33
 Summary: Libreria para extraccion de precios SNIIM
 Author-email: Rodolfo Lopez <1803672F@umich.mx>
 Project-URL: Homepage, https://github.com/rodolfolopezfcca/sniimapp_2
 Project-URL: Bug Tracker, https://github.com/rodolfolopezfcca/sniimapp_2
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -27,19 +27,19 @@
 - pip install pymongo
 
 ### Uso:
 
 - import sniimapp
 
 Los parametros obligatorios para hacer una busqueda son el tipo de mecado **granos**, **fyh**, **fecha inicial** y **fecha final**:
-- sniim = sniimapp.SNIIM('granos', '01/01/2018', '22/01/2018')
-- sniim = sniimapp.SNIIM('fyh', '01/01/2018', '22/01/2018')
+- sniim = sniimapp.SNIIM('granos', '2020-03-01', '2021-04-01')
+- sniim = sniimapp.SNIIM('fyh', '2020-03-01', '2021-04-01')
 
 Se pueden utilizar los parametros de **producto** y **origen** para afinar la busqueda:
-- sniim = sniimapp.SNIIM('granos', '01/01/2018', '22/01/2018', 'Alubia')
-- sniim = sniimapp.SNIIM('granos', '01/01/2018', '22/01/2018', 'Alubia', 'Durango')
+- sniim = sniimapp.SNIIM('granos', '2020-03-01', '2021-04-01', 'Alubia')
+- sniim = sniimapp.SNIIM('granos', '2020-03-01', '2021-04-01', 'Alubia', 'Durango')
 
 Una vez creado el objeto, se utiliza la funcion **get_data()** para obtener los datos:
 - data = sniim.get_data()
 
 La funcion get_data() regresa un objeto cursor Mongo con el cual se puede interactur con los datos.
 Para mas informaciion sobre cursor Mongo visite [Tools for iterating over MongoDB query results](https://pymongo.readthedocs.io/en/stable/api/pymongo/cursor.html#pymongo.cursor.Cursor.address)
```

### Comparing `sniimapp-0.0.32/README.md` & `sniimapp-0.0.33/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -13,19 +13,19 @@
 - pip install pymongo
 
 ### Uso:
 
 - import sniimapp
 
 Los parametros obligatorios para hacer una busqueda son el tipo de mecado **granos**, **fyh**, **fecha inicial** y **fecha final**:
-- sniim = sniimapp.SNIIM('granos', '01/01/2018', '22/01/2018')
-- sniim = sniimapp.SNIIM('fyh', '01/01/2018', '22/01/2018')
+- sniim = sniimapp.SNIIM('granos', '2020-03-01', '2021-04-01')
+- sniim = sniimapp.SNIIM('fyh', '2020-03-01', '2021-04-01')
 
 Se pueden utilizar los parametros de **producto** y **origen** para afinar la busqueda:
-- sniim = sniimapp.SNIIM('granos', '01/01/2018', '22/01/2018', 'Alubia')
-- sniim = sniimapp.SNIIM('granos', '01/01/2018', '22/01/2018', 'Alubia', 'Durango')
+- sniim = sniimapp.SNIIM('granos', '2020-03-01', '2021-04-01', 'Alubia')
+- sniim = sniimapp.SNIIM('granos', '2020-03-01', '2021-04-01', 'Alubia', 'Durango')
 
 Una vez creado el objeto, se utiliza la funcion **get_data()** para obtener los datos:
 - data = sniim.get_data()
 
 La funcion get_data() regresa un objeto cursor Mongo con el cual se puede interactur con los datos.
 Para mas informaciion sobre cursor Mongo visite [Tools for iterating over MongoDB query results](https://pymongo.readthedocs.io/en/stable/api/pymongo/cursor.html#pymongo.cursor.Cursor.address)
```

### Comparing `sniimapp-0.0.32/pyproject.toml` & `sniimapp-0.0.33/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "sniimapp"
-version = "0.0.32"
+version = "0.0.33"
 authors = [
   { name="Rodolfo Lopez", email="1803672F@umich.mx" },
 ]
 description = "Libreria para extraccion de precios SNIIM"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `sniimapp-0.0.32/sniimapp.egg-info/PKG-INFO` & `sniimapp-0.0.33/sniimapp.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sniimapp
-Version: 0.0.32
+Version: 0.0.33
 Summary: Libreria para extraccion de precios SNIIM
 Author-email: Rodolfo Lopez <1803672F@umich.mx>
 Project-URL: Homepage, https://github.com/rodolfolopezfcca/sniimapp_2
 Project-URL: Bug Tracker, https://github.com/rodolfolopezfcca/sniimapp_2
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -27,19 +27,19 @@
 - pip install pymongo
 
 ### Uso:
 
 - import sniimapp
 
 Los parametros obligatorios para hacer una busqueda son el tipo de mecado **granos**, **fyh**, **fecha inicial** y **fecha final**:
-- sniim = sniimapp.SNIIM('granos', '01/01/2018', '22/01/2018')
-- sniim = sniimapp.SNIIM('fyh', '01/01/2018', '22/01/2018')
+- sniim = sniimapp.SNIIM('granos', '2020-03-01', '2021-04-01')
+- sniim = sniimapp.SNIIM('fyh', '2020-03-01', '2021-04-01')
 
 Se pueden utilizar los parametros de **producto** y **origen** para afinar la busqueda:
-- sniim = sniimapp.SNIIM('granos', '01/01/2018', '22/01/2018', 'Alubia')
-- sniim = sniimapp.SNIIM('granos', '01/01/2018', '22/01/2018', 'Alubia', 'Durango')
+- sniim = sniimapp.SNIIM('granos', '2020-03-01', '2021-04-01', 'Alubia')
+- sniim = sniimapp.SNIIM('granos', '2020-03-01', '2021-04-01', 'Alubia', 'Durango')
 
 Una vez creado el objeto, se utiliza la funcion **get_data()** para obtener los datos:
 - data = sniim.get_data()
 
 La funcion get_data() regresa un objeto cursor Mongo con el cual se puede interactur con los datos.
 Para mas informaciion sobre cursor Mongo visite [Tools for iterating over MongoDB query results](https://pymongo.readthedocs.io/en/stable/api/pymongo/cursor.html#pymongo.cursor.Cursor.address)
```

### Comparing `sniimapp-0.0.32/sniimapp.py` & `sniimapp-0.0.33/sniimapp.py`

 * *Files identical despite different names*

