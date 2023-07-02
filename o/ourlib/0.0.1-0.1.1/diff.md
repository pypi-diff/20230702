# Comparing `tmp/ourlib-0.0.1.tar.gz` & `tmp/ourlib-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ourlib-0.0.1.tar", last modified: Sat Jul  1 19:01:31 2023, max compression
+gzip compressed data, was "ourlib-0.1.1.tar", last modified: Sun Jul  2 06:27:57 2023, max compression
```

## Comparing `ourlib-0.0.1.tar` & `ourlib-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-01 19:01:31.411041 ourlib-0.0.1/
--rw-rw-rw-   0        0        0     1090 2023-07-01 18:58:40.000000 ourlib-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      515 2023-07-01 19:01:31.410044 ourlib-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       51 2023-07-01 18:58:40.000000 ourlib-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-01 19:01:31.389245 ourlib-0.0.1/ourlib/
--rw-rw-rw-   0        0        0       25 2023-07-01 18:58:40.000000 ourlib-0.0.1/ourlib/__init__.py
--rw-rw-rw-   0        0        0       25 2023-07-01 18:58:40.000000 ourlib-0.0.1/ourlib/ourlib.py
-drwxrwxrwx   0        0        0        0 2023-07-01 19:01:31.409047 ourlib-0.0.1/ourlib.egg-info/
--rw-rw-rw-   0        0        0      515 2023-07-01 19:01:31.000000 ourlib-0.0.1/ourlib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      211 2023-07-01 19:01:31.000000 ourlib-0.0.1/ourlib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-01 19:01:31.000000 ourlib-0.0.1/ourlib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-07-01 19:01:31.000000 ourlib-0.0.1/ourlib.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-01 19:01:31.000000 ourlib-0.0.1/ourlib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-01 19:01:31.411041 ourlib-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1408 2023-07-01 18:58:40.000000 ourlib-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-02 06:27:57.778414 ourlib-0.1.1/
+-rw-rw-rw-   0        0        0     1090 2023-07-01 16:34:46.000000 ourlib-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0      474 2023-07-02 06:27:57.776986 ourlib-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0       51 2023-07-01 16:34:46.000000 ourlib-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-02 06:27:57.757339 ourlib-0.1.1/ourlib/
+-rw-rw-rw-   0        0        0       20 2023-07-02 04:38:49.000000 ourlib-0.1.1/ourlib/__init__.py
+-rw-rw-rw-   0        0        0      835 2023-07-02 05:28:28.000000 ourlib-0.1.1/ourlib/command_line.py
+-rw-rw-rw-   0        0        0      732 2023-07-02 05:02:24.000000 ourlib-0.1.1/ourlib/ourlib.py
+drwxrwxrwx   0        0        0        0 2023-07-02 06:27:57.774786 ourlib-0.1.1/ourlib.egg-info/
+-rw-rw-rw-   0        0        0      474 2023-07-02 06:27:57.000000 ourlib-0.1.1/ourlib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      267 2023-07-02 06:27:57.000000 ourlib-0.1.1/ourlib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-02 06:27:57.000000 ourlib-0.1.1/ourlib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-07-02 06:27:57.000000 ourlib-0.1.1/ourlib.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       32 2023-07-02 06:27:57.000000 ourlib-0.1.1/ourlib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-02 06:27:57.000000 ourlib-0.1.1/ourlib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-02 06:27:57.778882 ourlib-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1552 2023-07-02 06:25:41.000000 ourlib-0.1.1/setup.py
```

### Comparing `ourlib-0.0.1/LICENSE` & `ourlib-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ourlib-0.0.1/setup.py` & `ourlib-0.1.1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,25 +2,30 @@
 import re
 
 # Configurations
 with open("README.md", "r") as fh:
     long_description = fh.read()
 setuptools.setup(
      install_requires=['torch','numpy','pandas','scikit-learn'],        # Dependencies
-     python_requires='>=3.8',                                   # Minimum Python version
-     name='ourlib',                                             # Package name
-     version="0.0.1",                                     # Version
+     python_requires='>=3.8',                                           # Minimum Python version
+     name='ourlib',                                                     # Package name
+     version="0.1.1",                                                      # Version
      author="PT",                                     # Author name
      author_email="name@gmail.com",                           # Author mail
      description="Python package for ourlib.",    # Short package description
      long_description=long_description,                       # Long package description
      long_description_content_type="text/markdown",
      url="https://github.com/kunxl-gg/Mercor-pypi",       # Url to your Git Repo
      packages=setuptools.find_packages(),                     # Searches throughout all dirs for files to include
      include_package_data=True,                               # Must be true to include files depicted in MANIFEST.in
      license_files=["LICENSE"],                               # License file
      classifiers=[
          "Programming Language :: Python :: 3",
          "License :: OSI Approved :: MIT License",
          "Operating System :: OS Independent",
      ],
+     entry_points={
+      'console_scripts': [
+         'ourlib=ourlib.command_line:main',
+      ],
+   },
  )
```

