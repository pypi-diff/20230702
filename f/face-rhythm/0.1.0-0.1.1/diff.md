# Comparing `tmp/face_rhythm-0.1.0.tar.gz` & `tmp/face_rhythm-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "face_rhythm-0.1.0.tar", last modified: Sun Jul  2 20:47:35 2023, max compression
+gzip compressed data, was "face_rhythm-0.1.1.tar", last modified: Sun Jul  2 21:12:25 2023, max compression
```

## Comparing `face_rhythm-0.1.0.tar` & `face_rhythm-0.1.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-02 20:47:35.205504 face_rhythm-0.1.0/
--rwxrwxrwx   0 root         (0) root         (0)       52 2022-12-06 23:48:14.000000 face_rhythm-0.1.0/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)     5990 2023-07-02 20:47:35.205270 face_rhythm-0.1.0/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     5473 2022-12-14 16:31:29.000000 face_rhythm-0.1.0/README.md
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-02 20:47:35.203559 face_rhythm-0.1.0/face_rhythm/
--rwxrwxrwx   0 root         (0) root         (0)      499 2023-07-02 20:45:21.000000 face_rhythm-0.1.0/face_rhythm/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     8633 2023-05-12 20:21:02.000000 face_rhythm-0.1.0/face_rhythm/data_importing.py
--rwxrwxrwx   0 root         (0) root         (0)    32078 2023-05-13 04:09:53.000000 face_rhythm-0.1.0/face_rhythm/decomposition.py
--rwxrwxrwx   0 root         (0) root         (0)    11685 2023-05-12 00:14:16.000000 face_rhythm-0.1.0/face_rhythm/h5_handling.py
--rwxrwxrwx   0 root         (0) root         (0)   126521 2023-07-02 14:34:25.000000 face_rhythm-0.1.0/face_rhythm/helpers.py
--rwxrwxrwx   0 root         (0) root         (0)    30187 2023-07-02 14:05:50.000000 face_rhythm-0.1.0/face_rhythm/point_tracking.py
--rwxrwxrwx   0 root         (0) root         (0)     3460 2023-07-02 17:54:14.000000 face_rhythm-0.1.0/face_rhythm/project.py
--rwxrwxrwx   0 root         (0) root         (0)    67492 2023-07-02 00:34:16.000000 face_rhythm-0.1.0/face_rhythm/rois.py
--rwxrwxrwx   0 root         (0) root         (0)    14562 2023-05-13 02:35:47.000000 face_rhythm-0.1.0/face_rhythm/spectral_analysis.py
--rwxrwxrwx   0 root         (0) root         (0)    41698 2023-07-02 17:53:13.000000 face_rhythm-0.1.0/face_rhythm/util.py
--rwxrwxrwx   0 root         (0) root         (0)    31210 2023-05-13 02:22:13.000000 face_rhythm-0.1.0/face_rhythm/visualization.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-02 20:47:35.204869 face_rhythm-0.1.0/face_rhythm.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)     5990 2023-07-02 20:47:35.000000 face_rhythm-0.1.0/face_rhythm.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      454 2023-07-02 20:47:35.000000 face_rhythm-0.1.0/face_rhythm.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2023-07-02 20:47:35.000000 face_rhythm-0.1.0/face_rhythm.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)       12 2023-07-02 20:47:35.000000 face_rhythm-0.1.0/face_rhythm.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)       38 2023-07-02 20:47:35.205594 face_rhythm-0.1.0/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     2653 2023-01-07 06:49:49.000000 face_rhythm-0.1.0/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-02 21:12:25.602818 face_rhythm-0.1.1/
+-rwxrwxrwx   0 root         (0) root         (0)       52 2022-12-06 23:48:14.000000 face_rhythm-0.1.1/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)     5990 2023-07-02 21:12:25.602605 face_rhythm-0.1.1/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     5473 2022-12-14 16:31:29.000000 face_rhythm-0.1.1/README.md
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-02 21:12:25.595116 face_rhythm-0.1.1/face_rhythm/
+-rwxrwxrwx   0 root         (0) root         (0)      501 2023-07-02 21:10:31.000000 face_rhythm-0.1.1/face_rhythm/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     8633 2023-05-12 20:21:02.000000 face_rhythm-0.1.1/face_rhythm/data_importing.py
+-rwxrwxrwx   0 root         (0) root         (0)    32078 2023-05-13 04:09:53.000000 face_rhythm-0.1.1/face_rhythm/decomposition.py
+-rwxrwxrwx   0 root         (0) root         (0)    11685 2023-05-12 00:14:16.000000 face_rhythm-0.1.1/face_rhythm/h5_handling.py
+-rwxrwxrwx   0 root         (0) root         (0)   126521 2023-07-02 21:07:53.000000 face_rhythm-0.1.1/face_rhythm/helpers.py
+-rwxrwxrwx   0 root         (0) root         (0)    30187 2023-07-02 14:05:50.000000 face_rhythm-0.1.1/face_rhythm/point_tracking.py
+-rwxrwxrwx   0 root         (0) root         (0)     3460 2023-07-02 17:54:14.000000 face_rhythm-0.1.1/face_rhythm/project.py
+-rwxrwxrwx   0 root         (0) root         (0)    67492 2023-07-02 00:34:16.000000 face_rhythm-0.1.1/face_rhythm/rois.py
+-rwxrwxrwx   0 root         (0) root         (0)    14562 2023-05-13 02:35:47.000000 face_rhythm-0.1.1/face_rhythm/spectral_analysis.py
+-rwxrwxrwx   0 root         (0) root         (0)    41698 2023-07-02 17:53:13.000000 face_rhythm-0.1.1/face_rhythm/util.py
+-rwxrwxrwx   0 root         (0) root         (0)    31210 2023-05-13 02:22:13.000000 face_rhythm-0.1.1/face_rhythm/visualization.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-02 21:12:25.602220 face_rhythm-0.1.1/face_rhythm.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)     5990 2023-07-02 21:12:25.000000 face_rhythm-0.1.1/face_rhythm.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      454 2023-07-02 21:12:25.000000 face_rhythm-0.1.1/face_rhythm.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-07-02 21:12:25.000000 face_rhythm-0.1.1/face_rhythm.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)       12 2023-07-02 21:12:25.000000 face_rhythm-0.1.1/face_rhythm.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)       38 2023-07-02 21:12:25.602908 face_rhythm-0.1.1/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     2995 2023-07-02 21:12:13.000000 face_rhythm-0.1.1/setup.py
```

### Comparing `face_rhythm-0.1.0/PKG-INFO` & `face_rhythm-0.1.1/face_rhythm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: face_rhythm
-Version: 0.1.0
+Name: face-rhythm
+Version: 0.1.1
 Summary: A pipeline for analysis of facial behavior using optical flow
 Home-page: https://github.com/RichieHakim/face-rhythm
 Author: Rich Hakim
 Keywords: face beahvior optical flow
 Platform: Any
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `face_rhythm-0.1.0/README.md` & `face_rhythm-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `face_rhythm-0.1.0/face_rhythm/data_importing.py` & `face_rhythm-0.1.1/face_rhythm/data_importing.py`

 * *Files identical despite different names*

### Comparing `face_rhythm-0.1.0/face_rhythm/decomposition.py` & `face_rhythm-0.1.1/face_rhythm/decomposition.py`

 * *Files identical despite different names*

### Comparing `face_rhythm-0.1.0/face_rhythm/h5_handling.py` & `face_rhythm-0.1.1/face_rhythm/h5_handling.py`

 * *Files identical despite different names*

### Comparing `face_rhythm-0.1.0/face_rhythm/helpers.py` & `face_rhythm-0.1.1/face_rhythm/helpers.py`

 * *Files identical despite different names*

### Comparing `face_rhythm-0.1.0/face_rhythm/point_tracking.py` & `face_rhythm-0.1.1/face_rhythm/point_tracking.py`

 * *Files identical despite different names*

### Comparing `face_rhythm-0.1.0/face_rhythm/project.py` & `face_rhythm-0.1.1/face_rhythm/project.py`

 * *Files identical despite different names*

### Comparing `face_rhythm-0.1.0/face_rhythm/rois.py` & `face_rhythm-0.1.1/face_rhythm/rois.py`

 * *Files identical despite different names*

### Comparing `face_rhythm-0.1.0/face_rhythm/spectral_analysis.py` & `face_rhythm-0.1.1/face_rhythm/spectral_analysis.py`

 * *Files identical despite different names*

### Comparing `face_rhythm-0.1.0/face_rhythm/util.py` & `face_rhythm-0.1.1/face_rhythm/util.py`

 * *Files identical despite different names*

### Comparing `face_rhythm-0.1.0/face_rhythm/visualization.py` & `face_rhythm-0.1.1/face_rhythm/visualization.py`

 * *Files identical despite different names*

### Comparing `face_rhythm-0.1.0/face_rhythm.egg-info/PKG-INFO` & `face_rhythm-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: face-rhythm
-Version: 0.1.0
+Name: face_rhythm
+Version: 0.1.1
 Summary: A pipeline for analysis of facial behavior using optical flow
 Home-page: https://github.com/RichieHakim/face-rhythm
 Author: Rich Hakim
 Keywords: face beahvior optical flow
 Platform: Any
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `face_rhythm-0.1.0/setup.py` & `face_rhythm-0.1.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,29 +2,41 @@
 See:
 https://packaging.python.org/en/latest/distributing.html
 https://github.com/pypa/sampleproject
 """
 
 import setuptools
 from codecs import open
-from os import path
+import os
+from pathlib import Path
 
-here = path.abspath(path.dirname(__file__))
+dir_parent = Path(__file__).parent
+
+here = os.path.abspath(os.path.dirname(__file__))
 
 # Get the long description from the README file
-with open(path.join(here, 'README.md'), encoding='utf-8') as f:
+with open(os.path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 # with open('requirements.txt', 'r') as f:
 #     requirements = f.read().splitlines()
 # print(requirements)
 
+## Get version number
+with open(str(dir_parent / "face_rhythm" / "__init__.py"), "r") as f:
+    for line in f:
+        if line.startswith("__version__"):
+            version = line.split("=")[1].strip().replace("\"", "").replace("\'", "")
+            break
+
+
 setuptools.setup(
     name='face_rhythm',
-    version='0.1.0',
+    version=version,
+    # version='0.1.1',
 
     description="A pipeline for analysis of facial behavior using optical flow",
     long_description=long_description,
     long_description_content_type='text/markdown',
 
     # The project's main homepage.
     url='https://github.com/RichieHakim/face-rhythm',
```

