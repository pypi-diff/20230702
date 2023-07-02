# Comparing `tmp/pyzjr-0.0.4.tar.gz` & `tmp/pyzjr-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pyzjr-0.0.4.tar", last modified: Sun Jul  2 07:46:43 2023, max compression
+gzip compressed data, was "dist\pyzjr-0.0.7.tar", last modified: Sun Jul  2 08:17:51 2023, max compression
```

## Comparing `pyzjr-0.0.4.tar` & `pyzjr-0.0.7.tar`

### file list

```diff
@@ -1,15 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-07-02 07:46:43.000000 pyzjr-0.0.4/
--rw-rw-rw-   0        0        0      696 2023-07-02 07:46:43.000000 pyzjr-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0       21 2023-06-10 05:53:05.000000 pyzjr-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-07-02 07:46:43.000000 pyzjr-0.0.4/pyzjr/
--rw-rw-rw-   0        0        0      104 2023-06-10 05:53:05.000000 pyzjr-0.0.4/pyzjr/Z.py
--rw-rw-rw-   0        0        0     1071 2023-07-02 07:46:35.000000 pyzjr-0.0.4/pyzjr/__init__.py
--rw-rw-rw-   0        0        0     4073 2023-06-10 05:53:05.000000 pyzjr-0.0.4/pyzjr/utils.py
--rw-rw-rw-   0        0        0     2784 2023-06-10 05:53:05.000000 pyzjr-0.0.4/pyzjr/video.py
-drwxrwxrwx   0        0        0        0 2023-07-02 07:46:43.000000 pyzjr-0.0.4/pyzjr.egg-info/
--rw-rw-rw-   0        0        0      696 2023-07-02 07:46:43.000000 pyzjr-0.0.4/pyzjr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      193 2023-07-02 07:46:43.000000 pyzjr-0.0.4/pyzjr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-02 07:46:43.000000 pyzjr-0.0.4/pyzjr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-07-02 07:46:43.000000 pyzjr-0.0.4/pyzjr.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-02 07:46:43.000000 pyzjr-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1734 2023-07-02 07:46:32.000000 pyzjr-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-02 08:17:51.000000 pyzjr-0.0.7/
+-rw-rw-rw-   0        0        0      734 2023-07-02 08:17:51.000000 pyzjr-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0       41 2023-07-02 08:17:25.000000 pyzjr-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-07-02 08:17:51.000000 pyzjr-0.0.7/pyzjr/
+-rw-rw-rw-   0        0        0     3959 2023-07-02 08:05:46.000000 pyzjr-0.0.7/pyzjr/ColorModule.py
+-rw-rw-rw-   0        0        0    18261 2023-07-02 08:05:42.000000 pyzjr-0.0.7/pyzjr/Enimage.py
+-rw-rw-rw-   0        0        0     3624 2023-06-10 05:53:05.000000 pyzjr-0.0.7/pyzjr/PIC.py
+-rw-rw-rw-   0        0        0     4538 2023-07-02 08:05:25.000000 pyzjr-0.0.7/pyzjr/TrackBar.py
+-rw-rw-rw-   0        0        0      104 2023-06-10 05:53:05.000000 pyzjr-0.0.7/pyzjr/Z.py
+-rw-rw-rw-   0        0        0     1071 2023-07-02 08:17:00.000000 pyzjr-0.0.7/pyzjr/__init__.py
+-rw-rw-rw-   0        0        0     5022 2023-06-10 05:53:05.000000 pyzjr-0.0.7/pyzjr/definition.py
+-rw-rw-rw-   0        0        0     4073 2023-06-10 05:53:05.000000 pyzjr-0.0.7/pyzjr/utils.py
+-rw-rw-rw-   0        0        0     2784 2023-06-10 05:53:05.000000 pyzjr-0.0.7/pyzjr/video.py
+drwxrwxrwx   0        0        0        0 2023-07-02 08:17:51.000000 pyzjr-0.0.7/pyzjr.egg-info/
+-rw-rw-rw-   0        0        0      734 2023-07-02 08:17:51.000000 pyzjr-0.0.7/pyzjr.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      282 2023-07-02 08:17:51.000000 pyzjr-0.0.7/pyzjr.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-02 08:17:51.000000 pyzjr-0.0.7/pyzjr.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-07-02 08:17:51.000000 pyzjr-0.0.7/pyzjr.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-02 08:17:51.000000 pyzjr-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1734 2023-07-02 08:17:03.000000 pyzjr-0.0.7/setup.py
```

### Comparing `pyzjr-0.0.4/PKG-INFO` & `pyzjr-0.0.7/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 Metadata-Version: 2.1
 Name: pyzjr
-Version: 0.0.4
+Version: 0.0.7
 Summary:  a computer vision library that supports both Win and Mac 
 Home-page: https://github.com/Auorui/pyzjr
 Author: Auorui
 Author-email: zjricetea@gmail.com
 License: MIT
 Description: 
         # pyzjr
         个人私库
         
+        介绍后面补充
+        
 Keywords: python,computer vision,pyzjr,windows,mac,linux
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
```

### Comparing `pyzjr-0.0.4/pyzjr/__init__.py` & `pyzjr-0.0.7/pyzjr/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 """
 from pyzjr import pyps as ps  # Using Image Processing
 from pyzjr import pysift as sift  # Using SIFT matching algorithm
 from pyzjr import Color as color
 """
 
-__version__ = "0.0.4"
+__version__ = "0.0.7"
 
 import cv2
 from pyzjr.PIC import download_file,getPhotopath,Pic_rename,read_resize_image,\
                       load_images_from_folder,save_images
 from pyzjr.Enimage import Filter,Enhance,Random_Enhance,Retinex,\
                           repair_Img
 from pyzjr.definition import Fuzzy_image,Clear_quantification
```

### Comparing `pyzjr-0.0.4/pyzjr/utils.py` & `pyzjr-0.0.7/pyzjr/utils.py`

 * *Files identical despite different names*

### Comparing `pyzjr-0.0.4/pyzjr/video.py` & `pyzjr-0.0.7/pyzjr/video.py`

 * *Files identical despite different names*

### Comparing `pyzjr-0.0.4/pyzjr.egg-info/PKG-INFO` & `pyzjr-0.0.7/pyzjr.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 Metadata-Version: 2.1
 Name: pyzjr
-Version: 0.0.4
+Version: 0.0.7
 Summary:  a computer vision library that supports both Win and Mac 
 Home-page: https://github.com/Auorui/pyzjr
 Author: Auorui
 Author-email: zjricetea@gmail.com
 License: MIT
 Description: 
         # pyzjr
         个人私库
         
+        介绍后面补充
+        
 Keywords: python,computer vision,pyzjr,windows,mac,linux
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
```

### Comparing `pyzjr-0.0.4/setup.py` & `pyzjr-0.0.7/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 # these things are needed for the README.md show on pypi (if you dont need delete it)
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
 # you need to change all these
-VERSION = '0.0.4'
+VERSION = '0.0.7'
 DESCRIPTION = ' a computer vision library that supports both Win and Mac '
 LONG_DESCRIPTION = 'pyzjr is a computer vision library that supports both Win and Mac'
 
 setup(
     name="pyzjr",
     version=VERSION,
     author="Auorui",
```

