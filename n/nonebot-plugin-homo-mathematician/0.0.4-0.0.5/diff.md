# Comparing `tmp/nonebot_plugin_homo_mathematician-0.0.4.tar.gz` & `tmp/nonebot_plugin_homo_mathematician-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_homo_mathematician-0.0.4.tar", last modified: Tue Jun 20 13:32:08 2023, max compression
+gzip compressed data, was "nonebot_plugin_homo_mathematician-0.0.5.tar", last modified: Sun Jul  2 17:41:04 2023, max compression
```

## Comparing `nonebot_plugin_homo_mathematician-0.0.4.tar` & `nonebot_plugin_homo_mathematician-0.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 13:32:08.647036 nonebot_plugin_homo_mathematician-0.0.4/
--rw-rw-rw-   0        0        0     1064 2022-06-17 16:08:47.000000 nonebot_plugin_homo_mathematician-0.0.4/LICENSE
--rw-rw-rw-   0        0        0      434 2023-06-20 13:32:08.646037 nonebot_plugin_homo_mathematician-0.0.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-20 13:32:08.638035 nonebot_plugin_homo_mathematician-0.0.4/nonebot_plugin_homo_mathematician/
--rw-rw-rw-   0        0        0     1172 2023-06-20 13:29:27.000000 nonebot_plugin_homo_mathematician-0.0.4/nonebot_plugin_homo_mathematician/__init__.py
--rw-rw-rw-   0        0        0     3228 2023-06-20 13:27:33.000000 nonebot_plugin_homo_mathematician-0.0.4/nonebot_plugin_homo_mathematician/handle.py
--rw-rw-rw-   0        0        0    12647 2023-06-20 13:27:33.000000 nonebot_plugin_homo_mathematician-0.0.4/nonebot_plugin_homo_mathematician/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-20 13:32:08.645036 nonebot_plugin_homo_mathematician-0.0.4/nonebot_plugin_homo_mathematician.egg-info/
--rw-rw-rw-   0        0        0      434 2023-06-20 13:32:08.000000 nonebot_plugin_homo_mathematician-0.0.4/nonebot_plugin_homo_mathematician.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      433 2023-06-20 13:32:08.000000 nonebot_plugin_homo_mathematician-0.0.4/nonebot_plugin_homo_mathematician.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 13:32:08.000000 nonebot_plugin_homo_mathematician-0.0.4/nonebot_plugin_homo_mathematician.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2023-06-20 13:32:08.000000 nonebot_plugin_homo_mathematician-0.0.4/nonebot_plugin_homo_mathematician.egg-info/requires.txt
--rw-rw-rw-   0        0        0       34 2023-06-20 13:32:08.000000 nonebot_plugin_homo_mathematician-0.0.4/nonebot_plugin_homo_mathematician.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-20 13:32:08.647036 nonebot_plugin_homo_mathematician-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      651 2023-06-20 13:31:57.000000 nonebot_plugin_homo_mathematician-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-02 17:41:04.149226 nonebot_plugin_homo_mathematician-0.0.5/
+-rw-rw-rw-   0        0        0     1064 2022-06-17 16:08:47.000000 nonebot_plugin_homo_mathematician-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0      434 2023-07-02 17:41:04.149226 nonebot_plugin_homo_mathematician-0.0.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-02 17:41:04.141226 nonebot_plugin_homo_mathematician-0.0.5/nonebot_plugin_homo_mathematician/
+-rw-rw-rw-   0        0        0     1133 2023-07-02 17:40:36.000000 nonebot_plugin_homo_mathematician-0.0.5/nonebot_plugin_homo_mathematician/__init__.py
+-rw-rw-rw-   0        0        0     4193 2023-07-02 17:38:31.000000 nonebot_plugin_homo_mathematician-0.0.5/nonebot_plugin_homo_mathematician/handle.py
+-rw-rw-rw-   0        0        0    12122 2023-07-02 17:22:57.000000 nonebot_plugin_homo_mathematician-0.0.5/nonebot_plugin_homo_mathematician/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-02 17:41:04.147228 nonebot_plugin_homo_mathematician-0.0.5/nonebot_plugin_homo_mathematician.egg-info/
+-rw-rw-rw-   0        0        0      434 2023-07-02 17:41:03.000000 nonebot_plugin_homo_mathematician-0.0.5/nonebot_plugin_homo_mathematician.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      433 2023-07-02 17:41:04.000000 nonebot_plugin_homo_mathematician-0.0.5/nonebot_plugin_homo_mathematician.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-02 17:41:03.000000 nonebot_plugin_homo_mathematician-0.0.5/nonebot_plugin_homo_mathematician.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2023-07-02 17:41:03.000000 nonebot_plugin_homo_mathematician-0.0.5/nonebot_plugin_homo_mathematician.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       34 2023-07-02 17:41:03.000000 nonebot_plugin_homo_mathematician-0.0.5/nonebot_plugin_homo_mathematician.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-02 17:41:04.149226 nonebot_plugin_homo_mathematician-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      651 2023-07-02 17:40:29.000000 nonebot_plugin_homo_mathematician-0.0.5/setup.py
```

### Comparing `nonebot_plugin_homo_mathematician-0.0.4/LICENSE` & `nonebot_plugin_homo_mathematician-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_homo_mathematician-0.0.4/nonebot_plugin_homo_mathematician/__init__.py` & `nonebot_plugin_homo_mathematician-0.0.5/nonebot_plugin_homo_mathematician/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-import contextlib
-
-from nonebot import on_command
-
-from .handle import homo_number, lagrange_interpolation
-
-with contextlib.suppress(Exception):
-    from nonebot.plugin import PluginMetadata
-    __plugin_meta__ = PluginMetadata(
-        name="homo_mathematician",
-        description="任何实数都用连续的114514通过加减乘除达成, 任给一组数据都能找出其内在规律(函数表达式)",
-        usage=r'命令头: {lag, 找规律}  / {homonumber, 臭数字}  eg: 找规律 1 2 3 4 5 6 7 114514 1919810  / homonumber 2749903559',
-        type="application",
-        homepage="https://github.com/Special-Week/Hinata-Bot/tree/main/src/plugins/homo_mathematician",
-        supported_adapters={"~onebot.v11"},
-        extra={
-            'author':   'Special-Week',
-            'version':  '0.0.2',
-            'priority': 10,
-        }
-    )
-
-
-
-on_command(
-    cmd = "homonumber", 
-    block=True, 
-    priority=10, 
-    aliases={"臭数字"}, 
-    handlers=[homo_number.main]
-)
-
-on_command(
-    cmd = 'lag',
-    block=True,
-    priority=10,
-    aliases={"找规律"},
-    handlers=[lagrange_interpolation.main],
-)
+import contextlib
+
+from nonebot import on_command
+
+from .handle import homo_number, lagrange_interpolation
+
+with contextlib.suppress(Exception):
+    from nonebot.plugin import PluginMetadata
+    __plugin_meta__ = PluginMetadata(
+        name="homo_mathematician",
+        description="任何实数都用连续的114514通过加减乘除达成, 任给一组数据都能找出其内在规律(函数表达式)",
+        usage=r'命令头: {lag, 找规律}  / {homonumber, 臭数字}  eg: 找规律 1 2 3 4 5 6 7 114514 1919810  / homonumber 2749903559',
+        type="application",
+        homepage="https://github.com/Special-Week/Hinata-Bot/tree/main/src/plugins/homo_mathematician",
+        supported_adapters={"~onebot.v11"},
+        extra={
+            'author':   'Special-Week',
+            'version':  '0.0.5',
+            'priority': 10,
+        }
+    )
+
+
+
+on_command(
+    cmd = "homonumber", 
+    block=True, 
+    priority=10, 
+    aliases={"臭数字"}, 
+    handlers=[homo_number.main]
+)
+
+on_command(
+    cmd = 'lag',
+    block=True,
+    priority=10,
+    aliases={"找规律"},
+    handlers=[lagrange_interpolation.main],
+)
```

### Comparing `nonebot_plugin_homo_mathematician-0.0.4/setup.py` & `nonebot_plugin_homo_mathematician-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 
 from setuptools import find_packages, setup
 name = 'nonebot_plugin_homo_mathematician'
 
 setup(
     name=name,  
-    version='0.0.4',
+    version='0.0.5',
     author="Special-Week",
     author_email='2749903559@qq.com',
     description="encapsulate logger",
     python_requires=">=3.8.0",
     packages=find_packages(),
     long_description="任何实数都用连续的114514通过加减乘除达成, 任给一组数据都能找出其内在规律(函数表达式)",
     url="https://github.com/Special-Week/Hinata-Bot/tree/main/src/plugins/homo_mathematician",
```

