# Comparing `tmp/pp_project_pkg-1.0.202307011948-py3-none-any.whl.zip` & `tmp/pp_project_pkg-1.0.202307020131-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,21 +1,21 @@
-Zip file size: 12634 bytes, number of entries: 19
+Zip file size: 12588 bytes, number of entries: 19
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jun-27 22:23 mlflow_pipelines/__init__.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jun-27 22:23 mlflow_pipelines/fetch_data/__init__.py
 -rw-rw-r--  2.0 unx      887 b- defN 23-Jun-27 22:23 mlflow_pipelines/fetch_data/get_data.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jun-27 22:23 mlflow_pipelines/train_model/__init__.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jun-27 22:23 mlflow_pipelines/train_model/model_train.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jun-27 22:23 mlflow_pipelines/upload_data/__init__.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jun-27 22:23 mlflow_pipelines/upload_data/data_upload.py
 -rw-rw-r--  2.0 unx       71 b- defN 23-Jun-07 11:24 pp_project_pkg/__init__.py
 -rw-rw-r--  2.0 unx     5335 b- defN 23-Jun-23 12:39 pp_project_pkg/linear_train.py
 -rw-rw-r--  2.0 unx      577 b- defN 23-Jun-07 11:24 pp_project_pkg/newsvendor.py
 -rw-rw-r--  2.0 unx     9252 b- defN 23-Jun-27 22:23 pp_project_pkg/pp_tables.py
 -rw-rw-r--  2.0 unx     7448 b- defN 23-Jul-01 19:37 pp_project_pkg/utils.py
--rw-rw-r--  2.0 unx      396 b- defN 23-Jul-01 19:48 pp_project_pkg/version.py
--rw-rw-r--  2.0 unx     5395 b- defN 23-Jul-01 19:48 pp_project_pkg/wrangling.py
--rwxrwxr-x  2.0 unx     1316 b- defN 23-Jun-07 11:24 pp_project_pkg-1.0.202307011948.data/scripts/pp_project_run.py
--rw-rw-r--  2.0 unx      191 b- defN 23-Jul-01 19:49 pp_project_pkg-1.0.202307011948.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jul-01 19:49 pp_project_pkg-1.0.202307011948.dist-info/WHEEL
--rw-rw-r--  2.0 unx       32 b- defN 23-Jul-01 19:49 pp_project_pkg-1.0.202307011948.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1721 b- defN 23-Jul-01 19:49 pp_project_pkg-1.0.202307011948.dist-info/RECORD
-19 files, 32713 bytes uncompressed, 9728 bytes compressed:  70.3%
+-rw-rw-r--  2.0 unx      396 b- defN 23-Jul-02 01:31 pp_project_pkg/version.py
+-rw-rw-r--  2.0 unx     5301 b- defN 23-Jul-02 01:31 pp_project_pkg/wrangling.py
+-rwxrwxr-x  2.0 unx     1316 b- defN 23-Jun-07 11:24 pp_project_pkg-1.0.202307020131.data/scripts/pp_project_run.py
+-rw-rw-r--  2.0 unx      191 b- defN 23-Jul-02 01:31 pp_project_pkg-1.0.202307020131.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jul-02 01:31 pp_project_pkg-1.0.202307020131.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       32 b- defN 23-Jul-02 01:31 pp_project_pkg-1.0.202307020131.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1721 b- defN 23-Jul-02 01:31 pp_project_pkg-1.0.202307020131.dist-info/RECORD
+19 files, 32619 bytes uncompressed, 9682 bytes compressed:  70.3%
```

## zipnote {}

```diff
@@ -36,23 +36,23 @@
 
 Filename: pp_project_pkg/version.py
 Comment: 
 
 Filename: pp_project_pkg/wrangling.py
 Comment: 
 
-Filename: pp_project_pkg-1.0.202307011948.data/scripts/pp_project_run.py
+Filename: pp_project_pkg-1.0.202307020131.data/scripts/pp_project_run.py
 Comment: 
 
-Filename: pp_project_pkg-1.0.202307011948.dist-info/METADATA
+Filename: pp_project_pkg-1.0.202307020131.dist-info/METADATA
 Comment: 
 
-Filename: pp_project_pkg-1.0.202307011948.dist-info/WHEEL
+Filename: pp_project_pkg-1.0.202307020131.dist-info/WHEEL
 Comment: 
 
-Filename: pp_project_pkg-1.0.202307011948.dist-info/top_level.txt
+Filename: pp_project_pkg-1.0.202307020131.dist-info/top_level.txt
 Comment: 
 
-Filename: pp_project_pkg-1.0.202307011948.dist-info/RECORD
+Filename: pp_project_pkg-1.0.202307020131.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pp_project_pkg/version.py

```diff
@@ -1,11 +1,11 @@
 VERSION_YEAR = 2023
 VERSION_MONTH = int('07')
-VERSION_DAY = int('01')
-VERSION_HOUR = int('19')
-VERSION_MINUTE = int('48')
+VERSION_DAY = int('02')
+VERSION_HOUR = int('01')
+VERSION_MINUTE = int('31')
 MAJOR_VERSION = 1
 MINOR_VERSION = 0
-PATCH_VERSION = 202307011948
-version_date = '2023/07/01 19:48'
+PATCH_VERSION = 202307020131
+version_date = '2023/07/02 01:31'
 version = '{}.{}.{}'.format(MAJOR_VERSION, MINOR_VERSION, PATCH_VERSION)
 __all__  = ['MAJOR_VERSION', 'MINOR_VERSION', 'PATCH_VERSION', 'version_date', 'version']
```

## pp_project_pkg/wrangling.py

```diff
@@ -55,21 +55,20 @@
      
     if logger and site_data:
         logger.info('Site info {} : {}'.format(site_data['site_id'],site_info['tracker_name'].values[0]))
         logger.info('Cover count for the date {} : {}'.format(site_data['date'],cover_count))
         logger.info('pp_production_rework total : {}'.format(pp_production_rework['rework'].sum()))
 
     # Filter the filtered dataframe based on the 'local_time' column
-    try:     
+    if filtered_df.empty:
+        itemised_overproduction = pd.DataFrame(columns=list(waste_data_for_site.columns))
+    else:
         itemised_overproduction = filtered_df.loc[(filtered_df['local_time'].dt.time >= meal_period_start_dt.time()) & (filtered_df['local_time'].dt.time <= meal_period_end_dt.time())]
         itemised_overproduction = itemised_overproduction[list(waste_data_for_site.columns)]
-    except:
-        print("Error in filtering the dataframe")
-        print("filtered_df : {}".format(filtered_df.head()))
-        print("filetered_df['local_time'] : {}'.format(filtered_df['local_time'])")
+
 
     joined_df = food_items.join(itemised_overproduction.set_index('item_id'), on='waste_identifier', how='left',rsuffix='_2')
 
     # Group the joined dataframe by 'food_item_id' and calculate the sum of 'weight_g' column while replacing null values with 0
     grouped_df = joined_df.groupby('food_item_id')['weight_g'].sum().fillna(0)
 
     # Convert the resulting series object to a dataframe
```

## Comparing `pp_project_pkg-1.0.202307011948.data/scripts/pp_project_run.py` & `pp_project_pkg-1.0.202307020131.data/scripts/pp_project_run.py`

 * *Files identical despite different names*

## Comparing `pp_project_pkg-1.0.202307011948.dist-info/RECORD` & `pp_project_pkg-1.0.202307020131.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -6,14 +6,14 @@
 mlflow_pipelines/upload_data/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 mlflow_pipelines/upload_data/data_upload.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pp_project_pkg/__init__.py,sha256=9idX2X6SQKZg--ziGy6Ii9OB-kz9hOX1nEG9a0xEW9g,71
 pp_project_pkg/linear_train.py,sha256=xW9v6KON3cAC3-4yP50rC6VCwv0tCeJ6h25oILWyGRw,5335
 pp_project_pkg/newsvendor.py,sha256=E6JHp0Vtmq63toKM6bO3xTAdCgwmAZzRua-w10wrc5Y,577
 pp_project_pkg/pp_tables.py,sha256=aNBP-aExfiPWTINChNLIzIIgTUrVo-z26Oq8cLTky2w,9252
 pp_project_pkg/utils.py,sha256=KmLqDW3F66lo5e4oQFNCMrUZGVtFkHbqgxjyODeeVY8,7448
-pp_project_pkg/version.py,sha256=Zoflwovbuc01qfrfW2ScJex2Oj8aK_Bg--glhIxpiTc,396
-pp_project_pkg/wrangling.py,sha256=nbwQXo6AJ1HQ-bbMXBEdYYMSJvfL3RwU9yQCPYSxV-E,5395
-pp_project_pkg-1.0.202307011948.data/scripts/pp_project_run.py,sha256=hNrYjtDlo7nX9pwMbM7un9R7ToKRdjVosBt3qErKtaA,1316
-pp_project_pkg-1.0.202307011948.dist-info/METADATA,sha256=-pQ_bc0F_Mm2UxyWeZU1qZDurG_EpaSyzJP1Ot3Cdo4,191
-pp_project_pkg-1.0.202307011948.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
-pp_project_pkg-1.0.202307011948.dist-info/top_level.txt,sha256=aTmpGcM2s0GVN0z4bWc23t0I3mXhHxeqKNzUWghwIRA,32
-pp_project_pkg-1.0.202307011948.dist-info/RECORD,,
+pp_project_pkg/version.py,sha256=JAM_ju1LZ_eV87_h-9ZyDpmC2KqGGVvZHh_L5-kACis,396
+pp_project_pkg/wrangling.py,sha256=g9y6mJXvtV-C1YNel_fLRjhtqpPtXcL131Mc1NdVv8s,5301
+pp_project_pkg-1.0.202307020131.data/scripts/pp_project_run.py,sha256=hNrYjtDlo7nX9pwMbM7un9R7ToKRdjVosBt3qErKtaA,1316
+pp_project_pkg-1.0.202307020131.dist-info/METADATA,sha256=0evVB0EKKTTKZxWvfFOVWf1khQa1-345UfgEu-3bdjE,191
+pp_project_pkg-1.0.202307020131.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
+pp_project_pkg-1.0.202307020131.dist-info/top_level.txt,sha256=aTmpGcM2s0GVN0z4bWc23t0I3mXhHxeqKNzUWghwIRA,32
+pp_project_pkg-1.0.202307020131.dist-info/RECORD,,
```

