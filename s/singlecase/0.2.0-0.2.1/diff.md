# Comparing `tmp/singlecase-0.2.0.tar.gz` & `tmp/singlecase-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "singlecase-0.2.0.tar", last modified: Sun Jul  2 07:43:58 2023, max compression
+gzip compressed data, was "singlecase-0.2.1.tar", last modified: Sun Jul  2 14:06:07 2023, max compression
```

## Comparing `singlecase-0.2.0.tar` & `singlecase-0.2.1.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxrwxr-x   0 cw        (1000) cw        (1000)        0 2023-07-02 07:43:58.263678 singlecase-0.2.0/
--rw-rw-r--   0 cw        (1000) cw        (1000)     1502 2023-07-01 11:26:29.000000 singlecase-0.2.0/LICENSE
--rw-rw-r--   0 cw        (1000) cw        (1000)     6422 2023-07-02 07:43:58.263678 singlecase-0.2.0/PKG-INFO
--rw-rw-r--   0 cw        (1000) cw        (1000)     3582 2023-07-02 07:43:40.000000 singlecase-0.2.0/README.md
--rw-rw-r--   0 cw        (1000) cw        (1000)     1391 2023-07-02 07:31:39.000000 singlecase-0.2.0/pyproject.toml
--rw-rw-r--   0 cw        (1000) cw        (1000)       38 2023-07-02 07:43:58.263678 singlecase-0.2.0/setup.cfg
--rw-rw-r--   0 cw        (1000) cw        (1000)       37 2023-07-01 11:26:29.000000 singlecase-0.2.0/setup.py
-drwxrwxr-x   0 cw        (1000) cw        (1000)        0 2023-07-02 07:43:58.263678 singlecase-0.2.0/singlecase/
--rw-rw-r--   0 cw        (1000) cw        (1000)      144 2023-07-02 06:56:34.000000 singlecase-0.2.0/singlecase/__init__.py
-drwxrwxr-x   0 cw        (1000) cw        (1000)        0 2023-07-02 07:43:58.263678 singlecase-0.2.0/singlecase/data/
--rw-rw-r--   0 cw        (1000) cw        (1000)     2342 2023-07-02 07:07:38.000000 singlecase-0.2.0/singlecase/data/__init__.py
-drwxrwxr-x   0 cw        (1000) cw        (1000)        0 2023-07-02 07:43:58.263678 singlecase-0.2.0/singlecase/effectsize/
--rw-rw-r--   0 cw        (1000) cw        (1000)     2748 2023-07-02 06:56:48.000000 singlecase-0.2.0/singlecase/effectsize/__init__.py
-drwxrwxr-x   0 cw        (1000) cw        (1000)        0 2023-07-02 07:43:58.263678 singlecase-0.2.0/singlecase/permtest/
--rw-rw-r--   0 cw        (1000) cw        (1000)     2414 2023-07-02 06:57:09.000000 singlecase-0.2.0/singlecase/permtest/__init__.py
-drwxrwxr-x   0 cw        (1000) cw        (1000)        0 2023-07-02 07:43:58.263678 singlecase-0.2.0/singlecase.egg-info/
--rw-rw-r--   0 cw        (1000) cw        (1000)     6422 2023-07-02 07:43:58.000000 singlecase-0.2.0/singlecase.egg-info/PKG-INFO
--rw-rw-r--   0 cw        (1000) cw        (1000)      327 2023-07-02 07:43:58.000000 singlecase-0.2.0/singlecase.egg-info/SOURCES.txt
--rw-rw-r--   0 cw        (1000) cw        (1000)        1 2023-07-02 07:43:58.000000 singlecase-0.2.0/singlecase.egg-info/dependency_links.txt
--rw-rw-r--   0 cw        (1000) cw        (1000)       49 2023-07-02 07:43:58.000000 singlecase-0.2.0/singlecase.egg-info/requires.txt
--rw-rw-r--   0 cw        (1000) cw        (1000)       11 2023-07-02 07:43:58.000000 singlecase-0.2.0/singlecase.egg-info/top_level.txt
+drwxrwxr-x   0 cw        (1000) cw        (1000)        0 2023-07-02 14:06:07.017803 singlecase-0.2.1/
+-rw-rw-r--   0 cw        (1000) cw        (1000)     1502 2023-07-01 11:26:29.000000 singlecase-0.2.1/LICENSE
+-rw-rw-r--   0 cw        (1000) cw        (1000)     7321 2023-07-02 14:06:07.017803 singlecase-0.2.1/PKG-INFO
+-rw-rw-r--   0 cw        (1000) cw        (1000)     4481 2023-07-02 14:04:51.000000 singlecase-0.2.1/README.md
+-rw-rw-r--   0 cw        (1000) cw        (1000)     1391 2023-07-02 13:45:50.000000 singlecase-0.2.1/pyproject.toml
+-rw-rw-r--   0 cw        (1000) cw        (1000)       38 2023-07-02 14:06:07.017803 singlecase-0.2.1/setup.cfg
+-rw-rw-r--   0 cw        (1000) cw        (1000)       37 2023-07-01 11:26:29.000000 singlecase-0.2.1/setup.py
+drwxrwxr-x   0 cw        (1000) cw        (1000)        0 2023-07-02 14:06:07.017803 singlecase-0.2.1/singlecase/
+-rw-rw-r--   0 cw        (1000) cw        (1000)      144 2023-07-02 06:56:34.000000 singlecase-0.2.1/singlecase/__init__.py
+drwxrwxr-x   0 cw        (1000) cw        (1000)        0 2023-07-02 14:06:07.017803 singlecase-0.2.1/singlecase/data/
+-rw-rw-r--   0 cw        (1000) cw        (1000)     3810 2023-07-02 13:05:59.000000 singlecase-0.2.1/singlecase/data/__init__.py
+drwxrwxr-x   0 cw        (1000) cw        (1000)        0 2023-07-02 14:06:07.017803 singlecase-0.2.1/singlecase/effectsize/
+-rw-rw-r--   0 cw        (1000) cw        (1000)     3656 2023-07-02 13:42:18.000000 singlecase-0.2.1/singlecase/effectsize/__init__.py
+drwxrwxr-x   0 cw        (1000) cw        (1000)        0 2023-07-02 14:06:07.017803 singlecase-0.2.1/singlecase/permtest/
+-rw-rw-r--   0 cw        (1000) cw        (1000)     2884 2023-07-02 13:09:04.000000 singlecase-0.2.1/singlecase/permtest/__init__.py
+drwxrwxr-x   0 cw        (1000) cw        (1000)        0 2023-07-02 14:06:07.017803 singlecase-0.2.1/singlecase/table/
+-rw-rw-r--   0 cw        (1000) cw        (1000)      200 2023-07-02 12:56:44.000000 singlecase-0.2.1/singlecase/table/__init__.py
+drwxrwxr-x   0 cw        (1000) cw        (1000)        0 2023-07-02 14:06:07.017803 singlecase-0.2.1/singlecase.egg-info/
+-rw-rw-r--   0 cw        (1000) cw        (1000)     7321 2023-07-02 14:06:07.000000 singlecase-0.2.1/singlecase.egg-info/PKG-INFO
+-rw-rw-r--   0 cw        (1000) cw        (1000)      356 2023-07-02 14:06:07.000000 singlecase-0.2.1/singlecase.egg-info/SOURCES.txt
+-rw-rw-r--   0 cw        (1000) cw        (1000)        1 2023-07-02 14:06:07.000000 singlecase-0.2.1/singlecase.egg-info/dependency_links.txt
+-rw-rw-r--   0 cw        (1000) cw        (1000)       49 2023-07-02 14:06:07.000000 singlecase-0.2.1/singlecase.egg-info/requires.txt
+-rw-rw-r--   0 cw        (1000) cw        (1000)       11 2023-07-02 14:06:07.000000 singlecase-0.2.1/singlecase.egg-info/top_level.txt
```

### Comparing `singlecase-0.2.0/LICENSE` & `singlecase-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `singlecase-0.2.0/PKG-INFO` & `singlecase-0.2.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: singlecase
-Version: 0.2.0
+Version: 0.2.1
 Summary: A tool for single-case design data managment, statistical analysis and visualization.
 Author-email: Casper Wilstrup <casper.wilstrup@abzu.ai>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, Casper Wilstrup
         
         Redistribution and use in source and binary forms, with or without
@@ -73,93 +73,98 @@
 ```python
 from singlecase.data import Data
 ```
 
 Then, create a `Data` object with either a pandas DataFrame or a dictionary:
 
 ```python
-df = pd.DataFrame({...})  # Or load your data from a CSV, database, etc.
-data = Data(df)
+data = Data({
+    'phase': ['A1', 'A1', 'A1', 'B', 'B', 'B', 'A2', 'A2', 'A2'],
+    'dvar1': [1.0, 2.5, 3.2, 4.2, 5.5, 6.2, 2.0, 2.4, 3.1],
+    'dvar2': [2.5, 3.2, 4.6, 5.6, 6.2, 7.8, 3.3, 4.1, 4.8],
+})
 ```
 
-Now you're ready to perform single-case data analysis!
+Now you're ready to perform single-case data analysis.
 
 ## Core Features
 
 ### Data Class
 
 The `Data` class provides an object-oriented interface to represent your single-case data. It assumes any variable with datatype of float as a dependent variable. The dependent and phase variables can be accessed and modified using properties. For example:
 
 ```python
-data.pvar = 'column_name'  # Set the phase variable
+data.pvar = 'column_name'  # Set the phase variable, if it is not named 'phase'
 ```
 
 ### Nonoverlap Pairs (NAP)
 
 The `nap` function computes the Nonoverlap Pairs between two phases in a single-case data frame. It returns a pandas Series containing the NAP values for each dependent variable in the data set.
 
 ```python
 from singlecase.effectsize import nap
-nap_values = nap(data)
+nap_values = nap(data, phases["A1", "B"])
 ```
 
 ### Percent Non-overlapping Data (PND)
 
 The `pnd` function computes the Percent Non-overlapping Data between two phases in a single-case data frame. It returns a pandas Series containing the PND values for each dependent variable in the data set.
 
 ```python
 from singlecase.effectsize import pnd
-pnd_values = pnd(data)
+pnd_values = pnd(data, phases=["A1", "B"])
 ```
 
 ### Permutation Test
 
-The `permutation_test` function performs a permutation test between two phases in a single-case data frame. It returns a pandas Series containing the p-values for each dependent variable in the data set.
+The `permutation_test` function performs a permutation test between two phases in a single-case data frame. It returns a pandas Series containing the p-values for each dependent variable in the data set. The p-value is the probability that the two phases have the same mean.
 
 ```python
 from singlecase.permtest import permutation_test
-p_values = permutation_test(data)
+p_values = permutation_test(data, phases=["A1","A2"])
 ```
 
 
 ## Complete example
 
-This complete example creates a new `singlecase.Data` from a Python dictionary. The dataset has two dependent variables `dvar1` and `dvar2`. The phase variable is called `phase` and consists of the two phases "A" and "B". Based on this data, the PND and NAP values are calculated and printed.
+This complete example creates a new `singlecase.Data` from a Python dictionary. The dataset has two dependent variables `dvar1` and `dvar2`. The phase variable is called `phase` and consists of the two phases "A" and "B". Based on this data, the PND and NAP values are calculated and printed. The probability that the two phases have the same mean is then calculated using permutation tests and printed. Since the data contains only two phases, it is not necessary to specify which phases to compare in `pnd`, `nap` and `permutation_test` function calls.
 
 ```python
 import pandas as pd
 from singlecase.data import Data
 from singlecase.effectsize import pnd, nap
+from singlecase.permtest import permutation_test
 
 # Create a sample data
 data_dict = {
+    'phase': ['A', 'A', 'A', 'A', 'A', 'A', 'B', 'B', 'B', 'B', 'B', 'B'],
     'dvar1': [1.0, 2.5, 3.2, 4.6, 2.8, 5.6, 3.7, 4.2, 5.5, 6.2, 7.3, 8.5],
     'dvar2': [2.5, 3.2, 4.6, 5.1, 4.8, 5.2, 6.7, 5.6, 6.2, 7.8, 8.4, 7.2],
-    'phase': ['A', 'A', 'A', 'A', 'A', 'A', 'B', 'B', 'B', 'B', 'B', 'B']
 }
 
-df = pd.DataFrame(data_dict)
-
 # Instantiate Data object
-data = Data(df)
-
-# Set phase variable
-data.pvar = 'phase'
+data = Data(data_dict)
 
 # Calculate PND
 pnd_values = pnd(data)
-print(f"PND values: \n{pnd_values}")
+print(f"PND values:\n{pnd_values}\n")
 
 # Calculate NAP
 nap_values = nap(data)
-print(f"NAP values: \n{nap_values}")
+print(f"NAP values:\n{nap_values}\n")
+
+# Calculate the p-value the mean of the two phases being the same
+perm_p = permutation_test(data)
+print(f"Probability that A and B phases have same mean:\n{perm_p}\n")
 ```
 
 
 ## License
 
-This project is licensed under the BSD 3-clause license - see the [LICENSE](LICENSE) file for details.
+This project is licensed under the BSD 3-clause license - see the LICENSE file for details.
+
+## About the package
 
-## Acknowledgments
+The Single Case Research package is supported by [Abzu](https://www.abzu.ai) as part of an ongoing mission to improve scientific research powered by artificial intelligence.
 
-- The Single Case Research package is being developed by Casper Wilstrup.
+The primary author of the package is [Casper Wilstrup](https://twitter.com/cwilstrup). New contributors are welcome.
```

### Comparing `singlecase-0.2.0/README.md` & `singlecase-0.2.1/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -20,93 +20,98 @@
 ```python
 from singlecase.data import Data
 ```
 
 Then, create a `Data` object with either a pandas DataFrame or a dictionary:
 
 ```python
-df = pd.DataFrame({...})  # Or load your data from a CSV, database, etc.
-data = Data(df)
+data = Data({
+    'phase': ['A1', 'A1', 'A1', 'B', 'B', 'B', 'A2', 'A2', 'A2'],
+    'dvar1': [1.0, 2.5, 3.2, 4.2, 5.5, 6.2, 2.0, 2.4, 3.1],
+    'dvar2': [2.5, 3.2, 4.6, 5.6, 6.2, 7.8, 3.3, 4.1, 4.8],
+})
 ```
 
-Now you're ready to perform single-case data analysis!
+Now you're ready to perform single-case data analysis.
 
 ## Core Features
 
 ### Data Class
 
 The `Data` class provides an object-oriented interface to represent your single-case data. It assumes any variable with datatype of float as a dependent variable. The dependent and phase variables can be accessed and modified using properties. For example:
 
 ```python
-data.pvar = 'column_name'  # Set the phase variable
+data.pvar = 'column_name'  # Set the phase variable, if it is not named 'phase'
 ```
 
 ### Nonoverlap Pairs (NAP)
 
 The `nap` function computes the Nonoverlap Pairs between two phases in a single-case data frame. It returns a pandas Series containing the NAP values for each dependent variable in the data set.
 
 ```python
 from singlecase.effectsize import nap
-nap_values = nap(data)
+nap_values = nap(data, phases["A1", "B"])
 ```
 
 ### Percent Non-overlapping Data (PND)
 
 The `pnd` function computes the Percent Non-overlapping Data between two phases in a single-case data frame. It returns a pandas Series containing the PND values for each dependent variable in the data set.
 
 ```python
 from singlecase.effectsize import pnd
-pnd_values = pnd(data)
+pnd_values = pnd(data, phases=["A1", "B"])
 ```
 
 ### Permutation Test
 
-The `permutation_test` function performs a permutation test between two phases in a single-case data frame. It returns a pandas Series containing the p-values for each dependent variable in the data set.
+The `permutation_test` function performs a permutation test between two phases in a single-case data frame. It returns a pandas Series containing the p-values for each dependent variable in the data set. The p-value is the probability that the two phases have the same mean.
 
 ```python
 from singlecase.permtest import permutation_test
-p_values = permutation_test(data)
+p_values = permutation_test(data, phases=["A1","A2"])
 ```
 
 
 ## Complete example
 
-This complete example creates a new `singlecase.Data` from a Python dictionary. The dataset has two dependent variables `dvar1` and `dvar2`. The phase variable is called `phase` and consists of the two phases "A" and "B". Based on this data, the PND and NAP values are calculated and printed.
+This complete example creates a new `singlecase.Data` from a Python dictionary. The dataset has two dependent variables `dvar1` and `dvar2`. The phase variable is called `phase` and consists of the two phases "A" and "B". Based on this data, the PND and NAP values are calculated and printed. The probability that the two phases have the same mean is then calculated using permutation tests and printed. Since the data contains only two phases, it is not necessary to specify which phases to compare in `pnd`, `nap` and `permutation_test` function calls.
 
 ```python
 import pandas as pd
 from singlecase.data import Data
 from singlecase.effectsize import pnd, nap
+from singlecase.permtest import permutation_test
 
 # Create a sample data
 data_dict = {
+    'phase': ['A', 'A', 'A', 'A', 'A', 'A', 'B', 'B', 'B', 'B', 'B', 'B'],
     'dvar1': [1.0, 2.5, 3.2, 4.6, 2.8, 5.6, 3.7, 4.2, 5.5, 6.2, 7.3, 8.5],
     'dvar2': [2.5, 3.2, 4.6, 5.1, 4.8, 5.2, 6.7, 5.6, 6.2, 7.8, 8.4, 7.2],
-    'phase': ['A', 'A', 'A', 'A', 'A', 'A', 'B', 'B', 'B', 'B', 'B', 'B']
 }
 
-df = pd.DataFrame(data_dict)
-
 # Instantiate Data object
-data = Data(df)
-
-# Set phase variable
-data.pvar = 'phase'
+data = Data(data_dict)
 
 # Calculate PND
 pnd_values = pnd(data)
-print(f"PND values: \n{pnd_values}")
+print(f"PND values:\n{pnd_values}\n")
 
 # Calculate NAP
 nap_values = nap(data)
-print(f"NAP values: \n{nap_values}")
+print(f"NAP values:\n{nap_values}\n")
+
+# Calculate the p-value the mean of the two phases being the same
+perm_p = permutation_test(data)
+print(f"Probability that A and B phases have same mean:\n{perm_p}\n")
 ```
 
 
 ## License
 
-This project is licensed under the BSD 3-clause license - see the [LICENSE](LICENSE) file for details.
+This project is licensed under the BSD 3-clause license - see the LICENSE file for details.
+
+## About the package
 
-## Acknowledgments
+The Single Case Research package is supported by [Abzu](https://www.abzu.ai) as part of an ongoing mission to improve scientific research powered by artificial intelligence.
 
-- The Single Case Research package is being developed by Casper Wilstrup.
+The primary author of the package is [Casper Wilstrup](https://twitter.com/cwilstrup). New contributors are welcome.
```

### Comparing `singlecase-0.2.0/pyproject.toml` & `singlecase-0.2.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 
 [tool.setuptools.packages.find]
 include = ["singlecase", "singlecase.*"]
 
 [project]
 name = "singlecase"
-version = "0.2.0"
+version = "0.2.1"
 description = "A tool for single-case design data managment, statistical analysis and visualization."
 readme = "README.md"
 authors = [{ name = "Casper Wilstrup", email = "casper.wilstrup@abzu.ai" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: BSD License",
     "Programming Language :: Python",
```

### Comparing `singlecase-0.2.0/singlecase/data/__init__.py` & `singlecase-0.2.1/singlecase/data/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Union, Dict
+from typing import Union, Dict, List
 import pandas as pd
 
 
 class Data:
     """
     A class used to represent single-case data in a structured format.
 
@@ -12,32 +12,47 @@
     in the data.
 
     Any variable with datatype of float is assumed to be a dependent variable. The 
 
     Args:
         data (Union[pd.DataFrame, Dict]): The data set. Must be either a pandas DataFrame 
         or a dictionary.
+        pvar (str, optional): The name of the phase variable column in the data set. If the
+        data contains a column named "phase", this will be used as the phase variable by default.
+        index (str, optional): The name of the variable in the dataset to use as the index, i.e.
+        the labels of each test session. If not provided, the sessions will be numbered starting at 0.
     
     Raises:
         ValueError: If the provided data is not a pandas DataFrame or a dictionary.
     """
 
-    def __init__(self, data: Union[pd.DataFrame, Dict]):
+    def __init__(self, data: Union[pd.DataFrame, Dict], pvar: str=None, index: str = None):
         """
         Constructs and initializes the Data object.
         """
 
         if isinstance(data, dict):
             self._df = pd.DataFrame(data)
         elif isinstance(data, pd.DataFrame):
             self._df = data.copy()
         else:
             raise ValueError("data must be a pd.DataFrame or a dict")
 
-        self._pvar = None
+
+        if index is not None:
+            self._df.set_index(index, inplace=True)
+
+        if pvar is None:
+            if "phase" in self._df.columns:
+                pvar = "phase"
+        else:
+            if pvar not in self._df.columns:
+                raise ValueError("pvar must be the name of a column in the data frame")
+
+        self._pvar = pvar
 
         # float columns are assumend to be dependent variables
         self._dvars = [col for col in self._df.columns if self._df[col].dtype == float]
 
     @property
     def pvar(self):
         """
@@ -60,18 +75,41 @@
             ValueError: If the provided pvar is not a column name in the DataFrame.
         """
         if pvar not in self._df.columns:
             raise ValueError("pvar must be the name of a column in the data frame")
         self._pvar = pvar
 
     @property
+    def phases(self) -> List[str]:
+        """
+        Property that gets the phases in the data set.
+
+        Returns:
+            List[str]: The names of the phases in the data set.
+        """
+        return list(self._df[self.pvar].unique())
+
+    @property
     def dvars(self):
         """
         Property that gets the names of the dependent variable columns.
 
         These are identified as any columns in the DataFrame with float datatype.
 
         Returns:
             List[str]: The names of the dependent variable columns.
         """
         return self._dvars
 
+
+    def phase_data(self, phase: str, dvar: str) -> pd.DataFrame:
+        """
+        Get the data for a specific phase and dependent variable.
+
+        Args:
+            phase (str): The name of the phase.
+            dvar (str): The name of the dependent variable.
+
+        Returns:
+            pd.DataFrame: The data for the specified phase and dependent variable.
+        """
+        return self._df.loc[self._df[self.pvar] == phase, dvar]
```

### Comparing `singlecase-0.2.0/singlecase/effectsize/__init__.py` & `singlecase-0.2.1/singlecase/effectsize/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,37 +1,45 @@
 import pandas as pd
+from typing import List
 
 from singlecase.data import Data
 
-def nap(data: Data, decreasing: bool = False) -> pd.Series:
+def nap(data: Data, decreasing: bool = False, phases: List[str] = None) -> pd.Series:
     """
     Calculate the Nonoverlap Pairs (NAP) between two phases in a single-case data frame.
 
     Args:
         data (singlecase.Data): A single-case data set.
         decreasing (bool, optional): If you expect data to be lower in the second phase,
             set decreasing=True. Default is decreasing=False.
+        phases (List[str], optional): The phases to be compared. Must be provided if there are more than
+            two phases in the data set. Default is None.
 
     Returns:
         nap values: The calculated NAP values in a pd.Series.
     """
 
     pvar = data.pvar
-    phases = data._df[pvar].unique()
-    if len(phases) != 2:
-        raise ValueError(f"Only two phases are supported. The following phases were found in the phase variable : {pvar}: {phases}")
-    
+
+    if phases is not None:
+        if len(phases) != 2:
+            raise ValueError("Only two phases are supported")
+        for phase in phases:
+            if phase not in data.phases:
+                raise ValueError(f"Phase {phase} not found in phase variable {pvar}")
+    else:
+        phases = data.phases
+        if len(phases) != 2:
+            raise ValueError(f"Only two phases are supported. The following phases were found in the phase variable : {pvar}: {phases}")
 
     nap_values = {}
 
-    df = data._df
     for dvar in data.dvars:
-        
-        phase1_data = df.loc[df[pvar] == phases[0], dvar].dropna().values
-        phase2_data = df.loc[df[pvar] == phases[1], dvar].dropna().values
+        phase1_data = data.phase_data(phases[0], dvar).dropna().values
+        phase2_data = data.phase_data(phases[1], dvar).dropna().values
 
         non_overlapping_pairs = 0
         total_pairs = 0
 
         for value1 in phase1_data:
             for value2 in phase2_data:
                 total_pairs += 1
@@ -43,37 +51,46 @@
                         non_overlapping_pairs += 1
 
         nap_values[dvar] = non_overlapping_pairs / total_pairs
 
     return pd.Series(nap_values, name='nap')
 
 
-def pnd(data: Data, decreasing: bool = False) -> pd.Series:
+def pnd(data: Data, decreasing: bool = False, phases: List[str] = None) -> pd.Series:
     """
     Calculate the Percent Non-overlapping Data (PND) between two phases in a single-case data frame.
 
     Args:
         data (singlecase.Data): A single-case data set.
         decreasing (bool, optional): If you expect data to be lower in the second phase,
             set decreasing=True. Default is decreasing=False.
+        phases (List[str], optional): The phases to be compared. Must be provided if there are more than
+            two phases in the data set. Default is None.
     Returns:
         pnd_values (pd.Series): The calculated PND values in a pd.Series.
     """
 
     pvar = data.pvar
-    phases = data._df[pvar].unique()
-    if len(phases) != 2:
-        raise ValueError(f"Only two phases are supported. The following phases were found in the phase variable : {pvar}: {phases}")
+
+    if phases is not None:
+        if len(phases) != 2:
+            raise ValueError("Only two phases are supported")
+        for phase in phases:
+            if phase not in data.phases:
+                raise ValueError(f"Phase {phase} not found in phase variable {pvar}")
+    else:
+        phases = data.phases
+        if len(phases) != 2:
+            raise ValueError(f"Only two phases are supported. The following phases were found in the phase variable : {pvar}: {phases}")
 
     pnd_values = {}
 
-    df = data._df
     for dvar in data.dvars:
-        phase1_data = df.loc[df[pvar] == phases[0], dvar].dropna().values
-        phase2_data = df.loc[df[pvar] == phases[1], dvar].dropna().values
+        phase1_data = data.phase_data(phases[0], dvar).dropna().values
+        phase2_data = data.phase_data(phases[1], dvar).dropna().values
 
         extreme_value = max(phase1_data) if decreasing else min(phase1_data)
         non_overlapping_data = sum(value > extreme_value for value in phase2_data) if not decreasing else sum(value < extreme_value for value in phase2_data)
 
         pnd_values[dvar] = (non_overlapping_data / len(phase2_data)) * 100
 
     return pd.Series(pnd_values, name='pnd')
```

### Comparing `singlecase-0.2.0/singlecase/permtest/__init__.py` & `singlecase-0.2.1/singlecase/permtest/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,51 +2,61 @@
 from typing import List, Tuple, Union, Callable    
 import pandas as pd
 
 from singlecase.data import Data
 
 def permutation_test(data: Data,
                      statistic: Union[str, Callable] = 'mean',
+                     phases: List[str] = None,
                      num_rounds: int = 10000,
                      seed: int = None) -> pd.Series:
     """
     Perform a permutation test between two phases in a single-case data frame.
 
     Args:
         data (singlecase.Data): A single-case data set.
         statistic (Union[str, Callable], optional): The statistic to be used in the permutation test
             (either 'mean', 'median', or a custom callable). Default is 'mean'.
+        phases (List[str], optional): The phases to be compared. Must be provided if there are more than
+            two phases in the data set. Default is None.
         num_rounds (int, optional): The number of iterations for the permutation test. Default is 10000.
         seed (int, optional): Random seed for reproducibility. Default is None.
 
     Returns:
         p_values (pd.Series): The calculated p-values in a pd.Series.
     """
 
     pvar = data.pvar
-    phases = data._df[pvar].unique()
-    if len(phases) != 2:
-        raise ValueError(f"Only two phases are supported. The following phases were found in the phase variable : {pvar}: {phases}")
+
+    if phases is not None:
+        if len(phases) != 2:
+            raise ValueError("Only two phases are supported")
+        for phase in phases:
+            if phase not in data.phases:
+                raise ValueError(f"Phase {phase} not found in phase variable {pvar}")
+    else:
+        phases = data.phases
+        if len(phases) != 2:
+            raise ValueError(f"Only two phases are supported. The following phases were found in the phase variable : {pvar}: {phases}")
 
     if isinstance(statistic, str):
         if statistic == 'mean':
             statistic = np.mean
         elif statistic == 'median':
             statistic = np.median
         else:
             raise ValueError("statistic must be either 'mean', 'median', or a callable")
 
     np.random.seed(seed)
 
     p_values = {}
 
-    df = data._df
     for dvar in data.dvars:
-        phase1_data = df.loc[df[pvar] == phases[0], dvar].dropna().values
-        phase2_data = df.loc[df[pvar] == phases[1], dvar].dropna().values
+        phase1_data = data.phase_data(phases[0], dvar).dropna().values
+        phase2_data = data.phase_data(phases[1], dvar).dropna().values
 
         observed_diff = statistic(phase2_data) - statistic(phase1_data)
 
         combined_data = np.concatenate((phase1_data, phase2_data))
 
         permuted_diffs = []
         for _ in range(num_rounds):
```

### Comparing `singlecase-0.2.0/singlecase.egg-info/PKG-INFO` & `singlecase-0.2.1/singlecase.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: singlecase
-Version: 0.2.0
+Version: 0.2.1
 Summary: A tool for single-case design data managment, statistical analysis and visualization.
 Author-email: Casper Wilstrup <casper.wilstrup@abzu.ai>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, Casper Wilstrup
         
         Redistribution and use in source and binary forms, with or without
@@ -73,93 +73,98 @@
 ```python
 from singlecase.data import Data
 ```
 
 Then, create a `Data` object with either a pandas DataFrame or a dictionary:
 
 ```python
-df = pd.DataFrame({...})  # Or load your data from a CSV, database, etc.
-data = Data(df)
+data = Data({
+    'phase': ['A1', 'A1', 'A1', 'B', 'B', 'B', 'A2', 'A2', 'A2'],
+    'dvar1': [1.0, 2.5, 3.2, 4.2, 5.5, 6.2, 2.0, 2.4, 3.1],
+    'dvar2': [2.5, 3.2, 4.6, 5.6, 6.2, 7.8, 3.3, 4.1, 4.8],
+})
 ```
 
-Now you're ready to perform single-case data analysis!
+Now you're ready to perform single-case data analysis.
 
 ## Core Features
 
 ### Data Class
 
 The `Data` class provides an object-oriented interface to represent your single-case data. It assumes any variable with datatype of float as a dependent variable. The dependent and phase variables can be accessed and modified using properties. For example:
 
 ```python
-data.pvar = 'column_name'  # Set the phase variable
+data.pvar = 'column_name'  # Set the phase variable, if it is not named 'phase'
 ```
 
 ### Nonoverlap Pairs (NAP)
 
 The `nap` function computes the Nonoverlap Pairs between two phases in a single-case data frame. It returns a pandas Series containing the NAP values for each dependent variable in the data set.
 
 ```python
 from singlecase.effectsize import nap
-nap_values = nap(data)
+nap_values = nap(data, phases["A1", "B"])
 ```
 
 ### Percent Non-overlapping Data (PND)
 
 The `pnd` function computes the Percent Non-overlapping Data between two phases in a single-case data frame. It returns a pandas Series containing the PND values for each dependent variable in the data set.
 
 ```python
 from singlecase.effectsize import pnd
-pnd_values = pnd(data)
+pnd_values = pnd(data, phases=["A1", "B"])
 ```
 
 ### Permutation Test
 
-The `permutation_test` function performs a permutation test between two phases in a single-case data frame. It returns a pandas Series containing the p-values for each dependent variable in the data set.
+The `permutation_test` function performs a permutation test between two phases in a single-case data frame. It returns a pandas Series containing the p-values for each dependent variable in the data set. The p-value is the probability that the two phases have the same mean.
 
 ```python
 from singlecase.permtest import permutation_test
-p_values = permutation_test(data)
+p_values = permutation_test(data, phases=["A1","A2"])
 ```
 
 
 ## Complete example
 
-This complete example creates a new `singlecase.Data` from a Python dictionary. The dataset has two dependent variables `dvar1` and `dvar2`. The phase variable is called `phase` and consists of the two phases "A" and "B". Based on this data, the PND and NAP values are calculated and printed.
+This complete example creates a new `singlecase.Data` from a Python dictionary. The dataset has two dependent variables `dvar1` and `dvar2`. The phase variable is called `phase` and consists of the two phases "A" and "B". Based on this data, the PND and NAP values are calculated and printed. The probability that the two phases have the same mean is then calculated using permutation tests and printed. Since the data contains only two phases, it is not necessary to specify which phases to compare in `pnd`, `nap` and `permutation_test` function calls.
 
 ```python
 import pandas as pd
 from singlecase.data import Data
 from singlecase.effectsize import pnd, nap
+from singlecase.permtest import permutation_test
 
 # Create a sample data
 data_dict = {
+    'phase': ['A', 'A', 'A', 'A', 'A', 'A', 'B', 'B', 'B', 'B', 'B', 'B'],
     'dvar1': [1.0, 2.5, 3.2, 4.6, 2.8, 5.6, 3.7, 4.2, 5.5, 6.2, 7.3, 8.5],
     'dvar2': [2.5, 3.2, 4.6, 5.1, 4.8, 5.2, 6.7, 5.6, 6.2, 7.8, 8.4, 7.2],
-    'phase': ['A', 'A', 'A', 'A', 'A', 'A', 'B', 'B', 'B', 'B', 'B', 'B']
 }
 
-df = pd.DataFrame(data_dict)
-
 # Instantiate Data object
-data = Data(df)
-
-# Set phase variable
-data.pvar = 'phase'
+data = Data(data_dict)
 
 # Calculate PND
 pnd_values = pnd(data)
-print(f"PND values: \n{pnd_values}")
+print(f"PND values:\n{pnd_values}\n")
 
 # Calculate NAP
 nap_values = nap(data)
-print(f"NAP values: \n{nap_values}")
+print(f"NAP values:\n{nap_values}\n")
+
+# Calculate the p-value the mean of the two phases being the same
+perm_p = permutation_test(data)
+print(f"Probability that A and B phases have same mean:\n{perm_p}\n")
 ```
 
 
 ## License
 
-This project is licensed under the BSD 3-clause license - see the [LICENSE](LICENSE) file for details.
+This project is licensed under the BSD 3-clause license - see the LICENSE file for details.
+
+## About the package
 
-## Acknowledgments
+The Single Case Research package is supported by [Abzu](https://www.abzu.ai) as part of an ongoing mission to improve scientific research powered by artificial intelligence.
 
-- The Single Case Research package is being developed by Casper Wilstrup.
+The primary author of the package is [Casper Wilstrup](https://twitter.com/cwilstrup). New contributors are welcome.
```

