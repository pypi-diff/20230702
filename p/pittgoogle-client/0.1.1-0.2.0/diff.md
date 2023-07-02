# Comparing `tmp/pittgoogle_client-0.1.1.tar.gz` & `tmp/pittgoogle_client-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pittgoogle_client-0.1.1.tar", max compression
+gzip compressed data, was "pittgoogle_client-0.2.0.tar", max compression
```

## Comparing `pittgoogle_client-0.1.1.tar` & `pittgoogle_client-0.2.0.tar`

### file list

```diff
@@ -1,9 +1,11 @@
--rw-r--r--   0        0        0     1516 2023-05-15 15:45:17.853955 pittgoogle_client-0.1.1/LICENSE.txt
--rw-r--r--   0        0        0      615 2023-05-15 15:45:17.853955 pittgoogle_client-0.1.1/README.md
--rw-r--r--   0        0        0      680 2023-05-15 15:45:17.857956 pittgoogle_client-0.1.1/pittgoogle/__init__.py
--rw-r--r--   0        0        0    23547 2023-05-15 15:45:17.857956 pittgoogle_client-0.1.1/pittgoogle/bigquery.py
--rw-r--r--   0        0        0     4287 2023-05-15 15:45:17.857956 pittgoogle_client-0.1.1/pittgoogle/figures.py
--rw-r--r--   0        0        0    12389 2023-05-15 15:45:17.857956 pittgoogle_client-0.1.1/pittgoogle/pubsub.py
--rw-r--r--   0        0        0     2177 2023-05-15 15:45:17.857956 pittgoogle_client-0.1.1/pittgoogle/utils.py
--rw-r--r--   0        0        0     1358 2023-05-15 15:45:39.595834 pittgoogle_client-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1982 1970-01-01 00:00:00.000000 pittgoogle_client-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1516 2023-07-02 19:17:47.061784 pittgoogle_client-0.2.0/LICENSE.txt
+-rw-r--r--   0        0        0      707 2023-07-02 19:17:47.061784 pittgoogle_client-0.2.0/README.md
+-rw-r--r--   0        0        0      725 2023-07-02 19:17:47.065784 pittgoogle_client-0.2.0/pittgoogle/__init__.py
+-rw-r--r--   0        0        0     7656 2023-07-02 19:17:47.065784 pittgoogle_client-0.2.0/pittgoogle/auth.py
+-rw-r--r--   0        0        0    23583 2023-07-02 19:17:47.065784 pittgoogle_client-0.2.0/pittgoogle/bigquery.py
+-rw-r--r--   0        0        0      128 2023-07-02 19:17:47.065784 pittgoogle_client-0.2.0/pittgoogle/exceptions.py
+-rw-r--r--   0        0        0     4433 2023-07-02 19:17:47.065784 pittgoogle_client-0.2.0/pittgoogle/figures.py
+-rw-r--r--   0        0        0    20332 2023-07-02 19:17:47.065784 pittgoogle_client-0.2.0/pittgoogle/pubsub.py
+-rw-r--r--   0        0        0     6116 2023-07-02 19:17:47.065784 pittgoogle_client-0.2.0/pittgoogle/utils.py
+-rw-r--r--   0        0        0     1397 2023-07-02 19:18:07.194018 pittgoogle_client-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2083 1970-01-01 00:00:00.000000 pittgoogle_client-0.2.0/PKG-INFO
```

### Comparing `pittgoogle_client-0.1.1/LICENSE.txt` & `pittgoogle_client-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pittgoogle_client-0.1.1/pittgoogle/__init__.py` & `pittgoogle_client-0.2.0/pittgoogle/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,22 @@
-"""Tools for interacting with Pitt-Google Broker data resources."""
+# -*- coding: UTF-8 -*-
+"""Tools for interacting with Pitt-Google Broker data resources on Google Cloud Platform."""
+import logging
+import os
 
 try:
     from importlib import metadata
 
 except ImportError:  # for Python<3.8
     import importlib_metadata as metadata
 
-import logging
-import os as os
-
-from . import bigquery, figures, pubsub, utils
+from . import auth, bigquery, exceptions, figures, pubsub, utils
 
-__version__ = metadata.version('pittgoogle-client')
+__version__ = metadata.version("pittgoogle-client")
 
 for var in ["GOOGLE_CLOUD_PROJECT", "GOOGLE_APPLICATION_CREDENTIALS"]:
     if var not in os.environ:
         logger = logging.getLogger(__name__)
         logger.warning(
             f"Warning: The environment variable {var} is not set. "
-            "This may impact your ability to connect to your "
-            "Google Cloud Platform project."
+            "This may impact your ability to connect to your Google Cloud Platform project."
         )
```

### Comparing `pittgoogle_client-0.1.1/pittgoogle/bigquery.py` & `pittgoogle_client-0.2.0/pittgoogle/bigquery.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,24 @@
+# -*- coding: UTF-8 -*-
 """The ``bigquery`` module facilitates querying Pitt-Google Broker's
 BigQuery databases and reading the results.
+See the tutorial for usage help.
 """
-
 from typing import Generator, List, Optional, Tuple, Union
 
 import astropy
 import pandas as pd
 from astropy import coordinates as coord
 from google.cloud import bigquery
 from tabulate import tabulate
 
-pgb_project_id = "ardent-cycling-243415"
+from .utils import ProjectIds
+
+
+pgb_project_id = ProjectIds.pittgoogle
 
 # --- BigQuery Client
 user_bq_client, user_project_id = None, None  # module's global Client, related id
 
 
 def create_client(project_id: str):
     """Open a BigQuery Client.
@@ -108,15 +112,15 @@
     stop = _create_client_if_needed()
     if stop:  # the user has chosen to exit rather than create a client
         return
 
     # get the table names in a list
     if table == "all":
         tables = get_dataset_table_names(dataset=dataset)
-    elif type(table) == str:
+    elif isinstance(table, str):
         tables = [table]
     else:
         tables = table
 
     # get and print info about each table
     for t in tables:
         df = get_table_schema(table=t, dataset=dataset)
@@ -289,15 +293,15 @@
         # wrap each objectId in quotes and join to single string
         oids = ",".join([f'"{o}"' for o in objectIds])
         wheres = f"WHERE objectId IN ({oids})"
         # concat the statements into a SQL query statement
         sqlquery = " ".join([sqlquery, wheres])
 
     # GROUP BY statement
-    groupbys = f"GROUP BY objectId"
+    groupbys = "GROUP BY objectId"
     sqlquery = " ".join([sqlquery, groupbys])
 
     # LIMIT statement
     if limit is not None:
         limits = f"LIMIT {limit}"
         sqlquery = " ".join([sqlquery, limits])
 
@@ -322,17 +326,15 @@
     fcols = list(set(columns) & set(flatcols))
     # list of requested columns nested under 'candidate'
     ncols = list(set(columns) - set(objectcols) - set(flatcols))
     ncols = [f"candidate.{c}" for c in ncols]
     # complete list of columns to be aggregated (group by) objectId
     aggcols = fcols + ncols
     # attach the ARRAY_AGG, ORDER By, and AS statements to the aggcols
-    aggcols = [
-        f'ARRAY_AGG({c} ORDER BY candidate.jd) AS {c.split(".")[-1]}' for c in aggcols
-    ]
+    aggcols = [f'ARRAY_AGG({c} ORDER BY candidate.jd) AS {c.split(".")[-1]}' for c in aggcols]
 
     return aggcols
 
 
 # --- Dry runs
 def dry_run(query: str, notify: bool = True):
     """Perform a dry run to find out how many bytes the query will process.
@@ -343,17 +345,17 @@
     global user_project_id
     _check_client_isinstance()  # make sure we have a bigquery.client
 
     job_config = bigquery.QueryJobConfig(dry_run=True, use_query_cache=False)
     query_job = user_bq_client.query(query, job_config=job_config)
 
     if notify:
-        nbytes, TiB = query_job.total_bytes_processed, 2 ** 40
+        nbytes, TiB = query_job.total_bytes_processed, 2**40
         pTiB = nbytes / TiB * 100  # nbytes as a percent of 1 TiB
-        print(f"\nQuery statement:")
+        print("\nQuery statement:")
         print(f'\n"{query}"\n')
         print(f"will process {nbytes} bytes of data.")
         print(f"({pTiB:.3}% of your 1 TiB Free Tier monthly allotment.)")
 
 
 def _dry_run_and_confirm(query: str) -> bool:
     # print dry run info
@@ -421,17 +423,15 @@
     # make the API call
     query_job = user_bq_client.query(query)
 
     # return the results
     if format == "query_job":
         return query_job
     elif iterator:  # return a generator that cycles through the objects/rows
-        return (
-            format_history_query_results(row=row, format=format) for row in query_job
-        )
+        return (format_history_query_results(row=row, format=format) for row in query_job)
     else:  # format and return all rows at once
         return format_history_query_results(query_job=query_job, format=format)
 
 
 def _query_objects_check_history_column_names(columns: List[str]) -> List[str]:
     """Make sure user-submitted column names are appropriate for `query_objects()`.
 
@@ -510,15 +510,15 @@
 def _format_history_query_results_to_df(query_job: bigquery.job.QueryJob):
     """Convert a query_job (containing multiple rows of object history data)
     to a DataFrame.
     Any duplicate observations will be dropped.
     """
 
     dflist = []
-    for r, row in enumerate(query_job):
+    for row in query_job:
         # convert to DataFrame
         df = _format_history_row_to_df(row)
         # add the objectId so we can use it to multi-index
         df["objectId"] = df.objectId
         # set the multi-index and append to the list
         dflist.append(df.reset_index().set_index(["objectId", "candid"]))
```

### Comparing `pittgoogle_client-0.1.1/pittgoogle/figures.py` & `pittgoogle_client-0.2.0/pittgoogle/figures.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
+# -*- coding: UTF-8 -*-
 """``figures`` contains functions for plotting alert and history data.
+See the tutorials for usage help.
 """
-
 import gzip
 import io
 from typing import Optional
 
 import aplpy
 import matplotlib as mpl
 import numpy as np
@@ -91,14 +92,15 @@
                 subplot = (1, 1, 1)
             ffig = aplpy.FITSFigure(hdul[0], figure=fig, subplot=subplot, **kwargs)
 
             # the following has been throwing: `ValueError: a must be > 0 and <= 1`
             # this is fixed by requiring astropy==3.2.1
             # Note: I see this related thing: https://github.com/aplpy/aplpy/issues/420
             # but I am using the latest APLpy version (2.0.3).
+            # update (2023-06-26): this seems to be working now with astropy==5.2.2
             ffig.show_grayscale(stretch="arcsinh")
     return ffig
 
 
 def plot_cutouts(alert_dict):
     """Adapted from:
     https://github.com/ZwickyTransientFacility/ztf-avro-alert/blob/master/notebooks/Filtering_alerts.ipynb
@@ -115,13 +117,13 @@
 # --- Plot all
 def plot_lightcurve_cutouts(alert_dict):
     """Adapted from:
     https://github.com/ZwickyTransientFacility/ztf-avro-alert/blob/master/notebooks/Filtering_alerts.ipynb
     """
 
     fig = plt.figure(figsize=(16, 4))
-    dflc = pgbu.alert_dict_to_dataframe(alert_dict)
+    dflc = pgbu.Cast.alert_dict_to_dataframe(alert_dict)
     plot_lightcurve(dflc, ax=plt.subplot(1, 4, 1))
     for i, cutout in enumerate(["Science", "Template", "Difference"]):
         stamp = alert_dict["cutout{}".format(cutout)]["stampData"]
         ffig = plot_stamp(stamp, fig=fig, subplot=(1, 4, i + 2))
         ffig.set_title(cutout)
```

### Comparing `pittgoogle_client-0.1.1/pyproject.toml` & `pittgoogle_client-0.2.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "pittgoogle-client"
 repository = "https://github.com/mwvgroup/pittgoogle-client"
-version = "0.1.1"
+version = "0.2.0"
 description = "Client utilities for the Pitt-Google astronomical alert broker."
 keywords = ["astronomy", "alert", "broker", "rubin"]
 authors = ["MWV Research Group"]
 license = "BSD-3-Clause"
 readme = "README.md"
 packages = [{ include = "pittgoogle" }]
 classifiers = [
@@ -21,16 +21,18 @@
     "Programming Language :: Python :: 3 :: Only",
     "Typing :: Typed"
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 aplpy = "^2.1"
+attrs = "*"
 astropy = ">=4.0"
 fastavro = "^1.4"
+google-auth-oauthlib = "*"
 google-cloud-bigquery = "^3.7"
 google-cloud-pubsub = "^2.15"
 matplotlib = "^3.5"
 numpy = "^1.20.0"
 pandas = "^1.3"
 tabulate = "^0.9"
```

### Comparing `pittgoogle_client-0.1.1/PKG-INFO` & `pittgoogle_client-0.2.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,43 +1,49 @@
 Metadata-Version: 2.1
 Name: pittgoogle-client
-Version: 0.1.1
+Version: 0.2.0
 Summary: Client utilities for the Pitt-Google astronomical alert broker.
 Home-page: https://github.com/mwvgroup/pittgoogle-client
 License: BSD-3-Clause
 Keywords: astronomy,alert,broker,rubin
 Author: MWV Research Group
 Requires-Python: >=3.8,<4.0
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Typing :: Typed
 Requires-Dist: aplpy (>=2.1,<3.0)
 Requires-Dist: astropy (>=4.0)
+Requires-Dist: attrs
 Requires-Dist: fastavro (>=1.4,<2.0)
+Requires-Dist: google-auth-oauthlib
 Requires-Dist: google-cloud-bigquery (>=3.7,<4.0)
 Requires-Dist: google-cloud-pubsub (>=2.15,<3.0)
 Requires-Dist: matplotlib (>=3.5,<4.0)
 Requires-Dist: numpy (>=1.20.0,<2.0.0)
 Requires-Dist: pandas (>=1.3,<2.0)
 Requires-Dist: tabulate (>=0.9,<0.10)
 Project-URL: Repository, https://github.com/mwvgroup/pittgoogle-client
 Description-Content-Type: text/markdown
 
+.. image:: https://readthedocs.org/projects/pitt-broker/badge/?version=latest
+:target: https://pitt-broker.readthedocs.io/en/latest/?badge=latest
+:alt: Documentation Status
+:style: flat-square
+
 # pittgoogle-client
 
 [![](https://app.codacy.com/project/badge/Grade/ec909deaf09840f3b3f645f045dea468)](https://app.codacy.com/gh/mwvgroup/pittgoogle-client/dashboard)
 [![](https://app.codacy.com/project/badge/Coverage/ec909deaf09840f3b3f645f045dea468)](https://app.codacy.com/gh/mwvgroup/pittgoogle-client/dashboard)
 
+Read the docs: [http://pittgoogle-client.rtfd.io/](http://pittgoogle-client.rtfd.io/).
+
 This is the client package for the
-[Pitt-Google astronomical alert broker](https://pitt-broker.readthedocs.io/en/latest/index.html).
-It contains tools for interacting with Pitt-Google Broker data resources.
-Read the docs at [http://pittgoogle-client.rtfd.io/](http://pittgoogle-client.rtfd.io/).
+[Pitt-Google astronomical alert broker](https://pitt-broker.rtfd.io/).
```

