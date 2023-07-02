# Comparing `tmp/ssh_terminal_manager-0.0.2.tar.gz` & `tmp/ssh_terminal_manager-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssh_terminal_manager-0.0.2.tar", last modified: Sat Jul  1 07:49:17 2023, max compression
+gzip compressed data, was "ssh_terminal_manager-0.0.3.tar", last modified: Sun Jul  2 00:22:06 2023, max compression
```

## Comparing `ssh_terminal_manager-0.0.2.tar` & `ssh_terminal_manager-0.0.3.tar`

### file list

```diff
@@ -1,29 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-01 07:49:17.697689 ssh_terminal_manager-0.0.2/
--rw-rw-rw-   0        0        0     1084 2023-06-24 10:20:33.000000 ssh_terminal_manager-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      689 2023-07-01 07:49:17.696056 ssh_terminal_manager-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      234 2023-07-01 07:07:29.000000 ssh_terminal_manager-0.0.2/README.md
--rw-rw-rw-   0        0        0      674 2023-07-01 07:48:07.000000 ssh_terminal_manager-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-01 07:49:17.698691 ssh_terminal_manager-0.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-01 07:49:17.552478 ssh_terminal_manager-0.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-07-01 07:49:17.610433 ssh_terminal_manager-0.0.2/src/ssh_terminal_manager/
--rw-rw-rw-   0        0        0    10338 2023-07-01 07:37:03.000000 ssh_terminal_manager-0.0.2/src/ssh_terminal_manager/__init__.py
--rw-rw-rw-   0        0        0     3503 2023-07-01 05:12:13.000000 ssh_terminal_manager-0.0.2/src/ssh_terminal_manager/collection.py
--rw-rw-rw-   0        0        0     5199 2023-07-01 05:12:14.000000 ssh_terminal_manager-0.0.2/src/ssh_terminal_manager/command.py
-drwxrwxrwx   0        0        0        0 2023-07-01 07:49:17.693748 ssh_terminal_manager-0.0.2/src/ssh_terminal_manager/default_collections/
--rw-rw-rw-   0        0        0      161 2023-07-01 05:12:15.000000 ssh_terminal_manager-0.0.2/src/ssh_terminal_manager/default_collections/__init__.py
--rw-rw-rw-   0        0        0     1004 2023-07-01 05:12:15.000000 ssh_terminal_manager-0.0.2/src/ssh_terminal_manager/default_collections/const.py
--rw-rw-rw-   0        0        0     3825 2023-07-01 05:12:15.000000 ssh_terminal_manager-0.0.2/src/ssh_terminal_manager/default_collections/linux.py
--rw-rw-rw-   0        0        0     3720 2023-07-01 05:12:15.000000 ssh_terminal_manager-0.0.2/src/ssh_terminal_manager/default_collections/windows_cmd.py
--rw-rw-rw-   0        0        0     3961 2023-07-01 05:12:15.000000 ssh_terminal_manager-0.0.2/src/ssh_terminal_manager/default_collections/windows_ps.py
--rw-rw-rw-   0        0        0      405 2023-07-01 05:12:14.000000 ssh_terminal_manager-0.0.2/src/ssh_terminal_manager/errors.py
--rw-rw-rw-   0        0        0      645 2023-07-01 05:12:14.000000 ssh_terminal_manager-0.0.2/src/ssh_terminal_manager/event.py
--rw-rw-rw-   0        0        0      222 2023-07-01 05:12:14.000000 ssh_terminal_manager-0.0.2/src/ssh_terminal_manager/helpers.py
--rw-rw-rw-   0        0        0     1346 2023-07-01 05:12:14.000000 ssh_terminal_manager-0.0.2/src/ssh_terminal_manager/locker.py
--rw-rw-rw-   0        0        0     4133 2023-07-01 05:12:14.000000 ssh_terminal_manager-0.0.2/src/ssh_terminal_manager/manager.py
--rw-rw-rw-   0        0        0     8606 2023-07-01 05:12:14.000000 ssh_terminal_manager-0.0.2/src/ssh_terminal_manager/sensor.py
-drwxrwxrwx   0        0        0        0 2023-07-01 07:49:17.668184 ssh_terminal_manager-0.0.2/src/ssh_terminal_manager.egg-info/
--rw-rw-rw-   0        0        0      689 2023-07-01 07:49:17.000000 ssh_terminal_manager-0.0.2/src/ssh_terminal_manager.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      878 2023-07-01 07:49:17.000000 ssh_terminal_manager-0.0.2/src/ssh_terminal_manager.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-01 07:49:17.000000 ssh_terminal_manager-0.0.2/src/ssh_terminal_manager.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       68 2023-07-01 07:49:17.000000 ssh_terminal_manager-0.0.2/src/ssh_terminal_manager.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-07-01 07:49:17.000000 ssh_terminal_manager-0.0.2/src/ssh_terminal_manager.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-02 00:22:06.297123 ssh_terminal_manager-0.0.3/
+-rw-rw-rw-   0        0        0     1084 2023-06-24 10:20:33.000000 ssh_terminal_manager-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0      689 2023-07-02 00:22:06.296129 ssh_terminal_manager-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      234 2023-07-01 07:07:29.000000 ssh_terminal_manager-0.0.3/README.md
+-rw-rw-rw-   0        0        0      705 2023-07-02 00:21:40.000000 ssh_terminal_manager-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-02 00:22:06.297123 ssh_terminal_manager-0.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-02 00:22:06.236129 ssh_terminal_manager-0.0.3/src/
+drwxrwxrwx   0        0        0        0 2023-07-02 00:22:06.256122 ssh_terminal_manager-0.0.3/src/ssh_terminal_manager/
+-rw-rw-rw-   0        0        0    10318 2023-07-02 00:12:01.000000 ssh_terminal_manager-0.0.3/src/ssh_terminal_manager/__init__.py
+-rw-rw-rw-   0        0        0      347 2023-07-02 00:13:21.000000 ssh_terminal_manager-0.0.3/src/ssh_terminal_manager/errors.py
+drwxrwxrwx   0        0        0        0 2023-07-02 00:22:06.294121 ssh_terminal_manager-0.0.3/src/ssh_terminal_manager.egg-info/
+-rw-rw-rw-   0        0        0      689 2023-07-02 00:22:06.000000 ssh_terminal_manager-0.0.3/src/ssh_terminal_manager.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      343 2023-07-02 00:22:06.000000 ssh_terminal_manager-0.0.3/src/ssh_terminal_manager.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-02 00:22:06.000000 ssh_terminal_manager-0.0.3/src/ssh_terminal_manager.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       92 2023-07-02 00:22:06.000000 ssh_terminal_manager-0.0.3/src/ssh_terminal_manager.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-07-02 00:22:06.000000 ssh_terminal_manager-0.0.3/src/ssh_terminal_manager.egg-info/top_level.txt
```

### Comparing `ssh_terminal_manager-0.0.2/LICENSE` & `ssh_terminal_manager-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ssh_terminal_manager-0.0.2/PKG-INFO` & `ssh_terminal_manager-0.0.3/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssh_terminal_manager
-Version: 0.0.2
+Version: 0.0.3
 Summary: Control and monitor devices with SSH terminal commands
 Author-email: zhbjsh <zhbjsh@outlook.com>
 Keywords: ssh,terminal,command line
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `ssh_terminal_manager-0.0.2/pyproject.toml` & `ssh_terminal_manager-0.0.3/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ssh_terminal_manager"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="zhbjsh", email="zhbjsh@outlook.com" },
 ]
 description = "Control and monitor devices with SSH terminal commands"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
@@ -21,9 +21,10 @@
   "terminal", 
   "command line",
 ]
 dependencies = [
   "icmplib >= 3.0",
   "paramiko >= 3.2.0",
   "python-slugify >= 4.0.1",
-  "wakeonlan >= 3.0.0",
+  "terminal-manager >= 0.0.1",
+  "wakeonlan >= 3.0.0"
 ]
```

### Comparing `ssh_terminal_manager-0.0.2/src/ssh_terminal_manager/__init__.py` & `ssh_terminal_manager-0.0.3/src/ssh_terminal_manager/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,28 +4,32 @@
 import asyncio
 import logging
 from time import time
 
 import icmplib
 import paramiko
 import wakeonlan
-
-from .collection import Collection
-from .command import ActionCommand, Command, SensorCommand
-from .default_collections import ActionKey, SensorKey
-from .errors import (
+from terminal_manager import (
+    DEFAULT_COMMAND_TIMEOUT,
+    ActionCommand,
+    BinarySensor,
+    Collection,
+    Command,
     CommandError,
-    OfflineError,
-    SSHAuthError,
-    SSHConnectError,
-    SSHHostKeyUnknownError,
+    CommandOutput,
+    Event,
+    Manager,
+    NumberSensor,
+    Sensor,
+    SensorCommand,
+    TextSensor,
 )
-from .event import Event
-from .manager import DEFAULT_COMMAND_TIMEOUT, CommandOutput, Manager
-from .sensor import BinarySensor, NumberSensor, Sensor, TextSensor
+from terminal_manager.default_collections import ActionKey, SensorKey
+
+from .errors import OfflineError, SSHAuthError, SSHConnectError, SSHHostKeyUnknownError
 
 _LOGGER = logging.getLogger(__name__)
 _TEST_COMMAND = Command("")
 
 DEFAULT_PORT = 22
 DEFAULT_PING_TIMEOUT = 4
 DEFAULT_SSH_TIMEOUT = 4
```

### Comparing `ssh_terminal_manager-0.0.2/src/ssh_terminal_manager.egg-info/PKG-INFO` & `ssh_terminal_manager-0.0.3/src/ssh_terminal_manager.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssh-terminal-manager
-Version: 0.0.2
+Version: 0.0.3
 Summary: Control and monitor devices with SSH terminal commands
 Author-email: zhbjsh <zhbjsh@outlook.com>
 Keywords: ssh,terminal,command line
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

