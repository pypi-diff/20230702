# Comparing `tmp/prepup-0.1.5.tar.gz` & `tmp/prepup-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prepup-0.1.5.tar", last modified: Wed Jun  7 14:17:18 2023, max compression
+gzip compressed data, was "prepup-0.1.6.tar", last modified: Sun Jul  2 19:09:34 2023, max compression
```

## Comparing `prepup-0.1.5.tar` & `prepup-0.1.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-07 14:17:18.557392 prepup-0.1.5/
--rw-rw-rw-   0        0        0      188 2023-04-29 20:41:27.000000 prepup-0.1.5/AUTHORS.rst
--rw-rw-rw-   0        0        0     1100 2023-04-29 20:41:27.000000 prepup-0.1.5/LICENSE
--rw-rw-rw-   0        0        0      129 2023-04-29 20:41:27.000000 prepup-0.1.5/MANIFEST.in
--rw-rw-rw-   0        0        0     4255 2023-06-07 14:17:18.550575 prepup-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     3719 2023-05-17 04:35:37.000000 prepup-0.1.5/README.md
-drwxrwxrwx   0        0        0        0 2023-06-07 14:17:18.542084 prepup-0.1.5/prepup/
--rw-rw-rw-   0        0        0     7971 2023-06-07 14:16:53.000000 prepup-0.1.5/prepup/__init__.py
--rw-rw-rw-   0        0        0    33833 2023-05-17 04:34:27.000000 prepup-0.1.5/prepup/common.py
-drwxrwxrwx   0        0        0        0 2023-06-07 14:17:18.550575 prepup-0.1.5/prepup.egg-info/
--rw-rw-rw-   0        0        0     4255 2023-06-07 14:17:18.000000 prepup-0.1.5/prepup.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      285 2023-06-07 14:17:18.000000 prepup-0.1.5/prepup.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-07 14:17:18.000000 prepup-0.1.5/prepup.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-06-07 14:17:18.000000 prepup-0.1.5/prepup.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      220 2023-06-07 14:17:18.000000 prepup-0.1.5/prepup.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-07 14:17:18.000000 prepup-0.1.5/prepup.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      367 2023-05-17 04:35:39.000000 prepup-0.1.5/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-06-07 14:17:18.558377 prepup-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0     1488 2023-06-07 14:16:13.000000 prepup-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-02 19:09:34.970122 prepup-0.1.6/
+-rw-rw-rw-   0        0        0      188 2023-04-29 20:41:27.000000 prepup-0.1.6/AUTHORS.rst
+-rw-rw-rw-   0        0        0     1100 2023-04-29 20:41:27.000000 prepup-0.1.6/LICENSE
+-rw-rw-rw-   0        0        0      129 2023-04-29 20:41:27.000000 prepup-0.1.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     4798 2023-07-02 19:09:34.961279 prepup-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     4260 2023-07-02 19:08:54.000000 prepup-0.1.6/README.md
+drwxrwxrwx   0        0        0        0 2023-07-02 19:09:34.952934 prepup-0.1.6/prepup/
+-rw-rw-rw-   0        0        0     7998 2023-07-02 17:52:13.000000 prepup-0.1.6/prepup/__init__.py
+-rw-rw-rw-   0        0        0    33833 2023-05-17 04:34:27.000000 prepup-0.1.6/prepup/common.py
+drwxrwxrwx   0        0        0        0 2023-07-02 19:09:34.961279 prepup-0.1.6/prepup.egg-info/
+-rw-rw-rw-   0        0        0     4798 2023-07-02 19:09:34.000000 prepup-0.1.6/prepup.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      285 2023-07-02 19:09:34.000000 prepup-0.1.6/prepup.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-02 19:09:34.000000 prepup-0.1.6/prepup.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-07-02 19:09:34.000000 prepup-0.1.6/prepup.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      220 2023-07-02 19:09:34.000000 prepup-0.1.6/prepup.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-02 19:09:34.000000 prepup-0.1.6/prepup.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      367 2023-05-17 04:35:39.000000 prepup-0.1.6/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-02 19:09:34.970122 prepup-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0     1488 2023-07-02 17:32:14.000000 prepup-0.1.6/setup.py
```

### Comparing `prepup-0.1.5/LICENSE` & `prepup-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `prepup-0.1.5/PKG-INFO` & `prepup-0.1.6/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prepup
-Version: 0.1.5
+Version: 0.1.6
 Summary: Prepup is a free, open-source package that lets you open, explore, visualize, and pre-process datasets in your Computer's Terminal.
 Author: Sudhanshu Mukherjee
 Author-email: sudhanshumukherjeexx@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.5
@@ -50,56 +50,66 @@
 -   Prepup doesn't alters your raw data, It saves pre-processed data only when user specifies the path.
 
 ### Lives in your Terminal
 -   Prepup is terminal based and has specific entry points designed for using it instantly.
 
 # Command Line Arguments available in PREPUP
 
-## prepup <File name or File path> -inspect
+## prepup "File name or File path" -inspect
+<video width="320" height="240" controls>
+  <source src="C:\Users\Asus\prepup\datasets\gif\inspect.mp4" type="video/mp4">
+</video>
 
 -   inspect flag takes the dataframe and returns the Features available, Features datatype and missing values present in the Dataset.
 
-## prepup <File name or File path> -explore
+## prepup "File name or File path" -explore
+<video width="320" height="240" controls>
+  <source src="C:\Users\Asus\prepup\datasets\gif\explore.mp4" type="video/mp4">
+</video>
 
 -   explore flag takes the dataframe and returns the Features available, Features datatype, Correlation between features, Detects Outliers, Checks Normal Distribution, Checks Skewness, Checks Kurtosis and also allows the option to check if the dataset is Imbalanced.
 
-## prepup <File name or File path> -explore
+## prepup "File name or File path" -visualize
+<video width="320" height="240" controls>
+  <source src="C:\Users\Asus\prepup\datasets\gif\visualize.mp4" type="video/mp4">
+</video>
 
 -   visualize flag plots the feature distribution directly on the terminal.
 
-## prepup <File name or File path> -visualize
+## prepup "File name or File path" -impute
+<video width="320" height="240" controls>
+  <source src="C:\Users\Asus\prepup\datasets\gif\impute.mp4" type="video/mp4">
+</video>
 
--   visualize flag plots the feature distribution directly on the terminal.
-
-## prepup <File name or File path> -impute
 - There are 8 different strategies available to impute missing data using Prepup
 
     - Option 1 - Drops the Missing Data
     - Option 2 - Impute Missing values with a Specific value
     - Option 3 - Impute Missing values with Mean.
     - Option 4 - Impute Missing values with Median.
     - Option 5 - Impute Missing value based on the distribution of existing columns.
     - Option 6 - Impute Missing values based on Forward Fill Strategy where missing values are imputed based on the previous data points.
     - Option 7 - Impute Missing values based on Backward Strategy where missing values are imputed based on the next data points.
     - Option 8 - Impute missing values based on K-Nearest Neighbors.
 
-## prepup <File name or File path> -standardize
+## prepup "File name or File path" -standardize
+<video width="320" height="240" controls>
+  <source src="C:\Users\Asus\prepup\datasets\gif\standardize.mp4" type="video/mp4">
+</video>
 
 -   Standardize allows you to standardize the dataset using two different methods:
     1. Robust Scaler
 
     2. Standard Scaler 
 
 -   Robust Scaler is recommended if there are outliers present and you feel they can have influence on the Machine Learning model.
 
 -   Standard Scaler is go to function if you want to standardize the dataset before training the model on it.
 
-
 # License
 
 -   Free software: MIT license
 
 # Package Link
 -   Github: https://github.com/sudhanshumukherjeexx/prepup
 
 -   Documentation: https://sudhanshumukherjeexx.github.io/prepup
-
```

### Comparing `prepup-0.1.5/prepup/__init__.py` & `prepup-0.1.6/prepup/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     parser = argparse.ArgumentParser(description="Prepup is a free open-source package that lets you inspect, explore, visualize, and perform pre-processing tasks on datasets in your computers terminal.")
     parser.add_argument('file',type=str, help='Dataset file')
     parser.add_argument('-inspect', action='store_true', help='Observe the dataset and its Features.')
     parser.add_argument('-explore', action='store_true', help='Explore Dataset.')
     parser.add_argument('-visualize', action='store_true', help='Visualize Feature Distribution.')
     parser.add_argument('-impute', action='store_true', help='Impute Missing values.')
     parser.add_argument('-standardize', action='store_true', help='Standardize Feature Columns.')
-    parser.add_argument('-rii', action='store_true', help='Convert code to Python Notebook.')
+    parser.add_argument('-rii', action='store_true', help='Convert code to Python Notebook. (#Still Under Development)')
     return parser.parse_args()
 
 def load_file(file_path):
     # Check file extension
     if file_path.endswith('.csv'):
         return pl.read_csv(file_path, ignore_errors=True)
     elif file_path.endswith('.xlsx'):
```

### Comparing `prepup-0.1.5/prepup/common.py` & `prepup-0.1.6/prepup/common.py`

 * *Files identical despite different names*

### Comparing `prepup-0.1.5/prepup.egg-info/PKG-INFO` & `prepup-0.1.6/prepup.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prepup
-Version: 0.1.5
+Version: 0.1.6
 Summary: Prepup is a free, open-source package that lets you open, explore, visualize, and pre-process datasets in your Computer's Terminal.
 Author: Sudhanshu Mukherjee
 Author-email: sudhanshumukherjeexx@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.5
@@ -50,56 +50,66 @@
 -   Prepup doesn't alters your raw data, It saves pre-processed data only when user specifies the path.
 
 ### Lives in your Terminal
 -   Prepup is terminal based and has specific entry points designed for using it instantly.
 
 # Command Line Arguments available in PREPUP
 
-## prepup <File name or File path> -inspect
+## prepup "File name or File path" -inspect
+<video width="320" height="240" controls>
+  <source src="C:\Users\Asus\prepup\datasets\gif\inspect.mp4" type="video/mp4">
+</video>
 
 -   inspect flag takes the dataframe and returns the Features available, Features datatype and missing values present in the Dataset.
 
-## prepup <File name or File path> -explore
+## prepup "File name or File path" -explore
+<video width="320" height="240" controls>
+  <source src="C:\Users\Asus\prepup\datasets\gif\explore.mp4" type="video/mp4">
+</video>
 
 -   explore flag takes the dataframe and returns the Features available, Features datatype, Correlation between features, Detects Outliers, Checks Normal Distribution, Checks Skewness, Checks Kurtosis and also allows the option to check if the dataset is Imbalanced.
 
-## prepup <File name or File path> -explore
+## prepup "File name or File path" -visualize
+<video width="320" height="240" controls>
+  <source src="C:\Users\Asus\prepup\datasets\gif\visualize.mp4" type="video/mp4">
+</video>
 
 -   visualize flag plots the feature distribution directly on the terminal.
 
-## prepup <File name or File path> -visualize
+## prepup "File name or File path" -impute
+<video width="320" height="240" controls>
+  <source src="C:\Users\Asus\prepup\datasets\gif\impute.mp4" type="video/mp4">
+</video>
 
--   visualize flag plots the feature distribution directly on the terminal.
-
-## prepup <File name or File path> -impute
 - There are 8 different strategies available to impute missing data using Prepup
 
     - Option 1 - Drops the Missing Data
     - Option 2 - Impute Missing values with a Specific value
     - Option 3 - Impute Missing values with Mean.
     - Option 4 - Impute Missing values with Median.
     - Option 5 - Impute Missing value based on the distribution of existing columns.
     - Option 6 - Impute Missing values based on Forward Fill Strategy where missing values are imputed based on the previous data points.
     - Option 7 - Impute Missing values based on Backward Strategy where missing values are imputed based on the next data points.
     - Option 8 - Impute missing values based on K-Nearest Neighbors.
 
-## prepup <File name or File path> -standardize
+## prepup "File name or File path" -standardize
+<video width="320" height="240" controls>
+  <source src="C:\Users\Asus\prepup\datasets\gif\standardize.mp4" type="video/mp4">
+</video>
 
 -   Standardize allows you to standardize the dataset using two different methods:
     1. Robust Scaler
 
     2. Standard Scaler 
 
 -   Robust Scaler is recommended if there are outliers present and you feel they can have influence on the Machine Learning model.
 
 -   Standard Scaler is go to function if you want to standardize the dataset before training the model on it.
 
-
 # License
 
 -   Free software: MIT license
 
 # Package Link
 -   Github: https://github.com/sudhanshumukherjeexx/prepup
 
 -   Documentation: https://sudhanshumukherjeexx.github.io/prepup
-
```

### Comparing `prepup-0.1.5/setup.py` & `prepup-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 
 setuptools.setup(
     name="prepup",
-    version="0.1.5",
+    version="0.1.6",
     author="Sudhanshu Mukherjee",
     author_email="sudhanshumukherjeexx@gmail.com",
     description="Prepup is a free, open-source package that lets you open, explore, visualize, and pre-process datasets in your Computer's Terminal.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=setuptools.find_packages(),
     entry_points={
```

