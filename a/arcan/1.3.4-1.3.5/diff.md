# Comparing `tmp/arcan-1.3.4.tar.gz` & `tmp/arcan-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arcan-1.3.4.tar", max compression
+gzip compressed data, was "arcan-1.3.5.tar", max compression
```

## Comparing `arcan-1.3.4.tar` & `arcan-1.3.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1711 2023-07-01 05:13:19.079033 arcan-1.3.4/LICENSE
--rw-r--r--   0        0        0     5132 2023-07-01 05:13:19.079033 arcan-1.3.4/README.md
--rw-r--r--   0        0        0      907 2023-07-01 05:13:19.083033 arcan-1.3.4/arcan/__init__.py
--rw-r--r--   0        0        0        0 2023-07-01 05:13:19.083033 arcan-1.3.4/arcan/agent/__init__.py
--rw-r--r--   0        0        0        0 2023-07-01 05:13:19.083033 arcan-1.3.4/arcan/engines/__init__.py
--rw-r--r--   0        0        0       24 2023-07-01 05:13:19.083033 arcan-1.3.4/arcan/engines/io.py
--rw-r--r--   0        0        0        0 2023-07-01 05:13:19.083033 arcan-1.3.4/arcan/governance/__init__.py
--rw-r--r--   0        0        0        0 2023-07-01 05:13:19.083033 arcan-1.3.4/arcan/governance/catalog/__init__.py
--rw-r--r--   0        0        0        0 2023-07-01 05:13:19.083033 arcan-1.3.4/arcan/governance/lifecycle/__init__.py
--rw-r--r--   0        0        0        0 2023-07-01 05:13:19.083033 arcan-1.3.4/arcan/governance/mdm/__init__.py
--rw-r--r--   0        0        0        0 2023-07-01 05:13:19.083033 arcan-1.3.4/arcan/governance/quality/__init__.py
--rw-r--r--   0        0        0        0 2023-07-01 05:13:19.083033 arcan-1.3.4/arcan/orchestrator/__init__.py
--rw-r--r--   0        0        0      478 2023-07-01 05:13:19.083033 arcan-1.3.4/arcan/processing/__init__.py
--rw-r--r--   0        0        0        0 2023-07-01 05:13:19.083033 arcan-1.3.4/arcan/processing/pipelines/__init__.py
--rw-r--r--   0        0        0        0 2023-07-01 05:13:19.083033 arcan-1.3.4/arcan/processing/quality/__init__.py
--rw-r--r--   0        0        0        0 2023-07-01 05:13:19.083033 arcan-1.3.4/arcan/processing/transformations/__init__.py
--rw-r--r--   0        0        0       91 2023-07-01 05:13:19.083033 arcan-1.3.4/arcan/session/__init__.py
--rw-r--r--   0        0        0       62 2023-07-01 05:13:19.083033 arcan-1.3.4/main.py
--rw-r--r--   0        0        0      735 2023-07-01 05:13:19.087033 arcan-1.3.4/pyproject.toml
--rw-r--r--   0        0        0     5855 1970-01-01 00:00:00.000000 arcan-1.3.4/PKG-INFO
+-rw-r--r--   0        0        0     1711 2023-07-02 08:54:16.705825 arcan-1.3.5/LICENSE
+-rw-r--r--   0        0        0     2888 2023-07-02 08:54:16.705825 arcan-1.3.5/README.md
+-rw-r--r--   0        0        0      907 2023-07-02 08:54:16.709826 arcan-1.3.5/arcan/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-02 08:54:16.709826 arcan-1.3.5/arcan/agent/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-02 08:54:16.709826 arcan-1.3.5/arcan/engines/__init__.py
+-rw-r--r--   0        0        0       24 2023-07-02 08:54:16.709826 arcan-1.3.5/arcan/engines/io.py
+-rw-r--r--   0        0        0        0 2023-07-02 08:54:16.709826 arcan-1.3.5/arcan/governance/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-02 08:54:16.709826 arcan-1.3.5/arcan/governance/catalog/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-02 08:54:16.709826 arcan-1.3.5/arcan/governance/lifecycle/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-02 08:54:16.709826 arcan-1.3.5/arcan/governance/mdm/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-02 08:54:16.709826 arcan-1.3.5/arcan/governance/quality/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-02 08:54:16.709826 arcan-1.3.5/arcan/orchestrator/__init__.py
+-rw-r--r--   0        0        0      478 2023-07-02 08:54:16.709826 arcan-1.3.5/arcan/processing/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-02 08:54:16.709826 arcan-1.3.5/arcan/processing/pipelines/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-02 08:54:16.709826 arcan-1.3.5/arcan/processing/transformations/__init__.py
+-rw-r--r--   0        0        0       91 2023-07-02 08:54:16.709826 arcan-1.3.5/arcan/session/__init__.py
+-rw-r--r--   0        0        0       31 2023-07-02 08:54:16.709826 arcan-1.3.5/arcan/storage/__init__.py
+-rw-r--r--   0        0        0       62 2023-07-02 08:54:16.709826 arcan-1.3.5/main.py
+-rw-r--r--   0        0        0      753 2023-07-02 08:54:16.709826 arcan-1.3.5/pyproject.toml
+-rw-r--r--   0        0        0     3651 1970-01-01 00:00:00.000000 arcan-1.3.5/PKG-INFO
```

### Comparing `arcan-1.3.4/LICENSE` & `arcan-1.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `arcan-1.3.4/arcan/__init__.py` & `arcan-1.3.5/arcan/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # %%
 from modal import Stub, web_endpoint
 from modal import Image, Stub, web_endpoint
 
-__version__ = "1.3.4"
+__version__ = "1.3.5"
 
 
 # %%
 # %%
 def get_arcan_version():
     try:
         import arcan
```

### Comparing `arcan-1.3.4/pyproject.toml` & `arcan-1.3.5/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "arcan"
-version = "1.3.4"
+version = "1.3.5"
 description = "A multiheaded modern data bridging package based on pipeline manifests to integrate between any modern (and old) data stack tools"
 authors = ["Carlos D. Escobar-Valbuena <carlosdavidescobar@gmail.com>"]
 license = "arcan.ai Non-Commercial Open Source License"
 readme = "README.md"
 packages = [
     {include = "arcan"},
     {include = "main.py"}
@@ -12,14 +12,15 @@
 
 
 [tool.poetry.dependencies]
 python = "^3.10"
 fastapi = "^0.98.0"
 uvicorn = "^0.22.0"
 modal-client = "^0.49.2509"
+black = "^23.3.0"
 
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 ipykernel = "^6.23.3"
 
 [build-system]
```

