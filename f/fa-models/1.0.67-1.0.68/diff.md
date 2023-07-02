# Comparing `tmp/fa-models-1.0.67.tar.gz` & `tmp/fa-models-1.0.68.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fa-models-1.0.67.tar", last modified: Sun Jul  2 08:28:06 2023, max compression
+gzip compressed data, was "fa-models-1.0.68.tar", last modified: Sun Jul  2 09:18:56 2023, max compression
```

## Comparing `fa-models-1.0.67.tar` & `fa-models-1.0.68.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 08:28:06.240859 fa-models-1.0.67/
--rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-07-02 08:28:06.240859 fa-models-1.0.67/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-07-02 08:27:37.000000 fa-models-1.0.67/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 08:28:06.240859 fa-models-1.0.67/fa_models.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-07-02 08:28:06.000000 fa-models-1.0.67/fa_models.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-07-02 08:28:06.000000 fa-models-1.0.67/fa_models.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 08:28:06.000000 fa-models-1.0.67/fa_models.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-02 08:28:06.000000 fa-models-1.0.67/fa_models.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-02 08:28:06.000000 fa-models-1.0.67/fa_models.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 08:28:06.240859 fa-models-1.0.67/famodels/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 08:27:37.000000 fa-models-1.0.67/famodels/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 08:28:06.240859 fa-models-1.0.67/famodels/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 08:27:37.000000 fa-models-1.0.67/famodels/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-07-02 08:27:37.000000 fa-models-1.0.67/famodels/models/algorithm.py
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-02 08:27:37.000000 fa-models-1.0.67/famodels/models/direction.py
--rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-07-02 08:27:37.000000 fa-models-1.0.67/famodels/models/investor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-07-02 08:27:37.000000 fa-models-1.0.67/famodels/models/order.py
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-02 08:27:37.000000 fa-models-1.0.67/famodels/models/order_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-07-02 08:27:37.000000 fa-models-1.0.67/famodels/models/person.py
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-07-02 08:27:37.000000 fa-models-1.0.67/famodels/models/processed_signal.py
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-02 08:27:37.000000 fa-models-1.0.67/famodels/models/side.py
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-07-02 08:27:37.000000 fa-models-1.0.67/famodels/models/signal_supplier.py
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-02 08:27:37.000000 fa-models-1.0.67/famodels/models/state_of_signal.py
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-02 08:27:37.000000 fa-models-1.0.67/famodels/models/state_of_trade.py
--rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-07-02 08:27:37.000000 fa-models-1.0.67/famodels/models/trade.py
--rw-r--r--   0 runner    (1001) docker     (123)     3239 2023-07-02 08:27:37.000000 fa-models-1.0.67/famodels/models/trading_signal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-07-02 08:27:37.000000 fa-models-1.0.67/famodels/models/virtual_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-07-02 08:27:58.000000 fa-models-1.0.67/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 08:28:06.240859 fa-models-1.0.67/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-07-02 08:27:37.000000 fa-models-1.0.67/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 08:28:06.240859 fa-models-1.0.67/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6937 2023-07-02 08:27:37.000000 fa-models-1.0.67/tests/test_investor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-07-02 08:27:37.000000 fa-models-1.0.67/tests/test_processed_trading_signal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:18:56.971443 fa-models-1.0.68/
+-rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-07-02 09:18:56.971443 fa-models-1.0.68/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-07-02 09:18:24.000000 fa-models-1.0.68/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:18:56.971443 fa-models-1.0.68/fa_models.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-07-02 09:18:56.000000 fa-models-1.0.68/fa_models.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-07-02 09:18:56.000000 fa-models-1.0.68/fa_models.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 09:18:56.000000 fa-models-1.0.68/fa_models.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-02 09:18:56.000000 fa-models-1.0.68/fa_models.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-02 09:18:56.000000 fa-models-1.0.68/fa_models.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:18:56.971443 fa-models-1.0.68/famodels/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 09:18:24.000000 fa-models-1.0.68/famodels/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:18:56.971443 fa-models-1.0.68/famodels/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 09:18:24.000000 fa-models-1.0.68/famodels/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-07-02 09:18:24.000000 fa-models-1.0.68/famodels/models/algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-02 09:18:24.000000 fa-models-1.0.68/famodels/models/direction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4104 2023-07-02 09:18:24.000000 fa-models-1.0.68/famodels/models/investor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-07-02 09:18:24.000000 fa-models-1.0.68/famodels/models/order.py
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-02 09:18:24.000000 fa-models-1.0.68/famodels/models/order_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-02 09:18:24.000000 fa-models-1.0.68/famodels/models/person.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-07-02 09:18:24.000000 fa-models-1.0.68/famodels/models/processed_signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-02 09:18:24.000000 fa-models-1.0.68/famodels/models/side.py
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-07-02 09:18:24.000000 fa-models-1.0.68/famodels/models/signal_supplier.py
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-02 09:18:24.000000 fa-models-1.0.68/famodels/models/state_of_signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-02 09:18:24.000000 fa-models-1.0.68/famodels/models/state_of_trade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-07-02 09:18:24.000000 fa-models-1.0.68/famodels/models/trade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3239 2023-07-02 09:18:24.000000 fa-models-1.0.68/famodels/models/trading_signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-07-02 09:18:24.000000 fa-models-1.0.68/famodels/models/virtual_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-07-02 09:18:48.000000 fa-models-1.0.68/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 09:18:56.971443 fa-models-1.0.68/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-07-02 09:18:24.000000 fa-models-1.0.68/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:18:56.971443 fa-models-1.0.68/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6943 2023-07-02 09:18:24.000000 fa-models-1.0.68/tests/test_investor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-07-02 09:18:24.000000 fa-models-1.0.68/tests/test_processed_trading_signal.py
```

### Comparing `fa-models-1.0.67/PKG-INFO` & `fa-models-1.0.68/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fa-models
-Version: 1.0.67
+Version: 1.0.68
 Summary: A simple library of trading models.
 Author-email: Brayan Svan <brayan@freyaalpha.com>
 Project-URL: Homepage, https://github.com/svabra/fa-models
 Keywords: finance,trading,models
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Requires-Python: >=3.9
```

### Comparing `fa-models-1.0.67/README.md` & `fa-models-1.0.68/README.md`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.67/fa_models.egg-info/PKG-INFO` & `fa-models-1.0.68/fa_models.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fa-models
-Version: 1.0.67
+Version: 1.0.68
 Summary: A simple library of trading models.
 Author-email: Brayan Svan <brayan@freyaalpha.com>
 Project-URL: Homepage, https://github.com/svabra/fa-models
 Keywords: finance,trading,models
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Requires-Python: >=3.9
```

### Comparing `fa-models-1.0.67/fa_models.egg-info/SOURCES.txt` & `fa-models-1.0.68/fa_models.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.67/famodels/models/algorithm.py` & `fa-models-1.0.68/famodels/models/algorithm.py`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.67/famodels/models/investor.py` & `fa-models-1.0.68/famodels/models/investor.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,18 +25,18 @@
     class Meta:
         # global_key_prefix="fa-investor-processing"
         model_key_prefix="subscription"
         database = get_redis_connection(url=REDIS_OM_URL, decode_responses=True)
 
 class Fund(EmbeddedJsonModel):
     fund_id:str = Field(index=True)
-    name:str = Field(index=True)
-    investor_id:str = Field(index=True)    
-    subscriptions: Optional[List[Subscription]] = Field(index=False)  
-    compounding: int = Field(index=True, default=1)
+    name:str = Field(index=True)    
+    compounding: str = Field(index=True, default="true")
+    """Marks the investment as to be compounded with every trade. CAUTION: Due to redis-om model restrictions this could not be a boolean as it's value suggests. The workaround is a str with values 'true' and 'false'. Default is 'true'. Will bechanged as soon the redis-om library has enhanced."""
+    subscriptions: Optional[List[Subscription]]  
     absolute_max_amount: Optional[float]
     
     class Meta:
         # global_key_prefix="fa-investor-processing"
         model_key_prefix="fund"
         database = get_redis_connection(url=REDIS_OM_URL, decode_responses=True)
 
@@ -53,15 +53,14 @@
         f = Fernet(self.key)
         return f.encrypt(value.encode()).decode()
 
     def decrypt(self, encrypted_value: str) -> str:
         f = Fernet(self.key)
         return f.decrypt(encrypted_value.encode()).decode()
 
-
 class ExchangeKey(EmbeddedJsonModel):
     exchange: str = Field(index=True)
     key_id: str = Field(index=True)
     _key_secret: str = Field(index=False)
 
     def set_key_secret(self, value: str, encryption_service: EncryptionService):
         self._key_secret = encryption_service.encrypt(value)
@@ -70,22 +69,21 @@
         return encryption_service.decrypt(self._key_secret)
 
     class Meta:
         model_key_prefix = "exchange-key"
         database = get_redis_connection(url=REDIS_OM_URL, decode_responses=True)
 
 
-
 class Investor(JsonModel):
     investor_id: str = Field(index=True)
     email: EmailStr = Field(index=True)
     accountable: Person = Field(index=True)        
     _passphrase: Optional[str]
     #library constraint: "redis_om.model.model.RedisModelError: In this Preview release, list and tuple fields can only contain strings. Problem field: compounding"
-    # funds: Optional[List[Fund]]
+    funds: Optional[List[Fund]]
     exchange_keys: Optional[List[ExchangeKey]]
 
     @property
     def passphrase(self):
         raise Exception("Cannot retrieve passphrase.")
     
     def setPassphrase(self, passphrase:str):
```

### Comparing `fa-models-1.0.67/famodels/models/order.py` & `fa-models-1.0.68/famodels/models/order.py`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.67/famodels/models/person.py` & `fa-models-1.0.68/famodels/models/person.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 print(f"The env-var REDIS_OM_URL is: {REDIS_OM_URL}")
 
 class Person(EmbeddedJsonModel):    
     given_name: str = Field(index=True)
     family_name: str = Field(index=True, full_text_search=True)
     email: EmailStr = Field(index=True)
     sex: int = Field(index=True)    
+    """0=male, 1=female"""
     nationality_iso3: str = Field(index=True, max_length=3, min_length=3)
     identification_type: Optional[str]
     identification_reference: Optional[str]
     country_of_residence_iso3: str = Field(index=True, max_length=3, min_length=3)
     phone: str = Field(index=True)
     
     class Meta:
```

### Comparing `fa-models-1.0.67/famodels/models/processed_signal.py` & `fa-models-1.0.68/famodels/models/processed_signal.py`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.67/famodels/models/signal_supplier.py` & `fa-models-1.0.68/famodels/models/signal_supplier.py`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.67/famodels/models/state_of_trade.py` & `fa-models-1.0.68/famodels/models/state_of_trade.py`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.67/famodels/models/trade.py` & `fa-models-1.0.68/famodels/models/trade.py`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.67/famodels/models/trading_signal.py` & `fa-models-1.0.68/famodels/models/trading_signal.py`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.67/famodels/models/virtual_order.py` & `fa-models-1.0.68/famodels/models/virtual_order.py`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.67/pyproject.toml` & `fa-models-1.0.68/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=66.1.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fa-models"
-version = "1.0.67"
+version = "1.0.68"
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
-current_version = "1.0.67"
+current_version = "1.0.68"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `fa-models-1.0.67/setup.py` & `fa-models-1.0.68/setup.py`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.67/tests/test_investor.py` & `fa-models-1.0.68/tests/test_investor.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,15 +99,15 @@
     assert exchange_key.exchange == exchange
     assert exchange_key.key_id == key_id
     assert exchange_key.get_key_secret(encryption_service) == key_secret
 
 @pytest.mark.parametrize(
     "investor_id, email, funds",
     [
-        ("1", "investor1@example.com", [{"fund_id": "f1", "name": "fund1", "investor_id": "1", "subscriptions": [{"subscription_id": "s1", "algo_id": "a1"}], "compounding": 1, "absolute_max_amount": 1000.0}, {"fund_id": "f2", "name": "fund2", "investor_id": "1", "subscriptions": [{"subscription_id": "s2", "algo_id": "a2"}, {"subscription_id": "s3", "algo_id": "a3"}], "compounding": 0, "absolute_max_amount": 500.0}]),
+        ("1", "investor1@example.com", [{"fund_id": "f1", "name": "fund1", "investor_id": "1", "subscriptions": [{"subscription_id": "s1", "algo_id": "a1"}], "compounding": 1, "absolute_max_amount": 1000.0}, {"fund_id": "f2", "name": "fund2", "investor_id": "1", "subscriptions": [{"subscription_id": "s2", "algo_id": "a2"}, {"subscription_id": "s3", "algo_id": "a3"}], "compounding": "false", "absolute_max_amount": 500.0}]),
         ("2", "investor2@example.com", [{"fund_id": "f3", "name": "fund3", "investor_id": "2", "subscriptions": [{"subscription_id": "s4", "algo_id": "a4"}, {"subscription_id": "s5", "algo_id": "a5"}, {"subscription_id": "s6", "algo_id": "a6"}], "compounding": 1}]),
         ("3", "investor3@example.com", [{"fund_id": "f4", "name": "fund4", "investor_id": "3", "subscriptions": [{"subscription_id": "s7", "algo_id": "a7"}], "compounding": 0, "absolute_max_amount": 10000.0}, {"fund_id": "f5", "name": "fund5", "investor_id": "3", "subscriptions": [{"subscription_id": "s8", "algo_id": "a8"}, {"subscription_id": "s9", "algo_id": "a9"}, {"subscription_id": "s10", "algo_id": "a10"}]}])
     ]
 )
 def test_investor_funds(investor_id, email, funds):
     person = Person(given_name="john", family_name="Doe", email=email, sex=0, nationality_iso3="GBR", country_of_residence_iso3="IRE", phone="+43 681 11 24")
```

### Comparing `fa-models-1.0.67/tests/test_processed_trading_signal.py` & `fa-models-1.0.68/tests/test_processed_trading_signal.py`

 * *Files identical despite different names*

