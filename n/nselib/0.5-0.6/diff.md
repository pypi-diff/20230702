# Comparing `tmp/nselib-0.5.tar.gz` & `tmp/nselib-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nselib-0.5.tar", last modified: Sat Jun 24 15:00:36 2023, max compression
+gzip compressed data, was "nselib-0.6.tar", last modified: Sun Jul  2 18:16:47 2023, max compression
```

## Comparing `nselib-0.5.tar` & `nselib-0.6.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-06-24 15:00:36.901224 nselib-0.5/
--rw-rw-rw-   0        0        0    11558 2023-06-18 02:00:39.000000 nselib-0.5/LICENSE
--rw-rw-rw-   0        0        0        0 2023-06-18 00:57:58.000000 nselib-0.5/MANIFEST.in
--rw-rw-rw-   0        0        0     4004 2023-06-24 15:00:36.901224 nselib-0.5/PKG-INFO
--rw-rw-rw-   0        0        0     3311 2023-06-24 14:56:54.000000 nselib-0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-06-24 15:00:36.748499 nselib-0.5/nselib/
--rw-rw-rw-   0        0        0       68 2023-06-24 14:50:51.000000 nselib-0.5/nselib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-24 15:00:36.792185 nselib-0.5/nselib/capital_market/
--rw-rw-rw-   0        0        0      330 2023-06-24 13:55:00.000000 nselib-0.5/nselib/capital_market/__init__.py
--rw-rw-rw-   0        0        0    23344 2023-06-24 14:49:21.000000 nselib-0.5/nselib/capital_market/capital_market_data.py
--rw-rw-rw-   0        0        0     2556 2023-06-24 10:49:29.000000 nselib-0.5/nselib/constants.py
-drwxrwxrwx   0        0        0        0 2023-06-24 15:00:36.828662 nselib-0.5/nselib/debt/
--rw-rw-rw-   0        0        0        0 2023-06-18 00:50:56.000000 nselib-0.5/nselib/debt/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-24 15:00:36.864619 nselib-0.5/nselib/derivatives/
--rw-rw-rw-   0        0        0      273 2023-06-24 14:43:31.000000 nselib-0.5/nselib/derivatives/__init__.py
--rw-rw-rw-   0        0        0    16766 2023-06-24 14:49:21.000000 nselib-0.5/nselib/derivatives/derivative_data.py
--rw-rw-rw-   0        0        0     4841 2023-06-24 10:07:44.000000 nselib-0.5/nselib/libutil.py
--rw-rw-rw-   0        0        0      438 2023-06-18 06:43:26.000000 nselib-0.5/nselib/logger.py
-drwxrwxrwx   0        0        0        0 2023-06-24 15:00:36.755435 nselib-0.5/nselib.egg-info/
--rw-rw-rw-   0        0        0     4004 2023-06-24 15:00:36.000000 nselib-0.5/nselib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      443 2023-06-24 15:00:36.000000 nselib-0.5/nselib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-24 15:00:36.000000 nselib-0.5/nselib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-06-24 15:00:36.000000 nselib-0.5/nselib.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-24 15:00:36.000000 nselib-0.5/nselib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-06-24 15:00:36.902261 nselib-0.5/setup.cfg
--rw-rw-rw-   0        0        0     1011 2023-06-24 14:50:51.000000 nselib-0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-02 18:16:47.012832 nselib-0.6/
+-rw-rw-rw-   0        0        0    11558 2023-06-18 02:00:39.000000 nselib-0.6/LICENSE
+-rw-rw-rw-   0        0        0        0 2023-06-18 00:57:58.000000 nselib-0.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     4060 2023-07-02 18:16:47.012832 nselib-0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     3367 2023-07-02 18:13:29.000000 nselib-0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-07-02 18:16:46.784550 nselib-0.6/nselib/
+-rw-rw-rw-   0        0        0       68 2023-07-02 18:09:49.000000 nselib-0.6/nselib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-02 18:16:46.866511 nselib-0.6/nselib/capital_market/
+-rw-rw-rw-   0        0        0      356 2023-07-02 12:56:09.000000 nselib-0.6/nselib/capital_market/__init__.py
+-rw-rw-rw-   0        0        0    24350 2023-07-02 13:11:04.000000 nselib-0.6/nselib/capital_market/capital_market_data.py
+-rw-rw-rw-   0        0        0     2556 2023-06-24 10:49:29.000000 nselib-0.6/nselib/constants.py
+drwxrwxrwx   0        0        0        0 2023-07-02 18:16:46.907686 nselib-0.6/nselib/debt/
+-rw-rw-rw-   0        0        0        0 2023-06-18 00:50:56.000000 nselib-0.6/nselib/debt/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-02 18:16:46.974428 nselib-0.6/nselib/derivatives/
+-rw-rw-rw-   0        0        0      273 2023-06-24 14:43:31.000000 nselib-0.6/nselib/derivatives/__init__.py
+-rw-rw-rw-   0        0        0    16743 2023-07-02 12:58:11.000000 nselib-0.6/nselib/derivatives/derivative_data.py
+-rw-rw-rw-   0        0        0     4841 2023-06-24 10:07:44.000000 nselib-0.6/nselib/libutil.py
+-rw-rw-rw-   0        0        0      438 2023-06-18 06:43:26.000000 nselib-0.6/nselib/logger.py
+drwxrwxrwx   0        0        0        0 2023-07-02 18:16:46.825862 nselib-0.6/nselib.egg-info/
+-rw-rw-rw-   0        0        0     4060 2023-07-02 18:16:46.000000 nselib-0.6/nselib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      443 2023-07-02 18:16:46.000000 nselib-0.6/nselib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-02 18:16:46.000000 nselib-0.6/nselib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-07-02 18:16:46.000000 nselib-0.6/nselib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-02 18:16:46.000000 nselib-0.6/nselib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-07-02 18:16:47.013832 nselib-0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1011 2023-07-02 18:10:38.000000 nselib-0.6/setup.py
```

### Comparing `nselib-0.5/LICENSE` & `nselib-0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `nselib-0.5/PKG-INFO` & `nselib-0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nselib
-Version: 0.5
+Version: 0.6
 Summary: library to get NSE India data
 Home-page: https://github.com/RuchiTanmay/nselib
 Author: RuchiTanmay
 Author-email: ruchitanmay@gmail.com
 Keywords: nseindia,nse,python,sdk,trading,stock markets
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# NSElib 0.5
+# NSElib 0.6
 Python Library to get publicly available data on new NSE india website.
 
 Release Notes
 * Compatible and Tested with Python 3.8 and above 
 * Future release will be done on requirement basic
 
 ## Libraries Required
@@ -63,14 +63,16 @@
 * bhav_copy_with_delivery
 * bhav_copy_equities
 * equity_list
 * fno_equity_list
 * nifty50_equity_list
 * india_vix_data
 * index_data
+* market_watch_all_indices
+* fii_dii_trading_activity
 
 Example : 
 
 from nselib import capital_market 
 
 data = capital_market.price_volume_and_deliverable_position_data(symbol='SBIN', from_date='01-06-2023', to_date='10-06-2023')
```

### Comparing `nselib-0.5/README.md` & `nselib-0.6/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# NSElib 0.5
+# NSElib 0.6
 Python Library to get publicly available data on new NSE india website.
 
 Release Notes
 * Compatible and Tested with Python 3.8 and above 
 * Future release will be done on requirement basic
 
 ## Libraries Required
@@ -45,14 +45,16 @@
 * bhav_copy_with_delivery
 * bhav_copy_equities
 * equity_list
 * fno_equity_list
 * nifty50_equity_list
 * india_vix_data
 * index_data
+* market_watch_all_indices
+* fii_dii_trading_activity
 
 Example : 
 
 from nselib import capital_market 
 
 data = capital_market.price_volume_and_deliverable_position_data(symbol='SBIN', from_date='01-06-2023', to_date='10-06-2023')
```

### Comparing `nselib-0.5/nselib/capital_market/capital_market_data.py` & `nselib-0.6/nselib/capital_market/capital_market_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -367,19 +367,24 @@
         from_date = from_date + dt.timedelta(365)
         load_days = (to_date - from_date).days
         nse_df = pd.concat([nse_df, data_df], ignore_index=True)
     return nse_df
 
 
 def get_short_selling_data(from_date: str, to_date: str):
+    """
+    NSE short selling data in data frame
+    :param from_date:
+    :param to_date:
+    :return:
+    """
     # print(from_date, to_date)
     url = "https://www.nseindia.com/api/historical/short-selling?"
     payload = f"from={from_date}&to={to_date}&csv=true"
     data_text = nse_urlfetch(url + payload).text
-    print((url + payload))
     # data_text = data_text.replace('\x82','').replace('â¹', 'In Rs')
     with open('file.csv', 'w') as f:
         f.write(data_text)
     f.close()
     data_df = pd.read_csv('file.csv')
     data_df.columns = [name.replace(' ', '') for name in data_df.columns]
     return data_df
@@ -489,12 +494,38 @@
         data_df = pd.read_csv("https://archives.nseindia.com/content/indices/ind_nifty50list.csv")
     except Exception as e:
         raise FileNotFoundError(f' equities under NIFTY 50 index not found :: NSE error : {e}')
     data_df = data_df[['Company Name', 'Industry', 'Symbol']]
     return data_df
 
 
+def market_watch_all_indices():
+    """
+    Market Watch - Indices of the day in data frame
+    :return: pd.DataFrame
+    """
+    url = "https://www.nseindia.com/api/allIndices"
+    data_json = nse_urlfetch(url).json()
+    data_df = pd.DataFrame(data_json['data'])
+    return data_df[['key', 'index', 'indexSymbol', 'last', 'variation', 'percentChange', 'open', 'high', 'low',
+                   'previousClose', 'yearHigh', 'yearLow', 'pe', 'pb', 'dy', 'declines', 'advances', 'unchanged',
+                   'perChange365d', 'perChange30d', 'previousDay', 'oneWeekAgo', 'oneMonthAgo', 'oneYearAgo']]
+
+
+def fii_dii_trading_activity():
+    """
+    FII and DII trading activity of the day in data frame
+    :return: pd.DataFrame
+    """
+    url = "https://www.nseindia.com/api/fiidiiTradeReact"
+    data_json = nse_urlfetch(url).json()
+    data_df = pd.DataFrame(data_json)
+    return data_df
+
+
 # if __name__ == '__main__':
     # import nselib.capital_market as cm
-    # data = index_data(index='NIFTY 50', from_date='23-08-2022', to_date='23-06-2023')
+    # data = fii_dii_trading_activity()
+    # print(data)
+    # print(data.columns)
     # data = fno_equity_list()  #from_date='23-03-2022', to_date='23-06-2023'
```

### Comparing `nselib-0.5/nselib/constants.py` & `nselib-0.6/nselib/constants.py`

 * *Files identical despite different names*

### Comparing `nselib-0.5/nselib/derivatives/derivative_data.py` & `nselib-0.6/nselib/derivatives/derivative_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import pandas as pd
 import datetime as dt
-import time
 import zipfile
-from io import BytesIO, StringIO
+from io import BytesIO
 from nselib.libutil import *
 from nselib.constants import *
 
 
 def future_price_volume_data(symbol: str, instrument: str, from_date: str = None, to_date: str = None,
                              period: str = None):
     """
@@ -244,16 +243,17 @@
     get live nse option chain.
     :param symbol: eg:SBIN/BANKNIFTY
     :param expiry_date: '01-06-2023'
     :param oi_mode: eg: full/compact
     :return: pands dataframe
     """
     payload = get_nse_option_chain(symbol).json()
-    exp_date = pd.to_datetime(expiry_date, format='%d-%m-%Y')
-    expiry_date = exp_date.strftime('%d-%b-%Y')
+    if expiry_date:
+        exp_date = pd.to_datetime(expiry_date, format='%d-%m-%Y')
+        expiry_date = exp_date.strftime('%d-%b-%Y')
 
     if oi_mode == 'compact':
         col_names = ['Fetch_Time', 'Symbol', 'Expiry_Date', 'CALLS_OI', 'CALLS_Chng_in_OI', 'CALLS_Volume', 'CALLS_IV',
                      'CALLS_LTP', 'CALLS_Net_Chng', 'Strike_Price', 'PUTS_OI', 'PUTS_Chng_in_OI', 'PUTS_Volume',
                      'PUTS_IV', 'PUTS_LTP', 'PUTS_Net_Chng']
     else:
         col_names = ['Fetch_Time', 'Symbol', 'Expiry_Date', 'CALLS_OI', 'CALLS_Chng_in_OI', 'CALLS_Volume', 'CALLS_IV',
@@ -265,15 +265,15 @@
 
     oi_row = {'Fetch_Time': None, 'Symbol': None, 'Expiry_Date': None, 'CALLS_OI': 0, 'CALLS_Chng_in_OI': 0, 'CALLS_Volume': 0,
               'CALLS_IV': 0, 'CALLS_LTP': 0, 'CALLS_Net_Chng': 0, 'CALLS_Bid_Qty': 0, 'CALLS_Bid_Price': 0,
               'CALLS_Ask_Price': 0, 'CALLS_Ask_Qty': 0, 'Strike_Price': 0, 'PUTS_OI': 0, 'PUTS_Chng_in_OI': 0,
               'PUTS_Volume': 0, 'PUTS_IV': 0, 'PUTS_LTP': 0, 'PUTS_Net_Chng': 0, 'PUTS_Bid_Qty': 0,
               'PUTS_Bid_Price': 0, 'PUTS_Ask_Price': 0, 'PUTS_Ask_Qty': 0}
 
-    print(expiry_date)
+    # print(expiry_date)
     for m in range(len(payload['records']['data'])):
         if not expiry_date or (payload['records']['data'][m]['expiryDate'] == expiry_date):
             try:
                 oi_row['Expiry_Date'] = payload['records']['data'][m]['expiryDate']
                 oi_row['CALLS_OI'] = payload['records']['data'][m]['CE']['openInterest']
                 oi_row['CALLS_Chng_in_OI'] = payload['records']['data'][m]['CE']['changeinOpenInterest']
                 oi_row['CALLS_Volume'] = payload['records']['data'][m]['CE']['totalTradedVolume']
@@ -319,12 +319,12 @@
             oi_data = pd.concat([oi_data, pd.DataFrame([oi_row])], ignore_index=True)
             oi_data['Symbol'] = symbol
             oi_data['Fetch_Time'] = payload['records']['timestamp']
     return oi_data
 
 
 # if __name__ == '__main__':
-    #     df = future_price_volume_data("BANKNIFTY", "FUTIDX", from_date='17-06-2023', to_date='19-06-2023', period='1D')
-    #     df = participant_wise_trading_volume(trade_date='03-04-2023')
-    #     print(df)
-    #     print(df[df['EXPIRY_DT']=='27-Jul-2023'])
+    # df = future_price_volume_data("BANKNIFTY", "FUTIDX", from_date='17-06-2023', to_date='19-06-2023', period='1D')
+    # df = nse_live_option_chain(symbol='BANKNIFTY')
+    # print(df)
+    # print(df[df['EXPIRY_DT']=='27-Jul-2023'])
```

### Comparing `nselib-0.5/nselib/libutil.py` & `nselib-0.6/nselib/libutil.py`

 * *Files identical despite different names*

### Comparing `nselib-0.5/nselib.egg-info/PKG-INFO` & `nselib-0.6/nselib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nselib
-Version: 0.5
+Version: 0.6
 Summary: library to get NSE India data
 Home-page: https://github.com/RuchiTanmay/nselib
 Author: RuchiTanmay
 Author-email: ruchitanmay@gmail.com
 Keywords: nseindia,nse,python,sdk,trading,stock markets
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# NSElib 0.5
+# NSElib 0.6
 Python Library to get publicly available data on new NSE india website.
 
 Release Notes
 * Compatible and Tested with Python 3.8 and above 
 * Future release will be done on requirement basic
 
 ## Libraries Required
@@ -63,14 +63,16 @@
 * bhav_copy_with_delivery
 * bhav_copy_equities
 * equity_list
 * fno_equity_list
 * nifty50_equity_list
 * india_vix_data
 * index_data
+* market_watch_all_indices
+* fii_dii_trading_activity
 
 Example : 
 
 from nselib import capital_market 
 
 data = capital_market.price_volume_and_deliverable_position_data(symbol='SBIN', from_date='01-06-2023', to_date='10-06-2023')
```

### Comparing `nselib-0.5/setup.py` & `nselib-0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='nselib',
     packages=setuptools.find_packages(),
-    version='0.5',
+    version='0.6',
     include_package_data=True,
     description='library to get NSE India data',
     long_description=long_description,
     long_description_content_type="text/markdown", author='RuchiTanmay',
     author_email='ruchitanmay@gmail.com',
     url='https://github.com/RuchiTanmay/nselib',
     install_requires=['requests', 'pandas', 'scipy'],
```

