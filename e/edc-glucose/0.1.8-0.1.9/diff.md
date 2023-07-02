# Comparing `tmp/edc_glucose-0.1.8-py3-none-any.whl.zip` & `tmp/edc_glucose-0.1.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 25048 bytes, number of entries: 28
+Zip file size: 25037 bytes, number of entries: 28
 -rw-r--r--  2.0 unx        0 b- defN 21-Jul-02 03:33 edc_glucose/__init__.py
 -rw-r--r--  2.0 unx      147 b- defN 21-Aug-03 03:41 edc_glucose/apps.py
 -rw-r--r--  2.0 unx      112 b- defN 21-Oct-13 01:30 edc_glucose/constants.py
 -rw-r--r--  2.0 unx        0 b- defN 21-Sep-12 16:28 edc_glucose/models.py
 -rw-r--r--  2.0 unx     1138 b- defN 21-Oct-13 01:30 edc_glucose/utils.py
 -rw-r--r--  2.0 unx      316 b- defN 21-Sep-12 16:28 edc_glucose/form_validators/__init__.py
 -rw-r--r--  2.0 unx     1133 b- defN 21-Sep-12 16:28 edc_glucose/form_validators/glucose_form_validator.py
--rw-r--r--  2.0 unx      700 b- defN 21-Sep-13 03:13 edc_glucose/form_validators/glucose_form_validator_mixin.py
+-rw-r--r--  2.0 unx      696 b- defN 22-Jan-09 23:17 edc_glucose/form_validators/glucose_form_validator_mixin.py
 -rw-r--r--  2.0 unx      870 b- defN 21-Sep-13 03:13 edc_glucose/form_validators/ifg_form_validator_mixin.py
 -rw-r--r--  2.0 unx     1341 b- defN 21-Sep-13 03:13 edc_glucose/form_validators/ifg_ogtt_form_validator_mixin.py
 -rw-r--r--  2.0 unx     3191 b- defN 22-Jan-08 16:18 edc_glucose/form_validators/ogtt_form_validator_mixin.py
 -rw-r--r--  2.0 unx        0 b- defN 21-Sep-12 16:28 edc_glucose/migrations/__init__.py
 -rw-r--r--  2.0 unx      186 b- defN 21-Sep-12 16:28 edc_glucose/model_mixins/__init__.py
 -rw-r--r--  2.0 unx     2857 b- defN 21-Jul-02 03:33 edc_glucose/model_mixins/blood_glucose_model_mixin.py
 -rw-r--r--  2.0 unx     1016 b- defN 22-Jan-08 16:18 edc_glucose/model_mixins/fasting_model_mixin.py
@@ -18,13 +18,13 @@
 -rw-r--r--  2.0 unx     1186 b- defN 21-Oct-13 01:30 edc_glucose/model_mixins/ifg_model_mixin.py
 -rw-r--r--  2.0 unx     1578 b- defN 21-Oct-13 01:32 edc_glucose/model_mixins/ogtt_model_mixin.py
 -rw-r--r--  2.0 unx        0 b- defN 21-Sep-11 19:28 edc_glucose/tests/__init__.py
 -rw-r--r--  2.0 unx      627 b- defN 21-Sep-12 16:28 edc_glucose/tests/models.py
 -rw-r--r--  2.0 unx      257 b- defN 21-Aug-03 03:41 edc_glucose/tests/urls.py
 -rw-r--r--  2.0 unx        0 b- defN 21-Sep-11 19:04 edc_glucose/tests/tests/__init__.py
 -rw-r--r--  2.0 unx     4411 b- defN 21-Sep-12 16:28 edc_glucose/tests/tests/test_glucose_form_validator.py
--rw-r--r--  2.0 unx    35149 b- defN 22-Jan-08 16:18 edc_glucose-0.1.8.dist-info/LICENSE
--rw-r--r--  2.0 unx     1464 b- defN 22-Jan-08 16:18 edc_glucose-0.1.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 22-Jan-08 16:18 edc_glucose-0.1.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 22-Jan-08 16:18 edc_glucose-0.1.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     2596 b- defN 22-Jan-08 16:18 edc_glucose-0.1.8.dist-info/RECORD
-28 files, 61442 bytes uncompressed, 20738 bytes compressed:  66.2%
+-rw-r--r--  2.0 unx    35149 b- defN 22-Jan-09 23:17 edc_glucose-0.1.9.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1464 b- defN 22-Jan-09 23:17 edc_glucose-0.1.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 22-Jan-09 23:17 edc_glucose-0.1.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 22-Jan-09 23:17 edc_glucose-0.1.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     2596 b- defN 22-Jan-09 23:17 edc_glucose-0.1.9.dist-info/RECORD
+28 files, 61438 bytes uncompressed, 20727 bytes compressed:  66.3%
```

## zipnote {}

```diff
@@ -63,23 +63,23 @@
 
 Filename: edc_glucose/tests/tests/__init__.py
 Comment: 
 
 Filename: edc_glucose/tests/tests/test_glucose_form_validator.py
 Comment: 
 
-Filename: edc_glucose-0.1.8.dist-info/LICENSE
+Filename: edc_glucose-0.1.9.dist-info/LICENSE
 Comment: 
 
-Filename: edc_glucose-0.1.8.dist-info/METADATA
+Filename: edc_glucose-0.1.9.dist-info/METADATA
 Comment: 
 
-Filename: edc_glucose-0.1.8.dist-info/WHEEL
+Filename: edc_glucose-0.1.9.dist-info/WHEEL
 Comment: 
 
-Filename: edc_glucose-0.1.8.dist-info/top_level.txt
+Filename: edc_glucose-0.1.9.dist-info/top_level.txt
 Comment: 
 
-Filename: edc_glucose-0.1.8.dist-info/RECORD
+Filename: edc_glucose-0.1.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## edc_glucose/form_validators/glucose_form_validator_mixin.py

```diff
@@ -6,8 +6,8 @@
 class GlucoseFormValidatorMixin:
     def validate_glucose_test(self):
         self.required_if(YES, field="glucose_performed", field_required="glucose_date")
         self.required_if(YES, field="glucose_performed", field_required="fasting")
         self.required_if(YES, field="glucose_performed", field_required="glucose_value")
         validate_glucose_as_millimoles_per_liter("glucose", self.cleaned_data)
         self.required_if(YES, field="glucose_performed", field_required="glucose_quantifier")
-        self.applicable_if(YES, field="glucose_performed", field_applicable="glucose_units")
+        self.required_if(YES, field="glucose_performed", field_required="glucose_units")
```

## Comparing `edc_glucose-0.1.8.dist-info/LICENSE` & `edc_glucose-0.1.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `edc_glucose-0.1.8.dist-info/METADATA` & `edc_glucose-0.1.9.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edc-glucose
-Version: 0.1.8
+Version: 0.1.9
 Summary: Classes to collect glucose, IFG, OGTT
 Home-page: https://github.com/clinicedc/edc-glucose
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django edc glucose ifg ogtt
 Platform: UNKNOWN
```

## Comparing `edc_glucose-0.1.8.dist-info/RECORD` & `edc_glucose-0.1.9.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 edc_glucose/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 edc_glucose/apps.py,sha256=i9yDA3ArJQ5uPNPMmFkrAwZsuKBJjptHCfvjiHY7-Ok,147
 edc_glucose/constants.py,sha256=RiDCNh3bf_YkfAso3G-_7rjH2A7xL9VSZDE2l45GAy0,112
 edc_glucose/models.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 edc_glucose/utils.py,sha256=nPQhEn6woEQqVGSSpfn9oNs0aeLoQi7RCrZ8oK3dk28,1138
 edc_glucose/form_validators/__init__.py,sha256=_GWOl9bj2qtZb8tLKPCO8LUN6XpnnyeCNt-s2fXfuCY,316
 edc_glucose/form_validators/glucose_form_validator.py,sha256=hW8Tr7Cxgo2N_ipIOWVXaEw4kq5nrAbFMtMkPrYKgM0,1133
-edc_glucose/form_validators/glucose_form_validator_mixin.py,sha256=nyzYAVkkKVRr-xeJvpNxcpn3ePhnFeJgqscFbEw-sXs,700
+edc_glucose/form_validators/glucose_form_validator_mixin.py,sha256=RbYzLkMhSvt2kB77CUX9vdcWtsuAsttYvYdMaZvoed4,696
 edc_glucose/form_validators/ifg_form_validator_mixin.py,sha256=yGXQ8KyoM5QVbVykWaW6nYuVJlfj2NdXpDTtsZ3ScWE,870
 edc_glucose/form_validators/ifg_ogtt_form_validator_mixin.py,sha256=0rPqchuPrf4nSPMH_yNz3EWbCJ6YbFe4OueGx8wTZCc,1341
 edc_glucose/form_validators/ogtt_form_validator_mixin.py,sha256=vqbJzRcZqzIGKZqWd_709puQWlrnii_gR93B-dzr_pc,3191
 edc_glucose/migrations/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 edc_glucose/model_mixins/__init__.py,sha256=W4SSJTIF__BvD9rVx2q8-G66z7LgaO9ACv5WG0QF1wg,186
 edc_glucose/model_mixins/blood_glucose_model_mixin.py,sha256=Gqxms6nziBr9bQL2i2TGh5gxjB_a6GfsW1fwatxPeHw,2857
 edc_glucose/model_mixins/fasting_model_mixin.py,sha256=OYP1A0_KbqbqWSb4jvEJCgUDnSH5sn4N3FRDGzg3z54,1016
@@ -17,12 +17,12 @@
 edc_glucose/model_mixins/ifg_model_mixin.py,sha256=TIC3ZSTe5qfHheQ9GZBjT2MIzipjs-RbAdxIZDYYoUI,1186
 edc_glucose/model_mixins/ogtt_model_mixin.py,sha256=fnoOfsQJmD5e4dP9R7YBWm3SeD1zj7IBJ28IeX-XguE,1578
 edc_glucose/tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 edc_glucose/tests/models.py,sha256=M0yeOAbFij7mq-0erXogxrrCmB6mZg-jWM4WqKS2EJE,627
 edc_glucose/tests/urls.py,sha256=5zGAqQJHBg5gZN2Wmx3XTWq2vBHNcO7yGE85eeWZZmw,257
 edc_glucose/tests/tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 edc_glucose/tests/tests/test_glucose_form_validator.py,sha256=EADhJap9EkxPgOVqOMHY_QKUHa_A1Tt_3Ha3_atuYdk,4411
-edc_glucose-0.1.8.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
-edc_glucose-0.1.8.dist-info/METADATA,sha256=jy3O648UDrsTJZdPOAykkDimSNHXWqgb4QHPIQQSB88,1464
-edc_glucose-0.1.8.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
-edc_glucose-0.1.8.dist-info/top_level.txt,sha256=O4JbZNGghvng0innd3C46CuVttp8lmggUHF53RD_mU4,12
-edc_glucose-0.1.8.dist-info/RECORD,,
+edc_glucose-0.1.9.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
+edc_glucose-0.1.9.dist-info/METADATA,sha256=3HxvHZVsK4GYqE6IPZImcI5DXDGF-KesNCMlQSDupds,1464
+edc_glucose-0.1.9.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
+edc_glucose-0.1.9.dist-info/top_level.txt,sha256=O4JbZNGghvng0innd3C46CuVttp8lmggUHF53RD_mU4,12
+edc_glucose-0.1.9.dist-info/RECORD,,
```

