# Comparing `tmp/loren_frank_data_processing-0.9.9.dev0.tar.gz` & `tmp/loren_frank_data_processing-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/loren_frank_data_processing-0.9.9.dev0.tar", last modified: Fri Mar  6 02:11:38 2020, max compression
+gzip compressed data, was "loren_frank_data_processing-1.0.1.tar", last modified: Sat Jul  1 22:14:45 2023, max compression
```

## Comparing `loren_frank_data_processing-0.9.9.dev0.tar` & `loren_frank_data_processing-1.0.1.tar`

### file list

```diff
@@ -1,26 +1,30 @@
-drwxr-xr-x   0 edeno      (501) staff       (20)        0 2020-03-06 02:11:38.000000 loren_frank_data_processing-0.9.9.dev0/
--rw-r--r--   0 edeno      (501) staff       (20)      299 2020-03-06 02:11:38.000000 loren_frank_data_processing-0.9.9.dev0/PKG-INFO
--rw-r--r--   0 edeno      (501) staff       (20)     2900 2017-10-25 18:29:28.000000 loren_frank_data_processing-0.9.9.dev0/README.md
--rw-r--r--   0 edeno      (501) staff       (20)      667 2020-03-06 02:11:22.000000 loren_frank_data_processing-0.9.9.dev0/setup.py
--rw-r--r--   0 edeno      (501) staff       (20)       63 2020-03-06 02:11:38.000000 loren_frank_data_processing-0.9.9.dev0/setup.cfg
-drwxr-xr-x   0 edeno      (501) staff       (20)        0 2020-03-06 02:11:38.000000 loren_frank_data_processing-0.9.9.dev0/loren_frank_data_processing/
--rw-r--r--   0 edeno      (501) staff       (20)     1593 2018-10-24 18:08:53.000000 loren_frank_data_processing-0.9.9.dev0/loren_frank_data_processing/DIO.py
--rw-r--r--   0 edeno      (501) staff       (20)     2517 2020-01-30 19:22:24.000000 loren_frank_data_processing-0.9.9.dev0/loren_frank_data_processing/task.py
--rw-r--r--   0 edeno      (501) staff       (20)     3720 2017-10-23 16:54:51.000000 loren_frank_data_processing-0.9.9.dev0/loren_frank_data_processing/ripples.py
--rw-r--r--   0 edeno      (501) staff       (20)    10202 2020-01-23 05:58:23.000000 loren_frank_data_processing-0.9.9.dev0/loren_frank_data_processing/well_traversal_classification.py
--rw-r--r--   0 edeno      (501) staff       (20)      879 2018-09-26 14:55:06.000000 loren_frank_data_processing-0.9.9.dev0/loren_frank_data_processing/saving.py
--rw-r--r--   0 edeno      (501) staff       (20)      946 2020-01-22 00:40:54.000000 loren_frank_data_processing-0.9.9.dev0/loren_frank_data_processing/__init__.py
--rw-r--r--   0 edeno      (501) staff       (20)     4113 2020-01-30 20:13:54.000000 loren_frank_data_processing-0.9.9.dev0/loren_frank_data_processing/core.py
--rw-r--r--   0 edeno      (501) staff       (20)     6850 2020-01-30 19:22:24.000000 loren_frank_data_processing-0.9.9.dev0/loren_frank_data_processing/multiunit.py
--rw-r--r--   0 edeno      (501) staff       (20)     4359 2020-01-22 00:40:54.000000 loren_frank_data_processing-0.9.9.dev0/loren_frank_data_processing/visualization.py
--rw-r--r--   0 edeno      (501) staff       (20)     7538 2020-01-31 06:27:27.000000 loren_frank_data_processing-0.9.9.dev0/loren_frank_data_processing/neurons.py
--rw-r--r--   0 edeno      (501) staff       (20)    17524 2020-03-06 02:11:22.000000 loren_frank_data_processing-0.9.9.dev0/loren_frank_data_processing/position.py
--rw-r--r--   0 edeno      (501) staff       (20)     9609 2018-10-17 18:58:11.000000 loren_frank_data_processing-0.9.9.dev0/loren_frank_data_processing/utilities.py
--rw-r--r--   0 edeno      (501) staff       (20)     8103 2020-01-23 00:24:04.000000 loren_frank_data_processing-0.9.9.dev0/loren_frank_data_processing/tetrodes.py
--rw-r--r--   0 edeno      (501) staff       (20)    14280 2020-02-21 23:18:33.000000 loren_frank_data_processing-0.9.9.dev0/loren_frank_data_processing/track_segment_classification.py
-drwxr-xr-x   0 edeno      (501) staff       (20)        0 2020-03-06 02:11:38.000000 loren_frank_data_processing-0.9.9.dev0/loren_frank_data_processing.egg-info/
--rw-r--r--   0 edeno      (501) staff       (20)      299 2020-03-06 02:11:38.000000 loren_frank_data_processing-0.9.9.dev0/loren_frank_data_processing.egg-info/PKG-INFO
--rw-r--r--   0 edeno      (501) staff       (20)      873 2020-03-06 02:11:38.000000 loren_frank_data_processing-0.9.9.dev0/loren_frank_data_processing.egg-info/SOURCES.txt
--rw-r--r--   0 edeno      (501) staff       (20)       80 2020-03-06 02:11:38.000000 loren_frank_data_processing-0.9.9.dev0/loren_frank_data_processing.egg-info/requires.txt
--rw-r--r--   0 edeno      (501) staff       (20)       28 2020-03-06 02:11:38.000000 loren_frank_data_processing-0.9.9.dev0/loren_frank_data_processing.egg-info/top_level.txt
--rw-r--r--   0 edeno      (501) staff       (20)        1 2020-03-06 02:11:38.000000 loren_frank_data_processing-0.9.9.dev0/loren_frank_data_processing.egg-info/dependency_links.txt
+drwxr-xr-x   0 edeno      (501) staff       (20)        0 2023-07-01 22:14:45.414255 loren_frank_data_processing-1.0.1/
+-rw-r--r--   0 edeno      (501) staff       (20)    35139 2017-10-24 18:08:07.000000 loren_frank_data_processing-1.0.1/LICENSE
+-rw-r--r--   0 edeno      (501) staff       (20)      277 2023-07-01 22:14:45.414336 loren_frank_data_processing-1.0.1/PKG-INFO
+-rw-r--r--   0 edeno      (501) staff       (20)     2910 2022-10-17 17:51:30.000000 loren_frank_data_processing-1.0.1/README.md
+drwxr-xr-x   0 edeno      (501) staff       (20)        0 2023-07-01 22:14:45.412961 loren_frank_data_processing-1.0.1/loren_frank_data_processing/
+-rw-r--r--   0 edeno      (501) staff       (20)     1504 2023-07-01 22:11:52.000000 loren_frank_data_processing-1.0.1/loren_frank_data_processing/DIO.py
+-rw-r--r--   0 edeno      (501) staff       (20)      878 2023-07-01 22:11:45.000000 loren_frank_data_processing-1.0.1/loren_frank_data_processing/__init__.py
+-rw-r--r--   0 edeno      (501) staff       (20)     4112 2023-07-01 22:11:49.000000 loren_frank_data_processing-1.0.1/loren_frank_data_processing/core.py
+-rw-r--r--   0 edeno      (501) staff       (20)     6692 2023-07-01 22:11:59.000000 loren_frank_data_processing-1.0.1/loren_frank_data_processing/multiunit.py
+-rw-r--r--   0 edeno      (501) staff       (20)     8430 2023-07-01 22:12:03.000000 loren_frank_data_processing-1.0.1/loren_frank_data_processing/neurons.py
+-rw-r--r--   0 edeno      (501) staff       (20)    16882 2023-07-01 22:12:10.000000 loren_frank_data_processing-1.0.1/loren_frank_data_processing/position.py
+-rw-r--r--   0 edeno      (501) staff       (20)     3729 2023-07-01 22:12:14.000000 loren_frank_data_processing-1.0.1/loren_frank_data_processing/ripples.py
+-rw-r--r--   0 edeno      (501) staff       (20)      879 2023-07-01 22:12:19.000000 loren_frank_data_processing-1.0.1/loren_frank_data_processing/saving.py
+-rw-r--r--   0 edeno      (501) staff       (20)     2654 2023-07-01 22:12:23.000000 loren_frank_data_processing-1.0.1/loren_frank_data_processing/task.py
+-rw-r--r--   0 edeno      (501) staff       (20)     7636 2023-07-01 22:12:28.000000 loren_frank_data_processing-1.0.1/loren_frank_data_processing/tetrodes.py
+-rw-r--r--   0 edeno      (501) staff       (20)    14408 2023-07-01 22:12:33.000000 loren_frank_data_processing-1.0.1/loren_frank_data_processing/track_segment_classification.py
+-rw-r--r--   0 edeno      (501) staff       (20)     9600 2023-07-01 22:12:37.000000 loren_frank_data_processing-1.0.1/loren_frank_data_processing/utilities.py
+-rw-r--r--   0 edeno      (501) staff       (20)     4281 2023-07-01 22:12:43.000000 loren_frank_data_processing-1.0.1/loren_frank_data_processing/visualization.py
+-rw-r--r--   0 edeno      (501) staff       (20)    10120 2023-07-01 22:12:46.000000 loren_frank_data_processing-1.0.1/loren_frank_data_processing/well_traversal_classification.py
+drwxr-xr-x   0 edeno      (501) staff       (20)        0 2023-07-01 22:14:45.413673 loren_frank_data_processing-1.0.1/loren_frank_data_processing.egg-info/
+-rw-r--r--   0 edeno      (501) staff       (20)      277 2023-07-01 22:14:45.000000 loren_frank_data_processing-1.0.1/loren_frank_data_processing.egg-info/PKG-INFO
+-rw-r--r--   0 edeno      (501) staff       (20)      925 2023-07-01 22:14:45.000000 loren_frank_data_processing-1.0.1/loren_frank_data_processing.egg-info/SOURCES.txt
+-rw-r--r--   0 edeno      (501) staff       (20)        1 2023-07-01 22:14:45.000000 loren_frank_data_processing-1.0.1/loren_frank_data_processing.egg-info/dependency_links.txt
+-rw-r--r--   0 edeno      (501) staff       (20)       80 2023-07-01 22:14:45.000000 loren_frank_data_processing-1.0.1/loren_frank_data_processing.egg-info/requires.txt
+-rw-r--r--   0 edeno      (501) staff       (20)       28 2023-07-01 22:14:45.000000 loren_frank_data_processing-1.0.1/loren_frank_data_processing.egg-info/top_level.txt
+-rw-r--r--   0 edeno      (501) staff       (20)       63 2023-07-01 22:14:45.414617 loren_frank_data_processing-1.0.1/setup.cfg
+-rw-r--r--   0 edeno      (501) staff       (20)      657 2023-07-01 22:13:25.000000 loren_frank_data_processing-1.0.1/setup.py
+drwxr-xr-x   0 edeno      (501) staff       (20)        0 2023-07-01 22:14:45.414071 loren_frank_data_processing-1.0.1/tests/
+-rw-r--r--   0 edeno      (501) staff       (20)     1508 2022-10-17 17:51:50.000000 loren_frank_data_processing-1.0.1/tests/test_core_.py
+-rw-r--r--   0 edeno      (501) staff       (20)      580 2022-10-17 17:51:55.000000 loren_frank_data_processing-1.0.1/tests/test_utilities.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `loren_frank_data_processing-0.9.9.dev0/README.md` & `loren_frank_data_processing-1.0.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,44 +1,49 @@
 # loren_frank_data_processing
+
 ![](https://travis-ci.org/Eden-Kramer-Lab/loren_frank_data_processing.svg?branch=master)[![Coverage Status](https://coveralls.io/repos/github/Eden-Kramer-Lab/loren_frank_data_processing/badge.svg?branch=master)](https://coveralls.io/github/Eden-Kramer-Lab/loren_frank_data_processing?branch=master)
 
 The `loren_frank_data_processing` package imports Matlab data processed by [Loren Frank's lab](http://www.cin.ucsf.edu/HTML/Loren_Frank.html) into a friendly python format using [pandas](https://pandas.pydata.org/pandas-docs/stable/index.html).
 
 In order to use, the data must follow the format proscribed in this [wiki](https://github.com/Eden-Kramer-Lab/Loren-Frank-Data-Format--Description/wiki).
 
 Features
+
 + Takes advantages of pandas `DataFrame`, a expressive labeled data format, and associated data manipulation and alignment tools.
 + Time is encoded as pandas `Timedelta`, which avoids funny business with representing time series as floating points.
 + Handy utility for reshaping time series relative to events of interest (`reshape_to_segments`)
 
 ### Installation ###
+
 ```python
 pip install loren_frank_data_processing
 ```
 
 OR
 
 ```python
 conda install -c edeno loren_frank_data_processing
 ```
 
 ### Package Dependencies ###
+
 `loren_frank_data_processing` requires:
-- python>=3.5
-- numpy
-- scipy
-- pandas
-- xarray (only if using features from the saving module)
-- netcdf4 (only if using features from the saving module)
++ python>=3.5
++ numpy
++ scipy
++ pandas
++ xarray (only if using features from the saving module)
++ netcdf4 (only if using features from the saving module)
 
 See [environment.yml](environment.yml) for the most current list of dependencies.
 
-
 ### Example ###
+
 1. Find all recording epochs:
+
 ```pytho
 from collections import namedtuple
 from os.path import join
 
 from loren_frank_data_processing import make_epochs_dataframe
 
 ROOT_DIR = 'example/path'
@@ -50,24 +55,28 @@
                   short_name='HPa'),
 }
 
 epoch_info = make_epochs_dataframe(ANIMALS)
 
 epoch_info
 ```
+
 ![](epoch_info.png)
 
 2. We can filter by epoch type:
+
 ```python
 epoch_info.loc[epoch_info.type == 'run']
 ```
+
 ![](epoch_info_filtered.png)
 
 3. We can use the `epoch_info` index to access the tetrode information for a
 recording session.
+
 ```python
 epoch_info.loc[epoch_info.type == 'run'].index.tolist()
 Out:
 [('HPa', 1, 2),
  ('HPa', 1, 4),
  ('HPa', 1, 6),
  ('HPa', 2, 2),
@@ -87,11 +96,12 @@
 
  from loren_frank_data_processing import make_tetrode_dataframe
 
 epoch_key = ('HPa', 1, 2)
 tetrode_info = make_tetrode_dataframe(ANIMALS)
 tetrode_info.xs(epoch_key, drop_level=False)
 ```
+
 ![](/tetrode_info.png)
 
 Similarly, the index for the tetrode info can be used as a key to
 access LFP information
```

### Comparing `loren_frank_data_processing-0.9.9.dev0/loren_frank_data_processing/DIO.py` & `loren_frank_data_processing-1.0.1/loren_frank_data_processing/DIO.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,47 +1,43 @@
-'''
+"""
 The DIO cell gives arrival/departure times at the end of each arm of the maze
 (as indicated by the IR motion sensors at the end of the wells) and the
 start/stop times for the output trigger to the reward pump
-'''
+"""
 
 import numpy as np
 import pandas as pd
 
 from .core import get_data_structure
 from .tetrodes import get_trial_time
 
 
 def get_DIO(epoch_key, animals):
-    ''''''
+    """"""
     animal, day, epoch = epoch_key
-    pins = get_data_structure(
-        animals[animal], day, 'DIO', 'DIO')[epoch - 1].squeeze()
+    pins = get_data_structure(animals[animal], day, "DIO", "DIO")[epoch - 1].squeeze()
     pins_df = []
 
     for pin in pins:
         try:
             try:
-                time = pd.to_timedelta(pin['times'][0, 0].squeeze(), unit='s')
+                time = pd.to_timedelta(pin["times"][0, 0].squeeze(), unit="s")
             except ValueError:
-                time = pd.to_timedelta(pin['times'][0, 0].item(), unit='s')
-            values = pin['values'][0, 0].squeeze()
-            pin_id = pin['original_id'][0, 0].item()
+                time = pd.to_timedelta(pin["times"][0, 0].item(), unit="s")
+            values = pin["values"][0, 0].squeeze()
+            pin_id = pin["original_id"][0, 0].item()
 
             try:
                 series = pd.Series(values, index=time, name=pin_id)
             except TypeError:
-                series = pd.Series(name=pin_id)
+                series = pd.Series(index=[time], name=pin_id)
             pins_df.append(series)
         except IndexError:
             continue
     return pd.concat(pins_df, axis=1).fillna(0).sort_index()
 
 
 def get_DIO_indicator(epoch_key, animals, time_function=get_trial_time):
     time = time_function(epoch_key, animals)
     dio = get_DIO(epoch_key, animals)
-    time_index = np.digitize(dio.index.total_seconds(),
-                             time.total_seconds())
-    time_index[time_index == time.size] = time.size - 1
-    return (dio.groupby(time[time_index]).sum()
-            .reindex(index=time, fill_value=0))
+    time_index = np.digitize(dio.index.total_seconds(), time.total_seconds()[1:-1])
+    return dio.groupby(time[time_index]).sum().reindex(index=time, fill_value=0)
```

### Comparing `loren_frank_data_processing-0.9.9.dev0/loren_frank_data_processing/task.py` & `loren_frank_data_processing-1.0.1/loren_frank_data_processing/task.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,90 +3,100 @@
 
 import numpy as np
 import pandas as pd
 from scipy.io import loadmat
 
 
 def load_task(file_name, animal):
-    '''Loads task information for a specific day and converts it to a pandas
+    """Loads task information for a specific day and converts it to a pandas
     DataFrame.
 
     Parameters
     ----------
     file_name : str
         Task file name for an animal and recording session day.
     animal : namedtuple
         Information about data directory for the animal.
 
     Returns
     -------
     task_information : pandas.DataFrame
 
-    '''
-    data = loadmat(file_name, variable_names=('task'))['task']
+    """
+    data = loadmat(file_name, variable_names=("task"))["task"]
     day = data.shape[-1]
     epochs = data[0, -1][0]
     n_epochs = len(epochs)
     index = pd.MultiIndex.from_product(
         ([animal.short_name], [day], np.arange(n_epochs) + 1),
-        names=['animal', 'day', 'epoch'])
+        names=["animal", "day", "epoch"],
+    )
 
-    return pd.DataFrame(
-        [{name: epoch[name].item().squeeze()
-          for name in epoch.dtype.names
-          if name in ['environment', 'type']}
-         for epoch in epochs]).set_index(index).assign(
-        environment=lambda df: df.environment.astype(str),
-        type=lambda df: df.type.astype(str))
+    return (
+        pd.DataFrame(
+            [
+                {
+                    name: epoch[name].item().squeeze()
+                    for name in epoch.dtype.names
+                    if name in ["environment", "type"]
+                }
+                for epoch in epochs
+            ]
+        )
+        .set_index(index)
+        .assign(
+            environment=lambda df: df.environment.astype(str),
+            type=lambda df: df.type.astype(str),
+        )
+    )
 
 
 def _count_exposure(df):
-    df['exposure'] = np.arange(len(df)) + 1
+    df["exposure"] = np.arange(len(df)) + 1
     return df
 
 
 def compute_exposure(epoch_info):
-    df = epoch_info.groupby(['animal', 'environment']).apply(
-        _count_exposure)
-    df['exposure'] = df.exposure.where(
-        ~epoch_info.type.isin(['sleep', 'rest', 'nan', 'failed sleep']))
+    df = epoch_info.groupby(["animal", "environment"]).apply(_count_exposure)
+    df["exposure"] = df.exposure.where(
+        ~epoch_info.type.isin(["sleep", "rest", "nan", "failed sleep"])
+    )
     return df
 
 
 def get_task(animal):
-    '''Loads all experimental information for all days for a given animal.
+    """Loads all experimental information for all days for a given animal.
 
     Parameters
     ----------
     animals : dict of named-tuples
         Dictionary containing information about the directory for each
         animal. The key is the animal_short_name.
 
     Returns
     -------
     task_information : pandas.DataFrame
 
-    '''
-    task_files = glob(join(animal.directory, '*task*.mat'))
-    return pd.concat(load_task(task_file, animal)
-                     for task_file in task_files)
+    """
+    task_files = glob(join(animal.directory, "*task*.mat"))
+    return pd.concat(load_task(task_file, animal) for task_file in task_files)
 
 
 def make_epochs_dataframe(animals):
-    '''Experimental conditions for all recording epochs.
+    """Experimental conditions for all recording epochs.
 
     Index is a unique identifying key for that recording epoch.
 
     Parameters
     ----------
     animals : dict of named-tuples
         Dictionary containing information about the directory for each
         animal. The key is the animal_short_name.
 
     Returns
     -------
     epoch_information : pandas.DataFrame
 
-    '''
+    """
     return compute_exposure(
-        pd.concat([get_task(animal) for animal in animals.values()])
-        .sort_index())
+        pd.concat([get_task(animal) for animal in animals.values()]).sort_index()
+    )
```

### Comparing `loren_frank_data_processing-0.9.9.dev0/loren_frank_data_processing/ripples.py` & `loren_frank_data_processing-1.0.1/loren_frank_data_processing/ripples.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,57 +1,59 @@
 import pandas as pd
 
 from .core import get_data_structure
 from .tetrodes import get_LFP_dataframe
 
 
 def _get_computed_ripple_times(tetrode_tuple, animals):
-    '''Returns a list of tuples for a given tetrode in the format
+    """Returns a list of tuples for a given tetrode in the format
     (start_index, end_index). The indexes are relative
     to the trial time for that session. Data is extracted from the ripples
     data structure and calculated according to the Frank Lab criterion.
-    '''
+    """
     animal, day, epoch, tetrode_number = tetrode_tuple
-    ripples_data = get_data_structure(
-        animals[animal], day, 'ripples', 'ripples')
+    ripples_data = get_data_structure(animals[animal], day, "ripples", "ripples")
     return zip(
-        ripples_data[epoch - 1][0][tetrode_number - 1]['starttime'][
-            0, 0].flatten(),
-        ripples_data[epoch - 1][0][tetrode_number - 1]['endtime'][
-            0, 0].flatten())
+        ripples_data[epoch - 1][0][tetrode_number - 1]["starttime"][0, 0].flatten(),
+        ripples_data[epoch - 1][0][tetrode_number - 1]["endtime"][0, 0].flatten(),
+    )
 
 
 def _convert_ripple_times_to_dataframe(ripple_times, dataframe):
-    '''Given a list of ripple time tuples (ripple #, start time, end time)
+    """Given a list of ripple time tuples (ripple #, start time, end time)
     and a dataframe with a time index (such as the lfp dataframe), returns
     a pandas dataframe with a column with the timestamps of each ripple
     labeled according to the ripple number. Non-ripple times are marked as
     NaN.
-    '''
+    """
     try:
         index_dataframe = dataframe.drop(dataframe.columns, axis=1)
     except AttributeError:
         index_dataframe = dataframe[0].drop(dataframe[0].columns, axis=1)
-    ripple_dataframe = (pd.concat(
-        [index_dataframe.loc[start_time:end_time].assign(
-            ripple_number=number)
-         for number, start_time, end_time in ripple_times]))
+    ripple_dataframe = pd.concat(
+        [
+            index_dataframe.loc[start_time:end_time].assign(ripple_number=number)
+            for number, start_time, end_time in ripple_times
+        ]
+    )
     try:
         ripple_dataframe = pd.concat(
-            [dataframe, ripple_dataframe], axis=1,
-            join_axes=[index_dataframe.index])
+            [dataframe, ripple_dataframe], axis=1, join_axes=[index_dataframe.index]
+        )
     except TypeError:
         ripple_dataframe = pd.concat(
             [pd.concat(dataframe, axis=1), ripple_dataframe],
-            axis=1, join_axes=[index_dataframe.index])
+            axis=1,
+            join_axes=[index_dataframe.index],
+        )
     return ripple_dataframe
 
 
 def get_computed_ripples_dataframe(tetrode_key, animals):
-    '''Pre-computed ripples from the Frank lab labeled according to the
+    """Pre-computed ripples from the Frank lab labeled according to the
     ripple number with non-ripple times are marked as NaN.
 
      Parameters
      ----------
      tetrode_key : tuple
          Unique key identifying the tetrode. Elements are
          (animal_short_name, day, epoch, tetrode_number).
@@ -59,26 +61,28 @@
          Dictionary containing information about the directory for each
          animal. The key is the animal_short_name.
 
     Returns
     -------
     ripple_indicator : pandas.DataFrame
 
-    '''
+    """
     ripple_times = _get_computed_ripple_times(tetrode_key, animals)
-    [(ripple_ind + 1, start_time, end_time)
-     for ripple_ind, (start_time, end_time) in enumerate(ripple_times)]
+    [
+        (ripple_ind + 1, start_time, end_time)
+        for ripple_ind, (start_time, end_time) in enumerate(ripple_times)
+    ]
     lfp_dataframe = get_LFP_dataframe(tetrode_key, animals)
-    return (_convert_ripple_times_to_dataframe(ripple_times, lfp_dataframe)
-            .assign(
-                ripple_indicator=lambda x: x.ripple_number.fillna(0) > 0))
+    return _convert_ripple_times_to_dataframe(ripple_times, lfp_dataframe).assign(
+        ripple_indicator=lambda x: x.ripple_number.fillna(0) > 0
+    )
 
 
 def get_computed_consensus_ripple_times(epoch_key, animals):
-    '''Returns a list of tuples for a given epoch in the format
+    """Returns a list of tuples for a given epoch in the format
     (start_time, end_time).
 
     Parameters
     ----------
     epoch_key : tuple
         Unique key identifying the recording epoch. Elements are
         (animal_short_name, day, epoch).
@@ -86,12 +90,13 @@
         Dictionary containing information about the directory for each
         animal. The key is the animal_short_name.
 
     Returns
     -------
     ripple_times : list of tuples
         Each list element corresponds to a ripple with (start_time, end_time).
-    '''
+    """
     animal, day, epoch = epoch_key
     ripples_data = get_data_structure(
-        animals[animal], day, 'candripples', 'candripples')
-    return list(map(tuple, ripples_data[epoch - 1]['riptimes'][0][0]))
+        animals[animal], day, "candripples", "candripples"
+    )
+    return list(map(tuple, ripples_data[epoch - 1]["riptimes"][0][0]))
```

### Comparing `loren_frank_data_processing-0.9.9.dev0/loren_frank_data_processing/well_traversal_classification.py` & `loren_frank_data_processing-1.0.1/loren_frank_data_processing/well_traversal_classification.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,44 +1,40 @@
 import numpy as np
 import pandas as pd
 from scipy.ndimage.measurements import label
 
 from .core import logger
 from .DIO import get_DIO, get_DIO_indicator
 
-_WELL_NAMES = {
-    1: 'Center',
-    2: 'Left',
-    3: 'Right'
-}
+_WELL_NAMES = {1: "Center", 2: "Left", 3: "Right"}
 
-_REWARD_DIOS = ['Dout7', 'Dout8', 'Dout9']
-_DIO_WELL_ORDER = ['Din2', 'Din1', 'Din3']
+_REWARD_DIOS = ["Dout7", "Dout8", "Dout9"]
+_DIO_WELL_ORDER = ["Din2", "Din1", "Din3"]
 
 
 def paired_distances(x, y):
-    '''Euclidean distance between x and y at each time point.
+    """Euclidean distance between x and y at each time point.
 
     Parameters
     ----------
     x,y : ndarray, shape (n_time, n_space)
 
     Returns
     -------
     distance : ndarray, shape (n_time,)
 
-    '''
+    """
     x, y = np.array(x), np.array(y)
     x = np.atleast_2d(x).T if x.ndim < 2 else x
     y = np.atleast_2d(y).T if y.ndim < 2 else y
     return np.linalg.norm(x - y, axis=1)
 
 
 def enter_exit_target(position, target, max_distance=1):
-    '''Marks when a position has reached a target ("enter")
+    """Marks when a position has reached a target ("enter")
     and when it has left a target ("exit").
 
     The position is considered to have reached a target when it is less than
     the `max_distance` from the target.
 
     Enter and exit times are marked as follows:
      1: entered the target radius
@@ -55,40 +51,41 @@
         How close the position is to the target to be considered at the target.
 
     Returns
     -------
     enter_exit : ndarray, shape (n_time,)
     at_target : ndarray, shape (n_time,)
 
-    '''
+    """
     distance_from_target = paired_distances(position, target)
     at_target = distance_from_target < max_distance
     enter_exit = np.r_[0, np.diff(at_target.astype(float))]
     return enter_exit, at_target
 
 
 def enter_exit_target_dio(dio_indicator):
     at_target = (dio_indicator > 0).astype(np.float16)
     enter_exit = np.r_[0, np.diff(at_target)]
     return enter_exit, at_target
 
 
 def shift_well_enters(enter_exit):
-    '''Shifts the enter times back one time point.'''
+    """Shifts the enter times back one time point."""
     shifted_enter_exit = enter_exit.copy()
     old_ind = np.where(enter_exit > 0)[0]  # positive entries are well-entries
     new_ind = old_ind - 1
     shifted_enter_exit[new_ind] = enter_exit[old_ind]
     shifted_enter_exit[old_ind] = 0
     return shifted_enter_exit
 
 
-def segment_path(time, position, well_locations, epoch_key, animals,
-                 max_distance_from_well=10):
-    '''Label traversals between each well location.
+def segment_path(
+    time, position, well_locations, epoch_key, animals, max_distance_from_well=10
+):
+    """Label traversals between each well location.
 
     Parameters
     ----------
     time : ndarray, shape (n_time,)
     position : ndarray, shape (n_time, n_space)
     well_locations : array_like, shape (n_wells, n_space)
     max_distance_from_well : float, optional
@@ -96,30 +93,37 @@
         than this value.
 
     Returns
     -------
     segments_df : pandas DataFrame, shape (n_segments, 6)
     labeled_segments : pandas DataFrame, shape (n_time,)
 
-    '''
+    """
     try:
+
         def time_func(*args, **kwargs):
             return time
+
         dio_indicator = get_DIO_indicator(epoch_key, animals, time_func)
         well_enter_exit, at_target = np.stack(
-            [enter_exit_target_dio(
-                dio_indicator.loc[:, dio_name].values)
-             for dio_name in _DIO_WELL_ORDER], axis=1)
+            [
+                enter_exit_target_dio(dio_indicator.loc[:, dio_name].values)
+                for dio_name in _DIO_WELL_ORDER
+            ],
+            axis=1,
+        )
     except (FileNotFoundError, TypeError):
-        logger.warn(
-            'No DIO file found, using distance from well to segment trials')
+        logger.warn("No DIO file found, using distance from well to segment trials")
         well_enter_exit, at_target = np.stack(
-            [enter_exit_target(position, np.atleast_2d(well),
-                               max_distance_from_well)
-             for well in well_locations], axis=1)
+            [
+                enter_exit_target(position, np.atleast_2d(well), max_distance_from_well)
+                for well in well_locations
+            ],
+            axis=1,
+        )
     n_wells = len(well_locations)
     well_labels = np.arange(n_wells) + 1
     well_enter_exit = np.sum(well_enter_exit.T * well_labels, axis=1)
     shifted_well_enter_exit = shift_well_enters(well_enter_exit)
     is_segment = ~(np.sum(at_target, axis=0) > 0)
     labeled_segments, n_segment_labels = label(is_segment)
     segment_labels = np.arange(n_segment_labels) + 1
@@ -139,117 +143,124 @@
             start, end = np.nan, np.nan
 
         from_well.append(np.abs(start))
         to_well.append(np.abs(end))
         p = position[is_seg]
         distance_traveled.append(np.sum(paired_distances(p[1:], p[:-1])))
 
-    data = [('start_time', start_time), ('end_time', end_time),
-            ('duration', duration), ('from_well', from_well),
-            ('to_well', to_well),
-            ('distance_traveled', distance_traveled)]
-    index = pd.Index(segment_labels, name='segment')
-    return (pd.DataFrame.from_dict(dict(data)).set_index(index),
-            pd.DataFrame(dict(labeled_segments=labeled_segments), index=time))
+    data = [
+        ("start_time", start_time),
+        ("end_time", end_time),
+        ("duration", duration),
+        ("from_well", from_well),
+        ("to_well", to_well),
+        ("distance_traveled", distance_traveled),
+    ]
+    index = pd.Index(segment_labels, name="segment")
+    return (
+        pd.DataFrame.from_dict(dict(data)).set_index(index),
+        pd.DataFrame(dict(labeled_segments=labeled_segments), index=time),
+    )
 
 
 def find_last_non_center_well(segments_df, segment_ind):
     last_wells = segments_df.iloc[:segment_ind].to_well
     try:
-        return last_wells[last_wells != 'Center'].iloc[-1]
+        return last_wells[last_wells != "Center"].iloc[-1]
     except IndexError:
         # There are no non-center wells. Just return current well.
-        return ''
+        return ""
 
 
 def get_correct_inbound_outbound(segments_df):
     n_segments = segments_df.shape[0]
     task = np.empty((n_segments,), dtype=object)
     turn = np.empty((n_segments,), dtype=object)
     is_correct = np.zeros((n_segments,), dtype=bool)
 
     for segment_ind in np.arange(n_segments):
         cur_segment = segments_df.iloc[segment_ind]
-        if cur_segment.from_well == 'Center':
-            task[segment_ind] = 'Outbound'
-            last_non_center_well = find_last_non_center_well(
-                segments_df, segment_ind)
-            is_correct[segment_ind] = (
-                cur_segment.to_well !=
-                last_non_center_well) & (
-                cur_segment.to_well != 'Center'
+        if cur_segment.from_well == "Center":
+            task[segment_ind] = "Outbound"
+            last_non_center_well = find_last_non_center_well(segments_df, segment_ind)
+            is_correct[segment_ind] = (cur_segment.to_well != last_non_center_well) & (
+                cur_segment.to_well != "Center"
             )
-            if (last_non_center_well != '') | ~is_correct[segment_ind]:
+            if (last_non_center_well != "") | ~is_correct[segment_ind]:
                 turn[segment_ind] = last_non_center_well
             else:
-                is_left_turn = (((cur_segment.from_well == 'Left')
-                                 & (cur_segment.to_well == 'Center')) |
-                                ((cur_segment.from_well == 'Center') &
-                                 (cur_segment.to_well == 'Right')))
+                is_left_turn = (
+                    (cur_segment.from_well == "Left")
+                    & (cur_segment.to_well == "Center")
+                ) | (
+                    (cur_segment.from_well == "Center")
+                    & (cur_segment.to_well == "Right")
+                )
 
-                turn[segment_ind] = 'Left' if is_left_turn else 'Right'
+                turn[segment_ind] = "Left" if is_left_turn else "Right"
         else:
-            task[segment_ind] = 'Inbound'
-            is_correct[segment_ind] = (
-                segments_df.iloc[segment_ind].to_well == 'Center')
+            task[segment_ind] = "Inbound"
+            is_correct[segment_ind] = segments_df.iloc[segment_ind].to_well == "Center"
             turn[segment_ind] = cur_segment.from_well
 
-    segments_df['task'] = task
-    segments_df['is_correct'] = is_correct
-    segments_df['turn'] = turn
+    segments_df["task"] = task
+    segments_df["is_correct"] = is_correct
+    segments_df["turn"] = turn
 
     return segments_df
 
 
-def get_correct_inbound_outbound_dio(segments_df, epoch_key, animals,
-                                     reward_dio_names=_REWARD_DIOS):
+def get_correct_inbound_outbound_dio(
+    segments_df, epoch_key, animals, reward_dio_names=_REWARD_DIOS
+):
     dio = get_DIO(epoch_key, animals)
     dio_is_correct = dio.loc[:, reward_dio_names].sum(axis=1)
-    correct_times = (dio_is_correct.loc[dio_is_correct == 1].index
-                     .total_seconds().values)
+    correct_times = dio_is_correct.loc[dio_is_correct == 1].index.total_seconds().values
     end_times = segments_df.end_time.dt.total_seconds().values
     correct_ind = np.searchsorted(end_times, correct_times) - 1
 
     n_segments = len(segments_df)
     is_correct = np.zeros((n_segments,), dtype=bool)
     turn = np.empty((n_segments,), dtype=object)
 
     is_correct[correct_ind] = True
-    segments_df['is_correct'] = is_correct
+    segments_df["is_correct"] = is_correct
 
     task = np.empty((n_segments,), dtype=object)
     for segment_ind in np.arange(n_segments):
         cur_segment = segments_df.iloc[segment_ind]
-        if segments_df.iloc[segment_ind].from_well == 'Center':
-            task[segment_ind] = 'Outbound'
-            last_non_center_well = find_last_non_center_well(
-                segments_df, segment_ind)
-            if (last_non_center_well != '') | ~is_correct[segment_ind]:
+        if segments_df.iloc[segment_ind].from_well == "Center":
+            task[segment_ind] = "Outbound"
+            last_non_center_well = find_last_non_center_well(segments_df, segment_ind)
+            if (last_non_center_well != "") | ~is_correct[segment_ind]:
                 turn[segment_ind] = last_non_center_well
             else:
-                is_left_turn = (((cur_segment.from_well == 'Left')
-                                 & (cur_segment.to_well == 'Center')) |
-                                ((cur_segment.from_well == 'Center') &
-                                 (cur_segment.to_well == 'Right')))
+                is_left_turn = (
+                    (cur_segment.from_well == "Left")
+                    & (cur_segment.to_well == "Center")
+                ) | (
+                    (cur_segment.from_well == "Center")
+                    & (cur_segment.to_well == "Right")
+                )
 
-                turn[segment_ind] = 'Left' if is_left_turn else 'Right'
+                turn[segment_ind] = "Left" if is_left_turn else "Right"
         else:
-            task[segment_ind] = 'Inbound'
+            task[segment_ind] = "Inbound"
             turn[segment_ind] = cur_segment.from_well
 
-    segments_df['task'] = task
-    segments_df['turn'] = turn
+    segments_df["task"] = task
+    segments_df["turn"] = turn
 
     return segments_df
 
 
 def score_inbound_outbound(
-        segments_df, epoch_key, animals, min_distance_traveled=50,
-        well_names=_WELL_NAMES):
-    '''In the alternating arm task, determines whether the trial should be
+    segments_df, epoch_key, animals, min_distance_traveled=50, well_names=_WELL_NAMES
+):
+    """In the alternating arm task, determines whether the trial should be
     inbound (running to the center arm) or outbound (running to the opposite
     outer arm as before) and if the trial was performed correctly.
 
     Parameters
     ----------
     segments_df : pandas DataFrame
         Output of `segment_path` function.
@@ -259,22 +270,24 @@
 
     Returns
     -------
     segments_df : pandas DataFrame
         Same as the input dataframe but with the wells labeled
         (left, right, center) and columns for `task` (inbound/outbound) and
         `is_correct` (True/False).
-    '''
-    segments_df = (segments_df.copy()
-                   .loc[segments_df.distance_traveled > min_distance_traveled]
-                   .dropna())
+    """
+    segments_df = (
+        segments_df.copy()
+        .loc[segments_df.distance_traveled > min_distance_traveled]
+        .dropna()
+    )
     segments_df = segments_df.assign(
         to_well=lambda df: df.to_well.map(well_names),
-        from_well=lambda df: df.from_well.map(well_names))
+        from_well=lambda df: df.from_well.map(well_names),
+    )
     try:
-        return get_correct_inbound_outbound_dio(
-            segments_df, epoch_key, animals)
+        return get_correct_inbound_outbound_dio(segments_df, epoch_key, animals)
     except (FileNotFoundError, TypeError):
         logger.warn(
-            'No DIO file found, inferring correct inbound/outbound from task '
-            'rules')
+            "No DIO file found, inferring correct inbound/outbound from task " "rules"
+        )
         return get_correct_inbound_outbound(segments_df)
```

### Comparing `loren_frank_data_processing-0.9.9.dev0/loren_frank_data_processing/saving.py` & `loren_frank_data_processing-1.0.1/loren_frank_data_processing/saving.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 from os.path import isfile, join
 
 
 def get_analysis_file_path(processed_data_dir, animal, day, epoch):
-    '''File path for analysis file.
-    '''
-    filename = '{animal}_{day:02d}_{epoch:02d}.nc'.format(
-        animal=animal, day=day, epoch=epoch)
+    """File path for analysis file."""
+    filename = "{animal}_{day:02d}_{epoch:02d}.nc".format(
+        animal=animal, day=day, epoch=epoch
+    )
     return join(processed_data_dir, filename)
 
 
-def save_xarray(processed_data_dir, epoch_key, dataset, group=''):
-    '''Saves xarray data to file corresponding to epoch key
+def save_xarray(processed_data_dir, epoch_key, dataset, group=""):
+    """Saves xarray data to file corresponding to epoch key
 
     Parameters
     ----------
     processed_data_dir : str
         Path to processed data directory
     epoch_key : tuple
         (Animal, day, epoch)
     dataset : xarray Dataset or DataArray
         Data to be saved
     group : str, optional
         HDF5 group name
 
-    '''
+    """
     path = get_analysis_file_path(processed_data_dir, *epoch_key)
-    write_mode = 'a' if isfile(path) else 'w'
+    write_mode = "a" if isfile(path) else "w"
     dataset.to_netcdf(path=path, group=group, mode=write_mode)
```

### Comparing `loren_frank_data_processing-0.9.9.dev0/loren_frank_data_processing/__init__.py` & `loren_frank_data_processing-1.0.1/loren_frank_data_processing/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,30 @@
 # flake8: noqa
 from .core import Animal
-from .multiunit import (get_all_multiunit_indicators, get_multiunit_dataframe,
-                        get_multiunit_dataframe2,
-                        get_multiunit_indicator_dataframe)
-from .neurons import (get_all_spike_indicators, get_spike_indicator_dataframe,
-                      get_spikes_dataframe, make_neuron_dataframe)
-from .position import (get_interpolated_position_dataframe,
-                       get_position_dataframe, get_segments_df)
-from .ripples import (get_computed_consensus_ripple_times,
-                      get_computed_ripples_dataframe)
+from .multiunit import (
+    get_all_multiunit_indicators,
+    get_multiunit_dataframe,
+    get_multiunit_dataframe2,
+    get_multiunit_indicator_dataframe,
+)
+from .neurons import (
+    get_all_spike_indicators,
+    get_spike_indicator_dataframe,
+    get_spikes_dataframe,
+    make_neuron_dataframe,
+)
+from .position import (
+    get_interpolated_position_dataframe,
+    get_position_dataframe,
+    get_segments_df,
+)
+from .ripples import get_computed_consensus_ripple_times, get_computed_ripples_dataframe
 from .saving import get_analysis_file_path, save_xarray
 from .task import make_epochs_dataframe
-from .tetrodes import (get_LFP_dataframe, get_LFPs, get_trial_time,
-                       make_tetrode_dataframe)
+from .tetrodes import (
+    get_LFP_dataframe,
+    get_LFPs,
+    get_trial_time,
+    make_tetrode_dataframe,
+)
 from .utilities import copy_animal, reshape_to_segments
 from .visualization import make_actual_vs_linearized_position_movie
```

### Comparing `loren_frank_data_processing-0.9.9.dev0/loren_frank_data_processing/core.py` & `loren_frank_data_processing-1.0.1/loren_frank_data_processing/core.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-'''Functions for accessing data in the Frank lab format and saving
+"""Functions for accessing data in the Frank lab format and saving
 
-'''
+"""
 from collections import namedtuple
 from logging import getLogger
 from os.path import join
 
 import numpy as np
 import pandas as pd
 from scipy.io import loadmat
 
 logger = getLogger(__name__)
 
-Animal = namedtuple('Animal', {'directory', 'short_name'})
+Animal = namedtuple("Animal", {"directory", "short_name"})
 
 
 def get_data_filename(animal, day, file_type):
-    '''Returns the Matlab file name assuming it is in the Raw Data
+    """Returns the Matlab file name assuming it is in the Raw Data
     directory.
 
     Parameters
     ----------
     animal : namedtuple
         First element is the directory where the animal's data is located.
         The second element is the animal shortened name.
@@ -29,24 +29,23 @@
         Data structure name (e.g. linpos, dio)
 
     Returns
     -------
     filename : str
         Path to data file
 
-    '''
-    filename = '{animal.short_name}{file_type}{day:02d}.mat'.format(
-        animal=animal,
-        file_type=file_type,
-        day=day)
+    """
+    filename = "{animal.short_name}{file_type}{day:02d}.mat".format(
+        animal=animal, file_type=file_type, day=day
+    )
     return join(animal.directory, filename)
 
 
 def get_epochs(animal, day):
-    '''For a given recording day and animal, get the three-element epoch
+    """For a given recording day and animal, get the three-element epoch
     key that uniquely identifys the recording epochs in that day.
 
     Parameters
     ----------
     animal : namedtuple
         First element is the directory where the animal's data is located.
         The second element is the animal shortened name.
@@ -63,28 +62,30 @@
     --------
     >>> from collections import namedtuple
     >>> Animal = namedtuple('Animal', {'directory', 'short_name'})
     >>> animal = Animal(directory='test_dir', short_name='Test')
     >>> day = 2
     >>> get_epochs(animal, day)
 
-    '''
+    """
     try:
-        task_file = loadmat(
-            get_data_filename(animal, day, 'task'))
-        return [(animal, day, ind + 1)
-                for ind, epoch in enumerate(task_file['task'][0, -1][0])]
+        task_file = loadmat(get_data_filename(animal, day, "task"))
+        return [
+            (animal, day, ind + 1)
+            for ind, epoch in enumerate(task_file["task"][0, -1][0])
+        ]
     except (IOError, TypeError):
-        logger.warn('Failed to load file {0}'.format(
-            get_data_filename(animal, day, 'task')))
+        logger.warn(
+            "Failed to load file {0}".format(get_data_filename(animal, day, "task"))
+        )
         exit()
 
 
 def get_data_structure(animal, day, file_type, variable):
-    '''Returns data structures corresponding to the animal, day, file_type
+    """Returns data structures corresponding to the animal, day, file_type
     for all epochs
 
     Parameters
     ----------
     animal : namedtuple
         First element is the directory where the animal's data is located.
         The second element is the animal shortened name.
@@ -96,50 +97,53 @@
         Variable in data structure
 
     Returns
     -------
     variable : list, shape (n_epochs,)
         Elements of list are data structures corresponding to variable
 
-    '''
+    """
     try:
         file = loadmat(get_data_filename(animal, day, file_type))
         n_epochs = file[variable][0, -1].size
-        return [file[variable][0, -1][0, ind]
-                for ind in np.arange(n_epochs)]
+        return [file[variable][0, -1][0, ind] for ind in np.arange(n_epochs)]
     except (IOError, TypeError):
-        logger.warn('Failed to load file: {0}'.format(
-            get_data_filename(animal, day, file_type)))
+        logger.warn(
+            "Failed to load file: {0}".format(get_data_filename(animal, day, file_type))
+        )
         return None
 
 
 def reconstruct_time(start_time, n_samples, sampling_frequency):
-    '''Reconstructs the recording time
+    """Reconstructs the recording time
 
     Parameters
     ----------
     start_time : float
         Start time of recording.
     n_samples : int
         Number of samples in recording.
     sampling_frequency : float
         Number of samples per time
 
     Returns
     -------
     time : pandas Index
 
-    '''
+    """
     return pd.timedelta_range(
-        start=pd.Timedelta(start_time, unit='s'),
-        end=pd.Timedelta(start_time + (n_samples - 1) / sampling_frequency,
-                         unit='s'),
-        periods=n_samples, name='time')
+        start=pd.Timedelta(start_time, unit="s"),
+        end=pd.Timedelta(start_time + (n_samples - 1) / sampling_frequency, unit="s"),
+        periods=n_samples,
+        name="time",
+    )
 
 
 def _convert_to_dict(struct_array):
     try:
-        return {name: struct_array[name].item().item()
-                for name in struct_array.dtype.names
-                if struct_array[name].item().size == 1}
+        return {
+            name: struct_array[name].item().item()
+            for name in struct_array.dtype.names
+            if struct_array[name].item().size == 1
+        }
     except TypeError:
         return {}
```

### Comparing `loren_frank_data_processing-0.9.9.dev0/loren_frank_data_processing/multiunit.py` & `loren_frank_data_processing-1.0.1/loren_frank_data_processing/multiunit.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from os.path import join
 
 import dask
 import numpy as np
 import pandas as pd
 import xarray as xr
+from scipy.io import loadmat
+
 from loren_frank_data_processing.core import get_data_filename, logger
 from loren_frank_data_processing.tetrodes import get_trial_time
-from scipy.io import loadmat
 
 
 def get_multiunit_dataframe(tetrode_key, animals):
-    '''Retrieve the multiunits for each tetrode given a tetrode key
+    """Retrieve the multiunits for each tetrode given a tetrode key
 
     Parameters
     ----------
     tetrode_key : tuple
         Unique key identifying the tetrode. Elements are
         (animal_short_name, day, epoch, tetrode_number).
     animals : dict of named-tuples
@@ -24,38 +25,43 @@
     Returns
     -------
     multiunit_dataframe : pandas dataframe
         The dataframe index is the time at which the multiunit occurred
         (in seconds). THe other values are values that can be used as the
         multiunits.
 
-    '''
-    TO_NANOSECONDS = 1E5
+    """
+    TO_NANOSECONDS = 1e5
     try:
         multiunit_file = loadmat(get_multiunit_filename(tetrode_key, animals))
         multiunit_names = [
-            name[0][0].lower().replace(' ', '_')
-            for name in multiunit_file['filedata'][0, 0]['paramnames']]
-        multiunit_data = multiunit_file['filedata'][0, 0]['params']
+            name[0][0].lower().replace(" ", "_")
+            for name in multiunit_file["filedata"][0, 0]["paramnames"]
+        ]
+        multiunit_data = multiunit_file["filedata"][0, 0]["params"]
         time = pd.TimedeltaIndex(
-            multiunit_data[:, multiunit_names.index('time')].astype(int) *
-            TO_NANOSECONDS, unit='ns', name='time')
+            multiunit_data[:, multiunit_names.index("time")].astype(int)
+            * TO_NANOSECONDS,
+            unit="ns",
+            name="time",
+        )
         is_duplicated = time.duplicated()
 
-        return (pd.DataFrame(multiunit_data, columns=multiunit_names,
-                             index=time)
-                .drop('time', axis=1)
-                .loc[~is_duplicated]
-                .sort_index())
+        return (
+            pd.DataFrame(multiunit_data, columns=multiunit_names, index=time)
+            .drop("time", axis=1)
+            .loc[~is_duplicated]
+            .sort_index()
+        )
     except (FileNotFoundError, TypeError):
         pass
 
 
 def get_multiunit_dataframe2(tetrode_key, animals):
-    '''Retrieve the multiunits for each tetrode given a tetrode key
+    """Retrieve the multiunits for each tetrode given a tetrode key
     This function retrieves data according to Demetris's format.
 
     Parameters
     ----------
     tetrode_key : tuple
         Unique key identifying the tetrode. Elements are
         (animal_short_name, day, epoch, tetrode_number).
@@ -66,66 +72,72 @@
     Returns
     -------
     multiunit_dataframe : pandas dataframe
         The dataframe index is the time at which the multiunit occurred
         (in seconds). THe other values are values that can be used as the
         multiunits.
 
-    '''
+    """
     animal, day, epoch, tetrode_number = tetrode_key
     try:
-        multiunit_file = loadmat(
-            get_data_filename(animals[animal], day, 'marks'))
-        multiunit_data = multiunit_file['marks'][0, -1][0, epoch - 1][
-            0, tetrode_number - 1]
-
-        time = pd.TimedeltaIndex(multiunit_data['times'][0, 0].squeeze(),
-                                 unit='s', name='time')
-        multiunit = multiunit_data['marks'][0, 0].astype(np.float)
-        column_names = ['channel_{number}_max'.format(number=number + 1)
-                        for number in np.arange(multiunit.shape[1])]
+        multiunit_file = loadmat(get_data_filename(animals[animal], day, "marks"))
+        multiunit_data = multiunit_file["marks"][0, -1][0, epoch - 1][
+            0, tetrode_number - 1
+        ]
+
+        time = pd.TimedeltaIndex(
+            multiunit_data["times"][0, 0].squeeze(), unit="s", name="time"
+        )
+        multiunit = multiunit_data["marks"][0, 0].astype(float)
+        column_names = [
+            "channel_{number}_max".format(number=number + 1)
+            for number in np.arange(multiunit.shape[1])
+        ]
         is_duplicated = time.duplicated()
-        return (pd.DataFrame(multiunit, columns=column_names, index=time)
-                .loc[~is_duplicated]
-                .sort_index())
-    except (FileNotFoundError, TypeError):
-        logger.warning('Failed to load file: {0}'.format(
-            get_data_filename(animals[animal], day, 'marks')))
+        return (
+            pd.DataFrame(multiunit, columns=column_names, index=time)
+            .loc[~is_duplicated]
+            .sort_index()
+        )
+    except (FileNotFoundError, TypeError, IndexError):
+        logger.warning(
+            "Failed to load file: {0}".format(
+                get_data_filename(animals[animal], day, "marks")
+            )
+        )
 
 
 def get_multiunit_filename(tetrode_key, animals):
-    '''Path for the multiunits for a particular tetrode.
+    """Path for the multiunits for a particular tetrode.
 
     Parameters
     ----------
     tetrode_key : tuple
         Unique key identifying the tetrode. Elements are
         (animal_short_name, day, epoch, tetrode_number).
     animals : dict of named-tuples
         Dictionary containing information about the directory for each
         animal. The key is the animal_short_name.
 
     Returns
     -------
     multiunit_filename : str
 
-    '''
+    """
     animal, day, _, tetrode_number = tetrode_key
-    filename = ('{animal.short_name}marks{day:02d}-'
-                '{tetrode_number:02d}.mat').format(
-        animal=animals[animal],
-        day=day,
-        tetrode_number=tetrode_number
+    filename = ("{animal.short_name}marks{day:02d}-" "{tetrode_number:02d}.mat").format(
+        animal=animals[animal], day=day, tetrode_number=tetrode_number
     )
-    return join(animals[animal].directory, 'EEG', filename)
+    return join(animals[animal].directory, "EEG", filename)
 
 
-def get_multiunit_indicator_dataframe(tetrode_key, animals,
-                                      time_function=get_trial_time):
-    '''A time series where a value indicates multiunit activity at that time and
+def get_multiunit_indicator_dataframe(
+    tetrode_key, animals, time_function=get_trial_time
+):
+    """A time series where a value indicates multiunit activity at that time and
     NaN indicates no multiunit activity at that time.
 
     Parameters
     ----------
     tetrode_key : tuple
         Unique key identifying the tetrode. Elements are
         (animal_short_name, day, epoch, tetrode_number).
@@ -137,51 +149,51 @@
         defines the time the multiunits are relative to. Defaults to using
         the time the LFPs are sampled at.
 
     Returns
     -------
     multiunit_indicator : pandas.DataFrame, shape (n_time, n_features)
 
-    '''
+    """
     time = time_function(tetrode_key[:3], animals)
     try:
-        multiunit_dataframe = (get_multiunit_dataframe(tetrode_key, animals)
-                               .loc[time.min():time.max()])
+        multiunit_dataframe = get_multiunit_dataframe(tetrode_key, animals).loc[
+            time.min() : time.max()
+        ]
     except AttributeError:
-        multiunit_dataframe = get_multiunit_dataframe2(tetrode_key, animals)
-    time_index = np.digitize(multiunit_dataframe.index.total_seconds(),
-                             time.total_seconds())
-    time_index[time_index >= len(time)] = len(time) - 1
-    return (multiunit_dataframe.groupby(time[time_index]).mean()
-            .reindex(index=time))
+        multiunit_dataframe = get_multiunit_dataframe2(tetrode_key, animals).loc[
+            time.min() : time.max()
+        ]
+    time_index = np.digitize(
+        multiunit_dataframe.index.total_seconds(), time.total_seconds()[1:-1]
+    )
+    return multiunit_dataframe.groupby(time[time_index]).mean().reindex(index=time)
 
 
 @dask.delayed
 def _get_indicator(tetrode_key, animals, time):
     try:
-        df = (get_multiunit_dataframe(tetrode_key, animals)
-              .loc[time.min():time.max()])
+        df = get_multiunit_dataframe(tetrode_key, animals).loc[time.min() : time.max()]
     except AttributeError:
-        df = (get_multiunit_dataframe2(tetrode_key, animals)
-              .loc[time.min():time.max()])
+        df = get_multiunit_dataframe2(tetrode_key, animals).loc[time.min() : time.max()]
 
-    time_index = np.digitize(df.index.total_seconds(),
-                             time.total_seconds())
-    time_index[time_index >= len(time)] = len(time) - 1
+    time_index = np.digitize(df.index.total_seconds(), time.total_seconds()[1:-1])
 
-    return (df.groupby(time[time_index]).mean()
-            .reindex(index=time)
-            .to_xarray()
-            .to_array('features'))
+    return (
+        df.groupby(time[time_index])
+        .mean()
+        .reindex(index=time)
+        .to_xarray()
+        .to_array("features")
+    )
 
 
-def get_all_multiunit_indicators(tetrode_keys, animals,
-                                 time_function=get_trial_time):
+def get_all_multiunit_indicators(tetrode_keys, animals, time_function=get_trial_time):
     time = time_function(tetrode_keys[0][:3], animals)
     multiunit_dfs = []
 
     for tetrode_key in tetrode_keys:
         multiunit_dfs.append(_get_indicator(tetrode_key, animals, time))
 
-    return (xr.concat(
-        dask.compute(*multiunit_dfs, scheduler='threads'), dim='tetrodes')
-        .transpose('time', 'features', 'tetrodes'))
+    return xr.concat(
+        dask.compute(*multiunit_dfs, scheduler="threads"), dim="tetrodes"
+    ).transpose("time", "features", "tetrodes")
```

### Comparing `loren_frank_data_processing-0.9.9.dev0/loren_frank_data_processing/visualization.py` & `loren_frank_data_processing-1.0.1/loren_frank_data_processing/visualization.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,114 +1,126 @@
 import matplotlib.animation as animation
 import matplotlib.pyplot as plt
 import numpy as np
+
 from loren_frank_data_processing.track_segment_classification import (
-    get_track_segments_from_graph, plot_track, project_points_to_segment)
+    get_track_segments_from_graph,
+    plot_track,
+    project_points_to_segment,
+)
 
 
 def _get_projected_track_position(track_graph, track_segment_id, position):
     track_segment_id[np.isnan(track_segment_id)] = 0
     track_segment_id = track_segment_id.astype(int)
 
     track_segments = get_track_segments_from_graph(track_graph)
-    projected_track_position = project_points_to_segment(
-        track_segments, position)
+    projected_track_position = project_points_to_segment(track_segments, position)
     n_time = projected_track_position.shape[0]
-    return projected_track_position[(
-        np.arange(n_time), track_segment_id)]
+    return projected_track_position[(np.arange(n_time), track_segment_id)]
 
 
 def make_actual_vs_linearized_position_movie(
-        track_graph, position_df, time_slice=None,
-        movie_name='actual_vs_linearized', frame_rate=33):
-    '''
+    track_graph,
+    position_df,
+    time_slice=None,
+    movie_name="actual_vs_linearized",
+    frame_rate=33,
+):
+    """
 
     Parameters
     ----------
     track_graph : networkx.Graph
     position_df : pandas.DataFrame
     time_slice : slice or None, optional
     movie_name : str, optional
     frame_rate : float, optional
         Frames per second.
-    '''
+    """
 
-    all_position = position_df.loc[:, ['x_position', 'y_position']].values
+    all_position = position_df.loc[:, ["x_position", "y_position"]].values
     all_linear_position = position_df.linear_position.values
-    all_time = position_df.index.values / np.timedelta64(1, 's')
+    all_time = position_df.index.values / np.timedelta64(1, "s")
 
     if time_slice is None:
         position = all_position
         track_segment_id = position_df.track_segment_id.values
         linear_position = all_linear_position
         time = all_time
     else:
         position = all_position[time_slice]
         track_segment_id = position_df.iloc[time_slice].track_segment_id.values
         linear_position = all_linear_position[time_slice]
         time = all_time[time_slice]
 
     projected_track_position = _get_projected_track_position(
-        track_graph, track_segment_id, position)
+        track_graph, track_segment_id, position
+    )
 
     # Set up formatting for the movie files
-    Writer = animation.writers['ffmpeg']
-    writer = Writer(fps=15, metadata=dict(artist='Me'), bitrate=1800)
+    Writer = animation.writers["ffmpeg"]
+    writer = Writer(fps=15, metadata=dict(artist="Me"), bitrate=1800)
 
-    fig, axes = plt.subplots(1, 2, figsize=(21, 7), constrained_layout=True,
-                             gridspec_kw={'width_ratios': [2, 1]})
+    fig, axes = plt.subplots(
+        1,
+        2,
+        figsize=(21, 7),
+        constrained_layout=True,
+        gridspec_kw={"width_ratios": [2, 1]},
+    )
 
     # Subplot 1
-    axes[0].scatter(all_time, all_linear_position, color='lightgrey',
-                    zorder=0, s=10)
+    axes[0].scatter(all_time, all_linear_position, color="lightgrey", zorder=0, s=10)
     axes[0].set_xlim((all_time.min(), all_time.max()))
     axes[0].set_ylim((all_linear_position.min(), all_linear_position.max()))
-    linear_head = axes[0].scatter([], [], s=100, zorder=101, color='b')
+    linear_head = axes[0].scatter([], [], s=100, zorder=101, color="b")
 
-    axes[0].set_xlabel('Time [s]')
-    axes[0].set_ylabel('Position [cm]')
-    axes[0].set_title('Linearized Position')
+    axes[0].set_xlabel("Time [s]")
+    axes[0].set_ylabel("Position [cm]")
+    axes[0].set_title("Linearized Position")
 
-    axes[1].plot(all_position[:, 0], all_position[:, 1], color='lightgrey',
-                 zorder=-10)
+    axes[1].plot(all_position[:, 0], all_position[:, 1], color="lightgrey", zorder=-10)
     plot_track(track_graph, ax=axes[1])
-    plt.axis('off')
+    plt.axis("off")
 
     # Subplot 2
-    axes[1].set_xlim(all_position[:, 0].min() - 10,
-                     all_position[:, 0].max() + 10)
-    axes[1].set_ylim(all_position[:, 1].min() - 10,
-                     all_position[:, 1].max() + 10)
-
-    actual_line, = axes[1].plot(
-        [], [], 'g-', label='actual position', linewidth=3, zorder=101)
-    actual_head = axes[1].scatter([], [], s=80, zorder=101, color='g')
-
-    predicted_line, = axes[1].plot(
-        [], [], 'b-', label='linearized position', linewidth=3, zorder=102)
-    predicted_head = axes[1].scatter([], [], s=80, zorder=102, color='b')
+    axes[1].set_xlim(all_position[:, 0].min() - 10, all_position[:, 0].max() + 10)
+    axes[1].set_ylim(all_position[:, 1].min() - 10, all_position[:, 1].max() + 10)
+
+    (actual_line,) = axes[1].plot(
+        [], [], "g-", label="actual position", linewidth=3, zorder=101
+    )
+    actual_head = axes[1].scatter([], [], s=80, zorder=101, color="g")
+
+    (predicted_line,) = axes[1].plot(
+        [], [], "b-", label="linearized position", linewidth=3, zorder=102
+    )
+    predicted_head = axes[1].scatter([], [], s=80, zorder=102, color="b")
 
     axes[1].legend()
-    axes[1].set_xlabel('x-position')
-    axes[1].set_ylabel('y-position')
-    axes[1].set_title('Linearized vs. Actual Position')
+    axes[1].set_xlabel("x-position")
+    axes[1].set_ylabel("y-position")
+    axes[1].set_title("Linearized vs. Actual Position")
 
     def _update_plot(time_ind):
         start_ind = max(0, time_ind - 33)
         time_slice = slice(start_ind, time_ind)
 
-        linear_head.set_offsets(
-            np.array((time[time_ind], linear_position[time_ind])))
+        linear_head.set_offsets(np.array((time[time_ind], linear_position[time_ind])))
 
         actual_line.set_data(position[time_slice, 0], position[time_slice, 1])
         actual_head.set_offsets(position[time_ind])
 
-        predicted_line.set_data(projected_track_position[time_slice, 0],
-                                projected_track_position[time_slice, 1])
+        predicted_line.set_data(
+            projected_track_position[time_slice, 0],
+            projected_track_position[time_slice, 1],
+        )
         predicted_head.set_offsets(projected_track_position[time_ind])
 
         return actual_line, predicted_line
 
     n_time = position.shape[0]
-    line_ani = animation.FuncAnimation(fig, _update_plot, frames=n_time,
-                                       interval=1000 / frame_rate, blit=True)
-    line_ani.save(movie_name + '.mp4', writer=writer)
+    line_ani = animation.FuncAnimation(
+        fig, _update_plot, frames=n_time, interval=1000 / frame_rate, blit=True
+    )
+    line_ani.save(movie_name + ".mp4", writer=writer)
```

### Comparing `loren_frank_data_processing-0.9.9.dev0/loren_frank_data_processing/neurons.py` & `loren_frank_data_processing-1.0.1/loren_frank_data_processing/neurons.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,208 +1,264 @@
-'''Loads general information about each spike-sorted neuron, spike times, or
+"""Loads general information about each spike-sorted neuron, spike times, or
 spike indicators.
-'''
+"""
 
 from os.path import join
 
-import dask
 import numpy as np
 import pandas as pd
 from scipy.io import loadmat
 
 from .core import _convert_to_dict, get_data_filename, logger
 from .tetrodes import get_trial_time
 
 
-def make_neuron_dataframe(animals):
-    '''Information about all recorded neurons such as brain area.
+def make_neuron_dataframe(animals, exclude_animals=None):
+    """Information about all recorded neurons such as brain area.
 
     The index of the dataframe corresponds to the unique key for that neuron
     and can be used to load spiking information.
 
     Parameters
     ----------
     animals : dict of named-tuples
         Dictionary containing information about the directory for each
         animal. The key is the animal_short_name.
+    exclude_animals : list or None
+        Filter animals dictionary
 
     Returns
     -------
     neuron_information : pandas.DataFrame
 
-    '''
-    neuron_file_names = [(get_neuron_info_path(animals[animal]), animal)
-                         for animal in animals]
-    neuron_data = [(loadmat(file_name[0]), file_name[1])
-                   for file_name in neuron_file_names]
-    return pd.concat([
-        convert_neuron_epoch_to_dataframe(
-            epoch, animal, day_ind + 1, epoch_ind + 1)
-        for cellfile, animal in neuron_data
-        for day_ind, day in enumerate(cellfile['cellinfo'].T)
-        for epoch_ind, epoch in enumerate(day[0].T)
-    ]).sort_index()
+    """
+    if exclude_animals is None:
+        exclude_animals = []
+    neuron_file_names = [
+        (get_neuron_info_path(animals[animal]), animal)
+        for animal in animals
+        if animal not in exclude_animals
+    ]
+    neuron_data = [
+        (loadmat(file_name[0]), file_name[1]) for file_name in neuron_file_names
+    ]
+    return pd.concat(
+        [
+            convert_neuron_epoch_to_dataframe(epoch, animal, day_ind + 1, epoch_ind + 1)
+            for cellfile, animal in neuron_data
+            for day_ind, day in enumerate(cellfile["cellinfo"].T)
+            for epoch_ind, epoch in enumerate(day[0].T)
+        ]
+    ).sort_index()
 
 
 def get_spikes_dataframe(neuron_key, animals):
-    '''Spike times for a particular neuron.
+    """Spike times for a particular neuron.
 
     Parameters
     ----------
     neuron_key : tuple
         Unique key identifying that neuron. Elements of the tuple are
         (animal_short_name, day, epoch, tetrode_number, neuron_number).
         Key can be retrieved from `make_neuron_dataframe` function.
     animals : dict of named-tuples
         Dictionary containing information about the directory for each
         animal. The key is the animal_short_name.
 
     Returns
     -------
     spikes_dataframe : pandas.DataFrame
-    '''
+    """
     animal, day, epoch, tetrode_number, neuron_number = neuron_key
     try:
-        neuron_file = loadmat(
-            get_data_filename(animals[animal], day, 'spikes'))
+        neuron_file = loadmat(get_data_filename(animals[animal], day, "spikes"))
     except (FileNotFoundError, TypeError):
-        logger.warning('Failed to load file: {0}'.format(
-            get_data_filename(animals[animal], day, 'spikes')))
+        logger.warning(
+            "Failed to load file: {0}".format(
+                get_data_filename(animals[animal], day, "spikes")
+            )
+        )
     try:
-        spike_time = neuron_file['spikes'][0, -1][0, epoch - 1][
-            0, tetrode_number - 1][0, neuron_number - 1][0]['data'][0][
-            :, 0]
-        spike_time = pd.TimedeltaIndex(spike_time, unit='s', name='time')
+        spike_time = neuron_file["spikes"][0, -1][0, epoch - 1][0, tetrode_number - 1][
+            0, neuron_number - 1
+        ][0]["data"][0][:, 0]
+        spike_time = pd.TimedeltaIndex(spike_time, unit="s", name="time")
     except IndexError:
         spike_time = []
     return pd.Series(
-        np.ones_like(spike_time, dtype=int), index=spike_time,
-        name='{0}_{1:02d}_{2:02}_{3:03}_{4:03}'.format(*neuron_key))
+        np.ones_like(spike_time, dtype=int),
+        index=spike_time,
+        name="{0}_{1:02d}_{2:02}_{3:03}_{4:03}".format(*neuron_key),
+    )
 
 
-def get_spike_indicator_dataframe(neuron_key, animals,
-                                  time_function=get_trial_time):
-    '''A time series where 1 indicates a spike at that time and 0 indicates no
+def get_spike_indicator_dataframe(neuron_key, animals, time_function=get_trial_time):
+    """A time series where 1 indicates a spike at that time and 0 indicates no
     spike at that time.
 
     Parameters
     ----------
     neuron_key : tuple
         Unique key identifying that neuron. Elements of the tuple are
         (animal_short_name, day, epoch, tetrode_number, neuron_number).
         Key can be retrieved from `make_neuron_dataframe` function.
     animals : dict of named-tuples
         Dictionary containing information about the directory for each
         animal. The key is the animal_short_name.
     time_function : function, optional
         Function that take an epoch key (animal_short_name, day, epoch) that
         defines the time the multiunits are relative to. Defaults to using
-        the time the LFPs are sampled at.
+        the time the LFPs are s ampled at.
 
     Returns
     ---
 
-    '''
+    """
     time = time_function(neuron_key[:3], animals)
-    spikes_df = get_spikes_dataframe(neuron_key, animals)
-    time_index = np.digitize(spikes_df.index.total_seconds(),
-                             time.total_seconds())
-    time_index[time_index >= len(time)] = len(time) - 1
-    return (spikes_df.groupby(time[time_index]).sum()
-            .reindex(index=time, fill_value=0))
-
+    time_in_seconds = time.total_seconds()
 
-@dask.delayed
-def _get_indicator(neuron_key, animals, time):
-    n_time = time.size
     spikes_df = get_spikes_dataframe(neuron_key, animals)
-    try:
-        spike_time_ind = np.digitize(
-            spikes_df.index.total_seconds(), time.total_seconds())
-        spike_time_ind = spike_time_ind[spike_time_ind < n_time]
-        return (spikes_df.iloc[spike_time_ind < n_time]
-                .groupby(time[spike_time_ind]).sum()
-                .reindex(index=time, fill_value=0))
-    except AttributeError:
-        logger.debug(f'No spikes. Skipping...')
+    spike_times = spikes_df.index.total_seconds()
+    is_in_time = (spike_times >= time_in_seconds[0]) & (
+        spike_times < time_in_seconds[-1]
+    )
+    time_index = np.digitize(spike_times[is_in_time], time_in_seconds[1:-1])
+    return (
+        spikes_df.groupby(time[time_index].to_pytimedelta())
+        .sum()
+        .reindex(index=time, fill_value=0)
+    )
 
 
-def get_all_spike_indicators(neuron_keys, animals,
-                             time_function=get_trial_time):
+def get_all_spike_indicators(neuron_keys, animals, time_function=get_trial_time):
     time = time_function(neuron_keys[0][:3], animals)
-    spikes_dfs = []
+    time_in_seconds = time.total_seconds()
+
+    animal, day, _, _, _ = neuron_keys[0]
+    try:
+        neuron_file = loadmat(get_data_filename(animals[animal], day, "spikes"))
+    except (FileNotFoundError, TypeError):
+        logger.warning(
+            "Failed to load file: {0}".format(
+                get_data_filename(animals[animal], day, "spikes")
+            )
+        )
+
+    neuron_names = []
+    bin_counts = []
     for neuron_key in neuron_keys:
-        spikes_dfs.append(_get_indicator(neuron_key, animals, time))
+        animal, day, epoch, tetrode_number, neuron_number = neuron_key
+        neuron_names.append(
+            f"{animal}_{day:02d}_{epoch:02}_{tetrode_number:03}_{neuron_number:03}"
+        )
+        try:
+            spike_times = neuron_file["spikes"][0, -1][0, epoch - 1][
+                0, tetrode_number - 1
+            ][0, neuron_number - 1][0]["data"][0][:, 0]
+            is_in_time = (spike_times >= time_in_seconds[0]) & (
+                spike_times < time_in_seconds[-1]
+            )
+            bin_counts.append(
+                np.bincount(
+                    np.digitize(spike_times[is_in_time], time_in_seconds[1:-1]),
+                    minlength=time.shape[0],
+                )
+            )
+        except IndexError:
+            bin_counts.append(np.zeros_like(time, dtype=float))
 
-    return pd.concat(dask.compute(*spikes_dfs, scheduler='threads'), axis=1)
+    return pd.DataFrame(np.stack(bin_counts, axis=1), columns=neuron_names, index=time)
 
 
-def convert_neuron_epoch_to_dataframe(tetrodes_in_epoch, animal, day,
-                                      epoch):
-    '''
+def convert_neuron_epoch_to_dataframe(tetrodes_in_epoch, animal, day, epoch):
+    """
     Given an neuron data structure, return a cleaned up DataFrame
-    '''
-    DROP_COLUMNS = ['ripmodtag', 'thetamodtag', 'runripmodtag',
-                    'postsleepripmodtag', 'presleepripmodtag',
-                    'runthetamodtag', 'ripmodtag2', 'runripmodtag2',
-                    'postsleepripmodtag2', 'presleepripmodtag2',
-                    'ripmodtype', 'runripmodtype', 'postsleepripmodtype',
-                    'presleepripmodtype', 'FStag', 'ripmodtag3',
-                    'runripmodtag3', 'ripmodtype3', 'runripmodtype3',
-                    'tag', 'typetag', 'runripmodtype2',
-                    'tag2', 'ripmodtype2', 'descrip']
-
-    NEURON_INDEX = ['animal', 'day', 'epoch',
-                    'tetrode_number', 'neuron_number']
-
-    neuron_dict_list = [_add_to_dict(
-        _convert_to_dict(neuron), tetrode_ind, neuron_ind)
-        for tetrode_ind, tetrode in enumerate(
-        tetrodes_in_epoch[0][0])
+    """
+    DROP_COLUMNS = [
+        "ripmodtag",
+        "thetamodtag",
+        "runripmodtag",
+        "postsleepripmodtag",
+        "presleepripmodtag",
+        "runthetamodtag",
+        "ripmodtag2",
+        "runripmodtag2",
+        "postsleepripmodtag2",
+        "presleepripmodtag2",
+        "ripmodtype",
+        "runripmodtype",
+        "postsleepripmodtype",
+        "presleepripmodtype",
+        "FStag",
+        "ripmodtag3",
+        "runripmodtag3",
+        "ripmodtype3",
+        "runripmodtype3",
+        "tag",
+        "typetag",
+        "runripmodtype2",
+        "tag2",
+        "ripmodtype2",
+        "descrip",
+    ]
+
+    NEURON_INDEX = ["animal", "day", "epoch", "tetrode_number", "neuron_number"]
+
+    neuron_dict_list = [
+        _add_to_dict(_convert_to_dict(neuron), tetrode_ind, neuron_ind)
+        for tetrode_ind, tetrode in enumerate(tetrodes_in_epoch[0][0])
         for neuron_ind, neuron in enumerate(tetrode[0])
         if neuron.size > 0
     ]
     try:
-        return (pd.DataFrame(neuron_dict_list)
-                  .drop(DROP_COLUMNS, axis=1, errors='ignore')
-                  .assign(animal=animal)
-                  .assign(day=day)
-                  .assign(epoch=epoch)
-                  .assign(neuron_id=_get_neuron_id)
-                # set index to identify rows
-                  .set_index(NEURON_INDEX)
-                  .sort_index())
+        return (
+            pd.DataFrame(neuron_dict_list)
+            .drop(DROP_COLUMNS, axis=1, errors="ignore")
+            .assign(animal=animal)
+            .assign(day=day)
+            .assign(epoch=epoch)
+            .assign(neuron_id=_get_neuron_id)
+            # set index to identify rows
+            .set_index(NEURON_INDEX)
+            .sort_index()
+        )
     except AttributeError:
-        logger.debug(f'Neuron info {animal}, {day}, {epoch} not processed')
+        logger.debug(f"Neuron info {animal}, {day}, {epoch} not processed")
 
 
 def get_neuron_info_path(animal):
-    '''Returns the path to the neuron info matlab file
+    """Returns the path to the neuron info matlab file
 
     Parameters
     ----------
     animal : namedtuple
         First element is the directory where the animal's data is located.
         The second element is the animal shortened name.
 
     Returns
     -------
     path : str
 
-    '''
-    filename = '{animal.short_name}cellinfo.mat'.format(animal=animal)
+    """
+    filename = "{animal.short_name}cellinfo.mat".format(animal=animal)
     return join(animal.directory, filename)
 
 
 def _get_neuron_id(dataframe):
-    '''Unique identifier string for a neuron'''
-    return (dataframe.animal + '_' +
-            dataframe.day.map('{:02d}'.format) + '_' +
-            dataframe.epoch.map('{:02}'.format) + '_' +
-            dataframe.tetrode_number.map('{:03}'.format) + '_' +
-            dataframe.neuron_number.map('{:03}'.format))
+    """Unique identifier string for a neuron"""
+    return (
+        dataframe.animal
+        + "_"
+        + dataframe.day.map("{:02d}".format)
+        + "_"
+        + dataframe.epoch.map("{:02}".format)
+        + "_"
+        + dataframe.tetrode_number.map("{:03}".format)
+        + "_"
+        + dataframe.neuron_number.map("{:03}".format)
+    )
 
 
 def _add_to_dict(dictionary, tetrode_ind, neuron_ind):
-    dictionary['tetrode_number'] = tetrode_ind + 1
-    dictionary['neuron_number'] = neuron_ind + 1
+    dictionary["tetrode_number"] = tetrode_ind + 1
+    dictionary["neuron_number"] = neuron_ind + 1
     return dictionary
```

### Comparing `loren_frank_data_processing-0.9.9.dev0/loren_frank_data_processing/position.py` & `loren_frank_data_processing-1.0.1/loren_frank_data_processing/position.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,57 +1,71 @@
 import networkx as nx
 import numpy as np
 import pandas as pd
 from scipy.ndimage.filters import gaussian_filter1d
 
 from .core import get_data_structure
 from .tetrodes import get_trial_time
-from .track_segment_classification import (calculate_linear_distance,
-                                           classify_track_segments)
+from .track_segment_classification import (
+    calculate_linear_distance,
+    classify_track_segments,
+)
 from .well_traversal_classification import score_inbound_outbound, segment_path
 
 EDGE_ORDER = [0, 2, 4, 1, 3]
 EDGE_SPACING = [15, 0, 15, 0]
 
 
 def _get_pos_dataframe(epoch_key, animals):
     animal, day, epoch = epoch_key
-    struct = get_data_structure(animals[animal], day, 'pos', 'pos')[epoch - 1]
-    position_data = struct['data'][0, 0]
-    FIELD_NAMES = ['time', 'x_position', 'y_position', 'head_direction',
-                   'speed', 'smoothed_x_position', 'smoothed_y_position',
-                   'smoothed_head_direction', 'smoothed_speed']
-    time = pd.TimedeltaIndex(
-        position_data[:, 0], unit='s', name='time')
+    struct = get_data_structure(animals[animal], day, "pos", "pos")[epoch - 1]
+    position_data = struct["data"][0, 0]
+    FIELD_NAMES = [
+        "time",
+        "x_position",
+        "y_position",
+        "head_direction",
+        "speed",
+        "smoothed_x_position",
+        "smoothed_y_position",
+        "smoothed_head_direction",
+        "smoothed_speed",
+    ]
+    time = pd.TimedeltaIndex(position_data[:, 0], unit="s", name="time")
     n_cols = position_data.shape[1]
 
     if n_cols > 5:
         # Use the smoothed data if available
-        NEW_NAMES = {'smoothed_x_position': 'x_position',
-                     'smoothed_y_position': 'y_position',
-                     'smoothed_head_direction': 'head_direction',
-                     'smoothed_speed': 'speed'}
-        return (pd.DataFrame(
-            position_data[:, 5:], columns=FIELD_NAMES[5:], index=time)
-            .rename(columns=NEW_NAMES))
+        NEW_NAMES = {
+            "smoothed_x_position": "x_position",
+            "smoothed_y_position": "y_position",
+            "smoothed_head_direction": "head_direction",
+            "smoothed_speed": "speed",
+        }
+        return pd.DataFrame(
+            position_data[:, 5:9], columns=FIELD_NAMES[5:9], index=time
+        ).rename(columns=NEW_NAMES)
     else:
-        return pd.DataFrame(position_data[:, 1:5], columns=FIELD_NAMES[1:5],
-                            index=time)
+        return pd.DataFrame(position_data[:, 1:5], columns=FIELD_NAMES[1:5], index=time)
 
 
-def get_position_dataframe(epoch_key, animals, use_hmm=True,
-                           max_distance_from_well=5,
-                           route_euclidean_distance_scaling=1,
-                           min_distance_traveled=50,
-                           sensor_std_dev=5,
-                           diagonal_bias=1E-1,
-                           edge_spacing=EDGE_SPACING,
-                           edge_order=EDGE_ORDER,
-                           skip_linearization=False):
-    '''Returns a list of position dataframes with a length corresponding
+def get_position_dataframe(
+    epoch_key,
+    animals,
+    use_hmm=True,
+    max_distance_from_well=5,
+    route_euclidean_distance_scaling=1,
+    min_distance_traveled=50,
+    sensor_std_dev=5,
+    diagonal_bias=1e-1,
+    edge_spacing=EDGE_SPACING,
+    edge_order=EDGE_ORDER,
+    skip_linearization=False,
+):
+    """Returns a list of position dataframes with a length corresponding
      to the number of epochs in the epoch key -- either a tuple or a
     list of tuples with the format (animal, day, epoch_number)
 
     Parameters
     ----------
     epoch_key : tuple
         Unique key identifying a recording epoch. Elements are
@@ -62,35 +76,43 @@
 
     Returns
     -------
     position : pandas dataframe
         Contains information about the animal's position, head direction,
         and speed.
 
-    '''
+    """
     position_df = _get_pos_dataframe(epoch_key, animals)
     if not skip_linearization:
         if use_hmm:
             position_df = _get_linear_position_hmm(
-                epoch_key, animals, position_df,
-                max_distance_from_well, route_euclidean_distance_scaling,
-                min_distance_traveled, sensor_std_dev, diagonal_bias,
-                edge_order=edge_order, edge_spacing=edge_spacing)
+                epoch_key,
+                animals,
+                position_df,
+                max_distance_from_well,
+                route_euclidean_distance_scaling,
+                min_distance_traveled,
+                sensor_std_dev,
+                diagonal_bias,
+                edge_order=edge_order,
+                edge_spacing=edge_spacing,
+            )
         else:
             linear_position_df = _get_linpos_dataframe(
-                epoch_key, animals, edge_order=edge_order,
-                edge_spacing=edge_spacing)
+                epoch_key, animals, edge_order=edge_order, edge_spacing=edge_spacing
+            )
             position_df = position_df.join(linear_position_df)
 
     return position_df
 
 
-def _get_linpos_dataframe(epoch_key, animals, edge_spacing=EDGE_SPACING,
-                          edge_order=EDGE_ORDER):
-    '''The time series of linearized (1D) positions of the animal for a given
+def _get_linpos_dataframe(
+    epoch_key, animals, edge_spacing=EDGE_SPACING, edge_order=EDGE_ORDER
+):
+    """The time series of linearized (1D) positions of the animal for a given
     epoch.
 
     Parameters
     ----------
     epoch_key : tuple
         Unique key identifying a recording epoch. Elements are
         (animal, day, epoch)
@@ -98,82 +120,93 @@
         Dictionary containing information about the directory for each
         animal. The key is the animal_short_name.
 
     Returns
     -------
     linear_position : pandas.DataFrame
 
-    '''
+    """
     animal, day, epoch = epoch_key
-    struct = get_data_structure(
-        animals[animal], day, 'linpos', 'linpos')[epoch - 1][0][0][
-            'statematrix']
-    INCLUDE_FIELDS = ['traj', 'lindist', 'linearVelocity', 'segmentIndex']
-    time = pd.TimedeltaIndex(struct['time'][0][0].flatten(), unit='s',
-                             name='time')
-    new_names = {'time': 'time',
-                 'traj': 'labeled_segments',
-                 'lindist': 'linear_distance',
-                 'linearVelocity': 'linear_velocity',
-                 'segmentIndex': 'track_segment_id'}
-    data = {new_names[name]: struct[name][0][0][:, 0]
-            for name in struct.dtype.names
-            if name in INCLUDE_FIELDS}
+    struct = get_data_structure(animals[animal], day, "linpos", "linpos")[epoch - 1][0][
+        0
+    ]["statematrix"]
+    INCLUDE_FIELDS = ["traj", "lindist", "linearVelocity", "segmentIndex"]
+    time = pd.TimedeltaIndex(struct["time"][0][0].flatten(), unit="s", name="time")
+    new_names = {
+        "time": "time",
+        "traj": "labeled_segments",
+        "lindist": "linear_distance",
+        "linearVelocity": "linear_velocity",
+        "segmentIndex": "track_segment_id",
+    }
+    data = {
+        new_names[name]: struct[name][0][0][:, 0]
+        for name in struct.dtype.names
+        if name in INCLUDE_FIELDS
+    }
     position_df = pd.DataFrame(data, index=time)
     SEGMENT_ID_TO_ARM_NAME = {
-        1: 'Center Arm',
-        2: 'Left Arm',
-        3: 'Left Arm',
-        4: 'Right Arm',
-        5: 'Right Arm',
+        1: "Center Arm",
+        2: "Left Arm",
+        3: "Left Arm",
+        4: "Right Arm",
+        5: "Right Arm",
     }
     position_df = position_df.assign(
         arm_name=lambda df: df.track_segment_id.map(SEGMENT_ID_TO_ARM_NAME)
     )
     track_graph, center_well_id = make_track_graph(epoch_key, animals)
-    position_df['linear_position'] = _calulcate_linear_position(
+    position_df["linear_position"] = _calulcate_linear_position(
         position_df.linear_distance.values,
-        position_df.track_segment_id.values, track_graph, center_well_id,
-        edge_order=edge_order, edge_spacing=edge_spacing)
+        position_df.track_segment_id.values,
+        track_graph,
+        center_well_id,
+        edge_order=edge_order,
+        edge_spacing=edge_spacing,
+    )
     return position_df.assign(linear_speed=np.abs(position_df.linear_velocity))
 
 
-def calculate_linear_velocity(linear_distance, smooth_duration=0.500,
-                              sampling_frequency=29):
-
+def calculate_linear_velocity(
+    linear_distance, smooth_duration=0.500, sampling_frequency=29
+):
     smoothed_linear_distance = gaussian_filter1d(
-        linear_distance, smooth_duration * sampling_frequency)
+        linear_distance, smooth_duration * sampling_frequency
+    )
 
     smoothed_velocity = np.diff(smoothed_linear_distance) * sampling_frequency
     return np.r_[smoothed_velocity[0], smoothed_velocity]
 
 
 def convert_linear_distance_to_linear_position(
-        linear_distance, edge_id, edge_order, spacing=30):
+    linear_distance, edge_id, edge_order, spacing=30
+):
     linear_position = linear_distance.copy()
     n_edges = len(edge_order)
     if isinstance(spacing, int) | isinstance(spacing, float):
-        spacing = [spacing, ] * (n_edges - 1)
-
-    for prev_edge, cur_edge, space in zip(
-            edge_order[:-1], edge_order[1:], spacing):
-        is_cur_edge = (edge_id == cur_edge)
-        is_prev_edge = (edge_id == prev_edge)
+        spacing = [
+            spacing,
+        ] * (n_edges - 1)
+
+    for prev_edge, cur_edge, space in zip(edge_order[:-1], edge_order[1:], spacing):
+        is_cur_edge = edge_id == cur_edge
+        is_prev_edge = edge_id == prev_edge
 
         cur_distance = linear_position[is_cur_edge]
         cur_distance -= cur_distance.min()
         cur_distance += linear_position[is_prev_edge].max() + space
         linear_position[is_cur_edge] = cur_distance
 
     return linear_position
 
 
-def get_graph_1D_2D_relationships(track_graph, edge_order, edge_spacing,
-                                  center_well_id):
-    '''
+def get_graph_1D_2D_relationships(
+    track_graph, edge_order, edge_spacing, center_well_id
+):
+    """
 
     Parameters
     ----------
     track_graph : networkx.Graph
     edge_order : array-like, shape (n_edges,)
     edge_spacing : float or array-like, shape (n_edges,)
     center_well_id : int
@@ -181,21 +214,19 @@
     Returns
     -------
     node_linear_position : numpy.ndarray, shape (n_edges, n_position_dims)
     edges : numpy.ndarray, shape (n_edges, 2)
     node_2D_position : numpy.ndarray, shape (n_edges, 2, n_position_dims)
     edge_dist : numpy.ndarray, shape (n_edges,)
 
-    '''
+    """
     linear_distance = []
     edge_id = []
 
-    dist = dict(
-        nx.all_pairs_dijkstra_path_length(track_graph, weight="distance")
-    )
+    dist = dict(nx.all_pairs_dijkstra_path_length(track_graph, weight="distance"))
     n_edges = len(track_graph.edges)
 
     for ind, (node1, node2) in enumerate(track_graph.edges):
         linear_distance.append(dist[center_well_id][node1])
         linear_distance.append(dist[center_well_id][node2])
         edge_id.append(ind)
         edge_id.append(ind)
@@ -203,109 +234,137 @@
     linear_distance = np.array(linear_distance)
     edge_id = np.array(edge_id)
 
     node_linear_position = convert_linear_distance_to_linear_position(
         linear_distance, edge_id, edge_order, spacing=edge_spacing
     )
 
-    node_linear_position = node_linear_position.reshape((n_edges, 2))[
-        edge_order]
+    node_linear_position = node_linear_position.reshape((n_edges, 2))[edge_order]
     node_linear_distance = linear_distance.reshape((n_edges, 2))[edge_order]
 
     return node_linear_position, node_linear_distance
 
 
-def _calulcate_linear_position(linear_distance, edge_id, track_graph,
-                               center_well_id, edge_order, edge_spacing=15):
-    '''Calculate linear distance but map the left arm to the
-    range(max_linear_distance, max_linear_distance + max_left_arm_distance).'''
+def _calulcate_linear_position(
+    linear_distance, edge_id, track_graph, center_well_id, edge_order, edge_spacing=15
+):
+    """Calculate linear distance but map the left arm to the
+    range(max_linear_distance, max_linear_distance + max_left_arm_distance)."""
     linear_position = linear_distance.copy()
 
     node_linear_position, node_linear_distance = get_graph_1D_2D_relationships(
-        track_graph, edge_order, edge_spacing, center_well_id)
+        track_graph, edge_order, edge_spacing, center_well_id
+    )
 
     n_edges = len(edge_order)
     if isinstance(edge_spacing, int) | isinstance(edge_spacing, float):
-        edge_spacing = [edge_spacing, ] * (n_edges - 1)
+        edge_spacing = [
+            edge_spacing,
+        ] * (n_edges - 1)
 
     for start_linear_position, start_linear_distance, cur_edge in zip(
-            node_linear_position[:, 0], node_linear_distance[:, 0],
-            edge_order):
-        is_cur_edge = (edge_id == cur_edge)
+        node_linear_position[:, 0], node_linear_distance[:, 0], edge_order
+    ):
+        is_cur_edge = edge_id == cur_edge
 
         cur_distance = linear_distance[is_cur_edge] - start_linear_distance
         cur_distance += start_linear_position
         linear_position[is_cur_edge] = cur_distance
 
     return linear_position
 
 
-def _get_linear_position_hmm(epoch_key, animals, position_df,
-                             max_distance_from_well=5,
-                             route_euclidean_distance_scaling=1,
-                             min_distance_traveled=50,
-                             sensor_std_dev=5,
-                             diagonal_bias=1E-1,
-                             edge_order=EDGE_ORDER, edge_spacing=EDGE_SPACING,
-                             position_sampling_frequency=33):
+def _get_linear_position_hmm(
+    epoch_key,
+    animals,
+    position_df,
+    max_distance_from_well=5,
+    route_euclidean_distance_scaling=1,
+    min_distance_traveled=50,
+    sensor_std_dev=5,
+    diagonal_bias=1e-1,
+    edge_order=EDGE_ORDER,
+    edge_spacing=EDGE_SPACING,
+    position_sampling_frequency=33,
+):
     animal, day, epoch = epoch_key
     track_graph, center_well_id = make_track_graph(epoch_key, animals)
-    position = position_df.loc[:, ['x_position', 'y_position']].values
+    position = position_df.loc[:, ["x_position", "y_position"]].values
     track_segment_id = classify_track_segments(
-        track_graph, position,
+        track_graph,
+        position,
         route_euclidean_distance_scaling=route_euclidean_distance_scaling,
         sensor_std_dev=sensor_std_dev,
-        diagonal_bias=diagonal_bias)
-    (position_df['linear_distance'],
-     position_df['projected_x_position'],
-     position_df['projected_y_position']) = calculate_linear_distance(
-        track_graph, track_segment_id, center_well_id, position)
-    position_df['track_segment_id'] = track_segment_id
-    SEGMENT_ID_TO_ARM_NAME = {0.0: 'Center Arm',
-                              1.0: 'Left Arm',
-                              2.0: 'Right Arm',
-                              3.0: 'Left Arm',
-                              4.0: 'Right Arm'}
+        diagonal_bias=diagonal_bias,
+    )
+    (
+        position_df["linear_distance"],
+        position_df["projected_x_position"],
+        position_df["projected_y_position"],
+    ) = calculate_linear_distance(
+        track_graph, track_segment_id, center_well_id, position
+    )
+    position_df["track_segment_id"] = track_segment_id
+    SEGMENT_ID_TO_ARM_NAME = {
+        0.0: "Center Arm",
+        1.0: "Left Arm",
+        2.0: "Right Arm",
+        3.0: "Left Arm",
+        4.0: "Right Arm",
+    }
     position_df = position_df.assign(
         arm_name=lambda df: df.track_segment_id.map(SEGMENT_ID_TO_ARM_NAME)
     )
 
     segments_df, labeled_segments = get_segments_df(
-        epoch_key, animals, position_df, max_distance_from_well,
-        min_distance_traveled)
+        epoch_key, animals, position_df, max_distance_from_well, min_distance_traveled
+    )
 
     segments_df = pd.merge(
-        labeled_segments, segments_df, right_index=True,
-        left_on='labeled_segments', how='outer')
+        labeled_segments,
+        segments_df,
+        right_index=True,
+        left_on="labeled_segments",
+        how="outer",
+    )
     position_df = pd.concat((position_df, segments_df), axis=1)
-    position_df['linear_position'] = _calulcate_linear_position(
+    position_df["linear_position"] = _calulcate_linear_position(
         position_df.linear_distance.values,
-        position_df.track_segment_id.values, track_graph, center_well_id,
-        edge_order=edge_order, edge_spacing=edge_spacing)
-    position_df['linear_velocity'] = calculate_linear_velocity(
-        position_df.linear_distance, smooth_duration=0.500,
-        sampling_frequency=position_sampling_frequency)
-    position_df['linear_speed'] = np.abs(position_df.linear_velocity)
-    position_df['is_correct'] = position_df.is_correct.fillna(False)
+        position_df.track_segment_id.values,
+        track_graph,
+        center_well_id,
+        edge_order=edge_order,
+        edge_spacing=edge_spacing,
+    )
+    position_df["linear_velocity"] = calculate_linear_velocity(
+        position_df.linear_distance,
+        smooth_duration=0.500,
+        sampling_frequency=position_sampling_frequency,
+    )
+    position_df["linear_speed"] = np.abs(position_df.linear_velocity)
+    position_df["is_correct"] = position_df.is_correct.fillna(False)
 
     return position_df
 
 
-def get_interpolated_position_dataframe(epoch_key, animals,
-                                        time_function=get_trial_time,
-                                        use_hmm=True,
-                                        max_distance_from_well=5,
-                                        route_euclidean_distance_scaling=1,
-                                        min_distance_traveled=50,
-                                        sensor_std_dev=5,
-                                        diagonal_bias=1E-1,
-                                        edge_spacing=EDGE_SPACING,
-                                        edge_order=EDGE_ORDER,
-                                        position_sampling_frequency=1500):
-    '''Gives the interpolated position of animal for a given epoch.
+def get_interpolated_position_dataframe(
+    epoch_key,
+    animals,
+    time_function=get_trial_time,
+    use_hmm=True,
+    max_distance_from_well=5,
+    route_euclidean_distance_scaling=1,
+    min_distance_traveled=50,
+    sensor_std_dev=5,
+    diagonal_bias=1e-1,
+    edge_spacing=EDGE_SPACING,
+    edge_order=EDGE_ORDER,
+    position_sampling_frequency=1500,
+):
+    """Gives the interpolated position of animal for a given epoch.
 
     Defaults to interpolating the position to the LFP time. Can use the
     `time_function` to specify different time to interpolate to.
 
     Parameters
     ----------
     epoch_key : tuple
@@ -324,126 +383,143 @@
         This favors less jumps. Larger numbers favor more jumps.
     min_distance_traveled : float, optional
 
     Returns
     -------
     interpolated_position : pandas.DataFrame
 
-    '''
+    """
     time = time_function(epoch_key, animals)
-    position_df = get_position_dataframe(
-        epoch_key, animals, skip_linearization=True)
+    position_df = get_position_dataframe(epoch_key, animals, skip_linearization=True)
 
-    new_index = pd.Index(np.unique(np.concatenate(
-        (position_df.index, time))), name='time')
-    position_df = (position_df
-                   .reindex(index=new_index)
-                   .interpolate(method='linear')
-                   .reindex(index=time))
+    new_index = pd.Index(
+        np.unique(np.concatenate((position_df.index, time))), name="time"
+    )
+    position_df = (
+        position_df.reindex(index=new_index)
+        .interpolate(method="linear")
+        .reindex(index=time)
+    )
 
-    position_df.loc[position_df.speed < 0, 'speed'] = 0.0
+    position_df.loc[position_df.speed < 0, "speed"] = 0.0
 
     position_df = _get_linear_position_hmm(
-        epoch_key, animals, position_df,
-        max_distance_from_well, route_euclidean_distance_scaling,
-        min_distance_traveled, sensor_std_dev, diagonal_bias,
-        edge_order=edge_order, edge_spacing=edge_spacing,
-        position_sampling_frequency=position_sampling_frequency)
+        epoch_key,
+        animals,
+        position_df,
+        max_distance_from_well,
+        route_euclidean_distance_scaling,
+        min_distance_traveled,
+        sensor_std_dev,
+        diagonal_bias,
+        edge_order=edge_order,
+        edge_spacing=edge_spacing,
+        position_sampling_frequency=position_sampling_frequency,
+    )
 
     return position_df
 
 
 def get_well_locations(epoch_key, animals):
-    '''Retrieves the 2D coordinates for each well.
-    '''
+    """Retrieves the 2D coordinates for each well."""
     animal, day, epoch = epoch_key
-    task_file = get_data_structure(animals[animal], day, 'task', 'task')
-    linearcoord = task_file[epoch - 1]['linearcoord'][0, 0].squeeze()
+    task_file = get_data_structure(animals[animal], day, "task", "task")
+    linearcoord = task_file[epoch - 1]["linearcoord"][0, 0].squeeze(axis=0)
     well_locations = []
     for arm in linearcoord:
         well_locations.append(arm[0, :, 0])
         well_locations.append(arm[-1, :, 0])
     well_locations = np.stack(well_locations)
     _, ind = np.unique(well_locations, axis=0, return_index=True)
     return well_locations[np.sort(ind), :]
 
 
 def get_track_segments(epoch_key, animals):
-    '''
+    """
 
     Parameters
     ----------
     epoch_key : tuple
     animals : dict of namedtuples
 
     Returns
     -------
     track_segments : ndarray, shape (n_segments, n_nodes, n_space)
     center_well_position : ndarray, shape (n_space,)
 
-    '''
+    """
     animal, day, epoch = epoch_key
-    task_file = get_data_structure(animals[animal], day, 'task', 'task')
-    linearcoord = task_file[epoch - 1]['linearcoord'][0, 0].squeeze(axis=0)
-    track_segments = [np.stack(((arm[:-1, :, 0], arm[1:, :, 0])), axis=1)
-                      for arm in linearcoord]
+    task_file = get_data_structure(animals[animal], day, "task", "task")
+    linearcoord = task_file[epoch - 1]["linearcoord"][0, 0].squeeze(axis=0)
+    track_segments = [
+        np.stack(((arm[:-1, :, 0], arm[1:, :, 0])), axis=1) for arm in linearcoord
+    ]
     center_well_position = track_segments[0][0][0]
     track_segments = np.concatenate(track_segments)
     _, unique_ind = np.unique(track_segments, return_index=True, axis=0)
     return track_segments[np.sort(unique_ind)], center_well_position
 
 
 def make_track_graph(epoch_key, animals):
-    '''
+    """
 
     Parameters
     ----------
     epoch_key : tuple, (animal, day, epoch)
     animals : dict of namedtuples
 
     Returns
     -------
     track_graph : networkx Graph
     center_well_id : int
 
-    '''
-    track_segments, center_well_position = get_track_segments(
-        epoch_key, animals)
+    """
+    track_segments, center_well_position = get_track_segments(epoch_key, animals)
     nodes = track_segments.copy().reshape((-1, 2))
     _, unique_ind = np.unique(nodes, return_index=True, axis=0)
     nodes = nodes[np.sort(unique_ind)]
 
-    edges = np.zeros(track_segments.shape[:2], dtype=np.int)
+    edges = np.zeros(track_segments.shape[:2], dtype=int)
     for node_id, node in enumerate(nodes):
         edge_ind = np.nonzero(np.isin(track_segments, node).sum(axis=2) > 1)
         edges[edge_ind] = node_id
 
     edge_distances = np.linalg.norm(
-        np.diff(track_segments, axis=-2).squeeze(axis=-2), axis=1)
+        np.diff(track_segments, axis=-2).squeeze(axis=-2), axis=1
+    )
 
     track_graph = nx.Graph()
 
     for node_id, node_position in enumerate(nodes):
         track_graph.add_node(node_id, pos=tuple(node_position))
 
     for edge, distance in zip(edges, edge_distances):
         nx.add_path(track_graph, edge, distance=distance)
 
     center_well_id = np.unique(
-        np.nonzero(np.isin(nodes, center_well_position).sum(axis=1) > 1)[0])[0]
+        np.nonzero(np.isin(nodes, center_well_position).sum(axis=1) > 1)[0]
+    )[0]
 
     return track_graph, center_well_id
 
 
-def get_segments_df(epoch_key, animals, position_df, max_distance_from_well=5,
-                    min_distance_traveled=50):
+def get_segments_df(
+    epoch_key, animals, position_df, max_distance_from_well=5, min_distance_traveled=50
+):
     well_locations = get_well_locations(epoch_key, animals)
-    position = position_df.loc[:, ['x_position', 'y_position']].values
+    position = position_df.loc[:, ["x_position", "y_position"]].values
     segments_df, labeled_segments = segment_path(
-        position_df.index, position, well_locations, epoch_key, animals,
-        max_distance_from_well=max_distance_from_well)
+        position_df.index,
+        position,
+        well_locations,
+        epoch_key,
+        animals,
+        max_distance_from_well=max_distance_from_well,
+    )
     segments_df = score_inbound_outbound(
-        segments_df, epoch_key, animals, min_distance_traveled)
+        segments_df, epoch_key, animals, min_distance_traveled
+    )
     segments_df = segments_df.loc[
-        :, ['from_well', 'to_well', 'task', 'is_correct', 'turn']]
+        :, ["from_well", "to_well", "task", "is_correct", "turn"]
+    ]
 
     return segments_df, labeled_segments
```

### Comparing `loren_frank_data_processing-0.9.9.dev0/loren_frank_data_processing/utilities.py` & `loren_frank_data_processing-1.0.1/loren_frank_data_processing/utilities.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,179 +6,192 @@
 from shutil import copyfile
 
 import numpy as np
 import pandas as pd
 
 
 def copy_animal(animal, src_directory):
-    '''Copies essential data files and renames multiunit files.
+    """Copies essential data files and renames multiunit files.
 
     Parameters
     ----------
     animal : namedtuple
         First element is the target directory where the animal's data
         should be located. The second element is the animal shortened name.
     src_directory : str
 
-    '''
+    """
     processed_data_dir = join(src_directory, animal.short_name)
     try:
         makedirs(animal.directory)
     except FileExistsError:
         pass
 
-    FILE_TYPES = ['cellinfo', 'linpos', 'pos', 'rawpos', 'task', 'tetinfo',
-                  'spikes']
-    data_files = [glob(join(processed_data_dir,
-                            '{animal.short_name}{file_type}*.mat').format(
-        animal=animal, file_type=file_type))
-        for file_type in FILE_TYPES]
+    FILE_TYPES = ["cellinfo", "linpos", "pos", "rawpos", "task", "tetinfo", "spikes"]
+    data_files = [
+        glob(
+            join(processed_data_dir, "{animal.short_name}{file_type}*.mat").format(
+                animal=animal, file_type=file_type
+            )
+        )
+        for file_type in FILE_TYPES
+    ]
     for old_path in chain.from_iterable(data_files):
-        new_path = join(animal.directory, old_path.split('/')[-1])
+        new_path = join(animal.directory, old_path.split("/")[-1])
 
-        print('Copying {old_path}\nto \n{new_path}\n'.format(
-            old_path=old_path,
-            new_path=new_path
-        ))
+        print(
+            "Copying {old_path}\nto \n{new_path}\n".format(
+                old_path=old_path, new_path=new_path
+            )
+        )
         copyfile(old_path, new_path)
 
-    src_lfp_data_dir = join(processed_data_dir, 'EEG')
-    target_lfp_data_dir = join(animal.directory, 'EEG')
+    src_lfp_data_dir = join(processed_data_dir, "EEG")
+    target_lfp_data_dir = join(animal.directory, "EEG")
     try:
         makedirs(target_lfp_data_dir)
     except FileExistsError:
         pass
-    lfp_files = [file for file in listdir(src_lfp_data_dir)
-                 if 'gnd' not in file and 'eeg' in file]
+    lfp_files = [
+        file
+        for file in listdir(src_lfp_data_dir)
+        if "gnd" not in file and "eeg" in file
+    ]
 
     for file_name in lfp_files:
         old_path = join(src_lfp_data_dir, file_name)
         new_path = join(target_lfp_data_dir, file_name)
 
-        print('Copying {old_path}\nto \n{new_path}\n'.format(
-            old_path=old_path,
-            new_path=new_path
-        ))
+        print(
+            "Copying {old_path}\nto \n{new_path}\n".format(
+                old_path=old_path, new_path=new_path
+            )
+        )
         copyfile(old_path, new_path)
 
     marks_directory = join(src_directory, animal.directory)
-    mark_files = [join(root, f) for root, _, files in walk(marks_directory)
-                  for f in files if f.endswith('_params.mat')
-                  and not f.startswith('matclust')]
-    new_mark_filenames = [rename_mark_file(mark_file, animal)
-                          for mark_file in mark_files]
+    mark_files = [
+        join(root, f)
+        for root, _, files in walk(marks_directory)
+        for f in files
+        if f.endswith("_params.mat") and not f.startswith("matclust")
+    ]
+    new_mark_filenames = [
+        rename_mark_file(mark_file, animal) for mark_file in mark_files
+    ]
     for mark_file, new_filename in zip(mark_files, new_mark_filenames):
         mark_path = join(target_lfp_data_dir, new_filename)
-        print('Copying {mark_file}\nto \n{new_filename}\n'.format(
-            mark_file=mark_file,
-            new_filename=mark_path
-        ))
+        print(
+            "Copying {mark_file}\nto \n{new_filename}\n".format(
+                mark_file=mark_file, new_filename=mark_path
+            )
+        )
         copyfile(mark_file, mark_path)
 
 
 def rename_mark_file(file_str, animal):
-    matched = re.match(
-        r'.*(\d.+)-(\d.+)_params.mat', file_str.split('/')[-1])
+    matched = re.match(r".*(\d.+)-(\d.+)_params.mat", file_str.split("/")[-1])
     try:
         day, tetrode_number = matched.groups()
     except AttributeError:
-        matched = re.match(
-            r'.*(\d+)-.*-(\d+)_params.mat', file_str.split('/')[-1])
+        matched = re.match(r".*(\d+)-.*-(\d+)_params.mat", file_str.split("/")[-1])
         try:
             day, tetrode_number = matched.groups()
         except AttributeError:
             print(file_str)
             raise
 
-    new_name = ('{animal}marks{day:02d}-{tetrode_number:02d}.mat'.format(
-        animal=animal.short_name,
-        day=int(day),
-        tetrode_number=int(tetrode_number)
-    ))
+    new_name = "{animal}marks{day:02d}-{tetrode_number:02d}.mat".format(
+        animal=animal.short_name, day=int(day), tetrode_number=int(tetrode_number)
+    )
 
     return new_name
 
 
 def find_closest_ind(search_array, target):
-    '''Finds the index position in the search_array that is closest to the
+    """Finds the index position in the search_array that is closest to the
     target. This works for large search_arrays. See:
     http://stackoverflow.com/questions/8914491/finding-the-nearest-value-and-return-the-index-of-array-in-python
 
     Parameters
     ----------
     search_array : ndarray
     target : ndarray element
 
     Returns
     -------
     index : int
         Index closest to target element.
 
-    '''
+    """
     # Get insertion index, need to be sorted
     ind = search_array.searchsorted(target)
     # If index is out of bounds, move to bounds
     ind = np.clip(ind, 1, len(search_array) - 1)
     # Adjust if the left or right index is closer
-    adjust = (target - search_array[ind - 1]
-              ) < (search_array[ind] - target)
+    adjust = (target - search_array[ind - 1]) < (search_array[ind] - target)
     return ind - adjust
 
 
 def _get_windowed_dataframe(time_series, segments, window_start, window_end):
-    '''For each segment, return a dataframe with the time relative to
+    """For each segment, return a dataframe with the time relative to
     the start of the segment + window_offset.
-    '''
+    """
     for segment_start, segment_end in segments:
         if window_end is not None:
             segment_end = segment_start + window_end
         time_series_segment = time_series.loc[
-            (segment_start + window_start):segment_end, :]
+            (segment_start + window_start) : segment_end, :
+        ]
         new_time = time_series_segment.index - segment_start
         yield time_series_segment.set_index(new_time)
 
 
-def _get_windowed_dataframe_sampling_frequency(time_series, segments,
-                                               window_start, window_end,
-                                               sampling_frequency):
-    '''For each segment, return a dataframe with the time relative to
+def _get_windowed_dataframe_sampling_frequency(
+    time_series, segments, window_start, window_end, sampling_frequency
+):
+    """For each segment, return a dataframe with the time relative to
     the start of the segment + window_offset.
 
     Uses the sampling frequency to get more accurate time relative to the
     start time of the segments if the samples are evenly spaced.
-    '''
+    """
     n_time = len(time_series)
-    n_start_samples = np.fix(
-        window_start.total_seconds() * sampling_frequency).astype(int)
+
+    try:
+        window_start = window_start.total_seconds()
+        window_end = window_end.total_seconds()
+    except AttributeError:
+        pass
+
+    n_start_samples = np.fix(window_start * sampling_frequency).astype(int)
     if window_end is not None:
-        n_end_samples = np.fix(
-            window_end.total_seconds() * sampling_frequency).astype(int) + 1
+        n_end_samples = np.fix(window_end * sampling_frequency).astype(int) + 1
 
     for segment_start, segment_end in segments:
-        segment_start_ind = time_series.index.get_loc(
-            segment_start, method='nearest')
+        segment_start_ind = time_series.index.get_loc(segment_start, method="nearest")
         window_start_ind = np.max([0, segment_start_ind + n_start_samples])
         if window_end is not None:
-            window_end_ind = np.min(
-                [n_time, segment_start_ind + n_end_samples])
+            window_end_ind = np.min([n_time, segment_start_ind + n_end_samples])
         else:
-            window_end_ind = time_series.index.get_loc(
-                segment_end, method='nearest')
-        time_series_segment = time_series.iloc[
-            window_start_ind:window_end_ind, :]
-        time_ind = np.arange(window_start_ind - segment_start_ind,
-                             window_end_ind - segment_start_ind)
+            window_end_ind = time_series.index.get_loc(segment_end, method="nearest")
+        time_series_segment = time_series.iloc[window_start_ind:window_end_ind, :]
+        time_ind = np.arange(
+            window_start_ind - segment_start_ind, window_end_ind - segment_start_ind
+        )
         new_time = pd.TimedeltaIndex(
-            time_ind / sampling_frequency, unit='s', name='time')
+            time_ind / sampling_frequency, unit="s", name="time"
+        )
         yield time_series_segment.set_index(new_time)
 
 
-def reshape_to_segments(time_series, segments, window_offset=None,
-                        sampling_frequency=None, axis=0):
-    '''Take multiple windows of a time series and set time relative to
+def reshape_to_segments(
+    time_series, segments, window_offset=None, sampling_frequency=None, axis=0
+):
+    """Take multiple windows of a time series and set time relative to
     the start of the window.
 
     Useful for examining an event of interest.
 
     Parameters
     ----------
     time_series : pandas.DataFrame, shape (n_time, ...)
@@ -219,15 +232,15 @@
                             window_offset=(-0.001, None))
     >>> reshape_to_segments(time_series, segments,
                             window_offset=(-0.001, 0.001))
     >>> reshape_to_segments(time_series, segments,
                             window_offset=(-0.001, 0.001),
                             sampling_frequency=sampling_frequency)
 
-    '''
+    """
     segments_index = segments.index
     segments = segments.itertuples(index=False)
     time_series = pd.DataFrame(time_series)
 
     if window_offset is not None:
         window_start, window_end = window_offset
         if window_start is not None:
@@ -235,17 +248,20 @@
         else:
             window_start = pd.Timedelta(seconds=0)
         if window_end is not None:
             window_end = pd.Timedelta(seconds=window_end)
     else:
         window_start, window_end = pd.Timedelta(seconds=0), None
     if sampling_frequency is None:
-        return (pd.concat(_get_windowed_dataframe(
-            time_series, segments, window_start, window_end),
+        return pd.concat(
+            _get_windowed_dataframe(time_series, segments, window_start, window_end),
             keys=segments_index,
-            axis=axis).sort_index())
+            axis=axis,
+        ).sort_index()
     else:
-        return (pd.concat(_get_windowed_dataframe_sampling_frequency(
-            time_series, segments, window_start, window_end,
-            sampling_frequency),
+        return pd.concat(
+            _get_windowed_dataframe_sampling_frequency(
+                time_series, segments, window_start, window_end, sampling_frequency
+            ),
             keys=segments_index,
-            axis=axis).sort_index())
+            axis=axis,
+        ).sort_index()
```

### Comparing `loren_frank_data_processing-0.9.9.dev0/loren_frank_data_processing/tetrodes.py` & `loren_frank_data_processing-1.0.1/loren_frank_data_processing/tetrodes.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,75 +1,86 @@
 from os.path import join
 
 import numpy as np
 import pandas as pd
 from scipy.io import loadmat
 
-from .core import logger, reconstruct_time
+from loren_frank_data_processing.core import logger, reconstruct_time
 
 
-def _convert_to_dict(struct_array):
+def squeeze_matcell(x):
     try:
-        return {name: struct_array[name].item()
-                for name in struct_array.dtype.names}
+        return x[0, 0][0, 0]
+    except IndexError:
+        try:
+            return x[0, 0][0]
+        except IndexError:
+            return x[0, 0]
+
+
+def _convert_to_dict(tetrode):
+    try:
+        return {name: squeeze_matcell(tetrode[name]) for name in tetrode.dtype.names}
     except TypeError:
         return {}
 
 
 def get_tetrode_info_path(animal):
-    '''Returns the Matlab tetrode info file name assuming it is in the
+    """Returns the Matlab tetrode info file name assuming it is in the
     Raw Data directory.
 
     Parameters
     ----------
     animal : namedtuple
         First element is the directory where the animal's data is located.
         The second element is the animal shortened name.
 
     Returns
     -------
     filename : str
         The path to the information about the tetrodes for a given animal.
 
-    '''
-    filename = '{animal.short_name}tetinfo.mat'.format(animal=animal)
-    return join(animal.directory, filename)
+    """
+    return join(animal.directory, f"{animal.short_name}tetinfo.mat")
 
 
 def get_LFP_dataframe(tetrode_key, animals):
-    '''Gets the LFP data for a given epoch and tetrode.
+    """Gets the LFP data for a given epoch and tetrode.
 
     Parameters
     ----------
     tetrode_key : tuple
         Unique key identifying the tetrode. Elements are
         (animal_short_name, day, epoch, tetrode_number).
     animals : dict of named-tuples
         Dictionary containing information about the directory for each
         animal. The key is the animal_short_name.
 
     Returns
     -------
     LFP : pandas dataframe
         Contains the electric potential and time
-    '''
+    """
     try:
         lfp_file = loadmat(get_LFP_filename(tetrode_key, animals))
-        lfp_data = lfp_file['eeg'][0, -1][0, -1][0, -1]
+        lfp_data = lfp_file["eeg"][0, -1][0, -1][0, -1]
         lfp_time = reconstruct_time(
-            lfp_data['starttime'][0, 0].item(),
-            lfp_data['data'][0, 0].size,
-            float(lfp_data['samprate'][0, 0].squeeze()))
+            lfp_data["starttime"][0, 0].item(),
+            lfp_data["data"][0, 0].size,
+            float(lfp_data["samprate"][0, 0].squeeze()),
+        )
         return pd.Series(
-            data=lfp_data['data'][0, 0].squeeze().astype(float),
+            data=lfp_data["data"][0, 0].squeeze().astype(float),
             index=lfp_time,
-            name='{0}_{1:02d}_{2:02}_{3:03}'.format(*tetrode_key))
+            name="{0}_{1:02d}_{2:02}_{3:03}".format(*tetrode_key),
+        )
     except (FileNotFoundError, TypeError):
-        logger.warning('Failed to load file: {0}'.format(
-            get_LFP_filename(tetrode_key, animals)))
+        logger.warning(
+            "Failed to load file: {0}".format(get_LFP_filename(tetrode_key, animals))
+        )
 
 
 def make_tetrode_dataframe(animals, epoch_key=None):
     """Information about all tetrodes such as recording location.
 
     Parameters
     ----------
@@ -79,116 +90,109 @@
 
     Returns
     -------
     tetrode_infomation : pandas.DataFrame
 
     """
     tetrode_info = []
+
     if epoch_key is not None:
         animal, day, epoch = epoch_key
         file_name = get_tetrode_info_path(animals[animal])
-        tet_info = loadmat(file_name, squeeze_me=True)["tetinfo"]
+        tet_info = loadmat(file_name, squeeze_me=False)["tetinfo"].squeeze(axis=0)
         tetrode_info.append(
             convert_tetrode_epoch_to_dataframe(
-                tet_info[day - 1][epoch - 1], epoch_key))
+                tet_info[day - 1].squeeze(axis=0)[epoch - 1].squeeze(axis=0), epoch_key
+            )
+        )
         return pd.concat(tetrode_info, sort=True)
 
     for animal in animals.values():
         file_name = get_tetrode_info_path(animal)
-        tet_info = loadmat(file_name, squeeze_me=True)["tetinfo"]
-        try:
-            for day_ind, day in enumerate(tet_info):
-                try:
-                    for epoch_ind, epoch in enumerate(day):
-                        epoch_key = (
-                            animal.short_name,
-                            day_ind + 1,
-                            epoch_ind + 1,
-                        )  # noqa
-                        tetrode_info.append(
-                            convert_tetrode_epoch_to_dataframe(
-                                epoch, epoch_key)
-                        )
-                except IndexError:
-                    pass
-        except TypeError:
-            # Only one day of recording
-            try:
-                day_ind = 0
-                for epoch_ind, epoch in enumerate(tet_info):
-                    epoch_key = animal.short_name, day_ind + 1, epoch_ind + 1
-                    tetrode_info.append(
-                        convert_tetrode_epoch_to_dataframe(epoch, epoch_key))
-            except IndexError:
-                pass
+        tet_info = loadmat(file_name, squeeze_me=False)["tetinfo"]
+        for day_ind, day in enumerate(tet_info.squeeze(axis=0)):
+            for epoch_ind, epoch in enumerate(day.squeeze(axis=0)):
+                epoch_key = (
+                    animal.short_name,
+                    day_ind + 1,
+                    epoch_ind + 1,
+                )
+                tetrode_info.append(
+                    convert_tetrode_epoch_to_dataframe(epoch.squeeze(axis=0), epoch_key)
+                )
 
     return pd.concat(tetrode_info, sort=True)
 
 
 def get_LFP_filename(tetrode_key, animals):
-    '''Returns a file name for the tetrode file LFP for an epoch.
+    """Returns a file name for the tetrode file LFP for an epoch.
 
     Parameters
     ----------
     tetrode_key : tuple
         Unique key identifying the tetrode. Elements are
         (animal_short_name, day, epoch, tetrode_number).
     animals : dict of named-tuples
         Dictionary containing information about the directory for each
         animal. The key is the animal_short_name.
 
     Returns
     -------
     filename : str
         File path to tetrode file LFP
-    '''
+    """
     animal, day, epoch, tetrode_number = tetrode_key
-    filename = ('{animal.short_name}eeg{day:02d}-{epoch}-'
-                '{tetrode_number:02d}.mat').format(
-                    animal=animals[animal], day=day, epoch=epoch,
-                    tetrode_number=tetrode_number)
-    return join(animals[animal].directory, 'EEG', filename)
+    filename = (
+        "{animal.short_name}eeg{day:02d}-{epoch}-" "{tetrode_number:02d}.mat"
+    ).format(
+        animal=animals[animal], day=day, epoch=epoch, tetrode_number=tetrode_number
+    )
+    return join(animals[animal].directory, "EEG", filename)
 
 
 def _get_tetrode_id(dataframe):
-    '''Unique string identifier for a tetrode'''
-    return (dataframe.animal + '_' +
-            dataframe.day.map('{:02d}'.format) + '_' +
-            dataframe.epoch.map('{:02}'.format) + '_' +
-            dataframe.tetrode_number.map('{:03}'.format))
+    """Unique string identifier for a tetrode"""
+    return (
+        dataframe.animal
+        + "_"
+        + dataframe.day.map("{:02d}".format)
+        + "_"
+        + dataframe.epoch.map("{:02}".format)
+        + "_"
+        + dataframe.tetrode_number.map("{:03}".format)
+    )
 
 
 def convert_tetrode_epoch_to_dataframe(tetrodes_in_epoch, epoch_key):
-    '''Convert tetrode information data structure to dataframe.
+    """Convert tetrode information data structure to dataframe.
 
     Parameters
     ----------
     tetrodes_in_epoch : matlab data structure
     epoch_key : tuple
         Unique key identifying a recording epoch. Elements are
         (animal, day, epoch)
 
     Returns
     -------
     tetrode_info : dataframe
 
-    '''
+    """
     animal, day, epoch = epoch_key
-    tetrode_dict_list = [_convert_to_dict(
-        tetrode) for tetrode in tetrodes_in_epoch]
-    return (pd.DataFrame(tetrode_dict_list)
-              .assign(animal=lambda x: animal)
-              .assign(day=lambda x: day)
-              .assign(epoch=lambda x: epoch)
-              .assign(tetrode_number=lambda x: x.index + 1)
-              .assign(tetrode_id=_get_tetrode_id)
-            # set index to identify rows
-              .set_index(['animal', 'day', 'epoch', 'tetrode_number'])
-              .sort_index()
-            )
+    tetrode_dict_list = [_convert_to_dict(tetrode) for tetrode in tetrodes_in_epoch]
+    return (
+        pd.DataFrame(tetrode_dict_list)
+        .assign(animal=lambda x: animal)
+        .assign(day=lambda x: day)
+        .assign(epoch=lambda x: epoch)
+        .assign(tetrode_number=lambda x: x.index + 1)
+        .assign(tetrode_id=_get_tetrode_id)
+        .set_index(["animal", "day", "epoch", "tetrode_number"])
+        .sort_index()
+    )
 
 
 def get_trial_time(epoch_key, animals):
     """Time in the recording session in terms of the LFP.
 
     This will return the LFP time of the first tetrode found (according to the
     tetrode info). This is useful when there are slightly different timings
@@ -214,32 +218,31 @@
         if lfp_df is not None:
             break
 
     return lfp_df.index.rename("time")
 
 
 def get_LFPs(tetrode_keys, animals):
-    '''Retrieves LFP data and makes sure the data has the same timestamps.
+    """Retrieves LFP data and makes sure the data has the same timestamps.
 
     This function is useful when data is collected on different signal
     processing systems and have slightly different timings. This function will
     interpolate the data to the time of the first tetrode recorded.
 
     Parameters
     ----------
     tetrode_keys : list of tuples, shape (n_signals,)
     animals : dict of namedtuples, shape (n_animals)
 
     Returns
     -------
     LFPs : pandas DataFrame, shape (n_time, n_signals)
 
-    '''
+    """
     epoch_key = tetrode_keys[0][:3]
     time = get_trial_time(epoch_key, animals)
-    LFPs = pd.concat([get_LFP_dataframe(tetrode_key, animals)
-                      for tetrode_key in tetrode_keys], axis=1)
-    new_index = pd.Index(np.unique(np.concatenate(
-        (LFPs.index, time))), name='time')
-    return (LFPs.reindex(index=new_index)
-            .interpolate(method='time')
-            .reindex(index=time))
+    LFPs = pd.concat(
+        [get_LFP_dataframe(tetrode_key, animals) for tetrode_key in tetrode_keys],
+        axis=1,
+    )
+    new_index = pd.Index(np.unique(np.concatenate((LFPs.index, time))), name="time")
+    return LFPs.reindex(index=new_index).interpolate(method="time").reindex(index=time)
```

### Comparing `loren_frank_data_processing-0.9.9.dev0/loren_frank_data_processing/track_segment_classification.py` & `loren_frank_data_processing-1.0.1/loren_frank_data_processing/track_segment_classification.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,228 +1,246 @@
 from math import sqrt
 
 import dask
 import networkx as nx
 import numpy as np
 import scipy.stats
 
-np.warnings.filterwarnings('ignore')
-
 
 def get_track_segments_from_graph(track_graph):
-    '''
+    """
 
     Parameters
     ----------
     track_graph : networkx Graph
 
     Returns
     -------
     track_segments : ndarray, shape (n_segments, n_nodes, n_space)
 
-    '''
-    node_positions = nx.get_node_attributes(track_graph, 'pos')
-    return np.asarray([(node_positions[node1], node_positions[node2])
-                       for node1, node2 in track_graph.edges()])
+    """
+    node_positions = nx.get_node_attributes(track_graph, "pos")
+    return np.asarray(
+        [
+            (node_positions[node1], node_positions[node2])
+            for node1, node2 in track_graph.edges()
+        ]
+    )
 
 
-def plot_track(track_graph, ax=None, **kwds):
-    '''
+def plot_track(track_graph, ax=None, draw_edge_labels=False, **kwds):
+    """
 
     Parameters
     ----------
     track_graph : networkx Graph
 
-    '''
-    node_position = nx.get_node_attributes(track_graph, 'pos')
+    """
+    node_position = nx.get_node_attributes(track_graph, "pos")
     nx.draw_networkx(track_graph, node_position, ax, **kwds)
 
+    if draw_edge_labels:
+        edge_ids = {edge: ind for ind, edge in enumerate(track_graph.edges)}
+        nx.draw_networkx_edge_labels(track_graph, node_position, edge_labels=edge_ids)
+
 
 def project_points_to_segment(track_segments, position):
-    '''Finds the closet point on a track segment in terms of Euclidean distance
+    """Finds the closet point on a track segment in terms of Euclidean distance
 
     Parameters
     ----------
     track_segments : ndarray, shape (n_segments, n_nodes, 2)
     position : ndarray, shape (n_time, 2)
 
     Returns
     -------
     projected_positions : ndarray, shape (n_time, n_segments, n_space)
 
-    '''
-    segment_diff = np.diff(track_segments, axis=1).squeeze()
-    sum_squares = np.sum(segment_diff ** 2, axis=1)
+    """
+    segment_diff = np.diff(track_segments, axis=1).squeeze(axis=1)
+    sum_squares = np.sum(segment_diff**2, axis=1)
     node1 = track_segments[:, 0, :]
-    nx = (np.sum(segment_diff *
-                 (position[:, np.newaxis, :] - node1), axis=2) /
-          sum_squares)
+    nx = (
+        np.sum(segment_diff * (position[:, np.newaxis, :] - node1), axis=2)
+        / sum_squares
+    )
     nx[np.where(nx < 0)] = 0.0
     nx[np.where(nx > 1)] = 1.0
     return node1[np.newaxis, ...] + (
-        nx[:, :, np.newaxis] * segment_diff[np.newaxis, ...])
+        nx[:, :, np.newaxis] * segment_diff[np.newaxis, ...]
+    )
 
 
 def find_projected_point_distance(track_segments, position):
-    '''
-    '''
+    """ """
     return np.linalg.norm(
-        position[:, np.newaxis, :] -
-        project_points_to_segment(track_segments, position), axis=2)
+        position[:, np.newaxis, :]
+        - project_points_to_segment(track_segments, position),
+        axis=2,
+    )
 
 
 def find_nearest_segment(track_segments, position):
-    '''Returns the track segment that is closest to the position
+    """Returns the track segment that is closest to the position
     at each time point.
 
     Parameters
     ----------
     track_segments : ndarray, shape (n_segments, n_nodes, n_space)
     position : ndarray, shape (n_time, n_space)
 
     Returns
     -------
     segment_id : ndarray, shape (n_time,)
 
-    '''
+    """
     distance = find_projected_point_distance(track_segments, position)
     return np.argmin(distance, axis=1)
 
 
 def euclidean_distance_change(position):
-    '''Distance between position at successive time points
+    """Distance between position at successive time points
 
     Parameters
     ----------
     position : ndarray, shape (n_time, n_space)
 
     Returns
     -------
     distance : ndarray, shape (n_time,)
 
-    '''
+    """
     distance = np.linalg.norm(position[1:] - position[:-1], axis=1)
     return np.concatenate(([np.nan], distance))
 
 
 def route_distance(candidates_t_1, candidates_t, track_graph):
-    '''
+    """
 
     Parameters
     ----------
     candidates_t_1 : ndarray, shape (n_segments, n_space)
     candidates_t : ndarray, shape (n_segments, n_space)
     track_graph : networkx Graph
 
     Returns
     -------
     route_distance : ndarray, shape (n_segments, n_segments)
 
-    '''
+    """
     # TODO: speedup function. This takes the most time
     n_segments = len(track_graph.edges)
     if np.any(np.isnan(candidates_t) | np.isnan(candidates_t)):
         return np.full((n_segments, n_segments), np.nan)
     node_names = []
     edges = list(track_graph.edges.keys())
     n_original_nodes = len(track_graph.nodes)
     # insert virtual node
     for edge_number, (position_t, position_t_1, (node1, node2)) in enumerate(
-            zip(candidates_t, candidates_t_1, edges)):
-        node_name_t, node_name_t_1 = f't_0_{edge_number}', f't_1_{edge_number}'
+        zip(candidates_t, candidates_t_1, edges)
+    ):
+        node_name_t, node_name_t_1 = f"t_0_{edge_number}", f"t_1_{edge_number}"
         node_names.append(node_name_t)
         node_names.append(node_name_t_1)
         nx.add_path(track_graph, [node1, node_name_t, node2])
         nx.add_path(track_graph, [node1, node_name_t_1, node2])
         nx.add_path(track_graph, [node_name_t, node_name_t_1])
-        track_graph.nodes[node_name_t]['pos'] = tuple(position_t)
-        track_graph.nodes[node_name_t_1]['pos'] = tuple(position_t_1)
+        track_graph.nodes[node_name_t]["pos"] = tuple(position_t)
+        track_graph.nodes[node_name_t_1]["pos"] = tuple(position_t_1)
 
     # calculate distance
     for node1, node2 in track_graph.edges:
-        x1, y1 = track_graph.nodes[node1]['pos']
-        x2, y2 = track_graph.nodes[node2]['pos']
-        track_graph.edges[(node1, node2)]['distance'] = sqrt(
-            (x2 - x1)**2 + (y2 - y1)**2)
+        x1, y1 = track_graph.nodes[node1]["pos"]
+        x2, y2 = track_graph.nodes[node2]["pos"]
+        track_graph.edges[(node1, node2)]["distance"] = sqrt(
+            (x2 - x1) ** 2 + (y2 - y1) ** 2
+        )
 
     # calculate path distance
     path_distance = scipy.sparse.csgraph.dijkstra(
-        nx.to_scipy_sparse_matrix(track_graph, weight='distance'))
+        nx.to_scipy_sparse_matrix(track_graph, weight="distance")
+    )
     n_total_nodes = len(track_graph.nodes)
     node_ind = np.arange(n_total_nodes)
     start_node_ind = node_ind[n_original_nodes::2]
-    end_node_ind = node_ind[n_original_nodes + 1::2]
+    end_node_ind = node_ind[n_original_nodes + 1 :: 2]
 
     track_graph.remove_nodes_from(node_names)
 
     return path_distance[start_node_ind][:, end_node_ind]
 
 
 def batch(n_samples, batch_size=1):
     for ind in range(0, n_samples, batch_size):
         yield range(ind, min(ind + batch_size, n_samples))
 
 
 @dask.delayed
-def batch_route_distance(track_graph, projected_track_position_t,
-                         projected_track_position_t_1):
+def batch_route_distance(
+    track_graph, projected_track_position_t, projected_track_position_t_1
+):
     copy_graph = track_graph.copy()
-    distances = [route_distance(p_t, p_t_1, copy_graph)
-                 for p_t, p_t_1 in zip(projected_track_position_t,
-                                       projected_track_position_t_1)]
+    distances = [
+        route_distance(p_t, p_t_1, copy_graph)
+        for p_t, p_t_1 in zip(projected_track_position_t, projected_track_position_t_1)
+    ]
     return np.stack(distances)
 
 
 def route_distance_change(position, track_graph):
     track_segments = get_track_segments_from_graph(track_graph)
-    projected_track_position = project_points_to_segment(
-        track_segments, position)
+    projected_track_position = project_points_to_segment(track_segments, position)
     n_segments = len(track_segments)
 
     distances = [np.full((1, n_segments, n_segments), np.nan)]
     projected_track_position_t = projected_track_position[1:]
     projected_track_position_t_1 = projected_track_position[:-1]
     n_time = projected_track_position_t.shape[0]
 
     for time_ind in batch(n_time, batch_size=10_000):
         distances.append(
             batch_route_distance(
-                track_graph, projected_track_position_t[time_ind],
-                projected_track_position_t_1[time_ind]))
+                track_graph,
+                projected_track_position_t[time_ind],
+                projected_track_position_t_1[time_ind],
+            )
+        )
 
-    return np.concatenate(dask.compute(
-        *distances, scheduler='processes'), axis=0)
+    return np.concatenate(dask.compute(*distances, scheduler="processes"), axis=0)
 
 
 def calculate_position_likelihood(position, track_graph, sigma=10):
     track_segments = get_track_segments_from_graph(track_graph)
     projected_position_distance = find_projected_point_distance(
-        track_segments, position)
-    return (np.exp(-0.5 * (projected_position_distance / sigma) ** 2) /
-            (np.sqrt(2 * np.pi) * sigma))
+        track_segments, position
+    )
+    return np.exp(-0.5 * (projected_position_distance / sigma) ** 2) / (
+        np.sqrt(2 * np.pi) * sigma
+    )
 
 
 def normalize_to_probability(x, axis=-1):
-    '''Ensure the array axis sum to 1
+    """Ensure the array axis sum to 1
 
     Parameters
     ----------
     x : ndarray
 
     Returns
     -------
     normalized_x : ndarray
 
-    '''
+    """
     return x / x.sum(axis=axis, keepdims=True)
 
 
-def calculate_empirical_state_transition(position, track_graph,
-                                         scaling=1E-1, diagonal_bias=1E-1):
-    '''Calculates the state transition probabilty between track segments by
+def calculate_empirical_state_transition(
+    position, track_graph, scaling=1e-1, diagonal_bias=1e-1
+):
+    """Calculates the state transition probabilty between track segments by
     favoring route distances that are similar to euclidean distances between
     successive time points.
 
     Parameters
     ----------
     position : ndarray, shape (n_time, n_space)
     track_graph : networkx Graph
@@ -235,83 +253,92 @@
     References
     ----------
     .. [1] Newson, P., and Krumm, J. (2009). Hidden Markov map matching through
     noise and sparseness. In Proceedings of the 17th ACM SIGSPATIAL
     International Conference on Advances in Geographic Information Systems,
     (ACM), pp. 336-343.
 
-    '''
+    """
     route_and_euclidean_distance_similarity = np.abs(
-        route_distance_change(position, track_graph) -
-        euclidean_distance_change(position)[:, np.newaxis, np.newaxis])
+        route_distance_change(position, track_graph)
+        - euclidean_distance_change(position)[:, np.newaxis, np.newaxis]
+    )
     exponential_pdf = scipy.stats.expon.pdf(
-        route_and_euclidean_distance_similarity, scale=scaling)
+        route_and_euclidean_distance_similarity, scale=scaling
+    )
     exponential_pdf = normalize_to_probability(exponential_pdf, axis=2)
 
     n_states = route_and_euclidean_distance_similarity.shape[1]
     exponential_pdf += np.identity(n_states)[np.newaxis] * diagonal_bias
 
     return normalize_to_probability(exponential_pdf, axis=2)
 
 
 def viterbi(initial_conditions, state_transition, likelihood):
-    '''Find the most likely sequence of paths using the Viterbi algorithm.
+    """Find the most likely sequence of paths using the Viterbi algorithm.
 
     Note that the state_transition matrix is time-dependent. NaNs are removed
     and placed back in at the end.
 
     Parameters
     ----------
     initial_conditions : ndarray, shape (n_states,)
     state_transition : ndarray, shape (n_time, n_states, n_states)
     likelihood : ndarray, shape (n_time, n_states)
 
     Returns
     -------
     state_id : ndarray, shape (n_time,)
 
-    '''
-    is_bad = (np.any(np.isnan(likelihood), axis=1) |
-              np.any(np.isnan(state_transition), axis=(1, 2)) |
-              np.any(np.isinf(np.log(likelihood)), axis=1))
+    """
+    is_bad = np.any(np.isnan(likelihood), axis=1) | np.any(
+        np.isinf(np.log(likelihood)), axis=1
+    )
     log_likelihood = np.log(likelihood.copy()[~is_bad])
     state_transition = np.log(state_transition.copy()[~is_bad])
 
     n_time, n_states = log_likelihood.shape
     posterior = np.zeros((n_time, n_states))
-    max_state_ind = np.zeros((n_time, n_states), dtype=np.int)
+    max_state_ind = np.zeros((n_time, n_states), dtype=int)
 
     # initialization
     posterior[0] = np.log(initial_conditions) + log_likelihood[0]
 
     # recursion
     for time_ind in range(1, n_time):
         prior = posterior[time_ind - 1] + state_transition[time_ind]
         max_state_ind[time_ind] = prior.argmax(axis=1)
-        posterior[time_ind] = prior[np.arange(
-            n_states), max_state_ind[time_ind]] + log_likelihood[time_ind]
+        posterior[time_ind] = (
+            prior[np.arange(n_states), max_state_ind[time_ind]]
+            + log_likelihood[time_ind]
+        )
 
     # termination
-    most_probable_state_ind = np.zeros((n_time,), dtype=np.int)
+    most_probable_state_ind = np.zeros((n_time,), dtype=int)
     most_probable_state_ind[n_time - 1] = np.argmax(posterior[n_time - 1])
 
     # path back-tracking
     for time_ind in reversed(range(n_time - 1)):
         most_probable_state_ind[time_ind] = max_state_ind[
-            time_ind + 1, most_probable_state_ind[time_ind + 1]]
+            time_ind + 1, most_probable_state_ind[time_ind + 1]
+        ]
 
     most_probable_state_ind_with_nan = np.full((is_bad.size,), np.nan)
     most_probable_state_ind_with_nan[~is_bad] = most_probable_state_ind
     return most_probable_state_ind_with_nan
 
 
-def classify_track_segments(track_graph, position, sensor_std_dev=10,
-                            route_euclidean_distance_scaling=1E-1,
-                            diagonal_bias=1E-1):
-    '''Find the most likely track segment for a given position.
+def classify_track_segments(
+    track_graph,
+    position,
+    sensor_std_dev=10,
+    route_euclidean_distance_scaling=1e-1,
+    diagonal_bias=1e-1,
+):
+    """Find the most likely track segment for a given position.
 
     Tries to make sure the euclidean distance between successive time points
     is similar to the route distance along the graph.
 
     Parameters
     ----------
     track_graph : networkx Graph
@@ -332,54 +359,55 @@
     References
     ----------
     .. [1] Newson, P., and Krumm, J. (2009). Hidden Markov map matching through
     noise and sparseness. In Proceedings of the 17th ACM SIGSPATIAL
     International Conference on Advances in Geographic Information Systems,
     (ACM), pp. 336-343.
 
-    '''
+    """
     n_segments = len(track_graph.edges)
     initial_conditions = np.ones((n_segments,))
     state_transition = calculate_empirical_state_transition(
-        position, track_graph, scaling=route_euclidean_distance_scaling,
-        diagonal_bias=diagonal_bias)
+        position,
+        track_graph,
+        scaling=route_euclidean_distance_scaling,
+        diagonal_bias=diagonal_bias,
+    )
     likelihood = calculate_position_likelihood(
-        position, track_graph, sigma=sensor_std_dev)
+        position, track_graph, sigma=sensor_std_dev
+    )
 
     return viterbi(initial_conditions, state_transition, likelihood)
 
 
-def batch_linear_distance(track_graph, projected_track_positions, edge_ids,
-                          well_id):
-
+def batch_linear_distance(track_graph, projected_track_positions, edge_ids, well_id):
     copy_graph = track_graph.copy()
     linear_distance = []
 
-    for (x3, y3), (node1, node2) in zip(
-            projected_track_positions, edge_ids):
-
-        x1, y1 = copy_graph.nodes[node1]['pos']
-        left_distance = sqrt((x3 - x1)**2 + (y3 - y1)**2)
-        nx.add_path(copy_graph, [node1, 'projected'], distance=left_distance)
-
-        x2, y2 = copy_graph.nodes[node2]['pos']
-        right_distance = sqrt((x3 - x2)**2 + (y3 - y2)**2)
-        nx.add_path(copy_graph, ['projected', node2], distance=right_distance)
+    for (x3, y3), (node1, node2) in zip(projected_track_positions, edge_ids):
+        x1, y1 = copy_graph.nodes[node1]["pos"]
+        left_distance = sqrt((x3 - x1) ** 2 + (y3 - y1) ** 2)
+        nx.add_path(copy_graph, [node1, "projected"], distance=left_distance)
+
+        x2, y2 = copy_graph.nodes[node2]["pos"]
+        right_distance = sqrt((x3 - x2) ** 2 + (y3 - y2) ** 2)
+        nx.add_path(copy_graph, ["projected", node2], distance=right_distance)
 
         linear_distance.append(
-            nx.shortest_path_length(copy_graph, source=well_id,
-                                    target='projected', weight='distance'))
-        copy_graph.remove_node('projected')
+            nx.shortest_path_length(
+                copy_graph, source=well_id, target="projected", weight="distance"
+            )
+        )
+        copy_graph.remove_node("projected")
 
     return linear_distance
 
 
-def calculate_linear_distance(track_graph, track_segment_id, well_id,
-                              position):
-    '''Finds the path distance along a graph relative to a node.
+def calculate_linear_distance(track_graph, track_segment_id, well_id, position):
+    """Finds the path distance along a graph relative to a node.
 
     Parameters
     ----------
     track_graph : networkx Graph
     track_segment_id : ndarray, shape (n_time,)
     well_id : hashable object
     position : ndarray, shape (n_time, n_spaces)
@@ -387,34 +415,41 @@
     Returns
     -------
     linear_distance : ndarray, shape (n_time,)
         Linear distance from well specified by `well_id`
     projected_track_position_x : ndarray, shape (n_time,)
     projected_track_position_y : ndarray, shape (n_time,)
 
-    '''
+    """
     is_nan = np.isnan(track_segment_id)
-    track_segment_id[np.isnan(track_segment_id)] = -1  # need to check
+    track_segment_id[is_nan] = 0  # need to check
     track_segment_id = track_segment_id.astype(int)
 
     track_segments = get_track_segments_from_graph(track_graph)
-    projected_track_positions = project_points_to_segment(
-        track_segments, position)
+    projected_track_positions = project_points_to_segment(track_segments, position)
     n_time = projected_track_positions.shape[0]
-    projected_track_positions = projected_track_positions[(
-        np.arange(n_time), track_segment_id)]
-    edge_ids = np.array(track_graph.edges)[track_segment_id]
+    projected_track_positions = projected_track_positions[
+        (np.arange(n_time), track_segment_id)
+    ]
+    edge_ids = np.asarray(list(track_graph.edges))[track_segment_id]
 
     linear_distance = []
 
     for time_ind in batch(n_time, batch_size=10_000):
         linear_distance.append(
             batch_linear_distance(
-                track_graph, projected_track_positions[time_ind],
-                edge_ids[time_ind], well_id))
-    linear_distance = np.concatenate(dask.compute(
-        *linear_distance, scheduler='processes'))
+                track_graph,
+                projected_track_positions[time_ind],
+                edge_ids[time_ind],
+                well_id,
+            )
+        )
+    linear_distance = np.concatenate(
+        dask.compute(*linear_distance, scheduler="processes")
+    )
     linear_distance[is_nan] = np.nan
 
-    return (linear_distance,
-            projected_track_positions[:, 0],
-            projected_track_positions[:, 1])
+    return (
+        linear_distance,
+        projected_track_positions[:, 0],
+        projected_track_positions[:, 1],
+    )
```

### Comparing `loren_frank_data_processing-0.9.9.dev0/loren_frank_data_processing.egg-info/SOURCES.txt` & `loren_frank_data_processing-1.0.1/loren_frank_data_processing.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 setup.cfg
 setup.py
 loren_frank_data_processing/DIO.py
 loren_frank_data_processing/__init__.py
 loren_frank_data_processing/core.py
 loren_frank_data_processing/multiunit.py
@@ -15,8 +16,10 @@
 loren_frank_data_processing/utilities.py
 loren_frank_data_processing/visualization.py
 loren_frank_data_processing/well_traversal_classification.py
 loren_frank_data_processing.egg-info/PKG-INFO
 loren_frank_data_processing.egg-info/SOURCES.txt
 loren_frank_data_processing.egg-info/dependency_links.txt
 loren_frank_data_processing.egg-info/requires.txt
-loren_frank_data_processing.egg-info/top_level.txt
+loren_frank_data_processing.egg-info/top_level.txt
+tests/test_core_.py
+tests/test_utilities.py
```

