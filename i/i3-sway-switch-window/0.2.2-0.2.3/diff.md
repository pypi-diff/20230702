# Comparing `tmp/i3_sway_switch_window-0.2.2.tar.gz` & `tmp/i3_sway_switch_window-0.2.3.tar.gz`

## Comparing `i3_sway_switch_window-0.2.2.tar` & `i3_sway_switch_window-0.2.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.2.2/requirements.txt
--rw-r--r--   0        0        0     2016 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.2.2/setup.py
--rw-r--r--   0        0        0     2504 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.2.2/docs/construction.org
--rw-r--r--   0        0        0    21361 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.2.2/elisp/emacs-with-nyxt.el
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.2.2/i3_sway_switch_window/__init__.py
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.2.2/i3_sway_switch_window/__main__.py
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.2.2/i3_sway_switch_window/__version__.py
--rwxr-xr-x   0        0        0     2450 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.2.2/i3_sway_switch_window/browser_tab_list.py
--rw-r--r--   0        0        0     1990 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.2.2/i3_sway_switch_window/config.py
--rwxr-xr-x   0        0        0      524 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.2.2/i3_sway_switch_window/display_error_message.py
--rwxr-xr-x   0        0        0     2411 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.2.2/i3_sway_switch_window/emacs_buffer_lists.py
--rwxr-xr-x   0        0        0     1905 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.2.2/i3_sway_switch_window/emacs_recentf_list.py
--rw-r--r--   0        0        0     4368 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.2.2/i3_sway_switch_window/get_nyxt_title_url.py
--rwxr-xr-x   0        0        0     1139 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.2.2/i3_sway_switch_window/i3_do_add.py
--rwxr-xr-x   0        0        0     1482 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.2.2/i3_sway_switch_window/i3_do_switch.py
--rwxr-xr-x   0        0        0    15806 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.2.2/i3_sway_switch_window/main.py
--rwxr-xr-x   0        0        0     1329 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.2.2/i3_sway_switch_window/wm_window_list.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.2.2/.gitignore
--rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.2.2/LICENSE
--rw-r--r--   0        0        0    10955 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.2.2/README.md
--rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.2.2/pyproject.toml
--rw-r--r--   0        0        0    12031 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.2.3/requirements.txt
+-rw-r--r--   0        0        0     2016 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.2.3/setup.py
+-rw-r--r--   0        0        0     2504 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.2.3/docs/construction.org
+-rw-r--r--   0        0        0    21361 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.2.3/elisp/emacs-with-nyxt.el
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.2.3/i3_sway_switch_window/__init__.py
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.2.3/i3_sway_switch_window/__main__.py
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.2.3/i3_sway_switch_window/__version__.py
+-rwxr-xr-x   0        0        0     2450 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.2.3/i3_sway_switch_window/browser_tab_list.py
+-rw-r--r--   0        0        0     1990 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.2.3/i3_sway_switch_window/config.py
+-rwxr-xr-x   0        0        0      524 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.2.3/i3_sway_switch_window/display_error_message.py
+-rwxr-xr-x   0        0        0     2411 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.2.3/i3_sway_switch_window/emacs_buffer_lists.py
+-rwxr-xr-x   0        0        0     1905 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.2.3/i3_sway_switch_window/emacs_recentf_list.py
+-rw-r--r--   0        0        0     4420 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.2.3/i3_sway_switch_window/get_nyxt_title_url.py
+-rwxr-xr-x   0        0        0     1139 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.2.3/i3_sway_switch_window/i3_do_add.py
+-rwxr-xr-x   0        0        0     1482 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.2.3/i3_sway_switch_window/i3_do_switch.py
+-rwxr-xr-x   0        0        0    15806 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.2.3/i3_sway_switch_window/main.py
+-rwxr-xr-x   0        0        0     1329 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.2.3/i3_sway_switch_window/wm_window_list.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.2.3/.gitignore
+-rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.2.3/LICENSE
+-rw-r--r--   0        0        0    10749 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.2.3/README.md
+-rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0    11825 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.2.3/PKG-INFO
```

### Comparing `i3_sway_switch_window-0.2.2/setup.py` & `i3_sway_switch_window-0.2.3/setup.py`

 * *Files identical despite different names*

### Comparing `i3_sway_switch_window-0.2.2/docs/construction.org` & `i3_sway_switch_window-0.2.3/docs/construction.org`

 * *Files identical despite different names*

### Comparing `i3_sway_switch_window-0.2.2/elisp/emacs-with-nyxt.el` & `i3_sway_switch_window-0.2.3/elisp/emacs-with-nyxt.el`

 * *Files identical despite different names*

### Comparing `i3_sway_switch_window-0.2.2/i3_sway_switch_window/browser_tab_list.py` & `i3_sway_switch_window-0.2.3/i3_sway_switch_window/browser_tab_list.py`

 * *Files identical despite different names*

### Comparing `i3_sway_switch_window-0.2.2/i3_sway_switch_window/config.py` & `i3_sway_switch_window-0.2.3/i3_sway_switch_window/config.py`

 * *Files identical despite different names*

### Comparing `i3_sway_switch_window-0.2.2/i3_sway_switch_window/display_error_message.py` & `i3_sway_switch_window-0.2.3/i3_sway_switch_window/display_error_message.py`

 * *Files identical despite different names*

### Comparing `i3_sway_switch_window-0.2.2/i3_sway_switch_window/emacs_buffer_lists.py` & `i3_sway_switch_window-0.2.3/i3_sway_switch_window/emacs_buffer_lists.py`

 * *Files identical despite different names*

### Comparing `i3_sway_switch_window-0.2.2/i3_sway_switch_window/emacs_recentf_list.py` & `i3_sway_switch_window-0.2.3/i3_sway_switch_window/emacs_recentf_list.py`

 * *Files identical despite different names*

### Comparing `i3_sway_switch_window-0.2.2/i3_sway_switch_window/get_nyxt_title_url.py` & `i3_sway_switch_window-0.2.3/i3_sway_switch_window/get_nyxt_title_url.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,14 +74,15 @@
             title_url_list[-1] = title_url_list[-1][:-4]
         # Filter out internal URIs
         title_url_list = [token for token in title_url_list if '#<QURI.URI:URI' not in token]
         # Create a list of 'tile  URL' formatted similarly to brotab command 'bt list'
         title_list = []
         for item in title_url_list:
             title = re.sub(r'^....(.+)\\"\\n\s+#<QURI.*$', r'\1', item)
+            title = re.sub(r'\\\\\\"', r'"', title)
             url = re.sub(r'^.*:URI-HTTPS (.*)>$', r'\1', item)
             title_list.append(title + '  ' + url)
 
         # Make a sorted list, without duplicates
         set_res = set(title_list)
         title_list = sorted(list(set_res), key=str.casefold)
         return title_list
```

### Comparing `i3_sway_switch_window-0.2.2/i3_sway_switch_window/i3_do_add.py` & `i3_sway_switch_window-0.2.3/i3_sway_switch_window/i3_do_add.py`

 * *Files identical despite different names*

### Comparing `i3_sway_switch_window-0.2.2/i3_sway_switch_window/i3_do_switch.py` & `i3_sway_switch_window-0.2.3/i3_sway_switch_window/i3_do_switch.py`

 * *Files identical despite different names*

### Comparing `i3_sway_switch_window-0.2.2/i3_sway_switch_window/main.py` & `i3_sway_switch_window-0.2.3/i3_sway_switch_window/main.py`

 * *Files identical despite different names*

### Comparing `i3_sway_switch_window-0.2.2/i3_sway_switch_window/wm_window_list.py` & `i3_sway_switch_window-0.2.3/i3_sway_switch_window/wm_window_list.py`

 * *Files identical despite different names*

### Comparing `i3_sway_switch_window-0.2.2/.gitignore` & `i3_sway_switch_window-0.2.3/.gitignore`

 * *Files identical despite different names*

### Comparing `i3_sway_switch_window-0.2.2/LICENSE` & `i3_sway_switch_window-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `i3_sway_switch_window-0.2.2/README.md` & `i3_sway_switch_window-0.2.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # i3-sway-switch-window
 
 <div align="center">
 
-[![Build status](https://github.com/johanwiden/i3-sway-switch-window/workflows/build/badge.svg?branch=master&event=push)](https://github.com/johanwiden/i3-sway-switch-window/actions?query=workflow%3Abuild)
 [![Python Version](https://img.shields.io/pypi/pyversions/i3-sway-switch-window.svg)](https://pypi.org/project/i3-sway-switch-window/)
 [![Dependencies Status](https://img.shields.io/badge/dependencies-up%20to%20date-brightgreen.svg)](https://github.com/johanwiden/i3-sway-switch-window/pulls?utf8=%E2%9C%93&q=is%3Apr%20author%3Aapp%2Fdependabot)
 
 [![Pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/johanwiden/i3-sway-switch-window/blob/master/.pre-commit-config.yaml)
 [![Semantic Versions](https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--versions-e10079.svg)](https://github.com/johanwiden/i3-sway-switch-window/releases)
 [![License](https://img.shields.io/github/license/johanwiden/i3-sway-switch-window)](https://github.com/johanwiden/i3-sway-switch-window/blob/master/LICENSE)
```

### Comparing `i3_sway_switch_window-0.2.2/pyproject.toml` & `i3_sway_switch_window-0.2.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "i3_sway_switch_window"
-version = "0.2.2"
+version = "0.2.3"
 authors = [
   { name="Johan Widén", email="j.e.widen@gmail.com" },
 ]
 description = "In i3wm, or sway, replace current window with emacs buffer, browser tab or other window"
 readme = "README.md"
 requires-python = ">=3.8"
 dependencies = ["i3ipc", "psutil"]
```

### Comparing `i3_sway_switch_window-0.2.2/PKG-INFO` & `i3_sway_switch_window-0.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: i3_sway_switch_window
-Version: 0.2.2
+Version: 0.2.3
 Summary: In i3wm, or sway, replace current window with emacs buffer, browser tab or other window
 Project-URL: Homepage, https://github.com/johanwiden/i3-sway-switch-window
 Project-URL: Bug Tracker, https://github.com/johanwiden/i3-sway-switch-window/issues
 Author-email: Johan Widén <j.e.widen@gmail.com>
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: X11 Applications
@@ -23,15 +23,14 @@
 Requires-Dist: psutil
 Description-Content-Type: text/markdown
 
 # i3-sway-switch-window
 
 <div align="center">
 
-[![Build status](https://github.com/johanwiden/i3-sway-switch-window/workflows/build/badge.svg?branch=master&event=push)](https://github.com/johanwiden/i3-sway-switch-window/actions?query=workflow%3Abuild)
 [![Python Version](https://img.shields.io/pypi/pyversions/i3-sway-switch-window.svg)](https://pypi.org/project/i3-sway-switch-window/)
 [![Dependencies Status](https://img.shields.io/badge/dependencies-up%20to%20date-brightgreen.svg)](https://github.com/johanwiden/i3-sway-switch-window/pulls?utf8=%E2%9C%93&q=is%3Apr%20author%3Aapp%2Fdependabot)
 
 [![Pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/johanwiden/i3-sway-switch-window/blob/master/.pre-commit-config.yaml)
 [![Semantic Versions](https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--versions-e10079.svg)](https://github.com/johanwiden/i3-sway-switch-window/releases)
 [![License](https://img.shields.io/github/license/johanwiden/i3-sway-switch-window)](https://github.com/johanwiden/i3-sway-switch-window/blob/master/LICENSE)
```

