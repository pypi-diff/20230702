# Comparing `tmp/ourlib-0.2.0.tar.gz` & `tmp/ourlib-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ourlib-0.2.0.tar", last modified: Sun Jul  2 08:47:43 2023, max compression
+gzip compressed data, was "ourlib-0.2.1.tar", last modified: Sun Jul  2 08:53:57 2023, max compression
```

## Comparing `ourlib-0.2.0.tar` & `ourlib-0.2.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-02 08:47:43.362736 ourlib-0.2.0/
--rw-rw-rw-   0        0        0     1090 2023-07-01 16:34:46.000000 ourlib-0.2.0/LICENSE
--rw-rw-rw-   0        0        0      474 2023-07-02 08:47:43.361374 ourlib-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0       51 2023-07-01 16:34:46.000000 ourlib-0.2.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-02 08:47:43.312564 ourlib-0.2.0/ourlib/
--rw-rw-rw-   0        0        0       20 2023-07-02 07:13:33.000000 ourlib-0.2.0/ourlib/__init__.py
--rw-rw-rw-   0        0        0      786 2023-07-02 08:44:18.000000 ourlib-0.2.0/ourlib/command_line.py
--rw-rw-rw-   0        0        0      757 2023-07-02 08:39:24.000000 ourlib-0.2.0/ourlib/ourlib.py
-drwxrwxrwx   0        0        0        0 2023-07-02 08:47:43.357081 ourlib-0.2.0/ourlib.egg-info/
--rw-rw-rw-   0        0        0      474 2023-07-02 08:47:42.000000 ourlib-0.2.0/ourlib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      267 2023-07-02 08:47:43.000000 ourlib-0.2.0/ourlib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-02 08:47:42.000000 ourlib-0.2.0/ourlib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-07-02 08:47:42.000000 ourlib-0.2.0/ourlib.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       32 2023-07-02 08:47:42.000000 ourlib-0.2.0/ourlib.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-02 08:47:42.000000 ourlib-0.2.0/ourlib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-02 08:47:43.363232 ourlib-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1552 2023-07-02 08:39:53.000000 ourlib-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-02 08:53:56.997667 ourlib-0.2.1/
+-rw-rw-rw-   0        0        0     1090 2023-07-01 16:34:46.000000 ourlib-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0      474 2023-07-02 08:53:56.995627 ourlib-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0       51 2023-07-01 16:34:46.000000 ourlib-0.2.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-02 08:53:56.964878 ourlib-0.2.1/ourlib/
+-rw-rw-rw-   0        0        0       20 2023-07-02 07:13:33.000000 ourlib-0.2.1/ourlib/__init__.py
+-rw-rw-rw-   0        0        0      796 2023-07-02 08:53:02.000000 ourlib-0.2.1/ourlib/command_line.py
+-rw-rw-rw-   0        0        0      757 2023-07-02 08:39:24.000000 ourlib-0.2.1/ourlib/ourlib.py
+drwxrwxrwx   0        0        0        0 2023-07-02 08:53:56.993404 ourlib-0.2.1/ourlib.egg-info/
+-rw-rw-rw-   0        0        0      474 2023-07-02 08:53:56.000000 ourlib-0.2.1/ourlib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      267 2023-07-02 08:53:56.000000 ourlib-0.2.1/ourlib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-02 08:53:56.000000 ourlib-0.2.1/ourlib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-07-02 08:53:56.000000 ourlib-0.2.1/ourlib.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       32 2023-07-02 08:53:56.000000 ourlib-0.2.1/ourlib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-02 08:53:56.000000 ourlib-0.2.1/ourlib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-02 08:53:56.998672 ourlib-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     1552 2023-07-02 08:53:18.000000 ourlib-0.2.1/setup.py
```

### Comparing `ourlib-0.2.0/LICENSE` & `ourlib-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ourlib-0.2.0/ourlib/command_line.py` & `ourlib-0.2.1/ourlib/command_line.py`

 * *Files 24% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     deployment = args.deployment
 
     # Upload files to the server
     if deployment == "deploy":
         ourlib.Model.upload_files_to_server()
 
     # Import and execute the user-defined inference script as if it were run with `python inference.py`
-    sys.path.insert(0, "")
-    sys.path.insert(0, ".")
-    with open(deployment, "r") as script_file:
-        script_code = script_file.read()
-        exec(script_code)
+    # sys.path.insert(0, "")
+    # sys.path.insert(0, ".")
+    # with open(deployment, "r") as script_file:
+    #     script_code = script_file.read()
+    #     exec(script_code)
 
 if __name__ == "__main__":
     main()
```

### Comparing `ourlib-0.2.0/ourlib/ourlib.py` & `ourlib-0.2.1/ourlib/ourlib.py`

 * *Files identical despite different names*

### Comparing `ourlib-0.2.0/setup.py` & `ourlib-0.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # Configurations
 with open("README.md", "r") as fh:
     long_description = fh.read()
 setuptools.setup(
      install_requires=['torch','numpy','pandas','scikit-learn'],        # Dependencies
      python_requires='>=3.8',                                           # Minimum Python version
      name='ourlib',                                                     # Package name
-     version="0.2.0",                                                      # Version
+     version="0.2.1",                                                      # Version
      author="PT",                                     # Author name
      author_email="name@gmail.com",                           # Author mail
      description="Python package for ourlib.",    # Short package description
      long_description=long_description,                       # Long package description
      long_description_content_type="text/markdown",
      url="https://github.com/kunxl-gg/Mercor-pypi",       # Url to your Git Repo
      packages=setuptools.find_packages(),                     # Searches throughout all dirs for files to include
```

