# Comparing `tmp/robotframework-reportportal_updated-1.1.3.tar.gz` & `tmp/robotframework-reportportal_updated-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotframework-reportportal_updated-1.1.3.tar", last modified: Fri Jun 23 07:57:55 2023, max compression
+gzip compressed data, was "robotframework-reportportal_updated-1.1.6.tar", last modified: Sun Jul  2 10:51:17 2023, max compression
```

## Comparing `robotframework-reportportal_updated-1.1.3.tar` & `robotframework-reportportal_updated-1.1.6.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:57:55.431334 robotframework-reportportal_updated-1.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     5008 2023-06-23 07:57:47.000000 robotframework-reportportal_updated-1.1.3/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-23 07:57:47.000000 robotframework-reportportal_updated-1.1.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-23 07:57:47.000000 robotframework-reportportal_updated-1.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6931 2023-06-23 07:57:55.431334 robotframework-reportportal_updated-1.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6131 2023-06-23 07:57:47.000000 robotframework-reportportal_updated-1.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-06-23 07:57:47.000000 robotframework-reportportal_updated-1.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-23 07:57:47.000000 robotframework-reportportal_updated-1.1.3/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:57:55.427334 robotframework-reportportal_updated-1.1.3/robotframework_reportportal_updated/
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-23 07:57:47.000000 robotframework-reportportal_updated-1.1.3/robotframework_reportportal_updated/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-06-23 07:57:47.000000 robotframework-reportportal_updated-1.1.3/robotframework_reportportal_updated/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)    12463 2023-06-23 07:57:47.000000 robotframework-reportportal_updated-1.1.3/robotframework_reportportal_updated/listener.py
--rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-06-23 07:57:47.000000 robotframework-reportportal_updated-1.1.3/robotframework_reportportal_updated/listener.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4015 2023-06-23 07:57:47.000000 robotframework-reportportal_updated-1.1.3/robotframework_reportportal_updated/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     8176 2023-06-23 07:57:47.000000 robotframework-reportportal_updated-1.1.3/robotframework_reportportal_updated/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-06-23 07:57:47.000000 robotframework-reportportal_updated-1.1.3/robotframework_reportportal_updated/model.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-06-23 07:57:47.000000 robotframework-reportportal_updated-1.1.3/robotframework_reportportal_updated/post_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     5940 2023-06-23 07:57:47.000000 robotframework-reportportal_updated-1.1.3/robotframework_reportportal_updated/result_visitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-06-23 07:57:47.000000 robotframework-reportportal_updated-1.1.3/robotframework_reportportal_updated/result_visitor.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10727 2023-06-23 07:57:47.000000 robotframework-reportportal_updated-1.1.3/robotframework_reportportal_updated/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-06-23 07:57:47.000000 robotframework-reportportal_updated-1.1.3/robotframework_reportportal_updated/service.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-06-23 07:57:47.000000 robotframework-reportportal_updated-1.1.3/robotframework_reportportal_updated/static.py
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-06-23 07:57:47.000000 robotframework-reportportal_updated-1.1.3/robotframework_reportportal_updated/static.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-06-23 07:57:47.000000 robotframework-reportportal_updated-1.1.3/robotframework_reportportal_updated/time_visitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5251 2023-06-23 07:57:47.000000 robotframework-reportportal_updated-1.1.3/robotframework_reportportal_updated/variables.py
--rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-06-23 07:57:47.000000 robotframework-reportportal_updated-1.1.3/robotframework_reportportal_updated/variables.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:57:55.431334 robotframework-reportportal_updated-1.1.3/robotframework_reportportal_updated.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6931 2023-06-23 07:57:55.000000 robotframework-reportportal_updated-1.1.3/robotframework_reportportal_updated.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-06-23 07:57:55.000000 robotframework-reportportal_updated-1.1.3/robotframework_reportportal_updated.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 07:57:55.000000 robotframework-reportportal_updated-1.1.3/robotframework_reportportal_updated.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-23 07:57:55.000000 robotframework-reportportal_updated-1.1.3/robotframework_reportportal_updated.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-23 07:57:55.000000 robotframework-reportportal_updated-1.1.3/robotframework_reportportal_updated.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-23 07:57:55.000000 robotframework-reportportal_updated-1.1.3/robotframework_reportportal_updated.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-23 07:57:55.431334 robotframework-reportportal_updated-1.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-06-23 07:57:47.000000 robotframework-reportportal_updated-1.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:51:17.212798 robotframework-reportportal_updated-1.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     5008 2023-07-02 10:51:12.000000 robotframework-reportportal_updated-1.1.6/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-02 10:51:12.000000 robotframework-reportportal_updated-1.1.6/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-02 10:51:12.000000 robotframework-reportportal_updated-1.1.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6931 2023-07-02 10:51:17.212798 robotframework-reportportal_updated-1.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6131 2023-07-02 10:51:12.000000 robotframework-reportportal_updated-1.1.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-02 10:51:12.000000 robotframework-reportportal_updated-1.1.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-02 10:51:12.000000 robotframework-reportportal_updated-1.1.6/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:51:17.212798 robotframework-reportportal_updated-1.1.6/robotframework_reportportal_updated/
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-02 10:51:12.000000 robotframework-reportportal_updated-1.1.6/robotframework_reportportal_updated/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-07-02 10:51:12.000000 robotframework-reportportal_updated-1.1.6/robotframework_reportportal_updated/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12463 2023-07-02 10:51:12.000000 robotframework-reportportal_updated-1.1.6/robotframework_reportportal_updated/listener.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-07-02 10:51:12.000000 robotframework-reportportal_updated-1.1.6/robotframework_reportportal_updated/listener.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4015 2023-07-02 10:51:12.000000 robotframework-reportportal_updated-1.1.6/robotframework_reportportal_updated/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8176 2023-07-02 10:51:12.000000 robotframework-reportportal_updated-1.1.6/robotframework_reportportal_updated/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-07-02 10:51:12.000000 robotframework-reportportal_updated-1.1.6/robotframework_reportportal_updated/model.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-07-02 10:51:12.000000 robotframework-reportportal_updated-1.1.6/robotframework_reportportal_updated/post_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5940 2023-07-02 10:51:12.000000 robotframework-reportportal_updated-1.1.6/robotframework_reportportal_updated/result_visitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-07-02 10:51:12.000000 robotframework-reportportal_updated-1.1.6/robotframework_reportportal_updated/result_visitor.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10727 2023-07-02 10:51:12.000000 robotframework-reportportal_updated-1.1.6/robotframework_reportportal_updated/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-07-02 10:51:12.000000 robotframework-reportportal_updated-1.1.6/robotframework_reportportal_updated/service.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-07-02 10:51:12.000000 robotframework-reportportal_updated-1.1.6/robotframework_reportportal_updated/static.py
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-07-02 10:51:12.000000 robotframework-reportportal_updated-1.1.6/robotframework_reportportal_updated/static.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-07-02 10:51:12.000000 robotframework-reportportal_updated-1.1.6/robotframework_reportportal_updated/time_visitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5251 2023-07-02 10:51:12.000000 robotframework-reportportal_updated-1.1.6/robotframework_reportportal_updated/variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-07-02 10:51:12.000000 robotframework-reportportal_updated-1.1.6/robotframework_reportportal_updated/variables.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:51:17.212798 robotframework-reportportal_updated-1.1.6/robotframework_reportportal_updated.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6931 2023-07-02 10:51:17.000000 robotframework-reportportal_updated-1.1.6/robotframework_reportportal_updated.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-07-02 10:51:17.000000 robotframework-reportportal_updated-1.1.6/robotframework_reportportal_updated.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 10:51:17.000000 robotframework-reportportal_updated-1.1.6/robotframework_reportportal_updated.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-02 10:51:17.000000 robotframework-reportportal_updated-1.1.6/robotframework_reportportal_updated.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-02 10:51:17.000000 robotframework-reportportal_updated-1.1.6/robotframework_reportportal_updated.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-02 10:51:17.000000 robotframework-reportportal_updated-1.1.6/robotframework_reportportal_updated.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-02 10:51:17.212798 robotframework-reportportal_updated-1.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-07-02 10:51:12.000000 robotframework-reportportal_updated-1.1.6/setup.py
```

### Comparing `robotframework-reportportal_updated-1.1.3/CONTRIBUTING.rst` & `robotframework-reportportal_updated-1.1.6/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `robotframework-reportportal_updated-1.1.3/LICENSE.txt` & `robotframework-reportportal_updated-1.1.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `robotframework-reportportal_updated-1.1.3/PKG-INFO` & `robotframework-reportportal_updated-1.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: robotframework-reportportal_updated
-Version: 1.1.3
+Version: 1.1.6
 Summary: Agent for reporting RobotFramework test results to Report Portal
 Home-page: https://github.com/reportportal/agent-Python-RobotFramework
-Download-URL: https://github.com/reportportal/agent-Python-RobotFramework/tarball/1.1.3
+Download-URL: https://github.com/reportportal/agent-Python-RobotFramework/tarball/1.1.6
 Author: Report Portal Team
 Author-email: support@reportportal.io
 Keywords: testing,reporting,robot framework,reportportal,agent
 Classifier: Framework :: Robot Framework
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `robotframework-reportportal_updated-1.1.3/README.md` & `robotframework-reportportal_updated-1.1.6/README.md`

 * *Files identical despite different names*

### Comparing `robotframework-reportportal_updated-1.1.3/robotframework_reportportal_updated/__init__.py` & `robotframework-reportportal_updated-1.1.6/robotframework_reportportal_updated/__init__.py`

 * *Files identical despite different names*

### Comparing `robotframework-reportportal_updated-1.1.3/robotframework_reportportal_updated/exception.py` & `robotframework-reportportal_updated-1.1.6/robotframework_reportportal_updated/exception.py`

 * *Files identical despite different names*

### Comparing `robotframework-reportportal_updated-1.1.3/robotframework_reportportal_updated/listener.py` & `robotframework-reportportal_updated-1.1.6/robotframework_reportportal_updated/listener.py`

 * *Files identical despite different names*

### Comparing `robotframework-reportportal_updated-1.1.3/robotframework_reportportal_updated/listener.pyi` & `robotframework-reportportal_updated-1.1.6/robotframework_reportportal_updated/listener.pyi`

 * *Files identical despite different names*

### Comparing `robotframework-reportportal_updated-1.1.3/robotframework_reportportal_updated/logger.py` & `robotframework-reportportal_updated-1.1.6/robotframework_reportportal_updated/logger.py`

 * *Files identical despite different names*

### Comparing `robotframework-reportportal_updated-1.1.3/robotframework_reportportal_updated/model.py` & `robotframework-reportportal_updated-1.1.6/robotframework_reportportal_updated/model.py`

 * *Files identical despite different names*

### Comparing `robotframework-reportportal_updated-1.1.3/robotframework_reportportal_updated/model.pyi` & `robotframework-reportportal_updated-1.1.6/robotframework_reportportal_updated/model.pyi`

 * *Files identical despite different names*

### Comparing `robotframework-reportportal_updated-1.1.3/robotframework_reportportal_updated/post_report.py` & `robotframework-reportportal_updated-1.1.6/robotframework_reportportal_updated/post_report.py`

 * *Files 5% similar despite different names*

```diff
@@ -43,18 +43,18 @@
 
 import getopt
 import logging
 import sys
 
 from robot.api import ExecutionResult
 
-from robotframework_reportportal.result_visitor import RobotResultsVisitor
-from robotframework_reportportal.time_visitor import TimeVisitor, corrections
+from robotframework_reportportal_updated.result_visitor import RobotResultsVisitor
+from robotframework_reportportal_updated.time_visitor import TimeVisitor, corrections
 # noinspection PyUnresolvedReferences
-from robotframework_reportportal.variables import _variables
+from robotframework_reportportal_updated.variables import _variables
 
 
 def process(infile="output.xml"):
     test_run = ExecutionResult(infile)
     test_run.visit(TimeVisitor())
     if corrections:
         logging.warning("{0} is missing some of its starttime/endtime. "
```

### Comparing `robotframework-reportportal_updated-1.1.3/robotframework_reportportal_updated/result_visitor.py` & `robotframework-reportportal_updated-1.1.6/robotframework_reportportal_updated/result_visitor.py`

 * *Files identical despite different names*

### Comparing `robotframework-reportportal_updated-1.1.3/robotframework_reportportal_updated/result_visitor.pyi` & `robotframework-reportportal_updated-1.1.6/robotframework_reportportal_updated/result_visitor.pyi`

 * *Files identical despite different names*

### Comparing `robotframework-reportportal_updated-1.1.3/robotframework_reportportal_updated/service.py` & `robotframework-reportportal_updated-1.1.6/robotframework_reportportal_updated/service.py`

 * *Files identical despite different names*

### Comparing `robotframework-reportportal_updated-1.1.3/robotframework_reportportal_updated/service.pyi` & `robotframework-reportportal_updated-1.1.6/robotframework_reportportal_updated/service.pyi`

 * *Files identical despite different names*

### Comparing `robotframework-reportportal_updated-1.1.3/robotframework_reportportal_updated/static.py` & `robotframework-reportportal_updated-1.1.6/robotframework_reportportal_updated/static.py`

 * *Files identical despite different names*

### Comparing `robotframework-reportportal_updated-1.1.3/robotframework_reportportal_updated/static.pyi` & `robotframework-reportportal_updated-1.1.6/robotframework_reportportal_updated/static.pyi`

 * *Files identical despite different names*

### Comparing `robotframework-reportportal_updated-1.1.3/robotframework_reportportal_updated/time_visitor.py` & `robotframework-reportportal_updated-1.1.6/robotframework_reportportal_updated/time_visitor.py`

 * *Files identical despite different names*

### Comparing `robotframework-reportportal_updated-1.1.3/robotframework_reportportal_updated/variables.py` & `robotframework-reportportal_updated-1.1.6/robotframework_reportportal_updated/variables.py`

 * *Files identical despite different names*

### Comparing `robotframework-reportportal_updated-1.1.3/robotframework_reportportal_updated/variables.pyi` & `robotframework-reportportal_updated-1.1.6/robotframework_reportportal_updated/variables.pyi`

 * *Files identical despite different names*

### Comparing `robotframework-reportportal_updated-1.1.3/robotframework_reportportal_updated.egg-info/PKG-INFO` & `robotframework-reportportal_updated-1.1.6/robotframework_reportportal_updated.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: robotframework-reportportal-updated
-Version: 1.1.3
+Version: 1.1.6
 Summary: Agent for reporting RobotFramework test results to Report Portal
 Home-page: https://github.com/reportportal/agent-Python-RobotFramework
-Download-URL: https://github.com/reportportal/agent-Python-RobotFramework/tarball/1.1.3
+Download-URL: https://github.com/reportportal/agent-Python-RobotFramework/tarball/1.1.6
 Author: Report Portal Team
 Author-email: support@reportportal.io
 Keywords: testing,reporting,robot framework,reportportal,agent
 Classifier: Framework :: Robot Framework
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `robotframework-reportportal_updated-1.1.3/robotframework_reportportal_updated.egg-info/SOURCES.txt` & `robotframework-reportportal_updated-1.1.6/robotframework_reportportal_updated.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `robotframework-reportportal_updated-1.1.3/setup.py` & `robotframework-reportportal_updated-1.1.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Setup instructions for the package."""
 
 import os
 
 from setuptools import setup, find_packages
 
-__version__ = '1.1.3'
+__version__ = '1.1.6'
 
 
 def read_file(fname):
     """Read the given file.
 
     :param fname: Name of the file to be read
     :return:      Output of the given file
```

