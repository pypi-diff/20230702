# Comparing `tmp/cookieslicer-0.1.0.tar.gz` & `tmp/cookieslicer-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cookieslicer-0.1.0.tar", last modified: Sun Jul  2 02:36:35 2023, max compression
+gzip compressed data, was "cookieslicer-0.1.2.tar", last modified: Sun Jul  2 18:35:21 2023, max compression
```

## Comparing `cookieslicer-0.1.0.tar` & `cookieslicer-0.1.2.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxrwx   0        0        0        0 2023-07-02 02:36:35.472016 cookieslicer-0.1.0/
--rw-rw-rw-   0        0        0     1066 2023-05-22 04:17:06.000000 cookieslicer-0.1.0/LICENSE.txt
--rw-rw-rw-   0        0        0       65 2023-05-22 04:17:06.000000 cookieslicer-0.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0     6583 2023-07-02 02:36:35.472016 cookieslicer-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     5596 2023-07-02 02:04:29.000000 cookieslicer-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-02 02:36:35.425014 cookieslicer-0.1.0/cookieslicer/
--rw-rw-rw-   0        0        0        0 2023-05-22 04:17:06.000000 cookieslicer-0.1.0/cookieslicer/__init__.py
--rw-rw-rw-   0        0        0      398 2023-06-18 21:35:26.000000 cookieslicer-0.1.0/cookieslicer/__main__.py
--rw-rw-rw-   0        0        0      441 2023-07-01 18:35:07.000000 cookieslicer-0.1.0/cookieslicer/application_base_argument_parser.py
--rw-rw-rw-   0        0        0      281 2023-07-02 02:04:15.000000 cookieslicer-0.1.0/cookieslicer/application_return_code.py
--rw-rw-rw-   0        0        0     2982 2023-07-02 02:34:42.000000 cookieslicer-0.1.0/cookieslicer/cookieslicer.py
--rw-rw-rw-   0        0        0     3928 2023-07-02 02:04:07.000000 cookieslicer-0.1.0/cookieslicer/cookieslicer_argument_parser.py
--rw-rw-rw-   0        0        0     1749 2023-06-26 00:19:55.000000 cookieslicer-0.1.0/cookieslicer/cookieslicer_configuration.py
--rw-rw-rw-   0        0        0     1657 2023-07-01 21:15:56.000000 cookieslicer-0.1.0/cookieslicer/cookieslicer_constants.py
--rw-rw-rw-   0        0        0    26489 2023-07-01 23:00:08.000000 cookieslicer-0.1.0/cookieslicer/cookieslicer_processor.py
--rw-rw-rw-   0        0        0     1994 2023-05-28 16:58:10.000000 cookieslicer-0.1.0/cookieslicer/cookieslicer_template.py
--rw-rw-rw-   0        0        0     4167 2023-07-02 01:48:31.000000 cookieslicer-0.1.0/cookieslicer/main.py
--rw-rw-rw-   0        0        0       13 2023-05-22 04:17:06.000000 cookieslicer-0.1.0/cookieslicer/py.typed
--rw-rw-rw-   0        0        0      178 2023-06-29 23:45:50.000000 cookieslicer-0.1.0/cookieslicer/version.py
-drwxrwxrwx   0        0        0        0 2023-07-02 02:36:35.456014 cookieslicer-0.1.0/cookieslicer.egg-info/
--rw-rw-rw-   0        0        0     6583 2023-07-02 02:36:35.000000 cookieslicer-0.1.0/cookieslicer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      989 2023-07-02 02:36:35.000000 cookieslicer-0.1.0/cookieslicer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-02 02:36:35.000000 cookieslicer-0.1.0/cookieslicer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2023-07-02 02:36:35.000000 cookieslicer-0.1.0/cookieslicer.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       37 2023-07-02 02:36:35.000000 cookieslicer-0.1.0/cookieslicer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-07-02 02:36:35.000000 cookieslicer-0.1.0/cookieslicer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       39 2023-07-02 02:04:29.000000 cookieslicer-0.1.0/install-requirements.txt
--rw-rw-rw-   0        0        0       90 2023-07-01 15:18:41.000000 cookieslicer-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0      783 2023-07-02 02:36:35.474019 cookieslicer-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     3159 2023-07-02 02:04:29.000000 cookieslicer-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-02 02:36:35.470016 cookieslicer-0.1.0/test/
--rw-rw-rw-   0        0        0     6499 2023-07-01 21:04:17.000000 cookieslicer-0.1.0/test/test_attention.py
--rw-rw-rw-   0        0        0    29189 2023-07-01 21:04:17.000000 cookieslicer-0.1.0/test/test_complex.py
--rw-rw-rw-   0        0        0     2223 2023-07-01 21:15:56.000000 cookieslicer-0.1.0/test/test_extra.py
--rw-rw-rw-   0        0        0    21263 2023-07-01 21:15:56.000000 cookieslicer-0.1.0/test/test_general_failures.py
--rw-rw-rw-   0        0        0    14865 2023-07-01 21:04:17.000000 cookieslicer-0.1.0/test/test_generate_config.py
--rw-rw-rw-   0        0        0     3571 2023-07-01 23:17:38.000000 cookieslicer-0.1.0/test/test_help.py
--rw-rw-rw-   0        0        0     4465 2023-07-01 21:04:17.000000 cookieslicer-0.1.0/test/test_once.py
--rw-rw-rw-   0        0        0     4702 2023-07-01 21:04:17.000000 cookieslicer-0.1.0/test/test_pipfile.py
--rw-rw-rw-   0        0        0     7599 2023-07-01 21:04:17.000000 cookieslicer-0.1.0/test/test_remove.py
--rw-rw-rw-   0        0        0    15804 2023-07-01 21:04:17.000000 cookieslicer-0.1.0/test/test_simple.py
--rw-rw-rw-   0        0        0      508 2023-05-22 04:17:06.000000 cookieslicer-0.1.0/test/test_version.py
+drwxrwxrwx   0        0        0        0 2023-07-02 18:35:21.288839 cookieslicer-0.1.2/
+-rw-rw-rw-   0        0        0     1066 2023-05-22 04:17:06.000000 cookieslicer-0.1.2/LICENSE.txt
+-rw-rw-rw-   0        0        0       65 2023-05-22 04:17:06.000000 cookieslicer-0.1.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     8923 2023-07-02 18:35:21.288839 cookieslicer-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     7936 2023-07-02 15:35:37.000000 cookieslicer-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-02 18:35:21.263839 cookieslicer-0.1.2/cookieslicer/
+-rw-rw-rw-   0        0        0        0 2023-05-22 04:17:06.000000 cookieslicer-0.1.2/cookieslicer/__init__.py
+-rw-rw-rw-   0        0        0      398 2023-06-18 21:35:26.000000 cookieslicer-0.1.2/cookieslicer/__main__.py
+-rw-rw-rw-   0        0        0      441 2023-07-01 18:35:07.000000 cookieslicer-0.1.2/cookieslicer/application_base_argument_parser.py
+-rw-rw-rw-   0        0        0      281 2023-07-02 15:35:37.000000 cookieslicer-0.1.2/cookieslicer/application_return_code.py
+-rw-rw-rw-   0        0        0     2982 2023-07-02 15:35:37.000000 cookieslicer-0.1.2/cookieslicer/cookieslicer.py
+-rw-rw-rw-   0        0        0     3928 2023-07-02 15:35:37.000000 cookieslicer-0.1.2/cookieslicer/cookieslicer_argument_parser.py
+-rw-rw-rw-   0        0        0     1749 2023-06-26 00:19:55.000000 cookieslicer-0.1.2/cookieslicer/cookieslicer_configuration.py
+-rw-rw-rw-   0        0        0     1657 2023-07-01 21:15:56.000000 cookieslicer-0.1.2/cookieslicer/cookieslicer_constants.py
+-rw-rw-rw-   0        0        0    26489 2023-07-01 23:00:08.000000 cookieslicer-0.1.2/cookieslicer/cookieslicer_processor.py
+-rw-rw-rw-   0        0        0     1994 2023-05-28 16:58:10.000000 cookieslicer-0.1.2/cookieslicer/cookieslicer_template.py
+-rw-rw-rw-   0        0        0     4167 2023-07-02 01:48:31.000000 cookieslicer-0.1.2/cookieslicer/main.py
+-rw-rw-rw-   0        0        0       13 2023-05-22 04:17:06.000000 cookieslicer-0.1.2/cookieslicer/py.typed
+-rw-rw-rw-   0        0        0      178 2023-07-02 18:34:58.000000 cookieslicer-0.1.2/cookieslicer/version.py
+drwxrwxrwx   0        0        0        0 2023-07-02 18:35:21.271840 cookieslicer-0.1.2/cookieslicer.egg-info/
+-rw-rw-rw-   0        0        0     8923 2023-07-02 18:35:21.000000 cookieslicer-0.1.2/cookieslicer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      989 2023-07-02 18:35:21.000000 cookieslicer-0.1.2/cookieslicer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-02 18:35:21.000000 cookieslicer-0.1.2/cookieslicer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2023-07-02 18:35:21.000000 cookieslicer-0.1.2/cookieslicer.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       66 2023-07-02 18:35:21.000000 cookieslicer-0.1.2/cookieslicer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-02 18:35:21.000000 cookieslicer-0.1.2/cookieslicer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       69 2023-07-02 18:34:31.000000 cookieslicer-0.1.2/install-requirements.txt
+-rw-rw-rw-   0        0        0       90 2023-07-01 15:18:41.000000 cookieslicer-0.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0      783 2023-07-02 18:35:21.289838 cookieslicer-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     3163 2023-07-02 16:16:51.000000 cookieslicer-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-02 18:35:21.287840 cookieslicer-0.1.2/test/
+-rw-rw-rw-   0        0        0     6499 2023-07-01 21:04:17.000000 cookieslicer-0.1.2/test/test_attention.py
+-rw-rw-rw-   0        0        0    29189 2023-07-01 21:04:17.000000 cookieslicer-0.1.2/test/test_complex.py
+-rw-rw-rw-   0        0        0     2223 2023-07-01 21:15:56.000000 cookieslicer-0.1.2/test/test_extra.py
+-rw-rw-rw-   0        0        0    21263 2023-07-01 21:15:56.000000 cookieslicer-0.1.2/test/test_general_failures.py
+-rw-rw-rw-   0        0        0    14865 2023-07-01 21:04:17.000000 cookieslicer-0.1.2/test/test_generate_config.py
+-rw-rw-rw-   0        0        0     3571 2023-07-01 23:17:38.000000 cookieslicer-0.1.2/test/test_help.py
+-rw-rw-rw-   0        0        0     4465 2023-07-01 21:04:17.000000 cookieslicer-0.1.2/test/test_once.py
+-rw-rw-rw-   0        0        0     4702 2023-07-01 21:04:17.000000 cookieslicer-0.1.2/test/test_pipfile.py
+-rw-rw-rw-   0        0        0     7599 2023-07-01 21:04:17.000000 cookieslicer-0.1.2/test/test_remove.py
+-rw-rw-rw-   0        0        0    15804 2023-07-01 21:04:17.000000 cookieslicer-0.1.2/test/test_simple.py
+-rw-rw-rw-   0        0        0      508 2023-05-22 04:17:06.000000 cookieslicer-0.1.2/test/test_version.py
```

### Comparing `cookieslicer-0.1.0/LICENSE.txt` & `cookieslicer-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cookieslicer-0.1.0/PKG-INFO` & `cookieslicer-0.1.2/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,41 +1,50 @@
-Metadata-Version: 2.1
-Name: cookieslicer
-Version: 0.1.0
-Summary: Apply advanced templating by smartly using CookieCutter.
-Home-page: https://github.com/jackdewinter/cookieslicer
-Author: Jack De Winter
-Author-email: jack.de.winter@outlook.com
-Maintainer: Jack De Winter
-Maintainer-email: jack.de.winter@outlook.com
-Project-URL: Change Log, https://github.com/jackdewinter/cookieslicer/blob/main/changelog.md
-Keywords: cookiecutter
-Classifier: Development Status :: 4 - Beta
-Classifier: Environment :: Console
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Natural Language :: English
-Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
-Requires-Python: >=3.8.0
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
 # Library Package: cookieslicer
 
 |   |   |
 |---|---|
 |Project|[![Version](https://img.shields.io/pypi/v/cookieslicer.svg)](https://pypi.org/project/cookieslicer)  [![Python Versions](https://img.shields.io/pypi/pyversions/cookieslicer.svg)](https://pypi.org/project/cookieslicer)  ![platforms](https://img.shields.io/badge/platform-windows%20%7C%20macos%20%7C%20linux-lightgrey)  [![License](https://img.shields.io/github/license/jackdewinter/cookieslicer.svg)](https://github.com/jackdewinter/cookieslicer/blob/main/LICENSE.txt)  [![GitHub top language](https://img.shields.io/github/languages/top/jackdewinter/cookieslicer)](https://github.com/jackdewinter/cookieslicer)|
 |Quality|[![GitHub Workflow Status (event)](https://img.shields.io/github/workflow/status/jackdewinter/cookieslicer/Main)](https://github.com/jackdewinter/cookieslicer/actions/workflows/main.yml)  [![Issues](https://img.shields.io/github/issues/jackdewinter/cookieslicer.svg)](https://github.com/jackdewinter/cookieslicer/issues)  [![codecov](https://codecov.io/gh/jackdewinter/cookieslicer/branch/main/graph/badge.svg?token=PD5TKS8NQQ)](https://codecov.io/gh/jackdewinter/cookieslicer)  [![Sourcery](https://img.shields.io/badge/Sourcery-enabled-brightgreen)](https://sourcery.ai)  ![snyk](https://img.shields.io/snyk/vulnerabilities/github/jackdewinter/cookieslicer) |
 |  |![GitHub Pipenv locked dependency version (branch)](https://img.shields.io/github/pipenv/locked/dependency-version/jackdewinter/cookieslicer/black/main)  ![GitHub Pipenv locked dependency version (branch)](https://img.shields.io/github/pipenv/locked/dependency-version/jackdewinter/cookieslicer/flake8/main)  ![GitHub Pipenv locked dependency version (branch)](https://img.shields.io/github/pipenv/locked/dependency-version/jackdewinter/cookieslicer/pylint/main)  ![GitHub Pipenv locked dependency version (branch)](https://img.shields.io/github/pipenv/locked/dependency-version/jackdewinter/cookieslicer/mypy/main)  ![GitHub Pipenv locked dependency version (branch)](https://img.shields.io/github/pipenv/locked/dependency-version/jackdewinter/cookieslicer/pyroma/main)  ![GitHub Pipenv locked dependency version (branch)](https://img.shields.io/github/pipenv/locked/dependency-version/jackdewinter/cookieslicer/pre-commit/main)|
 |Community|[![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://github.com/jackdewinter/cookieslicer/graphs/commit-activity) [![Stars](https://img.shields.io/github/stars/jackdewinter/cookieslicer.svg)](https://github.com/jackdewinter/cookieslicer/stargazers)  [![Forks](https://img.shields.io/github/forks/jackdewinter/cookieslicer.svg)](https://github.com/jackdewinter/cookieslicer/network/members)  [![Contributors](https://img.shields.io/github/contributors/jackdewinter/cookieslicer.svg)](https://github.com/jackdewinter/cookieslicer/graphs/contributors)  [![Downloads](https://img.shields.io/pypi/dm/cookieslicer.svg)](https://pypistats.org/packages/cookieslicer)|
 |Maintainers|[![LinkedIn](https://img.shields.io/badge/-LinkedIn-black.svg?logo=linkedin&colorB=555)](https://www.linkedin.com/in/jackdewinter/)|
 
+The cookieslicer project was born out of a simple need: to have a templating system
+that we could apply multiple times as our knowledge grew.  With multiple open source
+projects being maintained, it was becoming difficult to remember which versions
+of which files were "the best".  While the [cookiecutter](https://github.com/cookiecutter/cookiecutter)
+project is a good first step to solving these problems, we felt it needed something
+in front of it to help control the templating.
+
+The cookieslicer application adds three files to a project that assist it in maintaining
+good templates.  The source directory is the location of the template to be applied,
+and contains a `cookieslicer.json` file that gives addition instructions on how
+to handle certain situations that arise when re-applying a template.  The output
+directory is the location that the template is applied to.  This directory contains
+a `cookiecutter-config.yaml` that is applied to the template in the source directory
+using `cookiecutter`.  This directory also contains a `cookieslicer.json` file with
+configuration information for the cookieslicer application.
+
+The rest of the process is (mostly) simple.  Cookieslicer uses the `cookiecutter-config.yaml`
+file and the source directory to generate a completed template in a temporary directory.
+With that template including the source directory's `cookieslicer.json` file, cookieslicer
+then checks to see if the source directory's template version is the same as the
+output directory's template version, quickly exitting if they are the same.  Otherwise,
+the source directory's `cookieslicer.json` file tells Cookieslicer how to alter files
+in the output directory.
+
+Outside of a normal file copy, there are three different modes in which this happens.
+The `once` mode instructs Cookieslicer to only copy a file if it does not exist
+in the output directory.  The `attention` mode instructs Cookieslicer to copy the
+file if it is different and to place it on an attention list.  This list is relayed
+to the end-user at the end of the templating.  Finally, the `remove` mode instructs
+Cookieslicer to remove a file with a specific path from the output directory. While
+we are not sure if this is a complete list of actions to take, we feel that it was
+a good enough list to start with.
+
 ## Requirements
 
 This project required Python 3.8 or later to function.
 
 ## Installation
 
 ```sh
```

### Comparing `cookieslicer-0.1.0/cookieslicer/cookieslicer.py` & `cookieslicer-0.1.2/cookieslicer/cookieslicer.py`

 * *Files identical despite different names*

### Comparing `cookieslicer-0.1.0/cookieslicer/cookieslicer_argument_parser.py` & `cookieslicer-0.1.2/cookieslicer/cookieslicer_argument_parser.py`

 * *Files identical despite different names*

### Comparing `cookieslicer-0.1.0/cookieslicer/cookieslicer_configuration.py` & `cookieslicer-0.1.2/cookieslicer/cookieslicer_configuration.py`

 * *Files identical despite different names*

### Comparing `cookieslicer-0.1.0/cookieslicer/cookieslicer_constants.py` & `cookieslicer-0.1.2/cookieslicer/cookieslicer_constants.py`

 * *Files identical despite different names*

### Comparing `cookieslicer-0.1.0/cookieslicer/cookieslicer_processor.py` & `cookieslicer-0.1.2/cookieslicer/cookieslicer_processor.py`

 * *Files identical despite different names*

### Comparing `cookieslicer-0.1.0/cookieslicer/cookieslicer_template.py` & `cookieslicer-0.1.2/cookieslicer/cookieslicer_template.py`

 * *Files identical despite different names*

### Comparing `cookieslicer-0.1.0/cookieslicer/main.py` & `cookieslicer-0.1.2/cookieslicer/main.py`

 * *Files identical despite different names*

### Comparing `cookieslicer-0.1.0/cookieslicer.egg-info/PKG-INFO` & `cookieslicer-0.1.2/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cookieslicer
-Version: 0.1.0
+Version: 0.1.2
 Summary: Apply advanced templating by smartly using CookieCutter.
 Home-page: https://github.com/jackdewinter/cookieslicer
 Author: Jack De Winter
 Author-email: jack.de.winter@outlook.com
 Maintainer: Jack De Winter
 Maintainer-email: jack.de.winter@outlook.com
 Project-URL: Change Log, https://github.com/jackdewinter/cookieslicer/blob/main/changelog.md
@@ -28,14 +28,47 @@
 |---|---|
 |Project|[![Version](https://img.shields.io/pypi/v/cookieslicer.svg)](https://pypi.org/project/cookieslicer)  [![Python Versions](https://img.shields.io/pypi/pyversions/cookieslicer.svg)](https://pypi.org/project/cookieslicer)  ![platforms](https://img.shields.io/badge/platform-windows%20%7C%20macos%20%7C%20linux-lightgrey)  [![License](https://img.shields.io/github/license/jackdewinter/cookieslicer.svg)](https://github.com/jackdewinter/cookieslicer/blob/main/LICENSE.txt)  [![GitHub top language](https://img.shields.io/github/languages/top/jackdewinter/cookieslicer)](https://github.com/jackdewinter/cookieslicer)|
 |Quality|[![GitHub Workflow Status (event)](https://img.shields.io/github/workflow/status/jackdewinter/cookieslicer/Main)](https://github.com/jackdewinter/cookieslicer/actions/workflows/main.yml)  [![Issues](https://img.shields.io/github/issues/jackdewinter/cookieslicer.svg)](https://github.com/jackdewinter/cookieslicer/issues)  [![codecov](https://codecov.io/gh/jackdewinter/cookieslicer/branch/main/graph/badge.svg?token=PD5TKS8NQQ)](https://codecov.io/gh/jackdewinter/cookieslicer)  [![Sourcery](https://img.shields.io/badge/Sourcery-enabled-brightgreen)](https://sourcery.ai)  ![snyk](https://img.shields.io/snyk/vulnerabilities/github/jackdewinter/cookieslicer) |
 |  |![GitHub Pipenv locked dependency version (branch)](https://img.shields.io/github/pipenv/locked/dependency-version/jackdewinter/cookieslicer/black/main)  ![GitHub Pipenv locked dependency version (branch)](https://img.shields.io/github/pipenv/locked/dependency-version/jackdewinter/cookieslicer/flake8/main)  ![GitHub Pipenv locked dependency version (branch)](https://img.shields.io/github/pipenv/locked/dependency-version/jackdewinter/cookieslicer/pylint/main)  ![GitHub Pipenv locked dependency version (branch)](https://img.shields.io/github/pipenv/locked/dependency-version/jackdewinter/cookieslicer/mypy/main)  ![GitHub Pipenv locked dependency version (branch)](https://img.shields.io/github/pipenv/locked/dependency-version/jackdewinter/cookieslicer/pyroma/main)  ![GitHub Pipenv locked dependency version (branch)](https://img.shields.io/github/pipenv/locked/dependency-version/jackdewinter/cookieslicer/pre-commit/main)|
 |Community|[![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://github.com/jackdewinter/cookieslicer/graphs/commit-activity) [![Stars](https://img.shields.io/github/stars/jackdewinter/cookieslicer.svg)](https://github.com/jackdewinter/cookieslicer/stargazers)  [![Forks](https://img.shields.io/github/forks/jackdewinter/cookieslicer.svg)](https://github.com/jackdewinter/cookieslicer/network/members)  [![Contributors](https://img.shields.io/github/contributors/jackdewinter/cookieslicer.svg)](https://github.com/jackdewinter/cookieslicer/graphs/contributors)  [![Downloads](https://img.shields.io/pypi/dm/cookieslicer.svg)](https://pypistats.org/packages/cookieslicer)|
 |Maintainers|[![LinkedIn](https://img.shields.io/badge/-LinkedIn-black.svg?logo=linkedin&colorB=555)](https://www.linkedin.com/in/jackdewinter/)|
 
+The cookieslicer project was born out of a simple need: to have a templating system
+that we could apply multiple times as our knowledge grew.  With multiple open source
+projects being maintained, it was becoming difficult to remember which versions
+of which files were "the best".  While the [cookiecutter](https://github.com/cookiecutter/cookiecutter)
+project is a good first step to solving these problems, we felt it needed something
+in front of it to help control the templating.
+
+The cookieslicer application adds three files to a project that assist it in maintaining
+good templates.  The source directory is the location of the template to be applied,
+and contains a `cookieslicer.json` file that gives addition instructions on how
+to handle certain situations that arise when re-applying a template.  The output
+directory is the location that the template is applied to.  This directory contains
+a `cookiecutter-config.yaml` that is applied to the template in the source directory
+using `cookiecutter`.  This directory also contains a `cookieslicer.json` file with
+configuration information for the cookieslicer application.
+
+The rest of the process is (mostly) simple.  Cookieslicer uses the `cookiecutter-config.yaml`
+file and the source directory to generate a completed template in a temporary directory.
+With that template including the source directory's `cookieslicer.json` file, cookieslicer
+then checks to see if the source directory's template version is the same as the
+output directory's template version, quickly exitting if they are the same.  Otherwise,
+the source directory's `cookieslicer.json` file tells Cookieslicer how to alter files
+in the output directory.
+
+Outside of a normal file copy, there are three different modes in which this happens.
+The `once` mode instructs Cookieslicer to only copy a file if it does not exist
+in the output directory.  The `attention` mode instructs Cookieslicer to copy the
+file if it is different and to place it on an attention list.  This list is relayed
+to the end-user at the end of the templating.  Finally, the `remove` mode instructs
+Cookieslicer to remove a file with a specific path from the output directory. While
+we are not sure if this is a complete list of actions to take, we feel that it was
+a good enough list to start with.
+
 ## Requirements
 
 This project required Python 3.8 or later to function.
 
 ## Installation
 
 ```sh
```

### Comparing `cookieslicer-0.1.0/cookieslicer.egg-info/SOURCES.txt` & `cookieslicer-0.1.2/cookieslicer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cookieslicer-0.1.0/setup.cfg` & `cookieslicer-0.1.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `cookieslicer-0.1.0/setup.py` & `cookieslicer-0.1.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -76,14 +76,16 @@
     "Programming Language :: Python :: 3.9",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Natural Language :: English",
     "Topic :: Software Development :: Libraries :: Application Frameworks",
 ]
 
+x = ["cookieslicer"]
+
 setup(
     name=PACKAGE_NAME,
     version=SEMANTIC_VERSION,
     python_requires=f">={MINIMUM_PYTHON_VERSION}",
     install_requires=parse_requirements(),
     author=AUTHOR,
     author_email=AUTHOR_EMAIL,
@@ -97,11 +99,11 @@
     classifiers=PROJECT_CLASSIFIERS,
     project_urls=PROJECT_URLS,
     entry_points={
         "console_scripts": [
             "cookieslicer=cookieslicer.__main__:main",
         ]
     },
-    packages=get_package_modules(),
+    packages=x,
     include_package_data=True,
     package_data={"": ["*.typed"]},
 )
```

### Comparing `cookieslicer-0.1.0/test/test_attention.py` & `cookieslicer-0.1.2/test/test_attention.py`

 * *Files identical despite different names*

### Comparing `cookieslicer-0.1.0/test/test_complex.py` & `cookieslicer-0.1.2/test/test_complex.py`

 * *Files identical despite different names*

### Comparing `cookieslicer-0.1.0/test/test_extra.py` & `cookieslicer-0.1.2/test/test_extra.py`

 * *Files identical despite different names*

### Comparing `cookieslicer-0.1.0/test/test_general_failures.py` & `cookieslicer-0.1.2/test/test_general_failures.py`

 * *Files identical despite different names*

### Comparing `cookieslicer-0.1.0/test/test_generate_config.py` & `cookieslicer-0.1.2/test/test_generate_config.py`

 * *Files identical despite different names*

### Comparing `cookieslicer-0.1.0/test/test_help.py` & `cookieslicer-0.1.2/test/test_help.py`

 * *Files identical despite different names*

### Comparing `cookieslicer-0.1.0/test/test_once.py` & `cookieslicer-0.1.2/test/test_once.py`

 * *Files identical despite different names*

### Comparing `cookieslicer-0.1.0/test/test_pipfile.py` & `cookieslicer-0.1.2/test/test_pipfile.py`

 * *Files identical despite different names*

### Comparing `cookieslicer-0.1.0/test/test_remove.py` & `cookieslicer-0.1.2/test/test_remove.py`

 * *Files identical despite different names*

### Comparing `cookieslicer-0.1.0/test/test_simple.py` & `cookieslicer-0.1.2/test/test_simple.py`

 * *Files identical despite different names*

