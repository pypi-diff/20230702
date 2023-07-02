# Comparing `tmp/autodistill_yolov8-0.1.0.tar.gz` & `tmp/autodistill_yolov8-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/autodistill_yolov8-0.1.0.tar", last modified: Sat May 27 03:02:18 2023, max compression
+gzip compressed data, was "autodistill_yolov8-0.1.1.tar", last modified: Sun Jul  2 19:49:15 2023, max compression
```

## Comparing `autodistill_yolov8-0.1.0.tar` & `autodistill_yolov8-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 yeldarb   (1000) yeldarb   (1001)        0 2023-05-27 03:02:18.000000 autodistill_yolov8-0.1.0/
--rw-r--r--   0 yeldarb   (1000) yeldarb   (1001)      594 2023-05-27 03:02:18.000000 autodistill_yolov8-0.1.0/PKG-INFO
--rw-r--r--   0 yeldarb   (1000) yeldarb   (1001)     3157 2023-05-27 02:55:33.000000 autodistill_yolov8-0.1.0/README.md
-drwxr-xr-x   0 yeldarb   (1000) yeldarb   (1001)        0 2023-05-27 03:02:18.000000 autodistill_yolov8-0.1.0/autodistill_yolov8/
--rw-r--r--   0 yeldarb   (1000) yeldarb   (1001)       68 2023-05-27 03:02:12.000000 autodistill_yolov8-0.1.0/autodistill_yolov8/__init__.py
--rw-r--r--   0 yeldarb   (1000) yeldarb   (1001)      442 2023-05-27 02:55:33.000000 autodistill_yolov8-0.1.0/autodistill_yolov8/yolov8.py
-drwxr-xr-x   0 yeldarb   (1000) yeldarb   (1001)        0 2023-05-27 03:02:18.000000 autodistill_yolov8-0.1.0/autodistill_yolov8.egg-info/
--rw-r--r--   0 yeldarb   (1000) yeldarb   (1001)      594 2023-05-27 03:02:18.000000 autodistill_yolov8-0.1.0/autodistill_yolov8.egg-info/PKG-INFO
--rw-r--r--   0 yeldarb   (1000) yeldarb   (1001)      306 2023-05-27 03:02:18.000000 autodistill_yolov8-0.1.0/autodistill_yolov8.egg-info/SOURCES.txt
--rw-r--r--   0 yeldarb   (1000) yeldarb   (1001)        1 2023-05-27 03:02:18.000000 autodistill_yolov8-0.1.0/autodistill_yolov8.egg-info/dependency_links.txt
--rw-r--r--   0 yeldarb   (1000) yeldarb   (1001)       85 2023-05-27 03:02:18.000000 autodistill_yolov8-0.1.0/autodistill_yolov8.egg-info/requires.txt
--rw-r--r--   0 yeldarb   (1000) yeldarb   (1001)       19 2023-05-27 03:02:18.000000 autodistill_yolov8-0.1.0/autodistill_yolov8.egg-info/top_level.txt
--rw-r--r--   0 yeldarb   (1000) yeldarb   (1001)       38 2023-05-27 03:02:18.000000 autodistill_yolov8-0.1.0/setup.cfg
--rw-r--r--   0 yeldarb   (1000) yeldarb   (1001)     1309 2023-05-27 02:55:33.000000 autodistill_yolov8-0.1.0/setup.py
-drwxr-xr-x   0 yeldarb   (1000) yeldarb   (1001)        0 2023-05-27 03:02:18.000000 autodistill_yolov8-0.1.0/test/
--rw-r--r--   0 yeldarb   (1000) yeldarb   (1001)       40 2023-05-27 02:55:33.000000 autodistill_yolov8-0.1.0/test/test_hello.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-07-02 19:49:15.964724 autodistill_yolov8-0.1.1/
+-rw-r--r--   0 james      (501) staff       (20)    34522 2023-06-08 06:15:45.000000 autodistill_yolov8-0.1.1/LICENSE
+-rw-r--r--   0 james      (501) staff       (20)      672 2023-07-02 19:49:15.964579 autodistill_yolov8-0.1.1/PKG-INFO
+-rw-r--r--   0 james      (501) staff       (20)     3503 2023-06-08 06:15:45.000000 autodistill_yolov8-0.1.1/README.md
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-07-02 19:49:15.963220 autodistill_yolov8-0.1.1/autodistill_yolov8/
+-rw-r--r--   0 james      (501) staff       (20)       68 2023-07-02 19:49:03.000000 autodistill_yolov8-0.1.1/autodistill_yolov8/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)      442 2023-06-08 06:20:26.000000 autodistill_yolov8-0.1.1/autodistill_yolov8/yolov8.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-07-02 19:49:15.964116 autodistill_yolov8-0.1.1/autodistill_yolov8.egg-info/
+-rw-r--r--   0 james      (501) staff       (20)      672 2023-07-02 19:49:15.000000 autodistill_yolov8-0.1.1/autodistill_yolov8.egg-info/PKG-INFO
+-rw-r--r--   0 james      (501) staff       (20)      314 2023-07-02 19:49:15.000000 autodistill_yolov8-0.1.1/autodistill_yolov8.egg-info/SOURCES.txt
+-rw-r--r--   0 james      (501) staff       (20)        1 2023-07-02 19:49:15.000000 autodistill_yolov8-0.1.1/autodistill_yolov8.egg-info/dependency_links.txt
+-rw-r--r--   0 james      (501) staff       (20)       97 2023-07-02 19:49:15.000000 autodistill_yolov8-0.1.1/autodistill_yolov8.egg-info/requires.txt
+-rw-r--r--   0 james      (501) staff       (20)       19 2023-07-02 19:49:15.000000 autodistill_yolov8-0.1.1/autodistill_yolov8.egg-info/top_level.txt
+-rw-r--r--   0 james      (501) staff       (20)       38 2023-07-02 19:49:15.964770 autodistill_yolov8-0.1.1/setup.cfg
+-rw-r--r--   0 james      (501) staff       (20)     1340 2023-07-02 19:48:26.000000 autodistill_yolov8-0.1.1/setup.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-07-02 19:49:15.964277 autodistill_yolov8-0.1.1/test/
+-rw-r--r--   0 james      (501) staff       (20)       40 2023-06-08 06:15:45.000000 autodistill_yolov8-0.1.1/test/test_hello.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `autodistill_yolov8-0.1.0/PKG-INFO` & `autodistill_yolov8-0.1.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: autodistill_yolov8
-Version: 0.1.0
+Version: 0.1.1
 Summary: Automatically distill large foundational models into smaller, in-domain models for deployment
-Home-page: https://www.youtube.com/watch?v=dQw4w9WgXcQ
+Home-page: https://github.com/autodistill/autodistill-yolov8
 Author: Roboflow
-Author-email: jacob@roboflow.com
+Author-email: autodistill@roboflow.com
 Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
+Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
+License-File: LICENSE
 
 Automatically distill large foundational models into smaller, in-domain models for deployment
```

### Comparing `autodistill_yolov8-0.1.0/autodistill_yolov8.egg-info/PKG-INFO` & `autodistill_yolov8-0.1.1/autodistill_yolov8.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: autodistill-yolov8
-Version: 0.1.0
+Version: 0.1.1
 Summary: Automatically distill large foundational models into smaller, in-domain models for deployment
-Home-page: https://www.youtube.com/watch?v=dQw4w9WgXcQ
+Home-page: https://github.com/autodistill/autodistill-yolov8
 Author: Roboflow
-Author-email: jacob@roboflow.com
+Author-email: autodistill@roboflow.com
 Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
+Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
+License-File: LICENSE
 
 Automatically distill large foundational models into smaller, in-domain models for deployment
```

### Comparing `autodistill_yolov8-0.1.0/setup.py` & `autodistill_yolov8-0.1.1/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,32 +5,33 @@
 with open("./autodistill_yolov8/__init__.py", 'r') as f:
     content = f.read()
     # from https://www.py4u.net/discuss/139845
     version = re.search(r'__version__\s*=\s*[\'"]([^\'"]*)[\'"]', content).group(1)
     
 with open("README.md", "r") as fh:
     long_description = fh.read()
-    
-with open("requirements.txt", "r") as fh:
-    install_requires = fh.read().split('\n')
 
 setuptools.setup(
     name="autodistill_yolov8",  
     version=version,
     author="Roboflow",
-    author_email="jacob@roboflow.com",
+    author_email="autodistill@roboflow.com",
     description="Automatically distill large foundational models into smaller, in-domain models for deployment",
     long_description="Automatically distill large foundational models into smaller, in-domain models for deployment",
     long_description_content_type="text/markdown",
-    url="https://www.youtube.com/watch?v=dQw4w9WgXcQ",
-    install_requires=install_requires,
+    url="https://github.com/autodistill/autodistill-yolov8",
+    install_requires=[
+        "autodistill",
+        "ultralytics==8.0.81",
+        "supervision"
+    ],
     packages=find_packages(exclude=("tests",)),
     extras_require={
         "dev": ["flake8", "black==22.3.0", "isort", "twine", "pytest", "wheel"],
     },
     classifiers=[
         "Programming Language :: Python :: 3",
-        "License :: OSI Approved :: MIT License",
+        "License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)",
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.7",
 )
```

