# Comparing `tmp/odoo_addons_oca_timesheet-16.0.20230629.0-py3-none-any.whl.zip` & `tmp/odoo_addons_oca_timesheet-16.0.20230701.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,6 +1,6 @@
-Zip file size: 1381 bytes, number of entries: 4
--rw-r--r--  2.0 unx      587 b- defN 23-Jun-30 07:05 odoo_addons_oca_timesheet-16.0.20230629.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-30 07:05 odoo_addons_oca_timesheet-16.0.20230629.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 23-Jun-30 07:05 odoo_addons_oca_timesheet-16.0.20230629.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      408 b- defN 23-Jun-30 07:05 odoo_addons_oca_timesheet-16.0.20230629.0.dist-info/RECORD
-4 files, 1088 bytes uncompressed, 575 bytes compressed:  47.2%
+Zip file size: 1392 bytes, number of entries: 4
+-rw-r--r--  2.0 unx      661 b- defN 23-Jul-02 05:34 odoo_addons_oca_timesheet-16.0.20230701.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-02 05:34 odoo_addons_oca_timesheet-16.0.20230701.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 23-Jul-02 05:34 odoo_addons_oca_timesheet-16.0.20230701.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      408 b- defN 23-Jul-02 05:34 odoo_addons_oca_timesheet-16.0.20230701.0.dist-info/RECORD
+4 files, 1162 bytes uncompressed, 586 bytes compressed:  49.6%
```

## zipnote {}

```diff
@@ -1,13 +1,13 @@
-Filename: odoo_addons_oca_timesheet-16.0.20230629.0.dist-info/METADATA
+Filename: odoo_addons_oca_timesheet-16.0.20230701.0.dist-info/METADATA
 Comment: 
 
-Filename: odoo_addons_oca_timesheet-16.0.20230629.0.dist-info/WHEEL
+Filename: odoo_addons_oca_timesheet-16.0.20230701.0.dist-info/WHEEL
 Comment: 
 
-Filename: odoo_addons_oca_timesheet-16.0.20230629.0.dist-info/top_level.txt
+Filename: odoo_addons_oca_timesheet-16.0.20230701.0.dist-info/top_level.txt
 Comment: 
 
-Filename: odoo_addons_oca_timesheet-16.0.20230629.0.dist-info/RECORD
+Filename: odoo_addons_oca_timesheet-16.0.20230701.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `odoo_addons_oca_timesheet-16.0.20230629.0.dist-info/METADATA` & `odoo_addons_oca_timesheet-16.0.20230701.0.dist-info/METADATA`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: odoo-addons-oca-timesheet
-Version: 16.0.20230629.0
+Version: 16.0.20230701.0
 Summary: Meta package for oca-timesheet Odoo addons
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Framework :: Odoo
 Classifier: Framework :: Odoo :: 16.0
 Requires-Dist: odoo-addon-hr-timesheet-begin-end (<16.1dev,>=16.0dev)
+Requires-Dist: odoo-addon-hr-timesheet-name-customer (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-hr-timesheet-sheet (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-hr-timesheet-task-required (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-hr-timesheet-task-stage (<16.1dev,>=16.0dev)
 
 UNKNOWN
```

