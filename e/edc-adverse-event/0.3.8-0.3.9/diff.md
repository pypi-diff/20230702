# Comparing `tmp/edc_adverse_event-0.3.8-py3-none-any.whl.zip` & `tmp/edc_adverse_event-0.3.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 122154 bytes, number of entries: 158
+Zip file size: 122099 bytes, number of entries: 158
 -rw-r--r--  2.0 unx        0 b- defN 20-Mar-04 23:30 adverse_event_app/__init__.py
 -rw-r--r--  2.0 unx     1417 b- defN 21-Feb-04 16:09 adverse_event_app/action_items.py
 -rw-r--r--  2.0 unx      452 b- defN 21-Feb-04 16:09 adverse_event_app/admin.py
 -rw-r--r--  2.0 unx      120 b- defN 21-Feb-04 16:09 adverse_event_app/apps.py
 -rw-r--r--  2.0 unx     1801 b- defN 21-Feb-04 16:09 adverse_event_app/baker_recipes.py
 -rw-r--r--  2.0 unx      488 b- defN 21-Feb-04 16:09 adverse_event_app/consents.py
--rw-r--r--  2.0 unx     1866 b- defN 21-Feb-04 16:09 adverse_event_app/list_data.py
+-rw-r--r--  2.0 unx     1740 b- defN 21-Jul-16 05:36 adverse_event_app/list_data.py
 -rw-r--r--  2.0 unx     3584 b- defN 21-Feb-04 16:09 adverse_event_app/models.py
 -rw-r--r--  2.0 unx     1100 b- defN 21-Feb-04 16:09 adverse_event_app/visit_schedules.py
 -rw-r--r--  2.0 unx       54 b- defN 20-Mar-04 23:31 edc_adverse_event/__init__.py
 -rw-r--r--  2.0 unx      603 b- defN 21-Feb-04 16:09 edc_adverse_event/admin.py
 -rw-r--r--  2.0 unx      185 b- defN 21-May-14 21:35 edc_adverse_event/admin_site.py
 -rw-r--r--  2.0 unx      610 b- defN 21-May-14 21:35 edc_adverse_event/apps.py
 -rw-r--r--  2.0 unx      228 b- defN 20-Mar-04 23:31 edc_adverse_event/baker_recipes.py
@@ -147,14 +147,14 @@
 -rw-r--r--  2.0 unx      207 b- defN 21-Feb-04 16:09 edc_adverse_event/views/__init__.py
 -rw-r--r--  2.0 unx     1451 b- defN 21-May-14 21:35 edc_adverse_event/views/home_view.py
 -rw-r--r--  2.0 unx      265 b- defN 21-Feb-04 16:09 edc_adverse_event/views/tmg/__init__.py
 -rw-r--r--  2.0 unx     2324 b- defN 21-Feb-04 16:09 edc_adverse_event/views/tmg/death_listboard_view.py
 -rw-r--r--  2.0 unx     2680 b- defN 21-Feb-04 16:09 edc_adverse_event/views/tmg/home_view.py
 -rw-r--r--  2.0 unx     1093 b- defN 21-Feb-04 16:09 edc_adverse_event/views/tmg/status_listboards.py
 -rw-r--r--  2.0 unx     3875 b- defN 21-Feb-04 16:09 edc_adverse_event/views/tmg/summary_listboard_view.py
--rw-r--r--  2.0 unx       37 b- defN 21-Jul-12 02:49 edc_adverse_event-0.3.8.dist-info/AUTHORS
--rw-r--r--  2.0 unx    35149 b- defN 21-Jul-12 02:49 edc_adverse_event-0.3.8.dist-info/LICENSE
--rw-r--r--  2.0 unx     4166 b- defN 21-Jul-12 02:49 edc_adverse_event-0.3.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 21-Jul-12 02:49 edc_adverse_event-0.3.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       36 b- defN 21-Jul-12 02:49 edc_adverse_event-0.3.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx    17067 b- defN 21-Jul-12 02:49 edc_adverse_event-0.3.8.dist-info/RECORD
-158 files, 334487 bytes uncompressed, 93708 bytes compressed:  72.0%
+-rw-r--r--  2.0 unx       37 b- defN 21-Jul-16 05:37 edc_adverse_event-0.3.9.dist-info/AUTHORS
+-rw-r--r--  2.0 unx    35149 b- defN 21-Jul-16 05:37 edc_adverse_event-0.3.9.dist-info/LICENSE
+-rw-r--r--  2.0 unx     4166 b- defN 21-Jul-16 05:37 edc_adverse_event-0.3.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 21-Jul-16 05:37 edc_adverse_event-0.3.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       36 b- defN 21-Jul-16 05:37 edc_adverse_event-0.3.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx    17067 b- defN 21-Jul-16 05:37 edc_adverse_event-0.3.9.dist-info/RECORD
+158 files, 334361 bytes uncompressed, 93653 bytes compressed:  72.0%
```

## zipnote {}

```diff
@@ -450,26 +450,26 @@
 
 Filename: edc_adverse_event/views/tmg/status_listboards.py
 Comment: 
 
 Filename: edc_adverse_event/views/tmg/summary_listboard_view.py
 Comment: 
 
-Filename: edc_adverse_event-0.3.8.dist-info/AUTHORS
+Filename: edc_adverse_event-0.3.9.dist-info/AUTHORS
 Comment: 
 
-Filename: edc_adverse_event-0.3.8.dist-info/LICENSE
+Filename: edc_adverse_event-0.3.9.dist-info/LICENSE
 Comment: 
 
-Filename: edc_adverse_event-0.3.8.dist-info/METADATA
+Filename: edc_adverse_event-0.3.9.dist-info/METADATA
 Comment: 
 
-Filename: edc_adverse_event-0.3.8.dist-info/WHEEL
+Filename: edc_adverse_event-0.3.9.dist-info/WHEEL
 Comment: 
 
-Filename: edc_adverse_event-0.3.8.dist-info/top_level.txt
+Filename: edc_adverse_event-0.3.9.dist-info/top_level.txt
 Comment: 
 
-Filename: edc_adverse_event-0.3.8.dist-info/RECORD
+Filename: edc_adverse_event-0.3.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## adverse_event_app/list_data.py

```diff
@@ -1,9 +1,8 @@
 from edc_constants.constants import DEAD, MALIGNANCY, NOT_APPLICABLE, OTHER, UNKNOWN
-from edc_list_data import PreloadData
 
 list_data = {
     "edc_adverse_event.causeofdeath": [
         ("bacteraemia", "Bacteraemia"),
         ("bacterial_pneumonia", "Bacterial pneumonia"),
         (MALIGNANCY, "Malignancy"),
         ("art_toxicity", "ART toxicity"),
@@ -43,9 +42,7 @@
             "medically_important_event",
             "Medically important event (e.g. Severe thrombophlebitis, Bacteraemia, "
             "recurrence of symptoms not requiring admission, Hospital acquired "
             "pneumonia)",
         ),
     ],
 }
-
-preload_data = PreloadData(list_data=list_data, model_data={}, unique_field_data=None)
```

## Comparing `edc_adverse_event-0.3.8.dist-info/LICENSE` & `edc_adverse_event-0.3.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `edc_adverse_event-0.3.8.dist-info/METADATA` & `edc_adverse_event-0.3.9.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edc-adverse-event
-Version: 0.3.8
+Version: 0.3.9
 Summary: Adverse event and death classes.
 Home-page: http://github.com/clinicedc/edc-adverse-event
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django edc adverse event
 Platform: UNKNOWN
```

## Comparing `edc_adverse_event-0.3.8.dist-info/RECORD` & `edc_adverse_event-0.3.9.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 adverse_event_app/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 adverse_event_app/action_items.py,sha256=uTtieSQ0N2mfWQYvRZ63jpZGTKRyOp6gJ2J8nnR4Lmo,1417
 adverse_event_app/admin.py,sha256=7C2Zf7_hQWTMRmjTuX9mCjJGMe3yKh0eJg3tuk5XHTs,452
 adverse_event_app/apps.py,sha256=GPWcQpyTHZOi7Wf-MrBJP3vNKBtavveUl1jUexaSFGg,120
 adverse_event_app/baker_recipes.py,sha256=oRltrodPpvtDN5t6Z2tU8DtK2QrgT_nuj4TZv3xrgeM,1801
 adverse_event_app/consents.py,sha256=Gnt9kZFwQ49R9ldbvQITlEjcDFFvTl266HSMyb0UHsc,488
-adverse_event_app/list_data.py,sha256=bvy9KUhVZyotZ2ZuaBh2TcxngPMgj6bwiEwgJRSLFJk,1866
+adverse_event_app/list_data.py,sha256=5GWR7PF9jXP_1bZqCzoz9Qd5qaugMOtAzb5l46CUU-Y,1740
 adverse_event_app/models.py,sha256=c3QMHcEKvlOSbNHVK7kPLUdkU9wn_cKehksL3gCX624,3584
 adverse_event_app/visit_schedules.py,sha256=F_RmtJZUmjevIrCFOya6ku9QsdHvsCnaxHtQ9CYHbhE,1100
 edc_adverse_event/__init__.py,sha256=2v6qMR2RJDh-uH8c2FpP35gl3YNrGM4zOPsH9UgNpVA,54
 edc_adverse_event/admin.py,sha256=-7VCcu2HY1UjxSHcVX6ng8HzHzPpHVCnYSVLdAIX-PY,603
 edc_adverse_event/admin_site.py,sha256=0-i75MQAyFI71TfoAkk3Z3LogsFsqksibAMUQymn3xk,185
 edc_adverse_event/apps.py,sha256=tc7B1Gt1FrnNJnRoWUdZSa-DrijZtcTcE2b9Yeb8VoA,610
 edc_adverse_event/baker_recipes.py,sha256=_eW98UqQdgZsqY1irZhsZNA52WaQjEutevyCkdE_YqY,228
@@ -146,13 +146,13 @@
 edc_adverse_event/views/__init__.py,sha256=PY-nkoQmCIlBR9MHq8x3TU_jeXvryx48AM728zkhtYg,207
 edc_adverse_event/views/home_view.py,sha256=4NmhlnefvVaCALDuzpJVlca56Nnu0ZhCIatZP-PKPkc,1451
 edc_adverse_event/views/tmg/__init__.py,sha256=9f4vIR0KEvH58IgN_eNcahHd1BavM2YYPe59aiM_-uE,265
 edc_adverse_event/views/tmg/death_listboard_view.py,sha256=U_xC9XNPY-ZrS1GDygUWk7eQRApeSnpObOpqPgYdg5o,2324
 edc_adverse_event/views/tmg/home_view.py,sha256=vNO8XWD7BYD1xEb6OGatEWU5Ce4IZl8Lq5ugmxNAV30,2680
 edc_adverse_event/views/tmg/status_listboards.py,sha256=Bcq3dz6RmtShbVwyUOou28cnC6UeZo-CW5Np1h8wYaY,1093
 edc_adverse_event/views/tmg/summary_listboard_view.py,sha256=iPkafrhvjuhmpf8GCRPevzHNtkIBBASHpbNqxKjs_UI,3875
-edc_adverse_event-0.3.8.dist-info/AUTHORS,sha256=bASVS-K7ZNbIK4-9QOpuBM4CAkpiE5g8DKv7rSqST5g,37
-edc_adverse_event-0.3.8.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
-edc_adverse_event-0.3.8.dist-info/METADATA,sha256=BuAJ1wN4ngvUTEVcMWVLU5dLgif0qKuNy-kjvhRyS1U,4166
-edc_adverse_event-0.3.8.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
-edc_adverse_event-0.3.8.dist-info/top_level.txt,sha256=S2P-niwij6F9npUC2ksYsDNzOmVPAe_rgrGxc4iVyoo,36
-edc_adverse_event-0.3.8.dist-info/RECORD,,
+edc_adverse_event-0.3.9.dist-info/AUTHORS,sha256=bASVS-K7ZNbIK4-9QOpuBM4CAkpiE5g8DKv7rSqST5g,37
+edc_adverse_event-0.3.9.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
+edc_adverse_event-0.3.9.dist-info/METADATA,sha256=HyL26Gqz6sp5Exn6UUvqCJCyoWZOXvR4PdfDLdda-Q8,4166
+edc_adverse_event-0.3.9.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
+edc_adverse_event-0.3.9.dist-info/top_level.txt,sha256=S2P-niwij6F9npUC2ksYsDNzOmVPAe_rgrGxc4iVyoo,36
+edc_adverse_event-0.3.9.dist-info/RECORD,,
```

