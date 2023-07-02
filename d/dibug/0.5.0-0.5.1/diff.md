# Comparing `tmp/dibug-0.5.0.tar.gz` & `tmp/dibug-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dibug-0.5.0.tar", max compression
+gzip compressed data, was "dibug-0.5.1.tar", max compression
```

## Comparing `dibug-0.5.0.tar` & `dibug-0.5.1.tar`

### file list

```diff
@@ -1,17 +1,18 @@
--rw-r--r--   0        0        0     1076 2023-06-30 02:31:28.764861 dibug-0.5.0/LICENSE
--rw-r--r--   0        0        0     1353 2023-06-30 02:31:28.764861 dibug-0.5.0/README.md
--rw-r--r--   0        0        0       66 2023-06-30 02:31:28.768861 dibug-0.5.0/dibug/__init__.py
--rw-r--r--   0        0        0      228 2023-06-30 02:31:28.768861 dibug-0.5.0/dibug/abc.py
--rw-r--r--   0        0        0      195 2023-06-30 02:31:28.768861 dibug-0.5.0/dibug/commands/__init__.py
--rw-r--r--   0        0        0     1746 2023-06-30 02:31:28.768861 dibug-0.5.0/dibug/commands/eval.py
--rw-r--r--   0        0        0     1694 2023-06-30 02:31:28.768861 dibug-0.5.0/dibug/commands/info.py
--rw-r--r--   0        0        0      286 2023-06-30 02:31:28.768861 dibug-0.5.0/dibug/commands/kill.py
--rw-r--r--   0        0        0     1317 2023-06-30 02:31:28.768861 dibug-0.5.0/dibug/commands/shell.py
--rw-r--r--   0        0        0     5350 2023-06-30 02:31:28.768861 dibug-0.5.0/dibug/dibugger.py
--rw-r--r--   0        0        0        0 2023-06-30 02:31:28.768861 dibug-0.5.0/dibug/py.typed
--rw-r--r--   0        0        0      143 2023-06-30 02:31:28.768861 dibug-0.5.0/dibug/utils/__init__.py
--rw-r--r--   0        0        0      470 2023-06-30 02:31:28.768861 dibug-0.5.0/dibug/utils/chunk.py
--rw-r--r--   0        0        0      675 2023-06-30 02:31:28.768861 dibug-0.5.0/dibug/utils/embed.py
--rw-r--r--   0        0        0      808 2023-06-30 02:31:28.768861 dibug-0.5.0/dibug/utils/object.py
--rw-r--r--   0        0        0      780 2023-06-30 02:31:28.768861 dibug-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     2001 1970-01-01 00:00:00.000000 dibug-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-07-02 13:39:37.520857 dibug-0.5.1/LICENSE
+-rw-r--r--   0        0        0     1353 2023-07-02 13:39:37.520857 dibug-0.5.1/README.md
+-rw-r--r--   0        0        0       91 2023-07-02 13:39:37.520857 dibug-0.5.1/dibug/__init__.py
+-rw-r--r--   0        0        0      228 2023-07-02 13:39:37.520857 dibug-0.5.1/dibug/abc.py
+-rw-r--r--   0        0        0      195 2023-07-02 13:39:37.520857 dibug-0.5.1/dibug/commands/__init__.py
+-rw-r--r--   0        0        0     1746 2023-07-02 13:39:37.520857 dibug-0.5.1/dibug/commands/eval.py
+-rw-r--r--   0        0        0     1702 2023-07-02 13:39:37.520857 dibug-0.5.1/dibug/commands/info.py
+-rw-r--r--   0        0        0      286 2023-07-02 13:39:37.520857 dibug-0.5.1/dibug/commands/kill.py
+-rw-r--r--   0        0        0     1317 2023-07-02 13:39:37.520857 dibug-0.5.1/dibug/commands/shell.py
+-rw-r--r--   0        0        0     5350 2023-07-02 13:39:37.520857 dibug-0.5.1/dibug/dibugger.py
+-rw-r--r--   0        0        0        0 2023-07-02 13:39:37.520857 dibug-0.5.1/dibug/py.typed
+-rw-r--r--   0        0        0      143 2023-07-02 13:39:37.520857 dibug-0.5.1/dibug/utils/__init__.py
+-rw-r--r--   0        0        0      470 2023-07-02 13:39:37.520857 dibug-0.5.1/dibug/utils/chunk.py
+-rw-r--r--   0        0        0      675 2023-07-02 13:39:37.520857 dibug-0.5.1/dibug/utils/embed.py
+-rw-r--r--   0        0        0      808 2023-07-02 13:39:37.520857 dibug-0.5.1/dibug/utils/object.py
+-rw-r--r--   0        0        0       22 2023-07-02 13:39:37.520857 dibug-0.5.1/dibug/version.py
+-rw-r--r--   0        0        0      780 2023-07-02 13:39:37.524857 dibug-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     2001 1970-01-01 00:00:00.000000 dibug-0.5.1/PKG-INFO
```

### Comparing `dibug-0.5.0/LICENSE` & `dibug-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dibug-0.5.0/README.md` & `dibug-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `dibug-0.5.0/dibug/commands/eval.py` & `dibug-0.5.1/dibug/commands/eval.py`

 * *Files identical despite different names*

### Comparing `dibug-0.5.0/dibug/commands/info.py` & `dibug-0.5.1/dibug/commands/info.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 from platform import release, system
 from sys import platform, version
 
-from discord import Client, Message, __version__
-from pkg_resources import get_distribution
+from discord import Client, Message
+from discord import __version__ as discord_version
 from psutil import Process
 
 from ..abc import DibugCommandABC
+from ..version import __version__ as dibug_version
 
 
 class InfoCommand(DibugCommandABC):
     def __init__(self, name: list[str], client: Client) -> None:
         super().__init__(name)
 
         self.__client = client
 
     async def execute(self, msg: Message, args: str) -> None:
         lines: list[str] = []
 
         lines.append(f"Python `{version}` on `{system()} {release()} ({platform})`")
 
-        lines.append(
-            f"dibug `{get_distribution('dibug').version}`, discord.py `{__version__}`"
-        )
+        lines.append(f"dibug `{dibug_version}`, discord.py `{discord_version}`")
 
         lines.append("")
 
         process = Process()
         lines.append(
             f"Process started at <t:{int(process.create_time())}:R>, PID {process.pid}, using {round(process.memory_info().rss / 2 ** 20, 2)}MB of memory"
         )
```

### Comparing `dibug-0.5.0/dibug/commands/shell.py` & `dibug-0.5.1/dibug/commands/shell.py`

 * *Files identical despite different names*

### Comparing `dibug-0.5.0/dibug/dibugger.py` & `dibug-0.5.1/dibug/dibugger.py`

 * *Files identical despite different names*

### Comparing `dibug-0.5.0/dibug/utils/embed.py` & `dibug-0.5.1/dibug/utils/embed.py`

 * *Files identical despite different names*

### Comparing `dibug-0.5.0/dibug/utils/object.py` & `dibug-0.5.1/dibug/utils/object.py`

 * *Files identical despite different names*

### Comparing `dibug-0.5.0/pyproject.toml` & `dibug-0.5.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dibug"
-version = "0.5.0"
+version = "0.5.1"
 description = "Debugging Tool for discord.py"
 authors = ["Starcea <stardev.uwu@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/star0202/dibug"
 
 [tool.poetry.dependencies]
```

### Comparing `dibug-0.5.0/PKG-INFO` & `dibug-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dibug
-Version: 0.5.0
+Version: 0.5.1
 Summary: Debugging Tool for discord.py
 Home-page: https://github.com/star0202/dibug
 License: MIT
 Author: Starcea
 Author-email: stardev.uwu@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

