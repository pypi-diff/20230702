# Comparing `tmp/NewFunctionsPYC-1.4.0b0.tar.gz` & `tmp/NewFunctionsPYC-1.4.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NewFunctionsPYC-1.4.0b0.tar", last modified: Sun Jul  2 01:35:35 2023, max compression
+gzip compressed data, was "NewFunctionsPYC-1.4.0b1.tar", last modified: Sun Jul  2 18:16:36 2023, max compression
```

## Comparing `NewFunctionsPYC-1.4.0b0.tar` & `NewFunctionsPYC-1.4.0b1.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-02 01:35:35.477888 NewFunctionsPYC-1.4.0b0/
-drwxrwxrwx   0        0        0        0 2023-07-02 01:35:35.462927 NewFunctionsPYC-1.4.0b0/NewFunctionsPYC/
--rw-rw-rw-   0        0        0     1028 2023-07-02 01:24:35.000000 NewFunctionsPYC-1.4.0b0/NewFunctionsPYC/__init__.py
--rw-rw-rw-   0        0        0     2746 2023-05-27 12:33:02.000000 NewFunctionsPYC-1.4.0b0/NewFunctionsPYC/checks.py
-drwxrwxrwx   0        0        0        0 2023-07-02 01:35:35.473898 NewFunctionsPYC-1.4.0b0/NewFunctionsPYC/commands/
--rw-rw-rw-   0        0        0     1353 2023-03-18 20:49:32.000000 NewFunctionsPYC-1.4.0b0/NewFunctionsPYC/commands/hybrid.py
--rw-rw-rw-   0        0        0     1300 2023-07-02 01:33:59.000000 NewFunctionsPYC-1.4.0b0/NewFunctionsPYC/commands/options.py
--rw-rw-rw-   0        0        0      858 2023-01-27 18:48:57.000000 NewFunctionsPYC-1.4.0b0/NewFunctionsPYC/commands/prefix.py
--rw-rw-rw-   0        0        0      809 2023-01-27 20:57:39.000000 NewFunctionsPYC-1.4.0b0/NewFunctionsPYC/commands/slash.py
--rw-rw-rw-   0        0        0     6259 2023-07-01 23:43:16.000000 NewFunctionsPYC-1.4.0b0/NewFunctionsPYC/embed.py
--rw-rw-rw-   0        0        0     4885 2023-07-02 01:31:30.000000 NewFunctionsPYC-1.4.0b0/NewFunctionsPYC/loader.py
-drwxrwxrwx   0        0        0        0 2023-07-02 01:35:35.468912 NewFunctionsPYC-1.4.0b0/NewFunctionsPYC.egg-info/
--rw-rw-rw-   0        0        0     1841 2023-07-02 01:35:35.000000 NewFunctionsPYC-1.4.0b0/NewFunctionsPYC.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      472 2023-07-02 01:35:35.000000 NewFunctionsPYC-1.4.0b0/NewFunctionsPYC.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-02 01:35:35.000000 NewFunctionsPYC-1.4.0b0/NewFunctionsPYC.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2023-07-02 01:35:35.000000 NewFunctionsPYC-1.4.0b0/NewFunctionsPYC.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-07-02 01:35:35.000000 NewFunctionsPYC-1.4.0b0/NewFunctionsPYC.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1841 2023-07-02 01:35:35.476891 NewFunctionsPYC-1.4.0b0/PKG-INFO
--rw-rw-rw-   0        0        0     1025 2023-01-24 21:24:03.000000 NewFunctionsPYC-1.4.0b0/README.md
--rw-rw-rw-   0        0        0     1009 2023-07-02 01:34:19.000000 NewFunctionsPYC-1.4.0b0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-02 01:35:35.477888 NewFunctionsPYC-1.4.0b0/setup.cfg
--rw-rw-rw-   0        0        0      142 2023-05-27 12:27:52.000000 NewFunctionsPYC-1.4.0b0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-02 18:16:36.951145 NewFunctionsPYC-1.4.0b1/
+drwxrwxrwx   0        0        0        0 2023-07-02 18:16:36.935187 NewFunctionsPYC-1.4.0b1/NewFunctionsPYC/
+-rw-rw-rw-   0        0        0     1028 2023-07-02 01:24:35.000000 NewFunctionsPYC-1.4.0b1/NewFunctionsPYC/__init__.py
+-rw-rw-rw-   0        0        0     2746 2023-05-27 12:33:02.000000 NewFunctionsPYC-1.4.0b1/NewFunctionsPYC/checks.py
+-rw-rw-rw-   0        0        0     1224 2023-07-02 17:33:28.000000 NewFunctionsPYC-1.4.0b1/NewFunctionsPYC/clientLogin.py
+drwxrwxrwx   0        0        0        0 2023-07-02 18:16:36.948177 NewFunctionsPYC-1.4.0b1/NewFunctionsPYC/commands/
+-rw-rw-rw-   0        0        0     1353 2023-03-18 20:49:32.000000 NewFunctionsPYC-1.4.0b1/NewFunctionsPYC/commands/hybrid.py
+-rw-rw-rw-   0        0        0     1284 2023-07-02 16:13:40.000000 NewFunctionsPYC-1.4.0b1/NewFunctionsPYC/commands/options.py
+-rw-rw-rw-   0        0        0      858 2023-01-27 18:48:57.000000 NewFunctionsPYC-1.4.0b1/NewFunctionsPYC/commands/prefix.py
+-rw-rw-rw-   0        0        0      809 2023-01-27 20:57:39.000000 NewFunctionsPYC-1.4.0b1/NewFunctionsPYC/commands/slash.py
+-rw-rw-rw-   0        0        0     6113 2023-07-02 18:11:46.000000 NewFunctionsPYC-1.4.0b1/NewFunctionsPYC/embed.py
+-rw-rw-rw-   0        0        0     4552 2023-07-02 18:14:00.000000 NewFunctionsPYC-1.4.0b1/NewFunctionsPYC/loader.py
+drwxrwxrwx   0        0        0        0 2023-07-02 18:16:36.942180 NewFunctionsPYC-1.4.0b1/NewFunctionsPYC.egg-info/
+-rw-rw-rw-   0        0        0     1841 2023-07-02 18:16:36.000000 NewFunctionsPYC-1.4.0b1/NewFunctionsPYC.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      503 2023-07-02 18:16:36.000000 NewFunctionsPYC-1.4.0b1/NewFunctionsPYC.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-02 18:16:36.000000 NewFunctionsPYC-1.4.0b1/NewFunctionsPYC.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2023-07-02 18:16:36.000000 NewFunctionsPYC-1.4.0b1/NewFunctionsPYC.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-07-02 18:16:36.000000 NewFunctionsPYC-1.4.0b1/NewFunctionsPYC.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1841 2023-07-02 18:16:36.950173 NewFunctionsPYC-1.4.0b1/PKG-INFO
+-rw-rw-rw-   0        0        0     1025 2023-01-24 21:24:03.000000 NewFunctionsPYC-1.4.0b1/README.md
+-rw-rw-rw-   0        0        0     1010 2023-07-02 18:15:57.000000 NewFunctionsPYC-1.4.0b1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-02 18:16:36.951145 NewFunctionsPYC-1.4.0b1/setup.cfg
+-rw-rw-rw-   0        0        0      130 2023-07-02 17:34:21.000000 NewFunctionsPYC-1.4.0b1/setup.py
```

### Comparing `NewFunctionsPYC-1.4.0b0/NewFunctionsPYC/__init__.py` & `NewFunctionsPYC-1.4.0b1/NewFunctionsPYC/__init__.py`

 * *Files identical despite different names*

### Comparing `NewFunctionsPYC-1.4.0b0/NewFunctionsPYC/checks.py` & `NewFunctionsPYC-1.4.0b1/NewFunctionsPYC/checks.py`

 * *Files identical despite different names*

### Comparing `NewFunctionsPYC-1.4.0b0/NewFunctionsPYC/commands/hybrid.py` & `NewFunctionsPYC-1.4.0b1/NewFunctionsPYC/commands/hybrid.py`

 * *Files identical despite different names*

### Comparing `NewFunctionsPYC-1.4.0b0/NewFunctionsPYC/commands/options.py` & `NewFunctionsPYC-1.4.0b1/NewFunctionsPYC/commands/options.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Any
 
 def Option(
         name: str, 
-        description: str = "Description not provided" , 
+        description: str = "Description not provided", 
         type: "OptionType" = None,
         choices: list["Choice"] = [],
         name_localizations: dict = {},
         description_localizations: dict = {}) -> dict:
     
     """A helper on how to create an option for the command"""
 
@@ -21,35 +21,35 @@
         "name_localizations": name_localizations,
         "description_localizations": description_localizations
     }
 
     return optionDict
 
 class OptionType:
+
     """Types for Options"""
 
     stringOption = 3
     intOption = 4
     boolOption = 5
     userOption = 6
     channelOption = 7
     roleOption = 8
-    attachmentOption= 11
+    attachmentOption = 11
 
 def Choice(
         name,
         name_localizations: dict = {},
         value: Any = None
         ) -> dict:
     """A helper on how to create a choice for the command"""
-    
-    choiceDict = {
-        "name": name,
-        "name_localizations": name_localizations
-    }
 
     if value is None:
         value = name
-    
-    choiceDict["value"] = value
+
+    choiceDict = {
+        "name": name,
+        "name_localizations": name_localizations,
+        "value": value
+    }
 
     return choiceDict
```

### Comparing `NewFunctionsPYC-1.4.0b0/NewFunctionsPYC/commands/prefix.py` & `NewFunctionsPYC-1.4.0b1/NewFunctionsPYC/commands/prefix.py`

 * *Files identical despite different names*

### Comparing `NewFunctionsPYC-1.4.0b0/NewFunctionsPYC/commands/slash.py` & `NewFunctionsPYC-1.4.0b1/NewFunctionsPYC/commands/slash.py`

 * *Files identical despite different names*

### Comparing `NewFunctionsPYC-1.4.0b0/NewFunctionsPYC/embed.py` & `NewFunctionsPYC-1.4.0b1/NewFunctionsPYC/embed.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 import discord
 import hexacolors
 
 class EmbedBuilder:
     """Embed contructor alike DiscordJs"""
 
-    def __init__(self) -> None:
-
-        self.settitle: str = ""
-        self.setdescription: str = ""
-        self.addfields: list = []
-        self.insertfield: list = []
-        self.removefield: list = []
-        self.clearfields: bool = False
-        self.setfooter: dict = {}
-        self.removefooter: bool = False
-        self.setauthor: dict = {}
-        self.removeauthor: bool = False
-        self.setimage: str = None
-        self.setthumb: str = None
-        self.removeimage: bool = False; self.removethumb: bool = False
-        self.setcolour: int = discord.Colour.dark_theme()
-        self.e: discord.Embed
+    settitle: str = ""
+    setdescription: str = ""
+    addfields: list = []
+    insertfield: list = []
+    removefield: list = []
+    clearfields: bool = False
+    setfooter: dict = {}
+    removefooter: bool = False
+    setauthor: dict = {}
+    removeauthor: bool = False
+    setimage: str = None
+    setthumb: str = None
+    removeimage: bool = False
+    removethumb: bool = False
+    setcolour: int = discord.Colour.dark_theme()
+    e: discord.Embed
 
     def set_title(self, title: str) -> str:
         self.settitle = str(title)
 
     def set_description(self, description: str) -> str:
         self.setdescription = str(description)
 
@@ -171,14 +170,16 @@
 
         if self.removethumb != False: 
             self.e.remove_thumbnail()
 
         if self.clearfields != False:
             self.e.clear_fields()
 
+        return self.e
+
     def detonarn(self):
         try:
             del self.e
         except AttributeError:
             pass
 
 class Colors:
```

### Comparing `NewFunctionsPYC-1.4.0b0/NewFunctionsPYC/loader.py` & `NewFunctionsPYC-1.4.0b1/NewFunctionsPYC/loader.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from os import listdir, getenv
 from discord.ext import bridge
 from discord import Intents, Game
 from dotenv import load_dotenv
+
+from NewFunctionsPYC.clientLogin import ClientAPI
 from .commands.options import Choice
-import requests
 
 def getTokenDotEnv():
     load_dotenv()
     token = getenv("token") or getenv("TOKEN")
 
     if token is None:
         raise Error("MISSING TOKEN")
@@ -49,33 +50,22 @@
             auto_sync_commands = auto_sync_commands,
             case_insensitive = case_insensitive,
             **options
         )
     
     async def on_ready(self):
 
-        for i in self.commandsREGISTER:
-            if i["guild_ids"] is None:
-                url = f"https://discord.com/api/v10/applications/{self.user.id}/commands"
-            else:
-                url = f"https://discord.com/api/v10/applications/{self.user.id}/guilds/{i['guild_id']}/commands"
-            
-            e = requests.post(
-                url=url,
-                json=i,
-                headers = {
-                    "Authorization": f"Bot {self.token}"
-                }
-            )
+        if self.commandsREGISTER.__len__() > 0:
 
-            if e.status_code == 201:
-                print(f"{i['name']} registered sucefully")
-            else:
-                print(f"Error registering {i['name']}")
-            
+            await ClientAPI().post(
+                "regSlashCommands",
+                token = self.token,
+                commandsREGISTER = self.commandsREGISTER,
+                botId = self.user.id
+            )
             
         if self.poweredby == True:
             await self.change_presence(activity=Game(name="PoweredBy PyCord and NewFunctionsPYC"))
             print("PoweredBy PyCord and NewFunctionsPYC")
 
     def upsertCommand(
             self,
@@ -83,33 +73,35 @@
             description: str = "Description not provided",
             nsfw: bool = False,
             options: list["Choice"] = [],
             guild_ids: list = None,
             name_localizations: dict = {},
             description_localizations: dict = {},
             guild_only: bool = None,
+            logRegister: bool = True
         ) -> any:
 
+        if guild_only is None:
+            guild_only = True
+        else:
+            guild_only = False
+
         dictCommand = {
             "type": 1,
             "name": name,
             "description": description,
             "nsfw": nsfw,
             "options": options,
             "guild_ids":guild_ids,
             "name_localizations": name_localizations,
-            "description_localizations": description_localizations
+            "description_localizations": description_localizations,
+            "dm_permission": guild_only,
+            "logRegister": logRegister
         }
 
-        if guild_only is None:
-            guild_only = True
-        else:
-            guild_only = False
-        dictCommand["dm_permission"] = guild_only
-
         self.commandsREGISTER.append(dictCommand)
 
     def load_cogs(self, folder: str):
 
         if folder.startswith("./") or folder.startswith("."):
             folder = folder.strip("./")
```

### Comparing `NewFunctionsPYC-1.4.0b0/NewFunctionsPYC.egg-info/PKG-INFO` & `NewFunctionsPYC-1.4.0b1/NewFunctionsPYC.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NewFunctionsPYC
-Version: 1.4.0b0
+Version: 1.4.0b1
 Summary: :A simple library for add new functions the Pycord
 Author: Marciel404
 License: MIT
 Project-URL: Homepage, https://github.com/Marciel404/NewFunctionsPYC
 Keywords: Pycord BetterFunctions
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
```

### Comparing `NewFunctionsPYC-1.4.0b0/PKG-INFO` & `NewFunctionsPYC-1.4.0b1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NewFunctionsPYC
-Version: 1.4.0b0
+Version: 1.4.0b1
 Summary: :A simple library for add new functions the Pycord
 Author: Marciel404
 License: MIT
 Project-URL: Homepage, https://github.com/Marciel404/NewFunctionsPYC
 Keywords: Pycord BetterFunctions
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
```

### Comparing `NewFunctionsPYC-1.4.0b0/README.md` & `NewFunctionsPYC-1.4.0b1/README.md`

 * *Files identical despite different names*

### Comparing `NewFunctionsPYC-1.4.0b0/pyproject.toml` & `NewFunctionsPYC-1.4.0b1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "NewFunctionsPYC"
-version = "1.4.0b"
+version = "1.4.0b1"
 keywords = ["Pycord BetterFunctions"]
 authors = [
     {name = "Marciel404"}
 ]
 description = """
 :A simple library for add new functions the Pycord
 """
```

