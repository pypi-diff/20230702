# Comparing `tmp/pelican_myst_reader-1.2.0b1.tar.gz` & `tmp/pelican_myst_reader-1.3.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pelican_myst_reader-1.2.0b1.tar", max compression
+gzip compressed data, was "pelican_myst_reader-1.3.0b1.tar", max compression
```

## Comparing `pelican_myst_reader-1.2.0b1.tar` & `pelican_myst_reader-1.3.0b1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    34523 2022-11-17 05:37:10.189973 pelican_myst_reader-1.2.0b1/LICENSE
--rw-r--r--   0        0        0     5326 2022-11-17 05:37:10.189973 pelican_myst_reader-1.2.0b1/README.md
--rw-r--r--   0        0        0       72 2022-11-17 05:37:10.189973 pelican_myst_reader-1.2.0b1/pelican/plugins/myst_reader/__init__.py
--rw-r--r--   0        0        0      586 2022-11-17 05:37:10.189973 pelican_myst_reader-1.2.0b1/pelican/plugins/myst_reader/_docutils_renderer.py
--rw-r--r--   0        0        0     2581 2022-11-17 05:37:10.189973 pelican_myst_reader-1.2.0b1/pelican/plugins/myst_reader/_sphinx_renderer.py
--rw-r--r--   0        0        0     8320 2022-11-17 05:37:10.189973 pelican_myst_reader-1.2.0b1/pelican/plugins/myst_reader/myst_reader.py
--rw-r--r--   0        0        0     2371 2022-11-17 05:37:10.193973 pelican_myst_reader-1.2.0b1/pyproject.toml
--rw-r--r--   0        0        0     6479 1970-01-01 00:00:00.000000 pelican_myst_reader-1.2.0b1/setup.py
--rw-r--r--   0        0        0     6987 1970-01-01 00:00:00.000000 pelican_myst_reader-1.2.0b1/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-07-02 11:46:22.218201 pelican_myst_reader-1.3.0b1/LICENSE
+-rw-r--r--   0        0        0     9819 2023-07-02 11:46:22.222201 pelican_myst_reader-1.3.0b1/README.md
+-rw-r--r--   0        0        0       72 2023-07-02 11:46:22.222201 pelican_myst_reader-1.3.0b1/pelican/plugins/myst_reader/__init__.py
+-rw-r--r--   0        0        0      654 2023-07-02 11:46:22.222201 pelican_myst_reader-1.3.0b1/pelican/plugins/myst_reader/_docutils_renderer.py
+-rw-r--r--   0        0        0     2373 2023-07-02 11:46:22.222201 pelican_myst_reader-1.3.0b1/pelican/plugins/myst_reader/_sphinx_renderer.py
+-rw-r--r--   0        0        0      107 2023-07-02 11:46:22.222201 pelican_myst_reader-1.3.0b1/pelican/plugins/myst_reader/exceptions.py
+-rw-r--r--   0        0        0    14245 2023-07-02 11:46:22.222201 pelican_myst_reader-1.3.0b1/pelican/plugins/myst_reader/myst_reader.py
+-rw-r--r--   0        0        0     2361 2023-07-02 11:46:22.222201 pelican_myst_reader-1.3.0b1/pyproject.toml
+-rw-r--r--   0        0        0    11470 1970-01-01 00:00:00.000000 pelican_myst_reader-1.3.0b1/PKG-INFO
```

### Comparing `pelican_myst_reader-1.2.0b1/LICENSE` & `pelican_myst_reader-1.3.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `pelican_myst_reader-1.2.0b1/pyproject.toml` & `pelican_myst_reader-1.3.0b1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pelican-myst-reader"
-version = "1.2.0b1"
+version = "1.3.0b1"
 description = "Pelican plugin for converting MyST's Markdown variant to HTML."
 authors = ["Ashwin Vishnu <dev@fluid.quest>"]
 license = "AGPL-3.0"
 readme = "README.md"
 keywords = ["pelican", "plugin", "markdown", "myst"]
 repository = "https://github.com/ashwinvis/myst-reader"
 documentation = "https://docs.getpelican.com"
@@ -29,16 +29,16 @@
 
 [tool.poetry.dependencies]
 python = "^3.9"
 pelican = "^4.5"
 markdown = {version = "^3.2.2", optional = true}
 markdown-word-count = "^0.0.1"
 beautifulsoup4 = "^4.9.3"
-myst-parser = "^0.18.0"
-docutils = ">=0.17.0,<=0.18"
+myst-parser = "^2.0.0"
+docutils = ">=0.17"
 sphinxcontrib-bibtex = "~2.5.0"
 pyyaml = "^6.0"
 
 [tool.poetry.group.tests.dependencies]
 pytest = "^6.0"
 pytest-cov = "^2.8"
 pytest-pythonpath = "^0.7.3"
```

