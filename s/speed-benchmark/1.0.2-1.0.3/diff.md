# Comparing `tmp/speed-benchmark-1.0.2.tar.gz` & `tmp/speed-benchmark-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "speed-benchmark-1.0.2.tar", last modified: Fri Jun 30 05:14:38 2023, max compression
+gzip compressed data, was "speed-benchmark-1.0.3.tar", last modified: Sun Jul  2 15:00:50 2023, max compression
```

## Comparing `speed-benchmark-1.0.2.tar` & `speed-benchmark-1.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 05:14:38.634760 speed-benchmark-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-06-30 05:14:38.634760 speed-benchmark-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-06-30 05:14:21.000000 speed-benchmark-1.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 05:14:38.634760 speed-benchmark-1.0.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1513 2023-06-30 05:14:21.000000 speed-benchmark-1.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 05:14:38.634760 speed-benchmark-1.0.2/speed_benchmark/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-30 05:14:21.000000 speed-benchmark-1.0.2/speed_benchmark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4767 2023-06-30 05:14:21.000000 speed-benchmark-1.0.2/speed_benchmark/speed_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 05:14:38.634760 speed-benchmark-1.0.2/speed_benchmark/visualization/
--rwxr-xr-x   0 runner    (1001) docker     (123)      106 2023-06-30 05:14:21.000000 speed-benchmark-1.0.2/speed_benchmark/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-30 05:14:21.000000 speed-benchmark-1.0.2/speed_benchmark/visualization/generate_color.py
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-06-30 05:14:21.000000 speed-benchmark-1.0.2/speed_benchmark/visualization/line_chart.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 05:14:38.634760 speed-benchmark-1.0.2/speed_benchmark.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-06-30 05:14:38.000000 speed-benchmark-1.0.2/speed_benchmark.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-30 05:14:38.000000 speed-benchmark-1.0.2/speed_benchmark.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 05:14:38.000000 speed-benchmark-1.0.2/speed_benchmark.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-30 05:14:38.000000 speed-benchmark-1.0.2/speed_benchmark.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-30 05:14:38.000000 speed-benchmark-1.0.2/speed_benchmark.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 15:00:50.317104 speed-benchmark-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-07-02 15:00:50.317104 speed-benchmark-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-07-02 15:00:40.000000 speed-benchmark-1.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 15:00:50.317104 speed-benchmark-1.0.3/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1513 2023-07-02 15:00:40.000000 speed-benchmark-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 15:00:50.313104 speed-benchmark-1.0.3/speed_benchmark/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-02 15:00:40.000000 speed-benchmark-1.0.3/speed_benchmark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4771 2023-07-02 15:00:40.000000 speed-benchmark-1.0.3/speed_benchmark/speed_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 15:00:50.317104 speed-benchmark-1.0.3/speed_benchmark/visualization/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      106 2023-07-02 15:00:40.000000 speed-benchmark-1.0.3/speed_benchmark/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-02 15:00:40.000000 speed-benchmark-1.0.3/speed_benchmark/visualization/generate_color.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-07-02 15:00:40.000000 speed-benchmark-1.0.3/speed_benchmark/visualization/line_chart.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 15:00:50.313104 speed-benchmark-1.0.3/speed_benchmark.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-07-02 15:00:50.000000 speed-benchmark-1.0.3/speed_benchmark.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-07-02 15:00:50.000000 speed-benchmark-1.0.3/speed_benchmark.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 15:00:50.000000 speed-benchmark-1.0.3/speed_benchmark.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-02 15:00:50.000000 speed-benchmark-1.0.3/speed_benchmark.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-02 15:00:50.000000 speed-benchmark-1.0.3/speed_benchmark.egg-info/top_level.txt
```

### Comparing `speed-benchmark-1.0.2/PKG-INFO` & `speed-benchmark-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: speed-benchmark
-Version: 1.0.2
+Version: 1.0.3
 Summary: A generic speed benchmark library.
 Home-page: https://github.com/shenmishajing/speed_benchmark
 Author: shenmishajing
 Author-email: shenmishajing@gmail.com
 License: MIT License
 Project-URL: Code, https://github.com/shenmishajing/speed_benchmark
 Project-URL: Issue tracker, https://github.com/shenmishajing/speed_benchmark/issues
```

### Comparing `speed-benchmark-1.0.2/README.md` & `speed-benchmark-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `speed-benchmark-1.0.2/setup.py` & `speed-benchmark-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="speed-benchmark",
-    version="1.0.2",
+    version="1.0.3",
     description="A generic speed benchmark library.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="shenmishajing",
     author_email="shenmishajing@gmail.com",
     url="https://github.com/shenmishajing/speed_benchmark",
     project_urls={
```

### Comparing `speed-benchmark-1.0.2/speed_benchmark/speed_benchmark.py` & `speed-benchmark-1.0.3/speed_benchmark/speed_benchmark.py`

 * *Files 0% similar despite different names*

```diff
@@ -82,15 +82,15 @@
     experiment_name=None,
     save_json=True,
     save_table=True,
     draw=True,
 ):
     if isinstance(funcs, list):
         funcs = {f.__name__: f for f in funcs}
-    elif isinstance(funcs, dict):
+    elif not isinstance(funcs, dict):
         funcs = {funcs.__name__: funcs}
 
     if not isinstance(args["data"], dict):
         args["data"] = {d[args["main_arg_name"]]: d for d in args["data"]}
 
     for k in args["data"]:
         if isinstance(args["data"][k], tuple | list):
```

### Comparing `speed-benchmark-1.0.2/speed_benchmark/visualization/line_chart.py` & `speed-benchmark-1.0.3/speed_benchmark/visualization/line_chart.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     save_path=None,
 ):
     if std_data is not None:
         assert upper_data is None and lower_data is None
         upper_data = data + std_data
         lower_data = data - std_data
 
-    colors = ncolors(len(data))
+    colors = ncolors(len(list(data)))
 
     for i, name in enumerate(data):
         plt.plot(data.index, data[name], color=colors[i], label=name, linewidth=3.5)
         if upper_data is not None and lower_data is not None:
             plt.fill_between(
                 data.index,
                 upper_data[name],
```

### Comparing `speed-benchmark-1.0.2/speed_benchmark.egg-info/PKG-INFO` & `speed-benchmark-1.0.3/speed_benchmark.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: speed-benchmark
-Version: 1.0.2
+Version: 1.0.3
 Summary: A generic speed benchmark library.
 Home-page: https://github.com/shenmishajing/speed_benchmark
 Author: shenmishajing
 Author-email: shenmishajing@gmail.com
 License: MIT License
 Project-URL: Code, https://github.com/shenmishajing/speed_benchmark
 Project-URL: Issue tracker, https://github.com/shenmishajing/speed_benchmark/issues
```

