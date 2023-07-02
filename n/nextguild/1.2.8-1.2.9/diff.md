# Comparing `tmp/nextguild-1.2.8.tar.gz` & `tmp/nextguild-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nextguild-1.2.8.tar", last modified: Thu Jun 29 19:57:34 2023, max compression
+gzip compressed data, was "nextguild-1.2.9.tar", last modified: Sun Jul  2 18:14:06 2023, max compression
```

## Comparing `nextguild-1.2.8.tar` & `nextguild-1.2.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:57:34.595032 nextguild-1.2.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-29 19:57:22.000000 nextguild-1.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-06-29 19:57:34.595032 nextguild-1.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-06-29 19:57:22.000000 nextguild-1.2.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:57:34.595032 nextguild-1.2.8/nextguild/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-29 19:57:22.000000 nextguild-1.2.8/nextguild/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28062 2023-06-29 19:57:22.000000 nextguild-1.2.8/nextguild/classes.py
--rw-r--r--   0 runner    (1001) docker     (123)    43661 2023-06-29 19:57:22.000000 nextguild-1.2.8/nextguild/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3522 2023-06-29 19:57:22.000000 nextguild-1.2.8/nextguild/embed.py
--rw-r--r--   0 runner    (1001) docker     (123)    48087 2023-06-29 19:57:22.000000 nextguild-1.2.8/nextguild/events.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:57:34.595032 nextguild-1.2.8/nextguild.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-06-29 19:57:34.000000 nextguild-1.2.8/nextguild.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-29 19:57:34.000000 nextguild-1.2.8/nextguild.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 19:57:34.000000 nextguild-1.2.8/nextguild.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-29 19:57:34.000000 nextguild-1.2.8/nextguild.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-06-29 19:57:22.000000 nextguild-1.2.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 19:57:34.595032 nextguild-1.2.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 18:14:06.264037 nextguild-1.2.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-02 18:13:54.000000 nextguild-1.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-07-02 18:14:06.260037 nextguild-1.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-07-02 18:13:54.000000 nextguild-1.2.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 18:14:06.260037 nextguild-1.2.9/nextguild/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-02 18:13:54.000000 nextguild-1.2.9/nextguild/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28062 2023-07-02 18:13:54.000000 nextguild-1.2.9/nextguild/classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43673 2023-07-02 18:13:54.000000 nextguild-1.2.9/nextguild/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3522 2023-07-02 18:13:54.000000 nextguild-1.2.9/nextguild/embed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48087 2023-07-02 18:13:54.000000 nextguild-1.2.9/nextguild/events.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 18:14:06.260037 nextguild-1.2.9/nextguild.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-07-02 18:14:06.000000 nextguild-1.2.9/nextguild.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-02 18:14:06.000000 nextguild-1.2.9/nextguild.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 18:14:06.000000 nextguild-1.2.9/nextguild.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-02 18:14:06.000000 nextguild-1.2.9/nextguild.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-07-02 18:13:54.000000 nextguild-1.2.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 18:14:06.264037 nextguild-1.2.9/setup.cfg
```

### Comparing `nextguild-1.2.8/LICENSE` & `nextguild-1.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `nextguild-1.2.8/PKG-INFO` & `nextguild-1.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nextguild
-Version: 1.2.8
+Version: 1.2.9
 Summary: Interactions with the Guilded API made simpler
 Author-email: Arjun Sharda <sharda.aj17@gmail.com>, Erik Thorsell <contact@erikthorsell.com>
 License: MIT License
         
         Copyright (c) 2023 Arjun Sharda
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `nextguild-1.2.8/README.md` & `nextguild-1.2.9/README.md`

 * *Files identical despite different names*

### Comparing `nextguild-1.2.8/nextguild/classes.py` & `nextguild-1.2.9/nextguild/classes.py`

 * *Files identical despite different names*

### Comparing `nextguild-1.2.8/nextguild/client.py` & `nextguild-1.2.9/nextguild/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from datetime import datetime
 
 import requests
 
 from .classes import Data
 from .embed import Embed
 
-version = '1.2.8'
+version = '1.2.9'
 
 class Client:
     def __init__(self, token: str) -> None:
         self.token = token
         self.headers = {
             'Authorization': f'Bearer {self.token}',
             'User-Agent': f'NextGuild/{version}',
@@ -1494,15 +1494,15 @@
 
     def get_user_servers(self, user_id: str):
         response = self.request('GET', f'{self.base_url}users/{user_id}/servers')
         return response
 
     def get_bot_servers(self):
         response = self.request('GET', f'{self.base_url}/users/@me/servers')
-        return response
+        return response['servers']
 
     def get_default_channel(self, server_id: str):
         r = self.request('GET', f'{self.base_url}/servers/{server_id}')
         try:
             print(r)
             response = r['server']['defaultChannelId']
         except:
@@ -1573,8 +1573,8 @@
     def get_subscription_tier(self, server_id: str, subscription_type: str):
         r = self.request('GET', f'{self.base_url}/servers/{server_id}/subscriptions/tiers/{subscription_type}')
         return r
     
     def get_subscription_tiers(self, server_id: str):
         r = self.request('GET', f'{self.base_url}/servers/{server_id}/subscriptions/tiers')
         return r
- 
+
```

### Comparing `nextguild-1.2.8/nextguild/embed.py` & `nextguild-1.2.9/nextguild/embed.py`

 * *Files identical despite different names*

### Comparing `nextguild-1.2.8/nextguild/events.py` & `nextguild-1.2.9/nextguild/events.py`

 * *Files identical despite different names*

### Comparing `nextguild-1.2.8/nextguild.egg-info/PKG-INFO` & `nextguild-1.2.9/nextguild.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nextguild
-Version: 1.2.8
+Version: 1.2.9
 Summary: Interactions with the Guilded API made simpler
 Author-email: Arjun Sharda <sharda.aj17@gmail.com>, Erik Thorsell <contact@erikthorsell.com>
 License: MIT License
         
         Copyright (c) 2023 Arjun Sharda
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `nextguild-1.2.8/pyproject.toml` & `nextguild-1.2.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "requests", "asyncio", "websockets"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "nextguild"
-version = "1.2.8"
+version = "1.2.9"
 authors = [
     { name="Arjun Sharda", email="sharda.aj17@gmail.com" },
     { name="Erik Thorsell", email="contact@erikthorsell.com" },
 ]
 description = "Interactions with the Guilded API made simpler"
 readme = "README.md"
 license = { file="LICENSE" }
```

