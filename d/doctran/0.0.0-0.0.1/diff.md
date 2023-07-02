# Comparing `tmp/doctran-0.0.0.tar.gz` & `tmp/doctran-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "doctran-0.0.0.tar", max compression
+gzip compressed data, was "doctran-0.0.1.tar", max compression
```

## Comparing `doctran-0.0.0.tar` & `doctran-0.0.1.tar`

### file list

```diff
@@ -1,6 +1,8 @@
--rw-r--r--   0        0        0     1064 2023-06-24 22:31:03.176553 doctran-0.0.0/LICENSE
--rw-r--r--   0        0        0        9 2023-06-24 22:31:03.176634 doctran-0.0.0/README.md
--rw-r--r--   0        0        0       28 2023-06-24 22:33:28.239525 doctran-0.0.0/doctran/__init__.py
--rw-r--r--   0        0        0     1636 2023-06-24 22:35:52.976860 doctran-0.0.0/doctran/doctran.py
--rw-r--r--   0        0        0      461 2023-06-24 22:38:08.862675 doctran-0.0.0/pyproject.toml
--rw-r--r--   0        0        0      599 1970-01-01 00:00:00.000000 doctran-0.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-06-24 22:31:03.176553 doctran-0.0.1/LICENSE
+-rw-r--r--   0        0        0     4562 2023-07-02 14:08:09.069031 doctran-0.0.1/README.md
+-rw-r--r--   0        0        0      117 2023-07-02 00:38:58.942692 doctran-0.0.1/doctran/__init__.py
+-rw-r--r--   0        0        0     7533 2023-07-02 02:13:13.276556 doctran-0.0.1/doctran/doctran.py
+-rw-r--r--   0        0        0      175 2023-07-01 18:30:41.396740 doctran-0.0.1/doctran/transformers/__init__.py
+-rw-r--r--   0        0        0    12122 2023-07-02 01:43:59.344967 doctran-0.0.1/doctran/transformers/transformers.py
+-rw-r--r--   0        0        0      684 2023-07-02 15:08:24.397662 doctran-0.0.1/pyproject.toml
+-rw-r--r--   0        0        0     5464 1970-01-01 00:00:00.000000 doctran-0.0.1/PKG-INFO
```

### Comparing `doctran-0.0.0/LICENSE` & `doctran-0.0.1/LICENSE`

 * *Files identical despite different names*

