# Comparing `tmp/mik_py-0.0.4.tar.gz` & `tmp/mik_py-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mik_py-0.0.4.tar", last modified: Sun Jul  2 11:21:48 2023, max compression
+gzip compressed data, was "mik_py-0.0.5.tar", last modified: Sun Jul  2 11:33:52 2023, max compression
```

## Comparing `mik_py-0.0.4.tar` & `mik_py-0.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 michaelchung   (501) staff       (20)        0 2023-07-02 11:21:48.136931 mik_py-0.0.4/
--rw-r--r--   0 michaelchung   (501) staff       (20)       67 2023-03-23 23:33:28.000000 mik_py-0.0.4/MANIFEST.in
--rw-r--r--   0 michaelchung   (501) staff       (20)      975 2023-07-02 11:21:48.136600 mik_py-0.0.4/PKG-INFO
--rw-r--r--   0 michaelchung   (501) staff       (20)      566 2023-07-02 11:07:52.000000 mik_py-0.0.4/README.md
--rw-r--r--   0 michaelchung   (501) staff       (20)       68 2023-03-21 13:16:23.000000 mik_py-0.0.4/eicar.com
-drwxr-xr-x   0 michaelchung   (501) staff       (20)        0 2023-07-02 11:21:48.133637 mik_py-0.0.4/mik_pack_10/
--rw-r--r--   0 michaelchung   (501) staff       (20)       34 2023-03-26 21:06:06.000000 mik_py-0.0.4/mik_pack_10/__init__.py
--rw-r--r--   0 michaelchung   (501) staff       (20)      680 2023-03-26 21:01:11.000000 mik_py-0.0.4/mik_pack_10/mik_py_.py
-drwxr-xr-x   0 michaelchung   (501) staff       (20)        0 2023-07-02 11:21:48.136174 mik_py-0.0.4/mik_py.egg-info/
--rw-r--r--   0 michaelchung   (501) staff       (20)      975 2023-07-02 11:21:47.000000 mik_py-0.0.4/mik_py.egg-info/PKG-INFO
--rw-r--r--   0 michaelchung   (501) staff       (20)      207 2023-07-02 11:21:48.000000 mik_py-0.0.4/mik_py.egg-info/SOURCES.txt
--rw-r--r--   0 michaelchung   (501) staff       (20)        1 2023-07-02 11:21:47.000000 mik_py-0.0.4/mik_py.egg-info/dependency_links.txt
--rw-r--r--   0 michaelchung   (501) staff       (20)       12 2023-07-02 11:21:47.000000 mik_py-0.0.4/mik_py.egg-info/top_level.txt
--rw-r--r--   0 michaelchung   (501) staff       (20)       38 2023-07-02 11:21:48.137034 mik_py-0.0.4/setup.cfg
--rw-r--r--   0 michaelchung   (501) staff       (20)     1415 2023-07-02 11:21:38.000000 mik_py-0.0.4/setup.py
+drwxr-xr-x   0 michaelchung   (501) staff       (20)        0 2023-07-02 11:33:52.384964 mik_py-0.0.5/
+-rw-r--r--   0 michaelchung   (501) staff       (20)       67 2023-03-23 23:33:28.000000 mik_py-0.0.5/MANIFEST.in
+-rw-r--r--   0 michaelchung   (501) staff       (20)      979 2023-07-02 11:33:52.384586 mik_py-0.0.5/PKG-INFO
+-rw-r--r--   0 michaelchung   (501) staff       (20)      566 2023-07-02 11:07:52.000000 mik_py-0.0.5/README.md
+-rw-r--r--   0 michaelchung   (501) staff       (20)       68 2023-03-21 13:16:23.000000 mik_py-0.0.5/eicar.com
+drwxr-xr-x   0 michaelchung   (501) staff       (20)        0 2023-07-02 11:33:52.381839 mik_py-0.0.5/mik_pack_10/
+-rw-r--r--   0 michaelchung   (501) staff       (20)       34 2023-03-26 21:06:06.000000 mik_py-0.0.5/mik_pack_10/__init__.py
+-rw-r--r--   0 michaelchung   (501) staff       (20)      680 2023-03-26 21:01:11.000000 mik_py-0.0.5/mik_pack_10/mik_py_.py
+drwxr-xr-x   0 michaelchung   (501) staff       (20)        0 2023-07-02 11:33:52.384059 mik_py-0.0.5/mik_py.egg-info/
+-rw-r--r--   0 michaelchung   (501) staff       (20)      979 2023-07-02 11:33:52.000000 mik_py-0.0.5/mik_py.egg-info/PKG-INFO
+-rw-r--r--   0 michaelchung   (501) staff       (20)      207 2023-07-02 11:33:52.000000 mik_py-0.0.5/mik_py.egg-info/SOURCES.txt
+-rw-r--r--   0 michaelchung   (501) staff       (20)        1 2023-07-02 11:33:52.000000 mik_py-0.0.5/mik_py.egg-info/dependency_links.txt
+-rw-r--r--   0 michaelchung   (501) staff       (20)       12 2023-07-02 11:33:52.000000 mik_py-0.0.5/mik_py.egg-info/top_level.txt
+-rw-r--r--   0 michaelchung   (501) staff       (20)       38 2023-07-02 11:33:52.385093 mik_py-0.0.5/setup.cfg
+-rw-r--r--   0 michaelchung   (501) staff       (20)     1395 2023-07-02 11:33:46.000000 mik_py-0.0.5/setup.py
```

### Comparing `mik_py-0.0.4/PKG-INFO` & `mik_py-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: mik_py
-Version: 0.0.4
+Version: 0.0.5
 Summary: A Python package containing the Eicar file to help test anti-malware or anti-virus software
 Author: Mike
 Author-email: michaelrchung@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
-Downloading this python package will also download the Eicar file as part of the python package https://www.eicar.org/download-anti-malware-testfile/.The Eicar file is a file used widely to test anti-malware software against malware and viruses. The Eicar file downloaded as part of this package is not malware but most anti-malware solutions will detect the Eicar file as malware or a virus and will trigger an alert. Please use this package with caution. This python package was created for testing purposes. Please use with caution as it will trigger alerts. 
+Downloading this python package will also download the Eicar file as part of the python package https://www.eicar.org/download-anti-malware-testfile/./n/nThe Eicar file is a file used widely to test anti-malware software against malware and viruses. The Eicar file downloaded as part of this package is not malware but most anti-malware solutions will detect the Eicar file as malware or a virus and will trigger an alert. Please use this package with caution. This python package was created for testing purposes. Please use with caution as it will trigger alerts.
```

### Comparing `mik_py-0.0.4/README.md` & `mik_py-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `mik_py-0.0.4/mik_pack_10/mik_py_.py` & `mik_py-0.0.5/mik_pack_10/mik_py_.py`

 * *Files identical despite different names*

### Comparing `mik_py-0.0.4/mik_py.egg-info/PKG-INFO` & `mik_py-0.0.5/mik_py.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: mik-py
-Version: 0.0.4
+Version: 0.0.5
 Summary: A Python package containing the Eicar file to help test anti-malware or anti-virus software
 Author: Mike
 Author-email: michaelrchung@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
-Downloading this python package will also download the Eicar file as part of the python package https://www.eicar.org/download-anti-malware-testfile/.The Eicar file is a file used widely to test anti-malware software against malware and viruses. The Eicar file downloaded as part of this package is not malware but most anti-malware solutions will detect the Eicar file as malware or a virus and will trigger an alert. Please use this package with caution. This python package was created for testing purposes. Please use with caution as it will trigger alerts. 
+Downloading this python package will also download the Eicar file as part of the python package https://www.eicar.org/download-anti-malware-testfile/./n/nThe Eicar file is a file used widely to test anti-malware software against malware and viruses. The Eicar file downloaded as part of this package is not malware but most anti-malware solutions will detect the Eicar file as malware or a virus and will trigger an alert. Please use this package with caution. This python package was created for testing purposes. Please use with caution as it will trigger alerts.
```

### Comparing `mik_py-0.0.4/setup.py` & `mik_py-0.0.5/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,20 +3,19 @@
 from setuptools import find_packages, setup
 
 with open(os.path.join(os.path.dirname(__file__), "README.md")) as readme:
     README = readme.read()
 
 setuptools.setup(
     name="mik_py",
-    version="0.0.4",
+    version="0.0.5",
     author="Mike",
     author_email="michaelrchung@gmail.com",
     description="A Python package containing the Eicar file to help test anti-malware or anti-virus software",
-    long_description="Downloading this python package will also download the Eicar file as part of the python package https://www.eicar.org/download-anti-malware-testfile/."
-                     "The Eicar file is a file used widely to test anti-malware software against malware and viruses. The Eicar file downloaded as part of this package is not malware but most anti-malware solutions will detect the Eicar file as malware or a virus and will trigger an alert. Please use this package with caution. This python package was created for testing purposes. Please use with caution as it will trigger alerts. ",
+    long_description="Downloading this python package will also download the Eicar file as part of the python package https://www.eicar.org/download-anti-malware-testfile/./n/nThe Eicar file is a file used widely to test anti-malware software against malware and viruses. The Eicar file downloaded as part of this package is not malware but most anti-malware solutions will detect the Eicar file as malware or a virus and will trigger an alert. Please use this package with caution. This python package was created for testing purposes. Please use with caution as it will trigger alerts. ",
     long_description_content_type="text/markdown",
     #url="www.test.com",
     packages=find_packages(),
     include_package_data=True,
     packages_data={
         'eicar_py':['eicar.com'],
     },
```

