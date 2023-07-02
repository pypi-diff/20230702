# Comparing `tmp/forks-sync-3.0.5.tar.gz` & `tmp/forks-sync-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "forks-sync-3.0.5.tar", last modified: Thu Mar 30 17:30:17 2023, max compression
+gzip compressed data, was "forks-sync-4.0.0.tar", last modified: Sun Jul  2 02:30:02 2023, max compression
```

## Comparing `forks-sync-3.0.5.tar` & `forks-sync-4.0.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 17:30:17.094869 forks-sync-3.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-03-30 17:29:38.000000 forks-sync-3.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-03-30 17:30:17.094869 forks-sync-3.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-03-30 17:29:38.000000 forks-sync-3.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 17:30:17.090870 forks-sync-3.0.5/forks_sync/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-03-30 17:29:38.000000 forks-sync-3.0.5/forks_sync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-03-30 17:29:38.000000 forks-sync-3.0.5/forks_sync/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-03-30 17:29:38.000000 forks-sync-3.0.5/forks_sync/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 17:29:38.000000 forks-sync-3.0.5/forks_sync/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     6370 2023-03-30 17:29:38.000000 forks-sync-3.0.5/forks_sync/sync.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 17:30:17.094869 forks-sync-3.0.5/forks_sync.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-03-30 17:30:17.000000 forks-sync-3.0.5/forks_sync.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-03-30 17:30:17.000000 forks-sync-3.0.5/forks_sync.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-30 17:30:17.000000 forks-sync-3.0.5/forks_sync.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-03-30 17:30:17.000000 forks-sync-3.0.5/forks_sync.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-03-30 17:30:17.000000 forks-sync-3.0.5/forks_sync.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-03-30 17:30:17.000000 forks-sync-3.0.5/forks_sync.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-03-30 17:29:38.000000 forks-sync-3.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-30 17:30:17.094869 forks-sync-3.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-03-30 17:29:38.000000 forks-sync-3.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 17:30:17.090870 forks-sync-3.0.5/test/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 17:30:17.094869 forks-sync-3.0.5/test/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 17:29:38.000000 forks-sync-3.0.5/test/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-03-30 17:29:38.000000 forks-sync-3.0.5/test/unit/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     7529 2023-03-30 17:29:38.000000 forks-sync-3.0.5/test/unit/test_sync.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 02:30:02.474401 forks-sync-4.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-02 02:29:31.000000 forks-sync-4.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-07-02 02:30:02.474401 forks-sync-4.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-07-02 02:29:31.000000 forks-sync-4.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 02:30:02.470401 forks-sync-4.0.0/forks_sync/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-02 02:29:31.000000 forks-sync-4.0.0/forks_sync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-07-02 02:29:31.000000 forks-sync-4.0.0/forks_sync/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-02 02:29:31.000000 forks-sync-4.0.0/forks_sync/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 02:29:31.000000 forks-sync-4.0.0/forks_sync/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     6370 2023-07-02 02:29:31.000000 forks-sync-4.0.0/forks_sync/sync.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 02:30:02.470401 forks-sync-4.0.0/forks_sync.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-07-02 02:30:02.000000 forks-sync-4.0.0/forks_sync.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-07-02 02:30:02.000000 forks-sync-4.0.0/forks_sync.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 02:30:02.000000 forks-sync-4.0.0/forks_sync.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-02 02:30:02.000000 forks-sync-4.0.0/forks_sync.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-02 02:30:02.000000 forks-sync-4.0.0/forks_sync.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-02 02:30:02.000000 forks-sync-4.0.0/forks_sync.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-02 02:29:31.000000 forks-sync-4.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 02:30:02.474401 forks-sync-4.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-07-02 02:29:31.000000 forks-sync-4.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 02:30:02.470401 forks-sync-4.0.0/test/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 02:30:02.474401 forks-sync-4.0.0/test/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 02:29:31.000000 forks-sync-4.0.0/test/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-02 02:29:31.000000 forks-sync-4.0.0/test/unit/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7529 2023-07-02 02:29:31.000000 forks-sync-4.0.0/test/unit/test_sync.py
```

### Comparing `forks-sync-3.0.5/LICENSE` & `forks-sync-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `forks-sync-3.0.5/PKG-INFO` & `forks-sync-4.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: forks-sync
-Version: 3.0.5
+Version: 4.0.0
 Summary: Keep all your git forks up to date with the remote default branch.
 Home-page: http://github.com/justintime50/forks-sync
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
 
 # Forks Sync
@@ -37,20 +37,20 @@
 ## Install
 
 ```bash
 # Install tool
 pip3 install forks-sync
 
 # Install locally
-make install
+just install
 ```
 
 ## Usage
 
-```
+```text
 Usage:
     forks-sync --token 123...
 
 Options:
     -h, --help            show this help message and exit
     -t TOKEN, --token TOKEN
                             Provide your GitHub token to authenticate with the GitHub API.
@@ -72,12 +72,12 @@
 ssh-add
 ```
 
 ## Development
 
 ```bash
 # Get a comprehensive list of development tools
-make help
+just --list
 
 # Run the tool locally
 venv/bin/python forks_sync/sync.py
 ```
```

### Comparing `forks-sync-3.0.5/README.md` & `forks-sync-4.0.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -22,20 +22,20 @@
 ## Install
 
 ```bash
 # Install tool
 pip3 install forks-sync
 
 # Install locally
-make install
+just install
 ```
 
 ## Usage
 
-```
+```text
 Usage:
     forks-sync --token 123...
 
 Options:
     -h, --help            show this help message and exit
     -t TOKEN, --token TOKEN
                             Provide your GitHub token to authenticate with the GitHub API.
@@ -57,12 +57,12 @@
 ssh-add
 ```
 
 ## Development
 
 ```bash
 # Get a comprehensive list of development tools
-make help
+just --list
 
 # Run the tool locally
 venv/bin/python forks_sync/sync.py
 ```
```

### Comparing `forks-sync-3.0.5/forks_sync/cli.py` & `forks-sync-4.0.0/forks_sync/cli.py`

 * *Files identical despite different names*

### Comparing `forks-sync-3.0.5/forks_sync/sync.py` & `forks-sync-4.0.0/forks_sync/sync.py`

 * *Files identical despite different names*

### Comparing `forks-sync-3.0.5/forks_sync.egg-info/PKG-INFO` & `forks-sync-4.0.0/forks_sync.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: forks-sync
-Version: 3.0.5
+Version: 4.0.0
 Summary: Keep all your git forks up to date with the remote default branch.
 Home-page: http://github.com/justintime50/forks-sync
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
 
 # Forks Sync
@@ -37,20 +37,20 @@
 ## Install
 
 ```bash
 # Install tool
 pip3 install forks-sync
 
 # Install locally
-make install
+just install
 ```
 
 ## Usage
 
-```
+```text
 Usage:
     forks-sync --token 123...
 
 Options:
     -h, --help            show this help message and exit
     -t TOKEN, --token TOKEN
                             Provide your GitHub token to authenticate with the GitHub API.
@@ -72,12 +72,12 @@
 ssh-add
 ```
 
 ## Development
 
 ```bash
 # Get a comprehensive list of development tools
-make help
+just --list
 
 # Run the tool locally
 venv/bin/python forks_sync/sync.py
 ```
```

### Comparing `forks-sync-3.0.5/setup.py` & `forks-sync-4.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,25 +9,25 @@
     'woodchips == 0.2.*',
 ]
 
 DEV_REQUIREMENTS = [
     'bandit == 1.7.*',
     'black == 23.*',
     'build == 0.10.*',
-    'flake8 == 5.*',
+    'flake8 == 6.*',
     'isort == 5.*',
-    'mypy == 1.1.*',
+    'mypy == 1.3.*',
     'pytest == 7.*',
     'pytest-cov == 4.*',
     'twine == 4.*',
 ]
 
 setuptools.setup(
     name='forks-sync',
-    version='3.0.5',
+    version='4.0.0',
     description='Keep all your git forks up to date with the remote default branch.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='http://github.com/justintime50/forks-sync',
     author='Justintime50',
     license='MIT',
     packages=setuptools.find_packages(
@@ -51,9 +51,9 @@
         'dev': DEV_REQUIREMENTS,
     },
     entry_points={
         'console_scripts': [
             'forks-sync=forks_sync.cli:main',
         ],
     },
-    python_requires='>=3.7, <4',
+    python_requires='>=3.8, <4',
 )
```

### Comparing `forks-sync-3.0.5/test/unit/test_sync.py` & `forks-sync-4.0.0/test/unit/test_sync.py`

 * *Files identical despite different names*

