# Comparing `tmp/rstyleslice-1.4.2.tar.gz` & `tmp/rstyleslice-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rstyleslice-1.4.2.tar", last modified: Tue Jun 13 15:52:03 2023, max compression
+gzip compressed data, was "rstyleslice-1.4.3.tar", last modified: Sun Jul  2 06:46:41 2023, max compression
```

## Comparing `rstyleslice-1.4.2.tar` & `rstyleslice-1.4.3.tar`

### file list

```diff
@@ -1,5 +1,6 @@
--rw-r--r--   0        0        0    10951 2023-02-13 16:30:40.665398 rstyleslice-1.4.2/LICENSE
--rw-r--r--   0        0        0     3510 2023-06-13 15:29:36.465110 rstyleslice-1.4.2/README.md
--rw-r--r--   0        0        0      591 2023-06-13 15:52:00.553142 rstyleslice-1.4.2/pyproject.toml
--rw-r--r--   0        0        0       31 2023-04-10 04:03:01.139197 rstyleslice-1.4.2/rstyleslice.py
--rw-r--r--   0        0        0     3843 1970-01-01 00:00:00.000000 rstyleslice-1.4.2/PKG-INFO
+-rw-r--r--   0        0        0    10951 2023-02-13 16:30:40.665398 rstyleslice-1.4.3/LICENSE
+-rw-r--r--   0        0        0     3213 2023-07-02 06:31:37.593584 rstyleslice-1.4.3/README.md
+-rw-r--r--   0        0        0      593 2023-07-02 06:29:08.610326 rstyleslice-1.4.3/pyproject.toml
+-rw-r--r--   0        0        0       31 2023-04-10 04:03:01.139197 rstyleslice-1.4.3/rstyleslice/__init__.py
+-rw-r--r--   0        0        0     5794 2023-04-25 13:10:59.200573 rstyleslice-1.4.3/rstyleslice/docs/index.md
+-rw-r--r--   0        0        0     3550 1970-01-01 00:00:00.000000 rstyleslice-1.4.3/PKG-INFO
```

### Comparing `rstyleslice-1.4.2/LICENSE` & `rstyleslice-1.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `rstyleslice-1.4.2/README.md` & `rstyleslice-1.4.3/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -10,29 +10,27 @@
 
 切片格式为  [start: stop: step]  ，start 表示从哪条开始，stop 表示到哪条停止，step 表示步长。当  step>=2  时表示间隔式切片。
 
 # 安装与教程
 
 安装：`pip install rstyleslice`
 
-[教程](https://github.com/lcctoor/lccpy/blob/main/packages/rstyleslice/docs/doc.md)
+[教程](https://github.com/lcctoor/lccpy/blob/main/packages/rstyleslice/rstyleslice/docs/index.md)
 
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
 from rstyleslice import rslice
@@ -92,8 +90,8 @@
 
 # 支持作者1元
 
 rstyleslice 是一个免费的开源项目，由个人维护。
 
 每个小的贡献，都是构成车轮的一份子，可以帮助保持车轮完美旋转。
 
-<img src="https://raw.githubusercontent.com/lcctoor/me/main/donation/donationQR-1rmb-max.jpg" width="200px">
+<img src="https://lcctoor.github.io/me/donation/donationQR-1rmb-max.jpg" width="200px">
```

### Comparing `rstyleslice-1.4.2/pyproject.toml` & `rstyleslice-1.4.3/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "rstyleslice"
-version = "1.4.2"
+version = "1.4.3"
 description = "一套符合直觉的索引和切片语法"
-dependencies = ["lccpy >=1.4.7"]
+dependencies = ["lccpy >=1.4.7.1"]
 keywords = ["rstyleslice", "slice"]
 
 readme = "README.md"
 authors = [{name = "许灿标", email = "lcctoor@outlook.com"}]
 license = {file = "LICENSE"}
 classifiers = ["License :: OSI Approved :: Apache Software License"]
 requires-python = ">=3.7"
```

### Comparing `rstyleslice-1.4.2/PKG-INFO` & `rstyleslice-1.4.3/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: rstyleslice
-Version: 1.4.2
+Version: 1.4.3
 Summary: 一套符合直觉的索引和切片语法
 Keywords: rstyleslice,slice
 Author-email: 许灿标 <lcctoor@outlook.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
-Requires-Dist: lccpy >=1.4.7
+Requires-Dist: lccpy >=1.4.7.1
 Project-URL: HomePage, https://github.com/lcctoor/lccpy/tree/main/packages/rstyleslice#readme
 
 # 项目描述
 
 一套符合直觉的索引和切片语法。
 
 |                                        | **Python**                                                           | **rstyleslice**                                                      |
@@ -22,29 +22,27 @@
 
 切片格式为  [start: stop: step]  ，start 表示从哪条开始，stop 表示到哪条停止，step 表示步长。当  step>=2  时表示间隔式切片。
 
 # 安装与教程
 
 安装：`pip install rstyleslice`
 
-[教程](https://github.com/lcctoor/lccpy/blob/main/packages/rstyleslice/docs/doc.md)
+[教程](https://github.com/lcctoor/lccpy/blob/main/packages/rstyleslice/rstyleslice/docs/index.md)
 
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
 from rstyleslice import rslice
@@ -104,9 +102,9 @@
 
 # 支持作者1元
 
 rstyleslice 是一个免费的开源项目，由个人维护。
 
 每个小的贡献，都是构成车轮的一份子，可以帮助保持车轮完美旋转。
 
-<img src="https://raw.githubusercontent.com/lcctoor/me/main/donation/donationQR-1rmb-max.jpg" width="200px">
+<img src="https://lcctoor.github.io/me/donation/donationQR-1rmb-max.jpg" width="200px">
```

