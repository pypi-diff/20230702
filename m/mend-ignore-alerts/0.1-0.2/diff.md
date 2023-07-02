# Comparing `tmp/mend_ignore_alerts-0.1-py3-none-any.whl.zip` & `tmp/mend_ignore_alerts-0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 11727 bytes, number of entries: 11
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-02 15:37 mend_ignore_alerts/__init__.py
--rw-r--r--  2.0 unx      105 b- defN 23-Jul-02 15:37 mend_ignore_alerts/_version.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-02 15:37 mend_ignore_alerts/conftest.py
--rw-r--r--  2.0 unx     1554 b- defN 23-Jul-02 15:37 mend_ignore_alerts/const.py
--rw-r--r--  2.0 unx    10552 b- defN 23-Jul-02 15:37 mend_ignore_alerts/ignore_alerts.py
--rw-r--r--  2.0 unx    11357 b- defN 23-Jul-02 15:37 mend_ignore_alerts-0.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     5213 b- defN 23-Jul-02 15:37 mend_ignore_alerts-0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-02 15:37 mend_ignore_alerts-0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       72 b- defN 23-Jul-02 15:37 mend_ignore_alerts-0.1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       19 b- defN 23-Jul-02 15:37 mend_ignore_alerts-0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      967 b- defN 23-Jul-02 15:37 mend_ignore_alerts-0.1.dist-info/RECORD
-11 files, 29931 bytes uncompressed, 10059 bytes compressed:  66.4%
+Zip file size: 11742 bytes, number of entries: 11
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-02 16:14 mend_ignore_alerts/__init__.py
+-rw-r--r--  2.0 unx      105 b- defN 23-Jul-02 16:14 mend_ignore_alerts/_version.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-02 16:14 mend_ignore_alerts/conftest.py
+-rw-r--r--  2.0 unx     1554 b- defN 23-Jul-02 16:14 mend_ignore_alerts/const.py
+-rw-r--r--  2.0 unx    10552 b- defN 23-Jul-02 16:14 mend_ignore_alerts/ignore_alerts.py
+-rw-r--r--  2.0 unx    11357 b- defN 23-Jul-02 16:14 mend_ignore_alerts-0.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     5248 b- defN 23-Jul-02 16:14 mend_ignore_alerts-0.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-02 16:14 mend_ignore_alerts-0.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       72 b- defN 23-Jul-02 16:14 mend_ignore_alerts-0.2.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       19 b- defN 23-Jul-02 16:14 mend_ignore_alerts-0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      967 b- defN 23-Jul-02 16:14 mend_ignore_alerts-0.2.dist-info/RECORD
+11 files, 29966 bytes uncompressed, 10074 bytes compressed:  66.4%
```

## zipnote {}

```diff
@@ -9,26 +9,26 @@
 
 Filename: mend_ignore_alerts/const.py
 Comment: 
 
 Filename: mend_ignore_alerts/ignore_alerts.py
 Comment: 
 
-Filename: mend_ignore_alerts-0.1.dist-info/LICENSE
+Filename: mend_ignore_alerts-0.2.dist-info/LICENSE
 Comment: 
 
-Filename: mend_ignore_alerts-0.1.dist-info/METADATA
+Filename: mend_ignore_alerts-0.2.dist-info/METADATA
 Comment: 
 
-Filename: mend_ignore_alerts-0.1.dist-info/WHEEL
+Filename: mend_ignore_alerts-0.2.dist-info/WHEEL
 Comment: 
 
-Filename: mend_ignore_alerts-0.1.dist-info/entry_points.txt
+Filename: mend_ignore_alerts-0.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: mend_ignore_alerts-0.1.dist-info/top_level.txt
+Filename: mend_ignore_alerts-0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: mend_ignore_alerts-0.1.dist-info/RECORD
+Filename: mend_ignore_alerts-0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mend_ignore_alerts/_version.py

```diff
@@ -1,3 +1,3 @@
-__version__ = "0.1"
+__version__ = "0.2"
 __tool_name__ = "ignore_alerts"
 __description__ = "Parse yml file and update alerts"
```

## Comparing `mend_ignore_alerts-0.1.dist-info/LICENSE` & `mend_ignore_alerts-0.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mend_ignore_alerts-0.1.dist-info/METADATA` & `mend_ignore_alerts-0.2.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mend-ignore-alerts
-Version: 0.1
+Version: 0.2
 Summary: Parse yml file and update alerts
 Home-page: https://github.com/mend-toolkit/ignore-alerts
 Author: Mend Professional Services
 Author-email: ps@mend.io
 License: LICENSE.txt
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -14,14 +14,15 @@
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: configparser (~=5.3.0)
 Requires-Dist: requests (~=2.31.0)
 Requires-Dist: setuptools (~=65.5.1)
 Requires-Dist: PyYAML (~=6.0)
+Requires-Dist: PyGithub (~=1.59.0)
 
 [![Logo](https://resources.mend.io/mend-sig/logo/mend-dark-logo-horizontal.png)](https://www.mend.io/)  
 
 [![License](https://img.shields.io/badge/License-Apache%202.0-yellowgreen.svg)](https://opensource.org/licenses/Apache-2.0)
 [![CI](https://github.com/whitesource-ps/mend-import-sbom/actions/workflows/ci.yml/badge.svg)](https://github.com/whitesource-ps/mend-import-sbom/actions/workflows/ci.yml/badge.svg)
 [![GitHub release](https://img.shields.io/github/v/release/whitesource-ps/ws-import-sbom)](https://github.com/whitesource-ps/ws-import-sbom/releases/latest)
```

## Comparing `mend_ignore_alerts-0.1.dist-info/RECORD` & `mend_ignore_alerts-0.2.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 mend_ignore_alerts/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-mend_ignore_alerts/_version.py,sha256=mOMz_-bbAR2WXcBmVxEwkM1P2FTxzjVOFwVIJYe4F9A,105
+mend_ignore_alerts/_version.py,sha256=BfHLlCJLU7j2RGjnRNlDvrZNY-eWXyCfYIRKoJMWkX8,105
 mend_ignore_alerts/conftest.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 mend_ignore_alerts/const.py,sha256=aRDadkUul_6NZB_LDIZTkGf5VkWTPqfnj6eap-1Y7As,1554
 mend_ignore_alerts/ignore_alerts.py,sha256=Tp4wLss1jaGEDbBWS4o3c4h7efuL54qw6Rx7aO82Wdc,10552
-mend_ignore_alerts-0.1.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-mend_ignore_alerts-0.1.dist-info/METADATA,sha256=At4s3EmvHJYXFbsPTrsxCzCwcglcS-fRs9upkNk2g6Y,5213
-mend_ignore_alerts-0.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-mend_ignore_alerts-0.1.dist-info/entry_points.txt,sha256=b_q3jF-WbTVm6sR0BrVXts8u1OhXtD1aM2IZ5CfWmpE,72
-mend_ignore_alerts-0.1.dist-info/top_level.txt,sha256=ookvTXlTz4JKFzjrBd6U6MmV6RzYs9C8B2E2vMscaZ8,19
-mend_ignore_alerts-0.1.dist-info/RECORD,,
+mend_ignore_alerts-0.2.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+mend_ignore_alerts-0.2.dist-info/METADATA,sha256=dTEfQ4J__-lZle80wI009ch7oqNQaQ6GZAKl66c7V5c,5248
+mend_ignore_alerts-0.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+mend_ignore_alerts-0.2.dist-info/entry_points.txt,sha256=b_q3jF-WbTVm6sR0BrVXts8u1OhXtD1aM2IZ5CfWmpE,72
+mend_ignore_alerts-0.2.dist-info/top_level.txt,sha256=ookvTXlTz4JKFzjrBd6U6MmV6RzYs9C8B2E2vMscaZ8,19
+mend_ignore_alerts-0.2.dist-info/RECORD,,
```

