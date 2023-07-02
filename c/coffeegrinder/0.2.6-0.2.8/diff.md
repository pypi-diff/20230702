# Comparing `tmp/coffeegrinder-0.2.6.tar.gz` & `tmp/coffeegrinder-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coffeegrinder-0.2.6.tar", last modified: Sun Jul  2 02:59:59 2023, max compression
+gzip compressed data, was "coffeegrinder-0.2.8.tar", last modified: Sun Jul  2 10:31:50 2023, max compression
```

## Comparing `coffeegrinder-0.2.6.tar` & `coffeegrinder-0.2.8.tar`

### file list

```diff
@@ -1,86 +1,106 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 02:59:59.705159 coffeegrinder-0.2.6/
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-02 02:59:46.000000 coffeegrinder-0.2.6/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 02:59:59.677158 coffeegrinder-0.2.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 02:59:59.689159 coffeegrinder-0.2.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-02 02:59:46.000000 coffeegrinder-0.2.6/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-07-02 02:59:46.000000 coffeegrinder-0.2.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-02 02:59:46.000000 coffeegrinder-0.2.6/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-02 02:59:46.000000 coffeegrinder-0.2.6/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-02 02:59:46.000000 coffeegrinder-0.2.6/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)    13801 2023-07-02 02:59:46.000000 coffeegrinder-0.2.6/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-02 02:59:46.000000 coffeegrinder-0.2.6/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2940 2023-07-02 02:59:59.705159 coffeegrinder-0.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-07-02 02:59:46.000000 coffeegrinder-0.2.6/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 02:59:59.689159 coffeegrinder-0.2.6/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-02 02:59:46.000000 coffeegrinder-0.2.6/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 02:59:59.689159 coffeegrinder-0.2.6/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-02 02:59:46.000000 coffeegrinder-0.2.6/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-02 02:59:46.000000 coffeegrinder-0.2.6/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-02 02:59:46.000000 coffeegrinder-0.2.6/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9729 2023-07-02 02:59:46.000000 coffeegrinder-0.2.6/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-02 02:59:46.000000 coffeegrinder-0.2.6/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-07-02 02:59:46.000000 coffeegrinder-0.2.6/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-02 02:59:46.000000 coffeegrinder-0.2.6/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-02 02:59:46.000000 coffeegrinder-0.2.6/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-02 02:59:46.000000 coffeegrinder-0.2.6/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-07-02 02:59:46.000000 coffeegrinder-0.2.6/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 02:59:59.689159 coffeegrinder-0.2.6/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-07-02 02:59:46.000000 coffeegrinder-0.2.6/scripts/compare.py
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-07-02 02:59:59.709159 coffeegrinder-0.2.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-02 02:59:46.000000 coffeegrinder-0.2.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 02:59:59.681159 coffeegrinder-0.2.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 02:59:59.693159 coffeegrinder-0.2.6/src/coffee/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-02 02:59:46.000000 coffeegrinder-0.2.6/src/coffee/DEPENDENCIES.txt
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-02 02:59:46.000000 coffeegrinder-0.2.6/src/coffee/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 02:59:59.693159 coffeegrinder-0.2.6/src/coffee/actions/
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-02 02:59:46.000000 coffeegrinder-0.2.6/src/coffee/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-07-02 02:59:46.000000 coffeegrinder-0.2.6/src/coffee/actions/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9225 2023-07-02 02:59:47.000000 coffeegrinder-0.2.6/src/coffee/actions/gp_plotter.py
--rw-r--r--   0 runner    (1001) docker     (123)    13497 2023-07-02 02:59:47.000000 coffeegrinder-0.2.6/src/coffee/actions/hdf_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-07-02 02:59:47.000000 coffeegrinder-0.2.6/src/coffee/actions/mpl_plotter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 02:59:59.697159 coffeegrinder-0.2.6/src/coffee/backend/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-02 02:59:47.000000 coffeegrinder-0.2.6/src/coffee/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9657 2023-07-02 02:59:47.000000 coffeegrinder-0.2.6/src/coffee/backend/backend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 02:59:59.697159 coffeegrinder-0.2.6/src/coffee/diffop/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 02:59:47.000000 coffeegrinder-0.2.6/src/coffee/diffop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11945 2023-07-02 02:59:47.000000 coffeegrinder-0.2.6/src/coffee/diffop/fd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 02:59:59.697159 coffeegrinder-0.2.6/src/coffee/diffop/sbp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 02:59:47.000000 coffeegrinder-0.2.6/src/coffee/diffop/sbp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17978 2023-07-02 02:59:47.000000 coffeegrinder-0.2.6/src/coffee/diffop/sbp/dissipation.py
--rw-r--r--   0 runner    (1001) docker     (123)    68798 2023-07-02 02:59:47.000000 coffeegrinder-0.2.6/src/coffee/diffop/sbp/dissipation_testing.nb
--rw-r--r--   0 runner    (1001) docker     (123)    27334 2023-07-02 02:59:47.000000 coffeegrinder-0.2.6/src/coffee/diffop/sbp/sbp.py
--rw-r--r--   0 runner    (1001) docker     (123)     5725 2023-07-02 02:59:47.000000 coffeegrinder-0.2.6/src/coffee/free_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 02:59:59.697159 coffeegrinder-0.2.6/src/coffee/grid/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-02 02:59:47.000000 coffeegrinder-0.2.6/src/coffee/grid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28687 2023-07-02 02:59:47.000000 coffeegrinder-0.2.6/src/coffee/grid/grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     7398 2023-07-02 02:59:47.000000 coffeegrinder-0.2.6/src/coffee/ibvp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 02:59:59.701159 coffeegrinder-0.2.6/src/coffee/io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 02:59:47.000000 coffeegrinder-0.2.6/src/coffee/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32849 2023-07-02 02:59:47.000000 coffeegrinder-0.2.6/src/coffee/io/simulation_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 02:59:59.701159 coffeegrinder-0.2.6/src/coffee/mpi/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 02:59:47.000000 coffeegrinder-0.2.6/src/coffee/mpi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14805 2023-07-02 02:59:47.000000 coffeegrinder-0.2.6/src/coffee/mpi/mpiinterfaces.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 02:59:59.701159 coffeegrinder-0.2.6/src/coffee/solvers/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-02 02:59:47.000000 coffeegrinder-0.2.6/src/coffee/solvers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8879 2023-07-02 02:59:47.000000 coffeegrinder-0.2.6/src/coffee/solvers/solvers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5149 2023-07-02 02:59:47.000000 coffeegrinder-0.2.6/src/coffee/system.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 02:59:59.701159 coffeegrinder-0.2.6/src/coffee/tslices/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 02:59:47.000000 coffeegrinder-0.2.6/src/coffee/tslices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11324 2023-07-02 02:59:47.000000 coffeegrinder-0.2.6/src/coffee/tslices/tslices.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 02:59:59.705159 coffeegrinder-0.2.6/src/coffeegrinder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2940 2023-07-02 02:59:59.000000 coffeegrinder-0.2.6/src/coffeegrinder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-07-02 02:59:59.000000 coffeegrinder-0.2.6/src/coffeegrinder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 02:59:59.000000 coffeegrinder-0.2.6/src/coffeegrinder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 02:59:59.000000 coffeegrinder-0.2.6/src/coffeegrinder.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-02 02:59:59.000000 coffeegrinder-0.2.6/src/coffeegrinder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-02 02:59:59.000000 coffeegrinder-0.2.6/src/coffeegrinder.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 02:59:59.681159 coffeegrinder-0.2.6/systems/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 02:59:59.705159 coffeegrinder-0.2.6/systems/OneDAdvection/
--rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-07-02 02:59:47.000000 coffeegrinder-0.2.6/systems/OneDAdvection/OneDAdvection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-07-02 02:59:47.000000 coffeegrinder-0.2.6/systems/OneDAdvection/OneDAdvection_plotter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5653 2023-07-02 02:59:47.000000 coffeegrinder-0.2.6/systems/OneDAdvection/OneDAdvection_setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 02:59:59.705159 coffeegrinder-0.2.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-07-02 02:59:47.000000 coffeegrinder-0.2.6/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-07-02 02:59:47.000000 coffeegrinder-0.2.6/tests/test_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-07-02 02:59:47.000000 coffeegrinder-0.2.6/tests/test_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-07-02 02:59:47.000000 coffeegrinder-0.2.6/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:31:50.617457 coffeegrinder-0.2.8/
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-02 10:31:38.000000 coffeegrinder-0.2.8/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:31:50.605457 coffeegrinder-0.2.8/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:31:50.609457 coffeegrinder-0.2.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-02 10:31:38.000000 coffeegrinder-0.2.8/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-07-02 10:31:38.000000 coffeegrinder-0.2.8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-02 10:31:38.000000 coffeegrinder-0.2.8/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-02 10:31:38.000000 coffeegrinder-0.2.8/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-02 10:31:38.000000 coffeegrinder-0.2.8/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    13801 2023-07-02 10:31:38.000000 coffeegrinder-0.2.8/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-02 10:31:38.000000 coffeegrinder-0.2.8/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-07-02 10:31:50.617457 coffeegrinder-0.2.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-07-02 10:31:38.000000 coffeegrinder-0.2.8/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:31:50.609457 coffeegrinder-0.2.8/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-02 10:31:38.000000 coffeegrinder-0.2.8/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:31:50.609457 coffeegrinder-0.2.8/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-02 10:31:38.000000 coffeegrinder-0.2.8/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-02 10:31:38.000000 coffeegrinder-0.2.8/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-02 10:31:38.000000 coffeegrinder-0.2.8/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9729 2023-07-02 10:31:38.000000 coffeegrinder-0.2.8/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-02 10:31:38.000000 coffeegrinder-0.2.8/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-07-02 10:31:38.000000 coffeegrinder-0.2.8/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-02 10:31:38.000000 coffeegrinder-0.2.8/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-02 10:31:38.000000 coffeegrinder-0.2.8/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-02 10:31:38.000000 coffeegrinder-0.2.8/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-07-02 10:31:38.000000 coffeegrinder-0.2.8/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:31:50.609457 coffeegrinder-0.2.8/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-07-02 10:31:38.000000 coffeegrinder-0.2.8/scripts/compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-07-02 10:31:50.617457 coffeegrinder-0.2.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-02 10:31:38.000000 coffeegrinder-0.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:31:50.605457 coffeegrinder-0.2.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:31:50.613457 coffeegrinder-0.2.8/src/coffee/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-02 10:31:38.000000 coffeegrinder-0.2.8/src/coffee/DEPENDENCIES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-02 10:31:38.000000 coffeegrinder-0.2.8/src/coffee/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:31:50.613457 coffeegrinder-0.2.8/src/coffee/actions/
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-02 10:31:38.000000 coffeegrinder-0.2.8/src/coffee/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4228 2023-07-02 10:31:38.000000 coffeegrinder-0.2.8/src/coffee/actions/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7831 2023-07-02 10:31:38.000000 coffeegrinder-0.2.8/src/coffee/actions/gp_plotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12908 2023-07-02 10:31:38.000000 coffeegrinder-0.2.8/src/coffee/actions/hdf_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-07-02 10:31:38.000000 coffeegrinder-0.2.8/src/coffee/actions/mpl_plotter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:31:50.613457 coffeegrinder-0.2.8/src/coffee/backend/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-02 10:31:38.000000 coffeegrinder-0.2.8/src/coffee/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9657 2023-07-02 10:31:38.000000 coffeegrinder-0.2.8/src/coffee/backend/backend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:31:50.613457 coffeegrinder-0.2.8/src/coffee/diffop/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 10:31:38.000000 coffeegrinder-0.2.8/src/coffee/diffop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11461 2023-07-02 10:31:38.000000 coffeegrinder-0.2.8/src/coffee/diffop/fd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:31:50.613457 coffeegrinder-0.2.8/src/coffee/diffop/sbp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 10:31:38.000000 coffeegrinder-0.2.8/src/coffee/diffop/sbp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15213 2023-07-02 10:31:38.000000 coffeegrinder-0.2.8/src/coffee/diffop/sbp/dissipation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68798 2023-07-02 10:31:38.000000 coffeegrinder-0.2.8/src/coffee/diffop/sbp/dissipation_testing.nb
+-rw-r--r--   0 runner    (1001) docker     (123)    26519 2023-07-02 10:31:38.000000 coffeegrinder-0.2.8/src/coffee/diffop/sbp/sbp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5724 2023-07-02 10:31:38.000000 coffeegrinder-0.2.8/src/coffee/free_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:31:50.613457 coffeegrinder-0.2.8/src/coffee/grid/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-02 10:31:38.000000 coffeegrinder-0.2.8/src/coffee/grid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28334 2023-07-02 10:31:38.000000 coffeegrinder-0.2.8/src/coffee/grid/grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5706 2023-07-02 10:31:38.000000 coffeegrinder-0.2.8/src/coffee/ibvp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:31:50.613457 coffeegrinder-0.2.8/src/coffee/io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 10:31:38.000000 coffeegrinder-0.2.8/src/coffee/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32830 2023-07-02 10:31:38.000000 coffeegrinder-0.2.8/src/coffee/io/simulation_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:31:50.613457 coffeegrinder-0.2.8/src/coffee/mpi/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 10:31:38.000000 coffeegrinder-0.2.8/src/coffee/mpi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11325 2023-07-02 10:31:38.000000 coffeegrinder-0.2.8/src/coffee/mpi/mpiinterfaces.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:31:50.613457 coffeegrinder-0.2.8/src/coffee/solvers/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-02 10:31:38.000000 coffeegrinder-0.2.8/src/coffee/solvers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8246 2023-07-02 10:31:38.000000 coffeegrinder-0.2.8/src/coffee/solvers/solvers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5138 2023-07-02 10:31:38.000000 coffeegrinder-0.2.8/src/coffee/system.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:31:50.613457 coffeegrinder-0.2.8/src/coffee/tslices/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 10:31:38.000000 coffeegrinder-0.2.8/src/coffee/tslices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11067 2023-07-02 10:31:38.000000 coffeegrinder-0.2.8/src/coffee/tslices/tslices.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:31:50.617457 coffeegrinder-0.2.8/src/coffeegrinder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-07-02 10:31:50.000000 coffeegrinder-0.2.8/src/coffeegrinder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-07-02 10:31:50.000000 coffeegrinder-0.2.8/src/coffeegrinder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 10:31:50.000000 coffeegrinder-0.2.8/src/coffeegrinder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 10:31:50.000000 coffeegrinder-0.2.8/src/coffeegrinder.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-02 10:31:50.000000 coffeegrinder-0.2.8/src/coffeegrinder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-02 10:31:50.000000 coffeegrinder-0.2.8/src/coffeegrinder.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:31:50.609457 coffeegrinder-0.2.8/systems/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:31:50.617457 coffeegrinder-0.2.8/systems/OneDAdvection/
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-07-02 10:31:38.000000 coffeegrinder-0.2.8/systems/OneDAdvection/OneDAdvection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-07-02 10:31:38.000000 coffeegrinder-0.2.8/systems/OneDAdvection/OneDAdvection_plotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5653 2023-07-02 10:31:38.000000 coffeegrinder-0.2.8/systems/OneDAdvection/OneDAdvection_setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:31:50.617457 coffeegrinder-0.2.8/systems/OneDAdvectionMpi_fd/
+-rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-07-02 10:31:38.000000 coffeegrinder-0.2.8/systems/OneDAdvectionMpi_fd/OneDAdvection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-07-02 10:31:38.000000 coffeegrinder-0.2.8/systems/OneDAdvectionMpi_fd/OneDAdvection_plotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5787 2023-07-02 10:31:38.000000 coffeegrinder-0.2.8/systems/OneDAdvectionMpi_fd/OneDAdvection_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-02 10:31:38.000000 coffeegrinder-0.2.8/systems/OneDAdvectionMpi_fd/README.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:31:50.617457 coffeegrinder-0.2.8/systems/OneDAdvectionMpi_sbp/
+-rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-07-02 10:31:38.000000 coffeegrinder-0.2.8/systems/OneDAdvectionMpi_sbp/OneDAdvection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-07-02 10:31:38.000000 coffeegrinder-0.2.8/systems/OneDAdvectionMpi_sbp/OneDAdvection_plotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5641 2023-07-02 10:31:38.000000 coffeegrinder-0.2.8/systems/OneDAdvectionMpi_sbp/OneDAdvection_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-02 10:31:38.000000 coffeegrinder-0.2.8/systems/OneDAdvectionMpi_sbp/README.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:31:50.617457 coffeegrinder-0.2.8/systems/OneDAdvection_fd/
+-rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-07-02 10:31:38.000000 coffeegrinder-0.2.8/systems/OneDAdvection_fd/OneDAdvection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-07-02 10:31:38.000000 coffeegrinder-0.2.8/systems/OneDAdvection_fd/OneDAdvection_plotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4791 2023-07-02 10:31:38.000000 coffeegrinder-0.2.8/systems/OneDAdvection_fd/OneDAdvection_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-02 10:31:38.000000 coffeegrinder-0.2.8/systems/OneDAdvection_fd/README.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:31:50.617457 coffeegrinder-0.2.8/systems/OneDAdvection_sbp/
+-rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-07-02 10:31:38.000000 coffeegrinder-0.2.8/systems/OneDAdvection_sbp/OneDAdvection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-07-02 10:31:38.000000 coffeegrinder-0.2.8/systems/OneDAdvection_sbp/OneDAdvection_plotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4980 2023-07-02 10:31:38.000000 coffeegrinder-0.2.8/systems/OneDAdvection_sbp/OneDAdvection_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-02 10:31:38.000000 coffeegrinder-0.2.8/systems/OneDAdvection_sbp/README.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 10:31:50.617457 coffeegrinder-0.2.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-07-02 10:31:38.000000 coffeegrinder-0.2.8/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-07-02 10:31:38.000000 coffeegrinder-0.2.8/tests/test_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-07-02 10:31:38.000000 coffeegrinder-0.2.8/tests/test_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-07-02 10:31:38.000000 coffeegrinder-0.2.8/tox.ini
```

### Comparing `coffeegrinder-0.2.6/.coveragerc` & `coffeegrinder-0.2.8/.coveragerc`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.2.6/.github/workflows/python-publish.yml` & `coffeegrinder-0.2.8/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.2.6/.gitignore` & `coffeegrinder-0.2.8/.gitignore`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.2.6/.readthedocs.yml` & `coffeegrinder-0.2.8/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.2.6/CONTRIBUTING.rst` & `coffeegrinder-0.2.8/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.2.6/LICENSE.txt` & `coffeegrinder-0.2.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.2.6/PKG-INFO` & `coffeegrinder-0.2.8/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 Metadata-Version: 2.1
 Name: coffeegrinder
-Version: 0.2.6
+Version: 0.2.8
 Summary: COFFEE is an MPI-Parallelised Python package for the numerical evolution of time-dependent differential equations.
 Home-page: https://github.com/coffee-gr/coffee
 Author: Chris Stevens
 Author-email: chris.stevens@canterbury.ac.nz
 License: MIT
 Project-URL: Documentation, https://pyscaffold.org/
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Description-Content-Type: text/x-rst; charset=UTF-8
+Provides-Extra: MPI
+Provides-Extra: JAX
+Provides-Extra: MPI-JAX
 Provides-Extra: testing
 License-File: LICENSE.txt
 
 .. These are examples of badges you might want to add to your README:
    please update the URLs accordingly
 
     .. image:: https://api.cirrus-ci.com/github/<USER>/coffee.svg?branch=main
@@ -48,35 +51,30 @@
 
 
 ======
 coffee
 ======
 
 
-    COFFEE is an MPI-Parallelised Python package for the numerical evolution of time-dependent differential equations.
+COFFEE is an MPI-Parallelised Python package for the numerical evolution of time-dependent differential equations.
 
 
 Installation
 ------------
 
-To use this software, you will need the following dependencies:
+There are four versions of COFFEE, which can include MPI and/or JAX capabilities. These can be installed via
 
-- 
-- HDF library
-
-Please make sure these dependencies are installed before using this software.
+    pip install coffeegrinder
+    pip install coffeegrinder[MPI]
+    pip install coffeegrinder[JAX]
+    pip install coffeegrinder[MPI-JAX]
 
 .. rubric:: Getting started
 
-One needs to point the ``PYTHONPATH`` environment variable to the packages directory. Then the system code can be run with::
-
-    python3.10 -O TwoDAdvection_setup.py
-
-Note that adding a ``-d`` flag to this allows you to see a visualization during the computation. You should see a wave propagating from right to left with varying amplitude.
-
+There is a systems directory that includes commented test cases for the 1D advection equation with a mixture of finite-differencing operators and boundary imposition methods.
 
 .. _pyscaffold-notes:
 
 Note
 ====
 
 This project has been set up using PyScaffold 4.4. For details and usage
```

### Comparing `coffeegrinder-0.2.6/README.rst` & `coffeegrinder-0.2.8/README.rst`

 * *Files 20% similar despite different names*

```diff
@@ -32,35 +32,30 @@
 
 
 ======
 coffee
 ======
 
 
-    COFFEE is an MPI-Parallelised Python package for the numerical evolution of time-dependent differential equations.
+COFFEE is an MPI-Parallelised Python package for the numerical evolution of time-dependent differential equations.
 
 
 Installation
 ------------
 
-To use this software, you will need the following dependencies:
+There are four versions of COFFEE, which can include MPI and/or JAX capabilities. These can be installed via
 
-- 
-- HDF library
-
-Please make sure these dependencies are installed before using this software.
+    pip install coffeegrinder
+    pip install coffeegrinder[MPI]
+    pip install coffeegrinder[JAX]
+    pip install coffeegrinder[MPI-JAX]
 
 .. rubric:: Getting started
 
-One needs to point the ``PYTHONPATH`` environment variable to the packages directory. Then the system code can be run with::
-
-    python3.10 -O TwoDAdvection_setup.py
-
-Note that adding a ``-d`` flag to this allows you to see a visualization during the computation. You should see a wave propagating from right to left with varying amplitude.
-
+There is a systems directory that includes commented test cases for the 1D advection equation with a mixture of finite-differencing operators and boundary imposition methods.
 
 .. _pyscaffold-notes:
 
 Note
 ====
 
 This project has been set up using PyScaffold 4.4. For details and usage
```

### Comparing `coffeegrinder-0.2.6/docs/Makefile` & `coffeegrinder-0.2.8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.2.6/docs/conf.py` & `coffeegrinder-0.2.8/docs/conf.py`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.2.6/docs/index.rst` & `coffeegrinder-0.2.8/docs/index.rst`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.2.6/scripts/compare.py` & `coffeegrinder-0.2.8/scripts/compare.py`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.2.6/setup.cfg` & `coffeegrinder-0.2.8/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -32,14 +32,22 @@
 
 [options.packages.find]
 where = src
 exclude = 
 	tests
 
 [options.extras_require]
+MPI = mpi4py
+JAX = 
+	jax
+	jaxlib
+MPI-JAX = 
+	mpi4py
+	jax
+	jaxlib
 testing = 
 	setuptools
 	pytest
 	pytest-cov
 
 [options.entry_points]
```

### Comparing `coffeegrinder-0.2.6/setup.py` & `coffeegrinder-0.2.8/setup.py`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.2.6/src/coffee/__init__.py` & `coffeegrinder-0.2.8/src/coffee/__init__.py`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.2.6/src/coffee/actions/actions.py` & `coffeegrinder-0.2.8/src/coffee/actions/actions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from builtins import object
 from coffee.backend import backend as be
-import logging
 
 
 class Prototype(object):
     """The prototype of all actions.
 
     This class provides basic functionality that all actions require.
 
@@ -137,12 +136,11 @@
 
     def __init__(self, *args, **kwds):
         """The initialiser for the Info action.
 
         All parameters as given for the initialiser for the
         actions.Prototype action are valid.
         """
-        self.log = logging.getLogger("Info")
         super(Info, self).__init__(*args, **kwds)
 
     def _doit(self, it, u):
-        self.log.info("Iteration: %d, Time: %f" % (it, u.time))
+        pass
```

### Comparing `coffeegrinder-0.2.6/src/coffee/actions/gp_plotter.py` & `coffeegrinder-0.2.8/src/coffee/actions/gp_plotter.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 
 from builtins import str
 from builtins import range
 import time
 import os
 from coffee.backend import backend as be
-import logging
 
 # Gnuplot currently only works with Python 2!
 try:
     import Gnuplot
 except ImportError:
     import sys
 
@@ -77,49 +76,33 @@
             self.delay = kwds.pop("delay")
         else:
             self.delay = 0.0
         self.title = r"Time %f"
         if "title" in kwds:
             self.title = kwds.pop("title")
         self.system = system
-        self.log = logging.getLogger("Plotter1D")
         try:
             if kwds["data_function"] is not None:
                 self.datafunc = kwds.pop("data_function")
             else:
                 self.datafunc = lambda y, x, z: (x.domain.axes[0], x.data)
         except:
             self.datafunc = lambda y, x, z: (x.domain.axes[0], x.data)
-        if __debug__:
-            self.log.debug("Initialising plotter...")
         super(Plotter1D, self).__init__(frequency=frequency, start=start, **kwds)
         self.Device = Gnuplot.Gnuplot()
         g = self.Device
         for arg in args:
             g(arg)
-        if __debug__:
-            self.log.debug("Done.-")
 
     def _doit(self, it, u):
         g = self.Device
-        if __debug__:
-            self.log.debug("Plotting iteration %i with data %s" % (it, str(u)))
         x, f = self.datafunc(it, u, self.system)
         f = be.atleast_2d(f)
-        if __debug__:
-            self.log.debug("Data after processing by self.datafunc is %s" % f)
-            self.log.debug("Shape of domain to plot over is %s" % x.shape)
-            self.log.debug("Domain to plot over is %s" % repr(x))
         graphs = []
         g("set title '" + self.title % u.time + "'")
-        for i, val in enumerate(f):
-            if __debug__:
-                self.log.debug("Shape of data to be plotted is %s" % val.shape)
-                self.log.debug("Data to be plotted is %s" % repr(val))
-            graphs += [Gnuplot.Data(x, val, title="Component %i" % i)]
         g.plot(*graphs)
         time.sleep(self.delay)
 
     def __del__(self):
         del self.Device
 
 
@@ -184,44 +167,30 @@
 
         if "components" in kwds:
             self.components = kwds.pop("components")
         else:
             self.components = None
 
         self.system = kwds.pop("system")
-        self.log = logging.getLogger("Plotter2D")
         try:
             if kwds["data_function"] is not None:
                 self.datafunc = kwds.pop("data_function")
             else:
                 self.datafunc = lambda y, x, z: (x.domain.axes, x.data)
         except:
             self.datafunc = lambda y, x, z: (x.domain.axes, x.data)
 
-        #        if __debug__:
-        #            self.log.debug("Initialising plotter...")
         self.device = Gnuplot.Gnuplot()
         for arg in args:
             self.device(arg)
         super(Plotter2D, self).__init__(**kwds)
 
-    #        if __debug__:
-    #            self.log.debug("Done.-")
-
     def _doit(self, it, u):
-        if __debug__:
-            self.log.debug("Plotting iteration %i with data %s" % (it, str(u)))
         x, f = self.datafunc(it, u, self.system)
         f = be.atleast_2d(f)
-        if __debug__:
-            self.log.debug("Data after processing by self.datafunc is %s" % f)
-            self.log.debug(
-                "Shape of domain to plot over is (%s,%s)"
-                % (x[0].shape[0], x[1].shape[0])
-            )
         graphs = []
         self.device('set title "%s" enhanced' % self.title % (it, u.time))
         for i in range(f.shape[0]):
             if self.components is None:
                 graphs += [
                     Gnuplot.GridData(
                         f[i, :, :],
```

### Comparing `coffeegrinder-0.2.6/src/coffee/actions/hdf_output.py` & `coffeegrinder-0.2.8/src/coffee/actions/hdf_output.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 
 I think of this method as a plugin for the system. The user writes a new output
 method for some kind of new data type in a sub class of SimOutputType and
 'plugs' this method into the 'action' list of SimOutput.
 """
 from builtins import str
 from builtins import object
-import logging
 from coffee.backend import backend as be
 
 from .actions import Prototype
 from ..io.simulation_data import dgTypes, systemD, DataGroup, sysDTypes
 from functools import reduce
 
 
@@ -84,17 +83,14 @@
         overwrite : bool
                     If you are outputting a simulation into an existing hdf
                     file do you want to allow the simulation to overwrite the
                     existing data?
         name : string
             What is the name of this simulation?
         """
-        self.log = logging.getLogger("SimOutput")
-        if __debug__:
-            self.log.debug("Setting up HDF output...")
         super(SimOutput, self).__init__(**kwds)
         if name == None:
             hour = str(time.localtime()[3])
             minute = str(time.localtime()[4])
             second = str(time.localtime()[5])
             name = hour + ":" + minute + ":" + second
         self.name = name
@@ -103,24 +99,17 @@
         self.system = theSystem
         self.domain = theInterval
         self.actions = actionTypes
         self.overwrite = overwrite
         self.cmp_ = cmp_
         for action in actionTypes:
             action.setup(self)
-        if __debug__:
-            self.log.debug("HDF output setup completed.")
 
     def _doit(self, it, u):
-        for action in self.actions:
-            if __debug__:
-                self.log.debug("Outputting %s" % action.groupname)
-            action(it, u)
-            if __debug__:
-                self.log.debug("Output done")
+        pass
 
     class SimOutputType(object):
         """If you want to customise the output to the hdf file subclass this
         class.
 
         This class handles the organisation of the hdf file structure so that
         you don't have to. It slices, it dices, it picks the group to store the
@@ -172,21 +161,18 @@
                 )
             else:
                 self.data_group = DataGroup(
                     parent.hdf.create_group(self.groupname).create_group(parent.name)
                 )
             self.parent = parent
             self.data_group.attrs["cmp"] = parent.cmp_
-            self.log = logging.getLogger(self.groupname)
 
         def __call__(self, it, u):
             for key, value in list(self.derivedAttrs.items()):
                 v = value(it, u, self.parent.system)
-                if __debug__:
-                    self.log.debug("Derived Attrs = %s" % str(v))
                 self.data_group[it].attrs[key] = v
 
     class Data(SimOutputType):
         """Writes out tslices.TimeSlice.data.
 
         This class assumes that tslice.TimeSlice.data has a type that h5py
         understands.
```

### Comparing `coffeegrinder-0.2.6/src/coffee/actions/mpl_plotter.py` & `coffeegrinder-0.2.8/src/coffee/actions/mpl_plotter.py`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.2.6/src/coffee/backend/backend.py` & `coffeegrinder-0.2.8/src/coffee/backend/backend.py`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.2.6/src/coffee/diffop/fd.py` & `coffeegrinder-0.2.8/src/coffee/diffop/fd.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,35 +7,24 @@
 Stencil values are calculated using Fornberg's paper. Code for the
 calculations is available in
 `finite_difference_weights_generator.py` located in Code/Utils.
 See Fornberg's paper for the notation.
 """
 
 from builtins import object
-import numpy as np
-import logging
 from coffee.backend import backend as be
 
-
 ################################################################################
 # Finite difference default ghost point processor
 ################################################################################
-def ghost_point_processor(data, b_values, log=None):
+def ghost_point_processor(data, b_values):
     """A utility function that understands how data defined over ghost points
     for finite difference stencils should be handled when communicated via MPI."""
-    if __debug__ and log:
-        log.debug("original data is " + repr(data))
     for b_slice, b_data in b_values:
-        if __debug__ and log:
-            log.debug("b_slice is %s" % (repr(b_slice)))
-            log.debug("b_data is %s" % (repr(b_data)))
         data[b_slice] = b_data
-    if __debug__ and log:
-        log.debug("new data is " + repr(data))
-
 
 ################################################################################
 # Finite difference stencil base class.
 ################################################################################
 
 
 class FD_stencil(object):
@@ -244,15 +233,15 @@
 class FD_diffop(object):
     """The FD_diffop class represents the action of a collection of
     FD_stencils on a vector of values."""
 
     name = "FD_diffop"
 
     def __init__(self):
-        self.log = logging.getLogger("FD")
+        pass
 
     def __call__(self, u, dx):
         """Gives the result of the linear operator represented by this
         class on a vector of data.
 
         Parameters
         ==========
@@ -264,16 +253,14 @@
         Returns
         =======
         numpy.ndarray:
             The vector of derivatives.
         """
         ru = self.central(u)
         for i, b in self.boundaries:
-            if __debug__:
-                self.log.debug("Applying boundary: i = " + repr(i) + ", b = " + repr(b))
             ru[i] = b(u, apply_at=i)
         return ru / (dx**self.order)
 
     def __str__(self):
         return "Differential operator " % self.name
 
     def save(self):
```

### Comparing `coffeegrinder-0.2.6/src/coffee/diffop/sbp/dissipation.py` & `coffeegrinder-0.2.8/src/coffee/diffop/sbp/dissipation.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,15 @@
 #!/usr/bin/env python
 # encoding: utf-8
 """
 A module that contains dissipation operators for SBP operators.
 """
 
-# import sys
-# import os
-# import unittest
 import math
-import numpy as np
 import abc
-import logging
-
 
 ################################################################################
 # Base classes for SBP artificial dissipation operators
 ################################################################################
 class Diss(object):
     """The parent class for SBP dissipation operators."""
 
@@ -27,55 +21,40 @@
     @abc.abstractmethod
     def __call__(self, u, dx, boundary_ID=None):
         pass
 
     def _consistancy_check(self, u, shape):
         r, c = shape
         if u.shape[0] + 1 <= 2 * c:
-            self.log.error("Domain too small for application of operator")
             raise ValueError("Domain too small for application of operator")
-        if __debug__:
-            self.log.debug("Boundary region r = %s, c = %s" % (r, c))
-            self.log.debug("Array to operate on is = %s" % repr(u))
 
     def __str__(self):
         return "SBP Dissipation operator" % self.name
 
 
 class DissDiag(Diss):
     """A class that represents dissipation operators that are diagonal."""
 
     name = "Dissipation Diagonal Norm"
 
     def __init__(self):
         self.bdyRegion = self.Ql.shape
-        self.log = logging.getLogger("DissDiag")
 
     def __call__(self, u, dx, boundary_ID=None):
         super(DissDiag, self)._consistancy_check(u, self.bdyRegion)
         r, c = self.bdyRegion
         diss_u = be.zeros_like(u)
         diss_u = be.convolve(u, self.A, mode="same")
-        if __debug__:
-            self.log.debug("After convolve: diss_u = %s" % repr(diss_u))
         if boundary_ID is None:
             diss_u[0:r] = be.dot(self.Ql, u[0:c])
             diss_u[-r:] = be.dot(self.Qr, u[-c:])
-            if __debug__:
-                self.log.debug("Applying both boundary region computation")
         elif boundary_ID == grid.LEFT:
             diss_u[0:r] = be.dot(self.Ql, u[0:c])
-            if __debug__:
-                self.log.debug("Applying left boundary region computation")
         elif boundary_ID == grid.RIGHT:
             diss_u[-r:] = be.dot(self.Qr, u[-c:])
-            if __debug__:
-                self.log.debug("Applying right boundary region computation")
-        if __debug__:
-            self.log.debug("After boundary conditions: diss_u = %s" % repr(diss_u))
         factor = math.pow(0.5, 2 * self.p)
         return factor * diss_u
 
 
 class DissRestFull(Diss):
     """A class that represents dissipation operators for restricted full norms."""
 
@@ -87,15 +66,14 @@
         Parameters
         ----------
         p : int
             The power of the operator.
         """
         self.bdyRegion = self.Ql.shape
         self.p = p
-        self.log = logging.getLogger("DissRestFull")
 
     def __call__(self, u, dx, boundary_ID=None):
         """Applies the operator.
 
         We follow the notation of Diener Dorband Schnetter and Tiglio. We
         make the assumption that the differencing operator D_p is always of the
         form of some central finite difference stencil in the interior and some
@@ -167,24 +145,16 @@
         # It turns out that this can be done by using the 'valid' mode in
         # the be.convolve method. This will reduce the size of the output by r
         # elements on the end and beginning of the output array. The values that
         # should be in these positions are all zero due to the r zero'd rows in
         # the matrix A.
         diss_u_int = be.zeros_like(u)
         diss_u_int[r:-r] = be.convolve(u, self.A, mode="valid")
-        if __debug__:
-            self.log.debug("A.u = %s" % repr(diss_u_int))
         for i in range(size):
             diss_u_int[i] = self.B(i, dx, size) * diss_u_int[i]
-        if __debug__:
-            B_string = "[ "
-            for i in range(size - 1):
-                B_string += "%f, " % diss_u_int[i]
-            B_string += "%f ]" % diss_u_int[size - 1]
-            self.log.debug("B.A.u = " + B_string)
 
         # To multiply my Transpose[A], requires some care. The zero'd rows now
         # become columns and the stencil is reversed. I make here the assumption
         # that the stencil is always symmetric, up to sign! For stencils with
         # odd length (p is even) the sign does not change, but for stencils with
         # even length (p is odd) the sign does change. For the stencil
         # [-1,3,-3,1] the matrix A is
@@ -208,69 +178,43 @@
         # Lastly the differences in vector length diss_u[r:-r] and diss_u is
         # inculded to account for the vector lengthening of the 'full' mode
         # of the convolve method which adds r number of terms to the vector
         # at both ends.
         diss_u_int = be.convolve(
             diss_u_int[r:-r], math.pow(-1, self.p) * self.A[::-1], mode="full"
         )
-        if __debug__:
-            self.log.debug("Transpose[A].B.A.u = %s" % repr(diss_u_int))
 
         # Second do the boundary convolution
         # The check at the beginning of the method ensures that the
         # two array's diss_u_b[0:r] and diss_u_b[-r:] do not share any points
         # of diss_u_b
         diss_u_b = be.zeros_like(u)
-        if __debug__:
-            self.log.debug("After convolve: diss_u = %s" % repr(diss_u))
         if boundary_ID is None:
             diss_u_b[0:r] = be.dot(self.Ql, u[0:c])
             diss_u_b[-r:] = be.dot(self.Qr, u[-c:])
-            if __debug__:
-                self.log.debug("Q.u = %s" % repr(diss_u_b))
             for i in range(size):
                 diss_u_b[i] = self.B(i, dx, size) * diss_u_b[i]
-            if __debug__:
-                B_string = "[ "
-                for i in range(size - 1):
-                    B_string += "%f, " % diss_u_b[i]
-                B_string += "%f ]" % diss_u_b[size - 1]
-                self.log.debug("B.Q.u = " + B_string)
             diss_u_b[0:c] = be.dot(diss_u_b[0:r], self.Ql)
             diss_u_b[-c:] = be.dot(diss_u_b[-r:], self.Qr)
-            if __debug__:
-                self.log.debug("Transpose[Q].B.Q.u = %s" % repr(diss_u_b))
-            if __debug__:
-                self.log.debug("Applying both boundary region computation")
         elif boundary_ID == grid.LEFT:
             diss_u[0:r] = be.dot(self.Ql, u[0:c])
             for i in range(size):
                 diss_u_b[i] = self.B(i, dx, size) * diss_u_b[i]
             diss_u_b[0:c] = be.dot(diss_u_b[0:r], self.Ql)
-            if __debug__:
-                self.log.debug("Applying left boundary region computation")
         elif boundary_ID == grid.RIGHT:
             diss_u[-r:] = be.dot(self.Qr, u[-c:])
             for i in range(size):
                 diss_u_b[i] = self.B(i, dx, size) * diss_u_b[i]
             diss_u_b[-c:] = be.dot(diss_u_b[-r:], self.Qr)
-            if __debug__:
-                self.log.debug("Applying right boundary region computation")
-        if __debug__:
-            self.log.debug("After boundary conditions: diss_u = %s" % repr(diss_u))
 
         # Add the two parts together and multiply by the appropriate
         # numerical factor.
         diss_u = diss_u_int + diss_u_b
-        if __debug__:
-            self.log.debug("Transpose[M].B.M.u = %s" % repr(diss_u))
         factor = math.pow(0.5, 2 * self.p) * math.pow(dx, 2 * self.p - 2)
         diss_u = -factor * diss_u
-        if __debug__:
-            self.log.debug("D(u,dx) = %s" % repr(diss_u))
 
         # Multiply by the inverse of the norm
         super(DissRestFull, self)._consistancy_check(u, self.norm_inv.shape)
         r, c = self.norm_inv.shape
         diss_u[0:r] = be.dot(self.norm_inv, diss_u[0:c])
         diss_u[-r:] = be.dot(self.norm_inv[::-1, ::-1], diss_u[-c:])
 
@@ -429,19 +373,8 @@
         """
         cut_off = math.floor(size * self.bdy_percent)
         if i < cut_off:
             return dx + (i / cut_off) * (1 - dx)
         elif i > size - 1 - cut_off:
             return 1 + (cut_off + 1 - size + i) * (dx - 1) / cut_off
         else:
-            return 1
-
-
-################################################################################
-# Testing
-################################################################################
-
-# if __name__ == "__main__":
-# D = Diss43_DDST(0.2)
-# u = be.arange(20, dtype=float)
-# u = 10 - (u - 5)**2
-# D(u, 0.1)
+            return 1
```

### Comparing `coffeegrinder-0.2.6/src/coffee/diffop/sbp/dissipation_testing.nb` & `coffeegrinder-0.2.8/src/coffee/diffop/sbp/dissipation_testing.nb`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.2.6/src/coffee/diffop/sbp/sbp.py` & `coffeegrinder-0.2.8/src/coffee/diffop/sbp/sbp.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 #!/usr/bin/env python
 # encoding: utf-8
 """
 A module to manage summation by parts finite difference operators.
 """
 
-import os
 import math
-import numpy as np
 import logging
 from coffee.backend import backend as be
 
 ################################################################################
 # Base class for SBP operators
 ################################################################################
 BOUNDARY_TYPE_SAT = 0
@@ -89,41 +87,25 @@
             The step size.
         boundary_ID: int, Optional
             One of None, grid.LEFT or grid.RIGHT. Specifies if only the
             right or left (or both) derivatives should be applied at the
             boundary.
         """
         r, c = self.bdyRegion
-        if __debug__:
-            self.log.debug("u.shape[0] = %s" % repr(u.shape[0]))
-            self.log.debug("c = %s" % repr(c))
         if u.shape[0] + 1 <= 2 * c:
             self.log.error("Domain too small for application of operator")
             raise ValueError("Domain too small for application of operator")
-        if __debug__:
-            self.log.debug("Boundary region r = %s, c = %s" % (r, c))
-            self.log.debug("Array to operate on is = %s" % repr(u))
         du = be.convolve(u, self.A, mode="same")
-        if __debug__:
-            self.log.debug("After convolve: du = %s" % repr(du))
         if boundary_ID is None:
             du[0:r] = be.dot(self.Ql, u[0:c])
             du[-r:] = be.dot(self.Qr, u[-c:])
-            if __debug__:
-                self.log.debug("Applying both boundary region computation")
         elif boundary_ID == grid.LEFT:
             du[0:r] = be.dot(self.Ql, u[0:c])
-            if __debug__:
-                self.log.debug("Applying left boundary region computation")
         elif boundary_ID == grid.RIGHT:
             du[-r:] = be.dot(self.Qr, u[-c:])
-            if __debug__:
-                self.log.debug("Applying right boundary region computation")
-        if __debug__:
-            self.log.debug("After boundary conditions: du = %s" % repr(du))
         return du / (dx**self.order)
 
     def penalty_boundary(self, dx, vector_selection):
         """Returns the penalty for use with penalty boundaries.
 
         The vector self.pbound is, in the notation of CGA,
         given by P^(-1)H^(-1)e_i, i=0,1 where
```

### Comparing `coffeegrinder-0.2.6/src/coffee/free_data.py` & `coffeegrinder-0.2.8/src/coffee/free_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 corresponds to free data could be included directly into system.System since
 all calls to FreeData are mediated through system.System.
 """
 
 import abc
 from abc import ABCMeta
 
-
 class FreeData(object, metaclass=ABCMeta):
     """This is a simple abstract base class for the implementation of exact
     solutions.
 
     All the 'virtual' functions must be defined, modulo the comments given in
     the module docstring.
     """
```

### Comparing `coffeegrinder-0.2.6/src/coffee/grid/grid.py` & `coffeegrinder-0.2.8/src/coffee/grid/grid.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 
 Each grid object understands it's own discretisation as well as how
 """
 
 
 from builtins import range
 from builtins import object
-import math
-import numpy as np
 import abc
-import logging
 
-from coffee.mpi import mpiinterfaces
-from coffee.backend import backend as be
+try:
+    from coffee.mpi import mpiinterfaces
+except ModuleNotFoundError:
+    pass
 
+from coffee.backend import backend as be
 
 ################################################################################
 # Base Boundary data class
 ################################################################################
 class ABCBoundary(object, metaclass=abc.ABCMeta):
     """The abstract base class for boundary classes.
 
@@ -227,28 +227,24 @@
             Each tuple of slices represents the sub array of the computational
             domain that made up of external boundary points.
         """
 
         # This implicitly assumes that the number of dimensions handled by
         # the grid object is the same as than managed by the mpi_comm
         dims = self.mpi_comm.Get_dim()
-        if __debug__:
-            self.log.debug("Shape = " + repr(shape))
         neg_slices = [
             (i, -1, self.external_slice(shape, i, -1))
             for i in range(dims)
             if self.external_slice(shape, i, -1) != self._empty_slice(len(shape))
         ]
         pos_slices = [
             (i, 1, self.external_slice(shape, i, 1))
             for i in range(dims)
             if self.external_slice(shape, i, 1) != self._empty_slice(len(shape))
         ]
-        if __debug__:
-            self.log.debug("external slices are = " + repr(pos_slices + neg_slices))
         return pos_slices + neg_slices
 
 
 ################################################################################
 # Base Boundary data class
 ################################################################################
 class SingleCartesianGridBoundary(ABCBoundary):
@@ -299,15 +295,14 @@
             The mpi4py wrapper of MPI_COMM.
 
         """
         super(MPIBoundary, self).__init__(*args, **kwargs)
         self._ghost_points = ghost_points
         self._internal_points = internal_points
         self.mpi_comm = mpi_comm
-        self.log = logging.getLogger("MPIBoundary")
 
     def ghost_points(self, dimension, direction):
         "See ABCBoundary.ghost_points() for documentation." ""
         return self._ghost_points[dimension][self._direction_to_index(direction)]
 
     def source_and_dest(self, dimension, direction):
         """A wrapper for the MPI_Cart_Shift function via mpi4py.
@@ -521,15 +516,14 @@
             An instance of an mpi4py wrapped MPI_COMM object.
         boundary_data: ABCBoundary, Optional
             An implementation of ABCBoundary
         """
         self.mpi = mpi
         self.dim = len(shape)
         self.name = name
-        self.log = logging.getLogger(name)
         self.comparison = comparison
         self.shape = shape
         self.bounds = bounds
         self.boundary_data = boundary_data
 
     def __strs__(self):
         return self.name
@@ -581,16 +575,14 @@
         return self.mpi.barrier()
 
     def external_slices(self, data_shape):
         """Wraps ABCBoundary.external_slices.
 
         See ABCBoundary.external_slices() for documentation.
         """
-        if __debug__:
-            self.log.debug("In grid.external_slices")
         return self.boundary_data.external_slices(data_shape)
 
     def collect_data(self, data):
         """Wraps mpi.mpiinterfaces.collect_data().
 
         See mpi.mpiinterfaces.collect_data() for documentation."""
         if self.mpi is None:
```

### Comparing `coffeegrinder-0.2.6/src/coffee/ibvp.py` & `coffeegrinder-0.2.8/src/coffee/ibvp.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,18 +6,14 @@
 
 The name ibvp comes from the original design of this class as the
 iterative step in an initial boundary value problem solver. However, this class
 is general enough to handle numerical techniques that have, at their highest
 level, some iterative method.
 """
 
-
-import logging
-
-
 class IBVP:
     """Handles computation of the solution to initial boundary value problems.
 
     This class manages the interative process of simulations and interleaves
     interative steps with calls to a list of actions. Information about events
     during the simulation are writen to logging.getLogger("IBVP").
     """
@@ -56,15 +52,14 @@
                  Specifies the minimum time step.
         """
         self.theSolver = sol
         self.theSystem = eqn
         self.maxIteration = maxIteration
         self.theGrid = grid
         self.theActions = action
-        self.log = logging.getLogger("IBVP")
         self.minTimestep = minTimestep
 
     def run(self, tstart, tstop=float("inf"), thits=None):
         """Go for it! Starts the simulation.
 
         Parameters
         ----------
@@ -92,90 +87,72 @@
         tstop = thits.pop()
 
         # Set start time.
         t = tstart
 
         # Get initial data and configure timeslices for multiple processors.
         u = self.theSystem.initial_data(t, self.theGrid)
-        self.log.info("Running system %s" % str(self.theSystem))
-        self.log.info("Grid = %s" % str(self.theGrid))
-        self.log.info("Stepsizes = %s" % repr(u.domain.step_sizes))
-        if __debug__:
-            self.log.debug("self.actions is %s" % repr(self.theActions))
-            self.log.debug("Initial data is = %s" % repr(u))
 
         advance = self.theSolver.advance
         computation_valid = True
         while computation_valid and t < tstop:
-            if __debug__:
-                self.log.debug("Beginning new iteration")
-
             # Check against maxIteration
             if self.iteration > self.maxIteration:
-                self.log.warning("Maximum number of iterations exceeded")
                 break
 
             dt = self.theSystem.timestep(u)
 
             # Check dt for size
             if dt < self.minTimestep:
-                self.log.error(
-                    "Exiting computation: timestep too small dt = %.15f" % dt
-                )
                 break
 
             # Check if dt needs to change in order to hit the next thits value.
             timeleft = tstop - t
             if timeleft < dt:
                 dt = timeleft
                 if not thits:
-                    self.log.warning("Final time step: adjusting to dt = %.15f" % dt)
                     computation_valid = False
                 else:
-                    self.log.warning("Forcing evaluation at time %f" % tstop)
                     tstop = thits.pop()
 
-            if __debug__:
-                self.log.debug("Using timestep dt = %f" % dt)
-
             # Run the actions.
             self._run_actions(t, u)
 
-            if __debug__:
-                self.log.debug("About to advance for iteration = %i" % self.iteration)
             try:
                 t, u = advance(t, u, dt)
             except OverflowError as e:
                 # OverflowErrors arn't always appropirately handled. So we
                 # do it ourselves here.
                 print("Overflow error({0}): {1}".format(e.errno, e.strerror))
                 computation_valid = False
 
+            # Dirichlet boundary conditions
+            try:
+                u = self.theSystem.dirichlet_boundary(u)
+            except AttributeError:
+                pass
+
             # If we're using an mpi enable grid, this ensures that all
             # processes have gotten to the same point before continuing the
             # simulation.
             u.barrier()
 
             # On to the next iteration.
             self.iteration += 1
-            if __debug__:
-                self.log.debug("time slice after advance = %s" % repr(u))
 
         # end (while)
 
         # Run the actions once more before exiting.
         self._run_actions(t, u)
 
         # This statement might be unnecessary. In principle it ensures that all
         # processes are about to complete the current simulation before exit
         # occurs.
         u.barrier()
-        self.log.info(
-            "Finished computation at time %f for iteration %i" % (t, self.iteration)
-        )
+
         return u
 
     def _run_actions(self, t, u):
         """A utility method that ensures that actions are only run after all data is collected across MPI nodes and only if an action is due to run.
 
         Parameters
         ----------
@@ -187,29 +164,16 @@
             The current timeslice.
         """
 
         # Ideally u.collect_data() should only be executed if there
         # actions that will run. Because of single process access to
         # actions this causes an issue.
         # Some thought is required to fix this problem.
-        if __debug__:
-            self.log.debug("Running actions")
         tslice = u.collect_data()
         if tslice is not None:
-            if __debug__:
-                self.log.debug("tslice is not None. Computing if actions will run")
             actions_do_actions = [
                 action.will_run(self.iteration, tslice) for action in self.theActions
             ]
             if any(actions_do_actions):
-                if __debug__:
-                    self.log.debug("Some actions will run")
                 for i, action in enumerate(self.theActions):
                     if actions_do_actions[i]:
-                        if __debug__:
-                            self.log.debug(
-                                "Running action %s at iteration %i"
-                                % (str(action), self.iteration)
-                            )
-                        action(self.iteration, tslice)
-            if __debug__:
-                self.log.debug("All actions done")
+                        action(self.iteration, tslice)
```

### Comparing `coffeegrinder-0.2.6/src/coffee/io/simulation_data.py` & `coffeegrinder-0.2.8/src/coffee/io/simulation_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 from builtins import zip
 from builtins import map
 from builtins import str
 from builtins import range
 from builtins import object
 import functools
 import h5py
-import numpy as np
 from coffee.backend import backend as be
 
 # Gnuplot currently only works with Python 2!
 try:
     import Gnuplot
 except ImportError:
     pass
```

### Comparing `coffeegrinder-0.2.6/src/coffee/mpi/mpiinterfaces.py` & `coffeegrinder-0.2.8/src/coffee/mpi/mpiinterfaces.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,16 @@
 """
 Contains classes that abstract the MPI C API.
 
 Classes in this module model the MPI node network and manage the relationship
 of the complete domain to each 
 """
-from builtins import str
 from builtins import range
 from builtins import object
 import abc
-from mpi4py import MPI
-import logging
-import numpy as np
 from coffee.backend import backend as be
 
 
 ###############################################################################
 # Abstract Base Class for MPI Interfaces
 ###############################################################################
 class MPIInterface(object, metaclass=abc.ABCMeta):
@@ -67,15 +63,14 @@
         ==========
         domain: numpy.ndarray
             A numpy array representing the values of points in the global
             computational domain
         boundary_data: grid.ABCBoundary
         """
         super(EvenCart, self).__init__(*args, **kwds)
-        self.log = logging.getLogger("EvenCart")
         self.domain = domain
         self.domain_mapping = self._make_domain_mappings(domain, boundary_data)
 
     def _make_domain_mappings(self, domain, boundary_data):
         """A utility that constructs the tuples of slices that represent
         the sub-grids for each MPI node based on that nodes rank.
 
@@ -111,16 +106,14 @@
                             boundary_data.ghost_points(i, -1),
                             boundary_data.ghost_points(i, 1),
                         )
                         for i, coord in enumerate(coords)
                     ]
                 )
             ]
-        if __debug__:
-            self.log.debug("domain_mapping is %s" % r_map)
         return r_map
 
     def _neighbour_slices(self, shape, b_data):
         """A utility function that collects the source and destination
         ranks for neighbouring MPI nodes along with the slices needed
         to describe what data should be transferred.
 
@@ -147,16 +140,14 @@
             for d in range(dims)
         ]
         neg_neighbours = [
             b_data.source_and_dest(d, -1) + b_data.internal_slice(shape, d, -1)
             for d in range(dims)
         ]
         neighbours = pos_neighbours + neg_neighbours
-        if __debug__:
-            self.log.debug("neighbour_slices is %s" % neighbours)
         return neighbours
 
     def _array_slice(
         self, array_length, rank, num_ranks, ghost_points_start, ghost_points_end
     ):
         """The utility method that calculates the slices that describe the
         sub-grid managed by the MPI node with rank ``rank``.
@@ -181,39 +172,30 @@
 
         Returns
         =======
         slice:
             A slice which gives the subdomain for the particular dimension and
             the needed MPI node rank.
         """
-        if __debug__:
-            self.log.debug("Calculating start and end indices for subdomain")
-            self.log.debug("Array_length is %i" % array_length)
         # divide domain into appropriate parts
         q, r = divmod(array_length, num_ranks)
-        if __debug__:
-            self.log.debug("q = %i, r = %i" % (q, r))
         # use the rank to details which part is relevant for this process
         s = rank * q + min(rank, r)
         e = s + q
         # Adjust e to account for min(rank, r) term, which spreads the remainder
         # over the appropriate number of processes
         if rank < r:
-            if __debug__:
-                self.log.debug("rank < r so we add one to end point")
             e = e + 1
         # add in ghost_points if we can
         # this currently works for gp = 1 for an SAT boudnary method.
         # The code will need to be checked for consistency if this changes.
         if s - ghost_points_start > -1:
             s = s - ghost_points_start
         if e + ghost_points_end < array_length:
             e = e + ghost_points_end
-        if __debug__:
-            self.log.debug("Start index = %i, End index = %i" % (s, e))
         return slice(s, e, None)
 
     @property
     def subdomain(self):
         """Returns the slices which give the subdomain for the MPI node
         that this method is called on.
 
@@ -242,25 +224,16 @@
             describes which grid points the communicated data relates to.
             The second element is the data received from whichever MPI node
             manages the sub-grid which looks after the relevant grid points.
         """
         # if self.comm.size == 1:
         # return []
         nslices = self._neighbour_slices(data.shape, b_data)
-        if __debug__:
-            self.log.debug("about to perform communication")
-            self.log.debug("nslices = %s" % (repr(nslices)))
-            self.log.debug("data is %s" % repr(data))
         r_data = []
         for source, dest, send_slice, recv_slice in nslices:
-            if __debug__:
-                self.log.debug(
-                    "source=%d, dest=%d, send_slice=%s, recv_slice=%s"
-                    % (source, dest, repr(send_slice), repr(recv_slice))
-                )
             if dest < 0:
                 send_data = None
             else:
                 # I really did not want to copy this view. For large data
                 # sets this feels like an unnecessary delay.
                 # However mpi4py did not seem to work with views and using
                 # self.comm.sendrecv to send and recv arbitrary objects.
@@ -270,30 +243,17 @@
                 send_data = be.array(data[send_slice], copy=True, order="C")
             if source < 0:
                 recv_data = None
             else:
                 # when testing the above assertion I suggest changing this
                 # line to be.ones_like, rather than be.empty_like
                 recv_data = be.empty_like(data[recv_slice])
-            if __debug__:
-                self.log.debug("About to sendrecv")
-                self.log.debug("data to be sent is %s" % repr(send_data))
-                self.log.debug("source is %s" % source)
-                self.log.debug("dest is %s" % dest)
-                self.log.debug("recv_data is %s" % repr(recv_data))
             self.comm.Sendrecv(send_data, dest=dest, recvbuf=recv_data, source=source)
-            if __debug__:
-                self.log.debug("Received data = %s" % repr(recv_data))
-                self.log.debug("data[0] is %s" % repr(data[0]))
-                self.log.debug("Sendrecv completed")
             if source >= 0:
                 r_data += [(recv_slice, recv_data)]
-        if __debug__:
-            self.log.debug("r_data = %s" % repr(r_data))
-            self.log.debug("communication complete")
         return r_data
 
     def collect_data(self, data):
         """A method that collects all computed function values over all
         sub-grids managed by all MPI nodes and returns the amalgamated data
         if the rank of this process is 0.
 
@@ -316,58 +276,24 @@
         # the domains. This does not cause a problem. It just means
         # that more data than necessary is passed.
 
         # If there are no partitions of the domain we don't need to collect
         if self.comm is None:
             return data
         # Gather the data
-        if __debug__:
-            self.log.debug("Data is %s" % repr(data))
         fields = self.comm.gather(data, root=0)
-        if __debug__:
-            self.log.debug("Data has been gathered.")
         # If this process is root then collate the data and return
         if self.comm.rank == 0:
-            if __debug__:
-                self.log.debug(
-                    "The collected fields have shapes %s"
-                    % repr([f.shape for f in fields])
-                )
             rdata_edims_shape = (data.shape[0],) + data.shape[len(self.domain) + 1 :]
             rdata_edims_slice = tuple(
                 [slice(None, None, None) for i in rdata_edims_shape]
             )
-            if __debug__:
-                self.log.debug("data.shape is %s" % str(data.shape))
-                self.log.debug("rdata_shape_edims is %s" % str(rdata_edims_slice))
-                self.log.debug("rdata_edims_shape is %s" % repr(rdata_edims_shape))
-                self.log.debug("self.domain is %s" % str(self.domain))
             rdata = be.zeros(
                 (rdata_edims_shape[0],) + self.domain + rdata_edims_shape[1:],
                 dtype=data.dtype,
             )
-            if __debug__:
-                self.log.debug("rdata.shape = %s" % (repr(rdata.shape)))
             for rank, field in enumerate(fields):
                 dslice = self.domain_mapping[rank]
-                if __debug__:
-                    self.log.debug("dslice is %s" % repr(dslice))
-                    self.log.debug("rdata_edims_slice is %s" % repr(rdata_edims_slice))
-                    self.log.debug("rdata.shape is %s" % repr(rdata.shape))
-                    self.log.debug("field.shape is %s" % repr(field.shape))
-                    self.log.debug(
-                        "rdata[(rdata_edims_slice[0],) + dslice].shape is + \
-                        rdata_edims_slice[1:] = %s"
-                        % (
-                            repr(
-                                rdata[
-                                    (rdata_edims_slice[0],)
-                                    + dslice
-                                    + rdata_edims_slice[1:]
-                                ].shape
-                            )
-                        )
-                    )
                 rdata[(rdata_edims_slice[0],) + dslice + rdata_edims_slice[1:]] = field
             return rdata
         else:
             return None
```

### Comparing `coffeegrinder-0.2.6/src/coffee/solvers/solvers.py` & `coffeegrinder-0.2.8/src/coffee/solvers/solvers.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,16 +6,14 @@
 
 This default implementations all assume that tslice.TimeSlice objects can be
 operated on by numerically (e.g. addition, multiplication, subtraction).
 """
 
 
 from builtins import object
-import math
-import logging
 import abc
 
 from coffee.tslices import tslices
 
 
 ################################################################################
 # Solver Abstract Base Class
@@ -37,15 +35,14 @@
         ----------
 
         system : system
             The system being used.
         """
         self.system = system
         super(ABCSolver, self).__init__(**kwds)
-        self.log = logging.getLogger(self.name)
 
     @abc.abstractproperty
     def name(self):
         """This should return a name associated to the subclass.
 
         The name will need to be defined in the subclasses constructor. The
         name is used to identify the instantiated class in the logger.
@@ -210,46 +207,33 @@
 
     def advance(self, t0, u0, dt):
         """See the ABCSolver.advance method for documentation.
 
         Very simple minded implementation of the standard 4th order Runge-Kutta
         method to solve an ODE of the form fdot = rhs(t,f)
         """
-        if __debug__:
-            self.log.debug("In advance")
-            self.log.debug("time = %s" % repr(t0))
-            self.log.debug("data = %s" % (repr(u0)))
-            self.log.debug("dt = %s" % repr(dt))
         eqn = self.system
         u = u0
         t = t0
         k = eqn.evaluate(t, u)
-        if __debug__:
-            self.log.debug("First evaluate, k = %s" % repr(k))
         u1 = u0 + (dt / 6.0) * k
 
         u = u0 + dt / 2.0 * k
         t = t0 + dt / 2.0
         k = eqn.evaluate(t, u)
-        if __debug__:
-            self.log.debug("Second evaluate, k = %s" % repr(k))
         u1 += dt / 3.0 * k
 
         u = u0 + dt / 2.0 * k
         t = t0 + dt / 2.0
         k = eqn.evaluate(t, u)
-        if __debug__:
-            self.log.debug("Third evaluate, k = %s" % repr(k))
         u1 += dt / 3.0 * k
 
         u = u0 + dt * k
         t = t0 + dt
         k = eqn.evaluate(t, u)
-        if __debug__:
-            self.log.debug("Fourth evaluate, k = %s" % repr(k))
         u1 += dt / 6.0 * k
         u1.time = t
 
         return (t, u1)
 
 
 class RungeKutta4Dirichlet(ABCSolver):
```

### Comparing `coffeegrinder-0.2.6/src/coffee/system.py` & `coffeegrinder-0.2.8/src/coffee/system.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 While you don't need to actually implement all the methods below, it really is
 recommended. You may get errors about the methods missing as a consequence.
 
 system.System has abc.ABCMeta as a meta class. This serves as a warning to
 really think about what you are doing if you don't implement all methods below.
 """
 
-import abc
 from abc import ABCMeta
 
 
 #############################################################################
 class System(object, metaclass=ABCMeta):
     """The System class that specifies the interface for all other system
     classes.
```

### Comparing `coffeegrinder-0.2.6/src/coffee/tslices/tslices.py` & `coffeegrinder-0.2.8/src/coffee/tslices/tslices.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,19 +28,16 @@
 TimeSlice objects should contain all information needed to interperet the
 values of the functions being numerically evolved. In particular, aim to ensure
 that you can restart a simulation if given a timeslice, system and solver.
 """
 
 from builtins import object
 import abc
-import logging
-import numpy as np
 from coffee.backend import backend as be
 
-
 ###############################################################################
 # TimeSlice Abstract Base Class
 ##############################################################################
 class ABCTimeSlice(object, metaclass=abc.ABCMeta):
     """The abstract base class for TimeSlice objects.
 
     The interface below is assumed by all other classes that interact with
@@ -74,15 +71,14 @@
         self.data = data
         self.domain = domain
         self.time = time
         if name is None:
             self.name = "ABCTimeSlice"
         else:
             self.name = name
-        self.log = logging.getLogger(self.name)
         super(ABCTimeSlice, self).__init__(*args, **kwds)
 
     def __repr__(self):
         """Returns a naive string representation of the slice.
 
         Returns
         -------
@@ -106,16 +102,14 @@
 
         Returns
         -------
         list, slices
             The result of a call to self.domain.external_slices(self.data.shape)
 
         """
-        if __debug__:
-            self.log.debug("calling self.domain.external_slices")
         return self.domain.external_slices(self.data.shape)
 
     def communicate(self, ghost_point_processor=None, data=None):
         """Returns a list of tuples that describe the boundaries of
         grids for internal boundaries.
 
         This is currently used when the full domain is divided into
@@ -162,16 +156,14 @@
             A single timeslice which represents the complete data and
             domain for that point of time.
 
         """
         data_all = self.domain.collect_data(self.data)
         domain_all = self.domain.full_grid
         r_tslice = self.__class__(data_all, domain_all, self.time)
-        if __debug__:
-            self.log.debug("r_tslice is %s" % (repr(r_tslice)))
         return r_tslice
 
     def __add__(self, other):
         # It is very important that the rv is other + self.data not
         # self.data + other.
         # The reason (seems) is because as self.data can be an
         # nd.array the sum self.data + other
```

### Comparing `coffeegrinder-0.2.6/src/coffeegrinder.egg-info/PKG-INFO` & `coffeegrinder-0.2.8/src/coffeegrinder.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 Metadata-Version: 2.1
 Name: coffeegrinder
-Version: 0.2.6
+Version: 0.2.8
 Summary: COFFEE is an MPI-Parallelised Python package for the numerical evolution of time-dependent differential equations.
 Home-page: https://github.com/coffee-gr/coffee
 Author: Chris Stevens
 Author-email: chris.stevens@canterbury.ac.nz
 License: MIT
 Project-URL: Documentation, https://pyscaffold.org/
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Description-Content-Type: text/x-rst; charset=UTF-8
+Provides-Extra: MPI
+Provides-Extra: JAX
+Provides-Extra: MPI-JAX
 Provides-Extra: testing
 License-File: LICENSE.txt
 
 .. These are examples of badges you might want to add to your README:
    please update the URLs accordingly
 
     .. image:: https://api.cirrus-ci.com/github/<USER>/coffee.svg?branch=main
@@ -48,35 +51,30 @@
 
 
 ======
 coffee
 ======
 
 
-    COFFEE is an MPI-Parallelised Python package for the numerical evolution of time-dependent differential equations.
+COFFEE is an MPI-Parallelised Python package for the numerical evolution of time-dependent differential equations.
 
 
 Installation
 ------------
 
-To use this software, you will need the following dependencies:
+There are four versions of COFFEE, which can include MPI and/or JAX capabilities. These can be installed via
 
-- 
-- HDF library
-
-Please make sure these dependencies are installed before using this software.
+    pip install coffeegrinder
+    pip install coffeegrinder[MPI]
+    pip install coffeegrinder[JAX]
+    pip install coffeegrinder[MPI-JAX]
 
 .. rubric:: Getting started
 
-One needs to point the ``PYTHONPATH`` environment variable to the packages directory. Then the system code can be run with::
-
-    python3.10 -O TwoDAdvection_setup.py
-
-Note that adding a ``-d`` flag to this allows you to see a visualization during the computation. You should see a wave propagating from right to left with varying amplitude.
-
+There is a systems directory that includes commented test cases for the 1D advection equation with a mixture of finite-differencing operators and boundary imposition methods.
 
 .. _pyscaffold-notes:
 
 Note
 ====
 
 This project has been set up using PyScaffold 4.4. For details and usage
```

### Comparing `coffeegrinder-0.2.6/systems/OneDAdvection/OneDAdvection.py` & `coffeegrinder-0.2.8/systems/OneDAdvection/OneDAdvection.py`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.2.6/systems/OneDAdvection/OneDAdvection_plotter.py` & `coffeegrinder-0.2.8/systems/OneDAdvection/OneDAdvection_plotter.py`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.2.6/systems/OneDAdvection/OneDAdvection_setup.py` & `coffeegrinder-0.2.8/systems/OneDAdvection/OneDAdvection_setup.py`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.2.6/tests/test_actions.py` & `coffeegrinder-0.2.8/tests/test_actions.py`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.2.6/tests/test_backend.py` & `coffeegrinder-0.2.8/tests/test_backend.py`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.2.6/tox.ini` & `coffeegrinder-0.2.8/tox.ini`

 * *Files identical despite different names*

