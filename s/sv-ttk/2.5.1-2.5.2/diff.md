# Comparing `tmp/sv_ttk-2.5.1.tar.gz` & `tmp/sv_ttk-2.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sv_ttk-2.5.1.tar", last modified: Wed Jun 28 11:58:59 2023, max compression
+gzip compressed data, was "sv_ttk-2.5.2.tar", last modified: Sun Jul  2 19:32:10 2023, max compression
```

## Comparing `sv_ttk-2.5.1.tar` & `sv_ttk-2.5.2.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:58:59.484024 sv_ttk-2.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-06-28 11:58:46.000000 sv_ttk-2.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-06-28 11:58:59.484024 sv_ttk-2.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-06-28 11:58:46.000000 sv_ttk-2.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-28 11:58:59.484024 sv_ttk-2.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-06-28 11:58:46.000000 sv_ttk-2.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:58:59.484024 sv_ttk-2.5.1/sv_ttk/
--rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-06-28 11:58:46.000000 sv_ttk-2.5.1/sv_ttk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5150 2023-06-28 11:58:46.000000 sv_ttk-2.5.1/sv_ttk/sv.tcl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:58:59.484024 sv_ttk-2.5.1/sv_ttk/theme/
--rw-r--r--   0 runner    (1001) docker     (123)    16187 2023-06-28 11:58:46.000000 sv_ttk-2.5.1/sv_ttk/theme/dark.tcl
--rw-r--r--   0 runner    (1001) docker     (123)    16295 2023-06-28 11:58:46.000000 sv_ttk-2.5.1/sv_ttk/theme/light.tcl
--rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-06-28 11:58:46.000000 sv_ttk-2.5.1/sv_ttk/theme/sprites_dark.tcl
--rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-06-28 11:58:46.000000 sv_ttk-2.5.1/sv_ttk/theme/sprites_light.tcl
--rw-r--r--   0 runner    (1001) docker     (123)    18371 2023-06-28 11:58:46.000000 sv_ttk-2.5.1/sv_ttk/theme/spritesheet_dark.png
--rw-r--r--   0 runner    (1001) docker     (123)    18388 2023-06-28 11:58:46.000000 sv_ttk-2.5.1/sv_ttk/theme/spritesheet_light.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:58:59.484024 sv_ttk-2.5.1/sv_ttk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-06-28 11:58:59.000000 sv_ttk-2.5.1/sv_ttk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-06-28 11:58:59.000000 sv_ttk-2.5.1/sv_ttk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 11:58:59.000000 sv_ttk-2.5.1/sv_ttk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-28 11:58:59.000000 sv_ttk-2.5.1/sv_ttk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 19:32:10.359921 sv_ttk-2.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-02 19:31:59.000000 sv_ttk-2.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-07-02 19:32:10.359921 sv_ttk-2.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-07-02 19:31:59.000000 sv_ttk-2.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 19:31:59.000000 sv_ttk-2.5.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 19:32:10.359921 sv_ttk-2.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-07-02 19:31:59.000000 sv_ttk-2.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 19:32:10.359921 sv_ttk-2.5.2/sv_ttk/
+-rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-07-02 19:31:59.000000 sv_ttk-2.5.2/sv_ttk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5150 2023-07-02 19:31:59.000000 sv_ttk-2.5.2/sv_ttk/sv.tcl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 19:32:10.359921 sv_ttk-2.5.2/sv_ttk/theme/
+-rw-r--r--   0 runner    (1001) docker     (123)    16187 2023-07-02 19:31:59.000000 sv_ttk-2.5.2/sv_ttk/theme/dark.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)    16295 2023-07-02 19:31:59.000000 sv_ttk-2.5.2/sv_ttk/theme/light.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-07-02 19:31:59.000000 sv_ttk-2.5.2/sv_ttk/theme/sprites_dark.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-07-02 19:31:59.000000 sv_ttk-2.5.2/sv_ttk/theme/sprites_light.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)     5817 2023-07-02 19:31:59.000000 sv_ttk-2.5.2/sv_ttk/theme/spritesheet_dark.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6677 2023-07-02 19:31:59.000000 sv_ttk-2.5.2/sv_ttk/theme/spritesheet_light.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 19:32:10.359921 sv_ttk-2.5.2/sv_ttk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-07-02 19:32:10.000000 sv_ttk-2.5.2/sv_ttk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-02 19:32:10.000000 sv_ttk-2.5.2/sv_ttk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 19:32:10.000000 sv_ttk-2.5.2/sv_ttk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-02 19:32:10.000000 sv_ttk-2.5.2/sv_ttk.egg-info/top_level.txt
```

### Comparing `sv_ttk-2.5.1/LICENSE` & `sv_ttk-2.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sv_ttk-2.5.1/PKG-INFO` & `sv_ttk-2.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sv_ttk
-Version: 2.5.1
+Version: 2.5.2
 Summary: A gorgeous theme for Tkinter, based on Windows 11's UI
 Home-page: https://github.com/rdbende/Sun-Valley-ttk-theme
 Author: rdbende
 Author-email: rdbende@proton.me
 License: MIT
 Project-URL: Source, https://github.com/rdbende/Sun-Valley-ttk-theme
 Project-URL: Documentation, https://github.com/rdbende/Sun-Valley-ttk-theme/wiki
```

### Comparing `sv_ttk-2.5.1/README.md` & `sv_ttk-2.5.2/README.md`

 * *Files identical despite different names*

### Comparing `sv_ttk-2.5.1/setup.py` & `sv_ttk-2.5.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     '<img alt="Cover image" src="https://raw.githubusercontent.com/rdbende/Sun-Valley-ttk-theme/master/assets/hero_light.png">',
     (Path(__file__).parent / "README.md").read_text(),
 )
 
 
 setup(
     name="sv_ttk",
-    version="2.5.1",
+    version="2.5.2",
     license="MIT",
     author="rdbende",
     author_email="rdbende@proton.me",
     url="https://github.com/rdbende/Sun-Valley-ttk-theme",
     project_urls={
         "Source": "https://github.com/rdbende/Sun-Valley-ttk-theme",
         "Documentation": "https://github.com/rdbende/Sun-Valley-ttk-theme/wiki",
```

### Comparing `sv_ttk-2.5.1/sv_ttk/__init__.py` & `sv_ttk-2.5.2/sv_ttk/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,42 +2,44 @@
 
 import sys
 import tkinter
 from functools import partial
 from pathlib import Path
 
 
-def get_default_root() -> tkinter.Misc:
-    if sys.version_info >= (3, 8):
+def _get_default_root() -> tkinter.Misc:
+    try:
         return tkinter._get_default_root()
-    else:
+    except AttributeError:
         try:
             return tkinter._default_root
         except AttributeError:
-            raise RuntimeError
+            raise RuntimeError(
+                "can't set theme, because tkinter is configured to not support implicit default root,"
+                + " and no explicit root was provided. Use the `root` argument."
+            )
+    except RuntimeError as e:
+        raise RuntimeError(
+            "can't set theme, because tkinter is configured to not support implicit default root,"
+            + " and no explicit root was provided. Use the `root` argument."
+        ) from e
 
 
 class SunValleyTtkTheme:
     initialized = False
 
     @classmethod
     def load_theme(cls, root: tkinter.Misc | None) -> None:
         if cls.initialized:
             return
 
         theme_file = (Path(__file__).parent / "sv.tcl").absolute()
 
         if root is None:
-            try:
-                cls.tcl = get_default_root()
-            except RuntimeError:
-                raise RuntimeError(
-                    "can't set theme, because tkinter is configured to not support"
-                    + " default root, and no explicit root was provided."
-                ) from None
+            cls.tcl = _get_default_root()
         else:
             cls.tcl = root
 
         cls.tcl.call("source", str(theme_file))
         cls.initialized = True
 
     @classmethod
```

### Comparing `sv_ttk-2.5.1/sv_ttk/sv.tcl` & `sv_ttk-2.5.2/sv_ttk/sv.tcl`

 * *Files identical despite different names*

### Comparing `sv_ttk-2.5.1/sv_ttk/theme/dark.tcl` & `sv_ttk-2.5.2/sv_ttk/theme/dark.tcl`

 * *Files identical despite different names*

### Comparing `sv_ttk-2.5.1/sv_ttk/theme/light.tcl` & `sv_ttk-2.5.2/sv_ttk/theme/light.tcl`

 * *Files identical despite different names*

### Comparing `sv_ttk-2.5.1/sv_ttk/theme/sprites_dark.tcl` & `sv_ttk-2.5.2/sv_ttk/theme/sprites_dark.tcl`

 * *Files identical despite different names*

### Comparing `sv_ttk-2.5.1/sv_ttk/theme/sprites_light.tcl` & `sv_ttk-2.5.2/sv_ttk/theme/sprites_light.tcl`

 * *Files identical despite different names*

### Comparing `sv_ttk-2.5.1/sv_ttk.egg-info/PKG-INFO` & `sv_ttk-2.5.2/sv_ttk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sv-ttk
-Version: 2.5.1
+Version: 2.5.2
 Summary: A gorgeous theme for Tkinter, based on Windows 11's UI
 Home-page: https://github.com/rdbende/Sun-Valley-ttk-theme
 Author: rdbende
 Author-email: rdbende@proton.me
 License: MIT
 Project-URL: Source, https://github.com/rdbende/Sun-Valley-ttk-theme
 Project-URL: Documentation, https://github.com/rdbende/Sun-Valley-ttk-theme/wiki
```

