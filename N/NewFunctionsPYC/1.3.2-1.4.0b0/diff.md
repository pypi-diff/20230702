# Comparing `tmp/NewFunctionsPYC-1.3.2.tar.gz` & `tmp/NewFunctionsPYC-1.4.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NewFunctionsPYC-1.3.2.tar", last modified: Tue Mar 21 21:22:42 2023, max compression
+gzip compressed data, was "NewFunctionsPYC-1.4.0b0.tar", last modified: Sun Jul  2 01:35:35 2023, max compression
```

## Comparing `NewFunctionsPYC-1.3.2.tar` & `NewFunctionsPYC-1.4.0b0.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-03-21 21:22:42.025324 NewFunctionsPYC-1.3.2/
-drwxrwxrwx   0        0        0        0 2023-03-21 21:22:41.994416 NewFunctionsPYC-1.3.2/NewFunctionsPYC/
--rw-rw-rw-   0        0        0      916 2023-03-21 21:21:29.000000 NewFunctionsPYC-1.3.2/NewFunctionsPYC/__init__.py
--rw-rw-rw-   0        0        0     1340 2023-03-21 21:17:02.000000 NewFunctionsPYC-1.3.2/NewFunctionsPYC/checks.py
-drwxrwxrwx   0        0        0        0 2023-03-21 21:22:42.022333 NewFunctionsPYC-1.3.2/NewFunctionsPYC/commands/
--rw-rw-rw-   0        0        0     1353 2023-03-18 20:49:32.000000 NewFunctionsPYC-1.3.2/NewFunctionsPYC/commands/hybrid.py
--rw-rw-rw-   0        0        0      858 2023-01-27 18:48:57.000000 NewFunctionsPYC-1.3.2/NewFunctionsPYC/commands/prefix.py
--rw-rw-rw-   0        0        0      809 2023-01-27 20:57:39.000000 NewFunctionsPYC-1.3.2/NewFunctionsPYC/commands/slash.py
--rw-rw-rw-   0        0        0     5334 2023-03-21 21:15:33.000000 NewFunctionsPYC-1.3.2/NewFunctionsPYC/embed.py
--rw-rw-rw-   0        0        0     3812 2023-03-18 20:34:11.000000 NewFunctionsPYC-1.3.2/NewFunctionsPYC/loader.py
-drwxrwxrwx   0        0        0        0 2023-03-21 21:22:42.018342 NewFunctionsPYC-1.3.2/NewFunctionsPYC.egg-info/
--rw-rw-rw-   0        0        0     1839 2023-03-21 21:22:41.000000 NewFunctionsPYC-1.3.2/NewFunctionsPYC.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      436 2023-03-21 21:22:41.000000 NewFunctionsPYC-1.3.2/NewFunctionsPYC.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-21 21:22:41.000000 NewFunctionsPYC-1.3.2/NewFunctionsPYC.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-03-21 21:22:41.000000 NewFunctionsPYC-1.3.2/NewFunctionsPYC.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-03-21 21:22:41.000000 NewFunctionsPYC-1.3.2/NewFunctionsPYC.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1839 2023-03-21 21:22:42.024333 NewFunctionsPYC-1.3.2/PKG-INFO
--rw-rw-rw-   0        0        0     1025 2023-01-24 21:24:03.000000 NewFunctionsPYC-1.3.2/README.md
--rw-rw-rw-   0        0        0     1008 2023-03-21 21:22:36.000000 NewFunctionsPYC-1.3.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-03-21 21:22:42.025324 NewFunctionsPYC-1.3.2/setup.cfg
--rw-rw-rw-   0        0        0      113 2023-01-25 14:17:10.000000 NewFunctionsPYC-1.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-02 01:35:35.477888 NewFunctionsPYC-1.4.0b0/
+drwxrwxrwx   0        0        0        0 2023-07-02 01:35:35.462927 NewFunctionsPYC-1.4.0b0/NewFunctionsPYC/
+-rw-rw-rw-   0        0        0     1028 2023-07-02 01:24:35.000000 NewFunctionsPYC-1.4.0b0/NewFunctionsPYC/__init__.py
+-rw-rw-rw-   0        0        0     2746 2023-05-27 12:33:02.000000 NewFunctionsPYC-1.4.0b0/NewFunctionsPYC/checks.py
+drwxrwxrwx   0        0        0        0 2023-07-02 01:35:35.473898 NewFunctionsPYC-1.4.0b0/NewFunctionsPYC/commands/
+-rw-rw-rw-   0        0        0     1353 2023-03-18 20:49:32.000000 NewFunctionsPYC-1.4.0b0/NewFunctionsPYC/commands/hybrid.py
+-rw-rw-rw-   0        0        0     1300 2023-07-02 01:33:59.000000 NewFunctionsPYC-1.4.0b0/NewFunctionsPYC/commands/options.py
+-rw-rw-rw-   0        0        0      858 2023-01-27 18:48:57.000000 NewFunctionsPYC-1.4.0b0/NewFunctionsPYC/commands/prefix.py
+-rw-rw-rw-   0        0        0      809 2023-01-27 20:57:39.000000 NewFunctionsPYC-1.4.0b0/NewFunctionsPYC/commands/slash.py
+-rw-rw-rw-   0        0        0     6259 2023-07-01 23:43:16.000000 NewFunctionsPYC-1.4.0b0/NewFunctionsPYC/embed.py
+-rw-rw-rw-   0        0        0     4885 2023-07-02 01:31:30.000000 NewFunctionsPYC-1.4.0b0/NewFunctionsPYC/loader.py
+drwxrwxrwx   0        0        0        0 2023-07-02 01:35:35.468912 NewFunctionsPYC-1.4.0b0/NewFunctionsPYC.egg-info/
+-rw-rw-rw-   0        0        0     1841 2023-07-02 01:35:35.000000 NewFunctionsPYC-1.4.0b0/NewFunctionsPYC.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      472 2023-07-02 01:35:35.000000 NewFunctionsPYC-1.4.0b0/NewFunctionsPYC.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-02 01:35:35.000000 NewFunctionsPYC-1.4.0b0/NewFunctionsPYC.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2023-07-02 01:35:35.000000 NewFunctionsPYC-1.4.0b0/NewFunctionsPYC.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-07-02 01:35:35.000000 NewFunctionsPYC-1.4.0b0/NewFunctionsPYC.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1841 2023-07-02 01:35:35.476891 NewFunctionsPYC-1.4.0b0/PKG-INFO
+-rw-rw-rw-   0        0        0     1025 2023-01-24 21:24:03.000000 NewFunctionsPYC-1.4.0b0/README.md
+-rw-rw-rw-   0        0        0     1009 2023-07-02 01:34:19.000000 NewFunctionsPYC-1.4.0b0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-02 01:35:35.477888 NewFunctionsPYC-1.4.0b0/setup.cfg
+-rw-rw-rw-   0        0        0      142 2023-05-27 12:27:52.000000 NewFunctionsPYC-1.4.0b0/setup.py
```

### Comparing `NewFunctionsPYC-1.3.2/NewFunctionsPYC/__init__.py` & `NewFunctionsPYC-1.4.0b0/NewFunctionsPYC/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,23 +16,31 @@
 
 __name__ = "NewFunctionsPYC"
 __author__ = "Marciel404"
 __license__ = "MIT"
 
 from .embed import (
     EmbedBuilder,
-    rgbColor, 
+    Colors,
+    rgbColor,
     hexadecimalColor
 )
 
 from .loader import (
     Client,
     client,
     bot,
     Bot,
+    getTokenDotEnv
+)
+
+from .commands.options import (
+    Option,
+    OptionType,
+    Choice
 )
 
 from .commands.prefix import (
     prefixContext,
     CommandPrefix,
 )
```

### Comparing `NewFunctionsPYC-1.3.2/NewFunctionsPYC/commands/hybrid.py` & `NewFunctionsPYC-1.4.0b0/NewFunctionsPYC/commands/hybrid.py`

 * *Files identical despite different names*

### Comparing `NewFunctionsPYC-1.3.2/NewFunctionsPYC/commands/prefix.py` & `NewFunctionsPYC-1.4.0b0/NewFunctionsPYC/commands/prefix.py`

 * *Files identical despite different names*

### Comparing `NewFunctionsPYC-1.3.2/NewFunctionsPYC/commands/slash.py` & `NewFunctionsPYC-1.4.0b0/NewFunctionsPYC/commands/slash.py`

 * *Files identical despite different names*

### Comparing `NewFunctionsPYC-1.3.2/NewFunctionsPYC/embed.py` & `NewFunctionsPYC-1.4.0b0/NewFunctionsPYC/embed.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import discord
 import hexacolors
 
 class EmbedBuilder:
+    """Embed contructor alike DiscordJs"""
 
     def __init__(self) -> None:
 
         self.settitle: str = ""
         self.setdescription: str = ""
         self.addfields: list = []
         self.insertfield: list = []
@@ -170,19 +171,51 @@
 
         if self.removethumb != False: 
             self.e.remove_thumbnail()
 
         if self.clearfields != False:
             self.e.clear_fields()
 
-        return self.e
-
     def detonarn(self):
         try:
             del self.e
         except AttributeError:
             pass
-    
+
+class Colors: 
+    """Return interger color for embed"""
+
+    default: int = 0
+    brand_red: int = 0xED4245
+    red: int = 0xE74C3C
+    dark_red: int = 0x992D22
+    blue: int = 0x3498DB
+    dark_blue: int = 0x206694
+    teal: int = 0x1ABC9C
+    dark_teal: int = 0x11806A
+    brand_green: int = 0x57F287
+    green: int = 0x2ECC71
+    dark_green: int = 0x1F8B4C
+    purple: int = 0x9B59B6
+    dark_purple: int = 0x71368A
+    magenta: int = 0xE91E63
+    dark_magenta: int = 0xAD1457
+    gold: int = 0xF1C40F
+    dark_gold: int = 0xC27C0E
+    orange: int = 0xE67E22
+    dark_orange: int = 0xA84300
+    lighter_grey: int = 0x95A5A6
+    dark_grey = 0x607D8B
+    light_grey = 0x979C9F
+    darker_grey = 0x546E7A
+    og_blurple = 0x7289DA
+    blurple = 0x5865F2
+    greyple = 0x99AAB5
+    dark_theme = 0x36393F
+    fuchsia = 0xEB459E
+    yellow = 0xFEE75C
+    nitro_pink = 0xF47FFF
+
 def hexadecimalColor(hex: str):
     return hexacolors.hexadecimal(str(hex))
 def rgbColor(r: int, g: int, b: int):
     return hexacolors.rgb(f"{r},{g},{b}")
```

### Comparing `NewFunctionsPYC-1.3.2/NewFunctionsPYC.egg-info/PKG-INFO` & `NewFunctionsPYC-1.4.0b0/NewFunctionsPYC.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NewFunctionsPYC
-Version: 1.3.2
+Version: 1.4.0b0
 Summary: :A simple library for add new functions the Pycord
 Author: Marciel404
 License: MIT
 Project-URL: Homepage, https://github.com/Marciel404/NewFunctionsPYC
 Keywords: Pycord BetterFunctions
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
```

### Comparing `NewFunctionsPYC-1.3.2/PKG-INFO` & `NewFunctionsPYC-1.4.0b0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NewFunctionsPYC
-Version: 1.3.2
+Version: 1.4.0b0
 Summary: :A simple library for add new functions the Pycord
 Author: Marciel404
 License: MIT
 Project-URL: Homepage, https://github.com/Marciel404/NewFunctionsPYC
 Keywords: Pycord BetterFunctions
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
```

### Comparing `NewFunctionsPYC-1.3.2/README.md` & `NewFunctionsPYC-1.4.0b0/README.md`

 * *Files identical despite different names*

### Comparing `NewFunctionsPYC-1.3.2/pyproject.toml` & `NewFunctionsPYC-1.4.0b0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "NewFunctionsPYC"
-version = "1.3.2"
+version = "1.4.0b"
 keywords = ["Pycord BetterFunctions"]
 authors = [
     {name = "Marciel404"}
 ]
 description = """
 :A simple library for add new functions the Pycord
 """
```

