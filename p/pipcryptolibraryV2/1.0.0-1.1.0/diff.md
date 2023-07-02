# Comparing `tmp/pipcryptolibraryV2-1.0.0.tar.gz` & `tmp/pipcryptolibraryV2-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipcryptolibraryV2-1.0.0.tar", last modified: Sun Jul  2 21:37:34 2023, max compression
+gzip compressed data, was "pipcryptolibraryV2-1.1.0.tar", last modified: Sun Jul  2 21:39:40 2023, max compression
```

## Comparing `pipcryptolibraryV2-1.0.0.tar` & `pipcryptolibraryV2-1.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 21:37:34.948714 pipcryptolibraryV2-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      351 2023-07-02 21:37:34.948714 pipcryptolibraryV2-1.0.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 21:37:34.944714 pipcryptolibraryV2-1.0.0/pipcryptolibraryV2/
--rw-r--r--   0 root         (0) root         (0)       21 2023-07-02 21:37:34.000000 pipcryptolibraryV2-1.0.0/pipcryptolibraryV2/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 21:37:34.948714 pipcryptolibraryV2-1.0.0/pipcryptolibraryV2.egg-info/
--rw-r--r--   0 root         (0) root         (0)      351 2023-07-02 21:37:34.000000 pipcryptolibraryV2-1.0.0/pipcryptolibraryV2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      207 2023-07-02 21:37:34.000000 pipcryptolibraryV2-1.0.0/pipcryptolibraryV2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-02 21:37:34.000000 pipcryptolibraryV2-1.0.0/pipcryptolibraryV2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-07-02 21:37:34.000000 pipcryptolibraryV2-1.0.0/pipcryptolibraryV2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-02 21:37:34.948714 pipcryptolibraryV2-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      564 2023-07-02 21:37:34.000000 pipcryptolibraryV2-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 21:39:40.484394 pipcryptolibraryV2-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)      351 2023-07-02 21:39:40.484394 pipcryptolibraryV2-1.1.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 21:39:40.480394 pipcryptolibraryV2-1.1.0/pipcryptolibraryV2/
+-rw-r--r--   0 root         (0) root         (0)    96763 2023-07-02 21:39:39.000000 pipcryptolibraryV2-1.1.0/pipcryptolibraryV2/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 21:39:40.484394 pipcryptolibraryV2-1.1.0/pipcryptolibraryV2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      351 2023-07-02 21:39:40.000000 pipcryptolibraryV2-1.1.0/pipcryptolibraryV2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      207 2023-07-02 21:39:40.000000 pipcryptolibraryV2-1.1.0/pipcryptolibraryV2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-02 21:39:40.000000 pipcryptolibraryV2-1.1.0/pipcryptolibraryV2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-07-02 21:39:40.000000 pipcryptolibraryV2-1.1.0/pipcryptolibraryV2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-02 21:39:40.484394 pipcryptolibraryV2-1.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      564 2023-07-02 21:39:39.000000 pipcryptolibraryV2-1.1.0/setup.py
```

### Comparing `pipcryptolibraryV2-1.0.0/setup.py` & `pipcryptolibraryV2-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.0.0'
+VERSION = '1.1.0'
 DESCRIPTION = "Usefull utility package"
 LONG_DESCRIPTION = "Usefull utility package"
 
 # Setting up
 setup(
     name="pipcryptolibraryV2",
     version=VERSION,
```

