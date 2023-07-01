# Comparing `tmp/streamlabsio-1.0.1.tar.gz` & `tmp/streamlabsio-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlabsio-1.0.1.tar", max compression
+gzip compressed data, was "streamlabsio-1.0.2.tar", max compression
```

## Comparing `streamlabsio-1.0.1.tar` & `streamlabsio-1.0.2.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0     1091 2022-11-13 08:19:22.113345 streamlabsio-1.0.1/LICENSE
--rw-r--r--   0        0        0      962 2023-06-28 03:28:40.778118 streamlabsio-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     2582 2023-06-28 02:39:37.040396 streamlabsio-1.0.1/README.md
--rw-r--r--   0        0        0       29 2023-06-27 16:58:43.358807 streamlabsio-1.0.1/streamlabsio/__init__.py
--rw-r--r--   0        0        0     3154 2023-06-28 03:28:10.049330 streamlabsio-1.0.1/streamlabsio/client.py
--rw-r--r--   0        0        0      104 2023-06-27 23:54:01.479898 streamlabsio-1.0.1/streamlabsio/error.py
--rw-r--r--   0        0        0      505 2023-06-27 20:27:01.395526 streamlabsio-1.0.1/streamlabsio/models.py
--rw-r--r--   0        0        0     3579 2023-06-28 03:29:09.498313 streamlabsio-1.0.1/setup.py
--rw-r--r--   0        0        0     3359 2023-06-28 03:29:09.499315 streamlabsio-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1091 2022-11-13 08:19:22.113345 streamlabsio-1.0.2/LICENSE
+-rw-r--r--   0        0        0      962 2023-07-01 22:06:00.271350 streamlabsio-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2599 2023-06-28 03:30:53.970102 streamlabsio-1.0.2/README.md
+-rw-r--r--   0        0        0       29 2023-06-27 16:58:43.358807 streamlabsio-1.0.2/streamlabsio/__init__.py
+-rw-r--r--   0        0        0     3226 2023-07-01 22:05:10.510362 streamlabsio-1.0.2/streamlabsio/client.py
+-rw-r--r--   0        0        0      104 2023-06-27 23:54:01.479898 streamlabsio-1.0.2/streamlabsio/error.py
+-rw-r--r--   0        0        0      505 2023-06-27 20:27:01.395526 streamlabsio-1.0.2/streamlabsio/models.py
+-rw-r--r--   0        0        0     3428 1970-01-01 00:00:00.000000 streamlabsio-1.0.2/PKG-INFO
```

### Comparing `streamlabsio-1.0.1/LICENSE` & `streamlabsio-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlabsio-1.0.1/pyproject.toml` & `streamlabsio-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "streamlabsio"
-version = "1.0.1"
+version = "1.0.2"
 description = "Get real time Twitch/Youtube events through Streamlabs SocketIO API"
 authors = ["onyx-and-iris <code@onyxandiris.online>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/onyx-and-iris/streamlabs-socketio-py"
 
 [tool.poetry.dependencies]
```

### Comparing `streamlabsio-1.0.1/README.md` & `streamlabsio-1.0.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -64,15 +64,15 @@
 
 ### Client class
 `streamlabsio.connect(token="<apikey>", raw=False)`
 
 The following keyword arguments may be passed:
 
 -   `token`: str   Streamlabs SocketIO api token.
--   `raw`: boolean=False    Receive raw json objects.
+-   `raw`: boolean=False    Receive raw data messages as json objects.
 
 ### Attributes
 
 For event data you may inspect the available attributes using `attrs()`.
 
 example:
```

### Comparing `streamlabsio-1.0.1/streamlabsio/client.py` & `streamlabsio-1.0.2/streamlabsio/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -67,20 +67,21 @@
     def connect_handler(self):
         self.logger.info("Connected to Streamlabs Socket API")
 
     def event_handler(self, data):
         if "for" in data and data["type"] in set(
             self.streamlabs + self.twitch + self.youtube
         ):
+            message = data["message"][0] if isinstance(data["message"][0], dict) else {}
             self.obs.trigger(
                 data["for"],
                 data["type"],
-                *data["message"]
+                message
                 if self._raw
-                else as_dataclass(data["type"], *data["message"]),
+                else as_dataclass(data["type"], message),
             )
             self.logger.debug(data)
 
     def disconnect_handler(self):
         self.logger.info("Disconnected from Streamlabs Socket API")
 
     def __exit__(self, exc_type, exc_val, exc_tb):
```

### Comparing `streamlabsio-1.0.1/PKG-INFO` & `streamlabsio-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: streamlabsio
-Version: 1.0.1
+Version: 1.0.2
 Summary: Get real time Twitch/Youtube events through Streamlabs SocketIO API
 Home-page: https://github.com/onyx-and-iris/streamlabs-socketio-py
 License: MIT
 Author: onyx-and-iris
 Author-email: code@onyxandiris.online
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: observable (>=1.0.3,<2.0.0)
 Requires-Dist: python-engineio (==3.14.2)
 Requires-Dist: python-socketio[client] (==4.6.0)
-Requires-Dist: tomli (>=2.0.1,<3.0.0); python_version < "3.11"
+Requires-Dist: tomli (>=2.0.1,<3.0.0) ; python_version < "3.11"
 Project-URL: Repository, https://github.com/onyx-and-iris/streamlabs-socketio-py
 Description-Content-Type: text/markdown
 
 [![PyPI version](https://badge.fury.io/py/streamlabsio.svg)](https://badge.fury.io/py/streamlabsio)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://github.com/onyx-and-iris/streamlabs-socketio-py/blob/dev/LICENSE)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
@@ -85,15 +86,15 @@
 
 ### Client class
 `streamlabsio.connect(token="<apikey>", raw=False)`
 
 The following keyword arguments may be passed:
 
 -   `token`: str   Streamlabs SocketIO api token.
--   `raw`: boolean=False    Receive raw json objects.
+-   `raw`: boolean=False    Receive raw data messages as json objects.
 
 ### Attributes
 
 For event data you may inspect the available attributes using `attrs()`.
 
 example:
```

