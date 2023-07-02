# Comparing `tmp/pip-tree-2.1.0.tar.gz` & `tmp/pip-tree-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pip-tree-2.1.0.tar", last modified: Sat Mar 25 21:33:12 2023, max compression
+gzip compressed data, was "pip-tree-3.0.0.tar", last modified: Sun Jul  2 02:37:04 2023, max compression
```

## Comparing `pip-tree-2.1.0.tar` & `pip-tree-3.0.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 21:33:12.080446 pip-tree-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-03-25 21:32:46.000000 pip-tree-2.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3590 2023-03-25 21:33:12.080446 pip-tree-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-03-25 21:32:46.000000 pip-tree-2.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 21:33:12.080446 pip-tree-2.1.0/pip_tree/
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-03-25 21:32:46.000000 pip-tree-2.1.0/pip_tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-03-25 21:32:46.000000 pip-tree-2.1.0/pip_tree/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-25 21:32:46.000000 pip-tree-2.1.0/pip_tree/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-03-25 21:32:46.000000 pip-tree-2.1.0/pip_tree/tree.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 21:33:12.080446 pip-tree-2.1.0/pip_tree.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3590 2023-03-25 21:33:12.000000 pip-tree-2.1.0/pip_tree.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-03-25 21:33:12.000000 pip-tree-2.1.0/pip_tree.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-25 21:33:12.000000 pip-tree-2.1.0/pip_tree.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-03-25 21:33:12.000000 pip-tree-2.1.0/pip_tree.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-03-25 21:33:12.000000 pip-tree-2.1.0/pip_tree.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-03-25 21:33:12.000000 pip-tree-2.1.0/pip_tree.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-03-25 21:32:46.000000 pip-tree-2.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-25 21:33:12.080446 pip-tree-2.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-03-25 21:32:46.000000 pip-tree-2.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 21:33:12.080446 pip-tree-2.1.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-25 21:32:46.000000 pip-tree-2.1.0/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 21:33:12.080446 pip-tree-2.1.0/test/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-25 21:32:46.000000 pip-tree-2.1.0/test/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-03-25 21:32:46.000000 pip-tree-2.1.0/test/unit/test_tree.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 02:37:04.322536 pip-tree-3.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-02 02:36:31.000000 pip-tree-3.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-07-02 02:37:04.322536 pip-tree-3.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-07-02 02:36:31.000000 pip-tree-3.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 02:37:04.318536 pip-tree-3.0.0/pip_tree/
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-02 02:36:31.000000 pip-tree-3.0.0/pip_tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-07-02 02:36:31.000000 pip-tree-3.0.0/pip_tree/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 02:36:31.000000 pip-tree-3.0.0/pip_tree/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-07-02 02:36:31.000000 pip-tree-3.0.0/pip_tree/tree.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 02:37:04.322536 pip-tree-3.0.0/pip_tree.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-07-02 02:37:04.000000 pip-tree-3.0.0/pip_tree.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-02 02:37:04.000000 pip-tree-3.0.0/pip_tree.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 02:37:04.000000 pip-tree-3.0.0/pip_tree.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-02 02:37:04.000000 pip-tree-3.0.0/pip_tree.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-02 02:37:04.000000 pip-tree-3.0.0/pip_tree.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-02 02:37:04.000000 pip-tree-3.0.0/pip_tree.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-02 02:36:31.000000 pip-tree-3.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 02:37:04.322536 pip-tree-3.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-07-02 02:36:31.000000 pip-tree-3.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 02:37:04.322536 pip-tree-3.0.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 02:36:31.000000 pip-tree-3.0.0/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 02:37:04.322536 pip-tree-3.0.0/test/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 02:36:31.000000 pip-tree-3.0.0/test/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-02 02:36:31.000000 pip-tree-3.0.0/test/unit/test_tree.py
```

### Comparing `pip-tree-2.1.0/LICENSE` & `pip-tree-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pip-tree-2.1.0/PKG-INFO` & `pip-tree-3.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: pip-tree
-Version: 2.1.0
+Version: 3.0.0
 Summary: Get the dependency tree of your Python virtual environment via Pip.
 Home-page: http://github.com/justintime50/pip-tree
 Author: Justintime50
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7, <4
+Requires-Python: >=3.8, <4
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 <div align="center">
 
 # Pip Tree
@@ -36,15 +36,15 @@
 # Install Pip Tree globally
 pip3 install pip-tree
 
 # Install Pip Tree into the virtual environment of the project you want to run it on
 venv/bin/pip install pip-tree
 
 # Install locally
-make install
+just install
 ```
 
 ## Usage
 
 ```text
 Virtual Env Usage:
     pip-tree
@@ -115,9 +115,9 @@
     print(package_details['name'])
 ```
 
 ## Development
 
 ```bash
 # Get a comprehensive list of development tools
-make help
+just --list
 ```
```

### Comparing `pip-tree-2.1.0/README.md` & `pip-tree-3.0.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 # Install Pip Tree globally
 pip3 install pip-tree
 
 # Install Pip Tree into the virtual environment of the project you want to run it on
 venv/bin/pip install pip-tree
 
 # Install locally
-make install
+just install
 ```
 
 ## Usage
 
 ```text
 Virtual Env Usage:
     pip-tree
@@ -100,9 +100,9 @@
     print(package_details['name'])
 ```
 
 ## Development
 
 ```bash
 # Get a comprehensive list of development tools
-make help
+just --list
 ```
```

### Comparing `pip-tree-2.1.0/pip_tree/cli.py` & `pip-tree-3.0.0/pip_tree/cli.py`

 * *Files identical despite different names*

### Comparing `pip-tree-2.1.0/pip_tree/tree.py` & `pip-tree-3.0.0/pip_tree/tree.py`

 * *Files identical despite different names*

### Comparing `pip-tree-2.1.0/pip_tree.egg-info/PKG-INFO` & `pip-tree-3.0.0/pip_tree.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: pip-tree
-Version: 2.1.0
+Version: 3.0.0
 Summary: Get the dependency tree of your Python virtual environment via Pip.
 Home-page: http://github.com/justintime50/pip-tree
 Author: Justintime50
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7, <4
+Requires-Python: >=3.8, <4
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 <div align="center">
 
 # Pip Tree
@@ -36,15 +36,15 @@
 # Install Pip Tree globally
 pip3 install pip-tree
 
 # Install Pip Tree into the virtual environment of the project you want to run it on
 venv/bin/pip install pip-tree
 
 # Install locally
-make install
+just install
 ```
 
 ## Usage
 
 ```text
 Virtual Env Usage:
     pip-tree
@@ -115,9 +115,9 @@
     print(package_details['name'])
 ```
 
 ## Development
 
 ```bash
 # Get a comprehensive list of development tools
-make help
+just --list
 ```
```

### Comparing `pip-tree-2.1.0/setup.py` & `pip-tree-3.0.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,28 +2,28 @@
 
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 DEV_REQUIREMENTS = [
     'bandit == 1.7.*',
-    'black == 22.*',
+    'black == 23.*',
     'build == 0.10.*',
-    'flake8 == 5.*',
+    'flake8 == 6.*',
     'isort == 5.*',
-    'mypy == 1.1.*',
+    'mypy == 1.3.*',
     'pytest == 7.*',
     'pytest-cov == 4.*',
     'twine == 4.*',
     'types-setuptools',
 ]
 
 setuptools.setup(
     name='pip-tree',
-    version='2.1.0',
+    version='3.0.0',
     description='Get the dependency tree of your Python virtual environment via Pip.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='http://github.com/justintime50/pip-tree',
     author='Justintime50',
     license='MIT',
     packages=setuptools.find_packages(),
@@ -37,9 +37,9 @@
         'dev': DEV_REQUIREMENTS,
     },
     entry_points={
         'console_scripts': [
             'pip-tree=pip_tree.cli:main',
         ],
     },
-    python_requires='>=3.7, <4',
+    python_requires='>=3.8, <4',
 )
```

