# Comparing `tmp/julienne-0.8.0.tar.gz` & `tmp/julienne-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "julienne-0.8.0.tar", last modified: Mon May 22 14:52:43 2023, max compression
+gzip compressed data, was "julienne-0.8.1.tar", last modified: Sun Jul  2 17:09:23 2023, max compression
```

## Comparing `julienne-0.8.0.tar` & `julienne-0.8.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 ctrudeau   (501) staff       (20)        0 2023-05-22 14:52:43.800991 julienne-0.8.0/
--rw-r--r--   0 ctrudeau   (501) staff       (20)     1076 2022-10-24 19:55:49.000000 julienne-0.8.0/LICENSE
--rw-r--r--   0 ctrudeau   (501) staff       (20)    11947 2023-05-22 14:52:43.801135 julienne-0.8.0/PKG-INFO
--rw-r--r--   0 ctrudeau   (501) staff       (20)    11087 2023-05-22 14:47:13.000000 julienne-0.8.0/README.rst
--rw-r--r--   0 ctrudeau   (501) staff       (20)       90 2022-10-24 20:30:47.000000 julienne-0.8.0/pyproject.toml
--rw-r--r--   0 ctrudeau   (501) staff       (20)     1220 2023-05-22 14:52:43.801977 julienne-0.8.0/setup.cfg
-drwxr-xr-x   0 ctrudeau   (501) staff       (20)        0 2023-05-22 14:52:43.695540 julienne-0.8.0/src/
-drwxr-xr-x   0 ctrudeau   (501) staff       (20)        0 2023-05-22 14:52:43.796324 julienne-0.8.0/src/julienne/
--rw-r--r--   0 ctrudeau   (501) staff       (20)       22 2023-05-22 14:38:20.000000 julienne-0.8.0/src/julienne/__init__.py
--rw-r--r--   0 ctrudeau   (501) staff       (20)     1897 2023-03-17 20:26:54.000000 julienne-0.8.0/src/julienne/cmd.py
--rw-r--r--   0 ctrudeau   (501) staff       (20)    11708 2023-03-17 21:00:23.000000 julienne-0.8.0/src/julienne/filemodel.py
--rw-r--r--   0 ctrudeau   (501) staff       (20)     6862 2023-03-17 20:27:23.000000 julienne-0.8.0/src/julienne/nodes.py
--rw-r--r--   0 ctrudeau   (501) staff       (20)    13488 2023-05-22 14:47:51.000000 julienne-0.8.0/src/julienne/parsers.py
-drwxr-xr-x   0 ctrudeau   (501) staff       (20)        0 2023-05-22 14:52:43.799358 julienne-0.8.0/src/julienne.egg-info/
--rw-r--r--   0 ctrudeau   (501) staff       (20)    11947 2023-05-22 14:52:43.000000 julienne-0.8.0/src/julienne.egg-info/PKG-INFO
--rw-r--r--   0 ctrudeau   (501) staff       (20)      442 2023-05-22 14:52:43.000000 julienne-0.8.0/src/julienne.egg-info/SOURCES.txt
--rw-r--r--   0 ctrudeau   (501) staff       (20)        1 2023-05-22 14:52:43.000000 julienne-0.8.0/src/julienne.egg-info/dependency_links.txt
--rw-r--r--   0 ctrudeau   (501) staff       (20)       43 2023-05-22 14:52:43.000000 julienne-0.8.0/src/julienne.egg-info/entry_points.txt
--rw-r--r--   0 ctrudeau   (501) staff       (20)      136 2023-05-22 14:52:43.000000 julienne-0.8.0/src/julienne.egg-info/requires.txt
--rw-r--r--   0 ctrudeau   (501) staff       (20)        9 2023-05-22 14:52:43.000000 julienne-0.8.0/src/julienne.egg-info/top_level.txt
-drwxr-xr-x   0 ctrudeau   (501) staff       (20)        0 2023-05-22 14:52:43.800625 julienne-0.8.0/tests/
--rw-r--r--   0 ctrudeau   (501) staff       (20)     2523 2023-03-17 19:24:24.000000 julienne-0.8.0/tests/test_files.py
--rw-r--r--   0 ctrudeau   (501) staff       (20)     5466 2023-05-22 14:48:15.000000 julienne-0.8.0/tests/test_pparser.py
--rw-r--r--   0 ctrudeau   (501) staff       (20)     5218 2023-05-22 14:49:19.000000 julienne-0.8.0/tests/test_xparser.py
+drwxr-xr-x   0 ctrudeau   (501) staff       (20)        0 2023-07-02 17:09:23.924195 julienne-0.8.1/
+-rw-r--r--   0 ctrudeau   (501) staff       (20)     1076 2022-10-24 19:55:49.000000 julienne-0.8.1/LICENSE
+-rw-r--r--   0 ctrudeau   (501) staff       (20)    11947 2023-07-02 17:09:23.924369 julienne-0.8.1/PKG-INFO
+-rw-r--r--   0 ctrudeau   (501) staff       (20)    11087 2023-05-22 14:47:13.000000 julienne-0.8.1/README.rst
+-rw-r--r--   0 ctrudeau   (501) staff       (20)       90 2022-10-24 20:30:47.000000 julienne-0.8.1/pyproject.toml
+-rw-r--r--   0 ctrudeau   (501) staff       (20)     1232 2023-07-02 17:09:23.925295 julienne-0.8.1/setup.cfg
+drwxr-xr-x   0 ctrudeau   (501) staff       (20)        0 2023-07-02 17:09:23.886136 julienne-0.8.1/src/
+drwxr-xr-x   0 ctrudeau   (501) staff       (20)        0 2023-07-02 17:09:23.920543 julienne-0.8.1/src/julienne/
+-rw-r--r--   0 ctrudeau   (501) staff       (20)       22 2023-07-02 17:06:07.000000 julienne-0.8.1/src/julienne/__init__.py
+-rw-r--r--   0 ctrudeau   (501) staff       (20)     1897 2023-03-17 20:26:54.000000 julienne-0.8.1/src/julienne/cmd.py
+-rw-r--r--   0 ctrudeau   (501) staff       (20)    12086 2023-07-02 17:05:55.000000 julienne-0.8.1/src/julienne/filemodel.py
+-rw-r--r--   0 ctrudeau   (501) staff       (20)     6862 2023-03-17 20:27:23.000000 julienne-0.8.1/src/julienne/nodes.py
+-rw-r--r--   0 ctrudeau   (501) staff       (20)    13488 2023-05-22 14:47:51.000000 julienne-0.8.1/src/julienne/parsers.py
+drwxr-xr-x   0 ctrudeau   (501) staff       (20)        0 2023-07-02 17:09:23.922836 julienne-0.8.1/src/julienne.egg-info/
+-rw-r--r--   0 ctrudeau   (501) staff       (20)    11947 2023-07-02 17:09:23.000000 julienne-0.8.1/src/julienne.egg-info/PKG-INFO
+-rw-r--r--   0 ctrudeau   (501) staff       (20)      442 2023-07-02 17:09:23.000000 julienne-0.8.1/src/julienne.egg-info/SOURCES.txt
+-rw-r--r--   0 ctrudeau   (501) staff       (20)        1 2023-07-02 17:09:23.000000 julienne-0.8.1/src/julienne.egg-info/dependency_links.txt
+-rw-r--r--   0 ctrudeau   (501) staff       (20)       43 2023-07-02 17:09:23.000000 julienne-0.8.1/src/julienne.egg-info/entry_points.txt
+-rw-r--r--   0 ctrudeau   (501) staff       (20)      150 2023-07-02 17:09:23.000000 julienne-0.8.1/src/julienne.egg-info/requires.txt
+-rw-r--r--   0 ctrudeau   (501) staff       (20)        9 2023-07-02 17:09:23.000000 julienne-0.8.1/src/julienne.egg-info/top_level.txt
+drwxr-xr-x   0 ctrudeau   (501) staff       (20)        0 2023-07-02 17:09:23.923914 julienne-0.8.1/tests/
+-rw-r--r--   0 ctrudeau   (501) staff       (20)     2523 2023-03-17 19:24:24.000000 julienne-0.8.1/tests/test_files.py
+-rw-r--r--   0 ctrudeau   (501) staff       (20)     5466 2023-05-22 14:48:15.000000 julienne-0.8.1/tests/test_pparser.py
+-rw-r--r--   0 ctrudeau   (501) staff       (20)     5218 2023-05-22 14:49:19.000000 julienne-0.8.1/tests/test_xparser.py
```

### Comparing `julienne-0.8.0/LICENSE` & `julienne-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `julienne-0.8.0/PKG-INFO` & `julienne-0.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: julienne
-Version: 0.8.0
+Version: 0.8.1
 Summary: Splits code into copies based on version numbers in comments
 Home-page: https://github.com/cltrudeau/julienne
 Author: Christopher Trudeau
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
```

### Comparing `julienne-0.8.0/README.rst` & `julienne-0.8.1/README.rst`

 * *Files identical despite different names*

### Comparing `julienne-0.8.0/setup.cfg` & `julienne-0.8.1/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 	Programming Language :: Python :: 3.11
 	Topic :: Software Development :: Code Generators
 	Topic :: Software Development :: Libraries :: Python Modules
 
 [options]
 install_requires = 
 	black==23.1.0
+	isort==5.12.0
 	tomli==2.0.1
 
 [options.extras_require]
 dev = 
 	build==0.8.0
 	coverage==6.5.0
 	pudb==2022.1.2
@@ -38,15 +39,15 @@
 
 [options.entry_points]
 console_scripts = 
 	juli = julienne.cmd:main
 
 [tox:tox]
 isolated_build = True
-envlist = py{37,38,39,310,311}
+envlist = py{38,39,310,311}
 
 [testenv]
 commands = python -m unittest
 deps = .[dev]
 
 [egg_info]
 tag_build =
```

### Comparing `julienne-0.8.0/src/julienne/cmd.py` & `julienne-0.8.1/src/julienne/cmd.py`

 * *Files identical despite different names*

### Comparing `julienne-0.8.0/src/julienne/filemodel.py` & `julienne-0.8.1/src/julienne/filemodel.py`

 * *Files 4% similar despite different names*

```diff
@@ -285,14 +285,26 @@
         if output_dir.exists():
             shutil.rmtree(output_dir)
 
     if verbose:
         print('\n**Processing')
     tree.generate(output_dir, single_chapter)
 
+    # Optionally run isort on the output
+    if config.get('isort', False):
+        print('\n**Calling isort')
+        sys.argv = ['isrot', str(output_dir)]
+        try:
+            # import only if being used
+            from isort.main import main as isort_main
+            isort_main()
+        except SystemExit:
+            # black calls quit(), ignore it
+            pass
+
     # Optionally run black on the output
     if config.get('black', False):
         print('\n**Calling black')
         #sys.argv = ['black', str(output_dir), '-l', 80, '--diff']
         sys.argv = ['black', str(output_dir), '-l', 80]
         try:
             import black    # import only if being used
```

### Comparing `julienne-0.8.0/src/julienne/nodes.py` & `julienne-0.8.1/src/julienne/nodes.py`

 * *Files identical despite different names*

### Comparing `julienne-0.8.0/src/julienne/parsers.py` & `julienne-0.8.1/src/julienne/parsers.py`

 * *Files identical despite different names*

### Comparing `julienne-0.8.0/src/julienne.egg-info/PKG-INFO` & `julienne-0.8.1/src/julienne.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: julienne
-Version: 0.8.0
+Version: 0.8.1
 Summary: Splits code into copies based on version numbers in comments
 Home-page: https://github.com/cltrudeau/julienne
 Author: Christopher Trudeau
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
```

### Comparing `julienne-0.8.0/tests/test_files.py` & `julienne-0.8.1/tests/test_files.py`

 * *Files identical despite different names*

### Comparing `julienne-0.8.0/tests/test_pparser.py` & `julienne-0.8.1/tests/test_pparser.py`

 * *Files identical despite different names*

### Comparing `julienne-0.8.0/tests/test_xparser.py` & `julienne-0.8.1/tests/test_xparser.py`

 * *Files identical despite different names*

