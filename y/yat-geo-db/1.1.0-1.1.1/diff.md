# Comparing `tmp/yat_geo_db-1.1.0.tar.gz` & `tmp/yat_geo_db-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yat_geo_db-1.1.0.tar", last modified: Wed Jun 21 22:00:27 2023, max compression
+gzip compressed data, was "yat_geo_db-1.1.1.tar", last modified: Sun Jul  2 13:25:34 2023, max compression
```

## Comparing `yat_geo_db-1.1.0.tar` & `yat_geo_db-1.1.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-06-21 22:00:27.194497 yat_geo_db-1.1.0/
--rw-rw-rw-   0        0        0     1100 2022-12-26 18:53:07.000000 yat_geo_db-1.1.0/LICENSE
--rw-rw-rw-   0        0        0     4944 2023-06-21 22:00:27.193498 yat_geo_db-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     4278 2023-06-21 21:53:49.000000 yat_geo_db-1.1.0/README.md
--rw-rw-rw-   0        0        0      682 2023-06-21 21:35:24.000000 yat_geo_db-1.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-21 22:00:27.194497 yat_geo_db-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0      822 2023-06-21 21:35:28.000000 yat_geo_db-1.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-21 22:00:27.168914 yat_geo_db-1.1.0/yat_geo_db/
--rw-rw-rw-   0        0        0       60 2023-06-21 21:35:33.000000 yat_geo_db-1.1.0/yat_geo_db/__init__.py
--rw-rw-rw-   0        0        0     1011 2022-10-10 16:54:18.000000 yat_geo_db-1.1.0/yat_geo_db/fuzzy.py
--rw-rw-rw-   0        0        0    29558 2023-06-21 21:55:44.000000 yat_geo_db-1.1.0/yat_geo_db/geo_manager.py
--rw-rw-rw-   0        0        0     2321 2022-12-26 17:19:52.000000 yat_geo_db-1.1.0/yat_geo_db/geometry.py
--rw-rw-rw-   0        0        0      107 2022-12-28 17:50:48.000000 yat_geo_db-1.1.0/yat_geo_db/settings.py
--rw-rw-rw-   0        0        0      450 2022-12-26 17:21:13.000000 yat_geo_db-1.1.0/yat_geo_db/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-21 22:00:27.192498 yat_geo_db-1.1.0/yat_geo_db.egg-info/
--rw-rw-rw-   0        0        0     4944 2023-06-21 22:00:27.000000 yat_geo_db-1.1.0/yat_geo_db.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      374 2023-06-21 22:00:27.000000 yat_geo_db-1.1.0/yat_geo_db.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-21 22:00:27.000000 yat_geo_db-1.1.0/yat_geo_db.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2023-06-21 22:00:27.000000 yat_geo_db-1.1.0/yat_geo_db.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-21 22:00:27.000000 yat_geo_db-1.1.0/yat_geo_db.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-01-11 17:08:51.000000 yat_geo_db-1.1.0/yat_geo_db.egg-info/zip-safe
+drwxrwxrwx   0        0        0        0 2023-07-02 13:25:34.157005 yat_geo_db-1.1.1/
+-rw-rw-rw-   0        0        0     1100 2022-12-26 18:53:07.000000 yat_geo_db-1.1.1/LICENSE
+-rw-rw-rw-   0        0        0     4944 2023-07-02 13:25:34.156000 yat_geo_db-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4278 2023-06-30 03:47:21.000000 yat_geo_db-1.1.1/README.md
+-rw-rw-rw-   0        0        0      682 2023-06-30 03:47:28.000000 yat_geo_db-1.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-02 13:25:34.157005 yat_geo_db-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      822 2023-06-30 03:47:28.000000 yat_geo_db-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-02 13:25:34.138428 yat_geo_db-1.1.1/yat_geo_db/
+-rw-rw-rw-   0        0        0       60 2023-06-30 03:47:28.000000 yat_geo_db-1.1.1/yat_geo_db/__init__.py
+-rw-rw-rw-   0        0        0     1011 2022-10-10 16:54:18.000000 yat_geo_db-1.1.1/yat_geo_db/fuzzy.py
+-rw-rw-rw-   0        0        0    30867 2023-06-30 03:47:28.000000 yat_geo_db-1.1.1/yat_geo_db/geo_manager.py
+-rw-rw-rw-   0        0        0     2321 2022-12-26 17:19:52.000000 yat_geo_db-1.1.1/yat_geo_db/geometry.py
+-rw-rw-rw-   0        0        0      107 2022-12-28 17:50:48.000000 yat_geo_db-1.1.1/yat_geo_db/settings.py
+-rw-rw-rw-   0        0        0      450 2022-12-26 17:21:13.000000 yat_geo_db-1.1.1/yat_geo_db/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-02 13:25:34.154993 yat_geo_db-1.1.1/yat_geo_db.egg-info/
+-rw-rw-rw-   0        0        0     4944 2023-07-02 13:25:34.000000 yat_geo_db-1.1.1/yat_geo_db.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      374 2023-07-02 13:25:34.000000 yat_geo_db-1.1.1/yat_geo_db.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-02 13:25:34.000000 yat_geo_db-1.1.1/yat_geo_db.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2023-07-02 13:25:34.000000 yat_geo_db-1.1.1/yat_geo_db.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-02 13:25:34.000000 yat_geo_db-1.1.1/yat_geo_db.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-07-02 13:25:33.000000 yat_geo_db-1.1.1/yat_geo_db.egg-info/zip-safe
```

### Comparing `yat_geo_db-1.1.0/LICENSE` & `yat_geo_db-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `yat_geo_db-1.1.0/PKG-INFO` & `yat_geo_db-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yat_geo_db
-Version: 1.1.0
+Version: 1.1.1
 Summary: A simple and effective Python wrapper around the Open Geo DB managed by YAT
 Home-page: https://github.com/yat-co/yat-geo-db
 Author: YAT, LLC
 Author-email: Robert Goss <rgoss@yat.ai>, Jarod Hart <jhart@yat.ai>
 License: MIT
 Project-URL: Homepage, https://github.com/yat-co/yat-geo-db
 Project-URL: Bug Tracker, https://github.com/yat-co/yat-geo-db/issues
```

### Comparing `yat_geo_db-1.1.0/README.md` & `yat_geo_db-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `yat_geo_db-1.1.0/pyproject.toml` & `yat_geo_db-1.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=42"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "yat_geo_db"
-version = "1.1.0"
+version = "1.1.1"
 authors = [
   { name="Robert Goss", email="rgoss@yat.ai" },
   { name="Jarod Hart", email="jhart@yat.ai" },
 ]
 description = "A simple and effective Python wrapper around the Open Geo DB managed by YAT"
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `yat_geo_db-1.1.0/setup.py` & `yat_geo_db-1.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup
 
 
 install_requires = ['requests', 'numpy', 'jellyfish', 'pytz']
 
 setup(
     name='yat_geo_db',
-    version='1.1.0',
+    version='1.1.1',
     author='YAT, LLC',
     author_email='rgoss@yat.ai, jhart@yat.ai',
     packages=['yat_geo_db'],
     license="MIT",
     url='https://github.com/yat-co/yat-geo-db',
     install_requires=install_requires,
     classifiers=[
```

### Comparing `yat_geo_db-1.1.0/yat_geo_db/fuzzy.py` & `yat_geo_db-1.1.1/yat_geo_db/fuzzy.py`

 * *Files identical despite different names*

### Comparing `yat_geo_db-1.1.0/yat_geo_db/geo_manager.py` & `yat_geo_db-1.1.1/yat_geo_db/geo_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 import os
 import json
 from pathlib import Path
 import pytz
 import re
 import requests
 from statistics import mean
-from typing import Dict, List, Set, Union
+from typing import Dict, List, Optional, Set, Union
 
 
 logger = logging.getLogger(__name__)
 
 
 def geo_damerau_levenshtein_distance(val1, val2):
     return min(
@@ -235,15 +235,15 @@
         return self.radius_search_map.get(reference_code)
 
     def radius_search(self,
                       reference_code,
                       radius,
                       country_exact: bool = False,
                       full_results: bool = False, 
-                      filters: Dict = None):
+                      filters: Dict = None) -> List[Union[int, Dict]]:
         """
         Perform Radius Search by Reference Code
         
         Parameters
         -----------
             reference_code str
                 Geo Reference Code, example `us__tn__nashville`
@@ -266,34 +266,64 @@
         if shape_obj is None:
             return []
 
         country_filter = None
         if country_exact:
             country_filter = shape_obj.get('ref_data', {}).get('country')
 
-        shape_id_ls = self.get_radius_lat_lng_shape_ids(
+        return self.radius_search_lat_lng(
             latitude=shape_obj['latitude'],
             longitude=shape_obj['longitude'],
             radius=radius,
+            reference_code=reference_code,
+            country_filter=country_filter,
+            full_results=full_results,
+            filters=filters
+        )
+
+    def radius_search_lat_lng(self,
+                              latitude: float,
+                              longitude: float,
+                              radius,
+                              reference_code: str = None,
+                              country_filter: str = None,
+                              full_results: bool = False,
+                              filters: Dict = None) -> List[Union[int, Dict]]:
+        shape_id_ls = self.get_radius_lat_lng_shape_ids(
+            latitude=latitude,
+            longitude=longitude,
+            radius=radius,
             country_filter=country_filter,
             filters=filters
         )
 
         # Return full results if parameter specified
         if full_results:
             shape_obj_ls = [
                 self.get_shape_by_id(shape_id) for shape_id in shape_id_ls
             ]
-            
+
             # Add Distance
             for shape_obj in shape_obj_ls:
-                shape_obj.update({
-                    "distance": self.get_shape_pair_distance(reference_code, shape_obj["reference_code"])
-                })
-            
+                if reference_code:
+                    shape_obj.update({
+                        "distance": self.get_shape_pair_distance(reference_code, shape_obj["reference_code"])
+                    })
+                else:
+                    raw_distance = round(lat_lng_dist(
+                        lat_lng_1=(latitude, longitude),
+                        lat_lng_2=(shape_obj["latitude"], shape_obj["longitude"]),
+                    ), 4)
+                    distance = {
+                        "distance": raw_distance,
+                        "normalized_distance": raw_distance,
+                        "aggregate": True
+                    }
+                    shape_obj.update({"distance": distance})
+
             return shape_obj_ls
 
         return shape_id_ls
 
     def get_radius_lat_lng_shape_ids(self,
                                      latitude,
                                      longitude,
@@ -319,27 +349,27 @@
 
     def radius_lat_lng_search(self, latitude, longitude, radius, filters: Dict = None):
         lng_delta = longitude_delta_from_miles(lat=latitude, miles=radius)
         lat_delta = latitude_delta_from_miles(miles=radius)
         res = [
             radius_shape for radius_shape in self.radius_search_map.values()
             if radius_shape.radius_match(
-                latitude = latitude,
-                longitude = longitude,
-                lat_delta = lat_delta,
-                lng_delta = lng_delta
-            ) 
+                latitude=latitude,
+                longitude=longitude,
+                lat_delta=lat_delta,
+                lng_delta=lng_delta
+            )
             and not radius_shape.is_aggregate
             and apply_shape_filters(
                 value=radius_shape.shape_extra, filters=filters
             )
         ]
         return res
 
-    def get_shape_pair_distance(self, orig_shape_ref, dest_shape_ref) -> dict:
+    def get_shape_pair_distance(self, orig_shape_ref, dest_shape_ref) -> Dict:
         """
         Get the distance between two Radius Shape object via `reference_code`
         """
         orig_shape = self.get_radius_shape_by_ref_code(reference_code=orig_shape_ref)
         dest_shape = self.get_radius_shape_by_ref_code(reference_code=dest_shape_ref)
         if orig_shape is None or dest_shape is None:
             logger.warning(
@@ -470,15 +500,15 @@
             return fuzzy_score * .9
         return (fuzzy_score * .9) + (log(population) * .1)
 
     def best_fuzzy_search(self,
                           search_entity: str,
                           partition: str = None,
                           score_threshold: float = .90,
-                          filters: Dict = None) -> Union[Dict, None]:
+                          filters: Dict = None) -> Optional[Dict]:
         """
         Wrapper around fuzzy_search to fetch the best result above a predefined
         threshold.  Intended to be a Best Result Search
         """
         res_ls = self.fuzzy_search(
             search_entity=search_entity, partition=partition, num_results=1,
             filters=filters
```

### Comparing `yat_geo_db-1.1.0/yat_geo_db/geometry.py` & `yat_geo_db-1.1.1/yat_geo_db/geometry.py`

 * *Files identical despite different names*

### Comparing `yat_geo_db-1.1.0/yat_geo_db.egg-info/PKG-INFO` & `yat_geo_db-1.1.1/yat_geo_db.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yat-geo-db
-Version: 1.1.0
+Version: 1.1.1
 Summary: A simple and effective Python wrapper around the Open Geo DB managed by YAT
 Home-page: https://github.com/yat-co/yat-geo-db
 Author: YAT, LLC
 Author-email: Robert Goss <rgoss@yat.ai>, Jarod Hart <jhart@yat.ai>
 License: MIT
 Project-URL: Homepage, https://github.com/yat-co/yat-geo-db
 Project-URL: Bug Tracker, https://github.com/yat-co/yat-geo-db/issues
```

