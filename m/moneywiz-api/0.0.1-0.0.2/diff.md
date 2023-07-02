# Comparing `tmp/moneywiz-api-0.0.1.tar.gz` & `tmp/moneywiz-api-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moneywiz-api-0.0.1.tar", last modified: Sun Jul  2 09:25:40 2023, max compression
+gzip compressed data, was "moneywiz-api-0.0.2.tar", last modified: Sun Jul  2 20:51:18 2023, max compression
```

## Comparing `moneywiz-api-0.0.1.tar` & `moneywiz-api-0.0.2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 leodong    (501) staff       (20)        0 2023-07-02 09:25:40.631310 moneywiz-api-0.0.1/
--rw-r--r--   0 leodong    (501) staff       (20)     1069 2023-07-02 07:48:38.000000 moneywiz-api-0.0.1/LICENSE
--rw-r--r--   0 leodong    (501) staff       (20)     1594 2023-07-02 09:25:40.631168 moneywiz-api-0.0.1/PKG-INFO
--rw-r--r--   0 leodong    (501) staff       (20)     1075 2023-07-02 08:53:58.000000 moneywiz-api-0.0.1/README.md
--rw-r--r--   0 leodong    (501) staff       (20)      596 2023-07-02 08:38:37.000000 moneywiz-api-0.0.1/pyproject.toml
--rw-r--r--   0 leodong    (501) staff       (20)       38 2023-07-02 09:25:40.631347 moneywiz-api-0.0.1/setup.cfg
-drwxr-xr-x   0 leodong    (501) staff       (20)        0 2023-07-02 09:25:40.624503 moneywiz-api-0.0.1/src/
--rw-r--r--   0 leodong    (501) staff       (20)        0 2023-07-02 07:51:08.000000 moneywiz-api-0.0.1/src/__init__.py
-drwxr-xr-x   0 leodong    (501) staff       (20)        0 2023-07-02 09:25:40.626101 moneywiz-api-0.0.1/src/moneywiz_api/
--rw-r--r--   0 leodong    (501) staff       (20)       81 2023-07-02 08:58:32.000000 moneywiz-api-0.0.1/src/moneywiz_api/__init__.py
--rw-r--r--   0 leodong    (501) staff       (20)     3154 2023-07-02 09:21:52.000000 moneywiz-api-0.0.1/src/moneywiz_api/database_accessor.py
-drwxr-xr-x   0 leodong    (501) staff       (20)        0 2023-07-02 09:25:40.628519 moneywiz-api-0.0.1/src/moneywiz_api/managers/
--rw-r--r--   0 leodong    (501) staff       (20)        0 2023-05-17 21:40:01.000000 moneywiz-api-0.0.1/src/moneywiz_api/managers/__init__.py
--rw-r--r--   0 leodong    (501) staff       (20)     1293 2023-07-02 07:53:25.000000 moneywiz-api-0.0.1/src/moneywiz_api/managers/account_manager.py
--rw-r--r--   0 leodong    (501) staff       (20)      971 2023-07-02 07:53:42.000000 moneywiz-api-0.0.1/src/moneywiz_api/managers/category_manager.py
--rw-r--r--   0 leodong    (501) staff       (20)      639 2023-07-02 07:53:58.000000 moneywiz-api-0.0.1/src/moneywiz_api/managers/investment_holding_manager.py
--rw-r--r--   0 leodong    (501) staff       (20)      357 2023-07-02 07:54:13.000000 moneywiz-api-0.0.1/src/moneywiz_api/managers/payee_manager.py
--rw-r--r--   0 leodong    (501) staff       (20)     1178 2023-07-02 07:53:33.000000 moneywiz-api-0.0.1/src/moneywiz_api/managers/record_manager.py
--rw-r--r--   0 leodong    (501) staff       (20)     3164 2023-07-02 07:54:28.000000 moneywiz-api-0.0.1/src/moneywiz_api/managers/transaction_manager.py
-drwxr-xr-x   0 leodong    (501) staff       (20)        0 2023-07-02 09:25:40.630504 moneywiz-api-0.0.1/src/moneywiz_api/model/
--rw-r--r--   0 leodong    (501) staff       (20)        0 2023-07-02 07:51:08.000000 moneywiz-api-0.0.1/src/moneywiz_api/model/__init__.py
--rw-r--r--   0 leodong    (501) staff       (20)     2071 2023-07-02 07:51:15.000000 moneywiz-api-0.0.1/src/moneywiz_api/model/account.py
--rw-r--r--   0 leodong    (501) staff       (20)      944 2023-07-02 07:51:15.000000 moneywiz-api-0.0.1/src/moneywiz_api/model/category.py
--rw-r--r--   0 leodong    (501) staff       (20)     2023 2023-07-02 07:51:15.000000 moneywiz-api-0.0.1/src/moneywiz_api/model/investment_holding.py
--rw-r--r--   0 leodong    (501) staff       (20)      434 2023-07-02 07:51:15.000000 moneywiz-api-0.0.1/src/moneywiz_api/model/payee.py
--rw-r--r--   0 leodong    (501) staff       (20)     1712 2023-07-02 07:51:15.000000 moneywiz-api-0.0.1/src/moneywiz_api/model/record.py
--rw-r--r--   0 leodong    (501) staff       (20)    10970 2023-07-02 08:58:32.000000 moneywiz-api-0.0.1/src/moneywiz_api/model/transaction.py
--rw-r--r--   0 leodong    (501) staff       (20)     1202 2023-07-02 09:14:01.000000 moneywiz-api-0.0.1/src/moneywiz_api/moneywiz_api.py
--rw-r--r--   0 leodong    (501) staff       (20)     2941 2023-07-02 09:16:57.000000 moneywiz-api-0.0.1/src/moneywiz_api/shell.py
--rw-r--r--   0 leodong    (501) staff       (20)       96 2023-05-24 21:32:43.000000 moneywiz-api-0.0.1/src/moneywiz_api/types.py
--rw-r--r--   0 leodong    (501) staff       (20)      342 2023-05-22 20:22:19.000000 moneywiz-api-0.0.1/src/moneywiz_api/utils.py
-drwxr-xr-x   0 leodong    (501) staff       (20)        0 2023-07-02 09:25:40.626961 moneywiz-api-0.0.1/src/moneywiz_api.egg-info/
--rw-r--r--   0 leodong    (501) staff       (20)     1594 2023-07-02 09:25:40.000000 moneywiz-api-0.0.1/src/moneywiz_api.egg-info/PKG-INFO
--rw-r--r--   0 leodong    (501) staff       (20)      980 2023-07-02 09:25:40.000000 moneywiz-api-0.0.1/src/moneywiz_api.egg-info/SOURCES.txt
--rw-r--r--   0 leodong    (501) staff       (20)        1 2023-07-02 09:25:40.000000 moneywiz-api-0.0.1/src/moneywiz_api.egg-info/dependency_links.txt
--rw-r--r--   0 leodong    (501) staff       (20)       22 2023-07-02 09:25:40.000000 moneywiz-api-0.0.1/src/moneywiz_api.egg-info/top_level.txt
-drwxr-xr-x   0 leodong    (501) staff       (20)        0 2023-07-02 09:25:40.630776 moneywiz-api-0.0.1/tests/
--rw-r--r--   0 leodong    (501) staff       (20)      467 2023-07-02 08:58:32.000000 moneywiz-api-0.0.1/tests/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 20:51:18.907366 moneywiz-api-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-02 20:51:09.000000 moneywiz-api-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-07-02 20:51:18.907366 moneywiz-api-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-02 20:51:09.000000 moneywiz-api-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-07-02 20:51:09.000000 moneywiz-api-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 20:51:18.907366 moneywiz-api-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 20:51:18.903366 moneywiz-api-0.0.2/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 20:51:09.000000 moneywiz-api-0.0.2/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 20:51:18.903366 moneywiz-api-0.0.2/src/moneywiz_api/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-02 20:51:09.000000 moneywiz-api-0.0.2/src/moneywiz_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-07-02 20:51:09.000000 moneywiz-api-0.0.2/src/moneywiz_api/database_accessor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 20:51:18.907366 moneywiz-api-0.0.2/src/moneywiz_api/managers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 20:51:09.000000 moneywiz-api-0.0.2/src/moneywiz_api/managers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-07-02 20:51:09.000000 moneywiz-api-0.0.2/src/moneywiz_api/managers/account_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-02 20:51:09.000000 moneywiz-api-0.0.2/src/moneywiz_api/managers/category_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-07-02 20:51:09.000000 moneywiz-api-0.0.2/src/moneywiz_api/managers/investment_holding_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-02 20:51:09.000000 moneywiz-api-0.0.2/src/moneywiz_api/managers/payee_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-07-02 20:51:09.000000 moneywiz-api-0.0.2/src/moneywiz_api/managers/record_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-07-02 20:51:09.000000 moneywiz-api-0.0.2/src/moneywiz_api/managers/transaction_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 20:51:18.907366 moneywiz-api-0.0.2/src/moneywiz_api/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 20:51:09.000000 moneywiz-api-0.0.2/src/moneywiz_api/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-07-02 20:51:09.000000 moneywiz-api-0.0.2/src/moneywiz_api/model/account.py
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-07-02 20:51:09.000000 moneywiz-api-0.0.2/src/moneywiz_api/model/category.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-07-02 20:51:09.000000 moneywiz-api-0.0.2/src/moneywiz_api/model/investment_holding.py
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-07-02 20:51:09.000000 moneywiz-api-0.0.2/src/moneywiz_api/model/payee.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-07-02 20:51:09.000000 moneywiz-api-0.0.2/src/moneywiz_api/model/record.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10962 2023-07-02 20:51:09.000000 moneywiz-api-0.0.2/src/moneywiz_api/model/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-07-02 20:51:09.000000 moneywiz-api-0.0.2/src/moneywiz_api/moneywiz_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-07-02 20:51:09.000000 moneywiz-api-0.0.2/src/moneywiz_api/shell.py
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-02 20:51:09.000000 moneywiz-api-0.0.2/src/moneywiz_api/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-07-02 20:51:09.000000 moneywiz-api-0.0.2/src/moneywiz_api/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 20:51:18.907366 moneywiz-api-0.0.2/src/moneywiz_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-07-02 20:51:18.000000 moneywiz-api-0.0.2/src/moneywiz_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-07-02 20:51:18.000000 moneywiz-api-0.0.2/src/moneywiz_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 20:51:18.000000 moneywiz-api-0.0.2/src/moneywiz_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-02 20:51:18.000000 moneywiz-api-0.0.2/src/moneywiz_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 20:51:18.907366 moneywiz-api-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-07-02 20:51:09.000000 moneywiz-api-0.0.2/tests/test_config.py
```

### Comparing `moneywiz-api-0.0.1/LICENSE` & `moneywiz-api-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `moneywiz-api-0.0.1/PKG-INFO` & `moneywiz-api-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moneywiz-api
-Version: 0.0.1
+Version: 0.0.2
 Summary: A Python api to access moneywiz sqlite database
 Author-email: iLeoDo <iLeoDo@gmail.com>
 Project-URL: Homepage, https://github.com/ileodo/moneywiz-api
 Project-URL: Bug Tracker, https://github.com/ileodo/moneywiz-api/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: moneywiz-api Version: 0.0.1 Summary: A Python api
+Metadata-Version: 2.1 Name: moneywiz-api Version: 0.0.2 Summary: A Python api
 to access moneywiz sqlite database Author-email: iLeoDo
 gmail.com> Project-URL: Homepage, https://github.com/ileodo/moneywiz-api
 Project-URL: Bug Tracker, https://github.com/ileodo/moneywiz-api/issues
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7 Description-Content-Type: text/markdown License-File:
 LICENSE # MoneyWiz-API ![Static Badge](https://img.shields.io/badge/Python-3-
```

### Comparing `moneywiz-api-0.0.1/README.md` & `moneywiz-api-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `moneywiz-api-0.0.1/pyproject.toml` & `moneywiz-api-0.0.2/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "moneywiz-api"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
     { name="iLeoDo", email="iLeoDo@gmail.com" },
 ]
 description = "A Python api to access moneywiz sqlite database"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
@@ -17,7 +17,13 @@
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/ileodo/moneywiz-api"
 "Bug Tracker" = "https://github.com/ileodo/moneywiz-api/issues"
+
+
+[tool.pytest.ini_options]
+pythonpath = [
+    ".", "src",
+]
```

### Comparing `moneywiz-api-0.0.1/src/moneywiz_api/database_accessor.py` & `moneywiz-api-0.0.2/src/moneywiz_api/database_accessor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import sqlite3
 from collections import defaultdict
 from pathlib import Path
 from typing import Dict, List, Any, Callable, Tuple
 
-from src.moneywiz_api.model.record import Record
-from src.moneywiz_api.types import ENT_ID, ID
+from moneywiz_api.model.record import Record
+from moneywiz_api.types import ENT_ID, ID
 
 
 class DatabaseAccessor:
     def __init__(self, db_path: Path):
         self._con = sqlite3.connect(db_path, uri=True)
 
         def dict_factory(cursor, row):
```

### Comparing `moneywiz-api-0.0.1/src/moneywiz_api/managers/account_manager.py` & `moneywiz-api-0.0.2/src/moneywiz_api/managers/account_manager.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from typing import Dict, Callable, List
 
-from src.moneywiz_api.model.account import Account
-from src.moneywiz_api.managers.record_manager import RecordManager
+from moneywiz_api.model.account import Account
+from moneywiz_api.managers.record_manager import RecordManager
 
-from src.moneywiz_api.model.account import (
+from moneywiz_api.model.account import (
     BankChequeAccount,
     BankSavingAccount,
     CashAccount,
     CreditCardAccount,
     LoanAccount,
     InvestmentAccount,
     ForexAccount,
 )
-from src.moneywiz_api.types import ID
+from moneywiz_api.types import ID
 
 
 class AccountManager(RecordManager[Account]):
     def __init__(self):
         super().__init__()
 
     @property
```

### Comparing `moneywiz-api-0.0.1/src/moneywiz_api/managers/category_manager.py` & `moneywiz-api-0.0.2/src/moneywiz_api/managers/category_manager.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Dict, Callable, List
 
-from src.moneywiz_api.model.category import Category
-from src.moneywiz_api.managers.record_manager import RecordManager
-from src.moneywiz_api.types import ID
+from moneywiz_api.model.category import Category
+from moneywiz_api.managers.record_manager import RecordManager
+from moneywiz_api.types import ID
 
 
 class CategoryManager(RecordManager[Category]):
     def __init__(self):
         super().__init__()
 
     @property
```

### Comparing `moneywiz-api-0.0.1/src/moneywiz_api/managers/investment_holding_manager.py` & `moneywiz-api-0.0.2/src/moneywiz_api/managers/investment_holding_manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Dict, Callable, List
 
-from src.moneywiz_api.model.investment_holding import InvestmentHolding
-from src.moneywiz_api.managers.record_manager import RecordManager
-from src.moneywiz_api.types import ID
+from moneywiz_api.model.investment_holding import InvestmentHolding
+from moneywiz_api.managers.record_manager import RecordManager
+from moneywiz_api.types import ID
 
 
 class InvestmentHoldingManager(RecordManager[InvestmentHolding]):
     def __init__(self):
         super().__init__()
 
     @property
```

### Comparing `moneywiz-api-0.0.1/src/moneywiz_api/managers/record_manager.py` & `moneywiz-api-0.0.2/src/moneywiz_api/managers/record_manager.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from abc import ABC, abstractmethod
 from typing import Dict, Generic, TypeVar, Callable
 
-from src.moneywiz_api.database_accessor import DatabaseAccessor
-from src.moneywiz_api.model.record import Record
-from src.moneywiz_api.types import ID
+from moneywiz_api.database_accessor import DatabaseAccessor
+from moneywiz_api.model.record import Record
+from moneywiz_api.types import ID
 
 
 T = TypeVar("T", bound=Record)
 
 
 class RecordManager(ABC, Generic[T]):
     def __init__(self):
```

### Comparing `moneywiz-api-0.0.1/src/moneywiz_api/managers/transaction_manager.py` & `moneywiz-api-0.0.2/src/moneywiz_api/managers/transaction_manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from datetime import datetime
 from typing import Dict, Callable, List, Tuple
 
-from src.moneywiz_api import utils
-from src.moneywiz_api.database_accessor import DatabaseAccessor
-from src.moneywiz_api.model.transaction import (
+from moneywiz_api import utils
+from moneywiz_api.database_accessor import DatabaseAccessor
+from moneywiz_api.model.transaction import (
     Transaction,
     DepositTransaction,
     InvestmentExchangeTransaction,
     InvestmentBuyTransaction,
     InvestmentSellTransaction,
     ReconcileTransaction,
     RefundTransaction,
     TransferBudgetTransaction,
     TransferDepositTransaction,
     TransferWithdrawTransaction,
     WithdrawTransaction,
 )
-from src.moneywiz_api.managers.record_manager import RecordManager
-from src.moneywiz_api.types import ID
+from moneywiz_api.managers.record_manager import RecordManager
+from moneywiz_api.types import ID
 
 
 class TransactionManager(RecordManager[Transaction]):
     def __init__(self):
         super().__init__()
         self.category_assignment: Dict[ID, List[Tuple[ID, float]]] = {}
         self.refund_maps: Dict[ID, ID] = {}
```

### Comparing `moneywiz-api-0.0.1/src/moneywiz_api/model/account.py` & `moneywiz-api-0.0.2/src/moneywiz_api/model/account.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from abc import ABC
 from dataclasses import dataclass, field
 
-from src.moneywiz_api.model.record import Record
-from src.moneywiz_api.types import ID
+from moneywiz_api.model.record import Record
+from moneywiz_api.types import ID
 
 
 @dataclass
 class Account(Record, ABC):
     """
     ENT: 9
     """
```

### Comparing `moneywiz-api-0.0.1/src/moneywiz_api/model/category.py` & `moneywiz-api-0.0.2/src/moneywiz_api/model/category.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from dataclasses import dataclass
 from typing import Optional
 
-from src.moneywiz_api.model.record import Record
-from src.moneywiz_api.types import CategoryType, ID
+from moneywiz_api.model.record import Record
+from moneywiz_api.types import CategoryType, ID
 
 
 @dataclass
 class Category(Record):
     """
     ENT: 19
     """
```

### Comparing `moneywiz-api-0.0.1/src/moneywiz_api/model/investment_holding.py` & `moneywiz-api-0.0.2/src/moneywiz_api/model/investment_holding.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from dataclasses import dataclass, field
 from typing import Dict, Any, Optional
 
-from src.moneywiz_api.model.record import Record
-from src.moneywiz_api.types import ID
+from moneywiz_api.model.record import Record
+from moneywiz_api.types import ID
 
 
 @dataclass
 class InvestmentHolding(Record):
     """
     ENT: 24
     """
```

### Comparing `moneywiz-api-0.0.1/src/moneywiz_api/model/record.py` & `moneywiz-api-0.0.2/src/moneywiz_api/model/record.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from dataclasses import dataclass, asdict, field
 from typing import Dict, Any
 
-from src.moneywiz_api.types import ID, ENT_ID
+from moneywiz_api.types import ID, ENT_ID
 
 
 @dataclass
 class Record:
     _raw: Dict[str, Any] = field(repr=False)
     _ent: ENT_ID = field(repr=False)
     _created_at: float = field(repr=False)
```

### Comparing `moneywiz-api-0.0.1/src/moneywiz_api/model/transaction.py` & `moneywiz-api-0.0.2/src/moneywiz_api/model/transaction.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from abc import ABC
 from dataclasses import dataclass
 from typing import Optional
 
-from src.moneywiz_api.model.record import Record
-from src.moneywiz_api.types import ID
+from moneywiz_api.model.record import Record
+from moneywiz_api.types import ID
 
 import pytest
 
 
 @dataclass
 class Transaction(Record, ABC):
     """
```

### Comparing `moneywiz-api-0.0.1/src/moneywiz_api/moneywiz_api.py` & `moneywiz-api-0.0.2/src/moneywiz_api/moneywiz_api.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from pathlib import Path
 import logging
 
-from src.moneywiz_api.database_accessor import DatabaseAccessor
-from src.moneywiz_api.managers.account_manager import AccountManager
-from src.moneywiz_api.managers.category_manager import CategoryManager
-from src.moneywiz_api.managers.investment_holding_manager import (
+from moneywiz_api.database_accessor import DatabaseAccessor
+from moneywiz_api.managers.account_manager import AccountManager
+from moneywiz_api.managers.category_manager import CategoryManager
+from moneywiz_api.managers.investment_holding_manager import (
     InvestmentHoldingManager,
 )
-from src.moneywiz_api.managers.payee_manager import PayeeManager
-from src.moneywiz_api.managers.transaction_manager import TransactionManager
+from moneywiz_api.managers.payee_manager import PayeeManager
+from moneywiz_api.managers.transaction_manager import TransactionManager
 
 logger = logging.getLogger(__name__)
 
 
 class MoneywizApi:
     def __init__(self, db_file: Path):
         self.accessor = DatabaseAccessor(db_file)
```

### Comparing `moneywiz-api-0.0.1/src/moneywiz_api/shell.py` & `moneywiz-api-0.0.2/src/moneywiz_api/shell.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 from pathlib import Path
 from typing import Dict
 import logging
 import json
 import code
 import pandas as pd
 
-from src.moneywiz_api import MoneywizApi
-from src.moneywiz_api.types import ID
+from moneywiz_api import MoneywizApi
+from moneywiz_api.types import ID
 
 logging.basicConfig(level=logging.DEBUG)
 
 logger = logging.getLogger(__name__)
 
 DB_PATH = sys.argv[1]
```

### Comparing `moneywiz-api-0.0.1/src/moneywiz_api.egg-info/PKG-INFO` & `moneywiz-api-0.0.2/src/moneywiz_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moneywiz-api
-Version: 0.0.1
+Version: 0.0.2
 Summary: A Python api to access moneywiz sqlite database
 Author-email: iLeoDo <iLeoDo@gmail.com>
 Project-URL: Homepage, https://github.com/ileodo/moneywiz-api
 Project-URL: Bug Tracker, https://github.com/ileodo/moneywiz-api/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: moneywiz-api Version: 0.0.1 Summary: A Python api
+Metadata-Version: 2.1 Name: moneywiz-api Version: 0.0.2 Summary: A Python api
 to access moneywiz sqlite database Author-email: iLeoDo
 gmail.com> Project-URL: Homepage, https://github.com/ileodo/moneywiz-api
 Project-URL: Bug Tracker, https://github.com/ileodo/moneywiz-api/issues
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7 Description-Content-Type: text/markdown License-File:
 LICENSE # MoneyWiz-API ![Static Badge](https://img.shields.io/badge/Python-3-
```

### Comparing `moneywiz-api-0.0.1/src/moneywiz_api.egg-info/SOURCES.txt` & `moneywiz-api-0.0.2/src/moneywiz_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

