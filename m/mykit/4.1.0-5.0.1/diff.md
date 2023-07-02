# Comparing `tmp/mykit-4.1.0.tar.gz` & `tmp/mykit-5.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/mykit/mykit/dist/.tmp-p06t2_t1/mykit-4.1.0.tar", last modified: Wed Jun 21 14:18:19 2023, max compression
+gzip compressed data, was "/home/runner/work/mykit/mykit/dist/.tmp-egkgwlc_/mykit-5.0.1.tar", last modified: Sun Jul  2 16:36:42 2023, max compression
```

## Comparing `mykit-4.1.0.tar` & `mykit-5.0.1.tar`

### file list

```diff
@@ -1,46 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:18:19.000000 mykit-4.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-21 14:18:03.000000 mykit-4.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5308 2023-06-21 14:18:19.000000 mykit-4.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-06-21 14:18:03.000000 mykit-4.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:18:19.000000 mykit-4.1.0/mykit/
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-06-21 14:18:03.000000 mykit-4.1.0/mykit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-06-21 14:18:03.000000 mykit-4.1.0/mykit/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:18:19.000000 mykit-4.1.0/mykit/app/
--rw-r--r--   0 runner    (1001) docker     (123)     4850 2023-06-21 14:18:03.000000 mykit-4.1.0/mykit/app/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:18:19.000000 mykit-4.1.0/mykit/app/architecture/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-21 14:18:03.000000 mykit-4.1.0/mykit/app/architecture/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-06-21 14:18:03.000000 mykit-4.1.0/mykit/app/architecture/eventdriven.py
--rw-r--r--   0 runner    (1001) docker     (123)     4613 2023-06-21 14:18:03.000000 mykit-4.1.0/mykit/app/arrow.py
--rw-r--r--   0 runner    (1001) docker     (123)    12806 2023-06-21 14:18:03.000000 mykit-4.1.0/mykit/app/button.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:18:19.000000 mykit-4.1.0/mykit/app/complex/
--rw-r--r--   0 runner    (1001) docker     (123)    21784 2023-06-21 14:18:03.000000 mykit-4.1.0/mykit/app/complex/biplot.py
--rw-r--r--   0 runner    (1001) docker     (123)    17555 2023-06-21 14:18:03.000000 mykit-4.1.0/mykit/app/complex/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     9227 2023-06-21 14:18:03.000000 mykit-4.1.0/mykit/app/label.py
--rw-r--r--   0 runner    (1001) docker     (123)    27474 2023-06-21 14:18:03.000000 mykit-4.1.0/mykit/app/slider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:18:19.000000 mykit-4.1.0/mykit/kit/
--rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-06-21 14:18:03.000000 mykit-4.1.0/mykit/kit/color.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:18:19.000000 mykit-4.1.0/mykit/kit/fast_visualizations/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:18:19.000000 mykit-4.1.0/mykit/kit/fast_visualizations/static/
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-06-21 14:18:03.000000 mykit-4.1.0/mykit/kit/fast_visualizations/static/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     5735 2023-06-21 14:18:03.000000 mykit-4.1.0/mykit/kit/ffmpeg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:18:19.000000 mykit-4.1.0/mykit/kit/keycrate/
--rw-r--r--   0 runner    (1001) docker     (123)     7223 2023-06-21 14:18:03.000000 mykit-4.1.0/mykit/kit/keycrate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-06-21 14:18:03.000000 mykit-4.1.0/mykit/kit/math.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:18:19.000000 mykit-4.1.0/mykit/kit/neuralnet/
--rw-r--r--   0 runner    (1001) docker     (123)     7203 2023-06-21 14:18:03.000000 mykit-4.1.0/mykit/kit/neuralnet/dense.py
--rw-r--r--   0 runner    (1001) docker     (123)    14840 2023-06-21 14:18:03.000000 mykit-4.1.0/mykit/kit/neuralnet/genetic.py
--rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-06-21 14:18:03.000000 mykit-4.1.0/mykit/kit/noise.py
--rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-06-21 14:18:03.000000 mykit-4.1.0/mykit/kit/path.py
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-21 14:18:03.000000 mykit-4.1.0/mykit/kit/text.py
--rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-06-21 14:18:03.000000 mykit-4.1.0/mykit/kit/time.py
--rw-r--r--   0 runner    (1001) docker     (123)     3938 2023-06-21 14:18:03.000000 mykit-4.1.0/mykit/kit/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:18:19.000000 mykit-4.1.0/mykit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5308 2023-06-21 14:18:19.000000 mykit-4.1.0/mykit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-21 14:18:19.000000 mykit-4.1.0/mykit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 14:18:19.000000 mykit-4.1.0/mykit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-21 14:18:19.000000 mykit-4.1.0/mykit.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-21 14:18:19.000000 mykit-4.1.0/mykit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-21 14:18:19.000000 mykit-4.1.0/mykit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-06-21 14:18:03.000000 mykit-4.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-21 14:18:19.000000 mykit-4.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-21 14:18:03.000000 mykit-4.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 16:36:42.000000 mykit-5.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-02 16:36:26.000000 mykit-5.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-07-02 16:36:42.000000 mykit-5.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-07-02 16:36:26.000000 mykit-5.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 16:36:42.000000 mykit-5.0.1/mykit/
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-07-02 16:36:26.000000 mykit-5.0.1/mykit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-02 16:36:26.000000 mykit-5.0.1/mykit/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 16:36:42.000000 mykit-5.0.1/mykit/app/
+-rw-r--r--   0 runner    (1001) docker     (123)     4791 2023-07-02 16:36:26.000000 mykit-5.0.1/mykit/app/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 16:36:42.000000 mykit-5.0.1/mykit/app/architecture/
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-07-02 16:36:26.000000 mykit-5.0.1/mykit/app/architecture/eventdriven.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4613 2023-07-02 16:36:26.000000 mykit-5.0.1/mykit/app/arrow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12806 2023-07-02 16:36:26.000000 mykit-5.0.1/mykit/app/button.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 16:36:42.000000 mykit-5.0.1/mykit/app/complex/
+-rw-r--r--   0 runner    (1001) docker     (123)    21784 2023-07-02 16:36:26.000000 mykit-5.0.1/mykit/app/complex/biplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17555 2023-07-02 16:36:26.000000 mykit-5.0.1/mykit/app/complex/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9227 2023-07-02 16:36:26.000000 mykit-5.0.1/mykit/app/label.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27474 2023-07-02 16:36:26.000000 mykit-5.0.1/mykit/app/slider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 16:36:42.000000 mykit-5.0.1/mykit/kit/
+-rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-07-02 16:36:26.000000 mykit-5.0.1/mykit/kit/color.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 16:36:42.000000 mykit-5.0.1/mykit/kit/fast_visualizations/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 16:36:42.000000 mykit-5.0.1/mykit/kit/fast_visualizations/static/
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-07-02 16:36:26.000000 mykit-5.0.1/mykit/kit/fast_visualizations/static/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5735 2023-07-02 16:36:26.000000 mykit-5.0.1/mykit/kit/ffmpeg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 16:36:42.000000 mykit-5.0.1/mykit/kit/keycrate/
+-rw-r--r--   0 runner    (1001) docker     (123)     7223 2023-07-02 16:36:26.000000 mykit-5.0.1/mykit/kit/keycrate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-07-02 16:36:26.000000 mykit-5.0.1/mykit/kit/math.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 16:36:42.000000 mykit-5.0.1/mykit/kit/neuralnet/
+-rw-r--r--   0 runner    (1001) docker     (123)     7203 2023-07-02 16:36:26.000000 mykit-5.0.1/mykit/kit/neuralnet/dense.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14840 2023-07-02 16:36:26.000000 mykit-5.0.1/mykit/kit/neuralnet/genetic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-07-02 16:36:26.000000 mykit-5.0.1/mykit/kit/noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-07-02 16:36:26.000000 mykit-5.0.1/mykit/kit/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-02 16:36:26.000000 mykit-5.0.1/mykit/kit/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-07-02 16:36:26.000000 mykit-5.0.1/mykit/kit/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3938 2023-07-02 16:36:26.000000 mykit-5.0.1/mykit/kit/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 16:36:42.000000 mykit-5.0.1/mykit/rec/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 16:36:26.000000 mykit-5.0.1/mykit/rec/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 16:36:42.000000 mykit-5.0.1/mykit/web/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 16:36:26.000000 mykit-5.0.1/mykit/web/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 16:36:42.000000 mykit-5.0.1/mykit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-07-02 16:36:42.000000 mykit-5.0.1/mykit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-07-02 16:36:42.000000 mykit-5.0.1/mykit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 16:36:42.000000 mykit-5.0.1/mykit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-02 16:36:42.000000 mykit-5.0.1/mykit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-02 16:36:42.000000 mykit-5.0.1/mykit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-02 16:36:42.000000 mykit-5.0.1/mykit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-07-02 16:36:26.000000 mykit-5.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-02 16:36:42.000000 mykit-5.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-02 16:36:26.000000 mykit-5.0.1/setup.py
```

### Comparing `mykit-4.1.0/LICENSE` & `mykit-5.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mykit-4.1.0/mykit/__init__.py` & `mykit-5.0.1/mykit/__init__.py`

 * *Files identical despite different names*

### Comparing `mykit-4.1.0/mykit/__main__.py` & `mykit-5.0.1/mykit/__main__.py`

 * *Files identical despite different names*

### Comparing `mykit-4.1.0/mykit/app/__init__.py` & `mykit-5.0.1/mykit/app/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,20 @@
 import tkinter as _tk
 from typing import (
     Callable as _Callable,
     List as _List,
-    Optional as _Optional
 )
 
-from mykit.app.architecture import Architecture as _Architecture
-
 from mykit.app.button import Button as _Button
 from mykit.app.label import Label as _Label
 from mykit.app.slider import _Slider
 
-from mykit.app.arrow import Arrow as _Arrow
 from mykit.app.complex.plot import Plot as _Plot
 from mykit.app.complex.biplot import Biplot as _Biplot
+from mykit.app.arrow import Arrow as _Arrow
 
 
 class App:
     """
     A single-page app framework.
     (currently in beta)
 
@@ -27,15 +24,14 @@
     - currently available only in fullscreen mode
     """
 
     def __init__(
         self,
         name: str = 'app',
         bg: str = '#111111',
-        architecture: _Optional[_Architecture] = None
     ) -> None:
 
         self.root = _tk.Tk()
         self.root.attributes('-fullscreen', True)
         self.root.title(name)
 
         ## app's page
@@ -123,14 +119,17 @@
         self._background_processes[every].append(do)
 
     def setup(self, funcs: _List[_Callable[[], None]]):
         self._setup = funcs
 
     def teardown(self, funcs: _List[_Callable[[], None]]):
         self._teardown = funcs
+    
+    def use(self, component: _Callable[[], None], /) -> None:
+        component()
 
     def run(self):
 
         ## <internal>
 
         self.listen(to='left-mouse-press', do=_Button._press_listener)
         self.listen(to='left-mouse-press', do=_Slider._press_listener)
```

### Comparing `mykit-4.1.0/mykit/app/arrow.py` & `mykit-5.0.1/mykit/app/arrow.py`

 * *Files identical despite different names*

### Comparing `mykit-4.1.0/mykit/app/button.py` & `mykit-5.0.1/mykit/app/button.py`

 * *Files identical despite different names*

### Comparing `mykit-4.1.0/mykit/app/complex/biplot.py` & `mykit-5.0.1/mykit/app/complex/biplot.py`

 * *Files identical despite different names*

### Comparing `mykit-4.1.0/mykit/app/complex/plot.py` & `mykit-5.0.1/mykit/app/complex/plot.py`

 * *Files identical despite different names*

### Comparing `mykit-4.1.0/mykit/app/label.py` & `mykit-5.0.1/mykit/app/label.py`

 * *Files identical despite different names*

### Comparing `mykit-4.1.0/mykit/app/slider.py` & `mykit-5.0.1/mykit/app/slider.py`

 * *Files identical despite different names*

### Comparing `mykit-4.1.0/mykit/kit/color.py` & `mykit-5.0.1/mykit/kit/color.py`

 * *Files identical despite different names*

### Comparing `mykit-4.1.0/mykit/kit/fast_visualizations/static/plot.py` & `mykit-5.0.1/mykit/kit/fast_visualizations/static/plot.py`

 * *Files identical despite different names*

### Comparing `mykit-4.1.0/mykit/kit/ffmpeg.py` & `mykit-5.0.1/mykit/kit/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `mykit-4.1.0/mykit/kit/keycrate/__init__.py` & `mykit-5.0.1/mykit/kit/keycrate/__init__.py`

 * *Files identical despite different names*

### Comparing `mykit-4.1.0/mykit/kit/math.py` & `mykit-5.0.1/mykit/kit/math.py`

 * *Files identical despite different names*

### Comparing `mykit-4.1.0/mykit/kit/neuralnet/dense.py` & `mykit-5.0.1/mykit/kit/neuralnet/dense.py`

 * *Files identical despite different names*

### Comparing `mykit-4.1.0/mykit/kit/neuralnet/genetic.py` & `mykit-5.0.1/mykit/kit/neuralnet/genetic.py`

 * *Files identical despite different names*

### Comparing `mykit-4.1.0/mykit/kit/noise.py` & `mykit-5.0.1/mykit/kit/noise.py`

 * *Files identical despite different names*

### Comparing `mykit-4.1.0/mykit/kit/path.py` & `mykit-5.0.1/mykit/kit/path.py`

 * *Files identical despite different names*

### Comparing `mykit-4.1.0/mykit/kit/time.py` & `mykit-5.0.1/mykit/kit/time.py`

 * *Files identical despite different names*

### Comparing `mykit-4.1.0/mykit/kit/utils.py` & `mykit-5.0.1/mykit/kit/utils.py`

 * *Files identical despite different names*

### Comparing `mykit-4.1.0/mykit.egg-info/SOURCES.txt` & `mykit-5.0.1/mykit.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -12,23 +12,24 @@
 mykit.egg-info/requires.txt
 mykit.egg-info/top_level.txt
 mykit/app/__init__.py
 mykit/app/arrow.py
 mykit/app/button.py
 mykit/app/label.py
 mykit/app/slider.py
-mykit/app/architecture/__init__.py
 mykit/app/architecture/eventdriven.py
 mykit/app/complex/biplot.py
 mykit/app/complex/plot.py
 mykit/kit/color.py
 mykit/kit/ffmpeg.py
 mykit/kit/math.py
 mykit/kit/noise.py
 mykit/kit/path.py
 mykit/kit/text.py
 mykit/kit/time.py
 mykit/kit/utils.py
 mykit/kit/fast_visualizations/static/plot.py
 mykit/kit/keycrate/__init__.py
 mykit/kit/neuralnet/dense.py
-mykit/kit/neuralnet/genetic.py
+mykit/kit/neuralnet/genetic.py
+mykit/rec/__init__.py
+mykit/web/__init__.py
```

### Comparing `mykit-4.1.0/pyproject.toml` & `mykit-5.0.1/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,52 +1,47 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "mykit"
-version = "4.1.0"
+version = "5.0.1"
 description = "Python utility library"
 readme = "README.md"
 requires-python = ">=3.8"
 license = {text = "MIT"}
 authors = [
   	{email = "nvfastplease@gmail.com"},
 ]
 keywords = ["python", "toolkit", "mykit"]
 classifiers = [
-	"Topic :: Scientific/Engineering",
     "License :: OSI Approved :: MIT License",
+    "Natural Language :: English",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
-    "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.8",
-    "Programming Language :: Python :: 3.9",
-    "Programming Language :: Python :: 3.10",
-    "Programming Language :: Python :: 3 :: Only",
-    "Natural Language :: English"
+	"Topic :: Scientific/Engineering",
 ]
 dependencies = [
 	"numba>=0.55.2",
-	"numpy>=1.22.4"
+	"numpy>=1.22.4",
 ]
 
 
 [tool.setuptools.packages.find]
 exclude = [
     "assets*",
-    "tests*",
     "demo*",
     "docs*",
+    "tests*",
 ]
 
 
 [project.urls]
-documentation = "https://nvfp.github.io/mykit/docs"
-"report bugs" = "https://github.com/nvfp/mykit/issues"
-repo = "https://github.com/nvfp/mykit"
-changelog = "https://nvfp.github.io/mykit/changelog"
+Documentation = "https://nvfp.github.io/mykit/docs"
+"Report bugs" = "https://github.com/nvfp/mykit/issues"
+Repository = "https://github.com/nvfp/mykit"
+Changelog = "https://nvfp.github.io/mykit/changelog"
 
 
 [project.scripts]
 mykit = "mykit.__main__:main"
```

