# Comparing `tmp/sn-nacl-0.3.tar.gz` & `tmp/sn-nacl-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sn-nacl-0.3.tar", last modified: Wed Nov  9 10:26:10 2022, max compression
+gzip compressed data, was "sn-nacl-0.4.tar", last modified: Sun Jul  2 10:04:25 2023, max compression
```

## Comparing `sn-nacl-0.3.tar` & `sn-nacl-0.4.tar`

### file list

```diff
@@ -1,54 +1,78 @@
-drwxrwxr-x   0 nrl       (1000) nrl       (1000)        0 2022-11-09 10:26:10.369440 sn-nacl-0.3/
--rw-rw-r--   0 nrl       (1000) nrl       (1000)      267 2022-11-09 10:26:10.369440 sn-nacl-0.3/PKG-INFO
--rw-rw-r--   0 nrl       (1000) nrl       (1000)     2745 2022-11-09 09:07:34.000000 sn-nacl-0.3/README.md
-drwxrwxr-x   0 nrl       (1000) nrl       (1000)        0 2022-11-09 10:26:10.365440 sn-nacl-0.3/nacl/
--rw-rw-r--   0 nrl       (1000) nrl       (1000)        0 2022-11-09 09:07:34.000000 sn-nacl-0.3/nacl/__init__.py
--rw-rw-r--   0 nrl       (1000) nrl       (1000)    12868 2022-11-09 09:07:34.000000 sn-nacl-0.3/nacl/dataset.py
--rw-rw-r--   0 nrl       (1000) nrl       (1000)     6742 2022-11-09 09:07:34.000000 sn-nacl-0.3/nacl/distance.py
--rw-rw-r--   0 nrl       (1000) nrl       (1000)    18720 2022-11-09 09:07:34.000000 sn-nacl-0.3/nacl/fit.py
--rw-rw-r--   0 nrl       (1000) nrl       (1000)     8760 2022-11-09 09:07:34.000000 sn-nacl-0.3/nacl/instruments.py
-drwxrwxr-x   0 nrl       (1000) nrl       (1000)        0 2022-11-09 10:26:10.365440 sn-nacl-0.3/nacl/lib/
--rw-rw-r--   0 nrl       (1000) nrl       (1000)        0 2022-11-09 09:07:34.000000 sn-nacl-0.3/nacl/lib/__init__.py
--rw-rw-r--   0 nrl       (1000) nrl       (1000)    31634 2022-11-09 09:07:34.000000 sn-nacl-0.3/nacl/lib/atmosphericmodel.py
--rw-rw-r--   0 nrl       (1000) nrl       (1000)    47811 2022-11-09 09:07:34.000000 sn-nacl-0.3/nacl/lib/bspline.py
--rw-rw-r--   0 nrl       (1000) nrl       (1000)     2917 2022-11-09 09:07:34.000000 sn-nacl-0.3/nacl/lib/constants.py
--rw-rw-r--   0 nrl       (1000) nrl       (1000)     3903 2022-11-09 09:07:34.000000 sn-nacl-0.3/nacl/lib/dataproxy.py
--rw-rw-r--   0 nrl       (1000) nrl       (1000)     9436 2022-11-09 09:07:34.000000 sn-nacl-0.3/nacl/lib/fitparameters.py
--rw-rw-r--   0 nrl       (1000) nrl       (1000)     1111 2022-11-09 09:07:34.000000 sn-nacl-0.3/nacl/lib/indextools.py
--rw-rw-r--   0 nrl       (1000) nrl       (1000)    36695 2022-11-09 09:07:34.000000 sn-nacl-0.3/nacl/lib/instruments.py
--rw-rw-r--   0 nrl       (1000) nrl       (1000)    11459 2022-11-09 09:07:34.000000 sn-nacl-0.3/nacl/lib/interpolation.py
--rw-rw-r--   0 nrl       (1000) nrl       (1000)     3662 2022-11-09 09:07:34.000000 sn-nacl-0.3/nacl/lib/optim.py
--rw-rw-r--   0 nrl       (1000) nrl       (1000)    20070 2022-11-09 09:07:34.000000 sn-nacl-0.3/nacl/lib/robuststat.py
--rw-rw-r--   0 nrl       (1000) nrl       (1000)    36881 2022-11-09 09:07:34.000000 sn-nacl-0.3/nacl/lib/spectrum.py
--rw-rw-r--   0 nrl       (1000) nrl       (1000)    24834 2022-11-09 09:07:34.000000 sn-nacl-0.3/nacl/lib/stellarlibs.py
--rw-rw-r--   0 nrl       (1000) nrl       (1000)     7552 2022-11-09 09:07:34.000000 sn-nacl-0.3/nacl/lib/utils.c
--rw-rw-r--   0 nrl       (1000) nrl       (1000)    41626 2022-11-09 09:07:34.000000 sn-nacl-0.3/nacl/minimizers.py
-drwxrwxr-x   0 nrl       (1000) nrl       (1000)        0 2022-11-09 10:26:10.365440 sn-nacl-0.3/nacl/models/
--rw-rw-r--   0 nrl       (1000) nrl       (1000)    14293 2022-11-09 09:07:34.000000 sn-nacl-0.3/nacl/models/constraints.py
--rw-rw-r--   0 nrl       (1000) nrl       (1000)    12673 2022-11-09 09:07:34.000000 sn-nacl-0.3/nacl/models/regularizations.py
--rw-rw-r--   0 nrl       (1000) nrl       (1000)    54055 2022-11-09 09:07:34.000000 sn-nacl-0.3/nacl/models/salt.py
--rw-rw-r--   0 nrl       (1000) nrl       (1000)    17177 2022-11-09 09:07:34.000000 sn-nacl-0.3/nacl/models/variancemodels.py
-drwxrwxr-x   0 nrl       (1000) nrl       (1000)        0 2022-11-09 10:26:10.369440 sn-nacl-0.3/nacl/plotting/
--rw-rw-r--   0 nrl       (1000) nrl       (1000)    99529 2022-11-09 09:07:34.000000 sn-nacl-0.3/nacl/plotting/plots.py
--rw-rw-r--   0 nrl       (1000) nrl       (1000)    18480 2022-11-09 09:07:34.000000 sn-nacl-0.3/nacl/plotting/plottools.py
-drwxrwxr-x   0 nrl       (1000) nrl       (1000)        0 2022-11-09 10:26:10.369440 sn-nacl-0.3/nacl/simulations/
--rw-rw-r--   0 nrl       (1000) nrl       (1000)    32296 2022-11-09 09:07:34.000000 sn-nacl-0.3/nacl/simulations/etc.py
--rw-rw-r--   0 nrl       (1000) nrl       (1000)    21446 2022-11-09 09:07:34.000000 sn-nacl-0.3/nacl/simulations/flux_simulator.py
--rw-rw-r--   0 nrl       (1000) nrl       (1000)    17420 2022-11-09 09:14:25.000000 sn-nacl-0.3/nacl/simulations/ideal.py
--rw-rw-r--   0 nrl       (1000) nrl       (1000)     9554 2022-11-09 09:07:34.000000 sn-nacl-0.3/nacl/simulations/jla.py
--rw-rw-r--   0 nrl       (1000) nrl       (1000)     9953 2022-11-09 09:07:34.000000 sn-nacl-0.3/nacl/simulations/k21.py
--rw-rw-r--   0 nrl       (1000) nrl       (1000)      688 2022-11-09 09:07:34.000000 sn-nacl-0.3/nacl/simulations/reindex.py
-drwxrwxr-x   0 nrl       (1000) nrl       (1000)        0 2022-11-09 10:26:10.369440 sn-nacl-0.3/nacl/util/
--rw-rw-r--   0 nrl       (1000) nrl       (1000)    45527 2022-11-09 09:07:34.000000 sn-nacl-0.3/nacl/util/io.py
--rw-rw-r--   0 nrl       (1000) nrl       (1000)    17260 2022-11-09 09:07:34.000000 sn-nacl-0.3/nacl/util/salt2.py
--rw-rw-r--   0 nrl       (1000) nrl       (1000)     1796 2022-11-09 09:07:34.000000 sn-nacl-0.3/nacl/util/saltpath.py
--rw-rw-r--   0 nrl       (1000) nrl       (1000)       98 2022-11-09 09:07:34.000000 sn-nacl-0.3/pyproject.toml
--rw-rw-r--   0 nrl       (1000) nrl       (1000)       38 2022-11-09 10:26:10.369440 sn-nacl-0.3/setup.cfg
--rw-rw-r--   0 nrl       (1000) nrl       (1000)      876 2022-11-09 10:25:42.000000 sn-nacl-0.3/setup.py
-drwxrwxr-x   0 nrl       (1000) nrl       (1000)        0 2022-11-09 10:26:10.369440 sn-nacl-0.3/sn_nacl.egg-info/
--rw-rw-r--   0 nrl       (1000) nrl       (1000)      267 2022-11-09 10:26:10.000000 sn-nacl-0.3/sn_nacl.egg-info/PKG-INFO
--rw-rw-r--   0 nrl       (1000) nrl       (1000)     1010 2022-11-09 10:26:10.000000 sn-nacl-0.3/sn_nacl.egg-info/SOURCES.txt
--rw-rw-r--   0 nrl       (1000) nrl       (1000)        1 2022-11-09 10:26:10.000000 sn-nacl-0.3/sn_nacl.egg-info/dependency_links.txt
--rw-rw-r--   0 nrl       (1000) nrl       (1000)        1 2022-11-09 10:01:00.000000 sn-nacl-0.3/sn_nacl.egg-info/not-zip-safe
--rw-rw-r--   0 nrl       (1000) nrl       (1000)       61 2022-11-09 10:26:10.000000 sn-nacl-0.3/sn_nacl.egg-info/requires.txt
--rw-rw-r--   0 nrl       (1000) nrl       (1000)        5 2022-11-09 10:26:10.000000 sn-nacl-0.3/sn_nacl.egg-info/top_level.txt
+drwxrwxr-x   0 nrl       (1000) nrl       (1000)        0 2023-07-02 10:04:25.078516 sn-nacl-0.4/
+-rw-rw-r--   0 nrl       (1000) nrl       (1000)      267 2023-07-02 10:04:25.078516 sn-nacl-0.4/PKG-INFO
+-rw-rw-r--   0 nrl       (1000) nrl       (1000)     4956 2023-06-30 07:57:19.000000 sn-nacl-0.4/README.md
+drwxrwxr-x   0 nrl       (1000) nrl       (1000)        0 2023-07-02 10:04:25.074516 sn-nacl-0.4/nacl/
+-rw-rw-r--   0 nrl       (1000) nrl       (1000)        0 2023-02-10 14:06:32.000000 sn-nacl-0.4/nacl/__init__.py
+-rw-rw-r--   0 nrl       (1000) nrl       (1000)     4320 2023-02-20 13:02:07.000000 sn-nacl-0.4/nacl/data_cuts.py
+-rw-rw-r--   0 nrl       (1000) nrl       (1000)    66678 2023-06-29 10:01:13.000000 sn-nacl-0.4/nacl/dataset.py
+-rw-rw-r--   0 nrl       (1000) nrl       (1000)     6742 2023-02-10 14:06:32.000000 sn-nacl-0.4/nacl/distance.py
+-rw-rw-r--   0 nrl       (1000) nrl       (1000)    20562 2023-06-20 06:24:36.000000 sn-nacl-0.4/nacl/fit.py
+-rw-rw-r--   0 nrl       (1000) nrl       (1000)     6500 2023-02-13 08:29:17.000000 sn-nacl-0.4/nacl/handles.py
+-rw-rw-r--   0 nrl       (1000) nrl       (1000)     8726 2023-06-12 12:45:14.000000 sn-nacl-0.4/nacl/instruments.py
+drwxrwxr-x   0 nrl       (1000) nrl       (1000)        0 2023-07-02 10:04:25.074516 sn-nacl-0.4/nacl/lib/
+-rw-rw-r--   0 nrl       (1000) nrl       (1000)        0 2023-02-10 14:06:32.000000 sn-nacl-0.4/nacl/lib/__init__.py
+-rw-rw-r--   0 nrl       (1000) nrl       (1000)    31634 2023-02-10 14:06:32.000000 sn-nacl-0.4/nacl/lib/atmosphericmodel.py
+-rw-rw-r--   0 nrl       (1000) nrl       (1000)    47821 2023-04-18 21:47:17.000000 sn-nacl-0.4/nacl/lib/bspline.py
+-rw-rw-r--   0 nrl       (1000) nrl       (1000)     2917 2023-02-10 14:06:32.000000 sn-nacl-0.4/nacl/lib/constants.py
+-rw-rw-r--   0 nrl       (1000) nrl       (1000)     4079 2023-02-17 16:01:06.000000 sn-nacl-0.4/nacl/lib/dataproxy.py
+-rw-rw-r--   0 nrl       (1000) nrl       (1000)     9436 2023-02-10 14:06:32.000000 sn-nacl-0.4/nacl/lib/fitparameters.py
+-rw-rw-r--   0 nrl       (1000) nrl       (1000)     1111 2023-02-10 14:06:32.000000 sn-nacl-0.4/nacl/lib/indextools.py
+-rw-rw-r--   0 nrl       (1000) nrl       (1000)    36695 2023-02-10 14:06:32.000000 sn-nacl-0.4/nacl/lib/instruments.py
+-rw-rw-r--   0 nrl       (1000) nrl       (1000)    11459 2023-02-10 14:06:32.000000 sn-nacl-0.4/nacl/lib/interpolation.py
+-rw-rw-r--   0 nrl       (1000) nrl       (1000)     3662 2023-02-10 14:06:32.000000 sn-nacl-0.4/nacl/lib/optim.py
+-rw-rw-r--   0 nrl       (1000) nrl       (1000)    20070 2023-02-10 14:06:32.000000 sn-nacl-0.4/nacl/lib/robuststat.py
+-rw-rw-r--   0 nrl       (1000) nrl       (1000)    36881 2023-02-10 14:06:32.000000 sn-nacl-0.4/nacl/lib/spectrum.py
+-rw-rw-r--   0 nrl       (1000) nrl       (1000)    24322 2023-06-12 12:39:11.000000 sn-nacl-0.4/nacl/lib/stellarlibs.py
+-rw-rw-r--   0 nrl       (1000) nrl       (1000)     7552 2023-02-10 14:06:32.000000 sn-nacl-0.4/nacl/lib/utils.c
+-rw-rw-r--   0 nrl       (1000) nrl       (1000)    19584 2023-06-30 14:57:10.000000 sn-nacl-0.4/nacl/minimize.py
+-rw-rw-r--   0 nrl       (1000) nrl       (1000)    41741 2023-05-26 07:48:01.000000 sn-nacl-0.4/nacl/minimizers.py
+drwxrwxr-x   0 nrl       (1000) nrl       (1000)        0 2023-07-02 10:04:25.074516 sn-nacl-0.4/nacl/models/
+-rw-rw-r--   0 nrl       (1000) nrl       (1000)    25263 2023-06-22 09:16:47.000000 sn-nacl-0.4/nacl/models/constraints.py
+-rw-rw-r--   0 nrl       (1000) nrl       (1000)    16025 2023-06-04 16:46:18.000000 sn-nacl-0.4/nacl/models/regularizations.py
+-rw-rw-r--   0 nrl       (1000) nrl       (1000)    77363 2023-06-30 14:57:55.000000 sn-nacl-0.4/nacl/models/salt.py
+-rw-rw-r--   0 nrl       (1000) nrl       (1000)    23780 2023-06-22 12:17:01.000000 sn-nacl-0.4/nacl/models/variancemodels.py
+drwxrwxr-x   0 nrl       (1000) nrl       (1000)        0 2023-07-02 10:04:25.074516 sn-nacl-0.4/nacl/plotting/
+-rw-rw-r--   0 nrl       (1000) nrl       (1000)        0 2023-02-13 08:21:48.000000 sn-nacl-0.4/nacl/plotting/__init__.py
+-rw-rw-r--   0 nrl       (1000) nrl       (1000)    99529 2023-02-10 14:06:32.000000 sn-nacl-0.4/nacl/plotting/plots.py
+-rw-rw-r--   0 nrl       (1000) nrl       (1000)    18480 2023-02-10 14:06:32.000000 sn-nacl-0.4/nacl/plotting/plottools.py
+drwxrwxr-x   0 nrl       (1000) nrl       (1000)        0 2023-07-02 10:04:25.078516 sn-nacl-0.4/nacl/simulations/
+-rw-rw-r--   0 nrl       (1000) nrl       (1000)      456 2023-02-13 08:21:48.000000 sn-nacl-0.4/nacl/simulations/__init__.py
+-rw-rw-r--   0 nrl       (1000) nrl       (1000)    32288 2023-02-17 12:35:25.000000 sn-nacl-0.4/nacl/simulations/etc.py
+-rw-rw-r--   0 nrl       (1000) nrl       (1000)    13802 2023-06-06 13:33:19.000000 sn-nacl-0.4/nacl/simulations/flux_simulator.py
+-rw-rw-r--   0 nrl       (1000) nrl       (1000)    17696 2023-02-10 14:06:32.000000 sn-nacl-0.4/nacl/simulations/ideal.py
+-rw-rw-r--   0 nrl       (1000) nrl       (1000)     7676 2023-06-21 13:59:42.000000 sn-nacl-0.4/nacl/simulations/jla.py
+-rw-rw-r--   0 nrl       (1000) nrl       (1000)    10496 2023-02-23 16:59:02.000000 sn-nacl-0.4/nacl/simulations/k21.py
+-rw-rw-r--   0 nrl       (1000) nrl       (1000)     1181 2023-02-13 08:21:48.000000 sn-nacl-0.4/nacl/simulations/randutils.py
+-rw-rw-r--   0 nrl       (1000) nrl       (1000)      688 2023-02-10 14:06:32.000000 sn-nacl-0.4/nacl/simulations/reindex.py
+drwxrwxr-x   0 nrl       (1000) nrl       (1000)        0 2023-07-02 10:04:25.078516 sn-nacl-0.4/nacl/util/
+-rw-rw-r--   0 nrl       (1000) nrl       (1000)    45527 2023-02-10 14:06:32.000000 sn-nacl-0.4/nacl/util/io.py
+-rw-rw-r--   0 nrl       (1000) nrl       (1000)    17260 2023-02-10 14:06:32.000000 sn-nacl-0.4/nacl/util/salt2.py
+-rw-rw-r--   0 nrl       (1000) nrl       (1000)     1796 2023-02-10 14:06:32.000000 sn-nacl-0.4/nacl/util/saltpath.py
+-rw-rw-r--   0 nrl       (1000) nrl       (1000)       98 2023-02-10 14:06:32.000000 sn-nacl-0.4/pyproject.toml
+-rw-rw-r--   0 nrl       (1000) nrl       (1000)       38 2023-07-02 10:04:25.078516 sn-nacl-0.4/setup.cfg
+-rw-rw-r--   0 nrl       (1000) nrl       (1000)      880 2023-07-02 09:51:55.000000 sn-nacl-0.4/setup.py
+drwxrwxr-x   0 nrl       (1000) nrl       (1000)        0 2023-07-02 10:04:25.078516 sn-nacl-0.4/sn_nacl.egg-info/
+-rw-rw-r--   0 nrl       (1000) nrl       (1000)      267 2023-07-02 10:04:25.000000 sn-nacl-0.4/sn_nacl.egg-info/PKG-INFO
+-rw-rw-r--   0 nrl       (1000) nrl       (1000)     1693 2023-07-02 10:04:25.000000 sn-nacl-0.4/sn_nacl.egg-info/SOURCES.txt
+-rw-rw-r--   0 nrl       (1000) nrl       (1000)        1 2023-07-02 10:04:25.000000 sn-nacl-0.4/sn_nacl.egg-info/dependency_links.txt
+-rw-rw-r--   0 nrl       (1000) nrl       (1000)        1 2023-06-29 20:14:39.000000 sn-nacl-0.4/sn_nacl.egg-info/not-zip-safe
+-rw-rw-r--   0 nrl       (1000) nrl       (1000)       68 2023-07-02 10:04:25.000000 sn-nacl-0.4/sn_nacl.egg-info/requires.txt
+-rw-rw-r--   0 nrl       (1000) nrl       (1000)        5 2023-07-02 10:04:25.000000 sn-nacl-0.4/sn_nacl.egg-info/top_level.txt
+drwxrwxr-x   0 nrl       (1000) nrl       (1000)        0 2023-07-02 10:04:25.078516 sn-nacl-0.4/tests/
+-rw-rw-r--   0 nrl       (1000) nrl       (1000)      677 2023-06-15 07:45:22.000000 sn-nacl-0.4/tests/test_constraints.py
+-rw-rw-r--   0 nrl       (1000) nrl       (1000)     6529 2023-06-28 15:19:27.000000 sn-nacl-0.4/tests/test_error_model_fit.py
+-rw-rw-r--   0 nrl       (1000) nrl       (1000)     1611 2023-06-07 13:27:12.000000 sn-nacl-0.4/tests/test_fullsim_sngen.py
+-rw-rw-r--   0 nrl       (1000) nrl       (1000)     2183 2023-06-22 07:54:44.000000 sn-nacl-0.4/tests/test_jla.py
+-rw-rw-r--   0 nrl       (1000) nrl       (1000)      794 2023-06-01 21:25:17.000000 sn-nacl-0.4/tests/test_loglikelihood.py
+-rw-rw-r--   0 nrl       (1000) nrl       (1000)    18439 2023-02-10 14:06:32.000000 sn-nacl-0.4/tests/test_minimize_1D_multibandmodel_sifto_with_variance.py
+-rw-rw-r--   0 nrl       (1000) nrl       (1000)     8434 2023-02-10 14:06:32.000000 sn-nacl-0.4/tests/test_minimize_1dsplinemodel.py
+-rw-rw-r--   0 nrl       (1000) nrl       (1000)     4880 2023-02-10 14:06:32.000000 sn-nacl-0.4/tests/test_minimize_polyc1.py
+-rw-rw-r--   0 nrl       (1000) nrl       (1000)     5978 2023-02-10 14:06:32.000000 sn-nacl-0.4/tests/test_minimize_sincos.py
+-rw-rw-r--   0 nrl       (1000) nrl       (1000)    11217 2023-02-10 14:06:32.000000 sn-nacl-0.4/tests/test_minimize_toy1dsplinemodel.py
+-rw-rw-r--   0 nrl       (1000) nrl       (1000)    12259 2023-02-10 14:06:32.000000 sn-nacl-0.4/tests/test_minimize_toy1dsplinemodelfull.py
+-rw-rw-r--   0 nrl       (1000) nrl       (1000)      521 2023-06-02 05:59:12.000000 sn-nacl-0.4/tests/test_regularization.py
+-rw-rw-r--   0 nrl       (1000) nrl       (1000)    10589 2023-06-30 15:31:58.000000 sn-nacl-0.4/tests/test_salt2_training.py
+-rw-rw-r--   0 nrl       (1000) nrl       (1000)      298 2023-05-26 09:01:54.000000 sn-nacl-0.4/tests/test_salt2like_constraints.py
+-rw-rw-r--   0 nrl       (1000) nrl       (1000)     1156 2023-06-15 08:53:55.000000 sn-nacl-0.4/tests/test_salt2like_model.py
+-rw-rw-r--   0 nrl       (1000) nrl       (1000)     7914 2023-06-29 20:21:16.000000 sn-nacl-0.4/tests/test_snf.py
+-rw-rw-r--   0 nrl       (1000) nrl       (1000)      642 2023-06-01 15:31:23.000000 sn-nacl-0.4/tests/test_weighted_residuals.py
```

### Comparing `sn-nacl-0.3/nacl/distance.py` & `sn-nacl-0.4/nacl/distance.py`

 * *Files identical despite different names*

### Comparing `sn-nacl-0.3/nacl/fit.py` & `sn-nacl-0.4/nacl/fit.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,96 @@
 """
 
 TODO: Put the iterative training steps.
 """
 import numpy as np
-import os 
+import os
 from .lib import bspline
 from .minimizers import Minimizer, ModelPulls
 from .models.constraints import Constraints2D
 from .models.regularizations import SplineRegul2D
 from .models.variancemodels import SimpleVarianceModel
+from nacl import minimize
+from nacl.models.regularizations import NaClSplineRegularization
+from nacl.models.constraints import SALT2LikeConstraints, ab_flux_at_10Mpc
 
 from .plotting import plots
 
 try:
     from sksparse.cholmod import cholesky_AAt
 except ImportError:
     from scikits.sparse.cholmod import cholesky_AAt
 
 
+
+def fit(model, block_names, init_pars=None,
+        reg_order=0, mu_reg=1.E-6, active_cons=None, mu_cons=1.E6,
+        Mb=-19.5, n_iter=100):
+    """
+    """
+    model.pars.fix()
+    for block_name in block_names:
+        model.pars[block_name].release()
+
+    # we may need some regularization
+    reg = []
+    to_regularize = []
+    for block_name in ['M0', 'M1']:
+        if block_name in block_names:
+            to_regularize.append(block_name)
+    if len(to_regularize) > 0:
+        reg = NaClSplineRegularization(model, to_regularize=to_regularize,
+                                       order=reg_order, mu=mu_reg)
+        reg = [reg]
+
+    # we may need some contraints
+    cons = []
+    active = {}
+    for cons_name in ['M0', 'dM0', 'M1', 'dM1', 'col', 'X1', 'X1_var']:
+        if 'M0' in block_names and 'X0' in block_names:
+            active['M0'] = ab_flux_at_10Mpc(Mb)
+        if 'M1' in block_names:
+            active['M1'] = 0.
+        if 'M0' in block_names and 'tmax' in block_names:
+            active['dM0'] = 0.
+        if 'M1' in block_names and 'tmax' in block_names:
+            active['dM1'] = 0.
+        if 'CL' in block_names and 'col' in block_names:
+            active['col'] = 0.
+        if 'X1' in block_names and 'M1' in block_names:
+            active['X1'] = 0.
+            active['X1_var'] = 1.
+    if len(active) > 0:
+        cons = [SALT2LikeConstraints(model, active=active, mu=mu_cons)]
+
+    # if there are constraints, make sure that they are fullfilled
+    # at first order
+    model.pars['X1'].full -= model.pars['X1'].full.mean()
+    model.pars['X1'].full /= model.pars['X1'].full.std()
+    model.pars['col'].full -= model.pars['col'].full.mean()
+
+    # fit
+    wres = minimize.WeightedResiduals(model)
+    chi2 = minimize.LogLikelihood(wres, reg=reg, cons=cons)
+    minz = minimize.Minimizer(chi2, n_iter=n_iter)
+
+    # start the fit
+    solution = minz.minimize(model.pars.free)
+
+    ret = {}
+    ret['solution'] = solution
+    ret['model'] = model
+    ret['cons'] = cons
+    ret['reg'] = reg
+    ret['chi2'] = chi2
+    ret['pars'] = model.pars.copy()
+
+    return ret
+
+
 class FitModel2D(object):
     """
     Fitting procedure class.
     From a simulation, a model, error models, and parameters,
     can fit the model (given a minimizer) on data.
     If parameters are fixed, regularization and constraints are adjusted.
 
@@ -107,28 +176,28 @@
     def __init__(self, training_dataset, model_func, normalization_band_name='SWOPE::B',
                  init_from_salt2_file='data/salt2.npz', pars_fix=[],
                  minimizer=Minimizer, degree=3, disconnect_sp=False,
                  gamma_init=0.05, kappa_init=None, x1_var_real=False,
                  mu_pq=1e10, mu_pq_var_x1=None, mu_reg=1,
                  variance_model_bins=(3,3),
                  chi2_normalization=1, color_scatter_func=None, beta=1e-10,
-                 log=True, df_stop=1e-1, n_iter=500, basis_knot=[127, 20],
+                 log=True, df_stop=1e-1, n_iter=500, basis_knots=[127, 20],
                  pars_generation=None):
         """
         Constructor.
 
         Parameters
         ----------
         training_dataset : nacl.dataset.TrainingDataset
             Training dataset.
         model_func : nacl.salt
             Model.
         gamma_init : numpy.array ou float
             Parameters used to initialize the error snake.
-        basis_knot : 2-list
+        basis_knots : 2-list
             Number of wavelength and photometric knot.
         init_from_salt2_file : str
             If the model is to be initialized with the original
             SALT2-4 surfaces and bases, get them from this file.
         normalization_band_name : str
             Use this band to normalize the model.
         degree : int
@@ -179,70 +248,67 @@
         self.gamma_init = gamma_init
         self.kappa_init = kappa_init
         self.color_scatter_func = color_scatter_func
         self.x1_var_real = x1_var_real
 
         self.pars_free, self.x0, self.g0, self.reg, self.cons = None, None, None, None, None
 
-        self.basis_knot = basis_knot
+        self.basis_knots = basis_knots
         self.model = model_func(self.training_dataset,
                                 normalization_band_name=self.norm_band,
                                 spectrum_recal_degree=self.degree,
-                                basis_knot=self.basis_knot)
-      
+                                basis_knots=self.basis_knots)
+
         self.queue_wsp = self.model.queue.copy()
 
-        self.init_model_pars(filename=init_from_salt2_file, sn_info=self.training_dataset.sne)
+        self.init_model_pars(filename=init_from_salt2_file, sn_info=self.training_dataset.sn_data)
 
-        self.variance_model = SimpleVarianceModel(self.model, disconnect_sp=disconnect_sp,
+        self.variance_model = SimpleVarianceModel(self.model,
                                                   gamma_init=self.gamma_init,
                                                   bins=variance_model_bins)
 
         self.pars_generation = pars_generation
         self.N_sn_4plot = None
-        self.all_pars = ['X0', 'tmax', 'X1', 'c', 'M0', 'M1', 'CL',
+        self.all_pars = ['X0', 'tmax', 'X1', 'col', 'M0', 'M1', 'CL',
                          'SpectrumRecalibration', 'eta_calib', 'kappa_color']
-        
+
         self.mu_pq = mu_pq
         self.mu_pq_var_x1 = mu_pq_var_x1
         self.mu_reg = mu_reg
         self.chi2_normalization = chi2_normalization
         self.minimize_func = minimizer
 
         self.log = log
         self.N_ITER = n_iter
         self.df_stop = df_stop
-        
+
         self.pars_fix = pars_fix
         self.pars_release()
         self.model.pars0 = self.model.pars.full[:].copy()
-        
-        
+
+
     def init_model_pars(self, filename, sn_info):
         r"""
         Initiate model parameters.
 
         Parameters
         ----------
         filename : str
             The original
             SALT2-4 surfaces and bases, get them from this file.
         sn_info : numpy.rec.array
             SNe information (:math:`(z, X_0, X_1, c, t_{max})`)
         """
         m0, m1, cl = self.init_with_salt2(filename, self.model)
-        try:
-            self.model.pars['X0'][:] = sn_info['x0']
-            self.model.pars['X1'][:] = sn_info['x1']
-        except KeyError:
-            self.model.pars['X0'][:] = sn_info['norm']
-            self.model.pars['X1'][:] = sn_info['sig']
-        self.model.pars['tmax'][:] = sn_info['tmax']
-        self.model.pars['c'][:] = sn_info['c']
-        
+
+        self.model.pars['X0'][:] = sn_info.x0
+        self.model.pars['X1'][:] = sn_info.x1
+        self.model.pars['tmax'][:] = sn_info.tmax
+        self.model.pars['col'][:] = sn_info.col
+
         self.model.pars['M0'][:] = m0
         self.model.pars['M1'][:] = m1
         self.model.pars['CL'][:] = cl
         self.model.norm = self.model.normalization(band_name=self.norm_band)
 
     @staticmethod
     def init_with_salt2(filename, model):
@@ -256,18 +322,18 @@
         model : nacl.models.salt.SALT2Like
             Model.
         """
         f = np.load(filename)
         phase_grid = f['phase_grid']
         wl_grid = f['wl_grid']
         basis = bspline.BSpline2D(wl_grid, phase_grid, x_order=4, y_order=4)
-        
-        xx = np.linspace(wl_grid[0], wl_grid[-1], basis.bx.nj)                               
-        yy = np.linspace(phase_grid[0], phase_grid[-1], basis.by.nj)                          
-        
+
+        xx = np.linspace(wl_grid[0], wl_grid[-1], basis.bx.nj)
+        yy = np.linspace(phase_grid[0], phase_grid[-1], basis.by.nj)
+
         x, y = np.meshgrid(xx, yy)
         x, y = x.ravel(), y.ravel()
         jacobian = model.basis.eval(x, y)
         factor = cholesky_AAt(jacobian.T, beta=1e-20)
 
         return factor(jacobian.T * f['M0']), factor(jacobian.T * f['M1']), f['CL_pars']
 
@@ -295,27 +361,27 @@
         var_coef_init : float
             Standard deviation for the error snake parameters : :math:`\gamma`
         seed : int
             Seed for numpy.random
         """
         if seed is not None:
             np.random.seed(seed)
-            
+
         self.variance_model.pars.full[:] *= np.random.normal(1., var_coef_init,
                                                              len(self.variance_model.pars.full))
         print(f'\nVarModPars times N(1, {var_coef_init})')
         nb_sn = len(self.model.training_dataset.sne)
         for ps in self.pars_free:
             if (ps != 'eta_calib') & (ps != 'tmax'):
                 mv = model_coef_init
                 self.model.pars[ps].full[:] *= np.random.normal(1., mv,
                                                                 len(self.model.pars[ps].full))
                 if ps == 'X1':
                     self.model.pars[ps].full[:] -= self.model.pars[ps].full[:].mean()
-                    
+
                 print(f'{ps} times N(1, {mv})')
 
             elif model_coef_init != 0.:
                 if ps == 'tmax':
                     s_tmax = 0.05
                     self.model.pars['tmax'].full[:] += np.random.normal(0, s_tmax, nb_sn)
                     print(f'{ps} + N(0, {s_tmax})')
@@ -385,69 +451,69 @@
         fit_spec : bool
             If spectral data are considered.
         sigma_kappa_fit : bool
             If color scatter should be fixed.
 
         TODO : add color scatter parameters fixation in pars_fix.
         """
-        
+
         self.pars_fix = np.array(pars_fix)
         self.pars_release()
 
         print("\nNumber of free parameters :")
         for i in self.all_pars:
             print(i, self.model.pars[i].free.shape)
         print("\n")
-        
+
         self.regularization()
         self.constraints()
         self.g = g
         if fit_spec is False:
             self.model.queue = [i for i in self.model.queue if (i.data['spec_id'].mean() == -1)]
-            
+
         self.f = ModelPulls(self.model,
                             variance_model=self.variance_model, fit_spec=fit_spec,
                             chi2_normalization=self.chi2_normalization)
-        
+
         if 'gamma' in pars_fix:
             self.f.VarianceModel.pars.fix()
 
         if sigma_kappa is not None:
-            self.color_scatter = self.color_scatter_func(self.model.lambda_c_red, sigma_kappa) 
+            self.color_scatter = self.color_scatter_func(self.model.lambda_c_red, sigma_kappa)
         else :
             self.color_scatter = None
-        
+
         minimizer = self.minimize_func(self.f, constrains=self.cons,
                                        regularization=self.reg,
                                        color_scatter=self.color_scatter, ##
-                                       n_iter=self.N_ITER, 
+                                       n_iter=self.N_ITER,
                                        df_stop=self.df_stop, log=self.log, beta_cholmod=self.BETA)
-        
+
         minimizer(self.model.pars.free, sigma_kappa=sigma_kappa,
                   gamma0=self.g, eta_covmatrix=eta_covmatrix, sigma_kappa_fit=sigma_kappa_fit)
 
         self.M = minimizer.M
         self.gradf = minimizer.gradf
         self.minim = minimizer
-        
+
         self.sigma_kappa = minimizer.sigma_kappa
         if (self.sigma_kappa is not None) & sigma_kappa_fit:
             self.dsigma_kappa = minimizer.dsigma_kappa
-        
+
         self.timing = {'iter': np.array(minimizer.titer).mean(),
                        'cholesky': np.array(minimizer.tcholesky).mean(),
                        'model': np.array(minimizer.tmodel).mean(),
                        'hessian': np.array(minimizer.thessian).mean(),
                        's_iter': np.array(minimizer.titer).std(),
                        's_cholesky': np.array(minimizer.tcholesky).std(),
                        's_model': np.array(minimizer.tmodel).std(),
                        's_hessian': np.array(minimizer.thessian).std()}
-        
+
         self.log = minimizer.log
-        
+
         self.beta = minimizer.beta
         self.gamma = minimizer.gamma
 
         if fit_spec is False:
             self.model.queue = self.queue_wsp
 
     def control_plot(self, n_fit, variance_model=None,
@@ -455,20 +521,20 @@
         """
         Make control plots.
         """
         if save_dir is not None:
             save_dir = f'{save_dir}'
             if not os.path.exists(save_dir):
                 os.makedirs(save_dir)
-            
+
         if variance_model is not None:
             variance_model = self.variance_model
         if self.N_sn_4plot is None:
             self.N_sn_4plot = np.random.randint(0, len(self.training_dataset.sne), 5)
-            
+
         for isn in self.N_sn_4plot:
             plots.plot_lc(self.model, isn, variance_model=variance_model,
                           save_dir=save_dir, add_name=add_name)
             plots.plot_spec(self.model, isn, variance_model=variance_model,
                             save_dir=save_dir, add_name=add_name)
         # plots.binning_residuals(self.model, save_dir=save_dir, add_name=add_name)
         plots.residual_histogram(self.model, n_fit, variance_model=variance_model,
```

### Comparing `sn-nacl-0.3/nacl/instruments.py` & `sn-nacl-0.4/nacl/instruments.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,14 +111,15 @@
 
     """
     global _transmission_repository
     full_name = instrument_name + '::' + passband_name
     ret = _transmission_repository.get(full_name)
     if ret is None:
         try:
+
             instr = load_instrument(instrument_name, path=path)
             ret = instr.EffectiveFilterByBand(passband_name)
             #print('FLux in e not ADU')
             #ret = instr.get_efficiency_at_airmass(passband_name)
             _transmission_repository[full_name] = ret
         except KeyError:
             raise KeyError
@@ -138,22 +139,23 @@
 
     Returns
     -------
     numpy.array
         Filter transmission.
     """
     instrument_name, passband_name = full_name.split('::')
+
     return load_transmission(instrument_name, passband_name, path=path)
 
 
 class FilterDb:
     """
-    Utility class that projects a set of filters on B-splines 
-    and stores the projection coefficients. 
-    
+    Utility class that projects a set of filters on B-splines
+    and stores the projection coefficients.
+
     The class is given a default projection basis, but it is always
     possible to define one (adapted) basis per filter.
 
     Attributes
     ----------
     basis : nacl.lib.bspline.BSpline
         Spline basis.
@@ -186,40 +188,40 @@
         self.basis = basis
         self._grid, self._J, self._factor = self._projector(self.basis)
         self.filterpath = filterpath
         # I leave a trace of the factor that the FilterSet did actually
         # include the possibility of adding an external atmosphere model
         # Never used in practice -> I got rid of that.
         # self._atm = np.ones_like(self._grid)
-        
+
         self.transmission_db = {}
         self.db = {}
 
         # if a tds is given, load all the transmissions
-        # which appear in it. 
-        if tds is not None:
-            for tr in tds.get_all_transmissions():
+        # which appear in it.
+        if tds is not None and tds.get_all_transmissions() is not None:
+            for tr in tds.get_all_transmissions().values():
                 self.insert(tr)
         if additional_band is not None:
             for bd in additional_band:
                 self.insert(load(bd))
-                
+
     def __len__(self):
         """
         Given number of filter stored in database.
         """
         return len(self.db)
 
     @staticmethod
     def _projector(basis):
         r"""
-        Precompute the elements and factorization of the fit matrix 
-            
+        Precompute the elements and factorization of the fit matrix
+
         .. math:: (J^T J)^{-1} J^T
-        
+
         this saves repeated calls to cholesky_AAt when processing
         other filters.
 
         Parameters
         ----------
         basis : nacl.lib.bspline.BSpline
             Spline basis.
@@ -243,15 +245,15 @@
         factor = cholesky_AAt(jacobian.T)
         return gxx, jacobian, factor
 
     def insert(self, tr, z=0., basis=None):
         """
         Project the transmission `tr` on the spline basis and insert it
         into the database.
-        
+
         If basis is None (which should be almost always the case) we
         use the default projector. Otherwise, we recompute a projector
         and use it.
 
         Parameters
         ----------
         tr :
@@ -270,29 +272,29 @@
         """
         if basis is None:  # then, use the default basis
             grid, jacobian, factor = self._grid, self._J, self._factor
             b = self.basis
         else:
             grid, jacobian, factor = self._projector(basis)
             b = basis
-            
+
         y = tr(grid * (1.+z))  # * atm
         tq = self._factor(self._J.T * y)
 
         full_name = tr.InstrumentName + '::' + tr.Band
         self.transmission_db[full_name] = tr
         self.db[(full_name, z)] = (tq, b)
         if z == 0.:
             self.db[full_name] = (tq, b)
         return tq, b
-        
+
     def __getitem__(self, key):
         """
-        Retrieve the coefficients and basis for the requested filter. 
+        Retrieve the coefficients and basis for the requested filter.
         """
         if key not in self.db:
             raise KeyError
         return self.db[key]
-    
+
     def plot(self, key):
         pass
-    
+
```

### Comparing `sn-nacl-0.3/nacl/lib/atmosphericmodel.py` & `sn-nacl-0.4/nacl/lib/atmosphericmodel.py`

 * *Files identical despite different names*

### Comparing `sn-nacl-0.3/nacl/lib/bspline.py` & `sn-nacl-0.4/nacl/lib/bspline.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,15 @@
     np.ctypeslib.ndpointer(np.double, ndim=1, flags='aligned, contiguous, writeable'),
     ctypes.c_int,
     ctypes.c_int,
     ctypes.c_int,
     ctypes.c_int]
 
 _binary_search_with_guess = _lib.binary_search_with_guess
-_binary_search_with_guess.restype = np.int
+_binary_search_with_guess.restype = np.int32
 _binary_search_with_guess.argtypes = [
     ctypes.c_double,
     np.ctypeslib.ndpointer(np.double, ndim=1, flags='aligned, contiguous'),
     ctypes.c_int,
     ctypes.c_int]
 
 _binary_search = _lib.binary_search
@@ -902,37 +902,37 @@
     
     # weights
     ww = np.tile(w, nk)
     N = len(ww)
     i = np.arange(N)
     W = coo_matrix((ak*ww, (i,i)), shape=(N,N))
     
-    # some bases accept dtypes, other not.. 
+    # some bases accept dtypes, other not...
     # TODO: uniformize this (ban np.float32 and remove dtype options ?)
     B1 = basis1.eval(pp)
     B2 = basis2.eval(pp)
     return B1.T * W * B2
 
 
 def lgram(spectrum_basis, filter_basis, **keys):
-    """Compute the :math:`\lambda-`Gramian of both bases.
+    """Compute the :math:`\\lambda-`Gramian of both bases.
 
     When computing broadband fluxes, using transmission functions as
     spectra developed on spline bases, one needs to compute the
-    following quantities: 
+    following quantities:
 
-    .. math:: 
-         G_{ij} = \int B_i(\lambda) B_j(\lambda) \lambda d\lambda
-      
+    .. math::
+         G_{ij} = \\int B_i(\\lambda) B_j(\\lambda) \\lambda d\\lambda
+     
     This function computes the G-matrix above, and returns it as a
     sparse matrix. The spectrum basis may be shifted by a factor
     (1+z), for example:
 
     .. math::
-         G_{ij} = \int B_i(\lambda) B_j(\lambda / (1+z)) \lambda d\lambda
+         G_{ij} = \\int B_i(\\lambda) B_j(\\lambda / (1+z)) \\lambda d\\lambda
 
     """
     # Gaussian quadrature points and weights
     deg = spectrum_basis.order + filter_basis.order
     p, w = leggauss(deg)
     
     z = keys.get('z', 0.)
```

### Comparing `sn-nacl-0.3/nacl/lib/constants.py` & `sn-nacl-0.4/nacl/lib/constants.py`

 * *Files identical despite different names*

### Comparing `sn-nacl-0.3/nacl/lib/dataproxy.py` & `sn-nacl-0.4/nacl/lib/dataproxy.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,44 +1,45 @@
 
 
 
 import numpy as np
-from ..util.io import NTuple
+import pandas
 
+# from ..util.io import NTuple
 
 
 class DataProxy:
     """ Provide flexible ntuple manipulation.
 
     In particular allows to map fields of a ntuple to arbitrary field
     names and eases the creation of index for fields.
     """
-    def __init__(self,filename, **keys):
+    def __init__(self, datasrc, **keys):
         """Parameters:
 	-----------
 
 	keys: provides a mapping between fields of the ntuple and
 	arbitrary names. For exemple, keys mag='mmag' will create
 	the view: dp.mag = nt['mmag']
 	"""
 	# Load data
-        if isinstance(filename, str):
-            self.nt = NTuple.fromfile(filename)
-        else:
-            self.nt = filename
+        self.nt = datasrc
         self.mapping = keys
         self._create_views()
         self._index_list=set()
         self._proxy_list=[]
         self._external_field_list=[]
 
+    def __len__(self):
+        return len(self.nt)
+        
     def _create_views(self):
         # Create views
         for k, v in self.mapping.items():
-            setattr(self,k,self.nt[v])
+            setattr(self, k, self.nt[v])
 
     def add_views(self, **keys):
         """ A view is a mapping of a NTuple field: dp.key = nt['otherkeyname']"""
         for k, v in keys.items():
             setattr(self, k, self.nt[v])
         self.mapping.update(keys)
 
@@ -56,18 +57,22 @@
         s[index.astype('int')] = data
         setattr(self, name, s)
 
     def add_field(self, name, data):
         """ Add external data sharing the same number of records.
 
 	There is no mem copy so this is more memory efficient than
-	just catenating the field to the existing NTuple.""" 
-        self._external_field_list.append(name)
-        setattr(self, name, data)
-
+	just catenating the field to the existing NTuple."""
+        if name not in self._external_field_list:
+            self._external_field_list.append(name)
+        if isinstance(self.nt, (pandas.DataFrame, pandas.Series)):
+            setattr(self, name, pandas.Series(data))
+        else:
+            setattr(self, name, data)
+            
     def _update_external_fields(self, condition):
         for name in self._external_field_list:
             setattr(self, name, getattr(self,name)[condition])
 
     def compress(self, condition):
         self.nt = self.nt[condition].squeeze()
         self._create_views()
```

### Comparing `sn-nacl-0.3/nacl/lib/fitparameters.py` & `sn-nacl-0.4/nacl/lib/fitparameters.py`

 * *Files identical despite different names*

### Comparing `sn-nacl-0.3/nacl/lib/indextools.py` & `sn-nacl-0.4/nacl/lib/indextools.py`

 * *Files identical despite different names*

### Comparing `sn-nacl-0.3/nacl/lib/instruments.py` & `sn-nacl-0.4/nacl/lib/instruments.py`

 * *Files identical despite different names*

### Comparing `sn-nacl-0.3/nacl/lib/interpolation.py` & `sn-nacl-0.4/nacl/lib/interpolation.py`

 * *Files identical despite different names*

### Comparing `sn-nacl-0.3/nacl/lib/optim.py` & `sn-nacl-0.4/nacl/lib/optim.py`

 * *Files identical despite different names*

### Comparing `sn-nacl-0.3/nacl/lib/robuststat.py` & `sn-nacl-0.4/nacl/lib/robuststat.py`

 * *Files identical despite different names*

### Comparing `sn-nacl-0.3/nacl/lib/spectrum.py` & `sn-nacl-0.4/nacl/lib/spectrum.py`

 * *Files identical despite different names*

### Comparing `sn-nacl-0.3/nacl/lib/stellarlibs.py` & `sn-nacl-0.4/nacl/lib/stellarlibs.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,27 +4,27 @@
 this code is to compute effiently broadband fluxes from potentially
 large series of SEDs.
 
 Rationale
 ---------
 When building broadband fluxes from spectra, it is efficient to first
 project the spectra on a unique, well defined spline basis (generally
-of low order, e.g.  1 or 2): 
+of low order, e.g.  1 or 2):
 
 .. math:: S(\lambda) = \sum_i s_i B_i(\lambda) = B^T S
-    
+
 If the transmissions functions of the telescope are also developed on
 a spline basis (not necessarily the same):
 
 .. math:: T(\lambda) = \sum_i f_i K_i(\lambda) = K^T F
 
 then, the broadband fluxes can be written as:
 
 .. math:: \Phi= \int T(\lambda) \\frac{\lambda}{hc} S(\lambda) d\lambda = F^T G S
-        
+
 where :math:`G` is the *gramian* of the two bases, i.e.  the matrix
 that contains the integrals of the dyadic products of the basis
 elements: :math:`G_{ij} = \int B_i(x) K_j(x) dx`. Since the support of
 the splines is finite, :math:`G` is a very sparse band-matrix, and the
 computation of the integral above is very fast. In fact, the product
 :math:`F^T G` can be precomputed and re-used for each spectrum, hence,
 the integral reduces to a scalar product.
@@ -61,15 +61,15 @@
 >>> calspec = stellarlibs.Calspec(basis=basis)
 
 Save / load the basis into / from a .npz file
 
 >>> calspec.save('calspec.npz')
 >>> calspec = stellarlibs.Calspec(filename='calspec.npz')
 
-Prepare a set of filters 
+Prepare a set of filters
 
 >>> from .instruments import InstrumentModel
 >>> grid = np.arange(3000., 12005., 10.)
 >>> lsst = InstrumentModel("LSST")
 >>> fs = stellarlibs.FilterSet(grid=grid, [lsst.EffectiveFilterByBand(b) for b in "griz"])
 
 Compute broadband fluxes
@@ -84,26 +84,26 @@
 
 >>> index, spectra = stellarlibs.Pickles.fetch(basis=None)
 
 Integrate the original spectra using Spectrum.IntegFlux
 
 >>> flx = stellarlib.flux(spectra, fs)
 
-Modify the atmosphere in the filter set 
+Modify the atmosphere in the filter set
 
 >>> from atmosphericmodel import Buton
 >>> atm = Buton()
 >>> fs.atmosphere = atm  # multiply by Buton and reproject the filters
 >>> flx = stellarlib.flux(spectra, fs)
 
 .. Warning:: IntegFlux and the gram() method (i.e.  the slow and
     fast options) should differ due to the infamous (hc)_snfit vs
     (hs)_scipy problem.  I am correcting the gram() flux by hand to
-    adjust them to what IntegFlux returns. At some point, we need to 
-    correct both methods. 
+    adjust them to what IntegFlux returns. At some point, we need to
+    correct both methods.
 """
 
 import os
 import os.path as op
 #from exceptions import NotImplementedError, ValueError
 
 import numpy as np
@@ -117,156 +117,156 @@
 from . import constants
 from ..util import saltpath, io
 
 try:
     from sksparse.cholmod import cholesky_AAt
 except ImportError:
     from scikits.sparse.cholmod import cholesky_AAt
-    
-# get rid of this at some point ! 
+
+# get rid of this at some point !
 ALIGN_WITH_INTEG_FLUX = 0.9964833253040145 / 1.001899
 
 
 
 class StellarLib(object):
     """Holds a collection of spectra projected on a spline basis.
-    
-    
+
+
     """
     def __init__(self, **kw):
-        """Build the library, from a 
+        """Build the library, from a
         """
         if 'filename' in kw:
             self.load(kw['filename'])
         elif 'basis' in kw:
             self.basis = kw.pop('basis')
             self.grid = self.basis.grid
             self.index, self.fluxes = self.__class__.fetch(self.basis, **kw)
         elif 'grid' in kw:
             self.grid = self.pop('grid')
             self.basis = BSpline(self.grid)
             self.index, self.fluxes = self.__class__.fetch(self.basis, **kw)
         else:
             self.index, self.fluxes = self.__class__.fetch(None,**kw)
-            
+
     def __len__(self):
         return len(self.index)
 
     def save(self, filename):
         """Save the stellar library contents into a .npz file
-        
-        Dump the basis, projected spectra and metadata into a single .npz file. 
+
+        Dump the basis, projected spectra and metadata into a single .npz file.
 
         Args:
             filename (str): name of the .npz file
         """
         np.savez(filename, grid=self.basis.grid, index=self.index, fluxes=self.fluxes)
-        
+
     def load(self, filename):
-        """Load the stellar library from a .npz filename. 
+        """Load the stellar library from a .npz filename.
 
         Load the basis, projected spectra, and spectrum metadata from
         the .npz file specified in argument.
 
         Args:
             filename (str): name of the .npz file
         """
         r = np.load(filename)
         self.grid = r['grid']
         self.basis = BSpline(self.grid)
         self.index = r['index']
-        self.fluxes = r['fluxes']        
-        
+        self.fluxes = r['fluxes']
+
 
 class Pickles(StellarLib):
     """Spectra from (Pickles, 1992), projected on a BSpline basis.
 
     This is a specialization of :class:`StellarLib`, for the library
     of spectra described in (Pickles, 1992). This class implements
     essentially a method :meth:`load` which fetches the original
     spectra from their files, and projects them onto the basis
-    specified by the user. 
+    specified by the user.
     """
     def __init__(self, **kw):
         """Constructor
 
         Instantiate the Pickles library.  This is not the original
         library in the sense that all the spectra are projected on a
         BSpline basis (of order 2, unless specified otherwise).
 
         Args:
-            filename (str, optional): load the library from the file 
+            filename (str, optional): load the library from the file
             basis (BSpline, optional): specify the BSpline basis on
                 which to project the spectra
             grid (ndarray, optional): specify the basis grid. An order 2
                 (degree 1) BSpline basis will be instantiated on that grid.
 
-        .. TODO 
-            add an option to self.load, so that it can retrieve the original 
+        .. TODO
+            add an option to self.load, so that it can retrieve the original
             (non projected) library.
         """
         super(Pickles, self).__init__(**kw)
-        
+
     @staticmethod
     def fetch(basis):
         """fetch original spectra and project them on the spline basis
-        
+
         Fetch the original spectra (from $SALTPATH/stellarlibs) and
         project them on the basis given in argument.
 
         Args:
             basis (BSpline type object): basis on which to project the spectra
-            
+
         Returns:
             recarray, ndarray: index, spline coefficients if basis is not None
-                               index, original spectra otherwise            
+                               index, original spectra otherwise
         """
-        import glob 
+        import glob
         path = op.join(saltpath.stellar_libs_path, 'pickles')
         # retain only the 'u*.dat' spectra (extended)
         filenames = glob.glob(path + os.sep + 'u*.dat')
         #        filenames = filter(lambda x: op.basename(x)[0]!='u', filenames)
         n = len(filenames)
-        
-        # data structure 
+
+        # data structure
         # we separate the metadata (put in the index tab)
         # from the spline coefficients (stored in spectra)
         # it seems better to have the spline coeffs contiguous in memory.
-        dtype = np.dtype([('styp', '|S10'), 
-                         ('filename', '|S20')]) 
+        dtype = np.dtype([('styp', '|S10'),
+                         ('filename', '|S20')])
         #                ('p', np.float64, len(basis))])
         index  = np.zeros(n, dtype=dtype)
         if basis is not None:
             spectra = np.zeros((n, len(basis)), dtype=np.float64)
             # we oversample a bit the spectra, to overconstrain
             # the basis projection a little
             gx = basis.grid
             ovsp_gx = np.hstack((gx, 0.5*(gx[1:]+gx[:-1])))
             ovsp_gx.sort()
         else:
             spectra = []
-        
+
         # loop on the spectra
         for i,fn in enumerate(filenames):
             with open(fn) as f:
                 wl, flux = [], []
                 for line in f.readlines():
                     wl.append(float(line[0:7]))
                     flux.append(float(line[8:17]))
             wl, flux = np.asarray(wl), np.asarray(flux)
             index[i]['styp'] = op.basename(fn).split('.')[0]
-            index[i]['filename'] = op.basename(fn)            
-            
+            index[i]['filename'] = op.basename(fn)
+
             # oversample the spectral data and project it on the basis
             if basis is not None:
                 yy = np.interp(ovsp_gx, wl, flux)
                 spectra[i,:] = basis.linear_fit(ovsp_gx, yy)
             else:
                 spectra.append(Spectrum(wl, flux))
-                
+
         return index, spectra
 
 class PicklesDepagne(StellarLib):
     """Spectra from (Pickles Depagne, 2010), projected on a BSpline basis.
 
     This is a specialization of :class:`StellarLib`, for the library
     of spectra described in (Pickles, 1992) plus a few peculiar
@@ -281,284 +281,283 @@
 
         Instantiate the library.  This is not the original library in
         the sense that all the spectra are projected on a BSpline
         basis (of order 2, unless specified otherwise), and have been
         renormalised to a synthetic mag VT=0.
 
         Args:
-            filename (str, optional): load the library from the file 
+            filename (str, optional): load the library from the file
             basis (BSpline, optional): specify the BSpline basis on
                 which to project the spectra
             grid (ndarray, optional): specify the basis grid. An order 2
                 (degree 1) BSpline basis will be instantiated on that grid.
         """
         super(PicklesDepagne, self).__init__(**kw)
-        
+
     @staticmethod
     def fetch(basis):
         """fetch original spectra and project them on the spline basis
-        
+
         Fetch the original spectra (from $SALTPATH/stellarlibs) and
         project them on the basis given in argument.
 
         Args:
             basis (BSpline type object): basis on which to project the spectra
-            
+
         Returns:
             recarray, ndarray: index, spline coefficients if basis is not None
-                               index, original spectra otherwise            
+                               index, original spectra otherwise
         """
-        import glob 
+        import glob
         path = op.join(saltpath.stellar_libs_path, 'picklesdepagne10')
         # retain only the 'u*.dat' spectra (extended)
         filenames = [op.join(path,  '%d.lib' % i) for i in range(141)]
         #        filenames = filter(lambda x: op.basename(x)[0]!='u', filenames)
         n = len(filenames)
-        
-        # data structure 
+
+        # data structure
         # we separate the metadata (put in the index tab)
         # from the spline coefficients (stored in spectra)
         # it seems better to have the spline coeffs contiguous in memory.
-        dtype = np.dtype([('styp', '|S10'), 
-                         ('filename', '|S20')]) 
+        dtype = np.dtype([('styp', '|S10'),
+                         ('filename', '|S20')])
         #                ('p', np.float64, len(basis))])
         index  = np.zeros(n, dtype=dtype)
         if basis is not None:
             spectra = np.zeros((n, len(basis)), dtype=np.float64)
             # we oversample a bit the spectra, to overconstrain
             # the basis projection a little
             gx = basis.grid
             ovsp_gx = np.hstack((gx, 0.5*(gx[1:]+gx[:-1])))
             ovsp_gx.sort()
         else:
             spectra = []
-        
+
         # loop on the spectra
         for i,fn in enumerate(filenames):
             nt = io.NTuple.fromtxt(fn)
-            
+
             index[i]['styp'] = '%d' % i
-            index[i]['filename'] = op.basename(fn)            
-            
+            index[i]['filename'] = op.basename(fn)
+
             # oversample the spectral data and project it on the basis
             if basis is not None:
                 yy = np.interp(ovsp_gx, nt['wl'], nt['flux'])
                 spectra[i,:] = basis.linear_fit(ovsp_gx, yy)
             else:
                 spectra.append(Spectrum(nt['wl'], nt['flux']))
-                
+
         return index, spectra
 
 class Calspec(StellarLib):
     """Spectra from the latest CALSPEC release (Bohlin, 2014),
     projected on a BSpline basis.
 
     This is a specialization of :class:`StellarLib`, for the library
-    of spectra described in (Bohlin, 2014). 
-    """    
+    of spectra described in (Bohlin, 2014).
+    """
     def __init__(self, **kw):
         super(Calspec, self).__init__(**kw)
-            
+
     @staticmethod
     def fetch(basis, version='2015-01'):
         """load the spectra from the original files
-        
+
         Args:
             basis (BSpline or None): BSpline basis to use
             version (str): CALSPEC release data
 
         Returns:
             recarray, ndarray: index and spline coeffs if basis is not None
                                index and list of Spectrum.Spectrum
         """
         path = op.join(saltpath.stellar_libs_path,
-                       'calspec-' + version)                       
-        # read the index 
+                       'calspec-' + version)
+        # read the index
         index_file = op.join(path, 'index.org')
         if not op.isfile(index_file):
             raise ValueError('unable to find CALSPEC index: %s' % index_file)
         index = io.NTuple.fromorg(index_file)
-        
+
         n = len(index)
         if basis is not None:
             gx = basis.grid
             ovsp_gx = np.hstack((gx, 0.5*(gx[1:]+gx[:-1])))
             ovsp_gx.sort()
             spectra = np.zeros((n, len(basis)), dtype=np.float64)
         else:
             spectra = []
-            
+
         for i,d in enumerate(index):
             with pf.open(path + os.sep + d['FILENAME']) as f:
                 wl = f[1].data['WAVELENGTH']
                 flux = f[1].data['FLUX']
                 if basis is not None:
                     #flux = flambda_to_fclambda(wl, flux)
                     yy = np.interp(ovsp_gx, wl, flux)
                     spectra[i,:] = basis.linear_fit(ovsp_gx, yy)
                 else:
                     spectra.append(Spectrum(wl, flux))
 
         return index, spectra
 
-    
+
 class FilterSet(object):
     """
     Utility class that projects a set of filters on B-Splines
-    and stores the projection coefficients. 
+    and stores the projection coefficients.
 
     ..  note:: this code should be merged with
         :class:`instruments.FilterWheel`. We keep it here
-        until we get to talk with the Great Guardians.    
+        until we get to talk with the Great Guardians.
     """
     def __init__(self, basis, transmissions, atmosphere_model=None, distort_func=None):
         self.basis = basis
         if type(transmissions) is dict:
             self.transmissions = transmissions
         elif type(transmissions) is list:
-            self.transmissions = dict([(t.InstrumentName + '::' + t.Band, t) 
+            self.transmissions = dict([(t.InstrumentName + '::' + t.Band, t)
                                        for t in transmissions])
         # projection grid (larger than basis grid)
         self._grid, self._J, self._factor = self._projector(self.basis)
         self.atm = np.ones_like(self._grid)
         if distort_func is None:
             self.distort = None
         else:
             self.distort = distort_func(self._grid)
         self.parameters = self._project(basis, self.transmissions)
         self.bands = list(self.transmissions.keys())
         self.mean_wl = dict([(k,t.mean(t.x_min, t.x_max)) for k,t in list(self.transmissions.items())])
 
-
     def _projector(self, basis):
         # refine the basis grid
         gx = basis.grid
         gxx = np.hstack((gx, 0.5*(gx[1:]+gx[:-1])))
         gxx.sort()
         # precompute the projector
         # (will save repeated calls to cholesky_AAt)
         J = basis.eval(gxx).tocsr()
         factor = cholesky_AAt(J.T)
         return gxx, J, factor
 
     def _project(self, basis, transmissions):
         ret = {}
         if type(self.atm) is dict:
-            # get rid of this case at some point. 
+            # get rid of this case at some point.
             # this adds complications to the code
-            # we do not need that anymore since 
+            # we do not need that anymore since
             # we now can extract a subset of the FilterSet
             for k,t in list(transmissions.items()):
                 y = t(self._grid) * self.atm[k]
                 if self.distort is not None:
                     y *= self.distort
                 ret[k] = self._factor(self._J.T * y)
         else:
             for k,t in list(transmissions.items()):
                 y = t(self._grid) * self.atm
                 if self.distort is not None:
                     y *= self.distort
                 ret[k] = self._factor(self._J.T * y)
         return ret
-    
+
     def __len__(self):
         return len(self.transmissions)
 
     def __getitem__(self, key):
         return self.parameters[key]
 
     def extract(self, band_names):
         tr = [self.transmissions[b] for b in band_names]
         return FilterSet(self.basis, tr)
 
     def mean_wavelength(self, bandnames):
         d = self.mean_wl
         return np.asarray([d[bn] for bn in bandnames])
-    
+
     @property
     def atmosphere(self):
         """return the current instance of the atmospheric transmission.
-        
+
         The atmospheric transmission is stored as a grid vector, of
         size equal to that of the internal grid (self._grid). Return
         that vector.
         """
         return self.atm
 
     @atmosphere.setter
     def atmosphere(self, atmosphere_model):
         """change the current instance of the atmospheric transmission.
-        
+
         Update the atmospheric transmission vector, and reproject the
         filters.
-        
+
         Args:
-            atmosphere_model (callable or dict of callables): 
+            atmosphere_model (callable or dict of callables):
                  the function that defines the atmospheric transmission.
                  (possibly one different transmission per band)
 
         .. todo: add atmospheric transmission as an explicit parameter in self._project
         """
         if type(atmosphere_model) is dict:
-            # get rid of this at some point 
+            # get rid of this at some point
             self.atm = {}
             for k,f in list(atmosphere_model.items()):
                 self.atm[k] = f(self._grid)
         else:
             self.atm = atmosphere_model(self._grid)
         self.parameters = self._project(self.basis, self.transmissions)
 
-    @property 
+    @property
     def distortion(self):
         return self.distort
-    
+
     @distortion.setter
     def distortion(self, distort_func):
         if distort_func is None:
             self.distort = None
         else:
             self.distort = distort_func(self._grid)
         self.parameters = self._project(self.basis, self.transmissions)
 
 
 def flux(filters, splib, wl_step=5., z=0.):
-    """Compute broadband fluxes (in e-/s) 
+    """Compute broadband fluxes (in e-/s)
 
     For each filter contained in the filter set, compute the the
     broadband fluxes of all the stars in the spectral library.
-    
+
     The function follows the snfit convention, in the sense that it
     expects *rest frame* SED's, expressed in
     :math:`\mathrm{erg/cm^2/s/A}` and returns *observer frame*
     broadband fluxes expressed in :math:`e^-/s`.  The broadband flux
     is defined as:
-            
+
     .. math:: f = \\frac{C}{(1+z)^2}\int S\\left(\\frac{\lambda}{1+z}\\right)\ \lambda\ T(\lambda)\ d\lambda
 
     where the integral is computed in the observer frame (hence the
     :math:`1/(1+z)^2` factor).  :math:`T` is the telescope
     transmission, in :math:`e^- cm^2 / \gamma`. The constant C is
     equal to :math:`1/hc` with h in erg s and c in A/s:
 
     .. math:: \\frac{1}{hc} \\approx 50341170.081942275\ \mathrm{erg^{-1} A^{-1}}
 
     using the values of h and c in `scipy.constants` (see however the
     warning section below).
-        
-    Args: 
+
+    Args:
         splib (inherits from `StellarLib`): a spectral library, or at
             least an object that holds a basis as well as a set of
             coefficients.
         filters (`FilterSet`): a filter set
         wl_step (float, optional): integration step (if using
             traditional method)
         z (float): redshift to apply to the spectrum
 
     Returns:
-        (numpy.rec.array) contains the broadband fluxes. 
+        (numpy.rec.array) contains the broadband fluxes.
 
     .. note:: The function may be passed either a FilterWheel and a
          list of ``Spectra``, in which case it is going to
          call ``spectrum.IntegFlux`` on each spectrum.  Alternatively,
          we can pass it a ``stellarlibs.FilterSet`` and a
          ``stellarlibs.StellarLib``. In this case, it uses the faster
          Gram method (see above). To decide what to do, it the
@@ -568,76 +567,76 @@
     .. WARNING:: IntegFlux and the gram() method (i.e.  the slow and
          fast options) differ due to the infamous (hc)_snfit vs
          (hs)_scipy problem.  I am correcting the gram() flux by hand
          to adjust them to what IntegFlux returns. At some point, we
          need to correct both methods.
     """
     names, fluxes = [], []
-    
+
     if hasattr(splib, 'basis') and hasattr(filters, 'basis'):
         G = lgram(splib.basis, filters.basis, z=z)
         for key, pars in list(filters.parameters.items()):
             U = G.dot(pars)
             names.append(key)
             fluxes.append(ALIGN_WITH_INTEG_FLUX * np.dot(splib.fluxes, U))
     elif type(splib) is list:
         for k,tr in list(filters.transmissions.items()):
             names.append(k)
             fluxes.append([s.IntegFlux(tr, wavelength_integration_step=wl_step, z=z)
                            for s in splib])
     else:
         raise ValueError("don't know what to do with splib=%s" % splib.__class__)
-    
+
     return np.rec.fromarrays(fluxes, names=names)
 
 
 # from instruments import MagSys
 # class MagSysFS(MagSys):
-    
+
 #     def __init__(self, magsys_name, basis=None):
 #         super(MagSysFS, self).__init__(magsys_name)
 #         if basis is None:
 #             grid = np.arange(2000., 12000., 1.)
 #             self.basis = BSpline(grid, order=4)
 #         print self.pure_ab
 #         if self.pure_ab:
 #             x = np.arange(2000., 12000., 0.5)
 #             self.spectrum = self.basis.linear_fit(x, constants.flux_ab(x))
 #         else:
 #             self.spectrum = self.
-                    
+
 #     def ZeroPoint(self, fs):
 #         pass
 
 #     def mag(self, filterset, splib, z=0.):
 #         pass
-    
+
 
 def mag(filters, splib, magsys, wl_step=5., z=0.):
-    """Broadband mags of the stars in the spectral library. 
+    """Broadband mags of the stars in the spectral library.
 
     For each filter contained in the filter set, compute the the
     broadband magnitudes, in the specified magnitude system, of all
     the stars in the spectral library.
-    
+
     Args:
-        splib (inherits from `StellarLib`): spectral library 
+        splib (inherits from `StellarLib`): spectral library
         filters (`FilterSet`): filters to use to compute the mags
         magsys (MagSys): magnitude system to use
-        wl_step(float, optional): integration step (if using 
+        wl_step(float, optional): integration step (if using
             traditional method).
         z (float): redshift to apply to the spectrum
 
     Returns:
         (numpy.rec.array): contains the broadband magnitudes.
     """
     names, mags = [], []
-    # fast option: splib and filters have a respline() method 
-    # that returns the basis and spline coefficients. 
-    # we can use the gram() method 
+    # fast option: splib and filters have a respline() method
+    # that returns the basis and spline coefficients.
+    # we can use the gram() method
     if hasattr(splib, 'basis') and hasattr(filters, 'basis'):
         G = lgram(splib.basis, filters.basis, z=z)
         for key, pars in list(filters.parameters.items()):
             T = filters.transmissions[key]
             zp = magsys.ZeroPoint(T)
             U = G.dot(pars)
             names.append(key)
@@ -648,11 +647,11 @@
             T = filters.transmissions[key]
             zp = magsys.ZeroPoint(T)
             flx = np.asarray([s.IntegFlux(tr, wavelength_integration_step=wl_step)
                               for s in splib])
             mags.append(-2.5 * np.log10(flx) + zp)
     else:
         raise ValueError("don't know what to do with splib=%s" % splib.__class__)
-            
-            
+
+
     return np.rec.fromarrays(mags, names=names)
```

### Comparing `sn-nacl-0.3/nacl/lib/utils.c` & `sn-nacl-0.4/nacl/lib/utils.c`

 * *Files identical despite different names*

### Comparing `sn-nacl-0.3/nacl/minimizers.py` & `sn-nacl-0.4/nacl/minimizers.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,19 +20,19 @@
                     level=logging.DEBUG)
 
 
 class Minimizer(object):
     r"""
     Newton Raphson minimizer.
 
-    Iterative algorithm that calculates for each iteration the increment :math:`\delta \beta`: 
+    Iterative algorithm that calculates for each iteration the increment :math:`\delta \beta`:
 
     .. math :: \delta \beta = -H^{-1} \nabla \chi^2
 
-    where :math:`\chi^2` is :math:`-2 \log(L)` and implemented in the Chi2Model class, 
+    where :math:`\chi^2` is :math:`-2 \log(L)` and implemented in the Chi2Model class,
     :math:`\nabla \chi^2` is the gradient and :math:`H` is the hessian.
 
     Attributes
     ----------
     pull_function : ModelPulls
         Class of pull evaluation, difference of model and data, on variance model.
         If no variance model is considered, the denominator is the 'FluxErr' of the data.
@@ -68,37 +68,37 @@
     hess : coo_matrix
         Iteration hessian matrix of the :math:`\chi^2`
     grad : array
         Iteration gradient of the :math:`\chi^2`
     increment : array
         increment
     """
-    
+
     def __init__(self, pull_function,
                  constrains=None, regularization=None, color_scatter = None,
                  n_iter=1000,
                  df_stop=1e-5, log=None, beta_cholmod=1e-10):
         r"""
-        Initiate the Minimizer class : 
+        Initiate the Minimizer class :
 
         Parameters
         ----------
         pull_function : ModelPulls
             Class of pull evaluation, difference of model and data, on variance model.
             If no variance model is considered, the denominator is the 'FluxErr' of the data.
         constrains : Constraints2D
             Class of constraints, evaluating the constraint as a function of the free
             parameters of the model.
         regularization : SplineRegul2D
             Class of regularization term, constraint splines parameters of surfaces without data.
         color_scatter :  ColorScatter
             Color scatter function that evaluate the color scatter and its derivatives.
         n_iter : int
-            Number of iteration maximum, after which the fit stops. 
-        df_stop : float 
+            Number of iteration maximum, after which the fit stops.
+        df_stop : float
             Threshold of :math:`\Delta \chi^2` that defines the convergence.
         log : bool
             Debug to keep in memory at each iteration all useful information,
             :math:`\beta, d\beta, \gamma, d\gamma, \chi^2(\beta), \chi^2(\beta+d\beta)`
         beta_cholmod : float
             Term in order to get the hessian positive definite (odg :math:`\sim 10^{-10}`)
         """
@@ -120,15 +120,15 @@
         self.beta, self.gamma, self.dbeta, self.dgamma, self.dsigma_kappa = None, None, None, None, None
         self.decrement = None
         self.hess, self.grad, self.increment = None, None, None
 
     def log_append(self, iteration, chi2_1, f_val, detail1, detail2):
         r"""
         Add to log the information of the iteration.
-        
+
         Parameters
         ----------
         iteration : int
             Iteration number.
         chi2_1 : float
             :math:`\chi^2(\beta_{iteration - 1})`
         f_val : float
@@ -142,60 +142,60 @@
             if self.sigma_kappa_fit & (self.sigma_kappa is not None):
                 self.log.append((iteration, self.beta, self.gamma, self.dgamma, self.dbeta,
                                  chi2_1, f_val, self.M, detail1, detail2,
                                  self.sigma_kappa.copy(), self.dsigma_kappa))
             else:
                 self.log.append((iteration, self.beta, self.gamma, self.dgamma, self.dbeta,
                                  chi2_1, f_val, self.M, detail1, detail2, None, None))
-        
+
     def parameter_update(self):
         r"""
         Updated the values of the model parameters :math:`\beta` and the variances model parameters : :math:`\gamma`,
         :math:`\sigma_\kappa` for the considered iteration.
-        
+
         Note
         ----
         In increment the parameters are stored as following :  :math:`(\beta, \gamma, \sigma_\kappa)`
         """
         if self.sigma_kappa_fit & (self.sigma_kappa is not None):
             # Slice the sigma_kappa parameters in increment
             self.dsigma_kappa = self.increment[self.fchi2.N_PAR:]
             # Slice the gamma parameters in increment
             self.dgamma = self.increment[len(self.beta): - len(self.dsigma_kappa)]
         else:
             self.dgamma = self.increment[len(self.beta):]
 
         self.dbeta = self.increment[: len(self.beta)]
         t = 1.
-        
+
         self.beta = self.beta + t * self.dbeta
-        
-        if len(self.pull_function.VarianceModel.pars.free) != 0:        
+
+        if len(self.pull_function.VarianceModel.pars.free) != 0:
             self.gamma = self.gamma + t * self.dgamma
         if self.sigma_kappa_fit & (self.sigma_kappa is not None):
             self.sigma_kappa += t * self.dsigma_kappa
             print('sigma_kappa : ', self.sigma_kappa)
             print('dsigma_kappa : ', self.dsigma_kappa)
 
     def print_end_iter(self, t, chi2_1, f_val, n_dof, detail1, detail2):
         r"""
         Print the iteration information of the :math:`\chi^2`.
-        
+
         Parameters
         ----------
         t : float
             Line-search parameters, default value is 1
-        chi2_1 : float                                                                                  
-            :math:`\chi^2(\beta_{iteration - 1})`                                                       
+        chi2_1 : float
+            :math:`\chi^2(\beta_{iteration - 1})`
         f_val : float
             :math:`\chi^2(\beta_{iteration})`
         n_dof : float
             Number of degrees of freedom, calculated as the difference of the number
             of data point and the number of free parameters.
-        detail1 : dict                       
+        detail1 : dict
             Values of the different component of the  :math:`\chi^2`, of the iteration number : iteration - 1
         detail2 : dict
             Values of the different component of the  :math:`\chi^2` of the iteration number : iteration
         """
         print('chi^2 contribution  i-1: ', detail1, '\n', 'chi^2 contribution  i: ',  detail2, '\n')
         if (np.isnan(f_val) ^ np.isinf(f_val)).sum() > 0:
             raise ValueError(f'Value of f_val : {f_val} ')
@@ -204,15 +204,15 @@
                      % (t, chi2_1, f_val, self.decrement, n_dof, f_val/n_dof))
         print(f"t_tot : {self.titer[-1]},  t_cho : {self.tcholesky[-1]}")
 
     def __call__(self, beta0, sigma_kappa=None, gamma0=None, eta_covmatrix=None,
                  sigma_kappa_fit=True):
         r"""
         Find the parameters of the model and the variance model by minimizing the log likelihood function.
-        
+
         Parameters
         ----------
         beta0 : array
             Initial model's parameters
         sigma_kappa : array or None
             Initial color scatter parameters.
             If None, the color scatter is not fitted.
@@ -226,123 +226,123 @@
         sigma_kappa_fit : bool
            True : sigma kappa of fitted
            False : They are not, but if sigma_kappa is not None, kappa parameters are fitted, with a fix color scatter.
         """
         self.gamma0 = self.gamma = gamma0
         self.beta = self.beta0 = beta0.copy()
         self.n = len(beta0)
-        
+
         self.factorCS = None
-            
+
         self.sigma_kappa_fit = sigma_kappa_fit
         self.sigma_kappa = sigma_kappa
-        
+
         if self.gamma0 is None:
             self.gamma = []
-                    
+
         self.M = np.ones(1)
         self.tcholesky, self.tmodel, self.thessian, self.titer = [], [],  [],  []
         for iteration in range(self.N_ITER):
             t0 = time.time()
             print('\n')
             logging.info('iteration: %d' % iteration)
             beta_keep = self.beta.copy()
             if len(self.gamma) != 0:
                 gamma_keep = self.gamma.copy()
             hess_keep = self.M.copy()
-            
+
             self.fchi2 = Chi2Model(pull_function=self.pull_function, constrains=self.constrains,
                                    regularization=self.regularization, color_scatter=self.color_scatter,
                                    sigma_kappa_fit=sigma_kappa_fit)
-            
+
             chi2_1, detail1, self.gradf, self.M = self.fchi2(self.beta, self.gamma, self.sigma_kappa,
                                                              eta_covmatrix=eta_covmatrix,
                                                              derivatives=True)
-            
+
             tmod = self.fchi2.model_evaluation
             thess = self.fchi2.hessian_construction
             self.thessian.append(thess)
             self.tmodel.append(tmod)
-            
+
             # solve the normal equation
-            t_cho = time.time()            
+            t_cho = time.time()
 
             # When Error snake is fitted : M not positively definated
             # => should use mode=simplicial (much slower)
             # if len(self.pull_function.VarianceModel.pars.free) == 0:
             #     fact = cholmod.cholesky(self.M.tocsc(), mode='supernodal',
             #                             ordering_method='metis', beta=self.beta_cholmod)
-                
+
             #     print('SUPERNODAL')
             # else :
             fact = cholmod.cholesky(self.M.tocsc(), mode='simplicial',
                                     ordering_method='metis', beta=self.beta_cholmod)
             print('SIMPLICIAL')
-            
+
             self.tcholesky.append(time.time() - t_cho)
-            self.increment = fact(-1*self.gradf) 
-            
+            self.increment = fact(-1*self.gradf)
+
             self.parameter_update()
-            
+
             if self.constrains is not None:
                 print('CHECK CONS 1: ', self.constrains(self.beta)*np.sqrt(self.constrains.sig_vals))
                 print('Variance X1 : ', self.constrains.var_x1(self.beta)/np.sqrt(self.constrains.mu_pq_var_x1), '\n')
-                
+
             ndof = len(self.pull_function.data) - len(self.beta)
             if len(self.pull_function.VarianceModel.pars.free) != 0:
                 ndof -= len(self.gamma)
-                
+
             if self.sigma_kappa_fit & (self.sigma_kappa is not None):
-                ndof -= len(self.sigma_kappa) 
+                ndof -= len(self.sigma_kappa)
 
             f_val, detail2 = self.fchi2(self.beta, self.gamma, self.sigma_kappa,
                                         eta_covmatrix=eta_covmatrix, derivatives=False)
             t = 1.
             self.titer.append(time.time() - t0)
             self.print_end_iter(t, chi2_1, f_val, ndof, detail1, detail2)
             self.log_append(iteration, chi2_1, f_val, detail1, detail2)
-            
+
             self.iminus1_chi2 = chi2_1
             self.final_chi2 = f_val
 
             self.iter = iteration
             if self.decrement < 0.0:
                 self.beta = beta_keep
-                self.M = hess_keep 
+                self.M = hess_keep
                 if len(self.gamma) != 0:
                     self.gamma = gamma_keep
                 if self.sigma_kappa_fit & (self.sigma_kappa is not None):
                     self.sigma_kappa = self.sigma_kappa - t * self.dsigma_kappa
                 self.pull_function.model.pars.free = self.beta
-                
+
                 if len(self.pull_function.VarianceModel.pars.free) != 0:
                     self.pull_function.VarianceModel.pars.free = self.gamma
 
             if self.decrement < self.DF_STOP:
                 break
 
 
 class Chi2Model(object):
     r"""
-     compute the full Lagrangian, including 
+     compute the full Lagrangian, including
       - the model,
-      - Error snake 
+      - Error snake
       - Color scatter
       - Constraints [optional]: a quadratic penalty derived from the constraints
       - Regularization [optional]
       - Propagation of calibration:
 
-     .. math:: 
+     .. math::
          \chi^{2} = \, & \chi^{2}_{model} + \chi^{2}_{cons} + \chi^{2}_{reg} +
          \chi^{2}_{calib} + \chi^{2}_{CS}  \nonumber \\
          =\, & \ln(|V(\beta, \gamma)|) + R(\beta)^T V^{-1}(\beta, \gamma) R(\beta) \nonumber \\
          + \, &  \mu_{pen} C(\beta)^T C(\beta) \nonumber \\
          +\, & \mu_{reg} \beta^T P \beta \nonumber \\
-         + \, & \eta^T V^{-1}_{\eta} \eta \nonumber\\ 
-         +\,& \ln{|V_{\kappa}( \sigma_\kappa)|} + \kappa^T V_\kappa^{-1}( \sigma_\kappa) \kappa 
+         + \, & \eta^T V^{-1}_{\eta} \eta \nonumber\\
+         +\,& \ln{|V_{\kappa}( \sigma_\kappa)|} + \kappa^T V_\kappa^{-1}( \sigma_\kappa) \kappa
 
 
     Attributes
     ----------
     pull_function : ModelPulls
         Class of pull evaluation, difference of model and data, on variance model.
         If no variance model is considered, the denominator is the 'FluxErr' of the data.
@@ -350,30 +350,30 @@
         Class of constraints, evaluating the constraint as a function of the free parameters of the model.
     regularization : SplineRegul2D
         Class of regularization term, constraints splines parameters of surfaces without data.
     lambda_c : array
         Mean rest-frame wavelength of each Light Curve.
     lambda_c_red :
         Reduced mean rest-frame wavelength of each Light Curve.
-    sigma_kappa_fit : bool 
+    sigma_kappa_fit : bool
         Whether color scatter parameters are fitted.
     beta : array
         Model parameters.
     gamma : array
         Variance model parameters.
     hess : coo_matrix
         Hessian matrix of the :math:`\chi^2`
     grad : array
         Gradient of the :math:`\chi^2`
     hessian_construction : float
-        Time of model part hessian matrix construction 
+        Time of model part hessian matrix construction
     model_evaluation : float
-        Time passing evaluating models           
-    """    
-    def __init__(self, pull_function, constrains=None, 
+        Time passing evaluating models
+    """
+    def __init__(self, pull_function, constrains=None,
                  regularization=None, color_scatter=None,
                  sigma_kappa_fit=True):
         """
         Initialization of the class.
 
         Parameters
         ----------
@@ -390,21 +390,21 @@
             Whether color scatter parameters are fitted.
 
         """
         self.pull_function = pull_function
         self.regularization = regularization
         self.constrains = constrains
         self.color_scatter = color_scatter
-        
+
         self.lambda_c_red = self.pull_function.model.lambda_c_red
         self.lambda_c = self.pull_function.model.lambda_c
         self.sigma_kappa_fit = sigma_kappa_fit
         self.hess, self.grad = None, None
         self.hessian_construction, self.model_evaluation = None, None
-        
+
     def __call__(self, beta, gamma, sigma_kappa=None, eta_covmatrix=None, derivatives=False):
         r"""
         Evaluation of the :math:`\chi^2`, with the update parameters
         (math:`\beta`, math:`\gamma`, math:`\sigma_\kappa`).
         Evaluated the gradiant and the hessian if needed.
 
         Parameters
@@ -437,15 +437,16 @@
         hess : scipy.sparse.csc_matrix
              Hessian of the :math:`\chi^2`
         """
         self.detail = {}
         self.beta, self.gamma = beta, gamma
         self.N_PAR = len(beta)
         self.rho = self.beta.copy()
-        if len(self.pull_function.VarianceModel.pars.free) != 0:
+        if self.pull_function.VarianceModel is not None and \
+                len(self.pull_function.VarianceModel.pars.free) != 0:
             self.N_PAR += len(self.gamma)
             self.rho = np.hstack((self.rho, self.gamma))
         self.sigma_kappa = sigma_kappa
         self.chi2 = 0
 
         self.model_reg(derivatives=derivatives)
         if eta_covmatrix is not None:
@@ -458,55 +459,55 @@
             return self.chi2, self.detail, self.grad, self.hess
         return self.chi2, self.detail
 
     def model_reg(self, derivatives=False):
         r"""
         - Compute the model and error snake contribution to the total :math:`\chi^2`,
         grouping all parameters under a single variable :
-        
+
         .. math::
             \rho = \left( \begin{matrix}
             \beta \\
             \gamma \\
             \sigma_\kappa
             \end{matrix}\right)
 
-        We get : 
+        We get :
 
         .. math::
          \chi^2_{model} = \ln(|V(\rho)|) + R(\rho)^T  V^{-1}(\rho) R(\rho)
-        
+
         For the gradient vector :
 
         .. math::
             \frac{\partial \chi^2_{model}(\rho)}{\partial \rho_i}  = Tr\left(V^{-1} J_{V,i} \right) -
             2 J_i^T V^{-1} R - R^T V^{-1} J_{V,i} V^{-1} R
 
         For the hessian matrix :
 
         .. math::
             H  = \frac{\partial^2 \chi^2_{model}(\rho)}{\partial \rho_i \partial \rho_j}= (H)_{ij} =
             \left( Tr\left( -V^{-1} J_{V,j} V^{-1} J_{V,i} \right) + 2  J_i^T V^{-1} J_j^T\right)_{ij}
 
-        
+
         - Compute regularization component of the total :math:`\chi^2`:
-        
+
         .. math::
             \chi^2_{reg} = \mu_{reg} \beta^T P \beta
 
         If derivatives are needed:
         adding to the total gradient :
-        
+
         .. math::
             \frac{\partial \chi^2_{reg}(\beta)}{\partial \beta}  = \mu_{reg} \rho^T P
-        
+
         and to the hessian matrix :
-        
+
         .. math::
-            \frac{\partial \chi^2_{reg}(\beta)}{\partial \beta \partial \beta} = 2 \mu_{reg} P        
+            \frac{\partial \chi^2_{reg}(\beta)}{\partial \beta \partial \beta} = 2 \mu_{reg} P
 
 
         Parameters
         ----------
         derivatives : bool
            If gradient and hessian are needed.
         """
@@ -523,62 +524,67 @@
         #        variance = self.pull_function.data['FluxErr']**2
         else:
             if len(self.gamma) != 0.:
                 pull, val = self.pull_function(self.beta, gamma=self.gamma, jac=False)
             else:
                 pull, val = self.pull_function(self.beta, jac=False)
         self.model_evaluation = time.time() - tmod
-        res = self.pull_function.data['Flux'] - val
+        # this is ugly. We're not supposed to know the internals
+        # of the pull function here - rewrite
+        # res = self.pull_function.data['Flux'] - val
+        res = self.pull_function.flux - val
         pull_tilde = pull
-        
+
         if self.regularization is not None:
             _, regularization_matrix = self.regularization(self.beta)
             if regularization_matrix.shape != (len(self.beta), len(self.beta)):
                 raise ValueError('wrong regularization matrix dimensions: regularization_matrix.shape=%r'
                                  % regularization_matrix.shape)
             fact = cholmod.cholesky(regularization_matrix.tocsc(), beta=1.E-12)
             lower_triangular_matrix = fact.L()
             pull_tilde = np.hstack((pull, lower_triangular_matrix.T.dot(self.beta)))
-        
+
         self.chi2 += pull_tilde.T.dot(pull_tilde)
-        
+
         self.detail['model'] = pull.T.dot(pull)
         if self.regularization is not None:
             regularization_triangular_matrix = lower_triangular_matrix.T.dot(self.beta)
             self.detail['reg'] = regularization_triangular_matrix.T.dot(regularization_triangular_matrix)
 
-        if len(self.pull_function.VarianceModel.pars.free) != 0:
+        if self.pull_function.VarianceModel is not None and \
+                len(self.pull_function.VarianceModel.pars.free) != 0:
             variance = self.pull_function.VarianceModel(self.gamma, self.beta)
             self.chi2 += np.log(variance).sum()
             self.detail['var_log_det'] = np.log(variance).sum()
-       
+
         if derivatives:
             if self.regularization is not None:
                 derivative_pull_tilde = scipy.sparse.bmat([[derivative_pull, None], [-lower_triangular_matrix.T, None]])
             else:
                 derivative_pull_tilde = derivative_pull
             derivative_pull_tilde = derivative_pull_tilde.tocsc()
 
             t0 = time.time()
-            if len(self.pull_function.VarianceModel.pars.free) != 0:
+            if self.pull_function.VarianceModel is not None and \
+                    len(self.pull_function.VarianceModel.pars.free) != 0:
                 w_diag = 1/variance
                 w_matrix = scipy.sparse.diags(w_diag)
                 matrix_variance_pull = (derivative_variance.tocsc().dot(w_matrix.tocsc()))
-                
+
                 self.hess = self.hessian_nr(matrix_variance_pull=matrix_variance_pull, derivative_pull=derivative_pull,
                                             derivative_pull_tilde=derivative_pull_tilde)
                 self.grad = self.grad_nr(res=res, w_diag=w_diag, matrix_variance_pull=matrix_variance_pull,
                                          pull_tilde=pull_tilde,
                                          derivative_pull_tilde=derivative_pull_tilde)
 
             else:
                 derivative_pull_tildecsr = derivative_pull_tilde.tocsr()
                 self.hess = 2 * derivative_pull_tildecsr.T.dot(derivative_pull_tildecsr)
                 self.grad = -2. * derivative_pull_tildecsr.T.dot(pull_tilde)
-                
+
             self.hessian_construction = time.time() - t0
 
     def hessian_nr(self, matrix_variance_pull, derivative_pull, derivative_pull_tilde):
         r"""
         Compute the Hessian of the simultaneous fit of the model parameters
         (beta) and th error snake parameters (gamma):
 
@@ -596,110 +602,110 @@
             parameters and the regularization cholesky decomposition term
 
         Returns
         -------
         Hessian of the model and regularization part :math:`H`
         """
         hessian0 = 2 * derivative_pull_tilde.T.dot(derivative_pull_tilde)
-         
+
         hessian = coo_matrix(hessian0)
         hessian.resize((self.N_PAR, self.N_PAR))
         hessian_csc = hessian.tocsc()
 
         ddvv = matrix_variance_pull.tocsc()
         trace_derivative_log_det_variance_hessian = -1 * (ddvv.dot(ddvv.T))
         hessian_log_det = trace_derivative_log_det_variance_hessian
         return hessian_csc + hessian_log_det
 
     def grad_nr(self, res, w_diag, matrix_variance_pull, pull_tilde, derivative_pull_tilde):
         r"""
         Compute the Gradient of the simultaneous fit of the model parameters
         (beta) and th error snake parameters (gamma):
-        
+
         .. math::
             \frac{\partial \chi^2_{model}(\rho)}{\partial \rho_i} = Tr\left( V^{-1} J_{V,i} \right) -
             2 J_i^T V^{-1}  R -  R^T  V^{-1}  J_{V,i}  V^{-1}  R
-        
-        Parameters 
+
+        Parameters
         ----------
         res : array
            Array of the model residuals.
         w_diag :
            Diagonal of the inverse of the variance matrix.
         matrix_variance_pull : scipy.sparse.csc_matrix or scipy.sparse.bmat
            Product of the derivative of the error snake wrt to beta and gamma and weight matrix, the variance inverse.
-        pull_tilde : array 
+        pull_tilde : array
            Concatenation of the pulls and the regularization cholesky decomposition term
-        derivative_pull_tilde : array 
+        derivative_pull_tilde : array
            Concatenation of the derivative of the pull wrt beta
            parameters and the regularization cholesky decomposition term
 
         Returns
         -------
         Gradient of the model and regularization part :math:`\frac{\partial \chi^2_{model}(\rho)}{\partial \rho_i}`
         """
         grad = -2. * derivative_pull_tilde.T.dot(pull_tilde)
         grad0 = np.concatenate([grad, np.zeros(self.gamma.shape)])
         trace_derivative_log_det_variance_grad = 1 * np.array(matrix_variance_pull.sum(axis=1)).ravel()
         pull_derivation_w_pull = - (matrix_variance_pull.dot((w_diag * res**2)))
         resul = grad0 - trace_derivative_log_det_variance_grad - pull_derivation_w_pull
         return resul
-            
+
     def color_scatter_evaluation(self, derivatives=False):
         r"""
         Evaluation of the color scatter \& its derivatives.
-        
+
         .. math::
             \chi^{2}_{CS}(\kappa, \sigma_\kappa) =  \ln{|V_{\kappa}( \sigma_\kappa)|} +
             \kappa^T V^{-1}_{\kappa}( \sigma_\kappa) \kappa
 
-        adding to de gradient : 
+        adding to de gradient :
 
         .. math::
             \frac{\partial \chi^2_{CS}}{\partial \kappa_i} =  2  V_{\kappa}^{-1} \kappa
-        
+
         .. math::
             \frac{\partial \chi^2_{CS}}{\partial \sigma_{\kappa,i}} =  Tr\left(V_{\kappa}^{-1}
             \frac{\partial V_{\kappa}}{\partial \sigma_{\kappa,i}} \right)	- \kappa^T V_{\kappa}^{-1}
             \frac{\partial V_{\kappa}}{\partial \sigma_{\kappa,i}} V_{\kappa}^{-1} \kappa
 
-        adding to de hessian : 
-        
+        adding to de hessian :
+
         .. math::
             \frac{\partial^2 \chi^2_{CS}}{\partial \kappa_j \partial \kappa_i} =  2  V_{\kappa}^{-1}
 
         .. math::
             \frac{\partial^2 \chi^2_{CS}}{\partial  \sigma_{\kappa,j} \partial  \sigma_{\kappa,i}} =
             -Tr\left( V_{\kappa}^{-1}  \frac{\partial V_{\kappa}}{\partial  \sigma_{\kappa,j}} V_{\kappa}^{-1}
             \frac{\partial V_{\kappa}}{\partial  \sigma_{\kappa,i}}  \right) + 2 \kappa^T V^{-1}_{\kappa}
             \frac{\partial V_{\kappa}}{\partial \sigma_{\kappa,i}} V_{\kappa}^{-1}
             \frac{\partial V_{\kappa}}{\partial \sigma_{\kappa,j}} V_{\kappa}^{-1} \kappa
-        
+
         Parameters
         ----------
         derivatives : bool
            If gradient and hessian are needed.
         """
-        sigma_kappa = self.sigma_kappa 
+        sigma_kappa = self.sigma_kappa
         # print(f'sigma_kappa : {sigma_kappa}')
-        # sig = np.polyval(sigma_kappa, self.lambda_c_red) 
+        # sig = np.polyval(sigma_kappa, self.lambda_c_red)
         if derivatives:
             sig, derivative_kappa_covmatrix = self.color_scatter(self.sigma_kappa, jac=True)  ##
             # vandermonde_matrix = np.vander(self.lambda_c_red, len(sigma_kappa)).T
-        else :  ## 
+        else :  ##
             sig = self.color_scatter(self.sigma_kappa)  ##
-            
+
         kappa = self.pull_function.model.pars['kappa_color'].full
         kappa_covmatrix = sig**2
         inv_kappa_covmatrix = 1/kappa_covmatrix
-        
+
         coomatrix_inv_kappa_covmatrix = coo_matrix(np.diag(inv_kappa_covmatrix))
         kappa_index_start = self.pull_function.model.pars['kappa_color'].indexof()[0]
         total_parameters_number = int(np.sum([self.hess.shape])/2)
-        
+
         row = kappa_index_start + coomatrix_inv_kappa_covmatrix.row
         col = kappa_index_start + coomatrix_inv_kappa_covmatrix.col
         extended_coomatrix_inv_kappa_covmatrix = coo_matrix((coomatrix_inv_kappa_covmatrix.data, (row, col)),
                                                             shape=(total_parameters_number, total_parameters_number))
 
         vc_cs = (inv_kappa_covmatrix.dot(kappa**2)).sum()
         self.chi2 += vc_cs
@@ -710,15 +716,15 @@
             self.chi2 += log_det_cs
             self.detail['CS_log_det'] = log_det_cs
 
         if derivatives:
             extended_coomatrix_inv_kappa_covmatrix = extended_coomatrix_inv_kappa_covmatrix.tocsc()
             self.hess += 2 * extended_coomatrix_inv_kappa_covmatrix
             self.grad += 2 * extended_coomatrix_inv_kappa_covmatrix.dot(self.rho)
-                
+
             if self.sigma_kappa_fit:
                 # derivative_kappa_covmatrix = (vandermonde_matrix * sig * 2).T
                 trace_derivative_log_det_kappa = 1 * inv_kappa_covmatrix.dot(derivative_kappa_covmatrix)
                 kappa_derivative_covmatrix_kappa = -1 * derivative_kappa_covmatrix.T.dot(
                     (inv_kappa_covmatrix * kappa)**2
                 )
 
@@ -729,33 +735,33 @@
                 double_product_derivative_covmatrix_kappa = 2*(derivative_covmatrix * inv_kappa_covmatrix).dot(
                     derivative_covmatrix.T
                 )
                 hess_kappa = coo_matrix(double_trace_log_det_kappa + double_product_derivative_covmatrix_kappa)
                 hess_coo = self.hess.tocoo()
 
                 hessian_combinaison = scipy.sparse.bmat([[hess_coo, None], [None, hess_kappa]], format='csc')
-                
+
                 self.grad = np.hstack((self.grad, grad_kappa))
                 self.hess = hessian_combinaison
-                
+
     def calibration_gaussian_prior(self, eta_covmatrix, derivatives=False):
-        r"""        
-        Compute calibration propagation component of the total :math:`\chi^2`:                          
+        r"""
+        Compute calibration propagation component of the total :math:`\chi^2`:
 
-        .. math::          
+        .. math::
             \chi^2_{calib} = \eta^T V_{\eta}^{-1} \eta
 
         If derivatives are needed:
-        adding to de gradient : 
-        
+        adding to de gradient :
+
         .. math::
             \frac{d \chi^2_{calib}}{d\eta} = V_{\eta}^{-1} \eta
 
-        adding to de hessian : 
-        
+        adding to de hessian :
+
         .. math::
            \frac{d^2 \chi^2_{calib}}{d\eta^2} =  V_{\eta}^{-1}
 
         Parameters
         ----------
         eta_covmatrix : float or array
            Calibration uncertainty matrix.
@@ -778,49 +784,49 @@
 
         row = eta_index_start + inv_coomatrix_eta_covmatrix.row
         col = eta_index_start + inv_coomatrix_eta_covmatrix.col
 
         extended_inv_cscmatrix_eta_covmatrix = coo_matrix((inv_coomatrix_eta_covmatrix.data, (row, col)),
                                                           shape=(self.N_PAR, self.N_PAR)).tocsc()
         v_eta = (extended_inv_cscmatrix_eta_covmatrix.dot(self.rho**2)).sum()
-        
+
         self.chi2 += v_eta
         self.detail['C_eta'] = v_eta
 
         if derivatives:
             self.hess += 2 * extended_inv_cscmatrix_eta_covmatrix
             self.grad += 2 * extended_inv_cscmatrix_eta_covmatrix @ self.rho
 
     def get_constrains_derivatives(self, derivatives=False):
         r"""
         Evaluate the constrains :math:`C(\beta)` contribution the the :math:`\chi^2` as a quadratic penalty:
 
-        .. math::                                                                                       
+        .. math::
             \chi^2_{cons} = \mu_{pen} C(\beta)^T C(\beta)
-            
+
         If derivatives are needed:
-        adding to de gradient : 
-        
+        adding to de gradient :
+
         .. math::
             \frac{d \chi^2_{cons}}{d\beta} = 2 \mu_{pen} \frac{\partial C(\beta)}{\partial \beta_i}^T C(\beta)
-        
-        adding to de hessian : 
-        
+
+        adding to de hessian :
+
         .. math::
             \frac{d^2 \chi^2_{cons}}{d\beta^2} = 2 \mu_{pen} \left(\frac{\partial^2
             C(\beta)}{\partial \beta_j \partial \beta_i}^T C(\beta) +
             \frac{\partial C(\beta)}{\partial \beta_i}^T \frac{\partial C(\beta)}{\partial \beta_j} \right)
 
         Parameters
         ----------
         derivatives : bool
            If gradient and hessian are needed.
         """
         con = self.constrains(self.beta, jac=False)
-        
+
         self.chi2 += (con**2).sum()
         self.detail['cons_qua'] = (con**2).sum()
         if len(self.pull_function.model.pars['X1'].free) != 0.:
             if derivatives:
                 p_free = self.pull_function.VarianceModel.pars.free
                 vcons, jacobian_cons, hessian_cons = self.constrains.var_x1(self.beta,
                                                                             gamma=p_free,
@@ -828,15 +834,15 @@
                 self.hess += hessian_cons.tocsc()
                 self.grad += jacobian_cons
 
             else:
                 vcons = self.constrains.var_x1(self.beta, jac=False)
             self.chi2 += vcons**2
             self.detail['x1_cons'] = vcons**2
-            
+
         if derivatives:
             v, bloc_hessian_cons = self.constrains(self.beta, jac=True)
             if len(self.gamma) != 0.:
                 bloc_hessian_cons.resize((bloc_hessian_cons.shape[0], self.N_PAR))
             self.hess += (2 * bloc_hessian_cons.T.dot(bloc_hessian_cons)).tocsc()
             self.grad -= 2 * bloc_hessian_cons.T.dot(v)
 
@@ -853,66 +859,78 @@
     .. note: ModelResiduals() should be able to accept either a model or a variance model !
     .. note: shorter code if model() could have the same signature regardless of jac=True or not
 
     Attributes
     ----------
     training_dataset : nacl.dataset.TrainingDataset
         Data set of photometric and spectroscopic observations.
-    idxlc : int 
+    idxlc : int
         Index where light curve data finish and spectra data starts.
-    data : array 
+    data : array
         Data point array.
     N : int
         Number of data point.
     model : nacl.salt.
         Model
     chi2_normalization : None or float
         Normalization between modelization of photometric and spectroscopic datat
         :math:`\chi^2_{photo}` and :math:`\chi^2_{spectro}`.
     VarianceModel : None or nacl.models.variancemodels
-        Variance model, error snake integration.      
+        Variance model, error snake integration.
     pars : FitParameters
         Model parameters.
     """
-    
+
     def __init__(self, model, variance_model=None, chi2_normalization=None, fit_spec=True):
         r"""
         Model pull initialisation.
 
         Parameters
         ----------
         model : nacl.models.salt
             Model.
         chi2_normalization : None or float
             Normalization between modelization of photometric and spectroscopic datat
             :math:`\chi^2_{photo}` and :math:`\chi^2_{spectro}`.
         variance_model : None or nacl.models.variancemodels
-            Variance model, error snake integration.      
+            Variance model, error snake integration.
         fit_spec : bool
             If spectroscopic data are fitted.
         """
         self.training_dataset = model.training_dataset
-        self.idxlc = len(self.training_dataset.lc_data) 
+        self.idxlc = len(self.training_dataset.lc_data)
         if fit_spec:
-            self.data = np.hstack((self.training_dataset.lc_data, self.training_dataset.spec_data))
+            self.flux = np.hstack((self.training_dataset.lc_data.flux,
+                                  self.training_dataset.spec_data.flux))
+            self.fluxerr = np.hstack((self.training_dataset.lc_data.fluxerr,
+                                     self.training_dataset.spec_data.fluxerr))
+            # self.data = np.hstack((self.training_dataset.lc_data,
+            #                        self.training_dataset.spec_data))
         else:
-            self.data = self.training_dataset.lc_data
-        self.N = len(self.data)
+            self.flux = self.training_dataset.lc_data.flux
+            self.fluxerr = self.training_dataset.lc_data.fluxerr
+            # self.data = self.training_dataset.lc_data
+        self.N = len(self.flux)
         self.model = model
-
         self.chi2_normalization = chi2_normalization
+        # the code line below are rather strange.
+        # I think the reason it is written that way is that Guy was working
+        # with several parameter vectors. Now, all the parameters have beem
+        # grouped into a single vector.
+        # TODO: rewrite
+        self.VarianceModel = None
         if variance_model is not None:
             self.VarianceModel = variance_model
         else:
             self.pars = model.pars
 
     def __call__(self, beta, gamma=[], jac=True):
         r"""
         Evaluation of the pull.
-        
+
         Parameters
         ----------
         beta : array
            Model parameters.
         gamma : array
            Error snake parameters.
         jac : bool
@@ -939,45 +957,47 @@
         derivative_variance : scipy.sparse.coo_matrix or None
             Error snake derivative evaluation.
         """
         if jac:
             v, jacobian = self.model(beta, jac=True)
         else:
             v = self.model(beta, jac=False)
-            
-        res = self.data['Flux'] - v
+
+        # res = self.data['Flux'] - v
+        res = self.flux - v
 
         if len(gamma) != 0:
             variance = self.VarianceModel(gamma, beta)
         else:
-            variance = self.data['FluxErr']**2
+            # variance = self.data['FluxErr']**2
+            variance = self.fluxerr**2
 
         ww = 1/np.sqrt(variance)
-            
+
         if self.chi2_normalization is None:
             chi2_normalization = len(self.training_dataset.lc_data)/len(self.training_dataset.spec_data)
         else:
             chi2_normalization = self.chi2_normalization
-            
+
         #print(f'chi2_normalization = {chi2_normalization}')
-        ww[self.idxlc:] *= np.sqrt(chi2_normalization)        
+        ww[self.idxlc:] *= np.sqrt(chi2_normalization)
 
         if len(variance.shape) == 1:
             w = scipy.sparse.dia_matrix((ww, [0]), shape=(self.N, self.N))
         else:
             w = scipy.sparse.csc_matrix(ww)
 
         w_res = w @ res
         if jac:
             w_jac = w @ jacobian  # -w @ jacobian #moins
-            
+
             if len(gamma) != 0:
                 variance, derivative_variance = self.VarianceModel(gamma, beta, jacobian=jacobian.tocoo())
                 return w_res, w_jac, v, jacobian, variance, derivative_variance
             else:
                 return w_res, w_jac, v, jacobian, variance, None
-        
+
         if np.isnan(w@res).sum() > 0.:
             raise ValueError('There are np.nan in w@res')
         if np.isinf(w@res).sum() > 0.:
             raise ValueError('There are np.inf in w@res')
         return w_res, v
```

### Comparing `sn-nacl-0.3/nacl/models/regularizations.py` & `sn-nacl-0.4/nacl/models/regularizations.py`

 * *Files 23% similar despite different names*

```diff
@@ -24,20 +24,127 @@
     0 & P_{\theta_{0|1}} & 0 & 0\\
     0 & 0 & P_{\theta_{0|1}} & 0\\
     0 & 0 & 0 & 0
     \end{array}
     \right)
     \end{equation}
 
-The matrix :math:`P_{\theta_{0|1}}` is defined in the different regularization class.
+The matrix :math:`P_{\theta_{0|1}}` is defined in the different
+regularization class.
 """
 
 import numpy as np
-from scipy.sparse import coo_matrix, dia_matrix, csc_matrix
-    
+from scipy.sparse import coo_matrix, dia_matrix, csc_matrix, dok_matrix
+
+
+
+# this is a minimal rewrite of the original class SplineRegul2D by Guy
+# to simplify it (we can condense both regulization inside one single class
+# and also to adapt it to the interface expected by the LogLikelihood class.
+
+class SplineRegularization:
+    """
+    """
+    def __init__(self, model, to_regularize=None, mu=1.E-6):
+        """
+        """
+        self.model = model
+        self.pars = self.model.pars
+        self.to_regularize = to_regularize
+        if to_regularize is None:
+            self.to_regularize = ['M0', 'M1']
+        self.mu = mu
+        # we call it P_full, to remind us that it regularizes all
+        # the parameters (free and fixed) of the selected blocks
+        self.P_full = self._init_regularization_matrices()
+
+    def _init_regularization_matrices(self):
+        raise NotImplementedError('SplineRegularization is pure virtual')
+
+    def get_free_mat(self):
+        n = len(self.model.pars.full)
+        assert n == self.P_full.shape[0]
+        idx = self.model.pars.indexof(np.arange(n)) >= 0
+        return self.P_full[:,idx][idx,:]
+
+    def __call__(self, p, deriv=False):
+        """
+        """
+        self.model.pars.free = p
+
+        full_pars = self.model.pars.full
+        penality = full_pars.T @ self.P_full @ full_pars
+        if not deriv:
+            return self.mu * penality
+
+        # gradient of the free parameters
+        n = self.P_full.shape[0]
+        idx = self.model.pars.indexof(np.arange(n)) >= 0
+        grad = -2. * (self.P_full @ full_pars)[idx]
+
+        # and finally, the hessian (needs to be sliced also)
+        if idx.sum() > 0:
+            P = self.P_full[:,idx][idx,:]
+        else:
+            P = self.P_full
+        hess = 2. * P
+
+        mu = self.mu
+
+        return mu * penality, mu * grad, mu * hess
+
+
+def get_naked_regularization_matrix(size, order=0):
+    """
+    """
+    if order == 0:
+        data = np.ones(size)
+        return dia_matrix((data, [0]), shape=(size,size)).tocoo()
+
+    data = np.vstack(([3.] * size, [-1.] * size, [-1.] * size))
+    data[0, 0] = data[0, -1] = 2.
+    mat = dia_matrix((data, [0, -1, 1]), shape=(size,size)).tocoo()
+    return mat
+
+
+class NaClSplineRegularization(SplineRegularization):
+
+    def __init__(self, model, to_regularize=None, mu=1.E-6, order=1):
+        """
+        """
+        self.order = order
+        super(NaClSplineRegularization, self).__init__(model, to_regularize, mu)
+
+    def _init_regularization_matrices(self):
+        """Build a NaCl regularization matrix
+        """
+        pars_full = self.model.pars.copy()
+        pars_full.release()
+        npars = len(pars_full.full)
+
+        P_full = dok_matrix((npars,npars))
+
+        for block_name in self.to_regularize:
+            block_pars = pars_full[block_name].full
+            block_size = len(block_pars)
+            mat = get_naked_regularization_matrix(block_size, order=self.order)
+
+            # full matrix (used to compute the regularization value)
+            i = pars_full[block_name].indexof(mat.row)
+            j = pars_full[block_name].indexof(mat.col)
+            P_full += coo_matrix((mat.data, (i,j)), shape=(npars,npars))
+
+            # i = pars[block_name].indexof(mat.row)
+            # j = pars[block_name].indexof(mat.col)
+            # idx = (i >= 0) & (j >= 0)
+            # P_free += coo_matrix((mat.data[idx], (i[idx], j[idx])),
+            #                      shape=(n_free_pars, n_free_pars))
+
+        return P_full
+
 
 class SplineRegul2D(object):
     r"""
     This regularization focuses on the model variations in phase.
     The density of spectra allows the basis to be constrained correctly, and the density of points
     on the spectra seems to limit the oscillation phenomena.
 
@@ -100,15 +207,15 @@
             data = np.vstack(([3.] * n, [-1.] * n, [-1.] * n))
             data[0, 0] = data[0, -1] = 2.
             idx_data = [0, -1, 1]
         else:
             # only diagonal term
             data = np.ones(n).astype(float)
             idx_data = [0]
-            
+
         matrix = dia_matrix((data, idx_data), shape=(n, n)).tocoo()
         # embed it in a larger matrix, that corresponds to the model parameters
         n_pars = len(self.pars.free)
         i = self.pars['M0'].indexof(matrix.row)
         j = self.pars['M0'].indexof(matrix.col)
         idx = (i >= 0) & (j >= 0)
         matrix_free0 = coo_matrix((matrix.data[idx]*self.mu, (i[idx], j[idx])), shape=(n_pars, n_pars))
@@ -119,15 +226,15 @@
                 data1 = np.vstack(([3.] * n1, [-1.] * n1, [-1.] * n1))
                 data1[0, 0] = data1[0, -1] = 2.
                 idx_data1 = [0, -1, 1]
             else:
                 # only diagonal term
                 data1 = np.ones(n1).astype(float)
                 idx_data1 = [0]
-                
+
             matrix_1 = dia_matrix((data1, idx_data1), shape=(n1, n1)).tocoo()
             i1 = self.pars['M1'].indexof(matrix_1.row)
             j1 = self.pars['M1'].indexof(matrix_1.col)
             idx1 = (i1 >= 0) & (j1 >= 0)
             matrix_free1 = coo_matrix((matrix_1.data[idx1]*self.mu, (i1[idx1], j1[idx1])), shape=(n_pars, n_pars))
             self.matrix_free = (matrix_free0 + matrix_free1)
         else:
@@ -206,22 +313,22 @@
         self.model = model
         self.pars = model.pars.copy()
         self.mu = mu
 
         self.ph1_range, self.wl1_range, self.N_eff = None, None, None
 
         self.surfaces_reg = surfaces_reg
-        
+
         self.wl_range = np.linspace(self.model.wl_range[0], self.model.wl_range[1],
-                                    self.model.basis.bx.nj) 
+                                    self.model.basis.bx.nj)
         self.ph_range = np.linspace(self.model.phase_range[0], self.model.phase_range[1],
                                     self.model.basis.by.nj)
-        
+
         self.SP = self.model.training_dataset.spec_data
-        # build the regularization matrix for the spline parameters                                     
+        # build the regularization matrix for the spline parameters
 
     def calculate_n_eff(self):
         """
         Calculate the number of data point per bin of wavelength and phase.
         """
         yy_sp, xx_sp = [], []
         bins = self.wl_range
@@ -261,24 +368,24 @@
         self.calculate_n_eff()
 
         x, y = np.meshgrid(self.wl_range, self.ph_range)
         model_eval = self.model.basis.eval(x.ravel(), y.ravel())
         jacobian_model_eval_wavelength, jacobian_model_eval_phase = self.model.basis.gradient(x.ravel(), y.ravel())
 
         _, _, hessian_model_eval_phase = self.model.basis.hessian(x.ravel(), y.ravel())
-        
+
         ddiag = jacobian_model_eval_wavelength * jacobian_model_eval_phase - model_eval * hessian_model_eval_phase
-        
+
         jacobian_model_eval_phase.data *= jacobian_model_eval_phase.data * self.mu * 0.75/1000  # diff or not
         jacobian_model_eval_wavelength.data *= jacobian_model_eval_wavelength.data * self.mu
         jacobian_model_eval_phase.data /= self.N_eff.ravel()[jacobian_model_eval_phase.row]
         jacobian_model_eval_wavelength.data /= self.N_eff.ravel()[jacobian_model_eval_wavelength.row]
 
         ddiag.data *= self.mu/self.N_eff.ravel()[ddiag.tocoo().row]  # diff or not
-        
+
         matrix = (jacobian_model_eval_phase + jacobian_model_eval_wavelength + ddiag)
         matrix = matrix.tocoo()
         n_pars = len(self.pars.free)
         matrix_free = coo_matrix((np.zeros_like(matrix.data), (matrix.row, matrix.col)), shape=(n_pars, n_pars))
 
         if 'M0' in self.surfaces_reg:
             i = self.pars['M0'].indexof(matrix.row)
```

### Comparing `sn-nacl-0.3/nacl/models/salt.py` & `sn-nacl-0.4/nacl/models/salt.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,154 +1,165 @@
 #!/usr/bin/python
 
 ####
 # Re-implementation of the original SALT2 model.
 ####
 
+import logging
 import time
+
 import numpy as np
 import scipy.sparse
 
-from ..lib.fitparameters import FitParameters
-from ..lib import bspline
+try:
+    from sksparse.cholmod import cholesky_AAt
+except ImportError:
+    from scikits.sparse.cholmod import cholesky_AAt
+
 from ..instruments import FilterDb
-import logging
+from ..lib import bspline
+from ..lib.fitparameters import FitParameters
+from ..lib.instruments import MagSys
+from . import variancemodels as vm
+
+from nacl.dataset import SimTrainingDataset
+
+
 logging.basicConfig(format='%(asctime)s %(levelname)s %(message)s',
                     level=logging.INFO)
 
 
-class ColorLaw(object):
-    r"""Implementation of the SALT2 color law (version 1) 
+class ColorLaw:
+    r"""Implementation of the SALT2 color law (version 1)
 
-    The SALT2 color law describes the color diversity of SNeIa. In
-    SALT 2.4, the color law is parametrized as follows:
-    
-    .. math::
-        CL(\lambda;c) = 10^{0.4\ c \times P(\lambda_r)}
+        The SALT2 color law describes the color diversity of SNeIa. In SALT 2.4, the
+        color law is parametrized as follows:
 
-    where :math:`P(\lambda_r)` is a polynomial, such as
-    :math:`P(\lambda_B) = 0` and :math:`P(\lambda_V) = 1`.
+        .. math::
+            CL(\lambda;c) = 10^{0.4\ c \times P(\lambda_r)}
 
-    This implies the following transformation :
+        where :math:`P(\lambda_r)` is a polynomial, such as :math:`P(\lambda_B) = 0`
+        and :math:`P(\lambda_V) = 1`.
 
-    .. math::
-        \lambda_r = \frac{\lambda-\lambda^B}{\lambda^V - \lambda^B}
+        This implies the following transformation :
+
+        .. math::
+            \lambda_r = \frac{\lambda-\lambda^B}{\lambda^V - \lambda^B}
 
-    It is defined in the wavelength range :math:`2800 A < \lambda < 7000 A`
-    and extrapolated with a linear function outside this interval.
+        It is defined in the wavelength range :math:`2800 A < \lambda < 7000 A` and
+        extrapolated with a linear function outside this interval.
 
-    This class evaluates :math:`P(\lambda, \alpha_i)` and its
-    derivatives :math:`\partial P/\partial \alpha_i` (which is the
-    painful part).
+        This class evaluates :math:`P(\lambda, \alpha_i)` and its derivatives
+        :math:`\partial P/\partial \alpha_i` (which is the painful part).
 
-    Attributes
-    ----------
-    min_lambda : float
-        Lower value of the wavelength interval
-    max_lambda : float
-        Upper value of the wavelength interval
-    min_reduced_lambda : float
-        Lower value of the reduce wavelength interval
-    max_reduced_lambda : float
-        Upper value of the reduce wavelength interval
-    pars : array
-        Color law polynomial parameters
-    pars_ir :
-        Parameters of the IR affine extension
-    pars_uv
-        Parameters of the UV affine extension
+        Attributes
+        ----------
+        min_lambda : float
+            Lower value of the wavelength interval
+        max_lambda : float
+            Upper value of the wavelength interval
+        min_reduced_lambda : float
+            Lower value of the reduce wavelength interval
+        max_reduced_lambda : float
+            Upper value of the reduce wavelength interval
+        pars : array
+            Color law polynomial parameters
+        pars_ir :
+            Parameters of the IR affine extension
+        pars_uv
+            Parameters of the UV affine extension
     """
     WAVELENGTH = {"U": 3650.88, "B": 4302.57, "V": 5428.55, "R": 6418.01, "I": 7968.34}
     U_WAVELENGTH = 3650.88
     B_WAVELENGTH = 4302.57
     V_WAVELENGTH = 5428.55
     R_WAVELENGTH = 6418.01
     I_WAVELENGTH = 7968.34
 
     def __init__(self, wl_range=[2800, 7000]):
         """
-        Constructor - computes the arguments
+            Constructor - computes the arguments
 
-        Parameters
-        ----------
-        wl_range : list or ndarray
-            nominal wavelength range for the polynom color law.
-            Outside this range, we don't expect to have valid data
-            and the color law is extrapolated with deg-1 polynomials.
+            Parameters
+            ----------
+            wl_range : list or ndarray
+                nominal wavelength range for the polynom color law.
+                Outside this range, we don't expect to have valid data
+                and the color law is extrapolated with deg-1 polynomials.
         """
-        assert(wl_range[0] < wl_range[1])
+        assert (wl_range[0] < wl_range[1])
         self.min_lambda, self.max_lambda = wl_range
-        
+
         self.min_reduced_lambda = self.reduce(self.min_lambda)
         self.max_reduced_lambda = self.reduce(self.max_lambda)
         self.pars = np.zeros(5)
 
     def reduce(self, wl):
-        r"""Linear remapping of the wavelength passed in argument. 
-        
-        The remapping is defined by:
+        r"""Linear remapping of the wavelength passed in argument.
 
-        .. math::
-            \lambda_r = \frac{\lambda - \lambda_B}{\lambda_V - \lambda_B}
+            The remapping is defined by:
 
-        Parameters
-        ----------
-        wl : array-like
-            the input wavelengths in Angstroms
+            .. math::
+                \lambda_r = \frac{\lambda - \lambda_B}{\lambda_V - \lambda_B}
 
-        Returns
-        ----------
-        array of floats
-            the reduced wavelengths
+            Parameters
+            ----------
+            wl : array-like
+                the input wavelengths in Angstroms
+
+            Returns
+            ----------
+            array of floats
+                the reduced wavelengths
         """
         B_WL, V_WL = self.WAVELENGTH["B"], self.WAVELENGTH["V"]
         return (wl-B_WL)/(V_WL-B_WL)
-    
-    def __call__(self, wl, p, jac=False):  #  , return_jacobian_as_coo_matrix=False):
-        r"""Evaluate the polynomial part of the color law 
-        
-        The full SALT2 color law is given by:
 
-        .. math::
-            CL(\lambda, c) = 10^{0.4\ c\ P(\lambda, \alpha_i)}
+    def __call__(self, wl, p, jac=False):  # return_jacobian_as_coo_matrix=False):
+        r"""Evaluate the polynomial part of the color law
 
-        with 
+            The full SALT2 color law is given by:
 
-        .. math::
-            P(\lambda) = \left\{ \begin{split}
-            P'(\bar\lambda_{UV}) \times (\bar\lambda-\bar\lambda_{UV}) + P(\bar\lambda_{UV})
-            & \ \ \ \ \mathrm{if \lambda < \lambda_{UV}} \\
-            \bar\lambda \times \left(\sum_{i=1}^4 \alpha_i \bar\lambda^i + 1 - \sum_{i=1}^4\alpha_i\right)
-            & \ \ \ \ \mathrm{if \lambda_{UV} < \lambda < \lambda_{IR}} \\
-            P'(\bar\lambda_{IR}) \times (\bar\lambda-\bar\lambda_{IR}) + P(\bar\lambda_{IR})
-            & \ \ \ \ \mathrm{if \lambda > \lambda_{IR}} \\
-            \end{split}\right.
-
-        and :math:`\lambda_r` defined above.
-        
-        This function evaluates :math:`P(\lambda,\alpha_i)` along with its derivatives w.r.t. the :math:`\alpha_i`:
-        :math:`\partial P/\partial \alpha_i`
-        
-        Parameters
-        ----------
-        wl : ndarray of float
-            input wavelengths (in Angstroms)
-        p : ndarray
-            color law parameters (i.e. the :math:`(\alpha_i)_{1\leq i \leq 4}`)
-        jac : bool (default=False)
-            whether to return the jacobian matrix
-        return_jacobian_as_coo_matrix : bool 
-            If jacobian needs to be scipy.sparse
+            .. math::
+                CL(\lambda, c) = 10^{0.4\ c\ P(\lambda, \alpha_i)}
 
-        Returns
-        ----------
-        cl : array-like of float
-            the color law values
-        jacobian : numpy.array or scipy.sparse.csr_matrix (return_jacobian_as_coo_matrix)
-            the matrix of derivatives, if `jac` is True
+            with
+
+            .. math::
+                P(\lambda) = \left\{ \begin{split}
+                P'(\bar\lambda_{UV}) \times (\bar\lambda-\bar\lambda_{UV}) + P(\bar\lambda_{UV})
+                & \ \ \ \ \mathrm{if \lambda < \lambda_{UV}} \\
+                \bar\lambda \times \left(\sum_{i=1}^4 \alpha_i \bar\lambda^i + 1 - \sum_{i=1}^4\alpha_i\right)
+                & \ \ \ \ \mathrm{if \lambda_{UV} < \lambda < \lambda_{IR}} \\
+                P'(\bar\lambda_{IR}) \times (\bar\lambda-\bar\lambda_{IR}) + P(\bar\lambda_{IR})
+                & \ \ \ \ \mathrm{if \lambda > \lambda_{IR}} \\
+                \end{split}\right.
+
+            and :math:`\lambda_r` defined above.
+
+            This function evaluates :math:`P(\lambda,\alpha_i)` along with its derivatives w.r.t. the :math:`\alpha_i`:
+            :math:`\partial P/\partial \alpha_i`
+
+            Parameters
+            ----------
+            wl : ndarray of float
+                input wavelengths (in Angstroms)
+            p : ndarray
+                color law parameters (i.e. the :math:`(\alpha_i)_{1\leq i \leq 4}`)
+            jac : bool (default=False)
+                whether to return the jacobian matrix
+            return_jacobian_as_coo_matrix : bool
+                If jacobian needs to be scipy.sparse
+
+            Returns
+            ----------
+            cl : array-like of float
+                the color law values
+            jacobian : numpy.array or scipy.sparse.csr_matrix (return_jacobian_as_coo_matrix)
+                the matrix of derivatives, if `jac` is True
         """
         self.pars[0:4] = p
         self.pars[4] = 1 - p.sum()
         d_pars = np.polyder(self.pars)
 
         # nominal range
         rwl = self.reduce(np.asarray(wl))
@@ -159,15 +170,15 @@
         has_uv_data = idx_uv.sum() > 0
         if has_uv_data:
             val = np.polyval(self.pars, self.min_reduced_lambda)
             d_val = np.polyval(d_pars, self.min_reduced_lambda)
             self.pars_uv = np.asarray([d_val * self.min_reduced_lambda + val,
                                        val * self.min_reduced_lambda])
             r[idx_uv] = np.polyval(self.pars_uv, rwl[idx_uv]-self.min_reduced_lambda)
-        
+
         # ir side
         idx_ir = rwl > self.max_reduced_lambda
         has_ir_data = idx_ir.sum() > 0
         if has_ir_data:
             val = np.polyval(self.pars, self.max_reduced_lambda)
             d_val = np.polyval(d_pars, self.max_reduced_lambda)
             self.pars_ir = np.asarray([d_val * self.max_reduced_lambda + val,
@@ -177,310 +188,331 @@
         if not jac:
             return r, None
 
         # the jacobian is unfortunately a dense matrix
         # (maybe we should try using splines)
         #
         # In the nominal wavelength range, it has the form:
-        # 
+        #
         #   [l_1**5-l_1   l_1**4-l1    l_1**3-l1  l_1**2-l1]
         #   [  ...          ...           ...       ...    ]
         #   [l_N**5-l_1   l_N**4-l1    l_N**3-l1  l_N**2-l1]
-        # 
+        #
         v = np.vander(rwl, 6)[:, 0:-2]
         jacobian = (v.T-rwl).T
 
-        # 
+        #
         # and in the extrapolation range, it has the form:
         #
         # J_ik = [dCL'/da_k(rwl-rwl_uv) + dCL/da_k]
         #
-        # Granted, it's not very readable. But it should be fast enough 
+        # Granted, it's not very readable. But it should be fast enough
         if has_uv_data:
             l_uv = self.min_reduced_lambda
             j1_luv = (np.vander([l_uv], 6)[:, 0:-2].T - np.array([l_uv])).T
             j2_luv = np.vander([l_uv], 5)[:, 0:-1] * np.array([5., 4., 3., 2.]) - 1.
             n_uv = idx_uv.sum()
             jacobian[idx_uv] = j2_luv * (rwl[idx_uv]-l_uv).reshape(n_uv, -1) + j1_luv * np.ones(n_uv).reshape(n_uv, -1)
-            
+
         if has_ir_data:
             l_ir = self.max_reduced_lambda
             j1_lir = (np.vander([l_ir], 6)[:, 0:-2].T - np.array([l_ir])).T
             j2_lir = np.vander([l_ir], 5)[:, 0:-1] * np.array([5., 4., 3., 2.]) - 1.
             n_ir = idx_ir.sum()
             jacobian[idx_ir] = j2_lir * (rwl[idx_ir]-l_ir).reshape(n_ir, -1) + j1_lir * np.ones(n_ir).reshape(n_ir, -1)
 
         # check for nan's and inf's
         if np.any(np.isnan(r)) or np.any(np.isinf(r)):
             raise ValueError('inf/nan values in color law')
 
-        #if return_jacobian_as_coo_matrix:
+        #
+        # if return_jacobian_as_coo_matrix:
         #    jacobian = scipy.sparse.coo_matrix(jacobian)
-        
+
         return r, jacobian
-    
+
 
 class SpectrumRecalibrationPolynomials:
     r"""A class to manage the spectrum recalibration polynomials
-    The photometric calibration of spectra is generally affected by significant
-    error modes at large wavelength scales.
-    It is imperative to remove these error modes, while preserving the information provided by
-    the spectra at small scales (spectral features)
-
-    This is achieved during training by multiplying the spectral predictions of the model by a
-    recalibration polynomial specific to each spectrum, function of the observation
-    wavelength :math:`\lambda_o`, and of order :math:`N_s = 3`, common to all spectra:
+        The photometric calibration of spectra is generally affected by significant
+        error modes at large wavelength scales.
+        It is imperative to remove these error modes, while preserving the information provided by
+        the spectra at small scales (spectral features)
+
+        This is achieved during training by multiplying the spectral predictions of the model by a
+        recalibration polynomial specific to each spectrum, function of the observation
+        wavelength :math:`\lambda_o`, and of order :math:`N_s = 3`, common to all spectra:
 
-    .. math::
-
-        s(\lambda_{rec}) = \sum_i^{N_s} s_i \lambda_{rec}^{N_s - i} %quad \mbox{and}
-        \quad \lambda_{0} = \frac{\lambda - 5000}{9000 - 2700}
+        .. math::
 
-    with:
+            s(\lambda_{rec}) = \sum_i^{N_s} s_i \lambda_{rec}^{N_s - i} %quad \mbox{and}
+            \quad \lambda_{0} = \frac{\lambda - 5000}{9000 - 2700}
 
-    .. math::
-        \lambda_{rec} = \frac{2 (\lambda_o - \lambda_{max})}{\lambda_{max} - \lambda_{min}+1
+        with:
 
-    Attributes
-    ----------
-    tds : nacl.dataset.TrainingDataset
-        Data set of photometric and spectroscopic observations.
-    model : nacl.model.salt
-        Model.
-    pol_degrees : int or indexable structure
-        Polynomial degree for each spectrum.
-    N : int
-        Number of spectral data point.
-    offset : numpy.array
-        Starting point of parameter index for each spectrum.
-    n : int
-        Number of recalibration parameters
-    jacobian : scipy.sparse.coo_matrix
-        Jacobian matrix of the recalibration polynomial functions.
-    """
-    def __init__(self, tds, model, pol_degrees):
-        """Constructor 
+        .. math::
+            \lambda_{rec} = \frac{2 (\lambda_o - \lambda_{max})}{\lambda_{max} - \lambda_{min}+1
 
-        Parameters
+        Attributes
         ----------
         tds : nacl.dataset.TrainingDataset
             Data set of photometric and spectroscopic observations.
         model : nacl.model.salt
             Model.
         pol_degrees : int or indexable structure
             Polynomial degree for each spectrum.
-        """
+        N : int
+            Number of spectral data point.
+        offset : numpy.array
+            Starting point of parameter index for each spectrum.
+        n : int
+            Number of recalibration parameters
+        jacobian : scipy.sparse.coo_matrix
+            Jacobian matrix of the recalibration polynomial functions.
+    """
+
+    def __init__(self, tds, model, pol_degrees):
+        """Constructor
+
+           Parameters
+           ----------
+            tds : nacl.dataset.TrainingDataset
+                Data set of photometric and spectroscopic observations.
+            model : nacl.model.salt
+                Model.
+            pol_degrees : int or indexable structure
+                Polynomial degree for each spectrum.
+            """
         self.tds = tds
         self.model = model
         self.pol_degrees = pol_degrees
         self.jacobian = None
-        
-        self.N = len(self.tds.sp_data)
+
+        self.N = len(self.tds.spec_data)
         o = np.cumsum(np.hstack(([0], self.pol_degrees+1)))
         self.offset, self.n = o[:-1], o[-1]
         self.build_jacobian_matrix()
-        
 
     def init_pars(self):
-        """
-        return a parameter vector initialized such that
-        the recalibration polynomials are evaluated to 1
-        for each spectra.
-
-        Returns
-        -------
-        array
-            Initiated parameters.
+        """return a parameter vector initialized such that
+            the recalibration polynomials are evaluated to 1
+            for each spectra.
+
+            Returns
+            -------
+            array
+                Initiated parameters.
         """
         p = np.zeros(self.n)
-        o = np.cumsum(self.pol_degrees+1)
+        o = np.cumsum(self.pol_degrees+1) - 1
         p[o] = 1.
         return p
-        
+
     def build_jacobian_matrix(self):
         """
-        Create the jacobian matrix where line correspond to all spectral data point and
-        the colones to parameters.
-        """
+            Create the jacobian matrix where line correspond to all spectral data point and
+            the colones to parameters.
+            """
         i, j, v = [], [], []
 
-        for isp in range(self.tds.nb_spectra()):
-            # for sp in self.tds.spectra:
-            idx_sp = self.tds.spec_data['spec_id'] == isp
-            sp = self.tds.spec_data[idx_sp]
-            sli = np.where(idx_sp)[0]
-            slc = slice(sli.min(), sli.max()+1)
-
-            lmin, lmax = sp['Wavelength'].min(), sp['Wavelength'].max()
+        # easier to write this with the spectra index
+        for sp in self.tds.spectra:
+            spec_index = sp.spec_index[0]
+            lmin, lmax = sp.wavelength.min(), sp.wavelength.max()
             a = 2. / (lmax-lmin)
             b = 1 - 2. * lmax / (lmax-lmin)
-            rwl = a * sp['Wavelength'] + b
-            deg = self.pol_degrees[isp]
+            rwl = a * sp.wavelength + b
+            deg = self.pol_degrees[spec_index]
             jacobian_spec_rec = scipy.sparse.coo_matrix(np.vander(rwl, deg+1))
-            i.append(jacobian_spec_rec.row + slc.start)
-            j.append(jacobian_spec_rec.col + self.offset[isp])
+            i.append(jacobian_spec_rec.row + sp.slc.start)
+            j.append(jacobian_spec_rec.col + self.offset[spec_index])
             v.append(jacobian_spec_rec.data)
-
         i = np.hstack(i)
         j = np.hstack(j)
         v = np.hstack(v)
         self.jacobian = scipy.sparse.coo_matrix((v, (i, j)), shape=(self.N, self.n)).tocsr()
-                             
+
+        # for isp in range(self.tds.nb_spectra()):
+        #     # for sp in self.tds.spectra:
+        #     idx_sp = self.tds.spec_data.spec_index == isp
+        #     sp = self.tds.spec_data[idx_sp]
+        #     sli = np.where(idx_sp)[0]
+        #     slc = slice(sli.min(), sli.max()+1)
+
+        #     lmin, lmax = sp['wavelength'].min(), sp['wavelength'].max()
+        #     a = 2. / (lmax-lmin)
+        #     b = 1 - 2. * lmax / (lmax-lmin)
+        #     rwl = a * sp['wavelength'] + b
+        #     deg = self.pol_degrees[isp]
+        #     jacobian_spec_rec = scipy.sparse.coo_matrix(np.vander(rwl, deg+1))
+        #     i.append(jacobian_spec_rec.row + slc.start)
+        #     j.append(jacobian_spec_rec.col + self.offset[isp])
+        #     v.append(jacobian_spec_rec.data)
+
+        # i = np.hstack(i)
+        # j = np.hstack(j)
+        # v = np.hstack(v)
+        # self.jacobian = scipy.sparse.coo_matrix((v, (i, j)), shape=(self.N, self.n)).tocsr()
+
     def __call__(self, jac=False):
         """Evaluate the recalibration polynomials
 
-        Parameters
-        ----------
-        jac : bool
-            If the jacobian is needed.
-
-        Returns
-        -------
-        v : numpy.array
-            Recalibration parameter evaluated.
-        self.jacobian : None or scipy.sparse.coo_matrix
-            Jacobian matrix of the recalibration polynomial functions.
-        """
+            Parameters
+            ----------
+            jac : bool
+                If the jacobian is needed.
+
+            Returns
+            -------
+            v : numpy.array
+                Recalibration parameter evaluated.
+            self.jacobian : None or scipy.sparse.coo_matrix
+                Jacobian matrix of the recalibration polynomial functions.
+            """
         p_full = self.model.pars['SpectrumRecalibration'].full
         v = self.jacobian.dot(p_full)
         if not jac:
             return v, None
         return v, self.jacobian
 
-    
+
 class SALT2Like(object):
-    r"""A re-implementation of the SALT2 model 
-    
-    SALT2 is an empirical SN spectrophotometric model. This class
-    provides a pure python re-implementation of SALT2 with a number of
-    improvements.
-
-    The SALT2 parametrization is defined as follows. In the SN restframe
-    the absolute spectral density :math:`S(\lambda)` is:
-
-    .. math::   
-
-          S(\lambda, \mathrm{p}) = X_0 \times \left[M_0(\lambda, \mathrm{p}) + X_1
-          \times M_1(\lambda, \mathrm{p})\right]\ 10^{0.4 c CL(\lambda)}
-    
-    where :math:`\mathrm{p}` is the SN phase, i.e. the restframe time since SN peak luminosity:
+    r"""A re-implementation of the SALT2 model
 
-    .. math::
-    
-        \mathrm{ph} = \frac{t_{MJD} - t_{max}}{1 + z}
+        SALT2 is an empirical SN spectrophotometric model. This class
+        provides a pure python re-implementation of SALT2 with a number of
+        improvements.
 
-    :math:`M_0`, :math:`M_1` are global surfaces describing the
-    spectral evolution of the average SN and its principal variation,
-    and :math:`CL(\lambda)` is a global "extinction correction"
-    describing the color diversity of the SNIa family.
-
-    :math:`(X_0, X_1, c)` are SN-dependent. :math:`X_0` is the
-    amplitude of the "SN-frame B-band lightcurve" as inferred from the
-    observer-frame fluxes. :math:`X_1` is the coordinate of the SN
-    along :math:`M_1`. In practice, it quantifies the variations of the
-    light curve width. :math:`c` is the SN color -- or more exactly,
-    the SN color excess with respect to the average SN color.
+        The SALT2 parametrization is defined as follows. In the SN restframe
+        the absolute spectral density :math:`S(\lambda)` is:
 
-    Each Light Curve are evaluated interactively to use multi-threading and spectra are evaluated simultaneously.
+        .. math::
 
-    Attributes
-    ----------
-    training_dataset : nacl.dataset.TrainingDataset
-        Data set of photometric and spectroscopic observations.
-    lc_data : numpy.rec.array
-        Photometric data of the training data set.
-    phase_range : tuple
-        Boundaries for defining the phase interval.
-    wl_range : tuple
-        Boundaries for defining the wavelength interval.
-    n_wl : int
-        Number of knot of the wavelength spline basis.
-    n_ph : int
-        Number of knot of the phase spline basis.
-    spectrum_recal_degree : int
-        Degree of the spectral recalibration polynomial function.
-    init_from_salt2_file : str
-        File salt2, created by script 'nacl.simulation.make_salt2_npz.py'.
-    delta_phase : float
-        Offset in phase wrt SALT2.4.
-    dphase_dtmax : numpy.array
-        Derivative phase basis wrt time.
-    filterpath : str
-        Path to the filters files repository in nacl.dev/data/
-    timing : list
-        Timing of photometric and spectroscopic evaluation.
-    basis : nacl.lib.bspline.BSpline2D
-        2D spline basis.
-    gram : scipy.sparse.csc_matrix
-        First order grammian use to evaluate integral product of Wavelength basis of the model and filter basis.
-        :math::` \int \lambda B_\ell(\lambda) B_q(\lambda) d\lambda`
-    G2 : scipy.sparse.csc_matrix
-        Second order grammian use to evaluate integral product of Wavelength basis of the model and filter basis.
-        :math::` \int \lambda^2 B_\ell(\lambda) B_q(\lambda) d\lambda`
-    L_eff : scipy.sparse.coo_matrix
-        Effective wavelength used to calculate the photometric data color law.
-    val : numpy.array
-        Gather evaluation of each light curve and all spectral data.
-    jacobian_val : numpy.array
-        Gather non-zero derivatives of each light curve and all spectral data.
-    jacobian_i : numpy.array
-        Gather data index of non-zero derivatives of each light curve and all spectral data.
-    jacobian_j : numpy.array
-        Gather parameter index of non-zero derivatives of each light curve and all spectral data.
-    filter_basis : nacl.lib.bspline.BSpline
-        Filter basis defined common to all the bands.
-    color_law : ColorLaw
-        Color law class.
-    polynome_color_law : array-like
-        Photometric color law evaluations.
-    jacobian_color_law : scipy.sparse.csr_matrix or None
-        Photometric color law matrix of derivatives.
-    filter_db : nacl.instruments.FilterDb
-        Filter transmission projected on B-splines
-    bands : numpy.array
-        Bands used for photometric data
-    lambda_c : numpy.array
-        Mean wavelength of the filter in the SN-restframe.
-    lambda_c_red : numpy.array
-        Reduced mean wavelength of the filter in the SN-restframe.
-    pars : FitParameters
-        Model parameters.
-    pars0 : numpy.array
-        Model initial parameters.
-    NORM : float
-        Model normalization.
-    queue : list
-        List of photometric and spectral EvalUnit class.
-    disable_cache : object
+           S(\lambda, \mathrm{p}) = X_0 \times \left[M_0(\lambda, \mathrm{p}) + X_1
+           \times M_1(\lambda, \mathrm{p})\right]\ 10^{0.4 c CL(\lambda)}
+
+        where :math:`\mathrm{p}` is the SN phase, i.e. the restframe time since
+        SN peak luminosity:
+
+        .. math::
+
+            \mathrm{ph} = \frac{t_{MJD} - t_{max}}{1 + z}
+
+        :math:`M_0`, :math:`M_1` are global surfaces describing the
+        spectral evolution of the average SN and its principal variation,
+        and :math:`CL(\lambda)` is a global "extinction correction"
+        describing the color diversity of the SNIa family.
+
+        :math:`(X_0, X_1, c)` are SN-dependent. :math:`X_0` is the
+        amplitude of the "SN-frame B-band lightcurve" as inferred from the
+        observer-frame fluxes. :math:`X_1` is the coordinate of the SN
+        along :math:`M_1`. In practice, it quantifies the variations of the
+        light curve width. :math:`c` is the SN color -- or more exactly,
+        the SN color excess with respect to the average SN color.
+
+        Each Light Curve are evaluated interactively to use multi-threading and spectra are evaluated simultaneously.
+
+        Attributes
+        ----------
+        training_dataset : nacl.dataset.TrainingDataset
+            Data set of photometric and spectroscopic observations.
+        lc_data : numpy.rec.array
+            Photometric data of the training data set.
+        phase_range : tuple
+            Boundaries for defining the phase interval.
+        wl_range : tuple
+            Boundaries for defining the wavelength interval.
+        n_wl : int
+            Number of knot of the wavelength spline basis.
+        n_ph : int
+            Number of knot of the phase spline basis.
+        spectrum_recal_degree : int
+            Degree of the spectral recalibration polynomial function.
+        init_from_salt2_file : str
+            File salt2, created by script 'nacl.simulation.make_salt2_npz.py'.
+        delta_phase : float
+            Offset in phase wrt SALT2.4.
+        dphase_dtmax : numpy.array
+            Derivative phase basis wrt time.
+        filterpath : str
+            Path to the filters files repository in nacl.dev/data/
+        timing : list
+            Timing of photometric and spectroscopic evaluation.
+        basis : nacl.lib.bspline.BSpline2D
+            2D spline basis.
+        gram : scipy.sparse.csc_matrix
+            First order grammian use to evaluate integral product of Wavelength basis of the model and filter basis.
+            :math::` \int \lambda B_\ell(\lambda) B_q(\lambda) d\lambda`
+        G2 : scipy.sparse.csc_matrix
+            Second order grammian use to evaluate integral product of Wavelength basis of the model and filter basis.
+            :math::` \int \lambda^2 B_\ell(\lambda) B_q(\lambda) d\lambda`
+        L_eff : scipy.sparse.coo_matrix
+            Effective wavelength used to calculate the photometric data color law.
+        val : numpy.array
+            Gather evaluation of each light curve and all spectral data.
+        jacobian_val : numpy.array
+            Gather non-zero derivatives of each light curve and all spectral data.
+        jacobian_i : numpy.array
+            Gather data index of non-zero derivatives of each light curve and all spectral data.
+        jacobian_j : numpy.array
+            Gather parameter index of non-zero derivatives of each light curve and all spectral data.
+        filter_basis : nacl.lib.bspline.BSpline
+            Filter basis defined common to all the bands.
+        color_law : ColorLaw
+            Color law class.
+        polynome_color_law : array-like
+            Photometric color law evaluations.
+        jacobian_color_law : scipy.sparse.csr_matrix or None
+            Photometric color law matrix of derivatives.
+        filter_db : nacl.instruments.FilterDb
+            Filter transmission projected on B-splines
+        bands : numpy.array
+            Bands used for photometric data
+        lambda_c : numpy.array
+            Mean wavelength of the filter in the SN-restframe.
+        lambda_c_red : numpy.array
+            Reduced mean wavelength of the filter in the SN-restframe.
+        pars : FitParameters
+            Model parameters.
+        pars0 : numpy.array
+            Model initial parameters.
+        NORM : float
+            Model normalization.
+        queue : list
+            List of photometric and spectral EvalUnit class.
+        disable_cache : object
+
+        """
 
-    """
-    
     def __init__(self, training_dataset,
                  phase_range=(-20., 50.), wl_range=(2000., 9000.),  # . 11000.),
-                 basis_knot=[127, 20],
-                 basis_filter_knots = 900, 
-                 spectrum_recal_degree=None,
+                 basis_knots=[127, 20],
+                 basis_filter_knots=900,
+                 spectrum_recal_degree=3,
                  init_from_salt2_file=None,
-                 normalization_band_name='SWOPE::B'):
-        """Constructor. 
-          - instantiate the bases (phase, wavelength, filter)
-          - compute the Grams
-          - compute the lambda_eff matrix
-          - instantiate a color law and evaluate it on the lambda_eff's
-          - organizes the data into spectral/photometric computing units         
+                 init_from_training_dataset=False,
+                 normalization_band_name='SWOPE::B',
+                 error_snake=None,
+                 calib_variance=0.005**2):
+        """Constructor.
+              - instantiate the bases (phase, wavelength, filter)
+              - compute the Grams
+              - compute the lambda_eff matrix
+              - instantiate a color law and evaluate it on the lambda_eff's
+          - organizes the data into spectral/photometric computing units
 
         Parameters
         ----------
         training_dataset : nacl.dataset.TrainingDataset
             Training dataset.
         phase_range : 2-tuple
             Nominal phase range of the model.
         wl_range : 2-tuple
             Nominal wavelength range of the model.
-        basis_knot : 2-list
+        basis_knots : 2-list
             Number of wavelength and photometric knot.
         basis_filter_knots : int
             Number of knot for the filter basis
         spectrum_recal_degree : int
             Degree of the spectrum recalibration polynomials
         init_from_salt2_file : str
             If the model is to be initialized with the original
@@ -488,99 +520,188 @@
         normalization_band_name : str
             Use this band to normalize the model.
         """
         self.training_dataset = training_dataset
         self.lc_data = training_dataset.lc_data
         self.phase_range = phase_range
         self.wl_range = wl_range
-        self.n_wl, self.n_ph = basis_knot[0],  basis_knot[1]
+        self.n_wl, self.n_ph = basis_knots[0],  basis_knots[1]
+        self.basis_knots = basis_knots
+        self.basis_filter_knots = basis_filter_knots
         self.spectrum_recal_degree = spectrum_recal_degree
-        self.delta_phase = 0.
+        self.delta_phase = 0. # check: do not remember what this is
         self.filterpath = self.training_dataset.filterpath
-        
+        if self.training_dataset.lc_data is not None:
+            self.bands = list(self.training_dataset.transmissions.keys())
+        self.normalization_band_name = normalization_band_name
+        self.calib_variance = calib_variance
+
         self.timing = []
 
         self.basis, self.gram, self.G2, self.L_eff = None, None, None, None
         self.val, self.jacobian_val, self.jacobian_i, self.jacobian_j = None, None, None, None
         self.polynome_color_law, self.jacobian_color_law = None, None
 
         # Filter database
         # TODO: we should be able to optimize this a little
         # (i.e. adapt the filter bases, to lower the size of the grams)
         self.filter_basis = bspline.BSpline(np.linspace(self.wl_range[0], self.wl_range[1],  # 2000., 9000.,  #
                                                         basis_filter_knots), order=4)  # was 9000
         self.filter_db = FilterDb(self.filter_basis, self.training_dataset,
-                                  additional_band=['SWOPE::B'],
+                                  additional_band=[normalization_band_name],
                                   filterpath=self.filterpath)
         self.color_law = ColorLaw()
-        lc = self.training_dataset.lc_data
 
-        d = dict({(lc[i]['band_id'], lc[i]['Filter']) for i in np.arange(len(lc))})
-        self.bands = np.array([d[i] for i in range(len(d))])
-        
+        n_lc_meas, n_spec_meas, n_spectrophot_meas = \
+            self.training_dataset.nb_meas(split_by_type=1)
+
+        # lc = self.training_dataset.lc_data
+        # d = dict({(lc[i]['band_id'], lc[i]['Filter']) for i in np.arange(len(lc))})
+        # self.bands = np.array([d[i] for i in range(len(d))])
+        # self.bands = self.lc_data.band_index
+
         # lambda_c needed for the color scatter estimation
-        lambda_c = self.training_dataset.lc_data['Wavelength']/(1+self.training_dataset.lc_data['ZHelio'])
-        idx_lam_c = np.array([lc.data['i'][0] for lc in self.training_dataset.lcs])
-        self.lambda_c = lambda_c[idx_lam_c]
-        self.lambda_c_red = self.color_law.reduce(self.lambda_c)
-        
+        # lambda_c = self.training_dataset.lc_data['Wavelength']/(1+self.training_dataset.lc_data['ZHelio'])
+        # idx_lam_c = np.array([lc.data['i'][0] for lc in self.training_dataset.lcs])
+        # self.lambda_c = lambda_c[idx_lam_c]
+        # self.lambda_c_red = self.color_law.reduce(self.lambda_c)
+        #
+        # TODO: where is this used ?
+        # TODO: we may replace this by n_lc_meas > 0
+        if self.training_dataset.lc_data is not None:
+            tds = self.training_dataset
+            ii = self.training_dataset.i_lc_first
+            self.lambda_c = tds.lc_data.wavelength[ii] / (1+tds.lc_data.z[ii])
+            self.lambda_c_red = self.color_law.reduce(self.lambda_c)
+
         # initialize degree of the spectral recalibration polynomial
         self._init_spectral_polynomial()
-        # initialize model basis and model parameter vector 
+
+        # initialize model basis and model parameter vector
+        # model component: bases, color law, and parameter vector
+        self._init_bases()
+
+        # OK. For now, the color scatter and the calibration scatter
+        # are explicitely instantiated in the model constructor
+        self.calib_scatter = None
+        self.color_scatter = None
+        self.error_snake = error_snake if error_snake is not None else None
+        if self.training_dataset.lc_data is not None:
+            self.calib_scatter = vm.CalibrationScatter(self, calib_variance=calib_variance)
+            self.color_scatter = vm.ColorScatter(self)
+            if self.error_snake is None:
+                self.error_snake = vm.SimpleErrorSnake(self)
+
+        # finally, it is better to have it here.
+        # NOTE: if there are spectra, the model must be evaluated for them.
+        # even if they are marked as invalid
+        self.recal_func = None
+        if self.training_dataset.spec_data is not None:
+            self.recal_func = \
+                SpectrumRecalibrationPolynomials(self.training_dataset, self,
+                                                 self.recalibration_degree)
+
+        # initialize the global model parameters (M0, M1, CL)
         if init_from_salt2_file:
             self.init_from_salt2(init_from_salt2_file)
         else:
-            # model component: bases, color law, and parameter vector
-            self._init_bases()
-            # parameter vector 
             self.pars = self.init_pars()
+        # why ?
         self.pars0 = self.pars.full.copy()
-        # model normalization 
-        self.norm = self.normalization(band_name=normalization_band_name)
+
+        # initialize the SN specific parameters (X0, X1, col, tmax)
+        if init_from_training_dataset:
+            self.init_from_training_dataset()
+
+        # we use a default model normalization
+        # this is what guarantees that the SALT2.4 absolute mag
+        # is -19.5 in the SWOPE::B band. Of course, this default
+        # normalization may be changed explicitely, by calling
+        # self.renorm(band_name=, Mb=, magsys='AB')
+        self.norm = self.normalization(band_name=normalization_band_name,
+                                       default_norm=1.01907246e-12)
 
         # grams
         self.init_grams_and_cc_grid()
-        
+
         # and finally, prepare the computing units
         self.queue = self._init_computing_units()
 
         # clear the cache
         self.clear_cache()
 
         # if we need to run queue units separately,
         # could be useful to disable caching of the results
         self.disable_cache = False
 
-    def init_from_salt2(self, salt2_filename):
-        """Load the SALT2.4 global surfaces and color law, and adapts them to
-        our model implementation. 
+    def clone(self, training_dataset):
+        """return a clone (same basis, same color law) for a different tds
+        """
+        ret = SALT2Like(training_dataset,
+                        phase_range=self.phase_range,
+                        wl_range=self.wl_range,
+                        basis_knots=self.basis_knots,
+                        basis_filter_knots=self.basis_filter_knots,
+                        spectrum_recal_degree=self.spectrum_recal_degree,
+                        normalization_band_name=self.normalization_band_name,
+                        calib_variance=self.calib_variance)
+        for block_name in ['M0', 'M1', 'CL']:
+            ret.pars[block_name].full[:] = self.pars[block_name].full[:]
+        ret.norm = ret.normalization(band_name=ret.normalization_band_name)
+
+        return ret
+
+    def init_from_salt2(self, salt2_filename, stick_to_original_model=False):
+        """Load & adapt the SALT2.4 global surfaces and color law.
+
+        Load the coefficients of the SALT2.4 surfaces and color law. The
+        definition of the model spline bases differs from the original
+        definition of the SALT2.4 bases; so, we reproject the original SALT2
+        surfaces on the model basis.
 
         Parameters
         ----------
         salt2_filename : str
-            a salt2.npz filename containing the definition of the SALT2.4 bases,
-            M0, M1 surfaces and color_law.
+            the classical salt2.npz filename containing the definition of the
+            SALT2.4 bases, M0, M1 surfaces and color_law.
         """
         f = np.load(salt2_filename)
-        # initialize the original SALT2 basis
-        # (just extend it so that it covers [-100,100] in phase)
-        #        phase_grid = np.hstack([np.linspace(-100., -21., 5),
-        #                                f['phase_grid'],
-        #                                np.linspace(55., 100., 5)])
         phase_grid = f['phase_grid']
         wl_grid = f['wl_grid']
-        self.basis = bspline.BSpline2D(wl_grid, phase_grid, x_order=4, y_order=4)
-        self.delta_phase = +0.7
+        basis = bspline.BSpline2D(wl_grid, phase_grid, x_order=4, y_order=4)
+
+        if stick_to_original_model:
+            # don't remember why we have this
+            self.delta_phase = +0.7
+            self.basis = basis
+            self.pars = self.init_pars()
+            self.pars['M0'].full[:] = f['M0'].T.ravel()
+            self.pars['M1'].full[:] = f['M1'].T.ravel()
+            self.pars['CL'].full[:] = f['CL_pars'][0:4]
+            return
+
+        # TODO: replace this with
+        # xx = self.basis.bx.grid
+        # yy = self.basis.by.grid
+        xx = np.linspace(wl_grid[0], wl_grid[-1], basis.bx.nj)
+        yy = np.linspace(phase_grid[0], phase_grid[-1], basis.by.nj)
+        x,y = np.meshgrid(xx,yy)
+        x,y = x.ravel(), y.ravel()
+        jac = self.basis.eval(x,y).tocsr()
+        factor = cholesky_AAt(jac.T, beta=1.E-20)
 
-        # and init the parameters
+        # and initialize the parameters
         self.pars = self.init_pars()
-        self.pars['M0'].full[:] = f['M0'].T.ravel()
-        self.pars['M1'].full[:] = f['M1'].T.ravel()
+        self.pars['M0'].full[:] = factor(jac.T * f['M0'])
+        self.pars['M1'].full[:] = factor(jac.T * f['M1'])
         self.pars['CL'].full[:] = f['CL_pars'][0:4]
-        
+
+    def reduce(self, wl):
+        return self.color_law.reduce(wl)
+
     def init_grams_and_cc_grid(self):
         r"""Compute the :math:`\Lambda^{\mathrm{eff}}_{\ell q}` matrix (see definition above) on which the color
         law is evaluated.
 
         .. math::
              \bar{\lambda}_{\ell q} = \frac{\int \lambda^2 B_\ell(\lambda) B_q(\lambda)
              d\lambda}{\int \lambda B_\ell(\lambda) B_q(\lambda) d\lambda}
@@ -589,122 +710,196 @@
 
         .. math::
             G = \int \lambda B_\ell(\lambda) B_q(\lambda) d\lambda \\
             G2 = \int \lambda^2 B_\ell(\lambda) B_q(\lambda) d\lambda
 
 
         .. note::
-             this method will be moved to the main model class (since we may work 
+             this method will be moved to the main model class (since we may work
              with one single :math:`\Lambda^{\mathrm{eff}}` matrix in a near future).
-        """        
+        """
         self.gram = get_gram(0., self.basis.bx, self.filter_basis, lambda_power=1)
         self.G2 = get_gram(0., self.basis.bx, self.filter_basis, lambda_power=2)
-            
+
         gram = self.gram.tocoo()
         gram2 = self.G2.tocoo()
         assert(~np.any(gram.row-gram2.row) and ~np.any(gram.col-gram2.col))
         l_eff = gram2.data / gram.data
         self.L_eff = scipy.sparse.coo_matrix((l_eff, (gram.row, gram.col)), shape=gram.shape)
 
-    def init_pars(self):
+    def get_struct(self):
+        """return the structure of the fit parameter vector
+
+        In practice, the fit parameter vector is larger than just the model
+        parameters: it also contains the parameters of the error models (error
+        snake, color scatter, calibration, see e.g. variancemodels.py). The
+        instantiation of the final fit parameter vector cannot therefore be
+        performed by the model itself.  What the model can do, is to return the
+        description of the fit parameter blocks it knows about.
         """
-        Instantiate a fit parameter vector and return it.
+        nb_sne = self.training_dataset.nb_sne()
+        # nb_spectra = self.training_dataset.nb_spectra()
+        # nb_passbands = len(self.bands)
+        spec_recalibration_npars = self.recalibration_degree + 1
+        nb_lightcurves = self.training_dataset.nb_lcs(valid_only=False)
+        d = [('X0',   nb_sne),
+             ('X1',   nb_sne),
+             ('col',  nb_sne),
+             ('tmax', nb_sne),
+             ('M0',   self.basis.bx.nj * self.basis.by.nj),
+             ('M1',   self.basis.bx.nj * self.basis.by.nj),
+             ('CL',  4)]
+        if self.training_dataset.spec_data is not None:
+            d.append(('SpectrumRecalibration', spec_recalibration_npars.sum()))
+
+             #             ('eta_calib', nb_passbands),
+             #             ('kappa_color', nb_lightcurves)
+             # ]
+        return d
+
+    def init_pars(self):
+        """instantiate a fit parameter vector
 
         Returns
         -------
         fp : nacl.lib.fitparameters.FitParameters
             Model parameters.
         """
-        nb_sne = self.training_dataset.nb_sne()
-        nb_spectra = self.training_dataset.nb_spectra()
-        nb_passbands = len(self.bands)
-        all_degree = self.recalibration_degree + 1
-        nb_lightcurves = self.training_dataset.nb_lcs()
-        fp = FitParameters([('X0', nb_sne),                            
-                            ('X1', nb_sne),
-                            ('c',  nb_sne),
-                            ('tmax', nb_sne),
-                            ('M0',  self.basis.bx.nj * self.basis.by.nj),
-                            ('M1',  self.basis.bx.nj * self.basis.by.nj),
-                            ('CL',  4),
-                            # TODO: size of recalibration parameters should be abstracted 
-                            ('SpectrumRecalibration', all_degree.sum()),
-                            ('eta_calib', nb_passbands),
-                            ('kappa_color', nb_lightcurves)])
+        p_struct = self.get_struct()
+        if self.calib_scatter is not None:
+            p_struct.extend(self.calib_scatter.get_struct())
+        if self.color_scatter is not None:
+            p_struct.extend(self.color_scatter.get_struct())
+        if self.error_snake is not None:
+            p_struct.extend(self.error_snake.get_struct())
+        fp = FitParameters(list(set(p_struct)))
 
+        # minimal initialization
         fp['X0'].full[:] = 1.
-        rec_val = np.zeros_like(fp['SpectrumRecalibration'].full[:])
-        
-        for i in np.arange(nb_spectra):
-            offset = all_degree[:i+1].sum()
-            rec_val[offset-1] = 1  # -0.2
-
-        fp['SpectrumRecalibration'].full[:] = rec_val  # + 0.2
-        fp['kappa_color'].full[:] = 0  # 1e-1
+        if 'SpectrumRecalibration' in fp._struct:
+            assert self.recal_func is not None
+            fp['SpectrumRecalibration'].full[:] = self.recal_func.init_pars()
         return fp
 
-    def _init_spectral_polynomial(self):
+    def init_from_training_dataset(self):
+        """load initial sn parameters from the training dataset
         """
-        Instantiate spectral polynomial for recalibration.
-        If : a degree is given, all spectra as the same, which is spectrum_recal_degree
-        else : 
+        sn_data = self.training_dataset.sn_data
+        self.pars['X0'].full[sn_data.sn_index] = sn_data.x0
+        self.pars['X1'].full[sn_data.sn_index] = sn_data.x1
+        self.pars['col'].full[sn_data.sn_index] = sn_data.col
+        self.pars['tmax'].full[sn_data.sn_index] = sn_data.tmax
+
+#        nb_sne = self.training_dataset.nb_sne()
+#        nb_spectra = self.training_dataset.nb_spectra()
+#        nb_passbands = len(self.bands)
+#        all_degree = self.recalibration_degree + 1
+#        nb_lightcurves = self.training_dataset.nb_lcs()
+#        fp = FitParameters([('X0', nb_sne),
+#                            ('X1', nb_sne),
+#                            ('col',  nb_sne),
+#                            ('tmax', nb_sne),
+#                            ('M0',  self.basis.bx.nj * self.basis.by.nj),
+#                            ('M1',  self.basis.bx.nj * self.basis.by.nj),
+#                            ('CL',  4),
+#                            # TODO: size of recalibration parameters should be abstracted
+#                            ('SpectrumRecalibration', all_degree.sum()),
+#                            ('eta_calib', nb_passbands),
+#                            ('kappa_color', nb_lightcurves)])
+
+#        fp['X0'].full[:] = 1.
+#        rec_val = np.zeros_like(fp['SpectrumRecalibration'].full[:])
+
+#        for i in np.arange(nb_spectra):
+#            offset = all_degree[:i+1].sum()
+#            rec_val[offset-1] = 1  # -0.2
+
+#        fp['SpectrumRecalibration'].full[:] = rec_val  # + 0.2
+#        fp['kappa_color'].full[:] = 0  # 1e-1
+#        return fp
+
+    def _init_spectral_polynomial(self):
+        """instantiate the recalibration polynomials
+
+        if a degree is specified, all spectra have the same degree.
         Since the degree of the polynomial must not exceed the number of Light curves :
         this degree is large odd number inferior to the numbers of light curves for this SN.
         """
-        nb_spectra = self.training_dataset.nb_spectra()
-        self.recalibration_degree = np.ones(nb_spectra).astype(int)
-        # print(self.spectrum_recal_degree)
-        # print(self.spectrum_recal_degree is None)
-        # print(self.spectrum_recal_degree is not None)
-        if self.spectrum_recal_degree is None:
-            # print(self.spectrum_recal_degree)
-            lcs = self.training_dataset.lc_data
-            sps = self.training_dataset.spec_data
-        
-            for isp in np.unique(sps['spec_id']):
-                isn = sps['sn_id'][sps['spec_id'] == isp][0]
-                n_lcs_sn = len(np.unique(lcs[lcs['sn_id'] == isn]['lc_id']))
-                if n_lcs_sn % 2 == 0:
-                    self.recalibration_degree[isp] = n_lcs_sn - 1 
-                elif n_lcs_sn % 2 == 1:
-                    self.recalibration_degree[isp] = n_lcs_sn - 2 
-        else:
-            self.recalibration_degree *= self.spectrum_recal_degree
+        # note: the model is evaluated on the full dataset.
+        # not just the valid data.
+        nb_spectra = self.training_dataset.nb_spectra(valid_only=False)
+        self.recalibration_degree = np.full(nb_spectra, self.spectrum_recal_degree)
+
+        # here, there was a code to limit the degree of the recalibration
+        # polynomials to the total number of light curves available for the
+        # corresponding SN.
+
+        # if self.spectrum_recal_degree is None:
+        #     # print(self.spectrum_recal_degree)
+        #     lcs = self.training_dataset.lc_data
+        #     sps = self.training_dataset.spec_data
+
+        #     for isp in sps.spec_set:
+        #         isn =
+        #     for isp in np.unique(sps['spec_id']):
+        #         isn = sps['sn_id'][sps['spec_id'] == isp][0]
+        #         n_lcs_sn = len(np.unique(lcs[lcs['sn_id'] == isn]['lc_id']))
+        #         if n_lcs_sn % 2 == 0:
+        #             self.recalibration_degree[isp] = n_lcs_sn - 1
+        #         elif n_lcs_sn % 2 == 1:
+        #             self.recalibration_degree[isp] = n_lcs_sn - 2
+        # else:
+        #     self.recalibration_degree *= self.spectrum_recal_degree
 
     def _init_bases(self):
         """
         Instantiate model bases
         """
         phase_grid = np.hstack([np.linspace(self.phase_range[0], self.phase_range[1], self.n_ph)])
         wl_grid = np.linspace(self.wl_range[0], self.wl_range[1], self.n_wl)
         self.basis = bspline.BSpline2D(wl_grid, phase_grid, x_order=4, y_order=4)
 
-    def normalization(self, band_name='SWOPE::B'):
-        r"""Compute the default model normalization.
+    def normalization(self, band_name='SWOPE::B', Mb=-19.5, magsys='AB',
+                      default_norm=None):
+        """model normalization
 
-        The model is normalized so that the broadband flux at peak, of
-        a normal :math:`(X1=0, c=0)` SN, in the band specified in
-        argument (generally some flavour of the :math:`B`-band) is
-        equal to unity.
-
-        .. math::
-               \int S(\lambda,0) \frac{\lambda}{hc} B(\lambda) d\lambda = 1
+        The SALT2Like normalization is set during training by the constraint
+        on the integral of M0 at phase zero.
 
-        Returns
-        -------
-        float
-            Overall normalization term of the model.
+        Therefore, by default, we do not renormalize the model during
+        evaluation.
         """
         tq, filter_basis = self.filter_db[band_name]
         phase_eval = self.basis.by.eval(np.array([0. + self.delta_phase])).tocsr()
-        gram = get_gram(z=0., model_basis=self.basis.bx, filter_basis=filter_basis, lambda_power=1)
+        gram = get_gram(z=0., model_basis=self.basis.bx,
+                        filter_basis=filter_basis, lambda_power=1)
         surface_0 = self.pars['M0'].full.reshape(len(self.basis.by), -1)
         # evaluate the integral of the model in the specified band
-        norm = phase_eval.dot(surface_0.dot(gram.dot(tq)))
-        return 1. / norm
+        self.int_M0_phase_0 = phase_eval.dot(surface_0.dot(gram.dot(tq)))
+
+        # AB flux in the specified band
+        ms = MagSys(magsys)
+        zp = ms.ZeroPoint(self.filter_db.transmission_db[band_name])
+        self.int_ab_spec = 10**(0.4 * zp)
+
+        # normalization quantities
+        self.flux_at_10pc = np.power(10., -0.4 * (Mb-zp))
+        self.flux_at_10Mpc = np.power(10., -0.4 * (Mb+30.-zp))
+
+        if default_norm is not None:
+            return default_norm
+
+        return self.flux_at_10Mpc / self.int_M0_phase_0
+
+    def renorm(self, band_name='SWOPE::B', Mb=-19.5, magsys='AB'):
+        """Adjust the model normalization
+        """
+        # explicitely recompute a normalization
+        self.norm = self.normalization(band_name, Mb, magsys,
+                                       default_norm=None)
 
     def _init_computing_units(self):
         """Prepare and queue all the computing units
 
         The model evaluation is deferred to two kinds of so-called
         'eval units'.
 
@@ -724,18 +919,24 @@
              practice, it seems that the overheads from using python
              parallelism at this level are high (because of the GIL)
              and that we gain much more by using numpy/scipy implicit
              multithreading. We stick to this design because it makes
              things clearer in fact.
 
         """
+        # n_lc_meas, n_spec_meas, n_spectrophot_meas = \
+        #     self.training_dataset.nb_meas(valid=True, split_by_type=True)
         queue = []
-        for lc in self.training_dataset.lcs:
-            queue.append(LightcurveEvalUnitTz(lc, self))
-        queue.append(SpectrumEvalUnitFast(self.training_dataset, self))
+        if self.training_dataset.lc_data is not None:
+            for lc in self.training_dataset.lcs:
+                queue.append(LightcurveEvalUnitTz(lc, self))
+        if self.training_dataset.spec_data is not None:
+            queue.append(SpectrumEvalUnitFast(self.training_dataset, self))
+        if self.training_dataset.spectrophotometric_data is not None:
+            queue.append(SpectroPhotoEvalUnit(self.training_dataset, self))
         return queue
 
     def update_computing_units(self, ilc=None, spec=False):
         """
         Recreate the model queue as a function of the wanted LCs and spectra.
 
         Parameters
@@ -752,67 +953,71 @@
         """
         queue = []
         if ilc is not None:
             for lc in [self.training_dataset.lcs[ilc]]:
                 queue.append(LightcurveEvalUnitTz(lc, self))
         if spec:
             queue.append(SpectrumEvalUnitFast(self.training_dataset, self))
-        return queue 
+        return queue
 
     def clear_cache(self):
         """
         Clear model evaluation, derivatives and timing.
         """
         self.val = []
         self.jacobian_i = []
         self.jacobian_j = []
         self.jacobian_val = []
         self.timing = []
-        
+
     def precompute_color_law(self, cl_pars=None, jac=False):
         """
         Precompute the color law for the photometric data.
 
         Parameters
         -------
         cl_pars : None or numpy.array
             Color law parameters
         jac : bool
             If derivatives are needed.
         """
         if cl_pars is None:
             cl_pars = self.pars['CL'].full
-            
-        polynome_color_law, jacobian_color_law = self.color_law(self.L_eff.data, cl_pars, jac=jac)  # return_jacobian_as_coo_matrix=False)
-        self.polynome_color_law = scipy.sparse.csr_matrix((polynome_color_law,
-                                                           (self.L_eff.row, self.L_eff.col)), shape=self.L_eff.shape)
+
+        polynome_color_law, jacobian_color_law = \
+            self.color_law(self.L_eff.data, cl_pars,
+                           jac=jac)  # return_jacobian_as_coo_matrix=False)
+        self.polynome_color_law = \
+            scipy.sparse.csr_matrix((polynome_color_law,
+                                     (self.L_eff.row, self.L_eff.col)),
+                                    shape=self.L_eff.shape)
         if jac:
             self.jacobian_color_law = []
             _, n = jacobian_color_law.shape
             for i in range(n):
-                jacobian_cl = scipy.sparse.csr_matrix((jacobian_color_law[:, i],
-                                                       (self.L_eff.row, self.L_eff.col)), shape=self.L_eff.shape)
+                jacobian_cl = \
+                    scipy.sparse.csr_matrix((jacobian_color_law[:, i],
+                                             (self.L_eff.row, self.L_eff.col)), shape=self.L_eff.shape)
                 self.jacobian_color_law.append(jacobian_cl)
-    
+
     def get_restframe_phases(self, data):
         """
         Given a chunk of data, return the restframe phases
 
         Returns
         -------
         numpy.array
             data SN-restframe phase
         """
-        sn_id = data['sn_id']
-        tmax = self.pars['tmax'].full[sn_id]
-        z = self.training_dataset.sne['z'][sn_id]
-        return (data['Date'] - tmax) / (1.+z)
-                
+        sn_index = data.sn_index
+        tmax = self.pars['tmax'].full[sn_index]
+        return (data.mjd - tmax) / (1.+data.z)
+
     def __call__(self, p, jac=False, plotting=False, ilc_plot=None, spec_plot=False):
-        """Evaluate the model for the parameter set p 
+        """Evaluate the model for the parameter set p
 
         In practice, loop over the queue and run each eval unit.
         Assemble the results into one single vector and (optionally)
         one single jacobian matrix.
 
         Parameters
         -------
@@ -824,70 +1029,76 @@
         plotting : bool
             Plotting need to evaluated only some data [plotting needs]
         ilc_plot : list
             Light curves to be evaluated [plotting needs]
         spec_plot : bool
             Spectra to be evaluated [plotting needs]
 
-
         Returns
         -------
         val : numpy.array
             model results
         jacobian : scipy.sparse.csr_matrix
             jacobian matrix (if jac is true)
         """
         # update pars
         self.pars.free = p
 
         # pre-evaluate the color law (shared between all light curves)
         self.precompute_color_law(jac=jac)
 
-        # precompute the values of the phase basis on the full dataset 
+        # precompute the values of the phase basis on the full dataset
         # significantly faster that way
-        restframe_phases = self.get_restframe_phases(self.lc_data)
-        self.phase_eval = self.basis.by.eval(restframe_phases + self.delta_phase).tocsr()
-        if jac:
-            self.dphase_dtmax = self.basis.by.deriv(restframe_phases + self.delta_phase).tocsr()
-        else:
-            self.dphase_dtmax = None
-            
+        if self.training_dataset.lc_data is not None:
+            restframe_phases = self.get_restframe_phases(self.lc_data)
+            self.phase_eval = self.basis.by.eval(restframe_phases + self.delta_phase).tocsr()
+            if jac:
+                self.dphase_dtmax = self.basis.by.deriv(restframe_phases + self.delta_phase).tocsr()
+            else:
+                self.dphase_dtmax = None
+
         self.clear_cache()
 
         # queue all Eval Unit for minimization or for plotting
         if plotting:
             queue = self.update_computing_units(ilc=ilc_plot, spec=spec_plot)
         else:
             queue = self.queue
-            
-        # now, we are ready to loop over the eval units 
+
+        # now, we are ready to loop over the eval units
         for q in queue:
             q(jac)
         val = np.hstack(self.val)
-        
+        # print('--> len(val):', len(val), len(self.training_dataset.lc_data), len(self.training_dataset.spec_data))
+
         if not jac:
             return val
 
-        # collect and assemble the results 
-        n_data = len(self.training_dataset.lc_data)  # + len(self.training_dataset.spec_data)
-        fit_spec = False
-        for ique in self.queue:
-            if ique.data['spec_id'].mean() != -1:
-                fit_spec = True
-                
-        if fit_spec:
-            n_data += len(self.training_dataset.spec_data)
-            
+        # collect and assemble the results
+        # n_data = len(self.training_dataset.lc_data)  + len(self.training_dataset.spec_data)
+        n_data = self.training_dataset.nb_meas(valid_only=False)
+
+        # nrl: I don't know what this is for. Commented out.
+        # fit_spec = False
+        # for ique in self.queue:
+        #     if ique.data['spec_id'].mean() != -1:
+        #         fit_spec = True
+
+        # if fit_spec:
+        #     n_data += len(self.training_dataset.spec_data)
+
+        logging.debug('computing derivatives: hstack...')
         n = len(self.pars.free)
-        
         i = np.hstack(self.jacobian_i)
         j = np.hstack(self.jacobian_j)
         v = np.hstack(self.jacobian_val)
+        logging.debug('building coo_matrix...')
         idx = j >= 0  # self.pars.indexof(j) >= 0
         jacobian = scipy.sparse.coo_matrix((v[idx], (i[idx], j[idx])), shape=(n_data, n))
+        logging.debug('ok, done.')
         return val, jacobian
 
 #       else:
 #            logging.info('SALT2Like.__call__: joblib.Parallel')
 #            def f(x):
 #                x.__call__(jac=jac)
 #            Parallel(n_jobs=n_jobs)(delayed(f)(x) for x in self.queue)
@@ -904,15 +1115,15 @@
     Calculate the grammian of to spline basis.
 
     The grammian :math:`G` of order :math:`N`, to basis :math:`B_0` (define on wavelength,
     in our case surfaces wavelength basis) and
     :math:`B_1` (define on SN-restframe wavelength, filter basis) is defined as :
 
     .. math::
-        G = \int \lambda^N B_0(\lambda) B_q(\lambda (1+z)) d\lambda
+        G = \\int \\lambda^N B_0(\\lambda) B_q(\\lambda (1+z)) d\\lambda
 
     Parameters
     -------
     z : numpy.array
         Vector containing the data redshift.
     model_basis : nacl.lib.bspline.BSpline
         Wavelength basis.
@@ -925,20 +1136,20 @@
     -------
     gram : scipy.sparse.csc_matrix
         Grammian
     """
     global _G
     global _G2
     key = (z, model_basis, filter_basis, lambda_power)
-    
+
     gram = _G.get(key, None)
     if gram is None:
         gram = bspline.lgram(model_basis, filter_basis, z=z, lambda_power=lambda_power).tocsc()
         _G[key] = gram
-        
+
     return gram
 
 
 class LightcurveEvalUnitTz(object):
     r"""
     Compute an SN light curve of one supernova in one single band.
 
@@ -1033,28 +1244,29 @@
         ----------
         lcdata : nacl.dataset.LcData
             Photometric of one Lc of one SN nacl data class.
         model : nacl.models.salt.SALT2Like
             Model.
         """
         self.lcdata = lcdata
-        self.data = lcdata.data
+        # self.data = lcdata.data # we no longer use this
         self.model = model
-        self.z = lcdata.z        
-        self.band = lcdata.band
+        self.z = lcdata.z[0]
+        self.band = lcdata.band[0]
         tr = model.filter_db.transmission_db[self.band]
         self.tqz, _ = model.filter_db.insert(tr, z=self.z)
         # set to zero very small values
         self.tqz[(np.abs(self.tqz)/self.tqz.max() < 1e-10)] = 0.
-        
-        self.sn_id = lcdata.sn_id
-        
+
+        # self.sn_id = lcdata.sn_id
+        self.sn_index = lcdata.sn_index[0]
+
         #        self.wl_basis_size = len(model.basis.bx)
         self.ph_basis_size = len(model.basis.by)
-        
+
         self.M0 = model.pars['M0'].full.reshape(self.ph_basis_size, -1)
         self.M1 = model.pars['M1'].full.reshape(self.ph_basis_size, -1)
         self.cl_pars = model.pars['CL'].full
 
     def __call__(self, jac=False, debug_mode=False):
         """
         Evaluate the SN light curve.
@@ -1071,156 +1283,167 @@
         ----------
         val : numpy.array
             Model evaluation
         jacobian : scipy.sparse.csr_matrix
             Jacobian matrix (optional)
 
         """
-        t0 = time.time()
-        sn_id = self.sn_id
+        t0 = time.perf_counter()
+        sn_index = self.sn_index
         zz = 1. + self.z
         pars = self.model.pars
-        data = self.lcdata.data
-        band_id = self.lcdata.data['band_id'][0]
+        # data = self.lcdata.data
+        band_index = self.lcdata.band_index[0]
+
+        # band_id = self.lcdata.data['band_id'][0]
         # print(self.model.bands[band_id], self.lcdata.data['Filter'][0])
-        lc_id = self.lcdata.data['lc_id'][0]
+        # lc_id = self.lcdata.data['lc_id'][0]
+        lc_index = self.lcdata.lc_index[0]
+        sn_index = self.lcdata.sn_index[0]
 
         # sn-related parameters
-        x0, x1 = pars['X0'].full[sn_id], pars['X1'].full[sn_id]
-        c, tmax = pars['c'].full[sn_id],  pars['tmax'].full[sn_id]
-        eta = pars['eta_calib'].full[band_id]
+        x0, x1 = pars['X0'].full[sn_index], pars['X1'].full[sn_index]
+        c, tmax = pars['col'].full[sn_index],  pars['tmax'].full[sn_index]
+        eta = pars['eta_calib'].full[band_index]
+        kappa = pars['kappa_color'].full[lc_index]
+        # model_to_meas_scale = self.lc_data.norm
+        flux_scale = self.model.norm * self.lcdata.norm
 
-        kappa = pars['kappa_color'].full[lc_id]
-        
         phase_eval = self.model.phase_eval[self.lcdata.slc]
         # color law evaluation -- on the Gram \lambda_eff's
         cl = np.power(10., 0.4 * c * self.model.polynome_color_law.data)
         csr_color_law = scipy.sparse.csr_matrix((cl, (self.model.L_eff.row, self.model.L_eff.col)),
                                                 shape=self.model.L_eff.shape)
         gram = self.model.gram.multiply(csr_color_law)
         tqz = self.tqz
 
         # much faster with the .dot's (instead of @)
         integral_surface_0 = phase_eval.dot(self.M0.dot(gram.dot(tqz)))
         integral_surface_1 = phase_eval.dot(self.M1.dot(gram.dot(tqz)))
-        flux = self.model.norm * zz * x0 * (integral_surface_0+x1*integral_surface_1)*(1+eta)*(1+kappa)
+        flux = flux_scale * zz * x0 * (integral_surface_0+x1*integral_surface_1)*(1+eta)*(1+kappa)
 
-        if debug_mode:
-            return self.model.norm * integral_surface_0, self.model.norm * integral_surface_1, \
-                   cl, flux, x0, x1, self.model.norm
+        # if debug_mode:
+        #     return model_norm * integral_surface_0, model_norm * integral_surface_1, \
+        #            cl, flux, x0, x1, model_norm
 
         self.model.val.append(flux)
         if not jac:
-            self.model.timing.append(time.time()-t0)
+            self.model.timing.append(time.perf_counter()-t0)
             return flux
 
-        n_data = len(self.data)
-        sn = np.full(n_data, self.sn_id)
-        norm = self.model.norm
-        
+        # n_data = len(self.lcdata)
+        # sn_index = np.full(n_data, self.sn_index)
+        # norm = self.model.norm
+
         # shortcut names to the internal cache holding the
-        # jacobian matrix definition 
+        # jacobian matrix definition
         jacobian_i, jacobian_j, jacobian_val = self.model.jacobian_i, self.model.jacobian_j, self.model.jacobian_val
-        
+
         # dMdX0
-        jacobian_i.append(self.data.i)
-        jacobian_j.append(self.model.pars['X0'].indexof(sn))
-        jacobian_val.append(norm * zz * (integral_surface_0 + x1*integral_surface_1) * (1+eta) * (1+kappa))
+        jacobian_i.append(self.lcdata.row)
+        jacobian_j.append(self.model.pars['X0'].indexof(self.lcdata.sn_index))
+        assert len(self.lcdata.row) == len(self.model.pars['X0'].indexof(self.lcdata.sn_index))
+        jacobian_val.append(flux_scale * zz * (integral_surface_0 + x1*integral_surface_1) * (1+eta) * (1+kappa))
 
         # dMdX1
-        jacobian_i.append(self.data.i)
-        jacobian_j.append(self.model.pars['X1'].indexof(sn))
-        jacobian_val.append(norm * zz * x0 * integral_surface_1 * (1+eta) * (1+kappa))
+        jacobian_i.append(self.lcdata.row)
+        jacobian_j.append(self.model.pars['X1'].indexof(self.lcdata.sn_index))
+        assert len(self.lcdata.row) == len(self.model.pars['X1'].indexof(self.lcdata.sn_index))
+        jacobian_val.append(flux_scale * zz * x0 * integral_surface_1 * (1+eta) * (1+kappa))
 
         # dMdc
-        jacobian_i.append(self.data.i)
-        jacobian_j.append(self.model.pars['c'].indexof(sn))
+        jacobian_i.append(self.lcdata.row)
+        jacobian_j.append(self.model.pars['col'].indexof(self.lcdata.sn_index))
+        assert len(self.lcdata.row) == len(self.model.pars['col'].indexof(self.lcdata.sn_index))
         gram_color_law = gram.multiply(self.model.polynome_color_law)
         dintegral0_dc = 0.4 * np.log(10.) * phase_eval.dot(self.M0.dot(gram_color_law.dot(tqz)))
         dintegral1_dc = 0.4 * np.log(10.) * phase_eval.dot(self.M1.dot(gram_color_law.dot(tqz)))
-        jacobian_val.append(norm * zz * x0 * (dintegral0_dc + x1*dintegral1_dc) * (1+eta) * (1+kappa))
+        jacobian_val.append(flux_scale * zz * x0 * (dintegral0_dc + x1*dintegral1_dc) * (1+eta) * (1+kappa))
 
         # dMdtmax
         dphase_dtmax = self.model.dphase_dtmax[self.lcdata.slc]
-        jacobian_i.append(self.data.i)
-        jacobian_j.append(self.model.pars['tmax'].indexof(sn))
+        jacobian_i.append(self.lcdata.row)
+        jacobian_j.append(self.model.pars['tmax'].indexof(self.lcdata.sn_index))
+        assert len(self.lcdata.row) == len(self.model.pars['tmax'].indexof(self.lcdata.sn_index))
         dintegral0_dtmax = -dphase_dtmax.dot(self.M0.dot(gram.dot(tqz))) / zz
         dintegral1_dtmax = -dphase_dtmax.dot(self.M1.dot(gram.dot(tqz))) / zz
-        jacobian_val.append(norm * zz * x0 * (dintegral0_dtmax + x1*dintegral1_dtmax)*(1+eta)*(1+kappa))
+        jacobian_val.append(flux_scale * zz * x0 * (dintegral0_dtmax + x1*dintegral1_dtmax)*(1+eta)*(1+kappa))
 
         # dMdtheta_0
         dbase_dtheta = scipy.sparse.kron(phase_eval, gram.dot(tqz)).tocoo()
-        jacobian_i.append(self.data.i[dbase_dtheta.row])
+        jacobian_i.append(self.lcdata.row[dbase_dtheta.row])
         jacobian_j.append(self.model.pars['M0'].indexof(dbase_dtheta.col))
-        jacobian_val.append(norm * zz * x0 * dbase_dtheta.data * (1+eta) * (1+kappa))
-        
+        assert len(self.lcdata.row[dbase_dtheta.row]) == len(self.model.pars['M0'].indexof(dbase_dtheta.col))
+        jacobian_val.append(flux_scale[dbase_dtheta.row] * zz * x0 * dbase_dtheta.data * (1+eta) * (1+kappa))
+
         # dMdtheta_1
-        jacobian_i.append(self.data.i[dbase_dtheta.row])
+        jacobian_i.append(self.lcdata.row[dbase_dtheta.row])
         jacobian_j.append(self.model.pars['M1'].indexof(dbase_dtheta.col))
-        jacobian_val.append(norm * zz * x0 * x1 * dbase_dtheta.data * (1+eta) * (1+kappa))
-        
+        assert len(self.lcdata.row[dbase_dtheta.row]) == len(self.model.pars['M1'].indexof(dbase_dtheta.col))
+        jacobian_val.append(flux_scale[dbase_dtheta.row] * zz * x0 * x1 * dbase_dtheta.data * (1+eta) * (1+kappa))
+
         # dMdcl
         # I really don't know how to vectorize the computation
-        # of these derivatives. If somebody has an idea let me know. 
-        buff = np.zeros(n_data).astype(int)
+        # of these derivatives. If somebody has an idea let me know.
+        buff = np.zeros(len(self.lcdata)).astype(int)
         for i, jacobian_color_law in enumerate(self.model.jacobian_color_law):
             buff[:] = i
-            jacobian_i.append(self.data.i)
+            jacobian_i.append(self.lcdata.row)
             jacobian_j.append(self.model.pars['CL'].indexof(buff))
             gram_jacobian_color_law = gram.multiply(jacobian_color_law)
             jacobian_surface0_color_law = 0.4 * np.log(10.) * c * phase_eval.dot(self.M0.dot(
                 gram_jacobian_color_law.dot(tqz)))
             jacobian_surface1_color_law = 0.4 * np.log(10.) * c * phase_eval.dot(self.M1.dot(
                 gram_jacobian_color_law.dot(tqz)))
-            jacobian_val.append(norm * zz * x0 * (jacobian_surface0_color_law + x1*jacobian_surface1_color_law)
+            jacobian_val.append(flux_scale * zz * x0 * (jacobian_surface0_color_law + x1*jacobian_surface1_color_law)
                                 * (1+eta) * (1+kappa))
 
         # dMdeta
-        jacobian_i.append(self.data.i)
-        jacobian_j.append(self.model.pars['eta_calib'].indexof(self.lcdata.data['band_id']))
-        jacobian_val.append(norm * x0 * zz * (integral_surface_0 + x1*integral_surface_1)*(1+kappa))
+        jacobian_i.append(self.lcdata.row)
+        jacobian_j.append(self.model.pars['eta_calib'].indexof(self.lcdata.band_index))
+        jacobian_val.append(flux_scale * x0 * zz * (integral_surface_0 + x1*integral_surface_1)*(1+kappa))
 
         # dKappa
-        jacobian_i.append(self.data.i)
-        jacobian_j.append(self.model.pars['kappa_color'].indexof()[data['lc_id']])
-        jacobian_val.append(norm * x0 * zz * (integral_surface_0 + x1*integral_surface_1) * (1+eta))
-    
+        jacobian_i.append(self.lcdata.row)
+        jacobian_j.append(self.model.pars['kappa_color'].indexof(self.lcdata.band_index))
+        jacobian_val.append(flux_scale * x0 * zz * (integral_surface_0 + x1*integral_surface_1) * (1+eta))
+
         if self.model.disable_cache:
             self.model.clear_cache()
-        self.model.timing.append(time.time()-t0)
+        self.model.timing.append(time.perf_counter()-t0)
         return flux
 
 
 class SpectrumEvalUnitFast(object):
     r"""Evaluate the model for all SN spectra in the training dataset
-    
+
     This class is one of the two type of "eval units". Given a chunk
     of the training dataset which corresponds the spectral observations,
-    and given the :math:`(X_0, X_1, c, t_{max})` parameters 
+    and given the :math:`(X_0, X_1, c, t_{max})` parameters
     of the SN, compute the quantity:
-    
+
     .. math::
-    
+
          \frac{1}{1+z} \left[M_0\left(\frac{\lambda}{1+z}, \mathrm{p}\right) + X_1\ M_1\left(\frac{\lambda}{1+z},
          \mathrm{p}\right) \right]\ 10^{0.4\ c\ P(\frac{\lambda}{1+z})}\ s(\lambda_{rec})
 
     where
 
     .. math::
-        M_{0|1}(\lambda, \mathrm{p}) = \sum_{k\ell} \theta_{k\ell} B_k(\mathrm{p}) B_l(\mathrm{\lambda}) 
+        M_{0|1}(\lambda, \mathrm{p}) = \sum_{k\ell} \theta_{k\ell} B_k(\mathrm{p}) B_l(\mathrm{\lambda})
 
-    and 
+    and
 
     .. math::
          \mathrm{p} = \frac{t - t_{max}}{1+z}
 
     and where :math:`R_s(\lambda)` is a polynomial correction which
     absorbs the wavelength-dependent large scale calibration errors
     affecting the spectrum.
-    
+
     Again, the evaluation reduces to a sparse matrix multiplication.
 
     Attributes
     ----------
     training_dataset : nacl.dataset.TrainingDataset
         Data set of photometric and spectroscopic observations.
     data : nacl.dataset.SpectrumData
@@ -1256,41 +1479,43 @@
         ----------
         tds : nacl.dataset.TrainingDataset
             Data set of photometric and spectroscopic observations.
         model : nacl.models.salt.SALT2Like
             Model.
         """
         self.training_dataset = tds
-        self.data = tds.sp_data
+        self.data = tds.spec_data
         self.model = model
 
-        self.spec_id = self.data['spec_id']
-        self.sn_id = self.data['sn_id']
-        self.z = self.training_dataset.sne['z'][self.sn_id]
-        
-        # Look at that later 
+        self.spec_index = self.data.spec_index
+        self.sn_index = self.data.sn_index
+        # self.z = self.training_dataset.sn_data.z[self.sn_id]
+        self.z = self.data.z
+
+        # Look at that later
         self.color_law = model.color_law
         self.pars = model.pars
         self.basis = model.basis
-        
+
         self.wl_basis_size = len(model.basis.bx)
         self.ph_basis_size = len(model.basis.by)
-        
+
         # restframe wavelengths
-        self.restframe_wl = self.data['Wavelength']/(1.+self.z)
+        self.restframe_wl = self.data.wavelength/(1.+self.z)
         #        self.Jl = model.basis.bx.eval(self.restframe_wl).tocsr()
 
-        # and we can connect directly to the global parameters 
+        # and we can connect directly to the global parameters
         self.M0 = model.pars['M0'].full
         self.M1 = model.pars['M1'].full
         self.cl_pars = model.pars['CL'].full
-        
+
         # recalibration polynomial (one per spectrum, because we adapt to the spectrum wavelength range)
-        self.recal_func = SpectrumRecalibrationPolynomials(self.training_dataset, self.model,
-                                                           self.model.recalibration_degree)
+        #        self.recal_func = SpectrumRecalibrationPolynomials(self.training_dataset, self.model,
+        #                                                           self.model.recalibration_degree)
+        self.recal_func = self.model.recal_func
 
     def __call__(self, jac=False, debug_mode=False):
         r"""
         Evaluate the model for a all spectra
 
         Parameters
         ----------
@@ -1302,93 +1527,410 @@
         Returns
         -------
         val : numpy.array
             Model evaluations.
         jacobian : scipy.sparse.csr_matrix
             Jacobian matrix (if jac is true).
         """
-        t0 = time.time()
+        t0 = time.perf_counter()
         pars = self.pars
 
         # sn-related parameters
-        x0, x1 = pars['X0'].full[self.sn_id], pars['X1'].full[self.sn_id]
-        c, tmax = pars['c'].full[self.sn_id],  pars['tmax'].full[self.sn_id]
+        x0, x1 = pars['X0'].full[self.sn_index], pars['X1'].full[self.sn_index]
+        c, tmax = pars['col'].full[self.sn_index],  pars['tmax'].full[self.sn_index]
 
         # we need to re-evaluate the basis on the phases, since tmax changes
-        restframe_phases = (self.data['Date']-tmax)/(1.+self.z)
+        restframe_phases = (self.data.mjd-tmax)/(1.+self.z)
         jacobian = self.basis.eval(self.restframe_wl, restframe_phases + self.model.delta_phase).tocsr()
-        
+
         # model components
         component_0 = jacobian.dot(self.M0)
         component_1 = jacobian.dot(self.M1)
         polynome_color_law, jacobian_color_law = self.color_law(self.restframe_wl, self.cl_pars, jac=jac)
         color_law = np.power(10., 0.4*c*polynome_color_law)
         zz = 1. + self.z
-        
+
         # recalibration polynomial
+        # if we evaluate this, then recal_func must be instantiated
+        # if self.recal_func is not None:
+        assert self.recal_func is not None
         recal, jacobian_spec_rec = self.recal_func(jac=jac)
-        
+        if jacobian_spec_rec is not None:
+            jacobian_spec_rec = jacobian_spec_rec.tocoo()
+            # don't know what to do with this
+            # jacobian_spec_rec.data *= recal[jacobian_spec_rec.row]
+
         # recal = np.exp(recal)
         pca = (component_0 + x1 * component_1)
         model = pca * color_law * recal / zz
-        
+
         if debug_mode:
             return component_0, component_1, color_law, recal, model
-        
+
         self.model.val.append(model)
         if not jac:
-            self.model.timing.append(time.time()-t0)
+            self.model.timing.append(time.perf_counter()-t0)
             return model
 
         jacobian = jacobian.tocoo()
-        jacobian_spec_rec = jacobian_spec_rec.tocoo()
-        # jacobian_spec_rec.data *= recal[jacobian_spec_rec.row]
-        # X0 does not appear in the spectral part of the model 
+        # X0 does not appear in the spectral part of the model
         # hence, dmdX0 = 0
 
         # dMdX1
         jacobian_i, jacobian_j, jacobian_val = self.model.jacobian_i, self.model.jacobian_j, self.model.jacobian_val
-        jacobian_i.append(self.data.i)
-        jacobian_j.append(self.model.pars['X1'].indexof(self.sn_id))
+        jacobian_i.append(self.data.row)
+        jacobian_j.append(self.model.pars['X1'].indexof(self.sn_index))
         jacobian_val.append(component_1 * color_law * recal / zz)
 
         # dMdc
-        jacobian_i.append(self.data.i)
-        jacobian_j.append(self.model.pars['c'].indexof(self.sn_id))
+        jacobian_i.append(self.data.row)
+        jacobian_j.append(self.model.pars['col'].indexof(self.sn_index))
         jacobian_val.append(model * 0.4 * np.log(10.) * polynome_color_law)
 
         # dMdtmax
         # we can gain a little here, by not evaluating the gradient along the wavelength (ddlambda)
         _, deval_phase = self.model.basis.gradient(self.restframe_wl, restframe_phases + self.model.delta_phase)
         deval_phase = deval_phase.tocsr()
-        jacobian_i.append(self.data.i)
-        jacobian_j.append(self.model.pars['tmax'].indexof(self.sn_id))
+        jacobian_i.append(self.data.row)
+        jacobian_j.append(self.model.pars['tmax'].indexof(self.sn_index))
         jacobian_val.append(-1. * (deval_phase.dot(self.M0) + x1*deval_phase.dot(self.M1)) * color_law * recal / zz**2)
 
         # dmdtheta_0
-        jacobian_i.append(self.data.i[jacobian.row])
+        jacobian_i.append(self.data.row[jacobian.row])
         jacobian_j.append(self.model.pars['M0'].indexof(jacobian.col))
         jacobian_val.append(jacobian.data * color_law[jacobian.row] * recal[jacobian.row] / zz[jacobian.row])
 
         # dmdtheta_1
-        jacobian_i.append(self.data.i[jacobian.row])
+        jacobian_i.append(self.data.row[jacobian.row])
         jacobian_j.append(self.model.pars['M1'].indexof(jacobian.col))
         jacobian_val.append(x1[jacobian.row] * jacobian.data * color_law[jacobian.row] *
                             recal[jacobian.row] / zz[jacobian.row])
-                
+
         # dMdcl (color law)
         jacobian_color_law = scipy.sparse.coo_matrix(jacobian_color_law)
-        jacobian_i.append(self.data.i[jacobian_color_law.row])
+        jacobian_i.append(self.data.row[jacobian_color_law.row])
         jacobian_j.append(self.model.pars['CL'].indexof(jacobian_color_law.col))
         jacobian_val.append(c[jacobian_color_law.row] * 0.4 * np.log(10.) * jacobian_color_law.data *
                             model[jacobian_color_law.row])
-        
+
         # dMdr (recalibration)
-        jacobian_i.append(self.data.i[jacobian_spec_rec.row])
-        jacobian_j.append(self.model.pars['SpectrumRecalibration'].indexof(jacobian_spec_rec.col))
-        jacobian_val.append(jacobian_spec_rec.data * (pca*color_law)[jacobian_spec_rec.row]/zz[jacobian_spec_rec.row])
-        
+        if jacobian_spec_rec is not None:
+            jacobian_i.append(self.data.row[jacobian_spec_rec.row])
+            jacobian_j.append(self.model.pars['SpectrumRecalibration'].indexof(jacobian_spec_rec.col))
+            jacobian_val.append(jacobian_spec_rec.data * (pca*color_law)[jacobian_spec_rec.row]/zz[jacobian_spec_rec.row])
+
+        if self.model.disable_cache:
+            self.model.clear_cache()
+        self.model.timing.append(time.perf_counter()-t0)
+
+        return model
+
+
+class SpectroPhotoEvalUnit(object):
+
+    def __init__(self, tds, model):
+        """Constructor.
+
+        Parameters
+        ----------
+        tds : nacl.dataset.TrainingDataset
+            Data set of photometric and spectroscopic observations.
+        model : nacl.models.salt.SALT2Like
+            Model.
+        """
+        self.training_dataset = tds
+        self.data = tds.spectrophotometric_data
+        self.model = model
+
+        self.spec_index = self.data.spec_index
+        self.sn_index = self.data.sn_index
+        self.z = self.data.z
+
+        # Look at that later
+        self.color_law = model.color_law
+        self.pars = model.pars
+        self.basis = model.basis
+
+        self.wl_basis_size = len(model.basis.bx)
+        self.ph_basis_size = len(model.basis.by)
+
+        # restframe wavelengths
+        self.restframe_wl = self.data.wavelength/(1.+self.z)
+        #        self.Jl = model.basis.bx.eval(self.restframe_wl).tocsr()
+
+        # and we can connect directly to the global parameters
+        self.M0 = model.pars['M0'].full
+        self.M1 = model.pars['M1'].full
+        self.cl_pars = model.pars['CL'].full
+
+    def __call__(self, jac=False, debug_mode=False):
+        r"""
+        Evaluate the model for a all spectra
+
+        Parameters
+        ----------
+        jac : bool
+            if True compute and return the jacobian matrix
+        debug_mode : bool
+            if true, just return the model components.
+
+        Returns
+        -------
+        val : numpy.array
+            Model evaluations.
+        jacobian : scipy.sparse.csr_matrix
+            Jacobian matrix (if jac is true).
+        """
+
+        t0 = time.perf_counter()
+        pars = self.pars
+
+        # sn-related parameters
+        x0, x1 = pars['X0'].full[self.sn_index], pars['X1'].full[self.sn_index]
+        c, tmax = pars['col'].full[self.sn_index],  pars['tmax'].full[self.sn_index]
+        # c, tmax = pars['col'].full[self.sn_index],  pars['tmax'].full[self.training_dataset.spectrophotometric_data.isn]
+
+        # we need to re-evaluate the basis on the phases, since tmax changes
+        restframe_phases = (self.data.mjd-tmax)/(1.+self.z)
+        jacobian = self.basis.eval(self.restframe_wl, restframe_phases + self.model.delta_phase).tocsr()
+
+        # norm
+        norm = self.model.norm
+
+        # model components
+        component_0 = jacobian.dot(self.M0)
+        component_1 = jacobian.dot(self.M1)
+
+        polynome_color_law, jacobian_color_law = self.color_law(self.restframe_wl, self.cl_pars, jac=jac)
+        color_law = np.power(10., 0.4*c*polynome_color_law)
+        zz = 1. + self.z
+
+        pca = (component_0 + x1 * component_1)
+        model = x0 * norm * pca * color_law / zz
+
+        if debug_mode:
+            return component_0, component_1, color_law, recal, model
+
+        self.model.val.append(model)
+        if not jac:
+            self.model.timing.append(time.perf_counter()-t0)
+            return model
+
+        jacobian = jacobian.tocoo()
+        # jacobian_spec_rec = jacobian_spec_rec.tocoo()
+
+        jacobian_i, jacobian_j, jacobian_val = self.model.jacobian_i, self.model.jacobian_j, self.model.jacobian_val
+        jacobian_i.append(self.data.row)
+        jacobian_j.append(self.model.pars['X0'].indexof(self.sn_index))
+        # jacobian_val.append((component_0 + x1*component_1) * color_law * recal / zz)
+        jacobian_val.append(norm * pca * color_law / zz)
+
+        # dMdX1
+        # jacobian_i, jacobian_j, jacobian_val = self.model.jacobian_i, self.model.jacobian_j, self.model.jacobian_val
+        jacobian_i.append(self.data.row)
+        jacobian_j.append(self.model.pars['X1'].indexof(self.sn_index))
+        # jacobian_val.append(x0 * component_1 * color_law * recal / zz)
+        jacobian_val.append(x0 * norm * component_1 * color_law / zz)
+
+        # dMdc
+        jacobian_i.append(self.data.row)
+        jacobian_j.append(self.model.pars['col'].indexof(self.sn_index))
+        jacobian_val.append(model * 0.4 * np.log(10.) * polynome_color_law)
+
+        # dMdtmax
+        # we can gain a little here, by not evaluating the gradient along the wavelength (ddlambda)
+        _, deval_phase = self.model.basis.gradient(self.restframe_wl, restframe_phases + self.model.delta_phase)
+        deval_phase = deval_phase.tocsr()
+        jacobian_i.append(self.data.row)
+        jacobian_j.append(self.model.pars['tmax'].indexof(self.sn_index))
+        #jacobian_val.append(-1. *x0* (deval_phase.dot(self.M0) + x1*deval_phase.dot(self.M1)) * color_law * recal / zz**2)
+        jacobian_val.append(-1. * x0 * norm * (deval_phase.dot(self.M0) + x1*deval_phase.dot(self.M1)) * color_law / zz**2)
+
+        # dmdtheta_0
+        jacobian_i.append(self.data.row[jacobian.row])
+        jacobian_j.append(self.model.pars['M0'].indexof(jacobian.col))
+        #jacobian_val.append(x0[jacobian.row] *jacobian.data * color_law[jacobian.row] * recal[jacobian.row] / zz[jacobian.row])
+        jacobian_val.append(x0[jacobian.row] * norm * jacobian.data * color_law[jacobian.row] / zz[jacobian.row])
+
+        # dmdtheta_1
+        jacobian_i.append(self.data.row[jacobian.row])
+        jacobian_j.append(self.model.pars['M1'].indexof(jacobian.col))
+        #jacobian_val.append(x0[jacobian.row]*x1[jacobian.row] * jacobian.data * color_law[jacobian.row] *
+        #                    recal[jacobian.row] / zz[jacobian.row])
+        jacobian_val.append(x0[jacobian.row] * x1[jacobian.row] * norm *  jacobian.data * color_law[jacobian.row]/ zz[jacobian.row])
+
+        # dMdcl (color law)
+        jacobian_color_law = scipy.sparse.coo_matrix(jacobian_color_law)
+        jacobian_i.append(self.data.row[jacobian_color_law.row])
+        jacobian_j.append(self.model.pars['CL'].indexof(jacobian_color_law.col))
+        jacobian_val.append(c[jacobian_color_law.row] * 0.4 * np.log(10.) * jacobian_color_law.data *
+                            model[jacobian_color_law.row])
+
         if self.model.disable_cache:
             self.model.clear_cache()
-        self.model.timing.append(time.time()-t0)
-        
+        self.model.timing.append(time.perf_counter()-t0)
+
+
         return model
+
+
+class SALT2Eval:
+    """Evaluate the model, for one single SN
+    """
+    def __init__(self, model, bands=['SWOPE::B'],
+                 n_spectra=1, n_phot_spectra=1):
+        """
+        """
+        self.orig_model = model
+        self.phase_range = model.phase_range
+        self.wl_range = model.wl_range
+        self.tds = SimTrainingDataset(bands,
+                                      n_spectra=n_spectra,
+                                      n_phot_spectra=n_phot_spectra)
+        # it is essential that the model is an exact duplicate
+        # of the original model - just 1 SN instead of many
+        self.model = model.clone(self.tds)
+
+    # def clone_model(self):
+    #     """instantiate a duplicate of the original model
+
+    #     .. note :: a model should be able to clone itself - would be cleaner
+    #     """
+    #     model = self.orig_model
+    #     ret = \
+    #         SALT2Like(self.tds,
+    #                   phase_range=model.phase_range,
+    #                   wl_range=model.wl_range,
+    #                   basis_knots=model.basis_knots,
+    #                   basis_filter_knots=model.basis_filter_knots,
+    #                   spectrum_recal_degree=model.spectrum_recal_degree,
+    #                   normalization_band_name=model.normalization_band_name,
+    #                   calib_variance=model.calib_variance)
+    #     return ret
+
+    def set(self, **kwargs):
+        """initialize the sn parameters
+
+        This function updates the dataset, and then the model
+        parameters.
+        """
+        # sn parameters
+        if 'z' in kwargs:
+            z = kwargs.get('z')
+            self.tds.sn_data.nt['z'] = z
+            if self.tds.lc_data:
+                self.tds.lc_data.z[:] = z
+            if self.tds.spec_data:
+                self.tds.spec_data.z[:] = z
+            if self.tds.spectrophotometric_data:
+                self.tds.spectrophotometric_data.z[:] = z
+        if 'x0' in kwargs:
+            self.tds.sn_data.nt['x0'] = kwargs['x0']
+        if 'x1' in kwargs:
+            self.tds.sn_data.nt['x1'] = kwargs['x1']
+        if 'col' in kwargs:
+            self.tds.sn_data.nt['col'] = kwargs['col']
+        if 'tmax' in kwargs:
+            tmax = kwargs['tmax']
+            self.tds.sn_data.nt['tmax'] = kwargs['tmax']
+            if self.tds.lc_data:
+                self.tds.lc_data.nt['mjd'] = self.tds.mjd +tmax
+        if 'ebv' in kwargs:
+            self.tds.sn_data.nt['ebv'] = kwargs['ebv']
+
+        if 'spec_mjd' in kwargs:
+            if self.tds.spec_data:
+                self.tds.spec_data.nt['mjd'] = kwargs['spec_mjd']
+            if self.tds.spectrophotometric_data:
+                self.tds.spectrophotometric_data.nt['mjd'] = kwargs['spec_mjd']
+
+        # light curve zero points and magsys
+        if 'zp' in kwargs:
+            zps = kwargs['zp']
+            for band_name in zps:
+                idx = self.tds.lc_data.band == band_name
+                self.tds.lc_data.nt['zp'] = zps[band_name]
+        if 'magsys' in kwargs:
+            magsys = kwargs['magsys']
+            if type(magsys) is str:
+                self.tds.lc_data.nt['magsys'][:] = magsys
+            for band_name in magsys:
+                idx = self.tds.lc_data.magsys == band_name
+                self.tds.lc_data.nt['magsys'] = magsys[band_name]
+
+        # recompute the photometric norm factors
+        self.tds.compute_photometric_norm_factors()
+        # propagate this into the model parameters
+        self.model = self.orig_model.clone(self.tds)
+        self.model.init_from_training_dataset()
+
+    def set_from_tds(self, sn, tds):
+        """load the sn parameters from a training dataset
+        """
+        sn_pars = tds.get_sn_pars(sn)
+        if self.tds.lc_data:
+            sn_pars['zp'] = tds.get_zp(sn)
+            sn_pars['magsys'] = tds.get_magsys(sn)
+        self.set(**sn_pars)
+        # self.set(z=sn_pars['z'], x0=sn_pars['x0'],
+        #          x1=sn_pars['x1'], col=sn_pars['col'],
+        #          tmax=sn_pars['tmax'], ebv=sn_pars['ebv'],
+        #          zp=zp, magsys=magsys)
+
+    def update_global_pars(self, pars):
+        """
+        """
+        for block_name in ['M0', 'M1', 'CL']:
+            self.orig_model.pars[block_name].full[:] = pars[block_name].full[:]
+            self.model.pars[block_name].full[:] = pars[block_name].full[:]
+
+    def __call__(self):
+        """evaluate the model and update the dataset with the model values
+
+        This is the simplest way to evaluate the model.
+        No need to clone the dataset or anything.
+        """
+        v = self.model(self.model.pars.free)
+        self.tds.update_flux(v)
+
+    def bandflux(self, bands, mjds, zp, zpsys):
+        """evaluate the model for the requested bands and at the requested mjds
+
+        This one in a little more costly, as we need to instantiate
+        a new training dataset and re-instantiate a model.
+        """
+        pass
+
+    def bandmag(self, bands, mjd, magsys):
+        """return mags for the requested bands and at the requested mjds
+
+        This is also a little more costly, as we need to instantiate
+        a new training dataset and re-instantiate a model.
+        """
+        pass
+
+    def spectrum(self, mjd):
+        """evaluate and return a spectrophotometric spectrum
+        """
+        pass
+
+    def photspectrum(self, mjd):
+        """evaluate and return a spectrophotometric spectrum
+        """
+        pass
+
+    def color_law(self, col=None):
+        pass
+
+
+# def main():
+#     model = ...
+#     m = SALT2LikeEval(model, bands=['SWOPE::B'])
+
+#     # evaluate the model on all the data for this SN
+#     # with the default parameters
+#     m.eval(sn=sn)
+
+#     # evaluate the model on all the data for this SN
+#     # with alternative parameters
+#     m.eval(sn=sn, sn_pars=sn_pars, model_pars=model_pars)
+
```

### Comparing `sn-nacl-0.3/nacl/models/variancemodels.py` & `sn-nacl-0.4/nacl/util/salt2.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,421 +1,488 @@
 """
-None of the existing empirical models perfectly describes the training data. More
-specifically, at the end of the training, the measurement uncertainties do not explain
-the dispersion of the residuals at the fitted model.
-This means that there is variability from SN to SN,
-bearing on the shape of the light curves, or on the spectral structure that cannot be
-captured by a two parameter model.
-It is therefore essential to model this intrinsic residual variability of SNe by an
-error model. This one is an empirical function of the phase and the wavelength. It
-depends on parameters that must be adjusted during the training procedure.
-
-In this study, we have implemented a simple error model, as a proof of concept.
-of concept. It includes a purely diagonal part (error snake), as well as a non-diagonal
-part, which describes a specific error mode (color scatter) observed on the training.
+The SALT2 model. 
+
+SALT2 parameterizes the *restframe* spectrophotometric evolution of
+SNe Ia with two surfaces and a color law:
+
+.. math:: S_{10}(p, \lambda) = X_0 \\left(M_0(p, \lambda) + X_1 M_1(p,\lambda)\\right) C(\lambda)
+
+Given a passband, :math:`T(\lambda)`, the model allows one to compute
+an *observer frame* broadband flux:
+
+.. math:: f = \\frac{C\ 10^{-12}}{1+z} \int S_{10}\\left(p, \\frac{\lambda}{1+z}\\right)\ \lambda\ T(\lambda)\ d\lambda
+
 """
 
-import numpy as np
-import pylab as pl
-from scipy.sparse import coo_matrix, dia_matrix, csc_matrix
-from ..lib.bspline import BSpline, CardinalBSplineC, integ, BSpline2D, lgram
+import os
+import os.path as op
+import sys 
+import re
+
+import numpy as np 
+from scipy.sparse import coo_matrix
+
+from ..util.io import NTuple
+from ..lib.stellarlibs import FilterSet, ALIGN_WITH_INTEG_FLUX
+from ..lib.instruments import InstrumentModel 
 from ..lib.fitparameters import FitParameters
-try:
-    from sksparse.cholmod import cholesky_AAt
-except ImportError:
-    from scikits.sparse.cholmod import cholesky_AAt
-
-
-class ColorScatter(object):
-    r"""
-    To model the residual variability of the SNe color not described by the model, we allow the relative amplitude of
-    each light curve to vary by a quantity :math:`(1+kappa)`:
-
-    .. math::
-        \phi_{phot}(p_0) = X_0 (1+z) (1+kappa) \int S(\lambda, p) T\left( \lambda \right) \frac{\lambda}{hc} d\lambda
-
-    where :math:`\kappa` is an additional parameter, depending on the SN and the observation band.
-
-    The variability of :math:`\kappa` is defined by a centered Gaussian a priori and whose variance depends on the
-    wavelength restframe, and must be determined during the adjustment.
-    In our model, this term is implemented by a polynomial of the wavelength restframe of the SN. For a light curve
-    observed in a band :math:`X`, of average wavelength :math:`\lambda^X`, the corresponding variance is:
-
-    .. math::
-        \sigma_\kappa^2 = P\left(\frac{\lambda^X}{1+z}\right)
-
-    where :math:`z` is redshift of the supernova and :math:`P` is a polynomial of the wavelength restframe.
-    In practice, :math:`P` is implemented in terms of a reduced restframe wavelength: :math:`\lambda_{r}`
-
-    Attributes
-    ----------
-    WL_REDUCED : numpy.array
-        Reduced SN-restframe mean wavelength
-    pars : nacl.lib.fitparameters.FitParameters
-        Color scatter parameter.
+from ..lib.bspline import BSpline, BSpline2D, lgram
+from . import saltpath
+
+
+def load_filters(bands):
+    """
+    Load all the filters that are requested in argument and return a
+    FilterSet
+    
+    .. note :: this function is currently slow, because no instrument
+               cache implemented.
     """
-    U_WAVELENGTH = 3650.88
-    B_WAVELENGTH = 4302.57
-    V_WAVELENGTH = 5428.55
-    R_WAVELENGTH = 6418.01
-    I_WAVELENGTH = 7968.34
-    WAVELENGTH = {"U": U_WAVELENGTH, "B": B_WAVELENGTH, "V": V_WAVELENGTH,
-                  "R": R_WAVELENGTH, "I": I_WAVELENGTH}
+    instrument_names = np.unique([re.search('(.+)::(.+)', bn).group(1) for bn in bands])
+    instruments = [InstrumentModel(nm) for nm in instrument_names]
+    instruments = dict(list(zip(instrument_names, instruments)))
+    tr, lmin, lmax = [], [], []
+    for bn in bands:
+        instr, band = re.search('(.+)::(.+)', bn).groups()
+        f = instruments[instr].EffectiveFilterByBand(band)
+        lmin.append(f.x_min)
+        lmax.append(f.x_max)
+        tr.append(f)
+    gwl = np.arange(min(2000., np.min(lmin)), 
+                    max(11000., np.max(lmax)), 5.)
+    basis = BSpline(gwl, order=2)
+    return FilterSet(basis, tr)
 
-    def __init__(self, wavelength_rest_reduced, sigma_kappa):
-        """
-        Constructor - computes the arguments
 
-        Parameters
-        ----------
-        wavelength_rest_reduced :
-            Reduced SN-restframe mean wavelength
-        sigma_kappa : numpy.array
-            Color scatter parameter initialisation.
-        """
-        self.WL_REDUCED = wavelength_rest_reduced
-        self.pars = self.init_pars(sigma_kappa)
+class ModelComponents(object):
+    """Basic ingredients of the SALT2 model
+    
+    Holds all the model ingredients that are shared between all supernovae:
+      - model validity area in phase and wavelength
+      - BSpline basis definitions
+      - surfaces
+      - color law
+      - error snakes
+      - color smearing laws
+    """
+    def __init__(self, filename=None):
+        self.basis, self.wl_basis, self.phase_basis = None, None, None
+        self.M0, self.M1 = None, None
+        self.cl = None
+        if filename is not None:
+            self.load(filename)
+
+    def save(self, filename):
+        if self.basis is None:
+            return 
+        np.savez(filename, 
+                 wl_grid=self.wl_basis.grid,
+                 phase_grid=self.phase_basis.grid, 
+                 M0=self.M0, 
+                 M1=self.M1, 
+                 CL_pars=self.cl.pars, 
+                 CL_range=[self.cl.min_lambda, self.cl.max_lambda])
+    
+    def load(self, filename):
+        arrs = np.load(filename)
+        wl_grid, phase_grid = arrs['wl_grid'], arrs['phase_grid']
+        self.basis = BSpline2D(wl_grid, phase_grid, x_order=4, y_order=4)
+        self.wl_basis = self.basis.bx
+        self.phase_basis = self.basis.by
+        self.M0, self.M1 = arrs['M0'], arrs['M1']
+        self.cl = ColorLaw(arrs['CL_pars'], arrs['CL_range'])
 
     @staticmethod
-    def init_pars(sigma_kappa):
+    def load_from_saltpath():
+        """load the SALT2 model from an "official" SALT2 repository
         """
-        Parameters initialisation.
 
-        Parameters
-        ----------
-        sigma_kappa : numpy.array
-            Color scatter parameter initialisation.
-
-        Returns
-        -------
-        pars : nacl.lib.fitparameters.FitParameters
-            Color scatter parameter.
-        """
-        pars = FitParameters([('sigma_kappa', len(sigma_kappa))])
-        pars['sigma_kappa'] = sigma_kappa
-        return pars
+        phase_grid = np.linspace(-20., 51., 50)
+        wl_grid    = np.linspace(2000., 9201., 300)
+        basis      = BSpline2D(phase_grid, wl_grid, x_order=4, y_order=4)
         
-    def __call__(self, sk, jac=False):
-        """
-        Evaluate the color scatter.
+        cfg = saltpath.read_card_file(saltpath.fitmodel_filename)
+        salt2_model_path = saltpath.SALTPATH + os.sep + cfg['SALT2']
+    
+        # first surface
+        M0_filename = salt2_model_path + os.sep + 'salt2_template_0.dat'
+        d = NTuple.fromtxt(M0_filename)
+        phase, wl, flx = d['f0'].copy(), d['f1'].copy(), d['f2'].copy()
+        M0 = basis.linear_fit(phase, wl, flx)
+    
+        # second surface 
+        M1_filename = salt2_model_path + os.sep + 'salt2_template_1.dat'
+        d = NTuple.fromtxt(M1_filename)
+        phase, wl, flx = d['f0'].copy(), d['f1'].copy(), d['f2'].copy()
+        M1 = basis.linear_fit(phase, wl, flx)
+    
+        # color law 
+        print((salt2_model_path + os.sep + 'salt2_color_correction.dat'))
+        cl_filename = salt2_model_path + os.sep + 'salt2_color_correction.dat'
+        with open(cl_filename) as f:
+            deg = int(f.readline())
+            p = []
+            for i in range(deg):
+                p.append(float(f.readline()))
+            r = {}
+            for line in f:
+                field, value = re.search('^Salt2ExtinctionLaw\.([\w_]+)\s*([\d\.+-]+)', line).groups()
+                r[field] = float(value)
+            assert 'version' in r and r['version'] == 1.0
+        
+        ret = ModelComponents()
+        ret.basis = basis
+        ret.phase_basis = basis.bx
+        ret.wl_basis = basis.by
+        ret.M0 = M0.reshape(len(ret.wl_basis), -1)
+        ret.M1 = M1.reshape(len(ret.wl_basis), -1)
+        alpha = 1. - np.sum(p)
+        p = np.asarray(p[::-1] + [alpha])
+        ret.cl = ColorLaw(p, (r['min_lambda'], r['max_lambda']))
+        ret.CC = ret.cl(ret.wl_basis.grid, 1.)
+        return ret
+
 
-        Parameters
-        ----------
-        sk : numpy.array
-            Color scatter parameter
-
-        Returns
-        -------
-        val : numpy.array
-            Color scatter evaluation, square root of the diagonal term of the color scatter 
-            matrix.
-        if jac:
-            jacobian of the color scatter.
+class ColorLaw(object):
+    """Implementation of the SALT2 color law (version 1)
+    
+    The SALT2 color law describes the color diversity of SNeIa. It is
+    fitted from a training sample. In SALT 2.4, the color law is
+    parametrized as follows:
+    
+    .. math:: C(\lambda;c) = 10^{0.4 (c \times P(\lambda))}
+
+    where :math:`P(\lambda)` is a polynomial, such as
+    :math:`P(\lambda_B) = 1` and :math:`P(\lambda_V) = 0` It is
+    defined in the wavelength range :math:`2800 A < \lambda < 7000 A`
+    """
+    WAVELENGTH = {"U": 3650.88, "B": 4302.57, "V": 5428.55, "R": 6418.01, "I": 7968.34}
+    U_WAVELENGTH=3650.88
+    B_WAVELENGTH=4302.57
+    V_WAVELENGTH=5428.55
+    R_WAVELENGTH=6418.01
+    I_WAVELENGTH=7968.34
+    
+    def __init__(self, pars, wl_range):
+        """Constructor - computes the arguments 
+        
         """
-        self.pars.free = sk
-        sigma_kappa = self.pars.full[:]
-        val = np.polyval(sigma_kappa, self.WL_REDUCED)  # * self.WL_REDUCED
-    
-        if jac:
-            vander = (np.vander(self.WL_REDUCED, len(sigma_kappa)).T )  # * self.WL_REDUCED)
-            jj = (vander * val * 2).T
-            return val, jj  # coo_matrix(jj)
-        return val
-
-
-class SimpleVarianceModel(object):
-    r"""
-    Implementation of the error snake,  residuals variability coming from SN Ia variability
-    not modeled and instrumental uncertainty not took into account.
-    The diagonal part of the error model (error snake) can be understood as the contribution
-    of the higher order terms of the PCA, having been truncated.
-
-    Variance model, function of the flux both for photometry and spectroscopy
-    (indiscriminately represented by X)
-
-    .. math::
-    V(\lambda, p) = \sigma_{Err}^2 + \sigma_{\mathrm{Mod}}^2(\lambda,p)
-
-    where :
-
-    .. math::
-        \sigma_{\mathrm{Mod}}^{spec} &= g(\lambda, p) \times \phi_{\mathrm{spec}}(p,\lambda)\ \ (\mathrm{spectra}) \\
-        \sigma_{\mathrm{Mod}}^{phot} &= g(\lambda, p) \times \phi_{\mathrm{phot}}(p,\lambda)\ \ (\mathrm{photometric})
-
-    :math:`\gamma(\lambda, p)` is a global surface describing the spectral residual of
-    a 2D spline surface defined on the same ranges as the corresponding model.
-
-
-    Attributes
-    ----------
-    disconnect_sp : bool
-        Whether error snake of spectral data is considered.
-    model : nacl.salt
-        Model.
-    sp : nacl.dataset.SpectrumData
-        Spectral data
-    lc : nacl.dataset.LcData
-        Photometric data
-    filter_db : nacl.instruments.FilterDb
-        Filter transmission projected on B-splines
-    bands : numpy.array
-        Bands used for photometric data
-    threshold : int
-        Fix the spline parameters for bin that gather less data points than this threshold value.
-    wl_grid : numpy.array
-        Wavelength grid.
-    phase_grid : numpy.array
-        Phase grid.
-    basis : nacl.lib.bspline.BSpline2D
-        2D spline basis.
-    factor_int : float
-        Model normalisation.
-    lambda_c : numpy.array
-        Mean wavelength of the filter in the SN-restframe.
-    pars : nacl.lib.fitparameters.FitParameters
-        Parameters :math:`\gamma`.
-    pars0 : numpy.array
-        Parameters used to initialize the error snake.
+        assert(wl_range[0] < wl_range[1])
+        self.min_lambda, self.max_lambda = wl_range
+        
+        self.pars = pars
+        
+        self.min_reduced_lambda = self.reduce(self.min_lambda)
+        self.max_reduced_lambda = self.reduce(self.max_lambda)
+        
+        dpars = np.polyder(self.pars)
+        
+        # uv side 
+        val = np.polyval(self.pars, self.min_reduced_lambda)
+        dval = np.polyval(dpars, self.min_reduced_lambda)
+        self.pars_uv = np.asarray([dval * self.min_reduced_lambda + val,
+                                   val * self.min_reduced_lambda])
+        # ir side 
+        val = np.polyval(self.pars, self.max_reduced_lambda)
+        dval = np.polyval(dpars, self.max_reduced_lambda)
+        self.pars_ir = np.asarray([dval * self.max_reduced_lambda + val,
+                                   val * self.max_reduced_lambda])
+        
+    def reduce(self, wl):
+        B_WL, V_WL = self.WAVELENGTH["B"], self.WAVELENGTH["V"]
+        return (wl-B_WL)/(V_WL-B_WL);
+    
+    def __call__(self, wl, color):
+        rwl = self.reduce(np.asarray(wl))
+        r = np.polyval(self.pars, rwl) * rwl
+        idx_uv = rwl<self.min_reduced_lambda
+        r[idx_uv] = np.polyval(self.pars_uv, rwl[idx_uv]-self.min_reduced_lambda)
+        idx_ir = rwl>self.max_reduced_lambda
+        r[idx_ir] = np.polyval(self.pars_ir, rwl[idx_ir]-self.max_reduced_lambda)
+        return np.power(10., 0.4 * color * r)
+
+
+def precompute_filter_effective_restframe_lambda(model, fs, zgrid):
+    """re
     """
-    def __init__(self, model, gamma_init=0.01,  disconnect_sp=False, threshold=None,
-                 adaptative_grid=False, bins=(3, 3), order=4):
-        r"""
-        Constructor.
-        - instantiate the bases (phase, wavelength)
-        - compute the \lambda_c for each light curve
-        - initiate the parameters
-        
-
-        Parameters
-        ----------
-        model : nacl.salt
-            Model.
-        gamma_init : numpy.array ou float
-            Parameters used to initialize the error snake.
-        disconnect_sp : bool
-            Whether error snake of spectral data is considered.
-        threshold : int
-            Fix the spline parameters for bin that gather less data points than this threshold value.
-        adaptative_grid : bool
-            It true, define Bspline knots where parameter space has data.
-        bins : tuple
-            Number of bins if the grid is not adaptative.
-        order :
-            Spline order.
+    def effective_lambda(model, fs, z):
         """
-        self.disconnect_sp = disconnect_sp
+        Compute 
+        \int \lambda^2 B_i(\lambda) B_j(\lambda (1+z)) d\lambda / \int \lambda B_i B_j d\lambda
+        """
+        G  = coo_matrix(lgram(model.wl_basis, fs.basis, z=z))
+        G2 = coo_matrix(lgram(model.wl_basis, fs.basis, z=z, lambda_power=2))
+        assert ~np.any(G.row-G2.row) and ~np.any(G.col-G2.col)
+        leff = G2.data/G.data
+        L = coo_matrix((leff, (G.row, G.col)), shape=G.shape)
+        N = coo_matrix((np.ones_like(leff), (G.row, G.col)), shape=G.shape)
+        leff = np.array(L.sum(axis=1)).squeeze()
+        N = np.array(N.sum(axis=1)).squeeze()
+        idx = N>0
+        leff[idx] /= N[idx]
+        return leff
         
-        self.model = model
-        self.lc = self.model.training_dataset.lc_data
-        self.sp = self.model.training_dataset.spec_data
-        self.filter_db = self.model.filter_db
-        self.bands = self.model.bands
-        self.threshold = threshold
-        
-        ph_bin, wl_bin = bins
-        order = order
-
-        if adaptative_grid:
-            phase_lc = self.model.get_restframe_phases(self.lc)
-            phase_sp = self.model.get_restframe_phases(self.sp)
-            wavelength_lc = self.lc['Wavelength']/(1 + self.lc['ZHelio'])
-            wavelength_sp = self.sp['Wavelength']/(1 + self.sp['ZHelio'])
-            phase = np.hstack((phase_sp, phase_lc))
-            wavelength = np.hstack((wavelength_sp, wavelength_lc))
-            _, self.wl_grid, self.phase_grid, _ = pl.hist2d(wavelength, phase, bins=2)
+    #    self.CC = self.model.cl(self.leff / (1.+self.z), 1.)
+    #    self.CC[~idx] = 1.
+    leff = []
+    # refine the z_grid
+    for z in zgrid:
+        leff.append(effective_lambda(model, fs, z))
+        print((z, leff[-1][0], leff[-1][-1]))
+    leff = np.vstack(leff)
+    bs = BSpline2D(model.wl_basis.grid, zgrid, x_order=1, y_order=1)
+    X,Y = np.meshgrid(model.wl_basis.grid, zgrid)
+    
+    return bs, X.flatten(), Y.flatten(), leff
 
-        else:
-            
-            print(f'\n VarModel N bins : ph : {ph_bin}, wl {wl_bin}')
-            self.phase_grid = np.linspace(model.basis.by.range[0], model.basis.by.range[-1], ph_bin)
-            self.wl_grid = np.linspace(model.basis.bx.range[0], model.basis.bx.range[-1], wl_bin)
-
-        self.basis = BSpline2D(self.wl_grid, self.phase_grid,
-                               x_order=order,
-                               y_order=order)
-        
-        self.factor_int = self.model.norm
-        if self.lc['Wavelength'].sum() == 0:
-            filter_mean_wl = [self.model.filter_db.transmission_db[bd].mean() for bd in self.model.bands.astype(str)]
-            self.lambda_c = np.array(filter_mean_wl)[self.lc['band_id']]/(1+self.lc['ZHelio']) 
-        else:
-            self.lambda_c = self.lc['Wavelength']/(1+self.lc['ZHelio'])
 
-        self.pars = self.init_pars(gamma_init=gamma_init)
-        self.pars0 = self.pars.full.copy()
+    
+def param_setter(name):
+    def set_param(self, val):
+        self.pars[name] = val
+    return set_param
 
-    def fix_non_constrain_pars(self, threshold):
-        """
-        Return index of parameters of the parameter space that don't have enough data to constraint the error snake.
 
-        Parameters
-        ----------
-        threshold : int
-            Threshold value defining the "enough". If the sum of the data in a bin is less than this value,
-            the corresponding parameter is fixed.
-
-        Returns
-        ----------
-        idx : numpy.array
-            Index of parameters that will be fixed.
-        """
-        lcs = self.model.training_dataset.lc_data
-        sps = self.model.training_dataset.spec_data
-        ph_sp = self.model.get_restframe_phases(sps)
-        ph_lc = self.model.get_restframe_phases(lcs)
-        wl_sp = sps['Wavelength']/(1 + sps['ZHelio'])
-        wl_lc = lcs['Wavelength']/(1 + lcs['ZHelio'])
-
-        x = np.hstack((wl_sp, wl_lc))
-        y = np.hstack((ph_sp, ph_lc))
-        jj = self.basis.eval(x, y)
+def param_getter(name):
+    def get_param(self):
+        return self.pars[name].full[0]
+    return get_param
 
-        idx = np.where(np.bincount(np.sort(jj.col)) < threshold)
-        return idx[0] 
 
-    def init_pars(self, gamma_init):
-        """
-        Initiate model parameters.
+class SALT2(object):
+    """Evaluate the SALT2 model for a specific supernova
+
+    An instance of this class takes as an input a list of observations
+    (MJDs, bands).  It precomputes and caches everything that can be
+    pre-computed, essentially, the color law, the gram at that
+    redshift and the Gram folded with the passband coefficients.  
+
+    When __call__'ed with a parameter vector, it evaluates the SALT2
+    model for each observation.
+    
+    """
+    def __init__(self, mjds, bands, model, filterset, z=0., wl_range=(3000., 8000.)):
+        """Constructor
 
-        Parameters
-        ----------
-        gamma_init : float
-            Parameters used to initialize the error snake.
-
-        Returns
-        ----------
-        gamma : nacl.lib.fitparameters.FitParameters
-            Parameters :math:`\gamma`.
+        Stores the list of observations, initialize a parameter vector, 
+        
         """
-        gamma = FitParameters([('gamma', self.basis.bx.nj * self.basis.by.nj)])
-        gamma['gamma'] = gamma_init
-        if self.threshold is not None:
-            idx = self.fix_non_constrain_pars(self.threshold)
-            print(idx)
-            print(gamma.free.shape)
-            gamma.fix(idx)
-            print(gamma.free.shape)
-        return gamma
-                    
-    def __call__(self, gamma, beta, jacobian=None, debug_mode=False, lc=None, sp=None):
-        r"""
-        Evaluate the model for a set of parameter :math:`\gamma` (variance model parameters)
-        and :math:`\beta` (flux model parameters).
-        
-
-        Parameters
-        ----------
-        gamma : np.array
-           set of parameter of the variance model;
-        beta : np.array
-           set of parameter of the flux model;
-        jacobian : None or scipy.sparse.coo_matrix
-           derivative of the flux, not necessary if derivative of variance model not needed,
-        debug_mode : bool
-           to get some variables...
-        lc : nacl.dataset.LcData
-           to get variance model of a set of light curve and is None will get for all
-        sp : nacl.dataset.SpectrumData
-           to get variance model of a set of spectra and is None will get for all
-
-        Returns
-        ----------
-        var : numpy.array
-            Variance value of the model, quadratic sum of the error measurement and the error snake.
-        if jacobian is not None:
-        var : numpy.array
-            Variance value of the model, quadratic sum of the error measurement and the error snake.
-        jacobian_var : scipy.sparse.coo_matrix
-            Jacobian (derivatives wrt :math:`\beta` and :math:`\gamma`)matrix of the error model.
+        # basic stuff 
+        self.mjds = mjds
+        self.bands = bands
+        #        self.bands_unique, self.band_index =
+        self.build_band_index(bands)
+        self.model = model
+        # assumes filterset has all bands that are needed
+        self.filterset = filterset
+        # expect M0 and M1 to be matrices
+        self.M0, self.M1 = model.M0, model.M1
+        self.restframe_wavelength_range = wl_range
+        
+        # set up an internal parameter vector 
+        self.pars = self.init_pars()
+        
+        # set the redshift. This triggers a recompute 
+        # of the Gram and Fz matrices and the color law
+        self.z = z
+        
+    # properties, for easy access to the internal parameter vector (somewhat slow)
+    X0 = property(fget=param_getter('X0'), fset=param_setter('X0'))
+    X1 = property(fget=param_getter('X1'), fset=param_setter('X1'))
+    Color = property(fget=param_getter('Color'), fset=param_setter('Color'))
+    DayMax = property(fget=param_getter('DayMax'), fset=param_setter('DayMax'))
+
+    # special property for z, because when we change z, 
+    # we have to recompute the grams and the color law...
+    @property
+    def z(self):
+        return self.pars['z'].full[0]
+    @z.setter
+    def z(self, val):
+        self.pars['z'] = val
+        self.G, self.Fz = self.init_fz()
+        self.init_CC()
+
+    def build_band_index(self, bands):
+        self.bands_unique = np.unique(bands)
+        idx = dict(list(zip(self.bands_unique, np.arange(len(self.bands_unique)))))
+        self.band_index = np.array([idx[b] for b in bands])
+        return self.bands_unique, self.band_index        
+        
+    def init_fz(self):
+        """creates and return the F(z) matrix
         """
-        if lc is None:
-            lc = self.lc
-        if sp is None:
-            sp = self.sp
-        lambda_c = self.lambda_c[lc['i']]
-
-        self.model.pars.free = beta
-        flux = self.model(beta, jac=False)
-        self.pars.full[:] = gamma
-
-        phase_lc = (lc['Date']-self.model.pars['tmax'].full[lc['sn_id']])/(1+lc['ZHelio'])
-        phase_sp = (sp['Date']-self.model.pars['tmax'].full[sp['sn_id']])/(1+sp['ZHelio'])
-
-        if self.disconnect_sp:
-            sigma_spectra = np.zeros_like(phase_sp)
-        else:
-            wl_sp = np.array(sp['Wavelength'])/(1+sp['ZHelio'])
-            spline_sp = self.basis.eval(wl_sp, phase_sp)
-            flux_sp = flux[sp['i']]
-            ss_sp = (spline_sp * self.pars['gamma'].full)
-            sigma_spectra = ss_sp * flux_sp
-
-        spline_lc = self.basis.eval(lambda_c, phase_lc)
-        flux_lc = flux[lc['i']] 
-        ss_lc = (spline_lc * self.pars['gamma'].full)
-        sigma_lightcurve = ss_lc * flux_lc
-        sig = np.hstack((sigma_lightcurve, sigma_spectra))
-        flux_err = np.hstack((lc['FluxErr'], sp['FluxErr']))
-        var = sig**2 + flux_err**2 
-        
-        if jacobian is not None:
-            n_pars, n_data = len(self.model.pars.free) + len(self.pars.free), len(sig)
-            v, jacobian = self.model(beta, jac=True)
-
-            if self.disconnect_sp:
-                i_dp, j_dp, jacobian_pars, i_dg0, j_dg0, jacobian_gamma = [], [], [], [], [], []
-            else:
-                jacobian_spectra = jacobian.tocsc()[sp['i']].tocoo()
-                # dp
-                i_dp = jacobian_spectra.row.copy()
-                j_dp = jacobian_spectra.col.copy()
-                jacobian_pars = 2 * jacobian_spectra.data * (sigma_spectra * ss_sp)[i_dp]
-                
-                # dtmax
-                idx = self.model.pars['tmax'].indexof(sp['sn_id'])
-                jacobian_wrt_phase, jacobian_wrt_wavelength = self.basis.gradient(wl_sp,
-                                                                                  phase_sp + self.model.delta_phase)
-                if len(jacobian_pars) != 0.:
-                    jacobian_pars[idx] -= 2 * (jacobian_wrt_phase * self.pars['gamma'].full) / \
-                                          (1+sp['ZHelio']) * v[sp['i']] * sigma_spectra
-                # dg
-                i_dg0 = spline_sp.row.copy()
-                j_dg0 = self.pars['gamma'].indexof(spline_sp.col) + len(self.model.pars.free)
-                jacobian_gamma = 2 * v[sp['i']][i_dg0]**2 * spline_sp.data * ss_sp[i_dg0]
-                if debug_mode:
-                    return i_dp, j_dp, jacobian_pars, i_dg0, j_dg0, jacobian_gamma, v, sp, spline_sp, ss_sp
+        G = lgram(self.model.wl_basis, self.filterset.basis, z=self.z)
+        Fz = np.vstack([G * self.filterset[b] for b in self.bands_unique])
+        return G, Fz
+    
+    def init_CC(self):
+        """evaluate the color law
+        """
+        if not hasattr(self, 'G'):
+            self.G = lgram(self.model.wl_basis, self.filterset.basis, z=self.z)
+        G = coo_matrix(self.G)
+        self.G2 = lgram(self.model.wl_basis, self.filterset.basis, z=self.z, lambda_power=2)
+        G2 = coo_matrix(self.G2)
+        assert ~np.any(G.row-G2.row) and ~np.any(G.col-G2.col)
+        leff = G2.data/G.data
+        L = self.L = coo_matrix((leff, (G.row, G.col)), shape=G.shape)
+        N = self.N = coo_matrix((np.ones_like(leff), (G.row, G.col)), shape=G.shape)
+        self.leff = np.array(L.sum(axis=1)).squeeze()
+        N = np.array(N.sum(axis=1)).squeeze()
+        idx = N>0
+        self.leff[idx] /= N[idx]
+        self.CC = self.model.cl(self.leff / (1.+self.z), 1.)
+        self.CC[~idx] = 1.
+
+    def mask_forbidden_bands(self):
+        """evaluate the mask
+        """
+        mean_restframe_wavelength = self.filterset.mean_wavelength(self.bands) / (1.+ self.z)
+        blue_cutoff, red_cutoff = self.restframe_wavelength_range
+        return (mean_restframe_wavelength>blue_cutoff) & (mean_restframe_wavelength<red_cutoff)
+        
+    @staticmethod
+    def init_pars():
+        p = FitParameters([('X0', 1), ('X1', 1), ('Color', 1), ('DayMax', 1), ('z', 1)])
+        p['X0'] = 1.
+        p['X1'] = 0.
+        p['Color'] = 0.
+        p['DayMax'] = 0.
+        p['z'] = 0.
+        p.fix('z')
+        return p
+    
+    def __call__(self, p=None, jac=False):
+        """evaluate the model and its derivatives (optional)
+        
+        The broadband flux is given by:
 
-            v_lc = v[lc['i']]
-            jacobian_lightcurve = jacobian.tocsc()[lc['i']].tocoo()
-            
-            i_dp_lc = jacobian_lightcurve.row.copy()
-            j_dp_lc = jacobian_lightcurve.col.copy()
-            jacobian_pars_lightcurve = 2 * jacobian_lightcurve.data * (sigma_lightcurve * ss_lc)[i_dp_lc]
-            
-            # dtmax
-            if self.model.pars['tmax'].indexof().sum() != len(self.model.pars['tmax'].full) * -1:
-                jacobian_wrt_phase, jacobian_wrt_wavelength = self.basis.gradient(lambda_c,
-                                                                                        phase_lc +
-                                                                                        self.model.delta_phase)
-                idx_lc = np.where(np.in1d(jacobian_lightcurve.col, self.model.pars['tmax'].indexof()))
-                if len(jacobian_pars_lightcurve) != 0.:
-                    jacobian_pars_lightcurve[idx_lc] -= 2 * (jacobian_wrt_phase * self.pars['gamma'].full) / (1+lc['ZHelio']) * v_lc * sigma_lightcurve
-                
-            # dg
-            i_dg0_lc = spline_lc.row.copy()
-            j_dg0_lc = self.pars['gamma'].indexof(spline_lc.col) + len(self.model.pars.free)
-            jacobian_gamma_lightcurve = 2 * v_lc[i_dg0_lc] ** 2 * spline_lc.data * ss_lc[i_dg0_lc]
-            
-            if len(i_dg0) != 0:
-                i_dg0 += len(lc)
-            if len(i_dp) != 0:
-                i_dp += len(lc)
+        .. math:: F(p) = X_0 \times \\left(I_0 + X_1 I_1\\right)) \\times  10^{0.4 c P(\lambda)}
+        """
+        if p is not None:
+            self.pars.free = p 
+        M0, M1, Fz = self.M0, self.M1, self.Fz
+        z, X0, X1, Color, DayMax = self.z, self.X0, self.X1, self.Color, self.DayMax
+        
+        phase = (self.mjds-DayMax) / (1. + self.z)
+
+        # using a sparse csc() makes a noticeable difference
+        # (x4 in speed with respect to multiply dense matrices)
+        # even in the other matrix (M0, M1) is dense
+        # (M0, M1 has to be a matrix though, not an array)
+        # 
+        # *TODO*: understand what underlying function is called
+        # 
+        P = self.model.phase_basis.eval(phase).tocsc()
+        CC = np.power(self.CC, Color)
+        M0_CC  = np.matrix(self.M0.T * CC)
+        M1_CC  = np.matrix(self.M1.T * CC)
+        Fz = Fz[self.band_index]
+        I0 = (np.array(P * M0_CC) * Fz).sum(axis=1)
+        I1 = (np.array(P * M1_CC) * Fz).sum(axis=1)
+        
+        # OLD version 
+        #        # seems to be much faster with dense matrices
+        #        P = self.model.phase_basis.eval(phase).todense()
+        #        CC = np.power(self.CC, Color)
+        #        I0 = (np.array(P * (M0.T * CC)) * Fz).sum(axis=1)
+        #        I1 = (np.array(P * (M1.T * CC)) * Fz).sum(axis=1)        
+        
+        # I add the (1+z) factor and the ALIGN_WITH_INTEG_FLUX here
+        norm = 1.E-12 * (1.+z) * ALIGN_WITH_INTEG_FLUX
+        flux = norm * X0 * (I0 + X1*I1)
+        
+        # no derivatives ? just return the model value 
+        if not jac:
+            return flux
+        
+        # compute the derivatives w.r.t. parameters 
+        n, N = len(self.pars.free), len(phase)
+        J = np.zeros((N,n))
+        
+        # ddX0
+        i = self.pars['X0'].indexof(0)
+        if i>=0:
+            J[:, i] = norm * (I0 + X1*I1)
             
-            i = np.hstack((i_dp, i_dg0, i_dp_lc, i_dg0_lc))
-            j = np.hstack((j_dp, j_dg0, j_dp_lc, j_dg0_lc))
-            val = np.hstack((jacobian_pars, jacobian_gamma, jacobian_pars_lightcurve, jacobian_gamma_lightcurve))
-             
-            idx_zeros = np.where((j != -1))[0]
-            jacobian_var = coo_matrix((val[idx_zeros], (i[idx_zeros], j[idx_zeros])), shape=(n_data, n_pars))
+        # ddX1
+        i = self.pars['X1'].indexof(0)
+        if i>=0:
+            J[:, i] = norm * (X0 * I1)
+        
+        # ddDayMax 
+        i = self.pars['DayMax'].indexof(0)
+        if i>=0:
+            #            dP = self.model.phase_basis.deriv(phase).todense() * (-1. / (1.+z))
+            dP = self.model.phase_basis.deriv(phase)
+            dP.data *= (-1. / (1.+z))
+            dP = dP.tocsc()
+            dI0 = (np.array(dP * M0_CC) * Fz).sum(axis=1)
+            dI1 = (np.array(dP * M0_CC) * Fz).sum(axis=1)
+            J[:, i] = norm * X0 * (dI0 + X1 * dI1)
+        
+        # ddColor 
+        i = self.pars['Color'].indexof(0)
+        if i>=0:
+            dCC = np.log(self.CC) * CC
+            M0_dCC, M1_dCC = np.matrix(M0.T * dCC), np.matrix(M1.T * dCC)
+            dI0 = (np.array(P * M0_dCC) * Fz).sum(axis=1)
+            dI1 = (np.array(P * M1_dCC) * Fz).sum(axis=1)
+            J[:, i] = norm * X0 * (dI0 + X1 * dI1)
+        
+        # ddz - this one is costly to compute
+        # I don't know how to compute it other than numerically
+        i = self.pars['z'].indexof(0)
+        if i>=0:
+            self.z += dz
+            dflux = self()
+            J[:,i] = (dflux-flux)/dz
+            self.z -= dz
+        
+        return flux, J
+    
+    def deriv_debug(self, p=None):
+        if p is not None:
+            self.pars.free = p 
+        
+        flx0 = self(jac=0)
+
+        n, N = len(self.pars.free), len(self.mjds)
+        J = np.zeros((N,n))        
+        
+        # ddX0
+        self.X0 += 0.01
+        flx = self()
+        J[:, self.pars['X0'].indexof(0)] = (flx-flx0) / 0.01
+        self.X0 -= 0.01
+        # ddX1
+        self.X1 += 0.01
+        flx = self()
+        J[:, self.pars['X1'].indexof(0)] = (flx-flx0) / 0.01
+        self.X1 -= 0.01
+        # ddDayMax 
+        self.DayMax += 0.01
+        flx = self()
+        J[:, self.pars['DayMax'].indexof(0)] = (flx-flx0) / 0.01
+        self.DayMax -= 0.01        
+        # ddColor 
+        self.Color += 0.001
+        flx = self()
+        J[:, self.pars['Color'].indexof(0)] = (flx-flx0) / 0.001
+        self.Color -= 0.001      
+        # ddz
+        self.z += 0.1
+        flx = self()
+        J[:, self.pars['z'].indexof(0)] = (flx-flx0) / 0.01
+        self.z -= 0.1
+
+        return J 
+        
+def test():
+    r = []
+    for sn in sne:
+        r.append(SALT2(sn))
+
+
+
 
-            return var, jacobian_var.T
-        return var
```

### Comparing `sn-nacl-0.3/nacl/plotting/plots.py` & `sn-nacl-0.4/nacl/plotting/plots.py`

 * *Files identical despite different names*

### Comparing `sn-nacl-0.3/nacl/plotting/plottools.py` & `sn-nacl-0.4/nacl/plotting/plottools.py`

 * *Files identical despite different names*

### Comparing `sn-nacl-0.3/nacl/simulations/etc.py` & `sn-nacl-0.4/nacl/simulations/etc.py`

 * *Files 0% similar despite different names*

```diff
@@ -668,15 +668,15 @@
         m = -2.5 * np.log10(flux) + zp
         return m
 
     def mag_to_flux(self, mag, band, zp=None):
         if zp is None:
             zp = self.zero_points(band)
         return np.power(10., -0.4 * (mag-zp))
-        
+
     def flux_variance(self, exptime, flux, skyflux, seeing, band):
         """The variance of PSF fluxes in the requested bands.
 
         Args:
           exptime (float or ndarray of floats): exposure times
           flux (float or ndarray of float, optional): source flux on the focal plane (in e/s)
           skyflux (float or ndarray of float, optional): sly brightness (in e/s/arcsecond^2)
```

### Comparing `sn-nacl-0.3/nacl/simulations/ideal.py` & `sn-nacl-0.4/nacl/simulations/ideal.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,25 @@
 from ..dataset import TrainingDataset
 from ..util import salt2
 
 from math import *
 import astropy.cosmology as cosmology
 
 
+
+def perret_rate(z):
+    """The SNLS SNIa rate according to (Perret et al, 201?)
+    """
+    rate = 0.17E-4
+    expn = 2.11
+    my_z = np.copy(z)
+    my_z[my_z>1.] = 1.
+    return rate * np.power(1+my_z, expn)
+
+
 class Generator(object):
     r"""
     Data generator.
     Generate ideal simulation.
 
     * Parameters of SNe
     For a fixed number of supernovae, we uniformly draw redshifts between :math:`z = 0.001` and :math:`z = 0.8`
@@ -239,14 +250,17 @@
 
         dL is calculated following a flat :math:`\Lambda CDM` and
         :math:`M_b`, :math:`\alpha`, :math:`\beta` are taken from JLA.
         """
         n_sn = self.nb_sn
         np.random.seed(self.seed)
         z = np.random.uniform(self.z_range[0], self.z_range[1], size=floor(n_sn))
+        
+        #        self.cosmo.comoving_volume()
+        
 
         color = np.random.normal(c_dist[0], c_dist[1], size=n_sn)
         sig = np.random.normal(x1_dist[0], x1_dist[1], size=n_sn)
         sig /= sig.std()
         print('X1 removing mean and correct from standard deviation; \n c removing mean')
         sig -= sig.mean()
         color -= color.mean()
```

### Comparing `sn-nacl-0.3/nacl/simulations/reindex.py` & `sn-nacl-0.4/nacl/simulations/reindex.py`

 * *Files identical despite different names*

### Comparing `sn-nacl-0.3/nacl/util/io.py` & `sn-nacl-0.4/nacl/util/io.py`

 * *Files identical despite different names*

### Comparing `sn-nacl-0.3/nacl/util/saltpath.py` & `sn-nacl-0.4/nacl/util/saltpath.py`

 * *Files identical despite different names*

