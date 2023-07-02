# Comparing `tmp/heavylight-1.0.0.tar.gz` & `tmp/heavylight-1.0.1.tar.gz`

## Comparing `heavylight-1.0.0.tar` & `heavylight-1.0.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 heavylight-1.0.0/Pipfile
--rw-r--r--   0        0        0   123112 2020-02-02 00:00:00.000000 heavylight-1.0.0/Pipfile.lock
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 heavylight-1.0.0/Untitled.ipynb
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 heavylight-1.0.0/server_user_id.txt
--rw-r--r--   0        0        0     5136 2020-02-02 00:00:00.000000 heavylight-1.0.0/cythonz/benchmark.ipynb
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 heavylight-1.0.0/cythonz/cvect_memo.cpp
--rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 heavylight-1.0.0/cythonz/cvect_memo.pyx
--rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 heavylight-1.0.0/cythonz/cvect_memo_vector.pyx
--rw-r--r--   0        0        0     6424 2020-02-02 00:00:00.000000 heavylight-1.0.0/cythonz/heavylight.py
--rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 heavylight-1.0.0/cythonz/make_data.ipynb
--rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 heavylight-1.0.0/cythonz/memo_dict.py
--rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 heavylight-1.0.0/cythonz/memo_hl.py
--rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 heavylight-1.0.0/cythonz/memo_np.py
--rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 heavylight-1.0.0/cythonz/memo_np_hl.py
--rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 heavylight-1.0.0/cythonz/memo_try.py
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 heavylight-1.0.0/cythonz/setup.py
--rw-r--r--   0        0        0     2505 2020-02-02 00:00:00.000000 heavylight-1.0.0/cythonz/table_a.csv
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 heavylight-1.0.0/cythonz/test.py
--rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 heavylight-1.0.0/cythonz/.vscode/c_cpp_properties.json
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 heavylight-1.0.0/examples/readme.md
--rw-r--r--   0        0        0     6424 2020-02-02 00:00:00.000000 heavylight-1.0.0/examples/notebook/heavylight.py
--rw-r--r--   0        0        0    61719 2020-02-02 00:00:00.000000 heavylight-1.0.0/examples/notebook/heavylight_basic.ipynb
--rw-r--r--   0        0        0    61991 2020-02-02 00:00:00.000000 heavylight-1.0.0/examples/notebook/heavylight_tables.ipynb
--rw-r--r--   0        0        0     1206 2020-02-02 00:00:00.000000 heavylight-1.0.0/examples/notebook/sample_q_x_table.csv
--rw-r--r--   0        0        0     9325 2020-02-02 00:00:00.000000 heavylight-1.0.0/examples/notebook/table_maker.ipynb
--rw-r--r--   0        0        0     4932 2020-02-02 00:00:00.000000 heavylight-1.0.0/examples/notebook/vectors.ipynb
--rw-r--r--   0        0        0     4606 2020-02-02 00:00:00.000000 heavylight-1.0.0/examples/notebook/vectors.py
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 heavylight-1.0.0/heavylight/build_examples.py
--rw-r--r--   0        0        0     6424 2020-02-02 00:00:00.000000 heavylight-1.0.0/heavylight/heavylight.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 heavylight-1.0.0/src/heavylight/__init__.py
--rw-r--r--   0        0        0     6424 2020-02-02 00:00:00.000000 heavylight-1.0.0/src/heavylight/heavylight.py
--rw-r--r--   0        0        0   300723 2020-02-02 00:00:00.000000 heavylight-1.0.0/tests/protection_risk_model_generic.xlsx
--rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 heavylight-1.0.0/.gitignore
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 heavylight-1.0.0/LICENSE
--rw-r--r--   0        0        0     2029 2020-02-02 00:00:00.000000 heavylight-1.0.0/README.md
--rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 heavylight-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     2472 2020-02-02 00:00:00.000000 heavylight-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 heavylight-1.0.1/Pipfile
+-rw-r--r--   0        0        0   123112 2020-02-02 00:00:00.000000 heavylight-1.0.1/Pipfile.lock
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 heavylight-1.0.1/Untitled.ipynb
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 heavylight-1.0.1/server_user_id.txt
+-rw-r--r--   0        0        0     5136 2020-02-02 00:00:00.000000 heavylight-1.0.1/cythonz/benchmark.ipynb
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 heavylight-1.0.1/cythonz/cvect_memo.cpp
+-rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 heavylight-1.0.1/cythonz/cvect_memo.pyx
+-rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 heavylight-1.0.1/cythonz/cvect_memo_vector.pyx
+-rw-r--r--   0        0        0     6424 2020-02-02 00:00:00.000000 heavylight-1.0.1/cythonz/heavylight.py
+-rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 heavylight-1.0.1/cythonz/make_data.ipynb
+-rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 heavylight-1.0.1/cythonz/memo_dict.py
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 heavylight-1.0.1/cythonz/memo_hl.py
+-rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 heavylight-1.0.1/cythonz/memo_np.py
+-rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 heavylight-1.0.1/cythonz/memo_np_hl.py
+-rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 heavylight-1.0.1/cythonz/memo_try.py
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 heavylight-1.0.1/cythonz/setup.py
+-rw-r--r--   0        0        0     2505 2020-02-02 00:00:00.000000 heavylight-1.0.1/cythonz/table_a.csv
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 heavylight-1.0.1/cythonz/test.py
+-rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 heavylight-1.0.1/cythonz/.vscode/c_cpp_properties.json
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 heavylight-1.0.1/examples/readme.md
+-rw-r--r--   0        0        0     6424 2020-02-02 00:00:00.000000 heavylight-1.0.1/examples/notebook/heavylight.py
+-rw-r--r--   0        0        0    61719 2020-02-02 00:00:00.000000 heavylight-1.0.1/examples/notebook/heavylight_basic.ipynb
+-rw-r--r--   0        0        0    61991 2020-02-02 00:00:00.000000 heavylight-1.0.1/examples/notebook/heavylight_tables.ipynb
+-rw-r--r--   0        0        0     1206 2020-02-02 00:00:00.000000 heavylight-1.0.1/examples/notebook/sample_q_x_table.csv
+-rw-r--r--   0        0        0     9325 2020-02-02 00:00:00.000000 heavylight-1.0.1/examples/notebook/table_maker.ipynb
+-rw-r--r--   0        0        0     4932 2020-02-02 00:00:00.000000 heavylight-1.0.1/examples/notebook/vectors.ipynb
+-rw-r--r--   0        0        0     4606 2020-02-02 00:00:00.000000 heavylight-1.0.1/examples/notebook/vectors.py
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 heavylight-1.0.1/heavylight/build_examples.py
+-rw-r--r--   0        0        0     6424 2020-02-02 00:00:00.000000 heavylight-1.0.1/heavylight/heavylight.py
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 heavylight-1.0.1/src/heavylight/__init__.py
+-rw-r--r--   0        0        0     6424 2020-02-02 00:00:00.000000 heavylight-1.0.1/src/heavylight/heavylight.py
+-rw-r--r--   0        0        0   300723 2020-02-02 00:00:00.000000 heavylight-1.0.1/tests/protection_risk_model_generic.xlsx
+-rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 heavylight-1.0.1/.gitignore
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 heavylight-1.0.1/LICENSE
+-rw-r--r--   0        0        0     2029 2020-02-02 00:00:00.000000 heavylight-1.0.1/README.md
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 heavylight-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     2472 2020-02-02 00:00:00.000000 heavylight-1.0.1/PKG-INFO
```

### Comparing `heavylight-1.0.0/Pipfile.lock` & `heavylight-1.0.1/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.0/cythonz/benchmark.ipynb` & `heavylight-1.0.1/cythonz/benchmark.ipynb`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.0/cythonz/cvect_memo.pyx` & `heavylight-1.0.1/cythonz/cvect_memo.pyx`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.0/cythonz/cvect_memo_vector.pyx` & `heavylight-1.0.1/cythonz/cvect_memo_vector.pyx`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.0/cythonz/heavylight.py` & `heavylight-1.0.1/cythonz/heavylight.py`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.0/cythonz/make_data.ipynb` & `heavylight-1.0.1/cythonz/make_data.ipynb`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.0/cythonz/memo_dict.py` & `heavylight-1.0.1/cythonz/memo_dict.py`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.0/cythonz/memo_np.py` & `heavylight-1.0.1/cythonz/memo_np.py`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.0/cythonz/memo_np_hl.py` & `heavylight-1.0.1/cythonz/memo_np_hl.py`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.0/cythonz/memo_try.py` & `heavylight-1.0.1/cythonz/memo_try.py`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.0/cythonz/table_a.csv` & `heavylight-1.0.1/cythonz/table_a.csv`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.0/examples/notebook/heavylight.py` & `heavylight-1.0.1/examples/notebook/heavylight.py`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.0/examples/notebook/heavylight_basic.ipynb` & `heavylight-1.0.1/examples/notebook/heavylight_basic.ipynb`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.0/examples/notebook/heavylight_tables.ipynb` & `heavylight-1.0.1/examples/notebook/heavylight_tables.ipynb`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.0/examples/notebook/sample_q_x_table.csv` & `heavylight-1.0.1/examples/notebook/sample_q_x_table.csv`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.0/examples/notebook/table_maker.ipynb` & `heavylight-1.0.1/examples/notebook/table_maker.ipynb`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.0/examples/notebook/vectors.ipynb` & `heavylight-1.0.1/examples/notebook/vectors.ipynb`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.0/examples/notebook/vectors.py` & `heavylight-1.0.1/examples/notebook/vectors.py`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.0/heavylight/heavylight.py` & `heavylight-1.0.1/heavylight/heavylight.py`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.0/src/heavylight/heavylight.py` & `heavylight-1.0.1/src/heavylight/heavylight.py`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.0/tests/protection_risk_model_generic.xlsx` & `heavylight-1.0.1/tests/protection_risk_model_generic.xlsx`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.0/.gitignore` & `heavylight-1.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.0/LICENSE` & `heavylight-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.0/README.md` & `heavylight-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `heavylight-1.0.0/pyproject.toml` & `heavylight-1.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 
 [project]
 name = "heavylight"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
   { name="Lewis Fogden", email="lewisfogden@gmail.com" },
 ]
 description = "Heavylight Actuarial Modelling Framework"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `heavylight-1.0.0/PKG-INFO` & `heavylight-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heavylight
-Version: 1.0.0
+Version: 1.0.1
 Summary: Heavylight Actuarial Modelling Framework
 Project-URL: Homepage, https://github.com/lewisfogden/heavylight/
 Project-URL: Bug Tracker, https://github.com/lewisfogden/heavylight/issues
 Author-email: Lewis Fogden <lewisfogden@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

