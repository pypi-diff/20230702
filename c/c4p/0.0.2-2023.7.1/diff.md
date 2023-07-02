# Comparing `tmp/c4p-0.0.2.tar.gz` & `tmp/c4p-2023.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "c4p-0.0.2.tar", last modified: Thu Jun  1 05:25:59 2023, max compression
+gzip compressed data, was "c4p-2023.7.1.tar", last modified: Sun Jul  2 04:25:58 2023, max compression
```

## Comparing `c4p-0.0.2.tar` & `c4p-2023.7.1.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 fengzhu  (40317) ncar      (1000)        0 2023-06-01 05:25:59.121749 c4p-0.0.2/
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)     1065 2023-05-22 19:27:41.000000 c4p-0.0.2/LICENSE
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)      510 2023-06-01 05:25:59.121309 c4p-0.0.2/PKG-INFO
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)       66 2023-05-31 23:29:16.000000 c4p-0.0.2/README.md
-drwxr-xr-x   0 fengzhu  (40317) ncar      (1000)        0 2023-06-01 05:25:59.117048 c4p-0.0.2/c4p/
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)      240 2023-06-01 04:08:45.000000 c4p-0.0.2/c4p/__init__.py
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)     5920 2023-06-01 05:24:39.000000 c4p-0.0.2/c4p/case.py
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)     1576 2023-06-01 04:11:06.000000 c4p-0.0.2/c4p/utils.py
-drwxr-xr-x   0 fengzhu  (40317) ncar      (1000)        0 2023-06-01 05:25:59.120715 c4p-0.0.2/c4p.egg-info/
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)      510 2023-06-01 05:25:58.000000 c4p-0.0.2/c4p.egg-info/PKG-INFO
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)      227 2023-06-01 05:25:58.000000 c4p-0.0.2/c4p.egg-info/SOURCES.txt
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)        1 2023-06-01 05:25:58.000000 c4p-0.0.2/c4p.egg-info/dependency_links.txt
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)        1 2023-06-01 04:07:36.000000 c4p-0.0.2/c4p.egg-info/not-zip-safe
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)       47 2023-06-01 05:25:58.000000 c4p-0.0.2/c4p.egg-info/requires.txt
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)        4 2023-06-01 05:25:58.000000 c4p-0.0.2/c4p.egg-info/top_level.txt
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)       38 2023-06-01 05:25:59.121878 c4p-0.0.2/setup.cfg
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)      877 2023-06-01 05:16:11.000000 c4p-0.0.2/setup.py
+drwxr-xr-x   0 fengzhu  (40317) ncar      (1000)        0 2023-07-02 04:25:58.919653 c4p-2023.7.1/
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)     1065 2023-05-22 19:27:41.000000 c4p-2023.7.1/LICENSE
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)      541 2023-07-02 04:25:58.918940 c4p-2023.7.1/PKG-INFO
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)       94 2023-07-02 04:04:59.000000 c4p-2023.7.1/README.md
+drwxr-xr-x   0 fengzhu  (40317) ncar      (1000)        0 2023-07-02 04:25:58.913683 c4p-2023.7.1/c4p/
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)      240 2023-06-01 04:08:45.000000 c4p-2023.7.1/c4p/__init__.py
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)     1074 2023-07-02 04:08:18.000000 c4p-2023.7.1/c4p/case.py
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)     7925 2023-07-02 04:13:46.000000 c4p-2023.7.1/c4p/runoff.py
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)     1718 2023-07-02 02:31:49.000000 c4p-2023.7.1/c4p/utils.py
+drwxr-xr-x   0 fengzhu  (40317) ncar      (1000)        0 2023-07-02 04:25:58.918122 c4p-2023.7.1/c4p.egg-info/
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)      541 2023-07-02 04:25:58.914490 c4p-2023.7.1/c4p.egg-info/PKG-INFO
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)      241 2023-07-02 04:25:58.915197 c4p-2023.7.1/c4p.egg-info/SOURCES.txt
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)        1 2023-07-02 04:25:58.915862 c4p-2023.7.1/c4p.egg-info/dependency_links.txt
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)        1 2023-06-01 04:07:36.000000 c4p-2023.7.1/c4p.egg-info/not-zip-safe
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)       47 2023-07-02 04:25:58.917504 c4p-2023.7.1/c4p.egg-info/requires.txt
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)        4 2023-07-02 04:25:58.918227 c4p-2023.7.1/c4p.egg-info/top_level.txt
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)       38 2023-07-02 04:25:58.919775 c4p-2023.7.1/setup.cfg
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)      880 2023-07-02 03:43:35.000000 c4p-2023.7.1/setup.py
```

### Comparing `c4p-0.0.2/LICENSE` & `c4p-2023.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `c4p-0.0.2/c4p/utils.py` & `c4p-2023.7.1/c4p/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+import shutil
 import subprocess
 import colorama as ca
 from tqdm import tqdm
 
 
 def p_header(text):
     print(ca.Fore.CYAN + ca.Style.BRIGHT + text)
@@ -49,13 +50,20 @@
     if fpath is None:
         fpath = os.path.basename(url)
 
     if os.path.exists(fpath): os.remove(fpath)
     run_shell(f'svn export {url} {fpath}')
     return fpath
 
+def copy(src, dst=None):
+    if dst is None:
+        dst = os.path.basename(src)
+
+    shutil.copyfile(src, dst)
+    return dst
+
 def exec_script(fpath, args=None, timeout=None):
     run_shell(f'chmod +x {fpath}')
     if args is None:
         run_shell(f'./{fpath}', timeout=timeout)
     else:
         run_shell(f'./{fpath} {args}', timeout=timeout)
```

### Comparing `c4p-0.0.2/setup.py` & `c4p-2023.7.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setup(
     name='c4p',  # required
-    version='0.0.2',
+    version='2023.7.1',
     description='c4p: CESM for Paleo',
     long_description=long_description,
     long_description_content_type='text/x-rst',
     author='Feng Zhu, Jiang Zhu',
     author_email='fengzhu@ucar.edu, jiangzhu@ucar.edu',
     url='https://github.com/fzhu2e/cesm4paleo',
     packages=find_packages(),
```

