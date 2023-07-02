# Comparing `tmp/fa-models-1.0.70.tar.gz` & `tmp/fa-models-1.0.72.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fa-models-1.0.70.tar", last modified: Sun Jul  2 10:26:41 2023, max compression
+gzip compressed data, was "fa-models-1.0.72.tar", last modified: Sun Jul  2 13:12:21 2023, max compression
```

## Comparing `fa-models-1.0.70.tar` & `fa-models-1.0.72.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:26:41.936799 fa-models-1.0.70/
--rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-07-02 10:26:41.936799 fa-models-1.0.70/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-07-02 10:26:06.000000 fa-models-1.0.70/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:26:41.932799 fa-models-1.0.70/fa_models.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-07-02 10:26:41.000000 fa-models-1.0.70/fa_models.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-07-02 10:26:41.000000 fa-models-1.0.70/fa_models.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 10:26:41.000000 fa-models-1.0.70/fa_models.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-02 10:26:41.000000 fa-models-1.0.70/fa_models.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-02 10:26:41.000000 fa-models-1.0.70/fa_models.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:26:41.932799 fa-models-1.0.70/famodels/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 10:26:06.000000 fa-models-1.0.70/famodels/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:26:41.932799 fa-models-1.0.70/famodels/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 10:26:06.000000 fa-models-1.0.70/famodels/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-07-02 10:26:06.000000 fa-models-1.0.70/famodels/models/algorithm.py
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-02 10:26:06.000000 fa-models-1.0.70/famodels/models/direction.py
--rw-r--r--   0 runner    (1001) docker     (123)     4179 2023-07-02 10:26:06.000000 fa-models-1.0.70/famodels/models/investor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-07-02 10:26:06.000000 fa-models-1.0.70/famodels/models/order.py
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-02 10:26:06.000000 fa-models-1.0.70/famodels/models/order_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-02 10:26:06.000000 fa-models-1.0.70/famodels/models/person.py
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-07-02 10:26:06.000000 fa-models-1.0.70/famodels/models/processed_signal.py
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-02 10:26:06.000000 fa-models-1.0.70/famodels/models/side.py
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-07-02 10:26:06.000000 fa-models-1.0.70/famodels/models/signal_supplier.py
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-07-02 10:26:06.000000 fa-models-1.0.70/famodels/models/state_of_investor.py
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-02 10:26:06.000000 fa-models-1.0.70/famodels/models/state_of_signal.py
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-02 10:26:06.000000 fa-models-1.0.70/famodels/models/state_of_trade.py
--rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-07-02 10:26:06.000000 fa-models-1.0.70/famodels/models/trade.py
--rw-r--r--   0 runner    (1001) docker     (123)     3239 2023-07-02 10:26:06.000000 fa-models-1.0.70/famodels/models/trading_signal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-07-02 10:26:06.000000 fa-models-1.0.70/famodels/models/virtual_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-07-02 10:26:32.000000 fa-models-1.0.70/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 10:26:41.936799 fa-models-1.0.70/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-07-02 10:26:06.000000 fa-models-1.0.70/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:26:41.932799 fa-models-1.0.70/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6943 2023-07-02 10:26:06.000000 fa-models-1.0.70/tests/test_investor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-07-02 10:26:06.000000 fa-models-1.0.70/tests/test_processed_trading_signal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:12:21.624729 fa-models-1.0.72/
+-rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-07-02 13:12:21.624729 fa-models-1.0.72/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-07-02 13:11:51.000000 fa-models-1.0.72/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:12:21.620729 fa-models-1.0.72/fa_models.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-07-02 13:12:21.000000 fa-models-1.0.72/fa_models.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-07-02 13:12:21.000000 fa-models-1.0.72/fa_models.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 13:12:21.000000 fa-models-1.0.72/fa_models.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-02 13:12:21.000000 fa-models-1.0.72/fa_models.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-02 13:12:21.000000 fa-models-1.0.72/fa_models.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:12:21.620729 fa-models-1.0.72/famodels/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 13:11:51.000000 fa-models-1.0.72/famodels/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:12:21.624729 fa-models-1.0.72/famodels/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 13:11:51.000000 fa-models-1.0.72/famodels/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-07-02 13:11:51.000000 fa-models-1.0.72/famodels/models/algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-02 13:11:51.000000 fa-models-1.0.72/famodels/models/direction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4309 2023-07-02 13:11:51.000000 fa-models-1.0.72/famodels/models/investor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-07-02 13:11:51.000000 fa-models-1.0.72/famodels/models/order.py
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-02 13:11:51.000000 fa-models-1.0.72/famodels/models/order_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-02 13:11:51.000000 fa-models-1.0.72/famodels/models/person.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-07-02 13:11:51.000000 fa-models-1.0.72/famodels/models/processed_signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-02 13:11:51.000000 fa-models-1.0.72/famodels/models/side.py
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-07-02 13:11:51.000000 fa-models-1.0.72/famodels/models/signal_supplier.py
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-07-02 13:11:51.000000 fa-models-1.0.72/famodels/models/state_of_investor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-02 13:11:51.000000 fa-models-1.0.72/famodels/models/state_of_signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-02 13:11:51.000000 fa-models-1.0.72/famodels/models/state_of_trade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-07-02 13:11:51.000000 fa-models-1.0.72/famodels/models/trade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3239 2023-07-02 13:11:51.000000 fa-models-1.0.72/famodels/models/trading_signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-07-02 13:11:51.000000 fa-models-1.0.72/famodels/models/virtual_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-07-02 13:12:13.000000 fa-models-1.0.72/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 13:12:21.624729 fa-models-1.0.72/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-07-02 13:11:51.000000 fa-models-1.0.72/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 13:12:21.624729 fa-models-1.0.72/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6943 2023-07-02 13:11:51.000000 fa-models-1.0.72/tests/test_investor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-07-02 13:11:51.000000 fa-models-1.0.72/tests/test_processed_trading_signal.py
```

### Comparing `fa-models-1.0.70/PKG-INFO` & `fa-models-1.0.72/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fa-models
-Version: 1.0.70
+Version: 1.0.72
 Summary: A simple library of trading models.
 Author-email: Brayan Svan <brayan@freyaalpha.com>
 Project-URL: Homepage, https://github.com/svabra/fa-models
 Keywords: finance,trading,models
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Requires-Python: >=3.9
```

### Comparing `fa-models-1.0.70/README.md` & `fa-models-1.0.72/README.md`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.70/fa_models.egg-info/PKG-INFO` & `fa-models-1.0.72/fa_models.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fa-models
-Version: 1.0.70
+Version: 1.0.72
 Summary: A simple library of trading models.
 Author-email: Brayan Svan <brayan@freyaalpha.com>
 Project-URL: Homepage, https://github.com/svabra/fa-models
 Keywords: finance,trading,models
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Requires-Python: >=3.9
```

### Comparing `fa-models-1.0.70/fa_models.egg-info/SOURCES.txt` & `fa-models-1.0.72/fa_models.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.70/famodels/models/algorithm.py` & `fa-models-1.0.72/famodels/models/algorithm.py`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.70/famodels/models/investor.py` & `fa-models-1.0.72/famodels/models/investor.py`

 * *Files 3% similar despite different names*

```diff
@@ -75,14 +75,16 @@
     email: EmailStr = Field(index=True)
     accountable: Person = Field(index=True)        
     state: StateOfInvestor = Field(index=True, default=StateOfInvestor.REGISTERED.value)
     _passphrase: Optional[str]
     #library constraint: "redis_om.model.model.RedisModelError: In this Preview release, list and tuple fields can only contain strings. Problem field: compounding"
     funds: Optional[List[Fund]]
     exchange_keys: Optional[List[ExchangeKey]]
+    priviledge_rank: int = Field(index=True, default=1, sortable=True)
+    """The higher the value, the higher the priviledge."""
 
     @property
     def passphrase(self):
         raise Exception("Cannot retrieve passphrase.")
     
     def setPassphrase(self, passphrase:str):
         """Use this method to set a password. The pydantic setter method does not work with JsonModel."""
```

### Comparing `fa-models-1.0.70/famodels/models/order.py` & `fa-models-1.0.72/famodels/models/order.py`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.70/famodels/models/person.py` & `fa-models-1.0.72/famodels/models/person.py`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.70/famodels/models/processed_signal.py` & `fa-models-1.0.72/famodels/models/processed_signal.py`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.70/famodels/models/signal_supplier.py` & `fa-models-1.0.72/famodels/models/signal_supplier.py`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.70/famodels/models/state_of_investor.py` & `fa-models-1.0.72/famodels/models/state_of_investor.py`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.70/famodels/models/state_of_trade.py` & `fa-models-1.0.72/famodels/models/state_of_trade.py`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.70/famodels/models/trade.py` & `fa-models-1.0.72/famodels/models/trade.py`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.70/famodels/models/trading_signal.py` & `fa-models-1.0.72/famodels/models/trading_signal.py`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.70/famodels/models/virtual_order.py` & `fa-models-1.0.72/famodels/models/virtual_order.py`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.70/pyproject.toml` & `fa-models-1.0.72/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=66.1.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fa-models"
-version = "1.0.70"
+version = "1.0.72"
 description = "A simple library of trading models."
 readme = "README.md"
 authors = [{ name = "Brayan Svan", email = "brayan@freyaalpha.com" }]
 #license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python"
@@ -25,15 +25,15 @@
 [project.optional-dependencies]
 dev = ["black", "bumpver", "isort", "pip-tools", "pytest"]
 
 [project.urls]
 Homepage = "https://github.com/svabra/fa-models"
 
 [tool.bumpver]
-current_version = "1.0.70"
+current_version = "1.0.72"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `fa-models-1.0.70/setup.py` & `fa-models-1.0.72/setup.py`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.70/tests/test_investor.py` & `fa-models-1.0.72/tests/test_investor.py`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.70/tests/test_processed_trading_signal.py` & `fa-models-1.0.72/tests/test_processed_trading_signal.py`

 * *Files identical despite different names*

