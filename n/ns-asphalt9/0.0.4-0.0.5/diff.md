# Comparing `tmp/ns_asphalt9-0.0.4.tar.gz` & `tmp/ns_asphalt9-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ns_asphalt9-0.0.4.tar", last modified: Fri Jun 30 07:55:43 2023, max compression
+gzip compressed data, was "dist/ns_asphalt9-0.0.5.tar", last modified: Sun Jul  2 12:38:46 2023, max compression
```

## Comparing `ns_asphalt9-0.0.4.tar` & `ns_asphalt9-0.0.5.tar`

### file list

```diff
@@ -1,50 +1,48 @@
-drwxr-xr-x   0 neo.sun    (502) staff       (20)        0 2023-06-30 07:55:43.354523 ns_asphalt9-0.0.4/
--rw-r--r--   0 neo.sun    (502) staff       (20)    35149 2023-04-10 06:16:35.000000 ns_asphalt9-0.0.4/LICENSE
--rw-r--r--   0 neo.sun    (502) staff       (20)      180 2023-06-30 07:35:13.000000 ns_asphalt9-0.0.4/MANIFEST.in
--rw-r--r--   0 neo.sun    (502) staff       (20)     2020 2023-06-30 07:55:43.354607 ns_asphalt9-0.0.4/PKG-INFO
--rw-r--r--   0 neo.sun    (502) staff       (20)     1041 2023-05-04 03:01:57.000000 ns_asphalt9-0.0.4/README.md
-drwxr-xr-x   0 neo.sun    (502) staff       (20)        0 2023-06-30 07:55:43.345411 ns_asphalt9-0.0.4/ns_asphalt9/
-drwxr-xr-x   0 neo.sun    (502) staff       (20)        0 2023-06-30 07:55:43.349405 ns_asphalt9-0.0.4/ns_asphalt9/core/
--rw-r--r--   0 neo.sun    (502) staff       (20)       20 2023-06-30 07:48:40.000000 ns_asphalt9-0.0.4/ns_asphalt9/core/__init__.py
-drwxr-xr-x   0 neo.sun    (502) staff       (20)        0 2023-06-30 07:55:43.350488 ns_asphalt9-0.0.4/ns_asphalt9/core/actions/
--rw-r--r--   0 neo.sun    (502) staff       (20)      197 2023-06-30 07:49:09.000000 ns_asphalt9-0.0.4/ns_asphalt9/core/actions/__init__.py
--rw-r--r--   0 neo.sun    (502) staff       (20)      336 2023-06-30 07:50:30.000000 ns_asphalt9-0.0.4/ns_asphalt9/core/actions/common.py
--rw-r--r--   0 neo.sun    (502) staff       (20)     3201 2023-06-30 07:52:00.000000 ns_asphalt9-0.0.4/ns_asphalt9/core/actions/enter_page.py
--rw-r--r--   0 neo.sun    (502) staff       (20)     3833 2023-06-30 07:52:43.000000 ns_asphalt9-0.0.4/ns_asphalt9/core/actions/process_race.py
--rw-r--r--   0 neo.sun    (502) staff       (20)     3524 2023-06-30 07:53:13.000000 ns_asphalt9-0.0.4/ns_asphalt9/core/actions/select_car.py
--rw-r--r--   0 neo.sun    (502) staff       (20)      706 2023-06-28 08:30:50.000000 ns_asphalt9-0.0.4/ns_asphalt9/core/cache.py
--rw-r--r--   0 neo.sun    (502) staff       (20)     2556 2023-06-28 07:46:07.000000 ns_asphalt9-0.0.4/ns_asphalt9/core/consts.py
--rw-r--r--   0 neo.sun    (502) staff       (20)     2146 2023-06-30 07:54:21.000000 ns_asphalt9-0.0.4/ns_asphalt9/core/controller.py
--rw-r--r--   0 neo.sun    (502) staff       (20)      498 2023-06-30 07:54:26.000000 ns_asphalt9-0.0.4/ns_asphalt9/core/globals.py
-drwxr-xr-x   0 neo.sun    (502) staff       (20)        0 2023-06-30 07:55:43.350801 ns_asphalt9-0.0.4/ns_asphalt9/core/gui/
--rw-r--r--   0 neo.sun    (502) staff       (20)        0 2023-06-26 05:07:57.000000 ns_asphalt9-0.0.4/ns_asphalt9/core/gui/__init__.py
--rw-r--r--   0 neo.sun    (502) staff       (20)    17447 2023-06-28 07:35:12.000000 ns_asphalt9-0.0.4/ns_asphalt9/core/gui/app.py
-drwxr-xr-x   0 neo.sun    (502) staff       (20)        0 2023-06-30 07:55:43.352901 ns_asphalt9-0.0.4/ns_asphalt9/core/gui/images/
--rw-r--r--   0 neo.sun    (502) staff       (20)     3097 2023-06-26 08:14:33.000000 ns_asphalt9-0.0.4/ns_asphalt9/core/gui/images/help.png
--rw-r--r--   0 neo.sun    (502) staff       (20)     2900 2023-06-26 08:18:26.000000 ns_asphalt9-0.0.4/ns_asphalt9/core/gui/images/home.png
--rw-r--r--   0 neo.sun    (502) staff       (20)   202347 2023-06-26 05:17:10.000000 ns_asphalt9-0.0.4/ns_asphalt9/core/gui/images/logo.png
--rw-r--r--   0 neo.sun    (502) staff       (20)     3159 2023-06-26 08:11:35.000000 ns_asphalt9-0.0.4/ns_asphalt9/core/gui/images/settings.png
--rw-r--r--   0 neo.sun    (502) staff       (20)     1530 2023-06-30 07:54:36.000000 ns_asphalt9-0.0.4/ns_asphalt9/core/ocr.py
--rw-r--r--   0 neo.sun    (502) staff       (20)     1847 2023-06-30 07:54:51.000000 ns_asphalt9-0.0.4/ns_asphalt9/core/page_factory.py
--rw-r--r--   0 neo.sun    (502) staff       (20)    10864 2023-06-30 07:55:03.000000 ns_asphalt9-0.0.4/ns_asphalt9/core/pages.py
--rw-r--r--   0 neo.sun    (502) staff       (20)      265 2023-06-29 06:50:43.000000 ns_asphalt9-0.0.4/ns_asphalt9/core/screenshot.py
--rw-r--r--   0 neo.sun    (502) staff       (20)     2488 2023-06-30 07:55:19.000000 ns_asphalt9-0.0.4/ns_asphalt9/core/tasks.py
-drwxr-xr-x   0 neo.sun    (502) staff       (20)        0 2023-06-30 07:55:43.354067 ns_asphalt9-0.0.4/ns_asphalt9/core/utils/
--rw-r--r--   0 neo.sun    (502) staff       (20)        0 2023-06-25 08:40:05.000000 ns_asphalt9-0.0.4/ns_asphalt9/core/utils/__init__.py
--rw-r--r--   0 neo.sun    (502) staff       (20)     1016 2023-06-30 07:53:42.000000 ns_asphalt9-0.0.4/ns_asphalt9/core/utils/decorator.py
--rw-r--r--   0 neo.sun    (502) staff       (20)      459 2023-06-25 08:40:05.000000 ns_asphalt9-0.0.4/ns_asphalt9/core/utils/fetch_cars.py
--rw-r--r--   0 neo.sun    (502) staff       (20)     1993 2023-06-30 07:53:54.000000 ns_asphalt9-0.0.4/ns_asphalt9/core/utils/log.py
--rw-r--r--   0 neo.sun    (502) staff       (20)      862 2023-06-30 07:54:03.000000 ns_asphalt9-0.0.4/ns_asphalt9/core/utils/timer.py
--rw-r--r--   0 neo.sun    (502) staff       (20)     5071 2023-06-30 07:48:31.000000 ns_asphalt9-0.0.4/ns_asphalt9/main.py
-drwxr-xr-x   0 neo.sun    (502) staff       (20)        0 2023-06-30 07:55:43.346745 ns_asphalt9-0.0.4/ns_asphalt9.egg-info/
--rw-r--r--   0 neo.sun    (502) staff       (20)     2020 2023-06-30 07:55:43.000000 ns_asphalt9-0.0.4/ns_asphalt9.egg-info/PKG-INFO
--rw-r--r--   0 neo.sun    (502) staff       (20)     1187 2023-06-30 07:55:43.000000 ns_asphalt9-0.0.4/ns_asphalt9.egg-info/SOURCES.txt
--rw-r--r--   0 neo.sun    (502) staff       (20)        1 2023-06-30 07:55:43.000000 ns_asphalt9-0.0.4/ns_asphalt9.egg-info/dependency_links.txt
--rw-r--r--   0 neo.sun    (502) staff       (20)       54 2023-06-30 07:55:43.000000 ns_asphalt9-0.0.4/ns_asphalt9.egg-info/entry_points.txt
--rw-r--r--   0 neo.sun    (502) staff       (20)        1 2023-06-30 07:09:01.000000 ns_asphalt9-0.0.4/ns_asphalt9.egg-info/not-zip-safe
--rw-r--r--   0 neo.sun    (502) staff       (20)      107 2023-06-30 07:55:43.000000 ns_asphalt9-0.0.4/ns_asphalt9.egg-info/requires.txt
--rw-r--r--   0 neo.sun    (502) staff       (20)       12 2023-06-30 07:55:43.000000 ns_asphalt9-0.0.4/ns_asphalt9.egg-info/top_level.txt
--rw-r--r--   0 neo.sun    (502) staff       (20)     1299 2023-06-30 07:55:43.354975 ns_asphalt9-0.0.4/setup.cfg
--rw-r--r--   0 neo.sun    (502) staff       (20)      387 2023-06-30 03:30:00.000000 ns_asphalt9-0.0.4/setup.py
-drwxr-xr-x   0 neo.sun    (502) staff       (20)        0 2023-06-30 07:55:43.354269 ns_asphalt9-0.0.4/tests/
--rw-r--r--   0 neo.sun    (502) staff       (20)     1204 2023-06-29 06:52:40.000000 ns_asphalt9-0.0.4/tests/test_ocr.py
+drwxr-xr-x   0 sunhao     (501) staff       (20)        0 2023-07-02 12:38:46.000000 ns_asphalt9-0.0.5/
+-rw-r--r--   0 sunhao     (501) staff       (20)    35149 2023-04-09 01:28:45.000000 ns_asphalt9-0.0.5/LICENSE
+-rw-r--r--   0 sunhao     (501) staff       (20)      180 2023-07-01 10:14:58.000000 ns_asphalt9-0.0.5/MANIFEST.in
+-rw-r--r--   0 sunhao     (501) staff       (20)     2276 2023-07-02 12:38:46.000000 ns_asphalt9-0.0.5/PKG-INFO
+-rw-r--r--   0 sunhao     (501) staff       (20)     1041 2023-05-15 13:28:06.000000 ns_asphalt9-0.0.5/README.md
+drwxr-xr-x   0 sunhao     (501) staff       (20)        0 2023-07-02 12:38:46.000000 ns_asphalt9-0.0.5/ns_asphalt9/
+drwxr-xr-x   0 sunhao     (501) staff       (20)        0 2023-07-02 12:38:46.000000 ns_asphalt9-0.0.5/ns_asphalt9/core/
+-rw-r--r--   0 sunhao     (501) staff       (20)       20 2023-07-01 10:14:58.000000 ns_asphalt9-0.0.5/ns_asphalt9/core/__init__.py
+drwxr-xr-x   0 sunhao     (501) staff       (20)        0 2023-07-02 12:38:46.000000 ns_asphalt9-0.0.5/ns_asphalt9/core/actions/
+-rw-r--r--   0 sunhao     (501) staff       (20)      208 2023-07-02 11:42:33.000000 ns_asphalt9-0.0.5/ns_asphalt9/core/actions/__init__.py
+-rw-r--r--   0 sunhao     (501) staff       (20)      336 2023-07-01 10:14:58.000000 ns_asphalt9-0.0.5/ns_asphalt9/core/actions/common.py
+-rw-r--r--   0 sunhao     (501) staff       (20)     4033 2023-07-02 12:16:45.000000 ns_asphalt9-0.0.5/ns_asphalt9/core/actions/enter_page.py
+-rw-r--r--   0 sunhao     (501) staff       (20)     3881 2023-07-02 05:05:14.000000 ns_asphalt9-0.0.5/ns_asphalt9/core/actions/process_race.py
+-rw-r--r--   0 sunhao     (501) staff       (20)     3777 2023-07-02 02:37:32.000000 ns_asphalt9-0.0.5/ns_asphalt9/core/actions/select_car.py
+-rw-r--r--   0 sunhao     (501) staff       (20)      706 2023-07-01 10:14:58.000000 ns_asphalt9-0.0.5/ns_asphalt9/core/cache.py
+-rw-r--r--   0 sunhao     (501) staff       (20)     2996 2023-07-02 12:30:27.000000 ns_asphalt9-0.0.5/ns_asphalt9/core/consts.py
+-rw-r--r--   0 sunhao     (501) staff       (20)     2146 2023-07-01 10:14:58.000000 ns_asphalt9-0.0.5/ns_asphalt9/core/controller.py
+-rw-r--r--   0 sunhao     (501) staff       (20)      634 2023-07-02 02:35:24.000000 ns_asphalt9-0.0.5/ns_asphalt9/core/globals.py
+drwxr-xr-x   0 sunhao     (501) staff       (20)        0 2023-07-02 12:38:46.000000 ns_asphalt9-0.0.5/ns_asphalt9/core/gui/
+-rw-r--r--   0 sunhao     (501) staff       (20)        0 2023-07-01 10:14:58.000000 ns_asphalt9-0.0.5/ns_asphalt9/core/gui/__init__.py
+-rw-r--r--   0 sunhao     (501) staff       (20)    18706 2023-07-02 12:06:23.000000 ns_asphalt9-0.0.5/ns_asphalt9/core/gui/app.py
+drwxr-xr-x   0 sunhao     (501) staff       (20)        0 2023-07-02 12:38:46.000000 ns_asphalt9-0.0.5/ns_asphalt9/core/gui/images/
+-rw-r--r--   0 sunhao     (501) staff       (20)     3097 2023-07-01 10:14:58.000000 ns_asphalt9-0.0.5/ns_asphalt9/core/gui/images/help.png
+-rw-r--r--   0 sunhao     (501) staff       (20)     2900 2023-07-01 10:14:58.000000 ns_asphalt9-0.0.5/ns_asphalt9/core/gui/images/home.png
+-rw-r--r--   0 sunhao     (501) staff       (20)   202347 2023-07-01 10:14:58.000000 ns_asphalt9-0.0.5/ns_asphalt9/core/gui/images/logo.png
+-rw-r--r--   0 sunhao     (501) staff       (20)     3159 2023-07-01 10:14:58.000000 ns_asphalt9-0.0.5/ns_asphalt9/core/gui/images/settings.png
+-rw-r--r--   0 sunhao     (501) staff       (20)     1530 2023-07-01 10:14:58.000000 ns_asphalt9-0.0.5/ns_asphalt9/core/ocr.py
+-rw-r--r--   0 sunhao     (501) staff       (20)     1841 2023-07-01 12:06:18.000000 ns_asphalt9-0.0.5/ns_asphalt9/core/page_factory.py
+-rw-r--r--   0 sunhao     (501) staff       (20)    12155 2023-07-02 12:33:09.000000 ns_asphalt9-0.0.5/ns_asphalt9/core/pages.py
+-rw-r--r--   0 sunhao     (501) staff       (20)      265 2023-07-01 10:14:58.000000 ns_asphalt9-0.0.5/ns_asphalt9/core/screenshot.py
+-rw-r--r--   0 sunhao     (501) staff       (20)     2572 2023-07-02 12:33:50.000000 ns_asphalt9-0.0.5/ns_asphalt9/core/tasks.py
+drwxr-xr-x   0 sunhao     (501) staff       (20)        0 2023-07-02 12:38:46.000000 ns_asphalt9-0.0.5/ns_asphalt9/core/utils/
+-rw-r--r--   0 sunhao     (501) staff       (20)        0 2023-07-01 10:14:58.000000 ns_asphalt9-0.0.5/ns_asphalt9/core/utils/__init__.py
+-rw-r--r--   0 sunhao     (501) staff       (20)     1016 2023-07-01 10:14:58.000000 ns_asphalt9-0.0.5/ns_asphalt9/core/utils/decorator.py
+-rw-r--r--   0 sunhao     (501) staff       (20)      459 2023-07-01 10:14:58.000000 ns_asphalt9-0.0.5/ns_asphalt9/core/utils/fetch_cars.py
+-rw-r--r--   0 sunhao     (501) staff       (20)     1993 2023-07-01 10:14:58.000000 ns_asphalt9-0.0.5/ns_asphalt9/core/utils/log.py
+-rw-r--r--   0 sunhao     (501) staff       (20)      862 2023-07-01 10:14:58.000000 ns_asphalt9-0.0.5/ns_asphalt9/core/utils/timer.py
+-rw-r--r--   0 sunhao     (501) staff       (20)     5558 2023-07-02 12:12:57.000000 ns_asphalt9-0.0.5/ns_asphalt9/main.py
+drwxr-xr-x   0 sunhao     (501) staff       (20)        0 2023-07-02 12:38:46.000000 ns_asphalt9-0.0.5/ns_asphalt9.egg-info/
+-rw-r--r--   0 sunhao     (501) staff       (20)     2276 2023-07-02 12:38:46.000000 ns_asphalt9-0.0.5/ns_asphalt9.egg-info/PKG-INFO
+-rw-r--r--   0 sunhao     (501) staff       (20)     1169 2023-07-02 12:38:46.000000 ns_asphalt9-0.0.5/ns_asphalt9.egg-info/SOURCES.txt
+-rw-r--r--   0 sunhao     (501) staff       (20)        1 2023-07-02 12:38:46.000000 ns_asphalt9-0.0.5/ns_asphalt9.egg-info/dependency_links.txt
+-rw-r--r--   0 sunhao     (501) staff       (20)       55 2023-07-02 12:38:46.000000 ns_asphalt9-0.0.5/ns_asphalt9.egg-info/entry_points.txt
+-rw-r--r--   0 sunhao     (501) staff       (20)        1 2023-07-02 12:38:46.000000 ns_asphalt9-0.0.5/ns_asphalt9.egg-info/not-zip-safe
+-rw-r--r--   0 sunhao     (501) staff       (20)      107 2023-07-02 12:38:46.000000 ns_asphalt9-0.0.5/ns_asphalt9.egg-info/requires.txt
+-rw-r--r--   0 sunhao     (501) staff       (20)       12 2023-07-02 12:38:46.000000 ns_asphalt9-0.0.5/ns_asphalt9.egg-info/top_level.txt
+-rw-r--r--   0 sunhao     (501) staff       (20)     1299 2023-07-02 12:38:46.000000 ns_asphalt9-0.0.5/setup.cfg
+-rw-r--r--   0 sunhao     (501) staff       (20)      387 2023-07-01 10:14:58.000000 ns_asphalt9-0.0.5/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `ns_asphalt9-0.0.4/LICENSE` & `ns_asphalt9-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.0.4/PKG-INFO` & `ns_asphalt9-0.0.5/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,57 +1,56 @@
 Metadata-Version: 2.1
 Name: ns_asphalt9
-Version: 0.0.4
+Version: 0.0.5
 Summary: Asphalt 9 daily task handling tool based on NXBT and V4L2.
 Home-page: https://pypi.python.org/pypi/ns_asphalt9
 Author: codehai
 Author-email: wmpksb@gmail.com
 License: GNU General Public License v3 (GPLv3)
 Project-URL: Code, https://github.com/codehai/ns_asphalt9
 Project-URL: Issue tracker, https://github.com/codehai/ns_asphalt9/issues
+Description: # ns_asphalt9 
+        
+        基于nxbt和v4l2实现了闭环控制的Asphalt9日常任务处理工具。
+        
+        
+        ### 硬件依赖
+            
+        1. **[HDMI采集卡(必选)](https://u.jd.com/bizS2eh)** 
+           
+           用于switch画面输入到虚拟机
+        
+        2. **蓝牙(必选)**
+           
+           用于模拟手柄向switch发消息,Linux环境下可用本机蓝牙，Mac，Windows，群晖虚拟机请买usb蓝牙，注意群晖请需要适用于群晖的免驱蓝牙。
+        
+        3. **[HDMI分配器一分二 一进二出(可选)](https://u.jd.com/bqzn2Ek )** 
+           
+           同时输出switch到显示器和采集卡，方便debug
+        
+        
+        ### 使用教程
+        
+        [Wiki](https://github.com/codehai/ns_asphalt9/wiki)
+        
+        
+        ### 免责声明
+        
+        ns_asphalt为python学习交流的开源非营利项目，仅作为程序员之间相互学交流之用，使用需严格遵守开源许可协议。严禁用于商业用途，禁止使用ns_asphalt进行任何盈利活动。对一切非法使用所产生的后果，我们概不负责。
+        
+        
+        ### 许可证
+        
+        ![GitHub](https://img.shields.io/github/license/codehai/ns_asphalt9.svg)
+        
 Platform: any
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.6
+Requires-Python: >= 3.6
 Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# ns_asphalt9 
-
-基于nxbt和v4l2实现了闭环控制的Asphalt9日常任务处理工具。
-
-
-### 硬件依赖
-    
-1. **[HDMI采集卡(必选)](https://u.jd.com/bizS2eh)** 
-   
-   用于switch画面输入到虚拟机
-
-2. **蓝牙(必选)**
-   
-   用于模拟手柄向switch发消息,Linux环境下可用本机蓝牙，Mac，Windows，群晖虚拟机请买usb蓝牙，注意群晖请需要适用于群晖的免驱蓝牙。
-
-3. **[HDMI分配器一分二 一进二出(可选)](https://u.jd.com/bqzn2Ek )** 
-   
-   同时输出switch到显示器和采集卡，方便debug
-
-
-### 使用教程
-
-[Wiki](https://github.com/codehai/ns_asphalt9/wiki)
-
-
-### 免责声明
-
-ns_asphalt为python学习交流的开源非营利项目，仅作为程序员之间相互学交流之用，使用需严格遵守开源许可协议。严禁用于商业用途，禁止使用ns_asphalt进行任何盈利活动。对一切非法使用所产生的后果，我们概不负责。
-
-
-### 许可证
-
-![GitHub](https://img.shields.io/github/license/codehai/ns_asphalt9.svg)
```

### Comparing `ns_asphalt9-0.0.4/README.md` & `ns_asphalt9-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.0.4/ns_asphalt9/core/actions/process_race.py` & `ns_asphalt9-0.0.5/ns_asphalt9/core/actions/process_race.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from .. import consts, globals, ocr
 from ..controller import Buttons, pro
 from ..utils.log import logger
 
 
 def process_race(race_mode=0):
+    logger.info(f"Start racing.")
     for i in range(60):
         progress = 0
         page = ocr.ocr_screen()
         if page.data and "progress" in page.data:
             progress = page.data["progress"] if page.data["progress"] else 0
         if race_mode == 1:
             if progress > 0 and progress < 22:
@@ -49,15 +50,15 @@
                         break
                     elif elapsed > 24 and elapsed < 43 or elapsed < 10:
                         pro.press_button(Buttons.Y, 0.7)
                         pro.press_button(Buttons.Y, 0)
                         time.sleep(3)
                     else:
                         time.sleep(0.5)
-        elif globals.MODE == "CAR_HUNT_APEX_AP0":
+        elif page.hunt_car == "APEX AP-0":
             if progress > 0:
                 start = time.perf_counter()
                 delta = progress * 0.55 + 4.5
                 while globals.G_RUN.is_set():
                     end = time.perf_counter()
                     elapsed = end - start + delta
                     logger.info(f"elapsed = {elapsed}")
@@ -78,12 +79,12 @@
                     else:
                         time.sleep(0.5)
 
         else:
             pro.press_button(Buttons.Y, 0.7)
             pro.press_button(Buttons.Y, 0)
 
-        if page.name in [consts.race_score, consts.race_results, consts.race_reward]:
+        if page.name in [consts.race_score, consts.race_results, consts.race_reward, consts.system_error]:
             break
 
     globals.FINISHED_COUNT += 1
     logger.info(f"Already finished {globals.FINISHED_COUNT} times loop count = {i}.")
```

### Comparing `ns_asphalt9-0.0.4/ns_asphalt9/core/actions/select_car.py` & `ns_asphalt9-0.0.5/ns_asphalt9/core/actions/select_car.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 import time
 
 from .. import consts, globals, tasks
 from ..actions import process_race
 from ..controller import Buttons, pro
 from ..ocr import ocr_screen
+from ..utils.log import logger
 
 
 def world_series_reset():
     division = globals.DIVISION
     if not division:
-        division = "BRONZE"
+        division = "青铜"
     config = globals.CONFIG["多人一"][division]
     level = config["车库等级"]
-    left_count_mapping = {"BRONZE": 4, "SILVER": 3, "GOLD": 2, "PLATINUM": 1}
+    left_count_mapping = {"青铜": 4, "白银": 3, "黄金": 2, "铂金": 1}
     pro.press_group([Buttons.DPAD_UP] * 4, 0)
     pro.press_group([Buttons.DPAD_RIGHT] * 6, 0)
     pro.press_group([Buttons.DPAD_LEFT] * 1, 0)
     pro.press_group([Buttons.DPAD_DOWN] * 1, 0)
     pro.press_group([Buttons.DPAD_LEFT] * left_count_mapping.get(level), 0)
     time.sleep(1)
     pro.press_a(2)
@@ -42,47 +43,51 @@
             positions.append({"row": row, "col": col})
     return positions
 
 
 def world_series_positions():
     division = globals.DIVISION
     if not division:
-        division = "BRONZE"
+        division = "青铜"
     config = globals.CONFIG["多人一"][division]
     return config["车库位置"]
 
 
 def other_series_position():
     return globals.CONFIG["多人二"]["车库位置"]
 
 
 def carhunt_position():
     return globals.CONFIG["寻车"]["车库位置"]
 
 
 def get_race_config():
-    task = consts.ModeTaskMapping.get(globals.MODE, globals.CONFIG["模式"])
-    if task == consts.other_series_zh:
-        return other_series_position(), other_series_reset
-    elif task == consts.car_hunt_zh:
-        return carhunt_position(), carhunt_reset
-    elif task == consts.world_series_zh:
-        return world_series_positions(), world_series_reset
+    mode = globals.MODE if globals.MODE else globals.CONFIG["模式"]
+    logger.info(f"Get mode {mode} config.")
+    if mode == consts.other_series_zh:
+        return other_series_position(), other_series_reset, mode
+    elif mode == consts.car_hunt_zh:
+        return carhunt_position(), carhunt_reset, mode
+    elif mode == consts.world_series_zh:
+        return world_series_positions(), world_series_reset, mode
     else:
-        return default_positions(), default_reset
+        return default_positions(), default_reset, mode
 
 
 def select_car():
     # 选车
+    logger.info("Start select car.")
     while globals.G_RUN.is_set():
-        positions, reset = get_race_config()
+        positions, reset, mode = get_race_config()
         reset()
-        if globals.SELECT_COUNT >= len(positions):
-            globals.SELECT_COUNT = 0
-        position = positions[globals.SELECT_COUNT]
+        if globals.SELECT_COUNT[mode] >= len(positions):
+            globals.SELECT_COUNT[mode] = 0
+        position = positions[globals.SELECT_COUNT[mode]]
+
+        logger.info(f"Start try position = {position}, count = {globals.SELECT_COUNT[mode]}")
 
         for i in range(position["row"] - 1):
             pro.press_button(Buttons.DPAD_DOWN, 0)
 
         for i in range(position["col"] - 1):
             pro.press_button(Buttons.DPAD_RIGHT, 0)
 
@@ -119,11 +124,11 @@
             ):
                 globals.DIVISION = ""
             for i in range(2):
                 pro.press_b()
                 page = ocr_screen()
                 if page.name == consts.select_car:
                     break
-            globals.SELECT_COUNT += 1
+            globals.SELECT_COUNT[mode] += 1
             continue
     process_race()
     tasks.TaskManager.set_done()
```

### Comparing `ns_asphalt9-0.0.4/ns_asphalt9/core/cache.py` & `ns_asphalt9-0.0.5/ns_asphalt9/core/cache.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.0.4/ns_asphalt9/core/consts.py` & `ns_asphalt9-0.0.5/ns_asphalt9/core/consts.py`

 * *Files 12% similar despite different names*

```diff
@@ -71,14 +71,18 @@
 club = "club"
 # 每日赛事
 daily_events = "daily_events"
 # 没匹配到对手
 no_opponents = "no_opponents"
 # 生涯
 career = "career"
+# 大奖赛
+grand_prix = "grand_prix"
+# 通行证页
+legend_pass = "legend_pass"
 
 
 # 键盘与手柄映射
 KEY_MAPPING = {
     "6": "MINUS",
     "7": "PLUS",
     "[": "CAPTURE",
@@ -93,14 +97,15 @@
     "d": "DPAD_RIGHT",
 }
 
 car_hunt_zh = "寻车"
 world_series_zh = "多人一"
 other_series_zh = "多人二"
 free_pack_zh = "免费抽卡"
+prix_pack_zh = "大奖赛抽卡"
 
 
 class Mode:
     car_hunt = "CAR HUNT"
     world_series = "WORLD SERIES"
     limited_series = "LIMITED SERIES"
     trial_series = "TRIAL SERIES"
@@ -116,12 +121,32 @@
 class TaskStatus:
     default = ""
     start = "start"
     done = "done"
 
 
 ModeTaskMapping = {
-    Mode.car_hunt: TaskName.car_hunt,
-    Mode.world_series: TaskName.world_series,
-    Mode.limited_series: TaskName.other_series,
-    Mode.trial_series: TaskName.other_series,
+    Mode.car_hunt: car_hunt_zh,
+    Mode.world_series: world_series_zh,
+    Mode.limited_series: other_series_zh,
+    Mode.trial_series: other_series_zh,
 }
+
+modes_zh = {
+    Mode.car_hunt: car_hunt_zh,
+    Mode.world_series: world_series_zh,
+    Mode.limited_series: other_series_zh,
+    Mode.trial_series: other_series_zh,
+}
+
+
+bronze = "BRONZE"
+silver = "SILVER"
+gold = "GOLD"
+platinum = "PLATINUM"
+
+divisions_zh = {
+    bronze: "青铜",
+    silver: "白银",
+    gold: "黄金",
+    platinum: "铂金"
+}
```

### Comparing `ns_asphalt9-0.0.4/ns_asphalt9/core/controller.py` & `ns_asphalt9-0.0.5/ns_asphalt9/core/controller.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.0.4/ns_asphalt9/core/gui/app.py` & `ns_asphalt9-0.0.5/ns_asphalt9/core/gui/app.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,23 +3,21 @@
 import tkinter
 
 import customtkinter
 from PIL import Image
 
 
 class App(customtkinter.CTk):
-    def __init__(self, queue):
+    def __init__(self, queue, config_name):
         super().__init__()
-
         self.queue = queue
-
         self.settings_data = None
-
-        if os.path.exists("settings.json"):
-            with open("settings.json", "r") as file:
+        self.config_file = f"{config_name}.json"
+        if os.path.exists(self.config_file):
+            with open(self.config_file, "r") as file:
                 self.settings_data = json.load(file)
 
         self.title("A9 AUTO")
         self.geometry("700x450")
 
         # set grid layout 1x2
         self.grid_rowconfigure(0, weight=1)
@@ -123,15 +121,15 @@
         self.setting_modules = {}
 
         # create settings frame
         self.settings = customtkinter.CTkScrollableFrame(
             self, corner_radius=0, fg_color="transparent"
         )
 
-        for row, label_text in enumerate(["模式", "任务", "多一", "多二", "寻车"]):
+        for row, label_text in enumerate(["模式", "任务", "多一", "多二", "寻车", "大奖赛"]):
             label = customtkinter.CTkLabel(master=self.settings, text=f"{label_text}:")
             label.grid(
                 row=row,
                 column=0,
                 columnspan=1,
                 padx=10,
                 pady=(20 if row == 0 else 10, 10),
@@ -369,14 +367,40 @@
 
             if self.settings_data:
                 option1.set(self.settings_data["寻车"]["车库位置"][r]["row"])
                 option2.set(self.settings_data["寻车"]["车库位置"][r]["col"])
 
             self.setting_modules["寻车"]["车库位置"].append({"row": option1, "col": option2})
 
+        # 大奖赛配置
+        self.setting_modules["大奖赛"] = {}
+        prix_setting_frame = customtkinter.CTkFrame(self.settings, width=340)
+        prix_setting_frame.grid(
+            row=5, column=1, columnspan=2, padx=(20, 0), pady=(20, 20), sticky="nsew"
+        )
+
+        prix_position = customtkinter.CTkLabel(
+            master=prix_setting_frame, text="位置:"
+        )
+        prix_position.grid(row=1, column=0, padx=(15, 10), pady=(10, 10))
+        prix_position_option = customtkinter.CTkOptionMenu(
+            prix_setting_frame,
+            dynamic_resizing=False,
+            values=[str(i) for i in range(0, 10)],
+            width=100,
+            height=28,
+            command=self.save_settings,
+        )
+
+        prix_position_option.grid(row=1, column=1, padx=(10, 10), pady=(10, 10))
+
+        if self.settings_data and "大奖赛" in self.settings_data:
+            prix_position_option.set(self.settings_data["大奖赛"]["位置"])
+        self.setting_modules["大奖赛"]["位置"] = prix_position_option
+
         # create third frame
         self.help = customtkinter.CTkFrame(
             self, corner_radius=0, fg_color="transparent"
         )
 
         # select default frame
         self.select_frame_by_name("home")
@@ -407,28 +431,30 @@
                 return objs
             else:
                 return objs.get()
 
         def convert_dict_values(data):
             if isinstance(data, dict):
                 for key, value in data.items():
+                    if key == "车库位置":
+                        data[key] = [v for v in value if int(v["col"]) and int(v["row"])]
                     if isinstance(value, str) and value.isdigit():
                         data[key] = int(value)
-                    elif isinstance(value, (dict, list)):
+                    if isinstance(value, (dict, list)):
                         convert_dict_values(value)  # 递归调用
             elif isinstance(data, list):
                 for i, item in enumerate(data):
                     if isinstance(item, str) and item.isdigit():
                         data[i] = int(item)
                     elif isinstance(item, (dict, list)):
                         convert_dict_values(item)  # 递归调用
 
         res = get_value(self.setting_modules)
         self.settings_data = res
-        with open("settings.json", "w") as file:
+        with open(self.config_file, "w") as file:
             file.write(json.dumps(res, indent=2, ensure_ascii=False))
         convert_dict_values(res)
         self.queue.put(res)
 
     def select_frame_by_name(self, name):
         # set button color for selected button
         self.home_button.configure(
```

### Comparing `ns_asphalt9-0.0.4/ns_asphalt9/core/gui/images/help.png` & `ns_asphalt9-0.0.5/ns_asphalt9/core/gui/images/help.png`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.0.4/ns_asphalt9/core/gui/images/home.png` & `ns_asphalt9-0.0.5/ns_asphalt9/core/gui/images/home.png`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.0.4/ns_asphalt9/core/gui/images/logo.png` & `ns_asphalt9-0.0.5/ns_asphalt9/core/gui/images/logo.png`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.0.4/ns_asphalt9/core/gui/images/settings.png` & `ns_asphalt9-0.0.5/ns_asphalt9/core/gui/images/settings.png`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.0.4/ns_asphalt9/core/ocr.py` & `ns_asphalt9-0.0.5/ns_asphalt9/core/ocr.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.0.4/ns_asphalt9/core/page_factory.py` & `ns_asphalt9-0.0.5/ns_asphalt9/core/page_factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,36 +20,37 @@
                 if last_page_name == consts.racing:
                     weight += 1
                 match_pages.append((page_instance, weight))
 
         match_pages.sort(key=lambda pages: pages[1], reverse=True)
 
         if last_page_name in [consts.loading_race, consts.racing] and not match_pages:
-            match_pages.append((self.last_page, 1))
+            match_pages.append((pages.Racing, 1))
 
         if (
             not match_pages
             and text
             or len(match_pages) >= 2
             and match_pages[0][1] == match_pages[1][1]
         ):
             logger.info(f"match_pages = {match_pages}")
             self.capture()
 
         if match_pages:
             page = match_pages[0][0](text, self.last_page)
-            methods = [
-                method for method in dir(page) if callable(getattr(page, method))
-            ]
-            for method in methods:
-                if method.startswith("parse"):
-                    func = getattr(page, method)
-                    func()
-            return page
-        page = pages.Empty(text, self.last_page)
+        else:
+            page = pages.Empty(text, self.last_page)
+        methods = [
+            method for method in dir(page) if callable(getattr(page, method))
+        ]
+        for method in methods:
+            if method.startswith("parse"):
+                func = getattr(page, method)
+                func()
+        self.last_page = page
         return page
 
     def capture(self):
         debug = os.environ.get("A9_DEBUG", 0)
         filename = (
             "".join([str(d) for d in datetime.datetime.now().timetuple()]) + ".jpg"
         )
```

### Comparing `ns_asphalt9-0.0.4/ns_asphalt9/core/pages.py` & `ns_asphalt9-0.0.5/ns_asphalt9/core/pages.py`

 * *Files 23% similar despite different names*

```diff
@@ -7,44 +7,50 @@
 
 
 class Page:
     text = None
     name = None
     data = None
     mode = None
+    hunt_car = None
     division = None
     touchdriver = None
 
     feature = ""
     part_match = False
 
     action = None
     args = ()
 
     def __init__(self, text: str, last_page: "Page" = None) -> None:
         if last_page:
             self.mode = last_page.mode
             self.division = last_page.division
             self.touchdriver = last_page.touchdriver
+            self.hunt_car = last_page.hunt_car
         self.text = text
 
     def parse_common(self):
         divisions = re.findall("BRONZE|SILVER|GOLD|PLATINUM", self.text)
         if divisions and self.name in [
             consts.world_series,
             consts.searching,
             consts.loading_race,
         ]:
-            self.division = divisions[0]
+            self.division = consts.divisions_zh.get(divisions[0], "")
 
         modes = re.findall(
             "CAR HUNT|WORLD SERIES|LIMITED SERIES|TRIAL SERIES", self.text
         )
         if modes and self.name not in [consts.multi_player]:
-            self.mode = modes[0]
+            self.mode = consts.modes_zh.get(modes[0], "")
+            if self.mode == consts.car_hunt_zh:
+                hunt_cars = re.findall("APEX AP-0", self.text)
+                if hunt_cars:
+                    self.hunt_car = hunt_cars[0]
 
         if "TOUCHDRIVE ON" in self.text:
             self.touchdriver = 1
         if "TOUCHDRIVE OFF" in self.text:
             self.touchdriver = 0
 
     @classmethod
@@ -270,15 +276,15 @@
 class Demoted(Page):
     """降级"""
 
     name = consts.demoted
     feature = "DEMOTED"
     part_match = False
 
-    action = actions.demoted
+    action = staticmethod(actions.demoted)
 
 
 @cache_decorator("page")
 class Disconnected(Page):
     """断开连接"""
 
     name = consts.disconnected
@@ -329,36 +335,57 @@
 
     name = consts.race_results
     feature = "RACE RESULTS|POS\.|PLAYER|CAR NAME|NEXT"
     part_match = True
     action = staticmethod(pro.press_button)
     args = (Buttons.A,)
 
+    @classmethod
+    def calc_weight(cls, text: str) -> int:
+        match_count = len(re.findall(cls.feature, text))
+        if "RACE RESULTS" in text:
+            match_count = 10
+        return match_count
+
 
 @cache_decorator("page")
 class RaceScore(Page):
     """比赛成绩"""
 
     name = consts.race_score
     feature = "WINNER|YOUR POSITION|YOUR TIME|RATING|NEXT"
     part_match = True
     action = staticmethod(pro.press_button)
     args = (Buttons.A,)
 
+    @classmethod
+    def calc_weight(cls, text: str) -> int:
+        match_count = len(re.findall(cls.feature, text))
+        if "WINNER" in text:
+            match_count = 10
+        return match_count
+
 
 @cache_decorator("page")
 class RaceReward(Page):
     """比赛奖励"""
 
     name = consts.race_reward
     feature = "RACE|REWARDS|REPUTATION|TOTAL|CREDITS|NEXT"
     part_match = True
     action = staticmethod(pro.press_button)
     args = (Buttons.A,)
 
+    @classmethod
+    def calc_weight(cls, text: str) -> int:
+        match_count = len(re.findall(cls.feature, text))
+        if "RACE REWARDS" in text:
+            match_count = 10
+        return match_count
+
 
 @cache_decorator("page")
 class MilestoneReward(Page):
     """里程碑奖励"""
 
     name = consts.milestone_reward
     feature = "CONGRATULATIONS"
@@ -494,7 +521,25 @@
 @cache_decorator("page")
 class Career(Page):
     """生涯"""
 
     name = consts.career
     feature = "COLLECTED.*CAREER"
     part_match = False
+
+
+@cache_decorator("page")
+class GrandPrix(Page):
+    """大奖赛抽卡"""
+
+    name = consts.grand_prix
+    feature = "GP Standings"
+    part_match = False
+
+
+@cache_decorator("page")
+class LegendPass(Page):
+    """通行证页"""
+
+    name = consts.legend_pass
+    feature = "ENDS IN|CURRENT TIER|GARAGE|GRANTS UP TO"
+    part_match = True
```

### Comparing `ns_asphalt9-0.0.4/ns_asphalt9/core/tasks.py` & `ns_asphalt9-0.0.5/ns_asphalt9/core/tasks.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import threading
 
-from . import consts, globals
-from .actions import enter_carhunt, enter_series, free_pack
+from . import consts, globals, actions
 from .utils.log import logger
 
 
 class TaskManager:
     timers = []
     status = consts.TaskStatus.default
     current_task = ""
@@ -40,14 +39,15 @@
 
         if page.name not in [
             consts.world_series,
             consts.limited_series,
             consts.trial_series,
             consts.carhunt,
             consts.card_pack,
+            consts.legend_pass
         ]:
             return False
 
         if globals.task_queue.empty():
             if cls.status == consts.TaskStatus.done:
                 cls.task_enter(globals.CONFIG["模式"], page=page)
                 cls.status = consts.TaskStatus.default
@@ -60,20 +60,22 @@
             cls.task_enter(task, page)
             return True
 
     @classmethod
     def task_enter(cls, task, page=None) -> None:
         logger.info(f"Start process {task} task.")
         if task == consts.world_series_zh:
-            enter_series(page=page)
+            actions.enter_series(page=page)
         if task == consts.other_series_zh:
-            enter_series(task=task, page=page)
+            actions.enter_series(mode=task, page=page)
         if task == consts.car_hunt_zh:
-            enter_carhunt(page=page)
+            actions.enter_carhunt(page=page)
         if task == consts.free_pack_zh:
-            free_pack()
+            actions.free_pack()
+        if task == consts.prix_pack_zh:
+            actions.prix_pack()
 
     @classmethod
     def set_done(cls) -> None:
         if cls.status == consts.TaskStatus.start:
             cls.status = consts.TaskStatus.done
             cls.current_task = ""
```

### Comparing `ns_asphalt9-0.0.4/ns_asphalt9/core/utils/decorator.py` & `ns_asphalt9-0.0.5/ns_asphalt9/core/utils/decorator.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.0.4/ns_asphalt9/core/utils/log.py` & `ns_asphalt9-0.0.5/ns_asphalt9/core/utils/log.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.0.4/ns_asphalt9/core/utils/timer.py` & `ns_asphalt9-0.0.5/ns_asphalt9/core/utils/timer.py`

 * *Files identical despite different names*

### Comparing `ns_asphalt9-0.0.4/ns_asphalt9/main.py` & `ns_asphalt9-0.0.5/ns_asphalt9/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,21 @@
+import argparse
 import datetime
 import multiprocessing
 import os
 import shutil
 import threading
 import time
 import traceback
 import types
 
 from .core import consts
 from .core import globals as G
+from .core.actions import (enter_carhunt, enter_game, enter_series, free_pack,
+                           prix_pack)
 from .core.controller import Buttons, pro
 from .core.gui.app import App
 from .core.ocr import ocr_screen
 from .core.pages import Page
 from .core.screenshot import screenshot
 from .core.tasks import TaskManager
 from .core.utils.log import logger
@@ -97,27 +100,28 @@
                 for timer in TaskManager.timers:
                     timer.cancel()
 
             elif command in consts.KEY_MAPPING:
                 # 手柄操作
                 control_data = consts.KEY_MAPPING.get(command)
                 if isinstance(control_data, str):
-                    pro.press_buttons(control_data)
+                    pro.press_button(control_data, 0)
                     screenshot()
                 if isinstance(control_data, types.FunctionType):
                     control_data()
             else:
                 global_vars = globals()
                 func = global_vars.get(command, "")
                 if isinstance(func, types.FunctionType):
                     func()
                 else:
                     logger.info(f"{command} command not support!")
 
         elif isinstance(command, dict):
+            logger.info("Received config update message.")
             G.CONFIG = command
 
         else:
             logger.info(f"{command} command not support!")
 
 
 def start_command_input(queue):
@@ -161,18 +165,27 @@
 def on_closing(app):
     G.G_RUN.clear()
     logger.info(f"G_RUN state {G.G_RUN.is_set()}")
     G.output_queue.put("Quit App.")
     app.destroy()
 
 
+def init_config():
+
+    parser = argparse.ArgumentParser(description="NS Asphalt9 Tool.")
+    parser.add_argument("-c", "--config", type=str, default="settings", help="自定义配置文件")
+    args = parser.parse_args()
+    return args.config
+
+
 def main():
     G.G_OUT_WORKER.set()
+    config_name = init_config()
     start_worker()
-    app = App(G.input_queue)
+    app = App(G.input_queue, config_name)
     start_output_worker(app)
     app.protocol("WM_DELETE_WINDOW", lambda: on_closing(app))
     app.mainloop()
     print("App quit quit.")
 
 
 if __name__ == "__main__":
```

### Comparing `ns_asphalt9-0.0.4/ns_asphalt9.egg-info/PKG-INFO` & `ns_asphalt9-0.0.5/ns_asphalt9.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,57 +1,56 @@
 Metadata-Version: 2.1
 Name: ns-asphalt9
-Version: 0.0.4
+Version: 0.0.5
 Summary: Asphalt 9 daily task handling tool based on NXBT and V4L2.
 Home-page: https://pypi.python.org/pypi/ns_asphalt9
 Author: codehai
 Author-email: wmpksb@gmail.com
 License: GNU General Public License v3 (GPLv3)
 Project-URL: Code, https://github.com/codehai/ns_asphalt9
 Project-URL: Issue tracker, https://github.com/codehai/ns_asphalt9/issues
+Description: # ns_asphalt9 
+        
+        基于nxbt和v4l2实现了闭环控制的Asphalt9日常任务处理工具。
+        
+        
+        ### 硬件依赖
+            
+        1. **[HDMI采集卡(必选)](https://u.jd.com/bizS2eh)** 
+           
+           用于switch画面输入到虚拟机
+        
+        2. **蓝牙(必选)**
+           
+           用于模拟手柄向switch发消息,Linux环境下可用本机蓝牙，Mac，Windows，群晖虚拟机请买usb蓝牙，注意群晖请需要适用于群晖的免驱蓝牙。
+        
+        3. **[HDMI分配器一分二 一进二出(可选)](https://u.jd.com/bqzn2Ek )** 
+           
+           同时输出switch到显示器和采集卡，方便debug
+        
+        
+        ### 使用教程
+        
+        [Wiki](https://github.com/codehai/ns_asphalt9/wiki)
+        
+        
+        ### 免责声明
+        
+        ns_asphalt为python学习交流的开源非营利项目，仅作为程序员之间相互学交流之用，使用需严格遵守开源许可协议。严禁用于商业用途，禁止使用ns_asphalt进行任何盈利活动。对一切非法使用所产生的后果，我们概不负责。
+        
+        
+        ### 许可证
+        
+        ![GitHub](https://img.shields.io/github/license/codehai/ns_asphalt9.svg)
+        
 Platform: any
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.6
+Requires-Python: >= 3.6
 Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# ns_asphalt9 
-
-基于nxbt和v4l2实现了闭环控制的Asphalt9日常任务处理工具。
-
-
-### 硬件依赖
-    
-1. **[HDMI采集卡(必选)](https://u.jd.com/bizS2eh)** 
-   
-   用于switch画面输入到虚拟机
-
-2. **蓝牙(必选)**
-   
-   用于模拟手柄向switch发消息,Linux环境下可用本机蓝牙，Mac，Windows，群晖虚拟机请买usb蓝牙，注意群晖请需要适用于群晖的免驱蓝牙。
-
-3. **[HDMI分配器一分二 一进二出(可选)](https://u.jd.com/bqzn2Ek )** 
-   
-   同时输出switch到显示器和采集卡，方便debug
-
-
-### 使用教程
-
-[Wiki](https://github.com/codehai/ns_asphalt9/wiki)
-
-
-### 免责声明
-
-ns_asphalt为python学习交流的开源非营利项目，仅作为程序员之间相互学交流之用，使用需严格遵守开源许可协议。严禁用于商业用途，禁止使用ns_asphalt进行任何盈利活动。对一切非法使用所产生的后果，我们概不负责。
-
-
-### 许可证
-
-![GitHub](https://img.shields.io/github/license/codehai/ns_asphalt9.svg)
```

### Comparing `ns_asphalt9-0.0.4/ns_asphalt9.egg-info/SOURCES.txt` & `ns_asphalt9-0.0.5/ns_asphalt9.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -32,9 +32,8 @@
 ns_asphalt9/core/gui/images/home.png
 ns_asphalt9/core/gui/images/logo.png
 ns_asphalt9/core/gui/images/settings.png
 ns_asphalt9/core/utils/__init__.py
 ns_asphalt9/core/utils/decorator.py
 ns_asphalt9/core/utils/fetch_cars.py
 ns_asphalt9/core/utils/log.py
-ns_asphalt9/core/utils/timer.py
-tests/test_ocr.py
+ns_asphalt9/core/utils/timer.py
```

### Comparing `ns_asphalt9-0.0.4/setup.cfg` & `ns_asphalt9-0.0.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = nxbt
-version = 0.0.4
+version = 0.0.5
 author = codehai
 author-email = wmpksb@gmail.com
 project_urls = 
 	Code = https://github.com/codehai/ns_asphalt9
 	Issue tracker = https://github.com/codehai/ns_asphalt9/issues
 license = GNU General Public License v3 (GPLv3)
 license-file = LICENSE
```

