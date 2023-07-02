# Comparing `tmp/work_login_lib-0.0.1.tar.gz` & `tmp/work_login_lib-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "work_login_lib-0.0.1.tar", last modified: Sun Jul  2 14:40:54 2023, max compression
+gzip compressed data, was "work_login_lib-0.0.2.tar", last modified: Sun Jul  2 14:50:00 2023, max compression
```

## Comparing `work_login_lib-0.0.1.tar` & `work_login_lib-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 hacky     (1000) hacky     (1000)        0 2023-07-02 14:40:54.870471 work_login_lib-0.0.1/
--rw-rw-r--   0 hacky     (1000) hacky     (1000)      208 2023-07-02 14:40:54.870471 work_login_lib-0.0.1/PKG-INFO
--rw-rw-r--   0 hacky     (1000) hacky     (1000)       38 2023-07-02 14:40:54.870471 work_login_lib-0.0.1/setup.cfg
--rw-rw-r--   0 hacky     (1000) hacky     (1000)      445 2023-07-02 14:34:15.000000 work_login_lib-0.0.1/setup.py
-drwxrwxr-x   0 hacky     (1000) hacky     (1000)        0 2023-07-02 14:40:54.866471 work_login_lib-0.0.1/work_login_lib/
--rw-rw-r--   0 hacky     (1000) hacky     (1000)       31 2023-06-29 14:19:50.000000 work_login_lib-0.0.1/work_login_lib/__init__.py
--rw-rw-r--   0 hacky     (1000) hacky     (1000)      121 2023-07-02 14:37:35.000000 work_login_lib-0.0.1/work_login_lib/__main__.py
-drwxrwxr-x   0 hacky     (1000) hacky     (1000)        0 2023-07-02 14:40:54.870471 work_login_lib-0.0.1/work_login_lib/sub_dir/
--rw-rw-r--   0 hacky     (1000) hacky     (1000)       34 2023-06-29 14:20:31.000000 work_login_lib-0.0.1/work_login_lib/sub_dir/__init__.py
--rwxrwxr-x   0 hacky     (1000) hacky     (1000)     1978 2023-06-29 14:01:01.000000 work_login_lib-0.0.1/work_login_lib/sub_dir/work_login.py
-drwxrwxr-x   0 hacky     (1000) hacky     (1000)        0 2023-07-02 14:40:54.870471 work_login_lib-0.0.1/work_login_lib.egg-info/
--rw-rw-r--   0 hacky     (1000) hacky     (1000)      208 2023-07-02 14:40:54.000000 work_login_lib-0.0.1/work_login_lib.egg-info/PKG-INFO
--rw-rw-r--   0 hacky     (1000) hacky     (1000)      364 2023-07-02 14:40:54.000000 work_login_lib-0.0.1/work_login_lib.egg-info/SOURCES.txt
--rw-rw-r--   0 hacky     (1000) hacky     (1000)        1 2023-07-02 14:40:54.000000 work_login_lib-0.0.1/work_login_lib.egg-info/dependency_links.txt
--rw-rw-r--   0 hacky     (1000) hacky     (1000)       53 2023-07-02 14:40:54.000000 work_login_lib-0.0.1/work_login_lib.egg-info/entry_points.txt
--rw-rw-r--   0 hacky     (1000) hacky     (1000)       21 2023-07-02 14:40:54.000000 work_login_lib-0.0.1/work_login_lib.egg-info/requires.txt
--rw-rw-r--   0 hacky     (1000) hacky     (1000)       15 2023-07-02 14:40:54.000000 work_login_lib-0.0.1/work_login_lib.egg-info/top_level.txt
+drwxrwxr-x   0 hacky     (1000) hacky     (1000)        0 2023-07-02 14:50:00.076743 work_login_lib-0.0.2/
+-rw-rw-r--   0 hacky     (1000) hacky     (1000)      208 2023-07-02 14:50:00.076743 work_login_lib-0.0.2/PKG-INFO
+-rw-rw-r--   0 hacky     (1000) hacky     (1000)       38 2023-07-02 14:50:00.076743 work_login_lib-0.0.2/setup.cfg
+-rw-rw-r--   0 hacky     (1000) hacky     (1000)      445 2023-07-02 14:49:19.000000 work_login_lib-0.0.2/setup.py
+drwxrwxr-x   0 hacky     (1000) hacky     (1000)        0 2023-07-02 14:50:00.072745 work_login_lib-0.0.2/work_login_lib/
+-rw-rw-r--   0 hacky     (1000) hacky     (1000)       31 2023-06-29 14:19:50.000000 work_login_lib-0.0.2/work_login_lib/__init__.py
+-rw-rw-r--   0 hacky     (1000) hacky     (1000)      121 2023-07-02 14:47:54.000000 work_login_lib-0.0.2/work_login_lib/__main__.py
+drwxrwxr-x   0 hacky     (1000) hacky     (1000)        0 2023-07-02 14:50:00.076743 work_login_lib-0.0.2/work_login_lib/sub_dir/
+-rw-rw-r--   0 hacky     (1000) hacky     (1000)       34 2023-06-29 14:20:31.000000 work_login_lib-0.0.2/work_login_lib/sub_dir/__init__.py
+-rwxrwxr-x   0 hacky     (1000) hacky     (1000)     1978 2023-06-29 14:01:01.000000 work_login_lib-0.0.2/work_login_lib/sub_dir/work_login.py
+drwxrwxr-x   0 hacky     (1000) hacky     (1000)        0 2023-07-02 14:50:00.076743 work_login_lib-0.0.2/work_login_lib.egg-info/
+-rw-rw-r--   0 hacky     (1000) hacky     (1000)      208 2023-07-02 14:50:00.000000 work_login_lib-0.0.2/work_login_lib.egg-info/PKG-INFO
+-rw-rw-r--   0 hacky     (1000) hacky     (1000)      364 2023-07-02 14:50:00.000000 work_login_lib-0.0.2/work_login_lib.egg-info/SOURCES.txt
+-rw-rw-r--   0 hacky     (1000) hacky     (1000)        1 2023-07-02 14:50:00.000000 work_login_lib-0.0.2/work_login_lib.egg-info/dependency_links.txt
+-rw-rw-r--   0 hacky     (1000) hacky     (1000)       53 2023-07-02 14:50:00.000000 work_login_lib-0.0.2/work_login_lib.egg-info/entry_points.txt
+-rw-rw-r--   0 hacky     (1000) hacky     (1000)       21 2023-07-02 14:50:00.000000 work_login_lib-0.0.2/work_login_lib.egg-info/requires.txt
+-rw-rw-r--   0 hacky     (1000) hacky     (1000)       15 2023-07-02 14:50:00.000000 work_login_lib-0.0.2/work_login_lib.egg-info/top_level.txt
```

### Comparing `work_login_lib-0.0.1/work_login_lib/sub_dir/work_login.py` & `work_login_lib-0.0.2/work_login_lib/sub_dir/work_login.py`

 * *Files identical despite different names*

