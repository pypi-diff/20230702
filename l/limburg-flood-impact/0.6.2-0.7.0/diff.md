# Comparing `tmp/limburg_flood_impact-0.6.2.tar.gz` & `tmp/limburg_flood_impact-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "limburg_flood_impact-0.6.2.tar", last modified: Thu Jun 29 14:07:39 2023, max compression
+gzip compressed data, was "limburg_flood_impact-0.7.0.tar", last modified: Sun Jul  2 11:54:32 2023, max compression
```

## Comparing `limburg_flood_impact-0.6.2.tar` & `limburg_flood_impact-0.7.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxr-x   0 cahik     (1000) cahik     (1000)        0 2023-06-29 14:07:39.180768 limburg_flood_impact-0.6.2/
--rw-rw-r--   0 cahik     (1000) cahik     (1000)    12858 2023-06-29 14:07:39.184768 limburg_flood_impact-0.6.2/PKG-INFO
--rw-rw-r--   0 cahik     (1000) cahik     (1000)    12509 2023-06-29 14:07:32.000000 limburg_flood_impact-0.6.2/README.rst
--rw-rw-r--   0 cahik     (1000) cahik     (1000)      149 2023-01-11 11:33:08.000000 limburg_flood_impact-0.6.2/pyproject.toml
--rwxrwxr-x   0 cahik     (1000) cahik     (1000)     1080 2023-06-29 14:07:39.184768 limburg_flood_impact-0.6.2/setup.cfg
--rw-rw-r--   0 cahik     (1000) cahik     (1000)       69 2022-03-23 16:23:16.000000 limburg_flood_impact-0.6.2/setup.py
-drwxrwxr-x   0 cahik     (1000) cahik     (1000)        0 2023-06-29 14:07:39.152767 limburg_flood_impact-0.6.2/src/
-drwxrwxr-x   0 cahik     (1000) cahik     (1000)        0 2023-06-29 14:07:39.156767 limburg_flood_impact-0.6.2/src/limburg_flood_impact/
--rw-rw-r--   0 cahik     (1000) cahik     (1000)      103 2023-02-02 08:42:26.000000 limburg_flood_impact-0.6.2/src/limburg_flood_impact/__init__.py
--rw-rw-r--   0 cahik     (1000) cahik     (1000)    13789 2023-06-16 12:56:54.000000 limburg_flood_impact-0.6.2/src/limburg_flood_impact/_functions.py
-drwxrwxr-x   0 cahik     (1000) cahik     (1000)        0 2023-06-29 14:07:39.180768 limburg_flood_impact-0.6.2/src/limburg_flood_impact/bin/
--rw-rw-r--   0 cahik     (1000) cahik     (1000)        0 2023-01-11 11:38:20.000000 limburg_flood_impact-0.6.2/src/limburg_flood_impact/bin/__init__.py
--rw-rw-r--   0 cahik     (1000) cahik     (1000)     1146 2023-06-16 13:18:40.000000 limburg_flood_impact-0.6.2/src/limburg_flood_impact/bin/check_address.py
--rw-rw-r--   0 cahik     (1000) cahik     (1000)     1182 2023-06-27 06:48:39.000000 limburg_flood_impact-0.6.2/src/limburg_flood_impact/bin/classify_area_wide_rain.py
--rw-rw-r--   0 cahik     (1000) cahik     (1000)     1163 2023-06-27 06:48:48.000000 limburg_flood_impact-0.6.2/src/limburg_flood_impact/bin/classify_rural_rain.py
--rw-rw-r--   0 cahik     (1000) cahik     (1000)     1163 2023-06-27 06:48:58.000000 limburg_flood_impact-0.6.2/src/limburg_flood_impact/bin/classify_urban_rain.py
--rw-rw-r--   0 cahik     (1000) cahik     (1000)      821 2023-06-16 13:19:45.000000 limburg_flood_impact-0.6.2/src/limburg_flood_impact/bin/combine_classification.py
--rw-rw-r--   0 cahik     (1000) cahik     (1000)     1265 2023-06-16 13:20:12.000000 limburg_flood_impact-0.6.2/src/limburg_flood_impact/bin/test_against_flood_protection_norm.py
--rw-rw-r--   0 cahik     (1000) cahik     (1000)     1981 2023-06-16 13:17:41.000000 limburg_flood_impact-0.6.2/src/limburg_flood_impact/check_address.py
--rw-rw-r--   0 cahik     (1000) cahik     (1000)     9992 2023-06-27 06:22:48.000000 limburg_flood_impact-0.6.2/src/limburg_flood_impact/classify_area_wide_rain.py
--rw-rw-r--   0 cahik     (1000) cahik     (1000)     2195 2023-06-27 06:22:44.000000 limburg_flood_impact-0.6.2/src/limburg_flood_impact/classify_rural_rain.py
--rw-rw-r--   0 cahik     (1000) cahik     (1000)     6638 2023-06-27 06:22:53.000000 limburg_flood_impact-0.6.2/src/limburg_flood_impact/classify_urban_rain.py
--rw-rw-r--   0 cahik     (1000) cahik     (1000)     3068 2023-06-29 13:58:16.000000 limburg_flood_impact-0.6.2/src/limburg_flood_impact/combine_classification.py
--rw-rw-r--   0 cahik     (1000) cahik     (1000)     2231 2023-06-16 09:43:54.000000 limburg_flood_impact-0.6.2/src/limburg_flood_impact/extent_tile.py
--rw-rw-r--   0 cahik     (1000) cahik     (1000)     4031 2023-06-16 13:17:41.000000 limburg_flood_impact-0.6.2/src/limburg_flood_impact/test_against_flood_protection_norm.py
-drwxrwxr-x   0 cahik     (1000) cahik     (1000)        0 2023-06-29 14:07:39.180768 limburg_flood_impact-0.6.2/src/limburg_flood_impact.egg-info/
--rw-rw-r--   0 cahik     (1000) cahik     (1000)    12858 2023-06-29 14:07:39.000000 limburg_flood_impact-0.6.2/src/limburg_flood_impact.egg-info/PKG-INFO
--rw-rw-r--   0 cahik     (1000) cahik     (1000)     1170 2023-06-29 14:07:39.000000 limburg_flood_impact-0.6.2/src/limburg_flood_impact.egg-info/SOURCES.txt
--rw-rw-r--   0 cahik     (1000) cahik     (1000)        1 2023-06-29 14:07:39.000000 limburg_flood_impact-0.6.2/src/limburg_flood_impact.egg-info/dependency_links.txt
--rw-rw-r--   0 cahik     (1000) cahik     (1000)      482 2023-06-29 14:07:39.000000 limburg_flood_impact-0.6.2/src/limburg_flood_impact.egg-info/entry_points.txt
--rw-rw-r--   0 cahik     (1000) cahik     (1000)        1 2023-02-08 17:43:18.000000 limburg_flood_impact-0.6.2/src/limburg_flood_impact.egg-info/not-zip-safe
--rw-rw-r--   0 cahik     (1000) cahik     (1000)       11 2023-06-29 14:07:39.000000 limburg_flood_impact-0.6.2/src/limburg_flood_impact.egg-info/requires.txt
--rw-rw-r--   0 cahik     (1000) cahik     (1000)       21 2023-06-29 14:07:39.000000 limburg_flood_impact-0.6.2/src/limburg_flood_impact.egg-info/top_level.txt
+drwxrwxr-x   0 cahik     (1000) cahik     (1000)        0 2023-07-02 11:54:32.015080 limburg_flood_impact-0.7.0/
+-rw-rw-r--   0 cahik     (1000) cahik     (1000)    12858 2023-07-02 11:54:32.015080 limburg_flood_impact-0.7.0/PKG-INFO
+-rw-rw-r--   0 cahik     (1000) cahik     (1000)    12509 2023-07-02 11:54:24.000000 limburg_flood_impact-0.7.0/README.rst
+-rw-rw-r--   0 cahik     (1000) cahik     (1000)      149 2023-01-11 11:33:08.000000 limburg_flood_impact-0.7.0/pyproject.toml
+-rwxrwxr-x   0 cahik     (1000) cahik     (1000)     1080 2023-07-02 11:54:32.019080 limburg_flood_impact-0.7.0/setup.cfg
+-rw-rw-r--   0 cahik     (1000) cahik     (1000)       69 2022-03-23 16:23:16.000000 limburg_flood_impact-0.7.0/setup.py
+drwxrwxr-x   0 cahik     (1000) cahik     (1000)        0 2023-07-02 11:54:31.919080 limburg_flood_impact-0.7.0/src/
+drwxrwxr-x   0 cahik     (1000) cahik     (1000)        0 2023-07-02 11:54:31.991080 limburg_flood_impact-0.7.0/src/limburg_flood_impact/
+-rw-rw-r--   0 cahik     (1000) cahik     (1000)      103 2023-02-02 08:42:26.000000 limburg_flood_impact-0.7.0/src/limburg_flood_impact/__init__.py
+-rw-rw-r--   0 cahik     (1000) cahik     (1000)    13789 2023-06-16 12:56:54.000000 limburg_flood_impact-0.7.0/src/limburg_flood_impact/_functions.py
+drwxrwxr-x   0 cahik     (1000) cahik     (1000)        0 2023-07-02 11:54:32.015080 limburg_flood_impact-0.7.0/src/limburg_flood_impact/bin/
+-rw-rw-r--   0 cahik     (1000) cahik     (1000)        0 2023-01-11 11:38:20.000000 limburg_flood_impact-0.7.0/src/limburg_flood_impact/bin/__init__.py
+-rw-rw-r--   0 cahik     (1000) cahik     (1000)     1146 2023-06-16 13:18:40.000000 limburg_flood_impact-0.7.0/src/limburg_flood_impact/bin/check_address.py
+-rw-rw-r--   0 cahik     (1000) cahik     (1000)     1182 2023-06-27 06:48:39.000000 limburg_flood_impact-0.7.0/src/limburg_flood_impact/bin/classify_area_wide_rain.py
+-rw-rw-r--   0 cahik     (1000) cahik     (1000)     1163 2023-06-27 06:48:48.000000 limburg_flood_impact-0.7.0/src/limburg_flood_impact/bin/classify_rural_rain.py
+-rw-rw-r--   0 cahik     (1000) cahik     (1000)     1163 2023-06-27 06:48:58.000000 limburg_flood_impact-0.7.0/src/limburg_flood_impact/bin/classify_urban_rain.py
+-rw-rw-r--   0 cahik     (1000) cahik     (1000)      821 2023-06-16 13:19:45.000000 limburg_flood_impact-0.7.0/src/limburg_flood_impact/bin/combine_classification.py
+-rw-rw-r--   0 cahik     (1000) cahik     (1000)     1265 2023-06-16 13:20:12.000000 limburg_flood_impact-0.7.0/src/limburg_flood_impact/bin/test_against_flood_protection_norm.py
+-rw-rw-r--   0 cahik     (1000) cahik     (1000)     1981 2023-06-16 13:17:41.000000 limburg_flood_impact-0.7.0/src/limburg_flood_impact/check_address.py
+-rw-rw-r--   0 cahik     (1000) cahik     (1000)     9992 2023-06-27 06:22:48.000000 limburg_flood_impact-0.7.0/src/limburg_flood_impact/classify_area_wide_rain.py
+-rw-rw-r--   0 cahik     (1000) cahik     (1000)     2195 2023-06-27 06:22:44.000000 limburg_flood_impact-0.7.0/src/limburg_flood_impact/classify_rural_rain.py
+-rw-rw-r--   0 cahik     (1000) cahik     (1000)     6638 2023-06-27 06:22:53.000000 limburg_flood_impact-0.7.0/src/limburg_flood_impact/classify_urban_rain.py
+-rw-rw-r--   0 cahik     (1000) cahik     (1000)     3068 2023-06-29 13:58:16.000000 limburg_flood_impact-0.7.0/src/limburg_flood_impact/combine_classification.py
+-rw-rw-r--   0 cahik     (1000) cahik     (1000)     2231 2023-06-16 09:43:54.000000 limburg_flood_impact-0.7.0/src/limburg_flood_impact/extent_tile.py
+-rw-rw-r--   0 cahik     (1000) cahik     (1000)     4031 2023-06-16 13:17:41.000000 limburg_flood_impact-0.7.0/src/limburg_flood_impact/test_against_flood_protection_norm.py
+drwxrwxr-x   0 cahik     (1000) cahik     (1000)        0 2023-07-02 11:54:32.015080 limburg_flood_impact-0.7.0/src/limburg_flood_impact.egg-info/
+-rw-rw-r--   0 cahik     (1000) cahik     (1000)    12858 2023-07-02 11:54:31.000000 limburg_flood_impact-0.7.0/src/limburg_flood_impact.egg-info/PKG-INFO
+-rw-rw-r--   0 cahik     (1000) cahik     (1000)     1170 2023-07-02 11:54:31.000000 limburg_flood_impact-0.7.0/src/limburg_flood_impact.egg-info/SOURCES.txt
+-rw-rw-r--   0 cahik     (1000) cahik     (1000)        1 2023-07-02 11:54:31.000000 limburg_flood_impact-0.7.0/src/limburg_flood_impact.egg-info/dependency_links.txt
+-rw-rw-r--   0 cahik     (1000) cahik     (1000)      482 2023-07-02 11:54:31.000000 limburg_flood_impact-0.7.0/src/limburg_flood_impact.egg-info/entry_points.txt
+-rw-rw-r--   0 cahik     (1000) cahik     (1000)        1 2023-02-08 17:43:18.000000 limburg_flood_impact-0.7.0/src/limburg_flood_impact.egg-info/not-zip-safe
+-rw-rw-r--   0 cahik     (1000) cahik     (1000)       11 2023-07-02 11:54:31.000000 limburg_flood_impact-0.7.0/src/limburg_flood_impact.egg-info/requires.txt
+-rw-rw-r--   0 cahik     (1000) cahik     (1000)       21 2023-07-02 11:54:31.000000 limburg_flood_impact-0.7.0/src/limburg_flood_impact.egg-info/top_level.txt
```

### Comparing `limburg_flood_impact-0.6.2/PKG-INFO` & `limburg_flood_impact-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: limburg_flood_impact
-Version: 0.6.2
+Version: 0.7.0
 Summary: Libmurg Flood Impact Package.
 Home-page: https://github.com/
 Author: Lutra Consulting Ltd.
 Author-email: jan.caha@lutraconsulting.co.uk
 License: MIT
 Project-URL: Documentation, https://
 Platform: any
```

### Comparing `limburg_flood_impact-0.6.2/README.rst` & `limburg_flood_impact-0.7.0/README.rst`

 * *Files identical despite different names*

### Comparing `limburg_flood_impact-0.6.2/setup.cfg` & `limburg_flood_impact-0.7.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = limburg_flood_impact
-version = 0.6.2
+version = 0.7.0
 description = Libmurg Flood Impact Package.
 url = https://github.com/
 project_urls = 
 	Documentation = https://
 author = Lutra Consulting Ltd.
 author_email = jan.caha@lutraconsulting.co.uk
 platforms = any
```

### Comparing `limburg_flood_impact-0.6.2/src/limburg_flood_impact/_functions.py` & `limburg_flood_impact-0.7.0/src/limburg_flood_impact/_functions.py`

 * *Files identical despite different names*

### Comparing `limburg_flood_impact-0.6.2/src/limburg_flood_impact/bin/check_address.py` & `limburg_flood_impact-0.7.0/src/limburg_flood_impact/bin/check_address.py`

 * *Files identical despite different names*

### Comparing `limburg_flood_impact-0.6.2/src/limburg_flood_impact/bin/classify_area_wide_rain.py` & `limburg_flood_impact-0.7.0/src/limburg_flood_impact/bin/classify_area_wide_rain.py`

 * *Files identical despite different names*

### Comparing `limburg_flood_impact-0.6.2/src/limburg_flood_impact/bin/classify_rural_rain.py` & `limburg_flood_impact-0.7.0/src/limburg_flood_impact/bin/classify_rural_rain.py`

 * *Files identical despite different names*

### Comparing `limburg_flood_impact-0.6.2/src/limburg_flood_impact/bin/classify_urban_rain.py` & `limburg_flood_impact-0.7.0/src/limburg_flood_impact/bin/classify_urban_rain.py`

 * *Files identical despite different names*

### Comparing `limburg_flood_impact-0.6.2/src/limburg_flood_impact/bin/combine_classification.py` & `limburg_flood_impact-0.7.0/src/limburg_flood_impact/bin/combine_classification.py`

 * *Files identical despite different names*

### Comparing `limburg_flood_impact-0.6.2/src/limburg_flood_impact/bin/test_against_flood_protection_norm.py` & `limburg_flood_impact-0.7.0/src/limburg_flood_impact/bin/test_against_flood_protection_norm.py`

 * *Files identical despite different names*

### Comparing `limburg_flood_impact-0.6.2/src/limburg_flood_impact/check_address.py` & `limburg_flood_impact-0.7.0/src/limburg_flood_impact/check_address.py`

 * *Files identical despite different names*

### Comparing `limburg_flood_impact-0.6.2/src/limburg_flood_impact/classify_area_wide_rain.py` & `limburg_flood_impact-0.7.0/src/limburg_flood_impact/classify_area_wide_rain.py`

 * *Files identical despite different names*

### Comparing `limburg_flood_impact-0.6.2/src/limburg_flood_impact/classify_rural_rain.py` & `limburg_flood_impact-0.7.0/src/limburg_flood_impact/classify_rural_rain.py`

 * *Files identical despite different names*

### Comparing `limburg_flood_impact-0.6.2/src/limburg_flood_impact/classify_urban_rain.py` & `limburg_flood_impact-0.7.0/src/limburg_flood_impact/classify_urban_rain.py`

 * *Files identical despite different names*

### Comparing `limburg_flood_impact-0.6.2/src/limburg_flood_impact/combine_classification.py` & `limburg_flood_impact-0.7.0/src/limburg_flood_impact/combine_classification.py`

 * *Files identical despite different names*

### Comparing `limburg_flood_impact-0.6.2/src/limburg_flood_impact/extent_tile.py` & `limburg_flood_impact-0.7.0/src/limburg_flood_impact/extent_tile.py`

 * *Files identical despite different names*

### Comparing `limburg_flood_impact-0.6.2/src/limburg_flood_impact/test_against_flood_protection_norm.py` & `limburg_flood_impact-0.7.0/src/limburg_flood_impact/test_against_flood_protection_norm.py`

 * *Files identical despite different names*

### Comparing `limburg_flood_impact-0.6.2/src/limburg_flood_impact.egg-info/PKG-INFO` & `limburg_flood_impact-0.7.0/src/limburg_flood_impact.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: limburg-flood-impact
-Version: 0.6.2
+Version: 0.7.0
 Summary: Libmurg Flood Impact Package.
 Home-page: https://github.com/
 Author: Lutra Consulting Ltd.
 Author-email: jan.caha@lutraconsulting.co.uk
 License: MIT
 Project-URL: Documentation, https://
 Platform: any
```

### Comparing `limburg_flood_impact-0.6.2/src/limburg_flood_impact.egg-info/SOURCES.txt` & `limburg_flood_impact-0.7.0/src/limburg_flood_impact.egg-info/SOURCES.txt`

 * *Files identical despite different names*

