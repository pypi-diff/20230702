# Comparing `tmp/ra2mix-0.0.3.tar.gz` & `tmp/ra2mix-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ra2mix-0.0.3.tar", last modified: Sun Jul  2 04:26:25 2023, max compression
+gzip compressed data, was "ra2mix-0.0.4.tar", last modified: Sun Jul  2 04:31:38 2023, max compression
```

## Comparing `ra2mix-0.0.3.tar` & `ra2mix-0.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 04:26:25.111780 ra2mix-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-02 04:26:16.000000 ra2mix-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-07-02 04:26:25.111780 ra2mix-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-02 04:26:16.000000 ra2mix-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-02 04:26:16.000000 ra2mix-0.0.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 04:26:25.111780 ra2mix-0.0.3/ra2mix/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-02 04:26:16.000000 ra2mix-0.0.3/ra2mix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-07-02 04:26:16.000000 ra2mix-0.0.3/ra2mix/checksum.py
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-02 04:26:16.000000 ra2mix-0.0.3/ra2mix/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-07-02 04:26:16.000000 ra2mix-0.0.3/ra2mix/reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-07-02 04:26:16.000000 ra2mix-0.0.3/ra2mix/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 04:26:25.111780 ra2mix-0.0.3/ra2mix.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-07-02 04:26:25.000000 ra2mix-0.0.3/ra2mix.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-02 04:26:25.000000 ra2mix-0.0.3/ra2mix.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 04:26:25.000000 ra2mix-0.0.3/ra2mix.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-02 04:26:25.000000 ra2mix-0.0.3/ra2mix.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-02 04:26:25.000000 ra2mix-0.0.3/ra2mix.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 04:26:25.111780 ra2mix-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 04:31:38.590053 ra2mix-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-02 04:31:29.000000 ra2mix-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-07-02 04:31:38.590053 ra2mix-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-02 04:31:29.000000 ra2mix-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-02 04:31:29.000000 ra2mix-0.0.4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 04:31:38.590053 ra2mix-0.0.4/ra2mix/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-02 04:31:29.000000 ra2mix-0.0.4/ra2mix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-07-02 04:31:29.000000 ra2mix-0.0.4/ra2mix/checksum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-02 04:31:29.000000 ra2mix-0.0.4/ra2mix/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-07-02 04:31:29.000000 ra2mix-0.0.4/ra2mix/reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-07-02 04:31:29.000000 ra2mix-0.0.4/ra2mix/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 04:31:38.590053 ra2mix-0.0.4/ra2mix.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-07-02 04:31:38.000000 ra2mix-0.0.4/ra2mix.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-02 04:31:38.000000 ra2mix-0.0.4/ra2mix.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 04:31:38.000000 ra2mix-0.0.4/ra2mix.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-02 04:31:38.000000 ra2mix-0.0.4/ra2mix.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-02 04:31:38.000000 ra2mix-0.0.4/ra2mix.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 04:31:38.590053 ra2mix-0.0.4/setup.cfg
```

### Comparing `ra2mix-0.0.3/LICENSE` & `ra2mix-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ra2mix-0.0.3/PKG-INFO` & `ra2mix-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ra2mix
-Version: 0.0.3
+Version: 0.0.4
 Summary: ra2mix is a python library for working with Red Alert 2 / Yuri's Revenge *.mix files
 Author-email: nyte_owl <nyteowldev@gmail.com>
 Project-URL: Homepage, https://github.com/endless-creation/ra2mix
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
```

### Comparing `ra2mix-0.0.3/pyproject.toml` & `ra2mix-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 name = "ra2mix"
 authors = [
     {name = "nyte_owl", email = "nyteowldev@gmail.com"}
 ]
 description = "ra2mix is a python library for working with Red Alert 2 / Yuri's Revenge *.mix files"
 readme = "README.md"
 requires-python = ">=3.11"
-version = "0.0.3"
+version = "0.0.4"
 dependencies = [
     "crc"
 ]
 classifiers = [
     "Programming Language :: Python :: 3.11",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: OS Independent",
```

### Comparing `ra2mix-0.0.3/ra2mix/checksum.py` & `ra2mix-0.0.4/ra2mix/checksum.py`

 * *Files identical despite different names*

### Comparing `ra2mix-0.0.3/ra2mix/const.py` & `ra2mix-0.0.4/ra2mix/const.py`

 * *Files identical despite different names*

### Comparing `ra2mix-0.0.3/ra2mix/reader.py` & `ra2mix-0.0.4/ra2mix/reader.py`

 * *Files identical despite different names*

### Comparing `ra2mix-0.0.3/ra2mix/writer.py` & `ra2mix-0.0.4/ra2mix/writer.py`

 * *Files identical despite different names*

### Comparing `ra2mix-0.0.3/ra2mix.egg-info/PKG-INFO` & `ra2mix-0.0.4/ra2mix.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ra2mix
-Version: 0.0.3
+Version: 0.0.4
 Summary: ra2mix is a python library for working with Red Alert 2 / Yuri's Revenge *.mix files
 Author-email: nyte_owl <nyteowldev@gmail.com>
 Project-URL: Homepage, https://github.com/endless-creation/ra2mix
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
```

