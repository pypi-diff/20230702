# Comparing `tmp/ocp_vscode-1.1.3.tar.gz` & `tmp/ocp_vscode-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ocp_vscode-1.1.3.tar", last modified: Sat Jun 24 13:20:12 2023, max compression
+gzip compressed data, was "ocp_vscode-1.2.0.tar", last modified: Sun Jul  2 15:36:03 2023, max compression
```

## Comparing `ocp_vscode-1.1.3.tar` & `ocp_vscode-1.2.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 bernhard   (501) staff       (20)        0 2023-06-24 13:20:12.407458 ocp_vscode-1.1.3/
--rw-r--r--   0 bernhard   (501) staff       (20)    10938 2023-04-23 10:16:29.000000 ocp_vscode-1.1.3/LICENSE
--rw-r--r--   0 bernhard   (501) staff       (20)      808 2023-06-24 13:20:12.407521 ocp_vscode-1.1.3/PKG-INFO
--rw-r--r--   0 bernhard   (501) staff       (20)     8749 2023-06-24 13:08:20.000000 ocp_vscode-1.1.3/README.md
-drwxr-xr-x   0 bernhard   (501) staff       (20)        0 2023-06-24 13:20:12.406628 ocp_vscode-1.1.3/ocp_vscode/
--rw-r--r--   0 bernhard   (501) staff       (20)      702 2023-06-07 07:17:54.000000 ocp_vscode-1.1.3/ocp_vscode/__init__.py
--rw-r--r--   0 bernhard   (501) staff       (20)     4759 2023-06-07 07:17:54.000000 ocp_vscode-1.1.3/ocp_vscode/animation.py
--rw-r--r--   0 bernhard   (501) staff       (20)    18168 2023-06-19 20:31:17.000000 ocp_vscode-1.1.3/ocp_vscode/colors.py
--rw-r--r--   0 bernhard   (501) staff       (20)     2800 2023-06-07 07:17:54.000000 ocp_vscode-1.1.3/ocp_vscode/comms.py
--rw-r--r--   0 bernhard   (501) staff       (20)     9869 2023-06-16 06:38:23.000000 ocp_vscode-1.1.3/ocp_vscode/config.py
--rw-r--r--   0 bernhard   (501) staff       (20)     4409 2023-06-08 06:20:47.000000 ocp_vscode-1.1.3/ocp_vscode/finder.py
--rw-r--r--   0 bernhard   (501) staff       (20)    24578 2023-06-19 20:31:17.000000 ocp_vscode-1.1.3/ocp_vscode/show.py
-drwxr-xr-x   0 bernhard   (501) staff       (20)        0 2023-06-24 13:20:12.407345 ocp_vscode-1.1.3/ocp_vscode.egg-info/
--rw-r--r--   0 bernhard   (501) staff       (20)      808 2023-06-24 13:20:12.000000 ocp_vscode-1.1.3/ocp_vscode.egg-info/PKG-INFO
--rw-r--r--   0 bernhard   (501) staff       (20)      387 2023-06-24 13:20:12.000000 ocp_vscode-1.1.3/ocp_vscode.egg-info/SOURCES.txt
--rw-r--r--   0 bernhard   (501) staff       (20)        1 2023-06-24 13:20:12.000000 ocp_vscode-1.1.3/ocp_vscode.egg-info/dependency_links.txt
--rw-r--r--   0 bernhard   (501) staff       (20)        1 2023-06-24 13:20:12.000000 ocp_vscode-1.1.3/ocp_vscode.egg-info/not-zip-safe
--rw-r--r--   0 bernhard   (501) staff       (20)       78 2023-06-24 13:20:12.000000 ocp_vscode-1.1.3/ocp_vscode.egg-info/requires.txt
--rw-r--r--   0 bernhard   (501) staff       (20)       11 2023-06-24 13:20:12.000000 ocp_vscode-1.1.3/ocp_vscode.egg-info/top_level.txt
--rw-r--r--   0 bernhard   (501) staff       (20)      900 2023-06-24 13:20:12.407790 ocp_vscode-1.1.3/setup.cfg
--rw-r--r--   0 bernhard   (501) staff       (20)     1229 2023-06-24 13:07:12.000000 ocp_vscode-1.1.3/setup.py
+drwxr-xr-x   0 bernhard   (501) staff       (20)        0 2023-07-02 15:36:03.056060 ocp_vscode-1.2.0/
+-rw-r--r--   0 bernhard   (501) staff       (20)    10938 2023-04-23 10:16:29.000000 ocp_vscode-1.2.0/LICENSE
+-rw-r--r--   0 bernhard   (501) staff       (20)      808 2023-07-02 15:36:03.056114 ocp_vscode-1.2.0/PKG-INFO
+-rw-r--r--   0 bernhard   (501) staff       (20)     9831 2023-07-02 14:30:51.000000 ocp_vscode-1.2.0/README.md
+drwxr-xr-x   0 bernhard   (501) staff       (20)        0 2023-07-02 15:36:03.055303 ocp_vscode-1.2.0/ocp_vscode/
+-rw-r--r--   0 bernhard   (501) staff       (20)      702 2023-06-07 07:17:54.000000 ocp_vscode-1.2.0/ocp_vscode/__init__.py
+-rw-r--r--   0 bernhard   (501) staff       (20)     4759 2023-06-07 07:17:54.000000 ocp_vscode-1.2.0/ocp_vscode/animation.py
+-rw-r--r--   0 bernhard   (501) staff       (20)    18168 2023-06-19 20:31:17.000000 ocp_vscode-1.2.0/ocp_vscode/colors.py
+-rw-r--r--   0 bernhard   (501) staff       (20)     2800 2023-06-07 07:17:54.000000 ocp_vscode-1.2.0/ocp_vscode/comms.py
+-rw-r--r--   0 bernhard   (501) staff       (20)    10270 2023-07-01 11:38:14.000000 ocp_vscode-1.2.0/ocp_vscode/config.py
+-rw-r--r--   0 bernhard   (501) staff       (20)     4409 2023-06-08 06:20:47.000000 ocp_vscode-1.2.0/ocp_vscode/finder.py
+-rw-r--r--   0 bernhard   (501) staff       (20)    25004 2023-07-02 08:06:35.000000 ocp_vscode-1.2.0/ocp_vscode/show.py
+drwxr-xr-x   0 bernhard   (501) staff       (20)        0 2023-07-02 15:36:03.055963 ocp_vscode-1.2.0/ocp_vscode.egg-info/
+-rw-r--r--   0 bernhard   (501) staff       (20)      808 2023-07-02 15:36:03.000000 ocp_vscode-1.2.0/ocp_vscode.egg-info/PKG-INFO
+-rw-r--r--   0 bernhard   (501) staff       (20)      387 2023-07-02 15:36:03.000000 ocp_vscode-1.2.0/ocp_vscode.egg-info/SOURCES.txt
+-rw-r--r--   0 bernhard   (501) staff       (20)        1 2023-07-02 15:36:03.000000 ocp_vscode-1.2.0/ocp_vscode.egg-info/dependency_links.txt
+-rw-r--r--   0 bernhard   (501) staff       (20)        1 2023-07-02 15:36:03.000000 ocp_vscode-1.2.0/ocp_vscode.egg-info/not-zip-safe
+-rw-r--r--   0 bernhard   (501) staff       (20)       78 2023-07-02 15:36:03.000000 ocp_vscode-1.2.0/ocp_vscode.egg-info/requires.txt
+-rw-r--r--   0 bernhard   (501) staff       (20)       11 2023-07-02 15:36:03.000000 ocp_vscode-1.2.0/ocp_vscode.egg-info/top_level.txt
+-rw-r--r--   0 bernhard   (501) staff       (20)      900 2023-07-02 15:36:03.056359 ocp_vscode-1.2.0/setup.cfg
+-rw-r--r--   0 bernhard   (501) staff       (20)     1229 2023-07-02 12:47:33.000000 ocp_vscode-1.2.0/setup.py
```

### Comparing `ocp_vscode-1.1.3/LICENSE` & `ocp_vscode-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ocp_vscode-1.1.3/PKG-INFO` & `ocp_vscode-1.2.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocp_vscode
-Version: 1.1.3
+Version: 1.2.0
 Summary: OCP CAD Viewer for VSCode
 Home-page: https://github.com/bernhard-42/vscode-ocp-cad-viewer
 Author: Bernhard Walter
 Author-email: b_walter@arcor.de
 Keywords: vscode,widgets,CAD,cadquery
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: IPython
```

### Comparing `ocp_vscode-1.1.3/README.md` & `ocp_vscode-1.2.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 ### Breaking changes from v1.0.0
 
 -   IPython and the ipython extensions are not supported any more out of the box. Instead the Microsoft's Jupyter extension with ipykernel is supported. If you have the installation configs in your local VS Code settings.json file, you might want to remove the ipython installation commands.
 -   For the color maps, `CM` is replaced by `ColorMap` (to resolve the conflict with build123d `CM`)
 
 ### Installation
 
-1. Open the VS Code Marketplace, and search and install _OCP CAD Viewer 1.1.3_.
+1. Open the VS Code Marketplace, and search and install _OCP CAD Viewer 1.2.0_.
 
     Afterwards the OCP viewer is available in the VS Code sidebar:
 
     ![](screenshots/ocp_icon.png)
 
 2. Clicking on it shows the OCP CAD Viewer UI:
 
@@ -164,14 +164,25 @@
         # %%
         ```
 
         ![named contexts](./screenshots/context_vars.png)
 
 ## Changes
 
+v1.2.0
+
+-   XYZ labels for orientation marker ([vscode-ocp-cad-viewer issue #13](https://github.com/bernhard-42/vscode-ocp-cad-viewer/issues/13))
+-   Support for metalness and roughness ([three-cad-viewer issue #9](https://github.com/bernhard-42/three-cad-viewer/issues/9))
+-   New "Material" configurator tab in the viewer UI
+-   Fix: OCP_Part can be shown now ([vscode-ocp-cad-viewer issue #20](https://github.com/bernhard-42/vscode-ocp-cad-viewer/issues/20))
+-   Fix: reset_camera respects panning ([vscode-ocp-cad-viewer issue #19](https://github.com/bernhard-42/vscode-ocp-cad-viewer/issues/19))
+-   Fix: `collapse="C"` also collapses single item trees ([vscode-ocp-cad-viewer issue #18](https://github.com/bernhard-42/vscode-ocp-cad-viewer/issues/18))
+-   Fix: Show_all supports having a sketch that uses face as a workplane ([vscode-ocp-cad-viewer issue #17](https://github.com/bernhard-42/vscode-ocp-cad-viewer/issues/17))
+-   Fix: `_config==undefined` is handled properly ([vscode-ocp-cad-viewer issue #12](https://github.com/bernhard-42/vscode-ocp-cad-viewer/issues/12))
+
 v1.1.3
 
 -   Fix racing conditions that prevented having more than one viewer window
 -   No need to add port for next viewer any more. The default port 3939 will be incremented until a free port is found
 -   Use ocp-tessellate 1.1.1 (fixes axis helper scale)
 
 v1.1.2
```

### Comparing `ocp_vscode-1.1.3/ocp_vscode/__init__.py` & `ocp_vscode-1.2.0/ocp_vscode/__init__.py`

 * *Files identical despite different names*

### Comparing `ocp_vscode-1.1.3/ocp_vscode/animation.py` & `ocp_vscode-1.2.0/ocp_vscode/animation.py`

 * *Files identical despite different names*

### Comparing `ocp_vscode-1.1.3/ocp_vscode/colors.py` & `ocp_vscode-1.2.0/ocp_vscode/colors.py`

 * *Files identical despite different names*

### Comparing `ocp_vscode-1.1.3/ocp_vscode/comms.py` & `ocp_vscode-1.2.0/ocp_vscode/comms.py`

 * *Files identical despite different names*

### Comparing `ocp_vscode-1.1.3/ocp_vscode/config.py` & `ocp_vscode-1.2.0/ocp_vscode/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,14 +31,18 @@
     "axes",
     "axes0",
     "black_edges",
     "grid",
     "ortho",
     "transparent",
     "explode",
+    "ambient_intensity",
+    "direct_intensity",
+    "metalness",
+    "roughness",
 ]
 
 CONFIG_WORKSPACE_KEYS = CONFIG_UI_KEYS + [
     # viewer
     "collapse",
     "dark",
     "glass",
@@ -49,23 +53,25 @@
     "up",
     # mouse
     "pan_speed",
     "rotate_speed",
     "zoom_speed",
     # render settings
     "ambient_intensity",
+    "direct_intensity",
+    "metalness",
+    "roughness",
     "angular_tolerance",
     "default_color",
     "default_edgecolor",
     "default_facecolor",
     "default_thickedgecolor",
     "default_vertexcolor",
     "default_opacity",
     "deviation",
-    "direct_intensity",
 ]
 
 CONFIG_CONTROL_KEYS = [
     "edge_accuracy",
     "debug",
     "helper_scale",
     "render_edges",
@@ -90,14 +96,16 @@
     "position",
     "quaternion",
     "target",
     "default_edgecolor",
     "default_opacity",
     "ambient_intensity",
     "direct_intensity",
+    "metalness",
+    "roughness",
     "zoom_speed",
     "pan_speed",
     "rotate_speed",
     "reset_camera",
     "glass",
     "tools",
     "tree_width",
@@ -128,14 +136,16 @@
     position=None,
     quaternion=None,
     target=None,
     default_edgecolor=None,
     default_opacity=None,
     ambient_intensity=None,
     direct_intensity=None,
+    metalness=None,
+    roughness=None,
     zoom_speed=None,
     pan_speed=None,
     rotate_speed=None,
     glass=None,
     tools=None,
     tree_width=None,
     collapse=None,
@@ -182,14 +192,16 @@
     deviation=None,
     angular_tolerance=None,
     edge_accuracy=None,
     default_color=None,
     default_edgecolor=None,
     ambient_intensity=None,
     direct_intensity=None,
+    metalness=None,
+    roughness=None,
     render_edges=None,
     render_normals=None,
     render_mates=None,
     render_joints=None,
     helper_scale=None,
     mate_scale=None,  # DEPRECATED
     debug=None,
@@ -230,16 +242,18 @@
     - Renderer
         deviation:         Shapes: Deviation from linear deflection value (default=0.1)
         angular_tolerance: Shapes: Angular deflection in radians for tessellation (default=0.2)
         edge_accuracy:     Edges: Precision of edge discretization (default: mesh quality / 100)
 
         default_color:     Default mesh color (default=(232, 176, 36))
         default_edgecolor: Default mesh color (default=(128, 128, 128))
-        ambient_intensity  Intensity of ambient ligth (default=1.0)
-        direct_intensity   Intensity of direct lights (default=0.12)
+        ambient_intensity: Intensity of ambient light (default=1.00)
+        direct_intensity:  Intensity of direct light (default=1.10)
+        metalness:         Metalness property of the default material (default=0.30)
+        roughness:         Roughness property of the default material (default=0.65)
 
         render_edges:      Render edges  (default=True)
         render_normals:    Render normals (default=False)
         render_mates:      Render mates for MAssemblies (default=False)
         render_joints:     Render mates for MAssemblies (default=False)
         helper_scale:      Scale of rendered helpers (locations, axis, mates for MAssemblies) (default=1)
```

### Comparing `ocp_vscode-1.1.3/ocp_vscode/finder.py` & `ocp_vscode-1.2.0/ocp_vscode/finder.py`

 * *Files identical despite different names*

### Comparing `ocp_vscode-1.1.3/ocp_vscode/show.py` & `ocp_vscode-1.2.0/ocp_vscode/show.py`

 * *Files 2% similar despite different names*

```diff
@@ -294,14 +294,16 @@
     default_color=None,
     default_edgecolor=None,
     default_facecolor=None,
     default_thickedgecolor=None,
     default_vertexcolor=None,
     ambient_intensity=None,
     direct_intensity=None,
+    metalness=None,
+    roughness=None,
     render_edges=None,
     render_normals=None,
     render_mates=None,
     render_joints=None,
     show_parent=None,
     parallel=None,
     helper_scale=None,
@@ -359,16 +361,18 @@
         edge_accuracy:           Edges: Precision of edge discretization (default: mesh quality / 100)
 
         default_color:           Default mesh color (default=(232, 176, 36))
         default_edgecolor:       Default color of the edges of a mesh (default=#707070)
         default_facecolor:       Default color of the edges of a mesh (default=#ee82ee)
         default_thickedgecolor:  Default color of the edges of a mesh (default=#ba55d3)
         default_vertexcolor:     Default color of the edges of a mesh (default=#ba55d3)
-        ambient_intensity        Intensity of ambient ligth (default=1.0)
-        direct_intensity         Intensity of direct lights (default=0.12)
+        ambient_intensity:       Intensity of ambient light (default=1.00)
+        direct_intensity:        Intensity of direct light (default=1.10)
+        metalness:               Metalness property of the default material (default=0.30)
+        roughness:               Roughness property of the default material (default=0.65)
 
         render_edges:            Render edges  (default=True)
         render_normals:          Render normals (default=False)
         render_mates:            Render mates for MAssemblies (default=False)
         render_joints:           Render build123d joints (default=False)
         parallel:                Tessellate objects in parallel (default=False)
         show_parent:             Render parent of faces, edges or vertices as wireframe
@@ -492,14 +496,16 @@
     edge_accuracy=None,
     default_color=None,
     default_facecolor=None,
     default_thickedgecolor=None,
     default_vertexcolor=None,
     default_edgecolor=None,
     ambient_intensity=None,
+    metalness=None,
+    roughness=None,
     direct_intensity=None,
     render_edges=None,
     render_normals=None,
     render_mates=None,
     render_joints=None,
     parallel=None,
     show_parent=None,
@@ -560,16 +566,19 @@
         edge_accuracy:           Edges: Precision of edge discretization (default: mesh quality / 100)
 
         default_color:           Default mesh color (default=(232, 176, 36))
         default_edgecolor:       Default color of the edges of a mesh (default=(128, 128, 128))
         default_facecolor:       Default color of the edges of a mesh (default=#ee82ee / Violet)
         default_thickedgecolor:  Default color of the edges of a mesh (default=#ba55d3 / MediumOrchid)
         default_vertexcolor:     Default color of the edges of a mesh (default=#ba55d3 / MediumOrchid)
-                                 ambient_intensity  Intensity of ambient ligth (default=1.0)
-        direct_intensity         Intensity of direct lights (default=0.12)
+        ambient_intensity:       Intensity of ambient light (default=1.00)
+        direct_intensity:        Intensity of direct light (default=1.10)
+        metalness:               Metalness property of the default material (default=0.30)
+        roughness:               Roughness property of the default material (default=0.65)
+
 
         render_edges:            Render edges  (default=True)
         render_normals:          Render normals (default=False)
         render_mates:            Render mates for MAssemblies (default=False)
         render_joints:           Render build123d joints (default=False)
         parallel:                Tessellate objects in parallel (default=False)
         show_parent:             Render parent of faces, edges or vertices as wireframe
```

### Comparing `ocp_vscode-1.1.3/ocp_vscode.egg-info/PKG-INFO` & `ocp_vscode-1.2.0/ocp_vscode.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocp-vscode
-Version: 1.1.3
+Version: 1.2.0
 Summary: OCP CAD Viewer for VSCode
 Home-page: https://github.com/bernhard-42/vscode-ocp-cad-viewer
 Author: Bernhard Walter
 Author-email: b_walter@arcor.de
 Keywords: vscode,widgets,CAD,cadquery
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: IPython
```

### Comparing `ocp_vscode-1.1.3/setup.cfg` & `ocp_vscode-1.2.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 1.1.3
+current_version = 1.2.0
 commit = False
 tag = False
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(?P<release>\D*)(?P<build>\d*)
 serialize = 
 	{major}.{minor}.{patch}{release}{build}
 	{major}.{minor}.{patch}
```

### Comparing `ocp_vscode-1.1.3/setup.py` & `ocp_vscode-1.2.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup_args = {
     "name": "ocp_vscode",
-    "version": "1.1.3",
+    "version": "1.2.0",
     "description": "OCP CAD Viewer for VSCode",
     "long_description": "An extension to show OCP cad CAD objects (CadQuery, build123d) in VS Code via pythreejs",
     "include_package_data": True,
     "python_requires": ">=3.9",
     "install_requires": [
         "ocp-tessellate>=1.1.1,<1.2.0",
         "requests",
```

