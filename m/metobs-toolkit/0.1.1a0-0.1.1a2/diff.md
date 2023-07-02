# Comparing `tmp/metobs_toolkit-0.1.1a0.tar.gz` & `tmp/metobs_toolkit-0.1.1a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metobs_toolkit-0.1.1a0.tar", max compression
+gzip compressed data, was "metobs_toolkit-0.1.1a2.tar", max compression
```

## Comparing `metobs_toolkit-0.1.1a0.tar` & `metobs_toolkit-0.1.1a2.tar`

### file list

```diff
@@ -1,58 +1,41 @@
--rw-r--r--   0        0        0     1074 2022-09-22 07:29:20.660989 metobs_toolkit-0.1.1a0/LICENSE
--rw-r--r--   0        0        0      403 2023-05-10 06:57:22.583568 metobs_toolkit-0.1.1a0/README.md
--rw-r--r--   0        0        0      222 2023-05-17 14:33:54.259368 metobs_toolkit-0.1.1a0/metobs_toolkit/GUI/cache/custom_template.csv
--rw-r--r--   0        0        0      485 2023-05-17 14:33:54.259368 metobs_toolkit-0.1.1a0/metobs_toolkit/GUI/cache/custom_template_Ian.csv
--rw-r--r--   0        0        0      295 2023-05-17 14:33:54.259368 metobs_toolkit-0.1.1a0/metobs_toolkit/GUI/cache/vlindersmall_template.csv
--rw-r--r--   0        0        0      160 2023-05-17 14:33:54.259368 metobs_toolkit-0.1.1a0/metobs_toolkit/GUI/cache/wow_template.csv
--rw-r--r--   0        0        0     1426 2023-05-17 14:33:54.259368 metobs_toolkit-0.1.1a0/metobs_toolkit/GUI/data_func.py
--rw-r--r--   0        0        0      825 2023-05-17 14:33:54.259368 metobs_toolkit-0.1.1a0/metobs_toolkit/GUI/errors.py
--rw-r--r--   0        0        0     4857 2023-05-17 14:33:54.259368 metobs_toolkit-0.1.1a0/metobs_toolkit/GUI/extra_windows.py
--rw-r--r--   0        0        0     3369 2023-05-17 14:33:54.259368 metobs_toolkit-0.1.1a0/metobs_toolkit/GUI/fig_window.ui
--rw-r--r--   0        0        0     2323 2023-05-17 14:33:54.259368 metobs_toolkit-0.1.1a0/metobs_toolkit/GUI/figuremodel.py
--rw-r--r--   0        0        0     2029 2023-05-17 14:33:54.259368 metobs_toolkit-0.1.1a0/metobs_toolkit/GUI/json_save_func.py
--rw-r--r--   0        0        0    11180 2023-05-17 14:33:54.259368 metobs_toolkit-0.1.1a0/metobs_toolkit/GUI/main.py
--rw-r--r--   0        0        0     1435 2023-05-17 14:33:54.263368 metobs_toolkit-0.1.1a0/metobs_toolkit/GUI/merge_overview.ui
--rw-r--r--   0        0        0     2367 2023-05-17 14:33:54.263368 metobs_toolkit-0.1.1a0/metobs_toolkit/GUI/pandasmodel.py
--rw-r--r--   0        0        0     2288 2023-05-17 14:33:54.263368 metobs_toolkit-0.1.1a0/metobs_toolkit/GUI/path_handler.py
--rw-r--r--   0        0        0      283 2023-05-17 14:33:54.263368 metobs_toolkit-0.1.1a0/metobs_toolkit/GUI/save_gui_vals.json
--rw-r--r--   0        0        0    46804 2023-05-17 14:33:54.263368 metobs_toolkit-0.1.1a0/metobs_toolkit/GUI/templ_build.ui
--rw-r--r--   0        0        0    11554 2023-05-17 14:33:54.263368 metobs_toolkit-0.1.1a0/metobs_toolkit/GUI/template_func.py
--rw-r--r--   0        0        0     7330 2023-05-17 14:33:54.263368 metobs_toolkit-0.1.1a0/metobs_toolkit/GUI/tlk_scripts.py
--rw-r--r--   0        0        0     2503 2023-05-22 09:08:00.896066 metobs_toolkit-0.1.1a0/metobs_toolkit/__init__.py
--rw-r--r--   0        0        0    19751 2023-05-12 09:54:16.821478 metobs_toolkit-0.1.1a0/metobs_toolkit/analysis.py
--rw-r--r--   0        0        0     2566 2023-05-10 06:57:22.695567 metobs_toolkit-0.1.1a0/metobs_toolkit/convertors.py
--rw-r--r--   0        0        0    12056 2023-05-12 09:54:16.821478 metobs_toolkit-0.1.1a0/metobs_toolkit/data_import.py
--rw-r--r--   0        0        0     2378 2023-05-10 06:57:22.695567 metobs_toolkit-0.1.1a0/metobs_toolkit/data_templates/db_templates.py
--rw-r--r--   0        0        0     1701 2023-05-12 09:54:16.821478 metobs_toolkit-0.1.1a0/metobs_toolkit/data_templates/import_templates.py
--rw-r--r--   0        0        0      931 2023-05-10 06:57:22.695567 metobs_toolkit-0.1.1a0/metobs_toolkit/data_templates/template_defaults/default_template.csv
--rwxr-xr-x   0        0        0  9062298 2023-05-12 09:54:16.849478 metobs_toolkit-0.1.1a0/metobs_toolkit/datafiles/demo_datafile.csv
--rw-r--r--   0        0        0     2306 2023-05-12 09:54:16.853478 metobs_toolkit-0.1.1a0/metobs_toolkit/datafiles/demo_metadatafile.csv
--rw-r--r--   0        0        0      931 2023-05-12 09:54:16.853478 metobs_toolkit-0.1.1a0/metobs_toolkit/datafiles/demo_templatefile.csv
--rw-r--r--   0        0        0    84881 2023-05-22 09:06:31.996064 metobs_toolkit-0.1.1a0/metobs_toolkit/dataset.py
--rw-r--r--   0        0        0    18352 2023-05-17 07:20:37.243724 metobs_toolkit-0.1.1a0/metobs_toolkit/dataset_settings_updater.py
--rw-r--r--   0        0        0    13810 2023-05-17 14:33:54.263368 metobs_toolkit-0.1.1a0/metobs_toolkit/df_helpers.py
--rw-r--r--   0        0        0    24294 2023-05-17 14:33:54.263368 metobs_toolkit-0.1.1a0/metobs_toolkit/gap.py
--rw-r--r--   0        0        0    17104 2023-05-17 14:33:54.263368 metobs_toolkit-0.1.1a0/metobs_toolkit/gap_filling.py
--rw-r--r--   0        0        0      673 2023-05-10 06:57:22.727566 metobs_toolkit-0.1.1a0/metobs_toolkit/geometry_functions.py
--rw-r--r--   0        0        0      222 2023-05-17 14:33:54.263368 metobs_toolkit-0.1.1a0/metobs_toolkit/gui_launcher.py
--rw-r--r--   0        0        0    18380 2023-05-17 14:33:54.263368 metobs_toolkit-0.1.1a0/metobs_toolkit/landcover_functions.py
--rw-r--r--   0        0        0     9081 2023-05-17 14:33:54.263368 metobs_toolkit-0.1.1a0/metobs_toolkit/missingobs.py
--rw-r--r--   0        0        0     5078 2023-05-17 07:20:37.243724 metobs_toolkit-0.1.1a0/metobs_toolkit/modeldata.py
--rw-r--r--   0        0        0    22849 2023-05-22 06:55:48.035309 metobs_toolkit-0.1.1a0/metobs_toolkit/plotting_functions.py
--rw-r--r--   0        0        0     1847 2023-05-12 09:54:16.853478 metobs_toolkit-0.1.1a0/metobs_toolkit/printing.py
--rw-r--r--   0        0        0    22903 2023-05-10 06:57:22.727566 metobs_toolkit-0.1.1a0/metobs_toolkit/qc_checks.py
--rw-r--r--   0        0        0     3978 2023-05-17 07:20:37.243724 metobs_toolkit-0.1.1a0/metobs_toolkit/qc_statistics.py
--rw-r--r--   0        0        0    14130 2023-05-17 07:20:37.243724 metobs_toolkit-0.1.1a0/metobs_toolkit/settings.py
--rw-r--r--   0        0        0       73 2023-05-10 06:57:22.727566 metobs_toolkit-0.1.1a0/metobs_toolkit/settings_files/app_print_settings.json
--rw-r--r--   0        0        0      225 2023-05-17 07:20:37.247724 metobs_toolkit-0.1.1a0/metobs_toolkit/settings_files/dataset_resolution_settings.json
--rw-r--r--   0        0        0     4599 2023-05-17 15:04:21.765513 metobs_toolkit-0.1.1a0/metobs_toolkit/settings_files/default_formats_settings.py
--rw-r--r--   0        0        0     1888 2023-05-17 07:20:37.247724 metobs_toolkit-0.1.1a0/metobs_toolkit/settings_files/gaps_and_missing_settings.py
--rw-r--r--   0        0        0     3880 2023-05-22 06:55:48.035309 metobs_toolkit-0.1.1a0/metobs_toolkit/settings_files/gee_settings.py
--rw-r--r--   0        0        0     2851 2023-05-12 09:54:16.853478 metobs_toolkit-0.1.1a0/metobs_toolkit/settings_files/qc_settings.py
--rw-r--r--   0        0        0      132 2023-05-10 06:57:22.727566 metobs_toolkit-0.1.1a0/metobs_toolkit/settings_files/server_login.json
--rw-r--r--   0        0        0  8385556 2023-05-10 06:57:22.787565 metobs_toolkit-0.1.1a0/metobs_toolkit/settings_files/world_boundaries/WB_countries_Admin0_10m.shp
--rw-r--r--   0        0        0     2108 2023-05-10 06:57:22.787565 metobs_toolkit-0.1.1a0/metobs_toolkit/settings_files/world_boundaries/WB_countries_Admin0_10m.shx
--rw-r--r--   0        0        0      916 2023-05-12 09:54:16.853478 metobs_toolkit-0.1.1a0/metobs_toolkit/station.py
--rw-r--r--   0        0        0     2269 2023-05-17 07:20:37.247724 metobs_toolkit-0.1.1a0/metobs_toolkit/writing_files.py
--rw-r--r--   0        0        0      933 2023-05-22 09:08:00.776065 metobs_toolkit-0.1.1a0/pyproject.toml
--rw-r--r--   0        0        0     1576 1970-01-01 00:00:00.000000 metobs_toolkit-0.1.1a0/PKG-INFO
+-rw-r--r--   0        0        0     1074 2022-09-22 07:29:20.660989 metobs_toolkit-0.1.1a2/LICENSE
+-rw-r--r--   0        0        0      403 2023-05-26 07:21:12.529777 metobs_toolkit-0.1.1a2/README.md
+-rw-r--r--   0        0        0     2538 2023-07-02 12:00:01.776759 metobs_toolkit-0.1.1a2/metobs_toolkit/__init__.py
+-rw-r--r--   0        0        0    47956 2023-07-02 11:55:51.772193 metobs_toolkit-0.1.1a2/metobs_toolkit/analysis.py
+-rw-r--r--   0        0        0     3323 2023-07-02 11:55:51.772193 metobs_toolkit-0.1.1a2/metobs_toolkit/convertors.py
+-rw-r--r--   0        0        0    14941 2023-07-02 11:55:51.772193 metobs_toolkit-0.1.1a2/metobs_toolkit/data_import.py
+-rw-r--r--   0        0        0     2378 2023-05-26 07:21:12.633777 metobs_toolkit-0.1.1a2/metobs_toolkit/data_templates/db_templates.py
+-rw-r--r--   0        0        0     1444 2023-05-26 07:21:12.633777 metobs_toolkit-0.1.1a2/metobs_toolkit/data_templates/import_templates.py
+-rw-r--r--   0        0        0    23974 2023-06-20 12:08:41.643275 metobs_toolkit-0.1.1a2/metobs_toolkit/data_templates/template_build_prompt.py
+-rw-r--r--   0        0        0      771 2023-05-26 07:21:12.633777 metobs_toolkit-0.1.1a2/metobs_toolkit/data_templates/template_defaults/default_template.csv
+-rwxr-xr-x   0        0        0  9062298 2023-05-26 07:21:12.665777 metobs_toolkit-0.1.1a2/metobs_toolkit/datafiles/demo_datafile.csv
+-rw-r--r--   0        0        0     2306 2023-05-26 07:21:12.665777 metobs_toolkit-0.1.1a2/metobs_toolkit/datafiles/demo_metadatafile.csv
+-rw-r--r--   0        0        0      931 2023-05-26 07:21:12.669777 metobs_toolkit-0.1.1a2/metobs_toolkit/datafiles/demo_templatefile.csv
+-rw-r--r--   0        0        0   117650 2023-07-02 11:55:51.772193 metobs_toolkit-0.1.1a2/metobs_toolkit/dataset.py
+-rw-r--r--   0        0        0    28550 2023-07-02 09:50:57.553108 metobs_toolkit-0.1.1a2/metobs_toolkit/dataset_settings_updater.py
+-rw-r--r--   0        0        0    16035 2023-07-02 11:55:51.772193 metobs_toolkit-0.1.1a2/metobs_toolkit/df_helpers.py
+-rw-r--r--   0        0        0    27167 2023-07-02 11:55:51.776193 metobs_toolkit-0.1.1a2/metobs_toolkit/gap.py
+-rw-r--r--   0        0        0    16319 2023-07-02 11:55:51.776193 metobs_toolkit-0.1.1a2/metobs_toolkit/gap_filling.py
+-rw-r--r--   0        0        0     1924 2023-06-27 14:58:53.388937 metobs_toolkit-0.1.1a2/metobs_toolkit/geometry_functions.py
+-rw-r--r--   0        0        0    18899 2023-07-02 11:55:51.776193 metobs_toolkit-0.1.1a2/metobs_toolkit/landcover_functions.py
+-rw-r--r--   0        0        0    12643 2023-07-02 07:43:41.838492 metobs_toolkit-0.1.1a2/metobs_toolkit/missingobs.py
+-rw-r--r--   0        0        0    31156 2023-07-02 11:55:51.776193 metobs_toolkit-0.1.1a2/metobs_toolkit/modeldata.py
+-rw-r--r--   0        0        0    37698 2023-07-02 11:55:51.776193 metobs_toolkit-0.1.1a2/metobs_toolkit/plotting_functions.py
+-rw-r--r--   0        0        0     1449 2023-07-01 07:36:36.792836 metobs_toolkit-0.1.1a2/metobs_toolkit/printing.py
+-rw-r--r--   0        0        0    31085 2023-07-02 11:55:51.776193 metobs_toolkit-0.1.1a2/metobs_toolkit/qc_checks.py
+-rw-r--r--   0        0        0     3978 2023-05-26 07:21:12.669777 metobs_toolkit-0.1.1a2/metobs_toolkit/qc_statistics.py
+-rw-r--r--   0        0        0    13918 2023-07-02 11:55:51.776193 metobs_toolkit-0.1.1a2/metobs_toolkit/settings.py
+-rw-r--r--   0        0        0     1416 2023-07-01 07:36:36.792836 metobs_toolkit-0.1.1a2/metobs_toolkit/settings_files/alaro_25_settings.py
+-rw-r--r--   0        0        0       73 2023-05-26 07:21:12.669777 metobs_toolkit-0.1.1a2/metobs_toolkit/settings_files/app_print_settings.json
+-rw-r--r--   0        0        0      225 2023-05-26 07:21:12.669777 metobs_toolkit-0.1.1a2/metobs_toolkit/settings_files/dataset_resolution_settings.json
+-rw-r--r--   0        0        0     5900 2023-06-30 13:30:05.539095 metobs_toolkit-0.1.1a2/metobs_toolkit/settings_files/default_formats_settings.py
+-rw-r--r--   0        0        0     1888 2023-05-26 07:21:12.669777 metobs_toolkit-0.1.1a2/metobs_toolkit/settings_files/gaps_and_missing_settings.py
+-rw-r--r--   0        0        0     4199 2023-05-26 07:21:12.669777 metobs_toolkit-0.1.1a2/metobs_toolkit/settings_files/gee_settings.py
+-rw-r--r--   0        0        0     5981 2023-06-20 12:08:41.651275 metobs_toolkit-0.1.1a2/metobs_toolkit/settings_files/qc_settings.py
+-rw-r--r--   0        0        0      132 2023-05-26 07:21:12.673777 metobs_toolkit-0.1.1a2/metobs_toolkit/settings_files/server_login.json
+-rw-r--r--   0        0        0  8385556 2023-05-26 07:21:12.733777 metobs_toolkit-0.1.1a2/metobs_toolkit/settings_files/world_boundaries/WB_countries_Admin0_10m.shp
+-rw-r--r--   0        0        0     2108 2023-05-26 07:21:12.733777 metobs_toolkit-0.1.1a2/metobs_toolkit/settings_files/world_boundaries/WB_countries_Admin0_10m.shx
+-rw-r--r--   0        0        0      998 2023-06-22 13:50:31.966358 metobs_toolkit-0.1.1a2/metobs_toolkit/station.py
+-rw-r--r--   0        0        0     2439 2023-07-02 11:55:51.776193 metobs_toolkit-0.1.1a2/metobs_toolkit/writing_files.py
+-rw-r--r--   0        0        0      969 2023-07-02 12:00:01.696759 metobs_toolkit-0.1.1a2/pyproject.toml
+-rw-r--r--   0        0        0     1534 1970-01-01 00:00:00.000000 metobs_toolkit-0.1.1a2/PKG-INFO
```

### Comparing `metobs_toolkit-0.1.1a0/LICENSE` & `metobs_toolkit-0.1.1a2/LICENSE`

 * *Files identical despite different names*

### Comparing `metobs_toolkit-0.1.1a0/metobs_toolkit/__init__.py` & `metobs_toolkit-0.1.1a2/metobs_toolkit/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -64,21 +64,21 @@
 # =============================================================================
 
 from metobs_toolkit.dataset import Dataset
 from metobs_toolkit.station import Station
 from metobs_toolkit.modeldata import Modeldata
 
 # import GUI
-from metobs_toolkit.gui_launcher import launch_gui
+from metobs_toolkit.data_templates.template_build_prompt import build_template_prompt
 
 # =============================================================================
 # Import extenders
 # =============================================================================
 from metobs_toolkit.dataset_settings_updater import Dataset
 
 # =============================================================================
 # Version
 # =============================================================================
 
 # DO not change this manually!
-__version__ = "0.1.1a0"
+__version__ = "0.1.1a2"
```

### Comparing `metobs_toolkit-0.1.1a0/metobs_toolkit/convertors.py` & `metobs_toolkit-0.1.1a2/metobs_toolkit/convertors.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,25 +3,47 @@
 """
 Created on Fri Feb 24 09:34:00 2023
 
 @author: thoverga
 """
 
 import sys
+import logging
 import numpy as np
 from collections.abc import Iterable
 
+logger = logging.getLogger(__name__)
+
+
 # =============================================================================
 # Unit defenitions and coversions
 # =============================================================================
 # Keys are the toolkit-units!! (not persee SI)
 # values expresions are of the form x $ val, where x is the numeric value,
 # $ an operator (+-*/) and val a concersion value
 unit_convertors = {
     "Celsius": {"K": "x - 273.15"},
+    'pa':{'pa' : 'x'}
+}
+
+# =============================================================================
+# Standard units
+# =============================================================================
+standard_tlk_units = {
+    "temp": 'Celsius',
+    "radiation_temp": 'Celcius',
+    "humidity": '%',
+    "precip": 'mm/m² per hour',
+    "precip_sum" : 'mm/m² from midnight',
+    "wind_speed" : 'm/s',
+    "wind_gust": 'm/s',
+    "wind_direction": '° from north (CW)',
+    "pressure" : 'pa',
+    "pressure_at_sea_level": 'pa',
+
 }
 
 
 # =============================================================================
 # Convert functions
 # =============================================================================
 
@@ -42,15 +64,15 @@
     elif "*" in equation:
         y = equation.split("*")
         return x * float(y[1])
     else:
         sys.exit(f"expression {equation}, can not be converted to mathematical.")
 
 
-def convert_to_toolkit_units(data, data_unit):
+def convert_to_toolkit_units(data, data_unit, new_units={}):
     """
     Convert the data to the toolkit perfered unit. Data can be a numeric value or an iterable.
     Data_unit is the unit of the input data.
 
     The converted data AND the corresponding toolkit unit is returned.
 
     Parameters
@@ -64,16 +86,20 @@
     -------
     numeric, numpy.array
         The data in toolkit units.
     String
         Corresponding toolkit unit name.
 
     """
+    # update the units
+    unit_convertors.update(new_units)
+
     # check if unit is already a toolkit unit
     if data_unit in unit_convertors.keys():
+        logger.info(f'Current unit ({data_unit}) is already the default, no coversion needed!')
         return data, data_unit
 
     # scan the units to find conversion
     expr = {
         toolk_unit: other_unit[data_unit]
         for toolk_unit, other_unit in unit_convertors.items()
         if data_unit in other_unit.keys()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `metobs_toolkit-0.1.1a0/metobs_toolkit/data_import.py` & `metobs_toolkit-0.1.1a2/metobs_toolkit/data_import.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,22 +2,26 @@
 # -*- coding: utf-8 -*-
 """
 Created on Thu Sep 22 16:24:06 2022
 
 @author: thoverga
 """
 import sys
-
+import warnings
+import logging
 import pandas as pd
 
 import mysql.connector
 from mysql.connector import errorcode
 from metobs_toolkit.df_helpers import init_multiindexdf
 from metobs_toolkit.data_templates.import_templates import read_csv_template
 
+from metobs_toolkit import observation_types
+
+logger = logging.getLogger(__name__)
 
 def template_to_package_space(specific_template):
     returndict = {
         val["varname"]: {"orig_name": key} for key, val in specific_template.items()
     }
     for key, item in returndict.items():
         orig_dict = dict(specific_template[item["orig_name"]])
@@ -26,15 +30,15 @@
     return returndict
 
 
 def find_compatible_templatefor(df_columns, template_list):
     for templ in template_list:
         found = all(keys in list(df_columns) for keys in templ.keys())
         if found:
-            print("Compatible template found. ")
+            logger.info("Compatible template found. ")
             return templ
     sys.exit("No compatible teplate found!")
 
 
 def compress_dict(nested_dict, valuesname):
     """
     This function unnests a nested dictionary for a specific valuename that is a key in the nested dict.
@@ -59,170 +63,242 @@
     returndict = {}
     for key, item in nested_dict.items():
         if valuesname in item:
             returndict[key] = item[valuesname]
     return returndict
 
 
-def check_template_compatibility(template, df_columns):
-    # test if all df_columns are in template keys
-    if not all(col in template.keys() for col in df_columns):
-        unmapped = list(set(df_columns) - set(template.keys()))
-        print(
-            f"WARNING! The following columns are not pressent in the template,\
-              and cannot be mapped: {unmapped}"
+def check_template_compatibility(template, df_columns, filetype):
+    # ignore datetime because this is already mapped
+    present_cols = [col for col in df_columns if col != 'datetime']
+    assumed_cols = [key for key in template.keys() if key != 'datetime']
+
+    # in mapper but not in df
+    unmapped_assumed = [templ_var for templ_var in assumed_cols if not templ_var in present_cols]
+
+    if len(unmapped_assumed) > 0:
+        logger.info(
+            f"The following columns are not present in the {filetype},\
+ and cannot be mapped: {unmapped_assumed}"
         )
 
-    if len(list(set(df_columns) - set(template.keys()))) == len(df_columns):
+    # in df but not in mapper
+    unmapped_appearing = [col for col in present_cols if col not in assumed_cols]
+    if len(unmapped_appearing) > 0:
+        logger.info(
+            f"The following columns in the {filetype} cannot be mapped with the template: {unmapped_appearing}.")
+
+    # check if at least one column is mapped
+    if len(list(set(present_cols) - set(assumed_cols))) == len(present_cols):
         sys.exit(
-            f"Fatal: The given template does not match with any of the data columns."
+            f"Fatal: The given template: {assumed_cols} does not match with any of the {filetype} columns: {present_cols}."
         )
 
 
-def import_metadata_from_csv(input_file, template_file):
-    common_seperators = [";", ",", "    ", "."]
+
+def import_metadata_from_csv(input_file, template_file, kwargs_metadata_read):
+
+
     assert not isinstance(input_file, type(None)), "Specify input file in the settings!"
-    for sep in common_seperators:
-        df = pd.read_csv(input_file, sep=sep)
-        assert not df.empty, "Dataset is empty!"
 
-        if len(df.columns) > 1:
-            break
+    with warnings.catch_warnings():
+        warnings.simplefilter("ignore")
+        if bool(kwargs_metadata_read):
+            df = pd.read_csv(filepath_or_buffer=input_file, **kwargs_metadata_read)
+        else:
+            common_seperators = [None, ";", ",", "    ", "."]
+            for sep in common_seperators:
+                df = pd.read_csv(input_file, sep=sep)
+                assert not df.empty, "Dataset is empty!"
+
+                if len(df.columns) > 1:
+                    break
 
     assert (
         len(df.columns) > 1
     ), f"Only one column detected from import using these seperators: {common_seperators}. See if csv template is correct."
 
     # validate template
     template = read_csv_template(template_file)
-    check_template_compatibility(template, df.columns)
+    check_template_compatibility(template, df.columns, filetype='metadata')
 
     # rename columns to toolkit attriute names
     df = df.rename(columns=compress_dict(template, "varname"))
 
     return df
-def wide_to_long(df, template, obstype):
 
-    print('Converting wide data to long')
-    mapped_colnames = [val['varname'] for val in template.values()]
-    data_colnames = [col for col in df.columns if not col in mapped_colnames]
-    longdf = pd.melt(df, id_vars=['Tijd'], value_vars=data_colnames,
-                   var_name='name', value_name=obstype)
-
-    # update template
-    template[obstype] = template['_wide_dummy']
-    del template['_wide_dummy']
 
-    template['name'] = {'varname': 'name', 'dtype':'object'}
 
-    return longdf, template
 
+def wide_to_long(df, template, obstype):
+
+    # the df is assumed to have one datetime column, and the others represent
+    # stations with their obstype values
 
+    stationnames = df.columns.to_list()
+    stationnames.remove('datetime')
 
-def wide_to_long(df, template, obstype):
-    print("Converting wide data to long")
-    mapped_colnames = [val["varname"] for val in template.values()]
-    data_colnames = [col for col in df.columns if not col in mapped_colnames]
     longdf = pd.melt(
         df,
-        id_vars=["Tijd"],
-        value_vars=data_colnames,
+        id_vars=["datetime"],
+        value_vars=stationnames,
         var_name="name",
         value_name=obstype,
     )
 
-    # update template
-    template[obstype] = template["_wide_dummy"]
-    del template["_wide_dummy"]
+    # # update template
+    # template[obstype] = template["_wide_dummy"]
+    # del template["_wide_dummy"]
 
+    # add name to the template
     template["name"] = {"varname": "name", "dtype": "object"}
 
     return longdf, template
 
-
-
-def import_data_from_csv(input_file, template_file, long_format, obstype):
-    common_seperators = [";", ",", "    ", "."]
-    assert not isinstance(input_file, type(None)), "Specify input file in the settings!"
-    for sep in common_seperators:
-        df = pd.read_csv(input_file, sep=sep)
-        assert not df.empty, "Dataset is empty!"
-
-        if len(df.columns) > 1:
-            break
-
-    assert (
-        len(df.columns) > 1
-    ), f"Only one column detected from import using these seperators: {common_seperators}. See if csv template is correct."
+def _read_csv_file(path, kwargsdict):
+    """ a helper function to read in csv data files, try multiple seperators, and
+        remove header text. """
+    with warnings.catch_warnings():
+        warnings.simplefilter("ignore")
+
+        if bool(kwargsdict):
+            df = pd.read_csv(filepath_or_buffer=path, **kwargsdict)
+        else:
+            common_seperators = [None, ";", ",", "    ", "."]
+            assert not isinstance(path, type(None)), "Specify input file in the settings!"
+            for sep in common_seperators:
+                df = pd.read_csv(path, sep=sep)
+                assert not df.empty, "Dataset is empty!"
+
+                if len(df.columns) > 1:
+                    break
+
+        assert (
+            len(df.columns) > 1
+        ), f"Only one column detected from import using these seperators: {common_seperators}. See if csv template is correct."
 
     # LINES TO DEAL WITH RANDOM PIECES OF TEXT BEFORE ACTUAL MEASUREMENTS
     if True in df.columns.str.contains(pat="Unnamed"):
         num_columns = df.iloc[-3].count().sum()
 
         rows_to_skip = 0
         for row in range(len(df)):
             if df.iloc[row : (row + 1), :].count().sum() != num_columns:
                 rows_to_skip += 1
             else:
                 break
         df = df.iloc[rows_to_skip:, :]
         df = df.rename(columns=df.iloc[0]).iloc[1:, :]
     df.index = range(len(df))
+    return df
 
-    # validate template
-    template = read_csv_template(template_file, long_format, obstype)
-    # convert wide data to long if needed
-    if not long_format:
-        df, template = wide_to_long(df, template, obstype)
-
-    check_template_compatibility(template, df.columns)
+def _remove_keys_from_dict(dictionary, keys):
+    for key in keys:
+        dictionary.pop(key, None)
+    return dictionary
 
 
+def import_data_from_csv(input_file, template_file,
+                         long_format, obstype,
+                         obstype_units, obstype_description,
+                         kwargs_data_read):
 
-    for key, value in template.items():
-        if value["dtype"] == "float64":
-            df[key] = pd.to_numeric(df[key], errors="coerce")
+    """ Wrapper data import function for long and wide"""
 
-    # rename columns to toolkit attriute names
-    df = df.rename(columns=compress_dict(template, "varname"))
+    # 1. Read data into df
+    df = _read_csv_file(input_file, kwargs_data_read)
 
-    # COnvert template to package-space
+    # 2. Read template
+    template = read_csv_template(template_file, long_format, obstype)
     invtemplate = template_to_package_space(template)
 
-    # format columns
-    # df = df.astype(dtype=compress_dict(template, 'dtype'))
+    # 3. Make datetime column (needed for wide to long conversion)
+    if ('datetime' in invtemplate.keys()):
 
-    if "datetime" in df.columns:
-        df["datetime"] = pd.to_datetime(
-            df["datetime"], format=invtemplate["datetime"]["format"]
-        )
+        df = df.rename(columns={invtemplate['datetime']['orig_name'] : 'datetime'})
+        df['datetime'] = pd.to_datetime(df["datetime"],
+                                        format=invtemplate["datetime"]["format"])
+
+        inv_temp_remove_keys = ['datetime']
+        temp_remove_keys = [invtemplate['datetime']['orig_name']]
+    elif (('_date' in invtemplate.keys()) & ('_time' in invtemplate.keys())):
 
-    else:
         datetime_fmt = (
             invtemplate["_date"]["format"] + " " + invtemplate["_time"]["format"]
         )
         df["datetime"] = pd.to_datetime(
-            df["_date"] + " " + df["_time"], format=datetime_fmt
+            df[invtemplate['_date']['orig_name']] + " " + df[invtemplate['_time']['orig_name']], format=datetime_fmt
         )
-        df = df.drop(columns=["_date", "_time"])
+        df = df.drop(columns=[invtemplate['_date']['orig_name'], invtemplate['_time']['orig_name']])
 
-    # Set datetime index
-    df = df.set_index("datetime", drop=True, verify_integrity=False)
-    # TODO implement timezone settings
+        inv_temp_remove_keys = ['_time', '_date']
+        temp_remove_keys = [invtemplate['_date']['orig_name'],
+                            invtemplate['_time']['orig_name']]
+    else:
+        sys.exit('Impossible to map the dataset to a datetime column, verify your template please.')
 
-    # Keep only columns as defined in the template
-    for column in df.columns:
-        if not (column in invtemplate.keys()):
-            df = df.drop(columns=[column])
+    # 3.b Remove the datetime keys from the template
+
+    invtemplate = _remove_keys_from_dict(invtemplate, inv_temp_remove_keys)
+    template = _remove_keys_from_dict(template, temp_remove_keys)
 
-    # add template to the return
 
+
+    # 4. convert wide data to long if needed
+    if not long_format:
+
+        template[obstype] = {}
+        invtemplate[obstype] = {}
+        template[obstype]['varname'] = obstype
+        invtemplate[obstype]['orig_name'] = obstype #use default as orig name
+        if not obstype_units is None:
+            template[obstype]['units'] = obstype_units
+            invtemplate[obstype]['units'] = obstype_units
+        if not obstype_description is None:
+            template[obstype]['description'] = obstype_description
+            invtemplate[obstype]['description'] = obstype_description
+
+        df, template = wide_to_long(df, template, obstype)
+
+
+    # 5. check compatibility
+    check_template_compatibility(template, df.columns, filetype='data')
+
+
+    # 6. map to default name space
+    df = df.rename(columns=compress_dict(template, "varname"))
+
+    # 7. Keep only columns as defined in the template
+    cols_to_keep = list(invtemplate.keys())
+    cols_to_keep.append('datetime')
+    cols_to_keep.append('name')
+    cols_to_keep = list(set(cols_to_keep))
+    df = df.loc[:,df.columns.isin(cols_to_keep)]
+
+
+
+    # 8. Set index
+    df = df.reset_index()
+    df = df.drop(columns=['index'], errors='ignore')
+    df = df.set_index('datetime')
+
+    # 8. map to numeric dtypes
+    for col in df.columns:
+        if col in observation_types:
+            df[col] = pd.to_numeric(df[col], errors='coerce')
+        if col in ['lon', 'lat']:
+            df[col] = pd.to_numeric(df[col], errors='coerce')
+
+
+    # add template to the return
     return df, invtemplate
 
 
+
+
 # %%
 def import_data_from_db(db_settings, start_datetime, end_datetime):
     # =============================================================================
     # Make connection to database
     # =============================================================================
 
     # Make connection with database (needs ugent VPN active)
@@ -372,8 +448,8 @@
         combdata["datetime"], format=datetime_db_info["fmt"]
     )
     # TODO implement timezone settings
 
     # Set datetime index
     combdata = combdata.set_index("datetime", drop=True, verify_integrity=False)
 
-    return combdata
+    return combdata
```

### Comparing `metobs_toolkit-0.1.1a0/metobs_toolkit/data_templates/db_templates.py` & `metobs_toolkit-0.1.1a2/metobs_toolkit/data_templates/db_templates.py`

 * *Files identical despite different names*

### Comparing `metobs_toolkit-0.1.1a0/metobs_toolkit/data_templates/import_templates.py` & `metobs_toolkit-0.1.1a2/metobs_toolkit/data_templates/import_templates.py`

 * *Files 17% similar despite different names*

```diff
@@ -36,19 +36,14 @@
     # Drop emty rows
     templ = templ.dropna(axis="index", how="all")
 
     if data_long_format:
         # Drop variables that are not present in templ
         templ = templ[templ["template column name"].notna()]
 
-    else:
-        # Do not do this for wide dataframes since the present obstype
-        # is not specified in template oclumn name, but the defenition and datatype do.
-        templ.loc[templ["varname"] == obstype, "template column name"] = "_wide_dummy"
-
 
     # create dictionary from templframe
     templ = templ.set_index("template column name")
 
     # create a dict from the dataframe, remove Nan value row wise
     template = {}
     for idx, row in templ.iterrows():
```

### Comparing `metobs_toolkit-0.1.1a0/metobs_toolkit/data_templates/template_defaults/default_template.csv` & `metobs_toolkit-0.1.1a2/metobs_toolkit/datafiles/demo_templatefile.csv`

 * *Files identical despite different names*

### Comparing `metobs_toolkit-0.1.1a0/metobs_toolkit/datafiles/demo_datafile.csv` & `metobs_toolkit-0.1.1a2/metobs_toolkit/datafiles/demo_datafile.csv`

 * *Files identical despite different names*

### Comparing `metobs_toolkit-0.1.1a0/metobs_toolkit/datafiles/demo_metadatafile.csv` & `metobs_toolkit-0.1.1a2/metobs_toolkit/datafiles/demo_metadatafile.csv`

 * *Files identical despite different names*

### Comparing `metobs_toolkit-0.1.1a0/metobs_toolkit/dataset.py` & `metobs_toolkit-0.1.1a2/metobs_toolkit/dataset.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 """
-The class object for a Vlinder/mocca station
-@author: thoverga
+This module contains the Dataset class and all its methods.
+
+A Dataset holds all observations and is at the center of the
+MetObs-toolkit.
 """
 
 import os
 import copy
 from datetime import datetime
 import pytz
 import logging
 import pandas as pd
 import numpy as np
+import pickle
+
 
 
 from metobs_toolkit.settings import Settings
 from metobs_toolkit.data_import import (
     import_data_from_csv,
     import_data_from_db,
     template_to_package_space,
@@ -24,61 +28,68 @@
 
 from metobs_toolkit.printing import print_dataset_info
 from metobs_toolkit.landcover_functions import (
     connect_to_gee,
     lcz_extractor,
     height_extractor,
     lc_fractions_extractor,
+    _validate_metadf
 )
 
 from metobs_toolkit.plotting_functions import (
     geospatial_plot,
     timeseries_plot,
     qc_stats_pie,
+    folium_plot,
+    add_stations_to_folium_map,
 )
 
 from metobs_toolkit.qc_checks import (
     gross_value_check,
     persistance_check,
     repetitions_check,
     duplicate_timestamp_check,
     step_check,
     window_variation_check,
     invalid_input_check,
+    titan_buddy_check,
+    titan_sct_resistant_check
 )
 
 
 from metobs_toolkit.qc_statistics import get_freq_statistics
 from metobs_toolkit.writing_files import write_dataset_to_csv
 
 from metobs_toolkit.missingobs import Missingob_collection
 
 from metobs_toolkit.gap import (
     Gap,
     remove_gaps_from_obs,
+    remove_gaps_from_outliers,
     missing_timestamp_and_gap_check,
     get_gaps_indx_in_obs_space,
     get_station_gaps,
     apply_interpolate_gaps,
     make_gapfill_df,
     apply_debias_era5_gapfill,
     gaps_to_df,
 )
 
 
 from metobs_toolkit.df_helpers import (
     multiindexdf_datetime_subsetting,
-    remove_outliers_from_obs,
+    fmt_datetime_argument,
     init_multiindex,
     init_multiindexdf,
     init_triple_multiindexdf,
     metadf_to_gdf,
     conv_applied_qc_to_df,
     get_freqency_series,
     value_labeled_doubleidxdf_to_triple_idxdf,
+    xs_save
 )
 
 from metobs_toolkit.analysis import Analysis
 from metobs_toolkit.modeldata import Modeldata
 
 from metobs_toolkit import observation_types
 
@@ -124,36 +135,294 @@
 
         self.settings = copy.deepcopy(Settings())
 
 
 
     def __str__(self):
         if self.df.empty:
-            return f"Empty instance of a Dataset."
+            if self._istype == 'Dataset':
+                return f"Empty instance of a Dataset."
+            else:
+                return f"Empty instance of a Station."
         add_info = ''
         n_stations = self.df.index.get_level_values('name').unique().shape[0]
         n_obs_tot = self.df.shape[0]
         n_outl = self.outliersdf.shape[0]
+        startdt = self.df.index.get_level_values('datetime').min()
+        enddt = self.df.index.get_level_values('datetime').max()
+
 
         if ((not self.metadf['lat'].isnull().all()) &
             (not self.metadf['lon'].isnull().all())):
-            add_info += '     *Coordinates are available for all stations. \n'
+            add_info += '    *Coordinates are available for all stations. \n'
 
 
         return (f"Dataset instance containing: \n \
     *{n_stations} stations \n \
+    *{self.df.columns.to_list()} observation types \n \
     *{n_obs_tot} observation records \n \
     *{n_outl} records labeled as outliers \n \
     *{len(self.gaps)} gaps \n \
-    *{self.missing_obs.series.shape[0]} missing observations \n" + add_info)
-
+    *{self.missing_obs.series.shape[0]} missing observations \n \
+    *records range: {startdt} --> {enddt} (total duration:  {enddt - startdt}) \n \
+    *time zone of the records: {self.settings.time_settings['timezone']} \n " + add_info)
     def __repr__(self):
         return self.__str__()
 
 
+    def __add__(self, other, gapsize=None):
+
+        # important !!!!!
+
+        # the toolkit makes a new dataframe, and assumes the df from self and other
+        # to be the input data.
+        # This means that missing obs, gaps, invalid and duplicated records are
+        # being looked for in the concatenation of both dataset, using their current
+        # resolution !
+
+
+
+
+
+
+        new = Dataset()
+
+
+        self_obstypes = self.df.columns.to_list().copy()
+        #  ---- df ----
+
+        # check if observation of self are also in other
+        assert all([(obs in other.df.columns) for obs in self_obstypes])
+        # subset obstype of other to self
+        other.df = other.df[self.df.columns.to_list()]
+
+        #remove duplicate rows
+        common_indexes = self.df.index.intersection(other.df.index)
+        other.df=other.df.drop(common_indexes)
+
+        # set new df
+        new.df = pd.concat([self.df, other.df])
+        new.df = new.df.sort_index()
+
+
+        #  ----- outliers df ---------
+
+
+        other_outliers = other.outliersdf.reset_index()
+        other_outliers = other_outliers[other_outliers['obstype'].isin(self_obstypes)]
+        other_outliers = other_outliers.set_index(['name', 'datetime', 'obstype'])
+        new.outliersdf = pd.concat([self.outliersdf, other_outliers])
+        new.outliersdf = new.outliersdf.sort_index()
+
+        #  ------- Gaps -------------
+        # Gaps have to be recaluculated using a frequency assumtion from the
+        # combination of self.df and other.df, thus NOT the native frequency if
+        # their is a coarsening allied on either of them.
+        new.gaps = []
+
+
+        # ---------- missing ---------
+        # Missing observations have to be recaluculated using a frequency assumtion from the
+        # combination of self.df and other.df, thus NOT the native frequency if
+        # their is a coarsening allied on either of them.
+        new.missing_obs = None
+
+        # ---------- metadf -----------
+        # Use the metadf from self and add new rows if they are present in other
+        new.metadf = pd.concat([self.metadf, other.metadf])
+        new.metadf = new.metadf.drop_duplicates(keep='first')
+        new.metadf = new.metadf.sort_index()
+
+        # ------- specific attributes ----------
+
+        # Template (units and descritpions) are taken from self
+        new.data_template = self.data_template
+
+        # Inherit Settings from self
+        new.settings = copy.deepcopy(self.settings)
+
+
+        # Applied qc:
+        # TODO:  is this oke to do?
+        new._applied_qc = pd.DataFrame(columns=["obstype", "checkname"])
+        new._qc_checked_obstypes = []  # list with qc-checked obstypes
+
+
+        # set init_dataframe to empty
+        #NOTE: this is not necesarry but users will use this method when they
+        # have a datafile that is to big. So storing and overloading a copy of
+        # the very big datafile is invalid for these cases.
+        new.input_df = pd.DataFrame()
+
+
+        # ----- Apply IO QC ---------
+        # Apply only checks that are relevant on records in between self and other
+        # OR
+        # that are dependand on the frequency (since the freq of the .df is used,
+        # which is not the naitive frequency if coarsening is applied on either. )
+
+
+        # missing and gap check
+        if gapsize is None:
+            gapsize =new.settings.gap["gaps_settings"]["gaps_finder"]["gapsize_n"]
+
+        # note gapsize is now defined on the frequency of self
+        new.missing_obs, new.gaps =  missing_timestamp_and_gap_check(
+            df=new.df,
+            gapsize_n=self.settings.gap["gaps_settings"]["gaps_finder"]["gapsize_n"],
+        )
+
+
+        # duplicate check
+        new.df, dup_outl_df = duplicate_timestamp_check(
+            df=new.df,
+            checks_info=new.settings.qc["qc_checks_info"],
+            checks_settings=new.settings.qc["qc_check_settings"],
+        )
+
+        if not dup_outl_df.empty:
+            new.update_outliersdf(add_to_outliersdf=dup_outl_df)
+
+        # update the order and which qc is applied on which obstype
+        checked_obstypes = [obs for obs in new.df.columns if obs in observation_types]
+
+        checknames = ["duplicated_timestamp"]  # KEEP order
+
+        new._applied_qc = pd.concat(
+            [
+                new._applied_qc,
+                conv_applied_qc_to_df(
+                    obstypes=checked_obstypes, ordered_checknames=checknames
+                ),
+            ],
+            ignore_index=True,
+        )
+
+
+
+        return new
+
+    def show(self, show_all_settings=False, max_disp_n_gaps = 5):
+        """
+        A function to print out a detailed overview information about the Dataset.
+
+        Parameters
+        ----------
+        show_all_settings : bool, optional
+            If True all the settings are printed out. The default is False.
+
+        Returns
+        -------
+        None.
+
+        """
+
+        logger.info("Show basic info of dataset.")
+
+        print_dataset_info(self, show_all_settings)
+
+    def get_info(self, show_all_settings=False, max_disp_n_gaps = 5):
+        """
+        (alias of .show() method)
+        A function to print out a detailed overview information about the Dataset.
+
+        Parameters
+        ----------
+        show_all_settings : bool, optional
+            If True all the settings are printed out. The default is False.
+
+        Returns
+        -------
+        None.
+
+        """
+        self.show(show_all_settings, max_disp_n_gaps)
+
+
+    def save_dataset(self, outputfolder=None, filename='saved_dataset.pkl'):
+        """
+        Method to save a Dataset instance to a (pickle) file.
+
+        Parameters
+        ----------
+        outputfolder : str or None, optional
+            The path to the folder to save the file. If None, the outputfolder
+            from the Settings is used. The default is None.
+        filename : str, optional
+            The name of the output file. The default is 'saved_dataset.pkl'.
+
+        Returns
+        -------
+        None.
+
+        """
+
+        # check if outputfolder is known and exists
+        if outputfolder is None:
+            outputfolder = self.settings.IO['output_folder']
+            assert not outputfolder is None, 'No outputfolder is given, and no outputfolder is found in the settings.'
+
+        assert os.path.isdir(outputfolder), f'{outputfolder} is not a directory!'
+
+        # check file extension in the filename:
+        if filename[-4:] != '.pkl':
+            filename += '.pkl'
+
+        full_path = os.path.join(outputfolder, filename)
+
+        # check if file exists
+        assert not os.path.isfile(full_path), f'{full_path} is already a file!'
+
+        with open(full_path, 'wb') as outp:
+            pickle.dump(self, outp, pickle.HIGHEST_PROTOCOL)
+
+        print(f'Dataset saved in {full_path}')
+        logger.info(f'Dataset saved in {full_path}')
+
+
+
+    def import_dataset(self, folder_path=None, filename='saved_dataset.pkl'):
+        """
+        Method to import a Dataset instance from a (pickle) file.
+
+        Parameters
+        ----------
+        folder_path : str or None, optional
+            The path to the folder to save the file. If None, the outputfolder
+            from the Settings is used. The default is None.
+        filename : str, optional
+            The name of the output file. The default is 'saved_dataset.pkl'.
+
+        Returns
+        -------
+        metobs_toolkit.Dataset
+            The Dataset instance.
+
+        """
+
+        # check if folder_path is known and exists
+        if folder_path is None:
+            folder_path = self.settings.IO['output_folder']
+            assert not folder_path is None, 'No folder_path is given, and no outputfolder is found in the settings.'
+
+        assert os.path.isdir(folder_path), f'{folder_path} is not a directory!'
+
+        full_path = os.path.join(folder_path, filename)
+
+        # check if file exists
+        assert os.path.isfile(full_path), f'{full_path} does not exist.'
+
+        with open(full_path, 'rb') as inp:
+            dataset = pickle.load(inp)
+
+        return dataset
+
+
+
+
     def show_settings(self):
         """
         A function that prints out all the settings, structured per thematic.
 
         Returns
         -------
         None.
@@ -185,23 +454,22 @@
         # so that all methods can be inherited.
 
         try:
             sta_df = self.df.xs(stationname, level="name", drop_level=False)
             sta_metadf = self.metadf.loc[stationname].to_frame().transpose()
         except KeyError:
             logger.warning(f"{stationname} not found in the dataset.")
-            print(f"{stationname} not found in the dataset.")
             return None
 
         try:
             sta_outliers = self.outliersdf.xs(
                 stationname, level="name", drop_level=False
             )
         except KeyError:
-            sta_outliers = init_multiindexdf()
+            sta_outliers = init_triple_multiindexdf()
 
         sta_gaps = get_station_gaps(self.gaps, stationname)
         sta_missingobs = self.missing_obs.get_station_missingobs(stationname)
 
         try:
             sta_gapfill = self.gapfilldf.xs(stationname, level="name", drop_level=False)
         except KeyError:
@@ -223,52 +491,25 @@
             metadf=sta_metadf,
             data_template=self.data_template,
             settings=self.settings,
             _qc_checked_obstypes=self._qc_checked_obstypes,
             _applied_qc=self._applied_qc,
         )
 
-    def show(self):
-        """
-        A function to print out some overview information about the Dataset.
-
-        Returns
-        -------
-        None.
-
-        """
-
-        logger.info("Show basic info of dataset.")
-
-        try:
-            gapsdf = self.gaps.to_df()
-        except:
-            gapsdf = init_multiindexdf()
 
-        if self.missing_obs is None:
-            missing_obs_series = pd.Series(dtype=object)
-        else:
-            missing_obs_series = self.missing_obs.series
-
-        print_dataset_info(
-            self.df,
-            self.outliersdf,
-            gapsdf,
-            missing_obs_series,
-            self.settings.app["print_fmt_datetime"],
-        )
 
     def make_plot(
         self,
         stationnames=None,
         obstype="temp",
         colorby="name",
         starttime=None,
         endtime=None,
         title=None,
+        y_label=None,
         legend=True,
         show_outliers=True,
         show_filled = True,
         _ax=None, #needed for GUI, not recommended use
     ):
         """
         This function creates a timeseries plot for the dataset. The variable observation type
@@ -288,104 +529,119 @@
              Indicate how colors should be assigned to the lines. 'label' will color the lines by their quality control label. 'name' will color by each station, defaults to 'name'.
         starttime : datetime.datetime, optional
              Specifiy the start datetime for the plot. If None is given it will use the start datetime of the dataset, defaults to None.
         endtime : datetime.datetime, optional
              Specifiy the end datetime for the plot. If None is given it will use the end datetime of the dataset, defaults to None.
         title : string, optional
              Title of the figure, if None a default title is generated. The default is None.
+        y_label : string, optional
+             y-axes label of the figure, if None a default label is generated. The default is None.
         legend : bool, optional
-             I True, a legend is added to the plot. The default is True.
+             If True, a legend is added to the plot. The default is True.
         show_outliers : bool, optional
-             If true the observations labeld as outliers will be included in the plot, defaults to True
+             If true the observations labeld as outliers will be included in
+             the plot. This is only true when colorby == 'name'. The default
+             is True.
         show_filled : bool, optional
              If true the filled values for gaps and missing observations will
-             be included in the plot, defaults to True
+             be included in the plot. This is only true when colorby == 'name'.
+             The default is True.
 
 
         Returns
         -------
         axis : matplotlib.pyplot.axes
              The timeseries axes of the plot is returned.
 
+        Note
+        --------
+        If a timezone unaware datetime is given as an argument, it is interpreted
+        as if it has the same timezone as the observations.
+
         """
 
-        logger.info(f"Make {obstype}-timeseries plot for {stationnames}")
+        if stationnames is None:
+            logger.info(f"Make {obstype}-timeseries plot for all stations")
+        else:
+            logger.info(f"Make {obstype}-timeseries plot for {stationnames}")
 
         # combine all dataframes
         mergedf = self.combine_all_to_obsspace()
 
         # subset to obstype
-        mergedf = mergedf.xs(obstype, level='obstype')
+        mergedf = xs_save(mergedf, obstype, level='obstype')
 
         # Subset on stationnames
         if not stationnames is None:
-            mergedf = mergedf.reset_index()
-            mergedf = mergedf.loc[mergedf['name'].isin(stationnames)]
-            mergedf = mergedf.set_index(['name', 'datetime'])
+            mergedf = mergedf[mergedf.index.get_level_values('name').isin(stationnames)]
 
 
         # Subset on start and endtime
-        mergedf = multiindexdf_datetime_subsetting(mergedf, starttime, endtime)
+        starttime = fmt_datetime_argument(starttime, self.settings.time_settings['timezone'])
+        endtime = fmt_datetime_argument(endtime, self.settings.time_settings['timezone'])
 
-        # remove outliers if required
-        if not show_outliers:
-            outlier_labels = [var['outlier_flag'] for var in self.settings.qc['qc_checks_info'].values()]
-            mergedf = mergedf[~mergedf['label'].isin(outlier_labels)]
-
-        # remove filled values if required
-        if not show_filled:
-            fill_labels = ['gap fill', 'missing observation fill'] #toolkit representation labels
-            mergedf = mergedf[~mergedf['toolkit_representation'].isin(fill_labels)]
+        mergedf = multiindexdf_datetime_subsetting(mergedf, starttime, endtime)
 
         # Get plot styling attributes
         if title is None:
             if stationnames is None:
                 if self._istype == "Dataset":
                     title = (
-                        self.settings.app["display_name_mapper"][obstype]
+                        self.data_template[obstype]["orig_name"]
                         + " for all stations. "
                     )
                 elif self._istype == "Station":
                     title = (
-                        self.settings.app["display_name_mapper"][obstype]
+                        self.data_template[obstype]["orig_name"]
                         + " of "
                         + self.name
                     )
 
             else:
                 title = (
-                    self.settings.app["display_name_mapper"][obstype]
+                    self.data_template[obstype]["orig_name"]
                     + " for stations: "
                     + str(stationnames)
                 )
-
+        # create y label
+        if y_label is None:
+            try:
+                if isinstance(self.data_template[obstype]["description"], str):
+                    description =self.data_template[obstype]["description"]
+                else:
+                    description =''
+
+                y_label = f'{self.data_template[obstype]["orig_name"]} ({self.data_template[obstype]["units"]}) \n {description}'
+            except KeyError:
+                y_label = obstype
 
         # Make plot
-        ax = timeseries_plot(
+        ax, _colmap = timeseries_plot(
             mergedf=mergedf,
             title=title,
-            xlabel="Timestamp",
-            ylabel=self.data_template[obstype]["orig_name"],
+            ylabel=y_label,
             colorby=colorby,
             show_legend=legend,
             show_outliers=show_outliers,
+            show_filled=show_filled,
             settings = self.settings,
             _ax = _ax
         )
 
         return ax
 
     def make_geo_plot(
         self,
-        obstype="temp",
+        variable="temp",
         title=None,
         timeinstance=None,
         legend=True,
         vmin=None,
         vmax=None,
+        boundbox = []
     ):
         """
         This functions creates a geospatial plot for a field
         (observations or attributes) of all stations.
 
         If the field is timedepending, than the timeinstance is used to plot
         the field status at that datetime.
@@ -393,128 +649,204 @@
         If the field is categorical than the leged will have categorical
         values, else a colorbar is used.
 
         All styling attributes are extracted from the Settings.
 
         Parameters
         ----------
-        obstype : string, optional
-            Fieldname to visualise. This can be an observation or station
-            attribute. The default is 'temp'.
+        variable : string, optional
+            Fieldname to visualise. This can be an observation type or station
+            or 'lcz'. The default is 'temp'.
         title : string, optional
             Title of the figure, if None a default title is generated. The default is None.
         timeinstance : datetime.datetime, optional
-            Datetime moment of the geospatial plot. If None, the first available datetime is used. The default is None.
+            Datetime moment of the geospatial plot. If None, the first occuring (not Nan) record is used. The default is None.
         legend : bool, optional
             I True, a legend is added to the plot. The default is True.
         vmin : numeric, optional
             The value corresponding with the minimum color. If None, the minimum of the presented observations is used. The default is None.
         vmax : numeric, optional
             The value corresponding with the maximum color. If None, the maximum of the presented observations is used. The default is None.
-
+        boundbox : [lon-west, lat-south, lon-east, lat-north], optional
+            The boundbox to indicate the domain to plot. The elemenst are numeric.
+            If the list is empty, a boundbox is created automatically. The default
+            is [].
         Returns
         -------
         axis : matplotlib.pyplot.geoaxes
             The geoaxes of the plot is returned.
 
+        Note
+        --------
+        If a timezone unaware datetime is given as an argument, it is interpreted
+        as if it has the same timezone as the observations.
+
         """
 
         # Load default plot settings
         # default_settings=Settings.plot_settings['spatial_geo']
 
-        # get first timeinstance of the dataset if not given
+        # get first (Not Nan) timeinstance of the dataset if not given
+        timeinstance = fmt_datetime_argument(timeinstance, self.settings.time_settings['timezone'])
         if timeinstance is None:
-            timeinstance = self.df.index.get_level_values("datetime").min()
+            timeinstance = self.df.dropna(subset=['temp']).index[0][1]
+
+        logger.info(f"Make {variable}-geo plot at {timeinstance}")
+
+
+        # check coordinates if available
+        if self.metadf['lat'].isnull().any():
+            _sta = self.metadf[self.metadf['lat'].isnull()]['lat']
+            logger.warning(f'Stations without coordinates detected: {_sta}')
+            return None
+        if self.metadf['lon'].isnull().any():
+            _sta = self.metadf[self.metadf['lon'].isnull()]['lon']
+            logger.warning(f'Stations without coordinates detected: {_sta}')
+            return None
+
+        if bool(boundbox):
+            if len(boundbox) != 4:
+                logger.warning(f'The boundbox ({boundbox}) does not contain 4 elements! The default boundbox is used!')
+                boundbox=[]
+
+        # Check if LCZ if available
+        if variable == 'lcz':
+            if self.metadf['lcz'].isnull().any():
+                _sta = self.metadf[self.metadf['lcz'].isnull()]['lcz']
+                logger.warning(f'Stations without lcz detected: {_sta}')
+                return None
 
-        logger.info(f"Make {obstype}-geo plot at {timeinstance}")
 
         # subset to timeinstance
-        plotdf = self.df.xs(timeinstance, level="datetime")
+        plotdf = xs_save(self.df, timeinstance, level="datetime")
 
         # merge metadata
         plotdf = plotdf.merge(
             self.metadf, how="left", left_index=True, right_index=True
         )
 
         axis = geospatial_plot(
             plotdf=plotdf,
-            variable=obstype,
+            variable=variable,
             timeinstance=timeinstance,
             title=title,
             legend=legend,
             vmin=vmin,
             vmax=vmax,
             plotsettings=self.settings.app["plot_settings"],
             categorical_fields=self.settings.app["categorical_fields"],
             static_fields=self.settings.app["static_fields"],
             display_name_mapper=self.settings.app["display_name_mapper"],
             world_boundaries_map=self.settings.app["world_boundary_map"],
+            data_template=self.data_template,
+            boundbox = boundbox
         )
 
         return axis
 
     # =============================================================================
     #   Gap Filling
     # =============================================================================
     def get_modeldata(
-        self, modelname="ERA5_hourly", stations=None, startdt=None, enddt=None
+        self, modelname="ERA5_hourly", modeldata=None, obstype='temp', stations=None, startdt=None, enddt=None
     ):
         """
         Make a metobs_toolkit.Modeldata object with modeldata at the locations
         of the stations present in the dataset.
 
         Parameters
         ----------
-        modelname : 'ERA5_hourly', optional
-            Which dataset to download timeseries from. The default is 'ERA5_hourly'.
+        modelname : str, optional
+            Which dataset to download timeseries from. This is only used when
+            no modeldata is provided. The default is 'ERA5_hourly'.
+        modeldata : metobs_toolkit.Modeldata, optional
+            Use the modelname attribute and the gee information stored in the
+            modeldata instance to extract timeseries.
+        obstype : String, optional
+            Name of the observationtype you want to apply gap filling on. The
+            modeldata must contain this observation type as well. The
+            default is 'temp'.
         stations : string or list of strings, optional
             Stationnames to subset the modeldata to. If None, all stations will be used. The default is None.
         startdt : datetime.datetime, optional
             Start datetime of the model timeseries. If None, the start datetime of the dataset is used. The default is None.
         enddt : datetime.datetime, optional
             End datetime of the model timeseries. If None, the last datetime of the dataset is used. The default is None.
 
         Returns
         -------
         Modl : metobs_toolkit.Modeldata
             The extracted modeldata for period and a set of stations.
 
-        NOTE
+        Note
+        --------
+        If a timezone unaware datetime is given as an argument, it is interpreted
+        as if it has the same timezone as the observations.
+
+        Note
+        ------
+        When extracting large amounts of data, the timeseries data will be
+        writen to a file and saved on your google drive. In this case, you need
+        to provide the Modeldata with the data using the .set_model_from_csv()
+        method.
+
+        Note
         ------
-        Only 2mT extraction of ERA5 is implemented at the moment.
+        Only 2mT extraction of ERA5 is implemented for all Modeldata instances.
+        To extract other variables, one must create a Modeldata instance in
+        advance, add or update a gee_dataset and give this Modeldata instance
+        to this method.
 
         """
-
-        Modl = Modeldata(modelname)
+        if modeldata is None:
+            Modl = Modeldata(modelname)
+        else:
+            Modl = modeldata
+            modelname = Modl.modelname
 
         # Filters
         if startdt is None:
             startdt = self.df.index.get_level_values("datetime").min()
+        else:
+            startdt = fmt_datetime_argument(startdt, self.settings.time_settings['timezone'])
+
         if enddt is None:
             enddt = self.df.index.get_level_values("datetime").max()
+        else:
+            enddt = fmt_datetime_argument(enddt, self.settings.time_settings['timezone'])
+
         if not stations is None:
             if isinstance(stations, str):
                 metadf = self.metadf.loc[[stations]]
             if isinstance(stations, list):
                 metadf = self.metadf.iloc[self.metadf.index.isin(stations)]
         else:
             metadf = self.metadf
 
         # Convert to UTC
+
         startdt_utc = startdt.astimezone(pytz.utc)
         enddt_utc = enddt.astimezone(pytz.utc)
 
         # fill modell with data
         if modelname == "ERA5_hourly":
-            Modl.get_ERA5_data(metadf, startdt_utc, enddt_utc)
+            Modl.get_ERA5_data(metadf=metadf,
+                               startdt_utc = startdt_utc,
+                               enddt_utc = enddt_utc,
+                               obstype=obstype)
 
-            return Modl
         else:
-            print(f"{modelname} for set_modeldata is not implemented yet")
-            return None
+            Modl.get_gee_dataset_data(mapname=modelname,
+                                      metadf=metadf,
+                                      startdt_utc = startdt_utc,
+                                      enddt_utc = enddt_utc,
+                                      obstype=obstype)
+        print(f'(When using the .set_model_from_csv() method, make shure the modelname of your Modeldata is {modelname})')
+        logger.info(f'(When using the .set_model_from_csv() method, make shure the modelname of your Modeldata is {modelname})')
+        return Modl
 
     def update_gaps_and_missing_from_outliers(self, obstype='temp', n_gapsize=None):
         """
         Interpret the outliers as missing observations. If there is a sequence
         of these outliers for a station, larger than n_gapsize than this will
         be interpreted as a gap.
 
@@ -546,45 +878,45 @@
         this is different from the gap check applied on the inported data, if
         the dataset is coarsend.
 
         """
         if n_gapsize is None:
             n_gapsize = self.settings.gap['gaps_settings']['gaps_finder']['gapsize_n']
             if not self.metadf["assumed_import_frequency"].eq(self.metadf['dataset_resolution']).all():
-                print(f'The defenition of the gapsize (n_gapsize = {n_gapsize}) \
+                logger.info(f'The defenition of the gapsize (n_gapsize = {n_gapsize}) \
                                will have another effect on the update of the gaps and missing \
                                    timestamps because coarsening is applied and the defenition \
                                    of the gapsize is not changed.')
 
 
 
         # combine to one dataframe
         mergedf = self.combine_all_to_obsspace()
-        mergedf = mergedf.xs(obstype, level='obstype')
+        mergedf = xs_save(mergedf, obstype, level='obstype')
 
 
         # ignore labels
         possible_outlier_labels = [vals['outlier_flag'] for vals in self.settings.qc['qc_checks_info'].values()]
 
 
         # create groups when the final label changes
         persistance_filter = ((mergedf['label'].shift() != mergedf['label'])).cumsum()
         grouped = mergedf.groupby(['name', persistance_filter])
 
         #locate new gaps by size of consecutive the same final label per station
         group_sizes = grouped.size()
-        outlier_groups = group_sizes[
+        large_groups = group_sizes[
             group_sizes > n_gapsize
         ]
 
         # find only groups with final label as an outlier
         gaps = []
         # new_gapsdf = pd.DataFrame()
         new_gaps_idx = init_multiindex()
-        for group_idx in outlier_groups.index:
+        for group_idx in large_groups.index:
             groupdf = grouped.get_group(group_idx)
             group_final_label = groupdf['label'].iloc[0]
             if not group_final_label in possible_outlier_labels:
                 #no gap candidates
                 continue
             else:
                 gap =Gap(name=groupdf.index.get_level_values('name')[0],
@@ -608,153 +940,78 @@
 
         # to series
         missing_obs_series = new_missing_obs.to_frame().reset_index(drop=True).set_index('name')['datetime']
         # Create missing obs
         new_missing_collection = Missingob_collection(missing_obs_series)
 
 
-
         # update self
         self.gaps.extend(gaps)
         self.missing_obs = self.missing_obs + new_missing_collection
 
+        # remove outliers that are converted to gaps
+        self.outliersdf = remove_gaps_from_outliers(gaplist=gaps,
+                                                    outldf = self.outliersdf)
+
+        # remove outliers that are converted to missing obs
+        self.outliersdf = self.missing_obs.remove_missing_from_outliers(self.outliersdf)
 
 
     # =============================================================================
     #   Gap Filling
     # =============================================================================
 
-    # def fill_gaps_automatic(self, modeldata, obstype='temp',
-    #                         max_interpolate_duration_str=None,
-    #                         overwrite=True):
-    #     """
-    #     Fill gaps using an automatic decision on which method to use to fill.
-    #     For small gaps (gap_duration <= max_interpolate_duration_str) interpolation
-    #     is applied, for larger gaps the model debias method is used.
-
-    #     Parameters
-    #     ----------
-    #     modeldata : metobs_toolkit.Modeldata
-    #         The ERA5 Modeldata instance containing observations for the periods
-    #         gaps and the leading/trailing periods..
-    #     obstype : str, optional
-    #         Observation type to fill the gaps for. The default is 'temp'.
-    #     max_interpolate_duration_str : timedelta or timedeltastring, optional
-    #         A time indication (like '5H') to indicate the maximum gapsize to use
-    #         interpolation for. If None, the default settings will be used. The default is None.
-    #     overwrite : bool, optional
-    #         If True, present gapfill values will be overwritten. The default is True.
-
-    #     Returns
-    #     -------
-    #     comb_df : TYPE
-    #         DESCRIPTION.
-
-    #     """
-
-    #     # Validate input
-    #     # check if modeldata is available
-    #     if modeldata is None:
-    #         print(
-    #             "The dataset has no modeldate. Use the set_modeldata() function to add modeldata."
-    #         )
-    #         return None
-
-    #     # check if obstype is present in eramodel
-    #     assert (
-    #         obstype in modeldata.df.columns
-    #     ), f"{obstype} is not present in the modeldate: {modeldata}"
-
-    #     # check if all station are present in eramodeldata
-    #     stations = self.gaps.to_df().index.unique().to_list()
-    #     assert all(
-    #         [sta in modeldata.df.index.get_level_values("name") for sta in stations]
-    #     ), f"Not all stations with gaps are in the modeldata!"
-
-    #     if not self.gapfilldf.empty:
-    #         if overwrite:
-    #             print("Gapfilldf will be overwritten!")
-    #             self.gapfilldf = init_multiindexdf()
-    #         else:
-    #             print('Gapfilldf is not empty, set "overwrite=True" to overwrite it!')
-    #             print("CANCEL gap fill with ERA5")
-    #             return
 
-    #     if max_interpolate_duration_str is None:
-    #         max_interpolate_duration_str = self.settings.gap["gaps_fill_settings"]["automatic"]["max_interpolation_duration_str"]
 
-    #     fill_info = self.settings.gap["gaps_fill_info"]
-
-    #     # select the method to apply gapfill per gap
-    #     interpolate_gaps = []
-    #     debias_gaps = []
-
-    #     for gap in self.gaps.list:
-    #         if gap.duration <= pd.to_timedelta(max_interpolate_duration_str):
-    #             interpolate_gaps.append(gap)
-    #         else:
-    #             debias_gaps.append(gap)
-
-
-    #     # convert to Gap_collection
-    #     interpolate_gap_collection = _gap_collection_from_list_of_gaps(interpolate_gaps)
-    #     debias_gap_collection =_gap_collection_from_list_of_gaps(debias_gaps)
-
-
-    #     #1  Fill by interpolation
-
-    #     filldf_interp = init_multiindexdf()
-
-    #     fill_settings_interp = self.settings.gap["gaps_fill_settings"]["linear"]
-
-
-    #     filldf_interp[obstype] = interpolate_gap_collection.apply_interpolate_gaps(
-    #                         obsdf=self.df,
-    #                         outliersdf=self.outliersdf,
-    #                         dataset_res=self.metadf["dataset_resolution"],
-    #                         obstype=obstype,
-    #                         method=fill_settings_interp["method"],
-    #                         max_consec_fill=fill_settings_interp["max_consec_fill"],
-    #                         )
-
-    #     # add label column
-    #     filldf_interp[obstype + "_" + fill_info["label_columnname"]] = fill_info["label"]["linear"]
-
-
-    #     #2 Fill by debias
-    #     filldf_debias = init_multiindexdf()
-
-    #     fill_settings_debias = self.settings.gap["gaps_fill_settings"]["model_debias"]
+    def fill_gaps_automatic(self, modeldata, obstype='temp',
+                            max_interpolate_duration_str=None,
+                            overwrite_fill=False):
+        """
+        Fill the gaps by using linear interpolation or debiased modeldata. The
+        method that is applied to perform the gapfill will be determined by the
+        duration of the gap.
+
+        When the duration of a gap is smaller or equal than
+        max_interpolation_duration, the linear interpolation method is applied
+        else the debiased modeldata method.
 
 
-    #     apply_debias_era5_gapfill(gapslist = self.gaps
-    #                               dataset=self,
-    #                               eraModelData=modeldata,
-    #                               obstype=obstype,
-    #                               debias_settings=fill_settings_debias)
+        Parameters
+        ----------
+        modeldata : metobs_toolkit.Modeldata
+            The modeldata to use for the gapfill. This model data should the required
+            timeseries to fill all gaps present in the dataset.
+        obstype : String, optional
+            Name of the observationtype you want to apply gap filling on. The
+            modeldata must contain this observation type as well. The
+            default is 'temp'.
+        max_interpolate_duration_str : Timedelta or str, optional
+            Maximum duration to apply interpolation for gapfill when using the
+            automatic gapfill method. Gaps with longer durations will be filled
+            using debiased modeldata. The default is None.
+        overwrite_fill: bool, optional
+            If a gap has already filled values, the interpolation of this gap
+            is skipped if overwrite_fill is False. If set to True, the gapfill
+            values and info will be overwitten. The default is False.
 
-    #     # add label column
-    #     filldf_debias[obstype + "_" + fill_info["label_columnname"]] = fill_info["label"]["model_debias"]
+        Returns
+        -------
+        comb_df : TYPE
+            gapfilldf : pandas.DataFrame
+                A dataframe containing all the filled records.
 
+        """
 
-    #     # combine both fill df's
-    #     comb_df = pd.concat([filldf_interp, filldf_debias])
-    #     if overwrite:
-    #         self.gapfilldf = comb_df
-    #     return comb_df
 
 
-    def fill_gaps_automatic(self, modeldata, obstype='temp',
-                            max_interpolate_duration_str=None,
-                            overwrite=True):
+        #  ----------- Validate ----------------------------------------
 
-        # Validate input
         # check if modeldata is available
         if modeldata is None:
-            print(
+            logger.warning(
                 "The dataset has no modeldate. Use the set_modeldata() function to add modeldata."
             )
             return None
 
         # check if obstype is present in eramodel
         assert (
             obstype in modeldata.df.columns
@@ -763,114 +1020,123 @@
         # check if all station are present in eramodeldata
         # stations = self.gaps.to_df().index.unique().to_list()
         stations = list(set([gap.name for gap in self.gaps]))
         assert all(
             [sta in modeldata.df.index.get_level_values("name") for sta in stations]
         ), f"Not all stations with gaps are in the modeldata!"
 
-        if not self.gapfilldf.empty:
-            if overwrite:
-                print("Gapfilldf will be overwritten!")
-                self.gapfilldf = init_multiindexdf()
-            else:
-                print('Gapfilldf is not empty, set "overwrite=True" to overwrite it!')
-                print("CANCEL gap fill with ERA5")
-                return
+
 
         if max_interpolate_duration_str is None:
             max_interpolate_duration_str = self.settings.gap["gaps_fill_settings"]["automatic"]["max_interpolation_duration_str"]
 
         fill_info = self.settings.gap["gaps_fill_info"]
 
-        # select the method to apply gapfill per gap
+        #  ------------select the method to apply gapfill per gap ----------
         interpolate_gaps = []
         debias_gaps = []
 
         for gap in self.gaps:
             if gap.duration <= pd.to_timedelta(max_interpolate_duration_str):
                 interpolate_gaps.append(gap)
             else:
                 debias_gaps.append(gap)
 
-        #1  Fill by interpolation
+        #1   ---------------Fill by interpolation ---------------------
 
         fill_settings_interp = self.settings.gap["gaps_fill_settings"]["linear"]
 
 
         apply_interpolate_gaps(
                             gapslist=interpolate_gaps,
                             obsdf=self.df,
                             outliersdf=self.outliersdf,
                             dataset_res=self.metadf["dataset_resolution"],
                             gapfill_settings=self.settings.gap['gaps_fill_info'],
                             obstype=obstype,
                             method=fill_settings_interp["method"],
                             max_consec_fill=fill_settings_interp["max_consec_fill"],
+                            overwrite_fill=overwrite_fill,
                             )
 
         filldf_interp = make_gapfill_df(interpolate_gaps)
 
-        #2 Fill by debias
+        #2  --------------  Fill by debias -----------------------------
 
         fill_settings_debias = self.settings.gap["gaps_fill_settings"]["model_debias"]
 
 
         apply_debias_era5_gapfill(gapslist=debias_gaps,
                                         dataset=self,
                                         eraModelData=modeldata,
                                         obstype=obstype,
-                                        debias_settings=fill_settings_debias)
+                                        debias_settings=fill_settings_debias,
+                                        overwrite_fill=overwrite_fill)
 
         # add label column
         filldf_debias = make_gapfill_df(debias_gaps)
 
 
         # combine both fill df's
         comb_df = pd.concat([filldf_interp, filldf_debias])
-        if overwrite:
-            self.gapfilldf = comb_df
+
+        # update attr
+        self.gapfilldf = comb_df
+
         return comb_df
 
 
-    def fill_gaps_linear(self, obstype="temp", overwrite=True):
+    def fill_gaps_linear(self, obstype="temp", overwrite_fill=False):
         """
         Fill the gaps using linear interpolation.
 
+        The gapsfilldf attribute of the Datasetinstance will be updated if
+        the gaps are not filled yet or if overwrite_fill is set to True.
+
         Parameters
         ----------
         obstype : string, optional
             Fieldname to visualise. This can be an observation or station
             attribute. The default is 'temp'.
+        overwrite_fill: bool, optional
+            If a gap has already filled values, the interpolation of this gap
+            is skipped if overwrite_fill is False. If set to True, the gapfill
+            values and info will be overwitten. The default is False.
 
         Returns
         -------
-        None.
+        gapfilldf : pandas.DataFrame
+            A dataframe containing all the filled records.
+
 
         """
+
+
         # TODO logging
         fill_settings = self.settings.gap["gaps_fill_settings"]["linear"]
         fill_info = self.settings.gap["gaps_fill_info"]
 
         # fill gaps
         apply_interpolate_gaps(
-            gapslist=self.gaps,
-            obsdf=self.df,
-            outliersdf=self.outliersdf,
-            dataset_res=self.metadf["dataset_resolution"],
-            gapfill_settings=self.settings.gap['gaps_fill_info'],
-            obstype=obstype,
-            method=fill_settings["method"],
-            max_consec_fill=fill_settings["max_consec_fill"],
+                gapslist=self.gaps,
+                obsdf=self.df,
+                outliersdf=self.outliersdf,
+                dataset_res=self.metadf["dataset_resolution"],
+                gapfill_settings=self.settings.gap['gaps_fill_info'],
+                obstype=obstype,
+                method=fill_settings["method"],
+                max_consec_fill=fill_settings["max_consec_fill"],
+                overwrite_fill = overwrite_fill,
         )
 
         # get gapfilldf
         gapfilldf = make_gapfill_df(self.gaps)
 
-        if overwrite:
-            self.gapfilldf = gapfilldf
+        # update attr
+        self.gapfilldf = gapfilldf
 
         return gapfilldf
 
 
     def fill_missing_obs_linear(self, obstype='temp'):
         # TODO logging
         fill_settings = self.settings.missing_obs['missing_obs_fill_settings']['linear']
@@ -882,14 +1148,15 @@
         self.missing_obs.interpolate_missing(
                                             obsdf=self.df,
                                             resolutionseries=self.metadf["dataset_resolution"],
                                             obstype=obstype,
                                             method=fill_settings["method"],
         )
         missing_fill_df = self.missing_obs.fill_df
+
         missing_fill_df[obstype+'_' + fill_info["label_columnname"]] = fill_info["label"]["linear"]
 
         # Update attribute
 
         self.missing_fill_df = missing_fill_df
 
     def get_gaps_df(self):
@@ -901,14 +1168,47 @@
         pandas.DataFrame
             A DataFrame with stationnames as index, and the start, end and duretion
             of the gaps as columns.
 
         """
         return gaps_to_df(self.gaps)
 
+    def get_gaps_info(self):
+        """
+        Print out detailed information of the gaps.
+
+        Returns
+        -------
+        None.
+
+        """
+
+
+        if bool(self.gaps):
+            # there are gaps
+            for gap in self.gaps:
+                gap.get_info()
+        else:
+            # no gaps
+            print('There are no gaps.')
+
+
+    def get_missing_obs_info(self):
+        """
+        Print out detailed information of the missing observations.
+
+        Returns
+        -------
+        None.
+
+        """
+        # empty obs protector in the .get_info method.
+        self.missing_obs.get_info()
+
+
 
 
     def get_analysis(self):
         """
         Create a MetObs_toolkit.Analysis instance from the Dataframe
 
         Returns
@@ -921,45 +1221,48 @@
         return Analysis(obsdf = self.df,
                         metadf = self.metadf,
                         settings = self.settings,
                         data_template=self.data_template)
 
 
     def fill_gaps_era5(
-        self, modeldata, method="debias", obstype="temp", overwrite=True
+        self, modeldata, method="debias", obstype="temp", overwrite_fill=False
     ):
         """
         Fill the gaps using a metobs_toolkit.Modeldata object.
 
 
         Parameters
         ----------
         modeldata : metobs_toolkit.Modeldata
             The modeldata to use for the gapfill. This model data should the required
             timeseries to fill all gaps present in the dataset.
         method : 'debias', optional
             Specify which method to use. The default is 'debias'.
-        obstype : TYPE, optional
-            Fieldname to visualise. This can be an observation or station
-            attribute. The default is 'temp'.
-        overwrite : bool, optional
-            If True, the Dataset.Gapfilldf will be overwritten. The default is True.
+        obstype : String, optional
+           Name of the observationtype you want to apply gap filling on. The
+           modeldata must contain this observation type as well. The
+           default is 'temp'.
+        overwrite_fill: bool, optional
+            If a gap has already filled values, the interpolation of this gap
+            is skipped if overwrite_fill is False. If set to True, the gapfill
+            values and info will be overwitten. The default is False.
 
         Returns
         -------
         Gapfilldf : pandas.DataFrame
             A dataframe containing all gap filled values and the use method.
 
         """
 
         fill_info = self.settings.gap["gaps_fill_info"]
 
         # check if modeldata is available
         if modeldata is None:
-            print(
+            logger.warning(
                 "The dataset has no modeldate. Use the set_modeldata() function to add modeldata."
             )
             return None
         # check if obstype is present in eramodel
         assert (
             obstype in modeldata.df.columns
         ), f"{obstype} is not present in the modeldate: {modeldata}"
@@ -976,23 +1279,25 @@
             fill_settings_debias = self.settings.gap["gaps_fill_settings"]["model_debias"]
 
 
             apply_debias_era5_gapfill(gapslist=self.gaps,
                                             dataset=self,
                                             eraModelData=modeldata,
                                             obstype=obstype,
-                                            debias_settings=fill_settings_debias)
+                                            debias_settings=fill_settings_debias,
+                                            overwrite_fill=overwrite_fill)
 
             # get fill df
             filldf = make_gapfill_df(self.gaps)
         else:
-            print("not implemented yet")
+            sys.exit(f"{method} not implemented yet")
+
+        # update attribute
+        self.gapfilldf = filldf
 
-        if overwrite:
-            self.gapfilldf = filldf
         return filldf
 
     def write_to_csv(
         self,
         obstype=None,
         filename=None,
         include_outliers=True,
@@ -1070,15 +1375,15 @@
 
         # drop fill values if required
         if not include_fill_values:
             fill_labels = ['gap fill', 'missing observation fill'] #toolkit representation labels
             mergedf = mergedf[~mergedf['toolkit_representation'].isin(fill_labels)]
 
         if not obstype is None:
-            mergedf = mergedf.xs(obstype, level='obstype', drop_level=False)
+            mergedf = xs_save(mergedf, obstype, level='obstype', drop_level=False)
 
 
 
         # Map obstypes columns
         if not use_tlk_obsnames:
             mapper = self.data_template.transpose()['orig_name'].to_dict()
             mergedf = mergedf.reset_index()
@@ -1137,192 +1442,428 @@
          obstype : String, optional
              Name of the observationtype you want to apply the checks on. The
              default is 'temp'.
          gross_value : Bool, optional
              If True the gross_value check is applied if False not. The default
              is True.
          persistance : Bool, optional
-            If True the persistance check is applied if False not. The default
-            is True.. The default is True.
+             If True the persistance check is applied if False not. The default
+             is True.. The default is True.
+         repetition : Bool, optional
+             If True the repetations check is applied if False not. The default
+             is True.
          step : Bool, optional
-            If True the step check is applied if False not. The default is True.
-         internal_consistency : Bool, optional
-            If True the internal consistency check is applied if False not. The
-            default is True.
-         qc_info: Bool, optional
-            If True info about the quality control is printed if False not. The
-            default is True.
-         ignore_val : numeric, optional
-             Values to ignore in the quality checks. The default is np.nan.
+             If True the step check is applied if False not. The default is True.
+         window_variation : Bool, optional
+             If True the window_variation check is applied if False not. The
+             default is True.
 
          Returns
          ---------
 
          None.
 
         """
 
+
+
+
         if repetitions:
-            print("Applying the repetitions-check on all stations.")
-            logger.info("Applying repetitions check on the full dataset")
+            logger.info("Applying repetitions check.")
+            apliable = _can_qc_be_applied(self._applied_qc, obstype, "repetitions")
 
-            obsdf, outl_df = repetitions_check(
-                obsdf=self.df,
-                obstype=obstype,
-                checks_info=self.settings.qc["qc_checks_info"],
-                checks_settings=self.settings.qc["qc_check_settings"],
-            )
+            if apliable:
 
-            # update the dataset and outliers
-            self.df = obsdf
-            if not outl_df.empty:
-                self.outliersdf = pd.concat([self.outliersdf, outl_df])
+                obsdf, outl_df = repetitions_check(
+                    obsdf=self.df,
+                    obstype=obstype,
+                    checks_info=self.settings.qc["qc_checks_info"],
+                    checks_settings=self.settings.qc["qc_check_settings"],
+                )
 
-            # add this check to the applied checks
-            self._applied_qc = pd.concat(
-                [
-                    self._applied_qc,
-                    conv_applied_qc_to_df(
-                        obstypes=obstype, ordered_checknames="repetitions"
-                    ),
-                ],
-                ignore_index=True,
-            )
+                # update the dataset and outliers
+                self.df = obsdf
+                if not outl_df.empty:
+                    self.outliersdf = pd.concat([self.outliersdf, outl_df])
+
+                # add this check to the applied checks
+                self._applied_qc = pd.concat(
+                    [
+                        self._applied_qc,
+                        conv_applied_qc_to_df(
+                            obstypes=obstype, ordered_checknames="repetitions"
+                        ),
+                    ],
+                    ignore_index=True,
+                )
+            else:
+                logger.warning(f'The repetitions check can NOT be applied on {obstype} because it was already applied on this observation type!')
 
         if gross_value:
-            print("Applying the gross-value-check on all stations.")
-            logger.info("Applying gross value check on the full dataset")
+            logger.info("Applying gross value check.")
 
-            obsdf, outl_df = gross_value_check(
-                obsdf=self.df,
-                obstype=obstype,
-                checks_info=self.settings.qc["qc_checks_info"],
-                checks_settings=self.settings.qc["qc_check_settings"],
-            )
+            apliable = _can_qc_be_applied(self._applied_qc, obstype, "gross_value")
 
-            # update the dataset and outliers
-            self.df = obsdf
-            if not outl_df.empty:
-                self.outliersdf = pd.concat([self.outliersdf, outl_df])
+            if apliable:
 
-            # add this check to the applied checks
-            self._applied_qc = pd.concat(
-                [
-                    self._applied_qc,
-                    conv_applied_qc_to_df(
-                        obstypes=obstype, ordered_checknames="gross_value"
-                    ),
-                ],
-                ignore_index=True,
-            )
+                obsdf, outl_df = gross_value_check(
+                    obsdf=self.df,
+                    obstype=obstype,
+                    checks_info=self.settings.qc["qc_checks_info"],
+                    checks_settings=self.settings.qc["qc_check_settings"],
+                )
+
+                # update the dataset and outliers
+                self.df = obsdf
+                if not outl_df.empty:
+                    self.outliersdf = pd.concat([self.outliersdf, outl_df])
+
+                # add this check to the applied checks
+                self._applied_qc = pd.concat(
+                    [
+                        self._applied_qc,
+                        conv_applied_qc_to_df(
+                            obstypes=obstype, ordered_checknames="gross_value"
+                        ),
+                    ],
+                    ignore_index=True,
+                )
+
+            else:
+                logger.warning(f'The gross_value check can NOT be applied on {obstype} because it was already applied on this observation type!')
 
         if persistance:
-            print("Applying the persistance-check on all stations.")
-            logger.info("Applying persistance check on the full dataset")
+            logger.info("Applying persistance check.")
+
+            apliable = _can_qc_be_applied(self._applied_qc, obstype, "persistance")
+
+            if apliable:
+
+                obsdf, outl_df = persistance_check(
+                    station_frequencies=self.metadf["dataset_resolution"],
+                    obsdf=self.df,
+                    obstype=obstype,
+                    checks_info=self.settings.qc["qc_checks_info"],
+                    checks_settings=self.settings.qc["qc_check_settings"],
+                )
+
+                # update the dataset and outliers
+                self.df = obsdf
+                if not outl_df.empty:
+                    self.outliersdf = pd.concat([self.outliersdf, outl_df])
+
+                # add this check to the applied checks
+                self._applied_qc = pd.concat(
+                    [
+                        self._applied_qc,
+                        conv_applied_qc_to_df(
+                            obstypes=obstype, ordered_checknames="persistance"
+                        ),
+                    ],
+                    ignore_index=True,
+                )
+
+            else:
+                 logger.warning(f'The persistance check can NOT be applied on {obstype} because it was already applied on this observation type!')
+
+        if step:
+            logger.info("Applying step-check.")
+
+            apliable = _can_qc_be_applied(self._applied_qc, obstype, "step")
+
+            if apliable:
+
+                obsdf, outl_df = step_check(
+                    obsdf=self.df,
+                    obstype=obstype,
+                    checks_info=self.settings.qc["qc_checks_info"],
+                    checks_settings=self.settings.qc["qc_check_settings"],
+                )
+
+                # update the dataset and outliers
+                self.df = obsdf
+                if not outl_df.empty:
+                    self.outliersdf = pd.concat([self.outliersdf, outl_df])
+
+                # add this check to the applied checks
+                self._applied_qc = pd.concat(
+                    [
+                        self._applied_qc,
+                        conv_applied_qc_to_df(obstypes=obstype, ordered_checknames="step"),
+                    ],
+                    ignore_index=True,
+                )
+
+            else:
+                 logger.warning(f'The step check can NOT be applied on {obstype} because it was already applied on this observation type!')
+
+        if window_variation:
+            logger.info("Applying window variation-check.")
+
+            apliable = _can_qc_be_applied(self._applied_qc, obstype, "window_variation")
+            if apliable:
+
+                obsdf, outl_df = window_variation_check(
+                    station_frequencies=self.metadf["dataset_resolution"],
+                    obsdf=self.df,
+                    obstype=obstype,
+                    checks_info=self.settings.qc["qc_checks_info"],
+                    checks_settings=self.settings.qc["qc_check_settings"],
+                )
+
+                # update the dataset and outliers
+                self.df = obsdf
+                if not outl_df.empty:
+                    self.outliersdf = pd.concat([self.outliersdf, outl_df])
+
+                # add this check to the applied checks
+                self._applied_qc = pd.concat(
+                    [
+                        self._applied_qc,
+                        conv_applied_qc_to_df(
+                            obstypes=obstype, ordered_checknames="window_variation"
+                        ),
+                    ],
+                    ignore_index=True,
+                )
+
+            else:
+                 logger.warning(f'The window_variation check can NOT be applied on {obstype} because it was already applied on this observation type!')
+
+
+        self._qc_checked_obstypes.append(obstype)
+        self._qc_checked_obstypes = list(set(self._qc_checked_obstypes))
+        self.outliersdf = self.outliersdf.sort_index()
+
+    def apply_titan_buddy_check(self, obstype='temp', use_constant_altitude=False):
+        """
+        Apply the TITAN buddy check on the observations.
+
+        The buddy check compares an observation against its neighbours (i.e. buddies). The check looks for
+        buddies in a neighbourhood specified by a certain radius. The buddy check flags observations if the
+        (absolute value of the) difference between the observations and the average of the neighbours
+        normalized by the standard deviation in the circle is greater than a predefined threshold.
+
+        See the [titanlib documentation on the buddy check](https://github.com/metno/titanlib/wiki/Buddy-check)
+        for futher details.
+
+        The observation and outliers attributes will be updated accordingly.
+
+        Parameters
+        ----------
+        obstype : String, optional
+            Name of the observationtype you want to apply the checks on. The
+            default is 'temp'.
+        use_constant_altitude : bool, optional
+            Use a constant altitude for all stations. The default is False.
+
+        Returns
+        -------
+        None.
+
+        Note
+        -------
+        To update the check settings, use the update_titan_qc_settings method
+        of the Dataset class.
+
+        """
+
+        logger.info("Applying the titan buddy check")
+
+        checkname = 'titan_buddy_check'
+
+        # 1. coordinates are available?
+        if self.metadf['lat'].isnull().any():
+            logger.warning(f'Not all coordinates are available, the {checkname} cannot be executed!')
+            return
+        if self.metadf['lon'].isnull().any():
+            logger.warning(f'Not all coordinates are available, the {checkname} cannot be executed!')
+            return
+
+
+        # set constant altitude if needed:
+
+        # if altitude is already available, save it to restore it after this check
+        restore_altitude = False
+        if (use_constant_altitude):
+            if ('altitulde' in self.metadf.columns):
+                self.metadf['altitude_backup'] = self.metadf['altitude']
+                restore_altitude=True
+
+            self.metadf['altitude'] = 2. #absolut value does not matter
+
+
+        # 2. altitude available?
+        if ((not use_constant_altitude) & ('altitude' not in self.metadf.columns)):
+            logger.warning(f'The altitude is not known for all stations. The {checkname} cannot be executed!')
+            logger.info('(To resolve this error you can: \n *Use the Dataset.get_altitude() method \n *Set use_constant_altitude to True \n update the "altitude" column in the metadf attribute of your Dataset.')
+            return
+        if ((not use_constant_altitude) & (self.metadf['altitude'].isnull().any())):
+            logger.warning(f'The altitude is not known for all stations. The {checkname} cannot be executed!')
+            logger.info('(To resolve this error you can: \n *Use the Dataset.get_altitude() method \n *Set use_constant_altitude to True \n *Update the "altitude" column in the metadf attribute of your Dataset.)')
+            return
+
+        apliable = _can_qc_be_applied(self._applied_qc, obstype, checkname)
+        if apliable:
+            obsdf, outliersdf = titan_buddy_check(obsdf = self.df,
+                                               metadf = self.metadf,
+                                               obstype = obstype,
+                                               checks_info = self.settings.qc["qc_checks_info"],
+                                               checks_settings = self.settings.qc['titan_check_settings'][checkname][obstype],
+                                               titan_specific_labeler = self.settings.qc['titan_specific_labeler'][checkname])
 
-            obsdf, outl_df = persistance_check(
-                station_frequencies=self.metadf["dataset_resolution"],
-                obsdf=self.df,
-                obstype=obstype,
-                checks_info=self.settings.qc["qc_checks_info"],
-                checks_settings=self.settings.qc["qc_check_settings"],
-            )
 
             # update the dataset and outliers
             self.df = obsdf
-            if not outl_df.empty:
-                self.outliersdf = pd.concat([self.outliersdf, outl_df])
+            if not outliersdf.empty:
+                self.outliersdf = pd.concat([self.outliersdf, outliersdf])
 
             # add this check to the applied checks
             self._applied_qc = pd.concat(
                 [
                     self._applied_qc,
                     conv_applied_qc_to_df(
-                        obstypes=obstype, ordered_checknames="persistance"
+                        obstypes=obstype, ordered_checknames=checkname
                     ),
                 ],
                 ignore_index=True,
             )
 
-        if step:
-            print("Applying the step-check on all stations.")
-            logger.info("Applying step-check on the full dataset")
+        else:
+            logger.warning(f'The {checkname} can NOT be applied on {obstype} because it was already applied on this observation type!')
 
-            obsdf, outl_df = step_check(
-                obsdf=self.df,
-                obstype=obstype,
-                checks_info=self.settings.qc["qc_checks_info"],
-                checks_settings=self.settings.qc["qc_check_settings"],
-            )
 
-            # update the dataset and outliers
-            self.df = obsdf
-            if not outl_df.empty:
-                self.outliersdf = pd.concat([self.outliersdf, outl_df])
+        # Revert artificial data that has been added if needed
+        if restore_altitude: #altitude was overwritten, thus revert it
+            self.metadf['altitude'] = self.metadf["altitude_backup"]
+            self.metadf = self.metadf.drop(columns=['altitude_backup'])
 
-            # add this check to the applied checks
-            self._applied_qc = pd.concat(
-                [
-                    self._applied_qc,
-                    conv_applied_qc_to_df(obstypes=obstype, ordered_checknames="step"),
-                ],
-                ignore_index=True,
-            )
+        elif (use_constant_altitude):
+            # when no alitude was available apriori, remove the fake constant altitude column
+            self.metadf = self.metadf.drop(columns=['altitude'])
 
-        if window_variation:
-            print("Applying the window variation-check on all stations.")
-            logger.info("Applying window variation-check on the full dataset")
 
-            obsdf, outl_df = window_variation_check(
-                station_frequencies=self.metadf["dataset_resolution"],
-                obsdf=self.df,
-                obstype=obstype,
-                checks_info=self.settings.qc["qc_checks_info"],
-                checks_settings=self.settings.qc["qc_check_settings"],
-            )
+
+
+
+    def apply_titan_sct_resistant_check(self, obstype='temp'):
+        """
+        Apply the TITAN spatial consistency test (resistant) on the observations.
+
+        The SCT resistant check is a spatial consistency check which compares each observations to what is expected given the other observations in the
+        nearby area. If the deviation is large, the observation is removed. The SCT uses optimal interpolation
+        (OI) to compute an expected value for each observation. The background for the OI is computed from
+        a general vertical profile of observations in the area.
+
+        See the [titanlib documentation on the buddy check](https://github.com/metno/titanlib/wiki/Spatial-consistency-test-resistant)
+        for futher details.
+
+        The observation and outliers attributes will be updated accordingly.
+
+
+        Parameters
+        ----------
+        obstype : String, optional
+            Name of the observationtype you want to apply the checks on. The
+            default is 'temp'.
+
+        Returns
+        -------
+        None.
+
+        Note
+        -------
+        To update the check settings, use the update_titan_qc_settings method
+        of the Dataset class.
+
+        Warning
+        -------
+        This method is a python wrapper on titanlib c++ scripts, and it is prone
+        to segmentation faults. The perfomance of this check is thus not
+        guaranteed!
+
+        """
+
+
+
+        logger.info("Applying the titan SCT check")
+
+
+        checkname ='titan_sct_resistant_check'
+        # check if required metadata is available:
+
+        # 1. coordinates are available?
+        if self.metadf['lat'].isnull().any():
+            logger.warning(f'Not all coordinates are available, the {checkname} cannot be executed!')
+            return
+        if self.metadf['lon'].isnull().any():
+            logger.warning(f'Not all coordinates are available, the {checkname} cannot be executed!')
+            return
+
+
+        # 2. altitude available?
+        if ('altitude' not in self.metadf.columns):
+            logger.warning(f'The altitude is not known for all stations. The {checkname} cannot be executed!')
+            logger.info('(To resolve this error you can: \n *Use the Dataset.get_altitude() method \n *Set use_constant_altitude to True \n update the "altitude" column in the metadf attribute of your Dataset.')
+            return
+        if (self.metadf['altitude'].isnull().any()):
+            logger.warning(f'The altitude is not known for all stations. The {checkname} cannot be executed!')
+            logger.info('(To resolve this error you can: \n *Use the Dataset.get_altitude() method \n *Set use_constant_altitude to True \n *Update the "altitude" column in the metadf attribute of your Dataset.)')
+            return
+
+        apliable = _can_qc_be_applied(self._applied_qc, obstype, checkname)
+        if apliable:
+
+            obsdf, outliersdf = titan_sct_resistant_check(obsdf = self.df,
+                                               metadf = self.metadf,
+                                               obstype = obstype,
+                                               checks_info = self.settings.qc["qc_checks_info"],
+                                               checks_settings = self.settings.qc['titan_check_settings'][checkname][obstype],
+                                               titan_specific_labeler = self.settings.qc['titan_specific_labeler'][checkname])
 
             # update the dataset and outliers
             self.df = obsdf
-            if not outl_df.empty:
-                self.outliersdf = pd.concat([self.outliersdf, outl_df])
+            if not outliersdf.empty:
+                self.outliersdf = pd.concat([self.outliersdf, outliersdf])
 
             # add this check to the applied checks
             self._applied_qc = pd.concat(
                 [
                     self._applied_qc,
                     conv_applied_qc_to_df(
-                        obstypes=obstype, ordered_checknames="window_variation"
+                        obstypes=obstype, ordered_checknames=checkname
                     ),
                 ],
                 ignore_index=True,
             )
 
-        self._qc_checked_obstypes.append(obstype)
-        self._qc_checked_obstypes = list(set(self._qc_checked_obstypes))
-        self.outliersdf = self.outliersdf.sort_index()
+
+        else:
+            logger.warning(f'The {checkname} can NOT be applied on {obstype} because it was already applied on this observation type!')
+
 
 
 
     def combine_all_to_obsspace(self, repr_outl_as_nan=False,
                                 overwrite_outliers_by_gaps_and_missing=True):
-        
+
         """
          Combine all observations, outliers, missing observations and gaps into
          one Dataframe. All observation types are combined an a label is added
-         in a serperate column. 
+         in a serperate column.
 
          When gaps and missing records are updated from outliers one has to choice
          to represent these records as outliers or gaps. There can not be duplicates
-         in the return dataframe. 
+         in the return dataframe.
 
-         By default the observation values of the outliers are saved, one can 
+         By default the observation values of the outliers are saved, one can
          choice to use these values or NaN's.
          following checks!
 
-        
+
 
          Parameters
          ----------
          repr_outl_as_nan : bool, optional
              If True, Nan's are use for the values of the outliers. The
              default is False.
          overwrite_outliers_by_gaps_and_missing : Bool, optional
@@ -1331,38 +1872,39 @@
              observations are updated from the outliers. The default
              is True.
 
          Returns
          ---------
          combdf : pandas.DataFrame()
             A dataframe containing a continious time resolution of records, where each
-            record is labeld. 
+            record is labeld.
 
         """
 
 
 
 
         # TODO: label values from settings not hardcoding
 
         # =============================================================================
         # Stack outliers
         # =============================================================================
 
-        outliersdf = self.outliersdf
+        outliersdf = self.outliersdf.copy()
         outliersdf['toolkit_representation'] = 'outlier'
         # TODO: use the repr_outl_as_nan argumenten here
         # =============================================================================
         # Stack observations
         # =============================================================================
         df = self.df
         # better save than sorry
         present_obstypes = [col for col in df if col in observation_types]
         df = df[present_obstypes]
 
+
         # to tripple index
         df = df.stack(dropna=False).reset_index().rename(columns={'level_2': 'obstype', 0: 'value'}).set_index(['name', 'datetime', 'obstype'])
 
         df['label'] = 'ok'
         df['toolkit_representation'] = 'observation'
 
         # remove outliers from the observations
@@ -1409,15 +1951,14 @@
         # Stack missing
         # =============================================================================
 
         missingfilldf = self.missing_fill_df.copy()
         missingfilldf = value_labeled_doubleidxdf_to_triple_idxdf(missingfilldf)
         missingfilldf['toolkit_representation'] = 'missing observation fill'
 
-
         # add missing observations if they occure in observation space
         missingidx = self.missing_obs.get_missing_indx_in_obs_space(
             self.df, self.metadf["dataset_resolution"]
         )
 
         missingdf = pd.DataFrame(index=missingidx, columns=present_obstypes)
 
@@ -1438,40 +1979,40 @@
 
 
         # =============================================================================
         # combine all
         # =============================================================================
 
         combdf = pd.concat([df, outliersdf, gapsdf, gapsfilldf, missingdf, missingfilldf]).sort_index()
-
+        combdf.index.names = ['name', 'datetime', 'obstype']
         # To be shure?
         combdf = combdf[~combdf.index.duplicated(keep='first')]
         return combdf
 
 
 
 
-    def get_qc_stats(self, obstype="temp", stationnames=None, make_plot=True):
+    def get_qc_stats(self, obstype="temp", stationname=None, make_plot=True):
         """
         Compute frequency statistics on the qc labels for an observationtype.
         The output is a dataframe containing the frequency statistics presented
         as percentages.
 
         These frequencies can also be presented as a collection of piecharts
         per check.
 
         With stationnames you can subset the data to one ore multiple stations.
 
         Parameters
 
-        obstype : Str, optional
+        obstype : str, optional
             Observation type to analyse the QC labels on. The default is
             'temp'.
-        stationnames : List, Str, optional
-            Stationname(s) to subset the quality labels on. If None, all
+        stationname : str, optional
+            Stationname to subset the quality labels on. If None, all
             stations are used. The default is None.
         make_plot : Bool, optional
             If True, a plot with piecharts is generated. The default is True.
 
         Returns
 
         dataset_qc_stats : pandas.DataFrame
@@ -1480,37 +2021,52 @@
 
         """
 
         # cobmine all and get final label
         comb_df = self.combine_all_to_obsspace()
 
         # subset to relevant columnt
-        comb_df = comb_df.xs(obstype, level='obstype')[['label']]
+        comb_df = xs_save(comb_df, obstype, level='obstype')[['label']]
+
+        # subset to stationnames
+        if not stationname is None:
+            assert stationname in comb_df.index.get_level_values('name'), f' stationnames: {stationname} is not a list.'
+
+            comb_df = comb_df.loc[stationname]
+
 
 
         # compute freq statistics
         final_freq, outl_freq, specific_freq = get_freq_statistics(
             comb_df=comb_df,
             obstype=obstype,
             checks_info=self.settings.qc["qc_checks_info"],
             gaps_info=self.settings.gap["gaps_info"],
             applied_qc_order=self._applied_qc,
         )
 
         if any([stat is None for stat in [final_freq, outl_freq, specific_freq]]):
             return None
 
+        # make title
+        if stationname is None:
+            title='Label frequency statistics on all stations.'
+        else:
+            title=f'Label frequency statistics for {stationname}'
+
+
         if make_plot:
             # make pie plots
             qc_stats_pie(
                 final_stats=final_freq,
                 outlier_stats=outl_freq,
                 specific_stats=specific_freq,
                 plot_settings=self.settings.app["plot_settings"],
                 qc_check_info=self.settings.qc["qc_checks_info"],
+                title=title,
             )
 
         return (final_freq, outl_freq, specific_freq)
 
     def update_outliersdf(self, add_to_outliersdf):
         """V5"""
 
@@ -1565,16 +2121,27 @@
         if origin_tz is None:
             origin_tz = self.settings.time_settings["timezone"]
 
         logger.info(
             f"Coarsening the timeresolution to {freq} using \
                     the {method}-method (with limit={limit})."
         )
+
+        # test if coarsening the resolution is valid for the dataset
+        # 1. If resolution-dep-qc is applied --> coarsening is not valid and will result in a broken dataset
+
+        if self._applied_qc[~self._applied_qc['checkname']
+                            .isin(["duplicated_timestamp", "invalid_input"])
+                            ].shape[0] > 0:
+            logger.warning('Coarsening time resolution is not possible because quality control checks that are resolution depening are already performed on the Dataset.')
+            logger.info('(Apply coarsening_time_resolution BEFORE applying quality control.)')
+            return
+
+
         # TODO: implement buffer method
-        # TODO: implement startdt point
         df = self.df.reset_index()
 
         if origin is None:
             # find earlyest timestamp, if it is on the hour, use it else use the following hour
             tstart = df["datetime"].min()
 
             if tstart.minute != 0 or tstart.second != 0 or tstart.microsecond != 0:
@@ -1601,15 +2168,15 @@
                 df.set_index("datetime")
                 .groupby("name")
                 .resample(freq, origin=tstart)
                 .bfill(limit=limit)
             )
 
         else:
-            print(f"The coarsening method: {method}, is not implemented yet.")
+            logger.warning(f"The coarsening method: {method}, is not implemented yet.")
             df = df.set_index(["name", "datetime"])
 
         if "name" in df.columns:
             df = df.drop(columns=["name"])
 
         # Update resolution info in metadf
         self.metadf["dataset_resolution"] = pd.to_timedelta(freq)
@@ -1657,16 +2224,21 @@
         Returns
         -------
         pandas.DataFrame (if verbose is True)
             A dataframe containing the original observations with original timestamps and the corresponding target timestamps.
 
         """
 
+        # get columns pressent in metadf, because the input df can have columns
+        # that does not have to be mapped to the toolkit
+
 
+        assert not self.input_df.empty, f'To syncronize a dataset, the (pure) input dataframe cannot be empty.'
 
+        init_meta_cols = self.metadf.columns.copy()
         df = self.input_df
 
         self.df = init_multiindexdf()
         self.outliersdf = init_triple_multiindexdf()
         self.gapfilldf = init_multiindexdf()
         self.missing_obs = None
         self.gaps = None
@@ -1705,15 +2277,15 @@
 
         merged_df = pd.DataFrame()
         _total_verbose_df = pd.DataFrame()
         for occur_res in occuring_resolutions:
             group_stations = simplified_resolution[
                 simplified_resolution == occur_res
             ].index.to_list()
-            print(
+            logger.info(
                 f" Grouping stations with simplified resolution of {pd.to_timedelta(occur_res)}: {group_stations}"
             )
             groupdf = df[df["name"].isin(group_stations)]
 
             tstart = groupdf["datetime"].min()
             tend = groupdf["datetime"].max()
 
@@ -1778,27 +2350,38 @@
             freq_estimation_method="highest",
             freq_estimation_simplify=False,
             freq_estimation_simplify_error=None,
             fixed_freq_series=simplified_resolution,
             update_full_metadf=False,
         )  # Do not overwrite full metadf, only the frequencies
 
+        self.metadf = self.metadf[[col for col in self.metadf.columns if col in init_meta_cols]]
+
         if verbose:
             _total_verbose_df = _total_verbose_df.rename(
                 columns={"datetime": "original_datetime", "target_datetime": "datetime"}
             ).set_index(["name", "datetime"])
             return _total_verbose_df
 
+
+
     def import_data_from_file(
         self,
         long_format=True,
         obstype=None,
+
+        obstype_dtype = None,
+        obstype_unit = None,
+        obstype_description = None,
+
         freq_estimation_method=None,
         freq_estimation_simplify=None,
         freq_estimation_simplify_error=None,
+        kwargs_data_read = {},
+        kwargs_metadata_read = {},
     ):
 
         """
         Read observations from a csv file as defined in the
         Settings.input_file. The input file columns should have a template
         that is stored in Settings.template_list.
 
@@ -1844,22 +2427,28 @@
             The default is None.
         freq_estimation_simplify_error : Timedelta or str, optional
             The tollerance string or object representing the maximum translation in time to form a simplified frequency estimation.
             Ex: '5T' is 5 minuts, '1H', is one hour. If None, the method
             stored in the
             Dataset.settings.time_settings['freq_estimation_simplify_error'] is
             used. The default is None.
+        kwargs_data_read : dict, optional
+            Keyword arguments collected in a dictionary to pass to the
+            pandas.read_csv() function on the data file. The default is {}.
+        kwargs_metadata_read : dict, optional
+            Keyword arguments collected in a dictionary to pass to the
+            pandas.read_csv() function on the metadata file. The default is {}.
 
         Returns
         -------
         None.
 
         """
 
-        print("Settings input data file: ", self.settings.IO["input_data_file"])
+
         logger.info(f'Importing data from file: {self.settings.IO["input_data_file"]}')
 
         if freq_estimation_method is None:
 
             freq_estimation_method = self.settings.time_settings[
                 "freq_estimation_method"
             ]
@@ -1874,24 +2463,28 @@
 
         # check if obstype is valid
         if not obstype is None:
             assert (
                 obstype in observation_types
             ), f'{obstype} is not a default obstype. Use one of: {self.settings.app["observation_types"]}'
 
-
         # Read observations into pandas dataframe
+
         df, template = import_data_from_csv(
             input_file=self.settings.IO["input_data_file"],
             template_file=self.settings.templates["data_template_file"],
             long_format=long_format,
             obstype=obstype,  # only relevant in wide format
+            obstype_units = obstype_unit, # only relevant in wide format
+            obstype_description = obstype_description, # only relevant in wide format
+            kwargs_data_read = kwargs_data_read
         )
 
 
+
         # Set timezone information
         df.index = df.index.tz_localize(
             tz=self.settings.time_settings["timezone"],
             ambiguous="infer",
             nonexistent="shift_forward",
         )
 
@@ -1899,41 +2492,64 @@
             f'Data from {self.settings.IO["input_data_file"]} \
                      imported to dataframe.'
         )
 
         # drop Nat datetimes if present
         df = df.loc[pd.notnull(df.index)]
 
-        if not "name" in df.columns:
-            logger.warning(
-                f'No station names find in the observations! \
-                           Assume the dataset is for ONE station with the \
-                         default name: {self.settings.app["default_name"]}.'
-            )
-            df["name"] = str(self.settings.app["default_name"])
+
 
         if self.settings.IO["input_metadata_file"] is None:
-            print(
-                "WARNING: No metadata file is defined.\
-                  Add your settings object."
-            )
             logger.warning(
                 "No metadata file is defined,\
                     no metadata attributes can be set!"
             )
+
+            # if no metadata is given, and no stationname found, assume one station
+            # with default name
+            if not "name" in df.columns:
+                logger.warning(
+                    f'No station names find in the observations! \
+                               Assume the dataset is for ONE station with the \
+                             default name: {self.settings.app["default_name"]}.'
+                )
+                df["name"] = str(self.settings.app["default_name"])
+
         else:
             logger.info(
                 f'Importing metadata from file:\
                         {self.settings.IO["input_metadata_file"]}'
             )
             meta_df = import_metadata_from_csv(
                 input_file=self.settings.IO["input_metadata_file"],
                 template_file=self.settings.templates["metadata_template_file"],
+                kwargs_metadata_read = kwargs_metadata_read,
             )
 
+
+            # in dataset of one station, the name is most often not present!
+            if not "name" in df.columns:
+                logger.warning(f'No station names find in the observations!' )
+
+                # If there is ONE name in the metadf, than we use that name for
+                # the df, else we use the default name
+                if (('name' in meta_df.columns) & (meta_df.shape[0] == 1)):
+                    name = meta_df['name'].iloc[0]
+                    df['name'] = name
+                    logger.warning(f'One stationname found in the metadata: {name}, this name is used for the data.')
+                else:
+                    df["name"] = str(self.settings.app["default_name"])
+                    # for later merging, we add the name column with the default
+                    # also in the metadf
+                    meta_df['name'] =str(self.settings.app["default_name"])
+                    logger.warning(
+                        f'Assume the dataset is for ONE station with the \
+                        default name: {self.settings.app["default_name"]}.')
+
+
             # merge additional metadata to observations
             meta_cols = [
                 colname for colname in meta_df.columns if not colname.startswith("_")
             ]
             additional_meta_cols = list(set(meta_cols).difference(df.columns))
 
             if bool(additional_meta_cols):
@@ -1961,81 +2577,81 @@
         self._construct_dataset(
             df=df,
             freq_estimation_method=freq_estimation_method,
             freq_estimation_simplify=freq_estimation_simplify,
             freq_estimation_simplify_error=freq_estimation_simplify_error,
         )
 
-    def import_data_from_database(
-        self, start_datetime=None, end_datetime=None, coarsen_timeres=False
-    ):
-        """
-        Function to import data directly from the framboos database and
-        updating the network and station objects.
-
-
-        Parameters
-        ----------
-
-        start_datetime : datetime, optional
-            Start datetime of the observations. The default is None and using
-            yesterday's midnight.
-        end_datetime : datetime, optional
-            End datetime of the observations. The default is None and using
-            todays midnight.
-        coarsen_timeres : Bool, optional
-            If True, the observations will be interpolated to a coarser
-            time resolution as is defined in the Settings. The default
-            is False.
-
-        Returns
-        ----------
-
-        None.
+    # def import_data_from_database(
+    #     self, start_datetime=None, end_datetime=None, coarsen_timeres=False
+    # ):
+    #     """
+    #     Function to import data directly from the framboos database and
+    #     updating the network and station objects.
 
-        Note
-        ----------
-        A Ugent VPN connection must be present, as well as the username and password
-        stored in the settings.
 
-        """
-        if start_datetime is None:
-            start_datetime = datetime.date.today() - datetime.timedelta(days=1)
-        if end_datetime is None:
-            end_datetime = datetime.date.today()
+    #     Parameters
+    #     ----------
 
-        # Read observations into pandas dataframe
-        df = import_data_from_db(
-            self.settings.db, start_datetime=start_datetime, end_datetime=end_datetime
-        )
+    #     start_datetime : datetime, optional
+    #         Start datetime of the observations. The default is None and using
+    #         yesterday's midnight.
+    #     end_datetime : datetime, optional
+    #         End datetime of the observations. The default is None and using
+    #         todays midnight.
+    #     coarsen_timeres : Bool, optional
+    #         If True, the observations will be interpolated to a coarser
+    #         time resolution as is defined in the Settings. The default
+    #         is False.
 
-        if df.empty:  # No data has, probably connection error
-            return
+    #     Returns
+    #     ----------
 
-        # Make data template
-        self.data_template = pd.DataFrame().from_dict(
-            template_to_package_space(self.settings.db["vlinder_db_obs_template"])
-        )
+    #     None.
 
-        # convert dataframe to multiindex (datetime - name)
-        df = df.set_index(["name", df.index])
-        df = df.sort_index()
+    #     Note
+    #     ----------
+    #     A Ugent VPN connection must be present, as well as the username and password
+    #     stored in the settings.
 
-        # If an ID has changed or not present in the metadatafile,
-        # the stationname and metadata is Nan
-        # These observations will be removed
-        unknown_obs = df[df.index.get_level_values("name").isnull()]
-        if not unknown_obs.empty:
-            logger.warning(
-                "There is an unknown station in the dataset \
-                           (probaply due to an ID that is not present in \
-                           the metadata file). This will be removed from the dataset."
-            )
-            df = df[~df.index.get_level_values("name").isnull()]
-        self._construct_dataset(df)
+    #     """
+    #     if start_datetime is None:
+    #         start_datetime = datetime.date.today() - datetime.timedelta(days=1)
+    #     if end_datetime is None:
+    #         end_datetime = datetime.date.today()
+
+    #     # Read observations into pandas dataframe
+    #     df = import_data_from_db(
+    #         self.settings.db, start_datetime=start_datetime, end_datetime=end_datetime
+    #     )
+
+    #     if df.empty:  # No data has, probably connection error
+    #         return
+
+    #     # Make data template
+    #     self.data_template = pd.DataFrame().from_dict(
+    #         template_to_package_space(self.settings.db["vlinder_db_obs_template"])
+    #     )
+
+    #     # convert dataframe to multiindex (datetime - name)
+    #     df = df.set_index(["name", df.index])
+    #     df = df.sort_index()
+
+    #     # If an ID has changed or not present in the metadatafile,
+    #     # the stationname and metadata is Nan
+    #     # These observations will be removed
+    #     unknown_obs = df[df.index.get_level_values("name").isnull()]
+    #     if not unknown_obs.empty:
+    #         logger.warning(
+    #             "There is an unknown station in the dataset \
+    #                        (probaply due to an ID that is not present in \
+    #                        the metadata file). This will be removed from the dataset."
+    #         )
+    #         df = df[~df.index.get_level_values("name").isnull()]
+    #     self._construct_dataset(df)
 
 
     def _construct_dataset(
         self,
         df,
         freq_estimation_method,
         freq_estimation_simplify,
@@ -2135,15 +2751,27 @@
             metadf.index = metadf.index.droplevel("datetime")  # drop datetimeindex
             # drop dubplicates due to datetime
             metadf = metadf[~metadf.index.duplicated(keep="first")]
 
             self.metadf = metadf_to_gdf(metadf)
 
 
+
+
+
     def _apply_qc_on_import(self):
+        # if the name is Nan, remove these records from df, and metadf (before)
+        # they end up in the gaps and missing obs
+        if np.nan in self.df.index.get_level_values('name'):
+            logger.warning(f'Following observations are not linked to a station name and will be removed: {xs_save(self.df, np.nan, "name")}')
+            self.df = self.df[~self.df.index.get_level_values('name').isna()]
+        if np.nan in self.metadf.index:
+            logger.warning(f'Following station will be removed from the Dataset {self.metadf[self.metadf.index.isna()]}')
+            self.metadf = self.metadf[~self.metadf.index.isna()]
+
         # find missing obs and gaps, and remove them from the df
         self.missing_obs, self.gaps = missing_timestamp_and_gap_check(
             df=self.df,
             gapsize_n=self.settings.gap["gaps_settings"]["gaps_finder"]["gapsize_n"],
         )
 
         # Create gaps and missing obs objects
@@ -2184,15 +2812,15 @@
 
     # =============================================================================
     # Physiography extractions
     # =============================================================================
 
     def get_lcz(self):
         """
-        Function to extract the Local CLimate zones (LCZ) from the 
+        Function to extract the Local CLimate zones (LCZ) from the
         wudapt global LCZ map on the Google engine for all stations.
 
         A 'LCZ' column will be added to the metadf, and series is returned.
 
         Returns
         -------
         lcz_series : pandas.Series()
@@ -2279,15 +2907,15 @@
         """
         # connect to gee
         connect_to_gee()
 
         df_list = []
         for buffer in buffers:
 
-            print(f'Extracting landcover from {gee_map} with buffer radius = {buffer}')
+            logger.info(f'Extracting landcover from {gee_map} with buffer radius = {buffer}')
             # Extract landcover fractions for all stations
             lc_frac_df, buffer = lc_fractions_extractor(
                 metadf=self.metadf,
                 mapinfo=self.settings.gee["gee_dataset_info"][gee_map],
                 buffer=buffer,
                 agg=aggregate,
             )
@@ -2305,14 +2933,209 @@
         frac_df = pd.concat(df_list)
         frac_df = frac_df.sort_index()
 
 
         if overwrite:
 
             for buf in frac_df.index.get_level_values('buffer_radius').unique():
-                buf_df = frac_df.xs(buf, level='buffer_radius')
+                buf_df = xs_save(frac_df, buf, level='buffer_radius')
                 buf_df.columns= [col + f'_{int(buf)}m' for col in buf_df.columns]
 
                 # overwrite the columns or add them if they did not exist
                 self.metadf[buf_df.columns] = buf_df
 
         return frac_df
+    def fairness_coordinates_for_alaro_25_csv_creator(self, outputfolder=None,
+                    filename='summerschool_modeldata_metadata.csv',
+                    lat_min=None, lon_min=None,
+                    lat_max=None, lon_max=None):
+        """
+        This is for the participants of the Cost FAIRNESS Summerschool in Ghent.
+        It will create a small csv file with the locations and names of your stations.
+        This information is needed to extract timeseries of Alaro 2.5km modeldata.
+
+        A spatial plot will be provided aswell. If no bounding box coordinates are given,
+        a boundingboux is create to encapsulate your stations.
+
+        A csv file will be saved in the outputfolder. Email this file to mivieijra@meteo.be.
+
+        Parameters
+        ----------
+        outputfolder : string, optional
+            The autput folder to store the csv file. If None, the default
+            autputfolder will be used. The default is None.
+        filename : string, optional
+            Name of the csv file. The default is
+            'summerschool_modeldata_metadata.csv'.
+        lat_min : num, optional
+            Minimum latitude of the bounding box. If None, a boundingbox will
+            be computed that fits your stations. The default is None.
+        lon_min : num, optional
+            Minimum longitude of the bounding box. If None, a boundingbox will
+            be computed that fits your stations. The default is None.
+        lat_max : num, optional
+            Maximum latitude of the bounding box. If None, a boundingbox will
+            be computed that fits your stations. The default is None.
+        lon_max : num, optional
+            Maximum longitude of the bounding box. If None, a boundingbox will
+            be computed that fits your stations. The default is None.
+
+        Returns
+        -------
+        None.
+
+        """
+
+        # checks
+        # check if metadata is available
+        if self.metadf['lat'].isnull().all():
+            logger.warning('No coordinates are found in the metadata. A csv cannot be created.')
+            return
+
+        if self.metadf['lon'].isnull().all():
+            logger.warning('No coordinates are found in the metadata. A csv cannot be created.')
+            return
+
+        if ((outputfolder is None) & (self.settings.IO['output_folder'] is None)):
+            logger.warning('No outputfolder is specified.')
+            return
+
+
+        if outputfolder is None:
+            outputfolder =self. settings.IO['output_folder']
+
+        user_bounds = [lat_min, lon_min, lat_max, lon_max]
+        if any([x is None for x in user_bounds]):
+            # use default bounds
+            make_bounds=True
+            logger.info('Since not (all) bounds are given, the bounds are the total bounds of the present stations.')
+        else:
+            make_bounds=False
+
+
+        metadf = self.metadf.copy()
+        metadf= metadf[metadf['lat'].notna()]
+        metadf= metadf[metadf['lon'].notna()]
+
+
+        if make_bounds:
+            # lonmin, latmin, lonmax, latmax
+            bounds = tuple(metadf.total_bounds)
+        else:
+            bounds = tuple([float(lon_min), float(lat_min),
+                            float(lon_max), float(lat_max)])
+
+
+        # add bounds as a column (avoid creating two files with data, and readin in problems in R)
+        metadf['bbox'] = [bounds for _ in range(len(metadf))]
+        # reset index so no problems in R
+        metadf = metadf.reset_index()
+        # subset to relevant columns
+        savedf = metadf[['name', 'lat', 'lon', 'bbox']]
+
+
+        # Write to a csv file
+        if not filename.endswith('.csv'):
+            filename += '.csv'
+
+        filepath = os.path.join(outputfolder, filename)
+        savedf.to_csv(filepath,
+                      sep=',',
+                      index=False,
+                      decimal='.')
+        print(f'\n File is writen to : {filepath}. \n')
+        print('Download the file (as a .csv), and send it by email to:  mivieijra@meteo.be.')
+
+        return
+
+
+
+    def make_gee_plot(self, gee_map, show_stations=True, save=False):
+        """
+        Make an interactive plot of a google earth dataset. The location of the
+        stations can be plotted on top of it.
+
+        Parameters
+        ----------
+        gee_map : str, optional
+            The name of the dataset to use. This name should be present in the
+            settings.gee['gee_dataset_info']. If aggregat is True, an aggregation
+            scheme should included as well. The default is 'worldcover'
+        show_stations : bool, optional
+            If True, the stations will be plotted as markers. The default is True.
+        save : bool, optional
+            If True, the map will be saved as an html file in the output_folder
+            as defined in the settings. The default is False.
+
+        Returns
+        -------
+        Map : geemap.foliumap.Map
+            The folium Map instance.
+
+
+        Warning
+        ---------
+        To display the interactive map a graphical backend is required, which
+        is often missing on (free) cloud platforms. Therefore it is better to
+        set save=True, and open the .html in your browser
+
+        """
+
+        # Connect to GEE
+        connect_to_gee()
+
+        # get the mapinfo
+        mapinfo = self.settings.gee["gee_dataset_info"][gee_map]
+
+
+        #Read in covers, numbers and labels
+        covernum = list(mapinfo['colorscheme'].keys())
+        colors =list(mapinfo['colorscheme'].values())
+        covername = [mapinfo['categorical_mapper'][covnum] for covnum in covernum]
+
+
+        # create visparams
+        vis_params ={
+            'min': min(covernum),
+            'max': max(covernum),
+            'palette': colors #hex colors!
+            }
+
+        if 'band_of_use' in mapinfo:
+            band=mapinfo['band_of_use']
+        else:
+            band=None
+
+        Map = folium_plot(mapinfo = mapinfo,
+                          band = band,
+                          vis_params = vis_params,
+                          labelnames = covername,
+                          layername = gee_map,
+                          legendname=f'{gee_map} covers',
+                          # showmap = show,
+                          )
+        if show_stations:
+            if not _validate_metadf(self.metadf):
+                logger.warning('Not enough coordinates information is provided to plot the stations.')
+            else:
+                Map = add_stations_to_folium_map(Map = Map,
+                                                 metadf = self.metadf)
+
+
+
+
+        # Save if needed
+        if save:
+            if self.settings.IO['output_folder'] is None:
+                logger.warning('The outputfolder is not set up, use the update_settings to specify the output_folder.')
+
+            else:
+                filename = f'gee_{gee_map}_figure.html'
+                filepath = os.path.join(self.settings.IO['output_folder'], filename)
+                print(f'Gee Map will be save at {filepath}')
+                logger.info(f'Gee Map will be save at {filepath}')
+                Map.save(filepath)
+
+
+def _can_qc_be_applied(applied_df, obstype, checkname):
+    """ test if the check is already performed on self """
+    return not applied_df[(applied_df['obstype'] == obstype) & (applied_df['checkname'] == checkname)].shape[0] > 0
```

### Comparing `metobs_toolkit-0.1.1a0/metobs_toolkit/df_helpers.py` & `metobs_toolkit-0.1.1a2/metobs_toolkit/df_helpers.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,14 +10,81 @@
 
 import sys
 import pandas as pd
 import numpy as np
 import geopandas as gpd
 import itertools
 from metobs_toolkit import observation_types
+import pytz
+import logging
+
+logger = logging.getLogger(__name__)
+
+
+
+def fmt_datetime_argument(dt, target_tz_str):
+    """
+    Helper function to format the datetime, a user enters as argument, to the
+    correct timezone.
+
+    If the datetime is timezone unaware, the toolkit ASSUMES the dt is in the
+    same timezone as target_tz_str (the timezone of the dataset).
+
+    if dt is None, None is returned
+    Parameters
+    ----------
+    dt : datetime.datetime
+        A datetime to convert to the timezone of tz_str_data.
+    target_tz_str : str
+        a pytz timezone string, to convert/assign the dt to.
+
+    Returns
+    -------
+    dt : datetime.datetime
+        Timezone-Aware datetime in tzone=tz_str_data.
+
+    """
+    if dt is None:
+        return None
+
+    # check if datime is timezone aware
+    if (dt.tzinfo is not None and dt.tzinfo.utcoffset(dt) is not None):
+        #timezone aware
+        dt = dt.astimezone(pytz.timezone(target_tz_str))
+
+    else: #timezon unaware
+        # assume timezone is the timezone of the data!
+        dt = pytz.timezone(target_tz_str).localize(dt)
+    return dt
+
+
+
+def xs_save(df, key, level, drop_level=True):
+    """ wrapper on pandas xs, but returns an empty df when key is not found """
+    try:
+        return df.xs(key, level=level, drop_level=drop_level)
+    except KeyError:
+        # create empty df with same columns and index names
+        columns = df.columns
+        names = list(df.index.names)
+        if drop_level:
+            names.remove(level)
+
+        levels = [[name] for name in names]
+        codes = [[] for name in names]
+        idx = pd.MultiIndex(
+                            levels=levels,
+                            codes=codes,
+                            names=names,
+                            )
+
+
+    return pd.DataFrame(index=idx, columns=columns)
+
+
 
 
 def init_multiindex():
     return pd.MultiIndex(
         levels=[["name"], ["datetime"]], codes=[[], []], names=["name", "datetime"]
     )
 
@@ -181,16 +248,16 @@
     subset_dt_df = subset_dt_df.reset_index()
     idx = pd.MultiIndex.from_frame(subset_dt_df[["name", "datetime"]])
     returndf = subset_dt_df.set_index(idx).drop(
         columns=["name", "datetime"], errors="ignore"
     )
 
     if returndf.empty:
-        print(
-            f"Warning: No observations left after subsetting datetime {starttime} -- {endtime} "
+        logger.warning(
+            f"No observations left after subsetting datetime {starttime} -- {endtime} "
         )
 
     return returndf
 
 
 
 # =============================================================================
@@ -199,15 +266,15 @@
 def subset_stations(df, stationslist):
     df = df.loc[df.index.get_level_values(
                 'name').isin(stationslist)]
 
     present_stations = df.index.get_level_values('name')
     not_present_stations = list(set(stationslist) - set(present_stations))
     if len(not_present_stations)!=0:
-        print(f'WARNING: The stations: {not_present_stations} not found in the dataframe.')
+        logger.warning(f'The stations: {not_present_stations} not found in the dataframe.')
 
     return df
 
 
 
 def datetime_subsetting(df, starttime, endtime):
     """
@@ -225,31 +292,39 @@
 
     Returns
     -------
     pandas.DataFrame
         Subset of the df.
 
     """
+
     idx_names = list(df.index.names)
     df = df.reset_index()
     df = df.set_index('datetime')
-    stand_format = "%Y-%m-%d %H:%M:%S"
 
     if isinstance(starttime, type(None)):
-        startstring = None  # will select from the beginning of the df
+        starttime = df.index.min() # will select from the beginning of the df
     else:
-        startstring = starttime.strftime(stand_format)
+        if starttime.tzinfo is None:
+            # set timezone when unaware
+            starttime = starttime.replace(tzinfo=df.index.tzinfo)
+
     if isinstance(endtime, type(None)):
-        endstring = None
+        endtime = df.index.max()
     else:
-        endstring = endtime.strftime(stand_format)
+        if endtime.tzinfo is None:
+            # set timezone when unaware
+            endtime = endtime.replace(tzinfo=df.index.tzinfo)
 
-    subset =  df[startstring:endstring]
+
+
+    subset = df[(df.index >= starttime) & (df.index <= endtime)]
     subset = subset.reset_index()
     subset = subset.set_index(idx_names)
+    subset = subset.sort_index()
     return subset
 
 
 def conv_applied_qc_to_df(obstypes, ordered_checknames):
     if isinstance(obstypes, str):
         obstypes = [obstypes]
     if isinstance(ordered_checknames, str):
@@ -313,23 +388,31 @@
     try:
         pd.to_timedelta(max_simplify_error)
     except ValueError:
         sys.exit(
             f'{max_simplify_error} is not valid timeindication. Example: "5T" indicates 5 minutes.'
         )
 
-    freqdist = abs(timestamps.to_series().diff().value_counts().index).sort_values(
-        ascending=True
-    )
+    # freqdist = abs(timestamps.to_series().diff().value_counts()).sort_values(
+    #     ascending=True
+    # )
+    freqs_blacklist = [pd.Timedelta(0), np.nan] #avoid a zero frequency
+
+
+    freqs = timestamps.to_series().diff()
+    freqs = freqs[~freqs.isin(freqs_blacklist)]
+
+
 
     if method == "highest":
-        assume_freq = freqdist[0]  # highest frequency
+
+        assume_freq = freqs.min()  # highest frequency
 
     elif method == "median":
-        assume_freq = freqdist.median()
+        assume_freq = freqs.median()
 
     if simplify:
         simplify_freq = None
 
         # try simplyfy to round hours
         trail_hour = assume_freq.ceil("H")
         lead_hour = assume_freq.floor("H")
@@ -401,23 +484,23 @@
         A pandas series with 'name' as index and likely frequencies as values.
 
     """
 
     problematic_stations = []
     freqs = {}
     for station in df.index.get_level_values(level="name").unique():
-        subdf = df.xs(station, level="name")
+        subdf = xs_save(df, station, level="name")
         # remove rows with all obstype nans
         subdf = subdf.dropna(axis=0, how="all")
 
         # Check if all observations have at least two observations
         if subdf.shape[0] < 2:
             problematic_stations.append(station)
-            print(
-                f"WARNING! Stations {station} have to few observations to make a frequency estimate."
+            logger.warning(
+                f"Stations {station} have to few observations to make a frequency estimate."
             )
             continue
 
         freqs[station] = get_likely_frequency(
             timestamps=subdf.index,
             method=method,
             simplify=simplify,
@@ -425,15 +508,15 @@
         )
 
     if len(problematic_stations) != 0:
         assign_med_freq = pd.to_timedelta(
             np.median([freq.total_seconds() for freq in freqs.values()]), unit="seconds"
         )
 
-        print(
+        logger.warning(
             f"Asigning the median of frequencies ({assign_med_freq}) to these stations {problematic_stations}."
         )
         for prob_station in problematic_stations:
             freqs[prob_station] = assign_med_freq
 
 
     return pd.Series(data=freqs)
```

### Comparing `metobs_toolkit-0.1.1a0/metobs_toolkit/gap.py` & `metobs_toolkit-0.1.1a2/metobs_toolkit/gap.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,13 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 """
+This module contains the Gap class and all its methods.
 
-Specific classes are created because gaps and missing obs can have out-of-sync
-datetimes wrt dataset.df.
-
-Created on Fri Mar  3 09:15:56 2023
-
-@author: thoverga
+A Gap contains all information and methods of a data-gap.
 """
 
 import pandas as pd
 import numpy as np
 import logging
 from datetime import datetime, timedelta
 import math
@@ -25,15 +21,16 @@
 
 from metobs_toolkit.df_helpers import (
     format_outliersdf_to_doubleidx,
     get_likely_frequency,
     _find_closes_occuring_date
 )
 
-from metobs_toolkit.df_helpers import init_multiindex, init_multiindexdf
+from metobs_toolkit import observation_types
+from metobs_toolkit.df_helpers import init_multiindex, init_multiindexdf, xs_save
 
 from metobs_toolkit.missingobs import Missingob_collection
 
 logger = logging.getLogger(__name__)
 
 
 # =============================================================================
@@ -77,54 +74,69 @@
         self.trailing_val = {} #keys are obstypes
 
         self.exp_gap_idx = None
 
         # gap fill (only for conventional saving)
         self.gapfill_df = pd.DataFrame() #index: datetime, columns: obstypes, values: fill_values
         self.gapfill_technique = None #will become a string
-        self.gapfill_info = None #only for the user
+        self.gapfill_info = None # detailed infomation on the gapfill technique (only for the user)
         self.gapfill_errormessage = {} #keys are obstypes
 
 
     def __str__(self):
         return f"Gap instance of {self.name} for {self.startgap} --> {self.endgap}, duration: {self.duration}"
     def __repr__(self):
         return self.__str__()
 
     def get_info(self):
         print(f'Gap for {self.name} with: \n')
         print(f'\n ---- Gap info ----- \n')
+        print('(Note: gaps are defined on the frequency estimation of the native dataset.)')
         print(f'  * Start gap: {self.startgap} \n')
         print(f'  * End gap: {self.endgap} \n')
         print(f'  * Duration gap: {self.duration} \n')
         print(f'\n ---- Gap fill info ----- \n')
-
         obstypes = self.gapfill_df.columns.to_list()
+        obstypes = [obs for obs in obstypes if obs in observation_types]
         if self.gapfill_df.empty:
             print ('(No gapfill applied)')
-        elif self.gapfill_technique == 'interpolation':
+        elif self.gapfill_technique == 'gap_interpolation':
             for obstype in obstypes:
                 print(f'  * On observation type: {obstype}')
                 print(f'  * Technique: {self.gapfill_technique} \n')
-                print(f'  * Leading timestamp: {self.leading_timestamp} with  {obstype} = {self.leading_val[obstype]}\n')
-                print(f'  * Trailing timestamp: {self.trailing_timestamp} with  {obstype} = {self.trailing_val[obstype]}\n')
+                if bool(self.leading_val):
+                    leading_val =self.leading_val[obstype]
+                else:
+                    leading_val = 'No leading observation value'
+                print(f'  * Leading timestamp: {self.leading_timestamp} with  {obstype} = {leading_val}\n')
+                if bool(self.trailing_val):
+                    trailing_val =self.trailing_val[obstype]
+                else:
+                    trailing_val = 'No trailing observation value'
+                print(f'  * Trailing timestamp: {self.trailing_timestamp} with  {obstype} = {trailing_val}\n')
                 print(f'  * Filled values: {self.gapfill_df[obstype]} \n')
                 if obstype in self.gapfill_errormessage:
                     print(f'  * Gapfill message: {self.gapfill_errormessage[obstype]} \n')
+                if not self.gapfill_info is None:
+                    print(f'  * Gapfill info: {self.gapfill_info.head()} \n')
+                    print(f'    (Extract the gapfill info dataframe by using the .gapfill_info attribute) \n')
 
-
-        elif self.gapfill_technique == "debias gapfill":
+        elif self.gapfill_technique == "gap_debiased_era5":
             for obstype in obstypes:
                 print(f'  * On observation type: {obstype}')
                 print(f'  * Technique: {self.gapfill_technique} \n')
                 # print(f'  * Leading timestamp: {self.leading_timestamp} with  {obstype} = {self.leading_val[obstype]}\n')
                 # print(f'  * Trailing timestamp: {self.trailing_timestamp} with  {obstype} = {self.trailing_val[obstype]}\n')
                 print(f'  * Filled values: {self.gapfill_df[obstype]} \n')
                 if obstype in self.gapfill_errormessage:
                     print(f'  * Gapfill message: {self.gapfill_errormessage[obstype]} \n')
+                if not self.gapfill_info is None:
+                    print(f'  * Gapfill info: {self.gapfill_info.head()} \n')
+                    print(f'    (Extract the gapfill info dataframe by using the .gapfill_info attribute) \n')
+
         else:
             print('technique not implemented in yet in show')
 
 
 
     def to_df(self):
         """
@@ -133,20 +145,23 @@
 
         Returns
         -------
         pandas.DataFrame()
             Gap in dataframe format.
 
         """
-        return pd.DataFrame(
+
+        returndf = pd.DataFrame(
             index=[self.name],
             data={"start_gap": self.startgap,
                   "end_gap": self.endgap,
                   "duration": self.duration}
         )
+        returndf.index.name = 'name'
+        return returndf
 
     def update_leading_trailing_obs(self, obsdf, outliersdf, obs_only=False):
         """
         Add the leading (last obs before gap) and trailing (first obs after gap)
         as extra columns to the self.df.
 
         One can specify to look for leading and trailing in the obsdf or in both
@@ -167,22 +182,23 @@
 
         Returns
         -------
         None.
 
         """
 
-        sta_obs = obsdf.xs(self.name, level="name").index
+        sta_obs = xs_save(obsdf, self.name, level="name").index
         if obs_only:
             sta_comb = sta_obs
         else:
+
             outliersdf = format_outliersdf_to_doubleidx(outliersdf)
 
             # combine timestamps of observations and outliers
-            sta_outl = outliersdf.xs(self.name, level="name").index
+            sta_outl = xs_save(outliersdf, self.name, level="name").index
             sta_comb = sta_obs.append(sta_outl)
 
         # find minimium timediff before
         before_diff = _find_closes_occuring_date(
             refdt=self.startgap, series_of_dt=sta_comb, where="before"
         )
 
@@ -202,20 +218,20 @@
         self.leading_timestamp = self.startgap - timedelta(seconds=before_diff)
         self.trailing_timestamp = self.endgap + timedelta(seconds=after_diff)
 
         # get the values
         try:
             self.leading_val = obsdf.loc[(self.name, self.leading_timestamp)].to_dict()
         except KeyError:
-            print('LEADING VAL NOT IN OBSDF --> THIS IS NOT WHAT YOU WHANT I THINK ; FIX THIS')
+            logger.warning('Leading value not found in the observations')
             self.leading_val = {}
         try:
             self.trailing_val = obsdf.loc[(self.name, self.trailing_timestamp)].to_dict()
         except KeyError:
-            print('LEADING VAL NOT IN OBSDF --> THIS IS NOT WHAT YOU WHANT I THINK ; FIX THIS')
+            logger.warning('Trailing value not found in the observations')
             self.trailing_val = {}
 
 
 
     def update_gaps_indx_in_obs_space(self, obsdf, outliersdf, dataset_res):
         """
 
@@ -296,15 +312,15 @@
 
         Returns
         -------
         Pandas.Series
             Multiindex Series with filled gap values in dataset space.
 
         """
-        print(f' interpolate on {self}')
+        logger.info(f' interpolate on {self}')
         outliersdf = format_outliersdf_to_doubleidx(outliersdf)
 
         gapfill_series= interpolate_gap(
             gap=self,
             obsdf=obsdf,
             outliersdf=outliersdf,
             dataset_res=dataset_res,
@@ -404,14 +420,22 @@
     """
 
 
     gapdflist = []
     for gap in gapslist:
         gapdflist.append(gap.to_df())
 
+    if not bool(gapdflist):
+        # when no gaps, make default return
+        default_df = pd.DataFrame(data={'start_gap':[],
+                                        'end_gap':[],
+                                        'duration':[]})
+        default_df.index.name = 'name'
+        return default_df
+
     return pd.concat(gapdflist)
 
 def remove_gaps_from_obs(gaplist, obsdf):
     """
     Remove station - datetime records that are in the gaps from the obsdf.
 
     (Usefull when filling timestamps to a df, and if you whant to remove the
@@ -428,15 +452,15 @@
         The same dataframe with records inside gaps removed.
 
     """
 
     # Create index for gaps records in the obsdf
     expanded_gabsidx = init_multiindex()
     for gap in gaplist:
-        sta_records = obsdf.xs(gap.name, level="name").index  # filter by name
+        sta_records = xs_save(obsdf, gap.name, level="name").index  # filter by name
 
         gaps_dt = sta_records[
             (sta_records >= gap.startgap)
             & (  # filter if the observations are within a gap
                 sta_records <= gap.endgap
             )
         ]
@@ -447,53 +471,77 @@
 
         expanded_gabsidx = expanded_gabsidx.append(gaps_multiidx)
 
     # remove gaps idx from the obsdf
     obsdf = obsdf.drop(index=expanded_gabsidx)
     return obsdf
 
+def remove_gaps_from_outliers(gaplist, outldf):
+    """
+    Remove station - datetime records that are in the gaps from the outliersdf.
+    This will ignore the observation types! So all outliers of any observation
+    type, that are in a gap period, are removed.
+
+
+
+    Parameters
+    ----------
+    obsdf : pandas.DataFrame()
+        A MultiIndex dataframe with name -- datetime -- as index.
+
+    Returns
+    -------
+    obsdf : pandas.DataFrame()
+        The same dataframe with records inside gaps removed.
+
+    """
+
+
+    # to multiindex
+    outldf = outldf.reset_index().set_index(['name', 'datetime'])
+
+    # remove records inside the gaps
+    suboutldf = remove_gaps_from_obs(gaplist = gaplist,
+                                     obsdf = outldf)
+
+    # restet to triple index
+    outldf = suboutldf.reset_index().set_index(['name', 'datetime', 'obstype'])
+
+    return outldf
+
 # =============================================================================
 # Helpers
 # =============================================================================
 
 
-# def _find_closes_occuring_date(refdt, series_of_dt, where="before"):
-#     if where == "before":
-#         diff = refdt - (series_of_dt[series_of_dt < refdt])
-#     elif where == "after":
-#         diff = (series_of_dt[series_of_dt > refdt]) - refdt
-
-#     if diff.empty:
-#         # no occurences before of after
-
-#         return np.nan
-#     else:
-#         return min(diff).total_seconds()
-
 
 
 def apply_debias_era5_gapfill(
         gapslist, dataset, eraModelData, debias_settings, obstype="temp",
-    ):
+        overwrite_fill=False):
 
         gapfill_settings = dataset.settings.gap['gaps_fill_info']
         expanded_gabsidx_obsspace = init_multiindex()
 
         filled_gaps_series = pd.Series(
             data=[], index=expanded_gabsidx_obsspace, dtype=object
         )
 
         # Convert modeldata to the same timzone as the data
         targettz = dataset.df.index.get_level_values('datetime').tz.zone
         eraModelData._conv_to_timezone(targettz)
 
 
         for gap in gapslist:
-            print(f' Era5 gapfill for {gap}')
-            gap.gapfill_technique = "debias gapfill"
+            if (not overwrite_fill) & (not gap.gapfill_df.empty):
+                logger.warning(f'Gap {gap.name} is already filled with {gap.gapfill_technique} and will not be overwirtten. Set overwrite_fill to True to overwrite.')
+                continue
+
+            logger.info(f' Era5 gapfill for {gap}')
+            gap.gapfill_technique = gapfill_settings['label']['model_debias']
 
             # avoid passing full dataset around
             station = dataset.get_station(gap.name)
 
             # Update gap attributes
             gap.update_gaps_indx_in_obs_space(
                 obsdf=station.df,
@@ -507,15 +555,15 @@
                 gap=gap,
                 debias_period_settings=debias_settings["debias_period"],
                 obstype=obstype,
             )
 
             # check if leading/trailing is valid
             if leading_obs.empty | trailing_obs.empty:
-                print(
+                logger.info(
                     "No suitable leading or trailing period found. Gapfill not possible"
                 )
                 gap.gapfill_errormessage[obstype] = 'gapfill not possible: no leading/trailing period'
 
                 default_return = pd.Series(
                     index=gap.exp_gap_idx, name=obstype, dtype="object"
                 )
@@ -533,15 +581,15 @@
             leading_model = eraModelData.interpolate_modeldata(leading_obs.index)
             trailing_model = eraModelData.interpolate_modeldata(trailing_obs.index)
 
             # TODO check if there is modeldata for the leading and trailing + obs period
             if (leading_model[obstype].isnull().any()) | (
                 trailing_model[obstype].isnull().any()
             ):
-                print(
+                logger.info(
                     "No modeldata for the full leading/trailing period found. Gapfill not possible"
                 )
                 gap.gapfill_errormessage[obstype] = 'gapfill not possible: not enough modeldata'
 
                 default_return = pd.Series(
                     index=gap.exp_gap_idx, name=obstype, dtype="object"
                 )
@@ -580,23 +628,27 @@
 
 
 
 
 
 def apply_interpolate_gaps(gapslist, obsdf, outliersdf, dataset_res, gapfill_settings,
                            obstype="temp", method="time", max_consec_fill=100,
+                           overwrite_fill=False,
                            ):
 
     """ No return, only update the gaps instances attributes"""
 
     for gap in gapslist:
+        if (not overwrite_fill) & (not gap.gapfill_df.empty):
+            logger.warning(f'Gap {gap.name} is already filled with {gap.gapfill_technique} and will not be overwirtten. Set overwrite_fill to True to overwrite.')
+            continue
         gapfill_series = interpolate_gap(
                         gap=gap,
-                        obsdf=obsdf.xs(gap.name, level='name', drop_level=False),
-                        outliersdf=outliersdf.xs(gap.name, level='name', drop_level=False),
+                        obsdf=xs_save(obsdf, gap.name, level='name', drop_level=False),
+                        outliersdf=xs_save(outliersdf, gap.name, level='name', drop_level=False),
                         dataset_res=dataset_res.loc[gap.name],
                         obstype=obstype,
                         method=method,
                         max_consec_fill=max_consec_fill,
                         )
 
         gapfill_series.name = obstype
@@ -605,23 +657,33 @@
 
         # update the gaps attributes
         gap.gapfill_df = gapfill_df
         gap.gapfill_technique = gapfill_settings["label"]["linear"]
 
 
 def make_gapfill_df(gapslist):
+    if not bool(gapslist):
+        # no gaps (will be in automatic gapfill if method is not triggerd)
+        return pd.DataFrame()
     concatlist = []
     for gap in gapslist:
         subgapfill = gap.gapfill_df.reset_index()
         subgapfill['name'] = gap.name
         subgapfill = subgapfill.set_index(['name', 'datetime'])
 
         concatlist.append(subgapfill)
 
-    return pd.concat(concatlist).sort_index()
+    filldf = pd.concat(concatlist).sort_index()
+
+    # When gapfill could (paritally) not been fulfilled,
+    # their values (=Nan) must be removed from gapfill,
+    # so they will be plotted as gaps
+    filldf = filldf.dropna()
+
+    return filldf
 
 
 def missing_timestamp_and_gap_check(df, gapsize_n):
     # TODO update docstring
     """
 
     V3
@@ -656,15 +718,15 @@
     station_freqs = {}
 
     # missing timestamp per station (because some stations can have other frequencies!)
 
     stationnames = df.index.get_level_values(level="name").unique()
     for station in stationnames:
         # find missing timestamps
-        timestamps = df.xs(station, level="name").index
+        timestamps = xs_save(df, station, level="name").index
         likely_freq = get_likely_frequency(timestamps, method="highest", simplify=False)
 
 
         assert likely_freq.seconds > 0, f"The frequency is not positive!"
 
         station_freqs[station] = likely_freq
```

### Comparing `metobs_toolkit-0.1.1a0/metobs_toolkit/gap_filling.py` & `metobs_toolkit-0.1.1a2/metobs_toolkit/gap_filling.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,24 +4,23 @@
 Created on Tue Feb 28 17:05:26 2023
 
 @author: thoverga
 """
 import numpy as np
 import pandas as pd
 from datetime import timedelta
+import logging
 
 from metobs_toolkit.df_helpers import (
     remove_outliers_from_obs,
     init_multiindexdf,
     format_outliersdf_to_doubleidx,
 )
 
-# def interpolate_missing_obs(missing_ob, obsdf, outliersdf, obstype, method):
-#     # 1 get trailing and leading obs
-
+logger = logging.getLogger(__name__)
 
 
 # =============================================================================
 # Gap fillers
 # =============================================================================
 
 
@@ -37,89 +36,47 @@
     # initiate return value when no interpolation can be performed
     empty_interp = pd.Series(data=np.nan, index=gap.exp_gap_idx.droplevel("name"))
     empty_interp.name = obstype
 
     # 2 check if there is a trailing and leading gap
     if gap.startgap == gap.leading_timestamp:
         message =f"No leading timestamp found for gap {gap}"
-        print(message)
+        logger.info(message)
         gap.gapfill_errormessage[obstype]=message
         return empty_interp
 
     if gap.endgap == gap.trailing_timestamp:
         message = f"No trailing timestamp found for gap {gap}"
-        print(message)
+        logger.info(message)
         gap.gapfill_errormessage[obstype]=message
         return empty_interp
 
 
     # 3. Get leading and trailing val
     if not bool(gap.leading_val):
         # empty dict --> no value in the obs
         message =f"No cadidate for leading {obstype} observation found for {gap}"
-        print(message)
+        logger.info(message)
         gap.gapfill_errormessage[obstype]=message
         return empty_interp
 
     if not bool(gap.trailing_val):
         # empty dict --> no value in the obs
         message =f"No cadidate for trailing {obstype} observation found for {gap}"
-        print(message)
+        logger.info(message)
         gap.gapfill_errormessage[obstype]=message
         return empty_interp
 
 
     leading_dt = gap.leading_timestamp
     leading_val = gap.leading_val[obstype]
     trailing_dt = gap.trailing_timestamp
     trailing_val = gap.trailing_val[obstype]
 
 
-    # # 3 check both leading and trailing are in obs, and look for alternative leading/trailing if the original is an outlier.
-    # sta_obs = obsdf.xs(gap.name, level="name")
-
-    # # leading
-    # if gap.leading_timestamp in sta_obs.index:
-    #     # leading found in obs
-    #     leading_dt = gap.leading_timestamp
-    #     leading_val = sta_obs.loc[gap.leading_timestamp, obstype]
-    # else:
-    #     # look for last observation before leading timestamp
-    #     delta_dt = (
-    #         gap.leading_timestamp - sta_obs.index[sta_obs.index < gap.leading_timestamp]
-    #     )
-    #     if delta_dt.empty:
-    #         print(
-    #             f"No cadidate for leading {obstype} observation found for {gap.name} with gap: {gap.startgap} --> {gap.endgap}"
-    #         )
-    #         return empty_interp
-
-    #     leading_dt = gap.leading_timestamp - delta_dt.min()
-    #     leading_val = sta_obs.loc[leading_dt, obstype]
-
-    # # trailing
-    # if gap.trailing_timestamp in sta_obs.index:
-    #     # leading found in obs
-    #     trailing_dt = gap.trailing_timestamp
-    #     trailing_val = sta_obs.loc[gap.trailing_timestamp, obstype]
-    # else:
-    #     # look for last observation before leading timestamp
-    #     delta_dt = (
-    #         sta_obs.index[sta_obs.index > gap.trailing_timestamp]
-    #         - gap.trailing_timestamp
-    #     )
-    #     if delta_dt.empty:
-    #         print(
-    #             f"No cadidate for trailing {obstype} observation found for {gap.name} with gap: {gap.startgap} --> {gap.endgap}"
-    #         )
-    #         return empty_interp
-    #     # TODO: settings restrictions on maximum delta_dt ??
-    #     trailing_dt = gap.trailing_timestamp + delta_dt.min()
-    #     trailing_val = sta_obs.loc[trailing_dt, obstype]
-
     # Make interpolation series
     gaps_series = pd.Series(data=np.nan, index=gap.exp_gap_idx.droplevel("name"))
     gaps_series = pd.concat(
         [
             gaps_series,
             pd.Series(
                 index=[leading_dt, trailing_dt], data=[leading_val, trailing_val]
@@ -136,17 +93,30 @@
         inplace=True,
     )
 
     # Subset only gap indixes
     gaps_fill_series = gaps_series[gap.exp_gap_idx.droplevel("name")]
     gaps_fill_series.name = obstype
 
-    # update gapfill info
-    gap.gapfill_info = gaps_series.to_frame()
+    # update gapfill info (for the user)
+    gapfill_df = gaps_series.to_frame()
+    gapfill_df = gapfill_df.reset_index()
+    gapfill_df = gapfill_df.rename(columns={0: obstype,
+                                            'index': 'datetime'})
+    gapfill_df = gapfill_df.set_index('datetime')
+
+    gapfill_df['label'] = 'interpolation'
+    gapfill_df.loc[leading_dt, 'label'] = 'leading observation'
+    gapfill_df.loc[trailing_dt, 'label'] = 'trailing observation'
+    gapfill_df['name'] = gap.name
 
+    gapfill_df = gapfill_df.reset_index()
+    gapfill_df = gapfill_df.set_index(['name', 'datetime'])
+
+    gap.gapfill_info = gapfill_df
 
     return gaps_fill_series
 
 
 # =============================================================================
 # Debiasing period
 # =============================================================================
@@ -190,153 +160,153 @@
     # only datetimes are relevant
     obs = obs.reset_index()
     obs = obs[["name", "datetime", obstype]]
 
     # Select all leading and all trailing obs
     leading_period = obs[obs["datetime"] < gap.startgap]
     trailing_period = obs[obs["datetime"] > gap.endgap]
-    print(f'   {leading_period.shape[0]} leading records, {trailing_period.shape[0]} trailing records.')
+    logger.debug(f'   {leading_period.shape[0]} leading records, {trailing_period.shape[0]} trailing records.')
 
     # some derived integers
     poss_shrinkage_leading = leading_period.shape[0] - debias_min_sample_size_leading
     poss_shrinkage_trailing = trailing_period.shape[0] - debias_min_sample_size_trailing
     poss_extention_leading = leading_period.shape[0] - debias_pref_sample_size_leading
     poss_extention_trailing = (
         trailing_period.shape[0] - debias_pref_sample_size_trailing
     )
 
     # check if desired sample sizes for leading and trailing are possible
     if (leading_period.shape[0] >= debias_pref_sample_size_leading) & (
         trailing_period.shape[0] >= debias_pref_sample_size_trailing
     ):
-        print(f"leading and trailing periods are both available for debiassing.")
+        logger.debug(f"leading and trailing periods are both available for debiassing.")
         # both periods are oke
         leading_df = leading_period[-debias_pref_sample_size_leading:]
         trailing_df = trailing_period[:debias_pref_sample_size_trailing]
 
     elif (leading_period.shape[0] <= debias_pref_sample_size_leading) & (
         trailing_period.shape[0] >= debias_pref_sample_size_trailing
     ):
-        print(
+        logger.debug(
             f"leading periods for debiassing does not have a preferable size. Try translation/shrinkage ..."
         )
 
         # leading period to small, trailing period is OK
 
         missing_records = debias_pref_sample_size_leading - leading_period.shape[0]
 
         # 1 if the leading period is smaller thatn the minimum leading size --> return default
         if poss_shrinkage_leading < 0:
             leading_df = init_multiindexdf()
             trailing_df = init_multiindexdf()  # this might be to strict
-            print(
+            logger.debug(
                 "The available leading debias samplesize is smaller than the minimum. A translation/shrinking is not possible."
             )
 
         # 2 Try translation without shrinkage
 
         elif missing_records <= poss_extention_trailing:
             # translation without shrinkage is possible
             translation_trailing = missing_records
 
             leading_df = leading_period
             trailing_df = trailing_period[
                 0 : (debias_pref_sample_size_trailing + translation_trailing)
             ]
 
-            print(
+            logger.debug(
                 f"A translation of {translation_trailing} records is done towards the trailing period. (n_leading + n_trailing is conserved: {leading_df.shape[0] + trailing_df.shape[0]}"
             )
 
         # 3. Try if a translation is within the limits of shrinkage
         elif (missing_records - poss_extention_trailing) <= poss_shrinkage_leading:
             translation_trailing = poss_extention_trailing
 
             leading_df = leading_period
             trailing_df = trailing_period[
                 0 : debias_pref_sample_size_trailing + translation_trailing
             ]
-            print(
+            logger.debug(
                 f"A translation of {translation_trailing} records is done towards the trailing period. Since there was not engough translation space for the trailing obs, the condition n_leading + n_trailing is NOT conserved: {leading_df.shape[0] + trailing_df.shape[0]}. \
                   Both leading and trailing sizes still achieves minimal size restrictions."
             )
         # 4. If all else fails, it is not possible to make a leading period
         else:
-            print(
+            logger.info(
                 "The available leading samplesize can not reach minimal size restrictions."
             )
             # no translation is possible, even with shrinking
             leading_df = init_multiindexdf()
             trailing_df = init_multiindexdf()  # this might be to strict
 
     elif (leading_period.shape[0] >= debias_pref_sample_size_leading) & (
         trailing_period.shape[0] <= debias_pref_sample_size_trailing
     ):
         # leading period is ok, trailing period is to short
-        print(
+        logger.debug(
             f"trailing periods for debiassing does not have a preferable size. Try translation/shrinkage ..."
         )
         missing_records = debias_pref_sample_size_trailing - trailing_period.shape[0]
 
         # 1 if the trailing period is smaller thatn the minimum trailing size --> return default
         if poss_shrinkage_trailing < 0:
             leading_df = init_multiindexdf()  # might be to strict
             trailing_df = init_multiindexdf()
-            print(
+            logger.debug(
                 "The available trailing debias samplesize is smaller than the minimum. A translation/shrinking is not possible."
             )
             # return
 
         # 2 Try translation without shrinkage
         elif missing_records <= poss_extention_leading:
             # translation without shrinkage is possible
             translation_leading = missing_records
 
             leading_df = leading_period[
                 -(debias_pref_sample_size_leading + translation_leading) :
             ]
             trailing_df = trailing_period
-            print(
+            logger.debug(
                 f"A translation of {translation_leading} records is done towards the leading period. (n_leading + n_trailing is conserved: {leading_df.shape[0] + trailing_df.shape[0]}"
             )
 
         # 3. Try if a translation is within the limits of shrinkage
         elif (missing_records - poss_extention_leading) <= poss_shrinkage_trailing:
             translation_leading = poss_extention_leading
 
             leading_df = leading_period[
                 -(debias_pref_sample_size_leading + translation_leading)
             ]
             trailing_df = trailing_period
-            print(
+            logger.debug(
                 f"A translation of {translation_leading} records is done towards the leading period. Since there was not engough translation space for the leading obs, the condition n_leading + n_trailing is NOT conserved: {leading_df.shape[0] + trailing_df.shape[0]}. \
                   Both leading and trailing sizes still achieves minimal size restrictions."
             )
         # 4. If all else fails, it is not possible to make a trailing period
         else:
             # no translation is possible, even with shrinking
-            print(
+            logger.info(
                 "The available trailing samplesize can not reach minimal size restrictions."
             )
             leading_df = init_multiindexdf()  # this might be to strict
             trailing_df = init_multiindexdf()
 
     else:
         # Both leading and trailing periods are not to small
 
         # 1 does both (leading and trailing) still acchieves the minimal size condition for shrinking?
         if (poss_shrinkage_leading >= 0) & (poss_shrinkage_trailing >= 0):
-            print(
+            logger.debug(
                 "Both leading and trailing periods do not have a prefered size, but still meet the minimal conditions."
             )
             leading_df = leading_period
             trailing_df = trailing_period
 
         else:
-            print(
+            logger.info(
                 "Both leading and trailing periods do not have a prefered size, and eighter of them does NOT meet minimal condition."
             )
             # either one of the periods does not reach minimal condition, so return default
             leading_df = init_multiindexdf()
             trailing_df = init_multiindexdf()
 
     # convert to multiindex
@@ -406,27 +376,35 @@
     gap_model = gap_model.set_index(['name', 'datetime'])
 
     # Idea: if BOTH leadin and trailing (hourly) biases is available, than use
     # use the debias corection (even if it is for a part of the gap!).
     # If either one or both are missing, than no bias correction is applied
     no_debias = gap_model[(gap_model[obstype + '_bias_lead'].isnull()) |
                           (gap_model[obstype + '_bias_trail'].isnull())].index
-    error_message =f'WARNING!, No debias possible for these gap records: {no_debias},the gap will be filled by model data without bias correction. '
-    print(error_message)
+    if not no_debias.empty:
+        error_message =f'No debias possible for these gap records: {no_debias},the gap will be filled by model data without bias correction. '
+        logger.warning(error_message)
 
 
     # set weights to zero if not debias correction can be applied on that record
     gap_model.loc[no_debias, obstype+'_bias_trail'] = 0.
     gap_model.loc[no_debias, obstype+'_bias_lead'] = 0.
 
 
     # 5. compute the debiased fill value
     # leave this dataframe for debugging
-    gap_model[obstype + "_fill"] = gap_model[obstype] - (
+    gap_model[obstype + "_debiased_value"] = gap_model[obstype] - (
         (gap_model["lead_weight"] * gap_model[obstype + "_bias_lead"])
         + (gap_model["trail_weight"] * gap_model[obstype + "_bias_trail"])
     )
 
+    # 7. format gapmodel
+    gap_model['time'] = (gap_model['hours'].astype(str).str.zfill(2) + ':' +
+                         gap_model['minutes'].astype(str).str.zfill(2) + ':' +
+                         gap_model['seconds'].astype(str).str.zfill(2))
+    gap_model = gap_model.rename(columns={obstype: f'{obstype}_model_value'})
+
+
     # 6. make returen
-    returnseries = gap_model[obstype + "_fill"]
+    returnseries = gap_model[obstype + "_debiased_value"]
     returnseries.name = obstype
     return returnseries, gap_model, error_message
```

### Comparing `metobs_toolkit-0.1.1a0/metobs_toolkit/landcover_functions.py` & `metobs_toolkit-0.1.1a2/metobs_toolkit/landcover_functions.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,21 +4,24 @@
 Created on Wed Oct 19 11:28:36 2022
 
 @author: thoverga
 """
 
 
 import sys
+import logging
 from time import sleep
 import pytz
 import pandas as pd
 import ee
 
 from metobs_toolkit.df_helpers import init_multiindexdf
 
+logger = logging.getLogger(__name__)
+
 # =============================================================================
 #  Connection functions
 # =============================================================================
 
 
 def connect_to_gee():
     if not ee.data._credentials:  # check if ee connection is initialized
@@ -35,43 +38,45 @@
 def lcz_extractor(metadf, mapinfo):
     # make return in case something went wrong
     default_return = pd.Series(
         index=metadf.index, data="Location_unknown", name="lcz", dtype=object
     )
     # test if metadata is suitable
     if not _validate_metadf(metadf):
-        print(f"Metadf is not suitable for GEE extractiond: {metadf}")
+        logger.warning(f"Metadf is not suitable for GEE extractiond: {metadf}")
         return default_return
 
     relevant_metadf = metadf.reset_index()[["name", "lat", "lon"]]
 
     lcz_df = extract_pointvalues(
         metadf=relevant_metadf, mapinfo=mapinfo, output_column_name="lcz"
     )
+    if lcz_df.empty:
+        return pd.Series(dtype=object)
     return lcz_df["lcz"]  # return series
 
 
 def lc_fractions_extractor(metadf, mapinfo, buffer, agg):
     # make return in case something went wrong
     default_return = (pd.DataFrame(index=metadf.index), buffer)
 
     # test if metadata is suitable
     if not _validate_metadf(metadf):
-        print(f"Metadf is not suitable for GEE extractiond: {metadf}")
+        logger.warning(f"Metadf is not suitable for GEE extractiond: {metadf}")
         return default_return
 
     relevant_metadf = metadf.reset_index()[["name", "lat", "lon"]]
 
     freqs_df = extract_buffer_frequencies(
         metadf=relevant_metadf, mapinfo=mapinfo, bufferradius=buffer
     )
 
     # apply aggregation if required
     if agg:
-        print(f"Using aggregation scheme: {mapinfo['aggregation']}")
+        logger.info(f"Using aggregation scheme: {mapinfo['aggregation']}")
         agg_df = pd.DataFrame()
         for agg_name, agg_classes in mapinfo["aggregation"].items():
             present_agg_classes = [
                 str(num) for num in agg_classes if str(num) in freqs_df.columns
             ]
             agg_df[agg_name] = freqs_df[present_agg_classes].sum(axis=1)
 
@@ -89,15 +94,15 @@
     # make return in case something went wrong
     default_return = pd.Series(
         index=metadf.index, data="Location_unknown", name="altitude", dtype=object
     )
 
     # test if metadata is suitable
     if not _validate_metadf(metadf):
-        print(f"Metadf is not suitable for GEE extractiond: {metadf}")
+        logger.warning(f"Metadf is not suitable for GEE extractiond: {metadf}")
         return default_return
 
     relevant_metadf = metadf.reset_index()[["name", "lat", "lon"]]
 
     altitude_df = extract_pointvalues(
         metadf=relevant_metadf, mapinfo=mapinfo, output_column_name="altitude"
     )
@@ -108,18 +113,17 @@
 # Object convertors
 # =============================================================================
 
 
 def _datetime_to_gee_datetime(datetime):
     # covert to UTC!
     utcdt = datetime.astimezone(pytz.utc)
-    print(utcdt.replace(tzinfo=None))
+    logger.debug(utcdt.replace(tzinfo=None))
     return ee.Date(utcdt.replace(tzinfo=None))
-    # print(f'formaat:   {utcdt.strftime("%Y-%m-%dT%H:%M:%S")}')
-    # return ee.Date(utcdt.strftime("%Y-%m-%dT%H:%M:%S"))
+
 
 
 def get_ee_obj(mapinfo, band=None):
     if mapinfo["is_image"]:
         obj = ee.Image(mapinfo["location"])
     elif mapinfo["is_imagecollection"]:
         if isinstance(band, type(None)):
@@ -150,15 +154,16 @@
 
     :param metadf: metadata dataframe
     :type metadf: pd.DataFrame
     :return: True if oke, else False
     :rtype: Bool
 
     """
-
+    if metadf.empty:
+        return False
     if metadf["geometry"].x.isnull().values.all():
         return False
     if metadf["geometry"].y.isnull().values.all():
         return False
     try:
         # Just testing if it can be converted
         metadf = metadf.to_crs("epsg:4326")
@@ -205,18 +210,18 @@
         features.append(poi_feature)
 
     return ee.FeatureCollection(features)
 
 
 def coordinates_available(metadf, latcol="lat", loncol="lon"):
     if metadf[latcol].isnull().all():
-        print("No coordinates are found!")
+        logger.warning("No coordinates are found!")
         return False
     if metadf[loncol].isnull().all():
-        print("No coordinates are found!")
+        logger.warning("No coordinates are found!")
         return False
     return True
 
 
 def _estimate_data_size(metadf, startdt, enddt, mapinfo):
     datatimerange = pd.date_range(start=startdt, end=enddt, freq=mapinfo["time_res"])
 
@@ -290,19 +295,27 @@
             collection=ee_fc, scale=scale  # feature collection here
         ).getInfo()
     else:
         sys.exit(
             f'gee dataset {mapinfo["location"]} is neighter image nor imagecollection.'
         )
 
+
+    # extract properties
+    if not bool(results['features']):
+        # no data retrieved
+        logger.warning(f'Something went wrong, gee did not return any data: {results}')
+        logger.info(f'(Could it be that (one) these coordinates are not on the map: {metadf}?)')
+        return pd.DataFrame()
     # =============================================================================
     # to dataframe
     # =============================================================================
 
-    # extract properties
+
+
     properties = [x["properties"] for x in results["features"]]
     df = pd.DataFrame(properties)
 
     # map to human space if categorical
     if mapinfo["value_type"] == "categorical":
         df[mapinfo["band_of_use"]] = df[mapinfo["band_of_use"]].map(
             mapinfo["categorical_mapper"]
@@ -348,16 +361,16 @@
 
     # test if coordiantes are available
     if not coordinates_available(metadf, "lat", "lon"):
         return pd.DataFrame()
 
     # test if map is categorical
     if not mapinfo["value_type"] == "categorical":
-        print(
-            "ERROR: Extract buffer frequencies is only implemented for categorical datasets!"
+        logger.warning(
+            "Extract buffer frequencies is only implemented for categorical datasets!"
         )
         return pd.DataFrame()
 
     # =============================================================================
     # df to featurecollection
     # =============================================================================
 
@@ -442,14 +455,18 @@
 
     use_drive = False
     _est_data_size = _estimate_data_size(metadf, startdt, enddt, mapinfo)
     if _est_data_size > 4000:
         print(
             "THE DATA AMOUT IS TO LAREGE FOR INTERACTIVE SESSION, THE DATA WILL BE EXPORTED TO YOUR GOOGLE DRIVE!"
         )
+        logger.info(
+            "THE DATA AMOUT IS TO LAREGE FOR INTERACTIVE SESSION, THE DATA WILL BE EXPORTED TO YOUR GOOGLE DRIVE!"
+        )
+
         use_drive = True
     # =============================================================================
     # df to featurecollection
     # =============================================================================
 
     ee_fc = _df_to_features_point_collection(metadf)
 
@@ -460,16 +477,15 @@
     def rasterExtraction(image):
         feature = image.sampleRegions(
             collection=ee_fc,  # feature collection here
             scale=scale,  # Cell size of raster
         )
         return feature
 
-    print(f'startdtfilter: { _datetime_to_gee_datetime(startdt).getInfo()}')
-    print(f'enddtfilter: { _datetime_to_gee_datetime(enddt).getInfo()}')
+
     raster = get_ee_obj(mapinfo, bandname)  # dataset
     results = (
         raster.filter(
             ee.Filter.date(
                 _datetime_to_gee_datetime(startdt), _datetime_to_gee_datetime(enddt)
             )
         )
@@ -510,37 +526,40 @@
     else:
         _filename = "era5_data"
         _drivefolder = "era5_timeseries"
 
         print(
             f"The timeseries will be writen to your Drive in {_drivefolder}/{_filename} "
         )
+        logger.info(
+            f"The timeseries will be writen to your Drive in {_drivefolder}/{_filename} "
+        )
 
         task = ee.batch.Export.table.toDrive(
             collection=results,
             description="extracting_era5",
             folder=_drivefolder,
             fileNamePrefix=_filename,
             fileFormat="CSV",
             selectors=["datetime", "name", bandname],
         )
 
         task.start()
-        print("The google server is handling your request ...")
+        logger.info("The google server is handling your request ...")
         sleep(3)
         finished = False
         while finished == False:
             if task.status()["state"] == "READY":
-                print("Awaitening execution ...")
+                logger.info("Awaitening execution ...")
                 sleep(4)
             elif task.status()["state"] == "RUNNING":
-                print("Running ...")
+                logger.info("Running ...")
                 sleep(4)
             else:
-                print("finished")
+                logger.info("finished")
                 finished = True
 
         doc_folder_id = task.status()["destination_uris"][0]
         print("The data is transfered! Open the following link in your browser: \n\n")
         print(f"{doc_folder_id} \n\n")
         print(
             "To upload the data to the model, use the Modeldata.set_model_from_csv() method"
```

### Comparing `metobs_toolkit-0.1.1a0/metobs_toolkit/missingobs.py` & `metobs_toolkit-0.1.1a2/metobs_toolkit/missingobs.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 """
-Created on Mon Mar 13 16:12:41 2023
+This module contains the Missingob_collection class and all its methods.
 
-@author: thoverga
+A Missingob_collection holds all missing observations and methods on how to
+fill them.
 """
 
 
 import pandas as pd
 import numpy as np
 from datetime import datetime, timedelta
 import logging
 
-from metobs_toolkit.df_helpers import _find_closes_occuring_date
+from metobs_toolkit.df_helpers import (
+    _find_closes_occuring_date,
+    xs_save,
+    )
 
 logger = logging.getLogger(__name__)
 
 # =============================================================================
 # Missing observation
 
 # a missing observation is a missing timestamp
@@ -26,15 +30,18 @@
 class Missingob_collection:
     """ Class object handling a set of missing observations. """
     def __init__(self, missing_obs_series):
 
         missing_obs_series.name = 'datetime'
         missing_obs_series.index.name = 'name'
 
-        missing_obs_series = missing_obs_series.drop_duplicates()
+
+        missing_obs_df = missing_obs_series.reset_index() #needed to find duplicates
+        missing_obs_df = missing_obs_df.drop_duplicates()
+        missing_obs_series = missing_obs_df.set_index('name')['datetime']
         missing_obs_series = missing_obs_series.sort_index()
 
         missing_idx = missing_obs_series.reset_index()
         missing_idx = missing_idx.set_index(['name', 'datetime'])
 
         self.series = missing_obs_series
         self.idx = missing_idx.index
@@ -42,36 +49,97 @@
         # gap fill (only for conventional saving)
         self.fill_df = pd.DataFrame()
         self.fill_technique = None
 
     def __add__(self, other):
         comb_series = pd.concat([self.series, other.series])
 
-        comb_series = comb_series.drop_duplicates()
+        # drop duplicates and sort
+        comb_df = comb_series.reset_index() #needed to find duplicates
+        comb_df = comb_df.drop_duplicates()
+        comb_series = comb_df.set_index('name')['datetime']
         comb_series = comb_series.sort_index()
 
         self.series = comb_series
         comb_idx = comb_series.reset_index()
         comb_idx = comb_idx.set_index(['name', 'datetime'])
         self.idx = comb_idx.index
         return self
-
+    def __len__(self):
+        return self.series.shape[0]
 
     def __str__(self):
         if self.series.empty:
             return f'Empty missing observations.'
+
         if not self.fill_df.empty:
             return f'Missing observations with filled ({self.fill_technique}) \
                 values: \n {self.fill_df} \n Original missing observations on import: \n {self.idx}'
 
         return f'Missing observations: \n {self.series}'
     def __repr__(self):
         return self.__str__()
 
 
+    def get_info(self, max_disp_list=7):
+        """
+        Print out detailed information on the missing observations.
+
+        Parameters
+        ----------
+
+        max_disp_list : int, optional
+            Max size of lists to print out. If listsize is larger, the length of
+            the list is printed. The default is 7.
+
+        Returns
+        -------
+        None.
+
+        """
+
+        print(f'\n -------- Missing observations info -------- \n')
+        if self.series.empty:
+            print(f'Empty missing observations.')
+            return
+        print('(Note: missing observations are defined on the frequency estimation of the native dataset.)')
+
+        n_missing = len(self)
+        stations = self.series.index.unique().to_list()
+
+        print(f'  * {n_missing} missing observations')
+        if n_missing <= max_disp_list:
+            print(f'\n {self.series} \n')
+
+        if len(stations) <= max_disp_list:
+            print(f'  * For these stations: {stations}')
+        else:
+            print(f'  * For {len(stations)} stations')
+
+        if self.fill_df.empty:
+            print(f'  * The missing observations are not filled.')
+        else:
+            filled_obstypes = [obs for obs in self.fill_df.columns if not obs.endswith('_final_label')]
+            print(f'  * Missing observations are filled with {{self.fill_technique}} for: ')
+            for obstype in filled_obstypes:
+                print(f'    {obstype}: \n {self.fill_df[[obstype]]}')
+
+            # print missing obs that could not be filled
+            print(f'  * Missing observations that could NOT be filled for: ')
+            for obstype in filled_obstypes:
+                unfilled = self.idx[~self.idx.isin(self.fill_df[[obstype]].dropna().index)]
+                print(f'    {obstype}: \n {unfilled}')
+
+
+        print('(More details on the missing observation can be found in the .series and .fill_df attributes.)')
+        return
+
+
+
+
     def get_station_missingobs(self, name):
         """
         Get the missing observations of a specific station.
 
         Parameters
         ----------
         name : str
@@ -114,14 +182,43 @@
             names=["name", "datetime"],
         )
 
         obsdf = obsdf.drop(index=missing_multiidx, errors="ignore")
 
         return obsdf
 
+    def remove_missing_from_outliers(self, outldf):
+        """
+        Drop the missing observation records from an outlier dataframe, if
+        they are present. This will ignore the observation types! So all
+        outliers of any observation type, at an missing timestamp are removed.
+
+        Parameters
+        ----------
+        obsdf : pandas.DataFrame
+            Multiindex (name-datetime-obstype) observational dataframe.
+
+        Returns
+        -------
+        obsdf : pandas.DataFrame
+            Multiindex observational dataframe without records linked to missing
+            observations.
+
+        """
+
+        # to multiindex
+        outldf = outldf.reset_index().set_index(['name', 'datetime'])
+
+        # remove records inside the gaps
+        suboutldf = self.remove_missing_from_obs(obsdf = outldf)
+
+        # reset to triple index
+        outldf = suboutldf.reset_index().set_index(['name', 'datetime', 'obstype'])
+        return outldf
+
     def interpolate_missing(self, obsdf, resolutionseries, obstype='temp', method='time'):
         """
         Fill the missing observations using an interpolation method.
 
         The "fill_df" and "fill_technique" attributes will be updated.
 
         Parameters
@@ -147,18 +244,18 @@
         missing_obsspace = self.get_missing_indx_in_obs_space(obsdf, resolutionseries)
 
         # Set index for df fill attribute
         self.fill_df = pd.DataFrame(index=missing_obsspace)
 
 
         for staname, missingdt in missing_obsspace:
-            staobs = obsdf.xs(staname, level='name')[obstype]
+            staobs = xs_save(obsdf, staname, level='name')[obstype]
             # exclude nan values because they are no good leading/trailing
             staobs = staobs[~staobs.isnull()]
-            print(f'staname: {staname}, missingdt: {missingdt}')
+
             # find leading and trailing datetimes
             leading_seconds =_find_closes_occuring_date(refdt = missingdt,
                                                         series_of_dt = staobs.index,
                                                         where='before')
             if np.isnan(leading_seconds):
                 logger.warn(f'missing obs: {staname}, at {missingdt} does not have a leading timestamp.')
                 continue
@@ -187,15 +284,17 @@
             # interpolate the missing obs
             stadf['interp'] = stadf[obstype].interpolate(
                                                 method=method,
                 )
 
             self.fill_df.loc[(staname, missingdt), obstype] = stadf.loc[missingdt, 'interp']
 
-
+        # if no fill is applied (no leading/trailing), remove them from fill to keep them as missing
+        if not self.fill_df.empty:
+            self.fill_df = self.fill_df.dropna(subset=obstype)
 
 
     def get_missing_indx_in_obs_space(self, obsdf, resolutionseries):
         """
         Function to found which missing timestamps are expected in the observation space.
         Because of time coarsening not all missing timestamps are expected in observation space.
 
@@ -225,16 +324,16 @@
         for sta in self.series.index.unique():
             # Get missing observations in IO space
             sta_missing = self.series.loc[sta]
             if not isinstance(sta_missing, type(pd.Series(dtype=object))):
                 sta_missing = pd.Series(data=[sta_missing], index=[sta], dtype=object)
 
             # Get start, end and frequency of the observation in obs space
-            startdt = obsdf.xs(sta, level="name").index.min()
-            enddt = obsdf.xs(sta, level="name").index.max()
+            startdt = xs_save(obsdf, sta, level="name").index.min()
+            enddt = xs_save(obsdf, sta, level="name").index.max()
             obs_freq = resolutionseries.loc[sta]
 
             # Make datetimerange
             obsrange = pd.date_range(
                 start=startdt, end=enddt, freq=obs_freq, inclusive="both"
             )
```

### Comparing `metobs_toolkit-0.1.1a0/metobs_toolkit/qc_checks.py` & `metobs_toolkit-0.1.1a2/metobs_toolkit/qc_checks.py`

 * *Files 25% similar despite different names*

```diff
@@ -6,20 +6,22 @@
 @author: thoverga
 """
 
 import sys
 import pandas as pd
 import numpy as np
 import logging
+import titanlib
 
 
 from metobs_toolkit.df_helpers import (
     init_multiindex,
     init_multiindexdf,
     init_triple_multiindexdf,
+    xs_save
 )
 
 
 logger = logging.getLogger(__name__)
 
 
 # =============================================================================
@@ -125,15 +127,15 @@
         # get stations that have ouliers for this obstype
         outl_stations = groups.loc[groups[obstype], obstype].index.to_list()
 
         outl_multiidx = init_multiindex()
         for sta in outl_stations:
             # apply check per station
             outl_idx = (
-                df.xs(sta, level="name", drop_level=False)[obstype]
+                xs_save(df, sta, level="name", drop_level=False)[obstype]
                 .isnull()
                 .loc[lambda x: x]
                 .index
             )
             outl_multiidx = outl_multiidx.append(outl_idx)
 
         outl_dict[obstype] = outl_multiidx
@@ -173,15 +175,15 @@
 
     duplicates = pd.Series(
         data=df.index.duplicated(keep=checks_settings[checkname]["keep"]),
         index=df.index,
     )
 
     if not df.loc[duplicates].empty:
-        logging.warning(
+        logger.warning(
             f" Following records are labeld as duplicates: {df.loc[duplicates]}, and are removed"
         )
 
     # Fill the outlierdf with the duplicates
     outliers = df[df.index.duplicated(keep=checks_settings[checkname]["keep"])]
 
     # convert values to nan in obsdf
@@ -247,15 +249,14 @@
     """
 
     checkname = "gross_value"
 
     try:
         specific_settings = checks_settings[checkname][obstype]
     except:
-        print(f"No {checkname} settings found for obstype={obstype}. Check is skipped!")
         logger.warning(
             f"No {checkname} settings found for obstype={obstype}. Check is skipped!"
         )
         return obsdf, init_multiindexdf()
 
     # drop outliers from the series (these are Nan's)
     input_series = obsdf[obstype].dropna()
@@ -307,32 +308,28 @@
     """
 
     checkname = "persistance"
 
     try:
         specific_settings = checks_settings[checkname][obstype]
     except:
-        print(f"No {checkname} settings found for obstype={obstype}. Check is skipped!")
         logger.warning(
             f"No {checkname} settings found for obstype={obstype}. Check is skipped!"
         )
         return obsdf, init_multiindexdf()
 
     invalid_windows_check_df = (
         pd.to_timedelta(specific_settings["time_window_to_check"]) / station_frequencies
         < specific_settings["min_num_obs"]
     )
     invalid_stations = list(
         invalid_windows_check_df[invalid_windows_check_df == True].index
     )
     if bool(invalid_stations):
-        print(
-            f"The windows are too small for stations  {invalid_stations} to perform persistance check"
-        )
-        logger.info(
+        logger.warning(
             f"The windows are too small for stations  {invalid_stations} to perform persistance check"
         )
 
     subset_not_used = obsdf[obsdf.index.get_level_values("name").isin(invalid_stations)]
     subset_used = obsdf[~obsdf.index.get_level_values("name").isin(invalid_stations)]
 
     if not subset_used.empty:
@@ -418,15 +415,14 @@
     """
 
     checkname = "repetitions"
 
     try:
         specific_settings = checks_settings[checkname][obstype]
     except:
-        print(f"No {checkname} settings found for obstype={obstype}. Check is skipped!")
         logger.warning(
             f"No {checkname} settings found for obstype={obstype}. Check is skipped!"
         )
         return obsdf, init_multiindexdf()
 
     # drop outliers from the series (these are Nan's)
     input_series = obsdf[obstype].dropna()
@@ -495,27 +491,26 @@
     """
 
     checkname = "step"
 
     try:
         specific_settings = checks_settings[checkname][obstype]
     except:
-        print(f"No {checkname} settings found for obstype={obstype}. Check is skipped!")
         logger.warning(
             f"No {checkname} settings found for obstype={obstype}. Check is skipped!"
         )
         return obsdf, init_multiindexdf()
 
     # drop outliers from the series (these are Nan's)
     input_series = obsdf[obstype].dropna()
 
     list_of_outliers = []
 
     for name in input_series.index.droplevel("datetime").unique():
-        subdata = input_series.xs(name, level="name", drop_level=False)
+        subdata = xs_save(input_series, name, level="name", drop_level=False)
 
         time_diff = subdata.index.get_level_values("datetime").to_series().diff()
         time_diff.index = subdata.index  # back to multiindex
         # define filter
         step_filter = (
             (subdata - subdata.shift(1))
             > (
@@ -583,32 +578,28 @@
 
     """
     checkname = "window_variation"
 
     try:
         specific_settings = checks_settings[checkname][obstype]
     except:
-        print(f"No {checkname} settings found for obstype={obstype}. Check is skipped!")
         logger.warning(
             f"No {checkname} settings found for obstype={obstype}. Check is skipped!"
         )
         return obsdf, init_multiindexdf()
 
     invalid_windows_check_df = (
         pd.to_timedelta(specific_settings["time_window_to_check"]) / station_frequencies
         < specific_settings["min_window_members"]
     )
     invalid_stations = list(
         invalid_windows_check_df[invalid_windows_check_df == True].index
     )
     if bool(invalid_stations):
-        print(
-            f"The windows are too small for stations  {invalid_stations} to perform window variation check"
-        )
-        logger.info(
+        logger.warning(
             f"The windows are too small for stations  {invalid_stations} to perform window variation check"
         )
 
     subset_not_used = obsdf[obsdf.index.get_level_values("name").isin(invalid_stations)]
     subset_used = obsdf[~obsdf.index.get_level_values("name").isin(invalid_stations)]
 
     if not subset_used.empty:
@@ -698,7 +689,231 @@
         names=["name", "datetime"],
     )
     outlier_sub_df = pd.DataFrame(data=None, index=multi_idx, columns=None)
 
     intersection = outlier_sub_df.index.intersection(input_data.dropna().index).values
 
     return intersection
+
+
+# =============================================================================
+# Titan checks
+# =============================================================================
+
+def create_titanlib_points_dict(obsdf, metadf, obstype):
+    obs = obsdf[[obstype]]
+    obs = obs.reset_index()
+
+    # merge metadata
+    obs = obs.merge(right = metadf[['lat', 'lon','altitude']],
+                    how = 'left',
+                    left_on='name',
+                    right_index=True)
+
+    dt_grouper = obs.groupby('datetime')
+
+
+    points_dict = {}
+    for dt, group in dt_grouper:
+
+        check_group = group[~group[obstype].isnull()]
+
+        points_dict[dt] = {
+            'values': check_group[obstype].to_numpy(),
+            'names': check_group['name'].to_numpy(),
+            'lats': check_group['lat'].to_numpy(),
+            'lons': check_group['lon'].to_numpy(),
+            'elev': check_group['altitude'].to_numpy(),
+            'ignore_names': group[group[obstype].isnull()]['name'].to_numpy()
+        }
+
+    return points_dict
+
+def titan_buddy_check(obsdf, metadf, obstype, checks_info, checks_settings, titan_specific_labeler):
+
+    """
+    The buddy check compares an observation against its neighbours (i.e. buddies). The check looks for
+    buddies in a neighbourhood specified by a certain radius. The buddy check flags observations if the
+    (absolute value of the) difference between the observations and the average of the neighbours
+    normalized by the standard deviation in the circle is greater than a predefined threshold.
+
+
+    Parameters
+
+    obsdf: Pandas.DataFrame
+        The dataframe containing the observations
+
+    metadf: Pandas.DataFrame
+        The dataframe containing the metadata (e.g. latitude, longitude...)
+
+    obstype: String, optional
+        The observation type that has to be checked. The default is 'temp'
+
+    checks_info: Dictionary
+        Dictionary with the names of the outlier flags for each check
+
+    checks_settings: Dictionary
+        Dictionary with the settings for each check
+
+    titan_specific_labeler: Dictionary
+        Dictionary that maps numeric flags to 'ok' or 'outlier' flags for each titan check
+
+
+    """
+
+    try:
+        alt = metadf['altitude']
+    except:
+        logger.warning(
+            f"Cannot find altitude of weather stations. Check is skipped!"
+        )
+
+    # Create points_dict
+    pointsdict = create_titanlib_points_dict(obsdf, metadf, obstype)
+
+    df_list = []
+    for dt, point in pointsdict.items():
+        obs = list(point['values'])
+        titan_points = titanlib.Points(np.asarray(point['lats']),
+                                       np.asarray(point['lons']),
+                                       np.asarray(point['elev']))
+
+
+        num_labels = titanlib.buddy_check(
+                titan_points,
+                np.asarray(obs),
+                np.asarray([checks_settings['radius']] * len(obs)), #same radius for all stations
+                np.asarray([checks_settings['num_min']] * len(obs)), #same min neighbours for all stations
+                checks_settings['threshold'],
+                checks_settings['max_elev_diff'],
+                checks_settings['elev_gradient'],
+                checks_settings['min_std'],
+                checks_settings['num_iterations'],
+                np.full(len(obs), 1)) #check all
+
+        labels = pd.Series(num_labels, name='num_label').to_frame()
+        labels['name'] = point['names']
+        labels['datetime'] = dt
+        df_list.append(labels)
+
+    checkeddf = pd.concat(df_list)
+
+    #Convert to toolkit format
+    outliersdf = checkeddf[checkeddf['num_label'].isin(titan_specific_labeler['outl'])]
+
+    outliersdf = outliersdf.set_index(['name', 'datetime'])
+
+
+    obsdf, outliersdf = make_outlier_df_for_check(station_dt_list=outliersdf.index,
+                                                  obsdf = obsdf,
+                                                  obstype=obstype,
+                                                  flag = checks_info["titan_buddy_check"]['outlier_flag'])
+
+
+    return obsdf, outliersdf
+
+def titan_sct_resistant_check(obsdf, metadf, obstype,
+                              checks_info, checks_settings,
+                              titan_specific_labeler):
+
+    """
+    The SCT resistant check is a spatial consistency check which compares each observations to what is expected given the other observations in the
+    nearby area. If the deviation is large, the observation is removed. The SCT uses optimal interpolation
+    (OI) to compute an expected value for each observation. The background for the OI is computed from
+    a general vertical profile of observations in the area.
+
+    Parameters
+
+    obsdf: Pandas.DataFrame
+        The dataframe containing the observations
+
+    metadf: Pandas.DataFrame
+        The dataframe containing the metadata (e.g. latitude, longitude...)
+
+    obstype: String, optional
+        The observation type that has to be checked. The default is 'temp'
+
+    checks_info: Dictionary
+        Dictionary with the names of the outlier flags for each check
+
+    checks_settings: Dictionary
+        Dictionary with the settings for each check
+
+    titan_specific_labeler: Dictionary
+        Dictionary that maps numeric flags to 'ok' or 'outlier' flags for each titan check
+
+
+    """
+
+    import time
+
+    try:
+        alt = metadf['altitude']
+    except:
+        logger.warning(
+            f"Cannot find altitude of weather stations. Check is skipped!"
+        )
+
+    # Create points_dict
+    pointsdict = create_titanlib_points_dict(obsdf, metadf, obstype)
+
+    df_list = []
+    for dt, point in pointsdict.items():
+        logger.debug(f'sct on observations at {dt}')
+        obs = list(point['values'])
+        titan_points = titanlib.Points(np.asarray(point['lats']),
+                                       np.asarray(point['lons']),
+                                       np.asarray(point['elev']))
+
+
+        flags, scores = titanlib.sct_resistant(
+                points=titan_points, #points
+                values=np.asarray(obs), # vlues
+                obs_to_check=np.full(len(obs), 1), # obs to check (check all)
+                background_values=np.full(len(obs), 0), # background values
+                background_elab_type=titanlib.MedianOuterCircle, #background elab type
+                num_min_outer=checks_settings['num_min_outer'], #num min outer
+                num_max_outer=checks_settings['num_max_outer'], #num mac outer
+                inner_radius=checks_settings['inner_radius'], #inner radius
+                outer_radius=checks_settings['outer_radius'], #outer radius
+                num_iterations=checks_settings['num_iterations'], #num iterations
+                num_min_prof=checks_settings['num_min_prof'], #num min prof
+                min_elev_diff=checks_settings['min_elev_diff'], # min elev diff
+                min_horizontal_scale=checks_settings['min_horizontal_scale'], #min horizontal scale
+                max_horizontal_scale=checks_settings['max_horizontal_scale'], # max horizontal scale
+                kth_closest_obs_horizontal_scale=checks_settings['kth_closest_obs_horizontal_scale'], #kth closest obs horizontal scale
+                vertical_scale=checks_settings['vertical_scale'], #vertical scale
+                value_mina=[x - checks_settings['mina_deviation'] for x in obs], # values mina
+                value_maxa=[x + checks_settings['maxa_deviation'] for x in obs], #values maxa
+                value_minv=[x - checks_settings['minv_deviation'] for x in obs], #values minv
+                value_maxv=[x + checks_settings['maxv_deviation'] for x in obs], # values maxv
+                eps2=np.full(len(obs),checks_settings['eps2']), #eps2
+                tpos=np.full(len(obs),checks_settings['tpos']), #tpos
+                tneg=np.full(len(obs),checks_settings['tneg']), #tneg
+                debug=checks_settings['debug'], #debug
+                basic=checks_settings['basic'] #basic
+                )
+        logger.debug('Sleeping ... (to avoid segmentaton errors)')
+        time.sleep(1)
+
+        labels = pd.Series(flags, name='num_label').to_frame()
+        labels['name'] = point['names']
+        labels['datetime'] = dt
+        df_list.append(labels)
+
+    checkeddf = pd.concat(df_list)
+
+    #Convert to toolkit format
+    outliersdf = checkeddf[checkeddf['num_label'].isin(titan_specific_labeler['outl'])]
+
+    outliersdf = outliersdf.set_index(['name', 'datetime'])
+
+
+    obsdf, outliersdf = make_outlier_df_for_check(station_dt_list=outliersdf.index,
+                                                  obsdf = obsdf,
+                                                  obstype=obstype,
+                                                  flag = checks_info["titan_sct_resistant_check"]['outlier_flag'])
+
+
+    return obsdf, outliersdf
+
+
```

### Comparing `metobs_toolkit-0.1.1a0/metobs_toolkit/qc_statistics.py` & `metobs_toolkit-0.1.1a2/metobs_toolkit/qc_statistics.py`

 * *Files identical despite different names*

### Comparing `metobs_toolkit-0.1.1a0/metobs_toolkit/settings.py` & `metobs_toolkit-0.1.1a2/metobs_toolkit/settings.py`

 * *Files 15% similar despite different names*

```diff
@@ -28,29 +28,30 @@
         self.time_settings = {}
         self.app = {}
         self.qc = {}
         self.gap = {}
         self.missing_obs = {}
         self.templates = {}
         self.gee = {}
+        self.alaro = {}
         self.IO = {
             "output_folder": None,
             "input_data_file": None,
             "input_metadata_file": None,
         }
 
         # Update (instance and class variables) what can be updated by setingsfiles
         self._update_db_settings()
         self._update_time_res_settings()
         self._update_app_settings()
         self._update_qc_settings()
         self._update_gap_settings()
         self._update_templates()
         self._update_gee_settings()
-
+        self._update_alaro_settings()
     # =============================================================================
     #     Update settings from files in initialisation
     # =============================================================================
 
     def _update_db_settings(self):
         """
         Update the database settings of self using the default settings templates
@@ -154,18 +155,22 @@
     def _update_qc_settings(self):
         """
         Update quality control settings of self using the default settings templates.
         :return: No return
         :rtype: No return
         """
         logger.debug("Updating QC settings.")
-        from .settings_files.qc_settings import check_settings, checks_info
+        from .settings_files.qc_settings import (check_settings, checks_info,
+                                                 titan_check_settings,
+                                                 titan_specific_labeler)
 
         self.qc["qc_check_settings"] = check_settings
         self.qc["qc_checks_info"] = checks_info
+        self.qc['titan_check_settings'] = titan_check_settings
+        self.qc['titan_specific_labeler'] = titan_specific_labeler
 
     def _update_gap_settings(self):
         """
         Update gap defenition and fill settings of self using the default settings templates.
         :return: No return
         :rtype: No return
         """
@@ -209,14 +214,26 @@
         :rtype: No return
         """
         logger.debug("Updating gee settings.")
         from .settings_files.gee_settings import gee_datasets
 
         self.gee["gee_dataset_info"] = gee_datasets
 
+    def _update_alaro_settings(self):
+        """
+        Update the Alaro settings using the default settings templates.
+        :return: No return
+        :rtype: No return
+        """
+        logger.debug("Updating gee settings.")
+        from .settings_files.alaro_25_settings import al25_mapinfo
+        self.alaro["info"] = al25_mapinfo
+
+
+
     def update_timezone(self, timezonestr):
         """
         Change the timezone of the input data.
 
         :param timezonestr: Timezone string of the input observations.
         :type timezonestr: String
         :return: None
@@ -225,15 +242,15 @@
         if not timezonestr in all_timezones:
             print(
                 f"timezone: {timezonestr}, is not a valid timezone. Select one of the following:"
             )
             print(f"{common_timezones}")
             return
         else:
-            print(
+            logger.info(
                 f'Update timezone: {self.time_settings["timezone"]} --> {timezonestr}'
             )
             self.time_settings["timezone"] = timezonestr
 
     def update_IO(
         self,
         output_folder=None,
@@ -260,68 +277,38 @@
         :rtype: No return
 
         """
 
         logger.info("Updating settings with input: ")
 
         if not isinstance(output_folder, type(None)):
-            print(
-                "Update output_folder: ",
-                self.IO["output_folder"],
-                " --> ",
-                output_folder,
-            )
             logger.info(
                 f'Update output_folder:  {self.IO["output_folder"]}  -->  {output_folder}'
             )
             self.IO["output_folder"] = output_folder
 
         if not isinstance(input_data_file, type(None)):
-            print(
-                "Update input_data_file: ",
-                self.IO["input_data_file"],
-                " --> ",
-                input_data_file,
-            )
             logger.info(
                 f'Update input_data_file:  {self.IO["input_data_file"]}  -->  {input_data_file}'
             )
             self.IO["input_data_file"] = input_data_file
 
         if not isinstance(input_metadata_file, type(None)):
-            print(
-                "Update input_metadata_file: ",
-                self.IO["input_metadata_file"],
-                " --> ",
-                input_metadata_file,
-            )
             logger.info(
                 f'Update meta_data_file:  {self.IO["input_metadata_file"]}  -->  {input_metadata_file}'
             )
             self.IO["input_metadata_file"] = input_metadata_file
 
         if not isinstance(data_template_file, type(None)):
-            print(
-                "Update data template file: ",
-                self.templates["data_template_file"],
-                " --> ",
-                data_template_file,
-            )
             logger.info(
                 f'Update data template file:  {self.templates["data_template_file"]}  -->  {data_template_file}'
             )
             self.templates["data_template_file"] = data_template_file
 
         if not isinstance(metadata_template_file, type(None)):
-            print(
-                "Update metadata template file: ",
-                self.templates["metadata_template_file"],
-                " --> ",
-                metadata_template_file,
-            )
             logger.info(
                 f'Update metadata template file:  {self.templates["metadata_template_file"]}  -->  {metadata_template_file}'
             )
             self.templates["metadata_template_file"] = metadata_template_file
 
     def copy_template_csv_files(self, target_folder):
         """
@@ -339,15 +326,15 @@
         # test if target_folder is a folder
         assert os.path.isdir(target_folder), f"{target_folder} is not a folder"
 
         target_file = os.path.join(target_folder, "default_template.csv")
 
         shutil.copy2(default_template_file, target_file)
 
-        print("Templates copied to : ", target_file)
+        logger.info("Templates copied to : ", target_file)
 
     # =============================================================================
     #     Check settings
     # =============================================================================
 
     def show(self):
         """
@@ -366,25 +353,26 @@
         attr_list = [
             "IO",
             "db",
             "time_settings",
             "app",
             "qc",
             "gap",
+            "missing_obs",
             "templates",
             "gee",
         ]
 
         # Drop variables starting with _
         class_vars_name = [mem for mem in class_vars_name if not mem.startswith("_")]
         print("All settings:")
         print(" \n ---------------------------------------\n")
 
         for theme in attr_list:
-            print(f" ---------------- {theme} ----------------------\n")
+            print(f" ---------------- {theme} (settings) ----------------------\n")
             printdict = getattr(self, theme)
             for key1, item1 in printdict.items():
                 print(f"* {key1}: \n")
                 if isinstance(item1, type({})):
                     # nested dict level 1
                     for key2, item2 in item1.items():
                         print(f"  - {key2}: \n")
```

### Comparing `metobs_toolkit-0.1.1a0/metobs_toolkit/settings_files/gaps_and_missing_settings.py` & `metobs_toolkit-0.1.1a2/metobs_toolkit/settings_files/gaps_and_missing_settings.py`

 * *Files identical despite different names*

### Comparing `metobs_toolkit-0.1.1a0/metobs_toolkit/settings_files/gee_settings.py` & `metobs_toolkit-0.1.1a2/metobs_toolkit/settings_files/gee_settings.py`

 * *Files 14% similar despite different names*

```diff
@@ -85,10 +85,24 @@
             100: "Moss and lichen",
         },
         "aggregation": {
             "water": [70, 80, 90, 95],
             "pervious": [10, 20, 30, 40, 60, 100],
             "impervious": [50],
         },
+        'colorscheme': {
+            10:	'006400',
+            20:	'ffbb22',
+            30:	'ffff4c',
+            40:	'f096ff',
+            50:	'fa0000',
+            60:	'b4b4b4',
+            70:	'f0f0f0',
+            80:	'0064c8',
+            90:	'0096a0',
+            95:	'00cf75',
+            100:'fae6a0',
+    },
+
         "credentials": "https://spdx.org/licenses/CC-BY-4.0.html",
     },
 }
```

### Comparing `metobs_toolkit-0.1.1a0/metobs_toolkit/settings_files/world_boundaries/WB_countries_Admin0_10m.shp` & `metobs_toolkit-0.1.1a2/metobs_toolkit/settings_files/world_boundaries/WB_countries_Admin0_10m.shp`

 * *Files identical despite different names*

### Comparing `metobs_toolkit-0.1.1a0/metobs_toolkit/settings_files/world_boundaries/WB_countries_Admin0_10m.shx` & `metobs_toolkit-0.1.1a2/metobs_toolkit/settings_files/world_boundaries/WB_countries_Admin0_10m.shx`

 * *Files identical despite different names*

### Comparing `metobs_toolkit-0.1.1a0/metobs_toolkit/writing_files.py` & `metobs_toolkit-0.1.1a2/metobs_toolkit/writing_files.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,14 +3,17 @@
 """
 Created on Thu Mar  2 15:30:55 2023
 
 @author: thoverga
 """
 # --
 import os
+import logging
+
+logger = logging.getLogger(__name__)
 
 
 def write_dataset_to_csv(
     df, metadf, filename, outputfolder, location_info, seperate_metadata_file,
 ):
     """
     Write the dataset to a file where the observations, metadata and (if available)
@@ -51,14 +54,15 @@
         # merge metadata
         df = df.merge(metadf, how="left", left_on="name", right_index=True)
         df = df.drop(columns=ignore_metadat)
     else:
         metadf = metadf.reset_index()
         metadf = metadf.drop(columns=ignore_metadat)
         metadatafile = os.path.join(outputfolder, "metadata_file.csv")
+        logger.info(f"write metadata to file: {metadatafile}")
         print(f"write metadata to file: {metadatafile}")
         metadf.to_csv(path_or_buf=metadatafile, sep=";", na_rep="NaN", index=False)
 
 
 
 
     df = df.sort_values(["name", "datetime"])
@@ -71,9 +75,10 @@
     else:
         if filename.endswith(".csv"):
             filename = filename[:-4]  # to avoid two times .csv.csv
 
     filepath = os.path.join(outputfolder, filename + ".csv")
 
     # write to csv in output folder
+    logger.info(f"write dataset to file: {filepath}")
     print(f"write dataset to file: {filepath}")
     df.to_csv(path_or_buf=filepath, sep=";", na_rep="NaN", index=False)
```

### Comparing `metobs_toolkit-0.1.1a0/pyproject.toml` & `metobs_toolkit-0.1.1a2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 [tool.poetry]
 name = "MetObs-toolkit"
-version = "0.1.1a0"
+version = "0.1.1a2"
 description = "A Meteorological observations toolkit for scientists"
 authors = ["Thomas Vergauwen <thomas.vergauwen@meteo.be>"]
 maintainers = ["Thomas Vergauwen <thomas.vergauwen@meteo.be>"]
 license = "LICENSE"
 readme = "README.md"
 documentation = "https://python-poetry.org/docs/"
 packages = [{include = "metobs_toolkit"}]
 keywords = ["meteorology", "observations", "urban climate"]
 
 [tool.poetry.dependencies]
-python = "^3.9"
+python = "^3.9" #can be converted to 3.8 (but to risky so close to the summerschool)
 pandas = "^1.3.0"
 numpy = "^1.17.3"
 matplotlib = "^3.0.0"
 mysql-connector-python = "^8.0.6"
 geopandas = "^0.9.0"
 pyproj = "~3.4"
 mapclassify = "^2.4.0"
 earthengine-api = "^0.1.340"
-PyQt5 = "=5.12.2" #Technical: this version is the latest to build from source
-pyqt5-sip = "^12.12.1"
-pyqt5-qt5 = "^5.15.2"
+geemap = '^0.20.0'
+titanlib = "^0.3" #can give errors due to C-compiler in windows ....
+
+
 
 
 
 [tool.poetry.group.dev.dependencies]
 poetry = "^1.3.2"
 
 [build-system]
```

### Comparing `metobs_toolkit-0.1.1a0/PKG-INFO` & `metobs_toolkit-0.1.1a2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 Metadata-Version: 2.1
 Name: metobs-toolkit
-Version: 0.1.1a0
+Version: 0.1.1a2
 Summary: A Meteorological observations toolkit for scientists
 License: LICENSE
 Keywords: meteorology,observations,urban climate
 Author: Thomas Vergauwen
 Author-email: thomas.vergauwen@meteo.be
 Maintainer: Thomas Vergauwen
 Maintainer-email: thomas.vergauwen@meteo.be
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: PyQt5 (==5.12.2)
 Requires-Dist: earthengine-api (>=0.1.340,<0.2.0)
+Requires-Dist: geemap (>=0.20.0,<0.21.0)
 Requires-Dist: geopandas (>=0.9.0,<0.10.0)
 Requires-Dist: mapclassify (>=2.4.0,<3.0.0)
 Requires-Dist: matplotlib (>=3.0.0,<4.0.0)
 Requires-Dist: mysql-connector-python (>=8.0.6,<9.0.0)
 Requires-Dist: numpy (>=1.17.3,<2.0.0)
 Requires-Dist: pandas (>=1.3.0,<2.0.0)
 Requires-Dist: pyproj (>=3.4,<3.5)
-Requires-Dist: pyqt5-qt5 (>=5.15.2,<6.0.0)
-Requires-Dist: pyqt5-sip (>=12.12.1,<13.0.0)
+Requires-Dist: titanlib (>=0.3,<0.4)
 Project-URL: Documentation, https://python-poetry.org/docs/
 Description-Content-Type: text/markdown
 
 # MetObs-toolkit
 
 This repo contains all the software for the [metobs_toolkit](https://test.pypi.org/project/metobs-toolkit/).
 The MetObs-toolkit is a package for scientists who make use meteorological observations.
```

