# Comparing `tmp/phxutils-1.1.8.tar.gz` & `tmp/phxutils-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phxutils-1.1.8.tar", last modified: Thu May  5 20:12:56 2022, max compression
+gzip compressed data, was "phxutils-1.1.9.tar", last modified: Tue May 10 16:43:07 2022, max compression
```

## Comparing `phxutils-1.1.8.tar` & `phxutils-1.1.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 phx       (1000) phx       (1000)        0 2022-05-05 20:12:56.485818 phxutils-1.1.8/
--rw-rw-r--   0 phx       (1000) phx       (1000)     1059 2022-01-11 15:02:08.000000 phxutils-1.1.8/LICENSE
--rw-rw-r--   0 phx       (1000) phx       (1000)     3327 2022-05-05 20:12:56.485818 phxutils-1.1.8/PKG-INFO
--rw-rw-r--   0 phx       (1000) phx       (1000)     2928 2022-04-11 16:27:38.000000 phxutils-1.1.8/README.md
-drwxrwxr-x   0 phx       (1000) phx       (1000)        0 2022-05-05 20:12:56.481818 phxutils-1.1.8/bin/
--rwxrwxr-x   0 phx       (1000) phx       (1000)      811 2022-01-19 18:52:13.000000 phxutils-1.1.8/bin/alarm
--rwxrwxr-x   0 phx       (1000) phx       (1000)      463 2022-04-01 17:12:42.000000 phxutils-1.1.8/bin/asntocidr
--rwxrwxr-x   0 phx       (1000) phx       (1000)      745 2022-04-09 17:36:24.000000 phxutils-1.1.8/bin/cidrgrep
--rwxrwxr-x   0 phx       (1000) phx       (1000)    19041 2022-05-05 20:11:05.000000 phxutils-1.1.8/bin/crackem
--rwxrwxr-x   0 phx       (1000) phx       (1000)     5589 2022-04-22 15:03:24.000000 phxutils-1.1.8/bin/getips
--rwxrwxr-x   0 phx       (1000) phx       (1000)     3068 2022-04-14 14:30:18.000000 phxutils-1.1.8/bin/gitswitch
--rwxrwxr-x   0 phx       (1000) phx       (1000)     1006 2022-04-09 17:29:46.000000 phxutils-1.1.8/bin/ipgrep
--rwxrwxr-x   0 phx       (1000) phx       (1000)     1247 2022-04-21 17:35:56.000000 phxutils-1.1.8/bin/ipportgrep
--rwxrwxr-x   0 phx       (1000) phx       (1000)     1440 2022-04-11 16:33:38.000000 phxutils-1.1.8/bin/pipbuild
--rwxrwxr-x   0 phx       (1000) phx       (1000)      361 2022-01-11 14:49:53.000000 phxutils-1.1.8/bin/rlookup
--rwxrwxr-x   0 phx       (1000) phx       (1000)     1113 2022-01-19 19:04:54.000000 phxutils-1.1.8/bin/timer
-drwxrwxr-x   0 phx       (1000) phx       (1000)        0 2022-05-05 20:12:56.485818 phxutils-1.1.8/phxutils.egg-info/
--rw-rw-r--   0 phx       (1000) phx       (1000)     3327 2022-05-05 20:12:56.000000 phxutils-1.1.8/phxutils.egg-info/PKG-INFO
--rw-rw-r--   0 phx       (1000) phx       (1000)      289 2022-05-05 20:12:56.000000 phxutils-1.1.8/phxutils.egg-info/SOURCES.txt
--rw-rw-r--   0 phx       (1000) phx       (1000)        1 2022-05-05 20:12:56.000000 phxutils-1.1.8/phxutils.egg-info/dependency_links.txt
--rw-rw-r--   0 phx       (1000) phx       (1000)        1 2022-05-05 20:12:56.000000 phxutils-1.1.8/phxutils.egg-info/top_level.txt
--rw-rw-r--   0 phx       (1000) phx       (1000)       38 2022-05-05 20:12:56.485818 phxutils-1.1.8/setup.cfg
--rw-rw-r--   0 phx       (1000) phx       (1000)      702 2022-05-05 20:12:49.000000 phxutils-1.1.8/setup.py
+drwxrwxr-x   0 phx       (1000) phx       (1000)        0 2022-05-10 16:43:07.023645 phxutils-1.1.9/
+-rw-rw-r--   0 phx       (1000) phx       (1000)     1059 2022-01-11 15:02:08.000000 phxutils-1.1.9/LICENSE
+-rw-rw-r--   0 phx       (1000) phx       (1000)     3290 2022-05-10 16:43:07.023645 phxutils-1.1.9/PKG-INFO
+-rw-rw-r--   0 phx       (1000) phx       (1000)     2928 2022-04-11 16:27:38.000000 phxutils-1.1.9/README.md
+drwxrwxr-x   0 phx       (1000) phx       (1000)        0 2022-05-10 16:43:07.023645 phxutils-1.1.9/bin/
+-rwxrwxr-x   0 phx       (1000) phx       (1000)      811 2022-01-19 18:52:13.000000 phxutils-1.1.9/bin/alarm
+-rwxrwxr-x   0 phx       (1000) phx       (1000)      463 2022-04-01 17:12:42.000000 phxutils-1.1.9/bin/asntocidr
+-rwxrwxr-x   0 phx       (1000) phx       (1000)      745 2022-04-09 17:36:24.000000 phxutils-1.1.9/bin/cidrgrep
+-rwxrwxr-x   0 phx       (1000) phx       (1000)    19036 2022-05-10 16:41:55.000000 phxutils-1.1.9/bin/crackem
+-rwxrwxr-x   0 phx       (1000) phx       (1000)     5589 2022-04-22 15:03:24.000000 phxutils-1.1.9/bin/getips
+-rwxrwxr-x   0 phx       (1000) phx       (1000)     3068 2022-04-14 14:30:18.000000 phxutils-1.1.9/bin/gitswitch
+-rwxrwxr-x   0 phx       (1000) phx       (1000)     1006 2022-04-09 17:29:46.000000 phxutils-1.1.9/bin/ipgrep
+-rwxrwxr-x   0 phx       (1000) phx       (1000)     1247 2022-04-21 17:35:56.000000 phxutils-1.1.9/bin/ipportgrep
+-rwxrwxr-x   0 phx       (1000) phx       (1000)     1440 2022-04-11 16:33:38.000000 phxutils-1.1.9/bin/pipbuild
+-rwxrwxr-x   0 phx       (1000) phx       (1000)      361 2022-01-11 14:49:53.000000 phxutils-1.1.9/bin/rlookup
+-rwxrwxr-x   0 phx       (1000) phx       (1000)     1113 2022-01-19 19:04:54.000000 phxutils-1.1.9/bin/timer
+drwxrwxr-x   0 phx       (1000) phx       (1000)        0 2022-05-10 16:43:07.023645 phxutils-1.1.9/phxutils.egg-info/
+-rw-rw-r--   0 phx       (1000) phx       (1000)     3290 2022-05-10 16:43:06.000000 phxutils-1.1.9/phxutils.egg-info/PKG-INFO
+-rw-rw-r--   0 phx       (1000) phx       (1000)      289 2022-05-10 16:43:07.000000 phxutils-1.1.9/phxutils.egg-info/SOURCES.txt
+-rw-rw-r--   0 phx       (1000) phx       (1000)        1 2022-05-10 16:43:06.000000 phxutils-1.1.9/phxutils.egg-info/dependency_links.txt
+-rw-rw-r--   0 phx       (1000) phx       (1000)        1 2022-05-10 16:43:07.000000 phxutils-1.1.9/phxutils.egg-info/top_level.txt
+-rw-rw-r--   0 phx       (1000) phx       (1000)       38 2022-05-10 16:43:07.023645 phxutils-1.1.9/setup.cfg
+-rw-rw-r--   0 phx       (1000) phx       (1000)      702 2022-05-10 16:43:00.000000 phxutils-1.1.9/setup.py
```

### Comparing `phxutils-1.1.8/LICENSE` & `phxutils-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `phxutils-1.1.8/PKG-INFO` & `phxutils-1.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: phxutils
-Version: 1.1.8
+Version: 1.1.9
 Summary: various useful shell utilities
 Home-page: https://github.com/phx/phxutils
 Author: phx
 Author-email: phx@example.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # phxutils
@@ -97,9 +95,7 @@
 
 ### Uninstall
 
 `sed -i '/PHX_UTILS/d' ~/.bashrc && rm -rf "$HOME/bin/phxutils"`
 
 Note: replace `.bashrc` with `.zshrc` or `.bash_profile`, etc., as necessary in the above command.
 
-
-
```

### Comparing `phxutils-1.1.8/README.md` & `phxutils-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `phxutils-1.1.8/bin/alarm` & `phxutils-1.1.9/bin/alarm`

 * *Files identical despite different names*

### Comparing `phxutils-1.1.8/bin/cidrgrep` & `phxutils-1.1.9/bin/cidrgrep`

 * *Files identical despite different names*

### Comparing `phxutils-1.1.8/bin/crackem` & `phxutils-1.1.9/bin/crackem`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env bash
 
-if ! command -v hashcat >/dev/null 2>&1; then
+if ! which hashcat >/dev/null 2>&1; then
   echo "This script requires 'hashcat' to be installed."
   exit 1
 fi
 
 usage() {
   echo "
 USAGE: crackem -t hashtype -r rules_file -i input_file -o output_file -l wordlist
```

### Comparing `phxutils-1.1.8/bin/getips` & `phxutils-1.1.9/bin/getips`

 * *Files identical despite different names*

### Comparing `phxutils-1.1.8/bin/gitswitch` & `phxutils-1.1.9/bin/gitswitch`

 * *Files identical despite different names*

### Comparing `phxutils-1.1.8/bin/ipgrep` & `phxutils-1.1.9/bin/ipgrep`

 * *Files identical despite different names*

### Comparing `phxutils-1.1.8/bin/ipportgrep` & `phxutils-1.1.9/bin/ipportgrep`

 * *Files identical despite different names*

### Comparing `phxutils-1.1.8/bin/pipbuild` & `phxutils-1.1.9/bin/pipbuild`

 * *Files identical despite different names*

### Comparing `phxutils-1.1.8/bin/timer` & `phxutils-1.1.9/bin/timer`

 * *Files identical despite different names*

### Comparing `phxutils-1.1.8/phxutils.egg-info/PKG-INFO` & `phxutils-1.1.9/phxutils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: phxutils
-Version: 1.1.8
+Version: 1.1.9
 Summary: various useful shell utilities
 Home-page: https://github.com/phx/phxutils
 Author: phx
 Author-email: phx@example.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # phxutils
@@ -97,9 +95,7 @@
 
 ### Uninstall
 
 `sed -i '/PHX_UTILS/d' ~/.bashrc && rm -rf "$HOME/bin/phxutils"`
 
 Note: replace `.bashrc` with `.zshrc` or `.bash_profile`, etc., as necessary in the above command.
 
-
-
```

### Comparing `phxutils-1.1.8/setup.py` & `phxutils-1.1.9/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 binfiles = glob.glob('bin/*')
 
 setuptools.setup(
     name='phxutils',
-    version='1.1.8',
+    version='1.1.9',
     scripts = binfiles,
     author='phx',
     author_email='phx@example.com',
     description='various useful shell utilities',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/phx/phxutils',
```

