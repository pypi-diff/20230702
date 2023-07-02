# Comparing `tmp/windeklar-0.2.tar.gz` & `tmp/windeklar-0.2.1.tar.gz`

## Comparing `windeklar-0.2.tar` & `windeklar-0.2.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 windeklar-0.2/requirements.txt
--rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 windeklar-0.2/setup.py
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 windeklar-0.2/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 windeklar-0.2/.idea/.gitignore
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 windeklar-0.2/.idea/.name
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 windeklar-0.2/.idea/WinDeklar.iml
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 windeklar-0.2/.idea/misc.xml
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 windeklar-0.2/.idea/modules.xml
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 windeklar-0.2/.idea/vcs.xml
--rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 windeklar-0.2/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 windeklar-0.2/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 windeklar-0.2/src/__init__.py
--rwxr-xr-x   0        0        0    15884 2020-02-02 00:00:00.000000 windeklar-0.2/src/WinDeklar/QTAux.py
--rw-r--r--   0        0        0    44640 2020-02-02 00:00:00.000000 windeklar-0.2/src/WinDeklar/WindowForm.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 windeklar-0.2/src/WinDeklar/__init__.py
--rw-r--r--   0        0        0     3724 2020-02-02 00:00:00.000000 windeklar-0.2/src/WinDeklar/graph_aux.py
--rw-r--r--   0        0        0     2280 2020-02-02 00:00:00.000000 windeklar-0.2/src/WinDeklar/points_box.py
--rw-r--r--   0        0        0     3485 2020-02-02 00:00:00.000000 windeklar-0.2/src/WinDeklar/record.py
--rw-r--r--   0        0        0     4241 2020-02-02 00:00:00.000000 windeklar-0.2/src/WinDeklar/signal_aux.py
--rw-r--r--   0        0        0     4228 2020-02-02 00:00:00.000000 windeklar-0.2/src/WinDeklar/test_animation.py
--rw-r--r--   0        0        0     3376 2020-02-02 00:00:00.000000 windeklar-0.2/src/WinDeklar/test_pyqt.py
--rw-r--r--   0        0        0     2467 2020-02-02 00:00:00.000000 windeklar-0.2/src/WinDeklar/view_animation.py
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 windeklar-0.2/src/WinDeklar/view_animation.yaml
--rw-r--r--   0        0        0     6973 2020-02-02 00:00:00.000000 windeklar-0.2/src/WinDeklar/view_example.py
--rw-r--r--   0        0        0     4525 2020-02-02 00:00:00.000000 windeklar-0.2/src/WinDeklar/view_example.yaml
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 windeklar-0.2/src/WinDeklar/view_simple_graph.py
--rwxr-xr-x   0        0        0     6638 2020-02-02 00:00:00.000000 windeklar-0.2/src/WinDeklar/yaml_functions.py
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 windeklar-0.2/LICENSE
--rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 windeklar-0.2/README.md
--rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 windeklar-0.2/pyproject.toml
--rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 windeklar-0.2/PKG-INFO
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 windeklar-0.2.1/requirements.txt
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 windeklar-0.2.1/setup.py
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 windeklar-0.2.1/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 windeklar-0.2.1/.idea/.gitignore
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 windeklar-0.2.1/.idea/.name
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 windeklar-0.2.1/.idea/WinDeklar.iml
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 windeklar-0.2.1/.idea/misc.xml
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 windeklar-0.2.1/.idea/modules.xml
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 windeklar-0.2.1/.idea/vcs.xml
+-rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 windeklar-0.2.1/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 windeklar-0.2.1/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 windeklar-0.2.1/src/__init__.py
+-rwxr-xr-x   0        0        0    16032 2020-02-02 00:00:00.000000 windeklar-0.2.1/src/WinDeklar/QTAux.py
+-rw-r--r--   0        0        0    44900 2020-02-02 00:00:00.000000 windeklar-0.2.1/src/WinDeklar/WindowForm.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 windeklar-0.2.1/src/WinDeklar/__init__.py
+-rw-r--r--   0        0        0     3724 2020-02-02 00:00:00.000000 windeklar-0.2.1/src/WinDeklar/graph_aux.py
+-rw-r--r--   0        0        0     2280 2020-02-02 00:00:00.000000 windeklar-0.2.1/src/WinDeklar/points_box.py
+-rw-r--r--   0        0        0     3485 2020-02-02 00:00:00.000000 windeklar-0.2.1/src/WinDeklar/record.py
+-rw-r--r--   0        0        0     4241 2020-02-02 00:00:00.000000 windeklar-0.2.1/src/WinDeklar/signal_aux.py
+-rw-r--r--   0        0        0     4228 2020-02-02 00:00:00.000000 windeklar-0.2.1/src/WinDeklar/test_animation.py
+-rw-r--r--   0        0        0     3376 2020-02-02 00:00:00.000000 windeklar-0.2.1/src/WinDeklar/test_pyqt.py
+-rw-r--r--   0        0        0     2467 2020-02-02 00:00:00.000000 windeklar-0.2.1/src/WinDeklar/view_animation.py
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 windeklar-0.2.1/src/WinDeklar/view_animation.yaml
+-rw-r--r--   0        0        0     6938 2020-02-02 00:00:00.000000 windeklar-0.2.1/src/WinDeklar/view_example.py
+-rw-r--r--   0        0        0     4560 2020-02-02 00:00:00.000000 windeklar-0.2.1/src/WinDeklar/view_example.yaml
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 windeklar-0.2.1/src/WinDeklar/view_simple_graph.py
+-rwxr-xr-x   0        0        0     6638 2020-02-02 00:00:00.000000 windeklar-0.2.1/src/WinDeklar/yaml_functions.py
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 windeklar-0.2.1/LICENSE
+-rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 windeklar-0.2.1/README.md
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 windeklar-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 windeklar-0.2.1/PKG-INFO
```

### Comparing `windeklar-0.2/.github/workflows/python-publish.yml` & `windeklar-0.2.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `windeklar-0.2/.idea/inspectionProfiles/Project_Default.xml` & `windeklar-0.2.1/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `windeklar-0.2/src/WinDeklar/QTAux.py` & `windeklar-0.2.1/src/WinDeklar/QTAux.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,14 +118,19 @@
     def refresh(self):
         # abstract method
         pass
 
     def set_ename(self, new_ename):
         self.ename = new_ename
 
+    def set_fixed_width(self, width):
+        _, widget = self.get_widget()
+        if widget is not None:
+            widget.setFixedWidth(width)
+
 
 class EnumCombo(ScreenControl):
     def __init__(self, name, title, bound, enum, action, layout, tooltip=None):
     
         self.enum  = enum
         self.combo = QtWidgets.QComboBox(None)
         for member in self.enum:
```

### Comparing `windeklar-0.2/src/WinDeklar/WindowForm.py` & `windeklar-0.2.1/src/WinDeklar/WindowForm.py`

 * *Files 0% similar despite different names*

```diff
@@ -188,14 +188,15 @@
 
         FigureCanvas.__init__(self, self.figure)
         self.setParent(self.parent)
 
         FigureCanvas.setSizePolicy(self, QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Expanding)
         FigureCanvas.updateGeometry(self)
         self.figure.tight_layout()
+        # self.figure.subplots_adjust(left=0.2, bottom=0.2, right=0.8, top=0.8, wspace=0.2, hspace=0.5)
 
         self.figure.canvas.mpl_connect('button_press_event', self.onclick)
         self.figure.canvas.mpl_connect('motion_notify_event', self.on_mouse_move)
 
         dec         = 0.95
         self.text_x = - width * dec
         self.text_y = height  * dec
@@ -930,14 +931,19 @@
     else:
         raise Exception('Subtype %s not implemented for %s' % (subtype, type))
     controls = add_controls_to_window(layout, layout_config, window)
     if not row_col:
         father_layout.addLayout(layout)
     else:
         father_layout.addLayout(layout, row_col[0], row_col[1])
+
+    fixed_width = layout_config.get('width', None)
+    if fixed_width is not None:
+        [control.set_fixed_width(fixed_width) for control in controls]
+
     return layout, controls
 
 
 def set_figure_layout(father_layout, figure_config, window):
     size     = window.provider.view_size() if window.provider is not None else (1, 0)
     fig_view = FigureView(window, figure_config, size=size)
     father_layout.addWidget(fig_view)
```

### Comparing `windeklar-0.2/src/WinDeklar/graph_aux.py` & `windeklar-0.2.1/src/WinDeklar/graph_aux.py`

 * *Files identical despite different names*

### Comparing `windeklar-0.2/src/WinDeklar/points_box.py` & `windeklar-0.2.1/src/WinDeklar/points_box.py`

 * *Files identical despite different names*

### Comparing `windeklar-0.2/src/WinDeklar/record.py` & `windeklar-0.2.1/src/WinDeklar/record.py`

 * *Files identical despite different names*

### Comparing `windeklar-0.2/src/WinDeklar/signal_aux.py` & `windeklar-0.2.1/src/WinDeklar/signal_aux.py`

 * *Files identical despite different names*

### Comparing `windeklar-0.2/src/WinDeklar/test_animation.py` & `windeklar-0.2.1/src/WinDeklar/test_animation.py`

 * *Files identical despite different names*

### Comparing `windeklar-0.2/src/WinDeklar/test_pyqt.py` & `windeklar-0.2.1/src/WinDeklar/test_pyqt.py`

 * *Files identical despite different names*

### Comparing `windeklar-0.2/src/WinDeklar/view_animation.py` & `windeklar-0.2.1/src/WinDeklar/view_animation.py`

 * *Files identical despite different names*

### Comparing `windeklar-0.2/src/WinDeklar/view_animation.yaml` & `windeklar-0.2.1/src/WinDeklar/view_animation.yaml`

 * *Files identical despite different names*

### Comparing `windeklar-0.2/src/WinDeklar/view_example.py` & `windeklar-0.2.1/src/WinDeklar/view_example.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 #!/usr/bin/env python
 
 import sys
 import time
 
-import matplotlib.lines as mlines
-
 import WinDeklar.WindowForm as WinForm
 import WinDeklar.graph_aux as ga
 import WinDeklar.QTAux as QTAux
 import WinDeklar.record as rc
 import WinDeklar.yaml_functions as ya
```

### Comparing `windeklar-0.2/src/WinDeklar/view_example.yaml` & `windeklar-0.2.1/src/WinDeklar/view_example.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -73,14 +73,15 @@
               type:    grid
               subtype: horizontal
               layout:
                 - item:
                     name:    controls
                     type:    grid
                     subtype: vertical
+                    width:   300
                     desc:    panel is composed of two sides, the one at the left has controls, at the right a Figure to show a grapth
                     controls:
                       - control:
                           name:    graph_type
                           title:   Graph Type
                           type:    Combo
                           values:  [Sine, Cosine, Random, Other]
@@ -115,15 +116,15 @@
                     type:    grid
                     subtype: vertical
                     layout:
                       - item:
                           name:    graph1
                           type:    figure
                           subtype: graph
-                          title:   Graph a function
+                          # title:   Graph a function
                           desc:    graph example
                           x_axis:  {name: 'points'}
                           y_axis:  {name: 'output'}
                           view_size: [100, 10]
                       - item:
                           name:    graph2
                           type:    figure
```

### Comparing `windeklar-0.2/src/WinDeklar/view_simple_graph.py` & `windeklar-0.2.1/src/WinDeklar/view_simple_graph.py`

 * *Files identical despite different names*

### Comparing `windeklar-0.2/src/WinDeklar/yaml_functions.py` & `windeklar-0.2.1/src/WinDeklar/yaml_functions.py`

 * *Files identical despite different names*

### Comparing `windeklar-0.2/LICENSE` & `windeklar-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `windeklar-0.2/README.md` & `windeklar-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `windeklar-0.2/pyproject.toml` & `windeklar-0.2.1/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name    = "WinDeklar"
-version = "0.2"
+version = "0.2.1"
 authors = [
   { name="Nicolas Jodal", email="jnj@genexus.com" },
 ]
 description = "Create winforms in an easy, declarative way. Specially suited for Robotics applications"
 readme      = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `windeklar-0.2/PKG-INFO` & `windeklar-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WinDeklar
-Version: 0.2
+Version: 0.2.1
 Summary: Create winforms in an easy, declarative way. Specially suited for Robotics applications
 Project-URL: Homepage, https://github.com/njodal/WinDeklar
 Project-URL: Bug Tracker, https://github.com/njodal/WinDeklar/issues
 Author-email: Nicolas Jodal <jnj@genexus.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

