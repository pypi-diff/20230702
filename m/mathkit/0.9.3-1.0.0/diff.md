# Comparing `tmp/mathkit-0.9.3.tar.gz` & `tmp/mathkit-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mathkit-0.9.3.tar", last modified: Sun Jul  2 03:39:18 2023, max compression
+gzip compressed data, was "mathkit-1.0.0.tar", last modified: Sun Jul  2 03:47:11 2023, max compression
```

## Comparing `mathkit-0.9.3.tar` & `mathkit-1.0.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-07-02 03:39:18.306041 mathkit-0.9.3/
--rw-rw-rw-   0        0        0     3466 2023-07-02 03:39:18.306041 mathkit-0.9.3/PKG-INFO
--rw-rw-rw-   0        0        0     3021 2023-07-02 02:47:56.000000 mathkit-0.9.3/README.md
-drwxrwxrwx   0        0        0        0 2023-07-02 03:39:18.273522 mathkit-0.9.3/mathkit/
--rw-rw-rw-   0        0        0      482 2023-07-02 03:38:48.000000 mathkit-0.9.3/mathkit/__init__.py
--rw-rw-rw-   0        0        0     5057 2023-07-02 01:46:47.000000 mathkit-0.9.3/mathkit/main.py
-drwxrwxrwx   0        0        0        0 2023-07-02 03:39:18.297891 mathkit-0.9.3/mathkit.egg-info/
--rw-rw-rw-   0        0        0     3466 2023-07-02 03:39:18.000000 mathkit-0.9.3/mathkit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      178 2023-07-02 03:39:18.000000 mathkit-0.9.3/mathkit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-02 03:39:18.000000 mathkit-0.9.3/mathkit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-07-02 03:39:18.000000 mathkit-0.9.3/mathkit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-02 03:39:18.306041 mathkit-0.9.3/setup.cfg
--rw-rw-rw-   0        0        0      712 2023-07-02 03:39:14.000000 mathkit-0.9.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-02 03:47:11.684589 mathkit-1.0.0/
+-rw-rw-rw-   0        0        0     3466 2023-07-02 03:47:11.684589 mathkit-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3021 2023-07-02 02:47:56.000000 mathkit-1.0.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-02 03:47:11.655924 mathkit-1.0.0/mathkit/
+-rw-rw-rw-   0        0        0      513 2023-07-02 03:44:28.000000 mathkit-1.0.0/mathkit/__init__.py
+-rw-rw-rw-   0        0        0     5813 2023-07-02 03:43:47.000000 mathkit-1.0.0/mathkit/main.py
+drwxrwxrwx   0        0        0        0 2023-07-02 03:47:11.680764 mathkit-1.0.0/mathkit.egg-info/
+-rw-rw-rw-   0        0        0     3466 2023-07-02 03:47:11.000000 mathkit-1.0.0/mathkit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      178 2023-07-02 03:47:11.000000 mathkit-1.0.0/mathkit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-02 03:47:11.000000 mathkit-1.0.0/mathkit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-07-02 03:47:11.000000 mathkit-1.0.0/mathkit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-02 03:47:11.684589 mathkit-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      712 2023-07-02 03:47:05.000000 mathkit-1.0.0/setup.py
```

### Comparing `mathkit-0.9.3/PKG-INFO` & `mathkit-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mathkit
-Version: 0.9.3
+Version: 1.0.0
 Summary: Python library for mathematical functions
 Home-page: https://github.com/theunkownhacker/mathkit
 Author: TheUnkownHacker
 Author-email: theunkownhacker@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mathkit-0.9.3/README.md` & `mathkit-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `mathkit-0.9.3/mathkit/main.py` & `mathkit-1.0.0/mathkit/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -157,7 +157,32 @@
 
 def sub(num1=None, num2=None):
     if num1 is None:
         num1 = int(input("Enter first number: "))
     if num2 is None:
         num2 = int(input("Enter second number: "))
     print("Your answer is", num1 - num2)
+
+def trig(num=None):
+    print("Trigonometry")
+    print("1. Sine")
+    print("2. Cosine")
+    print("3. Tangent")
+    print("4. Exit")
+    choice = int(input("Enter your choice: "))
+    if choice == 1:
+        if num is None:
+            num = float(input("Enter the number: "))
+        print("Sine of", num, "is", math.sin(num))
+    elif choice == 2:
+        if num is None:
+            num = float(input("Enter the number: "))
+        print("Cosine of", num, "is", math.cos(num))
+    elif choice == 3:
+        if num is None:
+            num = float(input("Enter the number: "))
+        print("Tangent of", num, "is", math.tan(num))
+    elif choice == 4:
+        exit()
+    else:
+        print("Invalid choice!")
+        trig()
```

### Comparing `mathkit-0.9.3/mathkit.egg-info/PKG-INFO` & `mathkit-1.0.0/mathkit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mathkit
-Version: 0.9.3
+Version: 1.0.0
 Summary: Python library for mathematical functions
 Home-page: https://github.com/theunkownhacker/mathkit
 Author: TheUnkownHacker
 Author-email: theunkownhacker@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mathkit-0.9.3/setup.py` & `mathkit-1.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="mathkit",
-    version="0.9.3",
+    version="1.0.0",
     author="TheUnkownHacker",
     author_email="theunkownhacker@gmail.com",
     description="Python library for mathematical functions",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/theunkownhacker/mathkit",
     packages=find_packages(),
```

