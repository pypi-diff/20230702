# Comparing `tmp/coolmysql-1.4.6.tar.gz` & `tmp/coolmysql-1.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coolmysql-1.4.6.tar", last modified: Tue Jun 13 15:47:55 2023, max compression
+gzip compressed data, was "coolmysql-1.4.7.tar", last modified: Sun Jul  2 06:46:18 2023, max compression
```

## Comparing `coolmysql-1.4.6.tar` & `coolmysql-1.4.7.tar`

### file list

```diff
@@ -1,5 +1,6 @@
--rw-r--r--   0        0        0    10953 2023-02-13 16:22:52.569575 coolmysql-1.4.6/LICENSE
--rw-r--r--   0        0        0     4427 2023-06-13 15:29:36.475109 coolmysql-1.4.6/README.md
--rw-r--r--   0        0        0       29 2023-04-10 03:59:45.387315 coolmysql-1.4.6/coolmysql.py
--rw-r--r--   0        0        0      601 2023-06-13 15:47:52.295261 coolmysql-1.4.6/pyproject.toml
--rw-r--r--   0        0        0     4712 1970-01-01 00:00:00.000000 coolmysql-1.4.6/PKG-INFO
+-rw-r--r--   0        0        0    10953 2023-02-13 16:22:52.569575 coolmysql-1.4.7/LICENSE
+-rw-r--r--   0        0        0     4128 2023-07-02 06:09:23.077760 coolmysql-1.4.7/README.md
+-rw-r--r--   0        0        0       29 2023-04-10 03:59:45.387315 coolmysql-1.4.7/coolmysql/__init__.py
+-rw-r--r--   0        0        0    18748 2023-06-14 09:13:53.682433 coolmysql-1.4.7/coolmysql/docs/index.md
+-rw-r--r--   0        0        0      603 2023-07-02 06:08:34.041733 coolmysql-1.4.7/pyproject.toml
+-rw-r--r--   0        0        0     4417 1970-01-01 00:00:00.000000 coolmysql-1.4.7/PKG-INFO
```

### Comparing `coolmysql-1.4.6/LICENSE` & `coolmysql-1.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `coolmysql-1.4.6/README.md` & `coolmysql-1.4.7/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -2,29 +2,27 @@
 
 史上最优雅的 mysql ORM 。
 
 # 安装与教程
 
 安装：`pip install coolmysql`
 
-[教程](https://github.com/lcctoor/lccpy/blob/main/packages/coolmysql/docs/doc.md)
+[教程](https://github.com/lcctoor/lccpy/blob/main/packages/coolmysql/coolmysql/docs/index.md)
 
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
 from pymysql import connect
@@ -141,8 +139,8 @@
 
 # 支持作者1元
 
 coolmysql 是一个免费的开源项目，由个人维护。
 
 每个小的贡献，都是构成车轮的一份子，可以帮助保持车轮完美旋转。
 
-<img src="https://raw.githubusercontent.com/lcctoor/me/main/donation/donationQR-1rmb-max.jpg" width="200px">
+<img src="https://lcctoor.github.io/me/donation/donationQR-1rmb-max.jpg" width="200px">
```

### Comparing `coolmysql-1.4.6/pyproject.toml` & `coolmysql-1.4.7/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "coolmysql"
-version = "1.4.6"
+version = "1.4.7"
 description = "史上最优雅的 mysql ORM"
-dependencies = ["lccpy >=1.4.7"]
+dependencies = ["lccpy >=1.4.7.1"]
 keywords = ["coolmysql", "pymysql", "mysql", "aiomysql", "orm"]
 
 readme = "README.md"
 authors = [{name = "许灿标", email = "lcctoor@outlook.com"}]
 license = {file = "LICENSE"}
 classifiers = ["License :: OSI Approved :: Apache Software License"]
 requires-python = ">=3.7"
```

### Comparing `coolmysql-1.4.6/PKG-INFO` & `coolmysql-1.4.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,42 +1,40 @@
 Metadata-Version: 2.1
 Name: coolmysql
-Version: 1.4.6
+Version: 1.4.7
 Summary: 史上最优雅的 mysql ORM
 Keywords: coolmysql,pymysql,mysql,aiomysql,orm
 Author-email: 许灿标 <lcctoor@outlook.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
-Requires-Dist: lccpy >=1.4.7
+Requires-Dist: lccpy >=1.4.7.1
 Project-URL: HomePage, https://github.com/lcctoor/lccpy/tree/main/packages/coolmysql#readme
 
 # 项目描述
 
 史上最优雅的 mysql ORM 。
 
 # 安装与教程
 
 安装：`pip install coolmysql`
 
-[教程](https://github.com/lcctoor/lccpy/blob/main/packages/coolmysql/docs/doc.md)
+[教程](https://github.com/lcctoor/lccpy/blob/main/packages/coolmysql/coolmysql/docs/index.md)
 
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
 from pymysql import connect
@@ -153,9 +151,9 @@
 
 # 支持作者1元
 
 coolmysql 是一个免费的开源项目，由个人维护。
 
 每个小的贡献，都是构成车轮的一份子，可以帮助保持车轮完美旋转。
 
-<img src="https://raw.githubusercontent.com/lcctoor/me/main/donation/donationQR-1rmb-max.jpg" width="200px">
+<img src="https://lcctoor.github.io/me/donation/donationQR-1rmb-max.jpg" width="200px">
```

