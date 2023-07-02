# Comparing `tmp/gfort2py-2.0.0.tar.gz` & `tmp/gfort2py-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gfort2py-2.0.0.tar", last modified: Sun Jun 25 11:02:05 2023, max compression
+gzip compressed data, was "gfort2py-2.1.0.tar", last modified: Sun Jul  2 17:50:38 2023, max compression
```

## Comparing `gfort2py-2.0.0.tar` & `gfort2py-2.1.0.tar`

### file list

```diff
@@ -1,88 +1,90 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 11:02:05.370244 gfort2py-2.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 11:02:05.358244 gfort2py-2.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 11:02:05.362244 gfort2py-2.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-06-25 11:01:49.000000 gfort2py-2.0.0/.github/workflows/ci-mac.yml
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-25 11:01:49.000000 gfort2py-2.0.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-06-25 11:01:49.000000 gfort2py-2.0.0/.github/workflows/ci_old.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-06-25 11:01:49.000000 gfort2py-2.0.0/.github/workflows/coveralls.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-25 11:01:49.000000 gfort2py-2.0.0/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-06-25 11:01:49.000000 gfort2py-2.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-06-25 11:01:49.000000 gfort2py-2.0.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-06-25 11:01:49.000000 gfort2py-2.0.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     5229 2023-06-25 11:01:49.000000 gfort2py-2.0.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)    15219 2023-06-25 11:01:49.000000 gfort2py-2.0.0/COPYING.txt
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-25 11:01:49.000000 gfort2py-2.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10797 2023-06-25 11:02:05.370244 gfort2py-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9982 2023-06-25 11:01:49.000000 gfort2py-2.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-25 11:01:49.000000 gfort2py-2.0.0/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 11:02:05.362244 gfort2py-2.0.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-25 11:01:49.000000 gfort2py-2.0.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-06-25 11:01:49.000000 gfort2py-2.0.0/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 11:02:05.362244 gfort2py-2.0.0/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-06-25 11:01:49.000000 gfort2py-2.0.0/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     6997 2023-06-25 11:01:49.000000 gfort2py-2.0.0/docs/source/fortranabi.rst
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-06-25 11:01:49.000000 gfort2py-2.0.0/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5155 2023-06-25 11:01:49.000000 gfort2py-2.0.0/docs/source/mod_files.rst
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-25 11:01:49.000000 gfort2py-2.0.0/docs/source/testsuite.rst
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-25 11:01:49.000000 gfort2py-2.0.0/docs/source/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 11:02:05.366244 gfort2py-2.0.0/gfort2py/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-25 11:01:49.000000 gfort2py-2.0.0/gfort2py/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7608 2023-06-25 11:01:49.000000 gfort2py-2.0.0/gfort2py/fArrays.py
--rw-r--r--   0 runner    (1001) docker     (123)     6922 2023-06-25 11:01:49.000000 gfort2py-2.0.0/gfort2py/fDT.py
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-06-25 11:01:49.000000 gfort2py-2.0.0/gfort2py/fParameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     6012 2023-06-25 11:01:49.000000 gfort2py-2.0.0/gfort2py/fProc.py
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-06-25 11:01:49.000000 gfort2py-2.0.0/gfort2py/fProcPtr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-06-25 11:01:49.000000 gfort2py-2.0.0/gfort2py/fScalars.py
--rw-r--r--   0 runner    (1001) docker     (123)     9791 2023-06-25 11:01:49.000000 gfort2py-2.0.0/gfort2py/fStrings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-25 11:01:49.000000 gfort2py-2.0.0/gfort2py/fUnary.py
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-06-25 11:01:49.000000 gfort2py-2.0.0/gfort2py/fVar.py
--rw-r--r--   0 runner    (1001) docker     (123)     3510 2023-06-25 11:01:49.000000 gfort2py-2.0.0/gfort2py/fVar_t.py
--rw-r--r--   0 runner    (1001) docker     (123)     3433 2023-06-25 11:01:49.000000 gfort2py-2.0.0/gfort2py/gfort2py.py
--rw-r--r--   0 runner    (1001) docker     (123)    21658 2023-06-25 11:01:49.000000 gfort2py-2.0.0/gfort2py/module_parse.py
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-06-25 11:01:49.000000 gfort2py-2.0.0/gfort2py/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-06-25 11:01:49.000000 gfort2py-2.0.0/gfort2py/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 11:02:05.366244 gfort2py-2.0.0/gfort2py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10797 2023-06-25 11:02:05.000000 gfort2py-2.0.0/gfort2py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-06-25 11:02:05.000000 gfort2py-2.0.0/gfort2py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 11:02:05.000000 gfort2py-2.0.0/gfort2py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 11:02:05.000000 gfort2py-2.0.0/gfort2py.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-25 11:02:05.000000 gfort2py-2.0.0/gfort2py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-25 11:02:05.000000 gfort2py-2.0.0/gfort2py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-25 11:01:49.000000 gfort2py-2.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-25 11:01:49.000000 gfort2py-2.0.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-25 11:01:49.000000 gfort2py-2.0.0/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-06-25 11:02:05.370244 gfort2py-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-25 11:01:49.000000 gfort2py-2.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 11:02:05.370244 gfort2py-2.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-06-25 11:01:49.000000 gfort2py-2.0.0/tests/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-06-25 11:01:49.000000 gfort2py-2.0.0/tests/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 11:01:49.000000 gfort2py-2.0.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4965 2023-06-25 11:01:49.000000 gfort2py-2.0.0/tests/basic.f90
--rw-r--r--   0 runner    (1001) docker     (123)     5936 2023-06-25 11:01:49.000000 gfort2py-2.0.0/tests/basic_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-06-25 11:01:49.000000 gfort2py-2.0.0/tests/common.f90
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-06-25 11:01:49.000000 gfort2py-2.0.0/tests/complex.f90
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-06-25 11:01:49.000000 gfort2py-2.0.0/tests/complex_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-06-25 11:01:49.000000 gfort2py-2.0.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     9440 2023-06-25 11:01:49.000000 gfort2py-2.0.0/tests/dt.f90
--rw-r--r--   0 runner    (1001) docker     (123)     6480 2023-06-25 11:01:49.000000 gfort2py-2.0.0/tests/dt_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10391 2023-06-25 11:01:49.000000 gfort2py-2.0.0/tests/dummy_arrays.f90
--rw-r--r--   0 runner    (1001) docker     (123)    13265 2023-06-25 11:01:49.000000 gfort2py-2.0.0/tests/dummy_arrays_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-06-25 11:01:49.000000 gfort2py-2.0.0/tests/elemental.f90
--rw-r--r--   0 runner    (1001) docker     (123)     4974 2023-06-25 11:01:49.000000 gfort2py-2.0.0/tests/explicit_arrays.f90
--rw-r--r--   0 runner    (1001) docker     (123)     9165 2023-06-25 11:01:49.000000 gfort2py-2.0.0/tests/explicit_arrays_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-06-25 11:01:49.000000 gfort2py-2.0.0/tests/interface.f90
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-06-25 11:01:49.000000 gfort2py-2.0.0/tests/namelist.f90
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-06-25 11:01:49.000000 gfort2py-2.0.0/tests/oo.f90
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-06-25 11:01:49.000000 gfort2py-2.0.0/tests/oo_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-06-25 11:01:49.000000 gfort2py-2.0.0/tests/pdt.f90
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-06-25 11:01:49.000000 gfort2py-2.0.0/tests/pdt_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-06-25 11:01:49.000000 gfort2py-2.0.0/tests/pointers.f90
--rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-06-25 11:01:49.000000 gfort2py-2.0.0/tests/pointers_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-06-25 11:01:49.000000 gfort2py-2.0.0/tests/proc_ptrs.f90
--rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-06-25 11:01:49.000000 gfort2py-2.0.0/tests/proc_ptrs_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6996 2023-06-25 11:01:49.000000 gfort2py-2.0.0/tests/strings.f90
--rw-r--r--   0 runner    (1001) docker     (123)     7764 2023-06-25 11:01:49.000000 gfort2py-2.0.0/tests/strings_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-06-25 11:01:49.000000 gfort2py-2.0.0/tests/submodule.f90
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-25 11:01:49.000000 gfort2py-2.0.0/tests/template._f90
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-25 11:01:49.000000 gfort2py-2.0.0/tests/test_template.py
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-06-25 11:01:49.000000 gfort2py-2.0.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 17:50:38.263303 gfort2py-2.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 17:50:38.251303 gfort2py-2.1.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-07-02 17:50:22.000000 gfort2py-2.1.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 17:50:38.251303 gfort2py-2.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-07-02 17:50:22.000000 gfort2py-2.1.0/.github/workflows/ci-mac.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-07-02 17:50:22.000000 gfort2py-2.1.0/.github/workflows/ci-old.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-07-02 17:50:22.000000 gfort2py-2.1.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-02 17:50:22.000000 gfort2py-2.1.0/.github/workflows/coveralls.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-02 17:50:22.000000 gfort2py-2.1.0/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-07-02 17:50:22.000000 gfort2py-2.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-07-02 17:50:22.000000 gfort2py-2.1.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-07-02 17:50:22.000000 gfort2py-2.1.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-02 17:50:22.000000 gfort2py-2.1.0/.zenodo.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5229 2023-07-02 17:50:22.000000 gfort2py-2.1.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)    15219 2023-07-02 17:50:22.000000 gfort2py-2.1.0/COPYING.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-02 17:50:22.000000 gfort2py-2.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11005 2023-07-02 17:50:38.263303 gfort2py-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10190 2023-07-02 17:50:22.000000 gfort2py-2.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-02 17:50:22.000000 gfort2py-2.1.0/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 17:50:38.251303 gfort2py-2.1.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-07-02 17:50:22.000000 gfort2py-2.1.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-07-02 17:50:22.000000 gfort2py-2.1.0/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 17:50:38.251303 gfort2py-2.1.0/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-07-02 17:50:22.000000 gfort2py-2.1.0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6997 2023-07-02 17:50:22.000000 gfort2py-2.1.0/docs/source/fortranabi.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-02 17:50:22.000000 gfort2py-2.1.0/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5155 2023-07-02 17:50:22.000000 gfort2py-2.1.0/docs/source/mod_files.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-02 17:50:22.000000 gfort2py-2.1.0/docs/source/testsuite.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-02 17:50:22.000000 gfort2py-2.1.0/docs/source/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 17:50:38.255303 gfort2py-2.1.0/gfort2py/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-02 17:50:22.000000 gfort2py-2.1.0/gfort2py/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7608 2023-07-02 17:50:22.000000 gfort2py-2.1.0/gfort2py/fArrays.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6922 2023-07-02 17:50:22.000000 gfort2py-2.1.0/gfort2py/fDT.py
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-07-02 17:50:22.000000 gfort2py-2.1.0/gfort2py/fParameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6012 2023-07-02 17:50:22.000000 gfort2py-2.1.0/gfort2py/fProc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-07-02 17:50:22.000000 gfort2py-2.1.0/gfort2py/fProcPtr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-07-02 17:50:22.000000 gfort2py-2.1.0/gfort2py/fScalars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9791 2023-07-02 17:50:22.000000 gfort2py-2.1.0/gfort2py/fStrings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-07-02 17:50:22.000000 gfort2py-2.1.0/gfort2py/fUnary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-07-02 17:50:22.000000 gfort2py-2.1.0/gfort2py/fVar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3510 2023-07-02 17:50:22.000000 gfort2py-2.1.0/gfort2py/fVar_t.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-07-02 17:50:22.000000 gfort2py-2.1.0/gfort2py/gfort2py.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22204 2023-07-02 17:50:22.000000 gfort2py-2.1.0/gfort2py/module_parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-07-02 17:50:22.000000 gfort2py-2.1.0/gfort2py/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-07-02 17:50:22.000000 gfort2py-2.1.0/gfort2py/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 17:50:38.259303 gfort2py-2.1.0/gfort2py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11005 2023-07-02 17:50:38.000000 gfort2py-2.1.0/gfort2py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-07-02 17:50:38.000000 gfort2py-2.1.0/gfort2py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 17:50:38.000000 gfort2py-2.1.0/gfort2py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 17:50:38.000000 gfort2py-2.1.0/gfort2py.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-02 17:50:38.000000 gfort2py-2.1.0/gfort2py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-02 17:50:38.000000 gfort2py-2.1.0/gfort2py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-02 17:50:22.000000 gfort2py-2.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-02 17:50:22.000000 gfort2py-2.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-02 17:50:22.000000 gfort2py-2.1.0/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-02 17:50:38.263303 gfort2py-2.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 17:50:22.000000 gfort2py-2.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 17:50:38.263303 gfort2py-2.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-07-02 17:50:22.000000 gfort2py-2.1.0/tests/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-07-02 17:50:22.000000 gfort2py-2.1.0/tests/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 17:50:22.000000 gfort2py-2.1.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5067 2023-07-02 17:50:22.000000 gfort2py-2.1.0/tests/basic.f90
+-rw-r--r--   0 runner    (1001) docker     (123)     6054 2023-07-02 17:50:22.000000 gfort2py-2.1.0/tests/basic_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-07-02 17:50:22.000000 gfort2py-2.1.0/tests/common.f90
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-07-02 17:50:22.000000 gfort2py-2.1.0/tests/complex.f90
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-07-02 17:50:22.000000 gfort2py-2.1.0/tests/complex_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-02 17:50:22.000000 gfort2py-2.1.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9440 2023-07-02 17:50:22.000000 gfort2py-2.1.0/tests/dt.f90
+-rw-r--r--   0 runner    (1001) docker     (123)     6480 2023-07-02 17:50:22.000000 gfort2py-2.1.0/tests/dt_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10391 2023-07-02 17:50:22.000000 gfort2py-2.1.0/tests/dummy_arrays.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    13265 2023-07-02 17:50:22.000000 gfort2py-2.1.0/tests/dummy_arrays_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-02 17:50:22.000000 gfort2py-2.1.0/tests/elemental.f90
+-rw-r--r--   0 runner    (1001) docker     (123)     5413 2023-07-02 17:50:22.000000 gfort2py-2.1.0/tests/explicit_arrays.f90
+-rw-r--r--   0 runner    (1001) docker     (123)     9643 2023-07-02 17:50:22.000000 gfort2py-2.1.0/tests/explicit_arrays_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-07-02 17:50:22.000000 gfort2py-2.1.0/tests/interface.f90
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-07-02 17:50:22.000000 gfort2py-2.1.0/tests/namelist.f90
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-07-02 17:50:22.000000 gfort2py-2.1.0/tests/oo.f90
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-07-02 17:50:22.000000 gfort2py-2.1.0/tests/oo_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-02 17:50:22.000000 gfort2py-2.1.0/tests/pdt.f90
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-02 17:50:22.000000 gfort2py-2.1.0/tests/pdt_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-07-02 17:50:22.000000 gfort2py-2.1.0/tests/pointers.f90
+-rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-07-02 17:50:22.000000 gfort2py-2.1.0/tests/pointers_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-07-02 17:50:22.000000 gfort2py-2.1.0/tests/proc_ptrs.f90
+-rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-07-02 17:50:22.000000 gfort2py-2.1.0/tests/proc_ptrs_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7297 2023-07-02 17:50:22.000000 gfort2py-2.1.0/tests/strings.f90
+-rw-r--r--   0 runner    (1001) docker     (123)     8006 2023-07-02 17:50:22.000000 gfort2py-2.1.0/tests/strings_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-07-02 17:50:22.000000 gfort2py-2.1.0/tests/submodule.f90
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-02 17:50:22.000000 gfort2py-2.1.0/tests/template._f90
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-02 17:50:22.000000 gfort2py-2.1.0/tests/test_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-07-02 17:50:22.000000 gfort2py-2.1.0/tox.ini
```

### Comparing `gfort2py-2.0.0/.github/workflows/ci-mac.yml` & `gfort2py-2.1.0/.github/workflows/ci-mac.yml`

 * *Files identical despite different names*

### Comparing `gfort2py-2.0.0/.github/workflows/ci.yml` & `gfort2py-2.1.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `gfort2py-2.0.0/.github/workflows/ci_old.yml` & `gfort2py-2.1.0/.github/workflows/ci-old.yml`

 * *Files 12% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     env:
       FC: ${{ matrix.fortran-compiler }}
       CC: gcc
 
     steps:
     - uses: actions/checkout@v3
     - name: Set up Python ${{ matrix.python-version }}
-      uses: actions/setup-python@v3
+      uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python-version }}
         cache: 'pip'
 
     - name: Setup compiler ${{ matrix.fortran-compiler }}
       run: |
         sudo apt-get update
```

### Comparing `gfort2py-2.0.0/.github/workflows/coveralls.yml` & `gfort2py-2.1.0/.github/workflows/coveralls.yml`

 * *Files identical despite different names*

### Comparing `gfort2py-2.0.0/.github/workflows/pypi.yml` & `gfort2py-2.1.0/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `gfort2py-2.0.0/.gitignore` & `gfort2py-2.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `gfort2py-2.0.0/CODE_OF_CONDUCT.md` & `gfort2py-2.1.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `gfort2py-2.0.0/COPYING.txt` & `gfort2py-2.1.0/COPYING.txt`

 * *Files identical despite different names*

### Comparing `gfort2py-2.0.0/PKG-INFO` & `gfort2py-2.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gfort2py
-Version: 2.0.0
+Version: 2.1.0
 Summary: "Python bindings for Fortran"
 Home-page: https://github.com/rjfarmer/gfort2py
 Author: Robert Farmer
 Author-email: robert.j.farmer37@gmail.com
 License: GPLv2+
 Platform: unix
 Platform: linux
@@ -23,22 +23,20 @@
 Provides-Extra: dev
 License-File: COPYING.txt
 
 [![Continuous Integration](https://github.com/rjfarmer/gfort2py/actions/workflows/ci.yml/badge.svg)](https://github.com/rjfarmer/gfort2py/actions/workflows/ci.yml)
 [![Coverage Status](https://coveralls.io/repos/github/rjfarmer/gfort2py/badge.svg?branch=main)](https://coveralls.io/github/rjfarmer/gfort2py?branch=main)
 [![PyPI version](https://badge.fury.io/py/gfort2py.svg)](https://badge.fury.io/py/gfort2py)
 [![DOI](https://zenodo.org/badge/72889348.svg)](https://zenodo.org/badge/latestdoi/72889348)
-
+[![Python versions](https://img.shields.io/pypi/pyversions/gfort2py.svg)](https://img.shields.io/pypi/pyversions/gfort2py.svg)
 
 
 # gfort2py
 Library to allow calling Fortran code from Python. Requires gfortran>=8.0, Works with python >= 3.7
 
-The current stable version is 1.1.7
-
 ## Build
 ````bash
 pip3 install -r requirements.txt
 python3 setup.py install --user
 ````
 
 or install via pip
@@ -73,14 +71,20 @@
 
 On MacOS: 
 ````bash
 gfortran -dynamiclib -c file.f90
 gfortran -dynamiclib -o libfile file.f90
 ````
 
+On Windows:
+````bash
+gfortran -shared -c file.f90
+gfortran -shared -o libfile.dll file.f90
+````
+
 If your code comes as program that does everything, then just turn the program into a function call inside a module,
 then create a new file with your program that uses the module and calls the function you just made.
 
 If the shared library needs other
 shared libraries you will need to set LD_LIBRARY_PATH environment variable, and it is also recommended is to run chrpath on the 
 shared libraries so you can access them from anywhere.
 
@@ -243,15 +247,15 @@
 - [x] Allocatable arrays of strings
 - [x] Pointer arguments 
 - [x] Optional arguments
 - [x] Value arguments
 - [x] Keyword arguments
 - [ ] Generic/Elemental functions
 - [ ] Functions as an argument
-- [ ] Unary operations (arguments that involve an expression to evaluate like dimension(n+1))
+- [x] Unary operations (arguments that involve an expression to evaluate like dimension(n+1) or dimension((2*n)+1))
 
 ### Accessing common block elements
 
 There's no direct way to access the common block elements, but if you declare the common block as a module variable you may access the elements by their name:
 
 
 ````fortran
```

### Comparing `gfort2py-2.0.0/README.md` & `gfort2py-2.1.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 [![Continuous Integration](https://github.com/rjfarmer/gfort2py/actions/workflows/ci.yml/badge.svg)](https://github.com/rjfarmer/gfort2py/actions/workflows/ci.yml)
 [![Coverage Status](https://coveralls.io/repos/github/rjfarmer/gfort2py/badge.svg?branch=main)](https://coveralls.io/github/rjfarmer/gfort2py?branch=main)
 [![PyPI version](https://badge.fury.io/py/gfort2py.svg)](https://badge.fury.io/py/gfort2py)
 [![DOI](https://zenodo.org/badge/72889348.svg)](https://zenodo.org/badge/latestdoi/72889348)
-
+[![Python versions](https://img.shields.io/pypi/pyversions/gfort2py.svg)](https://img.shields.io/pypi/pyversions/gfort2py.svg)
 
 
 # gfort2py
 Library to allow calling Fortran code from Python. Requires gfortran>=8.0, Works with python >= 3.7
 
-The current stable version is 1.1.7
-
 ## Build
 ````bash
 pip3 install -r requirements.txt
 python3 setup.py install --user
 ````
 
 or install via pip
@@ -48,14 +46,20 @@
 
 On MacOS: 
 ````bash
 gfortran -dynamiclib -c file.f90
 gfortran -dynamiclib -o libfile file.f90
 ````
 
+On Windows:
+````bash
+gfortran -shared -c file.f90
+gfortran -shared -o libfile.dll file.f90
+````
+
 If your code comes as program that does everything, then just turn the program into a function call inside a module,
 then create a new file with your program that uses the module and calls the function you just made.
 
 If the shared library needs other
 shared libraries you will need to set LD_LIBRARY_PATH environment variable, and it is also recommended is to run chrpath on the 
 shared libraries so you can access them from anywhere.
 
@@ -218,15 +222,15 @@
 - [x] Allocatable arrays of strings
 - [x] Pointer arguments 
 - [x] Optional arguments
 - [x] Value arguments
 - [x] Keyword arguments
 - [ ] Generic/Elemental functions
 - [ ] Functions as an argument
-- [ ] Unary operations (arguments that involve an expression to evaluate like dimension(n+1))
+- [x] Unary operations (arguments that involve an expression to evaluate like dimension(n+1) or dimension((2*n)+1))
 
 ### Accessing common block elements
 
 There's no direct way to access the common block elements, but if you declare the common block as a module variable you may access the elements by their name:
 
 
 ````fortran
```

### Comparing `gfort2py-2.0.0/docs/Makefile` & `gfort2py-2.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `gfort2py-2.0.0/docs/make.bat` & `gfort2py-2.1.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `gfort2py-2.0.0/docs/source/conf.py` & `gfort2py-2.1.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `gfort2py-2.0.0/docs/source/fortranabi.rst` & `gfort2py-2.1.0/docs/source/fortranabi.rst`

 * *Files identical despite different names*

### Comparing `gfort2py-2.0.0/docs/source/mod_files.rst` & `gfort2py-2.1.0/docs/source/mod_files.rst`

 * *Files identical despite different names*

### Comparing `gfort2py-2.0.0/gfort2py/fArrays.py` & `gfort2py-2.1.0/gfort2py/fArrays.py`

 * *Files identical despite different names*

### Comparing `gfort2py-2.0.0/gfort2py/fDT.py` & `gfort2py-2.1.0/gfort2py/fDT.py`

 * *Files identical despite different names*

### Comparing `gfort2py-2.0.0/gfort2py/fProc.py` & `gfort2py-2.1.0/gfort2py/fProc.py`

 * *Files identical despite different names*

### Comparing `gfort2py-2.0.0/gfort2py/fScalars.py` & `gfort2py-2.1.0/gfort2py/fScalars.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # SPDX-License-Identifier: GPL-2.0+
 
 import ctypes
+import numpy as np
 
 from .fVar_t import fVar_t
 
 
 class fScalar(fVar_t):
     def ctype(self):
         return self._ctype_base
@@ -19,15 +20,18 @@
     @property
     def value(self):
         if self.type == "INTEGER":
             return int(self.cvalue.value)
         elif self.type == "REAL":
             if self.kind == 16:
                 raise NotImplementedError(f"Quad precision floats not supported yet")
-            return float(self.cvalue.value)
+            elif self.kind == 8:
+                return np.double(self.cvalue.value)
+            else:
+                return float(self.cvalue.value)
         elif self.type == "LOGICAL":
             return self.cvalue.value == 1
 
     @value.setter
     def value(self, value):
         self.from_param(value)
```

### Comparing `gfort2py-2.0.0/gfort2py/fStrings.py` & `gfort2py-2.1.0/gfort2py/fStrings.py`

 * *Files identical despite different names*

### Comparing `gfort2py-2.0.0/gfort2py/fUnary.py` & `gfort2py-2.1.0/gfort2py/fUnary.py`

 * *Files 14% similar despite different names*

```diff
@@ -31,13 +31,16 @@
     "PARENTHESES": None,
     "USER": None,
     "NULL": None,
 }
 
 
 def run_unary(unary, x, y, *, ops=default_ops):
+    if unary == "PARENTHESES":
+        return x
+
     op = ops[unary]
 
     if op is None:
         raise NotImplementedError(f"Unary op {unary} not implemented")
 
     return op(x, y)
```

### Comparing `gfort2py-2.0.0/gfort2py/fVar.py` & `gfort2py-2.1.0/gfort2py/fVar.py`

 * *Files identical despite different names*

### Comparing `gfort2py-2.0.0/gfort2py/fVar_t.py` & `gfort2py-2.1.0/gfort2py/fVar_t.py`

 * *Files identical despite different names*

### Comparing `gfort2py-2.0.0/gfort2py/gfort2py.py` & `gfort2py-2.1.0/gfort2py/gfort2py.py`

 * *Files 5% similar despite different names*

```diff
@@ -100,9 +100,11 @@
     return module(mod_file)
 
 
 def lib_ext():
     os = platform.system()
     if os == "Darwin":
         return "dylib"
+    elif os == "Windows":
+        return "dll"
     else:
         return "so"
```

### Comparing `gfort2py-2.0.0/gfort2py/module_parse.py` & `gfort2py-2.1.0/gfort2py/module_parse.py`

 * *Files 4% similar despite different names*

```diff
@@ -113,27 +113,30 @@
         for i in args[2:]:
             self.id.append(int(i))
 
 
 #################################
 
 
-def hextofloat(s):
+def hextofloat(s, double=False):
     # Given hex like parameter '0.12decde@9' returns 5065465344.0
     man, exp = s.split("@")
     exp = int(exp)
     decimal = man.index(".")
     negative = man[0] == "-"
     man = man[decimal + 1 :]
     man = man.ljust(exp, "0")
     man = man[:exp] + "." + man[exp:]
     man = man + "P0"
     if negative:
         man = "-" + man
-    return float.fromhex(man)
+    if double:
+        return np.double.fromhex(man)
+    else:
+        return float.fromhex(man)
 
 
 #####################################
 
 
 def print_args(x):
     print()
@@ -259,16 +262,15 @@
     def is_assumed_shape(self):
         return self.sym.array_spec.array_type == "ASSUMED_SHAPE"
 
     def is_deferred_len(self):
         # Only needed for things that need an extra function argument for their length
         if self.is_char():
             try:
-                self.sym.ts.charlen.value
-                return False
+                return self.sym.ts.charlen.value == -1
             except AttributeError:
                 return True
         elif self.is_array():
             return self.is_assumed_size()
 
         return False
 
@@ -460,34 +462,40 @@
     class_ref: symbol_ref = None  # If class/derived type symbol_ref else kind
     interface: symbol_ref = None
     is_c_interop: int = -1
     is_iso_c: int = -1
     type2: str = ""  # Repeat of type
     charlen: int = -1  # If character
     deferred_cl: bool = False  # if character and deferred length
+    args = None
 
     def __init__(self, *args):
+        self.args = args
         self.type = args[0]
         if self.type == "CLASS" or self.type == "DERIVED":
             self.class_ref = symbol_ref(args[1])
         else:
             self.kind = int(args[1])
 
         if len(args[2]):
             self.interface = symbol_ref(args[2])
 
         self.is_c_interop = bool(int(args[3]))
         self.is_iso_c = bool(int(args[4]))
         self.type2 = args[5]
         try:
-            self.charlen = expression(
-                *args[6][0]
-            )  # TODO: might this need to be iterated for mulit-d strings?
+            if not args[6][0]:
+                self.charlen = -1
+            else:
+                self.charlen = expression(
+                    *args[6][0]
+                )  # TODO: might this need to be iterated for mulit-d strings?
         except IndexError:
             self.charlen = -1
+
         try:
             self.deferred_cl = args[7] == "DEFERRED_CL"
         except (TypeError, IndexError):
             self.deferred_cl = False
 
 
 @dataclass(init=False)
@@ -496,40 +504,50 @@
     ts: typespec = None
     rank: int = -1
     _value: t.Any = None
     _resolved_value: t.Any = None  # value may by a symbol_ref, so this is the value after resolving the reference
     arglist: actual_arglist = None  # PDT's?
     charlen: int = -1
     unary_op: str = ""
+    unary_args: t.Any = None
+    _unknown: t.Any = None
 
     def __init__(self, *args):
+        self._resolved_value = None
+        if not len(args):
+            return
         self.exp_type = args[0]
         self.ts = typespec(*args[1])
         self.rank = int(args[2])
-        self._resolved_value = None
 
         if self.exp_type == "OP":
             self._value = None
             self.unary_op = args[3]
             self.unary_args = [expression(*args[4]), expression(*args[5])]
-            self._unknown = args[6]  # What is this for?
+            try:
+                self._unknown = args[6]  # What is this for?
+            except IndexError:
+                pass
         elif self.exp_type == "FUNCTION":
             self._value = symbol_ref(args[3])
         elif self.exp_type == "CONSTANT":
             if self.ts.type == "REAL":
-                self._value = hextofloat(string_clean(args[3]))
+                self._value = hextofloat(string_clean(args[3]), self.ts.kind == 8)
             elif self.ts.type == "INTEGER":
                 self._value = int(string_clean(args[3]))
             elif self.ts.type == "CHARACTER":
                 self.charlen = int(args[3])
                 self._value = string_clean(args[4])
             elif self.ts.type == "COMPLEX":
                 self._value = complex(
-                    hextofloat(string_clean(args[3])), hextofloat(string_clean(args[4]))
+                    hextofloat(string_clean(args[3]), self.ts.kind == 8),
+                    hextofloat(string_clean(args[4]), self.ts.kind == 8),
                 )
+            elif self.ts.type == "LOGICAL":
+                self._value = int(args[3]) == 1
             else:
                 raise NotImplementedError(args)
         elif self.exp_type == "VARIABLE":
             self._value = symbol_ref(args[3])
         elif self.exp_type == "SUBSTRING":
             raise NotImplementedError(args)
         elif self.exp_type == "ARRAY":
```

### Comparing `gfort2py-2.0.0/gfort2py.egg-info/PKG-INFO` & `gfort2py-2.1.0/gfort2py.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gfort2py
-Version: 2.0.0
+Version: 2.1.0
 Summary: "Python bindings for Fortran"
 Home-page: https://github.com/rjfarmer/gfort2py
 Author: Robert Farmer
 Author-email: robert.j.farmer37@gmail.com
 License: GPLv2+
 Platform: unix
 Platform: linux
@@ -23,22 +23,20 @@
 Provides-Extra: dev
 License-File: COPYING.txt
 
 [![Continuous Integration](https://github.com/rjfarmer/gfort2py/actions/workflows/ci.yml/badge.svg)](https://github.com/rjfarmer/gfort2py/actions/workflows/ci.yml)
 [![Coverage Status](https://coveralls.io/repos/github/rjfarmer/gfort2py/badge.svg?branch=main)](https://coveralls.io/github/rjfarmer/gfort2py?branch=main)
 [![PyPI version](https://badge.fury.io/py/gfort2py.svg)](https://badge.fury.io/py/gfort2py)
 [![DOI](https://zenodo.org/badge/72889348.svg)](https://zenodo.org/badge/latestdoi/72889348)
-
+[![Python versions](https://img.shields.io/pypi/pyversions/gfort2py.svg)](https://img.shields.io/pypi/pyversions/gfort2py.svg)
 
 
 # gfort2py
 Library to allow calling Fortran code from Python. Requires gfortran>=8.0, Works with python >= 3.7
 
-The current stable version is 1.1.7
-
 ## Build
 ````bash
 pip3 install -r requirements.txt
 python3 setup.py install --user
 ````
 
 or install via pip
@@ -73,14 +71,20 @@
 
 On MacOS: 
 ````bash
 gfortran -dynamiclib -c file.f90
 gfortran -dynamiclib -o libfile file.f90
 ````
 
+On Windows:
+````bash
+gfortran -shared -c file.f90
+gfortran -shared -o libfile.dll file.f90
+````
+
 If your code comes as program that does everything, then just turn the program into a function call inside a module,
 then create a new file with your program that uses the module and calls the function you just made.
 
 If the shared library needs other
 shared libraries you will need to set LD_LIBRARY_PATH environment variable, and it is also recommended is to run chrpath on the 
 shared libraries so you can access them from anywhere.
 
@@ -243,15 +247,15 @@
 - [x] Allocatable arrays of strings
 - [x] Pointer arguments 
 - [x] Optional arguments
 - [x] Value arguments
 - [x] Keyword arguments
 - [ ] Generic/Elemental functions
 - [ ] Functions as an argument
-- [ ] Unary operations (arguments that involve an expression to evaluate like dimension(n+1))
+- [x] Unary operations (arguments that involve an expression to evaluate like dimension(n+1) or dimension((2*n)+1))
 
 ### Accessing common block elements
 
 There's no direct way to access the common block elements, but if you declare the common block as a module variable you may access the elements by their name:
 
 
 ````fortran
```

### Comparing `gfort2py-2.0.0/gfort2py.egg-info/SOURCES.txt` & `gfort2py-2.1.0/gfort2py.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 .gitignore
 .pre-commit-config.yaml
 .readthedocs.yml
+.zenodo.json
 CODE_OF_CONDUCT.md
 COPYING.txt
 MANIFEST.in
 README.md
 dependabot.yml
 pyproject.toml
 requirements.txt
 requirements_dev.txt
 setup.cfg
 setup.py
 tox.ini
+.github/dependabot.yml
 .github/workflows/ci-mac.yml
+.github/workflows/ci-old.yml
 .github/workflows/ci.yml
-.github/workflows/ci_old.yml
 .github/workflows/coveralls.yml
 .github/workflows/pypi.yml
 docs/Makefile
 docs/make.bat
 docs/source/conf.py
 docs/source/fortranabi.rst
 docs/source/index.rst
```

### Comparing `gfort2py-2.0.0/setup.cfg` & `gfort2py-2.1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `gfort2py-2.0.0/tests/Makefile` & `gfort2py-2.1.0/tests/Makefile`

 * *Files 10% similar despite different names*

```diff
@@ -8,24 +8,28 @@
 SRCS = $(wildcard *.f90)
 MODS =  $(wildcard *.mod)
 
 GZ = $(patsubst %.mod,%.gz,$(MODS))
 
 UNAME_S := $(shell uname -s)
 
-ifeq ($(UNAME_S),Linux)
-   # Rpaths need to resolve relative to module/test folder plus the final location of the library
+ifeq ($(OS),Windows_NT)
+   LIB_FLAGS = -shared
+   LIB_SUFFIX = dll
+   LIBS = $(patsubst %.f90,%.dll,$(SRCS))
+else ifeq ($(UNAME_S),Linux)
    LIB_FLAGS = -fPIC -shared
    LIB_SUFFIX = so
    LIBS = $(patsubst %.f90,%.so,$(SRCS))
-endif
-ifeq ($(UNAME_S),Darwin)
+else ifeq ($(UNAME_S),Darwin)
    LIB_FLAGS = -dynamiclib
    LIB_SUFFIX = dylib
    LIBS = $(patsubst %.f90,%.dylib,$(SRCS))
+else
+$(error Unknown OS)
 endif
 
 
 all: $(LIBS) $(GZ)
 
 
 %.$(LIB_SUFFIX): %.f90
```

### Comparing `gfort2py-2.0.0/tests/README.md` & `gfort2py-2.1.0/tests/README.md`

 * *Files identical despite different names*

### Comparing `gfort2py-2.0.0/tests/basic.f90` & `gfort2py-2.1.0/tests/basic.f90`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,18 @@
 		integer, parameter :: dp = selected_real_kind(p=15)
 		integer, parameter :: qp = selected_real_kind(p=30)
 		integer, parameter :: lp = selected_int_kind(8)
 		
 		integer, parameter      :: const_int=1
 		integer, parameter      :: const_int_p1=const_int+1
 		integer(lp), parameter  :: const_int_lp=1_lp
+
+		logical,parameter :: const_logical_true=.true.
+		logical,parameter :: const_logical_false=.false.
+
 		
 		real, parameter     :: const_real=1.0
 		real(dp), parameter :: const_real_dp=1.0_dp
 		real(dp), parameter :: const_real_pi_dp=3.14_dp
 		real(qp), parameter :: const_real_qp=1.0_qp
 
 		integer, parameter :: const_neg_int = -1.0
```

### Comparing `gfort2py-2.0.0/tests/basic_test.py` & `gfort2py-2.1.0/tests/basic_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -216,7 +216,11 @@
         y = x.func_test_bool(0)
         assert type(y.result) == bool
         self.assertEqual(y.result, False)
 
     def test_negatives(self):
         assert x.const_neg_int == -1
         assert x.const_neg_real == -3.14
+
+    def test_logical_parammeters(self):
+        assert x.const_logical_true
+        assert not x.const_logical_false
```

### Comparing `gfort2py-2.0.0/tests/common.f90` & `gfort2py-2.1.0/tests/common.f90`

 * *Files identical despite different names*

### Comparing `gfort2py-2.0.0/tests/complex.f90` & `gfort2py-2.1.0/tests/complex.f90`

 * *Files identical despite different names*

### Comparing `gfort2py-2.0.0/tests/complex_test.py` & `gfort2py-2.1.0/tests/complex_test.py`

 * *Files identical despite different names*

### Comparing `gfort2py-2.0.0/tests/dt.f90` & `gfort2py-2.1.0/tests/dt.f90`

 * *Files identical despite different names*

### Comparing `gfort2py-2.0.0/tests/dt_test.py` & `gfort2py-2.1.0/tests/dt_test.py`

 * *Files identical despite different names*

### Comparing `gfort2py-2.0.0/tests/dummy_arrays.f90` & `gfort2py-2.1.0/tests/dummy_arrays.f90`

 * *Files identical despite different names*

### Comparing `gfort2py-2.0.0/tests/dummy_arrays_test.py` & `gfort2py-2.1.0/tests/dummy_arrays_test.py`

 * *Files identical despite different names*

### Comparing `gfort2py-2.0.0/tests/elemental.f90` & `gfort2py-2.1.0/tests/elemental.f90`

 * *Files identical despite different names*

### Comparing `gfort2py-2.0.0/tests/explicit_arrays.f90` & `gfort2py-2.1.0/tests/explicit_arrays.f90`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,16 @@
 	integer, parameter :: qp = selected_real_kind(p=30)
 	integer, parameter :: lp = selected_int_kind(8)
 	
 	
 	integer,parameter,dimension(10) :: const_int_arr=(/1,2,3,4,5,6,7,8,9,0/)
 	real,parameter,dimension(10) :: const_real_arr=(/1.0,2.0,3.0,4.0,5.0,6.0,7.0,8.0,9.0,0.0/)
 	real(dp),parameter,dimension(10) :: const_real_dp_arr=(/1_dp,2_dp,3_dp,4_dp,5_dp,6_dp,7_dp,8_dp,9_dp,0_dp/)
-	
+	logical, parameter, dimension(5) :: const_logical_arr=(/.true.,.false.,.true.,.false.,.true./)
+
 	! Arrays
 	integer, dimension(5) :: b_int_exp_1d
 	integer, dimension(5,5) :: b_int_exp_2d
 	integer, dimension(5,5,5) :: b_int_exp_3d
 	integer, dimension(5,5,5,5) :: b_int_exp_4d
 	integer, dimension(5,5,5,5,5) :: b_int_exp_5d
 	
@@ -138,14 +139,38 @@
 		integer :: i
 		
 		do i=1,n+1
 			mesh(i) = i
 		end do
 		
 	end function func_mesh_exp
+
+
+	subroutine func_mesh_exp2(x,N) 
+		integer, intent(in) :: N
+		integer :: x(N+1)
+		integer :: i
+		
+		do i=1,n+1
+			x(i) = i
+		end do
+		
+	end subroutine func_mesh_exp2
+
+
+	subroutine func_mesh_exp3(x,N) 
+		integer, intent(in) :: N
+		integer :: x((N*2)+1)
+		integer :: i
+		
+		do i=1,(N*2)+1
+			x(i) = i
+		end do
+		
+	end subroutine func_mesh_exp3
 	
 	
 	subroutine check_exp_2d_2m3(arr, success)
 		! Github issues #19
 		integer, dimension(2,3) :: arr
 		logical :: success
```

### Comparing `gfort2py-2.0.0/tests/explicit_arrays_test.py` & `gfort2py-2.1.0/tests/explicit_arrays_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -251,22 +251,33 @@
     def test_logical_arr_multi(self):
         xarr = np.zeros(5)
         xarr[:] = True
 
         y = x.func_logical_multi(1.0, 2.0, xarr, 3.0, 4.0)
         self.assertEqual(y.result, True)
 
-    @pytest.mark.skip("Skipping as we seg fault")
+    @pytest.mark.skip
     def test_mesh_exp(self):
         # Github issue #13
         i = 5
         y = x.func_mesh_exp(i)
-        self.assertEqual(y.result, np.arrange(0, i))
+        np.all(y.result == np.arrange(0, i + 1 + 1))
+
+    def test_mesh_exp2(self):
+        i = 5
+        z = np.zeros(i + 1)
+        y = x.func_mesh_exp2(z, i)
+        assert np.all(y.args["x"] == np.arange(1, i + 1 + 1))
+
+    def test_mesh_exp3(self):
+        i = 5
+        z = np.zeros((i * 2) + 1)
+        y = x.func_mesh_exp3(z, i)
+        assert np.all(y.args["x"] == np.arange(1, (i * 2) + 1 + 1))
 
-    @pytest.mark.skip
     def test_check_exp_2d_2m3(self):
         # Github issue #19
         arr_test = np.zeros((3, 4), dtype=int, order="F")
 
         arr_test[0, 1] = 1
         arr_test[1, 0] = 2
         arr_test[1, 2] = 3
@@ -275,7 +286,13 @@
         y = x.check_exp_2d_2m3_nt(arr_test, 4, 0)
 
         self.assertEqual(y.args["success"], True)
 
         arr_test[0, 3] = 5
 
         np.testing.assert_array_equal(y.args["arr"], arr_test)
+
+    def test_logical_param_array(self):
+        assert np.all(
+            x.const_logical_arr
+            == np.array([True, False, True, False, True], dtype=bool)
+        )
```

### Comparing `gfort2py-2.0.0/tests/interface.f90` & `gfort2py-2.1.0/tests/interface.f90`

 * *Files identical despite different names*

### Comparing `gfort2py-2.0.0/tests/oo.f90` & `gfort2py-2.1.0/tests/oo.f90`

 * *Files identical despite different names*

### Comparing `gfort2py-2.0.0/tests/pdt.f90` & `gfort2py-2.1.0/tests/pdt.f90`

 * *Files identical despite different names*

### Comparing `gfort2py-2.0.0/tests/pointers.f90` & `gfort2py-2.1.0/tests/pointers.f90`

 * *Files identical despite different names*

### Comparing `gfort2py-2.0.0/tests/pointers_test.py` & `gfort2py-2.1.0/tests/pointers_test.py`

 * *Files identical despite different names*

### Comparing `gfort2py-2.0.0/tests/proc_ptrs.f90` & `gfort2py-2.1.0/tests/proc_ptrs.f90`

 * *Files identical despite different names*

### Comparing `gfort2py-2.0.0/tests/proc_ptrs_test.py` & `gfort2py-2.1.0/tests/proc_ptrs_test.py`

 * *Files identical despite different names*

### Comparing `gfort2py-2.0.0/tests/strings.f90` & `gfort2py-2.1.0/tests/strings.f90`

 * *Files 4% similar despite different names*

```diff
@@ -42,14 +42,19 @@
 	type str_array_dt_alloc
 		integer :: start_guard = 123456789
 		character(len=10),dimension(:),allocatable :: b_str_alloc_1d
 		integer :: end_guard = 123456789
 	end type str_array_dt_alloc
 
 
+	type str_array_dt_out
+		character(len=12) :: a_str1, a_str2
+		integer ::  a_int
+	end type str_array_dt_out
+
 	contains
 	
 	subroutine sub_str_in_explicit(x)
 		character(len=10), intent(in) ::x
 		write(output_unit,*) trim(x)
 	end subroutine sub_str_in_explicit
 	
@@ -331,8 +336,19 @@
 		if(b_str_alloc_1d(5) /= 'xxxxxxxxxx') return
 
 		check_b_str_alloc_1d = .true.
 
 	end function check_b_str_alloc_1d
 
 
+	subroutine set_str_array_dt_out(x)
+		type(str_array_dt_out),intent(out) :: x
+
+		x%a_str1 = 'qwertyuiop[]'
+		x%a_str2 = 'asdfghjkl;zx'
+
+		x% a_int = 99
+
+	end subroutine set_str_array_dt_out
+
+
 end module strings
```

### Comparing `gfort2py-2.0.0/tests/strings_test.py` & `gfort2py-2.1.0/tests/strings_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -273,7 +273,14 @@
         assert np.all(
             x.b_str_alloc_1d
             == np.array(
                 ["zzzzzzzzzz", "yyyyyyyyyy", "qqqqqqqqqq", "wwwwwwwwww", "xxxxxxxxxx"],
                 dtype="S10",
             )
         )
+
+    def test_set_str_array_dt_out(self):
+        res = x.set_str_array_dt_out({})
+
+        assert res.args["x"]["a_str1"] == "qwertyuiop[]"
+        assert res.args["x"]["a_str2"] == "asdfghjkl;zx"
+        assert res.args["x"]["a_int"] == 99
```

### Comparing `gfort2py-2.0.0/tests/submodule.f90` & `gfort2py-2.1.0/tests/submodule.f90`

 * *Files identical despite different names*

