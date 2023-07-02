# Comparing `tmp/squirrels-0.1.0.tar.gz` & `tmp/squirrels-0.1.1.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "squirrels-0.1.0.tar", last modified: Sun Jun 11 17:47:35 2023, max compression
+gzip compressed data, was "squirrels-0.1.1.post1.tar", last modified: Sun Jul  2 19:55:52 2023, max compression
```

## Comparing `squirrels-0.1.0.tar` & `squirrels-0.1.1.post1.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxrwxrwx   0        0        0        0 2023-06-11 17:47:35.319227 squirrels-0.1.0/
--rw-rw-rw-   0        0        0     1088 2023-04-24 03:56:44.000000 squirrels-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     1959 2023-06-11 17:47:35.317227 squirrels-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1705 2023-05-19 13:23:55.000000 squirrels-0.1.0/README.md
--rw-rw-rw-   0        0        0       42 2023-06-11 17:47:35.320229 squirrels-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1407 2023-06-11 17:43:54.000000 squirrels-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-11 17:47:35.180132 squirrels-0.1.0/squirrels/
--rw-rw-rw-   0        0        0      822 2023-06-11 15:20:47.000000 squirrels-0.1.0/squirrels/__init__.py
--rw-rw-rw-   0        0        0     6455 2023-06-11 15:20:47.000000 squirrels-0.1.0/squirrels/_api_server.py
--rw-rw-rw-   0        0        0     5978 2023-06-11 15:20:47.000000 squirrels-0.1.0/squirrels/_command_line.py
--rw-rw-rw-   0        0        0     1901 2023-06-11 15:20:47.000000 squirrels-0.1.0/squirrels/_constants.py
--rw-rw-rw-   0        0        0     3063 2023-05-19 13:23:55.000000 squirrels-0.1.0/squirrels/_credentials_manager.py
--rw-rw-rw-   0        0        0     4839 2023-05-19 13:23:55.000000 squirrels-0.1.0/squirrels/_initializer.py
--rw-rw-rw-   0        0        0     8292 2023-06-11 15:20:47.000000 squirrels-0.1.0/squirrels/_manifest.py
--rw-rw-rw-   0        0        0     1257 2023-05-19 13:23:55.000000 squirrels-0.1.0/squirrels/_module_loader.py
--rw-rw-rw-   0        0        0     6176 2023-06-11 15:20:47.000000 squirrels-0.1.0/squirrels/_parameter_set.py
--rw-rw-rw-   0        0        0    14484 2023-06-11 15:20:47.000000 squirrels-0.1.0/squirrels/_renderer.py
--rw-rw-rw-   0        0        0     1179 2023-05-19 13:23:55.000000 squirrels-0.1.0/squirrels/_timed_imports.py
--rw-rw-rw-   0        0        0     4170 2023-05-19 13:23:55.000000 squirrels-0.1.0/squirrels/_utils.py
--rw-rw-rw-   0        0        0       95 2023-05-19 13:23:55.000000 squirrels-0.1.0/squirrels/_version.py
--rw-rw-rw-   0        0        0     4382 2023-06-11 15:20:47.000000 squirrels-0.1.0/squirrels/connection_set.py
--rw-rw-rw-   0        0        0    12943 2023-05-19 13:23:55.000000 squirrels-0.1.0/squirrels/data_sources.py
--rw-rw-rw-   0        0        0    13433 2023-06-11 17:43:41.000000 squirrels-0.1.0/squirrels/dateutils.py
-drwxrwxrwx   0        0        0        0 2023-06-11 17:47:35.111131 squirrels-0.1.0/squirrels/package_data/
-drwxrwxrwx   0        0        0        0 2023-06-11 17:47:35.223680 squirrels-0.1.0/squirrels/package_data/base_project/
--rw-rw-rw-   0        0        0       40 2023-05-05 13:52:42.000000 squirrels-0.1.0/squirrels/package_data/base_project/.gitignore
--rw-rw-rw-   0        0        0      923 2023-05-30 22:48:25.000000 squirrels-0.1.0/squirrels/package_data/base_project/connections.py
-drwxrwxrwx   0        0        0        0 2023-06-11 17:47:35.231687 squirrels-0.1.0/squirrels/package_data/base_project/database/
--rw-rw-rw-   0        0        0     8192 2023-04-23 00:05:57.000000 squirrels-0.1.0/squirrels/package_data/base_project/database/sample_database.db
--rw-rw-rw-   0        0        0   188416 2023-03-18 14:11:28.000000 squirrels-0.1.0/squirrels/package_data/base_project/database/seattle_weather.db
-drwxrwxrwx   0        0        0        0 2023-06-11 17:47:35.108136 squirrels-0.1.0/squirrels/package_data/base_project/datasets/
-drwxrwxrwx   0        0        0        0 2023-06-11 17:47:35.293707 squirrels-0.1.0/squirrels/package_data/base_project/datasets/sample_dataset/
--rw-rw-rw-   0        0        0      306 2023-06-11 15:20:47.000000 squirrels-0.1.0/squirrels/package_data/base_project/datasets/sample_dataset/context.py
--rw-rw-rw-   0        0        0      929 2023-06-11 15:20:47.000000 squirrels-0.1.0/squirrels/package_data/base_project/datasets/sample_dataset/database_view1.py
--rw-rw-rw-   0        0        0      376 2023-05-09 13:28:24.000000 squirrels-0.1.0/squirrels/package_data/base_project/datasets/sample_dataset/database_view1.sql.j2
--rw-rw-rw-   0        0        0      320 2023-06-11 15:20:47.000000 squirrels-0.1.0/squirrels/package_data/base_project/datasets/sample_dataset/final_view.py
--rw-rw-rw-   0        0        0       31 2023-03-20 06:10:47.000000 squirrels-0.1.0/squirrels/package_data/base_project/datasets/sample_dataset/final_view.sql.j2
--rw-rw-rw-   0        0        0     1429 2023-06-11 15:20:47.000000 squirrels-0.1.0/squirrels/package_data/base_project/datasets/sample_dataset/parameters.py
--rw-rw-rw-   0        0        0      148 2023-06-11 15:20:47.000000 squirrels-0.1.0/squirrels/package_data/base_project/datasets/sample_dataset/selections.cfg
--rw-rw-rw-   0        0        0      728 2023-05-09 13:28:24.000000 squirrels-0.1.0/squirrels/package_data/base_project/squirrels.yaml
-drwxrwxrwx   0        0        0        0 2023-06-11 17:47:35.303696 squirrels-0.1.0/squirrels/package_data/static/
--rw-rw-rw-   0        0        0     4638 2023-03-12 05:51:40.000000 squirrels-0.1.0/squirrels/package_data/static/favicon.ico
--rw-rw-rw-   0        0        0     9179 2023-05-19 13:23:55.000000 squirrels-0.1.0/squirrels/package_data/static/script.js
--rw-rw-rw-   0        0        0     1841 2023-03-12 03:03:14.000000 squirrels-0.1.0/squirrels/package_data/static/style.css
-drwxrwxrwx   0        0        0        0 2023-06-11 17:47:35.314225 squirrels-0.1.0/squirrels/package_data/templates/
--rw-rw-rw-   0        0        0     1276 2023-06-11 15:20:47.000000 squirrels-0.1.0/squirrels/package_data/templates/index.html
--rw-rw-rw-   0        0        0     8281 2023-06-10 21:13:17.000000 squirrels-0.1.0/squirrels/parameter_options.py
--rw-rw-rw-   0        0        0    32879 2023-06-11 17:43:41.000000 squirrels-0.1.0/squirrels/parameters.py
-drwxrwxrwx   0        0        0        0 2023-06-11 17:47:35.214681 squirrels-0.1.0/squirrels.egg-info/
--rw-rw-rw-   0        0        0     1959 2023-06-11 17:47:35.000000 squirrels-0.1.0/squirrels.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1663 2023-06-11 17:47:35.000000 squirrels-0.1.0/squirrels.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-11 17:47:35.000000 squirrels-0.1.0/squirrels.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-06-11 17:47:35.000000 squirrels-0.1.0/squirrels.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       95 2023-06-11 17:47:35.000000 squirrels-0.1.0/squirrels.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-11 17:47:35.000000 squirrels-0.1.0/squirrels.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 19:55:52.060043 squirrels-0.1.1.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-02 19:55:41.000000 squirrels-0.1.1.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-07-02 19:55:52.060043 squirrels-0.1.1.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-07-02 19:55:41.000000 squirrels-0.1.1.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 19:55:52.060043 squirrels-0.1.1.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-07-02 19:55:41.000000 squirrels-0.1.1.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 19:55:52.060043 squirrels-0.1.1.post1/squirrels/
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-07-02 19:55:41.000000 squirrels-0.1.1.post1/squirrels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6321 2023-07-02 19:55:41.000000 squirrels-0.1.1.post1/squirrels/_api_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5871 2023-07-02 19:55:41.000000 squirrels-0.1.1.post1/squirrels/_command_line.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-07-02 19:55:41.000000 squirrels-0.1.1.post1/squirrels/_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-07-02 19:55:41.000000 squirrels-0.1.1.post1/squirrels/_credentials_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4730 2023-07-02 19:55:41.000000 squirrels-0.1.1.post1/squirrels/_initializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8105 2023-07-02 19:55:41.000000 squirrels-0.1.1.post1/squirrels/_manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-07-02 19:55:41.000000 squirrels-0.1.1.post1/squirrels/_module_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6025 2023-07-02 19:55:41.000000 squirrels-0.1.1.post1/squirrels/_parameter_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14198 2023-07-02 19:55:41.000000 squirrels-0.1.1.post1/squirrels/_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-07-02 19:55:41.000000 squirrels-0.1.1.post1/squirrels/_timed_imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4021 2023-07-02 19:55:41.000000 squirrels-0.1.1.post1/squirrels/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-02 19:55:41.000000 squirrels-0.1.1.post1/squirrels/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4256 2023-07-02 19:55:41.000000 squirrels-0.1.1.post1/squirrels/connection_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13111 2023-07-02 19:55:41.000000 squirrels-0.1.1.post1/squirrels/data_sources.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15393 2023-07-02 19:55:41.000000 squirrels-0.1.1.post1/squirrels/dateutils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 19:55:52.056043 squirrels-0.1.1.post1/squirrels/package_data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 19:55:52.060043 squirrels-0.1.1.post1/squirrels/package_data/base_project/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-02 19:55:41.000000 squirrels-0.1.1.post1/squirrels/package_data/base_project/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-07-02 19:55:41.000000 squirrels-0.1.1.post1/squirrels/package_data/base_project/connections.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 19:55:52.060043 squirrels-0.1.1.post1/squirrels/package_data/base_project/database/
+-rw-r--r--   0 runner    (1001) docker     (123)    32768 2023-07-02 19:55:41.000000 squirrels-0.1.1.post1/squirrels/package_data/base_project/database/sample_database.db
+-rw-r--r--   0 runner    (1001) docker     (123)   188416 2023-07-02 19:55:41.000000 squirrels-0.1.1.post1/squirrels/package_data/base_project/database/seattle_weather.db
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 19:55:52.056043 squirrels-0.1.1.post1/squirrels/package_data/base_project/datasets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 19:55:52.060043 squirrels-0.1.1.post1/squirrels/package_data/base_project/datasets/sample_dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-02 19:55:41.000000 squirrels-0.1.1.post1/squirrels/package_data/base_project/datasets/sample_dataset/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-07-02 19:55:41.000000 squirrels-0.1.1.post1/squirrels/package_data/base_project/datasets/sample_dataset/database_view1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-07-02 19:55:41.000000 squirrels-0.1.1.post1/squirrels/package_data/base_project/datasets/sample_dataset/database_view1.sql.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-07-02 19:55:41.000000 squirrels-0.1.1.post1/squirrels/package_data/base_project/datasets/sample_dataset/final_view.py
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-02 19:55:41.000000 squirrels-0.1.1.post1/squirrels/package_data/base_project/datasets/sample_dataset/final_view.sql.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-07-02 19:55:41.000000 squirrels-0.1.1.post1/squirrels/package_data/base_project/datasets/sample_dataset/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-02 19:55:41.000000 squirrels-0.1.1.post1/squirrels/package_data/base_project/datasets/sample_dataset/selections.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-07-02 19:55:41.000000 squirrels-0.1.1.post1/squirrels/package_data/base_project/squirrels.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 19:55:52.060043 squirrels-0.1.1.post1/squirrels/package_data/static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4638 2023-07-02 19:55:41.000000 squirrels-0.1.1.post1/squirrels/package_data/static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     8946 2023-07-02 19:55:41.000000 squirrels-0.1.1.post1/squirrels/package_data/static/script.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-07-02 19:55:41.000000 squirrels-0.1.1.post1/squirrels/package_data/static/style.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 19:55:52.060043 squirrels-0.1.1.post1/squirrels/package_data/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-07-02 19:55:41.000000 squirrels-0.1.1.post1/squirrels/package_data/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     9922 2023-07-02 19:55:41.000000 squirrels-0.1.1.post1/squirrels/parameter_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34151 2023-07-02 19:55:41.000000 squirrels-0.1.1.post1/squirrels/parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 19:55:52.060043 squirrels-0.1.1.post1/squirrels.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-07-02 19:55:52.000000 squirrels-0.1.1.post1/squirrels.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-07-02 19:55:52.000000 squirrels-0.1.1.post1/squirrels.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 19:55:52.000000 squirrels-0.1.1.post1/squirrels.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-02 19:55:52.000000 squirrels-0.1.1.post1/squirrels.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-02 19:55:52.000000 squirrels-0.1.1.post1/squirrels.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-02 19:55:52.000000 squirrels-0.1.1.post1/squirrels.egg-info/top_level.txt
```

### Comparing `squirrels-0.1.0/LICENSE` & `squirrels-0.1.1.post1/LICENSE`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-MIT License
-
-Copyright (c) 2023 Tim Huang
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2023 Tim Huang
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `squirrels-0.1.0/PKG-INFO` & `squirrels-0.1.1.post1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,56 +1,46 @@
-Metadata-Version: 2.1
-Name: squirrels
-Version: 0.1.0
-Summary: Python Package for Configuring SQL Generating APIs
-Author: Tim Huang
-Author-email: tim.yuting@hotmail.com
-License: MIT
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Squirrels
-
-Squirrels is an API framework for creating REST APIs that generate sql queries & dataframes dynamically from query parameters. 
-
-## Setup
-
-First, install the library and all dependencies **in a new virtual environment**.
-
-```bash
-# create and activate virtual environment...
-pip install -e .
-```
-
-To confirm that the setup worked, run this to show the help page for all squirrels CLI commands:
-
-```bash
-squirrels -h
-```
-
-## Testing
-
-```
-python setup.py pytest
-```
-
-## Usage Documentation
-
-To learn about using the squirrels framework, check out the documentation website [here](https://squirrels-nest.github.io/squirrels-docs/).
-
-## Developer Guide
-
-From the root of the git repo, the source code can be found in the `squirrels` folder and unit tests can be found in the `tests` folder.
-
-To understand what a specific squirrels command line utility is doing, start from the `_command_line.py` file as your entry point.
-
-The library version is maintained in both the `setup.py` file (for the next release or release-candidate version) and the `squirrels/_version.py` file (for the next release version only).
-
-When a user initializes a squirrels project using `squirrels init`, the files are copied from the `squirrels/package_data/base_project` folder. The contents in the `database` subfolder were constructed from the scripts in the `database_elt` folder at the top level.
-
-For the Squirrels UI activated by `squirrels run`, the HTML, CSS, and Javascript files can be found in the `static` and `templates` subfolders of `squirrels/package_data`.
-
-## License
-
-Squirrels is released under the MIT license.
-
-See the file LICENSE for more details.
+# Squirrels
+
+Squirrels is an API framework that lets you create REST APIs for dynamic BI analytics!
+
+## Setup
+
+First, install the library and all dependencies **in a new virtual environment**.
+
+```bash
+# create and activate virtual environment...
+pip install -e .
+```
+
+To confirm that the setup worked, run this to show the help page for all squirrels CLI commands:
+
+```bash
+squirrels -h
+```
+
+## Testing
+
+```
+python setup.py pytest
+```
+
+## Usage Documentation
+
+To learn about using the squirrels framework, check out the documentation website [here](https://squirrels-nest.github.io/squirrels-docs/).
+
+## Developer Guide
+
+From the root of the git repo, the source code can be found in the `squirrels` folder and unit tests can be found in the `tests` folder.
+
+To understand what a specific squirrels command line utility is doing, start from the `_command_line.py` file as your entry point.
+
+The library version is maintained in both the `setup.py` file (for the next release or release-candidate version) and the `squirrels/_version.py` file (for the next release version only).
+
+When a user initializes a squirrels project using `squirrels init`, the files are copied from the `squirrels/package_data/base_project` folder. The contents in the `database` subfolder were constructed from the scripts in the `database_elt` folder at the top level.
+
+For the Squirrels UI activated by `squirrels run`, the HTML, CSS, and Javascript files can be found in the `static` and `templates` subfolders of `squirrels/package_data`.
+
+## License
+
+Squirrels is released under the MIT license.
+
+See the file LICENSE for more details.
```

### Comparing `squirrels-0.1.0/setup.py` & `squirrels-0.1.1.post1/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-from setuptools import setup, find_packages
-import os
-
-# The directory containing this file
-HERE = os.path.abspath(os.path.dirname(__file__))
-
-# Get the long description from the README file
-with open(os.path.join(HERE, 'README.md'), encoding='utf-8') as f:
-    long_description = f.read()
-
-# Recursively get package data
-def package_files(directory):
-    paths = []
-    for (path, directories, filenames) in os.walk(directory):
-        for filename in filenames:
-            paths.append(os.path.join('..', path, filename))
-    return paths
-
-extra_files = package_files(os.path.join('squirrels', 'package_data'))
-
-setup(
-    name='squirrels',
-    version='0.1.0',
-    packages=find_packages(),
-    description='Python Package for Configuring SQL Generating APIs',
-    long_description=long_description,
-    long_description_content_type="text/markdown",
-    author='Tim Huang',
-    author_email='tim.yuting@hotmail.com',
-    license='MIT',
-    install_requires=[
-        'openpyxl', 'inquirer', 'pwinput', 'cachetools', 'fastapi', 'uvicorn', 
-        'Jinja2', 'GitPython', 'sqlalchemy', 'pandas', 'pyyaml'
-    ],
-    setup_requires=['pytest-runner==6.0.0'],
-    tests_require=['pytest==7.2.0'],
-    test_suite='tests',
-    package_data= {'squirrels': extra_files},
-    entry_points= {
-        'console_scripts': ['squirrels=squirrels._command_line:main']
-    }
-)
+from setuptools import setup, find_packages
+import os
+
+# The directory containing this file
+HERE = os.path.abspath(os.path.dirname(__file__))
+
+# Get the long description from the README file
+with open(os.path.join(HERE, 'README.md'), encoding='utf-8') as f:
+    long_description = f.read()
+
+# Recursively get package data
+def package_files(directory):
+    paths = []
+    for (path, directories, filenames) in os.walk(directory):
+        for filename in filenames:
+            paths.append(os.path.join('..', path, filename))
+    return paths
+
+extra_files = package_files(os.path.join('squirrels', 'package_data'))
+
+setup(
+    name='squirrels',
+    version='0.1.1.post1',
+    packages=find_packages(),
+    description='Squirrels - Configure REST APIs for BI Analytics',
+    long_description=long_description,
+    long_description_content_type="text/markdown",
+    author='Tim Huang',
+    author_email='tim.yuting@hotmail.com',
+    license='MIT',
+    install_requires=[
+        'openpyxl', 'inquirer', 'pwinput', 'cachetools', 'fastapi', 'uvicorn', 
+        'Jinja2', 'GitPython', 'sqlalchemy', 'pandas', 'pyyaml'
+    ],
+    setup_requires=['pytest-runner==6.0.0'],
+    tests_require=['pytest==7.2.0'],
+    test_suite='tests',
+    package_data= {'squirrels': extra_files},
+    entry_points= {
+        'console_scripts': ['squirrels=squirrels._command_line:main']
+    }
+)
```

### Comparing `squirrels-0.1.0/squirrels/__init__.py` & `squirrels-0.1.1.post1/squirrels/__init__.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-from .parameter_options import SelectParameterOption, DateParameterOption, NumberParameterOption, NumRangeParameterOption
-from .parameters import Parameter, SingleSelectParameter, MultiSelectParameter, DateParameter, NumberParameter, NumRangeParameter, DataSourceParameter
-from .data_sources import SelectionDataSource, DateDataSource, NumberDataSource, NumRangeDataSource
-from .connection_set import ConnectionSet
-
-
-def get_credential(key: str):
-    """
-    Gets the username and password that was set through "$squirrels set-credential [key]"
-
-    Parameters:
-        key (str): The credential key
-    
-    Returns:
-        Credential: Object with attributes "username" and "password"
-    """
-    from ._credentials_manager import squirrels_config_io
-    return squirrels_config_io.get_credential(key)
+from .parameter_options import SelectParameterOption, DateParameterOption, NumberParameterOption, NumRangeParameterOption
+from .parameters import Parameter, SingleSelectParameter, MultiSelectParameter, DateParameter, NumberParameter, NumRangeParameter, DataSourceParameter
+from .data_sources import SelectionDataSource, DateDataSource, NumberDataSource, NumRangeDataSource
+from .connection_set import ConnectionSet
+
+
+def get_credential(key: str):
+    """
+    Gets the username and password that was set through "$squirrels set-credential [key]"
+
+    Parameters:
+        key (str): The credential key
+    
+    Returns:
+        Credential: Object with attributes "username" and "password"
+    """
+    from ._credentials_manager import squirrels_config_io
+    return squirrels_config_io.get_credential(key)
```

### Comparing `squirrels-0.1.0/squirrels/_api_server.py` & `squirrels-0.1.1.post1/squirrels/_api_server.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,134 +1,134 @@
-from typing import Dict, List, Tuple, Set
-from fastapi import FastAPI, Request, HTTPException
-from fastapi.datastructures import QueryParams
-from fastapi.responses import HTMLResponse, JSONResponse
-from fastapi.templating import Jinja2Templates
-from fastapi.staticfiles import StaticFiles
-from cachetools.func import ttl_cache
-import os, traceback
-
-from squirrels import _constants as c, _utils
-from squirrels._version import major_version
-from squirrels._manifest import Manifest
-from squirrels.connection_set import ConnectionSet
-from squirrels._renderer import RendererIOWrapper, Renderer
-
-
-class ApiServer:
-    def __init__(self, manifest: Manifest, conn_set: ConnectionSet, no_cache: bool, debug: bool) -> None:
-        """
-        Constructor for ApiServer
-
-        Parameters:
-            manifest (Manifest): Manifest object produced from squirrels.yaml
-            conn_set (ConnectionSet): Set of all connection pools defined in connections.py
-            no_cache (bool): Whether to disable caching
-            debug (bool): Set to True to show "hidden" parameters in the /parameters endpoint response
-        """
-        self.manifest = manifest
-        self.conn_set = conn_set
-        self.no_cache = no_cache
-        self.debug = debug
-        
-        self.datasets = manifest.get_all_dataset_names()
-        self.renderers: Dict[str, Renderer] = {}
-        for dataset in self.datasets:
-            rendererIO = RendererIOWrapper(dataset, manifest, conn_set)
-            self.renderers[dataset] = rendererIO.renderer
-        
-    def _get_parameters_helper(self, dataset: str, query_params: Set[Tuple[str, str]]) -> Dict:
-        if len(query_params) > 1:
-            raise _utils.InvalidInputError("The /parameters endpoint takes at most 1 query parameter")
-        renderer = self.renderers[dataset]
-        parameters = renderer.apply_selections(dict(query_params), updates_only = True)
-        return parameters.to_json_dict(self.debug)
-    
-    def _get_results_helper(self, dataset: str, query_params: Set[Tuple[str, str]]) -> Dict:
-        renderer = self.renderers[dataset]
-        _, _, _, _, df = renderer.load_results(dict(query_params))
-        return _utils.df_to_json(df)
-
-    def _apply_api_function(self, api_function):
-        try:
-            return api_function()
-        except _utils.InvalidInputError as e:
-            traceback.print_exc()
-            raise HTTPException(status_code=400, detail="Invalid User Input: "+str(e)) from e
-        except _utils.ConfigurationError as e:
-            traceback.print_exc()
-            raise HTTPException(status_code=500, detail="Squirrels Configuration Error: "+str(e)) from e
-        except Exception as e:
-            traceback.print_exc()
-            raise HTTPException(status_code=500, detail="Squirrels Framework Error: "+str(e)) from e
-    
-    def _apply_dataset_api_function(self, api_function, dataset: str, raw_query_params: QueryParams):
-        dataset = _utils.normalize_name(dataset)
-        query_params = set()
-        for key, val in raw_query_params.items():
-            query_params.add((_utils.normalize_name(key), val))
-        query_params = frozenset(query_params)
-        return self._apply_api_function(lambda: api_function(dataset, query_params))
-    
-    def run(self, uvicorn_args: List[str]) -> None:
-        """
-        Runs the API server with uvicorn for CLI "squirrels run"
-
-        Parameters:
-            uvicorn_args (List[str]): List of arguments to pass to uvicorn.run. Currently only supports "host" and "port"
-        """
-        app = FastAPI()
-
-        squirrels_version_path = f'/squirrels{major_version}'
-        config_base_path = _utils.normalize_name_for_api(self.manifest.get_base_path())
-        base_path = squirrels_version_path + config_base_path
-
-        static_dir = _utils.join_paths(os.path.dirname(__file__), 'package_data', 'static')
-        app.mount('/static', StaticFiles(directory=static_dir), name='static')
-
-        templates_dir = _utils.join_paths(os.path.dirname(__file__), 'package_data', 'templates')
-        templates = Jinja2Templates(directory=templates_dir)
-
-        # Parameters API
-        parameters_path = base_path + '/{dataset}/parameters'
-        
-        parameters_cache_size = self.manifest.get_setting(c.PARAMETERS_CACHE_SIZE_SETTING, 1024)
-        parameters_cache_ttl = self.manifest.get_setting(c.PARAMETERS_CACHE_TTL_SETTING, 24*60*60)
-
-        @ttl_cache(maxsize=parameters_cache_size, ttl=parameters_cache_ttl)
-        def get_parameters_cachable(*args):
-            return self._get_parameters_helper(*args)
-        
-        @app.get(parameters_path, response_class=JSONResponse)
-        async def get_parameters(dataset: str, request: Request):
-            api_function = self._get_parameters_helper if self.no_cache else get_parameters_cachable
-            return self._apply_dataset_api_function(api_function, dataset, request.query_params)
-
-        # Results API
-        results_path = base_path + '/{dataset}'
-
-        results_cache_size = self.manifest.get_setting(c.RESULTS_CACHE_SIZE_SETTING, 128)
-        results_cache_ttl = self.manifest.get_setting(c.RESULTS_CACHE_TTL_SETTING, 60*60)
-
-        @ttl_cache(maxsize=results_cache_size, ttl=results_cache_ttl)
-        def get_results_cachable(*args):
-            return self._get_results_helper(*args)
-        
-        @app.get(results_path, response_class=JSONResponse)
-        async def get_results(dataset: str, request: Request):
-            api_function = self._get_results_helper if self.no_cache else get_results_cachable
-            return self._apply_dataset_api_function(api_function, dataset, request.query_params)
-        
-        # Catalog API
-        @app.get(squirrels_version_path, response_class=JSONResponse)
-        async def get_catalog():
-            api_function = lambda: self.manifest.get_catalog(parameters_path, results_path)
-            return self._apply_api_function(api_function)
-        
-        # Squirrels UI
-        @app.get('/', response_class=HTMLResponse)
-        async def get_ui(request: Request):
-            return templates.TemplateResponse('index.html', {'request': request, 'catalog_path': squirrels_version_path})
-        
-        # Run API server
-        import uvicorn
-        uvicorn.run(app, host=uvicorn_args.host, port=uvicorn_args.port)
+from typing import Dict, List, Tuple, Set
+from fastapi import FastAPI, Request, HTTPException
+from fastapi.datastructures import QueryParams
+from fastapi.responses import HTMLResponse, JSONResponse
+from fastapi.templating import Jinja2Templates
+from fastapi.staticfiles import StaticFiles
+from cachetools.func import ttl_cache
+import os, traceback
+
+from squirrels import _constants as c, _utils
+from squirrels._version import major_version
+from squirrels._manifest import Manifest
+from squirrels.connection_set import ConnectionSet
+from squirrels._renderer import RendererIOWrapper, Renderer
+
+
+class ApiServer:
+    def __init__(self, manifest: Manifest, conn_set: ConnectionSet, no_cache: bool, debug: bool) -> None:
+        """
+        Constructor for ApiServer
+
+        Parameters:
+            manifest (Manifest): Manifest object produced from squirrels.yaml
+            conn_set (ConnectionSet): Set of all connection pools defined in connections.py
+            no_cache (bool): Whether to disable caching
+            debug (bool): Set to True to show "hidden" parameters in the /parameters endpoint response
+        """
+        self.manifest = manifest
+        self.conn_set = conn_set
+        self.no_cache = no_cache
+        self.debug = debug
+        
+        self.datasets = manifest.get_all_dataset_names()
+        self.renderers: Dict[str, Renderer] = {}
+        for dataset in self.datasets:
+            rendererIO = RendererIOWrapper(dataset, manifest, conn_set)
+            self.renderers[dataset] = rendererIO.renderer
+        
+    def _get_parameters_helper(self, dataset: str, query_params: Set[Tuple[str, str]]) -> Dict:
+        if len(query_params) > 1:
+            raise _utils.InvalidInputError("The /parameters endpoint takes at most 1 query parameter")
+        renderer = self.renderers[dataset]
+        parameters = renderer.apply_selections(dict(query_params), updates_only = True)
+        return parameters.to_json_dict(self.debug)
+    
+    def _get_results_helper(self, dataset: str, query_params: Set[Tuple[str, str]]) -> Dict:
+        renderer = self.renderers[dataset]
+        _, _, _, _, df = renderer.load_results(dict(query_params))
+        return _utils.df_to_json(df)
+
+    def _apply_api_function(self, api_function):
+        try:
+            return api_function()
+        except _utils.InvalidInputError as e:
+            traceback.print_exc()
+            raise HTTPException(status_code=400, detail="Invalid User Input: "+str(e)) from e
+        except _utils.ConfigurationError as e:
+            traceback.print_exc()
+            raise HTTPException(status_code=500, detail="Squirrels Configuration Error: "+str(e)) from e
+        except Exception as e:
+            traceback.print_exc()
+            raise HTTPException(status_code=500, detail="Squirrels Framework Error: "+str(e)) from e
+    
+    def _apply_dataset_api_function(self, api_function, dataset: str, raw_query_params: QueryParams):
+        dataset = _utils.normalize_name(dataset)
+        query_params = set()
+        for key, val in raw_query_params.items():
+            query_params.add((_utils.normalize_name(key), val))
+        query_params = frozenset(query_params)
+        return self._apply_api_function(lambda: api_function(dataset, query_params))
+    
+    def run(self, uvicorn_args: List[str]) -> None:
+        """
+        Runs the API server with uvicorn for CLI "squirrels run"
+
+        Parameters:
+            uvicorn_args (List[str]): List of arguments to pass to uvicorn.run. Currently only supports "host" and "port"
+        """
+        app = FastAPI()
+
+        squirrels_version_path = f'/squirrels{major_version}'
+        config_base_path = _utils.normalize_name_for_api(self.manifest.get_base_path())
+        base_path = squirrels_version_path + config_base_path
+
+        static_dir = _utils.join_paths(os.path.dirname(__file__), 'package_data', 'static')
+        app.mount('/static', StaticFiles(directory=static_dir), name='static')
+
+        templates_dir = _utils.join_paths(os.path.dirname(__file__), 'package_data', 'templates')
+        templates = Jinja2Templates(directory=templates_dir)
+
+        # Parameters API
+        parameters_path = base_path + '/{dataset}/parameters'
+        
+        parameters_cache_size = self.manifest.get_setting(c.PARAMETERS_CACHE_SIZE_SETTING, 1024)
+        parameters_cache_ttl = self.manifest.get_setting(c.PARAMETERS_CACHE_TTL_SETTING, 24*60*60)
+
+        @ttl_cache(maxsize=parameters_cache_size, ttl=parameters_cache_ttl)
+        def get_parameters_cachable(*args):
+            return self._get_parameters_helper(*args)
+        
+        @app.get(parameters_path, response_class=JSONResponse)
+        async def get_parameters(dataset: str, request: Request):
+            api_function = self._get_parameters_helper if self.no_cache else get_parameters_cachable
+            return self._apply_dataset_api_function(api_function, dataset, request.query_params)
+
+        # Results API
+        results_path = base_path + '/{dataset}'
+
+        results_cache_size = self.manifest.get_setting(c.RESULTS_CACHE_SIZE_SETTING, 128)
+        results_cache_ttl = self.manifest.get_setting(c.RESULTS_CACHE_TTL_SETTING, 60*60)
+
+        @ttl_cache(maxsize=results_cache_size, ttl=results_cache_ttl)
+        def get_results_cachable(*args):
+            return self._get_results_helper(*args)
+        
+        @app.get(results_path, response_class=JSONResponse)
+        async def get_results(dataset: str, request: Request):
+            api_function = self._get_results_helper if self.no_cache else get_results_cachable
+            return self._apply_dataset_api_function(api_function, dataset, request.query_params)
+        
+        # Catalog API
+        @app.get(squirrels_version_path, response_class=JSONResponse)
+        async def get_catalog():
+            api_function = lambda: self.manifest.get_catalog(parameters_path, results_path)
+            return self._apply_api_function(api_function)
+        
+        # Squirrels UI
+        @app.get('/', response_class=HTMLResponse)
+        async def get_ui(request: Request):
+            return templates.TemplateResponse('index.html', {'request': request, 'catalog_path': squirrels_version_path})
+        
+        # Run API server
+        import uvicorn
+        uvicorn.run(app, host=uvicorn_args.host, port=uvicorn_args.port)
```

### Comparing `squirrels-0.1.0/squirrels/_command_line.py` & `squirrels-0.1.1.post1/squirrels/_command_line.py`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,107 +1,107 @@
-from typing import List, Tuple, Optional
-from argparse import ArgumentParser
-import sys, time, pwinput
-sys.path.append('.')
-
-from squirrels import _constants as c, _credentials_manager as cm, _manifest as mf, _module_loader as ml
-from squirrels import connection_set as cs
-from squirrels._version import __version__
-from squirrels._api_server import ApiServer
-from squirrels._renderer import RendererIOWrapper
-from squirrels._initializer import Initializer
-from squirrels._timed_imports import timer
-
-
-def _prompt_user_pw(args_values: Optional[List[str]]) -> Tuple[str, str]:
-    if args_values is not None:
-        user, pw = args_values
-    else:
-        user = input("Enter username: ")
-        pw = pwinput.pwinput("Enter password: ")
-    return user, pw
-
-
-def main():
-    """
-    Main entry point for the squirrels command line utilities.
-    """
-    start = time.time()
-    parser = ArgumentParser(description="Command line utilities from the squirrels python package")
-    parser.add_argument('-v', '--version', action='store_true', help='Show the version and exit')
-    parser.add_argument('--verbose', action='store_true', help='Enable verbose output')
-    subparsers = parser.add_subparsers(title='commands', dest='command')
-
-    init_parser = subparsers.add_parser(c.INIT_CMD, help='Initialize a squirrels project')
-    init_parser.add_argument('--overwrite', action='store_true', help="Overwrite files that already exist")
-    init_parser.add_argument('--core', action='store_true', help='Include all core files (squirrels.yaml, parameters.py, database view, etc.)')
-    init_parser.add_argument('--db-view', type=str, choices=c.FILE_TYPE_CHOICES, help='Create database view as sql (default) or python file. Ignored if "--core" is not specified')
-    init_parser.add_argument('--connections', action='store_true', help=f'Include the {c.CONNECTIONS_FILE} file')
-    init_parser.add_argument('--context', action='store_true', help=f'Include the {c.CONTEXT_FILE} file')
-    init_parser.add_argument('--selections-cfg', action='store_true', help=f'Include the {c.SELECTIONS_CFG_FILE} file')
-    init_parser.add_argument('--final-view', type=str, choices=c.FILE_TYPE_CHOICES, help='Include final view as sql or python file')
-    init_parser.add_argument('--sample-db', type=str, choices=c.DATABASE_CHOICES, help='Sample sqlite database to include')
-
-    subparsers.add_parser(c.LOAD_MODULES_CMD, help='Load all the modules specified in squirrels.yaml from git')
-
-    def _add_profile_argument(parser: ArgumentParser):
-        parser.add_argument('key', type=str, help='Key to the database connection credential')
-
-    set_cred_parser = subparsers.add_parser(c.SET_CRED_CMD, help='Set a database connection credential key')
-    _add_profile_argument(set_cred_parser)
-    set_cred_parser.add_argument('--values', type=str, nargs=2, help='The username and password')
-
-    subparsers.add_parser(c.GET_CREDS_CMD, help='Get all database connection credential keys')
-
-    delete_cred_parser = subparsers.add_parser(c.DELETE_CRED_CMD, help='Delete a database connection credential key')
-    _add_profile_argument(delete_cred_parser)
-
-    test_parser = subparsers.add_parser(c.TEST_CMD, help='For a given dataset, create outputs for parameter API response and rendered sql queries')
-    test_parser.add_argument('dataset', type=str, help='Name of dataset (provided in squirrels.yaml) to test. Results are written in an "outputs" folder')
-    test_parser.add_argument('-c', '--cfg', type=str, help="Configuration file for parameter selections. Path is relative to the dataset's folder")
-    test_parser.add_argument('-d', '--data', type=str, help="Excel file with lookup data to avoid making a database connection. Path is relative to the dataset's folder")
-    test_parser.add_argument('-r', '--runquery', action='store_true', help='Runs all database queries and final view, and produce the results as csv files')
-
-    run_parser = subparsers.add_parser(c.RUN_CMD, help='Run the builtin API server')
-    run_parser.add_argument('--no-cache', action='store_true', help='Do not cache any api results')
-    run_parser.add_argument('--debug', action='store_true', help='In debug mode, all "hidden parameters" show in the parameters response')
-    run_parser.add_argument('--host', type=str, default='127.0.0.1')
-    run_parser.add_argument('--port', type=int, default=8000)
-
-    args, _ = parser.parse_known_args()
-    timer.verbose = args.verbose
-    timer.add_activity_time('parsing arguments', start)
-
-    if args.version:
-        print(__version__)
-    elif args.command == c.INIT_CMD:
-        Initializer(args.overwrite).init_project(args)
-    elif args.command == c.LOAD_MODULES_CMD:
-        manifest = mf._from_file()
-        ml.load_modules(manifest)
-    elif args.command == c.SET_CRED_CMD:
-        user, pw = _prompt_user_pw(args.values)
-        cm.squirrels_config_io.set_credential(args.key, user, pw)
-    elif args.command == c.GET_CREDS_CMD: 
-        cm.squirrels_config_io.print_all_credentials()
-    elif args.command == c.DELETE_CRED_CMD:
-        cm.squirrels_config_io.delete_credential(args.key)
-    elif args.command in [c.RUN_CMD, c.TEST_CMD]:
-        manifest = mf._from_file()
-        conn_set = cs._from_file(manifest)
-        if args.command == c.RUN_CMD:
-            server = ApiServer(manifest, conn_set, args.no_cache, args.debug)
-            server.run(args)
-        elif args.command == c.TEST_CMD:
-            rendererIO = RendererIOWrapper(args.dataset, manifest, conn_set, args.data)
-            rendererIO.write_outputs(args.cfg, args.runquery)
-        conn_set._dispose()
-    elif args.command is None:
-        print(f'Command is missing. Enter "squirrels -h" for help.')
-    else:
-        print(f'Error: No such command "{args.command}". Enter "squirrels -h" for help.')
-    
-    timer.report_times()
-
-
-if __name__ == '__main__':
-    main()
+from typing import List, Tuple, Optional
+from argparse import ArgumentParser
+import sys, time, pwinput
+sys.path.append('.')
+
+from squirrels import _constants as c, _credentials_manager as cm, _manifest as mf, _module_loader as ml
+from squirrels import connection_set as cs
+from squirrels._version import __version__
+from squirrels._api_server import ApiServer
+from squirrels._renderer import RendererIOWrapper
+from squirrels._initializer import Initializer
+from squirrels._timed_imports import timer
+
+
+def _prompt_user_pw(args_values: Optional[List[str]]) -> Tuple[str, str]:
+    if args_values is not None:
+        user, pw = args_values
+    else:
+        user = input("Enter username: ")
+        pw = pwinput.pwinput("Enter password: ")
+    return user, pw
+
+
+def main():
+    """
+    Main entry point for the squirrels command line utilities.
+    """
+    start = time.time()
+    parser = ArgumentParser(description="Command line utilities from the squirrels python package")
+    parser.add_argument('-v', '--version', action='store_true', help='Show the version and exit')
+    parser.add_argument('--verbose', action='store_true', help='Enable verbose output')
+    subparsers = parser.add_subparsers(title='commands', dest='command')
+
+    init_parser = subparsers.add_parser(c.INIT_CMD, help='Initialize a squirrels project')
+    init_parser.add_argument('--overwrite', action='store_true', help="Overwrite files that already exist")
+    init_parser.add_argument('--core', action='store_true', help='Include all core files (squirrels.yaml, parameters.py, database view, etc.)')
+    init_parser.add_argument('--db-view', type=str, choices=c.FILE_TYPE_CHOICES, help='Create database view as sql (default) or python file. Ignored if "--core" is not specified')
+    init_parser.add_argument('--connections', action='store_true', help=f'Include the {c.CONNECTIONS_FILE} file')
+    init_parser.add_argument('--context', action='store_true', help=f'Include the {c.CONTEXT_FILE} file')
+    init_parser.add_argument('--selections-cfg', action='store_true', help=f'Include the {c.SELECTIONS_CFG_FILE} file')
+    init_parser.add_argument('--final-view', type=str, choices=c.FILE_TYPE_CHOICES, help='Include final view as sql or python file')
+    init_parser.add_argument('--sample-db', type=str, choices=c.DATABASE_CHOICES, help='Sample sqlite database to include')
+
+    subparsers.add_parser(c.LOAD_MODULES_CMD, help='Load all the modules specified in squirrels.yaml from git')
+
+    def _add_profile_argument(parser: ArgumentParser):
+        parser.add_argument('key', type=str, help='Key to the database connection credential')
+
+    set_cred_parser = subparsers.add_parser(c.SET_CRED_CMD, help='Set a database connection credential key')
+    _add_profile_argument(set_cred_parser)
+    set_cred_parser.add_argument('--values', type=str, nargs=2, help='The username and password')
+
+    subparsers.add_parser(c.GET_CREDS_CMD, help='Get all database connection credential keys')
+
+    delete_cred_parser = subparsers.add_parser(c.DELETE_CRED_CMD, help='Delete a database connection credential key')
+    _add_profile_argument(delete_cred_parser)
+
+    test_parser = subparsers.add_parser(c.TEST_CMD, help='For a given dataset, create outputs for parameter API response and rendered sql queries')
+    test_parser.add_argument('dataset', type=str, help='Name of dataset (provided in squirrels.yaml) to test. Results are written in an "outputs" folder')
+    test_parser.add_argument('-c', '--cfg', type=str, help="Configuration file for parameter selections. Path is relative to the dataset's folder")
+    test_parser.add_argument('-d', '--data', type=str, help="Excel file with lookup data to avoid making a database connection. Path is relative to the dataset's folder")
+    test_parser.add_argument('-r', '--runquery', action='store_true', help='Runs all database queries and final view, and produce the results as csv files')
+
+    run_parser = subparsers.add_parser(c.RUN_CMD, help='Run the builtin API server')
+    run_parser.add_argument('--no-cache', action='store_true', help='Do not cache any api results')
+    run_parser.add_argument('--debug', action='store_true', help='In debug mode, all "hidden parameters" show in the parameters response')
+    run_parser.add_argument('--host', type=str, default='127.0.0.1')
+    run_parser.add_argument('--port', type=int, default=8000)
+
+    args, _ = parser.parse_known_args()
+    timer.verbose = args.verbose
+    timer.add_activity_time('parsing arguments', start)
+
+    if args.version:
+        print(__version__)
+    elif args.command == c.INIT_CMD:
+        Initializer(args.overwrite).init_project(args)
+    elif args.command == c.LOAD_MODULES_CMD:
+        manifest = mf._from_file()
+        ml.load_modules(manifest)
+    elif args.command == c.SET_CRED_CMD:
+        user, pw = _prompt_user_pw(args.values)
+        cm.squirrels_config_io.set_credential(args.key, user, pw)
+    elif args.command == c.GET_CREDS_CMD: 
+        cm.squirrels_config_io.print_all_credentials()
+    elif args.command == c.DELETE_CRED_CMD:
+        cm.squirrels_config_io.delete_credential(args.key)
+    elif args.command in [c.RUN_CMD, c.TEST_CMD]:
+        manifest = mf._from_file()
+        conn_set = cs._from_file(manifest)
+        if args.command == c.RUN_CMD:
+            server = ApiServer(manifest, conn_set, args.no_cache, args.debug)
+            server.run(args)
+        elif args.command == c.TEST_CMD:
+            rendererIO = RendererIOWrapper(args.dataset, manifest, conn_set, args.data)
+            rendererIO.write_outputs(args.cfg, args.runquery)
+        conn_set._dispose()
+    elif args.command is None:
+        print(f'Command is missing. Enter "squirrels -h" for help.')
+    else:
+        print(f'Error: No such command "{args.command}". Enter "squirrels -h" for help.')
+    
+    timer.report_times()
+
+
+if __name__ == '__main__':
+    main()
```

### Comparing `squirrels-0.1.0/squirrels/_constants.py` & `squirrels-0.1.1.post1/squirrels/_constants.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,64 +1,64 @@
-# Squirrels CLI commands
-INIT_CMD = 'init'
-LOAD_MODULES_CMD = 'load-modules'
-GET_CREDS_CMD = 'get-all-credentials'
-SET_CRED_CMD = 'set-credential'
-DELETE_CRED_CMD = 'delete-credential'
-TEST_CMD = 'test'
-RUN_CMD = 'run'
-
-# Manifest file keys
-PROJ_VARS_KEY = 'project_variables'
-DB_CONNECTIONS_KEY = 'db_connections'
-DB_CREDENTIALS_KEY = 'credential_key'
-URL_KEY = 'url'
-DB_CONNECTION_KEY = 'db_connection'
-MODULES_KEY = 'modules'
-DATASET_LABEL_KEY = 'label'
-DATASETS_KEY = 'datasets'
-HEADERS_KEY = 'headers'
-DATABASE_VIEWS_KEY = 'database_views'
-FILE_KEY = 'file'
-FINAL_VIEW_KEY = 'final_view'
-BASE_PATH_KEY = 'base_path'
-SETTINGS_KEY = 'settings'
-
-# Project variable keys
-PRODUCT_KEY = 'product'
-MAJOR_VERSION_KEY = 'major_version'
-MINOR_VERSION_KEY = 'minor_version'
-
-# Database credentials keys
-CREDENTIALS_KEY = 'credentials'
-USERNAME_KEY = 'username'
-PASSWORD_KEY = 'password'
-DEFAULT_DB_CONN = 'default'
-
-# Folder/File names
-MANIFEST_FILE = 'squirrels.yaml'
-CONNECTIONS_FILE = 'connections.py'
-OUTPUTS_FOLDER = 'outputs'
-MODULES_FOLDER = 'modules'
-DATASETS_FOLDER = 'datasets'
-PARAMETERS_FILE = 'parameters.py'
-PARAMETERS_OUTPUT = 'parameters.json'
-DATABASE_VIEW_SQL_FILE = 'database_view1.sql.j2'
-DATABASE_VIEW_PY_FILE = 'database_view1.py'
-FINAL_VIEW_SQL_NAME = 'final_view.sql.j2'
-FINAL_VIEW_PY_NAME = 'final_view.py'
-FINAL_VIEW_OUT_STEM = 'final_view'
-CONTEXT_FILE = 'context.py'
-SELECTIONS_CFG_FILE = 'selections.cfg'
-
-# Dataset setting names
-PARAMETERS_CACHE_SIZE_SETTING = 'parameters.cache.size'
-PARAMETERS_CACHE_TTL_SETTING = 'parameters.cache.ttl'
-RESULTS_CACHE_SIZE_SETTING = 'results.cache.size'
-RESULTS_CACHE_TTL_SETTING = 'results.cache.ttl'
-
-# Selection cfg sections
-PARAMETERS_SECTION = 'parameters'
-
-# Init Command Choices
-FILE_TYPE_CHOICES = ['sql', 'py']
-DATABASE_CHOICES = ['sample_database', 'seattle_weather']
+# Squirrels CLI commands
+INIT_CMD = 'init'
+LOAD_MODULES_CMD = 'load-modules'
+GET_CREDS_CMD = 'get-all-credentials'
+SET_CRED_CMD = 'set-credential'
+DELETE_CRED_CMD = 'delete-credential'
+TEST_CMD = 'test'
+RUN_CMD = 'run'
+
+# Manifest file keys
+PROJ_VARS_KEY = 'project_variables'
+DB_CONNECTIONS_KEY = 'db_connections'
+DB_CREDENTIALS_KEY = 'credential_key'
+URL_KEY = 'url'
+DB_CONNECTION_KEY = 'db_connection'
+MODULES_KEY = 'modules'
+DATASET_LABEL_KEY = 'label'
+DATASETS_KEY = 'datasets'
+HEADERS_KEY = 'headers'
+DATABASE_VIEWS_KEY = 'database_views'
+FILE_KEY = 'file'
+FINAL_VIEW_KEY = 'final_view'
+BASE_PATH_KEY = 'base_path'
+SETTINGS_KEY = 'settings'
+
+# Project variable keys
+PRODUCT_KEY = 'product'
+MAJOR_VERSION_KEY = 'major_version'
+MINOR_VERSION_KEY = 'minor_version'
+
+# Database credentials keys
+CREDENTIALS_KEY = 'credentials'
+USERNAME_KEY = 'username'
+PASSWORD_KEY = 'password'
+DEFAULT_DB_CONN = 'default'
+
+# Folder/File names
+MANIFEST_FILE = 'squirrels.yaml'
+CONNECTIONS_FILE = 'connections.py'
+OUTPUTS_FOLDER = 'outputs'
+MODULES_FOLDER = 'modules'
+DATASETS_FOLDER = 'datasets'
+PARAMETERS_FILE = 'parameters.py'
+PARAMETERS_OUTPUT = 'parameters.json'
+DATABASE_VIEW_SQL_FILE = 'database_view1.sql.j2'
+DATABASE_VIEW_PY_FILE = 'database_view1.py'
+FINAL_VIEW_SQL_NAME = 'final_view.sql.j2'
+FINAL_VIEW_PY_NAME = 'final_view.py'
+FINAL_VIEW_OUT_STEM = 'final_view'
+CONTEXT_FILE = 'context.py'
+SELECTIONS_CFG_FILE = 'selections.cfg'
+
+# Dataset setting names
+PARAMETERS_CACHE_SIZE_SETTING = 'parameters.cache.size'
+PARAMETERS_CACHE_TTL_SETTING = 'parameters.cache.ttl'
+RESULTS_CACHE_SIZE_SETTING = 'results.cache.size'
+RESULTS_CACHE_TTL_SETTING = 'results.cache.ttl'
+
+# Selection cfg sections
+PARAMETERS_SECTION = 'parameters'
+
+# Init Command Choices
+FILE_TYPE_CHOICES = ['sql', 'py']
+DATABASE_CHOICES = ['sample_database', 'seattle_weather']
```

### Comparing `squirrels-0.1.0/squirrels/_credentials_manager.py` & `squirrels-0.1.1.post1/squirrels/_credentials_manager.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,87 +1,87 @@
-from typing import Dict
-from dataclasses import dataclass
-from configparser import ConfigParser
-import os, json
-
-from squirrels._utils import ConfigurationError
-from squirrels import _constants as c, _utils
-
-_SQUIRRELS_CFG_PATH = _utils.join_paths(os.path.expanduser('~'), '.squirrelscfg')
-
-
-@dataclass
-class Credential:
-    username: str
-    password: str
-    
-    def __str__(self) -> str:
-        redacted_pass = '*'*len(self.password)
-        return f'username={self.username}, password={redacted_pass}'
-
-
-class SquirrelsConfigParser(ConfigParser):
-    def _get_creds_section(self):
-        section_name: str = c.CREDENTIALS_KEY
-        if not self.has_section(section_name):
-            self.add_section(section_name)
-        return self[section_name]
-    
-    def _json_str_to_credential(self, json_str: str) -> Credential:
-        cred_dict = json.loads(json_str)
-        return Credential(cred_dict[c.USERNAME_KEY], cred_dict[c.PASSWORD_KEY])
-    
-    def get_credential(self, key: str) -> Credential:
-        section = self._get_creds_section()
-        try:
-            value = section[key]
-        except KeyError as e:
-            raise ConfigurationError(f'Credential key "{key}" has not been set. To set it, use $ squirrels set-credential {key}')
-        return self._json_str_to_credential(value)
-
-    def get_all_credentials(self) -> Dict[str, Credential]:
-        section = self._get_creds_section()
-        result = {}
-        for key, value in section.items():
-            result[key] = self._json_str_to_credential(value)
-        return result
-
-    def set_credential(self, key: str, credential: Credential) -> ConfigParser:
-        section = self._get_creds_section()
-        section[key] = json.dumps(credential.__dict__)
-        return self
-    
-    def delete_credential(self, key: str) -> ConfigParser:
-        section = self._get_creds_section()
-        section.pop(key)
-        return self
-
-
-class SquirrelsConfigIOWrapper:
-    def __init__(self) -> None:
-        self.config = SquirrelsConfigParser()
-        self.config.read(_SQUIRRELS_CFG_PATH)
-
-    def get_credential(self, key: str) -> Credential:
-        return self.config.get_credential(key)
-
-    def print_all_credentials(self) -> None:
-        credentials_dict = self.config.get_all_credentials()
-        for key, cred in credentials_dict.items():
-            print(f'{key}:', cred)
-
-    def _write_config(self) -> None:
-        with open(_SQUIRRELS_CFG_PATH, 'w') as f:
-            self.config.write(f)
-
-    def set_credential(self, key: str, user: str, pw: str) -> None:
-        credential = Credential(user, pw)
-        self.config.set_credential(key, credential)
-        print(f'Credential key "{key}" set to: {credential}')
-        self._write_config()
-
-    def delete_credential(self, key: str) -> None:
-        self.config.delete_credential(key)
-        print(f'Credential key "{key}" has been deleted')
-        self._write_config()
-
-squirrels_config_io = SquirrelsConfigIOWrapper()
+from typing import Dict
+from dataclasses import dataclass
+from configparser import ConfigParser
+import os, json
+
+from squirrels._utils import ConfigurationError
+from squirrels import _constants as c, _utils
+
+_SQUIRRELS_CFG_PATH = _utils.join_paths(os.path.expanduser('~'), '.squirrelscfg')
+
+
+@dataclass
+class Credential:
+    username: str
+    password: str
+    
+    def __str__(self) -> str:
+        redacted_pass = '*'*len(self.password)
+        return f'username={self.username}, password={redacted_pass}'
+
+
+class SquirrelsConfigParser(ConfigParser):
+    def _get_creds_section(self):
+        section_name: str = c.CREDENTIALS_KEY
+        if not self.has_section(section_name):
+            self.add_section(section_name)
+        return self[section_name]
+    
+    def _json_str_to_credential(self, json_str: str) -> Credential:
+        cred_dict = json.loads(json_str)
+        return Credential(cred_dict[c.USERNAME_KEY], cred_dict[c.PASSWORD_KEY])
+    
+    def get_credential(self, key: str) -> Credential:
+        section = self._get_creds_section()
+        try:
+            value = section[key]
+        except KeyError as e:
+            raise ConfigurationError(f'Credential key "{key}" has not been set. To set it, use $ squirrels set-credential {key}')
+        return self._json_str_to_credential(value)
+
+    def get_all_credentials(self) -> Dict[str, Credential]:
+        section = self._get_creds_section()
+        result = {}
+        for key, value in section.items():
+            result[key] = self._json_str_to_credential(value)
+        return result
+
+    def set_credential(self, key: str, credential: Credential) -> ConfigParser:
+        section = self._get_creds_section()
+        section[key] = json.dumps(credential.__dict__)
+        return self
+    
+    def delete_credential(self, key: str) -> ConfigParser:
+        section = self._get_creds_section()
+        section.pop(key)
+        return self
+
+
+class SquirrelsConfigIOWrapper:
+    def __init__(self) -> None:
+        self.config = SquirrelsConfigParser()
+        self.config.read(_SQUIRRELS_CFG_PATH)
+
+    def get_credential(self, key: str) -> Credential:
+        return self.config.get_credential(key)
+
+    def print_all_credentials(self) -> None:
+        credentials_dict = self.config.get_all_credentials()
+        for key, cred in credentials_dict.items():
+            print(f'{key}:', cred)
+
+    def _write_config(self) -> None:
+        with open(_SQUIRRELS_CFG_PATH, 'w') as f:
+            self.config.write(f)
+
+    def set_credential(self, key: str, user: str, pw: str) -> None:
+        credential = Credential(user, pw)
+        self.config.set_credential(key, credential)
+        print(f'Credential key "{key}" set to: {credential}')
+        self._write_config()
+
+    def delete_credential(self, key: str) -> None:
+        self.config.delete_credential(key)
+        print(f'Credential key "{key}" has been deleted')
+        self._write_config()
+
+squirrels_config_io = SquirrelsConfigIOWrapper()
```

### Comparing `squirrels-0.1.0/squirrels/_initializer.py` & `squirrels-0.1.1.post1/squirrels/_initializer.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,110 +1,110 @@
-import inquirer, os, shutil
-
-from squirrels import _constants as c, _utils
-from squirrels._version import major_version
-
-base_proj_dir = _utils.join_paths(os.path.dirname(__file__), 'package_data', 'base_project')
-dataset_dir = _utils.join_paths('datasets', 'sample_dataset')
-
-
-class Initializer:
-    def __init__(self, overwrite: bool):
-        self.overwrite = overwrite
-
-    def _path_exists(self, filepath: str) -> bool:
-        if not self.overwrite and os.path.exists(filepath):
-            print(f'File "{filepath}" already exists. Creation skipped.')
-            return True
-        return False
-    
-    def _copy_file(self, filepath: str):
-        if not self._path_exists(filepath):
-            dest_dir = os.path.dirname(filepath)
-            if dest_dir != '':
-                os.makedirs(dest_dir, exist_ok=True)
-            src_path = _utils.join_paths(base_proj_dir, filepath)
-            shutil.copy(src_path, filepath)
-
-    def _copy_dataset_file(self, filepath: str):
-        self._copy_file(_utils.join_paths(dataset_dir, filepath))
-
-    def _copy_database_file(self, filepath: str):
-        self._copy_file(_utils.join_paths('database', filepath))
-
-    def _create_requirements_txt(self):
-        filename = 'requirements.txt'
-        if not self._path_exists(filename):
-            next_major_version = int(major_version) + 1
-            content = f'squirrels<{next_major_version}'
-            with open(filename, 'w') as f:
-                f.write(content)
-
-    def init_project(self, args):
-        options = ['core', 'db_view', 'connections', 'context', 'selections_cfg', 'final_view', 'sample_db']
-        answers = { x: getattr(args, x) for x in options }
-        if not any(answers.values()):
-            core_questions = [
-                inquirer.Confirm('core', 
-                                message="Include all core project files?",
-                                default=True)
-            ]
-            answers = inquirer.prompt(core_questions)
-            
-            if answers.get('core', False):
-                conditional_questions = [
-                    inquirer.List('db_view', 
-                                  message="What's the file format for the database view?",
-                                  choices=c.FILE_TYPE_CHOICES),
-                ]
-                answers.update(inquirer.prompt(conditional_questions))
-
-            remaining_questions = [
-                inquirer.Confirm('connections',
-                                message=f"Do you want to add a '{c.CONNECTIONS_FILE}' file?" ,
-                                default=False),
-                inquirer.Confirm('context',
-                                message=f"Do you want to add a '{c.CONTEXT_FILE}' file?" ,
-                                default=False),
-                inquirer.Confirm('selections_cfg',
-                                message=f"Do you want to add a '{c.SELECTIONS_CFG_FILE}' file?" ,
-                                default=False),
-                inquirer.List('final_view', 
-                            message="What's the file format for the final view (if any)?",
-                            choices=['none'] + c.FILE_TYPE_CHOICES),
-                inquirer.List('sample_db', 
-                            message="What sample sqlite database do you wish to use (if any)?",
-                            choices=['none'] + c.DATABASE_CHOICES)
-            ]
-            answers.update(inquirer.prompt(remaining_questions))
-
-        if answers.get('core', False):
-            self._copy_file('.gitignore')
-            self._copy_file(c.MANIFEST_FILE)
-            self._create_requirements_txt()
-            self._copy_dataset_file(c.PARAMETERS_FILE)
-            if answers.get('db_view') == 'py':
-                self._copy_dataset_file(c.DATABASE_VIEW_PY_FILE)
-            else:
-                self._copy_dataset_file(c.DATABASE_VIEW_SQL_FILE)
-        
-        if answers.get('connections', False):
-            self._copy_file(c.CONNECTIONS_FILE)
-        
-        if answers.get('context', False):
-            self._copy_dataset_file(c.CONTEXT_FILE)
-        
-        if answers.get('selections_cfg', False):
-            self._copy_dataset_file(c.SELECTIONS_CFG_FILE)
-        
-        final_view_format = answers.get('final_view')
-        if final_view_format == 'py':
-            self._copy_dataset_file(c.FINAL_VIEW_PY_NAME)
-        elif final_view_format == 'sql':
-            self._copy_dataset_file(c.FINAL_VIEW_SQL_NAME)
-
-        sample_db = answers.get('sample_db')
-        if sample_db == 'sample_database':
-            self._copy_database_file('sample_database.db')
-        elif sample_db == 'seattle_weather':
-            self._copy_database_file('seattle_weather.db')
+import inquirer, os, shutil
+
+from squirrels import _constants as c, _utils
+from squirrels._version import major_version
+
+base_proj_dir = _utils.join_paths(os.path.dirname(__file__), 'package_data', 'base_project')
+dataset_dir = _utils.join_paths('datasets', 'sample_dataset')
+
+
+class Initializer:
+    def __init__(self, overwrite: bool):
+        self.overwrite = overwrite
+
+    def _path_exists(self, filepath: str) -> bool:
+        if not self.overwrite and os.path.exists(filepath):
+            print(f'File "{filepath}" already exists. Creation skipped.')
+            return True
+        return False
+    
+    def _copy_file(self, filepath: str):
+        if not self._path_exists(filepath):
+            dest_dir = os.path.dirname(filepath)
+            if dest_dir != '':
+                os.makedirs(dest_dir, exist_ok=True)
+            src_path = _utils.join_paths(base_proj_dir, filepath)
+            shutil.copy(src_path, filepath)
+
+    def _copy_dataset_file(self, filepath: str):
+        self._copy_file(_utils.join_paths(dataset_dir, filepath))
+
+    def _copy_database_file(self, filepath: str):
+        self._copy_file(_utils.join_paths('database', filepath))
+
+    def _create_requirements_txt(self):
+        filename = 'requirements.txt'
+        if not self._path_exists(filename):
+            next_major_version = int(major_version) + 1
+            content = f'squirrels<{next_major_version}'
+            with open(filename, 'w') as f:
+                f.write(content)
+
+    def init_project(self, args):
+        options = ['core', 'db_view', 'connections', 'context', 'selections_cfg', 'final_view', 'sample_db']
+        answers = { x: getattr(args, x) for x in options }
+        if not any(answers.values()):
+            core_questions = [
+                inquirer.Confirm('core', 
+                                message="Include all core project files?",
+                                default=True)
+            ]
+            answers = inquirer.prompt(core_questions)
+            
+            if answers.get('core', False):
+                conditional_questions = [
+                    inquirer.List('db_view', 
+                                  message="What's the file format for the database view?",
+                                  choices=c.FILE_TYPE_CHOICES),
+                ]
+                answers.update(inquirer.prompt(conditional_questions))
+
+            remaining_questions = [
+                inquirer.Confirm('connections',
+                                message=f"Do you want to add a '{c.CONNECTIONS_FILE}' file?" ,
+                                default=False),
+                inquirer.Confirm('context',
+                                message=f"Do you want to add a '{c.CONTEXT_FILE}' file?" ,
+                                default=False),
+                inquirer.Confirm('selections_cfg',
+                                message=f"Do you want to add a '{c.SELECTIONS_CFG_FILE}' file?" ,
+                                default=False),
+                inquirer.List('final_view', 
+                            message="What's the file format for the final view (if any)?",
+                            choices=['none'] + c.FILE_TYPE_CHOICES),
+                inquirer.List('sample_db', 
+                            message="What sample sqlite database do you wish to use (if any)?",
+                            choices=['none'] + c.DATABASE_CHOICES)
+            ]
+            answers.update(inquirer.prompt(remaining_questions))
+
+        if answers.get('core', False):
+            self._copy_file('.gitignore')
+            self._copy_file(c.MANIFEST_FILE)
+            self._create_requirements_txt()
+            self._copy_dataset_file(c.PARAMETERS_FILE)
+            if answers.get('db_view') == 'py':
+                self._copy_dataset_file(c.DATABASE_VIEW_PY_FILE)
+            else:
+                self._copy_dataset_file(c.DATABASE_VIEW_SQL_FILE)
+        
+        if answers.get('connections', False):
+            self._copy_file(c.CONNECTIONS_FILE)
+        
+        if answers.get('context', False):
+            self._copy_dataset_file(c.CONTEXT_FILE)
+        
+        if answers.get('selections_cfg', False):
+            self._copy_dataset_file(c.SELECTIONS_CFG_FILE)
+        
+        final_view_format = answers.get('final_view')
+        if final_view_format == 'py':
+            self._copy_dataset_file(c.FINAL_VIEW_PY_NAME)
+        elif final_view_format == 'sql':
+            self._copy_dataset_file(c.FINAL_VIEW_SQL_NAME)
+
+        sample_db = answers.get('sample_db')
+        if sample_db == 'sample_database':
+            self._copy_database_file('sample_database.db')
+        elif sample_db == 'seattle_weather':
+            self._copy_database_file('seattle_weather.db')
```

### Comparing `squirrels-0.1.0/squirrels/_manifest.py` & `squirrels-0.1.1.post1/squirrels/_manifest.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,187 +1,187 @@
-from typing import List, Dict, Any, Optional, Union
-from pathlib import Path
-from sqlalchemy import Engine, create_engine
-import yaml
-
-from squirrels import _constants as c, _utils
-from squirrels._credentials_manager import Credential, squirrels_config_io
-from squirrels._utils import ConfigurationError, InvalidInputError
-
-
-class Manifest:
-    def __init__(self, parms: Dict) -> None:
-        self._parms = parms
-    
-    @classmethod
-    def from_yaml_str(cls, parms_str: str):
-        parms = yaml.safe_load(parms_str)
-        return cls(parms)
-
-    @classmethod
-    def from_file(cls, manifest_path: str):
-        with open(manifest_path, 'r') as f:
-            parms_str = f.read()
-        
-        return Manifest.from_yaml_str(parms_str)
-    
-    def get_proj_vars(self) -> Dict[str, Any]:
-        return self._parms.get(c.PROJ_VARS_KEY, dict())
-    
-    def get_modules(self) -> List[str]:
-        return self._parms.get(c.MODULES_KEY, list())
-    
-    def _get_required_field(self, key: str) -> Any:
-        try:
-            return self._parms[key]
-        except KeyError as e:
-            raise ConfigurationError(f'Field "{key}" not found in squirrels.yaml') from e
-    
-    def get_base_path(self) -> str:
-        project_vars = self.get_proj_vars()
-        try:
-            product = project_vars[c.PRODUCT_KEY]
-            major_version = project_vars[c.MAJOR_VERSION_KEY]
-        except KeyError as e:
-            raise ConfigurationError("Could not construct API endpoint as 'product' and 'major_version'" + 
-                "were not specified in project variables") from e
-        base_path = f"/{product}/v{major_version}"
-        return base_path
-    
-    def get_db_connections(self, test_creds: Dict[str, Credential] = None) -> Dict[str, Engine]:
-        configs: Dict[str, Dict[str, str]] = self._parms.get(c.DB_CONNECTIONS_KEY, {})
-        output = {}
-        for key, config in configs.items():
-            cred_key = config.get(c.DB_CREDENTIALS_KEY)
-            if cred_key is None:
-                cred = Credential("", "")
-            elif test_creds is not None:
-                cred = test_creds[cred_key]
-            else:
-                cred = squirrels_config_io.get_credential(cred_key)
-            url = config[c.URL_KEY].replace("${username}", cred.username).replace("${password}", cred.password)
-            output[key] = create_engine(url)
-        return output
-
-    def _get_dataset_parms(self, dataset: str) -> Dict[str, Any]:
-        try:
-            return self._get_required_field(c.DATASETS_KEY)[dataset]
-        except KeyError as e:
-            raise InvalidInputError(f'No such dataset named "{dataset}" exists') from e
-        
-    def _get_required_field_from_dataset_parms(self, dataset: str, key: str):
-        try:
-            return self._get_dataset_parms(dataset)[key]
-        except KeyError as e:
-            raise ConfigurationError(f'The "{key}" field is not defined for dataset "{dataset}"') from e
-    
-    def _get_all_database_view_parms(self, dataset: str) -> Dict[str, Dict[str, str]]:
-        return self._get_required_field_from_dataset_parms(dataset, c.DATABASE_VIEWS_KEY)
-    
-    def get_all_dataset_names(self) -> str:
-        datasets: Dict[str, Any] = self._get_required_field(c.DATASETS_KEY)
-        return list(datasets.keys())
-    
-    def get_dataset_folder(self, dataset: str) -> Path:
-        return _utils.join_paths(c.DATASETS_FOLDER, dataset)
-        
-    def get_dataset_args(self, dataset: str) -> Dict[str, Any]:
-        dataset_args = self._get_dataset_parms(dataset).get("args", {})
-        full_args = {**self.get_proj_vars(), **dataset_args}
-        return full_args
-    
-    def get_all_database_view_names(self, dataset: str) -> List[str]:
-        all_database_views = self._get_all_database_view_parms(dataset)
-        return list(all_database_views.keys())
-    
-    def get_database_view_file(self, dataset: str, database_view: str) -> Path:
-        database_view_parms = self._get_all_database_view_parms(dataset)[database_view]
-        if isinstance(database_view_parms, str):
-            db_view_file = database_view_parms
-        else:
-            try:
-                db_view_file = database_view_parms[c.FILE_KEY]
-            except KeyError as e:
-                raise ConfigurationError(f'The "{c.FILE_KEY}" field is not defined for "{database_view}" in dataset "{dataset}"') from e
-        dataset_folder = self.get_dataset_folder(dataset)
-        return _utils.join_paths(dataset_folder, db_view_file)
-    
-    def get_view_args(self, dataset: str, database_view: str = None) -> Dict[str, Any]:
-        dataset_args = self.get_dataset_args(dataset)
-        if database_view is None:
-            view_parms: Dict[str, Any] = self._get_required_field_from_dataset_parms(dataset, c.FINAL_VIEW_KEY)
-        else:
-            view_parms: Dict[str, Any] = self._get_all_database_view_parms(dataset)[database_view]
-        view_args: Dict[str, Any] = {} if isinstance(view_parms, str) else view_parms.get("args", {})
-        full_args = {**dataset_args, **view_args}
-        return full_args
-
-    def get_database_view_db_connection(self, dataset: str, database_view: str) -> Optional[str]:
-        database_view_parms = self._get_all_database_view_parms(dataset)[database_view]
-        if isinstance(database_view_parms, str):
-            db_connection = c.DEFAULT_DB_CONN 
-        else: 
-            db_connection = database_view_parms.get(c.DB_CONNECTION_KEY, c.DEFAULT_DB_CONN)
-        return db_connection
-    
-    def get_dataset_label(self, dataset: str) -> str:
-        return self._get_required_field_from_dataset_parms(dataset, c.DATASET_LABEL_KEY)
-    
-    def get_dataset_final_view_file(self, dataset: str) -> Union[str, Path]:
-        final_view_parms: Dict[str, Any] = self._get_required_field_from_dataset_parms(dataset, c.FINAL_VIEW_KEY)
-        if isinstance(final_view_parms, str):
-            final_view_file = final_view_parms
-        else:
-            try:
-                final_view_file = final_view_parms[c.FILE_KEY]
-            except KeyError as e:
-                raise ConfigurationError(f'The "{c.FILE_KEY}" field is not defined for the final view') from e
-        
-        database_views = self.get_all_database_view_names(dataset)
-        if final_view_file in database_views:
-            return final_view_file
-        else:
-            dataset_path = self.get_dataset_folder(dataset)
-            return _utils.join_paths(dataset_path, final_view_file)
-
-    def get_setting(self, key: str, default: Any) -> Any:
-        settings: Dict[str, Any] = self._parms.get(c.SETTINGS_KEY, dict())
-        return settings.get(key, default)
-    
-    def get_catalog(self, parameters_path: str, results_path: str) -> Any:
-        """
-        Gets the component of the catalog API response that's generated by this manifest
-
-        Parameters:
-            parameters_path: The path to the parameters API endpoint
-            results_path: The path to the results API endpoint
-        
-        Returns:
-            A JSON response for the catalog API
-        """
-        datasets_info = []
-        for dataset in self.get_all_dataset_names():
-            dataset_normalized = _utils.normalize_name_for_api(dataset)
-            datasets_info.append({
-                'name': dataset,
-                'label': self.get_dataset_label(dataset),
-                'parameters_path': parameters_path.format(dataset=dataset_normalized),
-                'result_path': results_path.format(dataset=dataset_normalized),
-                'first_minor_version': 0
-            })
-        
-        project_vars = self.get_proj_vars()
-        return {
-            'response_version': 0,
-            'products': [{
-                'name': project_vars[c.PRODUCT_KEY],
-                'versions': [{
-                    'major_version': project_vars[c.MAJOR_VERSION_KEY],
-                    'latest_minor_version': project_vars[c.MINOR_VERSION_KEY],
-                    'datasets': datasets_info
-                }]
-            }]
-        }
-
-
-def _from_file():
-    return Manifest.from_file(c.MANIFEST_FILE)
+from typing import List, Dict, Any, Optional, Union
+from pathlib import Path
+from sqlalchemy import Engine, create_engine
+import yaml
+
+from squirrels import _constants as c, _utils
+from squirrels._credentials_manager import Credential, squirrels_config_io
+from squirrels._utils import ConfigurationError, InvalidInputError
+
+
+class Manifest:
+    def __init__(self, parms: Dict) -> None:
+        self._parms = parms
+    
+    @classmethod
+    def from_yaml_str(cls, parms_str: str):
+        parms = yaml.safe_load(parms_str)
+        return cls(parms)
+
+    @classmethod
+    def from_file(cls, manifest_path: str):
+        with open(manifest_path, 'r') as f:
+            parms_str = f.read()
+        
+        return Manifest.from_yaml_str(parms_str)
+    
+    def get_proj_vars(self) -> Dict[str, Any]:
+        return self._parms.get(c.PROJ_VARS_KEY, dict())
+    
+    def get_modules(self) -> List[str]:
+        return self._parms.get(c.MODULES_KEY, list())
+    
+    def _get_required_field(self, key: str) -> Any:
+        try:
+            return self._parms[key]
+        except KeyError as e:
+            raise ConfigurationError(f'Field "{key}" not found in squirrels.yaml') from e
+    
+    def get_base_path(self) -> str:
+        project_vars = self.get_proj_vars()
+        try:
+            product = project_vars[c.PRODUCT_KEY]
+            major_version = project_vars[c.MAJOR_VERSION_KEY]
+        except KeyError as e:
+            raise ConfigurationError("Could not construct API endpoint as 'product' and 'major_version'" + 
+                "were not specified in project variables") from e
+        base_path = f"/{product}/v{major_version}"
+        return base_path
+    
+    def get_db_connections(self, test_creds: Dict[str, Credential] = None) -> Dict[str, Engine]:
+        configs: Dict[str, Dict[str, str]] = self._parms.get(c.DB_CONNECTIONS_KEY, {})
+        output = {}
+        for key, config in configs.items():
+            cred_key = config.get(c.DB_CREDENTIALS_KEY)
+            if cred_key is None:
+                cred = Credential("", "")
+            elif test_creds is not None:
+                cred = test_creds[cred_key]
+            else:
+                cred = squirrels_config_io.get_credential(cred_key)
+            url = config[c.URL_KEY].replace("${username}", cred.username).replace("${password}", cred.password)
+            output[key] = create_engine(url)
+        return output
+
+    def _get_dataset_parms(self, dataset: str) -> Dict[str, Any]:
+        try:
+            return self._get_required_field(c.DATASETS_KEY)[dataset]
+        except KeyError as e:
+            raise InvalidInputError(f'No such dataset named "{dataset}" exists') from e
+        
+    def _get_required_field_from_dataset_parms(self, dataset: str, key: str):
+        try:
+            return self._get_dataset_parms(dataset)[key]
+        except KeyError as e:
+            raise ConfigurationError(f'The "{key}" field is not defined for dataset "{dataset}"') from e
+    
+    def _get_all_database_view_parms(self, dataset: str) -> Dict[str, Dict[str, str]]:
+        return self._get_required_field_from_dataset_parms(dataset, c.DATABASE_VIEWS_KEY)
+    
+    def get_all_dataset_names(self) -> str:
+        datasets: Dict[str, Any] = self._get_required_field(c.DATASETS_KEY)
+        return list(datasets.keys())
+    
+    def get_dataset_folder(self, dataset: str) -> Path:
+        return _utils.join_paths(c.DATASETS_FOLDER, dataset)
+        
+    def get_dataset_args(self, dataset: str) -> Dict[str, Any]:
+        dataset_args = self._get_dataset_parms(dataset).get("args", {})
+        full_args = {**self.get_proj_vars(), **dataset_args}
+        return full_args
+    
+    def get_all_database_view_names(self, dataset: str) -> List[str]:
+        all_database_views = self._get_all_database_view_parms(dataset)
+        return list(all_database_views.keys())
+    
+    def get_database_view_file(self, dataset: str, database_view: str) -> Path:
+        database_view_parms = self._get_all_database_view_parms(dataset)[database_view]
+        if isinstance(database_view_parms, str):
+            db_view_file = database_view_parms
+        else:
+            try:
+                db_view_file = database_view_parms[c.FILE_KEY]
+            except KeyError as e:
+                raise ConfigurationError(f'The "{c.FILE_KEY}" field is not defined for "{database_view}" in dataset "{dataset}"') from e
+        dataset_folder = self.get_dataset_folder(dataset)
+        return _utils.join_paths(dataset_folder, db_view_file)
+    
+    def get_view_args(self, dataset: str, database_view: str = None) -> Dict[str, Any]:
+        dataset_args = self.get_dataset_args(dataset)
+        if database_view is None:
+            view_parms: Dict[str, Any] = self._get_required_field_from_dataset_parms(dataset, c.FINAL_VIEW_KEY)
+        else:
+            view_parms: Dict[str, Any] = self._get_all_database_view_parms(dataset)[database_view]
+        view_args: Dict[str, Any] = {} if isinstance(view_parms, str) else view_parms.get("args", {})
+        full_args = {**dataset_args, **view_args}
+        return full_args
+
+    def get_database_view_db_connection(self, dataset: str, database_view: str) -> Optional[str]:
+        database_view_parms = self._get_all_database_view_parms(dataset)[database_view]
+        if isinstance(database_view_parms, str):
+            db_connection = c.DEFAULT_DB_CONN 
+        else: 
+            db_connection = database_view_parms.get(c.DB_CONNECTION_KEY, c.DEFAULT_DB_CONN)
+        return db_connection
+    
+    def get_dataset_label(self, dataset: str) -> str:
+        return self._get_required_field_from_dataset_parms(dataset, c.DATASET_LABEL_KEY)
+    
+    def get_dataset_final_view_file(self, dataset: str) -> Union[str, Path]:
+        final_view_parms: Dict[str, Any] = self._get_required_field_from_dataset_parms(dataset, c.FINAL_VIEW_KEY)
+        if isinstance(final_view_parms, str):
+            final_view_file = final_view_parms
+        else:
+            try:
+                final_view_file = final_view_parms[c.FILE_KEY]
+            except KeyError as e:
+                raise ConfigurationError(f'The "{c.FILE_KEY}" field is not defined for the final view') from e
+        
+        database_views = self.get_all_database_view_names(dataset)
+        if final_view_file in database_views:
+            return final_view_file
+        else:
+            dataset_path = self.get_dataset_folder(dataset)
+            return _utils.join_paths(dataset_path, final_view_file)
+
+    def get_setting(self, key: str, default: Any) -> Any:
+        settings: Dict[str, Any] = self._parms.get(c.SETTINGS_KEY, dict())
+        return settings.get(key, default)
+    
+    def get_catalog(self, parameters_path: str, results_path: str) -> Any:
+        """
+        Gets the component of the catalog API response that's generated by this manifest
+
+        Parameters:
+            parameters_path: The path to the parameters API endpoint
+            results_path: The path to the results API endpoint
+        
+        Returns:
+            A JSON response for the catalog API
+        """
+        datasets_info = []
+        for dataset in self.get_all_dataset_names():
+            dataset_normalized = _utils.normalize_name_for_api(dataset)
+            datasets_info.append({
+                'name': dataset,
+                'label': self.get_dataset_label(dataset),
+                'parameters_path': parameters_path.format(dataset=dataset_normalized),
+                'result_path': results_path.format(dataset=dataset_normalized),
+                'first_minor_version': 0
+            })
+        
+        project_vars = self.get_proj_vars()
+        return {
+            'response_version': 0,
+            'products': [{
+                'name': project_vars[c.PRODUCT_KEY],
+                'versions': [{
+                    'major_version': project_vars[c.MAJOR_VERSION_KEY],
+                    'latest_minor_version': project_vars[c.MINOR_VERSION_KEY],
+                    'datasets': datasets_info
+                }]
+            }]
+        }
+
+
+def _from_file():
+    return Manifest.from_file(c.MANIFEST_FILE)
```

### Comparing `squirrels-0.1.0/squirrels/_parameter_set.py` & `squirrels-0.1.1.post1/squirrels/_parameter_set.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,151 +1,151 @@
-from __future__ import annotations
-from typing import Sequence, Dict, Any
-from collections import OrderedDict
-
-from squirrels import data_sources as d, parameters as p
-from squirrels._timed_imports import pandas as pd
-
-
-class ParameterSetBase:
-    def __init__(self) -> None:
-        """
-        Constructor for ParameterSetBase, the base class for ParameterSet. Similar to ParameterSet but without 
-        a separate collection for DataSourceParameter's, and does not pre-set the parameters in constructor.
-        """
-        self._parameters_dict: OrderedDict[str, p.Parameter] = OrderedDict()
-    
-    def add_parameter(self, parameter: p.Parameter) -> None:
-        """
-        Adds a parameter to the "parameter collection"
-
-        Parameters:
-            parameter: The parameter to add
-        """
-        self._parameters_dict[parameter.name] = parameter
-
-    def get_parameter(self, param_name: str) -> p.Parameter:
-        """
-        Gets the Parameter object given the parameter name
-
-        Parameters:
-            param_name: The parameter name
-        
-        Returns:
-            The Parameter object corresponding to the parameter name
-        """
-        if param_name in self._parameters_dict:
-            return self._parameters_dict[param_name]
-        else:
-            raise KeyError(f'No such parameter exists called "{param_name}"')
-    
-    def __getitem__(self, param_name: str) -> p.Parameter:
-        return self.get_parameter(param_name)
-    
-    def get_parameters_as_ordered_dict(self) -> OrderedDict[str, p.Parameter]:
-        """
-        Returns the inner dictionary of the "parameter collection"
-
-        Returns:
-            A dictionary where key are the assigned names and values are the Parameter objects
-        """
-        return OrderedDict(self._parameters_dict)
-    
-    def merge(self, other: ParameterSetBase) -> ParameterSetBase:
-        """
-        Merges the "parameter collection" of this and another ParameterSetBase
-
-        Parameters:
-            other: The other ParameterSetBase
-        
-        Returns:
-            A new copy of the ParameterSetBase as a result of the merge
-        """
-        new_param_set = ParameterSetBase()
-        new_param_set._parameters_dict = OrderedDict(self._parameters_dict)
-        new_param_set._parameters_dict.update(other._parameters_dict)
-        return new_param_set
-
-    def to_json_dict(self, debug: bool = False) -> Dict[str, Any]:
-        """
-        Converts this object, and all parameters contained, into a JSON dictionary
-
-        Parameters:
-            debug: Set to True to make the "hidden" parameters show as part of the result
-
-        Returns:
-            A collection of parameters as a JSON dictionary used for the "parameters" endpoint
-        """
-        parameters = []
-        for x in self._parameters_dict.values():
-            if not x.is_hidden or debug:
-                parameters.append(x.to_json_dict())
-        
-        output = {
-            "response_version": 0, 
-            "parameters": parameters
-        }
-        return output
-
-
-class ParameterSet(ParameterSetBase):
-    def __init__(self, parameters: Sequence[p.Parameter]):
-        """
-        Constructor for ParameterSet, a wrapper class for a sequence of parameters, 
-        and stores the DataSourceParameters as a separate field as well
-
-        Parameters:
-            parameters: A sequence of parameters
-        """
-        super().__init__()
-        self._data_source_params: OrderedDict[str, p.DataSourceParameter] = OrderedDict()
-        for param in parameters:
-            self._parameters_dict[param.name] = param
-            if isinstance(param, p.DataSourceParameter):
-                self._data_source_params[param.name] = param
-    
-    def merge(self, other: ParameterSetBase) -> ParameterSet:
-        """
-        Merges this object with another ParameterSet (by combining the parameters) to create a new ParameterSet.
-
-        The _parameters_dict are merged (with the other ParameterSet taking precedence when a name exist in both dict),
-        while the _data_source_params are only taken from this object. This object and the other ParameterSet remain
-        unchanged.
-
-        Parameters:
-            other: The other parameter set
-        
-        Returns:
-            A new ParameterSet that contains all the parameters from this and the other parameter set.
-        """
-        new_param_set_base = super().merge(other)
-        new_param_set = ParameterSet(())
-        new_param_set._parameters_dict = new_param_set_base._parameters_dict
-        new_param_set._data_source_params = self._data_source_params
-        return new_param_set
-
-    def get_datasources(self) -> Dict[str, d.DataSource]:
-        """
-        Gets all the DataSource objects as values to a dictionary where keys are the DataSource parameter names.
-
-        Each DataSource object represents a lookup table with table name, connection name, corresponding columns to ID, label, etc.
-
-        Returns:
-            A dictionary where keys are the names of DataSourceParameter's and values are the corresponding DataSource.
-        """
-        new_dict = {}
-        for param_name, ds_param in self._data_source_params.items():
-            new_dict[param_name] = ds_param.data_source
-        return new_dict
-
-    def convert_datasource_params(self, df_dict: Dict[str, pd.DataFrame]) -> None:
-        """
-        Changes all the DataSourceParameters into other Parameter types. The _data_source_params field gets cleared.
-
-        Parameters:
-            df_dict: A dictionary of DataSourceParameter name to the pandas DataFrame of the lookup table data.
-        """
-        # Done sequentially since parents must be converted first before children
-        for key, ds_param in self._data_source_params.items():
-            ds_param.parent = self.get_parameter(ds_param.parent.name) if ds_param.parent is not None else None
-            self._parameters_dict[key] = ds_param.convert(df_dict[key])
-        self._data_source_params.clear()
+from __future__ import annotations
+from typing import Sequence, Dict, Any
+from collections import OrderedDict
+
+from squirrels import data_sources as d, parameters as p
+from squirrels._timed_imports import pandas as pd
+
+
+class ParameterSetBase:
+    def __init__(self) -> None:
+        """
+        Constructor for ParameterSetBase, the base class for ParameterSet. Similar to ParameterSet but without 
+        a separate collection for DataSourceParameter's, and does not pre-set the parameters in constructor.
+        """
+        self._parameters_dict: OrderedDict[str, p.Parameter] = OrderedDict()
+    
+    def add_parameter(self, parameter: p.Parameter) -> None:
+        """
+        Adds a parameter to the "parameter collection"
+
+        Parameters:
+            parameter: The parameter to add
+        """
+        self._parameters_dict[parameter.name] = parameter
+
+    def get_parameter(self, param_name: str) -> p.Parameter:
+        """
+        Gets the Parameter object given the parameter name
+
+        Parameters:
+            param_name: The parameter name
+        
+        Returns:
+            The Parameter object corresponding to the parameter name
+        """
+        if param_name in self._parameters_dict:
+            return self._parameters_dict[param_name]
+        else:
+            raise KeyError(f'No such parameter exists called "{param_name}"')
+    
+    def __getitem__(self, param_name: str) -> p.Parameter:
+        return self.get_parameter(param_name)
+    
+    def get_parameters_as_ordered_dict(self) -> OrderedDict[str, p.Parameter]:
+        """
+        Returns the inner dictionary of the "parameter collection"
+
+        Returns:
+            A dictionary where key are the assigned names and values are the Parameter objects
+        """
+        return OrderedDict(self._parameters_dict)
+    
+    def merge(self, other: ParameterSetBase) -> ParameterSetBase:
+        """
+        Merges the "parameter collection" of this and another ParameterSetBase
+
+        Parameters:
+            other: The other ParameterSetBase
+        
+        Returns:
+            A new copy of the ParameterSetBase as a result of the merge
+        """
+        new_param_set = ParameterSetBase()
+        new_param_set._parameters_dict = OrderedDict(self._parameters_dict)
+        new_param_set._parameters_dict.update(other._parameters_dict)
+        return new_param_set
+
+    def to_json_dict(self, debug: bool = False) -> Dict[str, Any]:
+        """
+        Converts this object, and all parameters contained, into a JSON dictionary
+
+        Parameters:
+            debug: Set to True to make the "hidden" parameters show as part of the result
+
+        Returns:
+            A collection of parameters as a JSON dictionary used for the "parameters" endpoint
+        """
+        parameters = []
+        for x in self._parameters_dict.values():
+            if not x.is_hidden or debug:
+                parameters.append(x.to_json_dict())
+        
+        output = {
+            "response_version": 0, 
+            "parameters": parameters
+        }
+        return output
+
+
+class ParameterSet(ParameterSetBase):
+    def __init__(self, parameters: Sequence[p.Parameter]):
+        """
+        Constructor for ParameterSet, a wrapper class for a sequence of parameters, 
+        and stores the DataSourceParameters as a separate field as well
+
+        Parameters:
+            parameters: A sequence of parameters
+        """
+        super().__init__()
+        self._data_source_params: OrderedDict[str, p.DataSourceParameter] = OrderedDict()
+        for param in parameters:
+            self._parameters_dict[param.name] = param
+            if isinstance(param, p.DataSourceParameter):
+                self._data_source_params[param.name] = param
+    
+    def merge(self, other: ParameterSetBase) -> ParameterSet:
+        """
+        Merges this object with another ParameterSet (by combining the parameters) to create a new ParameterSet.
+
+        The _parameters_dict are merged (with the other ParameterSet taking precedence when a name exist in both dict),
+        while the _data_source_params are only taken from this object. This object and the other ParameterSet remain
+        unchanged.
+
+        Parameters:
+            other: The other parameter set
+        
+        Returns:
+            A new ParameterSet that contains all the parameters from this and the other parameter set.
+        """
+        new_param_set_base = super().merge(other)
+        new_param_set = ParameterSet(())
+        new_param_set._parameters_dict = new_param_set_base._parameters_dict
+        new_param_set._data_source_params = self._data_source_params
+        return new_param_set
+
+    def get_datasources(self) -> Dict[str, d.DataSource]:
+        """
+        Gets all the DataSource objects as values to a dictionary where keys are the DataSource parameter names.
+
+        Each DataSource object represents a lookup table with table name, connection name, corresponding columns to ID, label, etc.
+
+        Returns:
+            A dictionary where keys are the names of DataSourceParameter's and values are the corresponding DataSource.
+        """
+        new_dict = {}
+        for param_name, ds_param in self._data_source_params.items():
+            new_dict[param_name] = ds_param.data_source
+        return new_dict
+
+    def convert_datasource_params(self, df_dict: Dict[str, pd.DataFrame]) -> None:
+        """
+        Changes all the DataSourceParameters into other Parameter types. The _data_source_params field gets cleared.
+
+        Parameters:
+            df_dict: A dictionary of DataSourceParameter name to the pandas DataFrame of the lookup table data.
+        """
+        # Done sequentially since parents must be converted first before children
+        for key, ds_param in self._data_source_params.items():
+            ds_param.parent = self.get_parameter(ds_param.parent.name) if ds_param.parent is not None else None
+            self._parameters_dict[key] = ds_param.convert(df_dict[key])
+        self._data_source_params.clear()
```

### Comparing `squirrels-0.1.0/squirrels/_renderer.py` & `squirrels-0.1.1.post1/squirrels/_renderer.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,286 +1,286 @@
-from typing import Dict, Tuple, Optional, Union, Callable, Any
-from functools import partial
-from configparser import ConfigParser
-import concurrent.futures, os, json, time
-
-from squirrels import _constants as c, _manifest as mf, _utils
-from squirrels.connection_set import ConnectionSet, sqldf
-from squirrels.data_sources import DataSource
-from squirrels._parameter_set import ParameterSet
-from squirrels._utils import ConfigurationError
-from squirrels._timed_imports import pandas as pd, timer
-
-ContextFunc = Optional[Callable[..., Dict[str, Any]]]
-DatabaseViews = Optional[Dict[str, pd.DataFrame]]
-Query = Union[Callable[..., pd.DataFrame], str]
-
-
-class Renderer:
-    def __init__(self, dataset: str, manifest: mf.Manifest, conn_set: ConnectionSet, raw_param_set: ParameterSet, 
-                 context_func: Callable[..., Dict[str, Any]], raw_query_by_db_view: Dict[str, Query], 
-                 raw_final_view_query: Query, excel_file: Optional[pd.ExcelFile] = None):
-        self.dataset = dataset
-        self.manifest = manifest
-        self.conn_set = conn_set
-        self.context_func = context_func
-        self.raw_query_by_db_view = raw_query_by_db_view
-        self.raw_final_view_query = raw_final_view_query
-
-        start = time.time()
-        self.param_set: ParameterSet = self._convert_param_set_datasources(raw_param_set, excel_file)
-        timer.add_activity_time(f"convert datasources - dataset {dataset}", start)
-    
-    def _convert_param_set_datasources(self, param_set: ParameterSet, excel_file: Optional[pd.ExcelFile] = None) -> ParameterSet:
-        datasources = param_set.get_datasources()
-        if excel_file is not None:
-            df_dict = pd.read_excel(excel_file, None)
-            for key in datasources:
-                if key not in df_dict:
-                    raise ConfigurationError('No sheet found for parameter "{key}" in the Excel workbook')
-        else:
-            def get_dataframe_from_query(item: Tuple[str, DataSource]) -> pd.DataFrame:
-                key, datasource = item
-                df = self.conn_set.get_dataframe_from_query(datasource.connection_name, datasource.get_query())
-                return key, df
-            
-            with concurrent.futures.ThreadPoolExecutor() as executor:
-                df_dict = dict(executor.map(get_dataframe_from_query, datasources.items()))
-        
-        param_set.convert_datasource_params(df_dict)
-        return param_set
-    
-    def apply_selections(self, selections: Dict[str, str], updates_only: bool = False) -> ParameterSet:
-        start = time.time()
-        parameter_set = self.param_set
-        parameters_dict = parameter_set.get_parameters_as_ordered_dict()
-        
-        # iterating through parameters dict instead of query_params since order matters for cascading parameters
-        for param_name, parameter in parameters_dict.items():
-            if param_name in selections:
-                value = selections[param_name]
-                parameter = parameter_set.get_parameter(param_name).with_selection(value)
-                updates = parameter.get_all_dependent_params()
-                if updates_only:
-                    parameter_set = updates
-                    break
-                parameter_set = parameter_set.merge(updates)
-        timer.add_activity_time(f"apply selections - dataset {self.dataset}", start)
-        
-        return parameter_set
-
-    def _render_context(self, context_func: ContextFunc, param_set: ParameterSet) -> Dict[str, Any]:
-        try:
-            return context_func(prms=param_set.get_parameters_as_ordered_dict()) if context_func is not None else {}
-        except Exception as e:
-            raise ConfigurationError(f'Error in the {c.CONTEXT_FILE} function for dataset "{self.dataset}"') from e
-    
-    def _get_args(self, param_set: ParameterSet, context: Dict[str, Any], db_view: str = None) -> Dict:
-        if db_view is not None:
-            args = self.manifest.get_view_args(self.dataset, db_view)
-        else:
-            args = self.manifest.get_view_args(self.dataset)
-        return {
-            'prms': param_set.get_parameters_as_ordered_dict(),
-            'ctx':  context,
-            'args': args
-        }
-    
-    def _render_query_from_raw(self, raw_query: Query, args: Dict) -> Query:
-        if isinstance(raw_query, str):
-            template = _utils.j2_env.from_string(raw_query)
-            return template.render(args)
-        else:
-            return partial(raw_query, **args)
-    
-    def _render_dataframe_from_sql(self, db_view_name: str, sql_str: str, 
-                                   database_views: DatabaseViews = None) -> pd.DataFrame:
-        if database_views is not None:
-            return sqldf(sql_str, database_views)
-        else:
-            conn_name = self.manifest.get_database_view_db_connection(self.dataset, db_view_name)
-            return self.conn_set.get_dataframe_from_query(conn_name, sql_str)
-
-    def _render_dataframe_from_py_func(self, db_view_name: str, py_func: Callable[[Any], pd.DataFrame], 
-                                       database_views: DatabaseViews = None) -> pd.DataFrame:
-        if database_views is not None:
-            try:
-                return py_func(database_views=database_views)
-            except Exception as e:
-                raise ConfigurationError(f'Error in the final view python function for dataset "{self.dataset}"') from e
-        else:
-            conn_name = self.manifest.get_database_view_db_connection(self.dataset, db_view_name)
-            connection_pool = self.conn_set.get_connection_pool(conn_name)
-            try:
-                return py_func(connection_pool=connection_pool, connection_set=self.conn_set)
-            except Exception as e:
-                raise ConfigurationError(f'Error in the python function for database view "{db_view_name}" in dataset "{self.dataset}"') from e
-    
-    def _render_db_view_dataframes(self, query_by_db_view: Dict[str, Query]) -> Dict[str, pd.DataFrame]:
-        def run_single_query(item: Tuple[str, Query]) -> Tuple[str, pd.DataFrame]:
-            view_name, query = item
-            if isinstance(query, str):
-                return view_name, self._render_dataframe_from_sql(view_name, query)
-            else:
-                return view_name, self._render_dataframe_from_py_func(view_name, query)
-        
-        with concurrent.futures.ThreadPoolExecutor() as executor:
-            df_by_view_name = executor.map(run_single_query, query_by_db_view.items())
-        
-        return dict(df_by_view_name)
-    
-    def _render_final_view_dataframe(self, df_by_db_views: Dict[str, pd.DataFrame], 
-                                    final_view_query: Optional[Query]) -> pd.DataFrame:
-        if final_view_query in df_by_db_views:
-            return df_by_db_views[final_view_query]
-        elif isinstance(final_view_query, str):
-            return self._render_dataframe_from_sql("final_view", final_view_query, df_by_db_views)
-        else:
-            return self._render_dataframe_from_py_func("final_view", final_view_query, df_by_db_views)
-
-    def load_results(self, selections: Dict[str, str], run_query: bool = True) \
-        -> Tuple[ParameterSet, Dict[str, Query], Query, Dict[str, pd.DataFrame], Optional[pd.DataFrame]]:
-        
-        # apply selections and render context
-        param_set = self.apply_selections(selections)
-        start = time.time()
-        context = self._render_context(self.context_func, param_set)
-        timer.add_activity_time(f"render context - dataset {self.dataset}", start)
-
-        # render database view queries
-        start = time.time()
-        query_by_db_view = {}
-        for db_view, raw_query in self.raw_query_by_db_view.items():
-            args = self._get_args(param_set, context, db_view)
-            query_by_db_view[db_view] = self._render_query_from_raw(raw_query, args)
-        timer.add_activity_time(f"render database view queries - dataset {self.dataset}", start)
-
-        # render final view query
-        start = time.time()
-        args = self._get_args(param_set, context)
-        final_view_query = self._render_query_from_raw(self.raw_final_view_query, args)
-        timer.add_activity_time(f"render final view query - dataset {self.dataset}", start)
-
-        # render all dataframes if "run_query" is enabled
-        df_by_db_views = {}
-        final_view_df = None
-        if run_query:
-            start = time.time()
-            df_by_db_views = self._render_db_view_dataframes(query_by_db_view)
-            timer.add_activity_time(f"execute dataview view queries - dataset {self.dataset}", start)
-
-            start = time.time()
-            final_view_df = self._render_final_view_dataframe(df_by_db_views, final_view_query)
-            timer.add_activity_time(f"execute final view query - dataset {self.dataset}", start)
-        
-        return param_set, query_by_db_view, final_view_query, df_by_db_views, final_view_df
-
-
-def default_context_func(*args, **kwargs):
-    return {}
-
-
-class RendererIOWrapper:
-    def __init__(self, dataset: str, manifest: mf.Manifest, conn_set: ConnectionSet, excel_file_name: Optional[str] = None):
-        dataset_folder = manifest.get_dataset_folder(dataset)
-        parameters_path = _utils.join_paths(dataset_folder, c.PARAMETERS_FILE)
-        args = manifest.get_dataset_args(dataset)
-        parameters_module = _utils.import_file_as_module(parameters_path)
-        try:
-            parameter_set = ParameterSet(parameters_module.main(args=args))
-        except Exception as e:
-            raise ConfigurationError(f'Error in the {c.PARAMETERS_FILE} function for dataset "{dataset}"') from e
-
-        context_path = _utils.join_paths(dataset_folder, c.CONTEXT_FILE)
-        try:
-            context_module = _utils.import_file_as_module(context_path)
-            context_func = partial(context_module.main, args=args)
-        except FileNotFoundError:
-            context_func = default_context_func
-        
-        excel_file = None
-        if excel_file_name is not None:
-            excel_file_path = _utils.join_paths(dataset_folder, excel_file_name)
-            excel_file = pd.ExcelFile(excel_file_path)
-        
-        db_views = manifest.get_all_database_view_names(dataset)
-        raw_query_by_db_view = {}
-        for db_view in db_views:
-            db_view_template_path = str(manifest.get_database_view_file(dataset, db_view))
-            raw_query_by_db_view[db_view] = self._get_raw_query(db_view_template_path)
-        
-        final_view_path = str(manifest.get_dataset_final_view_file(dataset))
-        if final_view_path in db_views:
-            raw_final_view_query = final_view_path
-        else:
-            raw_final_view_query = self._get_raw_query(final_view_path)
-        
-        self.dataset_folder = dataset_folder
-        self.output_folder = _utils.join_paths(c.OUTPUTS_FOLDER, dataset)
-        self.renderer = Renderer(dataset, manifest, conn_set, parameter_set, context_func,
-                                 raw_query_by_db_view, raw_final_view_query, excel_file)
-    
-    def _get_raw_query(self, template_path: str) -> Dict[str, Query]:
-        if template_path.endswith(".py"):
-            return _utils.import_file_as_module(template_path).main
-        else:
-            with open(template_path, 'r') as f:
-                sql_template = f.read()
-            return sql_template
-
-    def _get_selections(self, selection_cfg_file: Optional[str]) -> Dict[str, str]:
-        if selection_cfg_file is not None:
-            selection_cfg_path = _utils.join_paths(self.dataset_folder, selection_cfg_file)
-            config = ConfigParser()
-            config.read(selection_cfg_path)
-            if config.has_section(c.PARAMETERS_SECTION):
-                config_section = config[c.PARAMETERS_SECTION]
-                return dict(config_section.items())
-        return {}
-
-    def _write_sql_file(self, view_name: str, query: Any):
-        if isinstance(query, str):
-            db_view_sql_output_path = _utils.join_paths(self.output_folder, view_name+'.sql')
-            with open(db_view_sql_output_path, 'w') as f:
-                f.write(query)
-    
-    def write_outputs(self, selection_cfg_file: Optional[str], run_query: bool) -> None:
-        # create output folder if it doesn't exist
-        if not os.path.exists(self.output_folder):
-            os.makedirs(self.output_folder)
-        
-        # clear everything in output folder
-        files = os.listdir(self.output_folder)
-        for file in files:
-            file_path = _utils.join_paths(self.output_folder, file)
-            os.remove(file_path)
-        
-        # apply selections and render outputs
-        selections = self._get_selections(selection_cfg_file)
-        result = self.renderer.load_results(selections, run_query)
-        param_set, query_by_db_view, final_view_query, df_by_db_views, final_view_df = result
-        
-        # write the parameters response
-        param_set_dict = param_set.to_json_dict()
-        parameter_json_output_path = _utils.join_paths(self.output_folder, c.PARAMETERS_OUTPUT)
-        with open(parameter_json_output_path, 'w') as f:
-            json.dump(param_set_dict, f, indent=4)
-        
-        # write the rendered sql queries for database views
-        for db_view, query in query_by_db_view.items():
-            self._write_sql_file(db_view, query)
-
-        # write the rendered sql query for final view
-        if final_view_query not in query_by_db_view:
-            self._write_sql_file(c.FINAL_VIEW_OUT_STEM, final_view_query)
-        
-        # Run the sql queries and write output
-        if run_query:
-            for db_view, df in df_by_db_views.items():
-                csv_file = _utils.join_paths(self.output_folder, db_view+'.csv')
-                df.to_csv(csv_file, index=False)
-            
-            final_csv_path = _utils.join_paths(self.output_folder, c.FINAL_VIEW_OUT_STEM+'.csv')
-            final_view_df.to_csv(final_csv_path, index=False)
-
-            final_json_path = _utils.join_paths(self.output_folder, c.FINAL_VIEW_OUT_STEM+'.json')
-            final_view_df.to_json(final_json_path, orient='table', index=False, indent=4)
+from typing import Dict, Tuple, Optional, Union, Callable, Any
+from functools import partial
+from configparser import ConfigParser
+import concurrent.futures, os, json, time
+
+from squirrels import _constants as c, _manifest as mf, _utils
+from squirrels.connection_set import ConnectionSet, sqldf
+from squirrels.data_sources import DataSource
+from squirrels._parameter_set import ParameterSet
+from squirrels._utils import ConfigurationError
+from squirrels._timed_imports import pandas as pd, timer
+
+ContextFunc = Optional[Callable[..., Dict[str, Any]]]
+DatabaseViews = Optional[Dict[str, pd.DataFrame]]
+Query = Union[Callable[..., pd.DataFrame], str]
+
+
+class Renderer:
+    def __init__(self, dataset: str, manifest: mf.Manifest, conn_set: ConnectionSet, raw_param_set: ParameterSet, 
+                 context_func: Callable[..., Dict[str, Any]], raw_query_by_db_view: Dict[str, Query], 
+                 raw_final_view_query: Query, excel_file: Optional[pd.ExcelFile] = None):
+        self.dataset = dataset
+        self.manifest = manifest
+        self.conn_set = conn_set
+        self.context_func = context_func
+        self.raw_query_by_db_view = raw_query_by_db_view
+        self.raw_final_view_query = raw_final_view_query
+
+        start = time.time()
+        self.param_set: ParameterSet = self._convert_param_set_datasources(raw_param_set, excel_file)
+        timer.add_activity_time(f"convert datasources - dataset {dataset}", start)
+    
+    def _convert_param_set_datasources(self, param_set: ParameterSet, excel_file: Optional[pd.ExcelFile] = None) -> ParameterSet:
+        datasources = param_set.get_datasources()
+        if excel_file is not None:
+            df_dict = pd.read_excel(excel_file, None)
+            for key in datasources:
+                if key not in df_dict:
+                    raise ConfigurationError('No sheet found for parameter "{key}" in the Excel workbook')
+        else:
+            def get_dataframe_from_query(item: Tuple[str, DataSource]) -> pd.DataFrame:
+                key, datasource = item
+                df = self.conn_set.get_dataframe_from_query(datasource.connection_name, datasource.get_query())
+                return key, df
+            
+            with concurrent.futures.ThreadPoolExecutor() as executor:
+                df_dict = dict(executor.map(get_dataframe_from_query, datasources.items()))
+        
+        param_set.convert_datasource_params(df_dict)
+        return param_set
+    
+    def apply_selections(self, selections: Dict[str, str], updates_only: bool = False) -> ParameterSet:
+        start = time.time()
+        parameter_set = self.param_set
+        parameters_dict = parameter_set.get_parameters_as_ordered_dict()
+        
+        # iterating through parameters dict instead of query_params since order matters for cascading parameters
+        for param_name, parameter in parameters_dict.items():
+            if param_name in selections:
+                value = selections[param_name]
+                parameter = parameter_set.get_parameter(param_name).with_selection(value)
+                updates = parameter.get_all_dependent_params()
+                if updates_only:
+                    parameter_set = updates
+                    break
+                parameter_set = parameter_set.merge(updates)
+        timer.add_activity_time(f"apply selections - dataset {self.dataset}", start)
+        
+        return parameter_set
+
+    def _render_context(self, context_func: ContextFunc, param_set: ParameterSet) -> Dict[str, Any]:
+        try:
+            return context_func(prms=param_set.get_parameters_as_ordered_dict()) if context_func is not None else {}
+        except Exception as e:
+            raise ConfigurationError(f'Error in the {c.CONTEXT_FILE} function for dataset "{self.dataset}"') from e
+    
+    def _get_args(self, param_set: ParameterSet, context: Dict[str, Any], db_view: str = None) -> Dict:
+        if db_view is not None:
+            args = self.manifest.get_view_args(self.dataset, db_view)
+        else:
+            args = self.manifest.get_view_args(self.dataset)
+        return {
+            'prms': param_set.get_parameters_as_ordered_dict(),
+            'ctx':  context,
+            'args': args
+        }
+    
+    def _render_query_from_raw(self, raw_query: Query, args: Dict) -> Query:
+        if isinstance(raw_query, str):
+            template = _utils.j2_env.from_string(raw_query)
+            return template.render(args)
+        else:
+            return partial(raw_query, **args)
+    
+    def _render_dataframe_from_sql(self, db_view_name: str, sql_str: str, 
+                                   database_views: DatabaseViews = None) -> pd.DataFrame:
+        if database_views is not None:
+            return sqldf(sql_str, database_views)
+        else:
+            conn_name = self.manifest.get_database_view_db_connection(self.dataset, db_view_name)
+            return self.conn_set.get_dataframe_from_query(conn_name, sql_str)
+
+    def _render_dataframe_from_py_func(self, db_view_name: str, py_func: Callable[[Any], pd.DataFrame], 
+                                       database_views: DatabaseViews = None) -> pd.DataFrame:
+        if database_views is not None:
+            try:
+                return py_func(database_views=database_views)
+            except Exception as e:
+                raise ConfigurationError(f'Error in the final view python function for dataset "{self.dataset}"') from e
+        else:
+            conn_name = self.manifest.get_database_view_db_connection(self.dataset, db_view_name)
+            connection_pool = self.conn_set.get_connection_pool(conn_name)
+            try:
+                return py_func(connection_pool=connection_pool, connection_set=self.conn_set)
+            except Exception as e:
+                raise ConfigurationError(f'Error in the python function for database view "{db_view_name}" in dataset "{self.dataset}"') from e
+    
+    def _render_db_view_dataframes(self, query_by_db_view: Dict[str, Query]) -> Dict[str, pd.DataFrame]:
+        def run_single_query(item: Tuple[str, Query]) -> Tuple[str, pd.DataFrame]:
+            view_name, query = item
+            if isinstance(query, str):
+                return view_name, self._render_dataframe_from_sql(view_name, query)
+            else:
+                return view_name, self._render_dataframe_from_py_func(view_name, query)
+        
+        with concurrent.futures.ThreadPoolExecutor() as executor:
+            df_by_view_name = executor.map(run_single_query, query_by_db_view.items())
+        
+        return dict(df_by_view_name)
+    
+    def _render_final_view_dataframe(self, df_by_db_views: Dict[str, pd.DataFrame], 
+                                    final_view_query: Optional[Query]) -> pd.DataFrame:
+        if final_view_query in df_by_db_views:
+            return df_by_db_views[final_view_query]
+        elif isinstance(final_view_query, str):
+            return self._render_dataframe_from_sql("final_view", final_view_query, df_by_db_views)
+        else:
+            return self._render_dataframe_from_py_func("final_view", final_view_query, df_by_db_views)
+
+    def load_results(self, selections: Dict[str, str], run_query: bool = True) \
+        -> Tuple[ParameterSet, Dict[str, Query], Query, Dict[str, pd.DataFrame], Optional[pd.DataFrame]]:
+        
+        # apply selections and render context
+        param_set = self.apply_selections(selections)
+        start = time.time()
+        context = self._render_context(self.context_func, param_set)
+        timer.add_activity_time(f"render context - dataset {self.dataset}", start)
+
+        # render database view queries
+        start = time.time()
+        query_by_db_view = {}
+        for db_view, raw_query in self.raw_query_by_db_view.items():
+            args = self._get_args(param_set, context, db_view)
+            query_by_db_view[db_view] = self._render_query_from_raw(raw_query, args)
+        timer.add_activity_time(f"render database view queries - dataset {self.dataset}", start)
+
+        # render final view query
+        start = time.time()
+        args = self._get_args(param_set, context)
+        final_view_query = self._render_query_from_raw(self.raw_final_view_query, args)
+        timer.add_activity_time(f"render final view query - dataset {self.dataset}", start)
+
+        # render all dataframes if "run_query" is enabled
+        df_by_db_views = {}
+        final_view_df = None
+        if run_query:
+            start = time.time()
+            df_by_db_views = self._render_db_view_dataframes(query_by_db_view)
+            timer.add_activity_time(f"execute dataview view queries - dataset {self.dataset}", start)
+
+            start = time.time()
+            final_view_df = self._render_final_view_dataframe(df_by_db_views, final_view_query)
+            timer.add_activity_time(f"execute final view query - dataset {self.dataset}", start)
+        
+        return param_set, query_by_db_view, final_view_query, df_by_db_views, final_view_df
+
+
+def default_context_func(*args, **kwargs):
+    return {}
+
+
+class RendererIOWrapper:
+    def __init__(self, dataset: str, manifest: mf.Manifest, conn_set: ConnectionSet, excel_file_name: Optional[str] = None):
+        dataset_folder = manifest.get_dataset_folder(dataset)
+        parameters_path = _utils.join_paths(dataset_folder, c.PARAMETERS_FILE)
+        args = manifest.get_dataset_args(dataset)
+        parameters_module = _utils.import_file_as_module(parameters_path)
+        try:
+            parameter_set = ParameterSet(parameters_module.main(args=args))
+        except Exception as e:
+            raise ConfigurationError(f'Error in the {c.PARAMETERS_FILE} function for dataset "{dataset}"') from e
+
+        context_path = _utils.join_paths(dataset_folder, c.CONTEXT_FILE)
+        try:
+            context_module = _utils.import_file_as_module(context_path)
+            context_func = partial(context_module.main, args=args)
+        except FileNotFoundError:
+            context_func = default_context_func
+        
+        excel_file = None
+        if excel_file_name is not None:
+            excel_file_path = _utils.join_paths(dataset_folder, excel_file_name)
+            excel_file = pd.ExcelFile(excel_file_path)
+        
+        db_views = manifest.get_all_database_view_names(dataset)
+        raw_query_by_db_view = {}
+        for db_view in db_views:
+            db_view_template_path = str(manifest.get_database_view_file(dataset, db_view))
+            raw_query_by_db_view[db_view] = self._get_raw_query(db_view_template_path)
+        
+        final_view_path = str(manifest.get_dataset_final_view_file(dataset))
+        if final_view_path in db_views:
+            raw_final_view_query = final_view_path
+        else:
+            raw_final_view_query = self._get_raw_query(final_view_path)
+        
+        self.dataset_folder = dataset_folder
+        self.output_folder = _utils.join_paths(c.OUTPUTS_FOLDER, dataset)
+        self.renderer = Renderer(dataset, manifest, conn_set, parameter_set, context_func,
+                                 raw_query_by_db_view, raw_final_view_query, excel_file)
+    
+    def _get_raw_query(self, template_path: str) -> Dict[str, Query]:
+        if template_path.endswith(".py"):
+            return _utils.import_file_as_module(template_path).main
+        else:
+            with open(template_path, 'r') as f:
+                sql_template = f.read()
+            return sql_template
+
+    def _get_selections(self, selection_cfg_file: Optional[str]) -> Dict[str, str]:
+        if selection_cfg_file is not None:
+            selection_cfg_path = _utils.join_paths(self.dataset_folder, selection_cfg_file)
+            config = ConfigParser()
+            config.read(selection_cfg_path)
+            if config.has_section(c.PARAMETERS_SECTION):
+                config_section = config[c.PARAMETERS_SECTION]
+                return dict(config_section.items())
+        return {}
+
+    def _write_sql_file(self, view_name: str, query: Any):
+        if isinstance(query, str):
+            db_view_sql_output_path = _utils.join_paths(self.output_folder, view_name+'.sql')
+            with open(db_view_sql_output_path, 'w') as f:
+                f.write(query)
+    
+    def write_outputs(self, selection_cfg_file: Optional[str], run_query: bool) -> None:
+        # create output folder if it doesn't exist
+        if not os.path.exists(self.output_folder):
+            os.makedirs(self.output_folder)
+        
+        # clear everything in output folder
+        files = os.listdir(self.output_folder)
+        for file in files:
+            file_path = _utils.join_paths(self.output_folder, file)
+            os.remove(file_path)
+        
+        # apply selections and render outputs
+        selections = self._get_selections(selection_cfg_file)
+        result = self.renderer.load_results(selections, run_query)
+        param_set, query_by_db_view, final_view_query, df_by_db_views, final_view_df = result
+        
+        # write the parameters response
+        param_set_dict = param_set.to_json_dict()
+        parameter_json_output_path = _utils.join_paths(self.output_folder, c.PARAMETERS_OUTPUT)
+        with open(parameter_json_output_path, 'w') as f:
+            json.dump(param_set_dict, f, indent=4)
+        
+        # write the rendered sql queries for database views
+        for db_view, query in query_by_db_view.items():
+            self._write_sql_file(db_view, query)
+
+        # write the rendered sql query for final view
+        if final_view_query not in query_by_db_view:
+            self._write_sql_file(c.FINAL_VIEW_OUT_STEM, final_view_query)
+        
+        # Run the sql queries and write output
+        if run_query:
+            for db_view, df in df_by_db_views.items():
+                csv_file = _utils.join_paths(self.output_folder, db_view+'.csv')
+                df.to_csv(csv_file, index=False)
+            
+            final_csv_path = _utils.join_paths(self.output_folder, c.FINAL_VIEW_OUT_STEM+'.csv')
+            final_view_df.to_csv(final_csv_path, index=False)
+
+            final_json_path = _utils.join_paths(self.output_folder, c.FINAL_VIEW_OUT_STEM+'.json')
+            final_view_df.to_json(final_json_path, orient='table', index=False, indent=4)
```

### Comparing `squirrels-0.1.0/squirrels/data_sources.py` & `squirrels-0.1.1.post1/squirrels/data_sources.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,282 +1,290 @@
-from __future__ import annotations
-from typing import Type, Tuple, List, Optional
-from dataclasses import dataclass
-
-from squirrels import parameters as p, parameter_options as po
-from squirrels._timed_imports import pandas as pd
-from squirrels import _constants as c, _utils
-
-
-@dataclass
-class DataSource:
-    """
-    Abstract class for lookup tables coming from a database
-    """
-    table_or_query: str
-    
-    def __post_init__(self) -> None:
-        if not hasattr(self, 'parent_id_col'):
-            self.parent_id_col = None
-        if not hasattr(self, 'connection_name'):
-            self.connection_name = c.DEFAULT_DB_CONN
-
-    def get_query(self) -> str:
-        """
-        Get the "table_or_query" attribute as a select query
-
-        Returns:
-            str: The converted select query
-        """
-        if self.table_or_query.lower().startswith('select '):
-            query = self.table_or_query
-        else:
-            query = f'SELECT * FROM {self.table_or_query}'
-        return query
-    
-    def convert(self, ds_param: p.DataSourceParameter, df: pd.DataFrame) -> p.Parameter:
-        """
-        An abstract method for converting itself into a parameter
-
-        Args:
-            ds_param: The parameter to convert
-            df: The dataframe containing the parameter options data
-
-        Returns:
-            The converted parameter
-        """
-        raise _utils.AbstractMethodCallError(self.__class__, "convert")
-    
-    def _get_parent(self, row):
-        return str(_utils.get_row_value(row, self.parent_id_col)) if self.parent_id_col is not None else None
-    
-    def _validate_parameter_class(self, ds_param: p.DataSourceParameter, parameter_classes: List[Type[p.Parameter]]) -> None:
-        if ds_param.parameter_class not in parameter_classes:
-            parameter_class_name = ds_param.parameter_class.__name__
-            datasource_class_name = self.__class__.__name__
-            raise _utils.ConfigurationError(f'Invalid widget type "{parameter_class_name}" for {datasource_class_name}')
-
-
-@dataclass
-class SelectionDataSource(DataSource):
-    """
-    Lookup table for selection parameters (single and multi)
-
-    Attributes:
-        connection_name: Name of the connection to use defined in connections.py
-        table_or_query: Either the name of the table to use, or a query to run
-        id_col: The column name of the id
-        options_col: The column name of the options
-        order_by_col: The column name to order the options by. Orders by the id_col instead if this is None
-        is_default_col: The column name that indicates which options are the default
-        parent_id_col: The column name of the parent option id that this option belongs to
-    """
-    id_col: str
-    options_col: str
-    order_by_col: Optional[str] = None
-    is_default_col: Optional[str] = None
-    parent_id_col: Optional[str] = None
-    connection_name: str = c.DEFAULT_DB_CONN
-
-    def __post_init__(self):
-        self.order_by_col = self.order_by_col if self.order_by_col is not None else self.id_col
-
-    def convert(self, ds_param: p.DataSourceParameter, df: pd.DataFrame) -> p.Parameter:
-        """
-        Method to convert the associated DataSourceParameter into a SingleSelect or MultiSelect Parameter
-
-        Parameters:
-            ds_param: The parameter to convert
-            df: The dataframe containing the parameter options data
-
-        Returns:
-            The converted parameter
-        """
-        self._validate_parameter_class(ds_param, [p.SingleSelectParameter, p.MultiSelectParameter])
-
-        def is_default(row):
-            return int(_utils.get_row_value(row, self.is_default_col)) == 1 if self.is_default_col is not None else False
-        
-        try:
-            df.sort_values(self.order_by_col, inplace=True)
-        except KeyError as e:
-            raise _utils.ConfigurationError(f'Could not sort on column name "{self.order_by_col}" as it does not exist')
-        
-        options = tuple(
-            po.SelectParameterOption(str(_utils.get_row_value(row, self.id_col)), str(_utils.get_row_value(row, self.options_col)), is_default(row), 
-                                     parent_option_id=self._get_parent(row))
-            for _, row in df.iterrows()
-        )
-        
-        return ds_param.parameter_class(ds_param.name, ds_param.label, options, is_hidden=ds_param.is_hidden, parent=ds_param.parent)
-
-
-@dataclass
-class DateDataSource(DataSource):
-    """
-    Lookup table for date parameter default options
-
-    Attributes:
-        connection_name: Name of the connection to use defined in connections.py
-        table_or_query: Either the name of the table to use, or a query to run
-        default_date_col: The column name of the default date
-        date_format: The format of the default date(s). Defaults to '%Y-%m-%d'
-        parent_id_col: The column name of the parent option id that the default date belongs to
-    """
-    default_date_col: str
-    parent_id_col: Optional[str] = None
-    date_format: Optional[str] = '%Y-%m-%d'
-    connection_name: str = c.DEFAULT_DB_CONN
-
-    def convert(self, ds_param: p.DataSourceParameter, df: pd.DataFrame) -> p.DateParameter:
-        """
-        Method to convert the associated DataSourceParameter into a DateParameter
-
-        Parameters:
-            ds_param: The parameter to convert
-            df: The dataframe containing the parameter options data
-
-        Returns:
-            The converted parameter
-        """
-        self._validate_parameter_class(ds_param, [p.DateParameter])
-        
-        def get_date(row: pd.Series) -> str:
-            return str(_utils.get_row_value(row, self.default_date_col))
-        
-        def create_date_param_option(row: pd.Series) -> po.DateParameterOption:
-            return po.DateParameterOption(get_date(row), self.date_format, self._get_parent(row))
-        
-        if ds_param.parent is None:
-            row = df.iloc[0]
-            return p.DateParameter(ds_param.name, ds_param.label, get_date(row), self.date_format, 
-                                   is_hidden=ds_param.is_hidden)
-        else:
-            all_options = tuple(create_date_param_option(row) for _, row in df.iterrows())
-            return p.DateParameter.WithParent(ds_param.name, ds_param.label, all_options, ds_param.parent,
-                                              is_hidden=ds_param.is_hidden)
-
-
-@dataclass
-class _NumericDataSource(DataSource):
-    """
-    Abstract class for number or number range data sources
-    """
-    min_value_col: str
-    max_value_col: str
-    increment_col: Optional[str] = None
-
-    def _convert_helper(self, row: pd.Series) -> Tuple[str, str, str]:
-        min_val = str(_utils.get_row_value(row, self.min_value_col))
-        max_val = str(_utils.get_row_value(row, self.max_value_col))
-        incr_val = str(_utils.get_row_value(row, self.increment_col)) if self.increment_col is not None else '1'
-        return min_val, max_val, incr_val
-
-@dataclass
-class NumberDataSource(_NumericDataSource):
-    """
-    Lookup table for number parameter default options
-
-    Attributes:
-        connection_name: Name of the connection to use defined in connections.py
-        table_or_query: Either the name of the table to use, or a query to run
-        min_value_col: The column name of the minimum value
-        max_value_col: The column name of the maximum value
-        increment_col: The column name of the increment value. Defaults to column of 1's if None
-        default_value_col: The column name of the default value. Defaults to min_value_col if None
-        parent_id_col: The column name of the parent option id that the default value belongs to
-    """
-    default_value_col: Optional[str] = None
-    parent_id_col: Optional[str] = None
-    connection_name: str = c.DEFAULT_DB_CONN
-
-    def convert(self, ds_param: p.DataSourceParameter, df: pd.DataFrame) -> p.NumberParameter:
-        """
-        Method to convert the associated DataSourceParameter into a NumberParameter
-
-        Parameters:
-            ds_param: The parameter to convert
-            df: The dataframe containing the parameter options data
-
-        Returns:
-            The converted parameter
-        """
-        self._validate_parameter_class(ds_param, [p.NumberParameter])
-
-        def _get_default_value(row: pd.Series) -> str:
-            return str(_utils.get_row_value(row, self.default_value_col)) if self.default_value_col is not None \
-                else str(_utils.get_row_value(row, self.min_value_col))
-        
-        def _create_num_param_option(row: pd.Series) -> po.NumberParameterOption:
-            min_value, max_value, increment = self._convert_helper(row)
-            return po.NumberParameterOption(min_value, max_value, increment, _get_default_value(row), 
-                                            self._get_parent(row))
-
-        if ds_param.parent is None:
-            row = df.iloc[0]
-            min_value, max_value, increment = self._convert_helper(row)
-            return p.NumberParameter(ds_param.name, ds_param.label, min_value, max_value, increment, 
-                                     _get_default_value(row), is_hidden=ds_param.is_hidden)
-        else:
-            all_options = tuple(_create_num_param_option(row) for _, row in df.iterrows())
-            return p.NumberParameter.WithParent(ds_param.name, ds_param.label, all_options, ds_param.parent,
-                                                is_hidden=ds_param.is_hidden)
-
-
-@dataclass
-class NumRangeDataSource(_NumericDataSource):
-    """
-    Lookup table for number range parameter default options
-
-    Attributes:
-        connection_name: Name of the connection to use defined in connections.py
-        table_or_query: Either the name of the table to use, or a query to run
-        min_value_col: The column name of the minimum value
-        max_value_col: The column name of the maximum value
-        increment_col: The column name of the increment value. Defaults to column of 1's if None
-        default_lower_value_col: The column name of the default lower value. Defaults to min_value_col if None
-        default_upper_value_col: The column name of the default upper value. Defaults to max_value_col if None
-        parent_id_col: The column name of the parent option id that the default value belongs to
-    """
-    default_lower_value_col: Optional[str] = None
-    default_upper_value_col: Optional[str] = None
-    parent_id_col: Optional[str] = None
-    connection_name: str = c.DEFAULT_DB_CONN
-
-    def convert(self, ds_param: p.DataSourceParameter, df: pd.DataFrame) -> p.NumRangeParameter:
-        """
-        Method to convert the associated DataSourceParameter into a NumRangeParameter
-
-        Parameters:
-            ds_param: The parameter to convert
-            df: The dataframe containing the parameter options data
-
-        Returns:
-            The converted parameter
-        """
-        self._validate_parameter_class(ds_param, [p.NumRangeParameter])
-
-        def _get_default_lower_upper_values(row: pd.Series) -> Tuple[str, str]:
-            lower_value_col = self.default_lower_value_col if self.default_lower_value_col is not None \
-                else self.min_value_col
-            upper_value_col = self.default_upper_value_col if self.default_upper_value_col is not None \
-                else self.max_value_col
-            lower_value = str(_utils.get_row_value(row, lower_value_col))
-            upper_value = str(_utils.get_row_value(row, upper_value_col))
-            return lower_value, upper_value
-        
-        def _create_range_param_option(row: pd.Series) -> po.NumRangeParameterOption:
-            min_value, max_value, increment = self._convert_helper(row)
-            lower_value, upper_value = _get_default_lower_upper_values(row)
-            return po.NumRangeParameterOption(min_value, max_value, increment, lower_value, upper_value, 
-                                           self._get_parent(row)) 
-
-        if ds_param.parent is None:
-            row = df.iloc[0]
-            min_value, max_value, increment = self._convert_helper(row)
-            lower_value, upper_value = _get_default_lower_upper_values(row)
-            return p.NumRangeParameter(ds_param.name, ds_param.label, min_value, max_value, increment, 
-                                    lower_value, upper_value, is_hidden=ds_param.is_hidden)
-        else:
-            all_options = tuple(_create_range_param_option(row) for _, row in df.iterrows())
-            return p.NumRangeParameter.WithParent(ds_param.name, ds_param.label, all_options, ds_param.parent,
-                                                  is_hidden=ds_param.is_hidden)
+from __future__ import annotations
+from typing import Type, Dict, Tuple, List, Optional
+from dataclasses import dataclass, field
+
+from squirrels import parameters as p, parameter_options as po
+from squirrels._timed_imports import pandas as pd
+from squirrels import _constants as c, _utils
+
+
+@dataclass
+class DataSource:
+    """
+    Abstract class for lookup tables coming from a database
+    """
+    table_or_query: str
+    
+    def __post_init__(self) -> None:
+        if not hasattr(self, 'parent_id_col'):
+            self.parent_id_col = None
+        if not hasattr(self, 'connection_name'):
+            self.connection_name = c.DEFAULT_DB_CONN
+
+    def get_query(self) -> str:
+        """
+        Get the "table_or_query" attribute as a select query
+
+        Returns:
+            str: The converted select query
+        """
+        if self.table_or_query.strip().lower().startswith('select '):
+            query = self.table_or_query
+        else:
+            query = f'SELECT * FROM {self.table_or_query}'
+        return query
+    
+    def convert(self, ds_param: p.DataSourceParameter, df: pd.DataFrame) -> p.Parameter:
+        """
+        An abstract method for converting itself into a parameter
+
+        Args:
+            ds_param: The parameter to convert
+            df: The dataframe containing the parameter options data
+
+        Returns:
+            The converted parameter
+        """
+        raise _utils.AbstractMethodCallError(self.__class__, "convert")
+    
+    def _get_parent(self, row):
+        return str(_utils.get_row_value(row, self.parent_id_col)) if self.parent_id_col is not None else None
+    
+    def _validate_parameter_class(self, ds_param: p.DataSourceParameter, parameter_classes: List[Type[p.Parameter]]) -> None:
+        if ds_param.parameter_class not in parameter_classes:
+            parameter_class_name = ds_param.parameter_class.__name__
+            datasource_class_name = self.__class__.__name__
+            raise _utils.ConfigurationError(f'Invalid widget type "{parameter_class_name}" for {datasource_class_name}')
+
+
+@dataclass
+class SelectionDataSource(DataSource):
+    """
+    Lookup table for selection parameters (single and multi)
+
+    Attributes:
+        table_or_query: Either the name of the table to use, or a query to run
+        id_col: The column name of the id
+        options_col: The column name of the options
+        order_by_col: The column name to order the options by. Orders by the id_col instead if this is None
+        is_default_col: The column name that indicates which options are the default
+        parent_id_col: The column name of the parent option id that this option belongs to
+        custom_cols: Dictionary of attribute to column name for custom fields for the SelectParameterOption
+        connection_name: Name of the connection to use defined in connections.py
+    """
+    id_col: str
+    options_col: str
+    order_by_col: Optional[str] = None
+    is_default_col: Optional[str] = None
+    parent_id_col: Optional[str] = None
+    custom_cols: Dict[str, str] = field(default_factory=dict)
+    connection_name: str = c.DEFAULT_DB_CONN
+
+    def __post_init__(self):
+        self.order_by_col = self.order_by_col if self.order_by_col is not None else self.id_col
+
+    def convert(self, ds_param: p.DataSourceParameter, df: pd.DataFrame) -> p.Parameter:
+        """
+        Method to convert the associated DataSourceParameter into a SingleSelect or MultiSelect Parameter
+
+        Parameters:
+            ds_param: The parameter to convert
+            df: The dataframe containing the parameter options data
+
+        Returns:
+            The converted parameter
+        """
+        self._validate_parameter_class(ds_param, [p.SingleSelectParameter, p.MultiSelectParameter])
+
+        def is_default(row):
+            return int(_utils.get_row_value(row, self.is_default_col)) == 1 if self.is_default_col is not None else False
+        
+        def get_custom_fields(row):
+            result = {}
+            for key, val in self.custom_cols.items():
+                result[key] = _utils.get_row_value(row, val)
+            return result
+        
+        try:
+            df.sort_values(self.order_by_col, inplace=True)
+        except KeyError as e:
+            raise _utils.ConfigurationError(f'Could not sort on column name "{self.order_by_col}" as it does not exist')
+        
+        options = tuple(
+            po.SelectParameterOption(str(_utils.get_row_value(row, self.id_col)), str(_utils.get_row_value(row, self.options_col)), 
+                                     is_default=is_default(row), parent_option_id=self._get_parent(row), custom_fields=get_custom_fields(row))
+            for _, row in df.iterrows()
+        )
+        
+        return ds_param.parameter_class(ds_param.name, ds_param.label, options, is_hidden=ds_param.is_hidden, parent=ds_param.parent)
+
+
+@dataclass
+class DateDataSource(DataSource):
+    """
+    Lookup table for date parameter default options
+
+    Attributes:
+        table_or_query: Either the name of the table to use, or a query to run
+        default_date_col: The column name of the default date
+        parent_id_col: The column name of the parent option id that the default date belongs to
+        date_format: The format of the default date(s). Defaults to '%Y-%m-%d'
+        connection_name: Name of the connection to use defined in connections.py
+    """
+    default_date_col: str
+    parent_id_col: Optional[str] = None
+    date_format: Optional[str] = '%Y-%m-%d'
+    connection_name: str = c.DEFAULT_DB_CONN
+
+    def convert(self, ds_param: p.DataSourceParameter, df: pd.DataFrame) -> p.DateParameter:
+        """
+        Method to convert the associated DataSourceParameter into a DateParameter
+
+        Parameters:
+            ds_param: The parameter to convert
+            df: The dataframe containing the parameter options data
+
+        Returns:
+            The converted parameter
+        """
+        self._validate_parameter_class(ds_param, [p.DateParameter])
+        
+        def get_date(row: pd.Series) -> str:
+            return str(_utils.get_row_value(row, self.default_date_col))
+        
+        def create_date_param_option(row: pd.Series) -> po.DateParameterOption:
+            return po.DateParameterOption(get_date(row), self.date_format, self._get_parent(row))
+        
+        if ds_param.parent is None:
+            row = df.iloc[0]
+            return p.DateParameter(ds_param.name, ds_param.label, get_date(row), self.date_format, 
+                                   is_hidden=ds_param.is_hidden)
+        else:
+            all_options = tuple(create_date_param_option(row) for _, row in df.iterrows())
+            return p.DateParameter.WithParent(ds_param.name, ds_param.label, all_options, ds_param.parent,
+                                              is_hidden=ds_param.is_hidden)
+
+
+@dataclass
+class _NumericDataSource(DataSource):
+    """
+    Abstract class for number or number range data sources
+    """
+    min_value_col: str
+    max_value_col: str
+    increment_col: Optional[str] = None
+
+    def _convert_helper(self, row: pd.Series) -> Tuple[str, str, str]:
+        min_val = str(_utils.get_row_value(row, self.min_value_col))
+        max_val = str(_utils.get_row_value(row, self.max_value_col))
+        incr_val = str(_utils.get_row_value(row, self.increment_col)) if self.increment_col is not None else '1'
+        return min_val, max_val, incr_val
+
+@dataclass
+class NumberDataSource(_NumericDataSource):
+    """
+    Lookup table for number parameter default options
+
+    Attributes:
+        table_or_query: Either the name of the table to use, or a query to run
+        min_value_col: The column name of the minimum value
+        max_value_col: The column name of the maximum value
+        increment_col: The column name of the increment value. Defaults to column of 1's if None
+        default_value_col: The column name of the default value. Defaults to min_value_col if None
+        parent_id_col: The column name of the parent option id that the default value belongs to
+        connection_name: Name of the connection to use defined in connections.py
+    """
+    default_value_col: Optional[str] = None
+    parent_id_col: Optional[str] = None
+    connection_name: str = c.DEFAULT_DB_CONN
+
+    def convert(self, ds_param: p.DataSourceParameter, df: pd.DataFrame) -> p.NumberParameter:
+        """
+        Method to convert the associated DataSourceParameter into a NumberParameter
+
+        Parameters:
+            ds_param: The parameter to convert
+            df: The dataframe containing the parameter options data
+
+        Returns:
+            The converted parameter
+        """
+        self._validate_parameter_class(ds_param, [p.NumberParameter])
+
+        def _get_default_value(row: pd.Series) -> str:
+            return str(_utils.get_row_value(row, self.default_value_col)) if self.default_value_col is not None \
+                else str(_utils.get_row_value(row, self.min_value_col))
+        
+        def _create_num_param_option(row: pd.Series) -> po.NumberParameterOption:
+            min_value, max_value, increment = self._convert_helper(row)
+            return po.NumberParameterOption(min_value, max_value, increment, _get_default_value(row), 
+                                            self._get_parent(row))
+
+        if ds_param.parent is None:
+            row = df.iloc[0]
+            min_value, max_value, increment = self._convert_helper(row)
+            return p.NumberParameter(ds_param.name, ds_param.label, min_value, max_value, increment, 
+                                     _get_default_value(row), is_hidden=ds_param.is_hidden)
+        else:
+            all_options = tuple(_create_num_param_option(row) for _, row in df.iterrows())
+            return p.NumberParameter.WithParent(ds_param.name, ds_param.label, all_options, ds_param.parent,
+                                                is_hidden=ds_param.is_hidden)
+
+
+@dataclass
+class NumRangeDataSource(_NumericDataSource):
+    """
+    Lookup table for number range parameter default options
+
+    Attributes:
+        table_or_query: Either the name of the table to use, or a query to run
+        min_value_col: The column name of the minimum value
+        max_value_col: The column name of the maximum value
+        increment_col: The column name of the increment value. Defaults to column of 1's if None
+        default_lower_value_col: The column name of the default lower value. Defaults to min_value_col if None
+        default_upper_value_col: The column name of the default upper value. Defaults to max_value_col if None
+        parent_id_col: The column name of the parent option id that the default value belongs to
+        connection_name: Name of the connection to use defined in connections.py
+    """
+    default_lower_value_col: Optional[str] = None
+    default_upper_value_col: Optional[str] = None
+    parent_id_col: Optional[str] = None
+    connection_name: str = c.DEFAULT_DB_CONN
+
+    def convert(self, ds_param: p.DataSourceParameter, df: pd.DataFrame) -> p.NumRangeParameter:
+        """
+        Method to convert the associated DataSourceParameter into a NumRangeParameter
+
+        Parameters:
+            ds_param: The parameter to convert
+            df: The dataframe containing the parameter options data
+
+        Returns:
+            The converted parameter
+        """
+        self._validate_parameter_class(ds_param, [p.NumRangeParameter])
+
+        def _get_default_lower_upper_values(row: pd.Series) -> Tuple[str, str]:
+            lower_value_col = self.default_lower_value_col if self.default_lower_value_col is not None \
+                else self.min_value_col
+            upper_value_col = self.default_upper_value_col if self.default_upper_value_col is not None \
+                else self.max_value_col
+            lower_value = str(_utils.get_row_value(row, lower_value_col))
+            upper_value = str(_utils.get_row_value(row, upper_value_col))
+            return lower_value, upper_value
+        
+        def _create_range_param_option(row: pd.Series) -> po.NumRangeParameterOption:
+            min_value, max_value, increment = self._convert_helper(row)
+            lower_value, upper_value = _get_default_lower_upper_values(row)
+            return po.NumRangeParameterOption(min_value, max_value, increment, lower_value, upper_value, 
+                                           self._get_parent(row)) 
+
+        if ds_param.parent is None:
+            row = df.iloc[0]
+            min_value, max_value, increment = self._convert_helper(row)
+            lower_value, upper_value = _get_default_lower_upper_values(row)
+            return p.NumRangeParameter(ds_param.name, ds_param.label, min_value, max_value, increment, 
+                                    lower_value, upper_value, is_hidden=ds_param.is_hidden)
+        else:
+            all_options = tuple(_create_range_param_option(row) for _, row in df.iterrows())
+            return p.NumRangeParameter.WithParent(ds_param.name, ds_param.label, all_options, ds_param.parent,
+                                                  is_hidden=ds_param.is_hidden)
```

### Comparing `squirrels-0.1.0/squirrels/dateutils.py` & `squirrels-0.1.1.post1/squirrels/dateutils.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,380 +1,430 @@
-from typing import Sequence
-from dataclasses import dataclass
-from datetime import datetime
-from dateutil.relativedelta import relativedelta
-from enum import Enum
-
-from squirrels import _utils
-
-
-class DayOfWeek(Enum):
-    Sunday = 0
-    Monday = 1
-    Tuesday = 2
-    Wednesday = 3
-    Thursday = 4
-    Friday = 5
-    Saturday = 6
-
-class Month(Enum):
-    January = 1
-    February = 2
-    March = 3
-    April = 4
-    May = 5
-    June = 6
-    July = 7
-    August = 8
-    September = 9
-    October = 10
-    November = 11
-    December = 12
-
-
-@dataclass
-class DateModifier:
-    """
-    Interface for all Date modification classes, and declares a "modify" method
-    """
-
-    def modify(self, date: datetime) -> datetime:
-        """
-        Method to be overwritten, modifies the input date
-
-        Parameters:
-            date: The input date to modify.
-
-        Returns:
-            The modified date.
-        """
-        raise _utils.AbstractMethodCallError(self.__class__, "modify")
-
-
-@dataclass
-class _DayIdxOfCalendarUnit(DateModifier):
-    """
-    Interface for adjusting a date to some day of calendar unit
-    """
-    idx: int
-
-    def __post_init__(self):
-        if self.idx == 0:
-            raise _utils.ConfigurationError("The idx attribute of any DateModifier object cannot be zero")
-        self.incr = self.idx - 1 if self.idx > 0 else self.idx
-
-
-@dataclass
-class DayIdxOfMonthsCycle(_DayIdxOfCalendarUnit):
-    """
-    DateModifier class to get the idx-th day of a cycle of months for an input date
-
-    Attributes:
-        idx: 1 for first, 2 for second, etc. Or, -1 for last, -2 for second last, etc. Must not be 0
-        num_months_in_cycle: 2 for one 6th of year, 3 for Quarter, 4 for one 3rd of year, 6 for half year, 12 for full year. Must fit evenly in 12
-        first_month_of_cycle: The first month of months cycle of year. Default is January
-    """
-    num_months_in_cycle: int
-    first_month_of_cycle: Month = Month.January
-
-    def __post_init__(self):
-        super().__post_init__()
-        if 12 % self.num_months_in_cycle != 0:
-            raise _utils.ConfigurationError("Value X must fit evenly in 12")
-        self.first_month_of_first_cycle = (self.first_month_of_cycle.value - 1) % self.num_months_in_cycle + 1
-
-    def modify(self, date: datetime) -> datetime:
-        current_cycle = (date.month - self.first_month_of_first_cycle) % 12 // self.num_months_in_cycle
-        first_month_of_curr_cycle = current_cycle * self.num_months_in_cycle + self.first_month_of_first_cycle
-        year = date.year if date.month >= first_month_of_curr_cycle else date.year - 1
-        first_day = datetime(year, first_month_of_curr_cycle, 1)
-        ref_date = first_day if self.idx > 0 else first_day + relativedelta(months=self.num_months_in_cycle)
-        return ref_date + relativedelta(days=self.incr)
-
-
-@dataclass
-class DayIdxOfYear(DayIdxOfMonthsCycle):
-    """
-    DateModifier class to get the idx-th day of year of an input date
-
-    Attributes:
-        idx: 1 for first, 2 for second, etc. Or, -1 for last, -2 for second last, etc. Must not be 0
-        first_month_of_year: The first month of year. Default is January
-    """
-
-    def __init__(self, idx: int, first_month_of_year: Month = Month.January):
-        super().__init__(idx, num_months_in_cycle=12, first_month_of_cycle=first_month_of_year)
-
-
-@dataclass
-class DayIdxOfQuarter(DayIdxOfMonthsCycle):
-    """
-    DateModifier class to get the idx-th day of quarter of an input date
-
-    Attributes:
-        idx: 1 for first, 2 for second, etc. Or, -1 for last, -2 for second last, etc. Must not be 0
-        first_month_of_quarter: The first month of first quarter. Default is January
-    """
-
-    def __init__(self, idx: int, first_month_of_quarter: Month = Month.January):
-        super().__init__(idx, num_months_in_cycle=3, first_month_of_cycle=first_month_of_quarter)
-
-
-@dataclass
-class DayIdxOfMonth(_DayIdxOfCalendarUnit):
-    """
-    DateModifier class to get the idx-th day of month of an input date
-
-    Attributes:
-        idx: 1 for first, 2 for second, etc. Or, -1 for last, -2 for second last, etc. Must not be 0
-    """
-
-    def modify(self, date: datetime) -> datetime:
-        first_day = datetime(date.year, date.month, 1)
-        ref_date = first_day if self.idx > 0 else first_day + relativedelta(months=1)
-        return ref_date + relativedelta(days=self.incr)
-
-
-@dataclass
-class DayIdxOfWeek(_DayIdxOfCalendarUnit):
-    """
-    DateModifier class to get the idx-th day of week of an input date
-
-    Attributes:
-        idx: 1 for first, 2 for second, etc. Or, -1 for last, -2 for second last, etc. Must not be 0
-        first_day_of_week: The day of week identified as the "first". Default is Monday
-    """
-    first_day_of_week: DayOfWeek = DayOfWeek.Monday
-
-    def __post_init__(self):
-        super().__post_init__()
-        self.first_dow_num = self.first_day_of_week.value
-    
-    def modify(self, date: datetime) -> datetime:
-        distance_from_first_day = (1 + date.weekday() - self.first_dow_num) % 7
-        total_incr = -distance_from_first_day + (7 if self.idx < 0 else 0) + self.incr
-        return date + relativedelta(days=total_incr)
-
-
-@dataclass
-class _OffsetUnits(DateModifier):
-    """
-    Abstract DateModifier class to offset an input date by some number of some calendar unit
-    """
-    offset: int
-
-
-@dataclass
-class OffsetYears(_OffsetUnits):
-    """
-    DateModifier class to offset an input date by some number of years
-
-    Attributes:
-        offset: The number of years to offset the input date.
-    """
-
-    def modify(self, date: datetime) -> datetime:
-        return date + relativedelta(years=self.offset)
-    
-
-@dataclass
-class OffsetMonths(_OffsetUnits):
-    """
-    DateModifier class to offset an input date by some number of months
-
-    Attributes:
-        offset: The number of months to offset the input date.
-    """
-
-    def modify(self, date: datetime) -> datetime:
-        return date + relativedelta(months=self.offset)
-
-
-@dataclass
-class OffsetWeeks(_OffsetUnits):
-    """
-    DateModifier class to offset an input date by some number of weeks
-
-    Attributes:
-        offset: The number of weeks to offset the input date.
-    """
-
-    def modify(self, date: datetime) -> datetime:
-        return date + relativedelta(weeks=self.offset)
-
-
-@dataclass
-class OffsetDays(_OffsetUnits):
-    """
-    DateModifier class to offset an input date by some number of days
-
-    Attributes:
-        offset: The number of days to offset the input date.
-    """
-
-    def modify(self, date: datetime) -> datetime:
-        return date + relativedelta(days=self.offset)
-
-
-@dataclass
-class DateModPipeline(DateModifier):
-    """
-    DateModifier class to apply a list of date modifiers to an input date
-
-    Attributes:
-        modifiers: The list of DateModifier's to apply in sequence.
-    """
-    modifiers: Sequence[DateModifier]
-
-    def __post_init__(self):
-        self.modifiers = tuple(self.modifiers)
-    
-    def modify(self, date: datetime) -> datetime:
-        for modifier in self.modifiers:
-            date = modifier.modify(date)
-        return date
-
-
-@dataclass
-class _DateRepresentationModifier:
-    """
-    Abstract class for modifying other representations of dates (such as string or unix timestemp)
-    """
-    def __init__(self, date_modifiers: Sequence[DateModifier]):
-        self.date_modifier = DateModPipeline(date_modifiers)
-    
-    def _get_joined_modifiers(self, date_modifiers: Sequence[DateModifier]) -> Sequence[DateModifier]:
-        joined_modifiers = self.date_modifier.modifiers + tuple(date_modifiers)
-        return joined_modifiers
-
-    def with_more_modifiers(self, date_modifiers: Sequence[DateModifier]):
-        raise _utils.AbstractMethodCallError(self.__class__, "with_more_modifiers")
-    
-    def get_date_list(self, curr_date: datetime, step: DateModifier) -> Sequence[datetime]:
-        modified_date = self.date_modifier.modify(curr_date)
-        curr_date, end_date = min(curr_date, modified_date), max(curr_date, modified_date)
-        distance = None
-        output = []
-        while curr_date <= end_date:
-            if distance is not None and (end_date - curr_date) >= distance:
-                raise _utils.ConfigurationError("The step must increment forward in time")
-            distance = end_date - curr_date
-            output.append(curr_date)
-            curr_date = step.modify(curr_date)
-        return output
-
-
-@dataclass
-class DateStringModifier(_DateRepresentationModifier):
-    """
-    Class to modify a string representation of a date given a DateModifier
-
-    Attributes:
-        date_modifier: The DateModifier to apply on datetime objects
-        date_format: Format of the output date string. Default is '%Y-%m-%d'
-    """
-    def __init__(self, date_modifiers: Sequence[DateModifier], date_format: str = '%Y-%m-%d'):
-        super().__init__(date_modifiers)
-        self.date_format = date_format
-
-    def with_more_modifiers(self, date_modifiers: Sequence[DateModifier]):
-        """
-        Create a new DateStringModifier with more date modifiers
-
-        Parameters:
-            date_modifiers: The additional date modifiers to add
-
-        Returns:
-            A new DateStringModifier
-        """
-        joined_modifiers = self._get_joined_modifiers(date_modifiers)
-        return DateStringModifier(joined_modifiers, self.date_format)
-    
-    def _get_input_date_obj(self, date_str: str, input_format: str = None) -> datetime:
-        input_format = self.date_format if input_format is None else input_format
-        return datetime.strptime(date_str, input_format)
-
-    def modify(self, date_str: str, input_format: str = None) -> str:
-        """
-        Modifies the input date string with the date modifiers
-
-        Parameters:
-            date_str: The input date string
-            input_format: The input date format. Defaults to the same as output date format
-        
-        Returns:
-            The resulting date string
-        """
-        date_obj = self._get_input_date_obj(date_str, input_format)
-        return self.date_modifier.modify(date_obj).strftime(self.date_format)
-    
-    def get_date_list(self, date_str: str, step: DateModifier, input_format: str = None) -> Sequence[str]:
-        """
-        This method modifies the input date string, and returns all dates from the earlier to later date, 
-        incremented by a DateModifier step, until the last date is less than or equal to the later date.
-
-        Parameters:
-            date_str: The input date string, usually the first date in the output list
-            step: The increment to take (specified as a DateModifier). It must increment forward in time
-            input_format: The input date format. Defaults to the same as output date format
-
-        Returns:
-            A list of date strings
-        """
-        curr_date = self._get_input_date_obj(date_str, input_format)
-        output = super().get_date_list(curr_date, step)
-        return [x.strftime(self.date_format) for x in output]
-
-
-@dataclass
-class TimestampModifier(_DateRepresentationModifier):
-    """
-    Class to modify a numeric representation of a date (as Unix/Epoch/POSIX timestamp) given a DateModifier
-
-    Attributes:
-        date_modifier: The DateModifier to apply on datetime objects
-        date_format: Format of the date string. Default is '%Y-%m-%d'
-    """
-    def __init__(self, date_modifiers: Sequence[DateModifier]):
-        super().__init__(date_modifiers)
-
-    def with_more_modifiers(self, date_modifiers: Sequence[DateModifier]):
-        """
-        Create a new TimestampModifier with more date modifiers
-
-        Parameters:
-            date_modifiers: The additional date modifiers to add
-
-        Returns:
-            A new TimestampModifier
-        """
-        joined_modifiers = self._get_joined_modifiers(date_modifiers)
-        return TimestampModifier(joined_modifiers)
-
-    def modify(self, timestamp: float) -> float:
-        """
-        Modifies the input timestamp with the date modifiers
-
-        Parameters:
-            timestamp: The input timestamp as float
-        
-        Returns:
-            The resulting timestamp
-        """
-        date_obj = datetime.fromtimestamp(timestamp)
-        return self.date_modifier.modify(date_obj).timestamp()
-    
-    def get_date_list(self, timestamp: float, step: DateModifier) -> Sequence[float]:
-        """
-        This method modifies the input date string, and returns all dates from the earlier to later date, 
-        incremented by a DateModifier step, until the last date is less than or equal to the later date.
-
-        Parameters:
-            timestamp: The input timestamp as float, usually the first date in the output list
-            step: The increment to take (specified as a DateModifier). It must increment forward in time
-
-        Returns:
-            A list of timestamp as floats
-        """
-        curr_date = datetime.fromtimestamp(timestamp)
-        output = super().get_date_list(curr_date, step)
-        return [x.timestamp() for x in output]
+from typing import Sequence
+from dataclasses import dataclass
+from datetime import datetime
+from dateutil.relativedelta import relativedelta
+from enum import Enum
+
+from squirrels import _utils
+
+
+class DayOfWeek(Enum):
+    Sunday = 0
+    Monday = 1
+    Tuesday = 2
+    Wednesday = 3
+    Thursday = 4
+    Friday = 5
+    Saturday = 6
+
+class Month(Enum):
+    January = 1
+    February = 2
+    March = 3
+    April = 4
+    May = 5
+    June = 6
+    July = 7
+    August = 8
+    September = 9
+    October = 10
+    November = 11
+    December = 12
+
+
+@dataclass
+class DateModifier:
+    """
+    Interface for all Date modification classes, and declares a "modify" method
+    """
+
+    def modify(self, date: datetime) -> datetime:
+        """
+        Method to be overwritten, modifies the input date
+
+        Parameters:
+            date: The input date to modify.
+
+        Returns:
+            The modified date.
+        """
+        raise _utils.AbstractMethodCallError(self.__class__, "modify")
+
+
+@dataclass
+class _DayIdxOfCalendarUnit(DateModifier):
+    """
+    Interface for adjusting a date to some day of calendar unit
+    """
+    idx: int
+
+    def __post_init__(self):
+        if self.idx == 0:
+            raise _utils.ConfigurationError("For constructors of class names that start with DayIdxOf_, idx cannot be zero")
+        self.incr = self.idx - 1 if self.idx > 0 else self.idx
+
+
+@dataclass
+class DayIdxOfMonthsCycle(_DayIdxOfCalendarUnit):
+    """
+    DateModifier class to get the idx-th day of a cycle of months for an input date
+
+    Attributes:
+        idx: 1 for first, 2 for second, etc. Or, -1 for last, -2 for second last, etc. Must not be 0
+        num_months_in_cycle: 2 for one 6th of year, 3 for Quarter, 4 for one 3rd of year, 6 for half year, 12 for full year. Must fit evenly in 12
+        first_month_of_cycle: The first month of months cycle of year. Default is January
+    """
+    num_months_in_cycle: int
+    first_month_of_cycle: Month = Month.January
+
+    def __post_init__(self):
+        super().__post_init__()
+        if 12 % self.num_months_in_cycle != 0:
+            raise _utils.ConfigurationError("Value X must fit evenly in 12")
+        self.first_month_of_first_cycle = (self.first_month_of_cycle.value - 1) % self.num_months_in_cycle + 1
+
+    def modify(self, date: datetime) -> datetime:
+        current_cycle = (date.month - self.first_month_of_first_cycle) % 12 // self.num_months_in_cycle
+        first_month_of_curr_cycle = current_cycle * self.num_months_in_cycle + self.first_month_of_first_cycle
+        year = date.year if date.month >= first_month_of_curr_cycle else date.year - 1
+        first_day = datetime(year, first_month_of_curr_cycle, 1)
+        ref_date = first_day if self.idx > 0 else first_day + relativedelta(months=self.num_months_in_cycle)
+        return ref_date + relativedelta(days=self.incr)
+
+
+@dataclass
+class DayIdxOfYear(DayIdxOfMonthsCycle):
+    """
+    DateModifier class to get the idx-th day of year of an input date
+
+    Attributes:
+        idx: 1 for first, 2 for second, etc. Or, -1 for last, -2 for second last, etc. Must not be 0
+        first_month_of_year: The first month of year. Default is January
+    """
+
+    def __init__(self, idx: int, first_month_of_year: Month = Month.January):
+        super().__init__(idx, num_months_in_cycle=12, first_month_of_cycle=first_month_of_year)
+
+
+@dataclass
+class DayIdxOfQuarter(DayIdxOfMonthsCycle):
+    """
+    DateModifier class to get the idx-th day of quarter of an input date
+
+    Attributes:
+        idx: 1 for first, 2 for second, etc. Or, -1 for last, -2 for second last, etc. Must not be 0
+        first_month_of_quarter: The first month of first quarter. Default is January
+    """
+
+    def __init__(self, idx: int, first_month_of_quarter: Month = Month.January):
+        super().__init__(idx, num_months_in_cycle=3, first_month_of_cycle=first_month_of_quarter)
+
+
+@dataclass
+class DayIdxOfMonth(_DayIdxOfCalendarUnit):
+    """
+    DateModifier class to get the idx-th day of month of an input date
+
+    Attributes:
+        idx: 1 for first, 2 for second, etc. Or, -1 for last, -2 for second last, etc. Must not be 0
+    """
+
+    def modify(self, date: datetime) -> datetime:
+        first_day = datetime(date.year, date.month, 1)
+        ref_date = first_day if self.idx > 0 else first_day + relativedelta(months=1)
+        return ref_date + relativedelta(days=self.incr)
+
+
+@dataclass
+class DayIdxOfWeek(_DayIdxOfCalendarUnit):
+    """
+    DateModifier class to get the idx-th day of week of an input date
+
+    Attributes:
+        idx: 1 for first, 2 for second, etc. Or, -1 for last, -2 for second last, etc. Must not be 0
+        first_day_of_week: The day of week identified as the "first". Default is Monday
+    """
+    first_day_of_week: DayOfWeek = DayOfWeek.Monday
+
+    def __post_init__(self):
+        super().__post_init__()
+        self.first_dow_num = self.first_day_of_week.value
+    
+    def modify(self, date: datetime) -> datetime:
+        distance_from_first_day = (1 + date.weekday() - self.first_dow_num) % 7
+        total_incr = -distance_from_first_day + (7 if self.idx < 0 else 0) + self.incr
+        return date + relativedelta(days=total_incr)
+
+
+@dataclass
+class _OffsetUnits(DateModifier):
+    """
+    Abstract DateModifier class to offset an input date by some number of some calendar unit
+    """
+    offset: int
+
+
+@dataclass
+class OffsetYears(_OffsetUnits):
+    """
+    DateModifier class to offset an input date by some number of years
+
+    Attributes:
+        offset: The number of years to offset the input date.
+    """
+
+    def modify(self, date: datetime) -> datetime:
+        return date + relativedelta(years=self.offset)
+    
+
+@dataclass
+class OffsetMonths(_OffsetUnits):
+    """
+    DateModifier class to offset an input date by some number of months
+
+    Attributes:
+        offset: The number of months to offset the input date.
+    """
+
+    def modify(self, date: datetime) -> datetime:
+        return date + relativedelta(months=self.offset)
+
+
+@dataclass
+class OffsetWeeks(_OffsetUnits):
+    """
+    DateModifier class to offset an input date by some number of weeks
+
+    Attributes:
+        offset: The number of weeks to offset the input date.
+    """
+
+    def modify(self, date: datetime) -> datetime:
+        return date + relativedelta(weeks=self.offset)
+
+
+@dataclass
+class OffsetDays(_OffsetUnits):
+    """
+    DateModifier class to offset an input date by some number of days
+
+    Attributes:
+        offset: The number of days to offset the input date.
+    """
+
+    def modify(self, date: datetime) -> datetime:
+        return date + relativedelta(days=self.offset)
+
+
+@dataclass
+class DateModPipeline(DateModifier):
+    """
+    DateModifier class to apply a list of date modifiers to an input date
+
+    Attributes:
+        modifiers: The list of DateModifier's to apply in sequence.
+    """
+    date_modifiers: Sequence[DateModifier]
+
+    def __post_init__(self):
+        self.date_modifiers = tuple(self.date_modifiers)
+    
+    def modify(self, date: datetime) -> datetime:
+        for modifier in self.date_modifiers:
+            date = modifier.modify(date)
+        return date
+    
+    def get_joined_modifiers(self, date_modifiers: Sequence[DateModifier]) -> Sequence[DateModifier]:
+        """
+        Create a new sequence of DateModifier by joining the date modifiers in this class 
+        with the input date_modifiers
+
+        Parameters:
+            date_modifiers: The new date modifier sequence to join
+
+        Returns:
+            A new sequence of DateModifier
+        """
+        joined_modifiers = self.date_modifiers + tuple(date_modifiers)
+        return joined_modifiers
+
+    def with_more_modifiers(self, date_modifiers: Sequence[DateModifier]):
+        """
+        Create a new DateModPipeline with more date modifiers
+
+        Parameters:
+            date_modifiers: The additional date modifiers to add
+
+        Returns:
+            A new DateModPipeline
+        """
+        joined_modifiers = self.get_joined_modifiers(date_modifiers)
+        return DateModPipeline(joined_modifiers)
+    
+    def get_date_list(self, start_date: datetime, step: _OffsetUnits) -> Sequence[datetime]:
+        """
+        This method modifies the input date, and returns all dates from the input date to the modified date, 
+        incremented by a DateModifier step.
+
+        If the step is positive and start date is less than end date, then it'll return an increasing list of
+        dates starting from the start date. If the step is positive and start date is less than end date, 
+        then it'll return a decreasing list of dates starting from the start date. Otherwise, an empty list
+        is returned.
+
+        Parameters:
+            start_date: The input date (it's the first date in the output list if step moves towards end date)
+            step: The increment to take (specified as an offset DateModifier). Offset cannot be zero
+
+        Returns:
+            A list of datetime objects
+        """
+        if step.offset == 0:
+            raise _utils.ConfigurationError("The length of 'step' must not be zero")
+        
+        output = []
+        end_date = self.modify(start_date)
+        curr_date = start_date
+        is_not_done_positive_step = lambda: curr_date <= end_date and step.offset > 0
+        is_not_done_negative_step = lambda: curr_date >= end_date and step.offset < 0
+        while is_not_done_positive_step() or is_not_done_negative_step():
+            output.append(curr_date)
+            curr_date = step.modify(curr_date)
+        return output
+
+
+@dataclass
+class _DateRepresentationModifier:
+    """
+    Abstract class for modifying other representations of dates (such as string or unix timestemp)
+    """
+    def __init__(self, date_modifiers: Sequence[DateModifier]):
+        self.date_modifier = DateModPipeline(date_modifiers)
+
+    def with_more_modifiers(self, date_modifiers: Sequence[DateModifier]):
+        raise _utils.AbstractMethodCallError(self.__class__, "with_more_modifiers")
+
+
+@dataclass
+class DateStringModifier(_DateRepresentationModifier):
+    """
+    Class to modify a string representation of a date given a DateModifier
+
+    Attributes:
+        date_modifier: The DateModifier to apply on datetime objects
+        date_format: Format of the output date string. Default is '%Y-%m-%d'
+    """
+    def __init__(self, date_modifiers: Sequence[DateModifier], date_format: str = '%Y-%m-%d'):
+        super().__init__(date_modifiers)
+        self.date_format = date_format
+
+    def with_more_modifiers(self, date_modifiers: Sequence[DateModifier]):
+        """
+        Create a new DateStringModifier with more date modifiers
+
+        Parameters:
+            date_modifiers: The additional date modifiers to add
+
+        Returns:
+            A new DateStringModifier
+        """
+        joined_modifiers = self.date_modifier.get_joined_modifiers(date_modifiers)
+        return DateStringModifier(joined_modifiers, self.date_format)
+    
+    def _get_input_date_obj(self, date_str: str, input_format: str = None) -> datetime:
+        input_format = self.date_format if input_format is None else input_format
+        return datetime.strptime(date_str, input_format)
+
+    def modify(self, date_str: str, input_format: str = None) -> str:
+        """
+        Modifies the input date string with the date modifiers
+
+        Parameters:
+            date_str: The input date string
+            input_format: The input date format. Defaults to the same as output date format
+        
+        Returns:
+            The resulting date string
+        """
+        date_obj = self._get_input_date_obj(date_str, input_format)
+        return self.date_modifier.modify(date_obj).strftime(self.date_format)
+    
+    def get_date_list(self, start_date_str: str, step: DateModifier, input_format: str = None) -> Sequence[str]:
+        """
+        This method modifies the input date string, and returns all dates as strings from the input date 
+        to the modified date, incremented by a DateModifier step.
+
+        If the step is positive and start date is less than end date, then it'll return an increasing list of
+        dates starting from the start date. If the step is positive and start date is less than end date, 
+        then it'll return a decreasing list of dates starting from the start date. Otherwise, an empty list
+        is returned.
+
+        Parameters:
+            start_date_str: The input date string (it's the first date in the output list if step moves towards end date)
+            step: The increment to take (specified as an offset DateModifier). Offset cannot be zero
+            input_format: The input date format. Defaults to the same as output date format
+
+        Returns:
+            A list of date strings
+        """
+        curr_date = self._get_input_date_obj(start_date_str, input_format)
+        output = self.date_modifier.get_date_list(curr_date, step)
+        return [x.strftime(self.date_format) for x in output]
+
+
+@dataclass
+class TimestampModifier(_DateRepresentationModifier):
+    """
+    Class to modify a numeric representation of a date (as Unix/Epoch/POSIX timestamp) given a DateModifier
+
+    Attributes:
+        date_modifier: The DateModifier to apply on datetime objects
+        date_format: Format of the date string. Default is '%Y-%m-%d'
+    """
+    def __init__(self, date_modifiers: Sequence[DateModifier]):
+        super().__init__(date_modifiers)
+
+    def with_more_modifiers(self, date_modifiers: Sequence[DateModifier]):
+        """
+        Create a new TimestampModifier with more date modifiers
+
+        Parameters:
+            date_modifiers: The additional date modifiers to add
+
+        Returns:
+            A new TimestampModifier
+        """
+        joined_modifiers = self.date_modifier.get_joined_modifiers(date_modifiers)
+        return TimestampModifier(joined_modifiers)
+
+    def modify(self, timestamp: float) -> float:
+        """
+        Modifies the input timestamp with the date modifiers
+
+        Parameters:
+            timestamp: The input timestamp as float
+        
+        Returns:
+            The resulting timestamp
+        """
+        date_obj = datetime.fromtimestamp(timestamp)
+        return self.date_modifier.modify(date_obj).timestamp()
+    
+    def get_date_list(self, start_timestamp: float, step: DateModifier) -> Sequence[float]:
+        """
+        This method modifies the input timestamp, and returns all dates as timestampes/floats from the input date 
+        to the modified date, incremented by a DateModifier step.
+
+        If the step is positive and start date is less than end date, then it'll return an increasing list of
+        dates starting from the start date. If the step is positive and start date is less than end date, 
+        then it'll return a decreasing list of dates starting from the start date. Otherwise, an empty list
+        is returned.
+
+        Parameters:
+            start_timestamp: The input timestamp as float (it's the first date in the output list if step moves towards end date)
+            step: The increment to take (specified as an offset DateModifier). Offset cannot be zero
+
+        Returns:
+            A list of timestamp as floats
+        """
+        curr_date = datetime.fromtimestamp(start_timestamp)
+        output = self.date_modifier.get_date_list(curr_date, step)
+        return [x.timestamp() for x in output]
```

### Comparing `squirrels-0.1.0/squirrels/package_data/base_project/connections.py` & `squirrels-0.1.1.post1/squirrels/package_data/base_project/connections.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,20 @@
-from typing import Dict, Union, Any
-from sqlalchemy import create_engine, Engine, Pool, QueuePool
-
-from squirrels import get_credential
-
-
-# Note: all connections must be shareable across multiple thread. No writes will occur on them
-def main(proj: Dict[str, Any], *p_args, **kwargs) -> Dict[str, Union[Engine, Pool]]:
-
-    # ## Example of getting the username and password set with "$ squirrels set-credential [key]"
-    # cred = get_credential('my_key')
-    # # Use cred.username and cred.password to access the username and password
-
-    # Create a connection pool / engine
-    pool = create_engine('sqlite:///./database/sample_database.db')
-
-    # ## Example of using QueuePool instead for a custom db connector:
-    # connection_creator = lambda: sqlite3.connect('./database/sample_database.db', check_same_thread=False)
-    # pool = QueuePool(connection_creator)
-    
-    return {'default': pool}
+from typing import Dict, Union, Any
+from sqlalchemy import create_engine, Engine, Pool, QueuePool
+
+from squirrels import get_credential
+
+
+# Note: all connections must be shareable across multiple thread. No writes will occur on them
+def main(proj: Dict[str, Any], *p_args, **kwargs) -> Dict[str, Union[Engine, Pool]]:
+
+    ## Example of getting the username and password set with "$ squirrels set-credential [key]"
+    # cred = get_credential('my_key') # then use cred.username and cred.password to access the username and password
+
+    # Create a connection pool / engine
+    pool = create_engine('sqlite:///./database/sample_database.db')
+
+    ## Example of using QueuePool instead for a custom db connector:
+    # connection_creator = lambda: sqlite3.connect('./database/sample_database.db', check_same_thread=False)
+    # pool = QueuePool(connection_creator)
+    
+    return {'default': pool}
```

### Comparing `squirrels-0.1.0/squirrels/package_data/base_project/database/seattle_weather.db` & `squirrels-0.1.1.post1/squirrels/package_data/base_project/database/seattle_weather.db`

 * *Files identical despite different names*

### Comparing `squirrels-0.1.0/squirrels/package_data/static/favicon.ico` & `squirrels-0.1.1.post1/squirrels/package_data/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `squirrels-0.1.0/squirrels/package_data/static/script.js` & `squirrels-0.1.1.post1/squirrels/package_data/static/script.js`

 * *Files 12% similar despite different names*

#### js-beautify {}

```diff
@@ -1,234 +1,234 @@
-const datasetSelect = document.getElementById('dataset-select');
-const generatedParamsDiv = document.getElementById('generated-parameters');
-
-const tableContainers = document.getElementById('table-container');
-const resultTable = document.getElementById("result-table");
-const tableHeader = document.getElementById('table-header');
-const tableBody = document.getElementById('table-body');
-
-const loadingIndicator = document.getElementById('loading-indicator');
-
-const datasetsMap = new Map();
-const parametersMap = new Map();
-
-function callJsonAPI(path, func) {
-    loadingIndicator.style.display = 'flex';
-    fetch(path)
-        .then(response => response.json())
-        .then(data => {
-            func(data);
-        })
-        .catch(error => {
-            alert('Server error...')
-            console.log(error)
-        })
-        .then(_ => {
-            loadingIndicator.style.display = 'none'
-        })
-}
-
-function changeDatasetSelection() {
-    tableContainers.style.display = 'none';
-    parametersMap.clear()
-    refreshParameters();
-}
-
-function renderDatasetsSelection(data) {
-    const datasets = data.products[0].versions[0].datasets
-    datasets.forEach(resource => {
-        const option = document.createElement('option');
-        option.value = resource.name;
-        option.textContent = resource.label;
-        datasetSelect.appendChild(option);
-        datasetsMap.set(option.value, resource);
-    });
-    changeDatasetSelection();
-}
-
-function refreshParameters(provoker = null) {
-    const selectedDatasetValue = datasetSelect.value;
-    const parametersPath = datasetsMap.get(selectedDatasetValue).parameters_path;
-    const queryParameters = getQueryParams(provoker)
-    const parametersRequest = parametersPath + '?' + queryParameters
-    console.log('Parameters request:', parametersRequest)
-
-    callJsonAPI(parametersRequest, (jsonResponse) => {
-        jsonResponse.parameters.forEach(function(param) {
-            parametersMap.set(param.name, param);
-        })
-        generatedParamsDiv.innerHTML = "";
-        for (const param of parametersMap.values()) {
-            const newDiv = document.createElement('div')
-
-            const addLabel = function() {
-                const paramLabel = document.createElement('label')
-                paramLabel.innerHTML = param.label
-                newDiv.appendChild(paramLabel)
-            }
-
-            if (param.widget_type === "DateParameter") {
-                addLabel()
-                const dateInput = document.createElement('input')
-                dateInput.type = 'date'
-                dateInput.id = param.name
-                dateInput.value = param.selected_date
-                dateInput.onchange = updateParameter
-                newDiv.appendChild(dateInput)
-            } else if (param.widget_type === "NumberParameter") {
-                addLabel()
-                const sliderInput = document.createElement('input')
-                sliderInput.type = 'range'
-                sliderInput.id = param.name
-                sliderInput.min = param.min_value
-                sliderInput.max = param.max_value
-                sliderInput.step = param.increment
-                sliderInput.value = param.selected_value
-
-                const sliderValue = document.createElement('div')
-                sliderValue.id = param.name + '_value'
-                sliderValue.className = 'slider-value'
-                sliderValue.innerText = param.selected_value
-
-                sliderInput.oninput = function() {
-                    sliderValue.innerText = this.value;
-                }
-                sliderInput.onchange = updateParameter
-
-                newDiv.appendChild(sliderInput)
-                newDiv.appendChild(sliderValue)
-            } else if (param.widget_type === "NumRangeParameter") {
-                // TODO
-            } else if (param.widget_type === "SingleSelectParameter" && param.options.length > 0) {
-                addLabel()
-                const singleSelect = document.createElement('select');
-                singleSelect.id = param.name;
-                param.options.forEach(function(option) {
-                    const selectOption = document.createElement('option');
-                    selectOption.value = option.id;
-                    if (option.id === param.selected_id) {
-                        selectOption.selected = true;
-                    }
-                    selectOption.innerText = option.label;
-                    singleSelect.appendChild(selectOption);
-                });
-                singleSelect.onchange = updateParameter
-                newDiv.appendChild(singleSelect);
-            } else if (param.widget_type === "MultiSelectParameter" && param.options.length > 0) {
-                addLabel()
-                const multiSelect = document.createElement('select');
-                multiSelect.id = param.name;
-                multiSelect.multiple = true;
-                param.options.forEach(function(option) {
-                    const selectOption = document.createElement('option');
-                    selectOption.value = option.id;
-                    if (param.selected_ids.includes(option.id)) {
-                        selectOption.selected = true;
-                    }
-                    selectOption.innerText = option.label;
-                    multiSelect.appendChild(selectOption);
-                });
-                multiSelect.onchange = updateParameter
-                newDiv.appendChild(multiSelect);
-            }
-            generatedParamsDiv.appendChild(newDiv);
-        }
-    });
-}
-
-function updateParameter() {
-    const param = parametersMap.get(this.id)
-    if (param.widget_type === "DateParameter") {
-        param.selected_date = this.value
-    } else if (param.widget_type === "NumberParameter") {
-        param.selected_value = this.value
-    } else if (param.widget_type === "NumRangeParameter") {
-        // TODO
-    } else if (param.widget_type === "SingleSelectParameter") {
-        param.selected_id = this.options[this.selectedIndex].value
-    } else if (param.widget_type === "MultiSelectParameter") {
-        param.selected_ids = [...this.selectedOptions].map(option => option.value)
-    }
-
-    if (param.trigger_refresh) {
-        refreshParameters(param)
-    }
-}
-
-function getQueryParams(provoker = null) {
-    const queryParams = {}
-
-    function addToQueryParams(key, value) {
-        if (value.widget_type === "DateParameter") {
-            queryParams[key] = value.selected_date
-        } else if (value.widget_type === "NumberParameter") {
-            queryParams[key] = value.selected_value
-        } else if (value.widget_type === "NumRangeParameter") {
-            // TODO
-        } else if (value.widget_type === "SingleSelectParameter") {
-            queryParams[key] = value.selected_id
-        } else if (value.widget_type === "MultiSelectParameter") {
-            result = JSON.stringify(value.selected_ids)
-            if (result !== '') queryParams[key] = result
-        }
-    }
-    if (provoker !== null) {
-        addToQueryParams(provoker.name, provoker)
-    } else {
-        for (const [key, value] of parametersMap.entries()) {
-            addToQueryParams(key, value)
-        }
-    }
-    console.log(queryParams)
-    return new URLSearchParams(queryParams)
-}
-
-function getDatasetResults() {
-    const selectedDatasetValue = datasetSelect.value;
-    const resultPath = datasetsMap.get(selectedDatasetValue).result_path;
-    const resultRequest = resultPath + '?' + getQueryParams()
-    console.log('Result request:', resultRequest)
-
-    callJsonAPI(resultRequest, (jsonResponse) => {
-        tableHeader.innerHTML = ''
-        tableBody.innerHTML = ''
-
-        // Create the table header row
-        const headerRow = document.createElement('tr');
-        jsonResponse.schema.fields.forEach(field => {
-            const th = document.createElement('th');
-            th.textContent = field.name;
-            headerRow.appendChild(th);
-        });
-        tableHeader.appendChild(headerRow);
-
-        // Create the table data rows
-        jsonResponse.data.forEach(dataObject => {
-            const row = document.createElement('tr');
-            jsonResponse.schema.fields.forEach(field => {
-                const td = document.createElement('td');
-                td.textContent = dataObject[field.name];
-                row.appendChild(td);
-            });
-            tableBody.appendChild(row);
-        });
-
-        tableContainers.style.display = 'block'
-    });
-}
-
-function copyTable() {
-    let text = "";
-
-    for (let i = 0; i < resultTable.rows.length; i++) {
-        for (let j = 0; j < resultTable.rows[i].cells.length; j++) {
-            text += resultTable.rows[i].cells[j].innerHTML + "\t";
-        }
-        text += "\n";
-    }
-
-    navigator.clipboard.writeText(text).then(function() {
-        alert("Table copied to clipboard!");
-    }, function() {
-        alert("Copying failed.");
-    });
+const datasetSelect = document.getElementById('dataset-select');
+const generatedParamsDiv = document.getElementById('generated-parameters');
+
+const tableContainers = document.getElementById('table-container');
+const resultTable = document.getElementById("result-table");
+const tableHeader = document.getElementById('table-header');
+const tableBody = document.getElementById('table-body');
+
+const loadingIndicator = document.getElementById('loading-indicator');
+
+const datasetsMap = new Map();
+const parametersMap = new Map();
+
+function callJsonAPI(path, func) {
+    loadingIndicator.style.display = 'flex';
+    fetch(path)
+        .then(response => response.json())
+        .then(data => {
+            func(data);
+        })
+        .catch(error => {
+            alert('Server error...')
+            console.log(error)
+        })
+        .then(_ => {
+            loadingIndicator.style.display = 'none'
+        })
+}
+
+function changeDatasetSelection() {
+    tableContainers.style.display = 'none';
+    parametersMap.clear()
+    refreshParameters();
+}
+
+function renderDatasetsSelection(data) {
+    const datasets = data.products[0].versions[0].datasets
+    datasets.forEach(resource => {
+        const option = document.createElement('option');
+        option.value = resource.name;
+        option.textContent = resource.label;
+        datasetSelect.appendChild(option);
+        datasetsMap.set(option.value, resource);
+    });
+    changeDatasetSelection();
+}
+
+function refreshParameters(provoker = null) {
+    const selectedDatasetValue = datasetSelect.value;
+    const parametersPath = datasetsMap.get(selectedDatasetValue).parameters_path;
+    const queryParameters = getQueryParams(provoker)
+    const parametersRequest = parametersPath + '?' + queryParameters
+    console.log('Parameters request:', parametersRequest)
+
+    callJsonAPI(parametersRequest, (jsonResponse) => {
+        jsonResponse.parameters.forEach(function(param) {
+            parametersMap.set(param.name, param);
+        })
+        generatedParamsDiv.innerHTML = "";
+        for (const param of parametersMap.values()) {
+            const newDiv = document.createElement('div')
+
+            const addLabel = function() {
+                const paramLabel = document.createElement('label')
+                paramLabel.innerHTML = param.label
+                newDiv.appendChild(paramLabel)
+            }
+
+            if (param.widget_type === "DateParameter") {
+                addLabel()
+                const dateInput = document.createElement('input')
+                dateInput.type = 'date'
+                dateInput.id = param.name
+                dateInput.value = param.selected_date
+                dateInput.onchange = updateParameter
+                newDiv.appendChild(dateInput)
+            } else if (param.widget_type === "NumberParameter") {
+                addLabel()
+                const sliderInput = document.createElement('input')
+                sliderInput.type = 'range'
+                sliderInput.id = param.name
+                sliderInput.min = param.min_value
+                sliderInput.max = param.max_value
+                sliderInput.step = param.increment
+                sliderInput.value = param.selected_value
+
+                const sliderValue = document.createElement('div')
+                sliderValue.id = param.name + '_value'
+                sliderValue.className = 'slider-value'
+                sliderValue.innerText = param.selected_value
+
+                sliderInput.oninput = function() {
+                    sliderValue.innerText = this.value;
+                }
+                sliderInput.onchange = updateParameter
+
+                newDiv.appendChild(sliderInput)
+                newDiv.appendChild(sliderValue)
+            } else if (param.widget_type === "NumRangeParameter") {
+                // TODO
+            } else if (param.widget_type === "SingleSelectParameter" && param.options.length > 0) {
+                addLabel()
+                const singleSelect = document.createElement('select');
+                singleSelect.id = param.name;
+                param.options.forEach(function(option) {
+                    const selectOption = document.createElement('option');
+                    selectOption.value = option.id;
+                    if (option.id === param.selected_id) {
+                        selectOption.selected = true;
+                    }
+                    selectOption.innerText = option.label;
+                    singleSelect.appendChild(selectOption);
+                });
+                singleSelect.onchange = updateParameter
+                newDiv.appendChild(singleSelect);
+            } else if (param.widget_type === "MultiSelectParameter" && param.options.length > 0) {
+                addLabel()
+                const multiSelect = document.createElement('select');
+                multiSelect.id = param.name;
+                multiSelect.multiple = true;
+                param.options.forEach(function(option) {
+                    const selectOption = document.createElement('option');
+                    selectOption.value = option.id;
+                    if (param.selected_ids.includes(option.id)) {
+                        selectOption.selected = true;
+                    }
+                    selectOption.innerText = option.label;
+                    multiSelect.appendChild(selectOption);
+                });
+                multiSelect.onchange = updateParameter
+                newDiv.appendChild(multiSelect);
+            }
+            generatedParamsDiv.appendChild(newDiv);
+        }
+    });
+}
+
+function updateParameter() {
+    const param = parametersMap.get(this.id)
+    if (param.widget_type === "DateParameter") {
+        param.selected_date = this.value
+    } else if (param.widget_type === "NumberParameter") {
+        param.selected_value = this.value
+    } else if (param.widget_type === "NumRangeParameter") {
+        // TODO
+    } else if (param.widget_type === "SingleSelectParameter") {
+        param.selected_id = this.options[this.selectedIndex].value
+    } else if (param.widget_type === "MultiSelectParameter") {
+        param.selected_ids = [...this.selectedOptions].map(option => option.value)
+    }
+
+    if (param.trigger_refresh) {
+        refreshParameters(param)
+    }
+}
+
+function getQueryParams(provoker = null) {
+    const queryParams = {}
+
+    function addToQueryParams(key, value) {
+        if (value.widget_type === "DateParameter") {
+            queryParams[key] = value.selected_date
+        } else if (value.widget_type === "NumberParameter") {
+            queryParams[key] = value.selected_value
+        } else if (value.widget_type === "NumRangeParameter") {
+            // TODO
+        } else if (value.widget_type === "SingleSelectParameter") {
+            queryParams[key] = value.selected_id
+        } else if (value.widget_type === "MultiSelectParameter") {
+            result = JSON.stringify(value.selected_ids)
+            if (result !== '') queryParams[key] = result
+        }
+    }
+    if (provoker !== null) {
+        addToQueryParams(provoker.name, provoker)
+    } else {
+        for (const [key, value] of parametersMap.entries()) {
+            addToQueryParams(key, value)
+        }
+    }
+    console.log(queryParams)
+    return new URLSearchParams(queryParams)
+}
+
+function getDatasetResults() {
+    const selectedDatasetValue = datasetSelect.value;
+    const resultPath = datasetsMap.get(selectedDatasetValue).result_path;
+    const resultRequest = resultPath + '?' + getQueryParams()
+    console.log('Result request:', resultRequest)
+
+    callJsonAPI(resultRequest, (jsonResponse) => {
+        tableHeader.innerHTML = ''
+        tableBody.innerHTML = ''
+
+        // Create the table header row
+        const headerRow = document.createElement('tr');
+        jsonResponse.schema.fields.forEach(field => {
+            const th = document.createElement('th');
+            th.textContent = field.name;
+            headerRow.appendChild(th);
+        });
+        tableHeader.appendChild(headerRow);
+
+        // Create the table data rows
+        jsonResponse.data.forEach(dataObject => {
+            const row = document.createElement('tr');
+            jsonResponse.schema.fields.forEach(field => {
+                const td = document.createElement('td');
+                td.textContent = dataObject[field.name];
+                row.appendChild(td);
+            });
+            tableBody.appendChild(row);
+        });
+
+        tableContainers.style.display = 'block'
+    });
+}
+
+function copyTable() {
+    let text = "";
+
+    for (let i = 0; i < resultTable.rows.length; i++) {
+        for (let j = 0; j < resultTable.rows[i].cells.length; j++) {
+            text += resultTable.rows[i].cells[j].innerHTML + "\t";
+        }
+        text += "\n";
+    }
+
+    navigator.clipboard.writeText(text).then(function() {
+        alert("Table copied to clipboard!");
+    }, function() {
+        alert("Copying failed.");
+    });
 }
```

### Comparing `squirrels-0.1.0/squirrels/package_data/templates/index.html` & `squirrels-0.1.1.post1/squirrels/package_data/templates/index.html`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-<!DOCTYPE html>
-<html>
-    <head>
-        <title>Squirrels UI</title>
-        <link id="favicon" rel="icon" type="image/x-icon" href="static/favicon.ico">
-        <link href="{{ url_for('static', path='/style.css?version=0') }}" rel="stylesheet">
-        <script src="{{ url_for('static', path='/script.js?version=2') }}" defer></script>
-    </head>
-    <body onload="callJsonAPI('{{ catalog_path }}', renderDatasetsSelection)">
-    <div id="main-container">
-        <div id="parameter-container">
-            <label for="dataset-select">Select a Dataset:</label>
-            <select id="dataset-select" onchange="changeDatasetSelection()"></select>
-            <div id="generated-parameters"></div>
-            <input type="submit" value="Apply" onclick="getDatasetResults()">
-        </div>
-        <div id="table-container">
-            <button onclick="copyTable()">Copy Table</button>
-            <table id="result-table">
-                <thead id="table-header"></thead>
-                <tbody id="table-body"></tbody>
-            </table>
-        </div>
-    </div>
-    <div id="loading-indicator">
-        <div>
-            <div class="spinner"></div>
-            <div>Loading...</div>
-        </div>
-    </div>      
-    </body>
+<!DOCTYPE html>
+<html>
+    <head>
+        <title>Squirrels UI</title>
+        <link id="favicon" rel="icon" type="image/x-icon" href="static/favicon.ico">
+        <link href="{{ url_for('static', path='/style.css?version=0') }}" rel="stylesheet">
+        <script src="{{ url_for('static', path='/script.js?version=2') }}" defer></script>
+    </head>
+    <body onload="callJsonAPI('{{ catalog_path }}', renderDatasetsSelection)">
+    <div id="main-container">
+        <div id="parameter-container">
+            <label for="dataset-select">Select a Dataset:</label>
+            <select id="dataset-select" onchange="changeDatasetSelection()"></select>
+            <div id="generated-parameters"></div>
+            <input type="submit" value="Apply" onclick="getDatasetResults()">
+        </div>
+        <div id="table-container">
+            <button onclick="copyTable()">Copy Table</button>
+            <table id="result-table">
+                <thead id="table-header"></thead>
+                <tbody id="table-body"></tbody>
+            </table>
+        </div>
+    </div>
+    <div id="loading-indicator">
+        <div>
+            <div class="spinner"></div>
+            <div>Loading...</div>
+        </div>
+    </div>      
+    </body>
 </html>
```

### Comparing `squirrels-0.1.0/squirrels/parameters.py` & `squirrels-0.1.1.post1/squirrels/parameters.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,801 +1,826 @@
-from __future__ import annotations
-from typing import Type, Sequence, Dict, List, Iterator, Optional, Union
-from dataclasses import dataclass
-from datetime import datetime
-from decimal import Decimal
-import copy
-
-from squirrels import parameter_options as po, _utils as u
-from squirrels.data_sources import DataSource
-from squirrels._parameter_set import ParameterSetBase
-from squirrels._timed_imports import pandas as pd
-
-
-@dataclass
-class Parameter:
-    """
-    Abstract class for all parameter classes. Useful for type hints.
-    """
-    widget_type: str
-    name: str
-    label: str
-    all_options: Sequence[po.ParameterOption]
-    is_hidden: bool
-    parent: Optional[_SelectionParameter]
-
-    def WithParent(all_options: Sequence[po.ParameterOption], parent: SingleSelectParameter, new_param: Parameter):
-        """
-        Helper class method to assign a SingleSelectParameter as the parent for another parameter
-
-        Parameters:
-            all_options: The list of options with one of "parent_option_id" or "parent_option_ids" attribute set.
-            parent: The parent parameter. All option ids of the parent must exist at least once in "parent_option_ids" of all_options
-            new_param: The child parameter to modify. Usually not a selection parameter
-        """
-        new_param._set_parent_and_options(parent, all_options)
-        new_param.parent._add_child_mutate(new_param)
-        return new_param.refresh(parent)
-
-    def refresh(self, parent: Optional[_SelectionParameter] = None) -> Parameter:
-        """
-        Refreshes the selectable options (or change of default value) based on the selection of the parent parameter
-
-        Parameters:
-            parent: The parent parameter subscribed to for updates
-        
-        Returns:
-            A copy of self for the new selectable options based on current selection of parent
-        """
-        param_copy = copy.copy(self)
-        if parent is not None:
-            param_copy.parent = parent
-        param_copy._refresh_mutate()
-        return param_copy
-
-    def with_selection(self, _: str) -> Parameter:
-        """
-        Abstract method for applying the selection to the parameter
-        """
-        raise u.AbstractMethodCallError(self.__class__, "with_selection")
-    
-    def get_all_dependent_params(self) -> ParameterSetBase:
-        """
-        Gets the collection of descendent parameters with changes applied based on the selection of this parameter
-
-        Returns:
-            A collection of descendent parameters as a ParameterSetBase
-        """
-        dependent_params = ParameterSetBase()
-        self._accum_all_dependent_params(dependent_params)
-        return dependent_params
-    
-    def _set_default_as_selection_mutate(self) -> None:
-        raise u.AbstractMethodCallError(self.__class__, "_set_default_as_selection_mutate")
-    
-    def _refresh_mutate(self) -> None:
-        if self.parent is not None and hasattr(self, 'curr_option'):
-            self.curr_option = next(self._get_valid_options_iterator())
-        self._set_default_as_selection_mutate()
-    
-    def _get_valid_options_iterator(self) -> Iterator[po.ParameterOption]:
-        selected_parent_option_ids = self.parent._get_selected_ids_as_list()
-        return (x for x in self.all_options if x.is_valid(selected_parent_option_ids))
-    
-    def _raise_invalid_input_error(self, selection: str, more_details: str = '', e: Exception = None) -> None:
-        raise u.InvalidInputError(f'Selected value "{selection}" is not valid for parameter "{self.name}". ' + more_details) from e
-    
-    def _verify_parent_is_single_select(self) -> None:
-        if not isinstance(self.parent, SingleSelectParameter):
-            raise u.ConfigurationError(f'For "{self.name}", it''s not a selection parameter, so its parent must be a SingleSelectParameter')
-        
-    def _verify_parent_options_have_one_child_each(self) -> None:
-        accum_set = set()
-        for option in self.all_options:
-            if not accum_set.isdisjoint(option.parent_option_ids):
-                raise u.ConfigurationError(f'For "{self.name}", it''s not a selection parameter, so no two options can share the same parent option')
-            accum_set = accum_set.union(option.parent_option_ids)
-        if len(accum_set) != len(self.parent.options):
-            raise u.ConfigurationError(f'For "{self.name}", all parent option ids must exist across all options')
-    
-    def _set_parent_and_options(self, parent: SingleSelectParameter, all_options: Sequence[po.ParameterOption]) -> None:
-        self.parent = parent
-        self.all_options = all_options
-        self._verify_parent_is_single_select()
-        self._verify_parent_options_have_one_child_each()
-    
-    def _accum_all_dependent_params(self, param_set: ParameterSetBase) -> None:
-        param_set.add_parameter(self)
-        
-    def _enquote(self, value: str) -> str:
-        return "'" + value.replace("'", "''") + "'" 
-
-    def to_json_dict(self) -> Dict:
-        """
-        Helper method to convert the derived Parameter class into a JSON dictionary
-        """
-        return {
-            'widget_type': self.widget_type,
-            'name': self.name,
-            'label': self.label
-        }
-
-
-@dataclass
-class _SelectionParameter(Parameter):
-    def __post_init__(self) -> None:
-        self.trigger_refresh: bool = False
-        self.options: Sequence[po.SelectParameterOption] = tuple(self.all_options)
-        self.children: List[_SelectionParameter] = list()
-        if self.parent is not None:
-            self.parent._add_child_mutate(self)
-        self._refresh_mutate()
-    
-    def _add_child_mutate(self, child: Parameter) -> None:
-        self.children.append(child)
-        self.trigger_refresh = True
-    
-    def _refresh_mutate(self) -> None:
-        if self.parent is not None:
-            self.options = tuple(self._get_valid_options_iterator())
-        self._set_default_as_selection_mutate()
-        self.children = [child.refresh(self) for child in self.children]
-
-    def _get_selected_ids_as_list(self) -> Sequence[str]:
-        raise u.AbstractMethodCallError(self.__class__, "_get_selected_ids_as_list")
-
-    def _get_default_iterator(self) -> Iterator[po.ParameterOption]:
-        return (x.identifier for x in self.options if x.is_default)
-    
-    def _validate_selected_id_in_options(self, selected_id: str) -> str:
-        if selected_id in (x.identifier for x in self.options):
-            return selected_id
-        else:
-            self._raise_invalid_input_error(selected_id)
-    
-    def _accum_all_dependent_params(self, param_set: ParameterSetBase) -> None:
-        super()._accum_all_dependent_params(param_set)
-        for child in self.children:
-            child._accum_all_dependent_params(param_set)
-
-    def to_json_dict(self):
-        """
-        Helper method to convert the derived selection parameter class into a JSON object
-        """
-        output = super().to_json_dict()
-        output['options'] = [x.to_dict() for x in self.options]
-        output['trigger_refresh'] = self.trigger_refresh
-        return output
-
-
-@dataclass
-class SingleSelectParameter(_SelectionParameter):
-    """
-    Class to define attributes for single-select parameter widgets.
-    """
-    selected_id: Optional[str]
-
-    def __init__(self, name: str, label: str, all_options: Sequence[po.SelectParameterOption], *, 
-                 is_hidden: bool = False, parent: Optional[_SelectionParameter] = None) -> None:
-        """
-        Constructor for SingleSelectParameter class
-
-        Parameters:
-            name: The name of the parameter
-            label: The display label for the parameter
-            all_options: A sequence of SelectParameterOption which defines the attribute for each dropdown option
-            is_hidden: Whether the parameter is hidden in the parameters API response. Default is False.
-            parent: The parent parameter that may cascade the options for this parameter. Default is no parent
-        """
-        super().__init__("SingleSelectParameter", name, label, all_options, is_hidden, parent)
-    
-    def with_selection(self, selection: str) -> SingleSelectParameter:
-        """
-        Applies the selected value to this widget parameter
-
-        Parameters:
-            selection: The selected value as an ID of one of the dropdown options
-        
-        Returns:
-            A new copy of SingleSelectParameter with the selection applied
-        """
-        param_copy = copy.copy(self)
-        param_copy.selected_id = self._validate_selected_id_in_options(selection)
-        param_copy.children = [child.refresh(param_copy) for child in param_copy.children]
-        return param_copy
-
-    def get_selected(self) -> po.SelectParameterOption:
-        """
-        Gets the selected single-select option
-
-        Returns:
-            A SelectParameterOption class object
-        """
-        return next(x for x in self.options if x.identifier == self.selected_id)
-    
-    def get_selected_id(self) -> str:
-        """
-        Gets the ID of the selected option
-
-        Returns:
-            A string ID
-        """
-        return self.get_selected().identifier
-    
-    def get_selected_id_quoted(self) -> str:
-        """
-        Gets the ID of the selected option surrounded by single quotes
-
-        Returns:
-            A string
-        """
-        return self._enquote(self.get_selected_id())
-    
-    def get_selected_label(self) -> str:
-        """
-        Gets the label of the selected option
-
-        Returns:
-            A string
-        """
-        return self.get_selected().label
-    
-    def get_selected_label_quoted(self) -> str:
-        """
-        Gets the label of the selected option surrounded by single quotes
-
-        Returns:
-            A string
-        """
-        return self._enquote(self.get_selected_label())
-    
-    # Overriding for refresh method
-    def _get_selected_ids_as_list(self) -> Sequence[str]:
-        return (self.get_selected_id(),)
-    
-    def _get_default(self) -> str:
-        default_id = next(self._get_default_iterator(), None)
-        if default_id is None:
-            default_id = self.options[0].identifier if len(self.options) > 0 else None
-        return default_id
-    
-    def _set_default_as_selection_mutate(self) -> None:
-        self.selected_id = self._get_default()
-
-    def to_json_dict(self) -> Dict:
-        """
-        Converts this parameter as a JSON object for the parameters API response
-
-        Returns:
-            A dictionary for the JSON object
-        """
-        output = super().to_json_dict()
-        output['selected_id'] = self.selected_id
-        return output
-
-
-@dataclass
-class MultiSelectParameter(_SelectionParameter):
-    """
-    Class to define attributes for multi-select parameter widgets.
-    """
-    selected_ids: Sequence[str]
-    include_all: bool
-    order_matters: bool
-
-    def __init__(self, name: str, label: str, all_options: Sequence[po.SelectParameterOption], *, is_hidden = False,
-                 parent: Optional[_SelectionParameter] = None, include_all: bool = True, order_matters: bool = False) -> None:
-        """
-        Constructor for MultiSelectParameter class
-
-        Parameters:
-            name: The name of the parameter
-            label: The display label for the parameter
-            all_options: A sequence of SelectParameterOption which defines the attribute for each dropdown option
-            is_hidden: Whether the parameter is hidden in the parameters API response. Default is False.
-            parent: The parent parameter that may cascade the options for this parameter. Default is no parent
-            include_all: Whether applying no selection is equivalent to selecting all. Default is True
-            order_matters: Whether the ordering of the selection matters. Default is False 
-        """
-        super().__init__("MultiSelectParameter", name, label, all_options, is_hidden, parent)
-        self.include_all = include_all
-        self.order_matters = order_matters
-
-    def with_selection(self, selection: str) -> MultiSelectParameter:
-        """
-        Applies the selected value(s) to this widget parameter
-
-        Parameters:
-            selection: A JSON string of list of strings representing IDs of selected values
-        
-        Returns:
-            A new copy of MultiSelectParameter with the selection applied
-        """
-        param_copy = copy.copy(self)
-        selection_split = u.load_json_or_comma_delimited_str_as_list(selection)
-        param_copy.selected_ids = tuple(self._validate_selected_id_in_options(x) for x in selection_split)
-        param_copy.children = [child.refresh(param_copy) for child in self.children]
-        return param_copy
-    
-    def has_non_empty_selection(self) -> bool:
-        """
-        Returns True if more than zero options were selected. False otherwise.
-        
-        Note that even when this returns False, all "get_selected" functions would 
-        return the full list of options if "include_all" is set to True
-
-        Returns:
-            A boolean
-        """
-        return len(self.selected_ids) > 0
-
-    def get_selected_list(self) -> Sequence[po.SelectParameterOption]:
-        """
-        Gets the sequence of the selected option(s)
-
-        Returns:
-            A sequence of SelectParameterOption class objects
-        """
-        if not self.has_non_empty_selection() and self.include_all:
-            result = tuple(self.options)
-        else:
-            result = tuple(x for x in self.options if x.identifier in self.selected_ids)
-        return result
-    
-    def get_selected_ids_as_list(self) -> Sequence[str]:
-        """
-        Gets the sequence of ID(s) of the selected option(s)
-
-        Returns:
-            A sequence of strings
-        """
-        return tuple(x.identifier for x in self.get_selected_list())
-    
-    def get_selected_ids_joined(self) -> str:
-        """
-        Gets the ID(s) of the selected option(s) joined by comma
-
-        Returns:
-            A string
-        """
-        return ', '.join(self.get_selected_ids_as_list())
-    
-    def get_selected_ids_quoted_as_list(self) -> Sequence[str]:
-        """
-        Gets the sequence of ID(s) of the selected option(s) surrounded by single quotes
-
-        Returns:
-            A sequence of strings
-        """
-        return tuple(self._enquote(x) for x in self.get_selected_ids_as_list())
-    
-    def get_selected_ids_quoted_joined(self) -> str:
-        """
-        Gets the ID(s) of the selected option(s) surrounded by single quotes and joined by comma
-
-        Returns:
-            A string
-        """
-        return ', '.join(self.get_selected_ids_quoted_as_list())
-    
-    def get_selected_labels_as_list(self) -> Sequence[str]:
-        """
-        Gets the sequence of label(s) of the selected option(s)
-
-        Returns:
-            A sequence of strings
-        """
-        return tuple(x.label for x in self.get_selected_list())
-    
-    def get_selected_labels_joined(self) -> str:
-        """
-        Gets the label(s) of the selected option(s) joined by comma
-
-        Returns:
-            A string
-        """
-        return ', '.join(self.get_selected_labels_as_list())
-    
-    def get_selected_labels_quoted_as_list(self) -> Sequence[str]:
-        """
-        Gets the sequence of label(s) of the selected option(s) surrounded by single quotes
-
-        Returns:
-            A sequence of strings
-        """
-        return tuple(self._enquote(x) for x in self.get_selected_labels_as_list())
-    
-    def get_selected_labels_quoted_joined(self) -> str:
-        """
-        Gets the label(s) of the selected option(s) surrounded by single quotes and joined by comma
-
-        Returns:
-            A string
-        """
-        return ', '.join(self.get_selected_labels_quoted_as_list())
-    
-    def _get_selected_ids_as_list(self) -> Sequence[str]:
-        return self.get_selected_ids_as_list()
-    
-    def _get_default(self) -> Sequence[str]:
-        return tuple(self._get_default_iterator())
-    
-    def _set_default_as_selection_mutate(self):
-        self.selected_ids = self._get_default()
-
-    def to_json_dict(self):
-        """
-        Converts this parameter as a JSON object for the parameters API response
-
-        Returns:
-            A dictionary for the JSON object
-        """
-        output = super().to_json_dict()
-        output['selected_ids'] = list(self.selected_ids)
-        output['include_all'] = self.include_all
-        output['order_matters'] = self.order_matters
-        return output
-
-
-@dataclass
-class DateParameter(Parameter):
-    """
-    Class to define attributes for date parameter widgets.
-    """
-    curr_option: po.DateParameterOption
-    selected_date: datetime
-
-    def __init__(self, name: str, label: str, default_date: Union[str, datetime], date_format: str = '%Y-%m-%d', 
-                 *, is_hidden: bool = False) -> None:
-        """
-        Constructor for DateParameter class
-
-        Parameters:
-            name: The name of the parameter
-            label: The display label for the parameter
-            default_date: The default selected date
-            date_format: The format of the default_date. Default is '%Y-%m-%d'
-            is_hidden: Whether the parameter is hidden in the parameters API response. Default is False
-        """
-        self.curr_option = po.DateParameterOption(default_date, date_format)
-        all_options = (self.curr_option,)
-        super().__init__("DateParameter", name, label, all_options, is_hidden, None)
-        self._set_default_as_selection_mutate()
-    
-    @staticmethod
-    def WithParent(name: str, label: str, all_options: Sequence[po.DateParameterOption], parent: SingleSelectParameter, *, 
-                   is_hidden: bool = False) -> DateParameter:
-        """
-        A factory method to construct a DateParameter with a parent parameter
-
-        Parameters:
-            name: The name of the parameter
-            label: The display label for the parameter
-            all_options: A sequence of DateParameterOption which contains various default dates linked to specific parent options
-            parent: The parent parameter, which must be a SingleSelectParameter
-            is_hidden: Whether the parameter is hidden in the parameters API response. Default is False
-        """
-        new_param = DateParameter(name, label, '2020-01-01', is_hidden=is_hidden) # dummy date in valid format
-        return Parameter.WithParent(all_options, parent, new_param)
-    
-    def with_selection(self, selection: str):
-        """
-        Applies the selected date to this widget parameter
-
-        Parameters:
-            selection: The date string which must be in yyyy-mm-dd format (regardless of self.date_format value)
-        
-        Returns:
-            A new copy of DateParameter with the selection applied
-        """
-        param_copy = copy.copy(self)
-        try:
-            param_copy.selected_date = datetime.strptime(selection, "%Y-%m-%d")
-        except ValueError as e:
-            self._raise_invalid_input_error(selection, 'Invalid selection for date.', e)
-        return param_copy
-
-    def get_selected_date(self, date_format: str = None) -> str:
-        """
-        Gets selected date as string
-
-        Parameters:
-            date_format: The date format (see Python's datetime formats). If not specified, self.date_format is used
-
-        Returns:
-            A string
-        """
-        date_format = self.curr_option.date_format if date_format is None else date_format
-        return self.selected_date.strftime(date_format)
-
-    def get_selected_date_quoted(self, date_format: str = None) -> str:
-        """
-        Gets selected date as string surrounded by single quotes
-
-        Parameters:
-            date_format: The date format (see Python's datetime formats). If not specified, self.date_format is used
-
-        Returns:
-            A string
-        """
-        return self._enquote(self.get_selected_date(date_format))
-    
-    def _set_default_as_selection_mutate(self) -> None:
-        self.selected_date = self.curr_option.default_date
-    
-    def to_json_dict(self):
-        """
-        Converts this parameter as a JSON object for the parameters API response
-
-        The "selected_date" field will always be in yyyy-mm-dd format
-
-        Returns:
-            A dictionary for the JSON object
-        """
-        output = super().to_json_dict()
-        output['selected_date'] = self.get_selected_date("%Y-%m-%d")
-        return output
-
-
-@dataclass
-class _NumericParameter(Parameter):
-    curr_option: po.NumericParameterOption
-    
-    def to_json_dict(self):
-        """
-        Helper method to converts numeric parameters into JSON objects for the parameters API response
-
-        Returns:
-            A dictionary for the JSON object
-        """
-        output = super().to_json_dict()
-        output['min_value'] = str(self.curr_option.min_value)
-        output['max_value'] = str(self.curr_option.max_value)
-        output['increment'] = str(self.curr_option.increment)
-        return output
-
-
-@dataclass
-class NumberParameter(_NumericParameter):
-    """
-    Class to define attributes for number slider parameter widgets.
-    """
-    selected_value: Decimal
-
-    def __init__(self, name: str, label: str, min_value: po.Number, max_value: po.Number, increment: po.Number = 1, 
-                 default_value: po.Number = None, *, is_hidden: bool = False) -> None:
-        """
-        Constructor for NumberParameter class
-
-        Parameters:
-            name: The name of the parameter
-            label: The display label for the parameter
-            min_value: The minimum bound for selection. Can be of type Decimal, integer, or number parsable string
-            max_value: The maxixmum bound for selection. Can be of type Decimal, integer, or number parsable string
-            increment: The increment for allowable selections. Can be of type Decimal, integer, or number parsable string. Default is 1
-            default_value: The default selection. Can be of type Decimal, integer, or number parsable string. Default is min_value
-            is_hidden: Whether the parameter is hidden in the parameters API response. Default is False
-        """
-        default_value = default_value if default_value is not None else min_value
-        curr_option = po.NumberParameterOption(min_value, max_value, increment, default_value)
-        all_options = (curr_option,)
-        super().__init__("NumberParameter", name, label, all_options, is_hidden, None, curr_option)
-        self._set_default_as_selection_mutate()
-    
-    @staticmethod
-    def WithParent(name: str, label: str, all_options: Sequence[po.NumberParameterOption], parent: SingleSelectParameter, *, 
-                   is_hidden: bool = False) -> DateParameter:
-        """
-        A factory method to construct a NumberParameter with a parent parameter
-
-        Parameters:
-            name: The name of the parameter
-            label: The display label for the parameter
-            all_options: A sequence of NumberParameterOption which contains various bounds and default values linked to specific parent options
-            parent: The parent parameter, which must be a SingleSelectParameter
-            is_hidden: Whether the parameter is hidden in the parameters API response. Default is False
-        """
-        new_param = NumberParameter(name, label, 0, 1, is_hidden=is_hidden) # dummy values
-        return Parameter.WithParent(all_options, parent, new_param)
-    
-    def with_selection(self, selection: str):
-        """
-        Applies the selected number to this widget parameter
-
-        Parameters:
-            selection: The selected number (must be a string parsable as a number)
-        
-        Returns:
-            A new copy of NumberParameter with the selection applied
-        """
-        param_copy = copy.copy(self)
-        try:
-            param_copy.selected_value = param_copy.curr_option._validate_value(selection)
-        except u.ConfigurationError as e:
-            self._raise_invalid_input_error(selection, 'Invalid selection for number parameter.', e)
-        return param_copy
-
-    def get_selected_value(self) -> str:
-        """
-        Get the selected number
-
-        Returns:
-            A number parsable string of the selected number
-        """
-        return str(self.selected_value)
-    
-    def _set_default_as_selection_mutate(self) -> None:
-        self.curr_option: po.NumberParameterOption
-        self.selected_value = self.curr_option.default_value
-        
-    def to_json_dict(self):
-        """
-        Converts this parameter as a JSON object for the parameters API response
-
-        Returns:
-            A dictionary for the JSON object
-        """
-        output = super().to_json_dict()
-        output['selected_value'] = self.get_selected_value()
-        return output
-
-
-@dataclass
-class NumRangeParameter(_NumericParameter):
-    """
-    Class to define attributes for number range slider (double-ended) parameter widgets.
-    """
-    selected_lower_value: Decimal
-    selected_upper_value: Decimal
-
-    def __init__(self, name: str, label: str, min_value: po.Number, max_value: po.Number, increment: po.Number = 1, 
-                 default_lower_value: po.Number = None, default_upper_value: po.Number = None, *, is_hidden: bool = False) -> None:
-        """
-        Constructor for NumberParameter class
-
-        Parameters:
-            name: The name of the parameter
-            label: The display label for the parameter
-            min_value: The minimum bound for selection. Can be of type Decimal, integer, or number parsable string
-            max_value: The maxixmum bound for selection. Can be of type Decimal, integer, or number parsable string
-            increment: The increment for allowable selections. Can be of type Decimal, integer, or number parsable string. Default is 1
-            default_lower_value: The default lower selection. Can be of type Decimal, integer, or number parsable string. Default is min_value
-            default_upper_value: The default upper selection. Can be of type Decimal, integer, or number parsable string. Default is max_value
-            is_hidden: Whether the parameter is hidden in the parameters API response. Default is False
-        """
-        default_lower_value = default_lower_value if default_lower_value is not None else min_value
-        default_upper_value = default_upper_value if default_upper_value is not None else max_value
-        curr_option = po.NumRangeParameterOption(min_value, max_value, increment, default_lower_value, default_upper_value)
-        all_options = (curr_option,)
-        super().__init__("NumRangeParameter", name, label, all_options, is_hidden, None, curr_option)
-        self._set_default_as_selection_mutate()
-    
-    @staticmethod
-    def WithParent(name: str, label: str, all_options: Sequence[po.NumRangeParameterOption], parent: SingleSelectParameter, *, 
-                   is_hidden: bool = False) -> DateParameter:
-        """
-        A factory method to construct a NumRangeParameter with a parent parameter
-
-        Parameters:
-            name: The name of the parameter
-            label: The display label for the parameter
-            all_options: A sequence of NumRangeParameterOption which contains various bounds and default values linked to specific parent options
-            parent: The parent parameter, which must be a SingleSelectParameter
-            is_hidden: Whether the parameter is hidden in the parameters API response. Default is False
-        """
-        new_param = NumRangeParameter(name, label, 0, 1, is_hidden=is_hidden) # dummy values
-        return Parameter.WithParent(all_options, parent, new_param)
-    
-    def with_selection(self, selection: str):
-        """
-        Applies the selected numbers to this widget parameter
-
-        Parameters:
-            selection: The lower and upper selected numbers joined by comma (with no spaces)
-        
-        Returns:
-            A new copy of NumRangeParameter with the selection applied
-        """
-        try:
-            lower, upper = selection.split(',')
-        except ValueError as e:
-            self._raise_invalid_input_error(selection, "Range parameter selection must be two numbers joined by comma.", e)
-
-        param_copy = copy.copy(self)
-        try:
-            param_copy.selected_lower_value = param_copy.curr_option._validate_value(lower)
-            param_copy.selected_upper_value = param_copy.curr_option._validate_value(upper, param_copy.selected_lower_value)
-        except u.ConfigurationError as e:
-            self._raise_invalid_input_error(selection, 'Invalid selection for range parameter.', e)
-        return param_copy
-
-    def get_selected_lower_value(self) -> str:
-        """
-        Get the selected lower number
-
-        Returns:
-            A number parsable string of the selected number
-        """
-        return str(self.selected_lower_value)
-
-    def get_selected_upper_value(self) -> str:
-        """
-        Get the selected upper number
-
-        Returns:
-            A number parsable string of the selected number
-        """
-        return str(self.selected_upper_value)
-    
-    def _set_default_as_selection_mutate(self) -> None:
-        self.curr_option: po.NumRangeParameterOption
-        self.selected_lower_value = self.curr_option.default_lower_value
-        self.selected_upper_value = self.curr_option.default_upper_value
-
-    def to_json_dict(self):
-        """
-        Converts this parameter as a JSON object for the parameters API response
-
-        Returns:
-            A dictionary for the JSON object
-        """
-        output = super().to_json_dict()
-        output['selected_lower_value'] = self.get_selected_lower_value()
-        output['selected_upper_value'] = self.get_selected_upper_value()
-        return output
-
-
-@dataclass
-class DataSourceParameter(Parameter):
-    """
-    Class for parameters that can use a lookup table to convert itself into another parameter
-    """
-    parameter_class: Type[Parameter]
-    data_source: DataSource
-    parent: Optional[Parameter] 
-
-    def __init__(self, parameter_class: Type[Parameter], name: str, label: str, data_source: DataSource, *, 
-                 is_hidden: bool = False, parent: Optional[Parameter] = None) -> None:
-        """
-        Constructor for DataSourceParameter, a Parameter that uses a DataSource to convert itself to another Parameter
-
-        Parameters:
-            parameter_class: The class of widget parameter to convert to
-            name: The name of the parameter
-            label: The display label for the parameter
-            data_source: The lookup table to use for this parameter
-            is_hidden: Whether the parameter is hidden in the parameters API response. Default is False
-            parent: The parent parameter that may cascade the options for this parameter. Default is no parent
-        """
-        super().__init__("DataSourceParameter", name, label, None, is_hidden, None)
-        self.parameter_class = parameter_class
-        self.data_source = data_source
-        self.parent = parent
-
-    def convert(self, df: pd.DataFrame) -> Parameter:
-        """
-        Method to convert this DataSourceParameter into another parameter
-
-        Parameters:
-            df: The dataframe containing the parameter options data
-
-        Returns:
-            The converted parameter
-        """
-        return self.data_source.convert(self, df)
-    
-    def to_json_dict(self) -> Dict:
-        """
-        Converts this parameter as a JSON object for the parameters API response
-
-        Returns:
-            A dictionary for the JSON object
-        """
-        output = super().to_json_dict()
-        output['widget_type'] = self.parameter_class.__name__
-        output['data_source'] = self.data_source.__dict__
-        return output
-
-
-# Types:
-SelectionParameter = Union[SingleSelectParameter, MultiSelectParameter]
-NumericParameter = Union[NumberParameter, NumRangeParameter]
+from __future__ import annotations
+from typing import Type, Sequence, Dict, List, Any, Iterator, Optional, Union
+from dataclasses import dataclass
+from datetime import datetime
+from decimal import Decimal
+import copy
+
+from squirrels import parameter_options as po, _utils as u
+from squirrels.data_sources import DataSource
+from squirrels._parameter_set import ParameterSetBase
+from squirrels._timed_imports import pandas as pd
+
+
+@dataclass
+class Parameter:
+    """
+    Abstract class for all parameter classes. Useful for type hints.
+    """
+    widget_type: str
+    name: str
+    label: str
+    all_options: Sequence[po.ParameterOption]
+    is_hidden: bool
+    parent: Optional[_SelectionParameter]
+
+    def WithParent(all_options: Sequence[po.ParameterOption], parent: SingleSelectParameter, new_param: Parameter):
+        """
+        Helper class method to assign a SingleSelectParameter as the parent for another parameter
+
+        Parameters:
+            all_options: The list of options with one of "parent_option_id" or "parent_option_ids" attribute set.
+            parent: The parent parameter. All option ids of the parent must exist at least once in "parent_option_ids" of all_options
+            new_param: The child parameter to modify. Usually not a selection parameter
+        """
+        new_param._set_parent_and_options(parent, all_options)
+        new_param.parent._add_child_mutate(new_param)
+        return new_param.refresh(parent)
+
+    def refresh(self, parent: Optional[_SelectionParameter] = None) -> Parameter:
+        """
+        Refreshes the selectable options (or change of default value) based on the selection of the parent parameter
+
+        Parameters:
+            parent: The parent parameter subscribed to for updates
+        
+        Returns:
+            A copy of self for the new selectable options based on current selection of parent
+        """
+        param_copy = copy.copy(self)
+        if parent is not None:
+            param_copy.parent = parent
+        param_copy._refresh_mutate()
+        return param_copy
+
+    def with_selection(self, _: str) -> Parameter:
+        """
+        Abstract method for applying the selection to the parameter
+        """
+        raise u.AbstractMethodCallError(self.__class__, "with_selection")
+    
+    def get_all_dependent_params(self) -> ParameterSetBase:
+        """
+        Gets the collection of descendent parameters with changes applied based on the selection of this parameter
+
+        Returns:
+            A collection of descendent parameters as a ParameterSetBase
+        """
+        dependent_params = ParameterSetBase()
+        self._accum_all_dependent_params(dependent_params)
+        return dependent_params
+    
+    def _set_default_as_selection_mutate(self) -> None:
+        raise u.AbstractMethodCallError(self.__class__, "_set_default_as_selection_mutate")
+    
+    def _refresh_mutate(self) -> None:
+        if self.parent is not None and hasattr(self, 'curr_option'):
+            self.curr_option = next(self._get_valid_options_iterator())
+        self._set_default_as_selection_mutate()
+    
+    def _get_valid_options_iterator(self) -> Iterator[po.ParameterOption]:
+        selected_parent_option_ids = self.parent._get_selected_ids_as_list()
+        return (x for x in self.all_options if x.is_valid(selected_parent_option_ids))
+    
+    def _raise_invalid_input_error(self, selection: str, more_details: str = '', e: Exception = None) -> None:
+        raise u.InvalidInputError(f'Selected value "{selection}" is not valid for parameter "{self.name}". ' + more_details) from e
+    
+    def _verify_parent_is_single_select(self) -> None:
+        if not isinstance(self.parent, SingleSelectParameter):
+            raise u.ConfigurationError(f'For "{self.name}", it''s not a selection parameter, so its parent must be a SingleSelectParameter')
+        
+    def _verify_parent_options_have_one_child_each(self) -> None:
+        accum_set = set()
+        for option in self.all_options:
+            if not accum_set.isdisjoint(option.parent_option_ids):
+                raise u.ConfigurationError(f'For "{self.name}", it''s not a selection parameter, so no two options can share the same parent option')
+            accum_set = accum_set.union(option.parent_option_ids)
+        if len(accum_set) != len(self.parent.options):
+            raise u.ConfigurationError(f'For "{self.name}", all parent option ids must exist across all options')
+    
+    def _set_parent_and_options(self, parent: SingleSelectParameter, all_options: Sequence[po.ParameterOption]) -> None:
+        self.parent = parent
+        self.all_options = all_options
+        self._verify_parent_is_single_select()
+        self._verify_parent_options_have_one_child_each()
+    
+    def _accum_all_dependent_params(self, param_set: ParameterSetBase) -> None:
+        param_set.add_parameter(self)
+        
+    def _enquote(self, value: str) -> str:
+        return "'" + value.replace("'", "''") + "'" 
+
+    def to_json_dict(self) -> Dict:
+        """
+        Helper method to convert the derived Parameter class into a JSON dictionary
+        """
+        return {
+            'widget_type': self.widget_type,
+            'name': self.name,
+            'label': self.label
+        }
+
+
+@dataclass
+class _SelectionParameter(Parameter):
+    def __post_init__(self) -> None:
+        self.trigger_refresh: bool = False
+        self.options: Sequence[po.SelectParameterOption] = tuple(self.all_options)
+        self.children: List[_SelectionParameter] = list()
+        if self.parent is not None:
+            self.parent._add_child_mutate(self)
+        self._refresh_mutate()
+    
+    def _add_child_mutate(self, child: Parameter) -> None:
+        self.children.append(child)
+        self.trigger_refresh = True
+    
+    def _refresh_mutate(self) -> None:
+        if self.parent is not None:
+            self.options = tuple(self._get_valid_options_iterator())
+        self._set_default_as_selection_mutate()
+        self.children = [child.refresh(self) for child in self.children]
+
+    def _get_selected_ids_as_list(self) -> Sequence[str]:
+        raise u.AbstractMethodCallError(self.__class__, "_get_selected_ids_as_list")
+
+    def _get_default_iterator(self) -> Iterator[po.ParameterOption]:
+        return (x.identifier for x in self.options if x.is_default)
+    
+    def _validate_selected_id_in_options(self, selected_id: str) -> str:
+        if selected_id in (x.identifier for x in self.options):
+            return selected_id
+        else:
+            self._raise_invalid_input_error(selected_id)
+    
+    def _accum_all_dependent_params(self, param_set: ParameterSetBase) -> None:
+        super()._accum_all_dependent_params(param_set)
+        for child in self.children:
+            child._accum_all_dependent_params(param_set)
+
+    def to_json_dict(self):
+        """
+        Helper method to convert the derived selection parameter class into a JSON object
+        """
+        output = super().to_json_dict()
+        output['options'] = [x.to_dict() for x in self.options]
+        output['trigger_refresh'] = self.trigger_refresh
+        return output
+
+
+@dataclass
+class SingleSelectParameter(_SelectionParameter):
+    """
+    Class to define attributes for single-select parameter widgets.
+    """
+    selected_id: Optional[str]
+
+    def __init__(self, name: str, label: str, all_options: Sequence[po.SelectParameterOption], *, 
+                 is_hidden: bool = False, parent: Optional[_SelectionParameter] = None) -> None:
+        """
+        Constructor for SingleSelectParameter class
+
+        Parameters:
+            name: The name of the parameter
+            label: The display label for the parameter
+            all_options: A sequence of SelectParameterOption which defines the attribute for each dropdown option
+            is_hidden: Whether the parameter is hidden in the parameters API response. Default is False.
+            parent: The parent parameter that may cascade the options for this parameter. Default is no parent
+        """
+        super().__init__("SingleSelectParameter", name, label, all_options, is_hidden, parent)
+    
+    def with_selection(self, selection: str) -> SingleSelectParameter:
+        """
+        Applies the selected value to this widget parameter
+
+        Parameters:
+            selection: The selected value as an ID of one of the dropdown options
+        
+        Returns:
+            A new copy of SingleSelectParameter with the selection applied
+        """
+        param_copy = copy.copy(self)
+        param_copy.selected_id = self._validate_selected_id_in_options(selection)
+        param_copy.children = [child.refresh(param_copy) for child in param_copy.children]
+        return param_copy
+    
+    def get_selected(self, field: Optional[str] = None, *, default_field: Optional[str] = None,
+                     default: Any = None) -> Union[po.SelectParameterOption, str]:
+        """
+        Gets the selected single-select option or selected custom field
+
+        Parameters:
+            field: If field is not None, the method gets this field from the "custom_fields" attribute of the selected option. 
+                Otherwise, returns the class object of the selected option
+            default_field: If field does not exist for a parameter option and default_field is not None, the default_field is used 
+                as the "field" instead. Does nothing if field is None
+            default: If field does not exist for a parameter option, default_field is None, but default is not None, then the default 
+                is returned as the selected field. Does nothing if field is None or default_field is not None
+
+        Returns:
+            A SelectParameterOption class object if no field is provided, or the type of the custom field
+        """
+        selected = next(x for x in self.options if x.identifier == self.selected_id)
+        if field is not None:
+            selected = selected.get_custom_field(field, default_field, default)
+        return selected
+    
+    def get_selected_id(self) -> str:
+        """
+        Gets the ID of the selected option
+
+        Returns:
+            A string ID
+        """
+        return self.get_selected().identifier
+    
+    def get_selected_id_quoted(self) -> str:
+        """
+        Gets the ID of the selected option surrounded by single quotes
+
+        Returns:
+            A string
+        """
+        return self._enquote(self.get_selected_id())
+    
+    def get_selected_label(self) -> str:
+        """
+        Gets the label of the selected option
+
+        Returns:
+            A string
+        """
+        return self.get_selected().label
+    
+    def get_selected_label_quoted(self) -> str:
+        """
+        Gets the label of the selected option surrounded by single quotes
+
+        Returns:
+            A string
+        """
+        return self._enquote(self.get_selected_label())
+    
+    # Overriding for refresh method
+    def _get_selected_ids_as_list(self) -> Sequence[str]:
+        return (self.get_selected_id(),)
+    
+    def _get_default(self) -> str:
+        default_id = next(self._get_default_iterator(), None)
+        if default_id is None:
+            default_id = self.options[0].identifier if len(self.options) > 0 else None
+        return default_id
+    
+    def _set_default_as_selection_mutate(self) -> None:
+        self.selected_id = self._get_default()
+
+    def to_json_dict(self) -> Dict:
+        """
+        Converts this parameter as a JSON object for the parameters API response
+
+        Returns:
+            A dictionary for the JSON object
+        """
+        output = super().to_json_dict()
+        output['selected_id'] = self.selected_id
+        return output
+
+
+@dataclass
+class MultiSelectParameter(_SelectionParameter):
+    """
+    Class to define attributes for multi-select parameter widgets.
+    """
+    selected_ids: Sequence[str]
+    include_all: bool
+    order_matters: bool
+
+    def __init__(self, name: str, label: str, all_options: Sequence[po.SelectParameterOption], *, is_hidden = False,
+                 parent: Optional[_SelectionParameter] = None, include_all: bool = True, order_matters: bool = False) -> None:
+        """
+        Constructor for MultiSelectParameter class
+
+        Parameters:
+            name: The name of the parameter
+            label: The display label for the parameter
+            all_options: A sequence of SelectParameterOption which defines the attribute for each dropdown option
+            is_hidden: Whether the parameter is hidden in the parameters API response. Default is False.
+            parent: The parent parameter that may cascade the options for this parameter. Default is no parent
+            include_all: Whether applying no selection is equivalent to selecting all. Default is True
+            order_matters: Whether the ordering of the selection matters. Default is False 
+        """
+        super().__init__("MultiSelectParameter", name, label, all_options, is_hidden, parent)
+        self.include_all = include_all
+        self.order_matters = order_matters
+
+    def with_selection(self, selection: str) -> MultiSelectParameter:
+        """
+        Applies the selected value(s) to this widget parameter
+
+        Parameters:
+            selection: A JSON string of list of strings representing IDs of selected values
+        
+        Returns:
+            A new copy of MultiSelectParameter with the selection applied
+        """
+        param_copy = copy.copy(self)
+        selection_split = u.load_json_or_comma_delimited_str_as_list(selection)
+        param_copy.selected_ids = tuple(self._validate_selected_id_in_options(x) for x in selection_split)
+        param_copy.children = [child.refresh(param_copy) for child in self.children]
+        return param_copy
+    
+    def has_non_empty_selection(self) -> bool:
+        """
+        Returns True if more than zero options were selected. False otherwise.
+        
+        Note that even when this returns False, all "get_selected" functions would 
+        return the full list of options if "include_all" is set to True
+
+        Returns:
+            A boolean
+        """
+        return len(self.selected_ids) > 0
+
+    def get_selected_list(self, field: Optional[str] = None, *, default_field: Optional[str] = None,
+                          default: Any = None) -> Sequence[Union[po.SelectParameterOption, Any]]:
+        """
+        Gets the sequence of the selected option(s) or a sequence of selected custom fields
+
+        Parameters:
+            field: If field is not None, the method gets this field from the "custom_fields" attribute of the selected options. 
+                Otherwise, returns the class objects of the selected options
+            default_field: If field does not exist for a parameter option and default_field is not None, the default_field is used 
+                as the "field" instead. Does nothing if field is None
+            default: If field does not exist for a parameter option, default_field is None, but default is not None, the default 
+                is returned as the selected field. Does nothing if field is None or default_field is not None
+
+        Returns:
+            A sequence of SelectParameterOption class objects or sequence of type of custom field
+        """
+        if not self.has_non_empty_selection() and self.include_all:
+            selected_list = self.options
+        else:
+            selected_list = (x for x in self.options if x.identifier in self.selected_ids)
+        
+        if field is not None:
+            selected_list = [selected.get_custom_field(field, default_field, default) for selected in selected_list]
+        
+        return tuple(selected_list)
+
+    def get_selected_ids_as_list(self) -> Sequence[str]:
+        """
+        Gets the sequence of ID(s) of the selected option(s)
+
+        Returns:
+            A sequence of strings
+        """
+        return tuple(x.identifier for x in self.get_selected_list())
+    
+    def get_selected_ids_joined(self) -> str:
+        """
+        Gets the ID(s) of the selected option(s) joined by comma
+
+        Returns:
+            A string
+        """
+        return ', '.join(self.get_selected_ids_as_list())
+    
+    def get_selected_ids_quoted_as_list(self) -> Sequence[str]:
+        """
+        Gets the sequence of ID(s) of the selected option(s) surrounded by single quotes
+
+        Returns:
+            A sequence of strings
+        """
+        return tuple(self._enquote(x) for x in self.get_selected_ids_as_list())
+    
+    def get_selected_ids_quoted_joined(self) -> str:
+        """
+        Gets the ID(s) of the selected option(s) surrounded by single quotes and joined by comma
+
+        Returns:
+            A string
+        """
+        return ', '.join(self.get_selected_ids_quoted_as_list())
+    
+    def get_selected_labels_as_list(self) -> Sequence[str]:
+        """
+        Gets the sequence of label(s) of the selected option(s)
+
+        Returns:
+            A sequence of strings
+        """
+        return tuple(x.label for x in self.get_selected_list())
+    
+    def get_selected_labels_joined(self) -> str:
+        """
+        Gets the label(s) of the selected option(s) joined by comma
+
+        Returns:
+            A string
+        """
+        return ', '.join(self.get_selected_labels_as_list())
+    
+    def get_selected_labels_quoted_as_list(self) -> Sequence[str]:
+        """
+        Gets the sequence of label(s) of the selected option(s) surrounded by single quotes
+
+        Returns:
+            A sequence of strings
+        """
+        return tuple(self._enquote(x) for x in self.get_selected_labels_as_list())
+    
+    def get_selected_labels_quoted_joined(self) -> str:
+        """
+        Gets the label(s) of the selected option(s) surrounded by single quotes and joined by comma
+
+        Returns:
+            A string
+        """
+        return ', '.join(self.get_selected_labels_quoted_as_list())
+    
+    def _get_selected_ids_as_list(self) -> Sequence[str]:
+        return self.get_selected_ids_as_list()
+    
+    def _get_default(self) -> Sequence[str]:
+        return tuple(self._get_default_iterator())
+    
+    def _set_default_as_selection_mutate(self):
+        self.selected_ids = self._get_default()
+
+    def to_json_dict(self):
+        """
+        Converts this parameter as a JSON object for the parameters API response
+
+        Returns:
+            A dictionary for the JSON object
+        """
+        output = super().to_json_dict()
+        output['selected_ids'] = list(self.selected_ids)
+        output['include_all'] = self.include_all
+        output['order_matters'] = self.order_matters
+        return output
+
+
+@dataclass
+class DateParameter(Parameter):
+    """
+    Class to define attributes for date parameter widgets.
+    """
+    curr_option: po.DateParameterOption
+    selected_date: datetime
+
+    def __init__(self, name: str, label: str, default_date: Union[str, datetime], date_format: str = '%Y-%m-%d', 
+                 *, is_hidden: bool = False) -> None:
+        """
+        Constructor for DateParameter class
+
+        Parameters:
+            name: The name of the parameter
+            label: The display label for the parameter
+            default_date: The default selected date
+            date_format: The format of the default_date. Default is '%Y-%m-%d'
+            is_hidden: Whether the parameter is hidden in the parameters API response. Default is False
+        """
+        self.curr_option = po.DateParameterOption(default_date, date_format)
+        all_options = (self.curr_option,)
+        super().__init__("DateParameter", name, label, all_options, is_hidden, None)
+        self._set_default_as_selection_mutate()
+    
+    @staticmethod
+    def WithParent(name: str, label: str, all_options: Sequence[po.DateParameterOption], parent: SingleSelectParameter, *, 
+                   is_hidden: bool = False) -> DateParameter:
+        """
+        A factory method to construct a DateParameter with a parent parameter
+
+        Parameters:
+            name: The name of the parameter
+            label: The display label for the parameter
+            all_options: A sequence of DateParameterOption which contains various default dates linked to specific parent options
+            parent: The parent parameter, which must be a SingleSelectParameter
+            is_hidden: Whether the parameter is hidden in the parameters API response. Default is False
+        """
+        new_param = DateParameter(name, label, '2020-01-01', is_hidden=is_hidden) # dummy date in valid format
+        return Parameter.WithParent(all_options, parent, new_param)
+    
+    def with_selection(self, selection: str):
+        """
+        Applies the selected date to this widget parameter
+
+        Parameters:
+            selection: The date string which must be in yyyy-mm-dd format (regardless of self.date_format value)
+        
+        Returns:
+            A new copy of DateParameter with the selection applied
+        """
+        param_copy = copy.copy(self)
+        try:
+            param_copy.selected_date = datetime.strptime(selection, "%Y-%m-%d")
+        except ValueError as e:
+            self._raise_invalid_input_error(selection, 'Invalid selection for date.', e)
+        return param_copy
+
+    def get_selected_date(self, date_format: str = None) -> str:
+        """
+        Gets selected date as string
+
+        Parameters:
+            date_format: The date format (see Python's datetime formats). If not specified, self.date_format is used
+
+        Returns:
+            A string
+        """
+        date_format = self.curr_option.date_format if date_format is None else date_format
+        return self.selected_date.strftime(date_format)
+
+    def get_selected_date_quoted(self, date_format: str = None) -> str:
+        """
+        Gets selected date as string surrounded by single quotes
+
+        Parameters:
+            date_format: The date format (see Python's datetime formats). If not specified, self.date_format is used
+
+        Returns:
+            A string
+        """
+        return self._enquote(self.get_selected_date(date_format))
+    
+    def _set_default_as_selection_mutate(self) -> None:
+        self.selected_date = self.curr_option.default_date
+    
+    def to_json_dict(self):
+        """
+        Converts this parameter as a JSON object for the parameters API response
+
+        The "selected_date" field will always be in yyyy-mm-dd format
+
+        Returns:
+            A dictionary for the JSON object
+        """
+        output = super().to_json_dict()
+        output['selected_date'] = self.get_selected_date("%Y-%m-%d")
+        return output
+
+
+@dataclass
+class _NumericParameter(Parameter):
+    curr_option: po.NumericParameterOption
+    
+    def to_json_dict(self):
+        """
+        Helper method to converts numeric parameters into JSON objects for the parameters API response
+
+        Returns:
+            A dictionary for the JSON object
+        """
+        output = super().to_json_dict()
+        output['min_value'] = str(self.curr_option.min_value)
+        output['max_value'] = str(self.curr_option.max_value)
+        output['increment'] = str(self.curr_option.increment)
+        return output
+
+
+@dataclass
+class NumberParameter(_NumericParameter):
+    """
+    Class to define attributes for number slider parameter widgets.
+    """
+    selected_value: Decimal
+
+    def __init__(self, name: str, label: str, min_value: po.Number, max_value: po.Number, increment: po.Number = 1, 
+                 default_value: po.Number = None, *, is_hidden: bool = False) -> None:
+        """
+        Constructor for NumberParameter class
+
+        Parameters:
+            name: The name of the parameter
+            label: The display label for the parameter
+            min_value: The minimum bound for selection. Can be of type Decimal, integer, or number parsable string
+            max_value: The maxixmum bound for selection. Can be of type Decimal, integer, or number parsable string
+            increment: The increment for allowable selections. Can be of type Decimal, integer, or number parsable string. Default is 1
+            default_value: The default selection. Can be of type Decimal, integer, or number parsable string. Default is min_value
+            is_hidden: Whether the parameter is hidden in the parameters API response. Default is False
+        """
+        default_value = default_value if default_value is not None else min_value
+        curr_option = po.NumberParameterOption(min_value, max_value, increment, default_value)
+        all_options = (curr_option,)
+        super().__init__("NumberParameter", name, label, all_options, is_hidden, None, curr_option)
+        self._set_default_as_selection_mutate()
+    
+    @staticmethod
+    def WithParent(name: str, label: str, all_options: Sequence[po.NumberParameterOption], parent: SingleSelectParameter, *, 
+                   is_hidden: bool = False) -> DateParameter:
+        """
+        A factory method to construct a NumberParameter with a parent parameter
+
+        Parameters:
+            name: The name of the parameter
+            label: The display label for the parameter
+            all_options: A sequence of NumberParameterOption which contains various bounds and default values linked to specific parent options
+            parent: The parent parameter, which must be a SingleSelectParameter
+            is_hidden: Whether the parameter is hidden in the parameters API response. Default is False
+        """
+        new_param = NumberParameter(name, label, 0, 1, is_hidden=is_hidden) # dummy values
+        return Parameter.WithParent(all_options, parent, new_param)
+    
+    def with_selection(self, selection: str):
+        """
+        Applies the selected number to this widget parameter
+
+        Parameters:
+            selection: The selected number (must be a string parsable as a number)
+        
+        Returns:
+            A new copy of NumberParameter with the selection applied
+        """
+        param_copy = copy.copy(self)
+        try:
+            param_copy.selected_value = param_copy.curr_option._validate_value(selection)
+        except u.ConfigurationError as e:
+            self._raise_invalid_input_error(selection, 'Invalid selection for number parameter.', e)
+        return param_copy
+
+    def get_selected_value(self) -> str:
+        """
+        Get the selected number
+
+        Returns:
+            A number parsable string of the selected number
+        """
+        return str(self.selected_value)
+    
+    def _set_default_as_selection_mutate(self) -> None:
+        self.curr_option: po.NumberParameterOption
+        self.selected_value = self.curr_option.default_value
+        
+    def to_json_dict(self):
+        """
+        Converts this parameter as a JSON object for the parameters API response
+
+        Returns:
+            A dictionary for the JSON object
+        """
+        output = super().to_json_dict()
+        output['selected_value'] = self.get_selected_value()
+        return output
+
+
+@dataclass
+class NumRangeParameter(_NumericParameter):
+    """
+    Class to define attributes for number range slider (double-ended) parameter widgets.
+    """
+    selected_lower_value: Decimal
+    selected_upper_value: Decimal
+
+    def __init__(self, name: str, label: str, min_value: po.Number, max_value: po.Number, increment: po.Number = 1, 
+                 default_lower_value: po.Number = None, default_upper_value: po.Number = None, *, is_hidden: bool = False) -> None:
+        """
+        Constructor for NumberParameter class
+
+        Parameters:
+            name: The name of the parameter
+            label: The display label for the parameter
+            min_value: The minimum bound for selection. Can be of type Decimal, integer, or number parsable string
+            max_value: The maxixmum bound for selection. Can be of type Decimal, integer, or number parsable string
+            increment: The increment for allowable selections. Can be of type Decimal, integer, or number parsable string. Default is 1
+            default_lower_value: The default lower selection. Can be of type Decimal, integer, or number parsable string. Default is min_value
+            default_upper_value: The default upper selection. Can be of type Decimal, integer, or number parsable string. Default is max_value
+            is_hidden: Whether the parameter is hidden in the parameters API response. Default is False
+        """
+        default_lower_value = default_lower_value if default_lower_value is not None else min_value
+        default_upper_value = default_upper_value if default_upper_value is not None else max_value
+        curr_option = po.NumRangeParameterOption(min_value, max_value, increment, default_lower_value, default_upper_value)
+        all_options = (curr_option,)
+        super().__init__("NumRangeParameter", name, label, all_options, is_hidden, None, curr_option)
+        self._set_default_as_selection_mutate()
+    
+    @staticmethod
+    def WithParent(name: str, label: str, all_options: Sequence[po.NumRangeParameterOption], parent: SingleSelectParameter, *, 
+                   is_hidden: bool = False) -> DateParameter:
+        """
+        A factory method to construct a NumRangeParameter with a parent parameter
+
+        Parameters:
+            name: The name of the parameter
+            label: The display label for the parameter
+            all_options: A sequence of NumRangeParameterOption which contains various bounds and default values linked to specific parent options
+            parent: The parent parameter, which must be a SingleSelectParameter
+            is_hidden: Whether the parameter is hidden in the parameters API response. Default is False
+        """
+        new_param = NumRangeParameter(name, label, 0, 1, is_hidden=is_hidden) # dummy values
+        return Parameter.WithParent(all_options, parent, new_param)
+    
+    def with_selection(self, selection: str):
+        """
+        Applies the selected numbers to this widget parameter
+
+        Parameters:
+            selection: The lower and upper selected numbers joined by comma (with no spaces)
+        
+        Returns:
+            A new copy of NumRangeParameter with the selection applied
+        """
+        try:
+            lower, upper = selection.split(',')
+        except ValueError as e:
+            self._raise_invalid_input_error(selection, "Range parameter selection must be two numbers joined by comma.", e)
+
+        param_copy = copy.copy(self)
+        try:
+            param_copy.selected_lower_value = param_copy.curr_option._validate_value(lower)
+            param_copy.selected_upper_value = param_copy.curr_option._validate_value(upper, param_copy.selected_lower_value)
+        except u.ConfigurationError as e:
+            self._raise_invalid_input_error(selection, 'Invalid selection for range parameter.', e)
+        return param_copy
+
+    def get_selected_lower_value(self) -> str:
+        """
+        Get the selected lower number
+
+        Returns:
+            A number parsable string of the selected number
+        """
+        return str(self.selected_lower_value)
+
+    def get_selected_upper_value(self) -> str:
+        """
+        Get the selected upper number
+
+        Returns:
+            A number parsable string of the selected number
+        """
+        return str(self.selected_upper_value)
+    
+    def _set_default_as_selection_mutate(self) -> None:
+        self.curr_option: po.NumRangeParameterOption
+        self.selected_lower_value = self.curr_option.default_lower_value
+        self.selected_upper_value = self.curr_option.default_upper_value
+
+    def to_json_dict(self):
+        """
+        Converts this parameter as a JSON object for the parameters API response
+
+        Returns:
+            A dictionary for the JSON object
+        """
+        output = super().to_json_dict()
+        output['selected_lower_value'] = self.get_selected_lower_value()
+        output['selected_upper_value'] = self.get_selected_upper_value()
+        return output
+
+
+@dataclass
+class DataSourceParameter(Parameter):
+    """
+    Class for parameters that can use a lookup table to convert itself into another parameter
+    """
+    parameter_class: Type[Parameter]
+    data_source: DataSource
+    parent: Optional[Parameter] 
+
+    def __init__(self, parameter_class: Type[Parameter], name: str, label: str, data_source: DataSource, *, 
+                 is_hidden: bool = False, parent: Optional[Parameter] = None) -> None:
+        """
+        Constructor for DataSourceParameter, a Parameter that uses a DataSource to convert itself to another Parameter
+
+        Parameters:
+            parameter_class: The class of widget parameter to convert to
+            name: The name of the parameter
+            label: The display label for the parameter
+            data_source: The lookup table to use for this parameter
+            is_hidden: Whether the parameter is hidden in the parameters API response. Default is False
+            parent: The parent parameter that may cascade the options for this parameter. Default is no parent
+        """
+        super().__init__("DataSourceParameter", name, label, None, is_hidden, None)
+        self.parameter_class = parameter_class
+        self.data_source = data_source
+        self.parent = parent
+
+    def convert(self, df: pd.DataFrame) -> Parameter:
+        """
+        Method to convert this DataSourceParameter into another parameter
+
+        Parameters:
+            df: The dataframe containing the parameter options data
+
+        Returns:
+            The converted parameter
+        """
+        return self.data_source.convert(self, df)
+    
+    def to_json_dict(self) -> Dict:
+        """
+        Converts this parameter as a JSON object for the parameters API response
+
+        Returns:
+            A dictionary for the JSON object
+        """
+        output = super().to_json_dict()
+        output['widget_type'] = self.parameter_class.__name__
+        output['data_source'] = self.data_source.__dict__
+        return output
+
+
+# Types:
+SelectionParameter = Union[SingleSelectParameter, MultiSelectParameter]
+NumericParameter = Union[NumberParameter, NumRangeParameter]
```

### Comparing `squirrels-0.1.0/squirrels.egg-info/PKG-INFO` & `squirrels-0.1.1.post1/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,56 +1,56 @@
-Metadata-Version: 2.1
-Name: squirrels
-Version: 0.1.0
-Summary: Python Package for Configuring SQL Generating APIs
-Author: Tim Huang
-Author-email: tim.yuting@hotmail.com
-License: MIT
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Squirrels
-
-Squirrels is an API framework for creating REST APIs that generate sql queries & dataframes dynamically from query parameters. 
-
-## Setup
-
-First, install the library and all dependencies **in a new virtual environment**.
-
-```bash
-# create and activate virtual environment...
-pip install -e .
-```
-
-To confirm that the setup worked, run this to show the help page for all squirrels CLI commands:
-
-```bash
-squirrels -h
-```
-
-## Testing
-
-```
-python setup.py pytest
-```
-
-## Usage Documentation
-
-To learn about using the squirrels framework, check out the documentation website [here](https://squirrels-nest.github.io/squirrels-docs/).
-
-## Developer Guide
-
-From the root of the git repo, the source code can be found in the `squirrels` folder and unit tests can be found in the `tests` folder.
-
-To understand what a specific squirrels command line utility is doing, start from the `_command_line.py` file as your entry point.
-
-The library version is maintained in both the `setup.py` file (for the next release or release-candidate version) and the `squirrels/_version.py` file (for the next release version only).
-
-When a user initializes a squirrels project using `squirrels init`, the files are copied from the `squirrels/package_data/base_project` folder. The contents in the `database` subfolder were constructed from the scripts in the `database_elt` folder at the top level.
-
-For the Squirrels UI activated by `squirrels run`, the HTML, CSS, and Javascript files can be found in the `static` and `templates` subfolders of `squirrels/package_data`.
-
-## License
-
-Squirrels is released under the MIT license.
-
-See the file LICENSE for more details.
+Metadata-Version: 2.1
+Name: squirrels
+Version: 0.1.1.post1
+Summary: Squirrels - Configure REST APIs for BI Analytics
+Author: Tim Huang
+Author-email: tim.yuting@hotmail.com
+License: MIT
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Squirrels
+
+Squirrels is an API framework that lets you create REST APIs for dynamic BI analytics!
+
+## Setup
+
+First, install the library and all dependencies **in a new virtual environment**.
+
+```bash
+# create and activate virtual environment...
+pip install -e .
+```
+
+To confirm that the setup worked, run this to show the help page for all squirrels CLI commands:
+
+```bash
+squirrels -h
+```
+
+## Testing
+
+```
+python setup.py pytest
+```
+
+## Usage Documentation
+
+To learn about using the squirrels framework, check out the documentation website [here](https://squirrels-nest.github.io/squirrels-docs/).
+
+## Developer Guide
+
+From the root of the git repo, the source code can be found in the `squirrels` folder and unit tests can be found in the `tests` folder.
+
+To understand what a specific squirrels command line utility is doing, start from the `_command_line.py` file as your entry point.
+
+The library version is maintained in both the `setup.py` file (for the next release or release-candidate version) and the `squirrels/_version.py` file (for the next release version only).
+
+When a user initializes a squirrels project using `squirrels init`, the files are copied from the `squirrels/package_data/base_project` folder. The contents in the `database` subfolder were constructed from the scripts in the `database_elt` folder at the top level.
+
+For the Squirrels UI activated by `squirrels run`, the HTML, CSS, and Javascript files can be found in the `static` and `templates` subfolders of `squirrels/package_data`.
+
+## License
+
+Squirrels is released under the MIT license.
+
+See the file LICENSE for more details.
```

### Comparing `squirrels-0.1.0/squirrels.egg-info/SOURCES.txt` & `squirrels-0.1.1.post1/squirrels.egg-info/SOURCES.txt`

 * *Files identical despite different names*

