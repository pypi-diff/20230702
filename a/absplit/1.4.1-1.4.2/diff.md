# Comparing `tmp/absplit-1.4.1.tar.gz` & `tmp/absplit-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "absplit-1.4.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "absplit-1.4.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `absplit-1.4.1.tar` & `absplit-1.4.2.tar`

### file list

```diff
@@ -1,22 +1,23 @@
--rw-r--r--   0        0        0     4958 2023-06-05 23:23:06.124000 absplit-1.4.1/.gitignore
--rw-r--r--   0        0        0       50 2023-02-18 09:46:26.039000 absplit-1.4.1/.idea/.gitignore
--rw-r--r--   0        0        0      291 2023-06-12 08:40:13.087000 absplit-1.4.1/.idea/genetic_algorithm.iml
--rw-r--r--   0        0        0      179 2023-02-18 09:46:26.072000 absplit-1.4.1/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0      303 2023-06-12 08:40:13.168000 absplit-1.4.1/.idea/misc.xml
--rw-r--r--   0        0        0      293 2023-02-18 09:46:26.093000 absplit-1.4.1/.idea/modules.xml
--rw-r--r--   0        0        0      185 2023-02-18 09:46:26.104000 absplit-1.4.1/.idea/vcs.xml
--rw-r--r--   0        0        0     1026 2023-02-18 09:46:26.114000 absplit-1.4.1/LICENSE
--rw-r--r--   0        0        0      152 2023-02-18 09:46:26.124000 absplit-1.4.1/MANIFEST.in
--rw-r--r--   0        0        0     8252 2023-07-02 10:26:33.912000 absplit-1.4.1/README.md
--rw-r--r--   0        0        0       93 2023-07-02 10:26:33.957000 absplit-1.4.1/absplit/__init__.py
--rw-r--r--   0        0        0     8992 2023-07-02 10:01:16.253000 absplit-1.4.1/absplit/data.py
--rw-r--r--   0        0        0    30025 2023-07-02 10:24:16.883000 absplit-1.4.1/absplit/ga.py
--rw-r--r--   0        0        0     1866 2023-02-18 09:46:26.177000 absplit-1.4.1/absplit/param.py
--rw-r--r--   0        0        0     3978 2023-06-18 23:28:12.372000 absplit-1.4.1/absplit/tutorials.py
--rw-r--r--   0        0        0    29186 2023-02-18 09:46:26.190000 absplit-1.4.1/images/logo.jpeg
--rw-r--r--   0        0        0     1533 2023-07-02 10:26:33.999000 absplit-1.4.1/pyproject.toml
--rw-r--r--   0        0        0       50 2023-06-05 23:23:06.260000 absplit-1.4.1/requirements.txt
--rw-r--r--   0        0        0        0 2023-02-18 09:46:26.220000 absplit-1.4.1/tests/__init__.py
--rw-r--r--   0        0        0     5925 2023-02-18 09:46:26.238000 absplit-1.4.1/tests/test_data.py
--rw-r--r--   0        0        0     2125 2023-06-12 08:32:24.989000 absplit-1.4.1/tests/test_ga.py
--rw-r--r--   0        0        0     9285 1970-01-01 00:00:00.000000 absplit-1.4.1/PKG-INFO
+-rw-r--r--   0        0        0     4976 2023-07-02 18:57:33.878000 absplit-1.4.2/.gitignore
+-rw-r--r--   0        0        0       50 2023-02-18 09:46:26.039000 absplit-1.4.2/.idea/.gitignore
+-rw-r--r--   0        0        0      291 2023-06-12 08:40:13.087000 absplit-1.4.2/.idea/genetic_algorithm.iml
+-rw-r--r--   0        0        0      179 2023-02-18 09:46:26.072000 absplit-1.4.2/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0      303 2023-06-12 08:40:13.168000 absplit-1.4.2/.idea/misc.xml
+-rw-r--r--   0        0        0      293 2023-02-18 09:46:26.093000 absplit-1.4.2/.idea/modules.xml
+-rw-r--r--   0        0        0      185 2023-02-18 09:46:26.104000 absplit-1.4.2/.idea/vcs.xml
+-rw-r--r--   0        0        0     1026 2023-02-18 09:46:26.114000 absplit-1.4.2/LICENSE
+-rw-r--r--   0        0        0      152 2023-02-18 09:46:26.124000 absplit-1.4.2/MANIFEST.in
+-rw-r--r--   0        0        0     8437 2023-07-02 21:46:40.246000 absplit-1.4.2/README.md
+-rw-r--r--   0        0        0       93 2023-07-02 21:40:38.790000 absplit-1.4.2/absplit/__init__.py
+-rw-r--r--   0        0        0    14169 2023-07-02 21:37:04.782000 absplit-1.4.2/absplit/data.py
+-rw-r--r--   0        0        0    30539 2023-07-02 21:18:26.583000 absplit-1.4.2/absplit/ga.py
+-rw-r--r--   0        0        0      948 2023-07-02 21:08:06.736000 absplit-1.4.2/absplit/log.py
+-rw-r--r--   0        0        0     1866 2023-02-18 09:46:26.177000 absplit-1.4.2/absplit/param.py
+-rw-r--r--   0        0        0     4985 2023-07-02 19:20:22.297000 absplit-1.4.2/absplit/tutorials.py
+-rw-r--r--   0        0        0    29186 2023-02-18 09:46:26.190000 absplit-1.4.2/images/logo.jpeg
+-rw-r--r--   0        0        0     1533 2023-07-02 21:40:38.839000 absplit-1.4.2/pyproject.toml
+-rw-r--r--   0        0        0       50 2023-06-05 23:23:06.260000 absplit-1.4.2/requirements.txt
+-rw-r--r--   0        0        0        0 2023-02-18 09:46:26.220000 absplit-1.4.2/tests/__init__.py
+-rw-r--r--   0        0        0     6678 2023-07-02 21:38:57.605000 absplit-1.4.2/tests/test_data.py
+-rw-r--r--   0        0        0     5332 2023-07-02 21:01:43.528000 absplit-1.4.2/tests/test_ga.py
+-rw-r--r--   0        0        0     9467 1970-01-01 00:00:00.000000 absplit-1.4.2/PKG-INFO
```

### Comparing `absplit-1.4.1/.gitignore` & `absplit-1.4.2/.gitignore`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 archive/
 data/
 notebooks/
 .pypirc
 notes.txt
+absplit/log_flag
 
 # Byte-compiled / optimized / DLL files
 __pycache__/
 *.py[cod]
 *$py.class
 
 # C extensions
```

### Comparing `absplit-1.4.1/LICENSE` & `absplit-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `absplit-1.4.1/README.md` & `absplit-1.4.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 <div align="center">
 <img src="https://raw.githubusercontent.com/cormac-rynne/absplit/main/images/logo.jpeg" width="460" height="140">
 <h3><strong>ABSplit</strong></h3>
 Split your data into matching A/B/n groups
 
 ![license](https://img.shields.io/badge/License-MIT-blue.svg)
-![version](https://img.shields.io/badge/version-1.4.1-blue.svg)
+![version](https://img.shields.io/badge/version-1.4.2-blue.svg)
 ![version](https://img.shields.io/badge/python-3-orange.svg)
 
 </div>
 
 <details open>
   <summary>Table of Contents</summary>
   <ol>
@@ -150,20 +150,23 @@
 [here](https://pygad.readthedocs.io/en/latest/README_pygad_ReadTheDocs.html#pygad-ga-class) for arguments you can pass
 (default: `{}`)
 * `splits` (list, optional): How many groups to split into, and relative size of the groups (default: `[0.5, 0.5]`,
 2 groups of equal size)
 * `size_penalty` (float, optional): Penalty weighting for differences in the population count between groups 
 (default: `0`)
 * `sum_penalty` (float, optional): Penalty weighting for the sum of metrics over time. If this is greater than zero,
-it will add a penalty to the cost function that will try and make the sum of each metric the same for each group.
+it will add a penalty to the cost function that will try and make the sum of each metric the same for each group 
+(default: `0`)
 * `cutoff_date` (str, optional): Cutoff date between fitting and validation data. For example, if you have data between 
 2023-01-01 and 2023-03-01, and the cutoff date is 2023-02-01, the algorithm will only perform the fit on data between 
 2023-01-01 and 2023-02-01. If `None`, it will fit on all available data. If cutoff date is provided, RMSE scores
   (gotten by using the `ab.rmse` attribute) will only be for validation period (i.e., from 2023-02-01 to end of 
 timeseries)
+* `missing_dates` (str, optional): How to deal with missing dates in time series data, options: `['drop_dates',
+'drop_population', '0', 'median']` (default: `median`)
 * `metric_weights` (dict, optional): Weights for each metric in the data. If you want the splitting to focus on 
 one metrics more than the other, you can prioritise this here (default: `{}`)
 
 
 ### Match 
 `Match(population, sample, metrics, splitting, date_col=None, ga_params={}, metric_weights={})`
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
 [https://raw.githubusercontent.com/cormac-rynne/absplit/main/images/logo.jpeg]
                                **** ABSplit ****
  Split your data into matching A/B/n groups ![license](https://img.shields.io/
  badge/License-MIT-blue.svg) ![version](https://img.shields.io/badge/version-
- 1.4.1-blue.svg) ![version](https://img.shields.io/badge/python-3-orange.svg)
+ 1.4.2-blue.svg) ![version](https://img.shields.io/badge/python-3-orange.svg)
  Table of Contents
    1. About_The_Project
    2. Getting_Started
           o Installation
    3. Tutorials
           o Do_it_yourself
    4. Usage
@@ -69,35 +69,37 @@
 pygad.readthedocs.io/en/latest/README_pygad_ReadTheDocs.html#pygad-ga-class)
 for arguments you can pass (default: `{}`) * `splits` (list, optional): How
 many groups to split into, and relative size of the groups (default: `[0.5,
 0.5]`, 2 groups of equal size) * `size_penalty` (float, optional): Penalty
 weighting for differences in the population count between groups (default: `0`)
 * `sum_penalty` (float, optional): Penalty weighting for the sum of metrics
 over time. If this is greater than zero, it will add a penalty to the cost
-function that will try and make the sum of each metric the same for each group.
-* `cutoff_date` (str, optional): Cutoff date between fitting and validation
-data. For example, if you have data between 2023-01-01 and 2023-03-01, and the
-cutoff date is 2023-02-01, the algorithm will only perform the fit on data
-between 2023-01-01 and 2023-02-01. If `None`, it will fit on all available
-data. If cutoff date is provided, RMSE scores (gotten by using the `ab.rmse`
-attribute) will only be for validation period (i.e., from 2023-02-01 to end of
-timeseries) * `metric_weights` (dict, optional): Weights for each metric in the
-data. If you want the splitting to focus on one metrics more than the other,
-you can prioritise this here (default: `{}`) ### Match `Match(population,
-sample, metrics, splitting, date_col=None, ga_params={}, metric_weights={})`
-Takes DataFrame `sample` and finds a comparable group in `population`.
-Arguments: * `population` (pd.DataFrame): Population to search for comparable
-group (**Must exclude sample data**) * `sample` (pd.DataFrame): Sample we are
-looking to find a match for. * `metrics` (str, list): Name of, or list of names
-of, metric columns in DataFrame * `splitting` (str): Name of column that
-represents individuals in the population that is getting split * `date_col`
-(str, optional): Name of column that represents time periods, if applicable. If
-left empty, it will perform a static split, i.e. not across timeseries,
-(default `None`) * `ga_params` (dict, optional): Parameters for the genetic
-algorithm `pygad.GA` module parameters, see [here](https://
+function that will try and make the sum of each metric the same for each group
+(default: `0`) * `cutoff_date` (str, optional): Cutoff date between fitting and
+validation data. For example, if you have data between 2023-01-01 and 2023-03-
+01, and the cutoff date is 2023-02-01, the algorithm will only perform the fit
+on data between 2023-01-01 and 2023-02-01. If `None`, it will fit on all
+available data. If cutoff date is provided, RMSE scores (gotten by using the
+`ab.rmse` attribute) will only be for validation period (i.e., from 2023-02-01
+to end of timeseries) * `missing_dates` (str, optional): How to deal with
+missing dates in time series data, options: `['drop_dates', 'drop_population',
+'0', 'median']` (default: `median`) * `metric_weights` (dict, optional):
+Weights for each metric in the data. If you want the splitting to focus on one
+metrics more than the other, you can prioritise this here (default: `{}`) ###
+Match `Match(population, sample, metrics, splitting, date_col=None, ga_params=
+{}, metric_weights={})` Takes DataFrame `sample` and finds a comparable group
+in `population`. Arguments: * `population` (pd.DataFrame): Population to search
+for comparable group (**Must exclude sample data**) * `sample` (pd.DataFrame):
+Sample we are looking to find a match for. * `metrics` (str, list): Name of, or
+list of names of, metric columns in DataFrame * `splitting` (str): Name of
+column that represents individuals in the population that is getting split *
+`date_col` (str, optional): Name of column that represents time periods, if
+applicable. If left empty, it will perform a static split, i.e. not across
+timeseries, (default `None`) * `ga_params` (dict, optional): Parameters for the
+genetic algorithm `pygad.GA` module parameters, see [here](https://
 pygad.readthedocs.io/en/latest/README_pygad_ReadTheDocs.html#pygad-ga-class)
 for arguments you can pass (default: `{}`) * `splits` (list, optional): How
 many groups to split into, and relative size of the groups (default: `[0.5,
 0.5]`, 2 groups of equal size) * `metric_weights` (dict, optional): Weights for
 each metric in the data. If you want the splitting to focus on one metrics more
 than the other, you can prioritise this here (default: `{}`)
                                                                   (back_to_top)
```

### Comparing `absplit-1.4.1/absplit/ga.py` & `absplit-1.4.2/absplit/ga.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,20 @@
-from absplit.param import ParamMixin
-from absplit.data import Data
 from abc import ABC, abstractmethod
 import pandas as pd
 import pygad
-import logging
 import numpy as np
 import matplotlib.pyplot as plt
 import seaborn as sns
 from sklearn import preprocessing
 from itertools import combinations
+from absplit.param import ParamMixin
+from absplit.data import Data
+from absplit import log
 
-
-logger = logging.getLogger(__name__)
+logger = log.get_logger(__name__)
 
 
 class GAInstance:
     """Manages initialisation and running of pygad genetic algorithm instance
 
     Attributes:
         num_genes (int): Number of members in the population that is being searched
@@ -160,15 +159,15 @@
         _cost_weighting(): Modifies cost weighting array
         run(): Runs the genetic algorithm
         fitness(): Plot generation fitness graph
         visualise(): Plots metrics using results from genetic algorithm output
     """
 
     def __init__(self, ga_params={}, metric_weights={}, runs=1, splits=[0.5, 0.5], size_penalty=0, sum_penalty=0,
-                 cutoff_date=None, **kwargs):
+                 cutoff_date=None, missing_dates='median', **kwargs):
         """Initializes the class and sets the attributes
 
         Args:
             ga_params (dict, optional): Genetic algorithm parameters to add/modify
             metric_weights (dict, optional): Cost weightings to apply to metrics
             runs (int, optional): How many runs to try
             **kwargs: Additional keyword arguments
@@ -186,24 +185,25 @@
         self._runs = runs
         self._splits = splits
         self._splits_num = len(self._splits)
         self._ga_params = GAParams(splits=splits, **ga_params)
         self._best_score = -1
         self._metric_weights = metric_weights
         self._cutoff_date = cutoff_date
+        self._missing_dates = missing_dates
         self._df = None
         self._population = None
         self._df_result = None  # Final results dataframe
-        self._df_dist = None  # Group count distribution
-        self._df_agg = None  # Group aggregated data
+        self._df_dist = None    # Group count distribution
+        self._df_agg = None     # Group aggregated data
         self._df_totals = None  # Group metrics, summed over time
-        self._df_mape = None  # MAPE between groups
-        self._ga = None  # Genetic algorithm instance
-        self._df_vis = None  # Visualisation dataframe
-        self._df_rmse = None  # RMSE between groups
+        self._df_mape = None    # MAPE between groups
+        self._ga = None         # Genetic algorithm instance
+        self._df_vis = None     # Visualisation dataframe
+        self._df_rmse = None    # RMSE between groups
         self._best_ga = None
         self._solution = None
 
         self._cost_weighting()
 
     def _cost_weighting(self):
         """Set relative cost weights for each metric. Defaults to 1 unless specified.
@@ -233,18 +233,20 @@
 
         Returns:
             None
         """
 
         global all_metrics_global
         global splits_global
+        global scaled_mean_global
+        all_metrics_global = self._population.matrix
         splits_global = (np.array(self._splits).sum() / np.array(self._splits))
+        scaled_mean_global = np.mean(all_metrics_global) * all_metrics_global.shape[0] * all_metrics_global.shape[2]
 
         logger.debug('Splitting..')
-        all_metrics_global = self._population.matrix
 
         # Run multiple times, save the best solution
         for i in range(self._runs):
             if self._runs > 1:
                 print(f'[Run {i+1}]')
 
             # Initialise and run GA, get solution
@@ -321,14 +323,17 @@
         # If cutoff, use post cut off period for rmse
         if self.date_col and self._cutoff_date:
             df_agg.loc[df_agg[self.date_col] <= self._cutoff_date, 'period'] = 'pre-cutoff'
             df_agg.loc[df_agg[self.date_col] > self._cutoff_date, 'period'] = 'post-cutoff'
             df_total2 = df_agg.groupby(['period', 'bin'])[self.metrics].sum()
             df_total = pd.concat([df_total, df_total2], axis=0)
 
+        pct_cols = [f'{x}_pct' for x in self.metrics]
+        df_total[pct_cols] = df_total[self.metrics] / df_total.groupby('period')[self.metrics].transform('sum')
+
         self._df_totals = df_total
 
     def _build_score(self, function):
         """Scores each group, for each metric, based on the fuction passed.
 
         If cutoff_date is passed in class init, scores are only for the post-cutoff period.
 
@@ -739,14 +744,15 @@
 
     global all_metrics_global     # 3d matrix of metric values (metrics, population, dates)
     global metric_weights_global  # Relative weights for each metric
     global splits_global          # Proportional splits for each group
     global size_penalty_global    # Float weight for size penalty
     global sum_penalty_global     # Float weight for sum penalty
     global group_ids_global       # Array of group IDs
+    global scaled_mean_global     # Mean metric value, scaled by number of data
 
     # Generate binary array, 1 row of 0s and 1s for each group (where solution == 1/2/3 etc)
     groups = (solution == group_ids_global[:, None]).astype(int)
 
     # == Size penalty == #
     # Calculate all_metrics mean * number of days * number of metrics
     mean = np.mean(all_metrics_global) * all_metrics_global.shape[0] * all_metrics_global.shape[2]
@@ -757,15 +763,15 @@
 
     # == MSE == #
     costs = (groups @ all_metrics_global) * splits_global.reshape((1, -1, 1)) * metric_weights_global
     diffs = np.roll(costs, -1, axis=1) - costs
     mse = ((diffs ** 2).mean(axis=1)).sum()
 
     # == Sum penalty == #
-    sum_cost = (np.abs(costs.sum(2) - np.roll(costs.sum(2), shift=-1, axis=1)).sum() * sum_penalty_global) / (4*len(splits_global)) ** 1.2
+    sum_cost = (np.abs((costs.sum(2) - np.roll(costs.sum(2), shift=-1, axis=1)) * splits_global).sum() * sum_penalty_global) / (4*len(splits_global)) ** 1.2
 
     # Fitness
     total = mse + size_cost + sum_cost
     fitness = 1.0 / np.abs(total + 1e-5)  # Add small sum to prevent divide by zero
     return fitness
```

### Comparing `absplit-1.4.1/absplit/param.py` & `absplit-1.4.2/absplit/param.py`

 * *Files identical despite different names*

### Comparing `absplit-1.4.1/absplit/tutorials.py` & `absplit-1.4.2/absplit/tutorials.py`

 * *Files 17% similar despite different names*

```diff
@@ -76,14 +76,39 @@
     cols = cols + ['fips'] if not drop_fips else cols
     df = df.set_index(cols).sort_index()
     df = df.groupby(level=[0, 1]).diff().fillna(0).clip(lower=0)
     resampler = lambda x: x.set_index('date').resample('w').sum()
     df = df.reset_index(level=2).groupby([x for x in cols if x != 'date']).apply(resampler).reset_index()
     return df
 
+def retail(test=False):
+    url = 'https://raw.githubusercontent.com/nytimes/covid-19-data/master/us-counties.csv'
+    if test:
+        url = '../data/online-retail.csv'
+        print(f'TEST mode, pulling file')
+    else:
+        print(f'Pulling data from {url}')
+    df = pd.read_csv(url)
+    print(f'Cleaning and resampling data..')
+
+    df.columns = [x.lower().replace(' ', '_') for x in df.columns]
+    df.loc[:, 'invoicedate'] = pd.to_datetime(df['invoicedate'])
+    df['date'] = df['invoicedate'].dt.date
+    df['week'] = df['invoicedate'].dt.to_period('W').dt.start_time
+    df['cost'] = df['quantity'] * df['price']
+    df = df[~df['customer_id'].isna()].reset_index(drop=True)
+    df['customer_id'] = df['customer_id'].astype('int64').astype(str)
+
+    agg_dct = {
+        'cost': 'sum',
+        'quantity': 'sum',
+        'stockcode': pd.Series.nunique
+    }
+    df2 = df.groupby(['week', 'customer_id']).agg(agg_dct).reset_index().drop('stockcode', axis=1)
+    return df2
 
 def display(df):
     for i in range(5):
         df_ = df[df['id'] == i]
         plt.plot(df_['date'].values, df_['metric1'].values, label=f'id: {i}')
 
     plt.xticks(rotation=45)
```

### Comparing `absplit-1.4.1/images/logo.jpeg` & `absplit-1.4.2/images/logo.jpeg`

 * *Files identical despite different names*

### Comparing `absplit-1.4.1/pyproject.toml` & `absplit-1.4.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "absplit"
-version = "1.4.1"
+version = "1.4.2"
 description = "Generates A/B/n test groups"
 readme = "README.md"
 authors = [{name = "Cormac Rynne", email = "cormac.ry@gmail.com"}]
 license = {file = "LICENSE"}
 repository = "https://github.com/cormac-rynne/absplit"
 requires-python = "<=3.11"
 classifiers = [
```

### Comparing `absplit-1.4.1/PKG-INFO` & `absplit-1.4.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: absplit
-Version: 1.4.1
+Version: 1.4.2
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
-![version](https://img.shields.io/badge/version-1.4.1-blue.svg)
+![version](https://img.shields.io/badge/version-1.4.2-blue.svg)
 ![version](https://img.shields.io/badge/python-3-orange.svg)
 
 </div>
 
 <details open>
   <summary>Table of Contents</summary>
   <ol>
@@ -179,20 +179,23 @@
 [here](https://pygad.readthedocs.io/en/latest/README_pygad_ReadTheDocs.html#pygad-ga-class) for arguments you can pass
 (default: `{}`)
 * `splits` (list, optional): How many groups to split into, and relative size of the groups (default: `[0.5, 0.5]`,
 2 groups of equal size)
 * `size_penalty` (float, optional): Penalty weighting for differences in the population count between groups 
 (default: `0`)
 * `sum_penalty` (float, optional): Penalty weighting for the sum of metrics over time. If this is greater than zero,
-it will add a penalty to the cost function that will try and make the sum of each metric the same for each group.
+it will add a penalty to the cost function that will try and make the sum of each metric the same for each group 
+(default: `0`)
 * `cutoff_date` (str, optional): Cutoff date between fitting and validation data. For example, if you have data between 
 2023-01-01 and 2023-03-01, and the cutoff date is 2023-02-01, the algorithm will only perform the fit on data between 
 2023-01-01 and 2023-02-01. If `None`, it will fit on all available data. If cutoff date is provided, RMSE scores
   (gotten by using the `ab.rmse` attribute) will only be for validation period (i.e., from 2023-02-01 to end of 
 timeseries)
+* `missing_dates` (str, optional): How to deal with missing dates in time series data, options: `['drop_dates',
+'drop_population', '0', 'median']` (default: `median`)
 * `metric_weights` (dict, optional): Weights for each metric in the data. If you want the splitting to focus on 
 one metrics more than the other, you can prioritise this here (default: `{}`)
 
 
 ### Match 
 `Match(population, sample, metrics, splitting, date_col=None, ga_params={}, metric_weights={})`
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: absplit Version: 1.4.1 Summary: Generates A/B/
+Metadata-Version: 2.1 Name: absplit Version: 1.4.2 Summary: Generates A/B/
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
- 1.4.1-blue.svg) ![version](https://img.shields.io/badge/python-3-orange.svg)
+ 1.4.2-blue.svg) ![version](https://img.shields.io/badge/python-3-orange.svg)
  Table of Contents
    1. About_The_Project
    2. Getting_Started
           o Installation
    3. Tutorials
           o Do_it_yourself
    4. Usage
@@ -86,35 +86,37 @@
 pygad.readthedocs.io/en/latest/README_pygad_ReadTheDocs.html#pygad-ga-class)
 for arguments you can pass (default: `{}`) * `splits` (list, optional): How
 many groups to split into, and relative size of the groups (default: `[0.5,
 0.5]`, 2 groups of equal size) * `size_penalty` (float, optional): Penalty
 weighting for differences in the population count between groups (default: `0`)
 * `sum_penalty` (float, optional): Penalty weighting for the sum of metrics
 over time. If this is greater than zero, it will add a penalty to the cost
-function that will try and make the sum of each metric the same for each group.
-* `cutoff_date` (str, optional): Cutoff date between fitting and validation
-data. For example, if you have data between 2023-01-01 and 2023-03-01, and the
-cutoff date is 2023-02-01, the algorithm will only perform the fit on data
-between 2023-01-01 and 2023-02-01. If `None`, it will fit on all available
-data. If cutoff date is provided, RMSE scores (gotten by using the `ab.rmse`
-attribute) will only be for validation period (i.e., from 2023-02-01 to end of
-timeseries) * `metric_weights` (dict, optional): Weights for each metric in the
-data. If you want the splitting to focus on one metrics more than the other,
-you can prioritise this here (default: `{}`) ### Match `Match(population,
-sample, metrics, splitting, date_col=None, ga_params={}, metric_weights={})`
-Takes DataFrame `sample` and finds a comparable group in `population`.
-Arguments: * `population` (pd.DataFrame): Population to search for comparable
-group (**Must exclude sample data**) * `sample` (pd.DataFrame): Sample we are
-looking to find a match for. * `metrics` (str, list): Name of, or list of names
-of, metric columns in DataFrame * `splitting` (str): Name of column that
-represents individuals in the population that is getting split * `date_col`
-(str, optional): Name of column that represents time periods, if applicable. If
-left empty, it will perform a static split, i.e. not across timeseries,
-(default `None`) * `ga_params` (dict, optional): Parameters for the genetic
-algorithm `pygad.GA` module parameters, see [here](https://
+function that will try and make the sum of each metric the same for each group
+(default: `0`) * `cutoff_date` (str, optional): Cutoff date between fitting and
+validation data. For example, if you have data between 2023-01-01 and 2023-03-
+01, and the cutoff date is 2023-02-01, the algorithm will only perform the fit
+on data between 2023-01-01 and 2023-02-01. If `None`, it will fit on all
+available data. If cutoff date is provided, RMSE scores (gotten by using the
+`ab.rmse` attribute) will only be for validation period (i.e., from 2023-02-01
+to end of timeseries) * `missing_dates` (str, optional): How to deal with
+missing dates in time series data, options: `['drop_dates', 'drop_population',
+'0', 'median']` (default: `median`) * `metric_weights` (dict, optional):
+Weights for each metric in the data. If you want the splitting to focus on one
+metrics more than the other, you can prioritise this here (default: `{}`) ###
+Match `Match(population, sample, metrics, splitting, date_col=None, ga_params=
+{}, metric_weights={})` Takes DataFrame `sample` and finds a comparable group
+in `population`. Arguments: * `population` (pd.DataFrame): Population to search
+for comparable group (**Must exclude sample data**) * `sample` (pd.DataFrame):
+Sample we are looking to find a match for. * `metrics` (str, list): Name of, or
+list of names of, metric columns in DataFrame * `splitting` (str): Name of
+column that represents individuals in the population that is getting split *
+`date_col` (str, optional): Name of column that represents time periods, if
+applicable. If left empty, it will perform a static split, i.e. not across
+timeseries, (default `None`) * `ga_params` (dict, optional): Parameters for the
+genetic algorithm `pygad.GA` module parameters, see [here](https://
 pygad.readthedocs.io/en/latest/README_pygad_ReadTheDocs.html#pygad-ga-class)
 for arguments you can pass (default: `{}`) * `splits` (list, optional): How
 many groups to split into, and relative size of the groups (default: `[0.5,
 0.5]`, 2 groups of equal size) * `metric_weights` (dict, optional): Weights for
 each metric in the data. If you want the splitting to focus on one metrics more
 than the other, you can prioritise this here (default: `{}`)
                                                                   (back_to_top)
```

