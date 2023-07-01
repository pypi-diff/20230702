# Comparing `tmp/rabe_cridlib-0.8.0.tar.gz` & `tmp/rabe_cridlib-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rabe_cridlib-0.8.0.tar", max compression
+gzip compressed data, was "rabe_cridlib-0.9.0.tar", max compression
```

## Comparing `rabe_cridlib-0.8.0.tar` & `rabe_cridlib-0.9.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    34520 2023-05-19 00:58:15.059495 rabe_cridlib-0.8.0/LICENSE
--rw-r--r--   0        0        0     2844 2023-05-19 00:58:15.059495 rabe_cridlib-0.8.0/README.md
--rw-r--r--   0        0        0      343 2023-05-19 00:58:15.059495 rabe_cridlib-0.8.0/cridlib/__init__.py
--rw-r--r--   0        0        0     1419 2023-05-19 00:58:15.059495 rabe_cridlib-0.8.0/cridlib/get.py
--rw-r--r--   0        0        0     4586 2023-05-19 00:58:15.059495 rabe_cridlib-0.8.0/cridlib/lib.py
--rw-r--r--   0        0        0      221 2023-05-19 00:58:15.059495 rabe_cridlib-0.8.0/cridlib/parse.py
--rw-r--r--   0        0        0        0 2023-05-19 00:58:15.059495 rabe_cridlib-0.8.0/cridlib/py.typed
--rw-r--r--   0        0        0      192 2023-05-19 00:58:15.059495 rabe_cridlib-0.8.0/cridlib/strategy/__init__.py
--rw-r--r--   0        0        0     1305 2023-05-19 00:58:15.059495 rabe_cridlib-0.8.0/cridlib/strategy/future.py
--rw-r--r--   0        0        0      624 2023-05-19 00:58:15.059495 rabe_cridlib-0.8.0/cridlib/strategy/now.py
--rw-r--r--   0        0        0      772 2023-05-19 00:58:15.059495 rabe_cridlib-0.8.0/cridlib/strategy/past.py
--rw-r--r--   0        0        0     1051 2023-05-19 00:58:15.059495 rabe_cridlib-0.8.0/cridlib/util.py
--rw-r--r--   0        0        0     1544 2023-05-19 00:58:41.595635 rabe_cridlib-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     3835 1970-01-01 00:00:00.000000 rabe_cridlib-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0    34520 2023-06-04 20:48:12.261777 rabe_cridlib-0.9.0/LICENSE
+-rw-r--r--   0        0        0     2844 2023-06-04 20:48:12.261777 rabe_cridlib-0.9.0/README.md
+-rw-r--r--   0        0        0      343 2023-06-04 20:48:12.261777 rabe_cridlib-0.9.0/cridlib/__init__.py
+-rw-r--r--   0        0        0     1419 2023-06-04 20:48:12.261777 rabe_cridlib-0.9.0/cridlib/get.py
+-rw-r--r--   0        0        0     4586 2023-06-04 20:48:12.261777 rabe_cridlib-0.9.0/cridlib/lib.py
+-rw-r--r--   0        0        0      221 2023-06-04 20:48:12.261777 rabe_cridlib-0.9.0/cridlib/parse.py
+-rw-r--r--   0        0        0        0 2023-06-04 20:48:12.261777 rabe_cridlib-0.9.0/cridlib/py.typed
+-rw-r--r--   0        0        0      192 2023-06-04 20:48:12.261777 rabe_cridlib-0.9.0/cridlib/strategy/__init__.py
+-rw-r--r--   0        0        0     1305 2023-06-04 20:48:12.261777 rabe_cridlib-0.9.0/cridlib/strategy/future.py
+-rw-r--r--   0        0        0      624 2023-06-04 20:48:12.261777 rabe_cridlib-0.9.0/cridlib/strategy/now.py
+-rw-r--r--   0        0        0      772 2023-06-04 20:48:12.261777 rabe_cridlib-0.9.0/cridlib/strategy/past.py
+-rw-r--r--   0        0        0     1051 2023-06-04 20:48:12.261777 rabe_cridlib-0.9.0/cridlib/util.py
+-rw-r--r--   0        0        0     1634 2023-06-04 20:48:24.470030 rabe_cridlib-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     3882 1970-01-01 00:00:00.000000 rabe_cridlib-0.9.0/PKG-INFO
```

### Comparing `rabe_cridlib-0.8.0/LICENSE` & `rabe_cridlib-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rabe_cridlib-0.8.0/README.md` & `rabe_cridlib-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `rabe_cridlib-0.8.0/cridlib/get.py` & `rabe_cridlib-0.9.0/cridlib/get.py`

 * *Files identical despite different names*

### Comparing `rabe_cridlib-0.8.0/cridlib/lib.py` & `rabe_cridlib-0.9.0/cridlib/lib.py`

 * *Files identical despite different names*

### Comparing `rabe_cridlib-0.8.0/cridlib/strategy/future.py` & `rabe_cridlib-0.9.0/cridlib/strategy/future.py`

 * *Files identical despite different names*

### Comparing `rabe_cridlib-0.8.0/cridlib/strategy/now.py` & `rabe_cridlib-0.9.0/cridlib/strategy/now.py`

 * *Files identical despite different names*

### Comparing `rabe_cridlib-0.8.0/cridlib/strategy/past.py` & `rabe_cridlib-0.9.0/cridlib/strategy/past.py`

 * *Files identical despite different names*

### Comparing `rabe_cridlib-0.8.0/cridlib/util.py` & `rabe_cridlib-0.9.0/cridlib/util.py`

 * *Files identical despite different names*

### Comparing `rabe_cridlib-0.8.0/pyproject.toml` & `rabe_cridlib-0.9.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rabe-cridlib"
-version = "v0.8.0" # 0.0.0 placeholder is replaced on release
+version = "v0.9.0" # 0.0.0 placeholder is replaced on release
 description = "Generate CRIDs for RaBe"
 repository = "https://github.com/radiorabe/python-rabe-cridlib"
 authors = ["RaBe IT-Reaktion <it@rabe.ch>"]
 license = "AGPL-3"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
@@ -18,39 +18,41 @@
 
 [tool.poetry.dependencies]
 python = "^3.9"
 requests = "^2.28.1"
 uritools = "^4.0.0"
 pytz = ">=2022.6"
 python-slugify = "^8.0.0"
+cachecontrol = "^0.13.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.0"
 pytest-cov = "^4.0.0"
 wheel = ">=0.38.4,<0.41.0"
 types-requests = "^2.28.11"
 freezegun = "^1.2.2"
 requests-mock = "^1.10.0"
 black = ">=22.12,<24.0"
 isort = "^5.11.4"
 Markdown = "^3.3"
 pytest-mypy = "^0.10.3"
 pytest-random-order = "^1.1.0"
 types-pytz = ">=2022.7,<2024.0"
-mkdocstrings = {extras = ["python"], version = ">=0.20,<0.22"}
+mkdocstrings = {extras = ["python"], version = ">=0.20,<0.23"}
 mkdocs-material = ">=8,<10"
 mkdocs = "^1.4.2"
 mkdocs-gen-files = ">=0.4,<0.6"
 mkdocs-literate-nav = "^0.6.0"
 mkdocs-section-index = "^0.3.5"
 types-python-slugify = "^8.0.0.0"
 
 [tool.isort]
 profile = "black"
 
 [tool.pytest.ini_options]
 minversion = "7.2"
 addopts = "-ra -q --random-order --doctest-glob='*.md' --doctest-modules --cov=cridlib --cov-fail-under=100 --ignore=docs/ --mypy"
+filterwarnings = ["ignore::DeprecationWarning:pytest_freezegun"]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `rabe_cridlib-0.8.0/PKG-INFO` & `rabe_cridlib-0.9.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rabe-cridlib
-Version: 0.8.0
+Version: 0.9.0
 Summary: Generate CRIDs for RaBe
 Home-page: https://github.com/radiorabe/python-rabe-cridlib
 License: AGPL-3
 Author: RaBe IT-Reaktion
 Author-email: it@rabe.ch
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 3 - Alpha
@@ -12,14 +12,15 @@
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Multimedia :: Sound/Audio :: Conversion
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Dist: cachecontrol (>=0.13.0,<0.14.0)
 Requires-Dist: python-slugify (>=8.0.0,<9.0.0)
 Requires-Dist: pytz (>=2022.6)
 Requires-Dist: requests (>=2.28.1,<3.0.0)
 Requires-Dist: uritools (>=4.0.0,<5.0.0)
 Project-URL: Repository, https://github.com/radiorabe/python-rabe-cridlib
 Description-Content-Type: text/markdown
```

