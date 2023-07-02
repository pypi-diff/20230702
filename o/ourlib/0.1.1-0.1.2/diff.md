# Comparing `tmp/ourlib-0.1.1.tar.gz` & `tmp/ourlib-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ourlib-0.1.1.tar", last modified: Sun Jul  2 06:27:57 2023, max compression
+gzip compressed data, was "ourlib-0.1.2.tar", last modified: Sun Jul  2 07:16:43 2023, max compression
```

## Comparing `ourlib-0.1.1.tar` & `ourlib-0.1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-02 06:27:57.778414 ourlib-0.1.1/
--rw-rw-rw-   0        0        0     1090 2023-07-01 16:34:46.000000 ourlib-0.1.1/LICENSE
--rw-rw-rw-   0        0        0      474 2023-07-02 06:27:57.776986 ourlib-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0       51 2023-07-01 16:34:46.000000 ourlib-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-02 06:27:57.757339 ourlib-0.1.1/ourlib/
--rw-rw-rw-   0        0        0       20 2023-07-02 04:38:49.000000 ourlib-0.1.1/ourlib/__init__.py
--rw-rw-rw-   0        0        0      835 2023-07-02 05:28:28.000000 ourlib-0.1.1/ourlib/command_line.py
--rw-rw-rw-   0        0        0      732 2023-07-02 05:02:24.000000 ourlib-0.1.1/ourlib/ourlib.py
-drwxrwxrwx   0        0        0        0 2023-07-02 06:27:57.774786 ourlib-0.1.1/ourlib.egg-info/
--rw-rw-rw-   0        0        0      474 2023-07-02 06:27:57.000000 ourlib-0.1.1/ourlib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      267 2023-07-02 06:27:57.000000 ourlib-0.1.1/ourlib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-02 06:27:57.000000 ourlib-0.1.1/ourlib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-07-02 06:27:57.000000 ourlib-0.1.1/ourlib.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       32 2023-07-02 06:27:57.000000 ourlib-0.1.1/ourlib.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-02 06:27:57.000000 ourlib-0.1.1/ourlib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-02 06:27:57.778882 ourlib-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1552 2023-07-02 06:25:41.000000 ourlib-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-02 07:16:43.511840 ourlib-0.1.2/
+-rw-rw-rw-   0        0        0     1090 2023-07-01 16:34:46.000000 ourlib-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0      474 2023-07-02 07:16:43.510844 ourlib-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0       51 2023-07-01 16:34:46.000000 ourlib-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-02 07:16:43.448182 ourlib-0.1.2/ourlib/
+-rw-rw-rw-   0        0        0       20 2023-07-02 07:13:33.000000 ourlib-0.1.2/ourlib/__init__.py
+-rw-rw-rw-   0        0        0      843 2023-07-02 07:13:26.000000 ourlib-0.1.2/ourlib/command_line.py
+-rw-rw-rw-   0        0        0      732 2023-07-02 05:02:24.000000 ourlib-0.1.2/ourlib/ourlib.py
+drwxrwxrwx   0        0        0        0 2023-07-02 07:16:43.506840 ourlib-0.1.2/ourlib.egg-info/
+-rw-rw-rw-   0        0        0      474 2023-07-02 07:16:42.000000 ourlib-0.1.2/ourlib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      267 2023-07-02 07:16:43.000000 ourlib-0.1.2/ourlib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-02 07:16:42.000000 ourlib-0.1.2/ourlib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-07-02 07:16:42.000000 ourlib-0.1.2/ourlib.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       32 2023-07-02 07:16:42.000000 ourlib-0.1.2/ourlib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-02 07:16:42.000000 ourlib-0.1.2/ourlib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-02 07:16:43.512840 ourlib-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1552 2023-07-02 07:16:08.000000 ourlib-0.1.2/setup.py
```

### Comparing `ourlib-0.1.1/LICENSE` & `ourlib-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ourlib-0.1.1/ourlib/command_line.py` & `ourlib-0.1.2/ourlib/command_line.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import sys
-from ourlib import Model
+from ourlib import ourlib
 
 # def main():
 #     server_url = "http://your-server-url"
 #     Model.upload_files_to_server(server_url)
 
 # if __name__ == "__main__":
 #     main()
@@ -14,15 +14,15 @@
         return
 
     inference_script = args[0]
     model_class = args[1]
 
     # Upload files to the server
     # server_url = "http://your-server-url"
-    Model.upload_files_to_server()
+    ourlib.Model.upload_files_to_server()
 
      # Import and execute the user-defined inference script as if it were run with `python inference.py`
     sys.path.insert(0, "")
     sys.path.insert(0, ".")
     with open(inference_script, "r") as script_file:
         script_code = script_file.read()
         exec(script_code)
```

### Comparing `ourlib-0.1.1/ourlib/ourlib.py` & `ourlib-0.1.2/ourlib/ourlib.py`

 * *Files identical despite different names*

### Comparing `ourlib-0.1.1/setup.py` & `ourlib-0.1.2/setup.py`

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
-     version="0.1.1",                                                      # Version
+     version="0.1.2",                                                      # Version
      author="PT",                                     # Author name
      author_email="name@gmail.com",                           # Author mail
      description="Python package for ourlib.",    # Short package description
      long_description=long_description,                       # Long package description
      long_description_content_type="text/markdown",
      url="https://github.com/kunxl-gg/Mercor-pypi",       # Url to your Git Repo
      packages=setuptools.find_packages(),                     # Searches throughout all dirs for files to include
```

