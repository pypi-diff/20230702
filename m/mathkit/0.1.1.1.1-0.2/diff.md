# Comparing `tmp/mathkit-0.1.1.1.1.tar.gz` & `tmp/mathkit-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mathkit-0.1.1.1.1.tar", last modified: Fri Jun 30 07:00:55 2023, max compression
+gzip compressed data, was "mathkit-0.2.tar", last modified: Sun Jul  2 02:31:44 2023, max compression
```

## Comparing `mathkit-0.1.1.1.1.tar` & `mathkit-0.2.tar`

### file list

```diff
@@ -1,28 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-30 07:00:55.056739 mathkit-0.1.1.1.1/
--rw-rw-rw-   0        0        0     2816 2023-06-30 07:00:55.054808 mathkit-0.1.1.1.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-30 07:00:55.033738 mathkit-0.1.1.1.1/mathkit/
--rw-rw-rw-   0        0        0      966 2023-06-30 06:18:35.000000 mathkit-0.1.1.1.1/mathkit/__init__.py
--rw-rw-rw-   0        0        0      160 2023-06-30 04:01:47.000000 mathkit-0.1.1.1.1/mathkit/addition.py
--rw-rw-rw-   0        0        0      117 2023-06-30 06:13:56.000000 mathkit-0.1.1.1.1/mathkit/cube.py
--rw-rw-rw-   0        0        0      128 2023-06-30 05:06:59.000000 mathkit-0.1.1.1.1/mathkit/cube_root.py
--rw-rw-rw-   0        0        0      153 2023-06-30 04:06:14.000000 mathkit-0.1.1.1.1/mathkit/division.py
--rw-rw-rw-   0        0        0      356 2023-06-30 06:12:35.000000 mathkit-0.1.1.1.1/mathkit/factorial.py
--rw-rw-rw-   0        0        0      388 2023-06-30 05:08:17.000000 mathkit-0.1.1.1.1/mathkit/hcf_custom.py
--rw-rw-rw-   0        0        0      526 2023-06-30 05:07:56.000000 mathkit-0.1.1.1.1/mathkit/lcm_custom.py
--rw-rw-rw-   0        0        0      574 2023-06-30 05:08:44.000000 mathkit-0.1.1.1.1/mathkit/log_custom.py
--rw-rw-rw-   0        0        0     1524 2023-06-30 06:13:55.000000 mathkit-0.1.1.1.1/mathkit/main.py
--rw-rw-rw-   0        0        0      158 2023-06-30 04:06:46.000000 mathkit-0.1.1.1.1/mathkit/modulas.py
--rw-rw-rw-   0        0        0      143 2023-06-30 04:04:06.000000 mathkit-0.1.1.1.1/mathkit/multiply.py
--rw-rw-rw-   0        0        0      940 2023-06-30 06:12:48.000000 mathkit-0.1.1.1.1/mathkit/percentage.py
--rw-rw-rw-   0        0        0      175 2023-06-30 06:18:16.000000 mathkit-0.1.1.1.1/mathkit/power.py
--rw-rw-rw-   0        0        0      226 2023-06-30 06:13:01.000000 mathkit-0.1.1.1.1/mathkit/remainder.py
--rw-rw-rw-   0        0        0      106 2023-06-30 04:09:37.000000 mathkit-0.1.1.1.1/mathkit/square.py
--rw-rw-rw-   0        0        0      105 2023-06-30 04:11:40.000000 mathkit-0.1.1.1.1/mathkit/square_root.py
--rw-rw-rw-   0        0        0      158 2023-06-30 04:01:39.000000 mathkit-0.1.1.1.1/mathkit/subtract.py
-drwxrwxrwx   0        0        0        0 2023-06-30 07:00:55.052740 mathkit-0.1.1.1.1/mathkit.egg-info/
--rw-rw-rw-   0        0        0     2816 2023-06-30 07:00:54.000000 mathkit-0.1.1.1.1/mathkit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      492 2023-06-30 07:00:54.000000 mathkit-0.1.1.1.1/mathkit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-30 07:00:54.000000 mathkit-0.1.1.1.1/mathkit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-06-30 07:00:54.000000 mathkit-0.1.1.1.1/mathkit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-30 07:00:55.057752 mathkit-0.1.1.1.1/setup.cfg
--rw-rw-rw-   0        0        0     2944 2023-06-30 07:00:51.000000 mathkit-0.1.1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-02 02:31:44.775533 mathkit-0.2/
+-rw-rw-rw-   0        0        0     3834 2023-07-02 02:31:44.775533 mathkit-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3397 2023-07-02 02:29:33.000000 mathkit-0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-02 02:31:44.745838 mathkit-0.2/mathkit/
+-rw-rw-rw-   0        0        0      467 2023-07-02 02:00:13.000000 mathkit-0.2/mathkit/__init__.py
+-rw-rw-rw-   0        0        0     5057 2023-07-02 01:46:47.000000 mathkit-0.2/mathkit/main.py
+drwxrwxrwx   0        0        0        0 2023-07-02 02:31:44.770213 mathkit-0.2/mathkit.egg-info/
+-rw-rw-rw-   0        0        0     3834 2023-07-02 02:31:44.000000 mathkit-0.2/mathkit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      178 2023-07-02 02:31:44.000000 mathkit-0.2/mathkit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-02 02:31:44.000000 mathkit-0.2/mathkit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-07-02 02:31:44.000000 mathkit-0.2/mathkit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-02 02:31:44.778041 mathkit-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      704 2023-07-02 02:31:22.000000 mathkit-0.2/setup.py
```

