# Comparing `tmp/pcsFilter-1.0.0.tar.gz` & `tmp/pcsFilter-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pcsFilter-1.0.0.tar", last modified: Thu Jan  5 19:29:38 2023, max compression
+gzip compressed data, was "pcsFilter-1.0.1.tar", last modified: Sun Jun  4 18:31:03 2023, max compression
```

## Comparing `pcsFilter-1.0.0.tar` & `pcsFilter-1.0.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 Alex       (501) staff       (20)        0 2023-01-05 19:29:38.580594 pcsFilter-1.0.0/
--rw-r--r--   0 Alex       (501) staff       (20)     1083 2022-12-31 15:53:01.000000 pcsFilter-1.0.0/LICENSE
--rw-r--r--   0 Alex       (501) staff       (20)     2695 2023-01-05 19:29:38.580046 pcsFilter-1.0.0/PKG-INFO
--rw-r--r--   0 Alex       (501) staff       (20)     1862 2023-01-05 19:19:25.000000 pcsFilter-1.0.0/README.md
-drwxr-xr-x   0 Alex       (501) staff       (20)        0 2023-01-05 19:29:38.551598 pcsFilter-1.0.0/pcsFilter.egg-info/
--rw-r--r--   0 Alex       (501) staff       (20)     2695 2023-01-05 19:29:38.000000 pcsFilter-1.0.0/pcsFilter.egg-info/PKG-INFO
--rw-r--r--   0 Alex       (501) staff       (20)      685 2023-01-05 19:29:38.000000 pcsFilter-1.0.0/pcsFilter.egg-info/SOURCES.txt
--rw-r--r--   0 Alex       (501) staff       (20)        1 2023-01-05 19:29:38.000000 pcsFilter-1.0.0/pcsFilter.egg-info/dependency_links.txt
--rw-r--r--   0 Alex       (501) staff       (20)       53 2023-01-05 19:29:38.000000 pcsFilter-1.0.0/pcsFilter.egg-info/entry_points.txt
--rw-r--r--   0 Alex       (501) staff       (20)       92 2023-01-05 19:29:38.000000 pcsFilter-1.0.0/pcsFilter.egg-info/requires.txt
--rw-r--r--   0 Alex       (501) staff       (20)        6 2023-01-05 19:29:38.000000 pcsFilter-1.0.0/pcsFilter.egg-info/top_level.txt
--rw-r--r--   0 Alex       (501) staff       (20)       38 2023-01-05 19:29:38.580754 pcsFilter-1.0.0/setup.cfg
--rw-r--r--   0 Alex       (501) staff       (20)     1392 2023-01-05 19:22:04.000000 pcsFilter-1.0.0/setup.py
-drwxr-xr-x   0 Alex       (501) staff       (20)        0 2023-01-05 19:29:38.552554 pcsFilter-1.0.0/tests/
--rw-r--r--   0 Alex       (501) staff       (20)        0 2023-01-02 11:06:28.000000 pcsFilter-1.0.0/tests/__init__.py
-drwxr-xr-x   0 Alex       (501) staff       (20)        0 2023-01-05 19:29:38.553276 pcsFilter-1.0.0/tests/pcsFilter/
--rw-r--r--   0 Alex       (501) staff       (20)        0 2023-01-02 11:06:23.000000 pcsFilter-1.0.0/tests/pcsFilter/__init__.py
-drwxr-xr-x   0 Alex       (501) staff       (20)        0 2023-01-05 19:29:38.557016 pcsFilter-1.0.0/tests/pcsFilter/e2e/
--rw-r--r--   0 Alex       (501) staff       (20)        0 2023-01-02 11:06:38.000000 pcsFilter-1.0.0/tests/pcsFilter/e2e/__init__.py
--rw-r--r--   0 Alex       (501) staff       (20)     1007 2022-12-31 15:53:01.000000 pcsFilter-1.0.0/tests/pcsFilter/e2e/test_pcsFilter_results.py
-drwxr-xr-x   0 Alex       (501) staff       (20)        0 2023-01-05 19:29:38.561536 pcsFilter-1.0.0/tests/pcsFilter/integration/
--rw-r--r--   0 Alex       (501) staff       (20)        0 2023-01-02 11:06:34.000000 pcsFilter-1.0.0/tests/pcsFilter/integration/__init__.py
--rw-r--r--   0 Alex       (501) staff       (20)      490 2022-12-31 15:53:01.000000 pcsFilter-1.0.0/tests/pcsFilter/integration/test_without_setup_cfg.py
-drwxr-xr-x   0 Alex       (501) staff       (20)        0 2023-01-05 19:29:38.579140 pcsFilter-1.0.0/tests/pcsFilter/unit/
--rw-r--r--   0 Alex       (501) staff       (20)        0 2022-12-31 15:53:01.000000 pcsFilter-1.0.0/tests/pcsFilter/unit/__init__.py
--rw-r--r--   0 Alex       (501) staff       (20)      502 2023-01-03 20:58:55.000000 pcsFilter-1.0.0/tests/pcsFilter/unit/fixtures.py
--rw-r--r--   0 Alex       (501) staff       (20)      534 2023-01-03 20:58:55.000000 pcsFilter-1.0.0/tests/pcsFilter/unit/test_black.py
--rw-r--r--   0 Alex       (501) staff       (20)      524 2023-01-03 20:58:55.000000 pcsFilter-1.0.0/tests/pcsFilter/unit/test_blue.py
--rw-r--r--   0 Alex       (501) staff       (20)      840 2023-01-03 20:58:55.000000 pcsFilter-1.0.0/tests/pcsFilter/unit/test_flake8.py
--rw-r--r--   0 Alex       (501) staff       (20)      559 2023-01-03 20:58:55.000000 pcsFilter-1.0.0/tests/pcsFilter/unit/test_isort.py
--rw-r--r--   0 Alex       (501) staff       (20)      655 2023-01-03 20:58:55.000000 pcsFilter-1.0.0/tests/pcsFilter/unit/test_radon.py
+drwxr-xr-x   0 Alex       (501) staff       (20)        0 2023-06-04 18:31:03.074835 pcsFilter-1.0.1/
+-rw-r--r--   0 Alex       (501) staff       (20)     1083 2022-12-31 15:53:01.000000 pcsFilter-1.0.1/LICENSE
+-rw-r--r--   0 Alex       (501) staff       (20)     2695 2023-06-04 18:31:03.073900 pcsFilter-1.0.1/PKG-INFO
+-rw-r--r--   0 Alex       (501) staff       (20)     1862 2023-01-05 19:35:16.000000 pcsFilter-1.0.1/README.md
+drwxr-xr-x   0 Alex       (501) staff       (20)        0 2023-06-04 18:31:03.057108 pcsFilter-1.0.1/pcsFilter.egg-info/
+-rw-r--r--   0 Alex       (501) staff       (20)     2695 2023-06-04 18:31:03.000000 pcsFilter-1.0.1/pcsFilter.egg-info/PKG-INFO
+-rw-r--r--   0 Alex       (501) staff       (20)      685 2023-06-04 18:31:03.000000 pcsFilter-1.0.1/pcsFilter.egg-info/SOURCES.txt
+-rw-r--r--   0 Alex       (501) staff       (20)        1 2023-06-04 18:31:03.000000 pcsFilter-1.0.1/pcsFilter.egg-info/dependency_links.txt
+-rw-r--r--   0 Alex       (501) staff       (20)       53 2023-06-04 18:31:03.000000 pcsFilter-1.0.1/pcsFilter.egg-info/entry_points.txt
+-rw-r--r--   0 Alex       (501) staff       (20)       92 2023-06-04 18:31:03.000000 pcsFilter-1.0.1/pcsFilter.egg-info/requires.txt
+-rw-r--r--   0 Alex       (501) staff       (20)        6 2023-06-04 18:31:03.000000 pcsFilter-1.0.1/pcsFilter.egg-info/top_level.txt
+-rw-r--r--   0 Alex       (501) staff       (20)       38 2023-06-04 18:31:03.075192 pcsFilter-1.0.1/setup.cfg
+-rw-r--r--   0 Alex       (501) staff       (20)     1392 2023-06-04 18:30:06.000000 pcsFilter-1.0.1/setup.py
+drwxr-xr-x   0 Alex       (501) staff       (20)        0 2023-06-04 18:31:03.059741 pcsFilter-1.0.1/tests/
+-rw-r--r--   0 Alex       (501) staff       (20)        0 2023-01-02 11:06:28.000000 pcsFilter-1.0.1/tests/__init__.py
+drwxr-xr-x   0 Alex       (501) staff       (20)        0 2023-06-04 18:31:03.060880 pcsFilter-1.0.1/tests/pcsFilter/
+-rw-r--r--   0 Alex       (501) staff       (20)        0 2023-01-02 11:06:23.000000 pcsFilter-1.0.1/tests/pcsFilter/__init__.py
+drwxr-xr-x   0 Alex       (501) staff       (20)        0 2023-06-04 18:31:03.062801 pcsFilter-1.0.1/tests/pcsFilter/e2e/
+-rw-r--r--   0 Alex       (501) staff       (20)        0 2023-01-02 11:06:38.000000 pcsFilter-1.0.1/tests/pcsFilter/e2e/__init__.py
+-rw-r--r--   0 Alex       (501) staff       (20)     1007 2022-12-31 15:53:01.000000 pcsFilter-1.0.1/tests/pcsFilter/e2e/test_pcsFilter_results.py
+drwxr-xr-x   0 Alex       (501) staff       (20)        0 2023-06-04 18:31:03.066276 pcsFilter-1.0.1/tests/pcsFilter/integration/
+-rw-r--r--   0 Alex       (501) staff       (20)        0 2023-01-02 11:06:34.000000 pcsFilter-1.0.1/tests/pcsFilter/integration/__init__.py
+-rw-r--r--   0 Alex       (501) staff       (20)      490 2022-12-31 15:53:01.000000 pcsFilter-1.0.1/tests/pcsFilter/integration/test_without_setup_cfg.py
+drwxr-xr-x   0 Alex       (501) staff       (20)        0 2023-06-04 18:31:03.072347 pcsFilter-1.0.1/tests/pcsFilter/unit/
+-rw-r--r--   0 Alex       (501) staff       (20)        0 2022-12-31 15:53:01.000000 pcsFilter-1.0.1/tests/pcsFilter/unit/__init__.py
+-rw-r--r--   0 Alex       (501) staff       (20)      502 2023-01-03 20:58:55.000000 pcsFilter-1.0.1/tests/pcsFilter/unit/fixtures.py
+-rw-r--r--   0 Alex       (501) staff       (20)      534 2023-01-03 20:58:55.000000 pcsFilter-1.0.1/tests/pcsFilter/unit/test_black.py
+-rw-r--r--   0 Alex       (501) staff       (20)      524 2023-01-03 20:58:55.000000 pcsFilter-1.0.1/tests/pcsFilter/unit/test_blue.py
+-rw-r--r--   0 Alex       (501) staff       (20)      840 2023-01-03 20:58:55.000000 pcsFilter-1.0.1/tests/pcsFilter/unit/test_flake8.py
+-rw-r--r--   0 Alex       (501) staff       (20)      559 2023-01-03 20:58:55.000000 pcsFilter-1.0.1/tests/pcsFilter/unit/test_isort.py
+-rw-r--r--   0 Alex       (501) staff       (20)      655 2023-01-03 20:58:55.000000 pcsFilter-1.0.1/tests/pcsFilter/unit/test_radon.py
```

### Comparing `pcsFilter-1.0.0/LICENSE` & `pcsFilter-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pcsFilter-1.0.0/PKG-INFO` & `pcsFilter-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pcsFilter
-Version: 1.0.0
+Version: 1.0.1
 Summary: Tool for filtering out Python Code Smells
 Home-page: https://github.com/alex-d-bondarev/pcsFilter
 Author: Sasha Bondarev
 Author-email: github.pcsfilter@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `pcsFilter-1.0.0/README.md` & `pcsFilter-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `pcsFilter-1.0.0/pcsFilter.egg-info/PKG-INFO` & `pcsFilter-1.0.1/pcsFilter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pcsFilter
-Version: 1.0.0
+Version: 1.0.1
 Summary: Tool for filtering out Python Code Smells
 Home-page: https://github.com/alex-d-bondarev/pcsFilter
 Author: Sasha Bondarev
 Author-email: github.pcsfilter@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `pcsFilter-1.0.0/pcsFilter.egg-info/SOURCES.txt` & `pcsFilter-1.0.1/pcsFilter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pcsFilter-1.0.0/setup.py` & `pcsFilter-1.0.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as readme:
     long_description = readme.read()
 
 setup(
     name="pcsFilter",
-    version="1.0.0",
+    version="1.0.1",
     python_requires=">=3.7",
     author="Sasha Bondarev",
     author_email="github.pcsfilter@gmail.com",
     license="MIT",
     description="Tool for filtering out Python Code Smells",
     long_description=long_description,
     long_description_content_type="text/markdown",
@@ -18,15 +18,15 @@
     include_package_data=True,
     install_requires=[
         "blue~=0.9.0",
         "click~=8.0.0",
         "ConfigUpdater~=3.0.0",
         "flake8>=3.8,<5.0.0",
         "isort~=5.10.0",
-        "radon~=5.1.0",
+        "radon~=6.0.1",
     ],
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
```

### Comparing `pcsFilter-1.0.0/tests/pcsFilter/e2e/test_pcsFilter_results.py` & `pcsFilter-1.0.1/tests/pcsFilter/e2e/test_pcsFilter_results.py`

 * *Files identical despite different names*

### Comparing `pcsFilter-1.0.0/tests/pcsFilter/unit/test_black.py` & `pcsFilter-1.0.1/tests/pcsFilter/unit/test_black.py`

 * *Files identical despite different names*

### Comparing `pcsFilter-1.0.0/tests/pcsFilter/unit/test_blue.py` & `pcsFilter-1.0.1/tests/pcsFilter/unit/test_blue.py`

 * *Files identical despite different names*

### Comparing `pcsFilter-1.0.0/tests/pcsFilter/unit/test_flake8.py` & `pcsFilter-1.0.1/tests/pcsFilter/unit/test_flake8.py`

 * *Files identical despite different names*

### Comparing `pcsFilter-1.0.0/tests/pcsFilter/unit/test_isort.py` & `pcsFilter-1.0.1/tests/pcsFilter/unit/test_isort.py`

 * *Files identical despite different names*

### Comparing `pcsFilter-1.0.0/tests/pcsFilter/unit/test_radon.py` & `pcsFilter-1.0.1/tests/pcsFilter/unit/test_radon.py`

 * *Files identical despite different names*

