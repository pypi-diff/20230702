# Comparing `tmp/pulumiverse_purrl-0.4.0.tar.gz` & `tmp/pulumiverse_purrl-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumiverse_purrl-0.4.0.tar", last modified: Fri Apr 28 08:19:30 2023, max compression
+gzip compressed data, was "pulumiverse_purrl-0.4.1.tar", last modified: Sun Jul  2 10:20:39 2023, max compression
```

## Comparing `pulumiverse_purrl-0.4.0.tar` & `pulumiverse_purrl-0.4.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 08:19:30.453354 pulumiverse_purrl-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-04-28 08:19:30.453354 pulumiverse_purrl-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-04-28 08:19:30.000000 pulumiverse_purrl-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 08:19:30.453354 pulumiverse_purrl-0.4.0/pulumiverse_purrl/
--rw-------   0 runner    (1001) docker     (123)      606 2023-04-28 08:19:30.000000 pulumiverse_purrl-0.4.0/pulumiverse_purrl/__init__.py
--rw-------   0 runner    (1001) docker     (123)     8080 2023-04-28 08:19:30.000000 pulumiverse_purrl-0.4.0/pulumiverse_purrl/_utilities.py
--rw-------   0 runner    (1001) docker     (123)     2713 2023-04-28 08:19:30.000000 pulumiverse_purrl-0.4.0/pulumiverse_purrl/provider.py
--rw-------   0 runner    (1001) docker     (123)       93 2023-04-28 08:19:30.000000 pulumiverse_purrl-0.4.0/pulumiverse_purrl/pulumi-plugin.json
--rw-------   0 runner    (1001) docker     (123)    26974 2023-04-28 08:19:30.000000 pulumiverse_purrl-0.4.0/pulumiverse_purrl/purrl.py
--rw-------   0 runner    (1001) docker     (123)        0 2023-04-28 08:19:30.000000 pulumiverse_purrl-0.4.0/pulumiverse_purrl/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 08:19:30.453354 pulumiverse_purrl-0.4.0/pulumiverse_purrl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-04-28 08:19:30.000000 pulumiverse_purrl-0.4.0/pulumiverse_purrl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-04-28 08:19:30.000000 pulumiverse_purrl-0.4.0/pulumiverse_purrl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 08:19:30.000000 pulumiverse_purrl-0.4.0/pulumiverse_purrl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 08:19:30.000000 pulumiverse_purrl-0.4.0/pulumiverse_purrl.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-28 08:19:30.000000 pulumiverse_purrl-0.4.0/pulumiverse_purrl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-28 08:19:30.000000 pulumiverse_purrl-0.4.0/pulumiverse_purrl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 08:19:30.453354 pulumiverse_purrl-0.4.0/setup.cfg
--rw-------   0 runner    (1001) docker     (123)     2153 2023-04-28 08:19:30.000000 pulumiverse_purrl-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:20:39.061284 pulumiverse_purrl-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-07-02 10:20:39.057284 pulumiverse_purrl-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-07-02 10:20:38.000000 pulumiverse_purrl-0.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:20:39.057284 pulumiverse_purrl-0.4.1/pulumiverse_purrl/
+-rw-------   0 runner    (1001) docker     (123)      606 2023-07-02 10:20:38.000000 pulumiverse_purrl-0.4.1/pulumiverse_purrl/__init__.py
+-rw-------   0 runner    (1001) docker     (123)     8080 2023-07-02 10:20:38.000000 pulumiverse_purrl-0.4.1/pulumiverse_purrl/_utilities.py
+-rw-------   0 runner    (1001) docker     (123)     2713 2023-07-02 10:20:38.000000 pulumiverse_purrl-0.4.1/pulumiverse_purrl/provider.py
+-rw-------   0 runner    (1001) docker     (123)       93 2023-07-02 10:20:38.000000 pulumiverse_purrl-0.4.1/pulumiverse_purrl/pulumi-plugin.json
+-rw-------   0 runner    (1001) docker     (123)    26974 2023-07-02 10:20:38.000000 pulumiverse_purrl-0.4.1/pulumiverse_purrl/purrl.py
+-rw-------   0 runner    (1001) docker     (123)        0 2023-07-02 10:20:38.000000 pulumiverse_purrl-0.4.1/pulumiverse_purrl/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:20:39.057284 pulumiverse_purrl-0.4.1/pulumiverse_purrl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-07-02 10:20:39.000000 pulumiverse_purrl-0.4.1/pulumiverse_purrl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-02 10:20:39.000000 pulumiverse_purrl-0.4.1/pulumiverse_purrl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 10:20:39.000000 pulumiverse_purrl-0.4.1/pulumiverse_purrl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 10:20:39.000000 pulumiverse_purrl-0.4.1/pulumiverse_purrl.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-02 10:20:39.000000 pulumiverse_purrl-0.4.1/pulumiverse_purrl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-02 10:20:39.000000 pulumiverse_purrl-0.4.1/pulumiverse_purrl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 10:20:39.061284 pulumiverse_purrl-0.4.1/setup.cfg
+-rw-------   0 runner    (1001) docker     (123)     2153 2023-07-02 10:20:38.000000 pulumiverse_purrl-0.4.1/setup.py
```

### Comparing `pulumiverse_purrl-0.4.0/PKG-INFO` & `pulumiverse_purrl-0.4.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumiverse_purrl
-Version: 0.4.0
+Version: 0.4.1
 Summary: A Pulumi native provider for making API calls
 Home-page: https://pulumi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumiverse/pulumi-purrl
 Keywords: pulumi command category/utility kind/native
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumiverse_purrl-0.4.0/README.md` & `pulumiverse_purrl-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `pulumiverse_purrl-0.4.0/pulumiverse_purrl/__init__.py` & `pulumiverse_purrl-0.4.1/pulumiverse_purrl/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_purrl-0.4.0/pulumiverse_purrl/_utilities.py` & `pulumiverse_purrl-0.4.1/pulumiverse_purrl/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_purrl-0.4.0/pulumiverse_purrl/provider.py` & `pulumiverse_purrl-0.4.1/pulumiverse_purrl/provider.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_purrl-0.4.0/pulumiverse_purrl/purrl.py` & `pulumiverse_purrl-0.4.1/pulumiverse_purrl/purrl.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_purrl-0.4.0/pulumiverse_purrl.egg-info/PKG-INFO` & `pulumiverse_purrl-0.4.1/pulumiverse_purrl.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumiverse-purrl
-Version: 0.4.0
+Version: 0.4.1
 Summary: A Pulumi native provider for making API calls
 Home-page: https://pulumi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumiverse/pulumi-purrl
 Keywords: pulumi command category/utility kind/native
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumiverse_purrl-0.4.0/setup.py` & `pulumiverse_purrl-0.4.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "0.4.0"
-PLUGIN_VERSION = "0.4.0"
+VERSION = "0.4.1"
+PLUGIN_VERSION = "0.4.1"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'purrl', PLUGIN_VERSION, '--server', 'github://api.github.com/pulumiverse'])
         except OSError as error:
```

