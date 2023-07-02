# Comparing `tmp/approval_utilities-8.2.5.tar.gz` & `tmp/approval_utilities-8.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "approval_utilities-8.2.5.tar", last modified: Sun Mar 26 17:58:48 2023, max compression
+gzip compressed data, was "approval_utilities-8.3.0.tar", last modified: Sun Jul  2 05:59:54 2023, max compression
```

## Comparing `approval_utilities-8.2.5.tar` & `approval_utilities-8.3.0.tar`

### file list

```diff
@@ -1,48 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 17:58:48.138859 approval_utilities-8.2.5/
--rw-r--r--   0 runner    (1001) docker     (123)    10273 2023-03-26 17:58:35.000000 approval_utilities-8.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-03-26 17:58:35.000000 approval_utilities-8.2.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-03-26 17:58:48.138859 approval_utilities-8.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12482 2023-03-26 17:58:35.000000 approval_utilities-8.2.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 17:58:48.134859 approval_utilities-8.2.5/approval_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-26 17:58:35.000000 approval_utilities-8.2.5/approval_utilities/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 17:58:48.134859 approval_utilities-8.2.5/approval_utilities/approvaltests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-26 17:58:35.000000 approval_utilities-8.2.5/approval_utilities/approvaltests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 17:58:48.138859 approval_utilities-8.2.5/approval_utilities/approvaltests/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-26 17:58:35.000000 approval_utilities-8.2.5/approval_utilities/approvaltests/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-03-26 17:58:35.000000 approval_utilities-8.2.5/approval_utilities/approvaltests/core/verifiable.py
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-03-26 17:58:35.000000 approval_utilities-8.2.5/approval_utilities/approvaltests/core/verify_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-03-26 17:58:35.000000 approval_utilities-8.2.5/approval_utilities/list_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 17:58:48.138859 approval_utilities-8.2.5/approval_utilities/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-26 17:58:35.000000 approval_utilities-8.2.5/approval_utilities/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-03-26 17:58:35.000000 approval_utilities-8.2.5/approval_utilities/utilities/clipboard_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-03-26 17:58:35.000000 approval_utilities-8.2.5/approval_utilities/utilities/deprecated.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 17:58:48.138859 approval_utilities-8.2.5/approval_utilities/utilities/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-26 17:58:35.000000 approval_utilities-8.2.5/approval_utilities/utilities/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-03-26 17:58:35.000000 approval_utilities-8.2.5/approval_utilities/utilities/exceptions/exception_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-03-26 17:58:35.000000 approval_utilities-8.2.5/approval_utilities/utilities/exceptions/exception_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-03-26 17:58:35.000000 approval_utilities-8.2.5/approval_utilities/utilities/exceptions/multiple_exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 17:58:48.138859 approval_utilities-8.2.5/approval_utilities/utilities/logger/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-26 17:58:35.000000 approval_utilities-8.2.5/approval_utilities/utilities/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7505 2023-03-26 17:58:35.000000 approval_utilities-8.2.5/approval_utilities/utilities/logger/logging_instance.py
--rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-03-26 17:58:35.000000 approval_utilities-8.2.5/approval_utilities/utilities/logger/simple_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-03-26 17:58:35.000000 approval_utilities-8.2.5/approval_utilities/utilities/map_reduce.py
--rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-03-26 17:58:35.000000 approval_utilities-8.2.5/approval_utilities/utilities/markdown_table.py
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-03-26 17:58:35.000000 approval_utilities-8.2.5/approval_utilities/utilities/multiline_string_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-03-26 17:58:35.000000 approval_utilities-8.2.5/approval_utilities/utilities/os_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-03-26 17:58:35.000000 approval_utilities-8.2.5/approval_utilities/utilities/stack_frame_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-03-26 17:58:35.000000 approval_utilities-8.2.5/approval_utilities/utilities/string_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-03-26 17:58:35.000000 approval_utilities-8.2.5/approval_utilities/utilities/time_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-03-26 17:58:35.000000 approval_utilities-8.2.5/approval_utilities/utilities/wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-03-26 17:58:35.000000 approval_utilities-8.2.5/approval_utilities/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 17:58:48.134859 approval_utilities-8.2.5/approval_utilities.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-03-26 17:58:48.000000 approval_utilities-8.2.5/approval_utilities.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-03-26 17:58:48.000000 approval_utilities-8.2.5/approval_utilities.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-26 17:58:48.000000 approval_utilities-8.2.5/approval_utilities.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-03-26 17:58:48.000000 approval_utilities-8.2.5/approval_utilities.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-03-26 17:58:35.000000 approval_utilities-8.2.5/requirements.prod.extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-03-26 17:58:35.000000 approval_utilities-8.2.5/requirements.prod.required.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-03-26 17:58:35.000000 approval_utilities-8.2.5/requirements.prod.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-03-26 17:58:48.138859 approval_utilities-8.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-03-26 17:58:47.000000 approval_utilities-8.2.5/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-03-26 17:58:35.000000 approval_utilities-8.2.5/setup_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-03-26 17:58:46.000000 approval_utilities-8.2.5/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 05:59:54.937053 approval_utilities-8.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10273 2023-07-02 05:59:43.000000 approval_utilities-8.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-02 05:59:43.000000 approval_utilities-8.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-07-02 05:59:54.937053 approval_utilities-8.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12482 2023-07-02 05:59:43.000000 approval_utilities-8.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 05:59:54.937053 approval_utilities-8.3.0/approval_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 05:59:43.000000 approval_utilities-8.3.0/approval_utilities/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 05:59:54.937053 approval_utilities-8.3.0/approval_utilities/approvaltests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 05:59:43.000000 approval_utilities-8.3.0/approval_utilities/approvaltests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 05:59:54.937053 approval_utilities-8.3.0/approval_utilities/approvaltests/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 05:59:43.000000 approval_utilities-8.3.0/approval_utilities/approvaltests/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-02 05:59:43.000000 approval_utilities-8.3.0/approval_utilities/approvaltests/core/executable_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-02 05:59:43.000000 approval_utilities-8.3.0/approval_utilities/approvaltests/core/verifiable.py
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-02 05:59:43.000000 approval_utilities-8.3.0/approval_utilities/approvaltests/core/verify_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-07-02 05:59:43.000000 approval_utilities-8.3.0/approval_utilities/list_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 05:59:54.937053 approval_utilities-8.3.0/approval_utilities/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 05:59:43.000000 approval_utilities-8.3.0/approval_utilities/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-02 05:59:43.000000 approval_utilities-8.3.0/approval_utilities/utilities/clipboard_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-07-02 05:59:43.000000 approval_utilities-8.3.0/approval_utilities/utilities/deprecated.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 05:59:54.937053 approval_utilities-8.3.0/approval_utilities/utilities/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 05:59:43.000000 approval_utilities-8.3.0/approval_utilities/utilities/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-02 05:59:43.000000 approval_utilities-8.3.0/approval_utilities/utilities/exceptions/exception_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-02 05:59:43.000000 approval_utilities-8.3.0/approval_utilities/utilities/exceptions/exception_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-02 05:59:43.000000 approval_utilities-8.3.0/approval_utilities/utilities/exceptions/multiple_exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 05:59:54.937053 approval_utilities-8.3.0/approval_utilities/utilities/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 05:59:43.000000 approval_utilities-8.3.0/approval_utilities/utilities/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7505 2023-07-02 05:59:43.000000 approval_utilities-8.3.0/approval_utilities/utilities/logger/logging_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-07-02 05:59:43.000000 approval_utilities-8.3.0/approval_utilities/utilities/logger/simple_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-02 05:59:43.000000 approval_utilities-8.3.0/approval_utilities/utilities/map_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-07-02 05:59:43.000000 approval_utilities-8.3.0/approval_utilities/utilities/markdown_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-02 05:59:43.000000 approval_utilities-8.3.0/approval_utilities/utilities/multiline_string_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-02 05:59:43.000000 approval_utilities-8.3.0/approval_utilities/utilities/os_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 05:59:54.937053 approval_utilities-8.3.0/approval_utilities/utilities/persistence/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 05:59:43.000000 approval_utilities-8.3.0/approval_utilities/utilities/persistence/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-07-02 05:59:43.000000 approval_utilities-8.3.0/approval_utilities/utilities/persistence/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-02 05:59:43.000000 approval_utilities-8.3.0/approval_utilities/utilities/persistence/saver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-02 05:59:43.000000 approval_utilities-8.3.0/approval_utilities/utilities/stack_frame_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-02 05:59:43.000000 approval_utilities-8.3.0/approval_utilities/utilities/string_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-07-02 05:59:43.000000 approval_utilities-8.3.0/approval_utilities/utilities/time_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-07-02 05:59:43.000000 approval_utilities-8.3.0/approval_utilities/utilities/wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-07-02 05:59:43.000000 approval_utilities-8.3.0/approval_utilities/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 05:59:54.937053 approval_utilities-8.3.0/approval_utilities.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-07-02 05:59:54.000000 approval_utilities-8.3.0/approval_utilities.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-07-02 05:59:54.000000 approval_utilities-8.3.0/approval_utilities.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 05:59:54.000000 approval_utilities-8.3.0/approval_utilities.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-02 05:59:54.000000 approval_utilities-8.3.0/approval_utilities.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-07-02 05:59:43.000000 approval_utilities-8.3.0/requirements.prod.extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-02 05:59:43.000000 approval_utilities-8.3.0/requirements.prod.required.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-02 05:59:43.000000 approval_utilities-8.3.0/requirements.prod.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-02 05:59:54.937053 approval_utilities-8.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-07-02 05:59:54.000000 approval_utilities-8.3.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-07-02 05:59:43.000000 approval_utilities-8.3.0/setup_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-02 05:59:53.000000 approval_utilities-8.3.0/version.py
```

### Comparing `approval_utilities-8.2.5/LICENSE` & `approval_utilities-8.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `approval_utilities-8.2.5/PKG-INFO` & `approval_utilities-8.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: approval_utilities
-Version: 8.2.5
+Version: 8.3.0
 Summary: Utilities for your production code that work well with approvaltests
 Home-page: https://github.com/approvals/ApprovalTests.Python
 Author: ApprovalTests Contributors
 Author-email: llewellyn.falco@gmail.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `approval_utilities-8.2.5/README.md` & `approval_utilities-8.3.0/README.md`

 * *Files identical despite different names*

### Comparing `approval_utilities-8.2.5/approval_utilities/list_utils.py` & `approval_utilities-8.3.0/approval_utilities/list_utils.py`

 * *Files identical despite different names*

### Comparing `approval_utilities-8.2.5/approval_utilities/utilities/deprecated.py` & `approval_utilities-8.3.0/approval_utilities/utilities/deprecated.py`

 * *Files identical despite different names*

### Comparing `approval_utilities-8.2.5/approval_utilities/utilities/exceptions/exception_collector.py` & `approval_utilities-8.3.0/approval_utilities/utilities/exceptions/exception_collector.py`

 * *Files identical despite different names*

### Comparing `approval_utilities-8.2.5/approval_utilities/utilities/logger/logging_instance.py` & `approval_utilities-8.3.0/approval_utilities/utilities/logger/logging_instance.py`

 * *Files identical despite different names*

### Comparing `approval_utilities-8.2.5/approval_utilities/utilities/logger/simple_logger.py` & `approval_utilities-8.3.0/approval_utilities/utilities/logger/simple_logger.py`

 * *Files identical despite different names*

### Comparing `approval_utilities-8.2.5/approval_utilities/utilities/markdown_table.py` & `approval_utilities-8.3.0/approval_utilities/utilities/markdown_table.py`

 * *Files identical despite different names*

### Comparing `approval_utilities-8.2.5/approval_utilities/utilities/time_utilities.py` & `approval_utilities-8.3.0/approval_utilities/utilities/time_utilities.py`

 * *Files identical despite different names*

### Comparing `approval_utilities-8.2.5/approval_utilities/utilities/wrapper.py` & `approval_utilities-8.3.0/approval_utilities/utilities/wrapper.py`

 * *Files identical despite different names*

### Comparing `approval_utilities-8.2.5/approval_utilities/utils.py` & `approval_utilities-8.3.0/approval_utilities/utils.py`

 * *Files identical despite different names*

### Comparing `approval_utilities-8.2.5/approval_utilities.egg-info/PKG-INFO` & `approval_utilities-8.3.0/approval_utilities.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: approval-utilities
-Version: 8.2.5
+Version: 8.3.0
 Summary: Utilities for your production code that work well with approvaltests
 Home-page: https://github.com/approvals/ApprovalTests.Python
 Author: ApprovalTests Contributors
 Author-email: llewellyn.falco@gmail.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `approval_utilities-8.2.5/approval_utilities.egg-info/SOURCES.txt` & `approval_utilities-8.3.0/approval_utilities.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 approval_utilities/utils.py
 approval_utilities.egg-info/PKG-INFO
 approval_utilities.egg-info/SOURCES.txt
 approval_utilities.egg-info/dependency_links.txt
 approval_utilities.egg-info/top_level.txt
 approval_utilities/approvaltests/__init__.py
 approval_utilities/approvaltests/core/__init__.py
+approval_utilities/approvaltests/core/executable_command.py
 approval_utilities/approvaltests/core/verifiable.py
 approval_utilities/approvaltests/core/verify_parameters.py
 approval_utilities/utilities/__init__.py
 approval_utilities/utilities/clipboard_utilities.py
 approval_utilities/utilities/deprecated.py
 approval_utilities/utilities/map_reduce.py
 approval_utilities/utilities/markdown_table.py
@@ -32,8 +33,11 @@
 approval_utilities/utilities/wrapper.py
 approval_utilities/utilities/exceptions/__init__.py
 approval_utilities/utilities/exceptions/exception_collector.py
 approval_utilities/utilities/exceptions/exception_utils.py
 approval_utilities/utilities/exceptions/multiple_exceptions.py
 approval_utilities/utilities/logger/__init__.py
 approval_utilities/utilities/logger/logging_instance.py
-approval_utilities/utilities/logger/simple_logger.py
+approval_utilities/utilities/logger/simple_logger.py
+approval_utilities/utilities/persistence/__init__.py
+approval_utilities/utilities/persistence/loader.py
+approval_utilities/utilities/persistence/saver.py
```

### Comparing `approval_utilities-8.2.5/setup.py` & `approval_utilities-8.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `approval_utilities-8.2.5/setup_utils.py` & `approval_utilities-8.3.0/setup_utils.py`

 * *Files identical despite different names*

