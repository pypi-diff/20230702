# Comparing `tmp/warframe.py-0.4.0.tar.gz` & `tmp/warframe.py-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "warframe.py-0.4.0.tar", last modified: Sat Jul  1 12:06:30 2023, max compression
+gzip compressed data, was "warframe.py-0.5.0.tar", last modified: Sun Jul  2 07:38:07 2023, max compression
```

## Comparing `warframe.py-0.4.0.tar` & `warframe.py-0.5.0.tar`

### file list

```diff
@@ -1,48 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 12:06:30.122019 warframe.py-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-07-01 12:05:37.000000 warframe.py-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-07-01 12:06:30.122019 warframe.py-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-07-01 12:05:37.000000 warframe.py-0.4.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-01 12:05:37.000000 warframe.py-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-01 12:06:30.122019 warframe.py-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-07-01 12:05:37.000000 warframe.py-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 12:06:30.114019 warframe.py-0.4.0/warframe/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 12:06:30.118019 warframe.py-0.4.0/warframe/worldstate/
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-01 12:05:37.000000 warframe.py-0.4.0/warframe/worldstate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10385 2023-07-01 12:05:37.000000 warframe.py-0.4.0/warframe/worldstate/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 12:06:30.118019 warframe.py-0.4.0/warframe/worldstate/common/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-01 12:05:37.000000 warframe.py-0.4.0/warframe/worldstate/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-07-01 12:05:37.000000 warframe.py-0.4.0/warframe/worldstate/common/core.py
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-07-01 12:05:37.000000 warframe.py-0.4.0/warframe/worldstate/common/types_.py
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-07-01 12:05:37.000000 warframe.py-0.4.0/warframe/worldstate/endpoints.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 12:06:30.118019 warframe.py-0.4.0/warframe/worldstate/enums/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-01 12:05:37.000000 warframe.py-0.4.0/warframe/worldstate/enums/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-01 12:05:37.000000 warframe.py-0.4.0/warframe/worldstate/enums/faction.py
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-01 12:05:37.000000 warframe.py-0.4.0/warframe/worldstate/enums/language.py
--rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-07-01 12:05:37.000000 warframe.py-0.4.0/warframe/worldstate/enums/mission_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-07-01 12:05:37.000000 warframe.py-0.4.0/warframe/worldstate/enums/syndicate.py
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-07-01 12:05:37.000000 warframe.py-0.4.0/warframe/worldstate/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 12:06:30.122019 warframe.py-0.4.0/warframe/worldstate/models/
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-07-01 12:05:37.000000 warframe.py-0.4.0/warframe/worldstate/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-07-01 12:05:37.000000 warframe.py-0.4.0/warframe/worldstate/models/alert.py
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-01 12:05:37.000000 warframe.py-0.4.0/warframe/worldstate/models/arbitration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-07-01 12:05:37.000000 warframe.py-0.4.0/warframe/worldstate/models/archon_hunt.py
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-01 12:05:37.000000 warframe.py-0.4.0/warframe/worldstate/models/cambion_drift.py
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-07-01 12:05:37.000000 warframe.py-0.4.0/warframe/worldstate/models/cetus.py
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-01 12:05:37.000000 warframe.py-0.4.0/warframe/worldstate/models/counted_item.py
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-01 12:05:37.000000 warframe.py-0.4.0/warframe/worldstate/models/daily_deal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-07-01 12:05:37.000000 warframe.py-0.4.0/warframe/worldstate/models/event.py
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-07-01 12:05:37.000000 warframe.py-0.4.0/warframe/worldstate/models/fissure.py
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-07-01 12:05:37.000000 warframe.py-0.4.0/warframe/worldstate/models/flash_sale.py
--rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-07-01 12:05:37.000000 warframe.py-0.4.0/warframe/worldstate/models/invasion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-07-01 12:05:37.000000 warframe.py-0.4.0/warframe/worldstate/models/mission.py
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-07-01 12:05:37.000000 warframe.py-0.4.0/warframe/worldstate/models/orb_vallis.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-01 12:05:37.000000 warframe.py-0.4.0/warframe/worldstate/models/reward.py
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-01 12:05:37.000000 warframe.py-0.4.0/warframe/worldstate/models/sortie.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-01 12:05:37.000000 warframe.py-0.4.0/warframe/worldstate/models/void_trader.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 12:05:37.000000 warframe.py-0.4.0/warframe/worldstate/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 12:06:30.118019 warframe.py-0.4.0/warframe.py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-07-01 12:06:30.000000 warframe.py-0.4.0/warframe.py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-07-01 12:06:30.000000 warframe.py-0.4.0/warframe.py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 12:06:30.000000 warframe.py-0.4.0/warframe.py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-01 12:06:30.000000 warframe.py-0.4.0/warframe.py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-01 12:06:30.000000 warframe.py-0.4.0/warframe.py.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 07:38:07.117260 warframe.py-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-07-02 07:37:32.000000 warframe.py-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-07-02 07:38:07.117260 warframe.py-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-07-02 07:37:32.000000 warframe.py-0.5.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-02 07:37:32.000000 warframe.py-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-02 07:38:07.117260 warframe.py-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-07-02 07:37:32.000000 warframe.py-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 07:38:07.113260 warframe.py-0.5.0/warframe/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 07:38:07.117260 warframe.py-0.5.0/warframe/worldstate/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-02 07:37:32.000000 warframe.py-0.5.0/warframe/worldstate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10385 2023-07-02 07:37:32.000000 warframe.py-0.5.0/warframe/worldstate/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 07:38:07.117260 warframe.py-0.5.0/warframe/worldstate/common/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-02 07:37:32.000000 warframe.py-0.5.0/warframe/worldstate/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-07-02 07:37:32.000000 warframe.py-0.5.0/warframe/worldstate/common/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-07-02 07:37:32.000000 warframe.py-0.5.0/warframe/worldstate/common/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-07-02 07:37:32.000000 warframe.py-0.5.0/warframe/worldstate/common/types_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-07-02 07:37:32.000000 warframe.py-0.5.0/warframe/worldstate/endpoints.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 07:38:07.117260 warframe.py-0.5.0/warframe/worldstate/enums/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-02 07:37:32.000000 warframe.py-0.5.0/warframe/worldstate/enums/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-02 07:37:32.000000 warframe.py-0.5.0/warframe/worldstate/enums/faction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-02 07:37:32.000000 warframe.py-0.5.0/warframe/worldstate/enums/language.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-07-02 07:37:32.000000 warframe.py-0.5.0/warframe/worldstate/enums/mission_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-07-02 07:37:32.000000 warframe.py-0.5.0/warframe/worldstate/enums/syndicate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-07-02 07:37:32.000000 warframe.py-0.5.0/warframe/worldstate/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 07:38:07.117260 warframe.py-0.5.0/warframe/worldstate/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-07-02 07:37:32.000000 warframe.py-0.5.0/warframe/worldstate/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-07-02 07:37:32.000000 warframe.py-0.5.0/warframe/worldstate/models/alert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-02 07:37:32.000000 warframe.py-0.5.0/warframe/worldstate/models/arbitration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-07-02 07:37:32.000000 warframe.py-0.5.0/warframe/worldstate/models/archon_hunt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-02 07:37:32.000000 warframe.py-0.5.0/warframe/worldstate/models/cambion_drift.py
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-07-02 07:37:32.000000 warframe.py-0.5.0/warframe/worldstate/models/cetus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-02 07:37:32.000000 warframe.py-0.5.0/warframe/worldstate/models/counted_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-02 07:37:32.000000 warframe.py-0.5.0/warframe/worldstate/models/daily_deal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-07-02 07:37:32.000000 warframe.py-0.5.0/warframe/worldstate/models/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-07-02 07:37:32.000000 warframe.py-0.5.0/warframe/worldstate/models/fissure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-07-02 07:37:32.000000 warframe.py-0.5.0/warframe/worldstate/models/flash_sale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-07-02 07:37:32.000000 warframe.py-0.5.0/warframe/worldstate/models/invasion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-07-02 07:37:32.000000 warframe.py-0.5.0/warframe/worldstate/models/mission.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-07-02 07:37:32.000000 warframe.py-0.5.0/warframe/worldstate/models/orb_vallis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-02 07:37:32.000000 warframe.py-0.5.0/warframe/worldstate/models/reward.py
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-02 07:37:32.000000 warframe.py-0.5.0/warframe/worldstate/models/sortie.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-02 07:37:32.000000 warframe.py-0.5.0/warframe/worldstate/models/void_trader.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 07:37:32.000000 warframe.py-0.5.0/warframe/worldstate/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 07:38:07.117260 warframe.py-0.5.0/warframe.py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-07-02 07:38:07.000000 warframe.py-0.5.0/warframe.py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-07-02 07:38:07.000000 warframe.py-0.5.0/warframe.py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 07:38:07.000000 warframe.py-0.5.0/warframe.py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-02 07:38:07.000000 warframe.py-0.5.0/warframe.py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-02 07:38:07.000000 warframe.py-0.5.0/warframe.py.egg-info/top_level.txt
```

### Comparing `warframe.py-0.4.0/LICENSE` & `warframe.py-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `warframe.py-0.4.0/PKG-INFO` & `warframe.py-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: warframe.py
-Version: 0.4.0
+Version: 0.5.0
 Summary: An asynchronous Python API wrapper for the Warframestat API and (later) the warframe.market API.
 Home-page: https://github.com/WFCD/warframe.py
 Author: Mettwasser
 License: MIT
 Keywords: Warframe API worldstate market wrapper
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `warframe.py-0.4.0/README.rst` & `warframe.py-0.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `warframe.py-0.4.0/setup.py` & `warframe.py-0.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `warframe.py-0.4.0/warframe/worldstate/client.py` & `warframe.py-0.5.0/warframe/worldstate/client.py`

 * *Files identical despite different names*

### Comparing `warframe.py-0.4.0/warframe/worldstate/common/core.py` & `warframe.py-0.5.0/warframe/worldstate/common/core.py`

 * *Files identical despite different names*

### Comparing `warframe.py-0.4.0/warframe/worldstate/common/types_.py` & `warframe.py-0.5.0/warframe/worldstate/common/types_.py`

 * *Files identical despite different names*

### Comparing `warframe.py-0.4.0/warframe/worldstate/endpoints.py` & `warframe.py-0.5.0/warframe/worldstate/endpoints.py`

 * *Files identical despite different names*

### Comparing `warframe.py-0.4.0/warframe/worldstate/enums/mission_type.py` & `warframe.py-0.5.0/warframe/worldstate/enums/mission_type.py`

 * *Files identical despite different names*

### Comparing `warframe.py-0.4.0/warframe/worldstate/exceptions.py` & `warframe.py-0.5.0/warframe/worldstate/exceptions.py`

 * *Files identical despite different names*

### Comparing `warframe.py-0.4.0/warframe/worldstate/models/arbitration.py` & `warframe.py-0.5.0/warframe/worldstate/models/arbitration.py`

 * *Files identical despite different names*

### Comparing `warframe.py-0.4.0/warframe/worldstate/models/archon_hunt.py` & `warframe.py-0.5.0/warframe/worldstate/models/archon_hunt.py`

 * *Files identical despite different names*

### Comparing `warframe.py-0.4.0/warframe/worldstate/models/daily_deal.py` & `warframe.py-0.5.0/warframe/worldstate/models/daily_deal.py`

 * *Files identical despite different names*

### Comparing `warframe.py-0.4.0/warframe/worldstate/models/event.py` & `warframe.py-0.5.0/warframe/worldstate/models/event.py`

 * *Files identical despite different names*

### Comparing `warframe.py-0.4.0/warframe/worldstate/models/fissure.py` & `warframe.py-0.5.0/warframe/worldstate/models/fissure.py`

 * *Files identical despite different names*

### Comparing `warframe.py-0.4.0/warframe/worldstate/models/flash_sale.py` & `warframe.py-0.5.0/warframe/worldstate/models/flash_sale.py`

 * *Files identical despite different names*

### Comparing `warframe.py-0.4.0/warframe/worldstate/models/invasion.py` & `warframe.py-0.5.0/warframe/worldstate/models/invasion.py`

 * *Files identical despite different names*

### Comparing `warframe.py-0.4.0/warframe/worldstate/models/mission.py` & `warframe.py-0.5.0/warframe/worldstate/models/mission.py`

 * *Files identical despite different names*

### Comparing `warframe.py-0.4.0/warframe/worldstate/models/reward.py` & `warframe.py-0.5.0/warframe/worldstate/models/reward.py`

 * *Files identical despite different names*

### Comparing `warframe.py-0.4.0/warframe/worldstate/models/sortie.py` & `warframe.py-0.5.0/warframe/worldstate/models/sortie.py`

 * *Files identical despite different names*

### Comparing `warframe.py-0.4.0/warframe/worldstate/models/void_trader.py` & `warframe.py-0.5.0/warframe/worldstate/models/void_trader.py`

 * *Files identical despite different names*

### Comparing `warframe.py-0.4.0/warframe.py.egg-info/PKG-INFO` & `warframe.py-0.5.0/warframe.py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: warframe.py
-Version: 0.4.0
+Version: 0.5.0
 Summary: An asynchronous Python API wrapper for the Warframestat API and (later) the warframe.market API.
 Home-page: https://github.com/WFCD/warframe.py
 Author: Mettwasser
 License: MIT
 Keywords: Warframe API worldstate market wrapper
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `warframe.py-0.4.0/warframe.py.egg-info/SOURCES.txt` & `warframe.py-0.5.0/warframe.py.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 warframe/worldstate/__init__.py
 warframe/worldstate/client.py
 warframe/worldstate/endpoints.py
 warframe/worldstate/exceptions.py
 warframe/worldstate/utils.py
 warframe/worldstate/common/__init__.py
 warframe/worldstate/common/core.py
+warframe/worldstate/common/logger.py
 warframe/worldstate/common/types_.py
 warframe/worldstate/enums/__init__.py
 warframe/worldstate/enums/faction.py
 warframe/worldstate/enums/language.py
 warframe/worldstate/enums/mission_type.py
 warframe/worldstate/enums/syndicate.py
 warframe/worldstate/models/__init__.py
```

