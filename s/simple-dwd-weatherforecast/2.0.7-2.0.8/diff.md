# Comparing `tmp/simple_dwd_weatherforecast-2.0.7.tar.gz` & `tmp/simple_dwd_weatherforecast-2.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple_dwd_weatherforecast-2.0.7.tar", last modified: Sun Jul  2 13:07:20 2023, max compression
+gzip compressed data, was "simple_dwd_weatherforecast-2.0.8.tar", last modified: Sun Jul  2 15:46:33 2023, max compression
```

## Comparing `simple_dwd_weatherforecast-2.0.7.tar` & `simple_dwd_weatherforecast-2.0.8.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:07:20.306471 simple_dwd_weatherforecast-2.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-02 13:07:09.000000 simple_dwd_weatherforecast-2.0.7/LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)    10445 2023-07-02 13:07:20.306471 simple_dwd_weatherforecast-2.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9985 2023-07-02 13:07:09.000000 simple_dwd_weatherforecast-2.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 13:07:20.306471 simple_dwd_weatherforecast-2.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-07-02 13:07:09.000000 simple_dwd_weatherforecast-2.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:07:20.302471 simple_dwd_weatherforecast-2.0.7/simple_dwd_weatherforecast/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 13:07:09.000000 simple_dwd_weatherforecast-2.0.7/simple_dwd_weatherforecast/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30450 2023-07-02 13:07:09.000000 simple_dwd_weatherforecast-2.0.7/simple_dwd_weatherforecast/dwdforecast.py
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-07-02 13:07:09.000000 simple_dwd_weatherforecast-2.0.7/simple_dwd_weatherforecast/dwdmap.py
--rw-r--r--   0 runner    (1001) docker     (123)   861420 2023-07-02 13:07:09.000000 simple_dwd_weatherforecast-2.0.7/simple_dwd_weatherforecast/stations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:07:20.302471 simple_dwd_weatherforecast-2.0.7/simple_dwd_weatherforecast.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10445 2023-07-02 13:07:20.000000 simple_dwd_weatherforecast-2.0.7/simple_dwd_weatherforecast.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-07-02 13:07:20.000000 simple_dwd_weatherforecast-2.0.7/simple_dwd_weatherforecast.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 13:07:20.000000 simple_dwd_weatherforecast-2.0.7/simple_dwd_weatherforecast.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-02 13:07:20.000000 simple_dwd_weatherforecast-2.0.7/simple_dwd_weatherforecast.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-02 13:07:20.000000 simple_dwd_weatherforecast-2.0.7/simple_dwd_weatherforecast.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:07:20.306471 simple_dwd_weatherforecast-2.0.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 13:07:09.000000 simple_dwd_weatherforecast-2.0.7/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    63395 2023-07-02 13:07:09.000000 simple_dwd_weatherforecast-2.0.7/tests/dummy_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-07-02 13:07:09.000000 simple_dwd_weatherforecast-2.0.7/tests/test_get_daily_condition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-07-02 13:07:09.000000 simple_dwd_weatherforecast-2.0.7/tests/test_get_daily_max.py
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-07-02 13:07:09.000000 simple_dwd_weatherforecast-2.0.7/tests/test_get_daily_min.py
--rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-07-02 13:07:09.000000 simple_dwd_weatherforecast-2.0.7/tests/test_get_daily_sum.py
--rw-r--r--   0 runner    (1001) docker     (123)    28680 2023-07-02 13:07:09.000000 simple_dwd_weatherforecast-2.0.7/tests/test_get_day_values.py
--rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-07-02 13:07:09.000000 simple_dwd_weatherforecast-2.0.7/tests/test_get_forecast_condition.py
--rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-07-02 13:07:09.000000 simple_dwd_weatherforecast-2.0.7/tests/test_get_forecast_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-07-02 13:07:09.000000 simple_dwd_weatherforecast-2.0.7/tests/test_get_station_name.py
--rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-07-02 13:07:09.000000 simple_dwd_weatherforecast-2.0.7/tests/test_get_timeframe_avg.py
--rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-07-02 13:07:09.000000 simple_dwd_weatherforecast-2.0.7/tests/test_get_timeframe_condition.py
--rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-07-02 13:07:09.000000 simple_dwd_weatherforecast-2.0.7/tests/test_get_timeframe_max.py
--rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-07-02 13:07:09.000000 simple_dwd_weatherforecast-2.0.7/tests/test_get_timeframe_min.py
--rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-07-02 13:07:09.000000 simple_dwd_weatherforecast-2.0.7/tests/test_get_timeframe_sum.py
--rw-r--r--   0 runner    (1001) docker     (123)     6929 2023-07-02 13:07:09.000000 simple_dwd_weatherforecast-2.0.7/tests/test_get_timeframe_values.py
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-02 13:07:09.000000 simple_dwd_weatherforecast-2.0.7/tests/test_is_in_timerange.py
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-07-02 13:07:09.000000 simple_dwd_weatherforecast-2.0.7/tests/test_is_valid_timeframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-07-02 13:07:09.000000 simple_dwd_weatherforecast-2.0.7/tests/test_location_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-07-02 13:07:09.000000 simple_dwd_weatherforecast-2.0.7/tests/test_map.py
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-02 13:07:09.000000 simple_dwd_weatherforecast-2.0.7/tests/test_parsekml.py
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-07-02 13:07:09.000000 simple_dwd_weatherforecast-2.0.7/tests/test_region.py
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-07-02 13:07:09.000000 simple_dwd_weatherforecast-2.0.7/tests/test_reported_weather.py
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-07-02 13:07:09.000000 simple_dwd_weatherforecast-2.0.7/tests/test_station.py
--rw-r--r--   0 runner    (1001) docker     (123)     6761 2023-07-02 13:07:09.000000 simple_dwd_weatherforecast-2.0.7/tests/test_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-07-02 13:07:09.000000 simple_dwd_weatherforecast-2.0.7/tests/test_update_hourly.py
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-07-02 13:07:09.000000 simple_dwd_weatherforecast-2.0.7/tests/test_weather.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 15:46:33.526230 simple_dwd_weatherforecast-2.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-02 15:46:22.000000 simple_dwd_weatherforecast-2.0.8/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)    10445 2023-07-02 15:46:33.526230 simple_dwd_weatherforecast-2.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9985 2023-07-02 15:46:22.000000 simple_dwd_weatherforecast-2.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 15:46:33.526230 simple_dwd_weatherforecast-2.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-07-02 15:46:22.000000 simple_dwd_weatherforecast-2.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 15:46:33.522230 simple_dwd_weatherforecast-2.0.8/simple_dwd_weatherforecast/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 15:46:22.000000 simple_dwd_weatherforecast-2.0.8/simple_dwd_weatherforecast/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30450 2023-07-02 15:46:22.000000 simple_dwd_weatherforecast-2.0.8/simple_dwd_weatherforecast/dwdforecast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-07-02 15:46:22.000000 simple_dwd_weatherforecast-2.0.8/simple_dwd_weatherforecast/dwdmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)   861420 2023-07-02 15:46:22.000000 simple_dwd_weatherforecast-2.0.8/simple_dwd_weatherforecast/stations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 15:46:33.522230 simple_dwd_weatherforecast-2.0.8/simple_dwd_weatherforecast.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10445 2023-07-02 15:46:33.000000 simple_dwd_weatherforecast-2.0.8/simple_dwd_weatherforecast.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-07-02 15:46:33.000000 simple_dwd_weatherforecast-2.0.8/simple_dwd_weatherforecast.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 15:46:33.000000 simple_dwd_weatherforecast-2.0.8/simple_dwd_weatherforecast.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-02 15:46:33.000000 simple_dwd_weatherforecast-2.0.8/simple_dwd_weatherforecast.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-02 15:46:33.000000 simple_dwd_weatherforecast-2.0.8/simple_dwd_weatherforecast.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 15:46:33.526230 simple_dwd_weatherforecast-2.0.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 15:46:22.000000 simple_dwd_weatherforecast-2.0.8/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63395 2023-07-02 15:46:22.000000 simple_dwd_weatherforecast-2.0.8/tests/dummy_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-07-02 15:46:22.000000 simple_dwd_weatherforecast-2.0.8/tests/test_get_daily_condition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-07-02 15:46:22.000000 simple_dwd_weatherforecast-2.0.8/tests/test_get_daily_max.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-07-02 15:46:22.000000 simple_dwd_weatherforecast-2.0.8/tests/test_get_daily_min.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-07-02 15:46:22.000000 simple_dwd_weatherforecast-2.0.8/tests/test_get_daily_sum.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28680 2023-07-02 15:46:22.000000 simple_dwd_weatherforecast-2.0.8/tests/test_get_day_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-07-02 15:46:22.000000 simple_dwd_weatherforecast-2.0.8/tests/test_get_forecast_condition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-07-02 15:46:22.000000 simple_dwd_weatherforecast-2.0.8/tests/test_get_forecast_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-07-02 15:46:22.000000 simple_dwd_weatherforecast-2.0.8/tests/test_get_station_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-07-02 15:46:22.000000 simple_dwd_weatherforecast-2.0.8/tests/test_get_timeframe_avg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-07-02 15:46:22.000000 simple_dwd_weatherforecast-2.0.8/tests/test_get_timeframe_condition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-07-02 15:46:22.000000 simple_dwd_weatherforecast-2.0.8/tests/test_get_timeframe_max.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-07-02 15:46:22.000000 simple_dwd_weatherforecast-2.0.8/tests/test_get_timeframe_min.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-07-02 15:46:22.000000 simple_dwd_weatherforecast-2.0.8/tests/test_get_timeframe_sum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6929 2023-07-02 15:46:22.000000 simple_dwd_weatherforecast-2.0.8/tests/test_get_timeframe_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-02 15:46:22.000000 simple_dwd_weatherforecast-2.0.8/tests/test_is_in_timerange.py
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-07-02 15:46:22.000000 simple_dwd_weatherforecast-2.0.8/tests/test_is_valid_timeframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-07-02 15:46:22.000000 simple_dwd_weatherforecast-2.0.8/tests/test_location_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-07-02 15:46:22.000000 simple_dwd_weatherforecast-2.0.8/tests/test_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-02 15:46:22.000000 simple_dwd_weatherforecast-2.0.8/tests/test_parsekml.py
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-07-02 15:46:22.000000 simple_dwd_weatherforecast-2.0.8/tests/test_region.py
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-07-02 15:46:22.000000 simple_dwd_weatherforecast-2.0.8/tests/test_reported_weather.py
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-07-02 15:46:22.000000 simple_dwd_weatherforecast-2.0.8/tests/test_station.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6761 2023-07-02 15:46:22.000000 simple_dwd_weatherforecast-2.0.8/tests/test_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-07-02 15:46:22.000000 simple_dwd_weatherforecast-2.0.8/tests/test_update_hourly.py
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-07-02 15:46:22.000000 simple_dwd_weatherforecast-2.0.8/tests/test_weather.py
```

### Comparing `simple_dwd_weatherforecast-2.0.7/LICENCE` & `simple_dwd_weatherforecast-2.0.8/LICENCE`

 * *Files identical despite different names*

### Comparing `simple_dwd_weatherforecast-2.0.7/PKG-INFO` & `simple_dwd_weatherforecast-2.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple_dwd_weatherforecast
-Version: 2.0.7
+Version: 2.0.8
 Summary: A simple tool to retrieve a weather forecast from DWD OpenData
 Home-page: https://github.com/FL550/simple_dwd_weatherforecast.git
 Author: Max Fermor
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `simple_dwd_weatherforecast-2.0.7/README.md` & `simple_dwd_weatherforecast-2.0.8/README.md`

 * *Files identical despite different names*

### Comparing `simple_dwd_weatherforecast-2.0.7/setup.py` & `simple_dwd_weatherforecast-2.0.8/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="simple_dwd_weatherforecast",
-    version="2.0.7",
+    version="2.0.8",
     author="Max Fermor",
     description="A simple tool to retrieve a weather forecast from DWD OpenData",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/FL550/simple_dwd_weatherforecast.git",
     packages=setuptools.find_packages(),
     package_data={'': ['stations.json']},
```

### Comparing `simple_dwd_weatherforecast-2.0.7/simple_dwd_weatherforecast/dwdforecast.py` & `simple_dwd_weatherforecast-2.0.8/simple_dwd_weatherforecast/dwdforecast.py`

 * *Files identical despite different names*

### Comparing `simple_dwd_weatherforecast-2.0.7/simple_dwd_weatherforecast/dwdmap.py` & `simple_dwd_weatherforecast-2.0.8/simple_dwd_weatherforecast/dwdmap.py`

 * *Files identical despite different names*

### Comparing `simple_dwd_weatherforecast-2.0.7/simple_dwd_weatherforecast/stations.json` & `simple_dwd_weatherforecast-2.0.8/simple_dwd_weatherforecast/stations.json`

 * *Files identical despite different names*

### Comparing `simple_dwd_weatherforecast-2.0.7/simple_dwd_weatherforecast.egg-info/PKG-INFO` & `simple_dwd_weatherforecast-2.0.8/simple_dwd_weatherforecast.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-dwd-weatherforecast
-Version: 2.0.7
+Version: 2.0.8
 Summary: A simple tool to retrieve a weather forecast from DWD OpenData
 Home-page: https://github.com/FL550/simple_dwd_weatherforecast.git
 Author: Max Fermor
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `simple_dwd_weatherforecast-2.0.7/simple_dwd_weatherforecast.egg-info/SOURCES.txt` & `simple_dwd_weatherforecast-2.0.8/simple_dwd_weatherforecast.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `simple_dwd_weatherforecast-2.0.7/tests/dummy_data.py` & `simple_dwd_weatherforecast-2.0.8/tests/dummy_data.py`

 * *Files identical despite different names*

### Comparing `simple_dwd_weatherforecast-2.0.7/tests/test_get_daily_condition.py` & `simple_dwd_weatherforecast-2.0.8/tests/test_get_daily_condition.py`

 * *Files identical despite different names*

### Comparing `simple_dwd_weatherforecast-2.0.7/tests/test_get_daily_max.py` & `simple_dwd_weatherforecast-2.0.8/tests/test_get_daily_max.py`

 * *Files identical despite different names*

### Comparing `simple_dwd_weatherforecast-2.0.7/tests/test_get_daily_min.py` & `simple_dwd_weatherforecast-2.0.8/tests/test_get_daily_min.py`

 * *Files identical despite different names*

### Comparing `simple_dwd_weatherforecast-2.0.7/tests/test_get_daily_sum.py` & `simple_dwd_weatherforecast-2.0.8/tests/test_get_daily_sum.py`

 * *Files identical despite different names*

### Comparing `simple_dwd_weatherforecast-2.0.7/tests/test_get_day_values.py` & `simple_dwd_weatherforecast-2.0.8/tests/test_get_day_values.py`

 * *Files identical despite different names*

### Comparing `simple_dwd_weatherforecast-2.0.7/tests/test_get_forecast_condition.py` & `simple_dwd_weatherforecast-2.0.8/tests/test_get_forecast_condition.py`

 * *Files identical despite different names*

### Comparing `simple_dwd_weatherforecast-2.0.7/tests/test_get_forecast_data.py` & `simple_dwd_weatherforecast-2.0.8/tests/test_get_forecast_data.py`

 * *Files identical despite different names*

### Comparing `simple_dwd_weatherforecast-2.0.7/tests/test_get_timeframe_avg.py` & `simple_dwd_weatherforecast-2.0.8/tests/test_get_timeframe_avg.py`

 * *Files identical despite different names*

### Comparing `simple_dwd_weatherforecast-2.0.7/tests/test_get_timeframe_condition.py` & `simple_dwd_weatherforecast-2.0.8/tests/test_get_timeframe_condition.py`

 * *Files identical despite different names*

### Comparing `simple_dwd_weatherforecast-2.0.7/tests/test_get_timeframe_max.py` & `simple_dwd_weatherforecast-2.0.8/tests/test_get_timeframe_max.py`

 * *Files identical despite different names*

### Comparing `simple_dwd_weatherforecast-2.0.7/tests/test_get_timeframe_min.py` & `simple_dwd_weatherforecast-2.0.8/tests/test_get_timeframe_min.py`

 * *Files identical despite different names*

### Comparing `simple_dwd_weatherforecast-2.0.7/tests/test_get_timeframe_sum.py` & `simple_dwd_weatherforecast-2.0.8/tests/test_get_timeframe_sum.py`

 * *Files identical despite different names*

### Comparing `simple_dwd_weatherforecast-2.0.7/tests/test_get_timeframe_values.py` & `simple_dwd_weatherforecast-2.0.8/tests/test_get_timeframe_values.py`

 * *Files identical despite different names*

### Comparing `simple_dwd_weatherforecast-2.0.7/tests/test_is_in_timerange.py` & `simple_dwd_weatherforecast-2.0.8/tests/test_is_in_timerange.py`

 * *Files identical despite different names*

### Comparing `simple_dwd_weatherforecast-2.0.7/tests/test_is_valid_timeframe.py` & `simple_dwd_weatherforecast-2.0.8/tests/test_is_valid_timeframe.py`

 * *Files identical despite different names*

### Comparing `simple_dwd_weatherforecast-2.0.7/tests/test_location_tools.py` & `simple_dwd_weatherforecast-2.0.8/tests/test_location_tools.py`

 * *Files identical despite different names*

### Comparing `simple_dwd_weatherforecast-2.0.7/tests/test_map.py` & `simple_dwd_weatherforecast-2.0.8/tests/test_map.py`

 * *Files identical despite different names*

### Comparing `simple_dwd_weatherforecast-2.0.7/tests/test_region.py` & `simple_dwd_weatherforecast-2.0.8/tests/test_region.py`

 * *Files identical despite different names*

### Comparing `simple_dwd_weatherforecast-2.0.7/tests/test_reported_weather.py` & `simple_dwd_weatherforecast-2.0.8/tests/test_reported_weather.py`

 * *Files identical despite different names*

### Comparing `simple_dwd_weatherforecast-2.0.7/tests/test_station.py` & `simple_dwd_weatherforecast-2.0.8/tests/test_station.py`

 * *Files identical despite different names*

### Comparing `simple_dwd_weatherforecast-2.0.7/tests/test_update.py` & `simple_dwd_weatherforecast-2.0.8/tests/test_update.py`

 * *Files identical despite different names*

### Comparing `simple_dwd_weatherforecast-2.0.7/tests/test_update_hourly.py` & `simple_dwd_weatherforecast-2.0.8/tests/test_update_hourly.py`

 * *Files identical despite different names*

### Comparing `simple_dwd_weatherforecast-2.0.7/tests/test_weather.py` & `simple_dwd_weatherforecast-2.0.8/tests/test_weather.py`

 * *Files identical despite different names*

