# Comparing `tmp/edc_screening-0.3.8-py3-none-any.whl.zip` & `tmp/edc_screening-0.3.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,13 @@
-Zip file size: 26078 bytes, number of entries: 29
+Zip file size: 26580 bytes, number of entries: 31
 -rw-r--r--  2.0 unx      209 b- defN 21-Feb-07 13:38 edc_screening/__init__.py
 -rw-r--r--  2.0 unx     1225 b- defN 21-Mar-01 04:03 edc_screening/age_evaluator.py
 -rw-r--r--  2.0 unx      151 b- defN 20-Mar-04 23:31 edc_screening/apps.py
+-rw-r--r--  2.0 unx       24 b- defN 21-Sep-14 02:13 edc_screening/auth_objects.py
+-rw-r--r--  2.0 unx      211 b- defN 21-Sep-14 02:13 edc_screening/auths.py
 -rw-r--r--  2.0 unx      325 b- defN 21-Jul-15 03:55 edc_screening/choices.py
 -rw-r--r--  2.0 unx     2905 b- defN 21-Mar-01 04:03 edc_screening/eligibility.py
 -rw-r--r--  2.0 unx      519 b- defN 21-Mar-01 04:03 edc_screening/gender_evaluator.py
 -rw-r--r--  2.0 unx     1025 b- defN 21-Mar-01 04:03 edc_screening/modelform_mixins.py
 -rw-r--r--  2.0 unx        0 b- defN 20-Mar-04 23:31 edc_screening/models.py
 -rw-r--r--  2.0 unx     1040 b- defN 21-Mar-01 04:03 edc_screening/screening_eligibility.py
 -rw-r--r--  2.0 unx      318 b- defN 21-Feb-22 03:31 edc_screening/screening_identifier.py
@@ -18,14 +20,14 @@
 -rw-r--r--  2.0 unx      796 b- defN 21-Mar-01 04:03 edc_screening/model_mixins/screening_methods_model_mixin.py
 -rw-r--r--  2.0 unx      619 b- defN 20-Apr-29 22:06 edc_screening/model_mixins/screening_model_mixin.py
 -rw-r--r--  2.0 unx        0 b- defN 20-Mar-04 23:31 edc_screening/tests/__init__.py
 -rw-r--r--  2.0 unx      625 b- defN 21-Sep-12 17:18 edc_screening/tests/models.py
 -rw-r--r--  2.0 unx      350 b- defN 20-Mar-04 23:31 edc_screening/tests/test_evaluators.py
 -rw-r--r--  2.0 unx     1064 b- defN 21-Apr-16 14:44 edc_screening/tests/test_screening.py
 -rw-r--r--  2.0 unx      116 b- defN 21-Feb-07 13:38 edc_screening/tests/urls.py
--rw-r--r--  2.0 unx       37 b- defN 21-Sep-12 17:26 edc_screening-0.3.8.dist-info/AUTHORS
--rw-r--r--  2.0 unx    35149 b- defN 21-Sep-12 17:26 edc_screening-0.3.8.dist-info/LICENSE
--rw-r--r--  2.0 unx     1456 b- defN 21-Sep-12 17:26 edc_screening-0.3.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 21-Sep-12 17:26 edc_screening-0.3.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       14 b- defN 21-Sep-12 17:26 edc_screening-0.3.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     2621 b- defN 21-Sep-12 17:26 edc_screening-0.3.8.dist-info/RECORD
-29 files, 59482 bytes uncompressed, 21762 bytes compressed:  63.4%
+-rw-r--r--  2.0 unx       37 b- defN 21-Sep-14 02:13 edc_screening-0.3.9.dist-info/AUTHORS
+-rw-r--r--  2.0 unx    35149 b- defN 21-Sep-14 02:13 edc_screening-0.3.9.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1456 b- defN 21-Sep-14 02:13 edc_screening-0.3.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 21-Sep-14 02:13 edc_screening-0.3.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       14 b- defN 21-Sep-14 02:13 edc_screening-0.3.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     2783 b- defN 21-Sep-14 02:13 edc_screening-0.3.9.dist-info/RECORD
+31 files, 59879 bytes uncompressed, 22010 bytes compressed:  63.2%
```

## zipnote {}

```diff
@@ -3,14 +3,20 @@
 
 Filename: edc_screening/age_evaluator.py
 Comment: 
 
 Filename: edc_screening/apps.py
 Comment: 
 
+Filename: edc_screening/auth_objects.py
+Comment: 
+
+Filename: edc_screening/auths.py
+Comment: 
+
 Filename: edc_screening/choices.py
 Comment: 
 
 Filename: edc_screening/eligibility.py
 Comment: 
 
 Filename: edc_screening/gender_evaluator.py
@@ -63,26 +69,26 @@
 
 Filename: edc_screening/tests/test_screening.py
 Comment: 
 
 Filename: edc_screening/tests/urls.py
 Comment: 
 
-Filename: edc_screening-0.3.8.dist-info/AUTHORS
+Filename: edc_screening-0.3.9.dist-info/AUTHORS
 Comment: 
 
-Filename: edc_screening-0.3.8.dist-info/LICENSE
+Filename: edc_screening-0.3.9.dist-info/LICENSE
 Comment: 
 
-Filename: edc_screening-0.3.8.dist-info/METADATA
+Filename: edc_screening-0.3.9.dist-info/METADATA
 Comment: 
 
-Filename: edc_screening-0.3.8.dist-info/WHEEL
+Filename: edc_screening-0.3.9.dist-info/WHEEL
 Comment: 
 
-Filename: edc_screening-0.3.8.dist-info/top_level.txt
+Filename: edc_screening-0.3.9.dist-info/top_level.txt
 Comment: 
 
-Filename: edc_screening-0.3.8.dist-info/RECORD
+Filename: edc_screening-0.3.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `edc_screening-0.3.8.dist-info/LICENSE` & `edc_screening-0.3.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `edc_screening-0.3.8.dist-info/METADATA` & `edc_screening-0.3.9.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edc-screening
-Version: 0.3.8
+Version: 0.3.9
 Summary: Screening fields and method mixins.
 Home-page: https://github.com/clinicedc/edc_screening
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django edc screening
 Platform: UNKNOWN
```

## Comparing `edc_screening-0.3.8.dist-info/RECORD` & `edc_screening-0.3.9.dist-info/RECORD`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 edc_screening/__init__.py,sha256=mdINLrKcUHTscXlsPAZf43BqrgRPADJhj1tLvT6Jhwc,209
 edc_screening/age_evaluator.py,sha256=Rt1tli3LL4SFx38WnVsc6vJvwBXC7vIL0kebI5qCpWc,1225
 edc_screening/apps.py,sha256=O2ZdsusCjy7LOrv2BWm3vX_l32FsL4HHlaz6iUiMQyw,151
+edc_screening/auth_objects.py,sha256=rB6uVKAZZ8Ui-K6e7fPFsN6fnFJjBWbZh47CnvmSTWs,24
+edc_screening/auths.py,sha256=Cw_-o9O-DpocSe_ORU1XC0WDmZBJmKIk1VcNcBx8fcE,211
 edc_screening/choices.py,sha256=e8qx6dPCqTcgCTSRmzhciueOWxHPP1dbvvV0kpd2-P4,325
 edc_screening/eligibility.py,sha256=0Vh07m2ZuJ_ykBpnqUfo2rxPN5dXbHwvQ_UxhcE7WjY,2905
 edc_screening/gender_evaluator.py,sha256=4B-zyz3IHM2mpwK-A5KbfdPaXFyQsCk2gpEdrloS3yM,519
 edc_screening/modelform_mixins.py,sha256=d7FNNptBI52TJ1DEUcUXQy5-x7l4pvwp0fEjym49c1M,1025
 edc_screening/models.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 edc_screening/screening_eligibility.py,sha256=YeVWUI-6HbWgt8bkpQ1daUe_vTiYejzyThN0Y80x2PU,1040
 edc_screening/screening_identifier.py,sha256=EeQGCCj8eSFKR50GKYPG2ZB_utDcKjpUhcafYvcLMDk,318
@@ -17,13 +19,13 @@
 edc_screening/model_mixins/screening_methods_model_mixin.py,sha256=nQyPdORB-qsBgNfLi1MHTniebmBsthwkX1H5dpZgQ2M,796
 edc_screening/model_mixins/screening_model_mixin.py,sha256=3g6ZEuXlQusf8fLV2r-pkByKEF_6J0JdVqR3EpqwDuY,619
 edc_screening/tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 edc_screening/tests/models.py,sha256=_nlP0GXITSd2WoyvNEHM3wMmtNaHfiway-VijnEvd-E,625
 edc_screening/tests/test_evaluators.py,sha256=VW-vytZg3fDJZwicIt3euHMsUJADQRp5H2KtleeHBuI,350
 edc_screening/tests/test_screening.py,sha256=hChFm_TmlMStz0QyYGmzZD9y-ST0GobRFNwlQcfSl9E,1064
 edc_screening/tests/urls.py,sha256=CjGPtSGO4dflUXAQOEQXr5HdeyhFl9brQhgR-ONQ4cw,116
-edc_screening-0.3.8.dist-info/AUTHORS,sha256=bASVS-K7ZNbIK4-9QOpuBM4CAkpiE5g8DKv7rSqST5g,37
-edc_screening-0.3.8.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
-edc_screening-0.3.8.dist-info/METADATA,sha256=QrDm2dh0XOwO4dZTCZps4YZTXp227x8TSn3l8alTv4E,1456
-edc_screening-0.3.8.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
-edc_screening-0.3.8.dist-info/top_level.txt,sha256=rMABhPKdfH1meYhZ4wKTLsU_7cQAMukUQo1qdO15Ku0,14
-edc_screening-0.3.8.dist-info/RECORD,,
+edc_screening-0.3.9.dist-info/AUTHORS,sha256=bASVS-K7ZNbIK4-9QOpuBM4CAkpiE5g8DKv7rSqST5g,37
+edc_screening-0.3.9.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
+edc_screening-0.3.9.dist-info/METADATA,sha256=MaXvwSu1zcZkk9Hlcga_6mxNXvEFlEIWxL4BJ23CuDk,1456
+edc_screening-0.3.9.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
+edc_screening-0.3.9.dist-info/top_level.txt,sha256=rMABhPKdfH1meYhZ4wKTLsU_7cQAMukUQo1qdO15Ku0,14
+edc_screening-0.3.9.dist-info/RECORD,,
```

