# Comparing `tmp/fast-pagerank-0.0.4.tar.gz` & `tmp/fast-pagerank-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fast-pagerank-0.0.4.tar", last modified: Thu Jun 27 01:54:57 2019, max compression
+gzip compressed data, was "fast-pagerank-1.0.0.tar", last modified: Sun Jul  2 01:25:07 2023, max compression
```

## Comparing `fast-pagerank-0.0.4.tar` & `fast-pagerank-1.0.0.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxr-xr-x   0 arminsajadi   (502) staff       (20)        0 2019-06-27 01:54:57.000000 fast-pagerank-0.0.4/
--rw-r--r--   0 arminsajadi   (502) staff       (20)     4573 2019-06-27 01:54:57.000000 fast-pagerank-0.0.4/PKG-INFO
--rw-r--r--   0 arminsajadi   (502) staff       (20)     3670 2019-06-27 01:52:17.000000 fast-pagerank-0.0.4/README.md
-drwxr-xr-x   0 arminsajadi   (502) staff       (20)        0 2019-06-27 01:54:57.000000 fast-pagerank-0.0.4/fast_pagerank/
--rw-r--r--   0 arminsajadi   (502) staff       (20)      169 2019-06-02 05:21:24.000000 fast-pagerank-0.0.4/fast_pagerank/__init__.py
--rw-r--r--   0 arminsajadi   (502) staff       (20)     3049 2019-06-02 04:03:22.000000 fast-pagerank-0.0.4/fast_pagerank/fast_pagerank.py
-drwxr-xr-x   0 arminsajadi   (502) staff       (20)        0 2019-06-27 01:54:57.000000 fast-pagerank-0.0.4/fast_pagerank.egg-info/
--rw-r--r--   0 arminsajadi   (502) staff       (20)     4573 2019-06-27 01:54:56.000000 fast-pagerank-0.0.4/fast_pagerank.egg-info/PKG-INFO
--rw-r--r--   0 arminsajadi   (502) staff       (20)      223 2019-06-27 01:54:56.000000 fast-pagerank-0.0.4/fast_pagerank.egg-info/SOURCES.txt
--rw-r--r--   0 arminsajadi   (502) staff       (20)        1 2019-06-27 01:54:56.000000 fast-pagerank-0.0.4/fast_pagerank.egg-info/dependency_links.txt
--rw-r--r--   0 arminsajadi   (502) staff       (20)       14 2019-06-27 01:54:56.000000 fast-pagerank-0.0.4/fast_pagerank.egg-info/top_level.txt
--rw-r--r--   0 arminsajadi   (502) staff       (20)       38 2019-06-27 01:54:57.000000 fast-pagerank-0.0.4/setup.cfg
--rw-r--r--   0 arminsajadi   (502) staff       (20)      647 2019-06-27 01:54:47.000000 fast-pagerank-0.0.4/setup.py
+drwxrwxr-x   0 armin     (1000) armin     (1000)        0 2023-07-02 01:25:07.647865 fast-pagerank-1.0.0/
+-rw-rw-r--   0 armin     (1000) armin     (1000)     1068 2023-07-01 23:24:00.000000 fast-pagerank-1.0.0/LICENSE
+-rw-rw-r--   0 armin     (1000) armin     (1000)     4198 2023-07-02 01:25:07.643865 fast-pagerank-1.0.0/PKG-INFO
+-rw-rw-r--   0 armin     (1000) armin     (1000)     3761 2023-07-01 23:24:00.000000 fast-pagerank-1.0.0/README.md
+drwxrwxr-x   0 armin     (1000) armin     (1000)        0 2023-07-02 01:25:07.643865 fast-pagerank-1.0.0/fast_pagerank/
+-rw-rw-r--   0 armin     (1000) armin     (1000)      169 2023-07-01 23:24:00.000000 fast-pagerank-1.0.0/fast_pagerank/__init__.py
+-rw-rw-r--   0 armin     (1000) armin     (1000)     3072 2023-07-02 00:41:13.000000 fast-pagerank-1.0.0/fast_pagerank/fast_pagerank.py
+drwxrwxr-x   0 armin     (1000) armin     (1000)        0 2023-07-02 01:25:07.643865 fast-pagerank-1.0.0/fast_pagerank.egg-info/
+-rw-rw-r--   0 armin     (1000) armin     (1000)     4198 2023-07-02 01:25:07.000000 fast-pagerank-1.0.0/fast_pagerank.egg-info/PKG-INFO
+-rw-rw-r--   0 armin     (1000) armin     (1000)      231 2023-07-02 01:25:07.000000 fast-pagerank-1.0.0/fast_pagerank.egg-info/SOURCES.txt
+-rw-rw-r--   0 armin     (1000) armin     (1000)        1 2023-07-02 01:25:07.000000 fast-pagerank-1.0.0/fast_pagerank.egg-info/dependency_links.txt
+-rw-rw-r--   0 armin     (1000) armin     (1000)       14 2023-07-02 01:25:07.000000 fast-pagerank-1.0.0/fast_pagerank.egg-info/top_level.txt
+-rw-rw-r--   0 armin     (1000) armin     (1000)       38 2023-07-02 01:25:07.647865 fast-pagerank-1.0.0/setup.cfg
+-rw-rw-r--   0 armin     (1000) armin     (1000)      647 2023-07-02 01:22:59.000000 fast-pagerank-1.0.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `fast-pagerank-0.0.4/PKG-INFO` & `fast-pagerank-1.0.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,69 +1,71 @@
 Metadata-Version: 2.1
 Name: fast-pagerank
-Version: 0.0.4
+Version: 1.0.0
 Summary: A fast PageRank and Personalized PageRank implementation
 Home-page: https://github.com/asajadi/fast_pagerank
 Author: Armin Sajadi
 Author-email: asajadi@gmail.com
-License: UNKNOWN
-Description: # Fast Personalized PageRank Implementation
-        
-        I needed a fast PageRank for [Wikisim](https://github.com/asajadi/wikisim) project. It had to be fast enough to run real time on relatively large graphs. NetworkX was the obvious library to use, however, it needed back and forth translation from my graph representation (which was the pretty standard csr matrix), to its internal graph data structure. These translations were slowing down the process. 
-        
-        I implemented two versions of the algorithm in Python, both inspired by the sparse fast solutions given in [**Cleve Moler**](https://en.wikipedia.org/wiki/Cleve_Moler)'s book, [*Experiments with MATLAB*](https://www.mathworks.com/content/dam/mathworks/mathworks-dot-com/moler/exm/chapters/pagerank.pdf). The power method is much faster with enough precision for our task. 
-        
-        ### Personalized PageRank
-        I modified the algorithm a little bit to be able to calculate **personalized PageRank** as well. 
-        
-        
-        ### Comparison with Popular Python Implementations: NetworkX and iGraph
-        Both implementations (exact solution and *power method*) are much faster than their correspondent methods in NetworkX. The *power method* is also faster than the iGraph native implementation, which is also an eigen-vector based solution. Benchmarking is done on a `ml.t3.2xlarge` SageMaker instance. 
-        
-        ### What is the major drawback of NetworkX PageRank?
-        I gave up using NetworkX for one simple reason: I had to calculate PageRank several times, and my internal representation of a graph was a simple sparse matrix. Every time I wanted to calculate PageRank I had to translate it to the graph representation of NetworkX, which was slow. My benchmarking shows that NetworkX  has a pretty fast implementation of PageRank ( `networkx.pagerank_numpy` and  '`networkx.pagerank_scipy`), but translating from its own graph data structure to a csr matrix before doing the actual calculations is exactly what exactly slows down the whole algorithm. 
-        
-        **Note**: I didn't count the time spent on `nx.from_scipy_sparse_matrix` (converting a csr matrix before passing it to NetworkX PageRank) in my benchmarking, But I could! Because that was another bottleneck for me, and for many other cases that one has a `csr` adjacency matrix.
-        
-        ### Python Implementation
-        The python package is hosted at https://github.com/asajadi/fast-pagerank and you can find the installation guide in the [README.md](https://github.com/asajadi/fast-pagerank/blob/master/README.md) file. You also can find a detailed analysis in [the jupyter notebook](https://github.com/asajadi/fast-pagerank/blob/master/notebooks/Fast-PageRank.ipynb) or [this blog post](https://asajadi.github.io/fast-pagerank/). 
-        
-        
-        ## Usage
-        ### Installation:
-        `pip install fast-pagerank`
-        
-        ### Example
-        Let's take Example 1 from https://www.cs.princeton.edu/~chazelle/courses/BIB/pagerank.htm 
-        
-        ![](example1.gif)
-        
-        Assuming A=0, B=1, C=2, D=3:
-        
-        ```
-        >>> import numpy as np
-        >>> from scipy import sparse
-        >>> from fast_pagerank import pagerank
-        >>> from fast_pagerank import pagerank_power
-        >>> A = np.array([[0,1], [0, 2], [1, 2],[2,0],[3,2]])
-        >>> weights = [1,1,1,1,1]
-        >>> G = sparse.csr_matrix((weights, (A[:,0], A[:,1])), shape=(4, 4))
-        >>> pr=pagerank(G, p=0.85)
-        >>> pr
-        array([0.37252685, 0.19582391, 0.39414924, 0.0375    ])
-        ```
-        
-        The output elements are essentially the same numbers written on the nodes, but normalized (multiply the vector by 4 and you will get the same numbers) 
-        
-        We can add personalization, or use *power method*:
-        
-        ```
-        >>> personalize = np.array([0.4, 0.2, 0.2, 0.4])
-        >>> pr=pagerank_power(G, p=0.85, personalize=personalize, tol=1e-6)
-        >>> pr
-        array([0.37817981, 0.18572635, 0.38609383, 0.05      ])
-        ```
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+[![996.icu](https://img.shields.io/badge/link-996.icu-red.svg)](https://996.icu/#/en_US)
+
+# Fast Personalized PageRank Implementation
+
+I needed a fast PageRank for [Wikisim](https://github.com/asajadi/wikisim) project. It had to be fast enough to run real time on relatively large graphs. NetworkX was the obvious library to use, however, it needed back and forth translation from my graph representation (which was the pretty standard csr matrix), to its internal graph data structure. These translations were slowing down the process. 
+
+I implemented two versions of the algorithm in Python, both inspired by the sparse fast solutions given in [**Cleve Moler**](https://en.wikipedia.org/wiki/Cleve_Moler)'s book, [*Experiments with MATLAB*](https://www.mathworks.com/content/dam/mathworks/mathworks-dot-com/moler/exm/chapters/pagerank.pdf). The power method is much faster with enough precision for our task. 
+
+### Personalized PageRank
+I modified the algorithm a little bit to be able to calculate **personalized PageRank** as well. 
+
+
+### Comparison with Popular Python Implementations: NetworkX and iGraph
+Both implementations (exact solution and *power method*) are much faster than their correspondent methods in NetworkX. The *power method* is also faster than the iGraph native implementation, which is also an eigen-vector based solution. Benchmarking is done on a `ml.t3.2xlarge` SageMaker instance. 
+
+### What is the major drawback of NetworkX PageRank?
+I gave up using NetworkX for one simple reason: I had to calculate PageRank several times, and my internal representation of a graph was a simple sparse matrix. Every time I wanted to calculate PageRank I had to translate it to the graph representation of NetworkX, which was slow. My benchmarking shows that NetworkX  has a pretty fast implementation of PageRank ( `networkx.pagerank_numpy` and  '`networkx.pagerank_scipy`), but translating from its own graph data structure to a csr matrix before doing the actual calculations is exactly what exactly slows down the whole algorithm. 
+
+**Note**: I didn't count the time spent on `nx.from_scipy_sparse_matrix` (converting a csr matrix before passing it to NetworkX PageRank) in my benchmarking, But I could! Because that was another bottleneck for me, and for many other cases that one has a `csr` adjacency matrix.
+
+### Python Implementation
+The python package is hosted at https://github.com/asajadi/fast-pagerank and you can find the installation guide in the [README.md](https://github.com/asajadi/fast-pagerank/blob/master/README.md) file. You also can find a detailed analysis in [the jupyter notebook](https://github.com/asajadi/fast-pagerank/blob/master/notebooks/Fast-PageRank.ipynb) or [this blog post](https://asajadi.github.io/fast-pagerank/). 
+
+
+## Usage
+### Installation:
+`pip install fast-pagerank`
+
+### Example
+Let's take Example 1 from https://www.cs.princeton.edu/~chazelle/courses/BIB/pagerank.htm 
+
+![](example1.gif)
+
+Assuming A=0, B=1, C=2, D=3:
+
+```
+>>> import numpy as np
+>>> from scipy import sparse
+>>> from fast_pagerank import pagerank
+>>> from fast_pagerank import pagerank_power
+>>> A = np.array([[0,1], [0, 2], [1, 2],[2,0],[3,2]])
+>>> weights = [1,1,1,1,1]
+>>> G = sparse.csr_matrix((weights, (A[:,0], A[:,1])), shape=(4, 4))
+>>> pr=pagerank(G, p=0.85)
+>>> pr
+array([0.37252685, 0.19582391, 0.39414924, 0.0375    ])
+```
+
+The output elements are essentially the same numbers written on the nodes, but normalized (multiply the vector by 4 and you will get the same numbers) 
+
+We can add personalization, or use *power method*:
+
+```
+>>> personalize = np.array([0.4, 0.2, 0.2, 0.4])
+>>> pr=pagerank_power(G, p=0.85, personalize=personalize, tol=1e-6)
+>>> pr
+array([0.37817981, 0.18572635, 0.38609383, 0.05      ])
+```
```

### Comparing `fast-pagerank-0.0.4/README.md` & `fast-pagerank-1.0.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+[![996.icu](https://img.shields.io/badge/link-996.icu-red.svg)](https://996.icu/#/en_US)
+
 # Fast Personalized PageRank Implementation
 
 I needed a fast PageRank for [Wikisim](https://github.com/asajadi/wikisim) project. It had to be fast enough to run real time on relatively large graphs. NetworkX was the obvious library to use, however, it needed back and forth translation from my graph representation (which was the pretty standard csr matrix), to its internal graph data structure. These translations were slowing down the process. 
 
 I implemented two versions of the algorithm in Python, both inspired by the sparse fast solutions given in [**Cleve Moler**](https://en.wikipedia.org/wiki/Cleve_Moler)'s book, [*Experiments with MATLAB*](https://www.mathworks.com/content/dam/mathworks/mathworks-dot-com/moler/exm/chapters/pagerank.pdf). The power method is much faster with enough precision for our task. 
 
 ### Personalized PageRank
@@ -49,8 +51,8 @@
 We can add personalization, or use *power method*:
 
 ```
 >>> personalize = np.array([0.4, 0.2, 0.2, 0.4])
 >>> pr=pagerank_power(G, p=0.85, personalize=personalize, tol=1e-6)
 >>> pr
 array([0.37817981, 0.18572635, 0.38609383, 0.05      ])
-```
+```
```

### Comparing `fast-pagerank-0.0.4/fast_pagerank/fast_pagerank.py` & `fast-pagerank-1.0.0/fast_pagerank/fast_pagerank.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     [Reference]:
     Cleve Moler. 2011. Experiments with MATLAB (Electronic ed.).
     MathWorks, Inc.
 """
 # uncomment
 from __future__ import division
 
+import numpy as np
 import scipy as sp
 import scipy.sparse as sprs
 import scipy.spatial
 import scipy.sparse.linalg
 
 __author__ = "Armin Sajadi"
 __copyright__ = "Copyright 2015, The Wikisim Project"
@@ -42,22 +43,22 @@
     """
     # In Moler's algorithm, $A_{ij}$ represents the existences of an edge
     # from node $j$ to $i$, while we have assumed the opposite!
     if reverse:
         A = A.T
 
     n, _ = A.shape
-    r = sp.asarray(A.sum(axis=1)).reshape(-1)
+    r = np.asarray(A.sum(axis=1)).reshape(-1)
 
     k = r.nonzero()[0]
 
     D_1 = sprs.csr_matrix((1 / r[k], (k, k)), shape=(n, n))
 
     if personalize is None:
-        personalize = sp.ones(n)
+        personalize = np.ones(n)
     personalize = personalize.reshape(n, 1)
     s = (personalize / personalize.sum()) * n
 
     I = sprs.eye(n)
     x = sprs.linalg.spsolve((I - p * A.T @ D_1), s)
 
     x = x / x.sum()
@@ -85,34 +86,34 @@
     """
     # In Moler's algorithm, $G_{ij}$ represents the existences of an edge
     # from node $j$ to $i$, while we have assumed the opposite!
     if reverse:
         A = A.T
 
     n, _ = A.shape
-    r = sp.asarray(A.sum(axis=1)).reshape(-1)
+    r = np.asarray(A.sum(axis=1)).reshape(-1)
 
     k = r.nonzero()[0]
 
     D_1 = sprs.csr_matrix((1 / r[k], (k, k)), shape=(n, n))
 
     if personalize is None:
-        personalize = sp.ones(n)
+        personalize = np.ones(n)
     personalize = personalize.reshape(n, 1)
     s = (personalize / personalize.sum()) * n
 
-    z_T = (((1 - p) * (r != 0) + (r == 0)) / n)[sp.newaxis, :]
+    z_T = (((1 - p) * (r != 0) + (r == 0)) / n)[np.newaxis, :]
     W = p * A.T @ D_1
 
-    x = s
-    oldx = sp.zeros((n, 1))
+    x = s / n
+    oldx = np.zeros((n, 1))
 
     iteration = 0
 
-    while sp.linalg.norm(x - oldx) > tol:
+    while np.linalg.norm(x - oldx) > tol:
         oldx = x
         x = W @ x + s @ (z_T @ x)
         iteration += 1
         if iteration >= max_iter:
             break
     x = x / sum(x)
```

### Comparing `fast-pagerank-0.0.4/fast_pagerank.egg-info/PKG-INFO` & `fast-pagerank-1.0.0/fast_pagerank.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,69 +1,71 @@
 Metadata-Version: 2.1
 Name: fast-pagerank
-Version: 0.0.4
+Version: 1.0.0
 Summary: A fast PageRank and Personalized PageRank implementation
 Home-page: https://github.com/asajadi/fast_pagerank
 Author: Armin Sajadi
 Author-email: asajadi@gmail.com
-License: UNKNOWN
-Description: # Fast Personalized PageRank Implementation
-        
-        I needed a fast PageRank for [Wikisim](https://github.com/asajadi/wikisim) project. It had to be fast enough to run real time on relatively large graphs. NetworkX was the obvious library to use, however, it needed back and forth translation from my graph representation (which was the pretty standard csr matrix), to its internal graph data structure. These translations were slowing down the process. 
-        
-        I implemented two versions of the algorithm in Python, both inspired by the sparse fast solutions given in [**Cleve Moler**](https://en.wikipedia.org/wiki/Cleve_Moler)'s book, [*Experiments with MATLAB*](https://www.mathworks.com/content/dam/mathworks/mathworks-dot-com/moler/exm/chapters/pagerank.pdf). The power method is much faster with enough precision for our task. 
-        
-        ### Personalized PageRank
-        I modified the algorithm a little bit to be able to calculate **personalized PageRank** as well. 
-        
-        
-        ### Comparison with Popular Python Implementations: NetworkX and iGraph
-        Both implementations (exact solution and *power method*) are much faster than their correspondent methods in NetworkX. The *power method* is also faster than the iGraph native implementation, which is also an eigen-vector based solution. Benchmarking is done on a `ml.t3.2xlarge` SageMaker instance. 
-        
-        ### What is the major drawback of NetworkX PageRank?
-        I gave up using NetworkX for one simple reason: I had to calculate PageRank several times, and my internal representation of a graph was a simple sparse matrix. Every time I wanted to calculate PageRank I had to translate it to the graph representation of NetworkX, which was slow. My benchmarking shows that NetworkX  has a pretty fast implementation of PageRank ( `networkx.pagerank_numpy` and  '`networkx.pagerank_scipy`), but translating from its own graph data structure to a csr matrix before doing the actual calculations is exactly what exactly slows down the whole algorithm. 
-        
-        **Note**: I didn't count the time spent on `nx.from_scipy_sparse_matrix` (converting a csr matrix before passing it to NetworkX PageRank) in my benchmarking, But I could! Because that was another bottleneck for me, and for many other cases that one has a `csr` adjacency matrix.
-        
-        ### Python Implementation
-        The python package is hosted at https://github.com/asajadi/fast-pagerank and you can find the installation guide in the [README.md](https://github.com/asajadi/fast-pagerank/blob/master/README.md) file. You also can find a detailed analysis in [the jupyter notebook](https://github.com/asajadi/fast-pagerank/blob/master/notebooks/Fast-PageRank.ipynb) or [this blog post](https://asajadi.github.io/fast-pagerank/). 
-        
-        
-        ## Usage
-        ### Installation:
-        `pip install fast-pagerank`
-        
-        ### Example
-        Let's take Example 1 from https://www.cs.princeton.edu/~chazelle/courses/BIB/pagerank.htm 
-        
-        ![](example1.gif)
-        
-        Assuming A=0, B=1, C=2, D=3:
-        
-        ```
-        >>> import numpy as np
-        >>> from scipy import sparse
-        >>> from fast_pagerank import pagerank
-        >>> from fast_pagerank import pagerank_power
-        >>> A = np.array([[0,1], [0, 2], [1, 2],[2,0],[3,2]])
-        >>> weights = [1,1,1,1,1]
-        >>> G = sparse.csr_matrix((weights, (A[:,0], A[:,1])), shape=(4, 4))
-        >>> pr=pagerank(G, p=0.85)
-        >>> pr
-        array([0.37252685, 0.19582391, 0.39414924, 0.0375    ])
-        ```
-        
-        The output elements are essentially the same numbers written on the nodes, but normalized (multiply the vector by 4 and you will get the same numbers) 
-        
-        We can add personalization, or use *power method*:
-        
-        ```
-        >>> personalize = np.array([0.4, 0.2, 0.2, 0.4])
-        >>> pr=pagerank_power(G, p=0.85, personalize=personalize, tol=1e-6)
-        >>> pr
-        array([0.37817981, 0.18572635, 0.38609383, 0.05      ])
-        ```
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+[![996.icu](https://img.shields.io/badge/link-996.icu-red.svg)](https://996.icu/#/en_US)
+
+# Fast Personalized PageRank Implementation
+
+I needed a fast PageRank for [Wikisim](https://github.com/asajadi/wikisim) project. It had to be fast enough to run real time on relatively large graphs. NetworkX was the obvious library to use, however, it needed back and forth translation from my graph representation (which was the pretty standard csr matrix), to its internal graph data structure. These translations were slowing down the process. 
+
+I implemented two versions of the algorithm in Python, both inspired by the sparse fast solutions given in [**Cleve Moler**](https://en.wikipedia.org/wiki/Cleve_Moler)'s book, [*Experiments with MATLAB*](https://www.mathworks.com/content/dam/mathworks/mathworks-dot-com/moler/exm/chapters/pagerank.pdf). The power method is much faster with enough precision for our task. 
+
+### Personalized PageRank
+I modified the algorithm a little bit to be able to calculate **personalized PageRank** as well. 
+
+
+### Comparison with Popular Python Implementations: NetworkX and iGraph
+Both implementations (exact solution and *power method*) are much faster than their correspondent methods in NetworkX. The *power method* is also faster than the iGraph native implementation, which is also an eigen-vector based solution. Benchmarking is done on a `ml.t3.2xlarge` SageMaker instance. 
+
+### What is the major drawback of NetworkX PageRank?
+I gave up using NetworkX for one simple reason: I had to calculate PageRank several times, and my internal representation of a graph was a simple sparse matrix. Every time I wanted to calculate PageRank I had to translate it to the graph representation of NetworkX, which was slow. My benchmarking shows that NetworkX  has a pretty fast implementation of PageRank ( `networkx.pagerank_numpy` and  '`networkx.pagerank_scipy`), but translating from its own graph data structure to a csr matrix before doing the actual calculations is exactly what exactly slows down the whole algorithm. 
+
+**Note**: I didn't count the time spent on `nx.from_scipy_sparse_matrix` (converting a csr matrix before passing it to NetworkX PageRank) in my benchmarking, But I could! Because that was another bottleneck for me, and for many other cases that one has a `csr` adjacency matrix.
+
+### Python Implementation
+The python package is hosted at https://github.com/asajadi/fast-pagerank and you can find the installation guide in the [README.md](https://github.com/asajadi/fast-pagerank/blob/master/README.md) file. You also can find a detailed analysis in [the jupyter notebook](https://github.com/asajadi/fast-pagerank/blob/master/notebooks/Fast-PageRank.ipynb) or [this blog post](https://asajadi.github.io/fast-pagerank/). 
+
+
+## Usage
+### Installation:
+`pip install fast-pagerank`
+
+### Example
+Let's take Example 1 from https://www.cs.princeton.edu/~chazelle/courses/BIB/pagerank.htm 
+
+![](example1.gif)
+
+Assuming A=0, B=1, C=2, D=3:
+
+```
+>>> import numpy as np
+>>> from scipy import sparse
+>>> from fast_pagerank import pagerank
+>>> from fast_pagerank import pagerank_power
+>>> A = np.array([[0,1], [0, 2], [1, 2],[2,0],[3,2]])
+>>> weights = [1,1,1,1,1]
+>>> G = sparse.csr_matrix((weights, (A[:,0], A[:,1])), shape=(4, 4))
+>>> pr=pagerank(G, p=0.85)
+>>> pr
+array([0.37252685, 0.19582391, 0.39414924, 0.0375    ])
+```
+
+The output elements are essentially the same numbers written on the nodes, but normalized (multiply the vector by 4 and you will get the same numbers) 
+
+We can add personalization, or use *power method*:
+
+```
+>>> personalize = np.array([0.4, 0.2, 0.2, 0.4])
+>>> pr=pagerank_power(G, p=0.85, personalize=personalize, tol=1e-6)
+>>> pr
+array([0.37817981, 0.18572635, 0.38609383, 0.05      ])
+```
```

### Comparing `fast-pagerank-0.0.4/setup.py` & `fast-pagerank-1.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="fast-pagerank",
-    version="0.0.4",
+    version="1.0.0",
     author="Armin Sajadi",
     author_email="asajadi@gmail.com",
     description="A fast PageRank and Personalized PageRank implementation",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/asajadi/fast_pagerank",
     packages=setuptools.find_packages(),
```

