# Comparing `tmp/ourlib-0.2.2.tar.gz` & `tmp/ourlib-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ourlib-0.2.2.tar", last modified: Sun Jul  2 12:38:19 2023, max compression
+gzip compressed data, was "ourlib-0.2.3.tar", last modified: Sun Jul  2 16:54:37 2023, max compression
```

## Comparing `ourlib-0.2.2.tar` & `ourlib-0.2.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-02 12:38:19.410526 ourlib-0.2.2/
--rw-rw-rw-   0        0        0     1090 2023-07-01 16:34:46.000000 ourlib-0.2.2/LICENSE
--rw-rw-rw-   0        0        0      474 2023-07-02 12:38:19.409302 ourlib-0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0       51 2023-07-01 16:34:46.000000 ourlib-0.2.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-02 12:38:19.377667 ourlib-0.2.2/ourlib/
--rw-rw-rw-   0        0        0       20 2023-07-02 07:13:33.000000 ourlib-0.2.2/ourlib/__init__.py
--rw-rw-rw-   0        0        0      847 2023-07-02 12:17:16.000000 ourlib-0.2.2/ourlib/command_line.py
--rw-rw-rw-   0        0        0     1015 2023-07-02 12:30:34.000000 ourlib-0.2.2/ourlib/ourlib.py
-drwxrwxrwx   0        0        0        0 2023-07-02 12:38:19.405335 ourlib-0.2.2/ourlib.egg-info/
--rw-rw-rw-   0        0        0      474 2023-07-02 12:38:18.000000 ourlib-0.2.2/ourlib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      267 2023-07-02 12:38:19.000000 ourlib-0.2.2/ourlib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-02 12:38:18.000000 ourlib-0.2.2/ourlib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-07-02 12:38:18.000000 ourlib-0.2.2/ourlib.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       32 2023-07-02 12:38:18.000000 ourlib-0.2.2/ourlib.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-02 12:38:18.000000 ourlib-0.2.2/ourlib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-02 12:38:19.410943 ourlib-0.2.2/setup.cfg
--rw-rw-rw-   0        0        0     1552 2023-07-02 12:30:02.000000 ourlib-0.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-02 16:54:37.454614 ourlib-0.2.3/
+-rw-rw-rw-   0        0        0     1090 2023-07-01 16:34:46.000000 ourlib-0.2.3/LICENSE
+-rw-rw-rw-   0        0        0      474 2023-07-02 16:54:37.452618 ourlib-0.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0       51 2023-07-01 16:34:46.000000 ourlib-0.2.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-02 16:54:37.412376 ourlib-0.2.3/ourlib/
+-rw-rw-rw-   0        0        0       20 2023-07-02 07:13:33.000000 ourlib-0.2.3/ourlib/__init__.py
+-rw-rw-rw-   0        0        0      847 2023-07-02 12:17:16.000000 ourlib-0.2.3/ourlib/command_line.py
+-rw-rw-rw-   0        0        0      996 2023-07-02 13:22:12.000000 ourlib-0.2.3/ourlib/ourlib.py
+drwxrwxrwx   0        0        0        0 2023-07-02 16:54:37.447970 ourlib-0.2.3/ourlib.egg-info/
+-rw-rw-rw-   0        0        0      474 2023-07-02 16:54:37.000000 ourlib-0.2.3/ourlib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      267 2023-07-02 16:54:37.000000 ourlib-0.2.3/ourlib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-02 16:54:37.000000 ourlib-0.2.3/ourlib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-07-02 16:54:37.000000 ourlib-0.2.3/ourlib.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       26 2023-07-02 16:54:37.000000 ourlib-0.2.3/ourlib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-02 16:54:37.000000 ourlib-0.2.3/ourlib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-02 16:54:37.455507 ourlib-0.2.3/setup.cfg
+-rw-rw-rw-   0        0        0     1544 2023-07-02 16:43:45.000000 ourlib-0.2.3/setup.py
```

### Comparing `ourlib-0.2.2/LICENSE` & `ourlib-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ourlib-0.2.2/ourlib/command_line.py` & `ourlib-0.2.3/ourlib/command_line.py`

 * *Files identical despite different names*

### Comparing `ourlib-0.2.2/ourlib/ourlib.py` & `ourlib-0.2.3/ourlib/ourlib.py`

 * *Files 25% similar despite different names*

```diff
@@ -24,11 +24,9 @@
                     print("Failed to upload files!")
 
     async def deploy():
         response = await requests.get("http://localhost:8080/deploy")
         if response.status_code == 200:
             print("Deployed successfully!")
         else:
-            print("Failed to deploy!") 
-
-Model.deploy()
+            print("Failed to deploy!")
```

### Comparing `ourlib-0.2.2/setup.py` & `ourlib-0.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import setuptools
 import re
 
 # Configurations
 with open("README.md", "r") as fh:
     long_description = fh.read()
 setuptools.setup(
-     install_requires=['torch','numpy','pandas','scikit-learn'],        # Dependencies
+     install_requires=['torch','pandas','scikit-learn'],        # Dependencies
      python_requires='>=3.8',                                           # Minimum Python version
      name='ourlib',                                                     # Package name
-     version="0.2.2",                                                      # Version
+     version="0.2.3",                                                      # Version
      author="PT",                                     # Author name
      author_email="name@gmail.com",                           # Author mail
      description="Python package for ourlib.",    # Short package description
      long_description=long_description,                       # Long package description
      long_description_content_type="text/markdown",
      url="https://github.com/kunxl-gg/Mercor-pypi",       # Url to your Git Repo
      packages=setuptools.find_packages(),                     # Searches throughout all dirs for files to include
```

