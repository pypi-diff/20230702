# Comparing `tmp/tired-0.0.2.tar.gz` & `tmp/tired-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tired-0.0.2.tar", last modified: Sat Jun 17 13:11:55 2023, max compression
+gzip compressed data, was "tired-0.0.3.tar", last modified: Sun Jul  2 10:28:38 2023, max compression
```

## Comparing `tired-0.0.2.tar` & `tired-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,19 @@
-drwxr-xr-x   0 dm        (1000) dm        (1000)        0 2023-06-17 13:11:55.656507 tired-0.0.2/
--rw-r--r--   0 dm        (1000) dm        (1000)      518 2023-06-17 13:11:55.656507 tired-0.0.2/PKG-INFO
--rw-r--r--   0 dm        (1000) dm        (1000)      119 2023-06-17 12:57:13.000000 tired-0.0.2/README.md
--rw-r--r--   0 dm        (1000) dm        (1000)       38 2023-06-17 13:11:55.656507 tired-0.0.2/setup.cfg
--rw-r--r--   0 dm        (1000) dm        (1000)      799 2023-06-17 13:10:52.000000 tired-0.0.2/setup.py
-drwxr-xr-x   0 dm        (1000) dm        (1000)        0 2023-06-17 13:11:55.656507 tired-0.0.2/tired/
--rw-r--r--   0 dm        (1000) dm        (1000)     1246 2023-06-17 12:18:49.000000 tired-0.0.2/tired/command.py
--rw-r--r--   0 dm        (1000) dm        (1000)    13501 2023-06-11 17:36:43.000000 tired-0.0.2/tired/shlex.py
--rw-r--r--   0 dm        (1000) dm        (1000)      130 2023-06-17 13:06:53.000000 tired-0.0.2/tired/ui.py
-drwxr-xr-x   0 dm        (1000) dm        (1000)        0 2023-06-17 13:11:55.656507 tired-0.0.2/tired.egg-info/
--rw-r--r--   0 dm        (1000) dm        (1000)      518 2023-06-17 13:11:55.000000 tired-0.0.2/tired.egg-info/PKG-INFO
--rw-r--r--   0 dm        (1000) dm        (1000)      206 2023-06-17 13:11:55.000000 tired-0.0.2/tired.egg-info/SOURCES.txt
--rw-r--r--   0 dm        (1000) dm        (1000)        1 2023-06-17 13:11:55.000000 tired-0.0.2/tired.egg-info/dependency_links.txt
--rw-r--r--   0 dm        (1000) dm        (1000)       17 2023-06-17 13:11:55.000000 tired-0.0.2/tired.egg-info/requires.txt
--rw-r--r--   0 dm        (1000) dm        (1000)        6 2023-06-17 13:11:55.000000 tired-0.0.2/tired.egg-info/top_level.txt
+drwxr-xr-x   0 dm        (1000) dm        (1000)        0 2023-07-02 10:28:38.597775 tired-0.0.3/
+-rw-r--r--   0 dm        (1000) dm        (1000)      518 2023-07-02 10:28:38.597775 tired-0.0.3/PKG-INFO
+-rw-r--r--   0 dm        (1000) dm        (1000)      119 2023-06-17 12:57:13.000000 tired-0.0.3/README.md
+-rw-r--r--   0 dm        (1000) dm        (1000)       38 2023-07-02 10:28:38.597775 tired-0.0.3/setup.cfg
+-rw-r--r--   0 dm        (1000) dm        (1000)      799 2023-07-02 10:27:36.000000 tired-0.0.3/setup.py
+drwxr-xr-x   0 dm        (1000) dm        (1000)        0 2023-07-02 10:28:38.597775 tired-0.0.3/tired/
+-rw-r--r--   0 dm        (1000) dm        (1000)     1263 2023-07-02 10:13:00.000000 tired-0.0.3/tired/command.py
+-rw-r--r--   0 dm        (1000) dm        (1000)      711 2023-07-02 07:50:06.000000 tired-0.0.3/tired/fs.py
+-rw-r--r--   0 dm        (1000) dm        (1000)      179 2023-07-02 07:50:06.000000 tired-0.0.3/tired/git.py
+-rw-r--r--   0 dm        (1000) dm        (1000)      239 2023-07-02 07:50:06.000000 tired-0.0.3/tired/meta.py
+-rw-r--r--   0 dm        (1000) dm        (1000)       62 2023-07-02 07:50:06.000000 tired-0.0.3/tired/parse.py
+-rw-r--r--   0 dm        (1000) dm        (1000)    13501 2023-06-11 17:36:43.000000 tired-0.0.3/tired/shlex.py
+-rw-r--r--   0 dm        (1000) dm        (1000)      305 2023-07-02 08:24:54.000000 tired-0.0.3/tired/ui.py
+drwxr-xr-x   0 dm        (1000) dm        (1000)        0 2023-07-02 10:28:38.597775 tired-0.0.3/tired.egg-info/
+-rw-r--r--   0 dm        (1000) dm        (1000)      518 2023-07-02 10:28:38.000000 tired-0.0.3/tired.egg-info/PKG-INFO
+-rw-r--r--   0 dm        (1000) dm        (1000)      260 2023-07-02 10:28:38.000000 tired-0.0.3/tired.egg-info/SOURCES.txt
+-rw-r--r--   0 dm        (1000) dm        (1000)        1 2023-07-02 10:28:38.000000 tired-0.0.3/tired.egg-info/dependency_links.txt
+-rw-r--r--   0 dm        (1000) dm        (1000)       17 2023-07-02 10:28:38.000000 tired-0.0.3/tired.egg-info/requires.txt
+-rw-r--r--   0 dm        (1000) dm        (1000)        6 2023-07-02 10:28:38.000000 tired-0.0.3/tired.egg-info/top_level.txt
```

### Comparing `tired-0.0.2/PKG-INFO` & `tired-0.0.3/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tired
-Version: 0.0.2
+Version: 0.0.3
 Summary: Boilerplate I'm tired of writing over and over
 Home-page: https://github.com/damurashov/TIRED
 Author: Dmitry Murashov
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `tired-0.0.2/setup.py` & `tired-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,10 +22,10 @@
     ],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.7",
-    version="0.0.2",
+    version="0.0.3",
 )
```

### Comparing `tired-0.0.2/tired/command.py` & `tired-0.0.3/tired/command.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from shlex import split
 
 
 def listout(l: list):
 	print('>', ' '.join(l))
 
 
-def output_piped(commands, verbose=False):
+def get_output_piped(commands, verbose=False):
 	"""
 	:param commands: commands to execute. The commands are executed in a sequential manner, i.e. piped
 	:return: console output, string
 	"""
 	commands = [split(c) for c in commands]
 	procs = []
 
@@ -27,30 +27,30 @@
 
 	if verbose and len(out):
 		print(out.decode("unicode_escape"))
 
 	return out, p.returncode
 
 
-def output(cmd):
+def get_output(cmd):
 	print('>  ' + cmd)
 	ret = subprocess.run(split(cmd), stdout=subprocess.PIPE)
 
 	if ret.returncode != 0:
 		raise Exception("Command execution error")
 
 	return ret.stdout.decode("unicode_escape").strip()
 
 
-def output_code(cmd):
+def get_output_with_code(cmd):
 	print('>  ' + cmd)
 	ret = subprocess.run(split(cmd), stdout=subprocess.PIPE)
 
 	return ret.stdout.decode("unicode_escape").strip(), ret.returncode
 
 
-def command(cmd):
+def execute(cmd):
 	print('>  ' + cmd)
 	ret = subprocess.run(split(cmd))
 
 	if ret.returncode != 0:
 		raise Exception(f"Command execution error (returncode - {ret.returncode})")
```

### Comparing `tired-0.0.2/tired/shlex.py` & `tired-0.0.3/tired/shlex.py`

 * *Files identical despite different names*

### Comparing `tired-0.0.2/tired.egg-info/PKG-INFO` & `tired-0.0.3/tired.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tired
-Version: 0.0.2
+Version: 0.0.3
 Summary: Boilerplate I'm tired of writing over and over
 Home-page: https://github.com/damurashov/TIRED
 Author: Dmitry Murashov
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

