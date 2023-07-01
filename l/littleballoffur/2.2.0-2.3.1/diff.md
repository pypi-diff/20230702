# Comparing `tmp/littleballoffur-2.2.0.tar.gz` & `tmp/littleballoffur-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/littleballoffur-2.2.0.tar", last modified: Mon Aug 15 10:35:40 2022, max compression
+gzip compressed data, was "dist/littleballoffur-2.3.1.tar", last modified: Sat Jul  1 22:12:06 2023, max compression
```

## Comparing `littleballoffur-2.2.0.tar` & `littleballoffur-2.3.1.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxrwxr-x   0 benedek   (1000) benedek   (1000)        0 2022-08-15 10:35:40.694457 littleballoffur-2.2.0/
--rw-rw-r--   0 benedek   (1000) benedek   (1000)      822 2022-08-15 10:35:40.694457 littleballoffur-2.2.0/PKG-INFO
--rw-rw-r--   0 benedek   (1000) benedek   (1000)    15940 2022-08-15 08:38:57.000000 littleballoffur-2.2.0/README.md
-drwxrwxr-x   0 benedek   (1000) benedek   (1000)        0 2022-08-15 10:35:40.690458 littleballoffur-2.2.0/littleballoffur/
--rw-rw-r--   0 benedek   (1000) benedek   (1000)      397 2022-08-15 08:43:14.000000 littleballoffur-2.2.0/littleballoffur/__init__.py
--rw-rw-r--   0 benedek   (1000) benedek   (1000)     8448 2022-08-15 08:38:57.000000 littleballoffur-2.2.0/littleballoffur/backend.py
-drwxrwxr-x   0 benedek   (1000) benedek   (1000)        0 2022-08-15 10:35:40.690458 littleballoffur-2.2.0/littleballoffur/dataset/
--rw-rw-r--   0 benedek   (1000) benedek   (1000)       40 2022-08-15 08:38:57.000000 littleballoffur-2.2.0/littleballoffur/dataset/__init__.py
--rw-rw-r--   0 benedek   (1000) benedek   (1000)     1401 2022-08-15 08:38:57.000000 littleballoffur-2.2.0/littleballoffur/dataset/dataset_reader.py
-drwxrwxr-x   0 benedek   (1000) benedek   (1000)        0 2022-08-15 10:35:40.690458 littleballoffur-2.2.0/littleballoffur/edge_sampling/
--rw-rw-r--   0 benedek   (1000) benedek   (1000)      527 2022-08-15 08:38:57.000000 littleballoffur-2.2.0/littleballoffur/edge_sampling/__init__.py
--rw-rw-r--   0 benedek   (1000) benedek   (1000)     2447 2022-08-15 08:38:57.000000 littleballoffur-2.2.0/littleballoffur/edge_sampling/hybridnodeedgesampler.py
--rw-rw-r--   0 benedek   (1000) benedek   (1000)     1582 2022-08-15 08:38:57.000000 littleballoffur-2.2.0/littleballoffur/edge_sampling/randomedgesampler.py
--rw-rw-r--   0 benedek   (1000) benedek   (1000)     1745 2022-08-15 08:38:57.000000 littleballoffur-2.2.0/littleballoffur/edge_sampling/randomedgesamplerwithinduction.py
--rw-rw-r--   0 benedek   (1000) benedek   (1000)     2548 2022-08-15 08:38:57.000000 littleballoffur-2.2.0/littleballoffur/edge_sampling/randomedgesamplerwithpartialinduction.py
--rw-rw-r--   0 benedek   (1000) benedek   (1000)     1955 2022-08-15 08:38:57.000000 littleballoffur-2.2.0/littleballoffur/edge_sampling/randomnodeedgesampler.py
-drwxrwxr-x   0 benedek   (1000) benedek   (1000)        0 2022-08-15 10:35:40.694457 littleballoffur-2.2.0/littleballoffur/exploration_sampling/
--rw-rw-r--   0 benedek   (1000) benedek   (1000)     1854 2022-08-15 08:38:57.000000 littleballoffur-2.2.0/littleballoffur/exploration_sampling/__init__.py
--rw-rw-r--   0 benedek   (1000) benedek   (1000)     2793 2022-08-15 08:38:57.000000 littleballoffur-2.2.0/littleballoffur/exploration_sampling/breadthfirstsearchsampler.py
--rw-rw-r--   0 benedek   (1000) benedek   (1000)     3450 2022-08-15 08:38:57.000000 littleballoffur-2.2.0/littleballoffur/exploration_sampling/circulatedneighborsrandomwalksampler.py
--rw-rw-r--   0 benedek   (1000) benedek   (1000)     3745 2022-08-15 08:38:57.000000 littleballoffur-2.2.0/littleballoffur/exploration_sampling/commonneighborawarerandomwalksampler.py
--rw-rw-r--   0 benedek   (1000) benedek   (1000)     3350 2022-08-15 08:38:57.000000 littleballoffur-2.2.0/littleballoffur/exploration_sampling/communitystructureexpansionsampler.py
--rw-rw-r--   0 benedek   (1000) benedek   (1000)     2968 2022-08-15 08:38:57.000000 littleballoffur-2.2.0/littleballoffur/exploration_sampling/depthfirstsearchsampler.py
--rw-rw-r--   0 benedek   (1000) benedek   (1000)     2629 2022-08-15 08:38:57.000000 littleballoffur-2.2.0/littleballoffur/exploration_sampling/diffusionsampler.py
--rw-rw-r--   0 benedek   (1000) benedek   (1000)     2707 2022-08-15 08:38:57.000000 littleballoffur-2.2.0/littleballoffur/exploration_sampling/diffusiontreesampler.py
--rw-rw-r--   0 benedek   (1000) benedek   (1000)     3917 2022-08-15 08:38:57.000000 littleballoffur-2.2.0/littleballoffur/exploration_sampling/forestfiresampler.py
--rw-rw-r--   0 benedek   (1000) benedek   (1000)     2855 2022-08-15 08:38:57.000000 littleballoffur-2.2.0/littleballoffur/exploration_sampling/frontiersampler.py
--rw-rw-r--   0 benedek   (1000) benedek   (1000)     3052 2022-08-15 08:38:57.000000 littleballoffur-2.2.0/littleballoffur/exploration_sampling/looperasedrandomwalksampler.py
--rw-rw-r--   0 benedek   (1000) benedek   (1000)     3106 2022-08-15 08:38:57.000000 littleballoffur-2.2.0/littleballoffur/exploration_sampling/metropolishastingsrandomwalksampler.py
--rw-rw-r--   0 benedek   (1000) benedek   (1000)     2984 2022-08-15 08:38:57.000000 littleballoffur-2.2.0/littleballoffur/exploration_sampling/nonbacktrackingrandomwalksampler.py
--rw-rw-r--   0 benedek   (1000) benedek   (1000)     1915 2022-08-15 08:38:57.000000 littleballoffur-2.2.0/littleballoffur/exploration_sampling/randomnodeneighborsampler.py
--rw-rw-r--   0 benedek   (1000) benedek   (1000)     2470 2022-08-15 08:38:57.000000 littleballoffur-2.2.0/littleballoffur/exploration_sampling/randomwalksampler.py
--rw-rw-r--   0 benedek   (1000) benedek   (1000)     2941 2022-08-15 08:38:57.000000 littleballoffur-2.2.0/littleballoffur/exploration_sampling/randomwalkwithjumpsampler.py
--rw-rw-r--   0 benedek   (1000) benedek   (1000)     2939 2022-08-15 08:38:57.000000 littleballoffur-2.2.0/littleballoffur/exploration_sampling/randomwalkwithrestartsampler.py
--rw-rw-r--   0 benedek   (1000) benedek   (1000)     2361 2022-08-15 08:38:57.000000 littleballoffur-2.2.0/littleballoffur/exploration_sampling/shortestpathsampler.py
--rw-rw-r--   0 benedek   (1000) benedek   (1000)     3071 2022-08-15 08:38:57.000000 littleballoffur-2.2.0/littleballoffur/exploration_sampling/snowballsampler.py
--rw-rw-r--   0 benedek   (1000) benedek   (1000)     8379 2022-08-15 08:38:57.000000 littleballoffur-2.2.0/littleballoffur/exploration_sampling/spikyballsampler.py
--rw-rw-r--   0 benedek   (1000) benedek   (1000)      211 2022-08-15 08:38:57.000000 littleballoffur-2.2.0/littleballoffur/helpers.py
-drwxrwxr-x   0 benedek   (1000) benedek   (1000)        0 2022-08-15 10:35:40.694457 littleballoffur-2.2.0/littleballoffur/node_sampling/
--rw-rw-r--   0 benedek   (1000) benedek   (1000)      254 2022-08-15 08:38:57.000000 littleballoffur-2.2.0/littleballoffur/node_sampling/__init__.py
--rw-rw-r--   0 benedek   (1000) benedek   (1000)     1933 2022-08-15 08:38:57.000000 littleballoffur-2.2.0/littleballoffur/node_sampling/degreebasedsampler.py
--rw-rw-r--   0 benedek   (1000) benedek   (1000)     1997 2022-08-15 08:38:57.000000 littleballoffur-2.2.0/littleballoffur/node_sampling/pagerankbasedsampler.py
--rw-rw-r--   0 benedek   (1000) benedek   (1000)     1582 2022-08-15 08:38:57.000000 littleballoffur-2.2.0/littleballoffur/node_sampling/randomnodesampler.py
--rw-rw-r--   0 benedek   (1000) benedek   (1000)     2654 2022-08-15 08:38:57.000000 littleballoffur-2.2.0/littleballoffur/sampler.py
--rw-rw-r--   0 benedek   (1000) benedek   (1000)       73 2022-08-15 08:40:27.000000 littleballoffur-2.2.0/littleballoffur/version.py
-drwxrwxr-x   0 benedek   (1000) benedek   (1000)        0 2022-08-15 10:35:40.690458 littleballoffur-2.2.0/littleballoffur.egg-info/
--rw-rw-r--   0 benedek   (1000) benedek   (1000)      822 2022-08-15 10:35:40.000000 littleballoffur-2.2.0/littleballoffur.egg-info/PKG-INFO
--rw-rw-r--   0 benedek   (1000) benedek   (1000)     2252 2022-08-15 10:35:40.000000 littleballoffur-2.2.0/littleballoffur.egg-info/SOURCES.txt
--rw-rw-r--   0 benedek   (1000) benedek   (1000)        1 2022-08-15 10:35:40.000000 littleballoffur-2.2.0/littleballoffur.egg-info/dependency_links.txt
--rw-rw-r--   0 benedek   (1000) benedek   (1000)      115 2022-08-15 10:35:40.000000 littleballoffur-2.2.0/littleballoffur.egg-info/requires.txt
--rw-rw-r--   0 benedek   (1000) benedek   (1000)       16 2022-08-15 10:35:40.000000 littleballoffur-2.2.0/littleballoffur.egg-info/top_level.txt
--rw-rw-r--   0 benedek   (1000) benedek   (1000)       38 2022-08-15 10:35:40.694457 littleballoffur-2.2.0/setup.cfg
--rw-rw-r--   0 benedek   (1000) benedek   (1000)     1717 2022-08-15 08:39:37.000000 littleballoffur-2.2.0/setup.py
+drwxr-xr-x   0 benedek    (501) staff       (20)        0 2023-07-01 22:12:06.855942 littleballoffur-2.3.1/
+-rw-r--r--   0 benedek    (501) staff       (20)      822 2023-07-01 22:12:06.855797 littleballoffur-2.3.1/PKG-INFO
+-rw-r--r--   0 benedek    (501) staff       (20)    15936 2023-07-01 21:59:58.000000 littleballoffur-2.3.1/README.md
+drwxr-xr-x   0 benedek    (501) staff       (20)        0 2023-07-01 22:12:06.849833 littleballoffur-2.3.1/littleballoffur/
+-rw-r--r--   0 benedek    (501) staff       (20)      397 2023-07-01 21:59:58.000000 littleballoffur-2.3.1/littleballoffur/__init__.py
+-rw-r--r--   0 benedek    (501) staff       (20)     8559 2023-07-01 21:59:58.000000 littleballoffur-2.3.1/littleballoffur/backend.py
+drwxr-xr-x   0 benedek    (501) staff       (20)        0 2023-07-01 22:12:06.850788 littleballoffur-2.3.1/littleballoffur/dataset/
+-rw-r--r--   0 benedek    (501) staff       (20)       40 2023-07-01 21:59:58.000000 littleballoffur-2.3.1/littleballoffur/dataset/__init__.py
+-rw-r--r--   0 benedek    (501) staff       (20)     1401 2023-07-01 21:59:58.000000 littleballoffur-2.3.1/littleballoffur/dataset/dataset_reader.py
+drwxr-xr-x   0 benedek    (501) staff       (20)        0 2023-07-01 22:12:06.851732 littleballoffur-2.3.1/littleballoffur/edge_sampling/
+-rw-r--r--   0 benedek    (501) staff       (20)      527 2023-07-01 21:59:58.000000 littleballoffur-2.3.1/littleballoffur/edge_sampling/__init__.py
+-rw-r--r--   0 benedek    (501) staff       (20)     2447 2023-07-01 21:59:58.000000 littleballoffur-2.3.1/littleballoffur/edge_sampling/hybridnodeedgesampler.py
+-rw-r--r--   0 benedek    (501) staff       (20)     1582 2023-07-01 21:59:58.000000 littleballoffur-2.3.1/littleballoffur/edge_sampling/randomedgesampler.py
+-rw-r--r--   0 benedek    (501) staff       (20)     1745 2023-07-01 21:59:58.000000 littleballoffur-2.3.1/littleballoffur/edge_sampling/randomedgesamplerwithinduction.py
+-rw-r--r--   0 benedek    (501) staff       (20)     2548 2023-07-01 21:59:58.000000 littleballoffur-2.3.1/littleballoffur/edge_sampling/randomedgesamplerwithpartialinduction.py
+-rw-r--r--   0 benedek    (501) staff       (20)     1955 2023-07-01 21:59:58.000000 littleballoffur-2.3.1/littleballoffur/edge_sampling/randomnodeedgesampler.py
+drwxr-xr-x   0 benedek    (501) staff       (20)        0 2023-07-01 22:12:06.854905 littleballoffur-2.3.1/littleballoffur/exploration_sampling/
+-rw-r--r--   0 benedek    (501) staff       (20)     1854 2023-07-01 21:59:58.000000 littleballoffur-2.3.1/littleballoffur/exploration_sampling/__init__.py
+-rw-r--r--   0 benedek    (501) staff       (20)     2793 2023-07-01 21:59:58.000000 littleballoffur-2.3.1/littleballoffur/exploration_sampling/breadthfirstsearchsampler.py
+-rw-r--r--   0 benedek    (501) staff       (20)     3450 2023-07-01 21:59:58.000000 littleballoffur-2.3.1/littleballoffur/exploration_sampling/circulatedneighborsrandomwalksampler.py
+-rw-r--r--   0 benedek    (501) staff       (20)     3745 2023-07-01 21:59:58.000000 littleballoffur-2.3.1/littleballoffur/exploration_sampling/commonneighborawarerandomwalksampler.py
+-rw-r--r--   0 benedek    (501) staff       (20)     3350 2023-07-01 21:59:58.000000 littleballoffur-2.3.1/littleballoffur/exploration_sampling/communitystructureexpansionsampler.py
+-rw-r--r--   0 benedek    (501) staff       (20)     2968 2023-07-01 21:59:58.000000 littleballoffur-2.3.1/littleballoffur/exploration_sampling/depthfirstsearchsampler.py
+-rw-r--r--   0 benedek    (501) staff       (20)     2629 2023-07-01 21:59:58.000000 littleballoffur-2.3.1/littleballoffur/exploration_sampling/diffusionsampler.py
+-rw-r--r--   0 benedek    (501) staff       (20)     2707 2023-07-01 21:59:58.000000 littleballoffur-2.3.1/littleballoffur/exploration_sampling/diffusiontreesampler.py
+-rw-r--r--   0 benedek    (501) staff       (20)     3917 2023-07-01 21:59:58.000000 littleballoffur-2.3.1/littleballoffur/exploration_sampling/forestfiresampler.py
+-rw-r--r--   0 benedek    (501) staff       (20)     2855 2023-07-01 21:59:58.000000 littleballoffur-2.3.1/littleballoffur/exploration_sampling/frontiersampler.py
+-rw-r--r--   0 benedek    (501) staff       (20)     3052 2023-07-01 21:59:58.000000 littleballoffur-2.3.1/littleballoffur/exploration_sampling/looperasedrandomwalksampler.py
+-rw-r--r--   0 benedek    (501) staff       (20)     3106 2023-07-01 21:59:58.000000 littleballoffur-2.3.1/littleballoffur/exploration_sampling/metropolishastingsrandomwalksampler.py
+-rw-r--r--   0 benedek    (501) staff       (20)     2984 2023-07-01 21:59:58.000000 littleballoffur-2.3.1/littleballoffur/exploration_sampling/nonbacktrackingrandomwalksampler.py
+-rw-r--r--   0 benedek    (501) staff       (20)     1915 2023-07-01 21:59:58.000000 littleballoffur-2.3.1/littleballoffur/exploration_sampling/randomnodeneighborsampler.py
+-rw-r--r--   0 benedek    (501) staff       (20)     2470 2023-07-01 21:59:58.000000 littleballoffur-2.3.1/littleballoffur/exploration_sampling/randomwalksampler.py
+-rw-r--r--   0 benedek    (501) staff       (20)     2941 2023-07-01 21:59:58.000000 littleballoffur-2.3.1/littleballoffur/exploration_sampling/randomwalkwithjumpsampler.py
+-rw-r--r--   0 benedek    (501) staff       (20)     2939 2023-07-01 21:59:58.000000 littleballoffur-2.3.1/littleballoffur/exploration_sampling/randomwalkwithrestartsampler.py
+-rw-r--r--   0 benedek    (501) staff       (20)     2361 2023-07-01 21:59:58.000000 littleballoffur-2.3.1/littleballoffur/exploration_sampling/shortestpathsampler.py
+-rw-r--r--   0 benedek    (501) staff       (20)     3071 2023-07-01 21:59:58.000000 littleballoffur-2.3.1/littleballoffur/exploration_sampling/snowballsampler.py
+-rw-r--r--   0 benedek    (501) staff       (20)     8379 2023-07-01 21:59:58.000000 littleballoffur-2.3.1/littleballoffur/exploration_sampling/spikyballsampler.py
+-rw-r--r--   0 benedek    (501) staff       (20)      211 2023-07-01 21:59:58.000000 littleballoffur-2.3.1/littleballoffur/helpers.py
+drwxr-xr-x   0 benedek    (501) staff       (20)        0 2023-07-01 22:12:06.855538 littleballoffur-2.3.1/littleballoffur/node_sampling/
+-rw-r--r--   0 benedek    (501) staff       (20)      254 2023-07-01 21:59:58.000000 littleballoffur-2.3.1/littleballoffur/node_sampling/__init__.py
+-rw-r--r--   0 benedek    (501) staff       (20)     1933 2023-07-01 21:59:58.000000 littleballoffur-2.3.1/littleballoffur/node_sampling/degreebasedsampler.py
+-rw-r--r--   0 benedek    (501) staff       (20)     1997 2023-07-01 21:59:58.000000 littleballoffur-2.3.1/littleballoffur/node_sampling/pagerankbasedsampler.py
+-rw-r--r--   0 benedek    (501) staff       (20)     1582 2023-07-01 21:59:58.000000 littleballoffur-2.3.1/littleballoffur/node_sampling/randomnodesampler.py
+-rw-r--r--   0 benedek    (501) staff       (20)     2876 2023-07-01 21:59:58.000000 littleballoffur-2.3.1/littleballoffur/sampler.py
+-rw-r--r--   0 benedek    (501) staff       (20)       73 2023-07-01 21:59:58.000000 littleballoffur-2.3.1/littleballoffur/version.py
+drwxr-xr-x   0 benedek    (501) staff       (20)        0 2023-07-01 22:12:06.850483 littleballoffur-2.3.1/littleballoffur.egg-info/
+-rw-r--r--   0 benedek    (501) staff       (20)      822 2023-07-01 22:12:06.000000 littleballoffur-2.3.1/littleballoffur.egg-info/PKG-INFO
+-rw-r--r--   0 benedek    (501) staff       (20)     2252 2023-07-01 22:12:06.000000 littleballoffur-2.3.1/littleballoffur.egg-info/SOURCES.txt
+-rw-r--r--   0 benedek    (501) staff       (20)        1 2023-07-01 22:12:06.000000 littleballoffur-2.3.1/littleballoffur.egg-info/dependency_links.txt
+-rw-r--r--   0 benedek    (501) staff       (20)      137 2023-07-01 22:12:06.000000 littleballoffur-2.3.1/littleballoffur.egg-info/requires.txt
+-rw-r--r--   0 benedek    (501) staff       (20)       16 2023-07-01 22:12:06.000000 littleballoffur-2.3.1/littleballoffur.egg-info/top_level.txt
+-rw-r--r--   0 benedek    (501) staff       (20)       38 2023-07-01 22:12:06.855987 littleballoffur-2.3.1/setup.cfg
+-rw-r--r--   0 benedek    (501) staff       (20)     1602 2023-07-01 22:04:08.000000 littleballoffur-2.3.1/setup.py
```

### Comparing `littleballoffur-2.2.0/PKG-INFO` & `littleballoffur-2.3.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: littleballoffur
-Version: 2.2.0
+Version: 2.3.1
 Summary: A general purpose library for subsampling graphs.
 Home-page: https://github.com/benedekrozemberczki/littleballoffur
 Author: Benedek Rozemberczki
 Author-email: benedek.rozemberczki@gmail.com
 License: MIT
-Download-URL: https://github.com/benedekrozemberczki/littleballoffur/archive/v_2.2.0.tar.gz
+Download-URL: https://github.com/benedekrozemberczki/littleballoffur/archive/v_2.3.1.tar.gz
 Description: UNKNOWN
 Keywords: community,detection,networkx,graph,snow ball,metropolis hastings,shortest path,loop erased,spiky ball,graph sampling,sampling,tree sampling,random walk,forest fire
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `littleballoffur-2.2.0/README.md` & `littleballoffur-2.3.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ![Version](https://badge.fury.io/py/littleballoffur.svg?style=plastic) [![repo size](https://img.shields.io/github/repo-size/benedekrozemberczki/littleballoffur.svg)](https://github.com/benedekrozemberczki/littleballoffur/archive/master.zip) [![Arxiv](https://img.shields.io/badge/ArXiv-2006.04311-orange.svg)](https://arxiv.org/abs/2006.04311) [![build badge](https://github.com/benedekrozemberczki/littleballoffur/workflows/CI/badge.svg)](https://github.com/benedekrozemberczki/littleballoffur/actions?query=workflow%3ACI) [![coverage badge](https://codecov.io/gh/benedekrozemberczki/littleballoffur/branch/master/graph/badge.svg)](https://codecov.io/github/benedekrozemberczki/littleballoffur?branch=master) [![benedekrozemberczki](https://img.shields.io/twitter/follow/benrozemberczki?style=social&logo=twitter)](https://twitter.com/intent/follow?screen_name=benrozemberczki)
 
 <p align="center">
   <img width="90%" src="https://github.com/benedekrozemberczki/littleballoffur/blob/master/littleballoffurlogo.jpg?sanitize=true" />
 </p>
 
-------------------------------------------------------------------------------
+----------------------------------------------------------------------------
 
 **Little Ball of Fur** is a graph sampling extension library for Python.
 
 Please look at the **[Documentation](https://little-ball-of-fur.readthedocs.io/)**, relevant **[Paper](https://arxiv.org/abs/2006.04311)**, **[Promo video](https://youtu.be/5OpjBqlPWME)** and **[External Resources](https://little-ball-of-fur.readthedocs.io/en/latest/notes/resources.html)**.
 
-------------------------------------------------------------------------------
+----------------------------------------------------------------------------
 
 **Little Ball of Fur** consists of methods that can sample from graph structured data. To put it simply it is a Swiss Army knife for graph sampling tasks. First, it includes a large variety of vertex, edge, and exploration sampling techniques. Second, it provides a unified application public interface which makes the application of sampling algorithms trivial for end-users. Implemented methods cover a wide range of networking ([Networking](https://link.springer.com/conference/networking), [INFOCOM](https://infocom2020.ieee-infocom.org/), [SIGCOMM](http://www.sigcomm.org/)) and data mining ([KDD](https://www.kdd.org/kdd2020/), [TKDD](https://dl.acm.org/journal/tkdd), [ICDE](http://www.wikicfp.com/cfp/program?id=1331&s=ICDE&f=International%20Conference%20on%20Data%20Engineering)) conferences, workshops, and pieces from prominent journals. 
 
 ------------------------------------------------------------------------------
 
 **Citing**
```

### Comparing `littleballoffur-2.2.0/littleballoffur/backend.py` & `littleballoffur-2.3.1/littleballoffur/backend.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,102 +1,92 @@
 import random
-import numpy as np
-import networkx as nx
-import networkit as nk
 from typing import List, Tuple
 
+import networkit as nk
+import networkx as nx
+import numpy as np
 
 NKGraph = type(nk.graph.Graph())
 NXGraph = nx.classes.graph.Graph
 
 
 class NetworKitBackEnd(object):
     """
     Binding the NetworKit backend to serve graph operations.
     """
+
     def __init__(self):
         pass
 
     def get_number_of_nodes(self, graph: NKGraph) -> int:
         """
         Given a graph return the number of nodes.
         """
         return graph.numberOfNodes()
 
-
     def get_number_of_edges(self, graph: NKGraph) -> int:
         """
         Given a graph return the number of edges.
         """
         return graph.numberOfEdges()
 
-
     def get_nodes(self, graph: NKGraph) -> List:
         """
         Given a graph return the nodes.
         """
-        return graph.nodes()
-
+        return [node for node in self.get_node_iterator(graph)]
 
     def get_edges(self, graph: NKGraph) -> List[Tuple]:
         """
         Given a graph return the edges.
         """
-        return graph.edges()
-
+        return [edge for edge in self.get_edge_iterator(graph)]
 
     def get_node_iterator(self, graph: NKGraph):
         """
         Given a graph return the node iterator.
         """
         return graph.iterNodes()
 
-
     def get_edge_iterator(self, graph: NKGraph):
         """
         Given a graph return the edge iterator.
         """
         return graph.iterEdges()
 
-
     def get_degree(self, graph: NKGraph, node: int) -> int:
         """
         Given a graph and node return the degree.
         """
         return graph.degree(node)
 
-
     def get_subgraph(self, graph: NKGraph, nodes: List[int]) -> NKGraph:
         """
         Given a graph and set of inducing nodes return a subgraph.
         """
-        return graph.subgraphFromNodes(nodes)
-
+        return nk.graphtools.subgraphFromNodes(graph, nodes)
 
     def get_neighbors(self, graph: NKGraph, node: int) -> List[int]:
         """
         Given a graph and node return the neighbors.
         """
-        return graph.neighbors(node)
-
+        return [node for node in graph.iterNeighbors(node)]
 
     def get_random_neighbor(self, graph: NKGraph, node: int) -> int:
         """
         Given a graph and node returns a random neighbor.
         """
-        return graph.randomNeighbor(node)
-
+        return nk.graphtools.randomNeighbor(graph, node)
 
     def get_shortest_path(self, graph: NKGraph, source: int, target: int) -> List[int]:
         """
         Given a graph, a source and target node pair get the shortes path
         """
         return nk.distance.ReverseBFS(graph, source, True, False, target).run().getPath(target)
 
-
     def get_pagerank(self, graph: NKGraph, alpha: float) -> np.array:
         """
         Given a graph return the PageRank vector.
         """
         pagerank = nk.centrality.PageRank(graph, alpha)
         pagerank.run()
         pagerank = np.array(pagerank.scores())
@@ -114,177 +104,156 @@
         Given an edge list generate a graph.
         """
         new_graph = nk.graph.Graph(directed=False)
         for edge in edges:
             new_graph.addEdge(edge[0], edge[1], addMissing=True)
         return new_graph
 
-
     def _check_networkit_graph(self, graph: NKGraph):
         """Chechking the input type."""
         assert isinstance(graph, NKGraph), "This is not a NetworKit graph."
 
-
     def _check_connectivity(self, graph: NKGraph):
         """Checking the connected nature of a single graph."""
         connected = nk.components.ConnectedComponents(graph).run().numberOfComponents()
         assert connected == 1, "Graph is not connected."
 
-
     def _check_directedness(self, graph: NXGraph):
         """Checking the undirected nature of a single graph."""
         directed = graph.isDirected()
         assert directed == False, "Graph is directed."
 
-
     def _check_indexing(self, graph: NKGraph):
         """Checking the consecutive numeric indexing."""
         numeric_indices = [index for index in range(graph.numberOfNodes())]
-        node_indices = sorted([node for node in graph.nodes()])
+        node_indices = sorted([node for node in self.get_nodes(graph)])
         assert numeric_indices == node_indices, "The node indexing is wrong."
 
-
     def check_graph(self, graph: NKGraph):
         """Check the Little Ball of Fur assumptions about the graph."""
         self._check_networkit_graph(graph)
         self._check_directedness(graph)
         self._check_indexing(graph)
 
 
 class NetworkXBackEnd(object):
     """
     Binding the NetworkX backend to serve graph operations.
     """
+
     def __init__(self):
         pass
 
-
     def get_number_of_nodes(self, graph: NXGraph) -> int:
         """
         Given a graph return the number of nodes.
         """
         return graph.number_of_nodes()
 
-
     def get_number_of_edges(self, graph: NXGraph) -> int:
         """
         Given a graph return the number of edges.
         """
         return graph.number_of_edges()
 
-
     def get_nodes(self, graph: NXGraph) -> List:
         """
         Given a graph return the nodes.
         """
-        return [node for node in graph.nodes()]
-
+        return [node for node in self.get_node_iterator(graph)]
 
     def get_edges(self, graph: NXGraph) -> List[Tuple]:
         """
         Given a graph return the edges.
         """
         return [edge for edge in graph.edges()]
 
-
     def get_node_iterator(self, graph: NXGraph):
         """
         Given a graph return the node iterator.
         """
         return graph.nodes()
 
-
     def get_edge_iterator(self, graph: NXGraph):
         """
         Given a graph return the edge iterator.
         """
         return graph.edges()
 
-
     def get_degree(self, graph: NXGraph, node: int) -> int:
         """
         Given a graph and node return the degree.
         """
         return graph.degree[node]
 
-
     def get_subgraph(self, graph: NXGraph, nodes: List[int]) -> NXGraph:
         """
         Given a graph and set of inducing nodes return a subgraph.
         """
         return graph.subgraph(nodes)
 
-
     def get_neighbors(self, graph: NXGraph, node: int) -> List[int]:
         """
         Given a graph and node return the neighbors.
         """
         return [node for node in graph.neighbors(node)]
 
-
     def get_random_neighbor(self, graph: NXGraph, node: int) -> int:
         """
         Given a graph and node returns a random neighbor.
         """
         neighbors = self.get_neighbors(graph, node)
         return random.choice(neighbors)
 
-
     def get_shortest_path(self, graph: NXGraph, source: int, target: int) -> List[int]:
         """
         Given a graph, a source and target node pair get the shortes path
         """
         return nx.shortest_path(graph, source, target)
 
-
     def get_pagerank(self, graph: NXGraph, alpha: float) -> np.array:
         """
         Given a graph return the PageRank vector.
         """
-        pagerank = nx.pagerank_scipy(graph, alpha=alpha)
+        pagerank = nx.pagerank(graph, alpha=alpha)
         pagerank = np.array([pagerank[node] for node in graph.nodes()])
         pagerank = pagerank / pagerank.sum()
         return pagerank
 
     def is_weighted(self, graph: NXGraph) -> bool:
         return nx.is_weighted(graph)
 
     def get_edge_weight(self, graph: NXGraph, u: int, v: int) -> float:
-        return graph.get_edge_data(u, v)['weight']
+        return graph.get_edge_data(u, v)["weight"]
 
     def graph_from_edgelist(self, edges: List) -> NXGraph:
         """
         Given an edge list generate a graph.
         """
         graph = nx.from_edgelist(edges)
         return graph
 
-
     def _check_networkx_graph(self, graph: NXGraph):
         """Chechking the input type."""
         assert isinstance(graph, NXGraph), "This is not a NetworkX graph."
 
-
     def _check_connectivity(self, graph: NXGraph):
         """Checking the connected nature of a single graph."""
         connected = nx.is_connected(graph)
         assert connected, "Graph is not connected."
 
-
     def _check_directedness(self, graph: NXGraph):
         """Checking the undirected nature of a single graph."""
         directed = nx.is_directed(graph)
         assert directed == False, "Graph is directed."
 
-
     def _check_indexing(self, graph: NXGraph):
         """Checking the consecutive numeric indexing."""
         numeric_indices = [index for index in range(graph.number_of_nodes())]
         node_indices = sorted([node for node in graph.nodes()])
         assert numeric_indices == node_indices, "The node indexing is wrong."
 
-
     def check_graph(self, graph: NXGraph):
         """Check the Little Ball of Fur assumptions about the graph."""
         self._check_networkx_graph(graph)
         self._check_directedness(graph)
-        self._check_indexing(graph)
+        self._check_indexing(graph)
```

### Comparing `littleballoffur-2.2.0/littleballoffur/dataset/dataset_reader.py` & `littleballoffur-2.3.1/littleballoffur/dataset/dataset_reader.py`

 * *Files identical despite different names*

### Comparing `littleballoffur-2.2.0/littleballoffur/edge_sampling/__init__.py` & `littleballoffur-2.3.1/littleballoffur/edge_sampling/__init__.py`

 * *Files identical despite different names*

### Comparing `littleballoffur-2.2.0/littleballoffur/edge_sampling/hybridnodeedgesampler.py` & `littleballoffur-2.3.1/littleballoffur/edge_sampling/hybridnodeedgesampler.py`

 * *Files identical despite different names*

### Comparing `littleballoffur-2.2.0/littleballoffur/edge_sampling/randomedgesampler.py` & `littleballoffur-2.3.1/littleballoffur/edge_sampling/randomedgesampler.py`

 * *Files identical despite different names*

### Comparing `littleballoffur-2.2.0/littleballoffur/edge_sampling/randomedgesamplerwithinduction.py` & `littleballoffur-2.3.1/littleballoffur/edge_sampling/randomedgesamplerwithinduction.py`

 * *Files identical despite different names*

### Comparing `littleballoffur-2.2.0/littleballoffur/edge_sampling/randomedgesamplerwithpartialinduction.py` & `littleballoffur-2.3.1/littleballoffur/edge_sampling/randomedgesamplerwithpartialinduction.py`

 * *Files identical despite different names*

### Comparing `littleballoffur-2.2.0/littleballoffur/edge_sampling/randomnodeedgesampler.py` & `littleballoffur-2.3.1/littleballoffur/edge_sampling/randomnodeedgesampler.py`

 * *Files identical despite different names*

### Comparing `littleballoffur-2.2.0/littleballoffur/exploration_sampling/__init__.py` & `littleballoffur-2.3.1/littleballoffur/exploration_sampling/__init__.py`

 * *Files identical despite different names*

### Comparing `littleballoffur-2.2.0/littleballoffur/exploration_sampling/breadthfirstsearchsampler.py` & `littleballoffur-2.3.1/littleballoffur/exploration_sampling/breadthfirstsearchsampler.py`

 * *Files identical despite different names*

### Comparing `littleballoffur-2.2.0/littleballoffur/exploration_sampling/circulatedneighborsrandomwalksampler.py` & `littleballoffur-2.3.1/littleballoffur/exploration_sampling/circulatedneighborsrandomwalksampler.py`

 * *Files identical despite different names*

### Comparing `littleballoffur-2.2.0/littleballoffur/exploration_sampling/commonneighborawarerandomwalksampler.py` & `littleballoffur-2.3.1/littleballoffur/exploration_sampling/commonneighborawarerandomwalksampler.py`

 * *Files identical despite different names*

### Comparing `littleballoffur-2.2.0/littleballoffur/exploration_sampling/communitystructureexpansionsampler.py` & `littleballoffur-2.3.1/littleballoffur/exploration_sampling/communitystructureexpansionsampler.py`

 * *Files identical despite different names*

### Comparing `littleballoffur-2.2.0/littleballoffur/exploration_sampling/depthfirstsearchsampler.py` & `littleballoffur-2.3.1/littleballoffur/exploration_sampling/depthfirstsearchsampler.py`

 * *Files identical despite different names*

### Comparing `littleballoffur-2.2.0/littleballoffur/exploration_sampling/diffusionsampler.py` & `littleballoffur-2.3.1/littleballoffur/exploration_sampling/diffusionsampler.py`

 * *Files identical despite different names*

### Comparing `littleballoffur-2.2.0/littleballoffur/exploration_sampling/diffusiontreesampler.py` & `littleballoffur-2.3.1/littleballoffur/exploration_sampling/diffusiontreesampler.py`

 * *Files identical despite different names*

### Comparing `littleballoffur-2.2.0/littleballoffur/exploration_sampling/forestfiresampler.py` & `littleballoffur-2.3.1/littleballoffur/exploration_sampling/forestfiresampler.py`

 * *Files identical despite different names*

### Comparing `littleballoffur-2.2.0/littleballoffur/exploration_sampling/frontiersampler.py` & `littleballoffur-2.3.1/littleballoffur/exploration_sampling/frontiersampler.py`

 * *Files identical despite different names*

### Comparing `littleballoffur-2.2.0/littleballoffur/exploration_sampling/looperasedrandomwalksampler.py` & `littleballoffur-2.3.1/littleballoffur/exploration_sampling/looperasedrandomwalksampler.py`

 * *Files identical despite different names*

### Comparing `littleballoffur-2.2.0/littleballoffur/exploration_sampling/metropolishastingsrandomwalksampler.py` & `littleballoffur-2.3.1/littleballoffur/exploration_sampling/metropolishastingsrandomwalksampler.py`

 * *Files identical despite different names*

### Comparing `littleballoffur-2.2.0/littleballoffur/exploration_sampling/nonbacktrackingrandomwalksampler.py` & `littleballoffur-2.3.1/littleballoffur/exploration_sampling/nonbacktrackingrandomwalksampler.py`

 * *Files identical despite different names*

### Comparing `littleballoffur-2.2.0/littleballoffur/exploration_sampling/randomnodeneighborsampler.py` & `littleballoffur-2.3.1/littleballoffur/exploration_sampling/randomnodeneighborsampler.py`

 * *Files identical despite different names*

### Comparing `littleballoffur-2.2.0/littleballoffur/exploration_sampling/randomwalksampler.py` & `littleballoffur-2.3.1/littleballoffur/exploration_sampling/randomwalksampler.py`

 * *Files identical despite different names*

### Comparing `littleballoffur-2.2.0/littleballoffur/exploration_sampling/randomwalkwithjumpsampler.py` & `littleballoffur-2.3.1/littleballoffur/exploration_sampling/randomwalkwithjumpsampler.py`

 * *Files identical despite different names*

### Comparing `littleballoffur-2.2.0/littleballoffur/exploration_sampling/randomwalkwithrestartsampler.py` & `littleballoffur-2.3.1/littleballoffur/exploration_sampling/randomwalkwithrestartsampler.py`

 * *Files identical despite different names*

### Comparing `littleballoffur-2.2.0/littleballoffur/exploration_sampling/shortestpathsampler.py` & `littleballoffur-2.3.1/littleballoffur/exploration_sampling/shortestpathsampler.py`

 * *Files identical despite different names*

### Comparing `littleballoffur-2.2.0/littleballoffur/exploration_sampling/snowballsampler.py` & `littleballoffur-2.3.1/littleballoffur/exploration_sampling/snowballsampler.py`

 * *Files identical despite different names*

### Comparing `littleballoffur-2.2.0/littleballoffur/exploration_sampling/spikyballsampler.py` & `littleballoffur-2.3.1/littleballoffur/exploration_sampling/spikyballsampler.py`

 * *Files identical despite different names*

### Comparing `littleballoffur-2.2.0/littleballoffur/node_sampling/degreebasedsampler.py` & `littleballoffur-2.3.1/littleballoffur/node_sampling/degreebasedsampler.py`

 * *Files identical despite different names*

### Comparing `littleballoffur-2.2.0/littleballoffur/node_sampling/pagerankbasedsampler.py` & `littleballoffur-2.3.1/littleballoffur/node_sampling/pagerankbasedsampler.py`

 * *Files identical despite different names*

### Comparing `littleballoffur-2.2.0/littleballoffur/node_sampling/randomnodesampler.py` & `littleballoffur-2.3.1/littleballoffur/node_sampling/randomnodesampler.py`

 * *Files identical despite different names*

### Comparing `littleballoffur-2.2.0/littleballoffur/sampler.py` & `littleballoffur-2.3.1/littleballoffur/sampler.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import random
-import numpy as np
-import networkx as nx
-import networkit as nk
 from typing import Union
-from littleballoffur.backend import NetworKitBackEnd
-from littleballoffur.backend import NetworkXBackEnd
 
+import networkit as nk
+import networkx as nx
+import numpy as np
+
+from littleballoffur.backend import NetworKitBackEnd, NetworkXBackEnd
 
 NKGraph = type(nk.graph.Graph())
 NXGraph = nx.classes.graph.Graph
 
 
 class Sampler(object):
     """Sampler base class with constructor and private methods."""
 
     def __init__(self):
-        """Creatinng a sampler."""
+        """Creating a sampler."""
         pass
 
     def sample(self):
         """Sample from a model."""
         pass
 
     def _set_seed(self):
@@ -36,41 +36,40 @@
             self.backend = NetworkXBackEnd()
             self.backend.check_graph(graph)
         else:
             raise ValueError("Not a NetworKit or NetworkX graph.")
 
     def _check_networkx_graph(self, graph):
         """Chechking the input type."""
-        assert isinstance(
-            graph, nx.classes.graph.Graph
-        ), "This is not a NetworkX graph."
+        assert isinstance(graph, nx.classes.graph.Graph), "This is not a NetworkX graph."
 
     def _check_directedness(self, graph):
         """Checking the undirected nature of a single graph."""
         directed = nx.is_directed(graph)
-        assert directed == False, "Graph is directed."
+        assert directed is False, "Graph is directed."
 
     def _check_indexing(self, graph):
         """Checking the consecutive numeric indexing."""
         numeric_indices = [index for index in range(graph.number_of_nodes())]
-        node_indices = sorted([node for node in graph.nodes()])
+        if hasattr(self, "backend") and isinstance(self.backend, NetworKitBackEnd):
+            node_indices = sorted([node for node in self.backend.get_nodes(graph)])
+        elif hasattr(self, "backend") and isinstance(self.backend, NetworkXBackEnd):
+            node_indices = sorted([node for node in graph.nodes()])
+        else:
+            node_indices = sorted([node for node in graph.nodes()])
         assert numeric_indices == node_indices, "The node indexing is wrong."
 
     def _check_graph(self, graph: nx.classes.graph.Graph):
         """Check the Little Ball of Fur assumptions about the graph."""
         self._check_networkx_graph(graph)
         self._check_directedness(graph)
         self._check_indexing(graph)
 
     def _check_number_of_nodes(self, graph):
         """Checking the size of the graph - nodes."""
         if self.number_of_nodes > self.backend.get_number_of_nodes(graph):
-            raise ValueError(
-                "The number of nodes is too large. Please see requirements."
-            )
+            raise ValueError("The number of nodes is too large. Please see requirements.")
 
     def _check_number_of_edges(self, graph):
         """Checking the size of the graph -- edges."""
         if self.number_of_edges > self.backend.get_number_of_edges(graph):
-            raise ValueError(
-                "The number of edges is too large. Please see requirements."
-            )
+            raise ValueError("The number of edges is too large. Please see requirements.")
```

### Comparing `littleballoffur-2.2.0/littleballoffur.egg-info/PKG-INFO` & `littleballoffur-2.3.1/littleballoffur.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: littleballoffur
-Version: 2.2.0
+Version: 2.3.1
 Summary: A general purpose library for subsampling graphs.
 Home-page: https://github.com/benedekrozemberczki/littleballoffur
 Author: Benedek Rozemberczki
 Author-email: benedek.rozemberczki@gmail.com
 License: MIT
-Download-URL: https://github.com/benedekrozemberczki/littleballoffur/archive/v_2.2.0.tar.gz
+Download-URL: https://github.com/benedekrozemberczki/littleballoffur/archive/v_2.3.1.tar.gz
 Description: UNKNOWN
 Keywords: community,detection,networkx,graph,snow ball,metropolis hastings,shortest path,loop erased,spiky ball,graph sampling,sampling,tree sampling,random walk,forest fire
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `littleballoffur-2.2.0/littleballoffur.egg-info/SOURCES.txt` & `littleballoffur-2.3.1/littleballoffur.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `littleballoffur-2.2.0/setup.py` & `littleballoffur-2.3.1/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 import os
+
 from setuptools import find_packages, setup
 
 on_rtd = os.environ.get("READTHEDOCS") == "True"
 
-install_requires = ["numpy<1.23.0",
-                    "networkx<2.7",
-                    "decorator==4.4.2",
-                    "cmake",
-                    "Cython",
-                    "tqdm",
-                    "python-louvain",
-                    "pandas<=1.3.5",
-                    "six",
-                    "scipy"]
+install_requires = [
+    "cmake>=3.26",
+    "Cython>=0.29",
+    "decorator>=5.1",
+    "networkx>=3.1",
+    "numpy>=1.21",
+    "pandas<2.0",
+    "python-louvain>=0.16",
+    "six",
+    "scipy>=1.10.0",
+    "tqdm",
+]
 
 if not on_rtd:
-    install_requires.append("networkit==7.1")
+    install_requires.append("networkit>=10.1")
 
 setup_requires = ["cython", "numpy", "pytest-runner"]
 
 tests_require = ["pytest", "pytest-cov", "mock", "unittest"]
 
 
-
 keywords = [
     "community",
     "detection",
     "networkx",
     "graph",
     "snow ball",
     "metropolis hastings",
@@ -38,21 +40,21 @@
     "tree sampling",
     "random walk",
     "forest fire",
 ]
 
 setup(
     name="littleballoffur",
-    version="2.2.0",
+    version="2.3.1",
     license="MIT",
     description="A general purpose library for subsampling graphs.",
     author="Benedek Rozemberczki",
     author_email="benedek.rozemberczki@gmail.com",
     url="https://github.com/benedekrozemberczki/littleballoffur",
-    download_url="https://github.com/benedekrozemberczki/littleballoffur/archive/v_2.2.0.tar.gz",
+    download_url="https://github.com/benedekrozemberczki/littleballoffur/archive/v_2.3.1.tar.gz",
     keywords=keywords,
     install_requires=install_requires,
     setup_requires=setup_requires,
     tests_require=tests_require,
     packages=find_packages(),
     classifiers=[
         "Development Status :: 3 - Alpha",
```

