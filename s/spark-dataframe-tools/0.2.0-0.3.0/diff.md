# Comparing `tmp/spark_dataframe_tools-0.2.0.tar.gz` & `tmp/spark_dataframe_tools-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spark_dataframe_tools-0.2.0.tar", last modified: Mon May 22 08:47:59 2023, max compression
+gzip compressed data, was "spark_dataframe_tools-0.3.0.tar", last modified: Sun Jul  2 08:59:34 2023, max compression
```

## Comparing `spark_dataframe_tools-0.2.0.tar` & `spark_dataframe_tools-0.3.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-05-22 08:47:59.838310 spark_dataframe_tools-0.2.0/
--rw-rw-rw-   0        0        0     1092 2022-12-01 18:37:15.000000 spark_dataframe_tools-0.2.0/LICENSE
--rw-rw-rw-   0        0        0       47 2023-05-22 08:45:59.000000 spark_dataframe_tools-0.2.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2747 2023-05-22 08:47:59.838310 spark_dataframe_tools-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     1975 2023-05-22 05:38:16.000000 spark_dataframe_tools-0.2.0/README.md
--rw-rw-rw-   0        0        0      631 2023-05-22 08:47:48.000000 spark_dataframe_tools-0.2.0/pyproject.toml
--rw-rw-rw-   0        0        0       86 2023-05-22 08:47:59.838310 spark_dataframe_tools-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1177 2023-05-22 08:47:48.000000 spark_dataframe_tools-0.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-22 08:47:59.822682 spark_dataframe_tools-0.2.0/spark_dataframe_tools/
--rw-rw-rw-   0        0        0      532 2023-05-22 05:03:16.000000 spark_dataframe_tools-0.2.0/spark_dataframe_tools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-22 08:47:59.838310 spark_dataframe_tools-0.2.0/spark_dataframe_tools/functions/
--rw-rw-rw-   0        0        0        0 2022-12-01 18:37:15.000000 spark_dataframe_tools-0.2.0/spark_dataframe_tools/functions/__init__.py
--rw-rw-rw-   0        0        0     3190 2023-05-22 05:14:31.000000 spark_dataframe_tools-0.2.0/spark_dataframe_tools/functions/generator.py
-drwxrwxrwx   0        0        0        0 2023-05-22 08:47:59.838310 spark_dataframe_tools-0.2.0/spark_dataframe_tools/utils/
--rw-rw-rw-   0        0        0       75 2022-12-01 18:37:15.000000 spark_dataframe_tools-0.2.0/spark_dataframe_tools/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-22 08:47:59.838310 spark_dataframe_tools-0.2.0/spark_dataframe_tools/utils/templates/
--rw-rw-rw-   0        0        0        0 2022-12-01 18:37:15.000000 spark_dataframe_tools-0.2.0/spark_dataframe_tools/utils/templates/__init__.py
--rw-rw-rw-   0        0        0     1861 2022-12-01 18:37:15.000000 spark_dataframe_tools-0.2.0/spark_dataframe_tools/utils/templates/table.html
-drwxrwxrwx   0        0        0        0 2023-05-22 08:47:59.838310 spark_dataframe_tools-0.2.0/spark_dataframe_tools.egg-info/
--rw-rw-rw-   0        0        0     2747 2023-05-22 08:47:59.000000 spark_dataframe_tools-0.2.0/spark_dataframe_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      549 2023-05-22 08:47:59.000000 spark_dataframe_tools-0.2.0/spark_dataframe_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-22 08:47:59.000000 spark_dataframe_tools-0.2.0/spark_dataframe_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      162 2023-05-22 08:47:59.000000 spark_dataframe_tools-0.2.0/spark_dataframe_tools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-05-22 08:47:59.000000 spark_dataframe_tools-0.2.0/spark_dataframe_tools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-02 08:59:34.591905 spark_dataframe_tools-0.3.0/
+-rw-rw-rw-   0        0        0     1092 2022-12-01 18:37:15.000000 spark_dataframe_tools-0.3.0/LICENSE
+-rw-rw-rw-   0        0        0       47 2023-05-22 08:45:59.000000 spark_dataframe_tools-0.3.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2747 2023-07-02 08:59:34.591905 spark_dataframe_tools-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1975 2023-05-22 05:38:16.000000 spark_dataframe_tools-0.3.0/README.md
+-rw-rw-rw-   0        0        0      631 2023-05-22 08:47:48.000000 spark_dataframe_tools-0.3.0/pyproject.toml
+-rw-rw-rw-   0        0        0       86 2023-07-02 08:59:34.591905 spark_dataframe_tools-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     1177 2023-07-02 08:59:17.000000 spark_dataframe_tools-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-02 08:59:34.560653 spark_dataframe_tools-0.3.0/spark_dataframe_tools/
+-rw-rw-rw-   0        0        0      803 2023-07-02 08:59:17.000000 spark_dataframe_tools-0.3.0/spark_dataframe_tools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-02 08:59:34.576279 spark_dataframe_tools-0.3.0/spark_dataframe_tools/functions/
+-rw-rw-rw-   0        0        0        0 2022-12-01 18:37:15.000000 spark_dataframe_tools-0.3.0/spark_dataframe_tools/functions/__init__.py
+-rw-rw-rw-   0        0        0     3190 2023-05-22 05:14:31.000000 spark_dataframe_tools-0.3.0/spark_dataframe_tools/functions/generator.py
+drwxrwxrwx   0        0        0        0 2023-07-02 08:59:34.576279 spark_dataframe_tools-0.3.0/spark_dataframe_tools/utils/
+-rw-rw-rw-   0        0        0       75 2022-12-01 18:37:15.000000 spark_dataframe_tools-0.3.0/spark_dataframe_tools/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-02 08:59:34.591905 spark_dataframe_tools-0.3.0/spark_dataframe_tools/utils/templates/
+-rw-rw-rw-   0        0        0        0 2022-12-01 18:37:15.000000 spark_dataframe_tools-0.3.0/spark_dataframe_tools/utils/templates/__init__.py
+-rw-rw-rw-   0        0        0     1861 2022-12-01 18:37:15.000000 spark_dataframe_tools-0.3.0/spark_dataframe_tools/utils/templates/table.html
+drwxrwxrwx   0        0        0        0 2023-07-02 08:59:34.576279 spark_dataframe_tools-0.3.0/spark_dataframe_tools.egg-info/
+-rw-rw-rw-   0        0        0     2747 2023-07-02 08:59:34.000000 spark_dataframe_tools-0.3.0/spark_dataframe_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      549 2023-07-02 08:59:34.000000 spark_dataframe_tools-0.3.0/spark_dataframe_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-02 08:59:34.000000 spark_dataframe_tools-0.3.0/spark_dataframe_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      162 2023-07-02 08:59:34.000000 spark_dataframe_tools-0.3.0/spark_dataframe_tools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-07-02 08:59:34.000000 spark_dataframe_tools-0.3.0/spark_dataframe_tools.egg-info/top_level.txt
```

### Comparing `spark_dataframe_tools-0.2.0/LICENSE` & `spark_dataframe_tools-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `spark_dataframe_tools-0.2.0/PKG-INFO` & `spark_dataframe_tools-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spark_dataframe_tools
-Version: 0.2.0
+Version: 0.3.0
 Summary: spark_dataframe_tools
 Home-page: https://github.com/jonaqp/spark_dataframe_tools/
 Author: Jonathan Quiza
 Author-email: jony327@gmail.com
 License: UNKNOWN
 Download-URL: https://github.com/jonaqp/spark_dataframe_tools/archive/main.zip
 Keywords: spark,dataframe
```

### Comparing `spark_dataframe_tools-0.2.0/README.md` & `spark_dataframe_tools-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `spark_dataframe_tools-0.2.0/pyproject.toml` & `spark_dataframe_tools-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `spark_dataframe_tools-0.2.0/setup.py` & `spark_dataframe_tools-0.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from setuptools import find_packages
 
 setuppath = os.path.dirname(os.path.abspath(__file__))
 
 setup(
     name='spark_dataframe_tools',
     packages=find_packages(),
-    version='0.2.0',
+    version='0.3.0',
     description='spark_dataframe_tools',
     long_description=open(os.path.join(setuppath, 'README.md')).read(),
     long_description_content_type="text/markdown",
     author='Jonathan Quiza',
     author_email='jony327@gmail.com',
     url='https://github.com/jonaqp/spark_dataframe_tools/',
     download_url='https://github.com/jonaqp/spark_dataframe_tools/archive/main.zip',
```

### Comparing `spark_dataframe_tools-0.2.0/spark_dataframe_tools/functions/generator.py` & `spark_dataframe_tools-0.3.0/spark_dataframe_tools/functions/generator.py`

 * *Files identical despite different names*

### Comparing `spark_dataframe_tools-0.2.0/spark_dataframe_tools/utils/templates/table.html` & `spark_dataframe_tools-0.3.0/spark_dataframe_tools/utils/templates/table.html`

 * *Files identical despite different names*

### Comparing `spark_dataframe_tools-0.2.0/spark_dataframe_tools.egg-info/PKG-INFO` & `spark_dataframe_tools-0.3.0/spark_dataframe_tools.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spark-dataframe-tools
-Version: 0.2.0
+Version: 0.3.0
 Summary: spark_dataframe_tools
 Home-page: https://github.com/jonaqp/spark_dataframe_tools/
 Author: Jonathan Quiza
 Author-email: jony327@gmail.com
 License: UNKNOWN
 Download-URL: https://github.com/jonaqp/spark_dataframe_tools/archive/main.zip
 Keywords: spark,dataframe
```

### Comparing `spark_dataframe_tools-0.2.0/spark_dataframe_tools.egg-info/SOURCES.txt` & `spark_dataframe_tools-0.3.0/spark_dataframe_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

