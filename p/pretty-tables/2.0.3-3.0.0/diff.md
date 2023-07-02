# Comparing `tmp/pretty-tables-2.0.3.tar.gz` & `tmp/pretty-tables-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pretty-tables-2.0.3.tar", last modified: Tue Dec  7 16:46:39 2021, max compression
+gzip compressed data, was "pretty-tables-3.0.0.tar", last modified: Sun Jul  2 02:57:17 2023, max compression
```

## Comparing `pretty-tables-2.0.3.tar` & `pretty-tables-3.0.0.tar`

### file list

```diff
@@ -1,25 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-07 16:46:39.739481 pretty-tables-2.0.3/
--rw-r--r--   0 runner    (1001) docker     (121)     1071 2021-12-07 16:46:27.000000 pretty-tables-2.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     3567 2021-12-07 16:46:39.739481 pretty-tables-2.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3063 2021-12-07 16:46:27.000000 pretty-tables-2.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-07 16:46:39.731480 pretty-tables-2.0.3/pretty_tables/
--rw-r--r--   0 runner    (1001) docker     (121)      127 2021-12-07 16:46:27.000000 pretty-tables-2.0.3/pretty_tables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3942 2021-12-07 16:46:27.000000 pretty-tables-2.0.3/pretty_tables/formatting.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-07 16:46:27.000000 pretty-tables-2.0.3/pretty_tables/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)     2928 2021-12-07 16:46:27.000000 pretty-tables-2.0.3/pretty_tables/tables.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-07 16:46:39.735481 pretty-tables-2.0.3/pretty_tables.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3567 2021-12-07 16:46:39.000000 pretty-tables-2.0.3/pretty_tables.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      441 2021-12-07 16:46:39.000000 pretty-tables-2.0.3/pretty_tables.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-07 16:46:39.000000 pretty-tables-2.0.3/pretty_tables.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       74 2021-12-07 16:46:39.000000 pretty-tables-2.0.3/pretty_tables.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       19 2021-12-07 16:46:39.000000 pretty-tables-2.0.3/pretty_tables.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      134 2021-12-07 16:46:27.000000 pretty-tables-2.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-12-07 16:46:39.739481 pretty-tables-2.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      937 2021-12-07 16:46:27.000000 pretty-tables-2.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-07 16:46:39.735481 pretty-tables-2.0.3/test/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-07 16:46:27.000000 pretty-tables-2.0.3/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-07 16:46:39.739481 pretty-tables-2.0.3/test/unit/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-07 16:46:27.000000 pretty-tables-2.0.3/test/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      608 2021-12-07 16:46:27.000000 pretty-tables-2.0.3/test/unit/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)     3651 2021-12-07 16:46:27.000000 pretty-tables-2.0.3/test/unit/test_formatting.py
--rw-r--r--   0 runner    (1001) docker     (121)     3086 2021-12-07 16:46:27.000000 pretty-tables-2.0.3/test/unit/test_tables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 02:57:17.951873 pretty-tables-3.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-02 02:56:48.000000 pretty-tables-3.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-07-02 02:57:17.951873 pretty-tables-3.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-07-02 02:56:48.000000 pretty-tables-3.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 02:57:17.951873 pretty-tables-3.0.0/pretty_tables/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-02 02:56:48.000000 pretty-tables-3.0.0/pretty_tables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3959 2023-07-02 02:56:48.000000 pretty-tables-3.0.0/pretty_tables/formatting.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 02:56:48.000000 pretty-tables-3.0.0/pretty_tables/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-07-02 02:56:48.000000 pretty-tables-3.0.0/pretty_tables/tables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 02:57:17.951873 pretty-tables-3.0.0/pretty_tables.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-07-02 02:57:17.000000 pretty-tables-3.0.0/pretty_tables.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-07-02 02:57:17.000000 pretty-tables-3.0.0/pretty_tables.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 02:57:17.000000 pretty-tables-3.0.0/pretty_tables.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-02 02:57:17.000000 pretty-tables-3.0.0/pretty_tables.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-02 02:57:17.000000 pretty-tables-3.0.0/pretty_tables.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-02 02:56:48.000000 pretty-tables-3.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 02:57:17.951873 pretty-tables-3.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-07-02 02:56:48.000000 pretty-tables-3.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 02:57:17.951873 pretty-tables-3.0.0/test/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 02:57:17.951873 pretty-tables-3.0.0/test/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 02:56:48.000000 pretty-tables-3.0.0/test/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-07-02 02:56:48.000000 pretty-tables-3.0.0/test/unit/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-07-02 02:56:48.000000 pretty-tables-3.0.0/test/unit/test_formatting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-07-02 02:56:48.000000 pretty-tables-3.0.0/test/unit/test_tables.py
```

### Comparing `pretty-tables-2.0.3/LICENSE` & `pretty-tables-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pretty-tables-2.0.3/PKG-INFO` & `pretty-tables-3.0.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: pretty-tables
-Version: 2.0.3
+Version: 3.0.0
 Summary: Create pretty tables from headers and rows, perfect for console output.
 Home-page: http://github.com/justintime50/pretty-tables
 Author: Justintime50
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
 
 # Pretty Tables
@@ -34,15 +33,15 @@
 ## Install
 
 ```bash
 # Install package
 pip3 install pretty-tables
 
 # Install locally
-make install
+just install
 ```
 
 ## Usage
 
 Pretty Tables is simple to use. Create a table by calling `pretty_tables.create()`, pass a list of headers and a 2 dimensional list of rows (each row must match the length of the headers). Pass an optional `empty_cell_placeholder` string, `colors` list, or a `truthy` index to customize your Pretty Table.
 
 Pretty Tables will automatically validate the input and convert each item to a string before returning successfully; however, you can pass Pretty Tables any data type within the header or row lists. In the following example, we are using `integers`, `booleans`, `None`, and `strings`:
@@ -77,31 +76,29 @@
 print(table)
 ```
 
 ### Colors
 
 You can also color each column differently by using the `colors` argument and passing a list of colors from the `pretty_tables.Colors` class. The input list must match the length of the headers list.
 
-* black
-* blue
-* cyan
-* green
-* purple
-* red
-* white
-* yellow
-* bold
-* reset (resets all text formatting)
-* underline
+- black
+- blue
+- cyan
+- green
+- purple
+- red
+- white
+- yellow
+- bold
+- reset (resets all text formatting)
+- underline
 
 ## Development
 
 ```bash
 # Get a comprehensive list of development tools
-make help
+just --list
 ```
 
 ## Attribution
 
 - [Stack Overflow question on formatting tables for console](https://stackoverflow.com/a/8356620/865091)
-
-
```

### Comparing `pretty-tables-2.0.3/README.md` & `pretty-tables-3.0.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 ## Install
 
 ```bash
 # Install package
 pip3 install pretty-tables
 
 # Install locally
-make install
+just install
 ```
 
 ## Usage
 
 Pretty Tables is simple to use. Create a table by calling `pretty_tables.create()`, pass a list of headers and a 2 dimensional list of rows (each row must match the length of the headers). Pass an optional `empty_cell_placeholder` string, `colors` list, or a `truthy` index to customize your Pretty Table.
 
 Pretty Tables will automatically validate the input and convert each item to a string before returning successfully; however, you can pass Pretty Tables any data type within the header or row lists. In the following example, we are using `integers`, `booleans`, `None`, and `strings`:
@@ -61,29 +61,29 @@
 print(table)
 ```
 
 ### Colors
 
 You can also color each column differently by using the `colors` argument and passing a list of colors from the `pretty_tables.Colors` class. The input list must match the length of the headers list.
 
-* black
-* blue
-* cyan
-* green
-* purple
-* red
-* white
-* yellow
-* bold
-* reset (resets all text formatting)
-* underline
+- black
+- blue
+- cyan
+- green
+- purple
+- red
+- white
+- yellow
+- bold
+- reset (resets all text formatting)
+- underline
 
 ## Development
 
 ```bash
 # Get a comprehensive list of development tools
-make help
+just --list
 ```
 
 ## Attribution
 
 - [Stack Overflow question on formatting tables for console](https://stackoverflow.com/a/8356620/865091)
```

### Comparing `pretty-tables-2.0.3/pretty_tables/formatting.py` & `pretty-tables-3.0.0/pretty_tables/formatting.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,12 @@
-from typing import Any, List, Optional
+from typing import (
+    Any,
+    List,
+    Optional,
+)
 
 
 class Colors:
     """A collection of colors and formatters you can use to customize
     the output of your pretty table.
     """
```

### Comparing `pretty-tables-2.0.3/pretty_tables/tables.py` & `pretty-tables-3.0.0/pretty_tables/tables.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,17 @@
-from typing import Any, List, Optional
+from typing import (
+    Any,
+    List,
+    Optional,
+)
 
-from pretty_tables.formatting import Colors, _format_table
+from pretty_tables.formatting import (
+    Colors,
+    _format_table,
+)
 
 
 def create(
     headers: List[Any],
     rows: List[List[Any]],
     empty_cell_placeholder: Optional[str] = None,
     colors: Optional[List[Colors]] = None,
```

### Comparing `pretty-tables-2.0.3/pretty_tables.egg-info/PKG-INFO` & `pretty-tables-3.0.0/pretty_tables.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: pretty-tables
-Version: 2.0.3
+Version: 3.0.0
 Summary: Create pretty tables from headers and rows, perfect for console output.
 Home-page: http://github.com/justintime50/pretty-tables
 Author: Justintime50
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
 
 # Pretty Tables
@@ -34,15 +33,15 @@
 ## Install
 
 ```bash
 # Install package
 pip3 install pretty-tables
 
 # Install locally
-make install
+just install
 ```
 
 ## Usage
 
 Pretty Tables is simple to use. Create a table by calling `pretty_tables.create()`, pass a list of headers and a 2 dimensional list of rows (each row must match the length of the headers). Pass an optional `empty_cell_placeholder` string, `colors` list, or a `truthy` index to customize your Pretty Table.
 
 Pretty Tables will automatically validate the input and convert each item to a string before returning successfully; however, you can pass Pretty Tables any data type within the header or row lists. In the following example, we are using `integers`, `booleans`, `None`, and `strings`:
@@ -77,31 +76,29 @@
 print(table)
 ```
 
 ### Colors
 
 You can also color each column differently by using the `colors` argument and passing a list of colors from the `pretty_tables.Colors` class. The input list must match the length of the headers list.
 
-* black
-* blue
-* cyan
-* green
-* purple
-* red
-* white
-* yellow
-* bold
-* reset (resets all text formatting)
-* underline
+- black
+- blue
+- cyan
+- green
+- purple
+- red
+- white
+- yellow
+- bold
+- reset (resets all text formatting)
+- underline
 
 ## Development
 
 ```bash
 # Get a comprehensive list of development tools
-make help
+just --list
 ```
 
 ## Attribution
 
 - [Stack Overflow question on formatting tables for console](https://stackoverflow.com/a/8356620/865091)
-
-
```

### Comparing `pretty-tables-2.0.3/setup.py` & `pretty-tables-3.0.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,36 +1,48 @@
 import setuptools
 
+
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 DEV_REQUIREMENTS = [
-    'black',
-    'coveralls == 3.*',
-    'flake8',
-    'isort',
-    'mypy',
-    'pytest == 6.*',
-    'pytest-cov == 2.*',
+    'bandit == 1.7.*',
+    'black == 23.*',
+    'build == 0.7.*',
+    'flake8 == 6.*',
+    'isort == 5.*',
+    'mypy == 1.3.*',
+    'pytest == 7.*',
+    'pytest-cov == 4.*',
+    'twine == 4.*',
 ]
 
 setuptools.setup(
     name='pretty-tables',
-    version='2.0.3',
+    version='3.0.0',
     description='Create pretty tables from headers and rows, perfect for console output.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='http://github.com/justintime50/pretty-tables',
     author='Justintime50',
     license='MIT',
-    packages=setuptools.find_packages(),
-    package_data={'pretty_tables': ['py.typed']},
+    packages=setuptools.find_packages(
+        exclude=[
+            'examples',
+            'test',
+        ]
+    ),
+    package_data={
+        'pretty_tables': [
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

### Comparing `pretty-tables-2.0.3/test/unit/conftest.py` & `pretty-tables-3.0.0/test/unit/conftest.py`

 * *Files identical despite different names*

### Comparing `pretty-tables-2.0.3/test/unit/test_formatting.py` & `pretty-tables-3.0.0/test/unit/test_formatting.py`

 * *Files identical despite different names*

### Comparing `pretty-tables-2.0.3/test/unit/test_tables.py` & `pretty-tables-3.0.0/test/unit/test_tables.py`

 * *Files identical despite different names*

