# Comparing `tmp/ourlib-0.1.2.tar.gz` & `tmp/ourlib-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ourlib-0.1.2.tar", last modified: Sun Jul  2 07:16:43 2023, max compression
+gzip compressed data, was "ourlib-0.1.3.tar", last modified: Sun Jul  2 07:35:10 2023, max compression
```

## Comparing `ourlib-0.1.2.tar` & `ourlib-0.1.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-02 07:16:43.511840 ourlib-0.1.2/
--rw-rw-rw-   0        0        0     1090 2023-07-01 16:34:46.000000 ourlib-0.1.2/LICENSE
--rw-rw-rw-   0        0        0      474 2023-07-02 07:16:43.510844 ourlib-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0       51 2023-07-01 16:34:46.000000 ourlib-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-02 07:16:43.448182 ourlib-0.1.2/ourlib/
--rw-rw-rw-   0        0        0       20 2023-07-02 07:13:33.000000 ourlib-0.1.2/ourlib/__init__.py
--rw-rw-rw-   0        0        0      843 2023-07-02 07:13:26.000000 ourlib-0.1.2/ourlib/command_line.py
--rw-rw-rw-   0        0        0      732 2023-07-02 05:02:24.000000 ourlib-0.1.2/ourlib/ourlib.py
-drwxrwxrwx   0        0        0        0 2023-07-02 07:16:43.506840 ourlib-0.1.2/ourlib.egg-info/
--rw-rw-rw-   0        0        0      474 2023-07-02 07:16:42.000000 ourlib-0.1.2/ourlib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      267 2023-07-02 07:16:43.000000 ourlib-0.1.2/ourlib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-02 07:16:42.000000 ourlib-0.1.2/ourlib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-07-02 07:16:42.000000 ourlib-0.1.2/ourlib.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       32 2023-07-02 07:16:42.000000 ourlib-0.1.2/ourlib.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-02 07:16:42.000000 ourlib-0.1.2/ourlib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-02 07:16:43.512840 ourlib-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1552 2023-07-02 07:16:08.000000 ourlib-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-02 07:35:10.464751 ourlib-0.1.3/
+-rw-rw-rw-   0        0        0     1090 2023-07-01 16:34:46.000000 ourlib-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0      474 2023-07-02 07:35:10.462385 ourlib-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0       51 2023-07-01 16:34:46.000000 ourlib-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-02 07:35:10.430305 ourlib-0.1.3/ourlib/
+-rw-rw-rw-   0        0        0       20 2023-07-02 07:13:33.000000 ourlib-0.1.3/ourlib/__init__.py
+-rw-rw-rw-   0        0        0     1909 2023-07-02 07:34:02.000000 ourlib-0.1.3/ourlib/command_line.py
+-rw-rw-rw-   0        0        0      732 2023-07-02 05:02:24.000000 ourlib-0.1.3/ourlib/ourlib.py
+drwxrwxrwx   0        0        0        0 2023-07-02 07:35:10.459337 ourlib-0.1.3/ourlib.egg-info/
+-rw-rw-rw-   0        0        0      474 2023-07-02 07:35:10.000000 ourlib-0.1.3/ourlib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      267 2023-07-02 07:35:10.000000 ourlib-0.1.3/ourlib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-02 07:35:10.000000 ourlib-0.1.3/ourlib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-07-02 07:35:10.000000 ourlib-0.1.3/ourlib.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       32 2023-07-02 07:35:10.000000 ourlib-0.1.3/ourlib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-02 07:35:10.000000 ourlib-0.1.3/ourlib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-02 07:35:10.465251 ourlib-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1552 2023-07-02 07:34:26.000000 ourlib-0.1.3/setup.py
```

### Comparing `ourlib-0.1.2/LICENSE` & `ourlib-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ourlib-0.1.2/ourlib/ourlib.py` & `ourlib-0.1.3/ourlib/ourlib.py`

 * *Files identical despite different names*

### Comparing `ourlib-0.1.2/setup.py` & `ourlib-0.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # Configurations
 with open("README.md", "r") as fh:
     long_description = fh.read()
 setuptools.setup(
      install_requires=['torch','numpy','pandas','scikit-learn'],        # Dependencies
      python_requires='>=3.8',                                           # Minimum Python version
      name='ourlib',                                                     # Package name
-     version="0.1.2",                                                      # Version
+     version="0.1.3",                                                      # Version
      author="PT",                                     # Author name
      author_email="name@gmail.com",                           # Author mail
      description="Python package for ourlib.",    # Short package description
      long_description=long_description,                       # Long package description
      long_description_content_type="text/markdown",
      url="https://github.com/kunxl-gg/Mercor-pypi",       # Url to your Git Repo
      packages=setuptools.find_packages(),                     # Searches throughout all dirs for files to include
```

