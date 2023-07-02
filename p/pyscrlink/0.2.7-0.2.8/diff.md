# Comparing `tmp/pyscrlink-0.2.7.tar.gz` & `tmp/pyscrlink-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyscrlink-0.2.7.tar", last modified: Tue Mar 21 08:19:58 2023, max compression
+gzip compressed data, was "pyscrlink-0.2.8.tar", last modified: Sun Jul  2 13:07:23 2023, max compression
```

## Comparing `pyscrlink-0.2.7.tar` & `pyscrlink-0.2.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 shin      (1000) shin      (1000)        0 2023-03-21 08:19:58.010416 pyscrlink-0.2.7/
--rw-r--r--   0 shin      (1000) shin      (1000)     1528 2020-01-25 09:58:35.000000 pyscrlink-0.2.7/LICENSE
--rw-r--r--   0 shin      (1000) shin      (1000)     7817 2023-03-21 08:19:58.010416 pyscrlink-0.2.7/PKG-INFO
--rw-r--r--   0 shin      (1000) shin      (1000)     7370 2023-03-21 08:17:08.000000 pyscrlink-0.2.7/README.md
-drwxr-xr-x   0 shin      (1000) shin      (1000)        0 2023-03-21 08:19:58.010416 pyscrlink-0.2.7/pyscrlink/
--rw-r--r--   0 shin      (1000) shin      (1000)        0 2021-10-10 06:37:32.000000 pyscrlink-0.2.7/pyscrlink/__init__.py
--rw-r--r--   0 shin      (1000) shin      (1000)      108 2021-10-10 06:37:32.000000 pyscrlink-0.2.7/pyscrlink/__main__.py
--rwxr-xr-x   0 shin      (1000) shin      (1000)     2276 2021-10-10 06:37:32.000000 pyscrlink-0.2.7/pyscrlink/bluepy_helper_cap.py
--rwxr-xr-x   0 shin      (1000) shin      (1000)     6267 2023-03-21 06:55:40.000000 pyscrlink-0.2.7/pyscrlink/gencert.py
--rwxr-xr-x   0 shin      (1000) shin      (1000)    23169 2023-03-21 07:56:34.000000 pyscrlink-0.2.7/pyscrlink/scratch_link.py
-drwxr-xr-x   0 shin      (1000) shin      (1000)        0 2023-03-21 08:19:58.010416 pyscrlink-0.2.7/pyscrlink.egg-info/
--rw-r--r--   0 shin      (1000) shin      (1000)     7817 2023-03-21 08:19:58.000000 pyscrlink-0.2.7/pyscrlink.egg-info/PKG-INFO
--rw-r--r--   0 shin      (1000) shin      (1000)      348 2023-03-21 08:19:58.000000 pyscrlink-0.2.7/pyscrlink.egg-info/SOURCES.txt
--rw-r--r--   0 shin      (1000) shin      (1000)        1 2023-03-21 08:19:58.000000 pyscrlink-0.2.7/pyscrlink.egg-info/dependency_links.txt
--rw-r--r--   0 shin      (1000) shin      (1000)      116 2023-03-21 08:19:58.000000 pyscrlink-0.2.7/pyscrlink.egg-info/entry_points.txt
--rw-r--r--   0 shin      (1000) shin      (1000)       28 2023-03-21 08:19:58.000000 pyscrlink-0.2.7/pyscrlink.egg-info/requires.txt
--rw-r--r--   0 shin      (1000) shin      (1000)       10 2023-03-21 08:19:58.000000 pyscrlink-0.2.7/pyscrlink.egg-info/top_level.txt
--rw-r--r--   0 shin      (1000) shin      (1000)       38 2023-03-21 08:19:58.010416 pyscrlink-0.2.7/setup.cfg
--rw-r--r--   0 shin      (1000) shin      (1000)      955 2023-03-21 08:16:08.000000 pyscrlink-0.2.7/setup.py
+drwxr-xr-x   0 shin      (1000) shin      (1000)        0 2023-07-02 13:07:23.037766 pyscrlink-0.2.8/
+-rw-r--r--   0 shin      (1000) shin      (1000)     1528 2020-01-25 09:58:35.000000 pyscrlink-0.2.8/LICENSE
+-rw-r--r--   0 shin      (1000) shin      (1000)     7862 2023-07-02 13:07:23.037766 pyscrlink-0.2.8/PKG-INFO
+-rw-r--r--   0 shin      (1000) shin      (1000)     7415 2023-07-02 12:52:08.000000 pyscrlink-0.2.8/README.md
+drwxr-xr-x   0 shin      (1000) shin      (1000)        0 2023-07-02 13:07:23.037766 pyscrlink-0.2.8/pyscrlink/
+-rw-r--r--   0 shin      (1000) shin      (1000)        0 2021-10-10 06:37:32.000000 pyscrlink-0.2.8/pyscrlink/__init__.py
+-rw-r--r--   0 shin      (1000) shin      (1000)      108 2021-10-10 06:37:32.000000 pyscrlink-0.2.8/pyscrlink/__main__.py
+-rwxr-xr-x   0 shin      (1000) shin      (1000)     2276 2021-10-10 06:37:32.000000 pyscrlink-0.2.8/pyscrlink/bluepy_helper_cap.py
+-rwxr-xr-x   0 shin      (1000) shin      (1000)     6267 2023-03-21 06:55:40.000000 pyscrlink-0.2.8/pyscrlink/gencert.py
+-rwxr-xr-x   0 shin      (1000) shin      (1000)    23477 2023-07-02 12:52:08.000000 pyscrlink-0.2.8/pyscrlink/scratch_link.py
+drwxr-xr-x   0 shin      (1000) shin      (1000)        0 2023-07-02 13:07:23.037766 pyscrlink-0.2.8/pyscrlink.egg-info/
+-rw-r--r--   0 shin      (1000) shin      (1000)     7862 2023-07-02 13:07:23.000000 pyscrlink-0.2.8/pyscrlink.egg-info/PKG-INFO
+-rw-r--r--   0 shin      (1000) shin      (1000)      348 2023-07-02 13:07:23.000000 pyscrlink-0.2.8/pyscrlink.egg-info/SOURCES.txt
+-rw-r--r--   0 shin      (1000) shin      (1000)        1 2023-07-02 13:07:23.000000 pyscrlink-0.2.8/pyscrlink.egg-info/dependency_links.txt
+-rw-r--r--   0 shin      (1000) shin      (1000)      116 2023-07-02 13:07:23.000000 pyscrlink-0.2.8/pyscrlink.egg-info/entry_points.txt
+-rw-r--r--   0 shin      (1000) shin      (1000)       28 2023-07-02 13:07:23.000000 pyscrlink-0.2.8/pyscrlink.egg-info/requires.txt
+-rw-r--r--   0 shin      (1000) shin      (1000)       10 2023-07-02 13:07:23.000000 pyscrlink-0.2.8/pyscrlink.egg-info/top_level.txt
+-rw-r--r--   0 shin      (1000) shin      (1000)       38 2023-07-02 13:07:23.037766 pyscrlink-0.2.8/setup.cfg
+-rw-r--r--   0 shin      (1000) shin      (1000)      955 2023-07-02 12:52:08.000000 pyscrlink-0.2.8/setup.py
```

### Comparing `pyscrlink-0.2.7/LICENSE` & `pyscrlink-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pyscrlink-0.2.7/PKG-INFO` & `pyscrlink-0.2.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyscrlink
-Version: 0.2.7
+Version: 0.2.8
 Summary: Scratch-link for Linux with Python
 Home-page: https://github.com/kawasaki/pyscrlink
 Author: Shin'ichiro Kawasaki
 Author-email: kawasaki@juno.dti.ne.jp
 Classifier: Programming Language :: Python :: 3.6
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: POSIX :: Linux
@@ -180,14 +180,18 @@
 ---------------
 
 Please file issues to [GitHub issue tracker](https://github.com/kawasaki/pyscrlink/issues).
 
 Releases
 --------
 
+Release 0.2.8
+
+* Supported Microbit More v2
+
 Release 0.2.7
 
 * Supported Snap Firefox and Chromium
 * Added -r option to retry BLE scan
 
 Release 0.2.6
```

### Comparing `pyscrlink-0.2.7/README.md` & `pyscrlink-0.2.8/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -166,14 +166,18 @@
 ---------------
 
 Please file issues to [GitHub issue tracker](https://github.com/kawasaki/pyscrlink/issues).
 
 Releases
 --------
 
+Release 0.2.8
+
+* Supported Microbit More v2
+
 Release 0.2.7
 
 * Supported Snap Firefox and Chromium
 * Added -r option to retry BLE scan
 
 Release 0.2.6
```

### Comparing `pyscrlink-0.2.7/pyscrlink/bluepy_helper_cap.py` & `pyscrlink-0.2.8/pyscrlink/bluepy_helper_cap.py`

 * *Files identical despite different names*

### Comparing `pyscrlink-0.2.7/pyscrlink/gencert.py` & `pyscrlink-0.2.8/pyscrlink/gencert.py`

 * *Files identical despite different names*

### Comparing `pyscrlink-0.2.7/pyscrlink/scratch_link.py` & `pyscrlink-0.2.8/pyscrlink/scratch_link.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 import logging
 import sys
 import signal
 import traceback
 import argparse
 
 # for BLESession (e.g. BBC micro:bit)
-from bluepy.btle import Scanner, UUID, Peripheral, DefaultDelegate
+from bluepy.btle import Scanner, UUID, Peripheral, DefaultDelegate, ScanEntry
 from bluepy.btle import BTLEDisconnectError, BTLEManagementError
 from pyscrlink import bluepy_helper_cap
 
 import threading
 import time
 import queue
 
@@ -288,23 +288,27 @@
                     for u in dev_uuids:
                         logger.debug(f"dev UUID: {u} hash={u.__hash__()}")
                         logger.debug(given_uuid == u)
                         if given_uuid == u:
                             logger.debug("match...")
                             return True
             if 'namePrefix' in f:
-                # 0x08: Shortened Local Name
-                deviceName = dev.getValueText(0x08)
-                if not deviceName:
-                    continue
-                logger.debug(f"Name of \"{deviceName}\" begins with: \"{f['namePrefix']}\"?")
-                if(deviceName.startswith(f['namePrefix'])):
-                    logger.debug("Yes")
-                    return True
-                logger.debug("No")
+                logger.debug(f"given namePrefix: {f['namePrefix']}")
+                deviceName = dev.getValueText(ScanEntry.SHORT_LOCAL_NAME)
+                if deviceName:
+                    logger.debug(f"SHORT_LOCAL_NAME: {deviceName}")
+                    if deviceName.startswith(f['namePrefix']):
+                        logger.debug(f"match...")
+                        return True
+                deviceName = dev.getValueText(ScanEntry.COMPLETE_LOCAL_NAME)
+                if deviceName:
+                    logger.debug(f"COMPLETE_LOCAL_NAME: {deviceName}")
+                    if deviceName.startswith(f['namePrefix']):
+                        logger.debug(f"match...")
+                        return True
             if 'name' in f or 'manufactureData' in f:
                 logger.error("name/manufactureData filters not implemented")
                 # TODO: implement other filters defined:
                 # ref: https://github.com/LLK/scratch-link/blob/develop/Documentation/BluetoothLE.md
         return False
 
     def _scan_devices(self, params):
```

### Comparing `pyscrlink-0.2.7/pyscrlink.egg-info/PKG-INFO` & `pyscrlink-0.2.8/pyscrlink.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyscrlink
-Version: 0.2.7
+Version: 0.2.8
 Summary: Scratch-link for Linux with Python
 Home-page: https://github.com/kawasaki/pyscrlink
 Author: Shin'ichiro Kawasaki
 Author-email: kawasaki@juno.dti.ne.jp
 Classifier: Programming Language :: Python :: 3.6
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: POSIX :: Linux
@@ -180,14 +180,18 @@
 ---------------
 
 Please file issues to [GitHub issue tracker](https://github.com/kawasaki/pyscrlink/issues).
 
 Releases
 --------
 
+Release 0.2.8
+
+* Supported Microbit More v2
+
 Release 0.2.7
 
 * Supported Snap Firefox and Chromium
 * Added -r option to retry BLE scan
 
 Release 0.2.6
```

### Comparing `pyscrlink-0.2.7/setup.py` & `pyscrlink-0.2.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyscrlink",
-    version="0.2.7",
+    version="0.2.8",
     author="Shin'ichiro Kawasaki",
     author_email='kawasaki@juno.dti.ne.jp',
     description='Scratch-link for Linux with Python',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/kawasaki/pyscrlink",
     packages=setuptools.find_packages(),
```

