# Comparing `tmp/similarity_check-0.1.8.tar.gz` & `tmp/similarity_check-0.1.9.tar.gz`

## Comparing `similarity_check-0.1.8.tar` & `similarity_check-0.1.9.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 similarity_check-0.1.8/setup.cfg
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 similarity_check-0.1.8/setup.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 similarity_check-0.1.8/src/similarity_check/__init__.py
--rw-r--r--   0        0        0    23585 2020-02-02 00:00:00.000000 similarity_check-0.1.8/src/similarity_check/checkers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 similarity_check-0.1.8/LICENSE
--rw-r--r--   0        0        0     8552 2020-02-02 00:00:00.000000 similarity_check-0.1.8/README.md
--rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 similarity_check-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     8881 2020-02-02 00:00:00.000000 similarity_check-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 similarity_check-0.1.9/setup.cfg
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 similarity_check-0.1.9/setup.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 similarity_check-0.1.9/src/similarity_check/__init__.py
+-rw-r--r--   0        0        0    23554 2020-02-02 00:00:00.000000 similarity_check-0.1.9/src/similarity_check/checkers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 similarity_check-0.1.9/LICENSE
+-rw-r--r--   0        0        0     8657 2020-02-02 00:00:00.000000 similarity_check-0.1.9/README.md
+-rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 similarity_check-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     8984 2020-02-02 00:00:00.000000 similarity_check-0.1.9/PKG-INFO
```

### Comparing `similarity_check-0.1.8/setup.cfg` & `similarity_check-0.1.9/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2073 696d 696c 6172 6974 795f 6368   = similarity_ch
 00000020: 6563 6b0d 0a64 6573 6372 6970 7469 6f6e  eck..description
 00000030: 203d 2070 6163 6b61 6765 2066 6f72 206d   = package for m
 00000040: 6561 7375 7269 6e67 2074 6865 2073 696d  easuring the sim
 00000050: 696c 6172 6974 7920 6f66 2074 776f 2074  ilarity of two t
 00000060: 6578 7473 0d0a 7665 7273 696f 6e20 3d20  exts..version = 
-00000070: 302e 312e 380d 0a6c 6f6e 675f 6465 7363  0.1.8..long_desc
+00000070: 302e 312e 390d 0a6c 6f6e 675f 6465 7363  0.1.9..long_desc
 00000080: 7269 7074 696f 6e20 3d20 6669 6c65 3a20  ription = file: 
 00000090: 5245 4144 4d45 2e6d 640d 0a6c 6f6e 675f  README.md..long_
 000000a0: 6465 7363 7269 7074 696f 6e5f 636f 6e74  description_cont
 000000b0: 656e 745f 7479 7065 203d 2074 6578 742f  ent_type = text/
 000000c0: 6d61 726b 646f 776e 0d0a 6175 7468 6f72  markdown..author
 000000d0: 203d 206d 6573 6861 7269 0d0a 6175 7468   = meshari..auth
 000000e0: 6f72 5f65 6d61 696c 203d 206d 6573 6861  or_email = mesha
```

### Comparing `similarity_check-0.1.8/src/similarity_check/checkers.py` & `similarity_check-0.1.9/src/similarity_check/checkers.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from string import punctuation
 from nltk.stem import PorterStemmer
 from nltk.stem.isri import ISRIStemmer
 from tqdm import tqdm
 from collections import Counter
 download('stopwords')
 
+
 def preprocess(sentence: str, remove_punct: bool, remove_stop_words: bool, stemm: bool, lang: str='en') -> str: 
     if lang.lower() == 'en':
         ps = PorterStemmer()
         # remove punctuations
         if not remove_punct:
             sentence = sentence.translate(str.maketrans('', '', punctuation))
         # remove stop words and stem
@@ -88,46 +89,47 @@
     
 class sentence_tranformer_checker():
     def __init__(
         self, 
         targets: Union[List[str], pd.DataFrame], 
         target_group: Union[List[str], pd.DataFrame]=None,
         target_col: str=None, 
+        device: str = None,
         model: SentenceTransformer=None, 
         lang: str='en', 
         only_include: List[str]=None,
         encode_batch = 32,
         encode_target = True,
         remove_punct: bool=True, 
         remove_stop_words: bool=True, 
         stemm: bool=False
     ):    
         """
         parameters:
-            source: dataframe or list of input texts to find closest match for.
-            target: dataframe or list of targets text to compare with.
-            model (optional): a sentence tranformer model object, to use instead of the default one, for more [details](https://www.sbert.net/).
+            targets: dataframe or list of targets text to compare with.
             target_group (optional): goups ids for the target to match only a single target for each group, can either provide list of ids,
             or the column name in the target dataframe.
-            source_col (partially optional): the source column name used to match, *must be specified for dataframe matching*.
             target_col (partially optional): the target column name used to match, *must be specified for dataframe matching*.
+            device: the device to do the encoding on operations in (cpu|cuda),
+            model (optional): a sentence tranformer model object, to use instead of the default one, for more [details](https://www.sbert.net/).
+            lang (optional): the languge of the model ('en'|'ar').
             only_include (optional): used only for dataframe matching, allow providing a list of column names to only include for the target matches, provide empty list to get only target_col.
             encode_batch (optional): the number of sentences to encode in a batch.
             encode_target: boolean flag to indicate whatever to enocde the targets when initilizing the object (to cache target encoding).
-            lang (optional): the languge of the model ('en'|'ar').
             remove_punct: boolean flag to indicate whatever to remove punctuations. 
             remove_stop_words: boolean flag to indicate whatever to remove stop words.
             stemm: boolean flag to indicate whatever to do stemming.
         """
 
         self.encode_batch = encode_batch
         self.remove_punct = remove_punct
         self.remove_stop_words = remove_stop_words
         self.stemm = stemm
         self.lang = lang 
+        self.device = device.lower()
 
         if isinstance(targets, pd.DataFrame):
             self.use_frames = True
     
             if target_col not in targets.columns:
                 raise KeyError('target_col not found in target DataFrame cloumns')
 
@@ -166,24 +168,25 @@
             self.use_frames = False
             self.target_names = [preprocess(sent, self.remove_punct, self.remove_stop_words, self.stemm, self.lang) for sent in targets]
 
         if pd.isnull(self.target_names).any():
             raise ValueError('Targets contain null values')
 
         self.model = model
+        self.model.device = device
         # if no model is provided use the default model
         if model is None:
             print('initializing the model...')
             if lang.lower() == 'en':
-                self.model = SentenceTransformer('all-MiniLM-L6-v2', device='cuda')
+                self.model = SentenceTransformer('all-MiniLM-L6-v2', device=device)
                 print('done...')
             else:
-                self.model = SentenceTransformer('distiluse-base-multilingual-cased-v1', device='cuda')
+                self.model = SentenceTransformer('distiluse-base-multilingual-cased-v1', device=device)
                 print('done...')
-        
+
         if encode_target:  
             print('enocding targets: ')
             self.encoded_targets = self.model.encode(self.target_names, batch_size=self.encode_batch, show_progress_bar=True,  normalize_embeddings=True) # encode the targets
 
 
     # used to make sure that if the object targets are updated, the cached targets are deleted
     def __setattr__(self, key, value):
```

### Comparing `similarity_check-0.1.8/README.md` & `similarity_check-0.1.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -10,36 +10,38 @@
 pip install similarity_check 
 ```
 
 ## Usage
 ### sentence tranformer
 #### documentation
 * sentence_tranformer(
-        targets: Union[list[str], pd.DataFrame], 
-        target_group: Union[list[str], pd.DataFrame]=None,
+        targets: Union[List[str], pd.DataFrame], 
+        target_group: Union[List[str], pd.DataFrame]=None,
         target_col: str=None, 
+        device: str = None,
         model: SentenceTransformer=None, 
         lang: str='en', 
-        only_include: list[str]=None,
+        only_include: List[str]=None,
         encode_batch = 32,
-        encode_target = False,
+        encode_target = True,
         remove_punct: bool=True, 
         remove_stop_words: bool=True, 
         stemm: bool=False
   ):
   * parameters:
-    * target: dataframe or list of targets text to compare with.
-    * model (optional): a sentence tranformer model object, to use instead of the default one, for more [details](https://www.sbert.net/).
+    * targets: dataframe or list of targets text to compare with.
     * target_group (optional): goups ids for the target to match only a single target for each group, can either provide list of ids,
-    or the column name in the target dataframe.
+    * or the column name in the target dataframe.
     * target_col (partially optional): the target column name used to match, *must be specified for dataframe matching*.
+    * device: the device to do the encoding on operations in (cpu|cuda),
+    * model (optional): a sentence tranformer model object, to use instead of the default one, for more [details](https://www.sbert.net/).
+    * lang (optional): the languge of the model ('en'|'ar').
     * only_include (optional): used only for dataframe matching, allow providing a list of column names to only include for the target matches, provide empty list to get only target_col.
     * encode_batch (optional): the number of sentences to encode in a batch.
     * encode_target: boolean flag to indicate whatever to enocde the targets when initilizing the object (to cache target encoding).
-    * lang (optional): the languge of the model ('en'|'ar').
     * remove_punct: boolean flag to indicate whatever to remove punctuations. 
     * remove_stop_words: boolean flag to indicate whatever to remove stop words.
     * stemm: boolean flag to indicate whatever to do stemming.
 * sentence_tranformer.match(
         source: Union[list[str], pd.DataFrame], 
         source_col: str=None, 
         topn: int=1,
```

### Comparing `similarity_check-0.1.8/pyproject.toml` & `similarity_check-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "similarity_check"
-version = "0.1.8"
+version = "0.1.9"
 authors = [
   { name="meshari", email="meshari34343@gmail.com" },
 ]
 description = "package for measuring the similarity of two texts"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
```

### Comparing `similarity_check-0.1.8/PKG-INFO` & `similarity_check-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: similarity_check
-Version: 0.1.8
+Version: 0.1.9
 Summary: package for measuring the similarity of two texts
 Author-email: meshari <meshari34343@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
@@ -26,36 +26,38 @@
 pip install similarity_check 
 ```
 
 ## Usage
 ### sentence tranformer
 #### documentation
 * sentence_tranformer(
-        targets: Union[list[str], pd.DataFrame], 
-        target_group: Union[list[str], pd.DataFrame]=None,
+        targets: Union[List[str], pd.DataFrame], 
+        target_group: Union[List[str], pd.DataFrame]=None,
         target_col: str=None, 
+        device: str = None,
         model: SentenceTransformer=None, 
         lang: str='en', 
-        only_include: list[str]=None,
+        only_include: List[str]=None,
         encode_batch = 32,
-        encode_target = False,
+        encode_target = True,
         remove_punct: bool=True, 
         remove_stop_words: bool=True, 
         stemm: bool=False
   ):
   * parameters:
-    * target: dataframe or list of targets text to compare with.
-    * model (optional): a sentence tranformer model object, to use instead of the default one, for more [details](https://www.sbert.net/).
+    * targets: dataframe or list of targets text to compare with.
     * target_group (optional): goups ids for the target to match only a single target for each group, can either provide list of ids,
-    or the column name in the target dataframe.
+    * or the column name in the target dataframe.
     * target_col (partially optional): the target column name used to match, *must be specified for dataframe matching*.
+    * device: the device to do the encoding on operations in (cpu|cuda),
+    * model (optional): a sentence tranformer model object, to use instead of the default one, for more [details](https://www.sbert.net/).
+    * lang (optional): the languge of the model ('en'|'ar').
     * only_include (optional): used only for dataframe matching, allow providing a list of column names to only include for the target matches, provide empty list to get only target_col.
     * encode_batch (optional): the number of sentences to encode in a batch.
     * encode_target: boolean flag to indicate whatever to enocde the targets when initilizing the object (to cache target encoding).
-    * lang (optional): the languge of the model ('en'|'ar').
     * remove_punct: boolean flag to indicate whatever to remove punctuations. 
     * remove_stop_words: boolean flag to indicate whatever to remove stop words.
     * stemm: boolean flag to indicate whatever to do stemming.
 * sentence_tranformer.match(
         source: Union[list[str], pd.DataFrame], 
         source_col: str=None, 
         topn: int=1,
```

