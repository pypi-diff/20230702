# Comparing `tmp/devpi-client-6.0.4.tar.gz` & `tmp/devpi-client-6.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "devpi-client-6.0.4.tar", last modified: Thu Apr 13 05:14:10 2023, max compression
+gzip compressed data, was "devpi-client-6.0.5.tar", last modified: Sun Jul  2 12:04:15 2023, max compression
```

## Comparing `devpi-client-6.0.4.tar` & `devpi-client-6.0.5.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-04-13 05:14:10.172940 devpi-client-6.0.4/
--rw-r--r--   0 fschulze   (501) staff       (20)      192 2023-04-13 05:14:01.000000 devpi-client-6.0.4/AUTHORS
--rw-r--r--   0 fschulze   (501) staff       (20)    26534 2023-04-13 05:14:01.000000 devpi-client-6.0.4/CHANGELOG
--rw-r--r--   0 fschulze   (501) staff       (20)     1061 2023-04-13 05:14:01.000000 devpi-client-6.0.4/LICENSE
--rw-r--r--   0 fschulze   (501) staff       (20)      147 2023-04-13 05:14:01.000000 devpi-client-6.0.4/MANIFEST.in
--rw-r--r--   0 fschulze   (501) staff       (20)     6725 2023-04-13 05:14:10.173057 devpi-client-6.0.4/PKG-INFO
--rw-r--r--   0 fschulze   (501) staff       (20)      930 2023-04-13 05:14:01.000000 devpi-client-6.0.4/README.rst
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-04-13 05:14:10.161411 devpi-client-6.0.4/devpi/
--rw-r--r--   0 fschulze   (501) staff       (20)       23 2023-04-13 05:14:01.000000 devpi-client-6.0.4/devpi/__init__.py
--rw-r--r--   0 fschulze   (501) staff       (20)       70 2023-04-13 05:14:01.000000 devpi-client-6.0.4/devpi/__main__.py
--rw-r--r--   0 fschulze   (501) staff       (20)     1540 2023-04-13 05:14:01.000000 devpi-client-6.0.4/devpi/getjson.py
--rw-r--r--   0 fschulze   (501) staff       (20)      679 2023-04-13 05:14:01.000000 devpi-client-6.0.4/devpi/hookspecs.py
--rw-r--r--   0 fschulze   (501) staff       (20)     3772 2023-04-13 05:14:01.000000 devpi-client-6.0.4/devpi/index.py
--rw-r--r--   0 fschulze   (501) staff       (20)     2177 2023-04-13 05:14:01.000000 devpi-client-6.0.4/devpi/install.py
--rw-r--r--   0 fschulze   (501) staff       (20)     7711 2023-04-13 05:14:01.000000 devpi-client-6.0.4/devpi/list_remove.py
--rw-r--r--   0 fschulze   (501) staff       (20)     1430 2023-04-13 05:14:01.000000 devpi-client-6.0.4/devpi/login.py
--rw-r--r--   0 fschulze   (501) staff       (20)    45869 2023-04-13 05:14:01.000000 devpi-client-6.0.4/devpi/main.py
--rw-r--r--   0 fschulze   (501) staff       (20)     3565 2023-04-13 05:14:01.000000 devpi-client-6.0.4/devpi/push.py
--rw-r--r--   0 fschulze   (501) staff       (20)      536 2023-04-13 05:14:01.000000 devpi-client-6.0.4/devpi/pypirc.py
--rw-r--r--   0 fschulze   (501) staff       (20)      550 2023-04-13 05:14:01.000000 devpi-client-6.0.4/devpi/refresh.py
--rw-r--r--   0 fschulze   (501) staff       (20)     9930 2023-04-13 05:14:01.000000 devpi-client-6.0.4/devpi/test.py
--rw-r--r--   0 fschulze   (501) staff       (20)    20388 2023-04-13 05:14:01.000000 devpi-client-6.0.4/devpi/upload.py
--rw-r--r--   0 fschulze   (501) staff       (20)    28791 2023-04-13 05:14:01.000000 devpi-client-6.0.4/devpi/use.py
--rw-r--r--   0 fschulze   (501) staff       (20)     3290 2023-04-13 05:14:01.000000 devpi-client-6.0.4/devpi/user.py
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-04-13 05:14:10.163096 devpi-client-6.0.4/devpi_client.egg-info/
--rw-r--r--   0 fschulze   (501) staff       (20)     6725 2023-04-13 05:14:10.000000 devpi-client-6.0.4/devpi_client.egg-info/PKG-INFO
--rw-r--r--   0 fschulze   (501) staff       (20)      987 2023-04-13 05:14:10.000000 devpi-client-6.0.4/devpi_client.egg-info/SOURCES.txt
--rw-r--r--   0 fschulze   (501) staff       (20)        1 2023-04-13 05:14:10.000000 devpi-client-6.0.4/devpi_client.egg-info/dependency_links.txt
--rw-r--r--   0 fschulze   (501) staff       (20)      129 2023-04-13 05:14:10.000000 devpi-client-6.0.4/devpi_client.egg-info/entry_points.txt
--rw-r--r--   0 fschulze   (501) staff       (20)      125 2023-04-13 05:14:10.000000 devpi-client-6.0.4/devpi_client.egg-info/requires.txt
--rw-r--r--   0 fschulze   (501) staff       (20)        6 2023-04-13 05:14:10.000000 devpi-client-6.0.4/devpi_client.egg-info/top_level.txt
--rw-r--r--   0 fschulze   (501) staff       (20)      510 2023-04-13 05:14:01.000000 devpi-client-6.0.4/pyproject.toml
--rw-r--r--   0 fschulze   (501) staff       (20)      115 2023-04-13 05:14:10.173506 devpi-client-6.0.4/setup.cfg
--rwxr-xr-x   0 fschulze   (501) staff       (20)     2540 2023-04-13 05:14:01.000000 devpi-client-6.0.4/setup.py
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-04-13 05:14:10.172242 devpi-client-6.0.4/testing/
--rw-r--r--   0 fschulze   (501) staff       (20)        0 2023-04-13 05:14:01.000000 devpi-client-6.0.4/testing/__init__.py
--rw-r--r--   0 fschulze   (501) staff       (20)    25605 2023-04-13 05:14:01.000000 devpi-client-6.0.4/testing/conftest.py
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-04-13 05:14:10.172678 devpi-client-6.0.4/testing/data/
--rw-r--r--   0 fschulze   (501) staff       (20)     1846 2023-04-13 05:14:01.000000 devpi-client-6.0.4/testing/data/dddttt-0.1.dev45-py27-none-any.whl
--rw-r--r--   0 fschulze   (501) staff       (20)    21019 2023-04-13 05:14:01.000000 devpi-client-6.0.4/testing/functional.py
--rw-r--r--   0 fschulze   (501) staff       (20)     3056 2023-04-13 05:14:01.000000 devpi-client-6.0.4/testing/reqmock.py
--rw-r--r--   0 fschulze   (501) staff       (20)     6149 2023-04-13 05:14:01.000000 devpi-client-6.0.4/testing/simpypi.py
--rw-r--r--   0 fschulze   (501) staff       (20)    18203 2023-04-13 05:14:01.000000 devpi-client-6.0.4/testing/test_functional.py
--rw-r--r--   0 fschulze   (501) staff       (20)     4556 2023-04-13 05:14:01.000000 devpi-client-6.0.4/testing/test_index.py
--rw-r--r--   0 fschulze   (501) staff       (20)     4245 2023-04-13 05:14:01.000000 devpi-client-6.0.4/testing/test_install.py
--rw-r--r--   0 fschulze   (501) staff       (20)    13592 2023-04-13 05:14:01.000000 devpi-client-6.0.4/testing/test_list_remove.py
--rw-r--r--   0 fschulze   (501) staff       (20)     3811 2023-04-13 05:14:01.000000 devpi-client-6.0.4/testing/test_login.py
--rw-r--r--   0 fschulze   (501) staff       (20)     7466 2023-04-13 05:14:01.000000 devpi-client-6.0.4/testing/test_main.py
--rw-r--r--   0 fschulze   (501) staff       (20)    10817 2023-04-13 05:14:01.000000 devpi-client-6.0.4/testing/test_push.py
--rw-r--r--   0 fschulze   (501) staff       (20)      979 2023-04-13 05:14:01.000000 devpi-client-6.0.4/testing/test_pypirc.py
--rw-r--r--   0 fschulze   (501) staff       (20)    20033 2023-04-13 05:14:01.000000 devpi-client-6.0.4/testing/test_test.py
--rw-r--r--   0 fschulze   (501) staff       (20)    31200 2023-04-13 05:14:01.000000 devpi-client-6.0.4/testing/test_upload.py
--rw-r--r--   0 fschulze   (501) staff       (20)    47698 2023-04-13 05:14:01.000000 devpi-client-6.0.4/testing/test_use.py
--rw-r--r--   0 fschulze   (501) staff       (20)     1905 2023-04-13 05:14:01.000000 devpi-client-6.0.4/testing/test_user.py
--rw-r--r--   0 fschulze   (501) staff       (20)     1253 2023-04-13 05:14:01.000000 devpi-client-6.0.4/tox.ini
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-07-02 12:04:15.808924 devpi-client-6.0.5/
+-rw-r--r--   0 fschulze   (501) staff       (20)      192 2023-07-02 12:04:11.000000 devpi-client-6.0.5/AUTHORS
+-rw-r--r--   0 fschulze   (501) staff       (20)    26863 2023-07-02 12:04:11.000000 devpi-client-6.0.5/CHANGELOG
+-rw-r--r--   0 fschulze   (501) staff       (20)     1061 2023-07-02 12:04:11.000000 devpi-client-6.0.5/LICENSE
+-rw-r--r--   0 fschulze   (501) staff       (20)      147 2023-07-02 12:04:11.000000 devpi-client-6.0.5/MANIFEST.in
+-rw-r--r--   0 fschulze   (501) staff       (20)     3956 2023-07-02 12:04:15.809050 devpi-client-6.0.5/PKG-INFO
+-rw-r--r--   0 fschulze   (501) staff       (20)      930 2023-07-02 12:04:11.000000 devpi-client-6.0.5/README.rst
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-07-02 12:04:15.801390 devpi-client-6.0.5/devpi/
+-rw-r--r--   0 fschulze   (501) staff       (20)       23 2023-07-02 12:04:11.000000 devpi-client-6.0.5/devpi/__init__.py
+-rw-r--r--   0 fschulze   (501) staff       (20)       70 2023-07-02 12:04:11.000000 devpi-client-6.0.5/devpi/__main__.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     1540 2023-07-02 12:04:11.000000 devpi-client-6.0.5/devpi/getjson.py
+-rw-r--r--   0 fschulze   (501) staff       (20)      679 2023-07-02 12:04:11.000000 devpi-client-6.0.5/devpi/hookspecs.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     3772 2023-07-02 12:04:11.000000 devpi-client-6.0.5/devpi/index.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     2177 2023-07-02 12:04:11.000000 devpi-client-6.0.5/devpi/install.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     7711 2023-07-02 12:04:11.000000 devpi-client-6.0.5/devpi/list_remove.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     1430 2023-07-02 12:04:11.000000 devpi-client-6.0.5/devpi/login.py
+-rw-r--r--   0 fschulze   (501) staff       (20)    45776 2023-07-02 12:04:11.000000 devpi-client-6.0.5/devpi/main.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     3565 2023-07-02 12:04:11.000000 devpi-client-6.0.5/devpi/push.py
+-rw-r--r--   0 fschulze   (501) staff       (20)      536 2023-07-02 12:04:11.000000 devpi-client-6.0.5/devpi/pypirc.py
+-rw-r--r--   0 fschulze   (501) staff       (20)      550 2023-07-02 12:04:11.000000 devpi-client-6.0.5/devpi/refresh.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     9930 2023-07-02 12:04:11.000000 devpi-client-6.0.5/devpi/test.py
+-rw-r--r--   0 fschulze   (501) staff       (20)    20388 2023-07-02 12:04:11.000000 devpi-client-6.0.5/devpi/upload.py
+-rw-r--r--   0 fschulze   (501) staff       (20)    29391 2023-07-02 12:04:11.000000 devpi-client-6.0.5/devpi/use.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     3290 2023-07-02 12:04:11.000000 devpi-client-6.0.5/devpi/user.py
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-07-02 12:04:15.803123 devpi-client-6.0.5/devpi_client.egg-info/
+-rw-r--r--   0 fschulze   (501) staff       (20)     3956 2023-07-02 12:04:15.000000 devpi-client-6.0.5/devpi_client.egg-info/PKG-INFO
+-rw-r--r--   0 fschulze   (501) staff       (20)      987 2023-07-02 12:04:15.000000 devpi-client-6.0.5/devpi_client.egg-info/SOURCES.txt
+-rw-r--r--   0 fschulze   (501) staff       (20)        1 2023-07-02 12:04:15.000000 devpi-client-6.0.5/devpi_client.egg-info/dependency_links.txt
+-rw-r--r--   0 fschulze   (501) staff       (20)      129 2023-07-02 12:04:15.000000 devpi-client-6.0.5/devpi_client.egg-info/entry_points.txt
+-rw-r--r--   0 fschulze   (501) staff       (20)      125 2023-07-02 12:04:15.000000 devpi-client-6.0.5/devpi_client.egg-info/requires.txt
+-rw-r--r--   0 fschulze   (501) staff       (20)        6 2023-07-02 12:04:15.000000 devpi-client-6.0.5/devpi_client.egg-info/top_level.txt
+-rw-r--r--   0 fschulze   (501) staff       (20)      542 2023-07-02 12:04:11.000000 devpi-client-6.0.5/pyproject.toml
+-rw-r--r--   0 fschulze   (501) staff       (20)      115 2023-07-02 12:04:15.809480 devpi-client-6.0.5/setup.cfg
+-rwxr-xr-x   0 fschulze   (501) staff       (20)     2540 2023-07-02 12:04:11.000000 devpi-client-6.0.5/setup.py
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-07-02 12:04:15.808394 devpi-client-6.0.5/testing/
+-rw-r--r--   0 fschulze   (501) staff       (20)        0 2023-07-02 12:04:11.000000 devpi-client-6.0.5/testing/__init__.py
+-rw-r--r--   0 fschulze   (501) staff       (20)    25605 2023-07-02 12:04:11.000000 devpi-client-6.0.5/testing/conftest.py
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-07-02 12:04:15.808685 devpi-client-6.0.5/testing/data/
+-rw-r--r--   0 fschulze   (501) staff       (20)     1846 2023-07-02 12:04:11.000000 devpi-client-6.0.5/testing/data/dddttt-0.1.dev45-py27-none-any.whl
+-rw-r--r--   0 fschulze   (501) staff       (20)    21873 2023-07-02 12:04:11.000000 devpi-client-6.0.5/testing/functional.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     3056 2023-07-02 12:04:11.000000 devpi-client-6.0.5/testing/reqmock.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     6149 2023-07-02 12:04:11.000000 devpi-client-6.0.5/testing/simpypi.py
+-rw-r--r--   0 fschulze   (501) staff       (20)    18473 2023-07-02 12:04:11.000000 devpi-client-6.0.5/testing/test_functional.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     4556 2023-07-02 12:04:11.000000 devpi-client-6.0.5/testing/test_index.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     4245 2023-07-02 12:04:11.000000 devpi-client-6.0.5/testing/test_install.py
+-rw-r--r--   0 fschulze   (501) staff       (20)    13592 2023-07-02 12:04:11.000000 devpi-client-6.0.5/testing/test_list_remove.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     3811 2023-07-02 12:04:11.000000 devpi-client-6.0.5/testing/test_login.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     7466 2023-07-02 12:04:11.000000 devpi-client-6.0.5/testing/test_main.py
+-rw-r--r--   0 fschulze   (501) staff       (20)    10817 2023-07-02 12:04:11.000000 devpi-client-6.0.5/testing/test_push.py
+-rw-r--r--   0 fschulze   (501) staff       (20)      979 2023-07-02 12:04:11.000000 devpi-client-6.0.5/testing/test_pypirc.py
+-rw-r--r--   0 fschulze   (501) staff       (20)    20033 2023-07-02 12:04:11.000000 devpi-client-6.0.5/testing/test_test.py
+-rw-r--r--   0 fschulze   (501) staff       (20)    31035 2023-07-02 12:04:11.000000 devpi-client-6.0.5/testing/test_upload.py
+-rw-r--r--   0 fschulze   (501) staff       (20)    47698 2023-07-02 12:04:11.000000 devpi-client-6.0.5/testing/test_use.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     1905 2023-07-02 12:04:11.000000 devpi-client-6.0.5/testing/test_user.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     1460 2023-07-02 12:04:11.000000 devpi-client-6.0.5/tox.ini
```

### Comparing `devpi-client-6.0.4/CHANGELOG` & `devpi-client-6.0.5/CHANGELOG`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,24 @@
 
 
 .. towncrier release notes start
 
+6.0.5 (2023-07-02)
+==================
+
+Bug Fixes
+---------
+
+- Remember URL when ``devpi use`` causes a 403, so one can use ``devpi login`` afterwards.
+
+- Fix #978: Quote username and password when adding to URL.
+
+- Fix #980: Remove long deprecated backward compatibility for old pluggy versions to fix error with pluggy 1.1.0.
+
+
 6.0.4 (2023-04-13)
 ==================
 
 Bug Fixes
 ---------
 
 - Fix precedence of URL from command line over DEVPI_INDEX environment variable for ``devpi use``.
```

### Comparing `devpi-client-6.0.4/LICENSE` & `devpi-client-6.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `devpi-client-6.0.4/README.rst` & `devpi-client-6.0.5/README.rst`

 * *Files identical despite different names*

### Comparing `devpi-client-6.0.4/devpi/getjson.py` & `devpi-client-6.0.5/devpi/getjson.py`

 * *Files identical despite different names*

### Comparing `devpi-client-6.0.4/devpi/hookspecs.py` & `devpi-client-6.0.5/devpi/hookspecs.py`

 * *Files identical despite different names*

### Comparing `devpi-client-6.0.4/devpi/index.py` & `devpi-client-6.0.5/devpi/index.py`

 * *Files identical despite different names*

### Comparing `devpi-client-6.0.4/devpi/install.py` & `devpi-client-6.0.5/devpi/install.py`

 * *Files identical despite different names*

### Comparing `devpi-client-6.0.4/devpi/list_remove.py` & `devpi-client-6.0.5/devpi/list_remove.py`

 * *Files identical despite different names*

### Comparing `devpi-client-6.0.4/devpi/login.py` & `devpi-client-6.0.5/devpi/login.py`

 * *Files identical despite different names*

### Comparing `devpi-client-6.0.4/devpi/main.py` & `devpi-client-6.0.5/devpi/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,16 +55,14 @@
         mod, func = mod.split(":")
     mod = __import__(mod, None, None, ["__doc__"])
     return Hub(args, pm=pm), getattr(mod, func)
 
 
 def get_pluginmanager(load_entry_points=True):
     pm = PluginManager("devpiclient")
-    # support old plugins, but emit deprecation warnings
-    pm._implprefix = "devpiclient_"
     pm.add_hookspecs(hookspecs)
     if load_entry_points:
         pm.load_setuptools_entrypoints("devpi_client")
     pm.check_pending()
     return pm
```

### Comparing `devpi-client-6.0.4/devpi/push.py` & `devpi-client-6.0.5/devpi/push.py`

 * *Files identical despite different names*

### Comparing `devpi-client-6.0.4/devpi/pypirc.py` & `devpi-client-6.0.5/devpi/pypirc.py`

 * *Files identical despite different names*

### Comparing `devpi-client-6.0.4/devpi/refresh.py` & `devpi-client-6.0.5/devpi/refresh.py`

 * *Files identical despite different names*

### Comparing `devpi-client-6.0.4/devpi/test.py` & `devpi-client-6.0.5/devpi/test.py`

 * *Files identical despite different names*

### Comparing `devpi-client-6.0.4/devpi/upload.py` & `devpi-client-6.0.5/devpi/upload.py`

 * *Files identical despite different names*

### Comparing `devpi-client-6.0.4/devpi/use.py` & `devpi-client-6.0.5/devpi/use.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 from copy import deepcopy
 from operator import attrgetter
+try:
+    from urllib.parse import quote as url_quote
+except ImportError:
+    from urllib import quote as url_quote  # noqa: F401
 import itertools
 import os
 import sys
 import py
 import re
 import json
 
@@ -63,25 +67,27 @@
         self._currentdict = {}
 
     @property
     def simpleindex_auth(self):
         indexserver = URL(self.simpleindex)
         basic_auth = self.get_basic_auth(indexserver)
         if basic_auth:
-            indexserver = indexserver.replace(netloc="%s@%s" % (
-                ':'.join(basic_auth), indexserver.netloc))
+            (username, password) = basic_auth
+            indexserver = indexserver.replace(
+                username=url_quote(username), password=url_quote(password))
         return indexserver.url
 
     @property
     def searchindex_auth(self):
         indexserver = self.get_index_url()
         basic_auth = self.get_basic_auth(indexserver)
         if basic_auth:
-            indexserver = indexserver.replace(netloc="%s@%s" % (
-                ':'.join(basic_auth), indexserver.netloc))
+            (username, password) = basic_auth
+            indexserver = indexserver.replace(
+                username=url_quote(username), password=url_quote(password))
         return indexserver.url
 
     @property
     def indexname(self):
         return self.index[len(self.root_url.url):]
 
     @property
@@ -153,15 +159,15 @@
         return (username, auth) if auth is not None else None
 
     def add_auth_to_url(self, url):
         url = URL(url)
         auth = self.get_auth()
         if auth is not None:
             url = url.replace(
-                username=auth[0], password=auth[1])
+                username=url_quote(auth[0]), password=url_quote(auth[1]))
         return url
 
     def _get_basic_auth_dict(self):
         basic_auth = self._basic_auth
         if not isinstance(basic_auth, dict):
             basic_auth = {}
         return basic_auth
@@ -283,20 +289,28 @@
             client_cert = os.path.abspath(os.path.expanduser(client_cert))
             if not os.path.exists(client_cert):
                 hub.fatal("The client certificate at '%s' doesn't exist." % client_cert)
         elif self.get_client_cert(url=url) is not None:
             hub.info("Using existing client cert for '%s'." % url.url)
 
         def call_http_api(verify):
-            return hub.http_api(
+            r = hub.http_api(
                 "get", url.addpath("+api"), quiet=True,
                 auth=self.get_auth(url=url),
+                fatal=False,
                 basic_auth=basic_auth or self.get_basic_auth(url=url),
                 cert=client_cert or self.get_client_cert(url=url),
                 verify=verify)
+            if r.status_code == 403:
+                r = hub.http_api(
+                    "get", url.addpath("+api"), quiet=True,
+                    basic_auth=basic_auth or self.get_basic_auth(url=url),
+                    cert=client_cert or self.get_client_cert(url=url),
+                    verify=verify)
+            return r
         try:
             # Try calling http_api with ssl verification active
             r = call_http_api(verify=True)
         except hub.http.SSLError:
             # SSL certificate validation failed, set-trusted will be needed
             hub.args.settrusted = 'yes'
             # re-run http_api call ignoring the failed verification
```

### Comparing `devpi-client-6.0.4/devpi/user.py` & `devpi-client-6.0.5/devpi/user.py`

 * *Files identical despite different names*

### Comparing `devpi-client-6.0.4/devpi_client.egg-info/SOURCES.txt` & `devpi-client-6.0.5/devpi_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `devpi-client-6.0.4/setup.py` & `devpi-client-6.0.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     extras_require = {}
 
     setup(
       name="devpi-client",
       description="devpi upload/install/... workflow commands for Python "
                   "developers",
       long_description="\n\n".join([README, CHANGELOG]),
-      version='6.0.4',
+      version='6.0.5',
       packages=['devpi'],
       install_requires=install_requires,
       extras_require=extras_require,
       python_requires=">=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*",
       url="https://devpi.net",
       project_urls={
           'Bug Tracker': 'https://github.com/devpi/devpi/issues',
```

### Comparing `devpi-client-6.0.4/testing/conftest.py` & `devpi-client-6.0.5/testing/conftest.py`

 * *Files identical despite different names*

### Comparing `devpi-client-6.0.4/testing/data/dddttt-0.1.dev45-py27-none-any.whl` & `devpi-client-6.0.5/testing/data/dddttt-0.1.dev45-py27-none-any.whl`

 * *Files identical despite different names*

### Comparing `devpi-client-6.0.4/testing/functional.py` & `devpi-client-6.0.5/testing/functional.py`

 * *Files 6% similar despite different names*

```diff
@@ -344,14 +344,35 @@
         link, = res['result']['1.0']['+links']
         assert len(link['log']) == 1
         assert link['log'][0]['what'] == 'upload'
         assert link['log'][0]['dst'] == '%s/dev' % username
 
 
 @pytest.mark.nomocking
+class TestProjectThings:
+    def test_toxresult(self, mapp):
+        import json
+        mapp.create_and_use('pruser1/dev')
+        content = mapp.makepkg("hello-1.0.tar.gz", b"content", "hello", "1.0")
+        mapp.upload_file_pypi("hello-1.0.tar.gz", content, "hello", "1.0")
+        (pkg_url,) = mapp.getreleaseslist("hello")
+        tox_result_data = dict(foo="bar")
+        mapp.upload_toxresult(pkg_url, json.dumps(tox_result_data))
+        info = mapp.getjson("/%s/hello" % mapp.api.stagename)
+        (toxresult_url,) = [
+            x["href"]
+            for x in info["result"]["1.0"]["+links"]
+            if "for_href" in x]
+        r = mapp.downloadrelease(200, pkg_url)
+        assert r == content
+        r = mapp.downloadrelease(200, toxresult_url)
+        assert json.loads(r.decode('utf-8')) == tox_result_data
+
+
+@pytest.mark.nomocking
 class TestMirrorIndexThings:
     def test_create_and_delete_mirror_index(self, mapp, simpypi):
         mapp.create_and_login_user('mirror1')
         indexname = mapp.auth[0] + "/mirror"
         assert indexname not in mapp.getindexlist()
         indexconfig = dict(
             type="mirror",
```

### Comparing `devpi-client-6.0.4/testing/reqmock.py` & `devpi-client-6.0.5/testing/reqmock.py`

 * *Files identical despite different names*

### Comparing `devpi-client-6.0.4/testing/simpypi.py` & `devpi-client-6.0.5/testing/simpypi.py`

 * *Files identical despite different names*

### Comparing `devpi-client-6.0.4/testing/test_functional.py` & `devpi-client-6.0.5/testing/test_functional.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 from io import BytesIO
 import json
 import pytest
 import requests
 import tarfile
 import time
 
-from .functional import TestUserThings, TestIndexThings # noqa
+from .functional import TestIndexThings  # noqa: F401
+from .functional import TestProjectThings  # noqa: F401
+from .functional import TestUserThings  # noqa: F401
 try:
-    from .functional import TestMirrorIndexThings  # noqa
+    from .functional import TestMirrorIndexThings  # noqa: F401
 except ImportError:
     # when testing with older devpi-server
     class TestMirrorIndexThings:
         def test_mirror_things(self):
             pytest.skip(
                 "Couldn't import TestMirrorIndexThings from devpi server tests.")
 try:
-    from .functional import TestIndexPushThings  # noqa
+    from .functional import TestIndexPushThings  # noqa: F401
 except ImportError:
     # when testing with older devpi-server
     class TestIndexPushThings:
         def test_mirror_things(self):
             pytest.skip(
                 "Couldn't import TestIndexPushThings from devpi server tests.")
 from .functional import MappMixin
@@ -230,14 +232,19 @@
 
     def upload_file_pypi(self, basename, content,
                          name=None, version=None):
         pkg = self.tmpdir.join(basename)
         pkg.write_binary(content)
         self.devpi('upload', pkg.strpath)
 
+    def upload_toxresult(self, url, content, code=200):
+        r = requests.post(url, content)
+        assert r.status_code == code
+        return r.json()
+
     def push(self, name, version, index, indexname=None, code=200):
         self.devpi('push', '%s==%s' % (name, version), index, code=code)
 
     def create_project(self, projectname, code=201, indexname=None):
         pytest.xfail(reason="no way to create project via command line yet")
```

### Comparing `devpi-client-6.0.4/testing/test_index.py` & `devpi-client-6.0.5/testing/test_index.py`

 * *Files identical despite different names*

### Comparing `devpi-client-6.0.4/testing/test_install.py` & `devpi-client-6.0.5/testing/test_install.py`

 * *Files identical despite different names*

### Comparing `devpi-client-6.0.4/testing/test_list_remove.py` & `devpi-client-6.0.5/testing/test_list_remove.py`

 * *Files identical despite different names*

### Comparing `devpi-client-6.0.4/testing/test_login.py` & `devpi-client-6.0.5/testing/test_login.py`

 * *Files identical despite different names*

### Comparing `devpi-client-6.0.4/testing/test_main.py` & `devpi-client-6.0.5/testing/test_main.py`

 * *Files identical despite different names*

### Comparing `devpi-client-6.0.4/testing/test_push.py` & `devpi-client-6.0.5/testing/test_push.py`

 * *Files identical despite different names*

### Comparing `devpi-client-6.0.4/testing/test_pypirc.py` & `devpi-client-6.0.5/testing/test_pypirc.py`

 * *Files identical despite different names*

### Comparing `devpi-client-6.0.4/testing/test_test.py` & `devpi-client-6.0.5/testing/test_test.py`

 * *Files identical despite different names*

### Comparing `devpi-client-6.0.4/testing/test_upload.py` & `devpi-client-6.0.5/testing/test_upload.py`

 * *Files 1% similar despite different names*

```diff
@@ -707,20 +707,16 @@
         else:
             name_version_str = name_version
         initproj(name_version, {"doc": {
             "conf.py": "",
             "index.html": "<html/>"}})
         tmpdir = py.path.local()
         runproc(tmpdir, "python setup.py sdist --format=zip".split())
-        bpath = tmpdir.join('build')
-        out = runproc(
-            tmpdir,
-            "python setup.py build_sphinx -E --build-dir".split() + [bpath.strpath])
         dist = tmpdir.join("dist")
-        zip_dir(bpath.join('html'), dist.join("%s.doc.zip" % name_version_str))
+        zip_dir(tmpdir.join('doc'), dist.join("%s.doc.zip" % name_version_str))
         assert len(dist.listdir()) == 2
         (p, dp) = sorted(dist.listdir(), key=lambda x: '.doc.zip' in x.basename)
         hub = devpi("upload", "--no-isolation", p, dp)
         url = hub.current.get_index_url().url + path
         out = out_devpi("getjson", url)
         data = json.loads(out.stdout.str())
         vv = ViewLinkStore(url, data["result"])
```

### Comparing `devpi-client-6.0.4/testing/test_use.py` & `devpi-client-6.0.5/testing/test_use.py`

 * *Files identical despite different names*

### Comparing `devpi-client-6.0.4/testing/test_user.py` & `devpi-client-6.0.5/testing/test_user.py`

 * *Files identical despite different names*

### Comparing `devpi-client-6.0.4/tox.ini` & `devpi-client-6.0.5/tox.ini`

 * *Files 10% similar despite different names*

```diff
@@ -23,26 +23,34 @@
        flake8<5
        pytest-github-actions-annotate-failures
        pytest-instafail
        pytest-timeout
        devpi-server;python_version!="2.7"
        pypitoken;python_version>="3.7"
        importlib.metadata;python_version<"3.8"
-       py35: ruamel.yaml
-       py35: pyparsing<3
+       ruamel.yaml<0.17.22;python_version<"3.6"
+       pyparsing<3;python_version<"3.6"
        mock
        py!=1.4.32
        sphinx
        webtest
        wheel
        tox
 
 commands = py.test --instafail --maxfail=3 {posargs}
 
 
+[testenv:pypy]
+commands = py.test --instafail --maxfail=3 --timeout 300 {posargs}
+
+
+[testenv:pypy3]
+commands = py.test --instafail --maxfail=3 --timeout 300 {posargs}
+
+
 [testenv:py27-version]
 deps =
 commands = devpi --version
 
 
 [testenv:py27-server520]
 commands = py.test --timeout 300 --instafail --maxfail=3 {posargs} --devpi-server-requirements "devpi-server==5.2.0" --devpi-server-requirements "pyramid<2" --devpi-server-requirements "ruamel.yaml"
```

