# Comparing `tmp/cval-lib-0.0.0.1.tar.gz` & `tmp/cval-lib-0.0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cval-lib-0.0.0.1.tar", last modified: Thu Jun 29 10:20:59 2023, max compression
+gzip compressed data, was "cval-lib-0.0.1.2.tar", last modified: Sun Jul  2 18:45:51 2023, max compression
```

## Comparing `cval-lib-0.0.0.1.tar` & `cval-lib-0.0.1.2.tar`

### file list

```diff
@@ -1,40 +1,42 @@
-drwxrwxr-x   0 localhost  (1000) localhost  (1000)        0 2023-06-29 10:20:59.577180 cval-lib-0.0.0.1/
--rw-rw-r--   0 localhost  (1000) localhost  (1000)    11357 2023-06-29 09:48:08.000000 cval-lib-0.0.0.1/LICENSE
--rw-rw-r--   0 localhost  (1000) localhost  (1000)      202 2023-06-29 10:20:59.577180 cval-lib-0.0.0.1/PKG-INFO
--rw-rw-r--   0 localhost  (1000) localhost  (1000)     5473 2023-06-29 09:48:08.000000 cval-lib-0.0.0.1/README.md
-drwxrwxr-x   0 localhost  (1000) localhost  (1000)        0 2023-06-29 10:20:59.577180 cval-lib-0.0.0.1/cval_lib/
--rw-rw-r--   0 localhost  (1000) localhost  (1000)        0 2023-06-29 09:48:08.000000 cval-lib-0.0.0.1/cval_lib/__init__.py
-drwxrwxr-x   0 localhost  (1000) localhost  (1000)        0 2023-06-29 10:20:59.577180 cval-lib-0.0.0.1/cval_lib/configs/
--rw-rw-r--   0 localhost  (1000) localhost  (1000)        0 2023-06-29 09:48:08.000000 cval-lib-0.0.0.1/cval_lib/configs/__init__.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)      128 2023-06-29 09:48:08.000000 cval-lib-0.0.0.1/cval_lib/configs/main_config.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)     1428 2023-06-29 09:48:08.000000 cval-lib-0.0.0.1/cval_lib/connection.py
-drwxrwxr-x   0 localhost  (1000) localhost  (1000)        0 2023-06-29 10:20:59.577180 cval-lib-0.0.0.1/cval_lib/examples/
--rw-rw-r--   0 localhost  (1000) localhost  (1000)        0 2023-06-29 09:48:08.000000 cval-lib-0.0.0.1/cval_lib/examples/__init__.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)      622 2023-06-29 09:48:08.000000 cval-lib-0.0.0.1/cval_lib/examples/dataset.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)      259 2023-06-29 09:48:08.000000 cval-lib-0.0.0.1/cval_lib/examples/monkey_patch.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)     1344 2023-06-29 09:48:08.000000 cval-lib-0.0.0.1/cval_lib/examples/result.py
-drwxrwxr-x   0 localhost  (1000) localhost  (1000)        0 2023-06-29 10:20:59.577180 cval-lib-0.0.0.1/cval_lib/handlers/
--rw-rw-r--   0 localhost  (1000) localhost  (1000)     1260 2023-06-29 09:48:08.000000 cval-lib-0.0.0.1/cval_lib/handlers/__async.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)        0 2023-06-29 09:48:08.000000 cval-lib-0.0.0.1/cval_lib/handlers/__init__.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)     2366 2023-06-29 09:48:08.000000 cval-lib-0.0.0.1/cval_lib/handlers/_abstract_handler.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)     5018 2023-06-29 09:48:08.000000 cval-lib-0.0.0.1/cval_lib/handlers/dataset.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)     1906 2023-06-29 09:48:08.000000 cval-lib-0.0.0.1/cval_lib/handlers/detection.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)     5074 2023-06-29 09:48:08.000000 cval-lib-0.0.0.1/cval_lib/handlers/embedding.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)     2439 2023-06-29 09:48:08.000000 cval-lib-0.0.0.1/cval_lib/handlers/result.py
-drwxrwxr-x   0 localhost  (1000) localhost  (1000)        0 2023-06-29 10:20:59.577180 cval-lib-0.0.0.1/cval_lib/models/
--rw-rw-r--   0 localhost  (1000) localhost  (1000)        0 2023-06-29 09:48:08.000000 cval-lib-0.0.0.1/cval_lib/models/__init__.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)     1914 2023-06-29 09:48:08.000000 cval-lib-0.0.0.1/cval_lib/models/dataset.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)     3027 2023-06-29 09:48:08.000000 cval-lib-0.0.0.1/cval_lib/models/detection.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)     1403 2023-06-29 09:48:08.000000 cval-lib-0.0.0.1/cval_lib/models/embedding.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)     2167 2023-06-29 09:48:08.000000 cval-lib-0.0.0.1/cval_lib/models/result.py
-drwxrwxr-x   0 localhost  (1000) localhost  (1000)        0 2023-06-29 10:20:59.577180 cval-lib-0.0.0.1/cval_lib/patterns/
--rw-rw-r--   0 localhost  (1000) localhost  (1000)        0 2023-06-29 09:48:08.000000 cval-lib-0.0.0.1/cval_lib/patterns/__init__.py
--rw-rw-r--   0 localhost  (1000) localhost  (1000)      240 2023-06-29 09:48:08.000000 cval-lib-0.0.0.1/cval_lib/patterns/singleton.py
-drwxrwxr-x   0 localhost  (1000) localhost  (1000)        0 2023-06-29 10:20:59.577180 cval-lib-0.0.0.1/cval_lib.egg-info/
--rw-rw-r--   0 localhost  (1000) localhost  (1000)      202 2023-06-29 10:20:59.000000 cval-lib-0.0.0.1/cval_lib.egg-info/PKG-INFO
--rw-rw-r--   0 localhost  (1000) localhost  (1000)      926 2023-06-29 10:20:59.000000 cval-lib-0.0.0.1/cval_lib.egg-info/SOURCES.txt
--rw-rw-r--   0 localhost  (1000) localhost  (1000)        1 2023-06-29 10:20:59.000000 cval-lib-0.0.0.1/cval_lib.egg-info/dependency_links.txt
--rw-rw-r--   0 localhost  (1000) localhost  (1000)       18 2023-06-29 10:20:59.000000 cval-lib-0.0.0.1/cval_lib.egg-info/requires.txt
--rw-rw-r--   0 localhost  (1000) localhost  (1000)        9 2023-06-29 10:20:59.000000 cval-lib-0.0.0.1/cval_lib.egg-info/top_level.txt
--rw-rw-r--   0 localhost  (1000) localhost  (1000)       38 2023-06-29 10:20:59.577180 cval-lib-0.0.0.1/setup.cfg
--rw-rw-r--   0 localhost  (1000) localhost  (1000)      446 2023-06-29 10:20:44.000000 cval-lib-0.0.0.1/setup.py
+drwxrwxr-x   0 localhost  (1000) localhost  (1000)        0 2023-07-02 18:45:51.574573 cval-lib-0.0.1.2/
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)    11357 2023-06-29 09:48:08.000000 cval-lib-0.0.1.2/LICENSE
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)      202 2023-07-02 18:45:51.574573 cval-lib-0.0.1.2/PKG-INFO
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)     5555 2023-07-02 18:44:46.000000 cval-lib-0.0.1.2/README.md
+drwxrwxr-x   0 localhost  (1000) localhost  (1000)        0 2023-07-02 18:45:51.574573 cval-lib-0.0.1.2/cval_lib/
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)        0 2023-07-02 18:05:48.000000 cval-lib-0.0.1.2/cval_lib/__init__.py
+drwxrwxr-x   0 localhost  (1000) localhost  (1000)        0 2023-07-02 18:45:51.574573 cval-lib-0.0.1.2/cval_lib/configs/
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)        0 2023-06-29 09:48:08.000000 cval-lib-0.0.1.2/cval_lib/configs/__init__.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)      137 2023-07-02 13:22:21.000000 cval-lib-0.0.1.2/cval_lib/configs/main_config.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)     1428 2023-06-29 09:48:08.000000 cval-lib-0.0.1.2/cval_lib/connection.py
+drwxrwxr-x   0 localhost  (1000) localhost  (1000)        0 2023-07-02 18:45:51.574573 cval-lib-0.0.1.2/cval_lib/examples/
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)        0 2023-06-29 09:48:08.000000 cval-lib-0.0.1.2/cval_lib/examples/__init__.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)     1685 2023-07-02 18:45:46.000000 cval-lib-0.0.1.2/cval_lib/examples/dataset.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)      820 2023-07-02 18:35:48.000000 cval-lib-0.0.1.2/cval_lib/examples/embeddings.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)     1313 2023-07-02 18:34:57.000000 cval-lib-0.0.1.2/cval_lib/examples/monkey_patch.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)     2012 2023-07-02 18:34:57.000000 cval-lib-0.0.1.2/cval_lib/examples/on_pemise.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)     1306 2023-07-02 18:45:46.000000 cval-lib-0.0.1.2/cval_lib/examples/result.py
+drwxrwxr-x   0 localhost  (1000) localhost  (1000)        0 2023-07-02 18:45:51.574573 cval-lib-0.0.1.2/cval_lib/handlers/
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)     1260 2023-06-29 09:48:08.000000 cval-lib-0.0.1.2/cval_lib/handlers/__async.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)        0 2023-06-29 09:48:08.000000 cval-lib-0.0.1.2/cval_lib/handlers/__init__.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)     2743 2023-07-02 18:41:52.000000 cval-lib-0.0.1.2/cval_lib/handlers/_abstract_handler.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)     5155 2023-07-02 18:28:19.000000 cval-lib-0.0.1.2/cval_lib/handlers/dataset.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)     1875 2023-07-02 18:19:25.000000 cval-lib-0.0.1.2/cval_lib/handlers/detection.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)     5250 2023-07-02 18:30:35.000000 cval-lib-0.0.1.2/cval_lib/handlers/embedding.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)     2478 2023-07-02 18:08:51.000000 cval-lib-0.0.1.2/cval_lib/handlers/result.py
+drwxrwxr-x   0 localhost  (1000) localhost  (1000)        0 2023-07-02 18:45:51.574573 cval-lib-0.0.1.2/cval_lib/models/
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)        0 2023-06-29 09:48:08.000000 cval-lib-0.0.1.2/cval_lib/models/__init__.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)     1914 2023-06-29 09:48:08.000000 cval-lib-0.0.1.2/cval_lib/models/dataset.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)     3040 2023-07-02 14:57:53.000000 cval-lib-0.0.1.2/cval_lib/models/detection.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)     1404 2023-07-02 18:41:52.000000 cval-lib-0.0.1.2/cval_lib/models/embedding.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)     2214 2023-07-02 18:22:01.000000 cval-lib-0.0.1.2/cval_lib/models/result.py
+drwxrwxr-x   0 localhost  (1000) localhost  (1000)        0 2023-07-02 18:45:51.574573 cval-lib-0.0.1.2/cval_lib/patterns/
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)        0 2023-06-29 09:48:08.000000 cval-lib-0.0.1.2/cval_lib/patterns/__init__.py
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)      240 2023-06-29 09:48:08.000000 cval-lib-0.0.1.2/cval_lib/patterns/singleton.py
+drwxrwxr-x   0 localhost  (1000) localhost  (1000)        0 2023-07-02 18:45:51.574573 cval-lib-0.0.1.2/cval_lib.egg-info/
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)      202 2023-07-02 18:45:51.000000 cval-lib-0.0.1.2/cval_lib.egg-info/PKG-INFO
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)      993 2023-07-02 18:45:51.000000 cval-lib-0.0.1.2/cval_lib.egg-info/SOURCES.txt
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)        1 2023-07-02 18:45:51.000000 cval-lib-0.0.1.2/cval_lib.egg-info/dependency_links.txt
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)       18 2023-07-02 18:45:51.000000 cval-lib-0.0.1.2/cval_lib.egg-info/requires.txt
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)        9 2023-07-02 18:45:51.000000 cval-lib-0.0.1.2/cval_lib.egg-info/top_level.txt
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)       38 2023-07-02 18:45:51.574573 cval-lib-0.0.1.2/setup.cfg
+-rw-rw-r--   0 localhost  (1000) localhost  (1000)      446 2023-07-02 18:43:19.000000 cval-lib-0.0.1.2/setup.py
```

### Comparing `cval-lib-0.0.0.1/LICENSE` & `cval-lib-0.0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cval-lib-0.0.0.1/README.md` & `cval-lib-0.0.1.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -68,17 +68,17 @@
 3. _Model layer._ If the data structure changes, only this layer changes.
 
 ## Examples
 
 ##### Set your user_api_key
 
 ```python3
-from cval_lib import CVALConnection
+from cval_lib.connection import CVALConnection
 USER_API_KEY='awesome_api_key'
-cval = CVALConnection(api_key)
+cval = CVALConnection(USER_API_KEY)
 ```
 
 > The same actions are available with the rest of the entities, but there are some nuances, for example, somewhere there is the use of models, and somewhere only parameters. But anyway, these examples well reflect possible scenarios when working with cval. The most typical api scenario is a dataset, so let's start with it.
 
 ### Dataset
  > Within the framework of the created system, datasets are spaces in which data for machine learning is stored.
  Creating a dataset is similar to creating a folder.
@@ -86,52 +86,56 @@
 ```python3
 # :NOTE: To avoid incomprehensibility of errors, it is recommended to use  CVALConnection
 ds_id = cval.dataset().create(name='on-premise-scheme-ds', description='')
 print(ds_id)
 ```
 
 ##### Update dataset
-```python
+```python3
 ds = cval.dataset()
 print(ds.update(ds_id, description='any string data'))
 # :NOTE: the dataset can store the state (ds_id)
 ds.update(name='sample name')
 ```
 
 ##### Get dataset
-```python
+```python3
 print(ds.get())
 ```
 
 > A further example of using the library concerns embedding. Since embedding is a large data object and the method of its creation is completely defined by the user, the embedding method works through query schemes (models).
 
 ### Embeddings
 
 > Embeddings are vector representations of images obtained using pytorch or any other library
 
 ##### Create embeddings
 
-```python
+```python3
 from random import random
 import uuid
 from cval_lib.models.embedding import ImageEmbeddingModel
 
-img_id_1 = str(uuid.uuid4())
-img_id_2 = str(uuid.uuid4())
+img_id_1 = str(uuid.uuid4().hex)
+img_id_2 = str(uuid.uuid4().hex)
+
 
 embeddings = [
- ImageEmbeddingModel(id=img_id_1, image_embedding=list(map(random, range(1000)))), 
- ImageEmbeddingModel(id=img_id_2, image_embedding=list(map(random, range(1000)))),
+ ImageEmbeddingModel(id=img_id_1, image_embedding=list(map(lambda x:random(), range(1000)))),
+ ImageEmbeddingModel(id=img_id_2, image_embedding=list(map(lambda x: random(), range(1000)))),
 ]
+
+print(embeddings)
 ```
 
 
 ##### Upload & check embeddings
-```python
-emb = cval.embedding(ds_id)
+
+```python3
+emb = cval.embedding(ds_id, 'training')
 emb.upload_many(embeddings)
 print(emb.get_many())
 ```
 
 > The following example is used to invoke active learning
 
 ### Active learning
@@ -159,19 +163,19 @@
 
 ```
 
 ##### Construct config
 
 ```python3
 from cval_lib.models.detection import DetectionSamplingOnPremise
-response_model = DetectionSamplingOnPremise(
+request = DetectionSamplingOnPremise(
  num_of_samples=200, 
  bbox_selection_policy='min', 
  selection_strategy='margin', 
- sort_strategy='max',
+ sort_strategy='ascending',
  frames=frames_predictions,
 )
 ```
 
 ##### Run active learning
 ```python3
 emb = cval.detection()
```

#### html2text {}

```diff
@@ -20,51 +20,51 @@
 install cval-lib.tar ``` #### Submodule ```shell git submodule add https://
 github.com/fangorntreabeard/cval-lib.git cval ``` ## Architecture The library
 architecture consists of **three layers**: 1. _A layer of protocols and
 abstract handlers_. Responsible for the use of a particular library. If an
 error is found, it is enough to simply change one method. 2. _A layer of
 handlers._ These are all the methods that are present in the API. Are based on
 abstract 3. _Model layer._ If the data structure changes, only this layer
-changes. ## Examples ##### Set your user_api_key ```python3 from cval_lib
-import CVALConnection USER_API_KEY='awesome_api_key' cval = CVALConnection
-(api_key) ``` > The same actions are available with the rest of the entities,
-but there are some nuances, for example, somewhere there is the use of models,
-and somewhere only parameters. But anyway, these examples well reflect possible
-scenarios when working with cval. The most typical api scenario is a dataset,
-so let's start with it. ### Dataset > Within the framework of the created
-system, datasets are spaces in which data for machine learning is stored.
-Creating a dataset is similar to creating a folder. ##### Create dataset
-```python3 # :NOTE: To avoid incomprehensibility of errors, it is recommended
-to use CVALConnection ds_id = cval.dataset().create(name='on-premise-scheme-
-ds', description='') print(ds_id) ``` ##### Update dataset ```python ds =
-cval.dataset() print(ds.update(ds_id, description='any string data')) # :NOTE:
-the dataset can store the state (ds_id) ds.update(name='sample name') ``` #####
-Get dataset ```python print(ds.get()) ``` > A further example of using the
-library concerns embedding. Since embedding is a large data object and the
-method of its creation is completely defined by the user, the embedding method
-works through query schemes (models). ### Embeddings > Embeddings are vector
-representations of images obtained using pytorch or any other library #####
-Create embeddings ```python from random import random import uuid from
+changes. ## Examples ##### Set your user_api_key ```python3 from
+cval_lib.connection import CVALConnection USER_API_KEY='awesome_api_key' cval =
+CVALConnection(USER_API_KEY) ``` > The same actions are available with the rest
+of the entities, but there are some nuances, for example, somewhere there is
+the use of models, and somewhere only parameters. But anyway, these examples
+well reflect possible scenarios when working with cval. The most typical api
+scenario is a dataset, so let's start with it. ### Dataset > Within the
+framework of the created system, datasets are spaces in which data for machine
+learning is stored. Creating a dataset is similar to creating a folder. #####
+Create dataset ```python3 # :NOTE: To avoid incomprehensibility of errors, it
+is recommended to use CVALConnection ds_id = cval.dataset().create(name='on-
+premise-scheme-ds', description='') print(ds_id) ``` ##### Update dataset
+```python3 ds = cval.dataset() print(ds.update(ds_id, description='any string
+data')) # :NOTE: the dataset can store the state (ds_id) ds.update(name='sample
+name') ``` ##### Get dataset ```python3 print(ds.get()) ``` > A further example
+of using the library concerns embedding. Since embedding is a large data object
+and the method of its creation is completely defined by the user, the embedding
+method works through query schemes (models). ### Embeddings > Embeddings are
+vector representations of images obtained using pytorch or any other library
+##### Create embeddings ```python3 from random import random import uuid from
 cval_lib.models.embedding import ImageEmbeddingModel img_id_1 = str(uuid.uuid4
-()) img_id_2 = str(uuid.uuid4()) embeddings = [ ImageEmbeddingModel
-(id=img_id_1, image_embedding=list(map(random, range(1000)))),
-ImageEmbeddingModel(id=img_id_2, image_embedding=list(map(random, range
-(1000)))), ] ``` ##### Upload & check embeddings ```python emb = cval.embedding
-(ds_id) emb.upload_many(embeddings) print(emb.get_many()) ``` > The following
-example is used to invoke active learning ### Active learning ##### Get
-predictions data ```python3 import random import uuid from
-cval_lib.models.detection import BBoxScores, FramePrediction # :NOTE: example
-only frames_predictions = list( map( lambda x: FramePrediction( frame_id=str
-(uuid.uuid4()), predictions=list(map(lambda x: BBoxScores(category_id=str
-(uuid.uuid4()), random.random()), range(100))) ), range(100) ) ) print
-(frames_predictions) ``` ##### Construct config ```python3 from
-cval_lib.models.detection import DetectionSamplingOnPremise response_model =
+().hex) img_id_2 = str(uuid.uuid4().hex) embeddings = [ ImageEmbeddingModel
+(id=img_id_1, image_embedding=list(map(lambda x:random(), range(1000)))),
+ImageEmbeddingModel(id=img_id_2, image_embedding=list(map(lambda x: random(),
+range(1000)))), ] print(embeddings) ``` ##### Upload & check embeddings
+```python3 emb = cval.embedding(ds_id, 'training') emb.upload_many(embeddings)
+print(emb.get_many()) ``` > The following example is used to invoke active
+learning ### Active learning ##### Get predictions data ```python3 import
+random import uuid from cval_lib.models.detection import BBoxScores,
+FramePrediction # :NOTE: example only frames_predictions = list( map( lambda x:
+FramePrediction( frame_id=str(uuid.uuid4()), predictions=list(map(lambda x:
+BBoxScores(category_id=str(uuid.uuid4()), random.random()), range(100))) ),
+range(100) ) ) print(frames_predictions) ``` ##### Construct config ```python3
+from cval_lib.models.detection import DetectionSamplingOnPremise request =
 DetectionSamplingOnPremise( num_of_samples=200, bbox_selection_policy='min',
-selection_strategy='margin', sort_strategy='max', frames=frames_predictions, )
-``` ##### Run active learning ```python3 emb = cval.detection() print
-(emd.on_premise_sampling(response_model)) ``` > The following method is most
-relevant when we are dealing with long-term tasks and, accordingly, with
-asynchronous interaction. ##### Polling > refers to actively sampling the
-status of an external device by a client program as a synchronous activity.
-```python3 from time import sleep result = None sleep_sec = 1 while result is
-None: result = emb.result.get_result() sleep(sleep_sec) sleep_sec *= 2 print
-(result) ```
+selection_strategy='margin', sort_strategy='ascending',
+frames=frames_predictions, ) ``` ##### Run active learning ```python3 emb =
+cval.detection() print(emd.on_premise_sampling(response_model)) ``` > The
+following method is most relevant when we are dealing with long-term tasks and,
+accordingly, with asynchronous interaction. ##### Polling > refers to actively
+sampling the status of an external device by a client program as a synchronous
+activity. ```python3 from time import sleep result = None sleep_sec = 1 while
+result is None: result = emb.result.get_result() sleep(sleep_sec) sleep_sec *=
+2 print(result) ```
```

### Comparing `cval-lib-0.0.0.1/cval_lib/connection.py` & `cval-lib-0.0.1.2/cval_lib/connection.py`

 * *Files identical despite different names*

### Comparing `cval-lib-0.0.0.1/cval_lib/examples/result.py` & `cval-lib-0.0.1.2/cval_lib/examples/monkey_patch.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 
 Our service makes it easy to implement this workflow and improve your models quickly and efficiently.
 Try our demo notebook to see how CVAL can revolutionize your computer vision projects.
 
 To obtain a client_api_key, please send a request to k.suhorukov@digital-quarters.com
 """
 
-from cval_lib.connection import CVALConnection
 
 if __name__ == '__main__':
-    api_key = 'a42a3a750b2dfab2f90ef64e75ba99a7c49a6c3f427d762236459d87e6766af1'
+    from cval_lib.connection import CVALConnection
+    api_key = '1d770d0b3f5898ec9e24c5422480b2419b9363852fc14a2e8881de2c6e43b82a'
     cval = CVALConnection(api_key)
-    print(cval.result().get_results())
-    cval.result().get_result(cval.result().get_results()[0].result_id)
+    ds = cval.dataset()
+    ds.create()
+    print(ds.result.get_results())
```

### Comparing `cval-lib-0.0.0.1/cval_lib/handlers/__async.py` & `cval-lib-0.0.1.2/cval_lib/handlers/__async.py`

 * *Files identical despite different names*

### Comparing `cval-lib-0.0.0.1/cval_lib/handlers/_abstract_handler.py` & `cval-lib-0.0.1.2/cval_lib/handlers/_abstract_handler.py`

 * *Files 8% similar despite different names*

```diff
@@ -53,13 +53,23 @@
     def _put(self, url: str, json=None, params=None):
         self._post(url, json, params)
         self.method = 'put'
 
     @staticmethod
     def validate_response(resp: Response):
         if resp.status_code >= 400:
-            raise Exception(resp.json() if resp.status_code != 500 else 'Internal Server Error :(')
+            match resp.status_code:
+                case 422:
+                    raise ValueError(resp.json())
+                case 403:
+                    raise PermissionError(resp.json())
+                case 409:
+                    raise ValueError(resp.json())
+                case 400:
+                    raise ValueError(resp.json())
+                case _:
+                    raise Exception(resp.json() if resp.status_code != 500 else 'Internal Server Error :(')
 
     def send(self):
         resp = self.session.send(self.prepare())
         self.validate_response(resp)
         return resp
```

### Comparing `cval-lib-0.0.0.1/cval_lib/handlers/dataset.py` & `cval-lib-0.0.1.2/cval_lib/handlers/dataset.py`

 * *Files 8% similar despite different names*

```diff
@@ -34,15 +34,16 @@
     Creating a dataset is similar to creating a folder.
     """
     def __init__(self, session: Session):
         self.dataset_request = DatasetModel
         self.route = f'{MainConfig().main_url}/dataset'
         self.dataset_id = None
         self.result = Result(session)
-        self.embedding = Embedding(session, _is_not_second=False).monkey_patch_url
+        self._embedding = Embedding(session, _is_not_second=False)
+        self.embedding = self._embedding.monkey_patch_url
         self.detection = Detection(session)
         super().__init__(session)
 
     def __repr__(self):
         return f'<dataset {self.dataset_id}>'
 
     def _construct_request(self, name: str, description: str):
@@ -62,22 +63,23 @@
         :param name: the name of dataset
         :param description: the name of dataset
         :return: id of dataset (dataset_id)
         """
         self._construct_request(name, description)
         self._post(url=self.route, json=self.dataset_request().dict())
         self.dataset_id = self.send().json().get('dataset_id')
+        self._embedding.dataset_id = self.dataset_id
         return self.dataset_id
 
     def update(
             self,
             dataset_id: str = None,
             name: str = None,
             description: str = None,
-    ) -> DatasetResponse:
+    ) -> DatasetModel:
         """
         this method updates a dataset
         :param dataset_id: id of dataset
         :param name: the name of dataset
         :param description: the description of dataset
         :return: DatasetResponse model with updates
         """
@@ -90,20 +92,21 @@
 
     def set_dataset_id(self, dataset_id: str = None):
         if dataset_id is None:
             dataset_id = self.dataset_id
         self.dataset_id = dataset_id
         if self.dataset_id is None:
             raise ValueError('dataset_id cannot be None')
+        self._embedding.dataset_id = dataset_id
         return self.dataset_id
 
     def get(
             self,
             dataset_id: str = None,
-    ) -> DatasetResponse:
+    ) -> DatasetModel:
         """
         this method returns a dataset name and description by dataset_id
         :param dataset_id: id of dataset
         :return: DatasetResponse model with updates
         """
         dataset_id = self.set_dataset_id(dataset_id)
         self._get(url=self.route+f'/{dataset_id}')
```

### Comparing `cval-lib-0.0.0.1/cval_lib/handlers/detection.py` & `cval-lib-0.0.1.2/cval_lib/handlers/detection.py`

 * *Files 11% similar despite different names*

```diff
@@ -17,27 +17,27 @@
 
 from requests import Session
 
 from cval_lib.configs.main_config import MainConfig
 from cval_lib.handlers._abstract_handler import AbstractHandler
 from cval_lib.handlers.result import Result
 from cval_lib.models.detection import DetectionSamplingOnPremise
+from models.result import ResultResponse
 
 
 class Detection(AbstractHandler):
     def __init__(
             self,
             session: Session,
     ):
         self.route = f'{MainConfig().main_url}'
         self.result = Result(session)
         super().__init__(session)
 
-    def on_premise_sampling(self, config: DetectionSamplingOnPremise) -> str:
+    def on_premise_sampling(self, config: DetectionSamplingOnPremise):
         """
         :param config: request model
         :return: result_id
         """
-        self.result.result_id = self.session.send(
-            self._post(self.route + 'on-premice/sampling/detection', json=config.dict()),
-        ).json().get('result_id')
-        return self.result.result_id
+        self._post(self.route + '/on-premice/sampling/detection', json=config.dict())
+        return ResultResponse.parse_obj(self.send().json())
+
```

### Comparing `cval-lib-0.0.0.1/cval_lib/handlers/embedding.py` & `cval-lib-0.0.1.2/cval_lib/handlers/embedding.py`

 * *Files 8% similar despite different names*

```diff
@@ -35,45 +35,46 @@
             type_of_dataset: str = None,
             _is_not_second=True
     ):
         if _is_not_second and dataset_id is None:
             raise ValueError('dataset_id must be not None')
         if _is_not_second and type_of_dataset is None:
             raise ValueError('type_of_dataset must be not None')
-
+        self.dataset_id = dataset_id
+        self.type_of_dataset = type_of_dataset
         self.route = f'{MainConfig().main_url}/dataset/{dataset_id}/{type_of_dataset}/'
         super().__init__(session)
 
-    def monkey_patch_url(self, dataset_id: str, type_of_dataset: str, ) -> None:
-        self.route = f'{MainConfig().main_url}/dataset/{dataset_id}/{type_of_dataset}/'
+    def monkey_patch_url(self, type_of_dataset: str, ) -> None:
+        self.route = f'{MainConfig().main_url}/dataset/{self.dataset_id}/{type_of_dataset}/'
         return self
 
-    def get_many(self, start_limit: int = 0, stop_limit: int = 1000) -> ImageEmbeddingModel:
+    def get_many(self, start_limit: int = 0, stop_limit: int = 1000) -> List[ImageEmbeddingModel]:
         """
         :param start_limit: upper limit of items
         :param stop_limit: lower limit of items
         :return: List[ImageEmbeddingModel]
         """
-        self._get(self.route + '/embeddings', params={'start_limit': start_limit, 'stop_limit': stop_limit})
+        self._get(f'{MainConfig.main_url}/dataset/{self.dataset_id}/{self.type_of_dataset}/embeddings', params={'start_limit': start_limit, 'stop_limit': stop_limit})
         return [ImageEmbeddingModel.parse_obj(i) for i in self.send().json()]
 
-    def get_by_id(self, embedding_id: str, ) -> ImageEmbeddingModel:
+    def get_by_id(self, embedding_id: str, ) -> [ImageEmbeddingModel]:
         """
         :param embedding_id: id of embedding
         :return: ImageEmbeddingModel
         """
-        self._get(self.route + f'/embedding/{embedding_id}')
-        return [ImageEmbeddingModel.parse_obj(i) for i in self.send().json()]
+        self._get(self.route + f'embedding/{embedding_id}')
+        return ImageEmbeddingModel.parse_obj(self.send().json())
 
     def upload_many(self, embeddings: List[ImageEmbeddingModel]) -> Response:
         """
         :param embeddings: List[ImageEmbeddingModel]
         :return: Response, This method does not return anything useful to use, but performs an action
         """
-        self._post(self.route + f'/embeddings', json=[i.dict() for i in embeddings])
+        self._post(f'{MainConfig.main_url}/dataset/{self.dataset_id}/{self.type_of_dataset}/embeddings', json=[i.dict() for i in embeddings])
         return self.send()
 
     def upload_by_id(self, embedding_id: str, embedding: ImageEmbeddingModel) -> Response:
         """
         :param embedding: List[ImageEmbeddingModel]
         :param embedding_id: id of embedding
         :return: Response, This method does not return anything useful to use, but performs an action
@@ -82,33 +83,33 @@
         return self.send()
 
     def update_many(self, embeddings: List[ImageEmbeddingModel]) -> Response:
         """
         :param embeddings: List[ImageEmbeddingModel]
         :return: Response, This method does not return anything useful to use, but performs an action
         """
-        self._put(self.route + f'/embeddings', json=[i.dict() for i in embeddings])
+        self._put(self.route + f'embeddings', json=[i.dict() for i in embeddings])
         return self.send()
 
     def update_by_id(self, embedding_id: str, embedding: ImageEmbeddingModel) -> Response:
         """
         :param embedding: List[ImageEmbeddingModel]
         :param embedding_id: id of embedding
         :return: Response, This method does not return anything useful to use, but performs an action
         """
-        self._put(self.route + f'/embedding/{embedding_id}', json=embedding.dict())
+        self._put(self.route + f'embedding/{embedding_id}', json=embedding.dict())
         return self.send()
 
     def delete_all(self) -> Response:
         """
         :return: Response, This method does not return anything useful to use, but performs an action
         """
-        self._delete(self.route + f'/embeddings')
+        self._delete(self.route + f'embeddings')
         return self.send()
 
     def delete_by_id(self, embedding_id: str) -> Response:
         """
         :param embedding_id: id of embedding
         :return: Response, This method does not return anything useful to use, but performs an action
         """
-        self._delete(self.route + f'/embedding/{embedding_id}')
+        self._delete(self.route + f'embedding/{embedding_id}')
         return self.send()
```

### Comparing `cval-lib-0.0.0.1/cval_lib/handlers/result.py` & `cval-lib-0.0.1.2/cval_lib/handlers/result.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,27 +13,28 @@
 Try our demo notebook to see how CVAL can revolutionize your computer vision projects.
 
 To obtain a client_api_key, please send a request to k.suhorukov@digital-quarters.com
 """
 
 from requests import Session
 
+from configs.main_config import MainConfig
 from cval_lib.handlers._abstract_handler import AbstractHandler
 from cval_lib.models.result import ResultResponse
 
 
 class Result(AbstractHandler):
     """
     The result is the entity in which the processing data is stored
     """
     def __init__(
             self,
             session: Session,
     ):
-        self.route = f'http://127.0.0.1:9940/api/result'
+        self.route = f'{MainConfig.main_url}/result'
         self.result_id = None
         super().__init__(session)
 
     def _set_result_id(self, result_id: str = None):
         if result_id is None:
             result_id = self.result_id
         if result_id is None:
```

### Comparing `cval-lib-0.0.0.1/cval_lib/models/dataset.py` & `cval-lib-0.0.1.2/cval_lib/models/dataset.py`

 * *Files identical despite different names*

### Comparing `cval-lib-0.0.0.1/cval_lib/models/detection.py` & `cval-lib-0.0.1.2/cval_lib/models/detection.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,11 +67,11 @@
         allowed = 'margin,least,ratio,entropy,probability'.split(',')
         if value not in allowed:
             raise ValueError(f"allowed selection_strategy = {allowed}")
         return value
 
     @validator('sort_strategy')
     def validate_sort_strategy(cls, value):
-        allowed = 'max,min'.split(',')
+        allowed = 'ascending,descending'.split(',')
         if value not in allowed:
             raise ValueError(f"allowed sort_strategy = {allowed}")
         return value
```

### Comparing `cval-lib-0.0.0.1/cval_lib/models/embedding.py` & `cval-lib-0.0.1.2/cval_lib/models/embedding.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 Repeat this process until you achieve an acceptable quality of the model.
 
 Our service makes it easy to implement this workflow and improve your models quickly and efficiently.
 Try our demo notebook to see how CVAL can revolutionize your computer vision projects.
 
 To obtain a client_api_key, please send a request to k.suhorukov@digital-quarters.com
 """
+
 from typing import List
 
 from pydantic import BaseModel, Field
 
 
 class ImageEmbeddingModel(BaseModel):
     """
```

### Comparing `cval-lib-0.0.0.1/cval_lib/models/result.py` & `cval-lib-0.0.1.2/cval_lib/models/result.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 Repeat this process until you achieve an acceptable quality of the model.
 
 Our service makes it easy to implement this workflow and improve your models quickly and efficiently.
 Try our demo notebook to see how CVAL can revolutionize your computer vision projects.
 
 To obtain a client_api_key, please send a request to k.suhorukov@digital-quarters.com
 """
+from typing import Any
+
 from pydantic import BaseModel
 
 
 class WeightsConfigResponse(BaseModel):
     """
     :param weights_id: id of weights
     :param retrain_model: use model retrain
@@ -46,13 +48,14 @@
     :param time_start: starting unix timestamp
     :param time_end: ending unix timestamp
     :param type_of_task: type of task: detection, classification
     :param action: action of result: sampling or test
     :param weights: weights of result
     """
     result_id: str
-    dataset_id: str
+    dataset_id: str | None
     time_start: float
     time_end: float | None
     type_of_task: str
     action: str
     weights: WeightsConfigResponse | None
+    result: Any
```

### Comparing `cval-lib-0.0.0.1/cval_lib.egg-info/SOURCES.txt` & `cval-lib-0.0.1.2/cval_lib.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -4,15 +4,17 @@
 setup.py
 ./cval_lib/__init__.py
 ./cval_lib/connection.py
 ./cval_lib/configs/__init__.py
 ./cval_lib/configs/main_config.py
 ./cval_lib/examples/__init__.py
 ./cval_lib/examples/dataset.py
+./cval_lib/examples/embeddings.py
 ./cval_lib/examples/monkey_patch.py
+./cval_lib/examples/on_pemise.py
 ./cval_lib/examples/result.py
 ./cval_lib/handlers/__async.py
 ./cval_lib/handlers/__init__.py
 ./cval_lib/handlers/_abstract_handler.py
 ./cval_lib/handlers/dataset.py
 ./cval_lib/handlers/detection.py
 ./cval_lib/handlers/embedding.py
```

