# Comparing `tmp/konko-0.0.5.tar.gz` & `tmp/konko-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "konko-0.0.5.tar", last modified: Fri Jun  2 19:24:50 2023, max compression
+gzip compressed data, was "konko-0.0.6.tar", last modified: Sun Jul  2 20:00:17 2023, max compression
```

## Comparing `konko-0.0.5.tar` & `konko-0.0.6.tar`

### file list

```diff
@@ -1,16 +1,19 @@
-drwxr-xr-x   0 uday.kanwar   (501) staff       (20)        0 2023-06-02 19:24:50.677626 konko-0.0.5/
--rw-r--r--   0 uday.kanwar   (501) staff       (20)      254 2023-06-02 19:24:50.677496 konko-0.0.5/PKG-INFO
--rw-r--r--   0 uday.kanwar   (501) staff       (20)       29 2023-06-01 17:28:19.000000 konko-0.0.5/README.md
--rw-r--r--   0 uday.kanwar   (501) staff       (20)      304 2023-06-02 19:24:28.000000 konko-0.0.5/pyproject.toml
--rw-r--r--   0 uday.kanwar   (501) staff       (20)       38 2023-06-02 19:24:50.677665 konko-0.0.5/setup.cfg
-drwxr-xr-x   0 uday.kanwar   (501) staff       (20)        0 2023-06-02 19:24:50.675743 konko-0.0.5/src/
-drwxr-xr-x   0 uday.kanwar   (501) staff       (20)        0 2023-06-02 19:24:50.676721 konko-0.0.5/src/konko/
--rw-r--r--   0 uday.kanwar   (501) staff       (20)      123 2023-06-02 19:23:49.000000 konko-0.0.5/src/konko/__init__.py
--rw-r--r--   0 uday.kanwar   (501) staff       (20)      470 2023-06-02 18:45:34.000000 konko-0.0.5/src/konko/evaluate.py
--rw-r--r--   0 uday.kanwar   (501) staff       (20)      600 2023-06-02 19:03:42.000000 konko-0.0.5/src/konko/generate.py
--rw-r--r--   0 uday.kanwar   (501) staff       (20)      213 2023-06-02 18:51:00.000000 konko-0.0.5/src/konko/models.py
-drwxr-xr-x   0 uday.kanwar   (501) staff       (20)        0 2023-06-02 19:24:50.677334 konko-0.0.5/src/konko.egg-info/
--rw-r--r--   0 uday.kanwar   (501) staff       (20)      254 2023-06-02 19:24:50.000000 konko-0.0.5/src/konko.egg-info/PKG-INFO
--rw-r--r--   0 uday.kanwar   (501) staff       (20)      242 2023-06-02 19:24:50.000000 konko-0.0.5/src/konko.egg-info/SOURCES.txt
--rw-r--r--   0 uday.kanwar   (501) staff       (20)        1 2023-06-02 19:24:50.000000 konko-0.0.5/src/konko.egg-info/dependency_links.txt
--rw-r--r--   0 uday.kanwar   (501) staff       (20)        6 2023-06-02 19:24:50.000000 konko-0.0.5/src/konko.egg-info/top_level.txt
+drwxr-xr-x   0 uday.kanwar   (501) staff       (20)        0 2023-07-02 20:00:17.760256 konko-0.0.6/
+-rw-r--r--   0 uday.kanwar   (501) staff       (20)      254 2023-07-02 20:00:17.760125 konko-0.0.6/PKG-INFO
+-rw-r--r--   0 uday.kanwar   (501) staff       (20)       29 2023-06-01 17:28:19.000000 konko-0.0.6/README.md
+-rw-r--r--   0 uday.kanwar   (501) staff       (20)      304 2023-07-02 19:59:48.000000 konko-0.0.6/pyproject.toml
+-rw-r--r--   0 uday.kanwar   (501) staff       (20)       38 2023-07-02 20:00:17.760303 konko-0.0.6/setup.cfg
+drwxr-xr-x   0 uday.kanwar   (501) staff       (20)        0 2023-07-02 20:00:17.758551 konko-0.0.6/src/
+drwxr-xr-x   0 uday.kanwar   (501) staff       (20)        0 2023-07-02 20:00:17.759288 konko-0.0.6/src/konko/
+-rw-r--r--   0 uday.kanwar   (501) staff       (20)      119 2023-07-01 02:14:31.000000 konko-0.0.6/src/konko/__init__.py
+-rw-r--r--   0 uday.kanwar   (501) staff       (20)     1887 2023-06-15 22:41:35.000000 konko-0.0.6/src/konko/evaluate.py
+-rw-r--r--   0 uday.kanwar   (501) staff       (20)     4296 2023-07-01 02:13:25.000000 konko-0.0.6/src/konko/generate.py
+-rw-r--r--   0 uday.kanwar   (501) staff       (20)     1277 2023-07-01 02:14:39.000000 konko-0.0.6/src/konko/models.py
+drwxr-xr-x   0 uday.kanwar   (501) staff       (20)        0 2023-07-02 20:00:17.759971 konko-0.0.6/src/konko/utils/
+-rw-r--r--   0 uday.kanwar   (501) staff       (20)       41 2023-06-30 21:50:53.000000 konko-0.0.6/src/konko/utils/constants.py
+-rw-r--r--   0 uday.kanwar   (501) staff       (20)      209 2023-06-30 22:20:34.000000 konko-0.0.6/src/konko/utils/utils.py
+drwxr-xr-x   0 uday.kanwar   (501) staff       (20)        0 2023-07-02 20:00:17.759758 konko-0.0.6/src/konko.egg-info/
+-rw-r--r--   0 uday.kanwar   (501) staff       (20)      254 2023-07-02 20:00:17.000000 konko-0.0.6/src/konko.egg-info/PKG-INFO
+-rw-r--r--   0 uday.kanwar   (501) staff       (20)      296 2023-07-02 20:00:17.000000 konko-0.0.6/src/konko.egg-info/SOURCES.txt
+-rw-r--r--   0 uday.kanwar   (501) staff       (20)        1 2023-07-02 20:00:17.000000 konko-0.0.6/src/konko.egg-info/dependency_links.txt
+-rw-r--r--   0 uday.kanwar   (501) staff       (20)        6 2023-07-02 20:00:17.000000 konko-0.0.6/src/konko.egg-info/top_level.txt
```

