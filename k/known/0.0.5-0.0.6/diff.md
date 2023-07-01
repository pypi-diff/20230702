# Comparing `tmp/known-0.0.5.tar.gz` & `tmp/known-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "known-0.0.5.tar", last modified: Fri Mar 31 03:23:03 2023, max compression
+gzip compressed data, was "known-0.0.6.tar", last modified: Sat Jul  1 21:58:40 2023, max compression
```

## Comparing `known-0.0.5.tar` & `known-0.0.6.tar`

### file list

```diff
@@ -1,15 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-03-31 03:23:03.462794 known-0.0.5/
--rw-rw-rw-   0        0        0     1102 2023-01-13 14:13:36.000000 known-0.0.5/LICENSE
--rw-rw-rw-   0        0        0      263 2023-03-31 03:23:03.461791 known-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      374 2023-03-31 03:04:32.000000 known-0.0.5/README.rst
-drwxrwxrwx   0        0        0        0 2023-03-31 03:23:03.415789 known-0.0.5/module/
-drwxrwxrwx   0        0        0        0 2023-03-31 03:23:03.424791 known-0.0.5/module/known/
--rw-rw-rw-   0        0        0      522 2023-03-30 23:01:19.000000 known-0.0.5/module/known/__init__.py
--rw-rw-rw-   0        0        0    19221 2023-03-31 00:07:01.000000 known-0.0.5/module/known/basic.py
-drwxrwxrwx   0        0        0        0 2023-03-31 03:23:03.459793 known-0.0.5/module/known.egg-info/
--rw-rw-rw-   0        0        0      263 2023-03-31 03:23:03.000000 known-0.0.5/module/known.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      218 2023-03-31 03:23:03.000000 known-0.0.5/module/known.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-31 03:23:03.000000 known-0.0.5/module/known.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-03-31 03:23:03.000000 known-0.0.5/module/known.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-31 03:23:03.463793 known-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      594 2023-03-31 03:22:03.000000 known-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-01 21:58:40.519152 known-0.0.6/
+-rw-rw-rw-   0        0        0     1102 2023-01-13 14:13:36.000000 known-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0      263 2023-07-01 21:58:40.518158 known-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      442 2023-03-31 14:51:15.000000 known-0.0.6/README.rst
+drwxrwxrwx   0        0        0        0 2023-07-01 21:58:40.494175 known-0.0.6/module/
+drwxrwxrwx   0        0        0        0 2023-07-01 21:58:40.503153 known-0.0.6/module/known/
+-rw-rw-rw-   0        0        0      555 2023-07-01 21:52:09.000000 known-0.0.6/module/known/__init__.py
+-rw-rw-rw-   0        0        0    21804 2023-07-01 21:41:03.000000 known-0.0.6/module/known/basic.py
+-rw-rw-rw-   0        0        0     6166 2023-07-01 21:51:03.000000 known-0.0.6/module/known/imgu.py
+-rw-rw-rw-   0        0        0    10284 2023-07-01 18:24:41.000000 known-0.0.6/module/known/mailer.py
+-rw-rw-rw-   0        0        0     5849 2023-06-24 16:36:17.000000 known-0.0.6/module/known/store.py
+drwxrwxrwx   0        0        0        0 2023-07-01 21:58:40.516149 known-0.0.6/module/known.egg-info/
+-rw-rw-rw-   0        0        0      263 2023-07-01 21:58:40.000000 known-0.0.6/module/known.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      284 2023-07-01 21:58:40.000000 known-0.0.6/module/known.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-01 21:58:40.000000 known-0.0.6/module/known.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-07-01 21:58:40.000000 known-0.0.6/module/known.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-01 21:58:40.519152 known-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      595 2023-07-01 21:49:59.000000 known-0.0.6/setup.py
```

### Comparing `known-0.0.5/LICENSE` & `known-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `known-0.0.5/module/known/basic.py` & `known-0.0.6/module/known/basic.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,38 +1,32 @@
 #=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=
 __doc__=r"""
 :py:mod:`known/basic.py`
 """
 #=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=
 __all__ = [
-    'now', 'fdate', 'pdate', 
-    'uid', 'pjs', 'pj', 'pname', 'pext', 'psplit', 'walk', 
-    'Fake', 'Verbose', 'BaseConvert', 
+    'now', 'numel', 'arange', 'save_json', 'load_json', 'save_pickle', 'load_pickle',
+     
+    'Symbols', 'Verbose', 'BaseConvert', 'IndexedDict', 'Remap', 
     #==============================
-    'numel', 'arange', 'd2j', 'j2d',
-    'Remap', 'Misc'
+    
+    'onehot', 'onecold', 'dict_sort', 
 ]
 #=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=
-import datetime, os
-from typing import Any, Union, Iterable
+import datetime
+from typing import Any, Union, Iterable #, BinaryIO, cast, Dict, Optional, Type, Tuple, IO
 import numpy as np
 from numpy import ndarray
 from math import floor, log
-import json
+import json, pickle
+from collections import UserDict
+#import pickle, pathlib, io
 #=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=
 
-
-# Aliased functions
-
-now = datetime.datetime.now
-fdate = datetime.datetime.strftime
-pdate = datetime.datetime.strptime
-
-
-def uid(year:bool=True, month:bool=True, day:bool=True, 
+def now(year:bool=True, month:bool=True, day:bool=True, 
         hour:bool=True, minute:bool=True, second:bool=True, mirco:bool=True, 
         start:str='', sep:str='', end:str='') -> str:
     r""" Unique Identifier - useful in generating unique identifiers based on current timestamp. 
     Helpful in generating unique filenames based on timestamps. 
     
     .. seealso::
         :func:`~known.basic.Verbose.strU`
@@ -44,80 +38,79 @@
     if hour:    form.append("%H")
     if minute:  form.append("%M")
     if second:  form.append("%S")
     if mirco:   form.append("%f")
     assert (form), 'format should not be empty!'
     return (start + datetime.datetime.strftime(datetime.datetime.now(), sep.join(form)) + end)
 
-def pjs(*paths) -> str:
-    r""" Paths Join - shorthand for `os.path.join` """
-    return os.path.join('', *paths)
-
-def pj(path:str, sep:str='/') -> str: 
-    r""" Path Join - shorthand for `os.path.join`
-
-    .. note:: This is similar to :func:`~known.basic.pjs` but instead of taking multiple args,
-        takes a single string and splits it using the provided seperator.
-    """
-    return pjs(*path.split(sep))
-
-def pname(path:str, sep:str='.'): 
-    r""" Path Name - retuns the path except file extension using ``path[0:path.rfind(sep)]`` 
-    
-    .. seealso::
-        :func:`~known.basic.pext`
-        :func:`~known.basic.psplit`
-    """
-    return path[0:path.rfind(sep)]
-
-def pext(path:str, sep:str='.'): 
-    r""" Path Extension - retuns the extension from a path using ``path[path.rfind(sep):]`` 
-
-    .. seealso::
-        :func:`~known.basic.pname`
-        :func:`~known.basic.psplit`
-    """
-    return path[path.rfind(sep):]
-
-def psplit(path:str, sep:str='.'): 
-    r""" Path Split - splits the path into name and extension
-
-    :returns: 2-tuple (Name, Ext)
-
-    .. note:: This is the same as using :func:`~known.basic.pname` and :func:`~known.basic.pext` together. 
-        This may be used to create copies of a file by adding a suffix to its name witout changing the extension.
-
-    """
-    return (path[0:path.rfind(sep)], path[path.rfind(sep):])
-
-def walk(directory):
-    r""" recursively list all files and folders in a directory """
-    file_paths = []
-    dir_paths = []
-    for root, directories, files in os.walk(directory):
-        for dirname in directories: dir_paths.append(os.path.join(root, dirname))
-        for filename in files: file_paths.append(os.path.join(root, filename))
-    return file_paths, dir_paths
-
-def numel(shape) -> int: 
+def numel(shape:Iterable) -> int: 
     r""" Returns the number of elements in an array of given shape. """
     return np.prod(np.array(shape))
 
-def arange(shape, start:int=0, step:int=1, dtype=None) -> ndarray: 
+def arange(shape:Iterable, start:int=0, step:int=1, dtype=None) -> ndarray: 
     r""" Similar to ``np.arange`` but reshapes the array to given shape. """
     return np.arange(start=start, stop=start+step*numel(shape), step=step, dtype=dtype).reshape(shape)
 
-def d2j(d, path, indent='\t', sort_keys=False):
-    r""" save dictionary to json file """
-    with open(path, 'w') as f: json.dump(d, f, indent=indent, sort_keys=sort_keys)
-
-def j2d(path):
-    r""" load json file to dictionary """
-    with open(path, 'r') as f: d = json.load(f)
-    return d
+def save_json(o:Any, path:str, **kwargs) -> None:
+    r""" save object to json file """
+    with open(path, 'w') as f: json.dump(o, f, **kwargs)
+
+def load_json(path:str) -> Any:
+    r""" load json file to object """
+    with open(path, 'r') as f: o = json.load(f)
+    return o
+
+def save_pickle(o:Any, path:str,**kwargs):
+    r""" save object to pickle file """
+    with open(path, 'wb') as f: pickle.dump(o, f,**kwargs)
+
+def load_pickle(path:str):
+    r""" load pickle file to object """
+    with open(path, 'rb') as f: o = pickle.load(f)
+    return o
+
+def onehot(total:int, index:int, **kwargs):
+    res = np.zeros(total, **kwargs)
+    res[index]=1
+    return res
+
+def onecold(total:int, index:int, **kwargs):
+    res = np.ones(total, **kwargs)
+    res[index]=0
+    return res
+
+def dict_sort(D:dict, assending:bool=True, fin=lambda x:x, fmid=lambda x:x, fout=lambda x:x, return_dict=True):
+    r""" if D is like :: dict[str, numbers], then sorts  the numbers and keys
+        
+    1. ```fin``` is applied on each number and it is appended to a list
+    2. ```fmid``` is applied on the list
+    3. create np.array from the output of fmid
+    4. ```fout``` is applied on the ndarray
+    5. argsort is applied on ndarray
+    
+    returns keys, values and indices in sorted order
+    """
+    # sorts the values and keys into lists
+    K,V = [], []
+    for k,v in D.items():
+        K.append(k)
+        V.append(fin(v))
+    K=np.array(K)
+    V=fout(np.array(fmid(V)))
+    S = np.argsort(V)
+    if assending:
+        ks = K[S]
+        vs = V[S]
+        ss = S 
+    else:
+        ks = K[S][::-1]
+        vs = V[S][::-1]
+        ss = S[::-1]
+    
+    return {k:v for k,v in zip(ks,vs)} if return_dict else (ks,vs,ss)
 
 #=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=
 
 class BaseConvert:
     r""" Number System Conversion """
 
     @staticmethod
@@ -167,121 +160,108 @@
         """
         res = 0
         for i,n in enumerate(num): res+=(base**i)*n
         return res
 
 #=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=
 
-class Fake:
-    r""" Fake Object - an object with members given in a keyword-args dict """
-    def __init__(self, **members) -> None:
-        for k,v in members.items(): setattr(self, k, v)
-    
-    @staticmethod
-    def try_create(members):
-        res = Fake()
-        failed=[]
-        for k,v in members.items(): 
-            if k:
-                try:
-                    setattr(res, k, v)
-                except:
-                    failed.append(k)
-            else:
-                failed.append(k)
-        return res, failed
-
-class Verbose:
-    r""" Contains shorthand helper functions for printing outputs and representing objects as strings.
-    
-    Also contains some special symbols described in the table below
+class Symbols:
+    r"""
+    contains some special symbols described in the table below
 
     .. list-table:: 
         :widths: 5 3 5 3
         :header-rows: 1
 
         * - Name
           - Symbol
           - Name
           - Symbol
-        * - SYM_CORRECT
+        * - CORRECT
           - ✓
-          - SYM_INCORRECT
+          - INCORRECT
           - ✗
-        * - SYM_ALPHA
+        * - ALPHA
           - α
-          - SYM_BETA
+          - BETA
           - β
-        * - SYM_GAMMA
+        * - GAMMA
           - γ
-          - SYM_DELTA
+          - DELTA
           - δ
-        * - SYM_EPSILON
+        * - EPSILON
           - ε
-          - SYM_ZETA
+          - ZETA
           - ζ
-        * - SYM_ETA
+        * - ETA
           - η
-          - SYM_THETA
+          - THETA
           - θ
-        * - SYM_KAPPA
+        * - KAPPA
           - κ
-          - SYM_LAMBDA
+          - LAMBDA
           - λ
-        * - SYM_MU
+        * - MU
           - μ 
-          - SYM_XI
+          - XI
           - ξ
-        * - SYM_PI
+        * - PI
           - π
-          - SYM_ROH
+          - ROH
           - ρ
-        * - SYM_SIGMA
+        * - SIGMA
           - σ
-          - SYM_PHI
+          - PHI
           - φ
-        * - SYM_PSI
+        * - PSI
           - Ψ
-          - SYM_TAU
+          - TAU
           - τ
-        * - SYM_OMEGA
+        * - OMEGA
           - Ω
-          - SYM_TRI
+          - TRI
           - Δ
+    """
+    
+    CORRECT =       '✓'
+    INCORRECT =     '✗'
+    ALPHA =         'α'
+    BETA =          'β'
+    GAMMA =         'γ'
+    DELTA =         'δ'
+    EPSILON =       'ε'
+    ZETA =          'ζ'
+    ETA =           'η'
+    THETA =         'θ'
+    KAPPA =         'κ'
+    LAMBDA =        'λ'
+    MU =            'μ' 
+    XI =            'ξ'
+    PI =            'π'
+    ROH =           'ρ'
+    SIGMA =         'σ'
+    PHI =           'φ'
+    PSI =           'Ψ'
+    TAU =           'τ'
+    OMEGA =         'Ω'
+    TRI =           'Δ'
+
+#=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=
+
+class Verbose:
+    r""" Contains shorthand helper functions for printing outputs and representing objects as strings.
 
     .. note::
         This class contains only static methods.
     """
     DEFAULT_DATE_FORMAT = ["%Y","%m","%d","%H","%M","%S","%f"]
     r""" Default date format for :func:`~known.basic.Verbose.strU` """
 
-    SYM_CORRECT =       '✓'
-    SYM_INCORRECT =     '✗'
-    SYM_ALPHA =         'α'
-    SYM_BETA =          'β'
-    SYM_GAMMA =         'γ'
-    SYM_DELTA =         'δ'
-    SYM_EPSILON =       'ε'
-    SYM_ZETA =          'ζ'
-    SYM_ETA =           'η'
-    SYM_THETA =         'θ'
-    SYM_KAPPA =         'κ'
-    SYM_LAMBDA =        'λ'
-    SYM_MU =            'μ' 
-    SYM_XI =            'ξ'
-    SYM_PI =            'π'
-    SYM_ROH =           'ρ'
-    SYM_SIGMA =         'σ'
-    SYM_PHI =           'φ'
-    SYM_PSI =           'Ψ'
-    SYM_TAU =           'τ'
-    SYM_OMEGA =         'Ω'
-    SYM_TRI =           'Δ'
-
     DASHED_LINE = "=-=-=-=-==-=-=-=-="
+    DOCSTR_FORM = lambda x: f'\t!docstr:\n! - - - - - - - - - - - - - - - - -\n{x}\n- - - - - - - - - - - - - - - - - !'
 
     @staticmethod
     def strN(s:str, n:int) -> str:  
         r""" Repeates a string n-times """
         return ''.join([s for _ in range(n)])
 
     @staticmethod
@@ -397,14 +377,56 @@
             try:
                 v = getattr(x, d)
             except:
                 v='?'
             print(d, cep, v)
 
     @staticmethod
+    def dir(x:Any, doc=False, filter:str='', sew=('__','__')):
+        """ Calls ```dir``` on given argument and lists the name and types of non-dunder members.
+
+        :param filter: csv string of types to filter out like `type,function,module`, keep blank for no filter
+        :param doc: shows docstring ```__doc``` 
+            If ```doc``` is True, show all member's ```__doc__```.
+            If ```doc``` is False, does not show any ```__doc__```. 
+            If ```doc``` is a string, show ```__doc__``` of specific types only given by csv string.
+
+        :param sew: 2-Tuple (start:str, end:str) - excludes member names that start and end with specific chars, 
+            used to exclude dunder methods by default
+        """
+        #if self_doc: print( f'{type(x)}\n{x.__doc__}\n' )
+        if sew: sw, ew = f'{sew[0]}', f'{sew[1]}'
+        doc_is_specified = (isinstance(doc, str) and bool(doc))
+        if doc_is_specified: doc_match =[ t for t in doc.replace(' ','').split(',') if t ]
+        if filter: filter_match =[ t for t in filter.replace(' ','').split(',') if t ]
+        counter=1
+        for k in dir(x):
+            if sew:
+                if (k.startswith(sw) and k.endswith(ew)): continue
+            m = getattr(x,k)
+            n = str(type(m)).split("'")[1]
+            if filter:
+                if not (n in filter_match):  continue
+            s = f'[{counter}] {k} :: {n}'#.encode('utf-16')
+
+            if doc:
+                if doc_is_specified:
+                    if n in doc_match: 
+                        d = __class__.DOCSTR_FORM(m.__doc__)
+                    else:
+                        d=''
+                else:
+                    d = __class__.DOCSTR_FORM(m.__doc__)
+            else:
+                d = ''
+            counter+=1
+            print(f'{s}{d}')
+
+
+    @staticmethod
     def info(x:Any, show_object:bool=False):
         r""" Shows the `type`, `length` and `shape` of an object and optionally shows the object as well.
 
         :param x:           the object to get info about
         :param show_object: if `True`, prints the object itself
 
         .. note:: This is used to check output of some functions without having to print the full output
@@ -477,63 +499,114 @@
         self.input_delta = self.input_high - self.input_low
 
     def set_output_range(self, Range:tuple) -> None:
         r""" set the output range """
         self.output_low, self.output_high = Range
         self.output_delta = self.output_high - self.output_low
 
-    def o2i(self, X):
+    def backward(self, X):
         r""" maps ``X`` from ``Output_Range`` to ``Input_Range`` """
         return ((X - self.output_low)*self.input_delta/self.output_delta) + self.input_low
 
-    def i2o(self, X):
+    def forward(self, X):
         r""" maps ``X`` from ``Input_Range`` to ``Output_Range`` """
         return ((X - self.input_low)*self.output_delta/self.input_delta) + self.output_low
 
-class Misc:
-    r""" Helpful stuff """
+    def __call__(self, X, backward=False):
+        return self.backward(X) if backward else self.forward(X)
+    
+    def swap_range(self):
+        Input_Range, Output_Range = (self.output_low, self.output_high), (self.input_low, self.input_high)
+        self.set_input_range(Input_Range)
+        self.set_output_range(Output_Range)
 
-    @staticmethod
-    def graphfromimage(img_path:str, pixel_choice:str='first', dtype=None) -> ndarray:
-        r""" 
-        Covert an image to an array (1-Dimensional)
+#=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=
+
+class IndexedDict(UserDict):
+    r""" Implements an Indexed dict where values can be addressed using both index(int) and keys(str) """
 
-        :param img_path:        path of input image 
-        :param pixel_choice:    choose from ``[ 'first', 'last', 'mid', 'mean' ]``
+    def __init__(self, **members) -> None:
+        self.names = []
+        super().__init__(*[], **members)
+    
+    def keys(self): return enumerate(self.names, 0) # for i,k in self.keys()
 
-        :returns: 1-D numpy array containing the data points
+    def items(self): return enumerate(self.data.items(), 0) # for i,(k,v) in self.items()
 
-        .. note:: 
-            * This is used to generate synthetic data in 1-Dimension. 
-                The width of the image is the number of points (x-axis),
-                while the height of the image is the range of data points, choosen based on their index along y-axis.
-        
-            * The provided image is opened in grayscale mode.
-                All the *black pixels* are considered as data points.
-                If there are multiple black points in a column then ``pixel_choice`` argument specifies which pixel to choose.
-
-            * Requires ``opencv-python``
-
-                Input image should be readable using ``cv2.imread``.
-                Use ``pip install opencv-python`` to install ``cv2`` package
-        """
-        try:
-            import cv2 # pip install opencv-python
-        except:
-            print(f'[!] failed to import cv2!')
-            return None
-        img= cv2.imread(img_path, 0)
-        imgmax = img.shape[1]-1
-        j = img*0
-        j[np.where(img==0)]=1
-        pixel_choice = pixel_choice.lower()
-        pixel_choice_dict = {
-            'first':    (lambda ai: ai[0]),
-            'last':     (lambda ai: ai[-1]),
-            'mid':      (lambda ai: ai[int(len(ai)/2)]),
-            'mean':     (lambda ai: np.mean(ai))
-        }
-        px = pixel_choice_dict[pixel_choice]
-        if dtype is None: dtype=np.float_
-        return np.array([ imgmax-px(np.where(j[:,i]==1)[0]) for i in range(j.shape[1]) ], dtype=dtype)
+    def __len__(self): return len(self.data)
+
+    def __getitem__(self, name): 
+        if isinstance(name, int): name = self.names[name]
+        if name in self.data: 
+            return self.data[name]
+        else:
+            raise KeyError(name)
+
+    def __setitem__(self, name, item): 
+        if isinstance(name, int): name = self.names[name]
+        if name not in self.data: self.names.append(name)
+        self.data[name] = item
+
+    def __delitem__(self, name): 
+        index = None
+        if isinstance(name, int):  
+            index = name
+            name = self.names[name]
+        if name in self.data: 
+            del self.names[self.names.index(name) if index is None else index]
+            del self.data[name]
+
+    def __iter__(self): return iter(self.names)
+
+    def __contains__(self, name): return name in self.data
+
+    # Now, add the methods in dicts but not in MutableMapping
+
+    def __repr__(self) -> str:
+        return f'{__class__} :: {len(self)} Members'
+    
+    def __str__(self) -> str:
+        items = ''
+        for i,k in enumerate(self):
+            items += f'[{i}] \t {k} : {self[i]}\n'
+        return f'{__class__} :: {len(self)} Members\n{items}'
+    
+    def __copy__(self):
+        inst = self.__class__.__new__(self.__class__)
+        inst.__dict__.update(self.__dict__)
+        # Create a copy and avoid triggering descriptors
+        inst.__dict__["data"] = self.__dict__["data"].copy()
+        inst.__dict__["names"] = self.__dict__["names"].copy()
+        return inst
 
 #=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=
+
+
+
+# def pname(path:str, sep:str='.'): 
+#     r""" Path Name - retuns the path except file extension using ``path[0:path.rfind(sep)]`` 
+    
+#     .. seealso::
+#         :func:`~known.basic.pext`
+#         :func:`~known.basic.psplit`
+#     """
+#     return path[0:path.rfind(sep)]
+
+# def pext(path:str, sep:str='.'): 
+#     r""" Path Extension - retuns the extension from a path using ``path[path.rfind(sep):]`` 
+
+#     .. seealso::
+#         :func:`~known.basic.pname`
+#         :func:`~known.basic.psplit`
+#     """
+#     return path[path.rfind(sep):]
+
+# def psplit(path:str, sep:str='.'): 
+#     r""" Path Split - splits the path into name and extension
+
+#     :returns: 2-tuple (Name, Ext)
+
+#     .. note:: This is the same as using :func:`~known.basic.pname` and :func:`~known.basic.pext` together. 
+#         This may be used to create copies of a file by adding a suffix to its name witout changing the extension.
+
+#     """
+#     return (path[0:path.rfind(sep)], path[path.rfind(sep):])
```

### Comparing `known-0.0.5/setup.py` & `known-0.0.6/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from setuptools import setup
+
 setup(
     name =                      'known',
-    version =                   '0.0.5',
+    version =                   '0.0.6',
     url =                       'https://github.com/Nelson-iitp/known',
     author =                    'Nelson.S',
     author_email =              'mail.nelsonsharma@gmail.com',
     description =               'Module :: known',
     packages =                  ['known'],
     classifiers=                ['License :: OSI Approved :: MIT License'],
     package_dir =               { '' : 'module'},
```

