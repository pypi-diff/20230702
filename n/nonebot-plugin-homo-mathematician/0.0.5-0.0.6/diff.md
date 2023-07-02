# Comparing `tmp/nonebot_plugin_homo_mathematician-0.0.5.tar.gz` & `tmp/nonebot_plugin_homo_mathematician-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_homo_mathematician-0.0.5.tar", last modified: Sun Jul  2 17:41:04 2023, max compression
+gzip compressed data, was "nonebot_plugin_homo_mathematician-0.0.6.tar", last modified: Sun Jul  2 17:59:28 2023, max compression
```

## Comparing `nonebot_plugin_homo_mathematician-0.0.5.tar` & `nonebot_plugin_homo_mathematician-0.0.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-02 17:41:04.149226 nonebot_plugin_homo_mathematician-0.0.5/
--rw-rw-rw-   0        0        0     1064 2022-06-17 16:08:47.000000 nonebot_plugin_homo_mathematician-0.0.5/LICENSE
--rw-rw-rw-   0        0        0      434 2023-07-02 17:41:04.149226 nonebot_plugin_homo_mathematician-0.0.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-02 17:41:04.141226 nonebot_plugin_homo_mathematician-0.0.5/nonebot_plugin_homo_mathematician/
--rw-rw-rw-   0        0        0     1133 2023-07-02 17:40:36.000000 nonebot_plugin_homo_mathematician-0.0.5/nonebot_plugin_homo_mathematician/__init__.py
--rw-rw-rw-   0        0        0     4193 2023-07-02 17:38:31.000000 nonebot_plugin_homo_mathematician-0.0.5/nonebot_plugin_homo_mathematician/handle.py
--rw-rw-rw-   0        0        0    12122 2023-07-02 17:22:57.000000 nonebot_plugin_homo_mathematician-0.0.5/nonebot_plugin_homo_mathematician/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-02 17:41:04.147228 nonebot_plugin_homo_mathematician-0.0.5/nonebot_plugin_homo_mathematician.egg-info/
--rw-rw-rw-   0        0        0      434 2023-07-02 17:41:03.000000 nonebot_plugin_homo_mathematician-0.0.5/nonebot_plugin_homo_mathematician.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      433 2023-07-02 17:41:04.000000 nonebot_plugin_homo_mathematician-0.0.5/nonebot_plugin_homo_mathematician.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-02 17:41:03.000000 nonebot_plugin_homo_mathematician-0.0.5/nonebot_plugin_homo_mathematician.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2023-07-02 17:41:03.000000 nonebot_plugin_homo_mathematician-0.0.5/nonebot_plugin_homo_mathematician.egg-info/requires.txt
--rw-rw-rw-   0        0        0       34 2023-07-02 17:41:03.000000 nonebot_plugin_homo_mathematician-0.0.5/nonebot_plugin_homo_mathematician.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-02 17:41:04.149226 nonebot_plugin_homo_mathematician-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      651 2023-07-02 17:40:29.000000 nonebot_plugin_homo_mathematician-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-02 17:59:28.901095 nonebot_plugin_homo_mathematician-0.0.6/
+-rw-rw-rw-   0        0        0     1064 2022-06-17 16:08:47.000000 nonebot_plugin_homo_mathematician-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0      434 2023-07-02 17:59:28.901095 nonebot_plugin_homo_mathematician-0.0.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-02 17:59:28.893033 nonebot_plugin_homo_mathematician-0.0.6/nonebot_plugin_homo_mathematician/
+-rw-rw-rw-   0        0        0     1133 2023-07-02 17:56:07.000000 nonebot_plugin_homo_mathematician-0.0.6/nonebot_plugin_homo_mathematician/__init__.py
+-rw-rw-rw-   0        0        0     4157 2023-07-02 17:55:28.000000 nonebot_plugin_homo_mathematician-0.0.6/nonebot_plugin_homo_mathematician/handle.py
+-rw-rw-rw-   0        0        0    12122 2023-07-02 17:22:57.000000 nonebot_plugin_homo_mathematician-0.0.6/nonebot_plugin_homo_mathematician/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-02 17:59:28.898886 nonebot_plugin_homo_mathematician-0.0.6/nonebot_plugin_homo_mathematician.egg-info/
+-rw-rw-rw-   0        0        0      434 2023-07-02 17:59:28.000000 nonebot_plugin_homo_mathematician-0.0.6/nonebot_plugin_homo_mathematician.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      433 2023-07-02 17:59:28.000000 nonebot_plugin_homo_mathematician-0.0.6/nonebot_plugin_homo_mathematician.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-02 17:59:28.000000 nonebot_plugin_homo_mathematician-0.0.6/nonebot_plugin_homo_mathematician.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2023-07-02 17:59:28.000000 nonebot_plugin_homo_mathematician-0.0.6/nonebot_plugin_homo_mathematician.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       34 2023-07-02 17:59:28.000000 nonebot_plugin_homo_mathematician-0.0.6/nonebot_plugin_homo_mathematician.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-02 17:59:28.901095 nonebot_plugin_homo_mathematician-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      651 2023-07-02 17:59:14.000000 nonebot_plugin_homo_mathematician-0.0.6/setup.py
```

### Comparing `nonebot_plugin_homo_mathematician-0.0.5/LICENSE` & `nonebot_plugin_homo_mathematician-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_homo_mathematician-0.0.5/nonebot_plugin_homo_mathematician/__init__.py` & `nonebot_plugin_homo_mathematician-0.0.6/nonebot_plugin_homo_mathematician/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
         description="任何实数都用连续的114514通过加减乘除达成, 任给一组数据都能找出其内在规律(函数表达式)",
         usage=r'命令头: {lag, 找规律}  / {homonumber, 臭数字}  eg: 找规律 1 2 3 4 5 6 7 114514 1919810  / homonumber 2749903559',
         type="application",
         homepage="https://github.com/Special-Week/Hinata-Bot/tree/main/src/plugins/homo_mathematician",
         supported_adapters={"~onebot.v11"},
         extra={
             'author':   'Special-Week',
-            'version':  '0.0.5',
+            'version':  '0.0.6',
             'priority': 10,
         }
     )
 
 
 
 on_command(
```

### Comparing `nonebot_plugin_homo_mathematician-0.0.5/nonebot_plugin_homo_mathematician/handle.py` & `nonebot_plugin_homo_mathematician-0.0.6/nonebot_plugin_homo_mathematician/handle.py`

 * *Files 3% similar despite different names*

```diff
@@ -94,14 +94,14 @@
         """将字符串列表转换为数字列表"""
         numbers: list = []
         for string in strings:
             if string.isdigit():
                 numbers.append(int(string))
             elif string.startswith("-") and string[1:].isdigit():  # 判断是否为负整数
                 numbers.append(int(string))
-            elif string.replace(".", "", 1).isdigit():  # 判断是否为小数
+            else:   # 判断是否为小数
                 numbers.append(float(string))
         return numbers
 
 
 homo_number = HomoNumber()
 lagrange_interpolation = LagrangeInterpolation()
```

### Comparing `nonebot_plugin_homo_mathematician-0.0.5/nonebot_plugin_homo_mathematician/utils.py` & `nonebot_plugin_homo_mathematician-0.0.6/nonebot_plugin_homo_mathematician/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_homo_mathematician-0.0.5/setup.py` & `nonebot_plugin_homo_mathematician-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 
 from setuptools import find_packages, setup
 name = 'nonebot_plugin_homo_mathematician'
 
 setup(
     name=name,  
-    version='0.0.5',
+    version='0.0.6',
     author="Special-Week",
     author_email='2749903559@qq.com',
     description="encapsulate logger",
     python_requires=">=3.8.0",
     packages=find_packages(),
     long_description="任何实数都用连续的114514通过加减乘除达成, 任给一组数据都能找出其内在规律(函数表达式)",
     url="https://github.com/Special-Week/Hinata-Bot/tree/main/src/plugins/homo_mathematician",
```

