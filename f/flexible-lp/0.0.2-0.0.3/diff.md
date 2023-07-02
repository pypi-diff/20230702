# Comparing `tmp/flexible_lp-0.0.2.tar.gz` & `tmp/flexible_lp-0.0.3.tar.gz`

## Comparing `flexible_lp-0.0.2.tar` & `flexible_lp-0.0.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 flexible_lp-0.0.2/.DS_Store
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 flexible_lp-0.0.2/src/flexible_lp/__init__.py
--rw-r--r--   0        0        0    12769 2020-02-02 00:00:00.000000 flexible_lp-0.0.2/src/flexible_lp/simplex.py
--rw-r--r--   0        0        0     3767 2020-02-02 00:00:00.000000 flexible_lp-0.0.2/src/flexible_lp/tableau.py
--rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 flexible_lp-0.0.2/LICENSE
--rw-r--r--   0        0        0     3908 2020-02-02 00:00:00.000000 flexible_lp-0.0.2/README.md
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 flexible_lp-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     4474 2020-02-02 00:00:00.000000 flexible_lp-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 flexible_lp-0.0.3/.DS_Store
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 flexible_lp-0.0.3/src/flexible_lp/__init__.py
+-rw-r--r--   0        0        0    12481 2020-02-02 00:00:00.000000 flexible_lp-0.0.3/src/flexible_lp/simplex.py
+-rw-r--r--   0        0        0     3767 2020-02-02 00:00:00.000000 flexible_lp-0.0.3/src/flexible_lp/tableau.py
+-rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 flexible_lp-0.0.3/LICENSE
+-rw-r--r--   0        0        0     3908 2020-02-02 00:00:00.000000 flexible_lp-0.0.3/README.md
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 flexible_lp-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     4474 2020-02-02 00:00:00.000000 flexible_lp-0.0.3/PKG-INFO
```

### Comparing `flexible_lp-0.0.2/.DS_Store` & `flexible_lp-0.0.3/.DS_Store`

 * *Files identical despite different names*

### Comparing `flexible_lp-0.0.2/src/flexible_lp/simplex.py` & `flexible_lp-0.0.3/src/flexible_lp/simplex.py`

 * *Files 4% similar despite different names*

```diff
@@ -317,14 +317,8 @@
 			print(f"time for d = {d}: {round(end - start,2)} seconds")
 			#print(f"{c=}")
 			#print(opt_val, vars)
 			d *= 2
 		
 		import matplotlib.pyplot as plt
 		plt.plot(ds, times)
-		plt.show()
-
-
-from fractions import Fraction
-print(linprog(c = [Fraction(4,5),-Fraction(5)], A_l = [[Fraction(12,7),-Fraction(1,2)]], b_l = [Fraction(10)], maximize = True))
-
-linprog(c = [Fraction(4,5), 5], A_l = [[-Fraction(12,7),Fraction(1,2)]], b_l = [10], maximize = True, value_map = Fraction)
+		plt.show()
```

### Comparing `flexible_lp-0.0.2/src/flexible_lp/tableau.py` & `flexible_lp-0.0.3/src/flexible_lp/tableau.py`

 * *Files identical despite different names*

### Comparing `flexible_lp-0.0.2/LICENSE` & `flexible_lp-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `flexible_lp-0.0.2/README.md` & `flexible_lp-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `flexible_lp-0.0.2/pyproject.toml` & `flexible_lp-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "flexible_lp"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   {name="Matthew Ellison", email="matthew.v.ellison@gmail.com"},
 ]
 description = "A pure python3 library to solve linear programs using, for example, fractions."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `flexible_lp-0.0.2/PKG-INFO` & `flexible_lp-0.0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flexible_lp
-Version: 0.0.2
+Version: 0.0.3
 Summary: A pure python3 library to solve linear programs using, for example, fractions.
 Project-URL: Homepage, https://github.com/mve17/flexible_lp/
 Project-URL: Bug Tracker, https://github.com/mve17/flexible_lp/issues
 Author-email: Matthew Ellison <matthew.v.ellison@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

