# Comparing `tmp/mathkit-0.2.2.tar.gz` & `tmp/mathkit-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mathkit-0.2.2.tar", last modified: Sun Jul  2 02:42:49 2023, max compression
+gzip compressed data, was "mathkit-0.9.1.tar", last modified: Sun Jul  2 02:48:56 2023, max compression
```

## Comparing `mathkit-0.2.2.tar` & `mathkit-0.9.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-07-02 02:42:49.766100 mathkit-0.2.2/
--rw-rw-rw-   0        0        0     3478 2023-07-02 02:42:49.761087 mathkit-0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     3039 2023-07-02 02:42:27.000000 mathkit-0.2.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-02 02:42:49.733549 mathkit-0.2.2/mathkit/
--rw-rw-rw-   0        0        0      467 2023-07-02 02:00:13.000000 mathkit-0.2.2/mathkit/__init__.py
--rw-rw-rw-   0        0        0     5057 2023-07-02 01:46:47.000000 mathkit-0.2.2/mathkit/main.py
-drwxrwxrwx   0        0        0        0 2023-07-02 02:42:49.761087 mathkit-0.2.2/mathkit.egg-info/
--rw-rw-rw-   0        0        0     3478 2023-07-02 02:42:49.000000 mathkit-0.2.2/mathkit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      178 2023-07-02 02:42:49.000000 mathkit-0.2.2/mathkit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-02 02:42:49.000000 mathkit-0.2.2/mathkit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-07-02 02:42:49.000000 mathkit-0.2.2/mathkit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-02 02:42:49.766100 mathkit-0.2.2/setup.cfg
--rw-rw-rw-   0        0        0      706 2023-07-02 02:42:44.000000 mathkit-0.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-02 02:48:56.377047 mathkit-0.9.1/
+-rw-rw-rw-   0        0        0     3460 2023-07-02 02:48:56.377047 mathkit-0.9.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3021 2023-07-02 02:47:56.000000 mathkit-0.9.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-02 02:48:56.318289 mathkit-0.9.1/mathkit/
+-rw-rw-rw-   0        0        0      467 2023-07-02 02:00:13.000000 mathkit-0.9.1/mathkit/__init__.py
+-rw-rw-rw-   0        0        0     5057 2023-07-02 01:46:47.000000 mathkit-0.9.1/mathkit/main.py
+drwxrwxrwx   0        0        0        0 2023-07-02 02:48:56.377047 mathkit-0.9.1/mathkit.egg-info/
+-rw-rw-rw-   0        0        0     3460 2023-07-02 02:48:56.000000 mathkit-0.9.1/mathkit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      178 2023-07-02 02:48:56.000000 mathkit-0.9.1/mathkit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-02 02:48:56.000000 mathkit-0.9.1/mathkit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-07-02 02:48:56.000000 mathkit-0.9.1/mathkit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-02 02:48:56.377047 mathkit-0.9.1/setup.cfg
+-rw-rw-rw-   0        0        0      706 2023-07-02 02:48:50.000000 mathkit-0.9.1/setup.py
```

### Comparing `mathkit-0.2.2/PKG-INFO` & `mathkit-0.9.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: mathkit
-Version: 0.2.2
+Version: 0.9.1
 Summary: Python library for mathematical functions
 Home-page: https://github.com/theunkownhacker/mathkit
 Author: Your Name
 Author-email: theunkownhacker@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
-##MathKit
+# MathKit
 
-MathKit is a Python library that provides various mathematical functions and utilities for performing common mathematical calculations.
+**MathKit is a Python library that provides various mathematical functions and utilities for performing common mathematical calculations.**
 
-##Example Usage
+## Example Usage
 
 ```python
 from mathkit import *
 
 print("Welcome to the Math Library!")
 print("1. Addition")
 print("2. Subtraction")
@@ -73,40 +73,27 @@
 elif choice == 16:
     exit()
 else:
     print("Invalid choice!")
     print("Press Enter to continue")
     input()
 ```
-##Example Usage If you decide to predefine numbers
+
+## Example Usage If you decide to predefine numbers
 
 ```python
 add(5, 3)  # Output: Your answer is 8
-
 cbrt(27)  # Output: The cube root of 27 is 3.0
-
 div(10, 2)  # Output: Your answer is 5.0
-
 fact(5)  # Output: The factorial of 5 is 120
-
 hcf(24, 36)  # Output: The H.C.F. of 24 and 36 is 12
-
 lcm(12, 18)  # Output: The LCM of 12 and 18 is 36
-
 log(100)  # Output: Logarithm of 100 (base e) is 4.605...
-
 mod(10, 3)  # Output: Your answer is 1
-
 mul(4, 5)  # Output: Product = 20
-
 per(50, 10)  # Output: 10 percent of 50 is 5
-
 power(2, 3)  # Output: The answer is: 8
-
 sqrt(25)  # Output: Square root of 25 is 5.0
-
 sqr(4)  # Output: The square of 4 is 16
-
 sub(8, 3)  # Output: Your answer is 5
 ```
-
-##For more information, please visit the GitHub repository.
+ ## For more information, please visit the GitHub repository.
```

### Comparing `mathkit-0.2.2/README.md` & `mathkit-0.9.1/mathkit.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,25 @@
-##MathKit
+Metadata-Version: 2.1
+Name: mathkit
+Version: 0.9.1
+Summary: Python library for mathematical functions
+Home-page: https://github.com/theunkownhacker/mathkit
+Author: Your Name
+Author-email: theunkownhacker@gmail.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
 
-MathKit is a Python library that provides various mathematical functions and utilities for performing common mathematical calculations.
+# MathKit
 
-##Example Usage
+**MathKit is a Python library that provides various mathematical functions and utilities for performing common mathematical calculations.**
+
+## Example Usage
 
 ```python
 from mathkit import *
 
 print("Welcome to the Math Library!")
 print("1. Addition")
 print("2. Subtraction")
@@ -60,40 +73,27 @@
 elif choice == 16:
     exit()
 else:
     print("Invalid choice!")
     print("Press Enter to continue")
     input()
 ```
-##Example Usage If you decide to predefine numbers
+
+## Example Usage If you decide to predefine numbers
 
 ```python
 add(5, 3)  # Output: Your answer is 8
-
 cbrt(27)  # Output: The cube root of 27 is 3.0
-
 div(10, 2)  # Output: Your answer is 5.0
-
 fact(5)  # Output: The factorial of 5 is 120
-
 hcf(24, 36)  # Output: The H.C.F. of 24 and 36 is 12
-
 lcm(12, 18)  # Output: The LCM of 12 and 18 is 36
-
 log(100)  # Output: Logarithm of 100 (base e) is 4.605...
-
 mod(10, 3)  # Output: Your answer is 1
-
 mul(4, 5)  # Output: Product = 20
-
 per(50, 10)  # Output: 10 percent of 50 is 5
-
 power(2, 3)  # Output: The answer is: 8
-
 sqrt(25)  # Output: Square root of 25 is 5.0
-
 sqr(4)  # Output: The square of 4 is 16
-
 sub(8, 3)  # Output: Your answer is 5
 ```
-
-##For more information, please visit the GitHub repository.
+ ## For more information, please visit the GitHub repository.
```

### Comparing `mathkit-0.2.2/mathkit/main.py` & `mathkit-0.9.1/mathkit/main.py`

 * *Files identical despite different names*

### Comparing `mathkit-0.2.2/setup.py` & `mathkit-0.9.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="mathkit",
-    version="0.2.2",
+    version="0.9.1",
     author="Your Name",
     author_email="theunkownhacker@gmail.com",
     description="Python library for mathematical functions",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/theunkownhacker/mathkit",
     packages=find_packages(),
```

