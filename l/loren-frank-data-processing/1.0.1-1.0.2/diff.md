# Comparing `tmp/loren_frank_data_processing-1.0.1.tar.gz` & `tmp/loren_frank_data_processing-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loren_frank_data_processing-1.0.1.tar", last modified: Sat Jul  1 22:14:45 2023, max compression
+gzip compressed data, was "loren_frank_data_processing-1.0.2.tar", last modified: Sat Jul  1 22:49:50 2023, max compression
```

## Comparing `loren_frank_data_processing-1.0.1.tar` & `loren_frank_data_processing-1.0.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 edeno      (501) staff       (20)        0 2023-07-01 22:14:45.414255 loren_frank_data_processing-1.0.1/
--rw-r--r--   0 edeno      (501) staff       (20)    35139 2017-10-24 18:08:07.000000 loren_frank_data_processing-1.0.1/LICENSE
--rw-r--r--   0 edeno      (501) staff       (20)      277 2023-07-01 22:14:45.414336 loren_frank_data_processing-1.0.1/PKG-INFO
--rw-r--r--   0 edeno      (501) staff       (20)     2910 2022-10-17 17:51:30.000000 loren_frank_data_processing-1.0.1/README.md
-drwxr-xr-x   0 edeno      (501) staff       (20)        0 2023-07-01 22:14:45.412961 loren_frank_data_processing-1.0.1/loren_frank_data_processing/
--rw-r--r--   0 edeno      (501) staff       (20)     1504 2023-07-01 22:11:52.000000 loren_frank_data_processing-1.0.1/loren_frank_data_processing/DIO.py
--rw-r--r--   0 edeno      (501) staff       (20)      878 2023-07-01 22:11:45.000000 loren_frank_data_processing-1.0.1/loren_frank_data_processing/__init__.py
--rw-r--r--   0 edeno      (501) staff       (20)     4112 2023-07-01 22:11:49.000000 loren_frank_data_processing-1.0.1/loren_frank_data_processing/core.py
--rw-r--r--   0 edeno      (501) staff       (20)     6692 2023-07-01 22:11:59.000000 loren_frank_data_processing-1.0.1/loren_frank_data_processing/multiunit.py
--rw-r--r--   0 edeno      (501) staff       (20)     8430 2023-07-01 22:12:03.000000 loren_frank_data_processing-1.0.1/loren_frank_data_processing/neurons.py
--rw-r--r--   0 edeno      (501) staff       (20)    16882 2023-07-01 22:12:10.000000 loren_frank_data_processing-1.0.1/loren_frank_data_processing/position.py
--rw-r--r--   0 edeno      (501) staff       (20)     3729 2023-07-01 22:12:14.000000 loren_frank_data_processing-1.0.1/loren_frank_data_processing/ripples.py
--rw-r--r--   0 edeno      (501) staff       (20)      879 2023-07-01 22:12:19.000000 loren_frank_data_processing-1.0.1/loren_frank_data_processing/saving.py
--rw-r--r--   0 edeno      (501) staff       (20)     2654 2023-07-01 22:12:23.000000 loren_frank_data_processing-1.0.1/loren_frank_data_processing/task.py
--rw-r--r--   0 edeno      (501) staff       (20)     7636 2023-07-01 22:12:28.000000 loren_frank_data_processing-1.0.1/loren_frank_data_processing/tetrodes.py
--rw-r--r--   0 edeno      (501) staff       (20)    14408 2023-07-01 22:12:33.000000 loren_frank_data_processing-1.0.1/loren_frank_data_processing/track_segment_classification.py
--rw-r--r--   0 edeno      (501) staff       (20)     9600 2023-07-01 22:12:37.000000 loren_frank_data_processing-1.0.1/loren_frank_data_processing/utilities.py
--rw-r--r--   0 edeno      (501) staff       (20)     4281 2023-07-01 22:12:43.000000 loren_frank_data_processing-1.0.1/loren_frank_data_processing/visualization.py
--rw-r--r--   0 edeno      (501) staff       (20)    10120 2023-07-01 22:12:46.000000 loren_frank_data_processing-1.0.1/loren_frank_data_processing/well_traversal_classification.py
-drwxr-xr-x   0 edeno      (501) staff       (20)        0 2023-07-01 22:14:45.413673 loren_frank_data_processing-1.0.1/loren_frank_data_processing.egg-info/
--rw-r--r--   0 edeno      (501) staff       (20)      277 2023-07-01 22:14:45.000000 loren_frank_data_processing-1.0.1/loren_frank_data_processing.egg-info/PKG-INFO
--rw-r--r--   0 edeno      (501) staff       (20)      925 2023-07-01 22:14:45.000000 loren_frank_data_processing-1.0.1/loren_frank_data_processing.egg-info/SOURCES.txt
--rw-r--r--   0 edeno      (501) staff       (20)        1 2023-07-01 22:14:45.000000 loren_frank_data_processing-1.0.1/loren_frank_data_processing.egg-info/dependency_links.txt
--rw-r--r--   0 edeno      (501) staff       (20)       80 2023-07-01 22:14:45.000000 loren_frank_data_processing-1.0.1/loren_frank_data_processing.egg-info/requires.txt
--rw-r--r--   0 edeno      (501) staff       (20)       28 2023-07-01 22:14:45.000000 loren_frank_data_processing-1.0.1/loren_frank_data_processing.egg-info/top_level.txt
--rw-r--r--   0 edeno      (501) staff       (20)       63 2023-07-01 22:14:45.414617 loren_frank_data_processing-1.0.1/setup.cfg
--rw-r--r--   0 edeno      (501) staff       (20)      657 2023-07-01 22:13:25.000000 loren_frank_data_processing-1.0.1/setup.py
-drwxr-xr-x   0 edeno      (501) staff       (20)        0 2023-07-01 22:14:45.414071 loren_frank_data_processing-1.0.1/tests/
--rw-r--r--   0 edeno      (501) staff       (20)     1508 2022-10-17 17:51:50.000000 loren_frank_data_processing-1.0.1/tests/test_core_.py
--rw-r--r--   0 edeno      (501) staff       (20)      580 2022-10-17 17:51:55.000000 loren_frank_data_processing-1.0.1/tests/test_utilities.py
+drwxr-xr-x   0 edeno      (501) staff       (20)        0 2023-07-01 22:49:50.354158 loren_frank_data_processing-1.0.2/
+-rw-r--r--   0 edeno      (501) staff       (20)    35139 2017-10-24 18:08:07.000000 loren_frank_data_processing-1.0.2/LICENSE
+-rw-r--r--   0 edeno      (501) staff       (20)      277 2023-07-01 22:49:50.354260 loren_frank_data_processing-1.0.2/PKG-INFO
+-rw-r--r--   0 edeno      (501) staff       (20)     2910 2022-10-17 17:51:30.000000 loren_frank_data_processing-1.0.2/README.md
+drwxr-xr-x   0 edeno      (501) staff       (20)        0 2023-07-01 22:49:50.352867 loren_frank_data_processing-1.0.2/loren_frank_data_processing/
+-rw-r--r--   0 edeno      (501) staff       (20)     1504 2023-07-01 22:11:52.000000 loren_frank_data_processing-1.0.2/loren_frank_data_processing/DIO.py
+-rw-r--r--   0 edeno      (501) staff       (20)      878 2023-07-01 22:11:45.000000 loren_frank_data_processing-1.0.2/loren_frank_data_processing/__init__.py
+-rw-r--r--   0 edeno      (501) staff       (20)     4112 2023-07-01 22:11:49.000000 loren_frank_data_processing-1.0.2/loren_frank_data_processing/core.py
+-rw-r--r--   0 edeno      (501) staff       (20)     6692 2023-07-01 22:11:59.000000 loren_frank_data_processing-1.0.2/loren_frank_data_processing/multiunit.py
+-rw-r--r--   0 edeno      (501) staff       (20)     8430 2023-07-01 22:12:03.000000 loren_frank_data_processing-1.0.2/loren_frank_data_processing/neurons.py
+-rw-r--r--   0 edeno      (501) staff       (20)    16882 2023-07-01 22:12:10.000000 loren_frank_data_processing-1.0.2/loren_frank_data_processing/position.py
+-rw-r--r--   0 edeno      (501) staff       (20)     3729 2023-07-01 22:12:14.000000 loren_frank_data_processing-1.0.2/loren_frank_data_processing/ripples.py
+-rw-r--r--   0 edeno      (501) staff       (20)      879 2023-07-01 22:12:19.000000 loren_frank_data_processing-1.0.2/loren_frank_data_processing/saving.py
+-rw-r--r--   0 edeno      (501) staff       (20)     2666 2023-07-01 22:48:48.000000 loren_frank_data_processing-1.0.2/loren_frank_data_processing/task.py
+-rw-r--r--   0 edeno      (501) staff       (20)     7636 2023-07-01 22:12:28.000000 loren_frank_data_processing-1.0.2/loren_frank_data_processing/tetrodes.py
+-rw-r--r--   0 edeno      (501) staff       (20)    14408 2023-07-01 22:12:33.000000 loren_frank_data_processing-1.0.2/loren_frank_data_processing/track_segment_classification.py
+-rw-r--r--   0 edeno      (501) staff       (20)     9600 2023-07-01 22:12:37.000000 loren_frank_data_processing-1.0.2/loren_frank_data_processing/utilities.py
+-rw-r--r--   0 edeno      (501) staff       (20)     4281 2023-07-01 22:12:43.000000 loren_frank_data_processing-1.0.2/loren_frank_data_processing/visualization.py
+-rw-r--r--   0 edeno      (501) staff       (20)    10120 2023-07-01 22:12:46.000000 loren_frank_data_processing-1.0.2/loren_frank_data_processing/well_traversal_classification.py
+drwxr-xr-x   0 edeno      (501) staff       (20)        0 2023-07-01 22:49:50.353749 loren_frank_data_processing-1.0.2/loren_frank_data_processing.egg-info/
+-rw-r--r--   0 edeno      (501) staff       (20)      277 2023-07-01 22:49:50.000000 loren_frank_data_processing-1.0.2/loren_frank_data_processing.egg-info/PKG-INFO
+-rw-r--r--   0 edeno      (501) staff       (20)      925 2023-07-01 22:49:50.000000 loren_frank_data_processing-1.0.2/loren_frank_data_processing.egg-info/SOURCES.txt
+-rw-r--r--   0 edeno      (501) staff       (20)        1 2023-07-01 22:49:50.000000 loren_frank_data_processing-1.0.2/loren_frank_data_processing.egg-info/dependency_links.txt
+-rw-r--r--   0 edeno      (501) staff       (20)       80 2023-07-01 22:49:50.000000 loren_frank_data_processing-1.0.2/loren_frank_data_processing.egg-info/requires.txt
+-rw-r--r--   0 edeno      (501) staff       (20)       28 2023-07-01 22:49:50.000000 loren_frank_data_processing-1.0.2/loren_frank_data_processing.egg-info/top_level.txt
+-rw-r--r--   0 edeno      (501) staff       (20)       63 2023-07-01 22:49:50.354560 loren_frank_data_processing-1.0.2/setup.cfg
+-rw-r--r--   0 edeno      (501) staff       (20)      657 2023-07-01 22:49:08.000000 loren_frank_data_processing-1.0.2/setup.py
+drwxr-xr-x   0 edeno      (501) staff       (20)        0 2023-07-01 22:49:50.354038 loren_frank_data_processing-1.0.2/tests/
+-rw-r--r--   0 edeno      (501) staff       (20)     1508 2022-10-17 17:51:50.000000 loren_frank_data_processing-1.0.2/tests/test_core_.py
+-rw-r--r--   0 edeno      (501) staff       (20)      580 2022-10-17 17:51:55.000000 loren_frank_data_processing-1.0.2/tests/test_utilities.py
```

### Comparing `loren_frank_data_processing-1.0.1/LICENSE` & `loren_frank_data_processing-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `loren_frank_data_processing-1.0.1/README.md` & `loren_frank_data_processing-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `loren_frank_data_processing-1.0.1/loren_frank_data_processing/DIO.py` & `loren_frank_data_processing-1.0.2/loren_frank_data_processing/DIO.py`

 * *Files identical despite different names*

### Comparing `loren_frank_data_processing-1.0.1/loren_frank_data_processing/__init__.py` & `loren_frank_data_processing-1.0.2/loren_frank_data_processing/__init__.py`

 * *Files identical despite different names*

### Comparing `loren_frank_data_processing-1.0.1/loren_frank_data_processing/core.py` & `loren_frank_data_processing-1.0.2/loren_frank_data_processing/core.py`

 * *Files identical despite different names*

### Comparing `loren_frank_data_processing-1.0.1/loren_frank_data_processing/multiunit.py` & `loren_frank_data_processing-1.0.2/loren_frank_data_processing/multiunit.py`

 * *Files identical despite different names*

### Comparing `loren_frank_data_processing-1.0.1/loren_frank_data_processing/neurons.py` & `loren_frank_data_processing-1.0.2/loren_frank_data_processing/neurons.py`

 * *Files identical despite different names*

### Comparing `loren_frank_data_processing-1.0.1/loren_frank_data_processing/position.py` & `loren_frank_data_processing-1.0.2/loren_frank_data_processing/position.py`

 * *Files identical despite different names*

### Comparing `loren_frank_data_processing-1.0.1/loren_frank_data_processing/ripples.py` & `loren_frank_data_processing-1.0.2/loren_frank_data_processing/ripples.py`

 * *Files identical despite different names*

### Comparing `loren_frank_data_processing-1.0.1/loren_frank_data_processing/saving.py` & `loren_frank_data_processing-1.0.2/loren_frank_data_processing/saving.py`

 * *Files identical despite different names*

### Comparing `loren_frank_data_processing-1.0.1/loren_frank_data_processing/task.py` & `loren_frank_data_processing-1.0.2/loren_frank_data_processing/task.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     df["exposure"] = np.arange(len(df)) + 1
     return df
 
 
 def compute_exposure(epoch_info):
     df = epoch_info.groupby(["animal", "environment"]).apply(_count_exposure)
     df["exposure"] = df.exposure.where(
-        ~epoch_info.type.isin(["sleep", "rest", "nan", "failed sleep"])
+        ~epoch_info.type.isin(["sleep", "rest", "nan", "failed sleep"]).to_numpy(),
     )
     return df
 
 
 def get_task(animal):
     """Loads all experimental information for all days for a given animal.
```

### Comparing `loren_frank_data_processing-1.0.1/loren_frank_data_processing/tetrodes.py` & `loren_frank_data_processing-1.0.2/loren_frank_data_processing/tetrodes.py`

 * *Files identical despite different names*

### Comparing `loren_frank_data_processing-1.0.1/loren_frank_data_processing/track_segment_classification.py` & `loren_frank_data_processing-1.0.2/loren_frank_data_processing/track_segment_classification.py`

 * *Files identical despite different names*

### Comparing `loren_frank_data_processing-1.0.1/loren_frank_data_processing/utilities.py` & `loren_frank_data_processing-1.0.2/loren_frank_data_processing/utilities.py`

 * *Files identical despite different names*

### Comparing `loren_frank_data_processing-1.0.1/loren_frank_data_processing/visualization.py` & `loren_frank_data_processing-1.0.2/loren_frank_data_processing/visualization.py`

 * *Files identical despite different names*

### Comparing `loren_frank_data_processing-1.0.1/loren_frank_data_processing/well_traversal_classification.py` & `loren_frank_data_processing-1.0.2/loren_frank_data_processing/well_traversal_classification.py`

 * *Files identical despite different names*

### Comparing `loren_frank_data_processing-1.0.1/loren_frank_data_processing.egg-info/SOURCES.txt` & `loren_frank_data_processing-1.0.2/loren_frank_data_processing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `loren_frank_data_processing-1.0.1/setup.py` & `loren_frank_data_processing-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     "networkx >= 2.0.0",
     "matplotlib",
 ]
 TESTS_REQUIRE = ["pytest >= 2.7.1"]
 
 setup(
     name="loren_frank_data_processing",
-    version="1.0.1",
+    version="1.0.2",
     license="GPL-3.0",
     description=("Import data from Loren Frank lab"),
     author="Eric Denovellis",
     author_email="edeno@bu.edu",
     url="https://github.com/Eden-Kramer-Lab/loren_frank_data_processing",
     packages=find_packages(),
     install_requires=INSTALL_REQUIRES,
```

### Comparing `loren_frank_data_processing-1.0.1/tests/test_core_.py` & `loren_frank_data_processing-1.0.2/tests/test_core_.py`

 * *Files identical despite different names*

### Comparing `loren_frank_data_processing-1.0.1/tests/test_utilities.py` & `loren_frank_data_processing-1.0.2/tests/test_utilities.py`

 * *Files identical despite different names*

