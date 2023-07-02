# Comparing `tmp/pycatsearch-5.1.8.tar.gz` & `tmp/pycatsearch-5.1.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycatsearch-5.1.8.tar", last modified: Thu Jun 29 18:59:49 2023, max compression
+gzip compressed data, was "pycatsearch-5.1.9.2.tar", last modified: Sun Jul  2 07:44:37 2023, max compression
```

## Comparing `pycatsearch-5.1.8.tar` & `pycatsearch-5.1.9.2.tar`

### file list

```diff
@@ -1,47 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:59:49.205547 pycatsearch-5.1.8/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:59:49.197547 pycatsearch-5.1.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:59:49.197547 pycatsearch-5.1.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-06-29 18:59:33.000000 pycatsearch-5.1.8/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-29 18:59:33.000000 pycatsearch-5.1.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     7642 2023-06-29 18:59:33.000000 pycatsearch-5.1.8/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)    10690 2023-06-29 18:59:49.205547 pycatsearch-5.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9150 2023-06-29 18:59:33.000000 pycatsearch-5.1.8/README.md
--rwxr-xr-x   0 runner    (1001) docker     (123)     1230 2023-06-29 18:59:33.000000 pycatsearch-5.1.8/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-06-29 18:59:33.000000 pycatsearch-5.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-29 18:59:33.000000 pycatsearch-5.1.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 18:59:49.205547 pycatsearch-5.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-06-29 18:59:33.000000 pycatsearch-5.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:59:49.197547 pycatsearch-5.1.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:59:49.201547 pycatsearch-5.1.8/src/pycatsearch/
--rw-r--r--   0 runner    (1001) docker     (123)    11204 2023-06-29 18:59:33.000000 pycatsearch-5.1.8/src/pycatsearch/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      109 2023-06-29 18:59:33.000000 pycatsearch-5.1.8/src/pycatsearch/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-29 18:59:49.000000 pycatsearch-5.1.8/src/pycatsearch/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    11022 2023-06-29 18:59:33.000000 pycatsearch-5.1.8/src/pycatsearch/async_downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)    18966 2023-06-29 18:59:33.000000 pycatsearch-5.1.8/src/pycatsearch/catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-06-29 18:59:33.000000 pycatsearch-5.1.8/src/pycatsearch/catalog_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)    10619 2023-06-29 18:59:33.000000 pycatsearch-5.1.8/src/pycatsearch/downloader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:59:49.205547 pycatsearch-5.1.8/src/pycatsearch/gui/
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-06-29 18:59:33.000000 pycatsearch-5.1.8/src/pycatsearch/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6602 2023-06-29 18:59:33.000000 pycatsearch-5.1.8/src/pycatsearch/gui/catalog_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    11447 2023-06-29 18:59:33.000000 pycatsearch-5.1.8/src/pycatsearch/gui/download_dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-06-29 18:59:33.000000 pycatsearch-5.1.8/src/pycatsearch/gui/float_spinbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     7984 2023-06-29 18:59:33.000000 pycatsearch-5.1.8/src/pycatsearch/gui/frequency_box.py
--rw-r--r--   0 runner    (1001) docker     (123)     6405 2023-06-29 18:59:33.000000 pycatsearch-5.1.8/src/pycatsearch/gui/menu_bar.py
--rw-r--r--   0 runner    (1001) docker     (123)     8771 2023-06-29 18:59:33.000000 pycatsearch-5.1.8/src/pycatsearch/gui/preferences.py
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-06-29 18:59:33.000000 pycatsearch-5.1.8/src/pycatsearch/gui/selectable_label.py
--rw-r--r--   0 runner    (1001) docker     (123)    13910 2023-06-29 18:59:33.000000 pycatsearch-5.1.8/src/pycatsearch/gui/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     5587 2023-06-29 18:59:33.000000 pycatsearch-5.1.8/src/pycatsearch/gui/substance_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    10318 2023-06-29 18:59:33.000000 pycatsearch-5.1.8/src/pycatsearch/gui/substances_box.py
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-06-29 18:59:33.000000 pycatsearch-5.1.8/src/pycatsearch/gui/titled_list_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)    45716 2023-06-29 18:59:33.000000 pycatsearch-5.1.8/src/pycatsearch/gui/ui.py
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-06-29 18:59:33.000000 pycatsearch-5.1.8/src/pycatsearch/gui/url_label.py
--rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-06-29 18:59:33.000000 pycatsearch-5.1.8/src/pycatsearch/gui/waiting_screen.py
--rw-r--r--   0 runner    (1001) docker     (123)    25239 2023-06-29 18:59:33.000000 pycatsearch-5.1.8/src/pycatsearch/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:59:49.201547 pycatsearch-5.1.8/src/pycatsearch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10690 2023-06-29 18:59:49.000000 pycatsearch-5.1.8/src/pycatsearch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-06-29 18:59:49.000000 pycatsearch-5.1.8/src/pycatsearch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 18:59:49.000000 pycatsearch-5.1.8/src/pycatsearch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-29 18:59:49.000000 pycatsearch-5.1.8/src/pycatsearch.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 18:59:49.000000 pycatsearch-5.1.8/src/pycatsearch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-29 18:59:49.000000 pycatsearch-5.1.8/src/pycatsearch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7966 2023-06-29 18:59:33.000000 pycatsearch-5.1.8/updater.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 07:44:37.456112 pycatsearch-5.1.9.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 07:44:37.448112 pycatsearch-5.1.9.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 07:44:37.452112 pycatsearch-5.1.9.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-07-02 07:44:25.000000 pycatsearch-5.1.9.2/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-02 07:44:25.000000 pycatsearch-5.1.9.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     7642 2023-07-02 07:44:25.000000 pycatsearch-5.1.9.2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10608 2023-07-02 07:44:37.456112 pycatsearch-5.1.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9066 2023-07-02 07:44:25.000000 pycatsearch-5.1.9.2/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1230 2023-07-02 07:44:25.000000 pycatsearch-5.1.9.2/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-07-02 07:44:25.000000 pycatsearch-5.1.9.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-02 07:44:25.000000 pycatsearch-5.1.9.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 07:44:37.456112 pycatsearch-5.1.9.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-07-02 07:44:25.000000 pycatsearch-5.1.9.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 07:44:37.448112 pycatsearch-5.1.9.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 07:44:37.452112 pycatsearch-5.1.9.2/src/pycatsearch/
+-rw-r--r--   0 runner    (1001) docker     (123)    11090 2023-07-02 07:44:25.000000 pycatsearch-5.1.9.2/src/pycatsearch/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      109 2023-07-02 07:44:25.000000 pycatsearch-5.1.9.2/src/pycatsearch/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-02 07:44:37.000000 pycatsearch-5.1.9.2/src/pycatsearch/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11089 2023-07-02 07:44:25.000000 pycatsearch-5.1.9.2/src/pycatsearch/async_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18898 2023-07-02 07:44:25.000000 pycatsearch-5.1.9.2/src/pycatsearch/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-07-02 07:44:25.000000 pycatsearch-5.1.9.2/src/pycatsearch/catalog_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10686 2023-07-02 07:44:25.000000 pycatsearch-5.1.9.2/src/pycatsearch/downloader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 07:44:37.456112 pycatsearch-5.1.9.2/src/pycatsearch/gui/
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-07-02 07:44:25.000000 pycatsearch-5.1.9.2/src/pycatsearch/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6602 2023-07-02 07:44:25.000000 pycatsearch-5.1.9.2/src/pycatsearch/gui/catalog_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11348 2023-07-02 07:44:25.000000 pycatsearch-5.1.9.2/src/pycatsearch/gui/download_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-07-02 07:44:25.000000 pycatsearch-5.1.9.2/src/pycatsearch/gui/float_spinbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8203 2023-07-02 07:44:25.000000 pycatsearch-5.1.9.2/src/pycatsearch/gui/frequency_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-07-02 07:44:25.000000 pycatsearch-5.1.9.2/src/pycatsearch/gui/html_style_delegate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6377 2023-07-02 07:44:25.000000 pycatsearch-5.1.9.2/src/pycatsearch/gui/menu_bar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8771 2023-07-02 07:44:25.000000 pycatsearch-5.1.9.2/src/pycatsearch/gui/preferences.py
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-02 07:44:25.000000 pycatsearch-5.1.9.2/src/pycatsearch/gui/selectable_label.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13861 2023-07-02 07:44:25.000000 pycatsearch-5.1.9.2/src/pycatsearch/gui/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5319 2023-07-02 07:44:25.000000 pycatsearch-5.1.9.2/src/pycatsearch/gui/substance_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14347 2023-07-02 07:44:25.000000 pycatsearch-5.1.9.2/src/pycatsearch/gui/substances_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-07-02 07:44:25.000000 pycatsearch-5.1.9.2/src/pycatsearch/gui/titled_list_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44227 2023-07-02 07:44:25.000000 pycatsearch-5.1.9.2/src/pycatsearch/gui/ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-02 07:44:25.000000 pycatsearch-5.1.9.2/src/pycatsearch/gui/url_label.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-07-02 07:44:25.000000 pycatsearch-5.1.9.2/src/pycatsearch/gui/waiting_screen.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24484 2023-07-02 07:44:25.000000 pycatsearch-5.1.9.2/src/pycatsearch/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 07:44:37.452112 pycatsearch-5.1.9.2/src/pycatsearch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10608 2023-07-02 07:44:37.000000 pycatsearch-5.1.9.2/src/pycatsearch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-07-02 07:44:37.000000 pycatsearch-5.1.9.2/src/pycatsearch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 07:44:37.000000 pycatsearch-5.1.9.2/src/pycatsearch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-02 07:44:37.000000 pycatsearch-5.1.9.2/src/pycatsearch.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 07:44:37.000000 pycatsearch-5.1.9.2/src/pycatsearch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-02 07:44:37.000000 pycatsearch-5.1.9.2/src/pycatsearch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7966 2023-07-02 07:44:25.000000 pycatsearch-5.1.9.2/updater.py
```

### Comparing `pycatsearch-5.1.8/.github/workflows/publish-to-pypi.yml` & `pycatsearch-5.1.9.2/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.8/LICENSE.md` & `pycatsearch-5.1.9.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.8/PKG-INFO` & `pycatsearch-5.1.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycatsearch
-Version: 5.1.8
+Version: 5.1.9.2
 Summary: Yet another implementation of JPL and CDMS spectroscopy catalogs offline search
 Author-email: StSav012 <stsav012@gmail.com>
 License: LGPL-3.0-only
 Project-URL: Source Code, https://github.com/StSav012/pycatsearch
 Project-URL: Bug Tracker, https://github.com/StSav012/pycatsearch/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Win32 (MS Windows)
@@ -70,15 +70,15 @@
 - `entries_count` is the number of the substances loaded by `__init__`.
 - `sources` contains a list of files that have been loaded successfully by `__init__`.
 - `sources_info` returns a list of the files and the timestamps recorded there (if any).
 - `min_frequency` and `max_frequency` are the extreme values of `frequency_limits`.
 
 ###### Functions:
 
-- `__init__(self, *catalog_file_names: str)` accepts names of JSON or GZipped JSON files.
+- `__init__(self, *catalog_file_names: str)` accepts names of JSON or GZip/BZip2/LZMA-compressed JSON files.
   It loads them into memory joined.
 - `filter(self, *,
   min_frequency: float = 0.0,
   max_frequency: float = math.inf,
   min_intensity: float = -math.inf,
   max_intensity: float = math.inf,
   temperature: float = -math.inf,
@@ -90,16 +90,15 @@
   inchi: str = '',
   trivial_name: str = '',
   structural_formula: str = '',
   name: str = '',
   stoichiometric_formula: str = '',
   isotopolog: str = '',
   state: str = '',
-  degrees_of_freedom: Optional[int] = None,
-  timeout: Optional[float] = None) -> List[Dict[str, Union[int, str, List[Dict[str, float]]]]]`
+  degrees_of_freedom: Optional[int] = None) -> List[Dict[str, Union[int, str, List[Dict[str, float]]]]]`
   returns only the catalog entries that meet the criteria specified. The arguments are the following:
     - `float min_frequency`: the lower frequency \[MHz\] to take.
     - `float max_frequency`: the upper frequency \[MHz\] to take.
     - `float min_intensity`: the minimal intensity \[log10(nm²×MHz)\] to take.
     - `float max_intensity`: the maximal intensity \[log10(nm²×MHz)\] to take, use to avoid meta-stable substances.
     - `float temperature`: the temperature to calculate the line intensity at,
       use the catalog intensity if not set.
@@ -114,15 +113,14 @@
     - `str trivial_name`: a string to match the ``trivialname`` field.
     - `str structural_formula`: a string to match the ``structuralformula`` field.
     - `str name`: a string to match the ``name`` field.
     - `str stoichiometric_formula`: a string to match the ``stoichiometricformula`` field.
     - `str isotopolog`: a string to match the ``isotopolog`` field.
     - `str state`: a string to match the ``state`` or the ``state_html`` field.
     - `int degrees_of_freedom`: 0 for atoms, 2 for linear molecules, and 3 for nonlinear molecules.
-    - `float timeout`: maximum time span for the filtering to take.
 - `print(**kwargs)` prints a table of the filtered catalog entries.
   It accepts all the arguments valid for the `filter` function.
 
 ### `downloader`
 
 ###### Sample usage:
```

### Comparing `pycatsearch-5.1.8/README.md` & `pycatsearch-5.1.9.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 - `entries_count` is the number of the substances loaded by `__init__`.
 - `sources` contains a list of files that have been loaded successfully by `__init__`.
 - `sources_info` returns a list of the files and the timestamps recorded there (if any).
 - `min_frequency` and `max_frequency` are the extreme values of `frequency_limits`.
 
 ###### Functions:
 
-- `__init__(self, *catalog_file_names: str)` accepts names of JSON or GZipped JSON files.
+- `__init__(self, *catalog_file_names: str)` accepts names of JSON or GZip/BZip2/LZMA-compressed JSON files.
   It loads them into memory joined.
 - `filter(self, *,
   min_frequency: float = 0.0,
   max_frequency: float = math.inf,
   min_intensity: float = -math.inf,
   max_intensity: float = math.inf,
   temperature: float = -math.inf,
@@ -58,16 +58,15 @@
   inchi: str = '',
   trivial_name: str = '',
   structural_formula: str = '',
   name: str = '',
   stoichiometric_formula: str = '',
   isotopolog: str = '',
   state: str = '',
-  degrees_of_freedom: Optional[int] = None,
-  timeout: Optional[float] = None) -> List[Dict[str, Union[int, str, List[Dict[str, float]]]]]`
+  degrees_of_freedom: Optional[int] = None) -> List[Dict[str, Union[int, str, List[Dict[str, float]]]]]`
   returns only the catalog entries that meet the criteria specified. The arguments are the following:
     - `float min_frequency`: the lower frequency \[MHz\] to take.
     - `float max_frequency`: the upper frequency \[MHz\] to take.
     - `float min_intensity`: the minimal intensity \[log10(nm²×MHz)\] to take.
     - `float max_intensity`: the maximal intensity \[log10(nm²×MHz)\] to take, use to avoid meta-stable substances.
     - `float temperature`: the temperature to calculate the line intensity at,
       use the catalog intensity if not set.
@@ -82,15 +81,14 @@
     - `str trivial_name`: a string to match the ``trivialname`` field.
     - `str structural_formula`: a string to match the ``structuralformula`` field.
     - `str name`: a string to match the ``name`` field.
     - `str stoichiometric_formula`: a string to match the ``stoichiometricformula`` field.
     - `str isotopolog`: a string to match the ``isotopolog`` field.
     - `str state`: a string to match the ``state`` or the ``state_html`` field.
     - `int degrees_of_freedom`: 0 for atoms, 2 for linear molecules, and 3 for nonlinear molecules.
-    - `float timeout`: maximum time span for the filtering to take.
 - `print(**kwargs)` prints a table of the filtered catalog entries.
   It accepts all the arguments valid for the `filter` function.
 
 ### `downloader`
 
 ###### Sample usage:
```

### Comparing `pycatsearch-5.1.8/main.py` & `pycatsearch-5.1.9.2/main.py`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.8/pyproject.toml` & `pycatsearch-5.1.9.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.8/setup.py` & `pycatsearch-5.1.9.2/setup.py`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.8/src/pycatsearch/__init__.py` & `pycatsearch-5.1.9.2/src/pycatsearch/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -153,22 +153,21 @@
     ap_group.add_argument('--name', type=str, help='a string to match the `name` field')
     ap_group.add_argument('--stoichiometric-formula', type=str,
                           help='a string to match the `stoichiometric''formula` field')
     ap_group.add_argument('--isotopolog', type=str, help='a string to match the `isotopolog` field')
     ap_group.add_argument('--state', type=str, help='a string to match the `state` or `state_html` field')
     ap_group.add_argument('--dof', '--degrees_of_freedom', type=int, dest='degrees_of_freedom',
                           help='0 for atoms, 2 for linear molecules, and 3 for nonlinear molecules')
-    ap_group.add_argument('--timeout', type=float, help='maximum time span for the filtering to take')
 
     args: argparse.Namespace = ap.parse_intermixed_args()
 
     arg_names: list[str] = ['min_frequency', 'max_frequency', 'min_intensity', 'max_intensity',
                             'temperature', 'species_tag', 'any_name_or_formula', 'anything', 'any_name', 'any_formula',
                             'inchi_key', 'trivial_name', 'structural_formula', 'name', 'stoichiometric_formula',
-                            'isotopolog', 'state', 'degrees_of_freedom', 'timeout']
+                            'isotopolog', 'state', 'degrees_of_freedom']
     search_args: dict[str, str | float | int] = dict((arg, getattr(args, arg)) for arg in arg_names
                                                      if getattr(args, arg) is not None)
     if search_args:
         c: Catalog = Catalog(*args.catalog)
         c.print(**search_args)
         return 0
```

### Comparing `pycatsearch-5.1.8/src/pycatsearch/async_downloader.py` & `pycatsearch-5.1.9.2/src/pycatsearch/async_downloader.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 try:
     import orjson as json
 except ImportError:
     import json
 
 from .catalog_entry import CatalogEntry
-from .utils import *
+from .utils import LINES, SPECIES_TAG, DEGREES_OF_FREEDOM, within, save_catalog_to_file
 
 __all__ = ['Downloader', 'get_catalog', 'save_catalog', 'download']
 
 logger: logging.Logger = logging.getLogger('async_downloader')
 
 
 class Downloader(Thread):
```

### Comparing `pycatsearch-5.1.8/src/pycatsearch/catalog.py` & `pycatsearch-5.1.9.2/src/pycatsearch/catalog.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,27 +2,29 @@
 from __future__ import annotations
 
 import bz2
 import gzip
 import lzma
 import math
 import os.path
-import time
 from contextlib import contextmanager
 from datetime import datetime, timezone
 from os import PathLike
 from pathlib import Path
 from typing import Any, AnyStr, BinaryIO, Callable, Dict, List, NamedTuple, Optional, TextIO, Union, cast
 
 try:
     import orjson as json
 except ImportError:
     import json
 
-from .utils import *
+from .utils import (M_LOG10E, T0, c, h, k, CATALOG, BUILD_TIME, LINES, FREQUENCY, INTENSITY, STRUCTURAL_FORMULA,
+                    STOICHIOMETRIC_FORMULA, MOLECULE_SYMBOL, SPECIES_TAG, NAME, TRIVIAL_NAME, ISOTOPOLOG, STATE,
+                    STATE_HTML, INCHI_KEY, DEGREES_OF_FREEDOM, LOWER_STATE_ENERGY,
+                    merge_sorted, search_sorted)
 
 __all__ = ['Catalog', 'CatalogSourceInfo', 'LineType', 'LinesType', 'CatalogEntryType']
 
 LineType = Dict[str, float]
 LinesType = List[LineType]
 CatalogEntryType = Dict[str, Union[int, str, LinesType]]
 
@@ -216,15 +218,14 @@
                trivial_name: str = '',
                structural_formula: str = '',
                name: str = '',
                stoichiometric_formula: str = '',
                isotopolog: str = '',
                state: str = '',
                degrees_of_freedom: Optional[int] = None,
-               timeout: Optional[float] = None
                ) -> list[CatalogEntryType]:
         """
         Extract only the entries that match all the specified conditions
 
         :param float min_frequency: the lower frequency [MHz] to take.
         :param float max_frequency: the upper frequency [MHz] to take.
         :param float min_intensity: the minimal intensity [log10(nm²×MHz)] to take.
@@ -242,15 +243,14 @@
         :param str trivial_name: a string to match the ``trivialname`` field.
         :param str structural_formula: a string to match the ``structuralformula`` field.
         :param str name: a string to match the ``name`` field.
         :param str stoichiometric_formula: a string to match the ``stoichiometricformula`` field.
         :param str isotopolog: a string to match the ``isotopolog`` field.
         :param str state: a string to match the ``state`` or the ``state_html`` field.
         :param int degrees_of_freedom: 0 for atoms, 2 for linear molecules, and 3 for nonlinear molecules.
-        :param float timeout: if positive, the maximum time [seconds] for filtering.
         :return: a list of substances with non-empty lists of absorption lines that match all the conditions.
         """
 
         if self.is_empty:
             return []
 
         def filter_by_frequency_and_intensity(catalog_entry: CatalogEntryType) -> CatalogEntryType:
@@ -275,27 +275,24 @@
                 new_catalog_entry[LINES] = []
             return new_catalog_entry
 
         if (min_frequency > max_frequency
                 or min_frequency > self.max_frequency
                 or max_frequency < self.min_frequency):
             return []
-        start_time: float = time.monotonic()
         if (species_tag or inchi_key or trivial_name or structural_formula or name or stoichiometric_formula
                 or isotopolog or state or degrees_of_freedom or any_name or any_formula or any_name_or_formula
                 or anything):
             trivial_name: str = trivial_name.casefold()
             name: str = name.casefold()
             any_name: str = any_name.casefold()
             any_name_or_formula_lowercase: str = any_name_or_formula.casefold()
             anything_lowercase: str = anything.casefold()
             selected_entries: list[CatalogEntryType] = []
             for entry in self.catalog:
-                if timeout is not None and 0.0 < timeout <= time.monotonic() - start_time:
-                    break
                 if ((not species_tag or entry.get(SPECIES_TAG, 0) == species_tag)
                         and (not inchi_key or entry.get(INCHI_KEY, '') == inchi_key)
                         and (not trivial_name or entry.get(TRIVIAL_NAME, '').casefold() == trivial_name)
                         and (not structural_formula or entry.get(STRUCTURAL_FORMULA, '') == structural_formula)
                         and (not name or entry.get(NAME, '').casefold() == name)
                         and (not stoichiometric_formula
                              or entry.get(STOICHIOMETRIC_FORMULA, '') == stoichiometric_formula)
@@ -325,15 +322,14 @@
                     filtered_entry: CatalogEntryType = filter_by_frequency_and_intensity(entry)
                     if filtered_entry[LINES]:
                         selected_entries.append(filtered_entry)
         else:
             filtered_entries: list[CatalogEntryType] = [
                 filter_by_frequency_and_intensity(entry)
                 for entry in self._data.catalog
-                if timeout is None or (timeout > 0.0 and timeout >= time.monotonic() - start_time)
             ]
             selected_entries = [entry for entry in filtered_entries if entry[LINES]]
         return selected_entries
 
     def print(self, **kwargs: None | int | float | str) -> None:
         """
         Print a table of the filtered catalog entries
```

### Comparing `pycatsearch-5.1.8/src/pycatsearch/catalog_entry.py` & `pycatsearch-5.1.9.2/src/pycatsearch/catalog_entry.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # -*- coding: utf-8 -*-
 from __future__ import annotations
 
-import math
+from math import inf, log10, nan
 
-from .utils import *
+from .utils import FREQUENCY, INTENSITY, LOWER_STATE_ENERGY, M_LOG10E, T0, c, h, k
 
 __all__ = ['CatalogEntry']
 
 
 class CatalogEntry:
-    def __init__(self, spcat_line: str = '', *, frequency: float = math.nan, intensity: float = math.nan,
-                 degrees_of_freedom: int = -1, lower_state_energy: float = math.nan) -> None:
+    def __init__(self, spcat_line: str = '', *, frequency: float = nan, intensity: float = nan,
+                 degrees_of_freedom: int = -1, lower_state_energy: float = nan) -> None:
         self.FREQ: float  # frequency, MHz, mandatory
         self.INT: float  # intensity, log10(nm²×MHz), mandatory
         self.DR: int  # degrees of freedom: 0 for atoms, 2 for linear molecules, and 3 for nonlinear molecules.
         self.ELO: float  # lower state energy relative to the ground state, 1/cm
         self.FREQ = frequency
         self.INT = intensity
         self.DR = degrees_of_freedom
@@ -29,17 +29,17 @@
             self.DR = int(spcat_line[29:31])
             self.ELO = float(spcat_line[31:41])
 
     @property
     def frequency(self) -> float:
         return self.FREQ
 
-    def intensity(self, temperature: float = -math.inf) -> float:
+    def intensity(self, temperature: float = -inf) -> float:
         if self.DR >= 0 and temperature > 0. and temperature != T0:
-            return self.INT + (0.5 * self.DR + 1.0) * math.log10(T0 / temperature) + (
+            return self.INT + (0.5 * self.DR + 1.0) * log10(T0 / temperature) + (
                     -(1 / temperature - 1 / T0) * self.ELO * 100. * h * c / k) * M_LOG10E
         else:
             return self.INT
 
     @property
     def degrees_of_freedom(self) -> int:
         return self.DR
```

### Comparing `pycatsearch-5.1.8/src/pycatsearch/downloader.py` & `pycatsearch-5.1.9.2/src/pycatsearch/downloader.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 try:
     import orjson as json
 except ImportError:
     import json
 
 from .catalog_entry import CatalogEntry
-from .utils import *
+from .utils import LINES, SPECIES_TAG, DEGREES_OF_FREEDOM, within, save_catalog_to_file
 
 __all__ = ['Downloader', 'get_catalog', 'save_catalog', 'download']
 
 logger: logging.Logger = logging.getLogger('downloader')
 
 
 class Downloader(Thread):
```

### Comparing `pycatsearch-5.1.8/src/pycatsearch/gui/catalog_info.py` & `pycatsearch-5.1.9.2/src/pycatsearch/gui/catalog_info.py`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.8/src/pycatsearch/gui/download_dialog.py` & `pycatsearch-5.1.9.2/src/pycatsearch/gui/download_dialog.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from qtpy.compat import getsavefilename
 
 try:
     from ..async_downloader import Downloader
 except (SyntaxError, ImportError, ModuleNotFoundError):
     from ..downloader import Downloader
 from .waiting_screen import WaitingScreen
-from ..utils import all_cases, ensure_prefix, save_catalog_to_file
+from ..utils import ensure_prefix, save_catalog_to_file
 
 
 __all__ = ['DownloadDialog']
 
 
 class SettingsPage(QWizardPage):
     def __init__(self, parent: QWidget | None = None) -> None:
@@ -229,19 +229,18 @@
 
     def done(self, exit_code: QDialog.DialogCode) -> None:
         if self.progress_page.downloader is not None and self.progress_page.downloader.is_alive():
             self.progress_page.downloader.join(0.1)
 
         if exit_code == QDialog.DialogCode.Accepted and self.catalog:
             _formats: dict[tuple[str, ...], str] = {
-                tuple(all_cases('.json.gz')): self.tr('JSON with GZip compression', 'file type'),
-                tuple(all_cases('.json.bz2')): self.tr('JSON with Bzip2 compression', 'file type'),
-                (*all_cases('.json.xz'), *all_cases('.json.lzma')):
-                    self.tr('JSON with LZMA2 compression', 'file type'),
-                tuple(all_cases('.json')): self.tr('JSON', 'file type'),
+                ('.json.gz',): self.tr('JSON with GZip compression', 'file type'),
+                ('.json.bz2',): self.tr('JSON with Bzip2 compression', 'file type'),
+                ('.json.xz', '.json.lzma',): self.tr('JSON with LZMA2 compression', 'file type'),
+                ('.json',): self.tr('JSON', 'file type'),
             }
             save_file_name: str
             save_file_name, _ = self._get_save_file_name(formats=_formats, caption=self.tr('Save As...'))
             if not save_file_name:
                 return
 
             ws: WaitingScreen = WaitingScreen(
```

### Comparing `pycatsearch-5.1.8/src/pycatsearch/gui/float_spinbox.py` & `pycatsearch-5.1.9.2/src/pycatsearch/gui/float_spinbox.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,50 +1,53 @@
 # -*- coding: utf-8 -*-
 from __future__ import annotations
 
-import math
-from typing import Final, Optional
+import enum
+from math import floor, log10
 
 from qtpy.QtGui import QValidator
 from qtpy.QtWidgets import QDoubleSpinBox, QWidget
 
 __all__ = ['FloatSpinBox']
 
 
 class FloatSpinBox(QDoubleSpinBox):
-    MODES: Final[list[str]] = ['auto', 'fixed', 'scientific']
+    class Mode(enum.Enum):
+        auto = enum.auto()
+        fixed = enum.auto()
+        scientific = enum.auto()
 
-    def __init__(self, parent: Optional[QWidget] = None) -> None:
+    def __init__(self, parent: QWidget | None = None) -> None:
         super().__init__(parent)
-        self._mode: str = 'auto'
+        self._mode: FloatSpinBox.Mode = FloatSpinBox.Mode.auto
         self._decimals: int = 2
         super().setDecimals(1000)
 
     @property
-    def mode(self) -> str:
+    def mode(self) -> Mode:
         return self._mode
 
     @mode.setter
-    def mode(self, new_mode: str) -> None:
-        if new_mode not in self.MODES:
-            raise ValueError(f'Invalid mode: {new_mode}')
+    def mode(self, new_mode: 'FloatSpinBox.Mode') -> None:
+        if not isinstance(new_mode, FloatSpinBox.Mode):
+            raise TypeError(f'Invalid mode: {new_mode}')
         self._mode = new_mode
 
     def valueFromText(self, text: str) -> float:
         return float(text.strip().split()[0])
 
     def textFromValue(self, v: float) -> str:
-        if self._mode == 'auto':
+        if self._mode == FloatSpinBox.Mode.auto:
             if abs(v) < self.singleStep() and v != 0.0:
                 return f'{v:.{self._decimals}e}'
             else:
                 return f'{v:.{self._decimals}f}'
-        elif self._mode == 'fixed':
+        elif self._mode == FloatSpinBox.Mode.fixed:
             return f'{v:.{self._decimals}f}'
-        elif self._mode == 'scientific':
+        elif self._mode == FloatSpinBox.Mode.scientific:
             return f'{v:.{self._decimals}e}'
         else:
             raise RuntimeError(f'Unknown mode {self._mode}')
 
     def validate(self, text: str, pos: int) -> tuple[QValidator.State, str, int]:
         try:
             self.valueFromText(text)
@@ -61,15 +64,15 @@
                 continue
             else:
                 return word
         return ''
 
     def stepBy(self, steps: int) -> None:
         if self.value() != 0.0:
-            exp: int = round(math.floor(math.log10(abs(self.value()))))
+            exp: int = round(floor(log10(abs(self.value()))))
             self.setValue(self.value() + self.singleStep() * steps * 10.0 ** exp)
         else:
             self.setValue(self.singleStep() * steps)
 
     def decimals(self) -> int:
         return self._decimals
```

### Comparing `pycatsearch-5.1.8/src/pycatsearch/gui/frequency_box.py` & `pycatsearch-5.1.9.2/src/pycatsearch/gui/frequency_box.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # -*- coding: utf-8 -*-
 from __future__ import annotations
 
 from math import inf
+from typing import Callable
 
-from qtpy.QtCore import Qt, Slot
+from qtpy.QtCore import Qt, Signal, Slot
 from qtpy.QtWidgets import QAbstractSpinBox, QDoubleSpinBox, QFormLayout, QTabWidget, QWidget
 
 from .settings import Settings
-from ..utils import *
 
 __all__ = ['FrequencyBox']
 
 
 class FrequencySpinBox(QDoubleSpinBox):
     """`QDoubleSpinBox` with altered defaults"""
     def __init__(self, parent: QWidget | None = None) -> None:
@@ -21,17 +21,20 @@
                           | Qt.AlignmentFlag.AlignVCenter)
         self.setButtonSymbols(QAbstractSpinBox.ButtonSymbols.NoButtons)
         self.setAccelerated(True)
         self.setDecimals(4)
         self.setMaximum(9999999.9999)
         self.setSuffix(self.tr(' MHz'))
         self.setCorrectionMode(QAbstractSpinBox.CorrectionMode.CorrectToNearestValue)
+        self.setKeyboardTracking(False)  # not to emit signals while typing
 
 
 class FrequencyBox(QTabWidget):
+    frequencyLimitsChanged: Signal = Signal(name='frequencyLimitsChanged')
+
     def __init__(self, settings: Settings, parent: QWidget | None = None) -> None:
         from . import icon  # import locally to avoid a circular import
 
         super().__init__(parent)
 
         self._settings: Settings = settings
 
@@ -47,33 +50,33 @@
         self._page_by_center: QWidget = QWidget()
         self._layout_by_center: QFormLayout = QFormLayout(self._page_by_center)
         self._spin_frequency_center: FrequencySpinBox = FrequencySpinBox(self._page_by_center)
         self._spin_frequency_deviation: FrequencySpinBox = FrequencySpinBox(self._page_by_center)
 
         self._layout_by_range.setLabelAlignment(Qt.AlignmentFlag.AlignLeft)
         self._spin_frequency_from.setValue(118747.341)
-        self._layout_by_range.addRow(self._layout_by_range.tr('From:'), self._spin_frequency_from)
+        self._layout_by_range.addRow(self.tr('From:'), self._spin_frequency_from)
         self._spin_frequency_to.setValue(118753.341)
-        self._layout_by_range.addRow(self._layout_by_range.tr('To:'), self._spin_frequency_to)
+        self._layout_by_range.addRow(self.tr('To:'), self._spin_frequency_to)
         self.addTab(self._page_by_range, icon('mdi6.arrow-expand-horizontal'), self.tr('Range'))
 
         self._spin_frequency_center.setValue(118750.341)
-        self._layout_by_center.addRow(self._layout_by_center.tr('Center:'), self._spin_frequency_center)
+        self._layout_by_center.addRow(self.tr('Center:'), self._spin_frequency_center)
         self._spin_frequency_deviation.setMaximum(99.9999)
         self._spin_frequency_deviation.setSingleStep(0.1)
         self._spin_frequency_deviation.setValue(0.4)
-        self._layout_by_center.addRow(self._layout_by_center.tr('Deviation:'), self._spin_frequency_deviation)
+        self._layout_by_center.addRow(self.tr('Deviation:'), self._spin_frequency_deviation)
         self.addTab(self._page_by_center, icon('mdi6.format-horizontal-align-center'), self.tr('Center'))
 
         self.load_settings()
 
-        self._spin_frequency_from.editingFinished.connect(self._on_spin_frequency_from_edited)
-        self._spin_frequency_to.editingFinished.connect(self._on_spin_frequency_to_edited)
-        self._spin_frequency_center.editingFinished.connect(self._on_spin_frequency_center_edited)
-        self._spin_frequency_deviation.editingFinished.connect(self._on_spin_frequency_deviation_edited)
+        self._spin_frequency_from.valueChanged.connect(self._on_spin_frequency_from_edited)
+        self._spin_frequency_to.valueChanged.connect(self._on_spin_frequency_to_edited)
+        self._spin_frequency_center.valueChanged.connect(self._on_spin_frequency_center_edited)
+        self._spin_frequency_deviation.valueChanged.connect(self._on_spin_frequency_deviation_edited)
 
     def load_settings(self) -> None:
         self._settings.beginGroup('search')
         self._settings.beginGroup('frequency')
         self._frequency_from = self._settings.value('from', self._spin_frequency_from.value(), float)
         self._frequency_to = self._settings.value('to', self._spin_frequency_to.value(), float)
         self._frequency_center = self._settings.value('center', self._spin_frequency_center.value(), float)
@@ -111,45 +114,50 @@
         min_value = self._settings.from_mhz(min_value)
         max_value = self._settings.from_mhz(max_value)
         spin: QDoubleSpinBox
         for spin in frequency_spins:
             spin.setMinimum(min_value)
             spin.setMaximum(max_value)
 
-    @Slot()
-    def _on_spin_frequency_from_edited(self) -> None:
-        self._frequency_from = self._settings.to_mhz(self._spin_frequency_from.value())
-
-    @Slot()
-    def _on_spin_frequency_to_edited(self) -> None:
-        self._frequency_to = self._settings.to_mhz(self._spin_frequency_to.value())
-
-    @Slot()
-    def _on_spin_frequency_center_edited(self) -> None:
-        self._frequency_center = self._settings.to_mhz(self._spin_frequency_center.value())
-
-    @Slot()
-    def _on_spin_frequency_deviation_edited(self) -> None:
-        self._frequency_deviation = self._settings.to_mhz(self._spin_frequency_deviation.value())
+    @Slot(float)
+    def _on_spin_frequency_from_edited(self, value: float) -> None:
+        self._frequency_from = self._settings.to_mhz(value)
+        self.frequencyLimitsChanged.emit()
+
+    @Slot(float)
+    def _on_spin_frequency_to_edited(self, value: float) -> None:
+        self._frequency_to = self._settings.to_mhz(value)
+        self.frequencyLimitsChanged.emit()
+
+    @Slot(float)
+    def _on_spin_frequency_center_edited(self, value: float) -> None:
+        self._frequency_center = self._settings.to_mhz(value)
+        self.frequencyLimitsChanged.emit()
+
+    @Slot(float)
+    def _on_spin_frequency_deviation_edited(self, value: float) -> None:
+        self._frequency_deviation = self._settings.to_mhz(value)
+        self.frequencyLimitsChanged.emit()
 
     def fill_parameters(self) -> None:
         frequency_suffix: int = self._settings.frequency_unit
         frequency_suffix_str: str = ' ' + self._settings.FREQUENCY_UNITS[frequency_suffix]
+        from_mhz: Callable[[float], float] = self._settings.from_mhz
         if frequency_suffix in (0, 1, 2):  # MHz, GHz, cm⁻¹
-            self._spin_frequency_from.setValue(self._settings.from_mhz(self._frequency_from))
-            self._spin_frequency_to.setValue(self._settings.from_mhz(self._frequency_to))
-            self._spin_frequency_center.setValue(self._settings.from_mhz(self._frequency_center))
-            self._spin_frequency_deviation.setValue(self._settings.from_mhz(self._frequency_deviation))
+            self._spin_frequency_from.setValue(from_mhz(self._frequency_from))
+            self._spin_frequency_to.setValue(from_mhz(self._frequency_to))
+            self._spin_frequency_center.setValue(from_mhz(self._frequency_center))
+            self._spin_frequency_deviation.setValue(from_mhz(self._frequency_deviation))
         elif frequency_suffix == 3:  # nm
-            self._spin_frequency_from.setValue(mhz_to_nm(self._frequency_from))
-            self._spin_frequency_to.setValue(mhz_to_nm(self._frequency_to))
-            self._spin_frequency_center.setValue(mhz_to_nm(self._frequency_center))
+            self._spin_frequency_from.setValue(from_mhz(self._frequency_from))
+            self._spin_frequency_to.setValue(from_mhz(self._frequency_to))
+            self._spin_frequency_center.setValue(from_mhz(self._frequency_center))
             self._spin_frequency_deviation.setValue(
-                abs(mhz_to_nm(self._frequency_center - self._frequency_deviation) -
-                    mhz_to_nm(self._frequency_center + self._frequency_deviation)) / 2.0)
+                abs(from_mhz(self._frequency_center - self._frequency_deviation) -
+                    from_mhz(self._frequency_center + self._frequency_deviation)) / 2.0)
         else:
             raise IndexError('Wrong frequency unit index', frequency_suffix)
         precision: int = [4, 7, 8, 8][frequency_suffix]
         step_factor: float = [2.5, 2.5, 2.5, 0.25][frequency_suffix]
         frequency_spins: list[QDoubleSpinBox] = [self._spin_frequency_from, self._spin_frequency_to,
                                                  self._spin_frequency_center, self._spin_frequency_deviation]
         for spin in frequency_spins:
```

### Comparing `pycatsearch-5.1.8/src/pycatsearch/gui/menu_bar.py` & `pycatsearch-5.1.9.2/src/pycatsearch/gui/menu_bar.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,16 +40,15 @@
         self.menu_edit.addSeparator()
         self.menu_copy_only: QMenu = self.menu_edit.addMenu(self.tr('Copy &Only'))
         self.action_copy_current: QAction = self.menu_copy_only.addAction(self.tr('Active &Cell'))
         self.menu_copy_only.addSeparator()
         self.action_copy_name: QAction = self.menu_copy_only.addAction(self.tr('&Substance Name'))
         self.action_copy_frequency: QAction = self.menu_copy_only.addAction(self.tr('&Frequency'))
         self.action_copy_intensity: QAction = self.menu_copy_only.addAction(self.tr('&Intensity'))
-        self.action_copy_lower_state_energy: QAction = self.menu_copy_only.addAction(
-            self.menu_copy_only.tr('&Lower State Energy'))
+        self.action_copy_lower_state_energy: QAction = self.menu_copy_only.addAction(self.tr('&Lower State Energy'))
         self.action_copy: QAction = self.menu_edit.addAction(
             self._icon('edit-copy', 'mdi6.content-copy'),
             self.tr('Co&py Selection'))
         self.menu_edit.addSeparator()
         self.action_select_all: QAction = self.menu_edit.addAction(
             self._icon('edit-select-all', 'mdi6.select-all'),
             self.tr('&Select All'))
```

### Comparing `pycatsearch-5.1.8/src/pycatsearch/gui/preferences.py` & `pycatsearch-5.1.9.2/src/pycatsearch/gui/preferences.py`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.8/src/pycatsearch/gui/settings.py` & `pycatsearch-5.1.9.2/src/pycatsearch/gui/settings.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,19 @@
 from __future__ import annotations
 
 import os
 from typing import Any, Callable, Final, Hashable, Iterable, NamedTuple, Sequence
 
 from qtpy.QtCore import QObject, QSettings
 
-from ..utils import *
+from ..utils import (cm_per_molecule_to_log10_sq_nm_mhz, ghz_to_mhz, j_to_rec_cm,
+                     log10_cm_per_molecule_to_log10_sq_nm_mhz, log10_sq_nm_mhz_to_cm_per_molecule,
+                     log10_sq_nm_mhz_to_log10_cm_per_molecule, log10_sq_nm_mhz_to_sq_nm_mhz, meV_to_rec_cm, mhz_to_ghz,
+                     mhz_to_nm, mhz_to_rec_cm, nm_to_mhz, rec_cm_to_j, rec_cm_to_meV, rec_cm_to_mhz,
+                     sq_nm_mhz_to_log10_sq_nm_mhz)
 
 __all__ = ['Settings']
 
 
 class Settings(QSettings):
     """ convenient internal representation of the application settings """
 
@@ -89,31 +93,33 @@
         self.FREQUENCY_UNITS: Final[list[str]] = [self.tr('MHz'), self.tr('GHz'), self.tr('cm⁻¹'), self.tr('nm')]
         self.INTENSITY_UNITS: Final[list[str]] = [self.tr('lg(nm² × MHz)'), self.tr('nm² × MHz'),
                                                   self.tr('lg(cm / molecule)'), self.tr('cm / molecule')]
         self.ENERGY_UNITS: Final[list[str]] = [self.tr('cm⁻¹'), self.tr('meV'), self.tr('J')]
         self.TEMPERATURE_UNITS: Final[list[str]] = [self.tr('K'), self.tr('°C')]
 
     @property
-    def dialog(self) -> (dict[(str
-                               | tuple[str, tuple[str, ...]]
-                               | tuple[str, tuple[str, ...], tuple[tuple[str, Any], ...]]),
-    dict[str, (Settings.CallbackOnly
-               | Settings.SpinboxAndCallback
-               | Settings.ComboboxAndCallback)]]):
+    def dialog(self) -> (
+            dict[
+                (str
+                 | tuple[str, tuple[str, ...]]
+                 | tuple[str, tuple[str, ...], tuple[tuple[str, Any], ...]]
+                ),
+                dict[str, (CallbackOnly
+                           | SpinboxAndCallback
+                           | ComboboxAndCallback)]
+            ]
+    ):
         return {
             (self.tr('When the program starts'), ('mdi6.rocket-launch',)): {
                 self.tr('Load catalogs'): Settings.CallbackOnly('load_last_catalogs'),
                 self.tr('Check for update'): Settings.CallbackOnly('check_updates'),
             },
             (self.tr('Display'), ('mdi6.binoculars',)): {
                 self.tr('Allow rich text in formulas'): Settings.CallbackOnly('rich_text_in_formulas'),
             },
-            (self.tr('Search'), ('mdi6.table-search',)): {
-                self.tr('Timeout:'): Settings.SpinboxAndCallback(slice(1, 99), ('', 'sec'), 'timeout'),
-            },
             (self.tr('Units'), ('mdi6.pencil-ruler',)): {
                 self.tr('Frequency:'): Settings.ComboboxAndCallback(self.FREQUENCY_UNITS, 'frequency_unit'),
                 self.tr('Intensity:'): Settings.ComboboxAndCallback(self.INTENSITY_UNITS, 'intensity_unit'),
                 self.tr('Energy:'): Settings.ComboboxAndCallback(self.ENERGY_UNITS, 'energy_unit'),
                 self.tr('Temperature:'): Settings.ComboboxAndCallback(self.TEMPERATURE_UNITS, 'temperature_unit'),
             },
             (self.tr('Export'), ('mdi6.file-export',)): {
@@ -350,27 +356,14 @@
     @with_units.setter
     def with_units(self, new_value: bool) -> None:
         self.beginGroup('export')
         self.setValue('withUnits', new_value)
         self.endGroup()
 
     @property
-    def timeout(self) -> float:
-        self.beginGroup('search')
-        v: float = self.value('timeout', 99.0, float)
-        self.endGroup()
-        return v
-
-    @timeout.setter
-    def timeout(self, new_value: float) -> None:
-        self.beginGroup('search')
-        self.setValue('timeout', new_value)
-        self.endGroup()
-
-    @property
     def ignored_version(self) -> str:
         self.beginGroup('update')
         v: str = self.value('ignoredVersion', '', str)
         self.endGroup()
         return v
 
     @ignored_version.setter
```

### Comparing `pycatsearch-5.1.8/src/pycatsearch/gui/substance_info.py` & `pycatsearch-5.1.9.2/src/pycatsearch/gui/substance_info.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,101 +1,89 @@
 # -*- coding: utf-8 -*-
 from __future__ import annotations
 
 from typing import Collection
 
-from qtpy.QtCore import QModelIndex, Qt, Slot
-from qtpy.QtWidgets import (QDialog, QDialogButtonBox, QFormLayout, QLabel, QListWidget, QListWidgetItem, QVBoxLayout,
-                            QWidget)
+from qtpy.QtCore import QModelIndex, Qt, Signal, Slot
+from qtpy.QtWidgets import QDialog, QDialogButtonBox, QFormLayout, QListWidget, QListWidgetItem, QVBoxLayout, QWidget
 
+from .html_style_delegate import HTMLDelegate
 from .selectable_label import SelectableLabel
 from .url_label import URLLabel
 from ..catalog import Catalog
-from ..utils import *
+from ..utils import HUMAN_READABLE, ID, INCHI_KEY, LINES, SPECIES_TAG, STATE_HTML, best_name, chem_html
 
 __all__ = ['SubstanceInfoSelector', 'SubstanceInfo']
 
 
 class SubstanceInfoSelector(QDialog):
-    def __init__(self, catalog: Catalog, entry_ids: Collection[int],
+    tagSelectionChanged: Signal = Signal(int, bool, name='tagSelectionChanged')
+
+    def __init__(self, catalog: Catalog, species_tags: Collection[int], *,
+                 selected_species_tags: Collection[int] = (),
                  allow_html: bool = True, inchi_key_search_url_template: str = '',
                  parent: QWidget | None = None) -> None:
         super().__init__(parent)
         self._catalog: Catalog = catalog
         self._inchi_key_search_url_template: str = inchi_key_search_url_template
         self.setModal(True)
         self.setWindowTitle(self.tr('Select Substance'))
         if parent is not None:
             self.setWindowIcon(parent.windowIcon())
         layout: QVBoxLayout = QVBoxLayout(self)
         self._list_box: QListWidget = QListWidget(self)
-        self._list_box.itemSelectionChanged.connect(self._on_list_selection_changed)
+        self._list_box.itemChanged.connect(self._on_list_item_changed)
         self._list_box.doubleClicked.connect(self._on_list_double_clicked)
+        self._list_box.setItemDelegateForColumn(0, HTMLDelegate())
         layout.addWidget(self._list_box)
-        entry_ids = set(entry_ids)
+        species_tags = set(species_tags)
         for entry in catalog.catalog:
-            if not entry_ids:
+            if not species_tags:
                 break  # nothing to search for
-            if entry[ID] in entry_ids:
-                entry_ids.discard(entry[ID])  # don't search for the ID again
+            if (species_tag := entry[SPECIES_TAG]) in species_tags:
+                species_tags.discard(species_tag)  # don't search for the SPECIES_TAG again
                 # don't specify the parent here: https://t.me/qtforpython/20950
-                item: QListWidgetItem = QListWidgetItem()
-                item.setData(Qt.ItemDataRole.ToolTipRole, str(entry[SPECIES_TAG]))
-                item.setData(Qt.ItemDataRole.UserRole, entry[ID])
+                item: QListWidgetItem = QListWidgetItem(best_name(entry, allow_html=allow_html))
+                item.setData(Qt.ItemDataRole.ToolTipRole, str(species_tag))
+                item.setData(Qt.ItemDataRole.UserRole, species_tag)
+                item.setCheckState(Qt.CheckState.Checked
+                                   if species_tag in selected_species_tags
+                                   else Qt.CheckState.Unchecked)
                 self._list_box.addItem(item)
-                self._list_box.setItemWidget(item, QLabel(best_name(entry, allow_html=allow_html)))
-        self._buttons: QDialogButtonBox = QDialogButtonBox(
-            (QDialogButtonBox.StandardButton.Ok | QDialogButtonBox.StandardButton.Close), self)
-        self._buttons.button(QDialogButtonBox.StandardButton.Ok).setEnabled(False)
-        self._buttons.accepted.connect(self._on_accept)
+        self._buttons: QDialogButtonBox = QDialogButtonBox(QDialogButtonBox.StandardButton.Close, self)
         self._buttons.rejected.connect(self.reject)
         layout.addWidget(self._buttons)
 
-    @Slot()
-    def _on_list_selection_changed(self) -> None:
-        self._buttons.button(QDialogButtonBox.StandardButton.Ok).setEnabled(bool(self._list_box.selectedIndexes()))
+    @Slot(QListWidgetItem)
+    def _on_list_item_changed(self, item: QListWidgetItem) -> None:
+        self.tagSelectionChanged.emit(item.data(Qt.ItemDataRole.UserRole), item.checkState() == Qt.CheckState.Checked)
 
     @Slot(QModelIndex)
     def _on_list_double_clicked(self, index: QModelIndex) -> None:
-        self.hide()
         item: QListWidgetItem = self._list_box.item(index.row())
         syn: SubstanceInfo = SubstanceInfo(self._catalog, item.data(Qt.ItemDataRole.UserRole),
                                            inchi_key_search_url_template=self._inchi_key_search_url_template,
-                                           parent=self.parent())
-        syn.exec()
-        self.accept()
-
-    @Slot()
-    def _on_accept(self) -> None:
-        selected_items: list[QListWidgetItem] = self._list_box.selectedItems()
-        if not selected_items:
-            return
-        self.hide()
-        item: QListWidgetItem = selected_items.pop()
-        syn: SubstanceInfo = SubstanceInfo(self._catalog, item.data(Qt.ItemDataRole.UserRole),
-                                           inchi_key_search_url_template=self._inchi_key_search_url_template,
-                                           parent=self.parent())
+                                           parent=self)
         syn.exec()
-        self.accept()
 
 
 class SubstanceInfo(QDialog):
     """ A simple dialog that displays the information about a substance from the loaded catalog """
 
-    def __init__(self, catalog: Catalog, entry_id: int, inchi_key_search_url_template: str = '',
+    def __init__(self, catalog: Catalog, species_tag: int, inchi_key_search_url_template: str = '',
                  parent: QWidget | None = None) -> None:
         super().__init__(parent)
         self.setModal(True)
         self.setWindowTitle(self.tr('Substance Info'))
         if parent is not None:
             self.setWindowIcon(parent.windowIcon())
         layout: QFormLayout = QFormLayout(self)
         label: SelectableLabel
         for entry in catalog.catalog:
-            if entry[ID] == entry_id:
+            if entry[SPECIES_TAG] == species_tag:
                 for key in entry:
                     if key == LINES:
                         continue
                     elif key == ID:
                         label = URLLabel(
                             url=f'https://cdms.astro.uni-koeln.de/cdms/portal/catalog/{entry[key]}/',
                             text=f'{entry[key]}',
```

### Comparing `pycatsearch-5.1.8/src/pycatsearch/gui/titled_list_widget.py` & `pycatsearch-5.1.9.2/src/pycatsearch/gui/titled_list_widget.py`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.8/src/pycatsearch/gui/ui.py` & `pycatsearch-5.1.9.2/src/pycatsearch/gui/ui.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,39 @@
 # -*- coding: utf-8 -*-
 from __future__ import annotations
 
-import math
+import sys
+from math import inf
 from typing import Any, Callable, Final, final
 
 from qtpy.QtCore import (QAbstractTableModel, QByteArray, QItemSelection, QMimeData, QModelIndex, QPersistentModelIndex,
-                         QPoint, QPointF, QRect, QSize, Qt, Slot)
-from qtpy.QtGui import (QAbstractTextDocumentLayout, QClipboard, QCloseEvent, QCursor, QIcon, QPainter, QPixmap,
-                        QScreen, QTextDocument)
+                         QPoint, Qt, Slot, QLocale)
+from qtpy.QtGui import QClipboard, QCloseEvent, QCursor, QIcon, QPixmap, QScreen
 from qtpy.QtWidgets import (QAbstractItemView, QAbstractSpinBox, QApplication, QDoubleSpinBox, QFormLayout, QHeaderView,
-                            QMainWindow, QMessageBox, QPushButton, QSplitter, QStatusBar, QStyle, QStyleOptionViewItem,
-                            QStyledItemDelegate, QTableView, QVBoxLayout, QWidget)
+                            QMainWindow, QMessageBox, QPushButton, QSplitter, QStatusBar, QTableView, QVBoxLayout,
+                            QWidget)
 from qtpy.compat import getopenfilenames
 
 from .catalog_info import CatalogInfo
 from .download_dialog import DownloadDialog
 from .float_spinbox import FloatSpinBox
 from .frequency_box import FrequencyBox
+from .html_style_delegate import HTMLDelegate
 from .menu_bar import MenuBar
 from .preferences import Preferences
 from .settings import Settings
 from .substance_info import SubstanceInfo
 from .substances_box import SubstancesBox
 from .. import __version__
 from ..catalog import Catalog, CatalogEntryType
-from ..utils import *
+from ..utils import (FREQUENCY, INTENSITY, LINES, LOWER_STATE_ENERGY, ReleaseInfo, SPECIES_TAG, best_name,
+                     ensure_prefix, latest_release, remove_html, update_with_pip, wrap_in_html)
+
+if sys.version_info < (3, 10):
+    from ..utils import zip
 
 __all__ = ['UI']
 
 
 def copy_to_clipboard(text: str, text_type: Qt.TextFormat | str = Qt.TextFormat.PlainText) -> None:
     clipboard: QClipboard = QApplication.clipboard()
     if not text:
@@ -47,84 +52,47 @@
 def substitute(fmt: str, *args: Any) -> str:
     res: str = fmt
     for index, value in enumerate(args):
         res = res.replace(f'{{{index}}}', str(value))
     return res
 
 
-class HTMLDelegate(QStyledItemDelegate):
-    @staticmethod
-    def anchorAt(html: str, point: QPoint | QPointF) -> str:
-        doc: QTextDocument = QTextDocument()
-        doc.setHtml(html)
-        text_layout: QAbstractTextDocumentLayout = doc.documentLayout()
-        return text_layout.anchorAt(point)
-
-    def paint(self, painter: QPainter, option: QStyleOptionViewItem, index: QModelIndex | QPersistentModelIndex) -> None:
-        self.initStyleOption(option, index)
-        style: QStyle
-        if option.widget:
-            style = option.widget.style()
-        else:
-            style = QApplication.style()
-        doc: QTextDocument = QTextDocument()
-        doc.setHtml(option.text)
-        option.text = ''
-        style.drawControl(QStyle.ControlElement.CE_ItemViewItem, option, painter)
-        ctx: QAbstractTextDocumentLayout.PaintContext = QAbstractTextDocumentLayout.PaintContext()
-        text_rect: QRect = style.subElementRect(QStyle.SubElement.SE_ItemViewItemText, option)
-        painter.save()
-        painter.translate(text_rect.topLeft())
-        painter.setClipRect(text_rect.translated(-text_rect.topLeft()))
-        painter.translate(0, 0.5 * (option.rect.height() - doc.size().height()))
-        doc.documentLayout().draw(painter, ctx)
-        painter.restore()
-
-    def sizeHint(self, option: QStyleOptionViewItem | None, index: QModelIndex | QPersistentModelIndex) -> QSize:
-        options: QStyleOptionViewItem = QStyleOptionViewItem(option)
-        self.initStyleOption(options, index)
-        doc: QTextDocument = QTextDocument()
-        doc.setHtml(options.text)
-        doc.setTextWidth(options.rect.width())
-        return QSize(round(doc.idealWidth()), round(doc.size().height()))
-
-
 class LinesListModel(QAbstractTableModel):
     ROW_BATCH_COUNT: Final[int] = 5
 
     class DataType:
-        __slots__ = ['id', 'name',
+        __slots__ = ['species_tag', 'name',
                      'frequency_str', 'frequency',
                      'intensity_str', 'intensity',
                      'lower_state_energy_str', 'lower_state_energy']
 
         def __init__(self,
-                     species_id: int, name: str,
+                     species_tag: int, name: str,
                      frequency_str: str, frequency: float,
                      intensity_str: str, intensity: float,
                      lower_state_energy_str: str, lower_state_energy: float) -> None:
-            self.id: int = species_id
+            self.species_tag: int = species_tag
             self.name: str = name
             self.frequency_str: str = frequency_str
             self.frequency: float = frequency
             self.intensity_str: str = intensity_str
             self.intensity: float = intensity
             self.lower_state_energy_str: str = lower_state_energy_str
             self.lower_state_energy: float = lower_state_energy
 
-        def __eq__(self, other: LinesListModel.DataType) -> int:
+        def __eq__(self, other: 'LinesListModel.DataType') -> int:
             if not isinstance(other, LinesListModel.DataType):
                 return NotImplemented
-            return (self.id == other.id
+            return (self.species_tag == other.species_tag
                     and self.frequency == other.frequency
                     and self.intensity == other.intensity
                     and self.lower_state_energy == other.lower_state_energy)
 
         def __hash__(self) -> int:
-            return hash(self.id) ^ hash(self.frequency) ^ hash(self.lower_state_energy)
+            return hash(self.species_tag) ^ hash(self.frequency) ^ hash(self.lower_state_energy)
 
     def __init__(self, settings: Settings, parent: QWidget | None = None) -> None:
         super().__init__(parent)
         self._settings: Settings = settings
         self._entries: list[CatalogEntryType] = []
         self._data: list[LinesListModel.DataType] = []
         self._rows_loaded: int = LinesListModel.ROW_BATCH_COUNT
@@ -160,15 +128,15 @@
                     return item.frequency_str
                 if column_index == 2:
                     return item.intensity_str
                 if column_index == 3:
                     return item.lower_state_energy_str
         return None
 
-    def row(self, row_index: int) -> LinesListModel.DataType:
+    def row(self, row_index: int) -> DataType:
         return self._data[row_index]
 
     def headerData(self, col: int, orientation: Qt.Orientation, role: int = ...) -> str | None:
         if orientation == Qt.Orientation.Horizontal and role == Qt.ItemDataRole.DisplayRole:
             return self._header[col]
         return None
 
@@ -185,36 +153,38 @@
 
     def set_entries(self, new_data: list[CatalogEntryType]) -> None:
         from_mhz: Callable[[float], float] = self._settings.from_mhz
         from_log10_sq_nm_mhz: Callable[[float], float] = self._settings.from_log10_sq_nm_mhz
         from_rec_cm: Callable[[float], float] = self._settings.from_rec_cm
         frequency_suffix: int = self._settings.frequency_unit
         precision: int = [4, 7, 8, 8][frequency_suffix]
+        locale: QLocale = QLocale()
+        decimal_point: str = locale.decimalPoint()
 
         def frequency_str(frequency: float) -> tuple[str, float]:
             frequency = from_mhz(frequency)
-            return f'{frequency:.{precision}f}', frequency
+            return f'{frequency:.{precision}f}'.replace('.', decimal_point), frequency
 
         def intensity_str(intensity: float) -> tuple[str, float]:
             intensity = from_log10_sq_nm_mhz(intensity)
             if intensity == 0.0:
                 return '0', intensity
             elif abs(intensity) < 0.1:
-                return f'{intensity:.4e}', intensity
+                return f'{intensity:.4e}'.replace('.', decimal_point), intensity
             else:
-                return f'{intensity:.4f}', intensity
+                return f'{intensity:.4f}'.replace('.', decimal_point), intensity
 
         def lower_state_energy_str(lower_state_energy: float) -> tuple[str, float]:
             lower_state_energy = from_rec_cm(lower_state_energy)
             if lower_state_energy == 0.0:
                 return '0', lower_state_energy
             elif abs(lower_state_energy) < 0.1:
-                return f'{lower_state_energy:.4e}', lower_state_energy
+                return f'{lower_state_energy:.4e}'.replace('.', decimal_point), lower_state_energy
             else:
-                return f'{lower_state_energy:.4f}', lower_state_energy
+                return f'{lower_state_energy:.4f}'.replace('.', decimal_point), lower_state_energy
 
         self.beginResetModel()
         unique_entries: list[CatalogEntryType] = []
         non_unique_indices: set[int] = set()
         unique: bool
         all_unique: bool = True  # unless the opposite is proven
         for i in range(len(new_data)):
@@ -235,15 +205,15 @@
             self._entries = new_data.copy()
         else:
             self._entries = unique_entries
         entry: CatalogEntryType
         rich_text_in_formulas: bool = self._settings.rich_text_in_formulas
         self._data = list(set(
             LinesListModel.DataType(
-                entry[ID],
+                entry[SPECIES_TAG],
                 best_name(entry, rich_text_in_formulas),
                 *frequency_str(line[FREQUENCY]),
                 *intensity_str(line[INTENSITY]),
                 *lower_state_energy_str(line[LOWER_STATE_ENERGY]),
             )
             for entry in self._entries
             for line in entry[LINES]
@@ -353,32 +323,31 @@
             layout_right.addWidget(self.box_frequency, 1)
 
             self.spin_intensity.setAlignment(Qt.AlignmentFlag.AlignRight
                                              | Qt.AlignmentFlag.AlignTrailing
                                              | Qt.AlignmentFlag.AlignVCenter)
             self.spin_intensity.setButtonSymbols(QAbstractSpinBox.ButtonSymbols.NoButtons)
             self.spin_intensity.setDecimals(2)
-            self.spin_intensity.setMinimum(-math.inf)
-            self.spin_intensity.setMaximum(math.inf)
+            self.spin_intensity.setRange(-inf, inf)
             self.spin_intensity.setSingleStep(0.1)
             self.spin_intensity.setValue(-6.54)
-            self.spin_intensity.setStatusTip(self.spin_intensity.tr('Limit shown spectral lines'))
-            layout_options.addRow(layout_options.tr('Minimal Intensity:'), self.spin_intensity)
+            self.spin_intensity.setStatusTip(self.tr('Limit shown spectral lines'))
+            layout_options.addRow(self.tr('Minimal Intensity:'), self.spin_intensity)
             self.spin_temperature.setAlignment(Qt.AlignmentFlag.AlignRight
                                                | Qt.AlignmentFlag.AlignTrailing
                                                | Qt.AlignmentFlag.AlignVCenter)
             self.spin_temperature.setButtonSymbols(QAbstractSpinBox.ButtonSymbols.NoButtons)
             self.spin_temperature.setMaximum(999.99)
             self.spin_temperature.setValue(300.0)
-            self.spin_temperature.setStatusTip(self.spin_temperature.tr('Temperature to calculate intensity'))
-            self.spin_temperature.setSuffix(self.spin_temperature.tr(' K'))
-            layout_options.addRow(layout_options.tr('Temperature:'), self.spin_temperature)
+            self.spin_temperature.setStatusTip(self.tr('Temperature to calculate intensity'))
+            self.spin_temperature.setSuffix(self.tr(' K'))
+            layout_options.addRow(self.tr('Temperature:'), self.spin_temperature)
             layout_right.addLayout(layout_options, 0)
 
-            self.button_search.setText(self.button_search.tr('Show'))
+            self.button_search.setText(self.tr('Show'))
             layout_right.addWidget(self.button_search, 0)
 
             self._right_matter.setLayout(layout_right)
             self._top_matter.addWidget(self._right_matter)
             self._top_matter.setStretchFactor(0, 1)
             self._top_matter.setChildrenCollapsible(False)
 
@@ -395,32 +364,32 @@
             self.button_search.setIcon(icon('mdi6.magnify'))
 
             self.adjustSize()
 
         setup_ui()
 
         self.temperature: float = 300.0  # [K]
-        self.minimal_intensity: float = -math.inf  # [log10(nm²×MHz)]
+        self.minimal_intensity: float = -inf  # [log10(nm²×MHz)]
 
         self.button_search.setDisabled(self.catalog.is_empty)
 
         self.preferences_dialog: Preferences = Preferences(self.settings, self)
 
-        self.results_shown: bool = False
-
         self.preset_table()
 
         self.load_settings()
 
         self.results_table.customContextMenuRequested.connect(self._on_table_context_menu_requested)
         self.results_table.selectionModel().selectionChanged.connect(self._on_table_item_selection_changed)
         self.results_table.doubleClicked.connect(self._on_action_substance_info_triggered)
         self.spin_intensity.valueChanged.connect(self._on_spin_intensity_changed)
         self.spin_temperature.valueChanged.connect(self._on_spin_temperature_changed)
-        self.button_search.clicked.connect(self._on_button_search_clicked)
+        self.button_search.clicked.connect(self._on_search_requested)
+        self.box_frequency.frequencyLimitsChanged.connect(self._on_search_requested)
+        self.box_substance.selectedSubstancesChanged.connect(self._on_search_requested)
         self.menu_bar.action_load.triggered.connect(self._on_action_load_triggered)
         self.menu_bar.action_quit.triggered.connect(self._on_action_quit_triggered)
         self.menu_bar.action_check_updates.triggered.connect(self._on_action_check_updates_triggered)
         self.menu_bar.action_about_catalogs.triggered.connect(self._on_action_about_catalogs_triggered)
         self.menu_bar.action_about.triggered.connect(self._on_action_about_triggered)
         self.menu_bar.action_about_qt.triggered.connect(self._on_action_about_qt_triggered)
         self.menu_bar.action_download_catalog.triggered.connect(self._on_action_download_catalog_triggered)
@@ -482,16 +451,15 @@
     def _on_spin_temperature_changed(self, arg1: float) -> None:
         self.temperature = self.settings.to_k(arg1)
         self.fill_table()
 
     @Slot(float)
     def _on_spin_intensity_changed(self, arg1: float) -> None:
         self.minimal_intensity = self.settings.to_log10_sq_nm_mhz(arg1)
-        if self.results_shown:
-            self.fill_table()
+        self.fill_table()
 
     @Slot(QPoint)
     def _on_table_context_menu_requested(self, pos: QPoint) -> None:
         self.menu_bar.menu_edit.popup(self.results_table.viewport().mapToGlobal(pos))
 
     @Slot(QItemSelection, QItemSelection)
     def _on_table_item_selection_changed(self, _selected: QItemSelection, _deselected: QItemSelection) -> None:
@@ -524,20 +492,19 @@
                                              filters=join_file_dialog_formats(formats),
                                              basedir=directory)
         return filename, _filter
 
     @Slot()
     def _on_action_load_triggered(self) -> None:
         self.status_bar.showMessage(self.tr('Select a catalog file to load.'))
-        new_catalog_file_names: list[str]
         _formats: dict[tuple[str, ...], str] = {
-            (*all_cases('.json.gz'), *all_cases('.json.bz2'),
-             *all_cases('.json.xz'), *all_cases('.json.lzma')): self.tr('Compressed JSON', 'file type'),
-            tuple(all_cases('.json')): self.tr('JSON', 'file type'),
+            ('.json.gz', '.json.bz2', '.json.xz', '.json.lzma'): self.tr('Compressed JSON', 'file type'),
+            ('.json',): self.tr('JSON', 'file type'),
         }
+        new_catalog_file_names: list[str]
         new_catalog_file_names, _ = self.get_open_file_names(formats=_formats,
                                                              caption=self.tr('Load Catalog'),
                                                              directory=(*self.catalog.sources, '')[0])
 
         if new_catalog_file_names:
             self.status_bar.showMessage(self.tr('Loading...'))
             if self.load_catalog(*new_catalog_file_names):
@@ -570,41 +537,43 @@
         units: list[str] = [
             '',
             self.settings.frequency_unit_str,
             self.settings.intensity_unit_str,
             self.settings.energy_unit_str,
         ]
         with_units: bool = self.settings.with_units
+        csv_separator: str = self.settings.csv_separator
+        actions_checked: list[bool] = [_a.isChecked() for _a in self.menu_bar.menu_columns.actions()]
 
         def format_value(value: Any, unit: str) -> str:
             return (self.tr('{value} {unit}', 'format value in html').format(value=value, unit=unit)
                     if with_units and unit
                     else self.tr('{value}', 'format value in html').format(value=value))
 
         columns_order: list[int] = [self.results_table.horizontalHeader().logicalIndex(_c)
                                     for _c, _a in zip(range(self.results_table.horizontalHeader().count()),
-                                                      self.menu_bar.menu_columns.actions(),
+                                                      actions_checked,
                                                       strict=True)
-                                    if _a.isChecked()]
+                                    if _a]
         text: list[str] = ['<table>']
         values: list[str]
         index: QModelIndex
         for index in self.results_table.selectionModel().selectedRows():
             row: LinesListModel.DataType = self.results_model.row(index.row())
             values = [
                 format_value(_v, _u)
                 for _u, _v, _a in zip(units,
                                       (row.name, row.frequency, row.intensity, row.lower_state_energy),
-                                      self.menu_bar.menu_columns.actions(),
+                                      actions_checked,
                                       strict=True)
-                if _a.isChecked()
+                if _a
             ]
             text.append(
                 '<tr><td>' +
-                f'</td>{self.settings.csv_separator}<td>'.join(values[_c] for _c in columns_order) +
+                f'</td>{csv_separator}<td>'.join(values[_c] for _c in columns_order) +
                 '</td></tr>'
             )
         text.append('</table>')
         return self.settings.line_end.join(text)
 
     @Slot()
     def _on_action_download_catalog_triggered(self) -> None:
@@ -681,15 +650,15 @@
         self.results_table.selectAll()
 
     @Slot()
     def _on_action_substance_info_triggered(self) -> None:
         if self.results_table.selectionModel().selectedRows():
             syn: SubstanceInfo = SubstanceInfo(
                 self.catalog,
-                self.results_model.row(self.results_table.selectionModel().selectedRows()[0].row()).id,
+                self.results_model.row(self.results_table.selectionModel().selectedRows()[0].row()).species_tag,
                 inchi_key_search_url_template=self.settings.inchi_key_search_url_template,
                 parent=self)
             syn.exec()
 
     def toggle_results_table_column_visibility(self, column: int, is_visible: bool) -> None:
         if is_visible != self.results_table.isColumnHidden(column):
             return
@@ -747,20 +716,20 @@
                           self.tr("About CatSearch"),
                           "<html><p>"
                           + self.tr("CatSearch is a means of searching through spectroscopy lines catalogs. "
                                     "It's an offline application.")
                           + "</p><p>"
                           + self.tr("It relies on the data stored in JSON files.")
                           + "</p><p>"
-                          + self.tr("One can write his own catalogs as well as convert data from "
+                          + self.tr("One can write their own catalogs as well as download data from "
                                     "<a href='https://spec.jpl.nasa.gov/'>JPL</a> and "
                                     "<a href='https://astro.uni-koeln.de/'>CDMS</a> spectroscopy databases "
-                                    "freely available in the Internet or other sources.")
+                                    "available in the Internet.")
                           + "</p><p>"
-                          + self.tr("Both plain text JSON and GZip compressed JSON are supported.")
+                          + self.tr("Both plain text JSON and GZip/BZip2/LZMA-compressed JSON are supported.")
                           + "</p><p>"
                           + self.tr('See {0} for more info.')
                           .format('<a href="https://github.com/StSav012/pycatsearch/blob/master/README.md">{0}</a>')
                           .format(self.tr('readme'))
                           + "</p><br><p>"
                           + self.tr("CatSearch is licensed under the {0}.")
                           .format("<a href='https://www.gnu.org/copyleft/lesser.html'>{0}</a>"
@@ -844,15 +813,14 @@
         self.settings.setValue('horizontalSplitterState', self._central_widget.saveState())
         self.settings.endGroup()
         self.box_substance.save_settings()
         self.box_frequency.save_settings()
         self.settings.sync()
 
     def preset_table(self) -> None:
-        self.results_shown = False
         self.results_table.clearSelection()
         self.menu_bar.action_copy.setDisabled(True)
         self.menu_bar.action_substance_info.setDisabled(True)
         self.menu_bar.action_select_all.setDisabled(True)
         self.menu_bar.action_clear.setDisabled(True)
         self.menu_bar.menu_copy_only.setDisabled(True)
         self.results_model.update_units()
@@ -878,47 +846,48 @@
             self.spin_temperature.setMinimum(-273.15)
             self.spin_temperature.setValue(self.settings.from_k(self.temperature))
         else:
             raise IndexError('Wrong temperature unit index', temperature_suffix)
 
     def fill_table(self) -> None:
         self.preset_table()
+
+        if self.box_substance.isChecked() and not self.box_substance.selected_substances:
+            self.results_model.clear()
+            return
+
         self.results_table.setSortingEnabled(False)
 
         entries: list[dict[str, int | str | list[dict[str, float]]]] = \
             (sum(
                 (
                     self.catalog.filter(min_frequency=self.box_frequency.min_frequency,
                                         max_frequency=self.box_frequency.max_frequency,
                                         min_intensity=self.minimal_intensity,
-                                        anything=name,
-                                        temperature=self.temperature,
-                                        timeout=self.settings.timeout)
-                    for name in self.box_substance.selected_substances
+                                        species_tag=species_tag,
+                                        temperature=self.temperature)
+                    for species_tag in self.box_substance.selected_substances
                 ),
                 []
-            ) if self.box_substance.selected_substances and self.box_substance.isChecked()
+            ) if self.box_substance.isChecked()
              else self.catalog.filter(min_frequency=self.box_frequency.min_frequency,
                                       max_frequency=self.box_frequency.max_frequency,
                                       min_intensity=self.minimal_intensity,
-                                      temperature=self.temperature,
-                                      timeout=self.settings.timeout))
+                                      temperature=self.temperature))
         self.results_model.set_entries(entries)
 
         self.results_table.setSortingEnabled(True)
         self.menu_bar.action_select_all.setEnabled(bool(entries))
         self.menu_bar.action_clear.setEnabled(bool(entries))
         self.menu_bar.menu_copy_only.setEnabled(bool(entries))
-        self.results_shown = True
 
     @Slot()
-    def _on_button_search_clicked(self) -> None:
+    def _on_search_requested(self) -> None:
         self.status_bar.showMessage(self.tr('Searching...'))
         self.setDisabled(True)
         last_cursor: QCursor = self.cursor()
         self.setCursor(Qt.CursorShape.WaitCursor)
         self.repaint()
-        self.box_substance.update_selected_substances()
         self.fill_table()
         self.setCursor(last_cursor)
         self.setEnabled(True)
         self.status_bar.showMessage(self.tr('Ready.'))
```

### Comparing `pycatsearch-5.1.8/src/pycatsearch/gui/waiting_screen.py` & `pycatsearch-5.1.9.2/src/pycatsearch/gui/waiting_screen.py`

 * *Files identical despite different names*

### Comparing `pycatsearch-5.1.8/src/pycatsearch/utils.py` & `pycatsearch-5.1.9.2/src/pycatsearch/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # -*- coding: utf-8 -*-
 from __future__ import annotations
 
 import html
 import html.entities
 import itertools
-import math
 import os
 import sys
+from math import e as _e, inf, log10, nan, pow
 from numbers import Real
 from pathlib import Path
-from typing import Any, Callable, Final, Iterable, Iterator, Protocol, Sequence, TypeVar, cast, overload
+from typing import Any, Callable, Final, Iterable, Protocol, Sequence, TypeVar, cast, overload
 
 __all__ = ['M_LOG10E',
            'T0', 'c', 'h', 'k', 'e',
            'CATALOG', 'BUILD_TIME', 'LINES', 'FREQUENCY', 'INTENSITY', 'ID', 'STRUCTURAL_FORMULA',
            'STOICHIOMETRIC_FORMULA', 'MOLECULE', 'MOLECULE_SYMBOL', 'SPECIES_TAG', 'NAME', 'TRIVIAL_NAME', 'ISOTOPOLOG',
            'STATE', 'STATE_HTML', 'INCHI_KEY', 'DEGREES_OF_FREEDOM', 'LOWER_STATE_ENERGY', 'CONTRIBUTOR', 'VERSION',
            'DATE_OF_ENTRY', 'HUMAN_READABLE',
@@ -26,19 +26,19 @@
            'log10_sq_nm_mhz_to_log10_cm_per_molecule',
            'log10_sq_nm_mhz_to_cm_per_molecule',
            'sq_nm_mhz_to_log10_sq_nm_mhz',
            'log10_cm_per_molecule_to_log10_sq_nm_mhz',
            'cm_per_molecule_to_log10_sq_nm_mhz',
            'sort_unique', 'merge_sorted', 'search_sorted',
            'within', 'chem_html', 'best_name', 'remove_html', 'wrap_in_html',
-           'ensure_prefix', 'all_cases',
+           'ensure_prefix',
            'save_catalog_to_file',
            'ReleaseInfo', 'latest_release', 'update_with_pip']
 
-M_LOG10E: Final[float] = math.log10(math.e)
+M_LOG10E: Final[float] = log10(_e)
 
 T0: Final[float] = 300.00  # [K], see https://spec.jpl.nasa.gov/ftp/pub/catalog/doc/catdoc.pdf
 k: Final[float] = 1.380649000e-23  # [J/K],  see https://physics.nist.gov/cgi-bin/cuu/Value?k
 h: Final[float] = 6.626070150e-34  # [J/Hz], see https://physics.nist.gov/cgi-bin/cuu/Value?h
 e: Final[float] = 1.602176634e-19  # [C],    see https://physics.nist.gov/cgi-bin/cuu/Value?e
 c: Final[float] = 299_792_458.000  # [m/s],  see https://physics.nist.gov/cgi-bin/cuu/Value?c
 
@@ -305,43 +305,43 @@
 
 
 def j_to_rec_cm(energy_j: float) -> float:
     return 1e-2 / h / c * energy_j
 
 
 def log10_sq_nm_mhz_to_sq_nm_mhz(intensity_log10_sq_nm_mhz: float) -> float:
-    return math.pow(10.0, intensity_log10_sq_nm_mhz)
+    return pow(10.0, intensity_log10_sq_nm_mhz)
 
 
 def log10_sq_nm_mhz_to_log10_cm_per_molecule(intensity_log10_sq_nm_mhz: float) -> float:
-    return -10. + intensity_log10_sq_nm_mhz - math.log10(c)
+    return -10. + intensity_log10_sq_nm_mhz - log10(c)
 
 
 def log10_sq_nm_mhz_to_cm_per_molecule(intensity_log10_sq_nm_mhz: float) -> float:
-    return math.pow(10.0, log10_sq_nm_mhz_to_log10_cm_per_molecule(intensity_log10_sq_nm_mhz))
+    return pow(10.0, log10_sq_nm_mhz_to_log10_cm_per_molecule(intensity_log10_sq_nm_mhz))
 
 
 def sq_nm_mhz_to_log10_sq_nm_mhz(intensity_sq_nm_mhz: float) -> float:
     if intensity_sq_nm_mhz == 0.0:
-        return -math.inf
+        return -inf
     if intensity_sq_nm_mhz < 0.0:
-        return math.nan
-    return math.log10(intensity_sq_nm_mhz)
+        return nan
+    return log10(intensity_sq_nm_mhz)
 
 
 def log10_cm_per_molecule_to_log10_sq_nm_mhz(intensity_log10_cm_per_molecule: float) -> float:
-    return intensity_log10_cm_per_molecule + 10. + math.log10(c)
+    return intensity_log10_cm_per_molecule + 10. + log10(c)
 
 
 def cm_per_molecule_to_log10_sq_nm_mhz(intensity_cm_per_molecule: float) -> float:
     if intensity_cm_per_molecule == 0.0:
-        return -math.inf
+        return -inf
     if intensity_cm_per_molecule < 0.0:
-        return math.nan
-    return log10_cm_per_molecule_to_log10_sq_nm_mhz(math.log10(intensity_cm_per_molecule))
+        return nan
+    return log10_cm_per_molecule_to_log10_sq_nm_mhz(log10(intensity_cm_per_molecule))
 
 
 def tex_to_html_entity(s: str) -> str:
     r"""
     Change LaTeX entities syntax to HTML one.
     Get ‘\alpha’ to be ‘&alpha;’ and so on. Unknown LaTeX entities do not get replaced.
 
@@ -382,38 +382,47 @@
 
 def chem_html(formula: str) -> str:
     """ converts plain text chemical formula into html markup """
     if '<' in formula or '>' in formula:
         # we can not tell whether it's a tag or a mathematical sign
         return formula
 
+    def sub_tag(s: str) -> str:
+        return '<sub>' + s + '</sub>'
+
+    def sup_tag(s: str) -> str:
+        return '<sup>' + s + '</sup>'
+
+    def i_tag(s: str) -> str:
+        return '<i>' + s + '</i>'
+
     def subscript(s: str) -> str:
         number_start: int = -1
         number_started: bool = False
         cap_alpha_started: bool = False
         low_alpha_started: bool = False
         _i: int = 0
         while _i < len(s):
             _c: str = s[_i]
             if number_started and not _c.isdigit():
                 number_started = False
-                s = s[:number_start] + '<sub>' + s[number_start:_i] + '</sub>' + s[_i:]
-                _i += 11
+                s = s[:number_start] + sub_tag(s[number_start:_i]) + s[_i:]
+                _i += 1
             if (cap_alpha_started or low_alpha_started) and _c.isdigit() and not number_started:
                 number_start = _i
                 number_started = True
             if low_alpha_started:
                 cap_alpha_started = False
                 low_alpha_started = False
             if cap_alpha_started and _c.islower() or _c == ')':
                 low_alpha_started = True
             cap_alpha_started = _c.isupper()
             _i += 1
         if number_started:
-            s = s[:number_start] + '<sub>' + s[number_start:] + '</sub>'
+            s = s[:number_start] + sub_tag(s[number_start:])
         return s
 
     def prefix(s: str) -> str:
         no_digits: bool = False
         _i: int = len(s)
         while not no_digits:
             _i = s.rfind('-', 0, _i)
@@ -425,29 +434,29 @@
             _c: str
             unescaped_prefix: str = html.unescape(s[:_i])
             for _c in unescaped_prefix:
                 if _c.isdigit() or _c == '<':
                     no_digits = False
                     break
             if no_digits and (unescaped_prefix[0].islower() or unescaped_prefix[0] == '('):
-                return '<i>' + s[:_i] + '</i>' + s[_i:]
+                return i_tag(s[:_i]) + s[_i:]
         return s
 
     def charge(s: str) -> str:
         if s[-1] in '+-':
-            return s[:-1] + '<sup>' + s[-1] + '</sup>'
+            return s[:-1] + sup_tag(s[-1])
         return s
 
     def v(s: str) -> str:
         if '=' not in s:
             return s[0] + ' = ' + s[1:]
         ss: list[str] = list(map(str.strip, s.split('=')))
         for _i in range(len(ss)):
             if ss[_i].startswith('v'):
-                ss[_i] = ss[_i][0] + '<sub>' + ss[_i][1:] + '</sub>'
+                ss[_i] = ss[_i][0] + sub_tag(ss[_i][1:])
         return ' = '.join(ss)
 
     html_formula: str = html.escape(formula)
     html_formula_pieces: list[str] = list(map(str.strip, html_formula.split(',')))
     for i in range(len(html_formula_pieces)):
         if html_formula_pieces[i].startswith('v'):
             html_formula_pieces = html_formula_pieces[:i] + [', '.join(html_formula_pieces[i:])]
@@ -553,41 +562,14 @@
 def ensure_prefix(text: str, prefix: str) -> str:
     if text.startswith(prefix):
         return text
     else:
         return prefix + text
 
 
-def all_cases(text: str) -> Iterator[str]:
-    """ return all cases of the text given """
-
-    cases: list[str] = list({text.lower(), text.upper(), text.capitalize(), text.swapcase(), text.casefold()})
-
-    if len(cases) < 2:
-        # don't bother
-        yield from cases
-        return
-
-    length: int = len(cases[0])
-    case: str
-    if not all(len(case) == length for case in cases):
-        # don't know what to do with cases of different lengths
-        yield from cases
-        return
-    # now, all the cases are of the same length
-
-    # get all possible variants of characters at each position
-    i: int
-    variants: Iterator[list[str]] = (sorted(set(case[i] for case in cases), reverse=True) for i in range(length))
-
-    combination: tuple[str, ...]
-    for combination in itertools.product(*variants):
-        yield ''.join(combination)
-
-
 def save_catalog_to_file(filename: str | Path,
                          catalog: list[dict[str, int | str | list[dict[str, float]]]],
                          frequency_limits: tuple[float, float]) -> bool:
     from .catalog import Catalog
 
     if not catalog:
         return False
```

### Comparing `pycatsearch-5.1.8/src/pycatsearch.egg-info/PKG-INFO` & `pycatsearch-5.1.9.2/src/pycatsearch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycatsearch
-Version: 5.1.8
+Version: 5.1.9.2
 Summary: Yet another implementation of JPL and CDMS spectroscopy catalogs offline search
 Author-email: StSav012 <stsav012@gmail.com>
 License: LGPL-3.0-only
 Project-URL: Source Code, https://github.com/StSav012/pycatsearch
 Project-URL: Bug Tracker, https://github.com/StSav012/pycatsearch/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Win32 (MS Windows)
@@ -70,15 +70,15 @@
 - `entries_count` is the number of the substances loaded by `__init__`.
 - `sources` contains a list of files that have been loaded successfully by `__init__`.
 - `sources_info` returns a list of the files and the timestamps recorded there (if any).
 - `min_frequency` and `max_frequency` are the extreme values of `frequency_limits`.
 
 ###### Functions:
 
-- `__init__(self, *catalog_file_names: str)` accepts names of JSON or GZipped JSON files.
+- `__init__(self, *catalog_file_names: str)` accepts names of JSON or GZip/BZip2/LZMA-compressed JSON files.
   It loads them into memory joined.
 - `filter(self, *,
   min_frequency: float = 0.0,
   max_frequency: float = math.inf,
   min_intensity: float = -math.inf,
   max_intensity: float = math.inf,
   temperature: float = -math.inf,
@@ -90,16 +90,15 @@
   inchi: str = '',
   trivial_name: str = '',
   structural_formula: str = '',
   name: str = '',
   stoichiometric_formula: str = '',
   isotopolog: str = '',
   state: str = '',
-  degrees_of_freedom: Optional[int] = None,
-  timeout: Optional[float] = None) -> List[Dict[str, Union[int, str, List[Dict[str, float]]]]]`
+  degrees_of_freedom: Optional[int] = None) -> List[Dict[str, Union[int, str, List[Dict[str, float]]]]]`
   returns only the catalog entries that meet the criteria specified. The arguments are the following:
     - `float min_frequency`: the lower frequency \[MHz\] to take.
     - `float max_frequency`: the upper frequency \[MHz\] to take.
     - `float min_intensity`: the minimal intensity \[log10(nm²×MHz)\] to take.
     - `float max_intensity`: the maximal intensity \[log10(nm²×MHz)\] to take, use to avoid meta-stable substances.
     - `float temperature`: the temperature to calculate the line intensity at,
       use the catalog intensity if not set.
@@ -114,15 +113,14 @@
     - `str trivial_name`: a string to match the ``trivialname`` field.
     - `str structural_formula`: a string to match the ``structuralformula`` field.
     - `str name`: a string to match the ``name`` field.
     - `str stoichiometric_formula`: a string to match the ``stoichiometricformula`` field.
     - `str isotopolog`: a string to match the ``isotopolog`` field.
     - `str state`: a string to match the ``state`` or the ``state_html`` field.
     - `int degrees_of_freedom`: 0 for atoms, 2 for linear molecules, and 3 for nonlinear molecules.
-    - `float timeout`: maximum time span for the filtering to take.
 - `print(**kwargs)` prints a table of the filtered catalog entries.
   It accepts all the arguments valid for the `filter` function.
 
 ### `downloader`
 
 ###### Sample usage:
```

### Comparing `pycatsearch-5.1.8/src/pycatsearch.egg-info/SOURCES.txt` & `pycatsearch-5.1.9.2/src/pycatsearch.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 src/pycatsearch.egg-info/requires.txt
 src/pycatsearch.egg-info/top_level.txt
 src/pycatsearch/gui/__init__.py
 src/pycatsearch/gui/catalog_info.py
 src/pycatsearch/gui/download_dialog.py
 src/pycatsearch/gui/float_spinbox.py
 src/pycatsearch/gui/frequency_box.py
+src/pycatsearch/gui/html_style_delegate.py
 src/pycatsearch/gui/menu_bar.py
 src/pycatsearch/gui/preferences.py
 src/pycatsearch/gui/selectable_label.py
 src/pycatsearch/gui/settings.py
 src/pycatsearch/gui/substance_info.py
 src/pycatsearch/gui/substances_box.py
 src/pycatsearch/gui/titled_list_widget.py
```

### Comparing `pycatsearch-5.1.8/updater.py` & `pycatsearch-5.1.9.2/updater.py`

 * *Files identical despite different names*

