# Comparing `tmp/veloadmin-1.0.1.tar.gz` & `tmp/veloadmin-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "veloadmin-1.0.1.tar", last modified: Sun Jul  2 13:33:18 2023, max compression
+gzip compressed data, was "veloadmin-1.0.2.tar", last modified: Sun Jul  2 15:05:42 2023, max compression
```

## Comparing `veloadmin-1.0.1.tar` & `veloadmin-1.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-02 13:33:18.636734 veloadmin-1.0.1/
--rw-rw-rw-   0        0        0      169 2023-07-02 13:33:18.628731 veloadmin-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-02 13:33:18.636734 veloadmin-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      466 2023-07-02 13:25:26.000000 veloadmin-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-02 13:33:18.564056 veloadmin-1.0.1/veloAdmin/
--rw-rw-rw-   0        0        0        0 2023-07-02 13:22:37.000000 veloadmin-1.0.1/veloAdmin/__init__.py
--rw-rw-rw-   0        0        0     4698 2023-07-02 13:31:49.000000 veloadmin-1.0.1/veloAdmin/create.py
-drwxrwxrwx   0        0        0        0 2023-07-02 13:33:18.628731 veloadmin-1.0.1/veloadmin.egg-info/
--rw-rw-rw-   0        0        0      169 2023-07-02 13:33:17.000000 veloadmin-1.0.1/veloadmin.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      250 2023-07-02 13:33:17.000000 veloadmin-1.0.1/veloadmin.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-02 13:33:17.000000 veloadmin-1.0.1/veloadmin.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-07-02 13:33:17.000000 veloadmin-1.0.1/veloadmin.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        8 2023-07-02 13:33:17.000000 veloadmin-1.0.1/veloadmin.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-07-02 13:33:17.000000 veloadmin-1.0.1/veloadmin.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-02 15:05:42.749913 veloadmin-1.0.2/
+-rw-rw-rw-   0        0        0      169 2023-07-02 15:05:42.749913 veloadmin-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-02 15:05:42.749913 veloadmin-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      466 2023-07-02 14:35:33.000000 veloadmin-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-02 15:05:42.703024 veloadmin-1.0.2/veloAdmin/
+-rw-rw-rw-   0        0        0        0 2023-07-02 13:22:37.000000 veloadmin-1.0.2/veloAdmin/__init__.py
+-rw-rw-rw-   0        0        0    11100 2023-07-02 15:02:07.000000 veloadmin-1.0.2/veloAdmin/create.py
+drwxrwxrwx   0        0        0        0 2023-07-02 15:05:42.749913 veloadmin-1.0.2/veloadmin.egg-info/
+-rw-rw-rw-   0        0        0      169 2023-07-02 15:05:42.000000 veloadmin-1.0.2/veloadmin.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      250 2023-07-02 15:05:42.000000 veloadmin-1.0.2/veloadmin.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-02 15:05:42.000000 veloadmin-1.0.2/veloadmin.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-07-02 15:05:42.000000 veloadmin-1.0.2/veloadmin.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        8 2023-07-02 15:05:42.000000 veloadmin-1.0.2/veloadmin.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-07-02 15:05:42.000000 veloadmin-1.0.2/veloadmin.egg-info/top_level.txt
```

