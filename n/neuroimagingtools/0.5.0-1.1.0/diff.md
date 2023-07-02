# Comparing `tmp/neuroimagingtools-0.5.0.tar.gz` & `tmp/neuroimagingtools-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neuroimagingtools-0.5.0.tar", last modified: Thu Jun 30 18:46:01 2022, max compression
+gzip compressed data, was "neuroimagingtools-1.1.0.tar", last modified: Sun Jul  2 19:58:47 2023, max compression
```

## Comparing `neuroimagingtools-0.5.0.tar` & `neuroimagingtools-1.1.0.tar`

### file list

```diff
@@ -1,7 +1,11 @@
-drwxr-xr-x   0 jdiedrichsen   (501) staff       (20)        0 2022-06-30 18:46:01.609602 neuroimagingtools-0.5.0/
--rw-r--r--   0 jdiedrichsen   (501) staff       (20)      854 2022-06-30 18:46:01.609948 neuroimagingtools-0.5.0/PKG-INFO
-drwxr-xr-x   0 jdiedrichsen   (501) staff       (20)        0 2022-06-30 18:46:01.608990 neuroimagingtools-0.5.0/nitools/
--rw-r--r--   0 jdiedrichsen   (501) staff       (20)       29 2022-06-19 15:15:44.802477 neuroimagingtools-0.5.0/nitools/__init__.py
--rw-r--r--   0 jdiedrichsen   (501) staff       (20)    19374 2022-06-30 12:52:52.154062 neuroimagingtools-0.5.0/nitools/nitools.py
--rw-r--r--   0 jdiedrichsen   (501) staff       (20)       61 2022-06-30 12:52:52.155795 neuroimagingtools-0.5.0/setup.cfg
--rw-r--r--   0 jdiedrichsen   (501) staff       (20)     1007 2022-06-30 18:45:58.507607 neuroimagingtools-0.5.0/setup.py
+drwxr-xr-x   0 jdiedrichsen   (501) staff       (20)        0 2023-07-02 19:58:47.406175 neuroimagingtools-1.1.0/
+-rw-r--r--   0 jdiedrichsen   (501) staff       (20)      854 2023-07-02 19:58:47.406233 neuroimagingtools-1.1.0/PKG-INFO
+drwxr-xr-x   0 jdiedrichsen   (501) staff       (20)        0 2023-07-02 19:58:47.406149 neuroimagingtools-1.1.0/nitools/
+-rw-r--r--   0 jdiedrichsen   (501) staff       (20)      143 2023-06-29 02:16:21.647409 neuroimagingtools-1.1.0/nitools/__init__.py
+-rw-r--r--   0 jdiedrichsen   (501) staff       (20)     5579 2023-07-02 19:19:53.225758 neuroimagingtools-1.1.0/nitools/border.py
+-rw-r--r--   0 jdiedrichsen   (501) staff       (20)    13162 2023-07-02 19:14:20.360050 neuroimagingtools-1.1.0/nitools/cifti.py
+-rw-r--r--   0 jdiedrichsen   (501) staff       (20)     1579 2023-07-02 19:14:09.871026 neuroimagingtools-1.1.0/nitools/color.py
+-rw-r--r--   0 jdiedrichsen   (501) staff       (20)     9176 2023-07-02 19:13:43.720360 neuroimagingtools-1.1.0/nitools/gifti.py
+-rw-r--r--   0 jdiedrichsen   (501) staff       (20)     8289 2023-07-02 19:13:33.311992 neuroimagingtools-1.1.0/nitools/volume.py
+-rw-r--r--   0 jdiedrichsen   (501) staff       (20)       61 2022-06-30 12:52:52.155795 neuroimagingtools-1.1.0/setup.cfg
+-rw-r--r--   0 jdiedrichsen   (501) staff       (20)     1068 2023-07-02 19:56:28.984112 neuroimagingtools-1.1.0/setup.py
```

### Comparing `neuroimagingtools-0.5.0/PKG-INFO` & `neuroimagingtools-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: neuroimagingtools
-Version: 0.5.0
+Version: 1.1.0
 Summary: Neuroimaging analysis tools
 Home-page: https://github.com/DiedrichsenLab/nitools
 Author: Jörn Diedrichsen
 Author-email: joern.diedrichsen@googlemail.com
 License: MIT
-Download-URL: https://github.com/DiedrichsenLab/nitools/archive/refs/tags/v0.5.0.tar.gz
+Download-URL: https://github.com/DiedrichsenLab/nitools/archive/refs/tags/v1.1.0.tar.gz
 Description: UNKNOWN
 Keywords: imaging analysis,nifti,gifti,cifti
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `neuroimagingtools-0.5.0/setup.py` & `neuroimagingtools-1.1.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 from distutils.core import setup
 setup(
   name = 'neuroimagingtools',
   packages = ['nitools'],
-  version = '0.5.0',
+  version = '1.1.0',
   license='MIT',
   description = 'Neuroimaging analysis tools',
   author = 'Jörn Diedrichsen',
   author_email = 'joern.diedrichsen@googlemail.com',
   url = 'https://github.com/DiedrichsenLab/nitools',
-  download_url = 'https://github.com/DiedrichsenLab/nitools/archive/refs/tags/v0.5.0.tar.gz',
+  download_url = 'https://github.com/DiedrichsenLab/nitools/archive/refs/tags/v1.1.0.tar.gz',
   keywords = ['imaging analysis', 'nifti', 'gifti','cifti'],
   install_requires=[
+          'bezier',
+          'trimesh',
           'numpy',
           'matplotlib',
-          'nibabel'],
+          'nibabel',
+          'pandas'],
   classifiers=[
     'Development Status :: 4 - Beta',
     'Intended Audience :: Science/Research',
     'Intended Audience :: Developers',
     'Topic :: Software Development :: Build Tools',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3.6',
```

