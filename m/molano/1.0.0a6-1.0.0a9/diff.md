# Comparing `tmp/molano-1.0.0a6.tar.gz` & `tmp/molano-1.0.0a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "molano-1.0.0a6.tar", last modified: Sat Mar  4 15:02:23 2023, max compression
+gzip compressed data, was "molano-1.0.0a9.tar", last modified: Sat Mar  4 22:18:50 2023, max compression
```

## Comparing `molano-1.0.0a6.tar` & `molano-1.0.0a9.tar`

### file list

```diff
@@ -1,44 +1,45 @@
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-04 15:02:23.637575 molano-1.0.0a6/
--rw-r--r--   0 cochise    (501) staff       (20)      298 2022-10-12 13:09:40.000000 molano-1.0.0a6/MANIFEST.in
--rw-r--r--   0 cochise    (501) staff       (20)      899 2023-03-04 15:02:23.637412 molano-1.0.0a6/PKG-INFO
--rw-r--r--   0 cochise    (501) staff       (20)       12 2023-03-04 15:02:13.000000 molano-1.0.0a6/VERSION
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-04 15:02:23.633822 molano-1.0.0a6/molano/
--rw-r--r--   0 cochise    (501) staff       (20)        0 2022-10-12 13:09:40.000000 molano-1.0.0a6/molano/__init__.py
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-04 15:02:23.636200 molano-1.0.0a6/molano/canon/
--rw-r--r--   0 cochise    (501) staff       (20)     1088 2023-03-04 12:19:07.000000 molano-1.0.0a6/molano/canon/__init__.py
--rw-r--r--   0 cochise    (501) staff       (20)      572 2023-03-01 10:52:58.000000 molano-1.0.0a6/molano/canon/appleudid.py
--rw-r--r--   0 cochise    (501) staff       (20)      575 2023-03-01 14:19:27.000000 molano-1.0.0a6/molano/canon/decimalmeid.py
--rw-r--r--   0 cochise    (501) staff       (20)      464 2023-03-01 10:53:01.000000 molano-1.0.0a6/molano/canon/deviceinfo.py
--rw-r--r--   0 cochise    (501) staff       (20)      558 2023-03-01 10:53:04.000000 molano-1.0.0a6/molano/canon/deviceinspector.py
--rw-r--r--   0 cochise    (501) staff       (20)      494 2023-03-01 10:53:06.000000 molano-1.0.0a6/molano/canon/devicereportsource.py
--rw-r--r--   0 cochise    (501) staff       (20)      948 2023-03-01 22:51:51.000000 molano-1.0.0a6/molano/canon/deviceserialnumber.py
--rw-r--r--   0 cochise    (501) staff       (20)      501 2023-03-04 11:54:48.000000 molano-1.0.0a6/molano/canon/documentreference.py
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-04 15:02:23.636693 molano-1.0.0a6/molano/canon/events/
--rw-r--r--   0 cochise    (501) staff       (20)      615 2023-03-04 10:40:18.000000 molano-1.0.0a6/molano/canon/events/__init__.py
--rw-r--r--   0 cochise    (501) staff       (20)      788 2023-02-28 20:18:22.000000 molano-1.0.0a6/molano/canon/events/devicegraded.py
--rw-r--r--   0 cochise    (501) staff       (20)      777 2023-02-28 18:44:08.000000 molano-1.0.0a6/molano/canon/events/deviceinspected.py
--rw-r--r--   0 cochise    (501) staff       (20)      803 2023-03-04 12:08:05.000000 molano-1.0.0a6/molano/canon/events/devicereceived.py
--rw-r--r--   0 cochise    (501) staff       (20)      489 2023-03-01 15:49:47.000000 molano-1.0.0a6/molano/canon/imei.py
--rw-r--r--   0 cochise    (501) staff       (20)      567 2023-03-01 10:53:13.000000 molano-1.0.0a6/molano/canon/meid.py
--rw-r--r--   0 cochise    (501) staff       (20)      580 2023-03-02 15:34:29.000000 molano-1.0.0a6/molano/canon/ordernumber.py
--rw-r--r--   0 cochise    (501) staff       (20)     1193 2023-03-02 00:30:13.000000 molano-1.0.0a6/molano/canon/privateenterprisenumber.py
--rw-r--r--   0 cochise    (501) staff       (20)      589 2023-03-02 17:10:29.000000 molano-1.0.0a6/molano/canon/purchaseordernumber.py
--rw-r--r--   0 cochise    (501) staff       (20)      597 2023-03-04 12:07:51.000000 molano-1.0.0a6/molano/canon/trackedmobiledevicereference.py
--rw-r--r--   0 cochise    (501) staff       (20)     1160 2023-03-04 12:11:45.000000 molano-1.0.0a6/molano/package.json
--rw-r--r--   0 cochise    (501) staff       (20)     1222 2022-12-21 13:21:38.000000 molano-1.0.0a6/molano/runlevel.py
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-04 15:02:23.636917 molano-1.0.0a6/molano/runtime/
--rw-r--r--   0 cochise    (501) staff       (20)      888 2023-02-28 18:31:39.000000 molano-1.0.0a6/molano/runtime/ioc.py
--rw-r--r--   0 cochise    (501) staff       (20)      394 2023-02-28 18:31:36.000000 molano-1.0.0a6/molano/runtime/settings.py
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-04 15:02:23.637248 molano-1.0.0a6/molano/tests/
--rw-r--r--   0 cochise    (501) staff       (20)      357 2022-10-12 13:09:40.000000 molano-1.0.0a6/molano/tests/test_integration_noop.py
--rw-r--r--   0 cochise    (501) staff       (20)      347 2022-10-12 13:09:40.000000 molano-1.0.0a6/molano/tests/test_system_noop.py
--rw-r--r--   0 cochise    (501) staff       (20)      343 2022-10-12 13:09:40.000000 molano-1.0.0a6/molano/tests/test_unit_noop.py
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-04 15:02:23.634478 molano-1.0.0a6/molano.egg-info/
--rw-r--r--   0 cochise    (501) staff       (20)      899 2023-03-04 15:02:23.000000 molano-1.0.0a6/molano.egg-info/PKG-INFO
--rw-r--r--   0 cochise    (501) staff       (20)      997 2023-03-04 15:02:23.000000 molano-1.0.0a6/molano.egg-info/SOURCES.txt
--rw-r--r--   0 cochise    (501) staff       (20)        1 2023-03-04 15:02:23.000000 molano-1.0.0a6/molano.egg-info/dependency_links.txt
--rw-r--r--   0 cochise    (501) staff       (20)       55 2023-03-04 15:02:23.000000 molano-1.0.0a6/molano.egg-info/entry_points.txt
--rw-r--r--   0 cochise    (501) staff       (20)      121 2023-03-04 15:02:23.000000 molano-1.0.0a6/molano.egg-info/requires.txt
--rw-r--r--   0 cochise    (501) staff       (20)       17 2023-03-04 15:02:23.000000 molano-1.0.0a6/molano.egg-info/top_level.txt
--rw-r--r--   0 cochise    (501) staff       (20)       38 2023-03-04 15:02:23.637611 molano-1.0.0a6/setup.cfg
--rw-r--r--   0 cochise    (501) staff       (20)     1262 2022-10-12 14:27:11.000000 molano-1.0.0a6/setup.py
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-04 22:18:50.310930 molano-1.0.0a9/
+-rw-r--r--   0 cochise    (501) staff       (20)      298 2022-10-12 13:09:40.000000 molano-1.0.0a9/MANIFEST.in
+-rw-r--r--   0 cochise    (501) staff       (20)      899 2023-03-04 22:18:50.310749 molano-1.0.0a9/PKG-INFO
+-rw-r--r--   0 cochise    (501) staff       (20)       12 2023-03-04 22:18:46.000000 molano-1.0.0a9/VERSION
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-04 22:18:50.302024 molano-1.0.0a9/molano/
+-rw-r--r--   0 cochise    (501) staff       (20)        0 2022-10-12 13:09:40.000000 molano-1.0.0a9/molano/__init__.py
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-04 22:18:50.307911 molano-1.0.0a9/molano/canon/
+-rw-r--r--   0 cochise    (501) staff       (20)     1150 2023-03-04 18:16:42.000000 molano-1.0.0a9/molano/canon/__init__.py
+-rw-r--r--   0 cochise    (501) staff       (20)      572 2023-03-01 10:52:58.000000 molano-1.0.0a9/molano/canon/appleudid.py
+-rw-r--r--   0 cochise    (501) staff       (20)      575 2023-03-01 14:19:27.000000 molano-1.0.0a9/molano/canon/decimalmeid.py
+-rw-r--r--   0 cochise    (501) staff       (20)      464 2023-03-01 10:53:01.000000 molano-1.0.0a9/molano/canon/deviceinfo.py
+-rw-r--r--   0 cochise    (501) staff       (20)      558 2023-03-01 10:53:04.000000 molano-1.0.0a9/molano/canon/deviceinspector.py
+-rw-r--r--   0 cochise    (501) staff       (20)      494 2023-03-01 10:53:06.000000 molano-1.0.0a9/molano/canon/devicereportsource.py
+-rw-r--r--   0 cochise    (501) staff       (20)      948 2023-03-01 22:51:51.000000 molano-1.0.0a9/molano/canon/deviceserialnumber.py
+-rw-r--r--   0 cochise    (501) staff       (20)      571 2023-03-04 17:03:43.000000 molano-1.0.0a9/molano/canon/documentreference.py
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-04 22:18:50.309066 molano-1.0.0a9/molano/canon/events/
+-rw-r--r--   0 cochise    (501) staff       (20)      615 2023-03-04 10:40:18.000000 molano-1.0.0a9/molano/canon/events/__init__.py
+-rw-r--r--   0 cochise    (501) staff       (20)      788 2023-02-28 20:18:22.000000 molano-1.0.0a9/molano/canon/events/devicegraded.py
+-rw-r--r--   0 cochise    (501) staff       (20)      777 2023-02-28 18:44:08.000000 molano-1.0.0a9/molano/canon/events/deviceinspected.py
+-rw-r--r--   0 cochise    (501) staff       (20)      864 2023-03-04 20:19:47.000000 molano-1.0.0a9/molano/canon/events/devicereceived.py
+-rw-r--r--   0 cochise    (501) staff       (20)      489 2023-03-01 15:49:47.000000 molano-1.0.0a9/molano/canon/imei.py
+-rw-r--r--   0 cochise    (501) staff       (20)      567 2023-03-01 10:53:13.000000 molano-1.0.0a9/molano/canon/meid.py
+-rw-r--r--   0 cochise    (501) staff       (20)      580 2023-03-02 15:34:29.000000 molano-1.0.0a9/molano/canon/ordernumber.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1193 2023-03-02 00:30:13.000000 molano-1.0.0a9/molano/canon/privateenterprisenumber.py
+-rw-r--r--   0 cochise    (501) staff       (20)      589 2023-03-02 17:10:29.000000 molano-1.0.0a9/molano/canon/purchaseordernumber.py
+-rw-r--r--   0 cochise    (501) staff       (20)      583 2023-03-04 18:16:29.000000 molano-1.0.0a9/molano/canon/receiptnumber.py
+-rw-r--r--   0 cochise    (501) staff       (20)      597 2023-03-04 12:07:51.000000 molano-1.0.0a9/molano/canon/trackedmobiledevicereference.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1160 2023-03-04 12:11:45.000000 molano-1.0.0a9/molano/package.json
+-rw-r--r--   0 cochise    (501) staff       (20)     1222 2022-12-21 13:21:38.000000 molano-1.0.0a9/molano/runlevel.py
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-04 22:18:50.309760 molano-1.0.0a9/molano/runtime/
+-rw-r--r--   0 cochise    (501) staff       (20)      888 2023-02-28 18:31:39.000000 molano-1.0.0a9/molano/runtime/ioc.py
+-rw-r--r--   0 cochise    (501) staff       (20)      394 2023-02-28 18:31:36.000000 molano-1.0.0a9/molano/runtime/settings.py
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-04 22:18:50.310500 molano-1.0.0a9/molano/tests/
+-rw-r--r--   0 cochise    (501) staff       (20)      357 2022-10-12 13:09:40.000000 molano-1.0.0a9/molano/tests/test_integration_noop.py
+-rw-r--r--   0 cochise    (501) staff       (20)      347 2022-10-12 13:09:40.000000 molano-1.0.0a9/molano/tests/test_system_noop.py
+-rw-r--r--   0 cochise    (501) staff       (20)      343 2022-10-12 13:09:40.000000 molano-1.0.0a9/molano/tests/test_unit_noop.py
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-03-04 22:18:50.303186 molano-1.0.0a9/molano.egg-info/
+-rw-r--r--   0 cochise    (501) staff       (20)      899 2023-03-04 22:18:50.000000 molano-1.0.0a9/molano.egg-info/PKG-INFO
+-rw-r--r--   0 cochise    (501) staff       (20)     1027 2023-03-04 22:18:50.000000 molano-1.0.0a9/molano.egg-info/SOURCES.txt
+-rw-r--r--   0 cochise    (501) staff       (20)        1 2023-03-04 22:18:50.000000 molano-1.0.0a9/molano.egg-info/dependency_links.txt
+-rw-r--r--   0 cochise    (501) staff       (20)       55 2023-03-04 22:18:50.000000 molano-1.0.0a9/molano.egg-info/entry_points.txt
+-rw-r--r--   0 cochise    (501) staff       (20)      121 2023-03-04 22:18:50.000000 molano-1.0.0a9/molano.egg-info/requires.txt
+-rw-r--r--   0 cochise    (501) staff       (20)       17 2023-03-04 22:18:50.000000 molano-1.0.0a9/molano.egg-info/top_level.txt
+-rw-r--r--   0 cochise    (501) staff       (20)       38 2023-03-04 22:18:50.310970 molano-1.0.0a9/setup.cfg
+-rw-r--r--   0 cochise    (501) staff       (20)     1262 2022-10-12 14:27:11.000000 molano-1.0.0a9/setup.py
```

### Comparing `molano-1.0.0a6/PKG-INFO` & `molano-1.0.0a9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molano
-Version: 1.0.0a6
+Version: 1.0.0a9
 Summary: Molano Common Library
 Home-page: https://gitlab.com/unimatrixone
 Author: Cochise Ruhulessin
 Author-email: cochise.ruhulessin@unimatrixone.io
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
```

### Comparing `molano-1.0.0a6/molano/canon/__init__.py` & `molano-1.0.0a9/molano/canon/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,22 +11,24 @@
 from .deviceserialnumber import DeviceSerialNumber
 from .documentreference import DocumentReference
 from .imei import IMEI
 from .meid import MEID
 from .privateenterprisenumber import PrivateEnterpriseNumber
 from .ordernumber import OrderNumber
 from .purchaseordernumber import PurchaseOrderNumber
+from .receiptnumber import ReceiptNumber
 from .trackedmobiledevicereference import TrackedMobileDeviceReference
 
 
 __all__: list[str] = [
     'AppleUDID',
     'DecimalMEID',
     'DeviceSerialNumber',
     'DocumentReference',
     'IMEI',
     'MEID',
     'PrivateEnterpriseNumber',
     'OrderNumber',
     'PurchaseOrderNumber',
+    'ReceiptNumber',
     'TrackedMobileDeviceReference',
 ]
```

### Comparing `molano-1.0.0a6/molano/canon/appleudid.py` & `molano-1.0.0a9/molano/canon/appleudid.py`

 * *Files identical despite different names*

### Comparing `molano-1.0.0a6/molano/canon/decimalmeid.py` & `molano-1.0.0a9/molano/canon/decimalmeid.py`

 * *Files identical despite different names*

### Comparing `molano-1.0.0a6/molano/canon/deviceinspector.py` & `molano-1.0.0a9/molano/canon/deviceinspector.py`

 * *Files identical despite different names*

### Comparing `molano-1.0.0a6/molano/canon/deviceserialnumber.py` & `molano-1.0.0a9/molano/canon/deviceserialnumber.py`

 * *Files identical despite different names*

### Comparing `molano-1.0.0a6/molano/canon/events/__init__.py` & `molano-1.0.0a9/molano/canon/events/__init__.py`

 * *Files identical despite different names*

### Comparing `molano-1.0.0a6/molano/canon/events/devicegraded.py` & `molano-1.0.0a9/molano/canon/events/devicegraded.py`

 * *Files identical despite different names*

### Comparing `molano-1.0.0a6/molano/canon/events/deviceinspected.py` & `molano-1.0.0a9/molano/canon/events/deviceinspected.py`

 * *Files identical despite different names*

### Comparing `molano-1.0.0a6/molano/canon/events/devicereceived.py` & `molano-1.0.0a9/molano/canon/events/devicereceived.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,8 +17,10 @@
 
 
 class DeviceReceived(aorta.Event):
     device: TrackedMobileDeviceReference
     timestamp: datetime
     document: DocumentReference
     handler: EmailAddress
-    imei: list[IMEI]
+    imei: list[IMEI]
+    product_id: int | None = None
+    sku: str | None = None
```

### Comparing `molano-1.0.0a6/molano/canon/meid.py` & `molano-1.0.0a9/molano/canon/meid.py`

 * *Files identical despite different names*

### Comparing `molano-1.0.0a6/molano/canon/ordernumber.py` & `molano-1.0.0a9/molano/canon/ordernumber.py`

 * *Files identical despite different names*

### Comparing `molano-1.0.0a6/molano/canon/privateenterprisenumber.py` & `molano-1.0.0a9/molano/canon/privateenterprisenumber.py`

 * *Files identical despite different names*

### Comparing `molano-1.0.0a6/molano/canon/purchaseordernumber.py` & `molano-1.0.0a9/molano/canon/purchaseordernumber.py`

 * *Files identical despite different names*

### Comparing `molano-1.0.0a6/molano/canon/trackedmobiledevicereference.py` & `molano-1.0.0a9/molano/canon/trackedmobiledevicereference.py`

 * *Files identical despite different names*

### Comparing `molano-1.0.0a6/molano/package.json` & `molano-1.0.0a9/molano/package.json`

 * *Files identical despite different names*

### Comparing `molano-1.0.0a6/molano/runlevel.py` & `molano-1.0.0a9/molano/runlevel.py`

 * *Files identical despite different names*

### Comparing `molano-1.0.0a6/molano/runtime/ioc.py` & `molano-1.0.0a9/molano/runtime/ioc.py`

 * *Files identical despite different names*

### Comparing `molano-1.0.0a6/molano.egg-info/PKG-INFO` & `molano-1.0.0a9/molano.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molano
-Version: 1.0.0a6
+Version: 1.0.0a9
 Summary: Molano Common Library
 Home-page: https://gitlab.com/unimatrixone
 Author: Cochise Ruhulessin
 Author-email: cochise.ruhulessin@unimatrixone.io
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
```

### Comparing `molano-1.0.0a6/molano.egg-info/SOURCES.txt` & `molano-1.0.0a9/molano.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 molano/canon/deviceserialnumber.py
 molano/canon/documentreference.py
 molano/canon/imei.py
 molano/canon/meid.py
 molano/canon/ordernumber.py
 molano/canon/privateenterprisenumber.py
 molano/canon/purchaseordernumber.py
+molano/canon/receiptnumber.py
 molano/canon/trackedmobiledevicereference.py
 molano/canon/events/__init__.py
 molano/canon/events/devicegraded.py
 molano/canon/events/deviceinspected.py
 molano/canon/events/devicereceived.py
 molano/runtime/ioc.py
 molano/runtime/settings.py
```

### Comparing `molano-1.0.0a6/setup.py` & `molano-1.0.0a9/setup.py`

 * *Files identical despite different names*

