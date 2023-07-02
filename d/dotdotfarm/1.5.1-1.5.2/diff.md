# Comparing `tmp/dotdotfarm-1.5.1.tar.gz` & `tmp/dotdotfarm-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dotdotfarm-1.5.1.tar", last modified: Sat Jul  1 20:53:05 2023, max compression
+gzip compressed data, was "dotdotfarm-1.5.2.tar", last modified: Sun Jul  2 21:25:37 2023, max compression
```

## Comparing `dotdotfarm-1.5.1.tar` & `dotdotfarm-1.5.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-07-01 20:53:05.065767 dotdotfarm-1.5.1/
--rw-rw-rw-   0        0        0    35810 2023-01-16 18:50:58.000000 dotdotfarm-1.5.1/LICENSE
--rw-rw-rw-   0        0        0      154 2023-07-01 20:53:05.064793 dotdotfarm-1.5.1/PKG-INFO
--rw-rw-rw-   0        0        0     6935 2023-07-01 20:49:06.000000 dotdotfarm-1.5.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-01 20:53:05.046638 dotdotfarm-1.5.1/dotdotfarm/
--rw-rw-rw-   0        0        0        0 2023-01-22 10:12:14.000000 dotdotfarm-1.5.1/dotdotfarm/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-01 20:53:05.059291 dotdotfarm-1.5.1/dotdotfarm/callbacks/
--rw-rw-rw-   0        0        0      139 2023-03-09 19:14:53.000000 dotdotfarm-1.5.1/dotdotfarm/callbacks/__init__.py
--rw-rw-rw-   0        0        0     3178 2023-04-16 15:43:33.000000 dotdotfarm-1.5.1/dotdotfarm/callbacks/callbacks.py
--rw-rw-rw-   0        0        0      318 2023-03-07 20:07:03.000000 dotdotfarm-1.5.1/dotdotfarm/callbacks/cobject.py
--rw-rw-rw-   0        0        0     6222 2023-07-01 20:53:05.000000 dotdotfarm-1.5.1/dotdotfarm/dotdotweb.py
-drwxrwxrwx   0        0        0        0 2023-07-01 20:53:05.062339 dotdotfarm-1.5.1/dotdotfarm/engines/
--rw-rw-rw-   0        0        0        0 2023-01-17 19:46:18.000000 dotdotfarm-1.5.1/dotdotfarm/engines/__init__.py
--rw-rw-rw-   0        0        0     4120 2023-03-18 11:52:04.000000 dotdotfarm-1.5.1/dotdotfarm/engines/http_engine.py
--rw-rw-rw-   0        0        0        0 2023-05-01 19:28:12.000000 dotdotfarm-1.5.1/dotdotfarm/engines/websock_engine.py
-drwxrwxrwx   0        0        0        0 2023-07-01 20:53:05.064793 dotdotfarm-1.5.1/dotdotfarm/generators/
--rw-rw-rw-   0        0        0       81 2023-01-17 19:46:18.000000 dotdotfarm-1.5.1/dotdotfarm/generators/__init__.py
--rw-rw-rw-   0        0        0     2543 2023-03-18 12:06:54.000000 dotdotfarm-1.5.1/dotdotfarm/generators/words_generator.py
-drwxrwxrwx   0        0        0        0 2023-07-01 20:53:05.056371 dotdotfarm-1.5.1/dotdotfarm.egg-info/
--rw-rw-rw-   0        0        0      154 2023-07-01 20:53:05.000000 dotdotfarm-1.5.1/dotdotfarm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      555 2023-07-01 20:53:05.000000 dotdotfarm-1.5.1/dotdotfarm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-01 20:53:05.000000 dotdotfarm-1.5.1/dotdotfarm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2023-07-01 20:53:05.000000 dotdotfarm-1.5.1/dotdotfarm.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      156 2023-07-01 20:53:05.000000 dotdotfarm-1.5.1/dotdotfarm.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-01 20:53:05.000000 dotdotfarm-1.5.1/dotdotfarm.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-01 20:53:05.065767 dotdotfarm-1.5.1/setup.cfg
--rw-rw-rw-   0        0        0     1459 2023-07-01 20:52:54.000000 dotdotfarm-1.5.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-02 21:25:37.020761 dotdotfarm-1.5.2/
+-rw-rw-rw-   0        0        0    35810 2023-01-16 18:50:58.000000 dotdotfarm-1.5.2/LICENSE
+-rw-rw-rw-   0        0        0      154 2023-07-02 21:25:37.020761 dotdotfarm-1.5.2/PKG-INFO
+-rw-rw-rw-   0        0        0     6936 2023-07-02 21:22:50.000000 dotdotfarm-1.5.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-02 21:25:37.005137 dotdotfarm-1.5.2/dotdotfarm/
+-rw-rw-rw-   0        0        0        0 2023-01-22 10:12:14.000000 dotdotfarm-1.5.2/dotdotfarm/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-02 21:25:37.005137 dotdotfarm-1.5.2/dotdotfarm/callbacks/
+-rw-rw-rw-   0        0        0      139 2023-03-09 19:14:53.000000 dotdotfarm-1.5.2/dotdotfarm/callbacks/__init__.py
+-rw-rw-rw-   0        0        0     3178 2023-04-16 15:43:33.000000 dotdotfarm-1.5.2/dotdotfarm/callbacks/callbacks.py
+-rw-rw-rw-   0        0        0      318 2023-03-07 20:07:03.000000 dotdotfarm-1.5.2/dotdotfarm/callbacks/cobject.py
+-rw-rw-rw-   0        0        0     6222 2023-07-02 21:25:36.000000 dotdotfarm-1.5.2/dotdotfarm/dotdotweb.py
+drwxrwxrwx   0        0        0        0 2023-07-02 21:25:37.005137 dotdotfarm-1.5.2/dotdotfarm/engines/
+-rw-rw-rw-   0        0        0        0 2023-01-17 19:46:18.000000 dotdotfarm-1.5.2/dotdotfarm/engines/__init__.py
+-rw-rw-rw-   0        0        0     4433 2023-07-02 21:25:19.000000 dotdotfarm-1.5.2/dotdotfarm/engines/http_engine.py
+-rw-rw-rw-   0        0        0        0 2023-05-01 19:28:12.000000 dotdotfarm-1.5.2/dotdotfarm/engines/websock_engine.py
+drwxrwxrwx   0        0        0        0 2023-07-02 21:25:37.020761 dotdotfarm-1.5.2/dotdotfarm/generators/
+-rw-rw-rw-   0        0        0       81 2023-01-17 19:46:18.000000 dotdotfarm-1.5.2/dotdotfarm/generators/__init__.py
+-rw-rw-rw-   0        0        0     2543 2023-03-18 12:06:54.000000 dotdotfarm-1.5.2/dotdotfarm/generators/words_generator.py
+drwxrwxrwx   0        0        0        0 2023-07-02 21:25:37.005137 dotdotfarm-1.5.2/dotdotfarm.egg-info/
+-rw-rw-rw-   0        0        0      154 2023-07-02 21:25:36.000000 dotdotfarm-1.5.2/dotdotfarm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      555 2023-07-02 21:25:36.000000 dotdotfarm-1.5.2/dotdotfarm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-02 21:25:36.000000 dotdotfarm-1.5.2/dotdotfarm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2023-07-02 21:25:36.000000 dotdotfarm-1.5.2/dotdotfarm.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      156 2023-07-02 21:25:36.000000 dotdotfarm-1.5.2/dotdotfarm.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-02 21:25:36.000000 dotdotfarm-1.5.2/dotdotfarm.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-02 21:25:37.020761 dotdotfarm-1.5.2/setup.cfg
+-rw-rw-rw-   0        0        0     1590 2023-07-02 21:22:50.000000 dotdotfarm-1.5.2/setup.py
```

### Comparing `dotdotfarm-1.5.1/LICENSE` & `dotdotfarm-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dotdotfarm-1.5.1/README.md` & `dotdotfarm-1.5.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 dotdotfarm
 ==========
 
-![Version](https://img.shields.io/badge/version-1.5.1-blue?style=for-the-badge)
+![Version](https://img.shields.io/badge/version-1.5.2-blue?style=for-the-badge)
 
 Utility for detection & exploitation of Path Traversal vulnerabilities in various network services
 
 dotdotweb - PT tool for HTTP services
 
 
 Tools are written in Python with using asyncio requests (aiohttp) with some acceleration techniques, which allows you to make up to ~3K requests per second
@@ -17,27 +17,27 @@
 - specifying payload in any part of query (url, headers or POST data)
 - using callbacks for future handling of results
 
 Installation
 ============
 Install from PyPi
 ```bash
-pip install dotdotweb
+pip install dotdotfarm
 ```
 You can also install it directly from GitHub repository
 ```bash
 git clone https://github.com/treddis/dotdotfarm.git
 cd dotdotfarm
 pip install -r requirements.txt
 pip3 install .
 ```
 
 Usage
 =====
-```bash
+```text
 
     .___      __      .___      __    _____                      
   __| _/_____/  |_  __| _/_____/  |__/ ____\____ _______  _____  
  / __ |/  _ \   __\/ __ |/  _ \   __\   __\\__  \\_  __ \/     \ 
 / /_/ (  <_> )  | / /_/ (  <_> )  |  |  |   / __ \|  | \/  Y Y  \
 \____ |\____/|__| \____ |\____/|__|  |__|  (____  /__|  |__|_|  /
      \/                \/                       \/            \/
```

### Comparing `dotdotfarm-1.5.1/dotdotfarm/callbacks/callbacks.py` & `dotdotfarm-1.5.2/dotdotfarm/callbacks/callbacks.py`

 * *Files identical despite different names*

### Comparing `dotdotfarm-1.5.1/dotdotfarm/dotdotweb.py` & `dotdotfarm-1.5.2/dotdotfarm/dotdotweb.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from colorama import init, Fore, Style
 init()
 
 from dotdotfarm.generators.words_generator import Generator
 from dotdotfarm.engines.http_engine import HTTPEngine
 from dotdotfarm.callbacks.callbacks import print_http_result, add_file, validate_file
 
-__version__ = "1.5.1"
+__version__ = '1.5.2'
 
 argparse_list = partial(str.split, sep=',')
 
 async def factory(engine):
     try:
         task = asyncio.create_task(engine.run())
         await task
```

### Comparing `dotdotfarm-1.5.1/dotdotfarm/engines/http_engine.py` & `dotdotfarm-1.5.2/dotdotfarm/engines/http_engine.py`

 * *Files 10% similar despite different names*

```diff
@@ -50,14 +50,24 @@
 			raise ValueError
 
 	async def run(self):
 		try:
 			async with aiohttp.ClientSession(
 					connector=aiohttp.TCPConnector(limit=self.limit),
 					timeout=aiohttp.ClientTimeout(sock_connect=self.timeout)) as session:
+
+				# Check if server is available
+				try:
+					async with session.get(self.url) as response:
+						pass
+				except aiohttp.client_exceptions.ClientConnectorError as e:
+					print(f'[{Fore.RED}-{Style.RESET_ALL}] Connection error: {e.strerror}')
+					await aiohttp.TCPConnector().close()
+					return
+
 				for payload in self.payloads:
 					if payload.type_ == 'url':
 						self.tasks.append(
 							asyncio.create_task(
 								self.request(
 									session, 'GET', payload.fuzzed,
 									headers=self.headers,
```

### Comparing `dotdotfarm-1.5.1/dotdotfarm/generators/words_generator.py` & `dotdotfarm-1.5.2/dotdotfarm/generators/words_generator.py`

 * *Files identical despite different names*

### Comparing `dotdotfarm-1.5.1/dotdotfarm.egg-info/SOURCES.txt` & `dotdotfarm-1.5.2/dotdotfarm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dotdotfarm-1.5.1/setup.py` & `dotdotfarm-1.5.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 #!/usr/bin/env python3
 # ! -*- coding: utf-8 -*-
 
 import os
 import shutil
 from setuptools import setup, find_packages
 
-__version__ = '1.5.1'
+from pathlib import Path
+this_directory = Path(__file__).parent
+long_description = (this_directory / "README.md").read_text()
+
+__version__ = '1.5.2'
 install_requires = [
     "aiohttp==3.8.4",
     "colorama==0.4.6",
     "setuptools==66.1.1",
     "tqdm==4.64.1",
     "yarl==1.8.2",
     "multidict==6.0.4",
```

