# Comparing `tmp/i3_sway_switch_window-0.1.0.tar.gz` & `tmp/i3_sway_switch_window-0.2.0.tar.gz`

## Comparing `i3_sway_switch_window-0.1.0.tar` & `i3_sway_switch_window-0.2.0.tar`

### file list

```diff
@@ -1,20 +1,22 @@
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.1.0/requirements.txt
--rw-r--r--   0        0        0     2007 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.1.0/setup.py
--rw-r--r--   0        0        0     2504 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.1.0/docs/construction.org
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.1.0/i3_sway_switch_window/__init__.py
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.1.0/i3_sway_switch_window/__main__.py
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.1.0/i3_sway_switch_window/__version__.py
--rwxr-xr-x   0        0        0     1864 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.1.0/i3_sway_switch_window/browser_tab_list.py
--rw-r--r--   0        0        0     1990 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.1.0/i3_sway_switch_window/config.py
--rwxr-xr-x   0        0        0      524 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.1.0/i3_sway_switch_window/display_error_message.py
--rwxr-xr-x   0        0        0     2411 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.1.0/i3_sway_switch_window/emacs_buffer_lists.py
--rwxr-xr-x   0        0        0     1905 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.1.0/i3_sway_switch_window/emacs_recentf_list.py
--rwxr-xr-x   0        0        0     1139 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.1.0/i3_sway_switch_window/i3_do_add.py
--rwxr-xr-x   0        0        0     1482 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.1.0/i3_sway_switch_window/i3_do_switch.py
--rwxr-xr-x   0        0        0    14227 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.1.0/i3_sway_switch_window/main.py
--rwxr-xr-x   0        0        0     1329 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.1.0/i3_sway_switch_window/wm_window_list.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.1.0/.gitignore
--rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.1.0/LICENSE
--rw-r--r--   0        0        0     8405 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.1.0/README.md
--rw-r--r--   0        0        0     1438 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     9459 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.2.0/requirements.txt
+-rw-r--r--   0        0        0     2016 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.2.0/setup.py
+-rw-r--r--   0        0        0     2504 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.2.0/docs/construction.org
+-rw-r--r--   0        0        0    21361 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.2.0/elisp/emacs-with-nyxt.el
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.2.0/i3_sway_switch_window/__init__.py
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.2.0/i3_sway_switch_window/__main__.py
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.2.0/i3_sway_switch_window/__version__.py
+-rwxr-xr-x   0        0        0     2307 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.2.0/i3_sway_switch_window/browser_tab_list.py
+-rw-r--r--   0        0        0     1990 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.2.0/i3_sway_switch_window/config.py
+-rwxr-xr-x   0        0        0      524 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.2.0/i3_sway_switch_window/display_error_message.py
+-rwxr-xr-x   0        0        0     2411 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.2.0/i3_sway_switch_window/emacs_buffer_lists.py
+-rwxr-xr-x   0        0        0     1905 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.2.0/i3_sway_switch_window/emacs_recentf_list.py
+-rw-r--r--   0        0        0     4339 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.2.0/i3_sway_switch_window/get_nyxt_title_url.py
+-rwxr-xr-x   0        0        0     1139 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.2.0/i3_sway_switch_window/i3_do_add.py
+-rwxr-xr-x   0        0        0     1482 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.2.0/i3_sway_switch_window/i3_do_switch.py
+-rwxr-xr-x   0        0        0    15806 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.2.0/i3_sway_switch_window/main.py
+-rwxr-xr-x   0        0        0     1329 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.2.0/i3_sway_switch_window/wm_window_list.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.2.0/LICENSE
+-rw-r--r--   0        0        0    10945 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.2.0/README.md
+-rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0    12021 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.2.0/PKG-INFO
```

### Comparing `i3_sway_switch_window-0.1.0/setup.py` & `i3_sway_switch_window-0.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         ],
     project_urls = {
         "Bug Tracker": "https://github.com/johanwiden/i3-sway-switch-window/issues"
     },
     license='MIT License',
     packages=setuptools.find_packages(),
     # packages=['i3-switch-window'],
-    install_requires=['i3ipc','stat','subprocess','tempfile'],
+    install_requires=['i3ipc','psutil','stat','subprocess','tempfile'],
     entry_points = {
         'console_scripts': [
             'emacs_buffers = i3_sway_switch_window.main:cli_emacs_buffers',
             'emacs_recentf = i3_sway_switch_window.main:cli_emacs_recentf',
             'browser_tab = i3_sway_switch_window.main:cli_browser_tab',
             'wm_window_switch = i3_sway_switch_window.main:cli_wm_window_switch',
         ]
```

### Comparing `i3_sway_switch_window-0.1.0/docs/construction.org` & `i3_sway_switch_window-0.2.0/docs/construction.org`

 * *Files identical despite different names*

### Comparing `i3_sway_switch_window-0.1.0/i3_sway_switch_window/browser_tab_list.py` & `i3_sway_switch_window-0.2.0/i3_sway_switch_window/browser_tab_list.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,36 +4,46 @@
 #   To support other tabs we have to ensure we use the same web browser the tab comes from.
 # The list is sorted case insensitive.
 
 # Note to developer: All error messages are to be presented to the user in one (well known) place.
 
 import re
 import subprocess
+import i3_sway_switch_window.get_nyxt_title_url
 import i3_sway_switch_window.display_error_message
 
-def _browser_tab_list():
+def _browser_tab_list(get_urls_from_nyxt):
     """Return list of web browser tab titles and URLs.
 
+    If get_urls_from_nyxt is True then also try to get titles and URLs from nyxt browser.
     The first column (tab ID), of each list item, is removed. The list is sorted case insensitive.
     """
+    success = 1
     try:
         subprocess_result = subprocess.run(['bt','list'],
                                            capture_output=True, encoding="utf-8", check=True, timeout=5)
     except FileNotFoundError as exc:
+        success = 0
         error_message = f"Process failed because the executable could not be found.\n{exc}"
         i3_sway_switch_window.display_error_message._display_error_message(error_message)
-        return [[],[],[]]
     except subprocess.CalledProcessError as exc:
+        success = 0
         error_message = f"Process failed because did not return a successful return code: {exc.returncode}\n{exc}"
         i3_sway_switch_window.display_error_message._display_error_message(error_message)
-        return [[],[],[]]
     except subprocess.TimeoutExpired as exc:
+        success = 0
         error_message = f"Process timed out.\n{exc}"
         i3_sway_switch_window.display_error_message._display_error_message(error_message)
-        return [[],[],[]]
 
-    # print(subprocess_result.stdout)
-    all_tabs = list(subprocess_result.stdout.split("\n"))
-    all_tabs = [re.sub(r'^\S+\s', '', token) for token in all_tabs] # Remove tab ID column
-    web_tabs = [token for token in all_tabs if 'https://' in token]
-    web_tabs.sort(key=str.casefold)
-    return web_tabs
+    if success:
+        all_tabs = list(subprocess_result.stdout.split("\n"))
+        all_tabs = [re.sub(r'^\S+\s', '', token) for token in all_tabs] # Remove tab ID column
+        # Filter out internal URIs
+        web_tabs = [token for token in all_tabs if 'https://' in token]
+        if get_urls_from_nyxt:
+            web_tabs = web_tabs + i3_sway_switch_window.get_nyxt_title_url._get_nyxt_title_url()
+        # Make a sorted list, without duplicates
+        set_res = set(web_tabs)
+        web_tabs = sorted(list(set_res), key=str.casefold)
+        return web_tabs
+    else:
+        return []
```

### Comparing `i3_sway_switch_window-0.1.0/i3_sway_switch_window/config.py` & `i3_sway_switch_window-0.2.0/i3_sway_switch_window/config.py`

 * *Files identical despite different names*

### Comparing `i3_sway_switch_window-0.1.0/i3_sway_switch_window/display_error_message.py` & `i3_sway_switch_window-0.2.0/i3_sway_switch_window/display_error_message.py`

 * *Files identical despite different names*

### Comparing `i3_sway_switch_window-0.1.0/i3_sway_switch_window/emacs_buffer_lists.py` & `i3_sway_switch_window-0.2.0/i3_sway_switch_window/emacs_buffer_lists.py`

 * *Files identical despite different names*

### Comparing `i3_sway_switch_window-0.1.0/i3_sway_switch_window/emacs_recentf_list.py` & `i3_sway_switch_window-0.2.0/i3_sway_switch_window/emacs_recentf_list.py`

 * *Files identical despite different names*

### Comparing `i3_sway_switch_window-0.1.0/i3_sway_switch_window/i3_do_add.py` & `i3_sway_switch_window-0.2.0/i3_sway_switch_window/i3_do_add.py`

 * *Files identical despite different names*

### Comparing `i3_sway_switch_window-0.1.0/i3_sway_switch_window/i3_do_switch.py` & `i3_sway_switch_window-0.2.0/i3_sway_switch_window/i3_do_switch.py`

 * *Files identical despite different names*

### Comparing `i3_sway_switch_window-0.1.0/i3_sway_switch_window/main.py` & `i3_sway_switch_window-0.2.0/i3_sway_switch_window/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,15 +16,21 @@
 import i3_sway_switch_window.wm_window_list
 import i3_sway_switch_window.i3_do_add
 import i3_sway_switch_window.i3_do_switch
 import i3_sway_switch_window.__version__
 
 # Possible to change in config file
 roficommand = 'rofi -dmenu'
+
 webbrowser = 'vivaldi' # Default value
+webbrowser_commandlineoptions = '--new-window'
+webbrowser_urlprefix = ''
+webbrowser_urlsuffix = ''
+get_urls_from_nyxt = False
+
 swap_workspace = '2'
 
 def _select_item_and_switch(add_or_swap_window, focused_window_id, window_name_list):
     """Call 'rofi' to select an item from 'window_name_list'. Swap in or move window at focused window.
 
     Parameters:
     - add_or_swap_window:
@@ -163,20 +169,25 @@
     """Get browser tab titles and URLs. Select one, display it in desktop window.
 
     Use rofi to select URL. Display with web browser. Parameter 'add_or_swap_window':
     - add: Show the window next to the currently focused window.
     - swap: The window is displayed instead of the currently focused window.
             The currently focused window is moved to a different workspace.
     """
-    tab_list = i3_sway_switch_window.browser_tab_list._browser_tab_list()
-    command_prefix = webbrowser + " --new-window "
-    command_suffix = "\n"
-    _select_item_execute_and_switch(add_or_swap_window, tab_list,
-                                    command_prefix, command_suffix,
-                                    r'.*h(ttps://\S+)\s*$', r"'h\1'")
+    tab_list = i3_sway_switch_window.browser_tab_list._browser_tab_list(get_urls_from_nyxt)
+    command_prefix = webbrowser + " " + webbrowser_commandlineoptions + " " + webbrowser_urlprefix
+    command_suffix = webbrowser_urlsuffix + "\n"
+    if len(webbrowser_urlprefix) > 0 and webbrowser_urlprefix[-1] == '"':
+        _select_item_execute_and_switch(add_or_swap_window, tab_list,
+                                        command_prefix, command_suffix,
+                                        r'.*h(ttps://\S+)\s*$', r"h\1")
+    else:
+        _select_item_execute_and_switch(add_or_swap_window, tab_list,
+                                        command_prefix, command_suffix,
+                                        r'.*h(ttps://\S+)\s*$', r"'h\1'")
 
 def switch_in_wm_window(add_or_swap_window):
     """Use rofi to select a top level wm window (container) from a list. Move window to/near focused window.
 
     Parameter 'add_or_swap_window':
     - add: Show the window next to the currently focused window.
     - swap: The window is displayed instead of the currently focused window.
@@ -209,24 +220,40 @@
     config_path = ''
     if args.config:
         config_path = args.config
     if not i3_sway_switch_window.config._read_config_file(config_path):
         exit(1)
     config_roficommand = i3_sway_switch_window.config._get_value('roficommand', 'roficommand')
     config_webbrowser = i3_sway_switch_window.config._get_value('webbrowser', 'webbrowser')
+    config_webbrowser_commandlineoptions = i3_sway_switch_window.config._get_value('webbrowser', 'commandlineoptions')
+    config_webbrowser_urlprefix = i3_sway_switch_window.config._get_value('webbrowser', 'urlprefix')
+    config_webbrowser_urlsuffix = i3_sway_switch_window.config._get_value('webbrowser', 'urlsuffix')
+    config_webbrowser_get_urls_from_nyxt = i3_sway_switch_window.config._get_value('webbrowser', 'get_urls_from_nyxt')
     config_swap_workspace = i3_sway_switch_window.config._get_value('workspace', 'swap_workspace')
     global roficommand
     global webbrowser
+    global webbrowser_commandlineoptions
+    global webbrowser_urlprefix
+    global webbrowser_urlsuffix
+    global get_urls_from_nyxt
     global swap_workspace
     if len(config_roficommand) > 0:
         roficommand = config_roficommand
     if args.browser:
         webbrowser = args.browser
     elif len(config_webbrowser) > 0:
         webbrowser = config_webbrowser
+    if len(config_webbrowser_commandlineoptions) > 0:
+        webbrowser_commandlineoptions = config_webbrowser_commandlineoptions
+    if len(config_webbrowser_urlprefix) > 0:
+        webbrowser_urlprefix = config_webbrowser_urlprefix
+    if len(config_webbrowser_urlsuffix) > 0:
+        webbrowser_urlsuffix = config_webbrowser_urlsuffix
+    if len(config_webbrowser_get_urls_from_nyxt) > 0 and config_webbrowser_get_urls_from_nyxt == 'yes':
+        get_urls_from_nyxt = True
     if len(config_swap_workspace) > 0:
         swap_workspace = config_swap_workspace
     return args.action
 
 def cli_emacs_buffers():
     """Use rofi to select an emacs buffer. Open emacsclient with selected buffer.
```

### Comparing `i3_sway_switch_window-0.1.0/i3_sway_switch_window/wm_window_list.py` & `i3_sway_switch_window-0.2.0/i3_sway_switch_window/wm_window_list.py`

 * *Files identical despite different names*

### Comparing `i3_sway_switch_window-0.1.0/.gitignore` & `i3_sway_switch_window-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `i3_sway_switch_window-0.1.0/LICENSE` & `i3_sway_switch_window-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `i3_sway_switch_window-0.1.0/README.md` & `i3_sway_switch_window-0.2.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -45,26 +45,53 @@
 To use browser_tab, brotab must be installed. See https://github.com/balta2ar/brotab for how to install the command line application.
 You must also have the brotab browser extensiom installed in your browser, and enabled.
 
 Note that the brotab command line application 'bt', is currently unable to communicate with browsers installed via flatpak and snap.
 On Ubuntu I have had success with the vivaldi browser. It is still possible to open the URLs with for example chrome.
 Note 2023-06-22: bt now works also with chrome on Ubuntu.
 
+The browser_tab command can be configured to display in for example chrome and vivaldi. It can also be configured to display in the nyxt browser, see the details in the config example below.
+
+Beside getting info from brotab, browser_tab can be configured to also get info from the nyxt browser, but that requires some extra configuration. See below.
+
 The i3-sway-switch-window applications expect to find a configuration file in "i3_sway_switch_window/config.ini" in your config directory.
 The file can be empty.
 
 A sample config.ini is:
 ```bash
 [roficommand]
 # Default is "rofi -dmenu"
 roficommand = /usr/local/bin/rofi -dmenu
 
 [webbrowser]
 # Default is "vivaldi"
 webbrowser = google-chrome
+# commandlineoptions is default --new-window
+# urlprefix is default empty
+# urlsuffix is default empty
+
+# Config for displaying in the nyxt browser:
+# webbrowser = nyxt
+# commandlineoptions = -r -q -e
+# urlprefix = '(make-window (make-buffer :url "
+# urlsuffix = "))'
+#
+# Besides this the following is needed in nyxt config
+# (define-configuration browser
+#   (
+#    ;; Whether code sent to the socket gets executed.  You must understand the
+#    ;; risks before enabling this: a privileged user with access to your system
+#    ;; can then take control of the browser and execute arbitrary code under your
+#    ;; user profile.
+#    (remote-execution-p t)))
+
+# Should we try to get a list of titles and URLs from nyxt webbrowser.
+# There are some requirements: See the project README.
+# default is no
+get_urls_from_nyxt = yes
 
 [workspace]
 # i3, or sway, workspace to which focused window will be swapped
 # Default is "2"
 swap_workspace = 9
 ```
 
@@ -95,24 +122,53 @@
 
 # get recentf list from emacs, select one, display next to current desktop window
 bindsym $mod+Shift+r exec ~/.local/bin/emacs_recentf add
 ```
 
 Note for sway: An alternative to wm_window_switch is to use swayr command 'swap-focused-with', see https://sr.ht/~tsdh/swayr
 
-## Developer info
+### Requirements to get info from the nyxt browser
+i3-sway-switch-window currently uses emacsclient and emacs server to communicate with nyxt.
+This is a stopgap measure until a simpler means of getting info from nyxt, has been implemented.
+
+browser_tab will attempt to get info from nyxt, only if nyxt is running.
+The check for a running nyxt is done using python package psutil.
+
+emacs currently uses a modified version of https://github.com/ag91/emacs-with-nyxt to communicate with nyxt,
+as the version in the ag91 repo seems to be for an older version of nyxt (the elisp file is dated 230327).
+You can find the modified version of 'emacs-with-nyxt.el' here: [emacs-with-nyxt.el](https://github.com/johanwiden/i3-sway-switch-window/elisp/emacs-with-nyxt.el) 
+A few functions have been commented out, and the require for 'sly' has been uncommented.
+
+In my emacs config I have the following code to load 'emacs-with-nyxt.el':
+```bash
+(defun load-emacs-with-nyxt ()
+  (interactive)
+  (load "/home/someuser/.config/doom/emacs-with-nyxt.el"))
+```
+
+You need to add this (with the correct file path), to your emacs config, if you do not load 'emacs-with-nyxt.el' at start of emacs.
 
+Nyxt must also be configured to start a 'slynk' server. To do this add the line:
+```bash
+(start-slynk)
+```
+
+to your nyxt config.
+
+## Developer info
 To build the package:
 - Download the repo. E.g. git clone https://github.com/johanwiden/i3-sway-switch-window.git
 - Create a virtual environment, for development. E.g. with conda
   - conda create --name i3env
   - conda activate i3env
   - conda install -c anaconda pip
   - pip install i3ipc
     This is a package dependency
+  - pip install psutil
+    This is a package dependency
   - pip install build
     This is the tool to build the package.
 - Change directory to the downloaded repo
 - python3 -m build
     This should build the package, the result is stored in subdirectory 'dist'
 
 ### Running the applications
```

### Comparing `i3_sway_switch_window-0.1.0/pyproject.toml` & `i3_sway_switch_window-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "i3_sway_switch_window"
-version = "0.1.0"
+version = "0.2.0"
 authors = [
   { name="Johan Widén", email="j.e.widen@gmail.com" },
 ]
 description = "In i3wm, or sway, replace current window with emacs buffer, browser tab or other window"
 readme = "README.md"
 requires-python = ">=3.8"
-dependencies = ["i3ipc"]
+dependencies = ["i3ipc", "psutil"]
 classifiers = [
     # complete classifier list:
     # http://pypi.python.org/pypi?%3Aaction=list_classifiers
     'Development Status :: 4 - Beta',
     'License :: OSI Approved :: MIT License',
     'Environment :: X11 Applications',
     'Intended Audience :: End Users/Desktop',
```

### Comparing `i3_sway_switch_window-0.1.0/PKG-INFO` & `i3_sway_switch_window-0.2.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: i3_sway_switch_window
-Version: 0.1.0
+Version: 0.2.0
 Summary: In i3wm, or sway, replace current window with emacs buffer, browser tab or other window
 Project-URL: Homepage, https://github.com/johanwiden/i3-sway-switch-window
 Project-URL: Bug Tracker, https://github.com/johanwiden/i3-sway-switch-window/issues
 Author-email: Johan Widén <j.e.widen@gmail.com>
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: X11 Applications
@@ -16,14 +16,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Unix Shell
 Classifier: Topic :: Desktop Environment :: Window Managers
 Requires-Python: >=3.8
 Requires-Dist: i3ipc
+Requires-Dist: psutil
 Description-Content-Type: text/markdown
 
 # i3-sway-switch-window
 
 <div align="center">
 
 [![Build status](https://github.com/johanwiden/i3-sway-switch-window/workflows/build/badge.svg?branch=master&event=push)](https://github.com/johanwiden/i3-sway-switch-window/actions?query=workflow%3Abuild)
@@ -69,26 +70,53 @@
 To use browser_tab, brotab must be installed. See https://github.com/balta2ar/brotab for how to install the command line application.
 You must also have the brotab browser extensiom installed in your browser, and enabled.
 
 Note that the brotab command line application 'bt', is currently unable to communicate with browsers installed via flatpak and snap.
 On Ubuntu I have had success with the vivaldi browser. It is still possible to open the URLs with for example chrome.
 Note 2023-06-22: bt now works also with chrome on Ubuntu.
 
+The browser_tab command can be configured to display in for example chrome and vivaldi. It can also be configured to display in the nyxt browser, see the details in the config example below.
+
+Beside getting info from brotab, browser_tab can be configured to also get info from the nyxt browser, but that requires some extra configuration. See below.
+
 The i3-sway-switch-window applications expect to find a configuration file in "i3_sway_switch_window/config.ini" in your config directory.
 The file can be empty.
 
 A sample config.ini is:
 ```bash
 [roficommand]
 # Default is "rofi -dmenu"
 roficommand = /usr/local/bin/rofi -dmenu
 
 [webbrowser]
 # Default is "vivaldi"
 webbrowser = google-chrome
+# commandlineoptions is default --new-window
+# urlprefix is default empty
+# urlsuffix is default empty
+
+# Config for displaying in the nyxt browser:
+# webbrowser = nyxt
+# commandlineoptions = -r -q -e
+# urlprefix = '(make-window (make-buffer :url "
+# urlsuffix = "))'
+#
+# Besides this the following is needed in nyxt config
+# (define-configuration browser
+#   (
+#    ;; Whether code sent to the socket gets executed.  You must understand the
+#    ;; risks before enabling this: a privileged user with access to your system
+#    ;; can then take control of the browser and execute arbitrary code under your
+#    ;; user profile.
+#    (remote-execution-p t)))
+
+# Should we try to get a list of titles and URLs from nyxt webbrowser.
+# There are some requirements: See the project README.
+# default is no
+get_urls_from_nyxt = yes
 
 [workspace]
 # i3, or sway, workspace to which focused window will be swapped
 # Default is "2"
 swap_workspace = 9
 ```
 
@@ -119,24 +147,53 @@
 
 # get recentf list from emacs, select one, display next to current desktop window
 bindsym $mod+Shift+r exec ~/.local/bin/emacs_recentf add
 ```
 
 Note for sway: An alternative to wm_window_switch is to use swayr command 'swap-focused-with', see https://sr.ht/~tsdh/swayr
 
-## Developer info
+### Requirements to get info from the nyxt browser
+i3-sway-switch-window currently uses emacsclient and emacs server to communicate with nyxt.
+This is a stopgap measure until a simpler means of getting info from nyxt, has been implemented.
+
+browser_tab will attempt to get info from nyxt, only if nyxt is running.
+The check for a running nyxt is done using python package psutil.
+
+emacs currently uses a modified version of https://github.com/ag91/emacs-with-nyxt to communicate with nyxt,
+as the version in the ag91 repo seems to be for an older version of nyxt (the elisp file is dated 230327).
+You can find the modified version of 'emacs-with-nyxt.el' here: [emacs-with-nyxt.el](https://github.com/johanwiden/i3-sway-switch-window/elisp/emacs-with-nyxt.el) 
+A few functions have been commented out, and the require for 'sly' has been uncommented.
+
+In my emacs config I have the following code to load 'emacs-with-nyxt.el':
+```bash
+(defun load-emacs-with-nyxt ()
+  (interactive)
+  (load "/home/someuser/.config/doom/emacs-with-nyxt.el"))
+```
+
+You need to add this (with the correct file path), to your emacs config, if you do not load 'emacs-with-nyxt.el' at start of emacs.
 
+Nyxt must also be configured to start a 'slynk' server. To do this add the line:
+```bash
+(start-slynk)
+```
+
+to your nyxt config.
+
+## Developer info
 To build the package:
 - Download the repo. E.g. git clone https://github.com/johanwiden/i3-sway-switch-window.git
 - Create a virtual environment, for development. E.g. with conda
   - conda create --name i3env
   - conda activate i3env
   - conda install -c anaconda pip
   - pip install i3ipc
     This is a package dependency
+  - pip install psutil
+    This is a package dependency
   - pip install build
     This is the tool to build the package.
 - Change directory to the downloaded repo
 - python3 -m build
     This should build the package, the result is stored in subdirectory 'dist'
 
 ### Running the applications
```

