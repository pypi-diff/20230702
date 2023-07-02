# Comparing `tmp/minifit-1.0.2.tar.gz` & `tmp/minifit-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "minifit-1.0.2.tar", last modified: Thu Jun 22 11:16:44 2023, max compression
+gzip compressed data, was "minifit-1.0.3.tar", last modified: Sun Jul  2 13:38:18 2023, max compression
```

## Comparing `minifit-1.0.2.tar` & `minifit-1.0.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 mike313   (1000) mike313   (1000)        0 2023-06-22 11:16:44.710146 minifit-1.0.2/
--rw-rw-r--   0 mike313   (1000) mike313   (1000)    35149 2023-04-13 19:30:30.000000 minifit-1.0.2/COPYING
--rw-rw-r--   0 mike313   (1000) mike313   (1000)     1126 2023-06-22 11:16:44.710146 minifit-1.0.2/PKG-INFO
--rw-rw-r--   0 mike313   (1000) mike313   (1000)      333 2023-04-17 05:55:44.000000 minifit-1.0.2/README.md
--rw-rw-r--   0 mike313   (1000) mike313   (1000)       85 2023-04-14 00:11:27.000000 minifit-1.0.2/pyproject.toml
--rw-rw-r--   0 mike313   (1000) mike313   (1000)      927 2023-06-22 11:16:44.710146 minifit-1.0.2/setup.cfg
-drwxrwxr-x   0 mike313   (1000) mike313   (1000)        0 2023-06-22 11:16:44.698146 minifit-1.0.2/src/
-drwxrwxr-x   0 mike313   (1000) mike313   (1000)        0 2023-06-22 11:16:44.702146 minifit-1.0.2/src/minifit/
--rw-rw-r--   0 mike313   (1000) mike313   (1000)      966 2023-06-22 00:04:12.000000 minifit-1.0.2/src/minifit/__init__.py
--rw-rw-r--   0 mike313   (1000) mike313   (1000)     2817 2023-06-22 09:39:58.000000 minifit-1.0.2/src/minifit/exp.py
--rw-rw-r--   0 mike313   (1000) mike313   (1000)     8834 2023-06-22 10:23:54.000000 minifit-1.0.2/src/minifit/fit_base.py
--rw-rw-r--   0 mike313   (1000) mike313   (1000)     2857 2023-06-22 09:39:38.000000 minifit-1.0.2/src/minifit/gauss.py
--rw-rw-r--   0 mike313   (1000) mike313   (1000)     2914 2023-06-22 10:16:43.000000 minifit-1.0.2/src/minifit/lennard_jones.py
--rw-rw-r--   0 mike313   (1000) mike313   (1000)     4613 2023-06-22 10:16:43.000000 minifit-1.0.2/src/minifit/morse.py
--rw-rw-r--   0 mike313   (1000) mike313   (1000)     3275 2023-06-22 10:17:35.000000 minifit-1.0.2/src/minifit/poly.py
-drwxrwxr-x   0 mike313   (1000) mike313   (1000)        0 2023-06-22 11:16:44.710146 minifit-1.0.2/src/minifit/tests/
--rw-rw-r--   0 mike313   (1000) mike313   (1000)      744 2023-06-04 17:31:04.000000 minifit-1.0.2/src/minifit/tests/__init__.py
--rw-rw-r--   0 mike313   (1000) mike313   (1000)     1122 2023-06-22 09:43:33.000000 minifit-1.0.2/src/minifit/tests/common.py
--rw-rw-r--   0 mike313   (1000) mike313   (1000)     1954 2023-06-22 09:41:57.000000 minifit-1.0.2/src/minifit/tests/test_exponential.py
--rw-rw-r--   0 mike313   (1000) mike313   (1000)     1967 2023-06-22 09:41:52.000000 minifit-1.0.2/src/minifit/tests/test_gauss.py
--rw-rw-r--   0 mike313   (1000) mike313   (1000)     2128 2023-06-22 09:43:33.000000 minifit-1.0.2/src/minifit/tests/test_lennard_jones.py
--rw-rw-r--   0 mike313   (1000) mike313   (1000)     2969 2023-06-22 09:41:30.000000 minifit-1.0.2/src/minifit/tests/test_morse.py
--rw-rw-r--   0 mike313   (1000) mike313   (1000)     2573 2023-06-22 09:41:37.000000 minifit-1.0.2/src/minifit/tests/test_poly.py
--rw-rw-r--   0 mike313   (1000) mike313   (1000)     3090 2023-06-22 09:41:44.000000 minifit-1.0.2/src/minifit/tests/test_user.py
--rw-rw-r--   0 mike313   (1000) mike313   (1000)     4218 2023-06-22 10:26:59.000000 minifit-1.0.2/src/minifit/user_defined.py
-drwxrwxr-x   0 mike313   (1000) mike313   (1000)        0 2023-06-22 11:16:44.706146 minifit-1.0.2/src/minifit.egg-info/
--rw-rw-r--   0 mike313   (1000) mike313   (1000)     1126 2023-06-22 11:16:44.000000 minifit-1.0.2/src/minifit.egg-info/PKG-INFO
--rw-rw-r--   0 mike313   (1000) mike313   (1000)      664 2023-06-22 11:16:44.000000 minifit-1.0.2/src/minifit.egg-info/SOURCES.txt
--rw-rw-r--   0 mike313   (1000) mike313   (1000)        1 2023-06-22 11:16:44.000000 minifit-1.0.2/src/minifit.egg-info/dependency_links.txt
--rw-rw-r--   0 mike313   (1000) mike313   (1000)       41 2023-06-22 11:16:44.000000 minifit-1.0.2/src/minifit.egg-info/requires.txt
--rw-rw-r--   0 mike313   (1000) mike313   (1000)        8 2023-06-22 11:16:44.000000 minifit-1.0.2/src/minifit.egg-info/top_level.txt
+drwxrwxr-x   0 mike313   (1000) mike313   (1000)        0 2023-07-02 13:38:18.775580 minifit-1.0.3/
+-rw-rw-r--   0 mike313   (1000) mike313   (1000)    35149 2023-04-13 19:30:30.000000 minifit-1.0.3/COPYING
+-rw-rw-r--   0 mike313   (1000) mike313   (1000)     1126 2023-07-02 13:38:18.775580 minifit-1.0.3/PKG-INFO
+-rw-rw-r--   0 mike313   (1000) mike313   (1000)      333 2023-04-17 05:55:44.000000 minifit-1.0.3/README.md
+-rw-rw-r--   0 mike313   (1000) mike313   (1000)       85 2023-04-14 00:11:27.000000 minifit-1.0.3/pyproject.toml
+-rw-rw-r--   0 mike313   (1000) mike313   (1000)     1000 2023-07-02 13:38:18.775580 minifit-1.0.3/setup.cfg
+drwxrwxr-x   0 mike313   (1000) mike313   (1000)        0 2023-07-02 13:38:18.759581 minifit-1.0.3/src/
+drwxrwxr-x   0 mike313   (1000) mike313   (1000)        0 2023-07-02 13:38:18.763581 minifit-1.0.3/src/minifit/
+-rw-rw-r--   0 mike313   (1000) mike313   (1000)      966 2023-06-22 00:04:12.000000 minifit-1.0.3/src/minifit/__init__.py
+-rw-rw-r--   0 mike313   (1000) mike313   (1000)     4160 2023-06-29 18:50:46.000000 minifit-1.0.3/src/minifit/exp.py
+-rw-rw-r--   0 mike313   (1000) mike313   (1000)     8530 2023-06-29 19:05:51.000000 minifit-1.0.3/src/minifit/fit_base.py
+-rw-rw-r--   0 mike313   (1000) mike313   (1000)     4204 2023-06-29 18:50:35.000000 minifit-1.0.3/src/minifit/gauss.py
+-rw-rw-r--   0 mike313   (1000) mike313   (1000)     4203 2023-06-29 18:49:42.000000 minifit-1.0.3/src/minifit/lennard_jones.py
+-rw-rw-r--   0 mike313   (1000) mike313   (1000)     5580 2023-06-29 18:49:57.000000 minifit-1.0.3/src/minifit/morse.py
+-rw-rw-r--   0 mike313   (1000) mike313   (1000)     4640 2023-06-29 18:50:06.000000 minifit-1.0.3/src/minifit/poly.py
+drwxrwxr-x   0 mike313   (1000) mike313   (1000)        0 2023-07-02 13:38:18.771581 minifit-1.0.3/src/minifit/tests/
+-rw-rw-r--   0 mike313   (1000) mike313   (1000)      744 2023-06-04 17:31:04.000000 minifit-1.0.3/src/minifit/tests/__init__.py
+-rw-rw-r--   0 mike313   (1000) mike313   (1000)     1122 2023-06-22 09:43:33.000000 minifit-1.0.3/src/minifit/tests/common.py
+-rw-rw-r--   0 mike313   (1000) mike313   (1000)     2282 2023-06-29 18:36:15.000000 minifit-1.0.3/src/minifit/tests/test_exponential.py
+-rw-rw-r--   0 mike313   (1000) mike313   (1000)     2296 2023-06-29 18:36:15.000000 minifit-1.0.3/src/minifit/tests/test_gauss.py
+-rw-rw-r--   0 mike313   (1000) mike313   (1000)     2538 2023-06-29 18:36:15.000000 minifit-1.0.3/src/minifit/tests/test_lennard_jones.py
+-rw-rw-r--   0 mike313   (1000) mike313   (1000)     3396 2023-06-29 18:36:15.000000 minifit-1.0.3/src/minifit/tests/test_morse.py
+-rw-rw-r--   0 mike313   (1000) mike313   (1000)     2878 2023-06-29 18:36:15.000000 minifit-1.0.3/src/minifit/tests/test_poly.py
+-rw-rw-r--   0 mike313   (1000) mike313   (1000)     3512 2023-06-29 18:36:15.000000 minifit-1.0.3/src/minifit/tests/test_user.py
+-rw-rw-r--   0 mike313   (1000) mike313   (1000)     5674 2023-06-29 18:48:42.000000 minifit-1.0.3/src/minifit/user_defined.py
+drwxrwxr-x   0 mike313   (1000) mike313   (1000)        0 2023-07-02 13:38:18.763581 minifit-1.0.3/src/minifit.egg-info/
+-rw-rw-r--   0 mike313   (1000) mike313   (1000)     1126 2023-07-02 13:38:18.000000 minifit-1.0.3/src/minifit.egg-info/PKG-INFO
+-rw-rw-r--   0 mike313   (1000) mike313   (1000)      664 2023-07-02 13:38:18.000000 minifit-1.0.3/src/minifit.egg-info/SOURCES.txt
+-rw-rw-r--   0 mike313   (1000) mike313   (1000)        1 2023-07-02 13:38:18.000000 minifit-1.0.3/src/minifit.egg-info/dependency_links.txt
+-rw-rw-r--   0 mike313   (1000) mike313   (1000)       55 2023-07-02 13:38:18.000000 minifit-1.0.3/src/minifit.egg-info/requires.txt
+-rw-rw-r--   0 mike313   (1000) mike313   (1000)        8 2023-07-02 13:38:18.000000 minifit-1.0.3/src/minifit.egg-info/top_level.txt
```

### Comparing `minifit-1.0.2/COPYING` & `minifit-1.0.3/COPYING`

 * *Files identical despite different names*

### Comparing `minifit-1.0.2/PKG-INFO` & `minifit-1.0.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: minifit
-Version: 1.0.2
+Version: 1.0.3
 Summary: MiniFit is a python package that can be used for fitting data.
 Home-page: https://gitlab.com/mike3.14/minifit
 Author: Michał Kopczyński
 Author-email: michal.kopczynski3.14@gmail.com
 Project-URL: repository, https://gitlab.com/mike3.14/minifit
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
```

### Comparing `minifit-1.0.2/setup.cfg` & `minifit-1.0.3/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,14 @@
+[build_sphinx]
+add_module_directory = True
+all_files = 1
+
 [metadata]
 name = minifit
-version = 1.0.2
+version = 1.0.3
 author = Michał Kopczyński
 author_email = michal.kopczynski3.14@gmail.com
 description = MiniFit is a python package that can be used for fitting data.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://gitlab.com/mike3.14/minifit
 project_urls = 
@@ -24,14 +28,15 @@
 	= src
 packages = find:
 python_requires = >=3.8
 install_requires = 
 	scipy<2.0.0
 	numpy<2.0.0
 	matplotlib<4.0.0
+	pathlib<2.0.0
 
 [options.packages.find]
 where = src
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `minifit-1.0.2/src/minifit/__init__.py` & `minifit-1.0.3/src/minifit/__init__.py`

 * *Files identical despite different names*

### Comparing `minifit-1.0.2/src/minifit/exp.py` & `minifit-1.0.3/src/minifit/exp.py`

 * *Files 23% similar despite different names*

```diff
@@ -43,18 +43,40 @@
 
         filename:
             (string) Name of the file that contains data.
 
         **Keyword arguments:**
 
         guess:
-            (tuple) Guess of the optimal parameters for the model.
+            (tuple) A guess of the optimal parameters for the model.
+            The number of guesses should match
+            the arguments that the model function expects.
+            For ax^2 + bx + c it expects (val1, val2, val3) etc.
+            Otherwise, an exception will be raised. If not passed, a default guess adequate for
+            the model function will be used.
+        auto_guess:
+            (bool) If true, tries to fit until chosen precision is reached. Default false.
+        auto_range:
+            (tuple) Sets boundaries for each parameter of the guess.
+            If not set, the default range is used. Only used if auto_guess is True.
+            Instead of guess = (5., 10., -3.)
+            pass auto_range = ((0.,10.), (5., 15.), (-40., 30.))
+            If fitting takes a lot of time, giving a better range might be helpful.
+        precision:
+            (float) Used by auto_guess. Default 0.4. Only used if auto_guess is True.
+            If auto_guess is True and fitting takes a lot of time, lowering the precision may be
+            necessary for convergence. Lowering the precision will make the fitting process faster,
+            but the quality of popt may be worse.
+        shift:
+            (bool) If true, shifts the data. Default false.
+                Data can be shifted and it may
+                make the convergence of the least squares algorithm easier.
         """
 
-        self.common_init(filename, **kwargs)
+        super().__init__(filename, **kwargs)
         self.type_of_fit = "Exponential"
         self.label_type = "exp_fit"
 
     def default_guess(self, context):
         """Default guess adequate for the model function."""
         guess = [1, 2, 1]
```

### Comparing `minifit-1.0.2/src/minifit/fit_base.py` & `minifit-1.0.3/src/minifit/fit_base.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,81 +38,72 @@
         print("-" * 100)
     elif str1 == " ":
         print(" ")
     else:
         print(f"\t{str1}")
 
 
-# pylint: disable=unnecessary-pass,attribute-defined-outside-init
-
-
 class FitBase(ABC):
     """
     Base class for all fitting classes
     """
 
-    def common_init(self, filename, **kwargs):
+    def __init__(self, filename, **kwargs):
         """
         Common constructor
         """
         self.type_of_fit = (
             "FitBase instance attribute - needs to be overwritten"
         )
         self.label_type = (
             "FitBase instance attribute - needs to be overwritten"
         )
-        path_data = Path("./minifit-data/" + filename)
-        path_cwd = Path.cwd()
-        if path_data.exists() is not True and path_cwd.exists is not True:
+
+        absolute_path = Path(filename)
+        path_data = Path("./data/" + filename)
+        path_cwd = Path.cwd() / Path(filename)
+        if (
+            path_data.exists() is not True
+            and path_cwd.exists is not True
+            and absolute_path.exists() is not True
+        ):
             raise FileNotFoundError(
-                f"\"Couldn't find {filename} in minifit-data"
+                f"Couldn't find {filename} in the data folder,\n"
+                f"current working directory, and by using an absolute path"
             )
 
         self.filename = filename
 
-        if kwargs.get("guess") is None:
-            self.guess = None
-        else:
-            self.guess = kwargs.get("guess")
-
-        # self.guess = kwargs.get("guess", None)
+        self.guess = kwargs.get("guess", None)
 
         if kwargs.get("auto_guess") is True:
             self.auto_guess = True
             self.auto_range = kwargs.get("auto_range", None)
         else:
             self.auto_guess = False
             self.auto_range = None
 
-        if kwargs.get("precision") is not None:
-            self.precision = kwargs.get("precision")
-        else:
-            self.precision = 0.4
-        # self.precision = kwargs.get("precision",  0.4)
+        self.precision = kwargs.get("precision", 0.4)
 
-        if kwargs.get("shift") is None:
-            self.shift = False
-        else:
-            self.shift = kwargs.get("shift")
-        # self.precision = kwargs.get("shift",  False)
+        self.shift = kwargs.get("shift", False)
 
         if path_data.exists() is True:
-            self.filename = filename
             self.read_data(str(path_data))
-        else:
-            self.filename = filename
+        elif path_cwd.exists() is True:
             self.read_data(str(path_cwd))
+        else:
+            self.read_data(str(absolute_path))
 
         self.popt = None
         self.pcov = None
         self.abs_sum_diff = np.inf
         self.sq_root_error = np.inf
 
     def read_data(self, filename):
-        """Reads data from each column then shifts the data."""
+        """Reads data from each column then shifts the data if shift is set to True."""
         cols = None
         with open(filename) as file:
             for line in file:
                 if not line.startswith("#"):
                     data = [float(x) for x in line.split()]
                     if cols is not None:
                         cols = np.vstack((cols, data))
@@ -147,15 +138,15 @@
     def print_info(self, popt):
         """
         Print info about popt in the format adequate for the model function.
         """
 
     def context_setter(self, xdata, ydata):
         """
-        If overwritten can return data useful for setting guess in random_gues and default_guess
+        If overwritten can return data useful for setting guess in random_guess and default_guess
         """
         return [xdata, ydata]
 
     def optimize(self, xdata, ydata, ind):
         """Finds the optimal parameters and corresponding errors."""
 
         guess = self.default_guess(self.context_setter(xdata, ydata))
@@ -176,17 +167,15 @@
                     )
 
                     self.popt, self.pcov = curve_fit(
                         self.model_function, xdata, ydata, p0=guess
                     )
                     diff = self.model_function(xdata, *self.popt) - ydata
                     self.abs_sum_diff = np.sum(abs(diff))
-                    self.sq_root_error = self.sq_root_error = np.sqrt(
-                        np.dot(diff, diff)
-                    )
+                    self.sq_root_error = np.sqrt(np.dot(diff, diff))
                 except RuntimeError:
                     log(
                         "Unable to fit with the current guess. Trying again with a new one..."
                     )
                 finally:
                     if (
                         self.sq_root_error < self.precision
```

### Comparing `minifit-1.0.2/src/minifit/gauss.py` & `minifit-1.0.3/src/minifit/tests/test_gauss.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+"""
+Module containing tests for GaussFit class.
+"""
+
 # -*- coding: utf-8 -*-
 # Copyright (C) 2023-- Michał Kopczyński
 #
 # This file is part of MiniFit.
 #
 # MiniFit is free software; you can redistribute it and/or
 # modify it under the terms of the GNU General Public License
@@ -12,84 +16,60 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, see <http://www.gnu.org/licenses/>
 #
-"""
-Module containing GaussFit class for curve fitting with normal distribution.
-"""
-import random
-import numpy as np
-import matplotlib
-from .fit_base import FitBase, log
-
-matplotlib.use("Agg")
-
-
-class GaussFit(FitBase):
-    """
-    This class makes a curve fitting using normal distribution
-    It reads data from a file given as the first argument.
-    The data file must contain at least two columns.
-    The first column represents x values,
-    the second and following columns are the y values.
-    """
-
-    def __init__(self, filename, **kwargs):
-        """
-        **Arguments:**
-
-        filename:
-            (string) Name of the file that contains data.
-
-        **Keyword arguments:**
-
-        guess:
-            (tuple) Guess of the optimal parameters for the model.
-        """
-
-        self.common_init(filename, **kwargs)
-        self.type_of_fit = "Normal distribution"
-        self.label_type = "gauss_fit"
-
-    def model_function(self, x, *args, **kwargs):
-        """Depends on the module."""
-        if len(args) != 3:
-            raise TypeError("Wrong amount of guess parameters passed")
-        A, mu, sig = args
-        return A * np.exp(-((x - mu) ** 2) / sig**2)
-
-    def default_guess(self, context):
-        """Default guess adequate for the model function."""
-        guess = [2, 2, 3]
-
-        return guess
-
-    def random_guess(self, context):
-        """
-        Random guess adequate for the model function with constraints
-        chosen by the user.
-        """
-        if self.auto_range is None:
-
-            guess = [
-                random.uniform(-60, 60),
-                random.uniform(-60, 60),
-                random.uniform(-60, 60),
-            ]
-        else:
-            guess = [
-                random.uniform(min_val, max_val)
-                for min_val, max_val in self.auto_range
-            ]
-
-        return guess
-
-    def print_info(self, popt):
-        """
-        Print info about popt in the format adequate for the model function.
-        """
-        name_temp = ("A", "mu", "sigma")
-        for el in range(3):
-            log(f"\t {name_temp[el]}: {popt[el]:2.8f}")
+
+# pylint: skip-file
+
+import pytest
+from random import seed
+from .common import check_list_within_percentage
+from pathlib import Path
+from .. import gauss
+
+
+def test_GaussFit_model_function():
+    "Test of the model function"
+    seed(1)
+    gauss_1 = gauss.GaussFit("exp.dat")
+    with pytest.raises(TypeError):
+        gauss_1.model_function(-1)
+    with pytest.raises(TypeError):
+        gauss_1.model_function(1, 2, 3, 4, 5)
+    assert gauss_1.model_function(22, 44, 66, 22) == 0.8058881111043039
+
+
+def test_GaussFit_results_file():
+    "Tests if pdf with the graph is found in results directory"
+    seed(1)
+    gauss_1 = gauss.GaussFit("gauss_data.txt")
+    gauss_1()
+    file_path = Path.cwd() / "minifit-results" / "gauss_fit_gauss_data_1.pdf"
+    assert file_path.exists(), f"File {file_path} does not exist"
+
+
+def test_GaussFit_popt():
+    "Testing if the popt found is accurate"
+    seed(1)
+    gauss_1 = gauss.GaussFit("gauss_data.txt")
+    gauss_1()
+    assert check_list_within_percentage(
+        gauss_1.popt, (4.97587424, 20.00233527, 2.84768795), 1
+    )
+    assert (
+        check_list_within_percentage(
+            gauss_1.popt, (4.97587424 * 1.1, 20.00233527, 2.84768795), 1
+        )
+        is not True
+    )
+    # first element differes by 10%, arrays should not be considered equal if precison is set to 1%
+
+
+def test_GaussFit_precision():
+    """Testing precision of the fit"""
+    seed(1)
+    gauss_1 = gauss.GaussFit("gauss_data.txt")
+    gauss_1()
+    assert gauss_1.sq_root_error <= 10
```

### Comparing `minifit-1.0.2/src/minifit/morse.py` & `minifit-1.0.3/src/minifit/morse.py`

 * *Files 17% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 from .fit_base import FitBase, log
 
 matplotlib.use("Agg")
 
 
 class MorseFit(FitBase):
     """
-    This class makes curve fitting using morse potential formula.
+    This class makes curve fitting using the morse potential formula.
     It reads data from a file given as the first argument.
     The data file must contain at least two columns.
     The first column represents x values,
     the second and following columns are the y values.
     """
 
     def __init__(self, filename, **kwargs):
@@ -43,26 +43,40 @@
 
         filename:
             (string) Name of the file that contains data.
 
         **Keyword arguments:**
 
         guess:
-            (tuple) Guess of the optimal parameters for the model.
+            (tuple) A guess of the optimal parameters for the model.
+            The number of guesses should match
+            the arguments that the model function expects.
+            For ax^2 + bx + c it expects (val1, val2, val3) etc.
+            Otherwise, an exception will be raised. If not passed, a default guess adequate for
+            the model function will be used.
         auto_guess:
             (bool) If true, tries to fit until chosen precision is reached. Default false.
-        range_auto:
-            (tuple) Sets boundaries for each parameter of guess.
-            If not set, default range is used.
+        auto_range:
+            (tuple) Sets boundaries for each parameter of the guess.
+            If not set, the default range is used. Only used if auto_guess is True.
+            Instead of guess = (5., 10., -3.)
+            pass auto_range = ((0.,10.), (5., 15.), (-40., 30.))
+            If fitting takes a lot of time, giving a better range might be helpful.
         precision:
-            Used by auto_guess. Default 0.4
+            (float) Used by auto_guess. Default 0.4. Only used if auto_guess is True.
+            If auto_guess is True and fitting takes a lot of time, lowering the precision may be
+            necessary for convergence. Lowering the precision will make the fitting process faster,
+            but the quality of popt may be worse.
         shift:
             (bool) If true, shifts the data. Default false.
+                Data can be shifted and it may
+                make the convergence of the least squares algorithm easier.
         """
-        self.common_init(filename, **kwargs)
+
+        super().__init__(filename, **kwargs)
         self.type_of_fit = "Morse"
         self.label_type = "morse_fit"
 
     def model_function(self, x, *args, **kwargs):
         """Depends on the module."""
         if len(args) != 9:
             raise TypeError("Wrong amount of guess parameters passed")
```

### Comparing `minifit-1.0.2/src/minifit/poly.py` & `minifit-1.0.3/src/minifit/gauss.py`

 * *Files 20% similar despite different names*

```diff
@@ -13,29 +13,27 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, see <http://www.gnu.org/licenses/>
 #
 """
-Module containing PolyFit class for curve fitting with polynomials.
+Module containing GaussFit class for curve fitting with normal distribution.
 """
 import random
+import numpy as np
 import matplotlib
-import numpy as np  # pylint: disable=W0611
 from .fit_base import FitBase, log
 
-
 matplotlib.use("Agg")
 
 
-class PolyFit(FitBase):
+class GaussFit(FitBase):
     """
-    This class makes a polynomial curve fitting.
-    Order of the polynomial can be chosen.
+    This class makes a curve fitting using the normal distribution
     It reads data from a file given as the first argument.
     The data file must contain at least two columns.
     The first column represents x values,
     the second and following columns are the y values.
     """
 
     def __init__(self, filename, **kwargs):
@@ -44,63 +42,76 @@
 
         filename:
             (string) Name of the file that contains data.
 
         **Keyword arguments:**
 
         guess:
-            (tuple) Guess of the optimal parameters for the model.
-        order:
-            (int) Order of the polynomial. Optional. Default 1
-        """
-
-        if kwargs.get("order") is None:
-            log("=")
-            log("Order of the polynomial wasn't given. Using default (1)")
-            self.order = 1
-        else:
-            self.order = kwargs.get("order")
-        self.common_init(filename, **kwargs)
-        self.type_of_fit = "Polynomials"
-        self.label_type = "polynomial_fit"
+            (tuple) A guess of the optimal parameters for the model.
+            The number of guesses should match
+            the arguments that the model function expects.
+            For ax^2 + bx + c it expects (val1, val2, val3) etc.
+            Otherwise, an exception will be raised. If not passed, a default guess adequate for
+            the model function will be used.
+        auto_guess:
+            (bool) If true, tries to fit until chosen precision is reached. Default false.
+        auto_range:
+            (tuple) Sets boundaries for each parameter of the guess.
+            If not set, the default range is used. Only used if auto_guess is True.
+            Instead of guess = (5., 10., -3.)
+            pass auto_range = ((0.,10.), (5., 15.), (-40., 30.))
+            If fitting takes a lot of time, giving a better range might be helpful.
+        precision:
+            (float) Used by auto_guess. Default 0.4. Only used if auto_guess is True.
+            If auto_guess is True and fitting takes a lot of time, lowering the precision may be
+            necessary for convergence. Lowering the precision will make the fitting process faster,
+            but the quality of popt may be worse.
+        shift:
+            (bool) If true, shifts the data. Default false.
+                Data can be shifted and it may
+                make the convergence of the least squares algorithm easier.
+        """
+
+        super().__init__(filename, **kwargs)
+        self.type_of_fit = "Normal distribution"
+        self.label_type = "gauss_fit"
 
     def model_function(self, x, *args, **kwargs):
         """Depends on the module."""
-        if len(args) != self.order + 1:
+        if len(args) != 3:
             raise TypeError("Wrong amount of guess parameters passed")
-        val = 0.0
-        # a + b*x + c*x^2 + etc.
-        for exp in range(self.order + 1):
-            val += args[exp] * x**exp
-        return val
+        A, mu, sig = args
+        return A * np.exp(-((x - mu) ** 2) / sig**2)
 
     def default_guess(self, context):
         """Default guess adequate for the model function."""
-        guess = []
-        for _ in range(self.order + 1):
-            guess.append(1.0)
+        guess = [2, 2, 3]
+
         return guess
 
     def random_guess(self, context):
         """
         Random guess adequate for the model function with constraints
         chosen by the user.
         """
         if self.auto_range is None:
-            guess = []
-            for _ in range(self.order + 1):
-                guess.append(random.uniform(-150, 150))
 
+            guess = [
+                random.uniform(-60, 60),
+                random.uniform(-60, 60),
+                random.uniform(-60, 60),
+            ]
         else:
             guess = [
                 random.uniform(min_val, max_val)
                 for min_val, max_val in self.auto_range
             ]
 
         return guess
 
     def print_info(self, popt):
         """
         Print info about popt in the format adequate for the model function.
         """
-        for el in range(self.order + 1):
-            log(f"\t {el}: {self.popt[el]:2.8f}")
+        name_temp = ("A", "mu", "sigma")
+        for el in range(3):
+            log(f"\t {name_temp[el]}: {popt[el]:2.8f}")
```

### Comparing `minifit-1.0.2/src/minifit/tests/__init__.py` & `minifit-1.0.3/src/minifit/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `minifit-1.0.2/src/minifit/tests/common.py` & `minifit-1.0.3/src/minifit/tests/common.py`

 * *Files identical despite different names*

### Comparing `minifit-1.0.2/src/minifit/tests/test_exponential.py` & `minifit-1.0.3/src/minifit/tests/test_exponential.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,43 +21,56 @@
 # along with this program; if not, see <http://www.gnu.org/licenses/>
 #
 
 # pylint: skip-file
 
 
 import pytest
+from random import seed
 from .common import check_list_within_percentage
 from pathlib import Path
 from .. import exp
 
 
-def test_ExponentialFit():
-    """Simple general test"""
+def test_ExponentialFit_model_function():
+    "Test of the model function"
+    seed(1)
+    exp_1 = exp.ExponentialFit("exp.dat")
+    with pytest.raises(TypeError):
+        exp_1.model_function(-1)
+    with pytest.raises(TypeError):
+        exp_1.model_function(1, 2, 3, 4, 5)
+    assert exp_1.model_function(3, 4, 2, -1000) == 613.7151739709404
+
+
+def test_ExponentialFit_results_file():
+    "Tests if pdf with the graph is found in results directory"
+    seed(1)
     exp_1 = exp.ExponentialFit("exp.dat")
     exp_1()
-    assert exp_1.sq_root_error <= 20
     file_path = Path.cwd() / "minifit-results" / "exp_fit_exp_1.pdf"
     assert file_path.exists(), f"File {file_path} does not exist"
 
 
-def test_popt_ExponentialFit():
+def test_ExponentialFit_popt():
+    "Testing if the popt found is accurate"
+    seed(1)
     exp_1 = exp.ExponentialFit("exp.dat")
     exp_1()
     assert check_list_within_percentage(
         exp_1.popt, (2.70136445, 0.48028958, 0.79216127), 1
     )
     assert (
         check_list_within_percentage(
             exp_1.popt, (2.70136445 * 1.1, 0.48028958, 0.79216127), 1
         )
         is not True
     )
     # first element differes by 10%, arrays should not be considered equal if precison is set to 1%
 
 
-def test_ExponentialFit_model_function():
+def test_ExponentialFit_precision():
+    """Testing precision of the fit"""
+    seed(1)
     exp_1 = exp.ExponentialFit("exp.dat")
-    with pytest.raises(TypeError):
-        exp_1.model_function(-1)
-    with pytest.raises(TypeError):
-        exp_1.model_function(1, 2, 3, 4, 5)
-    assert exp_1.model_function(3, 4, 2, -1000) == 613.7151739709404
+    exp_1()
+    assert exp_1.sq_root_error <= 20
```

### Comparing `minifit-1.0.2/src/minifit/tests/test_lennard_jones.py` & `minifit-1.0.3/src/minifit/tests/test_lennard_jones.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,35 +18,49 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, see <http://www.gnu.org/licenses/>
 #
 
 import pytest
+from random import seed
 from .common import check_list_within_percentage
 from pathlib import Path
 from .. import lennard_jones
 
 # pylint: skip-file
 
 
-def test_LennardJonesFit():
-    """Simple general test"""
+def test_LennardJonesFit_model_function():
+    seed(1)
+    "Tests of the model function"
+    l_j_1 = lennard_jones.LennardJonesFit("exp.dat")
+    with pytest.raises(TypeError):
+        l_j_1.model_function(-1)
+    with pytest.raises(TypeError):
+        l_j_1.model_function(1, 2, 3, 4)
+    assert l_j_1.model_function(0.01, 0.02, 0.039) == 628.992
+
+
+def test_LennardJonesFit_results_file():
+    seed(1)
+    "Tests if the pdf with the graph is found in the results directory"
     l_j_1 = lennard_jones.LennardJonesFit(
         "foo_data.txt", auto_guess=True, precision=5, shift=True
     )
     l_j_1()
-    assert l_j_1.sq_root_error <= 10
     file_path = (
         Path.cwd() / "minifit-results" / "lennard_jones_fit_foo_data_2.pdf"
     )
     assert file_path.exists(), f"File {file_path} does not exist"
 
 
-def test_popt_LennardJonesFit():
+def test_LennardJonesFit_popt():
+    "Testing if the popt found is accurate"
+    seed(1)
     l_j_1 = lennard_jones.LennardJonesFit(
         "foo_data.txt", auto_guess=False, guess=(0.75, 0.26), shift=True
     )
     l_j_1()
     assert check_list_within_percentage(
         l_j_1.popt, (0.75353688, 0.26085384), 10
     )
@@ -55,14 +69,15 @@
             l_j_1.popt, (0.75353688 * 1.1, 0.26085384), 1
         )
         is not True
     )
     # first element differes by 10%, arrays should not be considered equal if precison is set to 1%
 
 
-def test_LennardJonesFit_model_function():
-    l_j_1 = lennard_jones.LennardJonesFit("exp.dat")
-    with pytest.raises(TypeError):
-        l_j_1.model_function(-1)
-    with pytest.raises(TypeError):
-        l_j_1.model_function(1, 2, 3, 4)
-    assert l_j_1.model_function(0.01, 0.02, 0.039) == 628.992
+def test_LennardJonesFit_precision():
+    seed(1)
+    """Testing precision of the fit"""
+    l_j_1 = lennard_jones.LennardJonesFit(
+        "foo_data.txt", auto_guess=True, precision=5, shift=True
+    )
+    l_j_1()
+    assert l_j_1.sq_root_error <= 10
```

### Comparing `minifit-1.0.2/src/minifit/tests/test_morse.py` & `minifit-1.0.3/src/minifit/tests/test_morse.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,34 +20,62 @@
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, see <http://www.gnu.org/licenses/>
 #
 
 # pylint: skip-file
 
 import pytest
+from random import seed
 from .common import check_list_within_percentage
 from pathlib import Path
 from .. import morse
 
 
-def test_MorseFit():
-    """Simple general test"""
+def test_MorseFit_model_function():
+    "Tests of the model function"
+    seed(1)
+    morse_1 = morse.MorseFit("exp.dat")
+    with pytest.raises(TypeError):
+        morse_1.model_function(-1)
+    with pytest.raises(TypeError):
+        morse_1.model_function(1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11)
+    assert (
+        morse_1.model_function(
+            0.06,
+            0.05,  # re
+            0.1,  # de
+            10.0,  # b0
+            0.1,  # b1
+            0.1,  # b2
+            0.001,  # b3
+            0.001,  # b4
+            0.0001,  # b5
+            0.000001,  # b6
+        )
+        == -0.007570818470665069
+    )
+
+
+def test_MorseFit_results_file():
+    "Tests if the pdf with the graph is found in the results directory"
+    seed(1)
     morse_1 = morse.MorseFit(
         "foo_data.txt",
         auto_guess=True,
         precision=5,
         shift=True,
     )
     morse_1()
-    assert morse_1.sq_root_error <= 6
     file_path = Path.cwd() / "minifit-results" / "morse_fit_foo_data_2.pdf"
     assert file_path.exists(), f"File {file_path} does not exist"
 
 
-def test_popt_MorseFit():
+def test_MorseFit_popt():
+    "Testing if the popt found is accurate"
+    seed(1)
     morse_1 = morse.MorseFit(
         "foo_data.txt",
         auto_guess=True,
         precision=0.1,
         shift=True,
     )
     morse_1()
@@ -85,28 +113,18 @@
             1,
         )
         is not True
     )
     # first element differes by 10%, arrays should not be considered equal if precison is set to 1%
 
 
-def test_MorseFit_model_function():
-    morse_1 = morse.MorseFit("exp.dat")
-    with pytest.raises(TypeError):
-        morse_1.model_function(-1)
-    with pytest.raises(TypeError):
-        morse_1.model_function(1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11)
-    assert (
-        morse_1.model_function(
-            0.06,
-            0.05,  # re
-            0.1,  # de
-            10.0,  # b0
-            0.1,  # b1
-            0.1,  # b2
-            0.001,  # b3
-            0.001,  # b4
-            0.0001,  # b5
-            0.000001,
-        )
-        == -0.007570818470665069
+def test_MorseFit_precision():
+    """Testing precision of the fit"""
+    seed(1)
+    morse_1 = morse.MorseFit(
+        "foo_data.txt",
+        auto_guess=True,
+        precision=0.1,
+        shift=True,
     )
+    morse_1()
+    assert morse_1.sq_root_error <= 0.1
```

### Comparing `minifit-1.0.2/src/minifit/tests/test_poly.py` & `minifit-1.0.3/src/minifit/tests/test_poly.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,29 +20,46 @@
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, see <http://www.gnu.org/licenses/>
 #
 
 # pylint: skip-file
 
 import pytest
+from random import seed
 from .common import check_list_within_percentage
 from pathlib import Path
 from .. import poly
 
 
-def test_PolyFit():
-    """Simple general test"""
+def test_PolyFit_model_function():
+    """Tests for model function"""
+    seed(1)
+    poly_1 = poly.PolyFit("exp.dat", order=7)
+    with pytest.raises(TypeError):
+        poly_1.model_function(-1)
+    with pytest.raises(TypeError):
+        poly_1.model_function(1, 2, 3, 4, 5, 6, 7, 8, 9, 10)
+    assert (
+        poly_1.model_function(-5, -1, -2, -3, 4, 5, 0.003, 0.03, 25000)
+        == -1953121981.625
+    )
+
+
+def test_PolyFit_results_file():
+    "Tests if the pdf with the graph is found in the results directory"
+    seed(1)
     poly_1 = poly.PolyFit("example.dat", order=7)
     poly_1()
-    assert poly_1.sq_root_error <= 6
     file_path = Path.cwd() / "minifit-results" / "polynomial_fit_example_3.pdf"
     assert file_path.exists(), f"File {file_path} does not exist"
 
 
-def test_popt_PolyFit():
+def test_PolyFit_popt():
+    "Testing if the popt found is accurate"
+    seed(1)
     poly_1 = poly.PolyFit("example.dat", order=7)
     poly_1()
     assert check_list_within_percentage(
         poly_1.popt,
         (
             -39.0169376799999981,
             -305.9215619700000275,
@@ -71,18 +88,13 @@
             1,
         )
         is not True
     )
     # first element differes by 10%, arrays should not be considered equal if precison is set to 1%
 
 
-def test_PolyFit_model_function():
-    """Tests for model function"""
-    poly_1 = poly.PolyFit("exp.dat", order=7)
-    with pytest.raises(TypeError):
-        poly_1.model_function(-1)
-    with pytest.raises(TypeError):
-        poly_1.model_function(1, 2, 3, 4, 5, 6, 7, 8, 9, 10)
-    assert (
-        poly_1.model_function(-5, -1, -2, -3, 4, 5, 0.003, 0.03, 25000)
-        == -1953121981.625
-    )
+def test_PolyFit_precision():
+    """Testing precision of the fit"""
+    seed(1)
+    poly_1 = poly.PolyFit("example.dat", order=7)
+    poly_1()
+    assert poly_1.sq_root_error <= 6
```

### Comparing `minifit-1.0.2/src/minifit/tests/test_user.py` & `minifit-1.0.3/src/minifit/tests/test_user.py`

 * *Files 26% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, see <http://www.gnu.org/licenses/>
 #
 
 # pylint: skip-file
 
 import pytest
+from random import seed
 from .common import check_list_within_percentage
 from pathlib import Path
 from .. import user_defined
 
 
 def user_poly(x, *args, **kwargs):
     a, b, c, d, e, f, g, h = args
@@ -51,31 +52,33 @@
     (-593.05923681 - 50, -593.05923681 + 50),
     (568.07666599 - 50, 568.07666599 + 50),
     (-304.20455678 - 50, -304.20455678 + 50),
     (-39.28501939 - 50, -39.28501939 + 50),
 )
 
 
-def test_UserFit():
-    """Simple general test"""
+def test_PolyFit_results_file():
+    "Tests if pdf with the graph is found in results directory"
+    seed(1)
     user_1 = user_defined.UserFit(
         "example.dat",
         model=user_poly,
         num_param=8,
         auto_guess=True,
         precision=0.01,
         auto_range=a_range,
     )
     user_1()
-    assert user_1.sq_root_error <= 1
     file_path = Path.cwd() / "minifit-results" / "user_fit_example_1.pdf"
     assert file_path.exists(), f"File {file_path} does not exist"
 
 
-def test_popt_UserFit():
+def test_UserFit_popt():
+    "Testing if the popt found is accurate"
+    seed(1)
     user_1 = user_defined.UserFit(
         "example.dat",
         model=user_poly,
         num_param=8,
         auto_guess=True,
         precision=0.01,
         auto_range=a_range,
@@ -110,7 +113,22 @@
                 -39.28501939,
             ),
             1,
         )
         is not True
     )
     # first element differes by 10%, arrays should not be considered equal if precison is set to 1%
+
+
+def test_UserFit_precision():
+    """Testing precision of the fit"""
+    seed(1)
+    user_1 = user_defined.UserFit(
+        "example.dat",
+        model=user_poly,
+        num_param=8,
+        auto_guess=True,
+        precision=0.01,
+        auto_range=a_range,
+    )
+    user_1()
+    assert user_1.sq_root_error <= 1
```

### Comparing `minifit-1.0.2/src/minifit/user_defined.py` & `minifit-1.0.3/src/minifit/poly.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,30 +13,29 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, see <http://www.gnu.org/licenses/>
 #
 """
-Module containing MorseFit class for curve fitting with morse.
+Module containing PolyFit class for curve fitting with polynomials.
 """
-
-
 import random
 import matplotlib
 import numpy as np  # pylint: disable=W0611
 from .fit_base import FitBase, log
 
 
 matplotlib.use("Agg")
 
 
-class UserFit(FitBase):
+class PolyFit(FitBase):
     """
-    This class makes curve fitting using morse potential formula.
+    This class makes a polynomial curve fitting.
+    Order of the polynomial can be chosen.
     It reads data from a file given as the first argument.
     The data file must contain at least two columns.
     The first column represents x values,
     the second and following columns are the y values.
     """
 
     def __init__(self, filename, **kwargs):
@@ -44,82 +43,87 @@
         **Arguments:**
 
         filename:
             (string) Name of the file that contains data.
 
         **Keyword arguments:**
 
-        num_param:
-            (int) Number of parameters of user defined model function.
-        model:
-            (function/callable) An object that expects (x, *args, **kwargs)
-            and returns y value for given arguments
+        order:
+            (int) Unique for PolyFit. Order of the polynomial. Optional. Default 1.
+
         guess:
-            (tuple) Guess of the optimal parameters for the model.
+            (tuple) A guess of the optimal parameters for the model.
+            The number of guesses should match
+            the arguments that the model function expects.
+            For ax^2 + bx + c it expects (val1, val2, val3) etc.
+            Otherwise, an exception will be raised. If not passed, a default guess adequate for
+            the model function will be used.
         auto_guess:
             (bool) If true, tries to fit until chosen precision is reached. Default false.
-        range_auto:
-            (tuple) Sets boundaries for each parameter of guess.
-            If not set, default range is used.
+        auto_range:
+            (tuple) Sets boundaries for each parameter of the guess.
+            If not set, the default range is used. Only used if auto_guess is True.
+            Instead of guess = (5., 10., -3.)
+            pass auto_range = ((0.,10.), (5., 15.), (-40., 30.))
+            If fitting takes a lot of time, giving a better range might be helpful.
         precision:
-            Used by auto_guess. Default 0.4
+            (float) Used by auto_guess. Default 0.4. Only used if auto_guess is True.
+            If auto_guess is True and fitting takes a lot of time, lowering the precision may be
+            necessary for convergence. Lowering the precision will make the fitting process faster,
+            but the quality of popt may be worse.
         shift:
             (bool) If true, shifts the data. Default false.
+                Data can be shifted and it may
+                make the convergence of the least squares algorithm easier.
         """
-        self.common_init(filename, **kwargs)
 
-        self.type_of_fit = kwargs.get("type_of_fit", "User defined function")
-        self.label_type = kwargs.get("label_type", "user_fit")
-        num_param = kwargs.get("num_param")
-        if num_param is None:
-            raise ValueError(
-                "Missing required parameter: num_param. How many parameters your functions has? Required for sanitazation"  # pylint: disable=C0301
-            )
-        self.num_param = num_param
-
-        user_def_func = kwargs.get("model")
-        if user_def_func is not None and callable(user_def_func):
-            # The object is a function
-            self.user_def_func = user_def_func
+        if kwargs.get("order") is None:
+            log("=")
+            log("Order of the polynomial wasn't given. Using default (1)")
+            self.order = 1
         else:
-            # The object is not a function or is None
-            raise ValueError(
-                "Missing required parameter: model. With what function do you want to fit?"
-            )
+            self.order = kwargs.get("order")
+        super().__init__(filename, **kwargs)
+        self.type_of_fit = "Polynomials"
+        self.label_type = "polynomial_fit"
 
     def model_function(self, x, *args, **kwargs):
         """Depends on the module."""
-        if len(args) != self.num_param:
+        if len(args) != self.order + 1:
             raise TypeError("Wrong amount of guess parameters passed")
-        return self.user_def_func(x, *args, **kwargs)
+        val = 0.0
+        # a + b*x + c*x^2 + etc.
+        for exp in range(self.order + 1):
+            val += args[exp] * x**exp
+        return val
 
     def default_guess(self, context):
         """Default guess adequate for the model function."""
         guess = []
-        for _ in range(self.num_param):
+        for _ in range(self.order + 1):
             guess.append(1.0)
         return guess
 
     def random_guess(self, context):
         """
         Random guess adequate for the model function with constraints
         chosen by the user.
         """
         if self.auto_range is None:
             guess = []
-            for _ in range(self.num_param):
+            for _ in range(self.order + 1):
                 guess.append(random.uniform(-150, 150))
 
         else:
             guess = [
                 random.uniform(min_val, max_val)
                 for min_val, max_val in self.auto_range
             ]
 
         return guess
 
     def print_info(self, popt):
         """
         Print info about popt in the format adequate for the model function.
         """
-        for el in range(self.num_param):
-            log(f"\t {el}: {popt[el]:2.8f}")
+        for el in range(self.order + 1):
+            log(f"\t {el}: {self.popt[el]:2.8f}")
```

### Comparing `minifit-1.0.2/src/minifit.egg-info/PKG-INFO` & `minifit-1.0.3/src/minifit.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: minifit
-Version: 1.0.2
+Version: 1.0.3
 Summary: MiniFit is a python package that can be used for fitting data.
 Home-page: https://gitlab.com/mike3.14/minifit
 Author: Michał Kopczyński
 Author-email: michal.kopczynski3.14@gmail.com
 Project-URL: repository, https://gitlab.com/mike3.14/minifit
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
```

### Comparing `minifit-1.0.2/src/minifit.egg-info/SOURCES.txt` & `minifit-1.0.3/src/minifit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

