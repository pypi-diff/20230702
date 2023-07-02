# Comparing `tmp/coolmongo-1.3.3.tar.gz` & `tmp/coolmongo-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coolmongo-1.3.3.tar", last modified: Tue Jun 13 15:47:30 2023, max compression
+gzip compressed data, was "coolmongo-1.3.4.tar", last modified: Sun Jul  2 06:46:07 2023, max compression
```

## Comparing `coolmongo-1.3.3.tar` & `coolmongo-1.3.4.tar`

### file list

```diff
@@ -1,5 +1,6 @@
--rw-r--r--   0        0        0    10953 2023-02-13 16:22:52.569575 coolmongo-1.3.3/LICENSE
--rw-r--r--   0        0        0     5200 2023-06-13 15:29:36.475109 coolmongo-1.3.3/README.md
--rw-r--r--   0        0        0       29 2023-04-10 03:54:46.072863 coolmongo-1.3.3/coolmongo.py
--rw-r--r--   0        0        0      593 2023-06-13 15:47:25.936483 coolmongo-1.3.3/pyproject.toml
--rw-r--r--   0        0        0     5482 1970-01-01 00:00:00.000000 coolmongo-1.3.3/PKG-INFO
+-rw-r--r--   0        0        0    10953 2023-02-13 16:22:52.569575 coolmongo-1.3.4/LICENSE
+-rw-r--r--   0        0        0     4901 2023-07-02 06:08:05.248699 coolmongo-1.3.4/README.md
+-rw-r--r--   0        0        0       29 2023-04-10 03:54:46.072863 coolmongo-1.3.4/coolmongo/__init__.py
+-rw-r--r--   0        0        0    18005 2023-05-25 16:58:30.727299 coolmongo-1.3.4/coolmongo/docs/index.md
+-rw-r--r--   0        0        0      595 2023-07-02 06:06:59.671803 coolmongo-1.3.4/pyproject.toml
+-rw-r--r--   0        0        0     5187 1970-01-01 00:00:00.000000 coolmongo-1.3.4/PKG-INFO
```

### Comparing `coolmongo-1.3.3/LICENSE` & `coolmongo-1.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `coolmongo-1.3.3/README.md` & `coolmongo-1.3.4/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -2,29 +2,27 @@
 
 史上最优雅的 MongoDB ORM 。
 
 # 安装与教程
 
 安装：`pip install coolmongo`
 
-[教程](https://github.com/lcctoor/lccpy/blob/main/packages/coolmongo/docs/doc.md)
+[教程](https://github.com/lcctoor/lccpy/blob/main/packages/coolmongo/coolmongo/docs/index.md)
 
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
 from pymongo import MongoClient
@@ -139,8 +137,8 @@
 
 # 支持作者1元
 
 coolmongo 是一个免费的开源项目，由个人维护。
 
 每个小的贡献，都是构成车轮的一份子，可以帮助保持车轮完美旋转。
 
-<img src="https://raw.githubusercontent.com/lcctoor/me/main/donation/donationQR-1rmb-max.jpg" width="200px">
+<img src="https://lcctoor.github.io/me/donation/donationQR-1rmb-max.jpg" width="200px">
```

### Comparing `coolmongo-1.3.3/pyproject.toml` & `coolmongo-1.3.4/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "coolmongo"
-version = "1.3.3"
+version = "1.3.4"
 description = "史上最优雅的 MongoDB ORM"
-dependencies = ["lccpy >=1.4.7"]
+dependencies = ["lccpy >=1.4.7.1"]
 keywords = ["coolmongo", "pymongo", "mongodb", "orm"]
 
 readme = "README.md"
 authors = [{name = "许灿标", email = "lcctoor@outlook.com"}]
 license = {file = "LICENSE"}
 classifiers = ["License :: OSI Approved :: Apache Software License"]
 requires-python = ">=3.7"
```

### Comparing `coolmongo-1.3.3/PKG-INFO` & `coolmongo-1.3.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,42 +1,40 @@
 Metadata-Version: 2.1
 Name: coolmongo
-Version: 1.3.3
+Version: 1.3.4
 Summary: 史上最优雅的 MongoDB ORM
 Keywords: coolmongo,pymongo,mongodb,orm
 Author-email: 许灿标 <lcctoor@outlook.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
-Requires-Dist: lccpy >=1.4.7
+Requires-Dist: lccpy >=1.4.7.1
 Project-URL: HomePage, https://github.com/lcctoor/lccpy/tree/main/packages/coolmongo#readme
 
 # 项目描述
 
 史上最优雅的 MongoDB ORM 。
 
 # 安装与教程
 
 安装：`pip install coolmongo`
 
-[教程](https://github.com/lcctoor/lccpy/blob/main/packages/coolmongo/docs/doc.md)
+[教程](https://github.com/lcctoor/lccpy/blob/main/packages/coolmongo/coolmongo/docs/index.md)
 
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
 from pymongo import MongoClient
@@ -151,9 +149,9 @@
 
 # 支持作者1元
 
 coolmongo 是一个免费的开源项目，由个人维护。
 
 每个小的贡献，都是构成车轮的一份子，可以帮助保持车轮完美旋转。
 
-<img src="https://raw.githubusercontent.com/lcctoor/me/main/donation/donationQR-1rmb-max.jpg" width="200px">
+<img src="https://lcctoor.github.io/me/donation/donationQR-1rmb-max.jpg" width="200px">
```

