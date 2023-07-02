# Comparing `tmp/elevenlabslib-0.9.3.tar.gz` & `tmp/elevenlabslib-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elevenlabslib-0.9.3.tar", last modified: Thu Jun 15 21:32:39 2023, max compression
+gzip compressed data, was "elevenlabslib-0.9.4.tar", last modified: Tue Jun 27 16:01:23 2023, max compression
```

## Comparing `elevenlabslib-0.9.3.tar` & `elevenlabslib-0.9.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 21:32:39.780508 elevenlabslib-0.9.3/
--rw-rw-rw-   0        0        0     1091 2023-02-17 22:48:32.000000 elevenlabslib-0.9.3/LICENSE
--rw-rw-rw-   0        0        0     3379 2023-06-15 21:32:39.780508 elevenlabslib-0.9.3/PKG-INFO
--rw-rw-rw-   0        0        0     2724 2023-06-01 12:12:53.000000 elevenlabslib-0.9.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-15 21:32:39.775509 elevenlabslib-0.9.3/elevenlabslib/
--rw-rw-rw-   0        0        0     7678 2023-05-14 14:43:03.000000 elevenlabslib-0.9.3/elevenlabslib/ElevenLabsHistoryItem.py
--rw-rw-rw-   0        0        0     3025 2023-05-14 14:33:26.000000 elevenlabslib-0.9.3/elevenlabslib/ElevenLabsSample.py
--rw-rw-rw-   0        0        0    20932 2023-06-01 11:49:17.000000 elevenlabslib-0.9.3/elevenlabslib/ElevenLabsUser.py
--rw-rw-rw-   0        0        0    42069 2023-06-15 21:32:11.000000 elevenlabslib-0.9.3/elevenlabslib/ElevenLabsVoice.py
--rw-rw-rw-   0        0        0      585 2023-05-31 18:40:03.000000 elevenlabslib-0.9.3/elevenlabslib/__init__.py
--rw-rw-rw-   0        0        0     9039 2023-06-15 21:13:31.000000 elevenlabslib-0.9.3/elevenlabslib/helpers.py
-drwxrwxrwx   0        0        0        0 2023-06-15 21:32:39.779508 elevenlabslib-0.9.3/elevenlabslib.egg-info/
--rw-rw-rw-   0        0        0     3379 2023-06-15 21:32:39.000000 elevenlabslib-0.9.3/elevenlabslib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      405 2023-06-15 21:32:39.000000 elevenlabslib-0.9.3/elevenlabslib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 21:32:39.000000 elevenlabslib-0.9.3/elevenlabslib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-06-15 21:32:39.000000 elevenlabslib-0.9.3/elevenlabslib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-06-15 21:32:39.000000 elevenlabslib-0.9.3/elevenlabslib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      855 2023-06-15 21:19:01.000000 elevenlabslib-0.9.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-15 21:32:39.780508 elevenlabslib-0.9.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-27 16:01:23.859801 elevenlabslib-0.9.4/
+-rw-rw-rw-   0        0        0     1091 2023-02-17 22:48:32.000000 elevenlabslib-0.9.4/LICENSE
+-rw-rw-rw-   0        0        0     3379 2023-06-27 16:01:23.859801 elevenlabslib-0.9.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2724 2023-06-01 12:12:53.000000 elevenlabslib-0.9.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-27 16:01:23.852800 elevenlabslib-0.9.4/elevenlabslib/
+-rw-rw-rw-   0        0        0     7678 2023-05-14 14:43:03.000000 elevenlabslib-0.9.4/elevenlabslib/ElevenLabsHistoryItem.py
+-rw-rw-rw-   0        0        0     3025 2023-05-14 14:33:26.000000 elevenlabslib-0.9.4/elevenlabslib/ElevenLabsSample.py
+-rw-rw-rw-   0        0        0    20932 2023-06-01 11:49:17.000000 elevenlabslib-0.9.4/elevenlabslib/ElevenLabsUser.py
+-rw-rw-rw-   0        0        0    42069 2023-06-15 21:32:11.000000 elevenlabslib-0.9.4/elevenlabslib/ElevenLabsVoice.py
+-rw-rw-rw-   0        0        0      585 2023-05-31 18:40:03.000000 elevenlabslib-0.9.4/elevenlabslib/__init__.py
+-rw-rw-rw-   0        0        0     9105 2023-06-27 15:58:04.000000 elevenlabslib-0.9.4/elevenlabslib/helpers.py
+drwxrwxrwx   0        0        0        0 2023-06-27 16:01:23.858800 elevenlabslib-0.9.4/elevenlabslib.egg-info/
+-rw-rw-rw-   0        0        0     3379 2023-06-27 16:01:23.000000 elevenlabslib-0.9.4/elevenlabslib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      405 2023-06-27 16:01:23.000000 elevenlabslib-0.9.4/elevenlabslib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 16:01:23.000000 elevenlabslib-0.9.4/elevenlabslib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-06-27 16:01:23.000000 elevenlabslib-0.9.4/elevenlabslib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-06-27 16:01:23.000000 elevenlabslib-0.9.4/elevenlabslib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      855 2023-06-27 16:01:02.000000 elevenlabslib-0.9.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-27 16:01:23.859801 elevenlabslib-0.9.4/setup.cfg
```

### Comparing `elevenlabslib-0.9.3/LICENSE` & `elevenlabslib-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `elevenlabslib-0.9.3/PKG-INFO` & `elevenlabslib-0.9.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elevenlabslib
-Version: 0.9.3
+Version: 0.9.4
 Summary: Complete python wrapper for the elevenlabs API
 Author-email: lugia19 <lugia19@lugia19.com>
 Project-URL: Documentation, https://elevenlabslib.readthedocs.io/en/latest/
 Project-URL: Homepage, https://github.com/lugia19/elevenlabslib
 Project-URL: Bug Tracker, https://github.com/lugia19/elevenlabslib
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: elevenlabslib Version: 0.9.3 Summary: Complete
+Metadata-Version: 2.1 Name: elevenlabslib Version: 0.9.4 Summary: Complete
 python wrapper for the elevenlabs API Author-email: lugia19
 lugia19.com> Project-URL: Documentation, https://elevenlabslib.readthedocs.io/
 en/latest/ Project-URL: Homepage, https://github.com/lugia19/elevenlabslib
 Project-URL: Bug Tracker, https://github.com/lugia19/elevenlabslib Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Classifier: Development
 Status :: 4 - Beta Requires-Python: >=3.7 Description-Content-Type: text/
```

### Comparing `elevenlabslib-0.9.3/README.md` & `elevenlabslib-0.9.4/README.md`

 * *Files identical despite different names*

### Comparing `elevenlabslib-0.9.3/elevenlabslib/ElevenLabsHistoryItem.py` & `elevenlabslib-0.9.4/elevenlabslib/ElevenLabsHistoryItem.py`

 * *Files identical despite different names*

### Comparing `elevenlabslib-0.9.3/elevenlabslib/ElevenLabsSample.py` & `elevenlabslib-0.9.4/elevenlabslib/ElevenLabsSample.py`

 * *Files identical despite different names*

### Comparing `elevenlabslib-0.9.3/elevenlabslib/ElevenLabsUser.py` & `elevenlabslib-0.9.4/elevenlabslib/ElevenLabsUser.py`

 * *Files identical despite different names*

### Comparing `elevenlabslib-0.9.3/elevenlabslib/ElevenLabsVoice.py` & `elevenlabslib-0.9.4/elevenlabslib/ElevenLabsVoice.py`

 * *Files identical despite different names*

### Comparing `elevenlabslib-0.9.3/elevenlabslib/__init__.py` & `elevenlabslib-0.9.4/elevenlabslib/__init__.py`

 * *Files identical despite different names*

### Comparing `elevenlabslib-0.9.3/elevenlabslib/helpers.py` & `elevenlabslib-0.9.4/elevenlabslib/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,16 +67,18 @@
     if params is not None:
         args["params"] = params
 
     return _api_call_v2(requests.post, args)
 
 def _pretty_print_POST(res:requests.Response):
     req = res.request
-    logging.debug(f"RESPONSE DATA: {res.text}")
-    logging.debug('REQUEST THAT CAUSED THE ERROR:\n{}\n{}\r\n{}\r\n\r\n{}'.format(
+    import logging
+    logging.basicConfig(level=logging.DEBUG)
+    logging.error(f"RESPONSE DATA: {res.text}")
+    logging.error('REQUEST THAT CAUSED THE ERROR:\n{}\n{}\r\n{}\r\n\r\n{}'.format(
         '-----------START-----------',
         req.method + ' ' + req.url,
         '\r\n'.join('{}: {}'.format(k, v) for k, v in req.headers.items()),
         req.body,
     ))
```

### Comparing `elevenlabslib-0.9.3/elevenlabslib.egg-info/PKG-INFO` & `elevenlabslib-0.9.4/elevenlabslib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elevenlabslib
-Version: 0.9.3
+Version: 0.9.4
 Summary: Complete python wrapper for the elevenlabs API
 Author-email: lugia19 <lugia19@lugia19.com>
 Project-URL: Documentation, https://elevenlabslib.readthedocs.io/en/latest/
 Project-URL: Homepage, https://github.com/lugia19/elevenlabslib
 Project-URL: Bug Tracker, https://github.com/lugia19/elevenlabslib
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: elevenlabslib Version: 0.9.3 Summary: Complete
+Metadata-Version: 2.1 Name: elevenlabslib Version: 0.9.4 Summary: Complete
 python wrapper for the elevenlabs API Author-email: lugia19
 lugia19.com> Project-URL: Documentation, https://elevenlabslib.readthedocs.io/
 en/latest/ Project-URL: Homepage, https://github.com/lugia19/elevenlabslib
 Project-URL: Bug Tracker, https://github.com/lugia19/elevenlabslib Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Classifier: Development
 Status :: 4 - Beta Requires-Python: >=3.7 Description-Content-Type: text/
```

### Comparing `elevenlabslib-0.9.3/pyproject.toml` & `elevenlabslib-0.9.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0",
             "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "elevenlabslib"
-version = "0.9.3"
+version = "0.9.4"
 authors = [
   { name="lugia19", email="lugia19@lugia19.com" },
 ]
 description = "Complete python wrapper for the elevenlabs API"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies=[
```

