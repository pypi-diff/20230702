# Comparing `tmp/tfv-0.0.9.tar.gz` & `tmp/tfv-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tfv-0.0.9.tar", last modified: Tue Jul 12 11:03:50 2022, max compression
+gzip compressed data, was "tfv-1.0.0.tar", last modified: Sun Jul  2 10:20:01 2023, max compression
```

## Comparing `tfv-0.0.9.tar` & `tfv-1.0.0.tar`

### file list

```diff
@@ -1,23 +1,90 @@
-drwxrwxrwx   0        0        0        0 2022-07-12 11:03:50.433551 tfv-0.0.9/
--rw-rw-rw-   0        0        0     1103 2022-06-27 10:18:28.000000 tfv-0.0.9/LICENSE
--rw-rw-rw-   0        0        0     1982 2022-07-12 11:03:50.433551 tfv-0.0.9/PKG-INFO
--rw-rw-rw-   0        0        0     1469 2022-07-12 10:44:36.000000 tfv-0.0.9/README.md
--rw-rw-rw-   0        0        0       42 2022-07-12 11:03:50.434551 tfv-0.0.9/setup.cfg
--rw-rw-rw-   0        0        0     1038 2022-07-12 10:43:32.000000 tfv-0.0.9/setup.py
-drwxrwxrwx   0        0        0        0 2022-07-12 11:03:50.420574 tfv-0.0.9/tfv/
--rw-rw-rw-   0        0        0      407 2022-07-12 10:45:02.000000 tfv-0.0.9/tfv/__init__.py
--rw-rw-rw-   0        0        0    36167 2022-06-27 10:22:09.000000 tfv-0.0.9/tfv/extractor.py
--rw-rw-rw-   0        0        0    18832 2022-06-27 10:18:28.000000 tfv-0.0.9/tfv/geometry.py
--rw-rw-rw-   0        0        0     4652 2022-06-27 10:18:28.000000 tfv-0.0.9/tfv/miscellaneous.py
--rw-rw-rw-   0        0        0     4906 2022-06-27 10:18:28.000000 tfv-0.0.9/tfv/mldatetime.py
--rw-rw-rw-   0        0        0     5972 2022-06-27 10:18:28.000000 tfv-0.0.9/tfv/particles.py
--rw-rw-rw-   0        0        0    10456 2022-06-27 10:18:28.000000 tfv-0.0.9/tfv/restart.py
--rw-rw-rw-   0        0        0     9754 2022-06-27 10:22:09.000000 tfv-0.0.9/tfv/timeseries.py
--rw-rw-rw-   0        0        0    20001 2022-07-08 03:48:03.000000 tfv-0.0.9/tfv/viewer.py
--rw-rw-rw-   0        0        0    40646 2022-07-12 10:41:21.000000 tfv-0.0.9/tfv/visual.py
-drwxrwxrwx   0        0        0        0 2022-07-12 11:03:50.431551 tfv-0.0.9/tfv.egg-info/
--rw-rw-rw-   0        0        0     1982 2022-07-12 11:03:50.000000 tfv-0.0.9/tfv.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      326 2022-07-12 11:03:50.000000 tfv-0.0.9/tfv.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-07-12 11:03:50.000000 tfv-0.0.9/tfv.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2022-07-12 11:03:50.000000 tfv-0.0.9/tfv.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2022-07-12 11:03:50.000000 tfv-0.0.9/tfv.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-02 10:20:01.183909 tfv-1.0.0/
+-rw-rw-rw-   0        0        0      962 2023-06-29 05:32:00.000000 tfv-1.0.0/.gitignore
+-rw-rw-rw-   0        0        0      869 2023-07-02 10:08:45.000000 tfv-1.0.0/.readthedocs.yaml
+-rw-rw-rw-   0        0        0     1105 2023-06-29 05:45:27.000000 tfv-1.0.0/LICENSE
+-rw-rw-rw-   0        0        0     2303 2023-07-02 10:20:01.183909 tfv-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1807 2023-06-29 05:45:27.000000 tfv-1.0.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-02 10:20:00.861122 tfv-1.0.0/docs/
+-rw-rw-rw-   0        0        0        5 2023-06-29 04:17:58.000000 tfv-1.0.0/docs/.gitignore
+-rw-rw-rw-   0        0        0      660 2023-06-29 04:17:58.000000 tfv-1.0.0/docs/Makefile
+-rwxrwxrwx   0        0        0      799 2023-06-29 04:17:58.000000 tfv-1.0.0/docs/make.bat
+drwxrwxrwx   0        0        0        0 2023-07-02 10:20:00.883347 tfv-1.0.0/docs/source/
+drwxrwxrwx   0        0        0        0 2023-07-02 10:20:00.899722 tfv-1.0.0/docs/source/api_reference/
+drwxrwxrwx   0        0        0        0 2023-07-02 10:20:00.899722 tfv-1.0.0/docs/source/api_reference/extractor/
+-rw-rw-rw-   0        0        0      121 2023-06-29 05:32:00.000000 tfv-1.0.0/docs/source/api_reference/extractor/FvExtractor.rst
+-rw-rw-rw-   0        0        0       87 2023-06-29 05:32:00.000000 tfv-1.0.0/docs/source/api_reference/extractor/index.rst
+drwxrwxrwx   0        0        0        0 2023-07-02 10:20:00.915383 tfv-1.0.0/docs/source/api_reference/geometry/
+drwxrwxrwx   0        0        0        0 2023-07-02 10:20:00.931003 tfv-1.0.0/docs/source/api_reference/geometry/classes/
+-rw-rw-rw-   0        0        0       95 2023-06-29 05:32:00.000000 tfv-1.0.0/docs/source/api_reference/geometry/classes/Mesh.rst
+-rw-rw-rw-   0        0        0       62 2023-06-29 05:32:00.000000 tfv-1.0.0/docs/source/api_reference/geometry/classes/index.rst
+drwxrwxrwx   0        0        0        0 2023-07-02 10:20:00.963016 tfv-1.0.0/docs/source/api_reference/geometry/functions/
+-rw-rw-rw-   0        0        0       85 2023-06-29 04:17:58.000000 tfv-1.0.0/docs/source/api_reference/geometry/functions/get_intersection.rst
+-rw-rw-rw-   0        0        0       85 2023-06-29 04:17:58.000000 tfv-1.0.0/docs/source/api_reference/geometry/functions/get_unit_vectors.rst
+-rw-rw-rw-   0        0        0      135 2023-06-29 04:17:58.000000 tfv-1.0.0/docs/source/api_reference/geometry/functions/index.rst
+-rw-rw-rw-   0        0        0       55 2023-06-29 04:17:58.000000 tfv-1.0.0/docs/source/api_reference/geometry/functions/is_ccw.rst
+-rw-rw-rw-   0        0        0       82 2023-06-29 04:17:58.000000 tfv-1.0.0/docs/source/api_reference/geometry/functions/is_intersection.rst
+-rw-rw-rw-   0        0        0      296 2023-06-29 05:32:00.000000 tfv-1.0.0/docs/source/api_reference/geometry/geometry.rst
+-rw-rw-rw-   0        0        0      108 2023-06-29 05:32:00.000000 tfv-1.0.0/docs/source/api_reference/geometry/index.rst
+-rw-rw-rw-   0        0        0      371 2023-06-29 05:32:00.000000 tfv-1.0.0/docs/source/api_reference/index.rst
+drwxrwxrwx   0        0        0        0 2023-07-02 10:20:00.983572 tfv-1.0.0/docs/source/api_reference/particles/
+-rw-rw-rw-   0        0        0      117 2023-06-29 05:32:00.000000 tfv-1.0.0/docs/source/api_reference/particles/FvParticles.rst
+-rw-rw-rw-   0        0        0       89 2023-06-29 05:32:00.000000 tfv-1.0.0/docs/source/api_reference/particles/index.rst
+drwxrwxrwx   0        0        0        0 2023-07-02 10:20:00.999667 tfv-1.0.0/docs/source/api_reference/timeseries/
+-rw-rw-rw-   0        0        0      121 2023-06-29 05:32:00.000000 tfv-1.0.0/docs/source/api_reference/timeseries/FvTimeSeries.rst
+-rw-rw-rw-   0        0        0       94 2023-06-29 05:32:00.000000 tfv-1.0.0/docs/source/api_reference/timeseries/index.rst
+drwxrwxrwx   0        0        0        0 2023-07-02 10:20:01.023695 tfv-1.0.0/docs/source/api_reference/viewer/
+-rw-rw-rw-   0        0        0      108 2023-06-29 05:32:00.000000 tfv-1.0.0/docs/source/api_reference/viewer/ColourBar.rst
+-rw-rw-rw-   0        0        0       99 2023-06-29 05:32:00.000000 tfv-1.0.0/docs/source/api_reference/viewer/Slider.rst
+-rw-rw-rw-   0        0        0       99 2023-06-29 05:32:00.000000 tfv-1.0.0/docs/source/api_reference/viewer/Viewer.rst
+-rw-rw-rw-   0        0        0      103 2023-06-29 05:32:00.000000 tfv-1.0.0/docs/source/api_reference/viewer/index.rst
+drwxrwxrwx   0        0        0        0 2023-07-02 10:20:01.054961 tfv-1.0.0/docs/source/api_reference/visual/
+-rw-rw-rw-   0        0        0      127 2023-06-29 05:32:00.000000 tfv-1.0.0/docs/source/api_reference/visual/ParticlesScatter.rst
+-rw-rw-rw-   0        0        0      117 2023-06-29 05:32:00.000000 tfv-1.0.0/docs/source/api_reference/visual/SheetContour.rst
+-rw-rw-rw-   0        0        0      111 2023-06-29 05:32:00.000000 tfv-1.0.0/docs/source/api_reference/visual/SheetPatch.rst
+-rw-rw-rw-   0        0        0      112 2023-06-29 05:32:00.000000 tfv-1.0.0/docs/source/api_reference/visual/SheetVector.rst
+-rw-rw-rw-   0        0        0      149 2023-06-29 05:32:00.000000 tfv-1.0.0/docs/source/api_reference/visual/index.rst
+drwxrwxrwx   0        0        0        0 2023-07-02 10:20:01.083586 tfv-1.0.0/docs/source/api_reference/xarray/
+-rw-rw-rw-   0        0        0     2118 2023-07-02 09:51:29.000000 tfv-1.0.0/docs/source/api_reference/xarray/index.md
+-rw-rw-rw-   0        0        0      107 2023-06-29 05:32:00.000000 tfv-1.0.0/docs/source/api_reference/xarray/tfvdomain.rst
+-rw-rw-rw-   0        0        0      119 2023-06-29 05:32:00.000000 tfv-1.0.0/docs/source/api_reference/xarray/tfvtimeseries.rst
+-rw-rw-rw-   0        0        0     2462 2023-06-29 05:32:00.000000 tfv-1.0.0/docs/source/conf.py
+-rw-rw-rw-   0        0        0       44 2023-07-02 10:08:45.000000 tfv-1.0.0/docs/source/dev-requirements.txt
+drwxrwxrwx   0        0        0        0 2023-07-02 10:20:01.083586 tfv-1.0.0/docs/source/examples/
+-rw-rw-rw-   0        0        0      257 2023-06-29 05:32:00.000000 tfv-1.0.0/docs/source/examples/index.rst
+drwxrwxrwx   0        0        0        0 2023-07-02 10:20:01.099245 tfv-1.0.0/docs/source/examples/notebooks/
+-rw-rw-rw-   0        0        0    17426 2023-06-29 05:32:00.000000 tfv-1.0.0/docs/source/examples/notebooks/tfv_tools_low_level.ipynb
+-rw-rw-rw-   0        0        0    12875 2023-06-29 05:32:00.000000 tfv-1.0.0/docs/source/examples/notebooks/tfv_tools_with_xarray.ipynb
+drwxrwxrwx   0        0        0        0 2023-07-02 10:20:01.099245 tfv-1.0.0/docs/source/examples/plot_composition/
+-rw-rw-rw-   0        0        0   475598 2023-06-29 05:32:00.000000 tfv-1.0.0/docs/source/examples/plot_composition/tfvdomain_plot_comp.ipynb
+drwxrwxrwx   0        0        0        0 2023-07-02 10:20:01.114869 tfv-1.0.0/docs/source/examples/xarray_basic_use/
+-rw-rw-rw-   0        0        0   837610 2023-06-29 05:32:00.000000 tfv-1.0.0/docs/source/examples/xarray_basic_use/tfv_tools_with_xarray.ipynb
+-rw-rw-rw-   0        0        0     1332 2023-06-29 05:45:27.000000 tfv-1.0.0/docs/source/index.rst
+-rw-rw-rw-   0        0        0       82 2023-06-29 04:17:58.000000 tfv-1.0.0/docs/source/installation.rst
+-rw-rw-rw-   0        0        0       42 2023-07-02 10:20:01.183909 tfv-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1225 2023-06-29 05:45:27.000000 tfv-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-02 10:20:01.130492 tfv-1.0.0/tests/
+drwxrwxrwx   0        0        0        0 2023-07-02 10:20:01.130492 tfv-1.0.0/tests/data/
+-rw-rw-rw-   0        0        0      322 2023-06-29 05:32:00.000000 tfv-1.0.0/tests/data/polyline.txt
+-rw-rw-rw-   0        0        0     2885 2023-06-29 05:32:00.000000 tfv-1.0.0/tests/test_extractor.py
+-rw-rw-rw-   0        0        0     5845 2023-06-29 05:32:00.000000 tfv-1.0.0/tests/test_xarray_accessor.py
+drwxrwxrwx   0        0        0        0 2023-07-02 10:20:01.161733 tfv-1.0.0/tfv/
+-rw-rw-rw-   0        0        0      510 2023-06-29 05:37:51.000000 tfv-1.0.0/tfv/__init__.py
+-rw-rw-rw-   0        0        0    46778 2023-06-29 05:32:00.000000 tfv-1.0.0/tfv/extractor.py
+-rw-rw-rw-   0        0        0    18829 2023-06-29 05:32:00.000000 tfv-1.0.0/tfv/geometry.py
+drwxrwxrwx   0        0        0        0 2023-07-02 10:20:01.183909 tfv-1.0.0/tfv/icons/
+-rw-rw-rw-   0        0        0     1775 2023-06-29 04:17:58.000000 tfv-1.0.0/tfv/icons/play_button.png
+-rw-rw-rw-   0        0        0      491 2023-06-29 04:17:58.000000 tfv-1.0.0/tfv/icons/stop_button.png
+-rw-rw-rw-   0        0        0     1748 2023-06-29 05:32:00.000000 tfv-1.0.0/tfv/miscellaneous.py
+-rw-rw-rw-   0        0        0     4906 2023-06-29 04:17:58.000000 tfv-1.0.0/tfv/mldatetime.py
+-rw-rw-rw-   0        0        0     5972 2023-06-29 04:17:58.000000 tfv-1.0.0/tfv/particles.py
+-rw-rw-rw-   0        0        0    10456 2023-06-29 04:17:58.000000 tfv-1.0.0/tfv/restart.py
+-rw-rw-rw-   0        0        0    15874 2023-06-29 05:32:00.000000 tfv-1.0.0/tfv/timeseries.py
+-rw-rw-rw-   0        0        0    21103 2023-06-29 05:32:00.000000 tfv-1.0.0/tfv/viewer.py
+-rw-rw-rw-   0        0        0    45252 2023-06-29 05:32:00.000000 tfv-1.0.0/tfv/visual.py
+-rw-rw-rw-   0        0        0    66702 2023-06-29 05:32:00.000000 tfv-1.0.0/tfv/xarray.py
+drwxrwxrwx   0        0        0        0 2023-07-02 10:20:01.183909 tfv-1.0.0/tfv.egg-info/
+-rw-rw-rw-   0        0        0     2303 2023-07-02 10:20:00.000000 tfv-1.0.0/tfv.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2325 2023-07-02 10:20:00.000000 tfv-1.0.0/tfv.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-02 10:20:00.000000 tfv-1.0.0/tfv.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      131 2023-07-02 10:20:00.000000 tfv-1.0.0/tfv.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-07-02 10:20:00.000000 tfv-1.0.0/tfv.egg-info/top_level.txt
```

### Comparing `tfv-0.0.9/LICENSE` & `tfv-1.0.0/LICENSE`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2019 Toby Devlin & Jonah Chorley
+Copyright (c) 2022 BMT Group Ltd, TUFLOW Support
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `tfv-0.0.9/PKG-INFO` & `tfv-1.0.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,65 +1,66 @@
 Metadata-Version: 2.1
 Name: tfv
-Version: 0.0.9
+Version: 1.0.0
 Summary: Post processing tools for TUFLOW FV results
 Home-page: https://gitlab.com/TUFLOW/tfv
 Author: Jonah Chorley, Toby Devlin & TUFLOW Support
 Author-email: support@tuflow.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
+Provides-Extra: viewer
 License-File: LICENSE
 
 # TFV
-The tfv package is a suite of tools for post-processing results from the
-[TUFLOW FV](https://www.tuflow.com/Tuflow%20FV.aspx) hydrodynamic, sediment transport, water quality and particle
-tracking modelling software. 
+The tfv package is a suite of tools for post-processing results from the [TUFLOW FV](https://www.tuflow.com/Tuflow%20FV.aspx) hydrodynamic, sediment transport, water quality and particle tracking modelling software. 
 
-It is also provides a basic framework for extracting and visualizing 2D and 3D oceanographic and atmospheric model result data on unstructured
-meshes.
+It is also provides a basic framework for extracting and visualizing 2D and 3D oceanographic and atmospheric model result data on unstructured meshes.
 
 ## Installing
 The tfv package is available via the Python Package Index ([PyPi](https://pypi.org/project/tfv/))
 
-*Note: Version 0.0.9 has been built and tested on Python 3.6 to 3.10*.
+*Note: Version 1.0.0 has been built and tested on Python 3.9 to 3.11*.
 
 From command prompt install and update using pip:
 
 ```
 python -m pip install tfv
 ```
 
-## Dependancies
-The tfv package depends on the following packages:
+## Dependencies
+The tfv package depends on the following core packages:
 
 ```
 matplotlib >= 3.2.2
 netCDF4 >= 1.5.3
 numpy >= 1.19.0
-PyQt5 >= 5.15.0
+xarray>=v2022.03.0
+dask>=2022.01.0
+scipy>=1.6.0
+tqdm>=4.50.0
 ```
 
 These will be automatically installed or updated as part of the tfv installation.
 
+The following packages provide additional functionality and are **not** installed by default:
+
+`ipywidgets >= 8.0.0` - Required for interactive results vizulisation in an interactive session (e.g., JuypterLab)
+
+`PyQt5 >= 5.15.0`  - Required for interactive popout results vizulisation
+
 ## Tutorials, Documentation & Support
 See the [API Reference](https://tfv.readthedocs.io/en/latest/) for code documentation and
 [TUFLOW FV Python Tools](https://fvwiki.tuflow.com/index.php?title=FV_Python_Tools) for tutorials and demonstration 
 datasets. 
 
 For support contact [TUFLOW Support](mailto:support@tuflow.com).
 
 ## Authors
 * **Jonah Chorley**
 * **Toby Devlin**
 * **TUFLOW Support**
 
 ## License
 This project is licensed under the MIT License - see the [LICENSE.txt](https://gitlab.com/TUFLOW/tfv/blob/master/LICENSE) file for details
-
-
-
-
```

### Comparing `tfv-0.0.9/setup.py` & `tfv-1.0.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as rm:
     long_description = rm.read()
 
 setup = \
     {
         'name': "tfv",
-        'version': '0.0.9',
+        'version': '1.0.0',
         'description': "Post processing tools for TUFLOW FV results",
         'long_description': long_description,
         'long_description_content_type': "text/markdown",
         'url': "https://gitlab.com/TUFLOW/tfv",
 
         'author': "Jonah Chorley, Toby Devlin & TUFLOW Support",
         'author_email': "support@tuflow.com",
@@ -20,18 +20,24 @@
         'classifiers':
             [
                 "Programming Language :: Python :: 3",
                 "License :: OSI Approved :: MIT License",
                 "Operating System :: OS Independent",
             ],
 
-        'python_requires': '>=3.6',
+        'python_requires': '>=3.9',
         'install_requires':
             [
                 'numpy>=1.19.0',
                 'matplotlib>3.2.2',
                 'netCDF4>=1.5.3',
-                'PyQt5>=5.15.0',
-            ]
+                'xarray>=v2022.03.0',
+                'dask>=2022.01.0',
+                'scipy>=1.6.0',
+                'tqdm>=4.50.0'
+            ],
+        'extras_require':{
+            'viewer': ["PyQt5>=5.15.0"]
+        }
     }
 
 setuptools.setup(**setup)
```

### Comparing `tfv-0.0.9/tfv/geometry.py` & `tfv-1.0.0/tfv/geometry.py`

 * *Files 0% similar despite different names*

```diff
@@ -237,15 +237,15 @@
 
         # Declare edge_node as tuple (n1, n2, idx)
         self.edge_node = \
             (
                 self.cell_node[:, [0, 1, 2, 3]].flatten(),
                 self.cell_node[:, [1, 2, 3, 0]].flatten(),
                 np.repeat(np.arange(self.cell_node.shape[0]), 4),
-                np.zeros((self.nc2 * 4,), dtype=np.bool)
+                np.zeros((self.nc2 * 4,), dtype=bool)
             )
 
         # Delete 4th edge of triangle cells (repeated 3rd node)
         invalid = np.where(self.edge_node[0] == self.edge_node[1])[0]
         self.edge_node = tuple(np.delete(arr, invalid) for arr in self.edge_node)
 
     def __prepare_node_weights__(self):
```

### Comparing `tfv-0.0.9/tfv/mldatetime.py` & `tfv-1.0.0/tfv/mldatetime.py`

 * *Files identical despite different names*

### Comparing `tfv-0.0.9/tfv/particles.py` & `tfv-1.0.0/tfv/particles.py`

 * *Files identical despite different names*

### Comparing `tfv-0.0.9/tfv/restart.py` & `tfv-1.0.0/tfv/restart.py`

 * *Files identical despite different names*

### Comparing `tfv-0.0.9/tfv/viewer.py` & `tfv-1.0.0/tfv/viewer.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,18 +6,36 @@
 
 import matplotlib as mpl
 import matplotlib.pyplot as plt
 from matplotlib.animation import FFMpegWriter
 from matplotlib.colorbar import Colorbar
 from matplotlib.text import Text
 
-from PyQt5.QtWidgets import QSlider, QWidget, QHBoxLayout, \
-                            QVBoxLayout, QLabel, QPushButton
-from PyQt5.QtGui import QIcon
-from PyQt5.QtCore import Qt
+# Check to see if PyQt5 is available
+import_err_msg = "\n".join([
+    "You must additionally install `PyQt5` to use the Viewer module",
+    "Please install this using your relevant python package distribution",
+    "PyPi - `pip install pyqt5` - https://pypi.org/project/PyQt5/ ",
+    "Anaconda - `conda install -c anaconda pyqt` - https://anaconda.org/anaconda/pyqt",
+    "Conda-forge - conda install -c conda-forge pyqt` - https://anaconda.org/conda-forge/pyqt"
+])
+
+import pkg_resources
+try:
+    pkg_resources.get_distribution('PyQt5')
+except pkg_resources.DistributionNotFound:
+    raise ImportError(import_err_msg)
+else:
+    HAS_PYQT5 = True
+
+if HAS_PYQT5:
+    from PyQt5.QtWidgets import QSlider, QWidget, QHBoxLayout, \
+                                QVBoxLayout, QLabel, QPushButton
+    from PyQt5.QtGui import QIcon
+    from PyQt5.QtCore import Qt
 
 # configure MPL
 mpl.use('Qt5Agg')
 plt.interactive(True)
 
 
 class Slider:
@@ -48,15 +66,20 @@
     index : integer
         The current index of the slider
     text : string
         The display text of the slider
     """
 
     # Constructor functions
-    def __init__(self, figure, range=np.arange(100), step=1, wait=0.01, format='num'):
+    def __init__(self,
+                 figure,
+                 range=np.arange(100),
+                 step=1,
+                 wait=0.01,
+                 format='num'):
         # protected attributes
         self._figure = figure
         self._range = range
 
         self._value = None
         self._index = None
         self._text = ''
@@ -178,24 +201,20 @@
 
     # Protected member functions
     def _synchronise(self):
         # set the value of the slider widget
         self.slider_widget.setValue(self.index)
 
         # update the text display above the slider
-        if self.format == 'num':
-            self._text = str(self.value)
-        elif self.format == 'hms':
-            rt = self.value - self.range[0]
-            hh = int(np.floor(rt/3600))
-            mm = int(np.floor((rt - hh*3600)/60))
-            ss = int(np.floor((rt - hh*3600 - mm*60)))
-            self._text = '{:02d}:{:02d}:{:02d}'.format(hh, mm, ss)
+        if self.format == 'int':
+            self._text = str(self.index)
+        elif type(self.value) == np.int32:
+            self._text = str(self.index)
         else:
-            self._text = datestr(float(self.value), self.format)
+            self._text = self.value.strftime(self.format)
         self.label_widget.setText(self._text)
 
         # pass new value to call backs
         for callback in self._callbacks:
             callback(self.value)
 
     def _changed(self):
@@ -269,15 +288,15 @@
     @property
     def range(self):
         return self._range
 
     @range.setter
     def range(self, range):
         # set the protected range
-        self._range = np.array(range)
+        self._range = range
 
         # update slider limits
         min_val, max_val = 0, len(range) - 1
         self.slider_widget.setMinimum(min_val)
         self.slider_widget.setMaximum(max_val)
 
         # reset the value
@@ -286,14 +305,16 @@
     @property
     def value(self):
         return self._value
 
     @value.setter
     def value(self, value):
         # set the index based on nearest value in range
+        if value == 0:
+            value = self.range[0]
         self.index = np.argmin(np.abs(self.range - value))
 
     @property
     def index(self):
         return self._index
 
     @index.setter
@@ -360,15 +381,21 @@
     text : string
         Text of the display
     """
 
     __register__ = list()
 
     # Constructor function
-    def __init__(self, size=(240, 120), units='mm', step=1, wait=0.01, format='%d/%m/%Y %H:%M:%S', display=True):
+    def __init__(self,
+                 size=(240, 120),
+                 units='mm',
+                 step=1,
+                 wait=0.01,
+                 format='%d/%m/%Y %H:%M:%S',
+                 display=True):
         """Initializes Viewer object with figure size, figure units & title time format"""
 
         # add self to the viewer register
         self.__register__.append(self)
 
         # public attributes
         self.figure = None
@@ -381,36 +408,44 @@
         self._title_axes = None
         self._title_obj = None
 
         # set up the MPL figure
         sf_map = {'mm': 12 / 300, 'cm': 12 / 30, 'm': 12 / 0.3}
 
         sf = sf_map[self.units]
-        w = self.size[0]*sf
-        h = self.size[1]*sf
+        w = self.size[0] * sf
+        h = self.size[1] * sf
 
         self.figure = plt.figure(figsize=(w, h))
 
         # add the slider
-        self._slider_bar = Slider(self.figure, step=step, wait=wait, format=format)
+        self._slider_bar = Slider(self.figure,
+                                  step=step,
+                                  wait=wait,
+                                  format=format)
 
         # create title axes and add text for title
         rec = [0.30, 0.96, 0.40, 0.04]
         self._title_axes = self.figure.add_axes(rec)
         self._title_axes.xaxis.set_visible(False)
         self._title_axes.yaxis.set_visible(False)
         self._title_axes.set_navigate(False)
 
         for spine in self._title_axes.spines.values():
             spine.set_color('white')
 
         self._title_axes.set_xlim(0, 2)
         self._title_axes.set_ylim(0, 2)
 
-        self._title_obj = Text(1, 1, '', fontsize=12, horizontalalignment='center', verticalalignment='center')
+        self._title_obj = Text(1,
+                               1,
+                               '',
+                               fontsize=12,
+                               horizontalalignment='center',
+                               verticalalignment='center')
         self._title_axes._add_text(self._title_obj)
 
         # connect display text to the slider bar
         self._slider_bar.connect(self._set_text)
 
         # set text and show_time
         self.text = self._slider_bar.text
@@ -427,21 +462,18 @@
 
     @property
     def time_vector(self):
         return self._slider_bar.range
 
     @time_vector.setter
     def time_vector(self, time_vector):
-        if np.all(self.time_vector == np.arange(100)):
-            self._slider_bar.range = time_vector
-        else:
-            t1 = np.hstack((self.time_vector, time_vector)).min()
-            t2 = np.hstack((self.time_vector, time_vector)).max()
-            dt = np.min((np.mean(np.diff(self.time_vector)), np.mean(np.diff(time_vector))))
-            self._slider_bar.range = np.arange(t1, t2 + dt, dt)
+        # if np.all(self.time_vector == np.arange(100)):
+        self._slider_bar.range = time_vector
+        # else:
+        #     self._slider_bar.range = np.arange(t1, t2 + dt, dt)
 
     @property
     def step(self):
         return self._slider_bar.step
 
     @step.setter
     def step(self, step):
@@ -472,15 +504,15 @@
         self._title_obj.set_text(text)
         self._slider_bar.text = text
 
     @property
     def show_time(self):
         return self._title_axes.get_visible()
 
-    @ show_time.setter
+    @show_time.setter
     def show_time(self, show_time):
         self._title_axes.axes.set_visible(show_time)
 
     # protected member functions
     def _set_text(self, dummy):
         self.text = self._slider_bar.text
 
@@ -505,15 +537,15 @@
             File format i.e 'png', 'pdf', 'jpg'
         dpi : integer
             Resolution in dots per inch (dpi)
         """
 
         self.figure.savefig(file_path, format=format, dpi=dpi)
 
-    def animate(self, file_path, ts, te, dt,  fps=10, dpi=150):
+    def animate(self, file_path, ts, te, dt, fps=10, dpi=150):
         """
         Writes animation file for specified time interval.
 
         Parameters
         ----------
         file_path : string
             File path to output animation
@@ -529,19 +561,19 @@
         fps : integer
             Frames per second
         dpi : integer
             Resolution in dots per inch (dpi)
         """
 
         # Loop through time
-        nt = int((te - ts) / dt)+1
+        nt = int((te - ts) / dt) + 1
         writer = FFMpegWriter(fps=fps)
         with writer.saving(self.figure, file_path, dpi):
             for ii in range(nt):
-                self.time_current = (ts + ii*dt)
+                self.time_current = (ts + ii * dt)
                 writer.grab_frame()
 
 
 class ColourBar(Colorbar):
     """
     A wrapper around the matplotlib colorbar, simplifying for neater plots.
 
@@ -558,15 +590,20 @@
         Offset from axes as fraction of total figure width or height
     thickness : float
         Thickness of bar as fraction of total figure width or height
     label : string
         String to label the colour bar.
     """
 
-    def __init__(self, patch, location='bottom', offset=0.075, thickness=0.010, label=''):
+    def __init__(self,
+                 patch,
+                 location='bottom',
+                 offset=0.075,
+                 thickness=0.010,
+                 label=''):
 
         # Get target axes handle
         if type(patch).__name__ == 'TriContourSet':
             target = patch.ax
         else:
             target = patch.axes
 
@@ -576,37 +613,49 @@
         else:
             offset_1 = 0
             offset_2 = offset
 
         # Determine rectangles for target axes & colour bar axes
         rec = target.get_position().extents
         if location == 'bottom':
-            rec1 = [rec[0], rec[1] + offset_1, rec[2] - rec[0], rec[3] - rec[1] - offset_1]
+            rec1 = [
+                rec[0], rec[1] + offset_1, rec[2] - rec[0],
+                rec[3] - rec[1] - offset_1
+            ]
             rec2 = [rec[0], rec[1] + offset_2, rec[2] - rec[0], thickness]
         elif location == 'top':
-            rec1 = [rec[0], rec[1], rec[2] - rec[0], rec[3] - rec[1] - offset_1]
+            rec1 = [
+                rec[0], rec[1], rec[2] - rec[0], rec[3] - rec[1] - offset_1
+            ]
             rec2 = [rec[0], rec[3] - offset_2, rec[2] - rec[0], thickness]
         elif location == 'left':
-            rec1 = [rec[0] + offset_1, rec[1], rec[2] - rec[0] - offset_1, rec[3] - rec[1]]
+            rec1 = [
+                rec[0] + offset_1, rec[1], rec[2] - rec[0] - offset_1,
+                rec[3] - rec[1]
+            ]
             rec2 = [rec[0] + offset_2, rec[1], thickness, rec[3] - rec[1]]
         elif location == 'right':
-            rec1 = [rec[0], rec[1], rec[2] - rec[0] - offset_1, rec[3] - rec[1]]
+            rec1 = [
+                rec[0], rec[1], rec[2] - rec[0] - offset_1, rec[3] - rec[1]
+            ]
             rec2 = [rec[2] - offset_2, rec[1], thickness, rec[3] - rec[1]]
 
         target.set_position(rec1)
         axes = target.figure.add_axes(rec2)
 
         # Set orientation
         if location == 'bottom' or location == 'top':
             orientation = 'horizontal'
         elif location == 'left' or location == 'right':
             orientation = 'vertical'
 
         # Initialize Colorbar
-        super(ColourBar, self).__init__(axes, mappable=patch, orientation=orientation)
+        super(ColourBar, self).__init__(axes,
+                                        mappable=patch,
+                                        orientation=orientation)
 
         # Finish formatting
         if orientation == 'horizontal':
             axes.xaxis.set_ticks_position(location)
             axes.xaxis.set_label_position(location)
             axes.set_xlabel(label)
         elif orientation == 'vertical':
```

### Comparing `tfv-0.0.9/tfv/visual.py` & `tfv-1.0.0/tfv/visual.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 """A module defining all objects used to visualise model result data extracts"""
 
-from tfv.viewer import *
+# from tfv.viewer import *
 from tfv.miscellaneous import *
+from tfv.geometry import Mesh
 from abc import ABC, abstractmethod
 
+import pandas as pd
 import matplotlib as mpl
 import matplotlib.pyplot as plt
 import matplotlib.dates as mdates
 from matplotlib.lines import Line2D
 from matplotlib.quiver import Quiver
 from matplotlib.tri import Triangulation, TriContourSet
 from matplotlib.cbook import silent_list
@@ -16,18 +18,14 @@
 
 # Non-essential imports
 from matplotlib import cm
 from matplotlib.dates import DateFormatter
 from matplotlib.colors import Normalize, BoundaryNorm
 
 
-mpl.use('Qt5Agg')
-plt.interactive(True)
-
-
 # --------------------------------------------------- Visual Objects ---------------------------------------------------
 class Visual(ABC):
     """
     An abstract base class for an object which visualizes a variable. The main purpose of a Visual sub-class is to
     initialize and store a plotting library specific graphics object for a given extract type i.e SheetPatch.
 
     The Visual object works by connecting its set_time_current method to the Slider object. When self.set_time_current
@@ -43,47 +41,82 @@
         self.axes = axes
 
         # Set extractor
         self.extractor = extractor
         self._time_current = self.time_vector[0]
         self._time_index = 0
 
-        # Set expression
-        if type(expression) is str:
-            self.expression = Expression(expression)
-        elif type(expression) is list:
-            self.expression = [Expression(exp) for exp in expression]
+        self.expression = expression
+        self.expression_kwargs = dict(
+            post_process=kwargs.pop("post_process", None),
+        )
+
+        # Check whether the user has supplied a normal exp
+        # (e.g., str 'V_x', list of vars ['V_x', 'V_y'])
+        # OR whether the user supplied a list of data [np.array, np.array]
+        self.custom_data = False
+        if isinstance(self.expression, list):
+            if isinstance(self.expression[0], np.ndarray):
+                self.__process_custom_data__()
+        elif isinstance(self.expression, np.ndarray):
+            self.__process_custom_data__()
         else:
-            self.expression = None
+            self.custom_data = False
 
         # Connect with viewer
-        viewer = kwargs.pop('viewer', None)
+        viewer = kwargs.pop("viewer", None)
         if viewer is None:
-            viewer = Viewer.__register__[0]
-        self.viewer = viewer
-        self.viewer.time_vector = self.time_vector
-        self.viewer.connect(self.set_time_current)
+            # viewer = Viewer.__register__[0]
+            self.viewer = None
+        else:
+            self.viewer = viewer
+            self.viewer.time_vector = self.time_vector
+            self.viewer.connect(self.set_time_current)
 
         # Initialize the graphics object
+        zoom = kwargs.pop("zoom", True)
         self.__prep_graphics_obj__(**kwargs)
 
+        # NOTE: AEW Dec 22, 2022: Moved zoom above __prep_graphics_object__
+        # Unsure what ramifications this will have, but it will solve vector grid for zoomed
         # Zoom to the graphics object
-        self.zoom()
+        if zoom is True:
+            self.zoom()
 
     def get_time_current(self):
         return self._time_current
 
     def set_time_current(self, time):
+        # Add a catch to allow str or int based indexing
+        if type(time) == str:
+            time = pd.Timestamp(time)
+        elif type(time) == int:
+            time = self.time_vector[time]
+
         ii = np.argmin(np.abs(self.time_vector - time))
 
         if ii != self._time_index:
             self._time_index = ii
             self._time_current = self.time_vector[ii]
             self.__dynamic_update__()
-            self.viewer.figure.canvas.draw()
+
+            if self.viewer:
+                self.viewer.figure.canvas.draw()
+
+    def __process_custom_data__(self):
+        self.custom_data = True
+        self.vardata = np.ma.stack(self.expression)
+
+        # Apply post-processing logic to data
+        if self.expression_kwargs["post_process"]:
+            fn = self.expression_kwargs["post_process"]
+            self.vardata = fn(self.vardata)
+        else:
+            self.vardata = np.squeeze(self.vardata)
+
     @abstractmethod
     def __get_data__(self):
         """Abstract method which returns object data based on the expression"""
 
     @abstractmethod
     def __prep_graphics_obj__(self, **kwargs):
         """Abstract method to initialize the graphics object which will be used to visualize the result"""
@@ -114,20 +147,23 @@
         Extractor object which is extracting data
     expression : string
         Expression that defines a variable
     datum : {'sigma', 'depth', 'height', 'elevation'}
         Vertical depth-averaging datum i.e sigma, depth, height, elevation, top, bottom.
     limits : tuple
         Vertical depth-averaging limits (z1, z2) relative to vertical datum.
+    data : numpy.array
+        Custom data array of data for plotting. Should have length equal to either
+        NumCells2D (if uses shading==flat, the default default) or NumVert2D if shading =='interp'
 
 
     Other Parameters
     ----------------
     shading : {'flat', 'interp'}
-        Sets the shading to be flat or interpolated (gourad)
+        Sets the shading to be flat (default) or interpolated (gourad)
     zorder : integer
         Layer order in which graphics object will be rendered (0 is bottom/first)
     cmap : matplotlib.colors.LinearSegmentedColormap
         Colormap object for mapping normalized data (0 - 1) to rgb colors
     norm : matplotlib.colors.BoundaryNorm
         Normalization object for normalizing raw data to (0 - 1) based on (min, max)
     clim : tuple
@@ -137,44 +173,67 @@
     antialiased : bool
         Sets the antialiasing state for rendering the underlying matplotlib.collections object
     alpha : float
         Sets the transparencies of the underlying matplotlib.collections object
 
     """
 
-    def __init__(self, axes, extractor, expression, datum='sigma', limits=(0, 1), **kwargs):
+    def __init__(
+        self,
+        axes,
+        extractor,
+        expression,
+        datum="sigma",
+        limits=(0, 1),
+        agg="mean",
+        mask_dry=True,
+        **kwargs
+    ):
         self.datum = datum
         self.limits = limits
+        self.agg = agg
+        self.mask_dry = mask_dry
 
         # Call initialize method of super class
         super(SheetPatch, self).__init__(axes, extractor, expression, **kwargs)
 
     def __get_data__(self):
-        args = (self.expression, self._time_index, self.datum, self.limits)
-        if self.shading == 'flat':
-            return self.extractor.get_sheet_cell(*args)
-        elif self.shading == 'interp':
-            return self.extractor.get_sheet_node(*args)
+        args = (
+            self.expression,
+            self._time_index,
+            self.datum,
+            self.limits,
+            self.agg,
+            self.mask_dry,
+        )
+        if self.shading == "flat":
+            return self.extractor.get_sheet_cell(*args, **self.expression_kwargs)
+        elif self.shading == "interp":
+            return self.extractor.get_sheet_node(*args, **self.expression_kwargs)
 
     def __prep_graphics_obj__(self, **kwargs):
         # Pop key word arguments which are not used by the graphics object
-        self.shading = kwargs.pop('shading', 'flat')
+        self.shading = kwargs.pop("shading", "flat")
 
         # Get handles on sheet geometry
         node_x = self.extractor.node_x
         node_y = self.extractor.node_y
         cell_node = self.extractor.cell_node
         tri_cell_node = self.extractor.tri_cell_node
 
-        # Instantiate graphics object based on shading type
-        data = self.__get_data__()
-        if self.shading == 'flat':
+        # # Instantiate graphics object based on shading type
+        if self.custom_data:
+            data = self.vardata
+        else:
+            data = self.__get_data__()
+
+        if self.shading == "flat":
             xy = np.dstack((node_x[cell_node], node_y[cell_node]))
             self.patch = PolyCollection(xy, array=data, **kwargs)
-        elif self.shading == 'interp':
+        elif self.shading == "interp":
             self.tri = Triangulation(node_x, node_y, triangles=tri_cell_node)
             self.patch = TriMesh(self.tri, array=data, antialiased=True, **kwargs)
 
             # Mask invalid triangles
             mask = np.any(data.mask[self.extractor.tri_cell_node], axis=1)
             self.tri.set_mask(mask)
 
@@ -185,21 +244,25 @@
         pass
 
     def __dynamic_update__(self):
         data = self.__get_data__()
         self.patch.set_array(data)
 
         # Mask invalid triangles
-        if self.shading == 'interp':
+        if self.shading == "interp":
             mask = np.any(data.mask[self.extractor.tri_cell_node], axis=1)
             self.tri.set_mask(mask)
 
     def zoom(self):
-        self.axes.set_xlim([np.min(self.extractor.node_x), np.max(self.extractor.node_x)])
-        self.axes.set_ylim([np.min(self.extractor.node_y), np.max(self.extractor.node_y)])
+        self.axes.set_xlim(
+            [np.min(self.extractor.node_x), np.max(self.extractor.node_x)]
+        )
+        self.axes.set_ylim(
+            [np.min(self.extractor.node_y), np.max(self.extractor.node_y)]
+        )
 
 
 class SheetContour(Visual):
     """
     Class for dynamic visualization of model result sheet extracts as contours
 
     Parameters
@@ -229,63 +292,97 @@
         Sets the mesh edge colouring of the underlying matplotlib.collections object
     antialiased : bool
         Sets the antialiasing state for rendering the underlying matplotlib.collections object
     alpha : float
         Sets the transparencies of the underlying matplotlib.collections object
     """
 
-    def __init__(self, axes, extractor, expression, datum='sigma', limits=(0, 1), **kwargs):
+    def __init__(
+        self,
+        axes,
+        extractor,
+        expression,
+        datum="sigma",
+        limits=(0, 1),
+        agg="mean",
+        mask_dry=True,
+        **kwargs
+    ):
         self.datum = datum
         self.limits = limits
+        self.agg = agg
+        self.mask_dry = mask_dry
 
         # Call initialize method of super class
         super(SheetContour, self).__init__(axes, extractor, expression, **kwargs)
 
     def __get_data__(self):
-        args = (self.expression, self._time_index, self.datum, self.limits)
-        return self.extractor.get_sheet_node(*args)
+        args = (
+            self.expression,
+            self._time_index,
+            self.datum,
+            self.limits,
+            self.agg,
+            self.mask_dry,
+        )
+        return self.extractor.get_sheet_node(*args, **self.expression_kwargs)
 
     def __prep_graphics_obj__(self, **kwargs):
         # Get handles on sheet geometry
         node_x = self.extractor.node_x
         node_y = self.extractor.node_y
         tri_cell_node = self.extractor.tri_cell_node
 
         # Get triangular mesh and initialize cpp triangulation
         tri = Triangulation(node_x, node_y, triangles=tri_cell_node)
+        self.tri = tri
         self.cpp_tri = tri.get_cpp_triangulation()
 
         # Get data
-        data = self.__get_data__()
+        if self.custom_data:
+            data = self.vardata
+        else:
+            data = self.__get_data__()
 
         # Mask bad triangles
         mask = np.any(data.mask[self.extractor.tri_cell_node], axis=1)
         self.cpp_tri.set_mask(mask)
-
+                
         # Set contour limits/levels
         zlim = [data.min(), data.max()]
+        
+        # BUG: This is a workaround for matplotlib's TriContourSet, which has issues on a log scale with nega values
+        # even if they are masked. Hence we will block out this data
+        data.data[data.mask] = zlim[0]
 
-        clim = kwargs.pop('clim', [zlim[0], zlim[1]])
-        self.levels = kwargs.pop('levels', 50)
+        clim = kwargs.pop("clim", [zlim[0], zlim[1]])
+        self.levels = kwargs.pop("levels", 50)
 
         if type(self.levels) is int:
             levels = np.linspace(clim[0], clim[1], self.levels)
         else:
             levels = self.levels
 
-        self.cont = TriContourSet(self.axes, tri, data.data, levels, filled=True, extend='both', **kwargs)
+        self.cont_args = kwargs  # For dynamic update
+        filled = kwargs.pop("filled", True)
+        extend = kwargs.pop("extend", "both")
+        self.cont = TriContourSet(
+            self.axes, tri, data.data, levels, filled=filled, extend=extend, **kwargs
+        )
 
         if clim is not None:
             self.cont.set_clim(clim)
 
     def __static_update__(self):
         pass
 
     def __dynamic_update__(self):
         # Get data
+        if self.custom_data:
+            assert False, "You can't update time dynamically when supplying custom data"
         data = self.__get_data__()
 
         # Mask bad triangles
         mask = np.any(data.mask[self.extractor.tri_cell_node], axis=1)
         self.cpp_tri.set_mask(mask)
 
         # Set contour limits/levels
@@ -293,57 +390,36 @@
         clim = self.cont.get_clim()
 
         if type(self.levels) is int:
             levels = np.linspace(clim[0], clim[1], self.levels)
         else:
             levels = self.levels
 
-        # self._contour_args(self, args, kwargs)
-        self.cont.zmin = zlim[0]
-        self.cont.zmax = zlim[1]
-
-        # self._contour_level_args
-        self.cont.levels = levels
-
-        # self.__init__
-        self.cont._process_levels()
-
-        # Update cpp generator
-        self.cont.cppContourGenerator = TriContourGenerator(self.cpp_tri, data)
-
-        # Update Paths
-        lowers, uppers = self.cont._get_lowers_and_uppers()
-        segs, kinds = self.cont._get_allsegs_and_allkinds()
-
-        zorder = self.cont.collections[0].zorder
         for collection in self.cont.collections:
-            self.cont.ax.collections.remove(collection)
-        self.cont.collections = silent_list('PathCollection')
+            self.cont.collections.remove(collection)
 
-        for level, level_upper, segs, kinds in \
-                zip(lowers, uppers, segs, kinds):
-            paths = self.cont._make_paths(segs, kinds)
-
-            col = \
-                PathCollection(
-                    paths,
-                    antialiaseds=(self.cont.antialiased,),
-                    edgecolors=None,
-                    alpha=self.cont.alpha,
-                    transform=self.cont.get_transform(),
-                    zorder=zorder
-                )
-
-            self.cont.ax.add_collection(col, autolim=False)
-            self.cont.collections.append(col)
-        self.cont.changed()
+        self.cont = TriContourSet(
+            self.axes,
+            self.tri,
+            data.data,
+            levels,
+            filled=True,
+            extend="both",
+            **self.cont_args
+        )
+
+        self.cont.set_clim(clim)
 
     def zoom(self):
-        self.axes.set_xlim([np.min(self.extractor.node_x), np.max(self.extractor.node_x)])
-        self.axes.set_ylim([np.min(self.extractor.node_y), np.max(self.extractor.node_y)])
+        self.axes.set_xlim(
+            [np.min(self.extractor.node_x), np.max(self.extractor.node_x)]
+        )
+        self.axes.set_ylim(
+            [np.min(self.extractor.node_y), np.max(self.extractor.node_y)]
+        )
 
 
 class SheetVector(Visual):
     """
     Class for dynamic visualization of model result sheet extracts as gridded vector field
 
     Parameters
@@ -356,70 +432,112 @@
         Tuple of string expressions that defines vector (vec_x, vec_y)
     datum : {'sigma', 'depth', 'height', 'elevation'}
         Vertical depth-averaging datum i.e sigma, depth, height, elevation, top, bottom.
     limits : tuple
         Vertical depth-averaging limits (z1, z2) relative to vertical datum.
     """
 
-    def __init__(self, axes, extractor, expression, datum, limits, **kwargs):
+    def __init__(
+        self,
+        axes,
+        extractor,
+        expression,
+        datum="sigma",
+        limits=(0, 1),
+        agg="mean",
+        normalise=False,
+        **kwargs
+    ):
         self.datum = datum
         self.limits = limits
+        self.agg = agg
+        self.norm = normalise
 
         self.xg = None
         self.yg = None
         self.grid_index = None
 
         # Call initialize method of super class
         super(SheetVector, self).__init__(axes, extractor, expression, **kwargs)
 
     def __get_data__(self):
-        args = (self._time_index, self.xg, self.yg, self.datum, self.limits)
-        u = self.extractor.get_sheet_grid(self.expression[0], *args, grid_index=self.grid_index)
-        v = self.extractor.get_sheet_grid(self.expression[1], *args, grid_index=self.grid_index)
+        args = (self._time_index, self.xg, self.yg, self.datum, self.limits, self.agg)
+        u = self.extractor.get_sheet_grid(
+            self.expression[0], *args, grid_index=self.grid_index
+        )
+        v = self.extractor.get_sheet_grid(
+            self.expression[1], *args, grid_index=self.grid_index
+        )
 
         return u, v
 
     def __prep_graphics_obj__(self, **kwargs):
         # Pop key word arguments which are not used by the graphics object
-        self.resolution = kwargs.pop('resolution', 40)
+        self.resolution = kwargs.pop("resolution", 40)
 
         # Instantiate graphics object with no data, data will be added on draw event automatically
-        self.quiver = Quiver(self.axes, np.mean(self.extractor.node_x), np.mean(self.extractor.node_y), 0, 0, **kwargs)
+        self.quiver = Quiver(
+            self.axes,
+            np.mean(self.extractor.node_x),
+            np.mean(self.extractor.node_y),
+            0,
+            0,
+            **kwargs
+        )
 
         # Add the graphics object to axes
         self.axes.add_collection(self.quiver)
 
         # Connect the regrid method to the draw event of the figure object.
-        self._x_cid = self.axes.callbacks.connect('xlim_changed', self.__static_update__)
-        self._y_cid = self.axes.callbacks.connect('ylim_changed', self.__static_update__)
+        self._x_cid = self.axes.callbacks.connect(
+            "xlim_changed", self.__static_update__
+        )
+        self._y_cid = self.axes.callbacks.connect(
+            "ylim_changed", self.__static_update__
+        )
 
     def __static_update__(self, event=None):
         xlim = self.axes.get_xlim()
         ylim = self.axes.get_ylim()
 
         self.xg = np.linspace(xlim[0], xlim[1], self.resolution)
         self.yg = np.linspace(ylim[0], ylim[1], self.resolution)
         self.grid_index = self.extractor.get_grid_index(self.xg, self.yg)
 
         u, v = self.__get_data__()
+        msk = u.mask  # This is for the first timestep when Vx Vy = 0.
+        if self.norm == True:
+            r = np.power(np.add(np.power(u, 2), np.power(v, 2)), 0.5)
+        else:
+            r = 1
+        u = u / r
+        v = v / r
 
         x, y = [arr.flatten() for arr in np.meshgrid(self.xg, self.yg)]
         xy = np.hstack((x[:, np.newaxis], y[:, np.newaxis]))
 
         self.quiver.set_offsets(xy)
         self.quiver.N = xy.shape[0]
         self.quiver.set_UVC(u.flatten(), v.flatten())
 
     def __dynamic_update__(self):
         u, v = self.__get_data__()
-        self.quiver.set_UVC(u, v)
+        if self.norm == True:
+            r = np.power(np.add(np.power(u, 2), np.power(v, 2)), 0.5)
+        else:
+            r = 1
+        self.quiver.set_UVC(u / r, v / r)
 
     def zoom(self):
-        self.axes.set_xlim([np.min(self.extractor.node_x), np.max(self.extractor.node_x)])
-        self.axes.set_ylim([np.min(self.extractor.node_y), np.max(self.extractor.node_y)])
+        self.axes.set_xlim(
+            [np.min(self.extractor.node_x), np.max(self.extractor.node_x)]
+        )
+        self.axes.set_ylim(
+            [np.min(self.extractor.node_y), np.max(self.extractor.node_y)]
+        )
 
 
 class CurtainPatch(Visual):
     """
     Class for dynamic visualization of model result curtain extracts as collection of patches.
 
     Arguments
@@ -432,33 +550,45 @@
     Returns
     -------
     :param curtain -- object | CurtainPatch instance.
 
     Examples
     --------
     >> xtr = FvExtractor('my_file_3D.nc')
-    >> curtain = SheetContour(axes, xtr, polyline, 'SAL')
+    >> curtain = CurtainPatch(axes, xtr, polyline, 'SAL')
     """
 
     def __init__(self, axes, extractor, expression, polyline, **kwargs):
         self.polyline = polyline
         self.x_data = extractor.get_intersection_data(polyline)
         self.index = extractor.get_curtain_cell_index(polyline)
 
         # Call initialize method of super class
         super(CurtainPatch, self).__init__(axes, extractor, expression, **kwargs)
 
     def __get_data__(self):
-        self.geo = self.extractor.get_curtain_cell_geo(self._time_index, self.polyline, self.x_data, self.index)
-
-        args = (self.expression, self._time_index, self.polyline, self.x_data, self.index)
-        return self.extractor.get_curtain_cell(*args)
+        self.geo = self.extractor.get_curtain_cell_geo(
+            self._time_index, self.polyline, self.x_data, self.index
+        )
+
+        args = (
+            self.expression,
+            self._time_index,
+            self.polyline,
+            self.x_data,
+            self.index,
+        )
+        return self.extractor.get_curtain_cell(*args, **self.expression_kwargs)
 
     def __prep_graphics_obj__(self, **kwargs):
-        data = self.__get_data__()
+        if self.custom_data:
+            data = self.vardata
+        else:
+            data = self.__get_data__()
+
         node_x, node_y, cell_node = self.geo
 
         xy = np.dstack((node_x[cell_node], node_y[cell_node]))
         self.patch = PolyCollection(xy, array=data, **kwargs)
 
         # Add the graphics object to axes
         self.axes.add_collection(self.patch)
@@ -494,52 +624,91 @@
     Returns
     -------
     :param curtain -- object | CurtainPatch instance.
 
     Examples
     --------
     >> xtr = FvExtractor('my_file_3D.nc')
-    >> curtain = SheetContour(axes, xtr, polyline, ['hyp(V_x, V_y)', 'W'])
+    >> curtain = SheetContour(axes, xtr, polyline, ['V', 'W'])
     """
 
-    def __init__(self, axes, extractor, expression, polyline, **kwargs):
+    def __init__(
+        self, axes, extractor, expression, polyline, tangential=True, **kwargs
+    ):
         self.polyline = polyline
         self.x_data = extractor.get_intersection_data(polyline)
         self.index = extractor.get_curtain_cell_index(polyline)
+        self.tangential = tangential
 
         self.xg = np.array([0, 1])
         self.yg = np.array([0, 1])
 
         # Call initialize method of super class
         super(CurtainVector, self).__init__(axes, extractor, expression, **kwargs)
 
     def __get_data__(self):
-        self.geo = self.extractor.get_curtain_cell_geo(self._time_index, self.polyline, self.x_data, self.index)
-
-        args = (self._time_index, self.polyline, self.xg, self.yg, self.x_data, self.index)
+        self.geo = self.extractor.get_curtain_cell_geo(
+            self._time_index,
+            self.polyline,
+            self.x_data,
+            self.index,
+            return_unit_vector=True,
+        )
+
+        args = (
+            self._time_index,
+            self.polyline,
+            self.xg,
+            self.yg,
+            self.x_data,
+            self.index,
+        )
+        
         u = self.extractor.get_curtain_grid(self.expression[0], *args)
         v = self.extractor.get_curtain_grid(self.expression[1], *args)
 
+        # Get the tangential component to the patch faces
+        if self.tangential:
+            grid_index = Mesh(*self.geo[:3]).get_grid_index(self.xg, self.yg)
+            mask = np.equal(grid_index, -999)
+            valid = np.equal(mask, False)
+            uv = np.stack((u.ravel(), v.ravel()))
+
+            utang = self.geo[4]
+            utang_msk = utang[:, grid_index[valid]]
+            tang = np.sum(uv[:, valid.ravel()].conj() * utang_msk, axis=0)
+
+            u[valid] = -tang * utang_msk[0, :]
+
+            if "W" in self.extractor.variables:
+                v[valid] = self.extractor.get_curtain_grid("W", *args)[valid]
+            else:
+                v[valid] = 0
+
         return u, v
 
     def __prep_graphics_obj__(self, **kwargs):
         # Pop key word arguments which are not used by the graphics object
-        self.resolution = kwargs.pop('resolution', 40)
+        self.resolution = kwargs.pop("resolution", 40)
 
         # Update geometry
         self.__get_data__()
 
         # Instantiate graphics object with no data, data will be added on draw event automatically
-        self.quiver = Quiver(self.axes, np.mean(self.geo[0]), np.mean(self.geo[1]), 0, 0, **kwargs)
+        self.quiver = Quiver(
+            self.axes, np.mean(self.geo[0]), np.mean(self.geo[1]), 0, 0, **kwargs
+        )
 
         # Add the graphics object to axes
         self.axes.add_collection(self.quiver)
 
         # Connect the regrid method to the draw event of the figure object.
-        self._cid = self.axes.figure.canvas.mpl_connect('draw_event', lambda event: self.__dynamic_update__())
+        self._cid = self.axes.figure.canvas.mpl_connect(
+            "draw_event", lambda event: self.__dynamic_update__()
+        )
 
     def __static_update__(self):
         pass
 
     def __dynamic_update__(self):
         xlim = self.axes.get_xlim()
         ylim = self.axes.get_ylim()
@@ -584,37 +753,42 @@
 
     def __init__(self, axes, extractor, expression, point, **kwargs):
         self.point = point
 
         super(ProfileCell, self).__init__(axes, extractor, expression, **kwargs)
 
     def __get_data__(self):
-        self.elevation = self.extractor.get_profile_cell_geo(self._time_index, self.point)
+        self.elevation = self.extractor.get_profile_cell_geo(
+            self._time_index, self.point
+        )
 
         args = (self.expression, self._time_index, self.point)
-        return self.extractor.get_profile_cell(*args)
+        return self.extractor.get_profile_cell(*args, **self.expression_kwargs)
 
     def __prep_graphics_obj__(self, **kwargs):
-        data = self.__get_data__()
+        if self.custom_data:
+            data = self.vardata
+        else:
+            data = self.__get_data__()
         self.line = Line2D(data, self.elevation, **kwargs)
 
         self.axes.add_line(self.line)
 
     def __static_update__(self):
         pass
 
     def __dynamic_update__(self):
         data = self.__get_data__()
         self.line.set_data(data, self.elevation)
 
     def zoom(self):
         data = self.__get_data__()
         if data.min() != 0 and data.max() != 0:
-            self.axes.set_xlim([data.min()*0.95, data.max()*1.05])
-        self.axes.set_ylim([self.elevation.min()*0.95, self.elevation.max()*1.05])
+            self.axes.set_xlim([data.min() * 0.95, data.max() * 1.05])
+        self.axes.set_ylim([self.elevation.min() * 0.95, self.elevation.max() * 1.05])
 
 
 class SeriesGlider(Visual):
     """
     Class for dynamic visualization of model result time series extracts with current time marked
 
     Arguments
@@ -635,90 +809,95 @@
 
     Examples
     --------
     >> xtr = FvExtractor('my_file_3D.nc')
     >> profile = ProfileCell(axes, xtr, point, 'SAL')
     """
 
-    def __init__(self, axes, extractor, expression, location, datum='sigma', limits=(0, 1), **kwargs):
+    def __init__(
+        self,
+        axes,
+        extractor,
+        expression,
+        location,
+        datum="sigma",
+        limits=(0, 1),
+        **kwargs
+    ):
         self.location = location
         self.datum = datum
         self.limits = limits
 
         super(SeriesGlider, self).__init__(axes, extractor, expression, **kwargs)
 
     def __get_data__(self):
         args = (self.expression, self.location, self.datum, self.limits)
         return self.extractor.get_data(*args)
 
     def __prep_graphics_obj__(self, **kwargs):
-        self.date_fmt = kwargs.pop('date_fmt', '%d/%m/%Y')
+        self.date_fmt = kwargs.pop("date_fmt", "%d/%m/%Y")
 
         x = self.extractor.time_vector
-        x = datetime(x)
         y = self.__get_data__()
 
         self.time_series = Line2D(x, y, **kwargs)
         self.axes.add_line(self.time_series)
 
-        glider_spec = dict(linewidth=0.8, linestyle='--', color='black')
-        self.glider = Line2D([x[0], x[0]], [-10**20, 10**20], **glider_spec)
+        glider_spec = dict(linewidth=0.8, linestyle="--", color="black")
+        self.glider = Line2D([x[0], x[0]], [-(10**20), 10**20], **glider_spec)
         self.axes.add_line(self.glider)
 
     def __static_update__(self):
         pass
 
     def __dynamic_update__(self):
         tc = self.get_time_current()
         x = np.array([tc, tc])
-        x = datetime(x)
         self.glider.set_xdata(x)
 
     def zoom(self):
         x, y = self.time_series.get_data()
         xlim = [x.min(), x.max()]
         ylim = [y.min(), y.max()]
         self.axes.set_xlim(xlim)
         self.axes.set_ylim(ylim)
 
 
 class HovmollerGlider(Visual):
-
     def __init__(self, axes, extractor, expression, location, **kwargs):
         self.location = location
 
         super(HovmollerGlider, self).__init__(axes, extractor, expression, **kwargs)
 
     def __get_data__(self):
         args = (self.expression, self.location)
-        return self.extractor.get_raw_data(*args).ravel('F')
+        return self.extractor.get_raw_data(*args).ravel("F")
 
     def __prep_graphics_obj__(self, **kwargs):
         self.mesh = self.extractor.get_geometry(self.location)
-        self.mesh.node_x = datetime(self.mesh.node_x)
-        self.mesh.node_x = mdates.date2num(self.mesh.node_x)
-
+        self.mesh.node_x = mdates.date2num(pd.to_datetime(self.mesh.node_x))
         node_x = self.mesh.node_x[self.mesh.cell_node]
         node_y = self.mesh.node_y[self.mesh.cell_node]
         verts = np.dstack((node_x, node_y))
 
         self.patch = PolyCollection(verts, array=self.__get_data__(), **kwargs)
         self.axes.add_collection(self.patch)
 
-        glider_spec = dict(linewidth=0.8, linestyle='--', color='black')
-        self.glider = Line2D(self.time_vector[[0, 0]], [-10 ** 20, 10 ** 20], **glider_spec)
+        glider_spec = dict(linewidth=0.8, linestyle="--", color="black")
+        self.glider = Line2D(
+            self.time_vector[[0, 0]], [-(10**20), 10**20], **glider_spec
+        )
         self.axes.add_line(self.glider)
 
     def __static_update__(self):
         pass
 
     def __dynamic_update__(self):
         tc = self.get_time_current()
         x = np.array([tc, tc])
-        x = datetime(x)
         self.glider.set_xdata(x)
 
     def zoom(self):
         xlim = [self.mesh.node_x.min(), self.mesh.node_x.max()]
         ylim = [self.mesh.node_y.min(), self.mesh.node_y.max()]
         self.axes.set_xlim(xlim)
         self.axes.set_ylim(ylim)
@@ -766,16 +945,28 @@
         Sets the face colouring of the underlying matplotlib.collections object
     antialiased : bool
         Sets the antialiasing state for rendering the underlying matplotlib.collections object
     alpha : float
         Sets the transparencies of the underlying matplotlib.collections object
     """
 
-    def __init__(self, axes, extractor, expression=None, datum=None, limits=None, show=None,
-                 highlight=None, track=0, scale=0.001, shape='tri', **kwargs):
+    def __init__(
+        self,
+        axes,
+        extractor,
+        expression=None,
+        datum=None,
+        limits=None,
+        show=None,
+        highlight=None,
+        track=0,
+        scale=0.001,
+        shape="tri",
+        **kwargs
+    ):
 
         self.datum = datum
         self.limits = limits
         self.track = track
         self.scale = scale
         self.shape = shape
 
@@ -794,41 +985,41 @@
     def __get_data__(self):
         return self.extractor.get_raw_data(self.expression, self._time_index)
 
     def __prep_graphics_obj__(self, **kwargs):
         # Initialize dimensionless shape
         pi = np.pi
         n = None
-        r = pi/2
+        r = pi / 2
 
         shape = self.shape.lower()
-        if shape in ['triangle', 'tri']:
+        if shape in ["triangle", "tri"]:
             n = 3
-        elif shape == 'square':
+        elif shape == "square":
             n = 4
-        elif shape in ['circle', 'o']:
+        elif shape in ["circle", "o"]:
             n = 50
-        elif shape in ['diamond', 'd']:
+        elif shape in ["diamond", "d"]:
             n = 4
             r = 0
-        elif shape == 'star':
+        elif shape == "star":
             rad = np.linspace(0, 2 * pi, 6) - pi / 5 - r
             rad = rad[1, 3, 5, 2, 4, 1]
             self.shape_x = np.cos(rad)
             self.shape_y = np.sin(rad)
         else:
             pass
 
         if n is not None:
             rad = np.linspace(0, 2 * pi, n + 1) - pi / n - r
             self.shape_x = np.cos(rad)
             self.shape_y = np.sin(rad)
 
-        node_x = 0 + self.scale*self.shape_x
-        node_y = 0 + self.scale*self.shape_y
+        node_x = 0 + self.scale * self.shape_x
+        node_y = 0 + self.scale * self.shape_y
 
         xy = np.dstack((node_x, node_y))
         self.patch = PolyCollection(xy, **kwargs)
 
         # Add the graphics object to axes
         self.axes.add_collection(self.patch)
 
@@ -844,73 +1035,79 @@
 
         # Apply additional elevation & inactivity filters
         if self.datum is None and self.limits is None:
             # Get valid particles based on mask only
             valid_lgi = np.invert(self.extractor.get_mask_vector(self._time_index))
         else:
             # Get valid particles based elevation filter (mask applied in get_vertical selection)
-            valid_lgi = self.extractor.get_vertical_selection(self._time_index, self.datum, self.limits)
+            valid_lgi = self.extractor.get_vertical_selection(
+                self._time_index, self.datum, self.limits
+            )
 
         # Update the 'show' logical index
-        show_lgi = (show_lgi & valid_lgi)
+        show_lgi = show_lgi & valid_lgi
 
         # Count number to show
         ns = np.sum(show_lgi)
 
         # Plot the particles
         if ns != 0:
             # Get logical index of particles to highlight
             if self.highlight is None:
                 # Default to highlighting none of the shown particles
                 highlight_lgi = np.zeros((ns,), dtype=np.bool)
             else:
                 # Get highlight logical index (sub setting with the 'show' lgi)
-                highlight_lgi = self.extractor.get_raw_data(self.highlight, self._time_index)[show_lgi]
+                highlight_lgi = self.extractor.get_raw_data(
+                    self.highlight, self._time_index
+                )[show_lgi]
             highlight_lgi[0] = False  # Stops from highlighting all particles (bug)
             nh = np.sum(highlight_lgi)  # Count number to highlight
 
             # Update patch faces (sub setting with the 'show' lgi)
-            x = self.extractor.get_raw_data('x', self._time_index)[show_lgi]
-            y = self.extractor.get_raw_data('y', self._time_index)[show_lgi]
+            x = self.extractor.get_raw_data("x", self._time_index)[show_lgi]
+            y = self.extractor.get_raw_data("y", self._time_index)[show_lgi]
 
-            node_x = x.reshape(x.size, 1) + self.scale*self.shape_x
-            node_y = y.reshape(y.size, 1) + self.scale*self.shape_y
+            node_x = x.reshape(x.size, 1) + self.scale * self.shape_x
+            node_y = y.reshape(y.size, 1) + self.scale * self.shape_y
 
             xy = np.dstack((node_x, node_y))
             self.patch.set_verts(xy)
 
             # Update colours
             if self.expression is None:
                 # Get face colours
                 c = self.patch.get_facecolor()[0]
                 face_colours = np.tile(c, (ns, 1))
 
                 # Finish highlighting with yellow
-                y = np.array([255, 255, 0., 255.]) / 255
+                y = np.array([255, 255, 0.0, 255.0]) / 255
                 face_colours[highlight_lgi, :] = np.tile(y, (nh, 1))
 
                 # Set face colours
                 self.patch.set_facecolor(face_colours)
 
                 # Get edge colours & set edge colors
                 c = self.patch.get_edgecolor()
                 if c.size > 0:
                     # Set edge colours
                     edge_colours = np.tile(c[0], (ns, 1))
                     self.patch.set_edgecolor(edge_colours)
             else:
                 # Get data relating to self.expression (sub setting with the 'show' lgi)
-                data = self.extractor.get_raw_data(self.expression, self._time_index)[show_lgi]
+                data = self.extractor.get_raw_data(self.expression, self._time_index)[
+                    show_lgi
+                ]
 
                 # Get face colours
                 norm = self.patch.norm(data)
                 face_colours = self.patch.cmap(norm)
 
                 # Finish highlighting
-                y = np.array([255, 255, 0., 255]) / 255
+                y = np.array([255, 255, 0.0, 255]) / 255
                 face_colours[highlight_lgi, :] = np.tile(y, (nh, 1))
 
                 # Set face colours
                 self.patch.set_facecolor(face_colours)
 
                 # Get & set edge colours
                 c = self.patch.get_edgecolor()
@@ -926,44 +1123,47 @@
             self.patch.set_verts(xy)
 
     def zoom(self):
         pass
 
 
 class ParticlesHeat(Visual):
-
-    def __init__(self, axes, extractor, expression, datum='sigma', limits=(0, 1), **kwargs):
+    def __init__(
+        self, axes, extractor, expression, datum="sigma", limits=(0, 1), **kwargs
+    ):
         self.datum = datum
         self.limits = limits
 
         # Call initialize method of super class
         super(ParticlesHeat, self).__init__(axes, extractor, expression, **kwargs)
 
     def __get_data__(self):
         args = (self._time_index, self.datum, self.limits, self.count)
 
         return self.extractor.get_particle_density(*args)
 
     def __prep_graphics_obj__(self, **kwargs):
         # Pop key word arguments which are not used by the graphics object
-        self.count = kwargs.pop('count', 10000)
-        self.index = np.arange(0, self.extractor.np, np.ceil(self.extractor.np/self.count)).astype(dtype=np.int32)
+        self.count = kwargs.pop("count", 10000)
+        self.index = np.arange(
+            0, self.extractor.np, np.ceil(self.extractor.np / self.count)
+        ).astype(dtype=np.int32)
 
-        x = self.extractor.get_particle_data('x', self._time_index)[self.index]
-        y = self.extractor.get_particle_data('y', self._time_index)[self.index]
+        x = self.extractor.get_particle_data("x", self._time_index)[self.index]
+        y = self.extractor.get_particle_data("y", self._time_index)[self.index]
 
         # Instantiate graphics object with no data, data will be added on draw event automatically
         self.sca = self.axes.scatter(x, y, **kwargs)
 
     def __static_update__(self):
         pass
 
     def __dynamic_update__(self):
-        x = self.extractor.get_particle_data('x', self._time_index)[self.index]
-        y = self.extractor.get_particle_data('y', self._time_index)[self.index]
+        x = self.extractor.get_particle_data("x", self._time_index)[self.index]
+        y = self.extractor.get_particle_data("y", self._time_index)[self.index]
         data = self.__get_data__()
 
         self.sca.set_offsets(np.column_stack((x, y)))
         self.sca.set_array(data)
 
     def zoom(self):
         pass
@@ -992,20 +1192,24 @@
     Examples
     --------
     >> base_xtr = FvExtractor('my_file_base.nc')
     >> dev_xtr = FvExtractor('my_file_developed.nc')
     >> diff_sheet = DeltaSheetPatch(axes, (base_xtr, dev_xtr), 'H')
     """
 
-    def __init__(self, axes, extractors, expression, datum='sigma', limits=(0, 1), **kwargs):
+    def __init__(
+        self, axes, extractors, expression, datum="sigma", limits=(0, 1), **kwargs
+    ):
         # Store multiple extractor objects
         self.extractors = extractors
 
         # Initialize as super class
-        super(DeltaSheetPatch, self).__init__(axes, self.extractors[0], expression, datum, limits, **kwargs)
+        super(DeltaSheetPatch, self).__init__(
+            axes, self.extractors[0], expression, datum, limits, **kwargs
+        )
 
     def __get_data__(self):
         self.extractor = self.extractors[0]
         data_1 = super(DeltaSheetPatch, self).__get_data__()
 
         self.extractor = self.extractors[1]
         data_2 = super(DeltaSheetPatch, self).__get_data__()
@@ -1035,20 +1239,24 @@
     Examples
     --------
     >> base_xtr = FvExtractor('my_file_base.nc')
     >> dev_xtr = FvExtractor('my_file_developed.nc')
     >> diff_sheet = DeltaSheetContour(axes, (base_xtr, dev_xtr), 'H')
     """
 
-    def __init__(self, axes, extractors, expression, datum='sigma', limits=(0, 1), **kwargs):
+    def __init__(
+        self, axes, extractors, expression, datum="sigma", limits=(0, 1), **kwargs
+    ):
         # Store multiple extractor objects
         self.extractors = extractors
 
         # Initialize as super class
-        super(DeltaSheetContour, self).__init__(axes, self.extractors[0], expression, datum, limits, **kwargs)
+        super(DeltaSheetContour, self).__init__(
+            axes, self.extractors[0], expression, datum, limits, **kwargs
+        )
 
     def __get_data__(self):
         self.extractor = self.extractors[0]
         data_1 = super(DeltaSheetContour, self).__get_data__()
 
         self.extractor = self.extractors[1]
         data_2 = super(DeltaSheetContour, self).__get_data__()
@@ -1078,22 +1286,26 @@
     Examples
     --------
     >> base_xtr = FvExtractor('my_file_base.nc')
     >> dev_xtr = FvExtractor('my_file_developed.nc')
     >> diff_sheet = DeltaSheetVector(axes, (base_xtr, dev_xtr), ['V_x', 'V_y'])
     """
 
-    def __init__(self, axes, extractors, expression, datum='sigma', limits=(0, 1), **kwargs):
+    def __init__(
+        self, axes, extractors, expression, datum="sigma", limits=(0, 1), **kwargs
+    ):
         # Store multiple extractor objects
         self.extractors = extractors
 
         # Initialize as super class
-        super(DeltaSheetVector, self).__init__(axes, self.extractors[0], expression, datum, limits, **kwargs)
+        super(DeltaSheetVector, self).__init__(
+            axes, self.extractors[0], expression, datum, limits, **kwargs
+        )
 
     def __get_data__(self):
         self.extractor = self.extractors[0]
         data_1 = super(DeltaSheetVector, self).__get_data__()
 
         self.extractor = self.extractors[1]
         data_2 = super(DeltaSheetVector, self).__get_data__()
 
-        return data_2[0] - data_1[0], data_2[1] - data_1[1]
+        return data_2[0] - data_1[0], data_2[1] - data_1[1]
```

### Comparing `tfv-0.0.9/tfv.egg-info/PKG-INFO` & `tfv-1.0.0/tfv.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,65 +1,66 @@
 Metadata-Version: 2.1
 Name: tfv
-Version: 0.0.9
+Version: 1.0.0
 Summary: Post processing tools for TUFLOW FV results
 Home-page: https://gitlab.com/TUFLOW/tfv
 Author: Jonah Chorley, Toby Devlin & TUFLOW Support
 Author-email: support@tuflow.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
+Provides-Extra: viewer
 License-File: LICENSE
 
 # TFV
-The tfv package is a suite of tools for post-processing results from the
-[TUFLOW FV](https://www.tuflow.com/Tuflow%20FV.aspx) hydrodynamic, sediment transport, water quality and particle
-tracking modelling software. 
+The tfv package is a suite of tools for post-processing results from the [TUFLOW FV](https://www.tuflow.com/Tuflow%20FV.aspx) hydrodynamic, sediment transport, water quality and particle tracking modelling software. 
 
-It is also provides a basic framework for extracting and visualizing 2D and 3D oceanographic and atmospheric model result data on unstructured
-meshes.
+It is also provides a basic framework for extracting and visualizing 2D and 3D oceanographic and atmospheric model result data on unstructured meshes.
 
 ## Installing
 The tfv package is available via the Python Package Index ([PyPi](https://pypi.org/project/tfv/))
 
-*Note: Version 0.0.9 has been built and tested on Python 3.6 to 3.10*.
+*Note: Version 1.0.0 has been built and tested on Python 3.9 to 3.11*.
 
 From command prompt install and update using pip:
 
 ```
 python -m pip install tfv
 ```
 
-## Dependancies
-The tfv package depends on the following packages:
+## Dependencies
+The tfv package depends on the following core packages:
 
 ```
 matplotlib >= 3.2.2
 netCDF4 >= 1.5.3
 numpy >= 1.19.0
-PyQt5 >= 5.15.0
+xarray>=v2022.03.0
+dask>=2022.01.0
+scipy>=1.6.0
+tqdm>=4.50.0
 ```
 
 These will be automatically installed or updated as part of the tfv installation.
 
+The following packages provide additional functionality and are **not** installed by default:
+
+`ipywidgets >= 8.0.0` - Required for interactive results vizulisation in an interactive session (e.g., JuypterLab)
+
+`PyQt5 >= 5.15.0`  - Required for interactive popout results vizulisation
+
 ## Tutorials, Documentation & Support
 See the [API Reference](https://tfv.readthedocs.io/en/latest/) for code documentation and
 [TUFLOW FV Python Tools](https://fvwiki.tuflow.com/index.php?title=FV_Python_Tools) for tutorials and demonstration 
 datasets. 
 
 For support contact [TUFLOW Support](mailto:support@tuflow.com).
 
 ## Authors
 * **Jonah Chorley**
 * **Toby Devlin**
 * **TUFLOW Support**
 
 ## License
 This project is licensed under the MIT License - see the [LICENSE.txt](https://gitlab.com/TUFLOW/tfv/blob/master/LICENSE) file for details
-
-
-
-
```

