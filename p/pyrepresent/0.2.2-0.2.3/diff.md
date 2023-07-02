# Comparing `tmp/pyrepresent-0.2.2.tar.gz` & `tmp/pyrepresent-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrepresent-0.2.2.tar", last modified: Sun Jul  2 16:45:02 2023, max compression
+gzip compressed data, was "pyrepresent-0.2.3.tar", last modified: Sun Jul  2 16:53:41 2023, max compression
```

## Comparing `pyrepresent-0.2.2.tar` & `pyrepresent-0.2.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-02 16:45:02.224856 pyrepresent-0.2.2/
--rw-rw-rw-   0        0        0      115 2023-07-02 16:45:01.000000 pyrepresent-0.2.2/MANIFEST.in
--rw-rw-rw-   0        0        0     2548 2023-07-02 16:45:02.223848 pyrepresent-0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     1669 2023-07-01 08:58:26.000000 pyrepresent-0.2.2/README.md
--rw-rw-rw-   0        0        0    12920 2023-03-17 11:12:17.000000 pyrepresent-0.2.2/build.py
--rw-rw-rw-   0        0        0      715 2023-07-02 16:45:01.000000 pyrepresent-0.2.2/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-07-02 16:45:02.219946 pyrepresent-0.2.2/pyrepresent.egg-info/
--rw-rw-rw-   0        0        0     2548 2023-07-02 16:45:02.000000 pyrepresent-0.2.2/pyrepresent.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      385 2023-07-02 16:45:02.000000 pyrepresent-0.2.2/pyrepresent.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-02 16:45:02.000000 pyrepresent-0.2.2/pyrepresent.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2023-07-02 16:45:02.000000 pyrepresent-0.2.2/pyrepresent.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-02 16:45:02.000000 pyrepresent-0.2.2/pyrepresent.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-02 16:45:02.223848 pyrepresent-0.2.2/represent/
--rw-rw-rw-   0        0        0      178 2023-07-02 15:44:48.000000 pyrepresent-0.2.2/represent/__init__.py
--rw-rw-rw-   0        0        0     8718 2023-07-02 15:44:34.000000 pyrepresent-0.2.2/represent/colors.py
--rw-rw-rw-   0        0        0     2133 2023-05-15 13:38:04.000000 pyrepresent-0.2.2/represent/indentation.py
--rw-rw-rw-   0        0        0    14681 2023-07-02 16:44:39.000000 pyrepresent-0.2.2/represent/object.py
--rw-rw-rw-   0        0        0    14396 2023-07-02 16:43:30.000000 pyrepresent-0.2.2/represent/structures.py
--rw-rw-rw-   0        0        0       30 2023-03-28 10:51:56.000000 pyrepresent-0.2.2/requirements-dev.txt
--rw-rw-rw-   0        0        0       21 2023-03-28 10:51:53.000000 pyrepresent-0.2.2/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-02 16:45:02.224856 pyrepresent-0.2.2/setup.cfg
--rw-rw-rw-   0        0        0     1682 2023-07-02 16:45:00.000000 pyrepresent-0.2.2/setup.py
--rw-rw-rw-   0        0        0     1361 2023-07-02 15:56:18.000000 pyrepresent-0.2.2/test.py
+drwxrwxrwx   0        0        0        0 2023-07-02 16:53:41.513990 pyrepresent-0.2.3/
+-rw-rw-rw-   0        0        0      115 2023-07-02 16:53:41.000000 pyrepresent-0.2.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     2548 2023-07-02 16:53:41.512977 pyrepresent-0.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1669 2023-07-01 08:58:26.000000 pyrepresent-0.2.3/README.md
+-rw-rw-rw-   0        0        0    12920 2023-03-17 11:12:17.000000 pyrepresent-0.2.3/build.py
+-rw-rw-rw-   0        0        0      715 2023-07-02 16:53:41.000000 pyrepresent-0.2.3/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-07-02 16:53:41.507994 pyrepresent-0.2.3/pyrepresent.egg-info/
+-rw-rw-rw-   0        0        0     2548 2023-07-02 16:53:41.000000 pyrepresent-0.2.3/pyrepresent.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      385 2023-07-02 16:53:41.000000 pyrepresent-0.2.3/pyrepresent.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-02 16:53:41.000000 pyrepresent-0.2.3/pyrepresent.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2023-07-02 16:53:41.000000 pyrepresent-0.2.3/pyrepresent.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-02 16:53:41.000000 pyrepresent-0.2.3/pyrepresent.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-02 16:53:41.511977 pyrepresent-0.2.3/represent/
+-rw-rw-rw-   0        0        0      178 2023-07-02 15:44:48.000000 pyrepresent-0.2.3/represent/__init__.py
+-rw-rw-rw-   0        0        0     8718 2023-07-02 15:44:34.000000 pyrepresent-0.2.3/represent/colors.py
+-rw-rw-rw-   0        0        0     2133 2023-05-15 13:38:04.000000 pyrepresent-0.2.3/represent/indentation.py
+-rw-rw-rw-   0        0        0    14704 2023-07-02 16:53:32.000000 pyrepresent-0.2.3/represent/object.py
+-rw-rw-rw-   0        0        0    14396 2023-07-02 16:43:30.000000 pyrepresent-0.2.3/represent/structures.py
+-rw-rw-rw-   0        0        0       30 2023-03-28 10:51:56.000000 pyrepresent-0.2.3/requirements-dev.txt
+-rw-rw-rw-   0        0        0       21 2023-03-28 10:51:53.000000 pyrepresent-0.2.3/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-02 16:53:41.513990 pyrepresent-0.2.3/setup.cfg
+-rw-rw-rw-   0        0        0     1682 2023-07-02 16:53:38.000000 pyrepresent-0.2.3/setup.py
+-rw-rw-rw-   0        0        0     1361 2023-07-02 15:56:18.000000 pyrepresent-0.2.3/test.py
```

### Comparing `pyrepresent-0.2.2/PKG-INFO` & `pyrepresent-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrepresent
-Version: 0.2.2
+Version: 0.2.3
 Summary: A module for object and model representations as strings, with vast configurations, colors, hidden and protected values, assignment operations, memory addresses and more.
 Home-page: https://github.com/Shahaf-F-S/represent
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyrepresent-0.2.2/README.md` & `pyrepresent-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `pyrepresent-0.2.2/build.py` & `pyrepresent-0.2.3/build.py`

 * *Files identical despite different names*

### Comparing `pyrepresent-0.2.2/pyproject.toml` & `pyrepresent-0.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'pyrepresent'
-version = '0.2.2'
+version = '0.2.3'
 description = 'A module for object and model representations as strings, with vast configurations, colors, hidden and protected values, assignment operations, memory addresses and more.'
 classifiers = [
 	'Intended Audience :: Developers',
 	'License :: OSI Approved :: MIT License',
 	'Programming Language :: Python',
 	'Programming Language :: Python :: 3',
 	'Programming Language :: Python :: 3.8',
```

### Comparing `pyrepresent-0.2.2/pyrepresent.egg-info/PKG-INFO` & `pyrepresent-0.2.3/pyrepresent.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrepresent
-Version: 0.2.2
+Version: 0.2.3
 Summary: A module for object and model representations as strings, with vast configurations, colors, hidden and protected values, assignment operations, memory addresses and more.
 Home-page: https://github.com/Shahaf-F-S/represent
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyrepresent-0.2.2/represent/colors.py` & `pyrepresent-0.2.3/represent/colors.py`

 * *Files identical despite different names*

### Comparing `pyrepresent-0.2.2/represent/indentation.py` & `pyrepresent-0.2.3/represent/indentation.py`

 * *Files identical despite different names*

### Comparing `pyrepresent-0.2.2/represent/object.py` & `pyrepresent-0.2.3/represent/object.py`

 * *Files 1% similar despite different names*

```diff
@@ -151,15 +151,15 @@
 
     :return: The properties of the object.
     """
 
     return {
         **extract_attributes(data),
         **(
-            extract_properties(data)
+            extract_properties(data, properties=properties)
             if properties else {}
         )
     }
 # end extract_data
 
 def is_protected(
         key: Any,
```

### Comparing `pyrepresent-0.2.2/represent/structures.py` & `pyrepresent-0.2.3/represent/structures.py`

 * *Files identical despite different names*

### Comparing `pyrepresent-0.2.2/setup.py` & `pyrepresent-0.2.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         ],
         include=[
             "test.py"
         ],
         requirements="requirements.txt",
         dev_requirements="requirements-dev.txt",
         name='pyrepresent',
-        version='0.2.2',
+        version='0.2.3',
         description=(
             "A module for object and model representations as strings, "
             "with vast configurations, colors, hidden and protected values, "
             "assignment operations, memory addresses and more."
         ),
         license='MIT',
         author="Shahaf Frank-Shapir",
```

### Comparing `pyrepresent-0.2.2/test.py` & `pyrepresent-0.2.3/test.py`

 * *Files identical despite different names*

