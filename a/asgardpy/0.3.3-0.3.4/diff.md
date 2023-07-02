# Comparing `tmp/asgardpy-0.3.3.tar.gz` & `tmp/asgardpy-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asgardpy-0.3.3.tar", last modified: Tue Jun 20 14:25:41 2023, max compression
+gzip compressed data, was "asgardpy-0.3.4.tar", last modified: Sun Jul  2 20:26:38 2023, max compression
```

## Comparing `asgardpy-0.3.3.tar` & `asgardpy-0.3.4.tar`

### file list

```diff
@@ -1,37 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:25:41.810742 asgardpy-0.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11353 2023-06-20 14:25:11.000000 asgardpy-0.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-06-20 14:25:41.810742 asgardpy-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-06-20 14:25:11.000000 asgardpy-0.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:25:41.806741 asgardpy-0.3.3/asgardpy/
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-06-20 14:25:11.000000 asgardpy-0.3.3/asgardpy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:25:41.806741 asgardpy-0.3.3/asgardpy/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-20 14:25:11.000000 asgardpy-0.3.3/asgardpy/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7842 2023-06-20 14:25:11.000000 asgardpy-0.3.3/asgardpy/analysis/analysis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:25:41.806741 asgardpy-0.3.3/asgardpy/base/
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-06-20 14:25:11.000000 asgardpy-0.3.3/asgardpy/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4095 2023-06-20 14:25:11.000000 asgardpy-0.3.3/asgardpy/base/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-06-20 14:25:11.000000 asgardpy-0.3.3/asgardpy/base/geom.py
--rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-06-20 14:25:11.000000 asgardpy-0.3.3/asgardpy/base/reduction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:25:41.806741 asgardpy-0.3.3/asgardpy/config/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-20 14:25:11.000000 asgardpy-0.3.3/asgardpy/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5657 2023-06-20 14:25:11.000000 asgardpy-0.3.3/asgardpy/config/generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:25:41.810742 asgardpy-0.3.3/asgardpy/data/
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-06-20 14:25:12.000000 asgardpy-0.3.3/asgardpy/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14528 2023-06-20 14:25:12.000000 asgardpy-0.3.3/asgardpy/data/dataset_1d.py
--rw-r--r--   0 runner    (1001) docker     (123)    24797 2023-06-20 14:25:12.000000 asgardpy-0.3.3/asgardpy/data/dataset_3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     5146 2023-06-20 14:25:12.000000 asgardpy-0.3.3/asgardpy/data/dl4.py
--rw-r--r--   0 runner    (1001) docker     (123)    32564 2023-06-20 14:25:12.000000 asgardpy-0.3.3/asgardpy/data/target.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:25:41.810742 asgardpy-0.3.3/asgardpy/io/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-20 14:25:12.000000 asgardpy-0.3.3/asgardpy/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6120 2023-06-20 14:25:12.000000 asgardpy-0.3.3/asgardpy/io/io.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:25:12.000000 asgardpy-0.3.3/asgardpy/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-06-20 14:25:12.000000 asgardpy-0.3.3/asgardpy/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:25:41.806741 asgardpy-0.3.3/asgardpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-06-20 14:25:41.000000 asgardpy-0.3.3/asgardpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-06-20 14:25:41.000000 asgardpy-0.3.3/asgardpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 14:25:41.000000 asgardpy-0.3.3/asgardpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-06-20 14:25:41.000000 asgardpy-0.3.3/asgardpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-20 14:25:41.000000 asgardpy-0.3.3/asgardpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-20 14:25:12.000000 asgardpy-0.3.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-06-20 14:25:41.810742 asgardpy-0.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-06-20 14:25:12.000000 asgardpy-0.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 20:26:38.111688 asgardpy-0.3.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11353 2023-07-02 20:26:16.000000 asgardpy-0.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-07-02 20:26:38.115688 asgardpy-0.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-07-02 20:26:16.000000 asgardpy-0.3.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 20:26:38.111688 asgardpy-0.3.4/asgardpy/
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-02 20:26:16.000000 asgardpy-0.3.4/asgardpy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 20:26:38.111688 asgardpy-0.3.4/asgardpy/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-02 20:26:16.000000 asgardpy-0.3.4/asgardpy/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7842 2023-07-02 20:26:16.000000 asgardpy-0.3.4/asgardpy/analysis/analysis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 20:26:38.111688 asgardpy-0.3.4/asgardpy/base/
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-07-02 20:26:16.000000 asgardpy-0.3.4/asgardpy/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4095 2023-07-02 20:26:16.000000 asgardpy-0.3.4/asgardpy/base/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-07-02 20:26:16.000000 asgardpy-0.3.4/asgardpy/base/geom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-07-02 20:26:16.000000 asgardpy-0.3.4/asgardpy/base/reduction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 20:26:38.111688 asgardpy-0.3.4/asgardpy/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-02 20:26:16.000000 asgardpy-0.3.4/asgardpy/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6218 2023-07-02 20:26:16.000000 asgardpy-0.3.4/asgardpy/config/generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 20:26:38.111688 asgardpy-0.3.4/asgardpy/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-07-02 20:26:16.000000 asgardpy-0.3.4/asgardpy/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4105 2023-07-02 20:26:16.000000 asgardpy-0.3.4/asgardpy/data/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14803 2023-07-02 20:26:16.000000 asgardpy-0.3.4/asgardpy/data/dataset_1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24791 2023-07-02 20:26:16.000000 asgardpy-0.3.4/asgardpy/data/dataset_3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4979 2023-07-02 20:26:16.000000 asgardpy-0.3.4/asgardpy/data/dl4.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35824 2023-07-02 20:26:16.000000 asgardpy-0.3.4/asgardpy/data/target.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 20:26:38.111688 asgardpy-0.3.4/asgardpy/io/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-02 20:26:16.000000 asgardpy-0.3.4/asgardpy/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6120 2023-07-02 20:26:16.000000 asgardpy-0.3.4/asgardpy/io/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 20:26:16.000000 asgardpy-0.3.4/asgardpy/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-02 20:26:16.000000 asgardpy-0.3.4/asgardpy/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 20:26:38.111688 asgardpy-0.3.4/asgardpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-07-02 20:26:38.000000 asgardpy-0.3.4/asgardpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-02 20:26:38.000000 asgardpy-0.3.4/asgardpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 20:26:38.000000 asgardpy-0.3.4/asgardpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-07-02 20:26:38.000000 asgardpy-0.3.4/asgardpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-02 20:26:38.000000 asgardpy-0.3.4/asgardpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-02 20:26:16.000000 asgardpy-0.3.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-02 20:26:38.115688 asgardpy-0.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-07-02 20:26:16.000000 asgardpy-0.3.4/setup.py
```

### Comparing `asgardpy-0.3.3/LICENSE` & `asgardpy-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `asgardpy-0.3.3/PKG-INFO` & `asgardpy-0.3.4/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asgardpy
-Version: 0.3.3
+Version: 0.3.4
 Summary: Gammapy-based pipeline for easy joint analysis of different gamma-ray datasets
 Home-page: https://github.com/chaimain/asgardpy
 Download-URL: https://github.com/chaimain/asgardpy/archive/refs/tags/v0.3.1.tar.gz
 Author: Chaitanya Priyadarshi
 Author-email: chaitanya.p.astrphys@gmail.com
 License: Apache
 Classifier: Intended Audience :: Science/Research
@@ -17,24 +17,24 @@
 Provides-Extra: dev
 License-File: LICENSE
 
 # asgardpy [![Build Status](https://github.com/chaimain/asgardpy/actions/workflows/main.yml/badge.svg?branch=main)](https://github.com/chaimain/asgardpy/actions?query=branch%3Amain) [![gammapy](https://img.shields.io/badge/powered%20by-gammapy-orange.svg?style=flat)](https://www.gammapy.org/) [![astropy](http://img.shields.io/badge/powered%20by-AstroPy-orange.svg?style=flat)](https://www.astropy.org/)
 ## Analysis Software for GAmma-Ray Data in Python
 
 'User-friendly' configuration-centred pipeline built over [Gammapy](https://github.com/gammapy/gammapy) to allow for easy simultaneous analysis of various datasets of different formats.
-Example: 3D Fermi-LAT (with various source models in the Region of Interest stored in XML file) + 1D energy-dependent selection cut MAGIC/LST [PointSkyRegion geometry for ON region] + 1D fixed-cut VERITAS [CircleSkyRegion geometry for ON region].
+Example: 3D Fermi-LAT (with various source models in the Region of Interest stored in XML file) + 1D energy-dependent directional cuts MAGIC/LST [PointSkyRegion geometry for ON region] + 1D global directional cut VERITAS [CircleSkyRegion geometry for ON region].
 
 Follow the documentation at https://asgardpy.readthedocs.io/en/latest/ for the main functionality of this pipeline.
 Follow the [Gammapy v1.1](https://docs.gammapy.org/1.1/) documentation for understanding the core Gammapy objects.
 
 The various Data Levels	used here follow the descriptions suggested by [GADF v0.3](https://gamma-astro-data-formats.readthedocs.io/en/latest/) and CTAO Data Model
 
 # Pipeline development
 
-The pipeline was developed with first testing with Fermi-LAT ([enrico](https://enrico.readthedocs.io/en/latest/) and [fermipy](https://fermipy.readthedocs.io/en/latest/)) files and LST-1 ([cta-lstchain](https://cta-observatory.github.io/cta-lstchain/)) DL3 files (with energy-dependent selection cuts) for point-like sources.
+The pipeline was developed with first testing with Fermi-LAT ([enrico](https://enrico.readthedocs.io/en/latest/) and [fermipy](https://fermipy.readthedocs.io/en/latest/)) files and LST-1 ([cta-lstchain](https://cta-observatory.github.io/cta-lstchain/)) DL3 files (with energy-dependent and global directional cuts) for point-like sources.
 The pipeline can be further expanded to support more types of DL3 files of gamma-ray instruments.
 
 An example of configuration file that can be used with asgardpy can be found at ``asgardpy/config/template.yaml``
 Examples of usage of asgardpy is shown in jupyter notebooks in ``notebooks/`` but as there are no public test data included with the pipeline yet, the results are empty.
 
 # Pipeline Template
```

### Comparing `asgardpy-0.3.3/README.md` & `asgardpy-0.3.4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # asgardpy [![Build Status](https://github.com/chaimain/asgardpy/actions/workflows/main.yml/badge.svg?branch=main)](https://github.com/chaimain/asgardpy/actions?query=branch%3Amain) [![gammapy](https://img.shields.io/badge/powered%20by-gammapy-orange.svg?style=flat)](https://www.gammapy.org/) [![astropy](http://img.shields.io/badge/powered%20by-AstroPy-orange.svg?style=flat)](https://www.astropy.org/)
 ## Analysis Software for GAmma-Ray Data in Python
 
 'User-friendly' configuration-centred pipeline built over [Gammapy](https://github.com/gammapy/gammapy) to allow for easy simultaneous analysis of various datasets of different formats.
-Example: 3D Fermi-LAT (with various source models in the Region of Interest stored in XML file) + 1D energy-dependent selection cut MAGIC/LST [PointSkyRegion geometry for ON region] + 1D fixed-cut VERITAS [CircleSkyRegion geometry for ON region].
+Example: 3D Fermi-LAT (with various source models in the Region of Interest stored in XML file) + 1D energy-dependent directional cuts MAGIC/LST [PointSkyRegion geometry for ON region] + 1D global directional cut VERITAS [CircleSkyRegion geometry for ON region].
 
 Follow the documentation at https://asgardpy.readthedocs.io/en/latest/ for the main functionality of this pipeline.
 Follow the [Gammapy v1.1](https://docs.gammapy.org/1.1/) documentation for understanding the core Gammapy objects.
 
 The various Data Levels	used here follow the descriptions suggested by [GADF v0.3](https://gamma-astro-data-formats.readthedocs.io/en/latest/) and CTAO Data Model
 
 # Pipeline development
 
-The pipeline was developed with first testing with Fermi-LAT ([enrico](https://enrico.readthedocs.io/en/latest/) and [fermipy](https://fermipy.readthedocs.io/en/latest/)) files and LST-1 ([cta-lstchain](https://cta-observatory.github.io/cta-lstchain/)) DL3 files (with energy-dependent selection cuts) for point-like sources.
+The pipeline was developed with first testing with Fermi-LAT ([enrico](https://enrico.readthedocs.io/en/latest/) and [fermipy](https://fermipy.readthedocs.io/en/latest/)) files and LST-1 ([cta-lstchain](https://cta-observatory.github.io/cta-lstchain/)) DL3 files (with energy-dependent and global directional cuts) for point-like sources.
 The pipeline can be further expanded to support more types of DL3 files of gamma-ray instruments.
 
 An example of configuration file that can be used with asgardpy can be found at ``asgardpy/config/template.yaml``
 Examples of usage of asgardpy is shown in jupyter notebooks in ``notebooks/`` but as there are no public test data included with the pipeline yet, the results are empty.
 
 # Pipeline Template
```

### Comparing `asgardpy-0.3.3/asgardpy/analysis/analysis.py` & `asgardpy-0.3.4/asgardpy/analysis/analysis.py`

 * *Files identical despite different names*

### Comparing `asgardpy-0.3.3/asgardpy/base/__init__.py` & `asgardpy-0.3.4/asgardpy/base/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,17 +17,15 @@
     EnergyAxisConfig,
     EnergyEdgesCustomConfig,
     GeomConfig,
     MapAxesConfig,
     MapFrameShapeConfig,
     ProjectionEnum,
     SelectionConfig,
-    SkyCoordConfig,
-    SpatialCircleConfig,
-    SpatialPointConfig,
+    SkyPositionConfig,
     WcsConfig,
     get_energy_axis,
 )
 from asgardpy.base.reduction import (
     BackgroundConfig,
     BackgroundMethodEnum,
     ExclusionRegionsConfig,
@@ -63,17 +61,15 @@
     "ProjectionEnum",
     "ReductionTypeEnum",
     "RegionsConfig",
     "RequiredHDUEnum",
     "SafeMaskConfig",
     "SafeMaskMethodsEnum",
     "SelectionConfig",
-    "SpatialCircleConfig",
-    "SpatialPointConfig",
-    "SkyCoordConfig",
+    "SkyPositionConfig",
     "TimeFormatEnum",
     "TimeIntervalsConfig",
     "TimeRangeConfig",
     "TimeType",
     "WcsConfig",
     "get_energy_axis",
 ]
```

### Comparing `asgardpy-0.3.3/asgardpy/base/base.py` & `asgardpy-0.3.4/asgardpy/base/base.py`

 * *Files identical despite different names*

### Comparing `asgardpy-0.3.3/asgardpy/base/geom.py` & `asgardpy-0.3.4/asgardpy/base/geom.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,36 +14,21 @@
     "EnergyAxisConfig",
     "EnergyEdgesCustomConfig",
     "GeomConfig",
     "MapAxesConfig",
     "MapFrameShapeConfig",
     "ProjectionEnum",
     "SelectionConfig",
-    "SkyCoordConfig",
-    "SpatialCircleConfig",
-    "SpatialPointConfig",
+    "SkyPositionConfig",
     "WcsConfig",
     "get_energy_axis",
 ]
 
 
 # Basic Components to define the main GeomConfig
-class SpatialCircleConfig(BaseConfig):
-    frame: FrameEnum = FrameEnum.icrs
-    lon: AngleType = 0 * u.deg
-    lat: AngleType = 0 * u.deg
-    radius: AngleType = 0.1 * u.rad
-
-
-class SpatialPointConfig(BaseConfig):
-    frame: FrameEnum = FrameEnum.icrs
-    lon: AngleType = 0 * u.deg
-    lat: AngleType = 0 * u.deg
-
-
 class EnergyAxisConfig(BaseConfig):
     min: EnergyType = 1 * u.GeV
     max: EnergyType = 1 * u.TeV
     nbins: int = 5
     per_decade: bool = True
 
 
@@ -63,27 +48,28 @@
 
 
 class MapFrameShapeConfig(BaseConfig):
     width: AngleType = 5 * u.deg
     height: AngleType = 5 * u.deg
 
 
-class SkyCoordConfig(BaseConfig):
+class SkyPositionConfig(BaseConfig):
     frame: FrameEnum = FrameEnum.icrs
     lon: AngleType = 0 * u.deg
     lat: AngleType = 0 * u.deg
+    radius: AngleType = 0 * u.deg
 
 
 class ProjectionEnum(str, Enum):
     tan = "TAN"
     car = "CAR"
 
 
 class WcsConfig(BaseConfig):
-    skydir: SkyCoordConfig = SkyCoordConfig()
+    skydir: SkyPositionConfig = SkyPositionConfig()
     binsize: AngleType = 0.1 * u.deg
     proj: ProjectionEnum = ProjectionEnum.tan
     map_frame_shape: MapFrameShapeConfig = MapFrameShapeConfig()
     binsize_irf: AngleType = 0.2 * u.deg
 
 
 class GeomConfig(BaseConfig):
```

### Comparing `asgardpy-0.3.3/asgardpy/base/reduction.py` & `asgardpy-0.3.4/asgardpy/base/reduction.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 from astropy import units as u
 
 from asgardpy.base import (
     AngleType,
     BaseConfig,
     PathType,
-    SkyCoordConfig,
+    SkyPositionConfig,
     TimeIntervalsConfig,
 )
 
 __all__ = [
     "BackgroundConfig",
     "BackgroundMethodEnum",
     "BackgroundRegionFinderMethodEnum",
@@ -79,15 +79,15 @@
     n_off_regions: int = 1
     binsz: AngleType = 0.05 * u.deg
 
 
 class RegionsConfig(BaseConfig):
     type: str = ""
     name: str = ""
-    position: SkyCoordConfig = SkyCoordConfig()
+    position: SkyPositionConfig = SkyPositionConfig()
     parameters: dict = {}
 
 
 class ExclusionRegionsConfig(BaseConfig):
     target_source: bool = True
     regions: List[RegionsConfig] = []
```

### Comparing `asgardpy-0.3.3/asgardpy/config/generator.py` & `asgardpy-0.3.4/asgardpy/config/generator.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import json
 import logging
+from enum import Enum
 from pathlib import Path
 from typing import List
 
 import yaml
 from gammapy.utils.scripts import make_path, read_yaml
 from pydantic.utils import deep_update
 
@@ -12,40 +13,61 @@
     Dataset1DConfig,
     Dataset3DConfig,
     FitConfig,
     FluxPointsConfig,
     Target,
 )
 
-__all__ = ["AsgardpyConfig", "recursive_merge_dicts"]
+__all__ = [
+    "AsgardpyConfig",
+    "get_model_template",
+    "recursive_merge_dicts",
+]
 
-CONFIG_PATH = Path(__file__).resolve().parent / "config"
-DOCS_FILE = CONFIG_PATH / "docs.yaml"
+CONFIG_PATH = Path(__file__).resolve().parent
 
 log = logging.getLogger(__name__)
 
 
 # Other general config params
 class LogConfig(BaseConfig):
     level: str = "info"
     filename: str = ""
     filemode: str = "w"
     format: str = ""
     datefmt: str = ""
 
 
+class ParallelBackendEnum(str, Enum):
+    multi = "multiprocessing"
+    ray = "ray"
+
+
 class GeneralConfig(BaseConfig):
     log: LogConfig = LogConfig()
     outdir: PathType = PathType(".")
     n_jobs: int = 1
+    parallel_backend: ParallelBackendEnum = ParallelBackendEnum.multi
     steps: List[AnalysisStepEnum] = []
     overwrite: bool = True
     stacked_dataset: bool = False
 
 
+def get_model_template(spec_model_tag):
+    """
+    Read a particular template model yaml file into AsgardpyConfig object.
+    """
+    template_files = sorted(list(CONFIG_PATH.glob("model_template*yaml")))
+    new_model_file = None
+    for file in template_files:
+        if spec_model_tag == file.name.split("_")[-1].split(".")[0]:
+            new_model_file = file
+    return new_model_file
+
+
 def recursive_merge_dicts(a, b):
     """
     recursively merge two dictionaries.
     Entries in b override entries in a. The built-in update function cannot be
     used for hierarchical dicts.
 
     Also for the case when there is a list of dicts involved, one has to be more careful.
```

### Comparing `asgardpy-0.3.3/asgardpy/data/__init__.py` & `asgardpy-0.3.4/asgardpy/data/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,14 +17,16 @@
     FluxPointsConfig,
 )
 from asgardpy.data.target import (
     BrokenPowerLaw2SpectralModel,
     ExpCutoffLogParabolaSpectralModel,
     Target,
     apply_selection_mask_to_models,
+    check_model_preference_aic,
+    check_model_preference_lrt,
     config_to_dict,
     create_gal_diffuse_skymodel,
     create_iso_diffuse_skymodel,
     create_source_skymodel,
     set_models,
     xml_spatial_model_to_gammapy,
     xml_spectral_model_to_gammapy_params,
@@ -44,14 +46,16 @@
     "BrokenPowerLaw2SpectralModel",
     "ExpCutoffLogParabolaSpectralModel",
     "set_models",
     "apply_selection_mask_to_models",
     "config_to_dict",
     "xml_spectral_model_to_gammapy_params",
     "xml_spatial_model_to_gammapy",
+    "check_model_preference_aic",
+    "check_model_preference_lrt",
     "create_source_skymodel",
     "create_iso_diffuse_skymodel",
     "create_gal_diffuse_skymodel",
     "SpatialCircleConfig",
     "SpatialPointConfig",
     "Dataset1DConfig",
     "Dataset1DGeneration",
```

### Comparing `asgardpy-0.3.3/asgardpy/data/dataset_1d.py` & `asgardpy-0.3.4/asgardpy/data/dataset_1d.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from astropy.coordinates import SkyCoord
 from astropy.time import Time
 
 # from gammapy.analysis import Analysis, AnalysisConfig - no support for DL3 with RAD_MAX
 from gammapy.data import DataStore
 from gammapy.datasets import Datasets, SpectrumDataset
 from gammapy.makers import (
+    DatasetsMaker,
     ReflectedRegionsBackgroundMaker,
     ReflectedRegionsFinder,
     SafeMaskMaker,
     SpectrumDatasetMaker,
     WobbleRegionsFinder,
 )
 from gammapy.maps import RegionGeom, WcsGeom
@@ -30,15 +31,15 @@
     BaseConfig,
     GeomConfig,
     MapAxesConfig,
     MapSelectionEnum,
     ObservationsConfig,
     ReductionTypeEnum,
     SafeMaskConfig,
-    SpatialPointConfig,
+    SkyPositionConfig,
     get_energy_axis,
 )
 from asgardpy.io import DL3Files, InputConfig
 
 __all__ = [
     "Datasets1DAnalysisStep",
     "Dataset1DBaseConfig",
@@ -53,15 +54,15 @@
 # Defining various components of 1D Dataset Config section
 class Dataset1DInfoConfig(BaseConfig):
     name: str = "dataset-name"
     geom: GeomConfig = GeomConfig()
     observation: ObservationsConfig = ObservationsConfig()
     background: BackgroundConfig = BackgroundConfig()
     safe_mask: SafeMaskConfig = SafeMaskConfig()
-    on_region: SpatialPointConfig = SpatialPointConfig()
+    on_region: SkyPositionConfig = SkyPositionConfig()
     containment_correction: bool = True
     map_selection: List[MapSelectionEnum] = []
     spectral_energy_range: MapAxesConfig = MapAxesConfig()
 
 
 class Dataset1DBaseConfig(BaseConfig):
     name: str = "Instrument-name"
@@ -92,17 +93,15 @@
         instrument_spectral_info = {"name": [], "spectral_energy_ranges": []}
 
         # Iterate over all instrument information given:
         for i in np.arange(len(instruments_list)):
             config_1d_dataset = instruments_list[i]
             instrument_spectral_info["name"].append(config_1d_dataset.name)
 
-            generate_1d_dataset = Dataset1DGeneration(
-                self.log, config_1d_dataset, self.config.target
-            )
+            generate_1d_dataset = Dataset1DGeneration(self.log, config_1d_dataset, self.config)
             dataset = generate_1d_dataset.run()
 
             # Get the spectral energy information for each Instrument Dataset
             energy_axes = config_1d_dataset.dataset_info.spectral_energy_range
             if len(energy_axes.axis_custom.edges) > 0:
                 energy_bin_edges = get_energy_axis(energy_axes, only_edges=True, custom_range=True)
             else:
@@ -140,19 +139,21 @@
     3. Create the base dataset template, including the main counts geometry.
 
     4. Prepare standard data reduction makers using the parameters passed in the config.
 
     5. Generate the final dataset.
     """
 
-    def __init__(self, log, config_1d_dataset, config_target):
+    def __init__(self, log, config_1d_dataset, config_full):
         self.config_1d_dataset_io = config_1d_dataset.io
         self.log = log
         self.config_1d_dataset_info = config_1d_dataset.dataset_info
-        self.config_target = config_target
+        self.config_target = config_full.target
+        self.n_jobs = config_full.general.n_jobs
+        self.parallel_backend = config_full.general.parallel_backend
         self.exclusion_regions = []
         self.datasets = Datasets()
 
     def run(self):
         # First check for the given file list if they are readable or not.
         file_list = {}
         dl3_info = DL3Files(
@@ -241,15 +242,15 @@
                 u.Quantity(self.config_target.sky_position.lon),
                 u.Quantity(self.config_target.sky_position.lat),
                 frame=self.config_target.sky_position.frame,
             )
 
         # Defining the ON region's geometry
         given_on_geom = self.config_1d_dataset_info.on_region
-        if ~hasattr(given_on_geom, "radius"):
+        if given_on_geom.radius == 0 * u.deg:
             on_region = PointSkyRegion(src_pos)
             # Hack to allow for the joint fit
             # (otherwise pointskyregion.contains returns None)
             on_region.meta = {"include": False}
 
         else:
             on_region = CircleSkyRegion(
@@ -365,26 +366,36 @@
         return safe_maker
 
     def generate_dataset(
         self, observations, dataset_template, dataset_maker, bkg_maker, safe_maker
     ):
         """
         From the given Observations, Dataset Template and various Makers,
-        produce the DatasetOnOff object and append it to the Datasets object.
+        use the multiprocessing method with DatasetsMaker and update the
+        datasets accordingly.
         """
-        for obs in observations:
-            dataset = dataset_maker.run(dataset_template.copy(name=str(obs.obs_id)), obs)
+        if safe_maker:
+            makers = [dataset_maker, safe_maker, bkg_maker]
+        else:
+            makers = [dataset_maker, bkg_maker]
+
+        datasets_maker = DatasetsMaker(
+            makers,
+            stack_datasets=False,
+            n_jobs=self.n_jobs,
+            parallel_backend=self.parallel_backend,
+        )
+        self.datasets = datasets_maker.run(dataset_template, observations)
 
-            dataset_on_off = bkg_maker.run(dataset, obs)
+        safe_cfg = self.config_1d_dataset_info.safe_mask
+        pars = safe_cfg.parameters
 
-            safe_cfg = self.config_1d_dataset_info.safe_mask
-            if "custom-mask" in safe_cfg.methods:
-                pars = safe_cfg.parameters
-                dataset_on_off.mask_safe = dataset_on_off.counts.geom.energy_mask(
-                    energy_min=u.Quantity(pars["min"]), energy_max=u.Quantity(pars["max"])
+        for data, obs in zip(self.datasets, observations):
+            # Rename the datasets using the appropriate Obs ID
+            data._name = obs.obs_id
+
+            # Use custom safe energy mask
+            if safe_maker is None:
+                data.mask_safe = data.counts.geom.energy_mask(
+                    energy_min=u.Quantity(pars["min"]),
+                    energy_max=u.Quantity(pars["max"]),
                 )
-            elif len(safe_cfg.methods) != 0:
-                dataset_on_off = safe_maker.run(dataset_on_off, obs)
-            else:
-                self.log.info(f"No safe mask applied for {obs.obs_id}")
-
-            self.datasets.append(dataset_on_off)
```

### Comparing `asgardpy-0.3.3/asgardpy/data/dataset_3d.py` & `asgardpy-0.3.4/asgardpy/data/dataset_3d.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     BackgroundConfig,
     BaseConfig,
     GeomConfig,
     MapAxesConfig,
     MapSelectionEnum,
     ReductionTypeEnum,
     SafeMaskConfig,
-    SpatialCircleConfig,
+    SkyPositionConfig,
     get_energy_axis,
 )
 from asgardpy.data.target import (
     apply_selection_mask_to_models,
     create_gal_diffuse_skymodel,
     create_iso_diffuse_skymodel,
     create_source_skymodel,
@@ -62,15 +62,15 @@
 class Dataset3DInfoConfig(BaseConfig):
     name: str = "dataset-name"
     key: List = []
     map_selection: List[MapSelectionEnum] = MapDatasetMaker.available_selection
     geom: GeomConfig = GeomConfig()
     background: BackgroundConfig = BackgroundConfig()
     safe_mask: SafeMaskConfig = SafeMaskConfig()
-    on_region: SpatialCircleConfig = SpatialCircleConfig()
+    on_region: SkyPositionConfig = SkyPositionConfig()
     containment_correction: bool = True
     spectral_energy_range: MapAxesConfig = MapAxesConfig()
 
 
 class Dataset3DBaseConfig(BaseConfig):
     name: str = "Instrument-name"
     io: List[InputConfig] = [InputConfig()]
```

### Comparing `asgardpy-0.3.3/asgardpy/data/dl4.py` & `asgardpy-0.3.4/asgardpy/data/dl4.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,31 +21,25 @@
 
 # Defining various components of High-level Analysis Config
 class BackendEnum(str, Enum):
     minuit = "minuit"
     scipy = "scipy"
 
 
-class ParallelBackendEnum(str, Enum):
-    multi = "multiprocessing"
-    ray = "ray"
-
-
 class FitConfig(BaseConfig):
     fit_range: EnergyRangeConfig = EnergyRangeConfig()
     backend: BackendEnum = BackendEnum.minuit
     optimize_opts: dict = {}
     covariance_opts: dict = {}
     confidence_opts: dict = {}
     store_trace: bool = True
 
 
 class FluxPointsConfig(BaseConfig):
     parameters: dict = {"selection_optional": "all"}
-    parallel_backend: ParallelBackendEnum = ParallelBackendEnum.multi
     reoptimize: bool = False
 
 
 # The main Analysis Steps
 class FitAnalysisStep(AnalysisStepBase):
     """
     Using the Fitting parameters as defined in the Config, with the given
@@ -120,15 +114,15 @@
         """
         fpe_settings = self.config.flux_points_params.parameters
 
         self.fpe = FluxPointsEstimator(
             energy_edges=energy_bin_edges,
             source=self.config.target.source_name,
             n_jobs=self.config.general.n_jobs,
-            parallel_backend=self.config.flux_points_params.parallel_backend,
+            parallel_backend=self.config.general.parallel_backend,
             reoptimize=self.config.flux_points_params.reoptimize,
             **fpe_settings
         )
 
     def _sort_datasets_info(self):
         """
         The given list of datasets may contain sub-instrument level datasets.
```

### Comparing `asgardpy-0.3.3/asgardpy/data/target.py` & `asgardpy-0.3.4/asgardpy/data/target.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,26 +16,29 @@
     DatasetModels,
     EBLAbsorptionNormSpectralModel,
     Models,
     SkyModel,
     SpectralModel,
     create_fermi_isotropic_diffuse_model,
 )
+from scipy.stats import chi2, norm
 
-from asgardpy.base import AngleType, BaseConfig, PathType, SkyCoordConfig
+from asgardpy.base import AngleType, BaseConfig, PathType, SkyPositionConfig
 
 __all__ = [
     "BrokenPowerLaw2SpectralModel",
     "EBLAbsorptionModel",
     "ExpCutoffLogParabolaSpectralModel",
     "RoISelectionConfig",
     "SpatialModelConfig",
     "SpectralModelConfig",
     "Target",
     "apply_selection_mask_to_models",
+    "check_model_preference_aic",
+    "check_model_preference_lrt",
     "config_to_dict",
     "create_gal_diffuse_skymodel",
     "create_iso_diffuse_skymodel",
     "create_source_skymodel",
     "params_renaming_to_gammapy",
     "params_rescale_to_gammapy",
     "read_models_from_asgardpy_config",
@@ -85,15 +88,15 @@
 class RoISelectionConfig(BaseConfig):
     roi_radius: AngleType = 0 * u.deg
     free_sources: List[str] = []
 
 
 class Target(BaseConfig):
     source_name: str = ""
-    sky_position: SkyCoordConfig = SkyCoordConfig()
+    sky_position: SkyPositionConfig = SkyPositionConfig()
     use_uniform_position: bool = True
     models_file: PathType = PathType(".")
     extended: bool = False
     components: List[SkyModelComponent] = [SkyModelComponent()]
     covariance: str = ""
     from_3d: bool = False
     roi_selection: RoISelectionConfig = RoISelectionConfig()
@@ -906,7 +909,109 @@
         name="diffuse-iem",
     )
     source.parameters["norm"].min = 0
     source.parameters["norm"].max = 10
     source.parameters["norm"].frozen = False
 
     return source
+
+
+def check_model_preference_lrt(result1, result2, model1, model2):
+    """
+    Log-likelihood ratio test. Checking the preference of a "nested" spectral
+    model2 (observed), over a primary model1.
+
+    Parameters
+    ----------
+    result1: `gammapy.modeling.fit.FitResult`
+        Fit result of the primary spectral model.
+    result2: `gammapy.modeling.fit.FitResult`
+        Fit result of the nested spectral model.
+    model1: `gammapy.modeling.models.spectral.SpectralModel`
+        Primary spectral model
+    model2: `gammapy.modeling.models.spectral.SpectralModel`
+        Nested spectral model
+
+    Returns
+    -------
+    p_value: float
+        p-value for the ratio of the likelihoods
+    gaussian_sigmas: float
+        significance (Chi2) of the ratio of the likelihoods estimated in
+        Gaussian distribution.
+    chi2_1: float
+        significance (Chi2) of the likelihood of primary fit model estimated in
+        Gaussian distribution.
+    chi2_2: float
+        significance (Chi2) of the likelihood of nested fit model estimated in
+        Gaussian distribution.
+    n_dof: int
+        number of degrees of freedom or free parameters between primary and
+        nested model.
+    """
+    Wstat_1 = result1.total_stat
+    Wstat_2 = result2.total_stat
+
+    pval_1 = chi2.sf(Wstat_1, len(list(model1.parameters.free_parameters)))
+    pval_2 = chi2.sf(Wstat_2, len(list(model2.parameters.free_parameters)))
+
+    chi2_1 = norm.isf(pval_1 / 2)
+    chi2_2 = norm.isf(pval_2 / 2)
+
+    n_dof = len(list(model2.parameters.free_parameters)) - len(
+        list(model1.parameters.free_parameters)
+    )
+    if n_dof < 1:
+        print(
+            f"DoF is lower in {model2.spectral_model.model1.tag[0]} compared "
+            f"to {model1.spectral_model.model1.tag[0]}"
+        )
+        return np.nan, np.nan, chi2_1, chi2_2, n_dof
+
+    p_value = chi2.sf((Wstat_1 - Wstat_2), n_dof)
+    gaussian_sigmas = norm.isf(p_value / 2)
+
+    if not np.isfinite(gaussian_sigmas):
+        gaussian_sigmas = np.sqrt((Wstat_1 - Wstat_2))
+
+    return p_value, gaussian_sigmas, chi2_1, chi2_2, n_dof
+
+
+def check_model_preference_aic(list_wstat, list_dof):
+    """
+    Akaike Information Criterion (AIC) preference over a list of wstat and DoF
+    (degree of freedom) to get relative likelihood of a given list of best-fit
+    models.
+
+    Parameters
+    ----------
+    list_wstat: list
+        List of wstat or -2 Log likelihood values for a list of models.
+    list_dof: list
+        List of degrees of freedom or list of free parameters, for a list of models.
+
+    Returns
+    -------
+    list_p: list
+        List of relative likelihood probabilities, for a list of models.
+    """
+    list_aic = []
+    for w, d in zip(list_wstat, list_dof):
+        aic = 2 * w + 2 * d
+        list_aic.append(aic)
+    list_aic = np.array(list_aic)
+
+    aic_min = np.min(list_aic)
+
+    list_b = []
+    for a in list_aic:
+        b = np.exp((aic_min - a) / 2)
+        list_b.append(b)
+    list_b = np.array(list_b)
+
+    list_p = []
+    for bb in list_b:
+        bbb = bb / np.sum(list_b)
+        list_p.append(bbb)
+    list_p = np.array(list_p)
+
+    return list_p
```

### Comparing `asgardpy-0.3.3/asgardpy/io/io.py` & `asgardpy-0.3.4/asgardpy/io/io.py`

 * *Files identical despite different names*

### Comparing `asgardpy-0.3.3/asgardpy.egg-info/PKG-INFO` & `asgardpy-0.3.4/asgardpy.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asgardpy
-Version: 0.3.3
+Version: 0.3.4
 Summary: Gammapy-based pipeline for easy joint analysis of different gamma-ray datasets
 Home-page: https://github.com/chaimain/asgardpy
 Download-URL: https://github.com/chaimain/asgardpy/archive/refs/tags/v0.3.1.tar.gz
 Author: Chaitanya Priyadarshi
 Author-email: chaitanya.p.astrphys@gmail.com
 License: Apache
 Classifier: Intended Audience :: Science/Research
@@ -17,24 +17,24 @@
 Provides-Extra: dev
 License-File: LICENSE
 
 # asgardpy [![Build Status](https://github.com/chaimain/asgardpy/actions/workflows/main.yml/badge.svg?branch=main)](https://github.com/chaimain/asgardpy/actions?query=branch%3Amain) [![gammapy](https://img.shields.io/badge/powered%20by-gammapy-orange.svg?style=flat)](https://www.gammapy.org/) [![astropy](http://img.shields.io/badge/powered%20by-AstroPy-orange.svg?style=flat)](https://www.astropy.org/)
 ## Analysis Software for GAmma-Ray Data in Python
 
 'User-friendly' configuration-centred pipeline built over [Gammapy](https://github.com/gammapy/gammapy) to allow for easy simultaneous analysis of various datasets of different formats.
-Example: 3D Fermi-LAT (with various source models in the Region of Interest stored in XML file) + 1D energy-dependent selection cut MAGIC/LST [PointSkyRegion geometry for ON region] + 1D fixed-cut VERITAS [CircleSkyRegion geometry for ON region].
+Example: 3D Fermi-LAT (with various source models in the Region of Interest stored in XML file) + 1D energy-dependent directional cuts MAGIC/LST [PointSkyRegion geometry for ON region] + 1D global directional cut VERITAS [CircleSkyRegion geometry for ON region].
 
 Follow the documentation at https://asgardpy.readthedocs.io/en/latest/ for the main functionality of this pipeline.
 Follow the [Gammapy v1.1](https://docs.gammapy.org/1.1/) documentation for understanding the core Gammapy objects.
 
 The various Data Levels	used here follow the descriptions suggested by [GADF v0.3](https://gamma-astro-data-formats.readthedocs.io/en/latest/) and CTAO Data Model
 
 # Pipeline development
 
-The pipeline was developed with first testing with Fermi-LAT ([enrico](https://enrico.readthedocs.io/en/latest/) and [fermipy](https://fermipy.readthedocs.io/en/latest/)) files and LST-1 ([cta-lstchain](https://cta-observatory.github.io/cta-lstchain/)) DL3 files (with energy-dependent selection cuts) for point-like sources.
+The pipeline was developed with first testing with Fermi-LAT ([enrico](https://enrico.readthedocs.io/en/latest/) and [fermipy](https://fermipy.readthedocs.io/en/latest/)) files and LST-1 ([cta-lstchain](https://cta-observatory.github.io/cta-lstchain/)) DL3 files (with energy-dependent and global directional cuts) for point-like sources.
 The pipeline can be further expanded to support more types of DL3 files of gamma-ray instruments.
 
 An example of configuration file that can be used with asgardpy can be found at ``asgardpy/config/template.yaml``
 Examples of usage of asgardpy is shown in jupyter notebooks in ``notebooks/`` but as there are no public test data included with the pipeline yet, the results are empty.
 
 # Pipeline Template
```

### Comparing `asgardpy-0.3.3/asgardpy.egg-info/SOURCES.txt` & `asgardpy-0.3.4/asgardpy.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -16,13 +16,14 @@
 asgardpy/base/__init__.py
 asgardpy/base/base.py
 asgardpy/base/geom.py
 asgardpy/base/reduction.py
 asgardpy/config/__init__.py
 asgardpy/config/generator.py
 asgardpy/data/__init__.py
+asgardpy/data/base.py
 asgardpy/data/dataset_1d.py
 asgardpy/data/dataset_3d.py
 asgardpy/data/dl4.py
 asgardpy/data/target.py
 asgardpy/io/__init__.py
 asgardpy/io/io.py
```

### Comparing `asgardpy-0.3.3/setup.py` & `asgardpy-0.3.4/setup.py`

 * *Files identical despite different names*

