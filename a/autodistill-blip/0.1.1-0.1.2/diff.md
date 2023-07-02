# Comparing `tmp/autodistill-blip-0.1.1.tar.gz` & `tmp/autodistill-blip-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autodistill-blip-0.1.1.tar", last modified: Fri Jun 30 09:05:19 2023, max compression
+gzip compressed data, was "autodistill-blip-0.1.2.tar", last modified: Sun Jul  2 19:40:32 2023, max compression
```

## Comparing `autodistill-blip-0.1.1.tar` & `autodistill-blip-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-30 09:05:19.613621 autodistill-blip-0.1.1/
--rw-r--r--   0 james      (501) staff       (20)     1501 2023-06-12 11:34:19.000000 autodistill-blip-0.1.1/LICENSE
--rw-r--r--   0 james      (501) staff       (20)     2217 2023-06-30 09:05:19.613497 autodistill-blip-0.1.1/PKG-INFO
--rw-r--r--   0 james      (501) staff       (20)     1794 2023-06-30 09:02:51.000000 autodistill-blip-0.1.1/README.md
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-30 09:05:19.612538 autodistill-blip-0.1.1/autodistill_blip/
--rw-r--r--   0 james      (501) staff       (20)       62 2023-06-30 09:05:14.000000 autodistill-blip-0.1.1/autodistill_blip/__init__.py
--rw-r--r--   0 james      (501) staff       (20)     2808 2023-06-30 09:02:45.000000 autodistill-blip-0.1.1/autodistill_blip/blip.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-30 09:05:19.613310 autodistill-blip-0.1.1/autodistill_blip.egg-info/
--rw-r--r--   0 james      (501) staff       (20)     2217 2023-06-30 09:05:19.000000 autodistill-blip-0.1.1/autodistill_blip.egg-info/PKG-INFO
--rw-r--r--   0 james      (501) staff       (20)      279 2023-06-30 09:05:19.000000 autodistill-blip-0.1.1/autodistill_blip.egg-info/SOURCES.txt
--rw-r--r--   0 james      (501) staff       (20)        1 2023-06-30 09:05:19.000000 autodistill-blip-0.1.1/autodistill_blip.egg-info/dependency_links.txt
--rw-r--r--   0 james      (501) staff       (20)      108 2023-06-30 09:05:19.000000 autodistill-blip-0.1.1/autodistill_blip.egg-info/requires.txt
--rw-r--r--   0 james      (501) staff       (20)       17 2023-06-30 09:05:19.000000 autodistill-blip-0.1.1/autodistill_blip.egg-info/top_level.txt
--rw-r--r--   0 james      (501) staff       (20)       38 2023-06-30 09:05:19.613667 autodistill-blip-0.1.1/setup.cfg
--rw-r--r--   0 james      (501) staff       (20)     1134 2023-06-30 09:05:06.000000 autodistill-blip-0.1.1/setup.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-07-02 19:40:32.997350 autodistill-blip-0.1.2/
+-rw-r--r--   0 james      (501) staff       (20)     1501 2023-06-12 11:34:19.000000 autodistill-blip-0.1.2/LICENSE
+-rw-r--r--   0 james      (501) staff       (20)     2217 2023-07-02 19:40:32.997200 autodistill-blip-0.1.2/PKG-INFO
+-rw-r--r--   0 james      (501) staff       (20)     1794 2023-06-30 09:02:51.000000 autodistill-blip-0.1.2/README.md
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-07-02 19:40:32.996111 autodistill-blip-0.1.2/autodistill_blip/
+-rw-r--r--   0 james      (501) staff       (20)       62 2023-07-02 19:40:13.000000 autodistill-blip-0.1.2/autodistill_blip/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)     2732 2023-06-30 09:08:43.000000 autodistill-blip-0.1.2/autodistill_blip/blip.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-07-02 19:40:32.996989 autodistill-blip-0.1.2/autodistill_blip.egg-info/
+-rw-r--r--   0 james      (501) staff       (20)     2217 2023-07-02 19:40:32.000000 autodistill-blip-0.1.2/autodistill_blip.egg-info/PKG-INFO
+-rw-r--r--   0 james      (501) staff       (20)      279 2023-07-02 19:40:32.000000 autodistill-blip-0.1.2/autodistill_blip.egg-info/SOURCES.txt
+-rw-r--r--   0 james      (501) staff       (20)        1 2023-07-02 19:40:32.000000 autodistill-blip-0.1.2/autodistill_blip.egg-info/dependency_links.txt
+-rw-r--r--   0 james      (501) staff       (20)      108 2023-07-02 19:40:32.000000 autodistill-blip-0.1.2/autodistill_blip.egg-info/requires.txt
+-rw-r--r--   0 james      (501) staff       (20)       17 2023-07-02 19:40:32.000000 autodistill-blip-0.1.2/autodistill_blip.egg-info/top_level.txt
+-rw-r--r--   0 james      (501) staff       (20)       38 2023-07-02 19:40:32.997401 autodistill-blip-0.1.2/setup.cfg
+-rw-r--r--   0 james      (501) staff       (20)     1134 2023-06-30 09:05:06.000000 autodistill-blip-0.1.2/setup.py
```

### Comparing `autodistill-blip-0.1.1/LICENSE` & `autodistill-blip-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `autodistill-blip-0.1.1/PKG-INFO` & `autodistill-blip-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autodistill-blip
-Version: 0.1.1
+Version: 0.1.2
 Summary: BLIP module for use with Autodistill
 Home-page: 
 Author: Roboflow
 Author-email: support@roboflow.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `autodistill-blip-0.1.1/README.md` & `autodistill-blip-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `autodistill-blip-0.1.1/autodistill_blip/blip.py` & `autodistill-blip-0.1.2/autodistill_blip/blip.py`

 * *Files 6% similar despite different names*

```diff
@@ -53,17 +53,14 @@
     def predict(self, input: str) -> sv.Classifications:
         image = Image.open(input).convert("RGB")
 
         image = self.vis_processors["eval"](image).unsqueeze(0).to(DEVICE)
 
         classes = self.ontology.classes()
 
-        if len(classes) == 1:
-            classes.append("something else")
-
         text_processor = self.tokenizer(prompt="A picture of ")
 
         cls_prompt = [text_processor(cls_nm) for cls_nm in classes]
 
         sample = {"image": image, "text_input": cls_prompt}
 
         image_features = self.model.extract_features(
```

### Comparing `autodistill-blip-0.1.1/autodistill_blip.egg-info/PKG-INFO` & `autodistill-blip-0.1.2/autodistill_blip.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autodistill-blip
-Version: 0.1.1
+Version: 0.1.2
 Summary: BLIP module for use with Autodistill
 Home-page: 
 Author: Roboflow
 Author-email: support@roboflow.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `autodistill-blip-0.1.1/setup.py` & `autodistill-blip-0.1.2/setup.py`

 * *Files identical despite different names*

