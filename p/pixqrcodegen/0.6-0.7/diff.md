# Comparing `tmp/pixqrcodegen-0.6.tar.gz` & `tmp/pixqrcodegen-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pixqrcodegen-0.6.tar", last modified: Thu Jun  1 15:23:39 2023, max compression
+gzip compressed data, was "pixqrcodegen-0.7.tar", last modified: Sun Jul  2 01:06:00 2023, max compression
```

## Comparing `pixqrcodegen-0.6.tar` & `pixqrcodegen-0.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 alexsussa  (1000) alexsussa  (1000)        0 2023-06-01 15:23:39.507767 pixqrcodegen-0.6/
--rwxrwxrwx   0 alexsussa  (1000) alexsussa  (1000)     1070 2022-09-15 18:59:18.000000 pixqrcodegen-0.6/LICENSE.txt
--rw-rw-r--   0 alexsussa  (1000) alexsussa  (1000)     2654 2023-06-01 15:23:39.507767 pixqrcodegen-0.6/PKG-INFO
--rwxrwxrwx   0 alexsussa  (1000) alexsussa  (1000)     2057 2023-06-01 15:06:22.000000 pixqrcodegen-0.6/README.md
-drwxrwxr-x   0 alexsussa  (1000) alexsussa  (1000)        0 2023-06-01 15:23:39.507767 pixqrcodegen-0.6/pixqrcodegen/
--rwxrwxrwx   0 alexsussa  (1000) alexsussa  (1000)       28 2022-09-15 20:30:52.000000 pixqrcodegen-0.6/pixqrcodegen/__init__.py
--rwxrwxrwx   0 alexsussa  (1000) alexsussa  (1000)     2562 2023-06-01 14:33:04.000000 pixqrcodegen-0.6/pixqrcodegen/pixqrcodegen.py
-drwxrwxr-x   0 alexsussa  (1000) alexsussa  (1000)        0 2023-06-01 15:23:39.507767 pixqrcodegen-0.6/pixqrcodegen.egg-info/
--rw-rw-r--   0 alexsussa  (1000) alexsussa  (1000)     2654 2023-06-01 15:23:39.000000 pixqrcodegen-0.6/pixqrcodegen.egg-info/PKG-INFO
--rw-rw-r--   0 alexsussa  (1000) alexsussa  (1000)      273 2023-06-01 15:23:39.000000 pixqrcodegen-0.6/pixqrcodegen.egg-info/SOURCES.txt
--rw-rw-r--   0 alexsussa  (1000) alexsussa  (1000)        1 2023-06-01 15:23:39.000000 pixqrcodegen-0.6/pixqrcodegen.egg-info/dependency_links.txt
--rw-rw-r--   0 alexsussa  (1000) alexsussa  (1000)       21 2023-06-01 15:23:39.000000 pixqrcodegen-0.6/pixqrcodegen.egg-info/requires.txt
--rw-rw-r--   0 alexsussa  (1000) alexsussa  (1000)       13 2023-06-01 15:23:39.000000 pixqrcodegen-0.6/pixqrcodegen.egg-info/top_level.txt
--rwxrwxrwx   0 alexsussa  (1000) alexsussa  (1000)      107 2023-06-01 15:23:39.507767 pixqrcodegen-0.6/setup.cfg
--rwxrwxrwx   0 alexsussa  (1000) alexsussa  (1000)      902 2023-06-01 14:32:41.000000 pixqrcodegen-0.6/setup.py
+drwxrwxr-x   0 alexsussa  (1000) alexsussa  (1000)        0 2023-07-02 01:06:00.763579 pixqrcodegen-0.7/
+-rw-r--r--   0 alexsussa  (1000) alexsussa  (1000)     1070 2022-09-15 18:59:18.000000 pixqrcodegen-0.7/LICENSE.txt
+-rw-rw-r--   0 alexsussa  (1000) alexsussa  (1000)     2654 2023-07-02 01:06:00.763579 pixqrcodegen-0.7/PKG-INFO
+-rw-r--r--   0 alexsussa  (1000) alexsussa  (1000)     2057 2023-06-01 15:06:22.000000 pixqrcodegen-0.7/README.md
+drwxrwxr-x   0 alexsussa  (1000) alexsussa  (1000)        0 2023-07-02 01:06:00.763579 pixqrcodegen-0.7/pixqrcodegen/
+-rw-r--r--   0 alexsussa  (1000) alexsussa  (1000)       28 2022-09-15 20:30:52.000000 pixqrcodegen-0.7/pixqrcodegen/__init__.py
+-rw-r--r--   0 alexsussa  (1000) alexsussa  (1000)     2576 2023-07-02 00:50:17.000000 pixqrcodegen-0.7/pixqrcodegen/pixqrcodegen.py
+drwxrwxr-x   0 alexsussa  (1000) alexsussa  (1000)        0 2023-07-02 01:06:00.763579 pixqrcodegen-0.7/pixqrcodegen.egg-info/
+-rw-r--r--   0 alexsussa  (1000) alexsussa  (1000)     2654 2023-07-02 01:06:00.000000 pixqrcodegen-0.7/pixqrcodegen.egg-info/PKG-INFO
+-rw-r--r--   0 alexsussa  (1000) alexsussa  (1000)      273 2023-07-02 01:06:00.000000 pixqrcodegen-0.7/pixqrcodegen.egg-info/SOURCES.txt
+-rw-r--r--   0 alexsussa  (1000) alexsussa  (1000)        1 2023-07-02 01:06:00.000000 pixqrcodegen-0.7/pixqrcodegen.egg-info/dependency_links.txt
+-rw-r--r--   0 alexsussa  (1000) alexsussa  (1000)       21 2023-07-02 01:06:00.000000 pixqrcodegen-0.7/pixqrcodegen.egg-info/requires.txt
+-rw-r--r--   0 alexsussa  (1000) alexsussa  (1000)       13 2023-07-02 01:06:00.000000 pixqrcodegen-0.7/pixqrcodegen.egg-info/top_level.txt
+-rw-r--r--   0 alexsussa  (1000) alexsussa  (1000)      107 2023-07-02 01:06:00.763579 pixqrcodegen-0.7/setup.cfg
+-rw-r--r--   0 alexsussa  (1000) alexsussa  (1000)      902 2023-07-02 01:05:48.000000 pixqrcodegen-0.7/setup.py
```

### Comparing `pixqrcodegen-0.6/LICENSE.txt` & `pixqrcodegen-0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pixqrcodegen-0.6/PKG-INFO` & `pixqrcodegen-0.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pixqrcodegen
-Version: 0.6
+Version: 0.7
 Summary: Gera a Payload do PIX e o QR Code
 Home-page: https://github.com/Alexsussa/pixqrcodegen
 Author: Alex Pinheiro
 License: MIT
 Keywords: qrcode,payload,qrcode-generator,pix,pix-payload-generator
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `pixqrcodegen-0.6/README.md` & `pixqrcodegen-0.7/README.md`

 * *Files identical despite different names*

### Comparing `pixqrcodegen-0.6/pixqrcodegen/pixqrcodegen.py` & `pixqrcodegen-0.7/pixqrcodegen/pixqrcodegen.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # -*- coding: utf-8 -*-
 
 import crcmod
 import qrcode
 
 
 class Payload():
-    def __init__(self, nome, chavepix, valor, cidade, txtId):
+    def __init__(self, nome, chavepix, valor, cidade, txtId, diretorio=''):
         
         self.nome = nome
         self.chavepix = chavepix
         self.valor = valor.replace(',', '.')
         self.cidade = cidade
         self.txtId = txtId
```

### Comparing `pixqrcodegen-0.6/pixqrcodegen.egg-info/PKG-INFO` & `pixqrcodegen-0.7/pixqrcodegen.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pixqrcodegen
-Version: 0.6
+Version: 0.7
 Summary: Gera a Payload do PIX e o QR Code
 Home-page: https://github.com/Alexsussa/pixqrcodegen
 Author: Alex Pinheiro
 License: MIT
 Keywords: qrcode,payload,qrcode-generator,pix,pix-payload-generator
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `pixqrcodegen-0.6/setup.py` & `pixqrcodegen-0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from setuptools import setup
 
 with open('README.md', 'r') as rm:
     full_desc = rm.read()
 
 setup(
     name="pixqrcodegen",
-    version="0.6",
+    version="0.7",
     author="Alex Pinheiro",
     url="https://github.com/Alexsussa/pixqrcodegen",
     packages=['pixqrcodegen'],
     description="Gera a Payload do PIX e o QR Code",
     long_description=full_desc,
     long_description_content_type='text/markdown',
     python_requires=">= 3.6",
```

