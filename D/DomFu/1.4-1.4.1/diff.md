# Comparing `tmp/DomFu-1.4.tar.gz` & `tmp/DomFu-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DomFu-1.4.tar", last modified: Sun Jul  2 20:30:22 2023, max compression
+gzip compressed data, was "DomFu-1.4.1.tar", last modified: Sun Jul  2 20:45:38 2023, max compression
```

## Comparing `DomFu-1.4.tar` & `DomFu-1.4.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-02 20:30:22.670242 DomFu-1.4/
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-02 20:30:22.666115 DomFu-1.4/DomFu/
--rw-r--r--   0 root         (0) staff       (20)      437 2023-07-02 20:27:04.000000 DomFu-1.4/DomFu/__init__.py
--rw-r--r--   0 root         (0) staff       (20)    13789 2023-07-02 20:14:47.000000 DomFu-1.4/DomFu/__main__.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-02 20:30:22.667339 DomFu-1.4/DomFu/modules/
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-02 20:30:22.667566 DomFu-1.4/DomFu/modules/Probe/
--rw-r--r--   0 root         (0) staff       (20)        0 2023-06-29 07:07:33.000000 DomFu-1.4/DomFu/modules/Probe/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     1476 2023-07-02 10:17:39.000000 DomFu-1.4/DomFu/modules/Probe/probe.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-02 20:30:22.669792 DomFu-1.4/DomFu/modules/Spies/
--rw-r--r--   0 root         (0) staff       (20)     1185 2023-07-02 17:54:56.000000 DomFu-1.4/DomFu/modules/Spies/VirusTotal.py
--rw-r--r--   0 root         (0) staff       (20)        0 2023-06-29 07:07:33.000000 DomFu-1.4/DomFu/modules/Spies/__init__.py
--rw-r--r--   0 root         (0) staff       (20)      794 2023-06-29 18:27:45.000000 DomFu-1.4/DomFu/modules/Spies/alienvault.py
--rw-r--r--   0 root         (0) staff       (20)      866 2023-06-29 18:19:39.000000 DomFu-1.4/DomFu/modules/Spies/certspot.py
--rw-r--r--   0 root         (0) staff       (20)      921 2023-06-29 07:07:33.000000 DomFu-1.4/DomFu/modules/Spies/chaos.py
--rw-r--r--   0 root         (0) staff       (20)      766 2023-06-29 09:20:48.000000 DomFu-1.4/DomFu/modules/Spies/crtsh.py
--rw-r--r--   0 root         (0) staff       (20)      827 2023-06-29 07:07:33.000000 DomFu-1.4/DomFu/modules/Spies/shodan.py
--rw-r--r--   0 root         (0) staff       (20)     3419 2023-07-02 20:26:54.000000 DomFu-1.4/DomFu/modules/Spies/subdomain.py
--rw-r--r--   0 root         (0) staff       (20)      988 2023-07-02 20:15:05.000000 DomFu-1.4/DomFu/modules/Spies/webarchive.py
--rw-r--r--   0 root         (0) staff       (20)        0 2023-06-29 07:07:33.000000 DomFu-1.4/DomFu/modules/__init__.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-02 20:30:22.667201 DomFu-1.4/DomFu.egg-info/
--rw-r--r--   0 root         (0) staff       (20)     2979 2023-07-02 20:30:22.000000 DomFu-1.4/DomFu.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)      616 2023-07-02 20:30:22.000000 DomFu-1.4/DomFu.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) staff       (20)        1 2023-07-02 20:30:22.000000 DomFu-1.4/DomFu.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) staff       (20)       50 2023-07-02 20:30:22.000000 DomFu-1.4/DomFu.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) staff       (20)       57 2023-07-02 20:30:22.000000 DomFu-1.4/DomFu.egg-info/requires.txt
--rw-r--r--   0 root         (0) staff       (20)        6 2023-07-02 20:30:22.000000 DomFu-1.4/DomFu.egg-info/top_level.txt
--rw-r--r--   0 root         (0) staff       (20)    35149 2023-06-29 07:07:33.000000 DomFu-1.4/LICENSE.txt
--rw-r--r--   0 root         (0) staff       (20)     2979 2023-07-02 20:30:22.670120 DomFu-1.4/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)     2674 2023-07-02 20:29:31.000000 DomFu-1.4/README.md
--rw-r--r--   0 root         (0) staff       (20)       38 2023-07-02 20:30:22.670281 DomFu-1.4/setup.cfg
--rw-r--r--   0 root         (0) staff       (20)      705 2023-07-02 20:16:09.000000 DomFu-1.4/setup.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-02 20:45:38.077575 DomFu-1.4.1/
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-02 20:45:38.074919 DomFu-1.4.1/DomFu/
+-rw-r--r--   0 root         (0) staff       (20)      437 2023-07-02 20:27:04.000000 DomFu-1.4.1/DomFu/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)    13789 2023-07-02 20:14:47.000000 DomFu-1.4.1/DomFu/__main__.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-02 20:45:38.075873 DomFu-1.4.1/DomFu/modules/
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-02 20:45:38.076115 DomFu-1.4.1/DomFu/modules/Probe/
+-rw-r--r--   0 root         (0) staff       (20)        0 2023-06-29 07:07:33.000000 DomFu-1.4.1/DomFu/modules/Probe/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     1476 2023-07-02 10:17:39.000000 DomFu-1.4.1/DomFu/modules/Probe/probe.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-02 20:45:38.077263 DomFu-1.4.1/DomFu/modules/Spies/
+-rw-r--r--   0 root         (0) staff       (20)     1185 2023-07-02 17:54:56.000000 DomFu-1.4.1/DomFu/modules/Spies/VirusTotal.py
+-rw-r--r--   0 root         (0) staff       (20)        0 2023-06-29 07:07:33.000000 DomFu-1.4.1/DomFu/modules/Spies/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)      794 2023-06-29 18:27:45.000000 DomFu-1.4.1/DomFu/modules/Spies/alienvault.py
+-rw-r--r--   0 root         (0) staff       (20)      866 2023-06-29 18:19:39.000000 DomFu-1.4.1/DomFu/modules/Spies/certspot.py
+-rw-r--r--   0 root         (0) staff       (20)      921 2023-06-29 07:07:33.000000 DomFu-1.4.1/DomFu/modules/Spies/chaos.py
+-rw-r--r--   0 root         (0) staff       (20)      766 2023-06-29 09:20:48.000000 DomFu-1.4.1/DomFu/modules/Spies/crtsh.py
+-rw-r--r--   0 root         (0) staff       (20)      827 2023-06-29 07:07:33.000000 DomFu-1.4.1/DomFu/modules/Spies/shodan.py
+-rw-r--r--   0 root         (0) staff       (20)     3419 2023-07-02 20:42:17.000000 DomFu-1.4.1/DomFu/modules/Spies/subdomain.py
+-rw-r--r--   0 root         (0) staff       (20)      988 2023-07-02 20:15:05.000000 DomFu-1.4.1/DomFu/modules/Spies/webarchive.py
+-rw-r--r--   0 root         (0) staff       (20)        0 2023-06-29 07:07:33.000000 DomFu-1.4.1/DomFu/modules/__init__.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-02 20:45:38.075652 DomFu-1.4.1/DomFu.egg-info/
+-rw-r--r--   0 root         (0) staff       (20)     2985 2023-07-02 20:45:38.000000 DomFu-1.4.1/DomFu.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)      616 2023-07-02 20:45:38.000000 DomFu-1.4.1/DomFu.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) staff       (20)        1 2023-07-02 20:45:38.000000 DomFu-1.4.1/DomFu.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) staff       (20)       50 2023-07-02 20:45:38.000000 DomFu-1.4.1/DomFu.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) staff       (20)       57 2023-07-02 20:45:38.000000 DomFu-1.4.1/DomFu.egg-info/requires.txt
+-rw-r--r--   0 root         (0) staff       (20)        6 2023-07-02 20:45:38.000000 DomFu-1.4.1/DomFu.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) staff       (20)    35149 2023-06-29 07:07:33.000000 DomFu-1.4.1/LICENSE.txt
+-rw-r--r--   0 root         (0) staff       (20)     2985 2023-07-02 20:45:38.077451 DomFu-1.4.1/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)     2678 2023-07-02 20:44:11.000000 DomFu-1.4.1/README.md
+-rw-r--r--   0 root         (0) staff       (20)       38 2023-07-02 20:45:38.077614 DomFu-1.4.1/setup.cfg
+-rw-r--r--   0 root         (0) staff       (20)      707 2023-07-02 20:44:37.000000 DomFu-1.4.1/setup.py
```

### Comparing `DomFu-1.4/DomFu/__main__.py` & `DomFu-1.4.1/DomFu/__main__.py`

 * *Files identical despite different names*

### Comparing `DomFu-1.4/DomFu/modules/Probe/probe.py` & `DomFu-1.4.1/DomFu/modules/Probe/probe.py`

 * *Files identical despite different names*

### Comparing `DomFu-1.4/DomFu/modules/Spies/VirusTotal.py` & `DomFu-1.4.1/DomFu/modules/Spies/VirusTotal.py`

 * *Files identical despite different names*

### Comparing `DomFu-1.4/DomFu/modules/Spies/alienvault.py` & `DomFu-1.4.1/DomFu/modules/Spies/alienvault.py`

 * *Files identical despite different names*

### Comparing `DomFu-1.4/DomFu/modules/Spies/certspot.py` & `DomFu-1.4.1/DomFu/modules/Spies/certspot.py`

 * *Files identical despite different names*

### Comparing `DomFu-1.4/DomFu/modules/Spies/chaos.py` & `DomFu-1.4.1/DomFu/modules/Spies/chaos.py`

 * *Files identical despite different names*

### Comparing `DomFu-1.4/DomFu/modules/Spies/crtsh.py` & `DomFu-1.4.1/DomFu/modules/Spies/crtsh.py`

 * *Files identical despite different names*

### Comparing `DomFu-1.4/DomFu/modules/Spies/shodan.py` & `DomFu-1.4.1/DomFu/modules/Spies/shodan.py`

 * *Files identical despite different names*

### Comparing `DomFu-1.4/DomFu/modules/Spies/subdomain.py` & `DomFu-1.4.1/DomFu/modules/Spies/subdomain.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from threading import *
 import queue
 from .crtsh import fetchCrtSh
 from .VirusTotal import fetchVirusTotal
 from .shodan import fetchShodan
 from .chaos import fetchChaos
 from .certspot import fetchCertSpot
-from .alienVault import fetchAlienv
+from .alienvault import fetchAlienv
 from .webarchive import fetchWebArchive
 
 
 def fetchAll(domain):
     '''
     string -> list
```

### Comparing `DomFu-1.4/DomFu/modules/Spies/webarchive.py` & `DomFu-1.4.1/DomFu/modules/Spies/webarchive.py`

 * *Files identical despite different names*

### Comparing `DomFu-1.4/DomFu.egg-info/PKG-INFO` & `DomFu-1.4.1/DomFu.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DomFu
-Version: 1.4
+Version: 1.4.1
 Summary: A CLI app to find domains and subdomains of a given domain
 Home-page: http://pypi.python.org/pypi/domfu/
 Author: Suman Basuli
 Author-email: thinisadhu@gmail.com
 License: LICENSE.txt
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
@@ -14,15 +14,15 @@
 </p>
 
 <p align="center">
   <a href="https://www.python.org/download/releases/3.8">
     <img src="https://img.shields.io/badge/Python-3.8-green.svg">
   </a>
   <a href="https://github.com/txsadhu/domfu/releases">
-    <img src="https://img.shields.io/badge/DomFu-v1.4-violet.svg">
+    <img src="https://img.shields.io/badge/DomFu-v1.4.1-violet.svg">
   </a>
   <a href="https://github.com/txsadhu/domfu/">
       <img src="https://img.shields.io/badge/Tested%20on-Linux-yellow.svg">
   </a>
   <a href="https://github.com/TxSadhu/DomFu/blob/master/LICENSE.txt">
     <img src="https://img.shields.io/badge/License-GPLv3-orange.svg">
   </a> 
@@ -62,15 +62,15 @@
 
 ## Update
 
 **Using pip:**
 
 ```bash
 $ sudo apt-get update -y
-$ sudo pip install DomFu==1.4 --upgrade
+$ sudo pip install DomFu==1.4.1 --upgrade
 ```
 
 **Manual Installation:**
 
 ```
 $ git clone https://github.com/TxSadhu/DomFu.git
 $ cd DomFu
```

#### html2text {}

```diff
@@ -1,23 +1,23 @@
-Metadata-Version: 2.1 Name: DomFu Version: 1.4 Summary: A CLI app to find
+Metadata-Version: 2.1 Name: DomFu Version: 1.4.1 Summary: A CLI app to find
 domains and subdomains of a given domain Home-page: http://pypi.python.org/
 pypi/domfu/ Author: Suman Basuli Author-email: thinisadhu@gmail.com License:
 LICENSE.txt Description-Content-Type: text/markdown License-File: LICENSE.txt
                                  [DomFu_logo]
  [https://img.shields.io/badge/Python-3.8-green.svg] [https://img.shields.io/
- badge/DomFu-v1.4-violet.svg] [https://img.shields.io/badge/Tested%20on-Linux-
+badge/DomFu-v1.4.1-violet.svg] [https://img.shields.io/badge/Tested%20on-Linux-
  yellow.svg] [https://img.shields.io/badge/License-GPLv3-orange.svg] [https://
                 img.shields.io/badge/Release-Stable-green.svg]
 --- A python module to find domains and subdomains of a given domain with a
 easy to use CLI. ## Installation **Using pip:** ```bash $ sudo apt-get update -
 y $ sudo pip install DomFu ``` **Manual Installation:** ```bash $ git clone
 https://github.com/TxSadhu/DomFu.git $ cd DomFu $ sudo python setup.py install
 ``` ## Post-Installation **Initiate the DB:** ```bash $ domfu api ``` ## Update
-**Using pip:** ```bash $ sudo apt-get update -y $ sudo pip install DomFu==1.4 -
--upgrade ``` **Manual Installation:** ``` $ git clone https://github.com/
+**Using pip:** ```bash $ sudo apt-get update -y $ sudo pip install DomFu==1.4.1
+--upgrade ``` **Manual Installation:** ``` $ git clone https://github.com/
 TxSadhu/DomFu.git $ cd DomFu $ sudo python setup.py install ``` ## Usage
 **Using as Standalone CLI app:** ```bash domfu --help ``` **Using it as a
 python module:** ([Check the wiki for more](https://github.com/TxSadhu/DomFu/
 wiki/Using-the-python-module)) ```python import DomFu as df dom = "tropyl.com"
 # Using all sources: df.subdomain(dom) # Using individual sources to find
 subdomain: df.fetchCrtSh(dom) df.fetchBufferOverRun(dom) df.fetchHackerTarget
 (dom) df.fetchThreatCrowd(dom) df.fetchVirusTotal(dom) # Check if a list of
```

### Comparing `DomFu-1.4/DomFu.egg-info/SOURCES.txt` & `DomFu-1.4.1/DomFu.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `DomFu-1.4/LICENSE.txt` & `DomFu-1.4.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `DomFu-1.4/PKG-INFO` & `DomFu-1.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DomFu
-Version: 1.4
+Version: 1.4.1
 Summary: A CLI app to find domains and subdomains of a given domain
 Home-page: http://pypi.python.org/pypi/domfu/
 Author: Suman Basuli
 Author-email: thinisadhu@gmail.com
 License: LICENSE.txt
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
@@ -14,15 +14,15 @@
 </p>
 
 <p align="center">
   <a href="https://www.python.org/download/releases/3.8">
     <img src="https://img.shields.io/badge/Python-3.8-green.svg">
   </a>
   <a href="https://github.com/txsadhu/domfu/releases">
-    <img src="https://img.shields.io/badge/DomFu-v1.4-violet.svg">
+    <img src="https://img.shields.io/badge/DomFu-v1.4.1-violet.svg">
   </a>
   <a href="https://github.com/txsadhu/domfu/">
       <img src="https://img.shields.io/badge/Tested%20on-Linux-yellow.svg">
   </a>
   <a href="https://github.com/TxSadhu/DomFu/blob/master/LICENSE.txt">
     <img src="https://img.shields.io/badge/License-GPLv3-orange.svg">
   </a> 
@@ -62,15 +62,15 @@
 
 ## Update
 
 **Using pip:**
 
 ```bash
 $ sudo apt-get update -y
-$ sudo pip install DomFu==1.4 --upgrade
+$ sudo pip install DomFu==1.4.1 --upgrade
 ```
 
 **Manual Installation:**
 
 ```
 $ git clone https://github.com/TxSadhu/DomFu.git
 $ cd DomFu
```

#### html2text {}

```diff
@@ -1,23 +1,23 @@
-Metadata-Version: 2.1 Name: DomFu Version: 1.4 Summary: A CLI app to find
+Metadata-Version: 2.1 Name: DomFu Version: 1.4.1 Summary: A CLI app to find
 domains and subdomains of a given domain Home-page: http://pypi.python.org/
 pypi/domfu/ Author: Suman Basuli Author-email: thinisadhu@gmail.com License:
 LICENSE.txt Description-Content-Type: text/markdown License-File: LICENSE.txt
                                  [DomFu_logo]
  [https://img.shields.io/badge/Python-3.8-green.svg] [https://img.shields.io/
- badge/DomFu-v1.4-violet.svg] [https://img.shields.io/badge/Tested%20on-Linux-
+badge/DomFu-v1.4.1-violet.svg] [https://img.shields.io/badge/Tested%20on-Linux-
  yellow.svg] [https://img.shields.io/badge/License-GPLv3-orange.svg] [https://
                 img.shields.io/badge/Release-Stable-green.svg]
 --- A python module to find domains and subdomains of a given domain with a
 easy to use CLI. ## Installation **Using pip:** ```bash $ sudo apt-get update -
 y $ sudo pip install DomFu ``` **Manual Installation:** ```bash $ git clone
 https://github.com/TxSadhu/DomFu.git $ cd DomFu $ sudo python setup.py install
 ``` ## Post-Installation **Initiate the DB:** ```bash $ domfu api ``` ## Update
-**Using pip:** ```bash $ sudo apt-get update -y $ sudo pip install DomFu==1.4 -
--upgrade ``` **Manual Installation:** ``` $ git clone https://github.com/
+**Using pip:** ```bash $ sudo apt-get update -y $ sudo pip install DomFu==1.4.1
+--upgrade ``` **Manual Installation:** ``` $ git clone https://github.com/
 TxSadhu/DomFu.git $ cd DomFu $ sudo python setup.py install ``` ## Usage
 **Using as Standalone CLI app:** ```bash domfu --help ``` **Using it as a
 python module:** ([Check the wiki for more](https://github.com/TxSadhu/DomFu/
 wiki/Using-the-python-module)) ```python import DomFu as df dom = "tropyl.com"
 # Using all sources: df.subdomain(dom) # Using individual sources to find
 subdomain: df.fetchCrtSh(dom) df.fetchBufferOverRun(dom) df.fetchHackerTarget
 (dom) df.fetchThreatCrowd(dom) df.fetchVirusTotal(dom) # Check if a list of
```

### Comparing `DomFu-1.4/README.md` & `DomFu-1.4.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 </p>
 
 <p align="center">
   <a href="https://www.python.org/download/releases/3.8">
     <img src="https://img.shields.io/badge/Python-3.8-green.svg">
   </a>
   <a href="https://github.com/txsadhu/domfu/releases">
-    <img src="https://img.shields.io/badge/DomFu-v1.4-violet.svg">
+    <img src="https://img.shields.io/badge/DomFu-v1.4.1-violet.svg">
   </a>
   <a href="https://github.com/txsadhu/domfu/">
       <img src="https://img.shields.io/badge/Tested%20on-Linux-yellow.svg">
   </a>
   <a href="https://github.com/TxSadhu/DomFu/blob/master/LICENSE.txt">
     <img src="https://img.shields.io/badge/License-GPLv3-orange.svg">
   </a> 
@@ -51,15 +51,15 @@
 
 ## Update
 
 **Using pip:**
 
 ```bash
 $ sudo apt-get update -y
-$ sudo pip install DomFu==1.4 --upgrade
+$ sudo pip install DomFu==1.4.1 --upgrade
 ```
 
 **Manual Installation:**
 
 ```
 $ git clone https://github.com/TxSadhu/DomFu.git
 $ cd DomFu
```

#### html2text {}

```diff
@@ -1,19 +1,19 @@
                                  [DomFu_logo]
  [https://img.shields.io/badge/Python-3.8-green.svg] [https://img.shields.io/
- badge/DomFu-v1.4-violet.svg] [https://img.shields.io/badge/Tested%20on-Linux-
+badge/DomFu-v1.4.1-violet.svg] [https://img.shields.io/badge/Tested%20on-Linux-
  yellow.svg] [https://img.shields.io/badge/License-GPLv3-orange.svg] [https://
                 img.shields.io/badge/Release-Stable-green.svg]
 --- A python module to find domains and subdomains of a given domain with a
 easy to use CLI. ## Installation **Using pip:** ```bash $ sudo apt-get update -
 y $ sudo pip install DomFu ``` **Manual Installation:** ```bash $ git clone
 https://github.com/TxSadhu/DomFu.git $ cd DomFu $ sudo python setup.py install
 ``` ## Post-Installation **Initiate the DB:** ```bash $ domfu api ``` ## Update
-**Using pip:** ```bash $ sudo apt-get update -y $ sudo pip install DomFu==1.4 -
--upgrade ``` **Manual Installation:** ``` $ git clone https://github.com/
+**Using pip:** ```bash $ sudo apt-get update -y $ sudo pip install DomFu==1.4.1
+--upgrade ``` **Manual Installation:** ``` $ git clone https://github.com/
 TxSadhu/DomFu.git $ cd DomFu $ sudo python setup.py install ``` ## Usage
 **Using as Standalone CLI app:** ```bash domfu --help ``` **Using it as a
 python module:** ([Check the wiki for more](https://github.com/TxSadhu/DomFu/
 wiki/Using-the-python-module)) ```python import DomFu as df dom = "tropyl.com"
 # Using all sources: df.subdomain(dom) # Using individual sources to find
 subdomain: df.fetchCrtSh(dom) df.fetchBufferOverRun(dom) df.fetchHackerTarget
 (dom) df.fetchThreatCrowd(dom) df.fetchVirusTotal(dom) # Check if a list of
```

### Comparing `DomFu-1.4/setup.py` & `DomFu-1.4.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='DomFu',
-    version='1.4',
+    version='1.4.1',
     author='Suman Basuli',
     author_email='thinisadhu@gmail.com',
     packages=find_packages(),
     include_package_data=True,
     url='http://pypi.python.org/pypi/domfu/',
     license='LICENSE.txt',
     description='A CLI app to find domains and subdomains of a given domain',
```

