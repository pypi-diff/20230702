# Comparing `tmp/mathkit-0.2.tar.gz` & `tmp/mathkit-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mathkit-0.2.tar", last modified: Sun Jul  2 02:31:44 2023, max compression
+gzip compressed data, was "mathkit-0.2.1.tar", last modified: Sun Jul  2 02:36:18 2023, max compression
```

## Comparing `mathkit-0.2.tar` & `mathkit-0.2.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-07-02 02:31:44.775533 mathkit-0.2/
--rw-rw-rw-   0        0        0     3834 2023-07-02 02:31:44.775533 mathkit-0.2/PKG-INFO
--rw-rw-rw-   0        0        0     3397 2023-07-02 02:29:33.000000 mathkit-0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-02 02:31:44.745838 mathkit-0.2/mathkit/
--rw-rw-rw-   0        0        0      467 2023-07-02 02:00:13.000000 mathkit-0.2/mathkit/__init__.py
--rw-rw-rw-   0        0        0     5057 2023-07-02 01:46:47.000000 mathkit-0.2/mathkit/main.py
-drwxrwxrwx   0        0        0        0 2023-07-02 02:31:44.770213 mathkit-0.2/mathkit.egg-info/
--rw-rw-rw-   0        0        0     3834 2023-07-02 02:31:44.000000 mathkit-0.2/mathkit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      178 2023-07-02 02:31:44.000000 mathkit-0.2/mathkit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-02 02:31:44.000000 mathkit-0.2/mathkit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-07-02 02:31:44.000000 mathkit-0.2/mathkit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-02 02:31:44.778041 mathkit-0.2/setup.cfg
--rw-rw-rw-   0        0        0      704 2023-07-02 02:31:22.000000 mathkit-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-02 02:36:17.994381 mathkit-0.2.1/
+-rw-rw-rw-   0        0        0     3456 2023-07-02 02:36:17.994381 mathkit-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3017 2023-07-02 02:35:21.000000 mathkit-0.2.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-02 02:36:17.970433 mathkit-0.2.1/mathkit/
+-rw-rw-rw-   0        0        0      467 2023-07-02 02:00:13.000000 mathkit-0.2.1/mathkit/__init__.py
+-rw-rw-rw-   0        0        0     5057 2023-07-02 01:46:47.000000 mathkit-0.2.1/mathkit/main.py
+drwxrwxrwx   0        0        0        0 2023-07-02 02:36:17.994381 mathkit-0.2.1/mathkit.egg-info/
+-rw-rw-rw-   0        0        0     3456 2023-07-02 02:36:17.000000 mathkit-0.2.1/mathkit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      178 2023-07-02 02:36:17.000000 mathkit-0.2.1/mathkit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-02 02:36:17.000000 mathkit-0.2.1/mathkit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-07-02 02:36:17.000000 mathkit-0.2.1/mathkit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-02 02:36:17.994381 mathkit-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      706 2023-07-02 02:36:15.000000 mathkit-0.2.1/setup.py
```

### Comparing `mathkit-0.2/PKG-INFO` & `mathkit-0.2.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: mathkit
-Version: 0.2
+Version: 0.2.1
 Summary: Python library for mathematical functions
 Home-page: https://github.com/theunkownhacker/mathkit
 Author: Your Name
 Author-email: theunkownhacker@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
-MathKit
+# MathKit
+
 MathKit is a Python library that provides various mathematical functions and utilities for performing common mathematical calculations.
 
-Example Usage
-================================================================================================
-================================================================================================
+## Example Usage
 
+```python
 from mathkit import *
 
 print("Welcome to the Math Library!")
 print("1. Addition")
 print("2. Subtraction")
 print("3. Multiplication")
 print("4. Division")
@@ -73,20 +73,16 @@
 elif choice == 16:
     exit()
 else:
     print("Invalid choice!")
     print("Press Enter to continue")
     input()
 
-================================================================================================
-================================================================================================
-
 Example Usage If you decide to predefine numbers
 
-
 add(5, 3)  # Output: Your answer is 8
 
 cbrt(27)  # Output: The cube root of 27 is 3.0
 
 div(10, 2)  # Output: Your answer is 5.0
 
 fact(5)  # Output: The factorial of 5 is 120
@@ -107,9 +103,8 @@
 
 sqrt(25)  # Output: Square root of 25 is 5.0
 
 sqr(4)  # Output: The square of 4 is 16
 
 sub(8, 3)  # Output: Your answer is 5
 
-
 For more information, please visit the GitHub repository.
```

### Comparing `mathkit-0.2/README.md` & `mathkit-0.2.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-MathKit
+# MathKit
+
 MathKit is a Python library that provides various mathematical functions and utilities for performing common mathematical calculations.
 
-Example Usage
-================================================================================================
-================================================================================================
+## Example Usage
 
+```python
 from mathkit import *
 
 print("Welcome to the Math Library!")
 print("1. Addition")
 print("2. Subtraction")
 print("3. Multiplication")
 print("4. Division")
@@ -60,20 +60,16 @@
 elif choice == 16:
     exit()
 else:
     print("Invalid choice!")
     print("Press Enter to continue")
     input()
 
-================================================================================================
-================================================================================================
-
 Example Usage If you decide to predefine numbers
 
-
 add(5, 3)  # Output: Your answer is 8
 
 cbrt(27)  # Output: The cube root of 27 is 3.0
 
 div(10, 2)  # Output: Your answer is 5.0
 
 fact(5)  # Output: The factorial of 5 is 120
@@ -94,9 +90,8 @@
 
 sqrt(25)  # Output: Square root of 25 is 5.0
 
 sqr(4)  # Output: The square of 4 is 16
 
 sub(8, 3)  # Output: Your answer is 5
 
-
 For more information, please visit the GitHub repository.
```

### Comparing `mathkit-0.2/mathkit/main.py` & `mathkit-0.2.1/mathkit/main.py`

 * *Files identical despite different names*

### Comparing `mathkit-0.2/mathkit.egg-info/PKG-INFO` & `mathkit-0.2.1/mathkit.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: mathkit
-Version: 0.2
+Version: 0.2.1
 Summary: Python library for mathematical functions
 Home-page: https://github.com/theunkownhacker/mathkit
 Author: Your Name
 Author-email: theunkownhacker@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
-MathKit
+# MathKit
+
 MathKit is a Python library that provides various mathematical functions and utilities for performing common mathematical calculations.
 
-Example Usage
-================================================================================================
-================================================================================================
+## Example Usage
 
+```python
 from mathkit import *
 
 print("Welcome to the Math Library!")
 print("1. Addition")
 print("2. Subtraction")
 print("3. Multiplication")
 print("4. Division")
@@ -73,20 +73,16 @@
 elif choice == 16:
     exit()
 else:
     print("Invalid choice!")
     print("Press Enter to continue")
     input()
 
-================================================================================================
-================================================================================================
-
 Example Usage If you decide to predefine numbers
 
-
 add(5, 3)  # Output: Your answer is 8
 
 cbrt(27)  # Output: The cube root of 27 is 3.0
 
 div(10, 2)  # Output: Your answer is 5.0
 
 fact(5)  # Output: The factorial of 5 is 120
@@ -107,9 +103,8 @@
 
 sqrt(25)  # Output: Square root of 25 is 5.0
 
 sqr(4)  # Output: The square of 4 is 16
 
 sub(8, 3)  # Output: Your answer is 5
 
-
 For more information, please visit the GitHub repository.
```

### Comparing `mathkit-0.2/setup.py` & `mathkit-0.2.1/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="mathkit",
-    version="0.2",
+    version="0.2.1",
     author="Your Name",
     author_email="theunkownhacker@gmail.com",
     description="Python library for mathematical functions",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/theunkownhacker/mathkit",
     packages=find_packages(),
```

