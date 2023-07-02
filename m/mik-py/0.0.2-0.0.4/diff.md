# Comparing `tmp/mik_py-0.0.2.tar.gz` & `tmp/mik_py-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mik_py-0.0.2.tar", last modified: Thu Jun 29 12:56:08 2023, max compression
+gzip compressed data, was "mik_py-0.0.4.tar", last modified: Sun Jul  2 11:21:48 2023, max compression
```

## Comparing `mik_py-0.0.2.tar` & `mik_py-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,15 @@
-drwxr-xr-x   0 michaelchung   (501) staff       (20)        0 2023-06-29 12:56:08.581893 mik_py-0.0.2/
--rw-r--r--   0 michaelchung   (501) staff       (20)       67 2023-03-23 23:33:28.000000 mik_py-0.0.2/MANIFEST.in
--rw-r--r--   0 michaelchung   (501) staff       (20)      554 2023-06-29 12:56:08.581433 mik_py-0.0.2/PKG-INFO
--rw-r--r--   0 michaelchung   (501) staff       (20)      169 2023-06-29 12:54:22.000000 mik_py-0.0.2/README.md
--rw-r--r--   0 michaelchung   (501) staff       (20)       68 2023-03-21 13:16:23.000000 mik_py-0.0.2/eicar.com
-drwxr-xr-x   0 michaelchung   (501) staff       (20)        0 2023-06-29 12:56:08.578273 mik_py-0.0.2/eicar_pack_10/
--rw-r--r--   0 michaelchung   (501) staff       (20)       34 2023-03-26 21:01:11.000000 mik_py-0.0.2/eicar_pack_10/__init__.py
--rw-r--r--   0 michaelchung   (501) staff       (20)      680 2023-03-26 21:01:11.000000 mik_py-0.0.2/eicar_pack_10/eic_py_.py
--rw-r--r--   0 michaelchung   (501) staff       (20)       68 2023-03-21 13:16:23.000000 mik_py-0.0.2/eicar_pack_10/eicar.com
-drwxr-xr-x   0 michaelchung   (501) staff       (20)        0 2023-06-29 12:56:08.580734 mik_py-0.0.2/mik_py.egg-info/
--rw-r--r--   0 michaelchung   (501) staff       (20)      554 2023-06-29 12:56:08.000000 mik_py-0.0.2/mik_py.egg-info/PKG-INFO
--rw-r--r--   0 michaelchung   (501) staff       (20)      235 2023-06-29 12:56:08.000000 mik_py-0.0.2/mik_py.egg-info/SOURCES.txt
--rw-r--r--   0 michaelchung   (501) staff       (20)        1 2023-06-29 12:56:08.000000 mik_py-0.0.2/mik_py.egg-info/dependency_links.txt
--rw-r--r--   0 michaelchung   (501) staff       (20)       14 2023-06-29 12:56:08.000000 mik_py-0.0.2/mik_py.egg-info/top_level.txt
--rw-r--r--   0 michaelchung   (501) staff       (20)       38 2023-06-29 12:56:08.582054 mik_py-0.0.2/setup.cfg
--rw-r--r--   0 michaelchung   (501) staff       (20)      970 2023-06-29 12:55:34.000000 mik_py-0.0.2/setup.py
+drwxr-xr-x   0 michaelchung   (501) staff       (20)        0 2023-07-02 11:21:48.136931 mik_py-0.0.4/
+-rw-r--r--   0 michaelchung   (501) staff       (20)       67 2023-03-23 23:33:28.000000 mik_py-0.0.4/MANIFEST.in
+-rw-r--r--   0 michaelchung   (501) staff       (20)      975 2023-07-02 11:21:48.136600 mik_py-0.0.4/PKG-INFO
+-rw-r--r--   0 michaelchung   (501) staff       (20)      566 2023-07-02 11:07:52.000000 mik_py-0.0.4/README.md
+-rw-r--r--   0 michaelchung   (501) staff       (20)       68 2023-03-21 13:16:23.000000 mik_py-0.0.4/eicar.com
+drwxr-xr-x   0 michaelchung   (501) staff       (20)        0 2023-07-02 11:21:48.133637 mik_py-0.0.4/mik_pack_10/
+-rw-r--r--   0 michaelchung   (501) staff       (20)       34 2023-03-26 21:06:06.000000 mik_py-0.0.4/mik_pack_10/__init__.py
+-rw-r--r--   0 michaelchung   (501) staff       (20)      680 2023-03-26 21:01:11.000000 mik_py-0.0.4/mik_pack_10/mik_py_.py
+drwxr-xr-x   0 michaelchung   (501) staff       (20)        0 2023-07-02 11:21:48.136174 mik_py-0.0.4/mik_py.egg-info/
+-rw-r--r--   0 michaelchung   (501) staff       (20)      975 2023-07-02 11:21:47.000000 mik_py-0.0.4/mik_py.egg-info/PKG-INFO
+-rw-r--r--   0 michaelchung   (501) staff       (20)      207 2023-07-02 11:21:48.000000 mik_py-0.0.4/mik_py.egg-info/SOURCES.txt
+-rw-r--r--   0 michaelchung   (501) staff       (20)        1 2023-07-02 11:21:47.000000 mik_py-0.0.4/mik_py.egg-info/dependency_links.txt
+-rw-r--r--   0 michaelchung   (501) staff       (20)       12 2023-07-02 11:21:47.000000 mik_py-0.0.4/mik_py.egg-info/top_level.txt
+-rw-r--r--   0 michaelchung   (501) staff       (20)       38 2023-07-02 11:21:48.137034 mik_py-0.0.4/setup.cfg
+-rw-r--r--   0 michaelchung   (501) staff       (20)     1415 2023-07-02 11:21:38.000000 mik_py-0.0.4/setup.py
```

### Comparing `mik_py-0.0.2/eicar_pack_10/eic_py_.py` & `mik_py-0.0.4/mik_pack_10/mik_py_.py`

 * *Files identical despite different names*

