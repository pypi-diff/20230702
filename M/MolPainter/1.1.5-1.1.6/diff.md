# Comparing `tmp/MolPainter-1.1.5.tar.gz` & `tmp/MolPainter-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MolPainter-1.1.5.tar", last modified: Thu Apr 13 21:36:14 2023, max compression
+gzip compressed data, was "MolPainter-1.1.6.tar", last modified: Sun Jul  2 00:01:53 2023, max compression
```

## Comparing `MolPainter-1.1.5.tar` & `MolPainter-1.1.6.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 gpantel    (501) staff       (20)        0 2023-04-13 21:36:14.431919 MolPainter-1.1.5/
--rwxr-xr-x   0 gpantel    (501) staff       (20)     1088 2023-03-20 03:43:53.000000 MolPainter-1.1.5/LICENSE
-drwxr-xr-x   0 gpantel    (501) staff       (20)        0 2023-04-13 21:36:14.420398 MolPainter-1.1.5/MolPainter/
--rwxr-xr-x   0 gpantel    (501) staff       (20)    18661 2023-04-13 21:35:34.000000 MolPainter-1.1.5/MolPainter/MolSolvator.py
--rwxr-xr-x   0 gpantel    (501) staff       (20)      149 2023-04-13 21:35:34.000000 MolPainter-1.1.5/MolPainter/__init__.py
--rw-r--r--   0 gpantel    (501) staff       (20)     1288 2023-04-09 23:22:03.000000 MolPainter-1.1.5/MolPainter/about_dialog.py
--rwxr-xr-x   0 gpantel    (501) staff       (20)     5116 2023-03-20 03:43:53.000000 MolPainter-1.1.5/MolPainter/blend_configurator.py
--rwxr-xr-x   0 gpantel    (501) staff       (20)     2915 2023-03-20 03:43:53.000000 MolPainter-1.1.5/MolPainter/cmdbar.py
--rwxr-xr-x   0 gpantel    (501) staff       (20)    22922 2023-03-20 03:43:53.000000 MolPainter-1.1.5/MolPainter/commands.py
--rwxr-xr-x   0 gpantel    (501) staff       (20)     4046 2023-03-20 03:43:53.000000 MolPainter-1.1.5/MolPainter/drawarea.py
--rwxr-xr-x   0 gpantel    (501) staff       (20)    11615 2023-04-13 21:35:30.000000 MolPainter-1.1.5/MolPainter/exporter.py
--rwxr-xr-x   0 gpantel    (501) staff       (20)     2937 2023-03-20 03:43:53.000000 MolPainter-1.1.5/MolPainter/grid_configurator.py
-drwxr-xr-x   0 gpantel    (501) staff       (20)        0 2023-04-13 21:36:14.429607 MolPainter-1.1.5/MolPainter/icons/
--rwxr-xr-x   0 gpantel    (501) staff       (20)     3393 2023-03-20 03:43:53.000000 MolPainter-1.1.5/MolPainter/icons/pencil.png
--rwxr-xr-x   0 gpantel    (501) staff       (20)     3252 2023-03-20 03:43:53.000000 MolPainter-1.1.5/MolPainter/icons/spraycan.png
--rwxr-xr-x   0 gpantel    (501) staff       (20)      694 2023-03-20 03:43:53.000000 MolPainter-1.1.5/MolPainter/icons/square.png
--rwxr-xr-x   0 gpantel    (501) staff       (20)     3405 2023-03-20 03:43:53.000000 MolPainter-1.1.5/MolPainter/icons/zoomin.png
--rwxr-xr-x   0 gpantel    (501) staff       (20)     3395 2023-03-20 03:43:53.000000 MolPainter-1.1.5/MolPainter/icons/zoomout.png
--rwxr-xr-x   0 gpantel    (501) staff       (20)     1985 2023-03-20 03:43:53.000000 MolPainter-1.1.5/MolPainter/layer_configurator.py
--rwxr-xr-x   0 gpantel    (501) staff       (20)    15045 2023-03-20 03:43:53.000000 MolPainter-1.1.5/MolPainter/layer_painter.py
--rwxr-xr-x   0 gpantel    (501) staff       (20)     3474 2023-03-20 03:43:53.000000 MolPainter-1.1.5/MolPainter/molecule_configurator.py
--rwxr-xr-x   0 gpantel    (501) staff       (20)     8057 2023-03-20 03:43:53.000000 MolPainter-1.1.5/MolPainter/molecule_lister.py
--rwxr-xr-x   0 gpantel    (501) staff       (20)     3242 2023-03-20 03:43:53.000000 MolPainter-1.1.5/MolPainter/painter.py
--rwxr-xr-x   0 gpantel    (501) staff       (20)     8507 2023-03-20 03:43:53.000000 MolPainter-1.1.5/MolPainter/proj_saver.py
--rwxr-xr-x   0 gpantel    (501) staff       (20)    10904 2023-03-20 03:43:53.000000 MolPainter-1.1.5/MolPainter/project.py
--rwxr-xr-x   0 gpantel    (501) staff       (20)     3298 2023-03-20 03:43:53.000000 MolPainter-1.1.5/MolPainter/solute_importer.py
--rwxr-xr-x   0 gpantel    (501) staff       (20)     2837 2023-03-20 03:43:53.000000 MolPainter-1.1.5/MolPainter/toolbox.py
-drwxr-xr-x   0 gpantel    (501) staff       (20)        0 2023-04-13 21:36:14.424360 MolPainter-1.1.5/MolPainter.egg-info/
--rw-r--r--   0 gpantel    (501) staff       (20)     4619 2023-04-13 21:36:14.000000 MolPainter-1.1.5/MolPainter.egg-info/PKG-INFO
--rw-r--r--   0 gpantel    (501) staff       (20)      878 2023-04-13 21:36:14.000000 MolPainter-1.1.5/MolPainter.egg-info/SOURCES.txt
--rw-r--r--   0 gpantel    (501) staff       (20)        1 2023-04-13 21:36:14.000000 MolPainter-1.1.5/MolPainter.egg-info/dependency_links.txt
--rw-r--r--   0 gpantel    (501) staff       (20)       97 2023-04-13 21:36:14.000000 MolPainter-1.1.5/MolPainter.egg-info/entry_points.txt
--rw-r--r--   0 gpantel    (501) staff       (20)       28 2023-04-13 21:36:14.000000 MolPainter-1.1.5/MolPainter.egg-info/requires.txt
--rw-r--r--   0 gpantel    (501) staff       (20)       11 2023-04-13 21:36:14.000000 MolPainter-1.1.5/MolPainter.egg-info/top_level.txt
--rw-r--r--   0 gpantel    (501) staff       (20)     4619 2023-04-13 21:36:14.431343 MolPainter-1.1.5/PKG-INFO
--rwxr-xr-x   0 gpantel    (501) staff       (20)     4065 2023-04-13 21:35:34.000000 MolPainter-1.1.5/README.md
--rw-r--r--   0 gpantel    (501) staff       (20)       38 2023-04-13 21:36:14.432083 MolPainter-1.1.5/setup.cfg
--rwxr-xr-x   0 gpantel    (501) staff       (20)      995 2023-03-20 03:43:53.000000 MolPainter-1.1.5/setup.py
-drwxr-xr-x   0 gpantel    (501) staff       (20)        0 2023-04-13 21:36:14.430440 MolPainter-1.1.5/test/
--rw-r--r--   0 gpantel    (501) staff       (20)     3501 2023-04-13 21:35:30.000000 MolPainter-1.1.5/test/test_molpainter.py
+drwxrwxr-x   0 mimashrimp  (1000) mimashrimp  (1000)        0 2023-07-02 00:01:53.906014 MolPainter-1.1.6/
+-rwxr-xr-x   0 mimashrimp  (1000) mimashrimp  (1000)     1088 2022-12-24 18:41:04.000000 MolPainter-1.1.6/LICENSE
+drwxrwxr-x   0 mimashrimp  (1000) mimashrimp  (1000)        0 2023-07-02 00:01:53.906014 MolPainter-1.1.6/MolPainter/
+-rwxr-xr-x   0 mimashrimp  (1000) mimashrimp  (1000)    18661 2023-07-01 23:19:41.000000 MolPainter-1.1.6/MolPainter/MolSolvator.py
+-rwxr-xr-x   0 mimashrimp  (1000) mimashrimp  (1000)      149 2023-07-01 23:54:03.000000 MolPainter-1.1.6/MolPainter/__init__.py
+-rw-rw-r--   0 mimashrimp  (1000) mimashrimp  (1000)     1288 2023-03-20 04:35:02.000000 MolPainter-1.1.6/MolPainter/about_dialog.py
+-rwxr-xr-x   0 mimashrimp  (1000) mimashrimp  (1000)     5116 2022-12-24 18:41:04.000000 MolPainter-1.1.6/MolPainter/blend_configurator.py
+-rwxrwxr-x   0 mimashrimp  (1000) mimashrimp  (1000)     2915 2023-03-19 01:36:09.000000 MolPainter-1.1.6/MolPainter/cmdbar.py
+-rwxrwxr-x   0 mimashrimp  (1000) mimashrimp  (1000)    22926 2023-07-01 23:28:57.000000 MolPainter-1.1.6/MolPainter/commands.py
+-rwxr-xr-x   0 mimashrimp  (1000) mimashrimp  (1000)     4065 2023-07-01 23:44:13.000000 MolPainter-1.1.6/MolPainter/drawarea.py
+-rwxr-xr-x   0 mimashrimp  (1000) mimashrimp  (1000)    11615 2023-07-01 23:19:41.000000 MolPainter-1.1.6/MolPainter/exporter.py
+-rwxr-xr-x   0 mimashrimp  (1000) mimashrimp  (1000)     2937 2022-12-24 18:41:04.000000 MolPainter-1.1.6/MolPainter/grid_configurator.py
+drwxrwxr-x   0 mimashrimp  (1000) mimashrimp  (1000)        0 2023-07-02 00:01:53.906014 MolPainter-1.1.6/MolPainter/icons/
+-rwxr-xr-x   0 mimashrimp  (1000) mimashrimp  (1000)     3393 2022-12-24 18:41:04.000000 MolPainter-1.1.6/MolPainter/icons/pencil.png
+-rwxr-xr-x   0 mimashrimp  (1000) mimashrimp  (1000)     3252 2022-12-24 18:41:04.000000 MolPainter-1.1.6/MolPainter/icons/spraycan.png
+-rwxr-xr-x   0 mimashrimp  (1000) mimashrimp  (1000)      694 2022-12-24 18:41:04.000000 MolPainter-1.1.6/MolPainter/icons/square.png
+-rwxr-xr-x   0 mimashrimp  (1000) mimashrimp  (1000)     3405 2022-12-24 18:41:04.000000 MolPainter-1.1.6/MolPainter/icons/zoomin.png
+-rwxr-xr-x   0 mimashrimp  (1000) mimashrimp  (1000)     3395 2022-12-24 18:41:04.000000 MolPainter-1.1.6/MolPainter/icons/zoomout.png
+-rwxr-xr-x   0 mimashrimp  (1000) mimashrimp  (1000)     1987 2023-07-01 23:23:10.000000 MolPainter-1.1.6/MolPainter/layer_configurator.py
+-rwxrwxr-x   0 mimashrimp  (1000) mimashrimp  (1000)    15045 2023-03-20 00:31:32.000000 MolPainter-1.1.6/MolPainter/layer_painter.py
+-rwxr-xr-x   0 mimashrimp  (1000) mimashrimp  (1000)     3474 2022-12-24 18:41:04.000000 MolPainter-1.1.6/MolPainter/molecule_configurator.py
+-rwxr-xr-x   0 mimashrimp  (1000) mimashrimp  (1000)     8057 2022-12-24 18:41:04.000000 MolPainter-1.1.6/MolPainter/molecule_lister.py
+-rwxr-xr-x   0 mimashrimp  (1000) mimashrimp  (1000)     3242 2022-12-24 18:41:04.000000 MolPainter-1.1.6/MolPainter/painter.py
+-rwxr-xr-x   0 mimashrimp  (1000) mimashrimp  (1000)     8507 2022-12-24 18:41:04.000000 MolPainter-1.1.6/MolPainter/proj_saver.py
+-rwxrwxr-x   0 mimashrimp  (1000) mimashrimp  (1000)    11016 2023-07-01 23:39:49.000000 MolPainter-1.1.6/MolPainter/project.py
+-rwxr-xr-x   0 mimashrimp  (1000) mimashrimp  (1000)     3298 2022-12-24 18:41:04.000000 MolPainter-1.1.6/MolPainter/solute_importer.py
+-rwxr-xr-x   0 mimashrimp  (1000) mimashrimp  (1000)     2837 2022-12-24 18:41:04.000000 MolPainter-1.1.6/MolPainter/toolbox.py
+drwxrwxr-x   0 mimashrimp  (1000) mimashrimp  (1000)        0 2023-07-02 00:01:53.906014 MolPainter-1.1.6/MolPainter.egg-info/
+-rw-rw-r--   0 mimashrimp  (1000) mimashrimp  (1000)     4619 2023-07-02 00:01:53.000000 MolPainter-1.1.6/MolPainter.egg-info/PKG-INFO
+-rw-rw-r--   0 mimashrimp  (1000) mimashrimp  (1000)      878 2023-07-02 00:01:53.000000 MolPainter-1.1.6/MolPainter.egg-info/SOURCES.txt
+-rw-rw-r--   0 mimashrimp  (1000) mimashrimp  (1000)        1 2023-07-02 00:01:53.000000 MolPainter-1.1.6/MolPainter.egg-info/dependency_links.txt
+-rw-rw-r--   0 mimashrimp  (1000) mimashrimp  (1000)       97 2023-07-02 00:01:53.000000 MolPainter-1.1.6/MolPainter.egg-info/entry_points.txt
+-rw-rw-r--   0 mimashrimp  (1000) mimashrimp  (1000)       28 2023-07-02 00:01:53.000000 MolPainter-1.1.6/MolPainter.egg-info/requires.txt
+-rw-rw-r--   0 mimashrimp  (1000) mimashrimp  (1000)       11 2023-07-02 00:01:53.000000 MolPainter-1.1.6/MolPainter.egg-info/top_level.txt
+-rw-rw-r--   0 mimashrimp  (1000) mimashrimp  (1000)     4619 2023-07-02 00:01:53.906014 MolPainter-1.1.6/PKG-INFO
+-rwxr-xr-x   0 mimashrimp  (1000) mimashrimp  (1000)     4065 2023-07-01 23:19:41.000000 MolPainter-1.1.6/README.md
+-rw-rw-r--   0 mimashrimp  (1000) mimashrimp  (1000)       38 2023-07-02 00:01:53.906014 MolPainter-1.1.6/setup.cfg
+-rwxrwxr-x   0 mimashrimp  (1000) mimashrimp  (1000)      995 2023-03-21 04:57:43.000000 MolPainter-1.1.6/setup.py
+drwxrwxr-x   0 mimashrimp  (1000) mimashrimp  (1000)        0 2023-07-02 00:01:53.906014 MolPainter-1.1.6/test/
+-rw-r--r--   0 mimashrimp  (1000) mimashrimp  (1000)     3501 2023-07-01 23:19:41.000000 MolPainter-1.1.6/test/test_molpainter.py
```

### Comparing `MolPainter-1.1.5/LICENSE` & `MolPainter-1.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `MolPainter-1.1.5/MolPainter/MolSolvator.py` & `MolPainter-1.1.6/MolPainter/MolSolvator.py`

 * *Files identical despite different names*

### Comparing `MolPainter-1.1.5/MolPainter/about_dialog.py` & `MolPainter-1.1.6/MolPainter/about_dialog.py`

 * *Files identical despite different names*

### Comparing `MolPainter-1.1.5/MolPainter/blend_configurator.py` & `MolPainter-1.1.6/MolPainter/blend_configurator.py`

 * *Files identical despite different names*

### Comparing `MolPainter-1.1.5/MolPainter/cmdbar.py` & `MolPainter-1.1.6/MolPainter/cmdbar.py`

 * *Files identical despite different names*

### Comparing `MolPainter-1.1.5/MolPainter/commands.py` & `MolPainter-1.1.6/MolPainter/commands.py`

 * *Files 0% similar despite different names*

```diff
@@ -277,22 +277,22 @@
     def layer_modified(self, arg1, arg2, arg3):
         """
         Determine if a layer should be modified with the new settings or if the
         changes should be discarded.
         """
         if self.layeraction.get() == "create":
             self.newlayer.name = self.layername.get()
-            self.newlayer.zdepth = int(self.layerdepth.get())
+            self.newlayer.zdepth = float(self.layerdepth.get())
             self.project.add_layer(self.newlayer)
             self.gui.layer_created(self.newlayer)
             self.layer_settings = None
             self.newlayer = None
         elif self.layeraction.get() == "modify":
             self.newlayer.name = self.layername.get()
-            self.newlayer.zdepth = int(self.layerdepth.get())
+            self.newlayer.zdepth = float(self.layerdepth.get())
             self.gui.layer_modified(self.newlayer)
             self.layer_settings = None
             self.newlayer = None
         elif self.layeraction.get() == "cancel":
             self.layer_settings = None
             self.newlayer = None
```

### Comparing `MolPainter-1.1.5/MolPainter/drawarea.py` & `MolPainter-1.1.6/MolPainter/drawarea.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,16 +26,16 @@
         super().__init__(master, relief="sunken", borderwidth=1)
         self.master = master
         self.grid(column=0, row=0)
 
         self.tabs = ttk.Notebook(self)
         self.tabs.grid(column=0, row=0)
         self.layers = []
-        self.zoomvalues = [5, 7, 10, 15, 20]
-        self.zoom = 2
+        self.zoomvalues = [3, 5, 7, 10, 15, 20, 25, 30, 35, 40]
+        self.zoom = 3
 
         self.tool = 'pencil'
 
         self.molecule = None
 
         self.actions = tk.Menu(self)
         self.actions.add_command(label="Modify Layer", command=self.master.cmds.edit_layer_action)
```

### Comparing `MolPainter-1.1.5/MolPainter/exporter.py` & `MolPainter-1.1.6/MolPainter/exporter.py`

 * *Files identical despite different names*

### Comparing `MolPainter-1.1.5/MolPainter/grid_configurator.py` & `MolPainter-1.1.6/MolPainter/grid_configurator.py`

 * *Files identical despite different names*

### Comparing `MolPainter-1.1.5/MolPainter/icons/pencil.png` & `MolPainter-1.1.6/MolPainter/icons/pencil.png`

 * *Files identical despite different names*

### Comparing `MolPainter-1.1.5/MolPainter/icons/spraycan.png` & `MolPainter-1.1.6/MolPainter/icons/spraycan.png`

 * *Files identical despite different names*

### Comparing `MolPainter-1.1.5/MolPainter/icons/square.png` & `MolPainter-1.1.6/MolPainter/icons/square.png`

 * *Files identical despite different names*

### Comparing `MolPainter-1.1.5/MolPainter/icons/zoomin.png` & `MolPainter-1.1.6/MolPainter/icons/zoomin.png`

 * *Files identical despite different names*

### Comparing `MolPainter-1.1.5/MolPainter/icons/zoomout.png` & `MolPainter-1.1.6/MolPainter/icons/zoomout.png`

 * *Files identical despite different names*

### Comparing `MolPainter-1.1.5/MolPainter/layer_configurator.py` & `MolPainter-1.1.6/MolPainter/layer_configurator.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
     def cancel_action(self):
         self.layeraction.set("cancel")
         self.master.destroy()
 
     def ok_action(self):
         try:
-            int(self.depthvar.get())
+            float(self.depthvar.get())
         except ValueError:
             self.lbl3["text"] = "The z position must be a number"
             return
         self.layeraction.set(self.task)
         self.master.destroy()
 
     def destroy_event(self, event):
```

### Comparing `MolPainter-1.1.5/MolPainter/layer_painter.py` & `MolPainter-1.1.6/MolPainter/layer_painter.py`

 * *Files identical despite different names*

### Comparing `MolPainter-1.1.5/MolPainter/molecule_configurator.py` & `MolPainter-1.1.6/MolPainter/molecule_configurator.py`

 * *Files identical despite different names*

### Comparing `MolPainter-1.1.5/MolPainter/molecule_lister.py` & `MolPainter-1.1.6/MolPainter/molecule_lister.py`

 * *Files identical despite different names*

### Comparing `MolPainter-1.1.5/MolPainter/painter.py` & `MolPainter-1.1.6/MolPainter/painter.py`

 * *Files identical despite different names*

### Comparing `MolPainter-1.1.5/MolPainter/proj_saver.py` & `MolPainter-1.1.6/MolPainter/proj_saver.py`

 * *Files identical despite different names*

### Comparing `MolPainter-1.1.5/MolPainter/project.py` & `MolPainter-1.1.6/MolPainter/project.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import json
 import random
 import numpy as np
 import MDAnalysis as mda
+import warnings
 
 
 class ZLayer():
     def __init__(self):
         self.lattice = None
         self.name = None
         self.zdepth = 0
@@ -248,15 +249,17 @@
             self.solute_z = None
 
     def load_solute(self, should_expand):
         """
         Import a solute into the project. Expands the lattice if needed.
         """
         if self.import_solute is not None:
-            self.solute = mda.Universe(self.import_solute)
+            with warnings.catch_warnings():
+                warnings.simplefilter("ignore")
+                self.solute = mda.Universe(self.import_solute)
         else:
             return
 
         if self.solute_z is not None:
             positions = self.solute.atoms.positions
             solute_indices = list(set(list(np.where(positions[:,2] > self.solute_z-self.lattice_spacing)[0])) & set(list(np.where(positions[:,2] < self.solute_z+self.lattice_spacing)[0])))
             solute_center = np.array([np.mean(positions[:,0]), np.mean(positions[:,1]), np.mean(positions[:,2])])
```

### Comparing `MolPainter-1.1.5/MolPainter/solute_importer.py` & `MolPainter-1.1.6/MolPainter/solute_importer.py`

 * *Files identical despite different names*

### Comparing `MolPainter-1.1.5/MolPainter/toolbox.py` & `MolPainter-1.1.6/MolPainter/toolbox.py`

 * *Files identical despite different names*

### Comparing `MolPainter-1.1.5/MolPainter.egg-info/PKG-INFO` & `MolPainter-1.1.6/MolPainter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MolPainter
-Version: 1.1.5
+Version: 1.1.6
 Summary: Tool for drawing complex planar molecular systems of arbitrary composition and molecule placement
 Home-page: https://github.com/gpantel/MolPainter
 Author: George Pantelopulos, Aaron Liberatore
 License: MIT
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
```

### Comparing `MolPainter-1.1.5/MolPainter.egg-info/SOURCES.txt` & `MolPainter-1.1.6/MolPainter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `MolPainter-1.1.5/PKG-INFO` & `MolPainter-1.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MolPainter
-Version: 1.1.5
+Version: 1.1.6
 Summary: Tool for drawing complex planar molecular systems of arbitrary composition and molecule placement
 Home-page: https://github.com/gpantel/MolPainter
 Author: George Pantelopulos, Aaron Liberatore
 License: MIT
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
```

### Comparing `MolPainter-1.1.5/README.md` & `MolPainter-1.1.6/README.md`

 * *Files identical despite different names*

### Comparing `MolPainter-1.1.5/setup.py` & `MolPainter-1.1.6/setup.py`

 * *Files identical despite different names*

### Comparing `MolPainter-1.1.5/test/test_molpainter.py` & `MolPainter-1.1.6/test/test_molpainter.py`

 * *Files identical despite different names*

