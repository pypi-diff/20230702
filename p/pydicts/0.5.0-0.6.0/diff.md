# Comparing `tmp/pydicts-0.5.0.tar.gz` & `tmp/pydicts-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydicts-0.5.0.tar", max compression
+gzip compressed data, was "pydicts-0.6.0.tar", max compression
```

## Comparing `pydicts-0.5.0.tar` & `pydicts-0.6.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0    35149 2023-04-10 16:27:20.112887 pydicts-0.5.0/LICENSE
--rw-r--r--   0        0        0     3401 2023-05-04 17:12:16.245845 pydicts-0.5.0/README.md
--rw-r--r--   0        0        0      143 2023-05-04 17:11:12.157843 pydicts-0.5.0/pydicts/__init__.py
--rw-r--r--   0        0        0     2814 2023-04-11 05:44:25.702913 pydicts-0.5.0/pydicts/classes.py
--rw-r--r--   0        0        0      424 2023-05-04 17:12:34.664846 pydicts-0.5.0/pydicts/locale/en/LC_MESSAGES/pydicts.mo
--rw-r--r--   0        0        0      738 2022-04-25 13:52:57.304754 pydicts-0.5.0/pydicts/locale/en.po
--rw-r--r--   0        0        0      513 2023-05-04 17:12:34.662845 pydicts-0.5.0/pydicts/locale/es/LC_MESSAGES/pydicts.mo
--rw-r--r--   0        0        0     2755 2023-04-19 17:40:24.132024 pydicts-0.5.0/pydicts/locale/es.po
--rw-r--r--   0        0        0      633 2023-04-19 17:40:13.925023 pydicts-0.5.0/pydicts/locale/pydicts.pot
--rw-r--r--   0        0        0     5811 2023-05-03 15:58:54.826246 pydicts-0.5.0/pydicts/lod.py
--rw-r--r--   0        0        0     1052 2023-04-12 05:25:02.458349 pydicts-0.5.0/pydicts/lod_xyv.py
--rw-r--r--   0        0        0     8792 2023-04-15 22:54:44.487769 pydicts-0.5.0/pydicts/lod_ymv.py
--rw-r--r--   0        0        0     3716 2023-05-04 17:10:10.584841 pydicts-0.5.0/pydicts/pylatex.py
--rw-r--r--   0        0        0        0 2023-04-10 16:27:20.112887 pydicts-0.5.0/pydicts/tests/__init__.py
--rw-r--r--   0        0        0     1064 2023-04-19 17:53:54.673048 pydicts-0.5.0/pydicts/tests/test_lod.py
--rw-r--r--   0        0        0      409 2023-04-12 05:32:28.379363 pydicts-0.5.0/pydicts/tests/test_lod_ymv.py
--rw-r--r--   0        0        0     1038 2023-05-04 17:14:37.488849 pydicts-0.5.0/pydicts/tests/test_pylatex.py
--rw-r--r--   0        0        0      816 2023-05-04 17:10:46.554842 pydicts-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     3918 1970-01-01 00:00:00.000000 pydicts-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-10 16:27:20.112887 pydicts-0.6.0/LICENSE
+-rw-r--r--   0        0        0     3496 2023-07-02 08:21:36.147527 pydicts-0.6.0/README.md
+-rw-r--r--   0        0        0      143 2023-07-02 08:20:07.917524 pydicts-0.6.0/pydicts/__init__.py
+-rw-r--r--   0        0        0     2814 2023-04-11 05:44:25.702913 pydicts-0.6.0/pydicts/classes.py
+-rw-r--r--   0        0        0      424 2023-07-02 08:21:43.953527 pydicts-0.6.0/pydicts/locale/en/LC_MESSAGES/pydicts.mo
+-rw-r--r--   0        0        0      738 2022-04-25 13:52:57.304754 pydicts-0.6.0/pydicts/locale/en.po
+-rw-r--r--   0        0        0      513 2023-07-02 08:21:43.951527 pydicts-0.6.0/pydicts/locale/es/LC_MESSAGES/pydicts.mo
+-rw-r--r--   0        0        0     2755 2023-04-19 17:40:24.132024 pydicts-0.6.0/pydicts/locale/es.po
+-rw-r--r--   0        0        0      633 2023-04-19 17:40:13.925023 pydicts-0.6.0/pydicts/locale/pydicts.pot
+-rw-r--r--   0        0        0     5811 2023-05-03 15:58:54.826246 pydicts-0.6.0/pydicts/lod.py
+-rw-r--r--   0        0        0     1052 2023-04-12 05:25:02.458349 pydicts-0.6.0/pydicts/lod_xyv.py
+-rw-r--r--   0        0        0     9707 2023-07-02 08:06:04.240499 pydicts-0.6.0/pydicts/lod_ymv.py
+-rw-r--r--   0        0        0     3716 2023-05-04 17:10:10.584841 pydicts-0.6.0/pydicts/pylatex.py
+-rw-r--r--   0        0        0        0 2023-04-10 16:27:20.112887 pydicts-0.6.0/pydicts/tests/__init__.py
+-rw-r--r--   0        0        0     1064 2023-04-19 17:53:54.673048 pydicts-0.6.0/pydicts/tests/test_lod.py
+-rw-r--r--   0        0        0     5973 2023-07-02 08:09:33.101505 pydicts-0.6.0/pydicts/tests/test_lod_ymv.py
+-rw-r--r--   0        0        0     1038 2023-05-04 17:14:37.488849 pydicts-0.6.0/pydicts/tests/test_pylatex.py
+-rw-r--r--   0        0        0      816 2023-07-02 08:19:47.082524 pydicts-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     4013 1970-01-01 00:00:00.000000 pydicts-0.6.0/PKG-INFO
```

### Comparing `pydicts-0.5.0/LICENSE` & `pydicts-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pydicts-0.5.0/README.md` & `pydicts-0.6.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -141,14 +141,17 @@
 ### lod_ymv_filling
 
 ## Testing
 poetry run pytest
 
 ## CHANGELOG
 
+### 0.6.0 (2023-07-02)
+- Fixed a race condition bug in lod_ymv_transposition_with_percentages
+
 ### 0.5.0 (2023-05-04)
 - Added support to latex tables from list of dictionaries
 
 ### 0.4.0 (2023-04-19)
 - Added poetry support
 - Added poethepoet support
 - Added lod_remove_key
```

### Comparing `pydicts-0.5.0/pydicts/classes.py` & `pydicts-0.6.0/pydicts/classes.py`

 * *Files identical despite different names*

### Comparing `pydicts-0.5.0/pydicts/locale/en.po` & `pydicts-0.6.0/pydicts/locale/en.po`

 * *Files identical despite different names*

### Comparing `pydicts-0.5.0/pydicts/locale/es/LC_MESSAGES/pydicts.mo` & `pydicts-0.6.0/pydicts/locale/es/LC_MESSAGES/pydicts.mo`

 * *Files identical despite different names*

### Comparing `pydicts-0.5.0/pydicts/locale/es.po` & `pydicts-0.6.0/pydicts/locale/es.po`

 * *Files identical despite different names*

### Comparing `pydicts-0.5.0/pydicts/locale/pydicts.pot` & `pydicts-0.6.0/pydicts/locale/pydicts.pot`

 * *Files identical despite different names*

### Comparing `pydicts-0.5.0/pydicts/lod.py` & `pydicts-0.6.0/pydicts/lod.py`

 * *Files identical despite different names*

### Comparing `pydicts-0.5.0/pydicts/lod_xyv.py` & `pydicts-0.6.0/pydicts/lod_xyv.py`

 * *Files identical despite different names*

### Comparing `pydicts-0.5.0/pydicts/lod_ymv.py` & `pydicts-0.6.0/pydicts/lod_ymv.py`

 * *Files 9% similar despite different names*

```diff
@@ -84,32 +84,53 @@
     #Calculate totals
     for year in range(min_year,max_year+1):
         d=r[year-min_year]
         d["total"]=d["m1"]+d["m2"]+d["m3"]+d["m4"]+d["m5"]+d["m6"]+d["m7"]+d["m8"]+d["m9"]+d["m10"]+d["m11"]+d["m12"]
 
     return r
     
-def d_ymv_transposition_first_value(d):
+def is_noz(v):
+    if v is None:
+        return True
+    if v==0:
+        return True
+    return False
+    
+def ymv_transposition_first_value_not_noz(lod_ymv_transposition):
+    """
+        REturns a dict with the coords of the first value of the ymv_transposition not null
+        noz null or zero
+        
+    """
+    for d in lod_ymv_transposition:
+        for i in range(1, 13):
+            if not is_noz(d[f"m{i}"]):
+                return {"year": d["year"],  "month": i ,  "value":d[f"m{i}"]  }
+    return None
+    
+def d_ymv_transposition_first_key_not_noz(d):
     """
         REturns the first key mX not null in dictionary
+        noz null or zero
     """
     r=None
     for i in range(1, 13):
-        if d[f"m{i}"]!=0:
+        if not is_noz(d[f"m{i}"]):
             r= f"m{i}"
             break
     return r
 
-def d_ymv_transposition_last_value(d):
+def d_ymv_transposition_last_key_not_noz(d):
     """
         REturns the last key mX not null in dictionary
+        noz null or zero
     """
     r=None
     for i in reversed(range(1, 13)):
-        if d[f"m{i}"]!=0:
+        if not is_noz(d[f"m{i}"]):
             r= f"m{i}"
             break
     return r
 
     
 def lod_ymv_transposition_with_percentages(lod_ymv_transposition):
     """
@@ -118,16 +139,18 @@
     def percentage(from_,  to_):
         if from_ is None or from_==0:
             return None
         if to_ is None or to_==0:
             return None
         return (to_-from_)/from_
     ###########################
+    
+    first_value_not_noz=ymv_transposition_first_value_not_noz(lod_ymv_transposition)
     r=[]
-    if len(lod_ymv_transposition)==0:
+    if first_value_not_noz is None:
         return r
     for i, d in enumerate(lod_ymv_transposition):
         new_d={"year":d["year"]}
         new_d["m1"]=None if i==0 else percentage(lod_ymv_transposition[i-1]["m12"], d["m1"])
         new_d["m2"]=percentage(d["m1"], d["m2"])
         new_d["m3"]=percentage(d["m2"], d["m3"])
         new_d["m4"]=percentage(d["m3"], d["m4"])
@@ -135,21 +158,22 @@
         new_d["m6"]=percentage(d["m5"], d["m6"])
         new_d["m7"]=percentage(d["m6"], d["m7"])
         new_d["m8"]=percentage(d["m7"], d["m8"])
         new_d["m9"]=percentage(d["m8"], d["m9"])
         new_d["m10"]=percentage(d["m9"], d["m10"])
         new_d["m11"]=percentage(d["m10"], d["m11"])
         new_d["m12"]=percentage(d["m11"], d["m12"])
+        key_first_value=d_ymv_transposition_first_key_not_noz(d)
+        key_last_value=d_ymv_transposition_last_key_not_noz(d)
         if i==0:
-            new_d["total"]=percentage(d[d_ymv_transposition_first_value(d)], d[d_ymv_transposition_last_value(d)])
-            new_d["from_first_quote"]=percentage
+            new_d["total"]=None if key_first_value is None or key_last_value is None else percentage(d[key_first_value], d[key_last_value])
         else:
-            new_d["total"]=percentage(lod_ymv_transposition[i-1]["m12"], d[d_ymv_transposition_last_value(d)])
-        new_d["from_first_quote"]=percentage(lod_ymv_transposition[0][d_ymv_transposition_first_value(lod_ymv_transposition[0])], d[d_ymv_transposition_last_value(d)])
-            
+            key_previous_last_value=d_ymv_transposition_last_key_not_noz(lod_ymv_transposition[i-1])
+            new_d["total"]=None if key_previous_last_value is None or key_last_value is None else percentage(lod_ymv_transposition[i-1][key_previous_last_value], d[key_last_value])
+        new_d["from_first_quote"]=None if key_last_value is None else percentage(first_value_not_noz["value"], d[key_last_value])
         r.append(new_d)
     return r
 
 def lod_ymv_transposition_sum(lymv_a, lymv_b):
     """
         Sums to lod_ymv_transpositions
     """
```

### Comparing `pydicts-0.5.0/pydicts/pylatex.py` & `pydicts-0.6.0/pydicts/pylatex.py`

 * *Files identical despite different names*

### Comparing `pydicts-0.5.0/pydicts/tests/test_lod.py` & `pydicts-0.6.0/pydicts/tests/test_lod.py`

 * *Files identical despite different names*

### Comparing `pydicts-0.5.0/pydicts/tests/test_pylatex.py` & `pydicts-0.6.0/pydicts/tests/test_pylatex.py`

 * *Files identical despite different names*

### Comparing `pydicts-0.5.0/pyproject.toml` & `pydicts-0.6.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "pydicts"
-version = "0.5.0"
+version = "0.6.0"
 description = "Module to use dictionaries in various situations"
 authors = ["turulomio <turulomio@yahoo.es>"]
 license = "GPL-3.0"
 readme = "README.md"
 exclude = [
     "pydicts/devscripts.py"
 ]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 tabulate = "^0.9.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.0"
-poethepoet = "^0.19.0"
+poethepoet = "^0.20.0"
 pylatex = "^1.4.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poe.tasks]
```

### Comparing `pydicts-0.5.0/PKG-INFO` & `pydicts-0.6.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydicts
-Version: 0.5.0
+Version: 0.6.0
 Summary: Module to use dictionaries in various situations
 License: GPL-3.0
 Author: turulomio
 Author-email: turulomio@yahoo.es
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
@@ -156,14 +156,17 @@
 ### lod_ymv_filling
 
 ## Testing
 poetry run pytest
 
 ## CHANGELOG
 
+### 0.6.0 (2023-07-02)
+- Fixed a race condition bug in lod_ymv_transposition_with_percentages
+
 ### 0.5.0 (2023-05-04)
 - Added support to latex tables from list of dictionaries
 
 ### 0.4.0 (2023-04-19)
 - Added poetry support
 - Added poethepoet support
 - Added lod_remove_key
```

