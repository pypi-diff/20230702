# Comparing `tmp/alibabacloud_rds20140815-2.2.0.tar.gz` & `tmp/alibabacloud_rds20140815-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_rds20140815-2.2.0.tar", last modified: Sat Jul  1 15:14:07 2023, max compression
+gzip compressed data, was "dist/alibabacloud_rds20140815-2.2.1.tar", last modified: Sun Jul  2 15:15:24 2023, max compression
```

## Comparing `alibabacloud_rds20140815-2.2.0.tar` & `alibabacloud_rds20140815-2.2.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 15:14:07.000000 alibabacloud_rds20140815-2.2.0/
--rw-r--r--   0 root         (0) root         (0)     1127 2023-07-01 15:14:07.000000 alibabacloud_rds20140815-2.2.0/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2023-07-01 15:14:07.000000 alibabacloud_rds20140815-2.2.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-07-01 15:14:07.000000 alibabacloud_rds20140815-2.2.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2328 2023-07-01 15:14:07.000000 alibabacloud_rds20140815-2.2.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1022 2023-07-01 15:14:07.000000 alibabacloud_rds20140815-2.2.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1107 2023-07-01 15:14:07.000000 alibabacloud_rds20140815-2.2.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 15:14:07.000000 alibabacloud_rds20140815-2.2.0/alibabacloud_rds20140815/
--rw-r--r--   0 root         (0) root         (0)       21 2023-07-01 15:14:07.000000 alibabacloud_rds20140815-2.2.0/alibabacloud_rds20140815/__init__.py
--rw-r--r--   0 root         (0) root         (0)  1661565 2023-07-01 15:14:07.000000 alibabacloud_rds20140815-2.2.0/alibabacloud_rds20140815/client.py
--rw-r--r--   0 root         (0) root         (0)  2537409 2023-07-01 15:14:07.000000 alibabacloud_rds20140815-2.2.0/alibabacloud_rds20140815/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-01 15:14:07.000000 alibabacloud_rds20140815-2.2.0/alibabacloud_rds20140815.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2328 2023-07-01 15:14:07.000000 alibabacloud_rds20140815-2.2.0/alibabacloud_rds20140815.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      420 2023-07-01 15:14:07.000000 alibabacloud_rds20140815-2.2.0/alibabacloud_rds20140815.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-01 15:14:07.000000 alibabacloud_rds20140815-2.2.0/alibabacloud_rds20140815.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      156 2023-07-01 15:14:07.000000 alibabacloud_rds20140815-2.2.0/alibabacloud_rds20140815.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2023-07-01 15:14:07.000000 alibabacloud_rds20140815-2.2.0/alibabacloud_rds20140815.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-07-01 15:14:07.000000 alibabacloud_rds20140815-2.2.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2610 2023-07-01 15:14:07.000000 alibabacloud_rds20140815-2.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 15:15:24.000000 alibabacloud_rds20140815-2.2.1/
+-rw-r--r--   0 root         (0) root         (0)     1207 2023-07-02 15:15:24.000000 alibabacloud_rds20140815-2.2.1/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-07-02 15:15:24.000000 alibabacloud_rds20140815-2.2.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-07-02 15:15:24.000000 alibabacloud_rds20140815-2.2.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2328 2023-07-02 15:15:24.000000 alibabacloud_rds20140815-2.2.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1022 2023-07-02 15:15:24.000000 alibabacloud_rds20140815-2.2.1/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1107 2023-07-02 15:15:24.000000 alibabacloud_rds20140815-2.2.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 15:15:24.000000 alibabacloud_rds20140815-2.2.1/alibabacloud_rds20140815/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-07-02 15:15:24.000000 alibabacloud_rds20140815-2.2.1/alibabacloud_rds20140815/__init__.py
+-rw-r--r--   0 root         (0) root         (0)  1661565 2023-07-02 15:15:24.000000 alibabacloud_rds20140815-2.2.1/alibabacloud_rds20140815/client.py
+-rw-r--r--   0 root         (0) root         (0)  2537409 2023-07-02 15:15:24.000000 alibabacloud_rds20140815-2.2.1/alibabacloud_rds20140815/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 15:15:24.000000 alibabacloud_rds20140815-2.2.1/alibabacloud_rds20140815.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2328 2023-07-02 15:15:24.000000 alibabacloud_rds20140815-2.2.1/alibabacloud_rds20140815.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      420 2023-07-02 15:15:24.000000 alibabacloud_rds20140815-2.2.1/alibabacloud_rds20140815.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-02 15:15:24.000000 alibabacloud_rds20140815-2.2.1/alibabacloud_rds20140815.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      156 2023-07-02 15:15:24.000000 alibabacloud_rds20140815-2.2.1/alibabacloud_rds20140815.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2023-07-02 15:15:24.000000 alibabacloud_rds20140815-2.2.1/alibabacloud_rds20140815.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-07-02 15:15:24.000000 alibabacloud_rds20140815-2.2.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2610 2023-07-02 15:15:24.000000 alibabacloud_rds20140815-2.2.1/setup.py
```

### Comparing `alibabacloud_rds20140815-2.2.0/ChangeLog.md` & `alibabacloud_rds20140815-2.2.1/ChangeLog.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+2023-07-01 Version: 2.2.0
+- Fixed bugs for lack of regionId.
+- Fix error code.
+
 2023-06-30 Version: 2.1.9
 - Fixed bugs for lack of regionId.
 - Fix error code.
 
 2023-06-30 Version: 2.1.8
 - ModifyBackupPolicy API support parameter BackupPriority.
 - DescribeBackupPolicy API add return parameters: BackupPriority and SupportModifyBackupPriority.
```

### Comparing `alibabacloud_rds20140815-2.2.0/LICENSE` & `alibabacloud_rds20140815-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_rds20140815-2.2.0/PKG-INFO` & `alibabacloud_rds20140815-2.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_rds20140815
-Version: 2.2.0
+Version: 2.2.1
 Summary: Alibaba Cloud rds (20140815) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_rds20140815-2.2.0/README-CN.md` & `alibabacloud_rds20140815-2.2.1/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_rds20140815-2.2.0/README.md` & `alibabacloud_rds20140815-2.2.1/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_rds20140815-2.2.0/alibabacloud_rds20140815/client.py` & `alibabacloud_rds20140815-2.2.1/alibabacloud_rds20140815/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_rds20140815-2.2.0/alibabacloud_rds20140815/models.py` & `alibabacloud_rds20140815-2.2.1/alibabacloud_rds20140815/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_rds20140815-2.2.0/alibabacloud_rds20140815.egg-info/PKG-INFO` & `alibabacloud_rds20140815-2.2.1/alibabacloud_rds20140815.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-rds20140815
-Version: 2.2.0
+Version: 2.2.1
 Summary: Alibaba Cloud rds (20140815) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_rds20140815-2.2.0/setup.py` & `alibabacloud_rds20140815-2.2.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_rds20140815.
 
-Created on 01/07/2023
+Created on 02/07/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_rds20140815"
 NAME = "alibabacloud_rds20140815" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud rds (20140815) SDK Library for Python"
```

