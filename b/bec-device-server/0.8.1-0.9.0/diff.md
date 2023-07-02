# Comparing `tmp/bec_device_server-0.8.1.tar.gz` & `tmp/bec_device_server-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bec_device_server-0.8.1.tar", last modified: Sun Jul  2 18:15:23 2023, max compression
+gzip compressed data, was "bec_device_server-0.9.0.tar", last modified: Sun Jul  2 18:58:57 2023, max compression
```

## Comparing `bec_device_server-0.8.1.tar` & `bec_device_server-0.9.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 18:15:23.287762 bec_device_server-0.8.1/
--rw-r--r--   0 root         (0) root         (0)      495 2023-07-02 18:15:23.287762 bec_device_server-0.8.1/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 18:15:23.286763 bec_device_server-0.8.1/bec_device_server.egg-info/
--rw-r--r--   0 root         (0) root         (0)      495 2023-07-02 18:15:23.000000 bec_device_server-0.8.1/bec_device_server.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      454 2023-07-02 18:15:23.000000 bec_device_server-0.8.1/bec_device_server.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-02 18:15:23.000000 bec_device_server-0.8.1/bec_device_server.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       27 2023-07-02 18:15:23.000000 bec_device_server-0.8.1/bec_device_server.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-07-02 18:15:23.000000 bec_device_server-0.8.1/bec_device_server.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 18:15:23.285762 bec_device_server-0.8.1/device_server/
--rw-r--r--   0 root         (0) root         (0)      161 2023-06-28 10:41:58.000000 bec_device_server-0.8.1/device_server/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18508 2023-06-28 10:41:58.000000 bec_device_server-0.8.1/device_server/device_server.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 18:15:23.286763 bec_device_server-0.8.1/device_server/devices/
--rw-r--r--   0 root         (0) root         (0)      159 2023-06-28 10:41:58.000000 bec_device_server-0.8.1/device_server/devices/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3473 2023-06-28 10:41:58.000000 bec_device_server-0.8.1/device_server/devices/config_update_handler.py
--rw-r--r--   0 root         (0) root         (0)     3096 2023-06-28 10:41:58.000000 bec_device_server-0.8.1/device_server/devices/device_serializer.py
--rw-r--r--   0 root         (0) root         (0)    13006 2023-06-28 10:41:58.000000 bec_device_server-0.8.1/device_server/devices/devicemanager.py
--rw-r--r--   0 root         (0) root         (0)      576 2023-07-02 18:15:23.287762 bec_device_server-0.8.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      857 2023-06-28 14:27:03.000000 bec_device_server-0.8.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 18:58:57.700787 bec_device_server-0.9.0/
+-rw-r--r--   0 root         (0) root         (0)      495 2023-07-02 18:58:57.701787 bec_device_server-0.9.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 18:58:57.700787 bec_device_server-0.9.0/bec_device_server.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      495 2023-07-02 18:58:57.000000 bec_device_server-0.9.0/bec_device_server.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      454 2023-07-02 18:58:57.000000 bec_device_server-0.9.0/bec_device_server.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-02 18:58:57.000000 bec_device_server-0.9.0/bec_device_server.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       27 2023-07-02 18:58:57.000000 bec_device_server-0.9.0/bec_device_server.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-07-02 18:58:57.000000 bec_device_server-0.9.0/bec_device_server.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 18:58:57.699787 bec_device_server-0.9.0/device_server/
+-rw-r--r--   0 root         (0) root         (0)      161 2023-06-28 10:41:58.000000 bec_device_server-0.9.0/device_server/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18508 2023-06-28 10:41:58.000000 bec_device_server-0.9.0/device_server/device_server.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 18:58:57.700787 bec_device_server-0.9.0/device_server/devices/
+-rw-r--r--   0 root         (0) root         (0)      159 2023-06-28 10:41:58.000000 bec_device_server-0.9.0/device_server/devices/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3473 2023-06-28 10:41:58.000000 bec_device_server-0.9.0/device_server/devices/config_update_handler.py
+-rw-r--r--   0 root         (0) root         (0)     3096 2023-06-28 10:41:58.000000 bec_device_server-0.9.0/device_server/devices/device_serializer.py
+-rw-r--r--   0 root         (0) root         (0)    13006 2023-06-28 10:41:58.000000 bec_device_server-0.9.0/device_server/devices/devicemanager.py
+-rw-r--r--   0 root         (0) root         (0)      576 2023-07-02 18:58:57.701787 bec_device_server-0.9.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      857 2023-06-28 14:27:03.000000 bec_device_server-0.9.0/setup.py
```

### Comparing `bec_device_server-0.8.1/device_server/device_server.py` & `bec_device_server-0.9.0/device_server/device_server.py`

 * *Files identical despite different names*

### Comparing `bec_device_server-0.8.1/device_server/devices/config_update_handler.py` & `bec_device_server-0.9.0/device_server/devices/config_update_handler.py`

 * *Files identical despite different names*

### Comparing `bec_device_server-0.8.1/device_server/devices/device_serializer.py` & `bec_device_server-0.9.0/device_server/devices/device_serializer.py`

 * *Files identical despite different names*

### Comparing `bec_device_server-0.8.1/device_server/devices/devicemanager.py` & `bec_device_server-0.9.0/device_server/devices/devicemanager.py`

 * *Files identical despite different names*

### Comparing `bec_device_server-0.8.1/setup.cfg` & `bec_device_server-0.9.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `bec_device_server-0.8.1/setup.py` & `bec_device_server-0.9.0/setup.py`

 * *Files identical despite different names*

