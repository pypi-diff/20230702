# Comparing `tmp/Andromeda-llm-0.0.1.tar.gz` & `tmp/Andromeda-llm-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Andromeda-llm-0.0.1.tar", last modified: Sun Jul  2 04:48:20 2023, max compression
+gzip compressed data, was "Andromeda-llm-0.0.2.tar", last modified: Sun Jul  2 04:56:18 2023, max compression
```

## Comparing `Andromeda-llm-0.0.1.tar` & `Andromeda-llm-0.0.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 04:48:20.067865 Andromeda-llm-0.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 04:48:20.067865 Andromeda-llm-0.0.1/Andromeda/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-02 04:48:10.000000 Andromeda-llm-0.0.1/Andromeda/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-07-02 04:48:10.000000 Andromeda-llm-0.0.1/Andromeda/build_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-07-02 04:48:10.000000 Andromeda-llm-0.0.1/Andromeda/inference.py
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-07-02 04:48:10.000000 Andromeda-llm-0.0.1/Andromeda/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 04:48:20.067865 Andromeda-llm-0.0.1/Andromeda/optimus_prime/
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-07-02 04:48:10.000000 Andromeda-llm-0.0.1/Andromeda/optimus_prime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7660 2023-07-02 04:48:10.000000 Andromeda-llm-0.0.1/Andromeda/optimus_prime/attend.py
--rw-r--r--   0 runner    (1001) docker     (123)     4523 2023-07-02 04:48:10.000000 Andromeda-llm-0.0.1/Andromeda/optimus_prime/autoregressive_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-07-02 04:48:10.000000 Andromeda-llm-0.0.1/Andromeda/optimus_prime/continuous_autoregressive_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    10414 2023-07-02 04:48:10.000000 Andromeda-llm-0.0.1/Andromeda/optimus_prime/nonautoregressive_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    55026 2023-07-02 04:48:10.000000 Andromeda-llm-0.0.1/Andromeda/optimus_prime/x_transformers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3987 2023-07-02 04:48:10.000000 Andromeda-llm-0.0.1/Andromeda/optimus_prime/xl_autoregressive_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    23943 2023-07-02 04:48:10.000000 Andromeda-llm-0.0.1/Andromeda/train_distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)    23620 2023-07-02 04:48:10.000000 Andromeda-llm-0.0.1/Andromeda/train_distributed_accelerate.py
--rw-r--r--   0 runner    (1001) docker     (123)    11404 2023-07-02 04:48:10.000000 Andromeda-llm-0.0.1/Andromeda/training.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 04:48:20.067865 Andromeda-llm-0.0.1/Andromeda_llm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-07-02 04:48:20.000000 Andromeda-llm-0.0.1/Andromeda_llm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-07-02 04:48:20.000000 Andromeda-llm-0.0.1/Andromeda_llm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 04:48:20.000000 Andromeda-llm-0.0.1/Andromeda_llm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-02 04:48:20.000000 Andromeda-llm-0.0.1/Andromeda_llm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-02 04:48:20.000000 Andromeda-llm-0.0.1/Andromeda_llm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-02 04:48:10.000000 Andromeda-llm-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-07-02 04:48:20.067865 Andromeda-llm-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9413 2023-07-02 04:48:10.000000 Andromeda-llm-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 04:48:20.067865 Andromeda-llm-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-07-02 04:48:10.000000 Andromeda-llm-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 04:56:18.778125 Andromeda-llm-0.0.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 04:56:18.774125 Andromeda-llm-0.0.2/Andromeda/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-02 04:56:09.000000 Andromeda-llm-0.0.2/Andromeda/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-07-02 04:56:09.000000 Andromeda-llm-0.0.2/Andromeda/build_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-07-02 04:56:09.000000 Andromeda-llm-0.0.2/Andromeda/inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-07-02 04:56:09.000000 Andromeda-llm-0.0.2/Andromeda/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 04:56:18.778125 Andromeda-llm-0.0.2/Andromeda/optimus_prime/
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-07-02 04:56:09.000000 Andromeda-llm-0.0.2/Andromeda/optimus_prime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7660 2023-07-02 04:56:09.000000 Andromeda-llm-0.0.2/Andromeda/optimus_prime/attend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4523 2023-07-02 04:56:09.000000 Andromeda-llm-0.0.2/Andromeda/optimus_prime/autoregressive_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-07-02 04:56:09.000000 Andromeda-llm-0.0.2/Andromeda/optimus_prime/continuous_autoregressive_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10414 2023-07-02 04:56:09.000000 Andromeda-llm-0.0.2/Andromeda/optimus_prime/nonautoregressive_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55026 2023-07-02 04:56:09.000000 Andromeda-llm-0.0.2/Andromeda/optimus_prime/x_transformers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3987 2023-07-02 04:56:09.000000 Andromeda-llm-0.0.2/Andromeda/optimus_prime/xl_autoregressive_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23945 2023-07-02 04:56:09.000000 Andromeda-llm-0.0.2/Andromeda/train_distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23620 2023-07-02 04:56:09.000000 Andromeda-llm-0.0.2/Andromeda/train_distributed_accelerate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11404 2023-07-02 04:56:09.000000 Andromeda-llm-0.0.2/Andromeda/training.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 04:56:18.778125 Andromeda-llm-0.0.2/Andromeda_llm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-07-02 04:56:18.000000 Andromeda-llm-0.0.2/Andromeda_llm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-07-02 04:56:18.000000 Andromeda-llm-0.0.2/Andromeda_llm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 04:56:18.000000 Andromeda-llm-0.0.2/Andromeda_llm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-02 04:56:18.000000 Andromeda-llm-0.0.2/Andromeda_llm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-02 04:56:18.000000 Andromeda-llm-0.0.2/Andromeda_llm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-02 04:56:09.000000 Andromeda-llm-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-07-02 04:56:18.778125 Andromeda-llm-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9721 2023-07-02 04:56:09.000000 Andromeda-llm-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 04:56:18.778125 Andromeda-llm-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-07-02 04:56:09.000000 Andromeda-llm-0.0.2/setup.py
```

### Comparing `Andromeda-llm-0.0.1/Andromeda/build_dataset.py` & `Andromeda-llm-0.0.2/Andromeda/build_dataset.py`

 * *Files identical despite different names*

### Comparing `Andromeda-llm-0.0.1/Andromeda/inference.py` & `Andromeda-llm-0.0.2/Andromeda/inference.py`

 * *Files identical despite different names*

### Comparing `Andromeda-llm-0.0.1/Andromeda/model.py` & `Andromeda-llm-0.0.2/Andromeda/model.py`

 * *Files identical despite different names*

### Comparing `Andromeda-llm-0.0.1/Andromeda/optimus_prime/__init__.py` & `Andromeda-llm-0.0.2/Andromeda/optimus_prime/__init__.py`

 * *Files identical despite different names*

### Comparing `Andromeda-llm-0.0.1/Andromeda/optimus_prime/attend.py` & `Andromeda-llm-0.0.2/Andromeda/optimus_prime/attend.py`

 * *Files identical despite different names*

### Comparing `Andromeda-llm-0.0.1/Andromeda/optimus_prime/autoregressive_wrapper.py` & `Andromeda-llm-0.0.2/Andromeda/optimus_prime/autoregressive_wrapper.py`

 * *Files identical despite different names*

### Comparing `Andromeda-llm-0.0.1/Andromeda/optimus_prime/continuous_autoregressive_wrapper.py` & `Andromeda-llm-0.0.2/Andromeda/optimus_prime/continuous_autoregressive_wrapper.py`

 * *Files identical despite different names*

### Comparing `Andromeda-llm-0.0.1/Andromeda/optimus_prime/nonautoregressive_wrapper.py` & `Andromeda-llm-0.0.2/Andromeda/optimus_prime/nonautoregressive_wrapper.py`

 * *Files identical despite different names*

### Comparing `Andromeda-llm-0.0.1/Andromeda/optimus_prime/x_transformers.py` & `Andromeda-llm-0.0.2/Andromeda/optimus_prime/x_transformers.py`

 * *Files identical despite different names*

### Comparing `Andromeda-llm-0.0.1/Andromeda/optimus_prime/xl_autoregressive_wrapper.py` & `Andromeda-llm-0.0.2/Andromeda/optimus_prime/xl_autoregressive_wrapper.py`

 * *Files identical despite different names*

### Comparing `Andromeda-llm-0.0.1/Andromeda/train_distributed.py` & `Andromeda-llm-0.0.2/Andromeda/train_distributed.py`

 * *Files 0% similar despite different names*

```diff
@@ -453,15 +453,15 @@
     # d3 = load_dataset("conceptofmind/c4_61-to-80_neox_with_eos_8k", split="train")
     # d4 = load_dataset("conceptofmind/c4_81-to-100_neox_with_eos_8k", split="train")
     # train_dataset = concatenate_datasets([d0, d1, d2, d3, d4])
     return d0
 
 
 
-def main():
+def Train():
     # accelerator
 
     timeout = InitProcessGroupKwargs(timeout=timedelta(seconds=1_000_000))
 
     accelerator = Accelerator(
         gradient_accumulation_steps=CFG.GRADIENT_ACCUMULATE_EVERY,
         mixed_precision="fp16",
@@ -672,8 +672,8 @@
         with accelerator.main_process_first():
             accelerator.save(
                 unwrapped_model.state_dict(), f"{CFG.OUTPUT_DIR}/final/final_model.pt"
             )
 
 
 if __name__ == "__main__":
-    main()
+    Train()
```

### Comparing `Andromeda-llm-0.0.1/Andromeda/train_distributed_accelerate.py` & `Andromeda-llm-0.0.2/Andromeda/train_distributed_accelerate.py`

 * *Files identical despite different names*

### Comparing `Andromeda-llm-0.0.1/Andromeda/training.py` & `Andromeda-llm-0.0.2/Andromeda/training.py`

 * *Files identical despite different names*

### Comparing `Andromeda-llm-0.0.1/Andromeda_llm.egg-info/PKG-INFO` & `Andromeda-llm-0.0.2/Andromeda_llm.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Andromeda-llm
-Version: 0.0.1
+Version: 0.0.2
 Summary: andromeda - Pytorch
 Home-page: https://github.com/kyegomez/Andromeda
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,attention mechanism,transformers
 Classifier: Development Status :: 4 - Beta
```

### Comparing `Andromeda-llm-0.0.1/Andromeda_llm.egg-info/SOURCES.txt` & `Andromeda-llm-0.0.2/Andromeda_llm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Andromeda-llm-0.0.1/LICENSE` & `Andromeda-llm-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `Andromeda-llm-0.0.1/PKG-INFO` & `Andromeda-llm-0.0.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Andromeda-llm
-Version: 0.0.1
+Version: 0.0.2
 Summary: andromeda - Pytorch
 Home-page: https://github.com/kyegomez/Andromeda
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,attention mechanism,transformers
 Classifier: Development Status :: 4 - Beta
```

### Comparing `Andromeda-llm-0.0.1/README.md` & `Andromeda-llm-0.0.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -16,14 +16,37 @@
 ![Andromeda Next Generation Open Source Language Model](/andromeda-banner.png)
 
 Andromeda is a state-of-the-art language model that pushes the boundaries of natural language understanding and generation. Designed for high performance and efficiency, Andromeda is built upon advanced techniques that make it a strong contender against the likes of OpenAI's GPT-4 and PALM.
 
 
 
 # Usage
+There are 2 methods to use Andromeda, 1 by `pip install Andromeda-llm` and the other by `git clone`
+
+# Method1
+First `pip install Andromeda-llm` then
+
+```python
+import torch
+from Andromeda import Andromeda, Train
+
+
+x = torch.randint(0, 20000, (1, 1024))
+
+Andromea(x)
+
+# or train
+
+Train()
+
+```
+
+
+## Method 2
+
 Get started:
 
 1. Clone the repository and install the required packages.
 
 
 ```
 git clone https://github.com/kyegomez/Andromeda
```

### Comparing `Andromeda-llm-0.0.1/setup.py` & `Andromeda-llm-0.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'Andromeda-llm',
   packages = find_packages(exclude=['examples']),
-  version = '0.0.1',
+  version = '0.0.2',
   license='MIT',
   description = 'andromeda - Pytorch',
   author = 'Kye Gomez',
   author_email = 'kye@apac.ai',
   url = 'https://github.com/kyegomez/Andromeda',
   long_description_content_type = 'text/markdown',
   keywords = [
```

