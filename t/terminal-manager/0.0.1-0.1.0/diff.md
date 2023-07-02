# Comparing `tmp/terminal_manager-0.0.1.tar.gz` & `tmp/terminal_manager-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "terminal_manager-0.0.1.tar", last modified: Sat Jul  1 07:32:13 2023, max compression
+gzip compressed data, was "terminal_manager-0.1.0.tar", last modified: Sun Jul  2 01:39:32 2023, max compression
```

## Comparing `terminal_manager-0.0.1.tar` & `terminal_manager-0.1.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-07-01 07:32:13.081525 terminal_manager-0.0.1/
--rw-rw-rw-   0        0        0     1084 2023-06-24 10:20:33.000000 terminal_manager-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      559 2023-07-01 07:32:13.070141 terminal_manager-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      116 2023-07-01 07:31:05.000000 terminal_manager-0.0.1/README.md
--rw-rw-rw-   0        0        0      586 2023-07-01 07:21:11.000000 terminal_manager-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-01 07:32:13.088727 terminal_manager-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-01 07:32:12.914859 terminal_manager-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-07-01 07:32:12.969537 terminal_manager-0.0.1/src/terminal_manager/
--rw-rw-rw-   0        0        0     4306 2023-07-01 07:23:49.000000 terminal_manager-0.0.1/src/terminal_manager/__init__.py
--rw-rw-rw-   0        0        0     3503 2023-07-01 05:12:13.000000 terminal_manager-0.0.1/src/terminal_manager/collection.py
--rw-rw-rw-   0        0        0     5192 2023-07-01 07:24:58.000000 terminal_manager-0.0.1/src/terminal_manager/command.py
-drwxrwxrwx   0        0        0        0 2023-07-01 07:32:13.070141 terminal_manager-0.0.1/src/terminal_manager/default_collections/
--rw-rw-rw-   0        0        0      161 2023-07-01 05:12:15.000000 terminal_manager-0.0.1/src/terminal_manager/default_collections/__init__.py
--rw-rw-rw-   0        0        0     1004 2023-07-01 05:12:15.000000 terminal_manager-0.0.1/src/terminal_manager/default_collections/const.py
--rw-rw-rw-   0        0        0     3825 2023-07-01 05:12:15.000000 terminal_manager-0.0.1/src/terminal_manager/default_collections/linux.py
--rw-rw-rw-   0        0        0     3720 2023-07-01 05:12:15.000000 terminal_manager-0.0.1/src/terminal_manager/default_collections/windows_cmd.py
--rw-rw-rw-   0        0        0     3961 2023-07-01 05:12:15.000000 terminal_manager-0.0.1/src/terminal_manager/default_collections/windows_ps.py
--rw-rw-rw-   0        0        0      405 2023-07-01 05:12:14.000000 terminal_manager-0.0.1/src/terminal_manager/errors.py
--rw-rw-rw-   0        0        0      645 2023-07-01 05:12:14.000000 terminal_manager-0.0.1/src/terminal_manager/event.py
--rw-rw-rw-   0        0        0      222 2023-07-01 05:12:14.000000 terminal_manager-0.0.1/src/terminal_manager/helpers.py
--rw-rw-rw-   0        0        0     1346 2023-07-01 05:12:14.000000 terminal_manager-0.0.1/src/terminal_manager/locker.py
--rw-rw-rw-   0        0        0     8599 2023-07-01 07:25:05.000000 terminal_manager-0.0.1/src/terminal_manager/sensor.py
-drwxrwxrwx   0        0        0        0 2023-07-01 07:32:13.036590 terminal_manager-0.0.1/src/terminal_manager.egg-info/
--rw-rw-rw-   0        0        0      559 2023-07-01 07:32:12.000000 terminal_manager-0.0.1/src/terminal_manager.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      770 2023-07-01 07:32:12.000000 terminal_manager-0.0.1/src/terminal_manager.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-01 07:32:12.000000 terminal_manager-0.0.1/src/terminal_manager.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-07-01 07:32:12.000000 terminal_manager-0.0.1/src/terminal_manager.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-07-01 07:32:12.000000 terminal_manager-0.0.1/src/terminal_manager.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-02 01:39:31.986119 terminal_manager-0.1.0/
+-rw-rw-rw-   0        0        0     1084 2023-06-24 10:20:33.000000 terminal_manager-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0      703 2023-07-02 01:39:31.981120 terminal_manager-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      116 2023-07-01 07:31:05.000000 terminal_manager-0.1.0/README.md
+-rw-rw-rw-   0        0        0      732 2023-07-02 01:35:25.000000 terminal_manager-0.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-02 01:39:31.986119 terminal_manager-0.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-02 01:39:31.732121 terminal_manager-0.1.0/src/
+drwxrwxrwx   0        0        0        0 2023-07-02 01:39:31.831120 terminal_manager-0.1.0/src/terminal_manager/
+-rw-rw-rw-   0        0        0     4306 2023-07-02 00:46:10.000000 terminal_manager-0.1.0/src/terminal_manager/__init__.py
+-rw-rw-rw-   0        0        0     3503 2023-07-02 00:46:10.000000 terminal_manager-0.1.0/src/terminal_manager/collection.py
+-rw-rw-rw-   0        0        0     5192 2023-07-02 00:46:11.000000 terminal_manager-0.1.0/src/terminal_manager/command.py
+drwxrwxrwx   0        0        0        0 2023-07-02 01:39:31.980121 terminal_manager-0.1.0/src/terminal_manager/default_collections/
+-rw-rw-rw-   0        0        0      161 2023-07-02 00:46:11.000000 terminal_manager-0.1.0/src/terminal_manager/default_collections/__init__.py
+-rw-rw-rw-   0        0        0     1004 2023-07-02 00:46:11.000000 terminal_manager-0.1.0/src/terminal_manager/default_collections/const.py
+-rw-rw-rw-   0        0        0     3825 2023-07-02 00:46:11.000000 terminal_manager-0.1.0/src/terminal_manager/default_collections/linux.py
+-rw-rw-rw-   0        0        0     3720 2023-07-02 00:46:11.000000 terminal_manager-0.1.0/src/terminal_manager/default_collections/windows_cmd.py
+-rw-rw-rw-   0        0        0     3961 2023-07-02 00:46:11.000000 terminal_manager-0.1.0/src/terminal_manager/default_collections/windows_ps.py
+-rw-rw-rw-   0        0        0       56 2023-07-02 00:46:11.000000 terminal_manager-0.1.0/src/terminal_manager/errors.py
+-rw-rw-rw-   0        0        0      645 2023-07-02 00:46:11.000000 terminal_manager-0.1.0/src/terminal_manager/event.py
+-rw-rw-rw-   0        0        0      222 2023-07-02 00:46:11.000000 terminal_manager-0.1.0/src/terminal_manager/helpers.py
+-rw-rw-rw-   0        0        0     1346 2023-07-02 00:46:11.000000 terminal_manager-0.1.0/src/terminal_manager/locker.py
+-rw-rw-rw-   0        0        0     8599 2023-07-02 00:46:11.000000 terminal_manager-0.1.0/src/terminal_manager/sensor.py
+drwxrwxrwx   0        0        0        0 2023-07-02 01:39:31.952120 terminal_manager-0.1.0/src/terminal_manager.egg-info/
+-rw-rw-rw-   0        0        0      703 2023-07-02 01:39:31.000000 terminal_manager-0.1.0/src/terminal_manager.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      770 2023-07-02 01:39:31.000000 terminal_manager-0.1.0/src/terminal_manager.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-02 01:39:31.000000 terminal_manager-0.1.0/src/terminal_manager.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-07-02 01:39:31.000000 terminal_manager-0.1.0/src/terminal_manager.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-02 01:39:31.000000 terminal_manager-0.1.0/src/terminal_manager.egg-info/top_level.txt
```

### Comparing `terminal_manager-0.0.1/LICENSE` & `terminal_manager-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `terminal_manager-0.0.1/pyproject.toml` & `terminal_manager-0.1.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "terminal_manager"
-version = "0.0.1"
+version = "0.1.0"
 authors = [
   { name="zhbjsh", email="zhbjsh@outlook.com" },
 ]
 description = "Control and monitor devices with terminal commands"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
@@ -18,8 +18,12 @@
 ]
 keywords = [ 
   "terminal", 
   "command line",
 ]
 dependencies = [
   "python-slugify >= 4.0.1",
-]
+]
+
+[project.urls]
+"Homepage" = "https://github.com/zhbjsh/terminal-manager"
+"Bug Tracker" = "https://github.com/zhbjsh/terminal-manager/issues"
```

### Comparing `terminal_manager-0.0.1/src/terminal_manager/__init__.py` & `terminal_manager-0.1.0/src/terminal_manager/__init__.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Terminal manager."""
 from __future__ import annotations
 
-import logging
 from collections.abc import Sequence
 from dataclasses import dataclass
+import logging
 from typing import Any
 
 from .collection import Collection
 from .command import ActionCommand, Command, SensorCommand
 from .default_collections import ActionKey, SensorKey
 from .errors import CommandError
 from .event import Event
```

### Comparing `terminal_manager-0.0.1/src/terminal_manager/collection.py` & `terminal_manager-0.1.0/src/terminal_manager/collection.py`

 * *Files identical despite different names*

### Comparing `terminal_manager-0.0.1/src/terminal_manager/command.py` & `terminal_manager-0.1.0/src/terminal_manager/command.py`

 * *Files identical despite different names*

### Comparing `terminal_manager-0.0.1/src/terminal_manager/default_collections/const.py` & `terminal_manager-0.1.0/src/terminal_manager/default_collections/const.py`

 * *Files identical despite different names*

### Comparing `terminal_manager-0.0.1/src/terminal_manager/default_collections/linux.py` & `terminal_manager-0.1.0/src/terminal_manager/default_collections/linux.py`

 * *Files identical despite different names*

### Comparing `terminal_manager-0.0.1/src/terminal_manager/default_collections/windows_cmd.py` & `terminal_manager-0.1.0/src/terminal_manager/default_collections/windows_cmd.py`

 * *Files identical despite different names*

### Comparing `terminal_manager-0.0.1/src/terminal_manager/default_collections/windows_ps.py` & `terminal_manager-0.1.0/src/terminal_manager/default_collections/windows_ps.py`

 * *Files identical despite different names*

### Comparing `terminal_manager-0.0.1/src/terminal_manager/event.py` & `terminal_manager-0.1.0/src/terminal_manager/event.py`

 * *Files identical despite different names*

### Comparing `terminal_manager-0.0.1/src/terminal_manager/locker.py` & `terminal_manager-0.1.0/src/terminal_manager/locker.py`

 * *Files identical despite different names*

### Comparing `terminal_manager-0.0.1/src/terminal_manager/sensor.py` & `terminal_manager-0.1.0/src/terminal_manager/sensor.py`

 * *Files identical despite different names*

### Comparing `terminal_manager-0.0.1/src/terminal_manager.egg-info/SOURCES.txt` & `terminal_manager-0.1.0/src/terminal_manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

