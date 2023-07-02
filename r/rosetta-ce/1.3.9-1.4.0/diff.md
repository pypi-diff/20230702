# Comparing `tmp/rosetta-ce-1.3.9.tar.gz` & `tmp/rosetta-ce-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rosetta-ce-1.3.9.tar", last modified: Sat Jul  1 06:47:16 2023, max compression
+gzip compressed data, was "rosetta-ce-1.4.0.tar", last modified: Sun Jul  2 08:56:40 2023, max compression
```

## Comparing `rosetta-ce-1.3.9.tar` & `rosetta-ce-1.4.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-07-01 06:47:16.806053 rosetta-ce-1.3.9/
--rw-r--r--   0 amahmoud   (502) staff       (20)     1070 2023-04-08 17:22:13.000000 rosetta-ce-1.3.9/LICENSE
--rw-r--r--   0 amahmoud   (502) staff       (20)    11253 2023-07-01 06:47:16.805736 rosetta-ce-1.3.9/PKG-INFO
--rw-r--r--   0 amahmoud   (502) staff       (20)    10721 2023-06-29 06:50:02.000000 rosetta-ce-1.3.9/README.md
-drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-07-01 06:47:16.799929 rosetta-ce-1.3.9/rosetta/
--rw-r--r--   0 amahmoud   (502) staff       (20)       92 2023-04-09 08:11:12.000000 rosetta-ce-1.3.9/rosetta/__init__.py
-drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-07-01 06:47:16.802029 rosetta-ce-1.3.9/rosetta/constants/
--rw-r--r--   0 amahmoud   (502) staff       (20)        0 2023-04-12 16:36:37.000000 rosetta-ce-1.3.9/rosetta/constants/__init__.py
--rw-r--r--   0 amahmoud   (502) staff       (20)     1936 2023-04-09 13:32:25.000000 rosetta-ce-1.3.9/rosetta/constants/sensors.py
--rw-r--r--   0 amahmoud   (502) staff       (20)     1658 2023-04-25 15:36:11.000000 rosetta-ce-1.3.9/rosetta/constants/sources.py
--rw-r--r--   0 amahmoud   (502) staff       (20)     6697 2023-04-25 15:36:11.000000 rosetta-ce-1.3.9/rosetta/constants/systems.py
--rw-r--r--   0 amahmoud   (502) staff       (20)     3008 2023-04-26 09:01:43.000000 rosetta-ce-1.3.9/rosetta/rconverter.py
--rw-r--r--   0 amahmoud   (502) staff       (20)    43882 2023-07-01 06:45:41.000000 rosetta-ce-1.3.9/rosetta/rfaker.py
--rw-r--r--   0 amahmoud   (502) staff       (20)     8572 2023-06-29 15:55:20.000000 rosetta-ce-1.3.9/rosetta/rsender.py
-drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-07-01 06:47:16.803809 rosetta-ce-1.3.9/rosetta_ce.egg-info/
--rw-r--r--   0 amahmoud   (502) staff       (20)    11253 2023-07-01 06:47:16.000000 rosetta-ce-1.3.9/rosetta_ce.egg-info/PKG-INFO
--rw-r--r--   0 amahmoud   (502) staff       (20)      459 2023-07-01 06:47:16.000000 rosetta-ce-1.3.9/rosetta_ce.egg-info/SOURCES.txt
--rw-r--r--   0 amahmoud   (502) staff       (20)        1 2023-07-01 06:47:16.000000 rosetta-ce-1.3.9/rosetta_ce.egg-info/dependency_links.txt
--rw-r--r--   0 amahmoud   (502) staff       (20)       23 2023-07-01 06:47:16.000000 rosetta-ce-1.3.9/rosetta_ce.egg-info/requires.txt
--rw-r--r--   0 amahmoud   (502) staff       (20)        8 2023-07-01 06:47:16.000000 rosetta-ce-1.3.9/rosetta_ce.egg-info/top_level.txt
--rw-r--r--   0 amahmoud   (502) staff       (20)       38 2023-07-01 06:47:16.806090 rosetta-ce-1.3.9/setup.cfg
--rw-r--r--   0 amahmoud   (502) staff       (20)      851 2023-07-01 06:45:54.000000 rosetta-ce-1.3.9/setup.py
-drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-07-01 06:47:16.805261 rosetta-ce-1.3.9/tests/
--rw-r--r--   0 amahmoud   (502) staff       (20)     1040 2023-04-26 09:01:43.000000 rosetta-ce-1.3.9/tests/test_rconverter.py
--rw-r--r--   0 amahmoud   (502) staff       (20)     5226 2023-04-25 15:36:11.000000 rosetta-ce-1.3.9/tests/test_rfaker.py
--rw-r--r--   0 amahmoud   (502) staff       (20)     1763 2023-04-26 09:02:44.000000 rosetta-ce-1.3.9/tests/test_rsender.py
+drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-07-02 08:56:40.185110 rosetta-ce-1.4.0/
+-rw-r--r--   0 amahmoud   (502) staff       (20)     1070 2023-04-08 17:22:13.000000 rosetta-ce-1.4.0/LICENSE
+-rw-r--r--   0 amahmoud   (502) staff       (20)    11253 2023-07-02 08:56:40.184771 rosetta-ce-1.4.0/PKG-INFO
+-rw-r--r--   0 amahmoud   (502) staff       (20)    10721 2023-06-29 06:50:02.000000 rosetta-ce-1.4.0/README.md
+drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-07-02 08:56:40.178525 rosetta-ce-1.4.0/rosetta/
+-rw-r--r--   0 amahmoud   (502) staff       (20)       92 2023-04-09 08:11:12.000000 rosetta-ce-1.4.0/rosetta/__init__.py
+drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-07-02 08:56:40.180637 rosetta-ce-1.4.0/rosetta/constants/
+-rw-r--r--   0 amahmoud   (502) staff       (20)        0 2023-04-12 16:36:37.000000 rosetta-ce-1.4.0/rosetta/constants/__init__.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)     1936 2023-04-09 13:32:25.000000 rosetta-ce-1.4.0/rosetta/constants/sensors.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)     1658 2023-04-25 15:36:11.000000 rosetta-ce-1.4.0/rosetta/constants/sources.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)     6697 2023-04-25 15:36:11.000000 rosetta-ce-1.4.0/rosetta/constants/systems.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)     3008 2023-04-26 09:01:43.000000 rosetta-ce-1.4.0/rosetta/rconverter.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)    44021 2023-07-02 08:53:18.000000 rosetta-ce-1.4.0/rosetta/rfaker.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)     8572 2023-06-29 15:55:20.000000 rosetta-ce-1.4.0/rosetta/rsender.py
+drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-07-02 08:56:40.182829 rosetta-ce-1.4.0/rosetta_ce.egg-info/
+-rw-r--r--   0 amahmoud   (502) staff       (20)    11253 2023-07-02 08:56:40.000000 rosetta-ce-1.4.0/rosetta_ce.egg-info/PKG-INFO
+-rw-r--r--   0 amahmoud   (502) staff       (20)      459 2023-07-02 08:56:40.000000 rosetta-ce-1.4.0/rosetta_ce.egg-info/SOURCES.txt
+-rw-r--r--   0 amahmoud   (502) staff       (20)        1 2023-07-02 08:56:40.000000 rosetta-ce-1.4.0/rosetta_ce.egg-info/dependency_links.txt
+-rw-r--r--   0 amahmoud   (502) staff       (20)       23 2023-07-02 08:56:40.000000 rosetta-ce-1.4.0/rosetta_ce.egg-info/requires.txt
+-rw-r--r--   0 amahmoud   (502) staff       (20)        8 2023-07-02 08:56:40.000000 rosetta-ce-1.4.0/rosetta_ce.egg-info/top_level.txt
+-rw-r--r--   0 amahmoud   (502) staff       (20)       38 2023-07-02 08:56:40.185148 rosetta-ce-1.4.0/setup.cfg
+-rw-r--r--   0 amahmoud   (502) staff       (20)      851 2023-07-02 08:56:13.000000 rosetta-ce-1.4.0/setup.py
+drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-07-02 08:56:40.184269 rosetta-ce-1.4.0/tests/
+-rw-r--r--   0 amahmoud   (502) staff       (20)     1040 2023-04-26 09:01:43.000000 rosetta-ce-1.4.0/tests/test_rconverter.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)     5226 2023-04-25 15:36:11.000000 rosetta-ce-1.4.0/tests/test_rfaker.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)     1763 2023-04-26 09:02:44.000000 rosetta-ce-1.4.0/tests/test_rsender.py
```

### Comparing `rosetta-ce-1.3.9/LICENSE` & `rosetta-ce-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.3.9/PKG-INFO` & `rosetta-ce-1.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rosetta-ce
-Version: 1.3.9
+Version: 1.4.0
 Summary: Rosetta is a Python package that can be used to fake security logs and alerts for testing different detection and response use cases.
 Home-page: https://github.com/ayman-m/rosetta
 Author: Ayman Mahmoud
 Author-email: content@ayman.online
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `rosetta-ce-1.3.9/README.md` & `rosetta-ce-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.3.9/rosetta/constants/sensors.py` & `rosetta-ce-1.4.0/rosetta/constants/sensors.py`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.3.9/rosetta/constants/sources.py` & `rosetta-ce-1.4.0/rosetta/constants/sources.py`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.3.9/rosetta/constants/systems.py` & `rosetta-ce-1.4.0/rosetta/constants/systems.py`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.3.9/rosetta/rconverter.py` & `rosetta-ce-1.4.0/rosetta/rconverter.py`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.3.9/rosetta/rfaker.py` & `rosetta-ce-1.4.0/rosetta/rfaker.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,28 +26,31 @@
 
 class ObservableKnown(Enum):
     BAD = 'bad'
     GOOD = 'good'
 
 
 class Observables:
-    def __init__(self, src_ip: list = None, dst_ip: Optional[list] = None, src_host: Optional[list] = None,
+    def __init__(self, src_ip: list = None, dst_ip: Optional[list] = None, src_ipv6: list = None,
+                 dst_ipv6: Optional[list] = None, src_host: Optional[list] = None,
                  dst_host: Optional[list] = None, src_domain: Optional[list] = None, dst_domain: Optional[list] = None,
                  sender_email: Optional[list] = None, recipient_email: Optional[list] = None,
                  email_subject: Optional[list] = None, email_body: Optional[list] = None,
                  url: Optional[list] = None, port: Optional[list] = None, protocol: Optional[list] = None,
                  inbound_bytes: Optional[list] = None, outbound_bytes: Optional[list] = None,
                  app: Optional[list] = None, os: Optional[list] = None, user: Optional[list] = None,
                  cve: Optional[list] = None, file_name: Optional[list] = None, file_hash: Optional[list] = None,
                  cmd: Optional[list] = None, process: Optional[list] = None, technique: Optional[list] = None,
                  entry_type: Optional[list] = None, severity: Optional[list] = None, sensor: Optional[list] = None,
                  action: Optional[list] = None, event_id: Optional[list] = None, error_code: Optional[list] = None,
                  terms: Optional[list] = None, incident_types: Optional[list] = None, analysts: Optional[list] = None):
         self.src_ip = src_ip
         self.dst_ip = dst_ip
+        self.src_ipv6 = src_ipv6
+        self.dst_ipv6 = dst_ipv6
         self.src_host = src_host
         self.dst_host = dst_host
         self.src_domain = src_domain
         self.dst_domain = dst_domain
         self.sender_email = sender_email
         self.recipient_email = recipient_email
         self.email_subject = email_subject
```

### Comparing `rosetta-ce-1.3.9/rosetta/rsender.py` & `rosetta-ce-1.4.0/rosetta/rsender.py`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.3.9/rosetta_ce.egg-info/PKG-INFO` & `rosetta-ce-1.4.0/rosetta_ce.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rosetta-ce
-Version: 1.3.9
+Version: 1.4.0
 Summary: Rosetta is a Python package that can be used to fake security logs and alerts for testing different detection and response use cases.
 Home-page: https://github.com/ayman-m/rosetta
 Author: Ayman Mahmoud
 Author-email: content@ayman.online
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `rosetta-ce-1.3.9/setup.py` & `rosetta-ce-1.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="rosetta-ce",
-    version="1.3.9",
+    version="1.4.0",
     author="Ayman Mahmoud",
     author_email="content@ayman.online",
     description="Rosetta is a Python package that can be used to fake security logs and alerts for testing different "
                 "detection and response use cases.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ayman-m/rosetta",
```

### Comparing `rosetta-ce-1.3.9/tests/test_rconverter.py` & `rosetta-ce-1.4.0/tests/test_rconverter.py`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.3.9/tests/test_rfaker.py` & `rosetta-ce-1.4.0/tests/test_rfaker.py`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.3.9/tests/test_rsender.py` & `rosetta-ce-1.4.0/tests/test_rsender.py`

 * *Files identical despite different names*

