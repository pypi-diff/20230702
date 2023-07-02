# Comparing `tmp/refiner-0.0.1.tar.gz` & `tmp/refiner-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "refiner-0.0.1.tar", last modified: Sun Jul  2 06:38:31 2023, max compression
+gzip compressed data, was "refiner-0.0.2.tar", last modified: Sun Jul  2 08:00:57 2023, max compression
```

## Comparing `refiner-0.0.1.tar` & `refiner-0.0.2.tar`

### file list

```diff
@@ -1,22 +1,20 @@
-drwxr-xr-x   0 adaro      (501) staff       (20)        0 2023-07-02 06:38:31.425717 refiner-0.0.1/
--rw-r--r--   0 adaro      (501) staff       (20)     1066 2023-04-22 07:38:04.000000 refiner-0.0.1/LICENSE
--rw-r--r--   0 adaro      (501) staff       (20)     1563 2023-07-02 06:38:31.425337 refiner-0.0.1/PKG-INFO
--rw-r--r--   0 adaro      (501) staff       (20)     1063 2023-06-20 08:46:58.000000 refiner-0.0.1/README.md
--rw-r--r--   0 adaro      (501) staff       (20)      643 2023-07-02 06:36:21.000000 refiner-0.0.1/pyproject.toml
--rw-r--r--   0 adaro      (501) staff       (20)       38 2023-07-02 06:38:31.425831 refiner-0.0.1/setup.cfg
-drwxr-xr-x   0 adaro      (501) staff       (20)        0 2023-07-02 06:38:31.417247 refiner-0.0.1/src/
-drwxr-xr-x   0 adaro      (501) staff       (20)        0 2023-07-02 06:38:31.419180 refiner-0.0.1/src/bin/
--rw-r--r--   0 adaro      (501) staff       (20)     2630 2023-07-02 06:30:11.000000 refiner-0.0.1/src/bin/cli.py
-drwxr-xr-x   0 adaro      (501) staff       (20)        0 2023-07-02 06:38:31.420145 refiner-0.0.1/src/refiner/
--rw-r--r--   0 adaro      (501) staff       (20)        0 2023-04-28 14:32:48.000000 refiner-0.0.1/src/refiner/__init__.py
--rw-r--r--   0 adaro      (501) staff       (20)     5197 2023-06-20 10:25:14.000000 refiner-0.0.1/src/refiner/embeddings.py
-drwxr-xr-x   0 adaro      (501) staff       (20)        0 2023-07-02 06:38:31.424393 refiner-0.0.1/src/refiner/integrations/
--rw-r--r--   0 adaro      (501) staff       (20)       86 2023-06-09 07:17:42.000000 refiner-0.0.1/src/refiner/integrations/__init__.py
--rw-r--r--   0 adaro      (501) staff       (20)      356 2023-06-09 09:24:33.000000 refiner-0.0.1/src/refiner/integrations/refiner_openai.py
--rw-r--r--   0 adaro      (501) staff       (20)     2668 2023-06-20 10:06:14.000000 refiner-0.0.1/src/refiner/integrations/refiner_pinecone.py
-drwxr-xr-x   0 adaro      (501) staff       (20)        0 2023-07-02 06:38:31.422530 refiner-0.0.1/src/refiner.egg-info/
--rw-r--r--   0 adaro      (501) staff       (20)     1563 2023-07-02 06:38:31.000000 refiner-0.0.1/src/refiner.egg-info/PKG-INFO
--rw-r--r--   0 adaro      (501) staff       (20)      396 2023-07-02 06:38:31.000000 refiner-0.0.1/src/refiner.egg-info/SOURCES.txt
--rw-r--r--   0 adaro      (501) staff       (20)        1 2023-07-02 06:38:31.000000 refiner-0.0.1/src/refiner.egg-info/dependency_links.txt
--rw-r--r--   0 adaro      (501) staff       (20)       87 2023-07-02 06:38:31.000000 refiner-0.0.1/src/refiner.egg-info/requires.txt
--rw-r--r--   0 adaro      (501) staff       (20)       12 2023-07-02 06:38:31.000000 refiner-0.0.1/src/refiner.egg-info/top_level.txt
+drwxr-xr-x   0 adaro      (501) staff       (20)        0 2023-07-02 08:00:57.002089 refiner-0.0.2/
+-rw-r--r--   0 adaro      (501) staff       (20)     1066 2023-04-22 07:38:04.000000 refiner-0.0.2/LICENSE
+-rw-r--r--   0 adaro      (501) staff       (20)     1881 2023-07-02 08:00:57.001794 refiner-0.0.2/PKG-INFO
+-rw-r--r--   0 adaro      (501) staff       (20)     1272 2023-07-02 07:49:51.000000 refiner-0.0.2/README.md
+-rw-r--r--   0 adaro      (501) staff       (20)      752 2023-07-02 07:59:44.000000 refiner-0.0.2/pyproject.toml
+-rw-r--r--   0 adaro      (501) staff       (20)       38 2023-07-02 08:00:57.002174 refiner-0.0.2/setup.cfg
+drwxr-xr-x   0 adaro      (501) staff       (20)        0 2023-07-02 08:00:56.995429 refiner-0.0.2/src/
+drwxr-xr-x   0 adaro      (501) staff       (20)        0 2023-07-02 08:00:56.997432 refiner-0.0.2/src/refiner/
+-rw-r--r--   0 adaro      (501) staff       (20)        0 2023-04-28 14:32:48.000000 refiner-0.0.2/src/refiner/__init__.py
+-rw-r--r--   0 adaro      (501) staff       (20)     5197 2023-06-20 10:25:14.000000 refiner-0.0.2/src/refiner/embeddings.py
+drwxr-xr-x   0 adaro      (501) staff       (20)        0 2023-07-02 08:00:57.001102 refiner-0.0.2/src/refiner/integrations/
+-rw-r--r--   0 adaro      (501) staff       (20)       86 2023-06-09 07:17:42.000000 refiner-0.0.2/src/refiner/integrations/__init__.py
+-rw-r--r--   0 adaro      (501) staff       (20)      356 2023-06-09 09:24:33.000000 refiner-0.0.2/src/refiner/integrations/refiner_openai.py
+-rw-r--r--   0 adaro      (501) staff       (20)     2668 2023-06-20 10:06:14.000000 refiner-0.0.2/src/refiner/integrations/refiner_pinecone.py
+drwxr-xr-x   0 adaro      (501) staff       (20)        0 2023-07-02 08:00:56.999348 refiner-0.0.2/src/refiner.egg-info/
+-rw-r--r--   0 adaro      (501) staff       (20)     1881 2023-07-02 08:00:56.000000 refiner-0.0.2/src/refiner.egg-info/PKG-INFO
+-rw-r--r--   0 adaro      (501) staff       (20)      381 2023-07-02 08:00:56.000000 refiner-0.0.2/src/refiner.egg-info/SOURCES.txt
+-rw-r--r--   0 adaro      (501) staff       (20)        1 2023-07-02 08:00:56.000000 refiner-0.0.2/src/refiner.egg-info/dependency_links.txt
+-rw-r--r--   0 adaro      (501) staff       (20)       87 2023-07-02 08:00:56.000000 refiner-0.0.2/src/refiner.egg-info/requires.txt
+-rw-r--r--   0 adaro      (501) staff       (20)        8 2023-07-02 08:00:56.000000 refiner-0.0.2/src/refiner.egg-info/top_level.txt
```

### Comparing `refiner-0.0.1/LICENSE` & `refiner-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `refiner-0.0.1/src/refiner/embeddings.py` & `refiner-0.0.2/src/refiner/embeddings.py`

 * *Files identical despite different names*

### Comparing `refiner-0.0.1/src/refiner/integrations/refiner_pinecone.py` & `refiner-0.0.2/src/refiner/integrations/refiner_pinecone.py`

 * *Files identical despite different names*

