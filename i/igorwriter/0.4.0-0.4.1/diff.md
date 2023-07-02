# Comparing `tmp/igorwriter-0.4.0.tar.gz` & `tmp/igorwriter-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "igorwriter-0.4.0.tar", last modified: Sat Jul  1 17:44:56 2023, max compression
+gzip compressed data, was "igorwriter-0.4.1.tar", last modified: Sun Jul  2 02:51:43 2023, max compression
```

## Comparing `igorwriter-0.4.0.tar` & `igorwriter-0.4.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-07-01 17:44:56.121068 igorwriter-0.4.0/
--rw-rw-rw-   0        0        0     1062 2019-11-16 04:29:14.000000 igorwriter-0.4.0/LICENSE.txt
--rw-rw-rw-   0        0        0     3594 2023-07-01 17:44:56.121068 igorwriter-0.4.0/PKG-INFO
--rw-rw-rw-   0        0        0     3121 2019-11-16 05:32:31.000000 igorwriter-0.4.0/README.rst
-drwxrwxrwx   0        0        0        0 2023-07-01 17:44:56.096041 igorwriter-0.4.0/igorwriter/
--rw-rw-rw-   0        0        0       53 2023-07-01 17:36:50.000000 igorwriter-0.4.0/igorwriter/__init__.py
--rw-rw-rw-   0        0        0      433 2019-11-16 04:29:14.000000 igorwriter-0.4.0/igorwriter/builtin_names.py
-drwxrwxrwx   0        0        0        0 2023-07-01 17:44:56.106042 igorwriter-0.4.0/igorwriter/builtins/
--rw-rw-rw-   0        0        0     5805 2019-11-16 04:29:14.000000 igorwriter-0.4.0/igorwriter/builtins/functions.txt
--rw-rw-rw-   0        0        0      104 2019-11-16 04:29:14.000000 igorwriter-0.4.0/igorwriter/builtins/keywords.txt
--rw-rw-rw-   0        0        0     6175 2019-11-16 04:29:14.000000 igorwriter-0.4.0/igorwriter/builtins/operations.txt
--rw-rw-rw-   0        0        0      213 2023-07-01 17:22:58.000000 igorwriter-0.4.0/igorwriter/errors.py
--rw-rw-rw-   0        0        0    18287 2023-07-01 17:36:50.000000 igorwriter-0.4.0/igorwriter/igorwave.py
--rw-rw-rw-   0        0        0     1511 2019-11-16 05:32:31.000000 igorwriter-0.4.0/igorwriter/utils.py
--rw-rw-rw-   0        0        0     2807 2023-07-01 17:22:58.000000 igorwriter-0.4.0/igorwriter/validator.py
-drwxrwxrwx   0        0        0        0 2023-07-01 17:44:56.104042 igorwriter-0.4.0/igorwriter.egg-info/
--rw-rw-rw-   0        0        0     3594 2023-07-01 17:44:56.000000 igorwriter-0.4.0/igorwriter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      510 2023-07-01 17:44:56.000000 igorwriter-0.4.0/igorwriter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-01 17:44:56.000000 igorwriter-0.4.0/igorwriter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-07-01 17:44:56.000000 igorwriter-0.4.0/igorwriter.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-01 17:44:56.000000 igorwriter-0.4.0/igorwriter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       74 2023-07-01 17:44:56.125067 igorwriter-0.4.0/setup.cfg
--rw-rw-rw-   0        0        0     1278 2023-07-01 17:38:27.000000 igorwriter-0.4.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-01 17:44:56.120068 igorwriter-0.4.0/tests/
--rw-rw-rw-   0        0        0     4191 2023-07-01 17:22:58.000000 igorwriter-0.4.0/tests/test_names.py
--rw-rw-rw-   0        0        0     1256 2019-11-16 04:29:14.000000 igorwriter-0.4.0/tests/test_utils.py
--rw-rw-rw-   0        0        0    12984 2023-07-01 17:36:50.000000 igorwriter-0.4.0/tests/test_wave.py
+drwxrwxrwx   0        0        0        0 2023-07-02 02:51:43.976578 igorwriter-0.4.1/
+-rw-rw-rw-   0        0        0     1062 2019-11-16 04:29:14.000000 igorwriter-0.4.1/LICENSE.txt
+-rw-rw-rw-   0        0        0     4816 2023-07-02 02:51:43.976578 igorwriter-0.4.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4307 2023-07-02 02:51:23.000000 igorwriter-0.4.1/README.rst
+drwxrwxrwx   0        0        0        0 2023-07-02 02:51:43.964584 igorwriter-0.4.1/igorwriter/
+-rw-rw-rw-   0        0        0       53 2023-07-01 17:36:50.000000 igorwriter-0.4.1/igorwriter/__init__.py
+-rw-rw-rw-   0        0        0      433 2019-11-16 04:29:14.000000 igorwriter-0.4.1/igorwriter/builtin_names.py
+drwxrwxrwx   0        0        0        0 2023-07-02 02:51:43.973584 igorwriter-0.4.1/igorwriter/builtins/
+-rw-rw-rw-   0        0        0     5805 2019-11-16 04:29:14.000000 igorwriter-0.4.1/igorwriter/builtins/functions.txt
+-rw-rw-rw-   0        0        0      104 2019-11-16 04:29:14.000000 igorwriter-0.4.1/igorwriter/builtins/keywords.txt
+-rw-rw-rw-   0        0        0     6175 2019-11-16 04:29:14.000000 igorwriter-0.4.1/igorwriter/builtins/operations.txt
+-rw-rw-rw-   0        0        0      213 2023-07-01 17:22:58.000000 igorwriter-0.4.1/igorwriter/errors.py
+-rw-rw-rw-   0        0        0    18287 2023-07-01 17:36:50.000000 igorwriter-0.4.1/igorwriter/igorwave.py
+-rw-rw-rw-   0        0        0     1511 2019-11-16 05:32:31.000000 igorwriter-0.4.1/igorwriter/utils.py
+-rw-rw-rw-   0        0        0     2807 2023-07-01 17:22:58.000000 igorwriter-0.4.1/igorwriter/validator.py
+drwxrwxrwx   0        0        0        0 2023-07-02 02:51:43.970590 igorwriter-0.4.1/igorwriter.egg-info/
+-rw-rw-rw-   0        0        0     4816 2023-07-02 02:51:43.000000 igorwriter-0.4.1/igorwriter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      510 2023-07-02 02:51:43.000000 igorwriter-0.4.1/igorwriter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-02 02:51:43.000000 igorwriter-0.4.1/igorwriter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-07-02 02:51:43.000000 igorwriter-0.4.1/igorwriter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-02 02:51:43.000000 igorwriter-0.4.1/igorwriter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       74 2023-07-02 02:51:43.980579 igorwriter-0.4.1/setup.cfg
+-rw-rw-rw-   0        0        0     1278 2023-07-02 02:51:23.000000 igorwriter-0.4.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-02 02:51:43.975587 igorwriter-0.4.1/tests/
+-rw-rw-rw-   0        0        0     4191 2023-07-01 17:22:58.000000 igorwriter-0.4.1/tests/test_names.py
+-rw-rw-rw-   0        0        0     1256 2019-11-16 04:29:14.000000 igorwriter-0.4.1/tests/test_utils.py
+-rw-rw-rw-   0        0        0    12984 2023-07-01 17:36:50.000000 igorwriter-0.4.1/tests/test_wave.py
```

### Comparing `igorwriter-0.4.0/LICENSE.txt` & `igorwriter-0.4.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `igorwriter-0.4.0/igorwriter/builtins/functions.txt` & `igorwriter-0.4.1/igorwriter/builtins/functions.txt`

 * *Files identical despite different names*

### Comparing `igorwriter-0.4.0/igorwriter/builtins/operations.txt` & `igorwriter-0.4.1/igorwriter/builtins/operations.txt`

 * *Files identical despite different names*

### Comparing `igorwriter-0.4.0/igorwriter/igorwave.py` & `igorwriter-0.4.1/igorwriter/igorwave.py`

 * *Files identical despite different names*

### Comparing `igorwriter-0.4.0/igorwriter/utils.py` & `igorwriter-0.4.1/igorwriter/utils.py`

 * *Files identical despite different names*

### Comparing `igorwriter-0.4.0/igorwriter/validator.py` & `igorwriter-0.4.1/igorwriter/validator.py`

 * *Files identical despite different names*

### Comparing `igorwriter-0.4.0/setup.py` & `igorwriter-0.4.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 # Get the long description from the README file
 with open(path.join(here, 'README.rst'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='igorwriter',
-    version='0.4.0',
+    version='0.4.1',
     description='Write IGOR binary (.ibw) or text (.itx) files from numpy array',
     long_description=long_description,
     url='https://github.com/t-onoz/igorwriter',
     author='t-onoz',
     license='MIT',
     classifiers=[
         # How mature is this project? Common values are
```

### Comparing `igorwriter-0.4.0/tests/test_names.py` & `igorwriter-0.4.1/tests/test_names.py`

 * *Files identical despite different names*

### Comparing `igorwriter-0.4.0/tests/test_utils.py` & `igorwriter-0.4.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `igorwriter-0.4.0/tests/test_wave.py` & `igorwriter-0.4.1/tests/test_wave.py`

 * *Files identical despite different names*

