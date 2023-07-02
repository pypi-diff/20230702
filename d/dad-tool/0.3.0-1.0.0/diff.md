# Comparing `tmp/dad-tool-0.3.0.tar.gz` & `tmp/dad-tool-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dad-tool-0.3.0.tar", last modified: Sun Feb  6 06:30:11 2022, max compression
+gzip compressed data, was "dad-tool-1.0.0.tar", last modified: Sun Jul  2 03:05:31 2023, max compression
```

## Comparing `dad-tool-0.3.0.tar` & `dad-tool-1.0.0.tar`

### file list

```diff
@@ -1,69 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-06 06:30:11.665684 dad-tool-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1071 2022-02-06 06:29:59.000000 dad-tool-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     4318 2022-02-06 06:30:11.661684 dad-tool-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3825 2022-02-06 06:29:59.000000 dad-tool-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-06 06:30:11.657684 dad-tool-0.3.0/dad_tool/
--rw-r--r--   0 runner    (1001) docker     (121)      192 2022-02-06 06:29:59.000000 dad-tool-0.3.0/dad_tool/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-06 06:30:11.653684 dad-tool-0.3.0/dad_tool/dad/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-06 06:30:11.653684 dad-tool-0.3.0/dad_tool/dad/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-06 06:30:11.653684 dad-tool-0.3.0/dad_tool/dad/src/addresses/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-06 06:30:11.657684 dad-tool-0.3.0/dad_tool/dad/src/addresses/australia/
--rw-r--r--   0 runner    (1001) docker     (121)      756 2022-02-06 06:30:00.000000 dad-tool-0.3.0/dad_tool/dad/src/addresses/australia/vt-addresses.json
--rw-r--r--   0 runner    (1001) docker     (121)      545 2022-02-06 06:30:00.000000 dad-tool-0.3.0/dad_tool/dad/src/addresses/australia/vt-addresses.min.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-06 06:30:11.657684 dad-tool-0.3.0/dad_tool/dad/src/addresses/canada/
--rw-r--r--   0 runner    (1001) docker     (121)      741 2022-02-06 06:30:00.000000 dad-tool-0.3.0/dad_tool/dad/src/addresses/canada/bc-addresses.json
--rw-r--r--   0 runner    (1001) docker     (121)      530 2022-02-06 06:30:00.000000 dad-tool-0.3.0/dad_tool/dad/src/addresses/canada/bc-addresses.min.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-06 06:30:11.657684 dad-tool-0.3.0/dad_tool/dad/src/addresses/china/
--rw-r--r--   0 runner    (1001) docker     (121)      750 2022-02-06 06:30:00.000000 dad-tool-0.3.0/dad_tool/dad/src/addresses/china/bj-addresses.json
--rw-r--r--   0 runner    (1001) docker     (121)      540 2022-02-06 06:30:00.000000 dad-tool-0.3.0/dad_tool/dad/src/addresses/china/bj-addresses.min.json
--rw-r--r--   0 runner    (1001) docker     (121)      740 2022-02-06 06:30:00.000000 dad-tool-0.3.0/dad_tool/dad/src/addresses/china/hk-addresses.json
--rw-r--r--   0 runner    (1001) docker     (121)      530 2022-02-06 06:30:00.000000 dad-tool-0.3.0/dad_tool/dad/src/addresses/china/hk-addresses.min.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-06 06:30:11.657684 dad-tool-0.3.0/dad_tool/dad/src/addresses/europe/
--rw-r--r--   0 runner    (1001) docker     (121)      703 2022-02-06 06:30:00.000000 dad-tool-0.3.0/dad_tool/dad/src/addresses/europe/de-addresses.json
--rw-r--r--   0 runner    (1001) docker     (121)      493 2022-02-06 06:30:00.000000 dad-tool-0.3.0/dad_tool/dad/src/addresses/europe/de-addresses.min.json
--rw-r--r--   0 runner    (1001) docker     (121)      784 2022-02-06 06:30:00.000000 dad-tool-0.3.0/dad_tool/dad/src/addresses/europe/es-addresses.json
--rw-r--r--   0 runner    (1001) docker     (121)      574 2022-02-06 06:30:00.000000 dad-tool-0.3.0/dad_tool/dad/src/addresses/europe/es-addresses.min.json
--rw-r--r--   0 runner    (1001) docker     (121)      732 2022-02-06 06:30:00.000000 dad-tool-0.3.0/dad_tool/dad/src/addresses/europe/fr-addresses.json
--rw-r--r--   0 runner    (1001) docker     (121)      520 2022-02-06 06:30:00.000000 dad-tool-0.3.0/dad_tool/dad/src/addresses/europe/fr-addresses.min.json
--rw-r--r--   0 runner    (1001) docker     (121)      722 2022-02-06 06:30:00.000000 dad-tool-0.3.0/dad_tool/dad/src/addresses/europe/uk-addresses.json
--rw-r--r--   0 runner    (1001) docker     (121)      512 2022-02-06 06:30:00.000000 dad-tool-0.3.0/dad_tool/dad/src/addresses/europe/uk-addresses.min.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-06 06:30:11.657684 dad-tool-0.3.0/dad_tool/dad/src/addresses/mexico/
--rw-r--r--   0 runner    (1001) docker     (121)      904 2022-02-06 06:30:00.000000 dad-tool-0.3.0/dad_tool/dad/src/addresses/mexico/mx-addresses.json
--rw-r--r--   0 runner    (1001) docker     (121)      694 2022-02-06 06:30:00.000000 dad-tool-0.3.0/dad_tool/dad/src/addresses/mexico/mx-addresses.min.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-06 06:30:11.661684 dad-tool-0.3.0/dad_tool/dad/src/addresses/united-states/
--rw-r--r--   0 runner    (1001) docker     (121)    14544 2022-02-06 06:30:00.000000 dad-tool-0.3.0/dad_tool/dad/src/addresses/united-states/az-addresses.json
--rw-r--r--   0 runner    (1001) docker     (121)    10344 2022-02-06 06:30:00.000000 dad-tool-0.3.0/dad_tool/dad/src/addresses/united-states/az-addresses.min.json
--rw-r--r--   0 runner    (1001) docker     (121)    14811 2022-02-06 06:30:00.000000 dad-tool-0.3.0/dad_tool/dad/src/addresses/united-states/ca-addresses.json
--rw-r--r--   0 runner    (1001) docker     (121)    10611 2022-02-06 06:30:00.000000 dad-tool-0.3.0/dad_tool/dad/src/addresses/united-states/ca-addresses.min.json
--rw-r--r--   0 runner    (1001) docker     (121)    14168 2022-02-06 06:30:00.000000 dad-tool-0.3.0/dad_tool/dad/src/addresses/united-states/id-addresses.json
--rw-r--r--   0 runner    (1001) docker     (121)     9968 2022-02-06 06:30:00.000000 dad-tool-0.3.0/dad_tool/dad/src/addresses/united-states/id-addresses.min.json
--rw-r--r--   0 runner    (1001) docker     (121)    14488 2022-02-06 06:30:00.000000 dad-tool-0.3.0/dad_tool/dad/src/addresses/united-states/ks-addresses.json
--rw-r--r--   0 runner    (1001) docker     (121)    10288 2022-02-06 06:30:00.000000 dad-tool-0.3.0/dad_tool/dad/src/addresses/united-states/ks-addresses.min.json
--rw-r--r--   0 runner    (1001) docker     (121)    14460 2022-02-06 06:30:00.000000 dad-tool-0.3.0/dad_tool/dad/src/addresses/united-states/nv-addresses.json
--rw-r--r--   0 runner    (1001) docker     (121)    10260 2022-02-06 06:30:00.000000 dad-tool-0.3.0/dad_tool/dad/src/addresses/united-states/nv-addresses.min.json
--rw-r--r--   0 runner    (1001) docker     (121)    14567 2022-02-06 06:30:00.000000 dad-tool-0.3.0/dad_tool/dad/src/addresses/united-states/ny-addresses.json
--rw-r--r--   0 runner    (1001) docker     (121)    10367 2022-02-06 06:30:00.000000 dad-tool-0.3.0/dad_tool/dad/src/addresses/united-states/ny-addresses.min.json
--rw-r--r--   0 runner    (1001) docker     (121)    14914 2022-02-06 06:30:00.000000 dad-tool-0.3.0/dad_tool/dad/src/addresses/united-states/or-addresses.json
--rw-r--r--   0 runner    (1001) docker     (121)    10714 2022-02-06 06:30:00.000000 dad-tool-0.3.0/dad_tool/dad/src/addresses/united-states/or-addresses.min.json
--rw-r--r--   0 runner    (1001) docker     (121)    14447 2022-02-06 06:30:00.000000 dad-tool-0.3.0/dad_tool/dad/src/addresses/united-states/tx-addresses.json
--rw-r--r--   0 runner    (1001) docker     (121)    10247 2022-02-06 06:30:00.000000 dad-tool-0.3.0/dad_tool/dad/src/addresses/united-states/tx-addresses.min.json
--rw-r--r--   0 runner    (1001) docker     (121)    14138 2022-02-06 06:30:00.000000 dad-tool-0.3.0/dad_tool/dad/src/addresses/united-states/ut-addresses.json
--rw-r--r--   0 runner    (1001) docker     (121)     9938 2022-02-06 06:30:00.000000 dad-tool-0.3.0/dad_tool/dad/src/addresses/united-states/ut-addresses.min.json
--rw-r--r--   0 runner    (1001) docker     (121)    14570 2022-02-06 06:30:00.000000 dad-tool-0.3.0/dad_tool/dad/src/addresses/united-states/wa-addresses.json
--rw-r--r--   0 runner    (1001) docker     (121)    10370 2022-02-06 06:30:00.000000 dad-tool-0.3.0/dad_tool/dad/src/addresses/united-states/wa-addresses.min.json
--rw-r--r--   0 runner    (1001) docker     (121)     3113 2022-02-06 06:29:59.000000 dad-tool-0.3.0/dad_tool/data_router.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-06 06:29:59.000000 dad-tool-0.3.0/dad_tool/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-06 06:30:11.657684 dad-tool-0.3.0/dad_tool.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4318 2022-02-06 06:30:11.000000 dad-tool-0.3.0/dad_tool.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2526 2022-02-06 06:30:11.000000 dad-tool-0.3.0/dad_tool.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-06 06:30:11.000000 dad-tool-0.3.0/dad_tool.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       91 2022-02-06 06:30:11.000000 dad-tool-0.3.0/dad_tool.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-02-06 06:30:11.000000 dad-tool-0.3.0/dad_tool.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      111 2022-02-06 06:29:59.000000 dad-tool-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-02-06 06:30:11.665684 dad-tool-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1065 2022-02-06 06:29:59.000000 dad-tool-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-06 06:30:11.661684 dad-tool-0.3.0/test/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-06 06:29:59.000000 dad-tool-0.3.0/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-06 06:30:11.661684 dad-tool-0.3.0/test/unit/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-06 06:29:59.000000 dad-tool-0.3.0/test/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      586 2022-02-06 06:29:59.000000 dad-tool-0.3.0/test/unit/test_data_router.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 03:05:31.394713 dad-tool-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-02 03:05:05.000000 dad-tool-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4262 2023-07-02 03:05:31.394713 dad-tool-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3789 2023-07-02 03:05:05.000000 dad-tool-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 03:05:31.394713 dad-tool-1.0.0/dad_tool/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-02 03:05:05.000000 dad-tool-1.0.0/dad_tool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-07-02 03:05:05.000000 dad-tool-1.0.0/dad_tool/data_router.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 03:05:05.000000 dad-tool-1.0.0/dad_tool/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 03:05:31.394713 dad-tool-1.0.0/dad_tool.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4262 2023-07-02 03:05:31.000000 dad-tool-1.0.0/dad_tool.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-02 03:05:31.000000 dad-tool-1.0.0/dad_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 03:05:31.000000 dad-tool-1.0.0/dad_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-02 03:05:31.000000 dad-tool-1.0.0/dad_tool.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-02 03:05:31.000000 dad-tool-1.0.0/dad_tool.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-02 03:05:05.000000 dad-tool-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 03:05:31.394713 dad-tool-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-07-02 03:05:05.000000 dad-tool-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 03:05:31.394713 dad-tool-1.0.0/test/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 03:05:31.394713 dad-tool-1.0.0/test/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 03:05:05.000000 dad-tool-1.0.0/test/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-07-02 03:05:05.000000 dad-tool-1.0.0/test/unit/test_data_router.py
```

### Comparing `dad-tool-0.3.0/LICENSE` & `dad-tool-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dad-tool-0.3.0/PKG-INFO` & `dad-tool-1.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: dad-tool
-Version: 0.3.0
+Version: 1.0.0
 Summary: Dummy Address Data (DAD) - Real addresses from all around the world.
 Home-page: http://github.com/Justintime50/dad-python
 Author: Justintime50
 License: MIT
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7, <4
+Requires-Python: >=3.8, <4
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 <div align="center">
 
 # Dummy Address Data (DAD) Python Library
@@ -34,15 +33,15 @@
 ## Install
 
 ```bash
 # Install tool
 pip3 install dad_tool
 
 # Install locally
-make install
+just install
 ```
 
 ## Address Data
 
 Address objects will look like the [sample below](#sample-address-object). The data type of each field on an address object is a `string`. A list of addresses is an `array` of `json` objects.
 
 Attempts have been made to verify addresses and ensure that street1, city, state, and zip are present on all records. Some lists may be shorter than others to avoid complexity or because of a lack of accurate data.
@@ -94,15 +93,14 @@
 | Nevada - Lincoln Area     | US_NV |
 | New York - Rochester Area | US_NY |
 | Oregon - Portland Area    | US_OR |
 | Texas - Austin Area       | US_TX |
 | Utah - Provo Area         | US_UT |
 | Washington - Spokane Area | US_WA |
 
-
 ## Usage
 
 ```python
 import dad_tool
 
 # Grab a random UT address
 address = dad_tool.random_address('US_UT')
@@ -142,18 +140,16 @@
 }
 ```
 
 ## Development
 
 ```bash
 # To setup the `DAD` git submodule
-git submodule init && git submodule update --remote
+just setup-dad
 
 # Get a comprehensive list of development tools
-make help
+just --list
 ```
 
 ## Attribution
 
 - Addresses provided by [DAD](https://github.com/justintime50/dad).
-
-
```

### Comparing `dad-tool-0.3.0/README.md` & `dad-tool-1.0.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 ## Install
 
 ```bash
 # Install tool
 pip3 install dad_tool
 
 # Install locally
-make install
+just install
 ```
 
 ## Address Data
 
 Address objects will look like the [sample below](#sample-address-object). The data type of each field on an address object is a `string`. A list of addresses is an `array` of `json` objects.
 
 Attempts have been made to verify addresses and ensure that street1, city, state, and zip are present on all records. Some lists may be shorter than others to avoid complexity or because of a lack of accurate data.
@@ -78,15 +78,14 @@
 | Nevada - Lincoln Area     | US_NV |
 | New York - Rochester Area | US_NY |
 | Oregon - Portland Area    | US_OR |
 | Texas - Austin Area       | US_TX |
 | Utah - Provo Area         | US_UT |
 | Washington - Spokane Area | US_WA |
 
-
 ## Usage
 
 ```python
 import dad_tool
 
 # Grab a random UT address
 address = dad_tool.random_address('US_UT')
@@ -126,16 +125,16 @@
 }
 ```
 
 ## Development
 
 ```bash
 # To setup the `DAD` git submodule
-git submodule init && git submodule update --remote
+just setup-dad
 
 # Get a comprehensive list of development tools
-make help
+just --list
 ```
 
 ## Attribution
 
 - Addresses provided by [DAD](https://github.com/justintime50/dad).
```

### Comparing `dad-tool-0.3.0/dad_tool/data_router.py` & `dad-tool-1.0.0/dad_tool/data_router.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 import json
 import random
-from typing import Dict, List
+from typing import (
+    Dict,
+    List,
+)
 
 import pkg_resources
 
 
 def list_addresses(address_tag: str) -> List[Dict[str, str]]:
     address_json = _open_json_file(address_tag)
 
     return address_json
 
 
 def random_address(address_tag: str) -> Dict[str, str]:
     address_json = _open_json_file(address_tag)
-    random_address = random.choice(address_json)
+    random_address = random.choice(address_json)  # nosec - not using random for security
 
     return random_address
 
 
 def list_iso_country_codes():
     raise NotImplementedError()
```

### Comparing `dad-tool-0.3.0/dad_tool.egg-info/PKG-INFO` & `dad-tool-1.0.0/dad_tool.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: dad-tool
-Version: 0.3.0
+Version: 1.0.0
 Summary: Dummy Address Data (DAD) - Real addresses from all around the world.
 Home-page: http://github.com/Justintime50/dad-python
 Author: Justintime50
 License: MIT
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7, <4
+Requires-Python: >=3.8, <4
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 <div align="center">
 
 # Dummy Address Data (DAD) Python Library
@@ -34,15 +33,15 @@
 ## Install
 
 ```bash
 # Install tool
 pip3 install dad_tool
 
 # Install locally
-make install
+just install
 ```
 
 ## Address Data
 
 Address objects will look like the [sample below](#sample-address-object). The data type of each field on an address object is a `string`. A list of addresses is an `array` of `json` objects.
 
 Attempts have been made to verify addresses and ensure that street1, city, state, and zip are present on all records. Some lists may be shorter than others to avoid complexity or because of a lack of accurate data.
@@ -94,15 +93,14 @@
 | Nevada - Lincoln Area     | US_NV |
 | New York - Rochester Area | US_NY |
 | Oregon - Portland Area    | US_OR |
 | Texas - Austin Area       | US_TX |
 | Utah - Provo Area         | US_UT |
 | Washington - Spokane Area | US_WA |
 
-
 ## Usage
 
 ```python
 import dad_tool
 
 # Grab a random UT address
 address = dad_tool.random_address('US_UT')
@@ -142,18 +140,16 @@
 }
 ```
 
 ## Development
 
 ```bash
 # To setup the `DAD` git submodule
-git submodule init && git submodule update --remote
+just setup-dad
 
 # Get a comprehensive list of development tools
-make help
+just --list
 ```
 
 ## Attribution
 
 - Addresses provided by [DAD](https://github.com/justintime50/dad).
-
-
```

### Comparing `dad-tool-0.3.0/setup.py` & `dad-tool-1.0.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,43 +1,51 @@
 import setuptools
 
+
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 DEV_REQUIREMENTS = [
-    'black',
-    'coveralls == 3.*',
-    'flake8',
-    'isort',
-    'mypy',
+    'bandit == 1.7.*',
+    'black == 23.*',
+    'build == 0.7.*',
+    'flake8 == 6.*',
+    'isort == 5.*',
+    'mypy == 1.3.*',
     'pytest == 7.*',
-    'pytest-cov == 3.*',
+    'pytest-cov == 4.*',
+    'twine == 4.*',
     'types-setuptools',
 ]
 
 setuptools.setup(
     name='dad-tool',
-    version='0.3.0',
+    version='1.0.0',
     description='Dummy Address Data (DAD) - Real addresses from all around the world.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='http://github.com/Justintime50/dad-python',
     author='Justintime50',
     license='MIT',
-    packages=setuptools.find_packages(),
+    packages=setuptools.find_packages(
+        exclude=[
+            'examples',
+            'test',
+        ]
+    ),
+    package_data={
+        'dad_tool': [
+            'dad/src/addresses/**/*.json',
+            'dad/src/other/**/*.json',
+            'py.typed',
+        ],
+    },
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
     extras_require={
         'dev': DEV_REQUIREMENTS,
     },
-    package_data={
-        'dad_tool': [
-            'dad/src/addresses/**/*.json',
-            'dad/src/other/**/*.json',
-            'py.typed',
-        ],
-    },
-    python_requires='>=3.7, <4',
+    python_requires='>=3.8, <4',
 )
```

### Comparing `dad-tool-0.3.0/test/unit/test_data_router.py` & `dad-tool-1.0.0/test/unit/test_data_router.py`

 * *Files identical despite different names*

