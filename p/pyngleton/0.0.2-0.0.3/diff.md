# Comparing `tmp/pyngleton-0.0.2-py3-none-any.whl.zip` & `tmp/pyngleton-0.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 2600 bytes, number of entries: 5
--rw-r--r--  2.0 unx     1078 b- defN 20-Feb-02 00:00 pyngleton/__init__.py
-?rw-r--r--  2.0 unx      854 b- defN 20-Feb-02 00:00 pyngleton-0.0.2.dist-info/METADATA
-?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 pyngleton-0.0.2.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1076 b- defN 20-Feb-02 00:00 pyngleton-0.0.2.dist-info/licenses/LICENSE
-?rw-r--r--  2.0 unx      388 b- defN 20-Feb-02 00:00 pyngleton-0.0.2.dist-info/RECORD
-5 files, 3483 bytes uncompressed, 1878 bytes compressed:  46.1%
+Zip file size: 2603 bytes, number of entries: 5
+-rw-r--r--  2.0 unx     1093 b- defN 20-Feb-02 00:00 pyngleton/__init__.py
+?rw-r--r--  2.0 unx      854 b- defN 20-Feb-02 00:00 pyngleton-0.0.3.dist-info/METADATA
+?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 pyngleton-0.0.3.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1076 b- defN 20-Feb-02 00:00 pyngleton-0.0.3.dist-info/licenses/LICENSE
+?rw-r--r--  2.0 unx      388 b- defN 20-Feb-02 00:00 pyngleton-0.0.3.dist-info/RECORD
+5 files, 3498 bytes uncompressed, 1881 bytes compressed:  46.2%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
 Filename: pyngleton/__init__.py
 Comment: 
 
-Filename: pyngleton-0.0.2.dist-info/METADATA
+Filename: pyngleton-0.0.3.dist-info/METADATA
 Comment: 
 
-Filename: pyngleton-0.0.2.dist-info/WHEEL
+Filename: pyngleton-0.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: pyngleton-0.0.2.dist-info/licenses/LICENSE
+Filename: pyngleton-0.0.3.dist-info/licenses/LICENSE
 Comment: 
 
-Filename: pyngleton-0.0.2.dist-info/RECORD
+Filename: pyngleton-0.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pyngleton/__init__.py

```diff
@@ -1,12 +1,12 @@
 import os
 import threading
 
 
-class _SingletonMeta(type):
+class SingletonMeta(type):
     """
     This is a metaclass that creates a Singleton instance. It creates the instance in a
     process-safe and thread-safe manner.
     """
 
     _instances = {}
     _lock: threading.Lock = threading.Lock()
@@ -22,21 +22,21 @@
             with cls._lock:
                 if pid not in cls._instances:
                     instance = super().__call__(*args, **kwargs)
                     cls._instances[pid] = instance
         return cls._instances[pid]
 
 
-class Singleton(metaclass=_SingletonMeta):
+class Singleton(metaclass=SingletonMeta):
     """
     This is the Singleton class that uses the SingletonMeta metaclass. It should be inherited by any class
     that should be a Singleton.
     """
     pass
 
     @classmethod
     def reset(cls):
         with cls._lock:
             cls._instances.clear()
 
 
-__all__ = ['Singleton']
+__all__ = ['Singleton', 'SingletonMeta']
```

## Comparing `pyngleton-0.0.2.dist-info/METADATA` & `pyngleton-0.0.3.dist-info/METADATA`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyngleton
-Version: 0.0.2
+Version: 0.0.3
 Summary: A small example package
 Project-URL: Homepage, https://github.com/yourlogarithm/pyngleton
 Project-URL: Bug Tracker, https://github.com/yourlogarithm/pyngleton/issues
 Author-email: Vlad-Sebastian Cretu <vlad.sebastian.cretu.dev@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

## Comparing `pyngleton-0.0.2.dist-info/licenses/LICENSE` & `pyngleton-0.0.3.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

