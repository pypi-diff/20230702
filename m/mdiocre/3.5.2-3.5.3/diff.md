# Comparing `tmp/mdiocre-3.5.2.tar.gz` & `tmp/mdiocre-3.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mdiocre-3.5.2.tar", last modified: Sun Jul  2 10:11:48 2023, max compression
+gzip compressed data, was "mdiocre-3.5.3.tar", last modified: Sun Jul  2 10:32:39 2023, max compression
```

## Comparing `mdiocre-3.5.2.tar` & `mdiocre-3.5.3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0 zumid     (1000) shared-drive  (1001)        0 2023-07-02 10:11:48.459704 mdiocre-3.5.2/
--rwxrwxrwx   0 zumid     (1000) shared-drive  (1001)     1060 2022-06-27 06:46:23.000000 mdiocre-3.5.2/LICENSE
--rwxrwxrwx   0 zumid     (1000) shared-drive  (1001)      128 2022-06-27 06:46:23.000000 mdiocre-3.5.2/MANIFEST.in
--rwxrwxrwx   0 zumid     (1000) shared-drive  (1001)     3411 2023-07-02 10:11:48.459470 mdiocre-3.5.2/PKG-INFO
--rwxrwxrwx   0 zumid     (1000) shared-drive  (1001)     2589 2022-06-27 06:46:23.000000 mdiocre-3.5.2/README.md
--rwxrwxrwx   0 zumid     (1000) shared-drive  (1001)        6 2023-07-02 10:11:03.000000 mdiocre-3.5.2/RELEASE-VERSION
-drwxrwxrwx   0 zumid     (1000) shared-drive  (1001)        0 2023-07-02 10:11:48.452147 mdiocre-3.5.2/mdiocre/
--rwxrwxrwx   0 zumid     (1000) shared-drive  (1001)      885 2022-06-29 11:48:02.000000 mdiocre-3.5.2/mdiocre/__init__.py
--rwxrwxrwx   0 zumid     (1000) shared-drive  (1001)       87 2023-07-02 10:05:44.000000 mdiocre-3.5.2/mdiocre/__meta__.py
--rwxrwxrwx   0 zumid     (1000) shared-drive  (1001)    12990 2023-07-02 10:10:59.000000 mdiocre-3.5.2/mdiocre/core.py
-drwxrwxrwx   0 zumid     (1000) shared-drive  (1001)        0 2023-07-02 10:11:48.455935 mdiocre-3.5.2/mdiocre/interface/
--rwxrwxrwx   0 zumid     (1000) shared-drive  (1001)     2024 2022-06-29 11:23:39.000000 mdiocre-3.5.2/mdiocre/interface/cli.py
--rwxrwxrwx   0 zumid     (1000) shared-drive  (1001)     7385 2022-06-27 06:46:23.000000 mdiocre-3.5.2/mdiocre/interface/gui.py
-drwxrwxrwx   0 zumid     (1000) shared-drive  (1001)        0 2023-07-02 10:11:48.458953 mdiocre-3.5.2/mdiocre/parsers/
--rwxrwxrwx   0 zumid     (1000) shared-drive  (1001)     1321 2022-06-27 06:46:23.000000 mdiocre-3.5.2/mdiocre/parsers/__init__.py
--rwxrwxrwx   0 zumid     (1000) shared-drive  (1001)     3775 2022-06-29 09:03:17.000000 mdiocre-3.5.2/mdiocre/parsers/gem.py
--rwxrwxrwx   0 zumid     (1000) shared-drive  (1001)      480 2022-06-29 08:49:31.000000 mdiocre-3.5.2/mdiocre/parsers/html.py
--rwxrwxrwx   0 zumid     (1000) shared-drive  (1001)      674 2022-06-29 08:49:00.000000 mdiocre-3.5.2/mdiocre/parsers/markdown.py
--rwxrwxrwx   0 zumid     (1000) shared-drive  (1001)     2361 2022-06-29 08:49:18.000000 mdiocre-3.5.2/mdiocre/parsers/rst.py
--rwxrwxrwx   0 zumid     (1000) shared-drive  (1001)     4706 2022-10-18 12:09:30.000000 mdiocre-3.5.2/mdiocre/parsers/zim.py
--rwxrwxrwx   0 zumid     (1000) shared-drive  (1001)     1400 2022-06-27 06:46:23.000000 mdiocre-3.5.2/mdiocre/utils.py
--rwxrwxrwx   0 zumid     (1000) shared-drive  (1001)    11978 2023-07-02 10:04:22.000000 mdiocre-3.5.2/mdiocre/wizard.py
-drwxrwxrwx   0 zumid     (1000) shared-drive  (1001)        0 2023-07-02 10:11:48.454922 mdiocre-3.5.2/mdiocre.egg-info/
--rwxrwxrwx   0 zumid     (1000) shared-drive  (1001)     3411 2023-07-02 10:11:48.000000 mdiocre-3.5.2/mdiocre.egg-info/PKG-INFO
--rwxrwxrwx   0 zumid     (1000) shared-drive  (1001)      546 2023-07-02 10:11:48.000000 mdiocre-3.5.2/mdiocre.egg-info/SOURCES.txt
--rwxrwxrwx   0 zumid     (1000) shared-drive  (1001)        1 2023-07-02 10:11:48.000000 mdiocre-3.5.2/mdiocre.egg-info/dependency_links.txt
--rwxrwxrwx   0 zumid     (1000) shared-drive  (1001)       54 2023-07-02 10:11:48.000000 mdiocre-3.5.2/mdiocre.egg-info/entry_points.txt
--rwxrwxrwx   0 zumid     (1000) shared-drive  (1001)       16 2023-07-02 10:11:48.000000 mdiocre-3.5.2/mdiocre.egg-info/requires.txt
--rwxrwxrwx   0 zumid     (1000) shared-drive  (1001)        8 2023-07-02 10:11:48.000000 mdiocre-3.5.2/mdiocre.egg-info/top_level.txt
--rwxrwxrwx   0 zumid     (1000) shared-drive  (1001)       38 2023-07-02 10:11:48.459769 mdiocre-3.5.2/setup.cfg
--rwxrwxrwx   0 zumid     (1000) shared-drive  (1001)     1292 2022-06-27 06:46:23.000000 mdiocre-3.5.2/setup.py
--rwxrwxrwx   0 zumid     (1000) shared-drive  (1001)     2872 2022-06-27 06:46:23.000000 mdiocre-3.5.2/versioning.py
+drwxrwxrwx   0 zumid     (1000) shared-drive  (1001)        0 2023-07-02 10:32:39.818898 mdiocre-3.5.3/
+-rwxrwxrwx   0 zumid     (1000) shared-drive  (1001)     1060 2022-06-27 06:46:23.000000 mdiocre-3.5.3/LICENSE
+-rwxrwxrwx   0 zumid     (1000) shared-drive  (1001)      128 2022-06-27 06:46:23.000000 mdiocre-3.5.3/MANIFEST.in
+-rwxrwxrwx   0 zumid     (1000) shared-drive  (1001)     3411 2023-07-02 10:32:39.818475 mdiocre-3.5.3/PKG-INFO
+-rwxrwxrwx   0 zumid     (1000) shared-drive  (1001)     2589 2022-06-27 06:46:23.000000 mdiocre-3.5.3/README.md
+-rwxrwxrwx   0 zumid     (1000) shared-drive  (1001)        6 2023-07-02 10:32:39.000000 mdiocre-3.5.3/RELEASE-VERSION
+drwxrwxrwx   0 zumid     (1000) shared-drive  (1001)        0 2023-07-02 10:32:39.810797 mdiocre-3.5.3/mdiocre/
+-rwxrwxrwx   0 zumid     (1000) shared-drive  (1001)      885 2022-06-29 11:48:02.000000 mdiocre-3.5.3/mdiocre/__init__.py
+-rwxrwxrwx   0 zumid     (1000) shared-drive  (1001)       87 2023-07-02 10:29:50.000000 mdiocre-3.5.3/mdiocre/__meta__.py
+-rwxrwxrwx   0 zumid     (1000) shared-drive  (1001)    12990 2023-07-02 10:10:59.000000 mdiocre-3.5.3/mdiocre/core.py
+drwxrwxrwx   0 zumid     (1000) shared-drive  (1001)        0 2023-07-02 10:32:39.814772 mdiocre-3.5.3/mdiocre/interface/
+-rwxrwxrwx   0 zumid     (1000) shared-drive  (1001)     2024 2022-06-29 11:23:39.000000 mdiocre-3.5.3/mdiocre/interface/cli.py
+-rwxrwxrwx   0 zumid     (1000) shared-drive  (1001)     7385 2022-06-27 06:46:23.000000 mdiocre-3.5.3/mdiocre/interface/gui.py
+drwxrwxrwx   0 zumid     (1000) shared-drive  (1001)        0 2023-07-02 10:32:39.817912 mdiocre-3.5.3/mdiocre/parsers/
+-rwxrwxrwx   0 zumid     (1000) shared-drive  (1001)     1321 2022-06-27 06:46:23.000000 mdiocre-3.5.3/mdiocre/parsers/__init__.py
+-rwxrwxrwx   0 zumid     (1000) shared-drive  (1001)     3775 2022-06-29 09:03:17.000000 mdiocre-3.5.3/mdiocre/parsers/gem.py
+-rwxrwxrwx   0 zumid     (1000) shared-drive  (1001)      480 2022-06-29 08:49:31.000000 mdiocre-3.5.3/mdiocre/parsers/html.py
+-rwxrwxrwx   0 zumid     (1000) shared-drive  (1001)      674 2022-06-29 08:49:00.000000 mdiocre-3.5.3/mdiocre/parsers/markdown.py
+-rwxrwxrwx   0 zumid     (1000) shared-drive  (1001)     2361 2022-06-29 08:49:18.000000 mdiocre-3.5.3/mdiocre/parsers/rst.py
+-rwxrwxrwx   0 zumid     (1000) shared-drive  (1001)     4706 2022-10-18 12:09:30.000000 mdiocre-3.5.3/mdiocre/parsers/zim.py
+-rwxrwxrwx   0 zumid     (1000) shared-drive  (1001)     1400 2022-06-27 06:46:23.000000 mdiocre-3.5.3/mdiocre/utils.py
+-rwxrwxrwx   0 zumid     (1000) shared-drive  (1001)    11973 2023-07-02 10:29:42.000000 mdiocre-3.5.3/mdiocre/wizard.py
+drwxrwxrwx   0 zumid     (1000) shared-drive  (1001)        0 2023-07-02 10:32:39.813686 mdiocre-3.5.3/mdiocre.egg-info/
+-rwxrwxrwx   0 zumid     (1000) shared-drive  (1001)     3411 2023-07-02 10:32:39.000000 mdiocre-3.5.3/mdiocre.egg-info/PKG-INFO
+-rwxrwxrwx   0 zumid     (1000) shared-drive  (1001)      546 2023-07-02 10:32:39.000000 mdiocre-3.5.3/mdiocre.egg-info/SOURCES.txt
+-rwxrwxrwx   0 zumid     (1000) shared-drive  (1001)        1 2023-07-02 10:32:39.000000 mdiocre-3.5.3/mdiocre.egg-info/dependency_links.txt
+-rwxrwxrwx   0 zumid     (1000) shared-drive  (1001)       54 2023-07-02 10:32:39.000000 mdiocre-3.5.3/mdiocre.egg-info/entry_points.txt
+-rwxrwxrwx   0 zumid     (1000) shared-drive  (1001)       16 2023-07-02 10:32:39.000000 mdiocre-3.5.3/mdiocre.egg-info/requires.txt
+-rwxrwxrwx   0 zumid     (1000) shared-drive  (1001)        8 2023-07-02 10:32:39.000000 mdiocre-3.5.3/mdiocre.egg-info/top_level.txt
+-rwxrwxrwx   0 zumid     (1000) shared-drive  (1001)       38 2023-07-02 10:32:39.818960 mdiocre-3.5.3/setup.cfg
+-rwxrwxrwx   0 zumid     (1000) shared-drive  (1001)     1292 2022-06-27 06:46:23.000000 mdiocre-3.5.3/setup.py
+-rwxrwxrwx   0 zumid     (1000) shared-drive  (1001)     2872 2022-06-27 06:46:23.000000 mdiocre-3.5.3/versioning.py
```

### Comparing `mdiocre-3.5.2/LICENSE` & `mdiocre-3.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mdiocre-3.5.2/PKG-INFO` & `mdiocre-3.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mdiocre
-Version: 3.5.2
+Version: 3.5.3
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
-Metadata-Version: 2.1 Name: mdiocre Version: 3.5.2 Summary: Static website
+Metadata-Version: 2.1 Name: mdiocre Version: 3.5.3 Summary: Static website
 generator Home-page: https://zumi.neocities.org/stuff/mdiocre Author: Zumi
 Daxuya Author-email: daxuya.zumi+mdiocre@protonmail.com License: MIT Keywords:
 converter,generator,markdown,html,static Classifier: Development Status :: 4 -
 Beta Classifier: Intended Audience :: Developers Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Classifier: Natural Language :: English Classifier: Programming Language ::
 Python Classifier: Programming Language :: Python :: 3 Classifier: Programming
```

### Comparing `mdiocre-3.5.2/README.md` & `mdiocre-3.5.3/README.md`

 * *Files identical despite different names*

### Comparing `mdiocre-3.5.2/mdiocre/__init__.py` & `mdiocre-3.5.3/mdiocre/__init__.py`

 * *Files identical despite different names*

### Comparing `mdiocre-3.5.2/mdiocre/core.py` & `mdiocre-3.5.3/mdiocre/core.py`

 * *Files identical despite different names*

### Comparing `mdiocre-3.5.2/mdiocre/interface/cli.py` & `mdiocre-3.5.3/mdiocre/interface/cli.py`

 * *Files identical despite different names*

### Comparing `mdiocre-3.5.2/mdiocre/interface/gui.py` & `mdiocre-3.5.3/mdiocre/interface/gui.py`

 * *Files identical despite different names*

### Comparing `mdiocre-3.5.2/mdiocre/parsers/__init__.py` & `mdiocre-3.5.3/mdiocre/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `mdiocre-3.5.2/mdiocre/parsers/gem.py` & `mdiocre-3.5.3/mdiocre/parsers/gem.py`

 * *Files identical despite different names*

### Comparing `mdiocre-3.5.2/mdiocre/parsers/markdown.py` & `mdiocre-3.5.3/mdiocre/parsers/markdown.py`

 * *Files identical despite different names*

### Comparing `mdiocre-3.5.2/mdiocre/parsers/rst.py` & `mdiocre-3.5.3/mdiocre/parsers/rst.py`

 * *Files identical despite different names*

### Comparing `mdiocre-3.5.2/mdiocre/parsers/zim.py` & `mdiocre-3.5.3/mdiocre/parsers/zim.py`

 * *Files identical despite different names*

### Comparing `mdiocre-3.5.2/mdiocre/utils.py` & `mdiocre-3.5.3/mdiocre/utils.py`

 * *Files identical despite different names*

### Comparing `mdiocre-3.5.2/mdiocre/wizard.py` & `mdiocre-3.5.3/mdiocre/wizard.py`

 * *Files 0% similar despite different names*

```diff
@@ -274,15 +274,15 @@
 					ts2js_result = subprocess.check_output(
 						['tsc', '--strict', '--outFile', built_file, source_file],
 						stderr = subprocess.STDOUT
 					)
 				
 				except FileNotFoundError as e:
 					logger.log(log_error + level, "can't find tsc on your system, copying instead")
-					built_file = os.path.extsep.join([built_name, built_ext])
+					built_file = os.path.extsep.join([built_name, 'ts'])
 					shutil.copyfile(
 						source_file,
 						built_file
 						)
 				
 				except subprocess.CalledProcessError as e:
 					logger.log(log_error + level, "compilation failed with code {}".format(e.returncode))
```

### Comparing `mdiocre-3.5.2/mdiocre.egg-info/PKG-INFO` & `mdiocre-3.5.3/mdiocre.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mdiocre
-Version: 3.5.2
+Version: 3.5.3
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
-Metadata-Version: 2.1 Name: mdiocre Version: 3.5.2 Summary: Static website
+Metadata-Version: 2.1 Name: mdiocre Version: 3.5.3 Summary: Static website
 generator Home-page: https://zumi.neocities.org/stuff/mdiocre Author: Zumi
 Daxuya Author-email: daxuya.zumi+mdiocre@protonmail.com License: MIT Keywords:
 converter,generator,markdown,html,static Classifier: Development Status :: 4 -
 Beta Classifier: Intended Audience :: Developers Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Classifier: Natural Language :: English Classifier: Programming Language ::
 Python Classifier: Programming Language :: Python :: 3 Classifier: Programming
```

### Comparing `mdiocre-3.5.2/mdiocre.egg-info/SOURCES.txt` & `mdiocre-3.5.3/mdiocre.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mdiocre-3.5.2/setup.py` & `mdiocre-3.5.3/setup.py`

 * *Files identical despite different names*

### Comparing `mdiocre-3.5.2/versioning.py` & `mdiocre-3.5.3/versioning.py`

 * *Files identical despite different names*

