# Comparing `tmp/pyzjr-0.0.2.tar.gz` & `tmp/pyzjr-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pyzjr-0.0.2.tar", last modified: Sun Jul  2 05:48:45 2023, max compression
+gzip compressed data, was "dist\pyzjr-0.0.3.tar", last modified: Sun Jul  2 07:24:27 2023, max compression
```

## Comparing `pyzjr-0.0.2.tar` & `pyzjr-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-02 05:48:45.000000 pyzjr-0.0.2/
--rw-rw-rw-   0        0        0      696 2023-07-02 05:48:45.000000 pyzjr-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       21 2023-06-10 05:53:05.000000 pyzjr-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-02 05:48:45.000000 pyzjr-0.0.2/pyzjr/
--rw-rw-rw-   0        0        0      104 2023-06-10 05:53:05.000000 pyzjr-0.0.2/pyzjr/Z.py
--rw-rw-rw-   0        0        0      767 2023-07-02 05:48:40.000000 pyzjr-0.0.2/pyzjr/__init__.py
--rw-rw-rw-   0        0        0      775 2023-07-02 04:11:00.000000 pyzjr-0.0.2/pyzjr/setup.py
--rw-rw-rw-   0        0        0     4073 2023-06-10 05:53:05.000000 pyzjr-0.0.2/pyzjr/utils.py
--rw-rw-rw-   0        0        0     2784 2023-06-10 05:53:05.000000 pyzjr-0.0.2/pyzjr/video.py
-drwxrwxrwx   0        0        0        0 2023-07-02 05:48:45.000000 pyzjr-0.0.2/pyzjr.egg-info/
--rw-rw-rw-   0        0        0      696 2023-07-02 05:48:44.000000 pyzjr-0.0.2/pyzjr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      208 2023-07-02 05:48:45.000000 pyzjr-0.0.2/pyzjr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-02 05:48:44.000000 pyzjr-0.0.2/pyzjr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-07-02 05:48:45.000000 pyzjr-0.0.2/pyzjr.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-02 05:48:45.000000 pyzjr-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1734 2023-07-02 05:48:32.000000 pyzjr-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-02 07:24:27.000000 pyzjr-0.0.3/
+-rw-rw-rw-   0        0        0      696 2023-07-02 07:24:27.000000 pyzjr-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       21 2023-06-10 05:53:05.000000 pyzjr-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-02 07:24:27.000000 pyzjr-0.0.3/pyzjr/
+-rw-rw-rw-   0        0        0      104 2023-06-10 05:53:05.000000 pyzjr-0.0.3/pyzjr/Z.py
+-rw-rw-rw-   0        0        0      765 2023-07-02 07:24:04.000000 pyzjr-0.0.3/pyzjr/__init__.py
+-rw-rw-rw-   0        0        0     4073 2023-06-10 05:53:05.000000 pyzjr-0.0.3/pyzjr/utils.py
+-rw-rw-rw-   0        0        0     2784 2023-06-10 05:53:05.000000 pyzjr-0.0.3/pyzjr/video.py
+drwxrwxrwx   0        0        0        0 2023-07-02 07:24:27.000000 pyzjr-0.0.3/pyzjr.egg-info/
+-rw-rw-rw-   0        0        0      696 2023-07-02 07:24:27.000000 pyzjr-0.0.3/pyzjr.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      193 2023-07-02 07:24:27.000000 pyzjr-0.0.3/pyzjr.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-02 07:24:27.000000 pyzjr-0.0.3/pyzjr.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-07-02 07:24:27.000000 pyzjr-0.0.3/pyzjr.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-02 07:24:27.000000 pyzjr-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1734 2023-07-02 07:24:17.000000 pyzjr-0.0.3/setup.py
```

### Comparing `pyzjr-0.0.2/PKG-INFO` & `pyzjr-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyzjr
-Version: 0.0.2
+Version: 0.0.3
 Summary:  a computer vision library that supports both Win and Mac 
 Home-page: https://github.com/Auorui/pyzjr
 Author: Auorui
 Author-email: zjricetea@gmail.com
 License: MIT
 Description: 
         # pyzjr
```

### Comparing `pyzjr-0.0.2/pyzjr/__init__.py` & `pyzjr-0.0.3/pyzjr/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,16 +11,15 @@
 
 """
 from pyzjr import pyps as ps  # Using Image Processing
 from pyzjr import pysift as sift  # Using SIFT matching algorithm
 from pyzjr import Color as color
 """
 
-
-__version__ = "0.0.2"
+__version__ = "0.0.3"
 
 import cv2
 
 repair_TELEA=cv2.INPAINT_TELEA
 repair_NS=cv2.INPAINT_NS
 Lap_64F=cv2.CV_64F
```

### Comparing `pyzjr-0.0.2/pyzjr/utils.py` & `pyzjr-0.0.3/pyzjr/utils.py`

 * *Files identical despite different names*

### Comparing `pyzjr-0.0.2/pyzjr/video.py` & `pyzjr-0.0.3/pyzjr/video.py`

 * *Files identical despite different names*

### Comparing `pyzjr-0.0.2/pyzjr.egg-info/PKG-INFO` & `pyzjr-0.0.3/pyzjr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyzjr
-Version: 0.0.2
+Version: 0.0.3
 Summary:  a computer vision library that supports both Win and Mac 
 Home-page: https://github.com/Auorui/pyzjr
 Author: Auorui
 Author-email: zjricetea@gmail.com
 License: MIT
 Description: 
         # pyzjr
```

### Comparing `pyzjr-0.0.2/setup.py` & `pyzjr-0.0.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 # these things are needed for the README.md show on pypi (if you dont need delete it)
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
 # you need to change all these
-VERSION = '0.0.2'
+VERSION = '0.0.3'
 DESCRIPTION = ' a computer vision library that supports both Win and Mac '
 LONG_DESCRIPTION = 'pyzjr is a computer vision library that supports both Win and Mac'
 
 setup(
     name="pyzjr",
     version=VERSION,
     author="Auorui",
```

