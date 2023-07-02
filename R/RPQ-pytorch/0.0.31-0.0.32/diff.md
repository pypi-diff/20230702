# Comparing `tmp/RPQ-pytorch-0.0.31.tar.gz` & `tmp/RPQ-pytorch-0.0.32.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RPQ-pytorch-0.0.31.tar", last modified: Thu Jun 22 14:43:58 2023, max compression
+gzip compressed data, was "RPQ-pytorch-0.0.32.tar", last modified: Sun Jul  2 18:59:53 2023, max compression
```

## Comparing `RPQ-pytorch-0.0.31.tar` & `RPQ-pytorch-0.0.32.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:43:58.573581 RPQ-pytorch-0.0.31/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-22 14:43:49.000000 RPQ-pytorch-0.0.31/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7636 2023-06-22 14:43:58.573581 RPQ-pytorch-0.0.31/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6903 2023-06-22 14:43:49.000000 RPQ-pytorch-0.0.31/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:43:58.569581 RPQ-pytorch-0.0.31/RPQ_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7636 2023-06-22 14:43:58.000000 RPQ-pytorch-0.0.31/RPQ_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-22 14:43:58.000000 RPQ-pytorch-0.0.31/RPQ_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 14:43:58.000000 RPQ-pytorch-0.0.31/RPQ_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-22 14:43:58.000000 RPQ-pytorch-0.0.31/RPQ_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-22 14:43:58.000000 RPQ-pytorch-0.0.31/RPQ_pytorch.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:43:58.573581 RPQ-pytorch-0.0.31/rpq/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 14:43:49.000000 RPQ-pytorch-0.0.31/rpq/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:43:58.573581 RPQ-pytorch-0.0.31/rpq/models/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-22 14:43:49.000000 RPQ-pytorch-0.0.31/rpq/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    57623 2023-06-22 14:43:49.000000 RPQ-pytorch-0.0.31/rpq/models/rpqopt.py
--rw-r--r--   0 runner    (1001) docker     (123)    59815 2023-06-22 14:43:49.000000 RPQ-pytorch-0.0.31/rpq/models/rpqopt_sc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4548 2023-06-22 14:43:49.000000 RPQ-pytorch-0.0.31/rpq/models/rpqvit.py
--rw-r--r--   0 runner    (1001) docker     (123)     6131 2023-06-22 14:43:49.000000 RPQ-pytorch-0.0.31/rpq/models/rpqvit_sc.py
--rw-r--r--   0 runner    (1001) docker     (123)     9004 2023-06-22 14:43:49.000000 RPQ-pytorch-0.0.31/rpq/nn.py
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-06-22 14:43:49.000000 RPQ-pytorch-0.0.31/rpq/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 14:43:58.573581 RPQ-pytorch-0.0.31/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-22 14:43:49.000000 RPQ-pytorch-0.0.31/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 18:59:53.771232 RPQ-pytorch-0.0.32/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-02 18:59:44.000000 RPQ-pytorch-0.0.32/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7636 2023-07-02 18:59:53.771232 RPQ-pytorch-0.0.32/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6903 2023-07-02 18:59:44.000000 RPQ-pytorch-0.0.32/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 18:59:53.767232 RPQ-pytorch-0.0.32/RPQ_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7636 2023-07-02 18:59:53.000000 RPQ-pytorch-0.0.32/RPQ_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-07-02 18:59:53.000000 RPQ-pytorch-0.0.32/RPQ_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 18:59:53.000000 RPQ-pytorch-0.0.32/RPQ_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-02 18:59:53.000000 RPQ-pytorch-0.0.32/RPQ_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-02 18:59:53.000000 RPQ-pytorch-0.0.32/RPQ_pytorch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 18:59:53.767232 RPQ-pytorch-0.0.32/rpq/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 18:59:44.000000 RPQ-pytorch-0.0.32/rpq/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 18:59:53.771232 RPQ-pytorch-0.0.32/rpq/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-02 18:59:44.000000 RPQ-pytorch-0.0.32/rpq/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57623 2023-07-02 18:59:44.000000 RPQ-pytorch-0.0.32/rpq/models/rpqopt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59815 2023-07-02 18:59:44.000000 RPQ-pytorch-0.0.32/rpq/models/rpqopt_sc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4548 2023-07-02 18:59:44.000000 RPQ-pytorch-0.0.32/rpq/models/rpqvit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6131 2023-07-02 18:59:44.000000 RPQ-pytorch-0.0.32/rpq/models/rpqvit_sc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8678 2023-07-02 18:59:44.000000 RPQ-pytorch-0.0.32/rpq/nn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-07-02 18:59:44.000000 RPQ-pytorch-0.0.32/rpq/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 18:59:53.771232 RPQ-pytorch-0.0.32/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-02 18:59:44.000000 RPQ-pytorch-0.0.32/setup.py
```

### Comparing `RPQ-pytorch-0.0.31/LICENSE` & `RPQ-pytorch-0.0.32/LICENSE`

 * *Files identical despite different names*

### Comparing `RPQ-pytorch-0.0.31/PKG-INFO` & `RPQ-pytorch-0.0.32/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RPQ-pytorch
-Version: 0.0.31
+Version: 0.0.32
 Summary: Reverse Product Quantization (RPQ) of weights to reduce static memory usage.
 Home-page: https://github.com/a-kore/RPQ-pytorch
 Author: Ali Kore
 Author-email: akore654@gmail.com
 License: MIT
 Keywords: artificial intelligence,AI,machine learning,deep learning,pytorch,quantization,product quantization,reverse product quantization,memory reduction
 Classifier: Development Status :: 4 - Beta
```

### Comparing `RPQ-pytorch-0.0.31/README.md` & `RPQ-pytorch-0.0.32/README.md`

 * *Files identical despite different names*

### Comparing `RPQ-pytorch-0.0.31/RPQ_pytorch.egg-info/PKG-INFO` & `RPQ-pytorch-0.0.32/RPQ_pytorch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RPQ-pytorch
-Version: 0.0.31
+Version: 0.0.32
 Summary: Reverse Product Quantization (RPQ) of weights to reduce static memory usage.
 Home-page: https://github.com/a-kore/RPQ-pytorch
 Author: Ali Kore
 Author-email: akore654@gmail.com
 License: MIT
 Keywords: artificial intelligence,AI,machine learning,deep learning,pytorch,quantization,product quantization,reverse product quantization,memory reduction
 Classifier: Development Status :: 4 - Beta
```

### Comparing `RPQ-pytorch-0.0.31/rpq/models/rpqopt.py` & `RPQ-pytorch-0.0.32/rpq/models/rpqopt.py`

 * *Files identical despite different names*

### Comparing `RPQ-pytorch-0.0.31/rpq/models/rpqopt_sc.py` & `RPQ-pytorch-0.0.32/rpq/models/rpqopt_sc.py`

 * *Files identical despite different names*

### Comparing `RPQ-pytorch-0.0.31/rpq/models/rpqvit.py` & `RPQ-pytorch-0.0.32/rpq/models/rpqvit.py`

 * *Files identical despite different names*

### Comparing `RPQ-pytorch-0.0.31/rpq/models/rpqvit_sc.py` & `RPQ-pytorch-0.0.32/rpq/models/rpqvit_sc.py`

 * *Files identical despite different names*

### Comparing `RPQ-pytorch-0.0.31/rpq/nn.py` & `RPQ-pytorch-0.0.32/rpq/nn.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     max_norm: Optional[float]
     norm_type: float
     scale_grad_by_freq: bool
     weight: Tensor
     sparse: bool
     num_codebooks: int
     
-    def __init__(self, num_embeddings: int, embedding_dim: int, num_codebooks: int, 
+    def __init__(self, num_embeddings: int, embedding_dim: int, num_codebooks: int, use_subset=True,
                  padding_idx: Optional[int] = None, max_norm: Optional[float] = None, norm_type: float = 2., 
                  scale_grad_by_freq: bool = False, sparse: bool = False, 
                  device=None, dtype=None) -> None:
         factory_kwargs = {'device': device, 'dtype': dtype}
         super().__init__()
         self.num_embeddings = num_embeddings
         self.embedding_dim = embedding_dim
@@ -44,42 +44,35 @@
                 padding_idx = self.num_embeddings + padding_idx
         self.padding_idx = padding_idx
         
         self.num_codebooks = num_codebooks
         assert self.embedding_dim % num_codebooks == 0, 'embedding_dim should be divisible by num_codebooks'
         self.codebook_dim = self.embedding_dim//self.num_codebooks
         
+        self.use_subset = use_subset
         self.max_norm = max_norm
         self.norm_type = norm_type
         self.scale_grad_by_freq = scale_grad_by_freq
         self.sparse = sparse
-        
-        self.register_buffer("codes",
-                             torch.randint(high=256, size=(self.num_codebooks, self.num_embeddings), 
-                                           dtype=torch.uint8, device=factory_kwargs['device']))
-        self.codebooks = Parameter(torch.empty(self.num_codebooks, 256, 
-                                               self.codebook_dim, **factory_kwargs))            
+
+        self.rpqweight = RPQWeight(self.num_codebooks, self.codebook_dim, self.num_embeddings,
+                                   device=factory_kwargs['device'], dtype=factory_kwargs['dtype'])
+                                         
         self.reset_parameters()
 
     def reset_parameters(self) -> None:
-        init.normal_(self.codebooks)
-
-    def expand(self, codes, codebooks):
-        dim = codebooks.shape[-1]
-        codes_expand = repeat(codes, 'h c -> h c d', d = dim)
-        return codebooks.gather(dim=1, index=codes_expand.long())
-        
-    def get_weight(self) -> Tensor:
-        return rearrange(self.expand(self.codes, self.codebooks), 
-                         'h c d -> c (h d )')
+        init.normal_(self.rpqweight.codebooks)
 
     def forward(self, input: Tensor) -> Tensor:
-        return F.embedding(
-            input, self.get_weight(), self.padding_idx, self.max_norm, 
-            self.norm_type, self.scale_grad_by_freq, sparse=self.sparse)
+        if self.use_subset:
+            return self.rpqweight(subset=input.flatten()).view(*input.shape, self.embedding_dim)
+        else:
+            return F.embedding(
+                input, self.rpqweight(), self.padding_idx, self.max_norm, 
+                self.norm_type, self.scale_grad_by_freq, sparse=self.sparse)
 
     def extra_repr(self) -> str:
         s = '{num_embeddings}, {embedding_dim}'
         if self.padding_idx is not None:
             s += ', padding_idx={padding_idx}'
         if self.max_norm is not None:
             s += ', max_norm={max_norm}'
```

### Comparing `RPQ-pytorch-0.0.31/rpq/utils.py` & `RPQ-pytorch-0.0.32/rpq/utils.py`

 * *Files identical despite different names*

### Comparing `RPQ-pytorch-0.0.31/setup.py` & `RPQ-pytorch-0.0.32/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'RPQ-pytorch',
   packages = find_packages(exclude=[]),
-  version = '0.0.31',
+  version = '0.0.32',
   license='MIT',
   description = 'Reverse Product Quantization (RPQ) of weights to reduce static memory usage.',
   author = 'Ali Kore',
   author_email = 'akore654@gmail.com',
   long_description=open('README.md', 'r').read(),
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/a-kore/RPQ-pytorch',
```

