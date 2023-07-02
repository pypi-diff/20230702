# Comparing `tmp/ccxtools-0.0.8.tar.gz` & `tmp/ccxtools-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ccxtools-0.0.8.tar", last modified: Tue Apr  5 19:23:54 2022, max compression
+gzip compressed data, was "ccxtools-0.0.9.tar", last modified: Sun Apr 10 12:52:35 2022, max compression
```

## Comparing `ccxtools-0.0.8.tar` & `ccxtools-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2022-04-05 19:23:54.962050 ccxtools-0.0.8/
--rw-rw-rw-   0        0        0      346 2022-04-05 19:23:54.962050 ccxtools-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0       10 2022-04-05 10:27:10.000000 ccxtools-0.0.8/README.md
--rw-rw-rw-   0        0        0       86 2022-04-05 10:00:45.000000 ccxtools-0.0.8/pyproject.toml
--rw-rw-rw-   0        0        0      512 2022-04-05 19:23:54.966049 ccxtools-0.0.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2022-04-05 19:23:54.933045 ccxtools-0.0.8/src/
-drwxrwxrwx   0        0        0        0 2022-04-05 19:23:54.943045 ccxtools-0.0.8/src/ccxtools/
--rw-rw-rw-   0        0        0        0 2022-04-05 18:32:32.000000 ccxtools-0.0.8/src/ccxtools/__init__.py
--rw-rw-rw-   0        0        0      736 2022-04-05 19:23:38.000000 ccxtools-0.0.8/src/ccxtools/bybit.py
--rw-rw-rw-   0        0        0       75 2022-04-05 19:09:47.000000 ccxtools-0.0.8/src/ccxtools/exchange.py
-drwxrwxrwx   0        0        0        0 2022-04-05 19:23:54.960049 ccxtools-0.0.8/src/ccxtools.egg-info/
--rw-rw-rw-   0        0        0      346 2022-04-05 19:23:54.000000 ccxtools-0.0.8/src/ccxtools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      285 2022-04-05 19:23:54.000000 ccxtools-0.0.8/src/ccxtools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-04-05 19:23:54.000000 ccxtools-0.0.8/src/ccxtools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2022-04-05 19:23:54.000000 ccxtools-0.0.8/src/ccxtools.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2022-04-05 19:23:54.000000 ccxtools-0.0.8/src/ccxtools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2022-04-10 12:52:35.806562 ccxtools-0.0.9/
+-rw-rw-rw-   0        0        0      346 2022-04-10 12:52:35.806562 ccxtools-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0       10 2022-04-05 10:27:10.000000 ccxtools-0.0.9/README.md
+-rw-rw-rw-   0        0        0       86 2022-04-05 10:00:45.000000 ccxtools-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0      512 2022-04-10 12:52:35.809564 ccxtools-0.0.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2022-04-10 12:52:35.778772 ccxtools-0.0.9/src/
+drwxrwxrwx   0        0        0        0 2022-04-10 12:52:35.791959 ccxtools-0.0.9/src/ccxtools/
+-rw-rw-rw-   0        0        0        0 2022-04-06 23:10:34.000000 ccxtools-0.0.9/src/ccxtools/__init__.py
+-rw-rw-rw-   0        0        0     1346 2022-04-07 13:50:16.000000 ccxtools-0.0.9/src/ccxtools/bybit.py
+-rw-rw-rw-   0        0        0      183 2022-04-07 06:56:49.000000 ccxtools-0.0.9/src/ccxtools/exchange.py
+drwxrwxrwx   0        0        0        0 2022-04-10 12:52:35.804949 ccxtools-0.0.9/src/ccxtools.egg-info/
+-rw-rw-rw-   0        0        0      346 2022-04-10 12:52:35.000000 ccxtools-0.0.9/src/ccxtools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      285 2022-04-10 12:52:35.000000 ccxtools-0.0.9/src/ccxtools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-04-10 12:52:35.000000 ccxtools-0.0.9/src/ccxtools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2022-04-10 12:52:35.000000 ccxtools-0.0.9/src/ccxtools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2022-04-10 12:52:35.000000 ccxtools-0.0.9/src/ccxtools.egg-info/top_level.txt
```

### Comparing `ccxtools-0.0.8/setup.cfg` & `ccxtools-0.0.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2063 6378 746f 6f6c 730d 0a76 6572   = ccxtools..ver
-00000020: 7369 6f6e 203d 2030 2e30 2e38 0d0a 6175  sion = 0.0.8..au
+00000020: 7369 6f6e 203d 2030 2e30 2e39 0d0a 6175  sion = 0.0.9..au
 00000030: 7468 6f72 203d 2057 6f6f 7375 6220 4c65  thor = Woosub Le
 00000040: 650d 0a61 7574 686f 725f 656d 6169 6c20  e..author_email 
 00000050: 3d20 7a62 7876 3134 3233 406e 6176 6572  = zbxv1423@naver
 00000060: 2e63 6f6d 0d0a 6465 7363 7269 7074 696f  .com..descriptio
 00000070: 6e20 3d20 6363 7874 6f6f 6c73 0d0a 6c6f  n = ccxtools..lo
 00000080: 6e67 5f64 6573 6372 6970 7469 6f6e 203d  ng_description =
 00000090: 2066 696c 653a 2052 4541 444d 452e 6d64   file: README.md
```

