# Comparing `tmp/krrsnkapi-0.5.tar.gz` & `tmp/krrsnkapi-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "krrsnkapi-0.5.tar", last modified: Tue Jun 20 20:56:29 2023, max compression
+gzip compressed data, was "krrsnkapi-0.6.tar", last modified: Sun Jul  2 17:46:00 2023, max compression
```

## Comparing `krrsnkapi-0.5.tar` & `krrsnkapi-0.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 20:56:29.210235 krrsnkapi-0.5/
--rw-rw-rw-   0        0        0     1087 2023-04-13 13:12:53.000000 krrsnkapi-0.5/LICENSE.txt
--rw-rw-rw-   0        0        0      617 2023-06-20 20:56:29.210235 krrsnkapi-0.5/PKG-INFO
--rw-rw-rw-   0        0        0     1569 2023-04-13 12:53:07.000000 krrsnkapi-0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-06-20 20:56:29.179035 krrsnkapi-0.5/krrsnkapi/
--rw-rw-rw-   0        0        0       52 2023-06-19 20:08:00.000000 krrsnkapi-0.5/krrsnkapi/__init__.py
--rw-rw-rw-   0        0        0     3086 2023-06-20 20:52:10.000000 krrsnkapi-0.5/krrsnkapi/krrsnkapi.py
-drwxrwxrwx   0        0        0        0 2023-06-20 20:56:29.194635 krrsnkapi-0.5/krrsnkapi.egg-info/
--rw-rw-rw-   0        0        0      617 2023-06-20 20:56:28.000000 krrsnkapi-0.5/krrsnkapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      249 2023-06-20 20:56:28.000000 krrsnkapi-0.5/krrsnkapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 20:56:28.000000 krrsnkapi-0.5/krrsnkapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-20 20:56:28.000000 krrsnkapi-0.5/krrsnkapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-20 20:56:28.000000 krrsnkapi-0.5/krrsnkapi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-06-20 20:56:29.210235 krrsnkapi-0.5/setup.cfg
--rw-rw-rw-   0        0        0     1445 2023-06-20 20:56:18.000000 krrsnkapi-0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-02 17:46:00.817140 krrsnkapi-0.6/
+-rw-rw-rw-   0        0        0     1087 2023-04-13 13:12:53.000000 krrsnkapi-0.6/LICENSE.txt
+-rw-rw-rw-   0        0        0      617 2023-07-02 17:46:00.818140 krrsnkapi-0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1569 2023-04-13 12:53:07.000000 krrsnkapi-0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-07-02 17:46:00.749136 krrsnkapi-0.6/krrsnkapi/
+-rw-rw-rw-   0        0        0       24 2023-07-02 17:24:18.000000 krrsnkapi-0.6/krrsnkapi/__init__.py
+-rw-rw-rw-   0        0        0     3246 2023-07-02 17:43:03.000000 krrsnkapi-0.6/krrsnkapi/krrsnkapi.py
+drwxrwxrwx   0        0        0        0 2023-07-02 17:46:00.815140 krrsnkapi-0.6/krrsnkapi.egg-info/
+-rw-rw-rw-   0        0        0      617 2023-07-02 17:45:58.000000 krrsnkapi-0.6/krrsnkapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      249 2023-07-02 17:45:59.000000 krrsnkapi-0.6/krrsnkapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-02 17:45:58.000000 krrsnkapi-0.6/krrsnkapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-02 17:45:58.000000 krrsnkapi-0.6/krrsnkapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-02 17:45:58.000000 krrsnkapi-0.6/krrsnkapi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-07-02 17:46:00.820140 krrsnkapi-0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1445 2023-07-02 17:45:24.000000 krrsnkapi-0.6/setup.py
```

### Comparing `krrsnkapi-0.5/LICENSE.txt` & `krrsnkapi-0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `krrsnkapi-0.5/PKG-INFO` & `krrsnkapi-0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: krrsnkapi
-Version: 0.5
+Version: 0.6
 Summary: Module for easy use of my api | info on GitHub: https://github.com/kararasenok-gd/krrsnkapi
 Home-page: https://github.com/kararasenok-gd/krrsnkapi
-Download-URL: https://github.com/kararasenok-gd/krrsnkapi/archive/v0.5.tar.gz
+Download-URL: https://github.com/kararasenok-gd/krrsnkapi/archive/v0.6.tar.gz
 Author: kararasenok_gd
 Author-email: murzikkurzikpro@gmail.com
 License: MIT
 Keywords: api
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `krrsnkapi-0.5/README.md` & `krrsnkapi-0.6/README.md`

 * *Files identical despite different names*

### Comparing `krrsnkapi-0.5/krrsnkapi/krrsnkapi.py` & `krrsnkapi-0.6/krrsnkapi/krrsnkapi.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,100 +1,97 @@
 import requests
 import json
 import random
 
+class apikeyError(Exception):
+	pass
+
+
 class Chat:
 	def __init__(self, apikey):
 		self.apikey = apikey
 
 	def send_message(self, message):
 		self.message = message
 
 		url = f'https://kararasenok.ueuo.com/api/v1/addchatmessage/?message={self.message}&apikey={self.apikey}'
 
 		self.response = requests.post(url)
-	
+		
 
 		self.status = self.response.text
 
+		if self.response.text == "KEY_NOT_FOUND":
+			raise apikeyError("The key you entered is incorrect!")
+
 		return self.status
 
 	def get_last_message_info(self, wReturn):
 		self.wReturn = wReturn
 
 		url = f'https://kararasenok.ueuo.com/api/v1/getlastmessageinfo/?apikey={self.apikey}&return={self.wReturn}'
 
 		self.response = requests.post(url)
-	
+		
 
 		self.status = self.response.text
 
+		if self.response.text == "KEY_NOT_FOUND":
+			raise apikeyError("The key you entered is incorrect!")
+
 		return self.status
 
 	def get_message_by_id(self, msgid, returnMessage = "0"):
 		self.msgid = msgid
 		self.returnMessage = returnMessage
 
 		url = f'https://kararasenok.ueuo.com/api/v1/getmessagebyid/?apikey={self.apikey}&id={self.msgid}&returnMessage={self.returnMessage}'
 
 		self.response = requests.post(url)
-	
+		
 
 		self.status = self.response.text
 
+		if self.response.text == "KEY_NOT_FOUND":
+			raise apikeyError("The key you entered is incorrect!")
+
 		return self.status
 
 	def get_message_info_by_id(self, msgid, wReturn):
 		self.msgid = msgid
 		self.wReturn = wReturn
 
 		url = f'https://kararasenok.ueuo.com/api/v1/getmessageinfobyid/?apikey={self.apikey}&id={self.msgid}&return={self.wReturn}'
 
 		self.response = requests.post(url)
-	
+		
 
 		self.status = self.response.text
 
-		return self.status
-
-class Base64:
-		def __init__(self, apikey):
-			self.apikey = apikey
-
-		def decode(self, text):
-			self.text = text
-
-			url = f'https://kararasenok.ueuo.com/api/v1/base64/decode/?text={self.text}&apikey={self.apikey}'
-
-			self.response = requests.post(url)
+		if self.response.text == "KEY_NOT_FOUND":
+			raise apikeyError("The key you entered is incorrect!")
 
-			return self.response.text
-
-		def encode(self, text):
-			self.text = text
-
-			url = f'https://kararasenok.ueuo.com/api/v1/base64/encode/?text={self.text}&apikey={self.apikey}'
-
-			self.response = requests.post(url)
-
-			return self.response.text
+		return self.status
 
 class PHPsandbox:
 	def __init__(self, apikey):
-		self.apikey = apikey
+			self.apikey = apikey
 
 	def create_code(self, code):
 		self.code = code
 
 		self.code = self.code.replace("\n", " ")
 
 		url = f'https://kararasenok.ueuo.com/api/v1/runphpscript/?apikey={self.apikey}&code={self.code}'
 
 		self.response = requests.post(url)
 
+		if self.response.text == "KEY_NOT_FOUND":
+			raise apikeyError("The key you entered is incorrect!")
+
 		return self.response.text
 
 class r34:
 	def __init__(self, apikey):
 		self.apikey = apikey
 
 	def get_url(self, keyword, page = 0, use_r34_api = False):
@@ -103,19 +100,24 @@
 		self.use_r34_api = use_r34_api
 
 		if self.use_r34_api is False:
 			self.response = requests.post(f"https://kararasenok.ueuo.com/api/v1/r34/?keyword={self.keyword}&apikey={self.apikey}&page={self.page}")
 		else:
 			self.response = requests.post(f"https://api.rule34.xxx/index.php?page=dapi&s=post&q=index&tags={self.keyword}&pid={self.page}&json=1&limit=1000")
 
+		if self.response.text == "KEY_NOT_FOUND":
+			raise apikeyError("The key you entered is incorrect!")
+
 		return self.response.text
 
 	def get_img_link(self, json_data):
 		self.json_data = json_data
 
 		self.data = json.loads(self.json_data)
 
 		self.random_object = random.choice(self.data)
 
 		self.random_fileurl = self.random_object['file_url']
 
 		return self.random_fileurl
+
+
```

### Comparing `krrsnkapi-0.5/krrsnkapi.egg-info/PKG-INFO` & `krrsnkapi-0.6/krrsnkapi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: krrsnkapi
-Version: 0.5
+Version: 0.6
 Summary: Module for easy use of my api | info on GitHub: https://github.com/kararasenok-gd/krrsnkapi
 Home-page: https://github.com/kararasenok-gd/krrsnkapi
-Download-URL: https://github.com/kararasenok-gd/krrsnkapi/archive/v0.5.tar.gz
+Download-URL: https://github.com/kararasenok-gd/krrsnkapi/archive/v0.6.tar.gz
 Author: kararasenok_gd
 Author-email: murzikkurzikpro@gmail.com
 License: MIT
 Keywords: api
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `krrsnkapi-0.5/setup.py` & `krrsnkapi-0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from setuptools import setup
 
 # ver = input("version: ")
 
 setup(
   name = 'krrsnkapi',         # How you named your package folder (MyLib)
   packages = ['krrsnkapi'],   # Chose the same as "name"
-  version = "0.5",      # Start with a small number and increase it with every change you make
+  version = "0.6",      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'Module for easy use of my api | info on GitHub: https://github.com/kararasenok-gd/krrsnkapi',   # Give a short description about your library
   author = 'kararasenok_gd',                   # Type in your name
   author_email = 'murzikkurzikpro@gmail.com',      # Type in your E-Mail
   url = 'https://github.com/kararasenok-gd/krrsnkapi',   # Provide either the link to your github or to your website
-  download_url = f'https://github.com/kararasenok-gd/krrsnkapi/archive/v0.5.tar.gz',    # I explain this later on
+  download_url = f'https://github.com/kararasenok-gd/krrsnkapi/archive/v0.6.tar.gz',    # I explain this later on
   keywords = ["api"],   # Keywords that define your package best
   install_requires=[            # I get to this in a second
           'requests'
       ],
   classifiers=[
     'Development Status :: 4 - Beta',      # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
     'Topic :: Software Development :: Build Tools',
```

