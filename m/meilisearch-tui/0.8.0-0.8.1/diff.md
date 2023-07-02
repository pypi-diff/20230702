# Comparing `tmp/meilisearch_tui-0.8.0.tar.gz` & `tmp/meilisearch_tui-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meilisearch_tui-0.8.0.tar", max compression
+gzip compressed data, was "meilisearch_tui-0.8.1.tar", max compression
```

## Comparing `meilisearch_tui-0.8.0.tar` & `meilisearch_tui-0.8.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1069 2023-06-23 13:58:16.256510 meilisearch_tui-0.8.0/LICENSE
--rw-r--r--   0        0        0     2045 2023-06-23 13:58:16.256510 meilisearch_tui-0.8.0/README.md
--rw-r--r--   0        0        0        0 2023-06-23 13:58:16.260511 meilisearch_tui-0.8.0/meilisearch_tui/__init__.py
--rw-r--r--   0        0        0      115 2023-06-23 13:58:16.260511 meilisearch_tui-0.8.0/meilisearch_tui/__main__.py
--rw-r--r--   0        0        0      608 2023-06-23 13:58:16.260511 meilisearch_tui-0.8.0/meilisearch_tui/client.py
--rw-r--r--   0        0        0     3226 2023-06-23 13:58:16.260511 meilisearch_tui-0.8.0/meilisearch_tui/config.py
--rw-r--r--   0        0        0       86 2023-06-23 13:58:16.260511 meilisearch_tui-0.8.0/meilisearch_tui/errors.py
--rw-r--r--   0        0        0     2780 2023-06-23 13:58:16.260511 meilisearch_tui-0.8.0/meilisearch_tui/main.py
--rw-r--r--   0        0        0     1908 2023-06-23 13:58:16.260511 meilisearch_tui-0.8.0/meilisearch_tui/meilisearch.css
--rw-r--r--   0        0        0        0 2023-06-23 13:58:16.260511 meilisearch_tui-0.8.0/meilisearch_tui/py.typed
--rw-r--r--   0        0        0        0 2023-06-23 13:58:16.260511 meilisearch_tui-0.8.0/meilisearch_tui/screens/__init__.py
--rw-r--r--   0        0        0     4518 2023-06-23 13:58:16.260511 meilisearch_tui-0.8.0/meilisearch_tui/screens/configuration.py
--rw-r--r--   0        0        0    28829 2023-06-23 13:58:16.260511 meilisearch_tui-0.8.0/meilisearch_tui/screens/indexes.py
--rw-r--r--   0        0        0     6974 2023-06-23 13:58:16.260511 meilisearch_tui-0.8.0/meilisearch_tui/screens/search.py
--rw-r--r--   0        0        0      897 2023-06-23 13:58:16.260511 meilisearch_tui-0.8.0/meilisearch_tui/utils.py
--rw-r--r--   0        0        0        0 2023-06-23 13:58:16.260511 meilisearch_tui-0.8.0/meilisearch_tui/widgets/__init__.py
--rw-r--r--   0        0        0      844 2023-06-23 13:58:16.260511 meilisearch_tui-0.8.0/meilisearch_tui/widgets/index.py
--rw-r--r--   0        0        0     1543 2023-06-23 13:58:16.260511 meilisearch_tui-0.8.0/meilisearch_tui/widgets/index_sidebar.py
--rw-r--r--   0        0        0     1730 2023-06-23 13:58:16.260511 meilisearch_tui-0.8.0/meilisearch_tui/widgets/input.py
--rw-r--r--   0        0        0      709 2023-06-23 13:58:16.260511 meilisearch_tui-0.8.0/meilisearch_tui/widgets/messages.py
--rw-r--r--   0        0        0     2099 2023-06-23 13:58:16.264511 meilisearch_tui-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     3095 1970-01-01 00:00:00.000000 meilisearch_tui-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-07-02 02:10:59.449308 meilisearch_tui-0.8.1/LICENSE
+-rw-r--r--   0        0        0     2045 2023-07-02 02:10:59.449308 meilisearch_tui-0.8.1/README.md
+-rw-r--r--   0        0        0        0 2023-07-02 02:10:59.449308 meilisearch_tui-0.8.1/meilisearch_tui/__init__.py
+-rw-r--r--   0        0        0      115 2023-07-02 02:10:59.449308 meilisearch_tui-0.8.1/meilisearch_tui/__main__.py
+-rw-r--r--   0        0        0      608 2023-07-02 02:10:59.449308 meilisearch_tui-0.8.1/meilisearch_tui/client.py
+-rw-r--r--   0        0        0     3226 2023-07-02 02:10:59.449308 meilisearch_tui-0.8.1/meilisearch_tui/config.py
+-rw-r--r--   0        0        0       86 2023-07-02 02:10:59.449308 meilisearch_tui-0.8.1/meilisearch_tui/errors.py
+-rw-r--r--   0        0        0     2780 2023-07-02 02:10:59.449308 meilisearch_tui-0.8.1/meilisearch_tui/main.py
+-rw-r--r--   0        0        0     1908 2023-07-02 02:10:59.449308 meilisearch_tui-0.8.1/meilisearch_tui/meilisearch.css
+-rw-r--r--   0        0        0        0 2023-07-02 02:10:59.449308 meilisearch_tui-0.8.1/meilisearch_tui/py.typed
+-rw-r--r--   0        0        0        0 2023-07-02 02:10:59.449308 meilisearch_tui-0.8.1/meilisearch_tui/screens/__init__.py
+-rw-r--r--   0        0        0     4518 2023-07-02 02:10:59.449308 meilisearch_tui-0.8.1/meilisearch_tui/screens/configuration.py
+-rw-r--r--   0        0        0    28829 2023-07-02 02:10:59.449308 meilisearch_tui-0.8.1/meilisearch_tui/screens/indexes.py
+-rw-r--r--   0        0        0     6974 2023-07-02 02:10:59.449308 meilisearch_tui-0.8.1/meilisearch_tui/screens/search.py
+-rw-r--r--   0        0        0      897 2023-07-02 02:10:59.453308 meilisearch_tui-0.8.1/meilisearch_tui/utils.py
+-rw-r--r--   0        0        0        0 2023-07-02 02:10:59.453308 meilisearch_tui-0.8.1/meilisearch_tui/widgets/__init__.py
+-rw-r--r--   0        0        0      844 2023-07-02 02:10:59.453308 meilisearch_tui-0.8.1/meilisearch_tui/widgets/index.py
+-rw-r--r--   0        0        0     1543 2023-07-02 02:10:59.453308 meilisearch_tui-0.8.1/meilisearch_tui/widgets/index_sidebar.py
+-rw-r--r--   0        0        0     1730 2023-07-02 02:10:59.453308 meilisearch_tui-0.8.1/meilisearch_tui/widgets/input.py
+-rw-r--r--   0        0        0      709 2023-07-02 02:10:59.453308 meilisearch_tui-0.8.1/meilisearch_tui/widgets/messages.py
+-rw-r--r--   0        0        0     2125 2023-07-02 02:10:59.453308 meilisearch_tui-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0     3095 1970-01-01 00:00:00.000000 meilisearch_tui-0.8.1/PKG-INFO
```

### Comparing `meilisearch_tui-0.8.0/LICENSE` & `meilisearch_tui-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `meilisearch_tui-0.8.0/README.md` & `meilisearch_tui-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `meilisearch_tui-0.8.0/meilisearch_tui/client.py` & `meilisearch_tui-0.8.1/meilisearch_tui/client.py`

 * *Files identical despite different names*

### Comparing `meilisearch_tui-0.8.0/meilisearch_tui/config.py` & `meilisearch_tui-0.8.1/meilisearch_tui/config.py`

 * *Files identical despite different names*

### Comparing `meilisearch_tui-0.8.0/meilisearch_tui/main.py` & `meilisearch_tui-0.8.1/meilisearch_tui/main.py`

 * *Files identical despite different names*

### Comparing `meilisearch_tui-0.8.0/meilisearch_tui/meilisearch.css` & `meilisearch_tui-0.8.1/meilisearch_tui/meilisearch.css`

 * *Files identical despite different names*

### Comparing `meilisearch_tui-0.8.0/meilisearch_tui/screens/configuration.py` & `meilisearch_tui-0.8.1/meilisearch_tui/screens/configuration.py`

 * *Files identical despite different names*

### Comparing `meilisearch_tui-0.8.0/meilisearch_tui/screens/indexes.py` & `meilisearch_tui-0.8.1/meilisearch_tui/screens/indexes.py`

 * *Files identical despite different names*

### Comparing `meilisearch_tui-0.8.0/meilisearch_tui/screens/search.py` & `meilisearch_tui-0.8.1/meilisearch_tui/screens/search.py`

 * *Files identical despite different names*

### Comparing `meilisearch_tui-0.8.0/meilisearch_tui/utils.py` & `meilisearch_tui-0.8.1/meilisearch_tui/utils.py`

 * *Files identical despite different names*

### Comparing `meilisearch_tui-0.8.0/meilisearch_tui/widgets/index.py` & `meilisearch_tui-0.8.1/meilisearch_tui/widgets/index.py`

 * *Files identical despite different names*

### Comparing `meilisearch_tui-0.8.0/meilisearch_tui/widgets/index_sidebar.py` & `meilisearch_tui-0.8.1/meilisearch_tui/widgets/index_sidebar.py`

 * *Files identical despite different names*

### Comparing `meilisearch_tui-0.8.0/meilisearch_tui/widgets/input.py` & `meilisearch_tui-0.8.1/meilisearch_tui/widgets/input.py`

 * *Files identical despite different names*

### Comparing `meilisearch_tui-0.8.0/meilisearch_tui/widgets/messages.py` & `meilisearch_tui-0.8.1/meilisearch_tui/widgets/messages.py`

 * *Files identical despite different names*

### Comparing `meilisearch_tui-0.8.0/pyproject.toml` & `meilisearch_tui-0.8.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "meilisearch-tui"
-version = "0.8.0"
+version = "0.8.1"
 description = "A TUI for Managing and Searching with Meilisearch"
 authors = ["Paul Sanders <psanders1@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/sanders41/meilisearch-tui"
 homepage = "https://github.com/sanders41/meilisearch-tui"
 documentation = "https://github.com/sanders41/meilisearch-tui"
@@ -17,27 +17,27 @@
   "Programming Language :: Python :: 3.11",
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-meilisearch-python-async = "1.4.1"
+meilisearch-python-async = "1.4.3"
 textual = "0.28.1"
 uvloop = {version = "0.17.0", markers = "sys_platform != 'win32'"}
 aiocache = "0.12.1"
 
 [tool.poetry.group.dev.dependencies]
 aiohttp = "3.8.4"
 black = "23.3.0"
 click = "8.1.3"
 msgpack = "1.0.5"
-mypy = "1.4.0"
+mypy = "1.4.1"
 pre-commit = "3.3.3"
-pytest = "7.3.2"
+pytest = "7.4.0"
 pytest-asyncio = "0.21.0"
 pytest-cov = "4.1.0"
 ruff = "0.0.275"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
@@ -77,14 +77,15 @@
 [[tool.mypy.overrides]]
 module = ["aiocache.*"]
 ignore_missing_imports = true
 
 [tool.pytest.ini_options]
 minversion = "6.0"
 addopts = "--cov=meilisearch_tui --cov-report term-missing"
+markers = ["meilisearch"]
 asyncio_mode = "auto"
 
 [tool.coverage.report]
 exclude_lines = ["if __name__ == .__main__.:", "pragma: no cover"]
 
 [tool.ruff]
 select = ["E", "F", "UP", "I001", "T201", "T203"]
```

### Comparing `meilisearch_tui-0.8.0/PKG-INFO` & `meilisearch_tui-0.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meilisearch-tui
-Version: 0.8.0
+Version: 0.8.1
 Summary: A TUI for Managing and Searching with Meilisearch
 Home-page: https://github.com/sanders41/meilisearch-tui
 License: MIT
 Keywords: meilisearch,tui
 Author: Paul Sanders
 Author-email: psanders1@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -13,15 +13,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiocache (==0.12.1)
-Requires-Dist: meilisearch-python-async (==1.4.1)
+Requires-Dist: meilisearch-python-async (==1.4.3)
 Requires-Dist: textual (==0.28.1)
 Requires-Dist: uvloop (==0.17.0) ; sys_platform != "win32"
 Project-URL: Documentation, https://github.com/sanders41/meilisearch-tui
 Project-URL: Repository, https://github.com/sanders41/meilisearch-tui
 Description-Content-Type: text/markdown
 
 # Meilisearch TUI
```

