# Comparing `tmp/windeklar-0.2.1.tar.gz` & `tmp/windeklar-0.2.2.tar.gz`

## Comparing `windeklar-0.2.1.tar` & `windeklar-0.2.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 windeklar-0.2.1/requirements.txt
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 windeklar-0.2.1/setup.py
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 windeklar-0.2.1/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 windeklar-0.2.1/.idea/.gitignore
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 windeklar-0.2.1/.idea/.name
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 windeklar-0.2.1/.idea/WinDeklar.iml
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 windeklar-0.2.1/.idea/misc.xml
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 windeklar-0.2.1/.idea/modules.xml
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 windeklar-0.2.1/.idea/vcs.xml
--rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 windeklar-0.2.1/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 windeklar-0.2.1/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 windeklar-0.2.1/src/__init__.py
--rwxr-xr-x   0        0        0    16032 2020-02-02 00:00:00.000000 windeklar-0.2.1/src/WinDeklar/QTAux.py
--rw-r--r--   0        0        0    44900 2020-02-02 00:00:00.000000 windeklar-0.2.1/src/WinDeklar/WindowForm.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 windeklar-0.2.1/src/WinDeklar/__init__.py
--rw-r--r--   0        0        0     3724 2020-02-02 00:00:00.000000 windeklar-0.2.1/src/WinDeklar/graph_aux.py
--rw-r--r--   0        0        0     2280 2020-02-02 00:00:00.000000 windeklar-0.2.1/src/WinDeklar/points_box.py
--rw-r--r--   0        0        0     3485 2020-02-02 00:00:00.000000 windeklar-0.2.1/src/WinDeklar/record.py
--rw-r--r--   0        0        0     4241 2020-02-02 00:00:00.000000 windeklar-0.2.1/src/WinDeklar/signal_aux.py
--rw-r--r--   0        0        0     4228 2020-02-02 00:00:00.000000 windeklar-0.2.1/src/WinDeklar/test_animation.py
--rw-r--r--   0        0        0     3376 2020-02-02 00:00:00.000000 windeklar-0.2.1/src/WinDeklar/test_pyqt.py
--rw-r--r--   0        0        0     2467 2020-02-02 00:00:00.000000 windeklar-0.2.1/src/WinDeklar/view_animation.py
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 windeklar-0.2.1/src/WinDeklar/view_animation.yaml
--rw-r--r--   0        0        0     6938 2020-02-02 00:00:00.000000 windeklar-0.2.1/src/WinDeklar/view_example.py
--rw-r--r--   0        0        0     4560 2020-02-02 00:00:00.000000 windeklar-0.2.1/src/WinDeklar/view_example.yaml
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 windeklar-0.2.1/src/WinDeklar/view_simple_graph.py
--rwxr-xr-x   0        0        0     6638 2020-02-02 00:00:00.000000 windeklar-0.2.1/src/WinDeklar/yaml_functions.py
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 windeklar-0.2.1/LICENSE
--rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 windeklar-0.2.1/README.md
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 windeklar-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 windeklar-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 windeklar-0.2.2/requirements.txt
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 windeklar-0.2.2/setup.py
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 windeklar-0.2.2/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 windeklar-0.2.2/.idea/.gitignore
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 windeklar-0.2.2/.idea/.name
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 windeklar-0.2.2/.idea/WinDeklar.iml
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 windeklar-0.2.2/.idea/misc.xml
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 windeklar-0.2.2/.idea/modules.xml
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 windeklar-0.2.2/.idea/vcs.xml
+-rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 windeklar-0.2.2/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 windeklar-0.2.2/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 windeklar-0.2.2/src/__init__.py
+-rwxr-xr-x   0        0        0    16032 2020-02-02 00:00:00.000000 windeklar-0.2.2/src/WinDeklar/QTAux.py
+-rw-r--r--   0        0        0    44876 2020-02-02 00:00:00.000000 windeklar-0.2.2/src/WinDeklar/WindowForm.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 windeklar-0.2.2/src/WinDeklar/__init__.py
+-rw-r--r--   0        0        0     3724 2020-02-02 00:00:00.000000 windeklar-0.2.2/src/WinDeklar/graph_aux.py
+-rw-r--r--   0        0        0     2280 2020-02-02 00:00:00.000000 windeklar-0.2.2/src/WinDeklar/points_box.py
+-rw-r--r--   0        0        0     3485 2020-02-02 00:00:00.000000 windeklar-0.2.2/src/WinDeklar/record.py
+-rw-r--r--   0        0        0     4241 2020-02-02 00:00:00.000000 windeklar-0.2.2/src/WinDeklar/signal_aux.py
+-rw-r--r--   0        0        0     4228 2020-02-02 00:00:00.000000 windeklar-0.2.2/src/WinDeklar/test_animation.py
+-rw-r--r--   0        0        0     3376 2020-02-02 00:00:00.000000 windeklar-0.2.2/src/WinDeklar/test_pyqt.py
+-rw-r--r--   0        0        0     2467 2020-02-02 00:00:00.000000 windeklar-0.2.2/src/WinDeklar/view_animation.py
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 windeklar-0.2.2/src/WinDeklar/view_animation.yaml
+-rw-r--r--   0        0        0     6938 2020-02-02 00:00:00.000000 windeklar-0.2.2/src/WinDeklar/view_example.py
+-rw-r--r--   0        0        0     4547 2020-02-02 00:00:00.000000 windeklar-0.2.2/src/WinDeklar/view_example.yaml
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 windeklar-0.2.2/src/WinDeklar/view_simple_graph.py
+-rwxr-xr-x   0        0        0     6638 2020-02-02 00:00:00.000000 windeklar-0.2.2/src/WinDeklar/yaml_functions.py
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 windeklar-0.2.2/LICENSE
+-rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 windeklar-0.2.2/README.md
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 windeklar-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 windeklar-0.2.2/PKG-INFO
```

### Comparing `windeklar-0.2.1/.github/workflows/python-publish.yml` & `windeklar-0.2.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `windeklar-0.2.1/.idea/inspectionProfiles/Project_Default.xml` & `windeklar-0.2.2/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `windeklar-0.2.1/src/WinDeklar/QTAux.py` & `windeklar-0.2.2/src/WinDeklar/QTAux.py`

 * *Files identical despite different names*

### Comparing `windeklar-0.2.1/src/WinDeklar/WindowForm.py` & `windeklar-0.2.2/src/WinDeklar/WindowForm.py`

 * *Files 1% similar despite different names*

```diff
@@ -187,16 +187,16 @@
         self.set_axis()
 
         FigureCanvas.__init__(self, self.figure)
         self.setParent(self.parent)
 
         FigureCanvas.setSizePolicy(self, QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Expanding)
         FigureCanvas.updateGeometry(self)
-        self.figure.tight_layout()
-        # self.figure.subplots_adjust(left=0.2, bottom=0.2, right=0.8, top=0.8, wspace=0.2, hspace=0.5)
+        # self.figure.tight_layout()
+        self.figure.subplots_adjust(left=0.1, right=0.9, bottom=0.1, top=0.9)
 
         self.figure.canvas.mpl_connect('button_press_event', self.onclick)
         self.figure.canvas.mpl_connect('motion_notify_event', self.on_mouse_move)
 
         dec         = 0.95
         self.text_x = - width * dec
         self.text_y = height  * dec
```

### Comparing `windeklar-0.2.1/src/WinDeklar/graph_aux.py` & `windeklar-0.2.2/src/WinDeklar/graph_aux.py`

 * *Files identical despite different names*

### Comparing `windeklar-0.2.1/src/WinDeklar/points_box.py` & `windeklar-0.2.2/src/WinDeklar/points_box.py`

 * *Files identical despite different names*

### Comparing `windeklar-0.2.1/src/WinDeklar/record.py` & `windeklar-0.2.2/src/WinDeklar/record.py`

 * *Files identical despite different names*

### Comparing `windeklar-0.2.1/src/WinDeklar/signal_aux.py` & `windeklar-0.2.2/src/WinDeklar/signal_aux.py`

 * *Files identical despite different names*

### Comparing `windeklar-0.2.1/src/WinDeklar/test_animation.py` & `windeklar-0.2.2/src/WinDeklar/test_animation.py`

 * *Files identical despite different names*

### Comparing `windeklar-0.2.1/src/WinDeklar/test_pyqt.py` & `windeklar-0.2.2/src/WinDeklar/test_pyqt.py`

 * *Files identical despite different names*

### Comparing `windeklar-0.2.1/src/WinDeklar/view_animation.py` & `windeklar-0.2.2/src/WinDeklar/view_animation.py`

 * *Files identical despite different names*

### Comparing `windeklar-0.2.1/src/WinDeklar/view_animation.yaml` & `windeklar-0.2.2/src/WinDeklar/view_animation.yaml`

 * *Files identical despite different names*

### Comparing `windeklar-0.2.1/src/WinDeklar/view_example.py` & `windeklar-0.2.2/src/WinDeklar/view_example.py`

 * *Files identical despite different names*

### Comparing `windeklar-0.2.1/src/WinDeklar/view_example.yaml` & `windeklar-0.2.2/src/WinDeklar/view_example.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -116,15 +116,15 @@
                     type:    grid
                     subtype: vertical
                     layout:
                       - item:
                           name:    graph1
                           type:    figure
                           subtype: graph
-                          # title:   Graph a function
+                          title:   Graph
                           desc:    graph example
                           x_axis:  {name: 'points'}
                           y_axis:  {name: 'output'}
                           view_size: [100, 10]
                       - item:
                           name:    graph2
                           type:    figure
```

### Comparing `windeklar-0.2.1/src/WinDeklar/view_simple_graph.py` & `windeklar-0.2.2/src/WinDeklar/view_simple_graph.py`

 * *Files identical despite different names*

### Comparing `windeklar-0.2.1/src/WinDeklar/yaml_functions.py` & `windeklar-0.2.2/src/WinDeklar/yaml_functions.py`

 * *Files identical despite different names*

### Comparing `windeklar-0.2.1/LICENSE` & `windeklar-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `windeklar-0.2.1/README.md` & `windeklar-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `windeklar-0.2.1/pyproject.toml` & `windeklar-0.2.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name    = "WinDeklar"
-version = "0.2.1"
+version = "0.2.2"
 authors = [
   { name="Nicolas Jodal", email="jnj@genexus.com" },
 ]
 description = "Create winforms in an easy, declarative way. Specially suited for Robotics applications"
 readme      = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `windeklar-0.2.1/PKG-INFO` & `windeklar-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WinDeklar
-Version: 0.2.1
+Version: 0.2.2
 Summary: Create winforms in an easy, declarative way. Specially suited for Robotics applications
 Project-URL: Homepage, https://github.com/njodal/WinDeklar
 Project-URL: Bug Tracker, https://github.com/njodal/WinDeklar/issues
 Author-email: Nicolas Jodal <jnj@genexus.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

