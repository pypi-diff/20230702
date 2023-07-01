# Comparing `tmp/absplit-1.3.1.tar.gz` & `tmp/absplit-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "absplit-1.3.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "absplit-1.4.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `absplit-1.3.1.tar` & `absplit-1.4.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     4958 2023-06-05 23:23:06.124000 absplit-1.3.1/.gitignore
--rw-r--r--   0        0        0       50 2023-02-18 09:46:26.039000 absplit-1.3.1/.idea/.gitignore
--rw-r--r--   0        0        0      291 2023-06-12 08:40:13.087000 absplit-1.3.1/.idea/genetic_algorithm.iml
--rw-r--r--   0        0        0      179 2023-02-18 09:46:26.072000 absplit-1.3.1/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0      303 2023-06-12 08:40:13.168000 absplit-1.3.1/.idea/misc.xml
--rw-r--r--   0        0        0      293 2023-02-18 09:46:26.093000 absplit-1.3.1/.idea/modules.xml
--rw-r--r--   0        0        0      185 2023-02-18 09:46:26.104000 absplit-1.3.1/.idea/vcs.xml
--rw-r--r--   0        0        0     1026 2023-02-18 09:46:26.114000 absplit-1.3.1/LICENSE
--rw-r--r--   0        0        0      152 2023-02-18 09:46:26.124000 absplit-1.3.1/MANIFEST.in
--rw-r--r--   0        0        0     7816 2023-06-18 23:24:24.991000 absplit-1.3.1/README.md
--rw-r--r--   0        0        0       93 2023-06-18 23:24:25.025000 absplit-1.3.1/absplit/__init__.py
--rw-r--r--   0        0        0     8940 2023-06-14 19:51:59.610000 absplit-1.3.1/absplit/data.py
--rw-r--r--   0        0        0    25425 2023-06-18 23:15:55.977000 absplit-1.3.1/absplit/ga.py
--rw-r--r--   0        0        0     1866 2023-02-18 09:46:26.177000 absplit-1.3.1/absplit/param.py
--rw-r--r--   0        0        0     3995 2023-06-18 23:23:52.087000 absplit-1.3.1/absplit/tutorials.py
--rw-r--r--   0        0        0    29186 2023-02-18 09:46:26.190000 absplit-1.3.1/images/logo.jpeg
--rw-r--r--   0        0        0     1531 2023-06-18 23:24:24.953000 absplit-1.3.1/pyproject.toml
--rw-r--r--   0        0        0       50 2023-06-05 23:23:06.260000 absplit-1.3.1/requirements.txt
--rw-r--r--   0        0        0        0 2023-02-18 09:46:26.220000 absplit-1.3.1/tests/__init__.py
--rw-r--r--   0        0        0     5925 2023-02-18 09:46:26.238000 absplit-1.3.1/tests/test_data.py
--rw-r--r--   0        0        0     2125 2023-06-12 08:32:24.989000 absplit-1.3.1/tests/test_ga.py
--rw-r--r--   0        0        0     8850 1970-01-01 00:00:00.000000 absplit-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0     4958 2023-06-05 23:23:06.124000 absplit-1.4.0/.gitignore
+-rw-r--r--   0        0        0       50 2023-02-18 09:46:26.039000 absplit-1.4.0/.idea/.gitignore
+-rw-r--r--   0        0        0      291 2023-06-12 08:40:13.087000 absplit-1.4.0/.idea/genetic_algorithm.iml
+-rw-r--r--   0        0        0      179 2023-02-18 09:46:26.072000 absplit-1.4.0/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0      303 2023-06-12 08:40:13.168000 absplit-1.4.0/.idea/misc.xml
+-rw-r--r--   0        0        0      293 2023-02-18 09:46:26.093000 absplit-1.4.0/.idea/modules.xml
+-rw-r--r--   0        0        0      185 2023-02-18 09:46:26.104000 absplit-1.4.0/.idea/vcs.xml
+-rw-r--r--   0        0        0     1026 2023-02-18 09:46:26.114000 absplit-1.4.0/LICENSE
+-rw-r--r--   0        0        0      152 2023-02-18 09:46:26.124000 absplit-1.4.0/MANIFEST.in
+-rw-r--r--   0        0        0     8252 2023-07-01 22:51:51.997000 absplit-1.4.0/README.md
+-rw-r--r--   0        0        0       93 2023-07-01 22:51:52.048000 absplit-1.4.0/absplit/__init__.py
+-rw-r--r--   0        0        0     8992 2023-07-01 22:59:45.945000 absplit-1.4.0/absplit/data.py
+-rw-r--r--   0        0        0    29970 2023-07-01 22:54:24.935000 absplit-1.4.0/absplit/ga.py
+-rw-r--r--   0        0        0     1866 2023-02-18 09:46:26.177000 absplit-1.4.0/absplit/param.py
+-rw-r--r--   0        0        0     3978 2023-06-18 23:28:12.372000 absplit-1.4.0/absplit/tutorials.py
+-rw-r--r--   0        0        0    29186 2023-02-18 09:46:26.190000 absplit-1.4.0/images/logo.jpeg
+-rw-r--r--   0        0        0     1533 2023-07-01 22:51:52.089000 absplit-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0       50 2023-06-05 23:23:06.260000 absplit-1.4.0/requirements.txt
+-rw-r--r--   0        0        0        0 2023-02-18 09:46:26.220000 absplit-1.4.0/tests/__init__.py
+-rw-r--r--   0        0        0     5925 2023-02-18 09:46:26.238000 absplit-1.4.0/tests/test_data.py
+-rw-r--r--   0        0        0     2125 2023-06-12 08:32:24.989000 absplit-1.4.0/tests/test_ga.py
+-rw-r--r--   0        0        0     9285 1970-01-01 00:00:00.000000 absplit-1.4.0/PKG-INFO
```

### Comparing `absplit-1.3.1/.gitignore` & `absplit-1.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `absplit-1.3.1/LICENSE` & `absplit-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `absplit-1.3.1/README.md` & `absplit-1.4.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 <div align="center">
 <img src="https://raw.githubusercontent.com/cormac-rynne/absplit/main/images/logo.jpeg" width="460" height="140">
 <h3><strong>ABSplit</strong></h3>
 Split your data into matching A/B/n groups
 
 ![license](https://img.shields.io/badge/License-MIT-blue.svg)
-![version](https://img.shields.io/badge/version-1.3.1-blue.svg)
+![version](https://img.shields.io/badge/version-1.4.0-blue.svg)
 ![version](https://img.shields.io/badge/python-3-orange.svg)
 
 </div>
 
 <details open>
   <summary>Table of Contents</summary>
   <ol>
@@ -117,22 +117,23 @@
 
 # Visualise data
 ab.visualise()
 
 # Extract bin splits
 df = ab.results
 
-# Extract distributions summary
-df_dist = ab.distributions
-
 # Extract data aggregated by bins
 df_agg = ab.aggregations
 
-# Extract RMSE summary
-df_rmse = ab.rmse
+# Extract summary statistics
+df_dist = ab.distributions    # Population counts between groups
+df_rmse = ab.rmse             # RMSE between groups for each metric
+df_mape = ab.mape             # MAPE between groups for each metric
+df_totals = ab.totals         # Total sum of each metric for each group
+
 ```
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 ## API Reference
 ### Absplit 
 `ABSplit(df, metrics, splitting, date_col=None, ga_params={}, metric_weights={}, splits=[0.5, 0.5], size_penalty=0)`
 
@@ -148,14 +149,16 @@
 * `ga_params` (dict, optional): Parameters for the genetic algorithm `pygad.GA` module parameters, see 
 [here](https://pygad.readthedocs.io/en/latest/README_pygad_ReadTheDocs.html#pygad-ga-class) for arguments you can pass
 (default: `{}`)
 * `splits` (list, optional): How many groups to split into, and relative size of the groups (default: `[0.5, 0.5]`,
 2 groups of equal size)
 * `size_penalty` (float, optional): Penalty weighting for differences in the population count between groups 
 (default: `0`)
+* `sum_penalty` (float, optional): Penalty weighting for the sum of metrics over time. If this is greater than zero,
+it will add a penalty to the cost function that will try and make the sum of each metric the same for each group.
 * `cutoff_date` (str, optional): Cutoff date between fitting and validation data. For example, if you have data between 
 2023-01-01 and 2023-03-01, and the cutoff date is 2023-02-01, the algorithm will only perform the fit on data between 
 2023-01-01 and 2023-02-01. If `None`, it will fit on all available data. If cutoff date is provided, RMSE scores
   (gotten by using the `ab.rmse` attribute) will only be for validation period (i.e., from 2023-02-01 to end of 
 timeseries)
 * `metric_weights` (dict, optional): Weights for each metric in the data. If you want the splitting to focus on 
 one metrics more than the other, you can prioritise this here (default: `{}`)
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
 [https://raw.githubusercontent.com/cormac-rynne/absplit/main/images/logo.jpeg]
                                **** ABSplit ****
  Split your data into matching A/B/n groups ![license](https://img.shields.io/
  badge/License-MIT-blue.svg) ![version](https://img.shields.io/badge/version-
- 1.3.1-blue.svg) ![version](https://img.shields.io/badge/python-3-orange.svg)
+ 1.4.0-blue.svg) ![version](https://img.shields.io/badge/python-3-orange.svg)
  Table of Contents
    1. About_The_Project
    2. Getting_Started
           o Installation
    3. Tutorials
           o Do_it_yourself
    4. Usage
@@ -44,17 +44,19 @@
 in ['a', 'b', 'c', 'd', 'e']] for item in sublist], 'metric1': np.arange(0, 15,
 1), 'metric2': np.arange(0, 150, 10) } df = pd.DataFrame(data_dct) # Identify
 which columns are metrics, which is the time period, and what to split on
 kwargs = { 'metrics': ['metric1', 'metric2'], 'date_col': 'date', 'splitting':
 'city' } # Initialise ab = ABSplit( df=df, split=[.5, .5], # Split into 2
 groups of equal size **kwargs, ) # Generate split ab.run() # Visualise
 generation fitness ab.fitness() # Visualise data ab.visualise() # Extract bin
-splits df = ab.results # Extract distributions summary df_dist =
-ab.distributions # Extract data aggregated by bins df_agg = ab.aggregations #
-Extract RMSE summary df_rmse = ab.rmse ```
+splits df = ab.results # Extract data aggregated by bins df_agg =
+ab.aggregations # Extract summary statistics df_dist = ab.distributions #
+Population counts between groups df_rmse = ab.rmse # RMSE between groups for
+each metric df_mape = ab.mape # MAPE between groups for each metric df_totals =
+ab.totals # Total sum of each metric for each group ```
                                                                   (back_to_top)
 ## API Reference ### Absplit `ABSplit(df, metrics, splitting, date_col=None,
 ga_params={}, metric_weights={}, splits=[0.5, 0.5], size_penalty=0)` Splits
 population into n groups. Mutually exclusive, completely exhaustive Arguments:
 * `df` (pd.DataFrame): Dataframe of population to be split * `metrics` (str,
 list): Name of, or list of names of, metric columns in DataFrame to be
 considered in split * `splitting` (str): Name of column that represents
@@ -65,14 +67,17 @@
 timeseries, (default `None`) * `ga_params` (dict, optional): Parameters for the
 genetic algorithm `pygad.GA` module parameters, see [here](https://
 pygad.readthedocs.io/en/latest/README_pygad_ReadTheDocs.html#pygad-ga-class)
 for arguments you can pass (default: `{}`) * `splits` (list, optional): How
 many groups to split into, and relative size of the groups (default: `[0.5,
 0.5]`, 2 groups of equal size) * `size_penalty` (float, optional): Penalty
 weighting for differences in the population count between groups (default: `0`)
+* `sum_penalty` (float, optional): Penalty weighting for the sum of metrics
+over time. If this is greater than zero, it will add a penalty to the cost
+function that will try and make the sum of each metric the same for each group.
 * `cutoff_date` (str, optional): Cutoff date between fitting and validation
 data. For example, if you have data between 2023-01-01 and 2023-03-01, and the
 cutoff date is 2023-02-01, the algorithm will only perform the fit on data
 between 2023-01-01 and 2023-02-01. If `None`, it will fit on all available
 data. If cutoff date is provided, RMSE scores (gotten by using the `ab.rmse`
 attribute) will only be for validation period (i.e., from 2023-02-01 to end of
 timeseries) * `metric_weights` (dict, optional): Weights for each metric in the
```

### Comparing `absplit-1.3.1/absplit/data.py` & `absplit-1.4.0/absplit/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -146,15 +146,16 @@
         """
         df_unstacked = self._df_unstacked
         if self.date_col and self._cutoff_date:
             df_unstacked = df_unstacked[
                 df_unstacked.index.get_level_values(self.date_col) <= pd.to_datetime(self._cutoff_date)
             ]
 
-        df_unstacked = df_unstacked.unstack(self.date_col, fill_value=0) if self.date_col \
+        # todo: feature to summarise missing data
+        df_unstacked = df_unstacked.unstack(self.date_col).dropna(axis=1) if self.date_col \
             else df_unstacked
         self._df_unstacked = df_unstacked
 
     def _scale(self):
         """Standardise all metrics so all metrics weighted as equally as possible
 
         Returns:
```

### Comparing `absplit-1.3.1/absplit/ga.py` & `absplit-1.4.0/absplit/ga.py`

 * *Files 12% similar despite different names*

```diff
@@ -121,15 +121,15 @@
             None
         """
 
         # Update if args passed
         if kwargs:
             for key, value in kwargs.items():
                 if key in self._dont_touch:
-                    print(f'Parameter \'{key}\' is essential to running the genetic algorithm as a'\
+                    print(f'Parameter \'{key}\' is essential to running the genetic algorithm as a '
                           f'discrete genetic algorith, and so you\'re not allowed to modify this')
                     continue
                 if callable(value) or key in self._silence:
                     print(f'[Updating] {key}')
                 else:
                     print(f'[Updating] {key} to {value}')
                 self.params[key] = value
@@ -159,29 +159,31 @@
     Methods:
         _cost_weighting(): Modifies cost weighting array
         run(): Runs the genetic algorithm
         fitness(): Plot generation fitness graph
         visualise(): Plots metrics using results from genetic algorithm output
     """
 
-    def __init__(self, ga_params={}, metric_weights={}, runs=1, splits=[0.5, 0.5], size_penalty=1, cutoff_date=None,
-                 **kwargs):
+    def __init__(self, ga_params={}, metric_weights={}, runs=1, splits=[0.5, 0.5], size_penalty=0, sum_penalty=0,
+                 cutoff_date=None, **kwargs):
         """Initializes the class and sets the attributes
 
         Args:
             ga_params (dict, optional): Genetic algorithm parameters to add/modify
             metric_weights (dict, optional): Cost weightings to apply to metrics
             runs (int, optional): How many runs to try
             **kwargs: Additional keyword arguments
         """
         super().__init__(**kwargs)
+        global sum_penalty_global
         global size_penalty_global
         global group_ids_global
         size_penalty_global = size_penalty
         group_ids_global = np.arange(0, len(splits))
+        sum_penalty_global = sum_penalty
 
         if ga_params:
             assert isinstance(ga_params, dict), 'ga_params must be a dictionary'
         self._runs = runs
         self._splits = splits
         self._splits_num = len(self._splits)
         self._ga_params = GAParams(splits=splits, **ga_params)
@@ -189,14 +191,16 @@
         self._metric_weights = metric_weights
         self._cutoff_date = cutoff_date
         self._df = None
         self._population = None
         self._df_result = None  # Final results dataframe
         self._df_dist = None  # Group count distribution
         self._df_agg = None  # Group aggregated data
+        self._df_totals = None  # Group metrics, summed over time
+        self._df_mape = None  # MAPE between groups
         self._ga = None  # Genetic algorithm instance
         self._df_vis = None  # Visualisation dataframe
         self._df_rmse = None  # RMSE between groups
         self._best_ga = None
         self._solution = None
 
         self._cost_weighting()
@@ -217,25 +221,27 @@
             for key, value in self._metric_weights.items():
                 try:
                     i = self.metrics.index(key)
                     metric_weights_global[i] = value
                     print(f'[Updating] {key} weight updated to {value}')
                 except ValueError:
                     print(f'Cant find metric name {key}, weight {value} not applied, defaulting to 1')
+        # Reshape to broadcast across metrics dimension of 3d array
+        metric_weights_global = metric_weights_global.reshape(-1, 1, 1)
 
     def run(self):
         """Runs genetic algorithm and returns bin splits into _df_result
 
         Returns:
             None
         """
 
         global all_metrics_global
         global splits_global
-        splits_global = np.array(self._splits).sum() / np.array(self._splits)
+        splits_global = (np.array(self._splits).sum() / np.array(self._splits)).reshape((1, -1, 1))
 
         logger.debug('Splitting..')
         all_metrics_global = self._population.matrix
 
         # Run multiple times, save the best solution
         for i in range(self._runs):
             if self._runs > 1:
@@ -263,15 +269,21 @@
         self._build_data()
         logger.debug('Split complete')
 
     def _build_data(self):
         self._build_distributions()
         self._build_df_vis()
         self._build_aggregation()
-        self._build_rmse()
+        self._build_totals()
+        self._df_mape = self._build_score(
+            function=lambda x, y: np.mean(np.abs(((x - y) / x)))
+        )
+        self._df_rmse = self._build_score(
+            function=lambda x, y: np.sqrt(((x - y) ** 2).mean())
+        )
 
     @abstractmethod
     def _build_df_vis(self):
         pass
 
     @abstractmethod
     def _post_run(self):
@@ -296,18 +308,36 @@
             _df_dist
         """
         self._df_dist = self._df_result['bin'].value_counts().to_frame('count')
         self._df_dist.index.name = 'bin'
         self._df_dist['pct'] = (self._df_dist['count'] / self._df_dist['count'].sum()).round(4)
         return self._df_dist.sort_index()
 
-    def _build_rmse(self):
-        """Scores the RMSE for each group, for each metric.
+    def _build_totals(self):
+        df_agg = self._df_agg.copy()
+
+        df_agg.loc[:, 'period'] = 'total'
+        df_total = df_agg.groupby(['period', 'bin'])[self.metrics].sum()
 
-        If cutoff_date is passed in class init, rmse scores are only for the post-cutoff period.
+        # If cutoff, use post cut off period for rmse
+        if self.date_col and self._cutoff_date:
+            df_agg.loc[df_agg[self.date_col] <= self._cutoff_date, 'period'] = 'pre-cutoff'
+            df_agg.loc[df_agg[self.date_col] > self._cutoff_date, 'period'] = 'post-cutoff'
+            df_total2 = df_agg.groupby(['period', 'bin'])[self.metrics].sum()
+            df_total = pd.concat([df_total, df_total2], axis=0)
+
+        self._df_totals = df_total
+
+    def _build_score(self, function):
+        """Scores each group, for each metric, based on the fuction passed.
+
+        If cutoff_date is passed in class init, scores are only for the post-cutoff period.
+
+        Args:
+            function (callable): Scoring function
 
         Sets:
             _df_rsme (pd.DataFrame): Datafame of RMSE scores for each group and metric
         """
         df_agg = self._df_agg.copy()
 
         if self.date_col is None:
@@ -315,64 +345,39 @@
 
         # If cutoff, use post cut off period for rmse
         if self.date_col and self._cutoff_date:
             df_agg = df_agg[
                 df_agg[self.date_col] > pd.to_datetime(self._cutoff_date)
             ]
 
+        # Pivot on bin groups
         df_ = df_agg.pivot(index=self.date_col, columns='bin', values=self.metrics)
+        # Flatten columns
         df_.columns = df_.columns.map('_'.join).str.lower()
-
         groups = self._df_agg['bin'].unique()
         combinations_lst = list(combinations(groups, 2))
 
         df_lst = []
-
         for metric in self.metrics:
             df_metric = pd.DataFrame()
             for a, b in combinations_lst:
-                col_a = f'{metric}_{a}'
-                col_b = f'{metric}_{b}'
-                rmse = np.sqrt(((df_[col_a] - df_[col_b]) ** 2).mean())
-                df_metric.loc[a, b] = rmse
-                df_metric.loc[b, a] = rmse
+                col_a, col_b = f'{metric}_{a}', f'{metric}_{b}'
+                score = function(df_[col_a], df_[col_b])
+                df_metric.loc[a, b] = score
+                df_metric.loc[b, a] = score
             df_metric = df_metric.reindex(sorted(df_metric.columns), axis=1)
-            columns = pd.MultiIndex.from_tuples([(metric, col) for col in df_metric.columns])
-            df_metric.columns = columns
-            df_lst.append(df_metric)
-
-        self._df_rmse = pd.concat(df_lst, axis=1)
-        self._df_rmse.columns.name = 'bin'
-        self._df_rmse.index.name = 'bin'
-
-    @property
-    def results(self):
-        """Returns compiled dataframe of solutions
 
-        Returns:
-            pd.DataFrame
-        """
-        return self._df_result
-
-    @property
-    def distributions(self):
-        """Returns distributions dataframe
-
-        Returns
-            pd.DataFrame
-        """
-        return self._df_dist
-
-    @property
-    def rmse(self):
-        return self._df_rmse
+            # Build multiindexed columns, top level for metric, bottom for group
+            df_metric.columns = pd.MultiIndex.from_tuples([(metric, col) for col in df_metric.columns])
+            df_lst.append(df_metric)
 
-    @property
-    def aggregations(self):
-        return self._df_agg
+        df = pd.concat(df_lst, axis=1)
+        df.columns.name = 'bin'
+        df.index.name = 'bin'
+        return df
 
     def _build_aggregation(self):
         """Aggregates metric data by bins
 
         Sets:
             _df_agg
         """
@@ -409,14 +414,48 @@
 
             ax[i].set_title(f'{metric.title()}')
             ax[i].tick_params(axis='x', labelrotation=45)
             ax[i].legend()
 
         plt.show()
 
+    @property
+    def totals(self):
+        return self._df_totals
+
+    @property
+    def mape(self):
+        return self._df_mape
+
+    @property
+    def results(self):
+        """Returns compiled dataframe of solutions
+
+        Returns:
+            pd.DataFrame
+        """
+        return self._df_result
+
+    @property
+    def distributions(self):
+        """Returns distributions dataframe
+
+        Returns
+            pd.DataFrame
+        """
+        return self._df_dist
+
+    @property
+    def rmse(self):
+        return self._df_rmse
+
+    @property
+    def aggregations(self):
+        return self._df_agg
+
 
 class ABSplit(SplitBase):
     """Splits data into A/B groups based on specified parameters. All members of the population will be in one bin or
     the other.
 
     Attributes:
         _runs (int): Number of runs of the genetic algorithm to try
@@ -446,15 +485,14 @@
 
         Args:
             df (pd.DataFrame): Dataframe to be split
             ga_params (dict): Parameters for the genetic algorithm (default: {})
             metric_weights (dict): Weights for each metric in the data (default: {})
             **kwargs: Additional keyword arguments
         """
-        # print(cutoff_date)
         super().__init__(ga_params=ga_params, metric_weights=metric_weights, cutoff_date=cutoff_date, **kwargs)
         self.df = df
         self._population = Data(self.df.copy(), cutoff_date=cutoff_date, **kwargs)
 
     def _build_df_vis(self):
         """Builds dataframe for use in visualisation of groups.
 
@@ -587,16 +625,24 @@
         scaler.fit(pd.concat([self._df_pop, self._df_samp], axis=0)[self.metrics])
 
         self._population = Data(self._df_pop, scaler=scaler, **kwargs)
         self._sample = Data(self._df_samp, scaler=scaler, **kwargs)
 
         # Makes the match matrix available globally, sum along population axis
         global match_metrics_global
+        global metric_weights_global
         match_metrics_global = self._sample.matrix.sum(1)
+        metric_weights_global = metric_weights_global.reshape(1, -1)
 
+        self._update_initial_population()
+
+    def _update_initial_population(self):
+        """Update initial population so frequency of '1's in starting population is sample_size/population_size
+        to speed up convergence.
+        """
         # Update initial population
         pop_size = self._population.unstacked.shape[0]
         sample_size = self._sample.unstacked.shape[0]
         total = pop_size + sample_size
         init_pop = np.random.choice(
             [0, 1],
             p=[pop_size/total, sample_size/total],
@@ -642,57 +688,99 @@
 
     def __repr__(self):
         lst_str = [f"'{col}', " for col in self.all_spec_columns]
         return f'Match([{lst_str}])'
 
 
 def fitness_func_absplit(ga_instance, solution, solution_idx):
-    """Fitness function for ABSplit
+    """Compute the fitness value for a given solution in the context of ABSplit class.
+
+    The fitness function is a measure of solution quality. In this case, it's computed
+    as the inverse of a sum of penalties related to size, mean squared error (MSE), and
+    sum, for different groups in the solution.
+
+    Args:
+        ga_instance (pygad.GA): An instance of the GA algorithm from the PyGAD library.
+            This argument is required by PyGAD but not used in this function.
+        solution (numpy.ndarray): A 1-D array representing a potential solution for the
+            GA. The elements in the array represent group identifiers.
+        solution_idx (int): The index of the solution in the current population. This
+            argument is required by PyGAD but not used in this function.
+
+    Globals:
+        all_metrics_global (numpy.ndarray): A 3-D array representing different metrics,
+            for different population groups, across different dates.
+        metric_weights_global (numpy.ndarray): A 1-D array representing the relative
+            importance of each metric in `all_metrics_global`.
+        splits_global (numpy.ndarray): A 1-D array representing the proportional split
+            for each group in the population.
+        size_penalty_global (float): A constant representing the penalty weight for size
+            discrepancy among different groups.
+        sum_penalty_global (float): A constant representing the penalty weight for sum
+            discrepancy among different groups.
+        group_ids_global (numpy.ndarray): A 1-D array representing the unique identifiers
+            for each group in the population.
+
+    Returns:
+        float: The fitness value for the given solution. Higher values represent better
+        solutions.
+
+    Notes:
+        The fitness is computed as follows:
+        1. First, for each group in the solution, a binary array is computed. Dimensions:
+            (number of groups, size of population.
+        2. Size penalty is calculated based on differences in population count between groups
+        3. The mean squared error (MSE) for each metric is calculated between groups
+        4. Sum penalty is calculated based on the difference in sum of metrics over time costs between groups.
+        5. The total cost is computed as the sum of the MSE, size penalty, and sum penalty.
+        6. The fitness value is then computed as the inverse of the absolute total cost
+           (plus a small number to prevent division by zero).
     """
+
     global all_metrics_global     # 3d matrix of (metrics, population, dates)
     global metric_weights_global  # Relative weights for each metric
     global splits_global          # Proportional splits for each group
     global size_penalty_global    # Float weight for size penalty
+    global sum_penalty_global     # Float weight for sum penalty
     global group_ids_global       # Array of group IDs
 
     # Generate binary array, 1 row of 0s and 1s for each group (where solution == 1/2/3 etc)
-    # groups = np.array([(solution == i).astype(int) for i in range(len(splits_global))])
     groups = (solution == group_ids_global[:, None]).astype(int)
 
-    # Size penalty
+    # == Size penalty == #
     # Calculate all_metrics mean * number of days * number of metrics
     mean = np.mean(all_metrics_global) * all_metrics_global.shape[0] * all_metrics_global.shape[2]
     # Get size cost for each group
     mean_group = (groups * mean).sum(1) * splits_global
     # Calculate group differences, sum
-    size_cost = (np.abs(np.roll(mean_group, -1) - mean_group).sum()) * size_penalty_global / len(splits_global)
-    # return
+    size_cost = (np.abs(np.roll(mean_group, -1) - mean_group).sum()) * size_penalty_global / (4*len(splits_global)) ** 1.2
 
-    # Metric cost
-    costs = (groups @ all_metrics_global) * splits_global.reshape((1, -1, 1)) * metric_weights_global.reshape(-1, 1, 1)
+    # == MSE == #
+    costs = (groups @ all_metrics_global) * splits_global * metric_weights_global
     diffs = np.roll(costs, -1, axis=1) - costs
     mse = ((diffs ** 2).mean(axis=1)).sum()
-    mse = mse + size_cost
+
+    # == Sum penalty == #
+    sum_cost = (np.abs(costs.sum(2) - np.roll(costs.sum(2), shift=-1, axis=1)).sum() * sum_penalty_global) / (4*len(splits_global)) ** 1.2
 
     # Fitness
-    fitness = 1.0 / np.abs(mse + 1e-10)  # Add small sum to prevent divide by zero
+    total = mse + size_cost + sum_cost
+    fitness = 1.0 / np.abs(total + 1e-5)  # Add small sum to prevent divide by zero
     return fitness
 
 
 def fitness_func_match(ga_instance, solution, solution_idx):
     """Fitness function for Match
     """
     global all_metrics_global
     global match_metrics_global
     global metric_weights_global
 
     cost1 = match_metrics_global  # Sum along population axis
     cost2 = solution @ all_metrics_global
+
     # Average over time axis, sum over metric axis
     mse = (metric_weights_global @ ((cost1 - cost2)**2).mean(1)).sum()
 
     # Fitness
     fitness = 1.0 / np.abs(mse + 1e-10)  # Add small sum to prevent divide by zero
     return fitness
-
-
-
```

### Comparing `absplit-1.3.1/absplit/param.py` & `absplit-1.4.0/absplit/param.py`

 * *Files identical despite different names*

### Comparing `absplit-1.3.1/absplit/tutorials.py` & `absplit-1.4.0/absplit/tutorials.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,15 +70,14 @@
     if drop_fips:
         df = df.drop('fips', axis=1)
     else:
         df = df[~df['fips'].isna()].reset_index(drop=True)
         df['fips'] = df['fips'].astype('int64').astype(str)
     cols = ['state', 'county', 'date']
     cols = cols + ['fips'] if not drop_fips else cols
-    print(cols)
     df = df.set_index(cols).sort_index()
     df = df.groupby(level=[0, 1]).diff().fillna(0).clip(lower=0)
     resampler = lambda x: x.set_index('date').resample('w').sum()
     df = df.reset_index(level=2).groupby([x for x in cols if x != 'date']).apply(resampler).reset_index()
     return df
```

### Comparing `absplit-1.3.1/images/logo.jpeg` & `absplit-1.4.0/images/logo.jpeg`

 * *Files identical despite different names*

### Comparing `absplit-1.3.1/pyproject.toml` & `absplit-1.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "absplit"
-version = "1.3.1"
-description = "Generates A/B test groups"
+version = "1.4.0"
+description = "Generates A/B/n test groups"
 readme = "README.md"
 authors = [{name = "Cormac Rynne", email = "cormac.ry@gmail.com"}]
 license = {file = "LICENSE"}
 repository = "https://github.com/cormac-rynne/absplit"
 requires-python = "<=3.11"
 classifiers = [
     "License :: OSI Approved :: MIT License",
```

### Comparing `absplit-1.3.1/tests/test_data.py` & `absplit-1.4.0/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `absplit-1.3.1/tests/test_ga.py` & `absplit-1.4.0/tests/test_ga.py`

 * *Files identical despite different names*

### Comparing `absplit-1.3.1/PKG-INFO` & `absplit-1.4.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: absplit
-Version: 1.3.1
-Summary: Generates A/B test groups
+Version: 1.4.0
+Summary: Generates A/B/n test groups
 Keywords: absplit,a/b test,ab test,ab split,split,set formation,group formation
 Author-email: Cormac Rynne <cormac.ry@gmail.com>
 Requires-Python: <=3.11
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
@@ -31,15 +31,15 @@
 
 <div align="center">
 <img src="https://raw.githubusercontent.com/cormac-rynne/absplit/main/images/logo.jpeg" width="460" height="140">
 <h3><strong>ABSplit</strong></h3>
 Split your data into matching A/B/n groups
 
 ![license](https://img.shields.io/badge/License-MIT-blue.svg)
-![version](https://img.shields.io/badge/version-1.3.1-blue.svg)
+![version](https://img.shields.io/badge/version-1.4.0-blue.svg)
 ![version](https://img.shields.io/badge/python-3-orange.svg)
 
 </div>
 
 <details open>
   <summary>Table of Contents</summary>
   <ol>
@@ -146,22 +146,23 @@
 
 # Visualise data
 ab.visualise()
 
 # Extract bin splits
 df = ab.results
 
-# Extract distributions summary
-df_dist = ab.distributions
-
 # Extract data aggregated by bins
 df_agg = ab.aggregations
 
-# Extract RMSE summary
-df_rmse = ab.rmse
+# Extract summary statistics
+df_dist = ab.distributions    # Population counts between groups
+df_rmse = ab.rmse             # RMSE between groups for each metric
+df_mape = ab.mape             # MAPE between groups for each metric
+df_totals = ab.totals         # Total sum of each metric for each group
+
 ```
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 ## API Reference
 ### Absplit 
 `ABSplit(df, metrics, splitting, date_col=None, ga_params={}, metric_weights={}, splits=[0.5, 0.5], size_penalty=0)`
 
@@ -177,14 +178,16 @@
 * `ga_params` (dict, optional): Parameters for the genetic algorithm `pygad.GA` module parameters, see 
 [here](https://pygad.readthedocs.io/en/latest/README_pygad_ReadTheDocs.html#pygad-ga-class) for arguments you can pass
 (default: `{}`)
 * `splits` (list, optional): How many groups to split into, and relative size of the groups (default: `[0.5, 0.5]`,
 2 groups of equal size)
 * `size_penalty` (float, optional): Penalty weighting for differences in the population count between groups 
 (default: `0`)
+* `sum_penalty` (float, optional): Penalty weighting for the sum of metrics over time. If this is greater than zero,
+it will add a penalty to the cost function that will try and make the sum of each metric the same for each group.
 * `cutoff_date` (str, optional): Cutoff date between fitting and validation data. For example, if you have data between 
 2023-01-01 and 2023-03-01, and the cutoff date is 2023-02-01, the algorithm will only perform the fit on data between 
 2023-01-01 and 2023-02-01. If `None`, it will fit on all available data. If cutoff date is provided, RMSE scores
   (gotten by using the `ab.rmse` attribute) will only be for validation period (i.e., from 2023-02-01 to end of 
 timeseries)
 * `metric_weights` (dict, optional): Weights for each metric in the data. If you want the splitting to focus on 
 one metrics more than the other, you can prioritise this here (default: `{}`)
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1 Name: absplit Version: 1.3.1 Summary: Generates A/B test
-groups Keywords: absplit,a/b test,ab test,ab split,split,set formation,group
-formation Author-email: Cormac Rynne
+Metadata-Version: 2.1 Name: absplit Version: 1.4.0 Summary: Generates A/B/
+n test groups Keywords: absplit,a/b test,ab test,ab split,split,set
+formation,group formation Author-email: Cormac Rynne
 ry@gmail.com> Requires-Python: <=3.11 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Intended
 Audience :: Developers Classifier: Intended Audience :: Science/Research
@@ -15,15 +15,15 @@
 Libraries :: Python Modules Requires-Dist: pygad==3.0.1 Requires-Dist: scikit-
 learn Requires-Dist: numpy Requires-Dist: pandas Requires-Dist: seaborn
 Project-URL: Home, https://github.com/cormac-rynne/absplit
 [https://raw.githubusercontent.com/cormac-rynne/absplit/main/images/logo.jpeg]
                                **** ABSplit ****
  Split your data into matching A/B/n groups ![license](https://img.shields.io/
  badge/License-MIT-blue.svg) ![version](https://img.shields.io/badge/version-
- 1.3.1-blue.svg) ![version](https://img.shields.io/badge/python-3-orange.svg)
+ 1.4.0-blue.svg) ![version](https://img.shields.io/badge/python-3-orange.svg)
  Table of Contents
    1. About_The_Project
    2. Getting_Started
           o Installation
    3. Tutorials
           o Do_it_yourself
    4. Usage
@@ -61,17 +61,19 @@
 in ['a', 'b', 'c', 'd', 'e']] for item in sublist], 'metric1': np.arange(0, 15,
 1), 'metric2': np.arange(0, 150, 10) } df = pd.DataFrame(data_dct) # Identify
 which columns are metrics, which is the time period, and what to split on
 kwargs = { 'metrics': ['metric1', 'metric2'], 'date_col': 'date', 'splitting':
 'city' } # Initialise ab = ABSplit( df=df, split=[.5, .5], # Split into 2
 groups of equal size **kwargs, ) # Generate split ab.run() # Visualise
 generation fitness ab.fitness() # Visualise data ab.visualise() # Extract bin
-splits df = ab.results # Extract distributions summary df_dist =
-ab.distributions # Extract data aggregated by bins df_agg = ab.aggregations #
-Extract RMSE summary df_rmse = ab.rmse ```
+splits df = ab.results # Extract data aggregated by bins df_agg =
+ab.aggregations # Extract summary statistics df_dist = ab.distributions #
+Population counts between groups df_rmse = ab.rmse # RMSE between groups for
+each metric df_mape = ab.mape # MAPE between groups for each metric df_totals =
+ab.totals # Total sum of each metric for each group ```
                                                                   (back_to_top)
 ## API Reference ### Absplit `ABSplit(df, metrics, splitting, date_col=None,
 ga_params={}, metric_weights={}, splits=[0.5, 0.5], size_penalty=0)` Splits
 population into n groups. Mutually exclusive, completely exhaustive Arguments:
 * `df` (pd.DataFrame): Dataframe of population to be split * `metrics` (str,
 list): Name of, or list of names of, metric columns in DataFrame to be
 considered in split * `splitting` (str): Name of column that represents
@@ -82,14 +84,17 @@
 timeseries, (default `None`) * `ga_params` (dict, optional): Parameters for the
 genetic algorithm `pygad.GA` module parameters, see [here](https://
 pygad.readthedocs.io/en/latest/README_pygad_ReadTheDocs.html#pygad-ga-class)
 for arguments you can pass (default: `{}`) * `splits` (list, optional): How
 many groups to split into, and relative size of the groups (default: `[0.5,
 0.5]`, 2 groups of equal size) * `size_penalty` (float, optional): Penalty
 weighting for differences in the population count between groups (default: `0`)
+* `sum_penalty` (float, optional): Penalty weighting for the sum of metrics
+over time. If this is greater than zero, it will add a penalty to the cost
+function that will try and make the sum of each metric the same for each group.
 * `cutoff_date` (str, optional): Cutoff date between fitting and validation
 data. For example, if you have data between 2023-01-01 and 2023-03-01, and the
 cutoff date is 2023-02-01, the algorithm will only perform the fit on data
 between 2023-01-01 and 2023-02-01. If `None`, it will fit on all available
 data. If cutoff date is provided, RMSE scores (gotten by using the `ab.rmse`
 attribute) will only be for validation period (i.e., from 2023-02-01 to end of
 timeseries) * `metric_weights` (dict, optional): Weights for each metric in the
```

