# Comparing `tmp/funcOAI-0.0.2.tar.gz` & `tmp/funcOAI-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funcOAI-0.0.2.tar", last modified: Thu Jun 29 07:52:43 2023, max compression
+gzip compressed data, was "funcOAI-0.0.3.tar", last modified: Sun Jul  2 00:25:30 2023, max compression
```

## Comparing `funcOAI-0.0.2.tar` & `funcOAI-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:52:43.203927 funcOAI-0.0.2/
--rw-r--r--   0 root         (0) root         (0)     1063 2023-06-29 07:17:55.000000 funcOAI-0.0.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2506 2023-06-29 07:52:43.203927 funcOAI-0.0.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1815 2023-06-29 07:17:55.000000 funcOAI-0.0.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:52:43.203927 funcOAI-0.0.2/funcOAI.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2506 2023-06-29 07:52:43.000000 funcOAI-0.0.2/funcOAI.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      199 2023-06-29 07:52:43.000000 funcOAI-0.0.2/funcOAI.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-29 07:52:43.000000 funcOAI-0.0.2/funcOAI.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-06-29 07:52:43.000000 funcOAI-0.0.2/funcOAI.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:52:43.203927 funcOAI-0.0.2/functionalOAI/
--rw-r--r--   0 root         (0) root         (0)       25 2023-06-29 07:17:55.000000 funcOAI-0.0.2/functionalOAI/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3462 2023-06-29 07:17:55.000000 funcOAI-0.0.2/functionalOAI/funAI.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-29 07:52:43.203927 funcOAI-0.0.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      979 2023-06-29 07:52:21.000000 funcOAI-0.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 00:25:30.599992 funcOAI-0.0.3/
+-rw-r--r--   0 root         (0) root         (0)     1063 2023-06-29 07:17:55.000000 funcOAI-0.0.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     4798 2023-07-02 00:25:30.599992 funcOAI-0.0.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4107 2023-07-01 13:11:14.000000 funcOAI-0.0.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 00:25:30.599992 funcOAI-0.0.3/funcOAI.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4798 2023-07-02 00:25:30.000000 funcOAI-0.0.3/funcOAI.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      226 2023-07-02 00:25:30.000000 funcOAI-0.0.3/funcOAI.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-02 00:25:30.000000 funcOAI-0.0.3/funcOAI.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-07-02 00:25:30.000000 funcOAI-0.0.3/funcOAI.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 00:25:30.599992 funcOAI-0.0.3/functionalOAI/
+-rw-r--r--   0 root         (0) root         (0)       62 2023-07-01 22:24:33.000000 funcOAI-0.0.3/functionalOAI/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3541 2023-07-02 00:19:01.000000 funcOAI-0.0.3/functionalOAI/funAI.py
+-rw-r--r--   0 root         (0) root         (0)     2890 2023-07-02 00:15:40.000000 funcOAI-0.0.3/functionalOAI/functions.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-02 00:25:30.599992 funcOAI-0.0.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      979 2023-07-02 00:19:30.000000 funcOAI-0.0.3/setup.py
```

### Comparing `funcOAI-0.0.2/LICENSE` & `funcOAI-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `funcOAI-0.0.2/functionalOAI/funAI.py` & `funcOAI-0.0.3/functionalOAI/funAI.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 from inspect import signature, Parameter
 from typing import Callable, List, Dict
+from functions import functionsList
 
 class FunAI:
     def __init__(self) -> None:
-        # TODO: create a special TYPE for the list of functions that has multiple useable methods
-        self.__functionsList: List[Dict] = list()
+        self.__functionsList: functionsList = functionsList()
 
     @property
-    def functions(self) -> List[Dict]:
+    def functions(self) -> functionsList:
         """
         return a list of all the attached functions.
         
         :returns: __functionsList
-        :rtype  : typing.List[typing.Dict]
+        :rtype  : <Class functionsList> 
         """
         return self.__functionsList
 
     @functions.setter
-    def functions(self, fn: List[Dict]) -> List[Dict]:
+    def functions(self, fn: List[Dict]) -> functionsList:
         """
-        manually attach function bodies to functionsList.
+        replace all the functions inside __functionsList with the functions that the user has provided 
 
         :param fn: functions to attach
-        :type fn : typing.List[typing.Dict]
+        :type fn : typing.List[typing.Dict] 
         :returns : __functionsList
-        :rtype   : typing.List[typing.Dict]
+        :rtype   : <Class functionsList>
         """
-        self.__functionsList = fn
+        self.__functionsList.clear()
+        for function in fn:
+            self.__functionsList.append(function)
         return self.__functionsList
 
     @property
     def attach(self) -> Callable:
         """
         attach a decorated function body to functionsList.
 
@@ -40,22 +42,22 @@
         def wrapper(func) -> Callable:
             self.attachFunctions([func])
             return func
 
         return wrapper
 
     @attach.setter
-    def attach(self, fn: Callable) -> List[Dict]:
+    def attach(self, fn: Callable) -> functionsList:
         """
         manually attach a single function body to functionsList.
 
         :param fn: function to attach
         :type fn : typing.Callable
         :returns : __functionsList
-        :rtype   : typing.List[typing.Dict]
+        :rtype   : <Class functionsList>
         """
         self.attachFunctions([fn])
         return self.__functionsList
     
     def attachFunctions(self, fn: List[Callable]) -> None:
         """
         Loop through a list of callables and append their bodies to functionsList,
```

### Comparing `funcOAI-0.0.2/setup.py` & `funcOAI-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 from pathlib import Path
 
 long_description = (Path(__file__).parent / "README.md").read_text()
 
-VERSION = '0.0.2'
+VERSION = '0.0.3'
 DESCRIPTION = 'A package that helps users easily create functions to feed to GPT function calling API'
 # Setting up
 setup(
     name="funcOAI",
     version=VERSION,
     author="x5up0 aka.ryan",
     author_email="x5up0sbu@gmail.com",
```

