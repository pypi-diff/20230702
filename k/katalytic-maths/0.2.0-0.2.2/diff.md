# Comparing `tmp/katalytic-maths-0.2.0.tar.gz` & `tmp/katalytic_maths-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "katalytic-maths-0.2.0.tar", last modified: Sat May  6 04:59:10 2023, max compression
+gzip compressed data, was "katalytic_maths-0.2.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `katalytic-maths-0.2.0.tar` & `katalytic_maths-0.2.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      109 2023-04-09 19:59:19.451546 katalytic-maths-0.2.0/.coveragerc
--rw-r--r--   0        0        0      641 2023-04-05 07:07:35.618314 katalytic-maths-0.2.0/.gitignore
--rw-r--r--   0        0        0     3242 2023-05-05 03:59:34.970335 katalytic-maths-0.2.0/.gitlab-ci.yml
--rw-r--r--   0        0        0     1181 2023-05-06 04:58:46.888399 katalytic-maths-0.2.0/CHANGELOG.md
--rw-r--r--   0        0        0     1066 2023-04-06 18:07:34.500276 katalytic-maths-0.2.0/LICENSE.txt
--rw-r--r--   0        0        0     1819 2023-05-03 04:08:20.003050 katalytic-maths-0.2.0/README.md
--rw-r--r--   0        0        0     1281 2023-05-06 04:58:46.852399 katalytic-maths-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     3381 2023-05-05 17:42:36.449173 katalytic-maths-0.2.0/src/katalytic/maths/__init__.py
--rw-r--r--   0        0        0    11398 2023-05-06 04:43:38.312592 katalytic-maths-0.2.0/src/katalytic/maths/bboxes.py
--rw-r--r--   0        0        0    13156 2023-05-06 04:53:18.580396 katalytic-maths-0.2.0/tests/test_bboxes.py
--rw-r--r--   0        0        0     3868 2023-05-02 05:45:43.867514 katalytic-maths-0.2.0/tests/test_maths.py
--rw-r--r--   0        0        0     2986 1970-01-01 00:00:00.000000 katalytic-maths-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      109 2023-04-09 19:59:19.451546 katalytic_maths-0.2.2/.coveragerc
+-rw-r--r--   0        0        0      651 2023-07-02 15:15:58.148082 katalytic_maths-0.2.2/.gitignore
+-rw-r--r--   0        0        0     3242 2023-05-05 03:59:34.970335 katalytic_maths-0.2.2/.gitlab-ci.yml
+-rw-r--r--   0        0        0     2553 2023-07-02 15:16:31.328359 katalytic_maths-0.2.2/CHANGELOG.md
+-rw-r--r--   0        0        0     1066 2023-04-06 18:07:34.500276 katalytic_maths-0.2.2/LICENSE.txt
+-rw-r--r--   0        0        0     1849 2023-05-14 08:37:35.659138 katalytic_maths-0.2.2/README.md
+-rw-r--r--   0        0        0     1281 2023-07-02 15:16:31.328359 katalytic_maths-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     5930 2023-06-27 18:19:02.980211 katalytic_maths-0.2.2/src/katalytic/maths/__init__.py
+-rw-r--r--   0        0        0    22812 2023-07-02 15:11:49.214051 katalytic_maths-0.2.2/src/katalytic/maths/bboxes.py
+-rw-r--r--   0        0        0    13200 2023-07-02 14:56:46.580225 katalytic_maths-0.2.2/tests/test_bboxes.py
+-rw-r--r--   0        0        0     3868 2023-05-02 05:45:43.867514 katalytic_maths-0.2.2/tests/test_maths.py
+-rw-r--r--   0        0        0     3016 1970-01-01 00:00:00.000000 katalytic_maths-0.2.2/PKG-INFO
```

### Comparing `katalytic-maths-0.2.0/.gitignore` & `katalytic_maths-0.2.2/.gitignore`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 #  Temporary and binary files
+*sandbox*
 **/tmp
 *.tmp
 *~
 *.py[cod]
 *.so
 *.cfg
 !.isort.cfg
```

### Comparing `katalytic-maths-0.2.0/.gitlab-ci.yml` & `katalytic_maths-0.2.2/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `katalytic-maths-0.2.0/LICENSE.txt` & `katalytic_maths-0.2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `katalytic-maths-0.2.0/README.md` & `katalytic_maths-0.2.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+# Not fit for public use yet
+
 ## Description
 TODO: Let people know what your project can do specifically. Provide context and add a link to any reference visitors might be unfamiliar with. A list of Features or a Background subsection can also be added here. If there are alternatives to your project, this is a good place to list differentiating factors.
 
 [![version](https://img.shields.io/pypi/v/katalytic-maths)](https://pypi.org/project/katalytic-maths/)
 [![tests](https://gitlab.com/katalytic/katalytic-maths/badges/main/pipeline.svg?key_text=tests&key_width=38)](https://gitlab.com/katalytic/katalytic-maths/-/commits/main)
 [![coverage](https://gitlab.com/katalytic/katalytic-maths/badges/main/coverage.svg)](https://gitlab.com/katalytic/katalytic-maths/-/commits/main)
 [![docs](https://img.shields.io/readthedocs/katalytic-maths.svg)](https://katalytic-maths.readthedocs.io/en/latest/)
```

### Comparing `katalytic-maths-0.2.0/pyproject.toml` & `katalytic_maths-0.2.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "katalytic-maths"
-version = "0.2.0"
+version = "0.2.2"
 description = "This plugin adds utilities for mathematical tasks"
 license = {file = "LICENSE.txt"}
 readme = "README.md"
 
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
```

### Comparing `katalytic-maths-0.2.0/tests/test_bboxes.py` & `katalytic_maths-0.2.2/tests/test_bboxes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 import itertools
 
 import pytest as pytest
 
 from katalytic.data import all_types_besides
-from katalytic.maths.bboxes import _FORMATS, calc_bbox_area, calc_bbox_center, calc_IoB, calc_IoB_max, calc_IoB_min, calc_IoU, convert_bbox, non_max_suppression, set_bbox_scores, intersect_bboxes, is_bbox
+# noinspection PyProtectedMember
+from katalytic.maths.bboxes import (
+    _FORMATS, calc_bbox_area, calc_bbox_center, calc_IoB, calc_IoB_max, calc_IoB_min,
+    calc_IoU, convert_bbox, non_max_suppression, set_bbox_scores, intersect_bboxes, is_bbox)
 
 
 _EXAMPLES = {
     'xyXY': (1,2,9,9),
     'xyXY_s': ((1,2,9,9), 0.5),
     'xyXYs': (1,2,9,9,0.5),
     'xy_XY': ((1,2), (9,9)),
```

### Comparing `katalytic-maths-0.2.0/tests/test_maths.py` & `katalytic_maths-0.2.2/tests/test_maths.py`

 * *Files identical despite different names*

### Comparing `katalytic-maths-0.2.0/PKG-INFO` & `katalytic_maths-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: katalytic-maths
-Version: 0.2.0
+Version: 0.2.2
 Summary: This plugin adds utilities for mathematical tasks
 Author-email: Valentin Neagu <vali19th@protonmail.com>
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
@@ -22,14 +22,16 @@
 Requires-Dist: pytest-cov ; extra == "dev"
 Requires-Dist: pytest-clarity ; extra == "dev"
 Requires-Dist: pytest-randomly ; extra == "dev"
 Project-URL: homepage, https://gitlab.com/katalytic/katalytic-maths.git
 Project-URL: repository, https://gitlab.com/katalytic/katalytic-maths.git
 Provides-Extra: dev
 
+# Not fit for public use yet
+
 ## Description
 TODO: Let people know what your project can do specifically. Provide context and add a link to any reference visitors might be unfamiliar with. A list of Features or a Background subsection can also be added here. If there are alternatives to your project, this is a good place to list differentiating factors.
 
 [![version](https://img.shields.io/pypi/v/katalytic-maths)](https://pypi.org/project/katalytic-maths/)
 [![tests](https://gitlab.com/katalytic/katalytic-maths/badges/main/pipeline.svg?key_text=tests&key_width=38)](https://gitlab.com/katalytic/katalytic-maths/-/commits/main)
 [![coverage](https://gitlab.com/katalytic/katalytic-maths/badges/main/coverage.svg)](https://gitlab.com/katalytic/katalytic-maths/-/commits/main)
 [![docs](https://img.shields.io/readthedocs/katalytic-maths.svg)](https://katalytic-maths.readthedocs.io/en/latest/)
```

