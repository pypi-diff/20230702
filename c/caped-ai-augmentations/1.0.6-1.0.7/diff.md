# Comparing `tmp/caped-ai-augmentations-1.0.6.tar.gz` & `tmp/caped-ai-augmentations-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/mnt/c/Users/rando/Downloads/Python_Workspace/caped-ai-augmentations/dist/.tmp-ibbtoh4a/caped-ai-augmentations-1.0.6.tar", last modified: Sun Jun 25 12:38:41 2023, max compression
+gzip compressed data, was "caped-ai-augmentations-1.0.7.tar", last modified: Sun Jul  2 19:04:46 2023, max compression
```

## Comparing `caped-ai-augmentations-1.0.6.tar` & `caped-ai-augmentations-1.0.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-25 12:38:41.582453 caped-ai-augmentations-1.0.6/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1512 2022-09-07 10:32:19.000000 caped-ai-augmentations-1.0.6/LICENSE
--rwxrwxrwx   0 debian    (1000) debian    (1000)      738 2023-06-25 12:38:41.578451 caped-ai-augmentations-1.0.6/PKG-INFO
--rwxrwxrwx   0 debian    (1000) debian    (1000)       75 2022-09-07 10:16:18.000000 caped-ai-augmentations-1.0.6/README.md
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-25 12:38:41.395400 caped-ai-augmentations-1.0.6/caped_ai_augmentations/
--rwxrwxrwx   0 debian    (1000) debian    (1000)    11274 2022-10-03 15:24:38.000000 caped-ai-augmentations-1.0.6/caped_ai_augmentations/AugmentTYXCsv.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)    11983 2022-10-03 15:24:27.000000 caped-ai-augmentations-1.0.6/caped_ai_augmentations/AugmentTZYXCsv.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)    11894 2022-12-23 20:19:23.000000 caped-ai-augmentations-1.0.6/caped_ai_augmentations/AugmentYX.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)    12485 2022-12-23 15:45:33.000000 caped-ai-augmentations-1.0.6/caped_ai_augmentations/AugmentYXC.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)    13152 2022-10-03 15:25:00.000000 caped-ai-augmentations-1.0.6/caped_ai_augmentations/AugmentZYX.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)      315 2022-10-12 12:10:32.000000 caped-ai-augmentations-1.0.6/caped_ai_augmentations/__init__.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)      105 2023-06-25 12:38:07.000000 caped-ai-augmentations-1.0.6/caped_ai_augmentations/_version.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)     4537 2022-12-23 19:35:26.000000 caped-ai-augmentations-1.0.6/caped_ai_augmentations/utils.py
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-25 12:38:41.540733 caped-ai-augmentations-1.0.6/caped_ai_augmentations.egg-info/
--rwxrwxrwx   0 debian    (1000) debian    (1000)      738 2023-06-25 12:38:40.000000 caped-ai-augmentations-1.0.6/caped_ai_augmentations.egg-info/PKG-INFO
--rwxrwxrwx   0 debian    (1000) debian    (1000)      548 2023-06-25 12:38:41.000000 caped-ai-augmentations-1.0.6/caped_ai_augmentations.egg-info/SOURCES.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)        1 2023-06-25 12:38:40.000000 caped-ai-augmentations-1.0.6/caped_ai_augmentations.egg-info/dependency_links.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       66 2023-06-25 12:38:40.000000 caped-ai-augmentations-1.0.6/caped_ai_augmentations.egg-info/requires.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       23 2023-06-25 12:38:40.000000 caped-ai-augmentations-1.0.6/caped_ai_augmentations.egg-info/top_level.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       38 2023-06-25 12:38:41.599793 caped-ai-augmentations-1.0.6/setup.cfg
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1289 2023-06-25 12:37:58.000000 caped-ai-augmentations-1.0.6/setup.py
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-02 19:04:46.296342 caped-ai-augmentations-1.0.7/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1512 2022-09-07 10:32:19.000000 caped-ai-augmentations-1.0.7/LICENSE
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      738 2023-07-02 19:04:46.290757 caped-ai-augmentations-1.0.7/PKG-INFO
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       75 2022-09-07 10:16:18.000000 caped-ai-augmentations-1.0.7/README.md
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-02 19:04:46.104431 caped-ai-augmentations-1.0.7/caped_ai_augmentations/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    11274 2022-10-03 15:24:38.000000 caped-ai-augmentations-1.0.7/caped_ai_augmentations/AugmentTYXCsv.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    11983 2022-10-03 15:24:27.000000 caped-ai-augmentations-1.0.7/caped_ai_augmentations/AugmentTZYXCsv.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    11894 2022-12-23 20:19:23.000000 caped-ai-augmentations-1.0.7/caped_ai_augmentations/AugmentYX.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    12485 2022-12-23 15:45:33.000000 caped-ai-augmentations-1.0.7/caped_ai_augmentations/AugmentYXC.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    13152 2022-10-03 15:25:00.000000 caped-ai-augmentations-1.0.7/caped_ai_augmentations/AugmentZYX.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      315 2022-10-12 12:10:32.000000 caped-ai-augmentations-1.0.7/caped_ai_augmentations/__init__.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      105 2023-07-02 19:03:39.000000 caped-ai-augmentations-1.0.7/caped_ai_augmentations/_version.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     4537 2022-12-23 19:35:26.000000 caped-ai-augmentations-1.0.7/caped_ai_augmentations/utils.py
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-02 19:04:46.255970 caped-ai-augmentations-1.0.7/caped_ai_augmentations.egg-info/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      738 2023-07-02 19:04:45.000000 caped-ai-augmentations-1.0.7/caped_ai_augmentations.egg-info/PKG-INFO
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      548 2023-07-02 19:04:45.000000 caped-ai-augmentations-1.0.7/caped_ai_augmentations.egg-info/SOURCES.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)        1 2023-07-02 19:04:45.000000 caped-ai-augmentations-1.0.7/caped_ai_augmentations.egg-info/dependency_links.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       71 2023-07-02 19:04:45.000000 caped-ai-augmentations-1.0.7/caped_ai_augmentations.egg-info/requires.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       23 2023-07-02 19:04:45.000000 caped-ai-augmentations-1.0.7/caped_ai_augmentations.egg-info/top_level.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       38 2023-07-02 19:04:46.297347 caped-ai-augmentations-1.0.7/setup.cfg
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1294 2023-07-02 19:03:29.000000 caped-ai-augmentations-1.0.7/setup.py
```

### Comparing `caped-ai-augmentations-1.0.6/LICENSE` & `caped-ai-augmentations-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `caped-ai-augmentations-1.0.6/PKG-INFO` & `caped-ai-augmentations-1.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caped-ai-augmentations
-Version: 1.0.6
+Version: 1.0.7
 Summary: Augmentations for volume, planar segmentation, classification image segmentation and associated csv file of oneat clicks.
 Home-page: https://github.com/Kapoorlabs-CAPED/Augmentations/
 Author: Varun Kapoor
 Author-email: randomaccessiblekapoor@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `caped-ai-augmentations-1.0.6/caped_ai_augmentations/AugmentTYXCsv.py` & `caped-ai-augmentations-1.0.7/caped_ai_augmentations/AugmentTYXCsv.py`

 * *Files identical despite different names*

### Comparing `caped-ai-augmentations-1.0.6/caped_ai_augmentations/AugmentTZYXCsv.py` & `caped-ai-augmentations-1.0.7/caped_ai_augmentations/AugmentTZYXCsv.py`

 * *Files identical despite different names*

### Comparing `caped-ai-augmentations-1.0.6/caped_ai_augmentations/AugmentYX.py` & `caped-ai-augmentations-1.0.7/caped_ai_augmentations/AugmentYX.py`

 * *Files identical despite different names*

### Comparing `caped-ai-augmentations-1.0.6/caped_ai_augmentations/AugmentYXC.py` & `caped-ai-augmentations-1.0.7/caped_ai_augmentations/AugmentYXC.py`

 * *Files identical despite different names*

### Comparing `caped-ai-augmentations-1.0.6/caped_ai_augmentations/AugmentZYX.py` & `caped-ai-augmentations-1.0.7/caped_ai_augmentations/AugmentZYX.py`

 * *Files identical despite different names*

### Comparing `caped-ai-augmentations-1.0.6/caped_ai_augmentations/utils.py` & `caped-ai-augmentations-1.0.7/caped_ai_augmentations/utils.py`

 * *Files identical despite different names*

### Comparing `caped-ai-augmentations-1.0.6/caped_ai_augmentations.egg-info/PKG-INFO` & `caped-ai-augmentations-1.0.7/caped_ai_augmentations.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caped-ai-augmentations
-Version: 1.0.6
+Version: 1.0.7
 Summary: Augmentations for volume, planar segmentation, classification image segmentation and associated csv file of oneat clicks.
 Home-page: https://github.com/Kapoorlabs-CAPED/Augmentations/
 Author: Varun Kapoor
 Author-email: randomaccessiblekapoor@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `caped-ai-augmentations-1.0.6/caped_ai_augmentations.egg-info/SOURCES.txt` & `caped-ai-augmentations-1.0.7/caped_ai_augmentations.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `caped-ai-augmentations-1.0.6/setup.py` & `caped-ai-augmentations-1.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     description='Augmentations for volume, planar segmentation, classification image segmentation and associated csv file of oneat clicks.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     install_requires=[
         "albumentations",
         "scipy",
         "opencv-python",
-        "sklearn",
+        "scikit-learn",
         "dask",
         "natsort",
         "photutils",
        
     ],
     packages=setuptools.find_packages(),
     classifiers=[
```

