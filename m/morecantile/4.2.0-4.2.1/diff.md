# Comparing `tmp/morecantile-4.2.0.tar.gz` & `tmp/morecantile-4.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "morecantile-4.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "morecantile-4.2.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `morecantile-4.2.0.tar` & `morecantile-4.2.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0      215 2023-06-09 09:16:46.762144 morecantile-4.2.0/.bumpversion.cfg
--rw-r--r--   0        0        0     1817 2023-06-09 09:16:46.762144 morecantile-4.2.0/.gitignore
--rw-r--r--   0        0        0      822 2023-06-09 09:16:46.762144 morecantile-4.2.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1073 2023-06-09 09:16:46.762144 morecantile-4.2.0/LICENSE
--rw-r--r--   0        0        0     5305 2023-06-09 09:16:46.762144 morecantile-4.2.0/README.md
--rw-r--r--   0        0        0      436 2023-06-09 09:16:46.766144 morecantile-4.2.0/morecantile/__init__.py
--rw-r--r--   0        0        0     1015 2023-06-09 09:16:46.766144 morecantile-4.2.0/morecantile/commons.py
--rw-r--r--   0        0        0     7267 2023-06-09 09:16:46.766144 morecantile-4.2.0/morecantile/data/CanadianNAD83_LCC.json
--rw-r--r--   0        0        0     4679 2023-06-09 09:16:46.766144 morecantile-4.2.0/morecantile/data/EuropeanETRS89_LAEAQuad.json
--rw-r--r--   0        0        0     5176 2023-06-09 09:16:46.766144 morecantile-4.2.0/morecantile/data/LINZAntarticaMapTilegrid.json
--rw-r--r--   0        0        0     8457 2023-06-09 09:16:46.766144 morecantile-4.2.0/morecantile/data/NZTM2000Quad.json
--rw-r--r--   0        0        0      242 2023-06-09 09:16:46.766144 morecantile-4.2.0/morecantile/data/README.md
--rw-r--r--   0        0        0     7374 2023-06-09 09:16:46.766144 morecantile-4.2.0/morecantile/data/UPSAntarcticWGS84Quad.json
--rw-r--r--   0        0        0     7365 2023-06-09 09:16:46.766144 morecantile-4.2.0/morecantile/data/UPSArcticWGS84Quad.json
--rw-r--r--   0        0        0     7367 2023-06-09 09:16:46.766144 morecantile-4.2.0/morecantile/data/UTM31WGS84Quad.json
--rw-r--r--   0        0        0     6932 2023-06-09 09:16:46.766144 morecantile-4.2.0/morecantile/data/WGS1984Quad.json
--rw-r--r--   0        0        0     7843 2023-06-09 09:16:46.766144 morecantile-4.2.0/morecantile/data/WebMercatorQuad.json
--rw-r--r--   0        0        0     7072 2023-06-09 09:16:46.766144 morecantile-4.2.0/morecantile/data/WorldCRS84Quad.json
--rw-r--r--   0        0        0     7001 2023-06-09 09:16:46.766144 morecantile-4.2.0/morecantile/data/WorldMercatorWGS84Quad.json
--rw-r--r--   0        0        0     1748 2023-06-09 09:16:46.766144 morecantile-4.2.0/morecantile/defaults.py
--rw-r--r--   0        0        0      907 2023-06-09 09:16:46.766144 morecantile-4.2.0/morecantile/errors.py
--rw-r--r--   0        0        0    41795 2023-06-09 09:16:46.766144 morecantile-4.2.0/morecantile/models.py
--rw-r--r--   0        0        0        0 2023-06-09 09:16:46.766144 morecantile-4.2.0/morecantile/py.typed
--rw-r--r--   0        0        0       23 2023-06-09 09:16:46.766144 morecantile-4.2.0/morecantile/scripts/__init__.py
--rw-r--r--   0        0        0    16657 2023-06-09 09:16:46.766144 morecantile-4.2.0/morecantile/scripts/cli.py
--rw-r--r--   0        0        0     3364 2023-06-09 09:16:46.766144 morecantile-4.2.0/morecantile/utils.py
--rw-r--r--   0        0        0     2295 2023-06-09 09:16:46.766144 morecantile-4.2.0/pyproject.toml
--rw-r--r--   0        0        0     6732 1970-01-01 00:00:00.000000 morecantile-4.2.0/PKG-INFO
+-rw-r--r--   0        0        0      215 2023-07-02 18:22:29.718076 morecantile-4.2.1/.bumpversion.cfg
+-rw-r--r--   0        0        0     1817 2023-07-02 18:22:29.718076 morecantile-4.2.1/.gitignore
+-rw-r--r--   0        0        0      822 2023-07-02 18:22:29.718076 morecantile-4.2.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1073 2023-07-02 18:22:29.718076 morecantile-4.2.1/LICENSE
+-rw-r--r--   0        0        0     5305 2023-07-02 18:22:29.718076 morecantile-4.2.1/README.md
+-rw-r--r--   0        0        0      436 2023-07-02 18:22:29.718076 morecantile-4.2.1/morecantile/__init__.py
+-rw-r--r--   0        0        0     1015 2023-07-02 18:22:29.718076 morecantile-4.2.1/morecantile/commons.py
+-rw-r--r--   0        0        0     7267 2023-07-02 18:22:29.718076 morecantile-4.2.1/morecantile/data/CanadianNAD83_LCC.json
+-rw-r--r--   0        0        0     4679 2023-07-02 18:22:29.718076 morecantile-4.2.1/morecantile/data/EuropeanETRS89_LAEAQuad.json
+-rw-r--r--   0        0        0     5176 2023-07-02 18:22:29.718076 morecantile-4.2.1/morecantile/data/LINZAntarticaMapTilegrid.json
+-rw-r--r--   0        0        0     8457 2023-07-02 18:22:29.718076 morecantile-4.2.1/morecantile/data/NZTM2000Quad.json
+-rw-r--r--   0        0        0      242 2023-07-02 18:22:29.718076 morecantile-4.2.1/morecantile/data/README.md
+-rw-r--r--   0        0        0     7374 2023-07-02 18:22:29.718076 morecantile-4.2.1/morecantile/data/UPSAntarcticWGS84Quad.json
+-rw-r--r--   0        0        0     7365 2023-07-02 18:22:29.718076 morecantile-4.2.1/morecantile/data/UPSArcticWGS84Quad.json
+-rw-r--r--   0        0        0     7367 2023-07-02 18:22:29.718076 morecantile-4.2.1/morecantile/data/UTM31WGS84Quad.json
+-rw-r--r--   0        0        0     6932 2023-07-02 18:22:29.718076 morecantile-4.2.1/morecantile/data/WGS1984Quad.json
+-rw-r--r--   0        0        0     7843 2023-07-02 18:22:29.718076 morecantile-4.2.1/morecantile/data/WebMercatorQuad.json
+-rw-r--r--   0        0        0     7072 2023-07-02 18:22:29.718076 morecantile-4.2.1/morecantile/data/WorldCRS84Quad.json
+-rw-r--r--   0        0        0     7001 2023-07-02 18:22:29.718076 morecantile-4.2.1/morecantile/data/WorldMercatorWGS84Quad.json
+-rw-r--r--   0        0        0     1748 2023-07-02 18:22:29.718076 morecantile-4.2.1/morecantile/defaults.py
+-rw-r--r--   0        0        0      907 2023-07-02 18:22:29.718076 morecantile-4.2.1/morecantile/errors.py
+-rw-r--r--   0        0        0    41795 2023-07-02 18:22:29.718076 morecantile-4.2.1/morecantile/models.py
+-rw-r--r--   0        0        0        0 2023-07-02 18:22:29.718076 morecantile-4.2.1/morecantile/py.typed
+-rw-r--r--   0        0        0       23 2023-07-02 18:22:29.718076 morecantile-4.2.1/morecantile/scripts/__init__.py
+-rw-r--r--   0        0        0    16657 2023-07-02 18:22:29.718076 morecantile-4.2.1/morecantile/scripts/cli.py
+-rw-r--r--   0        0        0     3364 2023-07-02 18:22:29.718076 morecantile-4.2.1/morecantile/utils.py
+-rw-r--r--   0        0        0     2300 2023-07-02 18:22:29.718076 morecantile-4.2.1/pyproject.toml
+-rw-r--r--   0        0        0     6737 1970-01-01 00:00:00.000000 morecantile-4.2.1/PKG-INFO
```

### Comparing `morecantile-4.2.0/.gitignore` & `morecantile-4.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `morecantile-4.2.0/.pre-commit-config.yaml` & `morecantile-4.2.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `morecantile-4.2.0/LICENSE` & `morecantile-4.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `morecantile-4.2.0/README.md` & `morecantile-4.2.1/README.md`

 * *Files identical despite different names*

### Comparing `morecantile-4.2.0/morecantile/commons.py` & `morecantile-4.2.1/morecantile/commons.py`

 * *Files identical despite different names*

### Comparing `morecantile-4.2.0/morecantile/data/CanadianNAD83_LCC.json` & `morecantile-4.2.1/morecantile/data/CanadianNAD83_LCC.json`

 * *Files identical despite different names*

### Comparing `morecantile-4.2.0/morecantile/data/EuropeanETRS89_LAEAQuad.json` & `morecantile-4.2.1/morecantile/data/EuropeanETRS89_LAEAQuad.json`

 * *Files identical despite different names*

### Comparing `morecantile-4.2.0/morecantile/data/LINZAntarticaMapTilegrid.json` & `morecantile-4.2.1/morecantile/data/LINZAntarticaMapTilegrid.json`

 * *Files identical despite different names*

### Comparing `morecantile-4.2.0/morecantile/data/NZTM2000Quad.json` & `morecantile-4.2.1/morecantile/data/NZTM2000Quad.json`

 * *Files identical despite different names*

### Comparing `morecantile-4.2.0/morecantile/data/UPSAntarcticWGS84Quad.json` & `morecantile-4.2.1/morecantile/data/UPSAntarcticWGS84Quad.json`

 * *Files identical despite different names*

### Comparing `morecantile-4.2.0/morecantile/data/UPSArcticWGS84Quad.json` & `morecantile-4.2.1/morecantile/data/UPSArcticWGS84Quad.json`

 * *Files identical despite different names*

### Comparing `morecantile-4.2.0/morecantile/data/UTM31WGS84Quad.json` & `morecantile-4.2.1/morecantile/data/UTM31WGS84Quad.json`

 * *Files identical despite different names*

### Comparing `morecantile-4.2.0/morecantile/data/WGS1984Quad.json` & `morecantile-4.2.1/morecantile/data/WGS1984Quad.json`

 * *Files identical despite different names*

### Comparing `morecantile-4.2.0/morecantile/data/WebMercatorQuad.json` & `morecantile-4.2.1/morecantile/data/WebMercatorQuad.json`

 * *Files identical despite different names*

### Comparing `morecantile-4.2.0/morecantile/data/WorldCRS84Quad.json` & `morecantile-4.2.1/morecantile/data/WorldCRS84Quad.json`

 * *Files identical despite different names*

### Comparing `morecantile-4.2.0/morecantile/data/WorldMercatorWGS84Quad.json` & `morecantile-4.2.1/morecantile/data/WorldMercatorWGS84Quad.json`

 * *Files identical despite different names*

### Comparing `morecantile-4.2.0/morecantile/defaults.py` & `morecantile-4.2.1/morecantile/defaults.py`

 * *Files identical despite different names*

### Comparing `morecantile-4.2.0/morecantile/errors.py` & `morecantile-4.2.1/morecantile/errors.py`

 * *Files identical despite different names*

### Comparing `morecantile-4.2.0/morecantile/models.py` & `morecantile-4.2.1/morecantile/models.py`

 * *Files identical despite different names*

### Comparing `morecantile-4.2.0/morecantile/scripts/cli.py` & `morecantile-4.2.1/morecantile/scripts/cli.py`

 * *Files identical despite different names*

### Comparing `morecantile-4.2.0/morecantile/utils.py` & `morecantile-4.2.1/morecantile/utils.py`

 * *Files identical despite different names*

### Comparing `morecantile-4.2.0/pyproject.toml` & `morecantile-4.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     "Programming Language :: Python :: 3.11",
     "Topic :: Scientific/Engineering :: GIS",
 ]
 dynamic = ["version"]
 dependencies = [
     "attrs",
     "pyproj~=3.1",
-    "pydantic",
+    "pydantic~=1.0",
     "cachetools",
 ]
 
 [project.optional-dependencies]
 rasterio = [
     "rasterio>=1.2.1",
 ]
```

### Comparing `morecantile-4.2.0/PKG-INFO` & `morecantile-4.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: morecantile
-Version: 4.2.0
+Version: 4.2.1
 Summary: Construct and use map tile grids (a.k.a TileMatrixSet / TMS).
 Keywords: GIS,TMS,TileMatrixSet,Map Tile
 Author-email: Vincent Sarago <vincent@developmentseed.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: GIS
 Requires-Dist: attrs
 Requires-Dist: pyproj~=3.1
-Requires-Dist: pydantic
+Requires-Dist: pydantic~=1.0
 Requires-Dist: cachetools
 Requires-Dist: pre-commit ; extra == "dev"
 Requires-Dist: mkdocs ; extra == "docs"
 Requires-Dist: mkdocs-material ; extra == "docs"
 Requires-Dist: pygments ; extra == "docs"
 Requires-Dist: rasterio>=1.2.1 ; extra == "rasterio"
 Requires-Dist: mercantile ; extra == "test"
```

#### html2text {}

```diff
@@ -1,27 +1,27 @@
-Metadata-Version: 2.1 Name: morecantile Version: 4.2.0 Summary: Construct and
+Metadata-Version: 2.1 Name: morecantile Version: 4.2.1 Summary: Construct and
 use map tile grids (a.k.a TileMatrixSet / TMS). Keywords:
 GIS,TMS,TileMatrixSet,Map Tile Author-email: Vincent Sarago
 developmentseed.com> Requires-Python: >=3.8 Description-Content-Type: text/
 markdown Classifier: Intended Audience :: Information Technology Classifier:
 Intended Audience :: Science/Research Classifier: License :: OSI Approved ::
 BSD License Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Topic :: Scientific/Engineering :: GIS Requires-Dist: attrs Requires-Dist:
-pyproj~=3.1 Requires-Dist: pydantic Requires-Dist: cachetools Requires-Dist:
-pre-commit ; extra == "dev" Requires-Dist: mkdocs ; extra == "docs" Requires-
-Dist: mkdocs-material ; extra == "docs" Requires-Dist: pygments ; extra ==
-"docs" Requires-Dist: rasterio>=1.2.1 ; extra == "rasterio" Requires-Dist:
-mercantile ; extra == "test" Requires-Dist: pytest ; extra == "test" Requires-
-Dist: pytest-cov ; extra == "test" Requires-Dist: rasterio>=1.2.1 ; extra ==
-"test" Project-URL: Documentation, https://developmentseed.org/morecantile/
-Project-URL: Source, https://github.com/developmentseed/morecantile Provides-
-Extra: dev Provides-Extra: docs Provides-Extra: rasterio Provides-Extra: test #
-Morecantile
+pyproj~=3.1 Requires-Dist: pydantic~=1.0 Requires-Dist: cachetools Requires-
+Dist: pre-commit ; extra == "dev" Requires-Dist: mkdocs ; extra == "docs"
+Requires-Dist: mkdocs-material ; extra == "docs" Requires-Dist: pygments ;
+extra == "docs" Requires-Dist: rasterio>=1.2.1 ; extra == "rasterio" Requires-
+Dist: mercantile ; extra == "test" Requires-Dist: pytest ; extra == "test"
+Requires-Dist: pytest-cov ; extra == "test" Requires-Dist: rasterio>=1.2.1 ;
+extra == "test" Project-URL: Documentation, https://developmentseed.org/
+morecantile/ Project-URL: Source, https://github.com/developmentseed/
+morecantile Provides-Extra: dev Provides-Extra: docs Provides-Extra: rasterio
+Provides-Extra: test # Morecantile
 [https://github.com/developmentseed/morecantile/assets/10407788/a1523c6d-e255-
                             4dc6-a201-20029715858a]
          Construct and use map tile grids (a.k.a TileMatrixSet / TMS).
            [Test] [Coverage] [Package_version] [Downloads] [License]
 --- **Documentation**: https://developmentseed.org/morecantile/ **Source
 Code**: https://github.com/developmentseed/morecantile --- Morecantile is like
 [mercantile](https://github.com/mapbox/mercantile) (the best tool to work with
```

