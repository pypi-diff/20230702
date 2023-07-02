# Comparing `tmp/WPP_Whatsapp-0.0.1.tar.gz` & `tmp/WPP_Whatsapp-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "WPP_Whatsapp-0.0.1.tar", last modified: Tue Jun 27 12:45:48 2023, max compression
+gzip compressed data, was "WPP_Whatsapp-0.1.0.tar", last modified: Sun Jul  2 14:52:47 2023, max compression
```

## Comparing `WPP_Whatsapp-0.0.1.tar` & `WPP_Whatsapp-0.1.0.tar`

### file list

```diff
@@ -1,43 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:45:48.458962 WPP_Whatsapp-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11745 2023-06-27 12:45:48.458962 WPP_Whatsapp-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10842 2023-06-27 12:45:35.000000 WPP_Whatsapp-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:45:48.454961 WPP_Whatsapp-0.0.1/WPP_Whatsapp/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:45:48.454961 WPP_Whatsapp-0.0.1/WPP_Whatsapp/WPP_Whatsapp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11745 2023-06-27 12:45:48.000000 WPP_Whatsapp-0.0.1/WPP_Whatsapp/WPP_Whatsapp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-06-27 12:45:48.000000 WPP_Whatsapp-0.0.1/WPP_Whatsapp/WPP_Whatsapp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 12:45:48.000000 WPP_Whatsapp-0.0.1/WPP_Whatsapp/WPP_Whatsapp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-27 12:45:48.000000 WPP_Whatsapp-0.0.1/WPP_Whatsapp/WPP_Whatsapp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-27 12:45:48.000000 WPP_Whatsapp-0.0.1/WPP_Whatsapp/WPP_Whatsapp.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:45:48.454961 WPP_Whatsapp-0.0.1/WPP_Whatsapp/api/
--rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-06-27 12:45:35.000000 WPP_Whatsapp-0.0.1/WPP_Whatsapp/api/Whatsapp.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 12:45:35.000000 WPP_Whatsapp-0.0.1/WPP_Whatsapp/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-06-27 12:45:35.000000 WPP_Whatsapp-0.0.1/WPP_Whatsapp/api/const.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:45:48.454961 WPP_Whatsapp-0.0.1/WPP_Whatsapp/api/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 12:45:35.000000 WPP_Whatsapp-0.0.1/WPP_Whatsapp/api/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-06-27 12:45:35.000000 WPP_Whatsapp-0.0.1/WPP_Whatsapp/api/helpers/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-06-27 12:45:35.000000 WPP_Whatsapp-0.0.1/WPP_Whatsapp/api/helpers/jsFunction.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 12:45:35.000000 WPP_Whatsapp-0.0.1/WPP_Whatsapp/api/helpers/scrap-img.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:45:48.458962 WPP_Whatsapp-0.0.1/WPP_Whatsapp/api/layers/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-27 12:45:35.000000 WPP_Whatsapp-0.0.1/WPP_Whatsapp/api/layers/BusinessLayer.py
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-27 12:45:35.000000 WPP_Whatsapp-0.0.1/WPP_Whatsapp/api/layers/CatalogLayer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-06-27 12:45:35.000000 WPP_Whatsapp-0.0.1/WPP_Whatsapp/api/layers/ControlsLayer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-06-27 12:45:35.000000 WPP_Whatsapp-0.0.1/WPP_Whatsapp/api/layers/GroupLayer.py
--rw-r--r--   0 runner    (1001) docker     (123)    20345 2023-06-27 12:45:35.000000 WPP_Whatsapp-0.0.1/WPP_Whatsapp/api/layers/HostLayer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-06-27 12:45:35.000000 WPP_Whatsapp-0.0.1/WPP_Whatsapp/api/layers/LabelsLayer.py
--rw-r--r--   0 runner    (1001) docker     (123)    12139 2023-06-27 12:45:35.000000 WPP_Whatsapp-0.0.1/WPP_Whatsapp/api/layers/ListenerLayer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-06-27 12:45:35.000000 WPP_Whatsapp-0.0.1/WPP_Whatsapp/api/layers/ProfileLayer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7728 2023-06-27 12:45:35.000000 WPP_Whatsapp-0.0.1/WPP_Whatsapp/api/layers/RetrieverLayer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11870 2023-06-27 12:45:35.000000 WPP_Whatsapp-0.0.1/WPP_Whatsapp/api/layers/SenderLayer.py
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-27 12:45:35.000000 WPP_Whatsapp-0.0.1/WPP_Whatsapp/api/layers/StatusLayer.py
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-06-27 12:45:35.000000 WPP_Whatsapp-0.0.1/WPP_Whatsapp/api/layers/UILayer.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 12:45:35.000000 WPP_Whatsapp-0.0.1/WPP_Whatsapp/api/layers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:45:48.458962 WPP_Whatsapp-0.0.1/WPP_Whatsapp/api/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 12:45:35.000000 WPP_Whatsapp-0.0.1/WPP_Whatsapp/api/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-06-27 12:45:35.000000 WPP_Whatsapp-0.0.1/WPP_Whatsapp/api/model/status_find.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 12:45:48.458962 WPP_Whatsapp-0.0.1/WPP_Whatsapp/controllers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 12:45:35.000000 WPP_Whatsapp-0.0.1/WPP_Whatsapp/controllers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 12:45:35.000000 WPP_Whatsapp-0.0.1/WPP_Whatsapp/controllers/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-06-27 12:45:35.000000 WPP_Whatsapp-0.0.1/WPP_Whatsapp/controllers/browser.py
--rw-r--r--   0 runner    (1001) docker     (123)     7532 2023-06-27 12:45:35.000000 WPP_Whatsapp-0.0.1/WPP_Whatsapp/controllers/initializer.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 12:45:48.458962 WPP_Whatsapp-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-06-27 12:45:35.000000 WPP_Whatsapp-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 14:52:47.632437 WPP_Whatsapp-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-07-02 14:52:47.632437 WPP_Whatsapp-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3977 2023-07-02 14:52:37.000000 WPP_Whatsapp-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 14:52:47.620437 WPP_Whatsapp-0.1.0/WPP_Whatsapp/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 14:52:47.620437 WPP_Whatsapp-0.1.0/WPP_Whatsapp/PlaywrightSafeThread/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-02 14:52:37.000000 WPP_Whatsapp-0.1.0/WPP_Whatsapp/PlaywrightSafeThread/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 14:52:47.620437 WPP_Whatsapp-0.1.0/WPP_Whatsapp/PlaywrightSafeThread/browser/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 14:52:37.000000 WPP_Whatsapp-0.1.0/WPP_Whatsapp/PlaywrightSafeThread/browser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-07-02 14:52:37.000000 WPP_Whatsapp-0.1.0/WPP_Whatsapp/PlaywrightSafeThread/browser/plawright_shim.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21892 2023-07-02 14:52:37.000000 WPP_Whatsapp-0.1.0/WPP_Whatsapp/PlaywrightSafeThread/browser/threadsafe_browser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 14:52:47.624436 WPP_Whatsapp-0.1.0/WPP_Whatsapp/WPP_Whatsapp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-07-02 14:52:47.000000 WPP_Whatsapp-0.1.0/WPP_Whatsapp/WPP_Whatsapp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-07-02 14:52:47.000000 WPP_Whatsapp-0.1.0/WPP_Whatsapp/WPP_Whatsapp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 14:52:47.000000 WPP_Whatsapp-0.1.0/WPP_Whatsapp/WPP_Whatsapp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-02 14:52:47.000000 WPP_Whatsapp-0.1.0/WPP_Whatsapp/WPP_Whatsapp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-02 14:52:47.000000 WPP_Whatsapp-0.1.0/WPP_Whatsapp/WPP_Whatsapp.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 14:52:47.624436 WPP_Whatsapp-0.1.0/WPP_Whatsapp/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-07-02 14:52:37.000000 WPP_Whatsapp-0.1.0/WPP_Whatsapp/api/Whatsapp.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 14:52:37.000000 WPP_Whatsapp-0.1.0/WPP_Whatsapp/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-07-02 14:52:37.000000 WPP_Whatsapp-0.1.0/WPP_Whatsapp/api/const.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 14:52:47.624436 WPP_Whatsapp-0.1.0/WPP_Whatsapp/api/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 14:52:37.000000 WPP_Whatsapp-0.1.0/WPP_Whatsapp/api/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-02 14:52:37.000000 WPP_Whatsapp-0.1.0/WPP_Whatsapp/api/helpers/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-02 14:52:37.000000 WPP_Whatsapp-0.1.0/WPP_Whatsapp/api/helpers/function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-07-02 14:52:37.000000 WPP_Whatsapp-0.1.0/WPP_Whatsapp/api/helpers/jsFunction.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 14:52:37.000000 WPP_Whatsapp-0.1.0/WPP_Whatsapp/api/helpers/scrap-img.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 14:52:47.628436 WPP_Whatsapp-0.1.0/WPP_Whatsapp/api/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-02 14:52:37.000000 WPP_Whatsapp-0.1.0/WPP_Whatsapp/api/layers/BusinessLayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-02 14:52:37.000000 WPP_Whatsapp-0.1.0/WPP_Whatsapp/api/layers/CatalogLayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-07-02 14:52:37.000000 WPP_Whatsapp-0.1.0/WPP_Whatsapp/api/layers/ControlsLayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3595 2023-07-02 14:52:37.000000 WPP_Whatsapp-0.1.0/WPP_Whatsapp/api/layers/GroupLayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20753 2023-07-02 14:52:37.000000 WPP_Whatsapp-0.1.0/WPP_Whatsapp/api/layers/HostLayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-07-02 14:52:37.000000 WPP_Whatsapp-0.1.0/WPP_Whatsapp/api/layers/LabelsLayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12209 2023-07-02 14:52:37.000000 WPP_Whatsapp-0.1.0/WPP_Whatsapp/api/layers/ListenerLayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-07-02 14:52:37.000000 WPP_Whatsapp-0.1.0/WPP_Whatsapp/api/layers/ProfileLayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8031 2023-07-02 14:52:37.000000 WPP_Whatsapp-0.1.0/WPP_Whatsapp/api/layers/RetrieverLayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11216 2023-07-02 14:52:37.000000 WPP_Whatsapp-0.1.0/WPP_Whatsapp/api/layers/SenderLayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-02 14:52:37.000000 WPP_Whatsapp-0.1.0/WPP_Whatsapp/api/layers/StatusLayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-07-02 14:52:37.000000 WPP_Whatsapp-0.1.0/WPP_Whatsapp/api/layers/UILayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 14:52:37.000000 WPP_Whatsapp-0.1.0/WPP_Whatsapp/api/layers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 14:52:47.628436 WPP_Whatsapp-0.1.0/WPP_Whatsapp/api/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 14:52:37.000000 WPP_Whatsapp-0.1.0/WPP_Whatsapp/api/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-07-02 14:52:37.000000 WPP_Whatsapp-0.1.0/WPP_Whatsapp/api/model/status_find.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 14:52:47.628436 WPP_Whatsapp-0.1.0/WPP_Whatsapp/controllers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 14:52:37.000000 WPP_Whatsapp-0.1.0/WPP_Whatsapp/controllers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 14:52:37.000000 WPP_Whatsapp-0.1.0/WPP_Whatsapp/controllers/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-07-02 14:52:37.000000 WPP_Whatsapp-0.1.0/WPP_Whatsapp/controllers/browser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6160 2023-07-02 14:52:37.000000 WPP_Whatsapp-0.1.0/WPP_Whatsapp/controllers/initializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 14:52:47.632437 WPP_Whatsapp-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-07-02 14:52:37.000000 WPP_Whatsapp-0.1.0/setup.py
```

### Comparing `WPP_Whatsapp-0.0.1/WPP_Whatsapp/WPP_Whatsapp.egg-info/SOURCES.txt` & `WPP_Whatsapp-0.1.0/WPP_Whatsapp/WPP_Whatsapp.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 README.md
 setup.py
+WPP_Whatsapp/PlaywrightSafeThread/__init__.py
+WPP_Whatsapp/PlaywrightSafeThread/browser/__init__.py
+WPP_Whatsapp/PlaywrightSafeThread/browser/plawright_shim.py
+WPP_Whatsapp/PlaywrightSafeThread/browser/threadsafe_browser.py
 WPP_Whatsapp/WPP_Whatsapp.egg-info/PKG-INFO
 WPP_Whatsapp/WPP_Whatsapp.egg-info/SOURCES.txt
 WPP_Whatsapp/WPP_Whatsapp.egg-info/dependency_links.txt
 WPP_Whatsapp/WPP_Whatsapp.egg-info/requires.txt
 WPP_Whatsapp/WPP_Whatsapp.egg-info/top_level.txt
 WPP_Whatsapp/api/Whatsapp.py
 WPP_Whatsapp/api/__init__.py
 WPP_Whatsapp/api/const.py
 WPP_Whatsapp/api/helpers/__init__.py
 WPP_Whatsapp/api/helpers/decorators.py
+WPP_Whatsapp/api/helpers/function.py
 WPP_Whatsapp/api/helpers/jsFunction.py
 WPP_Whatsapp/api/helpers/scrap-img.py
 WPP_Whatsapp/api/layers/BusinessLayer.py
 WPP_Whatsapp/api/layers/CatalogLayer.py
 WPP_Whatsapp/api/layers/ControlsLayer.py
 WPP_Whatsapp/api/layers/GroupLayer.py
 WPP_Whatsapp/api/layers/HostLayer.py
```

### Comparing `WPP_Whatsapp-0.0.1/WPP_Whatsapp/api/Whatsapp.py` & `WPP_Whatsapp-0.1.0/WPP_Whatsapp/api/Whatsapp.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,50 +1,58 @@
 import asyncio
+import inspect
 
+from api.layers.HostLayer import HostLayer
 from WPP_Whatsapp.api.const import defaultOptions, Logger
 from WPP_Whatsapp.api.layers.BusinessLayer import BusinessLayer
+from api.layers.ListenerLayer import ListenerLayer
 
 
 class Whatsapp(BusinessLayer):
     connected = None
 
-    def __init__(self, session, browser, *args, **kwargs):
+    def __init__(self, session, threadsafe_browser, *args, **kwargs):
         self.session = session
-        self.page = browser.page
-        self.browser = browser.browser
-        self.Browser = browser
-        self.loop = kwargs.get("loop")  # or asyncio.new_event_loop()
-        if not self.loop:
-            raise Exception("Not Add Loop")
-        asyncio.set_event_loop(self.loop)
+        self.page = threadsafe_browser.page
+        self.browser = threadsafe_browser.browser
+        self.ThreadsafeBrowser = threadsafe_browser
+        # self.loop = kwargs.get("loop")  # or asyncio.new_event_loop()
+        # if not self.loop:
+        #     raise Exception("Not Add Loop")
+        # asyncio.set_event_loop(self.loop)
         self.session = session
         self.options.update(defaultOptions)
         self.logger = self.options.get("logger") or Logger
         self.logger.info(f'{self.session}: Initializing...')
         self.logQR = kwargs.get("logQR") or False
         self.autoClose = kwargs.get("autoClose") or self.options.get("autoClose") or 0
-        super().__init__()
+        HostLayer.__init__(self)
+        ListenerLayer.__init__(self)
         self.handel()
 
     def handel(self):
         self.interval = None
         if self.page:
             self.page.on('close', lambda: self.clearInterval(self.interval))
 
-        # self.interval = self.__setInterval(self.__intervalHandel, 60)
+        self.interval = self.__setInterval(self.__intervalHandel, 60)
 
     @staticmethod
     def __setInterval(func, interval, *args, **kwargs):
         loop = kwargs.get('loop') or asyncio.get_event_loop()
         stopped = asyncio.Event()
 
         async def loop_():
             while not stopped.is_set():
-                func()
-                # asyncio.sleep(interval)
+                if inspect.iscoroutinefunction(func):
+                    await func()
+                    await asyncio.sleep(interval)
+                else:
+                    func()
+                    await asyncio.sleep(interval)
 
         loop.create_task(loop_())
         return stopped
 
     async def __intervalHandel(self):
         newConnected = self.page_evaluate("() => WPP && WPP.conn.isRegistered()")
 
@@ -56,34 +64,34 @@
             self.logger.info(f'{self.session}: Session Unpaired')
             # asyncio.sleep(1)
             self.statusFind('desconnectedMobile', self.session)
 
     async def afterPageScriptInjected(self):
         await self._afterPageScriptInjectedHost()
         await self._afterPageScriptInjectedListener()
-        is_authenticated = await self.page_evaluate("() => WPP.conn.isRegistered()")
+        is_authenticated = await self.ThreadsafeBrowser.page_evaluate("() => WPP.conn.isRegistered()")
         self.connected = is_authenticated
 
-    async def useHere(self):
-        return await self.page_evaluate("() => WAPI.takeOver()")
+    def useHere(self):
+        return self.ThreadsafeBrowser.page_evaluate("() => WAPI.takeOver()")
 
     async def logout(self):
-        return await self.page_evaluate("() => WPP.conn.logout()")
+        return self.ThreadsafeBrowser.page_evaluate("() => WPP.conn.logout()")
 
     async def getMessageById(self, messageId):
-        return await self.page_evaluate("(messageId) => WAPI.getMessageById(messageId)", messageId)
+        return self.ThreadsafeBrowser.page_evaluate("(messageId) => WAPI.getMessageById(messageId)", messageId)
 
     async def getMessages(self, chatId, params=None):
         """
         :param chatId:
         :param params: (count, id, direction)
         :return:
         """
         if not params:
             params = {}
         chatId = self.valid_chatId(chatId)
-        return await self.page_evaluate("({ chatId, params }) => WAPI.getMessages(chatId, params)",
-                                        {"chatId": chatId, "params": params})
+        return self.ThreadsafeBrowser.page_evaluate("({ chatId, params }) => WAPI.getMessages(chatId, params)",
+                                                    {"chatId": chatId, "params": params})
 
     async def rejectCall(self, callId):
-        return await self.page_evaluate(
+        return self.ThreadsafeBrowser.page_evaluate(
             "({callId}) => WPP.call.rejectCall(callId)", callId)
```

### Comparing `WPP_Whatsapp-0.0.1/WPP_Whatsapp/api/const.py` & `WPP_Whatsapp-0.1.0/WPP_Whatsapp/api/const.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,17 +37,17 @@
     '--disable-app-list-dismiss-on-blur',
     '--disable-accelerated-video-decode',
     '--disable-dev-shm-usage',
 ]
 
 
 def defaultLogger():
-    logging.basicConfig(level=logging.DEBUG, format='%(asctime)s - %(levelname)s - %(message)s',
+    logging.basicConfig(level=logging.ERROR, format='%(asctime)s - %(levelname)s - %(message)s',
                         datefmt='%d-%b-%y %H:%M:%S')
-    logger = logging.getLogger()
+    logger = logging.getLogger(name="WPP_Whatsapp")
     return logger
 
 
 Logger = defaultLogger()
 
 defaultOptions = {
     "folderNameToken": r"E:\Projects\Python\_Libs_\tokens",
```

### Comparing `WPP_Whatsapp-0.0.1/WPP_Whatsapp/api/helpers/decorators.py` & `WPP_Whatsapp-0.1.0/WPP_Whatsapp/api/helpers/decorators.py`

 * *Files identical despite different names*

### Comparing `WPP_Whatsapp-0.0.1/WPP_Whatsapp/api/helpers/jsFunction.py` & `WPP_Whatsapp-0.1.0/WPP_Whatsapp/api/helpers/jsFunction.py`

 * *Files identical despite different names*

### Comparing `WPP_Whatsapp-0.0.1/WPP_Whatsapp/api/layers/ControlsLayer.py` & `WPP_Whatsapp-0.1.0/WPP_Whatsapp/api/layers/ControlsLayer.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 from WPP_Whatsapp.api.layers.UILayer import UILayer
 
 
 class ControlsLayer(UILayer):
 
-    async def unblockContact(self, contactId):
+    def unblockContact(self, contactId):
         contactId = self.valid_chatId(contactId)
-        await self.page_evaluate("(contactId) => WPP.blocklist.unblockContact(contactId)", contactId)
+        self.ThreadsafeBrowser.sync_page_evaluate("(contactId) => WPP.blocklist.unblockContact(contactId)", contactId)
         return True
 
-    async def blockContact(self, contactId):
+    def blockContact(self, contactId):
         contactId = self.valid_chatId(contactId)
-        await self.page_evaluate("(contactId) => WPP.blocklist.blockContact(contactId)", contactId)
+        self.ThreadsafeBrowser.sync_page_evaluate("(contactId) => WPP.blocklist.blockContact(contactId)", contactId)
         return True
 
-    async def markUnseenMessage(self, contactId):
+    def markUnseenMessage(self, contactId):
         contactId = self.valid_chatId(contactId)
-        await self.page_evaluate("(contactId) => WPP.chat.markIsUnread(contactId)", contactId)
+        self.ThreadsafeBrowser.sync_page_evaluate("(contactId) => WPP.chat.markIsUnread(contactId)", contactId)
 
-    async def deleteChat(self, chatId):
+    def deleteChat(self, chatId):
         chatId = self.valid_chatId(chatId)
-        result = await self.page_evaluate("(chatId) => WPP.chat.delete(chatId)", chatId)
+        result = self.ThreadsafeBrowser.sync_page_evaluate("(chatId) => WPP.chat.delete(chatId)", chatId)
         return result and result.get("status") == 200
 
-    async def archiveChat(self, chatId, option=True):
+    def archiveChat(self, chatId, option=True):
         chatId = self.valid_chatId(chatId)
-        return await self.page_evaluate("({ chatId, option }) => WPP.chat.archive(chatId, option)",
+        return self.ThreadsafeBrowser.sync_page_evaluate("({ chatId, option }) => WPP.chat.archive(chatId, option)",
                                         {"chatId": chatId, "option": option})
 
-    async def pinChat(self, chatId, option, nonExistent=False):
+    def pinChat(self, chatId, option, nonExistent=False):
         chatId = self.valid_chatId(chatId)
         if nonExistent:
-            await self.page_evaluate("({ chatId }) => WPP.chat.find(chatId)", chatId)
+            self.ThreadsafeBrowser.sync_page_evaluate("({ chatId }) => WPP.chat.find(chatId)", chatId)
 
-        return await self.page_evaluate("({ chatId, option }) => WPP.chat.pin(chatId, option)",
+        return self.ThreadsafeBrowser.sync_page_evaluate("({ chatId, option }) => WPP.chat.pin(chatId, option)",
                                         {"chatId": chatId, "option": option})
 
-    async def starMessage(self, messagesId, star=True):
-        await self.page_evaluate("({ messagesId, star }) => WAPI.starMessages(messagesId, star)",
+    def starMessage(self, messagesId, star=True):
+        self.ThreadsafeBrowser.sync_page_evaluate("({ messagesId, star }) => WAPI.starMessages(messagesId, star)",
                                  {"messagesId": messagesId, "star": star})
```

### Comparing `WPP_Whatsapp-0.0.1/WPP_Whatsapp/api/layers/GroupLayer.py` & `WPP_Whatsapp-0.1.0/WPP_Whatsapp/api/layers/GroupLayer.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,67 +1,67 @@
 from WPP_Whatsapp.api.layers.RetrieverLayer import RetrieverLayer
 
 
 class GroupLayer(RetrieverLayer):
-    async def leaveGroup(self, groupId):
+    def leaveGroup(self, groupId):
         groupId = self.valid_chatId(groupId)
-        return await self.page_evaluate("(groupId) => WPP.group.leave(groupId)", groupId)
+        return self.ThreadsafeBrowser.sync_page_evaluate("(groupId) => WPP.group.leave(groupId)", groupId)
 
-    async def getGroupMembersIds(self, groupId):
+    def getGroupMembersIds(self, groupId):
         groupId = self.valid_chatId(groupId)
-        return await self.page_evaluate("""(groupId) => Promise.resolve(WPP.group.getParticipants(groupId)).then(
+        return self.ThreadsafeBrowser.sync_page_evaluate("""(groupId) => Promise.resolve(WPP.group.getParticipants(groupId)).then(
           (participants) => participants.map((p) => p.id))""", groupId)
 
-    async def getGroupMembers(self, groupId):
+    def getGroupMembers(self, groupId):
         groupId = self.valid_chatId(groupId)
-        membersIds = await self.getGroupMembersIds(groupId)
+        membersIds = self.getGroupMembersIds(groupId)
         return [self.getContact(memberId.get("_serialized")) for memberId in membersIds]
 
-    async def getGroupInviteLink(self, chatId):
+    def getGroupInviteLink(self, chatId):
         chatId = self.valid_chatId(chatId)
-        code = await self.page_evaluate("(chatId) => WPP.group.getInviteCode(chatId)", chatId)
+        code = self.ThreadsafeBrowser.sync_page_evaluate("(chatId) => WPP.group.getInviteCode(chatId)", chatId)
 
         return f"https://chat.whatsapp.com/{code}" if code else None
 
-    async def revokeGroupInviteLink(self, chatId):
+    def revokeGroupInviteLink(self, chatId):
         chatId = self.valid_chatId(chatId)
-        code = await self.page_evaluate("(chatId) => WPP.group.revokeInviteCode(chatId)", chatId)
+        code = self.ThreadsafeBrowser.sync_page_evaluate("(chatId) => WPP.group.revokeInviteCode(chatId)", chatId)
 
         return f"https://chat.whatsapp.com/{code}" if code else None
 
-    async def getGroupInfoFromInviteLink(self, invite_code):
+    def getGroupInfoFromInviteLink(self, invite_code):
         invite_code = invite_code.replace('chat.whatsapp.com/', '')
         invite_code = invite_code.replace('invite/', '')
         invite_code = invite_code.replace('https://', '')
         invite_code = invite_code.replace('http://', '')
-        return await self.page_evaluate("(inviteCode) => WPP.group.getGroupInfoFromInviteCode(inviteCode)", invite_code)
+        return self.ThreadsafeBrowser.sync_page_evaluate("(inviteCode) => WPP.group.getGroupInfoFromInviteCode(inviteCode)", invite_code)
 
-    async def createGroup(self, groupName, contacts=[]):
-        return await self.page_evaluate("({ groupName, contacts }) => WPP.group.create(groupName, contacts)",
+    def createGroup(self, groupName, contacts=[]):
+        return self.ThreadsafeBrowser.sync_page_evaluate("({ groupName, contacts }) => WPP.group.create(groupName, contacts)",
                                         {"groupName": groupName, "contacts": contacts})
 
-    async def removeParticipant(self, groupId, participantId):
+    def removeParticipant(self, groupId, participantId):
         groupId = self.valid_chatId(groupId)
-        await self.page_evaluate("""({ groupId, participantId }) =>
+        self.ThreadsafeBrowser.sync_page_evaluate("""({ groupId, participantId }) =>
         WPP.group.removeParticipants(groupId, participantId)""", {"groupId": groupId, "participantId": participantId})
         return True
 
-    async def addParticipant(self, groupId, participantId):
+    def addParticipant(self, groupId, participantId):
         groupId = self.valid_chatId(groupId)
-        return await self.page_evaluate("""({ groupId, participantId }) =>
+        return self.ThreadsafeBrowser.sync_page_evaluate("""({ groupId, participantId }) =>
         WPP.group.addParticipants(groupId, participantId)""", {"groupId": groupId, "participantId": participantId})
 
-    async def getGroupAdmins(self, chatId):
+    def getGroupAdmins(self, chatId):
         chatId = self.valid_chatId(chatId)
-        participants = await self.page_evaluate("""(chatId) =>
+        participants = self.ThreadsafeBrowser.sync_page_evaluate("""(chatId) =>
         Promise.resolve(WPP.group.getParticipants(chatId)).then(
           (participants) => participants.map((p) => p.toJSON())
         )""", chatId)
         # return [participant for participant in participants if participant.get("isAdmin")]
         return [participant.get("id") for participant in participants if participant.get("isAdmin")]
 
-    async def joinGroup(self, invite_code):
+    def joinGroup(self, invite_code):
         invite_code = invite_code.replace('chat.whatsapp.com/', '')
         invite_code = invite_code.replace('invite/', '')
         invite_code = invite_code.replace('https://', '')
         invite_code = invite_code.replace('http://', '')
-        return await self.page_evaluate("(inviteCode) => WPP.group.joinGroup(inviteCode)", invite_code)
+        return self.ThreadsafeBrowser.sync_page_evaluate("(inviteCode) => WPP.group.joinGroup(inviteCode)", invite_code)
```

### Comparing `WPP_Whatsapp-0.0.1/WPP_Whatsapp/api/layers/HostLayer.py` & `WPP_Whatsapp-0.1.0/WPP_Whatsapp/api/layers/HostLayer.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,25 +1,22 @@
 import asyncio
+import inspect
 import logging
 import os
-import traceback
-from asyncio import sleep
+from time import sleep
 from datetime import datetime
 from pathlib import Path
-
-import pyqrcode
-from playwright._impl import _api_types
-from playwright.async_api import Page, BrowserContext
-
+from playwright.async_api import Page
 from WPP_Whatsapp.api.const import whatsappUrl
+from WPP_Whatsapp.api.helpers.function import asciiQr
+from WPP_Whatsapp.PlaywrightSafeThread import ThreadsafeBrowser
 
 
 class HostLayer:
     page: Page
-    browser: BrowserContext
     session: str
     options = {}
     logger: logging
     autoCloseInterval = None
     autoCloseCalled = False
     isInitialized = False
     isInjected = False
@@ -28,72 +25,37 @@
     isInChat = False
     logQR = False
     checkStartInterval = None
     urlCode = ''
     status = ''
     attempt = 0
     autoClose = 0
-    # catchQR_dict = {}
-    # statusFind_dict = {}
-    # onLoadingScreen = LoadingScreen()
     lastPercent = None
     lastPercentMessage = None
-    Browser: "Browser"
+    ThreadsafeBrowser: "ThreadsafeBrowser"
 
     def __init__(self):
-        # self.session = session
-        # asyncio.set_event_loop(self.loop)
-
-        super().__init__()
         self.__initialize()
-        # self.start()
-
-    async def page_evaluate(self, expression, arg=None):
-        try:
-            return await self.Browser.page_evaluate(expression, arg)
-        except _api_types.Error as error:
-            if "WPP is not defined" in error.message:
-                pass
-
-            elif "Cannot read properties of null" in error.message:
-                pass
-
-            else:
-                raise error
-
-    async def page_wait_for_function(self, expression, arg=None, timeout=None, polling=None):
-        try:
-            return await self.Browser.page_wait_for_function(expression, arg, timeout, polling)
-        except _api_types.Error as error:
-            if "WPP is not defined" in error.message:
-                pass
-
-            elif "Cannot read properties of null" in error.message:
-                pass
-
-            else:
-                raise error
 
     def catchQR(self, **kwargs):
         # self.catchQR_dict = kwargs
         pass
 
     def statusFind(self, status, session):
         self.status = status
 
     def onLoadingScreen(self, percent, message):
         pass
 
     def __initialize(self):
         self.page.on('close', self.on_close)
-
         self.page.on('load', self.on_load)
         self.isInitialized = True
 
-    def on_close(self):
+    async def on_close(self):
         self.logger.info(f'{self.session}: Page Closed')
         self.cancelAutoClose()
 
     async def on_load(self):
         self.logger.info(f'{self.session}: Page loaded')
         await self._afterPageLoad()
 
@@ -102,71 +64,59 @@
         options = {
             "deviceName": self.options.get("deviceName"),
             "disableGoogleAnalytics": self.options.get("disableGoogleAnalytics"),
             "googleAnalyticsId": self.options.get("googleAnalyticsId"),
             "linkPreviewApiServers": self.options.get("linkPreviewApiServers"),
             "poweredBy": self.options.get("poweredBy"),
         }
-        await self.page_evaluate("""(options) => {window.WPPConfig = options;}""", options)
-
+        self.logger.info(f'{self.session}: Start WPPConfig')
+        await self.ThreadsafeBrowser.page_evaluate("""(options) => {window.WPPConfig = options;}""", options)
+        # await self.ThreadsafeBrowser.page.page_evaluate("""(options) => {window.WPPConfig = options;}""", options)
+        self.logger.info(f'{self.session}: WPPConfig')
         self.isInjected = False
-        try:
-            # TODO:____
-            if await self.inject_api():
-                self.isInjected = True
-                self.logger.info(f'{self.session}: wapi.js injected')
-                await self.afterPageScriptInjected()
-        except:
-            traceback.print_exc()
+        # TODO:
+        if await self.inject_api():
+            self.isInjected = True
+            self.logger.info(f'{self.session}: wapi.js injected')
+            await self.afterPageScriptInjected()
+        else:
             self.logger.info(f'{self.session}: wapi.js failed')
 
     async def _afterPageScriptInjectedHost(self):
         version = await self.getWAVersion()
         self.logger.info(f'{self.session}: WhatsApp WEB version: {version}')
         version = await self.getWAJSVersion()
         self.logger.info(f'{self.session}: WA-JS version: {version}')
-        await self.page_evaluate("""() => {WPP.on('conn.auth_code_change', window.checkQrCode);}""")
-        await self.page_evaluate("""() => {WPP.on('conn.main_ready', window.checkInChat);}""")
+        await self.ThreadsafeBrowser.page_evaluate("""() => {WPP.on('conn.auth_code_change', window.checkQrCode);}""")
+        await self.ThreadsafeBrowser.page_evaluate("""() => {WPP.on('conn.main_ready', window.checkInChat);}""")
         await self.__checkQrCode()
         await self.__checkInChat()
 
-    async def start(self):
-        try:
-            if self.isStarted:
-                return
-
-            self.isStarted = True
-            # ToDo:
-            await self.initWhatsapp()
-            await self.page.expose_function('checkQrCode', self.__checkQrCode)
-            await self.page.expose_function('checkInChat', self.__checkInChat)
-
-            # ToDo:
-            # self.checkStartInterval = self.__setInterval(self.__checkStart, 5)
-            # self.page.on('close', lambda: print("close"))
-            # self.page.on('close', lambda: self.clearInterval(self.checkStartInterval))
-            return True
-        except:
-            # traceback.print_exc()
-            print("failed start")
+    def start(self):
+        if self.isStarted:
+            return
 
-    async def initWhatsapp(self):
-        try:
-            self.logger.info(f'{self.session}: Loading WhatsApp WEB')
-            await self.page.goto(whatsappUrl, wait_until="domcontentloaded")
-            self.logger.info(f'{self.session}: WhatsApp WEB loaded')
-            # ToDo: unregisterServiceWorker, setWhatsappVersion,
-            return self.page
-        except:
-            traceback.print_exc()
+        self.isStarted = True
+        # ToDo:
+        self.initWhatsapp()
+        self.ThreadsafeBrowser.sync_expose_function('checkQrCode', self.__checkQrCode)
+        self.ThreadsafeBrowser.sync_expose_function('checkInChat', self.__checkInChat)
+        # ToDo:
+        # self.checkStartInterval = self.__setInterval(self.__checkStart, 10)
+        self.page.on('close', lambda: self.clearInterval(self.checkStartInterval))
+        return True
+
+    def initWhatsapp(self):
+        self.logger.info(f'{self.session}: Loading WhatsApp WEB')
+        self.ThreadsafeBrowser.sync_goto(whatsappUrl, wait_until="domcontentloaded")
+        self.logger.info(f'{self.session}: WhatsApp WEB loaded')
+        # ToDo: unregisterServiceWorker, setWhatsappVersion,
 
     async def __checkStart(self):
-        # print("__checkStart")
         need_scan = await self.__needsToScan()
-        # print(need_scan)
 
     async def __checkQrCode(self):
         need_scan = await self.__needsToScan()
         self.isLogged = not need_scan
         if not need_scan:
             self.attempt = 0
             return
@@ -211,237 +161,260 @@
             self.cancelAutoClose()
 
         if (self.autoClose > 0 or self.options.get(
                 "deviceSyncTimeout") > 0) and not self.autoCloseInterval and not self.page.is_closed():
             self.logger.info(f'{self.session}: Closing the page')
             self.autoCloseCalled = True
             self.statusFind('autocloseCalled', self.session)
-            try:
-                if not self.page.is_closed():
-                    await self.page.close()
-            except:
-                # traceback.print_exc()
-                pass
+            if not self.page.is_closed():
+                await self.ThreadsafeBrowser.close()
+
+    def sync_tryAutoClose(self):
+        if self.autoCloseInterval:
+            self.cancelAutoClose()
+
+        if (self.autoClose > 0 or self.options.get(
+                "deviceSyncTimeout") > 0) and not self.autoCloseInterval and not self.page.is_closed():
+            self.logger.info(f'{self.session}: Closing the page')
+            self.autoCloseCalled = True
+            self.statusFind('autocloseCalled', self.session)
+            if not self.page.is_closed():
+                self.ThreadsafeBrowser.sync_close()
 
     def startAutoClose(self, time=None):
         if not time:
             time = self.autoClose
 
         if time > 0 and not self.autoCloseInterval:
             seconds = round(time / 1000)
             self.logger.info(f'{self.session}: Auto close configured to {seconds}s')
             self.remain = seconds
 
             self.autoCloseInterval = self.__setInterval(self.autoCloseIntervalHandel, 5)
 
     def __setInterval(self, func, interval, *args, **kwargs):
+        self.logger.debug(f'{self.session}: setInterval {func}')
         stopped = asyncio.Event()
         loop = kwargs.get('loop') or asyncio.get_event_loop()
 
         async def loop_():
             while not stopped.is_set():
-                await func()
-                await asyncio.sleep(interval)
+                if inspect.iscoroutinefunction(func):
+                    await func()
+                    await asyncio.sleep(interval)
+                else:
+                    func()
+                    await asyncio.sleep(interval)
 
         loop.create_task(loop_())
         return stopped
 
     def clearInterval(self, Interval):
-        try:
-            if Interval:
-                Interval.set()
-                print("Interval", Interval.is_set())
-                # Interval.clear()
-        except:
-            traceback.print_exc()
+        self.logger.debug(f'{self.session}: clearInterval {Interval}')
+        if Interval:
+            Interval.set()
 
-    async def autoCloseIntervalHandel(self):
-        # print("autoCloseIntervalHandel")
+    def autoCloseIntervalHandel(self):
         if self.page.is_closed():
             self.cancelAutoClose()
             return
         self.remain -= 1
         if self.remain % 10 == 0 or self.remain <= 5:
             self.logger.info(f'{self.session}: http => Auto close remain: {self.remain}s')
 
         if self.remain <= 0:
-            await self.tryAutoClose()
+            self.tryAutoClose()
 
     def cancelAutoClose(self):
         self.clearInterval(self.autoCloseInterval)
         self.autoCloseInterval = None
 
     async def __getQrCode(self):
         qr_result = await self.scrapeImg()
         return qr_result
 
-    async def waitForQrCodeScan(self):
+    def waitForQrCodeScan(self):
         if not self.isStarted:
             raise Exception('waitForQrCodeScan error: Session not started')
         while not self.page.is_closed() and not self.isLogged:
-            await sleep(200 / 1000)
-            needScan = await self.__needsToScan()
+            # sleep(200 / 1000)
+            self.ThreadsafeBrowser.sleep(200 / 1000)
+            needScan = self.__sync_needsToScan()
             self.isLogged = not needScan
 
-    async def waitForInChat(self):
+    def waitForInChat(self):
         if not self.isStarted:
             raise Exception('waitForInChat error: Session not started')
 
         if not self.isLogged:
             return False
 
         start = datetime.now()
         while not self.page.is_closed() and self.isLogged and not self.isInChat:
             if 0 < self.options.get("deviceSyncTimeout") <= (datetime.now() - start).seconds:
                 return False
 
-            await sleep(1)
+            sleep(1)
 
-            inChat = await self.isInsideChat()
+            inChat = self.sync_isInsideChat()
             self.isInChat = inChat
 
         return self.isInChat
 
-    # @unsync
-    async def waitForPageLoad(self):
+    def waitForPageLoad(self):
         while not self.isInjected:
-            await sleep(.2)
-            # print("waitForPageLoad")
-        await self.page_wait_for_function("() => WPP.isReady")
+            sleep(.2)
+
+        self.ThreadsafeBrowser.sync_page_wait_for_function("() => WPP.isReady")
 
-    async def waitForLogin(self):
+    def waitForLogin(self):
         self.logger.info(f'{self.session}: http => Waiting page load')
-        await self.waitForPageLoad()
+        self.waitForPageLoad()
         self.logger.info(f'{self.session}: http => Checking is logged...')
-        authenticated = await self.isAuthenticated()
+        authenticated = self.sync_isAuthenticated()
+        self.logger.debug(f'{self.session}: http => {authenticated=}')
         self.startAutoClose()
         if authenticated is False:
             self.logger.info(f'{self.session}: http => Waiting for QRCode Scan...')
             self.statusFind('notLogged', self.session)
-            await self.waitForQrCodeScan()
+            self.waitForQrCodeScan()
             self.logger.info(f'{self.session}: http => Checking QRCode status...')
             # // Wait for interface update
-            await sleep(.2)
-            authenticated = await self.isAuthenticated()
+            sleep(.2)
+            authenticated = self.sync_isAuthenticated()
             if authenticated is None:
                 self.logger.warn(f'{self.session}: Failed to authenticate')
                 self.statusFind('qrReadError', self.session)
             elif authenticated:
                 self.logger.info(f'{self.session}: QRCode Success')
                 self.statusFind('qrReadSuccess', self.session)
             else:
                 self.logger.warn(f'{self.session}: QRCode Fail')
                 self.statusFind('qrReadFail', self.session)
-                await self.tryAutoClose()
+                self.sync_tryAutoClose()
                 raise Exception('Failed to read the QRCode')
         elif authenticated is True:
             self.logger.info(f'{self.session}: Authenticated')
             self.statusFind('isLogged', self.session)
         if authenticated is True:
             # Reset the autoclose counter
             self.cancelAutoClose()
             #  Wait for interface update
-            await sleep(.2)
+            sleep(.2)
             self.startAutoClose(self.options.get("deviceSyncTimeout"))
 
             self.logger.info(f'{self.session}: http => Checking phone is connected...')
-            inChat = await self.waitForInChat()
+            inChat = self.waitForInChat()
             if not inChat:
                 self.logger.warn(f'{self.session}: http => Phone not connected')
                 self.statusFind('phoneNotConnected', self.session)
-                await self.tryAutoClose()
+                self.sync_tryAutoClose()
                 raise Exception("Phone not connected")
             self.cancelAutoClose()
             return True
         if authenticated is False:
-            await self.tryAutoClose()
+            self.sync_tryAutoClose()
             self.logger.warn(f'{self.session}: Not logged')
             raise Exception("Not logged")
 
-        await self.tryAutoClose()
+        self.sync_tryAutoClose()
         if self.autoCloseCalled:
             self.logger.error(f'{self.session}: Auto Close Called')
             raise Exception("Auto Close Called")
 
         if self.page.is_closed():
             self.logger.error(f'{self.session}: Page Closed')
             raise Exception("Page Closed")
 
         self.logger.error(f'{self.session}: Unknow error')
         raise Exception("Unknow error")
 
-    async def getHostDevice(self):
+    def getHostDevice(self):
         """@returns Current host device details"""
-        return await self.page_evaluate("() => WAPI.getHost()")
+        return self.ThreadsafeBrowser.sync_page_evaluate("() => WAPI.getHost()")
 
-    async def getWid(self):
+    def getWid(self):
         """@returns Current wid connected"""
-        return await self.page_evaluate("() => WAPI.getWid()")
+        return self.ThreadsafeBrowser.sync_page_evaluate("() => WAPI.getWid()")
 
     async def getWAVersion(self):
         """Retrieves WA version"""
-        await self.page_wait_for_function("() => WAPI.getWAVersion()")
-        return await self.page_evaluate("() => WAPI.getWAVersion()")
+        await self.ThreadsafeBrowser.page_wait_for_function("() => WAPI.getWAVersion()")
+        return await self.ThreadsafeBrowser.page_evaluate("() => WAPI.getWAVersion()")
 
     async def getWAJSVersion(self):
-        await self.page_wait_for_function("() => WPP.version")
-        return await self.page_evaluate("() => WPP.version")
+        await self.ThreadsafeBrowser.page_wait_for_function("() => WPP.version")
+        return await self.ThreadsafeBrowser.page_evaluate("() => WPP.version")
 
-    async def getConnectionState(self):
-        return await self.page_evaluate("() => {return WPP.whatsapp.Socket.state;}")
+    def getConnectionState(self):
+        return self.ThreadsafeBrowser.sync_page_evaluate("() => {return WPP.whatsapp.Socket.state;}")
 
-    async def isConnected(self):
+    def isConnected(self):
         """Retrieves if the phone is online. Please note that this may not be real time."""
-        return await self.page_evaluate("() => WAPI.isConnected()")
+        return self.ThreadsafeBrowser.sync_page_evaluate("() => WAPI.isConnected()")
 
-    async def isLoggedIn(self):
-        return await self.page_evaluate("() => WAPI.isLoggedIn()")
+    def isLoggedIn(self):
+        return self.ThreadsafeBrowser.sync_page_evaluate("() => WAPI.isLoggedIn()")
 
-    async def getBatteryLevel(self):
-        return await self.page_evaluate("() => WAPI.getBatteryLevel()")
+    def getBatteryLevel(self):
+        return self.ThreadsafeBrowser.sync_page_evaluate("() => WAPI.getBatteryLevel()")
 
-    async def startPhoneWatchdog(self, interval=15000):
-        return await self.page_evaluate("(interval) => WAPI.startPhoneWatchdog(interval)", interval)
+    def startPhoneWatchdog(self, interval=15000):
+        return self.ThreadsafeBrowser.sync_page_evaluate("(interval) => WAPI.startPhoneWatchdog(interval)", interval)
 
-    async def stopPhoneWatchdog(self):
-        return await self.page_evaluate("() => WAPI.stopPhoneWatchdog()")
+    def stopPhoneWatchdog(self):
+        return self.ThreadsafeBrowser.sync_page_evaluate("() => WAPI.stopPhoneWatchdog()")
 
-    async def isMultiDevice(self):
-        return await self.page_evaluate("() => WPP.conn.isMultiDevice()")
+    def isMultiDevice(self):
+        return self.ThreadsafeBrowser.sync_page_evaluate("() => WPP.conn.isMultiDevice()")
 
     async def isAuthenticated(self):
+        try:
+            return await self.ThreadsafeBrowser.page_evaluate("() => WPP.conn.isRegistered()")
+        except Exception as e:
+            self.logger.debug(e)
+            return False
 
-        return await self.page_evaluate("() => WPP.conn.isRegistered()")
+    def sync_isAuthenticated(self):
+        try:
+            return self.ThreadsafeBrowser.sync_page_evaluate("() => WPP.conn.isRegistered()")
+        except Exception as e:
+            self.logger.debug(e)
+            return False
 
     async def __needsToScan(self):
         return not await self.isAuthenticated()
 
+    def __sync_needsToScan(self):
+        return not self.sync_isAuthenticated()
+
     def asciiQr(self, code):
-        return pyqrcode.create(code).terminal(quiet_zone=1)
+        return asciiQr(code=code)
+        # return pyqrcode.create(code).terminal(quiet_zone=1)
 
     async def scrapeImg(self):
-        click = await self.page_evaluate("""() => {
+        click = await self.ThreadsafeBrowser.page_evaluate("""() => {
               const selectorImg = document.querySelector('canvas');
               const selectorUrl = selectorImg.closest('[data-ref]');
               //const buttonReload = selectorUrl.querySelector('[role="button"]') as HTMLButtonElement;
               const buttonReload = selectorUrl.querySelector('button');
               if (buttonReload != null) {
                 buttonReload.click();
                 return true;
               }
               return false;
             }""")
         if click:
-            await self.page_wait_for_function("""() => {
+            await self.ThreadsafeBrowser.page_wait_for_function("""() => {
               const selectorImg = document.querySelector('canvas');
               const selectorUrl = selectorImg.closest('[data-ref]');
               return selectorUrl.getAttribute('data-ref');
             }""")
 
-        result = await self.page_evaluate("""() => {
+        result = await self.ThreadsafeBrowser.page_evaluate("""() => {
               const selectorImg = document.querySelector('canvas');
               const selectorUrl = selectorImg.closest('[data-ref]');
         
               if (selectorImg != null && selectorUrl != null) {
                 let data = {
                   base64Image: selectorImg.toDataURL(),
                   urlCode: selectorUrl.getAttribute('data-ref'),
@@ -450,67 +423,68 @@
               } else {
                 return undefined;
               }
             }""")
         return result
 
     async def isInsideChat(self):
-        result = await self.page_evaluate("() => WPP.conn.isMainReady()")
+        result = await self.ThreadsafeBrowser.page_evaluate("() => WPP.conn.isMainReady()")
+        return result if result else False
+
+    def sync_isInsideChat(self):
+        result = self.ThreadsafeBrowser.sync_page_evaluate("() => WPP.conn.isMainReady()")
         return result if result else False
 
     async def inject_api(self):
-        # {"percent": int, "message": str}
-        try:
-            injected = await self.page_evaluate("""() => {
-                        return (typeof window.WAPI !== 'undefined' &&typeof window.Store !== 'undefined');}"""
-                                                )
-            if injected:
-                print("- already injected ")
-                return
-
-            print(injected)
-            await self.page_evaluate("() => (window?.webpackChunkwhatsapp_web_client?.length || 0) > 3")
-            await self.page_wait_for_function("() => (window?.webpackChunkwhatsapp_web_client?.length || 0) > 3")
-            await sleep(1)
-            await self.page.add_script_tag(
-                url="https://github.com/wppconnect-team/wa-js/releases/download/nightly/wppconnect-wa.js")
-            await self.page_wait_for_function("() => window.WPP?.isReady")
-            await self.page_evaluate("""() => {
-                                  WPP.chat.defaultSendMessageOptions.createChat = true;
-                                  WPP.conn.setKeepAlive(true);
-                                }""")
-            base_dir = Path(__file__).resolve().parent.parent.parent
-            await self.page.add_script_tag(path=os.path.join(base_dir, 'js_lib/wapi.js'))
-            await self._onLoadingScreen()
-            # Make sure WAPI is initialized
-            await self.page_wait_for_function("""() => {
-            return (typeof window.WAPI !== 'undefined' && typeof window.Store !== 'undefined' && window.WPP.isReady);
-            }""")
-            return True
-        except:
-            print("- failed Inject ")
-            traceback.print_exc()
+        self.logger.debug(f'{self.session}: start inject')
+        injected = await self.ThreadsafeBrowser.page_evaluate("""() => {
+                    return (typeof window.WAPI !== 'undefined' &&typeof window.Store !== 'undefined');}"""
+                                                              )
+        if injected:
+            self.logger.info(f'{self.session}: already injected')
+            return
+
+        self.logger.info(f'{self.session}: injected state: {injected}')
+        await self.ThreadsafeBrowser.page_evaluate("() => (window?.webpackChunkwhatsapp_web_client?.length || 0) > 3")
+        await self.ThreadsafeBrowser.page_wait_for_function(
+            "() => (window?.webpackChunkwhatsapp_web_client?.length || 0) > 3")
+        await asyncio.sleep(1)
+        await self.ThreadsafeBrowser.add_script_tag(
+            url="https://github.com/wppconnect-team/wa-js/releases/download/nightly/wppconnect-wa.js")
+        await self.ThreadsafeBrowser.page_wait_for_function("() => window.WPP?.isReady")
+        await self.ThreadsafeBrowser.page_evaluate("""() => {
+                              WPP.chat.defaultSendMessageOptions.createChat = true;
+                              WPP.conn.setKeepAlive(true);
+                            }""")
+        base_dir = Path(__file__).resolve().parent.parent.parent
+        await self.ThreadsafeBrowser.add_script_tag(path=os.path.join(base_dir, 'js_lib/wapi.js'))
+        await self._onLoadingScreen()
+        # Make sure WAPI is initialized
+        await self.ThreadsafeBrowser.page_wait_for_function("""() => {
+        return (typeof window.WAPI !== 'undefined' && typeof window.Store !== 'undefined' && window.WPP.isReady);
+        }""")
+        return True
 
     def loadingScreen(self, percent, message):
-        print("loadingScreen", percent, message)
+        self.logger.info(f'{self.session}: loadingScreen: {percent}, {message}')
         if self.lastPercent != percent or self.lastPercentMessage != message:
             self.onLoadingScreen(percent, message)
             self.lastPercent = percent
             self.lastPercentMessage = message
 
     async def _onLoadingScreen(self):
-        await self.page_evaluate("""function getElementByXpath(path) {
+        await self.ThreadsafeBrowser.page_evaluate("""function getElementByXpath(path) {
         return document.evaluate(path, document, null, XPathResult.FIRST_ORDERED_NODE_TYPE, null).singleNodeValue;
             }""")
         try:
-            await self.page.expose_function('loadingScreen', self.loadingScreen)
+            await self.ThreadsafeBrowser.expose_function('loadingScreen', self.loadingScreen)
         except:
             # Function "loadingScreen" has been already registered
             pass
-        await self.page_evaluate("""
+        await self.ThreadsafeBrowser.page_evaluate("""
         function (selectors) {
               let observer = new MutationObserver(function () {
                 let window2 = window;
 
                 let progressBar = window2.getElementByXpath(selectors.PROGRESS);
                 let progressMessage = window2.getElementByXpath(
                   selectors.PROGRESS_MESSAGE
@@ -531,25 +505,22 @@
               observer.observe(document, {
                 attributes: true,
                 childList: true,
                 characterData: true,
                 subtree: true,
               });
             }""",
-                                 {
-                                     "PROGRESS": "//*[@id='app']/div/div/div[2]/progress",
-                                     "PROGRESS_MESSAGE": "//*[@id='app']/div/div/div[3]",
-                                 })
+                                                   {
+                                                       "PROGRESS": "//*[@id='app']/div/div/div[2]/progress",
+                                                       "PROGRESS_MESSAGE": "//*[@id='app']/div/div/div[3]",
+                                                   })
 
     @staticmethod
     def valid_chatId(chatId):
+        chatId = chatId.replace("+", "")
         if chatId and (not chatId.endswith('@c.us') and not chatId.endswith('@g.us')):
             chatId += '@g.us' if len(chatId) > 15 else '@c.us'
         return chatId
 
-    async def close(self):
+    def close(self):
         if not self.page.is_closed():
-            await self.page.close()
-        try:
-            await self.browser.close()
-        except:
-            pass
+            self.ThreadsafeBrowser.sync_close()
```

### Comparing `WPP_Whatsapp-0.0.1/WPP_Whatsapp/api/layers/LabelsLayer.py` & `WPP_Whatsapp-0.1.0/WPP_Whatsapp/api/layers/LabelsLayer.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from WPP_Whatsapp.api.layers.CatalogLayer import CatalogLayer
 
 
 class LabelsLayer(CatalogLayer):
-    async def addNewLabel(self, name, options):
+    def addNewLabel(self, name, options):
         """
           /**
            * Create New Label
            * @category Labels
            *
            * @example
            * ```javascript
@@ -16,19 +16,19 @@
            * //or
            * client.addNewLabel(`Name of label`, { labelColor: 4292849392 });
            * ```
            * @param name Name of label
            * @param options options of label
            */
         """
-        return await self.page_evaluate("""({ name, options }) => {
+        return self.ThreadsafeBrowser.sync_page_evaluate("""({ name, options }) => {
         WPP.labels.addNewLabel(name, options);
       }""", {"name": name, "options": options})
 
-    async def addOrRemoveLabels(self, chatIds, options):
+    def addOrRemoveLabels(self, chatIds, options):
         """
           /**
            * Add or delete label of chatId
            * @category Labels
            *
            * @example
            * ```javascript
@@ -36,22 +36,22 @@
            * [{labelId:'76', type:'add'},{labelId:'75', type:'remove'}]);
            * //or
            * ```
            * @param chatIds ChatIds
            * @param options options to remove or add
            */
         """
-        return await self.page_evaluate("""({ chatIds, options }) => {
+        return self.ThreadsafeBrowser.sync_page_evaluate("""({ chatIds, options }) => {
         WPP.labels.addOrRemoveLabels(chatIds, options);
       }""", {"chatIds": chatIds, "options": options})
 
-    async def getAllLabels(self):
-        return await self.page_evaluate("() => WPP.labels.getAllLabels()")
+    def getAllLabels(self):
+        return self.ThreadsafeBrowser.sync_page_evaluate("() => WPP.labels.getAllLabels()")
 
-    async def getLabelById(self, Id):
-        return await self.page_evaluate("""({ id }) => {WPP.labels.getLabelById(id); }""", {"id": Id})
+    def getLabelById(self, Id):
+        return self.ThreadsafeBrowser.sync_page_evaluate("""({ id }) => {WPP.labels.getLabelById(id); }""", {"id": Id})
 
-    async def deleteAllLabels(self):
-        return await self.page_evaluate("""() => {WPP.labels.deleteAllLabels();}""")
+    def deleteAllLabels(self):
+        return self.ThreadsafeBrowser.sync_page_evaluate("""() => {WPP.labels.deleteAllLabels();}""")
 
-    async def deleteLabel(self, Id):
-        return await self.page_evaluate("""({ id }) => {WPP.labels.deleteLabel(id); }""", {"id": Id})
+    def deleteLabel(self, Id):
+        return self.ThreadsafeBrowser.sync_page_evaluate("""({ id }) => {WPP.labels.deleteLabel(id); }""", {"id": Id})
```

### Comparing `WPP_Whatsapp-0.0.1/WPP_Whatsapp/api/layers/ListenerLayer.py` & `WPP_Whatsapp-0.1.0/WPP_Whatsapp/api/layers/ListenerLayer.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,14 @@
         self.__listenerEmitter.emit(self.func, *args, **kwargs)
 
 
 class ListenerLayer(ProfileLayer):
     __listenerEmitter = EventEmitter()
 
     def __init__(self):
-        super().__init__()
         self.__listenerEmitter.max_listener = 0
         self.__listenerEmitter.on(onInterfaceChange, self.onInterfaceChange_)
         # ToDo:
         # self.__listenerEmitter[captureRejectionSymbol]
 
     def onInterfaceChange_(self, state):
         self.logger.info(
@@ -63,21 +62,21 @@
             # 'onIncomingCall',
             # 'onRevokedMessage',
             # 'onReactionMessage',
             # 'onPollResponse'
         ]
 
         for func in functions:
-            has = await self.page_evaluate("(func) => typeof window[func] === 'function'", func)
+            has = await self.ThreadsafeBrowser.page_evaluate("(func) => typeof window[func] === 'function'", func)
             if not has:
                 self.logger.debug(f'{self.session}: Exposing {func} function')
                 handel_func = HandelFunc(func, self.session, self.logger, self.__listenerEmitter).handel_func
-                await self.page.expose_function(func, handel_func)
+                await self.ThreadsafeBrowser.expose_function(func, handel_func)
 
-        await self.page_evaluate("""() => {
+        await self.ThreadsafeBrowser.page_evaluate("""() => {
         try {
           if (!window['onMessage'].exposed) {
             WPP.on('chat.new_message', (msg) => {
               if (msg.isSentByMe || msg.isStatusV3) {
                 return;
               }
               const serialized = WAPI.processMessageObj(msg, false, false);
@@ -339,18 +338,18 @@
            * }
            * ```
            *
            * @param id contact id (xxxxx@c.us) or group id: xxxxx-yyyy@g.us
            * @returns number of subscribed
            */
         """
-        self.page_evaluate("(id) => WAPI.subscribePresence(id)", id_)
+        await self.ThreadsafeBrowser.page_evaluate("(id) => WAPI.subscribePresence(id)", id_)
 
     async def unsubscribePresence(self, id_):
-        self.page_evaluate("(id) => WAPI.unsubscribePresence(id)", id_)
+        await self.ThreadsafeBrowser.page_evaluate("(id) => WAPI.unsubscribePresence(id)", id_)
 
     def onRevokedMessage(self, callback):
         """ """
         return self.__registerEvent("onRevokedMessage", callback)
 
     def onReactionMessage(self, callback):
         """ """
```

### Comparing `WPP_Whatsapp-0.0.1/WPP_Whatsapp/api/layers/ProfileLayer.py` & `WPP_Whatsapp-0.1.0/WPP_Whatsapp/api/layers/ProfileLayer.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 from WPP_Whatsapp.api.layers.StatusLayer import StatusLayer
 
 
 class ProfileLayer(StatusLayer):
-    async def sendMute(self, chatId, time, type):
+    def sendMute(self, chatId, time, type):
         """
           /**
            * @category Chat
            * @param contactsId Example: 0000@c.us | [000@c.us, 1111@c.us]
            * @param time duration of silence
            * @param type kind of silence "hours" "minutes" "year"
            * To remove the silence, just enter the contact parameter
            */
         """
         chatId = self.valid_chatId(chatId)
-        return await self.page_evaluate("(id, time, type) => WAPI.sendMute(id, time, type)",
+        return self.ThreadsafeBrowser.sync_page_evaluate("(id, time, type) => WAPI.sendMute(id, time, type)",
                                         {"id": chatId, "time": time, "type": type})
 
-    async def setProfileStatus(self, status):
+    def setProfileStatus(self, status):
         """
           /**
            * Sets current user profile status
            * @category Profile
            * @param status
            */
         """
-        return await self.page_evaluate("""({ status }) => {
+        return self.ThreadsafeBrowser.sync_page_evaluate("""({ status }) => {
             WPP.profile.setMyStatus(status);
           }""", status)
 
-    async def setProfilePic(self, pathOrBase64, to):
+    def setProfilePic(self, pathOrBase64, to):
         pass
         # ToDO:
         # base64 = ''
         # if pathOrBase64.startswith('data:'):
         #     base64 = pathOrBase64
         # else:
         #     if pathOrBase64 and os.path.exists(pathOrBase64):
@@ -42,9 +42,9 @@
         #     print("Empty or invalid file or base64")
         #     return
         # mimeInfo = base64.split(";base64")[0].split(":")[-1]
         # if 'image' not in mimeInfo:
         #     print('Not an image, allowed formats png, jpeg and webp')
         #     return
 
-    async def setProfileName(self, name):
-        return await self.page_evaluate("({ name }) => {WAPI.setMyName(name);}", name)
+    def setProfileName(self, name):
+        return self.ThreadsafeBrowser.sync_page_evaluate("({ name }) => {WAPI.setMyName(name);}", name)
```

### Comparing `WPP_Whatsapp-0.0.1/WPP_Whatsapp/api/layers/RetrieverLayer.py` & `WPP_Whatsapp-0.1.0/WPP_Whatsapp/api/layers/RetrieverLayer.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,176 +1,176 @@
 from WPP_Whatsapp.api.layers.SenderLayer import SenderLayer
 
 
 class RetrieverLayer(SenderLayer):
-    async def getSessionTokenBrowser(self, removePath):
+    def getSessionTokenBrowser(self, removePath):
         # @returns obj [token]
         if removePath:
-            await self.page_evaluate("() => {window['pathSession'] = true;}")
+            self.ThreadsafeBrowser.sync_page_evaluate("() => {window['pathSession'] = true;}")
 
-        if await self.isMultiDevice():
-            return await self.page_evaluate("""() => {
+        if self.isMultiDevice():
+            return self.ThreadsafeBrowser.sync_page_evaluate("""() => {
           if (window.localStorage) {
             return {
               WABrowserId:
                 window.localStorage.getItem('WABrowserId') || 'MultiDevice',
               WASecretBundle: 'MultiDevice',
               WAToken1: 'MultiDevice',
               WAToken2: 'MultiDevice',
             };
           }
           return null;
         }""")
-        return await self.page_evaluate("""() => {
+        return self.ThreadsafeBrowser.sync_page_evaluate("""() => {
         if (window.localStorage) {
           return {
             WABrowserId: window.localStorage.getItem('WABrowserId'),
             WASecretBundle: window.localStorage.getItem('WASecretBundle'),
             WAToken1: window.localStorage.getItem('WAToken1'),
             WAToken2: window.localStorage.getItem('WAToken2'),
           };
         }
         return null;
       }""")
 
-    async def getTheme(self):
+    def getTheme(self):
         # @returns string light or dark
-        return await self.page_evaluate("() => WAPI.getTheme()")
+        return self.ThreadsafeBrowser.sync_page_evaluate("() => WAPI.getTheme()")
 
-    async def getAllChats(self, withNewMessageOnly=False):
+    def getAllChats(self, withNewMessageOnly=False):
         # @returns array of [Chat]
         if withNewMessageOnly:
-            return await self.page_evaluate("() => WAPI.getAllChatsWithNewMsg()")
+            return self.ThreadsafeBrowser.sync_page_evaluate("() => WAPI.getAllChatsWithNewMsg()")
 
-        return await self.page_evaluate("() => WAPI.getAllChats()")
+        return self.ThreadsafeBrowser.sync_page_evaluate("() => WAPI.getAllChats()")
 
-    async def checkNumberStatus(self, contactId):
+    def checkNumberStatus(self, contactId):
         # @returns contact detial as promise
         contactId = self.valid_chatId(contactId)
-        return await self.page_evaluate("(contactId) => WAPI.checkNumberStatus(contactId)", contactId)
+        return self.ThreadsafeBrowser.sync_page_evaluate("(contactId) => WAPI.checkNumberStatus(contactId)", contactId)
 
-    async def getAllChatsWithMessages(self, withNewMessageOnly=False):
+    def getAllChatsWithMessages(self, withNewMessageOnly=False):
         # @returns array of [Chat]
-        return await self.page_evaluate("""(withNewMessageOnly: boolean) =>
+        return self.ThreadsafeBrowser.sync_page_evaluate("""(withNewMessageOnly: boolean) =>
         WAPI.getAllChatsWithMessages(withNewMessageOnly)""", withNewMessageOnly)
 
-    async def getAllGroups(self, withNewMessagesOnly):
+    def getAllGroups(self, withNewMessagesOnly):
         # @returns array of groups
-        return await self.page_evaluate("""async ({ withNewMessagesOnly }) => {
+        return self.ThreadsafeBrowser.sync_page_evaluate("""async ({ withNewMessagesOnly }) => {
         const chats = await WPP.chat.list({
           onlyGroups: true,
           onlyWithUnreadMessage: withNewMessagesOnly,
         });
 
         const groups = await Promise.all(
           chats.map((c) => WPP.group.ensureGroup(c.id))
         );
 
         return groups.map((g) => WAPI._serializeChatObj(g));
       }""", withNewMessagesOnly)
 
-    async def getAllBroadcastList(self):
+    def getAllBroadcastList(self):
         # @returns array of broadcast list
-        chats = await self.page_evaluate("""() => WAPI.getAllChats()""")
+        chats = self.ThreadsafeBrowser.sync_page_evaluate("""() => WAPI.getAllChats()""")
         if chats:
             return list(
                 filter(lambda x: x.get("isBroadcast") and x.get("id").get("_serialized") != 'status@broadcast', chats))
 
-    async def getContact(self, contactId):
+    def getContact(self, contactId):
         # @returns contact detial as promise
         contactId = self.valid_chatId(contactId)
-        return await self.page_evaluate("(contactId) => WAPI.getContact(contactId)", contactId)
+        return self.ThreadsafeBrowser.sync_page_evaluate("(contactId) => WAPI.getContact(contactId)", contactId)
 
-    async def getAllContacts(self):
+    def getAllContacts(self):
         # @returns array of [Contact]
-        return await self.page_evaluate("() => WAPI.getAllContacts()")
+        return self.ThreadsafeBrowser.sync_page_evaluate("() => WAPI.getAllContacts()")
 
-    async def getChatById(self, contactId):
+    def getChatById(self, contactId):
         contactId = self.valid_chatId(contactId)
-        return await self.page_evaluate("(contactId) => WAPI.getChatById(contactId)", contactId)
+        return self.ThreadsafeBrowser.sync_page_evaluate("(contactId) => WAPI.getChatById(contactId)", contactId)
 
-    async def getChat(self, contactId):
+    def getChat(self, contactId):
         contactId = self.valid_chatId(contactId)
         return self.getChatById(contactId)
 
-    async def getProfilePicFromServer(self, chatId):
+    def getProfilePicFromServer(self, chatId):
         # @returns url of the chat picture or undefined if there is no picture for the chat.
         chatId = self.valid_chatId(chatId)
-        return await self.page_evaluate("(chatId) => WAPI._profilePicfunc(chatId)", chatId)
+        return self.ThreadsafeBrowser.sync_page_evaluate("(chatId) => WAPI._profilePicfunc(chatId)", chatId)
 
-    async def loadEarlierMessages(self, contactId):
+    def loadEarlierMessages(self, contactId):
         contactId = self.valid_chatId(contactId)
-        return await self.page_evaluate("(contactId) => WAPI.loadEarlierMessages(contactId)", contactId)
+        return self.ThreadsafeBrowser.sync_page_evaluate("(contactId) => WAPI.loadEarlierMessages(contactId)", contactId)
 
-    async def getStatus(self, contactId):
+    def getStatus(self, contactId):
         contactId = self.valid_chatId(contactId)
-        return await self.page_evaluate("""async (contactId) => {
+        return self.ThreadsafeBrowser.sync_page_evaluate("""async (contactId) => {
                                         const status = await WPP.contact.getStatus(contactId);
                                 
                                         return {
                                           id: contactId,
                                           status: (status as any)?.status || status,
                                         };
                                       }""", contactId)
 
-    async def getNumberProfile(self, contactId):
+    def getNumberProfile(self, contactId):
         contactId = self.valid_chatId(contactId)
-        return await self.page_evaluate("(contactId) => WAPI.getNumberProfile(contactId)", contactId)
+        return self.ThreadsafeBrowser.sync_page_evaluate("(contactId) => WAPI.getNumberProfile(contactId)", contactId)
 
-    async def getUnreadMessages(self, includeMe, includeNotifications, useUnreadCount):
-        return await self.page_evaluate(
+    def getUnreadMessages(self, includeMe, includeNotifications, useUnreadCount):
+        return self.ThreadsafeBrowser.sync_page_evaluate(
             """({ includeMe, includeNotifications, useUnreadCount }) =>
         WAPI.getUnreadMessages(includeMe, includeNotifications, useUnreadCount)""",
             {"includeMe": includeMe, "includeNotifications": includeNotifications, "useUnreadCount": useUnreadCount})
 
-    async def getAllUnreadMessages(self):
-        return await self.page_evaluate("() => WAPI.getAllUnreadMessages()")
+    def getAllUnreadMessages(self):
+        return self.ThreadsafeBrowser.sync_page_evaluate("() => WAPI.getAllUnreadMessages()")
 
-    async def getAllNewMessages(self):
+    def getAllNewMessages(self):
         # @deprecated Use getAllUnreadMessages
-        return await self.page_evaluate("() => WAPI.getAllNewMessages()")
+        return self.ThreadsafeBrowser.sync_page_evaluate("() => WAPI.getAllNewMessages()")
 
-    async def getAllMessagesInChat(self, chatId, includeMe=False, includeNotifications=False):
+    def getAllMessagesInChat(self, chatId, includeMe=False, includeNotifications=False):
         chatId = self.valid_chatId(chatId)
         """
         * Retrieves all messages already loaded in a chat
         * For loading every message use loadAndGetAllMessagesInChat
         """
-        return await self.page_evaluate("""({ chatId, includeMe, includeNotifications }) =>
+        return self.ThreadsafeBrowser.sync_page_evaluate("""({ chatId, includeMe, includeNotifications }) =>
         WAPI.getAllMessagesInChat(chatId, includeMe, includeNotifications)""",
                                         {"chatId": chatId, "includeMe": includeMe,
                                          "includeNotifications": includeNotifications})
 
-    async def loadAndGetAllMessagesInChat(self, chatId, includeMe=False, includeNotifications=False):
+    def loadAndGetAllMessagesInChat(self, chatId, includeMe=False, includeNotifications=False):
         chatId = self.valid_chatId(chatId)
         """
         * Loads and Retrieves all Messages in a chat
         """
-        return await self.page_evaluate("""({ chatId, includeMe, includeNotifications }) =>
+        return self.ThreadsafeBrowser.sync_page_evaluate("""({ chatId, includeMe, includeNotifications }) =>
         WAPI.loadAndGetAllMessagesInChat(chatId, includeMe, includeNotifications)""",
                                         {"chatId": chatId, "includeMe": includeMe,
                                          "includeNotifications": includeNotifications})
 
-    async def getChatIsOnline(self, chatId):
+    def getChatIsOnline(self, chatId):
         chatId = self.valid_chatId(chatId)
-        return await self.page_evaluate("(chatId) => WAPI.getChatIsOnline(chatId)", chatId)
+        return self.ThreadsafeBrowser.sync_page_evaluate("(chatId) => WAPI.getChatIsOnline(chatId)", chatId)
 
-    async def getLastSeen(self, chatId):
+    def getLastSeen(self, chatId):
         chatId = self.valid_chatId(chatId)
-        return await self.page_evaluate("(chatId) => WAPI.getLastSeen(chatId)", chatId)
+        return self.ThreadsafeBrowser.sync_page_evaluate("(chatId) => WAPI.getLastSeen(chatId)", chatId)
 
-    async def getPlatformFromMessage(self, msgId):
+    def getPlatformFromMessage(self, msgId):
         """
         * Get the platform message from message ID
         * The platform can be:
             * android
             * iphone
             * web
             * unknown
         """
-        return await self.page_evaluate("(msgId) => WPP.chat.getPlatformFromMessage(msgId)", msgId)
+        return self.ThreadsafeBrowser.sync_page_evaluate("(msgId) => WPP.chat.getPlatformFromMessage(msgId)", msgId)
 
-    async def getReactions(self, msgId):
-        return await self.page_evaluate("(msgId) => WPP.chat.getReactions(msgId)", msgId)
+    def getReactions(self, msgId):
+        return self.ThreadsafeBrowser.sync_page_evaluate("(msgId) => WPP.chat.getReactions(msgId)", msgId)
 
-    async def getVotes(self, msgId):
-        return await self.page_evaluate("(msgId) => WPP.chat.getVotes(msgId)", msgId)
+    def getVotes(self, msgId):
+        return self.ThreadsafeBrowser.sync_page_evaluate("(msgId) => WPP.chat.getVotes(msgId)", msgId)
```

### Comparing `WPP_Whatsapp-0.0.1/WPP_Whatsapp/api/layers/SenderLayer.py` & `WPP_Whatsapp-0.1.0/WPP_Whatsapp/api/layers/SenderLayer.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,110 +1,80 @@
 import base64
 import mimetypes
 import os
-
 from WPP_Whatsapp.api.layers.ListenerLayer import ListenerLayer
 
 
 class SenderLayer(ListenerLayer):
 
-    async def sendLinkPreview(self, chatId, url, text=''):
+    def sendLinkPreview(self, chatId, url, text=''):
         """
         * Automatically sends a link with the auto generated link preview. You can also add a custom message to be added.
         * Deprecated: please use {@link sendText}
         """
         message = text if url in text else f"{text}\n{url}"
         chatId = self.valid_chatId(chatId)
-        result = await self.page_evaluate("""({ chatId, message }) => {
+        result = self.ThreadsafeBrowser.sync_page_evaluate("""({ chatId, message }) => {
                     return WPP.chat.sendTextMessage(chatId, message, { linkPreview: true });
                     }""", {"chatId": chatId, "message": message})
         return result
 
-    async def sendText(self, to, content, options=None):
+    def sendText(self, to, content, options=None):
         """
-          /**
-           * Sends a text message to given chat
-           * @category Chat
-           * @param to chat id: xxxxx@us.c
-           * @param content text message
-           *
-           * @example
-           * ```javascript
-           * // Simple message
-           * client.sendText('<number>@c.us', 'A simple message');
-           *
-           * // With buttons
-           * client.sendText('<number>@c.us', 'WPPConnect message with buttons', {
-           *    useTemplateButtons: true, // False for legacy
-           *    buttons: [
-           *      {
-           *        url: 'https://wppconnect.io/',
-           *        text: 'WPPConnect Site'
-           *      },
-           *      {
-           *        phoneNumber: '+55 11 22334455',
-           *        text: 'Call me'
-           *      },
-           *      {
-           *        id: 'your custom id 1',
-           *        text: 'Some text'
-           *      },
-           *      {
-           *        id: 'another id 2',
-           *        text: 'Another text'
-           *      }
-           *    ],
-           *    title: 'Title text' // Optional
-           *    footer: 'Footer text' // Optional
-           * });
-           * ```
-           */
+           Sends a text message to given chat
+           @category Chat
+           @param to chat to: xxxxx@us.c
+           @param content text message
+           @param options dict
+           @example
+           // Simple message
+           client.sendText('<number>@c.us', 'A simple message')
+           :return: dict
         """
         if not options:
             options = {}
         to = self.valid_chatId(to)
-        send_result = await self.page_evaluate("""({ to, content, options }) =>
+        send_result = self.ThreadsafeBrowser.sync_page_evaluate("""({ to, content, options }) =>
                             WPP.chat.sendTextMessage(to, content, {
                               ...options,
                               waitForAck: true,
                             })""", {"to": to, "content": content, "options": options})
         self.logger.debug(f'{self.session}: Send Message {send_result=}')
-        # result = await self.page_evaluate("""async (messageId) => {
-        #                 return JSON.parse(JSON.stringify(await WAPI.getMessageById(messageId)));
-        #               }""", send_result.get("id"))
+
         return send_result
 
-    async def sendMessageOptions(self, chat, content, options=None):
+    def sendMessageOptions(self, chat, content, options=None):
         if not options:
             options = {}
-        message_id = await self.page_evaluate("""({ chat, content, options }) => {
+        message_id = self.ThreadsafeBrowser.sync_page_evaluate("""({ chat, content, options }) => {
         return WAPI.sendMessageOptions(chat, content, options);
       }""", {"chat": chat, "content": content, "options": options})
-        result = await self.page_evaluate("""(messageId) => WAPI.getMessageById(messageId)""", message_id)
+        result = self.ThreadsafeBrowser.sync_page_evaluate("""(messageId) => WAPI.getMessageById(messageId)""",
+                                                           message_id)
         return result
 
-    async def sendImage(self, to, filePath, filename="", caption="", quotedMessageId=None, isViewOnce=None):
+    def sendImage(self, to, filePath, filename="", caption="", quotedMessageId=None, isViewOnce=None):
         to = self.valid_chatId(to)
         if filePath and os.path.exists(filePath):
             _base64 = self.convert_to_base64(filePath)
             filename = os.path.basename(filePath) if not filename else filename
-            return await self.sendImageFromBase64(to, _base64, filename, caption, quotedMessageId, isViewOnce)
+            return self.sendImageFromBase64(to, _base64, filename, caption, quotedMessageId, isViewOnce)
         else:
-            print("Path Not Found")
+            raise Exception("Path Not Found")
 
-    async def sendImageFromBase64(self, to, _base64, filename, caption, quotedMessageId, isViewOnce):
+    def sendImageFromBase64(self, to, _base64, filename, caption, quotedMessageId, isViewOnce):
         mime_type = self.base64MimeType(_base64)
         if not mime_type:
-            print("Not valid mimeType")
-            return
+            raise Exception("Not valid mimeType")
+
         if 'image' not in mime_type:
-            print('Not an image, allowed formats png, jpeg and webp')
-            return
+            raise Exception('Not an image, allowed formats png, jpeg and webp')
+
         # filename = filenameFromMimeType(filename, mimeType)
-        result = await self.page_evaluate("""async ({
+        result = self.ThreadsafeBrowser.sync_page_evaluate("""async ({
         to,
         base64,
         filename,
         caption,
         quotedMessageId,
         isViewOnce,
       }) => {
@@ -123,30 +93,31 @@
           sendMsgResult: await result.sendMsgResult,
           error: result.message,
         };
       }""", {"to": to, "base64": _base64, "filename": filename, "caption": caption, "quotedMessageId": quotedMessageId,
              "isViewOnce": isViewOnce})
         return result
 
-    async def reply(self, to, content, quotedMsg):
+    def reply(self, to, content, quotedMsg):
         """
-
-        :param to:
-        :param content:
-        :param quotedMsg: @param quotedMsg Message id to reply to.
-        :return:
+            @param to chat to: xxxxx@us.c
+            @param content text message
+            @param quotedMsg: @param quotedMsg Message id to reply to.
+            @example
+           // Simple message
+           client.reply('<number>@c.us', 'A simple message', '<message-id>')
         """
         to = self.valid_chatId(to)
-        result = await self.page_evaluate("""({ to, content, quotedMsg }) => {
+        result = self.ThreadsafeBrowser.sync_page_evaluate("""({ to, content, quotedMsg }) => {
                                     return WPP.chat.sendTextMessage(to, content, { quotedMsg });
                                   }""", {"to": to, "content": content, "quotedMsg": quotedMsg})
-        message = await self.page_evaluate("(messageId: any) => WAPI.getMessageById(messageId)", result.get("id"))
-        return message
+        # message = self.ThreadsafeBrowser.sync_page_evaluate()("(messageId) => WAPI.getMessageById(messageId)", result.get("id"))
+        return result
 
-    async def sendFile(self, to, pathOrBase64, nameOrOptions, caption):
+    def sendFile(self, to, pathOrBase64, nameOrOptions, caption):
         to = self.valid_chatId(to)
         options = {"type": 'auto-detect'}
         if type(nameOrOptions) is str:
             options["filename"] = nameOrOptions
             options["caption"] = caption
 
         elif type(nameOrOptions) is dict:
@@ -158,83 +129,83 @@
         else:
             if pathOrBase64 and os.path.exists(pathOrBase64):
                 _base64 = self.convert_to_base64(pathOrBase64)
 
             if not options.get("filename"):
                 options["filename"] = os.path.basename(pathOrBase64)
         if not _base64:
-            print("Empty or invalid file or base64")
-            return
+            raise Exception("Empty or invalid file or base64")
 
-        return await self.page_evaluate("""async ({ to, base64, options }) => {
+        return self.ThreadsafeBrowser.sync_page_evaluate("""async ({ to, base64, options }) => {
         const result = await WPP.chat.sendFileMessage(to, base64, options);
         return {
           ack: result.ack,
           id: result.id,
           sendMsgResult: await result.sendMsgResult,
         };
       }""", {"to": to, "base64": _base64, "options": options})
 
-    async def sendContactVcard(self, to, contactsId, name):
+    def sendContactVcard(self, to, contactsId, name):
         """
           /**
            * Sends contact card to iven chat id
            * @category Chat
            * @param to Chat id
            * @param contactsId Example: 0000@c.us | [000@c.us, 1111@c.us]
            */
         """
         to = self.valid_chatId(to)
-        return await self.page_evaluate("""({ to, contactsId, name }) => {
+        return self.ThreadsafeBrowser.sync_page_evaluate("""({ to, contactsId, name }) => {
         return WPP.chat.sendVCardContactMessage(to, {
           id: contactsId,
           name: name,
         });
       }""", {"to": to, "contactsId": contactsId, "name": name})
 
-    async def forwardMessages(self, to, messages, skipMyMessages):
+    def forwardMessages(self, to, messages, skipMyMessages):
         to = self.valid_chatId(to)
-        return await self.page_evaluate("""({ to, messages, skipMyMessages }) =>
+        return self.ThreadsafeBrowser.sync_page_evaluate("""({ to, messages, skipMyMessages }) =>
         WAPI.forwardMessages(to, messages, skipMyMessages)""",
-                                        {"to": to, "messages": messages, "skipMyMessages": skipMyMessages})
+                                                         {"to": to, "messages": messages,
+                                                          "skipMyMessages": skipMyMessages})
 
-    async def sendLocation(self, to, options):
+    def sendLocation(self, to, options):
         to = self.valid_chatId(to)
         options = {
             "lat": options.get("latitude"),
             "lng": options.get("longitude"),
             "title": options.get("title"),
         }
-        return await self.page_evaluate("""async ({ to, options }) => {
+        return self.ThreadsafeBrowser.sync_page_evaluate("""async ({ to, options }) => {
         const result = await WPP.chat.sendLocationMessage(to, options);
 
         return {
           ack: result.ack,
           id: result.id,
           sendMsgResult: await result.sendMsgResult,
         };
       }""", {"to": to, "options": options})
 
-    async def sendSeen(self, chatId):
+    def sendSeen(self, chatId):
         chatId = self.valid_chatId(chatId)
-        return await self.page_evaluate("(chatId) => WPP.chat.markIsRead(chatId)", chatId)
+        return self.ThreadsafeBrowser.sync_page_evaluate("(chatId) => WPP.chat.markIsRead(chatId)", chatId)
 
-    async def startTyping(self, to, duration=None):
+    def startTyping(self, to, duration=None):
         to = self.valid_chatId(to)
-        return await self.page_evaluate("({ to, duration }) => WPP.chat.markIsComposing(to, duration)",
-                                        {"to": to, "duration": duration})
+        return self.ThreadsafeBrowser.sync_page_evaluate("({ to, duration }) => WPP.chat.markIsComposing(to, duration)",
+                                                         {"to": to, "duration": duration})
 
-    async def stopTyping(self, to):
+    def stopTyping(self, to):
         to = self.valid_chatId(to)
-        return await self.page_evaluate("(to) => WPP.chat.markIsPaused(to)", to)
+        return self.ThreadsafeBrowser.sync_page_evaluate("(to) => WPP.chat.markIsPaused(to)", to)
 
-    async def setOnlinePresence(self, online=True):
-        return await self.page_evaluate("(online) => WPP.conn.markAvailable(online)", online)
+    def setOnlinePresence(self, online=True):
+        return self.ThreadsafeBrowser.sync_page_evaluate("(online) => WPP.conn.markAvailable(online)", online)
 
-    async def sendListMessage(self, to, options):
+    def sendListMessage(self, to, options):
         to = self.valid_chatId(to)
         """
           /**
            * Sends a list message
            *
            * ```typescript
            *   // Example
@@ -260,34 +231,35 @@
            *     ],
            *   });
            * ```
            *
            * @category Chat
            */
         """
-        sendResult = await self.page_evaluate("({ to, options }) => WPP.chat.sendListMessage(to, options)",
-                                              {"to": to, "options": options})
-        result = await self.page_evaluate("""async ({ messageId }) => {
+        sendResult = self.ThreadsafeBrowser.sync_page_evaluate(
+            "({ to, options }) => WPP.chat.sendListMessage(to, options)",
+            {"to": to, "options": options})
+        result = self.ThreadsafeBrowser.sync_page_evaluate("""async ({ messageId }) => {
                         return JSON.parse(JSON.stringify(await WAPI.getMessageById(messageId)));
                       }""", sendResult.get("id"))
         return result
 
-    async def setChatState(self, chatId, chatState):
+    def setChatState(self, chatId, chatState):
         """
           /**
            * Sets the chat state
            * Deprecated in favor of Use startTyping or startRecording functions
            * @category Chat
            * @param chatState   Typing = 0, Recording = 1, Paused = 2
            * @param chatId
            * @deprecated Deprecated in favor of Use startTyping or startRecording functions
            */
         """
         chatId = self.valid_chatId(chatId)
-        return await self.page_evaluate("""({ chatState, chatId }) => {
+        return self.ThreadsafeBrowser.sync_page_evaluate("""({ chatState, chatId }) => {
                 WAPI.sendChatstate(chatState, chatId);
               }""", {"chatState": chatState, "chatId": chatId})
 
     @staticmethod
     def convert_to_base64(path):
         mimetypes_add = {"webp": "image/webp"}
         # mime = magic.Magic(mime=True)
```

### Comparing `WPP_Whatsapp-0.0.1/WPP_Whatsapp/api/layers/UILayer.py` & `WPP_Whatsapp-0.1.0/WPP_Whatsapp/api/layers/UILayer.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from WPP_Whatsapp.api.layers.GroupLayer import GroupLayer
 
 
 class UILayer(GroupLayer):
 
-    async def openChat(self, chatId):
+    def openChat(self, chatId):
         chatId = self.valid_chatId(chatId)
-        return await self.page_evaluate("(chatId) => WPP.chat.openChatBottom(chatId)", chatId)
+        return self.ThreadsafeBrowser.page_evaluate("(chatId) => WPP.chat.openChatBottom(chatId)", chatId)
 
-    async def openChatAt(self, chatId, messageId):
+    def openChatAt(self, chatId, messageId):
         chatId = self.valid_chatId(chatId)
-        return await self.page_evaluate("({chatId, messageId}) => WPP.chat.openChatAt(chatId, messageId)",
-                                        {"chatId": chatId, "messageId": messageId})
+        return self.ThreadsafeBrowser.page_evaluate("({chatId, messageId}) => WPP.chat.openChatAt(chatId, messageId)",
+                                                    {"chatId": chatId, "messageId": messageId})
```

### Comparing `WPP_Whatsapp-0.0.1/WPP_Whatsapp/api/model/status_find.py` & `WPP_Whatsapp-0.1.0/WPP_Whatsapp/api/model/status_find.py`

 * *Files identical despite different names*

### Comparing `WPP_Whatsapp-0.0.1/WPP_Whatsapp/controllers/browser.py` & `WPP_Whatsapp-0.1.0/WPP_Whatsapp/controllers/browser.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,16 +7,15 @@
 
 class Browser:
     session: str
     playwright: "Playwright"
     browser: "BrowserContext"
     page: "Page"
 
-    def __init__(self, session: str = "", user_data_dir: str = "", headless=False, *args, **kwargs):
-        self.session = session
+    def __init__(self, user_data_dir: str = "", headless: bool = False, *args, **kwargs):
         self.user_data_dir = user_data_dir
         self.loop = kwargs.get("loop")
         if not self.loop:
             raise Exception("Not Add Loop")
         asyncio.set_event_loop(self.loop)
         self.headless = headless
```

### Comparing `WPP_Whatsapp-0.0.1/WPP_Whatsapp/controllers/initializer.py` & `WPP_Whatsapp-0.1.0/WPP_Whatsapp/controllers/initializer.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,37 +1,31 @@
 import asyncio
 import os
-import traceback
 import types
 from time import sleep
 from typing import Optional
-
-import psutil as psutil
+from WPP_Whatsapp.PlaywrightSafeThread import ThreadsafeBrowser
 
 from WPP_Whatsapp.api.Whatsapp import Whatsapp
 from WPP_Whatsapp.api.const import Logger
-from WPP_Whatsapp.controllers.browser import Browser
 
 
 class Create:
     client: Optional[Whatsapp]
+    ThreadsafeBrowser: "ThreadsafeBrowser"
 
     def __init__(
-            self, session: str, user_data_dir='', folderNameToken="", headless=False,
+            self, session: str, user_data_dir='', folderNameToken="",
             catchQR: types.FunctionType = None,
             statusFind: types.FunctionType = None, onLoadingScreen: types.FunctionType = None,
             onStateChange: types.FunctionType = None, waitForLogin: bool = True, logQR: bool = False,
             autoClose: int = 0, *args, **kwargs) -> None:
-        """
 
-        @type session: object
-        """
         self.browserSessionToken = None
         self.waitLoginPromise = None
-        self.Browser = None
         self.client = None
         self.state = "CLOSED"
         self.statusFind_dict = {}
         self.catchQR_dict = {}
         self.session = session
         self.user_data_dir = user_data_dir
         self.folderNameToken = (
@@ -43,48 +37,43 @@
             self.user_data_dir = self.create_user_dir()
             if not self.user_data_dir:
                 raise Exception("- Cant create user_data_dir", user_data_dir)
 
         self.loop = kwargs.get("loop") or asyncio.new_event_loop()
         asyncio.set_event_loop(self.loop)
 
-        self.__catchQR = catchQR if type(catchQR) == types.FunctionType else self.catchQR
-        self.__statusFind = statusFind if type(statusFind) == types.FunctionType else self.statusFind
-        self.__onLoadingScreen = onLoadingScreen if type(
+        self.catchQR = catchQR if type(catchQR) == types.FunctionType else self.catchQR
+        self.statusFind = statusFind if type(statusFind) == types.FunctionType else self.statusFind
+        self.onLoadingScreen = onLoadingScreen if type(
             onLoadingScreen) == types.FunctionType else self.onLoadingScreen
-        self.__onStateChange = onStateChange if type(onStateChange) == types.FunctionType else None
+        self.onStateChange = onStateChange if type(onStateChange) == types.FunctionType else None
         self.logger = Logger
         self.waitForLogin = waitForLogin
         self.logQR = logQR
         self.autoClose = autoClose
-        self.headless = headless
         self.__kwargs = kwargs
 
-    def async_to_sync(self, future):
-        result = self.loop.run_until_complete(future)
-        return result
-
-    async def close(self):
+    def close(self):
         if self.client:
-            await self.client.close()
+            self.client.close()
             self.state = "CLOSED"
 
-    async def _onStateChange(self, state):
-        if type(self.__onStateChange) == types.FunctionType:
-            self.__onStateChange(state)
+    def _onStateChange(self, state):
+        if type(self.onStateChange) == types.FunctionType:
+            self.onStateChange(state)
         self.state = state
-        connected = await self.client.page_evaluate("() => WPP.conn.isRegistered()")
+        connected = self.ThreadsafeBrowser.page_evaluate("() => WPP.conn.isRegistered()")
         if not connected:
             sleep(2)
             if not self.waitLoginPromise:
                 try:
                     self.waitLoginPromise = self.client.waitForLogin
                 finally:
                     self.waitLoginPromise = None
-            await self.waitLoginPromise()
+            self.waitLoginPromise()
 
         if state == "CONNECTED":
             print("Ready ....")
 
         elif state in ["browserClose", 'serverClose']:
             self.state = "CLOSED"
             self.client = None
@@ -101,74 +90,51 @@
 
         # user_dir_temp = user_dir
         # for i in itertools.count(1):
         #     if not os.path.exists(user_dir_temp):
         #         return user_dir_temp
         #     user_dir_temp = f'{user_dir}-{i}'
 
-    @staticmethod
-    def check_profile(path):
-        try:
-            path_old = set()
-            for proc in psutil.process_iter():
-                if "chrome.exe" in proc.name():
-                    cmd = proc.cmdline()
-                    user = list(filter(lambda x: "--user-data-dir" in x, cmd))
-                    if user:
-                        path_old.add(os.path.normpath(user[0].split("=")[-1]))
-                elif "firefox.exe" in proc.name():
-                    cmd = proc.cmdline()
-                    user = list(filter(lambda x: "-profile" in x, cmd))
-                    if user:
-                        path_old.add(os.path.normpath(cmd[cmd.index(user[0]) + 1]))
-
-            if os.path.normpath(path) in path_old:
-                # print(f"- {path} is opened")
-                return True
-        except:
-            traceback.print_exc()
-
-    async def start(self) -> Whatsapp:
+    def start(self) -> "Whatsapp":
         if not self.state or self.state in ["CLOSED"]:
-            await self.create()
+            self.create()
 
         elif self.state in ["CONFLICT", "UNPAIRED", "UNLAUNCHED"]:
             print("client.useHere()")
-            await self.client.useHere()
+            self.client.useHere()
         else:
             print(self.get_state())
 
         return self.client
 
-    async def create(self) -> Whatsapp:
+    def create(self) -> Whatsapp:
         self.state = "STARTING"
-        # mergedOptions = defaultOptions
-        # user_data_dir = r"C:\Users\ammar\Whatsapp Pro\Profile-2-2022-09-21-20-21-23"
+        default = {"channel": "chrome", "no_viewport": True, "bypass_csp": True, "headless": False}
+        for key in default:
+            if key not in self.__kwargs:
+                self.__kwargs[key] = default[key]
+
+        self.ThreadsafeBrowser = ThreadsafeBrowser(
+            browser="chromium", install=False, user_data_dir=self.user_data_dir, **self.__kwargs)
+        self.ThreadsafeBrowser.browser.on("disconnected", lambda: self.statusFind('browserClose', self.session))
+
+        self.client = Whatsapp(self.session, self.ThreadsafeBrowser, logQR=self.logQR,
+                               autoClose=self.autoClose)
+        self.client.catchQR = self.catchQR
+        self.client.statusFind = self.statusFind
+        self.client.onLoadingScreen = self.onLoadingScreen
 
-        if self.check_profile(self.user_data_dir):
-            raise Exception("- Current user_data_dir Is Opened", self.user_data_dir)
-
-        self.Browser = Browser(self.session, self.user_data_dir, headless=self.headless, loop=self.loop)
-        await self.Browser.initBrowser()
-        self.Browser.browser.on("disconnected", lambda: self.statusFind('browserClose', self.session))
-
-        self.client = Whatsapp(self.session, self.Browser, loop=self.loop, logQR=self.logQR, autoClose=self.autoClose)
-        self.client.catchQR = self.__catchQR
-        self.client.statusFind = self.__statusFind
-        self.client.onLoadingScreen = self.__onLoadingScreen
-
-        if not await self.client.start():
-            raise Exception("cat start client")
+        self.client.start()
 
         if self.waitForLogin:
-            is_logged = await self.client.waitForLogin()
+            is_logged = self.client.waitForLogin()
             if not is_logged:
                 raise Exception('Not Logged')
             self.state = "CONNECTED"
-        await self.setup()
+        self.setup()
 
         return self.client
 
     def get_state(self) -> dict:
         return {
             "session_name": self.session,
             "state": self.state,
@@ -198,13 +164,9 @@
             "session": session
         }
         # print(session, status)
 
     def onLoadingScreen(self, percent, message):
         print("onLoadingScreen", percent, message)
 
-    async def setup(self):
+    def setup(self):
         self.client.onStateChange(self._onStateChange)
-        # self.client.onAnyMessage(self.on_any_message)
-
-    def on_any_message(self, message):
-        print("int", message)
```

### Comparing `WPP_Whatsapp-0.0.1/setup.py` & `WPP_Whatsapp-0.1.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,43 +1,41 @@
 from setuptools import find_packages
 from setuptools import setup
 
 long_description = open("README.md", encoding="utf-8").read()
 description = "WPP_Whatsapp aim of exporting functions from WhatsApp Web to the python, which can be used to support the creation of any interaction, such as customer service, media sending, intelligence recognition based on phrases artificial and many other things, use your imagination"
 
-version = "0.0.1"
+version = "0.1.0"
 
 setup(
     name="WPP_Whatsapp",
     version=version,
-    license="MIT License",
+    # license="MIT License",
     author="Ammar Alkotb",
     author_email="ammar.alkotb@gmail.com",
     description=description,
     packages=find_packages("WPP_Whatsapp"),
     package_dir={"": "WPP_Whatsapp"},
     url="https://github.com/3mora2/WPP_Whatsapp",
     project_urls={"Bug Report": "https://github.com/3mora2/WPP_Whatsapp/issues/new"},
     install_requires=[
         "event-emitter-js",
         "greenlet",
         "playwright",
         "Pillow",
         "psutil",
-        "pye",
         "pyee",
-        'PyQRCode',
+        'segno',
         'typing_extensions',
+        "playwright-stealth"
     ],
     long_description=long_description,
     long_description_content_type="text/markdown",
     py_modules=["WPP_Whatsapp"],
     classifiers=[
         # "License :: OSI Approved :: MIT License",
         "Intended Audience :: Developers",
+        "Programming Language :: Python",
         "Topic :: Software Development :: Libraries :: Python Modules",
-        "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9",
-        "Programming Language :: Python :: 3.10",
-        "Programming Language :: Python :: 3.11",
+
     ],
 )
```

