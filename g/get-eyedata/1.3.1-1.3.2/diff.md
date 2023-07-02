# Comparing `tmp/get_eyedata-1.3.1-py3-none-any.whl.zip` & `tmp/get_eyedata-1.3.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 8165 bytes, number of entries: 9
+Zip file size: 8122 bytes, number of entries: 9
 -rw-rw-rw-  2.0 fat        6 b- defN 23-Jun-05 08:24 get_eyedata/__init__.py
 -rw-rw-rw-  2.0 fat     2340 b- defN 23-Jun-30 06:07 get_eyedata/frame_utils.py
--rw-rw-rw-  2.0 fat     4216 b- defN 23-Jul-01 06:06 get_eyedata/ow2.py
+-rw-rw-rw-  2.0 fat     4008 b- defN 23-Jul-02 01:38 get_eyedata/ow2.py
 -rw-rw-rw-  2.0 fat     5284 b- defN 23-Jun-30 06:28 get_eyedata/valo.py
--rw-rw-rw-  2.0 fat     1091 b- defN 23-Jul-01 06:09 get_eyedata-1.3.1.dist-info/LICENCE
--rw-rw-rw-  2.0 fat     1869 b- defN 23-Jul-01 06:09 get_eyedata-1.3.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-01 06:09 get_eyedata-1.3.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       12 b- defN 23-Jul-01 06:09 get_eyedata-1.3.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      717 b- defN 23-Jul-01 06:09 get_eyedata-1.3.1.dist-info/RECORD
-9 files, 15627 bytes uncompressed, 6929 bytes compressed:  55.7%
+-rw-rw-rw-  2.0 fat     1091 b- defN 23-Jul-02 01:41 get_eyedata-1.3.2.dist-info/LICENCE
+-rw-rw-rw-  2.0 fat     1869 b- defN 23-Jul-02 01:41 get_eyedata-1.3.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-02 01:41 get_eyedata-1.3.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       12 b- defN 23-Jul-02 01:41 get_eyedata-1.3.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      717 b- defN 23-Jul-02 01:41 get_eyedata-1.3.2.dist-info/RECORD
+9 files, 15419 bytes uncompressed, 6886 bytes compressed:  55.3%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: get_eyedata/ow2.py
 Comment: 
 
 Filename: get_eyedata/valo.py
 Comment: 
 
-Filename: get_eyedata-1.3.1.dist-info/LICENCE
+Filename: get_eyedata-1.3.2.dist-info/LICENCE
 Comment: 
 
-Filename: get_eyedata-1.3.1.dist-info/METADATA
+Filename: get_eyedata-1.3.2.dist-info/METADATA
 Comment: 
 
-Filename: get_eyedata-1.3.1.dist-info/WHEEL
+Filename: get_eyedata-1.3.2.dist-info/WHEEL
 Comment: 
 
-Filename: get_eyedata-1.3.1.dist-info/top_level.txt
+Filename: get_eyedata-1.3.2.dist-info/top_level.txt
 Comment: 
 
-Filename: get_eyedata-1.3.1.dist-info/RECORD
+Filename: get_eyedata-1.3.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## get_eyedata/ow2.py

```diff
@@ -12,38 +12,33 @@
 @dataclass
 class Area:
     name: str
     top_x: int
     top_y: int
     bottom_x: int
     bottom_y: int
-    center_x: int = None
-    center_y: int = None
-    radius: int = None
-
+    
 areas = [
-    Area('center', 960, 540, 960, 540, 125),
     Area('hp', 50, 50, 500, 250),
     Area('chat', 50, 330, 500, 500),
     Area('ult', 880, 50, 1040, 220),
     Area('my_status', 1450, 50, 1900, 280),
     Area('match_status', 650, 880, 1300, 1080),
     Area('kill_log', 1450, 880, 1920, 1080)
 ]
 
 def get_roi(x, y):
-    for area in areas:
-        if area.name == 'center' and area.center_x and area.center_y and area.radius:
-            if ((x - area.center_x) ** 2 + (y - area.center_y) ** 2) <= area.radius ** 2:
+    if ((x - 960)**2 + (y - 540)**2) <= 125**2:
+        return 'center'
+    else:
+        for area in areas:
+            if area.top_x <= x <= area.bottom_x and area.top_y <= y <= area.bottom_y:
                 return area.name
-        elif area.top_x <= x <= area.bottom_x and area.top_y <= y <= area.bottom_y:
-            return area.name
-    return 'other'
-
-
+            else:
+                return 'other'
 
 def check(file_path:str):
     if os.path.exists(file_path):
         return True
     else:
         print('FileNotFoundError')
         return False
```

## Comparing `get_eyedata-1.3.1.dist-info/LICENCE` & `get_eyedata-1.3.2.dist-info/LICENCE`

 * *Files identical despite different names*

## Comparing `get_eyedata-1.3.1.dist-info/METADATA` & `get_eyedata-1.3.2.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: get-eyedata
-Version: 1.3.1
+Version: 1.3.2
 Summary: gat gaze data form record.
 Home-page: https://github.com/ikrfun/get_eyedata
 Download-URL: https://github.com/ikrfun/get_eyedata
 Author: ikrfun
 Author-email: t.nobuto130625@gmail.com
 Maintainer: ikrfun
 Maintainer-email: t.nobuto130625@gmail.com
```

## Comparing `get_eyedata-1.3.1.dist-info/RECORD` & `get_eyedata-1.3.2.dist-info/RECORD`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 get_eyedata/__init__.py,sha256=rqUtJyMLicobcyhmr74TepjmUQAEmlazKT3vjV_n3aA,6
 get_eyedata/frame_utils.py,sha256=YEFiSBzqLeJ12s0KBDzxYVdloB45AgOQrJxU-xGM1Y8,2340
-get_eyedata/ow2.py,sha256=hl7wzKS5qFwrwf1dV3IKU8z-qkEzMpXe_EFJDFva_l4,4216
+get_eyedata/ow2.py,sha256=8YoB58-9dRnBLnQ_V9KYs0jUTJYXp0zrrakB1Jlefj8,4008
 get_eyedata/valo.py,sha256=9NAJFBDHIoHGKbvwIL_5QWDtxheWg_3LPjMBxU5sdEA,5284
-get_eyedata-1.3.1.dist-info/LICENCE,sha256=44r0hK-BnpFZTBiPxTYe52HFlT034sEPBfHrJyaNI0g,1091
-get_eyedata-1.3.1.dist-info/METADATA,sha256=4ThJOOTCkueOJ7RMNIuDB4uw3o8Zsc4uynP2O8mY5QY,1869
-get_eyedata-1.3.1.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-get_eyedata-1.3.1.dist-info/top_level.txt,sha256=zlueM7ZefajCSIgOyib56hk_6HWx15EsED6S68g0mWE,12
-get_eyedata-1.3.1.dist-info/RECORD,,
+get_eyedata-1.3.2.dist-info/LICENCE,sha256=44r0hK-BnpFZTBiPxTYe52HFlT034sEPBfHrJyaNI0g,1091
+get_eyedata-1.3.2.dist-info/METADATA,sha256=cSGeOy1UJqtoTfuQ2ZNN2zVn5_D3JlV_-hmsGzOg3l4,1869
+get_eyedata-1.3.2.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+get_eyedata-1.3.2.dist-info/top_level.txt,sha256=zlueM7ZefajCSIgOyib56hk_6HWx15EsED6S68g0mWE,12
+get_eyedata-1.3.2.dist-info/RECORD,,
```

