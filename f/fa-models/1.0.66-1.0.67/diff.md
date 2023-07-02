# Comparing `tmp/fa-models-1.0.66.tar.gz` & `tmp/fa-models-1.0.67.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fa-models-1.0.66.tar", last modified: Sat Jul  1 17:58:37 2023, max compression
+gzip compressed data, was "fa-models-1.0.67.tar", last modified: Sun Jul  2 08:28:06 2023, max compression
```

## Comparing `fa-models-1.0.66.tar` & `fa-models-1.0.67.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 17:58:37.148902 fa-models-1.0.66/
--rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-07-01 17:58:37.148902 fa-models-1.0.66/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-07-01 17:58:02.000000 fa-models-1.0.66/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 17:58:37.144901 fa-models-1.0.66/fa_models.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-07-01 17:58:37.000000 fa-models-1.0.66/fa_models.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-07-01 17:58:37.000000 fa-models-1.0.66/fa_models.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 17:58:37.000000 fa-models-1.0.66/fa_models.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-01 17:58:37.000000 fa-models-1.0.66/fa_models.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-01 17:58:37.000000 fa-models-1.0.66/fa_models.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 17:58:37.144901 fa-models-1.0.66/famodels/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 17:58:02.000000 fa-models-1.0.66/famodels/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 17:58:37.148902 fa-models-1.0.66/famodels/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 17:58:02.000000 fa-models-1.0.66/famodels/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-07-01 17:58:02.000000 fa-models-1.0.66/famodels/models/algorithm.py
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-01 17:58:02.000000 fa-models-1.0.66/famodels/models/direction.py
--rw-r--r--   0 runner    (1001) docker     (123)     3575 2023-07-01 17:58:02.000000 fa-models-1.0.66/famodels/models/investor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-07-01 17:58:02.000000 fa-models-1.0.66/famodels/models/order.py
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-01 17:58:02.000000 fa-models-1.0.66/famodels/models/order_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-07-01 17:58:02.000000 fa-models-1.0.66/famodels/models/person.py
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-07-01 17:58:02.000000 fa-models-1.0.66/famodels/models/processed_signal.py
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-01 17:58:02.000000 fa-models-1.0.66/famodels/models/side.py
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-07-01 17:58:02.000000 fa-models-1.0.66/famodels/models/signal_supplier.py
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-01 17:58:02.000000 fa-models-1.0.66/famodels/models/state_of_signal.py
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-01 17:58:02.000000 fa-models-1.0.66/famodels/models/state_of_trade.py
--rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-07-01 17:58:02.000000 fa-models-1.0.66/famodels/models/trade.py
--rw-r--r--   0 runner    (1001) docker     (123)     3239 2023-07-01 17:58:02.000000 fa-models-1.0.66/famodels/models/trading_signal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-07-01 17:58:02.000000 fa-models-1.0.66/famodels/models/virtual_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-07-01 17:58:27.000000 fa-models-1.0.66/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 17:58:37.148902 fa-models-1.0.66/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-07-01 17:58:02.000000 fa-models-1.0.66/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 17:58:37.148902 fa-models-1.0.66/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6176 2023-07-01 17:58:02.000000 fa-models-1.0.66/tests/test_investor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-07-01 17:58:02.000000 fa-models-1.0.66/tests/test_processed_trading_signal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 08:28:06.240859 fa-models-1.0.67/
+-rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-07-02 08:28:06.240859 fa-models-1.0.67/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-07-02 08:27:37.000000 fa-models-1.0.67/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 08:28:06.240859 fa-models-1.0.67/fa_models.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-07-02 08:28:06.000000 fa-models-1.0.67/fa_models.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-07-02 08:28:06.000000 fa-models-1.0.67/fa_models.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 08:28:06.000000 fa-models-1.0.67/fa_models.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-02 08:28:06.000000 fa-models-1.0.67/fa_models.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-02 08:28:06.000000 fa-models-1.0.67/fa_models.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 08:28:06.240859 fa-models-1.0.67/famodels/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 08:27:37.000000 fa-models-1.0.67/famodels/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 08:28:06.240859 fa-models-1.0.67/famodels/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 08:27:37.000000 fa-models-1.0.67/famodels/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-07-02 08:27:37.000000 fa-models-1.0.67/famodels/models/algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-02 08:27:37.000000 fa-models-1.0.67/famodels/models/direction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-07-02 08:27:37.000000 fa-models-1.0.67/famodels/models/investor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-07-02 08:27:37.000000 fa-models-1.0.67/famodels/models/order.py
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-02 08:27:37.000000 fa-models-1.0.67/famodels/models/order_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-07-02 08:27:37.000000 fa-models-1.0.67/famodels/models/person.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-07-02 08:27:37.000000 fa-models-1.0.67/famodels/models/processed_signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-02 08:27:37.000000 fa-models-1.0.67/famodels/models/side.py
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-07-02 08:27:37.000000 fa-models-1.0.67/famodels/models/signal_supplier.py
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-02 08:27:37.000000 fa-models-1.0.67/famodels/models/state_of_signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-02 08:27:37.000000 fa-models-1.0.67/famodels/models/state_of_trade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-07-02 08:27:37.000000 fa-models-1.0.67/famodels/models/trade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3239 2023-07-02 08:27:37.000000 fa-models-1.0.67/famodels/models/trading_signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-07-02 08:27:37.000000 fa-models-1.0.67/famodels/models/virtual_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-07-02 08:27:58.000000 fa-models-1.0.67/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 08:28:06.240859 fa-models-1.0.67/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-07-02 08:27:37.000000 fa-models-1.0.67/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 08:28:06.240859 fa-models-1.0.67/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6937 2023-07-02 08:27:37.000000 fa-models-1.0.67/tests/test_investor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-07-02 08:27:37.000000 fa-models-1.0.67/tests/test_processed_trading_signal.py
```

### Comparing `fa-models-1.0.66/PKG-INFO` & `fa-models-1.0.67/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fa-models
-Version: 1.0.66
+Version: 1.0.67
 Summary: A simple library of trading models.
 Author-email: Brayan Svan <brayan@freyaalpha.com>
 Project-URL: Homepage, https://github.com/svabra/fa-models
 Keywords: finance,trading,models
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Requires-Python: >=3.9
```

### Comparing `fa-models-1.0.66/README.md` & `fa-models-1.0.67/README.md`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.66/fa_models.egg-info/PKG-INFO` & `fa-models-1.0.67/fa_models.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fa-models
-Version: 1.0.66
+Version: 1.0.67
 Summary: A simple library of trading models.
 Author-email: Brayan Svan <brayan@freyaalpha.com>
 Project-URL: Homepage, https://github.com/svabra/fa-models
 Keywords: finance,trading,models
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Requires-Python: >=3.9
```

### Comparing `fa-models-1.0.66/fa_models.egg-info/SOURCES.txt` & `fa-models-1.0.67/fa_models.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.66/famodels/models/algorithm.py` & `fa-models-1.0.67/famodels/models/algorithm.py`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.66/famodels/models/investor.py` & `fa-models-1.0.67/famodels/models/investor.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,26 +4,28 @@
 from pydantic import EmailStr
 from redis_om import Field, JsonModel, EmbeddedJsonModel
 from redis_om.connections import get_redis_connection
 from famodels.models.person import Person
 import hashlib
 from cryptography.fernet import Fernet
 from hashlib import sha256
+import bcrypt
 from base64 import urlsafe_b64encode, urlsafe_b64decode
 
 REDIS_OM_URL = os.environ.get("REDIS_OM_URL")
 print(f"The env-var REDIS_OM_URL is: {REDIS_OM_URL}")
 
 key = os.environ.get("ENCRYPTION_KEY").encode()
 ENCRYPTION_KEY = urlsafe_b64encode(sha256(key).digest())
 
+SALT = os.environ.get("SALT")
+
 class Subscription(EmbeddedJsonModel):
     subscription_id: str = Field(index=False)
     algo_id:str = Field(index=True)
-    
     class Meta:
         # global_key_prefix="fa-investor-processing"
         model_key_prefix="subscription"
         database = get_redis_connection(url=REDIS_OM_URL, decode_responses=True)
 
 class Fund(EmbeddedJsonModel):
     fund_id:str = Field(index=True)
@@ -73,28 +75,31 @@
 
 
 
 class Investor(JsonModel):
     investor_id: str = Field(index=True)
     email: EmailStr = Field(index=True)
     accountable: Person = Field(index=True)        
-    _passphrase: str = Field(index=False)
+    _passphrase: Optional[str]
     #library constraint: "redis_om.model.model.RedisModelError: In this Preview release, list and tuple fields can only contain strings. Problem field: compounding"
     # funds: Optional[List[Fund]]
     exchange_keys: Optional[List[ExchangeKey]]
 
-    # @property
-    # def passphrase(self):
-    #     raise Exception("Cannot retrieve passphrase.")
-        
-    # @passphrase.setter
-    # def passphrase(self, value):
-    #     hashed_value = hashlib.sha256(value.encode()).hexdigest()
-    #     self._passphrase = hashed_value
-
-    # def verify_passphrase(self, value):
-    #     return self._passphrase == hashlib.sha256(value.encode()).hexdigest()
+    @property
+    def passphrase(self):
+        raise Exception("Cannot retrieve passphrase.")
+    
+    def setPassphrase(self, passphrase:str):
+        """Use this method to set a password. The pydantic setter method does not work with JsonModel."""
+        encoded_pw = passphrase.encode()
+        # Adding the salt to prefent Rainbow Table Attacks and avoiding to hash the same password with the same hash.
+        # DO NOT USE A STATIC SALT!
+        salt = bcrypt.gensalt()
+        self._passphrase = bcrypt.hashpw(encoded_pw, salt)
 
+    def verify_passphrase(self, passphrase: str):
+        return bcrypt.checkpw(passphrase.encode(), self._passphrase)    
+    
     class Meta:
         # global_key_prefix="fa-investor-processing"
         model_key_prefix="investor"
         database = get_redis_connection(url=REDIS_OM_URL, decode_responses=True)
```

### Comparing `fa-models-1.0.66/famodels/models/order.py` & `fa-models-1.0.67/famodels/models/order.py`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.66/famodels/models/person.py` & `fa-models-1.0.67/famodels/models/person.py`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.66/famodels/models/processed_signal.py` & `fa-models-1.0.67/famodels/models/processed_signal.py`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.66/famodels/models/signal_supplier.py` & `fa-models-1.0.67/famodels/models/signal_supplier.py`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.66/famodels/models/state_of_trade.py` & `fa-models-1.0.67/famodels/models/state_of_trade.py`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.66/famodels/models/trade.py` & `fa-models-1.0.67/famodels/models/trade.py`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.66/famodels/models/trading_signal.py` & `fa-models-1.0.67/famodels/models/trading_signal.py`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.66/famodels/models/virtual_order.py` & `fa-models-1.0.67/famodels/models/virtual_order.py`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.66/pyproject.toml` & `fa-models-1.0.67/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=66.1.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fa-models"
-version = "1.0.66"
+version = "1.0.67"
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
-current_version = "1.0.66"
+current_version = "1.0.67"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `fa-models-1.0.66/setup.py` & `fa-models-1.0.67/setup.py`

 * *Files identical despite different names*

### Comparing `fa-models-1.0.66/tests/test_investor.py` & `fa-models-1.0.67/tests/test_investor.py`

 * *Files 13% similar despite different names*

```diff
@@ -123,7 +123,24 @@
     assert investor.email == email
     assert len(investor.funds) == len(funds_objects)
     for i in range(len(funds_objects)):
         assert investor.funds[i].fund_id == funds_objects[i].fund_id
         assert investor.funds[i].name == funds_objects[i].name
         assert investor.funds[i].compounding == funds_objects[i].compounding
         assert len(investor.funds[i].subscriptions) == len(funds_objects[i].subscriptions)
+
+
+def test_passphrase():
+    # Create an Investor instance
+    person = Person(given_name="john", family_name="Doe", email="john@doe.com", sex=0, nationality_iso3="GBR", country_of_residence_iso3="IRE", phone="+43 681 11 24")
+    investor = Investor(investor_id='123', email='test@example.com', accountable=person)
+    investor.setPassphrase("testpass")
+    # Check that passphrase can't be retrieved directly
+    with pytest.raises(Exception) as e:
+        print(f"INVOKING IS FORBIDDEN --> {investor.passphrase}")
+    assert str(e.value) == "Cannot retrieve passphrase."
+
+    # Check the passphrase
+    assert investor.verify_passphrase("testpass") is True
+
+    # Check with an incorrect passphrase
+    assert investor.verify_passphrase("wrongpass") is False
```

### Comparing `fa-models-1.0.66/tests/test_processed_trading_signal.py` & `fa-models-1.0.67/tests/test_processed_trading_signal.py`

 * *Files identical despite different names*

