# Comparing `tmp/sortd-1.2.2.tar.gz` & `tmp/sortd-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sortd-1.2.2.tar", last modified: Sun Jul  2 05:13:00 2023, max compression
+gzip compressed data, was "sortd-1.2.3.tar", last modified: Sun Jul  2 05:15:58 2023, max compression
```

## Comparing `sortd-1.2.2.tar` & `sortd-1.2.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 05:13:00.194594 sortd-1.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-07-02 05:13:00.194594 sortd-1.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-07-02 05:12:49.000000 sortd-1.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-02 05:12:49.000000 sortd-1.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-02 05:13:00.194594 sortd-1.2.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 05:13:00.194594 sortd-1.2.2/sortd/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 05:12:49.000000 sortd-1.2.2/sortd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-07-02 05:12:49.000000 sortd-1.2.2/sortd/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-02 05:12:49.000000 sortd-1.2.2/sortd/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-07-02 05:12:49.000000 sortd-1.2.2/sortd/lib.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 05:12:49.000000 sortd-1.2.2/sortd/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-02 05:12:49.000000 sortd-1.2.2/sortd/s_cfg.py
--rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-07-02 05:12:49.000000 sortd-1.2.2/sortd/s_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-07-02 05:12:49.000000 sortd-1.2.2/sortd/s_json.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-02 05:12:49.000000 sortd-1.2.2/sortd/s_lines.py
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-07-02 05:12:49.000000 sortd-1.2.2/sortd/s_plist.py
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-02 05:12:49.000000 sortd-1.2.2/sortd/s_toml.py
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-07-02 05:12:49.000000 sortd-1.2.2/sortd/s_yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 05:13:00.194594 sortd-1.2.2/sortd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-07-02 05:13:00.000000 sortd-1.2.2/sortd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-07-02 05:13:00.000000 sortd-1.2.2/sortd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 05:13:00.000000 sortd-1.2.2/sortd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-02 05:13:00.000000 sortd-1.2.2/sortd.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-02 05:13:00.000000 sortd-1.2.2/sortd.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-02 05:13:00.000000 sortd-1.2.2/sortd.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 05:15:58.634859 sortd-1.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-07-02 05:15:58.634859 sortd-1.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-07-02 05:15:48.000000 sortd-1.2.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-02 05:15:48.000000 sortd-1.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-02 05:15:58.634859 sortd-1.2.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 05:15:58.634859 sortd-1.2.3/sortd/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 05:15:48.000000 sortd-1.2.3/sortd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-07-02 05:15:48.000000 sortd-1.2.3/sortd/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-02 05:15:48.000000 sortd-1.2.3/sortd/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-07-02 05:15:48.000000 sortd-1.2.3/sortd/lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 05:15:48.000000 sortd-1.2.3/sortd/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-02 05:15:48.000000 sortd-1.2.3/sortd/s_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-07-02 05:15:48.000000 sortd-1.2.3/sortd/s_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-07-02 05:15:48.000000 sortd-1.2.3/sortd/s_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-02 05:15:48.000000 sortd-1.2.3/sortd/s_lines.py
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-07-02 05:15:48.000000 sortd-1.2.3/sortd/s_plist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-02 05:15:48.000000 sortd-1.2.3/sortd/s_toml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-07-02 05:15:48.000000 sortd-1.2.3/sortd/s_yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 05:15:58.634859 sortd-1.2.3/sortd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-07-02 05:15:58.000000 sortd-1.2.3/sortd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-07-02 05:15:58.000000 sortd-1.2.3/sortd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 05:15:58.000000 sortd-1.2.3/sortd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-02 05:15:58.000000 sortd-1.2.3/sortd.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-02 05:15:58.000000 sortd-1.2.3/sortd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-02 05:15:58.000000 sortd-1.2.3/sortd.egg-info/top_level.txt
```

### Comparing `sortd-1.2.2/PKG-INFO` & `sortd-1.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sortd
-Version: 1.2.2
+Version: 1.2.3
 Summary: sorting commands for stdin -> stdout
 Author-email: ms-jpq <github@bigly.dog>
 Project-URL: homepage, https://github.com/ms-jpq/sortd
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: dist
```

### Comparing `sortd-1.2.2/sortd/__main__.py` & `sortd-1.2.3/sortd/__main__.py`

 * *Files identical despite different names*

### Comparing `sortd-1.2.2/sortd/lib.py` & `sortd-1.2.3/sortd/lib.py`

 * *Files identical despite different names*

### Comparing `sortd-1.2.2/sortd/s_cfg.py` & `sortd-1.2.3/sortd/s_cfg.py`

 * *Files identical despite different names*

### Comparing `sortd-1.2.2/sortd/s_csv.py` & `sortd-1.2.3/sortd/s_csv.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,8 +72,7 @@
             w = writer(stdout, dialect=d)
             w.writerows(r)
     except CSVErr as e:
         log.critical("%s", f"{ERROR}{linesep}{e}")
         return 1
     else:
         return 0
-
```

### Comparing `sortd-1.2.2/sortd/s_yaml.py` & `sortd-1.2.3/sortd/s_yaml.py`

 * *Files identical despite different names*

### Comparing `sortd-1.2.2/sortd.egg-info/PKG-INFO` & `sortd-1.2.3/sortd.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sortd
-Version: 1.2.2
+Version: 1.2.3
 Summary: sorting commands for stdin -> stdout
 Author-email: ms-jpq <github@bigly.dog>
 Project-URL: homepage, https://github.com/ms-jpq/sortd
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: dist
```

