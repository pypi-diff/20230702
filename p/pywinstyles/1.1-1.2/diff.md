# Comparing `tmp/pywinstyles-1.1.tar.gz` & `tmp/pywinstyles-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pywinstyles-1.1.tar", last modified: Wed Jun 28 08:39:14 2023, max compression
+gzip compressed data, was "pywinstyles-1.2.tar", last modified: Sun Jul  2 11:32:56 2023, max compression
```

## Comparing `pywinstyles-1.1.tar` & `pywinstyles-1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-28 08:39:14.253406 pywinstyles-1.1/
--rw-rw-rw-   0        0        0     7048 2022-11-20 16:16:56.000000 pywinstyles-1.1/LICENSE
--rw-rw-rw-   0        0        0     3163 2023-06-28 08:39:14.253406 pywinstyles-1.1/PKG-INFO
--rw-rw-rw-   0        0        0     2563 2023-06-28 08:38:57.000000 pywinstyles-1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-28 08:39:14.237776 pywinstyles-1.1/pywinstyles/
--rw-rw-rw-   0        0        0      427 2023-06-27 12:16:04.000000 pywinstyles-1.1/pywinstyles/__init__.py
--rw-rw-rw-   0        0        0    10290 2023-06-28 08:36:10.000000 pywinstyles-1.1/pywinstyles/py_win_style.py
-drwxrwxrwx   0        0        0        0 2023-06-28 08:39:14.253406 pywinstyles-1.1/pywinstyles.egg-info/
--rw-rw-rw-   0        0        0     3163 2023-06-28 08:39:14.000000 pywinstyles-1.1/pywinstyles.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      228 2023-06-28 08:39:14.000000 pywinstyles-1.1/pywinstyles.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-28 08:39:14.000000 pywinstyles-1.1/pywinstyles.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-06-28 08:39:14.000000 pywinstyles-1.1/pywinstyles.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      602 2023-06-28 08:39:14.269035 pywinstyles-1.1/setup.cfg
--rw-rw-rw-   0        0        0     1026 2023-06-28 08:31:36.000000 pywinstyles-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-02 11:32:56.543139 pywinstyles-1.2/
+-rw-rw-rw-   0        0        0     7048 2022-11-20 16:16:56.000000 pywinstyles-1.2/LICENSE
+-rw-rw-rw-   0        0        0     3163 2023-07-02 11:32:56.543139 pywinstyles-1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2563 2023-06-28 08:38:57.000000 pywinstyles-1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-02 11:32:56.516406 pywinstyles-1.2/pywinstyles/
+-rw-rw-rw-   0        0        0      427 2023-07-02 11:23:45.000000 pywinstyles-1.2/pywinstyles/__init__.py
+-rw-rw-rw-   0        0        0    10915 2023-07-02 11:29:27.000000 pywinstyles-1.2/pywinstyles/py_win_style.py
+drwxrwxrwx   0        0        0        0 2023-07-02 11:32:56.543139 pywinstyles-1.2/pywinstyles.egg-info/
+-rw-rw-rw-   0        0        0     3163 2023-07-02 11:32:56.000000 pywinstyles-1.2/pywinstyles.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      228 2023-07-02 11:32:56.000000 pywinstyles-1.2/pywinstyles.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-02 11:32:56.000000 pywinstyles-1.2/pywinstyles.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-07-02 11:32:56.000000 pywinstyles-1.2/pywinstyles.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      602 2023-07-02 11:32:56.543139 pywinstyles-1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1026 2023-07-02 11:26:46.000000 pywinstyles-1.2/setup.py
```

### Comparing `pywinstyles-1.1/LICENSE` & `pywinstyles-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pywinstyles-1.1/PKG-INFO` & `pywinstyles-1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywinstyles
-Version: 1.1
+Version: 1.2
 Summary:  Customize window styles in windows 11
 Home-page: https://github.com/Akascape/py-window-styles
 Author: Akash Bora
 License: Creative Commons Zero v1.0 Universal
 Keywords: window-styles,customtkinter,tkinter,python-window,gui,python-gui,pyqt,title-bar,title-bar-color
 Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pywinstyles-1.1/README.md` & `pywinstyles-1.2/README.md`

 * *Files identical despite different names*

### Comparing `pywinstyles-1.1/pywinstyles/py_win_style.py` & `pywinstyles-1.2/pywinstyles/py_win_style.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 Py-Win-Styles
 Author: Akash Bora
-Version: 1.1
+Version: 1.2
 """
 
 try:
     from ctypes import POINTER, pointer, sizeof, windll, Structure, byref, c_int
     from ctypes.wintypes import DWORD, ULONG
 except ImportError:
     raise ImportError("pywinstyles import errror: No windows environment detected!")
@@ -34,17 +34,16 @@
         styles = ["dark", "mica", "aero", "transparent", "acrylic", "win7",
                   "inverse", "popup", "native", "optimised", "light"]
         
         if style not in styles:
             raise ValueError(f"Invalid style name! No such window style exists: {style} \nAvailable styles: {styles}")
             return
         
-        window.update()
-        self.HWND = windll.user32.GetParent(window.winfo_id())
-        
+        self.HWND = detect(window)
+
         if style=="mica":
             ChangeDWMAttrib(self.HWND, 19, c_int(1))
             ChangeDWMAttrib(self.HWND, 1029, c_int(0x01))
         elif style=="optimised":
             ChangeDWMAccent(self.HWND, 30, 1)
         elif style=="dark":
             ChangeDWMAttrib(self.HWND, 19, c_int(1))
@@ -53,39 +52,38 @@
             ChangeDWMAttrib(self.HWND, 19, c_int(0))
             ChangeDWMAttrib(self.HWND, 20, c_int(0))
         elif style=="inverse":
             ChangeDWMAccent(self.HWND, 6, 1)
         elif style=="win7":
             ChangeDWMAccent(self.HWND, 11, 1)
         elif style=="aero":
-            window.config(bg="black")
+            paint(window)
             ChangeDWMAccent(self.HWND, 30, 2)
             ChangeDWMAccent(self.HWND, 19, 3, color=0x000000)
         elif style=="acrylic":
-            window.config(bg="black")
+            paint(window)
             ChangeDWMAccent(self.HWND, 30, 2)
             ChangeDWMAccent(self.HWND, 19, 4, color=0x292929)
         elif style=="popup":
             ChangeDWMAccent(self.HWND, 4, 1)
         elif style=="native":
             ChangeDWMAccent(self.HWND, 30, 2)
             ChangeDWMAccent(self.HWND, 19, 2)
         elif style=="transparent":
-            window.config(bg="black")
+            paint(window)
             ChangeDWMAccent(self.HWND, 30, 2)
             ChangeDWMAccent(self.HWND, 19, 4, color=0)
-      
+     
 class change_header_color():
     """ change the titlebar background color """
     def __init__(self,
                  window,
                  color):
         
-        window.update()
-        self.HWND = windll.user32.GetParent(window.winfo_id())
+        self.HWND = detect(window)
     
         if color=="transparent":
             ChangeDWMAccent(self.HWND, 30, 2)
             return
         else:
             ChangeDWMAccent(self.HWND, 30, 0)
 
@@ -95,29 +93,27 @@
         
             
 class change_border_color():
     """ change the window border color """
     def __init__(self,
                  window,
                  color):
-        
-        window.update()            
-        self.HWND = windll.user32.GetParent(window.winfo_id())
+                   
+        self.HWND = detect(window)
         self.color = DWORD(int(convert_color(color), base=16))
         self.attrib = 34
         ChangeDWMAttrib(self.HWND, self.attrib, self.color)
         
 class change_title_color():
     """ change the title color """
     def __init__(self,
                  window,
                  color):
         
-        window.update()     
-        self.HWND = windll.user32.GetParent(window.winfo_id())
+        self.HWND = detect(window)
         self.color = DWORD(int(convert_color(color), base=16))
         self.attrib = 36
         ChangeDWMAttrib(self.HWND, self.attrib, self.color)
         
 def ChangeDWMAttrib(hWnd: int, attrib: int, color):
     windll.dwmapi.DwmSetWindowAttribute(hWnd, attrib, byref(color), sizeof(c_int))
         
@@ -130,15 +126,38 @@
     winCompAttrData.Data = pointer(accentPolicy)
 
     accentPolicy.AccentState =  state
     if color:
         accentPolicy.GradientColor = color
                                     
     windll.user32.SetWindowCompositionAttribute(hWnd, pointer(winCompAttrData))
-
+    
+def detect(window):
+    """ detect the type of UI library """
+    window_name = str(window).lower()
+    if window_name.startswith("."): # tkinter
+        window.update()
+        return windll.user32.GetParent(window.winfo_id())
+    elif window_name.startswith("<wx"): # wxpython
+        return window.GetHandle()
+    elif window_name.startswith("<py"): # pyqt/pyside
+        return window.winId().__int__()
+    else:
+        return window # other ui windows
+    
+def paint(window):
+    """ paint black color in background """
+    window_name = str(window).lower()
+    if window_name.startswith("."): # tkinter
+        window.config(bg="black")
+    elif window_name.startswith("<wx"): # wxpython
+        window.SetBackgroundColour("black")
+    elif window_name.startswith("<py"): # pyqt/pyside
+        window.setStyleSheet("background-color: transparent;")
+    
 def convert_color(color_name: str):
     """ convert colors to the required API """
     NAMES_TO_HEX = {
         "aliceblue": "#f0f8ff",
         "antiquewhite": "#faebd7",
         "aqua": "#00ffff",
         "aquamarine": "#7fffd4",
```

### Comparing `pywinstyles-1.1/pywinstyles.egg-info/PKG-INFO` & `pywinstyles-1.2/pywinstyles.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywinstyles
-Version: 1.1
+Version: 1.2
 Summary:  Customize window styles in windows 11
 Home-page: https://github.com/Akascape/py-window-styles
 Author: Akash Bora
 License: Creative Commons Zero v1.0 Universal
 Keywords: window-styles,customtkinter,tkinter,python-window,gui,python-gui,pyqt,title-bar,title-bar-color
 Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pywinstyles-1.1/setup.cfg` & `pywinstyles-1.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 7977 696e 7374 796c 6573 0d0a   = pywinstyles..
-00000020: 7665 7273 696f 6e20 3d20 312e 310d 0a64  version = 1.1..d
+00000020: 7665 7273 696f 6e20 3d20 312e 320d 0a64  version = 1.2..d
 00000030: 6573 6372 6970 7469 6f6e 203d 2043 7573  escription = Cus
 00000040: 746f 6d69 7a65 2077 696e 646f 7720 7374  tomize window st
 00000050: 796c 6573 2069 6e20 7769 6e64 6f77 7320  yles in windows 
 00000060: 3131 0d0a 6c6f 6e67 5f64 6573 6372 6970  11..long_descrip
 00000070: 7469 6f6e 203d 2066 696c 653a 2052 4541  tion = file: REA
 00000080: 444d 452e 6d64 0d0a 6c6f 6e67 5f64 6573  DME.md..long_des
 00000090: 6372 6970 7469 6f6e 5f63 6f6e 7465 6e74  cription_content
```

### Comparing `pywinstyles-1.1/setup.py` & `pywinstyles-1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     """Opens and fetches text of long descrition file."""
     with open(path, 'r') as f:
         text = f.read()
     return text
 
 setup(
     name = 'pywinstyles',
-    version = '1.1',
+    version = '1.2',
     description = " Customize window styles in windows 11",
     license = "Creative Commons Zero v1.0 Universal",
     readme = "README.md",
     long_description = get_long_description('README.md'),
     long_description_content_type = "text/markdown",
     author = 'Akash Bora',
     url = "https://github.com/Akascape/py-window-styles",
```

