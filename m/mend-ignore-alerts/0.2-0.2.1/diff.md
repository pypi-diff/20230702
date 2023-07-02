# Comparing `tmp/mend_ignore_alerts-0.2-py3-none-any.whl.zip` & `tmp/mend_ignore_alerts-0.2.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 11742 bytes, number of entries: 11
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-02 16:14 mend_ignore_alerts/__init__.py
--rw-r--r--  2.0 unx      105 b- defN 23-Jul-02 16:14 mend_ignore_alerts/_version.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-02 16:14 mend_ignore_alerts/conftest.py
--rw-r--r--  2.0 unx     1554 b- defN 23-Jul-02 16:14 mend_ignore_alerts/const.py
--rw-r--r--  2.0 unx    10552 b- defN 23-Jul-02 16:14 mend_ignore_alerts/ignore_alerts.py
--rw-r--r--  2.0 unx    11357 b- defN 23-Jul-02 16:14 mend_ignore_alerts-0.2.dist-info/LICENSE
--rw-r--r--  2.0 unx     5248 b- defN 23-Jul-02 16:14 mend_ignore_alerts-0.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-02 16:14 mend_ignore_alerts-0.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       72 b- defN 23-Jul-02 16:14 mend_ignore_alerts-0.2.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       19 b- defN 23-Jul-02 16:14 mend_ignore_alerts-0.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      967 b- defN 23-Jul-02 16:14 mend_ignore_alerts-0.2.dist-info/RECORD
-11 files, 29966 bytes uncompressed, 10074 bytes compressed:  66.4%
+Zip file size: 11777 bytes, number of entries: 11
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-02 16:23 mend_ignore_alerts/__init__.py
+-rw-r--r--  2.0 unx      107 b- defN 23-Jul-02 16:23 mend_ignore_alerts/_version.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-02 16:23 mend_ignore_alerts/conftest.py
+-rw-r--r--  2.0 unx     1554 b- defN 23-Jul-02 16:23 mend_ignore_alerts/const.py
+-rw-r--r--  2.0 unx    10597 b- defN 23-Jul-02 16:23 mend_ignore_alerts/ignore_alerts.py
+-rw-r--r--  2.0 unx    11357 b- defN 23-Jul-02 16:23 mend_ignore_alerts-0.2.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     5250 b- defN 23-Jul-02 16:23 mend_ignore_alerts-0.2.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-02 16:23 mend_ignore_alerts-0.2.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       72 b- defN 23-Jul-02 16:23 mend_ignore_alerts-0.2.1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       19 b- defN 23-Jul-02 16:23 mend_ignore_alerts-0.2.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      979 b- defN 23-Jul-02 16:23 mend_ignore_alerts-0.2.1.dist-info/RECORD
+11 files, 30027 bytes uncompressed, 10085 bytes compressed:  66.4%
```

## zipnote {}

```diff
@@ -9,26 +9,26 @@
 
 Filename: mend_ignore_alerts/const.py
 Comment: 
 
 Filename: mend_ignore_alerts/ignore_alerts.py
 Comment: 
 
-Filename: mend_ignore_alerts-0.2.dist-info/LICENSE
+Filename: mend_ignore_alerts-0.2.1.dist-info/LICENSE
 Comment: 
 
-Filename: mend_ignore_alerts-0.2.dist-info/METADATA
+Filename: mend_ignore_alerts-0.2.1.dist-info/METADATA
 Comment: 
 
-Filename: mend_ignore_alerts-0.2.dist-info/WHEEL
+Filename: mend_ignore_alerts-0.2.1.dist-info/WHEEL
 Comment: 
 
-Filename: mend_ignore_alerts-0.2.dist-info/entry_points.txt
+Filename: mend_ignore_alerts-0.2.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: mend_ignore_alerts-0.2.dist-info/top_level.txt
+Filename: mend_ignore_alerts-0.2.1.dist-info/top_level.txt
 Comment: 
 
-Filename: mend_ignore_alerts-0.2.dist-info/RECORD
+Filename: mend_ignore_alerts-0.2.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mend_ignore_alerts/_version.py

```diff
@@ -1,3 +1,3 @@
-__version__ = "0.2"
+__version__ = "0.2.1"
 __tool_name__ = "ignore_alerts"
 __description__ = "Parse yml file and update alerts"
```

## mend_ignore_alerts/ignore_alerts.py

```diff
@@ -10,15 +10,18 @@
 from github import Github
 
 from mend_ignore_alerts._version import __version__, __tool_name__, __description__
 from mend_ignore_alerts.const import aliases, varenvs
 
 logger = logging.getLogger(__tool_name__)
 logger.setLevel(logging.DEBUG)
-is_debug = logging.DEBUG if os.environ.get("DEBUG").lower() == 'true' else logging.INFO
+try:
+    is_debug = logging.DEBUG if os.environ.get("DEBUG").lower() == 'true' else logging.INFO
+except:
+    is_debug = logging.INFO
 
 formatter = logging.Formatter('[%(asctime)s] %(levelname)5s %(message)s', "%Y-%m-%d %H:%M:%S")
 s_handler = logging.StreamHandler()
 s_handler.setFormatter(formatter)
 s_handler.setLevel(is_debug)
 logger.addHandler(s_handler)
 logger.propagate = False
```

## Comparing `mend_ignore_alerts-0.2.dist-info/LICENSE` & `mend_ignore_alerts-0.2.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mend_ignore_alerts-0.2.dist-info/METADATA` & `mend_ignore_alerts-0.2.1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mend-ignore-alerts
-Version: 0.2
+Version: 0.2.1
 Summary: Parse yml file and update alerts
 Home-page: https://github.com/mend-toolkit/ignore-alerts
 Author: Mend Professional Services
 Author-email: ps@mend.io
 License: LICENSE.txt
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

