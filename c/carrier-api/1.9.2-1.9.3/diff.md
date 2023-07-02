# Comparing `tmp/carrier_api-1.9.2.tar.gz` & `tmp/carrier_api-1.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "carrier_api-1.9.2.tar", last modified: Fri Apr 14 04:19:11 2023, max compression
+gzip compressed data, was "carrier_api-1.9.3.tar", last modified: Sat Apr 15 11:41:11 2023, max compression
```

## Comparing `carrier_api-1.9.2.tar` & `carrier_api-1.9.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 04:19:11.962215 carrier_api-1.9.2/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1066 2023-04-14 04:18:53.000000 carrier_api-1.9.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-04-14 04:19:11.962215 carrier_api-1.9.2/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     1350 2023-04-14 04:18:53.000000 carrier_api-1.9.2/README.md
--rwxr-xr-x   0 runner    (1001) docker     (123)      104 2023-04-14 04:18:53.000000 carrier_api-1.9.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 04:19:11.962215 carrier_api-1.9.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-04-14 04:19:01.000000 carrier_api-1.9.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 04:19:11.962215 carrier_api-1.9.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 04:19:11.962215 carrier_api-1.9.2/src/carrier_api/
--rwxr-xr-x   0 runner    (1001) docker     (123)      322 2023-04-14 04:18:53.000000 carrier_api-1.9.2/src/carrier_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6617 2023-04-14 04:18:53.000000 carrier_api-1.9.2/src/carrier_api/api_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     6695 2023-04-14 04:18:53.000000 carrier_api-1.9.2/src/carrier_api/config.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      616 2023-04-14 04:18:53.000000 carrier_api-1.9.2/src/carrier_api/const.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      151 2023-04-14 04:18:53.000000 carrier_api-1.9.2/src/carrier_api/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-04-14 04:18:53.000000 carrier_api-1.9.2/src/carrier_api/profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-04-14 04:18:53.000000 carrier_api-1.9.2/src/carrier_api/status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-04-14 04:18:53.000000 carrier_api-1.9.2/src/carrier_api/stub.py
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-04-14 04:18:53.000000 carrier_api-1.9.2/src/carrier_api/system.py
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-04-14 04:18:53.000000 carrier_api-1.9.2/src/carrier_api/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 04:19:11.962215 carrier_api-1.9.2/src/carrier_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-04-14 04:19:11.000000 carrier_api-1.9.2/src/carrier_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-14 04:19:11.000000 carrier_api-1.9.2/src/carrier_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 04:19:11.000000 carrier_api-1.9.2/src/carrier_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-14 04:19:11.000000 carrier_api-1.9.2/src/carrier_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-14 04:19:11.000000 carrier_api-1.9.2/src/carrier_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 11:41:11.727828 carrier_api-1.9.3/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1066 2023-04-15 11:40:51.000000 carrier_api-1.9.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-04-15 11:41:11.727828 carrier_api-1.9.3/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1350 2023-04-15 11:40:51.000000 carrier_api-1.9.3/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)      104 2023-04-15 11:40:51.000000 carrier_api-1.9.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 11:41:11.727828 carrier_api-1.9.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-04-15 11:41:01.000000 carrier_api-1.9.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 11:41:11.723828 carrier_api-1.9.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 11:41:11.723828 carrier_api-1.9.3/src/carrier_api/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      322 2023-04-15 11:40:51.000000 carrier_api-1.9.3/src/carrier_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6617 2023-04-15 11:40:51.000000 carrier_api-1.9.3/src/carrier_api/api_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6695 2023-04-15 11:40:51.000000 carrier_api-1.9.3/src/carrier_api/config.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      616 2023-04-15 11:40:51.000000 carrier_api-1.9.3/src/carrier_api/const.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      151 2023-04-15 11:40:51.000000 carrier_api-1.9.3/src/carrier_api/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-04-15 11:40:51.000000 carrier_api-1.9.3/src/carrier_api/profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5043 2023-04-15 11:40:51.000000 carrier_api-1.9.3/src/carrier_api/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-04-15 11:40:51.000000 carrier_api-1.9.3/src/carrier_api/stub.py
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-04-15 11:40:51.000000 carrier_api-1.9.3/src/carrier_api/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-04-15 11:40:51.000000 carrier_api-1.9.3/src/carrier_api/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 11:41:11.727828 carrier_api-1.9.3/src/carrier_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-04-15 11:41:11.000000 carrier_api-1.9.3/src/carrier_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-15 11:41:11.000000 carrier_api-1.9.3/src/carrier_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 11:41:11.000000 carrier_api-1.9.3/src/carrier_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-15 11:41:11.000000 carrier_api-1.9.3/src/carrier_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-15 11:41:11.000000 carrier_api-1.9.3/src/carrier_api.egg-info/top_level.txt
```

### Comparing `carrier_api-1.9.2/LICENSE` & `carrier_api-1.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `carrier_api-1.9.2/PKG-INFO` & `carrier_api-1.9.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: carrier_api
-Version: 1.9.2
+Version: 1.9.3
 Summary: Carrier Api Wrapper
 Home-page: https://github.com/dahlb/carrier_api
 Author: Brendan Dahl
 Author-email: dahl.brendan@gmail.com
 Project-URL: Bug Reports, https://github.com/dahlb/carrier_api/issues
 Project-URL: Source, https://github.com/dahlb/carrier_api
 Keywords: carrier,api
```

### Comparing `carrier_api-1.9.2/README.md` & `carrier_api-1.9.3/README.md`

 * *Files identical despite different names*

### Comparing `carrier_api-1.9.2/setup.py` & `carrier_api-1.9.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import pathlib
 
 here = pathlib.Path(__file__).parent.resolve()
 
 # Get the long description from the README file
 LONG_DESCRIPTION = (here / "README.md").read_text(encoding="utf-8")
 
-VERSION = "1.9.2"
+VERSION = "1.9.3"
 
 # Setting up
 setup(
     name="carrier_api",
     version=VERSION,
     author="Brendan Dahl",
     author_email="dahl.brendan@gmail.com",
```

### Comparing `carrier_api-1.9.2/src/carrier_api/api_connection.py` & `carrier_api-1.9.3/src/carrier_api/api_connection.py`

 * *Files identical despite different names*

### Comparing `carrier_api-1.9.2/src/carrier_api/config.py` & `carrier_api-1.9.3/src/carrier_api/config.py`

 * *Files identical despite different names*

### Comparing `carrier_api-1.9.2/src/carrier_api/const.py` & `carrier_api-1.9.3/src/carrier_api/const.py`

 * *Files identical despite different names*

### Comparing `carrier_api-1.9.2/src/carrier_api/profile.py` & `carrier_api-1.9.3/src/carrier_api/profile.py`

 * *Files identical despite different names*

### Comparing `carrier_api-1.9.2/src/carrier_api/status.py` & `carrier_api-1.9.3/src/carrier_api/status.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,15 +76,15 @@
 
     def refresh(self):
         self.raw_status_json = self.system.api_connection.get_status(
             system_serial=self.system.serial
         )
         _LOGGER.debug(f"raw_status_json:{self.raw_status_json}")
         self.outdoor_temperature: float = safely_get_json_value(self.raw_status_json, "oat", float)
-        self.mode: str = self.raw_status_json["mode"]
+        self.mode: str = safely_get_json_value(self.raw_status_json, "mode")
         self.temperature_unit: TemperatureUnits = TemperatureUnits(self.raw_status_json["cfgem"])
         self.filter_used: int = safely_get_json_value(self.raw_status_json, "filtrlvl", int)
         self.is_disconnected: bool = safely_get_json_value(self.raw_status_json, "isDisconnected", bool)
         self.airflow_cfm: int = safely_get_json_value(self.raw_status_json, "idu.cfm", int)
         self.outdoor_unit_operational_status: str = safely_get_json_value(self.raw_status_json, "odu.opstat")
         self.indoor_unit_operational_status: str = safely_get_json_value(self.raw_status_json, "idu.opstat")
         self.time_stamp = isoparse(safely_get_json_value(self.raw_status_json, "timestamp"))
```

### Comparing `carrier_api-1.9.2/src/carrier_api/stub.py` & `carrier_api-1.9.3/src/carrier_api/stub.py`

 * *Files identical despite different names*

### Comparing `carrier_api-1.9.2/src/carrier_api/system.py` & `carrier_api-1.9.3/src/carrier_api/system.py`

 * *Files identical despite different names*

### Comparing `carrier_api-1.9.2/src/carrier_api/util.py` & `carrier_api-1.9.3/src/carrier_api/util.py`

 * *Files identical despite different names*

### Comparing `carrier_api-1.9.2/src/carrier_api.egg-info/PKG-INFO` & `carrier_api-1.9.3/src/carrier_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: carrier-api
-Version: 1.9.2
+Version: 1.9.3
 Summary: Carrier Api Wrapper
 Home-page: https://github.com/dahlb/carrier_api
 Author: Brendan Dahl
 Author-email: dahl.brendan@gmail.com
 Project-URL: Bug Reports, https://github.com/dahlb/carrier_api/issues
 Project-URL: Source, https://github.com/dahlb/carrier_api
 Keywords: carrier,api
```

