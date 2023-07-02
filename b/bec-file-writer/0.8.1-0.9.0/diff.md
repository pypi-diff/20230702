# Comparing `tmp/bec_file_writer-0.8.1.tar.gz` & `tmp/bec_file_writer-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bec_file_writer-0.8.1.tar", last modified: Sun Jul  2 18:15:29 2023, max compression
+gzip compressed data, was "bec_file_writer-0.9.0.tar", last modified: Sun Jul  2 18:59:03 2023, max compression
```

## Comparing `bec_file_writer-0.8.1.tar` & `bec_file_writer-0.9.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 18:15:29.126586 bec_file_writer-0.8.1/
--rw-r--r--   0 root         (0) root         (0)      455 2023-07-02 18:15:29.126586 bec_file_writer-0.8.1/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 18:15:29.126586 bec_file_writer-0.8.1/bec_file_writer.egg-info/
--rw-r--r--   0 root         (0) root         (0)      455 2023-07-02 18:15:29.000000 bec_file_writer-0.8.1/bec_file_writer.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      439 2023-07-02 18:15:29.000000 bec_file_writer-0.8.1/bec_file_writer.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-02 18:15:29.000000 bec_file_writer-0.8.1/bec_file_writer.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       28 2023-07-02 18:15:29.000000 bec_file_writer-0.8.1/bec_file_writer.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       32 2023-07-02 18:15:29.000000 bec_file_writer-0.8.1/bec_file_writer.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 18:15:29.124586 bec_file_writer-0.8.1/file_writer/
--rw-rw-rw-   0 root         (0) root         (0)      112 2023-04-24 15:23:42.000000 bec_file_writer-0.8.1/file_writer/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9251 2023-06-28 10:41:58.000000 bec_file_writer-0.8.1/file_writer/file_writer.py
--rw-r--r--   0 root         (0) root         (0)     8083 2023-06-28 10:41:58.000000 bec_file_writer-0.8.1/file_writer/file_writer_manager.py
--rw-rw-rw-   0 root         (0) root         (0)     1555 2023-06-19 08:14:59.000000 bec_file_writer-0.8.1/file_writer/merged_dicts.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 18:15:29.124586 bec_file_writer-0.8.1/file_writer_plugins/
--rw-rw-rw-   0 root         (0) root         (0)      119 2023-06-19 08:14:59.000000 bec_file_writer-0.8.1/file_writer_plugins/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17058 2023-06-25 18:29:43.000000 bec_file_writer-0.8.1/file_writer_plugins/cSAXS.py
--rw-r--r--   0 root         (0) root         (0)     2274 2023-06-25 18:29:43.000000 bec_file_writer-0.8.1/file_writer_plugins/default_writer.py
--rw-r--r--   0 root         (0) root         (0)      536 2023-07-02 18:15:29.127586 bec_file_writer-0.8.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      731 2023-06-28 14:27:03.000000 bec_file_writer-0.8.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 18:59:03.504611 bec_file_writer-0.9.0/
+-rw-r--r--   0 root         (0) root         (0)      455 2023-07-02 18:59:03.504611 bec_file_writer-0.9.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 18:59:03.504611 bec_file_writer-0.9.0/bec_file_writer.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      455 2023-07-02 18:59:03.000000 bec_file_writer-0.9.0/bec_file_writer.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      439 2023-07-02 18:59:03.000000 bec_file_writer-0.9.0/bec_file_writer.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-02 18:59:03.000000 bec_file_writer-0.9.0/bec_file_writer.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       28 2023-07-02 18:59:03.000000 bec_file_writer-0.9.0/bec_file_writer.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       32 2023-07-02 18:59:03.000000 bec_file_writer-0.9.0/bec_file_writer.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 18:59:03.502611 bec_file_writer-0.9.0/file_writer/
+-rw-rw-rw-   0 root         (0) root         (0)      112 2023-04-24 15:23:42.000000 bec_file_writer-0.9.0/file_writer/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9251 2023-06-28 10:41:58.000000 bec_file_writer-0.9.0/file_writer/file_writer.py
+-rw-r--r--   0 root         (0) root         (0)     8083 2023-06-28 10:41:58.000000 bec_file_writer-0.9.0/file_writer/file_writer_manager.py
+-rw-rw-rw-   0 root         (0) root         (0)     1555 2023-06-19 08:14:59.000000 bec_file_writer-0.9.0/file_writer/merged_dicts.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 18:59:03.503611 bec_file_writer-0.9.0/file_writer_plugins/
+-rw-rw-rw-   0 root         (0) root         (0)      119 2023-06-19 08:14:59.000000 bec_file_writer-0.9.0/file_writer_plugins/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17058 2023-06-25 18:29:43.000000 bec_file_writer-0.9.0/file_writer_plugins/cSAXS.py
+-rw-r--r--   0 root         (0) root         (0)     2274 2023-06-25 18:29:43.000000 bec_file_writer-0.9.0/file_writer_plugins/default_writer.py
+-rw-r--r--   0 root         (0) root         (0)      536 2023-07-02 18:59:03.505611 bec_file_writer-0.9.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      731 2023-06-28 14:27:03.000000 bec_file_writer-0.9.0/setup.py
```

### Comparing `bec_file_writer-0.8.1/file_writer/file_writer.py` & `bec_file_writer-0.9.0/file_writer/file_writer.py`

 * *Files identical despite different names*

### Comparing `bec_file_writer-0.8.1/file_writer/file_writer_manager.py` & `bec_file_writer-0.9.0/file_writer/file_writer_manager.py`

 * *Files identical despite different names*

### Comparing `bec_file_writer-0.8.1/file_writer/merged_dicts.py` & `bec_file_writer-0.9.0/file_writer/merged_dicts.py`

 * *Files identical despite different names*

### Comparing `bec_file_writer-0.8.1/file_writer_plugins/cSAXS.py` & `bec_file_writer-0.9.0/file_writer_plugins/cSAXS.py`

 * *Files identical despite different names*

### Comparing `bec_file_writer-0.8.1/file_writer_plugins/default_writer.py` & `bec_file_writer-0.9.0/file_writer_plugins/default_writer.py`

 * *Files identical despite different names*

### Comparing `bec_file_writer-0.8.1/setup.cfg` & `bec_file_writer-0.9.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `bec_file_writer-0.8.1/setup.py` & `bec_file_writer-0.9.0/setup.py`

 * *Files identical despite different names*

