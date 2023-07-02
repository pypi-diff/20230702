# Comparing `tmp/bpx-0.2.0.tar.gz` & `tmp/bpx-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bpx-0.2.0.tar", last modified: Tue Dec 13 14:49:04 2022, max compression
+gzip compressed data, was "bpx-0.3.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `bpx-0.2.0.tar` & `bpx-0.3.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     3341 2022-12-13 14:48:52.871957 bpx-0.2.0/README.md
--rw-r--r--   0        0        0      375 2022-12-13 14:48:52.871957 bpx-0.2.0/bpx/__init__.py
--rw-r--r--   0        0        0     2183 2022-12-13 14:48:52.871957 bpx-0.2.0/bpx/expression_parser.py
--rw-r--r--   0        0        0     2188 2022-12-13 14:48:52.871957 bpx-0.2.0/bpx/function.py
--rw-r--r--   0        0        0      355 2022-12-13 14:48:52.871957 bpx-0.2.0/bpx/interpolated_table.py
--rw-r--r--   0        0        0      721 2022-12-13 14:48:52.871957 bpx-0.2.0/bpx/parsers.py
--rw-r--r--   0        0        0     9109 2022-12-13 14:48:52.871957 bpx-0.2.0/bpx/schema.py
--rw-r--r--   0        0        0     1827 2022-12-13 14:48:52.871957 bpx-0.2.0/bpx/utilities.py
--rw-r--r--   0        0        0      443 2022-12-13 14:48:52.871957 bpx-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     3675 1970-01-01 00:00:00.000000 bpx-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     3282 2023-07-02 21:35:47.806817 bpx-0.3.1/README.md
+-rw-r--r--   0        0        0      375 2023-07-02 21:35:47.806817 bpx-0.3.1/bpx/__init__.py
+-rw-r--r--   0        0        0     2183 2023-07-02 21:35:47.806817 bpx-0.3.1/bpx/expression_parser.py
+-rw-r--r--   0        0        0     2188 2023-07-02 21:35:47.806817 bpx-0.3.1/bpx/function.py
+-rw-r--r--   0        0        0      355 2023-07-02 21:35:47.806817 bpx-0.3.1/bpx/interpolated_table.py
+-rw-r--r--   0        0        0      721 2023-07-02 21:35:47.806817 bpx-0.3.1/bpx/parsers.py
+-rw-r--r--   0        0        0     9109 2023-07-02 21:35:47.806817 bpx-0.3.1/bpx/schema.py
+-rw-r--r--   0        0        0     1827 2023-07-02 21:35:47.806817 bpx-0.3.1/bpx/utilities.py
+-rw-r--r--   0        0        0      445 2023-07-02 21:35:47.806817 bpx-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     3618 1970-01-01 00:00:00.000000 bpx-0.3.1/PKG-INFO
```

### Comparing `bpx-0.2.0/README.md` & `bpx-0.3.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -18,18 +18,18 @@
 Create a new virtual environment, or activate an existing one (this example uses the python `venv` module, but you could use Anaconda and a `conda` environment)
 
 ```bash
 python3 -m venv env
 source env/bin/activate
 ```
 
-Install the `BPX` module from the repository on GitHub
+Install the `BPX` module using pip
 
 ```bash
-pip install git+https://github.com/pybamm-team/BPX.git
+pip install bpx
 ```
 
 ## Usage
 
 Create a python script similar to that below
 
 ```python
```

### Comparing `bpx-0.2.0/bpx/expression_parser.py` & `bpx-0.3.1/bpx/expression_parser.py`

 * *Files identical despite different names*

### Comparing `bpx-0.2.0/bpx/function.py` & `bpx-0.3.1/bpx/function.py`

 * *Files identical despite different names*

### Comparing `bpx-0.2.0/bpx/parsers.py` & `bpx-0.3.1/bpx/parsers.py`

 * *Files identical despite different names*

### Comparing `bpx-0.2.0/bpx/schema.py` & `bpx-0.3.1/bpx/schema.py`

 * *Files identical despite different names*

### Comparing `bpx-0.2.0/bpx/utilities.py` & `bpx-0.3.1/bpx/utilities.py`

 * *Files identical despite different names*

### Comparing `bpx-0.2.0/PKG-INFO` & `bpx-0.3.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: bpx
-Version: 0.2.0
+Version: 0.3.1
 Summary: BPX schema and parsers
 Author-email: Martin Robinson <martin.robinson@dtc.ox.ac.uk>
 Description-Content-Type: text/markdown
-Requires-Dist: pydantic
+Requires-Dist: pydantic<2
 Requires-Dist: pyparsing
 Requires-Dist: coverage ; extra == "dev"
 Requires-Dist: flake8>=3 ; extra == "dev"
 Provides-Extra: dev
 
 # BPX
 ![tests](https://github.com/pybamm-team/BPX/actions/workflows/test.yml/badge.svg)
@@ -30,18 +30,18 @@
 Create a new virtual environment, or activate an existing one (this example uses the python `venv` module, but you could use Anaconda and a `conda` environment)
 
 ```bash
 python3 -m venv env
 source env/bin/activate
 ```
 
-Install the `BPX` module from the repository on GitHub
+Install the `BPX` module using pip
 
 ```bash
-pip install git+https://github.com/pybamm-team/BPX.git
+pip install bpx
 ```
 
 ## Usage
 
 Create a python script similar to that below
 
 ```python
```

