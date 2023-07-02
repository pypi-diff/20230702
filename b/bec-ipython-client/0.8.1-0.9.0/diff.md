# Comparing `tmp/bec_ipython_client-0.8.1.tar.gz` & `tmp/bec_ipython_client-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bec_ipython_client-0.8.1.tar", last modified: Sun Jul  2 18:15:06 2023, max compression
+gzip compressed data, was "bec_ipython_client-0.9.0.tar", last modified: Sun Jul  2 18:58:42 2023, max compression
```

## Comparing `bec_ipython_client-0.8.1.tar` & `bec_ipython_client-0.9.0.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 18:15:06.203279 bec_ipython_client-0.8.1/
--rw-r--r--   0 root         (0) root         (0)      458 2023-07-02 18:15:06.203279 bec_ipython_client-0.8.1/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 18:15:06.198279 bec_ipython_client-0.8.1/bec_client/
--rw-rw-rw-   0 root         (0) root         (0)       85 2023-06-19 08:14:59.000000 bec_ipython_client-0.8.1/bec_client/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1091 2023-06-19 08:14:59.000000 bec_ipython_client-0.8.1/bec_client/beamline_mixin.py
--rw-r--r--   0 root         (0) root         (0)     4664 2023-06-28 10:41:58.000000 bec_ipython_client-0.8.1/bec_client/bec_client.py
--rw-rw-rw-   0 root         (0) root         (0)     1972 2023-06-19 13:49:39.000000 bec_ipython_client-0.8.1/bec_client/bec_magics.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 18:15:06.201279 bec_ipython_client-0.8.1/bec_client/bin/
--rwxr-xr-x   0 root         (0) root         (0)      184 2023-07-02 18:14:52.000000 bec_ipython_client-0.8.1/bec_client/bin/bec
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 18:15:06.199279 bec_ipython_client-0.8.1/bec_client/callbacks/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-24 15:23:42.000000 bec_ipython_client-0.8.1/bec_client/callbacks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7462 2023-06-28 10:41:58.000000 bec_ipython_client-0.8.1/bec_client/callbacks/ipython_live_updates.py
--rw-r--r--   0 root         (0) root         (0)     9275 2023-06-28 15:23:35.000000 bec_ipython_client-0.8.1/bec_client/callbacks/live_table.py
--rw-r--r--   0 root         (0) root         (0)     4549 2023-06-28 10:41:58.000000 bec_ipython_client-0.8.1/bec_client/callbacks/move_device.py
--rw-r--r--   0 root         (0) root         (0)     3736 2023-06-28 10:41:58.000000 bec_ipython_client-0.8.1/bec_client/callbacks/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 18:15:06.199279 bec_ipython_client-0.8.1/bec_client/plugins/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 18:15:06.200279 bec_ipython_client-0.8.1/bec_client/plugins/LamNI/
--rw-rw-rw-   0 root         (0) root         (0)      149 2023-06-19 08:14:59.000000 bec_ipython_client-0.8.1/bec_client/plugins/LamNI/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5519 2023-06-19 13:49:39.000000 bec_ipython_client-0.8.1/bec_client/plugins/LamNI/lamni_optics_mixin.py
--rwxrwxrwx   0 root         (0) root         (0)      895 2023-04-24 15:23:42.000000 bec_ipython_client-0.8.1/bec_client/plugins/LamNI/load_additional_correction.py
--rw-r--r--   0 root         (0) root         (0)    54643 2023-06-28 10:41:58.000000 bec_ipython_client-0.8.1/bec_client/plugins/LamNI/x_ray_eye_align.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 18:15:06.200279 bec_ipython_client-0.8.1/bec_client/plugins/SLS/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-19 08:14:59.000000 bec_ipython_client-0.8.1/bec_client/plugins/SLS/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4926 2023-06-19 08:14:59.000000 bec_ipython_client-0.8.1/bec_client/plugins/SLS/sls_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 18:15:06.201279 bec_ipython_client-0.8.1/bec_client/plugins/XTreme/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-19 08:14:59.000000 bec_ipython_client-0.8.1/bec_client/plugins/XTreme/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3631 2023-06-19 08:14:59.000000 bec_ipython_client-0.8.1/bec_client/plugins/XTreme/x-treme.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-24 15:23:42.000000 bec_ipython_client-0.8.1/bec_client/plugins/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 18:15:06.201279 bec_ipython_client-0.8.1/bec_client/plugins/cSAXS/
--rw-rw-rw-   0 root         (0) root         (0)       79 2023-04-24 15:23:42.000000 bec_ipython_client-0.8.1/bec_client/plugins/cSAXS/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4433 2023-06-19 08:14:59.000000 bec_ipython_client-0.8.1/bec_client/plugins/cSAXS/beamline_info.py
--rw-rw-rw-   0 root         (0) root         (0)      445 2023-06-19 08:14:59.000000 bec_ipython_client-0.8.1/bec_client/plugins/cSAXS/cSAXS_beamline.py
--rw-rw-rw-   0 root         (0) root         (0)     2609 2023-04-24 15:23:42.000000 bec_ipython_client-0.8.1/bec_client/prettytable.py
--rw-rw-rw-   0 root         (0) root         (0)     8455 2023-04-24 15:23:42.000000 bec_ipython_client-0.8.1/bec_client/progressbar.py
--rw-r--r--   0 root         (0) root         (0)     4021 2023-06-28 10:41:58.000000 bec_ipython_client-0.8.1/bec_client/signals.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 18:15:06.203279 bec_ipython_client-0.8.1/bec_ipython_client.egg-info/
--rw-r--r--   0 root         (0) root         (0)      458 2023-07-02 18:15:06.000000 bec_ipython_client-0.8.1/bec_ipython_client.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1130 2023-07-02 18:15:06.000000 bec_ipython_client-0.8.1/bec_ipython_client.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-02 18:15:06.000000 bec_ipython_client-0.8.1/bec_ipython_client.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      113 2023-07-02 18:15:06.000000 bec_ipython_client-0.8.1/bec_ipython_client.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-07-02 18:15:06.000000 bec_ipython_client-0.8.1/bec_ipython_client.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      519 2023-07-02 18:15:06.203279 bec_ipython_client-0.8.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1026 2023-06-28 14:27:03.000000 bec_ipython_client-0.8.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 18:58:42.227246 bec_ipython_client-0.9.0/
+-rw-r--r--   0 root         (0) root         (0)      458 2023-07-02 18:58:42.227246 bec_ipython_client-0.9.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 18:58:42.224246 bec_ipython_client-0.9.0/bec_client/
+-rw-rw-rw-   0 root         (0) root         (0)       85 2023-06-19 08:14:59.000000 bec_ipython_client-0.9.0/bec_client/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1091 2023-06-19 08:14:59.000000 bec_ipython_client-0.9.0/bec_client/beamline_mixin.py
+-rw-r--r--   0 root         (0) root         (0)     4664 2023-06-28 10:41:58.000000 bec_ipython_client-0.9.0/bec_client/bec_client.py
+-rw-rw-rw-   0 root         (0) root         (0)     1972 2023-06-19 13:49:39.000000 bec_ipython_client-0.9.0/bec_client/bec_magics.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 18:58:42.226246 bec_ipython_client-0.9.0/bec_client/bin/
+-rwxr-xr-x   0 root         (0) root         (0)      184 2023-07-02 18:14:52.000000 bec_ipython_client-0.9.0/bec_client/bin/bec
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 18:58:42.225246 bec_ipython_client-0.9.0/bec_client/callbacks/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-24 15:23:42.000000 bec_ipython_client-0.9.0/bec_client/callbacks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7462 2023-06-28 10:41:58.000000 bec_ipython_client-0.9.0/bec_client/callbacks/ipython_live_updates.py
+-rw-r--r--   0 root         (0) root         (0)     9275 2023-06-28 15:23:35.000000 bec_ipython_client-0.9.0/bec_client/callbacks/live_table.py
+-rw-r--r--   0 root         (0) root         (0)     4549 2023-06-28 10:41:58.000000 bec_ipython_client-0.9.0/bec_client/callbacks/move_device.py
+-rw-r--r--   0 root         (0) root         (0)     3736 2023-06-28 10:41:58.000000 bec_ipython_client-0.9.0/bec_client/callbacks/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 18:58:42.225246 bec_ipython_client-0.9.0/bec_client/plugins/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 18:58:42.225246 bec_ipython_client-0.9.0/bec_client/plugins/LamNI/
+-rw-rw-rw-   0 root         (0) root         (0)      149 2023-06-19 08:14:59.000000 bec_ipython_client-0.9.0/bec_client/plugins/LamNI/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5519 2023-06-19 13:49:39.000000 bec_ipython_client-0.9.0/bec_client/plugins/LamNI/lamni_optics_mixin.py
+-rwxrwxrwx   0 root         (0) root         (0)      895 2023-04-24 15:23:42.000000 bec_ipython_client-0.9.0/bec_client/plugins/LamNI/load_additional_correction.py
+-rw-r--r--   0 root         (0) root         (0)    54643 2023-06-28 10:41:58.000000 bec_ipython_client-0.9.0/bec_client/plugins/LamNI/x_ray_eye_align.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 18:58:42.226246 bec_ipython_client-0.9.0/bec_client/plugins/SLS/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-19 08:14:59.000000 bec_ipython_client-0.9.0/bec_client/plugins/SLS/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4926 2023-06-19 08:14:59.000000 bec_ipython_client-0.9.0/bec_client/plugins/SLS/sls_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 18:58:42.226246 bec_ipython_client-0.9.0/bec_client/plugins/XTreme/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-19 08:14:59.000000 bec_ipython_client-0.9.0/bec_client/plugins/XTreme/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3631 2023-06-19 08:14:59.000000 bec_ipython_client-0.9.0/bec_client/plugins/XTreme/x-treme.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-24 15:23:42.000000 bec_ipython_client-0.9.0/bec_client/plugins/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 18:58:42.226246 bec_ipython_client-0.9.0/bec_client/plugins/cSAXS/
+-rw-rw-rw-   0 root         (0) root         (0)       79 2023-04-24 15:23:42.000000 bec_ipython_client-0.9.0/bec_client/plugins/cSAXS/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4433 2023-06-19 08:14:59.000000 bec_ipython_client-0.9.0/bec_client/plugins/cSAXS/beamline_info.py
+-rw-rw-rw-   0 root         (0) root         (0)      445 2023-06-19 08:14:59.000000 bec_ipython_client-0.9.0/bec_client/plugins/cSAXS/cSAXS_beamline.py
+-rw-rw-rw-   0 root         (0) root         (0)     2609 2023-04-24 15:23:42.000000 bec_ipython_client-0.9.0/bec_client/prettytable.py
+-rw-rw-rw-   0 root         (0) root         (0)     8455 2023-04-24 15:23:42.000000 bec_ipython_client-0.9.0/bec_client/progressbar.py
+-rw-r--r--   0 root         (0) root         (0)     4021 2023-06-28 10:41:58.000000 bec_ipython_client-0.9.0/bec_client/signals.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 18:58:42.227246 bec_ipython_client-0.9.0/bec_ipython_client.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      458 2023-07-02 18:58:42.000000 bec_ipython_client-0.9.0/bec_ipython_client.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1130 2023-07-02 18:58:42.000000 bec_ipython_client-0.9.0/bec_ipython_client.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-02 18:58:42.000000 bec_ipython_client-0.9.0/bec_ipython_client.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      113 2023-07-02 18:58:42.000000 bec_ipython_client-0.9.0/bec_ipython_client.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-07-02 18:58:42.000000 bec_ipython_client-0.9.0/bec_ipython_client.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      519 2023-07-02 18:58:42.228246 bec_ipython_client-0.9.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1026 2023-06-28 14:27:03.000000 bec_ipython_client-0.9.0/setup.py
```

### Comparing `bec_ipython_client-0.8.1/bec_client/beamline_mixin.py` & `bec_ipython_client-0.9.0/bec_client/beamline_mixin.py`

 * *Files identical despite different names*

### Comparing `bec_ipython_client-0.8.1/bec_client/bec_client.py` & `bec_ipython_client-0.9.0/bec_client/bec_client.py`

 * *Files identical despite different names*

### Comparing `bec_ipython_client-0.8.1/bec_client/bec_magics.py` & `bec_ipython_client-0.9.0/bec_client/bec_magics.py`

 * *Files identical despite different names*

### Comparing `bec_ipython_client-0.8.1/bec_client/callbacks/ipython_live_updates.py` & `bec_ipython_client-0.9.0/bec_client/callbacks/ipython_live_updates.py`

 * *Files identical despite different names*

### Comparing `bec_ipython_client-0.8.1/bec_client/callbacks/live_table.py` & `bec_ipython_client-0.9.0/bec_client/callbacks/live_table.py`

 * *Files identical despite different names*

### Comparing `bec_ipython_client-0.8.1/bec_client/callbacks/move_device.py` & `bec_ipython_client-0.9.0/bec_client/callbacks/move_device.py`

 * *Files identical despite different names*

### Comparing `bec_ipython_client-0.8.1/bec_client/callbacks/utils.py` & `bec_ipython_client-0.9.0/bec_client/callbacks/utils.py`

 * *Files identical despite different names*

### Comparing `bec_ipython_client-0.8.1/bec_client/plugins/LamNI/lamni_optics_mixin.py` & `bec_ipython_client-0.9.0/bec_client/plugins/LamNI/lamni_optics_mixin.py`

 * *Files identical despite different names*

### Comparing `bec_ipython_client-0.8.1/bec_client/plugins/LamNI/load_additional_correction.py` & `bec_ipython_client-0.9.0/bec_client/plugins/LamNI/load_additional_correction.py`

 * *Files identical despite different names*

### Comparing `bec_ipython_client-0.8.1/bec_client/plugins/LamNI/x_ray_eye_align.py` & `bec_ipython_client-0.9.0/bec_client/plugins/LamNI/x_ray_eye_align.py`

 * *Files identical despite different names*

### Comparing `bec_ipython_client-0.8.1/bec_client/plugins/SLS/sls_info.py` & `bec_ipython_client-0.9.0/bec_client/plugins/SLS/sls_info.py`

 * *Files identical despite different names*

### Comparing `bec_ipython_client-0.8.1/bec_client/plugins/XTreme/x-treme.py` & `bec_ipython_client-0.9.0/bec_client/plugins/XTreme/x-treme.py`

 * *Files identical despite different names*

### Comparing `bec_ipython_client-0.8.1/bec_client/plugins/cSAXS/beamline_info.py` & `bec_ipython_client-0.9.0/bec_client/plugins/cSAXS/beamline_info.py`

 * *Files identical despite different names*

### Comparing `bec_ipython_client-0.8.1/bec_client/prettytable.py` & `bec_ipython_client-0.9.0/bec_client/prettytable.py`

 * *Files identical despite different names*

### Comparing `bec_ipython_client-0.8.1/bec_client/progressbar.py` & `bec_ipython_client-0.9.0/bec_client/progressbar.py`

 * *Files identical despite different names*

### Comparing `bec_ipython_client-0.8.1/bec_client/signals.py` & `bec_ipython_client-0.9.0/bec_client/signals.py`

 * *Files identical despite different names*

### Comparing `bec_ipython_client-0.8.1/bec_ipython_client.egg-info/SOURCES.txt` & `bec_ipython_client-0.9.0/bec_ipython_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bec_ipython_client-0.8.1/setup.cfg` & `bec_ipython_client-0.9.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `bec_ipython_client-0.8.1/setup.py` & `bec_ipython_client-0.9.0/setup.py`

 * *Files identical despite different names*

