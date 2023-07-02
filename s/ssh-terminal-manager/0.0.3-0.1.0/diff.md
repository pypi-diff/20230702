# Comparing `tmp/ssh_terminal_manager-0.0.3.tar.gz` & `tmp/ssh_terminal_manager-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssh_terminal_manager-0.0.3.tar", last modified: Sun Jul  2 00:22:06 2023, max compression
+gzip compressed data, was "ssh_terminal_manager-0.1.0.tar", last modified: Sun Jul  2 01:46:54 2023, max compression
```

## Comparing `ssh_terminal_manager-0.0.3.tar` & `ssh_terminal_manager-0.1.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-02 00:22:06.297123 ssh_terminal_manager-0.0.3/
--rw-rw-rw-   0        0        0     1084 2023-06-24 10:20:33.000000 ssh_terminal_manager-0.0.3/LICENSE
--rw-rw-rw-   0        0        0      689 2023-07-02 00:22:06.296129 ssh_terminal_manager-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      234 2023-07-01 07:07:29.000000 ssh_terminal_manager-0.0.3/README.md
--rw-rw-rw-   0        0        0      705 2023-07-02 00:21:40.000000 ssh_terminal_manager-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-02 00:22:06.297123 ssh_terminal_manager-0.0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-02 00:22:06.236129 ssh_terminal_manager-0.0.3/src/
-drwxrwxrwx   0        0        0        0 2023-07-02 00:22:06.256122 ssh_terminal_manager-0.0.3/src/ssh_terminal_manager/
--rw-rw-rw-   0        0        0    10318 2023-07-02 00:12:01.000000 ssh_terminal_manager-0.0.3/src/ssh_terminal_manager/__init__.py
--rw-rw-rw-   0        0        0      347 2023-07-02 00:13:21.000000 ssh_terminal_manager-0.0.3/src/ssh_terminal_manager/errors.py
-drwxrwxrwx   0        0        0        0 2023-07-02 00:22:06.294121 ssh_terminal_manager-0.0.3/src/ssh_terminal_manager.egg-info/
--rw-rw-rw-   0        0        0      689 2023-07-02 00:22:06.000000 ssh_terminal_manager-0.0.3/src/ssh_terminal_manager.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      343 2023-07-02 00:22:06.000000 ssh_terminal_manager-0.0.3/src/ssh_terminal_manager.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-02 00:22:06.000000 ssh_terminal_manager-0.0.3/src/ssh_terminal_manager.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       92 2023-07-02 00:22:06.000000 ssh_terminal_manager-0.0.3/src/ssh_terminal_manager.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-07-02 00:22:06.000000 ssh_terminal_manager-0.0.3/src/ssh_terminal_manager.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-02 01:46:54.250198 ssh_terminal_manager-0.1.0/
+-rw-rw-rw-   0        0        0     1084 2023-06-24 10:20:33.000000 ssh_terminal_manager-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0      841 2023-07-02 01:46:54.248198 ssh_terminal_manager-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      234 2023-07-01 07:07:29.000000 ssh_terminal_manager-0.1.0/README.md
+-rw-rw-rw-   0        0        0      859 2023-07-02 01:44:15.000000 ssh_terminal_manager-0.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-02 01:46:54.250198 ssh_terminal_manager-0.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-02 01:46:54.184198 ssh_terminal_manager-0.1.0/src/
+drwxrwxrwx   0        0        0        0 2023-07-02 01:46:54.208198 ssh_terminal_manager-0.1.0/src/ssh_terminal_manager/
+-rw-rw-rw-   0        0        0    10344 2023-07-02 00:46:10.000000 ssh_terminal_manager-0.1.0/src/ssh_terminal_manager/__init__.py
+-rw-rw-rw-   0        0        0      347 2023-07-02 00:46:10.000000 ssh_terminal_manager-0.1.0/src/ssh_terminal_manager/errors.py
+drwxrwxrwx   0        0        0        0 2023-07-02 01:46:54.247195 ssh_terminal_manager-0.1.0/src/ssh_terminal_manager.egg-info/
+-rw-rw-rw-   0        0        0      841 2023-07-02 01:46:54.000000 ssh_terminal_manager-0.1.0/src/ssh_terminal_manager.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      343 2023-07-02 01:46:54.000000 ssh_terminal_manager-0.1.0/src/ssh_terminal_manager.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-02 01:46:54.000000 ssh_terminal_manager-0.1.0/src/ssh_terminal_manager.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       92 2023-07-02 01:46:54.000000 ssh_terminal_manager-0.1.0/src/ssh_terminal_manager.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-07-02 01:46:54.000000 ssh_terminal_manager-0.1.0/src/ssh_terminal_manager.egg-info/top_level.txt
```

### Comparing `ssh_terminal_manager-0.0.3/LICENSE` & `ssh_terminal_manager-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ssh_terminal_manager-0.0.3/pyproject.toml` & `ssh_terminal_manager-0.1.0/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ssh_terminal_manager"
-version = "0.0.3"
+version = "0.1.0"
 authors = [
   { name="zhbjsh", email="zhbjsh@outlook.com" },
 ]
 description = "Control and monitor devices with SSH terminal commands"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
@@ -23,8 +23,12 @@
 ]
 dependencies = [
   "icmplib >= 3.0",
   "paramiko >= 3.2.0",
   "python-slugify >= 4.0.1",
   "terminal-manager >= 0.0.1",
   "wakeonlan >= 3.0.0"
-]
+]
+
+[project.urls]
+"Homepage" = "https://github.com/zhbjsh/ssh-terminal-manager"
+"Bug Tracker" = "https://github.com/zhbjsh/ssh-terminal-manager/issues"
```

### Comparing `ssh_terminal_manager-0.0.3/src/ssh_terminal_manager/__init__.py` & `ssh_terminal_manager-0.1.0/src/ssh_terminal_manager/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,31 +3,32 @@
 
 import asyncio
 import logging
 from time import time
 
 import icmplib
 import paramiko
-import wakeonlan
 from terminal_manager import (
     DEFAULT_COMMAND_TIMEOUT,
     ActionCommand,
     BinarySensor,
     Collection,
     Command,
     CommandError,
     CommandOutput,
     Event,
     Manager,
     NumberSensor,
     Sensor,
     SensorCommand,
     TextSensor,
+    default_collections,
 )
 from terminal_manager.default_collections import ActionKey, SensorKey
+import wakeonlan
 
 from .errors import OfflineError, SSHAuthError, SSHConnectError, SSHHostKeyUnknownError
 
 _LOGGER = logging.getLogger(__name__)
 _TEST_COMMAND = Command("")
 
 DEFAULT_PORT = 22
```

### Comparing `ssh_terminal_manager-0.0.3/src/ssh_terminal_manager.egg-info/PKG-INFO` & `ssh_terminal_manager-0.1.0/src/ssh_terminal_manager.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 Metadata-Version: 2.1
 Name: ssh-terminal-manager
-Version: 0.0.3
+Version: 0.1.0
 Summary: Control and monitor devices with SSH terminal commands
 Author-email: zhbjsh <zhbjsh@outlook.com>
+Project-URL: Homepage, https://github.com/zhbjsh/ssh-terminal-manager
+Project-URL: Bug Tracker, https://github.com/zhbjsh/ssh-terminal-manager/issues
 Keywords: ssh,terminal,command line
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

