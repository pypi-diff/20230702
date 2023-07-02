# Comparing `tmp/pyTooling-4.0.1.tar.gz` & `tmp/pyTooling-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyTooling-4.0.1.tar", last modified: Sun Mar 26 21:03:09 2023, max compression
+gzip compressed data, was "pyTooling-5.0.0.tar", last modified: Sun Jul  2 18:22:26 2023, max compression
```

## Comparing `pyTooling-4.0.1.tar` & `pyTooling-5.0.0.tar`

### file list

```diff
@@ -1,47 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 21:03:09.593136 pyTooling-4.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    10567 2023-03-26 21:03:00.000000 pyTooling-4.0.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)    14682 2023-03-26 21:03:09.593136 pyTooling-4.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13142 2023-03-26 21:03:00.000000 pyTooling-4.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 21:03:09.589136 pyTooling-4.0.1/pyTooling/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 21:03:09.589136 pyTooling-4.0.1/pyTooling/CallByRef/
--rw-r--r--   0 runner    (1001) docker     (123)    13518 2023-03-26 21:03:00.000000 pyTooling-4.0.1/pyTooling/CallByRef/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 21:03:09.593136 pyTooling-4.0.1/pyTooling/Common/
--rw-r--r--   0 runner    (1001) docker     (123)    17366 2023-03-26 21:03:00.000000 pyTooling-4.0.1/pyTooling/Common/Platform.py
--rw-r--r--   0 runner    (1001) docker     (123)    11729 2023-03-26 21:03:00.000000 pyTooling-4.0.1/pyTooling/Common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 21:03:09.593136 pyTooling-4.0.1/pyTooling/Configuration/
--rw-r--r--   0 runner    (1001) docker     (123)    11367 2023-03-26 21:03:00.000000 pyTooling-4.0.1/pyTooling/Configuration/YAML.py
--rw-r--r--   0 runner    (1001) docker     (123)     5330 2023-03-26 21:03:00.000000 pyTooling-4.0.1/pyTooling/Configuration/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 21:03:09.593136 pyTooling-4.0.1/pyTooling/Decorators/
--rw-r--r--   0 runner    (1001) docker     (123)    10352 2023-03-26 21:03:00.000000 pyTooling-4.0.1/pyTooling/Decorators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 21:03:09.593136 pyTooling-4.0.1/pyTooling/Exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)     6520 2023-03-26 21:03:00.000000 pyTooling-4.0.1/pyTooling/Exceptions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 21:03:09.593136 pyTooling-4.0.1/pyTooling/GenericPath/
--rw-r--r--   0 runner    (1001) docker     (123)     7947 2023-03-26 21:03:00.000000 pyTooling-4.0.1/pyTooling/GenericPath/URL.py
--rw-r--r--   0 runner    (1001) docker     (123)     5575 2023-03-26 21:03:00.000000 pyTooling-4.0.1/pyTooling/GenericPath/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 21:03:09.593136 pyTooling-4.0.1/pyTooling/Graph/
--rw-r--r--   0 runner    (1001) docker     (123)    19196 2023-03-26 21:03:00.000000 pyTooling-4.0.1/pyTooling/Graph/GraphML.py
--rw-r--r--   0 runner    (1001) docker     (123)    84288 2023-03-26 21:03:00.000000 pyTooling-4.0.1/pyTooling/Graph/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 21:03:09.593136 pyTooling-4.0.1/pyTooling/Licensing/
--rw-r--r--   0 runner    (1001) docker     (123)    10291 2023-03-26 21:03:00.000000 pyTooling-4.0.1/pyTooling/Licensing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 21:03:09.593136 pyTooling-4.0.1/pyTooling/MetaClasses/
--rw-r--r--   0 runner    (1001) docker     (123)    18350 2023-03-26 21:03:00.000000 pyTooling-4.0.1/pyTooling/MetaClasses/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 21:03:09.593136 pyTooling-4.0.1/pyTooling/Packaging/
--rw-r--r--   0 runner    (1001) docker     (123)    19153 2023-03-26 21:03:00.000000 pyTooling-4.0.1/pyTooling/Packaging/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 21:03:09.593136 pyTooling-4.0.1/pyTooling/TerminalUI/
--rw-r--r--   0 runner    (1001) docker     (123)    24662 2023-03-26 21:03:00.000000 pyTooling-4.0.1/pyTooling/TerminalUI/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 21:03:09.593136 pyTooling-4.0.1/pyTooling/Timer/
--rw-r--r--   0 runner    (1001) docker     (123)     5155 2023-03-26 21:03:00.000000 pyTooling-4.0.1/pyTooling/Timer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 21:03:09.593136 pyTooling-4.0.1/pyTooling/Tree/
--rw-r--r--   0 runner    (1001) docker     (123)    33822 2023-03-26 21:03:00.000000 pyTooling-4.0.1/pyTooling/Tree/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 21:03:09.593136 pyTooling-4.0.1/pyTooling/Versioning/
--rw-r--r--   0 runner    (1001) docker     (123)    11267 2023-03-26 21:03:00.000000 pyTooling-4.0.1/pyTooling/Versioning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-26 21:03:00.000000 pyTooling-4.0.1/pyTooling/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 21:03:09.589136 pyTooling-4.0.1/pyTooling.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14682 2023-03-26 21:03:09.000000 pyTooling-4.0.1/pyTooling.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-03-26 21:03:09.000000 pyTooling-4.0.1/pyTooling.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-26 21:03:09.000000 pyTooling-4.0.1/pyTooling.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-03-26 21:03:09.000000 pyTooling-4.0.1/pyTooling.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-03-26 21:03:09.000000 pyTooling-4.0.1/pyTooling.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-03-26 21:03:00.000000 pyTooling-4.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-26 21:03:09.593136 pyTooling-4.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-03-26 21:03:00.000000 pyTooling-4.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 18:22:26.083871 pyTooling-5.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10567 2023-07-02 18:22:16.000000 pyTooling-5.0.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    15569 2023-07-02 18:22:26.083871 pyTooling-5.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14029 2023-07-02 18:22:16.000000 pyTooling-5.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 18:22:26.079871 pyTooling-5.0.0/pyTooling/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 18:22:26.079871 pyTooling-5.0.0/pyTooling/CallByRef/
+-rw-r--r--   0 runner    (1001) docker     (123)    13509 2023-07-02 18:22:16.000000 pyTooling-5.0.0/pyTooling/CallByRef/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 18:22:26.079871 pyTooling-5.0.0/pyTooling/Common/
+-rw-r--r--   0 runner    (1001) docker     (123)    12720 2023-07-02 18:22:16.000000 pyTooling-5.0.0/pyTooling/Common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 18:22:26.079871 pyTooling-5.0.0/pyTooling/Configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)    11062 2023-07-02 18:22:16.000000 pyTooling-5.0.0/pyTooling/Configuration/JSON.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11399 2023-07-02 18:22:16.000000 pyTooling-5.0.0/pyTooling/Configuration/YAML.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6470 2023-07-02 18:22:16.000000 pyTooling-5.0.0/pyTooling/Configuration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 18:22:26.079871 pyTooling-5.0.0/pyTooling/Decorators/
+-rw-r--r--   0 runner    (1001) docker     (123)    11171 2023-07-02 18:22:16.000000 pyTooling-5.0.0/pyTooling/Decorators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 18:22:26.079871 pyTooling-5.0.0/pyTooling/Exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)     6442 2023-07-02 18:22:16.000000 pyTooling-5.0.0/pyTooling/Exceptions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 18:22:26.079871 pyTooling-5.0.0/pyTooling/GenericPath/
+-rw-r--r--   0 runner    (1001) docker     (123)     7947 2023-07-02 18:22:16.000000 pyTooling-5.0.0/pyTooling/GenericPath/URL.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5575 2023-07-02 18:22:16.000000 pyTooling-5.0.0/pyTooling/GenericPath/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 18:22:26.079871 pyTooling-5.0.0/pyTooling/Graph/
+-rw-r--r--   0 runner    (1001) docker     (123)    19953 2023-07-02 18:22:16.000000 pyTooling-5.0.0/pyTooling/Graph/GraphML.py
+-rw-r--r--   0 runner    (1001) docker     (123)    89110 2023-07-02 18:22:16.000000 pyTooling-5.0.0/pyTooling/Graph/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 18:22:26.079871 pyTooling-5.0.0/pyTooling/Licensing/
+-rw-r--r--   0 runner    (1001) docker     (123)    10300 2023-07-02 18:22:16.000000 pyTooling-5.0.0/pyTooling/Licensing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 18:22:26.079871 pyTooling-5.0.0/pyTooling/MetaClasses/
+-rw-r--r--   0 runner    (1001) docker     (123)    29480 2023-07-02 18:22:16.000000 pyTooling-5.0.0/pyTooling/MetaClasses/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 18:22:26.079871 pyTooling-5.0.0/pyTooling/Packaging/
+-rw-r--r--   0 runner    (1001) docker     (123)    19150 2023-07-02 18:22:16.000000 pyTooling-5.0.0/pyTooling/Packaging/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 18:22:26.079871 pyTooling-5.0.0/pyTooling/Platform/
+-rw-r--r--   0 runner    (1001) docker     (123)    18531 2023-07-02 18:22:16.000000 pyTooling-5.0.0/pyTooling/Platform/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 18:22:26.083871 pyTooling-5.0.0/pyTooling/StateMachine/
+-rw-r--r--   0 runner    (1001) docker     (123)     5012 2023-07-02 18:22:16.000000 pyTooling-5.0.0/pyTooling/StateMachine/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 18:22:26.083871 pyTooling-5.0.0/pyTooling/TerminalUI/
+-rw-r--r--   0 runner    (1001) docker     (123)    24661 2023-07-02 18:22:16.000000 pyTooling-5.0.0/pyTooling/TerminalUI/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 18:22:26.083871 pyTooling-5.0.0/pyTooling/Timer/
+-rw-r--r--   0 runner    (1001) docker     (123)     5167 2023-07-02 18:22:16.000000 pyTooling-5.0.0/pyTooling/Timer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 18:22:26.083871 pyTooling-5.0.0/pyTooling/Tree/
+-rw-r--r--   0 runner    (1001) docker     (123)    33690 2023-07-02 18:22:16.000000 pyTooling-5.0.0/pyTooling/Tree/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 18:22:26.083871 pyTooling-5.0.0/pyTooling/Versioning/
+-rw-r--r--   0 runner    (1001) docker     (123)    12019 2023-07-02 18:22:16.000000 pyTooling-5.0.0/pyTooling/Versioning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 18:22:16.000000 pyTooling-5.0.0/pyTooling/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 18:22:26.079871 pyTooling-5.0.0/pyTooling.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15569 2023-07-02 18:22:26.000000 pyTooling-5.0.0/pyTooling.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-07-02 18:22:26.000000 pyTooling-5.0.0/pyTooling.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 18:22:26.000000 pyTooling-5.0.0/pyTooling.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-07-02 18:22:26.000000 pyTooling-5.0.0/pyTooling.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-02 18:22:26.000000 pyTooling-5.0.0/pyTooling.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-07-02 18:22:16.000000 pyTooling-5.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 18:22:26.083871 pyTooling-5.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-07-02 18:22:16.000000 pyTooling-5.0.0/setup.py
```

### Comparing `pyTooling-4.0.1/LICENSE.md` & `pyTooling-5.0.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyTooling-4.0.1/PKG-INFO` & `pyTooling-5.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyTooling
-Version: 4.0.1
+Version: 5.0.0
 Summary: pyTooling is a powerful collection of arbitrary useful classes, decorators, meta-classes and exceptions.
 Home-page: https://GitHub.com/pyTooling/pyTooling.*
 Author: Patrick Lehmann
 Author-email: Paebbels@gmail.com
 License: Apache-2.0
 Project-URL: Documentation, https://pyTooling.GitHub.io/pyTooling.*
 Project-URL: Source Code, https://GitHub.com/pyTooling/pyTooling.*
@@ -49,78 +49,85 @@
 [![Gitter](https://img.shields.io/badge/chat-on%20gitter-4db797.svg?longCache=true&style=flat-square&logo=gitter&logoColor=e8ecef)](https://gitter.im/hdl/community)
 [![Dependent repos (via libraries.io)](https://img.shields.io/librariesio/dependent-repos/pypi/pyTooling?longCache=true&style=flat-square&logo=GitHub)](https://github.com/pyTooling/pyTooling/network/dependents)
 [![Libraries.io SourceRank](https://img.shields.io/librariesio/sourcerank/pypi/pyTooling)](https://libraries.io/github/pyTooling/pyTooling/sourcerank)
 -->
 
 # pyTooling
 
-**pyTooling** is a powerful collection of arbitrary useful abstract data models, classes, decorators, meta-classes and
-exceptions. It also provides lots of helper functions e.g. to ease the handling of package descriptions.
+**pyTooling** is a powerful collection of arbitrary useful abstract data models, missing classes, decorators, a new
+performance boosting meta-class and enhanced exceptions. It also provides lots of helper functions e.g. to ease the
+handling of package descriptions or to unify multiple existing APIs into a single API.
 
-It's useful for **any** Python-base project independent if it's a library, framework or CLI tool.
+It's useful - if not even essential - for **any** Python-base project independent if it's a library, framework, CLI tool
+or just a "script".
 
 ## Introduction
 
 **pyTooling** is a basic collection of powerful helpers needed by almost any Python project. More specialized helpers
 can be found in sub-namespaces like:
 
 * [pyTooling.CLIAbstraction](https://github.com/pyTooling/pyTooling.CLIAbstraction)
-* [pyTooling.TerminalUI](https://github.com/pyTooling/pyTooling.TerminalUI)
 
-In addition, pyTooling provides a collection of CI job templates for GitHub Actions. This drastically simplifies
-GHA-based CI pipelines for Python projects.
+In addition, pyTooling provides a collection of [CI job templates for GitHub Actions](https://github.com/pyTooling/Actions).
+This drastically simplifies GHA-based CI pipelines for Python projects.
 
 ## Package Details
 
 ### Common Helper Functions
 
 This is a set of useful [helper functions](https://pytooling.github.io/pyTooling/Common/index.html#common-helperfunctions):
 
 * [getsizeof](https://pytooling.github.io/pyTooling/Common/index.html#getsizeof) calculates the "real" size of a data structure.
 * [isnestedclass](https://pytooling.github.io/pyTooling/Common/index.html#isnestedclass) checks if a class is nested inside another class.
+* [firstKey](https://pytooling.github.io/pyTooling/Common/index.html#firstkey), [firstValue](https://pytooling.github.io/pyTooling/Common/index.html#firstvalue), [firstItem](https://pytooling.github.io/pyTooling/Common/index.html#firstitem) get the first key/value/item from an ordered dictionary.
 * [mergedicts](https://pytooling.github.io/pyTooling/Common/index.html#mergedicts) merges multiple dictionaries into a new dictionary.
 * [zipdicts](https://pytooling.github.io/pyTooling/Common/index.html#zipdicts) iterate multiple dictionaries simultaneously.
 
 
 ### Common Classes
 
-* Python doesn't provide [call-by-reference parameters](https://pytooling.github.io/pyTooling/Common/CallByRef.html) for
-  simple types. This behavior can be emulated with classes provided by the `pyTooling.CallByRef` module.
-* Setuptools, PyPI, and others have a varying understanding of license names. The `pyTooling.Licensing` module
-  provides [unified license names](https://pytooling.github.io/pyTooling/Common/Licensing.html) as well as license name
-  mappings or translations.
-* Python has many ways in figuring out the current platform using APIs from `sys`, `platform`, `os`, ….
-  Unfortunately, none of the provided standard APIs offers a comprehensive answer. pyTooling provides a
-  [unified platform and environment description](https://pytooling.github.io/pyTooling/Common/Platform.html) by
-  summarizing multiple platform APIs into a single class instance.
-* While Python itself has a good versioning schema, there are no classes provided to abstract version numbers. pyTooling
-  provides such a [representations of version numbers](https://pytooling.github.io/pyTooling/Common/Versioning.html)
-  following semantic versioning (SemVer) and calendar versioning (CalVer) schemes. It's provided by the
-  `pyTooling.Versioning` module.
+* [Call-by-reference parameters](https://pytooling.github.io/pyTooling/Common/CallByRef.html): Python doesn't provide
+  *call-by-reference parameters* for simple types.  
+  This behavior can be emulated with classes provided by the `pyTooling.CallByRef` module.
+* [Unified license names](https://pytooling.github.io/pyTooling/Common/Licensing.html): Setuptools, PyPI, and others
+  have a varying understanding of license names.  
+  The `pyTooling.Licensing` module provides *unified license names* as well as license name mappings or translations.
+* [Unified platform and environment description](https://pytooling.github.io/pyTooling/Common/Platform.html): Python has
+  many ways in figuring out the current platform using APIs from `sys`, `platform`, `os`, …. Unfortunately, none of the
+  provided standard APIs offers a comprehensive answer. pyTooling provides a `CurrentPlatform` singleton summarizing
+  multiple platform APIs into a single class instance.
+* [Representations of version numbers](https://pytooling.github.io/pyTooling/Common/Versioning.html): While Python
+  itself has a good versioning schema, there are no classes provided to abstract version numbers. pyTooling provides
+  such representations following semantic versioning (SemVer) and calendar versioning (CalVer) schemes. It's provided by 
+  the `pyTooling.Versioning` module.
 
 ### Configuration
 
 Various file formats suitable for configuration information share the same features supporting: key-value pairs
 (dictionaries), sequences (lists), and simple types like string, integer and float. pyTooling provides an
 [abstract configuration file data model](https://pytooling.github.io/pyTooling/Configuration/index.html) supporting
 these features. Moreover, concrete [configuration file format reader](https://pytooling.github.io/pyTooling/Configuration/FileFormats.html)
 implementations are provided as well.
 
-* [JSON configuration reader](https://pytooling.github.io/pyTooling/Configuration/JSON.html) &rarr; To be implemented.
+* [JSON configuration reader](https://pytooling.github.io/pyTooling/Configuration/JSON.html) for the JSON file format.
 * [TOML configuration reader](https://pytooling.github.io/pyTooling/Configuration/TOML.html) &rarr; To be implemented.
 * [YAML configuration reader](https://pytooling.github.io/pyTooling/Configuration/YAML.html) for the YAML file format.
 
 
 ### Data Structures
 
-pyTooling also provides fast and powerful data structures offering object-oriented APIs:
+pyTooling also provides [fast and powerful data structures](https://pytooling.github.io/pyTooling/DataStructures/index.html)
+offering object-oriented APIs:
 
 * [Graph data structure](https://pytooling.github.io/pyTooling/DataStructures/Graph.html)  
-  &rarr; A directed graph implementation using a `Vertex` and `Edge`
-  class.
+  &rarr; A directed graph implementation using a `Vertex` and an `Edge` class.
+* [Path data structure](https://pytooling.github.io/pyTooling/DataStructures/Path/index.html)  
+  &rarr; To be documented.
+* [Finite State Machine data structure](https://pytooling.github.io/pyTooling/DataStructures/StateMachine.html)  
+  &rarr; A data model for state machines using a `State` and a `Transition` class.
 * [Tree data structure](https://pytooling.github.io/pyTooling/DataStructures/Tree.html)  
   &rarr; A fast and simple implementation using a single `Node` class.
 
 
 ### Decorators
 
 * [Abstract Methods](https://pytooling.github.io/pyTooling/MetaClasses.html#meta-abstract)
@@ -164,16 +171,16 @@
   `@abstractmethod` or `@mustoverride`.
 
 `class MyClass(metaclass=ExtendedType, singleton=True):`
   A class defined with enabled [singleton](https://pytooling.github.io/pyTooling/MetaClasses.html#singleton) behavior
   allows only a single instance of that class to exist. If another instance is going to be created, a previously cached
   instance of that class will be returned.
 
-`class MyClass(metaclass=ExtendedType, useSlots=True):`
-  A class defined with enabled [useSlots](https://pytooling.github.io/pyTooling/MetaClasses.html#slotted-type) behavior
+`class MyClass(metaclass=ExtendedType, slots=True):`
+  A class defined with enabled [slots](https://pytooling.github.io/pyTooling/MetaClasses.html#slotted-type) behavior
   stores instance fields in slots. The meta-class, translates all type-annotated fields in a class definition into
   slots. Slots allow a more efficient field storage and access compared to dynamically stored and accessed fields hosted
   by `__dict__`. This improves the memory footprint as well as the field access performance of all class instances. This
   behavior is automatically inherited to all derived classes.
 
 `class MyClass(ObjectWithSlots):`
   A class definition deriving from `ObjectWithSlots` will bring the slotted type behavior to that class and all derived
```

### Comparing `pyTooling-4.0.1/README.md` & `pyTooling-5.0.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -17,78 +17,85 @@
 [![Gitter](https://img.shields.io/badge/chat-on%20gitter-4db797.svg?longCache=true&style=flat-square&logo=gitter&logoColor=e8ecef)](https://gitter.im/hdl/community)
 [![Dependent repos (via libraries.io)](https://img.shields.io/librariesio/dependent-repos/pypi/pyTooling?longCache=true&style=flat-square&logo=GitHub)](https://github.com/pyTooling/pyTooling/network/dependents)
 [![Libraries.io SourceRank](https://img.shields.io/librariesio/sourcerank/pypi/pyTooling)](https://libraries.io/github/pyTooling/pyTooling/sourcerank)
 -->
 
 # pyTooling
 
-**pyTooling** is a powerful collection of arbitrary useful abstract data models, classes, decorators, meta-classes and
-exceptions. It also provides lots of helper functions e.g. to ease the handling of package descriptions.
+**pyTooling** is a powerful collection of arbitrary useful abstract data models, missing classes, decorators, a new
+performance boosting meta-class and enhanced exceptions. It also provides lots of helper functions e.g. to ease the
+handling of package descriptions or to unify multiple existing APIs into a single API.
 
-It's useful for **any** Python-base project independent if it's a library, framework or CLI tool.
+It's useful - if not even essential - for **any** Python-base project independent if it's a library, framework, CLI tool
+or just a "script".
 
 ## Introduction
 
 **pyTooling** is a basic collection of powerful helpers needed by almost any Python project. More specialized helpers
 can be found in sub-namespaces like:
 
 * [pyTooling.CLIAbstraction](https://github.com/pyTooling/pyTooling.CLIAbstraction)
-* [pyTooling.TerminalUI](https://github.com/pyTooling/pyTooling.TerminalUI)
 
-In addition, pyTooling provides a collection of CI job templates for GitHub Actions. This drastically simplifies
-GHA-based CI pipelines for Python projects.
+In addition, pyTooling provides a collection of [CI job templates for GitHub Actions](https://github.com/pyTooling/Actions).
+This drastically simplifies GHA-based CI pipelines for Python projects.
 
 ## Package Details
 
 ### Common Helper Functions
 
 This is a set of useful [helper functions](https://pytooling.github.io/pyTooling/Common/index.html#common-helperfunctions):
 
 * [getsizeof](https://pytooling.github.io/pyTooling/Common/index.html#getsizeof) calculates the "real" size of a data structure.
 * [isnestedclass](https://pytooling.github.io/pyTooling/Common/index.html#isnestedclass) checks if a class is nested inside another class.
+* [firstKey](https://pytooling.github.io/pyTooling/Common/index.html#firstkey), [firstValue](https://pytooling.github.io/pyTooling/Common/index.html#firstvalue), [firstItem](https://pytooling.github.io/pyTooling/Common/index.html#firstitem) get the first key/value/item from an ordered dictionary.
 * [mergedicts](https://pytooling.github.io/pyTooling/Common/index.html#mergedicts) merges multiple dictionaries into a new dictionary.
 * [zipdicts](https://pytooling.github.io/pyTooling/Common/index.html#zipdicts) iterate multiple dictionaries simultaneously.
 
 
 ### Common Classes
 
-* Python doesn't provide [call-by-reference parameters](https://pytooling.github.io/pyTooling/Common/CallByRef.html) for
-  simple types. This behavior can be emulated with classes provided by the `pyTooling.CallByRef` module.
-* Setuptools, PyPI, and others have a varying understanding of license names. The `pyTooling.Licensing` module
-  provides [unified license names](https://pytooling.github.io/pyTooling/Common/Licensing.html) as well as license name
-  mappings or translations.
-* Python has many ways in figuring out the current platform using APIs from `sys`, `platform`, `os`, ….
-  Unfortunately, none of the provided standard APIs offers a comprehensive answer. pyTooling provides a
-  [unified platform and environment description](https://pytooling.github.io/pyTooling/Common/Platform.html) by
-  summarizing multiple platform APIs into a single class instance.
-* While Python itself has a good versioning schema, there are no classes provided to abstract version numbers. pyTooling
-  provides such a [representations of version numbers](https://pytooling.github.io/pyTooling/Common/Versioning.html)
-  following semantic versioning (SemVer) and calendar versioning (CalVer) schemes. It's provided by the
-  `pyTooling.Versioning` module.
+* [Call-by-reference parameters](https://pytooling.github.io/pyTooling/Common/CallByRef.html): Python doesn't provide
+  *call-by-reference parameters* for simple types.  
+  This behavior can be emulated with classes provided by the `pyTooling.CallByRef` module.
+* [Unified license names](https://pytooling.github.io/pyTooling/Common/Licensing.html): Setuptools, PyPI, and others
+  have a varying understanding of license names.  
+  The `pyTooling.Licensing` module provides *unified license names* as well as license name mappings or translations.
+* [Unified platform and environment description](https://pytooling.github.io/pyTooling/Common/Platform.html): Python has
+  many ways in figuring out the current platform using APIs from `sys`, `platform`, `os`, …. Unfortunately, none of the
+  provided standard APIs offers a comprehensive answer. pyTooling provides a `CurrentPlatform` singleton summarizing
+  multiple platform APIs into a single class instance.
+* [Representations of version numbers](https://pytooling.github.io/pyTooling/Common/Versioning.html): While Python
+  itself has a good versioning schema, there are no classes provided to abstract version numbers. pyTooling provides
+  such representations following semantic versioning (SemVer) and calendar versioning (CalVer) schemes. It's provided by 
+  the `pyTooling.Versioning` module.
 
 ### Configuration
 
 Various file formats suitable for configuration information share the same features supporting: key-value pairs
 (dictionaries), sequences (lists), and simple types like string, integer and float. pyTooling provides an
 [abstract configuration file data model](https://pytooling.github.io/pyTooling/Configuration/index.html) supporting
 these features. Moreover, concrete [configuration file format reader](https://pytooling.github.io/pyTooling/Configuration/FileFormats.html)
 implementations are provided as well.
 
-* [JSON configuration reader](https://pytooling.github.io/pyTooling/Configuration/JSON.html) &rarr; To be implemented.
+* [JSON configuration reader](https://pytooling.github.io/pyTooling/Configuration/JSON.html) for the JSON file format.
 * [TOML configuration reader](https://pytooling.github.io/pyTooling/Configuration/TOML.html) &rarr; To be implemented.
 * [YAML configuration reader](https://pytooling.github.io/pyTooling/Configuration/YAML.html) for the YAML file format.
 
 
 ### Data Structures
 
-pyTooling also provides fast and powerful data structures offering object-oriented APIs:
+pyTooling also provides [fast and powerful data structures](https://pytooling.github.io/pyTooling/DataStructures/index.html)
+offering object-oriented APIs:
 
 * [Graph data structure](https://pytooling.github.io/pyTooling/DataStructures/Graph.html)  
-  &rarr; A directed graph implementation using a `Vertex` and `Edge`
-  class.
+  &rarr; A directed graph implementation using a `Vertex` and an `Edge` class.
+* [Path data structure](https://pytooling.github.io/pyTooling/DataStructures/Path/index.html)  
+  &rarr; To be documented.
+* [Finite State Machine data structure](https://pytooling.github.io/pyTooling/DataStructures/StateMachine.html)  
+  &rarr; A data model for state machines using a `State` and a `Transition` class.
 * [Tree data structure](https://pytooling.github.io/pyTooling/DataStructures/Tree.html)  
   &rarr; A fast and simple implementation using a single `Node` class.
 
 
 ### Decorators
 
 * [Abstract Methods](https://pytooling.github.io/pyTooling/MetaClasses.html#meta-abstract)
@@ -132,16 +139,16 @@
   `@abstractmethod` or `@mustoverride`.
 
 `class MyClass(metaclass=ExtendedType, singleton=True):`
   A class defined with enabled [singleton](https://pytooling.github.io/pyTooling/MetaClasses.html#singleton) behavior
   allows only a single instance of that class to exist. If another instance is going to be created, a previously cached
   instance of that class will be returned.
 
-`class MyClass(metaclass=ExtendedType, useSlots=True):`
-  A class defined with enabled [useSlots](https://pytooling.github.io/pyTooling/MetaClasses.html#slotted-type) behavior
+`class MyClass(metaclass=ExtendedType, slots=True):`
+  A class defined with enabled [slots](https://pytooling.github.io/pyTooling/MetaClasses.html#slotted-type) behavior
   stores instance fields in slots. The meta-class, translates all type-annotated fields in a class definition into
   slots. Slots allow a more efficient field storage and access compared to dynamically stored and accessed fields hosted
   by `__dict__`. This improves the memory footprint as well as the field access performance of all class instances. This
   behavior is automatically inherited to all derived classes.
 
 `class MyClass(ObjectWithSlots):`
   A class definition deriving from `ObjectWithSlots` will bring the slotted type behavior to that class and all derived
```

### Comparing `pyTooling-4.0.1/pyTooling/CallByRef/__init__.py` & `pyTooling-5.0.0/pyTooling/CallByRef/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,23 +38,23 @@
 from ..Decorators import export
 from ..MetaClasses import ExtendedType
 
 T = TypeVar("T")
 
 
 @export
-class CallByRefParam(Generic[T], metaclass=ExtendedType, useSlots=True):
+class CallByRefParam(Generic[T], metaclass=ExtendedType, slots=True):
 	"""
 	Implements a *call-by-reference* parameter.
 
 	.. seealso::
 
-	   * :py:class:`CallByRefBoolParam` |br|
+	   * :class:`CallByRefBoolParam` |br|
 	     |rarr| A special *call-by-reference* implementation for boolean reference types.
-	   * :py:class:`CallByRefIntParam` |br|
+	   * :class:`CallByRefIntParam` |br|
 	     |rarr| A special *call-by-reference* implementation for integer reference types.
 	"""
 
 	Value: T    #: internal value
 
 	def __init__(self, value: T = None):
 		"""Constructs a *call-by-reference* object for any type.
```

### Comparing `pyTooling-4.0.1/pyTooling/Common/Platform.py` & `pyTooling-5.0.0/pyTooling/Platform/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # ==================================================================================================================== #
-#             _____           _ _               ____                                                                   #
-#  _ __  _   |_   _|__   ___ | (_)_ __   __ _  / ___|___  _ __ ___  _ __ ___   ___  _ __                               #
-# | '_ \| | | || |/ _ \ / _ \| | | '_ \ / _` || |   / _ \| '_ ` _ \| '_ ` _ \ / _ \| '_ \                              #
-# | |_) | |_| || | (_) | (_) | | | | | | (_| || |__| (_) | | | | | | | | | | | (_) | | | |                             #
-# | .__/ \__, ||_|\___/ \___/|_|_|_| |_|\__, (_)____\___/|_| |_| |_|_| |_| |_|\___/|_| |_|                             #
+#             _____           _ _               ____  _       _    __                                                  #
+#  _ __  _   |_   _|__   ___ | (_)_ __   __ _  |  _ \| | __ _| |_ / _| ___  _ __ _ __ ___                              #
+# | '_ \| | | || |/ _ \ / _ \| | | '_ \ / _` | | |_) | |/ _` | __| |_ / _ \| '__| '_ ` _ \                             #
+# | |_) | |_| || | (_) | (_) | | | | | | (_| |_|  __/| | (_| | |_|  _| (_) | |  | | | | | |                            #
+# | .__/ \__, ||_|\___/ \___/|_|_|_| |_|\__, (_)_|   |_|\__,_|\__|_|  \___/|_|  |_| |_| |_|                            #
 # |_|    |___/                          |___/                                                                          #
 # ==================================================================================================================== #
 # Authors:                                                                                                             #
 #   Patrick Lehmann                                                                                                    #
 #                                                                                                                      #
 # License:                                                                                                             #
 # ==================================================================================================================== #
@@ -29,87 +29,121 @@
 # ==================================================================================================================== #
 #
 """
 Common platform information gathered from various sources.
 
 .. hint:: See :ref:`high-level help <COMMON/Platform>` for explanations and usage examples.
 """
-from enum import Flag, auto
+from enum                  import Flag, auto
 
-from pyTooling.Decorators import export
+from pyTooling.Decorators  import export
 from pyTooling.MetaClasses import ExtendedType
+from pyTooling.Versioning  import SemanticVersion
 
 
 @export
-class Platform(metaclass=ExtendedType, singleton=True):
+class PythonImplementation(Flag):
+	Unknown = 0
+
+	CPython = 1
+	PyPy = 2
+
+
+@export
+class PythonVersion(SemanticVersion):
+	def __init__(self):
+		from sys import version_info
+
+		super().__init__(version_info.major, version_info.minor, version_info.micro)
+
+
+@export
+class Platforms(Flag):
+	Unknown = 0
+
+	OS_BSD =     auto()        #: Operating System: BSD (Unix).
+	OS_Linux =   auto()        #: Operating System: Linux.
+	OS_MacOS =   auto()        #: Operating System: macOS.
+	OS_Windows = auto()        #: Operating System: Windows.
+
+	OperatingSystem = OS_BSD | OS_Linux | OS_MacOS | OS_Windows  #: Mask: Any operating system.
+
+	SEP_WindowsPath =  auto()  #: Seperator: Path element seperator (e.g. for directories).
+	SEP_WindowsValue = auto()  #: Seperator: Value seperator in variables (e.g. for paths in PATH).
+
+	ENV_Native = auto()        #: Environment: :term:`native`.
+	ENV_WSL =    auto()        #: Environment: :term:`Windows System for Linux <WSL>`.
+	ENV_MSYS2 =  auto()        #: Environment: :term:`MSYS2`.
+	ENV_Cygwin = auto()        #: Environment: :term:`Cygwin`.
+
+	Environment = ENV_Native | ENV_WSL | ENV_MSYS2 | ENV_Cygwin  #: Mask: Any environment.
+
+	ARCH_x86_32 =  auto()      #: Architecture: x86-32 (IA32).
+	ARCH_x86_64 =  auto()      #: Architecture: x86-64 (AMD64).
+	ARCH_AArch64 = auto()      #: Architecture: AArch64.
+
+	Arch_x86 =     ARCH_x86_32 | ARCH_x86_64  #: Mask: Any x86 architecture.
+	Arch_Arm =     ARCH_AArch64               #: Mask: Any Arm architecture.
+	Architecture = Arch_x86 | Arch_Arm        #: Mask: Any architecture.
+
+	FreeBSD = OS_BSD     | ENV_Native | ARCH_x86_64                                       #: Group: native FreeBSD on x86-64.
+	Linux =   OS_Linux   | ENV_Native | ARCH_x86_64                                       #: Group: native Linux on x86-64.
+	MacOS =   OS_MacOS   | ENV_Native | ARCH_x86_64                                       #: Group: native macOS on x86-64.
+	Windows = OS_Windows | ENV_Native | ARCH_x86_64 | SEP_WindowsPath | SEP_WindowsValue  #: Group: native Windows on x86-64.
+
+	MSYS =    auto()     #: MSYS2 Runtime: MSYS.
+	MinGW32 = auto()     #: MSYS2 Runtime: :term:`MinGW32 <MinGW>`.
+	MinGW64 = auto()     #: MSYS2 Runtime: :term:`MinGW64 <MinGW>`.
+	UCRT64 =  auto()     #: MSYS2 Runtime: :term:`UCRT64 <UCRT>`.
+	Clang32 = auto()     #: MSYS2 Runtime: Clang32.
+	Clang64 = auto()     #: MSYS2 Runtime: Clang64.
+
+	MSYS2_Runtime = MSYS | MinGW32 | MinGW64 | UCRT64 | Clang32 | Clang64    #: Mask: Any MSYS2 runtime environment.
+
+	Windows_MSYS2_MSYS =    OS_Windows | ENV_MSYS2 | ARCH_x86_64 | MSYS      #: Group: MSYS runtime running on Windows x86-64
+	Windows_MSYS2_MinGW32 = OS_Windows | ENV_MSYS2 | ARCH_x86_64 | MinGW32   #: Group: MinGW32 runtime running on Windows x86-64
+	Windows_MSYS2_MinGW64 = OS_Windows | ENV_MSYS2 | ARCH_x86_64 | MinGW64   #: Group: MinGW64 runtime running on Windows x86-64
+	Windows_MSYS2_UCRT64 =  OS_Windows | ENV_MSYS2 | ARCH_x86_64 | UCRT64    #: Group: UCRT64 runtime running on Windows x86-64
+	Windows_MSYS2_Clang32 = OS_Windows | ENV_MSYS2 | ARCH_x86_64 | Clang32   #: Group: Clang32 runtime running on Windows x86-64
+	Windows_MSYS2_Clang64 = OS_Windows | ENV_MSYS2 | ARCH_x86_64 | Clang64   #: Group: Clang64 runtime running on Windows x86-64
+
+
+@export
+class Platform(metaclass=ExtendedType, singleton=True, slots=True):
 	"""An instance of this class contains all gathered information available from various sources.
 
 	.. seealso::
 
 	   StackOverflow question: `Python: What OS am I running on? <https://stackoverflow.com/a/54837707/3719459>`__
 	"""
 
-	class Platforms(Flag):
-		Unknown = 0
-
-		OS_BSD =     auto()        #: Operating System: BSD (Unix).
-		OS_Linux =   auto()        #: Operating System: Linux.
-		OS_MacOS =   auto()        #: Operating System: macOS.
-		OS_Windows = auto()        #: Operating System: Windows.
-
-		OperatingSystem = OS_BSD | OS_Linux | OS_MacOS | OS_Windows  #: Mask: Any operating system.
-
-		SEP_WindowsPath =  auto()  #: Seperator: Path element seperator (e.g. for directories).
-		SEP_WindowsValue = auto()  #: Seperator: Value seperator in variables (e.g. for paths in PATH).
-
-		ENV_Native = auto()        #: Environment: :term:`native`.
-		ENV_WSL =    auto()        #: Environment: :term:`Windows System for Linux <WSL>`.
-		ENV_MSYS2 =  auto()        #: Environment: :term:`MSYS2`.
-		ENV_Cygwin = auto()        #: Environment: :term:`Cygwin`.
-
-		Environment = ENV_Native | ENV_WSL | ENV_MSYS2 | ENV_Cygwin  #: Mask: Any environment.
-
-		ARCH_x86_32 =  auto()      #: Architecture: x86-32 (IA32).
-		ARCH_x86_64 =  auto()      #: Architecture: x86-64 (AMD64).
-		ARCH_AArch64 = auto()      #: Architecture: AArch64.
-
-		Arch_x86 =     ARCH_x86_32 | ARCH_x86_64  #: Mask: Any x86 architecture.
-		Arch_Arm =     ARCH_AArch64               #: Mask: Any Arm architecture.
-		Architecture = Arch_x86 | Arch_Arm        #: Mask: Any architecture.
-
-		FreeBSD = OS_BSD     | ENV_Native | ARCH_x86_64                                       #: Group: native FreeBSD on x86-64.
-		Linux =   OS_Linux   | ENV_Native | ARCH_x86_64                                       #: Group: native Linux on x86-64.
-		MacOS =   OS_MacOS   | ENV_Native | ARCH_x86_64                                       #: Group: native macOS on x86-64.
-		Windows = OS_Windows | ENV_Native | ARCH_x86_64 | SEP_WindowsPath | SEP_WindowsValue  #: Group: native Windows on x86-64.
-
-		MSYS =    auto()     #: MSYS2 Runtime: MSYS.
-		MinGW32 = auto()     #: MSYS2 Runtime: :term:`MinGW32 <MinGW>`.
-		MinGW64 = auto()     #: MSYS2 Runtime: :term:`MinGW64 <MinGW>`.
-		UCRT64 =  auto()     #: MSYS2 Runtime: :term:`UCRT64 <UCRT>`.
-		Clang32 = auto()     #: MSYS2 Runtime: Clang32.
-		Clang64 = auto()     #: MSYS2 Runtime: Clang64.
-
-		MSYS2_Runtime = MSYS | MinGW32 | MinGW64 | UCRT64 | Clang32 | Clang64    #: Mask: Any MSYS2 runtime environment.
-
-		Windows_MSYS2_MSYS =    OS_Windows | ENV_MSYS2 | ARCH_x86_64 | MSYS      #: Group: MSYS runtime running on Windows x86-64
-		Windows_MSYS2_MinGW32 = OS_Windows | ENV_MSYS2 | ARCH_x86_64 | MinGW32   #: Group: MinGW32 runtime running on Windows x86-64
-		Windows_MSYS2_MinGW64 = OS_Windows | ENV_MSYS2 | ARCH_x86_64 | MinGW64   #: Group: MinGW64 runtime running on Windows x86-64
-		Windows_MSYS2_UCRT64 =  OS_Windows | ENV_MSYS2 | ARCH_x86_64 | UCRT64    #: Group: UCRT64 runtime running on Windows x86-64
-		Windows_MSYS2_Clang32 = OS_Windows | ENV_MSYS2 | ARCH_x86_64 | Clang32   #: Group: Clang32 runtime running on Windows x86-64
-		Windows_MSYS2_Clang64 = OS_Windows | ENV_MSYS2 | ARCH_x86_64 | Clang64   #: Group: Clang64 runtime running on Windows x86-64
-
-	_platform: Platforms
+	_platform:             Platforms
+	_pythonImplementation: PythonImplementation
+	_pythonVersion:        PythonVersion
 
 	def __init__(self):
 		import sys
 		import os
 		import platform
 		import sysconfig
 
-		self._platform = self.Platforms.Unknown
+		# Discover the Python implementation
+		pythonImplementation = platform.python_implementation()
+		if pythonImplementation == "CPython":
+			self._pythonImplementation = PythonImplementation.CPython
+		elif pythonImplementation == "PyPy":
+			self._pythonImplementation = PythonImplementation.PyPy
+		else:
+			self._pythonImplementation = PythonImplementation.Unknown
+
+		# Discover the Python version
+		self._pythonVersion = PythonVersion()
+
+		# Discover the platform
+		self._platform = Platforms.Unknown
 
 		# system = platform.system()
 		machine = platform.machine()
 		# architecture = platform.architecture()
 		sys_platform = sys.platform
 		sysconfig_platform = sysconfig.get_platform()
 
@@ -118,312 +152,337 @@
 		# print(system)
 		# print(machine)
 		# print(architecture)
 		# print(sys_platform)
 		# print(sysconfig_platform)
 
 		if os.name == "nt":
-			self._platform |= self.Platforms.OS_Windows
+			self._platform |= Platforms.OS_Windows
 
 			if sysconfig_platform == "win32":
-				self._platform |= self.Platforms.ENV_Native | self.Platforms.ARCH_x86_32 | self.Platforms.SEP_WindowsPath | self.Platforms.SEP_WindowsValue
+				self._platform |= Platforms.ENV_Native | Platforms.ARCH_x86_32 | Platforms.SEP_WindowsPath | Platforms.SEP_WindowsValue
 			elif sysconfig_platform == "win-amd64":
-				self._platform |= self.Platforms.ENV_Native | self.Platforms.ARCH_x86_64 | self.Platforms.SEP_WindowsPath | self.Platforms.SEP_WindowsValue
+				self._platform |= Platforms.ENV_Native | Platforms.ARCH_x86_64 | Platforms.SEP_WindowsPath | Platforms.SEP_WindowsValue
 			elif sysconfig_platform.startswith("mingw"):
 				if machine == "AMD64":
-					self._platform |= self.Platforms.ARCH_x86_64
+					self._platform |= Platforms.ARCH_x86_64
 				else:
 					raise Exception(f"Unknown architecture '{machine}' for Windows.")
 
 				if sysconfig_platform == "mingw_i686":
-					self._platform |= self.Platforms.ENV_MSYS2 | self.Platforms.MinGW32
+					self._platform |= Platforms.ENV_MSYS2 | Platforms.MinGW32
 				elif sysconfig_platform == "mingw_x86_64":
-					self._platform |= self.Platforms.ENV_MSYS2 | self.Platforms.MinGW64
+					self._platform |= Platforms.ENV_MSYS2 | Platforms.MinGW64
 				elif sysconfig_platform == "mingw_x86_64_ucrt":
-					self._platform |= self.Platforms.ENV_MSYS2 | self.Platforms.UCRT64
+					self._platform |= Platforms.ENV_MSYS2 | Platforms.UCRT64
 				elif sysconfig_platform == "mingw_x86_64_clang":
-					self._platform |= self.Platforms.ENV_MSYS2 | self.Platforms.Clang64
+					self._platform |= Platforms.ENV_MSYS2 | Platforms.Clang64
 				else:
 					raise Exception(f"Unknown MSYS2 architecture '{sysconfig_platform}'.")
 			else:
 				raise Exception(f"Unknown platform '{sysconfig_platform}' running on Windows.")
 
 		elif os.name == "posix":
 			if sys_platform == "linux":
-				self._platform |= self.Platforms.OS_Linux | self.Platforms.ENV_Native
+				self._platform |= Platforms.OS_Linux | Platforms.ENV_Native
 
 				if sysconfig_platform == "linux-x86_64":            # native Linux x86_64; Windows 64 + WSL
-					self._platform |= self.Platforms.ARCH_x86_64
+					self._platform |= Platforms.ARCH_x86_64
 				elif sysconfig_platform == "linux-aarch64":         # native Linux Aarch64
-					self._platform |= self.Platforms.ARCH_AArch64
+					self._platform |= Platforms.ARCH_AArch64
 				else:
 					raise Exception(f"Unknown architecture '{sysconfig_platform}' for a native Linux.")
 
 			elif sys_platform == "darwin":
-				self._platform |= self.Platforms.OS_MacOS | self.Platforms.ENV_Native | self.Platforms.ARCH_x86_64
+				self._platform |= Platforms.OS_MacOS | Platforms.ENV_Native | Platforms.ARCH_x86_64
 
 				# print()
 				# print(os.name)
 				# print(system)
 				# print(machine)
 				# print(architecture)
 				# print(sys_platform)
 				# print(sysconfig_platform)
 			elif sys_platform == "msys":
-				self._platform |= self.Platforms.OS_Windows | self.Platforms.ENV_MSYS2 | self.Platforms.MSYS
+				self._platform |= Platforms.OS_Windows | Platforms.ENV_MSYS2 | Platforms.MSYS
 
 				if machine == "i686":
-					self._platform |= self.Platforms.ARCH_x86_32
+					self._platform |= Platforms.ARCH_x86_32
 				elif machine == "x86_64":
-					self._platform |= self.Platforms.ARCH_x86_64
+					self._platform |= Platforms.ARCH_x86_64
 				else:
 					raise Exception(f"Unknown architecture '{machine}' for MSYS2-MSYS on Windows.")
 
 			elif sys_platform == "cygwin":
-				self._platform |= self.Platforms.OS_Windows
+				self._platform |= Platforms.OS_Windows
 
 				if sysconfig_platform.startswith("msys"):
-					self._platform |= self.Platforms.ENV_MSYS2 | self.Platforms.MSYS
+					self._platform |= Platforms.ENV_MSYS2 | Platforms.MSYS
 
 					if machine == "i686":
-						self._platform |= self.Platforms.ARCH_x86_32
+						self._platform |= Platforms.ARCH_x86_32
 					elif machine == "x86_64":
-						self._platform |= self.Platforms.ARCH_x86_64
+						self._platform |= Platforms.ARCH_x86_64
 					else:
 						raise Exception(f"Unknown architecture '{machine}' for MSYS2 on Windows.")
 
 				elif sysconfig_platform.startswith("mingw64"):
-					self._platform |= self.Platforms.ENV_MSYS2 | self.Platforms.MinGW64 | self.Platforms.ARCH_x86_64
+					self._platform |= Platforms.ENV_MSYS2 | Platforms.MinGW64 | Platforms.ARCH_x86_64
 				else:
 					raise Exception(f"Unknown architecture '{machine}' for Cygwin on Windows.")
 
 			elif sys_platform.startswith("freebsd"):
 				if machine == "amd64":
-					self._platform = self.Platforms.FreeBSD
+					self._platform = Platforms.FreeBSD
 				else:
 					raise Exception(f"Unknown architecture '{machine}' for FreeBSD.")
 			else:
 				raise Exception(f"Unknown POSIX platform '{sys_platform}'.")
 		else:
 			raise Exception(f"Unknown operating system '{os.name}'.")
 
 		# print(self._platform)
 
+
+	@property
+	def PythonImplementation(self) -> PythonImplementation:
+		return self._pythonImplementation
+
+	@property
+	def IsCPython(self) -> bool:
+		"""Returns true, if the Python implementation is a :term:`CPython`.
+
+		:returns: ``True``, if the Python implementation is CPython.
+		"""
+		return self._pythonImplementation is PythonImplementation.CPython
+
+	@property
+	def IsPyPy(self) -> bool:
+		"""Returns true, if the Python implementation is a :term:`PyPy`.
+
+		:returns: ``True``, if the Python implementation is PyPY.
+		"""
+		return self._pythonImplementation is PythonImplementation.PyPy
+
+	@property
+	def PythonVersion(self) -> PythonVersion:
+		return self._pythonVersion
+
 	@property
 	def HostOperatingSystem(self) -> Platforms:
-		return self._platform & self.Platforms.OperatingSystem
+		return self._platform & Platforms.OperatingSystem
 
 	@property
 	def IsNativePlatform(self) -> bool:
 		"""Returns true, if the platform is a :term:`native` platform.
 
 		:returns: ``True``, if the platform is a native platform.
 		"""
-		return self.Platforms.ENV_Native in self._platform
+		return Platforms.ENV_Native in self._platform
 
 	@property
 	def IsNativeWindows(self) -> bool:
 		"""Returns true, if the platform is a :term:`native` Windows x86-64 platform.
 
 		:returns: ``True``, if the platform is a native Windows x86-64 platform.
 		"""
-		return self.Platforms.Windows in self._platform
+		return Platforms.Windows in self._platform
 
 	@property
 	def IsNativeLinux(self) -> bool:
 		"""Returns true, if the platform is a :term:`native` Linux x86-64 platform.
 
 		:returns: ``True``, if the platform is a native Linux x86-64 platform.
 		"""
-		return self.Platforms.Linux in self._platform
+		return Platforms.Linux in self._platform
 
 	@property
 	def IsNativeMacOS(self) -> bool:
 		"""Returns true, if the platform is a :term:`native` macOS x86-64 platform.
 
 		:returns: ``True``, if the platform is a native macOS x86-64 platform.
 		"""
-		return self.Platforms.MacOS in self._platform
+		return Platforms.MacOS in self._platform
 
 	@property
 	def IsMSYS2Environment(self) -> bool:
 		"""Returns true, if the platform is a :term:`MSYS2` environment on Windows.
 
 		:returns: ``True``, if the platform is a MSYS2 environment on Windows.
 		"""
-		return self.Platforms.ENV_MSYS2 in self._platform
+		return Platforms.ENV_MSYS2 in self._platform
 
 	@property
 	def IsMSYSOnWindows(self) -> bool:
 		"""Returns true, if the platform is a MSYS runtime on Windows.
 
 		:returns: ``True``, if the platform is a MSYS runtime on Windows.
 		"""
-		return self.Platforms.Windows_MSYS2_MSYS in self._platform
+		return Platforms.Windows_MSYS2_MSYS in self._platform
 
 	@property
 	def IsMinGW32OnWindows(self) -> bool:
 		"""Returns true, if the platform is a :term:`MinGW32 <MinGW>` runtime on Windows.
 
 		:returns: ``True``, if the platform is a MINGW32 runtime on Windows.
 		"""
-		return self.Platforms.Windows_MSYS2_MinGW32 in self._platform
+		return Platforms.Windows_MSYS2_MinGW32 in self._platform
 
 	@property
 	def IsMinGW64OnWindows(self) -> bool:
 		"""Returns true, if the platform is a :term:`MinGW64 <MinGW>` runtime on Windows.
 
 		:returns: ``True``, if the platform is a MINGW64 runtime on Windows.
 		"""
-		return self.Platforms.Windows_MSYS2_MinGW64 in self._platform
+		return Platforms.Windows_MSYS2_MinGW64 in self._platform
 
 	@property
 	def IsUCRT64OnWindows(self) -> bool:
 		"""Returns true, if the platform is a :term:`UCRT64 <UCRT>` runtime on Windows.
 
 		:returns: ``True``, if the platform is a UCRT64 runtime on Windows.
 		"""
-		return self.Platforms.Windows_MSYS2_UCRT64 in self._platform
+		return Platforms.Windows_MSYS2_UCRT64 in self._platform
 
 	@property
 	def IsClang32OnWindows(self) -> bool:
 		"""Returns true, if the platform is a Clang32 runtime on Windows.
 
 		:returns: ``True``, if the platform is a Clang32 runtime on Windows.
 		"""
-		return self.Platforms.Windows_MSYS2_Clang32 in self._platform
+		return Platforms.Windows_MSYS2_Clang32 in self._platform
 
 	@property
 	def IsClang64OnWindows(self) -> bool:
 		"""Returns true, if the platform is a Clang64 runtime on Windows.
 
 		:returns: ``True``, if the platform is a Clang64 runtime on Windows.
 		"""
-		return self.Platforms.Windows_MSYS2_Clang64 in self._platform
+		return Platforms.Windows_MSYS2_Clang64 in self._platform
 
 	@property
 	def IsPOSIX(self) -> bool:
 		"""
 		Returns true, if the platform is POSIX or POSIX-like.
 
 		:returns: ``True``, if POSIX or POSIX-like.
 		"""
-		return self.Platforms.SEP_WindowsPath not in self._platform
+		return Platforms.SEP_WindowsPath not in self._platform
 
 	@property
 	def PathSeperator(self) -> str:
 		"""
 		Returns the path element separation character (e.g. for directories).
 
 		* POSIX-like: ``/``
 		* Windows: ``\\``
 
 		:returns: Path separation character.
 		"""
-		if self.Platforms.SEP_WindowsPath in self._platform:
+		if Platforms.SEP_WindowsPath in self._platform:
 			return "\\"
 		else:
 			return "/"
 
 	@property
 	def ValueSeperator(self) -> str:
 		"""
 		Returns the value separation character (e.g. for paths in PATH).
 
 		* POSIX-like: ``:``
 		* Windows: ``;``
 
 		:returns: Value separation character.
 		"""
-		if self.Platforms.SEP_WindowsValue in self._platform:
+		if Platforms.SEP_WindowsValue in self._platform:
 			return ";"
 		else:
 			return ":"
 
 	@property
 	def ExecutableExtension(self) -> str:
 		"""
 		Returns the file extension for an executable.
 
 		* Linux: ``""`` (empty string)
 		* macOS: ``""`` (empty string)
 		* Windows: ``"exe"``
 		"""
-		if self.Platforms.OS_Windows in self._platform:
+		if Platforms.OS_Windows in self._platform:
 			return "exe"
-		elif self.Platforms.OS_Linux in self._platform:
+		elif Platforms.OS_Linux in self._platform:
 			return ""
-		elif self.Platforms.OS_MacOS in self._platform:
+		elif Platforms.OS_MacOS in self._platform:
 			return ""
 		else:
 			raise Exception(f"Unknown operating system.")
 
 	@property
 	def SharedLibraryExtension(self) -> str:
 		"""
 		Returns the file extension for a shared library.
 
 		* Linux: ``"so"``
 		* macOS: ``"lib"``
 		* Windows: ``"dll"``
 		"""
-		if self.Platforms.OS_Windows in self._platform:
+		if Platforms.OS_Windows in self._platform:
 			return "dll"
-		elif self.Platforms.OS_Linux in self._platform:
+		elif Platforms.OS_Linux in self._platform:
 			return "so"
-		elif self.Platforms.OS_MacOS in self._platform:
+		elif Platforms.OS_MacOS in self._platform:
 			return "lib"
 		else:
 			raise Exception(f"Unknown operating system.")
 
 	def __repr__(self) -> str:
 		return str(self._platform)
 
 	def __str__(self) -> str:
 		runtime = ""
 
-		if self.Platforms.OS_MacOS in self._platform:
+		if Platforms.OS_MacOS in self._platform:
 			platform = "MacOS"
-		elif self.Platforms.OS_Linux in self._platform:
+		elif Platforms.OS_Linux in self._platform:
 			platform = "Linux"
-		elif self.Platforms.OS_Windows in self._platform:
+		elif Platforms.OS_Windows in self._platform:
 			platform = "Windows"
 		else:
 			platform = "plat:dec-err"
 
-		if self.Platforms.ENV_Native in self._platform:
+		if Platforms.ENV_Native in self._platform:
 			environment = ""
-		elif self.Platforms.ENV_WSL in self._platform:
+		elif Platforms.ENV_WSL in self._platform:
 			environment = "+WSL"
-		elif self.Platforms.ENV_MSYS2 in self._platform:
+		elif Platforms.ENV_MSYS2 in self._platform:
 			environment = "+MSYS2"
 
-			if self.Platforms.MSYS in self._platform:
+			if Platforms.MSYS in self._platform:
 				runtime = " - MSYS"
-			elif self.Platforms.MinGW32 in self._platform:
+			elif Platforms.MinGW32 in self._platform:
 				runtime = " - MinGW32"
-			elif self.Platforms.MinGW64 in self._platform:
+			elif Platforms.MinGW64 in self._platform:
 				runtime = " - MinGW64"
-			elif self.Platforms.UCRT64 in self._platform:
+			elif Platforms.UCRT64 in self._platform:
 				runtime = " - UCRT64"
-			elif self.Platforms.Clang32 in self._platform:
+			elif Platforms.Clang32 in self._platform:
 				runtime = " - Clang32"
-			elif self.Platforms.Clang64 in self._platform:
+			elif Platforms.Clang64 in self._platform:
 				runtime = " - Clang64"
 			else:
 				runtime = "rt:dec-err"
 
-		elif self.Platforms.ENV_Cygwin in self._platform:
+		elif Platforms.ENV_Cygwin in self._platform:
 			environment = "+Cygwin"
 		else:
 			environment = "env:dec-err"
 
-		if self.Platforms.ARCH_x86_32 in self._platform:
+		if Platforms.ARCH_x86_32 in self._platform:
 			architecture = "x86-32"
-		elif self.Platforms.ARCH_x86_64 in self._platform:
+		elif Platforms.ARCH_x86_64 in self._platform:
 			architecture = "x86-64"
-		elif self.Platforms.ARCH_AArch64 in self._platform:
+		elif Platforms.ARCH_AArch64 in self._platform:
 			architecture = "amd64"
 		else:
 			architecture = "arch:dec-err"
 
 		return f"{platform}{environment} ({architecture}){runtime}"
```

### Comparing `pyTooling-4.0.1/pyTooling/Common/__init__.py` & `pyTooling-5.0.0/pyTooling/Common/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,40 +31,39 @@
 """
 Common types, helper functions and classes.
 
 .. hint:: See :ref:`high-level help <COMMON>` for explanations and usage examples.
 """
 __author__ =    "Patrick Lehmann"
 __email__ =     "Paebbels@gmail.com"
-__copyright__ = "2017-2022, Patrick Lehmann"
+__copyright__ = "2017-2023, Patrick Lehmann"
 __license__ =   "Apache License, Version 2.0"
-__version__ =   "4.0.1"
+__version__ =   "5.0.0"
 __keywords__ =  ["decorators", "meta-classes", "exceptions", "platform", "versioning", "licensing", "overloading",
 								"singleton", "tree", "graph", "timer", "data structure", "setuptools", "wheel", "installation",
 								"packaging", "path", "generic path", "generic library", "url", "terminal", "shell", "TUI", "console",
 								"text user interface", "message logging", "abstract", "override"]
 
 from collections import deque
-from functools import reduce
-from numbers import Number
-from operator import or_
-from typing import Type, Any, Callable, Dict, Generator, Tuple, TypeVar, overload, Union, Mapping, Set
+from numbers     import Number
+from typing      import Type, Any, Callable, Dict, Generator, Tuple, TypeVar, overload, Union, Mapping, Set, Hashable, Optional
 
 try:
 	from pyTooling.Decorators import export
+	from pyTooling.Platform   import Platform
 except ModuleNotFoundError:  # pragma: no cover
 	print("[pyTooling.Packaging] Could not import from 'pyTooling.*'!")
 
 	try:
 		from Decorators import export
+		from Platform   import Platform
 	except ModuleNotFoundError as ex:  # pragma: no cover
 		print("[pyTooling.Packaging] Could not import from 'Decorators' or 'Licensing' directly!")
 		raise ex
 
-from pyTooling.Common.Platform import Platform
 
 __all__ = ["CurrentPlatform"]
 
 CurrentPlatform = Platform()     #: Gathered information for the current platform.
 
 
 @export
@@ -92,15 +91,15 @@
 	Recursively calculate the "true" size of an object including complex members like ``__dict__``.
 
 	:param obj: Object to calculate the size of.
 	:returns:   True size of an object in bytes.
 
 	.. admonition:: Background Information
 
-	   The function :py:func:`sys.getsizeof` only returns the raw size of a Python object and doesn't account for the
+	   The function :func:`sys.getsizeof` only returns the raw size of a Python object and doesn't account for the
 	   overhead of e.g. ``_dict__`` to store dynamically allocated object members.
 
 	.. seealso::
 
 	   The code is based on code snippets and ideas from:
 
 	   * `Compute Memory Footprint of an Object and its Contents <https://code.activestate.com/recipes/577504/>`__ (MIT Lizense)
@@ -168,105 +167,125 @@
 def firstKey(d: Dict[_DictKey1, _DictValue1]) -> _DictKey1:
 	"""
 	Retrieves the first key from a dictionary's keys.
 
 	:param d: Dictionary to get the first key from.
 	:returns: The first key.
 	"""
+	if len(d) == 0:
+		raise ValueError(f"Dictionary is empty.")
+
 	return next(iter(d.keys()))
 
 
 @export
 def firstValue(d: Dict[_DictKey1, _DictValue1]) -> _DictValue1:
 	"""
 	Retrieves the first value from a dictionary's values.
 
 	:param d: Dictionary to get the first value from.
 	:returns: The first value.
 	"""
+	if len(d) == 0:
+		raise ValueError(f"Dictionary is empty.")
+
 	return next(iter(d.values()))
 
 
 @export
 def firstItem(d: Dict[_DictKey1, _DictValue1]) -> Tuple[_DictKey1, _DictValue1]:
 	"""
 	Retrieves the first key-value-pair from a dictionary.
 
 	:param d: Dictionary to get the first key-value-pair from.
 	:returns: The first key-value-pair as tuple.
 	"""
+	if len(d) == 0:
+		raise ValueError(f"Dictionary is empty.")
+
 	return next(iter(d.items()))
 
 
 @overload
 def mergedicts(
 	m1: Mapping[_DictKey1, _DictValue1],
-	func: Callable
-) -> Generator[Tuple[Union[_DictKey1], Union[_DictValue1]], None, None]:
-	...
+	filter: Optional[Callable[[Hashable, Any], bool]]
+) -> Dict[Union[_DictKey1], Union[_DictValue1]]:
+#) -> Generator[Tuple[Union[_DictKey1], Union[_DictValue1]], None, None]:
+	...  # pragma: no cover
 
 
 @overload
 def mergedicts(
 	m1: Mapping[_DictKey1, _DictValue1],
 	m2: Mapping[_DictKey2, _DictValue2],
-	func: Callable
-) -> Generator[Tuple[Union[_DictKey1, _DictKey2], Union[_DictValue1, _DictValue2]], None, None]:
-	...
+	filter: Optional[Callable[[Hashable, Any], bool]]
+) -> Dict[Union[_DictKey1, _DictKey2], Union[_DictValue1, _DictValue2]]:
+# ) -> Generator[Tuple[Union[_DictKey1, _DictKey2], Union[_DictValue1, _DictValue2]], None, None]:
+	...  # pragma: no cover
 
 
 @overload
 def mergedicts(
 	m1: Mapping[_DictKey1, _DictValue1],
 	m2: Mapping[_DictKey2, _DictValue2],
 	m3: Mapping[_DictKey3, _DictValue3],
-	func: Callable
-) -> Generator[Tuple[Union[_DictKey1, _DictKey2, _DictKey3], Union[_DictValue1, _DictValue2, _DictValue3]], None, None]:
-	...
+	filter: Optional[Callable[[Hashable, Any], bool]]
+) -> Dict[Union[_DictKey1, _DictKey2, _DictKey3], Union[_DictValue1, _DictValue2, _DictValue3]]:
+#) -> Generator[Tuple[Union[_DictKey1, _DictKey2, _DictKey3], Union[_DictValue1, _DictValue2, _DictValue3]], None, None]:
+	...  # pragma: no cover
 
 
 @export
-def mergedicts(*dicts: Tuple[Dict, ...], func: Callable = None) -> Dict:
+def mergedicts(*dicts: Tuple[Dict, ...], filter: Callable[[Hashable, Any], bool] = None) -> Dict:
 	"""
 	Merge multiple dictionaries into a single new dictionary.
 
-	If parameter ``func`` isn't ``None``, then this function is applied to every element during the merge operation.
+	If parameter ``filter`` isn't ``None``, then this function is applied to every element during the merge operation. If
+	it returns true, the dictionary element will be present in the resulting dictionary.
+
+	:param dicts:  Tuple of dictionaries to merge as positional parameters.
+	:param filter: Optional filter function to apply to each dictionary element when merging.
+	:returns:      A new dictionary containing the merge result.
 
-	:param dicts: Tuple of dictionaries to merge as positional parameters.
-	:param func:  Optional function to apply to each dictionary element when merging.
-	:returns:     A new dictionary containing the merge result.
+	.. seealso::
+
+	   `How do I merge two dictionaries in a single expression in Python? <https://stackoverflow.com/questions/38987/how-do-i-merge-two-dictionaries-in-a-single-expression-in-python>`__
 	"""
-	if func is None:
-		return {k: reduce(lambda d,x: x.get(k, d), dicts, None) for k in reduce(or_, map(lambda x: x.keys(), dicts), set()) }
+	if len(dicts) == 0:
+		raise ValueError(f"Called 'mergedicts' without any dictionary parameter.")
+
+	if filter is None:
+		return {k: v for d in dicts for k, v in d.items()}
 	else:
-		return {k: reduce(lambda x: func(*x) if (len(x) > 1) else x[0])([d[k] for d in dicts if k in d]) for k in reduce(or_, map(lambda x: x.keys(), dicts), set())}
+		return {k: v for d in dicts for k, v in d.items() if filter(k, v)}
 
 
 @overload
 def zipdicts(
 	m1: Mapping[_DictKey, _DictValue1]
 ) -> Generator[Tuple[_DictKey, _DictValue1], None, None]:
-	...
+	...  # pragma: no cover
 
 
 @overload
 def zipdicts(
 	m1: Mapping[_DictKey, _DictValue1],
 	m2: Mapping[_DictKey, _DictValue2]
 ) -> Generator[Tuple[_DictKey, _DictValue1, _DictValue2], None, None]:
-	...
+	...  # pragma: no cover
 
 
 @overload
 def zipdicts(
 	m1: Mapping[_DictKey, _DictValue1],
 	m2: Mapping[_DictKey, _DictValue2],
 	m3: Mapping[_DictKey, _DictValue3]
 ) -> Generator[Tuple[_DictKey, _DictValue1, _DictValue2, _DictValue3], None, None]:
-	...
+	...  # pragma: no cover
 
 
 @export
 def zipdicts(*dicts: Tuple[Dict, ...]) -> Generator[Tuple, None, None]:
 	"""
 	Iterate multiple dictionaries simultaneously.
 
@@ -276,17 +295,20 @@
 
 	.. seealso::
 
 	   The code is based on code snippets and ideas from:
 
 	   * `zipping together Python dicts <https://github.com/mCodingLLC/VideosSampleCode/tree/master/videos/101_zip_dict>`__ (MIT Lizense)
 	"""
-	if not dicts:
+	if len(dicts) == 0:
 		raise ValueError(f"Called 'zipdicts' without any dictionary parameter.")
 
 	length = len(dicts[0])
 	if any(len(d) != length for d in dicts):
 		raise ValueError(f"All given dictionaries must have the same length.")
 
-	for key, item0 in dicts[0].items():
-		# WORKAROUND: using redundant parenthesis for Python 3.7
-		yield (key, item0, *(d[key] for d in dicts[1:]))
+	def gen(ds: Tuple[Dict, ...]) -> Generator[Tuple, None, None]:
+		for key, item0 in ds[0].items():
+			# WORKAROUND: using redundant parenthesis for Python 3.7
+			yield (key, item0, *(d[key] for d in ds[1:]))
+
+	return gen(dicts)
```

### Comparing `pyTooling-4.0.1/pyTooling/Configuration/YAML.py` & `pyTooling-5.0.0/pyTooling/Configuration/YAML.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,18 +29,18 @@
 # ==================================================================================================================== #
 #
 """
 Configuration reader for YAML files.
 
 .. hint:: See :ref:`high-level help <CONFIG/FileFormat/YAML>` for explanations and usage examples.
 """
-from pathlib import Path
-from typing import Dict, List, Union, Iterator as typing_Iterator
+from pathlib       import Path
+from typing        import Dict, List, Union, Iterator as typing_Iterator
 
-from ..Decorators import export
+from ..Decorators  import export
 from ..MetaClasses import ExtendedType
 
 try:
 	from ruamel.yaml import YAML, CommentedMap, CommentedSeq
 except ImportError as ex:  # pragma: no cover
 	raise Exception(f"Optional dependency 'ruamel.yaml' not installed. Either install pyTooling with extra dependencies 'pyTooling[yaml]' or install 'ruamel.yaml' directly.") from ex
 
@@ -52,20 +52,21 @@
 	KeyT, NodeT, ValueT
 )
 
 
 @export
 class Node(Abstract_Node):
 	_yamlNode: Union[CommentedMap, CommentedSeq]
-	_cache: Dict[str, ValueT]
-	_key: KeyT
-	_length: int
+	_cache:    Dict[str, ValueT]
+	_key:      KeyT
+	_length:   int
 
 	def __init__(self, root: "Configuration", parent: NodeT, key: KeyT, yamlNode: Union[CommentedMap, CommentedSeq]):
-		super().__init__(root, parent)
+		Abstract_Node.__init__(self, root, parent)
+
 		self._yamlNode = yamlNode
 		self._cache = {}
 		self._key = key
 		self._length = len(yamlNode)
 
 	def __len__(self) -> int:
 		"""
@@ -184,72 +185,74 @@
 			else:
 				node = node._GetNodeOrValue(p)
 
 		return node
 
 
 @export
-class Dictionary(Abstract_Dict, Node):
+class Dictionary(Node, Abstract_Dict):
 	"""A dictionary node in a YAML data file."""
 
 	_keys: List[KeyT]
 
 	def __init__(self, root: "Configuration", parent: NodeT, key: KeyT, yamlNode: CommentedMap):
 		Node.__init__(self, root, parent, key, yamlNode)
+
 		self._keys = [str(k) for k in yamlNode.keys()]
 
 	def __contains__(self, key: KeyT) -> bool:
 		return key in self._keys
 
 	def __iter__(self) -> typing_Iterator[ValueT]:
-		class Iterator(metaclass=ExtendedType, useSlots=True):
+		class Iterator(metaclass=ExtendedType, slots=True):
 			_iter: typing_Iterator
 			_obj: Dictionary
 
 			def __init__(self, obj: Dictionary):
 				self._iter = iter(obj._keys)
 				self._obj = obj
 
 			def __iter__(self) -> "Iterator":
 				"""
 				Return itself to fulfil the iterator protocol.
 
 				:returns: Itself.
 				"""
-				return self
+				return self  # pragma: no cover
 
 			def __next__(self) -> ValueT:
 				"""
 				Returns the next item in the dictionary.
 
 				:returns: Next item.
 				"""
 				key = next(self._iter)
 				return self._obj[key]
 
 		return Iterator(self)
 
 
 @export
-class Sequence(Abstract_Seq, Node):
+class Sequence(Node, Abstract_Seq):
 	"""A sequence node (ordered list) in a YAML data file."""
 
 	def __init__(self, root: "Configuration", parent: NodeT, key: KeyT, yamlNode: CommentedSeq):
 		Node.__init__(self, root, parent, key, yamlNode)
+
 		self._length = len(yamlNode)
 
 	__getitem__ = Node.__getitem__
 
 	def __iter__(self) -> typing_Iterator[ValueT]:
 		"""
 		Returns an iterator to iterate items in the sequence of sub-nodes.
 
 		:returns: Iterator to iterate items in a sequence.
 		"""
-		class Iterator(metaclass=ExtendedType, useSlots=True):
+		class Iterator(metaclass=ExtendedType, slots=True):
 			"""Iterator to iterate sequence items."""
 
 			_i: int         #: internal iterator position
 			_obj: Sequence  #: Sequence object to iterate
 
 			def __init__(self, obj: Sequence):
 				self._i = 0
@@ -257,15 +260,15 @@
 
 			def __iter__(self) -> "Iterator":
 				"""
 				Return itself to fulfil the iterator protocol.
 
 				:returns: Itself.
 				"""
-				return self
+				return self  # pragma: no cover
 
 			def __next__(self) -> ValueT:
 				"""
 				Returns the next item in the sequence.
 
 				:returns:              Next item.
 				:raises StopIteration: If end of sequence is reached.
@@ -281,29 +284,27 @@
 
 
 setattr(Node, "DICT_TYPE", Dictionary)
 setattr(Node, "SEQ_TYPE", Sequence)
 
 
 @export
-class Configuration(Abstract_Configuration, Dictionary):
+class Configuration(Dictionary, Abstract_Configuration):
 	"""A configuration read from a YAML file."""
 
 	_yamlConfig: YAML
 
 	def __init__(self, configFile: Path):
 		"""
 		Initializes a configuration instance that reads a YAML file as input.
 
 		All sequence items or dictionaries key-value-pairs in the YAML file are accessible via Python's dictionary syntax.
 
 		:param configFile: Configuration file to read and parse.
 		"""
-		Abstract_Configuration.__init__(self)
-
 		with configFile.open() as file:
 			self._yamlConfig = YAML().load(file)
 
 		Dictionary.__init__(self, self, self, None, self._yamlConfig)
 
 	def __getitem__(self, key: str) -> ValueT:
 		"""
```

### Comparing `pyTooling-4.0.1/pyTooling/Configuration/__init__.py` & `pyTooling-5.0.0/pyTooling/StateMachine/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # ==================================================================================================================== #
-#             _____           _ _               ____             __ _                       _   _                      #
-#  _ __  _   |_   _|__   ___ | (_)_ __   __ _  / ___|___  _ __  / _(_) __ _ _   _ _ __ __ _| |_(_) ___  _ __           #
-# | '_ \| | | || |/ _ \ / _ \| | | '_ \ / _` || |   / _ \| '_ \| |_| |/ _` | | | | '__/ _` | __| |/ _ \| '_ \          #
-# | |_) | |_| || | (_) | (_) | | | | | | (_| || |__| (_) | | | |  _| | (_| | |_| | | | (_| | |_| | (_) | | | |         #
-# | .__/ \__, ||_|\___/ \___/|_|_|_| |_|\__, (_)____\___/|_| |_|_| |_|\__, |\__,_|_|  \__,_|\__|_|\___/|_| |_|         #
-# |_|    |___/                          |___/                         |___/                                            #
+#             _____           _ _               ____  _        _       __  __            _     _                       #
+#  _ __  _   |_   _|__   ___ | (_)_ __   __ _  / ___|| |_ __ _| |_ ___|  \/  | __ _  ___| |__ (_)_ __   ___            #
+# | '_ \| | | || |/ _ \ / _ \| | | '_ \ / _` | \___ \| __/ _` | __/ _ \ |\/| |/ _` |/ __| '_ \| | '_ \ / _ \           #
+# | |_) | |_| || | (_) | (_) | | | | | | (_| |_ ___) | || (_| | ||  __/ |  | | (_| | (__| | | | | | | |  __/           #
+# | .__/ \__, ||_|\___/ \___/|_|_|_| |_|\__, (_)____/ \__\__,_|\__\___|_|  |_|\__,_|\___|_| |_|_|_| |_|\___|           #
+# |_|    |___/                          |___/                                                                          #
 # ==================================================================================================================== #
 # Authors:                                                                                                             #
 #   Patrick Lehmann                                                                                                    #
 #                                                                                                                      #
 # License:                                                                                                             #
 # ==================================================================================================================== #
-# Copyright 2021-2023 Patrick Lehmann - Bötzingen, Germany                                                             #
+# Copyright 2017-2023 Patrick Lehmann - Bötzingen, Germany                                                             #
 #                                                                                                                      #
 # Licensed under the Apache License, Version 2.0 (the "License");                                                      #
 # you may not use this file except in compliance with the License.                                                     #
 # You may obtain a copy of the License at                                                                              #
 #                                                                                                                      #
 #   http://www.apache.org/licenses/LICENSE-2.0                                                                         #
 #                                                                                                                      #
@@ -24,89 +24,70 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.                                             #
 # See the License for the specific language governing permissions and                                                  #
 # limitations under the License.                                                                                       #
 #                                                                                                                      #
 # SPDX-License-Identifier: Apache-2.0                                                                                  #
 # ==================================================================================================================== #
 #
-"""\
-Abstract configuration reader.
-
-.. hint:: See :ref:`high-level help <CONFIG>` for explanations and usage examples.
 """
-from typing import Union, ClassVar, Iterator
-
-from ..Decorators import export
-from ..MetaClasses import ExtendedType
+This packages provides a data structure to describe statemachines.
 
+.. hint:: See :ref:`high-level help <STRUCT/StateMachine>` for explanations and usage examples.
+"""
+from typing import List
 
-KeyT = Union[str, int]
-NodeT = Union["Dictionary", "Sequence"]
-ValueT = Union[NodeT, str, int, float]
+from pyTooling.Decorators import export
+from pyTooling.MetaClasses import ExtendedType
 
 
 @export
-class Node(metaclass=ExtendedType, useSlots=True):
-	"""Abstract node in a configuration data structure."""
-
-	DICT_TYPE: ClassVar["Dictionary"]
-	SEQ_TYPE: ClassVar["Sequence"]
-	_parent: "Dictionary"
-	_root: "Configuration"
-
-	def __init__(self, root: "Configuration" = None, parent: NodeT = None):
-		self._root = root
-		self._parent = parent
-
-	def __len__(self) -> int:
-		raise NotImplementedError()
-
-	def __getitem__(self, key: KeyT) -> ValueT:
-		raise NotImplementedError()
-
-	def __setitem__(self, key: KeyT, value: ValueT) -> None:
-		raise NotImplementedError()
-
-	def __iter__(self) -> Iterator[ValueT]:
-		raise NotImplementedError()
-
-	@property
-	def Key(self) -> KeyT:
-		raise NotImplementedError()
-
-	@Key.setter
-	def Key(self, value: KeyT):
-		raise NotImplementedError()
-
-	def QueryPath(self, query: str) -> ValueT:
-		raise NotImplementedError()
+class Base(metaclass=ExtendedType, slots=True):
+	pass
 
 
 @export
-class Dictionary(Node):
-	"""Abstract dictionary node in a configuration."""
-
-	def __contains__(self, key: KeyT) -> bool:
-		raise NotImplementedError()
+class Transition(Base):
+	"""
+	Represents a transition (edge) in a statemachine diagram (directed graph).
+	"""
+	_source:      "State"
+	_destination: "State"
+
+	def __init__(self, source: "State", destination: "State"):
+		self._source = source
+		self._destination = destination
 
 
 @export
-class Sequence(Node):
-	"""Abstract sequence node in a configuration."""
-
-	def __getitem__(self, index: int) -> ValueT:
-		raise NotImplementedError()
+class State(Base):
+	"""
+	Represents a state (node/vertex) in a statemachine diagram (directed graph).
+	"""
+	_inboundTransitions:  List[Transition]
+	_outboundTransitions: List[Transition]
 
-	def __setitem__(self, index: int, value: ValueT) -> None:
-		raise NotImplementedError()
-
-
-setattr(Node, "DICT_TYPE", Dictionary)
-setattr(Node, "SEQ_TYPE", Sequence)
+	def __init__(self):
+		self._inboundTransitions = []
+		self._outboundTransitions = []
 
 
 @export
-class Configuration(Node):
-	"""Abstract root node in a configuration."""
+class StateMachine(Base):
+	"""
+	Represents a statemachine (graph) in a statemachine diagram (directed graph).
+	"""
+	_states:       List[State]
+	_initialState: State
+
+	def __init__(self, initialState: State):
+		self._states = []
+		self._initialState = initialState
+
+	def AddState(self, state: State):
+		if state not in self._states:    # TODO: use a set to check for double added states?
+			self._states.append(state)
+		else:
+			raise ValueError(f"State '{state}' was already added to this statemachine.")
 
-	def __init__(self):
-		Node.__init__(self)
+	@property
+	def States(self) -> List[State]:
+		return self._states
```

### Comparing `pyTooling-4.0.1/pyTooling/Decorators/__init__.py` & `pyTooling-5.0.0/pyTooling/Decorators/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -29,64 +29,60 @@
 # ==================================================================================================================== #
 #
 """Decorators controlling visibility of entities in a Python module.
 
 .. hint:: See :ref:`high-level help <DECO>` for explanations and usage examples.
 """
 import sys
+from functools import wraps
 from types     import FunctionType
-from typing import Union, Type, TypeVar, Callable, Any
+from typing    import Union, Type, TypeVar, Callable, Any
 
 __all__ = ["export", "Param", "RetType", "Func", "T"]
 
 
 try:
 	# See https://stackoverflow.com/questions/47060133/python-3-type-hinting-for-decorator
-	from typing import ParamSpec    # exists since Python 3.10
+	from typing import ParamSpec                     # WORKAROUND: exists since Python 3.10
 
 	Param = ParamSpec("Param")                       #: A parameter specification for function or method
 	RetType = TypeVar("RetType")                     #: Type variable for a return type
 	Func = Callable[Param, RetType]                  #: Type specification for a function
 except ImportError:  # pragma: no cover
 	Param = ...                                      #: A parameter specification for function or method
 	RetType = TypeVar("RetType")                     #: Type variable for a return type
 	Func = Callable[..., RetType]                    #: Type specification for a function
 
 
-T = TypeVar("T", bound=Union[Type, FunctionType])  #: Type variable for a class or function
+T = TypeVar("T", bound=Union[Type, FunctionType])  #: A type variable for a classes or functions.
+C = TypeVar("C", bound=Callable)                   #: A type variable for functions or methods.
 
 
 def export(entity: T) -> T:
 	"""
 	Register the given function or class as publicly accessible in a module.
 
 	Creates or updates the ``__all__`` attribute in the module in which the decorated entity is defined to include the
 	name of the decorated entity.
 
-	.. admonition:: ``to_export.py``
-
-	   .. code-block:: python
-
-	      from pyTooling.Decorators import export
-
-	      @export
-	      def exported():
-	        pass
-
-	      def not_exported():
-	        pass
-
-	.. admonition:: ``another_file.py``
-
-	   .. code-block:: python
-
-	      from .to_export import *
-
-	      assert "exported" in globals()
-	      assert "not_exported" not in globals()
+	+---------------------------------------------+------------------------------------------------+
+	| ``to_export.py``                            | ``another_file.py``                            |
+	+=============================================+================================================+
+	| .. code-block:: python                      | .. code-block:: python                         |
+	|                                             |                                                |
+	|    from pyTooling.Decorators import export  |    from .to_export import *                    |
+	|                                             |                                                |
+	|    @export                                  |                                                |
+	|    def exported():                          |    # 'exported' will be listed in __all__      |
+	|      pass                                   |    assert "exported"         in globals()      |
+	|                                             |                                                |
+	|    def not_exported():                      |    # 'not_exported' won't be listed in __all__ |
+	|      pass                                   |    assert "not_exported" not in globals()      |
+	|                                             |                                                |
+	+---------------------------------------------+------------------------------------------------+
 
 	:param entity:          The function or class to include in `__all__`.
 	:returns:               The unmodified function or class.
 	:raises AttributeError: If parameter ``entity`` has no ``__module__`` member.
 	:raises TypeError:      If parameter ``entity`` is not a top-level entity in a module.
 	:raises TypeError:      If parameter ``entity`` has no ``__name__``.
 	"""
@@ -107,23 +103,61 @@
 
 	try:
 		module = sys.modules[entity.__module__]
 	except KeyError:
 		raise ValueError(f"Module {entity.__module__} is not present in sys.modules. Please ensure it is in the import path before calling export().")
 
 	if hasattr(module, "__all__"):
-		if entity.__name__ not in module.__all__:	# type: ignore
-			module.__all__.append(entity.__name__)	# type: ignore
+		if entity.__name__ not in module.__all__:  # type: ignore
+			module.__all__.append(entity.__name__)   # type: ignore
 	else:
-		module.__all__ = [entity.__name__]	      # type: ignore
+		module.__all__ = [entity.__name__]         # type: ignore
 
 	return entity
 
 
 @export
+def notimplemented(message: str) -> Callable:
+	"""
+	Mark a method as *not implemented* and replace the implementation with a new method raising a :exc:`NotImplementedError`.
+
+	The original method is stored in ``<method>.__wrapped__`` and it's doc-string is copied to the replacing method. In
+	additional the field ``<method>.__notImplemented__`` is added.
+
+	.. admonition:: ``example.py``
+
+	   .. code-block:: python
+
+	      class Data:
+	        @notimplemented
+	        def method(self) -> bool:
+	          '''This method needs to be implemented'''
+	          return True
+
+	:param method: Method that is marked as *not implemented*.
+	:returns:      Replacement method, which raises a :exc:`NotImplementedError`.
+
+	.. seealso::
+
+	   * :func:`~pyTooling.Metaclasses.abstractmethod`
+	   * :func:`~pyTooling.Metaclasses.mustoverride`
+	"""
+
+	def decorator(method: C) -> C:
+		@wraps(method)
+		def func(*_, **__):
+			raise NotImplementedError(message)
+
+		func.__notImplemented__ = True
+		return func
+
+	return decorator
+
+
+@export
 def classproperty(method):
 
 	class Descriptor:
 		"""A decorator adding properties to classes."""
 		_getter: Callable
 		_setter: Callable
 
@@ -142,62 +176,26 @@
 			return self.__class__(self._getter, setter)
 
 	descriptor = Descriptor(method)
 	return descriptor
 
 
 @export
-def OriginalFunction(func: FunctionType) -> Callable[[Func], Func]:
+def readonly(func: FunctionType) -> property:
 	"""
-	Store a reference to the original function/method on a new, wrapper or replacement function/method.
-
-	The function or method reference is stored in ``__orig_func__``.
-
-	.. admonition:: ``metaclass.py``
-
-	   .. code-block:: python
-
-	      from functools import wraps
-	      from pyTooling.Decorators import OriginalFunction
+	Marks a property as *read-only*.
 
-	      class Meta(type):
-	        def __new__(self, className: str, baseClasses: Tuple[type], members: Dict[str, Any]) -> type:
-	          # Create a new class
-	          newClass = type.__new__(self, className, baseClasses, members)
-
-	          @OriginalFunction(newClass.__new__)
-	          @wraps(newClass.__new__)
-	          def new(cls, *args, **kwargs):
-	            # ...
-	            obj = newClass.__new__(*args, **kwargs)
-	            # ...
-	            return obj
-
-	          newClass.__new__ = new
-
-	          return newClass
-
-	:param func: Function or method reference to be store on the decorated function or method.
-	:returns:    Decorator function that stores the function or method reference on the decorated object.
-	"""
-	def decorator(f: Func) -> Func:
-		"""
-		Decorator function, which stores a reference to a function or method in a new field called ``__orig_func__``.
-
-		:param f:          Function or method, where the original function or method reference is attached to.
-		:returns:          Same method, but with new field ``__orig_func__`` set to the original function or method.
-		:raises TypeError: If decorated object is not callable.
-		"""
-		if not isinstance(f, Callable):
-			raise TypeError(f"Decorated object is not callable.")
+	It will remove ``<property>.setter`` and ``<property>.deleter``.
 
-		f.__orig_func__ = func
-		return f
+	:param func:
+	:return:
+	"""
+	prop = property(fget=func, fset=None, fdel=None, doc=func.__doc__)
 
-	return decorator
+	return prop
 
 
 @export
 def InheritDocString(baseClass: type) -> Callable[[Func], Func]:
 	"""
 	Copy the doc-string from given base-class to the method this decorator is applied to.
```

### Comparing `pyTooling-4.0.1/pyTooling/Exceptions/__init__.py` & `pyTooling-5.0.0/pyTooling/Exceptions/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -30,83 +30,73 @@
 # ==================================================================================================================== #
 #
 """
 A common set of missing exceptions in Python.
 
 .. hint:: See :ref:`high-level help <EXECPTION>` for explanations and usage examples.
 """
+from sys    import version_info
+from typing import List
+
 try:
 	from ..Decorators import export
 except (ImportError, ModuleNotFoundError):  # pragma: no cover
 	print("[pyTooling.MetaClasses] Could not import from 'pyTooling.*'!")
 
 	try:
 		from Decorators import export
 	except (ImportError, ModuleNotFoundError) as ex:  # pragma: no cover
 		print("[pyTooling.MetaClasses] Could not import from 'Decorators' directly!")
 		raise ex
 
 
 @export
-class AbstractClassError(Exception):
-	"""
-	The exception is raised, when a class contains methods marked with *abstractmethod* or *mustoverride*.
-
-	.. seealso::
-
-	   :py:func:`@abstractmethod <pyTooling.MetaClasses.abstractmethod>`
-	      |rarr| Mark a method as *abstract*.
-	   :py:func:`@mustoverride <pyTooling.MetaClasses.mustoverride>`
-	      |rarr| Mark a method as *must overrride*.
-	   :py:exc:`~MustOverrideClassError`
-	      |rarr| Exception raised, if a method is marked as *must-override*.
-	"""
-
-
-@export
-class MustOverrideClassError(AbstractClassError):
-	"""
-	The exception is raised, when a class contains methods marked with *must-override*.
-
-	.. seealso::
-
-	   :py:func:`@abstractmethod <pyTooling.MetaClasses.abstractmethod>`
-	      |rarr| Mark a method as *abstract*.
-	   :py:func:`@mustoverride <pyTooling.MetaClasses.mustoverride>`
-	      |rarr| Mark a method as *must overrride*.
-	   :py:exc:`~AbstractClassError`
-	      |rarr| Exception raised, if a method is marked as *abstract*.
-	"""
-
-
-@export
 class OverloadResolutionError(Exception):
 	"""
 	The exception is raised, when no matching overloaded method was found.
 
 	.. seealso::
 
-	   :py:func:`@overloadable <pyTooling.MetaClasses.overloadable>`
+	   :func:`@overloadable <pyTooling.MetaClasses.overloadable>`
 	      |rarr| Mark a method as *overloadable*.
 	"""
+	# WORKAROUND: for Python <3.11
+	# Implementing a dummy method for Python versions before
+	__notes__: List[str]
+	if version_info < (3, 11):  # pragma: no cover
+		def add_note(self, message: str):
+			try:
+				self.__notes__.append(message)
+			except AttributeError:
+				self.__notes__ = [message]
 
 
 @export
 class ExceptionBase(Exception):
-	"""Base exception derived from :py:exc:`Exception <python:Exception>` for all custom exceptions."""
+	"""Base exception derived from :exc:`Exception <python:Exception>` for all custom exceptions."""
 
 	def __init__(self, message: str = ""):
 		"""
 		ExceptionBase initializer.
 
 		:param message:   The exception message.
 		"""
 		super().__init__()
 		self.message = message
 
+	# WORKAROUND: for Python <3.11
+	# Implementing a dummy method for Python versions before
+	__notes__: List[str]
+	if version_info < (3, 11):  # pragma: no cover
+		def add_note(self, message: str):
+			try:
+				self.__notes__.append(message)
+			except AttributeError:
+				self.__notes__ = [message]
+
 	def __str__(self) -> str:
 		"""Returns the exception's message text."""
 		return self.message
 
 	def with_traceback(self, tb) -> None:
 		super().with_traceback(tb)
 
@@ -128,8 +118,18 @@
 @export
 class NotConfiguredException(ExceptionBase):
 	"""The exception is raise if the requested setting is not configured."""
 
 
 @export
 class ToolingException(Exception):
-	"""the exception is raised by pyTooling internal features."""
+	"""The exception is raised by pyTooling internal features."""
+
+	# WORKAROUND: for Python <3.11
+	# Implementing a dummy method for Python versions before
+	__notes__: List[str]
+	if version_info < (3, 11):  # pragma: no cover
+		def add_note(self, message: str):
+			try:
+				self.__notes__.append(message)
+			except AttributeError:
+				self.__notes__ = [message]
```

### Comparing `pyTooling-4.0.1/pyTooling/GenericPath/URL.py` & `pyTooling-5.0.0/pyTooling/GenericPath/URL.py`

 * *Files identical despite different names*

### Comparing `pyTooling-4.0.1/pyTooling/GenericPath/__init__.py` & `pyTooling-5.0.0/pyTooling/GenericPath/__init__.py`

 * *Files identical despite different names*

### Comparing `pyTooling-4.0.1/pyTooling/Graph/GraphML.py` & `pyTooling-5.0.0/pyTooling/Graph/GraphML.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,67 +43,83 @@
 from pyTooling.MetaClasses import ExtendedType
 from pyTooling.Graph import Graph as pyToolingGraph, Subgraph as pyToolingSubgraph
 from pyTooling.Tree import Node as pyToolingNode
 
 
 @export
 class AttributeContext(Enum):
+	"""
+	Enumeration of all attribute contexts.
+
+	An attribute context describes to what kind of GraphML node an attribute can be applied.
+	"""
 	GraphML = auto()
 	Graph = auto()
 	Node = auto()
 	Edge = auto()
 	Port = auto()
 
 	def __str__(self) -> str:
 		return f"{self.name.lower()}"
 
 
 @export
 class AttributeTypes(Enum):
+	"""
+	Enumeration of all attribute types.
+
+	An attribute type describes what datatype can be applied to an attribute.
+	"""
 	Boolean = auto()
 	Int = auto()
 	Long = auto()
 	Float = auto()
 	Double = auto()
 	String = auto()
 
 	def __str__(self) -> str:
 		return f"{self.name.lower()}"
 
 
 @export
 class EdgeDefault(Enum):
+	"""An enumeration describing the default edge direction."""
 	Undirected = auto()
 	Directed = auto()
 
 	def __str__(self) -> str:
 		return f"{self.name.lower()}"
 
 
 @export
 class ParsingOrder(Enum):
-	NodesFirst = auto()
+	"""An enumeration describing the parsing order of the graph's representation."""
+	NodesFirst = auto()     #: First, all nodes are given, then followed by all edges.
 	AdjacencyList = auto()
 	Free = auto()
 
 	def __str__(self) -> str:
 		return f"{self.name.lower()}"
 
 
 @export
 class IDStyle(Enum):
+	"""An enumeration describing the style of identifiers (IDs)."""
 	Canonical = auto()
 	Free = auto()
 
 	def __str__(self) -> str:
 		return f"{self.name.lower()}"
 
 
 @export
-class Base(metaclass=ExtendedType, useSlots=True):
+class Base(metaclass=ExtendedType, slots=True):
+	"""
+	Base-class for all GraphML data model classes.
+	"""
 	@property
 	def HasClosingTag(self) -> bool:
 		return True
 
 	def Tag(self, indent: int = 0) -> str:
 		raise NotImplementedError()
 
@@ -118,14 +134,15 @@
 
 
 @export
 class BaseWithID(Base):
 	_id: str
 
 	def __init__(self, identifier: str):
+		super().__init__()
 		self._id = identifier
 
 	@property
 	def ID(self) -> str:
 		return self._id
 
 
@@ -185,14 +202,16 @@
 
 @export
 class Data(Base):
 	_key: Key
 	_data: Any
 
 	def __init__(self, key: Key, data: Any):
+		super().__init__()
+
 		self._key = key
 		self._data = data
 
 	@property
 	def Key(self) -> Key:
 		return self._key
 
@@ -214,14 +233,16 @@
 
 	def ToStringLines(self, indent: int = 2) -> List[str]:
 		return [self.Tag(indent)]
 
 
 @export
 class Node(BaseWithData):
+	def __init__(self, identifier: str):
+		super().__init__(identifier)
 
 	@property
 	def HasClosingTag(self) -> bool:
 		return len(self._data) > 0
 
 	def Tag(self, indent: int = 2) -> str:
 		return f"""{'  '*indent}<node id="{self._id}" />\n"""
@@ -285,15 +306,15 @@
 			lines.extend(data.ToStringLines(indent + 1))
 		lines.append(self.ClosingTag(indent))
 
 		return lines
 
 
 @export
-class BaseGraph(BaseWithData):
+class BaseGraph(BaseWithData, mixin=True):
 	_subgraphs: Dict[str, 'Subgraph']
 	_nodes: Dict[str, Node]
 	_edges: Dict[str, Edge]
 	_edgeDefault: EdgeDefault
 	_parseOrder: ParsingOrder
 	_nodeIDStyle: IDStyle
 	_edgeIDStyle: IDStyle
@@ -403,14 +424,15 @@
 @export
 class Subgraph(Node, BaseGraph):
 	_subgraphID: str
 	_root:       Nullable[Graph]
 
 	def __init__(self, nodeIdentifier: str, graphIdentifier: str):
 		super().__init__(nodeIdentifier)
+		BaseGraph.__init__(self, nodeIdentifier)
 
 		self._subgraphID = graphIdentifier
 		self._root = None
 
 	@property
 	def RootGraph(self) -> Graph:
 		return self._root
```

### Comparing `pyTooling-4.0.1/pyTooling/Graph/__init__.py` & `pyTooling-5.0.0/pyTooling/Graph/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -50,14 +50,15 @@
 			 D & F -.-> B
 			 I ---> E --> F --> D
 
 			 classDef node fill:#eee,stroke:#777,font-size:smaller;
 """
 import heapq
 from collections import deque
+from itertools   import chain
 from typing import TypeVar, Generic, Optional as Nullable, Iterable, Hashable, Generator, Callable
 from typing import List, Union, Dict, Iterator as typing_Iterator, Set, Deque, Tuple
 
 from pyTooling.Decorators  import export
 from pyTooling.Exceptions  import ToolingException
 from pyTooling.MetaClasses import ExtendedType
 from pyTooling.Tree        import Node
@@ -145,15 +146,15 @@
 
 GraphDictValueType = TypeVar("GraphDictValueType")
 """A type variable for a graph's dictionary values."""
 
 
 @export
 class GraphException(ToolingException):
-	"""Base exception of all exceptions raised by :py:mod:`pyTooling.Graph`."""
+	"""Base exception of all exceptions raised by :mod:`pyTooling.Graph`."""
 
 
 @export
 class InternalError(GraphException):
 	"""
 	The exception is raised when a data structure corruption is detected.
 
@@ -199,26 +200,35 @@
 class CycleError(GraphException):
 	"""The exception is raised when a not permitted cycle is found."""
 
 
 @export
 class Base(
 	Generic[DictKeyType, DictValueType],
-	metaclass=ExtendedType, useSlots=True
+	metaclass=ExtendedType, slots=True
 ):
 	_dict: Dict[DictKeyType, DictValueType]  #: Dictionary to store key-value-pairs.
 
 	def __init__(self):
-		""".. todo:: GRAPH::Base::init Needs documentation."""
+		"""
+		.. todo:: GRAPH::Base::init Needs documentation.
+
+		"""
 		self._dict = {}
 
 	def __del__(self):
-		""".. todo:: GRAPH::Base::del Needs documentation."""
+		"""
+		.. todo:: GRAPH::Base::del Needs documentation.
+
+		"""
 		del self._dict
 
+	def Delete(self) -> None:
+		self._dict = None
+
 	def __getitem__(self, key: DictKeyType) -> DictValueType:
 		"""
 		Read a vertex's attached attributes (key-value-pairs) by key.
 
 		:param key: The key to look for.
 		:returns:   The value associated to the given key.
 		"""
@@ -268,49 +278,52 @@
 	Generic[IDType, ValueType, WeightType, DictKeyType, DictValueType]
 ):
 	_id:        Nullable[IDType]      #: Field storing the object's Identifier.
 	_value:     Nullable[ValueType]   #: Field storing the object's value of any type.
 	_weight:    Nullable[WeightType]  #: Field storing the object's weight.
 
 	def __init__(self, identifier: IDType = None, value: ValueType = None, weight: WeightType = None):
-		""".. todo:: GRAPH::Vertex::init Needs documentation."""
+		"""
+		.. todo:: GRAPH::Vertex::init Needs documentation.
+
+		"""
 		super().__init__()
 
 		self._id = identifier
 		self._value = value
 		self._weight = weight
 
 	@property
 	def ID(self) -> Nullable[IDType]:
 		"""
-		Read-only property to access the unique ID (:py:attr:`_id`).
+		Read-only property to access the unique ID (:attr:`_id`).
 
 		If no ID was given at creation time, ID returns ``None``.
 
 		:returns: Unique ID, if ID was given at creation time, else ``None``.
 		"""
 		return self._id
 
 	@property
 	def Value(self) -> ValueType:
 		"""
-		Property to get and set the value (:py:attr:`_value`).
+		Property to get and set the value (:attr:`_value`).
 
 		:returns: The value.
 		"""
 		return self._value
 
 	@Value.setter
 	def Value(self, value: ValueType) -> None:
 		self._value = value
 
 	@property
 	def Weight(self) -> Nullable[EdgeWeightType]:
 		"""
-		Property to get and set the weight (:py:attr:`_weight`) of an edge.
+		Property to get and set the weight (:attr:`_weight`) of an edge.
 
 		:returns: The weight of an edge.
 		"""
 		return self._weight
 
 	@Weight.setter
 	def Weight(self, value: Nullable[EdgeWeightType]) -> None:
@@ -321,26 +334,29 @@
 class BaseWithName(
 	Base[DictKeyType, DictValueType],
 	Generic[DictKeyType, DictValueType]
 ):
 	_name: Nullable[str]  #: Field storing the object's name.
 
 	def __init__(self, name: str = None):
-		""".. todo:: GRAPH::BaseWithName::init Needs documentation."""
+		"""
+		.. todo:: GRAPH::BaseWithName::init Needs documentation.
+
+		"""
 		if name is not None and not isinstance(name, str):
 			raise TypeError("Parameter 'name' is not of type 'str'.")
 
 		super().__init__()
 
 		self._name = name
 
 	@property
 	def Name(self) -> Nullable[str]:
 		"""
-		Property to get and set the name (:py:attr:`_name`).
+		Property to get and set the name (:attr:`_name`).
 
 		:returns: The value of a component.
 		"""
 		return self._name
 
 	@Name.setter
 	def Name(self, value: str) -> None:
@@ -369,43 +385,50 @@
 	_vertices: Set['Vertex[GraphDictKeyType, GraphDictValueType,'
 								'VertexIDType, VertexWeightType, VertexValueType, VertexDictKeyType, VertexDictValueType,'
 								'EdgeIDType, EdgeWeightType, EdgeValueType, EdgeDictKeyType, EdgeDictValueType,'
 								'LinkIDType, LinkWeightType, LinkValueType, LinkDictKeyType, LinkDictValueType'
 								']']  #: Field storing a set of vertices.
 
 	def __init__(self, graph: 'Graph', name: str = None, vertices: Iterable['Vertex'] = None):
-		""".. todo:: GRAPH::Component::init Needs documentation."""
+		"""
+		.. todo:: GRAPH::Component::init Needs documentation.
+
+		"""
 		if graph is None:
 			raise ValueError("Parameter 'graph' is None.")
 		if not isinstance(graph, Graph):
 			raise TypeError("Parameter 'graph' is not of type 'Graph'.")
 
 		super().__init__(name)
 
 		self._graph = graph
 		self._vertices = set() if vertices is None else {v for v in vertices}
 
 	def __del__(self):
-		""".. todo:: GRAPH::BaseWithVertices::del Needs documentation."""
-		super().__del__()
+		"""
+		.. todo:: GRAPH::BaseWithVertices::del Needs documentation.
+
+		"""
 		del self._vertices
 
+		super().__del__()
+
 	@property
 	def Graph(self) -> 'Graph':
 		"""
-		Read-only property to access the graph, this object is associated to (:py:attr:`_graph`).
+		Read-only property to access the graph, this object is associated to (:attr:`_graph`).
 
 		:returns: The graph this object is associated to.
 		"""
 		return self._graph
 
 	@property
 	def Vertices(self) -> Set['Vertex']:
 		"""
-		Read-only property to access the vertices in this component (:py:attr:`_vertices`).
+		Read-only property to access the vertices in this component (:attr:`_vertices`).
 
 		:returns: The set of vertices in this component.
 		"""
 		return self._vertices
 
 	@property
 	def VertexCount(self) -> int:
@@ -437,15 +460,18 @@
 	_views:     Dict[Hashable, 'View']
 	_inboundEdges:   List['Edge[EdgeIDType, EdgeWeightType, EdgeValueType, EdgeDictKeyType, EdgeDictValueType]']  #: Field storing a list of inbound edges.
 	_outboundEdges:  List['Edge[EdgeIDType, EdgeWeightType, EdgeValueType, EdgeDictKeyType, EdgeDictValueType]']  #: Field storing a list of outbound edges.
 	_inboundLinks:   List['Link[EdgeIDType, EdgeWeightType, EdgeValueType, EdgeDictKeyType, EdgeDictValueType]']  #: Field storing a list of inbound links.
 	_outboundLinks:  List['Link[EdgeIDType, EdgeWeightType, EdgeValueType, EdgeDictKeyType, EdgeDictValueType]']  #: Field storing a list of outbound links.
 
 	def __init__(self, vertexID: VertexIDType = None, value: VertexValueType = None, weight: VertexWeightType = None, graph: 'Graph' = None, subgraph: 'Subgraph' = None):
-		""".. todo:: GRAPH::Vertex::init Needs documentation."""
+		"""
+		.. todo:: GRAPH::Vertex::init Needs documentation.
+
+		"""
 		if vertexID is not None and not isinstance(vertexID, Hashable):
 			raise TypeError("Parameter 'vertexID' is not of type 'VertexIDType'.")
 
 		super().__init__(vertexID, value, weight)
 
 		if subgraph is None:
 			self._graph = graph if graph is not None else Graph()
@@ -466,76 +492,115 @@
 			if vertexID is None:
 				subgraph._verticesWithoutID.append(self)
 			elif vertexID not in subgraph._verticesWithID:
 				subgraph._verticesWithID[vertexID] = self
 			else:
 				raise DuplicateVertexError(f"Vertex ID '{vertexID}' already exists in this subgraph.")
 
+		self._views =         {}
 		self._inboundEdges =  []
 		self._outboundEdges = []
 		self._inboundLinks =  []
 		self._outboundLinks = []
 
 	def __del__(self):
-		""".. todo:: GRAPH::BaseEdge::del Needs documentation."""
-		super().__del__()
+		"""
+		.. todo:: GRAPH::BaseEdge::del Needs documentation.
+
+		"""
+		del self._views
 		del self._inboundEdges
 		del self._outboundEdges
 		del self._inboundLinks
 		del self._outboundLinks
 
+		super().__del__()
+
+	def Delete(self) -> None:
+		for edge in self._outboundEdges:
+			edge._destination._inboundEdges.remove(edge)
+			edge._Delete()
+		for edge in self._inboundEdges:
+			edge._source._outboundEdges.remove(edge)
+			edge._Delete()
+		for link in self._outboundLinks:
+			link._destination._inboundLinks.remove(link)
+			link._Delete()
+		for link in self._inboundLinks:
+			link._source._outboundLinks.remove(link)
+			link._Delete()
+
+		if self._id is None:
+			self._graph._verticesWithoutID.remove(self)
+		else:
+			del self._graph._verticesWithID[self._id]
+
+		# subgraph
+
+		# component
+
+		# views
+		self._views =         None
+		self._inboundEdges =  None
+		self._outboundEdges = None
+		self._inboundLinks =  None
+		self._outboundLinks = None
+
+		super().Delete()
+		assert getrefcount(self) == 1
+
 	@property
 	def Graph(self) -> 'Graph':
 		"""
-		Read-only property to access the graph, this vertex is associated to (:py:attr:`_graph`).
+		Read-only property to access the graph, this vertex is associated to (:attr:`_graph`).
 
 		:returns: The graph this vertex is associated to.
 		"""
 		return self._graph
 
 	@property
 	def Component(self) -> 'Component':
 		"""
-		Read-only property to access the component, this vertex is associated to (:py:attr:`_component`).
+		Read-only property to access the component, this vertex is associated to (:attr:`_component`).
 
 		:returns: The component this vertex is associated to.
 		"""
 		return self._component
 
 	@property
 	def InboundEdges(self) -> Tuple['Edge', ...]:
 		"""
-		Read-only property to get a tuple of inbound edges (:py:attr:`_inboundEdges`).
+		Read-only property to get a tuple of inbound edges (:attr:`_inboundEdges`).
 
 		:return: Tuple of inbound edges.
 		"""
 		return tuple(self._inboundEdges)
 
 	@property
 	def OutboundEdges(self) -> Tuple['Edge', ...]:
 		"""
-		Read-only property to get a tuple of outbound edges (:py:attr:`_outboundEdges`).
+		Read-only property to get a tuple of outbound edges (:attr:`_outboundEdges`).
 
 		:return: Tuple of outbound edges.
 		"""
 		return tuple(self._outboundEdges)
 
 	@property
 	def InboundLinks(self) -> Tuple['Link', ...]:
 		"""
-		Read-only property to get a tuple of inbound links (:py:attr:`_inboundLinks`).
+		Read-only property to get a tuple of inbound links (:attr:`_inboundLinks`).
 
 		:return: Tuple of inbound links.
 		"""
 		return tuple(self._inboundLinks)
 
 	@property
 	def OutboundLinks(self) -> Tuple['Link', ...]:
 		"""
-		Read-only property to get a tuple of outbound links (:py:attr:`_outboundLinks`).
+		Read-only property to get a tuple of outbound links (:attr:`_outboundLinks`).
 
 		:return: Tuple of outbound links.
 		"""
 		return tuple(self._outboundLinks)
 
 	@property
 	def EdgeCount(self) -> int:
@@ -598,19 +663,19 @@
 
 		A root has no inbound edges (no predecessor vertices).
 
 		:returns: ``True``, if this vertex is a root.
 
 		.. seealso::
 
-		   :py:meth:`IsLeaf` |br|
+		   :meth:`IsLeaf` |br|
 		      |rarr| Check if a vertex is a leaf vertex in the graph.
-		   :py:meth:`Graph.IterateRoots <pyTooling.Graph.Graph.IterateRoots>` |br|
+		   :meth:`Graph.IterateRoots <pyTooling.Graph.Graph.IterateRoots>` |br|
 		      |rarr| Iterate all roots of a graph.
-		   :py:meth:`Graph.IterateLeafs <pyTooling.Graph.Graph.IterateLeafs>` |br|
+		   :meth:`Graph.IterateLeafs <pyTooling.Graph.Graph.IterateLeafs>` |br|
 		      |rarr| Iterate all leafs of a graph.
 		"""
 		return len(self._inboundEdges) == 0
 
 	@property
 	def IsLeaf(self) -> bool:
 		"""
@@ -618,19 +683,19 @@
 
 		A leaf has no outbound edges (no successor vertices).
 
 		:returns: ``True``, if this vertex is a leaf.
 
 		.. seealso::
 
-		   :py:meth:`IsRoot` |br|
+		   :meth:`IsRoot` |br|
 		      |rarr| Check if a vertex is a root vertex in the graph.
-		   :py:meth:`Graph.IterateRoots <pyTooling.Graph.Graph.IterateRoots>` |br|
+		   :meth:`Graph.IterateRoots <pyTooling.Graph.Graph.IterateRoots>` |br|
 		      |rarr| Iterate all roots of a graph.
-		   :py:meth:`Graph.IterateLeafs <pyTooling.Graph.Graph.IterateLeafs>` |br|
+		   :meth:`Graph.IterateLeafs <pyTooling.Graph.Graph.IterateLeafs>` |br|
 		      |rarr| Iterate all leafs of a graph.
 		"""
 		return len(self._outboundEdges) == 0
 
 	@property
 	def Predecessors(self) -> Tuple['Vertex', ...]:
 		"""
@@ -646,15 +711,18 @@
 		Read-only property to get a tuple of successor vertices.
 
 		:return: Tuple of successor vertices.
 		"""
 		return tuple([edge.Destination for edge in self._outboundEdges])
 
 	def EdgeToVertex(self, vertex: 'Vertex', edgeID: EdgeIDType = None, edgeWeight: EdgeWeightType = None, edgeValue: VertexValueType = None) -> 'Edge':
-		""".. todo:: GRAPH::Vertex::EdgeToVertex Needs documentation."""
+		"""
+		.. todo:: GRAPH::Vertex::EdgeToVertex Needs documentation.
+
+		"""
 		if self._subgraph is vertex._subgraph:
 			edge = Edge(self, vertex, edgeID, edgeValue, edgeWeight)
 
 			self._outboundEdges.append(edge)
 			vertex._inboundEdges.append(edge)
 
 			if self._subgraph is None:
@@ -677,15 +745,18 @@
 		else:
 			# FIXME: needs an error message
 			raise GraphException()
 
 		return edge
 
 	def EdgeFromVertex(self, vertex: 'Vertex', edgeID: EdgeIDType = None, edgeWeight: EdgeWeightType = None, edgeValue: VertexValueType = None) -> 'Edge':
-		""".. todo:: GRAPH::Vertex::EdgeFromVertex Needs documentation."""
+		"""
+		.. todo:: GRAPH::Vertex::EdgeFromVertex Needs documentation.
+
+		"""
 		if self._subgraph is vertex._subgraph:
 			edge = Edge(vertex, self, edgeID, edgeValue, edgeWeight)
 
 			vertex._outboundEdges.append(edge)
 			self._inboundEdges.append(edge)
 
 			if self._subgraph is None:
@@ -708,15 +779,18 @@
 		else:
 			# FIXME: needs an error message
 			raise GraphException()
 
 		return edge
 
 	def EdgeToNewVertex(self, vertexID: VertexIDType = None, vertexValue: VertexValueType = None, vertexWeight: VertexWeightType = None, edgeID: EdgeIDType = None, edgeWeight: EdgeWeightType = None, edgeValue: VertexValueType = None) -> 'Edge':
-		""".. todo:: GRAPH::Vertex::EdgeToNewVertex Needs documentation."""
+		"""
+		.. todo:: GRAPH::Vertex::EdgeToNewVertex Needs documentation.
+
+		"""
 		vertex = Vertex(vertexID, vertexValue, vertexWeight, graph=self._graph)  # , component=self._component)
 
 		if self._subgraph is vertex._subgraph:
 			edge = Edge(self, vertex, edgeID, edgeValue, edgeWeight)
 
 			self._outboundEdges.append(edge)
 			vertex._inboundEdges.append(edge)
@@ -741,15 +815,18 @@
 		else:
 			# FIXME: needs an error message
 			raise GraphException()
 
 		return edge
 
 	def EdgeFromNewVertex(self, vertexID: VertexIDType = None, vertexValue: VertexValueType = None, vertexWeight: VertexWeightType = None, edgeID: EdgeIDType = None, edgeWeight: EdgeWeightType = None, edgeValue: VertexValueType = None) -> 'Edge':
-		""".. todo:: GRAPH::Vertex::EdgeFromNewVertex Needs documentation."""
+		"""
+		.. todo:: GRAPH::Vertex::EdgeFromNewVertex Needs documentation.
+
+		"""
 		vertex = Vertex(vertexID, vertexValue, vertexWeight, graph=self._graph)  # , component=self._component)
 
 		if self._subgraph is vertex._subgraph:
 			edge = Edge(vertex, self, edgeID, edgeValue, edgeWeight)
 
 			vertex._outboundEdges.append(edge)
 			self._inboundEdges.append(edge)
@@ -774,15 +851,18 @@
 		else:
 			# FIXME: needs an error message
 			raise GraphException()
 
 		return edge
 
 	def LinkToVertex(self, vertex: 'Vertex', linkID: EdgeIDType = None, linkWeight: EdgeWeightType = None, linkValue: VertexValueType = None) -> 'Link':
-		""".. todo:: GRAPH::Vertex::LinkToVertex Needs documentation."""
+		"""
+		.. todo:: GRAPH::Vertex::LinkToVertex Needs documentation.
+
+		"""
 		if self._subgraph is vertex._subgraph:
 			# FIXME: needs an error message
 			raise GraphException()
 		else:
 			link = Link(self, vertex, linkID, linkValue, linkWeight)
 
 			self._outboundLinks.append(link)
@@ -807,15 +887,18 @@
 					vertex._subgraph._linksWithID[linkID] = link
 				else:
 					raise DuplicateEdgeError(f"Link ID '{linkID}' already exists in this graph.")
 
 		return link
 
 	def LinkFromVertex(self, vertex: 'Vertex', linkID: EdgeIDType = None, linkWeight: EdgeWeightType = None, linkValue: VertexValueType = None) -> 'Edge':
-		""".. todo:: GRAPH::Vertex::LinkToVertex Needs documentation."""
+		"""
+		.. todo:: GRAPH::Vertex::LinkToVertex Needs documentation.
+
+		"""
 		if self._subgraph is vertex._subgraph:
 			# FIXME: needs an error message
 			raise GraphException()
 		else:
 			link = Link(vertex, self, linkID, linkValue, linkWeight)
 
 			vertex._outboundLinks.append(link)
@@ -848,19 +931,19 @@
 		Check if this vertex is linked to another vertex by any outbound edge.
 
 		:param destination: Destination vertex to check.
 		:return:            ``True``, if the destination vertex is a destination on any outbound edge.
 
 		.. seealso::
 
-		   :py:meth:`HasEdgeFromSource` |br|
+		   :meth:`HasEdgeFromSource` |br|
 		      |rarr| Check if this vertex is linked to another vertex by any inbound edge.
-		   :py:meth:`HasLinkToDestination` |br|
+		   :meth:`HasLinkToDestination` |br|
 		      |rarr| Check if this vertex is linked to another vertex by any outbound link.
-		   :py:meth:`HasLinkFromSource` |br|
+		   :meth:`HasLinkFromSource` |br|
 		      |rarr| Check if this vertex is linked to another vertex by any inbound link.
 		"""
 		for edge in self._outboundEdges:
 			if destination is edge.Destination:
 				return True
 
 		return False
@@ -870,19 +953,19 @@
 		Check if this vertex is linked to another vertex by any inbound edge.
 
 		:param source: Source vertex to check.
 		:return:       ``True``, if the source vertex is a source on any inbound edge.
 
 		.. seealso::
 
-		   :py:meth:`HasEdgeToDestination` |br|
+		   :meth:`HasEdgeToDestination` |br|
 		      |rarr| Check if this vertex is linked to another vertex by any outbound edge.
-		   :py:meth:`HasLinkToDestination` |br|
+		   :meth:`HasLinkToDestination` |br|
 		      |rarr| Check if this vertex is linked to another vertex by any outbound link.
-		   :py:meth:`HasLinkFromSource` |br|
+		   :meth:`HasLinkFromSource` |br|
 		      |rarr| Check if this vertex is linked to another vertex by any inbound link.
 		"""
 		for edge in self._inboundEdges:
 			if source is edge.Source:
 				return True
 
 		return False
@@ -892,19 +975,19 @@
 		Check if this vertex is linked to another vertex by any outbound link.
 
 		:param destination: Destination vertex to check.
 		:return:            ``True``, if the destination vertex is a destination on any outbound link.
 
 		.. seealso::
 
-		   :py:meth:`HasEdgeToDestination` |br|
+		   :meth:`HasEdgeToDestination` |br|
 		      |rarr| Check if this vertex is linked to another vertex by any outbound edge.
-		   :py:meth:`HasEdgeFromSource` |br|
+		   :meth:`HasEdgeFromSource` |br|
 		      |rarr| Check if this vertex is linked to another vertex by any inbound edge.
-		   :py:meth:`HasLinkFromSource` |br|
+		   :meth:`HasLinkFromSource` |br|
 		      |rarr| Check if this vertex is linked to another vertex by any inbound link.
 		"""
 		for link in self._outboundLinks:
 			if destination is link.Destination:
 				return True
 
 		return False
@@ -914,27 +997,63 @@
 		Check if this vertex is linked to another vertex by any inbound link.
 
 		:param source: Source vertex to check.
 		:return:       ``True``, if the source vertex is a source on any inbound link.
 
 		.. seealso::
 
-		   :py:meth:`HasEdgeToDestination` |br|
+		   :meth:`HasEdgeToDestination` |br|
 		      |rarr| Check if this vertex is linked to another vertex by any outbound edge.
-		   :py:meth:`HasEdgeFromSource` |br|
+		   :meth:`HasEdgeFromSource` |br|
 		      |rarr| Check if this vertex is linked to another vertex by any inbound edge.
-		   :py:meth:`HasLinkToDestination` |br|
+		   :meth:`HasLinkToDestination` |br|
 		      |rarr| Check if this vertex is linked to another vertex by any outbound link.
 		"""
 		for link in self._inboundLinks:
 			if source is link.Source:
 				return True
 
 		return False
 
+	def DeleteEdgeTo(self, destination: 'Vertex'):
+		for edge in self._outboundEdges:
+			if edge._destination is destination:
+				break
+		else:
+			raise GraphException(f"No outbound edge found to '{destination!r}'.")
+
+		edge.Delete()
+
+	def DeleteEdgeFrom(self, source: 'Vertex'):
+		for edge in self._inboundEdges:
+			if edge._source is source:
+				break
+		else:
+			raise GraphException(f"No inbound edge found to '{source!r}'.")
+
+		edge.Delete()
+
+	def DeleteLinkTo(self, destination: 'Vertex'):
+		for link in self._outboundLinks:
+			if link._destination is destination:
+				break
+		else:
+			raise GraphException(f"No outbound link found to '{destination!r}'.")
+
+		link.Delete()
+
+	def DeleteLinkFrom(self, source: 'Vertex'):
+		for link in self._inboundLinks:
+			if link._source is source:
+				break
+		else:
+			raise GraphException(f"No inbound link found to '{source!r}'.")
+
+		link.Delete()
+
 	def Copy(self, graph: Graph, copyDict: bool = False, linkingKeyToOriginalVertex: str = None, linkingKeyFromOriginalVertex: str = None) -> 'Vertex':
 		"""
 		Creates a copy of this vertex in another graph.
 
 		Optionally, the vertex's attached attributes (key-value-pairs) can be copied and a linkage between both vertices
 		can be established.
 
@@ -1065,15 +1184,15 @@
 		"""
 		A generator to iterate all reachable vertices starting from this node in breadth-first search (BFS) order.
 
 		:returns: A generator to iterate vertices traversed in BFS order.
 
 		.. seealso::
 
-		   :py:meth:`IterateVerticesDFS` |br|
+		   :meth:`IterateVerticesDFS` |br|
 		      |rarr| Iterate all reachable vertices **depth-first search** order.
 		"""
 		visited: Set[Vertex] = set()
 		queue: Deque[Vertex] = deque()
 
 		yield self
 		visited.add(self)
@@ -1096,15 +1215,15 @@
 		"""
 		A generator to iterate all reachable vertices starting from this node in depth-first search (DFS) order.
 
 		:returns: A generator to iterate vertices traversed in DFS order.
 
 		.. seealso::
 
-		   :py:meth:`IterateVerticesBFS` |br|
+		   :meth:`IterateVerticesBFS` |br|
 		      |rarr| Iterate all reachable vertices **breadth-first search** order.
 
 		   Wikipedia - https://en.wikipedia.org/wiki/Depth-first_search
 		"""
 		visited: Set[Vertex] = set()
 		stack: List[typing_Iterator[Edge]] = list()
 
@@ -1123,14 +1242,52 @@
 						stack.append(iter(nextVertex._outboundEdges))
 			except StopIteration:
 				stack.pop()
 
 				if len(stack) == 0:
 					return
 
+	def IterateAllOutboundPathsAsVertexList(self) -> Generator[Tuple['Vertex', ...], None, None]:
+		if len(self._outboundEdges) == 0:
+			yield (self, )
+			return
+
+		visited:       Set[Vertex] =                 set()
+		vertexStack:   List[Vertex] =                list()
+		iteratorStack: List[typing_Iterator[Edge]] = list()
+
+		visited.add(self)
+		vertexStack.append(self)
+		iteratorStack.append(iter(self._outboundEdges))
+
+		while True:
+			try:
+				edge = next(iteratorStack[-1])
+				nextVertex = edge._destination
+				if nextVertex in visited:
+					ex = CycleError(f"Loop detected.")
+					ex.add_note(f"First loop is:")
+					for i, vertex in enumerate(vertexStack):
+						ex.add_note(f"  {i}: {vertex!r}")
+					raise ex
+
+				vertexStack.append(nextVertex)
+				if len(nextVertex._outboundEdges) == 0:
+					yield tuple(vertexStack)
+					vertexStack.pop()
+				else:
+					iteratorStack.append(iter(nextVertex._outboundEdges))
+
+			except StopIteration:
+				vertexStack.pop()
+				iteratorStack.pop()
+
+				if len(vertexStack) == 0:
+					return
+
 	def ShortestPathToByHops(self, destination: 'Vertex') -> Generator['Vertex', None, None]:
 		"""
 		Compute the shortest path (by hops) between this vertex and the destination vertex.
 
 		A generator is return to iterate all vertices along the path including source and destination vertex.
 
 		The search algorithm is breadth-first search (BFS) based. The found solution, if any, is not unique but deterministic
@@ -1143,15 +1300,15 @@
 		if self is destination:
 			yield self
 			return
 
 		# Local struct to create multiple linked-lists forming a paths from current node back to the starting point
 		# (actually a tree). Each node holds a reference to the vertex it represents.
 		# Hint: slotted classes are faster than '@dataclasses.dataclass'.
-		class Node(metaclass=ExtendedType, useSlots=True):
+		class Node(metaclass=ExtendedType, slots=True):
 			parent: 'Node'
 			ref: Vertex
 
 			def __init__(self, parent: 'Node', ref: Vertex):
 				self.parent = parent
 				self.ref = ref
 
@@ -1218,15 +1375,15 @@
 
 	def ShortestPathToByWeight(self, destination: 'Vertex') -> Generator['Vertex', None, None]:
 		"""
 		Compute the shortest path (by edge weight) between this vertex and the destination vertex.
 
 		A generator is return to iterate all vertices along the path including source and destination vertex.
 
-		The search algorithm is based on Dijkstra algorithm and using :py:mod:`heapq`. The found solution, if any, is not
+		The search algorithm is based on Dijkstra algorithm and using :mod:`heapq`. The found solution, if any, is not
 		unique but deterministic as long as the graph was not modified (e.g. ordering of edges on vertices).
 
 		:param destination: The destination vertex to reach.
 		:return:            A generator to iterate all vertices on the path found between this vertex and the destination vertex.
 		"""
 		# Improvements: both-sided Dijkstra (search from start and destination to reduce discovered area.
 
@@ -1235,15 +1392,15 @@
 			yield self
 			return
 
 		# Local struct to create multiple-linked lists forming a paths from current node back to the starting point
 		# (actually a tree). Each node holds the overall weight from start to current node and a reference to the vertex it
 		# represents.
 		# Hint: slotted classes are faster than '@dataclasses.dataclass'.
-		class Node(metaclass=ExtendedType, useSlots=True):
+		class Node(metaclass=ExtendedType, slots=True):
 			parent: 'Node'
 			distance: EdgeWeightType
 			ref: Vertex
 
 			def __init__(self, parent: 'Node', distance: EdgeWeightType, ref: Vertex):
 				self.parent = parent
 				self.distance = distance
@@ -1325,15 +1482,15 @@
 	# 	raise NotImplementedError()
 	# 	# Ford-Fulkerson algorithm
 	# 	# Edmons-Karp algorithm
 	# 	# Dinic's algorithm
 
 	def ConvertToTree(self) -> Node:
 		"""
-		Converts all reachable vertices from this starting vertex to a tree of :py:class:`~pyTooling.Tree.Node` instances.
+		Converts all reachable vertices from this starting vertex to a tree of :class:`~pyTooling.Tree.Node` instances.
 
 		The tree is traversed using depths-first-search.
 
 		:return:
 		"""
 		visited: Set[Vertex] = set()
 		stack: List[Tuple[Node, typing_Iterator[Edge]]] = list()
@@ -1382,17 +1539,17 @@
 
 	def __str__(self) -> str:
 		"""
 		Return a string representation of the vertex.
 
 		Order of resolution:
 
-		1. If :py:attr:`_value` is not None, return the string representation of :py:attr:`_value`.
-		2. If :py:attr:`_id` is not None, return the string representation of :py:attr:`_id`.
-		3. Else, return :py:meth:`__repr__`.
+		1. If :attr:`_value` is not None, return the string representation of :attr:`_value`.
+		2. If :attr:`_id` is not None, return the string representation of :attr:`_id`.
+		3. Else, return :meth:`__repr__`.
 
 		:returns: The resolved string representation of the vertex.
 		"""
 		if self._value is not None:
 			return str(self._value)
 		elif self._id is not None:
 			return str(self._id)
@@ -1409,15 +1566,18 @@
 	An **edge** can have a unique ID, a value, a weight and attached meta information as key-value-pairs. All edges are
 	directed.
 	"""
 	_source:      Vertex
 	_destination: Vertex
 
 	def __init__(self, source: Vertex, destination: Vertex, edgeID: EdgeIDType = None, value: EdgeValueType = None, weight: EdgeWeightType = None):
-		""".. todo:: GRAPH::BaseEdge::init Needs documentation."""
+		"""
+		.. todo:: GRAPH::BaseEdge::init Needs documentation.
+
+		"""
 		super().__init__(edgeID, value, weight)
 
 		self._source = source
 		self._destination = destination
 
 		component = source._component
 		if component is not destination._component:
@@ -1428,24 +1588,24 @@
 				component._vertices.add(vertex)
 			component._graph._components.remove(oldComponent)
 			del oldComponent
 
 	@property
 	def Source(self) -> Vertex:
 		"""
-		Read-only property to get the source (:py:attr:`_source`) of an edge.
+		Read-only property to get the source (:attr:`_source`) of an edge.
 
 		:returns: The source of an edge.
 		"""
 		return self._source
 
 	@property
 	def Destination(self) -> Vertex:
 		"""
-		Read-only property to get the destination (:py:attr:`_destination`) of an edge.
+		Read-only property to get the destination (:attr:`_destination`) of an edge.
 
 		:returns: The destination of an edge.
 		"""
 		return self._destination
 
 	def Reverse(self) -> None:
 		"""Reverse the direction of this edge."""
@@ -1461,15 +1621,18 @@
 ):
 	"""
 	An **edge** can have a unique ID, a value, a weight and attached meta information as key-value-pairs. All edges are
 	directed.
 	"""
 
 	def __init__(self, source: Vertex, destination: Vertex, edgeID: EdgeIDType = None, value: EdgeValueType = None, weight: EdgeWeightType = None):
-		""".. todo:: GRAPH::Edge::init Needs documentation."""
+		"""
+		.. todo:: GRAPH::Edge::init Needs documentation.
+
+		"""
 		if not isinstance(source, Vertex):
 			raise TypeError("Parameter 'source' is not of type 'Vertex'.")
 		if not isinstance(destination, Vertex):
 			raise TypeError("Parameter 'destination' is not of type 'Vertex'.")
 		if edgeID is not None and not isinstance(edgeID, Hashable):
 			raise TypeError("Parameter 'edgeID' is not of type 'EdgeIDType'.")
 		# if value is not None and  not isinstance(value, Vertex):
@@ -1477,14 +1640,34 @@
 		if weight is not None and not isinstance(weight, (int, float)):
 			raise TypeError("Parameter 'weight' is not of type 'EdgeWeightType'.")
 		if source._graph is not destination._graph:
 			raise NotInSameGraph(f"Source vertex and destination vertex are not in same graph.")
 
 		super().__init__(source, destination, edgeID, value, weight)
 
+	def Delete(self) -> None:
+		# Remove from Source and Destination
+		self._source._outboundEdges.remove(self)
+		self._destination._inboundEdges.remove(self)
+
+		# Remove from Graph and Subgraph
+		if self._id is None:
+			self._source._graph._edgesWithoutID.remove(self)
+			if self._source._subgraph is not None:
+				self._source._subgraph._edgesWithoutID.remove(self)
+		else:
+			del self._source._graph._edgesWithID[self._id]
+			if self._source._subgraph is not None:
+				del self._source._subgraph._edgesWithID[self]
+
+		self._Delete()
+
+	def _Delete(self) -> None:
+		super().Delete()
+
 	def Reverse(self) -> None:
 		"""Reverse the direction of this edge."""
 		self._source._outboundEdges.remove(self)
 		self._source._inboundEdges.append(self)
 		self._destination._inboundEdges.remove(self)
 		self._destination._outboundEdges.append(self)
 
@@ -1498,15 +1681,18 @@
 ):
 	"""
 	A **link** can have a unique ID, a value, a weight and attached meta information as key-value-pairs. All links are
 	directed.
 	"""
 
 	def __init__(self, source: Vertex, destination: Vertex, linkID: LinkIDType = None, value: LinkValueType = None, weight: LinkWeightType = None):
-		""".. todo:: GRAPH::Edge::init Needs documentation."""
+		"""
+		.. todo:: GRAPH::Edge::init Needs documentation.
+
+		"""
 		if not isinstance(source, Vertex):
 			raise TypeError("Parameter 'source' is not of type 'Vertex'.")
 		if not isinstance(destination, Vertex):
 			raise TypeError("Parameter 'destination' is not of type 'Vertex'.")
 		if linkID is not None and not isinstance(linkID, Hashable):
 			raise TypeError("Parameter 'edgeID' is not of type 'EdgeIDType'.")
 		# if value is not None and  not isinstance(value, Vertex):
@@ -1514,14 +1700,29 @@
 		if weight is not None and not isinstance(weight, (int, float)):
 			raise TypeError("Parameter 'weight' is not of type 'EdgeWeightType'.")
 		if source._graph is not destination._graph:
 			raise NotInSameGraph(f"Source vertex and destination vertex are not in same graph.")
 
 		super().__init__(source, destination, linkID, value, weight)
 
+	def Delete(self) -> None:
+		self._source._outboundEdges.remove(self)
+		self._destination._inboundEdges.remove(self)
+
+		if self._id is None:
+			self._source._graph._linksWithoutID.remove(self)
+		else:
+			del self._source._graph._linksWithID[self._id]
+
+		self._Delete()
+		assert getrefcount(self) == 1
+
+	def _Delete(self) -> None:
+		super().Delete()
+
 	def Reverse(self) -> None:
 		"""Reverse the direction of this link."""
 		self._source._outboundEdges.remove(self)
 		self._source._inboundEdges.append(self)
 		self._destination._inboundEdges.remove(self)
 		self._destination._outboundEdges.append(self)
 
@@ -1534,44 +1735,54 @@
 	Generic[
 		GraphDictKeyType, GraphDictValueType,
 		VertexIDType, VertexWeightType, VertexValueType, VertexDictKeyType, VertexDictValueType,
 		EdgeIDType, EdgeWeightType, EdgeValueType, EdgeDictKeyType, EdgeDictValueType,
 		LinkIDType, LinkWeightType, LinkValueType, LinkDictKeyType, LinkDictValueType
 	]
 ):
-	""".. todo:: GRAPH::BaseGraph Needs documentation."""
+	"""
+	.. todo:: GRAPH::BaseGraph Needs documentation.
+
+	"""
 
 	_verticesWithID:    Dict[VertexIDType, Vertex[GraphDictKeyType, GraphDictValueType, VertexIDType, VertexWeightType, VertexValueType, VertexDictKeyType, VertexDictValueType, EdgeIDType, EdgeWeightType, EdgeValueType, EdgeDictKeyType, EdgeDictValueType, LinkIDType, LinkWeightType, LinkValueType, LinkDictKeyType, LinkDictValueType]]
 	_verticesWithoutID: List[Vertex[GraphDictKeyType, GraphDictValueType, VertexIDType, VertexWeightType, VertexValueType, VertexDictKeyType, VertexDictValueType, EdgeIDType, EdgeWeightType, EdgeValueType, EdgeDictKeyType, EdgeDictValueType, LinkIDType, LinkWeightType, LinkValueType, LinkDictKeyType, LinkDictValueType]]
 	_edgesWithID:       Dict[EdgeIDType, Edge[EdgeIDType, EdgeWeightType, EdgeValueType, EdgeDictKeyType, EdgeDictValueType]]
 	_edgesWithoutID:    List[Edge[EdgeIDType, EdgeWeightType, EdgeValueType, EdgeDictKeyType, EdgeDictValueType]]
 	_linksWithID:       Dict[EdgeIDType, Link[LinkIDType, LinkWeightType, LinkValueType, LinkDictKeyType, LinkDictValueType]]
 	_linksWithoutID:    List[Link[LinkIDType, LinkWeightType, LinkValueType, LinkDictKeyType, LinkDictValueType]]
 
 	def __init__(self, name: str = None):  #, vertices: Iterable[Vertex] = None):
-		""".. todo:: GRAPH::BaseGraph::init Needs documentation."""
+		"""
+		.. todo:: GRAPH::BaseGraph::init Needs documentation.
+
+		"""
 		super().__init__(name)
 
 		self._verticesWithoutID = []
 		self._verticesWithID = {}
 		self._edgesWithoutID = []
 		self._edgesWithID = {}
 		self._linksWithoutID = []
 		self._linksWithID = {}
 
 	def __del__(self):
-		""".. todo:: GRAPH::BaseGraph::del Needs documentation."""
-		super().__del__()
+		"""
+		.. todo:: GRAPH::BaseGraph::del Needs documentation.
+
+		"""
 		del self._verticesWithoutID
 		del self._verticesWithID
 		del self._edgesWithoutID
 		del self._edgesWithID
 		del self._linksWithoutID
 		del self._linksWithID
 
+		super().__del__()
+
 	@property
 	def VertexCount(self) -> int:
 		"""Read-only property to access the number of vertices in this graph.
 
 		:returns: The number of vertices in this graph."""
 		return len(self._verticesWithoutID) + len(self._verticesWithID)
 
@@ -1618,19 +1829,19 @@
 		If parameter ``predicate`` is not None, the given filter function is used to skip vertices in the generator.
 
 		:param predicate: Filter function accepting any vertex and returning a boolean.
 		:returns:         A generator to iterate all vertices without inbound edges.
 
 		.. seealso::
 
-		   :py:meth:`IterateLeafs` |br|
+		   :meth:`IterateLeafs` |br|
 		      |rarr| Iterate leafs of a graph.
-		   :py:meth:`Vertex.IsRoot <pyTooling.Graph.Vertex.IsRoot>` |br|
+		   :meth:`Vertex.IsRoot <pyTooling.Graph.Vertex.IsRoot>` |br|
 		      |rarr| Check if a vertex is a root vertex in the graph.
-		   :py:meth:`Vertex.IsLeaf <pyTooling.Graph.Vertex.IsLeaf>` |br|
+		   :meth:`Vertex.IsLeaf <pyTooling.Graph.Vertex.IsLeaf>` |br|
 		      |rarr| Check if a vertex is a leaf vertex in the graph.
 		"""
 		if predicate is None:
 			for vertex in self._verticesWithoutID:
 				if len(vertex._inboundEdges) == 0:
 					yield vertex
 
@@ -1653,19 +1864,19 @@
 		If parameter ``predicate`` is not None, the given filter function is used to skip vertices in the generator.
 
 		:param predicate: Filter function accepting any vertex and returning a boolean.
 		:returns:         A generator to iterate all vertices without outbound edges.
 
 		.. seealso::
 
-		   :py:meth:`IterateRoots` |br|
+		   :meth:`IterateRoots` |br|
 		      |rarr| Iterate roots of a graph.
-		   :py:meth:`Vertex.IsRoot <pyTooling.Graph.Vertex.IsRoot>` |br|
+		   :meth:`Vertex.IsRoot <pyTooling.Graph.Vertex.IsRoot>` |br|
 		      |rarr| Check if a vertex is a root vertex in the graph.
-		   :py:meth:`Vertex.IsLeaf <pyTooling.Graph.Vertex.IsLeaf>` |br|
+		   :meth:`Vertex.IsLeaf <pyTooling.Graph.Vertex.IsLeaf>` |br|
 		      |rarr| Check if a vertex is a leaf vertex in the graph.
 		"""
 		if predicate is None:
 			for vertex in self._verticesWithoutID:
 				if len(vertex._outboundEdges) == 0:
 					yield vertex
 
@@ -1872,18 +2083,18 @@
 
 		If parameter ``predicate`` is not None, the given filter function is used to skip edges.
 
 		:param predicate: Filter function accepting any edge and returning a boolean.
 		"""
 		if predicate is None:
 			for edge in self._edgesWithoutID:
-				del edge
+				edge._Delete()
 
 			for edge in self._edgesWithID.values():
-				del edge
+				edge._Delete()
 
 			self._edgesWithoutID = []
 			self._edgesWithID = {}
 
 			for vertex in self._verticesWithoutID:
 				vertex._inboundEdges = []
 				vertex._outboundEdges = []
@@ -1895,38 +2106,38 @@
 		else:
 			delEdges = [edge for edge in self._edgesWithID.values() if predicate(edge)]
 			for edge in delEdges:
 				del self._edgesWithID[edge._id]
 
 				edge._source._outboundEdges.remove(edge)
 				edge._destination._inboundEdges.remove(edge)
-				del edge
+				edge._Delete()
 
 			for edge in self._edgesWithoutID:
 				if predicate(edge):
 					self._edgesWithoutID.remove(edge)
 
 					edge._source._outboundEdges.remove(edge)
 					edge._destination._inboundEdges.remove(edge)
-					del edge
+					edge._Delete()
 
 	def RemoveLinks(self, predicate: Callable[[Link], bool] = None):
 		"""
 		Remove all or selected links of a graph.
 
 		If parameter ``predicate`` is not None, the given filter function is used to skip links.
 
 		:param predicate: Filter function accepting any link and returning a boolean.
 		"""
 		if predicate is None:
 			for link in self._linksWithoutID:
-				del link
+				link._Delete()
 
 			for link in self._linksWithID.values():
-				del link
+				link._Delete()
 
 			self._linksWithoutID = []
 			self._linksWithID = {}
 
 			for vertex in self._verticesWithoutID:
 				vertex._inboundLinks = []
 				vertex._outboundLinks = []
@@ -1938,26 +2149,29 @@
 		else:
 			delLinks = [link for link in self._linksWithID.values() if predicate(link)]
 			for link in delLinks:
 				del self._linksWithID[link._id]
 
 				link._source._outboundLinks.remove(link)
 				link._destination._inboundLinks.remove(link)
-				del link
+				link._Delete()
 
 			for link in self._linksWithoutID:
 				if predicate(link):
 					self._linksWithoutID.remove(link)
 
 					link._source._outboundLinks.remove(link)
 					link._destination._inboundLinks.remove(link)
-					del link
+					link._Delete()
 
 	def HasCycle(self) -> bool:
-		""".. todo:: GRAPH::BaseGraph::HasCycle Needs documentation."""
+		"""
+		.. todo:: GRAPH::BaseGraph::HasCycle Needs documentation.
+
+		"""
 		# IsAcyclic ?
 
 		# Handle trivial case if graph is empty
 		if len(self._verticesWithID) + len(self._verticesWithoutID) == 0:
 			return False
 
 		outboundEdgeCounts = {}
@@ -2013,46 +2227,58 @@
 	Generic[
 		SubgraphDictKeyType, SubgraphDictValueType,
 		VertexIDType, VertexWeightType, VertexValueType, VertexDictKeyType, VertexDictValueType,
 		EdgeIDType, EdgeWeightType, EdgeValueType, EdgeDictKeyType, EdgeDictValueType,
 		LinkIDType, LinkWeightType, LinkValueType, LinkDictKeyType, LinkDictValueType
 	]
 ):
-	""".. todo:: GRAPH::Subgraph Needs documentation."""
+	"""
+	.. todo:: GRAPH::Subgraph Needs documentation.
+
+	"""
 
 	_graph:    'Graph'
 
 	def __init__(self, graph: 'Graph', name: str = None, vertices: Iterable[Vertex] = None):
-		""".. todo:: GRAPH::Subgraph::init Needs documentation."""
+		"""
+		.. todo:: GRAPH::Subgraph::init Needs documentation.
+
+		"""
 		if graph is None:
 			raise ValueError("Parameter 'graph' is None.")
 		if not isinstance(graph, Graph):
 			raise TypeError("Parameter 'graph' is not of type 'Graph'.")
 
 		super().__init__(name)
 
 		graph._subgraphs.add(self)
 
 		self._graph = graph
 
 	def __del__(self):
-		""".. todo:: GRAPH::Subgraph::del Needs documentation."""
+		"""
+		.. todo:: GRAPH::Subgraph::del Needs documentation.
+
+		"""
 		super().__del__()
 
 	@property
 	def Graph(self) -> 'Graph':
 		"""
-		Read-only property to access the graph, this subgraph is associated to (:py:attr:`_graph`).
+		Read-only property to access the graph, this subgraph is associated to (:attr:`_graph`).
 
 		:returns: The graph this subgraph is associated to.
 		"""
 		return self._graph
 
 	def __str__(self) -> str:
-		""".. todo:: GRAPH::Subgraph::str Needs documentation."""
+		"""
+		.. todo:: GRAPH::Subgraph::str Needs documentation.
+
+		"""
 		return self._name if self._name is not None else "Unnamed subgraph"
 
 
 @export
 class View(
 	BaseWithVertices[
 		ViewDictKeyType, ViewDictValueType,
@@ -2065,28 +2291,40 @@
 		ViewDictKeyType, ViewDictValueType,
 		GraphDictKeyType, GraphDictValueType,
 		VertexIDType, VertexWeightType, VertexValueType, VertexDictKeyType, VertexDictValueType,
 		EdgeIDType, EdgeWeightType, EdgeValueType, EdgeDictKeyType, EdgeDictValueType,
 		LinkIDType, LinkWeightType, LinkValueType, LinkDictKeyType, LinkDictValueType
 	]
 ):
-	""".. todo:: GRAPH::View Needs documentation."""
+	"""
+	.. todo:: GRAPH::View Needs documentation.
+
+	"""
 
 	def __init__(self, graph: 'Graph', name: str = None, vertices: Iterable[Vertex] = None):
-		""".. todo:: GRAPH::View::init Needs documentation."""
+		"""
+		.. todo:: GRAPH::View::init Needs documentation.
+
+		"""
 		super().__init__(graph, name, vertices)
 
 		graph._views.add(self)
 
 	def __del__(self):
-		""".. todo:: GRAPH::View::del Needs documentation."""
+		"""
+		.. todo:: GRAPH::View::del Needs documentation.
+
+		"""
 		super().__del__()
 
 	def __str__(self) -> str:
-		""".. todo:: GRAPH::View::str Needs documentation."""
+		"""
+		.. todo:: GRAPH::View::str Needs documentation.
+
+		"""
 		return self._name if self._name is not None else "Unnamed view"
 
 
 @export
 class Component(
 	BaseWithVertices[
 		ComponentDictKeyType, ComponentDictValueType,
@@ -2099,28 +2337,40 @@
 		ComponentDictKeyType, ComponentDictValueType,
 		GraphDictKeyType, GraphDictValueType,
 		VertexIDType, VertexWeightType, VertexValueType, VertexDictKeyType, VertexDictValueType,
 		EdgeIDType, EdgeWeightType, EdgeValueType, EdgeDictKeyType, EdgeDictValueType,
 		LinkIDType, LinkWeightType, LinkValueType, LinkDictKeyType, LinkDictValueType
 	]
 ):
-	""".. todo:: GRAPH::Component Needs documentation."""
+	"""
+	.. todo:: GRAPH::Component Needs documentation.
+
+	"""
 
 	def __init__(self, graph: 'Graph', name: str = None, vertices: Iterable[Vertex] = None):
-		""".. todo:: GRAPH::Component::init Needs documentation."""
+		"""
+		.. todo:: GRAPH::Component::init Needs documentation.
+
+		"""
 		super().__init__(graph, name, vertices)
 
 		graph._components.add(self)
 
 	def __del__(self):
-		""".. todo:: GRAPH::Component::del Needs documentation."""
+		"""
+		.. todo:: GRAPH::Component::del Needs documentation.
+
+		"""
 		super().__del__()
 
 	def __str__(self) -> str:
-		""".. todo:: GRAPH::Component::str Needs documentation."""
+		"""
+		.. todo:: GRAPH::Component::str Needs documentation.
+
+		"""
 		return self._name if self._name is not None else "Unnamed component"
 
 
 @export
 class Graph(
 	BaseGraph[
 		GraphDictKeyType, GraphDictValueType,
@@ -2135,54 +2385,61 @@
 		ViewDictKeyType, ViewDictValueType,
 		VertexIDType, VertexWeightType, VertexValueType, VertexDictKeyType, VertexDictValueType,
 		EdgeIDType, EdgeWeightType, EdgeValueType, EdgeDictKeyType, EdgeDictValueType,
 		LinkIDType, LinkWeightType, LinkValueType, LinkDictKeyType, LinkDictValueType
 	]
 ):
 	"""
-	A **graph** data structure is represented by an instance of :py:class:`~pyTooling.Graph.Graph` holding references to
-	all nodes. Nodes are instances of :py:class:`~pyTooling.Graph.Vertex` classes and directed links between nodes are
-	made of :py:class:`~pyTooling.Graph.Edge` instances. A graph can have attached meta information as key-value-pairs.
+	A **graph** data structure is represented by an instance of :class:`~pyTooling.Graph.Graph` holding references to
+	all nodes. Nodes are instances of :class:`~pyTooling.Graph.Vertex` classes and directed links between nodes are
+	made of :class:`~pyTooling.Graph.Edge` instances. A graph can have attached meta information as key-value-pairs.
 	"""
 	_subgraphs:         Set[Subgraph[SubgraphDictKeyType, SubgraphDictValueType, VertexIDType, VertexWeightType, VertexValueType, VertexDictKeyType, VertexDictValueType, EdgeIDType, EdgeWeightType, EdgeValueType, EdgeDictKeyType, EdgeDictValueType, LinkIDType, LinkWeightType, LinkValueType, LinkDictKeyType, LinkDictValueType]]
 	_views:             Set[View[ViewDictKeyType, ViewDictValueType, GraphDictKeyType, GraphDictValueType, VertexIDType, VertexWeightType, VertexValueType, VertexDictKeyType, VertexDictValueType, EdgeIDType, EdgeWeightType, EdgeValueType, EdgeDictKeyType, EdgeDictValueType, LinkIDType, LinkWeightType, LinkValueType, LinkDictKeyType, LinkDictValueType]]
 	_components:        Set[Component[ComponentDictKeyType, ComponentDictValueType, GraphDictKeyType, GraphDictValueType, VertexIDType, VertexWeightType, VertexValueType, VertexDictKeyType, VertexDictValueType, EdgeIDType, EdgeWeightType, EdgeValueType, EdgeDictKeyType, EdgeDictValueType, LinkIDType, LinkWeightType, LinkValueType, LinkDictKeyType, LinkDictValueType]]
 
 	def __init__(self, name: str = None):
-		""".. todo:: GRAPH::Graph::init Needs documentation."""
+		"""
+		.. todo:: GRAPH::Graph::init Needs documentation.
+
+		"""
 		super().__init__(name)
 
 		self._subgraphs = set()
 		self._views = set()
 		self._components = set()
 
 	def __del__(self):
-		""".. todo:: GRAPH::Graph::del Needs documentation."""
-		super().__del__()
+		"""
+		.. todo:: GRAPH::Graph::del Needs documentation.
+
+		"""
 		del self._subgraphs
 		del self._views
 		del self._components
 
+		super().__del__()
+
 	@property
 	def Subgraphs(self) -> Set[Subgraph]:
-		"""Read-only property to access the subgraphs in this graph (:py:attr:`_subgraphs`).
+		"""Read-only property to access the subgraphs in this graph (:attr:`_subgraphs`).
 
 		:returns: The set of subgraphs in this graph."""
 		return self._subgraphs
 
 	@property
 	def Views(self) -> Set[View]:
-		"""Read-only property to access the views in this graph (:py:attr:`_views`).
+		"""Read-only property to access the views in this graph (:attr:`_views`).
 
 		:returns: The set of views in this graph."""
 		return self._views
 
 	@property
 	def Components(self) -> Set[Component]:
-		"""Read-only property to access the components in this graph (:py:attr:`_components`).
+		"""Read-only property to access the components in this graph (:attr:`_components`).
 
 		:returns: The set of components in this graph."""
 		return self._components
 
 	@property
 	def SubgraphCount(self) -> int:
 		"""Read-only property to access the number of subgraphs in this graph.
@@ -2201,20 +2458,53 @@
 	def ComponentCount(self) -> int:
 		"""Read-only property to access the number of components in this graph.
 
 		:returns: The number of components in this graph."""
 		return len(self._components)
 
 	def __iter__(self) -> typing_Iterator[Vertex[GraphDictKeyType, GraphDictValueType, VertexIDType, VertexWeightType, VertexValueType, VertexDictKeyType, VertexDictValueType, EdgeIDType, EdgeWeightType, EdgeValueType, EdgeDictKeyType, EdgeDictValueType, LinkIDType, LinkWeightType, LinkValueType, LinkDictKeyType, LinkDictValueType]]:
-		""".. todo:: GRAPH::Graph::iter Needs documentation."""
+		"""
+		.. todo:: GRAPH::Graph::iter Needs documentation.
+
+		"""
 		def gen():
 			yield from self._verticesWithoutID
 			yield from self._verticesWithID
 		return iter(gen())
 
+	def GetVertexByID(self, vertexID: Nullable[VertexIDType]) -> Vertex:
+		"""
+		.. todo:: GRAPH::Graph::GetVertexByID Needs documentation.
+
+		"""
+		if vertexID is None:
+			if len(self._verticesWithoutID) > 1:
+				raise KeyError(f"Found multiple vertices with ID `None`.")
+			else:
+				try:
+					return self._verticesWithoutID[0]
+				except IndexError:
+					raise KeyError(f"Found no vertex with ID `None`.")
+		else:
+			return self._verticesWithID[vertexID]
+
+	def GetVertexByValue(self, value) -> Vertex:
+		"""
+		.. todo:: GRAPH::Graph::GetVertexByValue Needs documentation.
+
+		"""
+		vertices = [vertex for vertex in chain(self._verticesWithID.values(), self._verticesWithoutID) if vertex._value == value]
+		if len(vertices) > 1:
+			raise KeyError(f"Found multiple vertices with Value == `{value}`.")
+		else:
+			try:
+				return vertices[0]
+			except IndexError:
+				raise KeyError(f"Found no vertex with Value == `{value}`.")
+
 	def CopyGraph(self) -> 'Graph':
 		raise NotImplementedError()
 
 	def CopyVertices(self, predicate: Callable[[Vertex], bool] = None, copyGraphDict: bool = True, copyVertexDict: bool = True) -> 'Graph':
 		"""
 		Create a new graph and copy all or selected vertices of the original graph.
 
@@ -2282,20 +2572,26 @@
 	# def MinimumSpanningTree(self):
 	# 	raise NotImplementedError()
 	# 	# Kruskal
 	# 	# Prim's algorithm
 	# 	# Buruvka's algorithm
 
 	def __repr__(self) -> str:
-		""".. todo:: GRAPH::Graph::repr Needs documentation."""
+		"""
+		.. todo:: GRAPH::Graph::repr Needs documentation.
+
+		"""
 		statistics = f", vertices: {self.VertexCount}, edges: {self.EdgeCount}"
 		if self._name is None:
 			return f"<graph: unnamed graph{statistics}>"
 		else:
 			return f"<graph: '{self._name}'{statistics}>"
 
 	def __str__(self) -> str:
-		""".. todo:: GRAPH::Graph::str Needs documentation."""
+		"""
+		.. todo:: GRAPH::Graph::str Needs documentation.
+
+		"""
 		if self._name is None:
 			return f"Graph: unnamed graph"
 		else:
 			return f"Graph: '{self._name}'"
```

### Comparing `pyTooling-4.0.1/pyTooling/Licensing/__init__.py` & `pyTooling-5.0.0/pyTooling/Licensing/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -70,15 +70,15 @@
 
 	"SPDX_INDEX"
 ]
 
 
 @export
 @dataclass
-class PythonLicenseNames:
+class PythonLicenseName:
 	"""A *data class* to represent the license's short name and the package classifier for a license."""
 
 	ShortName: str    #: License's short name
 	Classifier: str   #: Package classifier for a license.
 
 	def __str__(self) -> str:
 		"""
@@ -86,24 +86,24 @@
 
 		:returns: Short name of the license.
 		"""
 		return self.ShortName
 
 
 #: Mapping of SPDX identifiers to Python license names
-PYTHON_LICENSE_NAMES: Dict[str, PythonLicenseNames] = {
-	"Apache-2.0":       PythonLicenseNames("Apache 2.0",       "Apache Software License"),
-	"BSD-3-Clause":     PythonLicenseNames("BSD",              "BSD License"),
-	"MIT":              PythonLicenseNames("MIT",              "MIT License"),
-	"GPL-2.0-or-later": PythonLicenseNames("GPL-2.0-or-later", "GNU General Public License v2 or later (GPLv2+)"),
+PYTHON_LICENSE_NAMES: Dict[str, PythonLicenseName] = {
+	"Apache-2.0":       PythonLicenseName("Apache 2.0",       "Apache Software License"),
+	"BSD-3-Clause":     PythonLicenseName("BSD",              "BSD License"),
+	"MIT":              PythonLicenseName("MIT",              "MIT License"),
+	"GPL-2.0-or-later": PythonLicenseName("GPL-2.0-or-later", "GNU General Public License v2 or later (GPLv2+)"),
 }
 
 
 @export
-class License(metaclass=ExtendedType, useSlots=True):
+class License(metaclass=ExtendedType, slots=True):
 	"""Representation of a license."""
 
 	_spdxIdentifier: str  #: Unique SPDX identifier.
 	_name: str            #: Name of the license.
 	_osiApproved: bool    #: OSI approval status
 	_fsfApproved: bool    #: FSF approval status
 
@@ -151,61 +151,61 @@
 
 	@property
 	def PythonLicenseName(self) -> str:
 		"""
 		Returns the Python license name for this license if it's defined.
 
 		:returns: The Python license name.
-		:raises ValueError: If there is no license name defined for the license. |br| (See and check :py:data:`~pyTooling.Licensing.PYTHON_LICENSE_NAMES`)
+		:raises ValueError: If there is no license name defined for the license. |br| (See and check :data:`~pyTooling.Licensing.PYTHON_LICENSE_NAMES`)
 		"""
 		try:
-			item: PythonLicenseNames = PYTHON_LICENSE_NAMES[self._spdxIdentifier]
+			item: PythonLicenseName = PYTHON_LICENSE_NAMES[self._spdxIdentifier]
 		except KeyError as ex:
 			raise ValueError("License has no Python specify information.") from ex
 
 		return item.ShortName
 
 	@property
 	def PythonClassifier(self) -> str:
 		"""
 		Returns the Python package classifier for this license if it's defined.
 
 		:returns: The Python package classifier.
-		:raises ValueError: If there is no classifier defined for the license. |br| (See and check :py:data:`~pyTooling.Licensing.PYTHON_LICENSE_NAMES`)
+		:raises ValueError: If there is no classifier defined for the license. |br| (See and check :data:`~pyTooling.Licensing.PYTHON_LICENSE_NAMES`)
 
 		.. seealso::
 
 		   List of `Python classifiers <https://pypi.org/classifiers/>`__
 		"""
 		try:
-			item: PythonLicenseNames = PYTHON_LICENSE_NAMES[self._spdxIdentifier]
+			item: PythonLicenseName = PYTHON_LICENSE_NAMES[self._spdxIdentifier]
 		except KeyError as ex:
 			raise ValueError(f"License has no Python specify information.") from ex
 
 		osi = "OSI Approved :: " if self._osiApproved else ""
 		return f"License :: {osi}{item.Classifier}"
 
 	def __eq__(self, other: Any) -> bool:
 		"""
 		Returns true, if both licenses are identical (comparison based on SPDX identifiers).
 
 		:returns:          ``True``, if both licenses are identical.
-		:raises TypeError: If second operand is not of type :py:class:`License`.
+		:raises TypeError: If second operand is not of type :class:`License` or :class:`str`.
 		"""
 		if isinstance(other, License):
 			return self._spdxIdentifier == other._spdxIdentifier
 		else:
 			raise TypeError(f"Second operand of type '{other.__class__.__name__}' is not supported by equal operator.")
 
 	def __ne__(self, other: Any) -> bool:
 		"""
 		Returns true, if both licenses are not identical (comparison based on SPDX identifiers).
 
 		:returns:          ``True``, if both licenses are not identical.
-		:raises TypeError: If second operand is not of type :py:class:`License`.
+		:raises TypeError: If second operand is not of type :class:`License` or :class:`str`.
 		"""
 		if isinstance(other, License):
 			return self._spdxIdentifier != other._spdxIdentifier
 		else:
 			raise TypeError(f"Second operand of type '{other.__class__.__name__}' is not supported by unequal operator.")
 
 	def __le__(self, other: Any) -> bool:
```

### Comparing `pyTooling-4.0.1/pyTooling/Packaging/__init__.py` & `pyTooling-5.0.0/pyTooling/Packaging/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -128,15 +128,15 @@
 
 				requirements.append(line)
 
 	return requirements
 
 
 @export
-class VersionInformation(metaclass=ExtendedType, useSlots=True):
+class VersionInformation(metaclass=ExtendedType, slots=True):
 	"""Encapsulates version information extracted from a Python source file."""
 
 	_author: str          #: Author name(s).
 	_copyright: str       #: Copyright information.
 	_email: str           #: Author's email address.
 	_keywords: List[str]  #: Keywords.
 	_license: str         #: License name.
```

### Comparing `pyTooling-4.0.1/pyTooling/TerminalUI/__init__.py` & `pyTooling-5.0.0/pyTooling/TerminalUI/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,19 +32,19 @@
 """A set of helpers to implement a text user interface (TUI) in a terminal."""
 
 from enum                   import Enum, unique
 from platform               import system as platform_system
 from typing                 import NoReturn, Tuple, Any
 
 from pyTooling.Decorators   import export
-from pyTooling.MetaClasses  import ExtendedType
+from pyTooling.MetaClasses  import ExtendedType, mixin
 
 
 @export
-class Terminal(metaclass=ExtendedType, useSlots=True, singleton=True):
+class Terminal(metaclass=ExtendedType, singleton=True):
 	FATAL_EXIT_CODE = 255
 
 	try:
 		from colorama import Fore as Foreground
 		Foreground = {
 			"RED":          Foreground.LIGHTRED_EX,
 			"DARK_RED":		  Foreground.RED,
@@ -419,14 +419,15 @@
 
 	def __str__(self) -> str:
 		"""Returns a formatted version of a ``Line`` objects as a string."""
 		return self._LOG_MESSAGE_FORMAT__[self._severity].format(message=self._message)
 
 
 @export
+@mixin
 class ILineTerminal:
 	"""A mixin class (interface) to provide class-local terminal writing methods."""
 
 	_terminal: Terminal
 
 	def __init__(self, terminal: Terminal = None):
 		"""MixIn initializer."""
```

### Comparing `pyTooling-4.0.1/pyTooling/Timer/__init__.py` & `pyTooling-5.0.0/pyTooling/Timer/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,35 +33,37 @@
 
 .. hint:: See :ref:`high-level help <TIMER>` for explanations and usage examples.
 """
 from time import perf_counter_ns
 from typing import List, Optional as Nullable, Dict
 
 from pyTooling.Decorators import export
-from pyTooling.MetaClasses import ObjectWithSlots
+from pyTooling.MetaClasses import SlottedObject
 
 
 @export
-class Timer(ObjectWithSlots):
+class Timer(SlottedObject):
 	"""
 	Undocumented.
 
 	.. todo::TIMER::Timer Needs class documentation.
 	"""
 
-	_timers: Dict[str, 'Timer'] = {}
+	_timers: Dict[str, 'Timer']
 
 	_startTime: Nullable[int]
 	_resumeTime: Nullable[int]
 	_pauseTime: int
 	_stopTime: int
 	_diffTime: int
 	_diffTimes: List[int]
 
 	def __init__(self):
+		self._timers = {}
+
 		self._startTime = None
 		self._resumeTime = None
 		self._diffTimes = []
 
 	def __enter__(self):
 		self.Start()
 		return self
```

### Comparing `pyTooling-4.0.1/pyTooling/Tree/__init__.py` & `pyTooling-5.0.0/pyTooling/Tree/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 
 DictValueType = TypeVar("DictValueType")
 """A type variable for a tree's dictionary values."""
 
 
 @export
 class TreeException(ToolingException):
-	"""Base exception of all exceptions raised by :py:mod:`pyTooling.Tree`."""
+	"""Base exception of all exceptions raised by :mod:`pyTooling.Tree`."""
 
 
 @export
 class InternalError(TreeException):
 	"""
 	The exception is raised when a data structure corruption is detected.
 
@@ -93,50 +93,50 @@
 
 @export
 class NotInSameTreeError(TreeException):
 	"""The exception is raised when the current node and the other node are not in the same tree."""
 
 
 @export
-class Node(Generic[IDType, ValueType, DictKeyType, DictValueType], metaclass=ExtendedType, useSlots=True):
+class Node(Generic[IDType, ValueType, DictKeyType, DictValueType], metaclass=ExtendedType, slots=True):
 	"""
 	A **tree** data structure can be constructed of ``Node`` instances.
 
 	Therefore, nodes can be connected to parent nodes or a parent node can add child nodes. This allows to construct a
 	tree top-down or bottom-up.
 
 	.. hint:: The top-down construction should be preferred, because it's slightly faster.
 
 	Each tree uses the **root** node (a.k.a. tree-representative) to store some per-tree data structures. E.g. a list of
 	all IDs in a tree. For easy and quick access to such data structures, each sibling node contains a reference to the
-	root node (:py:attr:`_root`). In case of adding a tree to an existing tree, such data structures get merged and all added
-	nodes get assigned with new root references. Use the read-only property :py:attr:`Root` to access the root reference.
+	root node (:attr:`_root`). In case of adding a tree to an existing tree, such data structures get merged and all added
+	nodes get assigned with new root references. Use the read-only property :attr:`Root` to access the root reference.
 
-	The reference to the parent node (:py:attr:`_parent`) can be access via property :py:attr:`Parent`. If the property's setter
+	The reference to the parent node (:attr:`_parent`) can be access via property :attr:`Parent`. If the property's setter
 	is used, a node and all its siblings are added to another tree or to a new position in the same tree.
 
-	The references to all node's children is stored in a list (:py:attr:`_children`). Children, siblings, ancestors, can be
+	The references to all node's children is stored in a list (:attr:`_children`). Children, siblings, ancestors, can be
 	accessed via various generators:
 
-	* :py:meth:`GetAncestors` |rarr| iterate all ancestors bottom-up.
-	* :py:meth:`GetChildren` |rarr| iterate all direct children.
-	* :py:meth:`GetDescendants` |rarr| iterate all descendants.
-	* :py:meth:`IterateLevelOrder` |rarr| IterateLevelOrder.
-	* :py:meth:`IteratePreOrder` |rarr| iterate siblings in pre-order.
-	* :py:meth:`IteratePostOrder` |rarr| iterate siblings in post-order.
+	* :meth:`GetAncestors` |rarr| iterate all ancestors bottom-up.
+	* :meth:`GetChildren` |rarr| iterate all direct children.
+	* :meth:`GetDescendants` |rarr| iterate all descendants.
+	* :meth:`IterateLevelOrder` |rarr| IterateLevelOrder.
+	* :meth:`IteratePreOrder` |rarr| iterate siblings in pre-order.
+	* :meth:`IteratePostOrder` |rarr| iterate siblings in post-order.
 
 	Each node can have a **unique ID** or no ID at all (``nodeID=None``). The root node is used to store all IDs in a
-	dictionary (:py:attr:`_nodesWithID`). In case no ID is given, all such ID-less nodes are collected in a single bin and store as a
-	list of nodes. An ID can be modified after the Node was created. Use the read-only property :py:attr:`ID` to access
+	dictionary (:attr:`_nodesWithID`). In case no ID is given, all such ID-less nodes are collected in a single bin and store as a
+	list of nodes. An ID can be modified after the Node was created. Use the read-only property :attr:`ID` to access
 	the ID.
 
-	Each node can have a **value** (:py:attr:`_value`), which can be given at node creation time, or it can be assigned and/or
-	modified later. Use the property :py:attr:`Value` to get or set the value.
+	Each node can have a **value** (:attr:`_value`), which can be given at node creation time, or it can be assigned and/or
+	modified later. Use the property :attr:`Value` to get or set the value.
 
-	Moreover, each node can store various key-value-pairs (:py:attr:`_dict`). Use the dictionary syntax to get and set
+	Moreover, each node can store various key-value-pairs (:attr:`_dict`). Use the dictionary syntax to get and set
 	key-value-pairs.
 	"""
 
 	_id: Nullable[IDType]                         #: Unique identifier of a node. ``None`` if not used.
 	_nodesWithID: Nullable[Dict[IDType, 'Node']]  #: Dictionary of all IDs in the tree. ``None`` if it's not the root node.
 	_nodesWithoutID: Nullable[List['Node']]       #: List of all nodes without an ID in the tree. ``None`` if it's not the root node.
 	_root: 'Node'                                 #: Reference to the root of a tree. ``self`` if it's the root node.
@@ -145,15 +145,18 @@
 #	_links: List['Node']
 
 	_level: int                                   #: Level of the node (distance to the root).
 	_value: Nullable[ValueType]                   #: Field to store the node's value.
 	_dict: Dict[DictKeyType, DictValueType]       #: Dictionary to store key-value-pairs attached to the node.
 
 	def __init__(self, nodeID: IDType = None, value: ValueType = None, parent: 'Node' = None, children: List['Node'] = None):
-		""".. todo:: TREE::Node::init Needs documentation."""
+		"""
+		.. todo:: TREE::Node::init Needs documentation.
+
+		"""
 		self._id = nodeID
 		self._value = value
 		self._dict = {}
 
 		if parent is not None and not isinstance(parent, Node):
 			raise TypeError(f"Parameter 'parent' is not of type 'Node'.")
 
@@ -194,26 +197,26 @@
 					raise TypeError(f"Item '{child}' in parameter 'children' is not of type 'Node'.")
 
 				child.Parent = self
 
 	@property
 	def ID(self) -> Nullable[IDType]:
 		"""
-		Read-only property to access the unique ID of a node (:py:attr:`_id`).
+		Read-only property to access the unique ID of a node (:attr:`_id`).
 
 		If no ID was given at node construction time, ID return None.
 
 		:returns: Unique ID of a node, if ID was given at node creation time, else None.
 		"""
 		return self._id
 
 	@property
 	def Value(self) -> Nullable[ValueType]:
 		"""
-		Property to get and set the value (:py:attr:`_value`) of a node.
+		Property to get and set the value (:attr:`_value`) of a node.
 
 		:returns: The value of a node.
 		"""
 		return self._value
 
 	@Value.setter
 	def Value(self, value: Nullable[ValueType]) -> None:
@@ -236,50 +239,56 @@
 
 		:param key:   The key to create or update.
 		:param value: The value to associate to the given key.
 		"""
 		self._dict[key] = value
 
 	def __delitem__(self, key: DictKeyType) -> None:
-		""".. todo:: TREE::Node::__delitem__ Needs documentation."""
+		"""
+		.. todo:: TREE::Node::__delitem__ Needs documentation.
+
+		"""
 		del self._dict[key]
 
 	def __contains__(self, key: DictKeyType) -> bool:
-		""".. todo:: TREE::Node::__contains__ Needs documentation."""
+		"""
+		.. todo:: TREE::Node::__contains__ Needs documentation.
+
+		"""
 		return key in self._dict
 
 	def __len__(self) -> int:
 		"""
 		Returns the number of attached attributes (key-value-pairs) on this node.
 
 		:returns: Number of attached attributes.
 		"""
 		return len(self._dict)
 
 	@property
 	def Root(self) -> 'Node':
 		"""
-		Read-only property to access the tree's root node (:py:attr:`_root`).
+		Read-only property to access the tree's root node (:attr:`_root`).
 
 		:returns: The root node (representative node) of a tree.
 		"""
 		return self._root
 
 	@property
 	def Parent(self) -> Nullable['Node']:
 		"""
-		Property to get and set the parent (:py:attr:`_parent`) of a node.
+		Property to get and set the parent (:attr:`_parent`) of a node.
 
 		.. note::
 
 		   As the current node might be a tree itself, appending this node to a tree can lead to a merge of trees and
-		   especially to a merge of IDs. As IDs are unique, it might raise an :py:exc:`Exception`.
+		   especially to a merge of IDs. As IDs are unique, it might raise an :exc:`Exception`.
 
 		:returns:                   The parent of a node.
-		:raises TypeError:          If parameter ``parent`` is not a :py:class:`Node`
+		:raises TypeError:          If parameter ``parent`` is not a :class:`Node`
 		:raises AlreadyInTreeError: Parent is already a child node in this tree.
 		"""
 		return self._parent
 
 	@Parent.setter
 	def Parent(self, parent: Nullable['Node']) -> None:
 		# TODO: is moved inside the same tree, don't move nodes in _nodesWithID and don't change _root
@@ -394,15 +403,15 @@
 		for node in iterator:
 			result.append(node)
 
 		return tuple(result)
 
 	def _GetPathAsLinkedList(self) -> Deque["Node"]:
 		"""
-		Compute the path from current node to root node by using a linked list (:py:class:`deque`).
+		Compute the path from current node to root node by using a linked list (:class:`deque`).
 
 		:meta private:
 		:returns: Path from node to root node as double-ended queue (deque).
 		"""
 		path: Deque['Node'] = deque()
 
 		node = self
@@ -480,26 +489,26 @@
 			self._root._nodesWithoutID.append(node)
 			node._root = self._root
 
 	def AddChild(self, child: 'Node'):
 		"""
 		Add a child node to the current node of the tree.
 
-		If ``child`` is a subtree, both trees get merged. So all nodes in ``child`` get a new :py:attr:`_root` assigned and
-		all IDs are merged into the node's root's ID lists (:py:attr:`_nodesWithID`).
+		If ``child`` is a subtree, both trees get merged. So all nodes in ``child`` get a new :attr:`_root` assigned and
+		all IDs are merged into the node's root's ID lists (:attr:`_nodesWithID`).
 
 		:param child:               The child node to be added to the tree.
-		:raises TypeError:          If parameter ``child`` is not a :py:class:`Node`.
+		:raises TypeError:          If parameter ``child`` is not a :class:`Node`.
 		:raises AlreadyInTreeError: If parameter ``child`` is already a node in the tree.
 
 		.. seealso::
 
-		   :py:attr:`Parent` |br|
+		   :attr:`Parent` |br|
 		      |rarr| Set the parent of a node.
-		   :py:meth:`AddChildren` |br|
+		   :meth:`AddChildren` |br|
 		      |rarr| Add multiple children at once.
 		"""
 		if not isinstance(child, Node):
 			raise TypeError(f"Parameter 'child' is not of type 'Node'.")
 
 		if child._root is self._root:
 			raise AlreadyInTreeError(f"Child '{child}' is already a node in this tree.")
@@ -514,22 +523,22 @@
 		self._children.append(child)
 
 	def AddChildren(self, children: Iterable['Node']):
 		"""
 		Add multiple children nodes to the current node of the tree.
 
 		:param children:            The list of children nodes to be added to the tree.
-		:raises TypeError:          If parameter ``children`` contains an item, which is not a :py:class:`Node`.
+		:raises TypeError:          If parameter ``children`` contains an item, which is not a :class:`Node`.
 		:raises AlreadyInTreeError: If parameter ``children`` contains an item, which is already a node in the tree.
 
 		.. seealso::
 
-		   :py:attr:`Parent` |br|
+		   :attr:`Parent` |br|
 		      |rarr| Set the parent of a node.
-		   :py:meth:`AddChild` |br|
+		   :meth:`AddChild` |br|
 		      |rarr| Add a child node to the tree.
 		"""
 		for child in children:
 			if not isinstance(child, Node):
 				raise TypeError(f"Item '{child}' in parameter 'children' is not of type 'Node'.")
 
 			if child._root is self._root:
@@ -542,27 +551,36 @@
 			for node in child.GetDescendants():
 				node._level = node._parent._level + 1
 			self._SetNewRoot(child._nodesWithID, child._nodesWithoutID)
 			child._nodesWithID = child._nodesWithoutID = None
 			self._children.append(child)
 
 	def GetPath(self) -> Generator['Node', None, None]:
-		""".. todo:: TREE::Node::GetPAth Needs documentation."""
+		"""
+		.. todo:: TREE::Node::GetPAth Needs documentation.
+
+		"""
 		for node in self._GetPathAsLinkedList():
 			yield node
 
 	def GetAncestors(self) -> Generator['Node', None, None]:
-		""".. todo:: TREE::Node::GetAncestors Needs documentation."""
+		"""
+		.. todo:: TREE::Node::GetAncestors Needs documentation.
+
+		"""
 		node = self._parent
 		while node is not None:
 			yield node
 			node = node._parent
 
 	def GetCommonAncestors(self, others: Union['Node', Iterable['Node']]) -> Generator['Node', None, None]:
-		""".. todo:: TREE::Node::GetCommonAncestors Needs documentation."""
+		"""
+		.. todo:: TREE::Node::GetCommonAncestors Needs documentation.
+
+		"""
 		if isinstance(others, Node):
 			# Check for trivial case
 			if others is self:
 				for node in self._GetPathAsLinkedList():
 					yield node
 				return
 
@@ -583,21 +601,21 @@
 		"""
 		A generator to iterate all direct children of the current node.
 
 		:returns: A generator to iterate all children.
 
 		.. seealso::
 
-		   :py:meth:`GetDescendants` |br|
+		   :meth:`GetDescendants` |br|
 		      |rarr| Iterate all descendants.
-		   :py:meth:`IterateLevelOrder` |br|
+		   :meth:`IterateLevelOrder` |br|
 		      |rarr| Iterate items level-by-level, which includes the node itself as a first returned node.
-		   :py:meth:`IteratePreOrder` |br|
+		   :meth:`IteratePreOrder` |br|
 		      |rarr| Iterate items in pre-order, which includes the node itself as a first returned node.
-		   :py:meth:`IteratePostOrder` |br|
+		   :meth:`IteratePostOrder` |br|
 		      |rarr| Iterate items in post-order, which includes the node itself as a last returned node.
 		"""
 		for child in self._children:
 			yield child
 
 	def GetSiblings(self) -> Generator['Node', None, None]:
 		"""
@@ -664,21 +682,21 @@
 		A generator to iterate all descendants of the current node. In contrast to `IteratePreOrder` and `IteratePostOrder`
 		it doesn't include the node itself.
 
 		:returns: A generator to iterate all descendants.
 
 		.. seealso::
 
-		   :py:meth:`GetChildren` |br|
+		   :meth:`GetChildren` |br|
 		      |rarr| Iterate all children, but no grand-children.
-		   :py:meth:`IterateLevelOrder` |br|
+		   :meth:`IterateLevelOrder` |br|
 		      |rarr| Iterate items level-by-level, which includes the node itself as a first returned node.
-		   :py:meth:`IteratePreOrder` |br|
+		   :meth:`IteratePreOrder` |br|
 		      |rarr| Iterate items in pre-order, which includes the node itself as a first returned node.
-		   :py:meth:`IteratePostOrder` |br|
+		   :meth:`IteratePostOrder` |br|
 		      |rarr| Iterate items in post-order, which includes the node itself as a last returned node.
 		"""
 		for child in self._children:
 			yield child
 			yield from child.GetDescendants()
 
 	def GetRelatives(self):
@@ -728,21 +746,21 @@
 		A generator to iterate all siblings of the current node level-by-level top-down. In contrast to `GetDescendants`,
 		this includes also the node itself as the first returned node.
 
 		:returns: A generator to iterate all siblings level-by-level.
 
 		.. seealso::
 
-		   :py:meth:`GetChildren` |br|
+		   :meth:`GetChildren` |br|
 		      |rarr| Iterate all children, but no grand-children.
-		   :py:meth:`GetDescendants` |br|
+		   :meth:`GetDescendants` |br|
 		      |rarr| Iterate all descendants.
-		   :py:meth:`IteratePreOrder` |br|
+		   :meth:`IteratePreOrder` |br|
 		      |rarr| Iterate items in pre-order, which includes the node itself as a first returned node.
-		   :py:meth:`IteratePostOrder` |br|
+		   :meth:`IteratePostOrder` |br|
 		      |rarr| Iterate items in post-order, which includes the node itself as a last returned node.
 		"""
 		queue = deque([self])
 		while queue:
 			currentNode = queue.pop()
 			yield currentNode
 			for node in currentNode._children:
@@ -753,21 +771,21 @@
 		A generator to iterate all siblings of the current node in pre-order. In contrast to `GetDescendants`, this includes
 		also the node itself as the first returned node.
 
 		:returns: A generator to iterate all siblings in pre-order.
 
 		.. seealso::
 
-		   :py:meth:`GetChildren` |br|
+		   :meth:`GetChildren` |br|
 		      |rarr| Iterate all children, but no grand-children.
-		   :py:meth:`GetDescendants` |br|
+		   :meth:`GetDescendants` |br|
 		      |rarr| Iterate all descendants.
-		   :py:meth:`IterateLevelOrder` |br|
+		   :meth:`IterateLevelOrder` |br|
 		      |rarr| Iterate items level-by-level, which includes the node itself as a first returned node.
-		   :py:meth:`IteratePostOrder` |br|
+		   :meth:`IteratePostOrder` |br|
 		      |rarr| Iterate items in post-order, which includes the node itself as a last returned node.
 		"""
 		yield self
 		for child in self._children:
 			yield from child.IteratePreOrder()
 
 	def IteratePostOrder(self) -> Generator['Node', None, None]:
@@ -775,21 +793,21 @@
 		A generator to iterate all siblings of the current node in post-order. In contrast to `GetDescendants`, this
 		includes also the node itself as the last returned node.
 
 		:returns: A generator to iterate all siblings in post-order.
 
 		.. seealso::
 
-		   :py:meth:`GetChildren` |br|
+		   :meth:`GetChildren` |br|
 		      |rarr| Iterate all children, but no grand-children.
-		   :py:meth:`GetDescendants` |br|
+		   :meth:`GetDescendants` |br|
 		      |rarr| Iterate all descendants.
-		   :py:meth:`IterateLevelOrder` |br|
+		   :meth:`IterateLevelOrder` |br|
 		      |rarr| Iterate items level-by-level, which includes the node itself as a first returned node.
-		   :py:meth:`IteratePreOrder` |br|
+		   :meth:`IteratePreOrder` |br|
 		      |rarr| Iterate items in pre-order, which includes the node itself as a first returned node.
 		"""
 		for child in self._children:
 			yield from child.IteratePostOrder()
 		yield self
 
 	def WalkTo(self, other: 'Node') -> Generator['Node', None, None]:
@@ -874,17 +892,17 @@
 
 	def __str__(self) -> str:
 		"""
 		Return a string representation of the node.
 
 		Order of resolution:
 
-		1. If :py:attr:`_value` is not None, return the string representation of :py:attr:`_value`.
-		2. If :py:attr:`_id` is not None, return the string representation of :py:attr:`_id`.
-		3. Else, return :py:meth:`__repr__`.
+		1. If :attr:`_value` is not None, return the string representation of :attr:`_value`.
+		2. If :attr:`_id` is not None, return the string representation of :attr:`_id`.
+		3. Else, return :meth:`__repr__`.
 
 		:returns: The resolved string representation of the node.
 		"""
 		if self._value is not None:
 			return str(self._value)
 		elif self._id is not None:
 			return str(self._id)
```

### Comparing `pyTooling-4.0.1/pyTooling/Versioning/__init__.py` & `pyTooling-5.0.0/pyTooling/Versioning/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -33,50 +33,60 @@
 
 .. hint:: See :ref:`high-level help <VERSIONING>` for explanations and usage examples.
 """
 from enum          import IntEnum
 from typing        import Optional as Nullable, Any
 
 from ..Decorators  import export
-from ..MetaClasses import Overloading
+from ..MetaClasses import ExtendedType
 
 
 @export
-class SemVersion(metaclass=Overloading):
-	"""Representation of a semantic version number like ``3.7.12``."""
-
-	class Parts(IntEnum):
-		"""Enumeration of parts in a version number that can be presents."""
+class Parts(IntEnum):
+	"""Enumeration of parts in a version number that can be presents."""
 
-		Major = 1       #: Major number is present. (e.g. X in ``vX.0.0``).
-		Minor = 2       #: Minor number is present. (e.g. Y in ``v0.Y.0``).
-		Patch = 4       #: Patch number is present. (e.g. Z in ``v0.0.Z``).
-		Build = 8       #: Build number is present. (e.g. bbbb in ``v0.0.0.bbbb``)
-		Pre   = 16      #: Pre-release number is present.
-		Post  = 32      #: Post-release number is present.
-		Prefix = 64     #: Prefix is present.
-		Postfix = 128   #: Postfix is present.
+	Unknown = 0     #: Undocumented
+	Major = 1       #: Major number is present. (e.g. X in ``vX.0.0``).
+	Minor = 2       #: Minor number is present. (e.g. Y in ``v0.Y.0``).
+	Patch = 4       #: Patch number is present. (e.g. Z in ``v0.0.Z``).
+	Build = 8       #: Build number is present. (e.g. bbbb in ``v0.0.0.bbbb``)
+	Pre   = 16      #: Pre-release number is present.
+	Post  = 32      #: Post-release number is present.
+	Prefix = 64     #: Prefix is present.
+	Postfix = 128   #: Postfix is present.
 #		AHead   = 256
 
-	class Flags(IntEnum):
-		"""State enumeration, if a (tagged) version is build from a clean or dirty working directory."""
 
-		Clean = 1       #: A versioned build was created from a *clean* working directory.
-		Dirty = 2       #: A versioned build was created from a *dirty* working directory.
+@export
+class Flags(IntEnum):
+	"""State enumeration, if a (tagged) version is build from a clean or dirty working directory."""
+
+	Clean = 1       #: A versioned build was created from a *clean* working directory.
+	Dirty = 2       #: A versioned build was created from a *dirty* working directory.
+
+
+@export
+class Version(metaclass=ExtendedType, slots=True):
+	pass
+
+
+@export
+class SemanticVersion(Version):
+	"""Representation of a semantic version number like ``3.7.12``."""
 
-	parts   : Parts                #: Integer flag enumeration of present parts in a version number.
-	flags   : int = Flags.Clean    #: State if the version in a working directory is clean or dirty compared to a tagged version.
-	major   : int = 0              #: Major number part of the version number.
-	minor   : int = 0              #: Minor number part of the version number.
-	patch   : int = 0              #: Patch number part of the version number.
-	build   : int = 0              #: Build number part of the version number.
-	pre     : int = 0              #: Pre-release version number part.
-	post    : int = 0              #: Post-release version number part.
-	prefix  : str = ""             #: Prefix string
-	postfix : str = ""             #: Postfix string
+	_parts   : Parts = Parts.Unknown  #: Integer flag enumeration of present parts in a version number.
+	_flags   : int = Flags.Clean      #: State if the version in a working directory is clean or dirty compared to a tagged version.
+	_major   : int = 0                #: Major number part of the version number.
+	_minor   : int = 0                #: Minor number part of the version number.
+	_patch   : int = 0                #: Patch number part of the version number.
+	_build   : int = 0                #: Build number part of the version number.
+	_pre     : int = 0                #: Pre-release version number part.
+	_post    : int = 0                #: Post-release version number part.
+	_prefix  : str = ""               #: Prefix string
+	_postfix : str = ""               #: Postfix string
 # QUESTION: was this how many commits a version is ahead of the last tagged version?
 #	ahead   : int = 0
 
 	def __init__(self, versionString : str):
 		if versionString == "":
 			raise ValueError("Parameter 'versionString' is empty.")
 		elif versionString is None:
@@ -84,161 +94,193 @@
 		elif versionString.startswith(("V", "v", "I", "i", "R", "r")):
 			versionString = versionString[1:]
 		elif versionString.startswith(("rev", "REV")):
 			versionString = versionString[3:]
 
 		split = versionString.split(".")
 		length = len(split)
-		self.major = int(split[0])
+		self._major = int(split[0])
+		self._minor = 0
+		self._patch = 0
+		self._build = 0
+		self._parts = Parts.Major
 		if length >= 2:
-			self.minor = int(split[1])
+			self._minor = int(split[1])
+			self._parts |= Parts.Minor
 		if length >= 3:
-			self.patch = int(split[2])
+			self._patch = int(split[2])
+			self._parts |= Parts.Patch
 		if length >= 4:
-			self.build = int(split[3])
-		self.flags = self.Flags.Clean
+			self._build = int(split[3])
+			self._parts |= Parts.Build
+		self._flags = Flags.Clean
 
 	def __init__(self, major: int, minor: int, patch: int = 0, build: int = 0):  # type: ignore[no-redef]
-		self.major = major
-		self.minor = minor
-		self.patch = patch
-		self.build = build
-		self.flags = self.Flags.Clean
+		self._major = major
+		self._minor = minor
+		self._patch = patch
+		self._build = build
+		self._parts = Parts.Minor | Parts.Minor | Parts.Patch | Parts.Build
+		self._flags = Flags.Clean
+
+	@property
+	def Major(self) -> int:
+		return self._major
+
+	@property
+	def Minor(self) -> int:
+		return self._minor
+
+	@property
+	def Patch(self) -> int:
+		return self._patch
+
+	@property
+	def Build(self) -> int:
+		return self._build
+
+	@property
+	def Parts(self) -> Parts:
+		return self._parts
+
+	@property
+	def Flags(self) -> Flags:
+		return self._flags
 
 	def __eq__(self, other: Any) -> bool:
 		"""
 		Compare two Version instances (version numbers) for equality.
 
 		:param other:      Parameter to compare against.
 		:returns:          ``True``, if both version numbers are equal.
-		:raises TypeError: If parameter ``other`` is not of type :py:class:`SemVersion`.
+		:raises TypeError: If parameter ``other`` is not of type :class:`SemVersion`.
 		"""
-		if not isinstance(other, SemVersion):
+		if not isinstance(other, SemanticVersion):
 			raise TypeError(f"Parameter 'other' is not of type 'SemVersion'.")
 
 		return (
-			(self.major == other.major) and
-			(self.minor == other.minor) and
-			(self.patch == other.patch) and
-			(self.build == other.build)
+			(self._major == other._major) and
+			(self._minor == other._minor) and
+			(self._patch == other._patch) and
+			(self._build == other._build)
 		)
 
 	def __ne__(self, other: Any) -> bool:
 		"""
 		Compare two Version instances (version numbers) for inequality.
 
 		:param other:      Parameter to compare against.
 		:returns:          ``True``, if both version numbers are not equal.
-		:raises TypeError: If parameter ``other`` is not of type :py:class:`SemVersion`.
+		:raises TypeError: If parameter ``other`` is not of type :class:`SemVersion`.
 		"""
-		if not isinstance(other, SemVersion):
+		if not isinstance(other, SemanticVersion):
 			raise TypeError(f"Parameter 'other' is not of type 'SemVersion'.")
 
 		return not self.__eq__(other)
 
 	@staticmethod
-	def __compare(left: 'SemVersion', right: 'SemVersion') -> Nullable[bool]:
+	def __compare(left: 'SemanticVersion', right: 'SemanticVersion') -> Nullable[bool]:
 		"""
-		Private helper method to compute the comparison of two :py:class:`SemVersion` instances.
+		Private helper method to compute the comparison of two :class:`SemVersion` instances.
 
 		:param left:  Left parameter.
 		:param right: Right parameter.
 		:returns:     ``True``, if ``left`` is smaller than ``right``. |br|
 		              False if ``left`` is greater than ``right``. |br|
 		              Otherwise it's None (both parameters are equal).
 		"""
-		if (left.major < right.major):
+		if left._major < right._major:
 			return True
-		if (left.major > right.major):
+		elif left._major > right._major:
 			return False
 
-		if (left.minor < right.minor):
+		if left._minor < right._minor:
 			return True
-		if (left.minor > right.minor):
+		elif left._minor > right._minor:
 			return False
 
-		if (left.patch < right.patch):
+		if left._patch < right._patch:
 			return True
-		if (left.patch > right.patch):
+		elif left._patch > right._patch:
 			return False
 
-		if (left.build < right.build):
+		if left._build < right._build:
 			return True
-		if (left.build > right.build):
+		elif left._build > right._build:
 			return False
 
 		return None
 
 	def __lt__(self, other: Any) -> bool:
 		"""
 		Compare two Version instances (version numbers) if the version is less than the second operand.
 
 		:param other:      Parameter to compare against.
 		:returns:          ``True``, if version is less than the second operand.
-		:raises TypeError: If parameter ``other`` is not of type :py:class:`SemVersion`.
+		:raises TypeError: If parameter ``other`` is not of type :class:`SemVersion`.
 		"""
-		if not isinstance(other, SemVersion):
+		if not isinstance(other, SemanticVersion):
 			raise TypeError(f"Parameter 'other' is not of type 'SemVersion'.")
 
 		result = self.__compare(self, other)
 		return result if result is not None else False
 
 	def __le__(self, other: Any) -> bool:
 		"""
 		Compare two Version instances (version numbers) if the version is less than or equal to the second operand.
 
 		:param other:      Parameter to compare against.
 		:returns:          ``True``, if version is less than or equal to the second operand.
-		:raises TypeError: If parameter ``other`` is not of type :py:class:`SemVersion`.
+		:raises TypeError: If parameter ``other`` is not of type :class:`SemVersion`.
 		"""
-		if not isinstance(other, SemVersion):
+		if not isinstance(other, SemanticVersion):
 			raise TypeError(f"Parameter 'other' is not of type 'SemVersion'.")
 
 		result = self.__compare(self, other)
 		return result if result is not None else True
 
 	def __gt__(self, other: Any) -> bool:
 		"""
 		Compare two Version instances (version numbers) if the version is greater than the second operand.
 
 		:param other:      Parameter to compare against.
 		:returns:          ``True``, if version is greater than the second operand.
-		:raises TypeError: If parameter ``other`` is not of type :py:class:`SemVersion`.
+		:raises TypeError: If parameter ``other`` is not of type :class:`SemVersion`.
 		"""
-		if not isinstance(other, SemVersion):
+		if not isinstance(other, SemanticVersion):
 			raise TypeError(f"Parameter 'other' is not of type 'SemVersion'.")
 
 		return not self.__le__(other)
 
 	def __ge__(self, other: Any) -> bool:
 		"""
 		Compare two Version instances (version numbers) if the version is greater than or equal to the second operand.
 
 		:param other:      Parameter to compare against.
 		:returns:          ``True``, if version is greater than or equal to the second operand.
-		:raises TypeError: If parameter ``other`` is not of type :py:class:`SemVersion`.
+		:raises TypeError: If parameter ``other`` is not of type :class:`SemVersion`.
 		"""
-		if not isinstance(other, SemVersion):
+		if not isinstance(other, SemanticVersion):
 			raise TypeError(f"Parameter 'other' is not of type 'SemVersion'.")
 
 		return not self.__lt__(other)
 
 	def __repr__(self) -> str:
 		"""
 		Return a string representation of this version number without prefix ``v``.
 
 		:returns: Raw version number representation without a prefix.
 		"""
-		return f"{self.major}.{self.minor}.{self.patch}"
+		return f"{self._major}.{self._minor}.{self._patch}"
 
 	def __str__(self) -> str:
 		"""
 		Return a string representation of this version number with prefix ``v``.
 
 		:returns: Version number representation including a prefix.
 		"""
-		return f"v{self.major}.{self.minor}.{self.patch}"
+		return f"v{self._major}.{self._minor}.{self._patch}"
 
 
 @export
-class CalVersion(metaclass=Overloading):
+class CalendarVersion(Version):
 	"""Representation of a calendar version number like ``2021.10``."""
```

### Comparing `pyTooling-4.0.1/pyTooling.egg-info/PKG-INFO` & `pyTooling-5.0.0/pyTooling.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyTooling
-Version: 4.0.1
+Version: 5.0.0
 Summary: pyTooling is a powerful collection of arbitrary useful classes, decorators, meta-classes and exceptions.
 Home-page: https://GitHub.com/pyTooling/pyTooling.*
 Author: Patrick Lehmann
 Author-email: Paebbels@gmail.com
 License: Apache-2.0
 Project-URL: Documentation, https://pyTooling.GitHub.io/pyTooling.*
 Project-URL: Source Code, https://GitHub.com/pyTooling/pyTooling.*
@@ -49,78 +49,85 @@
 [![Gitter](https://img.shields.io/badge/chat-on%20gitter-4db797.svg?longCache=true&style=flat-square&logo=gitter&logoColor=e8ecef)](https://gitter.im/hdl/community)
 [![Dependent repos (via libraries.io)](https://img.shields.io/librariesio/dependent-repos/pypi/pyTooling?longCache=true&style=flat-square&logo=GitHub)](https://github.com/pyTooling/pyTooling/network/dependents)
 [![Libraries.io SourceRank](https://img.shields.io/librariesio/sourcerank/pypi/pyTooling)](https://libraries.io/github/pyTooling/pyTooling/sourcerank)
 -->
 
 # pyTooling
 
-**pyTooling** is a powerful collection of arbitrary useful abstract data models, classes, decorators, meta-classes and
-exceptions. It also provides lots of helper functions e.g. to ease the handling of package descriptions.
+**pyTooling** is a powerful collection of arbitrary useful abstract data models, missing classes, decorators, a new
+performance boosting meta-class and enhanced exceptions. It also provides lots of helper functions e.g. to ease the
+handling of package descriptions or to unify multiple existing APIs into a single API.
 
-It's useful for **any** Python-base project independent if it's a library, framework or CLI tool.
+It's useful - if not even essential - for **any** Python-base project independent if it's a library, framework, CLI tool
+or just a "script".
 
 ## Introduction
 
 **pyTooling** is a basic collection of powerful helpers needed by almost any Python project. More specialized helpers
 can be found in sub-namespaces like:
 
 * [pyTooling.CLIAbstraction](https://github.com/pyTooling/pyTooling.CLIAbstraction)
-* [pyTooling.TerminalUI](https://github.com/pyTooling/pyTooling.TerminalUI)
 
-In addition, pyTooling provides a collection of CI job templates for GitHub Actions. This drastically simplifies
-GHA-based CI pipelines for Python projects.
+In addition, pyTooling provides a collection of [CI job templates for GitHub Actions](https://github.com/pyTooling/Actions).
+This drastically simplifies GHA-based CI pipelines for Python projects.
 
 ## Package Details
 
 ### Common Helper Functions
 
 This is a set of useful [helper functions](https://pytooling.github.io/pyTooling/Common/index.html#common-helperfunctions):
 
 * [getsizeof](https://pytooling.github.io/pyTooling/Common/index.html#getsizeof) calculates the "real" size of a data structure.
 * [isnestedclass](https://pytooling.github.io/pyTooling/Common/index.html#isnestedclass) checks if a class is nested inside another class.
+* [firstKey](https://pytooling.github.io/pyTooling/Common/index.html#firstkey), [firstValue](https://pytooling.github.io/pyTooling/Common/index.html#firstvalue), [firstItem](https://pytooling.github.io/pyTooling/Common/index.html#firstitem) get the first key/value/item from an ordered dictionary.
 * [mergedicts](https://pytooling.github.io/pyTooling/Common/index.html#mergedicts) merges multiple dictionaries into a new dictionary.
 * [zipdicts](https://pytooling.github.io/pyTooling/Common/index.html#zipdicts) iterate multiple dictionaries simultaneously.
 
 
 ### Common Classes
 
-* Python doesn't provide [call-by-reference parameters](https://pytooling.github.io/pyTooling/Common/CallByRef.html) for
-  simple types. This behavior can be emulated with classes provided by the `pyTooling.CallByRef` module.
-* Setuptools, PyPI, and others have a varying understanding of license names. The `pyTooling.Licensing` module
-  provides [unified license names](https://pytooling.github.io/pyTooling/Common/Licensing.html) as well as license name
-  mappings or translations.
-* Python has many ways in figuring out the current platform using APIs from `sys`, `platform`, `os`, ….
-  Unfortunately, none of the provided standard APIs offers a comprehensive answer. pyTooling provides a
-  [unified platform and environment description](https://pytooling.github.io/pyTooling/Common/Platform.html) by
-  summarizing multiple platform APIs into a single class instance.
-* While Python itself has a good versioning schema, there are no classes provided to abstract version numbers. pyTooling
-  provides such a [representations of version numbers](https://pytooling.github.io/pyTooling/Common/Versioning.html)
-  following semantic versioning (SemVer) and calendar versioning (CalVer) schemes. It's provided by the
-  `pyTooling.Versioning` module.
+* [Call-by-reference parameters](https://pytooling.github.io/pyTooling/Common/CallByRef.html): Python doesn't provide
+  *call-by-reference parameters* for simple types.  
+  This behavior can be emulated with classes provided by the `pyTooling.CallByRef` module.
+* [Unified license names](https://pytooling.github.io/pyTooling/Common/Licensing.html): Setuptools, PyPI, and others
+  have a varying understanding of license names.  
+  The `pyTooling.Licensing` module provides *unified license names* as well as license name mappings or translations.
+* [Unified platform and environment description](https://pytooling.github.io/pyTooling/Common/Platform.html): Python has
+  many ways in figuring out the current platform using APIs from `sys`, `platform`, `os`, …. Unfortunately, none of the
+  provided standard APIs offers a comprehensive answer. pyTooling provides a `CurrentPlatform` singleton summarizing
+  multiple platform APIs into a single class instance.
+* [Representations of version numbers](https://pytooling.github.io/pyTooling/Common/Versioning.html): While Python
+  itself has a good versioning schema, there are no classes provided to abstract version numbers. pyTooling provides
+  such representations following semantic versioning (SemVer) and calendar versioning (CalVer) schemes. It's provided by 
+  the `pyTooling.Versioning` module.
 
 ### Configuration
 
 Various file formats suitable for configuration information share the same features supporting: key-value pairs
 (dictionaries), sequences (lists), and simple types like string, integer and float. pyTooling provides an
 [abstract configuration file data model](https://pytooling.github.io/pyTooling/Configuration/index.html) supporting
 these features. Moreover, concrete [configuration file format reader](https://pytooling.github.io/pyTooling/Configuration/FileFormats.html)
 implementations are provided as well.
 
-* [JSON configuration reader](https://pytooling.github.io/pyTooling/Configuration/JSON.html) &rarr; To be implemented.
+* [JSON configuration reader](https://pytooling.github.io/pyTooling/Configuration/JSON.html) for the JSON file format.
 * [TOML configuration reader](https://pytooling.github.io/pyTooling/Configuration/TOML.html) &rarr; To be implemented.
 * [YAML configuration reader](https://pytooling.github.io/pyTooling/Configuration/YAML.html) for the YAML file format.
 
 
 ### Data Structures
 
-pyTooling also provides fast and powerful data structures offering object-oriented APIs:
+pyTooling also provides [fast and powerful data structures](https://pytooling.github.io/pyTooling/DataStructures/index.html)
+offering object-oriented APIs:
 
 * [Graph data structure](https://pytooling.github.io/pyTooling/DataStructures/Graph.html)  
-  &rarr; A directed graph implementation using a `Vertex` and `Edge`
-  class.
+  &rarr; A directed graph implementation using a `Vertex` and an `Edge` class.
+* [Path data structure](https://pytooling.github.io/pyTooling/DataStructures/Path/index.html)  
+  &rarr; To be documented.
+* [Finite State Machine data structure](https://pytooling.github.io/pyTooling/DataStructures/StateMachine.html)  
+  &rarr; A data model for state machines using a `State` and a `Transition` class.
 * [Tree data structure](https://pytooling.github.io/pyTooling/DataStructures/Tree.html)  
   &rarr; A fast and simple implementation using a single `Node` class.
 
 
 ### Decorators
 
 * [Abstract Methods](https://pytooling.github.io/pyTooling/MetaClasses.html#meta-abstract)
@@ -164,16 +171,16 @@
   `@abstractmethod` or `@mustoverride`.
 
 `class MyClass(metaclass=ExtendedType, singleton=True):`
   A class defined with enabled [singleton](https://pytooling.github.io/pyTooling/MetaClasses.html#singleton) behavior
   allows only a single instance of that class to exist. If another instance is going to be created, a previously cached
   instance of that class will be returned.
 
-`class MyClass(metaclass=ExtendedType, useSlots=True):`
-  A class defined with enabled [useSlots](https://pytooling.github.io/pyTooling/MetaClasses.html#slotted-type) behavior
+`class MyClass(metaclass=ExtendedType, slots=True):`
+  A class defined with enabled [slots](https://pytooling.github.io/pyTooling/MetaClasses.html#slotted-type) behavior
   stores instance fields in slots. The meta-class, translates all type-annotated fields in a class definition into
   slots. Slots allow a more efficient field storage and access compared to dynamically stored and accessed fields hosted
   by `__dict__`. This improves the memory footprint as well as the field access performance of all class instances. This
   behavior is automatically inherited to all derived classes.
 
 `class MyClass(ObjectWithSlots):`
   A class definition deriving from `ObjectWithSlots` will bring the slotted type behavior to that class and all derived
```

### Comparing `pyTooling-4.0.1/pyTooling.egg-info/SOURCES.txt` & `pyTooling-5.0.0/pyTooling.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -5,24 +5,26 @@
 pyTooling/py.typed
 pyTooling.egg-info/PKG-INFO
 pyTooling.egg-info/SOURCES.txt
 pyTooling.egg-info/dependency_links.txt
 pyTooling.egg-info/requires.txt
 pyTooling.egg-info/top_level.txt
 pyTooling/CallByRef/__init__.py
-pyTooling/Common/Platform.py
 pyTooling/Common/__init__.py
+pyTooling/Configuration/JSON.py
 pyTooling/Configuration/YAML.py
 pyTooling/Configuration/__init__.py
 pyTooling/Decorators/__init__.py
 pyTooling/Exceptions/__init__.py
 pyTooling/GenericPath/URL.py
 pyTooling/GenericPath/__init__.py
 pyTooling/Graph/GraphML.py
 pyTooling/Graph/__init__.py
 pyTooling/Licensing/__init__.py
 pyTooling/MetaClasses/__init__.py
 pyTooling/Packaging/__init__.py
+pyTooling/Platform/__init__.py
+pyTooling/StateMachine/__init__.py
 pyTooling/TerminalUI/__init__.py
 pyTooling/Timer/__init__.py
 pyTooling/Tree/__init__.py
 pyTooling/Versioning/__init__.py
```

### Comparing `pyTooling-4.0.1/pyTooling.egg-info/requires.txt` & `pyTooling-5.0.0/pyTooling.egg-info/requires.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,41 +1,43 @@
 
 [all]
-autoapi>=2.0.1
-Coverage>=7.2
-sphinxcontrib-mermaid>=0.8.1
-pytest-cov>=4.0.0
-pytest-benchmark>=4.0.0
-pyTooling<4.0,>=3.0.0
-mypy>=1.1.1
-sphinx_fontawesome>=0.0.6
-sphinx<6.0,>=5.3
 sphinx_autodoc_typehints>=1.19.5
-pytest>=7.2.0
+sphinx-inline-tabs>=2023.4.21
 lxml>=4.9
-colorama>=0.4.6
+mypy>=1.2.0
+sphinxcontrib-mermaid>=0.9.2
+pytest>=7.3.1
+sphinx_fontawesome>=0.0.6
+typing_extensions>=4.6.3
+Coverage>=7.2
+pyTooling<5.0,>=4.0.1
 ruamel.yaml>=0.17
+pytest-cov>=4.1.0
+colorama>=0.4.6
+autoapi>=2.0.1
+sphinx<6.0,>=5.3
 
 [doc]
-autoapi>=2.0.1
-sphinxcontrib-mermaid>=0.8.1
-ruamel.yaml>=0.17
+sphinx_autodoc_typehints>=1.19.5
+sphinx-inline-tabs>=2023.4.21
+sphinxcontrib-mermaid>=0.9.2
 sphinx_fontawesome>=0.0.6
+pyTooling<5.0,>=4.0.1
+ruamel.yaml>=0.17
+autoapi>=2.0.1
 sphinx<6.0,>=5.3
-sphinx_autodoc_typehints>=1.19.5
-pyTooling<4.0,>=3.0.0
 
 [terminal]
 colorama>=0.4.6
 
 [test]
-Coverage>=7.2
-pytest-cov>=4.0.0
-pytest-benchmark>=4.0.0
-mypy>=1.1.1
-pytest>=7.2.0
 lxml>=4.9
-colorama>=0.4.6
+mypy>=1.2.0
+pytest>=7.3.1
+typing_extensions>=4.6.3
+Coverage>=7.2
 ruamel.yaml>=0.17
+pytest-cov>=4.1.0
+colorama>=0.4.6
 
 [yaml]
 ruamel.yaml>=0.17
```

### Comparing `pyTooling-4.0.1/pyproject.toml` & `pyTooling-5.0.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [build-system]
 requires = [
   "setuptools >= 62.3.3",
   "wheel >= 0.38.1",
-  "pyTooling >= 2.12.0"
+  "pyTooling >= 4.0.1"
 ]
 build-backend = "setuptools.build_meta"
 
 [tool.black]
 line-length = 120
 
 [tool.mypy]
```

### Comparing `pyTooling-4.0.1/setup.py` & `pyTooling-5.0.0/setup.py`

 * *Files identical despite different names*

