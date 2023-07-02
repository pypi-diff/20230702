# Comparing `tmp/pycolonies-1.0.4-py3-none-any.whl.zip` & `tmp/pycolonies-1.0.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 9709 bytes, number of entries: 7
--rw-r--r--  2.0 unx     1116 b- defN 23-Mar-07 18:41 crypto.py
--rw-r--r--  2.0 unx    10986 b- defN 23-Jun-11 19:51 pycolonies.py
--rw-r--r--  2.0 unx     1065 b- defN 23-Jun-11 19:52 pycolonies-1.0.4.dist-info/LICENSE
--rw-r--r--  2.0 unx    18159 b- defN 23-Jun-11 19:52 pycolonies-1.0.4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-11 19:52 pycolonies-1.0.4.dist-info/WHEEL
--rw-r--r--  2.0 unx       18 b- defN 23-Jun-11 19:52 pycolonies-1.0.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      539 b- defN 23-Jun-11 19:52 pycolonies-1.0.4.dist-info/RECORD
-7 files, 31975 bytes uncompressed, 8763 bytes compressed:  72.6%
+Zip file size: 9720 bytes, number of entries: 7
+-rw-r--r--  2.0 unx     1116 b- defN 23-Jun-19 13:21 crypto.py
+-rw-r--r--  2.0 unx    11059 b- defN 23-Jul-02 21:04 pycolonies.py
+-rw-r--r--  2.0 unx     1065 b- defN 23-Jul-02 21:07 pycolonies-1.0.5.dist-info/LICENSE
+-rw-r--r--  2.0 unx    18151 b- defN 23-Jul-02 21:07 pycolonies-1.0.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-02 21:07 pycolonies-1.0.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx       18 b- defN 23-Jul-02 21:07 pycolonies-1.0.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      539 b- defN 23-Jul-02 21:07 pycolonies-1.0.5.dist-info/RECORD
+7 files, 32040 bytes uncompressed, 8774 bytes compressed:  72.6%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: crypto.py
 Comment: 
 
 Filename: pycolonies.py
 Comment: 
 
-Filename: pycolonies-1.0.4.dist-info/LICENSE
+Filename: pycolonies-1.0.5.dist-info/LICENSE
 Comment: 
 
-Filename: pycolonies-1.0.4.dist-info/METADATA
+Filename: pycolonies-1.0.5.dist-info/METADATA
 Comment: 
 
-Filename: pycolonies-1.0.4.dist-info/WHEEL
+Filename: pycolonies-1.0.5.dist-info/WHEEL
 Comment: 
 
-Filename: pycolonies-1.0.4.dist-info/top_level.txt
+Filename: pycolonies-1.0.5.dist-info/top_level.txt
 Comment: 
 
-Filename: pycolonies-1.0.4.dist-info/RECORD
+Filename: pycolonies-1.0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pycolonies.py

```diff
@@ -9,20 +9,21 @@
 
 class ColoniesConnectionError(Exception):
     pass
 
 class ColoniesError(Exception):
     pass
     
-def func_spec(func, args, colonyid, executortype, priority=1, maxexectime=-1, maxretries=-1, maxwaittime=-1, code=None):
+def func_spec(func, args, colonyid, executortype, priority=1, maxexectime=-1, maxretries=-1, maxwaittime=-1, code=None, kwargs=None):
     if isinstance(func, str):
         func_spec = {
             "nodename": func,
             "funcname": func, 
             "args": args,
+            "kwargs": kwargs,
             "priority": priority,
             "maxwaittime": maxwaittime,
             "maxexectime": maxexectime,
             "maxretries": maxretries,
             "conditions": {
                 "colonyid": colonyid,
                 "executortype": executortype
@@ -46,14 +47,15 @@
         args_spec = inspect.getfullargspec(func)
         args_spec_str = ','.join(args_spec.args)
 
         func_spec = {
             "nodename": funcname,
             "funcname": funcname,
             "args": args,
+            "kwargs": kwargs,
             "priority": priority,
             "maxwaittime": maxwaittime,
             "maxexectime": maxexectime,
             "maxretries": maxretries,
             "conditions": {
                 "colonyid": colonyid,
                 "executortype": executortype
```

## Comparing `pycolonies-1.0.4.dist-info/LICENSE` & `pycolonies-1.0.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pycolonies-1.0.4.dist-info/METADATA` & `pycolonies-1.0.5.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: pycolonies
-Version: 1.0.4
+Version: 1.0.5
 Summary: Colonies Python SDK
 Home-page: https://github.com/colonyos/pycolonies
 Author: Johan Kristiansson
 Author-email: johan.kristiansson@ri.se
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+License-File: LICENSE
 Requires-Dist: requests (>=2.27.1)
 Requires-Dist: websocket-client (>=1.3.1)
 
 [![Python3](https://github.com/colonyos/pycolonies/actions/workflows/python.yml/badge.svg)](https://github.com/colonyos/pycolonies/actions/workflows/python.yml)
 
 # Introduction
 This repo contains a Python [Colonies](https://github.com/colonyos/colonies), making it possible to implement Colonies Executors in Python. 
@@ -204,15 +203,15 @@
 
 ```console
 python3 examples/echo_executor.py
 ```
 
 # Code-injection
 Python has a built-in `eval()` function that allows execution of any piece of Python code encoded as strings. We are going to use the `eval()` function to implement an executor that can execute arbitrary Python functions.
-
+   
 Python also has support for introspection, which allows Python code to examine itself. We are going to use that to get the source code of function definitions, e.g. the `echo` function.
 ```python
 def echo(arg)
     return arg
 
 code = inspect.getsource(echo)
 ```
@@ -343,19 +342,19 @@
 
 The `map()` function below dynamically adds 5 `gen_nums()` functions to the processgraph.
 
 ```python
 def map(ctx={}):
     code = """def gen_nums(ctx={}):
                 return 1, 2""" 
-
+  
     processgraphid = ctx["process"]["processgraphid"]
     map_processid = ctx["process"]["processid"]
     executor_prvkey = ctx["executor_prvkey"]
-
+  
     processgraph = colonies.get_processgraph(processgraphid, executor_prvkey)
     print(processgraph)
     reduce_process = colonies.find_process("reduce", processgraph["processids"], executor_prvkey)
     reduce_processid = reduce_process["processid"]
 
     insert = True
     for i in range(5):
@@ -424,9 +423,7 @@
 
 m = ColoniesMonad("localhost", 50080, colonyid, executor_prvkey)
 result = (m >> gen_data >> process_data >> echo).unwrap()
 print(result)  # prints 3 
 ```
 
 See [colonies_monad.py](https://github.com/colonyos/pycolonies/blob/main/examples/colonies_monad.py) and [monad_example2.py](https://github.com/colonyos/pycolonies/blob/main/examples/monad_example2.py) for a full example.
-
-
```

## Comparing `pycolonies-1.0.4.dist-info/RECORD` & `pycolonies-1.0.5.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 crypto.py,sha256=E32-MZemEYRiHogWLDGIuLFxNufTFCyAG5Fuy0AuBA0,1116
-pycolonies.py,sha256=zLUBmtkIaan1tf9QHscb2Jk5RnAWdhLA6TMEJtUr4iA,10986
-pycolonies-1.0.4.dist-info/LICENSE,sha256=1sKaC4DMCeNr-aKTEhWaNrJeXuUWoWuOSO1Ir9UilCI,1065
-pycolonies-1.0.4.dist-info/METADATA,sha256=yWdvuQG3ki4yAaSxIxJS-KPxRDKSlOswqnRsQehXGps,18159
-pycolonies-1.0.4.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-pycolonies-1.0.4.dist-info/top_level.txt,sha256=iYJfMb3XHzfQmifMsYc1M5kQXhbakxb7iKcdyysYTU0,18
-pycolonies-1.0.4.dist-info/RECORD,,
+pycolonies.py,sha256=uADHXI21MI0RsVfIkcWnYEXza9wIfLpYZpILDdcEZ4U,11059
+pycolonies-1.0.5.dist-info/LICENSE,sha256=1sKaC4DMCeNr-aKTEhWaNrJeXuUWoWuOSO1Ir9UilCI,1065
+pycolonies-1.0.5.dist-info/METADATA,sha256=i_TLyUFHks_HzHSpKF8luIeYadWo_0pvakyRvn8dD3A,18151
+pycolonies-1.0.5.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+pycolonies-1.0.5.dist-info/top_level.txt,sha256=iYJfMb3XHzfQmifMsYc1M5kQXhbakxb7iKcdyysYTU0,18
+pycolonies-1.0.5.dist-info/RECORD,,
```

