# Comparing `tmp/dariusVision-0.0.6.tar.gz` & `tmp/dariusVision-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dariusVision-0.0.6.tar", last modified: Mon Jun 26 12:20:02 2023, max compression
+gzip compressed data, was "dariusVision-0.0.7.tar", last modified: Sun Jul  2 11:48:07 2023, max compression
```

## Comparing `dariusVision-0.0.6.tar` & `dariusVision-0.0.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-26 12:20:02.822504 dariusVision-0.0.6/
--rw-rw-rw-   0        0        0    35823 2023-06-26 09:14:06.000000 dariusVision-0.0.6/LICENSE
--rw-rw-rw-   0        0        0      459 2023-06-26 12:20:02.820508 dariusVision-0.0.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-26 12:20:02.808540 dariusVision-0.0.6/dariusVision/
--rw-rw-rw-   0        0        0      442 2023-06-26 09:19:19.000000 dariusVision-0.0.6/dariusVision/__init__.py
--rw-rw-rw-   0        0        0     3437 2023-06-26 09:14:06.000000 dariusVision-0.0.6/dariusVision/cam.py
--rw-rw-rw-   0        0        0    10808 2023-06-26 11:47:43.000000 dariusVision-0.0.6/dariusVision/realsense2.py
--rw-rw-rw-   0        0        0     2078 2023-06-26 09:14:06.000000 dariusVision-0.0.6/dariusVision/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-26 12:20:02.819522 dariusVision-0.0.6/dariusVision.egg-info/
--rw-rw-rw-   0        0        0      459 2023-06-26 12:20:02.000000 dariusVision-0.0.6/dariusVision.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      289 2023-06-26 12:20:02.000000 dariusVision-0.0.6/dariusVision.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-26 12:20:02.000000 dariusVision-0.0.6/dariusVision.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2023-06-26 12:20:02.000000 dariusVision-0.0.6/dariusVision.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-06-26 12:20:02.000000 dariusVision-0.0.6/dariusVision.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-26 12:20:02.822504 dariusVision-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      666 2023-06-26 12:19:46.000000 dariusVision-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-02 11:48:07.823038 dariusVision-0.0.7/
+-rw-rw-rw-   0        0        0    35823 2023-06-26 09:14:06.000000 dariusVision-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0      812 2023-07-02 11:48:07.822040 dariusVision-0.0.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-02 11:48:07.804088 dariusVision-0.0.7/dariusVision/
+-rw-rw-rw-   0        0        0      442 2023-07-02 11:39:02.000000 dariusVision-0.0.7/dariusVision/__init__.py
+-rw-rw-rw-   0        0        0     3437 2023-06-26 09:14:06.000000 dariusVision-0.0.7/dariusVision/cam.py
+-rw-rw-rw-   0        0        0    10808 2023-06-26 11:47:43.000000 dariusVision-0.0.7/dariusVision/realsense2.py
+-rw-rw-rw-   0        0        0     2078 2023-06-26 09:14:06.000000 dariusVision-0.0.7/dariusVision/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-02 11:48:07.819050 dariusVision-0.0.7/dariusVision.egg-info/
+-rw-rw-rw-   0        0        0      812 2023-07-02 11:48:07.000000 dariusVision-0.0.7/dariusVision.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      289 2023-07-02 11:48:07.000000 dariusVision-0.0.7/dariusVision.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-02 11:48:07.000000 dariusVision-0.0.7/dariusVision.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-07-02 11:48:07.000000 dariusVision-0.0.7/dariusVision.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-02 11:48:07.000000 dariusVision-0.0.7/dariusVision.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-02 11:48:07.824035 dariusVision-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1023 2023-07-02 11:45:03.000000 dariusVision-0.0.7/setup.py
```

### Comparing `dariusVision-0.0.6/LICENSE` & `dariusVision-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `dariusVision-0.0.6/dariusVision/cam.py` & `dariusVision-0.0.7/dariusVision/cam.py`

 * *Files identical despite different names*

### Comparing `dariusVision-0.0.6/dariusVision/realsense2.py` & `dariusVision-0.0.7/dariusVision/realsense2.py`

 * *Files identical despite different names*

### Comparing `dariusVision-0.0.6/dariusVision/utils.py` & `dariusVision-0.0.7/dariusVision/utils.py`

 * *Files identical despite different names*

