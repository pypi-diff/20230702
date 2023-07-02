# Comparing `tmp/radioplayer_dataclasses-0.4.0.tar.gz` & `tmp/radioplayer_dataclasses-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "radioplayer_dataclasses-0.4.0.tar", max compression
+gzip compressed data, was "radioplayer_dataclasses-0.5.0.tar", max compression
```

## Comparing `radioplayer_dataclasses-0.4.0.tar` & `radioplayer_dataclasses-0.5.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    34520 2023-06-16 08:15:31.300882 radioplayer_dataclasses-0.4.0/LICENSE
--rw-r--r--   0        0        0     3627 2023-06-16 08:15:31.300882 radioplayer_dataclasses-0.4.0/README.md
--rw-r--r--   0        0        0     2203 2023-06-16 08:15:55.336976 radioplayer_dataclasses-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     2351 2023-06-16 08:15:31.300882 radioplayer_dataclasses-0.4.0/radioplayer/dataclasses/__init__.py
--rw-r--r--   0        0        0    56147 2023-06-16 08:15:31.300882 radioplayer_dataclasses-0.4.0/radioplayer/dataclasses/dataclasses.py
--rw-r--r--   0        0        0        0 2023-06-16 08:15:31.300882 radioplayer_dataclasses-0.4.0/radioplayer/dataclasses/py.typed
--rw-r--r--   0        0        0     4498 1970-01-01 00:00:00.000000 radioplayer_dataclasses-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0    34520 2023-07-02 10:35:04.079011 radioplayer_dataclasses-0.5.0/LICENSE
+-rw-r--r--   0        0        0     3627 2023-07-02 10:35:04.079011 radioplayer_dataclasses-0.5.0/README.md
+-rw-r--r--   0        0        0     2203 2023-07-02 10:35:28.864344 radioplayer_dataclasses-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     2351 2023-07-02 10:35:04.079011 radioplayer_dataclasses-0.5.0/radioplayer/dataclasses/__init__.py
+-rw-r--r--   0        0        0    56457 2023-07-02 10:35:04.079011 radioplayer_dataclasses-0.5.0/radioplayer/dataclasses/dataclasses.py
+-rw-r--r--   0        0        0        0 2023-07-02 10:35:04.079011 radioplayer_dataclasses-0.5.0/radioplayer/dataclasses/py.typed
+-rw-r--r--   0        0        0     4498 1970-01-01 00:00:00.000000 radioplayer_dataclasses-0.5.0/PKG-INFO
```

### Comparing `radioplayer_dataclasses-0.4.0/LICENSE` & `radioplayer_dataclasses-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `radioplayer_dataclasses-0.4.0/README.md` & `radioplayer_dataclasses-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `radioplayer_dataclasses-0.4.0/pyproject.toml` & `radioplayer_dataclasses-0.5.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "radioplayer-dataclasses"
-version = "v0.4.0" # 0.0.0 placeholder is replaced on release
+version = "v0.5.0" # 0.0.0 placeholder is replaced on release
 description = "Python dataclasses for radioplayer generated from XSD"
 repository = "https://github.com/radiorabe/python-radioplayer-dataclasses"
 authors = ["RaBe IT-Reaktion <it@rabe.ch>"]
 license = "AGPL-3"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
```

### Comparing `radioplayer_dataclasses-0.4.0/radioplayer/dataclasses/__init__.py` & `radioplayer_dataclasses-0.5.0/radioplayer/dataclasses/__init__.py`

 * *Files identical despite different names*

### Comparing `radioplayer_dataclasses-0.4.0/radioplayer/dataclasses/dataclasses.py` & `radioplayer_dataclasses-0.5.0/radioplayer/dataclasses/dataclasses.py`

 * *Files 1% similar despite different names*

```diff
@@ -334,17 +334,18 @@
 
 @dataclass
 class SocialIdentifierType:
     class Meta:
         name = "socialIdentifierType"
         target_namespace = "http://www.radioplayer.co.uk/schemas/11/rpDataTypes"
 
-    type: Optional[str] = field(
+    type_value: Optional[str] = field(
         default=None,
         metadata={
+            "name": "type",
             "type": "Attribute",
             "required": True,
         }
     )
     uid: Optional[str] = field(
         default=None,
         metadata={
@@ -360,17 +361,18 @@
 
 @dataclass
 class Catype:
     class Meta:
         name = "CAType"
         target_namespace = "http://www.radioplayer.co.uk/schemas/11/epgDataTypes"
 
-    type: CatypeType = field(
+    type_value: CatypeType = field(
         default=CatypeType.NONE,
         metadata={
+            "name": "type",
             "type": "Attribute",
         }
     )
 
 
 @dataclass
 class EpgLanguageType:
@@ -429,17 +431,18 @@
         default=None,
         metadata={
             "name": "expiryTime",
             "type": "Attribute",
             "pattern": r"[^\-].+T[^\.]+",
         }
     )
-    type: Optional[str] = field(
+    type_value: Optional[str] = field(
         default=None,
         metadata={
+            "name": "type",
             "type": "Attribute",
         }
     )
     index: Optional[int] = field(
         default=None,
         metadata={
             "type": "Attribute",
@@ -493,17 +496,18 @@
 
 @dataclass
 class FrequencyType:
     class Meta:
         name = "frequencyType"
         target_namespace = "http://www.radioplayer.co.uk/schemas/11/epgSI"
 
-    type: FrequencyTypeType = field(
+    type_value: FrequencyTypeType = field(
         default=FrequencyTypeType.PRIMARY,
         metadata={
+            "name": "type",
             "type": "Attribute",
         }
     )
     k_hz: Optional[int] = field(
         default=None,
         metadata={
             "name": "kHz",
@@ -523,17 +527,18 @@
         metadata={
             "type": "Attribute",
             "required": True,
             "white_space": "collapse",
             "pattern": r"(([0-9a-fA-F]{2}\.[0-9a-fA-F]{4}\.)?[0-9a-fA-F]{4,8}\.[0-9a-fA-F]{1}(\.[0-9a-fA-F]{2})?)|([0-9a-fA-F]{6})",
         }
     )
-    type: ServiceIdTypeAttr = field(
+    type_value: ServiceIdTypeAttr = field(
         default=ServiceIdTypeAttr.PRIMARY,
         metadata={
+            "name": "type",
             "type": "Attribute",
         }
     )
 
 
 @dataclass
 class AlternateSourceType:
@@ -543,17 +548,18 @@
 
     protocol: AlternateSourceTypeProtocol = field(
         default=AlternateSourceTypeProtocol.URL,
         metadata={
             "type": "Attribute",
         }
     )
-    type: AlternateSourceTypeType = field(
+    type_value: AlternateSourceTypeType = field(
         default=AlternateSourceTypeType.IDENTICAL,
         metadata={
+            "name": "type",
             "type": "Attribute",
         }
     )
     url: Optional[str] = field(
         default=None,
         metadata={
             "type": "Attribute",
@@ -610,17 +616,18 @@
         metadata={
             "type": "Attribute",
             "required": True,
             "white_space": "collapse",
             "pattern": r":[^:]+:[^:]+",
         }
     )
-    type: GenreTypeType = field(
+    type_value: GenreTypeType = field(
         default=GenreTypeType.MAIN,
         metadata={
+            "name": "type",
             "type": "Attribute",
         }
     )
 
     @dataclass
     class Name(MessageType):
         preferred: Optional[bool] = field(
@@ -821,17 +828,18 @@
             default=None,
             metadata={
                 "type": "Attribute",
                 "white_space": "collapse",
                 "pattern": r"((crid|CRID|tel|mailto|postal|http|https|dab|drm):(//|\+|SMS=)?)?([a-zA-Z0-9]|\.|@|%|\-|/|_|\+|\?|=|;){1,}",
             }
         )
-        type: Optional[MultimediaType] = field(
+        type_value: Optional[MultimediaType] = field(
             default=None,
             metadata={
+                "name": "type",
                 "type": "Attribute",
             }
         )
         width: Optional[int] = field(
             default=None,
             metadata={
                 "type": "Attribute",
@@ -956,17 +964,18 @@
     )
     version: Optional[int] = field(
         default=None,
         metadata={
             "type": "Attribute",
         }
     )
-    type: Optional[ProgrammeGroupTypeType] = field(
+    type_value: Optional[ProgrammeGroupTypeType] = field(
         default=None,
         metadata={
+            "name": "type",
             "type": "Attribute",
         }
     )
     num_of_items: Optional[int] = field(
         default=None,
         metadata={
             "name": "numOfItems",
```

### Comparing `radioplayer_dataclasses-0.4.0/PKG-INFO` & `radioplayer_dataclasses-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: radioplayer-dataclasses
-Version: 0.4.0
+Version: 0.5.0
 Summary: Python dataclasses for radioplayer generated from XSD
 Home-page: https://github.com/radiorabe/python-radioplayer-dataclasses
 License: AGPL-3
 Author: RaBe IT-Reaktion
 Author-email: it@rabe.ch
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 3 - Alpha
```

