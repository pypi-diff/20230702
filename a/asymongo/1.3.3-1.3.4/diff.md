# Comparing `tmp/asymongo-1.3.3.tar.gz` & `tmp/asymongo-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asymongo-1.3.3.tar", last modified: Tue Jun 13 15:45:20 2023, max compression
+gzip compressed data, was "asymongo-1.3.4.tar", last modified: Sun Jul  2 06:44:32 2023, max compression
```

## Comparing `asymongo-1.3.3.tar` & `asymongo-1.3.4.tar`

### file list

```diff
@@ -1,5 +1,6 @@
--rw-r--r--   0        0        0    10953 2023-02-13 16:22:52.569575 asymongo-1.3.3/LICENSE
--rw-r--r--   0        0        0     5338 2023-06-13 15:29:36.475109 asymongo-1.3.3/README.md
--rw-r--r--   0        0        0       28 2023-04-10 03:40:07.519027 asymongo-1.3.3/asymongo.py
--rw-r--r--   0        0        0      590 2023-06-13 15:44:55.395808 asymongo-1.3.3/pyproject.toml
--rw-r--r--   0        0        0     5612 1970-01-01 00:00:00.000000 asymongo-1.3.3/PKG-INFO
+-rw-r--r--   0        0        0    10953 2023-02-13 16:22:52.569575 asymongo-1.3.4/LICENSE
+-rw-r--r--   0        0        0     5038 2023-07-02 06:03:16.291844 asymongo-1.3.4/README.md
+-rw-r--r--   0        0        0       28 2023-04-10 03:40:07.519027 asymongo-1.3.4/asymongo/__init__.py
+-rw-r--r--   0        0        0    16892 2023-04-25 13:09:33.999319 asymongo-1.3.4/asymongo/docs/index.md
+-rw-r--r--   0        0        0      592 2023-07-02 06:04:16.818887 asymongo-1.3.4/pyproject.toml
+-rw-r--r--   0        0        0     5316 1970-01-01 00:00:00.000000 asymongo-1.3.4/PKG-INFO
```

### Comparing `asymongo-1.3.3/LICENSE` & `asymongo-1.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `asymongo-1.3.3/README.md` & `asymongo-1.3.4/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -2,29 +2,27 @@
 
 异步的 MongoDB ORM 。
 
 # 安装与教程
 
 安装：`pip install asymongo`
 
-[教程](https://github.com/lcctoor/lccpy/blob/main/packages/asymongo/docs/doc.md)
+[教程](https://github.com/lcctoor/lccpy/blob/main/packages/asymongo/asymongo/docs/index.md)
 
 # Bug提交、功能提议
 
-您可以通过 [Github-Issues](https://github.com/lcctoor/lccpy/issues)、[微信](https://raw.githubusercontent.com/lcctoor/me/main/author/WeChatQR-max.jpg)、[技术交流群](https://raw.githubusercontent.com/lcctoor/me/main/lccpy/WechatReadersGroupQR-original.jpg) 与我联系。
+您可以通过 [Github-Issues](https://github.com/lcctoor/lccpy/issues)、[微信](https://lcctoor.github.io/me/author/WeChatQR-max.jpg)、[技术交流群](https://lcctoor.github.io/me/lccpy/WechatReadersGroupQR-original.jpg) 与我联系。
 
 # 关于作者
 
 作者：许灿标
 
 邮箱：lcctoor@outlook.com
 
-[主页](https://github.com/lcctoor/me#readme) | [微信](https://raw.githubusercontent.com/lcctoor/me/main/author/WeChatQR-max.jpg) | [微信公众号](https://raw.githubusercontent.com/lcctoor/me/main/author/WechatSubscribeQRAndSearch-max.png) | [Python技术交流群](https://raw.githubusercontent.com/lcctoor/me/main/lccpy/WechatReadersGroupQR-original.jpg)
-
-开源项目：[让Python更简单一点](https://github.com/lcctoor/lccpy#readme)
+[主页](https://lcctoor.github.io/me/) | [微信](https://lcctoor.github.io/me/author/WeChatQR-max.jpg) | [Python技术交流群](https://lcctoor.github.io/me/lccpy/WechatReadersGroupQR-original.jpg)
 
 # 教程预览
 
 #### 导入
 
 ```python
 from motor.motor_asyncio import AsyncIOMotorClient as MongoClient
@@ -141,8 +139,8 @@
 
 # 支持作者1元
 
 asymongo 是一个免费的开源项目，由个人维护。
 
 每个小的贡献，都是构成车轮的一份子，可以帮助保持车轮完美旋转。
 
-<img src="https://raw.githubusercontent.com/lcctoor/me/main/donation/donationQR-1rmb-max.jpg" width="200px">
+<img src="https://lcctoor.github.io/me/donation/donationQR-1rmb-max.jpg" width="200px">
```

### Comparing `asymongo-1.3.3/pyproject.toml` & `asymongo-1.3.4/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "asymongo"
-version = "1.3.3"
+version = "1.3.4"
 description = "异步的 MongoDB ORM"
-dependencies = ["lccpy >=1.4.7"]
+dependencies = ["lccpy >=1.4.7.1"]
 keywords = ["asymongo", "motor", "mongodb", "pymongo", "orm"]
 
 readme = "README.md"
 authors = [{name = "许灿标", email = "lcctoor@outlook.com"}]
 license = {file = "LICENSE"}
 classifiers = ["License :: OSI Approved :: Apache Software License"]
 requires-python = ">=3.7"
```

### Comparing `asymongo-1.3.3/PKG-INFO` & `asymongo-1.3.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,42 +1,40 @@
 Metadata-Version: 2.1
 Name: asymongo
-Version: 1.3.3
+Version: 1.3.4
 Summary: 异步的 MongoDB ORM
 Keywords: asymongo,motor,mongodb,pymongo,orm
 Author-email: 许灿标 <lcctoor@outlook.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
-Requires-Dist: lccpy >=1.4.7
+Requires-Dist: lccpy >=1.4.7.1
 Project-URL: HomePage, https://github.com/lcctoor/lccpy/tree/main/packages/asymongo#readme
 
 # 项目描述
 
 异步的 MongoDB ORM 。
 
 # 安装与教程
 
 安装：`pip install asymongo`
 
-[教程](https://github.com/lcctoor/lccpy/blob/main/packages/asymongo/docs/doc.md)
+[教程](https://github.com/lcctoor/lccpy/blob/main/packages/asymongo/asymongo/docs/index.md)
 
 # Bug提交、功能提议
 
-您可以通过 [Github-Issues](https://github.com/lcctoor/lccpy/issues)、[微信](https://raw.githubusercontent.com/lcctoor/me/main/author/WeChatQR-max.jpg)、[技术交流群](https://raw.githubusercontent.com/lcctoor/me/main/lccpy/WechatReadersGroupQR-original.jpg) 与我联系。
+您可以通过 [Github-Issues](https://github.com/lcctoor/lccpy/issues)、[微信](https://lcctoor.github.io/me/author/WeChatQR-max.jpg)、[技术交流群](https://lcctoor.github.io/me/lccpy/WechatReadersGroupQR-original.jpg) 与我联系。
 
 # 关于作者
 
 作者：许灿标
 
 邮箱：lcctoor@outlook.com
 
-[主页](https://github.com/lcctoor/me#readme) | [微信](https://raw.githubusercontent.com/lcctoor/me/main/author/WeChatQR-max.jpg) | [微信公众号](https://raw.githubusercontent.com/lcctoor/me/main/author/WechatSubscribeQRAndSearch-max.png) | [Python技术交流群](https://raw.githubusercontent.com/lcctoor/me/main/lccpy/WechatReadersGroupQR-original.jpg)
-
-开源项目：[让Python更简单一点](https://github.com/lcctoor/lccpy#readme)
+[主页](https://lcctoor.github.io/me/) | [微信](https://lcctoor.github.io/me/author/WeChatQR-max.jpg) | [Python技术交流群](https://lcctoor.github.io/me/lccpy/WechatReadersGroupQR-original.jpg)
 
 # 教程预览
 
 #### 导入
 
 ```python
 from motor.motor_asyncio import AsyncIOMotorClient as MongoClient
@@ -153,9 +151,9 @@
 
 # 支持作者1元
 
 asymongo 是一个免费的开源项目，由个人维护。
 
 每个小的贡献，都是构成车轮的一份子，可以帮助保持车轮完美旋转。
 
-<img src="https://raw.githubusercontent.com/lcctoor/me/main/donation/donationQR-1rmb-max.jpg" width="200px">
+<img src="https://lcctoor.github.io/me/donation/donationQR-1rmb-max.jpg" width="200px">
```

