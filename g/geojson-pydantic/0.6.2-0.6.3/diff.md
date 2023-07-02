# Comparing `tmp/geojson_pydantic-0.6.2.tar.gz` & `tmp/geojson_pydantic-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geojson_pydantic-0.6.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "geojson_pydantic-0.6.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `geojson_pydantic-0.6.2.tar` & `geojson_pydantic-0.6.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      220 2023-05-16 21:47:04.019785 geojson_pydantic-0.6.2/.bumpversion.cfg
--rw-r--r--   0        0        0     1173 2023-05-16 21:47:04.023785 geojson_pydantic-0.6.2/.gitignore
--rw-r--r--   0        0        0      792 2023-05-16 21:47:04.023785 geojson_pydantic-0.6.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1073 2023-05-16 21:47:04.023785 geojson_pydantic-0.6.2/LICENSE
--rw-r--r--   0        0        0     6592 2023-05-16 21:47:04.023785 geojson_pydantic-0.6.2/README.md
--rw-r--r--   0        0        0      448 2023-05-16 21:47:04.023785 geojson_pydantic-0.6.2/geojson_pydantic/__init__.py
--rw-r--r--   0        0        0     1906 2023-05-16 21:47:04.023785 geojson_pydantic-0.6.2/geojson_pydantic/features.py
--rw-r--r--   0        0        0      705 2023-05-16 21:47:04.023785 geojson_pydantic-0.6.2/geojson_pydantic/geo_interface.py
--rw-r--r--   0        0        0    10976 2023-05-16 21:47:04.023785 geojson_pydantic-0.6.2/geojson_pydantic/geometries.py
--rw-r--r--   0        0        0        0 2023-05-16 21:47:04.023785 geojson_pydantic-0.6.2/geojson_pydantic/py.typed
--rw-r--r--   0        0        0     1696 2023-05-16 21:47:04.023785 geojson_pydantic-0.6.2/geojson_pydantic/types.py
--rw-r--r--   0        0        0     2293 2023-05-16 21:47:04.023785 geojson_pydantic-0.6.2/pyproject.toml
--rw-r--r--   0        0        0     7596 1970-01-01 00:00:00.000000 geojson_pydantic-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0      220 2023-07-02 18:47:34.743742 geojson_pydantic-0.6.3/.bumpversion.cfg
+-rw-r--r--   0        0        0     1173 2023-07-02 18:47:34.743742 geojson_pydantic-0.6.3/.gitignore
+-rw-r--r--   0        0        0      797 2023-07-02 18:47:34.743742 geojson_pydantic-0.6.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1073 2023-07-02 18:47:34.743742 geojson_pydantic-0.6.3/LICENSE
+-rw-r--r--   0        0        0     7913 2023-07-02 18:47:34.743742 geojson_pydantic-0.6.3/README.md
+-rw-r--r--   0        0        0      448 2023-07-02 18:47:34.743742 geojson_pydantic-0.6.3/geojson_pydantic/__init__.py
+-rw-r--r--   0        0        0     1906 2023-07-02 18:47:34.743742 geojson_pydantic-0.6.3/geojson_pydantic/features.py
+-rw-r--r--   0        0        0      705 2023-07-02 18:47:34.743742 geojson_pydantic-0.6.3/geojson_pydantic/geo_interface.py
+-rw-r--r--   0        0        0    10976 2023-07-02 18:47:34.743742 geojson_pydantic-0.6.3/geojson_pydantic/geometries.py
+-rw-r--r--   0        0        0        0 2023-07-02 18:47:34.743742 geojson_pydantic-0.6.3/geojson_pydantic/py.typed
+-rw-r--r--   0        0        0     1696 2023-07-02 18:47:34.743742 geojson_pydantic-0.6.3/geojson_pydantic/types.py
+-rw-r--r--   0        0        0     2271 2023-07-02 18:47:34.743742 geojson_pydantic-0.6.3/pyproject.toml
+-rw-r--r--   0        0        0     8922 1970-01-01 00:00:00.000000 geojson_pydantic-0.6.3/PKG-INFO
```

### Comparing `geojson_pydantic-0.6.2/.gitignore` & `geojson_pydantic-0.6.3/.gitignore`

 * *Files identical despite different names*

### Comparing `geojson_pydantic-0.6.2/.pre-commit-config.yaml` & `geojson_pydantic-0.6.3/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -26,8 +26,8 @@
     rev: v0.991
     hooks:
       - id: mypy
         language_version: python
         # No reason to run if only tests have changed. They intentionally break typing.
         exclude: tests/.*
         additional_dependencies:
-        - pydantic
+        - pydantic~=1.0
```

### Comparing `geojson_pydantic-0.6.2/LICENSE` & `geojson_pydantic-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `geojson_pydantic-0.6.2/README.md` & `geojson_pydantic-0.6.3/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -22,15 +22,15 @@
   <a href="https://anaconda.org/conda-forge/geojson-pydantic" target="_blank">
       <img src="https://anaconda.org/conda-forge/geojson-pydantic/badges/version.svg" alt="Conda">
   </a>
 </p>
 
 ## Description
 
-`geojson_pydantic` provides a suite of Pydantic models matching the GeoJSON specification [rfc7946](https://datatracker.ietf.org/doc/html/rfc7946#section-3.1.1). Those models can be used for creating or validating geojson data.
+`geojson_pydantic` provides a suite of Pydantic models matching the GeoJSON specification [rfc7946](https://datatracker.ietf.org/doc/html/rfc7946). Those models can be used for creating or validating geojson data.
 
 ## Install
 
 ```bash
 $ python -m pip install -U pip
 $ python -m pip install geojson-pydantic
 ```
@@ -66,15 +66,15 @@
 
 
 feat = Feature(**geojson_feature)
 assert feat.type == "Feature"
 assert type(feat.geometry) == Point
 assert feat.properties["name"] == "jeff"
 
-fc = FeatureCollection(features=[geojson_feature, geojson_feature])
+fc = FeatureCollection(type="FeatureCollection", features=[geojson_feature, geojson_feature])
 assert fc.type == "FeatureCollection"
 assert len(fc) == 2
 assert type(fc.features[0].geometry) == Point
 assert fc.features[0].properties["name"] == "jeff"
 ```
 
 ### Advanced usage
@@ -178,14 +178,52 @@
   string does not match regex "^(drew|vincent)$" (type=value_error.str.regex; pattern=^(drew|vincent)$)
 
 geojson_feature["properties"]["name"] = "drew"
 feat = MyPointFeatureModel(**geojson_feature)
 assert feat.properties.name == "drew"
 ```
 
+## Enforced Keys
+
+Starting with version `0.6.0`, geojson-pydantic's classes will not define default keys such has `type`, `geometry` or `properties`.
+This is to make sure the library does well its first goal, which is `validating` GeoJSON object based on the [specification](https://datatracker.ietf.org/doc/html/rfc7946#section-3.1.1)
+
+    o A GeoJSON object has a member with the name "type".  The value of
+      the member MUST be one of the GeoJSON types.
+
+    o A Feature object HAS a "type" member with the value "Feature".
+
+    o A Feature object HAS a member with the name "geometry". The value
+    of the geometry member SHALL be either a Geometry object as
+    defined above or, in the case that the Feature is unlocated, a
+    JSON null value.
+
+    o A Feature object HAS a member with the name "properties". The
+    value of the properties member is an object (any JSON object or a
+    JSON null value).
+
+
+```python
+from geojson_pydantic import Point
+
+## Before 0.6
+Point(coordinates=(0,0))
+>> Point(type='Point', coordinates=(0.0, 0.0), bbox=None)
+
+## After 0.6
+Point(coordinates=(0,0))
+>> ValidationError: 1 validation error for Point
+   type
+      field required (type=value_error.missing)
+
+Point(type="Point", coordinates=(0,0))
+>> Point(type='Point', coordinates=(0.0, 0.0), bbox=None)
+```
+
+
 ## Contributing
 
 See [CONTRIBUTING.md](CONTRIBUTING.md).
 
 ## Changes
 
 See [CHANGES.md](https://github.com/developmentseed/geojson-pydantic/blob/main/CHANGELOG.md).
```

### Comparing `geojson_pydantic-0.6.2/geojson_pydantic/features.py` & `geojson_pydantic-0.6.3/geojson_pydantic/features.py`

 * *Files identical despite different names*

### Comparing `geojson_pydantic-0.6.2/geojson_pydantic/geo_interface.py` & `geojson_pydantic-0.6.3/geojson_pydantic/geo_interface.py`

 * *Files identical despite different names*

### Comparing `geojson_pydantic-0.6.2/geojson_pydantic/geometries.py` & `geojson_pydantic-0.6.3/geojson_pydantic/geometries.py`

 * *Files identical despite different names*

### Comparing `geojson_pydantic-0.6.2/geojson_pydantic/types.py` & `geojson_pydantic-0.6.3/geojson_pydantic/types.py`

 * *Files identical despite different names*

### Comparing `geojson_pydantic-0.6.2/pyproject.toml` & `geojson_pydantic-0.6.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Scientific/Engineering :: GIS",
     "Typing :: Typed",
 ]
 dynamic = ["version"]
-dependencies = ["pydantic"]
+dependencies = ["pydantic~=1.0"]
 
 [project.optional-dependencies]
 test = ["pytest", "pytest-cov", "shapely"]
 dev = ["pre-commit"]
 
 [project.urls]
 Source = "https://github.com/developmentseed/geojson-pydantic"
@@ -63,15 +63,14 @@
 default_section = "THIRDPARTY"
 
 [tool.mypy]
 plugins = ["pydantic.mypy"]
 disallow_untyped_calls = true
 disallow_untyped_defs = true
 disallow_incomplete_defs = true
-warn_untyped_fields = true
 warn_redundant_casts = true
 warn_unused_ignores = true
 no_implicit_optional = true
 show_error_codes = true
 
 [tool.ruff]
 select = [
```

### Comparing `geojson_pydantic-0.6.2/PKG-INFO` & `geojson_pydantic-0.6.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: geojson-pydantic
-Version: 0.6.2
+Version: 0.6.3
 Summary: Pydantic data models for the GeoJSON spec.
 Keywords: geojson,Pydantic
 Author-email: Drew Bollinger <drew@developmentseed.org>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: GIS
 Classifier: Typing :: Typed
-Requires-Dist: pydantic
+Requires-Dist: pydantic~=1.0
 Requires-Dist: pre-commit ; extra == "dev"
 Requires-Dist: pytest ; extra == "test"
 Requires-Dist: pytest-cov ; extra == "test"
 Requires-Dist: shapely ; extra == "test"
 Project-URL: Source, https://github.com/developmentseed/geojson-pydantic
 Provides-Extra: dev
 Provides-Extra: test
@@ -48,15 +48,15 @@
   <a href="https://anaconda.org/conda-forge/geojson-pydantic" target="_blank">
       <img src="https://anaconda.org/conda-forge/geojson-pydantic/badges/version.svg" alt="Conda">
   </a>
 </p>
 
 ## Description
 
-`geojson_pydantic` provides a suite of Pydantic models matching the GeoJSON specification [rfc7946](https://datatracker.ietf.org/doc/html/rfc7946#section-3.1.1). Those models can be used for creating or validating geojson data.
+`geojson_pydantic` provides a suite of Pydantic models matching the GeoJSON specification [rfc7946](https://datatracker.ietf.org/doc/html/rfc7946). Those models can be used for creating or validating geojson data.
 
 ## Install
 
 ```bash
 $ python -m pip install -U pip
 $ python -m pip install geojson-pydantic
 ```
@@ -92,15 +92,15 @@
 
 
 feat = Feature(**geojson_feature)
 assert feat.type == "Feature"
 assert type(feat.geometry) == Point
 assert feat.properties["name"] == "jeff"
 
-fc = FeatureCollection(features=[geojson_feature, geojson_feature])
+fc = FeatureCollection(type="FeatureCollection", features=[geojson_feature, geojson_feature])
 assert fc.type == "FeatureCollection"
 assert len(fc) == 2
 assert type(fc.features[0].geometry) == Point
 assert fc.features[0].properties["name"] == "jeff"
 ```
 
 ### Advanced usage
@@ -204,14 +204,52 @@
   string does not match regex "^(drew|vincent)$" (type=value_error.str.regex; pattern=^(drew|vincent)$)
 
 geojson_feature["properties"]["name"] = "drew"
 feat = MyPointFeatureModel(**geojson_feature)
 assert feat.properties.name == "drew"
 ```
 
+## Enforced Keys
+
+Starting with version `0.6.0`, geojson-pydantic's classes will not define default keys such has `type`, `geometry` or `properties`.
+This is to make sure the library does well its first goal, which is `validating` GeoJSON object based on the [specification](https://datatracker.ietf.org/doc/html/rfc7946#section-3.1.1)
+
+    o A GeoJSON object has a member with the name "type".  The value of
+      the member MUST be one of the GeoJSON types.
+
+    o A Feature object HAS a "type" member with the value "Feature".
+
+    o A Feature object HAS a member with the name "geometry". The value
+    of the geometry member SHALL be either a Geometry object as
+    defined above or, in the case that the Feature is unlocated, a
+    JSON null value.
+
+    o A Feature object HAS a member with the name "properties". The
+    value of the properties member is an object (any JSON object or a
+    JSON null value).
+
+
+```python
+from geojson_pydantic import Point
+
+## Before 0.6
+Point(coordinates=(0,0))
+>> Point(type='Point', coordinates=(0.0, 0.0), bbox=None)
+
+## After 0.6
+Point(coordinates=(0,0))
+>> ValidationError: 1 validation error for Point
+   type
+      field required (type=value_error.missing)
+
+Point(type="Point", coordinates=(0,0))
+>> Point(type='Point', coordinates=(0.0, 0.0), bbox=None)
+```
+
+
 ## Contributing
 
 See [CONTRIBUTING.md](CONTRIBUTING.md).
 
 ## Changes
 
 See [CHANGES.md](https://github.com/developmentseed/geojson-pydantic/blob/main/CHANGELOG.md).
```

