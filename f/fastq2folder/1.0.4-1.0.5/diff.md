# Comparing `tmp/fastq2folder-1.0.4.tar.gz` & `tmp/fastq2folder-1.0.5.tar.gz`

## Comparing `fastq2folder-1.0.4.tar` & `fastq2folder-1.0.5.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastq2folder-1.0.4/src/fastq2folder/__init__.py
--rw-r--r--   0        0        0     6151 2020-02-02 00:00:00.000000 fastq2folder-1.0.4/src/fastq2folder/fastq2folder.py
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 fastq2folder-1.0.4/LICENSE
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 fastq2folder-1.0.4/README.md
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 fastq2folder-1.0.4/pyproject.toml
--rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 fastq2folder-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastq2folder-1.0.5/src/fastq2folder/__init__.py
+-rw-r--r--   0        0        0     9241 2020-02-02 00:00:00.000000 fastq2folder-1.0.5/src/fastq2folder/fastq2folder.py
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 fastq2folder-1.0.5/LICENSE
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 fastq2folder-1.0.5/README.md
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 fastq2folder-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 fastq2folder-1.0.5/PKG-INFO
```

### Comparing `fastq2folder-1.0.4/LICENSE` & `fastq2folder-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `fastq2folder-1.0.4/README.md` & `fastq2folder-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `fastq2folder-1.0.4/pyproject.toml` & `fastq2folder-1.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling", "pandas", "Bio", "scipy", "numpy", "matplotlib", "seaborn"]
 build-backend = "hatchling.build"
 
 [project]
 name = "fastq2folder"
-version = "1.0.4"
+version = "1.0.5"
 authors = [
   { name="Elizabeth Gardner", email="egar18111@gmail.com" },
 ]
 description = "Script to process fastq files before epi2me analysis"
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `fastq2folder-1.0.4/PKG-INFO` & `fastq2folder-1.0.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastq2folder
-Version: 1.0.4
+Version: 1.0.5
 Summary: Script to process fastq files before epi2me analysis
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Author-email: Elizabeth Gardner <egar18111@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

