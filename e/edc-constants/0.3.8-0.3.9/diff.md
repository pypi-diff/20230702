# Comparing `tmp/edc_constants-0.3.8-py3-none-any.whl.zip` & `tmp/edc_constants-0.3.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 15771 bytes, number of entries: 11
+Zip file size: 15791 bytes, number of entries: 11
 -rw-r--r--  2.0 unx        0 b- defN 20-Mar-04 23:17 edc_constants/__init__.py
 -rw-r--r--  2.0 unx      151 b- defN 21-Feb-09 03:32 edc_constants/apps.py
--rw-r--r--  2.0 unx    14451 b- defN 21-Jul-01 03:04 edc_constants/choices.py
+-rw-r--r--  2.0 unx    14613 b- defN 21-Aug-12 02:46 edc_constants/choices.py
 -rw-r--r--  2.0 unx     2861 b- defN 21-Jul-27 17:40 edc_constants/constants.py
 -rw-r--r--  2.0 unx      663 b- defN 20-Mar-04 23:17 edc_constants/date_constants.py
 -rw-r--r--  2.0 unx      474 b- defN 21-Feb-09 03:32 edc_constants/utils.py
--rw-r--r--  2.0 unx    18047 b- defN 21-Jul-27 17:41 edc_constants-0.3.8.dist-info/LICENSE
--rw-r--r--  2.0 unx     1064 b- defN 21-Jul-27 17:41 edc_constants-0.3.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 21-Jul-27 17:41 edc_constants-0.3.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       14 b- defN 21-Jul-27 17:41 edc_constants-0.3.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      903 b- defN 21-Jul-27 17:41 edc_constants-0.3.8.dist-info/RECORD
-11 files, 38720 bytes uncompressed, 14237 bytes compressed:  63.2%
+-rw-r--r--  2.0 unx    18047 b- defN 21-Aug-12 02:46 edc_constants-0.3.9.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1064 b- defN 21-Aug-12 02:46 edc_constants-0.3.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 21-Aug-12 02:46 edc_constants-0.3.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       14 b- defN 21-Aug-12 02:46 edc_constants-0.3.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      903 b- defN 21-Aug-12 02:46 edc_constants-0.3.9.dist-info/RECORD
+11 files, 38882 bytes uncompressed, 14257 bytes compressed:  63.3%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: edc_constants/date_constants.py
 Comment: 
 
 Filename: edc_constants/utils.py
 Comment: 
 
-Filename: edc_constants-0.3.8.dist-info/LICENSE
+Filename: edc_constants-0.3.9.dist-info/LICENSE
 Comment: 
 
-Filename: edc_constants-0.3.8.dist-info/METADATA
+Filename: edc_constants-0.3.9.dist-info/METADATA
 Comment: 
 
-Filename: edc_constants-0.3.8.dist-info/WHEEL
+Filename: edc_constants-0.3.9.dist-info/WHEEL
 Comment: 
 
-Filename: edc_constants-0.3.8.dist-info/top_level.txt
+Filename: edc_constants-0.3.9.dist-info/top_level.txt
 Comment: 
 
-Filename: edc_constants-0.3.8.dist-info/RECORD
+Filename: edc_constants-0.3.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## edc_constants/choices.py

```diff
@@ -8,23 +8,25 @@
     ANYTIME,
     DEAD,
     DECLINED,
     DONT_KNOW,
     DWTA,
     EVENING,
     FALSE,
+    FASTING,
     FEMALE,
     FORMER_SMOKER,
     IND,
     MALE,
     MORNING,
     NAIVE,
     NEG,
     NEVER,
     NO,
+    NON_FASTING,
     NONSMOKER,
     NORMAL,
     NOT_APPLICABLE,
     NOT_DONE,
     NOT_ESTIMATED,
     NOT_RECORDED,
     NOT_REQUIRED,
@@ -40,16 +42,14 @@
     SMOKER,
     TBD,
     TRUE,
     UNKNOWN,
     WEEKDAYS,
     WEEKENDS,
     YES,
-    FASTING,
-    NON_FASTING,
 )
 
 BLANK_CHOICE_DASH = [("", "---------")]
 
 """ Try to keep these in alphabetical order
 """
 
@@ -269,22 +269,33 @@
 
 GENDER_UNDETERMINED = (
     (MALE, _("Male")),
     (FEMALE, _("Female")),
     ("U", _("Undetermined")),
 )
 
+
 GRADING_SCALE = (
     (1, "Grade 1"),
     (2, "Grade 2"),
     (3, "Grade 3"),
     (4, "Grade 4"),
     (5, "Grade 5"),
 )
 
+
+GRADING_SCALE_WITH_NOT_GRADED = (
+    (0, "Not graded"),
+    (1, "Grade 1"),
+    (2, "Grade 2"),
+    (3, "Grade 3"),
+    (4, "Grade 4"),
+    (5, "Grade 5"),
+)
+
 GRADING_SCALE_234 = ((2, "Grade 2"), (3, "Grade 3"), (4, "Grade 4"))
 
 GRADING_SCALE_34 = ((3, "Grade 3"), (4, "Grade 4"))
 
 HIV_RESULT = (
     (POS, "HIV Positive (Reactive)"),
     (NEG, "HIV Negative (Non-reactive)"),
```

## Comparing `edc_constants-0.3.8.dist-info/LICENSE` & `edc_constants-0.3.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `edc_constants-0.3.8.dist-info/METADATA` & `edc_constants-0.3.9.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edc-constants
-Version: 0.3.8
+Version: 0.3.9
 Summary: Common constants & choices for clinicedc/edc projects.
 Home-page: https://github.com/clinicedc/edc-constants
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django edc choices constants
 Platform: UNKNOWN
```

