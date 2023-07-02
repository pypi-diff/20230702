# Comparing `tmp/watermark-2.4.2.tar.gz` & `tmp/watermark-2.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watermark-2.4.2.tar", last modified: Tue May 23 19:00:07 2023, max compression
+gzip compressed data, was "watermark-2.4.3.tar", last modified: Sun Jul  2 14:32:01 2023, max compression
```

## Comparing `watermark-2.4.2.tar` & `watermark-2.4.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 sebastianraschka   (501) staff       (20)        0 2023-05-23 19:00:07.833177 watermark-2.4.2/
--rw-r--r--   0 sebastianraschka   (501) staff       (20)     1507 2023-05-23 16:50:16.000000 watermark-2.4.2/LICENSE
--rw-r--r--   0 sebastianraschka   (501) staff       (20)       58 2023-05-23 18:54:21.000000 watermark-2.4.2/MANIFEST.in
--rw-r--r--   0 sebastianraschka   (501) staff       (20)     1205 2023-05-23 19:00:07.833254 watermark-2.4.2/PKG-INFO
--rw-r--r--   0 sebastianraschka   (501) staff       (20)    11591 2023-05-23 16:50:16.000000 watermark-2.4.2/README.md
--rw-r--r--   0 sebastianraschka   (501) staff       (20)       49 2023-05-23 18:58:20.000000 watermark-2.4.2/requirements.txt
--rw-r--r--   0 sebastianraschka   (501) staff       (20)      512 2023-05-23 19:00:07.833504 watermark-2.4.2/setup.cfg
--rw-r--r--   0 sebastianraschka   (501) staff       (20)     1476 2023-05-23 16:50:16.000000 watermark-2.4.2/setup.py
-drwxr-xr-x   0 sebastianraschka   (501) staff       (20)        0 2023-05-23 19:00:07.832279 watermark-2.4.2/watermark/
--rw-r--r--   0 sebastianraschka   (501) staff       (20)      373 2023-05-23 16:50:16.000000 watermark-2.4.2/watermark/__init__.py
--rw-r--r--   0 sebastianraschka   (501) staff       (20)     3842 2023-05-23 16:50:16.000000 watermark-2.4.2/watermark/magic.py
--rw-r--r--   0 sebastianraschka   (501) staff       (20)      291 2023-05-23 16:50:16.000000 watermark-2.4.2/watermark/version.py
--rw-r--r--   0 sebastianraschka   (501) staff       (20)    10070 2023-05-23 16:50:16.000000 watermark-2.4.2/watermark/watermark.py
-drwxr-xr-x   0 sebastianraschka   (501) staff       (20)        0 2023-05-23 19:00:07.833028 watermark-2.4.2/watermark.egg-info/
--rw-r--r--   0 sebastianraschka   (501) staff       (20)     1205 2023-05-23 19:00:07.000000 watermark-2.4.2/watermark.egg-info/PKG-INFO
--rw-r--r--   0 sebastianraschka   (501) staff       (20)      314 2023-05-23 19:00:07.000000 watermark-2.4.2/watermark.egg-info/SOURCES.txt
--rw-r--r--   0 sebastianraschka   (501) staff       (20)        1 2023-05-23 19:00:07.000000 watermark-2.4.2/watermark.egg-info/dependency_links.txt
--rw-r--r--   0 sebastianraschka   (501) staff       (20)       61 2023-05-23 19:00:07.000000 watermark-2.4.2/watermark.egg-info/requires.txt
--rw-r--r--   0 sebastianraschka   (501) staff       (20)       10 2023-05-23 19:00:07.000000 watermark-2.4.2/watermark.egg-info/top_level.txt
+drwxr-xr-x   0 sebastian   (501) staff       (20)        0 2023-07-02 14:32:01.037516 watermark-2.4.3/
+-rw-r--r--   0 sebastian   (501) staff       (20)     1507 2022-01-04 01:54:42.000000 watermark-2.4.3/LICENSE
+-rw-r--r--   0 sebastian   (501) staff       (20)       58 2023-07-02 14:31:32.000000 watermark-2.4.3/MANIFEST.in
+-rw-r--r--   0 sebastian   (501) staff       (20)     1225 2023-07-02 14:32:01.037579 watermark-2.4.3/PKG-INFO
+-rw-r--r--   0 sebastian   (501) staff       (20)    11876 2023-07-02 14:31:32.000000 watermark-2.4.3/README.md
+-rw-r--r--   0 sebastian   (501) staff       (20)       41 2023-07-02 14:31:32.000000 watermark-2.4.3/requirements.txt
+-rw-r--r--   0 sebastian   (501) staff       (20)      512 2023-07-02 14:32:01.037904 watermark-2.4.3/setup.cfg
+-rw-r--r--   0 sebastian   (501) staff       (20)     1522 2023-07-02 14:31:32.000000 watermark-2.4.3/setup.py
+drwxr-xr-x   0 sebastian   (501) staff       (20)        0 2023-07-02 14:32:01.036767 watermark-2.4.3/watermark/
+-rw-r--r--   0 sebastian   (501) staff       (20)      373 2022-01-04 01:25:16.000000 watermark-2.4.3/watermark/__init__.py
+-rw-r--r--   0 sebastian   (501) staff       (20)     3842 2023-07-02 14:31:32.000000 watermark-2.4.3/watermark/magic.py
+-rw-r--r--   0 sebastian   (501) staff       (20)      291 2022-01-04 01:25:16.000000 watermark-2.4.3/watermark/version.py
+-rw-r--r--   0 sebastian   (501) staff       (20)    10313 2023-07-02 14:31:32.000000 watermark-2.4.3/watermark/watermark.py
+drwxr-xr-x   0 sebastian   (501) staff       (20)        0 2023-07-02 14:32:01.037415 watermark-2.4.3/watermark.egg-info/
+-rw-r--r--   0 sebastian   (501) staff       (20)     1225 2023-07-02 14:32:00.000000 watermark-2.4.3/watermark.egg-info/PKG-INFO
+-rw-r--r--   0 sebastian   (501) staff       (20)      314 2023-07-02 14:32:00.000000 watermark-2.4.3/watermark.egg-info/SOURCES.txt
+-rw-r--r--   0 sebastian   (501) staff       (20)        1 2023-07-02 14:32:00.000000 watermark-2.4.3/watermark.egg-info/dependency_links.txt
+-rw-r--r--   0 sebastian   (501) staff       (20)       68 2023-07-02 14:32:00.000000 watermark-2.4.3/watermark.egg-info/requires.txt
+-rw-r--r--   0 sebastian   (501) staff       (20)       10 2023-07-02 14:32:00.000000 watermark-2.4.3/watermark.egg-info/top_level.txt
```

### Comparing `watermark-2.4.2/LICENSE` & `watermark-2.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `watermark-2.4.2/PKG-INFO` & `watermark-2.4.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: watermark
-Version: 2.4.2
+Version: 2.4.3
 Summary: IPython magic function to print date/time stamps and various system information.
 Home-page: https://github.com/rasbt/watermark
 Author: Sebastian Raschka
 Author-email: mail@sebastianraschka.com
 License: newBSD
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: IPython
@@ -13,14 +13,15 @@
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.7
+Provides-Extra: gpu
 License-File: LICENSE
 
 An IPython magic extension for printing date and time stamps, version
 numbers, and hardware information.
 
 Contact
 =============
```

### Comparing `watermark-2.4.2/README.md` & `watermark-2.4.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -172,23 +172,31 @@
 
 <br>
 
 ## Changelog
 
 [[top](#sections)]
 
+#### v. 2.4.3 (May 23, 2023)
+
+- Make `py3nvml` installation for GPU info optional. ([#92](https://github.com/rasbt/watermark/pull/92), via contribution by [Ben Greiner](https://github.com/bnavigator))
+
+#### v. 2.4.1 and v 2.4.2 (May 23, 2023)
+
+- PyPI and Conda-Forge packaging fixes.
+
 #### v. 2.4.0 (May 23, 2023)
 
-- Adds a new `--gpu` flag to print out GPU information (currently limited to NVIDIA devices) ([#90](https://github.com/rasbt/watermark/pull/63), via contribution by [907Resident](https://github.com/907Resident))
+- Adds a new `--gpu` flag to print out GPU information (currently limited to NVIDIA devices) ([#90](https://github.com/rasbt/watermark/pull/90), via contribution by [907Resident](https://github.com/907Resident))
 
 
 #### v. 2.3.1 (May 27, 2022)
 
 - Upper limit on importlib-metadata caused trouble installing on Python 3.7.
-  Instead pin to minimum version with Python 3.8 functionality according to https://github.com/python/importlib_metadata#compatibility  ([#86](https://github.com/rasbt/watermark/pull/63), via contribution by [James Myatt](https://github.com/jamesmyatt))
+  Instead pin to minimum version with Python 3.8 functionality according to https://github.com/python/importlib_metadata#compatibility  ([#86](https://github.com/rasbt/watermark/pull/86), via contribution by [James Myatt](https://github.com/jamesmyatt))
 
 #### v. 2.3.0 (January 3, 2022)
 
 - Added the following arguments: `--github_username` - for prints author github username, `--email` - for prints author email, `--website` - for prints author or project website. ([#82](https://github.com/rasbt/watermark/pull/82), via contribution by [joschkazj](https://github.com/joschkazj))
 - Added a `--conda` option to print the name of the current conda environment. ([#79](https://github.com/rasbt/watermark/pull/79), via contribution by [Alexander Krasnikov](https://github.com/askras))
 -  It is now possible to inject globals when used outside IPython ([#80](https://github.com/rasbt/watermark/pull/80), via contribution by [
 Hugo Lapré](https://github.com/Hugovdberg)). For example, version numbers of imported packages can now be obtained as follows:
```

### Comparing `watermark-2.4.2/setup.cfg` & `watermark-2.4.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [metadata]
-version = 2.4.2
+version = 2.4.3
 license_file = LICENSE
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	Framework :: IPython
 	Intended Audience :: Developers
 	Intended Audience :: Science/Research
 	License :: OSI Approved :: BSD License
```

### Comparing `watermark-2.4.2/setup.py` & `watermark-2.4.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,14 +28,15 @@
         "various system information."
     ),
     author="Sebastian Raschka",
     author_email="mail@sebastianraschka.com",
     url="https://github.com/rasbt/watermark",
     packages=find_packages(exclude=[]),
     install_requires=install_reqs,
+    extras_require={'gpu': ['py3nvml>=0.2']},
     long_description=dedent(
         """\
         An IPython magic extension for printing date and time stamps, version
         numbers, and hardware information.
 
         Contact
         =============
```

### Comparing `watermark-2.4.2/watermark/magic.py` & `watermark-2.4.3/watermark/magic.py`

 * *Files identical despite different names*

### Comparing `watermark-2.4.2/watermark/watermark.py` & `watermark-2.4.3/watermark/watermark.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,19 @@
 import platform
 import subprocess
 import time
 import types
 from multiprocessing import cpu_count
 from socket import gethostname
 import platform
-from py3nvml import py3nvml
+
+try:
+    from py3nvml import py3nvml
+except ImportError:
+    py3nvml = None
 
 try:
     import importlib.metadata as importlib_metadata
 except ImportError:
     # Running on pre-3.8 Python; use importlib-metadata package
     import importlib_metadata
 
@@ -330,14 +334,18 @@
 
 def _get_conda_env():
     name = os.getenv('CONDA_DEFAULT_ENV', 'n/a')
     return {"conda environment": name}
 
 
 def _get_gpu_info():
+    if py3nvml is None:
+        return {"GPU Info": "Install the gpu extra "
+                "(pip install 'watermark[gpu]') "
+                "to display GPU information for NVIDIA chipsets"}
     try:
         gpu_info = [""]
         py3nvml.nvmlInit()
         num_gpus = py3nvml.nvmlDeviceGetCount()
         for i in range(num_gpus):
             handle = py3nvml.nvmlDeviceGetHandleByIndex(i)
             gpu_name = py3nvml.nvmlDeviceGetName(handle)
@@ -346,8 +354,8 @@
         return {"GPU Info": "\n  ".join(gpu_info)}
 
     except py3nvml.NVMLError_LibraryNotFound:
         return {"GPU Info": "NVIDIA drivers do not appear "
                 "to be installed on this machine."}
     except:
         return {"GPU Info": "GPU information is not "
-                "available for this machine."}
+                "available for this machine."}
```

### Comparing `watermark-2.4.2/watermark.egg-info/PKG-INFO` & `watermark-2.4.3/watermark.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: watermark
-Version: 2.4.2
+Version: 2.4.3
 Summary: IPython magic function to print date/time stamps and various system information.
 Home-page: https://github.com/rasbt/watermark
 Author: Sebastian Raschka
 Author-email: mail@sebastianraschka.com
 License: newBSD
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: IPython
@@ -13,14 +13,15 @@
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.7
+Provides-Extra: gpu
 License-File: LICENSE
 
 An IPython magic extension for printing date and time stamps, version
 numbers, and hardware information.
 
 Contact
 =============
```

