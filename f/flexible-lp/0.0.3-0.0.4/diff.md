# Comparing `tmp/flexible_lp-0.0.3.tar.gz` & `tmp/flexible_lp-0.0.4.tar.gz`

## Comparing `flexible_lp-0.0.3.tar` & `flexible_lp-0.0.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 flexible_lp-0.0.3/.DS_Store
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 flexible_lp-0.0.3/src/flexible_lp/__init__.py
--rw-r--r--   0        0        0    12481 2020-02-02 00:00:00.000000 flexible_lp-0.0.3/src/flexible_lp/simplex.py
--rw-r--r--   0        0        0     3767 2020-02-02 00:00:00.000000 flexible_lp-0.0.3/src/flexible_lp/tableau.py
--rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 flexible_lp-0.0.3/LICENSE
--rw-r--r--   0        0        0     3908 2020-02-02 00:00:00.000000 flexible_lp-0.0.3/README.md
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 flexible_lp-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     4474 2020-02-02 00:00:00.000000 flexible_lp-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 flexible_lp-0.0.4/.DS_Store
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 flexible_lp-0.0.4/src/flexible_lp/__init__.py
+-rw-r--r--   0        0        0    12481 2020-02-02 00:00:00.000000 flexible_lp-0.0.4/src/flexible_lp/simplex.py
+-rw-r--r--   0        0        0     3767 2020-02-02 00:00:00.000000 flexible_lp-0.0.4/src/flexible_lp/tableau.py
+-rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 flexible_lp-0.0.4/LICENSE
+-rw-r--r--   0        0        0     3956 2020-02-02 00:00:00.000000 flexible_lp-0.0.4/README.md
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 flexible_lp-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     4522 2020-02-02 00:00:00.000000 flexible_lp-0.0.4/PKG-INFO
```

### Comparing `flexible_lp-0.0.3/.DS_Store` & `flexible_lp-0.0.4/.DS_Store`

 * *Files identical despite different names*

### Comparing `flexible_lp-0.0.3/src/flexible_lp/simplex.py` & `flexible_lp-0.0.4/src/flexible_lp/simplex.py`

 * *Files identical despite different names*

### Comparing `flexible_lp-0.0.3/src/flexible_lp/tableau.py` & `flexible_lp-0.0.4/src/flexible_lp/tableau.py`

 * *Files identical despite different names*

### Comparing `flexible_lp-0.0.3/LICENSE` & `flexible_lp-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `flexible_lp-0.0.3/README.md` & `flexible_lp-0.0.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 ```
 # Example 0: solving an LP
 Suppose we had the following lp
 $$\text{maximize}\ 3x + 5y;\ x + y \leq 10,\ x,y\geq0.$$
 Its optimal value is `50`, with $x = 0, y = 10$.
 Here is a python3 file to solve it:
 ```
-from simplex import linprog
+from flexible_lp.simplex import linprog
 from fractions import Fraction
 
 opt_val, opt_vec = linprog(c = [3,5], A_l = [[1, 1]], b_l = [10], maximize = True)
 print(opt_val, opt_vec)
 ```
 This outputs the following:
 ```
@@ -53,29 +53,29 @@
 
 # Example 1: solving an LP with fractions
 Suppose we have the same lp
 $$\text{maximize}\ 3x + 5y;\ x + y \leq 10,\ x,y\geq0.$$
 Here is a python3 file to solve using fractions. 
 The `value_map` parameter converts the supplied integers to the Fraction type before solving:
 ```
-from simplex import linprog
+from flexible_lp.simplex import linprog
 from fractions import Fraction
 
 opt_val, opt_vec = linprog(c = [3,5], A_l = [[1, 1]], b_l = [10], maximize = True, value_map = Fraction)
 print(opt_val, opt_vec)
 ```
 This outputs the following:
 ```
 50 [0, Fraction(10, 1)]
 ```
 # Example 2: solving an LP with fractional coefficients
 $$\text{maximize}\ \frac{4}{5}x - 5y;\ \frac{12}{7}x - \frac{1}{2}y \leq 10,\ x,y\geq0.$$
 
 ```
-from simplex import linprog
+from flexible_lp.simplex import linprog
 from fractions import Fraction
 print(linprog(c = [Fraction(4,5), -Fraction(5)], A_l = [[Fraction(12,7), -Fraction(1,2)]], b_l = [Fraction(10)], maximize = True))
 ```
 ```
 (Fraction(14, 3), [Fraction(35, 6), 0])
 ```
 Note that `value_map` is not needed here since everything already starts as Fraction objects. But we could have still used it and saved ourselves a litte pain writing out fractions:
@@ -87,15 +87,15 @@
 
 $$x + y + z \geq 10,$$
 
 $$5x+3y+1\geq 9,$$
 
 $$x,y,z\geq0.$$
 ```
-from simplex import linprog
+from flexible_lp.simplex import linprog
 from fractions import Fraction
 print(linprog(c = [-2,7,1], A_g = [[5,1,1], [1,3,1]], b_g = [5,9], value_map = Fraction))
 ```
 
 ```
 (-inf, [inf, 0, 0])
 ```
```

### Comparing `flexible_lp-0.0.3/pyproject.toml` & `flexible_lp-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "flexible_lp"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   {name="Matthew Ellison", email="matthew.v.ellison@gmail.com"},
 ]
 description = "A pure python3 library to solve linear programs using, for example, fractions."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `flexible_lp-0.0.3/PKG-INFO` & `flexible_lp-0.0.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flexible_lp
-Version: 0.0.3
+Version: 0.0.4
 Summary: A pure python3 library to solve linear programs using, for example, fractions.
 Project-URL: Homepage, https://github.com/mve17/flexible_lp/
 Project-URL: Bug Tracker, https://github.com/mve17/flexible_lp/issues
 Author-email: Matthew Ellison <matthew.v.ellison@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -48,15 +48,15 @@
 ```
 # Example 0: solving an LP
 Suppose we had the following lp
 $$\text{maximize}\ 3x + 5y;\ x + y \leq 10,\ x,y\geq0.$$
 Its optimal value is `50`, with $x = 0, y = 10$.
 Here is a python3 file to solve it:
 ```
-from simplex import linprog
+from flexible_lp.simplex import linprog
 from fractions import Fraction
 
 opt_val, opt_vec = linprog(c = [3,5], A_l = [[1, 1]], b_l = [10], maximize = True)
 print(opt_val, opt_vec)
 ```
 This outputs the following:
 ```
@@ -67,29 +67,29 @@
 
 # Example 1: solving an LP with fractions
 Suppose we have the same lp
 $$\text{maximize}\ 3x + 5y;\ x + y \leq 10,\ x,y\geq0.$$
 Here is a python3 file to solve using fractions. 
 The `value_map` parameter converts the supplied integers to the Fraction type before solving:
 ```
-from simplex import linprog
+from flexible_lp.simplex import linprog
 from fractions import Fraction
 
 opt_val, opt_vec = linprog(c = [3,5], A_l = [[1, 1]], b_l = [10], maximize = True, value_map = Fraction)
 print(opt_val, opt_vec)
 ```
 This outputs the following:
 ```
 50 [0, Fraction(10, 1)]
 ```
 # Example 2: solving an LP with fractional coefficients
 $$\text{maximize}\ \frac{4}{5}x - 5y;\ \frac{12}{7}x - \frac{1}{2}y \leq 10,\ x,y\geq0.$$
 
 ```
-from simplex import linprog
+from flexible_lp.simplex import linprog
 from fractions import Fraction
 print(linprog(c = [Fraction(4,5), -Fraction(5)], A_l = [[Fraction(12,7), -Fraction(1,2)]], b_l = [Fraction(10)], maximize = True))
 ```
 ```
 (Fraction(14, 3), [Fraction(35, 6), 0])
 ```
 Note that `value_map` is not needed here since everything already starts as Fraction objects. But we could have still used it and saved ourselves a litte pain writing out fractions:
@@ -101,15 +101,15 @@
 
 $$x + y + z \geq 10,$$
 
 $$5x+3y+1\geq 9,$$
 
 $$x,y,z\geq0.$$
 ```
-from simplex import linprog
+from flexible_lp.simplex import linprog
 from fractions import Fraction
 print(linprog(c = [-2,7,1], A_g = [[5,1,1], [1,3,1]], b_g = [5,9], value_map = Fraction))
 ```
 
 ```
 (-inf, [inf, 0, 0])
 ```
```

