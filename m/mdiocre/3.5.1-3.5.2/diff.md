# Comparing `tmp/mdiocre-3.5.1.tar.gz` & `tmp/mdiocre-3.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mdiocre-3.5.1.tar", last modified: Tue Oct 18 12:18:18 2022, max compression
+gzip compressed data, was "mdiocre-3.5.2.tar", last modified: Sun Jul  2 10:11:48 2023, max compression
```

## Comparing `mdiocre-3.5.1.tar` & `mdiocre-3.5.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0 zumid     (1000) zumid     (1000)        0 2022-10-18 12:18:18.653551 mdiocre-3.5.1/
--rwxrwxrwx   0 zumid     (1000) zumid     (1000)     1060 2022-06-27 06:46:23.000000 mdiocre-3.5.1/LICENSE
--rwxrwxrwx   0 zumid     (1000) zumid     (1000)      128 2022-06-27 06:46:23.000000 mdiocre-3.5.1/MANIFEST.in
--rwxrwxrwx   0 zumid     (1000) zumid     (1000)     3411 2022-10-18 12:18:18.653348 mdiocre-3.5.1/PKG-INFO
--rwxrwxrwx   0 zumid     (1000) zumid     (1000)     2589 2022-06-27 06:46:23.000000 mdiocre-3.5.1/README.md
--rwxrwxrwx   0 zumid     (1000) zumid     (1000)        6 2022-10-18 12:17:27.000000 mdiocre-3.5.1/RELEASE-VERSION
-drwxrwxrwx   0 zumid     (1000) zumid     (1000)        0 2022-10-18 12:18:18.647432 mdiocre-3.5.1/mdiocre/
--rwxrwxrwx   0 zumid     (1000) zumid     (1000)      885 2022-06-29 11:48:02.000000 mdiocre-3.5.1/mdiocre/__init__.py
--rwxrwxrwx   0 zumid     (1000) zumid     (1000)       87 2022-10-18 12:10:45.000000 mdiocre-3.5.1/mdiocre/__meta__.py
--rwxrwxrwx   0 zumid     (1000) zumid     (1000)    12990 2022-10-18 12:17:20.000000 mdiocre-3.5.1/mdiocre/core.py
-drwxrwxrwx   0 zumid     (1000) zumid     (1000)        0 2022-10-18 12:18:18.650577 mdiocre-3.5.1/mdiocre/interface/
--rwxrwxrwx   0 zumid     (1000) zumid     (1000)     2024 2022-06-29 11:23:39.000000 mdiocre-3.5.1/mdiocre/interface/cli.py
--rwxrwxrwx   0 zumid     (1000) zumid     (1000)     7385 2022-06-27 06:46:23.000000 mdiocre-3.5.1/mdiocre/interface/gui.py
-drwxrwxrwx   0 zumid     (1000) zumid     (1000)        0 2022-10-18 12:18:18.652817 mdiocre-3.5.1/mdiocre/parsers/
--rwxrwxrwx   0 zumid     (1000) zumid     (1000)     1321 2022-06-27 06:46:23.000000 mdiocre-3.5.1/mdiocre/parsers/__init__.py
--rwxrwxrwx   0 zumid     (1000) zumid     (1000)     3775 2022-06-29 09:03:17.000000 mdiocre-3.5.1/mdiocre/parsers/gem.py
--rwxrwxrwx   0 zumid     (1000) zumid     (1000)      480 2022-06-29 08:49:31.000000 mdiocre-3.5.1/mdiocre/parsers/html.py
--rwxrwxrwx   0 zumid     (1000) zumid     (1000)      674 2022-06-29 08:49:00.000000 mdiocre-3.5.1/mdiocre/parsers/markdown.py
--rwxrwxrwx   0 zumid     (1000) zumid     (1000)     2361 2022-06-29 08:49:18.000000 mdiocre-3.5.1/mdiocre/parsers/rst.py
--rwxrwxrwx   0 zumid     (1000) zumid     (1000)     4706 2022-10-18 12:09:30.000000 mdiocre-3.5.1/mdiocre/parsers/zim.py
--rwxrwxrwx   0 zumid     (1000) zumid     (1000)     1400 2022-06-27 06:46:23.000000 mdiocre-3.5.1/mdiocre/utils.py
--rwxrwxrwx   0 zumid     (1000) zumid     (1000)    11832 2022-06-29 12:12:35.000000 mdiocre-3.5.1/mdiocre/wizard.py
-drwxrwxrwx   0 zumid     (1000) zumid     (1000)        0 2022-10-18 12:18:18.649676 mdiocre-3.5.1/mdiocre.egg-info/
--rwxrwxrwx   0 zumid     (1000) zumid     (1000)     3411 2022-10-18 12:18:18.000000 mdiocre-3.5.1/mdiocre.egg-info/PKG-INFO
--rwxrwxrwx   0 zumid     (1000) zumid     (1000)      546 2022-10-18 12:18:18.000000 mdiocre-3.5.1/mdiocre.egg-info/SOURCES.txt
--rwxrwxrwx   0 zumid     (1000) zumid     (1000)        1 2022-10-18 12:18:18.000000 mdiocre-3.5.1/mdiocre.egg-info/dependency_links.txt
--rwxrwxrwx   0 zumid     (1000) zumid     (1000)       54 2022-10-18 12:18:18.000000 mdiocre-3.5.1/mdiocre.egg-info/entry_points.txt
--rwxrwxrwx   0 zumid     (1000) zumid     (1000)       16 2022-10-18 12:18:18.000000 mdiocre-3.5.1/mdiocre.egg-info/requires.txt
--rwxrwxrwx   0 zumid     (1000) zumid     (1000)        8 2022-10-18 12:18:18.000000 mdiocre-3.5.1/mdiocre.egg-info/top_level.txt
--rwxrwxrwx   0 zumid     (1000) zumid     (1000)       38 2022-10-18 12:18:18.653616 mdiocre-3.5.1/setup.cfg
--rwxrwxrwx   0 zumid     (1000) zumid     (1000)     1292 2022-06-27 06:46:23.000000 mdiocre-3.5.1/setup.py
--rwxrwxrwx   0 zumid     (1000) zumid     (1000)     2872 2022-06-27 06:46:23.000000 mdiocre-3.5.1/versioning.py
+drwxrwxrwx   0 zumid     (1000) shared-drive  (1001)        0 2023-07-02 10:11:48.459704 mdiocre-3.5.2/
+-rwxrwxrwx   0 zumid     (1000) shared-drive  (1001)     1060 2022-06-27 06:46:23.000000 mdiocre-3.5.2/LICENSE
+-rwxrwxrwx   0 zumid     (1000) shared-drive  (1001)      128 2022-06-27 06:46:23.000000 mdiocre-3.5.2/MANIFEST.in
+-rwxrwxrwx   0 zumid     (1000) shared-drive  (1001)     3411 2023-07-02 10:11:48.459470 mdiocre-3.5.2/PKG-INFO
+-rwxrwxrwx   0 zumid     (1000) shared-drive  (1001)     2589 2022-06-27 06:46:23.000000 mdiocre-3.5.2/README.md
+-rwxrwxrwx   0 zumid     (1000) shared-drive  (1001)        6 2023-07-02 10:11:03.000000 mdiocre-3.5.2/RELEASE-VERSION
+drwxrwxrwx   0 zumid     (1000) shared-drive  (1001)        0 2023-07-02 10:11:48.452147 mdiocre-3.5.2/mdiocre/
+-rwxrwxrwx   0 zumid     (1000) shared-drive  (1001)      885 2022-06-29 11:48:02.000000 mdiocre-3.5.2/mdiocre/__init__.py
+-rwxrwxrwx   0 zumid     (1000) shared-drive  (1001)       87 2023-07-02 10:05:44.000000 mdiocre-3.5.2/mdiocre/__meta__.py
+-rwxrwxrwx   0 zumid     (1000) shared-drive  (1001)    12990 2023-07-02 10:10:59.000000 mdiocre-3.5.2/mdiocre/core.py
+drwxrwxrwx   0 zumid     (1000) shared-drive  (1001)        0 2023-07-02 10:11:48.455935 mdiocre-3.5.2/mdiocre/interface/
+-rwxrwxrwx   0 zumid     (1000) shared-drive  (1001)     2024 2022-06-29 11:23:39.000000 mdiocre-3.5.2/mdiocre/interface/cli.py
+-rwxrwxrwx   0 zumid     (1000) shared-drive  (1001)     7385 2022-06-27 06:46:23.000000 mdiocre-3.5.2/mdiocre/interface/gui.py
+drwxrwxrwx   0 zumid     (1000) shared-drive  (1001)        0 2023-07-02 10:11:48.458953 mdiocre-3.5.2/mdiocre/parsers/
+-rwxrwxrwx   0 zumid     (1000) shared-drive  (1001)     1321 2022-06-27 06:46:23.000000 mdiocre-3.5.2/mdiocre/parsers/__init__.py
+-rwxrwxrwx   0 zumid     (1000) shared-drive  (1001)     3775 2022-06-29 09:03:17.000000 mdiocre-3.5.2/mdiocre/parsers/gem.py
+-rwxrwxrwx   0 zumid     (1000) shared-drive  (1001)      480 2022-06-29 08:49:31.000000 mdiocre-3.5.2/mdiocre/parsers/html.py
+-rwxrwxrwx   0 zumid     (1000) shared-drive  (1001)      674 2022-06-29 08:49:00.000000 mdiocre-3.5.2/mdiocre/parsers/markdown.py
+-rwxrwxrwx   0 zumid     (1000) shared-drive  (1001)     2361 2022-06-29 08:49:18.000000 mdiocre-3.5.2/mdiocre/parsers/rst.py
+-rwxrwxrwx   0 zumid     (1000) shared-drive  (1001)     4706 2022-10-18 12:09:30.000000 mdiocre-3.5.2/mdiocre/parsers/zim.py
+-rwxrwxrwx   0 zumid     (1000) shared-drive  (1001)     1400 2022-06-27 06:46:23.000000 mdiocre-3.5.2/mdiocre/utils.py
+-rwxrwxrwx   0 zumid     (1000) shared-drive  (1001)    11978 2023-07-02 10:04:22.000000 mdiocre-3.5.2/mdiocre/wizard.py
+drwxrwxrwx   0 zumid     (1000) shared-drive  (1001)        0 2023-07-02 10:11:48.454922 mdiocre-3.5.2/mdiocre.egg-info/
+-rwxrwxrwx   0 zumid     (1000) shared-drive  (1001)     3411 2023-07-02 10:11:48.000000 mdiocre-3.5.2/mdiocre.egg-info/PKG-INFO
+-rwxrwxrwx   0 zumid     (1000) shared-drive  (1001)      546 2023-07-02 10:11:48.000000 mdiocre-3.5.2/mdiocre.egg-info/SOURCES.txt
+-rwxrwxrwx   0 zumid     (1000) shared-drive  (1001)        1 2023-07-02 10:11:48.000000 mdiocre-3.5.2/mdiocre.egg-info/dependency_links.txt
+-rwxrwxrwx   0 zumid     (1000) shared-drive  (1001)       54 2023-07-02 10:11:48.000000 mdiocre-3.5.2/mdiocre.egg-info/entry_points.txt
+-rwxrwxrwx   0 zumid     (1000) shared-drive  (1001)       16 2023-07-02 10:11:48.000000 mdiocre-3.5.2/mdiocre.egg-info/requires.txt
+-rwxrwxrwx   0 zumid     (1000) shared-drive  (1001)        8 2023-07-02 10:11:48.000000 mdiocre-3.5.2/mdiocre.egg-info/top_level.txt
+-rwxrwxrwx   0 zumid     (1000) shared-drive  (1001)       38 2023-07-02 10:11:48.459769 mdiocre-3.5.2/setup.cfg
+-rwxrwxrwx   0 zumid     (1000) shared-drive  (1001)     1292 2022-06-27 06:46:23.000000 mdiocre-3.5.2/setup.py
+-rwxrwxrwx   0 zumid     (1000) shared-drive  (1001)     2872 2022-06-27 06:46:23.000000 mdiocre-3.5.2/versioning.py
```

### Comparing `mdiocre-3.5.1/LICENSE` & `mdiocre-3.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mdiocre-3.5.1/PKG-INFO` & `mdiocre-3.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mdiocre
-Version: 3.5.1
+Version: 3.5.2
 Summary: Static website generator
 Home-page: https://zumi.neocities.org/stuff/mdiocre
 Author: Zumi Daxuya
 Author-email: daxuya.zumi+mdiocre@protonmail.com
 License: MIT
 Keywords: converter,generator,markdown,html,static
 Classifier: Development Status :: 4 - Beta
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mdiocre Version: 3.5.1 Summary: Static website
+Metadata-Version: 2.1 Name: mdiocre Version: 3.5.2 Summary: Static website
 generator Home-page: https://zumi.neocities.org/stuff/mdiocre Author: Zumi
 Daxuya Author-email: daxuya.zumi+mdiocre@protonmail.com License: MIT Keywords:
 converter,generator,markdown,html,static Classifier: Development Status :: 4 -
 Beta Classifier: Intended Audience :: Developers Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Classifier: Natural Language :: English Classifier: Programming Language ::
 Python Classifier: Programming Language :: Python :: 3 Classifier: Programming
```

### Comparing `mdiocre-3.5.1/README.md` & `mdiocre-3.5.2/README.md`

 * *Files identical despite different names*

### Comparing `mdiocre-3.5.1/mdiocre/__init__.py` & `mdiocre-3.5.2/mdiocre/__init__.py`

 * *Files identical despite different names*

### Comparing `mdiocre-3.5.1/mdiocre/core.py` & `mdiocre-3.5.2/mdiocre/core.py`

 * *Files identical despite different names*

### Comparing `mdiocre-3.5.1/mdiocre/interface/cli.py` & `mdiocre-3.5.2/mdiocre/interface/cli.py`

 * *Files identical despite different names*

### Comparing `mdiocre-3.5.1/mdiocre/interface/gui.py` & `mdiocre-3.5.2/mdiocre/interface/gui.py`

 * *Files identical despite different names*

### Comparing `mdiocre-3.5.1/mdiocre/parsers/__init__.py` & `mdiocre-3.5.2/mdiocre/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `mdiocre-3.5.1/mdiocre/parsers/gem.py` & `mdiocre-3.5.2/mdiocre/parsers/gem.py`

 * *Files identical despite different names*

### Comparing `mdiocre-3.5.1/mdiocre/parsers/markdown.py` & `mdiocre-3.5.2/mdiocre/parsers/markdown.py`

 * *Files identical despite different names*

### Comparing `mdiocre-3.5.1/mdiocre/parsers/rst.py` & `mdiocre-3.5.2/mdiocre/parsers/rst.py`

 * *Files identical despite different names*

### Comparing `mdiocre-3.5.1/mdiocre/parsers/zim.py` & `mdiocre-3.5.2/mdiocre/parsers/zim.py`

 * *Files identical despite different names*

### Comparing `mdiocre-3.5.1/mdiocre/utils.py` & `mdiocre-3.5.2/mdiocre/utils.py`

 * *Files identical despite different names*

### Comparing `mdiocre-3.5.1/mdiocre/wizard.py` & `mdiocre-3.5.2/mdiocre/wizard.py`

 * *Files 2% similar despite different names*

```diff
@@ -273,15 +273,20 @@
 				try:
 					ts2js_result = subprocess.check_output(
 						['tsc', '--strict', '--outFile', built_file, source_file],
 						stderr = subprocess.STDOUT
 					)
 				
 				except FileNotFoundError as e:
-					logger.log(log_error + level, "can't find tsc on your system")
+					logger.log(log_error + level, "can't find tsc on your system, copying instead")
+					built_file = os.path.extsep.join([built_name, built_ext])
+					shutil.copyfile(
+						source_file,
+						built_file
+						)
 				
 				except subprocess.CalledProcessError as e:
 					logger.log(log_error + level, "compilation failed with code {}".format(e.returncode))
 					logger.log(log_error + level + 1, "{}".format(e.output.decode("utf-8")))
 					
 					# delete the compiled file just in case tsc compiles it anyway
 					if os.path.isfile(built_file):
```

### Comparing `mdiocre-3.5.1/mdiocre.egg-info/PKG-INFO` & `mdiocre-3.5.2/mdiocre.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mdiocre
-Version: 3.5.1
+Version: 3.5.2
 Summary: Static website generator
 Home-page: https://zumi.neocities.org/stuff/mdiocre
 Author: Zumi Daxuya
 Author-email: daxuya.zumi+mdiocre@protonmail.com
 License: MIT
 Keywords: converter,generator,markdown,html,static
 Classifier: Development Status :: 4 - Beta
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mdiocre Version: 3.5.1 Summary: Static website
+Metadata-Version: 2.1 Name: mdiocre Version: 3.5.2 Summary: Static website
 generator Home-page: https://zumi.neocities.org/stuff/mdiocre Author: Zumi
 Daxuya Author-email: daxuya.zumi+mdiocre@protonmail.com License: MIT Keywords:
 converter,generator,markdown,html,static Classifier: Development Status :: 4 -
 Beta Classifier: Intended Audience :: Developers Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Classifier: Natural Language :: English Classifier: Programming Language ::
 Python Classifier: Programming Language :: Python :: 3 Classifier: Programming
```

### Comparing `mdiocre-3.5.1/mdiocre.egg-info/SOURCES.txt` & `mdiocre-3.5.2/mdiocre.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mdiocre-3.5.1/setup.py` & `mdiocre-3.5.2/setup.py`

 * *Files identical despite different names*

### Comparing `mdiocre-3.5.1/versioning.py` & `mdiocre-3.5.2/versioning.py`

 * *Files identical despite different names*

