# Comparing `tmp/rosetta-ce-1.4.1.tar.gz` & `tmp/rosetta-ce-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rosetta-ce-1.4.1.tar", last modified: Sun Jul  2 15:50:05 2023, max compression
+gzip compressed data, was "rosetta-ce-1.4.2.tar", last modified: Sun Jul  2 15:59:53 2023, max compression
```

## Comparing `rosetta-ce-1.4.1.tar` & `rosetta-ce-1.4.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-07-02 15:50:05.766526 rosetta-ce-1.4.1/
--rw-r--r--   0 amahmoud   (502) staff       (20)     1070 2023-04-08 17:22:13.000000 rosetta-ce-1.4.1/LICENSE
--rw-r--r--   0 amahmoud   (502) staff       (20)    11253 2023-07-02 15:50:05.766231 rosetta-ce-1.4.1/PKG-INFO
--rw-r--r--   0 amahmoud   (502) staff       (20)    10721 2023-06-29 06:50:02.000000 rosetta-ce-1.4.1/README.md
-drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-07-02 15:50:05.760109 rosetta-ce-1.4.1/rosetta/
--rw-r--r--   0 amahmoud   (502) staff       (20)       92 2023-04-09 08:11:12.000000 rosetta-ce-1.4.1/rosetta/__init__.py
-drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-07-02 15:50:05.762004 rosetta-ce-1.4.1/rosetta/constants/
--rw-r--r--   0 amahmoud   (502) staff       (20)        0 2023-04-12 16:36:37.000000 rosetta-ce-1.4.1/rosetta/constants/__init__.py
--rw-r--r--   0 amahmoud   (502) staff       (20)     1936 2023-04-09 13:32:25.000000 rosetta-ce-1.4.1/rosetta/constants/sensors.py
--rw-r--r--   0 amahmoud   (502) staff       (20)     1658 2023-04-25 15:36:11.000000 rosetta-ce-1.4.1/rosetta/constants/sources.py
--rw-r--r--   0 amahmoud   (502) staff       (20)     6697 2023-04-25 15:36:11.000000 rosetta-ce-1.4.1/rosetta/constants/systems.py
--rw-r--r--   0 amahmoud   (502) staff       (20)     3008 2023-04-26 09:01:43.000000 rosetta-ce-1.4.1/rosetta/rconverter.py
--rw-r--r--   0 amahmoud   (502) staff       (20)    42827 2023-07-02 15:44:30.000000 rosetta-ce-1.4.1/rosetta/rfaker.py
--rw-r--r--   0 amahmoud   (502) staff       (20)     8572 2023-06-29 15:55:20.000000 rosetta-ce-1.4.1/rosetta/rsender.py
-drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-07-02 15:50:05.764091 rosetta-ce-1.4.1/rosetta_ce.egg-info/
--rw-r--r--   0 amahmoud   (502) staff       (20)    11253 2023-07-02 15:50:05.000000 rosetta-ce-1.4.1/rosetta_ce.egg-info/PKG-INFO
--rw-r--r--   0 amahmoud   (502) staff       (20)      459 2023-07-02 15:50:05.000000 rosetta-ce-1.4.1/rosetta_ce.egg-info/SOURCES.txt
--rw-r--r--   0 amahmoud   (502) staff       (20)        1 2023-07-02 15:50:05.000000 rosetta-ce-1.4.1/rosetta_ce.egg-info/dependency_links.txt
--rw-r--r--   0 amahmoud   (502) staff       (20)       23 2023-07-02 15:50:05.000000 rosetta-ce-1.4.1/rosetta_ce.egg-info/requires.txt
--rw-r--r--   0 amahmoud   (502) staff       (20)        8 2023-07-02 15:50:05.000000 rosetta-ce-1.4.1/rosetta_ce.egg-info/top_level.txt
--rw-r--r--   0 amahmoud   (502) staff       (20)       38 2023-07-02 15:50:05.766568 rosetta-ce-1.4.1/setup.cfg
--rw-r--r--   0 amahmoud   (502) staff       (20)      851 2023-07-02 15:47:13.000000 rosetta-ce-1.4.1/setup.py
-drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-07-02 15:50:05.765704 rosetta-ce-1.4.1/tests/
--rw-r--r--   0 amahmoud   (502) staff       (20)     1040 2023-04-26 09:01:43.000000 rosetta-ce-1.4.1/tests/test_rconverter.py
--rw-r--r--   0 amahmoud   (502) staff       (20)     5226 2023-04-25 15:36:11.000000 rosetta-ce-1.4.1/tests/test_rfaker.py
--rw-r--r--   0 amahmoud   (502) staff       (20)     1763 2023-04-26 09:02:44.000000 rosetta-ce-1.4.1/tests/test_rsender.py
+drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-07-02 15:59:53.402395 rosetta-ce-1.4.2/
+-rw-r--r--   0 amahmoud   (502) staff       (20)     1070 2023-04-08 17:22:13.000000 rosetta-ce-1.4.2/LICENSE
+-rw-r--r--   0 amahmoud   (502) staff       (20)    11253 2023-07-02 15:59:53.402075 rosetta-ce-1.4.2/PKG-INFO
+-rw-r--r--   0 amahmoud   (502) staff       (20)    10721 2023-06-29 06:50:02.000000 rosetta-ce-1.4.2/README.md
+drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-07-02 15:59:53.396174 rosetta-ce-1.4.2/rosetta/
+-rw-r--r--   0 amahmoud   (502) staff       (20)       92 2023-04-09 08:11:12.000000 rosetta-ce-1.4.2/rosetta/__init__.py
+drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-07-02 15:59:53.397945 rosetta-ce-1.4.2/rosetta/constants/
+-rw-r--r--   0 amahmoud   (502) staff       (20)        0 2023-04-12 16:36:37.000000 rosetta-ce-1.4.2/rosetta/constants/__init__.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)     1936 2023-04-09 13:32:25.000000 rosetta-ce-1.4.2/rosetta/constants/sensors.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)     1658 2023-04-25 15:36:11.000000 rosetta-ce-1.4.2/rosetta/constants/sources.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)     6697 2023-04-25 15:36:11.000000 rosetta-ce-1.4.2/rosetta/constants/systems.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)     3008 2023-04-26 09:01:43.000000 rosetta-ce-1.4.2/rosetta/rconverter.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)    43246 2023-07-02 15:59:06.000000 rosetta-ce-1.4.2/rosetta/rfaker.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)     8572 2023-06-29 15:55:20.000000 rosetta-ce-1.4.2/rosetta/rsender.py
+drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-07-02 15:59:53.399825 rosetta-ce-1.4.2/rosetta_ce.egg-info/
+-rw-r--r--   0 amahmoud   (502) staff       (20)    11253 2023-07-02 15:59:53.000000 rosetta-ce-1.4.2/rosetta_ce.egg-info/PKG-INFO
+-rw-r--r--   0 amahmoud   (502) staff       (20)      459 2023-07-02 15:59:53.000000 rosetta-ce-1.4.2/rosetta_ce.egg-info/SOURCES.txt
+-rw-r--r--   0 amahmoud   (502) staff       (20)        1 2023-07-02 15:59:53.000000 rosetta-ce-1.4.2/rosetta_ce.egg-info/dependency_links.txt
+-rw-r--r--   0 amahmoud   (502) staff       (20)       23 2023-07-02 15:59:53.000000 rosetta-ce-1.4.2/rosetta_ce.egg-info/requires.txt
+-rw-r--r--   0 amahmoud   (502) staff       (20)        8 2023-07-02 15:59:53.000000 rosetta-ce-1.4.2/rosetta_ce.egg-info/top_level.txt
+-rw-r--r--   0 amahmoud   (502) staff       (20)       38 2023-07-02 15:59:53.402449 rosetta-ce-1.4.2/setup.cfg
+-rw-r--r--   0 amahmoud   (502) staff       (20)      851 2023-07-02 15:59:14.000000 rosetta-ce-1.4.2/setup.py
+drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-07-02 15:59:53.401502 rosetta-ce-1.4.2/tests/
+-rw-r--r--   0 amahmoud   (502) staff       (20)     1040 2023-04-26 09:01:43.000000 rosetta-ce-1.4.2/tests/test_rconverter.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)     5226 2023-04-25 15:36:11.000000 rosetta-ce-1.4.2/tests/test_rfaker.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)     1763 2023-04-26 09:02:44.000000 rosetta-ce-1.4.2/tests/test_rsender.py
```

### Comparing `rosetta-ce-1.4.1/LICENSE` & `rosetta-ce-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.4.1/PKG-INFO` & `rosetta-ce-1.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rosetta-ce
-Version: 1.4.1
+Version: 1.4.2
 Summary: Rosetta is a Python package that can be used to fake security logs and alerts for testing different detection and response use cases.
 Home-page: https://github.com/ayman-m/rosetta
 Author: Ayman Mahmoud
 Author-email: content@ayman.online
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `rosetta-ce-1.4.1/README.md` & `rosetta-ce-1.4.2/README.md`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.4.1/rosetta/constants/sensors.py` & `rosetta-ce-1.4.2/rosetta/constants/sensors.py`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.4.1/rosetta/constants/sources.py` & `rosetta-ce-1.4.2/rosetta/constants/sources.py`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.4.1/rosetta/constants/systems.py` & `rosetta-ce-1.4.2/rosetta/constants/systems.py`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.4.1/rosetta/rconverter.py` & `rosetta-ce-1.4.2/rosetta/rconverter.py`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.4.1/rosetta/rfaker.py` & `rosetta-ce-1.4.2/rosetta/rfaker.py`

 * *Files 2% similar despite different names*

```diff
@@ -714,28 +714,30 @@
                         event[observable] = random.choice(observable_value)
             json_messages.append(event)
         return json_messages
 
     @classmethod
     def incidents(cls, count, fields: Optional[str] = None, timestamp: Optional[datetime] = None,
                   vendor: Optional[str] = None, product: Optional[str] = None, version: Optional[str] = None,
-                  observables: Optional[Observables] = None) -> List[dict]:
+                  observables: Optional[Observables] = None, required_fields: Optional[str] = None) -> List[dict]:
         """
         Generates a list of fake incident data.
 
         Args:
             count (int): The number of incidents to generate.
             fields (str, optional): A comma-separated list of incident fields to include in the output. If None,
                 all fields will be included. Valid options are: 'id', 'duration', 'type', 'analyst', 'severity',
                 'description', 'events'.
             vendor: Optional. The vendor.
             product: Optional. The product.
             version: Optional. The version.
             timestamp: Optional. The starting timestamp for the syslog messages. If not provided, a random time during
             observables: An observables object. If not provided, random objservable will be generated and used.
+            required_fields: Optional. A list of fields that are required to present in the generated data, whether from
+            observables or randomely.
 
         Returns:
             List[Dict]: A list of incident dictionaries. Each dictionary contains the following fields:
                 - 'id' (int): A unique identifier for the incident.
                 - 'type' (str): The type of incident.
                 - 'duration' (int): The duration of the incident in hours.
                 - 'analyst' (str): The name of the analyst assigned to the incident.
@@ -797,22 +799,24 @@
                 if 'severity' in field_list:
                     incident['severity'] = severity
                 if 'description' in field_list:
                     incident_description = faker.paragraph(nb_sentences=1, ext_word_list=description)
                     incident['description'] = incident_description
                 if 'events' in field_list:
                     incident['events'] = [
-                        {"event": cls.syslog(count=1, timestamp=timestamp, observables=observables)[0]},
-                        {"event": cls.cef(count=1, timestamp=timestamp, vendor=vendor, product=product,
-                                          version=version, observables=observables)[0]},
+                        {"event": cls.syslog(count=1, timestamp=timestamp, observables=observables,
+                                             required_fields=required_fields)[0]},
+                        {"event": cls.cef(count=1, timestamp=timestamp, vendor=vendor, product=product, version=version
+                                          , observables=observables, required_fields=required_fields)[0]},
                         {"event": cls.leef(count=1, timestamp=timestamp, vendor=vendor, product=product,
-                                           version=version, observables=observables)[0]},
+                                           version=version, observables=observables, required_fields=required_fields)[0]},
                         {"event": cls.winevent(count=1, timestamp=timestamp, observables=observables)[0]},
                         {"event": cls.json(count=1, timestamp=timestamp, vendor=vendor, product=product,
-                                           version=version, observables=observables)[0]}
+                                           version=version, observables=observables,
+                                           required_fields=required_fields)[0]}
                     ]
             else:
                 incident = {
                     "id": incident_id,
                     "type": incident_type,
                     "duration": duration,
                     "analyst": analyst
```

### Comparing `rosetta-ce-1.4.1/rosetta/rsender.py` & `rosetta-ce-1.4.2/rosetta/rsender.py`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.4.1/rosetta_ce.egg-info/PKG-INFO` & `rosetta-ce-1.4.2/rosetta_ce.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rosetta-ce
-Version: 1.4.1
+Version: 1.4.2
 Summary: Rosetta is a Python package that can be used to fake security logs and alerts for testing different detection and response use cases.
 Home-page: https://github.com/ayman-m/rosetta
 Author: Ayman Mahmoud
 Author-email: content@ayman.online
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `rosetta-ce-1.4.1/setup.py` & `rosetta-ce-1.4.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="rosetta-ce",
-    version="1.4.1",
+    version="1.4.2",
     author="Ayman Mahmoud",
     author_email="content@ayman.online",
     description="Rosetta is a Python package that can be used to fake security logs and alerts for testing different "
                 "detection and response use cases.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ayman-m/rosetta",
```

### Comparing `rosetta-ce-1.4.1/tests/test_rconverter.py` & `rosetta-ce-1.4.2/tests/test_rconverter.py`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.4.1/tests/test_rfaker.py` & `rosetta-ce-1.4.2/tests/test_rfaker.py`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.4.1/tests/test_rsender.py` & `rosetta-ce-1.4.2/tests/test_rsender.py`

 * *Files identical despite different names*

