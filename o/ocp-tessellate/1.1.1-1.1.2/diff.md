# Comparing `tmp/ocp_tessellate-1.1.1.tar.gz` & `tmp/ocp_tessellate-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ocp_tessellate-1.1.1.tar", last modified: Sat Jun 24 13:03:12 2023, max compression
+gzip compressed data, was "ocp_tessellate-1.1.2.tar", last modified: Sun Jul  2 15:18:08 2023, max compression
```

## Comparing `ocp_tessellate-1.1.1.tar` & `ocp_tessellate-1.1.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 bernhard   (501) staff       (20)        0 2023-06-24 13:03:12.913377 ocp_tessellate-1.1.1/
--rw-r--r--   0 bernhard   (501) staff       (20)      774 2023-06-24 13:03:12.913434 ocp_tessellate-1.1.1/PKG-INFO
--rw-r--r--   0 bernhard   (501) staff       (20)       17 2023-02-04 10:28:52.000000 ocp_tessellate-1.1.1/README.md
-drwxr-xr-x   0 bernhard   (501) staff       (20)        0 2023-06-24 13:03:12.912602 ocp_tessellate-1.1.1/ocp_tessellate/
--rw-r--r--   0 bernhard   (501) staff       (20)     2926 2023-02-11 19:32:38.000000 ocp_tessellate-1.1.1/ocp_tessellate/__init__.py
--rw-r--r--   0 bernhard   (501) staff       (20)     1123 2023-06-24 13:02:34.000000 ocp_tessellate-1.1.1/ocp_tessellate/_version.py
--rw-r--r--   0 bernhard   (501) staff       (20)    13603 2023-06-24 13:01:17.000000 ocp_tessellate-1.1.1/ocp_tessellate/cad_objects.py
--rw-r--r--   0 bernhard   (501) staff       (20)    30958 2023-06-16 06:31:35.000000 ocp_tessellate-1.1.1/ocp_tessellate/convert.py
--rw-r--r--   0 bernhard   (501) staff       (20)    10521 2023-06-16 06:30:40.000000 ocp_tessellate-1.1.1/ocp_tessellate/defaults.py
--rw-r--r--   0 bernhard   (501) staff       (20)     1301 2023-02-11 19:32:38.000000 ocp_tessellate-1.1.1/ocp_tessellate/mp_tess.py
--rw-r--r--   0 bernhard   (501) staff       (20)     3033 2023-02-11 19:32:38.000000 ocp_tessellate-1.1.1/ocp_tessellate/mp_tessellator.py
--rw-r--r--   0 bernhard   (501) staff       (20)    22358 2023-06-15 21:03:54.000000 ocp_tessellate-1.1.1/ocp_tessellate/ocp_utils.py
--rw-r--r--   0 bernhard   (501) staff       (20)    13370 2023-04-23 10:15:07.000000 ocp_tessellate-1.1.1/ocp_tessellate/stepreader.py
--rw-r--r--   0 bernhard   (501) staff       (20)    13224 2023-04-23 10:15:07.000000 ocp_tessellate-1.1.1/ocp_tessellate/tessellator.py
--rw-r--r--   0 bernhard   (501) staff       (20)     6223 2023-04-29 10:55:18.000000 ocp_tessellate-1.1.1/ocp_tessellate/utils.py
-drwxr-xr-x   0 bernhard   (501) staff       (20)        0 2023-06-24 13:03:12.913244 ocp_tessellate-1.1.1/ocp_tessellate.egg-info/
--rw-r--r--   0 bernhard   (501) staff       (20)      774 2023-06-24 13:03:12.000000 ocp_tessellate-1.1.1/ocp_tessellate.egg-info/PKG-INFO
--rw-r--r--   0 bernhard   (501) staff       (20)      561 2023-06-24 13:03:12.000000 ocp_tessellate-1.1.1/ocp_tessellate.egg-info/SOURCES.txt
--rw-r--r--   0 bernhard   (501) staff       (20)        1 2023-06-24 13:03:12.000000 ocp_tessellate-1.1.1/ocp_tessellate.egg-info/dependency_links.txt
--rw-r--r--   0 bernhard   (501) staff       (20)        1 2023-06-24 13:03:12.000000 ocp_tessellate-1.1.1/ocp_tessellate.egg-info/not-zip-safe
--rw-r--r--   0 bernhard   (501) staff       (20)      102 2023-06-24 13:03:12.000000 ocp_tessellate-1.1.1/ocp_tessellate.egg-info/requires.txt
--rw-r--r--   0 bernhard   (501) staff       (20)       15 2023-06-24 13:03:12.000000 ocp_tessellate-1.1.1/ocp_tessellate.egg-info/top_level.txt
--rw-r--r--   0 bernhard   (501) staff       (20)      671 2023-06-24 13:03:12.913691 ocp_tessellate-1.1.1/setup.cfg
--rw-r--r--   0 bernhard   (501) staff       (20)     1646 2023-06-24 13:02:34.000000 ocp_tessellate-1.1.1/setup.py
+drwxr-xr-x   0 bernhard   (501) staff       (20)        0 2023-07-02 15:18:08.875318 ocp_tessellate-1.1.2/
+-rw-r--r--   0 bernhard   (501) staff       (20)      774 2023-07-02 15:18:08.875367 ocp_tessellate-1.1.2/PKG-INFO
+-rw-r--r--   0 bernhard   (501) staff       (20)       17 2023-02-04 10:28:52.000000 ocp_tessellate-1.1.2/README.md
+drwxr-xr-x   0 bernhard   (501) staff       (20)        0 2023-07-02 15:18:08.874563 ocp_tessellate-1.1.2/ocp_tessellate/
+-rw-r--r--   0 bernhard   (501) staff       (20)     2926 2023-02-11 19:32:38.000000 ocp_tessellate-1.1.2/ocp_tessellate/__init__.py
+-rw-r--r--   0 bernhard   (501) staff       (20)     1123 2023-07-02 08:32:34.000000 ocp_tessellate-1.1.2/ocp_tessellate/_version.py
+-rw-r--r--   0 bernhard   (501) staff       (20)    13603 2023-07-02 09:12:36.000000 ocp_tessellate-1.1.2/ocp_tessellate/cad_objects.py
+-rw-r--r--   0 bernhard   (501) staff       (20)    30968 2023-07-02 08:48:15.000000 ocp_tessellate-1.1.2/ocp_tessellate/convert.py
+-rw-r--r--   0 bernhard   (501) staff       (20)    10521 2023-06-16 06:30:40.000000 ocp_tessellate-1.1.2/ocp_tessellate/defaults.py
+-rw-r--r--   0 bernhard   (501) staff       (20)     1301 2023-02-11 19:32:38.000000 ocp_tessellate-1.1.2/ocp_tessellate/mp_tess.py
+-rw-r--r--   0 bernhard   (501) staff       (20)     3033 2023-02-11 19:32:38.000000 ocp_tessellate-1.1.2/ocp_tessellate/mp_tessellator.py
+-rw-r--r--   0 bernhard   (501) staff       (20)    22511 2023-07-02 08:26:11.000000 ocp_tessellate-1.1.2/ocp_tessellate/ocp_utils.py
+-rw-r--r--   0 bernhard   (501) staff       (20)    13370 2023-04-23 10:15:07.000000 ocp_tessellate-1.1.2/ocp_tessellate/stepreader.py
+-rw-r--r--   0 bernhard   (501) staff       (20)    13224 2023-04-23 10:15:07.000000 ocp_tessellate-1.1.2/ocp_tessellate/tessellator.py
+-rw-r--r--   0 bernhard   (501) staff       (20)     6223 2023-04-29 10:55:18.000000 ocp_tessellate-1.1.2/ocp_tessellate/utils.py
+drwxr-xr-x   0 bernhard   (501) staff       (20)        0 2023-07-02 15:18:08.875220 ocp_tessellate-1.1.2/ocp_tessellate.egg-info/
+-rw-r--r--   0 bernhard   (501) staff       (20)      774 2023-07-02 15:18:08.000000 ocp_tessellate-1.1.2/ocp_tessellate.egg-info/PKG-INFO
+-rw-r--r--   0 bernhard   (501) staff       (20)      561 2023-07-02 15:18:08.000000 ocp_tessellate-1.1.2/ocp_tessellate.egg-info/SOURCES.txt
+-rw-r--r--   0 bernhard   (501) staff       (20)        1 2023-07-02 15:18:08.000000 ocp_tessellate-1.1.2/ocp_tessellate.egg-info/dependency_links.txt
+-rw-r--r--   0 bernhard   (501) staff       (20)        1 2023-07-02 15:18:08.000000 ocp_tessellate-1.1.2/ocp_tessellate.egg-info/not-zip-safe
+-rw-r--r--   0 bernhard   (501) staff       (20)      102 2023-07-02 15:18:08.000000 ocp_tessellate-1.1.2/ocp_tessellate.egg-info/requires.txt
+-rw-r--r--   0 bernhard   (501) staff       (20)       15 2023-07-02 15:18:08.000000 ocp_tessellate-1.1.2/ocp_tessellate.egg-info/top_level.txt
+-rw-r--r--   0 bernhard   (501) staff       (20)      671 2023-07-02 15:18:08.875604 ocp_tessellate-1.1.2/setup.cfg
+-rw-r--r--   0 bernhard   (501) staff       (20)     1646 2023-07-02 08:32:34.000000 ocp_tessellate-1.1.2/setup.py
```

### Comparing `ocp_tessellate-1.1.1/PKG-INFO` & `ocp_tessellate-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocp_tessellate
-Version: 1.1.1
+Version: 1.1.2
 Summary: Tessellate OCP objects
 Home-page: https://github.com/bernhard-42/ocp-tessellate
 Author: Bernhard Walter
 Author-email: b_walter@arcor.de
 Keywords: CAD,cadquery
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: IPython
```

### Comparing `ocp_tessellate-1.1.1/ocp_tessellate/__init__.py` & `ocp_tessellate-1.1.2/ocp_tessellate/__init__.py`

 * *Files identical despite different names*

### Comparing `ocp_tessellate-1.1.1/ocp_tessellate/_version.py` & `ocp_tessellate-1.1.2/ocp_tessellate/_version.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,9 +24,9 @@
     r = re.compile(
         r"(?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)\-{0,1}(?P<release>\D*)(?P<build>\d*)"
     )
     major, minor, patch, release, build = r.match(version).groups()
     return VersionInfo(major, minor, patch, release, build)
 
 
-__version__ = "1.1.1"  # DO NOT EDIT THIS DIRECTLY!  It is managed by bumpversion
+__version__ = "1.1.2"  # DO NOT EDIT THIS DIRECTLY!  It is managed by bumpversion
 __version_info__ = get_version(__version__)
```

### Comparing `ocp_tessellate-1.1.1/ocp_tessellate/cad_objects.py` & `ocp_tessellate-1.1.2/ocp_tessellate/cad_objects.py`

 * *Files identical despite different names*

### Comparing `ocp_tessellate-1.1.1/ocp_tessellate/convert.py` & `ocp_tessellate-1.1.2/ocp_tessellate/convert.py`

 * *Files 0% similar despite different names*

```diff
@@ -877,15 +877,15 @@
 
             elif isinstance(cad_obj, OCP_PartGroup):
                 names = make_unique([obj.name for obj in cad_obj.objects])
                 for name, obj in zip(names, cad_obj.objects):
                     obj.name = name
                 pg.add(cad_obj)
 
-            elif isinstance(cad_obj, (OCP_Faces, OCP_Edges, OCP_Vertices)):
+            elif isinstance(cad_obj, (OCP_Part, OCP_Faces, OCP_Edges, OCP_Vertices)):
                 pg.add(cad_obj)
 
             else:
                 part = conv(cad_obj, obj_name, color, alpha)
                 if part.name is None:
                     part.name = get_object_name(part)
                 pg.add(part)  # no clear way to relocated
```

### Comparing `ocp_tessellate-1.1.1/ocp_tessellate/defaults.py` & `ocp_tessellate-1.1.2/ocp_tessellate/defaults.py`

 * *Files identical despite different names*

### Comparing `ocp_tessellate-1.1.1/ocp_tessellate/mp_tess.py` & `ocp_tessellate-1.1.2/ocp_tessellate/mp_tess.py`

 * *Files identical despite different names*

### Comparing `ocp_tessellate-1.1.1/ocp_tessellate/mp_tessellator.py` & `ocp_tessellate-1.1.2/ocp_tessellate/mp_tessellator.py`

 * *Files identical despite different names*

### Comparing `ocp_tessellate-1.1.1/ocp_tessellate/ocp_utils.py` & `ocp_tessellate-1.1.2/ocp_tessellate/ocp_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -778,14 +778,19 @@
     x = gp_Vec(ax3.XDirection().XYZ())
     y = gp_Vec(ax3.YDirection().XYZ())
     z = gp_Vec(ax3.Direction().XYZ())
     return (o, x, y, z)
 
 
 def is_same_plane(plane1, plane2):
+    if is_topods_face(plane1):
+        plane1 = BRep_Tool.Surface_s(plane1)
+    if is_topods_face(plane2):
+        plane2 = BRep_Tool.Surface_s(plane2)
+
     coordSystem1 = plane1.Position()
     coordSystem2 = plane2.Position()
 
     return (
         coordSystem1.Location().IsEqual(coordSystem2.Location(), 1e-6)
         and coordSystem1.XDirection().IsEqual(coordSystem2.XDirection(), 1e-6)
         and coordSystem1.YDirection().IsEqual(coordSystem2.YDirection(), 1e-6)
```

### Comparing `ocp_tessellate-1.1.1/ocp_tessellate/stepreader.py` & `ocp_tessellate-1.1.2/ocp_tessellate/stepreader.py`

 * *Files identical despite different names*

### Comparing `ocp_tessellate-1.1.1/ocp_tessellate/tessellator.py` & `ocp_tessellate-1.1.2/ocp_tessellate/tessellator.py`

 * *Files identical despite different names*

### Comparing `ocp_tessellate-1.1.1/ocp_tessellate/utils.py` & `ocp_tessellate-1.1.2/ocp_tessellate/utils.py`

 * *Files identical despite different names*

### Comparing `ocp_tessellate-1.1.1/ocp_tessellate.egg-info/PKG-INFO` & `ocp_tessellate-1.1.2/ocp_tessellate.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocp-tessellate
-Version: 1.1.1
+Version: 1.1.2
 Summary: Tessellate OCP objects
 Home-page: https://github.com/bernhard-42/ocp-tessellate
 Author: Bernhard Walter
 Author-email: b_walter@arcor.de
 Keywords: CAD,cadquery
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: IPython
```

### Comparing `ocp_tessellate-1.1.1/ocp_tessellate.egg-info/SOURCES.txt` & `ocp_tessellate-1.1.2/ocp_tessellate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ocp_tessellate-1.1.1/setup.cfg` & `ocp_tessellate-1.1.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 1.1.1
+current_version = 1.1.2
 commit = False
 tag = False
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(?P<release>\D*)(?P<build>\d*)
 serialize = 
 	{major}.{minor}.{patch}{release}{build}
 	{major}.{minor}.{patch}
```

### Comparing `ocp_tessellate-1.1.1/setup.py` & `ocp_tessellate-1.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 LONG_DESCRIPTION = (
     "Tessellate OCP (https://github.com/cadquery/OCP) objects to use with threejs"
 )
 
 setup_args = {
     "name": "ocp_tessellate",
-    "version": "1.1.1",
+    "version": "1.1.2",
     "description": "Tessellate OCP objects",
     "long_description": LONG_DESCRIPTION,
     "include_package_data": True,
     "python_requires": ">=3.9",
     "install_requires": [
         "webcolors~=1.12",
         "numpy",
```

