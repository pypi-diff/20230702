# Comparing `tmp/singlecase-0.1.0.tar.gz` & `tmp/singlecase-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "singlecase-0.1.0.tar", last modified: Sat Jul  1 12:26:23 2023, max compression
+gzip compressed data, was "singlecase-0.2.0.tar", last modified: Sun Jul  2 07:43:58 2023, max compression
```

## Comparing `singlecase-0.1.0.tar` & `singlecase-0.2.0.tar`

### file list

```diff
@@ -1,19 +1,21 @@
-drwxrwxr-x   0 cw        (1000) cw        (1000)        0 2023-07-01 12:26:23.211259 singlecase-0.1.0/
--rw-rw-r--   0 cw        (1000) cw        (1000)     1502 2023-07-01 11:26:29.000000 singlecase-0.1.0/LICENSE
--rw-rw-r--   0 cw        (1000) cw        (1000)     6133 2023-07-01 12:26:23.211259 singlecase-0.1.0/PKG-INFO
--rw-rw-r--   0 cw        (1000) cw        (1000)     3813 2023-07-01 11:26:29.000000 singlecase-0.1.0/README.md
--rw-rw-r--   0 cw        (1000) cw        (1000)      903 2023-07-01 12:25:50.000000 singlecase-0.1.0/pyproject.toml
--rw-rw-r--   0 cw        (1000) cw        (1000)       38 2023-07-01 12:26:23.211259 singlecase-0.1.0/setup.cfg
--rw-rw-r--   0 cw        (1000) cw        (1000)       37 2023-07-01 11:26:29.000000 singlecase-0.1.0/setup.py
-drwxrwxr-x   0 cw        (1000) cw        (1000)        0 2023-07-01 12:26:23.207258 singlecase-0.1.0/singlecase/
--rw-rw-r--   0 cw        (1000) cw        (1000)       47 2023-07-01 12:16:19.000000 singlecase-0.1.0/singlecase/__init__.py
-drwxrwxr-x   0 cw        (1000) cw        (1000)        0 2023-07-01 12:26:23.211259 singlecase-0.1.0/singlecase/effectsize/
--rw-rw-r--   0 cw        (1000) cw        (1000)     4293 2023-07-01 12:15:58.000000 singlecase-0.1.0/singlecase/effectsize/__init__.py
-drwxrwxr-x   0 cw        (1000) cw        (1000)        0 2023-07-01 12:26:23.211259 singlecase-0.1.0/singlecase/permtest/
--rw-rw-r--   0 cw        (1000) cw        (1000)     3304 2023-07-01 11:26:29.000000 singlecase-0.1.0/singlecase/permtest/__init__.py
-drwxrwxr-x   0 cw        (1000) cw        (1000)        0 2023-07-01 12:26:23.211259 singlecase-0.1.0/singlecase.egg-info/
--rw-rw-r--   0 cw        (1000) cw        (1000)     6133 2023-07-01 12:26:23.000000 singlecase-0.1.0/singlecase.egg-info/PKG-INFO
--rw-rw-r--   0 cw        (1000) cw        (1000)      299 2023-07-01 12:26:23.000000 singlecase-0.1.0/singlecase.egg-info/SOURCES.txt
--rw-rw-r--   0 cw        (1000) cw        (1000)        1 2023-07-01 12:26:23.000000 singlecase-0.1.0/singlecase.egg-info/dependency_links.txt
--rw-rw-r--   0 cw        (1000) cw        (1000)       49 2023-07-01 12:26:23.000000 singlecase-0.1.0/singlecase.egg-info/requires.txt
--rw-rw-r--   0 cw        (1000) cw        (1000)       11 2023-07-01 12:26:23.000000 singlecase-0.1.0/singlecase.egg-info/top_level.txt
+drwxrwxr-x   0 cw        (1000) cw        (1000)        0 2023-07-02 07:43:58.263678 singlecase-0.2.0/
+-rw-rw-r--   0 cw        (1000) cw        (1000)     1502 2023-07-01 11:26:29.000000 singlecase-0.2.0/LICENSE
+-rw-rw-r--   0 cw        (1000) cw        (1000)     6422 2023-07-02 07:43:58.263678 singlecase-0.2.0/PKG-INFO
+-rw-rw-r--   0 cw        (1000) cw        (1000)     3582 2023-07-02 07:43:40.000000 singlecase-0.2.0/README.md
+-rw-rw-r--   0 cw        (1000) cw        (1000)     1391 2023-07-02 07:31:39.000000 singlecase-0.2.0/pyproject.toml
+-rw-rw-r--   0 cw        (1000) cw        (1000)       38 2023-07-02 07:43:58.263678 singlecase-0.2.0/setup.cfg
+-rw-rw-r--   0 cw        (1000) cw        (1000)       37 2023-07-01 11:26:29.000000 singlecase-0.2.0/setup.py
+drwxrwxr-x   0 cw        (1000) cw        (1000)        0 2023-07-02 07:43:58.263678 singlecase-0.2.0/singlecase/
+-rw-rw-r--   0 cw        (1000) cw        (1000)      144 2023-07-02 06:56:34.000000 singlecase-0.2.0/singlecase/__init__.py
+drwxrwxr-x   0 cw        (1000) cw        (1000)        0 2023-07-02 07:43:58.263678 singlecase-0.2.0/singlecase/data/
+-rw-rw-r--   0 cw        (1000) cw        (1000)     2342 2023-07-02 07:07:38.000000 singlecase-0.2.0/singlecase/data/__init__.py
+drwxrwxr-x   0 cw        (1000) cw        (1000)        0 2023-07-02 07:43:58.263678 singlecase-0.2.0/singlecase/effectsize/
+-rw-rw-r--   0 cw        (1000) cw        (1000)     2748 2023-07-02 06:56:48.000000 singlecase-0.2.0/singlecase/effectsize/__init__.py
+drwxrwxr-x   0 cw        (1000) cw        (1000)        0 2023-07-02 07:43:58.263678 singlecase-0.2.0/singlecase/permtest/
+-rw-rw-r--   0 cw        (1000) cw        (1000)     2414 2023-07-02 06:57:09.000000 singlecase-0.2.0/singlecase/permtest/__init__.py
+drwxrwxr-x   0 cw        (1000) cw        (1000)        0 2023-07-02 07:43:58.263678 singlecase-0.2.0/singlecase.egg-info/
+-rw-rw-r--   0 cw        (1000) cw        (1000)     6422 2023-07-02 07:43:58.000000 singlecase-0.2.0/singlecase.egg-info/PKG-INFO
+-rw-rw-r--   0 cw        (1000) cw        (1000)      327 2023-07-02 07:43:58.000000 singlecase-0.2.0/singlecase.egg-info/SOURCES.txt
+-rw-rw-r--   0 cw        (1000) cw        (1000)        1 2023-07-02 07:43:58.000000 singlecase-0.2.0/singlecase.egg-info/dependency_links.txt
+-rw-rw-r--   0 cw        (1000) cw        (1000)       49 2023-07-02 07:43:58.000000 singlecase-0.2.0/singlecase.egg-info/requires.txt
+-rw-rw-r--   0 cw        (1000) cw        (1000)       11 2023-07-02 07:43:58.000000 singlecase-0.2.0/singlecase.egg-info/top_level.txt
```

### Comparing `singlecase-0.1.0/LICENSE` & `singlecase-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `singlecase-0.1.0/PKG-INFO` & `singlecase-0.2.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: singlecase
-Version: 0.1.0
-Summary: Work with data from single case study designs
+Version: 0.2.0
+Summary: A tool for single-case design data managment, statistical analysis and visualization.
 Author-email: Casper Wilstrup <casper.wilstrup@abzu.ai>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, Casper Wilstrup
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
@@ -29,117 +29,136 @@
         DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
         SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
         CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
         OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
         OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
         
 Project-URL: Homepage, https://github.com/wilstrup/singlecase
-Keywords: single case,permutation test,pnd,nap,effect size
+Keywords: single case,permutation test,pnd,nap,effect size,non-overlapping,statistical analysis,research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.9
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Intended Audience :: Science/Research
+Classifier: Intended Audience :: Healthcare Industry
+Classifier: Intended Audience :: Education
+Classifier: Topic :: Scientific/Engineering :: Mathematics
+Classifier: Topic :: Scientific/Engineering :: Visualization
+Classifier: Topic :: Scientific/Engineering :: Information Analysis
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # Single Case Research Package
 
-The Single Case Research package is a Python library designed to assist in conducting single-case research studies. It provides functions to calculate effect sizes and perform permutation tests between two phases in a single-case data frame.
+The Single Case Research package is a Python library designed to assist in conducting single-case research studies. The package provides tools to analyze single-case data sets. It is designed for simplicity and ease of use, with a range of methods to calculate various statistical measures for single-case data sets. The package is perfect for analysts and researchers dealing with single-case designs, providing a framework to load, manage, and manipulate such data, along with robust statistical functions to interpret the data.
 
 More functionality will be added as the package is further developed
 
 ## Installation
 
 You can install the package using pip:
 
 ```shell
 pip install singlecase
 ```
 
-## Functionality
 
-The package currently includes the following functions:
+## Usage
 
-### Effect Size Calculation
+To use `singlecase`, first import the package into your Python environment:
 
-#### `nap(data: pd.DataFrame, dvars: Union[List[str], str], pvar: str, decreasing: bool = False, phases: Tuple[str, str] = ("A", "B")) -> pd.Series`
+```python
+from singlecase.data import Data
+```
 
-Calculate the Nonoverlap Pairs (NAP) between two phases in a single-case data frame.
+Then, create a `Data` object with either a pandas DataFrame or a dictionary:
 
-- `data`: A single-case data frame.
-- `dvars`: One or more dependent variables to calculate NAP for.
-- `pvar`: The name of the phase variable.
-- `decreasing`: If you expect data to be lower in the second phase, set `decreasing=True`. Default is `decreasing=False`.
-- `phases`: A tuple of two column names in the data frame indicating the two phases that should be compared. Default is `("A", "B")`.
+```python
+df = pd.DataFrame({...})  # Or load your data from a CSV, database, etc.
+data = Data(df)
+```
 
-Returns the calculated NAP values in a Pandas Series.
+Now you're ready to perform single-case data analysis!
 
-#### `pnd(data: pd.DataFrame, dvars: Union[List[str], str], pvar: str, decreasing: bool = False, phases: Tuple[str, str] = ("A", "B")) -> pd.Series`
+## Core Features
 
-Calculate the Percent Non-overlapping Data (PND) between two phases in a single-case data frame.
+### Data Class
 
-- `data`: A single-case data frame.
-- `dvars`: One or more dependent variables to calculate PND for.
-- `pvar`: The name of the phase variable.
-- `decreasing`: If you expect data to be lower in the second phase, set `decreasing=True`. Default is `decreasing=False`.
-- `phases`: A tuple of two column names in the data frame indicating the two phases that should be compared. Default is `("A", "B")`.
+The `Data` class provides an object-oriented interface to represent your single-case data. It assumes any variable with datatype of float as a dependent variable. The dependent and phase variables can be accessed and modified using properties. For example:
 
-Returns the calculated PND values in a Pandas Series.
+```python
+data.pvar = 'column_name'  # Set the phase variable
+```
 
-### Permutation Test
+### Nonoverlap Pairs (NAP)
 
-#### `permutation_test(data: pd.DataFrame, dvars: Union[List[str], str], pvar: str, statistic: Union[str, Callable] = 'mean', phases: Tuple[str, str] = ("A", "B"), num_rounds: int = 10000, seed: int = None) -> pd.Series`
+The `nap` function computes the Nonoverlap Pairs between two phases in a single-case data frame. It returns a pandas Series containing the NAP values for each dependent variable in the data set.
 
-Perform a permutation test between two phases in a single-case data frame.
+```python
+from singlecase.effectsize import nap
+nap_values = nap(data)
+```
 
-- `data`: A single-case data frame.
-- `dvars`: One or more dependent variables to perform the permutation test on.
-- `pvar`: The name of the phase variable.
-- `statistic`: The statistic to be used in the permutation test (either 'mean', 'median', or a custom callable). Default is `'mean'`.
-- `phases`: A tuple of two column names in the data frame indicating the two phases that should be compared. Default is `("A", "B")`.
-- `num_rounds`: The number of iterations for the permutation test. Default is `10000`.
-- `seed`: Random seed for reproducibility. Default is `None`.
+### Percent Non-overlapping Data (PND)
 
-Returns the calculated p-values in a Pandas Series.
+The `pnd` function computes the Percent Non-overlapping Data between two phases in a single-case data frame. It returns a pandas Series containing the PND values for each dependent variable in the data set.
 
-## Usage
+```python
+from singlecase.effectsize import pnd
+pnd_values = pnd(data)
+```
 
-Here's a basic example demonstrating how to use the functions in the Single Case Research package:
+### Permutation Test
+
+The `permutation_test` function performs a permutation test between two phases in a single-case data frame. It returns a pandas Series containing the p-values for each dependent variable in the data set.
 
 ```python
-import pandas as pd
-from singlecase.effectsize import nap, pnd
 from singlecase.permtest import permutation_test
+p_values = permutation_test(data)
+```
 
-# Load your single-case data into a Pandas DataFrame
 
+## Complete example
 
+This complete example creates a new `singlecase.Data` from a Python dictionary. The dataset has two dependent variables `dvar1` and `dvar2`. The phase variable is called `phase` and consists of the two phases "A" and "B". Based on this data, the PND and NAP values are calculated and printed.
 
-# Calculate NAP
-nap_values = nap(data, dvars=['dependent_var1', 'dependent_var2'], pvar='phase_var')
+```python
+import pandas as pd
+from singlecase.data import Data
+from singlecase.effectsize import pnd, nap
 
-# Calculate PND
-pnd_values = pnd(data, dvars='dependent_var1', pvar='phase_var')
+# Create a sample data
+data_dict = {
+    'dvar1': [1.0, 2.5, 3.2, 4.6, 2.8, 5.6, 3.7, 4.2, 5.5, 6.2, 7.3, 8.5],
+    'dvar2': [2.5, 3.2, 4.6, 5.1, 4.8, 5.2, 6.7, 5.6, 6.2, 7.8, 8.4, 7.2],
+    'phase': ['A', 'A', 'A', 'A', 'A', 'A', 'B', 'B', 'B', 'B', 'B', 'B']
+}
+
+df = pd.DataFrame(data_dict)
 
-# Perform permutation test
-p_values = permutation_test(data, dvars='dependent_var1', pvar='phase_var')
+# Instantiate Data object
+data = Data(df)
 
-# Print the results
-print("NAP Values:")
-print(nap_values)
+# Set phase variable
+data.pvar = 'phase'
 
-print("PND Values:")
-print(pnd_values)
+# Calculate PND
+pnd_values = pnd(data)
+print(f"PND values: \n{pnd_values}")
 
-print("P-Values:")
-print(p_values)
+# Calculate NAP
+nap_values = nap(data)
+print(f"NAP values: \n{nap_values}")
 ```
 
+
 ## License
 
 This project is licensed under the BSD 3-clause license - see the [LICENSE](LICENSE) file for details.
 
 ## Acknowledgments
 
 - The Single Case Research package is being developed by Casper Wilstrup.
```

### Comparing `singlecase-0.1.0/README.md` & `singlecase-0.2.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,100 +1,111 @@
 # Single Case Research Package
 
-The Single Case Research package is a Python library designed to assist in conducting single-case research studies. It provides functions to calculate effect sizes and perform permutation tests between two phases in a single-case data frame.
+The Single Case Research package is a Python library designed to assist in conducting single-case research studies. The package provides tools to analyze single-case data sets. It is designed for simplicity and ease of use, with a range of methods to calculate various statistical measures for single-case data sets. The package is perfect for analysts and researchers dealing with single-case designs, providing a framework to load, manage, and manipulate such data, along with robust statistical functions to interpret the data.
 
 More functionality will be added as the package is further developed
 
 ## Installation
 
 You can install the package using pip:
 
 ```shell
 pip install singlecase
 ```
 
-## Functionality
 
-The package currently includes the following functions:
+## Usage
 
-### Effect Size Calculation
+To use `singlecase`, first import the package into your Python environment:
 
-#### `nap(data: pd.DataFrame, dvars: Union[List[str], str], pvar: str, decreasing: bool = False, phases: Tuple[str, str] = ("A", "B")) -> pd.Series`
+```python
+from singlecase.data import Data
+```
 
-Calculate the Nonoverlap Pairs (NAP) between two phases in a single-case data frame.
+Then, create a `Data` object with either a pandas DataFrame or a dictionary:
 
-- `data`: A single-case data frame.
-- `dvars`: One or more dependent variables to calculate NAP for.
-- `pvar`: The name of the phase variable.
-- `decreasing`: If you expect data to be lower in the second phase, set `decreasing=True`. Default is `decreasing=False`.
-- `phases`: A tuple of two column names in the data frame indicating the two phases that should be compared. Default is `("A", "B")`.
+```python
+df = pd.DataFrame({...})  # Or load your data from a CSV, database, etc.
+data = Data(df)
+```
 
-Returns the calculated NAP values in a Pandas Series.
+Now you're ready to perform single-case data analysis!
 
-#### `pnd(data: pd.DataFrame, dvars: Union[List[str], str], pvar: str, decreasing: bool = False, phases: Tuple[str, str] = ("A", "B")) -> pd.Series`
+## Core Features
 
-Calculate the Percent Non-overlapping Data (PND) between two phases in a single-case data frame.
+### Data Class
 
-- `data`: A single-case data frame.
-- `dvars`: One or more dependent variables to calculate PND for.
-- `pvar`: The name of the phase variable.
-- `decreasing`: If you expect data to be lower in the second phase, set `decreasing=True`. Default is `decreasing=False`.
-- `phases`: A tuple of two column names in the data frame indicating the two phases that should be compared. Default is `("A", "B")`.
+The `Data` class provides an object-oriented interface to represent your single-case data. It assumes any variable with datatype of float as a dependent variable. The dependent and phase variables can be accessed and modified using properties. For example:
 
-Returns the calculated PND values in a Pandas Series.
+```python
+data.pvar = 'column_name'  # Set the phase variable
+```
 
-### Permutation Test
+### Nonoverlap Pairs (NAP)
 
-#### `permutation_test(data: pd.DataFrame, dvars: Union[List[str], str], pvar: str, statistic: Union[str, Callable] = 'mean', phases: Tuple[str, str] = ("A", "B"), num_rounds: int = 10000, seed: int = None) -> pd.Series`
+The `nap` function computes the Nonoverlap Pairs between two phases in a single-case data frame. It returns a pandas Series containing the NAP values for each dependent variable in the data set.
 
-Perform a permutation test between two phases in a single-case data frame.
+```python
+from singlecase.effectsize import nap
+nap_values = nap(data)
+```
 
-- `data`: A single-case data frame.
-- `dvars`: One or more dependent variables to perform the permutation test on.
-- `pvar`: The name of the phase variable.
-- `statistic`: The statistic to be used in the permutation test (either 'mean', 'median', or a custom callable). Default is `'mean'`.
-- `phases`: A tuple of two column names in the data frame indicating the two phases that should be compared. Default is `("A", "B")`.
-- `num_rounds`: The number of iterations for the permutation test. Default is `10000`.
-- `seed`: Random seed for reproducibility. Default is `None`.
+### Percent Non-overlapping Data (PND)
 
-Returns the calculated p-values in a Pandas Series.
+The `pnd` function computes the Percent Non-overlapping Data between two phases in a single-case data frame. It returns a pandas Series containing the PND values for each dependent variable in the data set.
 
-## Usage
+```python
+from singlecase.effectsize import pnd
+pnd_values = pnd(data)
+```
 
-Here's a basic example demonstrating how to use the functions in the Single Case Research package:
+### Permutation Test
+
+The `permutation_test` function performs a permutation test between two phases in a single-case data frame. It returns a pandas Series containing the p-values for each dependent variable in the data set.
 
 ```python
-import pandas as pd
-from singlecase.effectsize import nap, pnd
 from singlecase.permtest import permutation_test
+p_values = permutation_test(data)
+```
 
-# Load your single-case data into a Pandas DataFrame
 
+## Complete example
 
+This complete example creates a new `singlecase.Data` from a Python dictionary. The dataset has two dependent variables `dvar1` and `dvar2`. The phase variable is called `phase` and consists of the two phases "A" and "B". Based on this data, the PND and NAP values are calculated and printed.
 
-# Calculate NAP
-nap_values = nap(data, dvars=['dependent_var1', 'dependent_var2'], pvar='phase_var')
+```python
+import pandas as pd
+from singlecase.data import Data
+from singlecase.effectsize import pnd, nap
 
-# Calculate PND
-pnd_values = pnd(data, dvars='dependent_var1', pvar='phase_var')
+# Create a sample data
+data_dict = {
+    'dvar1': [1.0, 2.5, 3.2, 4.6, 2.8, 5.6, 3.7, 4.2, 5.5, 6.2, 7.3, 8.5],
+    'dvar2': [2.5, 3.2, 4.6, 5.1, 4.8, 5.2, 6.7, 5.6, 6.2, 7.8, 8.4, 7.2],
+    'phase': ['A', 'A', 'A', 'A', 'A', 'A', 'B', 'B', 'B', 'B', 'B', 'B']
+}
+
+df = pd.DataFrame(data_dict)
 
-# Perform permutation test
-p_values = permutation_test(data, dvars='dependent_var1', pvar='phase_var')
+# Instantiate Data object
+data = Data(df)
 
-# Print the results
-print("NAP Values:")
-print(nap_values)
+# Set phase variable
+data.pvar = 'phase'
 
-print("PND Values:")
-print(pnd_values)
+# Calculate PND
+pnd_values = pnd(data)
+print(f"PND values: \n{pnd_values}")
 
-print("P-Values:")
-print(p_values)
+# Calculate NAP
+nap_values = nap(data)
+print(f"NAP values: \n{nap_values}")
 ```
 
+
 ## License
 
 This project is licensed under the BSD 3-clause license - see the [LICENSE](LICENSE) file for details.
 
 ## Acknowledgments
 
 - The Single Case Research package is being developed by Casper Wilstrup.
```

### Comparing `singlecase-0.1.0/singlecase/permtest/__init__.py` & `singlecase-0.2.0/singlecase/permtest/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,69 +1,52 @@
 import numpy as np
 from typing import List, Tuple, Union, Callable    
 import pandas as pd
 
-def permutation_test(data: pd.DataFrame,
-                     dvars: Union[List[str], str],
-                     pvar: str,
+from singlecase.data import Data
+
+def permutation_test(data: Data,
                      statistic: Union[str, Callable] = 'mean',
-                     phases: Tuple[str, str] = ("A", "B"),
                      num_rounds: int = 10000,
                      seed: int = None) -> pd.Series:
     """
     Perform a permutation test between two phases in a single-case data frame.
 
     Args:
-        data (pd.DataFrame): A single-case data frame.
-        dvars (Union[List[str], str]): One or more dependent variables to perform the permutation test on.
-        pvar (str): The name of the phase variable.
+        data (singlecase.Data): A single-case data set.
         statistic (Union[str, Callable], optional): The statistic to be used in the permutation test
             (either 'mean', 'median', or a custom callable). Default is 'mean'.
-        phases (Tuple[str, str], optional): A tuple of two column names in the data frame
-            indicating the two phases that should be compared. Default is ("A", "B").
         num_rounds (int, optional): The number of iterations for the permutation test. Default is 10000.
         seed (int, optional): Random seed for reproducibility. Default is None.
 
     Returns:
         p_values (pd.Series): The calculated p-values in a pd.Series.
     """
 
-    if isinstance(dvars, str):
-        dvars = [dvars]
-
-    if pvar not in data.columns:
-        raise ValueError("pvar must be the name of a column in the data frame")
-
+    pvar = data.pvar
+    phases = data._df[pvar].unique()
     if len(phases) != 2:
-        raise ValueError("phases must be a tuple of two phase names")
-
-    if phases[0] not in data[pvar].values or phases[1] not in data[pvar].values:
-        raise ValueError("phases must be a tuple of two phase names that are present in the data frame")
+        raise ValueError(f"Only two phases are supported. The following phases were found in the phase variable : {pvar}: {phases}")
 
     if isinstance(statistic, str):
         if statistic == 'mean':
             statistic = np.mean
         elif statistic == 'median':
             statistic = np.median
         else:
             raise ValueError("statistic must be either 'mean', 'median', or a callable")
 
     np.random.seed(seed)
 
     p_values = {}
 
-    for dvar in dvars:
-        if dvar not in data.columns:
-            raise ValueError("dvar must be the name of a column in the data frame")
-
-        phase1_data = data.loc[data[pvar] == phases[0], dvar].values
-        phase2_data = data.loc[data[pvar] == phases[1], dvar].values
-
-        phase1_data = phase1_data[~np.isnan(phase1_data)]
-        phase2_data = phase2_data[~np.isnan(phase2_data)]
+    df = data._df
+    for dvar in data.dvars:
+        phase1_data = df.loc[df[pvar] == phases[0], dvar].dropna().values
+        phase2_data = df.loc[df[pvar] == phases[1], dvar].dropna().values
 
         observed_diff = statistic(phase2_data) - statistic(phase1_data)
 
         combined_data = np.concatenate((phase1_data, phase2_data))
 
         permuted_diffs = []
         for _ in range(num_rounds):
@@ -74,7 +57,9 @@
             permuted_diffs.append(permuted_diff)
 
         permuted_diffs = np.array(permuted_diffs)
         p_value = (np.abs(permuted_diffs) >= np.abs(observed_diff)).sum() / num_rounds
         p_values[dvar] = p_value
 
     return pd.Series(p_values, name="p_value")
+
+
```

### Comparing `singlecase-0.1.0/singlecase.egg-info/PKG-INFO` & `singlecase-0.2.0/singlecase.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: singlecase
-Version: 0.1.0
-Summary: Work with data from single case study designs
+Version: 0.2.0
+Summary: A tool for single-case design data managment, statistical analysis and visualization.
 Author-email: Casper Wilstrup <casper.wilstrup@abzu.ai>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, Casper Wilstrup
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
@@ -29,117 +29,136 @@
         DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
         SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
         CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
         OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
         OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
         
 Project-URL: Homepage, https://github.com/wilstrup/singlecase
-Keywords: single case,permutation test,pnd,nap,effect size
+Keywords: single case,permutation test,pnd,nap,effect size,non-overlapping,statistical analysis,research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.9
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Intended Audience :: Science/Research
+Classifier: Intended Audience :: Healthcare Industry
+Classifier: Intended Audience :: Education
+Classifier: Topic :: Scientific/Engineering :: Mathematics
+Classifier: Topic :: Scientific/Engineering :: Visualization
+Classifier: Topic :: Scientific/Engineering :: Information Analysis
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # Single Case Research Package
 
-The Single Case Research package is a Python library designed to assist in conducting single-case research studies. It provides functions to calculate effect sizes and perform permutation tests between two phases in a single-case data frame.
+The Single Case Research package is a Python library designed to assist in conducting single-case research studies. The package provides tools to analyze single-case data sets. It is designed for simplicity and ease of use, with a range of methods to calculate various statistical measures for single-case data sets. The package is perfect for analysts and researchers dealing with single-case designs, providing a framework to load, manage, and manipulate such data, along with robust statistical functions to interpret the data.
 
 More functionality will be added as the package is further developed
 
 ## Installation
 
 You can install the package using pip:
 
 ```shell
 pip install singlecase
 ```
 
-## Functionality
 
-The package currently includes the following functions:
+## Usage
 
-### Effect Size Calculation
+To use `singlecase`, first import the package into your Python environment:
 
-#### `nap(data: pd.DataFrame, dvars: Union[List[str], str], pvar: str, decreasing: bool = False, phases: Tuple[str, str] = ("A", "B")) -> pd.Series`
+```python
+from singlecase.data import Data
+```
 
-Calculate the Nonoverlap Pairs (NAP) between two phases in a single-case data frame.
+Then, create a `Data` object with either a pandas DataFrame or a dictionary:
 
-- `data`: A single-case data frame.
-- `dvars`: One or more dependent variables to calculate NAP for.
-- `pvar`: The name of the phase variable.
-- `decreasing`: If you expect data to be lower in the second phase, set `decreasing=True`. Default is `decreasing=False`.
-- `phases`: A tuple of two column names in the data frame indicating the two phases that should be compared. Default is `("A", "B")`.
+```python
+df = pd.DataFrame({...})  # Or load your data from a CSV, database, etc.
+data = Data(df)
+```
 
-Returns the calculated NAP values in a Pandas Series.
+Now you're ready to perform single-case data analysis!
 
-#### `pnd(data: pd.DataFrame, dvars: Union[List[str], str], pvar: str, decreasing: bool = False, phases: Tuple[str, str] = ("A", "B")) -> pd.Series`
+## Core Features
 
-Calculate the Percent Non-overlapping Data (PND) between two phases in a single-case data frame.
+### Data Class
 
-- `data`: A single-case data frame.
-- `dvars`: One or more dependent variables to calculate PND for.
-- `pvar`: The name of the phase variable.
-- `decreasing`: If you expect data to be lower in the second phase, set `decreasing=True`. Default is `decreasing=False`.
-- `phases`: A tuple of two column names in the data frame indicating the two phases that should be compared. Default is `("A", "B")`.
+The `Data` class provides an object-oriented interface to represent your single-case data. It assumes any variable with datatype of float as a dependent variable. The dependent and phase variables can be accessed and modified using properties. For example:
 
-Returns the calculated PND values in a Pandas Series.
+```python
+data.pvar = 'column_name'  # Set the phase variable
+```
 
-### Permutation Test
+### Nonoverlap Pairs (NAP)
 
-#### `permutation_test(data: pd.DataFrame, dvars: Union[List[str], str], pvar: str, statistic: Union[str, Callable] = 'mean', phases: Tuple[str, str] = ("A", "B"), num_rounds: int = 10000, seed: int = None) -> pd.Series`
+The `nap` function computes the Nonoverlap Pairs between two phases in a single-case data frame. It returns a pandas Series containing the NAP values for each dependent variable in the data set.
 
-Perform a permutation test between two phases in a single-case data frame.
+```python
+from singlecase.effectsize import nap
+nap_values = nap(data)
+```
 
-- `data`: A single-case data frame.
-- `dvars`: One or more dependent variables to perform the permutation test on.
-- `pvar`: The name of the phase variable.
-- `statistic`: The statistic to be used in the permutation test (either 'mean', 'median', or a custom callable). Default is `'mean'`.
-- `phases`: A tuple of two column names in the data frame indicating the two phases that should be compared. Default is `("A", "B")`.
-- `num_rounds`: The number of iterations for the permutation test. Default is `10000`.
-- `seed`: Random seed for reproducibility. Default is `None`.
+### Percent Non-overlapping Data (PND)
 
-Returns the calculated p-values in a Pandas Series.
+The `pnd` function computes the Percent Non-overlapping Data between two phases in a single-case data frame. It returns a pandas Series containing the PND values for each dependent variable in the data set.
 
-## Usage
+```python
+from singlecase.effectsize import pnd
+pnd_values = pnd(data)
+```
 
-Here's a basic example demonstrating how to use the functions in the Single Case Research package:
+### Permutation Test
+
+The `permutation_test` function performs a permutation test between two phases in a single-case data frame. It returns a pandas Series containing the p-values for each dependent variable in the data set.
 
 ```python
-import pandas as pd
-from singlecase.effectsize import nap, pnd
 from singlecase.permtest import permutation_test
+p_values = permutation_test(data)
+```
 
-# Load your single-case data into a Pandas DataFrame
 
+## Complete example
 
+This complete example creates a new `singlecase.Data` from a Python dictionary. The dataset has two dependent variables `dvar1` and `dvar2`. The phase variable is called `phase` and consists of the two phases "A" and "B". Based on this data, the PND and NAP values are calculated and printed.
 
-# Calculate NAP
-nap_values = nap(data, dvars=['dependent_var1', 'dependent_var2'], pvar='phase_var')
+```python
+import pandas as pd
+from singlecase.data import Data
+from singlecase.effectsize import pnd, nap
 
-# Calculate PND
-pnd_values = pnd(data, dvars='dependent_var1', pvar='phase_var')
+# Create a sample data
+data_dict = {
+    'dvar1': [1.0, 2.5, 3.2, 4.6, 2.8, 5.6, 3.7, 4.2, 5.5, 6.2, 7.3, 8.5],
+    'dvar2': [2.5, 3.2, 4.6, 5.1, 4.8, 5.2, 6.7, 5.6, 6.2, 7.8, 8.4, 7.2],
+    'phase': ['A', 'A', 'A', 'A', 'A', 'A', 'B', 'B', 'B', 'B', 'B', 'B']
+}
+
+df = pd.DataFrame(data_dict)
 
-# Perform permutation test
-p_values = permutation_test(data, dvars='dependent_var1', pvar='phase_var')
+# Instantiate Data object
+data = Data(df)
 
-# Print the results
-print("NAP Values:")
-print(nap_values)
+# Set phase variable
+data.pvar = 'phase'
 
-print("PND Values:")
-print(pnd_values)
+# Calculate PND
+pnd_values = pnd(data)
+print(f"PND values: \n{pnd_values}")
 
-print("P-Values:")
-print(p_values)
+# Calculate NAP
+nap_values = nap(data)
+print(f"NAP values: \n{nap_values}")
 ```
 
+
 ## License
 
 This project is licensed under the BSD 3-clause license - see the [LICENSE](LICENSE) file for details.
 
 ## Acknowledgments
 
 - The Single Case Research package is being developed by Casper Wilstrup.
```

