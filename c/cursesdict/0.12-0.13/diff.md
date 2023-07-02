# Comparing `tmp/cursesdict-0.12.tar.gz` & `tmp/cursesdict-0.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cursesdict-0.12.tar", last modified: Sat Jul  1 06:02:36 2023, max compression
+gzip compressed data, was "cursesdict-0.13.tar", last modified: Sun Jul  2 00:25:40 2023, max compression
```

## Comparing `cursesdict-0.12.tar` & `cursesdict-0.13.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-01 06:02:36.365243 cursesdict-0.12/
--rw-rw-rw-   0        0        0     1148 2023-07-01 06:02:31.000000 cursesdict-0.12/LICENSE.rst
--rw-rw-rw-   0        0        0      101 2023-07-01 06:02:29.000000 cursesdict-0.12/MANIFEST.in
--rw-rw-rw-   0        0        0     9062 2023-07-01 06:02:36.365243 cursesdict-0.12/PKG-INFO
--rw-rw-rw-   0        0        0     8324 2023-07-01 06:01:17.000000 cursesdict-0.12/README.md
-drwxrwxrwx   0        0        0        0 2023-07-01 06:02:36.361254 cursesdict-0.12/cursesdict/
--rw-rw-rw-   0        0        0     8324 2023-07-01 06:01:17.000000 cursesdict-0.12/cursesdict/README.MD
--rw-rw-rw-   0        0        0    11442 2023-07-01 05:58:30.000000 cursesdict-0.12/cursesdict/__init__.py
--rw-rw-rw-   0        0        0       18 2023-07-01 06:02:35.000000 cursesdict-0.12/cursesdict/requirements.txt
--rw-rw-rw-   0        0        0     1256 2023-07-01 06:02:35.000000 cursesdict-0.12/cursesdict/thirdparty.json
-drwxrwxrwx   0        0        0        0 2023-07-01 06:02:36.365243 cursesdict-0.12/cursesdict.egg-info/
--rw-rw-rw-   0        0        0     9062 2023-07-01 06:02:36.000000 cursesdict-0.12/cursesdict.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      320 2023-07-01 06:02:36.000000 cursesdict-0.12/cursesdict.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-01 06:02:36.000000 cursesdict-0.12/cursesdict.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-07-01 06:02:36.000000 cursesdict-0.12/cursesdict.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-01 06:02:36.000000 cursesdict-0.12/cursesdict.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       85 2023-07-01 06:02:36.367238 cursesdict-0.12/setup.cfg
--rw-rw-rw-   0        0        0     1414 2023-07-01 06:02:35.000000 cursesdict-0.12/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-02 00:25:40.061246 cursesdict-0.13/
+-rw-rw-rw-   0        0        0     1148 2023-07-02 00:25:29.000000 cursesdict-0.13/LICENSE.rst
+-rw-rw-rw-   0        0        0      101 2023-07-02 00:25:27.000000 cursesdict-0.13/MANIFEST.in
+-rw-rw-rw-   0        0        0     9062 2023-07-02 00:25:40.062242 cursesdict-0.13/PKG-INFO
+-rw-rw-rw-   0        0        0     8324 2023-07-01 06:01:17.000000 cursesdict-0.13/README.md
+drwxrwxrwx   0        0        0        0 2023-07-02 00:25:40.058253 cursesdict-0.13/cursesdict/
+-rw-rw-rw-   0        0        0     8324 2023-07-01 06:01:17.000000 cursesdict-0.13/cursesdict/README.MD
+-rw-rw-rw-   0        0        0    11442 2023-07-02 00:24:31.000000 cursesdict-0.13/cursesdict/__init__.py
+-rw-rw-rw-   0        0        0       18 2023-07-02 00:25:38.000000 cursesdict-0.13/cursesdict/requirements.txt
+-rw-rw-rw-   0        0        0     1256 2023-07-02 00:25:38.000000 cursesdict-0.13/cursesdict/thirdparty.json
+drwxrwxrwx   0        0        0        0 2023-07-02 00:25:40.061246 cursesdict-0.13/cursesdict.egg-info/
+-rw-rw-rw-   0        0        0     9062 2023-07-02 00:25:39.000000 cursesdict-0.13/cursesdict.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      320 2023-07-02 00:25:39.000000 cursesdict-0.13/cursesdict.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-02 00:25:39.000000 cursesdict-0.13/cursesdict.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-07-02 00:25:39.000000 cursesdict-0.13/cursesdict.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-02 00:25:39.000000 cursesdict-0.13/cursesdict.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       85 2023-07-02 00:25:40.062242 cursesdict-0.13/setup.cfg
+-rw-rw-rw-   0        0        0     1414 2023-07-02 00:25:38.000000 cursesdict-0.13/setup.py
```

### Comparing `cursesdict-0.12/LICENSE.rst` & `cursesdict-0.13/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `cursesdict-0.12/PKG-INFO` & `cursesdict-0.13/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cursesdict
-Version: 0.12
+Version: 0.13
 Summary: creates an interactive menu system for your application or program, providing an intuitive and user-friendly interface for users to navigate and perform various actions
 Home-page: https://github.com/hansalemaos/cursesdict
 Author: Johannes Fischer
 Author-email: aulasparticularesdealemaosp@gmail.com
 License: MIT
 Keywords: curses,menu
 Classifier: Development Status :: 4 - Beta
```

### Comparing `cursesdict-0.12/README.md` & `cursesdict-0.13/README.md`

 * *Files identical despite different names*

### Comparing `cursesdict-0.12/cursesdict/README.MD` & `cursesdict-0.13/cursesdict/README.MD`

 * *Files identical despite different names*

### Comparing `cursesdict-0.12/cursesdict/__init__.py` & `cursesdict-0.13/cursesdict/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -292,11 +292,11 @@
                 current_choice = 0
             elif isinstance(fu, tuple):
                 active_choices = get_active_dict(menu_config.menudict, fu)
                 active_menu_choices = get_active_menu_items(active_choices)
                 current_choice = 0
         if key in menu_config.key_down_keys:
             current_choice = (current_choice + 1) % len(active_menu_choices)
-        elif key == menu_config.key_up_keys:
+        elif key in menu_config.key_up_keys:
             current_choice = (current_choice - 1) % len(active_menu_choices)
     break_window()
     curses.endwin()
```

### Comparing `cursesdict-0.12/cursesdict/thirdparty.json` & `cursesdict-0.13/cursesdict/thirdparty.json`

 * *Files identical despite different names*

### Comparing `cursesdict-0.12/cursesdict.egg-info/PKG-INFO` & `cursesdict-0.13/cursesdict.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cursesdict
-Version: 0.12
+Version: 0.13
 Summary: creates an interactive menu system for your application or program, providing an intuitive and user-friendly interface for users to navigate and perform various actions
 Home-page: https://github.com/hansalemaos/cursesdict
 Author: Johannes Fischer
 Author-email: aulasparticularesdealemaosp@gmail.com
 License: MIT
 Keywords: curses,menu
 Classifier: Development Status :: 4 - Beta
```

### Comparing `cursesdict-0.12/setup.py` & `cursesdict-0.13/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 with open(os.path.join(os.path.abspath(os.path.dirname(__file__)),'README.md'), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()\
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 #long_description = (this_directory / "README.md").read_text()
 
-VERSION = '''0.12'''
+VERSION = '''0.13'''
 DESCRIPTION = '''creates an interactive menu system for your application or program, providing an intuitive and user-friendly interface for users to navigate and perform various actions'''
 
 # Setting up
 setup(
     name="cursesdict",
     version=VERSION,
     license='MIT',
```

