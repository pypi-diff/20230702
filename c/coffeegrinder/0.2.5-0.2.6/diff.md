# Comparing `tmp/coffeegrinder-0.2.5.tar.gz` & `tmp/coffeegrinder-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coffeegrinder-0.2.5.tar", last modified: Mon Jun 19 08:31:25 2023, max compression
+gzip compressed data, was "coffeegrinder-0.2.6.tar", last modified: Sun Jul  2 02:59:59 2023, max compression
```

## Comparing `coffeegrinder-0.2.5.tar` & `coffeegrinder-0.2.6.tar`

### file list

```diff
@@ -1,163 +1,86 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:31:25.393846 coffeegrinder-0.2.5/
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-06-19 08:31:14.000000 coffeegrinder-0.2.5/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:31:25.345845 coffeegrinder-0.2.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:31:25.357845 coffeegrinder-0.2.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-19 08:31:14.000000 coffeegrinder-0.2.5/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-06-19 08:31:14.000000 coffeegrinder-0.2.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-19 08:31:14.000000 coffeegrinder-0.2.5/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-19 08:31:14.000000 coffeegrinder-0.2.5/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-19 08:31:14.000000 coffeegrinder-0.2.5/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)    13801 2023-06-19 08:31:14.000000 coffeegrinder-0.2.5/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-06-19 08:31:14.000000 coffeegrinder-0.2.5/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-06-19 08:31:25.393846 coffeegrinder-0.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-06-19 08:31:14.000000 coffeegrinder-0.2.5/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:31:25.357845 coffeegrinder-0.2.5/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-19 08:31:14.000000 coffeegrinder-0.2.5/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:31:25.357845 coffeegrinder-0.2.5/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-19 08:31:14.000000 coffeegrinder-0.2.5/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-19 08:31:14.000000 coffeegrinder-0.2.5/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-19 08:31:14.000000 coffeegrinder-0.2.5/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9729 2023-06-19 08:31:14.000000 coffeegrinder-0.2.5/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-19 08:31:14.000000 coffeegrinder-0.2.5/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-06-19 08:31:14.000000 coffeegrinder-0.2.5/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-19 08:31:14.000000 coffeegrinder-0.2.5/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-19 08:31:14.000000 coffeegrinder-0.2.5/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-19 08:31:14.000000 coffeegrinder-0.2.5/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-06-19 08:31:14.000000 coffeegrinder-0.2.5/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:31:25.361845 coffeegrinder-0.2.5/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-06-19 08:31:14.000000 coffeegrinder-0.2.5/scripts/compare.py
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-06-19 08:31:14.000000 coffeegrinder-0.2.5/scripts/dataOverTime.py
--rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-06-19 08:31:14.000000 coffeegrinder-0.2.5/scripts/details.py
--rw-r--r--   0 runner    (1001) docker     (123)    15025 2023-06-19 08:31:14.000000 coffeegrinder-0.2.5/scripts/error.py
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-06-19 08:31:14.000000 coffeegrinder-0.2.5/scripts/extract.py
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-06-19 08:31:14.000000 coffeegrinder-0.2.5/scripts/hdfvis_gnuplot_defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)     5005 2023-06-19 08:31:14.000000 coffeegrinder-0.2.5/scripts/simulate.py
--rw-r--r--   0 runner    (1001) docker     (123)     5286 2023-06-19 08:31:14.000000 coffeegrinder-0.2.5/scripts/viewFunction3D
--rw-r--r--   0 runner    (1001) docker     (123)    17860 2023-06-19 08:31:14.000000 coffeegrinder-0.2.5/scripts/visualise.py
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-06-19 08:31:25.393846 coffeegrinder-0.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-06-19 08:31:14.000000 coffeegrinder-0.2.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:31:25.349845 coffeegrinder-0.2.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:31:25.365846 coffeegrinder-0.2.5/src/coffee/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-19 08:31:14.000000 coffeegrinder-0.2.5/src/coffee/DEPENDENCIES.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-06-19 08:31:14.000000 coffeegrinder-0.2.5/src/coffee/THINGS_TO_DO.txt
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-06-19 08:31:14.000000 coffeegrinder-0.2.5/src/coffee/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:31:25.365846 coffeegrinder-0.2.5/src/coffee/actions/
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-19 08:31:14.000000 coffeegrinder-0.2.5/src/coffee/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-06-19 08:31:14.000000 coffeegrinder-0.2.5/src/coffee/actions/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9225 2023-06-19 08:31:14.000000 coffeegrinder-0.2.5/src/coffee/actions/gp_plotter.py
--rw-r--r--   0 runner    (1001) docker     (123)    13497 2023-06-19 08:31:14.000000 coffeegrinder-0.2.5/src/coffee/actions/hdf_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-06-19 08:31:14.000000 coffeegrinder-0.2.5/src/coffee/actions/mpl_plotter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:31:25.365846 coffeegrinder-0.2.5/src/coffee/backend/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-19 08:31:14.000000 coffeegrinder-0.2.5/src/coffee/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9655 2023-06-19 08:31:14.000000 coffeegrinder-0.2.5/src/coffee/backend/backend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:31:25.369845 coffeegrinder-0.2.5/src/coffee/diffop/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 08:31:14.000000 coffeegrinder-0.2.5/src/coffee/diffop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11945 2023-06-19 08:31:14.000000 coffeegrinder-0.2.5/src/coffee/diffop/fd.py
--rw-r--r--   0 runner    (1001) docker     (123)    11005 2023-06-19 08:31:14.000000 coffeegrinder-0.2.5/src/coffee/diffop/fft.py
--rw-r--r--   0 runner    (1001) docker     (123)     5255 2023-06-19 08:31:14.000000 coffeegrinder-0.2.5/src/coffee/diffop/ghp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-06-19 08:31:14.000000 coffeegrinder-0.2.5/src/coffee/diffop/ghp_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:31:25.369845 coffeegrinder-0.2.5/src/coffee/diffop/sbp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 08:31:14.000000 coffeegrinder-0.2.5/src/coffee/diffop/sbp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17978 2023-06-19 08:31:14.000000 coffeegrinder-0.2.5/src/coffee/diffop/sbp/dissipation.py
--rw-r--r--   0 runner    (1001) docker     (123)    68798 2023-06-19 08:31:14.000000 coffeegrinder-0.2.5/src/coffee/diffop/sbp/dissipation_testing.nb
--rw-r--r--   0 runner    (1001) docker     (123)    27334 2023-06-19 08:31:14.000000 coffeegrinder-0.2.5/src/coffee/diffop/sbp/sbp.py
--rw-r--r--   0 runner    (1001) docker     (123)     5725 2023-06-19 08:31:14.000000 coffeegrinder-0.2.5/src/coffee/free_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:31:25.369845 coffeegrinder-0.2.5/src/coffee/grid/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-19 08:31:14.000000 coffeegrinder-0.2.5/src/coffee/grid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28687 2023-06-19 08:31:14.000000 coffeegrinder-0.2.5/src/coffee/grid/grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     7398 2023-06-19 08:31:14.000000 coffeegrinder-0.2.5/src/coffee/ibvp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:31:25.369845 coffeegrinder-0.2.5/src/coffee/io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 08:31:14.000000 coffeegrinder-0.2.5/src/coffee/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32934 2023-06-19 08:31:14.000000 coffeegrinder-0.2.5/src/coffee/io/simulation_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:31:25.369845 coffeegrinder-0.2.5/src/coffee/mpi/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 08:31:14.000000 coffeegrinder-0.2.5/src/coffee/mpi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14845 2023-06-19 08:31:14.000000 coffeegrinder-0.2.5/src/coffee/mpi/mpiinterfaces.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:31:25.373846 coffeegrinder-0.2.5/src/coffee/solvers/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-19 08:31:14.000000 coffeegrinder-0.2.5/src/coffee/solvers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8916 2023-06-19 08:31:14.000000 coffeegrinder-0.2.5/src/coffee/solvers/solvers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:31:25.373846 coffeegrinder-0.2.5/src/coffee/swsh/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-19 08:31:14.000000 coffeegrinder-0.2.5/src/coffee/swsh/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:31:25.349845 coffeegrinder-0.2.5/src/coffee/swsh/c_code/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:31:25.373846 coffeegrinder-0.2.5/src/coffee/swsh/c_code/boris/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-19 08:31:14.000000 coffeegrinder-0.2.5/src/coffee/swsh/c_code/boris/makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:31:25.377846 coffeegrinder-0.2.5/src/coffee/swsh/c_code/boris/src/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-19 08:31:14.000000 coffeegrinder-0.2.5/src/coffee/swsh/c_code/boris/src/README.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-06-19 08:31:14.000000 coffeegrinder-0.2.5/src/coffee/swsh/c_code/boris/src/genArrManip.c
--rw-r--r--   0 runner    (1001) docker     (123)    12643 2023-06-19 08:31:14.000000 coffeegrinder-0.2.5/src/coffee/swsh/c_code/boris/src/genArrSorting.c
--rw-r--r--   0 runner    (1001) docker     (123)    18052 2023-06-19 08:31:14.000000 coffeegrinder-0.2.5/src/coffee/swsh/c_code/boris/src/hdf5Interface.c
--rw-r--r--   0 runner    (1001) docker     (123)     8295 2023-06-19 08:31:14.000000 coffeegrinder-0.2.5/src/coffee/swsh/c_code/boris/src/hdf5rwDataStructs.c
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-06-19 08:31:14.000000 coffeegrinder-0.2.5/src/coffee/swsh/c_code/boris/src/make.sh
--rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-06-19 08:31:14.000000 coffeegrinder-0.2.5/src/coffee/swsh/c_code/boris/src/mathClebschGordan.c
--rw-r--r--   0 runner    (1001) docker     (123)    17134 2023-06-19 08:31:14.000000 coffeegrinder-0.2.5/src/coffee/swsh/c_code/boris/src/mathWigner3j.c
--rw-r--r--   0 runner    (1001) docker     (123)    22748 2023-06-19 08:31:14.000000 coffeegrinder-0.2.5/src/coffee/swsh/c_code/boris/src/mathWigner3jRecursion.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:31:25.377846 coffeegrinder-0.2.5/src/coffee/swsh/c_code/boris/src/test/
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-06-19 08:31:14.000000 coffeegrinder-0.2.5/src/coffee/swsh/c_code/boris/src/test/calcCoef_mem_issue_tester.c
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-06-19 08:31:14.000000 coffeegrinder-0.2.5/src/coffee/swsh/c_code/boris/src/test/calcCoef_mem_issue_tester.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:31:25.377846 coffeegrinder-0.2.5/src/coffee/swsh/c_code/rrf-3.2/
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-06-19 08:31:14.000000 coffeegrinder-0.2.5/src/coffee/swsh/c_code/rrf-3.2/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-06-19 08:31:14.000000 coffeegrinder-0.2.5/src/coffee/swsh/c_code/rrf-3.2/README
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:31:25.385846 coffeegrinder-0.2.5/src/coffee/swsh/c_code/rrf-3.2/src/
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-06-19 08:31:14.000000 coffeegrinder-0.2.5/src/coffee/swsh/c_code/rrf-3.2/src/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     8892 2023-06-19 08:31:14.000000 coffeegrinder-0.2.5/src/coffee/swsh/c_code/rrf-3.2/src/arithmetic.f90
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-06-19 08:31:14.000000 coffeegrinder-0.2.5/src/coffee/swsh/c_code/rrf-3.2/src/arithmetic.mod
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-06-19 08:31:14.000000 coffeegrinder-0.2.5/src/coffee/swsh/c_code/rrf-3.2/src/compile.sh
--rw-r--r--   0 runner    (1001) docker     (123)    13754 2023-06-19 08:31:14.000000 coffeegrinder-0.2.5/src/coffee/swsh/c_code/rrf-3.2/src/conversions.f90
--rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-06-19 08:31:14.000000 coffeegrinder-0.2.5/src/coffee/swsh/c_code/rrf-3.2/src/conversions.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-06-19 08:31:14.000000 coffeegrinder-0.2.5/src/coffee/swsh/c_code/rrf-3.2/src/factorials.f90
--rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-06-19 08:31:14.000000 coffeegrinder-0.2.5/src/coffee/swsh/c_code/rrf-3.2/src/factorials.mod
--rw-r--r--   0 runner    (1001) docker     (123)    26682 2023-06-19 08:31:14.000000 coffeegrinder-0.2.5/src/coffee/swsh/c_code/rrf-3.2/src/input.f90
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-06-19 08:31:14.000000 coffeegrinder-0.2.5/src/coffee/swsh/c_code/rrf-3.2/src/input.mod
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 08:31:14.000000 coffeegrinder-0.2.5/src/coffee/swsh/c_code/rrf-3.2/src/modules
--rw-r--r--   0 runner    (1001) docker     (123)    13146 2023-06-19 08:31:14.000000 coffeegrinder-0.2.5/src/coffee/swsh/c_code/rrf-3.2/src/rrfcalc.f90
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-06-19 08:31:14.000000 coffeegrinder-0.2.5/src/coffee/swsh/c_code/rrf-3.2/src/rrfdata.f90
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-06-19 08:31:14.000000 coffeegrinder-0.2.5/src/coffee/swsh/c_code/rrf-3.2/src/rrfdata.mod
--rw-r--r--   0 runner    (1001) docker     (123)     5997 2023-06-19 08:31:14.000000 coffeegrinder-0.2.5/src/coffee/swsh/c_code/rrf-3.2/src/rrflist.f90
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-06-19 08:31:14.000000 coffeegrinder-0.2.5/src/coffee/swsh/c_code/rrf-3.2/src/rrflist.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-06-19 08:31:14.000000 coffeegrinder-0.2.5/src/coffee/swsh/c_code/rrf-3.2/src/start.f90
--rw-r--r--   0 runner    (1001) docker     (123)     4564 2023-06-19 08:31:14.000000 coffeegrinder-0.2.5/src/coffee/swsh/c_code/rrf-3.2/src/test3j.f90
--rw-r--r--   0 runner    (1001) docker     (123)    11371 2023-06-19 08:31:14.000000 coffeegrinder-0.2.5/src/coffee/swsh/c_code/rrf-3.2/src/test6j.f90
--rw-r--r--   0 runner    (1001) docker     (123)     4715 2023-06-19 08:31:14.000000 coffeegrinder-0.2.5/src/coffee/swsh/c_code/rrf-3.2/src/test9j.f90
--rw-r--r--   0 runner    (1001) docker     (123)     9561 2023-06-19 08:31:14.000000 coffeegrinder-0.2.5/src/coffee/swsh/c_code/rrf-3.2/src/wigner.f90
--rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-06-19 08:31:14.000000 coffeegrinder-0.2.5/src/coffee/swsh/c_code/rrf-3.2/src/wigner.mod
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:31:25.385846 coffeegrinder-0.2.5/src/coffee/swsh/clebschgordan/
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-19 08:31:14.000000 coffeegrinder-0.2.5/src/coffee/swsh/clebschgordan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12995 2023-06-19 08:31:14.000000 coffeegrinder-0.2.5/src/coffee/swsh/clebschgordan/clebschgordan.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:31:25.385846 coffeegrinder-0.2.5/src/coffee/swsh/lib/
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-19 08:31:14.000000 coffeegrinder-0.2.5/src/coffee/swsh/lib/how_to_make_libspinsfast.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3558 2023-06-19 08:31:14.000000 coffeegrinder-0.2.5/src/coffee/swsh/salm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:31:25.385846 coffeegrinder-0.2.5/src/coffee/swsh/spinsfastpy/
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-06-19 08:31:14.000000 coffeegrinder-0.2.5/src/coffee/swsh/spinsfastpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-06-19 08:31:14.000000 coffeegrinder-0.2.5/src/coffee/swsh/spinsfastpy/backward_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-06-19 08:31:14.000000 coffeegrinder-0.2.5/src/coffee/swsh/spinsfastpy/forward_transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:31:25.389846 coffeegrinder-0.2.5/src/coffee/swsh/spinsfastpy/huffenberger_wandelt/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-19 08:31:14.000000 coffeegrinder-0.2.5/src/coffee/swsh/spinsfastpy/huffenberger_wandelt/README.TXT
--rw-r--r--   0 runner    (1001) docker     (123)    35523 2023-06-19 08:31:14.000000 coffeegrinder-0.2.5/src/coffee/swsh/spinsfastpy/huffenberger_wandelt/spinsfast_rev104.tar.gz
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-06-19 08:31:14.000000 coffeegrinder-0.2.5/src/coffee/swsh/spinsfastpy/index_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-06-19 08:31:14.000000 coffeegrinder-0.2.5/src/coffee/swsh/spinsfastpy/io.py
--rw-r--r--   0 runner    (1001) docker     (123)    37023 2023-06-19 08:31:14.000000 coffeegrinder-0.2.5/src/coffee/swsh/spinsfastpy/salm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:31:25.389846 coffeegrinder-0.2.5/src/coffee/swsh/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-06-19 08:31:14.000000 coffeegrinder-0.2.5/src/coffee/swsh/test/test_swsh.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:31:25.389846 coffeegrinder-0.2.5/src/coffee/swsh/w3j/
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-19 08:31:14.000000 coffeegrinder-0.2.5/src/coffee/swsh/w3j/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24655 2023-06-19 08:31:14.000000 coffeegrinder-0.2.5/src/coffee/swsh/w3j/w3j.py
--rw-r--r--   0 runner    (1001) docker     (123)     5149 2023-06-19 08:31:14.000000 coffeegrinder-0.2.5/src/coffee/system.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:31:25.389846 coffeegrinder-0.2.5/src/coffee/tslices/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 08:31:14.000000 coffeegrinder-0.2.5/src/coffee/tslices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11364 2023-06-19 08:31:14.000000 coffeegrinder-0.2.5/src/coffee/tslices/tslices.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:31:25.393846 coffeegrinder-0.2.5/src/coffeegrinder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-06-19 08:31:25.000000 coffeegrinder-0.2.5/src/coffeegrinder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4330 2023-06-19 08:31:25.000000 coffeegrinder-0.2.5/src/coffeegrinder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 08:31:25.000000 coffeegrinder-0.2.5/src/coffeegrinder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 08:31:25.000000 coffeegrinder-0.2.5/src/coffeegrinder.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-19 08:31:25.000000 coffeegrinder-0.2.5/src/coffeegrinder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-19 08:31:25.000000 coffeegrinder-0.2.5/src/coffeegrinder.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:31:25.353845 coffeegrinder-0.2.5/systems/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:31:25.393846 coffeegrinder-0.2.5/systems/TwoDAdvection/
--rw-r--r--   0 runner    (1001) docker     (123)     8704 2023-06-19 08:31:14.000000 coffeegrinder-0.2.5/systems/TwoDAdvection/TwoDAdvection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-06-19 08:31:14.000000 coffeegrinder-0.2.5/systems/TwoDAdvection/TwoDAdvection_plotter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7143 2023-06-19 08:31:14.000000 coffeegrinder-0.2.5/systems/TwoDAdvection/TwoDAdvection_setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 08:31:25.393846 coffeegrinder-0.2.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-19 08:31:14.000000 coffeegrinder-0.2.5/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-06-19 08:31:14.000000 coffeegrinder-0.2.5/tests/test_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-06-19 08:31:14.000000 coffeegrinder-0.2.5/tests/test_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-06-19 08:31:14.000000 coffeegrinder-0.2.5/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 02:59:59.705159 coffeegrinder-0.2.6/
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-02 02:59:46.000000 coffeegrinder-0.2.6/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 02:59:59.677158 coffeegrinder-0.2.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 02:59:59.689159 coffeegrinder-0.2.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-02 02:59:46.000000 coffeegrinder-0.2.6/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-07-02 02:59:46.000000 coffeegrinder-0.2.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-02 02:59:46.000000 coffeegrinder-0.2.6/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-02 02:59:46.000000 coffeegrinder-0.2.6/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-02 02:59:46.000000 coffeegrinder-0.2.6/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    13801 2023-07-02 02:59:46.000000 coffeegrinder-0.2.6/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-02 02:59:46.000000 coffeegrinder-0.2.6/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2940 2023-07-02 02:59:59.705159 coffeegrinder-0.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-07-02 02:59:46.000000 coffeegrinder-0.2.6/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 02:59:59.689159 coffeegrinder-0.2.6/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-02 02:59:46.000000 coffeegrinder-0.2.6/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 02:59:59.689159 coffeegrinder-0.2.6/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-02 02:59:46.000000 coffeegrinder-0.2.6/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-02 02:59:46.000000 coffeegrinder-0.2.6/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-02 02:59:46.000000 coffeegrinder-0.2.6/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9729 2023-07-02 02:59:46.000000 coffeegrinder-0.2.6/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-02 02:59:46.000000 coffeegrinder-0.2.6/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-07-02 02:59:46.000000 coffeegrinder-0.2.6/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-02 02:59:46.000000 coffeegrinder-0.2.6/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-02 02:59:46.000000 coffeegrinder-0.2.6/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-02 02:59:46.000000 coffeegrinder-0.2.6/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-07-02 02:59:46.000000 coffeegrinder-0.2.6/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 02:59:59.689159 coffeegrinder-0.2.6/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-07-02 02:59:46.000000 coffeegrinder-0.2.6/scripts/compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-07-02 02:59:59.709159 coffeegrinder-0.2.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-02 02:59:46.000000 coffeegrinder-0.2.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 02:59:59.681159 coffeegrinder-0.2.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 02:59:59.693159 coffeegrinder-0.2.6/src/coffee/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-02 02:59:46.000000 coffeegrinder-0.2.6/src/coffee/DEPENDENCIES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-02 02:59:46.000000 coffeegrinder-0.2.6/src/coffee/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 02:59:59.693159 coffeegrinder-0.2.6/src/coffee/actions/
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-02 02:59:46.000000 coffeegrinder-0.2.6/src/coffee/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-07-02 02:59:46.000000 coffeegrinder-0.2.6/src/coffee/actions/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9225 2023-07-02 02:59:47.000000 coffeegrinder-0.2.6/src/coffee/actions/gp_plotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13497 2023-07-02 02:59:47.000000 coffeegrinder-0.2.6/src/coffee/actions/hdf_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-07-02 02:59:47.000000 coffeegrinder-0.2.6/src/coffee/actions/mpl_plotter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 02:59:59.697159 coffeegrinder-0.2.6/src/coffee/backend/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-02 02:59:47.000000 coffeegrinder-0.2.6/src/coffee/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9657 2023-07-02 02:59:47.000000 coffeegrinder-0.2.6/src/coffee/backend/backend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 02:59:59.697159 coffeegrinder-0.2.6/src/coffee/diffop/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 02:59:47.000000 coffeegrinder-0.2.6/src/coffee/diffop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11945 2023-07-02 02:59:47.000000 coffeegrinder-0.2.6/src/coffee/diffop/fd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 02:59:59.697159 coffeegrinder-0.2.6/src/coffee/diffop/sbp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 02:59:47.000000 coffeegrinder-0.2.6/src/coffee/diffop/sbp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17978 2023-07-02 02:59:47.000000 coffeegrinder-0.2.6/src/coffee/diffop/sbp/dissipation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68798 2023-07-02 02:59:47.000000 coffeegrinder-0.2.6/src/coffee/diffop/sbp/dissipation_testing.nb
+-rw-r--r--   0 runner    (1001) docker     (123)    27334 2023-07-02 02:59:47.000000 coffeegrinder-0.2.6/src/coffee/diffop/sbp/sbp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5725 2023-07-02 02:59:47.000000 coffeegrinder-0.2.6/src/coffee/free_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 02:59:59.697159 coffeegrinder-0.2.6/src/coffee/grid/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-02 02:59:47.000000 coffeegrinder-0.2.6/src/coffee/grid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28687 2023-07-02 02:59:47.000000 coffeegrinder-0.2.6/src/coffee/grid/grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7398 2023-07-02 02:59:47.000000 coffeegrinder-0.2.6/src/coffee/ibvp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 02:59:59.701159 coffeegrinder-0.2.6/src/coffee/io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 02:59:47.000000 coffeegrinder-0.2.6/src/coffee/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32849 2023-07-02 02:59:47.000000 coffeegrinder-0.2.6/src/coffee/io/simulation_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 02:59:59.701159 coffeegrinder-0.2.6/src/coffee/mpi/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 02:59:47.000000 coffeegrinder-0.2.6/src/coffee/mpi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14805 2023-07-02 02:59:47.000000 coffeegrinder-0.2.6/src/coffee/mpi/mpiinterfaces.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 02:59:59.701159 coffeegrinder-0.2.6/src/coffee/solvers/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-02 02:59:47.000000 coffeegrinder-0.2.6/src/coffee/solvers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8879 2023-07-02 02:59:47.000000 coffeegrinder-0.2.6/src/coffee/solvers/solvers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5149 2023-07-02 02:59:47.000000 coffeegrinder-0.2.6/src/coffee/system.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 02:59:59.701159 coffeegrinder-0.2.6/src/coffee/tslices/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-02 02:59:47.000000 coffeegrinder-0.2.6/src/coffee/tslices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11324 2023-07-02 02:59:47.000000 coffeegrinder-0.2.6/src/coffee/tslices/tslices.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 02:59:59.705159 coffeegrinder-0.2.6/src/coffeegrinder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2940 2023-07-02 02:59:59.000000 coffeegrinder-0.2.6/src/coffeegrinder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-07-02 02:59:59.000000 coffeegrinder-0.2.6/src/coffeegrinder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 02:59:59.000000 coffeegrinder-0.2.6/src/coffeegrinder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 02:59:59.000000 coffeegrinder-0.2.6/src/coffeegrinder.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-02 02:59:59.000000 coffeegrinder-0.2.6/src/coffeegrinder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-02 02:59:59.000000 coffeegrinder-0.2.6/src/coffeegrinder.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 02:59:59.681159 coffeegrinder-0.2.6/systems/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 02:59:59.705159 coffeegrinder-0.2.6/systems/OneDAdvection/
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-07-02 02:59:47.000000 coffeegrinder-0.2.6/systems/OneDAdvection/OneDAdvection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-07-02 02:59:47.000000 coffeegrinder-0.2.6/systems/OneDAdvection/OneDAdvection_plotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5653 2023-07-02 02:59:47.000000 coffeegrinder-0.2.6/systems/OneDAdvection/OneDAdvection_setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 02:59:59.705159 coffeegrinder-0.2.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-07-02 02:59:47.000000 coffeegrinder-0.2.6/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-07-02 02:59:47.000000 coffeegrinder-0.2.6/tests/test_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-07-02 02:59:47.000000 coffeegrinder-0.2.6/tests/test_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-07-02 02:59:47.000000 coffeegrinder-0.2.6/tox.ini
```

### Comparing `coffeegrinder-0.2.5/.coveragerc` & `coffeegrinder-0.2.6/.coveragerc`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.2.5/.github/workflows/python-publish.yml` & `coffeegrinder-0.2.6/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.2.5/.gitignore` & `coffeegrinder-0.2.6/.gitignore`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.2.5/.readthedocs.yml` & `coffeegrinder-0.2.6/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.2.5/CONTRIBUTING.rst` & `coffeegrinder-0.2.6/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.2.5/LICENSE.txt` & `coffeegrinder-0.2.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.2.5/PKG-INFO` & `coffeegrinder-0.2.6/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: coffeegrinder
-Version: 0.2.5
-Summary: Add a short description here!
+Version: 0.2.6
+Summary: COFFEE is an MPI-Parallelised Python package for the numerical evolution of time-dependent differential equations.
 Home-page: https://github.com/coffee-gr/coffee
 Author: Chris Stevens
 Author-email: chris.stevens@canterbury.ac.nz
 License: MIT
 Project-URL: Documentation, https://pyscaffold.org/
 Platform: any
 Classifier: Development Status :: 4 - Beta
@@ -48,27 +48,23 @@
 
 
 ======
 coffee
 ======
 
 
-    Add a short description here!
+    COFFEE is an MPI-Parallelised Python package for the numerical evolution of time-dependent differential equations.
 
 
 Installation
 ------------
 
 To use this software, you will need the following dependencies:
 
-- fitsio C library
-- chealpix C library
-- mpich or Open MPI
-- pyFFTW
-- gnuplot + appropriate terminal if needed
+- 
 - HDF library
 
 Please make sure these dependencies are installed before using this software.
 
 .. rubric:: Getting started
 
 One needs to point the ``PYTHONPATH`` environment variable to the packages directory. Then the system code can be run with::
```

### Comparing `coffeegrinder-0.2.5/README.rst` & `coffeegrinder-0.2.6/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -32,27 +32,23 @@
 
 
 ======
 coffee
 ======
 
 
-    Add a short description here!
+    COFFEE is an MPI-Parallelised Python package for the numerical evolution of time-dependent differential equations.
 
 
 Installation
 ------------
 
 To use this software, you will need the following dependencies:
 
-- fitsio C library
-- chealpix C library
-- mpich or Open MPI
-- pyFFTW
-- gnuplot + appropriate terminal if needed
+- 
 - HDF library
 
 Please make sure these dependencies are installed before using this software.
 
 .. rubric:: Getting started
 
 One needs to point the ``PYTHONPATH`` environment variable to the packages directory. Then the system code can be run with::
```

### Comparing `coffeegrinder-0.2.5/docs/Makefile` & `coffeegrinder-0.2.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.2.5/docs/conf.py` & `coffeegrinder-0.2.6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.2.5/docs/index.rst` & `coffeegrinder-0.2.6/docs/index.rst`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.2.5/scripts/compare.py` & `coffeegrinder-0.2.6/scripts/compare.py`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.2.5/scripts/error.py` & `coffeegrinder-0.2.6/src/coffee/mpi/mpiinterfaces.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,396 +1,373 @@
-#! /usr/bin/env python
+"""
+Contains classes that abstract the MPI C API.
 
-
-import argparse
-import sys
-from builtins import range
+Classes in this module model the MPI node network and manage the relationship
+of the complete domain to each 
+"""
 from builtins import str
-from builtins import zip
-
-# from coffee.swsh.spinsfastpy import io as swsh_io
-from coffee.io import simulation_data as sd
-
-
-def exact(args):
-    if args.dg != ["raw"]:
-        print("Exact errors can only be calculated for data type 'raw'.")
-        sys.exit(1)
-
-    with sd.SimulationHDF(args.file) as file:
-        print("Initialising data.")
-        sims = file.getSims()
-
-        # needed for fixing domain size to smallest domain. This will cause
-        # problems when plotting.
-        # smallest_domain = sims[0].domain
-
-        tSimNames = [sim.name for sim in sims]
-        stepsizes = []
-        # We make the assumption that the number of components for each run
-        # is the same and that the values of the components are in the first
-        # axis of raw.shape
-        num_of_comps = sims[0].numvar
-        tableE = be.zeros((len(args.Lp), len(tSimNames), num_of_comps), dtype=float)
-
-        for time in args.t:
-            print("==================================")
-            print("Doing calculation for time = %f" % time)
-            for i, sim in enumerate(sims):
-                # print "Doing calculation for simulation %s"%sim.name
-                it = sim.indexOfTime(time)
-                domain = sim.domain[it]
-
-                # needed for fixing domain size to smallest domain.
-                # This will cause
-                # problems when plotting.
-                # if i == 0:
-                # smallest_it = it
-                # smallest_domain = domain
-
-                print("Index for simulation %s is %i at time %f" % (sim.name, it, time))
-
-                # needed for fixing domain size to smallest domain.
-                # This will cause
-                # problems when plotting.
-                # if __debug__:
-                # print "Index for smallest_domain is %i at time %f"%(
-                # smallest_it, time)
-                # print "smallest domain is: %s"%repr(smallest_domain)
-                # axes_mappings = [
-                # sd.array_value_index_mapping(
-                # smallaxis,
-                # axis,
-                # compare_on_axes = 0
-                # )
-                # for smallaxis, axis in
-                # zip(smallest_domain, domain)
-                # ]
-                # if __debug__: print "Mapping = "+str(axes_mappings)
-
-                # Calculating difference in values of common domains
-
-                # needed for fixing domain size to smallest domain.
-                # This will cause
-                # problems when plotting.
-                # error = be.ones_like(sims[0].raw[smallest_it])
-                # for from_tup, to_tup in map_generator(axes_mappings):
-                # error[(slice(None),)+from_tup] = be.absolute(
-                # sim.raw[it][(slice(None), ) + to_tup] -
-                # sim.exact[it][(slice(None), ) + to_tup]
-                # )
-
-                error = be.absolute(sim.raw[it] - sim.exact[it])
-                if __debug__:
-                    print("Errors are: %s" % repr(error))
-                sim.write(sd.dgTypes["errorExa"], it, error)
-
-                # we assume that stepsizes is constant for each slice
-                stepsizes += [be.asarray([axis[1] - axis[0] for axis in domain])]
-                for j, p in enumerate(args.Lp):
-                    tableE[j][i] = Lp(error, stepsizes[-1], p)
-            for j, p in enumerate(args.Lp):
-                rows = _printErrorConv(
-                    tSimNames, list(range(num_of_comps)), tableE[j], stepsizes, time, p
+from builtins import range
+from builtins import object
+import abc
+from mpi4py import MPI
+import logging
+import numpy as np
+from coffee.backend import backend as be
+
+
+###############################################################################
+# Abstract Base Class for MPI Interfaces
+###############################################################################
+class MPIInterface(object, metaclass=abc.ABCMeta):
+    def __init__(self, mpi_comm, *args, **kwds):
+        """Initialisaer for MPIInterface objects.
+
+        Parameters
+        ==========
+        mpi_comm: mpi4py.Comm
+            A wrapper to an MPI_COMM object via mpi4py.
+        """
+        self.comm = mpi_comm
+        super(MPIInterface, self).__init__(*args, **kwds)
+
+    @abc.abstractmethod
+    def subdomain(self):
+        """Returns a tuple of slice objects that represents the subdomain of the full
+        grid that this MPI node should perform computations over.
+
+        Returns
+        =======
+        tuple of slices
+        """
+
+    @abc.abstractmethod
+    def communicate(self, data):
+        """Returns a list of tuples. The first element of each tuple is a slice
+        representing the portion of data which corresponds to the second
+        element of the tuple. The second element of the tuple is an array of
+        data which are the communicated values that correspond to the
+        positions described by the slice."""
+
+    def barrier(self):
+        if self.comm is None:
+            return
+        return self.comm.barrier()
+
+
+###############################################################################
+# Concrete implementations
+###############################################################################
+class EvenCart(MPIInterface):
+    def __init__(self, domain, boundary_data, *args, **kwds):
+        """Initialiser for EvenCart objects
+
+        An EvenCart object is an implementation of MPIInterface that
+        assumes that the global topology uses the MPI Cartesian methods.
+
+        Parameters
+        ==========
+        domain: numpy.ndarray
+            A numpy array representing the values of points in the global
+            computational domain
+        boundary_data: grid.ABCBoundary
+        """
+        super(EvenCart, self).__init__(*args, **kwds)
+        self.log = logging.getLogger("EvenCart")
+        self.domain = domain
+        self.domain_mapping = self._make_domain_mappings(domain, boundary_data)
+
+    def _make_domain_mappings(self, domain, boundary_data):
+        """A utility that constructs the tuples of slices that represent
+        the sub-grids for each MPI node based on that nodes rank.
+
+        The calculation assumes that each MPI node should handle roughly the
+        same load as all others and that the MPI topology is Cartesian.
+
+        Parameters
+        ==========
+        domain: numpy.ndarray
+            A numpy array representing the values of points in the global
+            computational domain
+        boundary_data: grid.ABCBoundary
+
+        Returns
+        =======
+        list of tuples of slices:
+            Each tuple of slices in index i gives the sub grid for MPI node
+            with rank i.
+
+        """
+        if self.comm is None:
+            return tuple([slice(None, None, None) for dim in domain])
+        r_map = []
+        for rank in range(self.comm.size):
+            coords = self.comm.Get_coords(rank)
+            r_map += [
+                tuple(
+                    [
+                        self._array_slice(
+                            domain[i],
+                            coord,
+                            self.comm.dims[i],
+                            boundary_data.ghost_points(i, -1),
+                            boundary_data.ghost_points(i, 1),
+                        )
+                        for i, coord in enumerate(coords)
+                    ]
                 )
-                with open(
-                    "%s-e-exa_L%f_%f.csv" % (args.ofile_base, p, time), "wb"
-                ) as file:
-                    for row in rows:
-                        file.write(row)
-
-
-def numer(args):
-    with sd.SimulationHDF(args.file) as file:
-        # Get all the current simulations
-        sims = file.getSims()
-        tSimNames = [sim.name for sim in sims[:-1]]
-        stepsizes = []
-
-        # We make the assumption that the number of components for each run
-        # is the same and that the values of the components are in the first
-        # axis of raw.shape
-        num_of_comps = sims[0].numvar
-        tableE = be.zeros((len(args.Lp), len(tSimNames), num_of_comps), dtype=float)
-
-        # Seperate them into the one with the best resolution
-        # and the others to be compared to this one.
-        # Note that the code assumes that sims is appropriately ordered
-        subtrahend = sims[-1]
-        minuends = sims[:-1]
-
-        #        # We must now check how the domains have been constructed.
-        #        # We need to tell the difference between [[i] for i in range]
-        #        # and [i for i in range].
-        #        # We make the assumption that the domain type remains the same
-        #        # throughout the simulation.
-        #        meshes = subtrahend.domain[0]
-        #        dims = len(subtrahend.domain.group['0'].attrs['shape'])
-        #        if dims is 1:
-        #            compare_on_axes = 0
-        #        else:
-        #            index = tuple([0 for i in domain.shape])
-        #            if len(be.array(domain[index]).shape) is 0 and be.array(domain[index[:-1]]).shape[0] == dims-1:
-        #                compare_on_axes = 1
-        #            elif len(be.array(domain[index])) is dims:
-        #                compare_on_axes = 0
-        #            else:
-        #                raise Exception("Unable to determine domain type")
-
-        for time in args.t:
-            print("==================================")
-            print("Doing calculation for time = %f" % time)
-
-            # Get data for the subtrahead, the index of time, the domain.
-            subtrahend_index = subtrahend.indexOfTime(time)
-            print(
-                "Subtrahend time = %f at index = %i"
-                % (subtrahend.time[subtrahend_index], subtrahend_index)
-            )
-            subtrahend_domain = subtrahend.domain[subtrahend_index]
+            ]
+        if __debug__:
+            self.log.debug("domain_mapping is %s" % r_map)
+        return r_map
+
+    def _neighbour_slices(self, shape, b_data):
+        """A utility function that collects the source and destination
+        ranks for neighbouring MPI nodes along with the slices needed
+        to describe what data should be transferred.
+
+        Parameters
+        ==========
+        shape: tuple of ints
+            The shape of the data that will be communicated to neighbouring MPI
+            nodes
+
+        b_data: grid.ABCBoundary
+
+        Returns
+        =======
+        list of tuples:
+            Each tuple has three members, first the source MPI node rank,
+            second the destination MPI node rank and third the list of tuples
+            of slices that describes the data to be communicated.
+        """
+        if self.comm is None:
+            return []
+        dims = self.comm.Get_dim()
+        pos_neighbours = [
+            b_data.source_and_dest(d, 1) + b_data.internal_slice(shape, d, 1)
+            for d in range(dims)
+        ]
+        neg_neighbours = [
+            b_data.source_and_dest(d, -1) + b_data.internal_slice(shape, d, -1)
+            for d in range(dims)
+        ]
+        neighbours = pos_neighbours + neg_neighbours
+        if __debug__:
+            self.log.debug("neighbour_slices is %s" % neighbours)
+        return neighbours
+
+    def _array_slice(
+        self, array_length, rank, num_ranks, ghost_points_start, ghost_points_end
+    ):
+        """The utility method that calculates the slices that describe the
+        sub-grid managed by the MPI node with rank ``rank``.
+
+        The method assumes that it is doing the calculation for a single
+        dimension. To build the full list of tuples of slices, all
+        dimensions will need to be iterated over.
+
+        Parameters
+        ==========
+        array_length: int
+            The number of grid points in this particular dimension of the
+            total computational domain.
+        rank: int
+            The MPI rank that the slices are computed for.
+        num_ranks: int
+            The number of MPI nodes that cover this particular dimension.
+        ghost_points_start: int
+            The number of ghost points at the start of the dimension.
+        ghost_points_end: int
+            The number of ghost points at the end of the dimension.
+
+        Returns
+        =======
+        slice:
+            A slice which gives the subdomain for the particular dimension and
+            the needed MPI node rank.
+        """
+        if __debug__:
+            self.log.debug("Calculating start and end indices for subdomain")
+            self.log.debug("Array_length is %i" % array_length)
+        # divide domain into appropriate parts
+        q, r = divmod(array_length, num_ranks)
+        if __debug__:
+            self.log.debug("q = %i, r = %i" % (q, r))
+        # use the rank to details which part is relevant for this process
+        s = rank * q + min(rank, r)
+        e = s + q
+        # Adjust e to account for min(rank, r) term, which spreads the remainder
+        # over the appropriate number of processes
+        if rank < r:
             if __debug__:
-                print("Subtrahend domain = %s" % str(subtrahend_domain))
-
-            # Need to collect the same information for each minuend and do the
-            # comparison.
-            for i, minuend in enumerate(minuends):
-                print("Calculating %s - %s" % (minuend.name, subtrahend.name))
-
-                # Finding index for correct time
-                minuend_index = minuend.indexOfTime(time)
-                print(
-                    "Minuend time = %f at index = %i"
-                    % (minuend.time[minuend_index], minuend_index)
+                self.log.debug("rank < r so we add one to end point")
+            e = e + 1
+        # add in ghost_points if we can
+        # this currently works for gp = 1 for an SAT boudnary method.
+        # The code will need to be checked for consistency if this changes.
+        if s - ghost_points_start > -1:
+            s = s - ghost_points_start
+        if e + ghost_points_end < array_length:
+            e = e + ghost_points_end
+        if __debug__:
+            self.log.debug("Start index = %i, End index = %i" % (s, e))
+        return slice(s, e, None)
+
+    @property
+    def subdomain(self):
+        """Returns the slices which give the subdomain for the MPI node
+        that this method is called on.
+
+        Returns
+        =======
+        list of tuples of slices
+        """
+        if self.comm is None:
+            return self.domain_mapping
+        return tuple(self.domain_mapping[self.comm.rank])
+
+    def communicate(self, data, b_data):
+        """Communicates the given data to appropriate neighbouring nodes.
+
+        Parameters
+        ==========
+        data: numpy.ndarray
+            An array representing the values of the computed function over
+            the sub-grid managed by the MPI node this code is being computed on.
+        b_data: grid.ABCBoundary
+
+        Returns
+        =======
+        list of tuples (list of slices, numpy.ndarray)
+            The returned data is a list of tuples. The first element of the tuple
+            describes which grid points the communicated data relates to.
+            The second element is the data received from whichever MPI node
+            manages the sub-grid which looks after the relevant grid points.
+        """
+        # if self.comm.size == 1:
+        # return []
+        nslices = self._neighbour_slices(data.shape, b_data)
+        if __debug__:
+            self.log.debug("about to perform communication")
+            self.log.debug("nslices = %s" % (repr(nslices)))
+            self.log.debug("data is %s" % repr(data))
+        r_data = []
+        for source, dest, send_slice, recv_slice in nslices:
+            if __debug__:
+                self.log.debug(
+                    "source=%d, dest=%d, send_slice=%s, recv_slice=%s"
+                    % (source, dest, repr(send_slice), repr(recv_slice))
                 )
-
-                # Comparing domains
-                minuend_domain = minuend.domain[minuend_index]
-                if __debug__:
-                    print("Minuend domain = %s" % str(minuend_domain))
-
-                #                # Get the mapping between the domains.
-                #                compare_on_axes = True
-                #                if len(minuend_domain.shape) == 1:
-                #                    compare_on_axes = False
-                #                mapping = sd.array_value_index_mapping(minuend_domain,\
-                #                    subtrahend_domain,compare_on_axes = compare_on_axes)
-                axes_mappings = [
-                    sd.array_value_index_mapping(
-                        minuend_axis, subtrahend_axis, compare_on_axes=0
-                    )
-                    for minuend_axis, subtrahend_axis in zip(
-                        minuend_domain, subtrahend_domain
-                    )
-                ]
+            if dest < 0:
+                send_data = None
+            else:
+                # I really did not want to copy this view. For large data
+                # sets this feels like an unnecessary delay.
+                # However mpi4py did not seem to work with views and using
+                # self.comm.sendrecv to send and recv arbitrary objects.
+                # Plus self.comm.Sendrecv requires contiguous data
+                # so only in rare cases is it possible to send.
+                # Hence the be.copy statement is required.
+                send_data = be.array(data[send_slice], copy=True, order="C")
+            if source < 0:
+                recv_data = None
+            else:
+                # when testing the above assertion I suggest changing this
+                # line to be.ones_like, rather than be.empty_like
+                recv_data = be.empty_like(data[recv_slice])
+            if __debug__:
+                self.log.debug("About to sendrecv")
+                self.log.debug("data to be sent is %s" % repr(send_data))
+                self.log.debug("source is %s" % source)
+                self.log.debug("dest is %s" % dest)
+                self.log.debug("recv_data is %s" % repr(recv_data))
+            self.comm.Sendrecv(send_data, dest=dest, recvbuf=recv_data, source=source)
+            if __debug__:
+                self.log.debug("Received data = %s" % repr(recv_data))
+                self.log.debug("data[0] is %s" % repr(data[0]))
+                self.log.debug("Sendrecv completed")
+            if source >= 0:
+                r_data += [(recv_slice, recv_data)]
+        if __debug__:
+            self.log.debug("r_data = %s" % repr(r_data))
+            self.log.debug("communication complete")
+        return r_data
+
+    def collect_data(self, data):
+        """A method that collects all computed function values over all
+        sub-grids managed by all MPI nodes and returns the amalgamated data
+        if the rank of this process is 0.
+
+        This gives a way to get a single copy of all computed data so far. It does,
+        however, assume that all subsequence processing occurs on a single MPI
+        node. This is a bottle neck.
+
+        Parameters
+        ==========
+        data: numpy.ndarray
+            The data to be communicated.
+
+        Returns
+        =======
+        None or numpy.ndarray
+            The collated data if MPI_Comm_Rank is 0, none otherwise.
+        """
+
+        # Note that this method does not take account of ghost_points in
+        # the domains. This does not cause a problem. It just means
+        # that more data than necessary is passed.
+
+        # If there are no partitions of the domain we don't need to collect
+        if self.comm is None:
+            return data
+        # Gather the data
+        if __debug__:
+            self.log.debug("Data is %s" % repr(data))
+        fields = self.comm.gather(data, root=0)
+        if __debug__:
+            self.log.debug("Data has been gathered.")
+        # If this process is root then collate the data and return
+        if self.comm.rank == 0:
+            if __debug__:
+                self.log.debug(
+                    "The collected fields have shapes %s"
+                    % repr([f.shape for f in fields])
+                )
+            rdata_edims_shape = (data.shape[0],) + data.shape[len(self.domain) + 1 :]
+            rdata_edims_slice = tuple(
+                [slice(None, None, None) for i in rdata_edims_shape]
+            )
+            if __debug__:
+                self.log.debug("data.shape is %s" % str(data.shape))
+                self.log.debug("rdata_shape_edims is %s" % str(rdata_edims_slice))
+                self.log.debug("rdata_edims_shape is %s" % repr(rdata_edims_shape))
+                self.log.debug("self.domain is %s" % str(self.domain))
+            rdata = be.zeros(
+                (rdata_edims_shape[0],) + self.domain + rdata_edims_shape[1:],
+                dtype=data.dtype,
+            )
+            if __debug__:
+                self.log.debug("rdata.shape = %s" % (repr(rdata.shape)))
+            for rank, field in enumerate(fields):
+                dslice = self.domain_mapping[rank]
                 if __debug__:
-                    print("Mapping = " + str(axes_mappings))
-
-                for dgType in args.dg:
-                    print("Calculating error for dgType %s" % dgType)
-
-                    # Collecting dgType data
-                    subtrahend_dg = getattr(subtrahend, dgType)
-                    minuend_dg = getattr(minuend, dgType)
-
-                    # Calculating difference in values of common domains
-                    # diff = be.ones_like(minuend_dg[minuend_index])
-                    diff = be.ones(
-                        (minuend_dg[minuend_index].shape[0], len(axes_mappings[0]))
-                    )
-                    # import pdb; pdb.set_trace()
-                    for index, from_tup, to_tup in map_generator(axes_mappings):
-                        diff[:, index] = (
-                            minuend_dg[minuend_index][(slice(None),) + from_tup]
-                            - subtrahend_dg[subtrahend_index][(slice(None),) + to_tup]
+                    self.log.debug("dslice is %s" % repr(dslice))
+                    self.log.debug("rdata_edims_slice is %s" % repr(rdata_edims_slice))
+                    self.log.debug("rdata.shape is %s" % repr(rdata.shape))
+                    self.log.debug("field.shape is %s" % repr(field.shape))
+                    self.log.debug(
+                        "rdata[(rdata_edims_slice[0],) + dslice].shape is + \
+                        rdata_edims_slice[1:] = %s"
+                        % (
+                            repr(
+                                rdata[
+                                    (rdata_edims_slice[0],)
+                                    + dslice
+                                    + rdata_edims_slice[1:]
+                                ].shape
+                            )
                         )
-
-                    # Storing data
-                    minuend.write(
-                        sd.dgTypes["errorNum"],
-                        minuend_index,
-                        be.absolute(diff),  # derivedAttrs = {sd.dgTypes['time']:time})
-                        # name=sd.dgTypes[dgType]
                     )
-
-                    # we assume that dx is constant for each slice
-                    stepsizes += [
-                        be.asarray([axis[1] - axis[0] for axis in minuend_domain])
-                    ]
-                    for j, p in enumerate(args.Lp):
-                        tableE[j][i] = Lp(diff, stepsizes, p)
-                # end loop over args.dg
-            for j, p in enumerate(args.Lp):
-                rows = _printErrorConv(
-                    tSimNames, list(range(num_of_comps)), tableE[j], stepsizes, time, p
-                )
-                with open(
-                    "%s-e-num_L%f_%f.csv" % (args.ofile_base, p, time), "wb"
-                ) as file:
-                    for row in rows:
-                        file.write(row)
-
-
-def map_generator(array, i=0):
-    data = array[i]
-    index = 0
-    for datum in data:
-        from_res = (datum[0][0],)
-        to_res = (datum[1][0],)
-        if i == len(array) - 1:
-            yield index, from_res, to_res
-            index += 1
+                rdata[(rdata_edims_slice[0],) + dslice + rdata_edims_slice[1:]] = field
+            return rdata
         else:
-            for res in map_generator(array, i + 1):
-                yield index, from_res + res[0], to_res + res[1]
-                index += 1
-
-
-################################################################################
-# Routines for numerical error estimation and output
-################################################################################
-
-# returns descrete version of lp norms
-
-
-def Lp(errors, stepsizes, p):
-    errors = be.absolute(errors)
-    if p == float("infinity"):
-        rerrors = be.max(errors)
-    else:
-        rerrors = be.power(
-            be.squeeze(
-                be.apply_over_axes(
-                    be.sum, be.power(errors, p), list(range(1, len(errors.shape)))
-                )
-            ),
-            1 / p,
-        )
-    return rerrors
-
-
-# helper method to print error conv data
-def _printErrorConv(Sims, Indices, errorData, stepSizes, time, p):
-    rString = []
-    firC = 10
-    secC = 10
-    thiC = 10
-    print("")
-    head1 = "{0:24} {1}".format("Simulation at t = %.4f" % time, "Error data")
-    head2 = "{0:24} ".format("")
-    head3 = head2
-    head4 = ""
-    for i in Indices:
-        head2 = head2 + "{0:^26} ".format("Component %i" % i)
-    for i in Indices:
-        head3 = head3 + "{0:15}  {1:10}".format("log(L_%.4f,2)" % p, "Conv R")
-    print(head1)
-    rString += [head1 + "\n"]
-    print(head2)
-    rString += [head2 + "\n"]
-    print(head3)
-    rString += [head3 + "\n"]
-    print(head4)
-    rString += [head4 + "\n"]
-    for i, simName in enumerate(Sims):
-        s = "{0:24} ".format(stepSizes[i])
-        for j, comp in enumerate(Indices):
-            if not i == 0:
-                s = s + "{0:<15.6f}  {1:<10.4f}".format(
-                    be.log2(errorData[i][j]),
-                    _conv(
-                        errorData[i - 1][j],
-                        stepSizes[i - 1],
-                        errorData[i][j],
-                        stepSizes[i],
-                    )[0],
-                )
-            else:
-                s = s + "{0:<15.6f}  {1:10}".format(be.log2(errorData[i][j]), "")
-        print(s)
-        rString += [s + "\n"]
-    return rString
-
-
-def _conv(old, numSteps1, new, numSteps2):
-    return be.log(old / new) / be.log(numSteps1 / numSteps2)
-
-
-################################################################################
-# Main parser
-################################################################################
-parser = argparse.ArgumentParser(
-    description="""This program calculates the error for a particular data type based on comparison to the highest resolution simulation or to exact data. The highest resolution is selected as the simulation with the highest cmp parameter. See simulation_hdf.py for the use of cmp."""
-)
-
-subparsers = parser.add_subparsers(
-    title="Subcommands",
-    description="""The subcommands
-allow for selection of numerical or exact calculation of error.""",
-    help="""For more information on any of the subcommands please use 'error <subcommand> -h""",
-)
-
-
-parser.add_argument(
-    "file",
-    help="""The hdf file, produced by simulation_data.py that contains the data to be
-analysed""",
-)
-parser.add_argument(
-    "-t",
-    "-time",
-    type=float,
-    metavar="TIME",
-    action="append",
-    required=True,
-    help="""A time at which the error analysis should be run. Multiple times can be given""",
-)
-parser.add_argument(
-    "-dg",
-    "-dgtype",
-    action="append",
-    help="""A data group to be analysed. See simulation_data for information on
-the different data groups. Defaults to "raw". Multiple data groups can be given.""",
-)
-parser.add_argument(
-    "-Lp",
-    metavar="P",
-    action="append",
-    help="""The p value of the norm to be used to calculate the error. The infinity
-norm can be entered by using -Lp "inf".""",
-)
-parser.add_argument(
-    "-O",
-    default=False,
-    action="store_true",
-    help="""If set debugging information will be printed.""",
-)
-
-################################################################################
-# Exact subcommand
-################################################################################
-parser_exact = subparsers.add_parser(
-    "exact", help="""This command calculates error using exact data."""
-)
-parser_exact.set_defaults(func=exact)
-
-################################################################################
-# Exact subcommand
-################################################################################
-parser_numer = subparsers.add_parser(
-    "numer",
-    help="""This command calculates error using the highest resolution, as determined by cmp,
-numerical data.""",
-)
-parser_numer.set_defaults(func=numer)
-
-
-args = parser.parse_args()
-if args.dg is None:
-    args.dg = ["raw"]
-print("Starting computation...")
-if args.Lp is None:
-    args.Lp = ["2"]
-for i in range(len(args.Lp)):
-    args.Lp[i] = float(args.Lp[i])
-args.ofile_base, sep, exten = args.file.rpartition(".")
-args.func(args)
-print("...computation complete.-")
+            return None
```

### Comparing `coffeegrinder-0.2.5/setup.cfg` & `coffeegrinder-0.2.6/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = coffeegrinder
-description = Add a short description here!
+description = COFFEE is an MPI-Parallelised Python package for the numerical evolution of time-dependent differential equations.
 author = Chris Stevens
 author_email = chris.stevens@canterbury.ac.nz
 license = MIT
 license_files = LICENSE.txt
 long_description = file: README.rst
 long_description_content_type = text/x-rst; charset=UTF-8
 url = https://github.com/coffee-gr/coffee
@@ -19,20 +19,20 @@
 zip_safe = False
 packages = find_namespace:
 include_package_data = True
 package_dir = 
 	=src
 install_requires = 
 	importlib-metadata; python_version<"3.8"
-	future
 	numpy
 	h5py
 	scipy
 	PyGnuplot
 	matplotlib
+	mpi4py
 
 [options.packages.find]
 where = src
 exclude = 
 	tests
 
 [options.extras_require]
```

### Comparing `coffeegrinder-0.2.5/setup.py` & `coffeegrinder-0.2.6/setup.py`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.2.5/src/coffee/__init__.py` & `coffeegrinder-0.2.6/src/coffee/__init__.py`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.2.5/src/coffee/actions/actions.py` & `coffeegrinder-0.2.6/src/coffee/actions/actions.py`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.2.5/src/coffee/actions/gp_plotter.py` & `coffeegrinder-0.2.6/src/coffee/actions/gp_plotter.py`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.2.5/src/coffee/actions/hdf_output.py` & `coffeegrinder-0.2.6/src/coffee/actions/hdf_output.py`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.2.5/src/coffee/actions/mpl_plotter.py` & `coffeegrinder-0.2.6/src/coffee/actions/mpl_plotter.py`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.2.5/src/coffee/backend/backend.py` & `coffeegrinder-0.2.6/src/coffee/backend/backend.py`

 * *Files 0% similar despite different names*

```diff
@@ -175,15 +175,15 @@
 # ################################################################################
 # # NumPy implementation
 # ################################################################################
 
 
 class NumpyBackend(BackendBase):
     def __init__(self):
-        print("Initialising Numpy Backend")
+        # print("Initialising Numpy Backend")
         try:
             import numpy as np
         except ImportError:
             raise ImportError(
                 "NumPy library is not installed. Please install NumPy to use this function."
             )
```

### Comparing `coffeegrinder-0.2.5/src/coffee/diffop/fd.py` & `coffeegrinder-0.2.6/src/coffee/diffop/fd.py`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.2.5/src/coffee/diffop/sbp/dissipation.py` & `coffeegrinder-0.2.6/src/coffee/diffop/sbp/dissipation.py`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.2.5/src/coffee/diffop/sbp/dissipation_testing.nb` & `coffeegrinder-0.2.6/src/coffee/diffop/sbp/dissipation_testing.nb`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.2.5/src/coffee/diffop/sbp/sbp.py` & `coffeegrinder-0.2.6/src/coffee/diffop/sbp/sbp.py`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.2.5/src/coffee/free_data.py` & `coffeegrinder-0.2.6/src/coffee/free_data.py`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.2.5/src/coffee/grid/grid.py` & `coffeegrinder-0.2.6/src/coffee/grid/grid.py`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.2.5/src/coffee/ibvp.py` & `coffeegrinder-0.2.6/src/coffee/ibvp.py`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.2.5/src/coffee/io/simulation_data.py` & `coffeegrinder-0.2.6/src/coffee/io/simulation_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,24 +10,19 @@
 documentation if the dgTypes dictionary needs to be altered.
 """
 
 from builtins import zip
 from builtins import map
 from builtins import str
 from builtins import range
-from past.utils import old_div
 from builtins import object
 import functools
 import h5py
 import numpy as np
-import time
-import sys
-import logging
-import math
-import importlib
+from coffee.backend import backend as be
 
 # Gnuplot currently only works with Python 2!
 try:
     import Gnuplot
 except ImportError:
     pass
 
@@ -608,15 +603,15 @@
         # Get x values
         domains = self.getDgType("domain")
 
         # Get all times
         times = self.getDgType("time")
         times.rV = True
         numOfFrames = len(times)
-        frameSkip = int(old_div(numOfFrames, (animationLength * framesPerSec)))
+        frameSkip = int(numOfFrames / (animationLength * framesPerSec))
 
         # Get data for scri
         scrif = self.getDgType("scrif")
         scrif.rV = True
 
         # Initialize gnuplot
         gnu = Gnuplot.Gnuplot(**gnuInitialisationCommands)
@@ -824,36 +819,36 @@
             else:
                 return -1
 
         # Check initial step
         time_dg = times_dg[indices[0]]
         if indices[1] - indices[0] == 1:
             dt = times_dg[indices[1]][()] - time_dg[()]
-            if t <= time_dg[()] < t + old_div(dt, 2):
+            if t <= time_dg[()] < t + (dt / 2.):
                 return indices[0]
         else:
             if abs(time_dg[(0)] - t) <= NUMERICAL_TOLERANCE:
                 return indices[0]
 
         # Check all other steps except final
         for i in range(1, len(indices) - 1):
             time_dg = times_dg[indices[i]]
             if indices[i + 1] - indices[i] == 1:
                 dt = times_dg[indices[i + 1]][()] - time_dg[()]
-                if t - old_div(dt, 2) <= time_dg[()] < t + old_div(dt, 2):
+                if t - (dt / 2.) <= time_dg[()] < t + (dt / 2.):
                     return indices[i]
             else:
                 if abs(time_dg[(0)] - t) <= NUMERICAL_TOLERANCE:
                     return indices[i]
 
         i = len(indices) - 1
         time_dg = times_dg[indices[i]]
         if indices[i] - indices[i - 1] == 1:
             dt = time_dg[()] - times_dg[indices[i - 1]]
-            if t - old_div(dt, 2) <= time_dg[()] <= t:
+            if t - (dt / 2.) <= time_dg[()] <= t:
                 return indices[i]
         else:
             if abs(time_dg[(0)] - t) <= NUMERICAL_TOLERANCE:
                 return indices[i]
         return -1
 
     def write(
```

### Comparing `coffeegrinder-0.2.5/src/coffee/solvers/solvers.py` & `coffeegrinder-0.2.6/src/coffee/solvers/solvers.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 default implementations.
 
 This default implementations all assume that tslice.TimeSlice objects can be
 operated on by numerically (e.g. addition, multiplication, subtraction).
 """
 
 
-from past.utils import old_div
 from builtins import object
 import math
 import logging
 import abc
 
 from coffee.tslices import tslices
 
@@ -159,15 +158,15 @@
             dg = dg.data
 
             # NR is applied to f
             f = prev_u_next - u_start - dt * g
             df = 1.0 - dt * dg
 
             # Compute next value of u_next
-            next_u_next = prev_u_next - old_div(f, df)
+            next_u_next = prev_u_next - (f / df)
 
             # If we get to within a certain accuracy of the root stop
             if all(abs(next_u_next - prev_u_next)[0] < TOL):
                 break
 
             # Otherwise continue
             prev_u_next = next_u_next
```

### Comparing `coffeegrinder-0.2.5/src/coffee/system.py` & `coffeegrinder-0.2.6/src/coffee/system.py`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.2.5/src/coffee/tslices/tslices.py` & `coffeegrinder-0.2.6/src/coffee/tslices/tslices.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,14 @@
 that you can restart a simulation if given a timeslice, system and solver.
 """
 
 from builtins import object
 import abc
 import logging
 import numpy as np
-from future.utils import with_metaclass
 from coffee.backend import backend as be
 
 
 ###############################################################################
 # TimeSlice Abstract Base Class
 ##############################################################################
 class ABCTimeSlice(object, metaclass=abc.ABCMeta):
```

### Comparing `coffeegrinder-0.2.5/src/coffeegrinder.egg-info/PKG-INFO` & `coffeegrinder-0.2.6/src/coffeegrinder.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: coffeegrinder
-Version: 0.2.5
-Summary: Add a short description here!
+Version: 0.2.6
+Summary: COFFEE is an MPI-Parallelised Python package for the numerical evolution of time-dependent differential equations.
 Home-page: https://github.com/coffee-gr/coffee
 Author: Chris Stevens
 Author-email: chris.stevens@canterbury.ac.nz
 License: MIT
 Project-URL: Documentation, https://pyscaffold.org/
 Platform: any
 Classifier: Development Status :: 4 - Beta
@@ -48,27 +48,23 @@
 
 
 ======
 coffee
 ======
 
 
-    Add a short description here!
+    COFFEE is an MPI-Parallelised Python package for the numerical evolution of time-dependent differential equations.
 
 
 Installation
 ------------
 
 To use this software, you will need the following dependencies:
 
-- fitsio C library
-- chealpix C library
-- mpich or Open MPI
-- pyFFTW
-- gnuplot + appropriate terminal if needed
+- 
 - HDF library
 
 Please make sure these dependencies are installed before using this software.
 
 .. rubric:: Getting started
 
 One needs to point the ``PYTHONPATH`` environment variable to the packages directory. Then the system code can be run with::
```

### Comparing `coffeegrinder-0.2.5/tests/test_actions.py` & `coffeegrinder-0.2.6/tests/test_actions.py`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.2.5/tests/test_backend.py` & `coffeegrinder-0.2.6/tests/test_backend.py`

 * *Files identical despite different names*

### Comparing `coffeegrinder-0.2.5/tox.ini` & `coffeegrinder-0.2.6/tox.ini`

 * *Files identical despite different names*

