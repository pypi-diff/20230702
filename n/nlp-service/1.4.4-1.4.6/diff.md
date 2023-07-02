# Comparing `tmp/nlp_service-1.4.4.tar.gz` & `tmp/nlp_service-1.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nlp_service-1.4.4.tar", max compression
+gzip compressed data, was "nlp_service-1.4.6.tar", max compression
```

## Comparing `nlp_service-1.4.4.tar` & `nlp_service-1.4.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1067 2023-06-29 13:28:53.760156 nlp_service-1.4.4/LICENSE
--rw-r--r--   0        0        0     7699 2023-06-29 13:28:53.760156 nlp_service-1.4.4/README.md
--rw-r--r--   0        0        0      226 2023-06-29 13:28:53.760156 nlp_service-1.4.4/nlp_service/__init__.py
--rw-r--r--   0        0        0       42 2023-06-29 13:28:53.760156 nlp_service-1.4.4/nlp_service/__main__.py
--rw-r--r--   0        0        0     2259 2023-06-29 13:28:53.760156 nlp_service-1.4.4/nlp_service/client.py
--rw-r--r--   0        0        0    10441 2023-06-29 13:28:53.760156 nlp_service-1.4.4/nlp_service/infersent.py
--rw-r--r--   0        0        0        0 2023-06-29 13:28:53.760156 nlp_service-1.4.4/nlp_service/py.typed
--rw-r--r--   0        0        0    17139 2023-06-29 13:28:53.760156 nlp_service-1.4.4/nlp_service/server.py
--rw-r--r--   0        0        0     9147 2023-06-29 13:28:53.760156 nlp_service-1.4.4/nlp_service/similarity.py
--rw-r--r--   0        0        0      344 2023-06-29 13:28:53.760156 nlp_service-1.4.4/nlp_service/typing.py
--rw-r--r--   0        0        0     1361 2023-06-29 13:29:21.196484 nlp_service-1.4.4/pyproject.toml
--rw-r--r--   0        0        0     9329 1970-01-01 00:00:00.000000 nlp_service-1.4.4/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-07-02 19:33:47.646233 nlp_service-1.4.6/LICENSE
+-rw-r--r--   0        0        0     7887 2023-07-02 19:33:47.646233 nlp_service-1.4.6/README.md
+-rw-r--r--   0        0        0      226 2023-07-02 19:33:47.646233 nlp_service-1.4.6/nlp_service/__init__.py
+-rw-r--r--   0        0        0       42 2023-07-02 19:33:47.646233 nlp_service-1.4.6/nlp_service/__main__.py
+-rw-r--r--   0        0        0     2259 2023-07-02 19:33:47.646233 nlp_service-1.4.6/nlp_service/client.py
+-rw-r--r--   0        0        0    10441 2023-07-02 19:33:47.646233 nlp_service-1.4.6/nlp_service/infersent.py
+-rw-r--r--   0        0        0        0 2023-07-02 19:33:47.646233 nlp_service-1.4.6/nlp_service/py.typed
+-rw-r--r--   0        0        0    17139 2023-07-02 19:33:47.646233 nlp_service-1.4.6/nlp_service/server.py
+-rw-r--r--   0        0        0     9147 2023-07-02 19:33:47.646233 nlp_service-1.4.6/nlp_service/similarity.py
+-rw-r--r--   0        0        0      344 2023-07-02 19:33:47.646233 nlp_service-1.4.6/nlp_service/typing.py
+-rw-r--r--   0        0        0     1361 2023-07-02 19:34:48.415220 nlp_service-1.4.6/pyproject.toml
+-rw-r--r--   0        0        0     9517 1970-01-01 00:00:00.000000 nlp_service-1.4.6/PKG-INFO
```

### Comparing `nlp_service-1.4.4/LICENSE` & `nlp_service-1.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `nlp_service-1.4.4/README.md` & `nlp_service-1.4.6/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -10,22 +10,29 @@
 
 In addition to the server, we also provide a client containing convenience functions.
 This makes it easier for python applications to interact with the gRPC server.
 We will discuss the client at the end of this README.
 
 ## Installation and Setup
 
-We are using `nix` and `poetry` to manage the dependencies.
-We will soon provide a pre-built docker image for simplify usage of the NLP service.
+We are using `nix` and `poetry` to manage the dependencies and provide a ready-to-use Docker image.
 
-### Nix (recommended)
+### Docker (recommended)
+
+The container caches the downloaded models, so you should not pass `--rm` to `docker run`.
+
+```sh
+docker run ghcr.io/recap-utr/nlp-service:latest "0.0.0.0:50100"
+```
+
+### Nix (advanced)
 
 ```sh
-nix run . -- "127.0.0.1:50100"
-# or alternatively
+nix run github:recap-utr/nlp-service -- "127.0.0.1:50100"
+# or after cloning this repository
 nix develop -c poetry run python -m nlp_service "127.0.0.1:50100"
 ```
 
 ### Poetry (advanced)
 
 ```sh
 # The server dependencies are optional, thus they have to be installed explicitly.
@@ -140,12 +147,12 @@
   # Please note that this particular method ignores your selected pooling method due to the fact that even plain word embeddings are not pooled at all.
   similarity_method=nlp_pb2.SimilarityMethod.SIMILARITY_METHOD_DYNAMAX_JACCARD
 )
 
 # It is also possible to determine a similarity score without the use of embeddings.
 config = nlp_pb2.NlpConfig(
   language="en",
-  spacy_model="en_core_web_lg",
+  spacy_model="en_core_web_sm",
   # Traditional metric (Jaccard similarity and Levenshtein edit distance) are also available
   similarity_method=nlp_pb2.SimilarityMethod.SIMILARITY_METHOD_EDIT
 )
 ```
```

### Comparing `nlp_service-1.4.4/nlp_service/client.py` & `nlp_service-1.4.6/nlp_service/client.py`

 * *Files identical despite different names*

### Comparing `nlp_service-1.4.4/nlp_service/infersent.py` & `nlp_service-1.4.6/nlp_service/infersent.py`

 * *Files identical despite different names*

### Comparing `nlp_service-1.4.4/nlp_service/server.py` & `nlp_service-1.4.6/nlp_service/server.py`

 * *Files identical despite different names*

### Comparing `nlp_service-1.4.4/nlp_service/similarity.py` & `nlp_service-1.4.6/nlp_service/similarity.py`

 * *Files identical despite different names*

### Comparing `nlp_service-1.4.4/pyproject.toml` & `nlp_service-1.4.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nlp-service"
-version = "1.4.4"
+version = "1.4.6"
 description = "Microservice for NLP tasks using gRPC"
 authors = ["Mirko Lenz <info@mirko-lenz.de>"]
 license = "MIT"
 readme = "README.md"
 homepage = "http://recap.uni-trier.de"
 repository = "https://github.com/recap-utr/nlp-service"
 packages = [{ include = "nlp_service" }]
```

### Comparing `nlp_service-1.4.4/PKG-INFO` & `nlp_service-1.4.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlp-service
-Version: 1.4.4
+Version: 1.4.6
 Summary: Microservice for NLP tasks using gRPC
 Home-page: http://recap.uni-trier.de
 License: MIT
 Author: Mirko Lenz
 Author-email: info@mirko-lenz.de
 Requires-Python: >=3.10,<3.12
 Classifier: License :: OSI Approved :: MIT License
@@ -47,22 +47,29 @@
 
 In addition to the server, we also provide a client containing convenience functions.
 This makes it easier for python applications to interact with the gRPC server.
 We will discuss the client at the end of this README.
 
 ## Installation and Setup
 
-We are using `nix` and `poetry` to manage the dependencies.
-We will soon provide a pre-built docker image for simplify usage of the NLP service.
+We are using `nix` and `poetry` to manage the dependencies and provide a ready-to-use Docker image.
 
-### Nix (recommended)
+### Docker (recommended)
+
+The container caches the downloaded models, so you should not pass `--rm` to `docker run`.
+
+```sh
+docker run ghcr.io/recap-utr/nlp-service:latest "0.0.0.0:50100"
+```
+
+### Nix (advanced)
 
 ```sh
-nix run . -- "127.0.0.1:50100"
-# or alternatively
+nix run github:recap-utr/nlp-service -- "127.0.0.1:50100"
+# or after cloning this repository
 nix develop -c poetry run python -m nlp_service "127.0.0.1:50100"
 ```
 
 ### Poetry (advanced)
 
 ```sh
 # The server dependencies are optional, thus they have to be installed explicitly.
@@ -177,13 +184,13 @@
   # Please note that this particular method ignores your selected pooling method due to the fact that even plain word embeddings are not pooled at all.
   similarity_method=nlp_pb2.SimilarityMethod.SIMILARITY_METHOD_DYNAMAX_JACCARD
 )
 
 # It is also possible to determine a similarity score without the use of embeddings.
 config = nlp_pb2.NlpConfig(
   language="en",
-  spacy_model="en_core_web_lg",
+  spacy_model="en_core_web_sm",
   # Traditional metric (Jaccard similarity and Levenshtein edit distance) are also available
   similarity_method=nlp_pb2.SimilarityMethod.SIMILARITY_METHOD_EDIT
 )
 ```
```

