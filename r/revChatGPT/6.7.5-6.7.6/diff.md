# Comparing `tmp/revChatGPT-6.7.5.tar.gz` & `tmp/revChatGPT-6.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "revChatGPT-6.7.5.tar", last modified: Sat Jul  1 06:53:42 2023, max compression
+gzip compressed data, was "revChatGPT-6.7.6.tar", last modified: Sun Jul  2 09:36:31 2023, max compression
```

## Comparing `revChatGPT-6.7.5.tar` & `revChatGPT-6.7.6.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 06:53:42.763179 revChatGPT-6.7.5/
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-07-01 06:53:12.000000 revChatGPT-6.7.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7499 2023-07-01 06:53:42.763179 revChatGPT-6.7.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6356 2023-07-01 06:53:42.000000 revChatGPT-6.7.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-01 06:53:42.763179 revChatGPT-6.7.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-07-01 06:53:12.000000 revChatGPT-6.7.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 06:53:42.759179 revChatGPT-6.7.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 06:53:42.763179 revChatGPT-6.7.5/src/revChatGPT/
--rw-r--r--   0 runner    (1001) docker     (123)    60876 2023-07-01 06:53:12.000000 revChatGPT-6.7.5/src/revChatGPT/V1.py
--rw-r--r--   0 runner    (1001) docker     (123)    25039 2023-07-01 06:53:12.000000 revChatGPT-6.7.5/src/revChatGPT/V3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-07-01 06:53:12.000000 revChatGPT-6.7.5/src/revChatGPT/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-07-01 06:53:12.000000 revChatGPT-6.7.5/src/revChatGPT/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 06:53:42.763179 revChatGPT-6.7.5/src/revChatGPT/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-07-01 06:53:12.000000 revChatGPT-6.7.5/src/revChatGPT/config/enable_internet.json
--rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-07-01 06:53:12.000000 revChatGPT-6.7.5/src/revChatGPT/typings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-07-01 06:53:12.000000 revChatGPT-6.7.5/src/revChatGPT/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-01 06:53:12.000000 revChatGPT-6.7.5/src/revChatGPT/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 06:53:42.763179 revChatGPT-6.7.5/src/revChatGPT.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7499 2023-07-01 06:53:42.000000 revChatGPT-6.7.5/src/revChatGPT.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-07-01 06:53:42.000000 revChatGPT-6.7.5/src/revChatGPT.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 06:53:42.000000 revChatGPT-6.7.5/src/revChatGPT.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-01 06:53:42.000000 revChatGPT-6.7.5/src/revChatGPT.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-01 06:53:42.000000 revChatGPT-6.7.5/src/revChatGPT.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 06:53:42.763179 revChatGPT-6.7.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-01 06:53:12.000000 revChatGPT-6.7.5/tests/test_recipient.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:36:31.288034 revChatGPT-6.7.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-07-02 09:36:02.000000 revChatGPT-6.7.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7499 2023-07-02 09:36:31.288034 revChatGPT-6.7.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6356 2023-07-02 09:36:31.000000 revChatGPT-6.7.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-02 09:36:31.292034 revChatGPT-6.7.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-07-02 09:36:02.000000 revChatGPT-6.7.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:36:31.288034 revChatGPT-6.7.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:36:31.288034 revChatGPT-6.7.6/src/revChatGPT/
+-rw-r--r--   0 runner    (1001) docker     (123)    60775 2023-07-02 09:36:02.000000 revChatGPT-6.7.6/src/revChatGPT/V1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25039 2023-07-02 09:36:02.000000 revChatGPT-6.7.6/src/revChatGPT/V3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-07-02 09:36:02.000000 revChatGPT-6.7.6/src/revChatGPT/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-07-02 09:36:02.000000 revChatGPT-6.7.6/src/revChatGPT/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:36:31.288034 revChatGPT-6.7.6/src/revChatGPT/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-07-02 09:36:02.000000 revChatGPT-6.7.6/src/revChatGPT/config/enable_internet.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-07-02 09:36:02.000000 revChatGPT-6.7.6/src/revChatGPT/typings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-07-02 09:36:02.000000 revChatGPT-6.7.6/src/revChatGPT/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-02 09:36:02.000000 revChatGPT-6.7.6/src/revChatGPT/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:36:31.288034 revChatGPT-6.7.6/src/revChatGPT.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7499 2023-07-02 09:36:31.000000 revChatGPT-6.7.6/src/revChatGPT.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-07-02 09:36:31.000000 revChatGPT-6.7.6/src/revChatGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 09:36:31.000000 revChatGPT-6.7.6/src/revChatGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-02 09:36:31.000000 revChatGPT-6.7.6/src/revChatGPT.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-02 09:36:31.000000 revChatGPT-6.7.6/src/revChatGPT.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:36:31.288034 revChatGPT-6.7.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-02 09:36:02.000000 revChatGPT-6.7.6/tests/test_recipient.py
```

### Comparing `revChatGPT-6.7.5/LICENSE` & `revChatGPT-6.7.6/LICENSE`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.7.5/PKG-INFO` & `revChatGPT-6.7.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revChatGPT
-Version: 6.7.5
+Version: 6.7.6
 Summary: ChatGPT is a reverse engineering of OpenAI's ChatGPT API
 Home-page: https://github.com/acheong08/ChatGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=bug-report&template=bug_report.yml&title=%5BBug%5D%3A+
 Project-URL: Feature request, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=enhancement&template=feature_request.yml&title=%5BFeature+Request%5D%3A+
```

### Comparing `revChatGPT-6.7.5/README.md` & `revChatGPT-6.7.6/README.md`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.7.5/setup.py` & `revChatGPT-6.7.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,14 @@
         "httpx[socks]",
         "async_tio",
         "prompt-toolkit",
         "tiktoken>=0.3.0",
         "openai",
         "curl_cffi",
         "rich",
-        "tls_client>=0.2.1",
     ],
     classifiers=[
         "License :: OSI Approved :: GNU General Public License v2 (GPLv2)",
         "Intended Audience :: Developers",
         "Intended Audience :: End Users/Desktop",
         "Natural Language :: English",
         "Topic :: Software Development :: Libraries :: Python Modules",
```

### Comparing `revChatGPT-6.7.5/src/revChatGPT/V1.py` & `revChatGPT-6.7.6/src/revChatGPT/V1.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,14 @@
 import tempfile
 
 # Import function type
 from typing import Callable as function
 
 import httpx
 import requests
-import tls_client
 from httpx import AsyncClient
 from OpenAIAuth import Auth0 as Authenticator
 from rich.live import Live
 from rich.markdown import Markdown
 
 from . import __version__
 from . import typings as t
@@ -113,23 +112,18 @@
             return out
 
         return wrapper
 
     return decorator
 
 
-BASE_URL = environ.get("CHATGPT_BASE_URL") or "https://bypass.churchless.tech/"
+BASE_URL = environ.get("CHATGPT_BASE_URL", "https://bypass.churchless.tech/")
 
 bcolors = t.Colors()
 
-session = tls_client.Session(
-    client_identifier="firefox110",
-    random_tls_extension_order=True,
-)
-
 
 def captcha_solver(images: list[str], challenge_details: dict) -> int:
     # Create tempfile
     with tempfile.TemporaryDirectory() as tempdir:
         filenames: list[Path] = []
 
         for image in images:
@@ -152,52 +146,54 @@
         )
         print("Enter the index of the images that matches the captcha instructions:")
         index = int(input())
 
         return index
 
 
+CAPTCHA_URL = getenv("CAPTCHA_URL", "https://bypass.churchless.tech/captcha/")
+
+
 def get_arkose_token(
     download_images: bool = True,
     solver: function = captcha_solver,
 ) -> str:
     """
     The solver function should take in a list of images in base64 and a dict of challenge details
     and return the index of the image that matches the challenge details
 
     Challenge details:
         game_type: str - Audio or Image
         instructions: str - Instructions for the captcha
         URLs: list[str] - URLs of the images or audio files
     """
-    captcha_url = BASE_URL.replace("/api/", "") + "/captcha/"
-    resp = session.get(
-        (captcha_url + "start?download_images=true")
+    resp = requests.get(
+        (CAPTCHA_URL + "start?download_images=true")
         if download_images
-        else captcha_url + "start",
+        else CAPTCHA_URL + "start",
     )
     resp_json: dict = resp.json()
-    if resp_json.get("status") == "success":
+    if resp.status_code == 200:
         return resp_json.get("token")
     if resp.status_code != 511:
-        raise Exception(resp_json.get("error"))
+        raise Exception(resp_json.get("error", "Unknown error"))
 
     if resp_json.get("status") != "captcha":
         raise Exception("unknown error")
 
     challenge_details: dict = resp_json.get("session", {}).get("concise_challenge")
     if not challenge_details:
         raise Exception("missing details")
 
     images: list[str] = resp_json.get("images")
 
     index = solver(images, challenge_details)
 
-    resp = session.post(
-        captcha_url + "verify",
+    resp = requests.post(
+        CAPTCHA_URL + "verify",
         json={"session": resp_json.get("session"), "index": index},
     )
     if resp.status_code != 200:
         raise Exception("Failed to verify captcha")
     return resp_json.get("token")
```

### Comparing `revChatGPT-6.7.5/src/revChatGPT/V3.py` & `revChatGPT-6.7.6/src/revChatGPT/V3.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.7.5/src/revChatGPT/__init__.py` & `revChatGPT-6.7.6/src/revChatGPT/__init__.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.7.5/src/revChatGPT/__main__.py` & `revChatGPT-6.7.6/src/revChatGPT/__main__.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.7.5/src/revChatGPT/config/enable_internet.json` & `revChatGPT-6.7.6/src/revChatGPT/config/enable_internet.json`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.7.5/src/revChatGPT/typings.py` & `revChatGPT-6.7.6/src/revChatGPT/typings.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.7.5/src/revChatGPT/utils.py` & `revChatGPT-6.7.6/src/revChatGPT/utils.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.7.5/src/revChatGPT.egg-info/PKG-INFO` & `revChatGPT-6.7.6/src/revChatGPT.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revChatGPT
-Version: 6.7.5
+Version: 6.7.6
 Summary: ChatGPT is a reverse engineering of OpenAI's ChatGPT API
 Home-page: https://github.com/acheong08/ChatGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=bug-report&template=bug_report.yml&title=%5BBug%5D%3A+
 Project-URL: Feature request, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=enhancement&template=feature_request.yml&title=%5BFeature+Request%5D%3A+
```

### Comparing `revChatGPT-6.7.5/tests/test_recipient.py` & `revChatGPT-6.7.6/tests/test_recipient.py`

 * *Files identical despite different names*

