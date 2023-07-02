# Comparing `tmp/bec_dap-0.8.0.tar.gz` & `tmp/bec_dap-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bec_dap-0.8.0.tar", last modified: Wed Jun 28 15:24:13 2023, max compression
+gzip compressed data, was "bec_dap-0.8.1.tar", last modified: Sun Jul  2 18:15:31 2023, max compression
```

## Comparing `bec_dap-0.8.0.tar` & `bec_dap-0.8.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 15:24:13.849405 bec_dap-0.8.0/
--rw-r--r--   0 root         (0) root         (0)      440 2023-06-28 15:24:13.849405 bec_dap-0.8.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 15:24:13.849405 bec_dap-0.8.0/bec_dap.egg-info/
--rw-r--r--   0 root         (0) root         (0)      440 2023-06-28 15:24:13.000000 bec_dap-0.8.0/bec_dap.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      308 2023-06-28 15:24:13.000000 bec_dap-0.8.0/bec_dap.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-28 15:24:13.000000 bec_dap-0.8.0/bec_dap.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-06-28 15:24:13.000000 bec_dap-0.8.0/bec_dap.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-06-28 15:24:13.000000 bec_dap-0.8.0/bec_dap.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 15:24:13.847405 bec_dap-0.8.0/data_processing/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 18:43:13.000000 bec_dap-0.8.0/data_processing/__init__.py
--rw-r--r--   0 root         (0) root         (0)      689 2023-06-28 10:41:58.000000 bec_dap-0.8.0/data_processing/dap_server.py
--rw-r--r--   0 root         (0) root         (0)     8024 2023-06-28 10:41:58.000000 bec_dap-0.8.0/data_processing/stream_processor.py
--rw-r--r--   0 root         (0) root         (0)     3508 2023-06-28 10:41:58.000000 bec_dap-0.8.0/data_processing/worker_manager.py
--rw-r--r--   0 root         (0) root         (0)      521 2023-06-28 15:24:13.850405 bec_dap-0.8.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      699 2023-06-28 10:41:58.000000 bec_dap-0.8.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 18:15:31.765506 bec_dap-0.8.1/
+-rw-r--r--   0 root         (0) root         (0)      440 2023-07-02 18:15:31.765506 bec_dap-0.8.1/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 18:15:31.764506 bec_dap-0.8.1/bec_dap.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      440 2023-07-02 18:15:31.000000 bec_dap-0.8.1/bec_dap.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      308 2023-07-02 18:15:31.000000 bec_dap-0.8.1/bec_dap.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-02 18:15:31.000000 bec_dap-0.8.1/bec_dap.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-07-02 18:15:31.000000 bec_dap-0.8.1/bec_dap.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-07-02 18:15:31.000000 bec_dap-0.8.1/bec_dap.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 18:15:31.763506 bec_dap-0.8.1/data_processing/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 18:43:13.000000 bec_dap-0.8.1/data_processing/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      689 2023-06-28 10:41:58.000000 bec_dap-0.8.1/data_processing/dap_server.py
+-rw-r--r--   0 root         (0) root         (0)     8024 2023-06-28 10:41:58.000000 bec_dap-0.8.1/data_processing/stream_processor.py
+-rw-r--r--   0 root         (0) root         (0)     3508 2023-06-28 10:41:58.000000 bec_dap-0.8.1/data_processing/worker_manager.py
+-rw-r--r--   0 root         (0) root         (0)      521 2023-07-02 18:15:31.765506 bec_dap-0.8.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      699 2023-06-28 10:41:58.000000 bec_dap-0.8.1/setup.py
```

### Comparing `bec_dap-0.8.0/data_processing/dap_server.py` & `bec_dap-0.8.1/data_processing/dap_server.py`

 * *Files identical despite different names*

### Comparing `bec_dap-0.8.0/data_processing/stream_processor.py` & `bec_dap-0.8.1/data_processing/stream_processor.py`

 * *Files identical despite different names*

### Comparing `bec_dap-0.8.0/data_processing/worker_manager.py` & `bec_dap-0.8.1/data_processing/worker_manager.py`

 * *Files identical despite different names*

### Comparing `bec_dap-0.8.0/setup.cfg` & `bec_dap-0.8.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `bec_dap-0.8.0/setup.py` & `bec_dap-0.8.1/setup.py`

 * *Files identical despite different names*

