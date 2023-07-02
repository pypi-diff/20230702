# Comparing `tmp/absplit-1.4.0.tar.gz` & `tmp/absplit-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "absplit-1.4.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "absplit-1.4.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `absplit-1.4.0.tar` & `absplit-1.4.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     4958 2023-06-05 23:23:06.124000 absplit-1.4.0/.gitignore
--rw-r--r--   0        0        0       50 2023-02-18 09:46:26.039000 absplit-1.4.0/.idea/.gitignore
--rw-r--r--   0        0        0      291 2023-06-12 08:40:13.087000 absplit-1.4.0/.idea/genetic_algorithm.iml
--rw-r--r--   0        0        0      179 2023-02-18 09:46:26.072000 absplit-1.4.0/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0      303 2023-06-12 08:40:13.168000 absplit-1.4.0/.idea/misc.xml
--rw-r--r--   0        0        0      293 2023-02-18 09:46:26.093000 absplit-1.4.0/.idea/modules.xml
--rw-r--r--   0        0        0      185 2023-02-18 09:46:26.104000 absplit-1.4.0/.idea/vcs.xml
--rw-r--r--   0        0        0     1026 2023-02-18 09:46:26.114000 absplit-1.4.0/LICENSE
--rw-r--r--   0        0        0      152 2023-02-18 09:46:26.124000 absplit-1.4.0/MANIFEST.in
--rw-r--r--   0        0        0     8252 2023-07-01 22:51:51.997000 absplit-1.4.0/README.md
--rw-r--r--   0        0        0       93 2023-07-01 22:51:52.048000 absplit-1.4.0/absplit/__init__.py
--rw-r--r--   0        0        0     8992 2023-07-01 22:59:45.945000 absplit-1.4.0/absplit/data.py
--rw-r--r--   0        0        0    29970 2023-07-01 22:54:24.935000 absplit-1.4.0/absplit/ga.py
--rw-r--r--   0        0        0     1866 2023-02-18 09:46:26.177000 absplit-1.4.0/absplit/param.py
--rw-r--r--   0        0        0     3978 2023-06-18 23:28:12.372000 absplit-1.4.0/absplit/tutorials.py
--rw-r--r--   0        0        0    29186 2023-02-18 09:46:26.190000 absplit-1.4.0/images/logo.jpeg
--rw-r--r--   0        0        0     1533 2023-07-01 22:51:52.089000 absplit-1.4.0/pyproject.toml
--rw-r--r--   0        0        0       50 2023-06-05 23:23:06.260000 absplit-1.4.0/requirements.txt
--rw-r--r--   0        0        0        0 2023-02-18 09:46:26.220000 absplit-1.4.0/tests/__init__.py
--rw-r--r--   0        0        0     5925 2023-02-18 09:46:26.238000 absplit-1.4.0/tests/test_data.py
--rw-r--r--   0        0        0     2125 2023-06-12 08:32:24.989000 absplit-1.4.0/tests/test_ga.py
--rw-r--r--   0        0        0     9285 1970-01-01 00:00:00.000000 absplit-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0     4958 2023-06-05 23:23:06.124000 absplit-1.4.1/.gitignore
+-rw-r--r--   0        0        0       50 2023-02-18 09:46:26.039000 absplit-1.4.1/.idea/.gitignore
+-rw-r--r--   0        0        0      291 2023-06-12 08:40:13.087000 absplit-1.4.1/.idea/genetic_algorithm.iml
+-rw-r--r--   0        0        0      179 2023-02-18 09:46:26.072000 absplit-1.4.1/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0      303 2023-06-12 08:40:13.168000 absplit-1.4.1/.idea/misc.xml
+-rw-r--r--   0        0        0      293 2023-02-18 09:46:26.093000 absplit-1.4.1/.idea/modules.xml
+-rw-r--r--   0        0        0      185 2023-02-18 09:46:26.104000 absplit-1.4.1/.idea/vcs.xml
+-rw-r--r--   0        0        0     1026 2023-02-18 09:46:26.114000 absplit-1.4.1/LICENSE
+-rw-r--r--   0        0        0      152 2023-02-18 09:46:26.124000 absplit-1.4.1/MANIFEST.in
+-rw-r--r--   0        0        0     8252 2023-07-02 10:26:33.912000 absplit-1.4.1/README.md
+-rw-r--r--   0        0        0       93 2023-07-02 10:26:33.957000 absplit-1.4.1/absplit/__init__.py
+-rw-r--r--   0        0        0     8992 2023-07-02 10:01:16.253000 absplit-1.4.1/absplit/data.py
+-rw-r--r--   0        0        0    30025 2023-07-02 10:24:16.883000 absplit-1.4.1/absplit/ga.py
+-rw-r--r--   0        0        0     1866 2023-02-18 09:46:26.177000 absplit-1.4.1/absplit/param.py
+-rw-r--r--   0        0        0     3978 2023-06-18 23:28:12.372000 absplit-1.4.1/absplit/tutorials.py
+-rw-r--r--   0        0        0    29186 2023-02-18 09:46:26.190000 absplit-1.4.1/images/logo.jpeg
+-rw-r--r--   0        0        0     1533 2023-07-02 10:26:33.999000 absplit-1.4.1/pyproject.toml
+-rw-r--r--   0        0        0       50 2023-06-05 23:23:06.260000 absplit-1.4.1/requirements.txt
+-rw-r--r--   0        0        0        0 2023-02-18 09:46:26.220000 absplit-1.4.1/tests/__init__.py
+-rw-r--r--   0        0        0     5925 2023-02-18 09:46:26.238000 absplit-1.4.1/tests/test_data.py
+-rw-r--r--   0        0        0     2125 2023-06-12 08:32:24.989000 absplit-1.4.1/tests/test_ga.py
+-rw-r--r--   0        0        0     9285 1970-01-01 00:00:00.000000 absplit-1.4.1/PKG-INFO
```

### Comparing `absplit-1.4.0/.gitignore` & `absplit-1.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `absplit-1.4.0/LICENSE` & `absplit-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `absplit-1.4.0/README.md` & `absplit-1.4.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 <div align="center">
 <img src="https://raw.githubusercontent.com/cormac-rynne/absplit/main/images/logo.jpeg" width="460" height="140">
 <h3><strong>ABSplit</strong></h3>
 Split your data into matching A/B/n groups
 
 ![license](https://img.shields.io/badge/License-MIT-blue.svg)
-![version](https://img.shields.io/badge/version-1.4.0-blue.svg)
+![version](https://img.shields.io/badge/version-1.4.1-blue.svg)
 ![version](https://img.shields.io/badge/python-3-orange.svg)
 
 </div>
 
 <details open>
   <summary>Table of Contents</summary>
   <ol>
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
 [https://raw.githubusercontent.com/cormac-rynne/absplit/main/images/logo.jpeg]
                                **** ABSplit ****
  Split your data into matching A/B/n groups ![license](https://img.shields.io/
  badge/License-MIT-blue.svg) ![version](https://img.shields.io/badge/version-
- 1.4.0-blue.svg) ![version](https://img.shields.io/badge/python-3-orange.svg)
+ 1.4.1-blue.svg) ![version](https://img.shields.io/badge/python-3-orange.svg)
  Table of Contents
    1. About_The_Project
    2. Getting_Started
           o Installation
    3. Tutorials
           o Do_it_yourself
    4. Usage
```

### Comparing `absplit-1.4.0/absplit/data.py` & `absplit-1.4.1/absplit/data.py`

 * *Files identical despite different names*

### Comparing `absplit-1.4.0/absplit/ga.py` & `absplit-1.4.1/absplit/ga.py`

 * *Files 0% similar despite different names*

```diff
@@ -233,15 +233,15 @@
 
         Returns:
             None
         """
 
         global all_metrics_global
         global splits_global
-        splits_global = (np.array(self._splits).sum() / np.array(self._splits)).reshape((1, -1, 1))
+        splits_global = (np.array(self._splits).sum() / np.array(self._splits))
 
         logger.debug('Splitting..')
         all_metrics_global = self._population.matrix
 
         # Run multiple times, save the best solution
         for i in range(self._runs):
             if self._runs > 1:
@@ -627,14 +627,15 @@
         self._population = Data(self._df_pop, scaler=scaler, **kwargs)
         self._sample = Data(self._df_samp, scaler=scaler, **kwargs)
 
         # Makes the match matrix available globally, sum along population axis
         global match_metrics_global
         global metric_weights_global
         match_metrics_global = self._sample.matrix.sum(1)
+        # Reshape to configure for 2d m
         metric_weights_global = metric_weights_global.reshape(1, -1)
 
         self._update_initial_population()
 
     def _update_initial_population(self):
         """Update initial population so frequency of '1's in starting population is sample_size/population_size
         to speed up convergence.
@@ -732,15 +733,15 @@
         3. The mean squared error (MSE) for each metric is calculated between groups
         4. Sum penalty is calculated based on the difference in sum of metrics over time costs between groups.
         5. The total cost is computed as the sum of the MSE, size penalty, and sum penalty.
         6. The fitness value is then computed as the inverse of the absolute total cost
            (plus a small number to prevent division by zero).
     """
 
-    global all_metrics_global     # 3d matrix of (metrics, population, dates)
+    global all_metrics_global     # 3d matrix of metric values (metrics, population, dates)
     global metric_weights_global  # Relative weights for each metric
     global splits_global          # Proportional splits for each group
     global size_penalty_global    # Float weight for size penalty
     global sum_penalty_global     # Float weight for sum penalty
     global group_ids_global       # Array of group IDs
 
     # Generate binary array, 1 row of 0s and 1s for each group (where solution == 1/2/3 etc)
@@ -751,15 +752,15 @@
     mean = np.mean(all_metrics_global) * all_metrics_global.shape[0] * all_metrics_global.shape[2]
     # Get size cost for each group
     mean_group = (groups * mean).sum(1) * splits_global
     # Calculate group differences, sum
     size_cost = (np.abs(np.roll(mean_group, -1) - mean_group).sum()) * size_penalty_global / (4*len(splits_global)) ** 1.2
 
     # == MSE == #
-    costs = (groups @ all_metrics_global) * splits_global * metric_weights_global
+    costs = (groups @ all_metrics_global) * splits_global.reshape((1, -1, 1)) * metric_weights_global
     diffs = np.roll(costs, -1, axis=1) - costs
     mse = ((diffs ** 2).mean(axis=1)).sum()
 
     # == Sum penalty == #
     sum_cost = (np.abs(costs.sum(2) - np.roll(costs.sum(2), shift=-1, axis=1)).sum() * sum_penalty_global) / (4*len(splits_global)) ** 1.2
 
     # Fitness
```

### Comparing `absplit-1.4.0/absplit/param.py` & `absplit-1.4.1/absplit/param.py`

 * *Files identical despite different names*

### Comparing `absplit-1.4.0/absplit/tutorials.py` & `absplit-1.4.1/absplit/tutorials.py`

 * *Files identical despite different names*

### Comparing `absplit-1.4.0/images/logo.jpeg` & `absplit-1.4.1/images/logo.jpeg`

 * *Files identical despite different names*

### Comparing `absplit-1.4.0/pyproject.toml` & `absplit-1.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "absplit"
-version = "1.4.0"
+version = "1.4.1"
 description = "Generates A/B/n test groups"
 readme = "README.md"
 authors = [{name = "Cormac Rynne", email = "cormac.ry@gmail.com"}]
 license = {file = "LICENSE"}
 repository = "https://github.com/cormac-rynne/absplit"
 requires-python = "<=3.11"
 classifiers = [
```

### Comparing `absplit-1.4.0/tests/test_data.py` & `absplit-1.4.1/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `absplit-1.4.0/tests/test_ga.py` & `absplit-1.4.1/tests/test_ga.py`

 * *Files identical despite different names*

### Comparing `absplit-1.4.0/PKG-INFO` & `absplit-1.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: absplit
-Version: 1.4.0
+Version: 1.4.1
 Summary: Generates A/B/n test groups
 Keywords: absplit,a/b test,ab test,ab split,split,set formation,group formation
 Author-email: Cormac Rynne <cormac.ry@gmail.com>
 Requires-Python: <=3.11
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -31,15 +31,15 @@
 
 <div align="center">
 <img src="https://raw.githubusercontent.com/cormac-rynne/absplit/main/images/logo.jpeg" width="460" height="140">
 <h3><strong>ABSplit</strong></h3>
 Split your data into matching A/B/n groups
 
 ![license](https://img.shields.io/badge/License-MIT-blue.svg)
-![version](https://img.shields.io/badge/version-1.4.0-blue.svg)
+![version](https://img.shields.io/badge/version-1.4.1-blue.svg)
 ![version](https://img.shields.io/badge/python-3-orange.svg)
 
 </div>
 
 <details open>
   <summary>Table of Contents</summary>
   <ol>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: absplit Version: 1.4.0 Summary: Generates A/B/
+Metadata-Version: 2.1 Name: absplit Version: 1.4.1 Summary: Generates A/B/
 n test groups Keywords: absplit,a/b test,ab test,ab split,split,set
 formation,group formation Author-email: Cormac Rynne
 ry@gmail.com> Requires-Python: <=3.11 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
@@ -15,15 +15,15 @@
 Libraries :: Python Modules Requires-Dist: pygad==3.0.1 Requires-Dist: scikit-
 learn Requires-Dist: numpy Requires-Dist: pandas Requires-Dist: seaborn
 Project-URL: Home, https://github.com/cormac-rynne/absplit
 [https://raw.githubusercontent.com/cormac-rynne/absplit/main/images/logo.jpeg]
                                **** ABSplit ****
  Split your data into matching A/B/n groups ![license](https://img.shields.io/
  badge/License-MIT-blue.svg) ![version](https://img.shields.io/badge/version-
- 1.4.0-blue.svg) ![version](https://img.shields.io/badge/python-3-orange.svg)
+ 1.4.1-blue.svg) ![version](https://img.shields.io/badge/python-3-orange.svg)
  Table of Contents
    1. About_The_Project
    2. Getting_Started
           o Installation
    3. Tutorials
           o Do_it_yourself
    4. Usage
```

