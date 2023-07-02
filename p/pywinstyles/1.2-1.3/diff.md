# Comparing `tmp/pywinstyles-1.2.tar.gz` & `tmp/pywinstyles-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pywinstyles-1.2.tar", last modified: Sun Jul  2 11:32:56 2023, max compression
+gzip compressed data, was "pywinstyles-1.3.tar", last modified: Sun Jul  2 14:41:09 2023, max compression
```

## Comparing `pywinstyles-1.2.tar` & `pywinstyles-1.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-02 11:32:56.543139 pywinstyles-1.2/
--rw-rw-rw-   0        0        0     7048 2022-11-20 16:16:56.000000 pywinstyles-1.2/LICENSE
--rw-rw-rw-   0        0        0     3163 2023-07-02 11:32:56.543139 pywinstyles-1.2/PKG-INFO
--rw-rw-rw-   0        0        0     2563 2023-06-28 08:38:57.000000 pywinstyles-1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-02 11:32:56.516406 pywinstyles-1.2/pywinstyles/
--rw-rw-rw-   0        0        0      427 2023-07-02 11:23:45.000000 pywinstyles-1.2/pywinstyles/__init__.py
--rw-rw-rw-   0        0        0    10915 2023-07-02 11:29:27.000000 pywinstyles-1.2/pywinstyles/py_win_style.py
-drwxrwxrwx   0        0        0        0 2023-07-02 11:32:56.543139 pywinstyles-1.2/pywinstyles.egg-info/
--rw-rw-rw-   0        0        0     3163 2023-07-02 11:32:56.000000 pywinstyles-1.2/pywinstyles.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      228 2023-07-02 11:32:56.000000 pywinstyles-1.2/pywinstyles.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-02 11:32:56.000000 pywinstyles-1.2/pywinstyles.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-07-02 11:32:56.000000 pywinstyles-1.2/pywinstyles.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      602 2023-07-02 11:32:56.543139 pywinstyles-1.2/setup.cfg
--rw-rw-rw-   0        0        0     1026 2023-07-02 11:26:46.000000 pywinstyles-1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-02 14:41:09.418124 pywinstyles-1.3/
+-rw-rw-rw-   0        0        0     7048 2022-11-20 16:16:56.000000 pywinstyles-1.3/LICENSE
+-rw-rw-rw-   0        0        0     3163 2023-07-02 14:41:09.418124 pywinstyles-1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2563 2023-06-28 08:38:57.000000 pywinstyles-1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-02 14:41:09.418124 pywinstyles-1.3/pywinstyles/
+-rw-rw-rw-   0        0        0      427 2023-07-02 14:39:20.000000 pywinstyles-1.3/pywinstyles/__init__.py
+-rw-rw-rw-   0        0        0    10800 2023-07-02 14:39:13.000000 pywinstyles-1.3/pywinstyles/py_win_style.py
+drwxrwxrwx   0        0        0        0 2023-07-02 14:41:09.418124 pywinstyles-1.3/pywinstyles.egg-info/
+-rw-rw-rw-   0        0        0     3163 2023-07-02 14:41:09.000000 pywinstyles-1.3/pywinstyles.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      228 2023-07-02 14:41:09.000000 pywinstyles-1.3/pywinstyles.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-02 14:41:09.000000 pywinstyles-1.3/pywinstyles.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-07-02 14:41:09.000000 pywinstyles-1.3/pywinstyles.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      602 2023-07-02 14:41:09.433748 pywinstyles-1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1026 2023-07-02 14:39:53.000000 pywinstyles-1.3/setup.py
```

### Comparing `pywinstyles-1.2/LICENSE` & `pywinstyles-1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pywinstyles-1.2/PKG-INFO` & `pywinstyles-1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywinstyles
-Version: 1.2
+Version: 1.3
 Summary:  Customize window styles in windows 11
 Home-page: https://github.com/Akascape/py-window-styles
 Author: Akash Bora
 License: Creative Commons Zero v1.0 Universal
 Keywords: window-styles,customtkinter,tkinter,python-window,gui,python-gui,pyqt,title-bar,title-bar-color
 Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pywinstyles-1.2/README.md` & `pywinstyles-1.3/README.md`

 * *Files identical despite different names*

### Comparing `pywinstyles-1.2/pywinstyles/py_win_style.py` & `pywinstyles-1.3/pywinstyles/py_win_style.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 Py-Win-Styles
 Author: Akash Bora
-Version: 1.2
+Version: 1.3
 """
 
 try:
     from ctypes import POINTER, pointer, sizeof, windll, Structure, byref, c_int
     from ctypes.wintypes import DWORD, ULONG
 except ImportError:
     raise ImportError("pywinstyles import errror: No windows environment detected!")
@@ -129,34 +129,40 @@
     if color:
         accentPolicy.GradientColor = color
                                     
     windll.user32.SetWindowCompositionAttribute(hWnd, pointer(winCompAttrData))
     
 def detect(window):
     """ detect the type of UI library """
-    window_name = str(window).lower()
-    if window_name.startswith("."): # tkinter
+    try: # tkinter
         window.update()
         return windll.user32.GetParent(window.winfo_id())
-    elif window_name.startswith("<wx"): # wxpython
-        return window.GetHandle()
-    elif window_name.startswith("<py"): # pyqt/pyside
+    except: pass
+    try: # pyqt/pyside
         return window.winId().__int__()
-    else:
-        return window # other ui windows
+    except: pass
+    try: # wxpython
+        return window.GetHandle()
+    except: pass
+    return window # other ui windows
     
 def paint(window):
     """ paint black color in background """
-    window_name = str(window).lower()
-    if window_name.startswith("."): # tkinter
+    try: # tkinter
         window.config(bg="black")
-    elif window_name.startswith("<wx"): # wxpython
-        window.SetBackgroundColour("black")
-    elif window_name.startswith("<py"): # pyqt/pyside
+        return
+    except: pass
+    try: # pyqt/pyside
         window.setStyleSheet("background-color: transparent;")
+        return
+    except: pass
+    try: # wxpython
+        window.SetBackgroundColour("black")
+        return
+    except: pass
     
 def convert_color(color_name: str):
     """ convert colors to the required API """
     NAMES_TO_HEX = {
         "aliceblue": "#f0f8ff",
         "antiquewhite": "#faebd7",
         "aqua": "#00ffff",
```

### Comparing `pywinstyles-1.2/pywinstyles.egg-info/PKG-INFO` & `pywinstyles-1.3/pywinstyles.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywinstyles
-Version: 1.2
+Version: 1.3
 Summary:  Customize window styles in windows 11
 Home-page: https://github.com/Akascape/py-window-styles
 Author: Akash Bora
 License: Creative Commons Zero v1.0 Universal
 Keywords: window-styles,customtkinter,tkinter,python-window,gui,python-gui,pyqt,title-bar,title-bar-color
 Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pywinstyles-1.2/setup.cfg` & `pywinstyles-1.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 7977 696e 7374 796c 6573 0d0a   = pywinstyles..
-00000020: 7665 7273 696f 6e20 3d20 312e 320d 0a64  version = 1.2..d
+00000020: 7665 7273 696f 6e20 3d20 312e 330d 0a64  version = 1.3..d
 00000030: 6573 6372 6970 7469 6f6e 203d 2043 7573  escription = Cus
 00000040: 746f 6d69 7a65 2077 696e 646f 7720 7374  tomize window st
 00000050: 796c 6573 2069 6e20 7769 6e64 6f77 7320  yles in windows 
 00000060: 3131 0d0a 6c6f 6e67 5f64 6573 6372 6970  11..long_descrip
 00000070: 7469 6f6e 203d 2066 696c 653a 2052 4541  tion = file: REA
 00000080: 444d 452e 6d64 0d0a 6c6f 6e67 5f64 6573  DME.md..long_des
 00000090: 6372 6970 7469 6f6e 5f63 6f6e 7465 6e74  cription_content
```

### Comparing `pywinstyles-1.2/setup.py` & `pywinstyles-1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     """Opens and fetches text of long descrition file."""
     with open(path, 'r') as f:
         text = f.read()
     return text
 
 setup(
     name = 'pywinstyles',
-    version = '1.2',
+    version = '1.3',
     description = " Customize window styles in windows 11",
     license = "Creative Commons Zero v1.0 Universal",
     readme = "README.md",
     long_description = get_long_description('README.md'),
     long_description_content_type = "text/markdown",
     author = 'Akash Bora',
     url = "https://github.com/Akascape/py-window-styles",
```

