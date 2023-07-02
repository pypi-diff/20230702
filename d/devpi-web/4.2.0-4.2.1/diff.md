# Comparing `tmp/devpi-web-4.2.0.tar.gz` & `tmp/devpi-web-4.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "devpi-web-4.2.0.tar", last modified: Mon Dec  5 10:10:40 2022, max compression
+gzip compressed data, was "devpi-web-4.2.1.tar", last modified: Sun Jul  2 12:03:58 2023, max compression
```

## Comparing `devpi-web-4.2.0.tar` & `devpi-web-4.2.1.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2022-12-05 10:10:40.048041 devpi-web-4.2.0/
--rw-r--r--   0 fschulze   (501) staff       (20)       80 2022-12-05 10:10:32.000000 devpi-web-4.2.0/AUTHORS
--rw-r--r--   0 fschulze   (501) staff       (20)    14916 2022-12-05 10:10:32.000000 devpi-web-4.2.0/CHANGELOG
--rw-r--r--   0 fschulze   (501) staff       (20)     1061 2022-12-05 10:10:32.000000 devpi-web-4.2.0/LICENSE
--rw-r--r--   0 fschulze   (501) staff       (20)      144 2022-12-05 10:10:32.000000 devpi-web-4.2.0/MANIFEST.in
--rw-r--r--   0 fschulze   (501) staff       (20)     4329 2022-12-05 10:10:40.048166 devpi-web-4.2.0/PKG-INFO
--rw-r--r--   0 fschulze   (501) staff       (20)     1122 2022-12-05 10:10:32.000000 devpi-web-4.2.0/README.rst
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2022-12-05 10:10:40.036788 devpi-web-4.2.0/devpi_web/
--rw-r--r--   0 fschulze   (501) staff       (20)       22 2022-12-05 10:10:32.000000 devpi-web-4.2.0/devpi_web/__init__.py
--rw-r--r--   0 fschulze   (501) staff       (20)     1575 2022-12-05 10:10:32.000000 devpi-web-4.2.0/devpi_web/clear_index.py
--rw-r--r--   0 fschulze   (501) staff       (20)      813 2022-12-05 10:10:32.000000 devpi-web-4.2.0/devpi_web/config.py
--rw-r--r--   0 fschulze   (501) staff       (20)     2921 2022-12-05 10:10:32.000000 devpi-web-4.2.0/devpi_web/description.py
--rw-r--r--   0 fschulze   (501) staff       (20)     8125 2022-12-05 10:10:32.000000 devpi-web-4.2.0/devpi_web/doczip.py
--rw-r--r--   0 fschulze   (501) staff       (20)      785 2022-12-05 10:10:32.000000 devpi-web-4.2.0/devpi_web/hookspecs.py
--rw-r--r--   0 fschulze   (501) staff       (20)     3568 2022-12-05 10:10:32.000000 devpi-web-4.2.0/devpi_web/indexing.py
--rw-r--r--   0 fschulze   (501) staff       (20)    13429 2022-12-05 10:10:32.000000 devpi-web-4.2.0/devpi_web/main.py
--rw-r--r--   0 fschulze   (501) staff       (20)     1940 2022-12-05 10:10:32.000000 devpi-web-4.2.0/devpi_web/null_index.py
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2022-12-05 10:10:40.040606 devpi-web-4.2.0/devpi_web/static/
--rw-r--r--   0 fschulze   (501) staff       (20)     1580 2022-12-05 10:10:32.000000 devpi-web-4.2.0/devpi_web/static/common.js
--rw-r--r--   0 fschulze   (501) staff       (20)     3477 2022-12-05 10:10:32.000000 devpi-web-4.2.0/devpi_web/static/docview.js
--rw-r--r--   0 fschulze   (501) staff       (20)    15086 2022-12-05 10:10:32.000000 devpi-web-4.2.0/devpi_web/static/favicon.ico
--rw-r--r--   0 fschulze   (501) staff       (20)    89501 2022-12-05 10:10:32.000000 devpi-web-4.2.0/devpi_web/static/jquery-3.6.0.min.js
--rw-r--r--   0 fschulze   (501) staff       (20)    10274 2022-12-05 10:10:32.000000 devpi-web-4.2.0/devpi_web/static/style.css
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2022-12-05 10:10:40.044690 devpi-web-4.2.0/devpi_web/templates/
--rw-r--r--   0 fschulze   (501) staff       (20)     1410 2022-12-05 10:10:32.000000 devpi-web-4.2.0/devpi_web/templates/doc.pt
--rw-r--r--   0 fschulze   (501) staff       (20)      467 2022-12-05 10:10:32.000000 devpi-web-4.2.0/devpi_web/templates/error.pt
--rw-r--r--   0 fschulze   (501) staff       (20)     3600 2022-12-05 10:10:32.000000 devpi-web-4.2.0/devpi_web/templates/index.pt
--rw-r--r--   0 fschulze   (501) staff       (20)     4818 2022-12-05 10:10:32.000000 devpi-web-4.2.0/devpi_web/templates/macros.pt
--rw-r--r--   0 fschulze   (501) staff       (20)      465 2022-12-05 10:10:32.000000 devpi-web-4.2.0/devpi_web/templates/notfound.pt
--rw-r--r--   0 fschulze   (501) staff       (20)     1838 2022-12-05 10:10:32.000000 devpi-web-4.2.0/devpi_web/templates/project.pt
--rw-r--r--   0 fschulze   (501) staff       (20)     1415 2022-12-05 10:10:32.000000 devpi-web-4.2.0/devpi_web/templates/root.pt
--rw-r--r--   0 fschulze   (501) staff       (20)     2237 2022-12-05 10:10:32.000000 devpi-web-4.2.0/devpi_web/templates/search.pt
--rw-r--r--   0 fschulze   (501) staff       (20)      462 2022-12-05 10:10:32.000000 devpi-web-4.2.0/devpi_web/templates/search_help.pt
--rw-r--r--   0 fschulze   (501) staff       (20)     4719 2022-12-05 10:10:32.000000 devpi-web-4.2.0/devpi_web/templates/status.pt
--rw-r--r--   0 fschulze   (501) staff       (20)     1853 2022-12-05 10:10:32.000000 devpi-web-4.2.0/devpi_web/templates/toxresult.pt
--rw-r--r--   0 fschulze   (501) staff       (20)     2418 2022-12-05 10:10:32.000000 devpi-web-4.2.0/devpi_web/templates/toxresults.pt
--rw-r--r--   0 fschulze   (501) staff       (20)     1278 2022-12-05 10:10:32.000000 devpi-web-4.2.0/devpi_web/templates/user.pt
--rw-r--r--   0 fschulze   (501) staff       (20)     4934 2022-12-05 10:10:32.000000 devpi-web-4.2.0/devpi_web/templates/version.pt
--rw-r--r--   0 fschulze   (501) staff       (20)    43032 2022-12-05 10:10:32.000000 devpi-web-4.2.0/devpi_web/views.py
--rw-r--r--   0 fschulze   (501) staff       (20)    36745 2022-12-05 10:10:32.000000 devpi-web-4.2.0/devpi_web/whoosh_index.py
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2022-12-05 10:10:40.038981 devpi-web-4.2.0/devpi_web.egg-info/
--rw-r--r--   0 fschulze   (501) staff       (20)     4329 2022-12-05 10:10:40.000000 devpi-web-4.2.0/devpi_web.egg-info/PKG-INFO
--rw-r--r--   0 fschulze   (501) staff       (20)     1376 2022-12-05 10:10:40.000000 devpi-web-4.2.0/devpi_web.egg-info/SOURCES.txt
--rw-r--r--   0 fschulze   (501) staff       (20)        1 2022-12-05 10:10:40.000000 devpi-web-4.2.0/devpi_web.egg-info/dependency_links.txt
--rw-r--r--   0 fschulze   (501) staff       (20)      257 2022-12-05 10:10:40.000000 devpi-web-4.2.0/devpi_web.egg-info/entry_points.txt
--rw-r--r--   0 fschulze   (501) staff       (20)        1 2022-12-05 10:10:39.000000 devpi-web-4.2.0/devpi_web.egg-info/not-zip-safe
--rw-r--r--   0 fschulze   (501) staff       (20)      171 2022-12-05 10:10:40.000000 devpi-web-4.2.0/devpi_web.egg-info/requires.txt
--rw-r--r--   0 fschulze   (501) staff       (20)       10 2022-12-05 10:10:40.000000 devpi-web-4.2.0/devpi_web.egg-info/top_level.txt
--rw-r--r--   0 fschulze   (501) staff       (20)      546 2022-12-05 10:10:32.000000 devpi-web-4.2.0/pyproject.toml
--rw-r--r--   0 fschulze   (501) staff       (20)       86 2022-12-05 10:10:40.048595 devpi-web-4.2.0/setup.cfg
--rw-r--r--   0 fschulze   (501) staff       (20)     2653 2022-12-05 10:10:32.000000 devpi-web-4.2.0/setup.py
-drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2022-12-05 10:10:40.047764 devpi-web-4.2.0/tests/
--rw-r--r--   0 fschulze   (501) staff       (20)     1732 2022-12-05 10:10:32.000000 devpi-web-4.2.0/tests/conftest.py
--rw-r--r--   0 fschulze   (501) staff       (20)     4002 2022-12-05 10:10:32.000000 devpi-web-4.2.0/tests/test_indexing.py
--rw-r--r--   0 fschulze   (501) staff       (20)     7000 2022-12-05 10:10:32.000000 devpi-web-4.2.0/tests/test_main.py
--rw-r--r--   0 fschulze   (501) staff       (20)     1378 2022-12-05 10:10:32.000000 devpi-web-4.2.0/tests/test_theme.py
--rw-r--r--   0 fschulze   (501) staff       (20)    30146 2022-12-05 10:10:32.000000 devpi-web-4.2.0/tests/test_views.py
--rw-r--r--   0 fschulze   (501) staff       (20)    11331 2022-12-05 10:10:32.000000 devpi-web-4.2.0/tests/test_views_docs.py
--rw-r--r--   0 fschulze   (501) staff       (20)    14749 2022-12-05 10:10:32.000000 devpi-web-4.2.0/tests/test_views_misc.py
--rw-r--r--   0 fschulze   (501) staff       (20)    14093 2022-12-05 10:10:32.000000 devpi-web-4.2.0/tests/test_views_search.py
--rw-r--r--   0 fschulze   (501) staff       (20)     9458 2022-12-05 10:10:32.000000 devpi-web-4.2.0/tests/test_views_toxresults.py
--rw-r--r--   0 fschulze   (501) staff       (20)    17960 2022-12-05 10:10:32.000000 devpi-web-4.2.0/tests/test_whoosh_index.py
--rw-r--r--   0 fschulze   (501) staff       (20)      943 2022-12-05 10:10:32.000000 devpi-web-4.2.0/tox.ini
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-07-02 12:03:58.274925 devpi-web-4.2.1/
+-rw-r--r--   0 fschulze   (501) staff       (20)       80 2023-07-02 12:03:52.000000 devpi-web-4.2.1/AUTHORS
+-rw-r--r--   0 fschulze   (501) staff       (20)    15164 2023-07-02 12:03:52.000000 devpi-web-4.2.1/CHANGELOG
+-rw-r--r--   0 fschulze   (501) staff       (20)     1061 2023-07-02 12:03:52.000000 devpi-web-4.2.1/LICENSE
+-rw-r--r--   0 fschulze   (501) staff       (20)      144 2023-07-02 12:03:52.000000 devpi-web-4.2.1/MANIFEST.in
+-rw-r--r--   0 fschulze   (501) staff       (20)     4420 2023-07-02 12:03:58.275063 devpi-web-4.2.1/PKG-INFO
+-rw-r--r--   0 fschulze   (501) staff       (20)     1122 2023-07-02 12:03:52.000000 devpi-web-4.2.1/README.rst
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-07-02 12:03:58.262475 devpi-web-4.2.1/devpi_web/
+-rw-r--r--   0 fschulze   (501) staff       (20)       22 2023-07-02 12:03:52.000000 devpi-web-4.2.1/devpi_web/__init__.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     1575 2023-07-02 12:03:52.000000 devpi-web-4.2.1/devpi_web/clear_index.py
+-rw-r--r--   0 fschulze   (501) staff       (20)      723 2023-07-02 12:03:52.000000 devpi-web-4.2.1/devpi_web/config.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     2921 2023-07-02 12:03:52.000000 devpi-web-4.2.1/devpi_web/description.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     8125 2023-07-02 12:03:52.000000 devpi-web-4.2.1/devpi_web/doczip.py
+-rw-r--r--   0 fschulze   (501) staff       (20)      785 2023-07-02 12:03:52.000000 devpi-web-4.2.1/devpi_web/hookspecs.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     3568 2023-07-02 12:03:52.000000 devpi-web-4.2.1/devpi_web/indexing.py
+-rw-r--r--   0 fschulze   (501) staff       (20)    12923 2023-07-02 12:03:52.000000 devpi-web-4.2.1/devpi_web/main.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     1940 2023-07-02 12:03:52.000000 devpi-web-4.2.1/devpi_web/null_index.py
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-07-02 12:03:58.266169 devpi-web-4.2.1/devpi_web/static/
+-rw-r--r--   0 fschulze   (501) staff       (20)     1580 2023-07-02 12:03:52.000000 devpi-web-4.2.1/devpi_web/static/common.js
+-rw-r--r--   0 fschulze   (501) staff       (20)     3477 2023-07-02 12:03:52.000000 devpi-web-4.2.1/devpi_web/static/docview.js
+-rw-r--r--   0 fschulze   (501) staff       (20)    15086 2023-07-02 12:03:52.000000 devpi-web-4.2.1/devpi_web/static/favicon.ico
+-rw-r--r--   0 fschulze   (501) staff       (20)    89501 2023-07-02 12:03:52.000000 devpi-web-4.2.1/devpi_web/static/jquery-3.6.0.min.js
+-rw-r--r--   0 fschulze   (501) staff       (20)    10274 2023-07-02 12:03:52.000000 devpi-web-4.2.1/devpi_web/static/style.css
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-07-02 12:03:58.270973 devpi-web-4.2.1/devpi_web/templates/
+-rw-r--r--   0 fschulze   (501) staff       (20)     1410 2023-07-02 12:03:52.000000 devpi-web-4.2.1/devpi_web/templates/doc.pt
+-rw-r--r--   0 fschulze   (501) staff       (20)      467 2023-07-02 12:03:52.000000 devpi-web-4.2.1/devpi_web/templates/error.pt
+-rw-r--r--   0 fschulze   (501) staff       (20)     3600 2023-07-02 12:03:52.000000 devpi-web-4.2.1/devpi_web/templates/index.pt
+-rw-r--r--   0 fschulze   (501) staff       (20)     4818 2023-07-02 12:03:52.000000 devpi-web-4.2.1/devpi_web/templates/macros.pt
+-rw-r--r--   0 fschulze   (501) staff       (20)      465 2023-07-02 12:03:52.000000 devpi-web-4.2.1/devpi_web/templates/notfound.pt
+-rw-r--r--   0 fschulze   (501) staff       (20)     1838 2023-07-02 12:03:52.000000 devpi-web-4.2.1/devpi_web/templates/project.pt
+-rw-r--r--   0 fschulze   (501) staff       (20)     1415 2023-07-02 12:03:52.000000 devpi-web-4.2.1/devpi_web/templates/root.pt
+-rw-r--r--   0 fschulze   (501) staff       (20)     2237 2023-07-02 12:03:52.000000 devpi-web-4.2.1/devpi_web/templates/search.pt
+-rw-r--r--   0 fschulze   (501) staff       (20)      462 2023-07-02 12:03:52.000000 devpi-web-4.2.1/devpi_web/templates/search_help.pt
+-rw-r--r--   0 fschulze   (501) staff       (20)     4719 2023-07-02 12:03:52.000000 devpi-web-4.2.1/devpi_web/templates/status.pt
+-rw-r--r--   0 fschulze   (501) staff       (20)     1853 2023-07-02 12:03:52.000000 devpi-web-4.2.1/devpi_web/templates/toxresult.pt
+-rw-r--r--   0 fschulze   (501) staff       (20)     2418 2023-07-02 12:03:52.000000 devpi-web-4.2.1/devpi_web/templates/toxresults.pt
+-rw-r--r--   0 fschulze   (501) staff       (20)     1278 2023-07-02 12:03:52.000000 devpi-web-4.2.1/devpi_web/templates/user.pt
+-rw-r--r--   0 fschulze   (501) staff       (20)     4934 2023-07-02 12:03:52.000000 devpi-web-4.2.1/devpi_web/templates/version.pt
+-rw-r--r--   0 fschulze   (501) staff       (20)    43032 2023-07-02 12:03:52.000000 devpi-web-4.2.1/devpi_web/views.py
+-rw-r--r--   0 fschulze   (501) staff       (20)    36687 2023-07-02 12:03:52.000000 devpi-web-4.2.1/devpi_web/whoosh_index.py
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-07-02 12:03:58.264580 devpi-web-4.2.1/devpi_web.egg-info/
+-rw-r--r--   0 fschulze   (501) staff       (20)     4420 2023-07-02 12:03:58.000000 devpi-web-4.2.1/devpi_web.egg-info/PKG-INFO
+-rw-r--r--   0 fschulze   (501) staff       (20)     1376 2023-07-02 12:03:58.000000 devpi-web-4.2.1/devpi_web.egg-info/SOURCES.txt
+-rw-r--r--   0 fschulze   (501) staff       (20)        1 2023-07-02 12:03:58.000000 devpi-web-4.2.1/devpi_web.egg-info/dependency_links.txt
+-rw-r--r--   0 fschulze   (501) staff       (20)      257 2023-07-02 12:03:58.000000 devpi-web-4.2.1/devpi_web.egg-info/entry_points.txt
+-rw-r--r--   0 fschulze   (501) staff       (20)        1 2023-07-02 12:03:58.000000 devpi-web-4.2.1/devpi_web.egg-info/not-zip-safe
+-rw-r--r--   0 fschulze   (501) staff       (20)      180 2023-07-02 12:03:58.000000 devpi-web-4.2.1/devpi_web.egg-info/requires.txt
+-rw-r--r--   0 fschulze   (501) staff       (20)       10 2023-07-02 12:03:58.000000 devpi-web-4.2.1/devpi_web.egg-info/top_level.txt
+-rw-r--r--   0 fschulze   (501) staff       (20)      546 2023-07-02 12:03:52.000000 devpi-web-4.2.1/pyproject.toml
+-rw-r--r--   0 fschulze   (501) staff       (20)       86 2023-07-02 12:03:58.275518 devpi-web-4.2.1/setup.cfg
+-rw-r--r--   0 fschulze   (501) staff       (20)     2662 2023-07-02 12:03:52.000000 devpi-web-4.2.1/setup.py
+drwxr-xr-x   0 fschulze   (501) staff       (20)        0 2023-07-02 12:03:58.274627 devpi-web-4.2.1/tests/
+-rw-r--r--   0 fschulze   (501) staff       (20)     1732 2023-07-02 12:03:52.000000 devpi-web-4.2.1/tests/conftest.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     4002 2023-07-02 12:03:52.000000 devpi-web-4.2.1/tests/test_indexing.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     6978 2023-07-02 12:03:52.000000 devpi-web-4.2.1/tests/test_main.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     1379 2023-07-02 12:03:52.000000 devpi-web-4.2.1/tests/test_theme.py
+-rw-r--r--   0 fschulze   (501) staff       (20)    30014 2023-07-02 12:03:52.000000 devpi-web-4.2.1/tests/test_views.py
+-rw-r--r--   0 fschulze   (501) staff       (20)    11471 2023-07-02 12:03:52.000000 devpi-web-4.2.1/tests/test_views_docs.py
+-rw-r--r--   0 fschulze   (501) staff       (20)    15385 2023-07-02 12:03:52.000000 devpi-web-4.2.1/tests/test_views_misc.py
+-rw-r--r--   0 fschulze   (501) staff       (20)    14095 2023-07-02 12:03:52.000000 devpi-web-4.2.1/tests/test_views_search.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     9459 2023-07-02 12:03:52.000000 devpi-web-4.2.1/tests/test_views_toxresults.py
+-rw-r--r--   0 fschulze   (501) staff       (20)    17960 2023-07-02 12:03:52.000000 devpi-web-4.2.1/tests/test_whoosh_index.py
+-rw-r--r--   0 fschulze   (501) staff       (20)     1047 2023-07-02 12:03:52.000000 devpi-web-4.2.1/tox.ini
```

### Comparing `devpi-web-4.2.0/CHANGELOG` & `devpi-web-4.2.1/CHANGELOG`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,22 @@
 
 
 .. towncrier release notes start
 
+4.2.1 (2023-07-02)
+==================
+
+Bug Fixes
+---------
+
+- Fix #953: Exception when browsers send ETag for documentation pages.
+
+- Fix #980: Remove long deprecated backward compatibility for old pluggy versions to fix error with pluggy 1.1.0.
+
+
 4.2.0 (2022-12-05)
 ==================
 
 Features
 --------
 
 - Set ETag header to the doczip hash and max-age to 60 seconds for all documentation files.
```

### Comparing `devpi-web-4.2.0/LICENSE` & `devpi-web-4.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `devpi-web-4.2.0/PKG-INFO` & `devpi-web-4.2.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devpi-web
-Version: 4.2.0
+Version: 4.2.1
 Summary: devpi-web: a web view for devpi-server
 Home-page: https://devpi.net
 Maintainer: Florian Schulze
 Maintainer-email: mail@pyfidelity.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/devpi/devpi/issues
 Project-URL: Changelog, https://github.com/devpi/devpi/blob/main/web/CHANGELOG
@@ -72,14 +72,25 @@
 Changelog
 =========
 
 
 
 .. towncrier release notes start
 
+4.2.1 (2023-07-02)
+==================
+
+Bug Fixes
+---------
+
+- Fix #953: Exception when browsers send ETag for documentation pages.
+
+- Fix #980: Remove long deprecated backward compatibility for old pluggy versions to fix error with pluggy 1.1.0.
+
+
 4.2.0 (2022-12-05)
 ==================
 
 Features
 --------
 
 - Set ETag header to the doczip hash and max-age to 60 seconds for all documentation files.
@@ -138,16 +149,7 @@
 ==================
 
 Bug Fixes
 ---------
 
 - On startup loop over mirror indexes last to avoid filling up the indexing queue, which processes non mirror indexes first.
 
-
-4.0.7 (2021-07-11)
-==================
-
-Bug Fixes
----------
-
-- The "Not Found" view now works correctly with request methods other than GET, HEAD and POST.
-
```

### Comparing `devpi-web-4.2.0/README.rst` & `devpi-web-4.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `devpi-web-4.2.0/devpi_web/clear_index.py` & `devpi-web-4.2.1/devpi_web/clear_index.py`

 * *Files identical despite different names*

### Comparing `devpi-web-4.2.0/devpi_web/description.py` & `devpi-web-4.2.1/devpi_web/description.py`

 * *Files identical despite different names*

### Comparing `devpi-web-4.2.0/devpi_web/doczip.py` & `devpi-web-4.2.1/devpi_web/doczip.py`

 * *Files identical despite different names*

### Comparing `devpi-web-4.2.0/devpi_web/hookspecs.py` & `devpi-web-4.2.1/devpi_web/hookspecs.py`

 * *Files identical despite different names*

### Comparing `devpi-web-4.2.0/devpi_web/indexing.py` & `devpi-web-4.2.1/devpi_web/indexing.py`

 * *Files identical despite different names*

### Comparing `devpi-web-4.2.0/devpi_web/main.py` & `devpi-web-4.2.1/devpi_web/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -235,27 +235,14 @@
     # by using include, the package name doesn't need to be set explicitly
     # for registrations of static views etc
     pyramid_config.include('devpi_web.main')
     pyramid_config.registry['devpiweb-pluginmanager'] = get_pluginmanager(config)
     xom = pyramid_config.registry['xom']
     pyramid_config.registry['search_index'] = get_indexer(xom)
 
-    # monkeypatch mimetypes.guess_type on because pyramid-1.5.1/webob
-    # choke on mimtypes.guess_type on windows with python2.7
-    if sys.platform == "win32" and sys.version_info[:2] == (2, 7):
-        import mimetypes
-        old = mimetypes.guess_type
-
-        def guess_type_str(url, strict=True):
-            res = old(url, strict)
-            return str(res[0]), res[1]
-
-        mimetypes.guess_type = guess_type_str
-        threadlog.debug("monkeypatched mimetypes.guess_type to return bytes")
-
 
 @devpiserver_hookimpl
 def devpiserver_add_parser_options(parser):
     theme = parser.addgroup("devpi-web theme options")
     theme.addoption(
         "--theme", action="store",
         help="folder with template and resource overwrites for the web interface")
@@ -303,16 +290,15 @@
 
 
 @devpiserver_hookimpl
 def devpiserver_cmdline_run(xom):
     docs_path = xom.config.args.documentation_path
     if docs_path is not None and not os.path.isabs(docs_path):
         fatal("The path for unzipped documentation must be absolute.")
-    # allow devpi-server to run
-    return None
+    # return None to allow devpi-server to run
 
 
 def delete_project(stage, name):
     if stage is None:
         return
     ix = get_indexer(stage.xom)
     ix.delete_projects([ProjectIndexingInfo(stage=stage, name=name)])
```

### Comparing `devpi-web-4.2.0/devpi_web/null_index.py` & `devpi-web-4.2.1/devpi_web/null_index.py`

 * *Files identical despite different names*

### Comparing `devpi-web-4.2.0/devpi_web/static/common.js` & `devpi-web-4.2.1/devpi_web/static/common.js`

 * *Files identical despite different names*

### Comparing `devpi-web-4.2.0/devpi_web/static/docview.js` & `devpi-web-4.2.1/devpi_web/static/docview.js`

 * *Files identical despite different names*

### Comparing `devpi-web-4.2.0/devpi_web/static/favicon.ico` & `devpi-web-4.2.1/devpi_web/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `devpi-web-4.2.0/devpi_web/static/jquery-3.6.0.min.js` & `devpi-web-4.2.1/devpi_web/static/jquery-3.6.0.min.js`

 * *Files identical despite different names*

### Comparing `devpi-web-4.2.0/devpi_web/static/style.css` & `devpi-web-4.2.1/devpi_web/static/style.css`

 * *Files identical despite different names*

### Comparing `devpi-web-4.2.0/devpi_web/templates/doc.pt` & `devpi-web-4.2.1/devpi_web/templates/doc.pt`

 * *Files identical despite different names*

### Comparing `devpi-web-4.2.0/devpi_web/templates/index.pt` & `devpi-web-4.2.1/devpi_web/templates/index.pt`

 * *Files identical despite different names*

### Comparing `devpi-web-4.2.0/devpi_web/templates/macros.pt` & `devpi-web-4.2.1/devpi_web/templates/macros.pt`

 * *Files identical despite different names*

### Comparing `devpi-web-4.2.0/devpi_web/templates/project.pt` & `devpi-web-4.2.1/devpi_web/templates/project.pt`

 * *Files identical despite different names*

### Comparing `devpi-web-4.2.0/devpi_web/templates/root.pt` & `devpi-web-4.2.1/devpi_web/templates/root.pt`

 * *Files identical despite different names*

### Comparing `devpi-web-4.2.0/devpi_web/templates/search.pt` & `devpi-web-4.2.1/devpi_web/templates/search.pt`

 * *Files identical despite different names*

### Comparing `devpi-web-4.2.0/devpi_web/templates/status.pt` & `devpi-web-4.2.1/devpi_web/templates/status.pt`

 * *Files identical despite different names*

### Comparing `devpi-web-4.2.0/devpi_web/templates/toxresult.pt` & `devpi-web-4.2.1/devpi_web/templates/toxresult.pt`

 * *Files identical despite different names*

### Comparing `devpi-web-4.2.0/devpi_web/templates/toxresults.pt` & `devpi-web-4.2.1/devpi_web/templates/toxresults.pt`

 * *Files identical despite different names*

### Comparing `devpi-web-4.2.0/devpi_web/templates/user.pt` & `devpi-web-4.2.1/devpi_web/templates/user.pt`

 * *Files identical despite different names*

### Comparing `devpi-web-4.2.0/devpi_web/templates/version.pt` & `devpi-web-4.2.1/devpi_web/templates/version.pt`

 * *Files identical despite different names*

### Comparing `devpi-web-4.2.0/devpi_web/views.py` & `devpi-web-4.2.1/devpi_web/views.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -169,20 +169,20 @@
         content_type = 'application/octet-stream'
     return (content_type, content_encoding)
 
 
 @view_config(route_name="docroot", request_method="GET")
 def doc_serve(context, request):
     """ Serves the raw documentation files. """
+    context = ContextWrapper(context)
     if_none_match = request.if_none_match
     if if_none_match:
         doc_info = get_doc_info(context, request, check_content=False)
         if doc_info['etag'] in if_none_match.etags:
             return HTTPNotModified()
-    context = ContextWrapper(context)
     doc_info = get_doc_info(context, request)
     if doc_info['doc_path'] is None:
         relpath = request.matchdict['relpath']
         (content_type, content_encoding) = _guess_type(relpath)
         response = Response(
             body=doc_info['body'],
             conditional_response=True,
```

### Comparing `devpi-web-4.2.0/devpi_web/whoosh_index.py` & `devpi-web-4.2.1/devpi_web/whoosh_index.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,20 +31,14 @@
 import traceback
 
 
 hookimpl = HookimplMarker("devpiweb")
 devpiserver_hookimpl = HookimplMarker("devpiserver")
 
 
-try:
-    xrange
-except NameError:
-    xrange = range
-
-
 class ProjectNameTokenizer(Tokenizer):
     def __init__(self):
         self.expression = rcompile(r'(\W|_)')
 
     def __eq__(self, other):
         if self.__class__ is other.__class__:
             if self.expression.pattern == other.expression.pattern:
@@ -156,23 +150,23 @@
                 startchar = t.startchar
             # Token positions don't mean much for N-grams,
             # so we'll leave the token's original position
             # untouched.
 
             if t.mode == "query":
                 size = min(self.max, len(t.text))
-                for start in xrange(0, len_text - size + 1):
+                for start in range(0, len_text - size + 1):
                     t.text = text[start:start + size]
                     if chars:
                         t.startchar = startchar + start
                         t.endchar = startchar + start + size
                     yield t
             else:
-                for start in xrange(0, len_text - self.min + 1):
-                    for size in xrange(self.min, self.max + 1):
+                for start in range(0, len_text - self.min + 1):
+                    for size in range(self.min, self.max + 1):
                         end = start + size
                         if end > len_text:
                             continue
 
                         t.text = text[start:end]
 
                         if chars:
```

### Comparing `devpi-web-4.2.0/devpi_web.egg-info/PKG-INFO` & `devpi-web-4.2.1/devpi_web.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devpi-web
-Version: 4.2.0
+Version: 4.2.1
 Summary: devpi-web: a web view for devpi-server
 Home-page: https://devpi.net
 Maintainer: Florian Schulze
 Maintainer-email: mail@pyfidelity.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/devpi/devpi/issues
 Project-URL: Changelog, https://github.com/devpi/devpi/blob/main/web/CHANGELOG
@@ -72,14 +72,25 @@
 Changelog
 =========
 
 
 
 .. towncrier release notes start
 
+4.2.1 (2023-07-02)
+==================
+
+Bug Fixes
+---------
+
+- Fix #953: Exception when browsers send ETag for documentation pages.
+
+- Fix #980: Remove long deprecated backward compatibility for old pluggy versions to fix error with pluggy 1.1.0.
+
+
 4.2.0 (2022-12-05)
 ==================
 
 Features
 --------
 
 - Set ETag header to the doczip hash and max-age to 60 seconds for all documentation files.
@@ -138,16 +149,7 @@
 ==================
 
 Bug Fixes
 ---------
 
 - On startup loop over mirror indexes last to avoid filling up the indexing queue, which processes non mirror indexes first.
 
-
-4.0.7 (2021-07-11)
-==================
-
-Bug Fixes
----------
-
-- The "Not Found" view now works correctly with request methods other than GET, HEAD and POST.
-
```

### Comparing `devpi-web-4.2.0/devpi_web.egg-info/SOURCES.txt` & `devpi-web-4.2.1/devpi_web.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `devpi-web-4.2.0/pyproject.toml` & `devpi-web-4.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `devpi-web-4.2.0/setup.py` & `devpi-web-4.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     url="https://devpi.net",
     project_urls={
         'Bug Tracker': 'https://github.com/devpi/devpi/issues',
         'Changelog': 'https://github.com/devpi/devpi/blob/main/web/CHANGELOG',
         'Documentation': 'https://doc.devpi.net',
         'Source Code': 'https://github.com/devpi/devpi'
     },
-    version='4.2.0',
+    version='4.2.1',
     maintainer="Florian Schulze",
     maintainer_email="mail@pyfidelity.com",
     license="MIT",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Web Environment",
         "Intended Audience :: Developers",
@@ -57,15 +57,15 @@
             "devpi-web = devpi_web.main",
             "devpi-web-whoosh = devpi_web.whoosh_index"],
         'devpi_web': [
             "devpi-web-null = devpi_web.null_index",
             "devpi-web-whoosh = devpi_web.whoosh_index"]},
     install_requires=[
         'Whoosh<3',
-        'beautifulsoup4>=4.3.2',
+        'beautifulsoup4>=4.3.2,!=4.12.1',
         'defusedxml',
         'devpi-server>=5.2.0',
         'devpi-common>=3.2.0',
         'docutils>=0.11',
         'pygments>=1.6',
         'pyramid!=1.10a1',
         'pyramid-chameleon',
```

### Comparing `devpi-web-4.2.0/tests/conftest.py` & `devpi-web-4.2.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `devpi-web-4.2.0/tests/test_indexing.py` & `devpi-web-4.2.1/tests/test_indexing.py`

 * *Files identical despite different names*

### Comparing `devpi-web-4.2.0/tests/test_main.py` & `devpi-web-4.2.1/tests/test_main.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 
 def test_pkgresources_version_matches_init():
     import devpi_web
     try:
         import importlib.metadata as importlib_metadata
     except ImportError:
-        import importlib_metadata as importlib_metadata
+        import importlib_metadata
     ver = devpi_web.__version__
     assert importlib_metadata.version("devpi-web") == ver
 
 
 def test_devpi_mirror_initialnames(caplog, pypistage):
     import logging
     caplog.set_level(logging.NOTSET)
```

### Comparing `devpi-web-4.2.0/tests/test_theme.py` & `devpi-web-4.2.1/tests/test_theme.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 <metal:head define-macro="headcss" use-macro="request.macros['original-headcss']">
     <metal:mycss fill-slot="headcss">
         <link rel="stylesheet" type="text/css" href="${request.theme_static_url('style.css')}" />
     </metal:mycss>
 </metal:head>
     """)
     r = testapp.get('/')
-    styles = [x.attrs.get('href') for x in r.html.findAll('link')]
+    styles = [x.attrs.get('href') for x in r.html.find_all('link')]
     assert 'http://localhost/+static-%s/style.css' % __version__ in styles
     assert 'http://localhost/+theme-static-%s/style.css' % __version__ in styles
 
 
 def test_template_overwrite(testapp, themedir):
     themedir.join('templates', 'root.pt').write("Foo Template!")
     r = testapp.get('/')
```

### Comparing `devpi-web-4.2.0/tests/test_views.py` & `devpi-web-4.2.1/tests/test_views.py`

 * *Files 2% similar despite different names*

```diff
@@ -342,17 +342,17 @@
     def gmtime(*x):
         return struct_time((2014, 9, 15, 11, 11, 11, 0, 258, 0))
 
     monkeypatch.setattr('time.gmtime', gmtime)
     monkeypatch.setattr(devpi_server.model, 'gmtime', gmtime)
     api = mapp.create_and_use()
     mapp.upload_file_pypi(
-        "pkg1-2.6.tar.gz", b"contentveryold", "pkg1", "2.6").file_url
+        "pkg1-2.6.tar.gz", b"contentveryold", "pkg1", "2.6")
     mapp.upload_file_pypi(
-        "pkg1-2.6.tar.gz", b"contentold", "pkg1", "2.6").file_url
+        "pkg1-2.6.tar.gz", b"contentold", "pkg1", "2.6")
     tar3 = mapp.upload_file_pypi(
         "pkg1-2.6.tar.gz", b"content", "pkg1", "2.6").file_url
     zip = mapp.upload_file_pypi(
         "pkg1-2.6.zip", b"contentzip", "pkg1", "2.6").file_url
     content = zip_dict({"index.html": "<html/>"})
     mapp.upload_doc("pkg1.zip", content, "pkg1", "2.6", code=200)
     classifiers = ["Intended Audience :: Developers",
@@ -363,26 +363,26 @@
         "author": "Foo Bear",
         "classifiers": classifiers,
         "description": u"föö".encode('utf-8')},
         waithooks=True)
     r = testapp.get(api.index + '/pkg1/2.6', headers=dict(accept="text/html"))
     assert r.status_code == 200
     assert r.html.find('title').text == "user1/dev/: pkg1-2.6 metadata and description"
-    info = dict((compareable_text(t.text) for t in x.findAll('td')) for x in r.html.select('.projectinfos tr'))
+    info = dict((compareable_text(t.text) for t in x.find_all('td')) for x in r.html.select('.projectinfos tr'))
     assert sorted(info.keys()) == ['author', 'classifiers']
     assert info['author'] == 'Foo Bear'
     assert info['classifiers'] == 'Intended Audience :: Developers License :: OSI Approved :: MIT License'
     description = r.html.select('#description')
     assert len(description) == 1
     description = description[0]
-    assert description.renderContents().strip().decode('utf-8') == u'<p>föö</p>'
+    assert description.decode_contents().strip() == '<p>föö</p>'
     filesinfo = [
         tuple(
             compareable_text(t.text).split()
-            for t in x.findAll('td'))
+            for t in x.find_all('td'))
         for x in r.html.select('.files tbody tr')]
 
     assert [x[:2] for x in filesinfo] == [
         (['pkg1-2.6.tar.gz', 'Size', '7', 'bytes', 'Type', 'Source'], []),
         (['pkg1-2.6.zip', 'Size', '10', 'bytes', 'Type', 'Source'], [])
     ]
 
@@ -400,46 +400,46 @@
         ('user1/dev', 'http://localhost/user1/dev')]
 
 
 @pytest.mark.with_notifier
 def test_markdown_description_without_content_type(mapp, testapp, monkeypatch):
     api = mapp.create_and_use()
     mapp.upload_file_pypi(
-        "pkg1-2.6.tar.gz", b"content", "pkg1", "2.6").file_url
+        "pkg1-2.6.tar.gz", b"content", "pkg1", "2.6")
     mapp.set_versiondata({
         "name": "pkg1",
         "version": "2.6",
         "author": "Foo Bear",
         "description": u'# Description'.encode('utf-8')},
         waithooks=True)
     r = testapp.get(api.index + '/pkg1/2.6', headers=dict(accept="text/html"))
 
     description = r.html.select('#description')
     assert len(description) == 1
-    assert '#' in description[0].renderContents().strip().decode('utf-8')
+    assert '#' in description[0].decode_contents()
 
 
 @pytest.mark.with_notifier
 @pytest.mark.skipif(devpi_server_version < parse_version("4.7.2dev"), reason="Needs Metadata 2.1 support")
 def test_markdown_description_with_content_type(mapp, testapp, monkeypatch):
     api = mapp.create_and_use()
     mapp.upload_file_pypi(
-        "pkg1-2.6.tar.gz", b"content", "pkg1", "2.6").file_url
+        "pkg1-2.6.tar.gz", b"content", "pkg1", "2.6")
     mapp.set_versiondata({
         "name": "pkg1",
         "version": "2.6",
         "author": "Foo Bear",
         "description": u'# Description'.encode('utf-8'),
         "description_content_type": 'text/markdown'},
         waithooks=True)
     r = testapp.get(api.index + '/pkg1/2.6', headers=dict(accept="text/html"))
 
     description = r.html.select('#description')
     assert len(description) == 1
-    assert description[0].renderContents().strip().decode('utf-8') == u'<h1>Description</h1>'
+    assert description[0].decode_contents().strip() == '<h1>Description</h1>'
 
 
 @pytest.mark.with_notifier
 def test_version_projectname(mapp, testapp):
     api = mapp.create_and_use()
     mapp.set_versiondata({
         "name": "pkg_hello", "version": "1.0", "description": "foo"})
@@ -453,30 +453,30 @@
 @pytest.mark.with_notifier
 def test_description_updated(mapp, testapp):
     api = mapp.create_and_use()
     mapp.set_versiondata({
         "name": "pkg-hello", "version": "1.0", "description": "foo"})
     r = testapp.xget(200, api.index + "/pkg-hello/1.0", headers=dict(accept="text/html"))
     description, = r.html.select('#description')
-    assert '<p>foo</p>' == description.renderContents().strip().decode('utf-8')
+    assert description.decode_contents().strip() == '<p>foo</p>'
     mapp.set_versiondata({
         "name": "pkg-hello", "version": "1.0", "description": "bar"})
     r = testapp.xget(200, api.index + "/pkg-hello/1.0", headers=dict(accept="text/html"))
     description, = r.html.select('#description')
-    assert '<p>bar</p>' == description.renderContents().strip().decode('utf-8')
+    assert description.decode_contents().strip() == '<p>bar</p>'
 
 
 @pytest.mark.with_notifier
 def test_description_empty(mapp, testapp):
     api = mapp.create_and_use()
     mapp.set_versiondata({
         "name": "pkg-hello", "version": "1.0"})
     r = testapp.xget(200, api.index + "/pkg-hello/1.0", headers=dict(accept="text/html"))
     description, = r.html.select('#description')
-    assert '<p>No description in metadata</p>' == description.renderContents().strip().decode('utf-8')
+    assert description.decode_contents().strip() == '<p>No description in metadata</p>'
 
 
 def test_version_not_found(mapp, testapp):
     api = mapp.create_and_use()
     mapp.upload_file_pypi(
         "pkg1-2.6.tar.gz", b"content", "pkg1", "2.6")
     r = testapp.get("/blubber/blubb/pkg1/2.6", headers=dict(accept="text/html"))
@@ -504,28 +504,28 @@
 
 def test_version_view_root_pypi(mapp, testapp, pypistage):
     pypistage.mock_simple("pkg1", text='''
             <a href="../../pkg/pkg1-2.6.zip" />
         ''', pypiserial=10)
     r = testapp.xget(200, '/root/pypi/pkg1/2.6',
                      headers=dict(accept="text/html"))
-    filesinfo = [tuple(compareable_text(t.text) for t in x.findAll('td')[:3]) for x in r.html.select('.files tbody tr')]
+    filesinfo = [tuple(compareable_text(t.text) for t in x.find_all('td')[:3]) for x in r.html.select('.files tbody tr')]
     assert filesinfo == [('pkg1-2.6.zip Type Source', '')]
     links = {l.text: l.attrs['href'] for l in r.html.select('#content a')}
     assert links["Simple index"] == "http://localhost/root/pypi/+simple/pkg1"
     assert links["pkg1-2.6.zip"].startswith("http://localhost/root/pypi/+e")
     assert "/pkg1" in links["PyPI page"]
 
 
 def test_version_view_root_pypi_external_files(mapp, testapp, pypistage):
     pypistage.mock_simple(
         "pkg1", '<a href="http://example.com/releases/pkg1-2.7.zip" /a>)')
     r = testapp.get('/root/pypi/pkg1/2.7', headers=dict(accept="text/html"))
     assert r.status_code == 200
-    filesinfo = [tuple(compareable_text(t.text) for t in x.findAll('td')[:3])
+    filesinfo = [tuple(compareable_text(t.text) for t in x.find_all('td')[:3])
                  for x in r.html.select('.files tbody tr')]
     assert filesinfo == [('pkg1-2.7.zip Type Source', '')]
     silink, pypi_link, link1, link2 = list(r.html.select("#content a"))
     assert silink.text == "Simple index"
     assert silink.attrs["href"] == "http://localhost/root/pypi/+simple/pkg1"
     assert pypi_link.text == "PyPI page"
     assert "/pkg1" in pypi_link.attrs["href"]
```

### Comparing `devpi-web-4.2.0/tests/test_views_docs.py` & `devpi-web-4.2.1/tests/test_views_docs.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,21 +25,25 @@
     mapp.set_versiondata({"name": "pkg1", "version": "2.6"})
     mapp.upload_doc("pkg1.zip", content, "pkg1", "2.6", code=200,
                     waithooks=True)
     r = testapp.xget(302, api.index + "/pkg1/2.6/+doc/")
     r = testapp.xget(200, r.location)
     assert r.cache_control.no_cache is None
     r = testapp.xget(302, api.index + "/pkg1/latest/+doc/")
-    r = testapp.xget(200, r.location)
+    url = r.location
+    r = testapp.xget(200, url)
     assert r.etag == etag
     assert r.cache_control.max_age == 60
+    r = testapp.xget(304, url, headers={"If-None-Match": r.etag})
     r = testapp.xget(302, api.index + "/pkg1/stable/+doc/")
-    r = testapp.xget(200, r.location)
+    url = r.location
+    r = testapp.xget(200, url)
     assert r.etag == etag
     assert r.cache_control.max_age == 60
+    r = testapp.xget(304, url, headers={"If-None-Match": r.etag})
     r = testapp.xget(404, "/blubber/blubb/pkg1/2.6/+doc/index.html")
     content, = r.html.select('#content')
     assert 'The stage blubber/blubb could not be found.' in compareable_text(content.text)
     r = testapp.xget(404, api.index + "/pkg1/2.7/+doc/index.html")
     content, = r.html.select('#content')
     assert 'No documentation available.' in compareable_text(content.text)
     r = testapp.xget(404, api.index + "/pkg1/2.6/+doc/foo.html")
@@ -52,15 +56,15 @@
     api = mapp.create_and_use()
     content = zip_dict({"index.html": "<html/>"})
     mapp.set_versiondata({"name": "pkg1", "version": "2.6"})
     mapp.upload_doc("pkg1.zip", content, "pkg1", "2.6", code=200,
                     waithooks=True)
     r = testapp.xget(302, api.index + "/pkg1/2.6/+d/")
     r = testapp.xget(200, r.location)
-    iframe, = r.html.findAll('iframe')
+    iframe, = r.html.find_all('iframe')
     assert iframe.attrs['src'] == api.index + "/pkg1/2.6/+doc/index.html"
     r = testapp.xget(404, "/blubber/blubb/pkg1/2.6/+d/index.html")
     content, = r.html.select('#content')
     assert 'The stage blubber/blubb could not be found.' in compareable_text(content.text)
     r = testapp.xget(404, api.index + "/pkg1/2.7/+d/index.html")
     content, = r.html.select('#content')
     assert 'No documentation available.' in compareable_text(content.text)
@@ -85,59 +89,59 @@
     navlinks = dict(
         (l.text, l.attrs['href'])
         for l in r.html.select('.projectnavigation a'))
     assert 'Documentation' in navlinks
     # the regular name should work
     location = '%s/pkg_hello/1.0/+doc/index.html' % api.index
     r = testapp.xget(200, location, headers=dict(accept="text/html"))
-    html = r.html.renderContents().strip().decode('utf-8')
-    assert '<html><body>foo</body></html>' == html
+    html = r.html.decode_contents()
+    assert html.strip() == '<html><body>foo</body></html>'
     # as well as the normalized name
     location = '%s/pkg-hello/1.0/+doc/index.html' % api.index
     r = testapp.xget(200, location, headers=dict(accept="text/html"))
-    html = r.html.renderContents().strip().decode('utf-8')
-    assert '<html><body>foo</body></html>' == html
+    html = r.html.decode_contents()
+    assert html.strip() == '<html><body>foo</body></html>'
 
 
 @pytest.mark.with_notifier
 def test_docs_show_projectname(mapp, testapp):
     api = mapp.create_and_use()
     content = zip_dict({"index.html": "<html><body>foo</body></html>"})
     mapp.set_versiondata({
         "name": "pkg_hello", "version": "1.0"})
     mapp.upload_doc(
         "pkg-hello.zip", content, "pkg-hello", "1.0", code=200, waithooks=True)
     location = '%s/pkg-hello/1.0/+d/index.html' % api.index
     r = testapp.xget(200, location, headers=dict(accept="text/html"))
-    iframe, = r.html.findAll('iframe')
+    iframe, = r.html.find_all('iframe')
     assert iframe.attrs['src'] == api.index + "/pkg-hello/1.0/+doc/index.html"
 
 
 @pytest.mark.with_notifier
 def test_docs_latest(mapp, testapp):
     api = mapp.create_and_use()
     content = zip_dict({"index.html": "<html><body>2.6</body></html>"})
     mapp.set_versiondata({"name": "pkg1", "version": "2.6"})
     mapp.upload_doc("pkg1.zip", content, "pkg1", "2.6", code=200,
                     waithooks=True)
     r = testapp.xget(200, api.index + "/pkg1/latest/+d/index.html")
-    iframe, = r.html.findAll('iframe')
+    iframe, = r.html.find_all('iframe')
     assert iframe.attrs['src'] == api.index + "/pkg1/latest/+doc/index.html"
     # navigation shows latest registered version
     navigation_links = r.html.select("#navigation a")
     assert navigation_links[4].text == '2.6'
     # there is no warning
     assert r.html.select('.infonote') == []
     # and the content matches
     r = testapp.xget(200, iframe.attrs['src'])
     assert r.text == "<html><body>2.6</body></html>"
     # now we register a newer version, but docs should still be 2.6
     mapp.set_versiondata({"name": "pkg1", "version": "2.7"}, waithooks=True)
     r = testapp.xget(200, api.index + "/pkg1/latest/+d/index.html")
-    iframe, = r.html.findAll('iframe')
+    iframe, = r.html.find_all('iframe')
     assert iframe.attrs['src'] == api.index + "/pkg1/latest/+doc/index.html"
     # navigation shows latest registered version
     navigation_links = r.html.select("#navigation a")
     assert navigation_links[4].text == '2.7'
     # there is a warning
     assert [x.text.strip() for x in r.html.select('.infonote')] == [
         "The latest available documentation (version 2.6) isn't for the latest available package version."]
@@ -145,15 +149,15 @@
     r = testapp.xget(200, iframe.attrs['src'])
     assert r.text == "<html><body>2.6</body></html>"
     # now we upload newer docs
     content = zip_dict({"index.html": "<html><body>2.7</body></html>"})
     mapp.upload_doc("pkg1.zip", content, "pkg1", "2.7", code=200,
                     waithooks=True)
     r = testapp.xget(200, api.index + "/pkg1/latest/+d/index.html")
-    iframe, = r.html.findAll('iframe')
+    iframe, = r.html.find_all('iframe')
     assert iframe.attrs['src'] == api.index + "/pkg1/latest/+doc/index.html"
     # navigation shows latest registered version
     navigation_links = r.html.select("#navigation a")
     assert navigation_links[4].text == '2.7'
     # there is no warning anymore
     assert r.html.select('.infonote') == []
     # and the content is from newest docs
@@ -165,57 +169,57 @@
 def test_docs_stable(mapp, testapp):
     api = mapp.create_and_use()
     content = zip_dict({"index.html": "<html><body>2.6</body></html>"})
     mapp.set_versiondata({"name": "pkg1", "version": "2.6"})
     mapp.upload_doc("pkg1.zip", content, "pkg1", "2.6", code=200,
                     waithooks=True)
     r = testapp.xget(200, api.index + "/pkg1/stable/+d/index.html")
-    iframe, = r.html.findAll('iframe')
+    iframe, = r.html.find_all('iframe')
     assert iframe.attrs['src'] == api.index + "/pkg1/stable/+doc/index.html"
     # navigation shows stable registered version
     navigation_links = r.html.select("#navigation a")
     assert navigation_links[4].text == '2.6'
     # there is no warning
     assert r.html.select('.infonote') == []
     # and the content matches
     r = testapp.xget(200, iframe.attrs['src'])
     assert r.text == "<html><body>2.6</body></html>"
     # now we register a newer version, but docs should still be 2.6
     mapp.set_versiondata({"name": "pkg1", "version": "2.7.a1"}, waithooks=True)
     r = testapp.xget(200, api.index + "/pkg1/stable/+d/index.html")
-    iframe, = r.html.findAll('iframe')
+    iframe, = r.html.find_all('iframe')
     assert iframe.attrs['src'] == api.index + "/pkg1/stable/+doc/index.html"
     # navigation shows stable registered version
     navigation_links = r.html.select("#navigation a")
     assert navigation_links[4].text == '2.6'
     # there is no warning
     assert r.html.select('.infonote') == []
     # and the content is also from stable docs
     r = testapp.xget(200, iframe.attrs['src'])
     assert r.text == "<html><body>2.6</body></html>"
     # now we upload newer docs
     content = zip_dict({"index.html": "<html><body>2.7.a1</body></html>"})
     mapp.upload_doc("pkg1.zip", content, "pkg1", "2.7.a1", code=200,
                     waithooks=True)
     r = testapp.xget(200, api.index + "/pkg1/stable/+d/index.html")
-    iframe, = r.html.findAll('iframe')
+    iframe, = r.html.find_all('iframe')
     assert iframe.attrs['src'] == api.index + "/pkg1/stable/+doc/index.html"
     # navigation shows stable registered version
     navigation_links = r.html.select("#navigation a")
     assert navigation_links[4].text == '2.6'
     # showing latest available version
     assert [x.text.strip() for x in r.html.select('.infonote')] == [
         "Latest documentation"]
     # and the content is also still from stable docs
     r = testapp.xget(200, iframe.attrs['src'])
     assert r.text == "<html><body>2.6</body></html>"
     # now we register a newer stable version, but docs should still be 2.6
     mapp.set_versiondata({"name": "pkg1", "version": "2.7"}, waithooks=True)
     r = testapp.xget(200, api.index + "/pkg1/stable/+d/index.html")
-    iframe, = r.html.findAll('iframe')
+    iframe, = r.html.find_all('iframe')
     assert iframe.attrs['src'] == api.index + "/pkg1/stable/+doc/index.html"
     # navigation shows latest registered stable version
     navigation_links = r.html.select("#navigation a")
     assert navigation_links[4].text == '2.7'
     # there is a warning
     assert [x.text.strip() for x in r.html.select('.infonote')] == [
         "The latest available documentation (version 2.6) isn't for the latest available package version.",
@@ -224,15 +228,15 @@
     r = testapp.xget(200, iframe.attrs['src'])
     assert r.text == "<html><body>2.6</body></html>"
     # now we upload newer docs
     content = zip_dict({"index.html": "<html><body>2.7</body></html>"})
     mapp.upload_doc("pkg1.zip", content, "pkg1", "2.7", code=200,
                     waithooks=True)
     r = testapp.xget(200, api.index + "/pkg1/stable/+d/index.html")
-    iframe, = r.html.findAll('iframe')
+    iframe, = r.html.find_all('iframe')
     assert iframe.attrs['src'] == api.index + "/pkg1/stable/+doc/index.html"
     # navigation shows latest registered stable version
     navigation_links = r.html.select("#navigation a")
     assert navigation_links[4].text == '2.7'
     # no warning anymore
     assert r.html.select('.infonote') == []
     # the content is now latest stable docs
```

### Comparing `devpi-web-4.2.0/tests/test_views_misc.py` & `devpi-web-4.2.1/tests/test_views_misc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,18 @@
+from devpi_common.metadata import parse_version
+from devpi_server import __version__ as _devpi_server_version
 from devpi_web.main import hookimpl
 from test_devpi_server.conftest import make_file_url
 import pytest
 import re
 
 
+devpi_server_version = parse_version(_devpi_server_version)
+
+
 def compareable_text(text):
     return re.sub(r'\s+', ' ', text.strip())
 
 
 @pytest.mark.parametrize("input, expected", [
     ((0, 0), []),
     ((1, 0), [0]),
@@ -207,14 +212,24 @@
     r = testapp.get('http://localhost/%s/pkg1/2.6' % api.stagename, follow=False)
     assert r.status_code == 200
     r = testapp.get('http://localhost/%s/pkg1/2.6/' % api.stagename, follow=False)
     assert r.status_code == 302
     assert r.headers["Location"] == 'http://localhost/%s/pkg1/2.6' % api.stagename
 
 
+@pytest.mark.skipif(devpi_server_version < parse_version("6.8.1.dev"), reason="Needs PATH_INFO fix")
+def test_redirects_outside_url(mapp, testapp):
+    headers = {'X-outside-url': 'http://outside.com/foo', 'Host': 'outside.com'}
+    r = testapp.get('/foo', headers=headers, follow=False)
+    assert r.status_code == 200
+    r = testapp.get('/foo/', headers=headers, follow=False)
+    assert r.status_code == 302
+    assert r.location == 'http://outside.com/foo'
+
+
 def test_static_404(testapp):
     from devpi_web import __version__
     r = testapp.xget(404, '/+static-%s/foo.png' % __version__)
     assert [x.text for x in r.html.select('#content p')] == [
         u'The following resource could not be found:',
         u'http://localhost/+static-%s/foo.png' % __version__]
```

### Comparing `devpi-web-4.2.0/tests/test_views_search.py` & `devpi-web-4.2.1/tests/test_views_search.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,15 +111,15 @@
         "description": "bar"})
     mapp.delete_project("pkg1/2.7", waithooks=True)
     indexer_thread = get_indexer(mapp.xom).indexer_thread
     indexer_thread.wait()
     r = testapp.xget(200, '/+search?query=bar%20OR%20foo')
     search_results = r.html.select('.searchresults > dl')
     assert len(search_results) == 1
-    links = search_results[0].findAll('a')
+    links = search_results[0].find_all('a')
     assert [(compareable_text(l.text), l.attrs['href']) for l in links] == [
         ("pkg1-2.6", "http://localhost/user1/dev/pkg1/2.6"),
         ("Summary", "http://localhost/user1/dev/pkg1/2.6#summary")]
 
 
 @pytest.mark.with_notifier
 def test_search_deleted_all_versions(mapp, testapp):
@@ -170,15 +170,15 @@
     mapp.upload_doc("pkg1.zip", content, "pkg1", "2.6", code=200,
                     waithooks=True)
     indexer_thread = get_indexer(mapp.xom).indexer_thread
     indexer_thread.wait()
     r = testapp.xget(200, '/+search?query=Foo')
     search_results = r.html.select('.searchresults > dl > dt')
     assert len(search_results) == 1
-    links = search_results[0].findAll('a')
+    links = search_results[0].find_all('a')
     assert sorted((compareable_text(l.text), l.attrs['href']) for l in links) == [
         ("pkg1-2.6", "http://localhost/user1/dev/pkg1/2.6")]
 
 
 @pytest.mark.with_indexer
 @pytest.mark.with_notifier
 def test_indexing_doc_with_unicode(mapp, testapp):
```

### Comparing `devpi-web-4.2.0/tests/test_views_toxresults.py` & `devpi-web-4.2.1/tests/test_views_toxresults.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     content = "\n".join([compareable_text(x.text) for x in r.html.select('.toxresult')])
     assert "No setup performed" in content
     assert "everything fine" in content
     r = testapp.xget(200, links[1].attrs['href'])
     (row,) = [
         tuple(
             compareable_text(t.text) if len(t.text.split()) < 2 else " ".join(t.text.split())
-            for t in x.findAll('td'))
+            for t in x.find_all('td'))
         for x in r.html.select('tbody tr')]
     assert row[0].startswith("pkg1-2.6.tgz.toxresult")
     assert row[1:] == ("foo", "linux2", "py27", "", "No setup performed Tests")
 
 
 @pytest.mark.with_notifier
 def test_testdata_notfound(mapp, testapp):
```

### Comparing `devpi-web-4.2.0/tests/test_whoosh_index.py` & `devpi-web-4.2.1/tests/test_whoosh_index.py`

 * *Files identical despite different names*

### Comparing `devpi-web-4.2.0/tox.ini` & `devpi-web-4.2.1/tox.ini`

 * *Files 11% similar despite different names*

```diff
@@ -3,28 +3,29 @@
 
 
 [testenv]
 commands =
     !keyfs: py.test --cov {envsitepackagesdir}/devpi_web {posargs}
     keyfs: py.test --backend=devpi_server.keyfs_sqlite {posargs}
 
-passenv = LANG
+passenv = GITHUB_ACTIONS, LANG
 setenv =
     CHAMELEON_CACHE = {envtmpdir}
 
 deps =
     webtest
     mock
     pytest
     pytest-cov
     pytest-flake8
     flake8<5
+    pytest-github-actions-annotate-failures
     server520: devpi-server==5.2.0
-    server520: ruamel.yaml
-    py35: pyparsing<3
+    server520: ruamel.yaml<0.17.22;python_version<"3.6"
+    pyparsing<3;python_version<"3.6"
     importlib.metadata;python_version<"3.8"
 
 
 [pytest]
 addopts = -r a --flake8 --cov-report=term --cov-report=html -W once::DeprecationWarning -W ignore::DeprecationWarning:webob.acceptparse -W ignore::DeprecationWarning:docutils.io -W once::pytest.PytestDeprecationWarning -W once::ResourceWarning
 flake8-ignore =
     * E501 E741 W503
```

