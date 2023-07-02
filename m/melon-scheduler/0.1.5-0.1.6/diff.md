# Comparing `tmp/melon_scheduler-0.1.5.tar.gz` & `tmp/melon_scheduler-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "melon_scheduler-0.1.5.tar", max compression
+gzip compressed data, was "melon_scheduler-0.1.6.tar", max compression
```

## Comparing `melon_scheduler-0.1.5.tar` & `melon_scheduler-0.1.6.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     2279 2023-07-02 11:26:12.884681 melon_scheduler-0.1.5/README.md
--rw-r--r--   0        0        0       77 2023-06-22 13:22:24.450031 melon_scheduler-0.1.5/melon/__init__.py
--rw-r--r--   0        0        0     4581 2023-06-30 17:27:21.260501 melon_scheduler-0.1.5/melon/calendar.py
--rw-r--r--   0        0        0      681 2023-07-02 11:05:41.555029 melon_scheduler-0.1.5/melon/config.py
--rw-r--r--   0        0        0     8578 2023-07-02 11:45:02.258976 melon_scheduler-0.1.5/melon/melon.py
--rw-r--r--   0        0        0       91 2023-07-01 17:20:32.719529 melon_scheduler-0.1.5/melon/scheduler/__init__.py
--rw-r--r--   0        0        0     2429 2023-07-02 10:51:28.366522 melon_scheduler-0.1.5/melon/scheduler/base.py
--rw-r--r--   0        0        0      970 2023-07-02 12:20:57.232115 melon_scheduler-0.1.5/melon/scheduler/cpp.py
--rw-r--r--   0        0        0     3714 2023-07-02 12:02:14.719308 melon_scheduler-0.1.5/melon/scheduler/libcppscheduler.cpp
--rw-r--r--   0        0        0      444 2023-07-01 19:54:02.564583 melon_scheduler-0.1.5/melon/scheduler/libcppscheduler.pyi
--rwxr-xr-x   0        0        0   130480 2023-07-02 12:19:17.364366 melon_scheduler-0.1.5/melon/scheduler/libcppscheduler.so
--rw-r--r--   0        0        0      444 2023-07-01 14:38:21.981201 melon_scheduler-0.1.5/melon/scheduler/libscheduler.pyi
--rw-r--r--   0        0        0     3728 2023-07-01 17:33:44.781423 melon_scheduler-0.1.5/melon/scheduler/libscheduler.rs
--rwxr-xr-x   0        0        0  4376960 2023-07-02 12:18:55.568422 melon_scheduler-0.1.5/melon/scheduler/libscheduler.so
--rw-r--r--   0        0        0     4515 2023-07-02 11:59:28.735931 melon_scheduler-0.1.5/melon/scheduler/numba.py
--rw-r--r--   0        0        0     6140 2023-07-02 11:49:50.126459 melon_scheduler-0.1.5/melon/scheduler/purepython.py
--rw-r--r--   0        0        0      973 2023-07-02 12:21:57.859964 melon_scheduler-0.1.5/melon/scheduler/rust.py
--rw-r--r--   0        0        0     6792 2023-07-02 11:45:14.654954 melon_scheduler-0.1.5/melon/todo.py
--rw-r--r--   0        0        0     1605 2023-07-02 11:27:59.016568 melon_scheduler-0.1.5/melon/visualise.py
--rw-r--r--   0        0        0      404 2023-06-30 13:41:03.809990 melon_scheduler-0.1.5/melongui/__init__.py
--rw-r--r--   0        0        0     1956 2023-06-17 21:27:46.117936 melon_scheduler-0.1.5/melongui/assets/complete.png
--rw-r--r--   0        0        0     1784 2023-06-17 21:25:13.617891 melon_scheduler-0.1.5/melongui/assets/complete.svg
--rw-r--r--   0        0        0     2047 2023-06-25 23:18:21.448400 melon_scheduler-0.1.5/melongui/calendarlist.py
--rw-r--r--   0        0        0     4749 2023-07-02 11:46:56.334773 melon_scheduler-0.1.5/melongui/mainwindow.py
--rw-r--r--   0        0        0     5948 2023-07-02 11:46:31.918816 melon_scheduler-0.1.5/melongui/taskitemdelegate.py
--rw-r--r--   0        0        0     5793 2023-07-02 11:46:43.370796 melon_scheduler-0.1.5/melongui/tasklist.py
--rw-r--r--   0        0        0     2152 2023-06-30 13:42:12.081810 melon_scheduler-0.1.5/melongui/taskwidgets.py
--rw-r--r--   0        0        0     1438 2023-07-02 12:28:16.910752 melon_scheduler-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     3037 1970-01-01 00:00:00.000000 melon_scheduler-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     2279 2023-07-02 11:26:12.884681 melon_scheduler-0.1.6/README.md
+-rw-r--r--   0        0        0       77 2023-06-22 13:22:24.450031 melon_scheduler-0.1.6/melon/__init__.py
+-rw-r--r--   0        0        0     4581 2023-06-30 17:27:21.260501 melon_scheduler-0.1.6/melon/calendar.py
+-rw-r--r--   0        0        0      681 2023-07-02 11:05:41.555029 melon_scheduler-0.1.6/melon/config.py
+-rw-r--r--   0        0        0     8578 2023-07-02 11:45:02.258976 melon_scheduler-0.1.6/melon/melon.py
+-rw-r--r--   0        0        0       91 2023-07-01 17:20:32.719529 melon_scheduler-0.1.6/melon/scheduler/__init__.py
+-rw-r--r--   0        0        0     2429 2023-07-02 10:51:28.366522 melon_scheduler-0.1.6/melon/scheduler/base.py
+-rw-r--r--   0        0        0     1128 2023-07-02 12:58:27.015897 melon_scheduler-0.1.6/melon/scheduler/cpp.py
+-rw-r--r--   0        0        0     3714 2023-07-02 12:02:14.719308 melon_scheduler-0.1.6/melon/scheduler/libcppscheduler.cpp
+-rw-r--r--   0        0        0      444 2023-07-01 19:54:02.564583 melon_scheduler-0.1.6/melon/scheduler/libcppscheduler.pyi
+-rwxr-xr-x   0        0        0   130480 2023-07-02 12:19:17.364366 melon_scheduler-0.1.6/melon/scheduler/libcppscheduler.so
+-rw-r--r--   0        0        0      444 2023-07-01 14:38:21.981201 melon_scheduler-0.1.6/melon/scheduler/libscheduler.pyi
+-rw-r--r--   0        0        0     3728 2023-07-01 17:33:44.781423 melon_scheduler-0.1.6/melon/scheduler/libscheduler.rs
+-rwxr-xr-x   0        0        0  4376960 2023-07-02 12:18:55.568422 melon_scheduler-0.1.6/melon/scheduler/libscheduler.so
+-rw-r--r--   0        0        0     4515 2023-07-02 11:59:28.735931 melon_scheduler-0.1.6/melon/scheduler/numba.py
+-rw-r--r--   0        0        0     6140 2023-07-02 11:49:50.126459 melon_scheduler-0.1.6/melon/scheduler/purepython.py
+-rw-r--r--   0        0        0     1131 2023-07-02 12:58:47.535835 melon_scheduler-0.1.6/melon/scheduler/rust.py
+-rw-r--r--   0        0        0     6792 2023-07-02 11:45:14.654954 melon_scheduler-0.1.6/melon/todo.py
+-rw-r--r--   0        0        0     1605 2023-07-02 11:27:59.016568 melon_scheduler-0.1.6/melon/visualise.py
+-rw-r--r--   0        0        0      404 2023-06-30 13:41:03.809990 melon_scheduler-0.1.6/melongui/__init__.py
+-rw-r--r--   0        0        0     1956 2023-06-17 21:27:46.117936 melon_scheduler-0.1.6/melongui/assets/complete.png
+-rw-r--r--   0        0        0     1784 2023-06-17 21:25:13.617891 melon_scheduler-0.1.6/melongui/assets/complete.svg
+-rw-r--r--   0        0        0     2047 2023-06-25 23:18:21.448400 melon_scheduler-0.1.6/melongui/calendarlist.py
+-rw-r--r--   0        0        0     4749 2023-07-02 11:46:56.334773 melon_scheduler-0.1.6/melongui/mainwindow.py
+-rw-r--r--   0        0        0     5948 2023-07-02 11:46:31.918816 melon_scheduler-0.1.6/melongui/taskitemdelegate.py
+-rw-r--r--   0        0        0     5793 2023-07-02 11:46:43.370796 melon_scheduler-0.1.6/melongui/tasklist.py
+-rw-r--r--   0        0        0     2152 2023-06-30 13:42:12.081810 melon_scheduler-0.1.6/melongui/taskwidgets.py
+-rw-r--r--   0        0        0     1438 2023-07-02 12:59:00.383796 melon_scheduler-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     3037 1970-01-01 00:00:00.000000 melon_scheduler-0.1.6/PKG-INFO
```

### Comparing `melon_scheduler-0.1.5/README.md` & `melon_scheduler-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `melon_scheduler-0.1.5/melon/calendar.py` & `melon_scheduler-0.1.6/melon/calendar.py`

 * *Files identical despite different names*

### Comparing `melon_scheduler-0.1.5/melon/config.py` & `melon_scheduler-0.1.6/melon/config.py`

 * *Files identical despite different names*

### Comparing `melon_scheduler-0.1.5/melon/melon.py` & `melon_scheduler-0.1.6/melon/melon.py`

 * *Files identical despite different names*

### Comparing `melon_scheduler-0.1.5/melon/scheduler/base.py` & `melon_scheduler-0.1.6/melon/scheduler/base.py`

 * *Files identical despite different names*

### Comparing `melon_scheduler-0.1.5/melon/scheduler/cpp.py` & `melon_scheduler-0.1.6/melon/scheduler/cpp.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 """The scheduler algorithm"""
 import dataclasses
+import logging
 import pathlib
 import sys
 from datetime import date, datetime, timedelta
 from typing import Mapping
 
 try:
-    import libcppscheduler
+    from melon.scheduler import libcppscheduler
 except ImportError:
-    sys.path.append(str(pathlib.Path(__file__).resolve().parent.parent.parent / "build"))
+    importPath = str(pathlib.Path(__file__).resolve().parent.parent.parent / "build")
+    logging.info(f"Could not find packaged .so file, falling back to {importPath} directory")
+    sys.path.append(importPath)
     import libcppscheduler
 
 from .base import START_OF_DAY, AbstractScheduler, TimeSlot
 
 
 class CppMCMCScheduler(AbstractScheduler):
     """Markov Chain Monte-Carlo Task Scheduler, implemented in Rust."""
```

### Comparing `melon_scheduler-0.1.5/melon/scheduler/libcppscheduler.cpp` & `melon_scheduler-0.1.6/melon/scheduler/libcppscheduler.cpp`

 * *Files identical despite different names*

### Comparing `melon_scheduler-0.1.5/melon/scheduler/libcppscheduler.so` & `melon_scheduler-0.1.6/melon/scheduler/libcppscheduler.so`

 * *Files identical despite different names*

### Comparing `melon_scheduler-0.1.5/melon/scheduler/libscheduler.rs` & `melon_scheduler-0.1.6/melon/scheduler/libscheduler.rs`

 * *Files identical despite different names*

### Comparing `melon_scheduler-0.1.5/melon/scheduler/libscheduler.so` & `melon_scheduler-0.1.6/melon/scheduler/libscheduler.so`

 * *Files identical despite different names*

### Comparing `melon_scheduler-0.1.5/melon/scheduler/numba.py` & `melon_scheduler-0.1.6/melon/scheduler/numba.py`

 * *Files identical despite different names*

### Comparing `melon_scheduler-0.1.5/melon/scheduler/purepython.py` & `melon_scheduler-0.1.6/melon/scheduler/purepython.py`

 * *Files identical despite different names*

### Comparing `melon_scheduler-0.1.5/melon/scheduler/rust.py` & `melon_scheduler-0.1.6/melon/scheduler/rust.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 """The scheduler algorithm"""
 import dataclasses
+import logging
 import pathlib
 import sys
 from datetime import date, datetime, timedelta
 from typing import Mapping
 
 try:
-    import libscheduler
+    from melon.scheduler import libscheduler
 except ImportError:
-    sys.path.append(str(pathlib.Path(__file__).resolve().parent.parent.parent / "target" / "release"))
+    importPath = str(pathlib.Path(__file__).resolve().parent.parent.parent / "target" / "release")
+    logging.info(f"Could not find packaged .so file, falling back to {importPath} directory")
+    sys.path.append(importPath)
     import libscheduler
 
 from .base import START_OF_DAY, AbstractScheduler, TimeSlot
 
 
 class RustyMCMCScheduler(AbstractScheduler):
     """Markov Chain Monte-Carlo Task Scheduler, implemented in Rust."""
```

### Comparing `melon_scheduler-0.1.5/melon/todo.py` & `melon_scheduler-0.1.6/melon/todo.py`

 * *Files identical despite different names*

### Comparing `melon_scheduler-0.1.5/melon/visualise.py` & `melon_scheduler-0.1.6/melon/visualise.py`

 * *Files identical despite different names*

### Comparing `melon_scheduler-0.1.5/melongui/assets/complete.png` & `melon_scheduler-0.1.6/melongui/assets/complete.png`

 * *Files identical despite different names*

### Comparing `melon_scheduler-0.1.5/melongui/assets/complete.svg` & `melon_scheduler-0.1.6/melongui/assets/complete.svg`

 * *Files identical despite different names*

### Comparing `melon_scheduler-0.1.5/melongui/calendarlist.py` & `melon_scheduler-0.1.6/melongui/calendarlist.py`

 * *Files identical despite different names*

### Comparing `melon_scheduler-0.1.5/melongui/mainwindow.py` & `melon_scheduler-0.1.6/melongui/mainwindow.py`

 * *Files identical despite different names*

### Comparing `melon_scheduler-0.1.5/melongui/taskitemdelegate.py` & `melon_scheduler-0.1.6/melongui/taskitemdelegate.py`

 * *Files identical despite different names*

### Comparing `melon_scheduler-0.1.5/melongui/tasklist.py` & `melon_scheduler-0.1.6/melongui/tasklist.py`

 * *Files identical despite different names*

### Comparing `melon_scheduler-0.1.5/melongui/taskwidgets.py` & `melon_scheduler-0.1.6/melongui/taskwidgets.py`

 * *Files identical despite different names*

### Comparing `melon_scheduler-0.1.5/pyproject.toml` & `melon_scheduler-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "melon-scheduler"
-version = "0.1.5"
+version = "0.1.6"
 description = "Schedules Todos into your Calendar"
 authors = ["redacted"]
 readme = "README.md"
 packages = [{ include = "melon" }, { include = "melongui" }]
 include = ["melon/scheduler/libscheduler.so", "melon/scheduler/libcppscheduler.so"]
 
 [tool.poetry.dependencies]
```

### Comparing `melon_scheduler-0.1.5/PKG-INFO` & `melon_scheduler-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: melon-scheduler
-Version: 0.1.5
+Version: 0.1.6
 Summary: Schedules Todos into your Calendar
 Author: redacted
 Requires-Python: >=3.10,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: gui
```

