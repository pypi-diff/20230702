# Comparing `tmp/srt_equalizer-0.1.4.tar.gz` & `tmp/srt_equalizer-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "srt_equalizer-0.1.4.tar", max compression
+gzip compressed data, was "srt_equalizer-0.1.5.tar", max compression
```

## Comparing `srt_equalizer-0.1.4.tar` & `srt_equalizer-0.1.5.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1069 2023-03-14 12:00:05.282587 srt_equalizer-0.1.4/LICENSE
--rw-r--r--   0        0        0     2688 2023-07-02 13:42:11.385032 srt_equalizer-0.1.4/README.md
--rw-r--r--   0        0        0      519 2023-07-02 13:46:44.045940 srt_equalizer-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      104 2023-04-01 12:40:07.008580 srt_equalizer-0.1.4/src/srt_equalizer/__init__.py
--rw-r--r--   0        0        0     3605 2023-04-02 12:51:15.799391 srt_equalizer-0.1.4/src/srt_equalizer/srt_equalizer.py
--rw-r--r--   0        0        0     3352 1970-01-01 00:00:00.000000 srt_equalizer-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-03-14 12:00:05.282587 srt_equalizer-0.1.5/LICENSE
+-rw-r--r--   0        0        0     2688 2023-07-02 13:42:11.385032 srt_equalizer-0.1.5/README.md
+-rw-r--r--   0        0        0      519 2023-07-02 15:17:34.795707 srt_equalizer-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      104 2023-04-01 12:40:07.008580 srt_equalizer-0.1.5/src/srt_equalizer/__init__.py
+-rw-r--r--   0        0        0     3605 2023-04-02 12:51:15.799391 srt_equalizer-0.1.5/src/srt_equalizer/srt_equalizer.py
+-rw-r--r--   0        0        0     3402 1970-01-01 00:00:00.000000 srt_equalizer-0.1.5/PKG-INFO
```

### Comparing `srt_equalizer-0.1.4/LICENSE` & `srt_equalizer-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `srt_equalizer-0.1.4/README.md` & `srt_equalizer-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `srt_equalizer-0.1.4/pyproject.toml` & `srt_equalizer-0.1.5/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [tool.poetry]
 name = "srt_equalizer"
-version = "0.1.3"
+version = "0.1.5"
 description = "Transform subtitle line lengths, splitting into multiple subtitle fragments if necessary. "
 authors = ["Peter Krantz"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/peterk/srt_equalizer"
 
 [tool.poetry.dependencies]
-python = "^3.9"
+python = "^3.8"
 srt = "^3.5.3"
 
 [tool.poetry.dev-dependencies]
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.2"
```

### Comparing `srt_equalizer-0.1.4/src/srt_equalizer/srt_equalizer.py` & `srt_equalizer-0.1.5/src/srt_equalizer/srt_equalizer.py`

 * *Files identical despite different names*

### Comparing `srt_equalizer-0.1.4/PKG-INFO` & `srt_equalizer-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: srt-equalizer
-Version: 0.1.4
+Version: 0.1.5
 Summary: Transform subtitle line lengths, splitting into multiple subtitle fragments if necessary. 
 Home-page: https://github.com/peterk/srt_equalizer
 License: MIT
 Author: Peter Krantz
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: srt (>=3.5.3,<4.0.0)
 Project-URL: Repository, https://github.com/peterk/srt_equalizer
 Description-Content-Type: text/markdown
```

