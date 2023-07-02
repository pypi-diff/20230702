# Comparing `tmp/alibabacloud_rds20140815_py2-1.1.1.tar.gz` & `tmp/alibabacloud_rds20140815_py2-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_rds20140815_py2-1.1.1.tar", last modified: Sat Jul  1 15:13:26 2023, max compression
+gzip compressed data, was "dist/alibabacloud_rds20140815_py2-1.1.2.tar", last modified: Sun Jul  2 15:14:02 2023, max compression
```

## Comparing `alibabacloud_rds20140815_py2-1.1.1.tar` & `alibabacloud_rds20140815_py2-1.1.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 15:13:26.000000 alibabacloud_rds20140815_py2-1.1.1/
--rw-r--r--   0 root         (0) root         (0)      716 2023-07-01 15:13:26.000000 alibabacloud_rds20140815_py2-1.1.1/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      588 2023-07-01 15:13:26.000000 alibabacloud_rds20140815_py2-1.1.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2023-07-01 15:13:26.000000 alibabacloud_rds20140815_py2-1.1.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2472 2023-07-01 15:13:26.000000 alibabacloud_rds20140815_py2-1.1.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1033 2023-07-01 15:13:26.000000 alibabacloud_rds20140815_py2-1.1.1/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1116 2023-07-01 15:13:26.000000 alibabacloud_rds20140815_py2-1.1.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 15:13:26.000000 alibabacloud_rds20140815_py2-1.1.1/alibabacloud_rds20140815/
--rw-r--r--   0 root         (0) root         (0)       21 2023-07-01 15:13:26.000000 alibabacloud_rds20140815_py2-1.1.1/alibabacloud_rds20140815/__init__.py
--rw-r--r--   0 root         (0) root         (0)   752466 2023-07-01 15:13:26.000000 alibabacloud_rds20140815_py2-1.1.1/alibabacloud_rds20140815/client.py
--rw-r--r--   0 root         (0) root         (0)  2559473 2023-07-01 15:13:26.000000 alibabacloud_rds20140815_py2-1.1.1/alibabacloud_rds20140815/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 15:13:26.000000 alibabacloud_rds20140815_py2-1.1.1/alibabacloud_rds20140815_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2472 2023-07-01 15:13:26.000000 alibabacloud_rds20140815_py2-1.1.1/alibabacloud_rds20140815_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      440 2023-07-01 15:13:26.000000 alibabacloud_rds20140815_py2-1.1.1/alibabacloud_rds20140815_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-01 15:13:26.000000 alibabacloud_rds20140815_py2-1.1.1/alibabacloud_rds20140815_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2023-07-01 15:13:26.000000 alibabacloud_rds20140815_py2-1.1.1/alibabacloud_rds20140815_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2023-07-01 15:13:26.000000 alibabacloud_rds20140815_py2-1.1.1/alibabacloud_rds20140815_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-07-01 15:13:26.000000 alibabacloud_rds20140815_py2-1.1.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2903 2023-07-01 15:13:26.000000 alibabacloud_rds20140815_py2-1.1.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 15:14:02.000000 alibabacloud_rds20140815_py2-1.1.2/
+-rw-r--r--   0 root         (0) root         (0)      796 2023-07-02 15:14:02.000000 alibabacloud_rds20140815_py2-1.1.2/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2023-07-02 15:14:02.000000 alibabacloud_rds20140815_py2-1.1.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2023-07-02 15:14:02.000000 alibabacloud_rds20140815_py2-1.1.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2472 2023-07-02 15:14:02.000000 alibabacloud_rds20140815_py2-1.1.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1033 2023-07-02 15:14:02.000000 alibabacloud_rds20140815_py2-1.1.2/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1116 2023-07-02 15:14:02.000000 alibabacloud_rds20140815_py2-1.1.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 15:14:02.000000 alibabacloud_rds20140815_py2-1.1.2/alibabacloud_rds20140815/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-07-02 15:14:02.000000 alibabacloud_rds20140815_py2-1.1.2/alibabacloud_rds20140815/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   752466 2023-07-02 15:14:02.000000 alibabacloud_rds20140815_py2-1.1.2/alibabacloud_rds20140815/client.py
+-rw-r--r--   0 root         (0) root         (0)  2559473 2023-07-02 15:14:02.000000 alibabacloud_rds20140815_py2-1.1.2/alibabacloud_rds20140815/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 15:14:02.000000 alibabacloud_rds20140815_py2-1.1.2/alibabacloud_rds20140815_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2472 2023-07-02 15:14:02.000000 alibabacloud_rds20140815_py2-1.1.2/alibabacloud_rds20140815_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      440 2023-07-02 15:14:02.000000 alibabacloud_rds20140815_py2-1.1.2/alibabacloud_rds20140815_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-02 15:14:02.000000 alibabacloud_rds20140815_py2-1.1.2/alibabacloud_rds20140815_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2023-07-02 15:14:02.000000 alibabacloud_rds20140815_py2-1.1.2/alibabacloud_rds20140815_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2023-07-02 15:14:02.000000 alibabacloud_rds20140815_py2-1.1.2/alibabacloud_rds20140815_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-07-02 15:14:02.000000 alibabacloud_rds20140815_py2-1.1.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2903 2023-07-02 15:14:02.000000 alibabacloud_rds20140815_py2-1.1.2/setup.py
```

### Comparing `alibabacloud_rds20140815_py2-1.1.1/ChangeLog.md` & `alibabacloud_rds20140815_py2-1.1.2/ChangeLog.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+2023-07-01 Version: 1.1.1
+- Fixed bugs for lack of regionId.
+- Fix error code.
+
 2023-06-30 Version: 1.1.0
 - Fixed bugs for lack of regionId.
 - Fix error code.
 
 2023-06-30 Version: 1.0.9
 - ModifyBackupPolicy API support parameter BackupPriority.
 - DescribeBackupPolicy API add return parameters: BackupPriority and SupportModifyBackupPriority.
```

### Comparing `alibabacloud_rds20140815_py2-1.1.1/LICENSE` & `alibabacloud_rds20140815_py2-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_rds20140815_py2-1.1.1/PKG-INFO` & `alibabacloud_rds20140815_py2-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_rds20140815_py2
-Version: 1.1.1
+Version: 1.1.2
 Summary: Alibaba Cloud rds (20140815) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_rds20140815_py2-1.1.1/README-CN.md` & `alibabacloud_rds20140815_py2-1.1.2/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_rds20140815_py2-1.1.1/README.md` & `alibabacloud_rds20140815_py2-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_rds20140815_py2-1.1.1/alibabacloud_rds20140815/client.py` & `alibabacloud_rds20140815_py2-1.1.2/alibabacloud_rds20140815/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_rds20140815_py2-1.1.1/alibabacloud_rds20140815/models.py` & `alibabacloud_rds20140815_py2-1.1.2/alibabacloud_rds20140815/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_rds20140815_py2-1.1.1/alibabacloud_rds20140815_py2.egg-info/PKG-INFO` & `alibabacloud_rds20140815_py2-1.1.2/alibabacloud_rds20140815_py2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-rds20140815-py2
-Version: 1.1.1
+Version: 1.1.2
 Summary: Alibaba Cloud rds (20140815) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_rds20140815_py2-1.1.1/setup.py` & `alibabacloud_rds20140815_py2-1.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_rds20140815_py2.
 
-Created on 01/07/2023
+Created on 02/07/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_rds20140815"
 NAME = "alibabacloud_rds20140815_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud rds (20140815) SDK Library for Python2"
```

