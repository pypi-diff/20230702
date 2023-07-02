# Comparing `tmp/i3_sway_switch_window-0.2.0.tar.gz` & `tmp/i3_sway_switch_window-0.2.1.tar.gz`

## Comparing `i3_sway_switch_window-0.2.0.tar` & `i3_sway_switch_window-0.2.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.2.0/requirements.txt
--rw-r--r--   0        0        0     2016 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.2.0/setup.py
--rw-r--r--   0        0        0     2504 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.2.0/docs/construction.org
--rw-r--r--   0        0        0    21361 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.2.0/elisp/emacs-with-nyxt.el
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.2.0/i3_sway_switch_window/__init__.py
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.2.0/i3_sway_switch_window/__main__.py
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.2.0/i3_sway_switch_window/__version__.py
--rwxr-xr-x   0        0        0     2307 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.2.0/i3_sway_switch_window/browser_tab_list.py
--rw-r--r--   0        0        0     1990 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.2.0/i3_sway_switch_window/config.py
--rwxr-xr-x   0        0        0      524 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.2.0/i3_sway_switch_window/display_error_message.py
--rwxr-xr-x   0        0        0     2411 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.2.0/i3_sway_switch_window/emacs_buffer_lists.py
--rwxr-xr-x   0        0        0     1905 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.2.0/i3_sway_switch_window/emacs_recentf_list.py
--rw-r--r--   0        0        0     4339 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.2.0/i3_sway_switch_window/get_nyxt_title_url.py
--rwxr-xr-x   0        0        0     1139 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.2.0/i3_sway_switch_window/i3_do_add.py
--rwxr-xr-x   0        0        0     1482 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.2.0/i3_sway_switch_window/i3_do_switch.py
--rwxr-xr-x   0        0        0    15806 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.2.0/i3_sway_switch_window/main.py
--rwxr-xr-x   0        0        0     1329 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.2.0/i3_sway_switch_window/wm_window_list.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.2.0/.gitignore
--rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.2.0/LICENSE
--rw-r--r--   0        0        0    10945 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.2.0/README.md
--rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.2.0/pyproject.toml
--rw-r--r--   0        0        0    12021 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.2.1/requirements.txt
+-rw-r--r--   0        0        0     2016 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.2.1/setup.py
+-rw-r--r--   0        0        0     2504 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.2.1/docs/construction.org
+-rw-r--r--   0        0        0    21361 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.2.1/elisp/emacs-with-nyxt.el
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.2.1/i3_sway_switch_window/__init__.py
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.2.1/i3_sway_switch_window/__main__.py
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.2.1/i3_sway_switch_window/__version__.py
+-rwxr-xr-x   0        0        0     2307 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.2.1/i3_sway_switch_window/browser_tab_list.py
+-rw-r--r--   0        0        0     1990 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.2.1/i3_sway_switch_window/config.py
+-rwxr-xr-x   0        0        0      524 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.2.1/i3_sway_switch_window/display_error_message.py
+-rwxr-xr-x   0        0        0     2411 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.2.1/i3_sway_switch_window/emacs_buffer_lists.py
+-rwxr-xr-x   0        0        0     1905 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.2.1/i3_sway_switch_window/emacs_recentf_list.py
+-rw-r--r--   0        0        0     4339 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.2.1/i3_sway_switch_window/get_nyxt_title_url.py
+-rwxr-xr-x   0        0        0     1139 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.2.1/i3_sway_switch_window/i3_do_add.py
+-rwxr-xr-x   0        0        0     1482 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.2.1/i3_sway_switch_window/i3_do_switch.py
+-rwxr-xr-x   0        0        0    15806 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.2.1/i3_sway_switch_window/main.py
+-rwxr-xr-x   0        0        0     1329 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.2.1/i3_sway_switch_window/wm_window_list.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.2.1/.gitignore
+-rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.2.1/LICENSE
+-rw-r--r--   0        0        0    10955 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.2.1/README.md
+-rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0    12031 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.2.1/PKG-INFO
```

### Comparing `i3_sway_switch_window-0.2.0/setup.py` & `i3_sway_switch_window-0.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `i3_sway_switch_window-0.2.0/docs/construction.org` & `i3_sway_switch_window-0.2.1/docs/construction.org`

 * *Files identical despite different names*

### Comparing `i3_sway_switch_window-0.2.0/elisp/emacs-with-nyxt.el` & `i3_sway_switch_window-0.2.1/elisp/emacs-with-nyxt.el`

 * *Files identical despite different names*

### Comparing `i3_sway_switch_window-0.2.0/i3_sway_switch_window/browser_tab_list.py` & `i3_sway_switch_window-0.2.1/i3_sway_switch_window/browser_tab_list.py`

 * *Files identical despite different names*

### Comparing `i3_sway_switch_window-0.2.0/i3_sway_switch_window/config.py` & `i3_sway_switch_window-0.2.1/i3_sway_switch_window/config.py`

 * *Files identical despite different names*

### Comparing `i3_sway_switch_window-0.2.0/i3_sway_switch_window/display_error_message.py` & `i3_sway_switch_window-0.2.1/i3_sway_switch_window/display_error_message.py`

 * *Files identical despite different names*

### Comparing `i3_sway_switch_window-0.2.0/i3_sway_switch_window/emacs_buffer_lists.py` & `i3_sway_switch_window-0.2.1/i3_sway_switch_window/emacs_buffer_lists.py`

 * *Files identical despite different names*

### Comparing `i3_sway_switch_window-0.2.0/i3_sway_switch_window/emacs_recentf_list.py` & `i3_sway_switch_window-0.2.1/i3_sway_switch_window/emacs_recentf_list.py`

 * *Files identical despite different names*

### Comparing `i3_sway_switch_window-0.2.0/i3_sway_switch_window/get_nyxt_title_url.py` & `i3_sway_switch_window-0.2.1/i3_sway_switch_window/get_nyxt_title_url.py`

 * *Files identical despite different names*

### Comparing `i3_sway_switch_window-0.2.0/i3_sway_switch_window/i3_do_add.py` & `i3_sway_switch_window-0.2.1/i3_sway_switch_window/i3_do_add.py`

 * *Files identical despite different names*

### Comparing `i3_sway_switch_window-0.2.0/i3_sway_switch_window/i3_do_switch.py` & `i3_sway_switch_window-0.2.1/i3_sway_switch_window/i3_do_switch.py`

 * *Files identical despite different names*

### Comparing `i3_sway_switch_window-0.2.0/i3_sway_switch_window/main.py` & `i3_sway_switch_window-0.2.1/i3_sway_switch_window/main.py`

 * *Files identical despite different names*

### Comparing `i3_sway_switch_window-0.2.0/i3_sway_switch_window/wm_window_list.py` & `i3_sway_switch_window-0.2.1/i3_sway_switch_window/wm_window_list.py`

 * *Files identical despite different names*

### Comparing `i3_sway_switch_window-0.2.0/.gitignore` & `i3_sway_switch_window-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `i3_sway_switch_window-0.2.0/LICENSE` & `i3_sway_switch_window-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `i3_sway_switch_window-0.2.0/README.md` & `i3_sway_switch_window-0.2.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -131,15 +131,15 @@
 This is a stopgap measure until a simpler means of getting info from nyxt, has been implemented.
 
 browser_tab will attempt to get info from nyxt, only if nyxt is running.
 The check for a running nyxt is done using python package psutil.
 
 emacs currently uses a modified version of https://github.com/ag91/emacs-with-nyxt to communicate with nyxt,
 as the version in the ag91 repo seems to be for an older version of nyxt (the elisp file is dated 230327).
-You can find the modified version of 'emacs-with-nyxt.el' here: [emacs-with-nyxt.el](https://github.com/johanwiden/i3-sway-switch-window/elisp/emacs-with-nyxt.el) 
+You can find the modified version of 'emacs-with-nyxt.el' here: [emacs-with-nyxt.el](https://github.com/johanwiden/i3-sway-switch-window/blob/main/elisp/emacs-with-nyxt.el) 
 A few functions have been commented out, and the require for 'sly' has been uncommented.
 
 In my emacs config I have the following code to load 'emacs-with-nyxt.el':
 ```bash
 (defun load-emacs-with-nyxt ()
   (interactive)
   (load "/home/someuser/.config/doom/emacs-with-nyxt.el"))
```

### Comparing `i3_sway_switch_window-0.2.0/pyproject.toml` & `i3_sway_switch_window-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "i3_sway_switch_window"
-version = "0.2.0"
+version = "0.2.1"
 authors = [
   { name="Johan Widén", email="j.e.widen@gmail.com" },
 ]
 description = "In i3wm, or sway, replace current window with emacs buffer, browser tab or other window"
 readme = "README.md"
 requires-python = ">=3.8"
 dependencies = ["i3ipc", "psutil"]
```

### Comparing `i3_sway_switch_window-0.2.0/PKG-INFO` & `i3_sway_switch_window-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: i3_sway_switch_window
-Version: 0.2.0
+Version: 0.2.1
 Summary: In i3wm, or sway, replace current window with emacs buffer, browser tab or other window
 Project-URL: Homepage, https://github.com/johanwiden/i3-sway-switch-window
 Project-URL: Bug Tracker, https://github.com/johanwiden/i3-sway-switch-window/issues
 Author-email: Johan Widén <j.e.widen@gmail.com>
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: X11 Applications
@@ -156,15 +156,15 @@
 This is a stopgap measure until a simpler means of getting info from nyxt, has been implemented.
 
 browser_tab will attempt to get info from nyxt, only if nyxt is running.
 The check for a running nyxt is done using python package psutil.
 
 emacs currently uses a modified version of https://github.com/ag91/emacs-with-nyxt to communicate with nyxt,
 as the version in the ag91 repo seems to be for an older version of nyxt (the elisp file is dated 230327).
-You can find the modified version of 'emacs-with-nyxt.el' here: [emacs-with-nyxt.el](https://github.com/johanwiden/i3-sway-switch-window/elisp/emacs-with-nyxt.el) 
+You can find the modified version of 'emacs-with-nyxt.el' here: [emacs-with-nyxt.el](https://github.com/johanwiden/i3-sway-switch-window/blob/main/elisp/emacs-with-nyxt.el) 
 A few functions have been commented out, and the require for 'sly' has been uncommented.
 
 In my emacs config I have the following code to load 'emacs-with-nyxt.el':
 ```bash
 (defun load-emacs-with-nyxt ()
   (interactive)
   (load "/home/someuser/.config/doom/emacs-with-nyxt.el"))
```

