# Comparing `tmp/ocp_vscode-1.2.0.tar.gz` & `tmp/ocp_vscode-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ocp_vscode-1.2.0.tar", last modified: Sun Jul  2 15:36:03 2023, max compression
+gzip compressed data, was "ocp_vscode-1.2.1.tar", last modified: Sun Jul  2 18:27:51 2023, max compression
```

## Comparing `ocp_vscode-1.2.0.tar` & `ocp_vscode-1.2.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 bernhard   (501) staff       (20)        0 2023-07-02 15:36:03.056060 ocp_vscode-1.2.0/
--rw-r--r--   0 bernhard   (501) staff       (20)    10938 2023-04-23 10:16:29.000000 ocp_vscode-1.2.0/LICENSE
--rw-r--r--   0 bernhard   (501) staff       (20)      808 2023-07-02 15:36:03.056114 ocp_vscode-1.2.0/PKG-INFO
--rw-r--r--   0 bernhard   (501) staff       (20)     9831 2023-07-02 14:30:51.000000 ocp_vscode-1.2.0/README.md
-drwxr-xr-x   0 bernhard   (501) staff       (20)        0 2023-07-02 15:36:03.055303 ocp_vscode-1.2.0/ocp_vscode/
--rw-r--r--   0 bernhard   (501) staff       (20)      702 2023-06-07 07:17:54.000000 ocp_vscode-1.2.0/ocp_vscode/__init__.py
--rw-r--r--   0 bernhard   (501) staff       (20)     4759 2023-06-07 07:17:54.000000 ocp_vscode-1.2.0/ocp_vscode/animation.py
--rw-r--r--   0 bernhard   (501) staff       (20)    18168 2023-06-19 20:31:17.000000 ocp_vscode-1.2.0/ocp_vscode/colors.py
--rw-r--r--   0 bernhard   (501) staff       (20)     2800 2023-06-07 07:17:54.000000 ocp_vscode-1.2.0/ocp_vscode/comms.py
--rw-r--r--   0 bernhard   (501) staff       (20)    10270 2023-07-01 11:38:14.000000 ocp_vscode-1.2.0/ocp_vscode/config.py
--rw-r--r--   0 bernhard   (501) staff       (20)     4409 2023-06-08 06:20:47.000000 ocp_vscode-1.2.0/ocp_vscode/finder.py
--rw-r--r--   0 bernhard   (501) staff       (20)    25004 2023-07-02 08:06:35.000000 ocp_vscode-1.2.0/ocp_vscode/show.py
-drwxr-xr-x   0 bernhard   (501) staff       (20)        0 2023-07-02 15:36:03.055963 ocp_vscode-1.2.0/ocp_vscode.egg-info/
--rw-r--r--   0 bernhard   (501) staff       (20)      808 2023-07-02 15:36:03.000000 ocp_vscode-1.2.0/ocp_vscode.egg-info/PKG-INFO
--rw-r--r--   0 bernhard   (501) staff       (20)      387 2023-07-02 15:36:03.000000 ocp_vscode-1.2.0/ocp_vscode.egg-info/SOURCES.txt
--rw-r--r--   0 bernhard   (501) staff       (20)        1 2023-07-02 15:36:03.000000 ocp_vscode-1.2.0/ocp_vscode.egg-info/dependency_links.txt
--rw-r--r--   0 bernhard   (501) staff       (20)        1 2023-07-02 15:36:03.000000 ocp_vscode-1.2.0/ocp_vscode.egg-info/not-zip-safe
--rw-r--r--   0 bernhard   (501) staff       (20)       78 2023-07-02 15:36:03.000000 ocp_vscode-1.2.0/ocp_vscode.egg-info/requires.txt
--rw-r--r--   0 bernhard   (501) staff       (20)       11 2023-07-02 15:36:03.000000 ocp_vscode-1.2.0/ocp_vscode.egg-info/top_level.txt
--rw-r--r--   0 bernhard   (501) staff       (20)      900 2023-07-02 15:36:03.056359 ocp_vscode-1.2.0/setup.cfg
--rw-r--r--   0 bernhard   (501) staff       (20)     1229 2023-07-02 12:47:33.000000 ocp_vscode-1.2.0/setup.py
+drwxr-xr-x   0 bernhard   (501) staff       (20)        0 2023-07-02 18:27:51.992004 ocp_vscode-1.2.1/
+-rw-r--r--   0 bernhard   (501) staff       (20)    10938 2023-04-23 10:16:29.000000 ocp_vscode-1.2.1/LICENSE
+-rw-r--r--   0 bernhard   (501) staff       (20)      808 2023-07-02 18:27:51.992058 ocp_vscode-1.2.1/PKG-INFO
+-rw-r--r--   0 bernhard   (501) staff       (20)     9831 2023-07-02 18:26:46.000000 ocp_vscode-1.2.1/README.md
+drwxr-xr-x   0 bernhard   (501) staff       (20)        0 2023-07-02 18:27:51.991124 ocp_vscode-1.2.1/ocp_vscode/
+-rw-r--r--   0 bernhard   (501) staff       (20)      702 2023-06-07 07:17:54.000000 ocp_vscode-1.2.1/ocp_vscode/__init__.py
+-rw-r--r--   0 bernhard   (501) staff       (20)     4759 2023-06-07 07:17:54.000000 ocp_vscode-1.2.1/ocp_vscode/animation.py
+-rw-r--r--   0 bernhard   (501) staff       (20)    18168 2023-06-19 20:31:17.000000 ocp_vscode-1.2.1/ocp_vscode/colors.py
+-rw-r--r--   0 bernhard   (501) staff       (20)     2800 2023-06-07 07:17:54.000000 ocp_vscode-1.2.1/ocp_vscode/comms.py
+-rw-r--r--   0 bernhard   (501) staff       (20)    10270 2023-07-01 11:38:14.000000 ocp_vscode-1.2.1/ocp_vscode/config.py
+-rw-r--r--   0 bernhard   (501) staff       (20)     4409 2023-06-08 06:20:47.000000 ocp_vscode-1.2.1/ocp_vscode/finder.py
+-rw-r--r--   0 bernhard   (501) staff       (20)    25004 2023-07-02 08:06:35.000000 ocp_vscode-1.2.1/ocp_vscode/show.py
+drwxr-xr-x   0 bernhard   (501) staff       (20)        0 2023-07-02 18:27:51.991885 ocp_vscode-1.2.1/ocp_vscode.egg-info/
+-rw-r--r--   0 bernhard   (501) staff       (20)      808 2023-07-02 18:27:51.000000 ocp_vscode-1.2.1/ocp_vscode.egg-info/PKG-INFO
+-rw-r--r--   0 bernhard   (501) staff       (20)      387 2023-07-02 18:27:51.000000 ocp_vscode-1.2.1/ocp_vscode.egg-info/SOURCES.txt
+-rw-r--r--   0 bernhard   (501) staff       (20)        1 2023-07-02 18:27:51.000000 ocp_vscode-1.2.1/ocp_vscode.egg-info/dependency_links.txt
+-rw-r--r--   0 bernhard   (501) staff       (20)        1 2023-07-02 18:27:51.000000 ocp_vscode-1.2.1/ocp_vscode.egg-info/not-zip-safe
+-rw-r--r--   0 bernhard   (501) staff       (20)       78 2023-07-02 18:27:51.000000 ocp_vscode-1.2.1/ocp_vscode.egg-info/requires.txt
+-rw-r--r--   0 bernhard   (501) staff       (20)       11 2023-07-02 18:27:51.000000 ocp_vscode-1.2.1/ocp_vscode.egg-info/top_level.txt
+-rw-r--r--   0 bernhard   (501) staff       (20)      900 2023-07-02 18:27:51.992310 ocp_vscode-1.2.1/setup.cfg
+-rw-r--r--   0 bernhard   (501) staff       (20)     1229 2023-07-02 18:26:46.000000 ocp_vscode-1.2.1/setup.py
```

### Comparing `ocp_vscode-1.2.0/LICENSE` & `ocp_vscode-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ocp_vscode-1.2.0/PKG-INFO` & `ocp_vscode-1.2.1/ocp_vscode.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: ocp_vscode
-Version: 1.2.0
+Name: ocp-vscode
+Version: 1.2.1
 Summary: OCP CAD Viewer for VSCode
 Home-page: https://github.com/bernhard-42/vscode-ocp-cad-viewer
 Author: Bernhard Walter
 Author-email: b_walter@arcor.de
 Keywords: vscode,widgets,CAD,cadquery
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: IPython
```

### Comparing `ocp_vscode-1.2.0/README.md` & `ocp_vscode-1.2.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 ### Breaking changes from v1.0.0
 
 -   IPython and the ipython extensions are not supported any more out of the box. Instead the Microsoft's Jupyter extension with ipykernel is supported. If you have the installation configs in your local VS Code settings.json file, you might want to remove the ipython installation commands.
 -   For the color maps, `CM` is replaced by `ColorMap` (to resolve the conflict with build123d `CM`)
 
 ### Installation
 
-1. Open the VS Code Marketplace, and search and install _OCP CAD Viewer 1.2.0_.
+1. Open the VS Code Marketplace, and search and install _OCP CAD Viewer 1.2.1_.
 
     Afterwards the OCP viewer is available in the VS Code sidebar:
 
     ![](screenshots/ocp_icon.png)
 
 2. Clicking on it shows the OCP CAD Viewer UI:
 
@@ -164,15 +164,15 @@
         # %%
         ```
 
         ![named contexts](./screenshots/context_vars.png)
 
 ## Changes
 
-v1.2.0
+v1.2.1
 
 -   XYZ labels for orientation marker ([vscode-ocp-cad-viewer issue #13](https://github.com/bernhard-42/vscode-ocp-cad-viewer/issues/13))
 -   Support for metalness and roughness ([three-cad-viewer issue #9](https://github.com/bernhard-42/three-cad-viewer/issues/9))
 -   New "Material" configurator tab in the viewer UI
 -   Fix: OCP_Part can be shown now ([vscode-ocp-cad-viewer issue #20](https://github.com/bernhard-42/vscode-ocp-cad-viewer/issues/20))
 -   Fix: reset_camera respects panning ([vscode-ocp-cad-viewer issue #19](https://github.com/bernhard-42/vscode-ocp-cad-viewer/issues/19))
 -   Fix: `collapse="C"` also collapses single item trees ([vscode-ocp-cad-viewer issue #18](https://github.com/bernhard-42/vscode-ocp-cad-viewer/issues/18))
```

### Comparing `ocp_vscode-1.2.0/ocp_vscode/__init__.py` & `ocp_vscode-1.2.1/ocp_vscode/__init__.py`

 * *Files identical despite different names*

### Comparing `ocp_vscode-1.2.0/ocp_vscode/animation.py` & `ocp_vscode-1.2.1/ocp_vscode/animation.py`

 * *Files identical despite different names*

### Comparing `ocp_vscode-1.2.0/ocp_vscode/colors.py` & `ocp_vscode-1.2.1/ocp_vscode/colors.py`

 * *Files identical despite different names*

### Comparing `ocp_vscode-1.2.0/ocp_vscode/comms.py` & `ocp_vscode-1.2.1/ocp_vscode/comms.py`

 * *Files identical despite different names*

### Comparing `ocp_vscode-1.2.0/ocp_vscode/config.py` & `ocp_vscode-1.2.1/ocp_vscode/config.py`

 * *Files identical despite different names*

### Comparing `ocp_vscode-1.2.0/ocp_vscode/finder.py` & `ocp_vscode-1.2.1/ocp_vscode/finder.py`

 * *Files identical despite different names*

### Comparing `ocp_vscode-1.2.0/ocp_vscode/show.py` & `ocp_vscode-1.2.1/ocp_vscode/show.py`

 * *Files identical despite different names*

### Comparing `ocp_vscode-1.2.0/ocp_vscode.egg-info/PKG-INFO` & `ocp_vscode-1.2.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: ocp-vscode
-Version: 1.2.0
+Name: ocp_vscode
+Version: 1.2.1
 Summary: OCP CAD Viewer for VSCode
 Home-page: https://github.com/bernhard-42/vscode-ocp-cad-viewer
 Author: Bernhard Walter
 Author-email: b_walter@arcor.de
 Keywords: vscode,widgets,CAD,cadquery
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: IPython
```

### Comparing `ocp_vscode-1.2.0/setup.cfg` & `ocp_vscode-1.2.1/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 1.2.0
+current_version = 1.2.1
 commit = False
 tag = False
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(?P<release>\D*)(?P<build>\d*)
 serialize = 
 	{major}.{minor}.{patch}{release}{build}
 	{major}.{minor}.{patch}
```

### Comparing `ocp_vscode-1.2.0/setup.py` & `ocp_vscode-1.2.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from setuptools import setup, find_packages
 
 setup_args = {
     "name": "ocp_vscode",
-    "version": "1.2.0",
+    "version": "1.2.1",
     "description": "OCP CAD Viewer for VSCode",
     "long_description": "An extension to show OCP cad CAD objects (CadQuery, build123d) in VS Code via pythreejs",
     "include_package_data": True,
     "python_requires": ">=3.9",
     "install_requires": [
-        "ocp-tessellate>=1.1.1,<1.2.0",
+        "ocp-tessellate>=1.1.2,<1.2.1",
         "requests",
         "ipykernel",
         "orjson",
         "websockets>=11.0,<11.1",
     ],
     "packages": find_packages(),
     "zip_safe": False,
```

