# Comparing `tmp/intex-spa-0.8.3.tar.gz` & `tmp/intex-spa-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "intex-spa-0.8.3.tar", last modified: Wed Aug 10 19:13:48 2022, max compression
+gzip compressed data, was "intex-spa-0.8.4.tar", last modified: Sun Jul  2 10:01:29 2023, max compression
```

## Comparing `intex-spa-0.8.3.tar` & `intex-spa-0.8.4.tar`

### file list

```diff
@@ -1,20 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 19:13:48.619398 intex-spa-0.8.3/
--rw-r--r--   0 runner    (1001) docker     (121)     1083 2022-08-10 19:13:36.000000 intex-spa-0.8.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     2170 2022-08-10 19:13:48.619398 intex-spa-0.8.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1768 2022-08-10 19:13:36.000000 intex-spa-0.8.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 19:13:48.619398 intex-spa-0.8.3/intex_spa/
--rw-r--r--   0 runner    (1001) docker     (121)      179 2022-08-10 19:13:36.000000 intex-spa-0.8.3/intex_spa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9122 2022-08-10 19:13:36.000000 intex-spa-0.8.3/intex_spa/intex_spa.py
--rw-r--r--   0 runner    (1001) docker     (121)      229 2022-08-10 19:13:36.000000 intex-spa-0.8.3/intex_spa/intex_spa_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     3664 2022-08-10 19:13:36.000000 intex-spa-0.8.3/intex_spa/intex_spa_network_layer.py
--rw-r--r--   0 runner    (1001) docker     (121)     1771 2022-08-10 19:13:36.000000 intex-spa-0.8.3/intex_spa/intex_spa_object_info.py
--rw-r--r--   0 runner    (1001) docker     (121)     4535 2022-08-10 19:13:36.000000 intex-spa-0.8.3/intex_spa/intex_spa_object_status.py
--rw-r--r--   0 runner    (1001) docker     (121)     4298 2022-08-10 19:13:36.000000 intex-spa-0.8.3/intex_spa/intex_spa_query.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-10 19:13:48.619398 intex-spa-0.8.3/intex_spa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2170 2022-08-10 19:13:48.000000 intex-spa-0.8.3/intex_spa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      417 2022-08-10 19:13:48.000000 intex-spa-0.8.3/intex_spa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-10 19:13:48.000000 intex-spa-0.8.3/intex_spa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-08-10 19:13:48.000000 intex-spa-0.8.3/intex_spa.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-08-10 19:13:48.000000 intex-spa-0.8.3/intex_spa.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      165 2022-08-10 19:13:48.619398 intex-spa-0.8.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      656 2022-08-10 19:13:46.000000 intex-spa-0.8.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:01:29.700034 intex-spa-0.8.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-07-02 10:01:20.000000 intex-spa-0.8.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-07-02 10:01:29.700034 intex-spa-0.8.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-07-02 10:01:20.000000 intex-spa-0.8.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:01:29.700034 intex-spa-0.8.4/intex_spa/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-02 10:01:20.000000 intex-spa-0.8.4/intex_spa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9122 2023-07-02 10:01:20.000000 intex-spa-0.8.4/intex_spa/intex_spa.py
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-02 10:01:20.000000 intex-spa-0.8.4/intex_spa/intex_spa_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3664 2023-07-02 10:01:20.000000 intex-spa-0.8.4/intex_spa/intex_spa_network_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-07-02 10:01:20.000000 intex-spa-0.8.4/intex_spa/intex_spa_object_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4535 2023-07-02 10:01:20.000000 intex-spa-0.8.4/intex_spa/intex_spa_object_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4469 2023-07-02 10:01:20.000000 intex-spa-0.8.4/intex_spa/intex_spa_query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:01:29.700034 intex-spa-0.8.4/intex_spa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-07-02 10:01:29.000000 intex-spa-0.8.4/intex_spa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-02 10:01:29.000000 intex-spa-0.8.4/intex_spa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 10:01:29.000000 intex-spa-0.8.4/intex_spa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-02 10:01:29.000000 intex-spa-0.8.4/intex_spa.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-02 10:01:29.704034 intex-spa-0.8.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-02 10:01:29.000000 intex-spa-0.8.4/setup.py
```

### Comparing `intex-spa-0.8.3/LICENSE` & `intex-spa-0.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `intex-spa-0.8.3/PKG-INFO` & `intex-spa-0.8.4/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,14 @@
-Metadata-Version: 2.1
-Name: intex-spa
-Version: 0.8.3
-Summary: Intex Spa wifi client
-Home-page: https://github.com/mathieu-mp/intex-spa
-Author: Mathieu Payrol
-Author-email: intex-spa@payrol.fr
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # intex-spa
 
 <!-- badges start -->
 
 [![PyPI version][pypibadge]][pypilink]
-[![Maintained][Maintained]](#)
+![Project Maintenance][maintenance-shield]
+[![Open in Remote - Containers][devcontainer-badge]][devcontainer]
 
 <!-- badges end -->
 
 _An AsyncIO-compatible Intex Spa wifi client_
 
 ## Description
 
@@ -70,13 +58,15 @@
 
 ***Reminder**: Major version zero (0.y.z) is for initial development. Anything MAY change at any time. The public API SHOULD NOT be considered stable.*
 
 For Changelog, please read [releases].
 
 <!-- links start -->
 
-[maintained]: https://img.shields.io/maintenance/yes/2022.svg
 [pypilink]: https://pypi.org/project/intex-spa/
 [pypibadge]: https://badge.fury.io/py/intex-spa.svg
 [releases]: https://github.com/mathieu-mp/intex-spa/releases
+[maintenance-shield]: https://img.shields.io/maintenance/yes/2023.svg
+[devcontainer]: https://vscode.dev/redirect?url=vscode://ms-vscode-remote.remote-containers/cloneInVolume?url=https://github.com/mathieu-mp/intex-spa
+[devcontainer-badge]: https://img.shields.io/static/v1?label=Remote%20-%20Containers&message=Open&color=blue&logo=visualstudiocode
 
-<!-- links end -->
+<!-- links end -->
```

### Comparing `intex-spa-0.8.3/README.md` & `intex-spa-0.8.4/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,27 @@
+Metadata-Version: 2.1
+Name: intex-spa
+Version: 0.8.4
+Summary: Intex Spa wifi client
+Home-page: https://github.com/mathieu-mp/intex-spa
+Author: Mathieu Payrol
+Author-email: intex-spa@payrol.fr
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # intex-spa
 
 <!-- badges start -->
 
 [![PyPI version][pypibadge]][pypilink]
-[![Maintained][Maintained]](#)
+![Project Maintenance][maintenance-shield]
+[![Open in Remote - Containers][devcontainer-badge]][devcontainer]
 
 <!-- badges end -->
 
 _An AsyncIO-compatible Intex Spa wifi client_
 
 ## Description
 
@@ -57,13 +71,15 @@
 
 ***Reminder**: Major version zero (0.y.z) is for initial development. Anything MAY change at any time. The public API SHOULD NOT be considered stable.*
 
 For Changelog, please read [releases].
 
 <!-- links start -->
 
-[maintained]: https://img.shields.io/maintenance/yes/2022.svg
 [pypilink]: https://pypi.org/project/intex-spa/
 [pypibadge]: https://badge.fury.io/py/intex-spa.svg
 [releases]: https://github.com/mathieu-mp/intex-spa/releases
+[maintenance-shield]: https://img.shields.io/maintenance/yes/2023.svg
+[devcontainer]: https://vscode.dev/redirect?url=vscode://ms-vscode-remote.remote-containers/cloneInVolume?url=https://github.com/mathieu-mp/intex-spa
+[devcontainer-badge]: https://img.shields.io/static/v1?label=Remote%20-%20Containers&message=Open&color=blue&logo=visualstudiocode
 
-<!-- links end -->
+<!-- links end -->
```

### Comparing `intex-spa-0.8.3/intex_spa/intex_spa.py` & `intex-spa-0.8.4/intex_spa/intex_spa.py`

 * *Files identical despite different names*

### Comparing `intex-spa-0.8.3/intex_spa/intex_spa_network_layer.py` & `intex-spa-0.8.4/intex_spa/intex_spa_network_layer.py`

 * *Files identical despite different names*

### Comparing `intex-spa-0.8.3/intex_spa/intex_spa_object_info.py` & `intex-spa-0.8.4/intex_spa/intex_spa_object_info.py`

 * *Files identical despite different names*

### Comparing `intex-spa-0.8.3/intex_spa/intex_spa_object_status.py` & `intex-spa-0.8.4/intex_spa/intex_spa_object_status.py`

 * *Files identical despite different names*

### Comparing `intex-spa-0.8.3/intex_spa/intex_spa_query.py` & `intex-spa-0.8.4/intex_spa/intex_spa_query.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,21 +51,25 @@
 def checksum_as_int(data: str) -> int:
     """Return integer checksum for the given data, as expected by Intex Spa protocol"""
     calculated_checksum = 0xFF
     for index in range(0, len(data), 2):
         calculated_checksum = calculated_checksum - (
             int("0x" + data[index : index + 2], 16)
         )
-    return calculated_checksum % 0xFF
+    calculated_checksum = calculated_checksum % 0xFF
+    # Fix: https://github.com/mathieu-mp/intex-spa/issues/27
+    if calculated_checksum == 0x00:
+        calculated_checksum = 0xFF
+    return calculated_checksum
 
 
 def checksum_as_str(data: str) -> str:
     """Return string checksum for the given data, as expected by Intex Spa protocol"""
     # Return checksum as a hex string without 0x prefix
-    return hex(checksum_as_int(data) % 0xFF)[2:].upper()
+    return hex(checksum_as_int(data))[2:].upper()
 
 
 class IntexSpaQuery:
     """
     Class to manage one application-layer query with Intex Spa wifi module
 
     Manages encoding and decoding of one request and its response messages
```

### Comparing `intex-spa-0.8.3/intex_spa.egg-info/PKG-INFO` & `intex-spa-0.8.4/intex_spa.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: intex-spa
-Version: 0.8.3
+Version: 0.8.4
 Summary: Intex Spa wifi client
 Home-page: https://github.com/mathieu-mp/intex-spa
 Author: Mathieu Payrol
 Author-email: intex-spa@payrol.fr
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -12,15 +12,16 @@
 License-File: LICENSE
 
 # intex-spa
 
 <!-- badges start -->
 
 [![PyPI version][pypibadge]][pypilink]
-[![Maintained][Maintained]](#)
+![Project Maintenance][maintenance-shield]
+[![Open in Remote - Containers][devcontainer-badge]][devcontainer]
 
 <!-- badges end -->
 
 _An AsyncIO-compatible Intex Spa wifi client_
 
 ## Description
 
@@ -70,13 +71,15 @@
 
 ***Reminder**: Major version zero (0.y.z) is for initial development. Anything MAY change at any time. The public API SHOULD NOT be considered stable.*
 
 For Changelog, please read [releases].
 
 <!-- links start -->
 
-[maintained]: https://img.shields.io/maintenance/yes/2022.svg
 [pypilink]: https://pypi.org/project/intex-spa/
 [pypibadge]: https://badge.fury.io/py/intex-spa.svg
 [releases]: https://github.com/mathieu-mp/intex-spa/releases
+[maintenance-shield]: https://img.shields.io/maintenance/yes/2023.svg
+[devcontainer]: https://vscode.dev/redirect?url=vscode://ms-vscode-remote.remote-containers/cloneInVolume?url=https://github.com/mathieu-mp/intex-spa
+[devcontainer-badge]: https://img.shields.io/static/v1?label=Remote%20-%20Containers&message=Open&color=blue&logo=visualstudiocode
 
 <!-- links end -->
```

### Comparing `intex-spa-0.8.3/setup.py` & `intex-spa-0.8.4/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 from setuptools import setup, find_packages
 
 
 with open("README.md", "r") as fh:
     README = fh.read()
 setup(
     name="intex-spa",
-    version="0.8.3",
+    version="0.8.4",
     author="Mathieu Payrol",
     author_email="intex-spa@payrol.fr",
     description="Intex Spa wifi client",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/mathieu-mp/intex-spa",
     packages=find_packages(),
-    install_requires=["asyncio"],
+    install_requires=[],
     classifiers=(
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ),
 )
```

