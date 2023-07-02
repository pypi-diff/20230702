# Comparing `tmp/heavylight-1.0.1.tar.gz` & `tmp/heavylight-1.0.2.tar.gz`

## Comparing `heavylight-1.0.1.tar` & `heavylight-1.0.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 heavylight-1.0.1/Pipfile
--rw-r--r--   0        0        0   123112 2020-02-02 00:00:00.000000 heavylight-1.0.1/Pipfile.lock
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 heavylight-1.0.1/Untitled.ipynb
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 heavylight-1.0.1/server_user_id.txt
--rw-r--r--   0        0        0     5136 2020-02-02 00:00:00.000000 heavylight-1.0.1/cythonz/benchmark.ipynb
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 heavylight-1.0.1/cythonz/cvect_memo.cpp
--rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 heavylight-1.0.1/cythonz/cvect_memo.pyx
--rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 heavylight-1.0.1/cythonz/cvect_memo_vector.pyx
--rw-r--r--   0        0        0     6424 2020-02-02 00:00:00.000000 heavylight-1.0.1/cythonz/heavylight.py
--rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 heavylight-1.0.1/cythonz/make_data.ipynb
--rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 heavylight-1.0.1/cythonz/memo_dict.py
--rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 heavylight-1.0.1/cythonz/memo_hl.py
--rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 heavylight-1.0.1/cythonz/memo_np.py
--rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 heavylight-1.0.1/cythonz/memo_np_hl.py
--rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 heavylight-1.0.1/cythonz/memo_try.py
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 heavylight-1.0.1/cythonz/setup.py
--rw-r--r--   0        0        0     2505 2020-02-02 00:00:00.000000 heavylight-1.0.1/cythonz/table_a.csv
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 heavylight-1.0.1/cythonz/test.py
--rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 heavylight-1.0.1/cythonz/.vscode/c_cpp_properties.json
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 heavylight-1.0.1/examples/readme.md
--rw-r--r--   0        0        0     6424 2020-02-02 00:00:00.000000 heavylight-1.0.1/examples/notebook/heavylight.py
--rw-r--r--   0        0        0    61719 2020-02-02 00:00:00.000000 heavylight-1.0.1/examples/notebook/heavylight_basic.ipynb
--rw-r--r--   0        0        0    61991 2020-02-02 00:00:00.000000 heavylight-1.0.1/examples/notebook/heavylight_tables.ipynb
--rw-r--r--   0        0        0     1206 2020-02-02 00:00:00.000000 heavylight-1.0.1/examples/notebook/sample_q_x_table.csv
--rw-r--r--   0        0        0     9325 2020-02-02 00:00:00.000000 heavylight-1.0.1/examples/notebook/table_maker.ipynb
--rw-r--r--   0        0        0     4932 2020-02-02 00:00:00.000000 heavylight-1.0.1/examples/notebook/vectors.ipynb
--rw-r--r--   0        0        0     4606 2020-02-02 00:00:00.000000 heavylight-1.0.1/examples/notebook/vectors.py
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 heavylight-1.0.1/heavylight/build_examples.py
--rw-r--r--   0        0        0     6424 2020-02-02 00:00:00.000000 heavylight-1.0.1/heavylight/heavylight.py
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 heavylight-1.0.1/src/heavylight/__init__.py
--rw-r--r--   0        0        0     6424 2020-02-02 00:00:00.000000 heavylight-1.0.1/src/heavylight/heavylight.py
--rw-r--r--   0        0        0   300723 2020-02-02 00:00:00.000000 heavylight-1.0.1/tests/protection_risk_model_generic.xlsx
--rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 heavylight-1.0.1/.gitignore
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 heavylight-1.0.1/LICENSE
--rw-r--r--   0        0        0     2029 2020-02-02 00:00:00.000000 heavylight-1.0.1/README.md
--rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 heavylight-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     2472 2020-02-02 00:00:00.000000 heavylight-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 heavylight-1.0.2/Pipfile
+-rw-r--r--   0        0        0   123112 2020-02-02 00:00:00.000000 heavylight-1.0.2/Pipfile.lock
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 heavylight-1.0.2/Untitled.ipynb
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 heavylight-1.0.2/server_user_id.txt
+-rw-r--r--   0        0        0     5136 2020-02-02 00:00:00.000000 heavylight-1.0.2/cythonz/benchmark.ipynb
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 heavylight-1.0.2/cythonz/cvect_memo.cpp
+-rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 heavylight-1.0.2/cythonz/cvect_memo.pyx
+-rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 heavylight-1.0.2/cythonz/cvect_memo_vector.pyx
+-rw-r--r--   0        0        0     6424 2020-02-02 00:00:00.000000 heavylight-1.0.2/cythonz/heavylight.py
+-rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 heavylight-1.0.2/cythonz/make_data.ipynb
+-rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 heavylight-1.0.2/cythonz/memo_dict.py
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 heavylight-1.0.2/cythonz/memo_hl.py
+-rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 heavylight-1.0.2/cythonz/memo_np.py
+-rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 heavylight-1.0.2/cythonz/memo_np_hl.py
+-rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 heavylight-1.0.2/cythonz/memo_try.py
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 heavylight-1.0.2/cythonz/setup.py
+-rw-r--r--   0        0        0     2505 2020-02-02 00:00:00.000000 heavylight-1.0.2/cythonz/table_a.csv
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 heavylight-1.0.2/cythonz/test.py
+-rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 heavylight-1.0.2/cythonz/.vscode/c_cpp_properties.json
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 heavylight-1.0.2/examples/readme.md
+-rw-r--r--   0        0        0     6424 2020-02-02 00:00:00.000000 heavylight-1.0.2/examples/notebook/heavylight.py
+-rw-r--r--   0        0        0    61719 2020-02-02 00:00:00.000000 heavylight-1.0.2/examples/notebook/heavylight_basic.ipynb
+-rw-r--r--   0        0        0    61991 2020-02-02 00:00:00.000000 heavylight-1.0.2/examples/notebook/heavylight_tables.ipynb
+-rw-r--r--   0        0        0     1206 2020-02-02 00:00:00.000000 heavylight-1.0.2/examples/notebook/sample_q_x_table.csv
+-rw-r--r--   0        0        0     9325 2020-02-02 00:00:00.000000 heavylight-1.0.2/examples/notebook/table_maker.ipynb
+-rw-r--r--   0        0        0     4932 2020-02-02 00:00:00.000000 heavylight-1.0.2/examples/notebook/vectors.ipynb
+-rw-r--r--   0        0        0     4606 2020-02-02 00:00:00.000000 heavylight-1.0.2/examples/notebook/vectors.py
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 heavylight-1.0.2/heavylight/build_examples.py
+-rw-r--r--   0        0        0     6424 2020-02-02 00:00:00.000000 heavylight-1.0.2/heavylight/heavylight.py
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 heavylight-1.0.2/src/heavylight/__init__.py
+-rw-r--r--   0        0        0     6424 2020-02-02 00:00:00.000000 heavylight-1.0.2/src/heavylight/heavylight.py
+-rw-r--r--   0        0        0   300723 2020-02-02 00:00:00.000000 heavylight-1.0.2/tests/protection_risk_model_generic.xlsx
+-rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 heavylight-1.0.2/.gitignore
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 heavylight-1.0.2/LICENSE
+-rw-r--r--   0        0        0     2029 2020-02-02 00:00:00.000000 heavylight-1.0.2/README.md
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 heavylight-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2499 2020-02-02 00:00:00.000000 heavylight-1.0.2/PKG-INFO
```

### Comparing `heavylight-1.0.1/Pipfile.lock` & `heavylight-1.0.2/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.1/cythonz/benchmark.ipynb` & `heavylight-1.0.2/cythonz/benchmark.ipynb`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.1/cythonz/cvect_memo.pyx` & `heavylight-1.0.2/cythonz/cvect_memo.pyx`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.1/cythonz/cvect_memo_vector.pyx` & `heavylight-1.0.2/cythonz/cvect_memo_vector.pyx`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.1/cythonz/heavylight.py` & `heavylight-1.0.2/cythonz/heavylight.py`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.1/cythonz/make_data.ipynb` & `heavylight-1.0.2/cythonz/make_data.ipynb`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.1/cythonz/memo_dict.py` & `heavylight-1.0.2/cythonz/memo_dict.py`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.1/cythonz/memo_np.py` & `heavylight-1.0.2/cythonz/memo_np.py`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.1/cythonz/memo_np_hl.py` & `heavylight-1.0.2/cythonz/memo_np_hl.py`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.1/cythonz/memo_try.py` & `heavylight-1.0.2/cythonz/memo_try.py`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.1/cythonz/table_a.csv` & `heavylight-1.0.2/cythonz/table_a.csv`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.1/examples/notebook/heavylight.py` & `heavylight-1.0.2/examples/notebook/heavylight.py`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.1/examples/notebook/heavylight_basic.ipynb` & `heavylight-1.0.2/examples/notebook/heavylight_basic.ipynb`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.1/examples/notebook/heavylight_tables.ipynb` & `heavylight-1.0.2/examples/notebook/heavylight_tables.ipynb`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.1/examples/notebook/sample_q_x_table.csv` & `heavylight-1.0.2/examples/notebook/sample_q_x_table.csv`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.1/examples/notebook/table_maker.ipynb` & `heavylight-1.0.2/examples/notebook/table_maker.ipynb`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.1/examples/notebook/vectors.ipynb` & `heavylight-1.0.2/examples/notebook/vectors.ipynb`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.1/examples/notebook/vectors.py` & `heavylight-1.0.2/examples/notebook/vectors.py`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.1/heavylight/heavylight.py` & `heavylight-1.0.2/heavylight/heavylight.py`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.1/src/heavylight/heavylight.py` & `heavylight-1.0.2/src/heavylight/heavylight.py`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.1/tests/protection_risk_model_generic.xlsx` & `heavylight-1.0.2/tests/protection_risk_model_generic.xlsx`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.1/.gitignore` & `heavylight-1.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.1/LICENSE` & `heavylight-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.1/README.md` & `heavylight-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.1/pyproject.toml` & `heavylight-1.0.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,26 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 
 [project]
 name = "heavylight"
-version = "1.0.1"
+version = "1.0.2"
 authors = [
   { name="Lewis Fogden", email="lewisfogden@gmail.com" },
 ]
 description = "Heavylight Actuarial Modelling Framework"
 readme = "README.md"
 requires-python = ">=3.8"
+
+dependencies = [
+    "pandas>=1.2",
+]
+
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
```

### Comparing `heavylight-1.0.1/PKG-INFO` & `heavylight-1.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: heavylight
-Version: 1.0.1
+Version: 1.0.2
 Summary: Heavylight Actuarial Modelling Framework
 Project-URL: Homepage, https://github.com/lewisfogden/heavylight/
 Project-URL: Bug Tracker, https://github.com/lewisfogden/heavylight/issues
 Author-email: Lewis Fogden <lewisfogden@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
+Requires-Dist: pandas>=1.2
 Description-Content-Type: text/markdown
 
 # heavylight
 
 A lightweight actuarial modelling framework for Python
 
 - single script
```

