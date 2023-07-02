# Comparing `tmp/tradingcomdados-1.1.1.tar.gz` & `tmp/tradingcomdados-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tradingcomdados-1.1.1.tar", last modified: Mon Jun 26 18:45:41 2023, max compression
+gzip compressed data, was "tradingcomdados-1.2.1.tar", last modified: Sun Jul  2 18:18:24 2023, max compression
```

## Comparing `tradingcomdados-1.1.1.tar` & `tradingcomdados-1.2.1.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-26 18:45:41.744973 tradingcomdados-1.1.1/
--rw-rw-rw-   0        0        0     1702 2023-06-26 18:45:41.744973 tradingcomdados-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     1500 2023-06-26 00:40:07.000000 tradingcomdados-1.1.1/README.md
--rw-rw-rw-   0        0        0      452 2023-06-26 00:54:22.000000 tradingcomdados-1.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-26 18:45:41.745973 tradingcomdados-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0      627 2023-05-23 23:49:47.000000 tradingcomdados-1.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-26 18:45:41.735842 tradingcomdados-1.1.1/tradingcomdados/
--rw-rw-rw-   0        0        0        0 2023-05-05 15:34:18.000000 tradingcomdados-1.1.1/tradingcomdados/__init__.py
--rw-rw-rw-   0        0        0    12162 2023-06-26 00:40:07.000000 tradingcomdados-1.1.1/tradingcomdados/data_provider.py
--rw-rw-rw-   0        0        0     6347 2023-06-20 01:15:28.000000 tradingcomdados-1.1.1/tradingcomdados/unsupervised_learning.py
-drwxrwxrwx   0        0        0        0 2023-06-26 18:45:41.743971 tradingcomdados-1.1.1/tradingcomdados.egg-info/
--rw-rw-rw-   0        0        0     1702 2023-06-26 18:45:41.000000 tradingcomdados-1.1.1/tradingcomdados.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      329 2023-06-26 18:45:41.000000 tradingcomdados-1.1.1/tradingcomdados.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-26 18:45:41.000000 tradingcomdados-1.1.1/tradingcomdados.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      131 2023-06-26 18:45:41.000000 tradingcomdados-1.1.1/tradingcomdados.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-06-26 18:45:41.000000 tradingcomdados-1.1.1/tradingcomdados.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-02 18:18:23.974869 tradingcomdados-1.2.1/
+-rw-rw-rw-   0        0        0     1702 2023-07-02 18:18:23.973869 tradingcomdados-1.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1500 2023-06-26 00:40:07.000000 tradingcomdados-1.2.1/README.md
+-rw-rw-rw-   0        0        0      452 2023-07-02 18:17:22.000000 tradingcomdados-1.2.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-02 18:18:23.974869 tradingcomdados-1.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      627 2023-05-23 23:49:47.000000 tradingcomdados-1.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-02 18:18:15.580250 tradingcomdados-1.2.1/tradingcomdados/
+-rw-rw-rw-   0        0        0        0 2023-05-05 15:34:18.000000 tradingcomdados-1.2.1/tradingcomdados/__init__.py
+-rw-rw-rw-   0        0        0     2080 2023-07-02 18:17:22.000000 tradingcomdados-1.2.1/tradingcomdados/alternative_data.py
+-rw-rw-rw-   0        0        0    12204 2023-07-02 18:17:22.000000 tradingcomdados-1.2.1/tradingcomdados/data_provider.py
+-rw-rw-rw-   0        0        0    37098 2023-07-02 18:17:22.000000 tradingcomdados-1.2.1/tradingcomdados/ta_indicators.py
+-rw-rw-rw-   0        0        0     6347 2023-06-20 01:15:28.000000 tradingcomdados-1.2.1/tradingcomdados/unsupervised_learning.py
+drwxrwxrwx   0        0        0        0 2023-07-02 18:18:23.972869 tradingcomdados-1.2.1/tradingcomdados.egg-info/
+-rw-rw-rw-   0        0        0     1702 2023-07-02 18:18:13.000000 tradingcomdados-1.2.1/tradingcomdados.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      398 2023-07-02 18:18:14.000000 tradingcomdados-1.2.1/tradingcomdados.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-02 18:18:13.000000 tradingcomdados-1.2.1/tradingcomdados.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      131 2023-07-02 18:18:13.000000 tradingcomdados-1.2.1/tradingcomdados.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-07-02 18:18:13.000000 tradingcomdados-1.2.1/tradingcomdados.egg-info/top_level.txt
```

### Comparing `tradingcomdados-1.1.1/PKG-INFO` & `tradingcomdados-1.2.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tradingcomdados
-Version: 1.1.1
+Version: 1.2.1
 Summary: tradingcomdados
 Author: Lucas Roberto Correa
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # tradingcomdados
```

### Comparing `tradingcomdados-1.1.1/README.md` & `tradingcomdados-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `tradingcomdados-1.1.1/setup.py` & `tradingcomdados-1.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `tradingcomdados-1.1.1/tradingcomdados/data_provider.py` & `tradingcomdados-1.2.1/tradingcomdados/data_provider.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,14 +22,15 @@
             logger.exception(
                 f"Exception raised in {func.__name__}. exception: {str(e)}"
             )
             raise e
 
     return wrapper
 
+
 @_logging_error
 def _run_request(
     data_type: str,
     request_type: str,
     ticker: str,
     date_begin: str,
     date_end: str,
@@ -77,14 +78,15 @@
         return res
 
     except:
         print(
             "An error occured during the process of gathering data, please check the ticker and dates used and also remember to use a valid api key"
         )
 
+
 @_logging_error
 def _run_request_report(
     data_type: str,
     request_type: str,
     ticker: str,
     date_begin: str,
     trimester: str,
@@ -122,14 +124,15 @@
         return res
 
     except:
         print(
             "An error occured during the process of gathering data, please check the ticker and dates used and also remember to use a valid api key"
         )
 
+
 @_logging_error
 def _request_type_validation(data_type, request_type, ticker):
 
     try:
         url_base = "https://api.fintz.com.br"
 
         if data_type == "stock":
@@ -201,28 +204,30 @@
         return endpoint
 
     except:
         return print(
             "Input request_type option not found, take a look at the documentation."
         )
 
+
 @_logging_error
 def _transform_to_dataframe(res, request_type):
     try:
         if request_type != "treasury_historical":
             df = pd.json_normalize(res)
 
         else:
             df = pd.DataFrame.from_dict(res["dados"])
 
         return df
 
     except:
         print("An error occured converting data from JSON to pandas DataFrame.")
 
+
 @_logging_error
 def get_data(
     data_type: str,
     request_type: str,
     ticker: str,
     date_begin: str,
     date_end: str,
@@ -264,14 +269,15 @@
     res = _run_request(
         data_type, request_type, ticker, date_begin, date_end, api_key, endpoint
     )
     df = _transform_to_dataframe(res, request_type)
 
     return df
 
+
 @_logging_error
 def get_data_tickers(
     data_type: str,
     request_type: str,
     tickers: list,
     date_begin: str,
     date_end: str,
@@ -301,14 +307,15 @@
 
     for i in tickers:
         temp = get_data(data_type, request_type, i, date_begin, date_end, api_key)
         df = pd.concat([df, temp], ignore_index=True)
 
     return df
 
+
 @_logging_error
 def get_data_report(
     data_type: str,
     request_type: str,
     ticker: str,
     date_begin: str,
     trimester: str,
@@ -346,14 +353,15 @@
     res = _run_request_report(
         data_type, request_type, ticker, date_begin, trimester, api_key, endpoint
     )
     df = _transform_to_dataframe(res, request_type)
 
     return df
 
+
 @_logging_error
 def get_data_report_tickers(
     data_type: str,
     request_type: str,
     tickers: list,
     date_begin: str,
     trimester: str,
@@ -378,11 +386,13 @@
     :return: DataFrame that contains the results for all tickers in the date range requested
     :rtype: DataFrame
     """
 
     df = pd.DataFrame()
 
     for i in tickers:
-        temp = get_data_report(data_type, request_type, i, date_begin, trimester, api_key)
+        temp = get_data_report(
+            data_type, request_type, i, date_begin, trimester, api_key
+        )
         df = pd.concat([df, temp], ignore_index=True)
 
-    return df
+    return df
```

### Comparing `tradingcomdados-1.1.1/tradingcomdados/unsupervised_learning.py` & `tradingcomdados-1.2.1/tradingcomdados/unsupervised_learning.py`

 * *Files identical despite different names*

### Comparing `tradingcomdados-1.1.1/tradingcomdados.egg-info/PKG-INFO` & `tradingcomdados-1.2.1/tradingcomdados.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tradingcomdados
-Version: 1.1.1
+Version: 1.2.1
 Summary: tradingcomdados
 Author: Lucas Roberto Correa
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # tradingcomdados
```

