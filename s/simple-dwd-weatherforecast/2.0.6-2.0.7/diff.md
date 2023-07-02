# Comparing `tmp/simple_dwd_weatherforecast-2.0.6.tar.gz` & `tmp/simple_dwd_weatherforecast-2.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple_dwd_weatherforecast-2.0.6.tar", last modified: Fri Jun 30 15:26:59 2023, max compression
+gzip compressed data, was "simple_dwd_weatherforecast-2.0.7.tar", last modified: Sun Jul  2 13:07:20 2023, max compression
```

## Comparing `simple_dwd_weatherforecast-2.0.6.tar` & `simple_dwd_weatherforecast-2.0.7.tar`

### file list

```diff
@@ -1,17 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:26:59.643264 simple_dwd_weatherforecast-2.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-30 15:26:47.000000 simple_dwd_weatherforecast-2.0.6/LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)    10216 2023-06-30 15:26:59.643264 simple_dwd_weatherforecast-2.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9756 2023-06-30 15:26:47.000000 simple_dwd_weatherforecast-2.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 15:26:59.643264 simple_dwd_weatherforecast-2.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-06-30 15:26:47.000000 simple_dwd_weatherforecast-2.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:26:59.639264 simple_dwd_weatherforecast-2.0.6/simple_dwd_weatherforecast/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 15:26:47.000000 simple_dwd_weatherforecast-2.0.6/simple_dwd_weatherforecast/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29920 2023-06-30 15:26:47.000000 simple_dwd_weatherforecast-2.0.6/simple_dwd_weatherforecast/dwdforecast.py
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-06-30 15:26:47.000000 simple_dwd_weatherforecast-2.0.6/simple_dwd_weatherforecast/dwdmap.py
--rw-r--r--   0 runner    (1001) docker     (123)   861420 2023-06-30 15:26:47.000000 simple_dwd_weatherforecast-2.0.6/simple_dwd_weatherforecast/stations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 15:26:59.643264 simple_dwd_weatherforecast-2.0.6/simple_dwd_weatherforecast.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10216 2023-06-30 15:26:59.000000 simple_dwd_weatherforecast-2.0.6/simple_dwd_weatherforecast.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-06-30 15:26:59.000000 simple_dwd_weatherforecast-2.0.6/simple_dwd_weatherforecast.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 15:26:59.000000 simple_dwd_weatherforecast-2.0.6/simple_dwd_weatherforecast.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-30 15:26:59.000000 simple_dwd_weatherforecast-2.0.6/simple_dwd_weatherforecast.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-30 15:26:59.000000 simple_dwd_weatherforecast-2.0.6/simple_dwd_weatherforecast.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:07:20.306471 simple_dwd_weatherforecast-2.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-02 13:07:09.000000 simple_dwd_weatherforecast-2.0.7/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)    10445 2023-07-02 13:07:20.306471 simple_dwd_weatherforecast-2.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9985 2023-07-02 13:07:09.000000 simple_dwd_weatherforecast-2.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 13:07:20.306471 simple_dwd_weatherforecast-2.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-07-02 13:07:09.000000 simple_dwd_weatherforecast-2.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:07:20.302471 simple_dwd_weatherforecast-2.0.7/simple_dwd_weatherforecast/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 13:07:09.000000 simple_dwd_weatherforecast-2.0.7/simple_dwd_weatherforecast/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30450 2023-07-02 13:07:09.000000 simple_dwd_weatherforecast-2.0.7/simple_dwd_weatherforecast/dwdforecast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-07-02 13:07:09.000000 simple_dwd_weatherforecast-2.0.7/simple_dwd_weatherforecast/dwdmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)   861420 2023-07-02 13:07:09.000000 simple_dwd_weatherforecast-2.0.7/simple_dwd_weatherforecast/stations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:07:20.302471 simple_dwd_weatherforecast-2.0.7/simple_dwd_weatherforecast.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10445 2023-07-02 13:07:20.000000 simple_dwd_weatherforecast-2.0.7/simple_dwd_weatherforecast.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-07-02 13:07:20.000000 simple_dwd_weatherforecast-2.0.7/simple_dwd_weatherforecast.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 13:07:20.000000 simple_dwd_weatherforecast-2.0.7/simple_dwd_weatherforecast.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-02 13:07:20.000000 simple_dwd_weatherforecast-2.0.7/simple_dwd_weatherforecast.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-02 13:07:20.000000 simple_dwd_weatherforecast-2.0.7/simple_dwd_weatherforecast.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:07:20.306471 simple_dwd_weatherforecast-2.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 13:07:09.000000 simple_dwd_weatherforecast-2.0.7/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63395 2023-07-02 13:07:09.000000 simple_dwd_weatherforecast-2.0.7/tests/dummy_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-07-02 13:07:09.000000 simple_dwd_weatherforecast-2.0.7/tests/test_get_daily_condition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-07-02 13:07:09.000000 simple_dwd_weatherforecast-2.0.7/tests/test_get_daily_max.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-07-02 13:07:09.000000 simple_dwd_weatherforecast-2.0.7/tests/test_get_daily_min.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-07-02 13:07:09.000000 simple_dwd_weatherforecast-2.0.7/tests/test_get_daily_sum.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28680 2023-07-02 13:07:09.000000 simple_dwd_weatherforecast-2.0.7/tests/test_get_day_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-07-02 13:07:09.000000 simple_dwd_weatherforecast-2.0.7/tests/test_get_forecast_condition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-07-02 13:07:09.000000 simple_dwd_weatherforecast-2.0.7/tests/test_get_forecast_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-07-02 13:07:09.000000 simple_dwd_weatherforecast-2.0.7/tests/test_get_station_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-07-02 13:07:09.000000 simple_dwd_weatherforecast-2.0.7/tests/test_get_timeframe_avg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-07-02 13:07:09.000000 simple_dwd_weatherforecast-2.0.7/tests/test_get_timeframe_condition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-07-02 13:07:09.000000 simple_dwd_weatherforecast-2.0.7/tests/test_get_timeframe_max.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-07-02 13:07:09.000000 simple_dwd_weatherforecast-2.0.7/tests/test_get_timeframe_min.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-07-02 13:07:09.000000 simple_dwd_weatherforecast-2.0.7/tests/test_get_timeframe_sum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6929 2023-07-02 13:07:09.000000 simple_dwd_weatherforecast-2.0.7/tests/test_get_timeframe_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-02 13:07:09.000000 simple_dwd_weatherforecast-2.0.7/tests/test_is_in_timerange.py
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-07-02 13:07:09.000000 simple_dwd_weatherforecast-2.0.7/tests/test_is_valid_timeframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-07-02 13:07:09.000000 simple_dwd_weatherforecast-2.0.7/tests/test_location_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-07-02 13:07:09.000000 simple_dwd_weatherforecast-2.0.7/tests/test_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-02 13:07:09.000000 simple_dwd_weatherforecast-2.0.7/tests/test_parsekml.py
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-07-02 13:07:09.000000 simple_dwd_weatherforecast-2.0.7/tests/test_region.py
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-07-02 13:07:09.000000 simple_dwd_weatherforecast-2.0.7/tests/test_reported_weather.py
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-07-02 13:07:09.000000 simple_dwd_weatherforecast-2.0.7/tests/test_station.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6761 2023-07-02 13:07:09.000000 simple_dwd_weatherforecast-2.0.7/tests/test_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-07-02 13:07:09.000000 simple_dwd_weatherforecast-2.0.7/tests/test_update_hourly.py
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-07-02 13:07:09.000000 simple_dwd_weatherforecast-2.0.7/tests/test_weather.py
```

### Comparing `simple_dwd_weatherforecast-2.0.6/LICENCE` & `simple_dwd_weatherforecast-2.0.7/LICENCE`

 * *Files identical despite different names*

### Comparing `simple_dwd_weatherforecast-2.0.6/PKG-INFO` & `simple_dwd_weatherforecast-2.0.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple_dwd_weatherforecast
-Version: 2.0.6
+Version: 2.0.7
 Summary: A simple tool to retrieve a weather forecast from DWD OpenData
 Home-page: https://github.com/FL550/simple_dwd_weatherforecast.git
 Author: Max Fermor
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
@@ -128,14 +128,16 @@
     get_forecast_condition(datetime, optional bool shouldUpdate) # Result is condition as text
 
     get_daily_condition(datetime, optional bool shouldUpdate) # Result is an approximate "feeled" condition at this day
 
     get_timeframe_condition(datetime, timeframe: hours after datetime as int, optional bool shouldUpdate) # Result is an approximate "feeled" condition at this time frame
 
     get_weather_report(optional bool shouldUpdate) # Returns the weather report for the geographical region of the station as HTML
+
+    update(self, optional bool force_hourly (default: False), optional bool with_forecast (default: True), optional bool with_measurements (default: False), optional bool with_report (default: False)) # Updates the weather data
 ```
 
 #### Advanced Usage
 
 If you want to access the forecast data for the next 10 days directly for further processing, you can do so. All data is stored in dictonary and can be accessed like this:
 
 ```python
```

### Comparing `simple_dwd_weatherforecast-2.0.6/README.md` & `simple_dwd_weatherforecast-2.0.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -115,14 +115,16 @@
     get_forecast_condition(datetime, optional bool shouldUpdate) # Result is condition as text
 
     get_daily_condition(datetime, optional bool shouldUpdate) # Result is an approximate "feeled" condition at this day
 
     get_timeframe_condition(datetime, timeframe: hours after datetime as int, optional bool shouldUpdate) # Result is an approximate "feeled" condition at this time frame
 
     get_weather_report(optional bool shouldUpdate) # Returns the weather report for the geographical region of the station as HTML
+
+    update(self, optional bool force_hourly (default: False), optional bool with_forecast (default: True), optional bool with_measurements (default: False), optional bool with_report (default: False)) # Updates the weather data
 ```
 
 #### Advanced Usage
 
 If you want to access the forecast data for the next 10 days directly for further processing, you can do so. All data is stored in dictonary and can be accessed like this:
 
 ```python
```

### Comparing `simple_dwd_weatherforecast-2.0.6/setup.py` & `simple_dwd_weatherforecast-2.0.7/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="simple_dwd_weatherforecast",
-    version="2.0.6",
+    version="2.0.7",
     author="Max Fermor",
     description="A simple tool to retrieve a weather forecast from DWD OpenData",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/FL550/simple_dwd_weatherforecast.git",
     packages=setuptools.find_packages(),
     package_data={'': ['stations.json']},
```

### Comparing `simple_dwd_weatherforecast-2.0.6/simple_dwd_weatherforecast/dwdforecast.py` & `simple_dwd_weatherforecast-2.0.7/simple_dwd_weatherforecast/dwdforecast.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,34 +35,40 @@
         lon (float): The longitude of the location.
 
     Returns:
         list: A list of stations sorted by distance, where each element is a list containing the station ID and its distance from the location.
     """
     result = []
     for station in stations.items():
-        _lat = station[1]["lat"].split(".")
-        if len(_lat) == 2:
-            _lat = round(float(_lat[0]) + float(_lat[1]) / 60, 2)
-        else:
-            _lat = float(_lat[0])
-        _lon = station[1]["lon"].split(".")
-        if len(_lon) == 2:
-            _lon = round(float(_lon[0]) + float(_lon[1]) / 60, 2)
-        else:
-            _lon = float(_lon[0])
+        _lat = float(station[1]["lat"])
+        _lon = float(station[1]["lon"])
+        # _lat = station[1]["lat"].split(".")
+        # if len(_lat) == 2:
+        #     _lat = round(float(_lat[0]) + float(_lat[1]) / 60, 2)
+        # else:
+        #     _lat = float(_lat[0])
+        # _lon = station[1]["lon"].split(".")
+        # if len(_lon) == 2:
+        #     _lon = round(float(_lon[0]) + float(_lon[1]) / 60, 2)
+        # else:
+        #     _lon = float(_lon[0])
         distance_temp = get_distance(lat, lon, _lat, _lon)
         result.append([station[0], distance_temp])
     result.sort(key=lambda x: x[1])
     return result
 
 
 def get_distance(lat, lon, _lat, _lon):
-    lat_diff = lat - _lat
-    lon_diff = lon - _lon
-    return math.sqrt(math.pow(lat_diff, 2) + math.pow(lon_diff, 2))
+    """Calculate the distance between two points. Result is returned in km."""
+
+    lon_diff = 111.3 * math.cos((lat + _lat) / 2 * 0.01745) * (lon - _lon)
+
+    lat_diff = 111.3 * (lat - _lat)
+
+    return round(math.sqrt(math.pow(lon_diff, 2) + math.pow(lat_diff, 2)), 1)
 
 
 def get_region(station_id: str):
     if (
         station_id in stations.keys()
         and stations[station_id]["bundesland"] in Weather.region_codes.keys()
     ):
@@ -216,15 +222,15 @@
         )
 
     def is_valid_timeframe(_, timeframe: int) -> bool:
         if 24 < timeframe or timeframe <= 0:
             return False
         return 24 % timeframe == 0
 
-    def has_report(self, station_id):
+    def has_measurement(self, station_id):
         if load_station_id(station_id):
             return stations[station_id]["report_available"] == 1
         return False
 
     def get_forecast_data(
         self, weatherDataType: WeatherDataType, timestamp: datetime, shouldUpdate=True
     ):
@@ -324,19 +330,19 @@
 
         if thunder_counter > 0:
             condition_text = "lightning-rainy"
 
         return str(condition_text)
 
     def get_reported_weather(self, weatherDataType: WeatherDataType, shouldUpdate=True):
-        if not self.has_report(self.station_id):
+        if not self.has_measurement(self.station_id):
             print("no report for this station available")
             return None
-        if shouldUpdate:
-            self.update()
+        if shouldUpdate or self.report_data is None:
+            self.update(with_measurements=True)
         if weatherDataType == WeatherDataType.CONDITION:
             return self.actual_report_codes[
                 self.report_data[WeatherDataType.CONDITION.value[0]]
             ]
         else:
             return self.report_data[weatherDataType.value[0]]
 
@@ -533,22 +539,28 @@
 
     def strip_to_hour(_, timestamp: datetime):
         return datetime(timestamp.year, timestamp.month, timestamp.day, timestamp.hour)
 
     def strip_to_day(_, timestamp: datetime):
         return datetime(timestamp.year, timestamp.month, timestamp.day)
 
-    def update(self, force_hourly=False):
-        if self.has_report(self.station_id):
+    def update(
+        self,
+        force_hourly=False,
+        with_forecast=True,
+        with_measurements=False,
+        with_report=False,
+    ):
+        if with_measurements and self.has_measurement(self.station_id):
             self.download_latest_report()
 
-        if self.region is not None:
+        if with_report and self.region is not None:
             self.download_weather_report(self.region_codes[self.region])
 
-        if (
+        if with_forecast and (
             (self.issue_time is None)
             or (datetime.now(timezone.utc) - self.issue_time >= timedelta(hours=6))
             or force_hourly
         ):
             self.download_latest_kml(self.station_id, force_hourly)
 
     def get_weather_type(self, kmlTree, weatherDataType: WeatherDataType):
@@ -753,16 +765,16 @@
                 row[WeatherDataType.HUMIDITY.value[1]].replace(",", ".")
             )
             if row[WeatherDataType.HUMIDITY.value[1]] != "---"
             else None,
         }
 
     def get_weather_report(self, shouldUpdate=False):
-        if shouldUpdate:
-            self.update()
+        if shouldUpdate or self.weather_report is None:
+            self.update(with_report=True)
         return self.weather_report
 
     def download_weather_report(self, region_code):
         url = f"https://www.dwd.de/DWD/wetter/wv_allg/deutschland/text/vhdl13_{region_code}.html"
         headers = {
             "user-agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/89.0.4389.116 Safari/537.36"
         }
```

### Comparing `simple_dwd_weatherforecast-2.0.6/simple_dwd_weatherforecast/dwdmap.py` & `simple_dwd_weatherforecast-2.0.7/simple_dwd_weatherforecast/dwdmap.py`

 * *Files identical despite different names*

### Comparing `simple_dwd_weatherforecast-2.0.6/simple_dwd_weatherforecast/stations.json` & `simple_dwd_weatherforecast-2.0.7/simple_dwd_weatherforecast/stations.json`

 * *Files identical despite different names*

### Comparing `simple_dwd_weatherforecast-2.0.6/simple_dwd_weatherforecast.egg-info/PKG-INFO` & `simple_dwd_weatherforecast-2.0.7/simple_dwd_weatherforecast.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-dwd-weatherforecast
-Version: 2.0.6
+Version: 2.0.7
 Summary: A simple tool to retrieve a weather forecast from DWD OpenData
 Home-page: https://github.com/FL550/simple_dwd_weatherforecast.git
 Author: Max Fermor
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
@@ -128,14 +128,16 @@
     get_forecast_condition(datetime, optional bool shouldUpdate) # Result is condition as text
 
     get_daily_condition(datetime, optional bool shouldUpdate) # Result is an approximate "feeled" condition at this day
 
     get_timeframe_condition(datetime, timeframe: hours after datetime as int, optional bool shouldUpdate) # Result is an approximate "feeled" condition at this time frame
 
     get_weather_report(optional bool shouldUpdate) # Returns the weather report for the geographical region of the station as HTML
+
+    update(self, optional bool force_hourly (default: False), optional bool with_forecast (default: True), optional bool with_measurements (default: False), optional bool with_report (default: False)) # Updates the weather data
 ```
 
 #### Advanced Usage
 
 If you want to access the forecast data for the next 10 days directly for further processing, you can do so. All data is stored in dictonary and can be accessed like this:
 
 ```python
```

