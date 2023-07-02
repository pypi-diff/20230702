# Comparing `tmp/woodchips-0.2.4.tar.gz` & `tmp/woodchips-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "woodchips-0.2.4.tar", last modified: Wed Apr 20 04:31:15 2022, max compression
+gzip compressed data, was "woodchips-1.0.0.tar", last modified: Sun Jul  2 02:52:14 2023, max compression
```

## Comparing `woodchips-0.2.4.tar` & `woodchips-1.0.0.tar`

### file list

```diff
@@ -1,22 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-20 04:31:15.674418 woodchips-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (121)     1071 2022-04-20 04:30:41.000000 woodchips-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     3897 2022-04-20 04:31:15.674418 woodchips-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3430 2022-04-20 04:30:41.000000 woodchips-0.2.4/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      111 2022-04-20 04:30:41.000000 woodchips-0.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-04-20 04:31:15.674418 woodchips-0.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      930 2022-04-20 04:30:41.000000 woodchips-0.2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-20 04:31:15.674418 woodchips-0.2.4/test/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-20 04:30:41.000000 woodchips-0.2.4/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-20 04:31:15.674418 woodchips-0.2.4/test/unit/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-20 04:30:41.000000 woodchips-0.2.4/test/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4206 2022-04-20 04:30:41.000000 woodchips-0.2.4/test/unit/test_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-20 04:31:15.674418 woodchips-0.2.4/woodchips/
--rw-r--r--   0 runner    (1001) docker     (121)       81 2022-04-20 04:30:41.000000 woodchips-0.2.4/woodchips/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3574 2022-04-20 04:30:41.000000 woodchips-0.2.4/woodchips/logger.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-20 04:30:41.000000 woodchips-0.2.4/woodchips/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-20 04:31:15.674418 woodchips-0.2.4/woodchips.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3897 2022-04-20 04:31:15.000000 woodchips-0.2.4/woodchips.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      330 2022-04-20 04:31:15.000000 woodchips-0.2.4/woodchips.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-20 04:31:15.000000 woodchips-0.2.4/woodchips.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       91 2022-04-20 04:31:15.000000 woodchips-0.2.4/woodchips.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-04-20 04:31:15.000000 woodchips-0.2.4/woodchips.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 02:52:14.305764 woodchips-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-02 02:51:44.000000 woodchips-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3879 2023-07-02 02:52:14.305764 woodchips-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-07-02 02:51:44.000000 woodchips-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-02 02:51:44.000000 woodchips-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 02:52:14.305764 woodchips-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-07-02 02:51:44.000000 woodchips-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 02:52:14.305764 woodchips-1.0.0/test/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 02:52:14.305764 woodchips-1.0.0/test/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 02:51:44.000000 woodchips-1.0.0/test/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4220 2023-07-02 02:51:44.000000 woodchips-1.0.0/test/unit/test_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 02:52:14.305764 woodchips-1.0.0/woodchips/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-02 02:51:44.000000 woodchips-1.0.0/woodchips/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-07-02 02:51:44.000000 woodchips-1.0.0/woodchips/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 02:51:44.000000 woodchips-1.0.0/woodchips/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 02:52:14.305764 woodchips-1.0.0/woodchips.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3879 2023-07-02 02:52:14.000000 woodchips-1.0.0/woodchips.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-02 02:52:14.000000 woodchips-1.0.0/woodchips.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 02:52:14.000000 woodchips-1.0.0/woodchips.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-02 02:52:14.000000 woodchips-1.0.0/woodchips.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-02 02:52:14.000000 woodchips-1.0.0/woodchips.egg-info/top_level.txt
```

### Comparing `woodchips-0.2.4/LICENSE` & `woodchips-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `woodchips-0.2.4/PKG-INFO` & `woodchips-1.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: woodchips
-Version: 0.2.4
+Version: 1.0.0
 Summary: The cutest little logger you've ever seen.
 Home-page: http://github.com/justintime50/woodchips
 Author: justintime50
 License: MIT
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7, <4
+Requires-Python: >=3.8, <4
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 <div align="center">
 
 # Woodchips
@@ -36,15 +35,15 @@
 ## Install
 
 ```bash
 # Install tool
 pip3 install woodchips
 
 # Install locally
-make install
+just install
 ```
 
 ## Usage
 
 - A `Logger` instance must be created to use Woodchips. Simply specify a name and logging level, tell Woodchips where to log items (console and/or files), and start chipping away!
 - Need multiple loggers, no problem. Spin up separate `Logger` instances for your needs. Maybe you need a console logger for certain output that requires a specific format while another module needs a generic file formatter. Woodchips makes it easy to setup and configure all your loggers.
 - **Logging to a file:** Woodchips will automatically roll over your log files once it reaches the `log_size`. You can configure `num_of_logs` to specify how many log files will be kept in the rotation.
@@ -95,11 +94,9 @@
 - DEBUG
 - NOTSET
 
 ## Development
 
 ```bash
 # Get a comprehensive list of development tools
-make help
+just --list
 ```
-
-
```

### Comparing `woodchips-0.2.4/README.md` & `woodchips-1.0.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 ## Install
 
 ```bash
 # Install tool
 pip3 install woodchips
 
 # Install locally
-make install
+just install
 ```
 
 ## Usage
 
 - A `Logger` instance must be created to use Woodchips. Simply specify a name and logging level, tell Woodchips where to log items (console and/or files), and start chipping away!
 - Need multiple loggers, no problem. Spin up separate `Logger` instances for your needs. Maybe you need a console logger for certain output that requires a specific format while another module needs a generic file formatter. Woodchips makes it easy to setup and configure all your loggers.
 - **Logging to a file:** Woodchips will automatically roll over your log files once it reaches the `log_size`. You can configure `num_of_logs` to specify how many log files will be kept in the rotation.
@@ -79,9 +79,9 @@
 - DEBUG
 - NOTSET
 
 ## Development
 
 ```bash
 # Get a comprehensive list of development tools
-make help
+just --list
 ```
```

### Comparing `woodchips-0.2.4/setup.py` & `woodchips-1.0.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,38 +1,48 @@
 import setuptools
 
+
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 DEV_REQUIREMENTS = [
-    'black',
-    'build',
-    'coveralls == 3.*',
-    'flake8',
-    'isort',
-    'mypy',
+    'bandit == 1.7.*',
+    'black == 23.*',
+    'build == 0.10.*',
+    'flake8 == 6.*',
+    'isort == 5.*',
+    'mypy == 1.3.*',
     'pytest == 7.*',
-    'pytest-cov == 3.*',
+    'pytest-cov == 4.*',
     'twine == 4.*',
 ]
 
 setuptools.setup(
     name='woodchips',
-    version='0.2.4',
+    version='1.0.0',
     description='The cutest little logger you\'ve ever seen.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='http://github.com/justintime50/woodchips',
     author='justintime50',
     license='MIT',
-    packages=setuptools.find_packages(),
-    package_data={'woodchips': ['py.typed']},
+    packages=setuptools.find_packages(
+        exclude=[
+            'examples',
+            'test',
+        ]
+    ),
+    package_data={
+        'woodchips': [
+            'py.typed',
+        ]
+    },
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     extras_require={
         'dev': DEV_REQUIREMENTS,
     },
-    python_requires='>=3.7, <4',
+    python_requires='>=3.8, <4',
 )
```

### Comparing `woodchips-0.2.4/test/unit/test_logger.py` & `woodchips-1.0.0/test/unit/test_logger.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 import inspect
 import logging
 import os
 import tempfile
-from unittest.mock import mock_open, patch
+from unittest.mock import (
+    mock_open,
+    patch,
+)
 
 import pytest
 
 import woodchips
 
+
 MOCK_LOG_PATH = os.path.join('test', 'mock-dir')
 LOG_PATH_EXISTS = os.path.join('test', 'logs')
 LOG_LEVEL = 'INFO'
 
 
 @patch('os.makedirs')
 def test_logger_class(mock_make_dirs):
```

### Comparing `woodchips-0.2.4/woodchips/logger.py` & `woodchips-1.0.0/woodchips/logger.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 import logging
 import logging.handlers
 import os
 
+
 # 200kb * 5 files = 1mb of logs
 DEFAULT_LOG_MAX_BYTES = 200000  # 200kb
 DEFAULT_LOG_BACKUP_COUNT = 5
-DEFAULT_FORMATTER = '%(asctime)s - %(levelname)s - %(module)s.%(funcName)s - %(message)s'
+
+DEFAULT_LOG_LEVEL = 'INFO'
+
+DEFAULT_CONSOLE_FORMATTER = '%(message)s'
+DEFAULT_FILE_FORMATTER = '%(asctime)s - %(levelname)s - %(module)s.%(funcName)s - %(message)s'
 
 
 class Logger:
-    def __init__(self, name: str, level: str = 'INFO'):
+    def __init__(self, name: str, level: str = DEFAULT_LOG_LEVEL):
         """Setup a logger based on a provided set of input.
 
         - `name`: Each module that requires logging should instantiate a new class and pass a
         new name based on the module using logging. Typically for most purposes, this
         should be `__name__` passed as `name` or the root name of your package.
         - `level`: Every logger needs a level. Logged messages of a greater or equal value
         to the log level will be logged while those of a lesser value will be ignored.
@@ -27,26 +32,26 @@
 
         # Internal variables
         self._logger = get(self.name)
         log_level = self._validate_log_level()
 
         self._logger.setLevel(log_level)
 
-    def log_to_console(self, formatter: str = '%(message)s') -> None:
+    def log_to_console(self, formatter: str = DEFAULT_CONSOLE_FORMATTER) -> None:
         """Adds a console handler to a logger."""
         console_handler = logging.StreamHandler()
 
         console_formatter = logging.Formatter(formatter)
         console_handler.setFormatter(console_formatter)
         self._logger.addHandler(console_handler)
 
     def log_to_file(
         self,
         location: str,
-        formatter: str = DEFAULT_FORMATTER,
+        formatter: str = DEFAULT_FILE_FORMATTER,
         log_size: int = DEFAULT_LOG_MAX_BYTES,
         num_of_logs: int = DEFAULT_LOG_BACKUP_COUNT,
     ) -> None:
         """Adds a file handler to a logger."""
         if not os.path.exists(location):
             os.makedirs(location)
```

### Comparing `woodchips-0.2.4/woodchips.egg-info/PKG-INFO` & `woodchips-1.0.0/woodchips.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: woodchips
-Version: 0.2.4
+Version: 1.0.0
 Summary: The cutest little logger you've ever seen.
 Home-page: http://github.com/justintime50/woodchips
 Author: justintime50
 License: MIT
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7, <4
+Requires-Python: >=3.8, <4
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 <div align="center">
 
 # Woodchips
@@ -36,15 +35,15 @@
 ## Install
 
 ```bash
 # Install tool
 pip3 install woodchips
 
 # Install locally
-make install
+just install
 ```
 
 ## Usage
 
 - A `Logger` instance must be created to use Woodchips. Simply specify a name and logging level, tell Woodchips where to log items (console and/or files), and start chipping away!
 - Need multiple loggers, no problem. Spin up separate `Logger` instances for your needs. Maybe you need a console logger for certain output that requires a specific format while another module needs a generic file formatter. Woodchips makes it easy to setup and configure all your loggers.
 - **Logging to a file:** Woodchips will automatically roll over your log files once it reaches the `log_size`. You can configure `num_of_logs` to specify how many log files will be kept in the rotation.
@@ -95,11 +94,9 @@
 - DEBUG
 - NOTSET
 
 ## Development
 
 ```bash
 # Get a comprehensive list of development tools
-make help
+just --list
 ```
-
-
```

