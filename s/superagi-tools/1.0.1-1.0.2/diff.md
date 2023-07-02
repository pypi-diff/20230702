# Comparing `tmp/superagi_tools-1.0.1.tar.gz` & `tmp/superagi_tools-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "superagi_tools-1.0.1.tar", last modified: Fri Jun 30 17:36:08 2023, max compression
+gzip compressed data, was "superagi_tools-1.0.2.tar", last modified: Sun Jul  2 04:54:06 2023, max compression
```

## Comparing `superagi_tools-1.0.1.tar` & `superagi_tools-1.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 abhijeet  (1000) abhijeet  (1000)        0 2023-06-30 17:36:08.539578 superagi_tools-1.0.1/
--rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)        0 2023-06-28 12:07:33.000000 superagi_tools-1.0.1/LICENSE
--rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)      187 2023-06-30 17:36:08.539578 superagi_tools-1.0.1/PKG-INFO
--rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)       76 2023-06-28 12:10:34.000000 superagi_tools-1.0.1/README.md
--rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)       38 2023-06-30 17:36:08.539578 superagi_tools-1.0.1/setup.cfg
--rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)      306 2023-06-30 17:36:03.000000 superagi_tools-1.0.1/setup.py
-drwxrwxr-x   0 abhijeet  (1000) abhijeet  (1000)        0 2023-06-30 17:36:08.483577 superagi_tools-1.0.1/superagi/
--rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)        0 2023-06-29 00:44:17.000000 superagi_tools-1.0.1/superagi/__init__.py
-drwxrwxr-x   0 abhijeet  (1000) abhijeet  (1000)        0 2023-06-30 17:36:08.483577 superagi_tools-1.0.1/superagi/tools/
--rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)        0 2023-06-29 00:51:45.000000 superagi_tools-1.0.1/superagi/tools/__init__.py
--rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)     6603 2023-06-30 05:10:33.000000 superagi_tools-1.0.1/superagi/tools/base_tool.py
-drwxrwxr-x   0 abhijeet  (1000) abhijeet  (1000)        0 2023-06-30 17:36:08.539578 superagi_tools-1.0.1/superagi_tools.egg-info/
--rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)      187 2023-06-30 17:36:07.000000 superagi_tools-1.0.1/superagi_tools.egg-info/PKG-INFO
--rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)      291 2023-06-30 17:36:08.000000 superagi_tools-1.0.1/superagi_tools.egg-info/SOURCES.txt
--rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)        1 2023-06-30 17:36:07.000000 superagi_tools-1.0.1/superagi_tools.egg-info/dependency_links.txt
--rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)       16 2023-06-30 17:36:07.000000 superagi_tools-1.0.1/superagi_tools.egg-info/requires.txt
--rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)        9 2023-06-30 17:36:07.000000 superagi_tools-1.0.1/superagi_tools.egg-info/top_level.txt
+drwxrwxr-x   0 abhijeet  (1000) abhijeet  (1000)        0 2023-07-02 04:54:06.912764 superagi_tools-1.0.2/
+-rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)     1054 2023-07-02 04:53:24.000000 superagi_tools-1.0.2/LICENSE
+-rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)      187 2023-07-02 04:54:06.912764 superagi_tools-1.0.2/PKG-INFO
+-rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)       76 2023-06-28 12:10:34.000000 superagi_tools-1.0.2/README.md
+-rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)       38 2023-07-02 04:54:06.912764 superagi_tools-1.0.2/setup.cfg
+-rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)      319 2023-07-02 04:52:07.000000 superagi_tools-1.0.2/setup.py
+drwxrwxr-x   0 abhijeet  (1000) abhijeet  (1000)        0 2023-07-02 04:54:06.896764 superagi_tools-1.0.2/superagi/
+-rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)        0 2023-06-29 00:44:17.000000 superagi_tools-1.0.2/superagi/__init__.py
+drwxrwxr-x   0 abhijeet  (1000) abhijeet  (1000)        0 2023-07-02 04:54:06.896764 superagi_tools-1.0.2/superagi/tools/
+-rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)        0 2023-06-29 00:51:45.000000 superagi_tools-1.0.2/superagi/tools/__init__.py
+-rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)     6603 2023-06-30 05:10:33.000000 superagi_tools-1.0.2/superagi/tools/base_tool.py
+drwxrwxr-x   0 abhijeet  (1000) abhijeet  (1000)        0 2023-07-02 04:54:06.912764 superagi_tools-1.0.2/superagi_tools.egg-info/
+-rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)      187 2023-07-02 04:54:06.000000 superagi_tools-1.0.2/superagi_tools.egg-info/PKG-INFO
+-rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)      291 2023-07-02 04:54:06.000000 superagi_tools-1.0.2/superagi_tools.egg-info/SOURCES.txt
+-rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)        1 2023-07-02 04:54:06.000000 superagi_tools-1.0.2/superagi_tools.egg-info/dependency_links.txt
+-rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)       29 2023-07-02 04:54:06.000000 superagi_tools-1.0.2/superagi_tools.egg-info/requires.txt
+-rw-rw-r--   0 abhijeet  (1000) abhijeet  (1000)        9 2023-07-02 04:54:06.000000 superagi_tools-1.0.2/superagi_tools.egg-info/top_level.txt
```

### Comparing `superagi_tools-1.0.1/superagi/tools/base_tool.py` & `superagi_tools-1.0.2/superagi/tools/base_tool.py`

 * *Files identical despite different names*

