# Comparing `tmp/atro-pylog-0.1.1.tar.gz` & `tmp/atro-pylog-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atro-pylog-0.1.1.tar", last modified: Sun Jun 25 10:17:29 2023, max compression
+gzip compressed data, was "atro-pylog-0.1.2.tar", last modified: Sun Jul  2 10:44:06 2023, max compression
```

## Comparing `atro-pylog-0.1.1.tar` & `atro-pylog-0.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 atropos   (1000) atropos   (1000)        0 2023-06-25 10:17:29.120400 atro-pylog-0.1.1/
--rw-r--r--   0 atropos   (1000) atropos   (1000)      772 2023-06-25 10:17:29.120400 atro-pylog-0.1.1/PKG-INFO
--rw-r--r--   0 atropos   (1000) atropos   (1000)        0 2023-06-17 12:33:58.000000 atro-pylog-0.1.1/README.md
-drwxr-xr-x   0 atropos   (1000) atropos   (1000)        0 2023-06-25 10:17:29.120400 atro-pylog-0.1.1/atro_pylog.egg-info/
--rw-r--r--   0 atropos   (1000) atropos   (1000)      772 2023-06-25 10:17:29.000000 atro-pylog-0.1.1/atro_pylog.egg-info/PKG-INFO
--rw-r--r--   0 atropos   (1000) atropos   (1000)      308 2023-06-25 10:17:29.000000 atro-pylog-0.1.1/atro_pylog.egg-info/SOURCES.txt
--rw-r--r--   0 atropos   (1000) atropos   (1000)        1 2023-06-25 10:17:29.000000 atro-pylog-0.1.1/atro_pylog.egg-info/dependency_links.txt
--rw-r--r--   0 atropos   (1000) atropos   (1000)      103 2023-06-25 10:17:29.000000 atro-pylog-0.1.1/atro_pylog.egg-info/requires.txt
--rw-r--r--   0 atropos   (1000) atropos   (1000)        6 2023-06-25 10:17:29.000000 atro-pylog-0.1.1/atro_pylog.egg-info/top_level.txt
-drwxr-xr-x   0 atropos   (1000) atropos   (1000)        0 2023-06-25 10:17:29.120400 atro-pylog-0.1.1/pylog/
--rw-r--r--   0 atropos   (1000) atropos   (1000)     1763 2023-06-25 09:30:27.000000 atro-pylog-0.1.1/pylog/__init__.py
--rw-r--r--   0 atropos   (1000) atropos   (1000)     1050 2023-06-24 13:08:30.000000 atro-pylog-0.1.1/pylog/level.py
--rw-r--r--   0 atropos   (1000) atropos   (1000)      363 2023-06-24 13:08:30.000000 atro-pylog-0.1.1/pylog/logger_type.py
--rw-r--r--   0 atropos   (1000) atropos   (1000)     1106 2023-06-25 09:30:29.000000 atro-pylog-0.1.1/pylog/opentelemetry_setup.py
--rw-r--r--   0 atropos   (1000) atropos   (1000)      127 2023-06-25 09:16:13.000000 atro-pylog-0.1.1/pylog/rich_setup.py
--rw-r--r--   0 atropos   (1000) atropos   (1000)      766 2023-06-25 10:09:27.000000 atro-pylog-0.1.1/pylog/settings.py
--rw-r--r--   0 atropos   (1000) atropos   (1000)       38 2023-06-25 10:17:29.120400 atro-pylog-0.1.1/setup.cfg
--rw-r--r--   0 atropos   (1000) atropos   (1000)     1086 2023-06-25 10:17:11.000000 atro-pylog-0.1.1/setup.py
+drwxr-xr-x   0 atropos   (1000) atropos   (1000)        0 2023-07-02 10:44:06.622421 atro-pylog-0.1.2/
+-rw-r--r--   0 atropos   (1000) atropos   (1000)      772 2023-07-02 10:44:06.622421 atro-pylog-0.1.2/PKG-INFO
+-rw-r--r--   0 atropos   (1000) atropos   (1000)        0 2023-07-02 10:20:33.000000 atro-pylog-0.1.2/README.md
+drwxr-xr-x   0 atropos   (1000) atropos   (1000)        0 2023-07-02 10:44:06.619088 atro-pylog-0.1.2/atro_pylog.egg-info/
+-rw-r--r--   0 atropos   (1000) atropos   (1000)      772 2023-07-02 10:44:06.000000 atro-pylog-0.1.2/atro_pylog.egg-info/PKG-INFO
+-rw-r--r--   0 atropos   (1000) atropos   (1000)      308 2023-07-02 10:44:06.000000 atro-pylog-0.1.2/atro_pylog.egg-info/SOURCES.txt
+-rw-r--r--   0 atropos   (1000) atropos   (1000)        1 2023-07-02 10:44:06.000000 atro-pylog-0.1.2/atro_pylog.egg-info/dependency_links.txt
+-rw-r--r--   0 atropos   (1000) atropos   (1000)      121 2023-07-02 10:44:06.000000 atro-pylog-0.1.2/atro_pylog.egg-info/requires.txt
+-rw-r--r--   0 atropos   (1000) atropos   (1000)        6 2023-07-02 10:44:06.000000 atro-pylog-0.1.2/atro_pylog.egg-info/top_level.txt
+drwxr-xr-x   0 atropos   (1000) atropos   (1000)        0 2023-07-02 10:44:06.619088 atro-pylog-0.1.2/pylog/
+-rw-r--r--   0 atropos   (1000) atropos   (1000)     1763 2023-07-02 10:28:41.000000 atro-pylog-0.1.2/pylog/__init__.py
+-rw-r--r--   0 atropos   (1000) atropos   (1000)     1050 2023-07-02 10:20:33.000000 atro-pylog-0.1.2/pylog/level.py
+-rw-r--r--   0 atropos   (1000) atropos   (1000)      363 2023-07-02 10:20:33.000000 atro-pylog-0.1.2/pylog/logger_type.py
+-rw-r--r--   0 atropos   (1000) atropos   (1000)     1106 2023-07-02 10:20:33.000000 atro-pylog-0.1.2/pylog/opentelemetry_setup.py
+-rw-r--r--   0 atropos   (1000) atropos   (1000)      127 2023-07-02 10:20:33.000000 atro-pylog-0.1.2/pylog/rich_setup.py
+-rw-r--r--   0 atropos   (1000) atropos   (1000)      647 2023-07-02 10:29:30.000000 atro-pylog-0.1.2/pylog/settings.py
+-rw-r--r--   0 atropos   (1000) atropos   (1000)       38 2023-07-02 10:44:06.622421 atro-pylog-0.1.2/setup.cfg
+-rw-r--r--   0 atropos   (1000) atropos   (1000)     1107 2023-07-02 10:29:48.000000 atro-pylog-0.1.2/setup.py
```

### Comparing `atro-pylog-0.1.1/PKG-INFO` & `atro-pylog-0.1.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atro-pylog
-Version: 0.1.1
+Version: 0.1.2
 Summary: A simple logging library for Python. That either uses Loguru or OpenTelmetry collector (useful for local & cluster logging).
 Home-page: https://github.com/atropos/atro-pylog
 Author: Atropos
 Author-email: pypi.rising@atro.xyz
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `atro-pylog-0.1.1/atro_pylog.egg-info/PKG-INFO` & `atro-pylog-0.1.2/atro_pylog.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atro-pylog
-Version: 0.1.1
+Version: 0.1.2
 Summary: A simple logging library for Python. That either uses Loguru or OpenTelmetry collector (useful for local & cluster logging).
 Home-page: https://github.com/atropos/atro-pylog
 Author: Atropos
 Author-email: pypi.rising@atro.xyz
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `atro-pylog-0.1.1/pylog/__init__.py` & `atro-pylog-0.1.2/pylog/__init__.py`

 * *Files identical despite different names*

### Comparing `atro-pylog-0.1.1/pylog/level.py` & `atro-pylog-0.1.2/pylog/level.py`

 * *Files identical despite different names*

### Comparing `atro-pylog-0.1.1/pylog/opentelemetry_setup.py` & `atro-pylog-0.1.2/pylog/opentelemetry_setup.py`

 * *Files identical despite different names*

### Comparing `atro-pylog-0.1.1/pylog/settings.py` & `atro-pylog-0.1.2/pylog/settings.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,23 @@
 import logging
-
-from pydantic import BaseSettings
 from pathlib import Path
 
+from pydantic_settings import BaseSettings, SettingsConfigDict
+
 class BaseLoggerSettings(BaseSettings):
     name: str = "pylog"
     type: str = "rich"
     level: int | str = logging.DEBUG
     msg_format: str = "%(message)s"
     date_format: str = "%X"
 
-    class Config:
-        env_prefix = "ATRO_PYLOG_"
-        env_file = (Path.home() / ".config" / "atro" / "pylog.env").as_posix(), ".env"
-        env_file_encoding = "utf-8"
+    model_config = SettingsConfigDict(
+        env_prefix="ATRO_PYLOG_",
+        env_file=[(Path.home() / ".config" / "atro" / "pylog.env").as_posix(), ".env"],
+        env_file_encoding="utf-8",
+    )
 
 
-class OpenTelemetryLoggerSettings(BaseSettings):
+class OpenTelemetryLoggerSettings(BaseLoggerSettings):
     service_name: str = "pylog"
     instance_id: str = "pylog"
-    endpoint: str | None = None
-
-    class Config:
-        env_prefix = "ATRO_PYLOG_"
-        env_file = (Path.home() / ".config" / "atro" / "pylog.env").as_posix(), ".env", 
-        env_file_encoding = "utf-8"
+    endpoint: str | None = None
```

### Comparing `atro-pylog-0.1.1/setup.py` & `atro-pylog-0.1.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from setuptools import find_packages, setup
 
 setup(
     name="atro-pylog",
-    version="0.1.1",
+    version="0.1.2",
     packages=find_packages(),
     author="Atropos",
     author_email="pypi.rising@atro.xyz",
     description="A simple logging library for Python. That either uses Loguru or OpenTelmetry collector (useful for local & cluster logging).",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/atropos/atro-pylog",
-    install_requires=["rich", "opentelemetry-api", "opentelemetry-exporter-otlp-proto-grpc", "opentelemetry-sdk", "pydantic", "python-dotenv"],
+    install_requires=["rich", "opentelemetry-api", "opentelemetry-exporter-otlp-proto-grpc", "opentelemetry-sdk", "pydantic", "python-dotenv", "pydantic-settings"],
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
```

