# Comparing `tmp/investlib-0.0.2.tar.gz` & `tmp/investlib-0.0.3.tar.gz`

## Comparing `investlib-0.0.2.tar` & `investlib-0.0.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 investlib-0.0.2/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 investlib-0.0.2/investlib/__init__.py
--rw-r--r--   0        0        0     3779 2020-02-02 00:00:00.000000 investlib-0.0.2/investlib/backtest.py
--rw-r--r--   0        0        0     5190 2020-02-02 00:00:00.000000 investlib-0.0.2/investlib/core.py
--rw-r--r--   0        0        0     4205 2020-02-02 00:00:00.000000 investlib-0.0.2/investlib/data.py
--rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 investlib-0.0.2/investlib/download.py
--rw-r--r--   0        0        0     5528 2020-02-02 00:00:00.000000 investlib-0.0.2/investlib/draw.py
--rw-r--r--   0        0        0     2757 2020-02-02 00:00:00.000000 investlib-0.0.2/investlib/filters.py
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 investlib-0.0.2/investlib/portfolio.py
--rw-r--r--   0        0        0     1472 2020-02-02 00:00:00.000000 investlib-0.0.2/investlib/rebalance.py
--rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 investlib-0.0.2/investlib/spydiffeqw.py
--rw-r--r--   0        0        0     2332 2020-02-02 00:00:00.000000 investlib-0.0.2/investlib/spystdreb.py
--rw-r--r--   0        0        0     5455 2020-02-02 00:00:00.000000 investlib-0.0.2/investlib/strategy.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 investlib-0.0.2/tests/__init__.py
--rw-r--r--   0        0        0    13283 2020-02-02 00:00:00.000000 investlib-0.0.2/tests/test_data.py
--rw-r--r--   0        0        0     4329 2020-02-02 00:00:00.000000 investlib-0.0.2/tests/test_filters.py
--rw-r--r--   0        0        0     2060 2020-02-02 00:00:00.000000 investlib-0.0.2/tests/test_rebalance.py
--rw-r--r--   0        0        0    14936 2020-02-02 00:00:00.000000 investlib-0.0.2/tests/test_strategy.py
--rw-r--r--   0        0        0     3125 2020-02-02 00:00:00.000000 investlib-0.0.2/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 investlib-0.0.2/LICENSE
--rw-r--r--   0        0        0     2865 2020-02-02 00:00:00.000000 investlib-0.0.2/README.md
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 investlib-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     3433 2020-02-02 00:00:00.000000 investlib-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 investlib-0.0.3/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 investlib-0.0.3/investlib/__init__.py
+-rw-r--r--   0        0        0     3779 2020-02-02 00:00:00.000000 investlib-0.0.3/investlib/backtest.py
+-rw-r--r--   0        0        0     5190 2020-02-02 00:00:00.000000 investlib-0.0.3/investlib/core.py
+-rw-r--r--   0        0        0     4205 2020-02-02 00:00:00.000000 investlib-0.0.3/investlib/data.py
+-rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 investlib-0.0.3/investlib/download.py
+-rw-r--r--   0        0        0     5528 2020-02-02 00:00:00.000000 investlib-0.0.3/investlib/draw.py
+-rw-r--r--   0        0        0     2757 2020-02-02 00:00:00.000000 investlib-0.0.3/investlib/filters.py
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 investlib-0.0.3/investlib/portfolio.py
+-rw-r--r--   0        0        0     1472 2020-02-02 00:00:00.000000 investlib-0.0.3/investlib/rebalance.py
+-rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 investlib-0.0.3/investlib/spydiffeqw.py
+-rw-r--r--   0        0        0     2332 2020-02-02 00:00:00.000000 investlib-0.0.3/investlib/spystdreb.py
+-rw-r--r--   0        0        0     5455 2020-02-02 00:00:00.000000 investlib-0.0.3/investlib/strategy.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 investlib-0.0.3/tests/__init__.py
+-rw-r--r--   0        0        0    13283 2020-02-02 00:00:00.000000 investlib-0.0.3/tests/test_data.py
+-rw-r--r--   0        0        0     4329 2020-02-02 00:00:00.000000 investlib-0.0.3/tests/test_filters.py
+-rw-r--r--   0        0        0     2060 2020-02-02 00:00:00.000000 investlib-0.0.3/tests/test_rebalance.py
+-rw-r--r--   0        0        0    14936 2020-02-02 00:00:00.000000 investlib-0.0.3/tests/test_strategy.py
+-rw-r--r--   0        0        0     3125 2020-02-02 00:00:00.000000 investlib-0.0.3/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 investlib-0.0.3/LICENSE
+-rw-r--r--   0        0        0     2865 2020-02-02 00:00:00.000000 investlib-0.0.3/README.md
+-rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 investlib-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     3837 2020-02-02 00:00:00.000000 investlib-0.0.3/PKG-INFO
```

### Comparing `investlib-0.0.2/investlib/backtest.py` & `investlib-0.0.3/investlib/backtest.py`

 * *Files identical despite different names*

### Comparing `investlib-0.0.2/investlib/core.py` & `investlib-0.0.3/investlib/core.py`

 * *Files identical despite different names*

### Comparing `investlib-0.0.2/investlib/data.py` & `investlib-0.0.3/investlib/data.py`

 * *Files identical despite different names*

### Comparing `investlib-0.0.2/investlib/download.py` & `investlib-0.0.3/investlib/download.py`

 * *Files identical despite different names*

### Comparing `investlib-0.0.2/investlib/draw.py` & `investlib-0.0.3/investlib/draw.py`

 * *Files identical despite different names*

### Comparing `investlib-0.0.2/investlib/filters.py` & `investlib-0.0.3/investlib/filters.py`

 * *Files identical despite different names*

### Comparing `investlib-0.0.2/investlib/portfolio.py` & `investlib-0.0.3/investlib/portfolio.py`

 * *Files identical despite different names*

### Comparing `investlib-0.0.2/investlib/rebalance.py` & `investlib-0.0.3/investlib/rebalance.py`

 * *Files identical despite different names*

### Comparing `investlib-0.0.2/investlib/spydiffeqw.py` & `investlib-0.0.3/investlib/spydiffeqw.py`

 * *Files identical despite different names*

### Comparing `investlib-0.0.2/investlib/spystdreb.py` & `investlib-0.0.3/investlib/spystdreb.py`

 * *Files identical despite different names*

### Comparing `investlib-0.0.2/investlib/strategy.py` & `investlib-0.0.3/investlib/strategy.py`

 * *Files identical despite different names*

### Comparing `investlib-0.0.2/tests/test_data.py` & `investlib-0.0.3/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `investlib-0.0.2/tests/test_filters.py` & `investlib-0.0.3/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `investlib-0.0.2/tests/test_rebalance.py` & `investlib-0.0.3/tests/test_rebalance.py`

 * *Files identical despite different names*

### Comparing `investlib-0.0.2/tests/test_strategy.py` & `investlib-0.0.3/tests/test_strategy.py`

 * *Files identical despite different names*

### Comparing `investlib-0.0.2/.gitignore` & `investlib-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `investlib-0.0.2/LICENSE` & `investlib-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `investlib-0.0.2/README.md` & `investlib-0.0.3/README.md`

 * *Files identical despite different names*

