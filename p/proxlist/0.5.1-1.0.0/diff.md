# Comparing `tmp/proxlist-0.5.1.tar.gz` & `tmp/proxlist-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proxlist-0.5.1.tar", last modified: Wed Apr 12 19:09:33 2023, max compression
+gzip compressed data, was "proxlist-1.0.0.tar", last modified: Sun Jul  2 02:22:49 2023, max compression
```

## Comparing `proxlist-0.5.1.tar` & `proxlist-1.0.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:09:33.656476 proxlist-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-12 19:09:06.000000 proxlist-0.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-04-12 19:09:33.656476 proxlist-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-04-12 19:09:06.000000 proxlist-0.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:09:33.656476 proxlist-0.5.1/proxlist/
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-04-12 19:09:06.000000 proxlist-0.5.1/proxlist/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4593 2023-04-12 19:09:06.000000 proxlist-0.5.1/proxlist/proxies.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 19:09:06.000000 proxlist-0.5.1/proxlist/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:09:33.656476 proxlist-0.5.1/proxlist.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-04-12 19:09:33.000000 proxlist-0.5.1/proxlist.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-04-12 19:09:33.000000 proxlist-0.5.1/proxlist.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 19:09:33.000000 proxlist-0.5.1/proxlist.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-12 19:09:33.000000 proxlist-0.5.1/proxlist.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-12 19:09:33.000000 proxlist-0.5.1/proxlist.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-12 19:09:06.000000 proxlist-0.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 19:09:33.656476 proxlist-0.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-04-12 19:09:06.000000 proxlist-0.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:09:33.656476 proxlist-0.5.1/test/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 19:09:33.656476 proxlist-0.5.1/test/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 19:09:06.000000 proxlist-0.5.1/test/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3696 2023-04-12 19:09:06.000000 proxlist-0.5.1/test/unit/test_proxies.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 02:22:49.900431 proxlist-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-02 02:22:21.000000 proxlist-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-07-02 02:22:49.900431 proxlist-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-07-02 02:22:21.000000 proxlist-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 02:22:49.900431 proxlist-1.0.0/proxlist/
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-02 02:22:21.000000 proxlist-1.0.0/proxlist/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4593 2023-07-02 02:22:21.000000 proxlist-1.0.0/proxlist/proxies.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 02:22:21.000000 proxlist-1.0.0/proxlist/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 02:22:49.900431 proxlist-1.0.0/proxlist.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-07-02 02:22:49.000000 proxlist-1.0.0/proxlist.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-07-02 02:22:49.000000 proxlist-1.0.0/proxlist.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 02:22:49.000000 proxlist-1.0.0/proxlist.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-02 02:22:49.000000 proxlist-1.0.0/proxlist.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-02 02:22:49.000000 proxlist-1.0.0/proxlist.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-02 02:22:21.000000 proxlist-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 02:22:49.904431 proxlist-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-07-02 02:22:21.000000 proxlist-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 02:22:49.896431 proxlist-1.0.0/test/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 02:22:49.900431 proxlist-1.0.0/test/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 02:22:21.000000 proxlist-1.0.0/test/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3696 2023-07-02 02:22:21.000000 proxlist-1.0.0/test/unit/test_proxies.py
```

### Comparing `proxlist-0.5.1/LICENSE` & `proxlist-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `proxlist-0.5.1/PKG-INFO` & `proxlist-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: proxlist
-Version: 0.5.1
-Summary: Retrieve proxy servers.
+Version: 1.0.0
+Summary: Retrieve free, open-source proxy servers.
 Home-page: http://github.com/Justintime50/proxlist
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
 
 # Proxlist
@@ -37,15 +37,15 @@
 ## Install
 
 ```bash
 # Install tool
 pip3 install proxlist
 
 # Install locally
-make install
+just install
 ```
 
 ## Usage
 
 ```python
 import proxlist
 import requests
@@ -75,9 +75,9 @@
 print(response.text)
 ```
 
 ## Development
 
 ```bash
 # Get a comprehensive list of development tools
-make help
+just --list
 ```
```

### Comparing `proxlist-0.5.1/README.md` & `proxlist-1.0.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 ## Install
 
 ```bash
 # Install tool
 pip3 install proxlist
 
 # Install locally
-make install
+just install
 ```
 
 ## Usage
 
 ```python
 import proxlist
 import requests
@@ -60,9 +60,9 @@
 print(response.text)
 ```
 
 ## Development
 
 ```bash
 # Get a comprehensive list of development tools
-make help
+just --list
 ```
```

### Comparing `proxlist-0.5.1/proxlist/proxies.py` & `proxlist-1.0.0/proxlist/proxies.py`

 * *Files identical despite different names*

### Comparing `proxlist-0.5.1/proxlist.egg-info/PKG-INFO` & `proxlist-1.0.0/proxlist.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: proxlist
-Version: 0.5.1
-Summary: Retrieve proxy servers.
+Version: 1.0.0
+Summary: Retrieve free, open-source proxy servers.
 Home-page: http://github.com/Justintime50/proxlist
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
 
 # Proxlist
@@ -37,15 +37,15 @@
 ## Install
 
 ```bash
 # Install tool
 pip3 install proxlist
 
 # Install locally
-make install
+just install
 ```
 
 ## Usage
 
 ```python
 import proxlist
 import requests
@@ -75,9 +75,9 @@
 print(response.text)
 ```
 
 ## Development
 
 ```bash
 # Get a comprehensive list of development tools
-make help
+just --list
 ```
```

### Comparing `proxlist-0.5.1/setup.py` & `proxlist-1.0.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,27 +10,27 @@
     'woodchips == 0.2.*',
 ]
 
 DEV_REQUIREMENTS = [
     'bandit == 1.7.*',
     'black == 23.*',
     'build == 0.10.*',
-    'flake8 == 5.*',
+    'flake8 == 6.*',
     'isort == 5.*',
-    'mypy == 1.2.*',
+    'mypy == 1.3.*',
     'pytest == 7.*',
     'pytest-cov == 4.*',
     'twine == 4.*',
     'types-requests',
 ]
 
 setuptools.setup(
     name='proxlist',
-    version='0.5.1',
-    description='Retrieve proxy servers.',
+    version='1.0.0',
+    description='Retrieve free, open-source proxy servers.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='http://github.com/Justintime50/proxlist',
     author='Justintime50',
     license='MIT',
     packages=setuptools.find_packages(
         exclude=[
@@ -48,9 +48,9 @@
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     install_requires=REQUIREMENTS,
     extras_require={
         'dev': DEV_REQUIREMENTS,
     },
-    python_requires='>=3.7, <4',
+    python_requires='>=3.8, <4',
 )
```

### Comparing `proxlist-0.5.1/test/unit/test_proxies.py` & `proxlist-1.0.0/test/unit/test_proxies.py`

 * *Files identical despite different names*

