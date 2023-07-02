# Comparing `tmp/ngrad-1.0.2.tar.gz` & `tmp/ngrad-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ngrad-1.0.2.tar", last modified: Fri Jun  2 07:15:51 2023, max compression
+gzip compressed data, was "ngrad-1.0.3.tar", last modified: Sun Jul  2 05:13:15 2023, max compression
```

## Comparing `ngrad-1.0.2.tar` & `ngrad-1.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 x0axz     (1000) x0axz     (1000)        0 2023-06-02 07:15:51.851438 ngrad-1.0.2/
--rw-rw-r--   0 x0axz     (1000) x0axz     (1000)     1061 2023-05-30 18:26:38.000000 ngrad-1.0.2/LICENSE
--rw-rw-r--   0 x0axz     (1000) x0axz     (1000)     3963 2023-06-02 07:15:51.847439 ngrad-1.0.2/PKG-INFO
--rw-rw-r--   0 x0axz     (1000) x0axz     (1000)     3462 2023-06-01 16:52:46.000000 ngrad-1.0.2/README.md
-drwxrwxr-x   0 x0axz     (1000) x0axz     (1000)        0 2023-06-02 07:15:51.835440 ngrad-1.0.2/ngrad/
--rw-rw-r--   0 x0axz     (1000) x0axz     (1000)        0 2023-05-29 09:04:57.000000 ngrad-1.0.2/ngrad/__init__.py
--rw-rw-r--   0 x0axz     (1000) x0axz     (1000)     5054 2023-06-02 07:10:55.000000 ngrad-1.0.2/ngrad/engine.py
--rw-rw-r--   0 x0axz     (1000) x0axz     (1000)     1898 2023-06-02 07:10:35.000000 ngrad-1.0.2/ngrad/library.py
-drwxrwxr-x   0 x0axz     (1000) x0axz     (1000)        0 2023-06-02 07:15:51.847439 ngrad-1.0.2/ngrad.egg-info/
--rw-rw-r--   0 x0axz     (1000) x0axz     (1000)     3963 2023-06-02 07:15:51.000000 ngrad-1.0.2/ngrad.egg-info/PKG-INFO
--rw-rw-r--   0 x0axz     (1000) x0axz     (1000)      241 2023-06-02 07:15:51.000000 ngrad-1.0.2/ngrad.egg-info/SOURCES.txt
--rw-rw-r--   0 x0axz     (1000) x0axz     (1000)        1 2023-06-02 07:15:51.000000 ngrad-1.0.2/ngrad.egg-info/dependency_links.txt
--rw-rw-r--   0 x0axz     (1000) x0axz     (1000)        6 2023-06-02 07:15:51.000000 ngrad-1.0.2/ngrad.egg-info/requires.txt
--rw-rw-r--   0 x0axz     (1000) x0axz     (1000)        6 2023-06-02 07:15:51.000000 ngrad-1.0.2/ngrad.egg-info/top_level.txt
--rw-rw-r--   0 x0axz     (1000) x0axz     (1000)       38 2023-06-02 07:15:51.851438 ngrad-1.0.2/setup.cfg
--rw-rw-r--   0 x0axz     (1000) x0axz     (1000)      727 2023-06-02 07:12:23.000000 ngrad-1.0.2/setup.py
-drwxrwxr-x   0 x0axz     (1000) x0axz     (1000)        0 2023-06-02 07:15:51.847439 ngrad-1.0.2/test/
--rw-rw-r--   0 x0axz     (1000) x0axz     (1000)     5098 2023-05-30 18:04:58.000000 ngrad-1.0.2/test/test_engine.py
+drwxrwxr-x   0 x0axz     (1000) x0axz     (1000)        0 2023-07-02 05:13:15.729863 ngrad-1.0.3/
+-rw-rw-r--   0 x0axz     (1000) x0axz     (1000)     1061 2023-05-30 18:26:38.000000 ngrad-1.0.3/LICENSE
+-rw-rw-r--   0 x0axz     (1000) x0axz     (1000)     3964 2023-07-02 05:13:15.729863 ngrad-1.0.3/PKG-INFO
+-rw-rw-r--   0 x0axz     (1000) x0axz     (1000)     3463 2023-06-28 09:17:45.000000 ngrad-1.0.3/README.md
+drwxrwxr-x   0 x0axz     (1000) x0axz     (1000)        0 2023-07-02 05:13:15.709866 ngrad-1.0.3/ngrad/
+-rw-rw-r--   0 x0axz     (1000) x0axz     (1000)        0 2023-05-29 09:04:57.000000 ngrad-1.0.3/ngrad/__init__.py
+-rw-rw-r--   0 x0axz     (1000) x0axz     (1000)     5054 2023-06-02 07:10:55.000000 ngrad-1.0.3/ngrad/engine.py
+-rw-rw-r--   0 x0axz     (1000) x0axz     (1000)     1898 2023-06-02 07:10:35.000000 ngrad-1.0.3/ngrad/library.py
+drwxrwxr-x   0 x0axz     (1000) x0axz     (1000)        0 2023-07-02 05:13:15.713865 ngrad-1.0.3/ngrad.egg-info/
+-rw-rw-r--   0 x0axz     (1000) x0axz     (1000)     3964 2023-07-02 05:13:15.000000 ngrad-1.0.3/ngrad.egg-info/PKG-INFO
+-rw-rw-r--   0 x0axz     (1000) x0axz     (1000)      241 2023-07-02 05:13:15.000000 ngrad-1.0.3/ngrad.egg-info/SOURCES.txt
+-rw-rw-r--   0 x0axz     (1000) x0axz     (1000)        1 2023-07-02 05:13:15.000000 ngrad-1.0.3/ngrad.egg-info/dependency_links.txt
+-rw-rw-r--   0 x0axz     (1000) x0axz     (1000)        6 2023-07-02 05:13:15.000000 ngrad-1.0.3/ngrad.egg-info/requires.txt
+-rw-rw-r--   0 x0axz     (1000) x0axz     (1000)        6 2023-07-02 05:13:15.000000 ngrad-1.0.3/ngrad.egg-info/top_level.txt
+-rw-rw-r--   0 x0axz     (1000) x0axz     (1000)       38 2023-07-02 05:13:15.729863 ngrad-1.0.3/setup.cfg
+-rw-rw-r--   0 x0axz     (1000) x0axz     (1000)      727 2023-07-02 05:12:54.000000 ngrad-1.0.3/setup.py
+drwxrwxr-x   0 x0axz     (1000) x0axz     (1000)        0 2023-07-02 05:13:15.713865 ngrad-1.0.3/test/
+-rw-rw-r--   0 x0axz     (1000) x0axz     (1000)     5098 2023-05-30 18:04:58.000000 ngrad-1.0.3/test/test_engine.py
```

### Comparing `ngrad-1.0.2/LICENSE` & `ngrad-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ngrad-1.0.2/PKG-INFO` & `ngrad-1.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ngrad
-Version: 1.0.2
+Version: 1.0.3
 Summary: An Autograd engine and a neural network library that handle an N-dimensional array.
 Home-page: https://github.com/x0axz/ngrad
 Author: Nooh
 Author-email: x0axz@protonmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -16,15 +16,15 @@
 
 # Autograd Engine & Neural Network Library
 
 The repository includes an Autograd engine and a neural network library that handle an N-dimensional array.
 
 Autograd is a tool used for derivative calculation. It tracks operations on values with enabled gradients and builds a dynamic computational graph — a graph without cycles. Input values serve as the leaves of the graph, while output values act as its roots. Gradients are computed by traversing the graph from root to leaf, applying the chain rule to multiply gradients at each step.
 
-Andrej Karaphy's [Micrograd](https://github.com/karpathy/micrograd) served as inspiration for this project. But this Autograd engine will accept N-dimensional array, whereas Microgard accepts scalar values only.
+Andrej Karpathy's [Micrograd](https://github.com/karpathy/micrograd) served as inspiration for this project. But this Autograd engine will accept N-dimensional array, whereas Microgard accepts scalar values only.
 
 ## Blog
 
 [Building Autograd Engine & Neural Network Library: An Interactive Guide](https://x0axz.com/blog/autograd.html)
 
 The article provides a comprehensive guide to building an autograd engine and a neural network library that handle an N-dimensional array. It assumes a basic understanding of Python programming, high school calculus, and neural networks but offers various teaching methods for beginners. It includes line-by-line code explanations, output visualizations, and an interactive area to explore derivatives. The guide covers the foundational concepts of neural networks, starting with derivatives and progressing to backpropagation. It explains how to perform backpropagation manually and programmatically, including implementation techniques. The article also demonstrates the building of an autograd class from scratch and its application to training a neural network on a dataset. It concludes by guiding readers through the development of a simple neural network library using the autograd class.
```

### Comparing `ngrad-1.0.2/README.md` & `ngrad-1.0.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Autograd Engine & Neural Network Library
 
 The repository includes an Autograd engine and a neural network library that handle an N-dimensional array.
 
 Autograd is a tool used for derivative calculation. It tracks operations on values with enabled gradients and builds a dynamic computational graph — a graph without cycles. Input values serve as the leaves of the graph, while output values act as its roots. Gradients are computed by traversing the graph from root to leaf, applying the chain rule to multiply gradients at each step.
 
-Andrej Karaphy's [Micrograd](https://github.com/karpathy/micrograd) served as inspiration for this project. But this Autograd engine will accept N-dimensional array, whereas Microgard accepts scalar values only.
+Andrej Karpathy's [Micrograd](https://github.com/karpathy/micrograd) served as inspiration for this project. But this Autograd engine will accept N-dimensional array, whereas Microgard accepts scalar values only.
 
 ## Blog
 
 [Building Autograd Engine & Neural Network Library: An Interactive Guide](https://x0axz.com/blog/autograd.html)
 
 The article provides a comprehensive guide to building an autograd engine and a neural network library that handle an N-dimensional array. It assumes a basic understanding of Python programming, high school calculus, and neural networks but offers various teaching methods for beginners. It includes line-by-line code explanations, output visualizations, and an interactive area to explore derivatives. The guide covers the foundational concepts of neural networks, starting with derivatives and progressing to backpropagation. It explains how to perform backpropagation manually and programmatically, including implementation techniques. The article also demonstrates the building of an autograd class from scratch and its application to training a neural network on a dataset. It concludes by guiding readers through the development of a simple neural network library using the autograd class.
```

### Comparing `ngrad-1.0.2/ngrad/engine.py` & `ngrad-1.0.3/ngrad/engine.py`

 * *Files identical despite different names*

### Comparing `ngrad-1.0.2/ngrad/library.py` & `ngrad-1.0.3/ngrad/library.py`

 * *Files identical despite different names*

### Comparing `ngrad-1.0.2/ngrad.egg-info/PKG-INFO` & `ngrad-1.0.3/ngrad.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ngrad
-Version: 1.0.2
+Version: 1.0.3
 Summary: An Autograd engine and a neural network library that handle an N-dimensional array.
 Home-page: https://github.com/x0axz/ngrad
 Author: Nooh
 Author-email: x0axz@protonmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -16,15 +16,15 @@
 
 # Autograd Engine & Neural Network Library
 
 The repository includes an Autograd engine and a neural network library that handle an N-dimensional array.
 
 Autograd is a tool used for derivative calculation. It tracks operations on values with enabled gradients and builds a dynamic computational graph — a graph without cycles. Input values serve as the leaves of the graph, while output values act as its roots. Gradients are computed by traversing the graph from root to leaf, applying the chain rule to multiply gradients at each step.
 
-Andrej Karaphy's [Micrograd](https://github.com/karpathy/micrograd) served as inspiration for this project. But this Autograd engine will accept N-dimensional array, whereas Microgard accepts scalar values only.
+Andrej Karpathy's [Micrograd](https://github.com/karpathy/micrograd) served as inspiration for this project. But this Autograd engine will accept N-dimensional array, whereas Microgard accepts scalar values only.
 
 ## Blog
 
 [Building Autograd Engine & Neural Network Library: An Interactive Guide](https://x0axz.com/blog/autograd.html)
 
 The article provides a comprehensive guide to building an autograd engine and a neural network library that handle an N-dimensional array. It assumes a basic understanding of Python programming, high school calculus, and neural networks but offers various teaching methods for beginners. It includes line-by-line code explanations, output visualizations, and an interactive area to explore derivatives. The guide covers the foundational concepts of neural networks, starting with derivatives and progressing to backpropagation. It explains how to perform backpropagation manually and programmatically, including implementation techniques. The article also demonstrates the building of an autograd class from scratch and its application to training a neural network on a dataset. It concludes by guiding readers through the development of a simple neural network library using the autograd class.
```

### Comparing `ngrad-1.0.2/setup.py` & `ngrad-1.0.3/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="ngrad",
-    version="1.0.2",
+    version="1.0.3",
     description="An Autograd engine and a neural network library that handle an N-dimensional array.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Nooh",
     author_email="x0axz@protonmail.com",
     url="https://github.com/x0axz/ngrad",
     packages=setuptools.find_packages(),
```

### Comparing `ngrad-1.0.2/test/test_engine.py` & `ngrad-1.0.3/test/test_engine.py`

 * *Files identical despite different names*

